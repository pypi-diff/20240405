# Comparing `tmp/gmdm-0.2.7.tar.gz` & `tmp/gmdm-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmdm-0.2.7.tar", last modified: Mon Feb  5 16:51:17 2024, max compression
+gzip compressed data, was "gmdm-0.2.8.tar", last modified: Fri Apr  5 20:44:59 2024, max compression
```

## Comparing `gmdm-0.2.7.tar` & `gmdm-0.2.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 16:51:17.602624 gmdm-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-05 16:51:07.000000 gmdm-0.2.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-02-05 16:51:17.602624 gmdm-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-02-05 16:51:07.000000 gmdm-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-02-05 16:51:07.000000 gmdm-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 16:51:17.602624 gmdm-0.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 16:51:17.598624 gmdm-0.2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 16:51:17.598624 gmdm-0.2.7/src/gmdm/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-05 16:51:07.000000 gmdm-0.2.7/src/gmdm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13530 2024-02-05 16:51:07.000000 gmdm-0.2.7/src/gmdm/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-02-05 16:51:07.000000 gmdm-0.2.7/src/gmdm/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-05 16:51:07.000000 gmdm-0.2.7/src/gmdm/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-02-05 16:51:07.000000 gmdm-0.2.7/src/gmdm/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-02-05 16:51:07.000000 gmdm-0.2.7/src/gmdm/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 16:51:17.602624 gmdm-0.2.7/src/gmdm/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-02-05 16:51:07.000000 gmdm-0.2.7/src/gmdm/utils/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-02-05 16:51:07.000000 gmdm-0.2.7/src/gmdm/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-02-05 16:51:07.000000 gmdm-0.2.7/src/gmdm/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-02-05 16:51:07.000000 gmdm-0.2.7/src/gmdm/utils/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 16:51:17.602624 gmdm-0.2.7/src/gmdm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-02-05 16:51:17.000000 gmdm-0.2.7/src/gmdm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-02-05 16:51:17.000000 gmdm-0.2.7/src/gmdm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 16:51:17.000000 gmdm-0.2.7/src/gmdm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-05 16:51:17.000000 gmdm-0.2.7/src/gmdm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-05 16:51:17.000000 gmdm-0.2.7/src/gmdm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-05 16:51:17.000000 gmdm-0.2.7/src/gmdm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:44:59.713845 gmdm-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-05 20:44:55.000000 gmdm-0.2.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-05 20:44:59.713845 gmdm-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-05 20:44:55.000000 gmdm-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-05 20:44:55.000000 gmdm-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 20:44:59.713845 gmdm-0.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:44:59.709845 gmdm-0.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:44:59.709845 gmdm-0.2.8/src/gmdm/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-05 20:44:55.000000 gmdm-0.2.8/src/gmdm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13530 2024-04-05 20:44:55.000000 gmdm-0.2.8/src/gmdm/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-05 20:44:55.000000 gmdm-0.2.8/src/gmdm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-05 20:44:55.000000 gmdm-0.2.8/src/gmdm/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-04-05 20:44:55.000000 gmdm-0.2.8/src/gmdm/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-05 20:44:55.000000 gmdm-0.2.8/src/gmdm/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:44:59.713845 gmdm-0.2.8/src/gmdm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-05 20:44:55.000000 gmdm-0.2.8/src/gmdm/utils/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-05 20:44:55.000000 gmdm-0.2.8/src/gmdm/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-05 20:44:55.000000 gmdm-0.2.8/src/gmdm/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-05 20:44:55.000000 gmdm-0.2.8/src/gmdm/utils/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:44:59.713845 gmdm-0.2.8/src/gmdm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-05 20:44:59.000000 gmdm-0.2.8/src/gmdm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-05 20:44:59.000000 gmdm-0.2.8/src/gmdm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 20:44:59.000000 gmdm-0.2.8/src/gmdm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-05 20:44:59.000000 gmdm-0.2.8/src/gmdm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 20:44:59.000000 gmdm-0.2.8/src/gmdm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-05 20:44:59.000000 gmdm-0.2.8/src/gmdm.egg-info/top_level.txt
```

### Comparing `gmdm-0.2.7/LICENSE.md` & `gmdm-0.2.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gmdm-0.2.7/PKG-INFO` & `gmdm-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmdm
-Version: 0.2.7
+Version: 0.2.8
 Summary: The GMDM CLI tool for managing dependencies of GameMaker projects and files.
 Author-email: Kenan Masri <kenanmasri@outlook.com>
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/knno/gmdm/issues
 Keywords: gamemaker,gml,dependencies,export,libraries
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gmdm-0.2.7/README.md` & `gmdm-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `gmdm-0.2.7/pyproject.toml` & `gmdm-0.2.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gmdm"
-version = "0.2.7"
+version = "0.2.8"
 authors = [{name = "Kenan Masri", email = "kenanmasri@outlook.com"}]
 description = "The GMDM CLI tool for managing dependencies of GameMaker projects and files."
 readme = "README.md"
 requires-python = ">=3.11"
 keywords = ["gamemaker", "gml", "dependencies", "export", "libraries",]
 license = {text = "MIT License"}
 classifiers = [
```

### Comparing `gmdm-0.2.7/src/gmdm/app.py` & `gmdm-0.2.8/src/gmdm/app.py`

 * *Files identical despite different names*

### Comparing `gmdm-0.2.7/src/gmdm/cli.py` & `gmdm-0.2.8/src/gmdm/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 """The GMDM CLI tool for managing dependencies of GameMaker projects and files.
 """
-__version__ = "0.2.7"
+__version__ = "0.2.8"
 
 import argparse
 import logging
 import sys
 
 from gmdm.app import get_app
 # Variables
```

### Comparing `gmdm-0.2.7/src/gmdm/models.py` & `gmdm-0.2.8/src/gmdm/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,18 @@
 class YYFolder:
     def __init__(self, pathyy: str):
         self.pathyy = pathyy
 
     @property
     def to_project_json(self):
         return {
+            "$GMFolder": "",
+            "%Name": name_from_path(self.pathyy),
             "resourceType": "GMFolder",
-            "resourceVersion": "1.0",
+            "resourceVersion": "2.0",
             "name": name_from_path(self.pathyy),
             "folderPath": self.pathyy,
         }
 
     @property
     def to_json(self):
         return {
```

### Comparing `gmdm-0.2.7/src/gmdm/ops.py` & `gmdm-0.2.8/src/gmdm/ops.py`

 * *Files identical despite different names*

### Comparing `gmdm-0.2.7/src/gmdm/utils/files.py` & `gmdm-0.2.8/src/gmdm/utils/files.py`

 * *Files identical despite different names*

### Comparing `gmdm-0.2.7/src/gmdm/utils/logging.py` & `gmdm-0.2.8/src/gmdm/utils/logging.py`

 * *Files identical despite different names*

### Comparing `gmdm-0.2.7/src/gmdm/utils/strings.py` & `gmdm-0.2.8/src/gmdm/utils/strings.py`

 * *Files identical despite different names*

### Comparing `gmdm-0.2.7/src/gmdm.egg-info/PKG-INFO` & `gmdm-0.2.8/src/gmdm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmdm
-Version: 0.2.7
+Version: 0.2.8
 Summary: The GMDM CLI tool for managing dependencies of GameMaker projects and files.
 Author-email: Kenan Masri <kenanmasri@outlook.com>
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/knno/gmdm/issues
 Keywords: gamemaker,gml,dependencies,export,libraries
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

