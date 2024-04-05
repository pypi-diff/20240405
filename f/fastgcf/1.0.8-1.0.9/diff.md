# Comparing `tmp/fastgcf-1.0.8.tar.gz` & `tmp/fastgcf-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastgcf-1.0.8.tar", last modified: Mon Mar 11 15:21:04 2024, max compression
+gzip compressed data, was "fastgcf-1.0.9.tar", last modified: Fri Apr  5 11:21:47 2024, max compression
```

## Comparing `fastgcf-1.0.8.tar` & `fastgcf-1.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:21:04.821632 fastgcf-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:21:04.817632 fastgcf-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:21:04.821632 fastgcf-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-11 15:20:57.000000 fastgcf-1.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-03-11 15:20:57.000000 fastgcf-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-11 15:20:57.000000 fastgcf-1.0.8/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-03-11 15:21:04.821632 fastgcf-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-03-11 15:20:57.000000 fastgcf-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:21:04.821632 fastgcf-1.0.8/fastgcf/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-11 15:20:57.000000 fastgcf-1.0.8/fastgcf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-03-11 15:20:57.000000 fastgcf-1.0.8/fastgcf/_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-03-11 15:20:57.000000 fastgcf-1.0.8/fastgcf/_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-03-11 15:20:57.000000 fastgcf-1.0.8/fastgcf/_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-03-11 15:20:57.000000 fastgcf-1.0.8/fastgcf/_router.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-03-11 15:20:57.000000 fastgcf-1.0.8/fastgcf/_streams.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-03-11 15:20:57.000000 fastgcf-1.0.8/fastgcf/_transport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:21:04.821632 fastgcf-1.0.8/fastgcf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-03-11 15:21:04.000000 fastgcf-1.0.8/fastgcf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-11 15:21:04.000000 fastgcf-1.0.8/fastgcf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 15:21:04.000000 fastgcf-1.0.8/fastgcf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-11 15:21:04.000000 fastgcf-1.0.8/fastgcf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-11 15:21:04.000000 fastgcf-1.0.8/fastgcf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-11 15:20:57.000000 fastgcf-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-11 15:20:57.000000 fastgcf-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 15:21:04.821632 fastgcf-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-03-11 15:20:57.000000 fastgcf-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:21:47.568238 fastgcf-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:21:47.564238 fastgcf-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:21:47.568238 fastgcf-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-05 11:21:43.000000 fastgcf-1.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-05 11:21:43.000000 fastgcf-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-05 11:21:43.000000 fastgcf-1.0.9/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-04-05 11:21:47.568238 fastgcf-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-04-05 11:21:43.000000 fastgcf-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:21:47.568238 fastgcf-1.0.9/fastgcf/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-05 11:21:43.000000 fastgcf-1.0.9/fastgcf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-05 11:21:43.000000 fastgcf-1.0.9/fastgcf/_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-05 11:21:43.000000 fastgcf-1.0.9/fastgcf/_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-05 11:21:43.000000 fastgcf-1.0.9/fastgcf/_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-05 11:21:43.000000 fastgcf-1.0.9/fastgcf/_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-05 11:21:43.000000 fastgcf-1.0.9/fastgcf/_streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-05 11:21:43.000000 fastgcf-1.0.9/fastgcf/_transport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:21:47.568238 fastgcf-1.0.9/fastgcf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-04-05 11:21:47.000000 fastgcf-1.0.9/fastgcf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-05 11:21:47.000000 fastgcf-1.0.9/fastgcf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 11:21:47.000000 fastgcf-1.0.9/fastgcf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-05 11:21:47.000000 fastgcf-1.0.9/fastgcf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 11:21:47.000000 fastgcf-1.0.9/fastgcf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-05 11:21:43.000000 fastgcf-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-05 11:21:43.000000 fastgcf-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 11:21:47.568238 fastgcf-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-05 11:21:43.000000 fastgcf-1.0.9/setup.py
```

### Comparing `fastgcf-1.0.8/.github/workflows/python-publish.yml` & `fastgcf-1.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fastgcf-1.0.8/.gitignore` & `fastgcf-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `fastgcf-1.0.8/LICENCE` & `fastgcf-1.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `fastgcf-1.0.8/PKG-INFO` & `fastgcf-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastgcf
-Version: 1.0.8
+Version: 1.0.9
 Summary: FastAPI in Google Cloud Functions
 Home-page: https://github.com/TigranZalian/fastgcf
 Author: Tigran Zalian
 Author-email: tigraanzalian@gmail.com
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE
-Requires-Dist: functions-framework==3.*
+Requires-Dist: functions-framework
 Requires-Dist: fastapi==0.110.0
 Requires-Dist: httpx==0.27.0
 Requires-Dist: nest_asyncio==1.5.8
 
 # fastgcf
 
 ## Unlock the full potential of Google Cloud Functions with FastAPI and async capabilities
```

### Comparing `fastgcf-1.0.8/README.md` & `fastgcf-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fastgcf-1.0.8/fastgcf/_converters.py` & `fastgcf-1.0.9/fastgcf/_converters.py`

 * *Files identical despite different names*

### Comparing `fastgcf-1.0.8/fastgcf/_handler.py` & `fastgcf-1.0.9/fastgcf/_handler.py`

 * *Files identical despite different names*

### Comparing `fastgcf-1.0.8/fastgcf/_proxy.py` & `fastgcf-1.0.9/fastgcf/_proxy.py`

 * *Files identical despite different names*

### Comparing `fastgcf-1.0.8/fastgcf/_router.py` & `fastgcf-1.0.9/fastgcf/_router.py`

 * *Files identical despite different names*

### Comparing `fastgcf-1.0.8/fastgcf/_streams.py` & `fastgcf-1.0.9/fastgcf/_streams.py`

 * *Files identical despite different names*

### Comparing `fastgcf-1.0.8/fastgcf/_transport.py` & `fastgcf-1.0.9/fastgcf/_transport.py`

 * *Files identical despite different names*

### Comparing `fastgcf-1.0.8/fastgcf.egg-info/PKG-INFO` & `fastgcf-1.0.9/fastgcf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastgcf
-Version: 1.0.8
+Version: 1.0.9
 Summary: FastAPI in Google Cloud Functions
 Home-page: https://github.com/TigranZalian/fastgcf
 Author: Tigran Zalian
 Author-email: tigraanzalian@gmail.com
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE
-Requires-Dist: functions-framework==3.*
+Requires-Dist: functions-framework
 Requires-Dist: fastapi==0.110.0
 Requires-Dist: httpx==0.27.0
 Requires-Dist: nest_asyncio==1.5.8
 
 # fastgcf
 
 ## Unlock the full potential of Google Cloud Functions with FastAPI and async capabilities
```

### Comparing `fastgcf-1.0.8/setup.py` & `fastgcf-1.0.9/setup.py`

 * *Files identical despite different names*

