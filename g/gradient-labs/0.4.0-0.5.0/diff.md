# Comparing `tmp/gradient_labs-0.4.0.tar.gz` & `tmp/gradient_labs-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gradient_labs-0.4.0.tar", max compression
+gzip compressed data, was "gradient_labs-0.5.0.tar", max compression
```

## Comparing `gradient_labs-0.4.0.tar` & `gradient_labs-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       99 2024-03-15 12:40:35.880695 gradient_labs-0.4.0/README.md
--rw-r--r--   0        0        0       88 2024-03-15 12:40:35.880695 gradient_labs-0.4.0/gradient_labs/__init__.py
--rw-r--r--   0        0        0     2747 2024-03-15 12:40:35.880695 gradient_labs-0.4.0/gradient_labs/client.py
--rw-r--r--   0        0        0      504 2024-03-15 12:40:35.880695 gradient_labs-0.4.0/gradient_labs/errors.py
--rw-r--r--   0        0        0     3776 2024-03-15 12:40:35.880695 gradient_labs-0.4.0/gradient_labs/types.py
--rw-r--r--   0        0        0     3653 2024-03-15 12:40:35.880695 gradient_labs-0.4.0/gradient_labs/webhook.py
--rw-r--r--   0        0        0      492 2024-03-15 12:40:35.880695 gradient_labs-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      784 1970-01-01 00:00:00.000000 gradient_labs-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       99 2024-04-05 16:24:24.201707 gradient_labs-0.5.0/README.md
+-rw-r--r--   0        0        0       88 2024-04-05 16:24:24.201707 gradient_labs-0.5.0/gradient_labs/__init__.py
+-rw-r--r--   0        0        0     4082 2024-04-05 16:24:24.201707 gradient_labs-0.5.0/gradient_labs/client.py
+-rw-r--r--   0        0        0      504 2024-04-05 16:24:24.201707 gradient_labs-0.5.0/gradient_labs/errors.py
+-rw-r--r--   0        0        0     3807 2024-04-05 16:24:24.201707 gradient_labs-0.5.0/gradient_labs/types.py
+-rw-r--r--   0        0        0     3653 2024-04-05 16:24:24.201707 gradient_labs-0.5.0/gradient_labs/webhook.py
+-rw-r--r--   0        0        0      492 2024-04-05 16:24:24.201707 gradient_labs-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      784 1970-01-01 00:00:00.000000 gradient_labs-0.5.0/PKG-INFO
```

### Comparing `gradient_labs-0.4.0/gradient_labs/client.py` & `gradient_labs-0.5.0/gradient_labs/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import Any, List
+from typing import Any, List, Optional, Callable
 
 import requests
 from pytz import UTC
 from .errors import ResponseError
 from .types import ParticipantType, Conversation, Attachment
 
 API_BASE_URL = "https://api.gradient-labs.ai"
@@ -11,23 +11,61 @@
 
 
 class Client:
     def __init__(self, *, api_key: str, base_url: str = API_BASE_URL):
         self.api_key = api_key
         self.base_url = base_url
 
+    def assign_conversation(
+        self,
+        *,
+        conversation_id: str,
+        participant_type: ParticipantType,
+        assignee_id: Optional[str] = None,
+        timeout: int = None,
+    ) -> None:
+        """Assigns a conversation to the given participant."""
+        _ = self._put(
+            f"conversations/{conversation_id}/assignee",
+            {
+                "assignee_id": assignee_id,
+                "assignee_type": participant_type,
+            },
+            timeout=timeout,
+        )
+
+    def end_conversation(self, *, conversation_id: str, timeout: int = None) -> None:
+        """Ends the conversation"""
+        _ = self._put(
+            f"conversations/{conversation_id}/end",
+            {},
+            timeout=timeout,
+        )
+
+    def read_conversation(
+        self, *, conversation_id: str, timeout: int = None
+    ) -> Conversation:
+        """Retrieves the conversation"""
+        body = self._get(
+            f"conversations/{conversation_id}",
+            {},
+            timeout=timeout,
+        )
+        return Conversation.from_dict(body)
+
     def start_conversation(
         self,
         *,
         conversation_id: str,
         customer_id: str,
         channel: str,
         metadata: Any = None,
         timeout: int = None,
     ) -> Conversation:
+        """Starts a conversation."""
         body = self._post(
             "conversations",
             {
                 "id": conversation_id,
                 "customer_id": customer_id,
                 "channel": channel,
                 "metadata": metadata,
@@ -44,14 +82,15 @@
         body: str,
         participant_id: str,
         participant_type: ParticipantType,
         created: datetime = None,
         timeout: int = None,
         attachments: List[Attachment] = None,
     ) -> None:
+        """Adds a message to a conversation."""
         if created is None:
             created = datetime.now()
 
         body = self._post(
             f"conversations/{conversation_id}/messages",
             {
                 "id": message_id,
@@ -62,32 +101,34 @@
                 "attachments": [a.to_dict() for a in attachments]
                 if attachments is not None
                 else [],
             },
             timeout=timeout,
         )
 
-    def cancel_conversation(self, *, conversation_id: str, timeout: int = None) -> None:
-        requests.put(
-            f"{self.base_url}/conversations/{conversation_id}/cancel",
-            headers={
-                "Authorization": f"Bearer {self.api_key}",
-                "User-Agent": USER_AGENT,
-            },
-            timeout=timeout,
-        )
-
     def _post(self, path: str, body: Any, timeout: int = None):
+        return self._api_call(requests.post, path, body, timeout)
+
+    def _put(self, path: str, body: Any, timeout: int = None):
+        return self._api_call(requests.put, path, body, timeout)
+
+    def _get(self, path: str, body: Any, timeout: int = None):
+        return self._api_call(requests.get, path, body, timeout)
+
+    def _api_call(
+        self, request_func: Callable, path: str, body: Any, timeout: int = None
+    ):
         url = f"{self.base_url}/{path}"
-        rsp = requests.post(
+        rsp = request_func(
             url,
             json=body,
             headers={
                 "Content-Type": "application/json",
                 "Authorization": f"Bearer {self.api_key}",
                 "User-Agent": USER_AGENT,
             },
             timeout=timeout,
         )
-        if rsp.status_code != 200:
+        if rsp.status_code < 200 or rsp.status_code > 299:
             raise ResponseError(rsp)
-        return rsp.json()
+        if len(rsp.content) != 0:
+            return rsp.json()
```

### Comparing `gradient_labs-0.4.0/gradient_labs/types.py` & `gradient_labs-0.5.0/gradient_labs/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 class ParticipantType(str, Enum):
 
     """A participant type identifies the type of user who has
     sent a message in a conversation."""
 
     CUSTOMER: str = "Customer"
     HUMAN_AGENT: str = "Agent"
+    AI_AGENT: str = "AI Agent"
     BOT: str = "Bot"
 
 
 class ConversationChannel(str, Enum):
 
     """A channel identifies how the customer has gotten
     in touch with customer support."""
```

### Comparing `gradient_labs-0.4.0/gradient_labs/webhook.py` & `gradient_labs-0.5.0/gradient_labs/webhook.py`

 * *Files identical despite different names*

### Comparing `gradient_labs-0.4.0/PKG-INFO` & `gradient_labs-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradient-labs
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python bindings for the Gradient Labs API
 Author: Gradient Labs
 Author-email: python-client@gradient-labs.ai
 Requires-Python: >=3.8,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

