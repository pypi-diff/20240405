# Comparing `tmp/langchain_nvidia_ai_endpoints-0.0.5.tar.gz` & `tmp/langchain_nvidia_ai_endpoints-0.0.5rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_nvidia_ai_endpoints-0.0.5.tar", max compression
+gzip compressed data, was "langchain_nvidia_ai_endpoints-0.0.5rc0.tar", max compression
```

## Comparing `langchain_nvidia_ai_endpoints-0.0.5.tar` & `langchain_nvidia_ai_endpoints-0.0.5rc0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1072 2024-04-05 17:32:17.736984 langchain_nvidia_ai_endpoints-0.0.5/LICENSE
--rw-r--r--   0        0        0    10720 2024-04-05 17:32:17.736984 langchain_nvidia_ai_endpoints-0.0.5/README.md
--rw-r--r--   0        0        0     2070 2024-04-05 17:32:17.744984 langchain_nvidia_ai_endpoints-0.0.5/langchain_nvidia_ai_endpoints/__init__.py
--rw-r--r--   0        0        0    29740 2024-04-05 17:32:17.744984 langchain_nvidia_ai_endpoints-0.0.5/langchain_nvidia_ai_endpoints/_common.py
--rw-r--r--   0        0        0     5358 2024-04-05 17:32:17.744984 langchain_nvidia_ai_endpoints-0.0.5/langchain_nvidia_ai_endpoints/_statics.py
--rw-r--r--   0        0        0    10149 2024-04-05 17:32:17.744984 langchain_nvidia_ai_endpoints-0.0.5/langchain_nvidia_ai_endpoints/callbacks.py
--rw-r--r--   0        0        0    15758 2024-04-05 17:32:17.744984 langchain_nvidia_ai_endpoints-0.0.5/langchain_nvidia_ai_endpoints/chat_models.py
--rw-r--r--   0        0        0     4955 2024-04-05 17:32:17.744984 langchain_nvidia_ai_endpoints-0.0.5/langchain_nvidia_ai_endpoints/embeddings.py
--rw-r--r--   0        0        0     5735 2024-04-05 17:32:17.744984 langchain_nvidia_ai_endpoints-0.0.5/langchain_nvidia_ai_endpoints/image_gen.py
--rw-r--r--   0        0        0     7597 2024-04-05 17:32:17.744984 langchain_nvidia_ai_endpoints-0.0.5/langchain_nvidia_ai_endpoints/llm.py
--rw-r--r--   0        0        0        0 2024-04-05 17:32:17.744984 langchain_nvidia_ai_endpoints-0.0.5/langchain_nvidia_ai_endpoints/py.typed
--rw-r--r--   0        0        0    10047 2024-04-05 17:32:17.744984 langchain_nvidia_ai_endpoints-0.0.5/langchain_nvidia_ai_endpoints/tools.py
--rw-r--r--   0        0        0     2669 2024-04-05 17:32:17.744984 langchain_nvidia_ai_endpoints-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    11619 1970-01-01 00:00:00.000000 langchain_nvidia_ai_endpoints-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-02 14:19:37.310745 langchain_nvidia_ai_endpoints-0.0.5rc0/LICENSE
+-rw-r--r--   0        0        0    10720 2024-04-02 14:19:37.310745 langchain_nvidia_ai_endpoints-0.0.5rc0/README.md
+-rw-r--r--   0        0        0     2070 2024-04-02 14:19:37.314746 langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/__init__.py
+-rw-r--r--   0        0        0    29698 2024-04-02 14:19:37.314746 langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/_common.py
+-rw-r--r--   0        0        0     5358 2024-04-02 14:19:37.314746 langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/_statics.py
+-rw-r--r--   0        0        0    10149 2024-04-02 14:19:37.314746 langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/callbacks.py
+-rw-r--r--   0        0        0    15746 2024-04-02 14:19:37.314746 langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/chat_models.py
+-rw-r--r--   0        0        0     4895 2024-04-02 14:19:37.314746 langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/embeddings.py
+-rw-r--r--   0        0        0     5735 2024-04-02 14:19:37.314746 langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/image_gen.py
+-rw-r--r--   0        0        0     7597 2024-04-02 14:19:37.314746 langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/llm.py
+-rw-r--r--   0        0        0        0 2024-04-02 14:19:37.314746 langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/py.typed
+-rw-r--r--   0        0        0    10047 2024-04-02 14:19:37.314746 langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/tools.py
+-rw-r--r--   0        0        0     2673 2024-04-02 14:19:37.318745 langchain_nvidia_ai_endpoints-0.0.5rc0/pyproject.toml
+-rw-r--r--   0        0        0    11622 1970-01-01 00:00:00.000000 langchain_nvidia_ai_endpoints-0.0.5rc0/PKG-INFO
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.5/LICENSE` & `langchain_nvidia_ai_endpoints-0.0.5rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.5/README.md` & `langchain_nvidia_ai_endpoints-0.0.5rc0/README.md`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.5/langchain_nvidia_ai_endpoints/__init__.py` & `langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.5/langchain_nvidia_ai_endpoints/_common.py` & `langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,15 +289,14 @@
                 if "detail" in rd:
                     body += f"{rd['detail']}\n"
                 body += "RequestID: " + rd["requestId"]
             else:
                 body = rd.get("detail", rd)
             if str(status) == "401":
                 body += "\nPlease check or regenerate your API key."
-            # todo: raise as an HTTPError
             raise Exception(f"{header}\n{body}") from None
 
     ####################################################################################
     ## Simple query interface to show the set of model options
 
     def query(
         self,
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.5/langchain_nvidia_ai_endpoints/_statics.py` & `langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/_statics.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.5/langchain_nvidia_ai_endpoints/callbacks.py` & `langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/callbacks.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.5/langchain_nvidia_ai_endpoints/chat_models.py` & `langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/chat_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
             from langchain_nvidia_ai_endpoints import ChatNVIDIA
 
 
             model = ChatNVIDIA(model="llama2_13b")
             response = model.invoke("Hello")
     """
 
-    _default_model: str = "ai-mixtral-8x7b-instruct"
+    _default_model: str = "mixtral_8x7b"
     infer_endpoint: str = Field("{base_url}/chat/completions")
     model: str = Field(_default_model, description="Name of the model to invoke")
     temperature: Optional[float] = Field(description="Sampling temperature in [0, 1]")
     max_tokens: Optional[int] = Field(description="Maximum # of tokens to generate")
     top_p: Optional[float] = Field(description="Top-p for distribution sampling")
     seed: Optional[int] = Field(description="The seed for deterministic results")
     bad: Optional[Sequence[str]] = Field(description="Bad words to avoid (cased)")
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.5/langchain_nvidia_ai_endpoints/embeddings.py` & `langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/embeddings.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,19 @@
 
 from ._statics import MODEL_SPECS
 
 
 class NVIDIAEmbeddings(_NVIDIAClient, Embeddings):
     """NVIDIA's AI Foundation Retriever Question-Answering Asymmetric Model."""
 
-    _default_model: str = "ai-embed-qa-4"
-    _default_max_batch_size: int = 50
+    _default_model: str = "nvolveqa_40k"
     infer_endpoint: str = Field("{base_url}/embeddings")
     model: str = Field(_default_model, description="Name of the model to invoke")
     max_length: int = Field(2048, ge=1, le=2048)
-    max_batch_size: int = Field(default=_default_max_batch_size)
+    max_batch_size: int = Field(default=50)
     model_type: Optional[Literal["passage", "query"]] = Field(
         None, description="The type of text to be embedded."
     )
 
     def _embed(
         self, texts: List[str], model_type: Literal["passage", "query"]
     ) -> List[List[float]]:
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.5/langchain_nvidia_ai_endpoints/image_gen.py` & `langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/image_gen.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.5/langchain_nvidia_ai_endpoints/llm.py` & `langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/llm.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.5/langchain_nvidia_ai_endpoints/tools.py` & `langchain_nvidia_ai_endpoints-0.0.5rc0/langchain_nvidia_ai_endpoints/tools.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.5/pyproject.toml` & `langchain_nvidia_ai_endpoints-0.0.5rc0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-nvidia-ai-endpoints"
-version = "0.0.5"
+version = "0.0.5-rc0"
 description = "An integration package connecting NVIDIA AI Endpoints and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.5/PKG-INFO` & `langchain_nvidia_ai_endpoints-0.0.5rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-nvidia-ai-endpoints
-Version: 0.0.5
+Version: 0.0.5rc0
 Summary: An integration package connecting NVIDIA AI Endpoints and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

