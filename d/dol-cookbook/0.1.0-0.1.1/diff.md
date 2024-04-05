# Comparing `tmp/dol_cookbook-0.1.0.tar.gz` & `tmp/dol_cookbook-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dol_cookbook-0.1.0.tar", last modified: Wed Apr  3 12:27:23 2024, max compression
+gzip compressed data, was "dol_cookbook-0.1.1.tar", last modified: Fri Apr  5 10:09:28 2024, max compression
```

## Comparing `dol_cookbook-0.1.0.tar` & `dol_cookbook-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:27:23.421945 dol_cookbook-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 12:26:40.000000 dol_cookbook-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-03 12:27:23.421945 dol_cookbook-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-03 12:26:40.000000 dol_cookbook-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:27:23.421945 dol_cookbook-0.1.0/dol_cookbook/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 12:26:40.000000 dol_cookbook-0.1.0/dol_cookbook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-03 12:26:56.000000 dol_cookbook-0.1.0/dol_cookbook/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:27:23.421945 dol_cookbook-0.1.0/dol_cookbook.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-03 12:27:23.000000 dol_cookbook-0.1.0/dol_cookbook.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-03 12:27:23.000000 dol_cookbook-0.1.0/dol_cookbook.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:27:23.000000 dol_cookbook-0.1.0/dol_cookbook.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:27:23.000000 dol_cookbook-0.1.0/dol_cookbook.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 12:27:23.000000 dol_cookbook-0.1.0/dol_cookbook.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-03 12:27:23.421945 dol_cookbook-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 12:26:40.000000 dol_cookbook-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:09:28.722408 dol_cookbook-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-05 10:09:03.000000 dol_cookbook-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-05 10:09:28.722408 dol_cookbook-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-05 10:09:03.000000 dol_cookbook-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:09:28.722408 dol_cookbook-0.1.1/dol_cookbook/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-05 10:09:03.000000 dol_cookbook-0.1.1/dol_cookbook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-05 10:09:08.000000 dol_cookbook-0.1.1/dol_cookbook/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:09:28.722408 dol_cookbook-0.1.1/dol_cookbook.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-05 10:09:28.000000 dol_cookbook-0.1.1/dol_cookbook.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-05 10:09:28.000000 dol_cookbook-0.1.1/dol_cookbook.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 10:09:28.000000 dol_cookbook-0.1.1/dol_cookbook.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 10:09:28.000000 dol_cookbook-0.1.1/dol_cookbook.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 10:09:28.000000 dol_cookbook-0.1.1/dol_cookbook.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-05 10:09:28.722408 dol_cookbook-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-05 10:09:03.000000 dol_cookbook-0.1.1/setup.py
```

### Comparing `dol_cookbook-0.1.0/LICENSE` & `dol_cookbook-0.1.1/LICENSE`

 * *Files identical despite different names*

