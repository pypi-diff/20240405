# Comparing `tmp/PyComplexHeatmap-1.6.8.tar.gz` & `tmp/PyComplexHeatmap-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyComplexHeatmap-1.6.8.tar", last modified: Wed Apr  3 18:04:24 2024, max compression
+gzip compressed data, was "PyComplexHeatmap-1.6.9.tar", last modified: Fri Apr  5 03:51:44 2024, max compression
```

## Comparing `PyComplexHeatmap-1.6.8.tar` & `PyComplexHeatmap-1.6.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:04:24.969965 PyComplexHeatmap-1.6.8/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:04:24.937965 PyComplexHeatmap-1.6.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:04:24.937965 PyComplexHeatmap-1.6.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:04:24.937965 PyComplexHeatmap-1.6.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-04-03 18:04:24.969965 PyComplexHeatmap-1.6.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:04:24.941965 PyComplexHeatmap-1.6.8/PyComplexHeatmap/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/PyComplexHeatmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 18:04:23.000000 PyComplexHeatmap-1.6.8/PyComplexHeatmap/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    63027 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/PyComplexHeatmap/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)    79542 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/PyComplexHeatmap/clustermap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/PyComplexHeatmap/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)    24603 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/PyComplexHeatmap/dotHeatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/PyComplexHeatmap/example.py
--rw-r--r--   0 runner    (1001) docker     (127)    19871 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/PyComplexHeatmap/oncoPrint.py
--rw-r--r--   0 runner    (1001) docker     (127)    26848 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/PyComplexHeatmap/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:04:24.969965 PyComplexHeatmap-1.6.8/PyComplexHeatmap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-04-03 18:04:24.000000 PyComplexHeatmap-1.6.8/PyComplexHeatmap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-03 18:04:24.000000 PyComplexHeatmap-1.6.8/PyComplexHeatmap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:04:24.000000 PyComplexHeatmap-1.6.8/PyComplexHeatmap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 18:04:24.000000 PyComplexHeatmap-1.6.8/PyComplexHeatmap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:04:24.965965 PyComplexHeatmap-1.6.8/comparison/
--rw-r--r--   0 runner    (1001) docker     (127)    88559 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/comparison/ComplexHeatmap.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   319414 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/comparison/ComplexHeatmap.png
--rw-r--r--   0 runner    (1001) docker     (127)   159236 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/comparison/PyComplexHeatmap.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   669615 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/comparison/PyComplexHeatmap.png
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/comparison/README.md
--rw-r--r--   0 runner    (1001) docker     (127) 15584021 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/comparison/beta.csv
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/comparison/compare.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/comparison/df_col.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2909164 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/comparison/df_row.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/comparison/heatmap.R
--rw-r--r--   0 runner    (1001) docker     (127)   182760 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/comparison/heatmap.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/comparison/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:04:24.969965 PyComplexHeatmap-1.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:51:44.211295 PyComplexHeatmap-1.6.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:51:44.179295 PyComplexHeatmap-1.6.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:51:44.179295 PyComplexHeatmap-1.6.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:51:44.183295 PyComplexHeatmap-1.6.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-04-05 03:51:44.211295 PyComplexHeatmap-1.6.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:51:44.183295 PyComplexHeatmap-1.6.9/PyComplexHeatmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/PyComplexHeatmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-05 03:51:43.000000 PyComplexHeatmap-1.6.9/PyComplexHeatmap/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63027 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/PyComplexHeatmap/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79542 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/PyComplexHeatmap/clustermap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/PyComplexHeatmap/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20240 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/PyComplexHeatmap/dotHeatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/PyComplexHeatmap/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19871 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/PyComplexHeatmap/oncoPrint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26848 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/PyComplexHeatmap/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:51:44.211295 PyComplexHeatmap-1.6.9/PyComplexHeatmap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-04-05 03:51:43.000000 PyComplexHeatmap-1.6.9/PyComplexHeatmap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-05 03:51:44.000000 PyComplexHeatmap-1.6.9/PyComplexHeatmap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:51:43.000000 PyComplexHeatmap-1.6.9/PyComplexHeatmap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 03:51:43.000000 PyComplexHeatmap-1.6.9/PyComplexHeatmap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:51:44.211295 PyComplexHeatmap-1.6.9/comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)    88559 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/comparison/ComplexHeatmap.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   319414 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/comparison/ComplexHeatmap.png
+-rw-r--r--   0 runner    (1001) docker     (127)   159236 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/comparison/PyComplexHeatmap.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   669615 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/comparison/PyComplexHeatmap.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/comparison/README.md
+-rw-r--r--   0 runner    (1001) docker     (127) 15584021 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/comparison/beta.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/comparison/compare.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/comparison/df_col.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2909164 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/comparison/df_row.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/comparison/heatmap.R
+-rw-r--r--   0 runner    (1001) docker     (127)   182760 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/comparison/heatmap.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-05 03:51:22.000000 PyComplexHeatmap-1.6.9/comparison/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-05 03:51:23.000000 PyComplexHeatmap-1.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 03:51:44.211295 PyComplexHeatmap-1.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-05 03:51:23.000000 PyComplexHeatmap-1.6.9/setup.py
```

### Comparing `PyComplexHeatmap-1.6.8/.github/FUNDING.yml` & `PyComplexHeatmap-1.6.9/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.8/.github/ISSUE_TEMPLATE/bug_report.md` & `PyComplexHeatmap-1.6.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.8/.github/ISSUE_TEMPLATE/feature_request.md` & `PyComplexHeatmap-1.6.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.8/.github/workflows/python-publish.yml` & `PyComplexHeatmap-1.6.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.8/CITATION.cff` & `PyComplexHeatmap-1.6.9/CITATION.cff`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.8/LICENSE` & `PyComplexHeatmap-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.8/PKG-INFO` & `PyComplexHeatmap-1.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.6.8
+Version: 1.6.9
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Wubin Ding
```

### Comparing `PyComplexHeatmap-1.6.8/PyComplexHeatmap/annotations.py` & `PyComplexHeatmap-1.6.9/PyComplexHeatmap/annotations.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.8/PyComplexHeatmap/clustermap.py` & `PyComplexHeatmap-1.6.9/PyComplexHeatmap/clustermap.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.8/PyComplexHeatmap/colors.py` & `PyComplexHeatmap-1.6.9/PyComplexHeatmap/colors.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.8/PyComplexHeatmap/example.py` & `PyComplexHeatmap-1.6.9/PyComplexHeatmap/example.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.8/PyComplexHeatmap/oncoPrint.py` & `PyComplexHeatmap-1.6.9/PyComplexHeatmap/oncoPrint.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.8/PyComplexHeatmap/utils.py` & `PyComplexHeatmap-1.6.9/PyComplexHeatmap/utils.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.8/PyComplexHeatmap.egg-info/PKG-INFO` & `PyComplexHeatmap-1.6.9/PyComplexHeatmap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.6.8
+Version: 1.6.9
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Wubin Ding
```

### Comparing `PyComplexHeatmap-1.6.8/PyComplexHeatmap.egg-info/SOURCES.txt` & `PyComplexHeatmap-1.6.9/PyComplexHeatmap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.8/README.md` & `PyComplexHeatmap-1.6.9/README.md`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.8/comparison/ComplexHeatmap.pdf` & `PyComplexHeatmap-1.6.9/comparison/ComplexHeatmap.pdf`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.8/comparison/ComplexHeatmap.png` & `PyComplexHeatmap-1.6.9/comparison/ComplexHeatmap.png`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.8/comparison/PyComplexHeatmap.pdf` & `PyComplexHeatmap-1.6.9/comparison/PyComplexHeatmap.pdf`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.8/comparison/PyComplexHeatmap.png` & `PyComplexHeatmap-1.6.9/comparison/PyComplexHeatmap.png`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.8/comparison/README.md` & `PyComplexHeatmap-1.6.9/comparison/README.md`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.8/comparison/beta.csv` & `PyComplexHeatmap-1.6.9/comparison/beta.csv`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.8/comparison/df_col.csv` & `PyComplexHeatmap-1.6.9/comparison/df_col.csv`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.8/comparison/df_row.csv` & `PyComplexHeatmap-1.6.9/comparison/df_row.csv`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.8/comparison/heatmap.R` & `PyComplexHeatmap-1.6.9/comparison/heatmap.R`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.8/comparison/heatmap.ipynb` & `PyComplexHeatmap-1.6.9/comparison/heatmap.ipynb`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.8/comparison/heatmap.py` & `PyComplexHeatmap-1.6.9/comparison/heatmap.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.8/pyproject.toml` & `PyComplexHeatmap-1.6.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.8/setup.py` & `PyComplexHeatmap-1.6.9/setup.py`

 * *Files identical despite different names*

