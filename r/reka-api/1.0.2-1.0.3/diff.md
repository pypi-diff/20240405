# Comparing `tmp/reka_api-1.0.2.tar.gz` & `tmp/reka_api-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reka_api-1.0.2.tar", max compression
+gzip compressed data, was "reka_api-1.0.3.tar", max compression
```

## Comparing `reka_api-1.0.2.tar` & `reka_api-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    25738 2024-03-14 17:41:01.616956 reka_api-1.0.2/LICENSE
--rw-r--r--   0        0        0      149 2024-03-14 17:41:01.616956 reka_api-1.0.2/README.md
--rw-r--r--   0        0        0     1125 2024-03-14 17:41:01.616956 reka_api-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      825 2024-03-14 17:41:01.616956 reka_api-1.0.2/src/reka/__init__.py
--rw-r--r--   0        0        0        0 2024-03-14 17:41:01.616956 reka_api-1.0.2/src/reka/api/__init__.py
--rw-r--r--   0        0        0     7107 2024-03-14 17:41:01.616956 reka_api-1.0.2/src/reka/api/chat.py
--rw-r--r--   0        0        0     2401 2024-03-14 17:41:01.616956 reka_api-1.0.2/src/reka/api/completion.py
--rw-r--r--   0        0        0     2077 2024-03-14 17:41:01.616956 reka_api-1.0.2/src/reka/api/dataset.py
--rw-r--r--   0        0        0     2223 2024-03-14 17:41:01.616956 reka_api-1.0.2/src/reka/api/driver.py
--rw-r--r--   0        0        0      694 2024-03-14 17:41:01.616956 reka_api-1.0.2/src/reka/api/job.py
--rw-r--r--   0        0        0      373 2024-03-14 17:41:01.616956 reka_api-1.0.2/src/reka/api/models.py
--rw-r--r--   0        0        0     3563 2024-03-14 17:41:01.616956 reka_api-1.0.2/src/reka/api/retrieval.py
--rw-r--r--   0        0        0     1141 2024-03-14 17:41:01.616956 reka_api-1.0.2/src/reka/errors.py
--rw-r--r--   0        0        0        0 2024-03-14 17:41:01.616956 reka_api-1.0.2/src/reka/py.typed
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 reka_api-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    25738 2024-04-05 19:13:00.208574 reka_api-1.0.3/LICENSE
+-rw-r--r--   0        0        0      149 2024-04-05 19:13:00.208574 reka_api-1.0.3/README.md
+-rw-r--r--   0        0        0     1125 2024-04-05 19:13:00.208574 reka_api-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      825 2024-04-05 19:13:00.208574 reka_api-1.0.3/src/reka/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:13:00.208574 reka_api-1.0.3/src/reka/api/__init__.py
+-rw-r--r--   0        0        0     7282 2024-04-05 19:13:00.208574 reka_api-1.0.3/src/reka/api/chat.py
+-rw-r--r--   0        0        0     2401 2024-04-05 19:13:00.208574 reka_api-1.0.3/src/reka/api/completion.py
+-rw-r--r--   0        0        0     2077 2024-04-05 19:13:00.208574 reka_api-1.0.3/src/reka/api/dataset.py
+-rw-r--r--   0        0        0     2223 2024-04-05 19:13:00.208574 reka_api-1.0.3/src/reka/api/driver.py
+-rw-r--r--   0        0        0      694 2024-04-05 19:13:00.208574 reka_api-1.0.3/src/reka/api/job.py
+-rw-r--r--   0        0        0      373 2024-04-05 19:13:00.208574 reka_api-1.0.3/src/reka/api/models.py
+-rw-r--r--   0        0        0     3563 2024-04-05 19:13:00.208574 reka_api-1.0.3/src/reka/api/retrieval.py
+-rw-r--r--   0        0        0     1141 2024-04-05 19:13:00.208574 reka_api-1.0.3/src/reka/errors.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:13:00.208574 reka_api-1.0.3/src/reka/py.typed
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 reka_api-1.0.3/PKG-INFO
```

### Comparing `reka_api-1.0.2/LICENSE` & `reka_api-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.2/pyproject.toml` & `reka_api-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reka-api"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
     "Reka Team <contact@reka.ai>",
 ]
 description = "Reka API"
 readme = "README.md"
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `reka_api-1.0.2/src/reka/__init__.py` & `reka_api-1.0.3/src/reka/__init__.py`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.2/src/reka/api/chat.py` & `reka_api-1.0.3/src/reka/api/chat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Chat-related server interactions (including VLM chat)"""
 
 from __future__ import annotations
 
-from typing import List, Literal, Optional, TypedDict, cast
+from typing import Any, Dict, List, Literal, Optional, TypedDict, cast
 
 import reka.api.driver as driver
 from reka.errors import InvalidConversationError
 
 
 class ModelTurn(TypedDict):
     """A turn in a conversation output by the model."""
@@ -41,14 +41,15 @@
     random_seed: Optional[int] = None,
     runtime_top_k: Optional[int] = None,
     runtime_top_p: Optional[float] = None,
     frequency_penalty: Optional[float] = None,
     presence_penalty: Optional[float] = None,
     length_penalty: Optional[float] = None,
     stop_words: Optional[List[str]] = None,
+    extra_request_args: Optional[Dict[str, Any]] = None,
 ) -> ModelTurn:
     """Chat endpoint.
 
     Example usage:
     ```python
     import reka
 
@@ -66,30 +67,30 @@
     ```
 
     Args:
         human: latest message from human.
         media_url: an optional URL for the media (image, video, or audio) to chat about. This may only be set for the
             first turn (when conversation_history is empty).
         media_type: the media type (image, video, or audio) - this should be set when media_url is set.
-        conversation_history: where each dict has a key "type"
+        conversation_history: list of dicts, where each dict has a key "type"
             indicating the speaker, either "human" or "model", and a key "text"
             containing the message from the speaker. If not set, will default to
             an empty history. The first turn may also have "media_url" and "media_type" set.
         retrieval_dataset: Previousy uploaded dataset to do retrieval on.
         model_name: Name of model.
         request_output_len: Completion length in tokens.
         temperature: Softmax temperature, higher is more diverse.
         random_seed: Seed to obtain different results.
         runtime_top_k: Keep only k top tokens when sampling.
         runtime_top_p: Keep only top p quantile when sampling.
-        frequency_penalty: Penalize repetitions. 1 means no penalty.
-        presence_penalty: Penalize repetitions. 1 means no penalty.
+        frequency_penalty: Penalize repetitions. 0 means no penalty.
+        presence_penalty: Penalize repetitions. 0 means no penalty.
         length_penalty: Penalize short answers. 1 means no penalty.
         stop_words: Optional list of words on which to stop generation.
-        assistant_start_text: Optional text that the assistant (model) response should start with.
+        extra_request_args: Optional extra arguments to include in the request, useful for experimental API features.
 
     Raises:
         InvalidConversationError: if the conversation history is not valid.
 
     Returns:
         ModelTurn: A dict containing `{"type": "model", "text": <response from the model>}`. If `retrieval_dataset` is
             set, then this will also contain `"retrieved_chunks"`.
@@ -121,14 +122,17 @@
             ("presence_penalty", presence_penalty),
             ("length_penalty", length_penalty),
             ("stop_words", stop_words or []),
         ]
         if value is not None
     }
 
+    if extra_request_args:
+        json_dict.update(extra_request_args)
+
     response = driver.make_request(
         method="post",
         endpoint="chat",
         headers={"Content-Type": "application/json"},
         json=json_dict,
     )
```

### Comparing `reka_api-1.0.2/src/reka/api/completion.py` & `reka_api-1.0.3/src/reka/api/completion.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 
         model_name: Name of model.
         request_output_len: Completion length in tokens.
         temperature: Softmax temperature, higher is more diverse.
         random_seed: Seed to obtain different results.
         runtime_top_k: Keep only k top tokens when sampling.
         runtime_top_p: Keep only top p quantile when sampling.
-        frequency_penalty: Penalize repetition. 1 means no penalty.
-        presence_penalty: Penalize repetition. 1 means no penalty.
+        frequency_penalty: Penalize repetition. 0 means no penalty.
+        presence_penalty: Penalize repetition. 0 means no penalty.
         length_penalty: Penalize short answers. 1 means no penalty.
         stop_words: Optional list of words on which to stop generation.
 
     Returns:
         model completion.
     """
     json_dict = {
```

### Comparing `reka_api-1.0.2/src/reka/api/dataset.py` & `reka_api-1.0.3/src/reka/api/dataset.py`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.2/src/reka/api/driver.py` & `reka_api-1.0.3/src/reka/api/driver.py`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.2/src/reka/api/job.py` & `reka_api-1.0.3/src/reka/api/job.py`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.2/src/reka/api/retrieval.py` & `reka_api-1.0.3/src/reka/api/retrieval.py`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.2/src/reka/errors.py` & `reka_api-1.0.3/src/reka/errors.py`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.2/PKG-INFO` & `reka_api-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reka-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: Reka API
 Home-page: https://reka.ai/
 Author: Reka Team
 Author-email: contact@reka.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

