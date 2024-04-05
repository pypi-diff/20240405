# Comparing `tmp/lockhart-serial-1.0.0.tar.gz` & `tmp/lockhart-serial-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lockhart-serial-1.0.0.tar", last modified: Wed Apr  3 23:19:50 2024, max compression
+gzip compressed data, was "lockhart-serial-1.0.1.tar", last modified: Fri Apr  5 01:20:59 2024, max compression
```

## Comparing `lockhart-serial-1.0.0.tar` & `lockhart-serial-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:19:50.586606 lockhart-serial-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-03 23:19:46.000000 lockhart-serial-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-03 23:19:50.586606 lockhart-serial-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 23:19:46.000000 lockhart-serial-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:19:50.582606 lockhart-serial-1.0.0/lockhart_serial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-03 23:19:50.000000 lockhart-serial-1.0.0/lockhart_serial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-03 23:19:50.000000 lockhart-serial-1.0.0/lockhart_serial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 23:19:50.000000 lockhart-serial-1.0.0/lockhart_serial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 23:19:50.000000 lockhart-serial-1.0.0/lockhart_serial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 23:19:50.000000 lockhart-serial-1.0.0/lockhart_serial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-03 23:19:46.000000 lockhart-serial-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 23:19:50.586606 lockhart-serial-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:20:59.423092 lockhart-serial-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-05 01:20:52.000000 lockhart-serial-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-05 01:20:59.423092 lockhart-serial-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 01:20:52.000000 lockhart-serial-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:20:59.423092 lockhart-serial-1.0.1/lockhart_serial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-05 01:20:59.000000 lockhart-serial-1.0.1/lockhart_serial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-05 01:20:59.000000 lockhart-serial-1.0.1/lockhart_serial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 01:20:59.000000 lockhart-serial-1.0.1/lockhart_serial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 01:20:59.000000 lockhart-serial-1.0.1/lockhart_serial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 01:20:59.000000 lockhart-serial-1.0.1/lockhart_serial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-05 01:20:52.000000 lockhart-serial-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 01:20:59.423092 lockhart-serial-1.0.1/setup.cfg
```

### Comparing `lockhart-serial-1.0.0/LICENSE` & `lockhart-serial-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lockhart-serial-1.0.0/PKG-INFO` & `lockhart-serial-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lockhart-serial
-Version: 1.0.0
+Version: 1.0.1
 Summary: Serial communication for Lockhart devices
 Author-email: NinjaBunny <xxninjabunnyxx@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lockhart-serial-1.0.0/lockhart_serial.egg-info/PKG-INFO` & `lockhart-serial-1.0.1/lockhart_serial.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lockhart-serial
-Version: 1.0.0
+Version: 1.0.1
 Summary: Serial communication for Lockhart devices
 Author-email: NinjaBunny <xxninjabunnyxx@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lockhart-serial-1.0.0/pyproject.toml` & `lockhart-serial-1.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lockhart-serial"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="NinjaBunny", email="xxninjabunnyxx@gmail.com" },
 ]
 description = "Serial communication for Lockhart devices"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -13,14 +13,17 @@
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
   "pyserial"
 ]
 
+[options.packages.find]
+where = "lockhart-serial"
+
 [project.urls]
 Homepage = "https://github.com/pypa/sampleproject"
 Issues = "https://github.com/pypa/sampleproject/issues"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
```

