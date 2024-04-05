# Comparing `tmp/neon-phal-plugin-device-updater-0.1.1a1.tar.gz` & `tmp/neon-phal-plugin-device-updater-0.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-phal-plugin-device-updater-0.1.1a1.tar", last modified: Tue Mar 12 00:33:44 2024, max compression
+gzip compressed data, was "neon-phal-plugin-device-updater-0.1.1a2.tar", last modified: Fri Apr  5 17:36:45 2024, max compression
```

## Comparing `neon-phal-plugin-device-updater-0.1.1a1.tar` & `neon-phal-plugin-device-updater-0.1.1a2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:33:44.381948 neon-phal-plugin-device-updater-0.1.1a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-12 00:33:38.000000 neon-phal-plugin-device-updater-0.1.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-03-12 00:33:44.381948 neon-phal-plugin-device-updater-0.1.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-03-12 00:33:38.000000 neon-phal-plugin-device-updater-0.1.1a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:33:44.381948 neon-phal-plugin-device-updater-0.1.1a1/neon_phal_plugin_device_updater/
--rw-r--r--   0 runner    (1001) docker     (127)    23786 2024-03-12 00:33:38.000000 neon-phal-plugin-device-updater-0.1.1a1/neon_phal_plugin_device_updater/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 00:33:44.381948 neon-phal-plugin-device-updater-0.1.1a1/neon_phal_plugin_device_updater.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-03-12 00:33:44.000000 neon-phal-plugin-device-updater-0.1.1a1/neon_phal_plugin_device_updater.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-12 00:33:44.000000 neon-phal-plugin-device-updater-0.1.1a1/neon_phal_plugin_device_updater.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 00:33:44.000000 neon-phal-plugin-device-updater-0.1.1a1/neon_phal_plugin_device_updater.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-12 00:33:44.000000 neon-phal-plugin-device-updater-0.1.1a1/neon_phal_plugin_device_updater.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-12 00:33:44.000000 neon-phal-plugin-device-updater-0.1.1a1/neon_phal_plugin_device_updater.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-12 00:33:44.000000 neon-phal-plugin-device-updater-0.1.1a1/neon_phal_plugin_device_updater.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 00:33:44.381948 neon-phal-plugin-device-updater-0.1.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-03-12 00:33:38.000000 neon-phal-plugin-device-updater-0.1.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:36:45.832819 neon-phal-plugin-device-updater-0.1.1a2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-05 17:36:42.000000 neon-phal-plugin-device-updater-0.1.1a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-05 17:36:45.832819 neon-phal-plugin-device-updater-0.1.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-05 17:36:42.000000 neon-phal-plugin-device-updater-0.1.1a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:36:45.832819 neon-phal-plugin-device-updater-0.1.1a2/neon_phal_plugin_device_updater/
+-rw-r--r--   0 runner    (1001) docker     (127)    23786 2024-04-05 17:36:42.000000 neon-phal-plugin-device-updater-0.1.1a2/neon_phal_plugin_device_updater/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:36:45.832819 neon-phal-plugin-device-updater-0.1.1a2/neon_phal_plugin_device_updater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-05 17:36:45.000000 neon-phal-plugin-device-updater-0.1.1a2/neon_phal_plugin_device_updater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-05 17:36:45.000000 neon-phal-plugin-device-updater-0.1.1a2/neon_phal_plugin_device_updater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:36:45.000000 neon-phal-plugin-device-updater-0.1.1a2/neon_phal_plugin_device_updater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-05 17:36:45.000000 neon-phal-plugin-device-updater-0.1.1a2/neon_phal_plugin_device_updater.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-05 17:36:45.000000 neon-phal-plugin-device-updater-0.1.1a2/neon_phal_plugin_device_updater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 17:36:45.000000 neon-phal-plugin-device-updater-0.1.1a2/neon_phal_plugin_device_updater.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 17:36:45.832819 neon-phal-plugin-device-updater-0.1.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-05 17:36:42.000000 neon-phal-plugin-device-updater-0.1.1a2/setup.py
```

### Comparing `neon-phal-plugin-device-updater-0.1.1a1/LICENSE.md` & `neon-phal-plugin-device-updater-0.1.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-device-updater-0.1.1a1/PKG-INFO` & `neon-phal-plugin-device-updater-0.1.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-device-updater
-Version: 0.1.1a1
+Version: 0.1.1a2
 Summary: Core Module Update Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-device-updater
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-device-updater-0.1.1a1/README.md` & `neon-phal-plugin-device-updater-0.1.1a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-device-updater-0.1.1a1/neon_phal_plugin_device_updater/__init__.py` & `neon-phal-plugin-device-updater-0.1.1a2/neon_phal_plugin_device_updater/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-device-updater-0.1.1a1/neon_phal_plugin_device_updater.egg-info/PKG-INFO` & `neon-phal-plugin-device-updater-0.1.1a2/neon_phal_plugin_device_updater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-device-updater
-Version: 0.1.1a1
+Version: 0.1.1a2
 Summary: Core Module Update Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-device-updater
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-device-updater-0.1.1a1/setup.py` & `neon-phal-plugin-device-updater-0.1.1a2/setup.py`

 * *Files identical despite different names*

