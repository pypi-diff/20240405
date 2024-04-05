# Comparing `tmp/pyaffalddk-2.0.20.tar.gz` & `tmp/pyaffalddk-2.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaffalddk-2.0.20.tar", last modified: Tue Apr  2 13:53:34 2024, max compression
+gzip compressed data, was "pyaffalddk-2.0.21.tar", last modified: Fri Apr  5 04:02:57 2024, max compression
```

## Comparing `pyaffalddk-2.0.20.tar` & `pyaffalddk-2.0.21.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:53:34.019479 pyaffalddk-2.0.20/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-02 13:53:29.000000 pyaffalddk-2.0.20/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-02 13:53:34.019479 pyaffalddk-2.0.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-02 13:53:29.000000 pyaffalddk-2.0.20/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:53:34.019479 pyaffalddk-2.0.20/pyaffalddk/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-02 13:53:29.000000 pyaffalddk-2.0.20/pyaffalddk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-04-02 13:53:29.000000 pyaffalddk-2.0.20/pyaffalddk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10756 2024-04-02 13:53:29.000000 pyaffalddk-2.0.20/pyaffalddk/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-02 13:53:29.000000 pyaffalddk-2.0.20/pyaffalddk/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-02 13:53:29.000000 pyaffalddk-2.0.20/pyaffalddk/images.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:53:34.019479 pyaffalddk-2.0.20/pyaffalddk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-02 13:53:34.000000 pyaffalddk-2.0.20/pyaffalddk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-02 13:53:34.000000 pyaffalddk-2.0.20/pyaffalddk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:53:34.000000 pyaffalddk-2.0.20/pyaffalddk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 13:53:34.000000 pyaffalddk-2.0.20/pyaffalddk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 13:53:34.019479 pyaffalddk-2.0.20/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-02 13:53:29.000000 pyaffalddk-2.0.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:02:57.319516 pyaffalddk-2.0.21/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-05 04:02:53.000000 pyaffalddk-2.0.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-05 04:02:57.319516 pyaffalddk-2.0.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-05 04:02:53.000000 pyaffalddk-2.0.21/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:02:57.319516 pyaffalddk-2.0.21/pyaffalddk/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-05 04:02:53.000000 pyaffalddk-2.0.21/pyaffalddk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-04-05 04:02:53.000000 pyaffalddk-2.0.21/pyaffalddk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-04-05 04:02:53.000000 pyaffalddk-2.0.21/pyaffalddk/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-05 04:02:53.000000 pyaffalddk-2.0.21/pyaffalddk/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-05 04:02:53.000000 pyaffalddk-2.0.21/pyaffalddk/images.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:02:57.319516 pyaffalddk-2.0.21/pyaffalddk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-05 04:02:57.000000 pyaffalddk-2.0.21/pyaffalddk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-05 04:02:57.000000 pyaffalddk-2.0.21/pyaffalddk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 04:02:57.000000 pyaffalddk-2.0.21/pyaffalddk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 04:02:57.000000 pyaffalddk-2.0.21/pyaffalddk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 04:02:57.319516 pyaffalddk-2.0.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-05 04:02:53.000000 pyaffalddk-2.0.21/setup.py
```

### Comparing `pyaffalddk-2.0.20/LICENSE` & `pyaffalddk-2.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaffalddk-2.0.20/PKG-INFO` & `pyaffalddk-2.0.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaffalddk
-Version: 2.0.20
+Version: 2.0.21
 Summary: Gets garbage collection data from danish Municipalities
 Home-page: https://github.com/briis/pyaffalddk
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyaffalddk-2.0.20/pyaffalddk/__init__.py` & `pyaffalddk-2.0.21/pyaffalddk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,10 +11,10 @@
     AffaldDKNoConnection,
 )
 from pyaffalddk.data import PickupEvents, PickupType, AffaldDKAddressInfo
 
 from pyaffalddk.const import ICON_LIST, MUNICIPALITIES_ARRAY, NAME_ARRAY, NAME_LIST
 
 __title__ = "pyaffalddk"
-__version__ = "2.0.20"
+__version__ = "2.0.21"
 __author__ = "briis"
 __license__ = "MIT"
```

### Comparing `pyaffalddk-2.0.20/pyaffalddk/api.py` & `pyaffalddk-2.0.21/pyaffalddk/api.py`

 * *Files identical despite different names*

### Comparing `pyaffalddk-2.0.20/pyaffalddk/const.py` & `pyaffalddk-2.0.21/pyaffalddk/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         "Miljøkasser",
         "Farligt Affald, Rød boks",
         "Genbrugsbilen",
     ],
     "farligtaffaldmiljoboks": [
         "Farligt affald/Miljøboks",
         "Papir og glas/dåser",
+        "Miljøboks",
     ],
     "flis": [
         "Flis",
         "Flishugning",
     ],
     "genbrug": [
         "Genbrug",
```

### Comparing `pyaffalddk-2.0.20/pyaffalddk/data.py` & `pyaffalddk-2.0.21/pyaffalddk/data.py`

 * *Files identical despite different names*

### Comparing `pyaffalddk-2.0.20/pyaffalddk/images.py` & `pyaffalddk-2.0.21/pyaffalddk/images.py`

 * *Files identical despite different names*

### Comparing `pyaffalddk-2.0.20/pyaffalddk.egg-info/PKG-INFO` & `pyaffalddk-2.0.21/pyaffalddk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaffalddk
-Version: 2.0.20
+Version: 2.0.21
 Summary: Gets garbage collection data from danish Municipalities
 Home-page: https://github.com/briis/pyaffalddk
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyaffalddk-2.0.20/setup.py` & `pyaffalddk-2.0.21/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyaffalddk",
-    version="2.0.20",
+    version="2.0.21",
     author="briis",
     author_email="bjarne@briis.com",
     description="Gets garbage collection data from danish Municipalities",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/briis/pyaffalddk",
```

