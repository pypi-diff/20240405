# Comparing `tmp/astr-0.0.8.tar.gz` & `tmp/astr-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astr-0.0.8.tar", last modified: Fri Apr  5 14:27:22 2024, max compression
+gzip compressed data, was "astr-0.0.9.tar", last modified: Fri Apr  5 14:30:47 2024, max compression
```

## Comparing `astr-0.0.8.tar` & `astr-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-05 14:27:22.176098 astr-0.0.8/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2024-01-13 21:01:11.000000 astr-0.0.8/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2024-01-13 21:01:11.000000 astr-0.0.8/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     2352 2024-04-05 14:27:22.175939 astr-0.0.8/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     1635 2024-01-13 21:09:28.000000 astr-0.0.8/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-05 14:27:22.174494 astr-0.0.8/astr/
--rw-r--r--   0 solst      (501) staff       (20)      322 2024-04-05 14:27:18.000000 astr-0.0.8/astr/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)     5994 2024-04-05 14:27:18.000000 astr-0.0.8/astr/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)      421 2024-04-05 14:27:18.000000 astr-0.0.8/astr/_tmp.py
--rw-r--r--   0 solst      (501) staff       (20)    27981 2024-04-05 14:27:18.000000 astr-0.0.8/astr/core.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-05 14:27:22.175566 astr-0.0.8/astr.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     2352 2024-04-05 14:27:22.000000 astr-0.0.8/astr.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      307 2024-04-05 14:27:22.000000 astr-0.0.8/astr.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-05 14:27:22.000000 astr-0.0.8/astr.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-05 14:27:22.000000 astr-0.0.8/astr.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-02-26 19:39:48.000000 astr-0.0.8/astr.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)        7 2024-04-05 14:27:22.000000 astr-0.0.8/astr.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-05 14:27:22.000000 astr-0.0.8/astr.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      878 2024-04-05 14:16:25.000000 astr-0.0.8/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-05 14:27:22.176143 astr-0.0.8/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2580 2024-01-13 21:01:11.000000 astr-0.0.8/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-05 14:30:47.345416 astr-0.0.9/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2024-01-13 21:01:11.000000 astr-0.0.9/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2024-01-13 21:01:11.000000 astr-0.0.9/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     2352 2024-04-05 14:30:47.345272 astr-0.0.9/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1635 2024-01-13 21:09:28.000000 astr-0.0.9/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-05 14:30:47.344139 astr-0.0.9/astr/
+-rw-r--r--   0 solst      (501) staff       (20)      322 2024-04-05 14:30:45.000000 astr-0.0.9/astr/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)     5994 2024-04-05 14:30:45.000000 astr-0.0.9/astr/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)      421 2024-04-05 14:30:45.000000 astr-0.0.9/astr/_tmp.py
+-rw-r--r--   0 solst      (501) staff       (20)    27978 2024-04-05 14:30:45.000000 astr-0.0.9/astr/core.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-05 14:30:47.345107 astr-0.0.9/astr.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     2352 2024-04-05 14:30:47.000000 astr-0.0.9/astr.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      307 2024-04-05 14:30:47.000000 astr-0.0.9/astr.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-05 14:30:47.000000 astr-0.0.9/astr.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-05 14:30:47.000000 astr-0.0.9/astr.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-02-26 19:39:48.000000 astr-0.0.9/astr.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)        7 2024-04-05 14:30:47.000000 astr-0.0.9/astr.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-05 14:30:47.000000 astr-0.0.9/astr.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      878 2024-04-05 14:28:23.000000 astr-0.0.9/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-05 14:30:47.345453 astr-0.0.9/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2580 2024-01-13 21:01:11.000000 astr-0.0.9/setup.py
```

### Comparing `astr-0.0.8/LICENSE` & `astr-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `astr-0.0.8/PKG-INFO` & `astr-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astr
-Version: 0.0.8
+Version: 0.0.9
 Summary: astr (attribute string) for defined getter / setter methods
 Home-page: https://github.com/dsm-72/astr
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: attr str attribute string astr attrstr python alias type astr typ get set instance ins insattr getter setter
 Classifier: Development Status :: 4 - Beta
```

### Comparing `astr-0.0.8/README.md` & `astr-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `astr-0.0.8/astr/_modidx.py` & `astr-0.0.9/astr/_modidx.py`

 * *Files identical despite different names*

### Comparing `astr-0.0.8/astr/core.py` & `astr-0.0.9/astr/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -494,15 +494,15 @@
         return decorator
     
     @wraps(insattr)
     def get(cls, item: object) -> Union[Any, bool, object]:
         '''Get the attribute specified by the this class from the object.'''
         if DOT in cls.attr: return cls.dot(item)
         kwds = {**cls.getvars()}
-        kwds.setdefault(RET_OPTION, ReturnOption.default)
+        kwds.setdefault(RET_OPTION, ReturnOption.self)
         return insattr(item, **cls.getvars())
     
     @wraps(insattr)
     def has(cls, item: object) -> TypeGuard[bool]:
         '''Returns whether the object has the attribute specified by the this class.'''
         if DOT in cls.attr: return cls.dot(item, ret_option = ReturnOption.has)
         kwds = {**cls.getvars(), **dict(ret_option = ReturnOption.has)}
```

### Comparing `astr-0.0.8/astr.egg-info/PKG-INFO` & `astr-0.0.9/astr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astr
-Version: 0.0.8
+Version: 0.0.9
 Summary: astr (attribute string) for defined getter / setter methods
 Home-page: https://github.com/dsm-72/astr
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: attr str attribute string astr attrstr python alias type astr typ get set instance ins insattr getter setter
 Classifier: Development Status :: 4 - Beta
```

### Comparing `astr-0.0.8/settings.ini` & `astr-0.0.9/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = astr
 lib_name = astr
-version = 0.0.8
+version = 0.0.9
 min_python = 3.11
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = astr
 nbs_path = nbs
 recursive = True
```

### Comparing `astr-0.0.8/setup.py` & `astr-0.0.9/setup.py`

 * *Files identical despite different names*

