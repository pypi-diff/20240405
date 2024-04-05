# Comparing `tmp/pyrtz2-1.1.17.tar.gz` & `tmp/pyrtz2-1.1.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrtz2-1.1.17.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyrtz2-1.1.18.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyrtz2-1.1.17.tar` & `pyrtz2-1.1.18.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0       66 2024-04-02 19:47:59.285340 pyrtz2-1.1.17/.gitattributes
--rw-r--r--   0        0        0       37 2024-04-05 12:35:50.341792 pyrtz2-1.1.17/.gitignore
--rw-r--r--   0        0        0    33041 2024-04-02 20:07:11.768711 pyrtz2-1.1.17/LICENSE
--rw-r--r--   0        0        0      455 2024-04-05 17:28:24.205830 pyrtz2-1.1.17/README.md
--rw-r--r--   0        0        0   442996 2024-03-22 20:48:12.000000 pyrtz2-1.1.17/example/con050/jasYcon050cell37m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:48:22.000000 pyrtz2-1.1.17/example/con050/jasYcon050cell37m0001.tif
--rw-r--r--   0        0        0   453575 2024-03-22 20:48:52.000000 pyrtz2-1.1.17/example/con050/jasYcon050cell38m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:49:00.000000 pyrtz2-1.1.17/example/con050/jasYcon050cell38m0001.tif
--rw-r--r--   0        0        0   458723 2024-03-22 20:49:32.000000 pyrtz2-1.1.17/example/con050/jasYcon050cell39m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:49:38.000000 pyrtz2-1.1.17/example/con050/jasYcon050cell39m0001.tif
--rw-r--r--   0        0        0   435180 2024-03-22 20:50:14.000000 pyrtz2-1.1.17/example/con050/jasYcon050cell40m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:50:22.000000 pyrtz2-1.1.17/example/con050/jasYcon050cell40m0001.tif
--rw-r--r--   0        0        0   457660 2024-03-22 20:54:28.000000 pyrtz2-1.1.17/example/con050/jasYcon050cell42m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:54:36.000000 pyrtz2-1.1.17/example/con050/jasYcon050cell42m0001.tif
--rw-r--r--   0        0        0      196 2024-03-27 20:17:56.223149 pyrtz2-1.1.17/example/con050_cp_annotations.json
--rw-r--r--   0        0        0   331740 2024-04-04 23:26:50.939244 pyrtz2-1.1.17/example/con050_curves.pdf
--rw-r--r--   0        0        0     1749 2024-04-04 23:26:34.450692 pyrtz2-1.1.17/example/con050_fits.csv
--rw-r--r--   0        0        0      205 2024-03-26 23:15:37.330282 pyrtz2-1.1.17/example/con050_vd_annotations.json
--rw-r--r--   0        0        0       37 2024-04-05 12:53:39.905466 pyrtz2-1.1.17/example/test.py
--rw-r--r--   0        0        0      794 2024-04-04 21:36:24.676720 pyrtz2-1.1.17/pyproject.toml
--rw-r--r--   0        0        0       62 2024-04-05 18:33:11.627424 pyrtz2-1.1.17/pyrtz2/__init__.py
--rw-r--r--   0        0        0     1874 2024-04-04 20:43:57.261121 pyrtz2-1.1.17/pyrtz2/afm.py
--rw-r--r--   0        0        0      335 2024-04-05 13:06:49.354563 pyrtz2-1.1.17/pyrtz2/app.py
--rw-r--r--   0        0        0     1320 2024-03-29 18:30:21.132859 pyrtz2-1.1.17/pyrtz2/assets/style.css
--rw-r--r--   0        0        0     4718 2024-04-04 20:43:28.570132 pyrtz2-1.1.17/pyrtz2/asylum.py
--rw-r--r--   0        0        0    20564 2024-04-05 18:32:48.059535 pyrtz2-1.1.17/pyrtz2/curves.py
--rw-r--r--   0        0        0     4451 2024-04-02 14:59:14.529838 pyrtz2-1.1.17/pyrtz2/fit.py
--rw-r--r--   0        0        0        0 2024-04-03 01:57:24.101285 pyrtz2-1.1.17/pyrtz2/src/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.17/pyrtz2/src/components/__init__.py
--rw-r--r--   0        0        0     1982 2024-04-04 23:28:38.697339 pyrtz2-1.1.17/pyrtz2/src/components/annotator.py
--rw-r--r--   0        0        0     5060 2024-04-05 12:35:50.358816 pyrtz2-1.1.17/pyrtz2/src/components/contact_controls.py
--rw-r--r--   0        0        0     4139 2024-04-03 02:17:21.251676 pyrtz2-1.1.17/pyrtz2/src/components/curve_dropdown.py
--rw-r--r--   0        0        0     3046 2024-04-05 12:35:50.362793 pyrtz2-1.1.17/pyrtz2/src/components/fig.py
--rw-r--r--   0        0        0     2910 2024-04-05 18:26:09.974631 pyrtz2-1.1.17/pyrtz2/src/components/fig_frame.py
--rw-r--r--   0        0        0     2393 2024-04-04 18:36:08.361121 pyrtz2-1.1.17/pyrtz2/src/components/fitter.py
--rw-r--r--   0        0        0     1194 2024-04-05 12:35:50.370793 pyrtz2-1.1.17/pyrtz2/src/components/ids.py
--rw-r--r--   0        0        0     1221 2024-04-05 12:35:50.375793 pyrtz2-1.1.17/pyrtz2/src/components/image_frame.py
--rw-r--r--   0        0        0     1666 2024-04-02 01:29:34.764572 pyrtz2-1.1.17/pyrtz2/src/components/layout.py
--rw-r--r--   0        0        0     3408 2024-04-05 12:35:50.379817 pyrtz2-1.1.17/pyrtz2/src/components/loader.py
--rw-r--r--   0        0        0     1052 2024-04-04 18:50:12.478289 pyrtz2-1.1.17/pyrtz2/src/components/toolbox.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.17/pyrtz2/src/data/__init__.py
--rw-r--r--   0        0        0     3307 2024-04-05 12:39:49.693713 pyrtz2-1.1.17/pyrtz2/src/data/downloader.py
--rw-r--r--   0        0        0     1560 2024-04-05 12:35:50.388794 pyrtz2-1.1.17/pyrtz2/src/data/experiment_loader.py
--rw-r--r--   0        0        0     1117 2024-04-05 12:35:50.392818 pyrtz2-1.1.17/pyrtz2/src/data/image_loader.py
--rw-r--r--   0        0        0     1218 2024-04-04 21:40:13.246607 pyrtz2-1.1.17/pyrtz2/src/data/processor.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.17/pyrtz2/src/utils/__init__.py
--rw-r--r--   0        0        0     2474 2024-04-05 12:35:50.397796 pyrtz2-1.1.17/pyrtz2/src/utils/utils.py
--rw-r--r--   0        0        0     1191 1970-01-01 00:00:00.000000 pyrtz2-1.1.17/PKG-INFO
+-rw-r--r--   0        0        0       66 2024-04-02 19:47:59.285340 pyrtz2-1.1.18/.gitattributes
+-rw-r--r--   0        0        0       37 2024-04-05 12:35:50.341792 pyrtz2-1.1.18/.gitignore
+-rw-r--r--   0        0        0    33041 2024-04-02 20:07:11.768711 pyrtz2-1.1.18/LICENSE
+-rw-r--r--   0        0        0      455 2024-04-05 17:28:24.205830 pyrtz2-1.1.18/README.md
+-rw-r--r--   0        0        0   442996 2024-03-22 20:48:12.000000 pyrtz2-1.1.18/example/con050/jasYcon050cell37m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:48:22.000000 pyrtz2-1.1.18/example/con050/jasYcon050cell37m0001.tif
+-rw-r--r--   0        0        0   453575 2024-03-22 20:48:52.000000 pyrtz2-1.1.18/example/con050/jasYcon050cell38m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:49:00.000000 pyrtz2-1.1.18/example/con050/jasYcon050cell38m0001.tif
+-rw-r--r--   0        0        0   458723 2024-03-22 20:49:32.000000 pyrtz2-1.1.18/example/con050/jasYcon050cell39m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:49:38.000000 pyrtz2-1.1.18/example/con050/jasYcon050cell39m0001.tif
+-rw-r--r--   0        0        0   435180 2024-03-22 20:50:14.000000 pyrtz2-1.1.18/example/con050/jasYcon050cell40m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:50:22.000000 pyrtz2-1.1.18/example/con050/jasYcon050cell40m0001.tif
+-rw-r--r--   0        0        0   457660 2024-03-22 20:54:28.000000 pyrtz2-1.1.18/example/con050/jasYcon050cell42m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:54:36.000000 pyrtz2-1.1.18/example/con050/jasYcon050cell42m0001.tif
+-rw-r--r--   0        0        0      196 2024-03-27 20:17:56.223149 pyrtz2-1.1.18/example/con050_cp_annotations.json
+-rw-r--r--   0        0        0   331740 2024-04-04 23:26:50.939244 pyrtz2-1.1.18/example/con050_curves.pdf
+-rw-r--r--   0        0        0     1749 2024-04-04 23:26:34.450692 pyrtz2-1.1.18/example/con050_fits.csv
+-rw-r--r--   0        0        0      205 2024-03-26 23:15:37.330282 pyrtz2-1.1.18/example/con050_vd_annotations.json
+-rw-r--r--   0        0        0       37 2024-04-05 12:53:39.905466 pyrtz2-1.1.18/example/test.py
+-rw-r--r--   0        0        0      794 2024-04-04 21:36:24.676720 pyrtz2-1.1.18/pyproject.toml
+-rw-r--r--   0        0        0       62 2024-04-05 18:43:42.871751 pyrtz2-1.1.18/pyrtz2/__init__.py
+-rw-r--r--   0        0        0     1874 2024-04-04 20:43:57.261121 pyrtz2-1.1.18/pyrtz2/afm.py
+-rw-r--r--   0        0        0      335 2024-04-05 13:06:49.354563 pyrtz2-1.1.18/pyrtz2/app.py
+-rw-r--r--   0        0        0     1320 2024-03-29 18:30:21.132859 pyrtz2-1.1.18/pyrtz2/assets/style.css
+-rw-r--r--   0        0        0     4718 2024-04-04 20:43:28.570132 pyrtz2-1.1.18/pyrtz2/asylum.py
+-rw-r--r--   0        0        0    18040 2024-04-05 18:43:29.214731 pyrtz2-1.1.18/pyrtz2/curves.py
+-rw-r--r--   0        0        0     4451 2024-04-02 14:59:14.529838 pyrtz2-1.1.18/pyrtz2/fit.py
+-rw-r--r--   0        0        0        0 2024-04-03 01:57:24.101285 pyrtz2-1.1.18/pyrtz2/src/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.18/pyrtz2/src/components/__init__.py
+-rw-r--r--   0        0        0     1982 2024-04-04 23:28:38.697339 pyrtz2-1.1.18/pyrtz2/src/components/annotator.py
+-rw-r--r--   0        0        0     5060 2024-04-05 12:35:50.358816 pyrtz2-1.1.18/pyrtz2/src/components/contact_controls.py
+-rw-r--r--   0        0        0     4139 2024-04-03 02:17:21.251676 pyrtz2-1.1.18/pyrtz2/src/components/curve_dropdown.py
+-rw-r--r--   0        0        0     2886 2024-04-05 18:47:58.605617 pyrtz2-1.1.18/pyrtz2/src/components/fig.py
+-rw-r--r--   0        0        0     2904 2024-04-05 18:42:39.056993 pyrtz2-1.1.18/pyrtz2/src/components/fig_frame.py
+-rw-r--r--   0        0        0     2393 2024-04-04 18:36:08.361121 pyrtz2-1.1.18/pyrtz2/src/components/fitter.py
+-rw-r--r--   0        0        0     1194 2024-04-05 12:35:50.370793 pyrtz2-1.1.18/pyrtz2/src/components/ids.py
+-rw-r--r--   0        0        0     1221 2024-04-05 12:35:50.375793 pyrtz2-1.1.18/pyrtz2/src/components/image_frame.py
+-rw-r--r--   0        0        0     1666 2024-04-02 01:29:34.764572 pyrtz2-1.1.18/pyrtz2/src/components/layout.py
+-rw-r--r--   0        0        0     3408 2024-04-05 12:35:50.379817 pyrtz2-1.1.18/pyrtz2/src/components/loader.py
+-rw-r--r--   0        0        0     1052 2024-04-04 18:50:12.478289 pyrtz2-1.1.18/pyrtz2/src/components/toolbox.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.18/pyrtz2/src/data/__init__.py
+-rw-r--r--   0        0        0     3307 2024-04-05 12:39:49.693713 pyrtz2-1.1.18/pyrtz2/src/data/downloader.py
+-rw-r--r--   0        0        0     1560 2024-04-05 12:35:50.388794 pyrtz2-1.1.18/pyrtz2/src/data/experiment_loader.py
+-rw-r--r--   0        0        0     1117 2024-04-05 12:35:50.392818 pyrtz2-1.1.18/pyrtz2/src/data/image_loader.py
+-rw-r--r--   0        0        0     1218 2024-04-04 21:40:13.246607 pyrtz2-1.1.18/pyrtz2/src/data/processor.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.18/pyrtz2/src/utils/__init__.py
+-rw-r--r--   0        0        0     2474 2024-04-05 12:35:50.397796 pyrtz2-1.1.18/pyrtz2/src/utils/utils.py
+-rw-r--r--   0        0        0     1191 1970-01-01 00:00:00.000000 pyrtz2-1.1.18/PKG-INFO
```

### Comparing `pyrtz2-1.1.17/LICENSE` & `pyrtz2-1.1.18/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/example/con050/jasYcon050cell37m0000.ibw` & `pyrtz2-1.1.18/example/con050/jasYcon050cell37m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/example/con050/jasYcon050cell37m0001.tif` & `pyrtz2-1.1.18/example/con050/jasYcon050cell37m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/example/con050/jasYcon050cell38m0000.ibw` & `pyrtz2-1.1.18/example/con050/jasYcon050cell38m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/example/con050/jasYcon050cell38m0001.tif` & `pyrtz2-1.1.18/example/con050/jasYcon050cell38m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/example/con050/jasYcon050cell39m0000.ibw` & `pyrtz2-1.1.18/example/con050/jasYcon050cell39m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/example/con050/jasYcon050cell39m0001.tif` & `pyrtz2-1.1.18/example/con050/jasYcon050cell39m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/example/con050/jasYcon050cell40m0000.ibw` & `pyrtz2-1.1.18/example/con050/jasYcon050cell40m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/example/con050/jasYcon050cell40m0001.tif` & `pyrtz2-1.1.18/example/con050/jasYcon050cell40m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/example/con050/jasYcon050cell42m0000.ibw` & `pyrtz2-1.1.18/example/con050/jasYcon050cell42m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/example/con050/jasYcon050cell42m0001.tif` & `pyrtz2-1.1.18/example/con050/jasYcon050cell42m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/example/con050_curves.pdf` & `pyrtz2-1.1.18/example/con050_curves.pdf`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/example/con050_fits.csv` & `pyrtz2-1.1.18/example/con050_fits.csv`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/pyproject.toml` & `pyrtz2-1.1.18/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/pyrtz2/afm.py` & `pyrtz2-1.1.18/pyrtz2/afm.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/pyrtz2/assets/style.css` & `pyrtz2-1.1.18/pyrtz2/assets/style.css`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/pyrtz2/asylum.py` & `pyrtz2-1.1.18/pyrtz2/asylum.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/pyrtz2/curves.py` & `pyrtz2-1.1.18/pyrtz2/curves.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     indent_param: list[float]
     indent_R2: float
     hertzian_param: list[float]
     hertzian_R2: float
     dwell_param: list[float]
     dwell_R2: float
     contact_fig: go.Figure
-    dwell_relax_fig: go.Figure
+    dwell_fig: go.Figure
 
     def __init__(
             self,
             filename: str,
             data: pd.DataFrame,
             notes: dict,
             invOLS: float,
@@ -113,19 +113,14 @@
         start_index = int(start * len(indent))
         last_index = int(last * len(indent))
         return indent.iloc[start_index:last_index].reset_index(drop=True)
 
     def get_dwell(self) -> pd.DataFrame:
         return self.get_data_between(self.dwell_range[0], self.dwell_range[1])
 
-    def get_relaxation(self) -> pd.DataFrame:
-        dwell = self.get_dwell()
-        max_ind = dwell['ind'].argmax()
-        return dwell.iloc[:max_ind].reset_index(drop=True)
-
     def get_repulsion(self) -> pd.DataFrame:
         dwell = self.get_dwell()
         max_ind = dwell['ind'].argmax()
         return dwell.iloc[max_ind:].reset_index(drop=True)
 
     def get_retract(self) -> pd.DataFrame:
         return self.get_data_between(self.dwell_range[1], -1)
@@ -190,35 +185,28 @@
         indent_between = self.get_indent_between(interval[0], interval[1])
         return hertzian_fit(indent_between['ind'], indent_between['f'], probe_diameter)
 
     def fit_dwell(self) -> tuple:
         dwell = self.get_dwell()
         return biexponential_fit(dwell['t'], dwell['f'])
 
-    def fit_relaxation(self) -> tuple:
-        relaxation = self.get_relaxation()
-        return biexponential_fit(relaxation['t'], relaxation['ind'])
-
     def get_figs_data(self, vd: bool = False, adjust: bool = False) -> None:
         if vd or adjust:
             self.restore_data()
         if vd:
             self.correct_virtual_defl()
         if adjust:
             self.adjust_to_contact()
 
         approach = self.get_approach()
-
         dwell = self.get_dwell()
-        relaxation = self.get_relaxation()
 
         self.figs_data = {
             'approach': (approach['ind'].to_numpy(), approach['f'].to_numpy()),
-            'dwell': (dwell['t'].to_numpy(), dwell['f'].to_numpy()),
-            'relaxation': (relaxation['t'].to_numpy(), relaxation['ind'].to_numpy()),
+            'dwell': (dwell['t'].to_numpy(), dwell['f'].to_numpy())
         }
 
     def get_contact_fig_plot(self) -> go.Figure:
         fig = make_fig(
             title=fr"$\text{{Selected Contact Point: {self.contact_index}}}$",
             xaxis=r"$Indentation \text{ (m)}$"
         )
@@ -241,46 +229,32 @@
         x_line = x[self.contact_index]
         y_line = y[self.contact_index]
         fig.add_vline(x=x_line, line=dict(color='red', width=1.2))
         fig.add_hline(y=y_line, line=dict(color='red', width=1.2))
         self.contact_fig = fig
         return fig
 
-    def get_dwell_relax_fig_plot(self) -> go.Figure:
+    def get_dwell_fig_plot(self) -> go.Figure:
         fig = make_fig(
-            title=r"$\text{Dwell and Relaxation}$",
+            title=r"$\text{Dwell}$",
             xaxis=r"$Time \text{ (s)}$"
         )
 
         x, y = self.figs_data['dwell']
         trace = go.Scattergl(
             x=x,
             y=y,
             name='Dwell',
             mode='markers',
             marker={'color': 'red'},
         )
 
         fig.add_trace(trace)
 
-        '''
-        x, y = self.figs_data['relaxation']
-        trace = go.Scattergl(
-            x=x,
-            y=y,
-            yaxis='y2',
-            name='Relaxation',
-            mode='markers',
-            marker={'color': 'blue'},
-        )
-
-        fig.add_trace(trace)
-        '''
-
-        self.dwell_relax_fig = fig
+        self.dwell_fig = fig
         return fig
 
     def get_fits_data(self, probe_diameter: float, ind: float | list[float]) -> None:
         indent = self.get_indent()
         indent_x_pred = indent['ind'].to_numpy()
         self.indent_param, self.indent_R2, indent_y_pred = self.fit_indent()
 
@@ -297,23 +271,19 @@
             hertzian_x_pred = self.get_indent_between(ind[0], ind[1])[
                 'ind'].to_numpy()
 
         dwell = self.get_dwell()
         dwell_x_pred = dwell['t'].to_numpy()
         self.dwell_param, self.dwell_R2, dwell_y_pred = self.fit_dwell()
 
-        relaxation = self.get_relaxation()
-        relaxation_x_pred = relaxation['t'].to_numpy()
-        self.relaxation_param, self.relaxation_R2, relaxation_y_pred = self.fit_relaxation()
-
         self.fits_data = {
             'indent': (indent_x_pred, indent_y_pred),
             'hertzian': (hertzian_x_pred, hertzian_y_pred),
             'dwell': (dwell_x_pred, dwell_y_pred),
-            'relaxation': (relaxation_x_pred, relaxation_y_pred),
+
         }
 
     def add_contact_fit(self) -> go.Figure:
         x, y = self.fits_data['indent']
         trace = go.Scattergl(
             x=x,
             y=y,
@@ -334,45 +304,30 @@
                 'width': 3,
             },
         )
         self.contact_fig.add_trace(trace)
 
         return self.contact_fig
 
-    def add_dwell_relax_fit(self) -> go.Figure:
+    def add_dwell_fit(self) -> go.Figure:
         x, y = self.fits_data['dwell']
 
         trace = go.Scattergl(
             x=x,
             y=y,
             name='DwellFit',
             mode='lines',
             line={
                 'color': 'green',
                 'width': 3,
             },
         )
-        self.dwell_relax_fig.add_trace(trace)
+        self.dwell_fig.add_trace(trace)
 
-        '''
-        x, y = self.fits_data['relaxation']
-        trace = go.Scattergl(
-            x=x,
-            y=y,
-            yaxis='y2',
-            name='RelaxationFit',
-            mode='lines',
-            line={
-                'color': 'green',
-                'width': 3,
-            },
-        )
-        self.dwell_relax_fig.add_trace(trace)
-        '''
-        return self.dwell_relax_fig
+        return self.dwell_fig
 
     def get_contact_fig_pdf(self) -> go.Figure:
         title = fr"$\text{{Selected Contact Point: {self.contact_index}}}$"
         xaxis = r"$Indentation \text{ (m)}$"
         fig = make_fig(title, xaxis)
 
         x, y = self.figs_data['approach']
@@ -395,16 +350,16 @@
             x, y = self.fits_data['hertzian']
             trace = go.Scatter(x=x, y=y, name='HertzianFit',
                                mode='lines', line={'color': 'green', 'width': 3})
             fig.add_trace(trace)
 
         return fig
 
-    def get_dwell_relax_fig_pdf(self) -> go.Figure:
-        title = r"$\text{Dwell and Relaxation}$"
+    def get_dwell_fig_pdf(self) -> go.Figure:
+        title = r"$\text{Dwell}$"
         xaxis = r"$Time \text{ (s)}$"
         fig = make_fig(title, xaxis)
 
         x, y = self.figs_data['dwell']
         trace = go.Scatter(x=x, y=y, name='Dwell',
                            marker_color='red')
         fig.add_trace(trace)
@@ -420,31 +375,21 @@
                 showline=True,
                 linewidth=2,
                 linecolor='black',
                 tickprefix=r"$",
                 ticksuffix=r"$",
             )
         )
-        '''
-        x, y = self.figs_data['relaxation']
-        trace = go.Scatter(x=x, y=y, name='Relaxation',
-                           marker_color='blue', yaxis='y2')
-        fig.add_trace(trace)
-        '''
+
         if hasattr(self, 'fits_data'):
             x, y = self.fits_data['dwell']
             trace = go.Scatter(x=x, y=y, name='DwellFit',
                                mode='lines', line={'color': 'green', 'width': 3})
             fig.add_trace(trace)
-            '''
-            x, y = self.fits_data['relaxation']
-            trace = go.Scatter(x=x, y=y, yaxis='y2', name='RelaxationFit',
-                               mode='lines', line={'color': 'green', 'width': 3})
-            fig.add_trace(trace)
-            '''
+
         return fig
 
     def get_all_fits(self) -> dict:
         fit_results_dict = {
             'max_ind': self.max_ind,
             'max_f': self.max_f,
 
@@ -462,22 +407,14 @@
             'dwell_c': self.dwell_param[0],
             'dwell_tau1': self.dwell_param[1],
             'dwell_tau2': self.dwell_param[2],
             'dwell_tauMax': max(self.dwell_param[1], self.dwell_param[2]),
             'dwell_tauMin': min(self.dwell_param[1], self.dwell_param[2]),
             'dwell_yf': self.dwell_param[3],
             'dwell_R2': self.dwell_R2,
-
-            # 'relaxation_c': self.relaxation_param[0],
-            # 'relaxation_tau1': self.relaxation_param[1],
-            # 'relaxation_tau2': self.relaxation_param[2],
-            # 'relaxation_tauMax': max(self.relaxation_param[1], self.relaxation_param[2]),
-            # 'relaxation_tauMin': min(self.relaxation_param[1], self.relaxation_param[2]),
-            # 'relaxation_yf': self.relaxation_param[3],
-            # 'relaxation_R2': self.relaxation_R2
         }
 
         return fit_results_dict
 
 
 class CurveSet:
     vd_dict: dict[tuple[str], bool] = {}
@@ -592,14 +529,14 @@
             title = fr"$\text{{{title}}}$"
             contact_fit_fig = curve.get_contact_fig_pdf()
             contact_fit_fig.update_layout(title={'text': title})
             contact_fit_fig_pdf = io.BytesIO(
                 contact_fit_fig.to_image(format='pdf'))
             merger.append(contact_fit_fig_pdf)
 
-            dwell_relaxation_fit_fig = curve.get_dwell_relax_fig_pdf()
-            dwell_relaxation_fit_fig.update_layout(title={'text': title})
-            dwell_relaxation_fit_fig_pdf = io.BytesIO(
-                dwell_relaxation_fit_fig.to_image(format='pdf'))
-            merger.append(dwell_relaxation_fit_fig_pdf)
+            dwell_fit_fig = curve.get_dwell_fig_pdf()
+            dwell_fit_fig.update_layout(title={'text': title})
+            dwell_fit_fig_pdf = io.BytesIO(
+                dwell_fit_fig.to_image(format='pdf'))
+            merger.append(dwell_fit_fig_pdf)
 
         return merger
```

### Comparing `pyrtz2-1.1.17/pyrtz2/fit.py` & `pyrtz2-1.1.18/pyrtz2/fit.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/pyrtz2/src/components/annotator.py` & `pyrtz2-1.1.18/pyrtz2/src/components/annotator.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/pyrtz2/src/components/contact_controls.py` & `pyrtz2-1.1.18/pyrtz2/src/components/contact_controls.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/pyrtz2/src/components/curve_dropdown.py` & `pyrtz2-1.1.18/pyrtz2/src/components/curve_dropdown.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/pyrtz2/src/components/fig.py` & `pyrtz2-1.1.18/pyrtz2/src/components/fig.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,21 +31,16 @@
             'xanchor': 'center'
         },
         plot_bgcolor='white',
         paper_bgcolor='white',
         margin=dict(t=50, b=50, l=50, r=50),
         showlegend=False,
         transition={'duration': 500},
-        yaxis2=dict(
-            title=r"$Indentation \text{ (m)}$",
-            overlaying='y',
-            side='right',
-            tickprefix=r"$",
-            ticksuffix=r"$",
-        )
+        width=800,
+        height=600
     )
 
     fig.update_annotations(yshift=10)
 
     fig.update_xaxes(
         showgrid=False,
         ticks='outside',
@@ -115,8 +110,7 @@
     fig.layout['shapes'][0]['x0'] = data_x[cp]
     fig.layout['shapes'][0]['x1'] = data_x[cp]
     fig.layout['shapes'][1]['y0'] = data_y[cp]
     fig.layout['shapes'][1]['y1'] = data_y[cp]
     fig.layout['title']['text'] = fr"$\text{{Selected Contact Point: {cp}}}$"
 
     return fig
-
```

### Comparing `pyrtz2-1.1.17/pyrtz2/src/components/fig_frame.py` & `pyrtz2-1.1.18/pyrtz2/src/components/fig_frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         file_name = os.path.join(experiment_path, name)
         curve = load_ibw(file_name)
         curve.reduce_data()
         cp = get_current_annotation(curve_value, cp_data)
         curve.set_contact_index(cp)
         curve.get_figs_data(vd=vd, adjust=adjust)
         contact_fig = curve.get_contact_fig_plot()
-        forcetime_fig = curve.get_dwell_relax_fig_plot()
+        forcetime_fig = curve.get_dwell_fig_plot()
 
         return contact_fig, forcetime_fig
 
     @app.callback(
         Output(ids.CP_ANNOTATIONS, 'data'),
         [Input(ids.CONTACT_FIG, 'clickData')],
         [State(ids.CURVE_DROPDOWN, 'value'),
```

### Comparing `pyrtz2-1.1.17/pyrtz2/src/components/fitter.py` & `pyrtz2-1.1.18/pyrtz2/src/components/fitter.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/pyrtz2/src/components/ids.py` & `pyrtz2-1.1.18/pyrtz2/src/components/ids.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/pyrtz2/src/components/image_frame.py` & `pyrtz2-1.1.18/pyrtz2/src/components/image_frame.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/pyrtz2/src/components/layout.py` & `pyrtz2-1.1.18/pyrtz2/src/components/layout.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/pyrtz2/src/components/loader.py` & `pyrtz2-1.1.18/pyrtz2/src/components/loader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/pyrtz2/src/components/toolbox.py` & `pyrtz2-1.1.18/pyrtz2/src/components/toolbox.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/pyrtz2/src/data/downloader.py` & `pyrtz2-1.1.18/pyrtz2/src/data/downloader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/pyrtz2/src/data/experiment_loader.py` & `pyrtz2-1.1.18/pyrtz2/src/data/experiment_loader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/pyrtz2/src/data/image_loader.py` & `pyrtz2-1.1.18/pyrtz2/src/data/image_loader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/pyrtz2/src/data/processor.py` & `pyrtz2-1.1.18/pyrtz2/src/data/processor.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/pyrtz2/src/utils/utils.py` & `pyrtz2-1.1.18/pyrtz2/src/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.17/PKG-INFO` & `pyrtz2-1.1.18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtz2
-Version: 1.1.17
+Version: 1.1.18
 Summary: Force spectroscopy in Python
 Author-email: "Hoseyn A. Amiri" <aamirihoseyn@gmail.com>
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: dash
 Requires-Dist: dash-bootstrap-components
```

