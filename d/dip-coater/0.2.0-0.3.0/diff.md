# Comparing `tmp/dip-coater-0.2.0.tar.gz` & `tmp/dip-coater-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dip-coater-0.2.0.tar", last modified: Fri Apr  5 10:26:20 2024, max compression
+gzip compressed data, was "dip-coater-0.3.0.tar", last modified: Fri Apr  5 10:32:28 2024, max compression
```

## Comparing `dip-coater-0.2.0.tar` & `dip-coater-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 10:26:20.733638 dip-coater-0.2.0/
--rw-r--r--   0 rik      (459800007) staff       (20)       89 2024-04-05 09:39:07.000000 dip-coater-0.2.0/MANIFEST.in
--rw-r--r--   0 rik      (459800007) staff       (20)      269 2024-04-05 10:26:20.733451 dip-coater-0.2.0/PKG-INFO
--rw-r--r--   0 rik      (459800007) staff       (20)      531 2024-04-05 10:26:14.000000 dip-coater-0.2.0/pyproject.toml
--rw-r--r--   0 rik      (459800007) staff       (20)       38 2024-04-05 10:26:20.733693 dip-coater-0.2.0/setup.cfg
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 10:26:20.731168 dip-coater-0.2.0/src/
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 10:26:20.731934 dip-coater-0.2.0/src/dip_coater/
--rw-r--r--   0 rik      (459800007) staff       (20)        0 2024-04-05 10:07:42.000000 dip-coater-0.2.0/src/dip_coater/__init__.py
--rw-r--r--   0 rik      (459800007) staff       (20)     4293 2024-04-04 11:06:11.000000 dip-coater-0.2.0/src/dip_coater/motor.py
--rw-r--r--   0 rik      (459800007) staff       (20)     8631 2024-04-05 10:10:36.000000 dip-coater-0.2.0/src/dip_coater/tui.py
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 10:26:20.733169 dip-coater-0.2.0/src/dip_coater.egg-info/
--rw-r--r--   0 rik      (459800007) staff       (20)      269 2024-04-05 10:26:20.000000 dip-coater-0.2.0/src/dip_coater.egg-info/PKG-INFO
--rw-r--r--   0 rik      (459800007) staff       (20)      329 2024-04-05 10:26:20.000000 dip-coater-0.2.0/src/dip_coater.egg-info/SOURCES.txt
--rw-r--r--   0 rik      (459800007) staff       (20)        1 2024-04-05 10:26:20.000000 dip-coater-0.2.0/src/dip_coater.egg-info/dependency_links.txt
--rw-r--r--   0 rik      (459800007) staff       (20)       51 2024-04-05 10:26:20.000000 dip-coater-0.2.0/src/dip_coater.egg-info/entry_points.txt
--rw-r--r--   0 rik      (459800007) staff       (20)       48 2024-04-05 10:26:20.000000 dip-coater-0.2.0/src/dip_coater.egg-info/requires.txt
--rw-r--r--   0 rik      (459800007) staff       (20)       15 2024-04-05 10:26:20.000000 dip-coater-0.2.0/src/dip_coater.egg-info/top_level.txt
+drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 10:32:28.946227 dip-coater-0.3.0/
+-rw-r--r--   0 rik      (459800007) staff       (20)      100 2024-04-05 10:30:51.000000 dip-coater-0.3.0/MANIFEST.in
+-rw-r--r--   0 rik      (459800007) staff       (20)      269 2024-04-05 10:32:28.946051 dip-coater-0.3.0/PKG-INFO
+-rw-r--r--   0 rik      (459800007) staff       (20)      531 2024-04-05 10:32:26.000000 dip-coater-0.3.0/pyproject.toml
+-rw-r--r--   0 rik      (459800007) staff       (20)       38 2024-04-05 10:32:28.946276 dip-coater-0.3.0/setup.cfg
+drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 10:32:28.943965 dip-coater-0.3.0/src/
+drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 10:32:28.944787 dip-coater-0.3.0/src/dip_coater/
+-rw-r--r--   0 rik      (459800007) staff       (20)        0 2024-04-05 10:07:42.000000 dip-coater-0.3.0/src/dip_coater/__init__.py
+-rw-r--r--   0 rik      (459800007) staff       (20)     4293 2024-04-04 11:06:11.000000 dip-coater-0.3.0/src/dip_coater/motor.py
+-rw-r--r--   0 rik      (459800007) staff       (20)     8631 2024-04-05 10:10:36.000000 dip-coater-0.3.0/src/dip_coater/tui.py
+-rw-r--r--   0 rik      (459800007) staff       (20)     1443 2024-04-05 09:18:29.000000 dip-coater-0.3.0/src/dip_coater/tui.tcss
+drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 10:32:28.945793 dip-coater-0.3.0/src/dip_coater.egg-info/
+-rw-r--r--   0 rik      (459800007) staff       (20)      269 2024-04-05 10:32:28.000000 dip-coater-0.3.0/src/dip_coater.egg-info/PKG-INFO
+-rw-r--r--   0 rik      (459800007) staff       (20)      353 2024-04-05 10:32:28.000000 dip-coater-0.3.0/src/dip_coater.egg-info/SOURCES.txt
+-rw-r--r--   0 rik      (459800007) staff       (20)        1 2024-04-05 10:32:28.000000 dip-coater-0.3.0/src/dip_coater.egg-info/dependency_links.txt
+-rw-r--r--   0 rik      (459800007) staff       (20)       51 2024-04-05 10:32:28.000000 dip-coater-0.3.0/src/dip_coater.egg-info/entry_points.txt
+-rw-r--r--   0 rik      (459800007) staff       (20)       48 2024-04-05 10:32:28.000000 dip-coater-0.3.0/src/dip_coater.egg-info/requires.txt
+-rw-r--r--   0 rik      (459800007) staff       (20)       15 2024-04-05 10:32:28.000000 dip-coater-0.3.0/src/dip_coater.egg-info/top_level.txt
```

### Comparing `dip-coater-0.2.0/pyproject.toml` & `dip-coater-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dip-coater"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
     {name="Rik Huygen", email="rik.huygen@kuleuven.be"}
 ]
 requires-python = ">=3.8, <4.0"
 
 dependencies = [
     "textual",
@@ -22,10 +22,10 @@
 [project.scripts]
 dip-coater = "dip_coater.tui:main"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
-scripts = [
-    "**/*.tcss",
+dip_coater = [
+    "*.tcss",
 ]
```

### Comparing `dip-coater-0.2.0/src/dip_coater/motor.py` & `dip-coater-0.3.0/src/dip_coater/motor.py`

 * *Files identical despite different names*

### Comparing `dip-coater-0.2.0/src/dip_coater/tui.py` & `dip-coater-0.3.0/src/dip_coater/tui.py`

 * *Files identical despite different names*

