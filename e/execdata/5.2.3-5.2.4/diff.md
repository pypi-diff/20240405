# Comparing `tmp/execdata-5.2.3.tar.gz` & `tmp/execdata-5.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "execdata-5.2.3.tar", last modified: Thu Apr  4 20:31:23 2024, max compression
+gzip compressed data, was "execdata-5.2.4.tar", last modified: Thu Apr  4 20:51:34 2024, max compression
```

## Comparing `execdata-5.2.3.tar` & `execdata-5.2.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:31:23.463508 execdata-5.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-04 20:31:19.000000 execdata-5.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-04 20:31:23.459508 execdata-5.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-04 20:31:19.000000 execdata-5.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:31:23.459508 execdata-5.2.3/execdata/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:31:23.459508 execdata-5.2.3/execdata/eda/
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/eda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/eda/_data_mining.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/eda/_data_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/eda/_feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/eda/_standardization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:31:23.459508 execdata-5.2.3/execdata/format/
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/format/_data_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/format/_format_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:31:23.459508 execdata-5.2.3/execdata/graph/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/graph/_data_analysis_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/graph/_data_mining_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/graph/_linear_regression_type_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/graph/_logistic_regression_type_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:31:23.459508 execdata-5.2.3/execdata/model/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/model/_model_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/model/_regression_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:31:23.459508 execdata-5.2.3/execdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-04 20:31:23.000000 execdata-5.2.3/execdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-04 20:31:23.000000 execdata-5.2.3/execdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 20:31:23.000000 execdata-5.2.3/execdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 20:31:23.000000 execdata-5.2.3/execdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-04 20:31:19.000000 execdata-5.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 20:31:23.463508 execdata-5.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-04 20:31:19.000000 execdata-5.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:51:34.379556 execdata-5.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-04 20:51:30.000000 execdata-5.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-04 20:51:34.379556 execdata-5.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-04 20:51:30.000000 execdata-5.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:51:34.375556 execdata-5.2.4/execdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-04 20:51:30.000000 execdata-5.2.4/execdata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:51:34.375556 execdata-5.2.4/execdata/eda/
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-04 20:51:30.000000 execdata-5.2.4/execdata/eda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-04-04 20:51:30.000000 execdata-5.2.4/execdata/eda/_data_mining.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-04 20:51:30.000000 execdata-5.2.4/execdata/eda/_data_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-04 20:51:30.000000 execdata-5.2.4/execdata/eda/_feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-04 20:51:30.000000 execdata-5.2.4/execdata/eda/_standardization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:51:34.375556 execdata-5.2.4/execdata/format/
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-04 20:51:30.000000 execdata-5.2.4/execdata/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-04 20:51:30.000000 execdata-5.2.4/execdata/format/_data_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-04 20:51:30.000000 execdata-5.2.4/execdata/format/_format_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:51:34.375556 execdata-5.2.4/execdata/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-04 20:51:30.000000 execdata-5.2.4/execdata/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-04 20:51:30.000000 execdata-5.2.4/execdata/graph/_data_analysis_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-04 20:51:30.000000 execdata-5.2.4/execdata/graph/_data_mining_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-04 20:51:30.000000 execdata-5.2.4/execdata/graph/_linear_regression_type_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:51:30.000000 execdata-5.2.4/execdata/graph/_logistic_regression_type_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:51:34.375556 execdata-5.2.4/execdata/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-04 20:51:30.000000 execdata-5.2.4/execdata/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-04 20:51:30.000000 execdata-5.2.4/execdata/model/_model_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-04 20:51:30.000000 execdata-5.2.4/execdata/model/_regression_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:51:34.375556 execdata-5.2.4/execdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-04 20:51:34.000000 execdata-5.2.4/execdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-04 20:51:34.000000 execdata-5.2.4/execdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 20:51:34.000000 execdata-5.2.4/execdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 20:51:34.000000 execdata-5.2.4/execdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-04 20:51:30.000000 execdata-5.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 20:51:34.379556 execdata-5.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-04 20:51:30.000000 execdata-5.2.4/setup.py
```

### Comparing `execdata-5.2.3/LICENSE` & `execdata-5.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `execdata-5.2.3/PKG-INFO` & `execdata-5.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: execdata
-Version: 5.2.3
+Version: 5.2.4
 Summary: Preprocessing dataset
 Home-page: https://github.com/bdfd
 Author: BDFD
 Author-email: bdfd2005@gmail.com
 Project-URL: Bug Tracker, https://github.com/bdfd
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `execdata-5.2.3/README.md` & `execdata-5.2.4/README.md`

 * *Files identical despite different names*

### Comparing `execdata-5.2.3/execdata/__init__.py` & `execdata-5.2.4/execdata/__init__.py`

 * *Files identical despite different names*

### Comparing `execdata-5.2.3/execdata/eda/__init__.py` & `execdata-5.2.4/execdata/eda/__init__.py`

 * *Files identical despite different names*

### Comparing `execdata-5.2.3/execdata/eda/_data_mining.py` & `execdata-5.2.4/execdata/eda/_data_mining.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Date         : 2023-10-12 14:56:26
 Author       : BDFD,bdfd2005@gmail.com
 Github       : https://github.com/bdfd
-LastEditTime : 2024-04-04 16:28:24
+LastEditTime : 2024-04-04 16:49:45
 LastEditors  : <BDFD>
 Description  : 
 FilePath     : \execdata\eda\_data_mining.py
 Copyright (c) 2023 by BDFD, All Rights Reserved. 
 '''
 import numpy as np
 import pandas as pd
@@ -38,18 +38,18 @@
 
     # visualize the categorical variables
     print(df[categorical_features_list].head())
     return categorical_features_list
 
 
 def column_identify(df, column_lists):
-    column_indentify = {}
+    column_indentify_dict = {}
     for col in column_lists:
-        num = len(df[col].unique().tolist())
-        column_indentify[col] = num
+        column_indentify_dict[col] = df[col].value_counts().shape[0]
+    column_indentify = pd.DataFrame(column_indentify_dict,index=["Unique Count"]).transpose()
     return column_indentify
 
 
 def filtered_value_count(df, column, limit_number=10):
     '''
     用于过滤当前column每个种类少于10个分类
     '''
```

### Comparing `execdata-5.2.3/execdata/eda/_data_preprocess.py` & `execdata-5.2.4/execdata/eda/_data_preprocess.py`

 * *Files identical despite different names*

### Comparing `execdata-5.2.3/execdata/eda/_feature_selection.py` & `execdata-5.2.4/execdata/eda/_feature_selection.py`

 * *Files identical despite different names*

### Comparing `execdata-5.2.3/execdata/eda/_standardization.py` & `execdata-5.2.4/execdata/eda/_standardization.py`

 * *Files identical despite different names*

### Comparing `execdata-5.2.3/execdata/format/_data_conversion.py` & `execdata-5.2.4/execdata/format/_data_conversion.py`

 * *Files identical despite different names*

### Comparing `execdata-5.2.3/execdata/format/_format_data.py` & `execdata-5.2.4/execdata/format/_format_data.py`

 * *Files identical despite different names*

### Comparing `execdata-5.2.3/execdata/graph/_data_analysis_graph.py` & `execdata-5.2.4/execdata/graph/_data_analysis_graph.py`

 * *Files identical despite different names*

### Comparing `execdata-5.2.3/execdata/graph/_data_mining_graph.py` & `execdata-5.2.4/execdata/graph/_data_mining_graph.py`

 * *Files identical despite different names*

### Comparing `execdata-5.2.3/execdata/graph/_linear_regression_type_graph.py` & `execdata-5.2.4/execdata/graph/_linear_regression_type_graph.py`

 * *Files identical despite different names*

### Comparing `execdata-5.2.3/execdata/model/_model_evaluate.py` & `execdata-5.2.4/execdata/model/_model_evaluate.py`

 * *Files identical despite different names*

### Comparing `execdata-5.2.3/execdata/model/_regression_model.py` & `execdata-5.2.4/execdata/model/_regression_model.py`

 * *Files identical despite different names*

### Comparing `execdata-5.2.3/execdata.egg-info/PKG-INFO` & `execdata-5.2.4/execdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: execdata
-Version: 5.2.3
+Version: 5.2.4
 Summary: Preprocessing dataset
 Home-page: https://github.com/bdfd
 Author: BDFD
 Author-email: bdfd2005@gmail.com
 Project-URL: Bug Tracker, https://github.com/bdfd
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `execdata-5.2.3/execdata.egg-info/SOURCES.txt` & `execdata-5.2.4/execdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `execdata-5.2.3/setup.py` & `execdata-5.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 '''
 Date         : 2022-10-25 15:44:41
 Author       : BDFD,bdfd2005@gmail.com
 Github       : https://github.com/bdfd
-LastEditTime : 2024-04-04 16:30:04
+LastEditTime : 2024-04-04 16:49:55
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
 
-VERSION = '5.2.3'
+VERSION = '5.2.4'
 DESCRIPTION = 'Preprocessing dataset'
 PACKAGE_NAME = 'execdata'
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     author="BDFD",
```

