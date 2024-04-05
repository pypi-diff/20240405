# Comparing `tmp/nonebot_plugin_diffsinger-0.1.8.tar.gz` & `tmp/nonebot_plugin_diffsinger-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_diffsinger-0.1.8.tar", last modified: Wed Apr  3 14:54:15 2024, max compression
+gzip compressed data, was "nonebot_plugin_diffsinger-0.1.9.tar", last modified: Thu Apr  4 15:50:51 2024, max compression
```

## Comparing `nonebot_plugin_diffsinger-0.1.8.tar` & `nonebot_plugin_diffsinger-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:54:15.541440 nonebot_plugin_diffsinger-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-03 14:54:11.000000 nonebot_plugin_diffsinger-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 14:54:11.000000 nonebot_plugin_diffsinger-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-03 14:54:15.541440 nonebot_plugin_diffsinger-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-03 14:54:11.000000 nonebot_plugin_diffsinger-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:54:15.541440 nonebot_plugin_diffsinger-0.1.8/nonebot_plugin_diffsinger/
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-03 14:54:11.000000 nonebot_plugin_diffsinger-0.1.8/nonebot_plugin_diffsinger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-03 14:54:11.000000 nonebot_plugin_diffsinger-0.1.8/nonebot_plugin_diffsinger/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-03 14:54:11.000000 nonebot_plugin_diffsinger-0.1.8/nonebot_plugin_diffsinger/data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:54:15.541440 nonebot_plugin_diffsinger-0.1.8/nonebot_plugin_diffsinger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-03 14:54:15.000000 nonebot_plugin_diffsinger-0.1.8/nonebot_plugin_diffsinger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-03 14:54:15.000000 nonebot_plugin_diffsinger-0.1.8/nonebot_plugin_diffsinger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:54:15.000000 nonebot_plugin_diffsinger-0.1.8/nonebot_plugin_diffsinger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-03 14:54:15.000000 nonebot_plugin_diffsinger-0.1.8/nonebot_plugin_diffsinger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-03 14:54:15.000000 nonebot_plugin_diffsinger-0.1.8/nonebot_plugin_diffsinger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:54:15.541440 nonebot_plugin_diffsinger-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-03 14:54:11.000000 nonebot_plugin_diffsinger-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:50:51.640489 nonebot_plugin_diffsinger-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-04 15:50:46.000000 nonebot_plugin_diffsinger-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-04 15:50:46.000000 nonebot_plugin_diffsinger-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-04 15:50:51.640489 nonebot_plugin_diffsinger-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-04 15:50:46.000000 nonebot_plugin_diffsinger-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:50:51.640489 nonebot_plugin_diffsinger-0.1.9/nonebot_plugin_diffsinger/
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-04 15:50:46.000000 nonebot_plugin_diffsinger-0.1.9/nonebot_plugin_diffsinger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-04 15:50:46.000000 nonebot_plugin_diffsinger-0.1.9/nonebot_plugin_diffsinger/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-04 15:50:46.000000 nonebot_plugin_diffsinger-0.1.9/nonebot_plugin_diffsinger/data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:50:51.640489 nonebot_plugin_diffsinger-0.1.9/nonebot_plugin_diffsinger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-04 15:50:51.000000 nonebot_plugin_diffsinger-0.1.9/nonebot_plugin_diffsinger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-04 15:50:51.000000 nonebot_plugin_diffsinger-0.1.9/nonebot_plugin_diffsinger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:50:51.000000 nonebot_plugin_diffsinger-0.1.9/nonebot_plugin_diffsinger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-04 15:50:51.000000 nonebot_plugin_diffsinger-0.1.9/nonebot_plugin_diffsinger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-04 15:50:51.000000 nonebot_plugin_diffsinger-0.1.9/nonebot_plugin_diffsinger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 15:50:51.640489 nonebot_plugin_diffsinger-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-04 15:50:46.000000 nonebot_plugin_diffsinger-0.1.9/setup.py
```

### Comparing `nonebot_plugin_diffsinger-0.1.8/LICENSE` & `nonebot_plugin_diffsinger-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_diffsinger-0.1.8/PKG-INFO` & `nonebot_plugin_diffsinger-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_diffsinger
-Version: 0.1.8
+Version: 0.1.9
 Summary: 用DiffSinger让bot唱歌
 Home-page: https://github.com/zhzhongshi/nonebot-plugin-diffsinger
 Author: zhzhongshi
 Author-email: zhzhongshi@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: nonebot2
+Requires-Dist: nonebot2<3.0.0,>=2.2.0
 Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: httpx
 Requires-Dist: librosa
 
 
 这个需要配合这个项目使用（[DiffSingerMiniEngine](https://github.com/zhzhongshi/DiffSingerMiniEngine)
 
@@ -46,14 +46,20 @@
 
 你要是打算用pip安装的话
 ```
 pip install nonebot-plugin-diffsinger
 ```
 别忘了把"nonebot-plugin-diffsinger"加到pyproject.toml里面的"plugins"里面
 
+配置
+```
+DS_URL="http://127.0.0.1:9266/" #后端的地址
+DS_SPEEDUP=200 #后端的推理速度，建议10-255
+```
+
 测试指令
 
 
 ```
 /diffsinger 120~[
 [60,2,"AP"],
 [57,2,"ba"],
```

### Comparing `nonebot_plugin_diffsinger-0.1.8/README.md` & `nonebot_plugin_diffsinger-0.1.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,20 @@
 
 你要是打算用pip安装的话
 ```
 pip install nonebot-plugin-diffsinger
 ```
 别忘了把"nonebot-plugin-diffsinger"加到pyproject.toml里面的"plugins"里面
 
+配置
+```
+DS_URL="http://127.0.0.1:9266/" #后端的地址
+DS_SPEEDUP=200 #后端的推理速度，建议10-255
+```
+
 测试指令
 
 
 ```
 /diffsinger 120~[
 [60,2,"AP"],
 [57,2,"ba"],
```

### Comparing `nonebot_plugin_diffsinger-0.1.8/nonebot_plugin_diffsinger/__init__.py` & `nonebot_plugin_diffsinger-0.1.9/nonebot_plugin_diffsinger/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 [59,4,"shou"],
 [55,16,"zhang"],
 [60,4,"AP"]
 ]
 
 """,
     type="application",
+    config=Config,
     homepage="https://github.com/zhzhongshi/nonebot-plugin-diffsinger",
     supported_adapters={"~onebot.v11"}
 )
 
 ds = on_command("diffsinger", priority=7)
 plugin_config = get_plugin_config(Config)
 url=plugin_config.ds_url
```

### Comparing `nonebot_plugin_diffsinger-0.1.8/nonebot_plugin_diffsinger/data_source.py` & `nonebot_plugin_diffsinger-0.1.9/nonebot_plugin_diffsinger/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_diffsinger-0.1.8/nonebot_plugin_diffsinger.egg-info/PKG-INFO` & `nonebot_plugin_diffsinger-0.1.9/nonebot_plugin_diffsinger.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_diffsinger
-Version: 0.1.8
+Version: 0.1.9
 Summary: 用DiffSinger让bot唱歌
 Home-page: https://github.com/zhzhongshi/nonebot-plugin-diffsinger
 Author: zhzhongshi
 Author-email: zhzhongshi@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: nonebot2
+Requires-Dist: nonebot2<3.0.0,>=2.2.0
 Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: httpx
 Requires-Dist: librosa
 
 
 这个需要配合这个项目使用（[DiffSingerMiniEngine](https://github.com/zhzhongshi/DiffSingerMiniEngine)
 
@@ -46,14 +46,20 @@
 
 你要是打算用pip安装的话
 ```
 pip install nonebot-plugin-diffsinger
 ```
 别忘了把"nonebot-plugin-diffsinger"加到pyproject.toml里面的"plugins"里面
 
+配置
+```
+DS_URL="http://127.0.0.1:9266/" #后端的地址
+DS_SPEEDUP=200 #后端的推理速度，建议10-255
+```
+
 测试指令
 
 
 ```
 /diffsinger 120~[
 [60,2,"AP"],
 [57,2,"ba"],
```

### Comparing `nonebot_plugin_diffsinger-0.1.8/setup.py` & `nonebot_plugin_diffsinger-0.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,33 @@
 import io
 import os
 import sys
 from shutil import rmtree
 
 from setuptools import find_packages, setup, Command
 
+#todo pyproject.toml for poetry
+
 # Package meta-data.
 NAME = 'nonebot_plugin_diffsinger'
 DESCRIPTION = '用DiffSinger让bot唱歌'
 URL = 'https://github.com/zhzhongshi/nonebot-plugin-diffsinger'
 EMAIL = 'zhzhongshi@qq.com'
 AUTHOR = 'zhzhongshi'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 REQUIRED = [
-    "nonebot2","nonebot-adapter-onebot","httpx","librosa"
+    "nonebot2>=2.2.0,<3.0.0",
+    "nonebot-adapter-onebot",
+    "httpx",
+    "librosa"
 ]
 # What packages are optional?
 EXTRAS = {
+    
 }
 
 # The rest you shouldn't have to touch too much :)
 # ------------------------------------------------
 # Except, perhaps the License and Trove Classifiers!
 # If you do change the License, remember to change the Trove Classifier for that!
```

