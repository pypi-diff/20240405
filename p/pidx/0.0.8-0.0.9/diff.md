# Comparing `tmp/pidx-0.0.8.tar.gz` & `tmp/pidx-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pidx-0.0.8.tar", last modified: Thu Dec 14 13:00:25 2023, max compression
+gzip compressed data, was "pidx-0.0.9.tar", last modified: Thu Dec 14 13:16:44 2023, max compression
```

## Comparing `pidx-0.0.8.tar` & `pidx-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-12-14 13:00:25.260176 pidx-0.0.8/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2023-11-17 15:53:23.000000 pidx-0.0.8/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2023-11-17 15:53:23.000000 pidx-0.0.8/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     4140 2023-12-14 13:00:25.259937 pidx-0.0.8/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     3025 2023-12-12 16:03:42.000000 pidx-0.0.8/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-12-14 13:00:25.258399 pidx-0.0.8/pidx/
--rw-r--r--   0 solst      (501) staff       (20)      441 2023-12-14 13:00:19.000000 pidx-0.0.8/pidx/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)     3540 2023-12-14 13:00:19.000000 pidx-0.0.8/pidx/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)      580 2023-12-14 13:00:19.000000 pidx-0.0.8/pidx/cons.py
--rw-r--r--   0 solst      (501) staff       (20)    22581 2023-12-14 13:00:19.000000 pidx-0.0.8/pidx/idxs.py
--rw-r--r--   0 solst      (501) staff       (20)      976 2023-12-14 13:00:19.000000 pidx-0.0.8/pidx/mock.py
--rw-r--r--   0 solst      (501) staff       (20)     1530 2023-12-12 13:31:47.000000 pidx-0.0.8/pidx/safe.py
--rw-r--r--   0 solst      (501) staff       (20)     5910 2023-12-14 13:00:19.000000 pidx-0.0.8/pidx/util.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-12-14 13:00:25.259381 pidx-0.0.8/pidx.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     4140 2023-12-14 13:00:25.000000 pidx-0.0.8/pidx.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      346 2023-12-14 13:00:25.000000 pidx-0.0.8/pidx.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-12-14 13:00:25.000000 pidx-0.0.8/pidx.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2023-12-14 13:00:25.000000 pidx-0.0.8/pidx.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-11-19 20:58:58.000000 pidx-0.0.8/pidx.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)      125 2023-12-14 13:00:25.000000 pidx-0.0.8/pidx.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2023-12-14 13:00:25.000000 pidx-0.0.8/pidx.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      912 2023-12-13 14:37:35.000000 pidx-0.0.8/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-12-14 13:00:25.260218 pidx-0.0.8/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2585 2023-11-17 15:53:23.000000 pidx-0.0.8/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-12-14 13:16:44.630086 pidx-0.0.9/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2023-11-17 15:53:23.000000 pidx-0.0.9/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2023-11-17 15:53:23.000000 pidx-0.0.9/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     3624 2023-12-14 13:16:44.629947 pidx-0.0.9/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     3025 2023-12-12 16:03:42.000000 pidx-0.0.9/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-12-14 13:16:44.628938 pidx-0.0.9/pidx/
+-rw-r--r--   0 solst      (501) staff       (20)      441 2023-12-14 13:16:32.000000 pidx-0.0.9/pidx/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)     3540 2023-12-14 13:16:32.000000 pidx-0.0.9/pidx/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)      580 2023-12-14 13:16:32.000000 pidx-0.0.9/pidx/cons.py
+-rw-r--r--   0 solst      (501) staff       (20)    22581 2023-12-14 13:16:32.000000 pidx-0.0.9/pidx/idxs.py
+-rw-r--r--   0 solst      (501) staff       (20)      976 2023-12-14 13:16:32.000000 pidx-0.0.9/pidx/mock.py
+-rw-r--r--   0 solst      (501) staff       (20)     1530 2023-12-12 13:31:47.000000 pidx-0.0.9/pidx/safe.py
+-rw-r--r--   0 solst      (501) staff       (20)     5910 2023-12-14 13:16:32.000000 pidx-0.0.9/pidx/util.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-12-14 13:16:44.629761 pidx-0.0.9/pidx.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     3624 2023-12-14 13:16:44.000000 pidx-0.0.9/pidx.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      346 2023-12-14 13:16:44.000000 pidx-0.0.9/pidx.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-12-14 13:16:44.000000 pidx-0.0.9/pidx.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2023-12-14 13:16:44.000000 pidx-0.0.9/pidx.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-11-19 20:58:58.000000 pidx-0.0.9/pidx.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)       81 2023-12-14 13:16:44.000000 pidx-0.0.9/pidx.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2023-12-14 13:16:44.000000 pidx-0.0.9/pidx.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      868 2023-12-14 13:09:50.000000 pidx-0.0.9/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-12-14 13:16:44.630131 pidx-0.0.9/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2585 2023-11-17 15:53:23.000000 pidx-0.0.9/setup.py
```

### Comparing `pidx-0.0.8/LICENSE` & `pidx-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pidx-0.0.8/PKG-INFO` & `pidx-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,25 @@
 Metadata-Version: 2.1
 Name: pidx
-Version: 0.0.8
+Version: 0.0.9
 Summary: In Vitro Fertilization
 Home-page: https://github.com/dsm-72/pidx
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: in vitro fertilization pidx
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: ptyp
-Requires-Dist: atyp
-Requires-Dist: itry
-Requires-Dist: putl
-Requires-Dist: asto
-Requires-Dist: atup
-Requires-Dist: chck
-Requires-Dist: excs
-Requires-Dist: hasr
-Requires-Dist: getr
 Provides-Extra: dev
-Requires-Dist: numpy; extra == "dev"
-Requires-Dist: pandas; extra == "dev"
-Requires-Dist: matplotlib; extra == "dev"
-Requires-Dist: torch; extra == "dev"
-Requires-Dist: pytorch_lightning; extra == "dev"
-Requires-Dist: torchvision; extra == "dev"
-Requires-Dist: cv2; extra == "dev"
-Requires-Dist: PIL; extra == "dev"
+License-File: LICENSE
 
 # pidx
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Developer Guide
```

### Comparing `pidx-0.0.8/README.md` & `pidx-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pidx-0.0.8/pidx/_modidx.py` & `pidx-0.0.9/pidx/_modidx.py`

 * *Files identical despite different names*

### Comparing `pidx-0.0.8/pidx/cons.py` & `pidx-0.0.9/pidx/cons.py`

 * *Files identical despite different names*

### Comparing `pidx-0.0.8/pidx/idxs.py` & `pidx-0.0.9/pidx/idxs.py`

 * *Files identical despite different names*

### Comparing `pidx-0.0.8/pidx/mock.py` & `pidx-0.0.9/pidx/mock.py`

 * *Files identical despite different names*

### Comparing `pidx-0.0.8/pidx/safe.py` & `pidx-0.0.9/pidx/safe.py`

 * *Files identical despite different names*

### Comparing `pidx-0.0.8/pidx/util.py` & `pidx-0.0.9/pidx/util.py`

 * *Files identical despite different names*

### Comparing `pidx-0.0.8/pidx.egg-info/PKG-INFO` & `pidx-0.0.9/pidx.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,25 @@
 Metadata-Version: 2.1
 Name: pidx
-Version: 0.0.8
+Version: 0.0.9
 Summary: In Vitro Fertilization
 Home-page: https://github.com/dsm-72/pidx
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: in vitro fertilization pidx
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: ptyp
-Requires-Dist: atyp
-Requires-Dist: itry
-Requires-Dist: putl
-Requires-Dist: asto
-Requires-Dist: atup
-Requires-Dist: chck
-Requires-Dist: excs
-Requires-Dist: hasr
-Requires-Dist: getr
 Provides-Extra: dev
-Requires-Dist: numpy; extra == "dev"
-Requires-Dist: pandas; extra == "dev"
-Requires-Dist: matplotlib; extra == "dev"
-Requires-Dist: torch; extra == "dev"
-Requires-Dist: pytorch_lightning; extra == "dev"
-Requires-Dist: torchvision; extra == "dev"
-Requires-Dist: cv2; extra == "dev"
-Requires-Dist: PIL; extra == "dev"
+License-File: LICENSE
 
 # pidx
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Developer Guide
```

### Comparing `pidx-0.0.8/settings.ini` & `pidx-0.0.9/settings.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = pidx
 lib_name = pidx
-version = 0.0.8
+version = 0.0.9
 min_python = 3.11
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = pidx
 nbs_path = nbs
 recursive = True
@@ -30,9 +30,9 @@
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 requirements = ptyp atyp itry putl asto atup chck excs hasr getr
-dev_requirements = numpy pandas matplotlib torch pytorch_lightning torchvision cv2 PIL
+dev_requirements = numpy pandas matplotlib
```

### Comparing `pidx-0.0.8/setup.py` & `pidx-0.0.9/setup.py`

 * *Files identical despite different names*

