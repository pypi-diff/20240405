# Comparing `tmp/eskiz_sms_client-1.0.3.tar.gz` & `tmp/eskiz_sms_client-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eskiz_sms_client-1.0.3.tar", max compression
+gzip compressed data, was "eskiz_sms_client-1.0.4.tar", max compression
```

## Comparing `eskiz_sms_client-1.0.3.tar` & `eskiz_sms_client-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1055 2024-02-29 08:59:14.532692 eskiz_sms_client-1.0.3/LICENSE
--rw-r--r--   0        0        0     2043 2024-02-29 08:59:14.532692 eskiz_sms_client-1.0.3/README.md
--rw-r--r--   0        0        0      198 2024-02-29 08:59:14.532692 eskiz_sms_client-1.0.3/eskiz/__init__.py
--rw-r--r--   0        0        0    16049 2024-02-29 08:59:14.532692 eskiz_sms_client-1.0.3/eskiz/api.py
--rw-r--r--   0        0        0      493 2024-02-29 08:59:14.532692 eskiz_sms_client-1.0.3/eskiz/types/__init__.py
--rw-r--r--   0        0        0      196 2024-02-29 08:59:14.532692 eskiz_sms_client-1.0.3/eskiz/types/base.py
--rw-r--r--   0        0        0      520 2024-02-29 08:59:14.532692 eskiz_sms_client-1.0.3/eskiz/types/enums.py
--rw-r--r--   0        0        0     2181 2024-02-29 08:59:14.532692 eskiz_sms_client-1.0.3/eskiz/types/sms.py
--rw-r--r--   0        0        0      834 2024-02-29 08:59:14.532692 eskiz_sms_client-1.0.3/eskiz/types/template.py
--rw-r--r--   0        0        0      169 2024-02-29 08:59:14.532692 eskiz_sms_client-1.0.3/eskiz/types/token.py
--rw-r--r--   0        0        0      442 2024-02-29 08:59:14.532692 eskiz_sms_client-1.0.3/eskiz/types/user.py
--rw-r--r--   0        0        0        0 2024-02-29 08:59:14.536692 eskiz_sms_client-1.0.3/eskiz/utils/__init__.py
--rw-r--r--   0        0        0     1234 2024-02-29 08:59:14.536692 eskiz_sms_client-1.0.3/eskiz/utils/exceptions.py
--rw-r--r--   0        0        0      881 2024-02-29 08:59:14.536692 eskiz_sms_client-1.0.3/eskiz/utils/fields.py
--rw-r--r--   0        0        0      930 2024-02-29 08:59:14.536692 eskiz_sms_client-1.0.3/eskiz/utils/message.py
--rw-r--r--   0        0        0     1256 2024-02-29 08:59:14.536692 eskiz_sms_client-1.0.3/eskiz/utils/methods.py
--rw-r--r--   0        0        0      425 2024-02-29 08:59:14.536692 eskiz_sms_client-1.0.3/eskiz/utils/sync.py
--rw-r--r--   0        0        0     1544 2024-02-29 08:59:14.536692 eskiz_sms_client-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     3164 1970-01-01 00:00:00.000000 eskiz_sms_client-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1055 2024-04-05 13:14:44.990953 eskiz_sms_client-1.0.4/LICENSE
+-rw-r--r--   0        0        0     2134 2024-04-05 13:14:44.990953 eskiz_sms_client-1.0.4/README.md
+-rw-r--r--   0        0        0      198 2024-04-05 13:14:44.994953 eskiz_sms_client-1.0.4/eskiz/__init__.py
+-rw-r--r--   0        0        0    16431 2024-04-05 13:14:44.994953 eskiz_sms_client-1.0.4/eskiz/api.py
+-rw-r--r--   0        0        0      493 2024-04-05 13:14:44.994953 eskiz_sms_client-1.0.4/eskiz/types/__init__.py
+-rw-r--r--   0        0        0      196 2024-04-05 13:14:44.994953 eskiz_sms_client-1.0.4/eskiz/types/base.py
+-rw-r--r--   0        0        0      520 2024-04-05 13:14:44.994953 eskiz_sms_client-1.0.4/eskiz/types/enums.py
+-rw-r--r--   0        0        0     2181 2024-04-05 13:14:44.994953 eskiz_sms_client-1.0.4/eskiz/types/sms.py
+-rw-r--r--   0        0        0      834 2024-04-05 13:14:44.994953 eskiz_sms_client-1.0.4/eskiz/types/template.py
+-rw-r--r--   0        0        0      169 2024-04-05 13:14:44.994953 eskiz_sms_client-1.0.4/eskiz/types/token.py
+-rw-r--r--   0        0        0      442 2024-04-05 13:14:44.994953 eskiz_sms_client-1.0.4/eskiz/types/user.py
+-rw-r--r--   0        0        0        0 2024-04-05 13:14:44.994953 eskiz_sms_client-1.0.4/eskiz/utils/__init__.py
+-rw-r--r--   0        0        0     1309 2024-04-05 13:14:44.994953 eskiz_sms_client-1.0.4/eskiz/utils/exceptions.py
+-rw-r--r--   0        0        0      881 2024-04-05 13:14:44.994953 eskiz_sms_client-1.0.4/eskiz/utils/fields.py
+-rw-r--r--   0        0        0      930 2024-04-05 13:14:44.994953 eskiz_sms_client-1.0.4/eskiz/utils/message.py
+-rw-r--r--   0        0        0     1256 2024-04-05 13:14:44.994953 eskiz_sms_client-1.0.4/eskiz/utils/methods.py
+-rw-r--r--   0        0        0      425 2024-04-05 13:14:44.994953 eskiz_sms_client-1.0.4/eskiz/utils/sync.py
+-rw-r--r--   0        0        0     1544 2024-04-05 13:14:44.994953 eskiz_sms_client-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3255 1970-01-01 00:00:00.000000 eskiz_sms_client-1.0.4/PKG-INFO
```

### Comparing `eskiz_sms_client-1.0.3/LICENSE` & `eskiz_sms_client-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eskiz_sms_client-1.0.3/README.md` & `eskiz_sms_client-1.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,17 @@
   await client.get_token('test@eskiz.uz', 'password')
 
   print(client.token) # NEW TOKEN
 
 asyncio.run(main())
 ```
 
+> [!TIP]
+> Enable `SMSClient(log_response=True)`; all responses will be logged on stdout.
+
 Example for refresh token:
 
 ```py
 if client.token.is_expired:
   await client.refresh_token()
 
 print(client.token) # REFRESHED TOKEN
```

### Comparing `eskiz_sms_client-1.0.3/eskiz/api.py` & `eskiz_sms_client-1.0.4/eskiz/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import contextlib
+import logging
 import ssl
 from contextvars import ContextVar
 from datetime import datetime
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import aiohttp
 import certifi
@@ -60,14 +61,15 @@
 class SMSClient:
     __context_token: ContextVar = ContextVar("EskizBearerToken")
 
     def __init__(
         self,
         token: Optional[str] = None,
         as_dict: bool = False,
+        log_response: bool = False,
         service_url: str = SERVICE_URL,
         connections_limit: int = 100,
         loop: Optional[asyncio.AbstractEventLoop] = None,
         json_serialize: Optional[Callable[..., Any]] = None,
         json_deserialize: Optional[Callable[..., Any]] = None,
     ):
         # Asyncio loop instance
@@ -106,14 +108,23 @@
         self.session = aiohttp.ClientSession(
             connector=connector, loop=self.loop, json_serialize=json_serialize
         )
 
         self._token = token
         self.as_dict = as_dict
 
+        self.log_response = log_response
+
+        if log_response:
+            logging.basicConfig(
+                encoding="utf-8",
+                level=logging.INFO,
+                format="%(asctime)s - %(levelname)s - %(message)s",
+            )
+
     @property
     def service(self):
         return self._service
 
     @service.setter
     def service(self, value: str):
         if "." not in value or "://" in value:
@@ -154,20 +165,23 @@
             url=url,
             data=payload,
             headers=headers,
         ) as response:
 
             json_data = await response.json(loads=self._json_deserialize)
 
+            if self.log_response:
+                logging.info(str(json_data))
+
             if "status" in json_data and json_data["status"] == "fail":
                 error_text = json_data["data"]["alert"]
                 await self.handle_error(error_text)
 
             if len(json_data) == 1 and "message" in json_data:
-                await self.handle_error("BEARER_TOKEN_INVALID")
+                await self.handle_error("AUTH_CREDS_INVALID")
 
         return json_data
 
     @property
     def token(self) -> Token:
         return Token(self.__context_token.get(None) or self._token)
```

### Comparing `eskiz_sms_client-1.0.3/eskiz/types/enums.py` & `eskiz_sms_client-1.0.4/eskiz/types/enums.py`

 * *Files identical despite different names*

### Comparing `eskiz_sms_client-1.0.3/eskiz/types/sms.py` & `eskiz_sms_client-1.0.4/eskiz/types/sms.py`

 * *Files identical despite different names*

### Comparing `eskiz_sms_client-1.0.3/eskiz/types/template.py` & `eskiz_sms_client-1.0.4/eskiz/types/template.py`

 * *Files identical despite different names*

### Comparing `eskiz_sms_client-1.0.3/eskiz/utils/exceptions.py` & `eskiz_sms_client-1.0.4/eskiz/utils/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,18 @@
                 continue
             if err.match in match:
                 raise err(err.get_text() or description)
 
         raise cls(description)
 
 
+class AuthCredsInvalid(EskizError, match="AUTH_CREDS_INVALID"):
+    pass
+
+
 class BearerTokenInvalid(EskizError, match="BEARER_TOKEN_INVALID"):
     pass
 
 
 class FieldsFormatInvalid(EskizError, match="FIELDS_FORMAT_INVALID"):
     pass
```

### Comparing `eskiz_sms_client-1.0.3/eskiz/utils/fields.py` & `eskiz_sms_client-1.0.4/eskiz/utils/fields.py`

 * *Files identical despite different names*

### Comparing `eskiz_sms_client-1.0.3/eskiz/utils/message.py` & `eskiz_sms_client-1.0.4/eskiz/utils/message.py`

 * *Files identical despite different names*

### Comparing `eskiz_sms_client-1.0.3/eskiz/utils/methods.py` & `eskiz_sms_client-1.0.4/eskiz/utils/methods.py`

 * *Files identical despite different names*

### Comparing `eskiz_sms_client-1.0.3/pyproject.toml` & `eskiz_sms_client-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [tool.mypy]
 warn_return_any = false
 warn_unused_configs = true
 
 [tool.poetry]
 name = "eskiz-sms-client"
 packages = [{ include = "eskiz" }]
-version = "1.0.3"
+version = "1.0.4"
 description = "Async/Sync Python SDK of Eskiz.uz SMS Gateway"
 authors = ["hoosnick <hoosnick@morphix.uz>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["eskiz-sms", "eskiz", "eskiz-sms-client", "eskiz.uz"]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `eskiz_sms_client-1.0.3/PKG-INFO` & `eskiz_sms_client-1.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eskiz-sms-client
-Version: 1.0.3
+Version: 1.0.4
 Summary: Async/Sync Python SDK of Eskiz.uz SMS Gateway
 License: MIT
 Keywords: eskiz-sms,eskiz,eskiz-sms-client,eskiz.uz
 Author: hoosnick
 Author-email: hoosnick@morphix.uz
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -68,14 +68,17 @@
   await client.get_token('test@eskiz.uz', 'password')
 
   print(client.token) # NEW TOKEN
 
 asyncio.run(main())
 ```
 
+> [!TIP]
+> Enable `SMSClient(log_response=True)`; all responses will be logged on stdout.
+
 Example for refresh token:
 
 ```py
 if client.token.is_expired:
   await client.refresh_token()
 
 print(client.token) # REFRESHED TOKEN
```

