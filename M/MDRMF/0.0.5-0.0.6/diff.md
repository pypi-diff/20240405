# Comparing `tmp/MDRMF-0.0.5.tar.gz` & `tmp/MDRMF-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MDRMF-0.0.5.tar", last modified: Wed Sep 13 08:06:01 2023, max compression
+gzip compressed data, was "MDRMF-0.0.6.tar", last modified: Fri Apr  5 07:24:24 2024, max compression
```

## Comparing `MDRMF-0.0.5.tar` & `MDRMF-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-09-13 08:06:01.498413 MDRMF-0.0.5/
-drwxrwxrwx   0        0        0        0 2023-09-13 08:06:01.462411 MDRMF-0.0.5/MDRMF/
--rw-rw-rw-   0        0        0      284 2023-09-13 08:03:40.000000 MDRMF-0.0.5/MDRMF/__init__.py
--rw-rw-rw-   0        0        0     3942 2023-09-12 19:22:27.000000 MDRMF-0.0.5/MDRMF/dataset.py
--rw-rw-rw-   0        0        0     2002 2023-06-09 10:42:18.000000 MDRMF-0.0.5/MDRMF/evaluator.py
--rw-rw-rw-   0        0        0     7639 2023-09-13 06:33:18.000000 MDRMF-0.0.5/MDRMF/experimenter.py
--rw-rw-rw-   0        0        0     3808 2023-06-09 10:44:26.000000 MDRMF-0.0.5/MDRMF/featurizer.py
--rw-rw-rw-   0        0        0     1727 2023-06-06 08:00:32.000000 MDRMF-0.0.5/MDRMF/model.py
-drwxrwxrwx   0        0        0        0 2023-09-13 08:06:01.494424 MDRMF-0.0.5/MDRMF/models/
--rw-rw-rw-   0        0        0       86 2023-05-23 10:56:06.000000 MDRMF-0.0.5/MDRMF/models/__init__.py
--rw-rw-rw-   0        0        0     4113 2023-09-13 06:29:52.000000 MDRMF-0.0.5/MDRMF/models/modeller.py
--rw-rw-rw-   0        0        0     4418 2023-09-13 06:44:40.000000 MDRMF-0.0.5/MDRMF/models/rfmodeller.py
--rw-rw-rw-   0        0        0     2643 2023-06-02 14:00:31.000000 MDRMF-0.0.5/MDRMF/moleculeloader.py
-drwxrwxrwx   0        0        0        0 2023-09-13 08:06:01.487416 MDRMF-0.0.5/MDRMF.egg-info/
--rw-rw-rw-   0        0        0      436 2023-09-13 08:06:01.000000 MDRMF-0.0.5/MDRMF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-09-13 08:06:01.000000 MDRMF-0.0.5/MDRMF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-13 08:06:01.000000 MDRMF-0.0.5/MDRMF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-09-13 08:06:01.000000 MDRMF-0.0.5/MDRMF.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      436 2023-09-13 08:06:01.497562 MDRMF-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-05-11 07:27:32.000000 MDRMF-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-09-13 08:06:01.498413 MDRMF-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      553 2023-09-13 08:05:31.000000 MDRMF-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:24:24.570031 MDRMF-0.0.6/
+drwxrwxrwx   0        0        0        0 2024-04-05 07:24:24.486540 MDRMF-0.0.6/MDRMF/
+-rw-rw-rw-   0        0        0      374 2024-04-05 07:23:24.000000 MDRMF-0.0.6/MDRMF/__init__.py
+-rw-rw-rw-   0        0        0    10824 2024-03-05 09:03:49.000000 MDRMF-0.0.6/MDRMF/configvalidator.py
+-rw-rw-rw-   0        0        0    14769 2024-02-27 06:57:27.000000 MDRMF-0.0.6/MDRMF/dataset.py
+-rw-rw-rw-   0        0        0      698 2023-11-29 06:20:37.000000 MDRMF-0.0.6/MDRMF/datasetflagged.py
+-rw-rw-rw-   0        0        0     3273 2024-01-18 14:12:49.000000 MDRMF-0.0.6/MDRMF/evaluator.py
+-rw-rw-rw-   0        0        0     3261 2024-01-05 13:16:29.000000 MDRMF-0.0.6/MDRMF/evaluator_old.py
+-rw-rw-rw-   0        0        0    21654 2024-03-05 11:18:21.000000 MDRMF-0.0.6/MDRMF/experimenter.py
+-rw-rw-rw-   0        0        0     5643 2024-04-05 07:21:35.000000 MDRMF-0.0.6/MDRMF/featurizer.py
+-rw-rw-rw-   0        0        0     1936 2024-03-05 09:01:29.000000 MDRMF-0.0.6/MDRMF/model.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:24:24.565030 MDRMF-0.0.6/MDRMF/models/
+-rw-rw-rw-   0        0        0      398 2024-01-03 12:44:45.000000 MDRMF-0.0.6/MDRMF/models/__init__.py
+-rw-rw-rw-   0        0        0     4692 2023-10-31 20:10:04.000000 MDRMF-0.0.6/MDRMF/models/dtmodeller.py
+-rw-rw-rw-   0        0        0     4769 2023-10-30 11:17:20.000000 MDRMF-0.0.6/MDRMF/models/knnmodeller.py
+-rw-rw-rw-   0        0        0     4537 2023-10-30 11:48:56.000000 MDRMF-0.0.6/MDRMF/models/lgbmmodeller.py
+-rw-rw-rw-   0        0        0     4552 2023-10-30 13:20:54.000000 MDRMF-0.0.6/MDRMF/models/mlprmodeller.py
+-rw-rw-rw-   0        0        0    12175 2024-03-05 11:16:43.000000 MDRMF-0.0.6/MDRMF/models/modeller.py
+-rw-rw-rw-   0        0        0    14938 2024-03-05 09:27:31.000000 MDRMF-0.0.6/MDRMF/models/rfmodeller.py
+-rw-rw-rw-   0        0        0    13815 2024-01-18 12:36:35.000000 MDRMF-0.0.6/MDRMF/models/rfmodeller_pairwise.py
+-rw-rw-rw-   0        0        0     4650 2023-11-02 06:40:44.000000 MDRMF-0.0.6/MDRMF/models/rfmodeller_vanilla.py
+-rw-rw-rw-   0        0        0     4705 2023-10-30 10:26:08.000000 MDRMF-0.0.6/MDRMF/models/svrmodeller.py
+-rw-rw-rw-   0        0        0     2643 2023-11-30 10:49:11.000000 MDRMF-0.0.6/MDRMF/moleculeloader.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:24:24.528427 MDRMF-0.0.6/MDRMF.egg-info/
+-rw-rw-rw-   0        0        0      436 2024-04-05 07:24:24.000000 MDRMF-0.0.6/MDRMF.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      630 2024-04-05 07:24:24.000000 MDRMF-0.0.6/MDRMF.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 07:24:24.000000 MDRMF-0.0.6/MDRMF.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-05 07:24:24.000000 MDRMF-0.0.6/MDRMF.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      436 2024-04-05 07:24:24.568031 MDRMF-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-05-11 07:27:32.000000 MDRMF-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-05 07:24:24.570314 MDRMF-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      553 2024-04-05 07:23:54.000000 MDRMF-0.0.6/setup.py
```

### Comparing `MDRMF-0.0.5/MDRMF/evaluator.py` & `MDRMF-0.0.6/MDRMF/evaluator_old.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,33 +5,45 @@
 
 class Evaluator:
     def __init__(self, original_dataset, metrics, k_values):
         self.dataset = copy.deepcopy(original_dataset)
         self.metrics = metrics
         self.k_values = [int(k) for k in k_values]
 
-    def evaluate(self, model, model_dataset):
+    def evaluate(self, model, eval_dataset, model_dataset):
+        self.dataset = eval_dataset.copy() #
         results = {}
         for metric in self.metrics:
             if metric == "R2_model":
-                results[metric] = self.r2_model(model, model_dataset)
+                results[metric] = self.r2_model(model, eval_dataset)
             else:
                 for k in self.k_values:
                     if metric == "top-k":
-                        results[f"top-{k}"] = self.top_n_correct(k, model)
+                        results[f"top-{k} model"] = self.top_n_correct(k, model, model_dataset)
                     elif metric == "R2_k":
-                        results[f"R2_k-{k}"] = self.r2_n(k, model)
+                        results[f"R2_k-{k}"] = self.r2_n(k, model, model_dataset)
+                    elif metric == "top-k-acquired":
+                        results[f"top-{k} acquired"] = self.top_n_in_model_set(k, model_dataset)
         return results
 
-    def top_n_correct(self, n, model):
-        model_predictions = model.predict(self.dataset)
-        correct_preds_indices = np.argsort(model_predictions)[:n]
-        top_n_real_indices = np.argsort(self.dataset.y)[:n]
-        return np.mean(np.isin(correct_preds_indices, top_n_real_indices))
+    def top_n_correct(self, n, model, model_dataset):
 
+        model_predictions = model.predict(self.dataset, model_dataset) # Predict on the full dataset
+        preds_indices = np.argsort(model_predictions)[:n] # Sort all predictions from lowest to highest and gets the indices of n amount of mols
+        top_n_real_indices = np.argsort(self.dataset.y)[:n] # Get the indices of the n "real" mols and sorts them from lowest to highest
+        return np.mean(np.isin(preds_indices, top_n_real_indices)) # np.isin calculates how many from the correct_preds_indices that are in top_n_real_indices and np.mean makes this a fraction
+    
+    def top_n_in_model_set(self, n, model_dataset):
+        lowest_y_indices = np.argsort(self.dataset.y)[:n]  # Get indices of the 'n' lowest y values.
+        lowest_y_ids = set(self.dataset.ids[lowest_y_indices])  # Retrieve corresponding IDs from the dataset and ensure uniqueness.
+
+        ids_acquired = set(model_dataset.ids)  # Retrieve unique ids from the internal model dataset.
+        intersection_count = len(lowest_y_ids.intersection(ids_acquired))  # Count of common ids between lowest_y_ids and ids_acquired.
+        
+        return intersection_count / n  # Return the proportion of top 'n' found in the model_dataset.  
 
     def r2_model(self, model, model_dataset):
         '''
         Returns the R2 value of the internal model
         '''
 
         # Find missing points in the model_dataset
@@ -39,19 +51,18 @@
 
         y_true = training_points.y
         y_pred = model.predict(training_points)
 
         return r2_score(y_true, y_pred)
     
 
-    def r2_n(self, n, model):
+    def r2_n(self, n, model, model_dataset):
         # Similar to top_n_correct but here we calculate the r2 score for the top n points
-        model_predictions = model.predict(self.dataset)
+        model_predictions = model.predict(self.dataset, model_dataset)
         top_n_pred_indices = np.argsort(model_predictions)[:n]
 
         # Get top n points as a Dataset
         top_n_dataset = self.dataset.get_points(top_n_pred_indices)
 
         y_pred = model.predict(top_n_dataset)
         
-        return r2_score(top_n_dataset.y, y_pred)
-
+        return r2_score(top_n_dataset.y, y_pred)
```

### Comparing `MDRMF-0.0.5/MDRMF/model.py` & `MDRMF-0.0.6/MDRMF/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,42 +17,53 @@
         Initializes a Model object with the provided Modeller object.
 
         Parameters:
             model (Modeller): The Modeller object to wrap.
         """
         self.model = model
 
+
     def train(self):
         """
         Trains the wrapped Modeller object.
         """
         self.model.fit()
 
+
     def predict(self, dataset: Dataset):
         """
         Generates predictions using the wrapped Modeller object.
 
         Parameters:
             dataset (Dataset): The dataset object containing the data to predict on.
 
         Returns:
             The predictions generated by the wrapped Modeller object.
         """
         return self.model.predict(dataset)
 
+
+    def get_acquired_points(self, unlabeled_dataset):
+        return self.model.unlabeled_acquisition(self.model, unlabeled_dataset)
+
     @property
     def results(self):
         """
         Property that returns the results of the wrapped Modeller object.
 
         Returns:
             dict: A dictionary containing the results of the model's evaluations.
         """
         return self.model.results
-    
+
+
+    def model_graphs(self):
+        return self.model.figures
+
+
     def save(self, filename: str):
         """
         Save the wrapped Modeller object to a pickle file
         """
         self.model.save(filename)
```

### Comparing `MDRMF-0.0.5/MDRMF/models/rfmodeller.py` & `MDRMF-0.0.6/MDRMF/models/mlprmodeller.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,94 +1,91 @@
 import logging
 import pickle
 import os
-from sklearn.ensemble import RandomForestRegressor
+import numpy as np
+from sklearn.neural_network import MLPRegressor
 from MDRMF.models.modeller import Modeller
 from MDRMF.dataset import Dataset
 
-class RFModeller(Modeller):
+class MLPRModeller(Modeller):
 
     def __init__(
         self, 
-        dataset, 
+        dataset,
         evaluator=None, 
         iterations=10, 
         initial_sample_size=10, 
         acquisition_size=10, 
         acquisition_method="greedy", 
         retrain=True,
         seeds=[],
         **kwargs) -> None:
 
         super().__init__(
             dataset, 
-            evaluator, 
+            evaluator,
             iterations, 
             initial_sample_size, 
             acquisition_size, 
             acquisition_method, 
             retrain,
             seeds
             )
 
         self.kwargs = kwargs
-        self.model = RandomForestRegressor(**self.kwargs)
+        self.model = MLPRegressor(**self.kwargs)
 
     def fit(self):
-        
-        # Get random points
-        if self.seeds == []:
-            initial_pts = self._initial_sampler()
-        
-        # If freeze_sample is not empty and it's a list of integers use this as starting points
-        elif self.seeds and isinstance(self.seeds, list) and all(isinstance(i, int) for i in self.seeds):
-
-            # Get the seeded points and remember to remove them from the dataset
+        if self.seeds is None or len(self.seeds) == 0:
+            initial_pts = self._initial_sampler(initial_sample_size=self.initial_sample_size)
+        elif isinstance(self.seeds, (list, np.ndarray)) and all(isinstance(i, int) for i in self.seeds):
+            self.seeds = list(self.seeds)  # Ensure seeds is a list
             initial_pts = self.dataset.get_points(self.seeds, remove_points=True)
-
         else:
-            logging.error("Seeds failed. Seeds must be a list of integers like [5, 25, 600, 5000]")
+            logging.error("Invalid seeds. Must be a list or ndarray of integers, or None.")
+            return
         
         print(f"y values of starting points {initial_pts.y}")
-        self.model.fit(initial_pts.X, initial_pts.y)
+        self.model.fit(initial_pts.X, initial_pts.y)        
+        
+        # First evaluation, using only the initial points
+        if self.evaluator is not None:
+            self.call_evaluator(i=-1, model_dataset=initial_pts) # -1 because ´call_evaluator´ starts at 1, and this iteration should be 0.
 
         for i in range(self.iterations):
         # Acquire new points
             acquired_pts = self._acquisition(self.model)
 
             # Merge old and new points
             if i == 0:
                 model_dataset = self.dataset.merge_datasets([initial_pts, acquired_pts])
             else:
                 model_dataset = self.dataset.merge_datasets([model_dataset, acquired_pts])
 
             if self.retrain:
                 # Reset model and train
-                self.model = RandomForestRegressor(**self.kwargs)
+                self.model = MLPRegressor(**self.kwargs)
                 self.model.fit(model_dataset.X, model_dataset.y)
             else:
                 # Train on existing model
                 self.model.fit(model_dataset.X, model_dataset.y)
 
             if self.evaluator is not None:
-                self.call_evaluator(i=i)
+                self.call_evaluator(i=i, model_dataset=model_dataset)
 
         return self.model
     
     def predict(self, dataset: Dataset):
 
         if isinstance(dataset, Dataset):
             return self.model.predict(dataset.X)
         else:
             logging.error("Wrong object type. Must be of type `Dataset`")
 
     def save(self, filename: str):
-        """
-        Save the RFModeller to a pickle file
-        """
         # Check if filename is a string.
         if not isinstance(filename, str):
             raise ValueError("filename must be a string")
         
         try:
             with open(filename, "wb") as f:
                 pickle.dump(self, f)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `MDRMF-0.0.5/MDRMF/moleculeloader.py` & `MDRMF-0.0.6/MDRMF/moleculeloader.py`

 * *Files identical despite different names*

### Comparing `MDRMF-0.0.5/setup.py` & `MDRMF-0.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='MDRMF',
-    version='0.0.5',
+    version='0.0.6',
     packages=find_packages(),
     description='Multidrug Resistance Machine Fishing',
     author='Jacob Molin Nielsen',
     author_email='jacob.molin@me.com',
     url='https://github.com/MolinDiscovery/MDRMF',  # use the URL to the github repo
-    download_url='https://github.com/MolinDiscovery/MDRMF/archive/v0.0.5.tar.gz',
+    download_url='https://github.com/MolinDiscovery/MDRMF/archive/v0.0.6.tar.gz',
     keywords=['machine fishing', 'drug discovery', 'machine learning', 'pool based active learning'],
     classifiers=[],
 )
```

