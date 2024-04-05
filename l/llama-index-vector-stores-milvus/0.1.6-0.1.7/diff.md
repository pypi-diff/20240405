# Comparing `tmp/llama_index_vector_stores_milvus-0.1.6.tar.gz` & `tmp/llama_index_vector_stores_milvus-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_milvus-0.1.6.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_milvus-0.1.7.tar", max compression
```

## Comparing `llama_index_vector_stores_milvus-0.1.6.tar` & `llama_index_vector_stores_milvus-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       47 2024-03-07 18:58:55.558529 llama_index_vector_stores_milvus-0.1.6/README.md
--rw-r--r--   0        0        0      101 2024-03-07 18:58:55.562529 llama_index_vector_stores_milvus-0.1.6/llama_index/vector_stores/milvus/__init__.py
--rw-r--r--   0        0        0    13175 2024-03-07 18:58:55.562529 llama_index_vector_stores_milvus-0.1.6/llama_index/vector_stores/milvus/base.py
--rw-r--r--   0        0        0     1479 2024-03-07 18:58:55.562529 llama_index_vector_stores_milvus-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 llama_index_vector_stores_milvus-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       47 2024-04-05 16:01:31.267661 llama_index_vector_stores_milvus-0.1.7/README.md
+-rw-r--r--   0        0        0      101 2024-04-05 16:01:31.267661 llama_index_vector_stores_milvus-0.1.7/llama_index/vector_stores/milvus/__init__.py
+-rw-r--r--   0        0        0    13737 2024-04-05 16:01:31.267661 llama_index_vector_stores_milvus-0.1.7/llama_index/vector_stores/milvus/base.py
+-rw-r--r--   0        0        0     1479 2024-04-05 16:01:31.267661 llama_index_vector_stores_milvus-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 llama_index_vector_stores_milvus-0.1.7/PKG-INFO
```

### Comparing `llama_index_vector_stores_milvus-0.1.6/llama_index/vector_stores/milvus/base.py` & `llama_index_vector_stores_milvus-0.1.7/llama_index/vector_stores/milvus/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Milvus vector store index.
 
 An index that is built within Milvus.
 
 """
+
 import logging
 from typing import Any, Dict, List, Optional, Union
 
 import pymilvus  # noqa
 from llama_index.core.bridge.pydantic import PrivateAttr
 from llama_index.core.schema import BaseNode, TextNode
 from llama_index.core.vector_stores.types import (
@@ -79,14 +80,30 @@
     Raises:
         ImportError: Unable to import `pymilvus`.
         MilvusException: Error communicating with Milvus, more can be found in logging
             under Debug.
 
     Returns:
         MilvusVectorstore: Vectorstore that supports add, delete, and query.
+
+    Examples:
+        `pip install llama-index-vector-stores-milvus`
+
+        ```python
+        from llama_index.vector_stores.milvus import MilvusVectorStore
+
+        # Setup MilvusVectorStore
+        vector_store = MilvusVectorStore(
+            dim=1536,
+            collection_name="your_collection_name",
+            uri="http://milvus_address:port",
+            token="your_milvus_token_here",
+            overwrite=True
+        )
+        ```
     """
 
     stores_text: bool = True
     stores_node: bool = True
 
     uri: str = "http://localhost:19530"
     token: str = ""
@@ -130,16 +147,23 @@
             overwrite=overwrite,
             text_key=text_key,
             index_config=index_config if index_config else {},
             search_config=search_config if search_config else {},
         )
 
         # Select the similarity metric
-        similarity_metrics_map = {"ip": "IP", "l2": "L2", "euclidean": "L2"}
-        similarity_metric = similarity_metrics_map.get(similarity_metric.lower(), "L2")
+        similarity_metrics_map = {
+            "ip": "IP",
+            "l2": "L2",
+            "euclidean": "L2",
+            "cosine": "COSINE",
+        }
+        self.similarity_metric = similarity_metrics_map.get(
+            similarity_metric.lower(), "L2"
+        )
 
         # Connect to Milvus instance
         self._milvusclient = MilvusClient(
             uri=uri,
             token=token,
             **kwargs,  # pass additional arguments such as server_pem_path
         )
@@ -153,15 +177,15 @@
                 raise ValueError("Dim argument required for collection creation.")
             self._milvusclient.create_collection(
                 collection_name=collection_name,
                 dimension=dim,
                 primary_field_name=MILVUS_ID_FIELD,
                 vector_field_name=embedding_field,
                 id_type="string",
-                metric_type=similarity_metric,
+                metric_type=self.similarity_metric,
                 max_length=65_535,
                 consistency_level=consistency_level,
             )
 
         self._collection = Collection(collection_name, using=self._milvusclient._using)
         self._create_index_if_required()
```

### Comparing `llama_index_vector_stores_milvus-0.1.6/pyproject.toml` & `llama_index_vector_stores_milvus-0.1.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores milvus integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-milvus"
 readme = "README.md"
-version = "0.1.6"
+version = "0.1.7"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 pymilvus = "^2.3.6"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_vector_stores_milvus-0.1.6/PKG-INFO` & `llama_index_vector_stores_milvus-0.1.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-milvus
-Version: 0.1.6
+Version: 0.1.7
 Summary: llama-index vector_stores milvus integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

