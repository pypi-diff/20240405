# Comparing `tmp/fidelius-0.5.0.tar.gz` & `tmp/fidelius-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fidelius-0.5.0.tar", last modified: Fri Apr  5 15:31:18 2024, max compression
+gzip compressed data, was "fidelius-0.6.0.tar", last modified: Fri Apr  5 16:56:16 2024, max compression
```

## Comparing `fidelius-0.5.0.tar` & `fidelius-0.6.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:31:18.309897 fidelius-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 15:31:04.000000 fidelius-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16861 2024-04-05 15:31:18.309897 fidelius-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14208 2024-04-05 15:31:04.000000 fidelius-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:31:18.305897 fidelius-0.5.0/fidelius/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-05 15:31:04.000000 fidelius-0.5.0/fidelius/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:31:18.305897 fidelius-0.5.0/fidelius/fideliusapi/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-05 15:31:04.000000 fidelius-0.5.0/fidelius/fideliusapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:31:18.305897 fidelius-0.5.0/fidelius/gateway/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:31:04.000000 fidelius-0.5.0/fidelius/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-05 15:31:04.000000 fidelius-0.5.0/fidelius/gateway/paramadmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-04-05 15:31:04.000000 fidelius-0.5.0/fidelius/gateway/paramstore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:31:18.309897 fidelius-0.5.0/fidelius/structs/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 15:31:04.000000 fidelius-0.5.0/fidelius/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 15:31:04.000000 fidelius-0.5.0/fidelius/structs/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-05 15:31:04.000000 fidelius-0.5.0/fidelius/structs/_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:31:18.309897 fidelius-0.5.0/fidelius/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 15:31:04.000000 fidelius-0.5.0/fidelius/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-05 15:31:04.000000 fidelius-0.5.0/fidelius/utils/replacer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:31:18.309897 fidelius-0.5.0/fidelius.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16861 2024-04-05 15:31:18.000000 fidelius-0.5.0/fidelius.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-05 15:31:18.000000 fidelius-0.5.0/fidelius.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:31:18.000000 fidelius-0.5.0/fidelius.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-05 15:31:18.000000 fidelius-0.5.0/fidelius.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 15:31:18.000000 fidelius-0.5.0/fidelius.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-05 15:31:04.000000 fidelius-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 15:31:18.309897 fidelius-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-05 15:31:04.000000 fidelius-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:56:16.104496 fidelius-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 16:56:05.000000 fidelius-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16861 2024-04-05 16:56:16.104496 fidelius-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14208 2024-04-05 16:56:05.000000 fidelius-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:56:16.104496 fidelius-0.6.0/fidelius/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-05 16:56:05.000000 fidelius-0.6.0/fidelius/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:56:16.104496 fidelius-0.6.0/fidelius/fideliusapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-05 16:56:05.000000 fidelius-0.6.0/fidelius/fideliusapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:56:16.104496 fidelius-0.6.0/fidelius/gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:56:05.000000 fidelius-0.6.0/fidelius/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-05 16:56:05.000000 fidelius-0.6.0/fidelius/gateway/paramadmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-04-05 16:56:05.000000 fidelius-0.6.0/fidelius/gateway/paramstore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:56:16.104496 fidelius-0.6.0/fidelius/structs/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 16:56:05.000000 fidelius-0.6.0/fidelius/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:56:05.000000 fidelius-0.6.0/fidelius/structs/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-05 16:56:05.000000 fidelius-0.6.0/fidelius/structs/_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:56:16.104496 fidelius-0.6.0/fidelius/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 16:56:05.000000 fidelius-0.6.0/fidelius/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-05 16:56:05.000000 fidelius-0.6.0/fidelius/utils/replacer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:56:16.104496 fidelius-0.6.0/fidelius.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16861 2024-04-05 16:56:16.000000 fidelius-0.6.0/fidelius.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-05 16:56:16.000000 fidelius-0.6.0/fidelius.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:56:16.000000 fidelius-0.6.0/fidelius.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-05 16:56:16.000000 fidelius-0.6.0/fidelius.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 16:56:16.000000 fidelius-0.6.0/fidelius.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-05 16:56:05.000000 fidelius-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:56:16.104496 fidelius-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-05 16:56:05.000000 fidelius-0.6.0/setup.py
```

### Comparing `fidelius-0.5.0/LICENSE` & `fidelius-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fidelius-0.5.0/PKG-INFO` & `fidelius-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fidelius
-Version: 0.5.0
+Version: 0.6.0
 Summary: The Fidelius Charm! (keeping things secret)
 Author-email: Thordur Matthiasson <thordurm@ccpgames.com>, Kristin Fjola Tomasdottir <kristinf@ccpgames.com>
 License: MIT License
         
         Copyright (c) 2022-2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fidelius-0.5.0/README.md` & `fidelius-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `fidelius-0.5.0/fidelius/gateway/paramadmin.py` & `fidelius-0.6.0/fidelius/gateway/paramadmin.py`

 * *Files identical despite different names*

### Comparing `fidelius-0.5.0/fidelius/gateway/paramstore.py` & `fidelius-0.6.0/fidelius/gateway/paramstore.py`

 * *Files identical despite different names*

### Comparing `fidelius-0.5.0/fidelius/structs/_tags.py` & `fidelius-0.6.0/fidelius/structs/_tags.py`

 * *Files identical despite different names*

### Comparing `fidelius-0.5.0/fidelius.egg-info/PKG-INFO` & `fidelius-0.6.0/fidelius.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fidelius
-Version: 0.5.0
+Version: 0.6.0
 Summary: The Fidelius Charm! (keeping things secret)
 Author-email: Thordur Matthiasson <thordurm@ccpgames.com>, Kristin Fjola Tomasdottir <kristinf@ccpgames.com>
 License: MIT License
         
         Copyright (c) 2022-2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fidelius-0.5.0/pyproject.toml` & `fidelius-0.6.0/pyproject.toml`

 * *Files identical despite different names*

