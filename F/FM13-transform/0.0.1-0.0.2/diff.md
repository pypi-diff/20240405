# Comparing `tmp/FM13_transform-0.0.1.tar.gz` & `tmp/FM13_transform-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FM13_transform-0.0.1.tar", last modified: Fri Apr  5 17:47:05 2024, max compression
+gzip compressed data, was "FM13_transform-0.0.2.tar", last modified: Fri Apr  5 18:15:40 2024, max compression
```

## Comparing `FM13_transform-0.0.1.tar` & `FM13_transform-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-04-05 17:47:05.558392 FM13_transform-0.0.1/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       43 2024-04-05 17:41:39.000000 FM13_transform-0.0.1/MANIFEST.in
--rw-r--r--   0 alexander.thompson  (1013) alexander.thompson  (1013)      565 2024-04-05 17:47:05.557392 FM13_transform-0.0.1/PKG-INFO
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-03-29 16:52:09.000000 FM13_transform-0.0.1/README.md
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      729 2024-04-05 17:45:38.000000 FM13_transform-0.0.1/pyproject.toml
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       37 2024-04-05 17:42:44.000000 FM13_transform-0.0.1/requirements.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2024-04-05 17:47:05.558392 FM13_transform-0.0.1/setup.cfg
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-04-05 17:47:05.553392 FM13_transform-0.0.1/src/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-04-05 17:47:05.555392 FM13_transform-0.0.1/src/FM13_transform/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-03-29 16:53:27.000000 FM13_transform-0.0.1/src/FM13_transform/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    84286 2024-04-05 17:46:47.000000 FM13_transform-0.0.1/src/FM13_transform/data2bufr.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-04-05 17:47:05.556392 FM13_transform-0.0.1/src/FM13_transform/resources/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-03-29 16:53:59.000000 FM13_transform-0.0.1/src/FM13_transform/resources/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    14244 2024-04-05 17:37:39.000000 FM13_transform-0.0.1/src/FM13_transform/resources/synop-mappings-309009.json
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-04-05 17:47:05.557392 FM13_transform-0.0.1/src/FM13_transform.egg-info/
--rw-r--r--   0 alexander.thompson  (1013) alexander.thompson  (1013)      565 2024-04-05 17:47:05.000000 FM13_transform-0.0.1/src/FM13_transform.egg-info/PKG-INFO
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      422 2024-04-05 17:47:05.000000 FM13_transform-0.0.1/src/FM13_transform.egg-info/SOURCES.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        1 2024-04-05 17:47:05.000000 FM13_transform-0.0.1/src/FM13_transform.egg-info/dependency_links.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2024-04-05 17:47:05.000000 FM13_transform-0.0.1/src/FM13_transform.egg-info/requires.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       15 2024-04-05 17:47:05.000000 FM13_transform-0.0.1/src/FM13_transform.egg-info/top_level.txt
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-04-05 18:15:40.500852 FM13_transform-0.0.2/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       43 2024-04-05 17:41:39.000000 FM13_transform-0.0.2/MANIFEST.in
+-rw-r--r--   0 alexander.thompson  (1013) alexander.thompson  (1013)      565 2024-04-05 18:15:40.499852 FM13_transform-0.0.2/PKG-INFO
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-03-29 16:52:09.000000 FM13_transform-0.0.2/README.md
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      729 2024-04-05 18:15:18.000000 FM13_transform-0.0.2/pyproject.toml
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       37 2024-04-05 17:42:44.000000 FM13_transform-0.0.2/requirements.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2024-04-05 18:15:40.500852 FM13_transform-0.0.2/setup.cfg
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-04-05 18:15:40.496852 FM13_transform-0.0.2/src/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-04-05 18:15:40.497852 FM13_transform-0.0.2/src/FM13_transform/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-03-29 16:53:27.000000 FM13_transform-0.0.2/src/FM13_transform/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    84286 2024-04-05 17:46:47.000000 FM13_transform-0.0.2/src/FM13_transform/data2bufr.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-04-05 18:15:40.499852 FM13_transform-0.0.2/src/FM13_transform/resources/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-03-29 16:53:59.000000 FM13_transform-0.0.2/src/FM13_transform/resources/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    14244 2024-04-05 17:37:39.000000 FM13_transform-0.0.2/src/FM13_transform/resources/synop-mappings-308009.json
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-04-05 18:15:40.499852 FM13_transform-0.0.2/src/FM13_transform.egg-info/
+-rw-r--r--   0 alexander.thompson  (1013) alexander.thompson  (1013)      565 2024-04-05 18:15:40.000000 FM13_transform-0.0.2/src/FM13_transform.egg-info/PKG-INFO
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      422 2024-04-05 18:15:40.000000 FM13_transform-0.0.2/src/FM13_transform.egg-info/SOURCES.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        1 2024-04-05 18:15:40.000000 FM13_transform-0.0.2/src/FM13_transform.egg-info/dependency_links.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2024-04-05 18:15:40.000000 FM13_transform-0.0.2/src/FM13_transform.egg-info/requires.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       15 2024-04-05 18:15:40.000000 FM13_transform-0.0.2/src/FM13_transform.egg-info/top_level.txt
```

### Comparing `FM13_transform-0.0.1/PKG-INFO` & `FM13_transform-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FM13_transform
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package for converting FM13 SYNOP to BUFR4
 Author-email: Zhan Zhang <zhan.j.zhang@noaa.gov>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: WMO,SYNOP SHIP,FM-13,BUFR,decoding,weather,observations
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
```

### Comparing `FM13_transform-0.0.1/pyproject.toml` & `FM13_transform-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "FM13_transform"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Zhan Zhang", email="zhan.j.zhang@noaa.gov" },
 ]
 description = "Package for converting FM13 SYNOP to BUFR4"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `FM13_transform-0.0.1/src/FM13_transform/data2bufr.py` & `FM13_transform-0.0.2/src/FM13_transform/data2bufr.py`

 * *Files identical despite different names*

### Comparing `FM13_transform-0.0.1/src/FM13_transform/resources/synop-mappings-309009.json` & `FM13_transform-0.0.2/src/FM13_transform/resources/synop-mappings-308009.json`

 * *Files identical despite different names*

### Comparing `FM13_transform-0.0.1/src/FM13_transform.egg-info/PKG-INFO` & `FM13_transform-0.0.2/src/FM13_transform.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FM13_transform
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package for converting FM13 SYNOP to BUFR4
 Author-email: Zhan Zhang <zhan.j.zhang@noaa.gov>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: WMO,SYNOP SHIP,FM-13,BUFR,decoding,weather,observations
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
```

