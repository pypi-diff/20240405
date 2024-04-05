# Comparing `tmp/turning_points-0.0.2.tar.gz` & `tmp/turning_points-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turning_points-0.0.2.tar", last modified: Fri Apr  5 04:26:11 2024, max compression
+gzip compressed data, was "turning_points-0.0.3.tar", last modified: Fri Apr  5 04:39:15 2024, max compression
```

## Comparing `turning_points-0.0.2.tar` & `turning_points-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 04:26:11.761201 turning_points-0.0.2/
--rw-rw-rw-   0        0        0     1070 2024-04-05 03:12:32.000000 turning_points-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     3313 2024-04-05 04:26:11.759201 turning_points-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1898 2024-04-05 03:45:54.000000 turning_points-0.0.2/README.md
--rw-rw-rw-   0        0        0     1261 2024-04-05 04:26:07.000000 turning_points-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 04:26:11.761201 turning_points-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      673 2024-04-05 04:26:07.000000 turning_points-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 04:26:11.750194 turning_points-0.0.2/tests/
--rw-rw-rw-   0        0        0      325 2024-04-05 03:35:58.000000 turning_points-0.0.2/tests/test_turning_point_analyzer.py
-drwxrwxrwx   0        0        0        0 2024-04-05 04:26:11.758207 turning_points-0.0.2/turning_points.egg-info/
--rw-rw-rw-   0        0        0     3313 2024-04-05 04:26:11.000000 turning_points-0.0.2/turning_points.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2024-04-05 04:26:11.000000 turning_points-0.0.2/turning_points.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 04:26:11.000000 turning_points-0.0.2/turning_points.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      339 2024-04-05 04:26:11.000000 turning_points-0.0.2/turning_points.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 04:26:11.000000 turning_points-0.0.2/turning_points.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 04:39:15.554109 turning_points-0.0.3/
+-rw-rw-rw-   0        0        0     1070 2024-04-05 03:12:32.000000 turning_points-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3313 2024-04-05 04:39:15.553108 turning_points-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1898 2024-04-05 03:45:54.000000 turning_points-0.0.3/README.md
+-rw-rw-rw-   0        0        0     1261 2024-04-05 04:37:56.000000 turning_points-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 04:39:15.554109 turning_points-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      703 2024-04-05 04:37:56.000000 turning_points-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:39:15.535081 turning_points-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 04:39:15.552108 turning_points-0.0.3/src/turning_points.egg-info/
+-rw-rw-rw-   0        0        0     3313 2024-04-05 04:39:15.000000 turning_points-0.0.3/src/turning_points.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2024-04-05 04:39:15.000000 turning_points-0.0.3/src/turning_points.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 04:39:15.000000 turning_points-0.0.3/src/turning_points.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      339 2024-04-05 04:39:15.000000 turning_points-0.0.3/src/turning_points.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 04:39:15.000000 turning_points-0.0.3/src/turning_points.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 04:39:15.550108 turning_points-0.0.3/tests/
+-rw-rw-rw-   0        0        0      325 2024-04-05 03:35:58.000000 turning_points-0.0.3/tests/test_turning_point_analyzer.py
```

### Comparing `turning_points-0.0.2/LICENSE` & `turning_points-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `turning_points-0.0.2/PKG-INFO` & `turning_points-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turning_points
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package to find turing points in tracks, andd plot
 Home-page: https://github.com/lesptizami/turning_points
 Author: Your Name
 Author-email: Charles Fosseprez <charles.fosseprez.me@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/lesptizami/turning_points
 Project-URL: Issues, https://github.com/lesptizami/turning_points/issues
```

### Comparing `turning_points-0.0.2/README.md` & `turning_points-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `turning_points-0.0.2/pyproject.toml` & `turning_points-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "turning_points"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Charles Fosseprez", email="charles.fosseprez.me@gmail.com" },
 ]
 description = "A package to find turing points in tracks, andd plot"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `turning_points-0.0.2/setup.py` & `turning_points-0.0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='turning_point_analyzer',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'scipy',
         'matplotlib',
     ],
     author='Your Name',
@@ -15,9 +15,10 @@
     url='https://github.com/lesptizami/turning_points',
     python_requires='>=3.6',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
+    package_dir={'': 'src'},
 
 )
```

### Comparing `turning_points-0.0.2/turning_points.egg-info/PKG-INFO` & `turning_points-0.0.3/src/turning_points.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turning_points
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package to find turing points in tracks, andd plot
 Home-page: https://github.com/lesptizami/turning_points
 Author: Your Name
 Author-email: Charles Fosseprez <charles.fosseprez.me@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/lesptizami/turning_points
 Project-URL: Issues, https://github.com/lesptizami/turning_points/issues
```

