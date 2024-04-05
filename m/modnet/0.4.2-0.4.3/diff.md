# Comparing `tmp/modnet-0.4.2.tar.gz` & `tmp/modnet-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/modnet-0.4.2.tar", last modified: Tue Apr  2 15:48:47 2024, max compression
+gzip compressed data, was "dist/modnet-0.4.3.tar", last modified: Fri Apr  5 10:43:47 2024, max compression
```

## Comparing `modnet-0.4.2.tar` & `modnet-0.4.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-02 15:48:47.000000 modnet-0.4.2/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     1078 2022-01-10 10:10:32.000000 modnet-0.4.2/LICENSE.md
--rw-r--r--   0 ppdebreuck   (501) staff       (20)       48 2022-01-10 10:10:32.000000 modnet-0.4.2/MANIFEST.in
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     6057 2024-04-02 15:48:47.000000 modnet-0.4.2/PKG-INFO
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     4243 2023-07-11 13:21:01.000000 modnet-0.4.2/README.md
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)       22 2024-03-28 10:26:50.000000 modnet-0.4.2/modnet/__init__.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet/data/
--rw-r--r--   0 ppdebreuck   (501) staff       (20) 13666623 2021-11-08 13:57:41.000000 modnet-0.4.2/modnet/data/Features_cross
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     4055 2022-05-12 10:28:50.000000 modnet-0.4.2/modnet/ext_data.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet/featurizers/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      264 2021-02-15 14:07:41.000000 modnet-0.4.2/modnet/featurizers/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    12908 2024-04-02 15:48:26.000000 modnet-0.4.2/modnet/featurizers/featurizers.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet/featurizers/presets/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      978 2023-07-11 13:21:01.000000 modnet-0.4.2/modnet/featurizers/presets/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    10080 2023-07-28 12:09:44.000000 modnet-0.4.2/modnet/featurizers/presets/debreuck_2020.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     9303 2023-07-28 12:09:44.000000 modnet-0.4.2/modnet/featurizers/presets/matminer_2023.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    16049 2023-07-28 12:09:44.000000 modnet-0.4.2/modnet/featurizers/presets/matminer_all_2023.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      623 2023-07-28 12:09:44.000000 modnet-0.4.2/modnet/featurizers/utils.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet/hyper_opt/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)       63 2022-01-12 21:23:06.000000 modnet-0.4.2/modnet/hyper_opt/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    27301 2024-03-28 10:26:50.000000 modnet-0.4.2/modnet/hyper_opt/fit_genetic.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet/matbench/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      116 2021-02-15 14:07:41.000000 modnet-0.4.2/modnet/matbench/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    11640 2023-07-11 13:21:01.000000 modnet-0.4.2/modnet/matbench/benchmark.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet/model_presets/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      166 2022-01-10 10:10:32.000000 modnet-0.4.2/modnet/model_presets/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     2292 2021-08-16 13:22:38.000000 modnet-0.4.2/modnet/model_presets/presets.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet/models/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      402 2024-02-07 15:47:41.000000 modnet-0.4.2/modnet/models/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    15169 2024-04-02 15:48:26.000000 modnet-0.4.2/modnet/models/bayesian.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    17887 2024-03-28 10:26:50.000000 modnet-0.4.2/modnet/models/ensemble.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    60314 2024-03-28 10:26:50.000000 modnet-0.4.2/modnet/models/vanilla.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    41991 2024-03-28 10:26:50.000000 modnet-0.4.2/modnet/preprocessing.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     6344 2024-03-28 10:26:50.000000 modnet-0.4.2/modnet/sklearn.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet/tests/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)        0 2020-09-16 10:22:36.000000 modnet-0.4.2/modnet/tests/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     4550 2024-04-02 15:48:26.000000 modnet-0.4.2/modnet/tests/conftest.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     4444 2023-07-11 13:21:01.000000 modnet-0.4.2/modnet/tests/test_benchmark.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      563 2021-01-14 10:39:09.000000 modnet-0.4.2/modnet/tests/test_ext_data.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      771 2024-04-02 15:48:22.000000 modnet-0.4.2/modnet/tests/test_hyper_opt.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     9504 2024-02-07 15:47:41.000000 modnet-0.4.2/modnet/tests/test_model.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    17907 2024-04-02 15:48:26.000000 modnet-0.4.2/modnet/tests/test_preprocessing.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     3110 2022-05-19 13:18:13.000000 modnet-0.4.2/modnet/tests/test_sklearn.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      737 2021-02-15 14:07:41.000000 modnet-0.4.2/modnet/utils.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet.egg-info/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     6057 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet.egg-info/PKG-INFO
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     1110 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet.egg-info/SOURCES.txt
--rw-r--r--   0 ppdebreuck   (501) staff       (20)        1 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet.egg-info/dependency_links.txt
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      206 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet.egg-info/requires.txt
--rw-r--r--   0 ppdebreuck   (501) staff       (20)        7 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet.egg-info/top_level.txt
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      118 2024-04-02 15:48:47.000000 modnet-0.4.2/setup.cfg
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     1877 2024-04-02 15:48:26.000000 modnet-0.4.2/setup.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-05 10:43:47.000000 modnet-0.4.3/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     1078 2022-01-10 10:10:32.000000 modnet-0.4.3/LICENSE.md
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)       48 2022-01-10 10:10:32.000000 modnet-0.4.3/MANIFEST.in
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     6057 2024-04-05 10:43:47.000000 modnet-0.4.3/PKG-INFO
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     4243 2023-07-11 13:21:01.000000 modnet-0.4.3/README.md
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-05 10:43:46.000000 modnet-0.4.3/modnet/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)       22 2024-04-05 10:41:33.000000 modnet-0.4.3/modnet/__init__.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-05 10:43:46.000000 modnet-0.4.3/modnet/data/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20) 13666623 2021-11-08 13:57:41.000000 modnet-0.4.3/modnet/data/Features_cross
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     4055 2022-05-12 10:28:50.000000 modnet-0.4.3/modnet/ext_data.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-05 10:43:47.000000 modnet-0.4.3/modnet/featurizers/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      264 2021-02-15 14:07:41.000000 modnet-0.4.3/modnet/featurizers/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    12908 2024-04-02 15:48:26.000000 modnet-0.4.3/modnet/featurizers/featurizers.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-05 10:43:47.000000 modnet-0.4.3/modnet/featurizers/presets/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      978 2023-07-11 13:21:01.000000 modnet-0.4.3/modnet/featurizers/presets/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    10080 2023-07-28 12:09:44.000000 modnet-0.4.3/modnet/featurizers/presets/debreuck_2020.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     9303 2023-07-28 12:09:44.000000 modnet-0.4.3/modnet/featurizers/presets/matminer_2023.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    16049 2023-07-28 12:09:44.000000 modnet-0.4.3/modnet/featurizers/presets/matminer_all_2023.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      623 2023-07-28 12:09:44.000000 modnet-0.4.3/modnet/featurizers/utils.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-05 10:43:47.000000 modnet-0.4.3/modnet/hyper_opt/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)       63 2022-01-12 21:23:06.000000 modnet-0.4.3/modnet/hyper_opt/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    27301 2024-03-28 10:26:50.000000 modnet-0.4.3/modnet/hyper_opt/fit_genetic.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-05 10:43:47.000000 modnet-0.4.3/modnet/matbench/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      116 2021-02-15 14:07:41.000000 modnet-0.4.3/modnet/matbench/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    11640 2023-07-11 13:21:01.000000 modnet-0.4.3/modnet/matbench/benchmark.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-05 10:43:47.000000 modnet-0.4.3/modnet/model_presets/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      166 2022-01-10 10:10:32.000000 modnet-0.4.3/modnet/model_presets/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     2292 2021-08-16 13:22:38.000000 modnet-0.4.3/modnet/model_presets/presets.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-05 10:43:47.000000 modnet-0.4.3/modnet/models/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      402 2024-02-07 15:47:41.000000 modnet-0.4.3/modnet/models/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    15169 2024-04-02 15:48:26.000000 modnet-0.4.3/modnet/models/bayesian.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    17887 2024-03-28 10:26:50.000000 modnet-0.4.3/modnet/models/ensemble.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    60336 2024-04-05 10:41:01.000000 modnet-0.4.3/modnet/models/vanilla.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    41991 2024-03-28 10:26:50.000000 modnet-0.4.3/modnet/preprocessing.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     6344 2024-03-28 10:26:50.000000 modnet-0.4.3/modnet/sklearn.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-05 10:43:47.000000 modnet-0.4.3/modnet/tests/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)        0 2020-09-16 10:22:36.000000 modnet-0.4.3/modnet/tests/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     4550 2024-04-02 15:48:26.000000 modnet-0.4.3/modnet/tests/conftest.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     4444 2023-07-11 13:21:01.000000 modnet-0.4.3/modnet/tests/test_benchmark.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      563 2021-01-14 10:39:09.000000 modnet-0.4.3/modnet/tests/test_ext_data.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      771 2024-04-02 15:48:22.000000 modnet-0.4.3/modnet/tests/test_hyper_opt.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    10034 2024-04-05 10:41:01.000000 modnet-0.4.3/modnet/tests/test_model.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    17907 2024-04-02 15:48:26.000000 modnet-0.4.3/modnet/tests/test_preprocessing.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     3110 2022-05-19 13:18:13.000000 modnet-0.4.3/modnet/tests/test_sklearn.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      737 2021-02-15 14:07:41.000000 modnet-0.4.3/modnet/utils.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-05 10:43:46.000000 modnet-0.4.3/modnet.egg-info/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     6057 2024-04-05 10:43:46.000000 modnet-0.4.3/modnet.egg-info/PKG-INFO
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     1110 2024-04-05 10:43:46.000000 modnet-0.4.3/modnet.egg-info/SOURCES.txt
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)        1 2024-04-05 10:43:46.000000 modnet-0.4.3/modnet.egg-info/dependency_links.txt
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      206 2024-04-05 10:43:46.000000 modnet-0.4.3/modnet.egg-info/requires.txt
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)        7 2024-04-05 10:43:46.000000 modnet-0.4.3/modnet.egg-info/top_level.txt
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      118 2024-04-05 10:43:47.000000 modnet-0.4.3/setup.cfg
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     1877 2024-04-02 15:48:26.000000 modnet-0.4.3/setup.py
```

### Comparing `modnet-0.4.2/LICENSE.md` & `modnet-0.4.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `modnet-0.4.2/PKG-INFO` & `modnet-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modnet
-Version: 0.4.2
+Version: 0.4.3
 Summary: MODNet, the Material Optimal Descriptor Network for materials properties prediction. 
 Home-page: https://github.com/ppdebreuck/modnet
 Author: Pierre-Paul De Breuck
 Author-email: pierre-paul.debreuck@uclouvain.be
 License: UNKNOWN
 Project-URL: GitHub, https://github.com/ppdebreuck/modnet
 Project-URL: Documentation, https://modnet.readthedocs.io
```

### Comparing `modnet-0.4.2/README.md` & `modnet-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `modnet-0.4.2/modnet/data/Features_cross` & `modnet-0.4.3/modnet/data/Features_cross`

 * *Files identical despite different names*

### Comparing `modnet-0.4.2/modnet/ext_data.py` & `modnet-0.4.3/modnet/ext_data.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.2/modnet/featurizers/featurizers.py` & `modnet-0.4.3/modnet/featurizers/featurizers.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.2/modnet/featurizers/presets/__init__.py` & `modnet-0.4.3/modnet/featurizers/presets/__init__.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.2/modnet/featurizers/presets/debreuck_2020.py` & `modnet-0.4.3/modnet/featurizers/presets/debreuck_2020.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.2/modnet/featurizers/presets/matminer_2023.py` & `modnet-0.4.3/modnet/featurizers/presets/matminer_2023.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.2/modnet/featurizers/presets/matminer_all_2023.py` & `modnet-0.4.3/modnet/featurizers/presets/matminer_all_2023.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.2/modnet/featurizers/utils.py` & `modnet-0.4.3/modnet/featurizers/utils.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.2/modnet/hyper_opt/fit_genetic.py` & `modnet-0.4.3/modnet/hyper_opt/fit_genetic.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.2/modnet/matbench/benchmark.py` & `modnet-0.4.3/modnet/matbench/benchmark.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.2/modnet/model_presets/presets.py` & `modnet-0.4.3/modnet/model_presets/presets.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.2/modnet/models/bayesian.py` & `modnet-0.4.3/modnet/models/bayesian.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.2/modnet/models/ensemble.py` & `modnet-0.4.3/modnet/models/ensemble.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.2/modnet/models/vanilla.py` & `modnet-0.4.3/modnet/models/vanilla.py`

 * *Files 0% similar despite different names*

```diff
@@ -821,15 +821,17 @@
                 elif loss == "mse":
                     loss = mean_squared_error
                 elif isinstance(loss, str):
                     raise RuntimeError(
                         f"Loss {loss} not recognized. Use mae, mse or a callable."
                     )
                 else:
-                    score.append(loss(y_true, y_pred[i]))
+                    pass
+
+                score.append(loss(y_true, y_pred[i]))
 
         return np.mean(score)
 
     def _make_picklable(self):
         """
         transforms inner keras model to jsons so that th MODNet object becomes picklable.
         """
```

### Comparing `modnet-0.4.2/modnet/preprocessing.py` & `modnet-0.4.3/modnet/preprocessing.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.2/modnet/sklearn.py` & `modnet-0.4.3/modnet/sklearn.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.2/modnet/tests/conftest.py` & `modnet-0.4.3/modnet/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.2/modnet/tests/test_benchmark.py` & `modnet-0.4.3/modnet/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.2/modnet/tests/test_ext_data.py` & `modnet-0.4.3/modnet/tests/test_ext_data.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.2/modnet/tests/test_hyper_opt.py` & `modnet-0.4.3/modnet/tests/test_hyper_opt.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.2/modnet/tests/test_model.py` & `modnet-0.4.3/modnet/tests/test_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python
 import pytest
+import numpy as np
 
 
 def test_train_small_model_single_target(subset_moddata, tf_session):
     """Tests the single target training."""
     from modnet.models import MODNetModel
 
     data = subset_moddata
@@ -17,14 +18,15 @@
         weights={"eform": 1},
         num_neurons=[[16], [8], [8], [4]],
         n_feat=10,
     )
 
     model.fit(data, epochs=2)
     model.predict(data)
+    assert not np.isnan(model.evaluate(data))
 
 
 def test_train_small_model_single_target_classif(subset_moddata, tf_session):
     """Tests the single target training."""
     from modnet.models import MODNetModel
 
     data = subset_moddata
@@ -45,14 +47,15 @@
         weights={"is_metal": 1},
         num_neurons=[[16], [8], [8], [4]],
         num_classes={"is_metal": 2},
         n_feat=10,
     )
 
     model.fit(data, epochs=2)
+    assert not np.isnan(model.evaluate(data))
 
 
 def test_train_small_model_multi_target(subset_moddata, tf_session):
     """Tests the multi-target training."""
     from modnet.models import MODNetModel
 
     data = subset_moddata
@@ -66,14 +69,15 @@
         weights={"eform": 1, "egap": 1},
         num_neurons=[[16], [8], [8], [4]],
         n_feat=10,
     )
 
     model.fit(data, epochs=2)
     model.predict(data)
+    assert not np.isnan(model.evaluate(data))
 
 
 def test_train_small_model_presets(subset_moddata, tf_session):
     """Tests the `fit_preset()` method."""
     from modnet.model_presets import gen_presets
     from modnet.models import MODNetModel
 
@@ -105,14 +109,15 @@
             val_fraction=0.2,
             n_jobs=1,
             refit=True,
         )
         models = results[0]
         assert len(models) == len(modified_presets)
         assert len(models[0]) == num_nested
+    assert not np.isnan(model.evaluate(data))
 
 
 def test_model_integration(subset_moddata, tf_session):
     """Tests training, saving, loading and predictions."""
     from modnet.models import MODNetModel
 
     data = subset_moddata
@@ -130,14 +135,15 @@
 
     model.fit(data, epochs=2)
 
     model.save("test")
     loaded_model = MODNetModel.load("test")
 
     assert model.predict(data).equals(loaded_model.predict(data))
+    assert not np.isnan(model.evaluate(data))
 
 
 def test_train_small_bayesian_single_target(subset_moddata, tf_session):
     """Tests the single target training."""
     from modnet.models import BayesianMODNetModel
 
     data = subset_moddata
@@ -152,14 +158,15 @@
         num_neurons=[[16], [8], [8], [4]],
         n_feat=10,
     )
 
     model.fit(data, epochs=2)
     model.predict(data)
     model.predict(data, return_unc=True)
+    assert not np.isnan(model.evaluate(data))
 
 
 def test_train_small_bayesian_single_target_classif(subset_moddata, tf_session):
     """Tests the single target training."""
     from modnet.models import BayesianMODNetModel
 
     data = subset_moddata
@@ -182,14 +189,15 @@
         num_classes={"is_metal": 2},
         n_feat=10,
     )
 
     model.fit(data, epochs=2)
     model.predict(data)
     model.predict(data, return_unc=True)
+    assert not np.isnan(model.evaluate(data))
 
 
 def test_train_small_bayesian_multi_target(subset_moddata, tf_session):
     """Tests the multi-target training."""
     from modnet.models import BayesianMODNetModel
 
     data = subset_moddata
@@ -204,14 +212,15 @@
         num_neurons=[[16], [8], [8], [4]],
         n_feat=10,
     )
 
     model.fit(data, epochs=2)
     model.predict(data)
     model.predict(data, return_unc=True)
+    assert not np.isnan(model.evaluate(data))
 
 
 def test_train_small_bootstrap_single_target(subset_moddata, tf_session):
     """Tests the single target training."""
     from modnet.models import EnsembleMODNetModel
 
     data = subset_moddata
@@ -228,14 +237,15 @@
         n_models=3,
         bootstrap=True,
     )
 
     model.fit(data, epochs=2)
     model.predict(data)
     model.predict(data, return_unc=True)
+    assert not np.isnan(model.evaluate(data))
 
 
 def test_train_small_bootstrap_single_target_classif(small_moddata, tf_session):
     """Tests the single target training."""
     from modnet.models import EnsembleMODNetModel
 
     data = small_moddata
@@ -260,14 +270,15 @@
         n_models=3,
         bootstrap=True,
     )
 
     model.fit(data, epochs=2)
     model.predict(data)
     model.predict(data, return_unc=True)
+    assert not np.isnan(model.evaluate(data))
 
 
 def test_train_small_bootstrap_multi_target(small_moddata, tf_session):
     """Tests the multi-target training."""
     from modnet.models import EnsembleMODNetModel
 
     data = small_moddata
@@ -329,7 +340,9 @@
             val_fraction=0.2,
             n_jobs=2,
         )
         print(f"{time.time() - start} elapsed nested {num_nested}, {nested_option}")
         models = results[0]
         assert len(models) == len(modified_presets)
         assert len(models[0]) == num_nested
+
+        assert not np.isnan(model.evaluate(data))
```

### Comparing `modnet-0.4.2/modnet/tests/test_preprocessing.py` & `modnet-0.4.3/modnet/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.2/modnet/tests/test_sklearn.py` & `modnet-0.4.3/modnet/tests/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.2/modnet/utils.py` & `modnet-0.4.3/modnet/utils.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.2/modnet.egg-info/PKG-INFO` & `modnet-0.4.3/modnet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modnet
-Version: 0.4.2
+Version: 0.4.3
 Summary: MODNet, the Material Optimal Descriptor Network for materials properties prediction. 
 Home-page: https://github.com/ppdebreuck/modnet
 Author: Pierre-Paul De Breuck
 Author-email: pierre-paul.debreuck@uclouvain.be
 License: UNKNOWN
 Project-URL: GitHub, https://github.com/ppdebreuck/modnet
 Project-URL: Documentation, https://modnet.readthedocs.io
```

### Comparing `modnet-0.4.2/modnet.egg-info/SOURCES.txt` & `modnet-0.4.3/modnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modnet-0.4.2/setup.py` & `modnet-0.4.3/setup.py`

 * *Files identical despite different names*

