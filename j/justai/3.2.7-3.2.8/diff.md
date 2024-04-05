# Comparing `tmp/justai-3.2.7.tar.gz` & `tmp/justai-3.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "justai-3.2.7.tar", last modified: Thu Apr  4 16:26:04 2024, max compression
+gzip compressed data, was "justai-3.2.8.tar", last modified: Fri Apr  5 09:49:12 2024, max compression
```

## Comparing `justai-3.2.7.tar` & `justai-3.2.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-04 16:26:04.606688 justai-3.2.7/
--rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 justai-3.2.7/LICENSE
--rw-r--r--   0 hp         (501) staff       (20)      198 2024-02-20 10:20:38.000000 justai-3.2.7/MANIFEST.in
--rw-r--r--   0 hp         (501) staff       (20)     6408 2024-04-04 16:26:04.606345 justai-3.2.7/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)     4082 2024-04-04 16:26:02.000000 justai-3.2.7/README.md
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-04 16:26:04.595757 justai-3.2.7/justai/
--rw-r--r--   0 hp         (501) staff       (20)      579 2024-04-01 20:26:06.000000 justai-3.2.7/justai/__init__.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-04 16:26:04.597725 justai-3.2.7/justai/agent/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:05:20.000000 justai-3.2.7/justai/agent/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     5992 2024-03-31 21:07:33.000000 justai-3.2.7/justai/agent/agent.py
--rw-r--r--   0 hp         (501) staff       (20)      997 2024-03-05 16:49:21.000000 justai-3.2.7/justai/agent/message.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-04 16:26:04.598983 justai-3.2.7/justai/interactive/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:06:50.000000 justai-3.2.7/justai/interactive/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     5452 2024-02-07 19:49:01.000000 justai-3.2.7/justai/interactive/commands.py
--rw-r--r--   0 hp         (501) staff       (20)     1320 2024-03-05 16:26:44.000000 justai-3.2.7/justai/interactive/repl.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-04 16:26:04.601332 justai-3.2.7/justai/models/
--rw-r--r--   0 hp         (501) staff       (20)     2675 2024-04-02 08:20:07.000000 justai-3.2.7/justai/models/anthropic_models.py
--rw-r--r--   0 hp         (501) staff       (20)     2334 2024-03-21 09:14:50.000000 justai-3.2.7/justai/models/gguf_models.py
--rw-r--r--   0 hp         (501) staff       (20)      871 2024-03-21 08:22:51.000000 justai-3.2.7/justai/models/model.py
--rw-r--r--   0 hp         (501) staff       (20)      709 2024-03-06 13:20:05.000000 justai-3.2.7/justai/models/modelfactory.py
--rw-r--r--   0 hp         (501) staff       (20)     5807 2024-03-21 09:14:50.000000 justai-3.2.7/justai/models/openai_models.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-04 16:26:04.603272 justai-3.2.7/justai/tools/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:08:21.000000 justai-3.2.7/justai/tools/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     3815 2024-04-02 09:00:24.000000 justai-3.2.7/justai/tools/cache.py
--rw-r--r--   0 hp         (501) staff       (20)      563 2023-08-26 19:32:55.000000 justai-3.2.7/justai/tools/display.py
--rw-r--r--   0 hp         (501) staff       (20)     3226 2024-04-02 08:38:55.000000 justai-3.2.7/justai/tools/log.py
--rw-r--r--   0 hp         (501) staff       (20)      615 2024-02-09 15:06:31.000000 justai-3.2.7/justai/tools/prompts.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-04 16:26:04.604881 justai-3.2.7/justai/translator/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:11:10.000000 justai-3.2.7/justai/translator/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     4052 2024-02-13 10:39:31.000000 justai-3.2.7/justai/translator/languages.py
--rw-r--r--   0 hp         (501) staff       (20)     1551 2024-03-30 11:43:22.000000 justai-3.2.7/justai/translator/prompts.toml
--rw-r--r--   0 hp         (501) staff       (20)    14079 2024-04-01 09:02:59.000000 justai-3.2.7/justai/translator/translator.py
--rw-r--r--   0 hp         (501) staff       (20)     5243 2024-02-16 15:51:36.000000 justai-3.2.7/justai/translator/xliff.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-04 16:26:04.605483 justai-3.2.7/justai.egg-info/
--rw-r--r--   0 hp         (501) staff       (20)     6408 2024-04-04 16:26:04.000000 justai-3.2.7/justai.egg-info/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)      785 2024-04-04 16:26:04.000000 justai-3.2.7/justai.egg-info/SOURCES.txt
--rw-r--r--   0 hp         (501) staff       (20)        1 2024-04-04 16:26:04.000000 justai-3.2.7/justai.egg-info/dependency_links.txt
--rw-r--r--   0 hp         (501) staff       (20)      137 2024-04-04 16:26:04.000000 justai-3.2.7/justai.egg-info/requires.txt
--rw-r--r--   0 hp         (501) staff       (20)        7 2024-04-04 16:26:04.000000 justai-3.2.7/justai.egg-info/top_level.txt
--rw-r--r--   0 hp         (501) staff       (20)      887 2024-04-04 16:26:02.000000 justai-3.2.7/pyproject.toml
--rw-r--r--   0 hp         (501) staff       (20)       38 2024-04-04 16:26:04.606750 justai-3.2.7/setup.cfg
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 09:49:12.954539 justai-3.2.8/
+-rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 justai-3.2.8/LICENSE
+-rw-r--r--   0 hp         (501) staff       (20)      198 2024-02-20 10:20:38.000000 justai-3.2.8/MANIFEST.in
+-rw-r--r--   0 hp         (501) staff       (20)     6408 2024-04-05 09:49:12.954273 justai-3.2.8/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)     4082 2024-04-05 09:49:11.000000 justai-3.2.8/README.md
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 09:49:12.946875 justai-3.2.8/justai/
+-rw-r--r--   0 hp         (501) staff       (20)      579 2024-04-01 20:26:06.000000 justai-3.2.8/justai/__init__.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 09:49:12.948410 justai-3.2.8/justai/agent/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:05:20.000000 justai-3.2.8/justai/agent/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     5992 2024-03-31 21:07:33.000000 justai-3.2.8/justai/agent/agent.py
+-rw-r--r--   0 hp         (501) staff       (20)      997 2024-03-05 16:49:21.000000 justai-3.2.8/justai/agent/message.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 09:49:12.949186 justai-3.2.8/justai/interactive/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:06:50.000000 justai-3.2.8/justai/interactive/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     5452 2024-02-07 19:49:01.000000 justai-3.2.8/justai/interactive/commands.py
+-rw-r--r--   0 hp         (501) staff       (20)     1320 2024-03-05 16:26:44.000000 justai-3.2.8/justai/interactive/repl.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 09:49:12.950634 justai-3.2.8/justai/models/
+-rw-r--r--   0 hp         (501) staff       (20)     2833 2024-04-05 09:47:29.000000 justai-3.2.8/justai/models/anthropic_models.py
+-rw-r--r--   0 hp         (501) staff       (20)     2334 2024-03-21 09:14:50.000000 justai-3.2.8/justai/models/gguf_models.py
+-rw-r--r--   0 hp         (501) staff       (20)      871 2024-03-21 08:22:51.000000 justai-3.2.8/justai/models/model.py
+-rw-r--r--   0 hp         (501) staff       (20)      709 2024-03-06 13:20:05.000000 justai-3.2.8/justai/models/modelfactory.py
+-rw-r--r--   0 hp         (501) staff       (20)     5907 2024-04-04 20:33:40.000000 justai-3.2.8/justai/models/openai_models.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 09:49:12.951978 justai-3.2.8/justai/tools/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:08:21.000000 justai-3.2.8/justai/tools/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     3815 2024-04-02 09:00:24.000000 justai-3.2.8/justai/tools/cache.py
+-rw-r--r--   0 hp         (501) staff       (20)      563 2023-08-26 19:32:55.000000 justai-3.2.8/justai/tools/display.py
+-rw-r--r--   0 hp         (501) staff       (20)     3226 2024-04-02 08:38:55.000000 justai-3.2.8/justai/tools/log.py
+-rw-r--r--   0 hp         (501) staff       (20)      615 2024-02-09 15:06:31.000000 justai-3.2.8/justai/tools/prompts.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 09:49:12.953220 justai-3.2.8/justai/translator/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:11:10.000000 justai-3.2.8/justai/translator/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     4052 2024-02-13 10:39:31.000000 justai-3.2.8/justai/translator/languages.py
+-rw-r--r--   0 hp         (501) staff       (20)     1759 2024-04-05 09:44:01.000000 justai-3.2.8/justai/translator/prompts.toml
+-rw-r--r--   0 hp         (501) staff       (20)    14332 2024-04-04 21:45:33.000000 justai-3.2.8/justai/translator/translator.py
+-rw-r--r--   0 hp         (501) staff       (20)     5243 2024-02-16 15:51:36.000000 justai-3.2.8/justai/translator/xliff.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 09:49:12.953664 justai-3.2.8/justai.egg-info/
+-rw-r--r--   0 hp         (501) staff       (20)     6408 2024-04-05 09:49:12.000000 justai-3.2.8/justai.egg-info/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)      785 2024-04-05 09:49:12.000000 justai-3.2.8/justai.egg-info/SOURCES.txt
+-rw-r--r--   0 hp         (501) staff       (20)        1 2024-04-05 09:49:12.000000 justai-3.2.8/justai.egg-info/dependency_links.txt
+-rw-r--r--   0 hp         (501) staff       (20)      137 2024-04-05 09:49:12.000000 justai-3.2.8/justai.egg-info/requires.txt
+-rw-r--r--   0 hp         (501) staff       (20)        7 2024-04-05 09:49:12.000000 justai-3.2.8/justai.egg-info/top_level.txt
+-rw-r--r--   0 hp         (501) staff       (20)      887 2024-04-05 09:49:11.000000 justai-3.2.8/pyproject.toml
+-rw-r--r--   0 hp         (501) staff       (20)       38 2024-04-05 09:49:12.954597 justai-3.2.8/setup.cfg
```

### Comparing `justai-3.2.7/LICENSE` & `justai-3.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `justai-3.2.7/PKG-INFO` & `justai-3.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: justai
-Version: 3.2.7
+Version: 3.2.8
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
-Current version: 3.2.7
+Current version: 3.2.8
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install justai
 ~~~~
 2. Create an OpenAI acccount (for GPT3.5 / 4) [here](https://platform.openai.com/) or an Anthropic account [here](https://console.anthropic.com/)
```

### Comparing `justai-3.2.7/README.md` & `justai-3.2.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # JustAI
 
 Package to make working with Large Language models in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 3.2.7
+Current version: 3.2.8
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install justai
 ~~~~
 2. Create an OpenAI acccount (for GPT3.5 / 4) [here](https://platform.openai.com/) or an Anthropic account [here](https://console.anthropic.com/)
```

### Comparing `justai-3.2.7/justai/__init__.py` & `justai-3.2.8/justai/__init__.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.7/justai/agent/agent.py` & `justai-3.2.8/justai/agent/agent.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.7/justai/agent/message.py` & `justai-3.2.8/justai/agent/message.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.7/justai/interactive/commands.py` & `justai-3.2.8/justai/interactive/commands.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.7/justai/interactive/repl.py` & `justai-3.2.8/justai/interactive/repl.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.7/justai/models/anthropic_models.py` & `justai-3.2.8/justai/models/anthropic_models.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,62 +3,68 @@
 
 import anthropic
 from dotenv import load_dotenv
 
 from justai.models.model import Model
 from justai.tools.display import ERROR_COLOR, color_print
 
+
 # Claude 3 Opus	    claude-3-opus-20240229
 # Claude 3 Sonnet	claude-3-sonnet-20240229
 # Claude 3 Haiku	Coming soon
 
 
 class AnthropicModel(Model):
 
     def __init__(self, model_name: str, params: dict):
         """ Model implemention should create attributes for all supported parameters """
         system_message = f"You are {model_name}, a large language model trained by Anthropic."
         super().__init__(model_name, params, system_message)
 
         # Authentication
-        if not os.getenv("ANTHROPIC_API_KEY"):
-            load_dotenv()  # Load the .env file into the environment
-        api_key = os.getenv("ANTHROPIC_API_KEY")
+        if "ANTHROPIC_API_KEY" in params:
+            api_key = params["ANTHROPIC_API_KEY"]
+        else:
+            if not os.getenv("ANTHROPIC_API_KEY"):
+                load_dotenv()  # Load the .env file into the environment
+            api_key = os.getenv("ANTHROPIC_API_KEY")
         if not api_key:
             color_print("No Anthropic API key found. Create one at https://console.anthropic.com/settings/keys and " +
                         "set it in the .env file like ANTHROPIC_API_KEY=here_comes_your_key.", color=ERROR_COLOR)
-        
+
         # Client
+        print("API Key: ", api_key)
         self.client = anthropic.Anthropic(api_key=api_key)
 
         # Model specific parameters
         self.model_params['max_tokens'] = params.get('max_tokens', 800)
         self.model_params['temperature'] = params.get('temperature', 0.8)
 
-    def chat(self,  messages: list[dict], return_json: bool, max_retries=None) -> tuple[[str | object], int, int]:
+    def chat(self, messages: list[dict], return_json: bool, max_retries=None, log=None) -> tuple[[str | object], int, int]:
         if max_retries is None:
             max_retries = 3
 
         anthropic_messages = [{"role": m['role'],
                                "content": [{"type": "text",
                                             "text": m['content']}]
                                } for m in messages if m['role'] != 'system']
         if return_json:
             anthropic_messages += [{"role": 'assistant',
                                     "content": [{"type": "text",
-                                                "text": "sure here's your json: {"}]
+                                                 "text": "sure here's your json: {"}]
                                     }]
 
         message = self.client.messages.create(
             model=self.model_name,
             max_tokens=self.model_params['max_tokens'],
             temperature=self.model_params['temperature'],
             system=self.system_message,
             messages=anthropic_messages
         )
+
         response = message.content[0].text
         if return_json:
             response = json.loads('{' + response)
         input_tokens = message.usage.input_tokens
         output_tokens = message.usage.output_tokens
         return response, input_tokens, output_tokens
```

### Comparing `justai-3.2.7/justai/models/gguf_models.py` & `justai-3.2.8/justai/models/gguf_models.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.7/justai/models/model.py` & `justai-3.2.8/justai/models/model.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.7/justai/models/modelfactory.py` & `justai-3.2.8/justai/models/modelfactory.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.7/justai/models/openai_models.py` & `justai-3.2.8/justai/models/openai_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,20 @@
 
 class OpenAIModel(Model):
     def __init__(self, model_name: str, params: dict = None):
         system_message = f"You are {model_name}, a large language model trained by OpenAI."
         super().__init__(model_name, params, system_message)
 
         # Authentication
-        if not os.getenv("OPENAI_API_KEY"):
-            load_dotenv()  # Load the .env file into the environment
-        openai.api_key = os.getenv("OPENAI_API_KEY")
+        if "OPENAI_API_KEY" in params:
+            api_key = params["OPENAI_API_KEY"]
+        else:
+            if not os.getenv("OPENAI_API_KEY"):
+                load_dotenv()  # Load the .env file into the environment
+            openai.api_key = os.getenv("OPENAI_API_KEY")
         if not openai.api_key:
             color_print("No OpenAI API key found. Create one at https://platform.openai.com/account/api-keys and " +
                         "set it in the .env file like OPENAI_API_KEY=here_comes_your_key.", color=ERROR_COLOR)
         self.client = OpenAI()
 
         # The maximum number of tokens to generate in the completion.
         # Defaults to 16
@@ -66,15 +69,15 @@
         # decreasing the model's likelihood to repeat the same line verbatim.
         # Defaults to 0
         self.model_params['frequency_penalty'] = params.get('frequency_penalty', 0)
 
     def chat(self, messages: list[dict], return_json: bool, use_cache: bool = False, max_retries=None):
         if max_retries is None:
             max_retries = 3
-            
+
         if self.debug:
             color_print("\nRunning completion with these messages", color=DEBUG_COLOR1)
             [color_print(m, color=DEBUG_COLOR1) for m in messages if hasattr(m, 'text')]
             print()
 
         last_error = None
         for _ in range(max_retries):
```

### Comparing `justai-3.2.7/justai/tools/cache.py` & `justai-3.2.8/justai/tools/cache.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.7/justai/tools/display.py` & `justai-3.2.8/justai/tools/display.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.7/justai/tools/log.py` & `justai-3.2.8/justai/tools/log.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.7/justai/tools/prompts.py` & `justai-3.2.8/justai/tools/prompts.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.7/justai/translator/languages.py` & `justai-3.2.8/justai/translator/languages.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.7/justai/translator/prompts.toml` & `justai-3.2.8/justai/translator/prompts.toml`

 * *Files 7% similar despite different names*

```diff
@@ -10,16 +10,19 @@
 {translate_str}
 
 **Belangrijke instructies voor de vertaling:**
 
 - **Alleen tekst vertalen:** Vertaal enkel de tekst die zich bevindt tussen de dubbele vierkante haakjes `[[` en `]]`.
 - **Behoud van speciale tekens:** Alle spaties, tabs, leestekens, `@@`, `###`, symbolen, en andere speciale tekens moeten exact behouden blijven zoals ze in de oorspronkelijke tekst staan.
 - **Formatteerkenmerken behouden:** Als een tekst eindigt op `@@`, de vertaalde tekst moet ook eindigen op `@@`.
-- **Strikte behoud van structuur:** Let er specifiek op dat alle structurele elementen, inclusief dubbele pipelines (||), in exact dezelfde hoeveelheid en op dezelfde posities behouden blijven in de vertaling als in de originele tekst. De integriteit van deze elementen is cruciaal voor de juiste formatteer- en interpretatiedoeleinden.
-
+- **Strikte behoud van structuur:** Let er specifiek op dat alle structurele elementen, inclusief dubbele pipelines (||),
+in exact dezelfde hoeveelheid en op dezelfde posities behouden blijven in de vertaling als in de originele tekst.
+De integriteit van deze elementen is cruciaal voor de juiste formatteer- en interpretatiedoeleinden.
+Probeer waar mogelijk de lengte van de stukken tekst tussen || zoveel mogelijk gelijk te houden.
+- **Volgorde behouden:** Behoud de volgorde van de {count} teksten zoals die in de oorspronkelijke tekst staan.
 **Vertaalverzoek:**
 
 Geef de vertalingen terug met behoud van de originele structuur, nummering, en formatteerkenmerken.
 Gebruik de dubbele rechte haakjes om de vertaalde tekst aan te geven.
 
 ** Belangrijk**
 Na vertaling, controleer a.u.b. zorgvuldig of het aantal en de plaatsing van dubbele pipelines (||) exact overeenkomen met die in de originele tekst. Deze stap is cruciaal voor de nauwkeurigheid en integriteit van de vertaling."""
```

### Comparing `justai-3.2.7/justai/translator/translator.py` & `justai-3.2.8/justai/translator/translator.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 from justai.tools.log import Log
 from justai.tools.prompts import get_prompt, set_prompt_file
 from justai.translator.languages import LANGUAGES
 
 
 class Translator(Agent):
 
-    def __init__(self, model=None):
+    def __init__(self, model=None, **kwargs):
         if not model:
             model = os.environ.get('MODEL', 'claude-3-opus-20240229')
-        super().__init__(model, temperature=0, max_tokens=4096)
+        super().__init__(model, temperature=0, max_tokens=4096, **kwargs)
         set_prompt_file(Path(__file__).parent / 'prompts.toml')
         self.system_message = get_prompt('SYSTEM')
         self.xml = ''
         self.version = ''
         self.logger = Log()
 
     def load(self, input_file: str | Path):
@@ -50,49 +50,48 @@
     def translate(self, language: str, string_cached: bool = False) -> str:
         log = self.logger
         parser = etree.XMLParser(ns_clean=True)
         root = etree.fromstring(self.xml.encode('utf-8'), parser=parser)
         namespaces = {'ns': f'urn:oasis:names:tc:xliff:document:{self.version}'}
 
         segment_name = 'trans-unit' if self.version == '1.2' else 'segment'
-            
+
         if self.version >= '2.0':
             root.attrib['trgLang'] = LANGUAGES.get(language)
 
         # Verzamel teksten als lijst van samengevoegde strings per <source>
         all_texts = []
         translatable_texts = []
         for source in root.xpath('.//ns:source', namespaces=namespaces):
             texts = collect_texts_from_element(source)
             all_texts.append(texts)
             # Verzamel alleen de teksten die ook echt vertaald moeten worden
             translatable_text = "||".join(text for text in texts if is_translatable(text))
             if translatable_text:
                 translatable_texts.append(translatable_text)
-        log.info('all_texts', all_texts)
-        log.info('translatable_texts', translatable_texts)
+        log.info('translate - all_texts', all_texts)
+        log.info('translate - translatable_texts', translatable_texts)
 
         # Vertaal de lijst van samengevoegde strings
         translated_texts = self.do_translate(translatable_texts, language, string_cached=string_cached)
-        log.info('translated_texts', translated_texts)      
-        for src, dst in zip(translatable_texts, translated_texts):
-            assert len(src.split('||')) == len(dst.split('||'))
-        
+
         # Zet nu de delen die niet vertaald hoefden te worden terug in de lijst
         for i1, line in enumerate(all_texts):
             if any(is_translatable(text) for text in line):
                 sc = len([l for l in line if is_translatable(l)])
                 tc = len(translated_texts[0].split("||"))
                 if sc != tc:
-                    log.error('mismatch', f'Translated texts ({sc}) does not match number of source texts ({tc})')
-                    log.info('line', line)
-                    log.info('original:', [l for l in line if is_translatable(l)])
-                    log.info('Translated:', translated_texts[0].split("||"))
-                assert len([l for l in line if is_translatable(l)]) == len(translated_texts[0].split("||"))
-                
+                    log.error('translate - mismatch',
+                              f'Translated texts ({sc}) does not match number of source texts ({tc})')
+                    log.info('translate - line', line)
+                    log.info('translate - Original:', [l for l in line if is_translatable(l)])
+                    log.info('translate - Translated:', translated_texts[0].split("||"))
+                assert len([l for l in line if is_translatable(l)]) == len(
+                    translated_texts[0].split("||")), 'Mismatch see log'
+
                 translated = translated_texts.pop(0).split("||")
                 for index, text in enumerate(line):
                     if is_translatable(text):
                         line[index] = translated.pop(0)
         translated_texts = [item for sublist in all_texts for item in sublist]  # And flatten
 
         # Plaats vertaalde teksten in nieuwe <target> elementen met behoud van structuur
@@ -104,16 +103,15 @@
 
         updated_xml = etree.tostring(root, pretty_print=True, xml_declaration=True, encoding='UTF-8').decode('utf-8')
         return updated_xml
 
     def do_translate(self, texts, language: str, string_cached=False):
         log = self.logger
 
-        # source_list = list(set([text for text in texts if is_translatable(text)]))  # Filter out doubles
-        assert all(is_translatable(text) for text in texts)  # !! Tijdelijk
+        assert all(is_translatable(text) for text in texts), "Not all translatable"  # !! Tijdelijk
         source_list = list(set(texts))
         cache = StringCache(language) if string_cached else {}
         source_list = [text for text in source_list if text not in cache]
 
         if source_list:
             variables = []
             source_str_no_vars = ''
@@ -123,49 +121,54 @@
                 source_str_no_vars += f'{index + 1} [[{text_no_vars}]]\n'
             prompt = get_prompt('TRANSLATE_MULTIPLE', language=language, translate_str=source_str_no_vars,
                                 count=len(source_list))
             log.prompt('prompt', prompt)
             target_str_no_vars = self.chat(prompt, return_json=False)
             log.response('target_str_no_vars', target_str_no_vars)
             target_str = replace_hash_with_variables(target_str_no_vars, variables)
-            log.info('target_str', target_str)
+            log.info('do_translate - target_str', target_str)
 
             target_list = [t.split(']]')[0] for t in target_str.split('[[')[1:]]
             translation_dict = dict(zip(source_list, target_list))
-            log.info('translation_dict', translation_dict)
+            log.info('do_translate - translation_dict', translation_dict)
 
             count = 1
             for source, translation in translation_dict.items():
 
                 source_parts = source.split('||')
                 translation_parts = translation.split('||')
-                log.info('source_parts', source_parts)
-                log.info('translation_parts', translation_parts)
+                log.info('do_translate - source_parts', source_parts)
 
                 # Check op het aantal onderdelen tussen ||. Dit moet gelijk zijn in de bron en de vertaling
                 sc = len(source_parts)
                 tc = len(translation_parts)
                 if tc != sc:
-                    log.error('do_translate',
-                              f'Number of translated texts ({tc}) does not match number of source texts ({sc}).')
+                    log.warning('do_translate',
+                                f'Number of translated texts ({tc}) does not match number of source texts ({sc}). Correcting.')
                     if tc < sc:
                         translation_parts += [' '] * (sc - tc)
                     else:
                         # Dit is een hack! Het model geeft kennelijk meer ||'s terug in dan in het origineel.
                         # Dat breekt de code verderop. Daarom voegen we de laatste onderdelen samen.
                         # Maar dat levert wel een onjuiste vertaling op.
                         translation_parts = translation_parts[:sc - 1] + [' '.join(translation_parts[sc - 1:])]
-                assert len(source_parts) == len(translation_parts)
+                    sc = len(source_parts)
+                    tc = len(translation_parts)
+                    if tc != sc:
+                        log.error('do_translate',
+                                  f'Number of translated texts ({tc}) still does not match number of source texts ({sc}). Correcting.')
+                    assert (tc == sc), 'Mismatch in number of parts, see log for info'
 
                 # Zorg dat de vertaling dezelfde whitespace aan het begin en eind heeft als de bron
                 for i, (source_part, translation_part) in enumerate(zip(source_parts, translation_parts)):
                     if source_part.strip() and (source_part[0] == ' ' or source_part[-1] == ' '):
                         start_spaces = (len(source_part) - len(source_part.lstrip(' '))) * ' '
                         end_spaces = (len(source_part) - len(source_part.rstrip(' '))) * ' '
                         translation_parts[i] = start_spaces + translation_part.strip() + end_spaces
+                log.info('do_translate - translation_parts', source_parts)
                 translation = '||'.join(translation_parts)
 
                 log.info('', f'{count}. [{source}] -> [{translation}]')
                 count += 1
                 ratio = len(source) / len(translation)
                 if ratio >= 1.5 or ratio <= 0.7:
                     log.warning('', f'Vertaling van {source} naar {translation} is onverwacht lang of kort')
```

### Comparing `justai-3.2.7/justai/translator/xliff.py` & `justai-3.2.8/justai/translator/xliff.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.7/justai.egg-info/PKG-INFO` & `justai-3.2.8/justai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: justai
-Version: 3.2.7
+Version: 3.2.8
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
-Current version: 3.2.7
+Current version: 3.2.8
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install justai
 ~~~~
 2. Create an OpenAI acccount (for GPT3.5 / 4) [here](https://platform.openai.com/) or an Anthropic account [here](https://console.anthropic.com/)
```

### Comparing `justai-3.2.7/justai.egg-info/SOURCES.txt` & `justai-3.2.8/justai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `justai-3.2.7/pyproject.toml` & `justai-3.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=69", "wheel>=0.42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "justai"
-version = "3.2.7"
+version = "3.2.8"
 description = "Makes working with OpenAI's GPT API and other LLM's super easy"
 readme = "README.md"
 authors = [{ name = "HP Harmsen", email = "hp@harmsen.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

