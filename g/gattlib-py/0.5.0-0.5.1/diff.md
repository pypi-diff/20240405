# Comparing `tmp/gattlib-py-0.5.0.tar.gz` & `tmp/gattlib-py-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gattlib-py-0.5.0.tar", last modified: Thu Apr  4 10:53:19 2024, max compression
+gzip compressed data, was "gattlib-py-0.5.1.tar", last modified: Thu Apr  4 20:12:55 2024, max compression
```

## Comparing `gattlib-py-0.5.0.tar` & `gattlib-py-0.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:53:19.333000 gattlib-py-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-04 10:53:19.333000 gattlib-py-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-04 10:35:39.000000 gattlib-py-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:53:19.333000 gattlib-py-0.5.0/gattlib/
--rw-r--r--   0 runner    (1001) docker     (127)    10838 2024-04-04 10:35:39.000000 gattlib-py-0.5.0/gattlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 10:53:19.000000 gattlib-py-0.5.0/gattlib/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-04-04 10:35:39.000000 gattlib-py-0.5.0/gattlib/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11167 2024-04-04 10:35:39.000000 gattlib-py-0.5.0/gattlib/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-04 10:35:39.000000 gattlib-py-0.5.0/gattlib/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-04 10:35:39.000000 gattlib-py-0.5.0/gattlib/gatt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-04 10:35:39.000000 gattlib-py-0.5.0/gattlib/mainloop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-04 10:35:39.000000 gattlib-py-0.5.0/gattlib/uuid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:53:19.333000 gattlib-py-0.5.0/gattlib_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-04 10:53:19.000000 gattlib-py-0.5.0/gattlib_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-04 10:53:19.000000 gattlib-py-0.5.0/gattlib_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 10:53:19.000000 gattlib-py-0.5.0/gattlib_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-04 10:53:19.000000 gattlib-py-0.5.0/gattlib_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 10:53:19.000000 gattlib-py-0.5.0/gattlib_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 10:53:19.333000 gattlib-py-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-04 10:35:39.000000 gattlib-py-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.267451 gattlib-py-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-04 20:12:55.263451 gattlib-py-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-04 19:55:03.000000 gattlib-py-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.263451 gattlib-py-0.5.1/gattlib/
+-rw-r--r--   0 runner    (1001) docker     (127)    10838 2024-04-04 19:55:03.000000 gattlib-py-0.5.1/gattlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 20:12:55.000000 gattlib-py-0.5.1/gattlib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-04-04 19:55:03.000000 gattlib-py-0.5.1/gattlib/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11167 2024-04-04 19:55:03.000000 gattlib-py-0.5.1/gattlib/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-04 19:55:03.000000 gattlib-py-0.5.1/gattlib/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-04 19:55:03.000000 gattlib-py-0.5.1/gattlib/gatt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-04 19:55:03.000000 gattlib-py-0.5.1/gattlib/mainloop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-04 19:55:03.000000 gattlib-py-0.5.1/gattlib/uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.263451 gattlib-py-0.5.1/gattlib_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-04 20:12:55.000000 gattlib-py-0.5.1/gattlib_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-04 20:12:55.000000 gattlib-py-0.5.1/gattlib_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 20:12:55.000000 gattlib-py-0.5.1/gattlib_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-04 20:12:55.000000 gattlib-py-0.5.1/gattlib_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 20:12:55.000000 gattlib-py-0.5.1/gattlib_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 20:12:55.267451 gattlib-py-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-04 19:55:03.000000 gattlib-py-0.5.1/setup.py
```

### Comparing `gattlib-py-0.5.0/PKG-INFO` & `gattlib-py-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gattlib-py
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python wrapper for gattlib library
 Home-page: https://github.com/labapart/gattlib/gattlib-py
 Author: Olivier Martin
 Author-email: olivier@labapart.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `gattlib-py-0.5.0/gattlib/__init__.py` & `gattlib-py-0.5.1/gattlib/__init__.py`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.5.0/gattlib/adapter.py` & `gattlib-py-0.5.1/gattlib/adapter.py`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.5.0/gattlib/device.py` & `gattlib-py-0.5.1/gattlib/device.py`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.5.0/gattlib/exception.py` & `gattlib-py-0.5.1/gattlib/exception.py`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.5.0/gattlib/gatt.py` & `gattlib-py-0.5.1/gattlib/gatt.py`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.5.0/gattlib/mainloop.py` & `gattlib-py-0.5.1/gattlib/mainloop.py`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.5.0/gattlib/uuid.py` & `gattlib-py-0.5.1/gattlib/uuid.py`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.5.0/gattlib_py.egg-info/PKG-INFO` & `gattlib-py-0.5.1/gattlib_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gattlib-py
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python wrapper for gattlib library
 Home-page: https://github.com/labapart/gattlib/gattlib-py
 Author: Olivier Martin
 Author-email: olivier@labapart.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `gattlib-py-0.5.0/setup.py` & `gattlib-py-0.5.1/setup.py`

 * *Files identical despite different names*

