# Comparing `tmp/llama_index_packs_dense_x_retrieval-0.1.3.tar.gz` & `tmp/llama_index_packs_dense_x_retrieval-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_packs_dense_x_retrieval-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_packs_dense_x_retrieval-0.1.4.tar", max compression
```

## Comparing `llama_index_packs_dense_x_retrieval-0.1.3.tar` & `llama_index_packs_dense_x_retrieval-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2062 2024-02-20 18:45:10.380662 llama_index_packs_dense_x_retrieval-0.1.3/README.md
--rw-r--r--   0        0        0      108 2024-02-13 13:53:02.169719 llama_index_packs_dense_x_retrieval-0.1.3/llama_index/packs/dense_x_retrieval/__init__.py
--rw-r--r--   0        0        0     7711 2024-02-13 13:53:02.169792 llama_index_packs_dense_x_retrieval-0.1.3/llama_index/packs/dense_x_retrieval/base.py
--rw-r--r--   0        0        0     1507 2024-02-22 01:11:42.516463 llama_index_packs_dense_x_retrieval-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2712 1970-01-01 00:00:00.000000 llama_index_packs_dense_x_retrieval-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2357 2024-04-05 18:28:37.275460 llama_index_packs_dense_x_retrieval-0.1.4/README.md
+-rw-r--r--   0        0        0      108 2024-04-05 18:28:37.275460 llama_index_packs_dense_x_retrieval-0.1.4/llama_index/packs/dense_x_retrieval/__init__.py
+-rw-r--r--   0        0        0     7790 2024-04-05 18:28:37.275460 llama_index_packs_dense_x_retrieval-0.1.4/llama_index/packs/dense_x_retrieval/base.py
+-rw-r--r--   0        0        0     1507 2024-04-05 18:28:37.275460 llama_index_packs_dense_x_retrieval-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2956 1970-01-01 00:00:00.000000 llama_index_packs_dense_x_retrieval-0.1.4/PKG-INFO
```

### Comparing `llama_index_packs_dense_x_retrieval-0.1.3/README.md` & `llama_index_packs_dense_x_retrieval-0.1.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -25,30 +25,43 @@
 You can then inspect the files at `./dense_pack` and use them as a template for your own project!
 
 ## Code Usage
 
 You can download the pack to a the `./dense_pack` directory:
 
 ```python
-from llama_index import SimpleDirectoryReader
+from llama_index.core import SimpleDirectoryReader
 from llama_index.core.llama_pack import download_llama_pack
 
 # download and install dependencies
 DenseXRetrievalPack = download_llama_pack(
     "DenseXRetrievalPack", "./dense_pack"
 )
 
 documents = SimpleDirectoryReader("./data").load_data()
 
 # uses the LLM to extract propositions from every document/node!
 dense_pack = DenseXRetrievalPack(documents)
+
+# for streaming
+dense_pack = DenseXRetrievalPack(documents, streaming=True)
 ```
 
 The `run()` function is a light wrapper around `query_engine.query()`.
 
 ```python
 response = dense_pack.run("What can you tell me about LLMs?")
 
 print(response)
 ```
 
+for streaming:
+
+The `run()` function is a light wrapper around `query_engine.query()`.
+
+```python
+stream_response = dense_pack.run("What can you tell me about LLMs?")
+
+stream_response.print_response_stream()
+```
+
 See the [notebook on llama-hub](https://github.com/run-llama/llama-hub/blob/main/llama_hub/llama_packs/dense_x_retrieval/dense_x_retrieval.ipynb) for a full example.
```

### Comparing `llama_index_packs_dense_x_retrieval-0.1.3/llama_index/packs/dense_x_retrieval/base.py` & `llama_index_packs_dense_x_retrieval-0.1.4/llama_index/packs/dense_x_retrieval/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,15 @@
         self,
         documents: List[Document],
         proposition_llm: Optional[LLM] = None,
         query_llm: Optional[LLM] = None,
         embed_model: Optional[BaseEmbedding] = None,
         text_splitter: TextSplitter = SentenceSplitter(),
         similarity_top_k: int = 4,
+        streaming: bool = False,
     ) -> None:
         """Init params."""
         self._proposition_llm = proposition_llm or OpenAI(
             model="gpt-3.5-turbo",
             temperature=0.1,
             max_tokens=750,
         )
@@ -108,15 +109,17 @@
                     similarity_top_k=similarity_top_k
                 )
             },
             node_dict=all_nodes_dict,
         )
 
         self.query_engine = RetrieverQueryEngine.from_args(
-            self.retriever, service_context=service_context
+            self.retriever,
+            service_context=service_context,
+            streaming=streaming,
         )
 
     async def _aget_proposition(self, node: TextNode) -> List[TextNode]:
         """Get proposition."""
         inital_output = await self._proposition_llm.apredict(
             PROPOSITIONS_PROMPT, node_text=node.text
         )
```

### Comparing `llama_index_packs_dense_x_retrieval-0.1.3/pyproject.toml` & `llama_index_packs_dense_x_retrieval-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 authors = ["Your Name <you@example.com>"]
 description = "llama-index packs dense_x_retrieval integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 maintainers = ["logan-markewich"]
 name = "llama-index-packs-dense-x-retrieval"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
```

### Comparing `llama_index_packs_dense_x_retrieval-0.1.3/PKG-INFO` & `llama_index_packs_dense_x_retrieval-0.1.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: llama-index-packs-dense-x-retrieval
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index packs dense_x_retrieval integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Maintainer: logan-markewich
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Description-Content-Type: text/markdown
 
 # Dense-X-Retrieval Pack
 
 This LlamaPack creates a query engine that uses a `RecursiveRetriever` in llama-index to fetch nodes based on propoistions extracted from each node.
 
@@ -43,31 +42,44 @@
 You can then inspect the files at `./dense_pack` and use them as a template for your own project!
 
 ## Code Usage
 
 You can download the pack to a the `./dense_pack` directory:
 
 ```python
-from llama_index import SimpleDirectoryReader
+from llama_index.core import SimpleDirectoryReader
 from llama_index.core.llama_pack import download_llama_pack
 
 # download and install dependencies
 DenseXRetrievalPack = download_llama_pack(
     "DenseXRetrievalPack", "./dense_pack"
 )
 
 documents = SimpleDirectoryReader("./data").load_data()
 
 # uses the LLM to extract propositions from every document/node!
 dense_pack = DenseXRetrievalPack(documents)
+
+# for streaming
+dense_pack = DenseXRetrievalPack(documents, streaming=True)
 ```
 
 The `run()` function is a light wrapper around `query_engine.query()`.
 
 ```python
 response = dense_pack.run("What can you tell me about LLMs?")
 
 print(response)
 ```
 
+for streaming:
+
+The `run()` function is a light wrapper around `query_engine.query()`.
+
+```python
+stream_response = dense_pack.run("What can you tell me about LLMs?")
+
+stream_response.print_response_stream()
+```
+
 See the [notebook on llama-hub](https://github.com/run-llama/llama-hub/blob/main/llama_hub/llama_packs/dense_x_retrieval/dense_x_retrieval.ipynb) for a full example.
```

