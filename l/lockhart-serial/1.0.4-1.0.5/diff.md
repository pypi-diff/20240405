# Comparing `tmp/lockhart-serial-1.0.4.tar.gz` & `tmp/lockhart-serial-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lockhart-serial-1.0.4.tar", last modified: Fri Apr  5 02:28:29 2024, max compression
+gzip compressed data, was "lockhart-serial-1.0.5.tar", last modified: Fri Apr  5 02:55:40 2024, max compression
```

## Comparing `lockhart-serial-1.0.4.tar` & `lockhart-serial-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:28:29.161287 lockhart-serial-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-05 02:28:19.000000 lockhart-serial-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-05 02:28:29.161287 lockhart-serial-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:28:19.000000 lockhart-serial-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:28:29.157287 lockhart-serial-1.0.4/lockhart-serial/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:28:19.000000 lockhart-serial-1.0.4/lockhart-serial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-05 02:28:19.000000 lockhart-serial-1.0.4/lockhart-serial/lockhart_serial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:28:29.161287 lockhart-serial-1.0.4/lockhart_serial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-05 02:28:29.000000 lockhart-serial-1.0.4/lockhart_serial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-05 02:28:29.000000 lockhart-serial-1.0.4/lockhart_serial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:28:29.000000 lockhart-serial-1.0.4/lockhart_serial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 02:28:29.000000 lockhart-serial-1.0.4/lockhart_serial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 02:28:29.000000 lockhart-serial-1.0.4/lockhart_serial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-05 02:28:19.000000 lockhart-serial-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 02:28:29.161287 lockhart-serial-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:55:40.610452 lockhart-serial-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-05 02:55:35.000000 lockhart-serial-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-05 02:55:40.610452 lockhart-serial-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:55:35.000000 lockhart-serial-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:55:40.610452 lockhart-serial-1.0.5/lockhart-serial/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 02:55:35.000000 lockhart-serial-1.0.5/lockhart-serial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-05 02:55:35.000000 lockhart-serial-1.0.5/lockhart-serial/lockhart_serial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:55:40.610452 lockhart-serial-1.0.5/lockhart_serial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-05 02:55:40.000000 lockhart-serial-1.0.5/lockhart_serial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-05 02:55:40.000000 lockhart-serial-1.0.5/lockhart_serial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:55:40.000000 lockhart-serial-1.0.5/lockhart_serial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 02:55:40.000000 lockhart-serial-1.0.5/lockhart_serial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 02:55:40.000000 lockhart-serial-1.0.5/lockhart_serial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-05 02:55:35.000000 lockhart-serial-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 02:55:40.610452 lockhart-serial-1.0.5/setup.cfg
```

### Comparing `lockhart-serial-1.0.4/LICENSE` & `lockhart-serial-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lockhart-serial-1.0.4/PKG-INFO` & `lockhart-serial-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lockhart-serial
-Version: 1.0.4
+Version: 1.0.5
 Summary: Serial communication for Lockhart devices
 Author-email: NinjaBunny <xxninjabunnyxx@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lockhart-serial-1.0.4/lockhart-serial/lockhart_serial.py` & `lockhart-serial-1.0.5/lockhart-serial/lockhart_serial.py`

 * *Files identical despite different names*

### Comparing `lockhart-serial-1.0.4/lockhart_serial.egg-info/PKG-INFO` & `lockhart-serial-1.0.5/lockhart_serial.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lockhart-serial
-Version: 1.0.4
+Version: 1.0.5
 Summary: Serial communication for Lockhart devices
 Author-email: NinjaBunny <xxninjabunnyxx@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lockhart-serial-1.0.4/pyproject.toml` & `lockhart-serial-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lockhart-serial"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="NinjaBunny", email="xxninjabunnyxx@gmail.com" },
 ]
 description = "Serial communication for Lockhart devices"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

