# Comparing `tmp/chck-0.0.8.tar.gz` & `tmp/chck-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chck-0.0.8.tar", last modified: Thu Oct 12 14:31:58 2023, max compression
+gzip compressed data, was "chck-0.0.9.tar", last modified: Thu Oct 19 20:42:46 2023, max compression
```

## Comparing `chck-0.0.8.tar` & `chck-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-10-12 14:31:58.103730 chck-0.0.8/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2023-10-08 12:24:31.000000 chck-0.0.8/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2023-10-08 12:24:31.000000 chck-0.0.8/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     2038 2023-10-12 14:31:58.103607 chck-0.0.8/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     1431 2023-10-08 13:14:58.000000 chck-0.0.8/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-10-12 14:31:58.102345 chck-0.0.8/chck/
--rw-r--r--   0 solst      (501) staff       (20)      281 2023-10-12 14:31:55.000000 chck-0.0.8/chck/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)     4441 2023-10-12 14:31:55.000000 chck-0.0.8/chck/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)      731 2023-10-12 14:31:55.000000 chck-0.0.8/chck/bool.py
--rw-r--r--   0 solst      (501) staff       (20)      606 2023-10-12 14:31:55.000000 chck-0.0.8/chck/comp.py
--rw-r--r--   0 solst      (501) staff       (20)     1776 2023-10-12 14:31:55.000000 chck-0.0.8/chck/core.py
--rw-r--r--   0 solst      (501) staff       (20)      371 2023-10-12 14:31:55.000000 chck-0.0.8/chck/dcls.py
--rw-r--r--   0 solst      (501) staff       (20)     1619 2023-10-12 14:31:55.000000 chck-0.0.8/chck/insp.py
--rw-r--r--   0 solst      (501) staff       (20)      478 2023-10-12 14:31:55.000000 chck-0.0.8/chck/isad.py
--rw-r--r--   0 solst      (501) staff       (20)      719 2023-10-12 14:31:55.000000 chck-0.0.8/chck/isnp.py
--rw-r--r--   0 solst      (501) staff       (20)      968 2023-10-12 14:31:55.000000 chck-0.0.8/chck/ispd.py
--rw-r--r--   0 solst      (501) staff       (20)      896 2023-10-12 14:31:55.000000 chck-0.0.8/chck/misc.py
--rw-r--r--   0 solst      (501) staff       (20)      868 2023-10-12 14:31:55.000000 chck-0.0.8/chck/path.py
--rw-r--r--   0 solst      (501) staff       (20)      782 2023-10-12 14:31:55.000000 chck-0.0.8/chck/strs.py
--rw-r--r--   0 solst      (501) staff       (20)     1885 2023-10-12 14:31:55.000000 chck-0.0.8/chck/trch.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-10-12 14:31:58.103397 chck-0.0.8/chck.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     2038 2023-10-12 14:31:58.000000 chck-0.0.8/chck.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      437 2023-10-12 14:31:58.000000 chck-0.0.8/chck.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-10-12 14:31:58.000000 chck-0.0.8/chck.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2023-10-12 14:31:58.000000 chck-0.0.8/chck.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-10-08 13:15:01.000000 chck-0.0.8/chck.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)        7 2023-10-12 14:31:58.000000 chck-0.0.8/chck.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2023-10-12 14:31:58.000000 chck-0.0.8/chck.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      768 2023-10-12 14:31:22.000000 chck-0.0.8/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-10-12 14:31:58.103774 chck-0.0.8/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2580 2023-10-08 12:24:31.000000 chck-0.0.8/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-10-19 20:42:46.166283 chck-0.0.9/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2023-10-08 12:24:31.000000 chck-0.0.9/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2023-10-08 12:24:31.000000 chck-0.0.9/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     2038 2023-10-19 20:42:46.166144 chck-0.0.9/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1431 2023-10-08 13:14:58.000000 chck-0.0.9/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-10-19 20:42:46.165025 chck-0.0.9/chck/
+-rw-r--r--   0 solst      (501) staff       (20)      281 2023-10-19 20:42:34.000000 chck-0.0.9/chck/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)     5228 2023-10-19 20:42:34.000000 chck-0.0.9/chck/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)      731 2023-10-19 20:42:34.000000 chck-0.0.9/chck/bool.py
+-rw-r--r--   0 solst      (501) staff       (20)      606 2023-10-19 20:42:34.000000 chck-0.0.9/chck/comp.py
+-rw-r--r--   0 solst      (501) staff       (20)     1776 2023-10-19 20:42:34.000000 chck-0.0.9/chck/core.py
+-rw-r--r--   0 solst      (501) staff       (20)      371 2023-10-19 20:42:34.000000 chck-0.0.9/chck/dcls.py
+-rw-r--r--   0 solst      (501) staff       (20)     1619 2023-10-19 20:42:34.000000 chck-0.0.9/chck/insp.py
+-rw-r--r--   0 solst      (501) staff       (20)      478 2023-10-19 20:42:34.000000 chck-0.0.9/chck/isad.py
+-rw-r--r--   0 solst      (501) staff       (20)      719 2023-10-19 20:42:34.000000 chck-0.0.9/chck/isnp.py
+-rw-r--r--   0 solst      (501) staff       (20)      968 2023-10-19 20:42:34.000000 chck-0.0.9/chck/ispd.py
+-rw-r--r--   0 solst      (501) staff       (20)      896 2023-10-19 20:42:34.000000 chck-0.0.9/chck/misc.py
+-rw-r--r--   0 solst      (501) staff       (20)      868 2023-10-19 20:42:34.000000 chck-0.0.9/chck/path.py
+-rw-r--r--   0 solst      (501) staff       (20)     2231 2023-10-19 20:42:34.000000 chck-0.0.9/chck/strs.py
+-rw-r--r--   0 solst      (501) staff       (20)     1885 2023-10-19 20:42:34.000000 chck-0.0.9/chck/trch.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-10-19 20:42:46.165949 chck-0.0.9/chck.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     2038 2023-10-19 20:42:46.000000 chck-0.0.9/chck.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      437 2023-10-19 20:42:46.000000 chck-0.0.9/chck.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-10-19 20:42:46.000000 chck-0.0.9/chck.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2023-10-19 20:42:46.000000 chck-0.0.9/chck.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-10-08 13:15:01.000000 chck-0.0.9/chck.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)        7 2023-10-19 20:42:46.000000 chck-0.0.9/chck.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2023-10-19 20:42:46.000000 chck-0.0.9/chck.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      768 2023-10-12 14:33:15.000000 chck-0.0.9/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-10-19 20:42:46.166325 chck-0.0.9/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2580 2023-10-08 12:24:31.000000 chck-0.0.9/setup.py
```

### Comparing `chck-0.0.8/LICENSE` & `chck-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chck-0.0.8/PKG-INFO` & `chck-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chck
-Version: 0.0.8
+Version: 0.0.9
 Summary: chck
 Home-page: https://github.com/dsm-72/chck
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: chck is question bool type guard typeguard check chck
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chck-0.0.8/README.md` & `chck-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `chck-0.0.8/chck/_modidx.py` & `chck-0.0.9/chck/_modidx.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,15 +40,24 @@
                            'chck.misc.isin': ('misc.html#isin', 'chck/misc.py')},
             'chck.path': { 'chck.path.isdir': ('path.html#isdir', 'chck/path.py'),
                            'chck.path.isfile': ('path.html#isfile', 'chck/path.py'),
                            'chck.path.ispath': ('path.html#ispath', 'chck/path.py'),
                            'chck.path.ispathlike': ('path.html#ispathlike', 'chck/path.py')},
             'chck.strs': { 'chck.strs.isallstr': ('strs.html#isallstr', 'chck/strs.py'),
                            'chck.strs.isdunder': ('strs.html#isdunder', 'chck/strs.py'),
-                           'chck.strs.isnilstr': ('strs.html#isnilstr', 'chck/strs.py')},
+                           'chck.strs.iselps': ('strs.html#iselps', 'chck/strs.py'),
+                           'chck.strs.islower': ('strs.html#islower', 'chck/strs.py'),
+                           'chck.strs.ismangled': ('strs.html#ismangled', 'chck/strs.py'),
+                           'chck.strs.isnilstr': ('strs.html#isnilstr', 'chck/strs.py'),
+                           'chck.strs.isprivate': ('strs.html#isprivate', 'chck/strs.py'),
+                           'chck.strs.ispunc': ('strs.html#ispunc', 'chck/strs.py'),
+                           'chck.strs.isquote': ('strs.html#isquote', 'chck/strs.py'),
+                           'chck.strs.isstar': ('strs.html#isstar', 'chck/strs.py'),
+                           'chck.strs.issunder': ('strs.html#issunder', 'chck/strs.py'),
+                           'chck.strs.isupper': ('strs.html#isupper', 'chck/strs.py')},
             'chck.trch': { 'chck.trch.iscpu': ('trch.html#iscpu', 'chck/trch.py'),
                            'chck.trch.iscputensor': ('trch.html#iscputensor', 'chck/trch.py'),
                            'chck.trch.iscuda': ('trch.html#iscuda', 'chck/trch.py'),
                            'chck.trch.isdevice': ('trch.html#isdevice', 'chck/trch.py'),
                            'chck.trch.ismps': ('trch.html#ismps', 'chck/trch.py'),
                            'chck.trch.ismpstensor': ('trch.html#ismpstensor', 'chck/trch.py'),
                            'chck.trch.istensor': ('trch.html#istensor', 'chck/trch.py')}}}
```

### Comparing `chck-0.0.8/chck/bool.py` & `chck-0.0.9/chck/bool.py`

 * *Files identical despite different names*

### Comparing `chck-0.0.8/chck/comp.py` & `chck-0.0.9/chck/comp.py`

 * *Files identical despite different names*

### Comparing `chck-0.0.8/chck/core.py` & `chck-0.0.9/chck/core.py`

 * *Files identical despite different names*

### Comparing `chck-0.0.8/chck/insp.py` & `chck-0.0.9/chck/insp.py`

 * *Files identical despite different names*

### Comparing `chck-0.0.8/chck/isnp.py` & `chck-0.0.9/chck/isnp.py`

 * *Files identical despite different names*

### Comparing `chck-0.0.8/chck/ispd.py` & `chck-0.0.9/chck/ispd.py`

 * *Files identical despite different names*

### Comparing `chck-0.0.8/chck/misc.py` & `chck-0.0.9/chck/misc.py`

 * *Files identical despite different names*

### Comparing `chck-0.0.8/chck/path.py` & `chck-0.0.9/chck/path.py`

 * *Files identical despite different names*

### Comparing `chck-0.0.8/chck/trch.py` & `chck-0.0.9/chck/trch.py`

 * *Files identical despite different names*

### Comparing `chck-0.0.8/chck.egg-info/PKG-INFO` & `chck-0.0.9/chck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chck
-Version: 0.0.8
+Version: 0.0.9
 Summary: chck
 Home-page: https://github.com/dsm-72/chck
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: chck is question bool type guard typeguard check chck
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chck-0.0.8/settings.ini` & `chck-0.0.9/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = chck
 lib_name = chck
-version = 0.0.8
+version = 0.0.9
 min_python = 3.11
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = chck
 nbs_path = nbs
 recursive = True
```

### Comparing `chck-0.0.8/setup.py` & `chck-0.0.9/setup.py`

 * *Files identical despite different names*

