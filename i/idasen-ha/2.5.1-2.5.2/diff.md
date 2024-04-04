# Comparing `tmp/idasen-ha-2.5.1.tar.gz` & `tmp/idasen-ha-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idasen-ha-2.5.1.tar", last modified: Mon Feb 26 01:09:39 2024, max compression
+gzip compressed data, was "idasen-ha-2.5.2.tar", last modified: Thu Apr  4 23:26:20 2024, max compression
```

## Comparing `idasen-ha-2.5.1.tar` & `idasen-ha-2.5.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 01:09:39.527990 idasen-ha-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-26 01:09:28.000000 idasen-ha-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-26 01:09:28.000000 idasen-ha-2.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-02-26 01:09:39.527990 idasen-ha-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-26 01:09:28.000000 idasen-ha-2.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 01:09:39.527990 idasen-ha-2.5.1/idasen_ha/
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-02-26 01:09:28.000000 idasen-ha-2.5.1/idasen_ha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-02-26 01:09:28.000000 idasen-ha-2.5.1/idasen_ha/connection_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-26 01:09:28.000000 idasen-ha-2.5.1/idasen_ha/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 01:09:39.527990 idasen-ha-2.5.1/idasen_ha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-02-26 01:09:39.000000 idasen-ha-2.5.1/idasen_ha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-02-26 01:09:39.000000 idasen-ha-2.5.1/idasen_ha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 01:09:39.000000 idasen-ha-2.5.1/idasen_ha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-26 01:09:39.000000 idasen-ha-2.5.1/idasen_ha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-26 01:09:39.000000 idasen-ha-2.5.1/idasen_ha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-02-26 01:09:28.000000 idasen-ha-2.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-26 01:09:28.000000 idasen-ha-2.5.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-26 01:09:28.000000 idasen-ha-2.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 01:09:39.527990 idasen-ha-2.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 01:09:39.527990 idasen-ha-2.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-02-26 01:09:28.000000 idasen-ha-2.5.1/tests/test_connection_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-02-26 01:09:28.000000 idasen-ha-2.5.1/tests/test_desk_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:26:20.091425 idasen-ha-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-04 23:26:11.000000 idasen-ha-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-04 23:26:11.000000 idasen-ha-2.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-04 23:26:20.091425 idasen-ha-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-04 23:26:11.000000 idasen-ha-2.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:26:20.087425 idasen-ha-2.5.2/idasen_ha/
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-04 23:26:11.000000 idasen-ha-2.5.2/idasen_ha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-04 23:26:11.000000 idasen-ha-2.5.2/idasen_ha/connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-04 23:26:11.000000 idasen-ha-2.5.2/idasen_ha/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:26:20.091425 idasen-ha-2.5.2/idasen_ha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-04 23:26:20.000000 idasen-ha-2.5.2/idasen_ha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-04 23:26:20.000000 idasen-ha-2.5.2/idasen_ha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 23:26:20.000000 idasen-ha-2.5.2/idasen_ha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 23:26:20.000000 idasen-ha-2.5.2/idasen_ha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 23:26:20.000000 idasen-ha-2.5.2/idasen_ha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-04-04 23:26:11.000000 idasen-ha-2.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-04 23:26:11.000000 idasen-ha-2.5.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 23:26:11.000000 idasen-ha-2.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 23:26:20.091425 idasen-ha-2.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:26:20.091425 idasen-ha-2.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-04-04 23:26:11.000000 idasen-ha-2.5.2/tests/test_connection_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-04 23:26:11.000000 idasen-ha-2.5.2/tests/test_desk_functions.py
```

### Comparing `idasen-ha-2.5.1/LICENSE` & `idasen-ha-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `idasen-ha-2.5.1/PKG-INFO` & `idasen-ha-2.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: idasen-ha
-Version: 2.5.1
+Version: 2.5.2
 Summary: Home Assistant helper lib for the IKEA Idasen Desk integration
 Author-email: Abílio Costa <amfcalt@gmail.com>
 Project-URL: Homepage, https://github.com/abmantis/idasen-ha/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: idasen<=0.11.0,>=0.10
+Requires-Dist: idasen<=0.12.0,>=0.10
 
 # Idasen HA
 
 Home Assistant helper lib for the IKEA Idasen Desk integration.
```

### Comparing `idasen-ha-2.5.1/idasen_ha/__init__.py` & `idasen-ha-2.5.2/idasen_ha/__init__.py`

 * *Files identical despite different names*

### Comparing `idasen-ha-2.5.1/idasen_ha/connection_manager.py` & `idasen-ha-2.5.2/idasen_ha/connection_manager.py`

 * *Files identical despite different names*

### Comparing `idasen-ha-2.5.1/idasen_ha.egg-info/PKG-INFO` & `idasen-ha-2.5.2/idasen_ha.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: idasen-ha
-Version: 2.5.1
+Version: 2.5.2
 Summary: Home Assistant helper lib for the IKEA Idasen Desk integration
 Author-email: Abílio Costa <amfcalt@gmail.com>
 Project-URL: Homepage, https://github.com/abmantis/idasen-ha/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: idasen<=0.11.0,>=0.10
+Requires-Dist: idasen<=0.12.0,>=0.10
 
 # Idasen HA
 
 Home Assistant helper lib for the IKEA Idasen Desk integration.
```

### Comparing `idasen-ha-2.5.1/pyproject.toml` & `idasen-ha-2.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "idasen-ha"
-version = "2.5.1"
+version = "2.5.2"
 authors = [{name = "Abílio Costa", email = "amfcalt@gmail.com"}]
 description = "Home Assistant helper lib for the IKEA Idasen Desk integration"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.9"
 dependencies = [
-    "idasen>=0.10,<=0.11.0"
+    "idasen>=0.10,<=0.12.0"
 ]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.urls]
```

### Comparing `idasen-ha-2.5.1/tests/test_connection_management.py` & `idasen-ha-2.5.2/tests/test_connection_management.py`

 * *Files identical despite different names*

### Comparing `idasen-ha-2.5.1/tests/test_desk_functions.py` & `idasen-ha-2.5.2/tests/test_desk_functions.py`

 * *Files identical despite different names*

