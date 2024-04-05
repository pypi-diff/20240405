# Comparing `tmp/execdata-5.4.0.tar.gz` & `tmp/execdata-5.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "execdata-5.4.0.tar", last modified: Fri Apr  5 15:06:03 2024, max compression
+gzip compressed data, was "execdata-5.4.1.tar", last modified: Fri Apr  5 15:41:24 2024, max compression
```

## Comparing `execdata-5.4.0.tar` & `execdata-5.4.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:06:03.198979 execdata-5.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-05 15:05:59.000000 execdata-5.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-05 15:06:03.198979 execdata-5.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-05 15:05:59.000000 execdata-5.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:06:03.194979 execdata-5.4.0/execdata/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:06:03.198979 execdata-5.4.0/execdata/eda/
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/eda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/eda/_data_mining.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/eda/_data_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/eda/_feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/eda/_standardization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:06:03.198979 execdata-5.4.0/execdata/format/
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/format/_data_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/format/_format_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:06:03.198979 execdata-5.4.0/execdata/graph/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/graph/_data_analysis_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/graph/_data_mining_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/graph/_linear_regression_type_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/graph/_logistic_regression_type_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:06:03.198979 execdata-5.4.0/execdata/model/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/model/_model_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-05 15:05:59.000000 execdata-5.4.0/execdata/model/_regression_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:06:03.198979 execdata-5.4.0/execdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-05 15:06:03.000000 execdata-5.4.0/execdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-05 15:06:03.000000 execdata-5.4.0/execdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:06:03.000000 execdata-5.4.0/execdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 15:06:03.000000 execdata-5.4.0/execdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-05 15:05:59.000000 execdata-5.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 15:06:03.198979 execdata-5.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-05 15:05:59.000000 execdata-5.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:24.242294 execdata-5.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-05 15:41:20.000000 execdata-5.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-05 15:41:24.242294 execdata-5.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-05 15:41:20.000000 execdata-5.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:24.238294 execdata-5.4.1/execdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-05 15:41:20.000000 execdata-5.4.1/execdata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:24.238294 execdata-5.4.1/execdata/eda/
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-05 15:41:20.000000 execdata-5.4.1/execdata/eda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-05 15:41:20.000000 execdata-5.4.1/execdata/eda/_data_mining.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-05 15:41:20.000000 execdata-5.4.1/execdata/eda/_data_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-05 15:41:20.000000 execdata-5.4.1/execdata/eda/_feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-05 15:41:20.000000 execdata-5.4.1/execdata/eda/_standardization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:24.238294 execdata-5.4.1/execdata/format/
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-05 15:41:20.000000 execdata-5.4.1/execdata/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-05 15:41:20.000000 execdata-5.4.1/execdata/format/_data_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-05 15:41:20.000000 execdata-5.4.1/execdata/format/_format_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:24.242294 execdata-5.4.1/execdata/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-05 15:41:20.000000 execdata-5.4.1/execdata/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-05 15:41:20.000000 execdata-5.4.1/execdata/graph/_data_analysis_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-05 15:41:20.000000 execdata-5.4.1/execdata/graph/_data_mining_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-05 15:41:20.000000 execdata-5.4.1/execdata/graph/_linear_regression_type_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:20.000000 execdata-5.4.1/execdata/graph/_logistic_regression_type_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:24.242294 execdata-5.4.1/execdata/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-05 15:41:20.000000 execdata-5.4.1/execdata/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-05 15:41:20.000000 execdata-5.4.1/execdata/model/_model_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-05 15:41:20.000000 execdata-5.4.1/execdata/model/_regression_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:24.242294 execdata-5.4.1/execdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-05 15:41:24.000000 execdata-5.4.1/execdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-05 15:41:24.000000 execdata-5.4.1/execdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:41:24.000000 execdata-5.4.1/execdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 15:41:24.000000 execdata-5.4.1/execdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-05 15:41:20.000000 execdata-5.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 15:41:24.242294 execdata-5.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-05 15:41:20.000000 execdata-5.4.1/setup.py
```

### Comparing `execdata-5.4.0/LICENSE` & `execdata-5.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `execdata-5.4.0/PKG-INFO` & `execdata-5.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: execdata
-Version: 5.4.0
+Version: 5.4.1
 Summary: Preprocessing dataset
 Home-page: https://github.com/bdfd
 Author: BDFD
 Author-email: bdfd2005@gmail.com
 Project-URL: Bug Tracker, https://github.com/bdfd
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `execdata-5.4.0/README.md` & `execdata-5.4.1/README.md`

 * *Files identical despite different names*

### Comparing `execdata-5.4.0/execdata/__init__.py` & `execdata-5.4.1/execdata/__init__.py`

 * *Files identical despite different names*

### Comparing `execdata-5.4.0/execdata/eda/__init__.py` & `execdata-5.4.1/execdata/eda/__init__.py`

 * *Files identical despite different names*

### Comparing `execdata-5.4.0/execdata/eda/_data_mining.py` & `execdata-5.4.1/execdata/eda/_data_mining.py`

 * *Files identical despite different names*

### Comparing `execdata-5.4.0/execdata/eda/_data_preprocess.py` & `execdata-5.4.1/execdata/eda/_data_preprocess.py`

 * *Files identical despite different names*

### Comparing `execdata-5.4.0/execdata/eda/_feature_selection.py` & `execdata-5.4.1/execdata/eda/_feature_selection.py`

 * *Files identical despite different names*

### Comparing `execdata-5.4.0/execdata/eda/_standardization.py` & `execdata-5.4.1/execdata/eda/_standardization.py`

 * *Files identical despite different names*

### Comparing `execdata-5.4.0/execdata/format/_data_conversion.py` & `execdata-5.4.1/execdata/format/_data_conversion.py`

 * *Files identical despite different names*

### Comparing `execdata-5.4.0/execdata/format/_format_data.py` & `execdata-5.4.1/execdata/format/_format_data.py`

 * *Files identical despite different names*

### Comparing `execdata-5.4.0/execdata/graph/__init__.py` & `execdata-5.4.1/execdata/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `execdata-5.4.0/execdata/graph/_data_analysis_graph.py` & `execdata-5.4.1/execdata/graph/_data_analysis_graph.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 '''
 Date         : 2023-11-02 12:47:29
 Author       : BDFD,bdfd2005@gmail.com
 Github       : https://github.com/bdfd
-LastEditTime : 2024-04-05 11:00:32
+LastEditTime : 2024-04-05 11:35:02
 LastEditors  : <BDFD>
 Description  : 
 FilePath     : \execdata\graph\_data_analysis_graph.py
 Copyright (c) 2023 by BDFD, All Rights Reserved. 
 '''
 from tabulate import tabulate
 import seaborn as sns
 import matplotlib.pyplot as plt
 import math
 
+
 def top_correlation(df, target_feature, top_feature_number=10, correlation_boundary=0.05):
     # Get Correlation of "Churn" with other variables:
     plt.figure(figsize=(20, 20))
     df.corr()[target_feature].sort_values(ascending=False).plot(kind='bar')
 
     # Calculate the correlation with the target variable and sort by values
     correlations = []
@@ -45,29 +46,36 @@
         f"Feature Correlations (sorted by absolute values):")
     print(
         f"Top 10 feature and target feature list:", top_feature_column_names)
     print(table)
 
     return top_feature_column_names
 
+
 def categorical_numerical_feature_vs_target_graph(df, categorical_numerical_feature_list, target_feature):
     figsize = math.ceil(math.sqrt(len(categorical_numerical_feature_list)))
-    fig = plt.figure(figsize=(18,15))
-    gs = fig.add_gridspec(figsize,figsize)
+    fig = plt.figure(figsize=(18, 15))
+    gs = fig.add_gridspec(figsize, figsize)
     gs.update(wspace=0.5, hspace=0.25)
     for i in range(figsize):
         for j in range(figsize):
             num = 0
-            # print(i,j)
             num = i * figsize + j
-            # print('number is',num)
-            ax = fig.add_subplot(gs[i,j])
-            background_color = "#ffe6e6"
-            color_palette = ["#800000","#8000ff","#6aac90","#5833ff","#da8829"]
-            fig.patch.set_facecolor(background_color)
-            # print(categorical_numerical_feature_list[num])
-            ax.set_facecolor(background_color)
-            # ax.text(0.5, 150, discrete_numerical_features[num], fontsize=14, fontweight='bold', fontfamily='serif', color="#000000") 
-            ax.grid(color='#000000', linestyle=':', axis='y', zorder=0,  dashes=(1,5))
-            sns.countplot(ax=ax,data=df,x=categorical_numerical_feature_list[num],palette=color_palette)
-            ax.set_xlabel(categorical_numerical_feature_list[num],fontsize=14,fontweight='bold', fontfamily='serif', color="#000000")
-            ax.set_ylabel(target_feature,fontsize=14,fontweight='bold', fontfamily='serif', color="#000000")
+            if num < len(categorical_numerical_feature_list):
+                print(i, j)
+                print('number is', num)
+                print('number is', len(categorical_numerical_feature_list))
+                ax = fig.add_subplot(gs[i, j])
+                background_color = "#ffe6e6"
+                color_palette = ["#800000", "#8000ff",
+                                 "#6aac90", "#5833ff", "#da8829"]
+                fig.patch.set_facecolor(background_color)
+                print(categorical_numerical_feature_list[num])
+                ax.set_facecolor(background_color)
+                ax.grid(color='#000000', linestyle=':',
+                        axis='y', zorder=0,  dashes=(1, 5))
+                sns.countplot(
+                    ax=ax, data=df, x=categorical_numerical_feature_list[num], palette=color_palette)
+                ax.set_xlabel(
+                    categorical_numerical_feature_list[num], fontsize=14, fontweight='bold', fontfamily='serif', color="#000000")
+                ax.set_ylabel(target_feature, fontsize=14,
+                              fontweight='bold', fontfamily='serif', color="#000000")
```

### Comparing `execdata-5.4.0/execdata/graph/_data_mining_graph.py` & `execdata-5.4.1/execdata/graph/_data_mining_graph.py`

 * *Files identical despite different names*

### Comparing `execdata-5.4.0/execdata/graph/_linear_regression_type_graph.py` & `execdata-5.4.1/execdata/graph/_linear_regression_type_graph.py`

 * *Files identical despite different names*

### Comparing `execdata-5.4.0/execdata/model/_model_evaluate.py` & `execdata-5.4.1/execdata/model/_model_evaluate.py`

 * *Files identical despite different names*

### Comparing `execdata-5.4.0/execdata/model/_regression_model.py` & `execdata-5.4.1/execdata/model/_regression_model.py`

 * *Files identical despite different names*

### Comparing `execdata-5.4.0/execdata.egg-info/PKG-INFO` & `execdata-5.4.1/execdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: execdata
-Version: 5.4.0
+Version: 5.4.1
 Summary: Preprocessing dataset
 Home-page: https://github.com/bdfd
 Author: BDFD
 Author-email: bdfd2005@gmail.com
 Project-URL: Bug Tracker, https://github.com/bdfd
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `execdata-5.4.0/execdata.egg-info/SOURCES.txt` & `execdata-5.4.1/execdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `execdata-5.4.0/setup.py` & `execdata-5.4.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 '''
 Date         : 2022-10-25 15:44:41
 Author       : BDFD,bdfd2005@gmail.com
 Github       : https://github.com/bdfd
-LastEditTime : 2024-04-05 11:03:49
+LastEditTime : 2024-04-05 11:35:15
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
 
-VERSION = '5.4.0'
+VERSION = '5.4.1'
 DESCRIPTION = 'Preprocessing dataset'
 PACKAGE_NAME = 'execdata'
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     author="BDFD",
```

