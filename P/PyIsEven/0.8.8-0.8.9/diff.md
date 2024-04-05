# Comparing `tmp/PyIsEven-0.8.8.tar.gz` & `tmp/PyIsEven-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyIsEven-0.8.8.tar", last modified: Thu Aug 12 23:45:29 2021, max compression
+gzip compressed data, was "PyIsEven-0.8.9.tar", last modified: Tue Aug 17 23:13:23 2021, max compression
```

## Comparing `PyIsEven-0.8.8.tar` & `PyIsEven-0.8.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-12 23:45:29.375286 PyIsEven-0.8.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2021-08-12 23:45:18.000000 PyIsEven-0.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1366 2021-08-12 23:45:29.375286 PyIsEven-0.8.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-12 23:45:29.375286 PyIsEven-0.8.8/PyIsEven.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1366 2021-08-12 23:45:29.000000 PyIsEven-0.8.8/PyIsEven.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      403 2021-08-12 23:45:29.000000 PyIsEven-0.8.8/PyIsEven.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-12 23:45:29.000000 PyIsEven-0.8.8/PyIsEven.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2021-08-12 23:45:29.000000 PyIsEven-0.8.8/PyIsEven.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-08-12 23:45:29.000000 PyIsEven-0.8.8/PyIsEven.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      803 2021-08-12 23:45:18.000000 PyIsEven-0.8.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-12 23:45:29.375286 PyIsEven-0.8.8/is_even/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-12 23:45:18.000000 PyIsEven-0.8.8/is_even/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      994 2021-08-12 23:45:18.000000 PyIsEven-0.8.8/is_even/_py2_is_even.py
--rw-r--r--   0 runner    (1001) docker     (121)     1262 2021-08-12 23:45:18.000000 PyIsEven-0.8.8/is_even/_py3_10_is_even.py
--rw-r--r--   0 runner    (1001) docker     (121)     1427 2021-08-12 23:45:18.000000 PyIsEven-0.8.8/is_even/_py3_8_is_even.py
--rw-r--r--   0 runner    (1001) docker     (121)      229 2021-08-12 23:45:18.000000 PyIsEven-0.8.8/is_even/_py3_api_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2021-08-12 23:45:18.000000 PyIsEven-0.8.8/is_even/_py3_is_even.py
--rw-r--r--   0 runner    (1001) docker     (121)       80 2021-08-12 23:45:18.000000 PyIsEven-0.8.8/is_even/_py_api_exception.py
--rw-r--r--   0 runner    (1001) docker     (121)      127 2021-08-12 23:45:18.000000 PyIsEven-0.8.8/is_even/_typings.py
--rw-r--r--   0 runner    (1001) docker     (121)      396 2021-08-12 23:45:18.000000 PyIsEven-0.8.8/is_even/is_even.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-12 23:45:29.375286 PyIsEven-0.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      613 2021-08-12 23:45:18.000000 PyIsEven-0.8.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 23:13:23.663598 PyIsEven-0.8.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2021-08-17 23:13:12.000000 PyIsEven-0.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1366 2021-08-17 23:13:23.663598 PyIsEven-0.8.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 23:13:23.663598 PyIsEven-0.8.9/PyIsEven.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1366 2021-08-17 23:13:23.000000 PyIsEven-0.8.9/PyIsEven.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      403 2021-08-17 23:13:23.000000 PyIsEven-0.8.9/PyIsEven.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-17 23:13:23.000000 PyIsEven-0.8.9/PyIsEven.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2021-08-17 23:13:23.000000 PyIsEven-0.8.9/PyIsEven.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2021-08-17 23:13:23.000000 PyIsEven-0.8.9/PyIsEven.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      803 2021-08-17 23:13:12.000000 PyIsEven-0.8.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 23:13:23.663598 PyIsEven-0.8.9/is_even/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-17 23:13:12.000000 PyIsEven-0.8.9/is_even/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      976 2021-08-17 23:13:12.000000 PyIsEven-0.8.9/is_even/_py2_is_even.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1262 2021-08-17 23:13:12.000000 PyIsEven-0.8.9/is_even/_py3_10_is_even.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1427 2021-08-17 23:13:12.000000 PyIsEven-0.8.9/is_even/_py3_8_is_even.py
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2021-08-17 23:13:12.000000 PyIsEven-0.8.9/is_even/_py3_api_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1100 2021-08-17 23:13:12.000000 PyIsEven-0.8.9/is_even/_py3_is_even.py
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2021-08-17 23:13:12.000000 PyIsEven-0.8.9/is_even/_py_api_exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2021-08-17 23:13:12.000000 PyIsEven-0.8.9/is_even/_typings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      396 2021-08-17 23:13:12.000000 PyIsEven-0.8.9/is_even/is_even.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-17 23:13:23.663598 PyIsEven-0.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      613 2021-08-17 23:13:12.000000 PyIsEven-0.8.9/setup.py
```

### Comparing `PyIsEven-0.8.8/LICENSE` & `PyIsEven-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyIsEven-0.8.8/PKG-INFO` & `PyIsEven-0.8.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyIsEven
-Version: 0.8.8
+Version: 0.8.9
 Summary: Check is a integer is even
 Home-page: https://github.com/rosineygp/PyIsEven
 Author: Rosiney Gomes Pereira
 License: MIT
 Description: # Is Even
         
         ![PyPI - Downloads](https://img.shields.io/pypi/dm/PyIsEven)
```

### Comparing `PyIsEven-0.8.8/PyIsEven.egg-info/PKG-INFO` & `PyIsEven-0.8.9/PyIsEven.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyIsEven
-Version: 0.8.8
+Version: 0.8.9
 Summary: Check is a integer is even
 Home-page: https://github.com/rosineygp/PyIsEven
 Author: Rosiney Gomes Pereira
 License: MIT
 Description: # Is Even
         
         ![PyPI - Downloads](https://img.shields.io/pypi/dm/PyIsEven)
```

### Comparing `PyIsEven-0.8.8/README.md` & `PyIsEven-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `PyIsEven-0.8.8/is_even/_py2_is_even.py` & `PyIsEven-0.8.9/is_even/_py2_is_even.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from ._py_api_exception import IsEvenException
 
 
 class IsEven(int):
     def __new__(cls, value, ad):
         cls.ad = ad
         cls.value = value
-        return int.__new__(cls, bool(value))
+        return bool(value)
 
     def __repr__(self):
         return str(bool(self.value))
 
 
 def is_even(number):
     n = _positive(number)
```

### Comparing `PyIsEven-0.8.8/is_even/_py3_10_is_even.py` & `PyIsEven-0.8.9/is_even/_py3_10_is_even.py`

 * *Files identical despite different names*

### Comparing `PyIsEven-0.8.8/is_even/_py3_8_is_even.py` & `PyIsEven-0.8.9/is_even/_py3_8_is_even.py`

 * *Files identical despite different names*

### Comparing `PyIsEven-0.8.8/is_even/_py3_is_even.py` & `PyIsEven-0.8.9/is_even/_py3_is_even.py`

 * *Files identical despite different names*

### Comparing `PyIsEven-0.8.8/setup.py` & `PyIsEven-0.8.9/setup.py`

 * *Files identical despite different names*

