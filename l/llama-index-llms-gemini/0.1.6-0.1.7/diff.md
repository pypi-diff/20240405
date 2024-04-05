# Comparing `tmp/llama_index_llms_gemini-0.1.6.tar.gz` & `tmp/llama_index_llms_gemini-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_gemini-0.1.6.tar", max compression
+gzip compressed data, was "llama_index_llms_gemini-0.1.7.tar", max compression
```

## Comparing `llama_index_llms_gemini-0.1.6.tar` & `llama_index_llms_gemini-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       38 2024-03-20 20:45:24.819482 llama_index_llms_gemini-0.1.6/README.md
--rw-r--r--   0        0        0       70 2024-03-20 20:45:24.819482 llama_index_llms_gemini-0.1.6/llama_index/llms/gemini/__init__.py
--rw-r--r--   0        0        0     6778 2024-03-20 20:45:24.819482 llama_index_llms_gemini-0.1.6/llama_index/llms/gemini/base.py
--rw-r--r--   0        0        0     2450 2024-03-20 20:45:24.819482 llama_index_llms_gemini-0.1.6/llama_index/llms/gemini/utils.py
--rw-r--r--   0        0        0     1476 2024-03-20 20:45:24.819482 llama_index_llms_gemini-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      683 1970-01-01 00:00:00.000000 llama_index_llms_gemini-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       38 2024-04-05 18:55:12.248015 llama_index_llms_gemini-0.1.7/README.md
+-rw-r--r--   0        0        0       70 2024-04-05 18:55:12.248015 llama_index_llms_gemini-0.1.7/llama_index/llms/gemini/__init__.py
+-rw-r--r--   0        0        0     7097 2024-04-05 18:55:12.248015 llama_index_llms_gemini-0.1.7/llama_index/llms/gemini/base.py
+-rw-r--r--   0        0        0     2450 2024-04-05 18:55:12.248015 llama_index_llms_gemini-0.1.7/llama_index/llms/gemini/utils.py
+-rw-r--r--   0        0        0     1476 2024-04-05 18:55:12.248015 llama_index_llms_gemini-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      683 1970-01-01 00:00:00.000000 llama_index_llms_gemini-0.1.7/PKG-INFO
```

### Comparing `llama_index_llms_gemini-0.1.6/llama_index/llms/gemini/base.py` & `llama_index_llms_gemini-0.1.7/llama_index/llms/gemini/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,15 +34,27 @@
 GEMINI_MODELS = (
     "models/gemini-pro",
     "models/gemini-ultra",
 )
 
 
 class Gemini(CustomLLM):
-    """Gemini."""
+    """Gemini LLM.
+
+    Examples:
+        `pip install llama-index-llms-gemini`
+
+        ```python
+        from llama_index.llms.gemini import Gemini
+
+        llm = Gemini(model_name="models/gemini-ultra", api_key="YOUR_API_KEY")
+        resp = llm.complete("Write a poem about a magic backpack")
+        print(resp)
+        ```
+    """
 
     model_name: str = Field(
         default=GEMINI_MODELS[0], description="The Gemini model to use."
     )
     temperature: float = Field(
         default=DEFAULT_TEMPERATURE,
         description="The temperature to use during generation.",
```

### Comparing `llama_index_llms_gemini-0.1.6/llama_index/llms/gemini/utils.py` & `llama_index_llms_gemini-0.1.7/llama_index/llms/gemini/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_gemini-0.1.6/pyproject.toml` & `llama_index_llms_gemini-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms gemini integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-gemini"
 readme = "README.md"
-version = "0.1.6"
+version = "0.1.7"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 llama-index-core = "^0.10.11.post1"
 pillow = "^10.2.0"
-google-generativeai = "^0.3.2"
+google-generativeai = "^0.4.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_llms_gemini-0.1.6/PKG-INFO` & `llama_index_llms_gemini-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-gemini
-Version: 0.1.6
+Version: 0.1.7
 Summary: llama-index llms gemini integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: google-generativeai (>=0.3.2,<0.4.0)
+Requires-Dist: google-generativeai (>=0.4.1,<0.5.0)
 Requires-Dist: llama-index-core (>=0.10.11.post1,<0.11.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Llms Integration: Gemini
```

