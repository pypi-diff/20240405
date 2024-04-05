# Comparing `tmp/opsramp-analytics-utils-3.4.8.tar.gz` & `tmp/opsramp-analytics-utils-3.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opsramp-analytics-utils-3.4.8.tar", last modified: Fri Mar  8 09:39:28 2024, max compression
+gzip compressed data, was "opsramp-analytics-utils-3.4.9.tar", last modified: Fri Apr  5 11:27:10 2024, max compression
```

## Comparing `opsramp-analytics-utils-3.4.8.tar` & `opsramp-analytics-utils-3.4.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-03-08 09:39:28.519747 opsramp-analytics-utils-3.4.8/
--rw-r--r--   0 rajumummidi   (502) staff       (20)     1073 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.8/LICENSE
--rw-r--r--   0 rajumummidi   (502) staff       (20)      186 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.8/MANIFEST.in
--rw-r--r--   0 rajumummidi   (502) staff       (20)     1336 2024-03-08 09:39:28.519456 opsramp-analytics-utils-3.4.8/PKG-INFO
--rw-r--r--   0 rajumummidi   (502) staff       (20)      711 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.8/README.md
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-03-08 09:39:28.500915 opsramp-analytics-utils-3.4.8/analytics_sdk/
--rw-r--r--   0 rajumummidi   (502) staff       (20)       30 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/__init__.py
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-03-08 09:39:28.504460 opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/
--rw-r--r--   0 rajumummidi   (502) staff       (20)      921 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/main.js
--rw-r--r--   0 rajumummidi   (502) staff       (20)  3321723 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/main.wrapper.css
--rw-r--r--   0 rajumummidi   (502) staff       (20)  2628164 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/main.wrapper.js
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-03-08 09:39:28.516156 opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/media/
--rw-r--r--   0 rajumummidi   (502) staff       (20)      320 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/media/close.82b1ae2d.svg
--rw-r--r--   0 rajumummidi   (502) staff       (20)    34172 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff
--rw-r--r--   0 rajumummidi   (502) staff       (20)   148200 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg
--rw-r--r--   0 rajumummidi   (502) staff       (20)    64440 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf
--rw-r--r--   0 rajumummidi   (502) staff       (20)    29136 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2
--rw-r--r--   0 rajumummidi   (502) staff       (20)    64608 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot
--rw-r--r--   0 rajumummidi   (502) staff       (20)      602 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg
--rw-r--r--   0 rajumummidi   (502) staff       (20)      861 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg
--rw-r--r--   0 rajumummidi   (502) staff       (20)     1403 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg
--rw-r--r--   0 rajumummidi   (502) staff       (20)     7536 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff
--rw-r--r--   0 rajumummidi   (502) staff       (20)    11968 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf
--rw-r--r--   0 rajumummidi   (502) staff       (20)    12136 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot
--rw-r--r--   0 rajumummidi   (502) staff       (20)      733 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-03-08 09:39:28.516912 opsramp-analytics-utils-3.4.8/analytics_sdk/api/
--rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/api/__init__.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)    17387 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/api/api_client.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     9382 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/api/api_task.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)      992 2024-01-29 06:36:39.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/api/thread_process.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)    17374 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/api_client.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     4100 2024-03-08 08:04:41.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/components.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)       38 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/constants.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     4730 2024-03-08 08:03:00.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/oap_dash.py
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-03-08 09:39:28.517497 opsramp-analytics-utils-3.4.8/analytics_sdk/process/
--rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/process/__init__.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     5809 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/process/process.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     4692 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/process/querybuilder.py
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-03-08 09:39:28.518412 opsramp-analytics-utils-3.4.8/analytics_sdk/renderer/
--rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/renderer/__init__.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)    35042 2024-01-29 09:30:11.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/renderer/excel.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     2887 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/renderer/pdf.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)    43575 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.4.8/analytics_sdk/utilities.py
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-03-08 09:39:28.519102 opsramp-analytics-utils-3.4.8/opsramp_analytics_utils.egg-info/
--rw-r--r--   0 rajumummidi   (502) staff       (20)     1336 2024-03-08 09:39:28.000000 opsramp-analytics-utils-3.4.8/opsramp_analytics_utils.egg-info/PKG-INFO
--rw-r--r--   0 rajumummidi   (502) staff       (20)     1698 2024-03-08 09:39:28.000000 opsramp-analytics-utils-3.4.8/opsramp_analytics_utils.egg-info/SOURCES.txt
--rw-r--r--   0 rajumummidi   (502) staff       (20)        1 2024-03-08 09:39:28.000000 opsramp-analytics-utils-3.4.8/opsramp_analytics_utils.egg-info/dependency_links.txt
--rw-r--r--   0 rajumummidi   (502) staff       (20)      125 2024-03-08 09:39:28.000000 opsramp-analytics-utils-3.4.8/opsramp_analytics_utils.egg-info/requires.txt
--rw-r--r--   0 rajumummidi   (502) staff       (20)       14 2024-03-08 09:39:28.000000 opsramp-analytics-utils-3.4.8/opsramp_analytics_utils.egg-info/top_level.txt
--rw-r--r--   0 rajumummidi   (502) staff       (20)      125 2024-03-08 08:09:17.000000 opsramp-analytics-utils-3.4.8/requires-install.txt
--rw-r--r--   0 rajumummidi   (502) staff       (20)       38 2024-03-08 09:39:28.519805 opsramp-analytics-utils-3.4.8/setup.cfg
--rw-r--r--   0 rajumummidi   (502) staff       (20)      943 2024-03-08 09:33:55.000000 opsramp-analytics-utils-3.4.8/setup.py
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-05 11:27:10.553773 opsramp-analytics-utils-3.4.9/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     1073 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.9/LICENSE
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      186 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.9/MANIFEST.in
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     1328 2024-04-05 11:27:10.553612 opsramp-analytics-utils-3.4.9/PKG-INFO
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      711 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.9/README.md
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-05 11:27:10.536516 opsramp-analytics-utils-3.4.9/analytics_sdk/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)       30 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/__init__.py
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-05 11:27:10.540763 opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      921 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/main.js
+-rw-r--r--   0 rajumummidi   (502) staff       (20)  3321723 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/main.wrapper.css
+-rw-r--r--   0 rajumummidi   (502) staff       (20)  2628164 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/main.wrapper.js
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-05 11:27:10.550390 opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/media/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      320 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/media/close.82b1ae2d.svg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    34172 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff
+-rw-r--r--   0 rajumummidi   (502) staff       (20)   148200 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    64440 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    29136 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    64608 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      602 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      861 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     1403 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     7536 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    11968 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    12136 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      733 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-05 11:27:10.551190 opsramp-analytics-utils-3.4.9/analytics_sdk/api/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/api/__init__.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    17387 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/api/api_client.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     9382 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/api/api_task.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      992 2024-01-29 06:36:39.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/api/thread_process.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    17374 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/api_client.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     4100 2024-03-08 08:04:41.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/components.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)       38 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/constants.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     4730 2024-03-08 08:03:00.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/oap_dash.py
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-05 11:27:10.551760 opsramp-analytics-utils-3.4.9/analytics_sdk/process/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/process/__init__.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     5809 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/process/process.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     4692 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/process/querybuilder.py
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-05 11:27:10.552569 opsramp-analytics-utils-3.4.9/analytics_sdk/renderer/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/renderer/__init__.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    35042 2024-01-29 09:30:11.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/renderer/excel.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     2887 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/renderer/pdf.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    43575 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.4.9/analytics_sdk/utilities.py
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-05 11:27:10.553400 opsramp-analytics-utils-3.4.9/opsramp_analytics_utils.egg-info/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     1328 2024-04-05 11:27:10.000000 opsramp-analytics-utils-3.4.9/opsramp_analytics_utils.egg-info/PKG-INFO
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     1698 2024-04-05 11:27:10.000000 opsramp-analytics-utils-3.4.9/opsramp_analytics_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 rajumummidi   (502) staff       (20)        1 2024-04-05 11:27:10.000000 opsramp-analytics-utils-3.4.9/opsramp_analytics_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      125 2024-04-05 11:27:10.000000 opsramp-analytics-utils-3.4.9/opsramp_analytics_utils.egg-info/requires.txt
+-rw-r--r--   0 rajumummidi   (502) staff       (20)       14 2024-04-05 11:27:10.000000 opsramp-analytics-utils-3.4.9/opsramp_analytics_utils.egg-info/top_level.txt
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      139 2024-04-02 11:40:54.000000 opsramp-analytics-utils-3.4.9/requires-install.txt
+-rw-r--r--   0 rajumummidi   (502) staff       (20)       38 2024-04-05 11:27:10.553827 opsramp-analytics-utils-3.4.9/setup.cfg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      943 2024-04-05 11:18:35.000000 opsramp-analytics-utils-3.4.9/setup.py
```

### Comparing `opsramp-analytics-utils-3.4.8/LICENSE` & `opsramp-analytics-utils-3.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/PKG-INFO` & `opsramp-analytics-utils-3.4.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,39 @@
 Metadata-Version: 2.1
 Name: opsramp-analytics-utils
-Version: 3.4.8
+Version: 3.4.9
 Summary: OpsRamp Analytics SDK
+Home-page: UNKNOWN
 Author: OpsRamp
 Author-email: opsramp@support.com
+License: UNKNOWN
+Description: ## OpsRamp Analytics Utilities
+        
+        This is the SDK for writing OpsRamp analytics apps. It is based on [dash](https://plotly.com/dash/), and it has a number of utility functions.
+        
+        It contains [analysis wrapper project](https://github.com/opsramp/analysis-wrapper).
+        
+        It is published on [Pypi](https://pypi.org/project/opsramp-analytics-utils/)
+        
+        #### How to publish on Pypi
+        
+        After make updates on SDK, modify the version in _setup.py_.
+        
+        ```
+        python setup.py sdist bdist_wheel
+        python -m twine upload dist/*
+        
+        Note: if above command not works, then use below command
+        python -m twine upload --skip-existing dist/*
+        ```
+        
+        - To upgrade the sdk for your app
+        ```
+        pip install --no-cache-dir --upgrade opsramp-analytics-utils
+        ```
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: boto3==1.17.51
-Requires-Dist: botocore==1.20.51
-Requires-Dist: openpyxl==3.0.7
-Requires-Dist: flask==3.0.0
-Requires-Dist: dash==2.14.2
-Requires-Dist: requests==2.31.0
-Requires-Dist: Werkzeug==3.0.1
-Requires-Dist: urllib3==1.26.18
-
-## OpsRamp Analytics Utilities
-
-This is the SDK for writing OpsRamp analytics apps. It is based on [dash](https://plotly.com/dash/), and it has a number of utility functions.
-
-It contains [analysis wrapper project](https://github.com/opsramp/analysis-wrapper).
-
-It is published on [Pypi](https://pypi.org/project/opsramp-analytics-utils/)
-
-#### How to publish on Pypi
-
-After make updates on SDK, modify the version in _setup.py_.
-
-```
-python setup.py sdist bdist_wheel
-python -m twine upload dist/*
-
-Note: if above command not works, then use below command
-python -m twine upload --skip-existing dist/*
-```
-
-- To upgrade the sdk for your app
-```
-pip install --no-cache-dir --upgrade opsramp-analytics-utils
-```
```

### Comparing `opsramp-analytics-utils-3.4.8/README.md` & `opsramp-analytics-utils-3.4.9/README.md`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/main.js` & `opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/main.js`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/main.wrapper.css` & `opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/main.wrapper.css`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/main.wrapper.js` & `opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/main.wrapper.js`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff` & `opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg` & `opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf` & `opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2` & `opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot` & `opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg` & `opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg` & `opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg` & `opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff` & `opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf` & `opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot` & `opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg` & `opsramp-analytics-utils-3.4.9/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/analytics_sdk/api/api_client.py` & `opsramp-analytics-utils-3.4.9/analytics_sdk/api/api_client.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/analytics_sdk/api/api_task.py` & `opsramp-analytics-utils-3.4.9/analytics_sdk/api/api_task.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/analytics_sdk/api/thread_process.py` & `opsramp-analytics-utils-3.4.9/analytics_sdk/api/thread_process.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/analytics_sdk/api_client.py` & `opsramp-analytics-utils-3.4.9/analytics_sdk/api_client.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/analytics_sdk/components.py` & `opsramp-analytics-utils-3.4.9/analytics_sdk/components.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/analytics_sdk/oap_dash.py` & `opsramp-analytics-utils-3.4.9/analytics_sdk/oap_dash.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/analytics_sdk/process/process.py` & `opsramp-analytics-utils-3.4.9/analytics_sdk/process/process.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/analytics_sdk/process/querybuilder.py` & `opsramp-analytics-utils-3.4.9/analytics_sdk/process/querybuilder.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/analytics_sdk/renderer/excel.py` & `opsramp-analytics-utils-3.4.9/analytics_sdk/renderer/excel.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/analytics_sdk/renderer/pdf.py` & `opsramp-analytics-utils-3.4.9/analytics_sdk/renderer/pdf.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/analytics_sdk/utilities.py` & `opsramp-analytics-utils-3.4.9/analytics_sdk/utilities.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/opsramp_analytics_utils.egg-info/PKG-INFO` & `opsramp-analytics-utils-3.4.9/opsramp_analytics_utils.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,39 @@
 Metadata-Version: 2.1
 Name: opsramp-analytics-utils
-Version: 3.4.8
+Version: 3.4.9
 Summary: OpsRamp Analytics SDK
+Home-page: UNKNOWN
 Author: OpsRamp
 Author-email: opsramp@support.com
+License: UNKNOWN
+Description: ## OpsRamp Analytics Utilities
+        
+        This is the SDK for writing OpsRamp analytics apps. It is based on [dash](https://plotly.com/dash/), and it has a number of utility functions.
+        
+        It contains [analysis wrapper project](https://github.com/opsramp/analysis-wrapper).
+        
+        It is published on [Pypi](https://pypi.org/project/opsramp-analytics-utils/)
+        
+        #### How to publish on Pypi
+        
+        After make updates on SDK, modify the version in _setup.py_.
+        
+        ```
+        python setup.py sdist bdist_wheel
+        python -m twine upload dist/*
+        
+        Note: if above command not works, then use below command
+        python -m twine upload --skip-existing dist/*
+        ```
+        
+        - To upgrade the sdk for your app
+        ```
+        pip install --no-cache-dir --upgrade opsramp-analytics-utils
+        ```
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: boto3==1.17.51
-Requires-Dist: botocore==1.20.51
-Requires-Dist: openpyxl==3.0.7
-Requires-Dist: flask==3.0.0
-Requires-Dist: dash==2.14.2
-Requires-Dist: requests==2.31.0
-Requires-Dist: Werkzeug==3.0.1
-Requires-Dist: urllib3==1.26.18
-
-## OpsRamp Analytics Utilities
-
-This is the SDK for writing OpsRamp analytics apps. It is based on [dash](https://plotly.com/dash/), and it has a number of utility functions.
-
-It contains [analysis wrapper project](https://github.com/opsramp/analysis-wrapper).
-
-It is published on [Pypi](https://pypi.org/project/opsramp-analytics-utils/)
-
-#### How to publish on Pypi
-
-After make updates on SDK, modify the version in _setup.py_.
-
-```
-python setup.py sdist bdist_wheel
-python -m twine upload dist/*
-
-Note: if above command not works, then use below command
-python -m twine upload --skip-existing dist/*
-```
-
-- To upgrade the sdk for your app
-```
-pip install --no-cache-dir --upgrade opsramp-analytics-utils
-```
```

### Comparing `opsramp-analytics-utils-3.4.8/opsramp_analytics_utils.egg-info/SOURCES.txt` & `opsramp-analytics-utils-3.4.9/opsramp_analytics_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.4.8/setup.py` & `opsramp-analytics-utils-3.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     with open("requires-{}.txt".format(req_type)) as fp:
         requires = (line.strip() for line in fp)
         return [req for req in requires if req and not req.startswith("#")]
 
 
 setuptools.setup(
     name="opsramp-analytics-utils",
-    version="3.4.8",
+    version="3.4.9",
     author="OpsRamp",
     author_email="opsramp@support.com",
     description="OpsRamp Analytics SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=read_req_file("install"),
     # url="https://github.com/opsramp/analytics-sdk",
```

