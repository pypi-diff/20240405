# Comparing `tmp/mlpro-int-sb3-0.1.0.tar.gz` & `tmp/mlpro-int-sb3-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpro-int-sb3-0.1.0.tar", last modified: Mon Apr  1 20:59:30 2024, max compression
+gzip compressed data, was "mlpro-int-sb3-0.1.1.tar", last modified: Fri Apr  5 09:20:07 2024, max compression
```

## Comparing `mlpro-int-sb3-0.1.0.tar` & `mlpro-int-sb3-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:59:30.780149 mlpro-int-sb3-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-01 20:59:26.000000 mlpro-int-sb3-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-01 20:59:30.780149 mlpro-int-sb3-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-01 20:59:26.000000 mlpro-int-sb3-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-01 20:59:26.000000 mlpro-int-sb3-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-01 20:59:30.780149 mlpro-int-sb3-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:59:30.776149 mlpro-int-sb3-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:59:30.780149 mlpro-int-sb3-0.1.0/src/mlpro_int_sb3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:59:26.000000 mlpro-int-sb3-0.1.0/src/mlpro_int_sb3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:59:30.780149 mlpro-int-sb3-0.1.0/src/mlpro_int_sb3/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-01 20:59:26.000000 mlpro-int-sb3-0.1.0/src/mlpro_int_sb3/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23250 2024-04-01 20:59:26.000000 mlpro-int-sb3-0.1.0/src/mlpro_int_sb3/wrappers/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:59:30.780149 mlpro-int-sb3-0.1.0/src/mlpro_int_sb3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-01 20:59:30.000000 mlpro-int-sb3-0.1.0/src/mlpro_int_sb3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-01 20:59:30.000000 mlpro-int-sb3-0.1.0/src/mlpro_int_sb3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:59:30.000000 mlpro-int-sb3-0.1.0/src/mlpro_int_sb3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-01 20:59:30.000000 mlpro-int-sb3-0.1.0/src/mlpro_int_sb3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 20:59:30.000000 mlpro-int-sb3-0.1.0/src/mlpro_int_sb3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:59:30.780149 mlpro-int-sb3-0.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-01 20:59:26.000000 mlpro-int-sb3-0.1.0/test/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)    10795 2024-04-01 20:59:26.000000 mlpro-int-sb3-0.1.0/test/test_sb3_policy_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:20:07.417007 mlpro-int-sb3-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-05 09:19:59.000000 mlpro-int-sb3-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-05 09:20:07.417007 mlpro-int-sb3-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-05 09:19:59.000000 mlpro-int-sb3-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-05 09:19:59.000000 mlpro-int-sb3-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-05 09:20:07.421007 mlpro-int-sb3-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:20:07.413007 mlpro-int-sb3-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:20:07.417007 mlpro-int-sb3-0.1.1/src/mlpro_int_sb3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:19:59.000000 mlpro-int-sb3-0.1.1/src/mlpro_int_sb3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:20:07.417007 mlpro-int-sb3-0.1.1/src/mlpro_int_sb3/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-05 09:19:59.000000 mlpro-int-sb3-0.1.1/src/mlpro_int_sb3/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23250 2024-04-05 09:19:59.000000 mlpro-int-sb3-0.1.1/src/mlpro_int_sb3/wrappers/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:20:07.417007 mlpro-int-sb3-0.1.1/src/mlpro_int_sb3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-05 09:20:07.000000 mlpro-int-sb3-0.1.1/src/mlpro_int_sb3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-05 09:20:07.000000 mlpro-int-sb3-0.1.1/src/mlpro_int_sb3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 09:20:07.000000 mlpro-int-sb3-0.1.1/src/mlpro_int_sb3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-05 09:20:07.000000 mlpro-int-sb3-0.1.1/src/mlpro_int_sb3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 09:20:07.000000 mlpro-int-sb3-0.1.1/src/mlpro_int_sb3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:20:07.417007 mlpro-int-sb3-0.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-05 09:19:59.000000 mlpro-int-sb3-0.1.1/test/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10795 2024-04-05 09:19:59.000000 mlpro-int-sb3-0.1.1/test/test_sb3_policy_wrapper.py
```

### Comparing `mlpro-int-sb3-0.1.0/LICENSE` & `mlpro-int-sb3-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpro-int-sb3-0.1.0/PKG-INFO` & `mlpro-int-sb3-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpro-int-sb3
-Version: 0.1.0
+Version: 0.1.1
 Summary: MLPro: Integration StableBaselines3
 Home-page: https://mlpro-int-sb3.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro-int-sb3.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mlpro-int-sb3-0.1.0/README.md` & `mlpro-int-sb3-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mlpro-int-sb3-0.1.0/setup.cfg` & `mlpro-int-sb3-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mlpro-int-sb3
-version = 0.1.0
+version = 0.1.1
 author = MLPro Team
 author_email = mlpro@listen.fh-swf.de
 description = MLPro: Integration StableBaselines3
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://mlpro-int-sb3.readthedocs.io
 project_urls =
```

### Comparing `mlpro-int-sb3-0.1.0/src/mlpro_int_sb3/wrappers/basics.py` & `mlpro-int-sb3-0.1.1/src/mlpro_int_sb3/wrappers/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-int-sb3-0.1.0/src/mlpro_int_sb3.egg-info/PKG-INFO` & `mlpro-int-sb3-0.1.1/src/mlpro_int_sb3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpro-int-sb3
-Version: 0.1.0
+Version: 0.1.1
 Summary: MLPro: Integration StableBaselines3
 Home-page: https://mlpro-int-sb3.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro-int-sb3.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mlpro-int-sb3-0.1.0/test/test_examples.py` & `mlpro-int-sb3-0.1.1/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `mlpro-int-sb3-0.1.0/test/test_sb3_policy_wrapper.py` & `mlpro-int-sb3-0.1.1/test/test_sb3_policy_wrapper.py`

 * *Files identical despite different names*

