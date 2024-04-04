# Comparing `tmp/llama_index_embeddings_clip-0.1.4.tar.gz` & `tmp/llama_index_embeddings_clip-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_embeddings_clip-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_embeddings_clip-0.1.5.tar", max compression
```

## Comparing `llama_index_embeddings_clip-0.1.4.tar` & `llama_index_embeddings_clip-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       42 2024-02-13 13:53:01.605393 llama_index_embeddings_clip-0.1.4/README.md
--rw-r--r--   0        0        0       88 2024-02-13 13:53:01.605609 llama_index_embeddings_clip-0.1.4/llama_index/embeddings/clip/__init__.py
--rw-r--r--   0        0        0     4624 2024-02-20 18:45:10.197104 llama_index_embeddings_clip-0.1.4/llama_index/embeddings/clip/base.py
--rw-r--r--   0        0        0     1516 2024-02-21 16:18:40.976711 llama_index_embeddings_clip-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      810 1970-01-01 00:00:00.000000 llama_index_embeddings_clip-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       42 2024-04-04 22:08:09.077314 llama_index_embeddings_clip-0.1.5/README.md
+-rw-r--r--   0        0        0       88 2024-04-04 22:08:09.081314 llama_index_embeddings_clip-0.1.5/llama_index/embeddings/clip/__init__.py
+-rw-r--r--   0        0        0     4716 2024-04-04 22:08:09.081314 llama_index_embeddings_clip-0.1.5/llama_index/embeddings/clip/base.py
+-rw-r--r--   0        0        0     1516 2024-04-04 22:08:09.081314 llama_index_embeddings_clip-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 llama_index_embeddings_clip-0.1.5/PKG-INFO
```

### Comparing `llama_index_embeddings_clip-0.1.4/llama_index/embeddings/clip/base.py` & `llama_index_embeddings_clip-0.1.5/llama_index/embeddings/clip/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from llama_index.core.base.embeddings.base import Embedding
 from llama_index.core.bridge.pydantic import Field, PrivateAttr
 from llama_index.core.constants import DEFAULT_EMBED_BATCH_SIZE
 from llama_index.core.embeddings.multi_modal_base import MultiModalEmbedding
 from llama_index.core.schema import ImageType
 from PIL import Image
+import os
 
 logger = logging.getLogger(__name__)
 
 
 AVAILABLE_CLIP_MODELS = (
     "RN50",
     "RN101",
@@ -82,15 +83,16 @@
 
         super().__init__(
             embed_batch_size=embed_batch_size, model_name=model_name, **kwargs
         )
 
         try:
             self._device = "cuda" if torch.cuda.is_available() else "cpu"
-            if self.model_name not in AVAILABLE_CLIP_MODELS:
+            is_local_path = os.path.exists(self.model_name)
+            if not is_local_path and self.model_name not in AVAILABLE_CLIP_MODELS:
                 raise ValueError(
                     f"Model name {self.model_name} is not available in CLIP."
                 )
             self._model, self._preprocess = clip.load(
                 self.model_name, device=self._device
             )
```

### Comparing `llama_index_embeddings_clip-0.1.4/pyproject.toml` & `llama_index_embeddings_clip-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index embeddings clip integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-embeddings-clip"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 torch = "^2.1.2"
 pillow = "^10.2.0"
 torchvision = "^0.17.0"
```

### Comparing `llama_index_embeddings_clip-0.1.4/PKG-INFO` & `llama_index_embeddings_clip-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: llama-index-embeddings-clip
-Version: 0.1.4
+Version: 0.1.5
 Summary: llama-index embeddings clip integration
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
 Requires-Dist: ftfy (>=6.1.3,<7.0.0)
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: torch (>=2.1.2,<3.0.0)
 Requires-Dist: torchvision (>=0.17.0,<0.18.0)
 Description-Content-Type: text/markdown
```

