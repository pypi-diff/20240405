# Comparing `tmp/llama_index_finetuning-0.1.4.tar.gz` & `tmp/llama_index_finetuning-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_finetuning-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_finetuning-0.1.5.tar", max compression
```

## Comparing `llama_index_finetuning-0.1.4.tar` & `llama_index_finetuning-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      156 2024-02-13 13:53:01.578174 llama_index_finetuning-0.1.4/README.md
--rw-r--r--   0        0        0     1012 2024-02-13 13:53:01.578347 llama_index_finetuning-0.1.4/llama_index/finetuning/__init__.py
--rw-r--r--   0        0        0      188 2024-02-13 13:53:01.578480 llama_index_finetuning-0.1.4/llama_index/finetuning/callbacks/__init__.py
--rw-r--r--   0        0        0     7574 2024-02-20 22:37:41.272297 llama_index_finetuning-0.1.4/llama_index/finetuning/callbacks/finetuning_handler.py
--rw-r--r--   0        0        0      161 2024-02-13 13:53:01.578688 llama_index_finetuning-0.1.4/llama_index/finetuning/cross_encoders/__init__.py
--rw-r--r--   0        0        0     4797 2024-02-13 13:53:01.578760 llama_index_finetuning-0.1.4/llama_index/finetuning/cross_encoders/cross_encoder.py
--rw-r--r--   0        0        0     9431 2024-02-13 13:53:01.578848 llama_index_finetuning-0.1.4/llama_index/finetuning/cross_encoders/dataset_gen.py
--rw-r--r--   0        0        0      299 2024-02-13 13:53:01.578978 llama_index_finetuning-0.1.4/llama_index/finetuning/embeddings/__init__.py
--rw-r--r--   0        0        0     6400 2024-02-16 04:21:21.875871 llama_index_finetuning-0.1.4/llama_index/finetuning/embeddings/adapter.py
--rw-r--r--   0        0        0     5008 2024-02-16 04:21:21.875997 llama_index_finetuning-0.1.4/llama_index/finetuning/embeddings/adapter_utils.py
--rw-r--r--   0        0        0     3127 2024-02-13 13:53:01.579171 llama_index_finetuning-0.1.4/llama_index/finetuning/embeddings/common.py
--rw-r--r--   0        0        0     3353 2024-02-13 13:53:01.579237 llama_index_finetuning-0.1.4/llama_index/finetuning/embeddings/sentence_transformer.py
--rw-r--r--   0        0        0      110 2024-02-13 13:53:01.579366 llama_index_finetuning-0.1.4/llama_index/finetuning/gradient/__init__.py
--rw-r--r--   0        0        0     4946 2024-02-13 13:53:01.579439 llama_index_finetuning-0.1.4/llama_index/finetuning/gradient/base.py
--rw-r--r--   0        0        0      123 2024-02-13 13:53:01.579576 llama_index_finetuning-0.1.4/llama_index/finetuning/openai/__init__.py
--rw-r--r--   0        0        0     3880 2024-02-13 13:53:01.579630 llama_index_finetuning-0.1.4/llama_index/finetuning/openai/base.py
--rw-r--r--   0        0        0     6562 2024-02-13 13:53:01.579692 llama_index_finetuning-0.1.4/llama_index/finetuning/openai/validate_json.py
--rw-r--r--   0        0        0      282 2024-02-13 13:53:01.579822 llama_index_finetuning-0.1.4/llama_index/finetuning/rerankers/__init__.py
--rw-r--r--   0        0        0     2753 2024-02-13 13:53:01.579880 llama_index_finetuning-0.1.4/llama_index/finetuning/rerankers/cohere_reranker.py
--rw-r--r--   0        0        0     4700 2024-02-13 13:53:01.579941 llama_index_finetuning-0.1.4/llama_index/finetuning/rerankers/dataset_gen.py
--rw-r--r--   0        0        0     1618 2024-02-13 13:53:01.580006 llama_index_finetuning-0.1.4/llama_index/finetuning/types.py
--rw-r--r--   0        0        0     1830 2024-02-22 03:30:22.578374 llama_index_finetuning-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1050 1970-01-01 00:00:00.000000 llama_index_finetuning-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      156 2024-04-04 22:08:09.061314 llama_index_finetuning-0.1.5/README.md
+-rw-r--r--   0        0        0     1012 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/__init__.py
+-rw-r--r--   0        0        0      188 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/callbacks/__init__.py
+-rw-r--r--   0        0        0     7574 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/callbacks/finetuning_handler.py
+-rw-r--r--   0        0        0      161 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/cross_encoders/__init__.py
+-rw-r--r--   0        0        0     4797 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/cross_encoders/cross_encoder.py
+-rw-r--r--   0        0        0     9431 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/cross_encoders/dataset_gen.py
+-rw-r--r--   0        0        0      299 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/embeddings/__init__.py
+-rw-r--r--   0        0        0     6400 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/embeddings/adapter.py
+-rw-r--r--   0        0        0     5008 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/embeddings/adapter_utils.py
+-rw-r--r--   0        0        0     3126 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/embeddings/common.py
+-rw-r--r--   0        0        0     3353 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/embeddings/sentence_transformer.py
+-rw-r--r--   0        0        0      110 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/gradient/__init__.py
+-rw-r--r--   0        0        0     4946 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/gradient/base.py
+-rw-r--r--   0        0        0      123 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/openai/__init__.py
+-rw-r--r--   0        0        0     3880 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/openai/base.py
+-rw-r--r--   0        0        0     6562 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/openai/validate_json.py
+-rw-r--r--   0        0        0      282 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/rerankers/__init__.py
+-rw-r--r--   0        0        0     2753 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/rerankers/cohere_reranker.py
+-rw-r--r--   0        0        0     4700 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/rerankers/dataset_gen.py
+-rw-r--r--   0        0        0     1618 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/llama_index/finetuning/types.py
+-rw-r--r--   0        0        0     1830 2024-04-04 22:08:09.065314 llama_index_finetuning-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      999 1970-01-01 00:00:00.000000 llama_index_finetuning-0.1.5/PKG-INFO
```

### Comparing `llama_index_finetuning-0.1.4/llama_index/finetuning/__init__.py` & `llama_index_finetuning-0.1.5/llama_index/finetuning/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_finetuning-0.1.4/llama_index/finetuning/callbacks/finetuning_handler.py` & `llama_index_finetuning-0.1.5/llama_index/finetuning/callbacks/finetuning_handler.py`

 * *Files identical despite different names*

### Comparing `llama_index_finetuning-0.1.4/llama_index/finetuning/cross_encoders/cross_encoder.py` & `llama_index_finetuning-0.1.5/llama_index/finetuning/cross_encoders/cross_encoder.py`

 * *Files identical despite different names*

### Comparing `llama_index_finetuning-0.1.4/llama_index/finetuning/cross_encoders/dataset_gen.py` & `llama_index_finetuning-0.1.5/llama_index/finetuning/cross_encoders/dataset_gen.py`

 * *Files identical despite different names*

### Comparing `llama_index_finetuning-0.1.4/llama_index/finetuning/embeddings/adapter.py` & `llama_index_finetuning-0.1.5/llama_index/finetuning/embeddings/adapter.py`

 * *Files identical despite different names*

### Comparing `llama_index_finetuning-0.1.4/llama_index/finetuning/embeddings/adapter_utils.py` & `llama_index_finetuning-0.1.5/llama_index/finetuning/embeddings/adapter_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_finetuning-0.1.4/llama_index/finetuning/embeddings/common.py` & `llama_index_finetuning-0.1.5/llama_index/finetuning/embeddings/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 DEFAULT_QA_GENERATE_PROMPT_TMPL = """\
 Context information is below.
 
 ---------------------
 {context_str}
 ---------------------
 
-Given the context information and not prior knowledge.
+Given the context information and no prior knowledge.
 generate only questions based on the below query.
 
 You are a Teacher/ Professor. Your task is to setup \
 {num_questions_per_chunk} questions for an upcoming \
 quiz/examination. The questions should be diverse in nature \
 across the document. Restrict the questions to the \
 context information provided."
```

### Comparing `llama_index_finetuning-0.1.4/llama_index/finetuning/embeddings/sentence_transformer.py` & `llama_index_finetuning-0.1.5/llama_index/finetuning/embeddings/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `llama_index_finetuning-0.1.4/llama_index/finetuning/gradient/base.py` & `llama_index_finetuning-0.1.5/llama_index/finetuning/gradient/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_finetuning-0.1.4/llama_index/finetuning/openai/base.py` & `llama_index_finetuning-0.1.5/llama_index/finetuning/openai/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_finetuning-0.1.4/llama_index/finetuning/openai/validate_json.py` & `llama_index_finetuning-0.1.5/llama_index/finetuning/openai/validate_json.py`

 * *Files identical despite different names*

### Comparing `llama_index_finetuning-0.1.4/llama_index/finetuning/rerankers/cohere_reranker.py` & `llama_index_finetuning-0.1.5/llama_index/finetuning/rerankers/cohere_reranker.py`

 * *Files identical despite different names*

### Comparing `llama_index_finetuning-0.1.4/llama_index/finetuning/rerankers/dataset_gen.py` & `llama_index_finetuning-0.1.5/llama_index/finetuning/rerankers/dataset_gen.py`

 * *Files identical despite different names*

### Comparing `llama_index_finetuning-0.1.4/llama_index/finetuning/types.py` & `llama_index_finetuning-0.1.5/llama_index/finetuning/types.py`

 * *Files identical despite different names*

### Comparing `llama_index_finetuning-0.1.4/pyproject.toml` & `llama_index_finetuning-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 exclude = ["_static", "build", "examples", "notebooks", "venv"]
 ignore_missing_imports = true
 python_version = "3.8"
 
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index finetuning"
+exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-finetuning"
 readme = "README.md"
-version = "0.1.4"
-exclude = ["**/BUILD"]
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.11.post1"
 llama-index-llms-openai = "^0.1.1"
 llama-index-llms-gradient = "^0.1.1"
 llama-index-postprocessor-cohere-rerank = "^0.1.1"
```

### Comparing `llama_index_finetuning-0.1.4/PKG-INFO` & `llama_index_finetuning-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: llama-index-finetuning
-Version: 0.1.4
+Version: 0.1.5
 Summary: llama-index finetuning
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.11.post1,<0.11.0)
 Requires-Dist: llama-index-embeddings-adapter (>=0.1.2,<0.2.0)
 Requires-Dist: llama-index-llms-gradient (>=0.1.1,<0.2.0)
 Requires-Dist: llama-index-llms-openai (>=0.1.1,<0.2.0)
 Requires-Dist: llama-index-postprocessor-cohere-rerank (>=0.1.1,<0.2.0)
 Requires-Dist: sentence-transformers (>=2.3.0,<3.0.0)
 Description-Content-Type: text/markdown
```

