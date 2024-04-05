# Comparing `tmp/icutil_IGNchinmay-0.0.2.tar.gz` & `tmp/icutil_IGNchinmay-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icutil_IGNchinmay-0.0.2.tar", last modified: Fri Apr  5 05:50:57 2024, max compression
+gzip compressed data, was "icutil_IGNchinmay-0.0.3.tar", last modified: Fri Apr  5 06:15:46 2024, max compression
```

## Comparing `icutil_IGNchinmay-0.0.2.tar` & `icutil_IGNchinmay-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:57.934367 icutil_IGNchinmay-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 05:50:52.000000 icutil_IGNchinmay-0.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-05 05:50:57.934367 icutil_IGNchinmay-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 05:50:52.000000 icutil_IGNchinmay-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:57.930367 icutil_IGNchinmay-0.0.2/icutil_IGNchinmay/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-05 05:50:52.000000 icutil_IGNchinmay-0.0.2/icutil_IGNchinmay/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9800 2024-04-05 05:50:52.000000 icutil_IGNchinmay-0.0.2/icutil_IGNchinmay/draw_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-05 05:50:52.000000 icutil_IGNchinmay-0.0.2/icutil_IGNchinmay/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-05 05:50:52.000000 icutil_IGNchinmay-0.0.2/icutil_IGNchinmay/typehint_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:57.934367 icutil_IGNchinmay-0.0.2/icutil_IGNchinmay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-05 05:50:57.000000 icutil_IGNchinmay-0.0.2/icutil_IGNchinmay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-05 05:50:57.000000 icutil_IGNchinmay-0.0.2/icutil_IGNchinmay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 05:50:57.000000 icutil_IGNchinmay-0.0.2/icutil_IGNchinmay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-05 05:50:57.000000 icutil_IGNchinmay-0.0.2/icutil_IGNchinmay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 05:50:57.000000 icutil_IGNchinmay-0.0.2/icutil_IGNchinmay.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-05 05:50:52.000000 icutil_IGNchinmay-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-05 05:50:52.000000 icutil_IGNchinmay-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 05:50:57.934367 icutil_IGNchinmay-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:57.934367 icutil_IGNchinmay-0.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-05 05:50:52.000000 icutil_IGNchinmay-0.0.2/test/test_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:15:46.748992 icutil_IGNchinmay-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 06:15:35.000000 icutil_IGNchinmay-0.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-05 06:15:46.748992 icutil_IGNchinmay-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 06:15:35.000000 icutil_IGNchinmay-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:15:46.748992 icutil_IGNchinmay-0.0.3/icutil_IGNchinmay/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-05 06:15:35.000000 icutil_IGNchinmay-0.0.3/icutil_IGNchinmay/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9800 2024-04-05 06:15:35.000000 icutil_IGNchinmay-0.0.3/icutil_IGNchinmay/draw_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-05 06:15:35.000000 icutil_IGNchinmay-0.0.3/icutil_IGNchinmay/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-05 06:15:35.000000 icutil_IGNchinmay-0.0.3/icutil_IGNchinmay/typehint_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:15:46.748992 icutil_IGNchinmay-0.0.3/icutil_IGNchinmay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-05 06:15:46.000000 icutil_IGNchinmay-0.0.3/icutil_IGNchinmay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-05 06:15:46.000000 icutil_IGNchinmay-0.0.3/icutil_IGNchinmay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 06:15:46.000000 icutil_IGNchinmay-0.0.3/icutil_IGNchinmay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-05 06:15:46.000000 icutil_IGNchinmay-0.0.3/icutil_IGNchinmay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 06:15:46.000000 icutil_IGNchinmay-0.0.3/icutil_IGNchinmay.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-05 06:15:35.000000 icutil_IGNchinmay-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-05 06:15:35.000000 icutil_IGNchinmay-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 06:15:46.748992 icutil_IGNchinmay-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:15:46.748992 icutil_IGNchinmay-0.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-05 06:15:35.000000 icutil_IGNchinmay-0.0.3/test/test_json.py
```

### Comparing `icutil_IGNchinmay-0.0.2/LICENSE.txt` & `icutil_IGNchinmay-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `icutil_IGNchinmay-0.0.2/PKG-INFO` & `icutil_IGNchinmay-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icutil_IGNchinmay
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small CV test package
 Author-email: Chinmay <chinmayananda.sahu@ignitarium.com>
 Project-URL: Homepage, https://github.com/IGNchinmay/PypiPublishTest
 Project-URL: Issues, https://github.com/IGNchinmay/PypiPublishTest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,22 +14,20 @@
 Requires-Dist: docker
 Requires-Dist: easyprocess
 Requires-Dist: fabulous
 Requires-Dist: imgaug
 Requires-Dist: loguru
 Requires-Dist: lsb_release_ex
 Requires-Dist: matplotlib
-Requires-Dist: numpy==1.23.0
 Requires-Dist: opencv-python
 Requires-Dist: pandas
 Requires-Dist: Pillow
 Requires-Dist: pandas
 Requires-Dist: pynput
 Requires-Dist: scikit-image
-Requires-Dist: setuptools
 Requires-Dist: shapely
 Requires-Dist: sympy
 Requires-Dist: termcolor
 
 # icutils
 
 A sample test package
```

### Comparing `icutil_IGNchinmay-0.0.2/icutil_IGNchinmay/draw_utils.py` & `icutil_IGNchinmay-0.0.3/icutil_IGNchinmay/draw_utils.py`

 * *Files identical despite different names*

### Comparing `icutil_IGNchinmay-0.0.2/icutil_IGNchinmay/json_utils.py` & `icutil_IGNchinmay-0.0.3/icutil_IGNchinmay/json_utils.py`

 * *Files identical despite different names*

### Comparing `icutil_IGNchinmay-0.0.2/icutil_IGNchinmay/typehint_utils.py` & `icutil_IGNchinmay-0.0.3/icutil_IGNchinmay/typehint_utils.py`

 * *Files identical despite different names*

### Comparing `icutil_IGNchinmay-0.0.2/icutil_IGNchinmay.egg-info/PKG-INFO` & `icutil_IGNchinmay-0.0.3/icutil_IGNchinmay.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icutil_IGNchinmay
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small CV test package
 Author-email: Chinmay <chinmayananda.sahu@ignitarium.com>
 Project-URL: Homepage, https://github.com/IGNchinmay/PypiPublishTest
 Project-URL: Issues, https://github.com/IGNchinmay/PypiPublishTest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,22 +14,20 @@
 Requires-Dist: docker
 Requires-Dist: easyprocess
 Requires-Dist: fabulous
 Requires-Dist: imgaug
 Requires-Dist: loguru
 Requires-Dist: lsb_release_ex
 Requires-Dist: matplotlib
-Requires-Dist: numpy==1.23.0
 Requires-Dist: opencv-python
 Requires-Dist: pandas
 Requires-Dist: Pillow
 Requires-Dist: pandas
 Requires-Dist: pynput
 Requires-Dist: scikit-image
-Requires-Dist: setuptools
 Requires-Dist: shapely
 Requires-Dist: sympy
 Requires-Dist: termcolor
 
 # icutils
 
 A sample test package
```

### Comparing `icutil_IGNchinmay-0.0.2/pyproject.toml` & `icutil_IGNchinmay-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "icutil_IGNchinmay"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Chinmay", email="chinmayananda.sahu@ignitarium.com" },
 ]
 description = "A small CV test package"
 readme = "README.md"
 requires-python = ">=3.8"
 dynamic = ["dependencies"]              #used for requiremnts.txt file
```

