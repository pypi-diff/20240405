# Comparing `tmp/metricsreport-2024.1.2.tar.gz` & `tmp/metricsreport-2024.4.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metricsreport-2024.1.2.tar", max compression
+gzip compressed data, was "metricsreport-2024.4.17.tar", max compression
```

## Comparing `metricsreport-2024.1.2.tar` & `metricsreport-2024.4.17.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-10-05 13:07:10.366522 metricsreport-2024.1.2/LICENSE
--rw-r--r--   0        0        0     2207 2023-10-05 13:07:10.366522 metricsreport-2024.1.2/README.md
--rw-r--r--   0        0        0       98 2024-01-01 00:09:10.248127 metricsreport-2024.1.2/metricsreport/__init__.py
--rw-r--r--   0        0        0     2749 2023-12-31 22:17:25.169580 metricsreport-2024.1.2/metricsreport/custom_metrics.py
--rw-r--r--   0        0        0    23803 2023-12-31 23:45:16.196473 metricsreport-2024.1.2/metricsreport/metricsreport.py
--rw-r--r--   0        0        0      576 2024-01-01 00:09:33.620708 metricsreport-2024.1.2/pyproject.toml
--rw-r--r--   0        0        0     3077 1970-01-01 00:00:00.000000 metricsreport-2024.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-05 14:51:42.426099 metricsreport-2024.4.17/LICENSE
+-rw-r--r--   0        0        0     2266 2024-04-05 14:55:55.211390 metricsreport-2024.4.17/README.md
+-rw-r--r--   0        0        0       99 2024-04-05 18:52:11.484316 metricsreport-2024.4.17/metricsreport/__init__.py
+-rw-r--r--   0        0        0     2749 2024-04-05 14:51:42.450099 metricsreport-2024.4.17/metricsreport/custom_metrics.py
+-rw-r--r--   0        0        0    28628 2024-04-05 18:51:12.084028 metricsreport-2024.4.17/metricsreport/metricsreport.py
+-rw-r--r--   0        0        0      577 2024-04-05 18:52:08.248300 metricsreport-2024.4.17/pyproject.toml
+-rw-r--r--   0        0        0     3188 1970-01-01 00:00:00.000000 metricsreport-2024.4.17/PKG-INFO
```

### Comparing `metricsreport-2024.1.2/LICENSE` & `metricsreport-2024.4.17/LICENSE`

 * *Files identical despite different names*

### Comparing `metricsreport-2024.1.2/README.md` & `metricsreport-2024.4.17/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 
 following methods can be used to generate plots:
 
 *   `plot_roc_curve()`: Generates a ROC curve plot.
 *   `plot_precision_recall_curve()`: Generates a precision-recall curve plot.
 *   `plot_confusion_matrix()`: Generates a confusion matrix plot.
 *   `plot_class_distribution()`: Generates a class distribution plot.
+*   `plot_class_hist()`: Generates a class histogram plot.
 *   `plot_calibration_curve()`: Generates a calibration curve plot.
 *   `plot_lift_curve()`: Generates a lift curve plot.
 *   `plot_cumulative_gain()`: Generates a cumulative gain curve plot.
 
 ### Dependencies
 
 *   numpy
```

### Comparing `metricsreport-2024.1.2/metricsreport/custom_metrics.py` & `metricsreport-2024.4.17/metricsreport/custom_metrics.py`

 * *Files identical despite different names*

### Comparing `metricsreport-2024.1.2/metricsreport/metricsreport.py` & `metricsreport-2024.4.17/metricsreport/metricsreport.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,23 +15,24 @@
     average_precision_score,
     mean_squared_error,
     mean_absolute_error,
     r2_score,
     explained_variance_score,
     max_error,
     mean_squared_log_error,
-    mean_poisson_deviance
+    mean_poisson_deviance,
+    classification_report,
+    precision_recall_curve,
+    roc_curve
 )
-from sklearn.metrics import classification_report
-from sklearn.metrics import precision_recall_curve
-from sklearn.metrics import confusion_matrix
+
 import scikitplot as skplt
 from plot_metric.functions import BinaryClassification
 import matplotlib.pyplot as plt
-from markdownify import markdownify
+from io import BytesIO
 
 from .custom_metrics import lift, recall_score, f1_score
 
 
 class MetricsReport:
     """
     Class for generating reports on the metrics of a machine learning model.
@@ -68,21 +69,36 @@
         self.threshold = threshold
         self.metrics = {}
         self.target_info = {}
 
         if self.task_type == "classification":
             self.y_pred_binary = (self.y_pred > self.threshold).astype(int)
             # fix for skplt
-            self.probas_reval = pd.DataFrame({"proba_0": 1 - self.y_pred.ravel(), "proba_1": self.y_pred.ravel()})
+            self.probas_reval = pd.DataFrame(data={"proba_0": 1 - self.y_pred.ravel(), "proba_1": self.y_pred.ravel()})
             self.metrics = self._generate_classification_metrics()
         else:
             # assuming y_pred is a numpy array
             self.y_pred_nonnegative = np.maximum(self.y_pred, 0)
             self.metrics = self._generate_regression_metrics()
 
+        self.plots = {
+            "all_count_metrics": self.plot_all_count_metrics,
+            "class_hist": self.plot_class_hist,
+            "tp_fp_with_optimal_threshold": self.plot_tp_fp_with_optimal_threshold,
+            "class_distribution": self.plot_class_distribution,
+            "confusion_matrix": self.plot_confusion_matrix,
+            "precision_recall_curve": self.plot_precision_recall_curve,
+            "roc_curve": self.plot_roc_curve,
+            "ks_statistic": self.plot_ks_statistic,
+            "calibration_curve": self.plot_calibration_curve,
+            "cumulative_gain": self.plot_cumulative_gain,
+            "precision_recall_vs_threshold": self.plot_precision_recall_vs_threshold,
+            "lift_curve": self.plot_lift_curve
+            }
+
     def _determine_task_type(self, y_true) -> str:
         """
         Determines the type of task based on the number of unique values in y_true.
 
         Args:
             y_true: A list of true target values.
 
@@ -92,126 +108,228 @@
         if len(np.unique(y_true)) > 2:
             return "regression"
         else:
             return "classification"
 
     ########## classification ###################################################
 
-    def _generate_classification_metrics(self):
+    def _generate_classification_metrics(self) -> dict:
         """
         Generates a dictionary of classification metrics.
 
         Returns:
             A dictionary of classification metrics.
         """
-        tn, fp, fn, tp = confusion_matrix(self.y_true, self.y_pred_binary).ravel()
+        tn, fp, fn, tp = confusion_matrix(y_true=self.y_true, y_pred=self.y_pred_binary).ravel()
+        report = classification_report(
+            y_true=self.y_true, 
+            y_pred=self.y_pred_binary, 
+            output_dict=True, 
+            labels=[0, 1], 
+            target_names=['negative', 'positive'], 
+            zero_division='warn'
+            )
+        report = pd.json_normalize(report, sep=' ').to_dict(orient='records')[0]
 
         metrics = {
+            'AP': round(average_precision_score(self.y_true, self.y_pred), 4),
             'AUC': round(roc_auc_score(self.y_true, self.y_pred), 4),
             'Log Loss': round(log_loss(self.y_true, self.y_pred), 4),
-            'Average_Precision': round(average_precision_score(self.y_true, self.y_pred), 4),
-            'Accuracy': round(accuracy_score(self.y_true, self.y_pred_binary), 4),
-            'Precision': round(precision_score(self.y_true, self.y_pred_binary, average='weighted'), 4),
-            'Recall': round(recall_score(self.y_true, self.y_pred_binary, average='weighted'), 4),
-            'F1 Score': round(f1_score(self.y_true, self.y_pred_binary, average='weighted'), 4),
+            'MSE': round(mean_squared_error(self.y_true, self.y_pred), 4),
+            'Accuracy': round(accuracy_score(self.y_true, self.y_pred_binary,), 4),
+            'Precision_weighted': round(precision_score(self.y_true, self.y_pred_binary, average='weighted'), 4),
             'MCC': round(matthews_corrcoef(self.y_true, self.y_pred_binary), 4),
             'TN': tn,
             'FP': fp,
             'FN': fn,
             'TP': tp,
+            'P precision': round(report['positive precision'], 4),
+            'P recall': round(report['positive recall'], 4),
+            'P f1-score': round(report['positive f1-score'], 4),
+            'P support': report['positive support'],
+            'N precision': round(report['negative precision'], 4),
+            'N recall': round(report['negative recall'], 4),
+            'N f1-score': round(report['negative f1-score'], 4),
+            'N support': report['negative support'],
+            #'Recall_weighted': round(recall_score(self.y_true, self.y_pred_binary, average='weighted'), 4),
+            #'F1_weighted': round(f1_score(self.y_true, self.y_pred_binary, average='weighted'), 4),
         }
         return metrics
     
-    def plot_roc_curve(self, figsize = (12, 10)) -> plt:
+    def plot_roc_curve(self, figsize = (15, 10)) -> plt:
         """
         Generates a ROC curve plot.
 
         Args:
             figsize: the width and height of the figure.
 
         Returns:
             A ROC curve plot.
         """
-        bc = BinaryClassification(self.y_true, self.y_pred, labels=["Class 1", "Class 2"])
+        bc = BinaryClassification(y_true=self.y_true, y_pred=self.y_pred, labels=["Class 1", "Class 2"])
         plt.figure(figsize=figsize)
         bc.plot_roc_curve()
         return plt
     
-    def plot_precision_recall_curve(self, figsize = (12, 10)) -> plt:
+    def plot_precision_recall_curve(self, figsize = (15, 10)) -> plt:
         """
         Generates a precision recall curve plot.
 
         Args:
             figsize: A tuple of the width and height of the figure.
 
         Returns:
             A precision recall curve plot.
         """
-        bc = BinaryClassification(self.y_true, self.y_pred, labels=["Class 1", "Class 2"])
+        bc = BinaryClassification(y_true=self.y_true, y_pred=self.y_pred, labels=["Class 1", "Class 2"])
         plt.figure(figsize=figsize)
         bc.plot_precision_recall_curve()
         return plt
     
-    def plot_confusion_matrix(self, figsize = (12, 10)) -> plt:
+    def plot_confusion_matrix(self, figsize = (15, 10)) -> plt:
         """
         Generates a confusion matrix plot.
 
         Args:
             figsize: A tuple of the width and height of the figure.
 
         Returns:
             A confusion matrix plot.
         """
-        bc = BinaryClassification(self.y_true, self.y_pred, labels=["Class 1", "Class 2"])
+        bc = BinaryClassification(y_true=self.y_true, y_pred=self.y_pred, labels=["Class 1", "Class 2"])
         plt.figure(figsize=figsize)
         bc.plot_confusion_matrix()
         return plt
     
-    def plot_class_distribution(self, figsize = (12, 10)) -> plt:
+    def plot_class_distribution(self, figsize = (15, 10)) -> plt:
         """
         Generates a class distribution plot.
 
         Args:
             figsize: A tuple of the width and height of the figure.
 
         Returns:
             A class distribution plot.
         """
-        bc = BinaryClassification(self.y_true, self.y_pred, labels=["Class 1", "Class 2"])
+        bc = BinaryClassification(y_true=self.y_true, y_pred=self.y_pred, labels=["Class 1", "Class 2"])
         plt.figure(figsize=figsize)
         bc.plot_class_distribution()
         return plt
     
-    def plot_calibration_curve(self, figsize = (12, 10)) -> plt:
+    def plot_class_hist(self, figsize = (15, 10)) -> plt:
+        """
+        Generates a class histogram plot, showing the distribution of predicted probabilities
+        for each actual class label.
+
+        Args:
+            figsize: A tuple of the width and height of the figure.
+
+        Returns:
+            A matplotlib figure with the histogram plot.
+        """
+        plt.style.use('ggplot')
+        plt.figure(figsize=figsize)
+
+        # Отдельные предсказания для классов 0 и 1
+        preds_for_true_0 = [pred for pred, true in zip(self.y_pred, self.y_true) if true == 0]
+        preds_for_true_1 = [pred for pred, true in zip(self.y_pred, self.y_true) if true == 1]
+
+        # Гистограмма для класса 0
+        plt.hist(preds_for_true_0, bins=100, edgecolor='black', alpha=0.5, label='Class 0')
+
+        # Гистограмма для класса 1
+        plt.hist(preds_for_true_1, bins=100, edgecolor='black', alpha=0.5, label='Class 1')
+
+        plt.axvline(x=self.threshold, color='r', linestyle='--', label=f'Threshold: {self.threshold}')
+
+        plt.xlabel('Predicted Probability')
+        plt.ylabel('Frequency')
+        plt.title('Predicted Probability Histogram by Class')
+        plt.legend()
+        return plt
+    
+    def plot_all_count_metrics(self, step=101, plot_count_coef=1e-2, figsize=(15, 10)) -> plt:
+        """
+        Generates a plot of accuracy, precision, recall, and class distribution as a function of the decision threshold.
+
+        Args:
+            step: The number of steps to take between 0 and 1.
+            plot_count_coef: The coefficient to multiply the count by in the scoring rule.
+            figsize: A tuple of the width and height of the figure.
+
+        Returns:
+            A plot of accuracy, precision, recall, and class distribution as a function of the decision threshold.
+        """
+        plt.style.use('ggplot')
+        plt.figure(figsize=figsize)
+        accuracy_score_list = []
+        precision_score_list = []
+        recall_score_list = []
+        list_classes = []
+        list_counts = []
+
+        pred_prob = np.array(self.y_pred)
+        target = np.array(self.y_true, dtype=int)
+
+        thresholds = np.linspace(0, 1, step)[:-1]
+        for i in thresholds:
+            predicted_labels = pred_prob > i
+
+            accuracy_score_list.append(accuracy_score(target, predicted_labels))
+            precision_score_list.append(precision_score(target, predicted_labels,))
+            recall_score_list.append(recall_score(target, predicted_labels,))
+            list_classes.append(predicted_labels.sum() / len(predicted_labels))
+            list_counts.append(predicted_labels.sum())
+
+        plt.plot(thresholds, accuracy_score_list, label='Accuracy')
+        plt.plot(thresholds, precision_score_list, label='Precision')
+        plt.plot(thresholds, recall_score_list, label='Recall')
+        plt.plot(thresholds, list_classes, label='Class 1 count', color='black', linestyle='--')
+        plt.axvline(x=self.threshold, color='r', linestyle='--', label=f'Threshold: {self.threshold}')
+
+        min_count, max_count = min(list_counts), max(list_counts)
+        for i, count in enumerate(list_counts):
+            if (i % (len(list_counts) // 80) == 0 or count in (min_count, max_count)) and (list_counts[i-1] / list_counts[i]) - 1 > plot_count_coef:
+                y_offset = list_classes[i] + (max(list_classes) - min(list_classes)) * 0.02
+                plt.text(thresholds[i], y_offset, str(count), fontsize=7, rotation=90, fontweight='bold')
+
+        plt.xlabel('Threshold')
+        plt.ylabel('Scores')
+        plt.title(f'accuracy, precision, recall, and class distribution')
+        plt.legend()
+        plt.grid(True)
+        return plt
+    
+    def plot_calibration_curve(self, figsize = (15, 10)) -> plt:
         """
         Generates a calibration curve plot.
 
         Args:
             figsize: A tuple of the width and height of the figure.
 
         Returns:
             A calibration curve plot.
         """
         skplt.metrics.plot_calibration_curve(self.y_true, [self.probas_reval], n_bins=10, figsize=figsize)
         return plt
     
-    def plot_lift_curve(self, figsize = (12, 10)) -> plt:
+    def plot_lift_curve(self, figsize = (15, 10)) -> plt:
         """
         Generates a lift curve plot.
 
         Args:
             figsize: A tuple of the width and height of the figure.
 
         Returns:
             A lift curve plot.
         """
         skplt.metrics.plot_lift_curve(self.y_true, self.probas_reval, figsize=figsize)
         return plt
     
-    def plot_cumulative_gain(self, figsize = (12, 10)) -> plt:
+    def plot_cumulative_gain(self, figsize = (15, 10)) -> plt:
         """
         Generates a cumulative gain curve plot.
 
         Args:
             figsize: A tuple of the width and height of the figure.
 
         Returns:
@@ -230,15 +348,15 @@
         Returns:
             A KS statistic plot.
         """
         skplt.metrics.plot_ks_statistic(self.y_true, self.probas_reval, figsize=figsize)
         return plt
     
 
-    def plot_precision_recall_vs_threshold(self, fp_coefficient: int =1, figsize=(12, 10)):
+    def plot_precision_recall_vs_threshold(self, fp_coefficient: int =1, figsize=(15, 10)):
         """
         Plots Precision and Recall as a function of the decision threshold.
 
         Args:
             fp_coefficient (int): The coefficient to multiply FP by in the scoring rule.
             figsize (tuple): Figure size.
 
@@ -268,15 +386,14 @@
         
         optimal_idx = np.argmax(Scores_list)
         optimal_threshold = thresholds[optimal_idx]
 
         # Calculate precision and recall for various thresholds
         precision, recall, thresholds = precision_recall_curve(y_true, probas_pred)
         
-        
         # Create the plot
         plt.figure(figsize=figsize)
         plt.plot(thresholds, precision[:-1], "b--", label="Precision")
         plt.plot(thresholds, recall[:-1], "g-", label="Recall")
         # Highlighting the best threshold
         plt.scatter([optimal_threshold], [precision[optimal_idx]], color="blue", marker='o', label=f"Best for Precision: {optimal_threshold:.2f}")
         plt.scatter([optimal_threshold], [recall[optimal_idx]], color="green", marker='x', label=f"Best for Recall: {optimal_threshold:.2f}")
@@ -286,15 +403,15 @@
         plt.ylabel("Metrics")
         plt.legend(loc="best")
         plt.title("Precision and Recall as a function of the decision threshold")
         plt.grid(True)
         
         return plt
     
-    def plot_tp_fp_with_optimal_threshold(self, fp_coefficient: int =1, figsize=(12, 10)):
+    def plot_tp_fp_with_optimal_threshold(self, fp_coefficient: int =1, figsize=(15, 10)):
         """
         Plots the True Positives (TP) and False Positives (FP) rates across different thresholds and
         identifies the optimal threshold based on a scoring rule (TP - 2*FP).
 
         Args:
             fp_coefficient (int): The coefficient to multiply FP by in the scoring rule.
             figsize (tuple): Figure size.
@@ -354,28 +471,15 @@
             None.
         """
         if save:
             if os.path.exists(folder+'/plots'):
                 shutil.rmtree(folder+'/plots')
             os.makedirs(folder+'/plots')
 
-        plots = {
-            "class_distribution": self.plot_class_distribution,
-            "confusion_matrix": self.plot_confusion_matrix,
-            "precision_recall_curve": self.plot_precision_recall_curve,
-            "roc_curve": self.plot_roc_curve,
-            "ks_statistic": self.plot_ks_statistic,
-            "calibration_curve": self.plot_calibration_curve,
-            "cumulative_gain": self.plot_cumulative_gain,
-            "precision_recall_vs_threshold": self.plot_precision_recall_vs_threshold,
-            "tp_fp_with_optimal_threshold": self.plot_tp_fp_with_optimal_threshold,
-            "lift_curve": self.plot_lift_curve
-            }
-
-        for plot_name, plot_func in plots.items():
+        for plot_name, plot_func in self.plots.items():
             plt = plot_func()
             if save:
                 plt.savefig(f'{folder}/plots/{plot_name}.png')
             else:
                 plt.show()
             plt.close()
 
@@ -395,15 +499,15 @@
             'R^2': round(r2_score(self.y_true, self.y_pred), 4),
             'Explained Variance Score': round(explained_variance_score(self.y_true, self.y_pred), 4),
             'Max Error': round(max_error(self.y_true, self.y_pred), 4),
             'Mean Absolute Percentage Error': round(np.mean(np.abs((self.y_true - self.y_pred) / self.y_true)) * 100, 1),
         }
         return metrics
     
-    def plot_residual_plot(self, figsize = (12, 10)) -> plt:
+    def plot_residual_plot(self, figsize = (15, 10)) -> plt:
         """
         Generates a residual plot.
 
         Args:
             figsize: Figure size for plot.
 
         Returns:
@@ -412,15 +516,15 @@
         plt.figure(figsize=figsize)
         plt.scatter(self.y_pred, self.y_true - self.y_pred)
         plt.xlabel("Predicted Values")
         plt.ylabel("Residuals")
         plt.title("Residual Plot")
         return plt
     
-    def plot_predicted_vs_actual(self, figsize = (12, 10)) -> plt:
+    def plot_predicted_vs_actual(self, figsize = (15, 10)) -> plt:
         """
         Generates a predicted vs actual plot.
 
         Args:
             figsize: Figure size for plot.
 
         Returns:
@@ -559,19 +663,42 @@
                         </tr>
                     </thead>
                     <tbody>
                         {self.__generate_html_rows(self.metrics)}
                     </tbody>
                 </table>
                 <h2>Plots</h2>
-                {self.__add_plot_images_to_report(folder)}
+                {self.add_svg_plots_to_html_rows()}
             </body>
         </html>
         """
         return html
+    
+    def add_svg_plots_to_html_rows(self, figsize = (15, 10)) -> str:
+        """
+        Adds SVG plots to HTML rows.
+
+        Args:
+            plots: A dictionary containing the SVG plots.
+
+        Returns:
+            A string containing the HTML rows with the SVG plots.
+        """
+        rows = ''
+        for name, plot in self.plots.items():
+            plt = plot(figsize=figsize)
+            # Создаем объект BytesIO в памяти
+            svg_io = BytesIO()
+            # Сохраняем график в формате SVG в объект BytesIO
+            plt.savefig(svg_io, format='svg', bbox_inches='tight')
+            # Получаем содержимое объекта BytesIO и декодируем его в строку
+            svg = '<svg' + svg_io.getvalue().decode('utf-8').split('<svg')[1]
+            plt.close()
+            rows += f'<tr><td>{svg}<br></td></tr>\n'
+        return rows
 
     def __generate_html_rows(self, data: dict) -> str:
         """
         Generates HTML rows.
 
         Args:
             data: A dictionary containing the data to be displayed.
@@ -580,58 +707,37 @@
             A string containing the HTML rows.
         """
         rows = ''
         for name, value in data.items():
             rows += f'<tr><td>{name}</td><td>{value}</td></tr>\n' if isinstance(value, float) else f'<tr><td>{name}</td><td>{int(value)}</td></tr>\n'
         return rows
 
-    def __add_plot_images_to_report(self, folder='report_metrics',) -> str:
-        """
-        Generates HTML image tags for each plot.
-
-        Returns:
-            A string containing the HTML or markdown image tags for each plot.
-        """
-        images = ''
-        directory = f'{folder}/plots/'
-        png_files = [file for file in os.listdir(directory) if file.endswith('.png')]
-
-        for name in png_files:
-            images += f'<img src="./plots/{name}"></br>\n'
-        return images
-
-    def save_report(self, folder: str = 'report_metrics', name: str = 'report_metrics') -> None:
+    def save_report(self, folder: str = 'report_metrics', name: str = 'report_metrics', verbose=0) -> None:
         """
         Creates and saves a report in HTML or markdown format.
 
         Args:
             folder (str): The folder to save the report to.
             name (str): The name of the report.
         """
         # Create the report directory
         if folder != '.':
-            if os.path.exists(folder):
-                shutil.rmtree(folder)
-            os.makedirs(folder)
+            if not os.path.exists(folder):
+                os.makedirs(folder)
         # Get target info
         self.__target_info()
-        # Generate plots based on task type
-        if self.task_type == 'classification':
-            self._classification_plots(save=True, folder=folder)
-        elif self.task_type == 'regression':
-            self._regression_plots(save=True, folder=folder)
         # Generate HTML report
         html = self._generate_html_report(folder, add_css=True)
-        with open(f'{folder}/{name}.html', 'w') as f:
+
+        file_path = f'{folder}/{name}.html'
+        with open(file_path, 'w') as f:
             f.write(html)
-        # Convert HTML report to markdown
-        md = markdownify(self._generate_html_report(folder, add_css=False), heading_style="ATX")
-        with open(f'{folder}/{name}.md', 'w') as f:
-            f.write(md)
-        print(f'Report saved in folder: {folder}')
+
+        if verbose > 0:
+            print(f'Report saved in folder: {folder}')
 
     def print_metrics(self) -> None:
         """
         Prints the metrics dictionary.
         """
         print(pd.DataFrame(self.metrics, index=['score']).T)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `metricsreport-2024.1.2/pyproject.toml` & `metricsreport-2024.4.17/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metricsreport"
-version = "2024.1.2"
+version = "2024.4.17"
 description = "Generating reports on metrics for Machine Learning models"
 authors = ["Alex Lekov <11148364-AlexLekov@users.noreply.gitlab.com>"]
 repository = 'https://github.com/Alex-Lekov/metricsreport'
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `metricsreport-2024.1.2/PKG-INFO` & `metricsreport-2024.4.17/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: metricsreport
-Version: 2024.1.2
+Version: 2024.4.17
 Summary: Generating reports on metrics for Machine Learning models
 Home-page: https://github.com/Alex-Lekov/metricsreport
 Author: Alex Lekov
 Author-email: 11148364-AlexLekov@users.noreply.gitlab.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: markdownify (>=0.11.6,<0.12.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: plot-metric (>=0.0.6,<0.0.7)
 Requires-Dist: scikit-learn (>=1.3.0,<2.0.0)
 Requires-Dist: scikit-plot (>=0.3.7,<0.4.0)
 Project-URL: Repository, https://github.com/Alex-Lekov/metricsreport
 Description-Content-Type: text/markdown
@@ -90,14 +91,15 @@
 
 following methods can be used to generate plots:
 
 *   `plot_roc_curve()`: Generates a ROC curve plot.
 *   `plot_precision_recall_curve()`: Generates a precision-recall curve plot.
 *   `plot_confusion_matrix()`: Generates a confusion matrix plot.
 *   `plot_class_distribution()`: Generates a class distribution plot.
+*   `plot_class_hist()`: Generates a class histogram plot.
 *   `plot_calibration_curve()`: Generates a calibration curve plot.
 *   `plot_lift_curve()`: Generates a lift curve plot.
 *   `plot_cumulative_gain()`: Generates a cumulative gain curve plot.
 
 ### Dependencies
 
 *   numpy
```

