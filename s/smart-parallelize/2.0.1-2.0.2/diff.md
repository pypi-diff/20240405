# Comparing `tmp/smart_parallelize-2.0.1.tar.gz` & `tmp/smart_parallelize-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart_parallelize-2.0.1.tar", max compression
+gzip compressed data, was "smart_parallelize-2.0.2.tar", max compression
```

## Comparing `smart_parallelize-2.0.1.tar` & `smart_parallelize-2.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      560 2024-03-22 16:57:28.000000 smart_parallelize-2.0.1/README.md
--rw-r--r--   0        0        0      316 2024-04-05 18:17:41.204659 smart_parallelize-2.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-22 13:20:52.000000 smart_parallelize-2.0.1/smart_parallelize/__init__.py
--rw-r--r--   0        0        0     4285 2024-04-05 18:16:25.834211 smart_parallelize-2.0.1/smart_parallelize/parallelize.py
--rw-r--r--   0        0        0      988 1970-01-01 00:00:00.000000 smart_parallelize-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      560 2024-03-22 16:57:28.000000 smart_parallelize-2.0.2/README.md
+-rw-r--r--   0        0        0      317 2024-04-05 18:18:43.022369 smart_parallelize-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-22 13:20:52.000000 smart_parallelize-2.0.2/smart_parallelize/__init__.py
+-rw-r--r--   0        0        0     4285 2024-04-05 18:16:25.834211 smart_parallelize-2.0.2/smart_parallelize/parallelize.py
+-rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 smart_parallelize-2.0.2/PKG-INFO
```

### Comparing `smart_parallelize-2.0.1/README.md` & `smart_parallelize-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `smart_parallelize-2.0.1/smart_parallelize/parallelize.py` & `smart_parallelize-2.0.2/smart_parallelize/parallelize.py`

 * *Files identical despite different names*

### Comparing `smart_parallelize-2.0.1/PKG-INFO` & `smart_parallelize-2.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: smart-parallelize
-Version: 2.0.1
+Version: 2.0.2
 Summary: 
 Author: Truman DeWalch
 Author-email: trumandewalch@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
-Requires-Dist: ray (>=2.7.0,<3.0.0)
+Requires-Dist: ray (>=2.10.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <!-- write a heading for describing this -->
 ## Description
 
 This is a simply python package for easily parallelizing functions using.
```

