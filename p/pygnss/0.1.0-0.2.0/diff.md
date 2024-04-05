# Comparing `tmp/pygnss-0.1.0.tar.gz` & `tmp/pygnss-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygnss-0.1.0.tar", max compression
+gzip compressed data, was "pygnss-0.2.0.tar", max compression
```

## Comparing `pygnss-0.1.0.tar` & `pygnss-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,10 @@
--rw-r--r--   0        0        0     1064 2024-04-04 14:51:48.227539 pygnss-0.1.0/LICENSE
--rw-r--r--   0        0        0      160 2024-04-04 14:51:48.227539 pygnss-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-04 14:51:48.227539 pygnss-0.1.0/pygnss/__init__.py
--rw-r--r--   0        0        0      389 2024-04-04 14:51:48.227539 pygnss-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      632 1970-01-01 00:00:00.000000 pygnss-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-05 13:36:52.301320 pygnss-0.2.0/LICENSE
+-rw-r--r--   0        0        0      160 2024-04-05 13:36:52.301320 pygnss-0.2.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-05 13:36:52.301320 pygnss-0.2.0/pygnss/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 13:36:52.301320 pygnss-0.2.0/pygnss/gnss/__init__.py
+-rw-r--r--   0        0        0     1877 2024-04-05 13:36:52.301320 pygnss-0.2.0/pygnss/gnss/edit.py
+-rw-r--r--   0        0        0     1643 2024-04-05 13:36:52.301320 pygnss-0.2.0/pygnss/gnss/observables.py
+-rw-r--r--   0        0        0     9505 2024-04-05 13:36:52.301320 pygnss-0.2.0/pygnss/gnss/types.py
+-rw-r--r--   0        0        0      561 2024-04-05 13:36:52.301320 pygnss-0.2.0/pygnss/helpers.py
+-rw-r--r--   0        0        0      753 2024-04-05 13:36:52.301320 pygnss-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 pygnss-0.2.0/PKG-INFO
```

### Comparing `pygnss-0.1.0/LICENSE` & `pygnss-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygnss-0.1.0/PKG-INFO` & `pygnss-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: pygnss
-Version: 0.1.0
-Summary: 
+Version: 0.2.0
+Summary: Package with utilities for GNSS data processing
 Author: Miquel Garcia
 Author-email: miquel.garcia@rokubun.cat
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
+Requires-Dist: roktools (>=5.30.1,<6.0.0)
 Description-Content-Type: text/markdown
 
 # Python GNSS Data processing library
 
 This repository includes a series of tools to process GNSS data
 
 To install the package:
```

