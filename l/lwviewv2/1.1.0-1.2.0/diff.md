# Comparing `tmp/lwviewv2-1.1.0.tar.gz` & `tmp/lwviewv2-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lwviewv2-1.1.0.tar", last modified: Tue Mar 19 18:02:01 2024, max compression
+gzip compressed data, was "lwviewv2-1.2.0.tar", last modified: Fri Apr  5 12:47:11 2024, max compression
```

## Comparing `lwviewv2-1.1.0.tar` & `lwviewv2-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 tk928      (502) staff       (20)        0 2024-03-19 18:02:01.674629 lwviewv2-1.1.0/
--rw-r--r--   0 tk928      (502) staff       (20)      618 2024-03-19 18:02:01.674398 lwviewv2-1.1.0/PKG-INFO
-drwxr-xr-x   0 tk928      (502) staff       (20)        0 2024-03-19 18:02:01.674108 lwviewv2-1.1.0/lwviewv2.egg-info/
--rw-r--r--   0 tk928      (502) staff       (20)      618 2024-03-19 18:02:01.000000 lwviewv2-1.1.0/lwviewv2.egg-info/PKG-INFO
--rw-r--r--   0 tk928      (502) staff       (20)      198 2024-03-19 18:02:01.000000 lwviewv2-1.1.0/lwviewv2.egg-info/SOURCES.txt
--rw-r--r--   0 tk928      (502) staff       (20)        1 2024-03-19 18:02:01.000000 lwviewv2-1.1.0/lwviewv2.egg-info/dependency_links.txt
--rw-r--r--   0 tk928      (502) staff       (20)        1 2024-03-19 17:22:03.000000 lwviewv2-1.1.0/lwviewv2.egg-info/not-zip-safe
--rw-r--r--   0 tk928      (502) staff       (20)       37 2024-03-19 18:02:01.000000 lwviewv2-1.1.0/lwviewv2.egg-info/requires.txt
--rw-r--r--   0 tk928      (502) staff       (20)        1 2024-03-19 18:02:01.000000 lwviewv2-1.1.0/lwviewv2.egg-info/top_level.txt
--rw-r--r--   0 tk928      (502) staff       (20)       38 2024-03-19 18:02:01.674685 lwviewv2-1.1.0/setup.cfg
--rw-r--r--   0 tk928      (502) staff       (20)      894 2024-03-19 17:17:48.000000 lwviewv2-1.1.0/setup.py
+drwxr-xr-x   0 tk928      (502) staff       (20)        0 2024-04-05 12:47:11.029227 lwviewv2-1.2.0/
+-rw-r--r--   0 tk928      (502) staff       (20)      618 2024-04-05 12:47:11.028918 lwviewv2-1.2.0/PKG-INFO
+drwxr-xr-x   0 tk928      (502) staff       (20)        0 2024-04-05 12:47:11.028431 lwviewv2-1.2.0/lwviewv2.egg-info/
+-rw-r--r--   0 tk928      (502) staff       (20)      618 2024-04-05 12:47:10.000000 lwviewv2-1.2.0/lwviewv2.egg-info/PKG-INFO
+-rw-r--r--   0 tk928      (502) staff       (20)      198 2024-04-05 12:47:11.000000 lwviewv2-1.2.0/lwviewv2.egg-info/SOURCES.txt
+-rw-r--r--   0 tk928      (502) staff       (20)        1 2024-04-05 12:47:10.000000 lwviewv2-1.2.0/lwviewv2.egg-info/dependency_links.txt
+-rw-r--r--   0 tk928      (502) staff       (20)        1 2024-03-19 17:22:03.000000 lwviewv2-1.2.0/lwviewv2.egg-info/not-zip-safe
+-rw-r--r--   0 tk928      (502) staff       (20)       37 2024-04-05 12:47:11.000000 lwviewv2-1.2.0/lwviewv2.egg-info/requires.txt
+-rw-r--r--   0 tk928      (502) staff       (20)        1 2024-04-05 12:47:11.000000 lwviewv2-1.2.0/lwviewv2.egg-info/top_level.txt
+-rw-r--r--   0 tk928      (502) staff       (20)       38 2024-04-05 12:47:11.029287 lwviewv2-1.2.0/setup.cfg
+-rw-r--r--   0 tk928      (502) staff       (20)      894 2024-04-05 12:45:24.000000 lwviewv2-1.2.0/setup.py
```

### Comparing `lwviewv2-1.1.0/PKG-INFO` & `lwviewv2-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lwviewv2
-Version: 1.1.0
+Version: 1.2.0
 Summary: Viewer of images in python.
 Home-page: https://github.com/ReubenDo/lightweight-viewer
 Author: Sandy Wells
 Author-email: sw@bwh.harvard.edu
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `lwviewv2-1.1.0/lwviewv2.egg-info/PKG-INFO` & `lwviewv2-1.2.0/lwviewv2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lwviewv2
-Version: 1.1.0
+Version: 1.2.0
 Summary: Viewer of images in python.
 Home-page: https://github.com/ReubenDo/lightweight-viewer
 Author: Sandy Wells
 Author-email: sw@bwh.harvard.edu
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `lwviewv2-1.1.0/setup.py` & `lwviewv2-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 
 setup(name='lwviewv2',
-        version='1.1.0',
+        version='1.2.0',
         description='Viewer of images in python.',
         long_description="See Readme.md on github for more details.",
         url='https://github.com/ReubenDo/lightweight-viewer',
         author='Sandy Wells',
         author_email='sw@bwh.harvard.edu',
         python_requires='>=3.9',
         license='MIT',
```

