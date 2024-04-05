# Comparing `tmp/mixedbread_ai-2.1.0.tar.gz` & `tmp/mixedbread_ai-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixedbread_ai-2.1.0.tar", max compression
+gzip compressed data, was "mixedbread_ai-2.1.1.tar", max compression
```

## Comparing `mixedbread_ai-2.1.0.tar` & `mixedbread_ai-2.1.1.tar`

### file list

```diff
@@ -1,54 +1,56 @@
--rw-r--r--   0        0        0    11348 2024-04-03 13:00:22.152145 mixedbread_ai-2.1.0/LICENSE.md
--rw-r--r--   0        0        0     3841 2024-04-03 13:00:22.152145 mixedbread_ai-2.1.0/README.md
--rw-r--r--   0        0        0     1981 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/__init__.py
--rw-r--r--   0        0        0    24344 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/client.py
--rw-r--r--   0        0        0      790 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/core/api_error.py
--rw-r--r--   0        0        0     1081 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/core/file.py
--rw-r--r--   0        0        0     4882 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/core/http_client.py
--rw-r--r--   0        0        0     3799 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/core/request_options.py
--rw-r--r--   0        0        0      163 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/environment.py
--rw-r--r--   0        0        0      620 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/errors/__init__.py
--rw-r--r--   0        0        0      305 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/errors/bad_request_error.py
--rw-r--r--   0        0        0      300 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/errors/forbidden_error.py
--rw-r--r--   0        0        0      289 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/errors/internal_server_error.py
--rw-r--r--   0        0        0      297 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/errors/not_found_error.py
--rw-r--r--   0        0        0      326 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/errors/too_many_requests_error.py
--rw-r--r--   0        0        0      312 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/errors/unauthorized_error.py
--rw-r--r--   0        0        0      300 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0     2337 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/__init__.py
--rw-r--r--   0        0        0     1163 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/bad_request_error_body.py
--rw-r--r--   0        0        0      268 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/data.py
--rw-r--r--   0        0        0     1202 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/embedding.py
--rw-r--r--   0        0        0      152 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/embedding_item.py
--rw-r--r--   0        0        0      217 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/embeddings_request_encoding_format.py
--rw-r--r--   0        0        0     1612 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/embeddings_response.py
--rw-r--r--   0        0        0      218 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/embeddings_response_encoding_format.py
--rw-r--r--   0        0        0     1052 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/encoding_format.py
--rw-r--r--   0        0        0     1160 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/forbidden_error_body.py
--rw-r--r--   0        0        0      206 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/input.py
--rw-r--r--   0        0        0     1152 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/internal_error.py
--rw-r--r--   0        0        0     1194 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/invalid_matryoshka_dimensions_error.py
--rw-r--r--   0        0        0     1184 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/invalid_matryoshka_model_error.py
--rw-r--r--   0        0        0     1166 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/model_not_found_error.py
--rw-r--r--   0        0        0     1411 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/multiple_encodings_embedding.py
--rw-r--r--   0        0        0     1293 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/multiple_encodings_embedding_item.py
--rw-r--r--   0        0        0     1125 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/mxbai_api_error.py
--rw-r--r--   0        0        0      171 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/mxbai_api_error_details.py
--rw-r--r--   0        0        0     1159 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/not_found_error_body.py
--rw-r--r--   0        0        0      837 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/object_type.py
--rw-r--r--   0        0        0     1223 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/ranked_document.py
--rw-r--r--   0        0        0     1558 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/reranking_response.py
--rw-r--r--   0        0        0      970 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/text_document.py
--rw-r--r--   0        0        0     1174 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/too_many_requests_error_body.py
--rw-r--r--   0        0        0      689 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/truncation_strategy.py
--rw-r--r--   0        0        0     1166 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/unauthorized_error_body.py
--rw-r--r--   0        0        0     1133 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/usage.py
--rw-r--r--   0        0        0      141 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/validation_error.py
--rw-r--r--   0        0        0     1161 2024-04-03 13:00:22.160145 mixedbread_ai-2.1.0/mixedbread_ai/types/web_truncation_error.py
--rw-r--r--   0        0        0      544 2024-04-03 13:00:22.160145 mixedbread_ai-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     4842 1970-01-01 00:00:00.000000 mixedbread_ai-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11348 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/LICENSE.md
+-rw-r--r--   0        0        0     4368 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/README.md
+-rw-r--r--   0        0        0     2049 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/__init__.py
+-rw-r--r--   0        0        0    24258 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/client.py
+-rw-r--r--   0        0        0      790 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/core/api_error.py
+-rw-r--r--   0        0        0     1081 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/core/file.py
+-rw-r--r--   0        0        0     4882 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/core/http_client.py
+-rw-r--r--   0        0        0     3799 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/core/request_options.py
+-rw-r--r--   0        0        0      163 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/environment.py
+-rw-r--r--   0        0        0      620 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/errors/__init__.py
+-rw-r--r--   0        0        0      305 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/errors/bad_request_error.py
+-rw-r--r--   0        0        0      300 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/errors/forbidden_error.py
+-rw-r--r--   0        0        0      289 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/errors/internal_server_error.py
+-rw-r--r--   0        0        0      297 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/errors/not_found_error.py
+-rw-r--r--   0        0        0      326 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/errors/too_many_requests_error.py
+-rw-r--r--   0        0        0      312 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      300 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0     2445 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/__init__.py
+-rw-r--r--   0        0        0     1163 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/bad_request_error_body.py
+-rw-r--r--   0        0        0      268 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/data.py
+-rw-r--r--   0        0        0     1202 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/embedding.py
+-rw-r--r--   0        0        0      152 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/embedding_item.py
+-rw-r--r--   0        0        0      217 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/embeddings_request_encoding_format.py
+-rw-r--r--   0        0        0     1613 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/embeddings_response.py
+-rw-r--r--   0        0        0      218 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/embeddings_response_encoding_format.py
+-rw-r--r--   0        0        0     1052 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/encoding_format.py
+-rw-r--r--   0        0        0     1160 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/forbidden_error_body.py
+-rw-r--r--   0        0        0      187 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/input.py
+-rw-r--r--   0        0        0     1152 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/internal_error.py
+-rw-r--r--   0        0        0     1194 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/invalid_matryoshka_dimensions_error.py
+-rw-r--r--   0        0        0     1184 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/invalid_matryoshka_model_error.py
+-rw-r--r--   0        0        0     1166 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/model_not_found_error.py
+-rw-r--r--   0        0        0      216 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/multi_modal_input.py
+-rw-r--r--   0        0        0     1411 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/multiple_encodings_embedding.py
+-rw-r--r--   0        0        0     1465 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/multiple_encodings_embedding_item.py
+-rw-r--r--   0        0        0     1125 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/mxbai_api_error.py
+-rw-r--r--   0        0        0      171 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/mxbai_api_error_details.py
+-rw-r--r--   0        0        0     1159 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/not_found_error_body.py
+-rw-r--r--   0        0        0      837 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/object_type.py
+-rw-r--r--   0        0        0      161 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/query.py
+-rw-r--r--   0        0        0     1223 2024-04-05 14:40:30.879906 mixedbread_ai-2.1.1/mixedbread_ai/types/ranked_document.py
+-rw-r--r--   0        0        0     1558 2024-04-05 14:40:30.879906 mixedbread_ai-2.1.1/mixedbread_ai/types/reranking_response.py
+-rw-r--r--   0        0        0      970 2024-04-05 14:40:30.879906 mixedbread_ai-2.1.1/mixedbread_ai/types/text_document.py
+-rw-r--r--   0        0        0     1174 2024-04-05 14:40:30.879906 mixedbread_ai-2.1.1/mixedbread_ai/types/too_many_requests_error_body.py
+-rw-r--r--   0        0        0      689 2024-04-05 14:40:30.879906 mixedbread_ai-2.1.1/mixedbread_ai/types/truncation_strategy.py
+-rw-r--r--   0        0        0     1166 2024-04-05 14:40:30.879906 mixedbread_ai-2.1.1/mixedbread_ai/types/unauthorized_error_body.py
+-rw-r--r--   0        0        0     1134 2024-04-05 14:40:30.879906 mixedbread_ai-2.1.1/mixedbread_ai/types/usage.py
+-rw-r--r--   0        0        0      141 2024-04-05 14:40:30.879906 mixedbread_ai-2.1.1/mixedbread_ai/types/validation_error.py
+-rw-r--r--   0        0        0     1161 2024-04-05 14:40:30.879906 mixedbread_ai-2.1.1/mixedbread_ai/types/web_truncation_error.py
+-rw-r--r--   0        0        0      544 2024-04-05 14:40:30.879906 mixedbread_ai-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5369 1970-01-01 00:00:00.000000 mixedbread_ai-2.1.1/PKG-INFO
```

### Comparing `mixedbread_ai-2.1.0/LICENSE.md` & `mixedbread_ai-2.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.0/README.md` & `mixedbread_ai-2.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -64,14 +64,31 @@
     input=["I like to eat apples.", "I like to eat bananas."],
     prompt="Represent this sentence for searching relevant passages"
 )
 
 print(embeddings)
 ```
 
+By specifying the encoding format, you can leverage f.e. binary embeddings.
+
+```python
+from mixedbread_ai.client import MixedbreadAI
+from mixedbread_ai.types import EncodingFormat
+
+mxbai = MixedbreadAI(api_key="{YOUR_API_KEY}")
+
+embeddings = mxbai.embeddings(
+    model="mixedbread-ai/mxbai-embed-large-v1",
+    input=["I like to eat apples.", "I like to eat bananas."],
+    encoding_format=[EncodingFormat.FLOAT, EncodingFormat.UBINARY]
+)
+
+print(embeddings.data[0].embedding.float_, embeddings.data[0].embedding.ubinary)
+```
+
 ### Reranking (Asynchronous)
 Here's an asynchronous example of using the mixedbread ai SDK to rerank documents:
 ```python
 from mixedbread_ai.client import AsyncMixedbreadAI
 
 mxbai_async = AsyncMixedbreadAI(api_key="{YOUR_API_KEY}")
```

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/__init__.py` & `mixedbread_ai-2.1.1/mixedbread_ai/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,20 +11,22 @@
     EncodingFormat,
     ForbiddenErrorBody,
     Input,
     InternalError,
     InvalidMatryoshkaDimensionsError,
     InvalidMatryoshkaModelError,
     ModelNotFoundError,
+    MultiModalInput,
     MultipleEncodingsEmbedding,
     MultipleEncodingsEmbeddingItem,
     MxbaiApiError,
     MxbaiApiErrorDetails,
     NotFoundErrorBody,
     ObjectType,
+    Query,
     RankedDocument,
     RerankingResponse,
     TextDocument,
     TooManyRequestsErrorBody,
     TruncationStrategy,
     UnauthorizedErrorBody,
     Usage,
@@ -57,21 +59,23 @@
     "Input",
     "InternalError",
     "InternalServerError",
     "InvalidMatryoshkaDimensionsError",
     "InvalidMatryoshkaModelError",
     "MixedbreadAIEnvironment",
     "ModelNotFoundError",
+    "MultiModalInput",
     "MultipleEncodingsEmbedding",
     "MultipleEncodingsEmbeddingItem",
     "MxbaiApiError",
     "MxbaiApiErrorDetails",
     "NotFoundError",
     "NotFoundErrorBody",
     "ObjectType",
+    "Query",
     "RankedDocument",
     "RerankingResponse",
     "TextDocument",
     "TooManyRequestsError",
     "TooManyRequestsErrorBody",
     "TruncationStrategy",
     "UnauthorizedError",
```

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/client.py` & `mixedbread_ai-2.1.1/mixedbread_ai/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,18 @@
 from .errors.unprocessable_entity_error import UnprocessableEntityError
 from .types.bad_request_error_body import BadRequestErrorBody
 from .types.embeddings_request_encoding_format import EmbeddingsRequestEncodingFormat
 from .types.embeddings_response import EmbeddingsResponse
 from .types.forbidden_error_body import ForbiddenErrorBody
 from .types.input import Input
 from .types.internal_error import InternalError
+from .types.multi_modal_input import MultiModalInput
 from .types.not_found_error_body import NotFoundErrorBody
+from .types.query import Query
 from .types.reranking_response import RerankingResponse
-from .types.text_document import TextDocument
 from .types.too_many_requests_error_body import TooManyRequestsErrorBody
 from .types.truncation_strategy import TruncationStrategy
 from .types.unauthorized_error_body import UnauthorizedErrorBody
 from .types.validation_error import ValidationError
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
@@ -78,69 +79,69 @@
             api_key=api_key,
             httpx_client=httpx.Client(timeout=timeout) if httpx_client is None else httpx_client,
         )
 
     def embeddings(
         self,
         *,
-        dimensions: typing.Optional[int] = OMIT,
-        encoding_format: typing.Optional[EmbeddingsRequestEncodingFormat] = OMIT,
-        input: Input,
-        instruction: typing.Optional[str] = OMIT,
         model: str,
+        input: MultiModalInput,
         normalized: typing.Optional[bool] = OMIT,
-        prompt: typing.Optional[str] = OMIT,
-        texts: typing.Optional[typing.Sequence[str]] = OMIT,
+        encoding_format: typing.Optional[EmbeddingsRequestEncodingFormat] = OMIT,
         truncation_strategy: typing.Optional[TruncationStrategy] = OMIT,
+        dimensions: typing.Optional[int] = OMIT,
+        instruction: typing.Optional[str] = OMIT,
+        texts: typing.Optional[typing.Sequence[str]] = OMIT,
+        prompt: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> EmbeddingsResponse:
         """
         Create embeddings for text or images using the specified model, encoding format, and normalization.
 
         Parameters:
-            - dimensions: typing.Optional[int].
+            - model: str. The model to use for creating embeddings
 
-            - encoding_format: typing.Optional[EmbeddingsRequestEncodingFormat].
+            - input: MultiModalInput.
 
-            - input: Input.
+            - normalized: typing.Optional[bool]. Whether to normalize the embeddings
 
-            - instruction: typing.Optional[str].
+            - encoding_format: typing.Optional[EmbeddingsRequestEncodingFormat].
 
-            - model: str. The model to use for creating embeddings
+            - truncation_strategy: typing.Optional[TruncationStrategy]. The truncation strategy to use for the input
 
-            - normalized: typing.Optional[bool]. Whether to normalize the embeddings
+            - dimensions: typing.Optional[int].
 
-            - prompt: typing.Optional[str].
+            - instruction: typing.Optional[str].
 
             - texts: typing.Optional[typing.Sequence[str]].
 
-            - truncation_strategy: typing.Optional[TruncationStrategy]. The truncation strategy to use for the input
+            - prompt: typing.Optional[str].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from mixedbread-ai.client import MixedbreadAI
 
         client = MixedbreadAI(api_key="YOUR_API_KEY", )
-        client.embeddings(input="input", model="model", )
+        client.embeddings(model="model", input="input", )
         """
-        _request: typing.Dict[str, typing.Any] = {"input": input, "model": model}
-        if dimensions is not OMIT:
-            _request["dimensions"] = dimensions
+        _request: typing.Dict[str, typing.Any] = {"model": model, "input": input}
+        if normalized is not OMIT:
+            _request["normalized"] = normalized
         if encoding_format is not OMIT:
             _request["encoding_format"] = encoding_format
+        if truncation_strategy is not OMIT:
+            _request["truncation_strategy"] = truncation_strategy
+        if dimensions is not OMIT:
+            _request["dimensions"] = dimensions
         if instruction is not OMIT:
             _request["instruction"] = instruction
-        if normalized is not OMIT:
-            _request["normalized"] = normalized
-        if prompt is not OMIT:
-            _request["prompt"] = prompt
         if texts is not OMIT:
             _request["texts"] = texts
-        if truncation_strategy is not OMIT:
-            _request["truncation_strategy"] = truncation_strategy
+        if prompt is not OMIT:
+            _request["prompt"] = prompt
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/embeddings"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
@@ -186,46 +187,46 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def reranking(
         self,
         *,
-        input: typing.Sequence[TextDocument],
         model: str,
-        query: TextDocument,
-        return_input: typing.Optional[bool] = OMIT,
+        input: Input,
+        query: Query,
         top_k: typing.Optional[int] = OMIT,
+        return_input: typing.Optional[bool] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> RerankingResponse:
         """
         Parameters:
-            - input: typing.Sequence[TextDocument]. The input documents to rerank
-
             - model: str. The model to use for creating embeddings
 
-            - query: TextDocument. The query to rerank the documents
+            - input: Input. The input documents to rerank
 
-            - return_input: typing.Optional[bool]. Whether to return the documents
+            - query: Query. The query to rerank the documents
 
             - top_k: typing.Optional[int]. The number of documents to return
 
+            - return_input: typing.Optional[bool]. Whether to return the documents
+
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from mixedbread-ai import TextDocument
         from mixedbread-ai.client import MixedbreadAI
 
         client = MixedbreadAI(api_key="YOUR_API_KEY", )
-        client.reranking(input=[TextDocument(text="text", )], model="model", query=TextDocument(text="text", ), return_input=False, top_k=10, )
+        client.reranking(model="model", input=["input"], query=TextDocument(text="text", ), top_k=10, return_input=False, )
         """
-        _request: typing.Dict[str, typing.Any] = {"input": input, "model": model, "query": query}
-        if return_input is not OMIT:
-            _request["return_input"] = return_input
+        _request: typing.Dict[str, typing.Any] = {"model": model, "input": input, "query": query}
         if top_k is not OMIT:
             _request["top_k"] = top_k
+        if return_input is not OMIT:
+            _request["return_input"] = return_input
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/reranking"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
@@ -309,69 +310,69 @@
             api_key=api_key,
             httpx_client=httpx.AsyncClient(timeout=timeout) if httpx_client is None else httpx_client,
         )
 
     async def embeddings(
         self,
         *,
-        dimensions: typing.Optional[int] = OMIT,
-        encoding_format: typing.Optional[EmbeddingsRequestEncodingFormat] = OMIT,
-        input: Input,
-        instruction: typing.Optional[str] = OMIT,
         model: str,
+        input: MultiModalInput,
         normalized: typing.Optional[bool] = OMIT,
-        prompt: typing.Optional[str] = OMIT,
-        texts: typing.Optional[typing.Sequence[str]] = OMIT,
+        encoding_format: typing.Optional[EmbeddingsRequestEncodingFormat] = OMIT,
         truncation_strategy: typing.Optional[TruncationStrategy] = OMIT,
+        dimensions: typing.Optional[int] = OMIT,
+        instruction: typing.Optional[str] = OMIT,
+        texts: typing.Optional[typing.Sequence[str]] = OMIT,
+        prompt: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> EmbeddingsResponse:
         """
         Create embeddings for text or images using the specified model, encoding format, and normalization.
 
         Parameters:
-            - dimensions: typing.Optional[int].
+            - model: str. The model to use for creating embeddings
 
-            - encoding_format: typing.Optional[EmbeddingsRequestEncodingFormat].
+            - input: MultiModalInput.
 
-            - input: Input.
+            - normalized: typing.Optional[bool]. Whether to normalize the embeddings
 
-            - instruction: typing.Optional[str].
+            - encoding_format: typing.Optional[EmbeddingsRequestEncodingFormat].
 
-            - model: str. The model to use for creating embeddings
+            - truncation_strategy: typing.Optional[TruncationStrategy]. The truncation strategy to use for the input
 
-            - normalized: typing.Optional[bool]. Whether to normalize the embeddings
+            - dimensions: typing.Optional[int].
 
-            - prompt: typing.Optional[str].
+            - instruction: typing.Optional[str].
 
             - texts: typing.Optional[typing.Sequence[str]].
 
-            - truncation_strategy: typing.Optional[TruncationStrategy]. The truncation strategy to use for the input
+            - prompt: typing.Optional[str].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from mixedbread-ai.client import AsyncMixedbreadAI
 
         client = AsyncMixedbreadAI(api_key="YOUR_API_KEY", )
-        await client.embeddings(input="input", model="model", )
+        await client.embeddings(model="model", input="input", )
         """
-        _request: typing.Dict[str, typing.Any] = {"input": input, "model": model}
-        if dimensions is not OMIT:
-            _request["dimensions"] = dimensions
+        _request: typing.Dict[str, typing.Any] = {"model": model, "input": input}
+        if normalized is not OMIT:
+            _request["normalized"] = normalized
         if encoding_format is not OMIT:
             _request["encoding_format"] = encoding_format
+        if truncation_strategy is not OMIT:
+            _request["truncation_strategy"] = truncation_strategy
+        if dimensions is not OMIT:
+            _request["dimensions"] = dimensions
         if instruction is not OMIT:
             _request["instruction"] = instruction
-        if normalized is not OMIT:
-            _request["normalized"] = normalized
-        if prompt is not OMIT:
-            _request["prompt"] = prompt
         if texts is not OMIT:
             _request["texts"] = texts
-        if truncation_strategy is not OMIT:
-            _request["truncation_strategy"] = truncation_strategy
+        if prompt is not OMIT:
+            _request["prompt"] = prompt
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/embeddings"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
@@ -417,46 +418,46 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def reranking(
         self,
         *,
-        input: typing.Sequence[TextDocument],
         model: str,
-        query: TextDocument,
-        return_input: typing.Optional[bool] = OMIT,
+        input: Input,
+        query: Query,
         top_k: typing.Optional[int] = OMIT,
+        return_input: typing.Optional[bool] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> RerankingResponse:
         """
         Parameters:
-            - input: typing.Sequence[TextDocument]. The input documents to rerank
-
             - model: str. The model to use for creating embeddings
 
-            - query: TextDocument. The query to rerank the documents
+            - input: Input. The input documents to rerank
 
-            - return_input: typing.Optional[bool]. Whether to return the documents
+            - query: Query. The query to rerank the documents
 
             - top_k: typing.Optional[int]. The number of documents to return
 
+            - return_input: typing.Optional[bool]. Whether to return the documents
+
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from mixedbread-ai import TextDocument
         from mixedbread-ai.client import AsyncMixedbreadAI
 
         client = AsyncMixedbreadAI(api_key="YOUR_API_KEY", )
-        await client.reranking(input=[TextDocument(text="text", )], model="model", query=TextDocument(text="text", ), return_input=False, top_k=10, )
+        await client.reranking(model="model", input=["input"], query=TextDocument(text="text", ), top_k=10, return_input=False, )
         """
-        _request: typing.Dict[str, typing.Any] = {"input": input, "model": model, "query": query}
-        if return_input is not OMIT:
-            _request["return_input"] = return_input
+        _request: typing.Dict[str, typing.Any] = {"model": model, "input": input, "query": query}
         if top_k is not OMIT:
             _request["top_k"] = top_k
+        if return_input is not OMIT:
+            _request["return_input"] = return_input
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/reranking"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
```

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/core/__init__.py` & `mixedbread_ai-2.1.1/mixedbread_ai/core/__init__.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/core/client_wrapper.py` & `mixedbread_ai-2.1.1/mixedbread_ai/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/core/datetime_utils.py` & `mixedbread_ai-2.1.1/mixedbread_ai/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/core/file.py` & `mixedbread_ai-2.1.1/mixedbread_ai/core/file.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/core/http_client.py` & `mixedbread_ai-2.1.1/mixedbread_ai/core/http_client.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/core/jsonable_encoder.py` & `mixedbread_ai-2.1.1/mixedbread_ai/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/core/request_options.py` & `mixedbread_ai-2.1.1/mixedbread_ai/core/request_options.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/errors/__init__.py` & `mixedbread_ai-2.1.1/mixedbread_ai/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/types/__init__.py` & `mixedbread_ai-2.1.1/mixedbread_ai/types/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,20 +10,22 @@
 from .encoding_format import EncodingFormat
 from .forbidden_error_body import ForbiddenErrorBody
 from .input import Input
 from .internal_error import InternalError
 from .invalid_matryoshka_dimensions_error import InvalidMatryoshkaDimensionsError
 from .invalid_matryoshka_model_error import InvalidMatryoshkaModelError
 from .model_not_found_error import ModelNotFoundError
+from .multi_modal_input import MultiModalInput
 from .multiple_encodings_embedding import MultipleEncodingsEmbedding
 from .multiple_encodings_embedding_item import MultipleEncodingsEmbeddingItem
 from .mxbai_api_error import MxbaiApiError
 from .mxbai_api_error_details import MxbaiApiErrorDetails
 from .not_found_error_body import NotFoundErrorBody
 from .object_type import ObjectType
+from .query import Query
 from .ranked_document import RankedDocument
 from .reranking_response import RerankingResponse
 from .text_document import TextDocument
 from .too_many_requests_error_body import TooManyRequestsErrorBody
 from .truncation_strategy import TruncationStrategy
 from .unauthorized_error_body import UnauthorizedErrorBody
 from .usage import Usage
@@ -41,20 +43,22 @@
     "EncodingFormat",
     "ForbiddenErrorBody",
     "Input",
     "InternalError",
     "InvalidMatryoshkaDimensionsError",
     "InvalidMatryoshkaModelError",
     "ModelNotFoundError",
+    "MultiModalInput",
     "MultipleEncodingsEmbedding",
     "MultipleEncodingsEmbeddingItem",
     "MxbaiApiError",
     "MxbaiApiErrorDetails",
     "NotFoundErrorBody",
     "ObjectType",
+    "Query",
     "RankedDocument",
     "RerankingResponse",
     "TextDocument",
     "TooManyRequestsErrorBody",
     "TruncationStrategy",
     "UnauthorizedErrorBody",
     "Usage",
```

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/types/bad_request_error_body.py` & `mixedbread_ai-2.1.1/mixedbread_ai/types/bad_request_error_body.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class BadRequestErrorBody(pydantic.BaseModel):
     type: typing.Optional[typing.Literal["bad_request_error"]] = None
-    details: typing.Optional[MxbaiApiErrorDetails] = None
-    message: typing.Optional[str] = None
     url: typing.Optional[str] = None
+    message: typing.Optional[str] = None
+    details: typing.Optional[MxbaiApiErrorDetails] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/types/embedding.py` & `mixedbread_ai-2.1.1/mixedbread_ai/types/embedding.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/types/embeddings_response.py` & `mixedbread_ai-2.1.1/mixedbread_ai/types/embeddings_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,41 +12,42 @@
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class EmbeddingsResponse(pydantic.BaseModel):
-    data: Data = pydantic.Field()
+    usage: Usage = pydantic.Field()
     """
-    The created embeddings
+    The usage of the model
     """
 
-    dimensions: typing.Optional[int] = None
-    encoding_format: EmbeddingsResponseEncodingFormat
     model: str = pydantic.Field()
     """
     The model used
     """
 
-    normalized: bool = pydantic.Field()
+    data: Data = pydantic.Field()
     """
-    Whether the embeddings are normalized
+    The created embeddings
     """
 
     object: typing.Optional[ObjectType] = pydantic.Field(default=None)
     """
     The object type of the response
     """
 
-    usage: Usage = pydantic.Field()
+    normalized: bool = pydantic.Field()
     """
-    The usage of the model
+    Whether the embeddings are normalized
     """
 
+    encoding_format: EmbeddingsResponseEncodingFormat
+    dimensions: typing.Optional[int] = None
+
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/types/encoding_format.py` & `mixedbread_ai-2.1.1/mixedbread_ai/types/encoding_format.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/types/forbidden_error_body.py` & `mixedbread_ai-2.1.1/mixedbread_ai/types/forbidden_error_body.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class ForbiddenErrorBody(pydantic.BaseModel):
     type: typing.Optional[typing.Literal["forbidden_error"]] = None
-    details: typing.Optional[MxbaiApiErrorDetails] = None
-    message: typing.Optional[str] = None
     url: typing.Optional[str] = None
+    message: typing.Optional[str] = None
+    details: typing.Optional[MxbaiApiErrorDetails] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/types/internal_error.py` & `mixedbread_ai-2.1.1/mixedbread_ai/types/internal_error.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class InternalError(pydantic.BaseModel):
     type: typing.Optional[typing.Literal["server_error"]] = None
-    details: typing.Optional[MxbaiApiErrorDetails] = None
-    message: typing.Optional[str] = None
     url: typing.Optional[str] = None
+    message: typing.Optional[str] = None
+    details: typing.Optional[MxbaiApiErrorDetails] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/types/invalid_matryoshka_dimensions_error.py` & `mixedbread_ai-2.1.1/mixedbread_ai/types/invalid_matryoshka_dimensions_error.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class InvalidMatryoshkaDimensionsError(pydantic.BaseModel):
     type: typing.Optional[typing.Literal["invalid_matryoshka_dimensions_error"]] = None
-    details: typing.Optional[MxbaiApiErrorDetails] = None
-    message: typing.Optional[str] = None
     url: typing.Optional[str] = None
+    message: typing.Optional[str] = None
+    details: typing.Optional[MxbaiApiErrorDetails] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/types/invalid_matryoshka_model_error.py` & `mixedbread_ai-2.1.1/mixedbread_ai/types/invalid_matryoshka_model_error.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class InvalidMatryoshkaModelError(pydantic.BaseModel):
     type: typing.Optional[typing.Literal["invalid_matryoshka_model_error"]] = None
-    details: typing.Optional[MxbaiApiErrorDetails] = None
-    message: typing.Optional[str] = None
     url: typing.Optional[str] = None
+    message: typing.Optional[str] = None
+    details: typing.Optional[MxbaiApiErrorDetails] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/types/model_not_found_error.py` & `mixedbread_ai-2.1.1/mixedbread_ai/types/model_not_found_error.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class ModelNotFoundError(pydantic.BaseModel):
     type: typing.Optional[typing.Literal["model_not_found_error"]] = None
-    details: typing.Optional[MxbaiApiErrorDetails] = None
-    message: typing.Optional[str] = None
     url: typing.Optional[str] = None
+    message: typing.Optional[str] = None
+    details: typing.Optional[MxbaiApiErrorDetails] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/types/multiple_encodings_embedding.py` & `mixedbread_ai-2.1.1/mixedbread_ai/types/multiple_encodings_embedding.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/types/multiple_encodings_embedding_item.py` & `mixedbread_ai-2.1.1/mixedbread_ai/types/multiple_encodings_embedding_item.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class MultipleEncodingsEmbeddingItem(pydantic.BaseModel):
-    base_64: typing.List[str] = pydantic.Field(alias="base64")
-    binary: typing.List[int]
-    float_: typing.List[float] = pydantic.Field(alias="float")
-    int_8: typing.List[int] = pydantic.Field(alias="int8")
-    ubinary: typing.List[int]
-    uint_8: typing.List[int] = pydantic.Field(alias="uint8")
+    float_: typing.Optional[typing.List[float]] = pydantic.Field(alias="float", default=None)
+    int_8: typing.Optional[typing.List[int]] = pydantic.Field(alias="int8", default=None)
+    uint_8: typing.Optional[typing.List[int]] = pydantic.Field(alias="uint8", default=None)
+    binary: typing.Optional[typing.List[int]] = None
+    ubinary: typing.Optional[typing.List[int]] = None
+    base_64: typing.Optional[typing.List[str]] = pydantic.Field(alias="base64", default=None)
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/types/mxbai_api_error.py` & `mixedbread_ai-2.1.1/mixedbread_ai/types/mxbai_api_error.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class MxbaiApiError(pydantic.BaseModel):
-    details: typing.Optional[MxbaiApiErrorDetails] = None
-    message: typing.Optional[str] = None
     type: typing.Optional[str] = None
     url: typing.Optional[str] = None
+    message: typing.Optional[str] = None
+    details: typing.Optional[MxbaiApiErrorDetails] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/types/not_found_error_body.py` & `mixedbread_ai-2.1.1/mixedbread_ai/types/not_found_error_body.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class NotFoundErrorBody(pydantic.BaseModel):
     type: typing.Optional[typing.Literal["not_found_error"]] = None
-    details: typing.Optional[MxbaiApiErrorDetails] = None
-    message: typing.Optional[str] = None
     url: typing.Optional[str] = None
+    message: typing.Optional[str] = None
+    details: typing.Optional[MxbaiApiErrorDetails] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/types/object_type.py` & `mixedbread_ai-2.1.1/mixedbread_ai/types/object_type.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/types/ranked_document.py` & `mixedbread_ai-2.1.1/mixedbread_ai/types/ranked_document.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 
 class RankedDocument(pydantic.BaseModel):
     index: int = pydantic.Field()
     """
     The index of the document
     """
 
-    input: typing.Any
-    object: typing.Optional[ObjectType] = pydantic.Field(default=None)
+    score: float = pydantic.Field()
     """
-    The object type
+    The score of the document
     """
 
-    score: float = pydantic.Field()
+    input: typing.Any
+    object: typing.Optional[ObjectType] = pydantic.Field(default=None)
     """
-    The score of the document
+    The object type
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/types/reranking_response.py` & `mixedbread_ai-2.1.1/mixedbread_ai/types/reranking_response.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -11,42 +11,42 @@
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class RerankingResponse(pydantic.BaseModel):
-    data: typing.List[RankedDocument] = pydantic.Field()
+    usage: Usage = pydantic.Field()
     """
-    The ranked documents
+    The usage of the model
     """
 
     model: str = pydantic.Field()
     """
     The model used
     """
 
-    object: typing.Optional[ObjectType] = pydantic.Field(default=None)
+    data: typing.List[RankedDocument] = pydantic.Field()
     """
-    The object type of the response
+    The ranked documents
     """
 
-    return_input: bool = pydantic.Field()
+    object: typing.Optional[ObjectType] = pydantic.Field(default=None)
     """
-    Whether to return the documents
+    The object type of the response
     """
 
     top_k: int = pydantic.Field()
     """
     The number of documents to return
     """
 
-    usage: Usage = pydantic.Field()
+    return_input: bool = pydantic.Field()
     """
-    The usage of the model
+    Whether to return the documents
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/types/text_document.py` & `mixedbread_ai-2.1.1/mixedbread_ai/types/text_document.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/types/too_many_requests_error_body.py` & `mixedbread_ai-2.1.1/mixedbread_ai/types/too_many_requests_error_body.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class TooManyRequestsErrorBody(pydantic.BaseModel):
     type: typing.Optional[typing.Literal["too_many_requests_error"]] = None
-    details: typing.Optional[MxbaiApiErrorDetails] = None
-    message: typing.Optional[str] = None
     url: typing.Optional[str] = None
+    message: typing.Optional[str] = None
+    details: typing.Optional[MxbaiApiErrorDetails] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/types/truncation_strategy.py` & `mixedbread_ai-2.1.1/mixedbread_ai/types/truncation_strategy.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/types/unauthorized_error_body.py` & `mixedbread_ai-2.1.1/mixedbread_ai/types/unauthorized_error_body.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class UnauthorizedErrorBody(pydantic.BaseModel):
     type: typing.Optional[typing.Literal["unauthorized_error"]] = None
-    details: typing.Optional[MxbaiApiErrorDetails] = None
-    message: typing.Optional[str] = None
     url: typing.Optional[str] = None
+    message: typing.Optional[str] = None
+    details: typing.Optional[MxbaiApiErrorDetails] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/types/usage.py` & `mixedbread_ai-2.1.1/mixedbread_ai/types/usage.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,25 +8,26 @@
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class Usage(pydantic.BaseModel):
-    completion_tokens: typing.Optional[int] = None
     prompt_tokens: int = pydantic.Field()
     """
     The number of tokens used for the prompt
     """
 
     total_tokens: int = pydantic.Field()
     """
     The total number of tokens used
     """
 
+    completion_tokens: typing.Optional[int] = None
+
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `mixedbread_ai-2.1.0/mixedbread_ai/types/web_truncation_error.py` & `mixedbread_ai-2.1.1/mixedbread_ai/types/web_truncation_error.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class WebTruncationError(pydantic.BaseModel):
     type: typing.Optional[typing.Literal["truncation_error"]] = None
-    details: typing.Optional[MxbaiApiErrorDetails] = None
-    message: typing.Optional[str] = None
     url: typing.Optional[str] = None
+    message: typing.Optional[str] = None
+    details: typing.Optional[MxbaiApiErrorDetails] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mixedbread_ai-2.1.0/pyproject.toml` & `mixedbread_ai-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mixedbread-ai"
-version = "2.1.0"
+version = "2.1.1"
 description = "mixedbread ai (https://www.mixedbread.ai)"
 authors = ["mixedbread.ai <support@mixedbread.ai>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/mixedbread-ai/python-sdk.git"
 keywords = ["Embeddings", "NLP", "mixedbread.ai"]
 packages = [
```

### Comparing `mixedbread_ai-2.1.0/PKG-INFO` & `mixedbread_ai-2.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixedbread-ai
-Version: 2.1.0
+Version: 2.1.1
 Summary: mixedbread ai (https://www.mixedbread.ai)
 Home-page: https://github.com/mixedbread-ai/python-sdk.git
 License: Apache-2.0
 Keywords: Embeddings,NLP,mixedbread.ai
 Author: mixedbread.ai
 Author-email: support@mixedbread.ai
 Requires-Python: >=3.8,<4.0
@@ -89,14 +89,31 @@
     input=["I like to eat apples.", "I like to eat bananas."],
     prompt="Represent this sentence for searching relevant passages"
 )
 
 print(embeddings)
 ```
 
+By specifying the encoding format, you can leverage f.e. binary embeddings.
+
+```python
+from mixedbread_ai.client import MixedbreadAI
+from mixedbread_ai.types import EncodingFormat
+
+mxbai = MixedbreadAI(api_key="{YOUR_API_KEY}")
+
+embeddings = mxbai.embeddings(
+    model="mixedbread-ai/mxbai-embed-large-v1",
+    input=["I like to eat apples.", "I like to eat bananas."],
+    encoding_format=[EncodingFormat.FLOAT, EncodingFormat.UBINARY]
+)
+
+print(embeddings.data[0].embedding.float_, embeddings.data[0].embedding.ubinary)
+```
+
 ### Reranking (Asynchronous)
 Here's an asynchronous example of using the mixedbread ai SDK to rerank documents:
 ```python
 from mixedbread_ai.client import AsyncMixedbreadAI
 
 mxbai_async = AsyncMixedbreadAI(api_key="{YOUR_API_KEY}")
```

