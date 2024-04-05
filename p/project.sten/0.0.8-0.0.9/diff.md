# Comparing `tmp/project.sten-0.0.8.tar.gz` & `tmp/project.sten-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project.sten-0.0.8.tar", last modified: Wed Mar 20 06:32:14 2024, max compression
+gzip compressed data, was "project.sten-0.0.9.tar", last modified: Fri Apr  5 01:40:37 2024, max compression
```

## Comparing `project.sten-0.0.8.tar` & `project.sten-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 serhat    (1000) serhat    (1000)        0 2024-03-20 06:32:14.776867 project.sten-0.0.8/
--rw-r--r--   0 serhat    (1000) serhat    (1000)    35823 2024-03-20 06:31:54.000000 project.sten-0.0.8/LICENSE
--rw-r--r--   0 serhat    (1000) serhat    (1000)      907 2024-03-20 06:32:14.776867 project.sten-0.0.8/PKG-INFO
-drwxr-xr-x   0 serhat    (1000) serhat    (1000)        0 2024-03-20 06:32:14.776867 project.sten-0.0.8/project.sten.egg-info/
--rw-r--r--   0 serhat    (1000) serhat    (1000)      907 2024-03-20 06:32:14.000000 project.sten-0.0.8/project.sten.egg-info/PKG-INFO
--rw-r--r--   0 serhat    (1000) serhat    (1000)      446 2024-03-20 06:32:14.000000 project.sten-0.0.8/project.sten.egg-info/SOURCES.txt
--rw-r--r--   0 serhat    (1000) serhat    (1000)        1 2024-03-20 06:32:14.000000 project.sten-0.0.8/project.sten.egg-info/dependency_links.txt
--rw-r--r--   0 serhat    (1000) serhat    (1000)       40 2024-03-20 06:32:14.000000 project.sten-0.0.8/project.sten.egg-info/entry_points.txt
--rw-r--r--   0 serhat    (1000) serhat    (1000)        1 2024-03-20 06:32:14.000000 project.sten-0.0.8/project.sten.egg-info/not-zip-safe
--rw-r--r--   0 serhat    (1000) serhat    (1000)       47 2024-03-20 06:32:14.000000 project.sten-0.0.8/project.sten.egg-info/requires.txt
--rw-r--r--   0 serhat    (1000) serhat    (1000)        5 2024-03-20 06:32:14.000000 project.sten-0.0.8/project.sten.egg-info/top_level.txt
--rw-r--r--   0 serhat    (1000) serhat    (1000)     1145 2024-03-20 06:31:54.000000 project.sten-0.0.8/pyproject.toml
--rw-r--r--   0 serhat    (1000) serhat    (1000)       50 2024-03-20 06:31:54.000000 project.sten-0.0.8/requirements.txt
--rw-r--r--   0 serhat    (1000) serhat    (1000)       38 2024-03-20 06:32:14.776867 project.sten-0.0.8/setup.cfg
-drwxr-xr-x   0 serhat    (1000) serhat    (1000)        0 2024-03-20 06:32:14.776867 project.sten-0.0.8/sten/
--rw-r--r--   0 serhat    (1000) serhat    (1000)        0 2024-03-20 06:31:54.000000 project.sten-0.0.8/sten/__init__.py
--rw-r--r--   0 serhat    (1000) serhat    (1000)    33136 2024-03-20 06:31:54.000000 project.sten-0.0.8/sten/__main__.py
--rw-r--r--   0 serhat    (1000) serhat    (1000)       80 2024-03-20 06:31:54.000000 project.sten-0.0.8/sten/__version__.py
--rw-r--r--   0 serhat    (1000) serhat    (1000)      753 2024-03-20 06:31:54.000000 project.sten-0.0.8/sten/config.py
--rw-r--r--   0 serhat    (1000) serhat    (1000)     1308 2024-03-20 06:31:54.000000 project.sten-0.0.8/sten/consts.py
--rw-r--r--   0 serhat    (1000) serhat    (1000)     7108 2024-03-20 06:31:54.000000 project.sten-0.0.8/sten/crypto.py
--rw-r--r--   0 serhat    (1000) serhat    (1000)     1686 2024-03-20 06:31:54.000000 project.sten-0.0.8/sten/data.py
--rw-r--r--   0 serhat    (1000) serhat    (1000)      202 2024-03-20 06:31:54.000000 project.sten-0.0.8/sten/error.py
--rw-r--r--   0 serhat    (1000) serhat    (1000)     6862 2024-03-20 06:31:54.000000 project.sten-0.0.8/sten/icons.py
--rw-r--r--   0 serhat    (1000) serhat    (1000)      590 2024-03-20 06:31:54.000000 project.sten-0.0.8/sten/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-05 01:40:37.013916 project.sten-0.0.9/
+-rw-rw-rw-   0        0        0    35823 2024-04-05 01:38:23.000000 project.sten-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      930 2024-04-05 01:40:37.013916 project.sten-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-04-05 01:38:23.000000 project.sten-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 01:40:37.013916 project.sten-0.0.9/project.sten.egg-info/
+-rw-rw-rw-   0        0        0      930 2024-04-05 01:40:36.000000 project.sten-0.0.9/project.sten.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2024-04-05 01:40:36.000000 project.sten-0.0.9/project.sten.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 01:40:36.000000 project.sten-0.0.9/project.sten.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-05 01:40:36.000000 project.sten-0.0.9/project.sten.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-05 01:40:36.000000 project.sten-0.0.9/project.sten.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       47 2024-04-05 01:40:36.000000 project.sten-0.0.9/project.sten.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-05 01:40:36.000000 project.sten-0.0.9/project.sten.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1145 2024-04-05 01:38:23.000000 project.sten-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       50 2024-04-05 01:38:23.000000 project.sten-0.0.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 01:40:37.013916 project.sten-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 01:40:37.010212 project.sten-0.0.9/sten/
+-rw-rw-rw-   0        0        0        0 2024-04-05 01:38:23.000000 project.sten-0.0.9/sten/__init__.py
+-rw-rw-rw-   0        0        0    33136 2024-04-05 01:38:23.000000 project.sten-0.0.9/sten/__main__.py
+-rw-rw-rw-   0        0        0       80 2024-04-05 01:38:23.000000 project.sten-0.0.9/sten/__version__.py
+-rw-rw-rw-   0        0        0      753 2024-04-05 01:38:23.000000 project.sten-0.0.9/sten/config.py
+-rw-rw-rw-   0        0        0     1308 2024-04-05 01:38:23.000000 project.sten-0.0.9/sten/consts.py
+-rw-rw-rw-   0        0        0     7108 2024-04-05 01:38:23.000000 project.sten-0.0.9/sten/crypto.py
+-rw-rw-rw-   0        0        0     1686 2024-04-05 01:38:23.000000 project.sten-0.0.9/sten/data.py
+-rw-rw-rw-   0        0        0      202 2024-04-05 01:38:23.000000 project.sten-0.0.9/sten/error.py
+-rw-rw-rw-   0        0        0     6862 2024-04-05 01:38:23.000000 project.sten-0.0.9/sten/icons.py
+-rw-rw-rw-   0        0        0      590 2024-04-05 01:38:23.000000 project.sten-0.0.9/sten/utils.py
```

### Comparing `project.sten-0.0.8/LICENSE` & `project.sten-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `project.sten-0.0.8/pyproject.toml` & `project.sten-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `project.sten-0.0.8/sten/__main__.py` & `project.sten-0.0.9/sten/__main__.py`

 * *Files identical despite different names*

### Comparing `project.sten-0.0.8/sten/config.py` & `project.sten-0.0.9/sten/config.py`

 * *Files identical despite different names*

### Comparing `project.sten-0.0.8/sten/consts.py` & `project.sten-0.0.9/sten/consts.py`

 * *Files identical despite different names*

### Comparing `project.sten-0.0.8/sten/crypto.py` & `project.sten-0.0.9/sten/crypto.py`

 * *Files identical despite different names*

### Comparing `project.sten-0.0.8/sten/data.py` & `project.sten-0.0.9/sten/data.py`

 * *Files identical despite different names*

### Comparing `project.sten-0.0.8/sten/icons.py` & `project.sten-0.0.9/sten/icons.py`

 * *Files identical despite different names*

### Comparing `project.sten-0.0.8/sten/utils.py` & `project.sten-0.0.9/sten/utils.py`

 * *Files identical despite different names*

