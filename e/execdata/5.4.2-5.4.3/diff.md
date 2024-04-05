# Comparing `tmp/execdata-5.4.2.tar.gz` & `tmp/execdata-5.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "execdata-5.4.2.tar", last modified: Fri Apr  5 15:46:38 2024, max compression
+gzip compressed data, was "execdata-5.4.3.tar", last modified: Fri Apr  5 15:52:44 2024, max compression
```

## Comparing `execdata-5.4.2.tar` & `execdata-5.4.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:46:38.289649 execdata-5.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-05 15:46:32.000000 execdata-5.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-05 15:46:38.289649 execdata-5.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-05 15:46:32.000000 execdata-5.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:46:38.285649 execdata-5.4.2/execdata/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-05 15:46:32.000000 execdata-5.4.2/execdata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:46:38.289649 execdata-5.4.2/execdata/eda/
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-05 15:46:32.000000 execdata-5.4.2/execdata/eda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-05 15:46:32.000000 execdata-5.4.2/execdata/eda/_data_mining.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-05 15:46:32.000000 execdata-5.4.2/execdata/eda/_data_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-05 15:46:32.000000 execdata-5.4.2/execdata/eda/_feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-05 15:46:32.000000 execdata-5.4.2/execdata/eda/_standardization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:46:38.289649 execdata-5.4.2/execdata/format/
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-05 15:46:32.000000 execdata-5.4.2/execdata/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-05 15:46:32.000000 execdata-5.4.2/execdata/format/_data_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-05 15:46:32.000000 execdata-5.4.2/execdata/format/_format_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:46:38.289649 execdata-5.4.2/execdata/graph/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-05 15:46:32.000000 execdata-5.4.2/execdata/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-05 15:46:32.000000 execdata-5.4.2/execdata/graph/_data_analysis_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-05 15:46:32.000000 execdata-5.4.2/execdata/graph/_data_mining_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-05 15:46:32.000000 execdata-5.4.2/execdata/graph/_linear_regression_type_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:46:32.000000 execdata-5.4.2/execdata/graph/_logistic_regression_type_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:46:38.289649 execdata-5.4.2/execdata/model/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-05 15:46:32.000000 execdata-5.4.2/execdata/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-05 15:46:32.000000 execdata-5.4.2/execdata/model/_model_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-05 15:46:32.000000 execdata-5.4.2/execdata/model/_regression_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:46:38.289649 execdata-5.4.2/execdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-05 15:46:38.000000 execdata-5.4.2/execdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-05 15:46:38.000000 execdata-5.4.2/execdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:46:38.000000 execdata-5.4.2/execdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 15:46:38.000000 execdata-5.4.2/execdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-05 15:46:32.000000 execdata-5.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 15:46:38.289649 execdata-5.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-05 15:46:32.000000 execdata-5.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:52:44.189819 execdata-5.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-05 15:52:34.000000 execdata-5.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-05 15:52:44.189819 execdata-5.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-05 15:52:34.000000 execdata-5.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:52:44.185819 execdata-5.4.3/execdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-05 15:52:34.000000 execdata-5.4.3/execdata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:52:44.189819 execdata-5.4.3/execdata/eda/
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-05 15:52:34.000000 execdata-5.4.3/execdata/eda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-05 15:52:34.000000 execdata-5.4.3/execdata/eda/_data_mining.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-05 15:52:34.000000 execdata-5.4.3/execdata/eda/_data_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-05 15:52:34.000000 execdata-5.4.3/execdata/eda/_feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-05 15:52:34.000000 execdata-5.4.3/execdata/eda/_standardization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:52:44.189819 execdata-5.4.3/execdata/format/
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-05 15:52:34.000000 execdata-5.4.3/execdata/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-05 15:52:34.000000 execdata-5.4.3/execdata/format/_data_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-05 15:52:34.000000 execdata-5.4.3/execdata/format/_format_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:52:44.189819 execdata-5.4.3/execdata/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-05 15:52:34.000000 execdata-5.4.3/execdata/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-04-05 15:52:34.000000 execdata-5.4.3/execdata/graph/_data_analysis_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-05 15:52:34.000000 execdata-5.4.3/execdata/graph/_data_mining_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-05 15:52:34.000000 execdata-5.4.3/execdata/graph/_linear_regression_type_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:52:34.000000 execdata-5.4.3/execdata/graph/_logistic_regression_type_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:52:44.189819 execdata-5.4.3/execdata/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-05 15:52:34.000000 execdata-5.4.3/execdata/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-05 15:52:34.000000 execdata-5.4.3/execdata/model/_model_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-05 15:52:34.000000 execdata-5.4.3/execdata/model/_regression_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:52:44.189819 execdata-5.4.3/execdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-05 15:52:44.000000 execdata-5.4.3/execdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-05 15:52:44.000000 execdata-5.4.3/execdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:52:44.000000 execdata-5.4.3/execdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 15:52:44.000000 execdata-5.4.3/execdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-05 15:52:34.000000 execdata-5.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 15:52:44.189819 execdata-5.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-05 15:52:34.000000 execdata-5.4.3/setup.py
```

### Comparing `execdata-5.4.2/LICENSE` & `execdata-5.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `execdata-5.4.2/PKG-INFO` & `execdata-5.4.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: execdata
-Version: 5.4.2
+Version: 5.4.3
 Summary: Preprocessing dataset
 Home-page: https://github.com/bdfd
 Author: BDFD
 Author-email: bdfd2005@gmail.com
 Project-URL: Bug Tracker, https://github.com/bdfd
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `execdata-5.4.2/README.md` & `execdata-5.4.3/README.md`

 * *Files identical despite different names*

### Comparing `execdata-5.4.2/execdata/__init__.py` & `execdata-5.4.3/execdata/__init__.py`

 * *Files identical despite different names*

### Comparing `execdata-5.4.2/execdata/eda/__init__.py` & `execdata-5.4.3/execdata/eda/__init__.py`

 * *Files identical despite different names*

### Comparing `execdata-5.4.2/execdata/eda/_data_mining.py` & `execdata-5.4.3/execdata/eda/_data_mining.py`

 * *Files identical despite different names*

### Comparing `execdata-5.4.2/execdata/eda/_data_preprocess.py` & `execdata-5.4.3/execdata/eda/_data_preprocess.py`

 * *Files identical despite different names*

### Comparing `execdata-5.4.2/execdata/eda/_feature_selection.py` & `execdata-5.4.3/execdata/eda/_feature_selection.py`

 * *Files identical despite different names*

### Comparing `execdata-5.4.2/execdata/eda/_standardization.py` & `execdata-5.4.3/execdata/eda/_standardization.py`

 * *Files identical despite different names*

### Comparing `execdata-5.4.2/execdata/format/_data_conversion.py` & `execdata-5.4.3/execdata/format/_data_conversion.py`

 * *Files identical despite different names*

### Comparing `execdata-5.4.2/execdata/format/_format_data.py` & `execdata-5.4.3/execdata/format/_format_data.py`

 * *Files identical despite different names*

### Comparing `execdata-5.4.2/execdata/graph/__init__.py` & `execdata-5.4.3/execdata/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `execdata-5.4.2/execdata/graph/_data_analysis_graph.py` & `execdata-5.4.3/execdata/graph/_data_analysis_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Date         : 2023-11-02 12:47:29
 Author       : BDFD,bdfd2005@gmail.com
 Github       : https://github.com/bdfd
-LastEditTime : 2024-04-05 11:44:47
+LastEditTime : 2024-04-05 11:50:35
 LastEditors  : <BDFD>
 Description  : 
 FilePath     : \execdata\graph\_data_analysis_graph.py
 Copyright (c) 2023 by BDFD, All Rights Reserved. 
 '''
 from tabulate import tabulate
 import seaborn as sns
@@ -57,23 +57,23 @@
     gs = fig.add_gridspec(figsize, figsize)
     gs.update(wspace=0.5, hspace=0.25)
     for i in range(figsize):
         for j in range(figsize):
             num = 0
             num = i * figsize + j
             if num < len(categorical_numerical_feature_list):
-                print(i, j)
+                # print(i, j)
                 # print('number is', num)
                 # print('number is', len(categorical_numerical_feature_list))
                 ax = fig.add_subplot(gs[i, j])
                 background_color = "#ffe6e6"
                 color_palette = ["#800000", "#8000ff",
                                  "#6aac90", "#5833ff", "#da8829"]
                 fig.patch.set_facecolor(background_color)
-                print(categorical_numerical_feature_list[num])
+                # print(categorical_numerical_feature_list[num])
                 ax.set_facecolor(background_color)
                 ax.grid(color='#000000', linestyle=':',
                         axis='y', zorder=0,  dashes=(1, 5))
                 sns.countplot(
                     ax=ax, data=df, x=categorical_numerical_feature_list[num], palette=color_palette)
                 ax.set_xlabel(
                     categorical_numerical_feature_list[num], fontsize=14, fontweight='bold', fontfamily='serif', color="#000000")
```

### Comparing `execdata-5.4.2/execdata/graph/_data_mining_graph.py` & `execdata-5.4.3/execdata/graph/_data_mining_graph.py`

 * *Files identical despite different names*

### Comparing `execdata-5.4.2/execdata/graph/_linear_regression_type_graph.py` & `execdata-5.4.3/execdata/graph/_linear_regression_type_graph.py`

 * *Files identical despite different names*

### Comparing `execdata-5.4.2/execdata/model/_model_evaluate.py` & `execdata-5.4.3/execdata/model/_model_evaluate.py`

 * *Files identical despite different names*

### Comparing `execdata-5.4.2/execdata/model/_regression_model.py` & `execdata-5.4.3/execdata/model/_regression_model.py`

 * *Files identical despite different names*

### Comparing `execdata-5.4.2/execdata.egg-info/PKG-INFO` & `execdata-5.4.3/execdata.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: execdata
-Version: 5.4.2
+Version: 5.4.3
 Summary: Preprocessing dataset
 Home-page: https://github.com/bdfd
 Author: BDFD
 Author-email: bdfd2005@gmail.com
 Project-URL: Bug Tracker, https://github.com/bdfd
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `execdata-5.4.2/execdata.egg-info/SOURCES.txt` & `execdata-5.4.3/execdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `execdata-5.4.2/setup.py` & `execdata-5.4.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 '''
 Date         : 2022-10-25 15:44:41
 Author       : BDFD,bdfd2005@gmail.com
 Github       : https://github.com/bdfd
-LastEditTime : 2024-04-05 11:35:15
+LastEditTime : 2024-04-05 11:51:09
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
 
-VERSION = '5.4.2'
+VERSION = '5.4.3'
 DESCRIPTION = 'Preprocessing dataset'
 PACKAGE_NAME = 'execdata'
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     author="BDFD",
```

