# Comparing `tmp/shuttleai-3.8.2.tar.gz` & `tmp/shuttleai-3.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shuttleai-3.8.2.tar", last modified: Fri Apr  5 17:14:45 2024, max compression
+gzip compressed data, was "shuttleai-3.8.3.tar", last modified: Fri Apr  5 20:15:23 2024, max compression
```

## Comparing `shuttleai-3.8.2.tar` & `shuttleai-3.8.3.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 17:14:45.654879 shuttleai-3.8.2/
--rw-rw-rw-   0        0        0     4184 2024-04-05 17:14:45.653880 shuttleai-3.8.2/PKG-INFO
--rw-rw-rw-   0        0        0     3226 2024-04-03 08:41:19.000000 shuttleai-3.8.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-05 17:14:45.654879 shuttleai-3.8.2/setup.cfg
--rw-rw-rw-   0        0        0     1783 2024-04-05 17:11:32.000000 shuttleai-3.8.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 17:14:45.613884 shuttleai-3.8.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 17:14:45.618879 shuttleai-3.8.2/src/shuttleai/
--rw-rw-rw-   0        0        0      576 2024-04-05 17:13:49.000000 shuttleai-3.8.2/src/shuttleai/__init__.py
--rw-rw-rw-   0        0        0     4419 2024-04-03 08:54:56.000000 shuttleai-3.8.2/src/shuttleai/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-05 17:14:45.646881 shuttleai-3.8.2/src/shuttleai/client/
--rw-rw-rw-   0        0        0       72 2024-04-03 19:49:40.000000 shuttleai-3.8.2/src/shuttleai/client/__init__.py
--rw-rw-rw-   0        0        0    17420 2024-04-05 17:14:00.000000 shuttleai-3.8.2/src/shuttleai/client/_async.py
--rw-rw-rw-   0        0        0     3331 2024-04-05 17:14:05.000000 shuttleai-3.8.2/src/shuttleai/client/_sync.py
--rw-rw-rw-   0        0        0    10161 2024-04-05 17:14:08.000000 shuttleai-3.8.2/src/shuttleai/client/_syncr.py
--rw-rw-rw-   0        0        0     1636 2024-04-01 03:32:40.000000 shuttleai-3.8.2/src/shuttleai/log.py
-drwxrwxrwx   0        0        0        0 2024-04-05 17:14:45.649879 shuttleai-3.8.2/src/shuttleai/schemas/
--rw-rw-rw-   0        0        0      230 2024-04-03 02:14:24.000000 shuttleai-3.8.2/src/shuttleai/schemas/__init__.py
--rw-rw-rw-   0        0        0     2030 2024-04-03 02:15:03.000000 shuttleai-3.8.2/src/shuttleai/schemas/schemas.py
-drwxrwxrwx   0        0        0        0 2024-04-05 17:14:45.651879 shuttleai-3.8.2/src/shuttleai.egg-info/
--rw-rw-rw-   0        0        0     4184 2024-04-05 17:14:45.000000 shuttleai-3.8.2/src/shuttleai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2024-04-05 17:14:45.000000 shuttleai-3.8.2/src/shuttleai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 17:14:45.000000 shuttleai-3.8.2/src/shuttleai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-05 17:14:45.000000 shuttleai-3.8.2/src/shuttleai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       67 2024-04-05 17:14:45.000000 shuttleai-3.8.2/src/shuttleai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-05 17:14:45.000000 shuttleai-3.8.2/src/shuttleai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 20:15:23.827007 shuttleai-3.8.3/
+-rw-rw-rw-   0        0        0     4184 2024-04-05 20:15:23.825009 shuttleai-3.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3226 2024-04-03 08:41:19.000000 shuttleai-3.8.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-05 20:15:23.827007 shuttleai-3.8.3/setup.cfg
+-rw-rw-rw-   0        0        0     1783 2024-04-05 17:17:27.000000 shuttleai-3.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:15:23.751008 shuttleai-3.8.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 20:15:23.761009 shuttleai-3.8.3/src/shuttleai/
+-rw-rw-rw-   0        0        0      576 2024-04-05 20:15:18.000000 shuttleai-3.8.3/src/shuttleai/__init__.py
+-rw-rw-rw-   0        0        0     4419 2024-04-03 08:54:56.000000 shuttleai-3.8.3/src/shuttleai/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:15:23.817010 shuttleai-3.8.3/src/shuttleai/client/
+-rw-rw-rw-   0        0        0       72 2024-04-03 19:49:40.000000 shuttleai-3.8.3/src/shuttleai/client/__init__.py
+-rw-rw-rw-   0        0        0    17420 2024-04-05 20:15:15.000000 shuttleai-3.8.3/src/shuttleai/client/_async.py
+-rw-rw-rw-   0        0        0    15283 2024-04-05 20:15:16.000000 shuttleai-3.8.3/src/shuttleai/client/_sync.py
+-rw-rw-rw-   0        0        0     1636 2024-04-01 03:32:40.000000 shuttleai-3.8.3/src/shuttleai/log.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:15:23.820008 shuttleai-3.8.3/src/shuttleai/schemas/
+-rw-rw-rw-   0        0        0      230 2024-04-03 02:14:24.000000 shuttleai-3.8.3/src/shuttleai/schemas/__init__.py
+-rw-rw-rw-   0        0        0     2030 2024-04-03 02:15:03.000000 shuttleai-3.8.3/src/shuttleai/schemas/schemas.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:15:23.823008 shuttleai-3.8.3/src/shuttleai.egg-info/
+-rw-rw-rw-   0        0        0     4184 2024-04-05 20:15:23.000000 shuttleai-3.8.3/src/shuttleai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2024-04-05 20:15:23.000000 shuttleai-3.8.3/src/shuttleai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 20:15:23.000000 shuttleai-3.8.3/src/shuttleai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-05 20:15:23.000000 shuttleai-3.8.3/src/shuttleai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       67 2024-04-05 20:15:23.000000 shuttleai-3.8.3/src/shuttleai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-05 20:15:23.000000 shuttleai-3.8.3/src/shuttleai.egg-info/top_level.txt
```

### Comparing `shuttleai-3.8.2/PKG-INFO` & `shuttleai-3.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shuttleai
-Version: 3.8.2
+Version: 3.8.3
 Summary: Access Shuttle AI's API via a simple and user-friendly lib. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai
 Home-page: https://github.com/shuttleai/shuttleai-python
 Author: shuttle
 Author-email: noreply@shuttleai.app
 Keywords: shuttleai,ai,gpt,claude,api,free,chatgpt,gpt-4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shuttleai-3.8.2/README.md` & `shuttleai-3.8.3/README.md`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.2/setup.py` & `shuttleai-3.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.2/src/shuttleai/__init__.py` & `shuttleai-3.8.3/src/shuttleai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .client import ShuttleAsyncClient, ShuttleClient
 
 from sys import executable
 from os import system
 from httpx import get
 
-__version__ = "3.8.2"
+__version__ = "3.8.3"
 
 try:
     CURRENT_VERSION = get(
         "https://pypi.org/pypi/shuttleai/json").json().get("info").get("version")
 except:
     CURRENT_VERSION = __version__
```

### Comparing `shuttleai-3.8.2/src/shuttleai/cli.py` & `shuttleai-3.8.3/src/shuttleai/cli.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.2/src/shuttleai/client/_async.py` & `shuttleai-3.8.3/src/shuttleai/client/_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 @Author: ShuttleAI
-@Version: 3.8.2
+@Version: 3.8.3
 @Date: 4-5-2024
 """
 from __future__ import annotations
 from typing import (
     List,
     Dict,
     Any,
```

### Comparing `shuttleai-3.8.2/src/shuttleai/log.py` & `shuttleai-3.8.3/src/shuttleai/log.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.2/src/shuttleai/schemas/schemas.py` & `shuttleai-3.8.3/src/shuttleai/schemas/schemas.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.2/src/shuttleai.egg-info/PKG-INFO` & `shuttleai-3.8.3/src/shuttleai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shuttleai
-Version: 3.8.2
+Version: 3.8.3
 Summary: Access Shuttle AI's API via a simple and user-friendly lib. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai
 Home-page: https://github.com/shuttleai/shuttleai-python
 Author: shuttle
 Author-email: noreply@shuttleai.app
 Keywords: shuttleai,ai,gpt,claude,api,free,chatgpt,gpt-4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

