# Comparing `tmp/llama_index_llms_palm-0.1.4.tar.gz` & `tmp/llama_index_llms_palm-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_palm-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_llms_palm-0.1.5.tar", max compression
```

## Comparing `llama_index_llms_palm-0.1.4.tar` & `llama_index_llms_palm-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       36 2024-03-20 20:45:24.835482 llama_index_llms_palm-0.1.4/README.md
--rw-r--r--   0        0        0       64 2024-03-20 20:45:24.835482 llama_index_llms_palm-0.1.4/llama_index/llms/palm/__init__.py
--rw-r--r--   0        0        0     4412 2024-03-20 20:45:24.835482 llama_index_llms_palm-0.1.4/llama_index/llms/palm/base.py
--rw-r--r--   0        0        0     1449 2024-03-20 20:45:24.835482 llama_index_llms_palm-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 llama_index_llms_palm-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       36 2024-04-05 18:55:12.264015 llama_index_llms_palm-0.1.5/README.md
+-rw-r--r--   0        0        0       64 2024-04-05 18:55:12.264015 llama_index_llms_palm-0.1.5/llama_index/llms/palm/__init__.py
+-rw-r--r--   0        0        0     5253 2024-04-05 18:55:12.264015 llama_index_llms_palm-0.1.5/llama_index/llms/palm/base.py
+-rw-r--r--   0        0        0     1449 2024-04-05 18:55:12.264015 llama_index_llms_palm-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 llama_index_llms_palm-0.1.5/PKG-INFO
```

### Comparing `llama_index_llms_palm-0.1.4/llama_index/llms/palm/base.py` & `llama_index_llms_palm-0.1.5/llama_index/llms/palm/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Palm API."""
+
 import os
 from typing import Any, Callable, Optional, Sequence
 
 import google.generativeai as palm
 from llama_index.core.base.llms.types import (
     ChatMessage,
     CompletionResponse,
@@ -16,15 +17,45 @@
 from llama_index.core.llms.custom import CustomLLM
 from llama_index.core.types import BaseOutputParser, PydanticProgramMode
 
 DEFAULT_PALM_MODEL = "models/text-bison-001"
 
 
 class PaLM(CustomLLM):
-    """PaLM LLM."""
+    """PaLM LLM.
+
+    Examples:
+        `pip install llama-index-llms-palm`
+
+        ```python
+        import google.generativeai as palm
+
+        # API key for PaLM
+        palm_api_key = "YOUR_API_KEY_HERE"
+
+        # List all models that support text generation
+        models = [
+            m
+            for m in palm.list_models()
+            if "generateText" in m.supported_generation_methods
+        ]
+        model = models[0].name
+        print(model)
+
+        # Start using our PaLM LLM abstraction
+        from llama_index.llms.palm import PaLM
+
+        # Create an instance of the PaLM class with the API key
+        llm = PaLM(model_name=model, api_key=palm_api_key)
+
+        # Use the complete method to generate text based on a prompt
+        response = llm.complete("Your prompt text here.")
+        print(str(response))
+        ```
+    """
 
     model_name: str = Field(
         default=DEFAULT_PALM_MODEL, description="The PaLM model to use."
     )
     num_output: int = Field(
         default=DEFAULT_NUM_OUTPUTS,
         description="The number of tokens to generate.",
```

### Comparing `llama_index_llms_palm-0.1.4/pyproject.toml` & `llama_index_llms_palm-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms palm integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-palm"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 llama-index-core = "^0.10.11.post1"
-google-generativeai = "^0.3.2"
+google-generativeai = "^0.4.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_llms_palm-0.1.4/PKG-INFO` & `llama_index_llms_palm-0.1.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-palm
-Version: 0.1.4
+Version: 0.1.5
 Summary: llama-index llms palm integration
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
 Description-Content-Type: text/markdown
 
 # LlamaIndex Llms Integration: Palm
```

