# Comparing `tmp/retell_sdk-3.3.0.tar.gz` & `tmp/retell_sdk-3.4.0.tar.gz`

## Comparing `retell_sdk-3.3.0.tar` & `retell_sdk-3.4.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/__init__.py
--rw-r--r--   0        0        0    62533 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/_base_client.py
--rw-r--r--   0        0        0    15012 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/_constants.py
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/_files.py
--rw-r--r--   0        0        0    22361 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/_qs.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/_resource.py
--rw-r--r--   0        0        0    28375 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/_response.py
--rw-r--r--   0        0        0     9104 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/_streaming.py
--rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/_types.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/py.typed
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/_utils/__init__.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/_utils/_logs.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/_utils/_typing.py
--rw-r--r--   0        0        0    11105 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/lib/.keep
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/resources/__init__.py
--rw-r--r--   0        0        0    41849 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/resources/agent.py
--rw-r--r--   0        0        0    25014 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/resources/call.py
--rw-r--r--   0        0        0    23757 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/resources/llm.py
--rw-r--r--   0        0        0    17883 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/resources/phone_number.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/types/__init__.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/types/agent_create_params.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/types/agent_list_response.py
--rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/types/agent_response.py
--rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/types/agent_update_params.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/types/call_create_params.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/types/call_list_params.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/types/call_list_response.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/types/call_register_params.py
--rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/types/call_response.py
--rw-r--r--   0        0        0    15574 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/types/llm_create_params.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/types/llm_list_response.py
--rw-r--r--   0        0        0    15654 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/types/llm_response.py
--rw-r--r--   0        0        0    15574 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/types/llm_update_params.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/types/phone_number_create_params.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/types/phone_number_list_response.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/types/phone_number_response.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/types/phone_number_update_params.py
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell/types/register_call_response.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell_ai/lib/.keep
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/retell_sdk/lib/.keep
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/src/toddlzt/lib/.keep
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/.gitignore
--rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/LICENSE
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/pyproject.toml
--rw-r--r--   0        0        0    11968 2020-02-02 00:00:00.000000 retell_sdk-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/__init__.py
+-rw-r--r--   0        0        0    62887 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_base_client.py
+-rw-r--r--   0        0        0    15012 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_constants.py
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_files.py
+-rw-r--r--   0        0        0    22489 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_qs.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_resource.py
+-rw-r--r--   0        0        0    28375 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_response.py
+-rw-r--r--   0        0        0    10100 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_streaming.py
+-rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_types.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/py.typed
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_utils/__init__.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_utils/_logs.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_utils/_typing.py
+-rw-r--r--   0        0        0    11105 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/lib/.keep
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/resources/__init__.py
+-rw-r--r--   0        0        0    39853 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/resources/agent.py
+-rw-r--r--   0        0        0    25014 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/resources/call.py
+-rw-r--r--   0        0        0    25717 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/resources/llm.py
+-rw-r--r--   0        0        0    17883 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/resources/phone_number.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/__init__.py
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/agent_create_params.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/agent_list_response.py
+-rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/agent_response.py
+-rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/agent_update_params.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/call_create_params.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/call_list_params.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/call_list_response.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/call_register_params.py
+-rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/call_response.py
+-rw-r--r--   0        0        0    17004 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/llm_create_params.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/llm_list_response.py
+-rw-r--r--   0        0        0    17091 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/llm_response.py
+-rw-r--r--   0        0        0    17004 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/llm_update_params.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/phone_number_create_params.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/phone_number_list_response.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/phone_number_response.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/phone_number_update_params.py
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/register_call_response.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell_ai/lib/.keep
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell_sdk/lib/.keep
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/toddlzt/lib/.keep
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/.gitignore
+-rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/LICENSE
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/pyproject.toml
+-rw-r--r--   0        0        0    11985 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/PKG-INFO
```

### Comparing `retell_sdk-3.3.0/src/retell/__init__.py` & `retell_sdk-3.4.0/src/retell/__init__.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/src/retell/_base_client.py` & `retell_sdk-3.4.0/src/retell/_base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,14 +356,19 @@
         self._proxies = proxies
         self._transport = transport
         self._custom_headers = custom_headers or {}
         self._custom_query = custom_query or {}
         self._strict_response_validation = _strict_response_validation
         self._idempotency_header = None
 
+        if max_retries is None:  # pyright: ignore[reportUnnecessaryComparison]
+            raise TypeError(
+                "max_retries cannot be None. If you want to disable retries, pass `0`; if you want unlimited retries, pass `math.inf` or a very high number; if you want the default behavior, pass `retell-sdk.DEFAULT_MAX_RETRIES`"
+            )
+
     def _enforce_trailing_slash(self, url: URL) -> URL:
         if url.raw_path.endswith(b"/"):
             return url
         return url.copy_with(raw_path=url.raw_path + b"/")
 
     def _make_status_error_from_response(
         self,
```

### Comparing `retell_sdk-3.3.0/src/retell/_client.py` & `retell_sdk-3.4.0/src/retell/_client.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/src/retell/_compat.py` & `retell_sdk-3.4.0/src/retell/_compat.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/src/retell/_exceptions.py` & `retell_sdk-3.4.0/src/retell/_exceptions.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/src/retell/_files.py` & `retell_sdk-3.4.0/src/retell/_files.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/src/retell/_models.py` & `retell_sdk-3.4.0/src/retell/_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import os
 import inspect
 from typing import TYPE_CHECKING, Any, Type, Union, Generic, TypeVar, Callable, cast
 from datetime import date, datetime
 from functools import lru_cache
 from typing_extensions import (
     Unpack,
     Literal,
@@ -34,14 +35,15 @@
 )
 from ._utils import (
     PropertyInfo,
     is_list,
     is_given,
     is_mapping,
     parse_date,
+    coerce_boolean,
     parse_datetime,
     strip_not_given,
     extract_type_arg,
     is_annotated_type,
     strip_annotated_type,
 )
 from ._compat import (
@@ -70,15 +72,17 @@
 @runtime_checkable
 class _ConfigProtocol(Protocol):
     allow_population_by_field_name: bool
 
 
 class BaseModel(pydantic.BaseModel):
     if PYDANTIC_V2:
-        model_config: ClassVar[ConfigDict] = ConfigDict(extra="allow")
+        model_config: ClassVar[ConfigDict] = ConfigDict(
+            extra="allow", defer_build=coerce_boolean(os.environ.get("DEFER_PYDANTIC_BUILD", "true"))
+        )
     else:
 
         @property
         @override
         def model_fields_set(self) -> set[str]:
             # a forwards-compat shim for pydantic v2
             return self.__fields_set__  # type: ignore
```

### Comparing `retell_sdk-3.3.0/src/retell/_qs.py` & `retell_sdk-3.4.0/src/retell/_qs.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/src/retell/_resource.py` & `retell_sdk-3.4.0/src/retell/_resource.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/src/retell/_response.py` & `retell_sdk-3.4.0/src/retell/_response.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/src/retell/_streaming.py` & `retell_sdk-3.4.0/src/retell/_streaming.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 class Stream(Generic[_T]):
     """Provides the core interface to iterate over a synchronous stream response."""
 
     response: httpx.Response
 
-    _decoder: SSEDecoder | SSEBytesDecoder
+    _decoder: SSEBytesDecoder
 
     def __init__(
         self,
         *,
         cast_to: type[_T],
         response: httpx.Response,
         client: Retell,
@@ -42,18 +42,15 @@
         return self._iterator.__next__()
 
     def __iter__(self) -> Iterator[_T]:
         for item in self._iterator:
             yield item
 
     def _iter_events(self) -> Iterator[ServerSentEvent]:
-        if isinstance(self._decoder, SSEBytesDecoder):
-            yield from self._decoder.iter_bytes(self.response.iter_bytes())
-        else:
-            yield from self._decoder.iter(self.response.iter_lines())
+        yield from self._decoder.iter_bytes(self.response.iter_bytes())
 
     def __stream__(self) -> Iterator[_T]:
         cast_to = cast(Any, self._cast_to)
         response = self.response
         process_data = self._client._process_response_data
         iterator = self._iter_events()
 
@@ -108,20 +105,16 @@
         return await self._iterator.__anext__()
 
     async def __aiter__(self) -> AsyncIterator[_T]:
         async for item in self._iterator:
             yield item
 
     async def _iter_events(self) -> AsyncIterator[ServerSentEvent]:
-        if isinstance(self._decoder, SSEBytesDecoder):
-            async for sse in self._decoder.aiter_bytes(self.response.aiter_bytes()):
-                yield sse
-        else:
-            async for sse in self._decoder.aiter(self.response.aiter_lines()):
-                yield sse
+        async for sse in self._decoder.aiter_bytes(self.response.aiter_bytes()):
+            yield sse
 
     async def __stream__(self) -> AsyncIterator[_T]:
         cast_to = cast(Any, self._cast_to)
         response = self.response
         process_data = self._client._process_response_data
         iterator = self._iter_events()
 
@@ -201,29 +194,57 @@
 
     def __init__(self) -> None:
         self._event = None
         self._data = []
         self._last_event_id = None
         self._retry = None
 
-    def iter(self, iterator: Iterator[str]) -> Iterator[ServerSentEvent]:
-        """Given an iterator that yields lines, iterate over it & yield every event encountered"""
-        for line in iterator:
-            line = line.rstrip("\n")
-            sse = self.decode(line)
-            if sse is not None:
-                yield sse
-
-    async def aiter(self, iterator: AsyncIterator[str]) -> AsyncIterator[ServerSentEvent]:
-        """Given an async iterator that yields lines, iterate over it & yield every event encountered"""
-        async for line in iterator:
-            line = line.rstrip("\n")
-            sse = self.decode(line)
-            if sse is not None:
-                yield sse
+    def iter_bytes(self, iterator: Iterator[bytes]) -> Iterator[ServerSentEvent]:
+        """Given an iterator that yields raw binary data, iterate over it & yield every event encountered"""
+        for chunk in self._iter_chunks(iterator):
+            # Split before decoding so splitlines() only uses \r and \n
+            for raw_line in chunk.splitlines():
+                line = raw_line.decode("utf-8")
+                sse = self.decode(line)
+                if sse:
+                    yield sse
+
+    def _iter_chunks(self, iterator: Iterator[bytes]) -> Iterator[bytes]:
+        """Given an iterator that yields raw binary data, iterate over it and yield individual SSE chunks"""
+        data = b""
+        for chunk in iterator:
+            for line in chunk.splitlines(keepends=True):
+                data += line
+                if data.endswith((b"\r\r", b"\n\n", b"\r\n\r\n")):
+                    yield data
+                    data = b""
+        if data:
+            yield data
+
+    async def aiter_bytes(self, iterator: AsyncIterator[bytes]) -> AsyncIterator[ServerSentEvent]:
+        """Given an iterator that yields raw binary data, iterate over it & yield every event encountered"""
+        async for chunk in self._aiter_chunks(iterator):
+            # Split before decoding so splitlines() only uses \r and \n
+            for raw_line in chunk.splitlines():
+                line = raw_line.decode("utf-8")
+                sse = self.decode(line)
+                if sse:
+                    yield sse
+
+    async def _aiter_chunks(self, iterator: AsyncIterator[bytes]) -> AsyncIterator[bytes]:
+        """Given an iterator that yields raw binary data, iterate over it and yield individual SSE chunks"""
+        data = b""
+        async for chunk in iterator:
+            for line in chunk.splitlines(keepends=True):
+                data += line
+                if data.endswith((b"\r\r", b"\n\n", b"\r\n\r\n")):
+                    yield data
+                    data = b""
+        if data:
+            yield data
 
     def decode(self, line: str) -> ServerSentEvent | None:
         # See: https://html.spec.whatwg.org/multipage/server-sent-events.html#event-stream-interpretation  # noqa: E501
 
         if not line:
             if not self._event and not self._data and not self._last_event_id and self._retry is None:
                 return None
```

### Comparing `retell_sdk-3.3.0/src/retell/_types.py` & `retell_sdk-3.4.0/src/retell/_types.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/src/retell/_utils/__init__.py` & `retell_sdk-3.4.0/src/retell/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/src/retell/_utils/_logs.py` & `retell_sdk-3.4.0/src/retell/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/src/retell/_utils/_proxy.py` & `retell_sdk-3.4.0/src/retell/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/src/retell/_utils/_sync.py` & `retell_sdk-3.4.0/src/retell/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/src/retell/_utils/_transform.py` & `retell_sdk-3.4.0/src/retell/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/src/retell/_utils/_typing.py` & `retell_sdk-3.4.0/src/retell/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/src/retell/_utils/_utils.py` & `retell_sdk-3.4.0/src/retell/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/src/retell/resources/__init__.py` & `retell_sdk-3.4.0/src/retell/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/src/retell/resources/agent.py` & `retell_sdk-3.4.0/src/retell/resources/agent.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,15 +43,14 @@
         llm_websocket_url: str,
         voice_id: str,
         agent_name: Optional[str] | NotGiven = NOT_GIVEN,
         ambient_sound: Optional[Literal["coffee-shop", "convention-hall", "summer-outdoor", "mountain-outdoor"]]
         | NotGiven = NOT_GIVEN,
         boosted_keywords: Optional[List[str]] | NotGiven = NOT_GIVEN,
         enable_backchannel: bool | NotGiven = NOT_GIVEN,
-        format_text: bool | NotGiven = NOT_GIVEN,
         language: Literal["en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR"]
         | NotGiven = NOT_GIVEN,
         opt_out_sensitive_data_storage: bool | NotGiven = NOT_GIVEN,
         responsiveness: float | NotGiven = NOT_GIVEN,
         voice_speed: float | NotGiven = NOT_GIVEN,
         voice_temperature: float | NotGiven = NOT_GIVEN,
         webhook_url: Optional[str] | NotGiven = NOT_GIVEN,
@@ -98,20 +97,14 @@
               street, etc.
 
           enable_backchannel: Controls whether the agent would backchannel (agent interjects the speaker with
               phrases like "yeah", "uh-huh" to signify interest and engagement). Backchannel
               when enabled tends to show up more in longer user utterances. If not set, agent
               will not backchannel.
 
-          format_text: Whether to format the transcribed text with inverse text normalization. It
-              transforms the spoken form of text into written form for entities like phone
-              number, email address, street address, etc. For example, "february fourth twenty
-              twenty two" can be converted into "february 4th 2022". If not set, the default
-              is true.
-
           language: `Beta feature, use with caution.`
 
               This setting specifies the agent's operational language, including base language
               and dialect. Speech recognition considers both elements, but text-to-speech
               currently only recognizes the base language.
 
               For instance, selecting `en-GB` optimizes speech recognition for British
@@ -165,15 +158,14 @@
                 {
                     "llm_websocket_url": llm_websocket_url,
                     "voice_id": voice_id,
                     "agent_name": agent_name,
                     "ambient_sound": ambient_sound,
                     "boosted_keywords": boosted_keywords,
                     "enable_backchannel": enable_backchannel,
-                    "format_text": format_text,
                     "language": language,
                     "opt_out_sensitive_data_storage": opt_out_sensitive_data_storage,
                     "responsiveness": responsiveness,
                     "voice_speed": voice_speed,
                     "voice_temperature": voice_temperature,
                     "webhook_url": webhook_url,
                 },
@@ -223,15 +215,14 @@
         agent_id: str,
         *,
         agent_name: Optional[str] | NotGiven = NOT_GIVEN,
         ambient_sound: Optional[Literal["coffee-shop", "convention-hall", "summer-outdoor", "mountain-outdoor"]]
         | NotGiven = NOT_GIVEN,
         boosted_keywords: Optional[List[str]] | NotGiven = NOT_GIVEN,
         enable_backchannel: bool | NotGiven = NOT_GIVEN,
-        format_text: bool | NotGiven = NOT_GIVEN,
         language: Literal["en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR"]
         | NotGiven = NOT_GIVEN,
         llm_websocket_url: str | NotGiven = NOT_GIVEN,
         opt_out_sensitive_data_storage: bool | NotGiven = NOT_GIVEN,
         responsiveness: float | NotGiven = NOT_GIVEN,
         voice_id: str | NotGiven = NOT_GIVEN,
         voice_speed: float | NotGiven = NOT_GIVEN,
@@ -274,20 +265,14 @@
               street, etc.
 
           enable_backchannel: Controls whether the agent would backchannel (agent interjects the speaker with
               phrases like "yeah", "uh-huh" to signify interest and engagement). Backchannel
               when enabled tends to show up more in longer user utterances. If not set, agent
               will not backchannel.
 
-          format_text: Whether to format the transcribed text with inverse text normalization. It
-              transforms the spoken form of text into written form for entities like phone
-              number, email address, street address, etc. For example, "february fourth twenty
-              twenty two" can be converted into "february 4th 2022". If not set, the default
-              is true.
-
           language: `Beta feature, use with caution.`
 
               This setting specifies the agent's operational language, including base language
               and dialect. Speech recognition considers both elements, but text-to-speech
               currently only recognizes the base language.
 
               For instance, selecting `en-GB` optimizes speech recognition for British
@@ -348,15 +333,14 @@
             f"/update-agent/{agent_id}",
             body=maybe_transform(
                 {
                     "agent_name": agent_name,
                     "ambient_sound": ambient_sound,
                     "boosted_keywords": boosted_keywords,
                     "enable_backchannel": enable_backchannel,
-                    "format_text": format_text,
                     "language": language,
                     "llm_websocket_url": llm_websocket_url,
                     "opt_out_sensitive_data_storage": opt_out_sensitive_data_storage,
                     "responsiveness": responsiveness,
                     "voice_id": voice_id,
                     "voice_speed": voice_speed,
                     "voice_temperature": voice_temperature,
@@ -439,15 +423,14 @@
         llm_websocket_url: str,
         voice_id: str,
         agent_name: Optional[str] | NotGiven = NOT_GIVEN,
         ambient_sound: Optional[Literal["coffee-shop", "convention-hall", "summer-outdoor", "mountain-outdoor"]]
         | NotGiven = NOT_GIVEN,
         boosted_keywords: Optional[List[str]] | NotGiven = NOT_GIVEN,
         enable_backchannel: bool | NotGiven = NOT_GIVEN,
-        format_text: bool | NotGiven = NOT_GIVEN,
         language: Literal["en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR"]
         | NotGiven = NOT_GIVEN,
         opt_out_sensitive_data_storage: bool | NotGiven = NOT_GIVEN,
         responsiveness: float | NotGiven = NOT_GIVEN,
         voice_speed: float | NotGiven = NOT_GIVEN,
         voice_temperature: float | NotGiven = NOT_GIVEN,
         webhook_url: Optional[str] | NotGiven = NOT_GIVEN,
@@ -494,20 +477,14 @@
               street, etc.
 
           enable_backchannel: Controls whether the agent would backchannel (agent interjects the speaker with
               phrases like "yeah", "uh-huh" to signify interest and engagement). Backchannel
               when enabled tends to show up more in longer user utterances. If not set, agent
               will not backchannel.
 
-          format_text: Whether to format the transcribed text with inverse text normalization. It
-              transforms the spoken form of text into written form for entities like phone
-              number, email address, street address, etc. For example, "february fourth twenty
-              twenty two" can be converted into "february 4th 2022". If not set, the default
-              is true.
-
           language: `Beta feature, use with caution.`
 
               This setting specifies the agent's operational language, including base language
               and dialect. Speech recognition considers both elements, but text-to-speech
               currently only recognizes the base language.
 
               For instance, selecting `en-GB` optimizes speech recognition for British
@@ -561,15 +538,14 @@
                 {
                     "llm_websocket_url": llm_websocket_url,
                     "voice_id": voice_id,
                     "agent_name": agent_name,
                     "ambient_sound": ambient_sound,
                     "boosted_keywords": boosted_keywords,
                     "enable_backchannel": enable_backchannel,
-                    "format_text": format_text,
                     "language": language,
                     "opt_out_sensitive_data_storage": opt_out_sensitive_data_storage,
                     "responsiveness": responsiveness,
                     "voice_speed": voice_speed,
                     "voice_temperature": voice_temperature,
                     "webhook_url": webhook_url,
                 },
@@ -619,15 +595,14 @@
         agent_id: str,
         *,
         agent_name: Optional[str] | NotGiven = NOT_GIVEN,
         ambient_sound: Optional[Literal["coffee-shop", "convention-hall", "summer-outdoor", "mountain-outdoor"]]
         | NotGiven = NOT_GIVEN,
         boosted_keywords: Optional[List[str]] | NotGiven = NOT_GIVEN,
         enable_backchannel: bool | NotGiven = NOT_GIVEN,
-        format_text: bool | NotGiven = NOT_GIVEN,
         language: Literal["en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR"]
         | NotGiven = NOT_GIVEN,
         llm_websocket_url: str | NotGiven = NOT_GIVEN,
         opt_out_sensitive_data_storage: bool | NotGiven = NOT_GIVEN,
         responsiveness: float | NotGiven = NOT_GIVEN,
         voice_id: str | NotGiven = NOT_GIVEN,
         voice_speed: float | NotGiven = NOT_GIVEN,
@@ -670,20 +645,14 @@
               street, etc.
 
           enable_backchannel: Controls whether the agent would backchannel (agent interjects the speaker with
               phrases like "yeah", "uh-huh" to signify interest and engagement). Backchannel
               when enabled tends to show up more in longer user utterances. If not set, agent
               will not backchannel.
 
-          format_text: Whether to format the transcribed text with inverse text normalization. It
-              transforms the spoken form of text into written form for entities like phone
-              number, email address, street address, etc. For example, "february fourth twenty
-              twenty two" can be converted into "february 4th 2022". If not set, the default
-              is true.
-
           language: `Beta feature, use with caution.`
 
               This setting specifies the agent's operational language, including base language
               and dialect. Speech recognition considers both elements, but text-to-speech
               currently only recognizes the base language.
 
               For instance, selecting `en-GB` optimizes speech recognition for British
@@ -744,15 +713,14 @@
             f"/update-agent/{agent_id}",
             body=await async_maybe_transform(
                 {
                     "agent_name": agent_name,
                     "ambient_sound": ambient_sound,
                     "boosted_keywords": boosted_keywords,
                     "enable_backchannel": enable_backchannel,
-                    "format_text": format_text,
                     "language": language,
                     "llm_websocket_url": llm_websocket_url,
                     "opt_out_sensitive_data_storage": opt_out_sensitive_data_storage,
                     "responsiveness": responsiveness,
                     "voice_id": voice_id,
                     "voice_speed": voice_speed,
                     "voice_temperature": voice_temperature,
```

### Comparing `retell_sdk-3.3.0/src/retell/resources/call.py` & `retell_sdk-3.4.0/src/retell/resources/call.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/src/retell/resources/llm.py` & `retell_sdk-3.4.0/src/retell/resources/llm.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
     def create(
         self,
         *,
         begin_message: Optional[str] | NotGiven = NOT_GIVEN,
         general_prompt: Optional[str] | NotGiven = NOT_GIVEN,
         general_tools: Optional[Iterable[llm_create_params.GeneralTool]] | NotGiven = NOT_GIVEN,
+        inbound_dynamic_variables_webhook_url: Optional[str] | NotGiven = NOT_GIVEN,
         starting_state: Optional[str] | NotGiven = NOT_GIVEN,
         states: Optional[Iterable[llm_create_params.State]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
@@ -68,14 +69,18 @@
               You can select from some common predefined tools like end call, transfer call,
               etc; or you can create your own custom tool (last option) for the LLM to use.
 
               - Tools of LLM (with state) = general tools + state tools + state transitions
 
               - Tools of LLM (no state) = general tools
 
+          inbound_dynamic_variables_webhook_url: For inbound phone calls with Retell numbers, if this webhook is set, will POST
+              to it to retrieve dynamic variables to use for the call. Without this, there's
+              no way to pass dynamic variables to inbound calls of Retell numbers.
+
           starting_state: Name of the starting state. Required if states is not empty.
 
           states: States of the LLM. This is to help reduce prompt length and tool choices when
               the call can be broken into distinct states. With shorter prompts and less
               tools, the LLM can better focus and follow the rules, minimizing hallucination.
               If this field is not set, the agent would only have general prompt and general
               tools (essentially one state).
@@ -91,14 +96,15 @@
         return self._post(
             "/create-retell-llm",
             body=maybe_transform(
                 {
                     "begin_message": begin_message,
                     "general_prompt": general_prompt,
                     "general_tools": general_tools,
+                    "inbound_dynamic_variables_webhook_url": inbound_dynamic_variables_webhook_url,
                     "starting_state": starting_state,
                     "states": states,
                 },
                 llm_create_params.LlmCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
@@ -142,14 +148,15 @@
     def update(
         self,
         llm_id: str,
         *,
         begin_message: Optional[str] | NotGiven = NOT_GIVEN,
         general_prompt: Optional[str] | NotGiven = NOT_GIVEN,
         general_tools: Optional[Iterable[llm_update_params.GeneralTool]] | NotGiven = NOT_GIVEN,
+        inbound_dynamic_variables_webhook_url: Optional[str] | NotGiven = NOT_GIVEN,
         starting_state: Optional[str] | NotGiven = NOT_GIVEN,
         states: Optional[Iterable[llm_update_params.State]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
@@ -172,14 +179,18 @@
               You can select from some common predefined tools like end call, transfer call,
               etc; or you can create your own custom tool (last option) for the LLM to use.
 
               - Tools of LLM (with state) = general tools + state tools + state transitions
 
               - Tools of LLM (no state) = general tools
 
+          inbound_dynamic_variables_webhook_url: For inbound phone calls with Retell numbers, if this webhook is set, will POST
+              to it to retrieve dynamic variables to use for the call. Without this, there's
+              no way to pass dynamic variables to inbound calls of Retell numbers.
+
           starting_state: Name of the starting state. Required if states is not empty.
 
           states: States of the LLM. This is to help reduce prompt length and tool choices when
               the call can be broken into distinct states. With shorter prompts and less
               tools, the LLM can better focus and follow the rules, minimizing hallucination.
               If this field is not set, the agent would only have general prompt and general
               tools (essentially one state).
@@ -197,14 +208,15 @@
         return self._patch(
             f"/update-retell-llm/{llm_id}",
             body=maybe_transform(
                 {
                     "begin_message": begin_message,
                     "general_prompt": general_prompt,
                     "general_tools": general_tools,
+                    "inbound_dynamic_variables_webhook_url": inbound_dynamic_variables_webhook_url,
                     "starting_state": starting_state,
                     "states": states,
                 },
                 llm_update_params.LlmUpdateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
@@ -277,14 +289,15 @@
 
     async def create(
         self,
         *,
         begin_message: Optional[str] | NotGiven = NOT_GIVEN,
         general_prompt: Optional[str] | NotGiven = NOT_GIVEN,
         general_tools: Optional[Iterable[llm_create_params.GeneralTool]] | NotGiven = NOT_GIVEN,
+        inbound_dynamic_variables_webhook_url: Optional[str] | NotGiven = NOT_GIVEN,
         starting_state: Optional[str] | NotGiven = NOT_GIVEN,
         states: Optional[Iterable[llm_create_params.State]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
@@ -307,14 +320,18 @@
               You can select from some common predefined tools like end call, transfer call,
               etc; or you can create your own custom tool (last option) for the LLM to use.
 
               - Tools of LLM (with state) = general tools + state tools + state transitions
 
               - Tools of LLM (no state) = general tools
 
+          inbound_dynamic_variables_webhook_url: For inbound phone calls with Retell numbers, if this webhook is set, will POST
+              to it to retrieve dynamic variables to use for the call. Without this, there's
+              no way to pass dynamic variables to inbound calls of Retell numbers.
+
           starting_state: Name of the starting state. Required if states is not empty.
 
           states: States of the LLM. This is to help reduce prompt length and tool choices when
               the call can be broken into distinct states. With shorter prompts and less
               tools, the LLM can better focus and follow the rules, minimizing hallucination.
               If this field is not set, the agent would only have general prompt and general
               tools (essentially one state).
@@ -330,14 +347,15 @@
         return await self._post(
             "/create-retell-llm",
             body=await async_maybe_transform(
                 {
                     "begin_message": begin_message,
                     "general_prompt": general_prompt,
                     "general_tools": general_tools,
+                    "inbound_dynamic_variables_webhook_url": inbound_dynamic_variables_webhook_url,
                     "starting_state": starting_state,
                     "states": states,
                 },
                 llm_create_params.LlmCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
@@ -381,14 +399,15 @@
     async def update(
         self,
         llm_id: str,
         *,
         begin_message: Optional[str] | NotGiven = NOT_GIVEN,
         general_prompt: Optional[str] | NotGiven = NOT_GIVEN,
         general_tools: Optional[Iterable[llm_update_params.GeneralTool]] | NotGiven = NOT_GIVEN,
+        inbound_dynamic_variables_webhook_url: Optional[str] | NotGiven = NOT_GIVEN,
         starting_state: Optional[str] | NotGiven = NOT_GIVEN,
         states: Optional[Iterable[llm_update_params.State]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
@@ -411,14 +430,18 @@
               You can select from some common predefined tools like end call, transfer call,
               etc; or you can create your own custom tool (last option) for the LLM to use.
 
               - Tools of LLM (with state) = general tools + state tools + state transitions
 
               - Tools of LLM (no state) = general tools
 
+          inbound_dynamic_variables_webhook_url: For inbound phone calls with Retell numbers, if this webhook is set, will POST
+              to it to retrieve dynamic variables to use for the call. Without this, there's
+              no way to pass dynamic variables to inbound calls of Retell numbers.
+
           starting_state: Name of the starting state. Required if states is not empty.
 
           states: States of the LLM. This is to help reduce prompt length and tool choices when
               the call can be broken into distinct states. With shorter prompts and less
               tools, the LLM can better focus and follow the rules, minimizing hallucination.
               If this field is not set, the agent would only have general prompt and general
               tools (essentially one state).
@@ -436,14 +459,15 @@
         return await self._patch(
             f"/update-retell-llm/{llm_id}",
             body=await async_maybe_transform(
                 {
                     "begin_message": begin_message,
                     "general_prompt": general_prompt,
                     "general_tools": general_tools,
+                    "inbound_dynamic_variables_webhook_url": inbound_dynamic_variables_webhook_url,
                     "starting_state": starting_state,
                     "states": states,
                 },
                 llm_update_params.LlmUpdateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
```

### Comparing `retell_sdk-3.3.0/src/retell/resources/phone_number.py` & `retell_sdk-3.4.0/src/retell/resources/phone_number.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/src/retell/types/__init__.py` & `retell_sdk-3.4.0/src/retell/types/__init__.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/src/retell/types/agent_create_params.py` & `retell_sdk-3.4.0/src/retell/types/agent_update_params.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,18 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 from typing import List, Optional
-from typing_extensions import Literal, Required, TypedDict
+from typing_extensions import Literal, TypedDict
 
-__all__ = ["AgentCreateParams"]
+__all__ = ["AgentUpdateParams"]
 
 
-class AgentCreateParams(TypedDict, total=False):
-    llm_websocket_url: Required[str]
-    """
-    The URL we will establish LLM websocket for getting response, usually your
-    server. Check out [LLM WebSocket](/api-references/llm-websocket) for more about
-    request format (sent from us) and response format (send to us).
-    """
-
-    voice_id: Required[str]
-    """Unique voice id used for the agent.
-
-    Find list of available voices and their preview in Dashboard.
-    """
-
+class AgentUpdateParams(TypedDict, total=False):
     agent_name: Optional[str]
     """The name of the agent. Only used for your own reference."""
 
     ambient_sound: Optional[Literal["coffee-shop", "convention-hall", "summer-outdoor", "mountain-outdoor"]]
     """
     If set, will add ambient environment sound to the call to make experience more
     realistic. Currently supports the following options:
@@ -57,23 +44,14 @@
     """
     Controls whether the agent would backchannel (agent interjects the speaker with
     phrases like "yeah", "uh-huh" to signify interest and engagement). Backchannel
     when enabled tends to show up more in longer user utterances. If not set, agent
     will not backchannel.
     """
 
-    format_text: bool
-    """Whether to format the transcribed text with inverse text normalization.
-
-    It transforms the spoken form of text into written form for entities like phone
-    number, email address, street address, etc. For example, "february fourth twenty
-    twenty two" can be converted into "february 4th 2022". If not set, the default
-    is true.
-    """
-
     language: Literal["en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR"]
     """`Beta feature, use with caution.`
 
     This setting specifies the agent's operational language, including base language
     and dialect. Speech recognition considers both elements, but text-to-speech
     currently only recognizes the base language.
 
@@ -88,14 +66,21 @@
 
     - `openAI voices`: supports English(en), German(de), Spanish(es), Hindi(hi),
       Portuguese(pt), Japanese(ja)
 
     - `deepgram voices`: supports English(en)
     """
 
+    llm_websocket_url: str
+    """
+    The URL we will establish LLM websocket for getting response, usually your
+    server. Check out [LLM WebSocket](/api-references/llm-websocket) for more about
+    request format (sent from us) and response format (send to us).
+    """
+
     opt_out_sensitive_data_storage: bool
     """Disable transcripts and recordings storage for enhanced privacy.
 
     Access transcripts securely via webhooks. If not set, default value of false
     will apply.
     """
 
@@ -103,14 +88,20 @@
     """Controls how responsive is the agent.
 
     Value ranging from [0,1]. Lower value means less responsive agent (wait more,
     respond slower), while higher value means faster exchanges (respond when it
     can). If unset, default value 1 will apply.
     """
 
+    voice_id: str
+    """Unique voice id used for the agent.
+
+    Find list of available voices and their preview in Dashboard.
+    """
+
     voice_speed: float
     """Controls speed of voice.
 
     Value ranging from [0.5,2]. Lower value means slower speech, while higher value
     means faster speech rate. If unset, default value 1 will apply.
     """
```

### Comparing `retell_sdk-3.3.0/src/retell/types/agent_response.py` & `retell_sdk-3.4.0/src/retell/types/agent_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -66,23 +66,14 @@
     """
     Controls whether the agent would backchannel (agent interjects the speaker with
     phrases like "yeah", "uh-huh" to signify interest and engagement). Backchannel
     when enabled tends to show up more in longer user utterances. If not set, agent
     will not backchannel.
     """
 
-    format_text: Optional[bool] = None
-    """Whether to format the transcribed text with inverse text normalization.
-
-    It transforms the spoken form of text into written form for entities like phone
-    number, email address, street address, etc. For example, "february fourth twenty
-    twenty two" can be converted into "february 4th 2022". If not set, the default
-    is true.
-    """
-
     language: Optional[
         Literal["en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR"]
     ] = None
     """`Beta feature, use with caution.`
 
     This setting specifies the agent's operational language, including base language
     and dialect. Speech recognition considers both elements, but text-to-speech
```

### Comparing `retell_sdk-3.3.0/src/retell/types/agent_update_params.py` & `retell_sdk-3.4.0/src/retell/types/agent_create_params.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 from typing import List, Optional
-from typing_extensions import Literal, TypedDict
+from typing_extensions import Literal, Required, TypedDict
 
-__all__ = ["AgentUpdateParams"]
+__all__ = ["AgentCreateParams"]
 
 
-class AgentUpdateParams(TypedDict, total=False):
+class AgentCreateParams(TypedDict, total=False):
+    llm_websocket_url: Required[str]
+    """
+    The URL we will establish LLM websocket for getting response, usually your
+    server. Check out [LLM WebSocket](/api-references/llm-websocket) for more about
+    request format (sent from us) and response format (send to us).
+    """
+
+    voice_id: Required[str]
+    """Unique voice id used for the agent.
+
+    Find list of available voices and their preview in Dashboard.
+    """
+
     agent_name: Optional[str]
     """The name of the agent. Only used for your own reference."""
 
     ambient_sound: Optional[Literal["coffee-shop", "convention-hall", "summer-outdoor", "mountain-outdoor"]]
     """
     If set, will add ambient environment sound to the call to make experience more
     realistic. Currently supports the following options:
@@ -44,23 +57,14 @@
     """
     Controls whether the agent would backchannel (agent interjects the speaker with
     phrases like "yeah", "uh-huh" to signify interest and engagement). Backchannel
     when enabled tends to show up more in longer user utterances. If not set, agent
     will not backchannel.
     """
 
-    format_text: bool
-    """Whether to format the transcribed text with inverse text normalization.
-
-    It transforms the spoken form of text into written form for entities like phone
-    number, email address, street address, etc. For example, "february fourth twenty
-    twenty two" can be converted into "february 4th 2022". If not set, the default
-    is true.
-    """
-
     language: Literal["en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR"]
     """`Beta feature, use with caution.`
 
     This setting specifies the agent's operational language, including base language
     and dialect. Speech recognition considers both elements, but text-to-speech
     currently only recognizes the base language.
 
@@ -75,21 +79,14 @@
 
     - `openAI voices`: supports English(en), German(de), Spanish(es), Hindi(hi),
       Portuguese(pt), Japanese(ja)
 
     - `deepgram voices`: supports English(en)
     """
 
-    llm_websocket_url: str
-    """
-    The URL we will establish LLM websocket for getting response, usually your
-    server. Check out [LLM WebSocket](/api-references/llm-websocket) for more about
-    request format (sent from us) and response format (send to us).
-    """
-
     opt_out_sensitive_data_storage: bool
     """Disable transcripts and recordings storage for enhanced privacy.
 
     Access transcripts securely via webhooks. If not set, default value of false
     will apply.
     """
 
@@ -97,20 +94,14 @@
     """Controls how responsive is the agent.
 
     Value ranging from [0,1]. Lower value means less responsive agent (wait more,
     respond slower), while higher value means faster exchanges (respond when it
     can). If unset, default value 1 will apply.
     """
 
-    voice_id: str
-    """Unique voice id used for the agent.
-
-    Find list of available voices and their preview in Dashboard.
-    """
-
     voice_speed: float
     """Controls speed of voice.
 
     Value ranging from [0.5,2]. Lower value means slower speech, while higher value
     means faster speech rate. If unset, default value 1 will apply.
     """
```

### Comparing `retell_sdk-3.3.0/src/retell/types/call_create_params.py` & `retell_sdk-3.4.0/src/retell/types/call_create_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/src/retell/types/call_list_params.py` & `retell_sdk-3.4.0/src/retell/types/call_list_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/src/retell/types/call_register_params.py` & `retell_sdk-3.4.0/src/retell/types/call_register_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/src/retell/types/call_response.py` & `retell_sdk-3.4.0/src/retell/types/call_response.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/src/retell/types/llm_create_params.py` & `retell_sdk-3.4.0/src/retell/types/llm_update_params.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 from typing import Dict, List, Union, Iterable, Optional
 from typing_extensions import Literal, Required, TypedDict
 
 __all__ = [
-    "LlmCreateParams",
+    "LlmUpdateParams",
     "GeneralTool",
     "GeneralToolEndCallTool",
     "GeneralToolTransferCallTool",
     "GeneralToolCheckAvailabilityCalTool",
     "GeneralToolBookAppointmentCalTool",
     "GeneralToolCustomTool",
     "GeneralToolCustomToolParameters",
@@ -23,15 +23,15 @@
     "StateToolCheckAvailabilityCalTool",
     "StateToolBookAppointmentCalTool",
     "StateToolCustomTool",
     "StateToolCustomToolParameters",
 ]
 
 
-class LlmCreateParams(TypedDict, total=False):
+class LlmUpdateParams(TypedDict, total=False):
     begin_message: Optional[str]
     """First utterance said by the agent in the call.
 
     If not set, LLM will dynamically generate a message. If set to "", agent will
     wait for user to speak first.
     """
 
@@ -50,14 +50,21 @@
     etc; or you can create your own custom tool (last option) for the LLM to use.
 
     - Tools of LLM (with state) = general tools + state tools + state transitions
 
     - Tools of LLM (no state) = general tools
     """
 
+    inbound_dynamic_variables_webhook_url: Optional[str]
+    """
+    For inbound phone calls with Retell numbers, if this webhook is set, will POST
+    to it to retrieve dynamic variables to use for the call. Without this, there's
+    no way to pass dynamic variables to inbound calls of Retell numbers.
+    """
+
     starting_state: Optional[str]
     """Name of the starting state. Required if states is not empty."""
 
     states: Optional[Iterable[State]]
     """States of the LLM.
 
     This is to help reduce prompt length and tool choices when the call can be
@@ -69,15 +76,16 @@
 
 
 class GeneralToolEndCallTool(TypedDict, total=False):
     name: Required[str]
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
-    tools + state tools + state transitions).
+    tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
+    contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Required[Literal["end_call"]]
 
     description: str
     """Describes when to end the call."""
 
@@ -115,15 +123,16 @@
     availability for.
     """
 
     name: Required[str]
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
-    tools + state tools + state transitions).
+    tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
+    contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Required[Literal["check_availability_cal"]]
 
     description: str
     """Describes when to check availability."""
 
@@ -148,15 +157,16 @@
     Cal.com event type id number for the cal.com event you want to book appointment.
     """
 
     name: Required[str]
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
-    tools + state tools + state transitions).
+    tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
+    contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Required[Literal["book_appointment_cal"]]
 
     description: str
     """Describes when to book the appointment."""
 
@@ -191,15 +201,16 @@
     description: Required[str]
     """Describes what this tool does and when to call this tool."""
 
     name: Required[str]
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
-    tools + state tools + state edges).
+    tools + state tools + state edges). Must be consisted of a-z, A-Z, 0-9, or
+    contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     speak_after_execution: Required[bool]
     """
     Determines whether the agent would call LLM another time and speak when the
     result of function is obtained. Usually this needs to get turned on so user can
     get update for the function call.
@@ -292,15 +303,16 @@
 
 
 class StateToolEndCallTool(TypedDict, total=False):
     name: Required[str]
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
-    tools + state tools + state transitions).
+    tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
+    contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Required[Literal["end_call"]]
 
     description: str
     """Describes when to end the call."""
 
@@ -338,15 +350,16 @@
     availability for.
     """
 
     name: Required[str]
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
-    tools + state tools + state transitions).
+    tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
+    contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Required[Literal["check_availability_cal"]]
 
     description: str
     """Describes when to check availability."""
 
@@ -371,15 +384,16 @@
     Cal.com event type id number for the cal.com event you want to book appointment.
     """
 
     name: Required[str]
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
-    tools + state tools + state transitions).
+    tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
+    contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Required[Literal["book_appointment_cal"]]
 
     description: str
     """Describes when to book the appointment."""
 
@@ -414,15 +428,16 @@
     description: Required[str]
     """Describes what this tool does and when to call this tool."""
 
     name: Required[str]
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
-    tools + state tools + state edges).
+    tools + state tools + state edges). Must be consisted of a-z, A-Z, 0-9, or
+    contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     speak_after_execution: Required[bool]
     """
     Determines whether the agent would call LLM another time and speak when the
     result of function is obtained. Usually this needs to get turned on so user can
     get update for the function call.
@@ -468,15 +483,19 @@
     StateToolBookAppointmentCalTool,
     StateToolCustomTool,
 ]
 
 
 class State(TypedDict, total=False):
     name: Required[str]
-    """Name of the state, must be unique for each state."""
+    """Name of the state, must be unique for each state.
+
+    Must be consisted of a-z, A-Z, 0-9, or contain underscores and dashes, with a
+    maximum length of 64 (no space allowed).
+    """
 
     edges: Iterable[StateEdge]
     """Edges of the state define how and what state can be reached from this state."""
 
     state_prompt: str
     """Prompt of the state, will be appended to the system prompt of LLM.
```

### Comparing `retell_sdk-3.3.0/src/retell/types/llm_response.py` & `retell_sdk-3.4.0/src/retell/types/llm_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 
 
 class GeneralToolEndCallTool(BaseModel):
     name: str
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
-    tools + state tools + state transitions).
+    tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
+    contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Literal["end_call"]
 
     description: Optional[str] = None
     """Describes when to end the call."""
 
@@ -74,15 +75,16 @@
     availability for.
     """
 
     name: str
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
-    tools + state tools + state transitions).
+    tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
+    contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Literal["check_availability_cal"]
 
     description: Optional[str] = None
     """Describes when to check availability."""
 
@@ -107,15 +109,16 @@
     Cal.com event type id number for the cal.com event you want to book appointment.
     """
 
     name: str
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
-    tools + state tools + state transitions).
+    tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
+    contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Literal["book_appointment_cal"]
 
     description: Optional[str] = None
     """Describes when to book the appointment."""
 
@@ -150,15 +153,16 @@
     description: str
     """Describes what this tool does and when to call this tool."""
 
     name: str
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
-    tools + state tools + state edges).
+    tools + state tools + state edges). Must be consisted of a-z, A-Z, 0-9, or
+    contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     speak_after_execution: bool
     """
     Determines whether the agent would call LLM another time and speak when the
     result of function is obtained. Usually this needs to get turned on so user can
     get update for the function call.
@@ -251,15 +255,16 @@
 
 
 class StateToolEndCallTool(BaseModel):
     name: str
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
-    tools + state tools + state transitions).
+    tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
+    contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Literal["end_call"]
 
     description: Optional[str] = None
     """Describes when to end the call."""
 
@@ -297,15 +302,16 @@
     availability for.
     """
 
     name: str
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
-    tools + state tools + state transitions).
+    tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
+    contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Literal["check_availability_cal"]
 
     description: Optional[str] = None
     """Describes when to check availability."""
 
@@ -330,15 +336,16 @@
     Cal.com event type id number for the cal.com event you want to book appointment.
     """
 
     name: str
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
-    tools + state tools + state transitions).
+    tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
+    contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Literal["book_appointment_cal"]
 
     description: Optional[str] = None
     """Describes when to book the appointment."""
 
@@ -373,15 +380,16 @@
     description: str
     """Describes what this tool does and when to call this tool."""
 
     name: str
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
-    tools + state tools + state edges).
+    tools + state tools + state edges). Must be consisted of a-z, A-Z, 0-9, or
+    contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     speak_after_execution: bool
     """
     Determines whether the agent would call LLM another time and speak when the
     result of function is obtained. Usually this needs to get turned on so user can
     get update for the function call.
@@ -427,15 +435,19 @@
     StateToolBookAppointmentCalTool,
     StateToolCustomTool,
 ]
 
 
 class State(BaseModel):
     name: str
-    """Name of the state, must be unique for each state."""
+    """Name of the state, must be unique for each state.
+
+    Must be consisted of a-z, A-Z, 0-9, or contain underscores and dashes, with a
+    maximum length of 64 (no space allowed).
+    """
 
     edges: Optional[List[StateEdge]] = None
     """Edges of the state define how and what state can be reached from this state."""
 
     state_prompt: Optional[str] = None
     """Prompt of the state, will be appended to the system prompt of LLM.
 
@@ -491,14 +503,21 @@
     etc; or you can create your own custom tool (last option) for the LLM to use.
 
     - Tools of LLM (with state) = general tools + state tools + state transitions
 
     - Tools of LLM (no state) = general tools
     """
 
+    inbound_dynamic_variables_webhook_url: Optional[str] = None
+    """
+    For inbound phone calls with Retell numbers, if this webhook is set, will POST
+    to it to retrieve dynamic variables to use for the call. Without this, there's
+    no way to pass dynamic variables to inbound calls of Retell numbers.
+    """
+
     starting_state: Optional[str] = None
     """Name of the starting state. Required if states is not empty."""
 
     states: Optional[List[State]] = None
     """States of the LLM.
 
     This is to help reduce prompt length and tool choices when the call can be
```

### Comparing `retell_sdk-3.3.0/src/retell/types/llm_update_params.py` & `retell_sdk-3.4.0/src/retell/types/llm_create_params.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 from typing import Dict, List, Union, Iterable, Optional
 from typing_extensions import Literal, Required, TypedDict
 
 __all__ = [
-    "LlmUpdateParams",
+    "LlmCreateParams",
     "GeneralTool",
     "GeneralToolEndCallTool",
     "GeneralToolTransferCallTool",
     "GeneralToolCheckAvailabilityCalTool",
     "GeneralToolBookAppointmentCalTool",
     "GeneralToolCustomTool",
     "GeneralToolCustomToolParameters",
@@ -23,15 +23,15 @@
     "StateToolCheckAvailabilityCalTool",
     "StateToolBookAppointmentCalTool",
     "StateToolCustomTool",
     "StateToolCustomToolParameters",
 ]
 
 
-class LlmUpdateParams(TypedDict, total=False):
+class LlmCreateParams(TypedDict, total=False):
     begin_message: Optional[str]
     """First utterance said by the agent in the call.
 
     If not set, LLM will dynamically generate a message. If set to "", agent will
     wait for user to speak first.
     """
 
@@ -50,14 +50,21 @@
     etc; or you can create your own custom tool (last option) for the LLM to use.
 
     - Tools of LLM (with state) = general tools + state tools + state transitions
 
     - Tools of LLM (no state) = general tools
     """
 
+    inbound_dynamic_variables_webhook_url: Optional[str]
+    """
+    For inbound phone calls with Retell numbers, if this webhook is set, will POST
+    to it to retrieve dynamic variables to use for the call. Without this, there's
+    no way to pass dynamic variables to inbound calls of Retell numbers.
+    """
+
     starting_state: Optional[str]
     """Name of the starting state. Required if states is not empty."""
 
     states: Optional[Iterable[State]]
     """States of the LLM.
 
     This is to help reduce prompt length and tool choices when the call can be
@@ -69,15 +76,16 @@
 
 
 class GeneralToolEndCallTool(TypedDict, total=False):
     name: Required[str]
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
-    tools + state tools + state transitions).
+    tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
+    contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Required[Literal["end_call"]]
 
     description: str
     """Describes when to end the call."""
 
@@ -115,15 +123,16 @@
     availability for.
     """
 
     name: Required[str]
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
-    tools + state tools + state transitions).
+    tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
+    contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Required[Literal["check_availability_cal"]]
 
     description: str
     """Describes when to check availability."""
 
@@ -148,15 +157,16 @@
     Cal.com event type id number for the cal.com event you want to book appointment.
     """
 
     name: Required[str]
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
-    tools + state tools + state transitions).
+    tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
+    contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Required[Literal["book_appointment_cal"]]
 
     description: str
     """Describes when to book the appointment."""
 
@@ -191,15 +201,16 @@
     description: Required[str]
     """Describes what this tool does and when to call this tool."""
 
     name: Required[str]
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
-    tools + state tools + state edges).
+    tools + state tools + state edges). Must be consisted of a-z, A-Z, 0-9, or
+    contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     speak_after_execution: Required[bool]
     """
     Determines whether the agent would call LLM another time and speak when the
     result of function is obtained. Usually this needs to get turned on so user can
     get update for the function call.
@@ -292,15 +303,16 @@
 
 
 class StateToolEndCallTool(TypedDict, total=False):
     name: Required[str]
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
-    tools + state tools + state transitions).
+    tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
+    contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Required[Literal["end_call"]]
 
     description: str
     """Describes when to end the call."""
 
@@ -338,15 +350,16 @@
     availability for.
     """
 
     name: Required[str]
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
-    tools + state tools + state transitions).
+    tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
+    contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Required[Literal["check_availability_cal"]]
 
     description: str
     """Describes when to check availability."""
 
@@ -371,15 +384,16 @@
     Cal.com event type id number for the cal.com event you want to book appointment.
     """
 
     name: Required[str]
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
-    tools + state tools + state transitions).
+    tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
+    contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Required[Literal["book_appointment_cal"]]
 
     description: str
     """Describes when to book the appointment."""
 
@@ -414,15 +428,16 @@
     description: Required[str]
     """Describes what this tool does and when to call this tool."""
 
     name: Required[str]
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
-    tools + state tools + state edges).
+    tools + state tools + state edges). Must be consisted of a-z, A-Z, 0-9, or
+    contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     speak_after_execution: Required[bool]
     """
     Determines whether the agent would call LLM another time and speak when the
     result of function is obtained. Usually this needs to get turned on so user can
     get update for the function call.
@@ -468,15 +483,19 @@
     StateToolBookAppointmentCalTool,
     StateToolCustomTool,
 ]
 
 
 class State(TypedDict, total=False):
     name: Required[str]
-    """Name of the state, must be unique for each state."""
+    """Name of the state, must be unique for each state.
+
+    Must be consisted of a-z, A-Z, 0-9, or contain underscores and dashes, with a
+    maximum length of 64 (no space allowed).
+    """
 
     edges: Iterable[StateEdge]
     """Edges of the state define how and what state can be reached from this state."""
 
     state_prompt: str
     """Prompt of the state, will be appended to the system prompt of LLM.
```

### Comparing `retell_sdk-3.3.0/src/retell/types/phone_number_create_params.py` & `retell_sdk-3.4.0/src/retell/types/phone_number_create_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/src/retell/types/phone_number_response.py` & `retell_sdk-3.4.0/src/retell/types/phone_number_response.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/src/retell/types/register_call_response.py` & `retell_sdk-3.4.0/src/retell/types/register_call_response.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/LICENSE` & `retell_sdk-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.3.0/pyproject.toml` & `retell_sdk-3.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "retell-sdk"
-version = "3.3.0"
+version = "3.4.0"
 description = "The official Python library for the retell API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Retell", email = "founders@retellai.com" },
 ]
 dependencies = [
```

### Comparing `retell_sdk-3.3.0/PKG-INFO` & `retell_sdk-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: retell-sdk
-Version: 3.3.0
+Version: 3.4.0
 Summary: The official Python library for the retell API
 Project-URL: Homepage, https://github.com/RetellAI/retell-python-sdk
 Project-URL: Repository, https://github.com/RetellAI/retell-python-sdk
 Author-email: Retell <founders@retellai.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -287,20 +287,20 @@
     cast_to=httpx.Response,
     body={"my_param": True},
 )
 
 print(response.headers.get("x-foo"))
 ```
 
-#### Undocumented params
+#### Undocumented request params
 
 If you want to explicitly send an extra param, you can do so with the `extra_query`, `extra_body`, and `extra_headers` request
 options.
 
-#### Undocumented properties
+#### Undocumented response properties
 
 To access undocumented response properties, you can access the extra fields like `response.unknown_prop`. You
 can also get all the extra fields on the Pydantic model as a dict with
 [`response.model_extra`](https://docs.pydantic.dev/latest/api/base_model/#pydantic.BaseModel.model_extra).
 
 ### Configuring the HTTP client
```

