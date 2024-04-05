# Comparing `tmp/crosslab_soa_service_parameter-0.2.6.tar.gz` & `tmp/crosslab_soa_service_parameter-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslab_soa_service_parameter-0.2.6.tar", last modified: Thu Feb  8 15:31:45 2024, max compression
+gzip compressed data, was "crosslab_soa_service_parameter-0.2.7.tar", last modified: Fri Apr  5 09:18:03 2024, max compression
```

## Comparing `crosslab_soa_service_parameter-0.2.6.tar` & `crosslab_soa_service_parameter-0.2.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:31:45.897572 crosslab_soa_service_parameter-0.2.6/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2117 2024-02-08 15:31:45.897572 crosslab_soa_service_parameter-0.2.6/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1706 2023-11-08 12:05:40.000000 crosslab_soa_service_parameter-0.2.6/README.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-11-08 12:05:40.000000 crosslab_soa_service_parameter-0.2.6/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)      620 2024-02-08 15:31:45.897572 crosslab_soa_service_parameter-0.2.6/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)       37 2023-11-08 12:05:40.000000 crosslab_soa_service_parameter-0.2.6/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:31:45.897572 crosslab_soa_service_parameter-0.2.6/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:31:45.897572 crosslab_soa_service_parameter-0.2.6/src/crosslab/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:31:45.897572 crosslab_soa_service_parameter-0.2.6/src/crosslab/soa_services/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:31:45.897572 crosslab_soa_service_parameter-0.2.6/src/crosslab/soa_services/parameter/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      302 2023-11-08 12:05:40.000000 crosslab_soa_service_parameter-0.2.6/src/crosslab/soa_services/parameter/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      542 2023-11-08 12:05:40.000000 crosslab_soa_service_parameter-0.2.6/src/crosslab/soa_services/parameter/messages.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3344 2023-11-08 12:05:40.000000 crosslab_soa_service_parameter-0.2.6/src/crosslab/soa_services/parameter/parameter_service.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_service_parameter-0.2.6/src/crosslab/soa_services/parameter/py.typed
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:31:45.897572 crosslab_soa_service_parameter-0.2.6/src/crosslab_soa_service_parameter.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2117 2024-02-08 15:31:45.000000 crosslab_soa_service_parameter-0.2.6/src/crosslab_soa_service_parameter.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      554 2024-02-08 15:31:45.000000 crosslab_soa_service_parameter-0.2.6/src/crosslab_soa_service_parameter.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-02-08 15:31:45.000000 crosslab_soa_service_parameter-0.2.6/src/crosslab_soa_service_parameter.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       25 2024-02-08 15:31:45.000000 crosslab_soa_service_parameter-0.2.6/src/crosslab_soa_service_parameter.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2024-02-08 15:31:45.000000 crosslab_soa_service_parameter-0.2.6/src/crosslab_soa_service_parameter.egg-info/top_level.txt
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:31:45.897572 crosslab_soa_service_parameter-0.2.6/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1042 2023-11-08 12:05:40.000000 crosslab_soa_service_parameter-0.2.6/tests/test_standard.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:18:03.782829 crosslab_soa_service_parameter-0.2.7/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2117 2024-04-05 09:18:03.782829 crosslab_soa_service_parameter-0.2.7/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1706 2023-11-08 12:05:40.000000 crosslab_soa_service_parameter-0.2.7/README.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-11-08 12:05:40.000000 crosslab_soa_service_parameter-0.2.7/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      620 2024-04-05 09:18:03.782829 crosslab_soa_service_parameter-0.2.7/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       37 2023-11-08 12:05:40.000000 crosslab_soa_service_parameter-0.2.7/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:18:03.778829 crosslab_soa_service_parameter-0.2.7/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:18:03.778829 crosslab_soa_service_parameter-0.2.7/src/crosslab/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:18:03.778829 crosslab_soa_service_parameter-0.2.7/src/crosslab/soa_services/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:18:03.782829 crosslab_soa_service_parameter-0.2.7/src/crosslab/soa_services/parameter/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      302 2023-11-08 12:05:40.000000 crosslab_soa_service_parameter-0.2.7/src/crosslab/soa_services/parameter/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      542 2023-11-08 12:05:40.000000 crosslab_soa_service_parameter-0.2.7/src/crosslab/soa_services/parameter/messages.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3344 2023-11-08 12:05:40.000000 crosslab_soa_service_parameter-0.2.7/src/crosslab/soa_services/parameter/parameter_service.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_service_parameter-0.2.7/src/crosslab/soa_services/parameter/py.typed
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:18:03.782829 crosslab_soa_service_parameter-0.2.7/src/crosslab_soa_service_parameter.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2117 2024-04-05 09:18:03.000000 crosslab_soa_service_parameter-0.2.7/src/crosslab_soa_service_parameter.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      554 2024-04-05 09:18:03.000000 crosslab_soa_service_parameter-0.2.7/src/crosslab_soa_service_parameter.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-04-05 09:18:03.000000 crosslab_soa_service_parameter-0.2.7/src/crosslab_soa_service_parameter.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       25 2024-04-05 09:18:03.000000 crosslab_soa_service_parameter-0.2.7/src/crosslab_soa_service_parameter.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2024-04-05 09:18:03.000000 crosslab_soa_service_parameter-0.2.7/src/crosslab_soa_service_parameter.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:18:03.782829 crosslab_soa_service_parameter-0.2.7/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1042 2023-11-08 12:05:40.000000 crosslab_soa_service_parameter-0.2.7/tests/test_standard.py
```

### Comparing `crosslab_soa_service_parameter-0.2.6/PKG-INFO` & `crosslab_soa_service_parameter-0.2.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosslab_soa_service_parameter
-Version: 0.2.6
+Version: 0.2.7
 Summary: The CrossLab SOA parameter Service.
 Author: Johannes Nau
 Author-email: johannes.nau@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: <3.11,>=3.8
```

### Comparing `crosslab_soa_service_parameter-0.2.6/README.rst` & `crosslab_soa_service_parameter-0.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_parameter-0.2.6/setup.cfg` & `crosslab_soa_service_parameter-0.2.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosslab_soa_service_parameter
-version = 0.2.6
+version = 0.2.7
 author = Johannes Nau
 author_email = johannes.nau@tu-ilmenau.de
 description = The CrossLab SOA parameter Service.
 long_description = file: README.rst
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Other/Proprietary License
```

### Comparing `crosslab_soa_service_parameter-0.2.6/src/crosslab/soa_services/parameter/messages.py` & `crosslab_soa_service_parameter-0.2.7/src/crosslab/soa_services/parameter/messages.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_parameter-0.2.6/src/crosslab/soa_services/parameter/parameter_service.py` & `crosslab_soa_service_parameter-0.2.7/src/crosslab/soa_services/parameter/parameter_service.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_parameter-0.2.6/src/crosslab_soa_service_parameter.egg-info/PKG-INFO` & `crosslab_soa_service_parameter-0.2.7/src/crosslab_soa_service_parameter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosslab_soa_service_parameter
-Version: 0.2.6
+Version: 0.2.7
 Summary: The CrossLab SOA parameter Service.
 Author: Johannes Nau
 Author-email: johannes.nau@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: <3.11,>=3.8
```

### Comparing `crosslab_soa_service_parameter-0.2.6/src/crosslab_soa_service_parameter.egg-info/SOURCES.txt` & `crosslab_soa_service_parameter-0.2.7/src/crosslab_soa_service_parameter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_parameter-0.2.6/tests/test_standard.py` & `crosslab_soa_service_parameter-0.2.7/tests/test_standard.py`

 * *Files identical despite different names*

