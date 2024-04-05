# Comparing `tmp/gpx_vis-0.1.1.tar.gz` & `tmp/gpx_vis-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpx_vis-0.1.1.tar", last modified: Fri Apr  5 12:50:51 2024, max compression
+gzip compressed data, was "gpx_vis-0.1.3.tar", last modified: Fri Apr  5 13:36:11 2024, max compression
```

## Comparing `gpx_vis-0.1.1.tar` & `gpx_vis-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-05 12:50:51.051637 gpx_vis-0.1.1/
--rw-r--r--   0 jwt        (501) staff       (20)     1514 2024-04-05 12:16:08.000000 gpx_vis-0.1.1/LICENSE
--rw-r--r--   0 jwt        (501) staff       (20)      513 2024-04-05 12:50:51.051386 gpx_vis-0.1.1/PKG-INFO
--rw-r--r--   0 jwt        (501) staff       (20)      142 2024-04-05 12:13:11.000000 gpx_vis-0.1.1/README.md
--rw-r--r--   0 jwt        (501) staff       (20)      454 2024-04-05 12:50:44.000000 gpx_vis-0.1.1/pyproject.toml
--rw-r--r--   0 jwt        (501) staff       (20)       38 2024-04-05 12:50:51.051698 gpx_vis-0.1.1/setup.cfg
-drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-05 12:50:51.049834 gpx_vis-0.1.1/src/
--rw-r--r--   0 jwt        (501) staff       (20)      174 2024-04-05 12:36:48.000000 gpx_vis-0.1.1/src/__init__.py
-drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-05 12:50:51.051122 gpx_vis-0.1.1/src/gpx_vis.egg-info/
--rw-r--r--   0 jwt        (501) staff       (20)      513 2024-04-05 12:50:51.000000 gpx_vis-0.1.1/src/gpx_vis.egg-info/PKG-INFO
--rw-r--r--   0 jwt        (501) staff       (20)      202 2024-04-05 12:50:51.000000 gpx_vis-0.1.1/src/gpx_vis.egg-info/SOURCES.txt
--rw-r--r--   0 jwt        (501) staff       (20)        1 2024-04-05 12:50:51.000000 gpx_vis-0.1.1/src/gpx_vis.egg-info/dependency_links.txt
--rw-r--r--   0 jwt        (501) staff       (20)       16 2024-04-05 12:50:51.000000 gpx_vis-0.1.1/src/gpx_vis.egg-info/top_level.txt
--rw-r--r--   0 jwt        (501) staff       (20)    16848 2024-04-05 10:40:17.000000 gpx_vis-0.1.1/src/gpxvis.py
+drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-05 13:36:11.370875 gpx_vis-0.1.3/
+-rw-r--r--   0 jwt        (501) staff       (20)     1514 2024-04-05 12:16:08.000000 gpx_vis-0.1.3/LICENSE
+-rw-r--r--   0 jwt        (501) staff       (20)      513 2024-04-05 13:36:11.370619 gpx_vis-0.1.3/PKG-INFO
+-rw-r--r--   0 jwt        (501) staff       (20)      142 2024-04-05 12:13:11.000000 gpx_vis-0.1.3/README.md
+-rw-r--r--   0 jwt        (501) staff       (20)      454 2024-04-05 13:35:45.000000 gpx_vis-0.1.3/pyproject.toml
+-rw-r--r--   0 jwt        (501) staff       (20)       38 2024-04-05 13:36:11.370939 gpx_vis-0.1.3/setup.cfg
+drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-05 13:36:11.368878 gpx_vis-0.1.3/src/
+-rw-r--r--   0 jwt        (501) staff       (20)      174 2024-04-05 12:36:48.000000 gpx_vis-0.1.3/src/__init__.py
+drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-05 13:36:11.370365 gpx_vis-0.1.3/src/gpx_vis.egg-info/
+-rw-r--r--   0 jwt        (501) staff       (20)      513 2024-04-05 13:36:11.000000 gpx_vis-0.1.3/src/gpx_vis.egg-info/PKG-INFO
+-rw-r--r--   0 jwt        (501) staff       (20)      203 2024-04-05 13:36:11.000000 gpx_vis-0.1.3/src/gpx_vis.egg-info/SOURCES.txt
+-rw-r--r--   0 jwt        (501) staff       (20)        1 2024-04-05 13:36:11.000000 gpx_vis-0.1.3/src/gpx_vis.egg-info/dependency_links.txt
+-rw-r--r--   0 jwt        (501) staff       (20)       17 2024-04-05 13:36:11.000000 gpx_vis-0.1.3/src/gpx_vis.egg-info/top_level.txt
+-rw-r--r--   0 jwt        (501) staff       (20)    16848 2024-04-05 10:40:17.000000 gpx_vis-0.1.3/src/gpx_vis.py
```

### Comparing `gpx_vis-0.1.1/LICENSE` & `gpx_vis-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gpx_vis-0.1.1/PKG-INFO` & `gpx_vis-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpx_vis
-Version: 0.1.1
+Version: 0.1.3
 Summary: A small example package
 Author-email: Jia Wei Teh <jiaweiteh.astro@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `gpx_vis-0.1.1/src/gpx_vis.egg-info/PKG-INFO` & `gpx_vis-0.1.3/src/gpx_vis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpx_vis
-Version: 0.1.1
+Version: 0.1.3
 Summary: A small example package
 Author-email: Jia Wei Teh <jiaweiteh.astro@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `gpx_vis-0.1.1/src/gpxvis.py` & `gpx_vis-0.1.3/src/gpx_vis.py`

 * *Files identical despite different names*

