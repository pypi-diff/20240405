# Comparing `tmp/langchain_weaviate-0.0.1rc5.tar.gz` & `tmp/langchain_weaviate-0.0.1rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_weaviate-0.0.1rc5.tar", max compression
+gzip compressed data, was "langchain_weaviate-0.0.1rc6.tar", max compression
```

## Comparing `langchain_weaviate-0.0.1rc5.tar` & `langchain_weaviate-0.0.1rc6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2024-01-31 16:37:46.885288 langchain_weaviate-0.0.1rc5/LICENSE
--rw-r--r--   0        0        0      232 2024-01-31 16:37:46.885288 langchain_weaviate-0.0.1rc5/README.md
--rw-r--r--   0        0        0      106 2024-01-31 16:37:46.885288 langchain_weaviate-0.0.1rc5/langchain_weaviate/__init__.py
--rw-r--r--   0        0        0     2061 2024-01-31 16:37:46.885288 langchain_weaviate-0.0.1rc5/langchain_weaviate/_math.py
--rw-r--r--   0        0        0        0 2024-01-31 16:37:46.885288 langchain_weaviate-0.0.1rc5/langchain_weaviate/py.typed
--rw-r--r--   0        0        0     1776 2024-01-31 16:37:46.885288 langchain_weaviate-0.0.1rc5/langchain_weaviate/utils.py
--rw-r--r--   0        0        0    17843 2024-01-31 16:37:46.885288 langchain_weaviate-0.0.1rc5/langchain_weaviate/vectorstores.py
--rw-r--r--   0        0        0     2305 2024-01-31 16:37:46.889288 langchain_weaviate-0.0.1rc5/pyproject.toml
--rw-r--r--   0        0        0      853 1970-01-01 00:00:00.000000 langchain_weaviate-0.0.1rc5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-05 01:22:22.759948 langchain_weaviate-0.0.1rc6/LICENSE
+-rw-r--r--   0        0        0     1770 2024-04-05 01:22:22.759948 langchain_weaviate-0.0.1rc6/README.md
+-rw-r--r--   0        0        0      106 2024-04-05 01:22:22.759948 langchain_weaviate-0.0.1rc6/langchain_weaviate/__init__.py
+-rw-r--r--   0        0        0     2083 2024-04-05 01:22:22.759948 langchain_weaviate-0.0.1rc6/langchain_weaviate/_math.py
+-rw-r--r--   0        0        0        0 2024-04-05 01:22:22.759948 langchain_weaviate-0.0.1rc6/langchain_weaviate/py.typed
+-rw-r--r--   0        0        0     1794 2024-04-05 01:22:22.759948 langchain_weaviate-0.0.1rc6/langchain_weaviate/utils.py
+-rw-r--r--   0        0        0    18248 2024-04-05 01:22:22.759948 langchain_weaviate-0.0.1rc6/langchain_weaviate/vectorstores.py
+-rw-r--r--   0        0        0     2334 2024-04-05 01:22:22.759948 langchain_weaviate-0.0.1rc6/pyproject.toml
+-rw-r--r--   0        0        0     2397 1970-01-01 00:00:00.000000 langchain_weaviate-0.0.1rc6/PKG-INFO
```

### Comparing `langchain_weaviate-0.0.1rc5/LICENSE` & `langchain_weaviate-0.0.1rc6/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 LangChain, Inc.
+Copyright (c) 2024 LangChain, Inc.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `langchain_weaviate-0.0.1rc5/langchain_weaviate/_math.py` & `langchain_weaviate-0.0.1rc6/langchain_weaviate/_math.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Math utils."""
+
 import logging
 from typing import List, Optional, Tuple, Union
 
 import numpy as np
-import simsimd as simd
+import simsimd  # type: ignore
 
 logger = logging.getLogger(__name__)
 
 Matrix = Union[List[List[float]], List[np.ndarray], np.ndarray]
 
 
 def cosine_similarity(X: Matrix, Y: Matrix) -> np.ndarray:
@@ -21,15 +22,15 @@
         raise ValueError(
             f"Number of columns in X and Y must be the same. X has shape {X.shape} "
             f"and Y has shape {Y.shape}."
         )
 
     X = np.array(X, dtype=np.float32)
     Y = np.array(Y, dtype=np.float32)
-    Z = 1 - simd.cdist(X, Y, metric="cosine")
+    Z = 1 - np.array(simsimd.cdist(X, Y, metric="cosine"))
     if isinstance(Z, float):
         return np.array([Z])
     return Z
 
 
 def cosine_similarity_top_k(
     X: Matrix,
```

### Comparing `langchain_weaviate-0.0.1rc5/langchain_weaviate/utils.py` & `langchain_weaviate-0.0.1rc6/langchain_weaviate/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Utility functions for working with vectors and vectorstores."""
 
 from enum import Enum
 from typing import List
 
 import numpy as np
 
-from ._math import cosine_similarity
+from langchain_weaviate._math import cosine_similarity
 
 
 class DistanceStrategy(str, Enum):
     """Enumerator of the Distance strategies for calculating distances
     between vectors."""
 
     EUCLIDEAN_DISTANCE = "EUCLIDEAN_DISTANCE"
```

### Comparing `langchain_weaviate-0.0.1rc5/langchain_weaviate/vectorstores.py` & `langchain_weaviate-0.0.1rc6/langchain_weaviate/vectorstores.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,24 +11,25 @@
     Dict,
     Iterable,
     List,
     Literal,
     Optional,
     Tuple,
     Union,
+    overload,
 )
 from uuid import uuid4
 
 import numpy as np
-import weaviate
+import weaviate  # type: ignore
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
 from langchain_core.vectorstores import VectorStore
 
-from .utils import maximal_marginal_relevance
+from langchain_weaviate.utils import maximal_marginal_relevance
 
 if TYPE_CHECKING:
     import weaviate
 
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
@@ -83,38 +84,36 @@
             weaviate = Weaviate(client, index_name, text_key)
 
     """
 
     def __init__(
         self,
         client: weaviate.WeaviateClient,
-        index_name: str,
+        index_name: Optional[str],
         text_key: str,
         embedding: Optional[Embeddings] = None,
         attributes: Optional[List[str]] = None,
         relevance_score_fn: Optional[
             Callable[[float], float]
         ] = _default_score_normalizer,
-        by_text: bool = True,
         use_multi_tenancy: bool = False,
     ):
         """Initialize with Weaviate client."""
 
         if not isinstance(client, weaviate.WeaviateClient):
             raise ValueError(
-                "client should be an instance of "
-                "weaviate.WeaviateClient, got {type(client)}"
+                "client should be an instance of"
+                f" weaviate.WeaviateClient, got {type(client)}"
             )
         self._client = client
         self._index_name = index_name or f"LangChain_{uuid4().hex}"
         self._embedding = embedding
         self._text_key = text_key
         self._query_attrs = [self._text_key]
         self.relevance_score_fn = relevance_score_fn
-        self._by_text = by_text
         if attributes is not None:
             self._query_attrs.extend(attributes)
 
         schema = _default_schema(self._index_name)
         schema["MultiTenancyConfig"] = {"enabled": use_multi_tenancy}
 
         # check whether the index already exists
@@ -146,30 +145,28 @@
         self,
         texts: Iterable[str],
         metadatas: Optional[List[dict]] = None,
         tenant: Optional[str] = None,
         **kwargs: Any,
     ) -> List[str]:
         """Upload texts with metadata (properties) to Weaviate."""
-        from weaviate.util import get_valid_uuid
+        from weaviate.util import get_valid_uuid  # type: ignore
 
         if tenant and not self._does_tenant_exist(tenant):
             logger.info(
                 f"Tenant {tenant} does not exist in index {self._index_name}. "
                 "Creating tenant."
             )
             tenant_objs = [weaviate.classes.tenants.Tenant(name=tenant)]
             self._collection.tenants.create(tenants=tenant_objs)
 
         ids = []
         embeddings: Optional[List[List[float]]] = None
         if self._embedding:
-            if not isinstance(texts, list):
-                texts = list(texts)
-            embeddings = self._embedding.embed_documents(texts)
+            embeddings = self._embedding.embed_documents(list(texts))
 
         with self._client.batch.dynamic() as batch:
             for i, text in enumerate(texts):
                 data_properties = {self._text_key: text}
                 if metadatas is not None:
                     for key, val in metadatas[i].items():
                         data_properties[key] = _json_serializable(val)
@@ -189,35 +186,59 @@
                     properties=data_properties,
                     uuid=_id,
                     vector=embeddings[i] if embeddings else None,
                     tenant=tenant,
                 )
 
                 ids.append(_id)
+
+        failed_objs = self._client.batch.failed_objects
+        for obj in failed_objs:
+            err_message = (
+                f"Failed to add object: {obj.original_uuid}\nReason: {obj.message}"
+            )
+
+            logger.error(err_message)
+
         return ids
 
+    @overload
     def _perform_search(
         self,
-        query: str,
+        query: Optional[str],
+        k: int,
+        return_score: Literal[False] = False,
+        tenant: Optional[str] = None,
+        **kwargs: Any,
+    ) -> List[Document]: ...
+    @overload
+    def _perform_search(
+        self,
+        query: Optional[str],
         k: int,
-        return_score=False,
-        search_method: Literal["hybrid", "near_vector"] = "hybrid",
+        return_score: Literal[True],
         tenant: Optional[str] = None,
         **kwargs: Any,
-    ) -> List[Union[Document, Tuple[Document, float]]]:
+    ) -> List[Tuple[Document, float]]: ...
+    def _perform_search(
+        self,
+        query: Optional[str],
+        k: int,
+        return_score: bool = False,
+        tenant: Optional[str] = None,
+        **kwargs: Any,
+    ) -> Union[List[Document], List[Tuple[Document, float]]]:
         """
         Perform a similarity search.
 
         Parameters:
         query (str): The query string to search for.
         k (int): The number of results to return.
         return_score (bool, optional): Whether to return the score along with the
           document. Defaults to False.
-        search_method (Literal['hybrid', 'near_vector'], optional): The search method
-          to use. Can be 'hybrid' or 'near_vector'. Defaults to 'hybrid'.
         tenant (Optional[str], optional): The tenant name. Defaults to None.
         **kwargs: Additional parameters to pass to the search method. These parameters
           will be directly passed to the underlying Weaviate client's search method.
 
         Returns:
         List[Union[Document, Tuple[Document, float]]]: A list of documents that match
           the query. If return_score is True, each document is returned as a tuple
@@ -225,54 +246,68 @@
 
         Raises:
         ValueError: If _embedding is None or an invalid search method is provided.
         """
         if self._embedding is None:
             raise ValueError("_embedding cannot be None for similarity_search")
 
-        if "return_metadata" in kwargs and "score" not in kwargs["return_metadata"]:
-            kwargs["return_metadata"].append("score")
-        else:
+        if "return_metadata" not in kwargs:
             kwargs["return_metadata"] = ["score"]
+        elif "score" not in kwargs["return_metadata"]:
+            kwargs["return_metadata"].append("score")
+
+        if (
+            "return_properties" in kwargs
+            and self._text_key not in kwargs["return_properties"]
+        ):
+            kwargs["return_properties"].append(self._text_key)
+
+        vector = kwargs.pop("vector", None)
+
+        # workaround to handle test_max_marginal_relevance_search
+        if vector is None:
+            if query is None:
+                # raise an error because weaviate will do a fetch object query
+                # if both query and vector are None
+                raise ValueError("Either query or vector must be provided.")
+            else:
+                vector = self._embedding.embed_query(query)
+
+        return_uuids = kwargs.pop("return_uuids", False)
 
         with self._tenant_context(tenant) as collection:
             try:
-                if search_method == "hybrid":
-                    embedding = self._embedding.embed_query(query)
-                    result = collection.query.hybrid(
-                        query=query, vector=embedding, limit=k, **kwargs
-                    )
-                elif search_method == "near_vector":
-                    result = collection.query.near_vector(limit=k, **kwargs)
-                else:
-                    raise ValueError(f"Invalid search method: {search_method}")
+                result = collection.query.hybrid(
+                    query=query, vector=vector, limit=k, **kwargs
+                )
             except weaviate.exceptions.WeaviateQueryException as e:
                 raise ValueError(f"Error during query: {e}")
 
-        docs = []
+        docs_and_scores: List[Tuple[Document, float]] = []
         for obj in result.objects:
             text = obj.properties.pop(self._text_key)
             filtered_metadata = {
                 k: v
                 for k, v in obj.metadata.__dict__.items()
                 if v is not None and k != "score"
             }
             merged_props = {
                 **obj.properties,
                 **filtered_metadata,
                 **({"vector": obj.vector["default"]} if obj.vector else {}),
+                **({"uuid": str(obj.uuid)} if return_uuids else {}),
             }
             doc = Document(page_content=text, metadata=merged_props)
-            if not return_score:
-                docs.append(doc)
-            else:
-                score = obj.metadata.score
-                docs.append((doc, score))
+            score = obj.metadata.score
+            docs_and_scores.append((doc, score))
 
-        return docs
+        if return_score:
+            return docs_and_scores
+        else:
+            return [doc for doc, _ in docs_and_scores]
 
     def similarity_search(
         self, query: str, k: int = 4, **kwargs: Any
     ) -> List[Document]:
         """Return docs most similar to query.
 
         Args:
@@ -284,27 +319,14 @@
         Returns:
             List of Documents most similar to the query.
         """
 
         result = self._perform_search(query, k, **kwargs)
         return result
 
-    def similarity_search_by_vector(
-        self, embedding: List[float], k: int = 4, **kwargs: Any
-    ) -> List[Document]:
-        """Look up similar documents by embedding vector in Weaviate."""
-
-        return self._perform_search(
-            query=None,
-            k=k,
-            near_vector=embedding,
-            search_method="near_vector",
-            **kwargs,
-        )
-
     def max_marginal_relevance_search(
         self,
         query: str,
         k: int = 4,
         fetch_k: int = 20,
         lambda_mult: float = 0.5,
         **kwargs: Any,
@@ -363,16 +385,15 @@
             List of Documents selected by maximal marginal relevance.
         """
 
         results = self._perform_search(
             query=None,
             k=fetch_k,
             include_vector=True,
-            near_vector=embedding,
-            search_method="near_vector",
+            vector=embedding,
             **kwargs,
         )
 
         embeddings = [result.metadata["vector"] for result in results]
         mmr_selected = maximal_marginal_relevance(
             np.array(embedding), embeddings, k=k, lambda_mult=lambda_mult
         )
@@ -399,22 +420,21 @@
 
         return results
 
     @classmethod
     def from_texts(
         cls,
         texts: List[str],
-        embedding: Embeddings,
-        client: weaviate.WeaviateClient = None,
+        embedding: Optional[Embeddings],
         metadatas: Optional[List[dict]] = None,
-        tenant: Optional[str] = None,
         *,
+        tenant: Optional[str] = None,
+        client: weaviate.WeaviateClient = None,
         index_name: Optional[str] = None,
         text_key: str = "text",
-        by_text: bool = False,
         relevance_score_fn: Optional[
             Callable[[float], float]
         ] = _default_score_normalizer,
         **kwargs: Any,
     ) -> WeaviateVectorStore:
         """Construct Weaviate wrapper from raw documents.
 
@@ -429,15 +449,14 @@
             texts: Texts to add to vector store.
             embedding: Text embedding model to use.
             client: weaviate.Client to use.
             metadatas: Metadata associated with each text.
             tenant: The tenant name. Defaults to None.
             index_name: Index name.
             text_key: Key to use for uploading/retrieving text to/from vectorstore.
-            by_text: Whether to search by text or by embedding.
             relevance_score_fn: Function for converting whatever distance function the
                 vector store uses to a relevance score, which is a normalized similarity
                 score (0 means dissimilar, 1 means similar).
             **kwargs: Additional named parameters to pass to ``Weaviate.__init__()``.
 
         Example:
             .. code-block:: python
@@ -458,15 +477,14 @@
         weaviate_vector_store = cls(
             client,
             index_name,
             text_key,
             embedding=embedding,
             attributes=attributes,
             relevance_score_fn=relevance_score_fn,
-            by_text=by_text,
             use_multi_tenancy=tenant is not None,
         )
 
         weaviate_vector_store.add_texts(texts, metadatas, tenant=tenant, **kwargs)
 
         return weaviate_vector_store
```

### Comparing `langchain_weaviate-0.0.1rc5/pyproject.toml` & `langchain_weaviate-0.0.1rc6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,79 +1,78 @@
 [tool.poetry]
 name = "langchain-weaviate"
-version = "0.0.1rc5"
+version = "0.0.1rc6"
 description = "An integration package connecting Weaviate and LangChain"
 authors = []
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-langchain-core = ">=0.0.12"
-weaviate-client = {version = "^4.0.0b", allow-prereleases = true}
+langchain-core = "^0.1.33"
+weaviate-client = "^4.0.0"
 numpy = "^1.26.2"
-simsimd = "^3.6.1"
+simsimd = ">=3.6.1,<5.0.0"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.3.0"
+pytest = ">=7.3,<9.0"
 freezegun = "^1.2.2"
-pytest-mock  = "^3.10.0"
+pytest-mock = "^3.10.0"
 syrupy = "^4.0.2"
-pytest-watcher = "^0.3.4"
+pytest-watcher = ">=0.3.4,<0.5.0"
 pytest-asyncio = ">=0.21.1,<0.24.0"
-langchain = "^0.0.352"
+langchain = "^0.1.8"
 pytest-docker = ">=2.0.1,<4.0.0"
 pytest-xdist = "^3.5.0"
 openai = "^1.6.0"
-tiktoken = "^0.5.2"
-pytest-cov = "^4.1.0"
+tiktoken = ">=0.5.2,<0.7.0"
+pytest-cov = ">=4.1,<6.0"
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
 
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
-ruff = "^0.1.5"
+ruff = ">=0.1.5,<0.4.0"
 
 [tool.poetry.group.typing.dependencies]
-mypy = ">=0.991,<1.9"
+mypy = ">=0.991,<1.10"
+types-requests = "^2.31.0.20240403"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.27.1"
 
 [tool.poetry.group.test_integration]
 optional = true
 
 [tool.poetry.group.test_integration.dependencies]
-langchain-openai = ">=0.0.3,<0.1"
+langchain-openai = ">=0.0.3,<0.2"
 
 [tool.ruff]
-select = [
-  "E",  # pycodestyle
-  "F",  # pyflakes
-  "I",  # isort
+lint.select = [
+  "E", # pycodestyle
+  "F", # pyflakes
+  "I", # isort
 ]
 
 [tool.mypy]
 disallow_untyped_defs = "True"
 
 [tool.coverage.run]
-omit = [
-    "tests/*",
-]
+omit = ["tests/*"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 # --strict-markers will raise errors on unknown marks.
```

