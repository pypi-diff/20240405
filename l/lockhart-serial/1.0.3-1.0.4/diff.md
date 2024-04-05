# Comparing `tmp/lockhart_serial-1.0.3.tar.gz` & `tmp/lockhart-serial-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lockhart_serial-1.0.3.tar", last modified: Fri Apr  5 02:10:13 2024, max compression
+gzip compressed data, was "lockhart-serial-1.0.4.tar", last modified: Fri Apr  5 02:28:29 2024, max compression
```

## Comparing `lockhart_serial-1.0.3.tar` & `lockhart-serial-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:10:13.154410 lockhart_serial-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-05 02:10:08.000000 lockhart_serial-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-05 02:10:13.154410 lockhart_serial-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:10:08.000000 lockhart_serial-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:10:13.154410 lockhart_serial-1.0.3/lockhart-serial/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:10:08.000000 lockhart_serial-1.0.3/lockhart-serial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-05 02:10:08.000000 lockhart_serial-1.0.3/lockhart-serial/lockhart_serial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:10:13.154410 lockhart_serial-1.0.3/lockhart_serial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-05 02:10:13.000000 lockhart_serial-1.0.3/lockhart_serial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-05 02:10:13.000000 lockhart_serial-1.0.3/lockhart_serial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:10:13.000000 lockhart_serial-1.0.3/lockhart_serial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 02:10:13.000000 lockhart_serial-1.0.3/lockhart_serial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 02:10:13.000000 lockhart_serial-1.0.3/lockhart_serial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-05 02:10:08.000000 lockhart_serial-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 02:10:13.154410 lockhart_serial-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:28:29.161287 lockhart-serial-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-05 02:28:19.000000 lockhart-serial-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-05 02:28:29.161287 lockhart-serial-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:28:19.000000 lockhart-serial-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:28:29.157287 lockhart-serial-1.0.4/lockhart-serial/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:28:19.000000 lockhart-serial-1.0.4/lockhart-serial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-05 02:28:19.000000 lockhart-serial-1.0.4/lockhart-serial/lockhart_serial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:28:29.161287 lockhart-serial-1.0.4/lockhart_serial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-05 02:28:29.000000 lockhart-serial-1.0.4/lockhart_serial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-05 02:28:29.000000 lockhart-serial-1.0.4/lockhart_serial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:28:29.000000 lockhart-serial-1.0.4/lockhart_serial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 02:28:29.000000 lockhart-serial-1.0.4/lockhart_serial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 02:28:29.000000 lockhart-serial-1.0.4/lockhart_serial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-05 02:28:19.000000 lockhart-serial-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 02:28:29.161287 lockhart-serial-1.0.4/setup.cfg
```

### Comparing `lockhart_serial-1.0.3/LICENSE` & `lockhart-serial-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lockhart_serial-1.0.3/PKG-INFO` & `lockhart-serial-1.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lockhart_serial
-Version: 1.0.3
+Name: lockhart-serial
+Version: 1.0.4
 Summary: Serial communication for Lockhart devices
 Author-email: NinjaBunny <xxninjabunnyxx@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lockhart_serial-1.0.3/lockhart-serial/lockhart_serial.py` & `lockhart-serial-1.0.4/lockhart-serial/lockhart_serial.py`

 * *Files identical despite different names*

### Comparing `lockhart_serial-1.0.3/lockhart_serial.egg-info/PKG-INFO` & `lockhart-serial-1.0.4/lockhart_serial.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lockhart_serial
-Version: 1.0.3
+Name: lockhart-serial
+Version: 1.0.4
 Summary: Serial communication for Lockhart devices
 Author-email: NinjaBunny <xxninjabunnyxx@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lockhart_serial-1.0.3/pyproject.toml` & `lockhart-serial-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
-name = "lockhart_serial"
-version = "1.0.3"
+name = "lockhart-serial"
+version = "1.0.4"
 authors = [
   { name="NinjaBunny", email="xxninjabunnyxx@gmail.com" },
 ]
 description = "Serial communication for Lockhart devices"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

