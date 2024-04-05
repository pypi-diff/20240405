# Comparing `tmp/sciveo-0.0.8.tar.gz` & `tmp/sciveo-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciveo-0.0.8.tar", last modified: Sat Nov 18 15:31:57 2023, max compression
+gzip compressed data, was "sciveo-0.0.9.tar", last modified: Sat Nov 18 18:35:37 2023, max compression
```

## Comparing `sciveo-0.0.8.tar` & `sciveo-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2023-11-18 15:31:57.028540 sciveo-0.0.8/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       50 2023-11-18 15:31:57.028404 sciveo-0.0.8/PKG-INFO
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      809 2023-11-15 13:39:07.000000 sciveo-0.0.8/README.md
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2023-11-18 15:31:57.008917 sciveo-0.0.8/sciveo/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      847 2023-11-15 15:33:57.000000 sciveo-0.0.8/sciveo/__init__.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2023-11-18 15:31:57.015517 sciveo-0.0.8/sciveo/api/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:04:12.000000 sciveo-0.0.8/sciveo/api/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1246 2023-11-18 15:17:13.000000 sciveo-0.0.8/sciveo/api/base.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1187 2023-11-15 15:20:35.000000 sciveo-0.0.8/sciveo/api/content.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2023-11-18 15:31:57.017480 sciveo-0.0.8/sciveo/common/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:03:59.000000 sciveo-0.0.8/sciveo/common/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1977 2023-11-18 15:15:32.000000 sciveo-0.0.8/sciveo/common/configuration.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2056 2023-11-18 13:09:32.000000 sciveo-0.0.8/sciveo/common/sampling.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2023-11-18 15:31:57.021701 sciveo-0.0.8/sciveo/common/tools/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:07:07.000000 sciveo-0.0.8/sciveo/common/tools/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1053 2023-11-17 12:42:35.000000 sciveo-0.0.8/sciveo/common/tools/formating.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      920 2023-11-17 12:49:55.000000 sciveo-0.0.8/sciveo/common/tools/hardware.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1071 2023-11-15 15:21:05.000000 sciveo-0.0.8/sciveo/common/tools/logger.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2023-11-18 15:31:57.027210 sciveo-0.0.8/sciveo/content/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:14:23.000000 sciveo-0.0.8/sciveo/content/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     4134 2023-11-18 15:15:52.000000 sciveo-0.0.8/sciveo/content/experiment.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2423 2023-11-17 15:04:23.000000 sciveo-0.0.8/sciveo/content/project.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1309 2023-11-18 14:55:43.000000 sciveo-0.0.8/sciveo/content/runner.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2023-11-18 15:31:57.013563 sciveo-0.0.8/sciveo.egg-info/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       50 2023-11-18 15:31:56.000000 sciveo-0.0.8/sciveo.egg-info/PKG-INFO
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      616 2023-11-18 15:31:56.000000 sciveo-0.0.8/sciveo.egg-info/SOURCES.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        1 2023-11-18 15:31:56.000000 sciveo-0.0.8/sciveo.egg-info/dependency_links.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       43 2023-11-18 15:31:56.000000 sciveo-0.0.8/sciveo.egg-info/requires.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        7 2023-11-18 15:31:56.000000 sciveo-0.0.8/sciveo.egg-info/top_level.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       38 2023-11-18 15:31:57.028591 sciveo-0.0.8/setup.cfg
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      223 2023-11-18 15:13:32.000000 sciveo-0.0.8/setup.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2023-11-18 15:31:57.027993 sciveo-0.0.8/test/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      521 2023-11-18 13:23:37.000000 sciveo-0.0.8/test/test_configuration.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1813 2023-11-18 14:17:32.000000 sciveo-0.0.8/test/test_sampling.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2023-11-18 18:35:37.392445 sciveo-0.0.9/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       50 2023-11-18 18:35:37.392304 sciveo-0.0.9/PKG-INFO
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      809 2023-11-15 13:39:07.000000 sciveo-0.0.9/README.md
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2023-11-18 18:35:37.380878 sciveo-0.0.9/sciveo/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      847 2023-11-15 15:33:57.000000 sciveo-0.0.9/sciveo/__init__.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2023-11-18 18:35:37.385612 sciveo-0.0.9/sciveo/api/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:04:12.000000 sciveo-0.0.9/sciveo/api/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1246 2023-11-18 15:17:13.000000 sciveo-0.0.9/sciveo/api/base.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2023-11-18 18:35:37.387311 sciveo-0.0.9/sciveo/common/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:03:59.000000 sciveo-0.0.9/sciveo/common/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1977 2023-11-18 15:15:32.000000 sciveo-0.0.9/sciveo/common/configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1303 2023-11-18 18:30:56.000000 sciveo-0.0.9/sciveo/common/model.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2056 2023-11-18 13:09:32.000000 sciveo-0.0.9/sciveo/common/sampling.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2023-11-18 18:35:37.389061 sciveo-0.0.9/sciveo/common/tools/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:07:07.000000 sciveo-0.0.9/sciveo/common/tools/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1053 2023-11-17 12:42:35.000000 sciveo-0.0.9/sciveo/common/tools/formating.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1058 2023-11-18 15:34:18.000000 sciveo-0.0.9/sciveo/common/tools/hardware.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1071 2023-11-15 15:21:05.000000 sciveo-0.0.9/sciveo/common/tools/logger.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2023-11-18 18:35:37.391017 sciveo-0.0.9/sciveo/content/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:14:23.000000 sciveo-0.0.9/sciveo/content/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     4156 2023-11-18 18:31:10.000000 sciveo-0.0.9/sciveo/content/experiment.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2384 2023-11-18 17:43:34.000000 sciveo-0.0.9/sciveo/content/project.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1309 2023-11-18 14:55:43.000000 sciveo-0.0.9/sciveo/content/runner.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2023-11-18 18:35:37.385198 sciveo-0.0.9/sciveo.egg-info/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       50 2023-11-18 18:35:37.000000 sciveo-0.0.9/sciveo.egg-info/PKG-INFO
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      617 2023-11-18 18:35:37.000000 sciveo-0.0.9/sciveo.egg-info/SOURCES.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        1 2023-11-18 18:35:37.000000 sciveo-0.0.9/sciveo.egg-info/dependency_links.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       43 2023-11-18 18:35:37.000000 sciveo-0.0.9/sciveo.egg-info/requires.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        7 2023-11-18 18:35:37.000000 sciveo-0.0.9/sciveo.egg-info/top_level.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       38 2023-11-18 18:35:37.392523 sciveo-0.0.9/setup.cfg
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      223 2023-11-18 18:35:35.000000 sciveo-0.0.9/setup.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2023-11-18 18:35:37.391958 sciveo-0.0.9/test/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      521 2023-11-18 13:23:37.000000 sciveo-0.0.9/test/test_configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1813 2023-11-18 14:17:32.000000 sciveo-0.0.9/test/test_sampling.py
```

### Comparing `sciveo-0.0.8/README.md` & `sciveo-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.8/sciveo/__init__.py` & `sciveo-0.0.9/sciveo/__init__.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.8/sciveo/api/base.py` & `sciveo-0.0.9/sciveo/api/base.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.8/sciveo/common/configuration.py` & `sciveo-0.0.9/sciveo/common/configuration.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.8/sciveo/common/sampling.py` & `sciveo-0.0.9/sciveo/common/sampling.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.8/sciveo/common/tools/formating.py` & `sciveo-0.0.9/sciveo/common/tools/formating.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.8/sciveo/common/tools/hardware.py` & `sciveo-0.0.9/sciveo/common/tools/hardware.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,20 +22,22 @@
 
     self.get_cpuinfo()
 
   def __call__(self):
     return self.data
 
   def get_cpuinfo(self):
+    list_keys = ["model name", "stepping", "cpu MHz", "cache size", "siblings", "cpu cores", "bogomips"]
     try:
       cpu_info = {}
       with open('/proc/cpuinfo', 'r') as file:
         lines = file.readlines()
 
       for line in lines:
         if ':' in line:
           key, value = map(str.strip, line.split(':', 1))
-          cpu_info[key] = value
+          if key in list_keys:
+            cpu_info[key] = value
 
       self.data["CPU"]["info"] = cpu_info
     except Exception:
       return
```

### Comparing `sciveo-0.0.8/sciveo/common/tools/logger.py` & `sciveo-0.0.9/sciveo/common/tools/logger.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.8/sciveo/content/experiment.py` & `sciveo-0.0.9/sciveo/content/experiment.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 import datetime
 
 import numpy as np
 import pandas as pd
 
 from sciveo.common.tools.logger import *
 from sciveo.api.base import APIRemoteClient
-from sciveo.api.content import Content
 from sciveo.common.tools.formating import format_elapsed_time
 from sciveo.common.tools.hardware import HardwareInfo
 from sciveo.common.configuration import Configuration
+from sciveo.common.model import ModelInfo
 
 
 class Experiment:
   def __init__(self, project_name, project_guid, config):
     self.project_name = project_name
     self.project_guid = project_guid
     self.config = config
@@ -84,34 +84,37 @@
     }
     result = self.api.POST("experiment", remote_data)
     debug(type(self).__name__, "close", self.name, "api", result)
 
   def append(self, d):
     self.data["experiment"]["log"].append(d)
 
-  def eval(self, key, value):
+  def eval(self, key, value, **kwargs):
     self.data["experiment"]["eval"][key] = value
+    for k, v in kwargs.items():
+      self.data["experiment"]["eval"][k] = v
   # Score value (no matter of its true meaning) which is used for experiments sorting
   def score(self, value):
     self.eval("score", value)
 
+  def model(self, m):
+    self.data["experiment"]["model"] = ModelInfo(m).any()
+  def model_keras(self, m):
+    self.data["experiment"]["model"] = ModelInfo(m).keras()
+  def model_torch(self, m):
+    self.data["experiment"]["model"] = ModelInfo(m).torch()
+
   def log(self, data, val=None, *args, **kwargs):
-    if isinstance(data, Content):
-      self.log_content(data)
-    elif isinstance(data, dict):
+    if isinstance(data, dict):
       self.log_dict(data)
     else:
       self.log_any(data, val, *args, **kwargs)
-  def log_content(self, content):
-    debug(type(self).__name__, self.project_name, "LOG content", content)
   def log_dict(self, data):
-    debug(type(self).__name__, self.project_name, "LOG data", data)
     self.append(data)
   def log_any(self, data, val=None, *args, **kwargs):
-    debug(type(self).__name__, self.project_name, "LOG", (data, val), args, kwargs)
     if val is None:
       self.append(data)
     else:
       self.append({data: val})
     for a in args:
       self.append(a)
     for k, v in kwargs.items():
```

### Comparing `sciveo-0.0.8/sciveo/content/project.py` & `sciveo-0.0.9/sciveo/content/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import time
 
 import numpy as np
 import pandas as pd
 
 from sciveo.common.tools.logger import *
 from sciveo.api.base import *
-from sciveo.api.content import Content
 from sciveo.common.configuration import Configuration
 from sciveo.content.experiment import Experiment
 
 
 class ProjectBase:
   def __init__(self, project_name):
     self.project_name = project_name
```

### Comparing `sciveo-0.0.8/sciveo/content/runner.py` & `sciveo-0.0.9/sciveo/content/runner.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.8/sciveo.egg-info/SOURCES.txt` & `sciveo-0.0.9/sciveo.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 sciveo.egg-info/PKG-INFO
 sciveo.egg-info/SOURCES.txt
 sciveo.egg-info/dependency_links.txt
 sciveo.egg-info/requires.txt
 sciveo.egg-info/top_level.txt
 sciveo/api/__init__.py
 sciveo/api/base.py
-sciveo/api/content.py
 sciveo/common/__init__.py
 sciveo/common/configuration.py
+sciveo/common/model.py
 sciveo/common/sampling.py
 sciveo/common/tools/__init__.py
 sciveo/common/tools/formating.py
 sciveo/common/tools/hardware.py
 sciveo/common/tools/logger.py
 sciveo/content/__init__.py
 sciveo/content/experiment.py
```

### Comparing `sciveo-0.0.8/test/test_configuration.py` & `sciveo-0.0.9/test/test_configuration.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.8/test/test_sampling.py` & `sciveo-0.0.9/test/test_sampling.py`

 * *Files identical despite different names*

