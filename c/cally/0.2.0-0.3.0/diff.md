# Comparing `tmp/cally-0.2.0.tar.gz` & `tmp/cally-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cally-0.2.0.tar", last modified: Sat Mar 30 05:35:10 2024, max compression
+gzip compressed data, was "cally-0.3.0.tar", last modified: Fri Apr  5 09:41:52 2024, max compression
```

## Comparing `cally-0.2.0.tar` & `cally-0.3.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 05:35:10.248362 cally-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-03-30 05:35:06.000000 cally-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    27147 2024-03-30 05:35:10.248362 cally-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-03-30 05:35:06.000000 cally-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-03-30 05:35:06.000000 cally-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 05:35:10.248362 cally-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 05:35:10.240363 cally-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 05:35:10.240363 cally-0.2.0/src/cally/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 05:35:10.240363 cally-0.2.0/src/cally/cdk/
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-03-30 05:35:06.000000 cally-0.2.0/src/cally/cdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 05:35:06.000000 cally-0.2.0/src/cally/cdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 05:35:10.244362 cally-0.2.0/src/cally/cdk/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 05:35:06.000000 cally-0.2.0/src/cally/cdk/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 05:35:10.244362 cally-0.2.0/src/cally/cdk/stacks/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-03-30 05:35:06.000000 cally-0.2.0/src/cally/cdk/stacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 05:35:10.244362 cally-0.2.0/src/cally/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-03-30 05:35:06.000000 cally-0.2.0/src/cally/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-30 05:35:06.000000 cally-0.2.0/src/cally/cli/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 05:35:10.244362 cally-0.2.0/src/cally/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 05:35:06.000000 cally-0.2.0/src/cally/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-30 05:35:06.000000 cally-0.2.0/src/cally/cli/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-30 05:35:06.000000 cally-0.2.0/src/cally/cli/commands/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-03-30 05:35:06.000000 cally-0.2.0/src/cally/cli/commands/tf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 05:35:10.244362 cally-0.2.0/src/cally/cli/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-03-30 05:35:06.000000 cally-0.2.0/src/cally/cli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-03-30 05:35:06.000000 cally-0.2.0/src/cally/cli/config/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-03-30 05:35:06.000000 cally-0.2.0/src/cally/cli/config/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-03-30 05:35:06.000000 cally-0.2.0/src/cally/cli/config/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-30 05:35:06.000000 cally-0.2.0/src/cally/cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 05:35:06.000000 cally-0.2.0/src/cally/cli/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 05:35:10.244362 cally-0.2.0/src/cally/cli/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 05:35:06.000000 cally-0.2.0/src/cally/cli/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-03-30 05:35:06.000000 cally-0.2.0/src/cally/cli/tools/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-03-30 05:35:06.000000 cally-0.2.0/src/cally/cli/tools/terraform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 05:35:10.244362 cally-0.2.0/src/cally/testing/
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-03-30 05:35:06.000000 cally-0.2.0/src/cally/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-30 05:35:06.000000 cally-0.2.0/src/cally/testing/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-30 05:35:06.000000 cally-0.2.0/src/cally/testing/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 05:35:06.000000 cally-0.2.0/src/cally/testing/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 05:35:10.244362 cally-0.2.0/src/cally.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27147 2024-03-30 05:35:10.000000 cally-0.2.0/src/cally.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-30 05:35:10.000000 cally-0.2.0/src/cally.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 05:35:10.000000 cally-0.2.0/src/cally.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-30 05:35:10.000000 cally-0.2.0/src/cally.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-30 05:35:10.000000 cally-0.2.0/src/cally.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-30 05:35:10.000000 cally-0.2.0/src/cally.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:52.818641 cally-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-05 09:41:45.000000 cally-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    27147 2024-04-05 09:41:52.818641 cally-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-04-05 09:41:45.000000 cally-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-05 09:41:45.000000 cally-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 09:41:52.818641 cally-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:52.810641 cally-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:52.810641 cally-0.3.0/src/cally/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:52.814641 cally-0.3.0/src/cally/cdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:52.814641 cally-0.3.0/src/cally/cdk/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cdk/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:52.814641 cally-0.3.0/src/cally/cdk/stacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cdk/stacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:52.814641 cally-0.3.0/src/cally/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:52.814641 cally-0.3.0/src/cally/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/commands/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/commands/tf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:52.814641 cally-0.3.0/src/cally/cli/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/config/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/config/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/config/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:52.818641 cally-0.3.0/src/cally/cli/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/tools/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/tools/terraform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:52.818641 cally-0.3.0/src/cally/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/testing/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/testing/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/testing/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:52.818641 cally-0.3.0/src/cally.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27147 2024-04-05 09:41:52.000000 cally-0.3.0/src/cally.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-05 09:41:52.000000 cally-0.3.0/src/cally.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 09:41:52.000000 cally-0.3.0/src/cally.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 09:41:52.000000 cally-0.3.0/src/cally.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-05 09:41:52.000000 cally-0.3.0/src/cally.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 09:41:52.000000 cally-0.3.0/src/cally.egg-info/top_level.txt
```

### Comparing `cally-0.2.0/LICENSE` & `cally-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cally-0.2.0/PKG-INFO` & `cally-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cally
-Version: 0.2.0
+Version: 0.3.0
 Summary: A config as infrastructure foundation for your Internal Developer Platform
 Author-email: Leon Wright <techman83@gmail.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

### Comparing `cally-0.2.0/README.md` & `cally-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cally-0.2.0/pyproject.toml` & `cally-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cally-0.2.0/src/cally/cdk/stacks/__init__.py` & `cally-0.3.0/src/cally/cdk/stacks/__init__.py`

 * *Files identical despite different names*

### Comparing `cally-0.2.0/src/cally/cli/__init__.py` & `cally-0.3.0/src/cally/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cally-0.2.0/src/cally/cli/commands/tf.py` & `cally-0.3.0/src/cally/cli/commands/tf.py`

 * *Files identical despite different names*

### Comparing `cally-0.2.0/src/cally/cli/config/__init__.py` & `cally-0.3.0/src/cally/cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cally-0.2.0/src/cally/cli/config/loader.py` & `cally-0.3.0/src/cally/cli/config/loader.py`

 * *Files identical despite different names*

### Comparing `cally-0.2.0/src/cally/cli/config/types.py` & `cally-0.3.0/src/cally/cli/config/types.py`

 * *Files identical despite different names*

### Comparing `cally-0.2.0/src/cally/cli/config/validators.py` & `cally-0.3.0/src/cally/cli/config/validators.py`

 * *Files identical despite different names*

### Comparing `cally-0.2.0/src/cally/cli/constants.py` & `cally-0.3.0/src/cally/cli/constants.py`

 * *Files identical despite different names*

### Comparing `cally-0.2.0/src/cally/cli/tools/provider.py` & `cally-0.3.0/src/cally/cli/tools/provider.py`

 * *Files identical despite different names*

### Comparing `cally-0.2.0/src/cally/cli/tools/terraform.py` & `cally-0.3.0/src/cally/cli/tools/terraform.py`

 * *Files identical despite different names*

### Comparing `cally-0.2.0/src/cally/testing/__init__.py` & `cally-0.3.0/src/cally/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `cally-0.2.0/src/cally.egg-info/PKG-INFO` & `cally-0.3.0/src/cally.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cally
-Version: 0.2.0
+Version: 0.3.0
 Summary: A config as infrastructure foundation for your Internal Developer Platform
 Author-email: Leon Wright <techman83@gmail.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

### Comparing `cally-0.2.0/src/cally.egg-info/SOURCES.txt` & `cally-0.3.0/src/cally.egg-info/SOURCES.txt`

 * *Files identical despite different names*

