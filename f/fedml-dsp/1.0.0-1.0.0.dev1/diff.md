# Comparing `tmp/fedml_dsp-1.0.0.tar.gz` & `tmp/fedml_dsp-1.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedml_dsp-1.0.0.tar", last modified: Fri Apr  5 20:45:44 2024, max compression
+gzip compressed data, was "fedml_dsp-1.0.0.dev1.tar", last modified: Fri Apr  5 18:53:59 2024, max compression
```

## Comparing `fedml_dsp-1.0.0.tar` & `fedml_dsp-1.0.0.dev1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 I542957    (501) staff       (20)        0 2024-04-05 20:45:44.804509 fedml_dsp-1.0.0/
--rw-r--r--   0 I542957    (501) staff       (20)     1477 2024-04-05 20:45:44.803455 fedml_dsp-1.0.0/PKG-INFO
--rw-r--r--   0 I542957    (501) staff       (20)      879 2024-04-05 18:53:39.000000 fedml_dsp-1.0.0/README.md
--rw-r--r--   0 I542957    (501) staff       (20)      105 2023-12-05 19:55:41.000000 fedml_dsp-1.0.0/pyproject.toml
--rw-r--r--   0 I542957    (501) staff       (20)       38 2024-04-05 20:45:44.804712 fedml_dsp-1.0.0/setup.cfg
--rw-r--r--   0 I542957    (501) staff       (20)      930 2024-04-05 20:37:36.000000 fedml_dsp-1.0.0/setup.py
-drwxr-xr-x   0 I542957    (501) staff       (20)        0 2024-04-05 20:45:44.747765 fedml_dsp-1.0.0/src/
-drwxr-xr-x   0 I542957    (501) staff       (20)        0 2024-04-05 20:45:44.780450 fedml_dsp-1.0.0/src/fedml_dsp/
--rw-r--r--   0 I542957    (501) staff       (20)       90 2024-02-14 22:44:18.000000 fedml_dsp-1.0.0/src/fedml_dsp/__init__.py
--rw-r--r--   0 I542957    (501) staff       (20)    21647 2024-02-29 19:15:35.000000 fedml_dsp-1.0.0/src/fedml_dsp/dbconnection.py
--rw-r--r--   0 I542957    (501) staff       (20)     6639 2024-02-14 22:44:18.000000 fedml_dsp-1.0.0/src/fedml_dsp/fedml.py
--rw-r--r--   0 I542957    (501) staff       (20)      656 2024-02-14 22:44:18.000000 fedml_dsp-1.0.0/src/fedml_dsp/logger.py
-drwxr-xr-x   0 I542957    (501) staff       (20)        0 2024-04-05 20:45:44.802289 fedml_dsp-1.0.0/src/fedml_dsp.egg-info/
--rw-r--r--   0 I542957    (501) staff       (20)     1477 2024-04-05 20:45:44.000000 fedml_dsp-1.0.0/src/fedml_dsp.egg-info/PKG-INFO
--rw-r--r--   0 I542957    (501) staff       (20)      320 2024-04-05 20:45:44.000000 fedml_dsp-1.0.0/src/fedml_dsp.egg-info/SOURCES.txt
--rw-r--r--   0 I542957    (501) staff       (20)        1 2024-04-05 20:45:44.000000 fedml_dsp-1.0.0/src/fedml_dsp.egg-info/dependency_links.txt
--rw-r--r--   0 I542957    (501) staff       (20)       97 2024-04-05 20:45:44.000000 fedml_dsp-1.0.0/src/fedml_dsp.egg-info/requires.txt
--rw-r--r--   0 I542957    (501) staff       (20)       10 2024-04-05 20:45:44.000000 fedml_dsp-1.0.0/src/fedml_dsp.egg-info/top_level.txt
+drwxr-xr-x   0 I542957    (501) staff       (20)        0 2024-04-05 18:53:59.320210 fedml_dsp-1.0.0.dev1/
+-rw-r--r--   0 I542957    (501) staff       (20)     1482 2024-04-05 18:53:59.319440 fedml_dsp-1.0.0.dev1/PKG-INFO
+-rw-r--r--   0 I542957    (501) staff       (20)      879 2024-04-05 18:53:39.000000 fedml_dsp-1.0.0.dev1/README.md
+-rw-r--r--   0 I542957    (501) staff       (20)      105 2023-12-05 19:55:41.000000 fedml_dsp-1.0.0.dev1/pyproject.toml
+-rw-r--r--   0 I542957    (501) staff       (20)       38 2024-04-05 18:53:59.320347 fedml_dsp-1.0.0.dev1/setup.cfg
+-rw-r--r--   0 I542957    (501) staff       (20)      935 2024-04-05 18:51:21.000000 fedml_dsp-1.0.0.dev1/setup.py
+drwxr-xr-x   0 I542957    (501) staff       (20)        0 2024-04-05 18:53:59.302784 fedml_dsp-1.0.0.dev1/src/
+drwxr-xr-x   0 I542957    (501) staff       (20)        0 2024-04-05 18:53:59.307223 fedml_dsp-1.0.0.dev1/src/fedml_dsp/
+-rw-r--r--   0 I542957    (501) staff       (20)       90 2024-02-14 22:44:18.000000 fedml_dsp-1.0.0.dev1/src/fedml_dsp/__init__.py
+-rw-r--r--   0 I542957    (501) staff       (20)    21647 2024-02-29 19:15:35.000000 fedml_dsp-1.0.0.dev1/src/fedml_dsp/dbconnection.py
+-rw-r--r--   0 I542957    (501) staff       (20)     6639 2024-02-14 22:44:18.000000 fedml_dsp-1.0.0.dev1/src/fedml_dsp/fedml.py
+-rw-r--r--   0 I542957    (501) staff       (20)      656 2024-02-14 22:44:18.000000 fedml_dsp-1.0.0.dev1/src/fedml_dsp/logger.py
+drwxr-xr-x   0 I542957    (501) staff       (20)        0 2024-04-05 18:53:59.318635 fedml_dsp-1.0.0.dev1/src/fedml_dsp.egg-info/
+-rw-r--r--   0 I542957    (501) staff       (20)     1482 2024-04-05 18:53:59.000000 fedml_dsp-1.0.0.dev1/src/fedml_dsp.egg-info/PKG-INFO
+-rw-r--r--   0 I542957    (501) staff       (20)      320 2024-04-05 18:53:59.000000 fedml_dsp-1.0.0.dev1/src/fedml_dsp.egg-info/SOURCES.txt
+-rw-r--r--   0 I542957    (501) staff       (20)        1 2024-04-05 18:53:59.000000 fedml_dsp-1.0.0.dev1/src/fedml_dsp.egg-info/dependency_links.txt
+-rw-r--r--   0 I542957    (501) staff       (20)       97 2024-04-05 18:53:59.000000 fedml_dsp-1.0.0.dev1/src/fedml_dsp.egg-info/requires.txt
+-rw-r--r--   0 I542957    (501) staff       (20)       10 2024-04-05 18:53:59.000000 fedml_dsp-1.0.0.dev1/src/fedml_dsp.egg-info/top_level.txt
```

### Comparing `fedml_dsp-1.0.0/PKG-INFO` & `fedml_dsp-1.0.0.dev1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedml_dsp
-Version: 1.0.0
+Version: 1.0.0.dev1
 Summary: A python library for building machine learning models on gpu AI Platforms using a federated data source
 Author: SAP SE
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `fedml_dsp-1.0.0/README.md` & `fedml_dsp-1.0.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `fedml_dsp-1.0.0/setup.py` & `fedml_dsp-1.0.0.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="fedml_dsp",
-    version="1.0.0",
+    version="1.0.0.dev1",
     author="SAP SE",
     description="A python library for building machine learning models on gpu AI Platforms using a federated data source",
     license='Apache License 2.0',
     license_files = ['LICENSE.txt'],
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
```

### Comparing `fedml_dsp-1.0.0/src/fedml_dsp/dbconnection.py` & `fedml_dsp-1.0.0.dev1/src/fedml_dsp/dbconnection.py`

 * *Files identical despite different names*

### Comparing `fedml_dsp-1.0.0/src/fedml_dsp/fedml.py` & `fedml_dsp-1.0.0.dev1/src/fedml_dsp/fedml.py`

 * *Files identical despite different names*

### Comparing `fedml_dsp-1.0.0/src/fedml_dsp/logger.py` & `fedml_dsp-1.0.0.dev1/src/fedml_dsp/logger.py`

 * *Files identical despite different names*

### Comparing `fedml_dsp-1.0.0/src/fedml_dsp.egg-info/PKG-INFO` & `fedml_dsp-1.0.0.dev1/src/fedml_dsp.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedml_dsp
-Version: 1.0.0
+Version: 1.0.0.dev1
 Summary: A python library for building machine learning models on gpu AI Platforms using a federated data source
 Author: SAP SE
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

