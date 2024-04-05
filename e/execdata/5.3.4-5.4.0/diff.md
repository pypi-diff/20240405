# Comparing `tmp/execdata-5.3.4.tar.gz` & `tmp/execdata-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "execdata-5.3.4.tar", last modified: Thu Apr  4 22:01:12 2024, max compression
+gzip compressed data, was "execdata-5.4.0.tar", last modified: Fri Apr  5 15:06:03 2024, max compression
```

## Comparing `execdata-5.3.4.tar` & `execdata-5.4.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:01:12.854395 execdata-5.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-04 22:01:06.000000 execdata-5.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-04 22:01:12.854395 execdata-5.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-04 22:01:06.000000 execdata-5.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:01:12.850396 execdata-5.3.4/execdata/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-04 22:01:06.000000 execdata-5.3.4/execdata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:01:12.854395 execdata-5.3.4/execdata/eda/
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-04 22:01:06.000000 execdata-5.3.4/execdata/eda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-04 22:01:06.000000 execdata-5.3.4/execdata/eda/_data_mining.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-04 22:01:06.000000 execdata-5.3.4/execdata/eda/_data_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-04 22:01:06.000000 execdata-5.3.4/execdata/eda/_feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-04 22:01:06.000000 execdata-5.3.4/execdata/eda/_standardization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:01:12.854395 execdata-5.3.4/execdata/format/
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-04 22:01:06.000000 execdata-5.3.4/execdata/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-04 22:01:06.000000 execdata-5.3.4/execdata/format/_data_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-04 22:01:06.000000 execdata-5.3.4/execdata/format/_format_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:01:12.854395 execdata-5.3.4/execdata/graph/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-04 22:01:06.000000 execdata-5.3.4/execdata/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-04 22:01:06.000000 execdata-5.3.4/execdata/graph/_data_analysis_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-04 22:01:06.000000 execdata-5.3.4/execdata/graph/_data_mining_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-04 22:01:06.000000 execdata-5.3.4/execdata/graph/_linear_regression_type_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 22:01:06.000000 execdata-5.3.4/execdata/graph/_logistic_regression_type_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:01:12.854395 execdata-5.3.4/execdata/model/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-04 22:01:06.000000 execdata-5.3.4/execdata/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-04 22:01:06.000000 execdata-5.3.4/execdata/model/_model_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-04 22:01:06.000000 execdata-5.3.4/execdata/model/_regression_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:01:12.854395 execdata-5.3.4/execdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-04 22:01:12.000000 execdata-5.3.4/execdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-04 22:01:12.000000 execdata-5.3.4/execdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 22:01:12.000000 execdata-5.3.4/execdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 22:01:12.000000 execdata-5.3.4/execdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-04 22:01:06.000000 execdata-5.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 22:01:12.854395 execdata-5.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-04 22:01:06.000000 execdata-5.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:06:03.198979 execdata-5.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-05 15:05:59.000000 execdata-5.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-05 15:06:03.198979 execdata-5.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-05 15:05:59.000000 execdata-5.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:06:03.194979 execdata-5.4.0/execdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:06:03.198979 execdata-5.4.0/execdata/eda/
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/eda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/eda/_data_mining.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/eda/_data_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/eda/_feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/eda/_standardization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:06:03.198979 execdata-5.4.0/execdata/format/
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/format/_data_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/format/_format_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:06:03.198979 execdata-5.4.0/execdata/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/graph/_data_analysis_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/graph/_data_mining_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/graph/_linear_regression_type_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/graph/_logistic_regression_type_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:06:03.198979 execdata-5.4.0/execdata/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/model/_model_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/model/_regression_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:06:03.198979 execdata-5.4.0/execdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-05 15:06:03.000000 execdata-5.4.0/execdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-05 15:06:03.000000 execdata-5.4.0/execdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:06:03.000000 execdata-5.4.0/execdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 15:06:03.000000 execdata-5.4.0/execdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-05 15:05:59.000000 execdata-5.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 15:06:03.198979 execdata-5.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-05 15:05:59.000000 execdata-5.4.0/setup.py
```

### Comparing `execdata-5.3.4/LICENSE` & `execdata-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `execdata-5.3.4/PKG-INFO` & `execdata-5.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: execdata
-Version: 5.3.4
+Version: 5.4.0
 Summary: Preprocessing dataset
 Home-page: https://github.com/bdfd
 Author: BDFD
 Author-email: bdfd2005@gmail.com
 Project-URL: Bug Tracker, https://github.com/bdfd
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `execdata-5.3.4/README.md` & `execdata-5.4.0/README.md`

 * *Files identical despite different names*

### Comparing `execdata-5.3.4/execdata/__init__.py` & `execdata-5.4.0/execdata/__init__.py`

 * *Files identical despite different names*

### Comparing `execdata-5.3.4/execdata/eda/__init__.py` & `execdata-5.4.0/execdata/eda/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 '''
 Date         : 2023-11-02 17:34:28
 Author       : BDFD,bdfd2005@gmail.com
 Github       : https://github.com/bdfd
-LastEditTime : 2024-04-04 17:51:44
+LastEditTime : 2024-04-05 10:53:42
 LastEditors  : <BDFD>
 Description  : 
 FilePath     : \execdata\eda\__init__.py
 Copyright (c) 2023 by BDFD, All Rights Reserved. 
 '''
 from ._data_mining import high_miss_rate_column
 from ._data_mining import numerical_features_list
-from ._data_mining import discrete_numerical_feature_list 
+from ._data_mining import categorical_numerical_feature_list 
 from ._data_mining import continuous_numerical_feature_list
 from ._data_mining import categorical_features_list
 from ._data_mining import column_identify
 from ._data_mining import filtered_value_count
 from ._data_mining import filtered_value_list
 from ._data_mining import majority_target_variable
 # from ._data_mining import filtered_value_list
```

### Comparing `execdata-5.3.4/execdata/eda/_data_mining.py` & `execdata-5.4.0/execdata/eda/_data_mining.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Date         : 2023-10-12 14:56:26
 Author       : BDFD,bdfd2005@gmail.com
 Github       : https://github.com/bdfd
-LastEditTime : 2024-04-04 17:53:32
+LastEditTime : 2024-04-05 10:51:09
 LastEditors  : <BDFD>
 Description  : 
 FilePath     : \execdata\eda\_data_mining.py
 Copyright (c) 2023 by BDFD, All Rights Reserved. 
 '''
 import numpy as np
 import pandas as pd
@@ -26,19 +26,19 @@
     print('Number of Numerical Variables:', len(numerical_features_list))
 
     # visualize the numerical variables
     print(df[numerical_features_list].head())
     print(numerical_features_list)
     return numerical_features_list
 
-def discrete_numerical_feature_list(df, numerical_features_list):
-    discrete_numerical_feature_list = [
+def categorical_numerical_feature_list(df, numerical_features_list):
+    categorical_numerical_feature_list = [
             feature for feature in numerical_features_list if len(df[feature].unique()) < 15]
-    print(discrete_numerical_feature_list)
-    return discrete_numerical_feature_list
+    print(categorical_numerical_feature_list)
+    return categorical_numerical_feature_list
 
 def continuous_numerical_feature_list(df, numerical_features_list):
     continuous_numerical_feature_list = [
             feature for feature in numerical_features_list if len(df[feature].unique()) >= 15]
     print(continuous_numerical_feature_list)
     return continuous_numerical_feature_list
```

### Comparing `execdata-5.3.4/execdata/eda/_data_preprocess.py` & `execdata-5.4.0/execdata/eda/_data_preprocess.py`

 * *Files identical despite different names*

### Comparing `execdata-5.3.4/execdata/eda/_feature_selection.py` & `execdata-5.4.0/execdata/eda/_feature_selection.py`

 * *Files identical despite different names*

### Comparing `execdata-5.3.4/execdata/eda/_standardization.py` & `execdata-5.4.0/execdata/eda/_standardization.py`

 * *Files identical despite different names*

### Comparing `execdata-5.3.4/execdata/format/_data_conversion.py` & `execdata-5.4.0/execdata/format/_data_conversion.py`

 * *Files identical despite different names*

### Comparing `execdata-5.3.4/execdata/format/_format_data.py` & `execdata-5.4.0/execdata/format/_format_data.py`

 * *Files identical despite different names*

### Comparing `execdata-5.3.4/execdata/graph/_data_mining_graph.py` & `execdata-5.4.0/execdata/graph/_data_mining_graph.py`

 * *Files identical despite different names*

### Comparing `execdata-5.3.4/execdata/graph/_linear_regression_type_graph.py` & `execdata-5.4.0/execdata/graph/_linear_regression_type_graph.py`

 * *Files identical despite different names*

### Comparing `execdata-5.3.4/execdata/model/_model_evaluate.py` & `execdata-5.4.0/execdata/model/_model_evaluate.py`

 * *Files identical despite different names*

### Comparing `execdata-5.3.4/execdata/model/_regression_model.py` & `execdata-5.4.0/execdata/model/_regression_model.py`

 * *Files identical despite different names*

### Comparing `execdata-5.3.4/execdata.egg-info/PKG-INFO` & `execdata-5.4.0/execdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: execdata
-Version: 5.3.4
+Version: 5.4.0
 Summary: Preprocessing dataset
 Home-page: https://github.com/bdfd
 Author: BDFD
 Author-email: bdfd2005@gmail.com
 Project-URL: Bug Tracker, https://github.com/bdfd
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `execdata-5.3.4/execdata.egg-info/SOURCES.txt` & `execdata-5.4.0/execdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `execdata-5.3.4/setup.py` & `execdata-5.4.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 '''
 Date         : 2022-10-25 15:44:41
 Author       : BDFD,bdfd2005@gmail.com
 Github       : https://github.com/bdfd
-LastEditTime : 2024-04-04 17:58:20
+LastEditTime : 2024-04-05 11:03:49
 LastEditors  : <BDFD>
 Description  : 
 FilePath     : \setup.py
 Copyright (c) 2022 by BDFD, All Rights Reserved. 
 '''
 from setuptools import setup, find_packages
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-VERSION = '5.3.4'
+VERSION = '5.4.0'
 DESCRIPTION = 'Preprocessing dataset'
 PACKAGE_NAME = 'execdata'
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     author="BDFD",
```

