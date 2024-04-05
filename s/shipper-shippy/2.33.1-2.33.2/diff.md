# Comparing `tmp/shipper-shippy-2.33.1.tar.gz` & `tmp/shipper-shippy-2.33.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipper-shippy-2.33.1.tar", last modified: Tue Apr  2 23:45:29 2024, max compression
+gzip compressed data, was "shipper-shippy-2.33.2.tar", last modified: Fri Apr  5 20:29:57 2024, max compression
```

## Comparing `shipper-shippy-2.33.1.tar` & `shipper-shippy-2.33.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:45:29.426113 shipper-shippy-2.33.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-02 23:45:29.426113 shipper-shippy-2.33.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-02 23:45:21.000000 shipper-shippy-2.33.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-02 23:45:21.000000 shipper-shippy-2.33.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 23:45:29.426113 shipper-shippy-2.33.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-02 23:45:21.000000 shipper-shippy-2.33.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:45:29.426113 shipper-shippy-2.33.1/shipper_shippy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-02 23:45:29.000000 shipper-shippy-2.33.1/shipper_shippy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-02 23:45:29.000000 shipper-shippy-2.33.1/shipper_shippy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 23:45:29.000000 shipper-shippy-2.33.1/shipper_shippy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-02 23:45:29.000000 shipper-shippy-2.33.1/shipper_shippy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 23:45:29.000000 shipper-shippy-2.33.1/shipper_shippy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 23:45:29.000000 shipper-shippy-2.33.1/shipper_shippy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:45:29.426113 shipper-shippy-2.33.1/shippy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 23:45:21.000000 shipper-shippy-2.33.1/shippy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12218 2024-04-02 23:45:21.000000 shipper-shippy-2.33.1/shippy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13708 2024-04-02 23:45:21.000000 shipper-shippy-2.33.1/shippy/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-02 23:45:21.000000 shipper-shippy-2.33.1/shippy/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-02 23:45:21.000000 shipper-shippy-2.33.1/shippy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-02 23:45:21.000000 shipper-shippy-2.33.1/shippy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-02 23:45:21.000000 shipper-shippy-2.33.1/shippy/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 23:45:21.000000 shipper-shippy-2.33.1/shippy/server_compat_version.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 23:45:21.000000 shipper-shippy-2.33.1/shippy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:29:57.926961 shipper-shippy-2.33.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-05 20:29:57.926961 shipper-shippy-2.33.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-05 20:29:43.000000 shipper-shippy-2.33.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-05 20:29:43.000000 shipper-shippy-2.33.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 20:29:57.926961 shipper-shippy-2.33.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-05 20:29:43.000000 shipper-shippy-2.33.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:29:57.926961 shipper-shippy-2.33.2/shipper_shippy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-05 20:29:57.000000 shipper-shippy-2.33.2/shipper_shippy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-05 20:29:57.000000 shipper-shippy-2.33.2/shipper_shippy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 20:29:57.000000 shipper-shippy-2.33.2/shipper_shippy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-05 20:29:57.000000 shipper-shippy-2.33.2/shipper_shippy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-05 20:29:57.000000 shipper-shippy-2.33.2/shipper_shippy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 20:29:57.000000 shipper-shippy-2.33.2/shipper_shippy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:29:57.926961 shipper-shippy-2.33.2/shippy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:29:43.000000 shipper-shippy-2.33.2/shippy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12218 2024-04-05 20:29:43.000000 shipper-shippy-2.33.2/shippy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13708 2024-04-05 20:29:43.000000 shipper-shippy-2.33.2/shippy/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-05 20:29:43.000000 shipper-shippy-2.33.2/shippy/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-05 20:29:43.000000 shipper-shippy-2.33.2/shippy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-05 20:29:43.000000 shipper-shippy-2.33.2/shippy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-05 20:29:43.000000 shipper-shippy-2.33.2/shippy/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 20:29:43.000000 shipper-shippy-2.33.2/shippy/server_compat_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-05 20:29:43.000000 shipper-shippy-2.33.2/shippy/version.py
```

### Comparing `shipper-shippy-2.33.1/PKG-INFO` & `shipper-shippy-2.33.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipper-shippy
-Version: 2.33.1
+Version: 2.33.2
 Summary: Client-side tool to interface with shipper
 Home-page: https://github.com/ericswpark/shippy
 Author: Eric Park
 Author-email: me@ericswpark.com
 Project-URL: Bug Tracker, https://github.com/ericswpark/shippy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shipper-shippy-2.33.1/README.md` & `shipper-shippy-2.33.2/README.md`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.33.1/setup.py` & `shipper-shippy-2.33.2/setup.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.33.1/shipper_shippy.egg-info/PKG-INFO` & `shipper-shippy-2.33.2/shipper_shippy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipper-shippy
-Version: 2.33.1
+Version: 2.33.2
 Summary: Client-side tool to interface with shipper
 Home-page: https://github.com/ericswpark/shippy
 Author: Eric Park
 Author-email: me@ericswpark.com
 Project-URL: Bug Tracker, https://github.com/ericswpark/shippy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shipper-shippy-2.33.1/shippy/__main__.py` & `shipper-shippy-2.33.2/shippy/__main__.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.33.1/shippy/client.py` & `shipper-shippy-2.33.2/shippy/client.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.33.1/shippy/config.py` & `shipper-shippy-2.33.2/shippy/config.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.33.1/shippy/constants.py` & `shipper-shippy-2.33.2/shippy/constants.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.33.1/shippy/helper.py` & `shipper-shippy-2.33.2/shippy/helper.py`

 * *Files identical despite different names*

