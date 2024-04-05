# Comparing `tmp/justai-3.2.6.tar.gz` & `tmp/justai-3.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "justai-3.2.6.tar", last modified: Tue Apr  2 09:52:41 2024, max compression
+gzip compressed data, was "justai-3.2.7.tar", last modified: Thu Apr  4 16:26:04 2024, max compression
```

## Comparing `justai-3.2.6.tar` & `justai-3.2.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-02 09:52:41.527233 justai-3.2.6/
--rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 justai-3.2.6/LICENSE
--rw-r--r--   0 hp         (501) staff       (20)      198 2024-02-20 10:20:38.000000 justai-3.2.6/MANIFEST.in
--rw-r--r--   0 hp         (501) staff       (20)     6408 2024-04-02 09:52:41.527005 justai-3.2.6/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)     4082 2024-04-02 09:52:39.000000 justai-3.2.6/README.md
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-02 09:52:41.520849 justai-3.2.6/justai/
--rw-r--r--   0 hp         (501) staff       (20)      579 2024-04-01 20:26:06.000000 justai-3.2.6/justai/__init__.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-02 09:52:41.521982 justai-3.2.6/justai/agent/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:05:20.000000 justai-3.2.6/justai/agent/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     5992 2024-03-31 21:07:33.000000 justai-3.2.6/justai/agent/agent.py
--rw-r--r--   0 hp         (501) staff       (20)      997 2024-03-05 16:49:21.000000 justai-3.2.6/justai/agent/message.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-02 09:52:41.522827 justai-3.2.6/justai/interactive/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:06:50.000000 justai-3.2.6/justai/interactive/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     5452 2024-02-07 19:49:01.000000 justai-3.2.6/justai/interactive/commands.py
--rw-r--r--   0 hp         (501) staff       (20)     1320 2024-03-05 16:26:44.000000 justai-3.2.6/justai/interactive/repl.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-02 09:52:41.524131 justai-3.2.6/justai/models/
--rw-r--r--   0 hp         (501) staff       (20)     2675 2024-04-02 08:20:07.000000 justai-3.2.6/justai/models/anthropic_models.py
--rw-r--r--   0 hp         (501) staff       (20)     2334 2024-03-21 09:14:50.000000 justai-3.2.6/justai/models/gguf_models.py
--rw-r--r--   0 hp         (501) staff       (20)      871 2024-03-21 08:22:51.000000 justai-3.2.6/justai/models/model.py
--rw-r--r--   0 hp         (501) staff       (20)      709 2024-03-06 13:20:05.000000 justai-3.2.6/justai/models/modelfactory.py
--rw-r--r--   0 hp         (501) staff       (20)     5807 2024-03-21 09:14:50.000000 justai-3.2.6/justai/models/openai_models.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-02 09:52:41.525083 justai-3.2.6/justai/tools/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:08:21.000000 justai-3.2.6/justai/tools/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     3815 2024-04-02 09:00:24.000000 justai-3.2.6/justai/tools/cache.py
--rw-r--r--   0 hp         (501) staff       (20)      563 2023-08-26 19:32:55.000000 justai-3.2.6/justai/tools/display.py
--rw-r--r--   0 hp         (501) staff       (20)     3226 2024-04-02 08:38:55.000000 justai-3.2.6/justai/tools/log.py
--rw-r--r--   0 hp         (501) staff       (20)      615 2024-02-09 15:06:31.000000 justai-3.2.6/justai/tools/prompts.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-02 09:52:41.526065 justai-3.2.6/justai/translator/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:11:10.000000 justai-3.2.6/justai/translator/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     4052 2024-02-13 10:39:31.000000 justai-3.2.6/justai/translator/languages.py
--rw-r--r--   0 hp         (501) staff       (20)     1551 2024-03-30 11:43:22.000000 justai-3.2.6/justai/translator/prompts.toml
--rw-r--r--   0 hp         (501) staff       (20)    14079 2024-04-01 09:02:59.000000 justai-3.2.6/justai/translator/translator.py
--rw-r--r--   0 hp         (501) staff       (20)     5243 2024-02-16 15:51:36.000000 justai-3.2.6/justai/translator/xliff.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-02 09:52:41.526495 justai-3.2.6/justai.egg-info/
--rw-r--r--   0 hp         (501) staff       (20)     6408 2024-04-02 09:52:41.000000 justai-3.2.6/justai.egg-info/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)      785 2024-04-02 09:52:41.000000 justai-3.2.6/justai.egg-info/SOURCES.txt
--rw-r--r--   0 hp         (501) staff       (20)        1 2024-04-02 09:52:41.000000 justai-3.2.6/justai.egg-info/dependency_links.txt
--rw-r--r--   0 hp         (501) staff       (20)      137 2024-04-02 09:52:41.000000 justai-3.2.6/justai.egg-info/requires.txt
--rw-r--r--   0 hp         (501) staff       (20)        7 2024-04-02 09:52:41.000000 justai-3.2.6/justai.egg-info/top_level.txt
--rw-r--r--   0 hp         (501) staff       (20)      887 2024-04-02 09:52:39.000000 justai-3.2.6/pyproject.toml
--rw-r--r--   0 hp         (501) staff       (20)       38 2024-04-02 09:52:41.527281 justai-3.2.6/setup.cfg
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-04 16:26:04.606688 justai-3.2.7/
+-rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 justai-3.2.7/LICENSE
+-rw-r--r--   0 hp         (501) staff       (20)      198 2024-02-20 10:20:38.000000 justai-3.2.7/MANIFEST.in
+-rw-r--r--   0 hp         (501) staff       (20)     6408 2024-04-04 16:26:04.606345 justai-3.2.7/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)     4082 2024-04-04 16:26:02.000000 justai-3.2.7/README.md
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-04 16:26:04.595757 justai-3.2.7/justai/
+-rw-r--r--   0 hp         (501) staff       (20)      579 2024-04-01 20:26:06.000000 justai-3.2.7/justai/__init__.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-04 16:26:04.597725 justai-3.2.7/justai/agent/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:05:20.000000 justai-3.2.7/justai/agent/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     5992 2024-03-31 21:07:33.000000 justai-3.2.7/justai/agent/agent.py
+-rw-r--r--   0 hp         (501) staff       (20)      997 2024-03-05 16:49:21.000000 justai-3.2.7/justai/agent/message.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-04 16:26:04.598983 justai-3.2.7/justai/interactive/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:06:50.000000 justai-3.2.7/justai/interactive/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     5452 2024-02-07 19:49:01.000000 justai-3.2.7/justai/interactive/commands.py
+-rw-r--r--   0 hp         (501) staff       (20)     1320 2024-03-05 16:26:44.000000 justai-3.2.7/justai/interactive/repl.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-04 16:26:04.601332 justai-3.2.7/justai/models/
+-rw-r--r--   0 hp         (501) staff       (20)     2675 2024-04-02 08:20:07.000000 justai-3.2.7/justai/models/anthropic_models.py
+-rw-r--r--   0 hp         (501) staff       (20)     2334 2024-03-21 09:14:50.000000 justai-3.2.7/justai/models/gguf_models.py
+-rw-r--r--   0 hp         (501) staff       (20)      871 2024-03-21 08:22:51.000000 justai-3.2.7/justai/models/model.py
+-rw-r--r--   0 hp         (501) staff       (20)      709 2024-03-06 13:20:05.000000 justai-3.2.7/justai/models/modelfactory.py
+-rw-r--r--   0 hp         (501) staff       (20)     5807 2024-03-21 09:14:50.000000 justai-3.2.7/justai/models/openai_models.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-04 16:26:04.603272 justai-3.2.7/justai/tools/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:08:21.000000 justai-3.2.7/justai/tools/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     3815 2024-04-02 09:00:24.000000 justai-3.2.7/justai/tools/cache.py
+-rw-r--r--   0 hp         (501) staff       (20)      563 2023-08-26 19:32:55.000000 justai-3.2.7/justai/tools/display.py
+-rw-r--r--   0 hp         (501) staff       (20)     3226 2024-04-02 08:38:55.000000 justai-3.2.7/justai/tools/log.py
+-rw-r--r--   0 hp         (501) staff       (20)      615 2024-02-09 15:06:31.000000 justai-3.2.7/justai/tools/prompts.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-04 16:26:04.604881 justai-3.2.7/justai/translator/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:11:10.000000 justai-3.2.7/justai/translator/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     4052 2024-02-13 10:39:31.000000 justai-3.2.7/justai/translator/languages.py
+-rw-r--r--   0 hp         (501) staff       (20)     1551 2024-03-30 11:43:22.000000 justai-3.2.7/justai/translator/prompts.toml
+-rw-r--r--   0 hp         (501) staff       (20)    14079 2024-04-01 09:02:59.000000 justai-3.2.7/justai/translator/translator.py
+-rw-r--r--   0 hp         (501) staff       (20)     5243 2024-02-16 15:51:36.000000 justai-3.2.7/justai/translator/xliff.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-04 16:26:04.605483 justai-3.2.7/justai.egg-info/
+-rw-r--r--   0 hp         (501) staff       (20)     6408 2024-04-04 16:26:04.000000 justai-3.2.7/justai.egg-info/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)      785 2024-04-04 16:26:04.000000 justai-3.2.7/justai.egg-info/SOURCES.txt
+-rw-r--r--   0 hp         (501) staff       (20)        1 2024-04-04 16:26:04.000000 justai-3.2.7/justai.egg-info/dependency_links.txt
+-rw-r--r--   0 hp         (501) staff       (20)      137 2024-04-04 16:26:04.000000 justai-3.2.7/justai.egg-info/requires.txt
+-rw-r--r--   0 hp         (501) staff       (20)        7 2024-04-04 16:26:04.000000 justai-3.2.7/justai.egg-info/top_level.txt
+-rw-r--r--   0 hp         (501) staff       (20)      887 2024-04-04 16:26:02.000000 justai-3.2.7/pyproject.toml
+-rw-r--r--   0 hp         (501) staff       (20)       38 2024-04-04 16:26:04.606750 justai-3.2.7/setup.cfg
```

### Comparing `justai-3.2.6/LICENSE` & `justai-3.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `justai-3.2.6/PKG-INFO` & `justai-3.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: justai
-Version: 3.2.6
+Version: 3.2.7
 Summary: Makes working with OpenAI's GPT API and other LLM's super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -53,15 +53,15 @@
 Requires-Dist: nox; extra == "dev"
 
 # JustAI
 
 Package to make working with Large Language models in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 3.2.6
+Current version: 3.2.7
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install justai
 ~~~~
 2. Create an OpenAI acccount (for GPT3.5 / 4) [here](https://platform.openai.com/) or an Anthropic account [here](https://console.anthropic.com/)
```

### Comparing `justai-3.2.6/README.md` & `justai-3.2.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # JustAI
 
 Package to make working with Large Language models in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 3.2.6
+Current version: 3.2.7
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install justai
 ~~~~
 2. Create an OpenAI acccount (for GPT3.5 / 4) [here](https://platform.openai.com/) or an Anthropic account [here](https://console.anthropic.com/)
```

### Comparing `justai-3.2.6/justai/__init__.py` & `justai-3.2.7/justai/__init__.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.6/justai/agent/agent.py` & `justai-3.2.7/justai/agent/agent.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.6/justai/agent/message.py` & `justai-3.2.7/justai/agent/message.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.6/justai/interactive/commands.py` & `justai-3.2.7/justai/interactive/commands.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.6/justai/interactive/repl.py` & `justai-3.2.7/justai/interactive/repl.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.6/justai/models/anthropic_models.py` & `justai-3.2.7/justai/models/anthropic_models.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.6/justai/models/gguf_models.py` & `justai-3.2.7/justai/models/gguf_models.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.6/justai/models/model.py` & `justai-3.2.7/justai/models/model.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.6/justai/models/modelfactory.py` & `justai-3.2.7/justai/models/modelfactory.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.6/justai/models/openai_models.py` & `justai-3.2.7/justai/models/openai_models.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.6/justai/tools/cache.py` & `justai-3.2.7/justai/tools/cache.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.6/justai/tools/display.py` & `justai-3.2.7/justai/tools/display.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.6/justai/tools/log.py` & `justai-3.2.7/justai/tools/log.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.6/justai/tools/prompts.py` & `justai-3.2.7/justai/tools/prompts.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.6/justai/translator/languages.py` & `justai-3.2.7/justai/translator/languages.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.6/justai/translator/prompts.toml` & `justai-3.2.7/justai/translator/prompts.toml`

 * *Files identical despite different names*

### Comparing `justai-3.2.6/justai/translator/translator.py` & `justai-3.2.7/justai/translator/translator.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.6/justai/translator/xliff.py` & `justai-3.2.7/justai/translator/xliff.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.6/justai.egg-info/PKG-INFO` & `justai-3.2.7/justai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: justai
-Version: 3.2.6
+Version: 3.2.7
 Summary: Makes working with OpenAI's GPT API and other LLM's super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -53,15 +53,15 @@
 Requires-Dist: nox; extra == "dev"
 
 # JustAI
 
 Package to make working with Large Language models in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 3.2.6
+Current version: 3.2.7
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install justai
 ~~~~
 2. Create an OpenAI acccount (for GPT3.5 / 4) [here](https://platform.openai.com/) or an Anthropic account [here](https://console.anthropic.com/)
```

### Comparing `justai-3.2.6/justai.egg-info/SOURCES.txt` & `justai-3.2.7/justai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `justai-3.2.6/pyproject.toml` & `justai-3.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=69", "wheel>=0.42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "justai"
-version = "3.2.6"
+version = "3.2.7"
 description = "Makes working with OpenAI's GPT API and other LLM's super easy"
 readme = "README.md"
 authors = [{ name = "HP Harmsen", email = "hp@harmsen.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

