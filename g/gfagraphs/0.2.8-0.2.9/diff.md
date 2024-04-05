# Comparing `tmp/gfagraphs-0.2.8.tar.gz` & `tmp/gfagraphs-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfagraphs-0.2.8.tar", last modified: Fri Dec  8 14:52:06 2023, max compression
+gzip compressed data, was "gfagraphs-0.2.9.tar", last modified: Fri Dec  8 14:59:10 2023, max compression
```

## Comparing `gfagraphs-0.2.8.tar` & `gfagraphs-0.2.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2023-12-08 14:52:06.518311 gfagraphs-0.2.8/
--rw-r--r--   0 sidubois (669136) genscale (35005)    34521 2023-11-29 09:58:07.000000 gfagraphs-0.2.8/LICENSE.md
--rw-r--r--   0 sidubois (669136) genscale (35005)     1994 2023-12-08 14:52:06.518311 gfagraphs-0.2.8/PKG-INFO
--rw-r--r--   0 sidubois (669136) genscale (35005)     1368 2023-11-29 09:43:15.000000 gfagraphs-0.2.8/README.md
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2023-12-08 14:52:06.517311 gfagraphs-0.2.8/gfagraphs/
--rw-r--r--   0 sidubois (669136) genscale (35005)      192 2023-09-22 08:36:37.000000 gfagraphs-0.2.8/gfagraphs/__init__.py
--rw-r--r--   0 sidubois (669136) genscale (35005)    39437 2023-11-29 14:54:03.000000 gfagraphs-0.2.8/gfagraphs/gfagraphs.py
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2023-12-08 14:52:06.518311 gfagraphs-0.2.8/gfagraphs.egg-info/
--rw-r--r--   0 sidubois (669136) genscale (35005)     1994 2023-12-08 14:52:06.000000 gfagraphs-0.2.8/gfagraphs.egg-info/PKG-INFO
--rw-r--r--   0 sidubois (669136) genscale (35005)      374 2023-12-08 14:52:06.000000 gfagraphs-0.2.8/gfagraphs.egg-info/SOURCES.txt
--rw-r--r--   0 sidubois (669136) genscale (35005)        1 2023-12-08 14:52:06.000000 gfagraphs-0.2.8/gfagraphs.egg-info/dependency_links.txt
--rw-r--r--   0 sidubois (669136) genscale (35005)        1 2023-09-22 09:02:54.000000 gfagraphs-0.2.8/gfagraphs.egg-info/not-zip-safe
--rw-r--r--   0 sidubois (669136) genscale (35005)       19 2023-12-08 14:52:06.000000 gfagraphs-0.2.8/gfagraphs.egg-info/top_level.txt
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2023-12-08 14:52:06.518311 gfagraphs-0.2.8/pgGraphs/
--rw-r--r--   0 sidubois (669136) genscale (35005)      184 2023-11-29 08:56:43.000000 gfagraphs-0.2.8/pgGraphs/__init__.py
--rw-r--r--   0 sidubois (669136) genscale (35005)      533 2023-11-29 08:50:19.000000 gfagraphs-0.2.8/pgGraphs/abstractions.py
--rw-r--r--   0 sidubois (669136) genscale (35005)    12000 2023-12-08 14:51:41.000000 gfagraphs-0.2.8/pgGraphs/gfaparser.py
--rw-r--r--   0 sidubois (669136) genscale (35005)    15528 2023-12-07 10:52:26.000000 gfagraphs-0.2.8/pgGraphs/graph.py
--rw-r--r--   0 sidubois (669136) genscale (35005)     5228 2023-11-29 09:41:37.000000 gfagraphs-0.2.8/pgGraphs/networkx.py
--rw-r--r--   0 sidubois (669136) genscale (35005)      695 2023-12-08 14:52:06.000000 gfagraphs-0.2.8/pyproject.toml
--rw-r--r--   0 sidubois (669136) genscale (35005)       38 2023-12-08 14:52:06.518311 gfagraphs-0.2.8/setup.cfg
--rw-r--r--   0 sidubois (669136) genscale (35005)     2436 2023-12-08 14:52:03.000000 gfagraphs-0.2.8/setup.py
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2023-12-08 14:52:06.518311 gfagraphs-0.2.8/tests/
--rw-r--r--   0 sidubois (669136) genscale (35005)     1302 2023-09-18 13:15:00.000000 gfagraphs-0.2.8/tests/test.py
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2023-12-08 14:59:10.784022 gfagraphs-0.2.9/
+-rw-r--r--   0 sidubois (669136) genscale (35005)    34521 2023-11-29 09:58:07.000000 gfagraphs-0.2.9/LICENSE.md
+-rw-r--r--   0 sidubois (669136) genscale (35005)     1994 2023-12-08 14:59:10.784022 gfagraphs-0.2.9/PKG-INFO
+-rw-r--r--   0 sidubois (669136) genscale (35005)     1368 2023-11-29 09:43:15.000000 gfagraphs-0.2.9/README.md
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2023-12-08 14:59:10.783022 gfagraphs-0.2.9/gfagraphs/
+-rw-r--r--   0 sidubois (669136) genscale (35005)      192 2023-09-22 08:36:37.000000 gfagraphs-0.2.9/gfagraphs/__init__.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)    39437 2023-11-29 14:54:03.000000 gfagraphs-0.2.9/gfagraphs/gfagraphs.py
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2023-12-08 14:59:10.784022 gfagraphs-0.2.9/gfagraphs.egg-info/
+-rw-r--r--   0 sidubois (669136) genscale (35005)     1994 2023-12-08 14:59:10.000000 gfagraphs-0.2.9/gfagraphs.egg-info/PKG-INFO
+-rw-r--r--   0 sidubois (669136) genscale (35005)      374 2023-12-08 14:59:10.000000 gfagraphs-0.2.9/gfagraphs.egg-info/SOURCES.txt
+-rw-r--r--   0 sidubois (669136) genscale (35005)        1 2023-12-08 14:59:10.000000 gfagraphs-0.2.9/gfagraphs.egg-info/dependency_links.txt
+-rw-r--r--   0 sidubois (669136) genscale (35005)        1 2023-09-22 09:02:54.000000 gfagraphs-0.2.9/gfagraphs.egg-info/not-zip-safe
+-rw-r--r--   0 sidubois (669136) genscale (35005)       19 2023-12-08 14:59:10.000000 gfagraphs-0.2.9/gfagraphs.egg-info/top_level.txt
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2023-12-08 14:59:10.783022 gfagraphs-0.2.9/pgGraphs/
+-rw-r--r--   0 sidubois (669136) genscale (35005)      184 2023-11-29 08:56:43.000000 gfagraphs-0.2.9/pgGraphs/__init__.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)      533 2023-11-29 08:50:19.000000 gfagraphs-0.2.9/pgGraphs/abstractions.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)    12000 2023-12-08 14:51:41.000000 gfagraphs-0.2.9/pgGraphs/gfaparser.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)    15532 2023-12-08 14:58:48.000000 gfagraphs-0.2.9/pgGraphs/graph.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)     5228 2023-11-29 09:41:37.000000 gfagraphs-0.2.9/pgGraphs/networkx.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)      695 2023-12-08 14:59:10.000000 gfagraphs-0.2.9/pyproject.toml
+-rw-r--r--   0 sidubois (669136) genscale (35005)       38 2023-12-08 14:59:10.784022 gfagraphs-0.2.9/setup.cfg
+-rw-r--r--   0 sidubois (669136) genscale (35005)     2436 2023-12-08 14:59:07.000000 gfagraphs-0.2.9/setup.py
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2023-12-08 14:59:10.783022 gfagraphs-0.2.9/tests/
+-rw-r--r--   0 sidubois (669136) genscale (35005)     1302 2023-09-18 13:15:00.000000 gfagraphs-0.2.9/tests/test.py
```

### Comparing `gfagraphs-0.2.8/LICENSE.md` & `gfagraphs-0.2.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.2.8/PKG-INFO` & `gfagraphs-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gfagraphs
-Version: 0.2.8
+Version: 0.2.9
 Summary: Library to parse, edit and handle in memory GFA graphs
 Home-page: https://github.com/Tharos-ux/gfagraphs
 Author: ('Siegfried Dubois',)
 Author-email: Siegfried Dubois <siegfried.dubois@inria.fr>
 Project-URL: Homepage, https://github.com/Tharos-ux/gfagraphs
 Project-URL: Bug Tracker, https://github.com/Tharos-ux/gfagraphs/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gfagraphs-0.2.8/README.md` & `gfagraphs-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.2.8/gfagraphs/gfagraphs.py` & `gfagraphs-0.2.9/gfagraphs/gfagraphs.py`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.2.8/gfagraphs.egg-info/PKG-INFO` & `gfagraphs-0.2.9/gfagraphs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gfagraphs
-Version: 0.2.8
+Version: 0.2.9
 Summary: Library to parse, edit and handle in memory GFA graphs
 Home-page: https://github.com/Tharos-ux/gfagraphs
 Author: ('Siegfried Dubois',)
 Author-email: Siegfried Dubois <siegfried.dubois@inria.fr>
 Project-URL: Homepage, https://github.com/Tharos-ux/gfagraphs
 Project-URL: Bug Tracker, https://github.com/Tharos-ux/gfagraphs/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gfagraphs-0.2.8/pgGraphs/abstractions.py` & `gfagraphs-0.2.9/pgGraphs/abstractions.py`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.2.8/pgGraphs/gfaparser.py` & `gfagraphs-0.2.9/pgGraphs/gfaparser.py`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.2.8/pgGraphs/graph.py` & `gfagraphs-0.2.9/pgGraphs/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
                     if not gfa_line[0].isupper() and len(gfa_line.strip()) != 0:
                         raise ValueError(
                             "All GFA lines shall start with a capital letter. Wrong format, please fix."
                         )
 
                     name, line_type, datas = GFAParser.read_gfa_line(
-                        gfa_line.split(), with_sequence)
+                        gfa_line.split('\t'), with_sequence)
                     match line_type:
                         case GFALine.SEGMENT:
                             self.segments[name] = datas
                         case GFALine.WALK | GFALine.PATH:
                             self.paths[name] = datas
                         case GFALine.LINE:
                             self.lines[name] = datas
```

### Comparing `gfagraphs-0.2.8/pgGraphs/networkx.py` & `gfagraphs-0.2.9/pgGraphs/networkx.py`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.2.8/pyproject.toml` & `gfagraphs-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires = ["setuptools>=61.0"]
     build-backend = "setuptools.build_meta"
 
     [project]
     name = "gfagraphs"
-    version = "0.2.8"
+    version = "0.2.9"
     authors = [
     { name="Siegfried Dubois", email="siegfried.dubois@inria.fr" },
     ]
     description = "Library to parse, edit and handle in memory GFA graphs"
     readme = "README.md"
     requires-python = ">=3.10"
     classifiers = [
```

### Comparing `gfagraphs-0.2.8/setup.py` & `gfagraphs-0.2.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 NAME: str = "gfagraphs"
 AUTHOR: str = "Siegfried Dubois",
 AUTHOR_EMAIL: str = "siegfried.dubois@inria.fr",
 LICENCE: str = "LICENCE"
 DESCRIPTION: str = "Library to parse, edit and handle in memory GFA graphs"
 REQUIRED_PYTHON: tuple = (3, 10)
 OVERRIDE_VN: bool = True
-VN: str = "0.2.8"
+VN: str = "0.2.9"
 URL: str = "https://github.com/Tharos-ux/gfagraphs"
 REQUIREMENTS: list[str] = ['networkx', 'tharos-pytools']
 
 
 if argv[1] in ('install', 'sdist', 'bdist_wheel'):
     # Checking if Python version is correct
     if version_info[:2] < REQUIRED_PYTHON:
```

### Comparing `gfagraphs-0.2.8/tests/test.py` & `gfagraphs-0.2.9/tests/test.py`

 * *Files identical despite different names*

