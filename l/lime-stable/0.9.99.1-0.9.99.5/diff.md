# Comparing `tmp/lime-stable-0.9.99.1.tar.gz` & `tmp/lime-stable-0.9.99.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lime-stable-0.9.99.1.tar", last modified: Wed Mar 27 17:48:46 2024, max compression
+gzip compressed data, was "lime-stable-0.9.99.5.tar", last modified: Fri Apr  5 18:40:01 2024, max compression
```

## Comparing `lime-stable-0.9.99.1.tar` & `lime-stable-0.9.99.5.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-03-27 17:48:46.417144 lime-stable-0.9.99.1/
--rw-rw-r--   0 vital     (1000) vital     (1000)    35608 2024-01-06 20:52:21.000000 lime-stable-0.9.99.1/LICENSE.rst
--rw-rw-r--   0 vital     (1000) vital     (1000)      144 2024-01-06 20:52:21.000000 lime-stable-0.9.99.1/MANIFEST.in
--rw-r--r--   0 vital     (1000) vital     (1000)     3638 2024-03-27 17:48:46.417144 lime-stable-0.9.99.1/PKG-INFO
--rw-rw-r--   0 vital     (1000) vital     (1000)     2684 2024-01-06 20:52:21.000000 lime-stable-0.9.99.1/README.rst
--rw-rw-r--   0 vital     (1000) vital     (1000)     1149 2024-03-27 17:47:48.000000 lime-stable-0.9.99.1/pyproject.toml
--rw-rw-r--   0 vital     (1000) vital     (1000)      436 2024-03-27 17:48:46.417144 lime-stable-0.9.99.1/setup.cfg
--rw-rw-r--   0 vital     (1000) vital     (1000)     1367 2024-02-07 20:40:09.000000 lime-stable-0.9.99.1/setup.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-03-27 17:48:46.413144 lime-stable-0.9.99.1/src/
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-03-27 17:48:46.413144 lime-stable-0.9.99.1/src/lime/
--rw-rw-r--   0 vital     (1000) vital     (1000)     1529 2024-02-07 21:15:07.000000 lime-stable-0.9.99.1/src/lime/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)      134 2024-03-27 17:47:48.000000 lime-stable-0.9.99.1/src/lime/config.toml
--rw-rw-r--   0 vital     (1000) vital     (1000)    39465 2024-03-27 17:47:48.000000 lime-stable-0.9.99.1/src/lime/io.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     2809 2024-03-20 19:32:47.000000 lime-stable-0.9.99.1/src/lime/logo.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    39061 2024-03-27 17:47:48.000000 lime-stable-0.9.99.1/src/lime/model.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    72799 2024-03-27 17:47:48.000000 lime-stable-0.9.99.1/src/lime/observations.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    81756 2024-02-15 20:43:53.000000 lime-stable-0.9.99.1/src/lime/plots.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    70825 2024-02-15 20:43:46.000000 lime-stable-0.9.99.1/src/lime/plots_interactive.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    31175 2024-03-22 14:35:43.000000 lime-stable-0.9.99.1/src/lime/read_fits.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    17583 2024-03-27 17:47:48.000000 lime-stable-0.9.99.1/src/lime/recognition.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-03-27 17:48:46.413144 lime-stable-0.9.99.1/src/lime/resources/
--rw-rw-r--   0 vital     (1000) vital     (1000)     1100 2024-01-06 20:52:21.000000 lime-stable-0.9.99.1/src/lime/resources/GradientDescent_v2_cost1_logNorm.joblib
--rw-rw-r--   0 vital     (1000) vital     (1000)      858 2024-01-06 20:52:21.000000 lime-stable-0.9.99.1/src/lime/resources/LogitistRegression_v2_cost1_logNorm.joblib
--rw-rw-r--   0 vital     (1000) vital     (1000)    15311 2024-01-06 20:52:21.000000 lime-stable-0.9.99.1/src/lime/resources/parent_bands.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)    15311 2024-01-06 20:52:21.000000 lime-stable-0.9.99.1/src/lime/resources/parent_mask_v0.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)     2842 2024-01-06 20:52:21.000000 lime-stable-0.9.99.1/src/lime/resources/sketch.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     9855 2024-03-27 17:47:48.000000 lime-stable-0.9.99.1/src/lime/resources/types_params.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)     9100 2024-01-31 19:44:41.000000 lime-stable-0.9.99.1/src/lime/resources/types_params2.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)    14172 2024-02-13 22:39:44.000000 lime-stable-0.9.99.1/src/lime/tables.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    28577 2024-03-27 17:47:48.000000 lime-stable-0.9.99.1/src/lime/tools.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    27613 2024-03-27 17:47:48.000000 lime-stable-0.9.99.1/src/lime/transitions.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    35389 2024-03-27 17:47:48.000000 lime-stable-0.9.99.1/src/lime/workflow.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-03-27 17:48:46.413144 lime-stable-0.9.99.1/src/lime_stable.egg-info/
--rw-r--r--   0 vital     (1000) vital     (1000)     3638 2024-03-27 17:48:46.000000 lime-stable-0.9.99.1/src/lime_stable.egg-info/PKG-INFO
--rw-rw-r--   0 vital     (1000) vital     (1000)     1035 2024-03-27 17:48:46.000000 lime-stable-0.9.99.1/src/lime_stable.egg-info/SOURCES.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)        1 2024-03-27 17:48:46.000000 lime-stable-0.9.99.1/src/lime_stable.egg-info/dependency_links.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)      257 2024-03-27 17:48:46.000000 lime-stable-0.9.99.1/src/lime_stable.egg-info/requires.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)        5 2024-03-27 17:48:46.000000 lime-stable-0.9.99.1/src/lime_stable.egg-info/top_level.txt
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-03-27 17:48:46.417144 lime-stable-0.9.99.1/tests/
--rw-rw-r--   0 vital     (1000) vital     (1000)      991 2024-01-06 20:52:21.000000 lime-stable-0.9.99.1/tests/test_astro.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     7086 2024-03-25 19:38:26.000000 lime-stable-0.9.99.1/tests/test_cube.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     3547 2024-01-31 22:26:33.000000 lime-stable-0.9.99.1/tests/test_io.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     7455 2024-01-19 22:37:34.000000 lime-stable-0.9.99.1/tests/test_line.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4388 2024-02-15 20:55:38.000000 lime-stable-0.9.99.1/tests/test_model.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     2346 2024-01-16 14:15:34.000000 lime-stable-0.9.99.1/tests/test_read_fits.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     1991 2024-01-06 20:52:21.000000 lime-stable-0.9.99.1/tests/test_sample.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    11134 2024-03-27 17:47:48.000000 lime-stable-0.9.99.1/tests/test_spectrum.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    13350 2024-02-22 18:08:19.000000 lime-stable-0.9.99.1/tests/test_tools.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-05 18:40:01.430581 lime-stable-0.9.99.5/
+-rw-rw-r--   0 vital     (1000) vital     (1000)    35608 2024-01-06 20:52:21.000000 lime-stable-0.9.99.5/LICENSE.rst
+-rw-rw-r--   0 vital     (1000) vital     (1000)      144 2024-01-06 20:52:21.000000 lime-stable-0.9.99.5/MANIFEST.in
+-rw-r--r--   0 vital     (1000) vital     (1000)     3638 2024-04-05 18:40:01.430581 lime-stable-0.9.99.5/PKG-INFO
+-rw-rw-r--   0 vital     (1000) vital     (1000)     2684 2024-01-06 20:52:21.000000 lime-stable-0.9.99.5/README.rst
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1149 2024-04-05 18:12:49.000000 lime-stable-0.9.99.5/pyproject.toml
+-rw-rw-r--   0 vital     (1000) vital     (1000)      436 2024-04-05 18:40:01.430581 lime-stable-0.9.99.5/setup.cfg
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1367 2024-02-07 20:40:09.000000 lime-stable-0.9.99.5/setup.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-05 18:40:01.426581 lime-stable-0.9.99.5/src/
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-05 18:40:01.430581 lime-stable-0.9.99.5/src/lime/
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1528 2024-04-03 19:45:09.000000 lime-stable-0.9.99.5/src/lime/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     2438 2024-04-05 18:12:49.000000 lime-stable-0.9.99.5/src/lime/config.toml
+-rw-rw-r--   0 vital     (1000) vital     (1000)    31035 2024-04-04 18:46:13.000000 lime-stable-0.9.99.5/src/lime/io.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     2809 2024-03-20 19:32:47.000000 lime-stable-0.9.99.5/src/lime/logo.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    38583 2024-04-05 18:09:59.000000 lime-stable-0.9.99.5/src/lime/model.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    73078 2024-04-05 15:48:29.000000 lime-stable-0.9.99.5/src/lime/observations.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    82193 2024-04-05 14:08:28.000000 lime-stable-0.9.99.5/src/lime/plots.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    70363 2024-04-04 22:15:39.000000 lime-stable-0.9.99.5/src/lime/plots_interactive.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    31175 2024-03-22 14:35:43.000000 lime-stable-0.9.99.5/src/lime/read_fits.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    17248 2024-04-04 14:44:02.000000 lime-stable-0.9.99.5/src/lime/recognition.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-05 18:40:01.430581 lime-stable-0.9.99.5/src/lime/resources/
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1100 2024-01-06 20:52:21.000000 lime-stable-0.9.99.5/src/lime/resources/GradientDescent_v2_cost1_logNorm.joblib
+-rw-rw-r--   0 vital     (1000) vital     (1000)      858 2024-01-06 20:52:21.000000 lime-stable-0.9.99.5/src/lime/resources/LogitistRegression_v2_cost1_logNorm.joblib
+-rw-rw-r--   0 vital     (1000) vital     (1000)      144 2024-04-05 15:26:56.000000 lime-stable-0.9.99.5/src/lime/resources/adjust_bands_database.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    17051 2024-04-05 15:27:04.000000 lime-stable-0.9.99.5/src/lime/resources/parent_bands.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)    16094 2024-04-05 15:05:16.000000 lime-stable-0.9.99.5/src/lime/resources/parent_mask_v0.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)     2842 2024-01-06 20:52:21.000000 lime-stable-0.9.99.5/src/lime/resources/sketch.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     9855 2024-03-27 17:47:48.000000 lime-stable-0.9.99.5/src/lime/resources/types_params.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)     9100 2024-01-31 19:44:41.000000 lime-stable-0.9.99.5/src/lime/resources/types_params2.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)    14172 2024-02-13 22:39:44.000000 lime-stable-0.9.99.5/src/lime/tables.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    37522 2024-04-03 15:58:07.000000 lime-stable-0.9.99.5/src/lime/tools.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    27774 2024-04-05 15:01:34.000000 lime-stable-0.9.99.5/src/lime/transitions.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    35814 2024-04-03 15:31:58.000000 lime-stable-0.9.99.5/src/lime/workflow.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-05 18:40:01.430581 lime-stable-0.9.99.5/src/lime_stable.egg-info/
+-rw-r--r--   0 vital     (1000) vital     (1000)     3638 2024-04-05 18:40:01.000000 lime-stable-0.9.99.5/src/lime_stable.egg-info/PKG-INFO
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1079 2024-04-05 18:40:01.000000 lime-stable-0.9.99.5/src/lime_stable.egg-info/SOURCES.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)        1 2024-04-05 18:40:01.000000 lime-stable-0.9.99.5/src/lime_stable.egg-info/dependency_links.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)      257 2024-04-05 18:40:01.000000 lime-stable-0.9.99.5/src/lime_stable.egg-info/requires.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)        5 2024-04-05 18:40:01.000000 lime-stable-0.9.99.5/src/lime_stable.egg-info/top_level.txt
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-05 18:40:01.430581 lime-stable-0.9.99.5/tests/
+-rw-rw-r--   0 vital     (1000) vital     (1000)      993 2024-04-02 21:30:23.000000 lime-stable-0.9.99.5/tests/test_astro.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     7092 2024-04-02 21:30:24.000000 lime-stable-0.9.99.5/tests/test_cube.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     3549 2024-04-02 21:30:23.000000 lime-stable-0.9.99.5/tests/test_io.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     7626 2024-04-05 15:36:26.000000 lime-stable-0.9.99.5/tests/test_line.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4388 2024-02-15 20:55:38.000000 lime-stable-0.9.99.5/tests/test_model.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     2346 2024-01-16 14:15:34.000000 lime-stable-0.9.99.5/tests/test_read_fits.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1997 2024-04-02 21:30:23.000000 lime-stable-0.9.99.5/tests/test_sample.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    11168 2024-04-02 21:34:26.000000 lime-stable-0.9.99.5/tests/test_spectrum.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    13366 2024-04-02 21:30:23.000000 lime-stable-0.9.99.5/tests/test_tools.py
```

### Comparing `lime-stable-0.9.99.1/LICENSE.rst` & `lime-stable-0.9.99.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `lime-stable-0.9.99.1/PKG-INFO` & `lime-stable-0.9.99.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lime-stable
-Version: 0.9.99.1
+Version: 0.9.99.5
 Summary: Line measuring algorithm for astronomical spectra
 Home-page: https://github.com/Vital-Fernandez/lime
 Author: Vital Fernandez
 Author-email: Vital Fernández <vgf@umich.edu>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `lime-stable-0.9.99.1/README.rst` & `lime-stable-0.9.99.5/README.rst`

 * *Files identical despite different names*

### Comparing `lime-stable-0.9.99.1/pyproject.toml` & `lime-stable-0.9.99.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lime-stable"
-version = "0.9.99.1"
+version = "0.9.99.5"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {file = "COPYING"}
 authors = [{name = "Vital Fernández", email = "vgf@umich.edu"}]
 description = "Line measuring algorithm for astronomical spectra"
 
 dependencies = ["joblib==1.3.1",
```

### Comparing `lime-stable-0.9.99.1/setup.py` & `lime-stable-0.9.99.5/setup.py`

 * *Files identical despite different names*

### Comparing `lime-stable-0.9.99.1/src/lime/__init__.py` & `lime-stable-0.9.99.5/src/lime/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -49,8 +49,8 @@
 
 from .observations import Spectrum, Sample, Cube, line_bands
 from .io import *
 from .tools import *
 from .transitions import Line, label_decomposition
 from .read_fits import OpenFits
 from .recognition import detection_function
-from .plots import theme
+from .plots import theme
```

### Comparing `lime-stable-0.9.99.1/src/lime/io.py` & `lime-stable-0.9.99.5/src/lime/io.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 __all__ = [
     'save_cfg',
     'load_cfg',
-    'load_log',
+    'load_frame',
     'load_spatial_mask',
-    'save_log',
+    'save_frame',
     'log_parameters_calculation',
     'log_to_HDU',
-    'save_parameter_maps',
     '_LOG_EXPORT_RECARR',
     '_LOG_EXPORT',
     '_LOG_COLUMNS']
 
 import os
 import configparser
 import logging
@@ -52,18 +51,24 @@
     toml_check = True
 except ImportError:
     toml_check = False
 
 _logger = logging.getLogger('LiMe')
 
 # Reading file with the format and export status for the measurements
-_params_table_file = Path(__file__).parent/'resources/types_params.txt'
+_LIME_FOLDER = Path(__file__).parent
+_params_table_file = _LIME_FOLDER/'resources/types_params.txt'
 _PARAMS_CONF_TABLE = pd.read_csv(_params_table_file, delim_whitespace=True, header=0, index_col=0)
 
-_LINES_DATABASE_FILE = Path(__file__).parent/'resources/parent_bands.txt'
+_LINES_DATABASE_FILE = _LIME_FOLDER/'resources/parent_bands.txt'
+_CONF_FILE = _LIME_FOLDER/'config.toml'
+
+# # Read lime configuration file
+# with open(_CONF_FILE, mode="rb") as fp:
+#     _cfg_lime = tomllib.load(fp)
 
 # Dictionary with the parameter formart
 _LOG_COLUMNS = dict(zip(_PARAMS_CONF_TABLE.index.values,
                         _PARAMS_CONF_TABLE.loc[:, 'Norm_by_flux':'dtype'].values))
 
 # Parameters notation latex formatDictionary with the parameter formart
 _LOG_COLUMNS_LATEX = dict(zip(_PARAMS_CONF_TABLE.index.values,
@@ -243,45 +248,45 @@
             # Save to a text file
             with open(output_file, 'w') as f:
                 output_cfg.write(f)
 
     return
 
 
-def load_log(file_address, page: str = 'LINELOG', levels: list = ['id', 'line']):
+def load_frame(fname, page: str = 'LINELOG', levels: list = ['id', 'line']):
 
     """
     This function reads the input ``file_address`` as a pandas dataframe.
 
     The expected file types are ".txt", ".pdf", ".fits", ".asdf" and ".xlsx". The dataframes expected format is discussed
     on the `line bands <https://lime-stable.readthedocs.io/en/latest/inputs/n_inputs3_line_bands.html>`_ and `measurements <https://lime-stable.readthedocs.io/en/latest/inputs/n_inputs4_fit_configuration.html>`_ documentation.
 
     For ".fits" and ".xlsx" files the user can provide a page name ``ext`` for the HDU/sheet. The default name is "_LINELOG".
 
     To reconstruct a `MultiIndex dataframe <https://pandas.pydata.org/docs/user_guide/advanced.html#advanced-hierarchical>`_
     the user needs to specify the ``sample_levels``.
 
-    :param file_address: Input log address.
-    :type file_address: str, Path
+    :param fname: Lines frame file address.
+    :type fname: str, Path
 
     :param page: Name of the HDU/sheet for ".fits"/".xlsx" files. The default value is "_LINELOG".
     :type page: str, optional
 
     :param levels: Indexes name list for MultiIndex dataframes. The default value is ['id', 'line'].
     :type levels: list, optional
 
     :return: lines log table
     :rtype: pandas.DataFrame
 
     """
 
     # Check file is at path
-    log_path = Path(file_address)
+    log_path = Path(fname)
     if not log_path.is_file():
-        raise LiMe_Error(f'No lines log found at {file_address}\n')
+        raise LiMe_Error(f'No lines log found at {fname}\n')
 
     file_name, file_type = log_path.name, log_path.suffix
 
     try:
 
         # Fits file:
         if file_type == '.fits':
@@ -319,37 +324,37 @@
     # Restore levels if multi-index
     if log.columns.isin(levels).sum() == len(levels):
         log.set_index(levels, inplace=True)
 
     return log
 
 
-def save_log(dataframe, file_address, page='LINELOG', parameters='all', header=None, column_dtypes=None,
-             safe_version=True, **kwargs):
+def save_frame(fname, dataframe, page='LINELOG', parameters='all', header=None, column_dtypes=None,
+               safe_version=True, **kwargs):
 
     """
 
-    This function saves the input ``log_dataframe`` at the ``file_address`` provided by the user.
+    This function saves the input ``dataframe`` at the ``fname`` provided by the user.
 
     The accepted extensions are ".txt", ".pdf", ".fits", ".asdf" and ".xlsx".
 
     For ".fits" and ".xlsx" files the user can provide a page name for the HDU/sheet with the ``ext`` argument.
     The default name is "LINELOG".
 
     The user can specify the ``parameters`` to be saved in the output file.
 
     For ".fits" files the user can provide a dictionary to add to the ``fits_header``. The user can provide a ``column_dtypes``
     string or dictionary for the output fits file record array. This overwrites LiMe deafult formatting and it must have the
     same columns as the file names.
 
-    :param dataframe: Lines log dataframe.
-    :type dataframe: pandas.DataFrame
+    :param fname: Lines frame file address.
+    :type fname: str, Path
 
-    :param file_address: Output log address.
-    :type file_address: str, Path
+    :param dataframe: Lines dataframe.
+    :type dataframe: pandas.DataFrame
 
     :param parameters: Output parameters list. The default value is "all"
     :type parameters: list
 
     :param page: Name of the HDU/sheet for ".fits"/".xlsx" files.
     :type page: str, optional
 
@@ -363,15 +368,15 @@
 
     :param safe_version: Save LiMe version as footnote or page header on the output log. The default value is True.
     :type safe_version: bool, optional
 
     """
 
     # Confirm file path exits
-    log_path = Path(file_address)
+    log_path = Path(fname)
     assert log_path.parent.exists(), LiMe_Error(f'- ERROR: Output lines log folder not found: {log_path.parent}')
     file_name, file_type = log_path.name, log_path.suffix
 
     if len(dataframe.index) > 0:
 
         # In case of multi-index dataframe
         if isinstance(dataframe.index, pd.MultiIndex):
@@ -473,15 +478,15 @@
                         if len(row) > 1: # TOFIX Remove the frozen list logic
                             sheet.append(row)
 
                     # Save the data
                     wb.save(log_path)
 
             else:
-                _logger.critical(f'openpyxl is not installed. Lines log {file_address} could not be saved')
+                _logger.critical(f'openpyxl is not installed. Lines log {fname} could not be saved')
 
         # Advance Scientific Storage Format
         elif file_type == '.asdf':
             # TODO review this one and add the metadata
             tree = {page: lines_log.to_records(index=True, column_dtypes=_LOG_TYPES_DICT, index_dtypes='<U50')}
 
             # Create new file
@@ -555,15 +560,15 @@
             output = df_variable.copy()
         else:
             output = df_variable
 
     elif isinstance(df_variable, (str, Path)):
         input_path = Path(df_variable)
         if input_path.is_file():
-            output = load_log(df_variable, page=ext, levels=sample_levels)
+            output = load_frame(df_variable, page=ext, levels=sample_levels)
         else:
             _logger.warning(f'Lines bands file not found at {df_variable}')
             output = None
 
     else:
         output = df_variable
 
@@ -634,15 +639,15 @@
     else:
         output_cfg = {}
 
     return output_cfg
 
 
 _parent_bands_file = Path(__file__).parent/'resources/parent_bands.txt'
-_PARENT_BANDS = load_log(_parent_bands_file)
+_PARENT_BANDS = load_frame(_parent_bands_file)
 
 
 def check_numeric_value(s):
 
     # Function to check if variable can be converte to float else leave as string
 
     try:
@@ -693,15 +698,15 @@
     # Load the log if necessary file:
     file_check = False
     if isinstance(input_log, pd.DataFrame):
         log_df = input_log
 
     elif isinstance(input_log, (str, Path)):
         file_check = True
-        log_df = load_log(input_log)
+        log_df = load_frame(input_log)
 
     else:
         _logger.critical(
             f'Not a recognize log format. Please use a pandas dataframe or a string/Path object for file {input_log}')
         exit(1)
 
     # Parse the combined expression
@@ -710,47 +715,20 @@
         expr += f'{col}={formula}\n'
 
     # Compute the new parameters
     log_df.eval(expr=expr, inplace=True)
 
     # Save to the previous location
     if file_check:
-        save_log(log_df, input_log)
+        save_frame(log_df, input_log)
 
 
     return
 
 
-def extract_wcs_header(wcs, drop_axis=None):
-
-    if wcs is not None:
-
-        # Remove 3rd dimensional axis if present
-        if drop_axis is not None:
-            if drop_axis == 'spectral':
-                input_wcs = wcs.dropaxis(2) if wcs.naxis == 3 else wcs
-            elif drop_axis == 'spatial':
-                if wcs.naxis == 3:
-                    input_wcs = wcs.dropaxis(1)
-                    input_wcs = wcs.dropaxis(0)
-            else:
-                raise LiMe_Error(f'Fits coordinates axis: "{drop_axis}" not recognized. Please use: "spectral" or'
-                                 f' "spatial"')
-
-        else:
-            input_wcs = wcs
-
-        # Convert to HDU header
-        hdr_coords = input_wcs.to_fits()[0].header
-
-    else:
-        hdr_coords = None
-
-    return hdr_coords
-
 
 def log_to_HDU(log, ext_name=None, column_dtypes=None, header_dict=None):
 
     # For non empty logs
     if not log.empty:
 
         if column_dtypes is None:
@@ -811,209 +789,27 @@
 
     else:
         formatted_value = 'None'
 
     return formatted_value
 
 
-def progress_bar(i, i_max, post_text, n_bar=10):
-
-    # Size of progress bar
-    j = i/i_max
-    stdout.write('\r')
-    message = f"[{'=' * int(n_bar * j):{n_bar}s}] {int(100 * j)}% {post_text}"
-    stdout.write(message)
-    stdout.flush()
-
-    return
-
-
-def save_parameter_maps(lines_log_file, output_folder, param_list, line_list, mask_file=None, mask_list='all',
-                        image_shape=None, log_ext_suffix='_LINELOG', spaxel_fill_value=np.nan, output_file_prefix=None,
-                        header=None, wcs=None):
+# def progress_bar(i, i_max, post_text, n_bar=10):
+#
+#     # Size of progress bar
+#     j = i/i_max
+#     stdout.write('\r')
+#     message = f"[{'=' * int(n_bar * j):{n_bar}s}] {int(100 * j)}% {post_text}"
+#     stdout.write(message)
+#     stdout.flush()
+#
+#     return
 
-    """
-
-    This function converts a line measurements log from an IFS cube, into a set of 2D parameter maps.
-
-    The parameter ".fits" files are saved into the ``output_folder``. These files are named after the parameters in the
-    ``param_list`` with the optional prefix from the ``output_file_prefix`` argument. These files will have one page per
-    line in the ``line_list`` argument.
-
-    The user can provide a spatial mask file address from which to recover the spaxels with line measurements. If the
-    mask ``.fits`` file contains several pages, the user can provide a ``mask_list`` with the ones to explore. Otherwise,
-    all mask pages will be used.
-
-    .. attention::
-        The user can provide an ``image_shape`` tuple to generate the output parameter map. However, for a large image
-        size this approach may require a long time to query the log file pages.
-
-    The expected page name in the input ``lines_log_file`` is "idx_j-idx_i_log_ext_suffix" where "idx_j" and "idx_i"
-    are the y and x array coordinates of the cube coordinates, by default ``log_ext_suffix='_LINELOG'``.
-
-    The output ``.fits`` parameter page header includes the ``PARAM`` and ``LINE`` entries with the line and parameter
-    labels respectively. The user should also include a ``wcs`` argument to export the astronomical coordinates to the
-    output files. The user can add additional information via the ``header`` argument.
-
-    :param lines_log_file: Fits file with IFU cube line measurements.
-    :param lines_log_file: str, pathlib.Path
-
-    :param param_list: List of parameters to map
-    :param param_list: list
 
-    :param line_list: List of lines to map
-    :param line_list: list
-
-    :param output_folder: Output folder to save the maps
-    :param output_folder: str, pathlib.Path
-
-    :param mask_file: Address of binary spatial mask file
-    :type mask_file: str, pathlib.Path
-
-    :param mask_list: Mask name list to explore on the ``mask_file``.
-    :type mask_list: list, optional
-
-    :param image_shape: Array with the image spatial size.
-    :param image_shape: list, tuple, optional
-
-    :param spaxel_fill_value: Map filling value for empty pixels. The default value is "numpy.nan".
-    :param spaxel_fill_value: float, optional
-
-    :param log_ext_suffix: Suffix for the lines log extension. The default value is "_LINELOG"
-    :param log_ext_suffix: str, optional
-
-    :param output_file_prefix: Prefix for the output parameter ".fits" file. The default value is None.
-    :param output_file_prefix: str, optional
-
-    :param header: Dictionary for parameter ".fits" file header
-    :type header: dict, optional
 
-    :param wcs: Observation `world coordinate system <https://docs.astropy.org/en/stable/wcs/index.html>`_.
-    :type wcs: astropy WCS, optional
-
-    """
-
-    assert Path(lines_log_file).is_file(), f'- ERROR: lines log at {lines_log_file} not found'
-    assert Path(output_folder).is_dir(), f'- ERROR: Output parameter maps folder {output_folder} not found'
-
-    # Compile the list of voxels to recover the provided masks
-    if mask_file is not None:
-
-        assert Path(mask_file).is_file(), f'- ERROR: mask file at {mask_file} not found'
-
-        with fits.open(mask_file) as maskHDUs:
-
-            # Get the list of mask extensions
-            if mask_list == 'all':
-                if ('PRIMARY' in maskHDUs) and (len(maskHDUs) > 1):
-                    mask_list = []
-                    for i, HDU in enumerate(maskHDUs):
-                        mask_name = HDU.name
-                        if mask_name != 'PRIMARY':
-                            mask_list.append(mask_name)
-                    mask_list = np.array(mask_list)
-                else:
-                    mask_list = np.array(['PRIMARY'])
-            else:
-                mask_list = np.array(mask_list, ndmin=1)
-
-            # Combine all the mask voxels into one
-            for i, mask_name in enumerate(mask_list):
-                if i == 0:
-                    mask_array = maskHDUs[mask_name].data
-                    image_shape = mask_array.shape
-                else:
-                    assert image_shape == maskHDUs[mask_name].data.shape, '- ERROR: Input masks do not have the same dimensions'
-                    mask_array += maskHDUs[mask_name].data
-
-            # Convert to boolean
-            mask_array = mask_array.astype(bool)
-
-            # List of spaxels in list [(idx_j, idx_i), ...] format
-            spaxel_list = np.argwhere(mask_array)
-
-    # No mask file is provided and the user just defines an image size tupple (nY, nX)
-    else:
-        mask_array = np.ones(image_shape).astype(bool)
-        spaxel_list = np.argwhere(mask_array)
-
-    # Generate containers for the data:
-    images_dict = {}
-    for param in param_list:
-
-        # Make sure is an array and loop throuh them
-        for line in line_list:
-            images_dict[f'{param}-{line}'] = np.full(image_shape, spaxel_fill_value)
-
-    # Loop through the spaxels and fill the parameter images
-    n_spaxels = spaxel_list.shape[0]
-    spaxel_range = np.arange(n_spaxels)
-
-    with fits.open(lines_log_file) as logHDUs:
-
-        for i_spaxel in spaxel_range:
-            idx_j, idx_i = spaxel_list[i_spaxel]
-            spaxel_ref = f'{idx_j}-{idx_i}{log_ext_suffix}'
-
-            progress_bar(i_spaxel, n_spaxels, post_text=f'of spaxels from file ({lines_log_file}) read ({n_spaxels} total spaxels)')
-
-            # Confirm log extension exists
-            if spaxel_ref in logHDUs:
-
-                # Recover extension data
-                log_data = logHDUs[spaxel_ref].data
-                log_lines = log_data['index']
-
-                # Loop through the parameters and the lines:
-                for param in param_list:
-                    idcs_log = np.argwhere(np.in1d(log_lines, line_list))
-                    for i_line in idcs_log:
-                        images_dict[f'{param}-{log_lines[i_line][0]}'][idx_j, idx_i] = log_data[param][i_line][0]
-
-    # New line after the rustic progress bar
-    print()
-
-    # Recover coordinates from the wcs to store in the headers:
-    hdr_coords = extract_wcs_header(wcs, drop_axis='spectral')
-
-    # Save the parameter maps as individual fits files with one line per page
-    output_file_prefix = '' if output_file_prefix is None else output_file_prefix
-    for param in param_list:
-
-        # Primary header
-        paramHDUs = fits.HDUList()
-        paramHDUs.append(fits.PrimaryHDU())
-
-        # ImageHDU for the parameter maps
-        for line in line_list:
-
-            # Create page header with the default data
-            hdr_i = fits.Header()
-            hdr_i['LINE'] = (line, 'Line label')
-            hdr_i['PARAM'] = (param, 'LiMe parameter label')
-
-            # Add WCS information
-            if hdr_coords is not None:
-                hdr_i.update(hdr_coords)
-
-            # Add user information
-            if header is not None:
-                page_hdr = header.get(f'{param}-{line}', None)
-                page_hdr = header if page_hdr is None else page_hdr
-                hdr_i.update(page_hdr)
-
-            # Create page HDU entry
-            HDU_i = fits.ImageHDU(name=line, data=images_dict[f'{param}-{line}'], header=hdr_i, ver=1)
-            paramHDUs.append(HDU_i)
-
-        # Write to new file
-        output_file = Path(output_folder)/f'{output_file_prefix}{param}.fits'
-        paramHDUs.writeto(output_file, overwrite=True, output_verify='fix')
-
-    return
 
 
 def load_spatial_mask(mask_file, mask_list=None, return_coords=False):
 
     # Masks array container
     spatial_mask_dict = {}
```

### Comparing `lime-stable-0.9.99.1/src/lime/logo.py` & `lime-stable-0.9.99.5/src/lime/logo.py`

 * *Files identical despite different names*

### Comparing `lime-stable-0.9.99.1/src/lime/model.py` & `lime-stable-0.9.99.5/src/lime/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -511,15 +511,14 @@
             y_in = y.data[idcs_good]
             weights_in = weights[idcs_good]
         else:
             x_in, y_in, weights_in = x, y, weights
 
         # Fit the line
         self.params = self.model.make_params()
-        # self.output = self.model.fit(y_in, self.params, x=x_in, weights=weights_in, method=method, nan_policy='omit')
 
         with warnings.catch_warnings():
             warnings.simplefilter(_VERBOSE_WARNINGS)
             self.output = self.model.fit(y_in, self.params, x=x_in, weights=weights_in, method=method, nan_policy='omit')
 
         # Check fitting quality
         self.review_fitting(line)
@@ -559,14 +558,19 @@
                 line.profile_flux = np.full(self.n_comps, np.nan)
                 line.profile_flux_err = np.full(self.n_comps, np.nan)
                 line.eqw = np.full(self.n_comps, np.nan)
                 line.eqw_err = np.full(self.n_comps, np.nan)
                 line.FWHM_p = np.full(self.n_comps, np.nan)
                 line.sigma_thermal = np.full(self.n_comps, np.nan)
 
+            # Check for negative sigmas # TODO this needs a better place
+            if line.sigma[i] < 0:
+                _logger.warning(f'Negative value for profile sigma at {line.label}')
+                line.sigma[i] = np.nan
+
             # Compute the profile areas
             profile_flux_dist = AREA_FUNCTIONS[line._p_shape[i]](line, i, 1000)
             line.profile_flux[i] = np.mean(profile_flux_dist)
             line.profile_flux_err[i] = np.std(profile_flux_dist)
 
             # Compute FWHM_p (Profile Full Width Half Maximum)
             line.FWHM_p[i] = FWHM_FUNCTIONS[line._p_shape[i]](line, i)
@@ -741,16 +745,14 @@
         self.profile = None
 
         return
 
     def integrated_properties(self, line, emis_wave, emis_flux, emis_err, cont_wave, cont_flux, cont_err, emission_check,
                               n_steps=1000):
 
-
-
         # Assign values peak/through properties
         peakIdx = np.argmax(emis_flux) if emission_check else np.argmin(emis_flux)
         line.n_pixels = emis_wave.size
         line.peak_wave = emis_wave[peakIdx]
         line.peak_flux = emis_flux[peakIdx]
         line.pixelWidth = np.diff(emis_wave).mean()
 
@@ -778,26 +780,14 @@
             line.m_cont_err_intg = np.nan if m_param is None else m_param.stderr
             line.n_cont_err_intg = np.nan if n_param is None else n_param.stderr
 
             # Use the standard deviation from the continuum minus the linear fitting as the continuum error
             line.cont = line.peak_wave * line.m_cont + line.n_cont
             line.cont_err = np.std((cont_wave * line.m_cont + line.n_cont) - cont_flux)
 
-            # Using the middle point has a lot uncertainty
-            # from matplotlib import pyplot as plt
-            # fig, ax = plt.subplots()
-            # ax.step(emis_wave, emis_flux, where='mid')
-            # ax.step(cont_wave, cont_flux, where='mid')
-            # ax.plot(cont_wave, cont_wave * line.m_cont + line.n_cont, linestyle='--')
-            # plt.show()
-
-            #np.sqrt(np.square(line.peak_wave*line.m_cont_err_intg) + np.square(line.n_cont_err_intg))
-
-            # np.sqrt(np.square(line.peak_wave * line.m_cont_err_intg) + np.square(line.n_cont_err_intg))
-
         # Using line first and last point
         else:
             w2, w3 = emis_wave[0], emis_wave[-1]
             f2, f3 = emis_flux[0], emis_flux[-1]
             line.m_cont = (f3 - f2) / (w3 - w2)
             line.n_cont = f3 - line.m_cont * w3
```

### Comparing `lime-stable-0.9.99.1/src/lime/observations.py` & `lime-stable-0.9.99.5/src/lime/observations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import logging
 import numpy as np
 import pandas as pd
 from pathlib import Path
 from astropy.io import fits
 from collections import UserDict
 
-from .tools import unit_conversion, define_masks, extract_fluxes, normalize_fluxes, ProgressBar, check_units, au
+from .tools import unit_conversion, define_masks, extract_fluxes, normalize_fluxes, ProgressBar, check_units, au, extract_wcs_header
 
 from .recognition import LineFinder, DetectionInference
 from .plots import SpectrumFigures, SampleFigures, CubeFigures
 from .plots_interactive import SpectrumCheck, CubeCheck, SampleCheck
-from .io import _LOG_EXPORT_RECARR, save_log, LiMe_Error, check_file_dataframe, extract_wcs_header, _PARENT_BANDS, \
-    check_file_array_mask, load_log
+from .io import _LOG_EXPORT_RECARR, save_frame, LiMe_Error, check_file_dataframe, _PARENT_BANDS, \
+    check_file_array_mask, load_frame
 
 from .read_fits import OpenFits, SPECTRUM_FITS_PARAMS
 from .transitions import Line, latex_from_label, air_to_vacuum_function
 from .workflow import SpecTreatment, CubeTreatment
 from . import Error, __version__
 
 # Log variable
@@ -256,15 +256,15 @@
 
         if err_flux is not None:
             err_flux = np.ma.masked_array(err_flux, bool_mask)
 
     return wave, wave_rest, flux, err_flux
 
 
-def line_bands(wave_intvl=None, lines_list=None, particle_list=None, z_intvl=None, units_wave='A', decimals=None,
+def line_bands(wave_intvl=None, lines_list=None, particle_list=None, z_intvl=None, units_wave='Angstrom', decimals=None,
                vacuum=False, ref_bands=None):
     """
 
     This function returns `LiMe bands database <https://lime-stable.readthedocs.io/en/latest/inputs/n_inputs3_line_bands.html>`_
     as a pandas dataframe.
 
     If the user provides a wavelength array (``wave_inter``), a lime.Spectrum or lime.Cube the output dataframe will be
@@ -327,17 +327,17 @@
     if vacuum:
 
         # First the table data
         air_columns = ['wavelength', 'w1', 'w2', 'w3', 'w4', 'w5', 'w6']
         mask_df[air_columns] = mask_df[air_columns].apply(air_to_vacuum_function, raw=True)
 
     # Convert to requested units
-    if units_wave != 'A':
-
-        conversion_factor = unit_conversion('A', units_wave, wave_array=1, dispersion_units='dispersion axis')
+    units_wave = au.Unit(units_wave)
+    if units_wave != 'Angstrom':
+        conversion_factor = unit_conversion('Angstrom', units_wave, wave_array=1, dispersion_units='dispersion axis')
         mask_df.loc[:, 'wavelength':'w6'] = mask_df.loc[:, 'wavelength':'w6'] * conversion_factor
 
     # Reconstruct the latex label
     n_bands = mask_df.index.size
     mask_df['latex_label'] = latex_from_label(None, mask_df['particle'], mask_df['wavelength'],
                                               np.array([units_wave] * n_bands), np.zeros(n_bands),
                                               mask_df['transition'], decimals=decimals)
@@ -345,17 +345,19 @@
     # Re-write the line band
     particle_array = mask_df['particle'].to_numpy().astype(str)
 
     wave_array = mask_df['wavelength'].to_numpy()
     wave_array = np.round(wave_array, decimals) if decimals is not None else np.round(wave_array, 0).astype(int)
     wave_array = wave_array.astype(str)
 
+    unit_string = 'A' if units_wave == 'Angstrom' else str(units_wave)
+
     labels_array = np.core.defchararray.add(particle_array, '_')
     labels_array = np.core.defchararray.add(labels_array, wave_array)
-    labels_array = np.core.defchararray.add(labels_array, units_wave)
+    labels_array = np.core.defchararray.add(labels_array, unit_string)
 
     mask_df.rename(index=dict(zip(mask_df.index.values, labels_array)), inplace=True)
 
     # First slice by wavelength and redshift
     if wave_intvl is not None:
 
         # In case the input is a spectrum
@@ -715,16 +717,16 @@
             # Re-apply mask
             self.flux = flux_arr if input_mask is None else np.ma.masked_array(flux_arr, self.flux.mask)
             self.err_flux = err_arr if input_mask is None else np.ma.masked_array(err_arr, self.err_flux.mask)
             self.norm_flux = norm_flux
 
         return
 
-    def save_log(self, file_address, page='LINELOG', param_list='all', header=None, column_dtypes=None,
-                 safe_version=True):
+    def save_frame(self, fname, page='LINELOG', param_list='all', header=None, column_dtypes=None,
+                   safe_version=True):
 
 
         """
 
         This function saves the spectrum measurements at the ``file_address`` provided by the user.
 
         The accepted extensions  are ".txt", ".pdf", ".fits", ".asdf" and ".xlsx".
@@ -735,16 +737,16 @@
         The user can specify the ``parameters`` to be saved in the output file.
 
         For ".fits" files the user can provide a dictionary to add to the ``fits_header``. The user can provide a ``column_dtypes``
         string or dictionary for the output fits file record array. This overwrites LiMe deafult formatting and it must have the
         same columns as the file names.
 
 
-        :param file_address: Output log address.
-        :type file_address: str, Path
+        :param fname: Output log address.
+        :type fname: str, Path
 
         :param param_list: Output parameters list. The default value is "all"
         :type param_list: list
 
         :param page: Name for the HDU/sheet for ".fits"/".xlsx" files.
         :type page: str, optional
 
@@ -759,66 +761,67 @@
         :param safe_version: Save LiMe version as footnote or page header on the output log. The default value is True.
         :type safe_version: bool, optional
 
         """
 
         # Meta parameters from the observations
         meta_params = {'LiMe':       __version__,
-                       'units_wave': self.units_wave.to_string(),
-                       'units_flux': self.units_flux.to_string(),
+                       'u_wave':     self.units_wave.to_string(),
+                       'u_flux':     self.units_flux.to_string(),
                        'redshift':   self.redshift,
                        'id':         self.label}
 
         # Save the file
-        save_log(self.log, file_address, page, param_list, header, column_dtypes=column_dtypes,
-                 safe_version=safe_version, **meta_params)
+        save_frame(fname, self.log, page, param_list, header, column_dtypes=column_dtypes,
+                   safe_version=safe_version, **meta_params)
 
         return
 
-    def load_log(self, file_address, page='LINELOG'):
+    def load_frame(self, fname, page='LINELOG'):
 
         """
 
         This function loads a lines measurements log as a lime.Spectrum.log variable.
 
         The appropriate variables are normalized by the current spectrum flux normalization.
 
-        :param file_address: Input log address.
-        :type file_address: str, Path
+        :param fname: Input log address.
+        :type fname: str, Path
 
         :param page: Name of the HDU/sheet for ".fits"/".xlsx" files.
         :type page: str, optional
 
         """
 
         # Load the log file if it is a log file
-        log_df = check_file_dataframe(file_address, pd.DataFrame, ext=page)
+        log_df = check_file_dataframe(fname, pd.DataFrame, ext=page)
 
         # Security checks:
         if log_df.index.size > 0:
             line_list = log_df.index.values
 
             # Get the first line in the log
             line_0 = Line.from_log(line_list[0], log_df, norm_flux=self.norm_flux)
 
-            # Confirm the lines in the log match the one of the spectrum # TODO fix the units
-            # if line_0.units_wave != self.units_wave:
-            #     _logger.warning(f'Different units in the spectrum dispersion ({self.units_wave}) axis and the lines log'
-            #                     f' in {line_0.units_wave}')
+            # Confirm the lines in the log match the one of the spectrum
+            if line_0.units_wave[0] != self.units_wave:
+                _logger.warning(f'Different units in the spectrum dispersion ({self.units_wave}) axis and the lines log'
+                                f' in {line_0.units_wave[0]}')
 
             # Confirm all the log lines have the same units
-            same_units_check = np.flatnonzero(np.core.defchararray.find(line_list.astype(str), line_0.units_wave) != -1).size == line_list.size
+            au_str = 'A' if line_0.units_wave[0] == 'Angstrom' else str(line_0.units_wave)
+            same_units_check = np.flatnonzero(np.core.defchararray.find(line_list.astype(str), au_str) != -1).size == line_list.size
             if not same_units_check:
                 _logger.warning(f'The log has lines with different units')
 
             # Assign the log
             self.log = log_df
 
         else:
-            _logger.info(f'Log file with 0 entries ({file_address})')
+            _logger.info(f'Log file with 0 entries ({fname})')
 
         return
 
     def update_redshift(self, redshift):
 
         # Check if it is a masked array
         if np.ma.is_masked(self.wave):
@@ -1407,15 +1410,15 @@
     :type folder_obs: string, optional.
 
     :param kwargs: Additional keyword arguments for the creation of the LiMe observation variables.
 
     """
 
     def __init__(self, sample_log, levels=('id', 'file', 'line'), load_function=None, instrument=None, folder_obs=None,
-                 **kwargs):
+                 units_wave='AA', units_flux='FLAM', **kwargs):
 
         # Initiate the user dictionary with a dictionary of observations if provided
         super().__init__()
 
         # Load parent classes
         OpenFits.__init__(self, folder_obs, instrument, load_function, 'Sample')
 
@@ -1424,14 +1427,17 @@
         self.objects = None
         self.group_list = None
         self.levels = list(levels)
 
         # Check the levels on combined labels target log
         check_sample_levels(self.levels)
 
+        # Checks units
+        self.units_wave, self.units_flux = check_units(units_wave, units_flux)
+
         self.log = check_file_dataframe(sample_log, pd.DataFrame, sample_levels=self.levels)
         self._load_function = load_function
         self.load_params = kwargs
 
         # Functionality objects
         self.plot = SampleFigures(self)
         self.check = SampleCheck(self)
@@ -1515,15 +1521,15 @@
 
             # Page and spec index
             file_spec = None if file_list is None else file_list[i]
             page_name = page_list[i] if page_list is not None else 'LINELOG'
 
             # Load the log and check the levels
             if log_list is not None:
-                log_i = load_log(log_list[i], page_name, levels)
+                log_i = load_frame(log_list[i], page_name, levels)
                 df_list.append(review_sample_levels(log_i, id_spec, file_spec))
             else:
                 log_i = pd.DataFrame(columns=["id", "file"], data=(id_spec, file_spec))
                 log_i.set_index(["id", "file"], inplace=True)
 
         sample_log = pd.concat(df_list)
 
@@ -1653,18 +1659,18 @@
     def lines(self):
         return self.log.index.get_level_values('line')
 
     @property
     def size(self):
         return self.log.index.size
 
-    def load_log(self, log_var, ext='LINELOG', sample_levels=['id', 'line']):
+    def load_frame(self, dataframe, ext='LINELOG', sample_levels=['id', 'line']):
 
         # Load the log file if it is a log file
-        log_df = check_file_dataframe(log_var, pd.DataFrame, ext=ext, sample_levels=sample_levels)
+        log_df = check_file_dataframe(dataframe, pd.DataFrame, ext=ext, sample_levels=sample_levels)
 
         # Security checks:
         if log_df.index.size > 0:
 
             if self.units_wave is not None:
                 line_list = log_df.index.values
 
@@ -1679,25 +1685,25 @@
 
                 # Confirm all the log lines have the same units
                 same_units_check = np.flatnonzero(np.core.defchararray.find(line_list.astype(str), line_0.units_wave) != -1).size == line_list.size
                 if not same_units_check:
                     _logger.warning(f'The log has lines with different units')
 
         else:
-            _logger.info(f'Log file with 0 entries ({log_var})')
+            _logger.info(f'Log file with 0 entries ({dataframe})')
 
         # Assign the log
         self.log = log_df
 
         return
 
-    def save_log(self, file_address, ext='LINELOG', param_list='all', fits_header=None):
+    def save_frame(self, fname, ext='LINELOG', param_list='all', fits_header=None):
 
         # Save the file
-        save_log(self.log, file_address, ext, param_list, fits_header)
+        save_frame(fname, self.log, ext, param_list, fits_header)
 
         return
 
     def extract_fluxes(self, flux_type='mixture', sample_level='line', column_names='line_flux', column_positions=1):
 
         return extract_fluxes(self.log, flux_type, sample_level, column_names, column_positions)
```

### Comparing `lime-stable-0.9.99.1/src/lime/plots.py` & `lime-stable-0.9.99.5/src/lime/plots.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import logging
 import numpy as np
+import pandas as pd
 
 from matplotlib import pyplot as plt, gridspec, patches, rc_context, cm, colors
 
-import pandas as pd
-
 from .model import c_KMpS, profiles_computation, linear_continuum_computation
-from .tools import blended_label_from_log, latex_science_float, PARAMETER_LATEX_DICT
-from .tools import define_masks, format_line_mask_option, au
-from .io import check_file_dataframe, save_log, _PARENT_BANDS, load_spatial_mask, LiMe_Error, _LOG_COLUMNS_LATEX
+from .tools import latex_science_float, PARAMETER_LATEX_DICT
+from .tools import define_masks, format_line_mask_option
+from .io import check_file_dataframe, _PARENT_BANDS, load_spatial_mask, LiMe_Error, _LOG_COLUMNS_LATEX
 from .transitions import check_line_in_log, Line, label_decomposition
 from . import _setup_cfg
 
 _logger = logging.getLogger('LiMe')
 
 
 try:
@@ -21,53 +20,197 @@
 except ImportError:
     mplcursors_check = False
 
 if mplcursors_check:
     from mplcursors._mplcursors import _default_annotation_kwargs as popupProps
     popupProps['bbox']['alpha'] = 0.9
 
-PLOT_SIZE_FONT = {'figure.figsize': (11, 6),
-                  'axes.titlesize': 14,
-                  'axes.labelsize': 14,
-                  'legend.fontsize': 12,
-                  'xtick.labelsize': 12,
-                  'ytick.labelsize': 12}
-
-COLOR_DICT = {'bg': 'white', 'fg': 'black',
-             'cont_band': '#8c564b', 'line_band': '#b5bd61',
-             'color_cycle': ['#279e68', '#d62728', '#aa40fc', '#8c564b',
-                             '#e377c2', '#7f7f7f', '#b5bd61', '#17becf', '#1f77b4', '#ff7f0e'],
-             'matched_line': '#b5bd61',
-             'peak': '#aa40fc',
-             'trough': '#7f7f7f',
-             'profile': '#1f77b4',
-             'cont': '#ff7f0e',
-             'error': 'red',
-             'mask_map': 'viridis',
-              'comps_map': 'Dark2',
-              'mask_marker': 'red'}
-
-PLOT_COLORS = {'figure.facecolor': COLOR_DICT['bg'], 'axes.facecolor': COLOR_DICT['bg'],
-               'axes.edgecolor': COLOR_DICT['fg'], 'axes.labelcolor': COLOR_DICT['fg'],
-               'xtick.color': COLOR_DICT['fg'], 'ytick.color': COLOR_DICT['fg'],
-               'text.color': COLOR_DICT['fg'], 'legend.edgecolor': 'inherit', 'legend.facecolor': 'inherit'}
-
-colorDictDark = {'bg': np.array((43, 43, 43))/255.0, 'fg': np.array((179, 199, 216))/255.0,
-                 'red': np.array((43, 43, 43))/255.0, 'yellow': np.array((191, 144, 0))/255.0}
-
-PLOT_COLORS_DARK = {'figure.facecolor': colorDictDark['bg'], 'axes.facecolor': colorDictDark['bg'],
-                    'axes.edgecolor': colorDictDark['fg'], 'axes.labelcolor': colorDictDark['fg'],
-                    'xtick.color': colorDictDark['fg'],  'ytick.color': colorDictDark['fg'],
-                    'text.color': colorDictDark['fg'], 'legend.edgecolor': 'inherit', 'legend.facecolor': 'inherit'}
 
-PLOT_COLORS = {}
+class Themer:
+
+    def __init__(self, conf, style='default', library='matplotlib'):
+
+        # Attributes
+        self.conf = None
+        self.style = None
+        self.base_conf = None
+        self.colors = None
+        self.library = None
+
+        # Assign default
+        self.conf = conf.copy()
+        self.library = library
+        self.set_style(style)
+
+        return
+
+    def fig_defaults(self, user_fig, fig_type=None):
+
+        # Get plot configuration
+        if fig_type is None:
+            fig_conf = self.base_conf.copy()
+        else:
+            fig_conf = {** self.base_conf, **self.conf[self.library][fig_type]}
+
+        # Get user configuration
+        fig_conf = fig_conf if user_fig is None else {**fig_conf, **user_fig}
+
+        return fig_conf
+
+    def ax_defaults(self, user_ax, units_wave, units_flux, norm_flux, fig_type='default', **kwargs):
+
+        # Default wavelength and flux
+        if fig_type == 'default':
+
+            # Wavelength axis units
+            x_label = units_wave.to_string('latex')
+            x_label = f'Wavelength ({x_label})'
+
+            # Flux axis units
+            norm_flux = units_flux.scale if norm_flux is None else norm_flux
+            norm_label = r'\right)$' if norm_flux == 1 else r' \,\cdot\,{}\right)$'.format(latex_science_float(1/norm_flux))
+
+            y_label = f"Flux {units_flux.to_string('latex')}"
+            y_label = y_label.replace('$\mathrm{', '$\left(')
+            y_label = y_label.replace('}$', norm_label)
+
+            ax_cfg = {'xlabel': x_label, 'ylabel': y_label}
+
+            # Update with the user configuration
+            ax_cfg = ax_cfg if user_ax is None else {**ax_cfg, **user_ax}
+
+        # Spatial cubes
+        elif fig_type == 'cube':
+
+            ax_cfg = {} if user_ax is None else user_ax.copy()
+
+            # Define the title
+            if ax_cfg.get('title') is None:
+
+                title = r'{} band'.format(kwargs['line_bg'].latex_label[0])
+
+                line_fg = kwargs.get('line_fg')
+                if line_fg is not None:
+                    title = f'{title} with {line_fg.latex_label[0]} contours'
+
+                if len(kwargs['masks_dict']) > 0:
+                    title += f'\n and spatial masks at foreground'
+
+                ax_cfg['title'] = title
+
+            # Define x axis
+            if ax_cfg.get('xlabel') is None:
+                ax_cfg['xlabel'] = 'x' if kwargs['wcs'] is None else 'RA'
 
-STANDARD_PLOT = {**PLOT_SIZE_FONT, **PLOT_COLORS}
+            # Define y axis
+            if ax_cfg.get('ylabel') is None:
+                ax_cfg['ylabel'] = 'y' if kwargs['wcs'] is None else 'DEC'
 
-STANDARD_AXES = {'xlabel': r'Wavelength $(\AA)$', 'ylabel': r'Flux $(erg\,cm^{-2} s^{-1} \AA^{-1})$'}
+            # Update with the user configuration
+            ax_cfg = ax_cfg if user_ax is None else {**ax_cfg, **user_ax}
+
+        elif fig_type == 'velocity':
+
+            x_label = 'Velocity (Km/s)'
+
+            # Flux axis units
+            norm_flux = units_flux.scale if norm_flux is None else norm_flux
+            norm_label = r'\right)$' if norm_flux == 1 else r' \,\cdot\,{}\right)$'.format(latex_science_float(1/norm_flux))
+
+            y_label = f"Flux {units_flux.to_string('latex')}"
+            y_label = y_label.replace('$\mathrm{', '$\left(')
+            y_label = y_label.replace('}$', norm_label)
+
+            ax_cfg = {'xlabel': x_label, 'ylabel': y_label}
+
+            # Update with the user configuration
+            ax_cfg = ax_cfg if user_ax is None else {**ax_cfg, **user_ax}
+
+        # No labels
+        else:
+            ax_cfg = {}
+
+            # Update with the user configuration
+            ax_cfg = ax_cfg if user_ax is None else {**ax_cfg, **user_ax}
+
+        return ax_cfg
+
+    def set_style(self, style, style_conf=None, colors_conf=None):
+
+        # Set the new style
+        self.style = np.atleast_1d(style)
+
+        # Add the new configuration
+        if style_conf is not None:
+            existing_set = {} if self.style not in self.conf[self.library] else self.conf[self.library][self.style]
+            self.conf[self.library][self.style] = {**existing_set, **style_conf}
+
+        # Generate the default
+        self.base_conf = self.conf[self.library]['default'].copy()
+        for style in self.style:
+            self.base_conf = {**self.base_conf, **self.conf[self.library][style]}
+
+        # Add the new colors
+        if colors_conf is not None:
+            existing_set = {} if self.style not in self.conf['lime_colors'] else self.conf['lime_colors'][self.style]
+            self.conf['lime_colors'][self.style] = {**existing_set, **colors_conf}
+
+        # Set the colors
+        for i_style in self.style:
+            if i_style in self.conf['lime_colors']:
+                self.colors = self.conf['lime_colors'][style].copy()
+
+        if self.colors is None:
+            _logger.warning(f'The input style {self.style} does not have a LiMe color database')
+
+        return
+
+
+# LiMe figure labels and color formatter
+theme = Themer(_setup_cfg)
+
+# PLOT_SIZE_FONT = {'figure.figsize': (11, 6),
+#                   'axes.titlesize': 14,
+#                   'axes.labelsize': 14,
+#                   'legend.fontsize': 12,
+#                   'xtick.labelsize': 12,
+#                   'ytick.labelsize': 12}
+#
+# COLOR_DICT = {'bg': 'white', 'fg': 'black',
+#              'cont_band': '#8c564b', 'line_band': '#b5bd61',
+#              'color_cycle': ['#279e68', '#d62728', '#aa40fc', '#8c564b',
+#                              '#e377c2', '#7f7f7f', '#b5bd61', '#17becf', '#1f77b4', '#ff7f0e'],
+#              'matched_line': '#b5bd61',
+#              'peak': '#aa40fc',
+#              'trough': '#7f7f7f',
+#              'profile': '#1f77b4',
+#              'cont': '#ff7f0e',
+#              'error': 'red',
+#              'mask_map': 'viridis',
+#              'comps_map': 'Dark2',
+#              'mask_marker': 'red'}
+#
+# PLOT_COLORS = {'figure.facecolor': COLOR_DICT['bg'], 'axes.facecolor': COLOR_DICT['bg'],
+#                'axes.edgecolor': COLOR_DICT['fg'], 'axes.labelcolor': COLOR_DICT['fg'],
+#                'xtick.color': COLOR_DICT['fg'], 'ytick.color': COLOR_DICT['fg'],
+#                'text.color': COLOR_DICT['fg'], 'legend.edgecolor': 'inherit', 'legend.facecolor': 'inherit'}
+#
+# colorDictDark = {'bg': np.array((43, 43, 43))/255.0, 'fg': np.array((179, 199, 216))/255.0,
+#                  'red': np.array((43, 43, 43))/255.0, 'yellow': np.array((191, 144, 0))/255.0}
+#
+# PLOT_COLORS_DARK = {'figure.facecolor': colorDictDark['bg'], 'axes.facecolor': colorDictDark['bg'],
+#                     'axes.edgecolor': colorDictDark['fg'], 'axes.labelcolor': colorDictDark['fg'],
+#                     'xtick.color': colorDictDark['fg'],  'ytick.color': colorDictDark['fg'],
+#                     'text.color': colorDictDark['fg'], 'legend.edgecolor': 'inherit', 'legend.facecolor': 'inherit'}
+#
+# PLOT_COLORS = {}
+#
+# STANDARD_PLOT = {**PLOT_SIZE_FONT, **PLOT_COLORS}
+#
+# STANDARD_AXES = {'xlabel': r'Wavelength $(\AA)$', 'ylabel': r'Flux $(erg\,cm^{-2} s^{-1} \AA^{-1})$'}
 
 
 def mplcursors_legend(line, log, latex_label, norm_flux, units_wave, units_flux):
 
     legend_text = latex_label + '\n'
 
     units_line_flux = units_wave * units_flux
@@ -302,41 +445,14 @@
 
     else:
         line, image, levels, color_scale = None, None, None, None
 
     return line, image, levels, color_scale
 
 
-def image_map_labels(input_labels, wcs, line_bg, line_fg, masks_dict):
-
-    if input_labels is None:
-        output_labels = {}
-    else:
-        output_labels = input_labels.copy()
-
-    # Define the title
-    if output_labels.get('title') is None:
-        title = r'{} band'.format(line_bg.latex_label[0])
-        if line_fg is not None:
-            title = f'{title} with {line_fg.latex_label[0]} contours'
-        if len(masks_dict) > 0:
-            title += f'\n and spatial masks at foreground'
-        output_labels['title'] = title
-
-    # Define x axis
-    if output_labels.get('xlabel') is None:
-        output_labels['xlabel'] = 'x' if wcs is None else 'RA'
-
-    # Define y axis
-    if output_labels.get('ylabel') is None:
-        output_labels['ylabel'] = 'y' if wcs is None else 'DEC'
-
-    return output_labels
-
-
 def image_plot(ax, image_bg, image_fg, fg_levels, fg_mesh, bg_scale, fg_scale, bg_color, fg_color, cursor_cords=None):
 
     # Background image plot
     im = ax.imshow(image_bg, cmap=bg_color, norm=bg_scale)
 
     # Foreground contours
     if image_fg is not None:
@@ -395,15 +511,15 @@
 
             ax.imshow(inv_mask_array, cmap=cm_i, vmin=0, vmax=1, alpha=mask_alpha)
 
     return legend_list
 
 
 def spec_plot(ax, wave, flux, redshift, norm_flux, label='', rest_frame=False, log=None, include_fits=True,
-              units_wave='A', units_flux='Flam', log_scale=False, color_dict=COLOR_DICT):
+              units_wave='A', units_flux='Flam', log_scale=False, color_dict=theme.colors):
 
 
     # Reference frame for the plot
     wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch_2(wave, flux, redshift, rest_frame)
 
     # Plot the spectrum
     ax.step(wave_plot / z_corr, flux_plot * z_corr, label=label, where='mid', color=color_dict['fg'])
@@ -426,15 +542,15 @@
 
     # Plot the masked pixels
     _masks_plot(ax, line_list, wave_plot, flux_plot, z_corr, log, idcs_mask)
 
     return
 
 
-def _profile_plot(axis, x, y, label, idx_line=0, n_comps=1, observations_list='yes', color_dict=COLOR_DICT):
+def _profile_plot(axis, x, y, label, idx_line=0, n_comps=1, observations_list='yes', color_dict=theme.colors):
 
     # Color and thickness
     if observations_list == 'no':
 
         # If only one component or combined
         if n_comps == 1:
             width_i, style, color = 1.5, '-', color_dict['profile']
@@ -457,26 +573,26 @@
 
     # Plot the profile
     line_g = axis.plot(x, y, label=label, linewidth=width_i, linestyle=style, color=color)
 
     return line_g
 
 
-def color_selector(label, observations, idx_line, n_comps, color_dict):
+def color_selector(label, observations, idx_line, n_comps):
 
     # Color and thickness
     if observations == 'no':
 
         # If only one component or combined
         if n_comps == 1:
-            width_i, style, color = 1.5, '-', color_dict['profile']
+            width_i, style, color = 1.5, '-', theme.colors['profile']
 
         # Component
         else:
-            cmap = cm.get_cmap(color_dict['comps_map'])
+            cmap = cm.get_cmap(theme.colors['comps_map'])
 
             """  /home/usuario/PycharmProjects/lime/src/lime/plots.py:725: MatplotlibDeprecationWarning: 
             The get_cmap function was deprecated in Matplotlib 3.7 and will be removed two minor releases later. 
             Use ``matplotlib.colormaps[name]`` or ``matplotlib.colormaps.get_cmap(obj)`` instead.
                 cmap = cm.get_cmap(color_dict['comps_map'])
             """
 
@@ -488,18 +604,15 @@
 
     # Make dictionary with the params
     cont_format = dict(label=label, color=color, linestyle=style, linewidth=width_i)
 
     return cont_format
 
 
-def _profile_plt(axis, line, z_cor, log, redshift, norm_flux, color_dict=None):
-
-    # Get default colors
-    color_dict = COLOR_DICT if color_dict is None else color_dict
+def _profile_plt(axis, line, z_cor, log, redshift, norm_flux):
 
     # Check if blended line or Single/merged
     if line.blended_check:
         if line.list_comps:
             idx_line = line.list_comps.index(line.label)
             n_comps = len(line.list_comps)
     else:
@@ -512,33 +625,32 @@
 
     wave_i = wave_array[:, 0]
     cont_i = cont_array[:, 0]
     flux_i = flux_array[:, idx_line]
 
     # Plot a continuum (only one per line)
     if idx_line == 0:
-        cont_format = dict(label=None, color=COLOR_DICT['cont'], linestyle='--', linewidth=0.5)
+        cont_format = dict(label=None, color=theme.colors['cont'], linestyle='--', linewidth=0.5)
         axis.plot(wave_array/z_cor, cont_array[:, 0] * z_cor / norm_flux, **cont_format)
 
     # Plot combined gaussian profile if blended
     if (idx_line == 0) and (n_comps > 1):
         comb_array = (flux_array.sum(axis=1) + cont_i) * z_cor / norm_flux
-        line_format = color_selector(None, line.observations, 0, 1, color_dict)
+        line_format = color_selector(None, line.observations, 0, 1)
         axis.plot(wave_i / z_cor, comb_array, **line_format)
 
     # Gaussian component plot
     single_array = (flux_i + cont_i) * z_cor / norm_flux
-    line_format = color_selector(line.label, line.observations, idx_line, n_comps, color_dict)
+    line_format = color_selector(line.label, line.observations, idx_line, n_comps)
     line_single = axis.plot(wave_i/z_cor, single_array, **line_format)
 
     return line_single
 
 
-def _gaussian_line_profiler(axis, line_list, wave_array, gaussian_array, cont_array, z_corr, log, norm_flux,
-                            color_dict=COLOR_DICT):
+def _gaussian_line_profiler(axis, line_list, wave_array, gaussian_array, cont_array, z_corr, log, norm_flux):
 
     # Data for the plot
     observations = log.loc[log.index.isin(line_list)].observations.values
 
     # Plot them
     line_g_list = [None] * len(line_list)
     for i, line in enumerate(line_list):
@@ -566,27 +678,27 @@
         # Get the corresponding axis
         wave_i = wave_array[:, i]
         cont_i = cont_array[:, i]
         gauss_i = gaussian_array[:, i]
 
         # Continuum (only one per line)
         if idx_line == 0:
-            axis.plot(wave_i / z_corr, cont_i * z_corr / norm_flux, color=COLOR_DICT['cont'], label=None,
+            axis.plot(wave_i / z_corr, cont_i * z_corr / norm_flux, color=theme.colors['cont'], label=None,
                       linestyle='--', linewidth=0.5)
 
         # Plot combined gaussian profile if blended
         if idcs_comp is not None:
             gauss_comb = gaussian_array[:, idcs_comp].sum(axis=1) + cont_i
             _profile_plot(axis, wave_i/z_corr, gauss_comb*z_corr/norm_flux, None,
-                               idx_line=idx_line, n_comps=1, observations_list=observations[i], color_dict=color_dict)
+                               idx_line=idx_line, n_comps=1, observations_list=observations[i], color_dict=theme.colors)
 
         # Gaussian component plot
         line_g_list[i] = _profile_plot(axis, wave_i/z_corr, (gauss_i+cont_i)*z_corr/norm_flux, latex_label,
                                        idx_line=idx_line, n_comps=n_comps, observations_list=observations[i],
-                                       color_dict=color_dict)
+                                       color_dict=theme.colors)
 
     return line_g_list
 
 
 def _masks_plot(axis, line_list, x, y, z_corr, log, spectrum_mask, color_dict={}):
 
     # Spectrum mask
@@ -610,32 +722,14 @@
                             if np.sum(idcsMask) >= 1:
                                 axis.scatter(x[idcsMask]/z_corr, y[idcsMask]*z_corr, marker="x",
                                              color=color_dict['mask_marker'])
 
     return
 
 
-def parse_figure_format(input_conf, local_conf=None, default_conf=STANDARD_PLOT, theme=None):
-
-    # Check whether there is an input configuration
-    if input_conf is None:
-        output_conf = {}
-    else:
-        output_conf = input_conf.copy()
-
-    # Default configuration
-    if local_conf is not None:
-        output_conf = {**local_conf, **output_conf}
-
-    # Final configuration
-    output_conf = {**default_conf, **output_conf}
-
-    return output_conf
-
-
 def label_generator(idx_sample, log, legend_handle):
 
     if legend_handle == 'levels':
         spec_label = ", ".join(map(str, idx_sample))
 
     elif legend_handle is None:
         spec_label = None
@@ -651,52 +745,18 @@
 
         else:
             raise LiMe_Error(f'The input handle "{legend_handle}" is not found on the sample log columns')
 
     return spec_label
 
 
-def axis_labeling(norm_flux, units_wave, units_flux, plot_type=None):
-
-    # TODO maybe make this a dictionary to get the default ax_cfg
-
-    # Wavelength axis units
-    x_label = units_wave.to_string('latex')
-    x_label = f'Wavelength ({x_label})'
-
-    # Flux axis units
-    norm_flux = units_flux.scale if norm_flux is None else norm_flux
-    norm_label = r'\right)$' if norm_flux == 1 else r' \,\cdot\,{}\right)$'.format(latex_science_float(1 / norm_flux))
-    # norm_label = '' if norm_flux == 1 else r' $\,/\,{}$'.format(latex_science_float(norm_flux))
-
-    y_label = f"Flux {units_flux.to_string('latex')}"
-    y_label = y_label.replace('$\mathrm{', '$\left(')
-    y_label = y_label.replace('}$', norm_label)
-
-    return x_label, y_label
-
-
-class Themer:
-
-    def __init__(self, conf=None, theme_list=None):
-
-        # Use the default configuration if non is provided
-        conf = _setup_cfg if conf is None else conf
-
-        self.high_dpi_check = False
-        self.plt_themes = conf['matplotlib_cfg']
-
-        return
-
-
 class Plotter:
 
     def __init__(self):
 
-        self._color_dict = COLOR_DICT
         self._legends_dict = {}
 
         return
 
     def _plot_container(self, fig, ax, ax_cfg={}, gfit_type=False):
 
         #Plot for residual axis
@@ -714,63 +774,42 @@
             if (fig is None) and (ax is None):
                 fig, ax = plt.subplots()
 
             ax.set(**ax_cfg)
 
         return fig, ax
 
-    def _figure_format(self, fig_cfg, ax_cfg, norm_flux, units_wave=None, units_flux=None):
-
-        # Adjust default theme
-        PLOT_CONF, AXES_CONF = STANDARD_PLOT.copy(), STANDARD_AXES.copy()
-
-        # Assign the default axis labels
-        AXES_CONF['xlabel'], AXES_CONF['ylabel'] = axis_labeling(norm_flux, units_wave, units_flux)
-
-        # User configuration overrites user
-        PLT_CONF = {**PLOT_CONF, **fig_cfg}
-        AXES_CONF = {**AXES_CONF, **ax_cfg}
-
-        return PLT_CONF, AXES_CONF
-
     def _line_matching_plot(self, axis, match_log, x, y, z_corr, redshift, units_wave):
 
-        # Plot peaks and troughs if provided
-        color_peaks = (self._color_dict['peak'], self._color_dict['trough'])
-        labels = ('Peaks', 'Troughs')
-        line_types = ('emission', 'absorption')
-        labels = ('Peaks', 'Troughs')
-
         # Plot the detected line peaks
         if 'signal_peak' in match_log.columns:
             idcs_linePeaks = match_log['signal_peak'].values.astype(int)
             axis.scatter(x[idcs_linePeaks]/z_corr, y[idcs_linePeaks]*z_corr, label='Peaks',
-                         facecolors='none', edgecolors=self._color_dict['peak'])
+                         facecolors='none', edgecolors=theme.colors['peak'])
 
         # Get the line labels and the bands labels for the lines
-        # ion_array, wave_array, latex = label_decomposition(match_log.index.values, units_wave=units_wave)
         wave_array, latex = label_decomposition(match_log.index.values, params_list=('wavelength', 'latex_label'))
 
         w3 = match_log.w3.values * (1 + redshift)
         w4 = match_log.w4.values * (1 + redshift)
         idcsLineBand = np.searchsorted(x, np.array([w3, w4]))
 
         # Loop through the detections and plot the names
         for i in np.arange(latex.size):
             label = 'Matched line' if i == 0 else '_'
             max_region = np.max(y[idcsLineBand[0, i]:idcsLineBand[1, i]])
-            axis.axvspan(w3[i]/z_corr, w4[i]/z_corr, label=label, alpha=0.30, color=self._color_dict['matched_line'])
+            axis.axvspan(w3[i]/z_corr, w4[i]/z_corr, label=label, alpha=0.30, color=theme.colors['match_line'])
             axis.text(wave_array[i] * (1 + redshift) / z_corr, max_region * 0.9 * z_corr, latex[i], rotation=270)
 
         return
 
     def _bands_plot(self, axis, x, y, z_corr, idcs_mask, label):
 
-        cont_dict = {'facecolor': self._color_dict['cont_band'], 'step': 'mid', 'alpha': 0.25}
-        line_dict = {'facecolor': self._color_dict['line_band'], 'step': 'mid', 'alpha': 0.25}
+        cont_dict = {'facecolor': theme.colors['cont_band'], 'step': 'mid', 'alpha': 0.25}
+        line_dict = {'facecolor': theme.colors['line_band'], 'step': 'mid', 'alpha': 0.25}
 
         # Plot
         if len(y[idcs_mask[0]:idcs_mask[5]]) > 1:
             low_lim = np.min(y[idcs_mask[0]:idcs_mask[5]])
             low_lim = 0 if np.isnan(low_lim) else low_lim
             axis.fill_between(x[idcs_mask[0]:idcs_mask[1]]/z_corr, low_lim*z_corr, y[idcs_mask[0]:idcs_mask[1]]*z_corr, **cont_dict)
             axis.fill_between(x[idcs_mask[2]:idcs_mask[3]]/z_corr, low_lim*z_corr, y[idcs_mask[2]:idcs_mask[3]]*z_corr, **line_dict)
@@ -780,108 +819,102 @@
 
         return
 
     def _peak_plot(self, axis, log, list_comps, z_corr, norm_flux):
 
         peak_wave = log.loc[list_comps[0]].peak_wave/z_corr,
         peak_flux = log.loc[list_comps[0]].peak_flux*z_corr/norm_flux
-        axis.scatter(peak_wave, peak_flux, facecolors=self._color_dict['peak'])
+        axis.scatter(peak_wave, peak_flux, facecolors=theme.colors['peak'])
 
         return
 
     def _cont_plot(self, axis, x, y, z_corr, norm_flux):
 
         # Plot the continuum,  Usine wavelength array and continuum form the first component
         # cont_wave = wave_array[:, 0]
         # cont_linear = cont_array[:, 0]
-        axis.plot(x/z_corr, y*z_corr/norm_flux, color=self._color_dict['cont'], linestyle='--', linewidth=0.5)
+        axis.plot(x/z_corr, y*z_corr/norm_flux, color=theme.colors['cont'], linestyle='--', linewidth=0.5)
 
         return
 
     def _plot_continuum_fit(self, continuum_fit, idcs_cont, low_lim, high_lim, threshold_factor, plot_title=''):
 
-        PLOT_CONF = STANDARD_PLOT.copy()
-        AXES_CONF = STANDARD_AXES.copy()
-
         norm_flux = self._spec.norm_flux
         wave = self._spec.wave
         flux = self._spec.flux
         units_wave = self._spec.units_wave
         units_flux = self._spec.units_flux
         redshift = self._spec.redshift
 
         # Assign the default axis labels
-        xlabel, y_label = axis_labeling(norm_flux, units_wave, units_flux)
-        AXES_CONF['title'], AXES_CONF['xlabel'], AXES_CONF['ylabel'] = plot_title, xlabel, y_label
+        PLOT_CONF = theme.fig_defaults(None)
+        AXES_CONF = theme.ax_defaults(None, units_wave, units_flux, norm_flux)
 
         wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch_2(wave, flux, redshift, False)
 
         with rc_context(PLOT_CONF):
 
             fig, ax = plt.subplots()
 
             # Object spectrum
-            ax.step(wave_plot, flux_plot, label='Object spectrum', color=self._color_dict['fg'], where='mid')
+            ax.step(wave_plot, flux_plot, label='Object spectrum', color=theme.colors['fg'], where='mid')
 
             # Band limits
             label = r'$16^{{th}}/{} - 84^{{th}}\cdot{}$ flux percentiles band'.format(threshold_factor, threshold_factor)
-            ax.axhspan(low_lim, high_lim, alpha=0.2, label=label, color=self._color_dict['line_band'])
+            ax.axhspan(low_lim, high_lim, alpha=0.2, label=label, color=theme.colors['line_band'])
             ax.axhline(np.median(flux_plot[idcs_cont]), label='Median flux', linestyle=':', color='black')
 
             # Masked and rectected pixels
-            ax.scatter(wave_plot[~idcs_cont], flux_plot[~idcs_cont], label='Rejected pixels', color=self._color_dict['peak'], facecolor='none')
-            ax.scatter(wave_plot[idcs_mask], flux_plot[idcs_mask], marker='x', label='Masked pixels', color=self._color_dict['mask_marker'])
+            ax.scatter(wave_plot[~idcs_cont], flux_plot[~idcs_cont], label='Rejected pixels', color=theme.colors['peak'], facecolor='none')
+            ax.scatter(wave_plot[idcs_mask], flux_plot[idcs_mask], marker='x', label='Masked pixels', color=theme.colors['mask_marker'])
 
             # Output continuum
             ax.plot(wave_plot, continuum_fit, label='Continuum')
 
             ax.update(AXES_CONF)
             ax.legend()
             plt.tight_layout()
             plt.show()
 
         return
 
     def _plot_peak_detection(self, peak_idcs, detect_limit, continuum=None, plot_title='', ml_mask=None):
 
-        PLOT_CONF = STANDARD_PLOT.copy()
-        AXES_CONF = STANDARD_AXES.copy()
 
         norm_flux = self._spec.norm_flux
         wave = self._spec.wave
         flux = self._spec.flux
         units_wave = self._spec.units_wave
         units_flux = self._spec.units_flux
         redshift = self._spec.redshift
 
-        # Assign the default axis labels
-        xlabel, y_label = axis_labeling(norm_flux, units_wave, units_flux)
-        AXES_CONF['title'], AXES_CONF['xlabel'], AXES_CONF['ylabel'] = plot_title, xlabel, y_label
+        PLOT_CONF = theme.fig_defaults(None)
+        AXES_CONF = theme.ax_defaults(None, units_wave, units_flux, norm_flux)
 
         wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch_2(wave, flux, redshift, 'observed')
 
         continuum = continuum if continuum is not None else np.zeros(flux.size)
 
         with rc_context(PLOT_CONF):
 
             fig, ax = plt.subplots()
-            ax.step(wave_plot, flux_plot, color=self._color_dict['fg'], label='Object spectrum', where='mid')
+            ax.step(wave_plot, flux_plot, color=theme.colors['fg'], label='Object spectrum', where='mid')
 
             if ml_mask is not None:
                 if np.any(ml_mask):
                     ax.scatter(wave_plot[ml_mask], flux_plot[ml_mask], label='ML detection', color='palegreen')
 
-            ax.scatter(wave_plot[peak_idcs], flux_plot[peak_idcs], marker='o', label='Peaks', color=self._color_dict['peak'], facecolors='none')
-            ax.fill_between(wave_plot, continuum, detect_limit, facecolor=self._color_dict['line_band'], label='Noise_region', alpha=0.5)
+            ax.scatter(wave_plot[peak_idcs], flux_plot[peak_idcs], marker='o', label='Peaks', color=theme.colors['peak'], facecolors='none')
+            ax.fill_between(wave_plot, continuum, detect_limit, facecolor=theme.colors['line_band'], label='Noise_region', alpha=0.5)
 
             if continuum is not None:
                 ax.plot(wave_plot, continuum, label='Continuum')
 
             ax.scatter(wave_plot[idcs_mask], flux_plot[idcs_mask], label='Masked pixels', marker='x',
-                       color=self._color_dict['mask_marker'])
+                       color=theme.colors['mask_marker'])
 
             ax.legend()
             ax.update(AXES_CONF)
             plt.tight_layout()
             plt.show()
 
         return
@@ -961,21 +994,20 @@
         :type maximize:  bool, optional
 
         """
 
         # Display check for the user figures
         display_check = True if in_fig is None else False
 
-
-
         # Set figure format with the user inputs overwriting the default conf
         legend_check = True if label is not None else False
-        fig_cfg.setdefault('figure.figsize', (8, 5))
-        PLT_CONF, AXES_CONF = self._figure_format(fig_cfg, ax_cfg, norm_flux=self._spec.norm_flux,
-                                                  units_wave=self._spec.units_wave, units_flux=self._spec.units_flux)
+
+        # Adjust the default theme
+        PLT_CONF = theme.fig_defaults(fig_cfg)
+        AXES_CONF = theme.ax_defaults(ax_cfg, self._spec.units_wave, self._spec.units_flux, self._spec.norm_flux)
 
         # Create and fill the figure
         with rc_context(PLT_CONF):
 
             # Generate the figure object and figures
             if in_fig is None:
                 in_fig, in_ax = self._plot_container(in_fig, None, AXES_CONF)
@@ -984,15 +1016,15 @@
                 in_ax.set(**AXES_CONF)
 
             # Reference _frame for the plot
             wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch_2(self._spec.wave, self._spec.flux,
                                                                           self._spec.redshift, rest_frame)
 
             # Plot the spectrum
-            in_ax.step(wave_plot / z_corr, flux_plot * z_corr, label=label, where='mid', color=self._color_dict['fg'])
+            in_ax.step(wave_plot / z_corr, flux_plot * z_corr, label=label, where='mid', color=theme.colors['fg'])
 
             # Plot peaks and troughs if provided
             if line_bands is not None:
                 line_bands = check_file_dataframe(line_bands, pd.DataFrame)
                 self._line_matching_plot(in_ax, line_bands, wave_plot, flux_plot, z_corr, self._spec.redshift,
                                          self._spec.units_wave)
 
@@ -1016,15 +1048,15 @@
                                                        self._spec.norm_flux)
 
                     # Add the interactive pop-ups
                     _mplcursor_parser(profile_list, line_list, self._spec.log, self._spec.norm_flux, self._spec.units_wave,
                                       self._spec.units_flux)
 
                 # Plot the masked pixels
-                _masks_plot(in_ax, line_list, wave_plot, flux_plot, z_corr, self._spec.log, idcs_mask, self._color_dict)
+                _masks_plot(in_ax, line_list, wave_plot, flux_plot, z_corr, self._spec.log, idcs_mask, theme.colors)
 
             # Plot the normalize continuum
             if include_cont and self._spec.cont is not None:
                 in_ax.plot(wave_plot/z_corr, self._spec.cont, label='Fitted continuum', linestyle='--')
 
             # Switch y_axis to logarithmic scale if requested
             if log_scale:
@@ -1036,15 +1068,15 @@
 
             # By default, plot on screen unless an output address is provided
             in_fig = save_close_fig_swicth(output_address, 'tight', in_fig, maximize, display_check)
 
         return in_fig
 
     def grid(self, output_address=None, rest_frame=True, y_scale='auto', n_cols=6, n_rows=None, col_row_scale=(2, 1.5),
-             include_fits=True, in_fig=None, fig_cfg={}, ax_cfg={}, maximize=False):
+             include_fits=True, in_fig=None, fig_cfg=None, ax_cfg=None, maximize=False):
 
         """
 
         This function plots the lines from the object spectrum log as a grid.
 
         If the user has installed the library `mplcursors <https://mplcursors.readthedocs.io/en/stable/>`_, a left-click
         on a fitted profile will pop-up properties of the fitting, right-click to delete the annotation.
@@ -1112,20 +1144,20 @@
                 if n_rows is None:
                     n_rows = int(np.ceil(n_lines / n_cols))
             else:
                 n_cols, n_rows = n_lines, 1
             n_grid = n_cols * n_rows
 
             # Set the plot format where the user's overwrites the default
-            default_fig_cfg = {'figure.figsize': (n_cols * col_row_scale[0], n_rows * col_row_scale[1]),
-                               'axes.titlesize': 12}
-            default_fig_cfg.update(fig_cfg)
-            PLT_CONF, AXES_CONF = self._figure_format(default_fig_cfg, ax_cfg, norm_flux=self._spec.norm_flux,
-                                                      units_wave=self._spec.units_wave, units_flux=self._spec.units_flux)
-            AXES_CONF.pop('xlabel')
+            size_conf = {'figure.figsize': (n_cols * col_row_scale[0], n_rows * col_row_scale[1])}
+            size_conf = size_conf if fig_cfg is None else {**size_conf, **fig_cfg}
+
+            PLT_CONF = theme.fig_defaults(size_conf, fig_type='grid')
+            AXES_CONF = theme.ax_defaults(ax_cfg, self._spec.units_wave, self._spec.units_flux, self._spec.norm_flux,
+                                          fig_type=None)
 
             # Launch the interative figure
             with rc_context(PLT_CONF):
 
                 # Generate the figure if not provided
                 if in_fig is None:
                     in_fig = plt.figure()
@@ -1149,36 +1181,35 @@
                         # Establish the limits for the line spectrum plot
                         idcs_m = np.searchsorted(wave_plot, line_i.mask * (1 + self._spec.redshift))
                         idx_blue = idcs_m[0] - 5 if idcs_m[0] > 5 else idcs_m[0]
                         idx_red = idcs_m[-1] + 5 if idcs_m[-1] < idcs_m[-1] + 5 else idcs_m[-1]
 
                         # Plot the spectrum
                         in_ax.step(wave_plot[idx_blue:idx_red] / z_corr, flux_plot[idx_blue:idx_red] * z_corr,
-                                   where='mid', color=self._color_dict['fg'])
+                                   where='mid', color=theme.colors['fg'])
 
                         # Continuum bands
                         self._bands_plot(in_ax, wave_plot, flux_plot, z_corr, idcs_m, line_i)
 
                         # Plot the masked pixels
                         _masks_plot(in_ax, [line_i], wave_plot[idx_blue:idx_red], flux_plot[idx_blue:idx_red],
-                                    z_corr, log, idcs_mask[idx_blue:idx_red], self._color_dict)
+                                    z_corr, log, idcs_mask[idx_blue:idx_red], theme.colors)
 
                         # Plot the fitting results
                         if include_fits:
 
                             line_list, profiles_list = [line_i.label], line_i._p_shape
                             wave_array, gaussian_array = profiles_computation([line_i.label], log,
                                                                               (1 + self._spec.redshift), profiles_list)
                             wave_array, cont_array = linear_continuum_computation(line_list, self._spec.log,
                                                                                   (1 + self._spec.redshift))
 
                             # Single component lines
                             line_g_list = _gaussian_line_profiler(in_ax, line_list, wave_array, gaussian_array,
-                                                                  cont_array, z_corr, log, self._spec.norm_flux,
-                                                                  color_dict=self._color_dict)
+                                                                  cont_array, z_corr, log, self._spec.norm_flux)
 
                             # Add the interactive pop-ups
                             _mplcursor_parser(line_g_list, line_list, log, self._spec.norm_flux,
                                               self._spec.units_wave, self._spec.units_flux)
 
                         # Formatting the figure
                         in_ax.yaxis.set_major_locator(plt.NullLocator())
@@ -1195,16 +1226,16 @@
                 in_fig = save_close_fig_swicth(output_address, 'tight', in_fig, maximize, display_check)
 
         else:
             _logger.info('The bands log does not contain lines')
 
         return in_fig
 
-    def bands(self, line=None, bands=None, output_address=None, include_fits=True, rest_frame=False, y_scale='auto',
-              in_fig=None, fig_cfg={}, ax_cfg={}, maximize=False):
+    def bands(self, line=None, output_address=None, include_fits=True, rest_frame=False, y_scale='auto', fig_cfg=None,
+              ax_cfg=None, in_fig=None, maximize=False):
 
         """
 
         This function plots a spectrum ``line``. If a ``line`` is not provided the function will select the last line
         from the measurements log.
 
         The user can also introduce a ``bands`` dataframe (or its file path) to query the input ``line``.
@@ -1218,17 +1249,14 @@
 
         The default axes and plot titles can be modified via the ``ax_cfg``. These dictionary keys are "xlabel", "ylabel"
         and "title". It is not necessary to include all the keys in this argument.
 
         :param line: Line label to display.
         :type line: str, optional
 
-        :param bands: Bands array or dataframe (or its file) to display.
-        :type bands: np.array, pandas.Dataframe, str, path.pathlib, optional
-
         :param output_address: File location to store the plot.
         :type output_address: str, optional
 
         :param include_fits: Set to True to display fitted profiles. The default value is False.
         :type include_fits:  bool, optional
 
         :param rest_frame: Set to True for a display in rest frame. The default value is False
@@ -1274,16 +1302,16 @@
         # Proceed to plot
         if line is not None:
 
             # Guess whether we need both lines
             include_fits = include_fits and (line.intg_flux is not None)
 
             # Adjust the default theme
-            fig_cfg.setdefault('axes.labelsize', 14)
-            PLT_CONF, AXES_CONF = self._figure_format(fig_cfg, ax_cfg, norm_flux, units_wave, units_flux)
+            PLT_CONF = theme.fig_defaults(fig_cfg, fig_type='bands')
+            AXES_CONF = theme.ax_defaults(ax_cfg, units_wave, units_flux, norm_flux)
 
             # Create and fill the figure
             with rc_context(PLT_CONF):
 
                 # Generate the figure if not provided
                 if in_fig is None:
                     in_fig = plt.figure()
@@ -1311,15 +1339,15 @@
                 pixel_mask = 'no' if line not in log.index else log.loc[line, 'pixel_mask']
                 idcsEmis, idcsCont = define_masks(self._spec.wave, line.mask * (1 + self._spec.redshift), line_mask_entry=line.pixel_mask)
                 idcs_line = idcsEmis + idcsCont
 
                 # Plot the spectrum
                 label = '' if include_fits else line
                 in_ax[0].step(wave_plot[idcsM[0]:idcsM[5]] / z_corr, flux_plot[idcsM[0]:idcsM[5]] * z_corr,
-                              where='mid', color=self._color_dict['fg'], label=label)
+                              where='mid', color=theme.colors['fg'], label=label)
 
                 # Add the fitting results
                 if include_fits:
 
                     # Check components
                     list_comps = line.group_label.split('+') if line.blended_check else [line.label]
 
@@ -1328,16 +1356,15 @@
 
                     # Continuum bands
                     self._bands_plot(in_ax[0], wave_plot, flux_plot, z_corr, idcsM, line)
 
                     # Gaussian profiles
                     idcs_lines = self._spec.log.index.isin(list_comps)
                     line_g_list = _gaussian_line_profiler(in_ax[0], list_comps, wave_array, gaussian_array, cont_array,
-                                                          z_corr, log.loc[idcs_lines], norm_flux,
-                                                          color_dict=self._color_dict)
+                                                          z_corr, log.loc[idcs_lines], norm_flux)
 
                     # Add the interactive text
                     _mplcursor_parser(line_g_list, list_comps, log, norm_flux, units_wave, units_flux)
 
 
                     cont_linear_flux = (log.loc[list_comps[0], 'm_cont'] * wave_plot[idcsCont] + log.loc[list_comps[0], 'n_cont'])
                     linear_cont_std = np.std(cont_linear_flux - flux_plot[idcsCont]*norm_flux)
@@ -1351,49 +1378,44 @@
                     # Synchronizing the x-axis
                     in_ax[1].set_xlim(in_ax[0].get_xlim())
                     in_ax[1].set_xlabel(AXES_CONF['xlabel'])
                     in_ax[0].set_xlabel(None)
 
                 # Plot the masked pixels
                 _masks_plot(in_ax[0], [line], wave_plot[idcsM[0]:idcsM[5]], flux_plot[idcsM[0]:idcsM[5]], z_corr,
-                            log, idcs_mask[idcsM[0]:idcsM[5]], self._color_dict)
-
-                # # Line location
-                # if trans_line:
-                #     in_ax[0].axvline(line.wavelength, linestyle='--', alpha=0.5, color=self._color_dict['fg'])
+                            log, idcs_mask[idcsM[0]:idcsM[5]], theme.colors)
 
                 # Display the legend
                 in_ax[0].legend()
 
-                # in_ax[0].set_xscale('log')
                 # Set the scale
                 _auto_flux_scale(in_ax[0], y=flux_plot[idcsM[0]:idcsM[5]] * z_corr, y_scale=y_scale)
 
                 # By default, plot on screen unless an output address is provided
                 in_fig = save_close_fig_swicth(output_address, 'tight', in_fig, maximize, display_check)
 
         else:
             in_fig = None
             _logger.info(f'The line "{line}" was not found in the spectrum log for plotting.')
 
         return in_fig
 
-    def velocity_profile(self,  line=None, band=None, y_scale='linear', plt_cfg={}, ax_cfg={}, in_fig=None,
+    def velocity_profile(self, line=None, band=None, y_scale='linear', fig_cfg=None, ax_cfg=None, in_fig=None,
                          output_address=None, maximize=False):
 
         # Establish the line and band to user for the analysis
         line, band = check_line_for_bandplot(line, band, self._spec, _PARENT_BANDS)
 
         # Display check for the user figures
         display_check = True if in_fig is None else False
 
         # Adjust the default theme
-        ax_cfg.setdefault('xlabel',  'Velocity (Km/s)')
-        PLT_CONF, AXES_CONF = self._figure_format(plt_cfg, ax_cfg, self._spec.norm_flux, self._spec.units_wave,
-                                                  self._spec.units_flux)
+        PLT_CONF = theme.fig_defaults(fig_cfg)
+        AXES_CONF = theme.ax_defaults(ax_cfg, self._spec.units_wave, self._spec.units_flux, self._spec.norm_flux,
+                                      fig_type='velocity')
 
         # Recover the line data
         line = Line.from_log(line, self._spec.log, self._spec.norm_flux)
 
         # Line spectrum
         wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch_2(self._spec.wave, self._spec.flux,
                                                                       self._spec.redshift, False)
@@ -1422,40 +1444,40 @@
                 self._fig = in_fig
                 self._ax = self._fig.add_subplot()
 
             self._ax.set(**AXES_CONF)
             trans = self._ax.get_xaxis_transform()
 
             # Plot the spectrum
-            self._ax.step(vel_plot, flux_plot, label=line.latex_label, where='mid', color=self._color_dict['fg'])
+            self._ax.step(vel_plot, flux_plot, label=line.latex_label, where='mid', color=theme.colors['fg'])
 
             # Velocity percentiles
             target_percen = ['v_1', 'v_5', 'v_10', 'v_50', 'v_90', 'v_95', 'v_99']
             for i_percentil, percentil in enumerate(target_percen):
 
                 vel_per = line.__getattribute__(percentil)
                 label_text = None if i_percentil > 0 else r'$v_{Pth}$'
-                self._ax.axvline(x=vel_per, label=label_text, color=self._color_dict['fg'], linestyle='dotted', alpha=0.5)
+                self._ax.axvline(x=vel_per, label=label_text, color=theme.colors['fg'], linestyle='dotted', alpha=0.5)
 
                 label_plot = r'$v_{{{}}}$'.format(percentil[2:])
                 self._ax.text(vel_per, 0.80, label_plot, ha='center', va='center', rotation='vertical',
-                              backgroundcolor=self._color_dict['bg'], transform=trans, alpha=0.5)
+                              backgroundcolor=theme.colors['bg'], transform=trans, alpha=0.5)
 
             # Velocity edges
             label_v_i, label_v_f = r'$v_{{0}}$', r'$v_{{100}}$'
-            self._ax.axvline(x=v_i, alpha=0.5, color=self._color_dict['fg'], linestyle='dotted')
+            self._ax.axvline(x=v_i, alpha=0.5, color=theme.colors['fg'], linestyle='dotted')
             self._ax.text(v_i, 0.80, label_v_i, ha='center', va='center', rotation='vertical',
-                          backgroundcolor=self._color_dict['bg'], transform=trans, alpha=0.5)
+                          backgroundcolor=theme.colors['bg'], transform=trans, alpha=0.5)
 
-            self._ax.axvline(x=v_f, alpha=0.5, color=self._color_dict['fg'], linestyle='dotted')
+            self._ax.axvline(x=v_f, alpha=0.5, color=theme.colors['fg'], linestyle='dotted')
             self._ax.text(v_f, 0.80, label_v_f, ha='center', va='center', rotation='vertical',
-                          backgroundcolor=self._color_dict['bg'], transform=trans, alpha=0.5)
+                          backgroundcolor=theme.colors['bg'], transform=trans, alpha=0.5)
 
             # Plot the line profile
-            self._ax.plot(vel_plot, cont_plot, linestyle='--', color=self._color_dict['fg'])
+            self._ax.plot(vel_plot, cont_plot, linestyle='--', color=theme.colors['fg'])
 
             # Plot velocity bands
             w80 = line.v_90-line.v_10
             label_arrow = r'$w_{{80}}={:0.1f}\,Km/s$'.format(w80)
             p1 = patches.FancyArrowPatch((line.v_10, 0.4),
                                          (line.v_90, 0.4),
                                          label=label_arrow,
@@ -1474,19 +1496,19 @@
                                          color='tab:red',
                                          transform=self._ax.transData,
                                          mutation_scale=20)
             self._ax.add_patch(p2)
 
             # Median velocity
             label_vmed = r'$v_{{med}}={:0.1f}\,Km/s$'.format(line.v_med)
-            self._ax.axvline(x=line.v_med, color=self._color_dict['fg'], label=label_vmed, linestyle='dashed', alpha=0.5)
+            self._ax.axvline(x=line.v_med, color=theme.colors['fg'], label=label_vmed, linestyle='dashed', alpha=0.5)
 
             # Peak velocity
             label_vmed = r'$v_{{peak}}$'
-            self._ax.axvline(x=0.0, color=self._color_dict['fg'], label=label_vmed, alpha=0.5)
+            self._ax.axvline(x=0.0, color=theme.colors['fg'], label=label_vmed, alpha=0.5)
 
             # Set the scale
             _auto_flux_scale(self._ax, y=flux_plot, y_scale=y_scale)
 
             # Legend
             self._ax.legend()
 
@@ -1507,15 +1529,15 @@
         cont_i_resd = linear_continuum_computation(list_comps, log, z_corr=(1 + redshift), x_array=x)
         gaussian_i_resd = profiles_computation(list_comps, log, (1 + redshift), profile_list, x_array=x)
         total_resd = gaussian_i_resd.sum(axis=1) + cont_i_resd[:, 0]
 
         # Lower plot residual
         label_residual = r'$\frac{F_{obs} - F_{fit}}{F_{cont}}$'
         residual = ((y - total_resd / norm_flux) / (cont_level/norm_flux))
-        axis.step(x/z_corr, residual*z_corr, where='mid', color=self._color_dict['fg'])
+        axis.step(x/z_corr, residual*z_corr, where='mid', color=theme.colors['fg'])
 
         # Shade Continuum flux standard deviation # TODO revisit this calculation
         label = r'$\sigma_{Continuum}/\overline{F_{cont}}$'
         y_limit = cont_std / cont_level
         axis.fill_between(x/z_corr, -y_limit, +y_limit, facecolor='yellow', alpha=0.5, label=label)
 
         # Shade the pixel error spectrum if available:
@@ -1534,15 +1556,15 @@
             _logger.warning(f'Nan or inf entries in axis limit for {self.bands}')
 
         # Residual plot labeling
         axis.legend(loc='center right')
         axis.set_ylabel(label_residual, fontsize=22)
 
         # Spectrum mask
-        _masks_plot(axis, [list_comps[0]], x, y, z_corr, log, spec_mask, color_dict=self._color_dict)
+        _masks_plot(axis, [list_comps[0]], x, y, z_corr, log, spec_mask, color_dict=theme.colors)
 
         return
 
     def _continuum_iteration(self, wave, flux, continuum_fit, idcs_cont, low_lim, high_lim, threshold_factor,
                              plot_title=''):
 
         PLOT_CONF = STANDARD_PLOT.copy()
@@ -1707,21 +1729,24 @@
 
         # Check that the images have the same size
         check_image_size(bg_image, fg_image, masks_dict)
 
         # Use the input wcs or use the parent one
         wcs = self._cube.wcs if wcs is None else wcs
 
-        # State the plot labelling
-        AXES_CONF = image_map_labels(ax_cfg, wcs, line_bg, line_fg, masks_dict)
-
-        # User figure format overwrite default format
+        # False for embed figures
         display_check = True if in_fig is None else False
-        local_cfg = {'figure.figsize': (8 if masks_file is None else 15, 8), 'axes.titlesize': 14, 'legend.fontsize': 12}
-        PLT_CONF = parse_figure_format(fig_cfg, local_cfg)
+
+        # Set the plot format where the user's overwrites the default
+        size_conf = {'figure.figsize': (8 if masks_file is None else 15, 8)}
+        size_conf = size_conf if fig_cfg is None else {**size_conf, **fig_cfg}
+
+        PLT_CONF = theme.fig_defaults(size_conf)
+        AXES_CONF = theme.ax_defaults(ax_cfg, self._cube.units_wave, self._cube.units_flux, self._cube.norm_flux,
+                                      fig_type='cube', line_bg=line_bg, line_fg=line_fg, masks_dict=masks_dict, wcs=wcs)
 
         # Create and fill the figure
         with rc_context(PLT_CONF):
 
             if in_fig is None:
                 in_fig = plt.figure()
 
@@ -1764,27 +1789,27 @@
         # Container for the matplotlib figures
         self._fig, self._ax = None, None
         self._legend_handle = None
 
         return
 
     def spectra(self, obj_idcs=None, log_scale=False, output_address=None, rest_frame=False, include_fits=False,
-                legend_handle='levels', in_fig=None, in_axis=None, plt_cfg={}, ax_cfg={}, maximize=False):
+                legend_handle='levels', in_fig=None, in_axis=None, fig_cfg=None, ax_cfg=None, maximize=False):
 
         if self._sample.load_function is not None:
 
             legend_check = True
-            plt_cfg.setdefault('figure.figsize', (10, 6))
 
             norm_flux = self._sample.load_params.get('norm_flux')
-            units_wave = self._sample.load_params.get('units_wave')
-            units_flux = self._sample.load_params.get('units_flux')
+            units_wave = self._sample.units_wave
+            units_flux = self._sample.units_flux
 
-            PLT_CONF, AXES_CONF = self._figure_format(plt_cfg, ax_cfg, norm_flux=norm_flux,
-                                                      units_wave=units_wave, units_flux=units_flux)
+            # Adjust the default theme
+            PLT_CONF = theme.fig_defaults(fig_cfg)
+            AXES_CONF = theme.ax_defaults(ax_cfg, units_wave, units_flux, norm_flux)
 
             # Get the spectra list to plot
             if obj_idcs is None:
                 sub_sample = self._sample
             else:
                 sub_sample = self._sample[obj_idcs]
 
@@ -1897,14 +1922,16 @@
             for level, idcs in idcs_dict.items():
                 data_dict[level] = {'x_param': slice_df.loc[idcs, x_param].values,
                                     'y_values': slice_df.loc[idcs, y_param].values,
                                     'x_err': slice_df.loc[idcs, x_param_err].values if x_param_err in slice_df else None,
                                     'y_err': slice_df.loc[idcs, y_param_err].values if y_param_err in slice_df else None}
 
             # Default figure format
+
+
             fig_format = {**STANDARD_PLOT, **{'figure.figsize': (10, 6)}}
             ax_format = {'xlabel': _LOG_COLUMNS_LATEX.get(x_param, x_param), 'ylabel': _LOG_COLUMNS_LATEX.get(y_param, y_param)}
 
             # User format overwrites default params
             plt_cfg.update(fig_format)
             ax_cfg.update(ax_format)
 
@@ -1940,8 +1967,7 @@
 
         else:
             _logger.info(f'There is no data on the sample panel for the input observation selection')
 
         return
 
 
-theme = Themer()
```

### Comparing `lime-stable-0.9.99.1/src/lime/plots_interactive.py` & `lime-stable-0.9.99.5/src/lime/plots_interactive.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import pandas as pd
 
 from pathlib import Path
 from matplotlib import pyplot as plt, gridspec, rc_context
 from matplotlib.widgets import RadioButtons, SpanSelector, Slider
 from astropy.io import fits
 
-from .io import load_log, save_log, LiMe_Error, check_file_dataframe, _LINES_DATABASE_FILE, hdu_to_log_df
-from .plots import Plotter, frame_mask_switch_2, save_close_fig_swicth, _auto_flux_scale, parse_figure_format,\
-                    determine_cube_images, load_spatial_mask, check_image_size, image_map_labels, \
-                    image_plot, spec_plot, spatial_mask_plot, _masks_plot, axis_labeling
+from .io import load_frame, save_frame, LiMe_Error, check_file_dataframe, _LINES_DATABASE_FILE
+from .plots import Plotter, frame_mask_switch_2, save_close_fig_swicth, _auto_flux_scale,\
+                    determine_cube_images, load_spatial_mask, check_image_size, \
+                    image_plot, spec_plot, spatial_mask_plot, _masks_plot, theme
 
 
 from .tools import blended_label_from_log, define_masks
 from .transitions import label_decomposition, Line
 
 
 _logger = logging.getLogger('LiMe')
@@ -84,15 +84,15 @@
 
 def load_redshift_table(file_address, column_name):
 
     file_address = Path(file_address)
 
     # Open the file
     if file_address.is_file():
-        log = load_log(file_address)
+        log = load_frame(file_address)
         if not (column_name in log.columns):
             _logger.info(f'No column "{column_name}" found in input dataframe, a new column will be added to the file')
 
     # Load the file
     else:
         if file_address.parent.is_dir():
             log = pd.DataFrame(columns=[column_name])
@@ -145,15 +145,15 @@
 def save_or_clear_log(log, log_address, activeLines, log_parameters=['w1', 'w2', 'w3', 'w4', 'w5', 'w6'], input_log=None):
 
     if np.sum(activeLines) == 0:
         if log_address.is_file():
             log_address.unlink()
     else:
         if log_address is not None:
-            save_log(log.loc[activeLines], log_address, parameters=log_parameters)
+            save_frame(log_address, log.loc[activeLines], parameters=log_parameters)
         else:
             _logger.warning(r"Not output redshift log provided, the selection won't be stored")
 
     # Update the user input log to the new selection
     if input_log is not None:
         input_log = log.loc[activeLines]
 
@@ -178,21 +178,21 @@
         self._inter_mask = None
 
         self.line = None
         self.mask = None
         self.log = None
 
         self._idx_ax = None
-        self._color_bg = {True: 'white',
-                          False: 'xkcd:salmon'}
+        self._color_bg = {True: theme.colors['inspection_positive'],
+                          False: theme.colors['inspection_negative']}
 
         return
 
     def bands(self, bands_file, ref_bands=None, y_scale='auto', n_cols=6, n_rows=None, col_row_scale=(2, 1.5),
-              z_log_address=None, object_label=None, z_column='redshift', fig_cfg={}, ax_cfg={}, in_fig=None,
+              z_log_address=None, object_label=None, z_column='redshift', fig_cfg=None, ax_cfg=None, in_fig=None,
               maximize=False):
 
         # TODO the selection should be None
 
         """
 
         This function launches an interactive plot from which to select the line bands on the observed spectrum. If this
@@ -292,21 +292,20 @@
                 if n_rows is None:
                     n_rows = int(np.ceil(n_lines / n_cols))
             else:
                 n_cols, n_rows = n_lines, 1
             n_grid = n_cols * n_rows
 
             # Set the plot format where the user's overwrites the default
-            default_fig_cfg = {'figure.figsize': (n_cols * col_row_scale[0], n_rows * col_row_scale[1]),
-                               'axes.titlesize': 11}
-            default_fig_cfg.update(fig_cfg)
-            PLT_CONF, self._AXES_CONF = self._figure_format(default_fig_cfg, ax_cfg, norm_flux=self._spec.norm_flux,
-                                                            units_wave=self._spec.units_wave,
-                                                            units_flux=self._spec.units_flux)
-            self._AXES_CONF.pop('xlabel')
+            size_conf = {'figure.figsize': (n_cols * col_row_scale[0], n_rows * col_row_scale[1])}
+            size_conf = size_conf if fig_cfg is None else {**size_conf, **fig_cfg}
+
+            PLT_CONF = theme.fig_defaults(size_conf, fig_type='grid')
+            AXES_CONF = theme.ax_defaults(ax_cfg, self._spec.units_wave, self._spec.units_flux, self._spec.norm_flux,
+                                          fig_type=None)
 
             # Launch the interative figure
             with rc_context(PLT_CONF):
 
                 # Main structure
                 self._fig = plt.figure() if in_fig is None else in_fig
                 gs0 = self._fig.add_gridspec(2, 1, height_ratios=[1, 0.1])
@@ -351,15 +350,15 @@
                         self.z_df = pd.DataFrame(index=[self._obj_ref], columns=[self._redshift_column])
 
                     if self._redshift_column not in self.z_df.columns:
                         raise LiMe_Error(f'Input redshift log file does not have a {z_column} column.')
 
                     # Add the current value
                     self.z_df.loc[self._obj_ref, self._redshift_column] = self._spec.redshift
-                    save_log(self.z_df, self._redshift_log_path)
+                    save_frame(self._redshift_log_path, self.z_df)
 
                     self._z_orig = self._spec.redshift
                     self._inter_z = np.abs(self._spec.redshift - (self._spec.wave/(self._spec.wave_rest + self._inter_mask) - 1).mean())
                     z_slider = Slider(ax_sliders[1], 'Redshift\n($\Delta z$)', -10, 10, 0, valstep=1)
                     z_slider.on_changed(self._on_z_slider_MI)
 
                 # Connecting the figure to the interactive widgets
@@ -396,22 +395,22 @@
             # Establish the limits for the line spectrum plot
             mask = self.log.loc[list_comps[0], 'w1':'w6'] * (1 + self._spec.redshift)
             idcsM = np.searchsorted(wave_plot, mask)
             idxL = idcsM[0] - 5 if idcsM[0] > 5 else idcsM[0]
             idxH = idcsM[-1] + 5 if idcsM[-1] < idcsM[-1] + 5 else idcsM[-1]
 
             # Plot the spectrum
-            ax.step(wave_plot[idxL:idxH]/z_corr, flux_plot[idxL:idxH]*z_corr, where='mid', color=self._color_dict['fg'])
+            ax.step(wave_plot[idxL:idxH]/z_corr, flux_plot[idxL:idxH]*z_corr, where='mid', color=theme.colors['fg'])
 
             # Continuum bands
             self._bands_plot(ax, wave_plot, flux_plot, z_corr, idcsM, line)
 
             # Plot the masked pixels
             _masks_plot(ax, [line], wave_plot[idxL:idxH], flux_plot[idxL:idxH], z_corr, self.log, idcs_mask[idxL:idxH],
-                        color_dict=self._color_dict)
+                        color_dict=theme.colors)
 
             ax.axvline(self.log.loc[line, 'wavelength'], linestyle='--', color='grey', linewidth=0.5)
 
             # Formatting the figure
             ax.yaxis.set_major_locator(plt.NullLocator())
             ax.xaxis.set_major_locator(plt.NullLocator())
 
@@ -521,15 +520,15 @@
         for i, line in enumerate(self._lineList):
             self.ax_list[i].clear()
             self._plot_line_BI(self.ax_list[i], line, self._rest_frame, self._y_scale)
         self._fig.canvas.draw()
 
         # Save to the data frame
         self.z_df.loc[self._obj_ref, self._redshift_column] = z_new
-        save_log(self.z_df, self._redshift_log_path)
+        save_frame(self._redshift_log_path, self.z_df, )
 
         return
 
     def _on_mask_slider_MI(self, val):
 
         # Remove the previous value
         mask_matrix = self.log.loc[:, 'w1':'w6'].to_numpy() - self._sweep_mask
@@ -1078,15 +1077,15 @@
             _redshift_pred = redshift_output
 
         # Store the new redshift
         self._sample.loc[self._output_idcs, self._column_log] = _redshift_pred
 
         # Save to file if provided
         if self._log_address is not None:
-            save_log(self._sample.log, self._log_address)
+            save_frame(self._log_address, self._sample.log)
 
         return
 
     def _button_ZI(self, line_selection):
 
         # Button selection
         self._lineSelection = line_selection
@@ -1166,15 +1165,15 @@
         self.rest_frame = None
         self.log_scale = None
 
         return
 
     def cube(self, line, bands=None, line_fg=None, min_pctl_bg=60, cont_pctls_fg=(90, 95, 99), bg_cmap='gray',
              fg_cmap='viridis', bg_norm=None, fg_norm=None, masks_file=None, masks_cmap='viridis_r', masks_alpha=0.2,
-             rest_frame=False, log_scale=False, fig_cfg={}, ax_cfg_image={}, ax_cfg_spec={}, in_fig=None,
+             rest_frame=False, log_scale=False, fig_cfg=None, ax_cfg_image=None, ax_cfg_spec=None, in_fig=None,
              lines_log_file=None, ext_log='_LINELOG', wcs=None, maximize=False):
 
         """
 
         This function opens an interactive plot to display and individual spaxel spectrum from the selection on the
         image map.
 
@@ -1314,27 +1313,21 @@
         # Load the complete fits lines log if input
         if lines_log_file is not None:
             if Path(lines_log_file).is_file():
                 self.hdul_linelog = fits.open(lines_log_file, lazy_load_hdus=False)
             else:
                 _logger.info(f'The lines log at {lines_log_file} was not found.')
 
-        # State the plot labelling
-        default_ax_cfg_im = image_map_labels(ax_cfg_image, wcs, line_bg, line_fg, self.masks_dict)
-        default_ax_cfg_spec = dict(zip(('xlabel', 'ylabel'), axis_labeling(self._cube.norm_flux, self._cube.units_wave,
-                                                                           self._cube.units_flux)))
-        default_ax_cfg_spec.update(ax_cfg_spec)
-
-        # User configuration overwrite default figure format
-        local_cfg = {'figure.figsize': (16, 8), 'axes.titlesize': 12, 'legend.fontsize': 12, 'axes.labelsize': 12,
-                     'xtick.labelsize': 10, 'ytick.labelsize': 10}
-        self.fig_conf = parse_figure_format(fig_cfg, local_cfg)
-
-        # Container for both axes format
-        self.axes_conf = {'image': default_ax_cfg_im, 'spectrum': default_ax_cfg_spec}
+        # Get figure configuration configuration
+        self.fig_conf = theme.fig_defaults(fig_cfg, fig_type='cube_interactive')
+        ax_im = theme.ax_defaults(ax_cfg_image, self._cube.units_wave, self._cube.units_flux, self._cube.norm_flux,
+                                fig_type='cube', line_bg=line_bg, line_fg=line_fg, masks_dict=self.masks_dict, wcs=wcs)
+        ax_spec = theme.ax_defaults(ax_cfg_spec, self._cube.units_wave, self._cube.units_flux, self._cube.norm_flux,
+                               g_type='default', line_bg=line_bg, line_fg=line_fg, masks_dict=self.masks_dict, wcs=wcs)
+        self.axes_conf = {'image': ax_im, 'spectrum': ax_spec}
 
         # Create the figure
         with rc_context(self.fig_conf):
 
             # Figure structure
             self._fig = plt.figure() if in_fig is None else in_fig
             gs = gridspec.GridSpec(nrows=1, ncols=2, figure=self._fig, width_ratios=[1, 2], height_ratios=[1])
@@ -1416,15 +1409,15 @@
 
                 except KeyError:
                     _logger.info(f'Extension {ext_name} not found in the input file')
 
             # Plot spectrum
             spec_plot(self._ax1, self._cube.wave, flux_voxel, self._cube.redshift, self._cube.norm_flux,
                       rest_frame=self.rest_frame, log=log, units_wave=self._cube.units_wave,
-                      units_flux=self._cube.units_flux, color_dict=self._color_dict)
+                      units_flux=self._cube.units_flux, color_dict=theme.colors)
 
             if self.log_scale:
                 self._ax.set_yscale('log')
 
         # Update the axis
         self.axes_conf['spectrum']['title'] = f'Spaxel {idx_j} - {idx_i}'
         self._ax0.update(self.axes_conf['image'])
@@ -1583,31 +1576,23 @@
         self.bg_color, self.fg_color, self.mask_color, self.mask_alpha = bg_cmap, fg_cmap, masks_cmap, masks_alpha
 
         # Image mesh grid
         frame_size = self._cube.flux.shape
         y, x = np.arange(0, frame_size[1]), np.arange(0, frame_size[2])
         self.grid_mesh = np.meshgrid(x, y)
 
-
         self.mask_ext = 'CUM_SN'
 
-
-        # State the plot labelling
-        default_ax_cfg_im = image_map_labels(ax_cfg_image, wcs, line_bg, None, self.masks_dict)
-        default_ax_cfg_spec = dict(zip(('xlabel', 'ylabel'), axis_labeling(self._cube.norm_flux, self._cube.units_wave,
-                                                                           self._cube.units_flux)))
-        default_ax_cfg_spec.update(ax_cfg_spec)
-
-        # User configuration overwrite default figure format
-        local_cfg = {'figure.figsize': (10, 5), 'axes.titlesize': 10, 'legend.fontsize': 10, 'axes.labelsize': 10,
-                     'xtick.labelsize': 10, 'ytick.labelsize': 10}
-        self.fig_conf = parse_figure_format(fig_cfg, local_cfg)
-
-        # Container for both axes format
-        self.axes_conf = {'image': default_ax_cfg_im, 'spectrum': ax_cfg_spec}
+        # Get figure configuration configuration
+        self.fig_conf = theme.fig_defaults(fig_cfg, fig_type='cube_interactive')
+        ax_im = theme.ax_defaults(ax_cfg_image, self._cube.units_wave, self._cube.units_flux, self._cube.norm_flux,
+                                fig_type='cube', line_bg=line_bg, line_fg=None, masks_dict=self.masks_dict, wcs=wcs)
+        ax_spec = theme.ax_defaults(ax_cfg_spec, self._cube.units_wave, self._cube.units_flux, self._cube.norm_flux,
+                               g_type='default', line_bg=line_bg, line_fg=None, masks_dict=self.masks_dict, wcs=wcs)
+        self.axes_conf = {'image': ax_im, 'spectrum': ax_spec}
 
         # Create the figure
         with rc_context(self.fig_conf):
 
             # Figure structure
             self._fig = plt.figure() if in_fig is None else in_fig
             gs = gridspec.GridSpec(nrows=1, ncols=2, figure=self._fig, width_ratios=[1, 2], height_ratios=[1])
```

### Comparing `lime-stable-0.9.99.1/src/lime/read_fits.py` & `lime-stable-0.9.99.5/src/lime/read_fits.py`

 * *Files identical despite different names*

### Comparing `lime-stable-0.9.99.1/src/lime/recognition.py` & `lime-stable-0.9.99.5/src/lime/recognition.py`

 * *Files 4% similar despite different names*

```diff
@@ -141,19 +141,14 @@
 
     def peak_detection(self, limit_threshold=None, continuum=None, distance=4, ml_mask=None, plot_results=False):
 
         # No user imput provided compute the intensity threshold from the 84th percentil
         limit_threshold = np.percentile(self.flux, 84) if limit_threshold is None else limit_threshold
         limit_threshold = limit_threshold + continuum if continuum is not None else limit_threshold
 
-        # Index the intensity peaks
-        # input_flux = self.flux.data if np.ma.is_masked()
-        # mask_valid = ~self.flux.mask if np.ma.is_masked(self.flux) else np.ones(self.flux.data.size).astype(bool)
-        # peak_fp, _ = signal.find_peaks(self.flux.data[mask_valid], height=limit_threshold[mask_valid], distance=distance)
-
         peak_fp, _ = signal.find_peaks(self.flux, height=limit_threshold, distance=distance)
 
         # Plot the results
         if plot_results:
             self.plot._plot_peak_detection(peak_fp, limit_threshold, continuum, ml_mask=ml_mask,
                                       plot_title='Peak detection results ')
 
@@ -392,14 +387,15 @@
 
         # Remove nan entries
         idcs_nan_rows = np.isnan(input_flux).any(axis=1)
         input_flux = input_flux[~idcs_nan_rows, :]
 
         # Add Monte Carlo columns (7858, 13) To (7858, 13, 100)
 
+
         # Normalize the flux
         input_flux = feature_scaling(input_flux, transformation=scale_type, log_base=log_base)
 
         # Perform the 1D detection
         if box_width == model_dim:
             detection_array = model.predict(input_flux)
         else:
```

### Comparing `lime-stable-0.9.99.1/src/lime/resources/GradientDescent_v2_cost1_logNorm.joblib` & `lime-stable-0.9.99.5/src/lime/resources/GradientDescent_v2_cost1_logNorm.joblib`

 * *Files identical despite different names*

### Comparing `lime-stable-0.9.99.1/src/lime/resources/LogitistRegression_v2_cost1_logNorm.joblib` & `lime-stable-0.9.99.5/src/lime/resources/LogitistRegression_v2_cost1_logNorm.joblib`

 * *Files identical despite different names*

### Comparing `lime-stable-0.9.99.1/src/lime/resources/parent_bands.txt` & `lime-stable-0.9.99.5/src/lime/resources/parent_mask_v0.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-              wavelength     wave_vac             w1             w2             w3             w4             w5             w6        latex_label particle transition  rel_int
-H1_1216A       1215.1108    1215.6699    1100.000000    1150.000000    1195.000000    1230.000000    1250.000000    1300.000000        $HI1216\AA$       H1        rec        0
-C4_1548A       1547.6001    1548.1870    1400.000000    1450.000000    1530.000000    1565.000000    1600.000000    1650.000000      $CIV1548\AA$        C4        rec        0
-He2_1640A      1639.7896    1640.3913    1600.000000    1630.000000    1635.000000    1645.000000    1700.000000    1750.000000      $HeII1640\AA$      He2        rec        0
-O3_1666A       1665.5438    1666.1500    1600.000000    1630.000000    1660.000000    1680.000000    1700.000000    1750.000000    $[OIII]1666\AA$       O3        col        0
-C3_1909A       1908.0803    1908.7340    1870.000000    1895.000000    1898.187820    1912.243544    1930.000000    1950.000000     $CIII]1909\AA$       C3        sem        0
-Mg2_2803A      2802.6607    2803.5310    2700.000000    2750.000000    2790.000000    2810.000000    2850.000000    2900.000000    $[MgII]2803\AA$      Mg2        col        0
-Ne5_3426A      3426.0000    3426.0000    3390.000000    3410.000000    3420.000000    3430.000000    3445.000000    3465.000000     $[NeV]3426\AA$      Ne5        col        0
-H1_3704A       3703.8013    3704.9132    3671.309441    3681.364925    3700.450000    3709.100000    3758.000000    3764.000000        $HI3704\AA$       H1        rec        0
-O2_3726A       3726.0300    3727.1000    3665.750000    3694.260000    3716.020000    3743.700000    3754.880000    3767.500000     $[OII]3726\AA$       O2        col        0
-O2_3729A       3728.8200    3729.8600    3665.750000    3694.260000    3716.020000    3743.700000    3754.880000    3767.500000     $[OII]3729\AA$       O2        col        0
-H1_3750A       3750.0998    3751.2244    3664.503848    3675.720417    3746.433569    3756.674784    3775.220000    3792.040000        $HI3750\AA$       H1        rec        0
-H1_3771A       3770.5779    3771.7081    3759.191222    3767.280375    3767.467189    3775.787336    3776.807987    3782.905843        $HI3771\AA$       H1        rec        0
-H1_3798A       3797.8450    3798.9827    3780.949179    3792.078244    3793.707971    3803.676860    3807.127865    3816.774280        $HI3798\AA$       H1        rec        0
-H1_3835A       3835.3309    3836.4789    3823.148476    3829.538777    3831.331855    3840.896149    3844.260000    3852.830000        $HI3835\AA$       H1        rec        0
-Ne3_3869A      3868.7029    3869.8600    3848.429950    3858.099497    3862.724063    3876.597761    3895.538694    3910.048413   $[NeIII]3869\AA$      Ne3        col        0
-H1_3889A       3888.9950    3890.1577    3842.087829    3861.282614    3880.390000    3899.420000    3905.000000    3950.000000        $HI3889\AA$       H1        rec        0
-H1_3970A       3970.0170    3971.2020    3945.566344    3957.862489    3962.153343    3976.592758    3979.317175    3989.942405        $HI3970\AA$       H1        rec        0
-He1_4026A      4026.1340    4027.3345    4013.837737    4021.250734    4021.502052    4032.149534    4033.154014    4040.185370       $HeI4026\AA$      He1        rec        0
-S2_4069A       4068.5368    4069.7490    4058.171690    4064.665875    4065.093604    4073.198887    4080.376366    4086.974251     $[SII]4069\AA$       S2        col        0
-H1_4102A       4101.6777    4102.8991    4084.633589    4093.799103    4095.935564    4108.433334    4110.113141    4119.294537        $HI4102\AA$       H1        rec        0
-H1_4340A       4340.4035    4341.6910    4322.549217    4332.509864    4333.660230    4347.675999    4350.262697    4360.488238        $HI4340\AA$       H1        rec        0
-O3_4363A       4363.1421    4364.4360    4297.700000    4323.660000    4356.886082    4372.721331    4390.760000    4416.200000    $[OIII]4363\AA$       O3        col        0
-He1_4471A      4471.4164    4472.7404    4451.913360    4465.069336    4467.196330    4477.442236    4480.772156    4496.909458       $HeI4471\AA$      He1        rec        0
-Fe3_4658A      4658.0240    4659.4000    4637.507567    4650.238986    4653.613936    4666.293945    4669.709024    4679.097970   $[FeIII]4658\AA$      Fe3        col        0
-He2_4685A      4685.4956    4686.8793    4663.804252    4678.301808    4681.274066    4691.509985    4718.751912    4733.650293      $HeII4685\AA$      He2        rec        0
-Ar4_4711A      4711.1891    4712.5800    4664.639652    4680.894598    4707.992152    4720.882185    4723.932671    4738.660669    $[ArIV]4711\AA$      Ar4        col        0
-Ar4_4740A      4740.0511    4741.4500    4605.870000    4635.300000    4731.467840    4748.658238    4757.090000    4776.100000    $[ArIV]4740\AA$      Ar4        col        0
-H1_4861A       4861.2582    4862.6910    4809.800000    4836.100000    4848.715437    4876.181741    4883.130000    4908.400000        $HI4861\AA$       H1        rec        0
-He1_4922A      4921.8552    4923.3050    4905.736141    4916.176415    4917.632529    4928.081261    4930.590000    4939.710000       $HeI4922\AA$      He1        rec        0
-O3_4959A       4958.8348    4960.2950    4929.281844    4946.732665    4948.310671    4970.712011    4972.820372    4984.416360    $[OIII]4959\AA$       O3        col        0
-O3_5007A       5006.7664    5008.2400    4971.796688    4984.514249    4995.348943    5024.303156    5027.743260    5043.797081    $[OIII]5007\AA$       O3        col        0
-N2_5755A       5754.6400    5755.0000    5700.000000    5720.000000    5745.000000    5765.000000    5800.000000    5820.000000     $[NII]5755\AA$       N2        col        0
-He1_5876A      5875.5250    5877.2433    5845.715833    5865.712378    5867.148419    5885.578291    5888.378245    5901.854752       $HeI5876\AA$      He1        rec        0
-O1_6300A       6300.2076    6302.0460    6282.963147    6293.637954    6294.754436    6307.155360    6319.711710    6327.945925      $[OI]6300\AA$       O1        col        0
-S3_6312A       6311.9682    6313.8100    6280.559495    6295.351299    6307.225753    6319.552583    6321.428405    6328.663719    $[SIII]6312\AA$       S3        col        0
-N2_6548A       6547.9514    6549.8600    6480.030000    6520.660000    6540.100000    6555.950000    6627.700000    6661.820000     $[NII]6548\AA$       N2        col        0
-H1_6563A       6562.7192    6564.6320    6480.030000    6520.660000    6545.100000    6575.950000    6627.700000    6661.820000        $HI6563\AA$       H1        rec        0
-N2_6583A       6583.3513    6585.2700    6480.030000    6520.660000    6575.100000    6590.950000    6627.700000    6661.820000     $[NII]6583\AA$       N2        col        0
-He1_6678A      6678.0500    6679.9955    6659.110795    6670.102081    6670.734647    6688.067396    6689.800671    6698.178167       $HeI6678\AA$      He1        rec        0
-S2_6716A       6716.3386    6718.2950    6686.785257    6706.310255    6707.458647    6725.466528    6744.438091    6759.956250     $[SII]6716\AA$       S2        col        0
-S2_6731A       6730.7135    6732.6740    6686.785257    6706.310255    6725.458647    6741.466528    6744.438091    6759.956250     $[SII]6731\AA$       S2        col        0
-He1_7065A      7065.1078    7067.1633    7029.100000    7041.640000    7055.220000    7079.440000    7087.490000    7104.450000       $HeI7065\AA$      He1        rec        0
-Ar3_7136A      7135.6845    7137.7600    7099.804897    7122.016894    7129.546717    7145.645711    7149.984073    7166.354990   $[ArIII]7136\AA$      Ar3        col        0
-O2_7319A       7318.8124    7320.9400    7294.873033    7310.151519    7311.373798    7338.569503    7340.444100    7357.066344     $[OII]7319\AA$       O2        col        0
-O2_7330A       7329.5494    7331.6800    7294.873033    7310.151519    7311.373798    7338.569503    7340.444100    7357.066344     $[OII]7330\AA$       O2        col        0
-Ar3_7751A      7750.9894    7753.2400    7731.458685    7743.423077    7744.234222    7759.848767    7759.955932    7770.429591   $[ArIII]7751\AA$      Ar3        col        0
-H1_8392A       8392.2696    8394.7030    8378.449304    8387.961949    8388.394342    8398.627642    8398.730000    8409.950000        $HI8392\AA$       H1        rec        0
-H1_8413A       8413.1907    8415.6300    8399.595403    8407.110952    8410.140000    8418.040000    8423.876407    8432.548195        $HI8413\AA$       H1        rec        0
-H1_8438A       8437.8276    8440.2740    8396.910000    8408.320000    8432.872822    8443.316230    8452.150208    8464.463395        $HI8438\AA$       H1        rec        0
-H1_8467A       8467.1263    8469.5810    8450.080000    8459.460000    8461.707801    8473.595713    8474.880000    8493.320000        $HI8467\AA$       H1        rec        0
-H1_8502A       8502.3542    8504.8190    8474.500000    8491.730000    8499.235520    8509.640000    8511.060000    8533.050000        $HI8502\AA$       H1        rec        0
-H1_8545A       8545.2540    8547.7310    8515.180000    8536.310000    8539.268883    8552.720348    8555.470000    8574.470000        $HI8545\AA$       H1        rec        0
-H1_8598A       8598.2619    8600.7540    8556.050000    8573.810000    8590.837675    8605.251074    8607.110000    8622.240000        $HI8598\AA$       H1        rec        0
-H1_8665A       8664.8868    8667.3980    8635.370000    8656.680000    8657.198447    8673.721156    8684.080000    8699.840000        $HI8665\AA$       H1        rec        0
-H1_8750A       8750.3405    8752.8760    8722.780989    8743.677211    8744.762589    8759.907241    8760.041533    8772.919906        $HI8750\AA$       H1        rec        0
-H1_8863A       8862.6484    8865.2160    8826.510933    8849.703031    8856.225808    8873.619881    8875.570594    8886.725336        $HI8863\AA$       H1        rec        0
-H1_9015A       9014.7730    9017.3840    8975.870000    9001.890000    9009.997734    9023.899851    9029.944250    9048.681886        $HI9015\AA$       H1        rec        0
-S3_9068A       9068.4736    9071.1000    9028.280000    9056.360000    9057.861172    9081.241507    9083.325784    9100.603298    $[SIII]9068\AA$       S3        col        0
-H1_9229A       9228.8738    9231.5460    9204.503433    9221.674676    9222.628281    9238.719001    9239.094777    9251.786565        $HI9229\AA$       H1        rec        0
-S3_9530A       9530.4417    9533.2000    9471.122554    9489.978978    9516.201346    9545.330603    9569.193420    9600.501253    $[SIII]9530\AA$       S3        col        0
-H1_9546A       9545.8253    9548.5880    9471.122554    9489.978978    9535.201346    9556.330603    9569.193420    9600.501253        $HI9546\AA$       H1        rec        0
-H1_10049A     10049.2164   10052.1230    9963.330920   10014.100110   10033.912480   10078.490320   10085.683630   10157.030360       $HI10049\AA$       H1        rec        0
-He1_10830A    10830.1763   10833.3064   10753.419250   10794.263650   10802.042830   10855.528780   10856.984350   10895.058030      $HeI10830\AA$      He1        rec        0
-H1_10938A     10937.9211   10941.0820   10720.442470   10778.669070   10900.000000   10960.000000   11006.496460   11117.881210       $HI10938\AA$       H1        rec        0
-O1_11287A     11287.0000   11287.0000   11200.000000   11260.000000   11275.000000   11300.000000   11310.000000   11370.000000     $[OI]11287\AA$       O1        col        0
-Fe2_12566A    12566.0000   12566.0000   12485.000000   12540.000000   12555.000000   12575.000000   12585.000000   12630.000000   $[FeII]12566\AA$      Fe2        col        0
-H1_12818A     12817.8766   12821.5760   12707.118358   12770.347194   12798.311804   12848.895029   12883.388729   12974.122245       $HI12818\AA$       H1        rec        0
-Fe2_16443A    16443.2162   16447.9555   16410.000000   16425.000000   16435.000000   16445.000000   16470.000000   16485.000000   $[FeII]16443\AA$      Fe2        col        0
-H1_18751A     18750.6943   18756.0960   18609.558032   18656.837942   18721.051210   18796.838715   18813.400465   18894.450760       $HI18751\AA$       H1        rec        0
-H1_19445A     19445.2888   19450.8900   19316.427400   19392.542082   19425.601994   19470.194434   19488.494259   19546.645072       $HI19445\AA$       H1        rec        0
-H2_19570A     19570.3629   19576.0000   19317.214761   19417.398018   19531.524439   19609.655373   19622.326345   19678.132739    $[HII]19570\AA$       H2        col        0
-Si6_19640A    19640.3428   19646.0000   19595.000000   19610.000000   19615.000000   19625.000000   19635.000000   19655.000000   $[SiVI]19640\AA$      Si6        col        0
-He1_20587A    20580.9773   20586.9046   20436.136293   20506.474038   20553.752643   20619.278457   20638.302080   20718.624046      $HeI20587\AA$      He1        rec        0
-H2_21218A     21212.2213   21218.3300   21098.000543   21169.879588   21187.759064   21252.802441   21276.821582   21329.416005    $[HII]21218\AA$       H2        col        0
-H1_21661A     21654.9742   21661.2100   21519.246668   21614.386714   21634.197272   21692.559846   21726.878918   21795.633622       $HI21661\AA$       H1        rec        0
-H2_24066A     24058.9915   24065.9180   24000.000000   24020.000000   24040.000000   24100.000000   24120.000000   24150.000000    $[HII]24066\AA$       H2        col        0
-Si6_24830A    24822.8540   24830.0000   24790.000000   24800.000000   24820.000000   24840.000000   24840.000000   24860.000000   $[SiVI]24830\AA$      Si6        col        0
-H1_26259A     26251.1236   26258.6800   26200.000000   26220.000000   26245.000000   26275.000000   26300.000000   26320.000000       $HI26259\AA$       H1        rec        0
-H1_30392A     30383.2759   30392.0200   30365.000000   30375.000000   30385.000000   30405.000000   30415.000000   30425.000000       $HI30392\AA$       H1        rec        0
-H1_32970A     32960.4251   32969.9100   32945.000000   32955.000000   32965.000000   32975.000000   32985.000000   32995.000000       $HI32970\AA$       H1        rec        0
-PAH1_33000A   32990.5065   33000.0000   32800.000000   32850.000000   32900.000000   33100.000000   33150.000000   33200.000000   $[PAHI]33000\AA$     PAH1        col        0
-H1_37406A     37394.7903   37405.5500   37365.000000   37385.000000   37395.000000   37415.000000   37425.000000   37440.000000       $HI37406\AA$       H1        rec        0
-H1_40523A     40511.0344   40522.6900   40490.000000   40500.000000   40510.000000   40535.000000   40550.000000   40570.000000       $HI40523\AA$       H1        rec        0
-H1_46538A     46524.3554   46537.7400   46510.000000   46515.000000   46534.000000   46546.000000   46555.000000   46575.000000       $HI46538\AA$       H1        rec        0
-S4_105105A   105074.7773  105105.0000  104700.000000  104900.000000  105000.000000  105200.000000  105300.000000  105500.000000   $[SIV]105105\AA$       S4        col        0
-S3_187130A   187076.1931  187130.0000  186700.000000  186900.000000  187100.000000  187160.000000  187200.000000  187300.000000  $[SIII]187130\AA$       S3        col        0
+              wavelength     wave_vac             w1             w2             w3             w4             w5             w6                 latex_label particle transition  rel_int
+H1_1216A       1215.1108    1215.6699    1100.000000    1150.000000    1195.000000    1230.000000    1250.000000    1300.000000        $HI1216\mathring{A}$       H1        rec        0
+C4_1548A       1547.6001    1548.1870    1400.000000    1450.000000    1530.000000    1565.000000    1600.000000    1650.000000       $CIV1548\mathring{A}$       C4        rec        0
+He2_1640A      1639.7896    1640.3913    1600.000000    1630.000000    1635.000000    1645.000000    1700.000000    1750.000000      $HeII1640\mathring{A}$      He2        rec        0
+O3_1666A       1665.5438    1666.1500    1600.000000    1630.000000    1660.000000    1680.000000    1700.000000    1750.000000    $[OIII]1666\mathring{A}$       O3        col        0
+C3_1909A       1908.0803    1908.7340    1870.000000    1895.000000    1898.187820    1912.243544    1930.000000    1950.000000     $CIII]1909\mathring{A}$       C3        sem        0
+Mg2_2803A      2802.6607    2803.5310    2700.000000    2750.000000    2790.000000    2810.000000    2850.000000    2900.000000    $[MgII]2803\mathring{A}$      Mg2        col        0
+Ne5_3426A      3426.0000    3426.0000    3390.000000    3410.000000    3420.000000    3430.000000    3445.000000    3465.000000     $[NeV]3426\mathring{A}$      Ne5        col        0
+H1_3704A       3703.8013    3704.9132    3671.309441    3681.364925    3700.450000    3709.100000    3758.000000    3764.000000        $HI3704\mathring{A}$       H1        rec        0
+O2_3726A       3726.0300    3727.1000    3665.750000    3694.260000    3716.020000    3743.700000    3754.880000    3767.500000     $[OII]3726\mathring{A}$       O2        col        0
+O2_3729A       3728.8200    3729.8600    3665.750000    3694.260000    3716.020000    3743.700000    3754.880000    3767.500000     $[OII]3729\mathring{A}$       O2        col        0
+H1_3750A       3750.0998    3751.2244    3664.503848    3675.720417    3746.433569    3756.674784    3775.220000    3792.040000        $HI3750\mathring{A}$       H1        rec        0
+H1_3771A       3770.5779    3771.7081    3759.191222    3767.280375    3767.467189    3775.787336    3776.807987    3782.905843        $HI3771\mathring{A}$       H1        rec        0
+H1_3798A       3797.8450    3798.9827    3780.949179    3792.078244    3793.707971    3803.676860    3807.127865    3816.774280        $HI3798\mathring{A}$       H1        rec        0
+H1_3835A       3835.3309    3836.4789    3823.148476    3829.538777    3831.331855    3840.896149    3844.260000    3852.830000        $HI3835\mathring{A}$       H1        rec        0
+Ne3_3869A      3868.7029    3869.8600    3848.429950    3858.099497    3862.724063    3876.597761    3895.538694    3910.048413   $[NeIII]3869\mathring{A}$      Ne3        col        0
+H1_3889A       3888.9950    3890.1577    3842.087829    3861.282614    3880.390000    3899.420000    3905.000000    3950.000000        $HI3889\mathring{A}$       H1        rec        0
+H1_3970A       3970.0170    3971.2020    3945.566344    3957.862489    3962.153343    3976.592758    3979.317175    3989.942405        $HI3970\mathring{A}$       H1        rec        0
+He1_4026A      4026.1340    4027.3345    4013.837737    4021.250734    4021.502052    4032.149534    4033.154014    4040.185370       $HeI4026\mathring{A}$      He1        rec        0
+S2_4069A       4068.5368    4069.7490    4058.171690    4064.665875    4065.093604    4073.198887    4080.376366    4086.974251     $[SII]4069\mathring{A}$       S2        col        0
+H1_4102A       4101.6777    4102.8991    4084.633589    4093.799103    4095.935564    4108.433334    4110.113141    4119.294537        $HI4102\mathring{A}$       H1        rec        0
+H1_4340A       4340.4035    4341.6910    4322.549217    4332.509864    4333.660230    4347.675999    4350.262697    4360.488238        $HI4340\mathring{A}$       H1        rec        0
+O3_4363A       4363.1421    4364.4360    4297.700000    4323.660000    4356.886082    4372.721331    4390.760000    4416.200000    $[OIII]4363\mathring{A}$       O3        col        0
+He1_4471A      4471.4164    4472.7404    4451.913360    4465.069336    4467.196330    4477.442236    4480.772156    4496.909458       $HeI4471\mathring{A}$      He1        rec        0
+Fe3_4658A      4658.0240    4659.4000    4637.507567    4650.238986    4653.613936    4666.293945    4669.709024    4679.097970   $[FeIII]4658\mathring{A}$      Fe3        col        0
+He2_4685A      4685.4956    4686.8793    4663.804252    4678.301808    4681.274066    4691.509985    4718.751912    4733.650293      $HeII4685\mathring{A}$      He2        rec        0
+Ar4_4711A      4711.1891    4712.5800    4664.639652    4680.894598    4707.992152    4720.882185    4723.932671    4738.660669    $[ArIV]4711\mathring{A}$      Ar4        col        0
+Ar4_4740A      4740.0511    4741.4500    4605.870000    4635.300000    4731.467840    4748.658238    4757.090000    4776.100000    $[ArIV]4740\mathring{A}$      Ar4        col        0
+H1_4861A       4861.2582    4862.6910    4809.800000    4836.100000    4848.715437    4876.181741    4883.130000    4908.400000        $HI4861\mathring{A}$       H1        rec        0
+He1_4922A      4921.8552    4923.3050    4905.736141    4916.176415    4917.632529    4928.081261    4930.590000    4939.710000       $HeI4922\mathring{A}$      He1        rec        0
+O3_4959A       4958.8348    4960.2950    4929.281844    4946.732665    4948.310671    4970.712011    4972.820372    4984.416360    $[OIII]4959\mathring{A}$       O3        col        0
+O3_5007A       5006.7664    5008.2400    4971.796688    4984.514249    4995.348943    5024.303156    5027.743260    5043.797081    $[OIII]5007\mathring{A}$       O3        col        0
+N2_5755A       5754.6400    5755.0000    5700.000000    5720.000000    5745.000000    5765.000000    5800.000000    5820.000000     $[NII]5755\mathring{A}$       N2        col        0
+He1_5876A      5875.5250    5877.2433    5845.715833    5865.712378    5867.148419    5885.578291    5888.378245    5901.854752       $HeI5876\mathring{A}$      He1        rec        0
+O1_6300A       6300.2076    6302.0460    6282.963147    6293.637954    6294.754436    6307.155360    6319.711710    6327.945925      $[OI]6300\mathring{A}$       O1        col        0
+S3_6312A       6311.9682    6313.8100    6280.559495    6295.351299    6307.225753    6319.552583    6321.428405    6328.663719    $[SIII]6312\mathring{A}$       S3        col        0
+N2_6548A       6547.9514    6549.8600    6480.030000    6520.660000    6540.100000    6555.950000    6627.700000    6661.820000     $[NII]6548\mathring{A}$       N2        col        0
+H1_6563A       6562.7192    6564.6320    6480.030000    6520.660000    6545.100000    6575.950000    6627.700000    6661.820000        $HI6563\mathring{A}$       H1        rec        0
+N2_6583A       6583.3513    6585.2700    6480.030000    6520.660000    6575.100000    6590.950000    6627.700000    6661.820000     $[NII]6583\mathring{A}$       N2        col        0
+He1_6678A      6678.0500    6679.9955    6659.110795    6670.102081    6670.734647    6688.067396    6689.800671    6698.178167       $HeI6678\mathring{A}$      He1        rec        0
+S2_6716A       6716.3386    6718.2950    6686.785257    6706.310255    6707.458647    6725.466528    6744.438091    6759.956250     $[SII]6716\mathring{A}$       S2        col        0
+S2_6731A       6730.7135    6732.6740    6686.785257    6706.310255    6725.458647    6741.466528    6744.438091    6759.956250     $[SII]6731\mathring{A}$       S2        col        0
+He1_7065A      7065.1078    7067.1633    7029.100000    7041.640000    7055.220000    7079.440000    7087.490000    7104.450000       $HeI7065\mathring{A}$      He1        rec        0
+Ar3_7136A      7135.6845    7137.7600    7099.804897    7122.016894    7129.546717    7145.645711    7149.984073    7166.354990   $[ArIII]7136\mathring{A}$      Ar3        col        0
+O2_7319A       7318.8124    7320.9400    7294.873033    7310.151519    7311.373798    7338.569503    7340.444100    7357.066344     $[OII]7319\mathring{A}$       O2        col        0
+O2_7330A       7329.5494    7331.6800    7294.873033    7310.151519    7311.373798    7338.569503    7340.444100    7357.066344     $[OII]7330\mathring{A}$       O2        col        0
+Ar3_7751A      7750.9894    7753.2400    7731.458685    7743.423077    7744.234222    7759.848767    7759.955932    7770.429591   $[ArIII]7751\mathring{A}$      Ar3        col        0
+H1_8392A       8392.2696    8394.7030    8378.449304    8387.961949    8388.394342    8398.627642    8398.730000    8409.950000        $HI8392\mathring{A}$       H1        rec        0
+H1_8413A       8413.1907    8415.6300    8399.595403    8407.110952    8410.140000    8418.040000    8423.876407    8432.548195        $HI8413\mathring{A}$       H1        rec        0
+H1_8438A       8437.8276    8440.2740    8396.910000    8408.320000    8432.872822    8443.316230    8452.150208    8464.463395        $HI8438\mathring{A}$       H1        rec        0
+H1_8467A       8467.1263    8469.5810    8450.080000    8459.460000    8461.707801    8473.595713    8474.880000    8493.320000        $HI8467\mathring{A}$       H1        rec        0
+H1_8502A       8502.3542    8504.8190    8474.500000    8491.730000    8499.235520    8509.640000    8511.060000    8533.050000        $HI8502\mathring{A}$       H1        rec        0
+H1_8545A       8545.2540    8547.7310    8515.180000    8536.310000    8539.268883    8552.720348    8555.470000    8574.470000        $HI8545\mathring{A}$       H1        rec        0
+H1_8598A       8598.2619    8600.7540    8556.050000    8573.810000    8590.837675    8605.251074    8607.110000    8622.240000        $HI8598\mathring{A}$       H1        rec        0
+H1_8665A       8664.8868    8667.3980    8635.370000    8656.680000    8657.198447    8673.721156    8684.080000    8699.840000        $HI8665\mathring{A}$       H1        rec        0
+H1_8750A       8750.3405    8752.8760    8722.780989    8743.677211    8744.762589    8759.907241    8760.041533    8772.919906        $HI8750\mathring{A}$       H1        rec        0
+H1_8863A       8862.6484    8865.2160    8826.510933    8849.703031    8856.225808    8873.619881    8875.570594    8886.725336        $HI8863\mathring{A}$       H1        rec        0
+H1_9015A       9014.7730    9017.3840    8975.870000    9001.890000    9009.997734    9023.899851    9029.944250    9048.681886        $HI9015\mathring{A}$       H1        rec        0
+S3_9068A       9068.4736    9071.1000    9028.280000    9056.360000    9057.861172    9081.241507    9083.325784    9100.603298    $[SIII]9068\mathring{A}$       S3        col        0
+H1_9229A       9228.8738    9231.5460    9204.503433    9221.674676    9222.628281    9238.719001    9239.094777    9251.786565        $HI9229\mathring{A}$       H1        rec        0
+S3_9530A       9530.4417    9533.2000    9471.122554    9489.978978    9516.201346    9545.330603    9569.193420    9600.501253    $[SIII]9530\mathring{A}$       S3        col        0
+H1_9546A       9545.8253    9548.5880    9471.122554    9489.978978    9535.201346    9556.330603    9569.193420    9600.501253        $HI9546\mathring{A}$       H1        rec        0
+H1_10049A     10049.2164   10052.1230    9963.330920   10014.100110   10033.912480   10078.490320   10085.683630   10157.030360       $HI10049\mathring{A}$       H1        rec        0
+He1_10830A    10830.1763   10833.3064   10753.419250   10794.263650   10802.042830   10855.528780   10856.984350   10895.058030      $HeI10830\mathring{A}$      He1        rec        0
+H1_10938A     10937.9211   10941.0820   10720.442470   10778.669070   10900.000000   10960.000000   11006.496460   11117.881210       $HI10938\mathring{A}$       H1        rec        0
+O1_11287A     11287.0000   11287.0000   11200.000000   11260.000000   11275.000000   11300.000000   11310.000000   11370.000000     $[OI]11287\mathring{A}$       O1        col        0
+Fe2_12566A    12566.0000   12566.0000   12485.000000   12540.000000   12555.000000   12575.000000   12585.000000   12630.000000   $[FeII]12566\mathring{A}$      Fe2        col        0
+H1_12818A     12817.8766   12821.5760   12707.118358   12770.347194   12798.311804   12848.895029   12883.388729   12974.122245       $HI12818\mathring{A}$       H1        rec        0
+Fe2_16443A    16443.2162   16447.9555   16410.000000   16425.000000   16435.000000   16445.000000   16470.000000   16485.000000   $[FeII]16443\mathring{A}$      Fe2        col        0
+H1_18751A     18750.6943   18756.0960   18609.558032   18656.837942   18721.051210   18796.838715   18813.400465   18894.450760       $HI18751\mathring{A}$       H1        rec        0
+H1_19445A     19445.2888   19450.8900   19316.427400   19392.542082   19425.601994   19470.194434   19488.494259   19546.645072       $HI19445\mathring{A}$       H1        rec        0
+H2_19570A     19570.3629   19576.0000   19317.214761   19417.398018   19531.524439   19609.655373   19622.326345   19678.132739    $[HII]19570\mathring{A}$       H2        col        0
+Si6_19640A    19640.3428   19646.0000   19595.000000   19610.000000   19615.000000   19625.000000   19635.000000   19655.000000   $[SiVI]19640\mathring{A}$      Si6        col        0
+He1_20587A    20580.9773   20586.9046   20436.136293   20506.474038   20553.752643   20619.278457   20638.302080   20718.624046      $HeI20587\mathring{A}$      He1        rec        0
+H2_21218A     21212.2213   21218.3300   21098.000543   21169.879588   21187.759064   21252.802441   21276.821582   21329.416005    $[HII]21218\mathring{A}$       H2        col        0
+H1_21661A     21654.9742   21661.2100   21519.246668   21614.386714   21634.197272   21692.559846   21726.878918   21795.633622       $HI21661\mathring{A}$       H1        rec        0
+H2_24066A     24058.9915   24065.9180   24000.000000   24020.000000   24040.000000   24100.000000   24120.000000   24150.000000    $[HII]24066\mathring{A}$       H2        col        0
+Si6_24830A    24822.8540   24830.0000   24790.000000   24800.000000   24820.000000   24840.000000   24840.000000   24860.000000   $[SiVI]24830\mathring{A}$      Si6        col        0
+H1_26259A     26251.1236   26258.6800   26200.000000   26220.000000   26245.000000   26275.000000   26300.000000   26320.000000       $HI26259\mathring{A}$       H1        rec        0
+H1_30392A     30383.2759   30392.0200   30365.000000   30375.000000   30385.000000   30405.000000   30415.000000   30425.000000       $HI30392\mathring{A}$       H1        rec        0
+H1_32970A     32960.4251   32969.9100   32945.000000   32955.000000   32965.000000   32975.000000   32985.000000   32995.000000       $HI32970\mathring{A}$       H1        rec        0
+PAH1_33000A   32990.5065   33000.0000   32800.000000   32850.000000   32900.000000   33100.000000   33150.000000   33200.000000   $[PAHI]33000\mathring{A}$     PAH1        col        0
+H1_37406A     37394.7903   37405.5500   37365.000000   37385.000000   37395.000000   37415.000000   37425.000000   37440.000000       $HI37406\mathring{A}$       H1        rec        0
+H1_40523A     40511.0344   40522.6900   40490.000000   40500.000000   40510.000000   40535.000000   40550.000000   40570.000000       $HI40523\mathring{A}$       H1        rec        0
+H1_46538A     46524.3554   46537.7400   46510.000000   46515.000000   46534.000000   46546.000000   46555.000000   46575.000000       $HI46538\mathring{A}$       H1        rec        0
+S4_105105A   105074.7773  105105.0000  104700.000000  104900.000000  105000.000000  105200.000000  105300.000000  105500.000000   $[SIV]105105\mathring{A}$       S4        col        0
+S3_187130A   187076.1931  187130.0000  186700.000000  186900.000000  187100.000000  187160.000000  187200.000000  187300.000000  $[SIII]187130\mathring{A}$       S3        col        0
```

### Comparing `lime-stable-0.9.99.1/src/lime/resources/sketch.py` & `lime-stable-0.9.99.5/src/lime/resources/sketch.py`

 * *Files identical despite different names*

### Comparing `lime-stable-0.9.99.1/src/lime/resources/types_params.txt` & `lime-stable-0.9.99.5/src/lime/resources/types_params.txt`

 * *Files identical despite different names*

### Comparing `lime-stable-0.9.99.1/src/lime/resources/types_params2.txt` & `lime-stable-0.9.99.5/src/lime/resources/types_params2.txt`

 * *Files identical despite different names*

### Comparing `lime-stable-0.9.99.1/src/lime/tables.py` & `lime-stable-0.9.99.5/src/lime/tables.py`

 * *Files identical despite different names*

### Comparing `lime-stable-0.9.99.1/src/lime/tools.py` & `lime-stable-0.9.99.5/src/lime/tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 __all__ = ['unit_conversion',
            'extract_fluxes',
            'normalize_fluxes',
-           'redshift_calculation']
+           'redshift_calculation',
+           'save_parameter_maps']
 
 import logging
 import numpy as np
 import pandas as pd
 
-from .io import LiMe_Error, load_log, log_to_HDU
+from .io import LiMe_Error, load_frame, log_to_HDU
 from sys import stdout
 
 from astropy import units as au
 from astropy.units.core import CompositeUnit, IrreducibleUnit, Unit
 
 from astropy.io import fits
 from pathlib import Path
@@ -61,14 +62,28 @@
         for _ in range(num // VAL_LIST[i]):
             roman_num += SYB_LIST[i]
             num -= VAL_LIST[i]
         i += 1
     return roman_num
 
 
+def pd_get(df, row, column, default=None, transform=None):
+
+    # Fast get from dataframe
+    try:
+        cell = df.at[row, column]
+    except KeyError:
+        cell = default
+
+    # Transform the value from the dataframe to the default if requested
+    if transform is not None:
+        cell = default if cell == transform else cell
+
+    return cell
+
 # Favoured method to get line fluxes according to resolution
 def extract_fluxes(log, flux_type='mixture', sample_level='line', column_name='line_flux', column_positions=None):
 
     if flux_type not in ('mixture', 'intg', 'profile'):
         raise LiMe_Error(f'Flux type "{flux_type}" is not recognized please one of "intg", "profile", or "mixture" ')
 
     # Get indeces of blended lines
@@ -660,15 +675,15 @@
                                                       character_as_bytes=False)
                         # Append
                         if hdu_i is not None:
                             hdulist.append(hdu_i)
 
             # Remaining types
             else:
-                df_i = load_log(log_path, levels=levels)
+                df_i = load_frame(log_path, levels=levels)
                 name_i = log_path.stem
                 hdu_i = log_to_HDU(df_i, ext_name=name_i)
 
                 # Append
                 if hdu_i is not None:
                     hdulist.append(hdu_i)
 
@@ -709,46 +724,253 @@
     # Check if input are already astropy units
     units_wave = au.Unit(units_wave) if not isinstance(units_wave, (IrreducibleUnit, CompositeUnit, Unit)) else units_wave
     units_flux = au.Unit(units_flux) if not isinstance(units_flux, (IrreducibleUnit, CompositeUnit, Unit)) else units_flux
 
     return units_wave, units_flux
 
 
+def save_parameter_maps(lines_log_file, output_folder, param_list, line_list, mask_file=None, mask_list='all',
+                        image_shape=None, log_ext_suffix='_LINELOG', spaxel_fill_value=np.nan, output_file_prefix=None,
+                        header=None, wcs=None):
+
+    """
+
+    This function converts a line measurements log from an IFS cube, into a set of 2D parameter maps.
+
+    The parameter ".fits" files are saved into the ``output_folder``. These files are named after the parameters in the
+    ``param_list`` with the optional prefix from the ``output_file_prefix`` argument. These files will have one page per
+    line in the ``line_list`` argument.
+
+    The user can provide a spatial mask file address from which to recover the spaxels with line measurements. If the
+    mask ``.fits`` file contains several pages, the user can provide a ``mask_list`` with the ones to explore. Otherwise,
+    all mask pages will be used.
+
+    .. attention::
+        The user can provide an ``image_shape`` tuple to generate the output parameter map. However, for a large image
+        size this approach may require a long time to query the log file pages.
+
+    The expected page name in the input ``lines_log_file`` is "idx_j-idx_i_log_ext_suffix" where "idx_j" and "idx_i"
+    are the y and x array coordinates of the cube coordinates, by default ``log_ext_suffix='_LINELOG'``.
+
+    The output ``.fits`` parameter page header includes the ``PARAM`` and ``LINE`` entries with the line and parameter
+    labels respectively. The user should also include a ``wcs`` argument to export the astronomical coordinates to the
+    output files. The user can add additional information via the ``header`` argument.
+
+    :param lines_log_file: Fits file with IFU cube line measurements.
+    :param lines_log_file: str, pathlib.Path
+
+    :param param_list: List of parameters to map
+    :param param_list: list
+
+    :param line_list: List of lines to map
+    :param line_list: list
+
+    :param output_folder: Output folder to save the maps
+    :param output_folder: str, pathlib.Path
+
+    :param mask_file: Address of binary spatial mask file
+    :type mask_file: str, pathlib.Path
+
+    :param mask_list: Mask name list to explore on the ``mask_file``.
+    :type mask_list: list, optional
+
+    :param image_shape: Array with the image spatial size.
+    :param image_shape: list, tuple, optional
+
+    :param spaxel_fill_value: Map filling value for empty pixels. The default value is "numpy.nan".
+    :param spaxel_fill_value: float, optional
+
+    :param log_ext_suffix: Suffix for the lines log extension. The default value is "_LINELOG"
+    :param log_ext_suffix: str, optional
+
+    :param output_file_prefix: Prefix for the output parameter ".fits" file. The default value is None.
+    :param output_file_prefix: str, optional
+
+    :param header: Dictionary for parameter ".fits" file header
+    :type header: dict, optional
+
+    :param wcs: Observation `world coordinate system <https://docs.astropy.org/en/stable/wcs/index.html>`_.
+    :type wcs: astropy WCS, optional
+
+    """
+
+    assert Path(lines_log_file).is_file(), f'- ERROR: lines log at {lines_log_file} not found'
+    assert Path(output_folder).is_dir(), f'- ERROR: Output parameter maps folder {output_folder} not found'
+
+    # Compile the list of voxels to recover the provided masks
+    if mask_file is not None:
+
+        assert Path(mask_file).is_file(), f'- ERROR: mask file at {mask_file} not found'
+
+        with fits.open(mask_file) as maskHDUs:
+
+            # Get the list of mask extensions
+            if mask_list == 'all':
+                if ('PRIMARY' in maskHDUs) and (len(maskHDUs) > 1):
+                    mask_list = []
+                    for i, HDU in enumerate(maskHDUs):
+                        mask_name = HDU.name
+                        if mask_name != 'PRIMARY':
+                            mask_list.append(mask_name)
+                    mask_list = np.array(mask_list)
+                else:
+                    mask_list = np.array(['PRIMARY'])
+            else:
+                mask_list = np.array(mask_list, ndmin=1)
+
+            # Combine all the mask voxels into one
+            for i, mask_name in enumerate(mask_list):
+                if i == 0:
+                    mask_array = maskHDUs[mask_name].data
+                    image_shape = mask_array.shape
+                else:
+                    assert image_shape == maskHDUs[mask_name].data.shape, '- ERROR: Input masks do not have the same dimensions'
+                    mask_array += maskHDUs[mask_name].data
+
+            # Convert to boolean
+            mask_array = mask_array.astype(bool)
+
+            # List of spaxels in list [(idx_j, idx_i), ...] format
+            spaxel_list = np.argwhere(mask_array)
+
+    # No mask file is provided and the user just defines an image size tupple (nY, nX)
+    else:
+        mask_array = np.ones(image_shape).astype(bool)
+        spaxel_list = np.argwhere(mask_array)
+
+    # Generate containers for the data:
+    images_dict = {}
+    for param in param_list:
+
+        # Make sure is an array and loop throuh them
+        for line in line_list:
+            images_dict[f'{param}-{line}'] = np.full(image_shape, spaxel_fill_value)
+
+    # Loop through the spaxels and fill the parameter images
+    n_spaxels = spaxel_list.shape[0]
+    spaxel_range = np.arange(n_spaxels)
+    pbar = ProgressBar('bar', f'spaxels from file')
+
+    with fits.open(lines_log_file) as logHDUs:
+
+        for i_spaxel in spaxel_range:
+            idx_j, idx_i = spaxel_list[i_spaxel]
+            spaxel_ref = f'{idx_j}-{idx_i}{log_ext_suffix}'
+
+            post_text = f'of spaxels from file ({lines_log_file}) read ({n_spaxels} total spaxels)'
+            pbar.output_message(i_spaxel, n_spaxels, pre_text="", post_text=post_text)
+
+            # progress_bar(i_spaxel, n_spaxels, post_text=f'of spaxels from file ({lines_log_file}) read ({n_spaxels} total spaxels)')
+
+            # Confirm log extension exists
+            if spaxel_ref in logHDUs:
+
+                # Recover extension data
+                log_data = logHDUs[spaxel_ref].data
+                log_lines = log_data['index']
+
+                # Loop through the parameters and the lines:
+                for param in param_list:
+                    idcs_log = np.argwhere(np.in1d(log_lines, line_list))
+                    for i_line in idcs_log:
+                        images_dict[f'{param}-{log_lines[i_line][0]}'][idx_j, idx_i] = log_data[param][i_line][0]
+
+    # New line after the rustic progress bar
+    print()
+
+    # Recover coordinates from the wcs to store in the headers:
+    hdr_coords = extract_wcs_header(wcs, drop_axis='spectral')
+
+    # Save the parameter maps as individual fits files with one line per page
+    output_file_prefix = '' if output_file_prefix is None else output_file_prefix
+    for param in param_list:
+
+        # Primary header
+        paramHDUs = fits.HDUList()
+        paramHDUs.append(fits.PrimaryHDU())
+
+        # ImageHDU for the parameter maps
+        for line in line_list:
+
+            # Create page header with the default data
+            hdr_i = fits.Header()
+            hdr_i['LINE'] = (line, 'Line label')
+            hdr_i['PARAM'] = (param, 'LiMe parameter label')
+
+            # Add WCS information
+            if hdr_coords is not None:
+                hdr_i.update(hdr_coords)
+
+            # Add user information
+            if header is not None:
+                page_hdr = header.get(f'{param}-{line}', None)
+                page_hdr = header if page_hdr is None else page_hdr
+                hdr_i.update(page_hdr)
+
+            # Create page HDU entry
+            HDU_i = fits.ImageHDU(name=line, data=images_dict[f'{param}-{line}'], header=hdr_i, ver=1)
+            paramHDUs.append(HDU_i)
+
+        # Write to new file
+        output_file = Path(output_folder)/f'{output_file_prefix}{param}.fits'
+        paramHDUs.writeto(output_file, overwrite=True, output_verify='fix')
+
+    return
+
+
+def extract_wcs_header(wcs, drop_axis=None):
+
+    if wcs is not None:
+
+        # Remove 3rd dimensional axis if present
+        if drop_axis is not None:
+            if drop_axis == 'spectral':
+                input_wcs = wcs.dropaxis(2) if wcs.naxis == 3 else wcs
+            elif drop_axis == 'spatial':
+                if wcs.naxis == 3:
+                    input_wcs = wcs.dropaxis(1)
+                    input_wcs = wcs.dropaxis(0)
+            else:
+                raise LiMe_Error(f'Fits coordinates axis: "{drop_axis}" not recognized. Please use: "spectral" or'
+                                 f' "spatial"')
+
+        else:
+            input_wcs = wcs
+
+        # Convert to HDU header
+        hdr_coords = input_wcs.to_fits()[0].header
+
+    else:
+        hdr_coords = None
+
+    return hdr_coords
 
 class ProgressBar:
 
-    def __init__(self, message_type=None, count_type=""):
+    def __init__(self, message_type=None, count_type='bar'):
 
         self.output_message = None
         self.count_type = count_type
 
         if message_type is None:
             self.output_message = self.no_output
 
         if message_type == 'bar':
             self.output_message = self.progress_bar
 
-        if message_type == 'counter':
-            self.output_message = self.counter
-
         return
 
     def progress_bar(self, i, i_max, pre_text, post_text, n_bar=10):
 
         post_text = "" if post_text is None else post_text
 
         j = (i + 1) / i_max
         stdout.write('\r')
         message = f'[{"=" * int(n_bar * j):{n_bar}s}] {int(100 * j)}% of {self.count_type} {post_text}'
         stdout.write(message)
         stdout.flush()
 
         return
 
-    def counter(self, i, i_max, pre_text="", post_text="", n_bar=10):
-        print(f'{i + 1}/{self.count_type}) {post_text}')
-
-        return
-
     def no_output(self, i, i_max, pre_text, post_text, n_bar=10):
 
         return
```

### Comparing `lime-stable-0.9.99.1/src/lime/transitions.py` & `lime-stable-0.9.99.5/src/lime/transitions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import logging
 
 import numpy as np
 import pandas as pd
 from numpy import array, abs, all, diff, char, searchsorted, unique, empty, arange, zeros
 from .io import _PARENT_BANDS, _LOG_EXPORT, _LOG_COLUMNS, check_file_dataframe, LiMe_Error
 from pandas import DataFrame
+from .tools import pd_get, au
 
-
-UNITS_LATEX_DICT = {'A': r'\AA',
-                    'um': r'\mu\!m',
-                    'nm': 'nm',
-                    'Hz': 'Hz',
-                    'cm': 'cm',
-                    'mm': 'mm',
-                    'Flam': r'erg\,cm^{-2}s^{-1}\AA^{-1}',
-                    'Fnu': r'erg\,cm^{-2}s^{-1}\Hz^{-1}',
-                    'Jy': 'Jy',
-                    'mJy': 'mJy',
-                    'nJy': 'nJy'}
-
-# TODO need a new mechanic to get the units
-DISPERSION_UNITS = ('A', 'um', 'nm', 'Hz', 'cm', 'mm')
+# UNITS_LATEX_DICT = {'A': r'\AA',
+#                     'um': r'\mu\!m',
+#                     'nm': 'nm',
+#                     'Hz': 'Hz',
+#                     'cm': 'cm',
+#                     'mm': 'mm',
+#                     'Flam': r'erg\,cm^{-2}s^{-1}\AA^{-1}',
+#                     'Fnu': r'erg\,cm^{-2}s^{-1}\Hz^{-1}',
+#                     'Jy': 'Jy',
+#                     'mJy': 'mJy',
+#                     'nJy': 'nJy'}
+#
+# # TODO need a new mechanic to get the units
+# DISPERSION_UNITS = ('A', 'um', 'nm', 'Hz', 'cm', 'mm')
 
 # FLUX_DENSITY_UNITS = ('Flam', 'Fnu', 'Jy', 'mJy', 'nJy')
 
 
 _DEFAULT_PROFILE = 'g-emi'
 
 _logger = logging.getLogger('LiMe')
@@ -161,63 +161,85 @@
         output_array = np.core.defchararray.add(ion_array, '_')
         output_array = np.core.defchararray.add(output_array, vacuum_wave)
         output_array = np.core.defchararray.add(output_array, 'A')
 
     return output_array
 
 
-def check_units_from_wave(str_wave):
+def check_units_from_wave(line, str_ion, str_wave, lines_df):
+
+    # Try to recover from dataframe
+    if lines_df is not None:
+
+        # Check literal unit
+        wave = pd_get(lines_df, line, 'wavelength')
+        units = pd_get(lines_df, line, 'units_wave')
+
+        # Check core element
+        if wave is None:
+            core_element = f'{str_ion}_{str_wave}'
+            wave = pd_get(lines_df, core_element, 'wavelength')
+            units = pd_get(lines_df, core_element, 'units_wave')
+
+        # Convert to units
+        units = au.Unit(units) if units is not None else units
+
+    else:
+        wave, units = None, None
+
+    # Otherwise decipher from label
+    if (units is None) or (wave is None):
 
-    # One character unit
-    units = str_wave[-1] if str_wave[-1] in DISPERSION_UNITS else None
+        # First check for Angstroms
+        if str_wave[-1] == 'A':
+            units_label = au.Unit('AA')
+            wave_label = float(str_wave[:-1])
 
-    # Two characters unit
-    if units is None:
-        units = str_wave[-2:] if str_wave[-2:] in DISPERSION_UNITS else None
-
-        # Warning for an unsuccessful notation
-        if units is None:
-            _logger.warning(f'The units from the transition "{str_wave}" could not be interpreted')
-            wave = None
         else:
-            wave = float(str_wave[:-2])
+            au_unit = au.Unit(str_wave)
+            units_label = au_unit.bases[0]
+            wave_label = au_unit.scale
 
     else:
-        wave = float(str_wave[:-1])
+        units_label, wave_label = None, None
+
+    # Give preferences to the tabel values
+    wave = wave_label if wave is None else wave
+    units = units_label if units is None else units
 
     return wave, units
 
 
 def check_line_in_log(input_label, log=None, tol=1):
 
     # Guess the transition if only a wavelength provided
     if not isinstance(input_label, str):
 
         if log is not None:
 
             # Check the wavelength from the wave_obs column
-            if ('wave_obs' in log.columns) and ('units_wave' in log.columns): # TODO is this reading?
-                ref_waves = log.wave_obs.values
-                # units_wave = log.units_wave.values[0]
+            if 'wavelength' in log.columns:
+                ref_waves = log.wavelength.to_numpy()
+
 
             # Get it from the indexes
             else:
                 ion_array, ref_waves = zip(*log.index.str.split('_').to_numpy())
                 _wave0, units_wave = check_units_from_wave(ref_waves[0])
                 ref_waves = char.strip(ref_waves, units_wave).astype(float)
 
             # Check if table rows are not sorted
             if not all(diff(ref_waves) >= 0): # TODO we might need to use something else than searchsorted
                 _logger.warning(f'The lines log rows are not sorted from lower to higher wavelengths. This can cause '
                                 f'issues to identify the lines using the transition wavelength. Try to use the string '
                                 f'line label')
 
             # Locate the best candidate
-            idx_closest = searchsorted(ref_waves, input_label)
-            line_ion, line_wave = ion_array[idx_closest], ref_waves[idx_closest]
+            idx_closest = np.argmin(np.abs(ref_waves - input_label))
+            line_wave = ref_waves[idx_closest]
 
             # Check if input wavelength is close to the guessed line
             disc = abs(line_wave - input_label)
             if tol < disc < 1.5 * tol:
                 _logger.info(f'The input line {input_label} has been identified with {log.iloc[idx_closest].name}')
 
             if disc > 1.5 * tol:
@@ -258,15 +280,15 @@
 
     for i in arange(n_items):
 
         # Particle label
         part_label = particle_notation(particle[i], transition_comp[i])
 
         # Wavelength and units label
-        units_latex = UNITS_LATEX_DICT[units_wave[i]]
+        units_latex = f'{units_wave[i]:latex}'[9:-2]
 
         # Kinematic label
         kinetic_comp = '' if kinem[i] == 0 else f'-k_{kinem[i]}'
 
         # Combine items
         latex_array[i] = f'{part_label}{wave[i]}{units_latex}{kinetic_comp}$'
 
@@ -280,15 +302,15 @@
 
 def label_composition(line_list, ref_df=None, default_profile=None):
 
     # Empty containers for the label componentes
     n_comps = len(line_list)
     particle = [None] * n_comps #empty(n_comps).astype(str)
     wavelength = empty(n_comps)
-    units_wave = empty(n_comps).astype(str)
+    units_wave = [None] * n_comps
     kinem = zeros(n_comps, dtype=int)
     profile_comp = [None] * n_comps
     transition_comp = [None] * n_comps
 
     # If there isn't an input profile use LiMe default
     default_profile = _DEFAULT_PROFILE if default_profile is None else default_profile
 
@@ -303,15 +325,15 @@
                              f' recognised format. Please use a "Particle_WavelengthUnits" format in the configuration'
                              f'file')
 
         # Particle properties
         particle[i] = Particle.from_label(line_items[0])
 
         # Wavelength properties
-        wavelength[i], units_wave[i] = check_units_from_wave(line_items[1])
+        wavelength[i], units_wave[i] = check_units_from_wave(line, line_items[0], line_items[1], ref_df)
 
         # Split the optional components: "H1_1216A_t-rec_k-0_p-g" -> {'t': 'rec', 'k': '0', 'p': 'g'} # TODO better do that with optional_comps
         comp_conf = {optC[0]: optC[2:] for optC in line_items[2:]}
 
         # Check there are no accepted optional components
         for opt_key in comp_conf.keys():
             if opt_key != 'm' and opt_key != 'b':
@@ -327,16 +349,15 @@
             profile_comp[i] = default_profile
 
         # Transition component
         trans = comp_conf.get('t', None)
 
         # If none is provided check from the table
         if (trans is None) and (ref_df is not None):
-            if (line in ref_df.index) and ('transition' in ref_df.columns):
-                trans = ref_df.loc[line, 'transition']
+            trans = pd_get(ref_df, line, 'transition')
 
         # Else assume default
         if trans is None:
             trans = recover_transition(particle[i])
 
         transition_comp[i] = trans
 
@@ -397,16 +418,14 @@
 
     # If requested and single line, return the input as a scalar
     if scalar_output and (output[0].shape[0] == 1):
         output = tuple(item[0] for item in output)
     else:
         output = tuple(output)
 
-    # TODO should we output as single array only if one property is requested?
-
     return output
 
 
 def label_profiling(profile_comp, default_type='emi'):
 
     _p_type_list, _p_shape_list = [], []
     for prof_comp in profile_comp:
@@ -655,49 +674,35 @@
             elif modularity_label == 'm':
                 self.merged_check = True
 
             else:
                 raise LiMe_Error(f'The modularity component {modularity_label} in the input line "{self.label}" is not'
                                  f' recognized')
 
-        # Restore the group label from the log if provided
-        group_label = None
-        if bands_log is not None:
-            if isinstance(bands_log, pd.DataFrame):
-                try:
-                    group_label = bands_log.at[self.label, 'group_label']
-                except KeyError:
-                    group_label = None
-
-                # Check if we have a blended or merged line
-                if group_label is not None:
-                    if group_label != 'none':
-                        if self.merged_check is False:
-                            self.blended_check = True
-                    else:
-                        group_label = None
+        # Restore the group label if provided (Configuration file over rules log)
+        group_label_cfg = None if fit_conf is None else fit_conf.get(self.label, None)
+        group_label_frame = None if not isinstance(bands_log, pd.DataFrame) else pd_get(bands_log, self.label,
+                                                                                        'group_label', transform='none')
+
+        self.group_label = group_label_cfg if group_label_cfg is not None else group_label_frame
+
+        # Confirm blended or merged
+        self.blended_check = True if (self.group_label is not None) and (self.merged_check is False) else False
 
         # Recover the profile components
         if self.merged_check or self.blended_check:
 
-            # Check for profile label
-            # TODO check this fit_conf is nan
-            if group_label is None:
-                self.group_label = None if fit_conf is None else fit_conf.get(self.label, None)
-            else:
-                self.group_label = group_label
-
             # Reset and warned the line has a suffix but there are no components provided
             if self.group_label is None:
                 self.merged_check, self.blended_check = False, False
 
                 # Warning incase there is an input configuration but the line is not there
                 if fit_conf is not None:
                     _logger.warning(f'The {self.label} line has a "_{modularity_label}" suffix but not components were '
-                                    f'specified on the configuration:\n{fit_conf}')
+                                    f' on the lines frames or the input configuration the configuration:\n{fit_conf}')
 
         # List of components only for blended
         if (self.merged_check or self.blended_check) and (self.group_label is not None):
             self.list_comps = self.group_label.split('+') if self.blended_check else [self.label]
 
             # Check if there are repeated elements
             if len(self.list_comps) > 1:
```

### Comparing `lime-stable-0.9.99.1/src/lime/workflow.py` & `lime-stable-0.9.99.5/src/lime/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import numpy as np
 import pandas as pd
 from pathlib import Path
 from astropy.io import fits
 from time import time
 
 from .model import LineFitting, signal_to_noise_rola
-from .tools import define_masks, ProgressBar, logs_into_fits
+from .tools import define_masks, ProgressBar, logs_into_fits, extract_wcs_header, pd_get
 from .transitions import Line
-from .io import check_file_dataframe, check_file_array_mask, log_to_HDU, results_to_log, load_log, extract_wcs_header, LiMe_Error, check_fit_conf
+from .io import check_file_dataframe, check_file_array_mask, log_to_HDU, results_to_log, load_frame, LiMe_Error, check_fit_conf
 from lmfit.models import PolynomialModel
 
 _logger = logging.getLogger('LiMe')
 
 
 def review_bands(line, emis_wave, cont_wave, limit_narrow=7):
 
@@ -115,15 +115,14 @@
     else:
         _logger.warning(f'Line {line} was not found on the input bands database.')
         valid_check = False
 
     return valid_check
 
 
-
 def check_cube_bands(input_bands, mask_list, fit_cfg):
 
     if input_bands is None:
 
         # Recover the mask_configuration as a list
         for mask_name in mask_list:
 
@@ -175,24 +174,41 @@
             output_conf['line_detection'] = default_detect
         else:
             pass
 
     return output_conf
 
 
+def check_compound_line_exclusion(line, lines_df):
+
+    # Confirm the dataframe includes the group of lines
+    group_label = pd_get(lines_df, line, 'group_label', transform='none')
+
+    # Confirm if the line is in the group of lines
+    if group_label is not None:
+        comp_list = group_label.split('+')
+        measure_check = False if line in comp_list else True
+    else:
+        measure_check = True
+
+    return measure_check
+
+
 class SpecTreatment(LineFitting):
 
     def __init__(self, spectrum):
 
         # Instantiate the dependencies
         LineFitting.__init__(self)
 
         # Lime spectrum object with the scientific data
         self._spec = spectrum
         self.line = None
+        self._i_line = 0
+        self._n_lines = 0
 
     def bands(self, label, bands=None, fit_conf=None, min_method='least_squares', profile='g-emi', cont_from_bands=True,
               temp=10000.0, id_conf_prefix=None, default_conf_prefix='default'):
 
         """
 
         This function fits a line on the spectrum object from a given band.
@@ -274,15 +290,15 @@
             emisWave, emisFlux = self._spec.wave[idcsEmis], self._spec.flux[idcsEmis]
             emisErr = None if self._spec.err_flux is None else self._spec.err_flux[idcsEmis]
 
             contWave, contFlux = self._spec.wave[idcsCont], self._spec.flux[idcsCont]
             contErr = None if self._spec.err_flux is None else self._spec.err_flux[idcsCont]
 
             # Check the bands size
-            review_bands(self.line, emisWave, contWave) # TODO put this one in fit frame
+            review_bands(self.line, emisWave, contWave)
 
             # Default line type is in emission unless all are absorption
             emission_check = False if np.all(~self.line._p_type) else True
 
             # Non-parametric measurements
             self.integrated_properties(self.line, emisWave, emisFlux, emisErr, contWave, contFlux, contErr, emission_check)
 
@@ -394,50 +410,50 @@
 
             # Crop the analysis to the target lines
             if line_list is not None:
                 idcs = bands.index.isin(line_list)
                 bands = bands.loc[idcs]
 
             # Load configuration
-            # fit_conf = {} if fit_conf is None else fit_conf
-            # input_conf = recover_level_conf(fit_conf, id_conf_prefix, default_conf_prefix)
             input_conf = check_fit_conf(fit_conf, default_conf_prefix, id_conf_prefix)
 
             # Line detection if requested
             if line_detection:
                 detect_conf = input_conf.get('line_detection', {})
                 bands = self._spec.line_detection(bands, **detect_conf)
 
-            # Loop through the lines # TODO exclude (blended/kinematic) components, use the core elements...
+            # Define lines to treat through the lines
             label_list = bands.index.to_numpy()
-            bands_matrix = bands.loc[:, 'w1':'w6'].to_numpy()
-            n_lines = label_list.size
+            self._n_lines = label_list.size
 
             # Loop through the lines
-            if n_lines > 0:
+            if self._n_lines > 0:
 
                 # On screen progress bar
+                pbar = ProgressBar(progress_output, f'{self._n_lines} lines')
                 if progress_output is not None:
                     print(f'\nLine fitting progress:')
-                pbar = ProgressBar(progress_output, f'{n_lines} lines')
 
-                for i in np.arange(n_lines):
+                for self._i_line in np.arange(self._n_lines):
+
+                    # Ignore line if part of a blended/merge group
+                    line = label_list[self._i_line]
+                    measure_check = check_compound_line_exclusion(line, bands)
 
-                    # Current line
-                    line = label_list[i]
+                    if measure_check:
 
-                    # Progress message
-                    pbar.output_message(i, n_lines, pre_text="", post_text=f'({line})')
+                        # Progress message
+                        pbar.output_message(self._i_line, self._n_lines, pre_text="", post_text=f'({line})')
 
-                    # Fit the lines
-                    self.bands(line, bands_matrix[i], input_conf, min_method, profile, cont_from_bands, temp,
-                               id_conf_prefix=None, default_conf_prefix=None)
+                        # Fit the lines
+                        self.bands(line, bands, input_conf, min_method, profile, cont_from_bands, temp,
+                                   id_conf_prefix=None, default_conf_prefix=None)
 
-                    if plot_fit:
-                        self._spec.plot.bands()
+                        if plot_fit:
+                            self._spec.plot.bands()
 
             else:
                 msg = f'No lines were measured from the input dataframe:\n - line_list: {line_list}\n - line_detection: {line_detection}'
                 _logger.info(msg)
 
         else:
             _logger.info(f'Not input dataframe. Lines were not measured')
@@ -680,15 +696,15 @@
             # mask_conf = recover_level_conf(fit_conf, default_conf_prefix, mask_name)
             mask_conf = check_fit_conf(input_conf, default_conf_prefix, mask_name)
 
             # Load the mask log if provided
             if bands is None:
                 bands_file = mask_conf['bands']
                 bands_path = Path(bands_file).absolute() if bands_file[0] == '.' else Path(bands_file)
-                bands_in = load_log(bands_path)
+                bands_in = load_frame(bands_path)
             else:
                 bands_in = bands
 
             # Loop through the spaxels
             n_spaxels = idcs_spaxels.shape[0]
             n_lines, start_time = 0, time()
```

### Comparing `lime-stable-0.9.99.1/src/lime_stable.egg-info/PKG-INFO` & `lime-stable-0.9.99.5/src/lime_stable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lime-stable
-Version: 0.9.99.1
+Version: 0.9.99.5
 Summary: Line measuring algorithm for astronomical spectra
 Home-page: https://github.com/Vital-Fernandez/lime
 Author: Vital Fernandez
 Author-email: Vital Fernández <vgf@umich.edu>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `lime-stable-0.9.99.1/src/lime_stable.egg-info/SOURCES.txt` & `lime-stable-0.9.99.5/src/lime_stable.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 src/lime/recognition.py
 src/lime/tables.py
 src/lime/tools.py
 src/lime/transitions.py
 src/lime/workflow.py
 src/lime/resources/GradientDescent_v2_cost1_logNorm.joblib
 src/lime/resources/LogitistRegression_v2_cost1_logNorm.joblib
+src/lime/resources/adjust_bands_database.py
 src/lime/resources/parent_bands.txt
 src/lime/resources/parent_mask_v0.txt
 src/lime/resources/sketch.py
 src/lime/resources/types_params.txt
 src/lime/resources/types_params2.txt
 src/lime_stable.egg-info/PKG-INFO
 src/lime_stable.egg-info/SOURCES.txt
```

### Comparing `lime-stable-0.9.99.1/tests/test_astro.py` & `lime-stable-0.9.99.5/tests/test_astro.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import pandas as pd
 import lime
 
 def test_line_bands():
 
     log0 = lime.line_bands()
-    parent_bands = lime.load_log(lime._lines_database_path)
+    parent_bands = lime.load_frame(lime._lines_database_path)
 
     # TODO rework on the master database
     # assert np.all(log0.index == parent_bands.index)
     assert np.all(log0.columns == parent_bands.columns)
     # assert log0.equals(parent_bands)
 
     log1 = lime.line_bands(wave_intvl=(3000, 7000))
```

### Comparing `lime-stable-0.9.99.1/tests/test_cube.py` & `lime-stable-0.9.99.5/tests/test_cube.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,16 +112,16 @@
 
         cfg['MASK_0_line_fitting']['bands'] = bands_file_address.as_posix()
         cube.fit.spatial_mask(spatial_mask_address, fit_conf=cfg, line_detection=True, mask_list=['MASK_0'],
                               output_address=spatial_log_address)
 
         assert spatial_log_address.is_file()
 
-        spax_log = lime.load_log(spatial_log_address, page=f'{spaxel_label}_LINELOG')
-        orig_log = lime.load_log(lines_log_address)
+        spax_log = lime.load_frame(spatial_log_address, page=f'{spaxel_label}_LINELOG')
+        orig_log = lime.load_frame(lines_log_address)
 
         # Test 3 lines # TODO review these fluxes
         assert np.sum(spax_log.index.isin(['O3_5007A', 'O3_5007A_k-1', 'He1_5016A'])) == 3
         assert np.isclose(spax_log.loc['O3_5007A', 'profile_flux'], orig_log.loc['O3_5007A', 'profile_flux'])
         assert np.isclose(spax_log.loc['O3_5007A_k-1', 'profile_flux'], orig_log.loc['O3_5007A_k-1', 'profile_flux'])
         assert np.isclose(spax_log.loc['He1_5016A', 'profile_flux'], orig_log.loc['He1_5016A', 'profile_flux'])
 
@@ -175,15 +175,15 @@
 
         int_flux_map = fits.getdata(intg_flux_file, extname='O3_5007A')
         gauss_flux_map = fits.getdata(gauss_flux_file, extname='O3_5007A')
 
         assert np.isnan(int_flux_map).sum() == 5443
         assert np.isnan(gauss_flux_map).sum() == 5443
 
-        orig_log = lime.load_log(lines_log_address)
+        orig_log = lime.load_frame(lines_log_address)
 
         idx_j, idx_x = [int(item) for item in spaxel_label.split('-')]
 
         assert np.isclose(orig_log.loc['O3_5007A', 'intg_flux'], int_flux_map[idx_j, idx_x])
         assert np.isclose(orig_log.loc['O3_5007A', 'profile_flux'], gauss_flux_map[idx_j, idx_x])
 
         return
```

### Comparing `lime-stable-0.9.99.1/tests/test_io.py` & `lime-stable-0.9.99.5/tests/test_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     assert new_cfg['new_line_fitting']['He1_5016A_sigma']['max'] == 2.0
 
     return
 
 
 def test_log_parameters_calculation():
 
-    log_lines = lime.load_log(lines_log_address)
+    log_lines = lime.load_frame(lines_log_address)
     lime.extract_fluxes(log_lines, flux_type='profile')
 
     parameters = ['eqw_new', 'eqw_new_err']
 
     formulation = ['line_flux/cont', '(line_flux/cont) * sqrt((line_flux_err/line_flux)**2 + (cont_err/cont)**2)']
 
     lime.log_parameters_calculation(log_lines, parameters, formulation)
```

### Comparing `lime-stable-0.9.99.1/tests/test_line.py` & `lime-stable-0.9.99.5/tests/test_line.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 
     # Components configuration
     fit_conf = {'O3_5007A_b': 'O3_5007A+O3_5007A_k-1+He1_5016A',
                 'O3_5007A_m': 'O3_5007A+O3_5007A_k-1'}
 
     particle, wavelength, latex = label_decomposition('O3_5007A', fit_conf=fit_conf)
     assert particle[0] == 'O3'
-    assert wavelength[0] == 5007.0
-    assert latex[0] == r'$[OIII]5007\AA$'
+    assert wavelength[0] == 5006.7664
+    assert latex[0] == '$[OIII]5007\\mathring{A}$'
 
     particle, wavelength, latex = label_decomposition('O3_5007A_b', fit_conf=fit_conf)
     assert particle[0] == 'O3'
-    assert wavelength[0] == 5007.0
-    assert latex[0] == r'$[OIII]5007\AA$'
+    assert wavelength[0] ==  5006.7664
+    assert latex[0] == '$[OIII]5007\\mathring{A}$'
 
     particle, wavelength, latex = label_decomposition('O3_5007A_m', fit_conf=fit_conf)
     assert particle[0] == 'O3'
-    assert wavelength[0] == 5007.0
-    assert latex[0] == r'$[OIII]5007\AA$+$[OIII]5007\AA-k_1$'
+    assert wavelength[0] == 5006.7664
+    assert latex[0] == '$[OIII]5007\\mathring{A}$+$[OIII]5007\\mathring{A}-k_1$'
 
     return
 
 
 class TestLineClass:
 
     def test_single_merged_blended(self):
@@ -36,45 +36,45 @@
 
         # Default band O3_5007A
         O3_band = np.array([4971.796688, 4984.514249, 4995.348943, 5024.303156, 5027.74326, 5043.797081])
 
         line = Line('O3_5007A', fit_conf=fit_conf)
         assert line.particle[0].label == 'O3'
         assert line.particle[0].symbol == 'O', line.particle[0].ionization == 3
-        assert np.all(line.wavelength == np.array([5007.]))
+        assert np.all(line.wavelength == np.array([5006.7664]))
         assert np.all(line.kinem == np.array([0]))
         assert np.all(line.transition_comp == np.array(['col']))
         assert np.all(line.profile_comp == np.array(['g-emi']))
-        assert np.all(line.latex_label == np.array([r'$[OIII]5007\AA$']))
+        assert np.all(line.latex_label == np.array(['$[OIII]5007\mathring{A}$']))
         assert np.all(line.list_comps == ['O3_5007A'])
 
         assert line.label == 'O3_5007A'
         assert line.group_label is None
         assert np.all(line.mask == O3_band)
 
         line = Line('O3_5007A_b', band=None, fit_conf=fit_conf)
         assert np.all(line.particle == [Particle.from_label('O3'), Particle.from_label('O3'), Particle.from_label('He1')])
-        assert np.all(line.wavelength == np.array([5007., 5007., 5016.]))
+        assert np.all(line.wavelength == np.array([5006.7664, 5006.7664, 5016.]))
         assert np.all(line.kinem == np.array([0, 1, 0]))
         assert np.all(line.transition_comp == np.array(['col', 'col', 'rec']))
         assert np.all(line.profile_comp == np.array(['g-emi', 'g-emi', 'g-emi']))
-        assert np.all(line.latex_label == np.array([r'$[OIII]5007\AA$', r'$[OIII]5007\AA-k_1$', r'$HeI5016\AA$']))
+        assert np.all(line.latex_label == np.array(['$[OIII]5007\mathring{A}$', '$[OIII]5007\mathring{A}-k_1$', '$HeI5016\mathring{A}$']))
         assert np.all(line.list_comps == ['O3_5007A', 'O3_5007A_k-1', 'He1_5016A'])
 
         assert line.label == 'O3_5007A_b'
         assert line.group_label == 'O3_5007A+O3_5007A_k-1+He1_5016A'
         assert np.all(line.mask == O3_band)
 
         line = Line('O3_5007A_m', band=np.array([1, 2, 3, 4, 5, 6]), fit_conf=fit_conf)
         assert np.all(line.particle == [Particle('O3', symbol='O', ionization=3)])
         assert np.all(line.wavelength == np.array([5007]))
         assert np.all(line.kinem == np.array([0]))
         assert np.all(line.transition_comp == np.array(['col']))
         assert np.all(line.profile_comp == np.array(['g-emi', 'g-emi']))
-        assert np.all(line.latex_label == np.array([r'$[OIII]5007\AA$+$[OIII]5007\AA-k_1$']))
+        assert np.all(line.latex_label == np.array([r'$[OIII]5007\mathring{A}$+$[OIII]5007\mathring{A}-k_1$']))
         assert np.all(line.list_comps == ['O3_5007A_m'])
 
         assert line.label == 'O3_5007A_m'
         assert line.group_label == 'O3_5007A+O3_5007A_k-1'
         assert np.all(line.mask == np.array([1, 2, 3, 4, 5, 6]))
 
         return
@@ -83,80 +83,80 @@
 
         line = Line('OIII_5007A')
         assert line.particle[0].label == 'OIII'
         assert np.all(line.wavelength == np.array([5007.]))
         assert np.all(line.kinem == np.array([0]))
         assert np.all(line.transition_comp == [None])
         assert np.all(line.profile_comp == np.array(['g-emi']))
-        assert np.all(line.latex_label == np.array([r'OIII-$5007\AA$']))
+        assert np.all(line.latex_label == np.array(['OIII-$5007\\mathring{A}$']))
         assert np.all(line.list_comps == ['OIII_5007A'])
 
         assert line.label == 'OIII_5007A'
         assert line.group_label is None
         assert line.mask is None
 
         line = Line('Halpha_6563A')
         assert line.particle[0].label == 'Halpha'
         assert np.all(line.wavelength == np.array([6563.]))
         assert np.all(line.kinem == np.array([0]))
         assert np.all(line.transition_comp == [None])
         assert np.all(line.profile_comp == np.array(['g-emi']))
-        assert np.all(line.latex_label == np.array([r'Halpha-$6563\AA$']))
+        assert np.all(line.latex_label == np.array(['Halpha-$6563\\mathring{A}$']))
         assert np.all(line.list_comps == ['Halpha_6563A'])
 
         assert line.label == 'Halpha_6563A'
         assert line.group_label is None
         assert line.mask is None
 
         line = Line('HIPas4-3_18751A')
         assert line.particle[0].label == 'HIPas4-3'
         assert np.all(line.wavelength == np.array([18751.]))
         assert np.all(line.kinem == np.array([0]))
         assert np.all(line.transition_comp == [None])
         assert np.all(line.profile_comp == np.array(['g-emi']))
-        assert np.all(line.latex_label == np.array([r'HIPas4-3-$18751\AA$']))
+        assert np.all(line.latex_label == np.array(['HIPas4-3-$18751\\mathring{A}$']))
         assert np.all(line.list_comps == ['HIPas4-3_18751A'])
 
         assert line.label == 'HIPas4-3_18751A'
         assert line.group_label is None
         assert line.mask is None
 
         line = Line('OIII_5007A')
         assert line.particle[0].label == 'OIII'
         assert np.all(line.wavelength == np.array([5007.]))
         assert np.all(line.kinem == np.array([0]))
         assert np.all(line.transition_comp == [None])
         assert np.all(line.profile_comp == np.array(['g-emi']))
-        assert np.all(line.latex_label == np.array([r'OIII-$5007\AA$']))
+        assert np.all(line.latex_label == np.array(['OIII-$5007\\mathring{A}$']))
         assert np.all(line.list_comps == ['OIII_5007A'])
 
         assert line.label == 'OIII_5007A'
         assert line.group_label is None
         assert line.mask is None
 
         line = Line('C3_1909A')
         assert line.particle[0].label == 'C3'
-        assert np.all(line.wavelength == np.array([1909.]))
+        assert np.all(line.wavelength == np.array([1908.0803]))
         assert np.all(line.kinem == np.array([0]))
         assert np.all(line.transition_comp == ['sem'])
         assert np.all(line.profile_comp == np.array(['g-emi']))
-        assert np.all(line.latex_label == np.array([r'$CIII]1909\AA$']))
+        assert np.all(line.latex_label == np.array(['$CIII]1909\\mathring{A}$']))
         assert np.all(line.list_comps == ['C3_1909A'])
 
         assert line.label == 'C3_1909A'
         assert line.group_label is None
         assert line.mask is not None
 
         line = Line('C3_1909A_t-sem', band=None)
         assert line.particle[0].label == 'C3'
-        assert np.all(line.wavelength == np.array([1909.]))
+        assert np.all(line.wavelength == np.array([1908.0803]))
         assert np.all(line.kinem == np.array([0]))
         assert np.all(line.transition_comp == ['sem'])
         assert np.all(line.profile_comp == np.array(['g-emi']))
-        assert np.all(line.latex_label == np.array([r'$CIII]1909\AA$']))
+        assert np.all(line.latex_label == np.array(['$CIII]1908\\mathring{A}$']))
         assert np.all(line.list_comps == ['C3_1909A_t-sem'])
 
         assert line.label == 'C3_1909A_t-sem'
         assert line.group_label is None
         assert np.all(line.mask == np.array([1870., 1895., 1898.18782, 1912.243544, 1930., 1950.]))
 
         return
```

### Comparing `lime-stable-0.9.99.1/tests/test_model.py` & `lime-stable-0.9.99.5/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `lime-stable-0.9.99.1/tests/test_read_fits.py` & `lime-stable-0.9.99.5/tests/test_read_fits.py`

 * *Files identical despite different names*

### Comparing `lime-stable-0.9.99.1/tests/test_sample.py` & `lime-stable-0.9.99.5/tests/test_sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 
 
 baseline_folder = Path(__file__).parent / 'baseline'
 outputs_folder = Path(__file__).parent / 'outputs'
 lines_log_address = baseline_folder / 'manga_lines_log.txt'
 
 # Data for the tests
-lines_log = lime.load_log(lines_log_address)
+lines_log = lime.load_frame(lines_log_address)
 
 
 class TestSampleClass:
 
     def test_from_sample_creation(self):
 
         sample1 = lime.Sample.from_file(id_list=['spec1', 'spec2'],
                                         log_list=[lines_log_address, lines_log_address],
                                         file_list=['spec1.fits', 'spec2.fits'],
                                         instrument='isis')
-        sample1.save_log(outputs_folder / f'sample1_3indeces.txt')
+        sample1.save_frame(outputs_folder / f'sample1_3indeces.txt')
 
         assert list(sample1.log.index.names) == ['id', 'file', 'line']
 
         sample2 = lime.Sample.from_file(id_list=['spec1', 'spec2'], log_list=[lines_log_address, lines_log_address],
                                         instrument='isis')
-        sample2.save_log(outputs_folder / f'sample1_2indeces.txt')
+        sample2.save_frame(outputs_folder / f'sample1_2indeces.txt')
         assert list(sample2.log.index.names) == ['id', 'line']
 
         sample3 = lime.Sample(outputs_folder / f'sample1_3indeces.txt', instrument='isis')
         sample4 = lime.Sample(outputs_folder / f'sample1_2indeces.txt', levels=['id', 'line'], instrument='isis')
 
         assert list(sample3.log.index.names) == ['id', 'file', 'line']
         assert list(sample4.log.index.names) == ['id', 'line']
```

### Comparing `lime-stable-0.9.99.1/tests/test_spectrum.py` & `lime-stable-0.9.99.5/tests/test_spectrum.py`

 * *Files 6% similar despite different names*

```diff
@@ -196,54 +196,54 @@
         spec.plot.velocity_profile('O3_5007A', in_fig=fig)
 
         return fig
 
     def test_measurements_txt_file(self):
 
         extension = 'txt'
-        spec.save_log(outputs_folder / f'test_lines_log.{extension}')
+        spec.save_frame(outputs_folder / f'test_lines_log.{extension}')
 
-        log_orig = lime.load_log(lines_log_address)
-        log_test = lime.load_log(outputs_folder / f'test_lines_log.{extension}')
+        log_orig = lime.load_frame(lines_log_address)
+        log_test = lime.load_frame(outputs_folder / f'test_lines_log.{extension}')
 
         measurement_tolerance_test(spec, log_orig, log_test)
 
         return
 
     def test_measurements_fits_file(self):
 
         extension = 'fits'
-        spec.save_log(outputs_folder / f'test_lines_log.{extension}')
+        spec.save_frame(outputs_folder / f'test_lines_log.{extension}')
 
-        log_orig = lime.load_log(lines_log_address)
-        log_test = lime.load_log(outputs_folder / f'test_lines_log.{extension}')
+        log_orig = lime.load_frame(lines_log_address)
+        log_test = lime.load_frame(outputs_folder / f'test_lines_log.{extension}')
 
         measurement_tolerance_test(spec, log_orig, log_test)
 
         return
 
     def test_measurements_csv_file(self):
 
         extension = 'csv'
-        spec.save_log(outputs_folder / f'test_lines_log.{extension}')
+        spec.save_frame(outputs_folder / f'test_lines_log.{extension}')
 
-        log_orig = lime.load_log(lines_log_address)
-        log_test = lime.load_log(outputs_folder / f'test_lines_log.{extension}')
+        log_orig = lime.load_frame(lines_log_address)
+        log_test = lime.load_frame(outputs_folder / f'test_lines_log.{extension}')
 
         measurement_tolerance_test(spec, log_orig, log_test)
 
         return
 
     def test_measurements_xlsx_file(self):
 
         extension = 'xlsx'
-        spec.save_log(outputs_folder / f'test_lines_log.{extension}')
+        spec.save_frame(outputs_folder / f'test_lines_log.{extension}')
 
-        log_orig = lime.load_log(lines_log_address)
-        log_test = lime.load_log(outputs_folder / f'test_lines_log.{extension}')
+        log_orig = lime.load_frame(lines_log_address)
+        log_test = lime.load_frame(outputs_folder / f'test_lines_log.{extension}')
 
         measurement_tolerance_test(spec, log_orig, log_test)
 
         return
 
     def test_extra_pages_xlsx(self):
 
@@ -252,19 +252,19 @@
         if file_xlsx.is_file():
             try:
                 remove(file_xlsx)
                 print(f"File '{file_xlsx}' has been deleted successfully.")
             except OSError as e:
                 print(f"Error: {e.strerror}")
 
-        log_orig = lime.load_log(lines_log_address)
+        log_orig = lime.load_frame(lines_log_address)
 
         for page in ['LINELOG', 'LINESLOG2', 'LINELOG']:
-            spec.save_log(outputs_folder / file_xlsx, page=page)
-            log_test = lime.load_log(file_xlsx)
+            spec.save_frame(outputs_folder / file_xlsx, page=page)
+            log_test = lime.load_frame(file_xlsx)
 
             measurement_tolerance_test(spec, log_orig, log_test)
 
         return
 
     # def test_measurements_asdf_file(self):
     #
@@ -297,15 +297,15 @@
     #     return
 
     def test_save_load_log(self):
 
         spec0 = lime.Spectrum(wave_array, flux_array, err_array, redshift=redshift, norm_flux=norm_flux,
                              pixel_mask=pixel_mask)
 
-        spec0.load_log(lines_log_address)
+        spec0.load_frame(lines_log_address)
 
         new_log_spectrum = outputs_folder / 'manga_lines_log_from_spectrum.txt'
-        spec0.save_log(new_log_spectrum)
+        spec0.save_frame(new_log_spectrum)
 
         assert new_log_spectrum.is_file()
 
         return
```

### Comparing `lime-stable-0.9.99.1/tests/test_tools.py` & `lime-stable-0.9.99.5/tests/test_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Data for the tests
 baseline_folder = Path(__file__).parent / 'baseline'
 outputs_folder = Path(__file__).parent / 'outputs'
 
 file_address = baseline_folder/'manga_spaxel.txt'
 lines_log_address = baseline_folder/'manga_lines_log.txt'
-lines_log = lime.load_log(lines_log_address)
+lines_log = lime.load_frame(lines_log_address)
 redshift = 0.0475
 norm_flux = 1e-17
 wave_array, flux_array, err_array = np.loadtxt(file_address, unpack=True)
 pixel_mask = np.isnan(err_array)
 
 spec = lime.Spectrum(wave_array, flux_array, err_array, redshift=redshift, norm_flux=norm_flux,
                      pixel_mask=pixel_mask)
@@ -258,20 +258,20 @@
 
     return
 
 
 def test_logs_into_fits():
 
     # Load existing log
-    log_orig = lime.load_log(lines_log_address)
+    log_orig = lime.load_frame(lines_log_address)
 
     # New text file
-    lime.save_log(log_orig, outputs_folder/f'log_1.txt')
-    lime.save_log(log_orig, outputs_folder/f'log_2.fits', page='LOG2')
-    lime.save_log(log_orig, outputs_folder/f'log_2.fits', page='LOG3')
+    lime.save_frame(outputs_folder / f'log_1.txt', log_orig)
+    lime.save_frame(outputs_folder / f'log_2.fits', log_orig, page='LOG2')
+    lime.save_frame(outputs_folder / f'log_2.fits', log_orig, page='LOG3')
 
     file_list = [outputs_folder/f'log_1.txt', outputs_folder/f'log_2.fits']
     output_file = outputs_folder/'joined_log.fits'
 
     logs_into_fits(file_list, output_file, delete_after_join=True)
 
     # Check new and deteled files
```

