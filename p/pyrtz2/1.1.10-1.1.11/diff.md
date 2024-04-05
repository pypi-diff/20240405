# Comparing `tmp/pyrtz2-1.1.10.tar.gz` & `tmp/pyrtz2-1.1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrtz2-1.1.10.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyrtz2-1.1.11.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyrtz2-1.1.10.tar` & `pyrtz2-1.1.11.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0       66 2024-04-02 19:47:59.285340 pyrtz2-1.1.10/.gitattributes
--rw-r--r--   0        0        0       20 2024-04-04 22:35:31.627883 pyrtz2-1.1.10/.gitignore
--rw-r--r--   0        0        0    33041 2024-04-02 20:07:11.768711 pyrtz2-1.1.10/LICENSE
--rw-r--r--   0        0        0      228 2024-04-02 19:51:47.632334 pyrtz2-1.1.10/README.md
--rw-r--r--   0        0        0      794 2024-04-04 21:36:24.676720 pyrtz2-1.1.10/pyproject.toml
--rw-r--r--   0        0        0       62 2024-04-04 23:32:50.850451 pyrtz2-1.1.10/pyrtz2/__init__.py
--rw-r--r--   0        0        0     1874 2024-04-04 20:43:57.261121 pyrtz2-1.1.10/pyrtz2/afm.py
--rw-r--r--   0        0        0      404 2024-04-04 22:20:09.403050 pyrtz2-1.1.10/pyrtz2/app.py
--rw-r--r--   0        0        0     1320 2024-03-29 18:30:21.132859 pyrtz2-1.1.10/pyrtz2/assets/style.css
--rw-r--r--   0        0        0     4718 2024-04-04 20:43:28.570132 pyrtz2-1.1.10/pyrtz2/asylum.py
--rw-r--r--   0        0        0    20124 2024-04-04 20:43:38.173145 pyrtz2-1.1.10/pyrtz2/curves.py
--rw-r--r--   0        0        0     4451 2024-04-02 14:59:14.529838 pyrtz2-1.1.10/pyrtz2/fit.py
--rw-r--r--   0        0        0        0 2024-04-03 01:57:24.101285 pyrtz2-1.1.10/pyrtz2/src/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.10/pyrtz2/src/components/__init__.py
--rw-r--r--   0        0        0     1982 2024-04-04 23:28:38.697339 pyrtz2-1.1.10/pyrtz2/src/components/annotator.py
--rw-r--r--   0        0        0     5604 2024-04-04 18:49:51.040442 pyrtz2-1.1.10/pyrtz2/src/components/contact_controls.py
--rw-r--r--   0        0        0     4139 2024-04-03 02:17:21.251676 pyrtz2-1.1.10/pyrtz2/src/components/curve_dropdown.py
--rw-r--r--   0        0        0     3409 2024-04-04 18:23:41.184544 pyrtz2-1.1.10/pyrtz2/src/components/fig.py
--rw-r--r--   0        0        0     4506 2024-04-04 23:26:04.798786 pyrtz2-1.1.10/pyrtz2/src/components/fig_frame.py
--rw-r--r--   0        0        0     2393 2024-04-04 18:36:08.361121 pyrtz2-1.1.10/pyrtz2/src/components/fitter.py
--rw-r--r--   0        0        0     1241 2024-04-04 18:49:04.376522 pyrtz2-1.1.10/pyrtz2/src/components/ids.py
--rw-r--r--   0        0        0     1195 2024-04-03 02:18:43.224430 pyrtz2-1.1.10/pyrtz2/src/components/image_frame.py
--rw-r--r--   0        0        0     1666 2024-04-02 01:29:34.764572 pyrtz2-1.1.10/pyrtz2/src/components/layout.py
--rw-r--r--   0        0        0     3461 2024-04-04 20:44:27.712291 pyrtz2-1.1.10/pyrtz2/src/components/loader.py
--rw-r--r--   0        0        0     1052 2024-04-04 18:50:12.478289 pyrtz2-1.1.10/pyrtz2/src/components/toolbox.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.10/pyrtz2/src/data/__init__.py
--rw-r--r--   0        0        0     3346 2024-04-04 20:08:19.361627 pyrtz2-1.1.10/pyrtz2/src/data/downloader.py
--rw-r--r--   0        0        0     1620 2024-04-04 20:44:13.562141 pyrtz2-1.1.10/pyrtz2/src/data/experiment_loader.py
--rw-r--r--   0        0        0     1128 2024-04-03 02:24:32.297813 pyrtz2-1.1.10/pyrtz2/src/data/image_loader.py
--rw-r--r--   0        0        0     1218 2024-04-04 21:40:13.246607 pyrtz2-1.1.10/pyrtz2/src/data/processor.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.10/pyrtz2/src/utils/__init__.py
--rw-r--r--   0        0        0     1020 2024-03-29 20:53:21.746168 pyrtz2-1.1.10/pyrtz2/src/utils/_backup/igor/__init__.py
--rw-r--r--   0        0        0    30699 2024-03-29 20:52:56.279210 pyrtz2-1.1.10/pyrtz2/src/utils/_backup/igor/binarywave.py
--rw-r--r--   0        0        0    29217 2024-03-29 21:12:48.091560 pyrtz2-1.1.10/pyrtz2/src/utils/_backup/igor/structure.py
--rw-r--r--   0        0        0     3911 2024-02-02 05:34:10.456245 pyrtz2-1.1.10/pyrtz2/src/utils/_backup/igor/util.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.10/pyrtz2/src/utils/_backup/pyrtz/__init__.py
--rw-r--r--   0        0        0     4623 2024-03-29 23:09:57.877567 pyrtz2-1.1.10/pyrtz2/src/utils/_backup/pyrtz/asylum.py
--rw-r--r--   0        0        0    35543 2024-03-30 00:31:39.650484 pyrtz2-1.1.10/pyrtz2/src/utils/_backup/pyrtz/curves.py
--rw-r--r--   0        0        0     2428 2024-04-04 23:30:58.773035 pyrtz2-1.1.10/pyrtz2/src/utils/utils.py
--rw-r--r--   0        0        0      976 1970-01-01 00:00:00.000000 pyrtz2-1.1.10/PKG-INFO
+-rw-r--r--   0        0        0       66 2024-04-02 19:47:59.285340 pyrtz2-1.1.11/.gitattributes
+-rw-r--r--   0        0        0       20 2024-04-04 22:35:31.627883 pyrtz2-1.1.11/.gitignore
+-rw-r--r--   0        0        0    33041 2024-04-02 20:07:11.768711 pyrtz2-1.1.11/LICENSE
+-rw-r--r--   0        0        0      228 2024-04-02 19:51:47.632334 pyrtz2-1.1.11/README.md
+-rw-r--r--   0        0        0      794 2024-04-04 21:36:24.676720 pyrtz2-1.1.11/pyproject.toml
+-rw-r--r--   0        0        0       62 2024-04-05 02:11:21.366282 pyrtz2-1.1.11/pyrtz2/__init__.py
+-rw-r--r--   0        0        0     1874 2024-04-04 20:43:57.261121 pyrtz2-1.1.11/pyrtz2/afm.py
+-rw-r--r--   0        0        0      359 2024-04-05 02:11:14.258329 pyrtz2-1.1.11/pyrtz2/app.py
+-rw-r--r--   0        0        0     1320 2024-03-29 18:30:21.132859 pyrtz2-1.1.11/pyrtz2/assets/style.css
+-rw-r--r--   0        0        0     4718 2024-04-04 20:43:28.570132 pyrtz2-1.1.11/pyrtz2/asylum.py
+-rw-r--r--   0        0        0    20124 2024-04-04 20:43:38.173145 pyrtz2-1.1.11/pyrtz2/curves.py
+-rw-r--r--   0        0        0     4451 2024-04-02 14:59:14.529838 pyrtz2-1.1.11/pyrtz2/fit.py
+-rw-r--r--   0        0        0        0 2024-04-03 01:57:24.101285 pyrtz2-1.1.11/pyrtz2/src/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.11/pyrtz2/src/components/__init__.py
+-rw-r--r--   0        0        0     1982 2024-04-04 23:28:38.697339 pyrtz2-1.1.11/pyrtz2/src/components/annotator.py
+-rw-r--r--   0        0        0     5604 2024-04-04 18:49:51.040442 pyrtz2-1.1.11/pyrtz2/src/components/contact_controls.py
+-rw-r--r--   0        0        0     4139 2024-04-03 02:17:21.251676 pyrtz2-1.1.11/pyrtz2/src/components/curve_dropdown.py
+-rw-r--r--   0        0        0     3409 2024-04-04 18:23:41.184544 pyrtz2-1.1.11/pyrtz2/src/components/fig.py
+-rw-r--r--   0        0        0     4525 2024-04-05 00:22:08.628868 pyrtz2-1.1.11/pyrtz2/src/components/fig_frame.py
+-rw-r--r--   0        0        0     2393 2024-04-04 18:36:08.361121 pyrtz2-1.1.11/pyrtz2/src/components/fitter.py
+-rw-r--r--   0        0        0     1241 2024-04-04 18:49:04.376522 pyrtz2-1.1.11/pyrtz2/src/components/ids.py
+-rw-r--r--   0        0        0     1195 2024-04-03 02:18:43.224430 pyrtz2-1.1.11/pyrtz2/src/components/image_frame.py
+-rw-r--r--   0        0        0     1666 2024-04-02 01:29:34.764572 pyrtz2-1.1.11/pyrtz2/src/components/layout.py
+-rw-r--r--   0        0        0     3461 2024-04-04 20:44:27.712291 pyrtz2-1.1.11/pyrtz2/src/components/loader.py
+-rw-r--r--   0        0        0     1052 2024-04-04 18:50:12.478289 pyrtz2-1.1.11/pyrtz2/src/components/toolbox.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.11/pyrtz2/src/data/__init__.py
+-rw-r--r--   0        0        0     3346 2024-04-04 20:08:19.361627 pyrtz2-1.1.11/pyrtz2/src/data/downloader.py
+-rw-r--r--   0        0        0     1824 2024-04-05 02:11:14.359347 pyrtz2-1.1.11/pyrtz2/src/data/experiment_loader.py
+-rw-r--r--   0        0        0     1131 2024-04-05 02:11:14.364347 pyrtz2-1.1.11/pyrtz2/src/data/image_loader.py
+-rw-r--r--   0        0        0     1218 2024-04-04 21:40:13.246607 pyrtz2-1.1.11/pyrtz2/src/data/processor.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.11/pyrtz2/src/utils/__init__.py
+-rw-r--r--   0        0        0     1020 2024-03-29 20:53:21.746168 pyrtz2-1.1.11/pyrtz2/src/utils/_backup/igor/__init__.py
+-rw-r--r--   0        0        0    30699 2024-03-29 20:52:56.279210 pyrtz2-1.1.11/pyrtz2/src/utils/_backup/igor/binarywave.py
+-rw-r--r--   0        0        0    29217 2024-03-29 21:12:48.091560 pyrtz2-1.1.11/pyrtz2/src/utils/_backup/igor/structure.py
+-rw-r--r--   0        0        0     3911 2024-02-02 05:34:10.456245 pyrtz2-1.1.11/pyrtz2/src/utils/_backup/igor/util.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.11/pyrtz2/src/utils/_backup/pyrtz/__init__.py
+-rw-r--r--   0        0        0     4623 2024-03-29 23:09:57.877567 pyrtz2-1.1.11/pyrtz2/src/utils/_backup/pyrtz/asylum.py
+-rw-r--r--   0        0        0    35543 2024-03-30 00:31:39.650484 pyrtz2-1.1.11/pyrtz2/src/utils/_backup/pyrtz/curves.py
+-rw-r--r--   0        0        0     2403 2024-04-05 00:44:05.466747 pyrtz2-1.1.11/pyrtz2/src/utils/utils.py
+-rw-r--r--   0        0        0      976 1970-01-01 00:00:00.000000 pyrtz2-1.1.11/PKG-INFO
```

### Comparing `pyrtz2-1.1.10/LICENSE` & `pyrtz2-1.1.11/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.10/pyproject.toml` & `pyrtz2-1.1.11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.10/pyrtz2/afm.py` & `pyrtz2-1.1.11/pyrtz2/afm.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.10/pyrtz2/assets/style.css` & `pyrtz2-1.1.11/pyrtz2/assets/style.css`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.10/pyrtz2/asylum.py` & `pyrtz2-1.1.11/pyrtz2/asylum.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.10/pyrtz2/curves.py` & `pyrtz2-1.1.11/pyrtz2/curves.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.10/pyrtz2/fit.py` & `pyrtz2-1.1.11/pyrtz2/fit.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.10/pyrtz2/src/components/annotator.py` & `pyrtz2-1.1.11/pyrtz2/src/components/annotator.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.10/pyrtz2/src/components/contact_controls.py` & `pyrtz2-1.1.11/pyrtz2/src/components/contact_controls.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.10/pyrtz2/src/components/curve_dropdown.py` & `pyrtz2-1.1.11/pyrtz2/src/components/curve_dropdown.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.10/pyrtz2/src/components/fig.py` & `pyrtz2-1.1.11/pyrtz2/src/components/fig.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.10/pyrtz2/src/components/fig_frame.py` & `pyrtz2-1.1.11/pyrtz2/src/components/fig_frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
          State(ids.CONTACT_FIG, 'figure'),
          State(ids.FORCETIME_FIG, 'figure'),
          ],
         prevent_initial_call=True
     )
     def show_data(curve_value, adjust, vd_data, cp_data, encoded_experiment, contact_fig, forcetime_fig):
         ctx = callback_context
-        if not ctx.triggered or not vd_data or not cp_data:
+        if not ctx.triggered or not curve_value or not vd_data or not cp_data:
             raise PreventUpdate
         trigger_id = ctx.triggered[0]['prop_id'].split('.')[0]
 
         vd = get_current_annotation(curve_value, vd_data)
         if trigger_id == ids.CP_ANNOTATIONS and not vd:
             raise PreventUpdate
```

### Comparing `pyrtz2-1.1.10/pyrtz2/src/components/fitter.py` & `pyrtz2-1.1.11/pyrtz2/src/components/fitter.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.10/pyrtz2/src/components/ids.py` & `pyrtz2-1.1.11/pyrtz2/src/components/ids.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.10/pyrtz2/src/components/image_frame.py` & `pyrtz2-1.1.11/pyrtz2/src/components/image_frame.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.10/pyrtz2/src/components/layout.py` & `pyrtz2-1.1.11/pyrtz2/src/components/layout.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.10/pyrtz2/src/components/loader.py` & `pyrtz2-1.1.11/pyrtz2/src/components/loader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.10/pyrtz2/src/components/toolbox.py` & `pyrtz2-1.1.11/pyrtz2/src/components/toolbox.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.10/pyrtz2/src/data/downloader.py` & `pyrtz2-1.1.11/pyrtz2/src/data/downloader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.10/pyrtz2/src/data/experiment_loader.py` & `pyrtz2-1.1.11/pyrtz2/src/data/experiment_loader.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 from ...afm import AFM
 from ..components import ids
 from ..utils.utils import dump, make_json
 
 
 def render(app: Dash) -> dcc.Store:
     @app.callback(
-        [Output(ids.EXPERIMENT, 'data', allow_duplicate=True),
-         Output(ids.EXPERIMENT_PROCESSED, 'data', allow_duplicate=True),
-         Output(ids.CP_ANNOTATIONS, 'data', allow_duplicate=True),
+        [Output(ids.EXPERIMENT, 'data', allow_duplicate=True),Output(ids.CP_ANNOTATIONS, 'data', allow_duplicate=True),
          Output(ids.VD_ANNOTATIONS, 'data', allow_duplicate=True)],
         [Input(ids.LOAD_EXPERIMENT, 'n_clicks')],
         [State(ids.EXPERIMENT_PATH, 'value'),
          State(ids.EXPERIMENT_LABELS, 'value'),
          State(ids.PROBE_DIAMETER, 'value')],
         prevent_initial_call=True
     )
@@ -27,13 +25,21 @@
         if not labels or not probe_diameter:
             raise PreventUpdate
 
         exp_name = os.path.basename(os.path.normpath(experiment_path))
         path = os.path.dirname(os.path.normpath(experiment_path))
         label_list = [label.strip() for label in labels.split(';')]
         experiment = AFM(path, exp_name, label_list, float(probe_diameter))
-
+        experiment.experiment.reduce_data()
         cp_data = make_json(experiment.curve_keys, 0)
         vd_data = make_json(experiment.curve_keys, False)
-        return dump(experiment), dump(experiment), cp_data, vd_data
+        return dump(experiment), cp_data, vd_data
+    
+    @app.callback(
+        Output(ids.EXPERIMENT_PROCESSED, 'data', allow_duplicate=True),
+        Input(ids.EXPERIMENT, 'data'),
+        prevent_initial_call=True
+    )
+    def copy_to_processed(encoded_experiment):
+        return encoded_experiment
 
     return dcc.Store(id=ids.EXPERIMENT)
```

### Comparing `pyrtz2-1.1.10/pyrtz2/src/data/image_loader.py` & `pyrtz2-1.1.11/pyrtz2/src/data/image_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     tif_to_base64
 )
 
 
 def render(app: Dash) -> dcc.Store:
     @app.callback(
         Output(ids.IMAGES, 'data', allow_duplicate=True),
-        [Input(ids.CURVE_DROPDOWN, 'options')],
+        [Input(ids.EXPERIMENT_PROCESSED, 'data')],
         [State(ids.EXPERIMENT_PATH, 'value'),
          State(ids.EXPERIMENT_LABELS, 'value')],
         prevent_initial_call=True
     )
     def store_images(_, experiment_path, labels):
         label_list = [label.strip() for label in labels.split(';')]
```

### Comparing `pyrtz2-1.1.10/pyrtz2/src/data/processor.py` & `pyrtz2-1.1.11/pyrtz2/src/data/processor.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.10/pyrtz2/src/utils/_backup/igor/__init__.py` & `pyrtz2-1.1.11/pyrtz2/src/utils/_backup/igor/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.10/pyrtz2/src/utils/_backup/igor/binarywave.py` & `pyrtz2-1.1.11/pyrtz2/src/utils/_backup/igor/binarywave.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.10/pyrtz2/src/utils/_backup/igor/structure.py` & `pyrtz2-1.1.11/pyrtz2/src/utils/_backup/igor/structure.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.10/pyrtz2/src/utils/_backup/igor/util.py` & `pyrtz2-1.1.11/pyrtz2/src/utils/_backup/igor/util.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.10/pyrtz2/src/utils/_backup/pyrtz/asylum.py` & `pyrtz2-1.1.11/pyrtz2/src/utils/_backup/pyrtz/asylum.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.10/pyrtz2/src/utils/_backup/pyrtz/curves.py` & `pyrtz2-1.1.11/pyrtz2/src/utils/_backup/pyrtz/curves.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.10/pyrtz2/src/utils/utils.py` & `pyrtz2-1.1.11/pyrtz2/src/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 def group_values_by_keys(original_dict: dict) -> dict:
     if len(next(iter(original_dict))) == 1:
         return original_dict
 
     new_dict = {}
     for key, value in original_dict.items():
-        new_key = key[:-1] if len(key) > 1 else key
+        new_key = key[:-1]
         if new_key not in new_dict:
             new_dict[new_key] = [value]
         else:
             new_dict[new_key].append(value)
     return new_dict
```

### Comparing `pyrtz2-1.1.10/PKG-INFO` & `pyrtz2-1.1.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtz2
-Version: 1.1.10
+Version: 1.1.11
 Summary: Force spectroscopy in Python
 Author-email: "Hoseyn A. Amiri" <aamirihoseyn@gmail.com>
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: dash
 Requires-Dist: dash-bootstrap-components
```

