# Comparing `tmp/llama_index_llms_databricks-0.1.0.tar.gz` & `tmp/llama_index_llms_databricks-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_databricks-0.1.0.tar", max compression
+gzip compressed data, was "llama_index_llms_databricks-0.1.1.tar", max compression
```

## Comparing `llama_index_llms_databricks-0.1.0.tar` & `llama_index_llms_databricks-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1171 2024-04-03 02:38:42.558184 llama_index_llms_databricks-0.1.0/README.md
--rw-r--r--   0        0        0       17 2024-04-03 02:38:42.558184 llama_index_llms_databricks-0.1.0/llama_index/llms/databricks/BUILD
--rw-r--r--   0        0        0       82 2024-04-03 02:38:42.558184 llama_index_llms_databricks-0.1.0/llama_index/llms/databricks/__init__.py
--rw-r--r--   0        0        0     1388 2024-04-03 02:38:42.558184 llama_index_llms_databricks-0.1.0/llama_index/llms/databricks/base.py
--rw-r--r--   0        0        0     1628 2024-04-03 02:38:42.558184 llama_index_llms_databricks-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1816 1970-01-01 00:00:00.000000 llama_index_llms_databricks-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1129 2024-04-05 18:58:54.788307 llama_index_llms_databricks-0.1.1/README.md
+-rw-r--r--   0        0        0       17 2024-04-05 18:58:54.788307 llama_index_llms_databricks-0.1.1/llama_index/llms/databricks/BUILD
+-rw-r--r--   0        0        0       82 2024-04-05 18:58:54.788307 llama_index_llms_databricks-0.1.1/llama_index/llms/databricks/__init__.py
+-rw-r--r--   0        0        0     1370 2024-04-05 18:58:54.788307 llama_index_llms_databricks-0.1.1/llama_index/llms/databricks/base.py
+-rw-r--r--   0        0        0     1628 2024-04-05 18:58:54.788307 llama_index_llms_databricks-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1774 1970-01-01 00:00:00.000000 llama_index_llms_databricks-0.1.1/PKG-INFO
```

### Comparing `llama_index_llms_databricks-0.1.0/README.md` & `llama_index_llms_databricks-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 # LlamaIndex Llms Integration: Databricks
 
 ## Overview
 
-Integrate with DataBricks LLMs APIs.
+Integrate with Databricks LLMs APIs.
 
 ## Installation
 
 ```bash
 pip install llama-index-llms-databricks
 ```
 
 ## Example
 
 With environmental variables.
 
 ```.env
-DATABRICKS_API_KEY=your_api_key
-DATABRICKS_API_BASE=https://[your-work-space].cloud.databricks.com/serving-endpoints/[your-serving-endpoint]
+DATABRICKS_TOKEN=your_api_key
+DATABRICKS_SERVING_ENDPOINT=https://[your-work-space].cloud.databricks.com/serving-endpoints
 ```
 
 ```python
-from llama_index.llms.databricks import DataBricks
+from llama_index.llms.databricks import Databricks
 
-# Initialize DataBricks LLM without explicitly passing the API key and base
-llm = DataBricks(model="databricks-dbrx-instruct")
+# Initialize Databricks LLM without explicitly passing the API key and base
+llm = Databricks(model="databricks-dbrx-instruct")
 
 # Make a query to the LLM
 response = llm.complete("Explain the importance of open source LLMs")
 
 print(response)
 ```
 
 Without environmental variables
 
 ```python
-from llama_index.llms.databricks import DataBricks
+from llama_index.llms.databricks import Databricks
 
-# Set up the DataBricks class with the required model, API key and serving endpoint
-llm = DataBricks(
+# Set up the Databricks class with the required model, API key and serving endpoint
+llm = Databricks(
     model="databricks-dbrx-instruct",
     api_key="your_api_key",
-    api_base="https://[your-work-space].cloud.databricks.com/serving-endpoints/[your-serving-endpoint]",
+    api_base="https://[your-work-space].cloud.databricks.com/serving-endpoints",
 )
 
 # Call the complete method with a query
 response = llm.complete("Explain the importance of open source LLMs")
 
 print(response)
 ```
```

### Comparing `llama_index_llms_databricks-0.1.0/llama_index/llms/databricks/base.py` & `llama_index_llms_databricks-0.1.1/llama_index/llms/databricks/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
 from typing import Any, Optional
 
 from llama_index.llms.openai_like import OpenAILike
 
 
-class DataBricks(OpenAILike):
-    """DataBricks LLM.
+class Databricks(OpenAILike):
+    """Databricks LLM.
 
     Examples:
         `pip install llama-index-llms-databricks`
 
         ```python
-        from llama_index.llms.databricks import DataBricks
+        from llama_index.llms.databricks import Databricks
 
-        # Set up the DataBricks class with the required model, API key and serving endpoint
-        llm = DataBricks(model="databricks-dbrx-instruct", api_key="your_api_key", api_base="https://[your-work-space].cloud.databricks.com/serving-endpoints/[your-serving-endpoint]")
+        # Set up the Databricks class with the required model, API key and serving endpoint
+        llm = Databricks(model="databricks-dbrx-instruct", api_key="your_api_key", api_base="https://[your-work-space].cloud.databricks.com/serving-endpoints")
 
         # Call the complete method with a query
         response = llm.complete("Explain the importance of open source LLMs")
 
         print(response)
         ```
     """
@@ -27,21 +27,21 @@
         self,
         model: str,
         api_key: Optional[str] = None,
         api_base: Optional[str] = None,
         is_chat_model: bool = True,
         **kwargs: Any,
     ) -> None:
-        api_key = api_key or os.environ.get("DATABRICKS_API_KEY", None)
-        api_base = api_base or os.environ.get("DATABRICKS_API_BASE", None)
+        api_key = api_key or os.environ.get("DATABRICKS_TOKEN", None)
+        api_base = api_base or os.environ.get("DATABRICKS_SERVING_ENDPOINT", None)
         super().__init__(
             model=model,
             api_key=api_key,
             api_base=api_base,
             is_chat_model=is_chat_model,
             **kwargs,
         )
 
     @classmethod
     def class_name(cls) -> str:
         """Get class name."""
-        return "DataBricks"
+        return "Databricks"
```

### Comparing `llama_index_llms_databricks-0.1.0/pyproject.toml` & `llama_index_llms_databricks-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 [tool.poetry]
 authors = ["Abdulaziz Almuhaidib <abdulaziz.almuhaidib.97@gmail.com>"]
 description = "llama-index llms databricks integration"
 license = "MIT"
 name = "llama-index-llms-databricks"
 packages = [{include = "llama_index/"}]
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.0"
 llama-index-llms-openai-like = "^0.1.3"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_llms_databricks-0.1.0/PKG-INFO` & `llama_index_llms_databricks-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-databricks
-Version: 0.1.0
+Version: 0.1.1
 Summary: llama-index llms databricks integration
 License: MIT
 Author: Abdulaziz Almuhaidib
 Author-email: abdulaziz.almuhaidib.97@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,53 +15,53 @@
 Requires-Dist: llama-index-llms-openai-like (>=0.1.3,<0.2.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Llms Integration: Databricks
 
 ## Overview
 
-Integrate with DataBricks LLMs APIs.
+Integrate with Databricks LLMs APIs.
 
 ## Installation
 
 ```bash
 pip install llama-index-llms-databricks
 ```
 
 ## Example
 
 With environmental variables.
 
 ```.env
-DATABRICKS_API_KEY=your_api_key
-DATABRICKS_API_BASE=https://[your-work-space].cloud.databricks.com/serving-endpoints/[your-serving-endpoint]
+DATABRICKS_TOKEN=your_api_key
+DATABRICKS_SERVING_ENDPOINT=https://[your-work-space].cloud.databricks.com/serving-endpoints
 ```
 
 ```python
-from llama_index.llms.databricks import DataBricks
+from llama_index.llms.databricks import Databricks
 
-# Initialize DataBricks LLM without explicitly passing the API key and base
-llm = DataBricks(model="databricks-dbrx-instruct")
+# Initialize Databricks LLM without explicitly passing the API key and base
+llm = Databricks(model="databricks-dbrx-instruct")
 
 # Make a query to the LLM
 response = llm.complete("Explain the importance of open source LLMs")
 
 print(response)
 ```
 
 Without environmental variables
 
 ```python
-from llama_index.llms.databricks import DataBricks
+from llama_index.llms.databricks import Databricks
 
-# Set up the DataBricks class with the required model, API key and serving endpoint
-llm = DataBricks(
+# Set up the Databricks class with the required model, API key and serving endpoint
+llm = Databricks(
     model="databricks-dbrx-instruct",
     api_key="your_api_key",
-    api_base="https://[your-work-space].cloud.databricks.com/serving-endpoints/[your-serving-endpoint]",
+    api_base="https://[your-work-space].cloud.databricks.com/serving-endpoints",
 )
 
 # Call the complete method with a query
 response = llm.complete("Explain the importance of open source LLMs")
 
 print(response)
 ```
```

