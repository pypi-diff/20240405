# Comparing `tmp/AIPySdeAnalyzer-0.3.2.tar.gz` & `tmp/AIPySdeAnalyzer-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AIPySdeAnalyzer-0.3.2.tar", last modified: Fri Apr  5 15:05:02 2024, max compression
+gzip compressed data, was "AIPySdeAnalyzer-0.3.4.tar", last modified: Fri Apr  5 15:19:04 2024, max compression
```

## Comparing `AIPySdeAnalyzer-0.3.2.tar` & `AIPySdeAnalyzer-0.3.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 15:05:02.980673 AIPySdeAnalyzer-0.3.2/
-drwxrwxrwx   0        0        0        0 2024-04-05 15:05:02.945314 AIPySdeAnalyzer-0.3.2/AIPySdeAnalyzer.egg-info/
--rw-rw-rw-   0        0        0     4328 2024-04-05 15:05:02.000000 AIPySdeAnalyzer-0.3.2/AIPySdeAnalyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      614 2024-04-05 15:05:02.000000 AIPySdeAnalyzer-0.3.2/AIPySdeAnalyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 15:05:02.000000 AIPySdeAnalyzer-0.3.2/AIPySdeAnalyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      148 2024-04-05 15:05:02.000000 AIPySdeAnalyzer-0.3.2/AIPySdeAnalyzer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      116 2024-04-05 15:05:02.000000 AIPySdeAnalyzer-0.3.2/AIPySdeAnalyzer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-05 15:05:02.000000 AIPySdeAnalyzer-0.3.2/AIPySdeAnalyzer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-03-21 11:55:37.000000 AIPySdeAnalyzer-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     4328 2024-04-05 15:05:02.977680 AIPySdeAnalyzer-0.3.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-05 15:05:02.852200 AIPySdeAnalyzer-0.3.2/aipys_analyse/
-drwxrwxrwx   0        0        0        0 2024-04-05 15:05:02.888499 AIPySdeAnalyzer-0.3.2/aipys_analyse/CLI/
--rw-rw-rw-   0        0        0        0 2024-03-07 19:26:43.000000 AIPySdeAnalyzer-0.3.2/aipys_analyse/CLI/__init__.py
--rw-rw-rw-   0        0        0     3059 2024-03-07 19:26:43.000000 AIPySdeAnalyzer-0.3.2/aipys_analyse/CLI/loadParametres.py
--rw-rw-rw-   0        0        0     5903 2024-03-07 19:26:43.000000 AIPySdeAnalyzer-0.3.2/aipys_analyse/CLI/setParameters.py
--rw-rw-rw-   0        0        0     4881 2024-03-18 09:47:02.000000 AIPySdeAnalyzer-0.3.2/aipys_analyse/SimInit.py
--rw-rw-rw-   0        0        0        0 2024-03-07 22:29:43.000000 AIPySdeAnalyzer-0.3.2/aipys_analyse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 15:05:02.914878 AIPySdeAnalyzer-0.3.2/aipys_analyse/func/
--rw-rw-rw-   0        0        0        0 2024-03-07 19:26:44.000000 AIPySdeAnalyzer-0.3.2/aipys_analyse/func/__init__.py
--rw-rw-rw-   0        0        0     2633 2024-03-07 19:26:44.000000 AIPySdeAnalyzer-0.3.2/aipys_analyse/func/mapSgRNA.py
--rw-rw-rw-   0        0        0     2364 2024-03-07 19:26:44.000000 AIPySdeAnalyzer-0.3.2/aipys_analyse/func/unPacking.py
-drwxrwxrwx   0        0        0        0 2024-04-05 15:05:02.942323 AIPySdeAnalyzer-0.3.2/aipys_analyse/simulation/
--rw-rw-rw-   0        0        0     7929 2024-03-20 20:40:38.000000 AIPySdeAnalyzer-0.3.2/aipys_analyse/simulation/Simulate.py
--rw-rw-rw-   0        0        0        0 2024-03-07 19:26:43.000000 AIPySdeAnalyzer-0.3.2/aipys_analyse/simulation/__init__.py
--rw-rw-rw-   0        0        0     2391 2024-04-05 13:02:47.000000 AIPySdeAnalyzer-0.3.2/aipys_analyse/simulation/runSimulation.py
--rw-rw-rw-   0        0        0       42 2024-04-05 15:05:02.980673 AIPySdeAnalyzer-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1162 2024-04-05 15:04:54.000000 AIPySdeAnalyzer-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:19:04.568809 AIPySdeAnalyzer-0.3.4/
+drwxrwxrwx   0        0        0        0 2024-04-05 15:19:04.505833 AIPySdeAnalyzer-0.3.4/AIPySdeAnalyzer.egg-info/
+-rw-rw-rw-   0        0        0     4304 2024-04-05 15:19:03.000000 AIPySdeAnalyzer-0.3.4/AIPySdeAnalyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      614 2024-04-05 15:19:04.000000 AIPySdeAnalyzer-0.3.4/AIPySdeAnalyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 15:19:03.000000 AIPySdeAnalyzer-0.3.4/AIPySdeAnalyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      148 2024-04-05 15:19:03.000000 AIPySdeAnalyzer-0.3.4/AIPySdeAnalyzer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      108 2024-04-05 15:19:03.000000 AIPySdeAnalyzer-0.3.4/AIPySdeAnalyzer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-05 15:19:03.000000 AIPySdeAnalyzer-0.3.4/AIPySdeAnalyzer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-03-21 11:55:37.000000 AIPySdeAnalyzer-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0     4304 2024-04-05 15:19:04.562824 AIPySdeAnalyzer-0.3.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-05 15:19:04.399150 AIPySdeAnalyzer-0.3.4/aipys_analyse/
+drwxrwxrwx   0        0        0        0 2024-04-05 15:19:04.438774 AIPySdeAnalyzer-0.3.4/aipys_analyse/CLI/
+-rw-rw-rw-   0        0        0        0 2024-03-07 19:26:43.000000 AIPySdeAnalyzer-0.3.4/aipys_analyse/CLI/__init__.py
+-rw-rw-rw-   0        0        0     3059 2024-03-07 19:26:43.000000 AIPySdeAnalyzer-0.3.4/aipys_analyse/CLI/loadParametres.py
+-rw-rw-rw-   0        0        0     5903 2024-03-07 19:26:43.000000 AIPySdeAnalyzer-0.3.4/aipys_analyse/CLI/setParameters.py
+-rw-rw-rw-   0        0        0     4881 2024-03-18 09:47:02.000000 AIPySdeAnalyzer-0.3.4/aipys_analyse/SimInit.py
+-rw-rw-rw-   0        0        0        0 2024-03-07 22:29:43.000000 AIPySdeAnalyzer-0.3.4/aipys_analyse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:19:04.470166 AIPySdeAnalyzer-0.3.4/aipys_analyse/func/
+-rw-rw-rw-   0        0        0        0 2024-03-07 19:26:44.000000 AIPySdeAnalyzer-0.3.4/aipys_analyse/func/__init__.py
+-rw-rw-rw-   0        0        0     2633 2024-03-07 19:26:44.000000 AIPySdeAnalyzer-0.3.4/aipys_analyse/func/mapSgRNA.py
+-rw-rw-rw-   0        0        0     2364 2024-03-07 19:26:44.000000 AIPySdeAnalyzer-0.3.4/aipys_analyse/func/unPacking.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:19:04.499629 AIPySdeAnalyzer-0.3.4/aipys_analyse/simulation/
+-rw-rw-rw-   0        0        0     7929 2024-03-20 20:40:38.000000 AIPySdeAnalyzer-0.3.4/aipys_analyse/simulation/Simulate.py
+-rw-rw-rw-   0        0        0        0 2024-03-07 19:26:43.000000 AIPySdeAnalyzer-0.3.4/aipys_analyse/simulation/__init__.py
+-rw-rw-rw-   0        0        0     2391 2024-04-05 13:02:47.000000 AIPySdeAnalyzer-0.3.4/aipys_analyse/simulation/runSimulation.py
+-rw-rw-rw-   0        0        0       42 2024-04-05 15:19:04.568809 AIPySdeAnalyzer-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1162 2024-04-05 15:18:48.000000 AIPySdeAnalyzer-0.3.4/setup.py
```

### Comparing `AIPySdeAnalyzer-0.3.2/AIPySdeAnalyzer.egg-info/PKG-INFO` & `AIPySdeAnalyzer-0.3.4/AIPySdeAnalyzer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: AIPySdeAnalyzer
-Version: 0.3.2
+Version: 0.3.4
 Summary: AI Powered Photoswitchable Screen analysis
 Home-page: 
 Author: Gil Kanfer
 Author-email: gil.kanfer.il@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytensors
 Requires-Dist: pymc
 Requires-Dist: imageio
-Requires-Dist: numpyro
 Requires-Dist: bnlearn
 Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: seaborn
 Requires-Dist: scikit-learn
 Requires-Dist: IPython
 Requires-Dist: openpyxl
```

### Comparing `AIPySdeAnalyzer-0.3.2/AIPySdeAnalyzer.egg-info/SOURCES.txt` & `AIPySdeAnalyzer-0.3.4/AIPySdeAnalyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AIPySdeAnalyzer-0.3.2/LICENSE` & `AIPySdeAnalyzer-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `AIPySdeAnalyzer-0.3.2/PKG-INFO` & `AIPySdeAnalyzer-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: AIPySdeAnalyzer
-Version: 0.3.2
+Version: 0.3.4
 Summary: AI Powered Photoswitchable Screen analysis
 Home-page: 
 Author: Gil Kanfer
 Author-email: gil.kanfer.il@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytensors
 Requires-Dist: pymc
 Requires-Dist: imageio
-Requires-Dist: numpyro
 Requires-Dist: bnlearn
 Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: seaborn
 Requires-Dist: scikit-learn
 Requires-Dist: IPython
 Requires-Dist: openpyxl
```

### Comparing `AIPySdeAnalyzer-0.3.2/aipys_analyse/CLI/loadParametres.py` & `AIPySdeAnalyzer-0.3.4/aipys_analyse/CLI/loadParametres.py`

 * *Files identical despite different names*

### Comparing `AIPySdeAnalyzer-0.3.2/aipys_analyse/CLI/setParameters.py` & `AIPySdeAnalyzer-0.3.4/aipys_analyse/CLI/setParameters.py`

 * *Files identical despite different names*

### Comparing `AIPySdeAnalyzer-0.3.2/aipys_analyse/SimInit.py` & `AIPySdeAnalyzer-0.3.4/aipys_analyse/SimInit.py`

 * *Files identical despite different names*

### Comparing `AIPySdeAnalyzer-0.3.2/aipys_analyse/func/mapSgRNA.py` & `AIPySdeAnalyzer-0.3.4/aipys_analyse/func/mapSgRNA.py`

 * *Files identical despite different names*

### Comparing `AIPySdeAnalyzer-0.3.2/aipys_analyse/func/unPacking.py` & `AIPySdeAnalyzer-0.3.4/aipys_analyse/func/unPacking.py`

 * *Files identical despite different names*

### Comparing `AIPySdeAnalyzer-0.3.2/aipys_analyse/simulation/Simulate.py` & `AIPySdeAnalyzer-0.3.4/aipys_analyse/simulation/Simulate.py`

 * *Files identical despite different names*

### Comparing `AIPySdeAnalyzer-0.3.2/aipys_analyse/simulation/runSimulation.py` & `AIPySdeAnalyzer-0.3.4/aipys_analyse/simulation/runSimulation.py`

 * *Files identical despite different names*

### Comparing `AIPySdeAnalyzer-0.3.2/setup.py` & `AIPySdeAnalyzer-0.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages,find_namespace_packages
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name="AIPySdeAnalyzer",
-    version="0.3.2",
+    version="0.3.4",
     install_requires=required,
     packages=find_packages(include=['aipys_analyse','aipys_analyse.simulation','aipys_analyse.CLI','aipys_analyse.func']),
     entry_points={
         'console_scripts': [
         'updateParameters=aipys_analyse.CLI.setParameters:update_user_parameters',
         'load-parameters=aipys_analyse.CLI.loadParametres:main', 
             ],
```

