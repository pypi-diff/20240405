# Comparing `tmp/asbe-0.1.3.tar.gz` & `tmp/asbe-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asbe-0.1.3.tar", last modified: Mon Nov 20 19:29:29 2023, max compression
+gzip compressed data, was "asbe-0.1.4.tar", last modified: Fri Apr  5 07:39:48 2024, max compression
```

## Comparing `asbe-0.1.3.tar` & `asbe-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 zoltan     (501) staff       (20)        0 2023-11-20 19:29:29.496695 asbe-0.1.3/
--rw-r--r--   0 zoltan     (501) staff       (20)     2348 2023-11-17 16:47:45.000000 asbe-0.1.3/CONTRIBUTING.md
--rw-r--r--   0 zoltan     (501) staff       (20)    11357 2023-11-17 16:47:45.000000 asbe-0.1.3/LICENSE
--rw-r--r--   0 zoltan     (501) staff       (20)      111 2023-11-17 16:47:45.000000 asbe-0.1.3/MANIFEST.in
--rw-r--r--   0 zoltan     (501) staff       (20)     5399 2023-11-20 19:29:29.496178 asbe-0.1.3/PKG-INFO
--rw-r--r--   0 zoltan     (501) staff       (20)     4509 2023-11-20 19:05:38.000000 asbe-0.1.3/README.md
-drwxr-xr-x   0 zoltan     (501) staff       (20)        0 2023-11-20 19:29:29.492973 asbe-0.1.3/asbe/
--rw-r--r--   0 zoltan     (501) staff       (20)       22 2023-11-20 19:28:46.000000 asbe-0.1.3/asbe/__init__.py
--rw-r--r--   0 zoltan     (501) staff       (20)    11033 2023-11-20 19:28:46.000000 asbe-0.1.3/asbe/_modidx.py
--rw-r--r--   0 zoltan     (501) staff       (20)     1340 2023-11-17 16:47:45.000000 asbe-0.1.3/asbe/_nbdev.py
--rw-r--r--   0 zoltan     (501) staff       (20)    33680 2023-11-20 19:28:46.000000 asbe-0.1.3/asbe/base.py
--rw-r--r--   0 zoltan     (501) staff       (20)    14266 2023-11-17 16:47:45.000000 asbe-0.1.3/asbe/core.py
--rw-r--r--   0 zoltan     (501) staff       (20)     3409 2023-11-20 19:28:46.000000 asbe-0.1.3/asbe/estimators.py
--rw-r--r--   0 zoltan     (501) staff       (20)     3180 2023-11-20 19:28:46.000000 asbe-0.1.3/asbe/helper.py
--rw-r--r--   0 zoltan     (501) staff       (20)     7838 2023-11-20 19:28:46.000000 asbe-0.1.3/asbe/models.py
-drwxr-xr-x   0 zoltan     (501) staff       (20)        0 2023-11-20 19:29:29.495682 asbe-0.1.3/asbe.egg-info/
--rw-r--r--   0 zoltan     (501) staff       (20)     5399 2023-11-20 19:29:29.000000 asbe-0.1.3/asbe.egg-info/PKG-INFO
--rw-r--r--   0 zoltan     (501) staff       (20)      387 2023-11-20 19:29:29.000000 asbe-0.1.3/asbe.egg-info/SOURCES.txt
--rw-r--r--   0 zoltan     (501) staff       (20)        1 2023-11-20 19:29:29.000000 asbe-0.1.3/asbe.egg-info/dependency_links.txt
--rw-r--r--   0 zoltan     (501) staff       (20)       30 2023-11-20 19:29:29.000000 asbe-0.1.3/asbe.egg-info/entry_points.txt
--rw-r--r--   0 zoltan     (501) staff       (20)        1 2023-11-17 16:48:09.000000 asbe-0.1.3/asbe.egg-info/not-zip-safe
--rw-r--r--   0 zoltan     (501) staff       (20)       94 2023-11-20 19:29:29.000000 asbe-0.1.3/asbe.egg-info/requires.txt
--rw-r--r--   0 zoltan     (501) staff       (20)        5 2023-11-20 19:29:29.000000 asbe-0.1.3/asbe.egg-info/top_level.txt
--rw-r--r--   0 zoltan     (501) staff       (20)      894 2023-11-20 19:28:46.000000 asbe-0.1.3/settings.ini
--rw-r--r--   0 zoltan     (501) staff       (20)       38 2023-11-20 19:29:29.496788 asbe-0.1.3/setup.cfg
--rw-r--r--   0 zoltan     (501) staff       (20)     2541 2023-11-17 16:47:45.000000 asbe-0.1.3/setup.py
+drwxr-xr-x   0 zpuha      (501) staff       (20)        0 2024-04-05 07:39:48.169399 asbe-0.1.4/
+-rw-r--r--   0 zpuha      (501) staff       (20)     2348 2023-11-16 23:06:51.000000 asbe-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0 zpuha      (501) staff       (20)    35149 2024-03-25 19:58:59.000000 asbe-0.1.4/LICENSE
+-rw-r--r--   0 zpuha      (501) staff       (20)      111 2023-11-16 23:06:51.000000 asbe-0.1.4/MANIFEST.in
+-rw-r--r--   0 zpuha      (501) staff       (20)     5454 2024-04-05 07:39:48.168797 asbe-0.1.4/PKG-INFO
+-rw-r--r--   0 zpuha      (501) staff       (20)     4509 2024-03-25 19:58:59.000000 asbe-0.1.4/README.md
+drwxr-xr-x   0 zpuha      (501) staff       (20)        0 2024-04-05 07:39:48.164970 asbe-0.1.4/asbe/
+-rw-r--r--   0 zpuha      (501) staff       (20)       22 2024-03-25 19:58:59.000000 asbe-0.1.4/asbe/__init__.py
+-rw-r--r--   0 zpuha      (501) staff       (20)    11033 2024-03-25 19:58:59.000000 asbe-0.1.4/asbe/_modidx.py
+-rw-r--r--   0 zpuha      (501) staff       (20)     1340 2023-11-16 23:06:51.000000 asbe-0.1.4/asbe/_nbdev.py
+-rw-r--r--   0 zpuha      (501) staff       (20)    33680 2024-03-25 19:58:59.000000 asbe-0.1.4/asbe/base.py
+-rw-r--r--   0 zpuha      (501) staff       (20)    14266 2023-11-16 23:06:51.000000 asbe-0.1.4/asbe/core.py
+-rw-r--r--   0 zpuha      (501) staff       (20)     3409 2024-03-25 19:58:59.000000 asbe-0.1.4/asbe/estimators.py
+-rw-r--r--   0 zpuha      (501) staff       (20)     3180 2023-11-17 08:24:57.000000 asbe-0.1.4/asbe/helper.py
+-rw-r--r--   0 zpuha      (501) staff       (20)     7838 2024-03-25 19:58:59.000000 asbe-0.1.4/asbe/models.py
+drwxr-xr-x   0 zpuha      (501) staff       (20)        0 2024-04-05 07:39:48.167945 asbe-0.1.4/asbe.egg-info/
+-rw-r--r--   0 zpuha      (501) staff       (20)     5454 2024-04-05 07:39:48.000000 asbe-0.1.4/asbe.egg-info/PKG-INFO
+-rw-r--r--   0 zpuha      (501) staff       (20)      387 2024-04-05 07:39:48.000000 asbe-0.1.4/asbe.egg-info/SOURCES.txt
+-rw-r--r--   0 zpuha      (501) staff       (20)        1 2024-04-05 07:39:48.000000 asbe-0.1.4/asbe.egg-info/dependency_links.txt
+-rw-r--r--   0 zpuha      (501) staff       (20)       30 2024-04-05 07:39:48.000000 asbe-0.1.4/asbe.egg-info/entry_points.txt
+-rw-r--r--   0 zpuha      (501) staff       (20)        1 2023-11-16 23:09:16.000000 asbe-0.1.4/asbe.egg-info/not-zip-safe
+-rw-r--r--   0 zpuha      (501) staff       (20)      138 2024-04-05 07:39:48.000000 asbe-0.1.4/asbe.egg-info/requires.txt
+-rw-r--r--   0 zpuha      (501) staff       (20)        5 2024-04-05 07:39:48.000000 asbe-0.1.4/asbe.egg-info/top_level.txt
+-rw-r--r--   0 zpuha      (501) staff       (20)      939 2024-04-05 07:39:09.000000 asbe-0.1.4/settings.ini
+-rw-r--r--   0 zpuha      (501) staff       (20)       38 2024-04-05 07:39:48.169470 asbe-0.1.4/setup.cfg
+-rw-r--r--   0 zpuha      (501) staff       (20)     2541 2023-11-16 23:06:51.000000 asbe-0.1.4/setup.py
```

### Comparing `asbe-0.1.3/CONTRIBUTING.md` & `asbe-0.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `asbe-0.1.3/PKG-INFO` & `asbe-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: asbe
-Version: 0.1.3
+Version: 0.1.4
 Summary: Active Learning for treatment effect estimation
 Home-page: https://github.com/puhazoli/asbe/
 Author: puhazoli
 Author-email: puha.zoli@gmail.com
 License: Apache Software License 2.0
 Keywords: active learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: scikit-learn
-Requires-Dist: pandas
+Requires-Dist: numpy>=1.20
+Requires-Dist: scikit-learn>=1.2
+Requires-Dist: pandas>=2.0
 Requires-Dist: matplotlib
 Requires-Dist: pylift
 Requires-Dist: econml
 Requires-Dist: scikit-uplift
 Requires-Dist: pymc-bart>=0.5.2
 Requires-Dist: pymc
+Requires-Dist: fastcore
+Requires-Dist: xbart
+Requires-Dist: gpy
+Requires-Dist: pyopenbt
 Provides-Extra: dev
 
 Automatic Stopping for Batch-mode Experimentation
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
```

### Comparing `asbe-0.1.3/README.md` & `asbe-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `asbe-0.1.3/asbe/_modidx.py` & `asbe-0.1.4/asbe/_modidx.py`

 * *Files identical despite different names*

### Comparing `asbe-0.1.3/asbe/_nbdev.py` & `asbe-0.1.4/asbe/_nbdev.py`

 * *Files identical despite different names*

### Comparing `asbe-0.1.3/asbe/base.py` & `asbe-0.1.4/asbe/base.py`

 * *Files identical despite different names*

### Comparing `asbe-0.1.3/asbe/core.py` & `asbe-0.1.4/asbe/core.py`

 * *Files identical despite different names*

### Comparing `asbe-0.1.3/asbe/estimators.py` & `asbe-0.1.4/asbe/estimators.py`

 * *Files identical despite different names*

### Comparing `asbe-0.1.3/asbe/helper.py` & `asbe-0.1.4/asbe/helper.py`

 * *Files identical despite different names*

### Comparing `asbe-0.1.3/asbe/models.py` & `asbe-0.1.4/asbe/models.py`

 * *Files identical despite different names*

### Comparing `asbe-0.1.3/asbe.egg-info/PKG-INFO` & `asbe-0.1.4/asbe.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: asbe
-Version: 0.1.3
+Version: 0.1.4
 Summary: Active Learning for treatment effect estimation
 Home-page: https://github.com/puhazoli/asbe/
 Author: puhazoli
 Author-email: puha.zoli@gmail.com
 License: Apache Software License 2.0
 Keywords: active learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: scikit-learn
-Requires-Dist: pandas
+Requires-Dist: numpy>=1.20
+Requires-Dist: scikit-learn>=1.2
+Requires-Dist: pandas>=2.0
 Requires-Dist: matplotlib
 Requires-Dist: pylift
 Requires-Dist: econml
 Requires-Dist: scikit-uplift
 Requires-Dist: pymc-bart>=0.5.2
 Requires-Dist: pymc
+Requires-Dist: fastcore
+Requires-Dist: xbart
+Requires-Dist: gpy
+Requires-Dist: pyopenbt
 Provides-Extra: dev
 
 Automatic Stopping for Batch-mode Experimentation
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
```

### Comparing `asbe-0.1.3/settings.ini` & `asbe-0.1.4/settings.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [DEFAULT]
 lib_name = asbe
-min_python = 3.9
-version = 0.1.3
+min_python = 3.10
+version = 0.1.4
 nbs_path = .
 doc_path = _docs
 recursive = False
 tst_flags = slow
-requirements = numpy scikit-learn pandas matplotlib pylift econml scikit-uplift pymc-bart>=0.5.2 pymc
+requirements = numpy>=1.20 scikit-learn>=1.2 pandas>=2.0 matplotlib pylift econml scikit-uplift pymc-bart>=0.5.2 pymc fastcore xbart gpy pyopenbt
 audience = Science/Research
 author = puhazoli
 author_email = puha.zoli@gmail.com
 copyright = Apache 2.0
 description = Active Learning for treatment effect estimation
 keywords = active learning
 language = English
```

### Comparing `asbe-0.1.3/setup.py` & `asbe-0.1.4/setup.py`

 * *Files identical despite different names*

