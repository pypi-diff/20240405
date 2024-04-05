# Comparing `tmp/langfuse_haystack-0.0.1.tar.gz` & `tmp/langfuse_haystack-0.0.2.tar.gz`

## Comparing `langfuse_haystack-0.0.1.tar` & `langfuse_haystack-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.1/example/basic_rag.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.1/example/requirements.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.1/src/haystack_integrations/components/others/langfuse/__about__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.1/src/haystack_integrations/components/others/langfuse/__init__.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.1/src/haystack_integrations/components/others/langfuse/langfuse.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.1/src/haystack_integrations/tracing/langfuse/__init__.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.1/src/haystack_integrations/tracing/langfuse/tracer.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.1/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.1/README.md
--rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.2/example/basic_rag.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.2/example/requirements.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.2/src/haystack_integrations/components/others/langfuse/__about__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.2/src/haystack_integrations/components/others/langfuse/__init__.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.2/src/haystack_integrations/components/others/langfuse/langfuse.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.2/src/haystack_integrations/tracing/langfuse/__init__.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.2/src/haystack_integrations/tracing/langfuse/tracer.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.2/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.2/README.md
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.2/PKG-INFO
```

### Comparing `langfuse_haystack-0.0.1/example/basic_rag.py` & `langfuse_haystack-0.0.2/example/basic_rag.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     # Add components to your pipeline
     basic_rag_pipeline.add_component("tracer", LangfuseComponent("Basic RAG Pipeline"))
     basic_rag_pipeline.add_component(
         "text_embedder", SentenceTransformersTextEmbedder(model="sentence-transformers/all-MiniLM-L6-v2")
     )
     basic_rag_pipeline.add_component("retriever", retriever)
     basic_rag_pipeline.add_component("prompt_builder", prompt_builder)
-    basic_rag_pipeline.add_component("llm", OpenAIGenerator(model="gpt-3.5-turbo"))
+    basic_rag_pipeline.add_component("llm", OpenAIGenerator(model="gpt-3.5-turbo", generation_kwargs={"n": 2}))
 
     # Now, connect the components to each other
     # NOTE: the tracer component doesn't need to be connected to anything in order to work
     basic_rag_pipeline.connect("text_embedder.embedding", "retriever.query_embedding")
     basic_rag_pipeline.connect("retriever", "prompt_builder.documents")
     basic_rag_pipeline.connect("prompt_builder", "llm")
```

### Comparing `langfuse_haystack-0.0.1/src/haystack_integrations/tracing/langfuse/tracer.py` & `langfuse_haystack-0.0.2/src/haystack_integrations/tracing/langfuse/tracer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 import contextlib
 from typing import Any, Dict, Iterator, Optional, Union
 
-from haystack.lazy_imports import LazyImport
 from haystack.tracing import Span, Tracer, tracer
 from haystack.tracing import utils as tracing_utils
 
 import langfuse
 
 
 class LangfuseSpan(Span):
     def __init__(self, span: "Union[langfuse.client.StatefulSpanClient, langfuse.client.StatefulTraceClient]") -> None:
         self._span = span
+        # locally cache tags
+        self._data = {}
 
     def set_tag(self, key: str, value: Any) -> None:
         coerced_value = tracing_utils.coerce_tag_value(value)
         self._span.update(metadata={key: coerced_value})
+        self._data[key] = value
 
     def set_content_tag(self, key: str, value: Any) -> None:
         if not tracer.is_content_tracing_enabled:
             return
 
         if key.endswith(".input"):
             self._span.update(input=value)
         elif key.endswith(".output"):
             self._span.update(output=value)
 
+        self._data[key] = value
+
     def raw_span(self) -> Any:
         return self._span
 
     def get_correlation_data_for_logs(self) -> Dict[str, Any]:
         return {}
 
 
@@ -38,25 +42,35 @@
         self._context: list[LangfuseSpan] = []
         self._name = name
 
     @contextlib.contextmanager
     def trace(self, operation_name: str, tags: Optional[Dict[str, Any]] = None) -> Iterator[Span]:
         tags = tags or {}
         span_name = tags.get("haystack.component.name", operation_name)
+        is_generation = False
 
         if tags.get("haystack.component.type") in ["OpenAIGenerator"]:
             span = LangfuseSpan(self.current_span().raw_span().generation(name=span_name))
+            is_generation = True
         else:
             span = LangfuseSpan(self.current_span().raw_span().span(name=span_name))
 
         self._context.append(span)
         span.set_tags(tags)
 
         yield span
 
+        if is_generation:
+            meta = span._data.get("haystack.component.output", {}).get("meta")
+            if meta:
+                # Haystack returns one meta dict for each message, but the 'usage' value
+                # is always the same, let's just pick the first item
+                m = meta[0]
+                span._span.update(usage=m.get("usage"), model=m.get("model"))
+
         span.raw_span().end()
         self._context.pop()
         self._tracer.flush()
 
     def current_span(self) -> Span:
         if not self._context:
             # The root span has to be a trace
```

### Comparing `langfuse_haystack-0.0.1/.gitignore` & `langfuse_haystack-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `langfuse_haystack-0.0.1/LICENSE.txt` & `langfuse_haystack-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langfuse_haystack-0.0.1/pyproject.toml` & `langfuse_haystack-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `langfuse_haystack-0.0.1/PKG-INFO` & `langfuse_haystack-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: langfuse-haystack
-Version: 0.0.1
+Version: 0.0.2
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/langfuse#readme
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/langfuse
 Author-email: deepset GmbH <info@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -19,26 +19,27 @@
 Requires-Python: >=3.8
 Requires-Dist: haystack-ai
 Requires-Dist: langfuse
 Description-Content-Type: text/markdown
 
 # langfuse
 
-[![PyPI - Version](https://img.shields.io/pypi/v/langfuse.svg)](https://pypi.org/project/langfuse)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/langfuse.svg)](https://pypi.org/project/langfuse)
+[![PyPI - Version](https://img.shields.io/pypi/v/langfuse-haystack.svg)](https://pypi.org/project/langfuse-haystack)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/langfuse-haystack.svg)](https://pypi.org/project/langfuse-haystack)
 
 -----
 
 **Table of Contents**
 
-- [Installation](#installation)
-- [License](#license)
+- [langfuse](#langfuse)
+  - [Installation](#installation)
+  - [License](#license)
 
 ## Installation
 
 ```console
-pip install langfuse
+pip install langfuse-haystack
 ```
 
 ## License
 
 `langfuse` is distributed under the terms of the [Apache-2.0](https://spdx.org/licenses/Apache-2.0.html) license.
```

