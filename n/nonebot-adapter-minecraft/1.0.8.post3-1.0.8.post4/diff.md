# Comparing `tmp/nonebot_adapter_minecraft-1.0.8.post3.tar.gz` & `tmp/nonebot_adapter_minecraft-1.0.8.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_minecraft-1.0.8.post3.tar", max compression
+gzip compressed data, was "nonebot_adapter_minecraft-1.0.8.post4.tar", max compression
```

## Comparing `nonebot_adapter_minecraft-1.0.8.post3.tar` & `nonebot_adapter_minecraft-1.0.8.post4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1065 2024-03-10 06:43:07.623363 nonebot_adapter_minecraft-1.0.8.post3/LICENSE
--rw-r--r--   0        0        0     1693 2024-03-10 06:43:07.623363 nonebot_adapter_minecraft-1.0.8.post3/README.md
--rw-r--r--   0        0        0      375 2024-03-10 06:43:07.623363 nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/__init__.py
--rw-r--r--   0        0        0     8535 2024-03-10 06:43:07.623363 nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/adapter.py
--rw-r--r--   0        0        0     2317 2024-03-10 06:43:07.623363 nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/bot.py
--rw-r--r--   0        0        0     1104 2024-03-10 06:43:07.623363 nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/bot.pyi
--rw-r--r--   0        0        0     3794 2024-03-10 06:43:07.623363 nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/collator.py
--rw-r--r--   0        0        0      527 2024-03-10 06:43:07.623363 nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/compat.py
--rw-r--r--   0        0        0      285 2024-03-10 06:43:07.623363 nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/config.py
--rw-r--r--   0        0        0     1179 2024-03-10 06:43:07.623363 nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/event/__init__.py
--rw-r--r--   0        0        0     3533 2024-03-10 06:43:07.623363 nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/event/base.py
--rw-r--r--   0        0        0     1703 2024-03-10 06:43:07.623363 nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/event/fabric.py
--rw-r--r--   0        0        0      949 2024-03-10 06:43:07.623363 nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/event/forge.py
--rw-r--r--   0        0        0      648 2024-03-10 06:43:07.623363 nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/event/minecraft.py
--rw-r--r--   0        0        0     1775 2024-03-10 06:43:07.623363 nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/event/spigot.py
--rw-r--r--   0        0        0     1250 2024-03-10 06:43:07.623363 nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/exception.py
--rw-r--r--   0        0        0     4844 2024-03-10 06:43:07.623363 nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/message.py
--rw-r--r--   0        0        0     5449 2024-03-10 06:43:07.623363 nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/model.py
--rw-r--r--   0        0        0     1008 2024-03-10 06:43:07.623363 nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/utils.py
--rw-r--r--   0        0        0      660 2024-03-10 06:43:07.623363 nonebot_adapter_minecraft-1.0.8.post3/pyproject.toml
--rw-r--r--   0        0        0     2396 1970-01-01 00:00:00.000000 nonebot_adapter_minecraft-1.0.8.post3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-05 07:10:05.237191 nonebot_adapter_minecraft-1.0.8.post4/LICENSE
+-rw-r--r--   0        0        0     1693 2024-04-05 07:10:05.237191 nonebot_adapter_minecraft-1.0.8.post4/README.md
+-rw-r--r--   0        0        0      375 2024-04-05 07:10:05.237191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/__init__.py
+-rw-r--r--   0        0        0     8535 2024-04-05 07:10:05.237191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/adapter.py
+-rw-r--r--   0        0        0     2317 2024-04-05 07:10:05.237191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/bot.py
+-rw-r--r--   0        0        0     1104 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/bot.pyi
+-rw-r--r--   0        0        0     3794 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/collator.py
+-rw-r--r--   0        0        0      527 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/compat.py
+-rw-r--r--   0        0        0      285 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/config.py
+-rw-r--r--   0        0        0     1179 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/event/__init__.py
+-rw-r--r--   0        0        0     3533 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/event/base.py
+-rw-r--r--   0        0        0     1703 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/event/fabric.py
+-rw-r--r--   0        0        0      949 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/event/forge.py
+-rw-r--r--   0        0        0      648 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/event/minecraft.py
+-rw-r--r--   0        0        0     1775 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/event/spigot.py
+-rw-r--r--   0        0        0     1250 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/exception.py
+-rw-r--r--   0        0        0     4844 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/message.py
+-rw-r--r--   0        0        0     5449 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/model.py
+-rw-r--r--   0        0        0     1008 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/utils.py
+-rw-r--r--   0        0        0      642 2024-04-05 07:10:05.241191 nonebot_adapter_minecraft-1.0.8.post4/pyproject.toml
+-rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 nonebot_adapter_minecraft-1.0.8.post4/PKG-INFO
```

### Comparing `nonebot_adapter_minecraft-1.0.8.post3/LICENSE` & `nonebot_adapter_minecraft-1.0.8.post4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post3/README.md` & `nonebot_adapter_minecraft-1.0.8.post4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/adapter.py` & `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/bot.py` & `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/bot.pyi` & `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/bot.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/collator.py` & `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/collator.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/compat.py` & `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/compat.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/event/__init__.py` & `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/event/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/event/base.py` & `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/event/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/event/fabric.py` & `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/event/fabric.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/event/forge.py` & `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/event/forge.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/event/minecraft.py` & `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/event/minecraft.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/event/spigot.py` & `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/event/spigot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/exception.py` & `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/message.py` & `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/model.py` & `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post3/nonebot/adapters/minecraft/utils.py` & `nonebot_adapter_minecraft-1.0.8.post4/nonebot/adapters/minecraft/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.0.8.post3/pyproject.toml` & `nonebot_adapter_minecraft-1.0.8.post4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [tool.poetry]
 name = "nonebot-adapter-minecraft"
-version = "1.0.8.post3"
+version = "1.0.8.post4"
 description = "NoneBot2与MineCraft Server互通的适配器。"
 authors = ["17TheWord <17theword@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "nonebot" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-nb-cli = "^1.4.0"
 aio-mc-rcon = "^3.2.2"
 nonebot2 = { version = "^2.2.0", extras = ["fastapi"] }
 
 
 [tool.poetry.group.test.dependencies]
 anyio = "~=3.6"
 nonebug = "^0.3.5"
```

### Comparing `nonebot_adapter_minecraft-1.0.8.post3/PKG-INFO` & `nonebot_adapter_minecraft-1.0.8.post4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-minecraft
-Version: 1.0.8.post3
+Version: 1.0.8.post4
 Summary: NoneBot2与MineCraft Server互通的适配器。
 License: MIT
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aio-mc-rcon (>=3.2.2,<4.0.0)
-Requires-Dist: nb-cli (>=1.4.0,<2.0.0)
 Requires-Dist: nonebot2[fastapi] (>=2.2.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/17TheWord/nonebot-adapter-minecraft/main/assets/logo.png" width="200" height="200" alt="nonebot-adapter-minecraft">
 </p>
```

