# Comparing `tmp/schedulefree-1.0.tar.gz` & `tmp/schedulefree-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schedulefree-1.0.tar", last modified: Fri Apr  5 14:52:11 2024, max compression
+gzip compressed data, was "schedulefree-1.1.tar", last modified: Fri Apr  5 14:56:25 2024, max compression
```

## Comparing `schedulefree-1.0.tar` & `schedulefree-1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2024-04-05 14:52:11.124571 schedulefree-1.0/
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)    11356 2024-04-01 19:27:30.000000 schedulefree-1.0/LICENSE
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     6626 2024-04-05 14:52:11.125817 schedulefree-1.0/PKG-INFO
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     6170 2024-04-05 14:28:11.000000 schedulefree-1.0/README.md
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      303 2024-04-01 19:31:49.000000 schedulefree-1.0/pyproject.toml
-drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2024-04-05 14:52:11.104411 schedulefree-1.0/schedulefree/
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      416 2024-04-04 14:32:58.000000 schedulefree-1.0/schedulefree/__init__.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     5744 2024-04-04 15:51:08.000000 schedulefree-1.0/schedulefree/adamw_schedulefree.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     5035 2024-04-04 15:52:02.000000 schedulefree-1.0/schedulefree/adamw_schedulefree_closure.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     5325 2024-04-04 14:49:28.000000 schedulefree-1.0/schedulefree/sgd_schedulefree.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     4571 2024-04-04 15:54:19.000000 schedulefree-1.0/schedulefree/sgd_schedulefree_closure.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     3617 2024-04-04 17:59:14.000000 schedulefree-1.0/schedulefree/test_schedulefree.py
-drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2024-04-05 14:52:11.120453 schedulefree-1.0/schedulefree.egg-info/
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     6626 2024-04-05 14:52:10.000000 schedulefree-1.0/schedulefree.egg-info/PKG-INFO
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      406 2024-04-05 14:52:11.000000 schedulefree-1.0/schedulefree.egg-info/SOURCES.txt
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)        1 2024-04-05 14:52:10.000000 schedulefree-1.0/schedulefree.egg-info/dependency_links.txt
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       13 2024-04-05 14:52:10.000000 schedulefree-1.0/schedulefree.egg-info/top_level.txt
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       79 2024-04-05 14:52:11.129362 schedulefree-1.0/setup.cfg
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      889 2024-04-01 19:30:53.000000 schedulefree-1.0/setup.py
+drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2024-04-05 14:56:25.734014 schedulefree-1.1/
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)    11356 2024-04-01 19:27:30.000000 schedulefree-1.1/LICENSE
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     6626 2024-04-05 14:56:25.735133 schedulefree-1.1/PKG-INFO
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     6170 2024-04-05 14:28:11.000000 schedulefree-1.1/README.md
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      303 2024-04-01 19:31:49.000000 schedulefree-1.1/pyproject.toml
+drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2024-04-05 14:56:25.713160 schedulefree-1.1/schedulefree/
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      420 2024-04-05 14:54:15.000000 schedulefree-1.1/schedulefree/__init__.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     5744 2024-04-04 15:51:08.000000 schedulefree-1.1/schedulefree/adamw_schedulefree.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     5035 2024-04-04 15:52:02.000000 schedulefree-1.1/schedulefree/adamw_schedulefree_closure.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     5325 2024-04-04 14:49:28.000000 schedulefree-1.1/schedulefree/sgd_schedulefree.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     4571 2024-04-04 15:54:19.000000 schedulefree-1.1/schedulefree/sgd_schedulefree_closure.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     3617 2024-04-04 17:59:14.000000 schedulefree-1.1/schedulefree/test_schedulefree.py
+drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2024-04-05 14:56:25.729130 schedulefree-1.1/schedulefree.egg-info/
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     6626 2024-04-05 14:56:25.000000 schedulefree-1.1/schedulefree.egg-info/PKG-INFO
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      406 2024-04-05 14:56:25.000000 schedulefree-1.1/schedulefree.egg-info/SOURCES.txt
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)        1 2024-04-05 14:56:25.000000 schedulefree-1.1/schedulefree.egg-info/dependency_links.txt
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       13 2024-04-05 14:56:25.000000 schedulefree-1.1/schedulefree.egg-info/top_level.txt
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       79 2024-04-05 14:56:25.738262 schedulefree-1.1/setup.cfg
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      889 2024-04-05 14:55:56.000000 schedulefree-1.1/setup.py
```

### Comparing `schedulefree-1.0/LICENSE` & `schedulefree-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `schedulefree-1.0/PKG-INFO` & `schedulefree-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schedulefree
-Version: 1.0
+Version: 1.1
 Summary: Schedule Free Learning in PyTorch
 Home-page: https://github.com/facebookresearch/schedule_free
 Author: Aaron Defazio
 Author-email: adefazio@meta.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `schedulefree-1.0/README.md` & `schedulefree-1.1/README.md`

 * *Files identical despite different names*

### Comparing `schedulefree-1.0/schedulefree/adamw_schedulefree.py` & `schedulefree-1.1/schedulefree/adamw_schedulefree.py`

 * *Files identical despite different names*

### Comparing `schedulefree-1.0/schedulefree/adamw_schedulefree_closure.py` & `schedulefree-1.1/schedulefree/adamw_schedulefree_closure.py`

 * *Files identical despite different names*

### Comparing `schedulefree-1.0/schedulefree/sgd_schedulefree.py` & `schedulefree-1.1/schedulefree/sgd_schedulefree.py`

 * *Files identical despite different names*

### Comparing `schedulefree-1.0/schedulefree/sgd_schedulefree_closure.py` & `schedulefree-1.1/schedulefree/sgd_schedulefree_closure.py`

 * *Files identical despite different names*

### Comparing `schedulefree-1.0/schedulefree/test_schedulefree.py` & `schedulefree-1.1/schedulefree/test_schedulefree.py`

 * *Files identical despite different names*

### Comparing `schedulefree-1.0/schedulefree.egg-info/PKG-INFO` & `schedulefree-1.1/schedulefree.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schedulefree
-Version: 1.0
+Version: 1.1
 Summary: Schedule Free Learning in PyTorch
 Home-page: https://github.com/facebookresearch/schedule_free
 Author: Aaron Defazio
 Author-email: adefazio@meta.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `schedulefree-1.0/setup.py` & `schedulefree-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="schedulefree",
-    version="1.0",
+    version="1.1",
     author="Aaron Defazio",
     author_email="adefazio@meta.com",
     description="Schedule Free Learning in PyTorch",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/facebookresearch/schedule_free",
     packages=setuptools.find_packages(),
```

