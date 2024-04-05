# Comparing `tmp/multion-0.4.5.tar.gz` & `tmp/multion-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multion-0.4.5.tar", max compression
+gzip compressed data, was "multion-0.5.0.tar", max compression
```

## Comparing `multion-0.4.5.tar` & `multion-0.5.0.tar`

### file list

```diff
@@ -1,37 +1,44 @@
--rw-r--r--   0        0        0     3937 2024-04-04 19:24:49.734526 multion-0.4.5/README.md
--rw-r--r--   0        0        0      592 2024-04-04 19:24:49.734526 multion-0.4.5/pyproject.toml
--rw-r--r--   0        0        0      990 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/__init__.py
--rw-r--r--   0        0        0    14283 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/client.py
--rw-r--r--   0        0        0      853 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/core/api_error.py
--rw-r--r--   0        0        0     1490 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/core/file.py
--rw-r--r--   0        0        0     5059 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/core/request_options.py
--rw-r--r--   0        0        0      162 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/environment.py
--rw-r--r--   0        0        0      170 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/py.typed
--rw-r--r--   0        0        0      247 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/sessions/__init__.py
--rw-r--r--   0        0        0    24518 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/sessions/client.py
--rw-r--r--   0        0        0      341 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/sessions/types/__init__.py
--rw-r--r--   0        0        0     1048 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/sessions/types/sessions_close_response.py
--rw-r--r--   0        0        0      953 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/sessions/types/sessions_list_response.py
--rw-r--r--   0        0        0      967 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/sessions/types/sessions_screenshot_response.py
--rw-r--r--   0        0        0      812 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/types/__init__.py
--rw-r--r--   0        0        0     1466 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/types/browse_output.py
--rw-r--r--   0        0        0      953 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/types/http_validation_error.py
--rw-r--r--   0        0        0      850 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/types/remote_value.py
--rw-r--r--   0        0        0     1312 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/types/retrieve_output.py
--rw-r--r--   0        0        0     1361 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/types/session_created.py
--rw-r--r--   0        0        0     1650 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/types/session_input.py
--rw-r--r--   0        0        0     1016 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/types/session_input_browser_params.py
--rw-r--r--   0        0        0     1365 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/types/session_step_success.py
--rw-r--r--   0        0        0      972 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/types/validation_error_loc_item.py
--rw-r--r--   0        0        0       75 2024-04-04 19:24:49.734526 multion-0.4.5/src/multion/version.py
--rw-r--r--   0        0        0     4427 1970-01-01 00:00:00.000000 multion-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     3937 2024-04-05 19:55:43.250646 multion-0.5.0/README.md
+-rw-r--r--   0        0        0      592 2024-04-05 19:55:43.250646 multion-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1417 2024-04-05 19:55:43.250646 multion-0.5.0/src/multion/__init__.py
+-rw-r--r--   0        0        0    15613 2024-04-05 19:55:43.250646 multion-0.5.0/src/multion/client.py
+-rw-r--r--   0        0        0      853 2024-04-05 19:55:43.250646 multion-0.5.0/src/multion/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-05 19:55:43.250646 multion-0.5.0/src/multion/core/api_error.py
+-rw-r--r--   0        0        0     1490 2024-04-05 19:55:43.250646 multion-0.5.0/src/multion/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-05 19:55:43.250646 multion-0.5.0/src/multion/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-05 19:55:43.250646 multion-0.5.0/src/multion/core/file.py
+-rw-r--r--   0        0        0     5059 2024-04-05 19:55:43.250646 multion-0.5.0/src/multion/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-04-05 19:55:43.250646 multion-0.5.0/src/multion/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-04-05 19:55:43.250646 multion-0.5.0/src/multion/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/core/request_options.py
+-rw-r--r--   0        0        0      162 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/environment.py
+-rw-r--r--   0        0        0      385 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/errors/__init__.py
+-rw-r--r--   0        0        0      301 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/errors/bad_request_error.py
+-rw-r--r--   0        0        0      333 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/errors/internal_server_error.py
+-rw-r--r--   0        0        0      308 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      313 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/py.typed
+-rw-r--r--   0        0        0      427 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/sessions/__init__.py
+-rw-r--r--   0        0        0    28787 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/sessions/client.py
+-rw-r--r--   0        0        0      590 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/sessions/types/__init__.py
+-rw-r--r--   0        0        0     1024 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/sessions/types/create_session_input_browser_params.py
+-rw-r--r--   0        0        0     1048 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/sessions/types/sessions_close_response.py
+-rw-r--r--   0        0        0      953 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/sessions/types/sessions_list_response.py
+-rw-r--r--   0        0        0      967 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/sessions/types/sessions_screenshot_response.py
+-rw-r--r--   0        0        0     1022 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/sessions/types/step_session_input_browser_params.py
+-rw-r--r--   0        0        0     1015 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/types/__init__.py
+-rw-r--r--   0        0        0     1091 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/types/bad_request_response.py
+-rw-r--r--   0        0        0     1355 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/types/browse_output.py
+-rw-r--r--   0        0        0      953 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/types/http_validation_error.py
+-rw-r--r--   0        0        0     1100 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/types/internal_server_error_response.py
+-rw-r--r--   0        0        0     1096 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/types/payment_required_response.py
+-rw-r--r--   0        0        0      850 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/types/remote_value.py
+-rw-r--r--   0        0        0     1312 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/types/retrieve_output.py
+-rw-r--r--   0        0        0     1361 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/types/session_created.py
+-rw-r--r--   0        0        0     1365 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/types/session_step_success.py
+-rw-r--r--   0        0        0     1093 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/types/unauthorized_response.py
+-rw-r--r--   0        0        0      972 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0       75 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/version.py
+-rw-r--r--   0        0        0     4427 1970-01-01 00:00:00.000000 multion-0.5.0/PKG-INFO
```

### Comparing `multion-0.4.5/README.md` & `multion-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `multion-0.4.5/pyproject.toml` & `multion-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "multion"
-version = "0.4.5"
+version = "0.5.0"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "multion", from = "src"}
 ]
```

### Comparing `multion-0.4.5/src/multion/client.py` & `multion-0.5.0/src/multion/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,18 +10,24 @@
 from .core.api_error import ApiError
 from .core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .core.jsonable_encoder import jsonable_encoder
 from .core.pydantic_utilities import pydantic_v1
 from .core.remove_none_from_dict import remove_none_from_dict
 from .core.request_options import RequestOptions
 from .environment import MultiOnEnvironment
+from .errors.bad_request_error import BadRequestError
+from .errors.internal_server_error import InternalServerError
+from .errors.unauthorized_error import UnauthorizedError
 from .errors.unprocessable_entity_error import UnprocessableEntityError
 from .sessions.client import AsyncSessionsClient, SessionsClient
+from .types.bad_request_response import BadRequestResponse
 from .types.browse_output import BrowseOutput
 from .types.http_validation_error import HttpValidationError
+from .types.internal_server_error_response import InternalServerErrorResponse
+from .types.unauthorized_response import UnauthorizedResponse
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class MultiOn:
     """
@@ -76,61 +82,57 @@
         )
         self.sessions = SessionsClient(client_wrapper=self._client_wrapper)
 
     def browse(
         self,
         *,
         cmd: str,
-        url: str,
+        url: typing.Optional[str] = OMIT,
         local: typing.Optional[bool] = OMIT,
         session_id: typing.Optional[str] = OMIT,
         max_steps: typing.Optional[int] = OMIT,
-        stream: typing.Optional[bool] = OMIT,
         include_screenshot: typing.Optional[bool] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> BrowseOutput:
         """
         Allows for browsing the web using detailed natural language instructions. The function supports multi-step command execution based on the `CONTINUE` status.
 
         Parameters:
-            - cmd: str. The command for the agent to carry out (Default: www.google.com)
+            - cmd: str. A specific natural language instruction for the agent to execute
 
-            - url: str. The URL to start or continue browsing from.
+            - url: typing.Optional[str]. The URL to start or continue browsing from. (Default: google.com)
 
             - local: typing.Optional[bool]. Boolean flag to indicate if session to be run locally or in the cloud (Default: False)
 
-            - session_id: typing.Optional[str].
+            - session_id: typing.Optional[str]. Continues the session with session_id if provided.
 
             - max_steps: typing.Optional[int]. Maximum number of steps to execute. (Default: 20)
 
-            - stream: typing.Optional[bool]. Boolean flag to stream results back to the client (Default: False)
-
-            - include_screenshot: typing.Optional[bool].
+            - include_screenshot: typing.Optional[bool]. Boolean flag to include a screenshot of the final page.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from multion.client import MultiOn
 
         client = MultiOn(
             api_key="YOUR_API_KEY",
         )
         client.browse(
             cmd="cmd",
-            url="url",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"cmd": cmd, "url": url}
+        _request: typing.Dict[str, typing.Any] = {"cmd": cmd}
+        if url is not OMIT:
+            _request["url"] = url
         if local is not OMIT:
             _request["local"] = local
         if session_id is not OMIT:
             _request["session_id"] = session_id
         if max_steps is not OMIT:
             _request["max_steps"] = max_steps
-        if stream is not OMIT:
-            _request["stream"] = stream
         if include_screenshot is not OMIT:
             _request["include_screenshot"] = include_screenshot
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "browse"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
@@ -153,18 +155,26 @@
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic_v1.parse_obj_as(BrowseOutput, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequestResponse, _response.json()))  # type: ignore
+        if _response.status_code == 401:
+            raise UnauthorizedError(pydantic_v1.parse_obj_as(UnauthorizedResponse, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(
                 pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
             )
+        if _response.status_code == 500:
+            raise InternalServerError(
+                pydantic_v1.parse_obj_as(InternalServerErrorResponse, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -221,61 +231,57 @@
         )
         self.sessions = AsyncSessionsClient(client_wrapper=self._client_wrapper)
 
     async def browse(
         self,
         *,
         cmd: str,
-        url: str,
+        url: typing.Optional[str] = OMIT,
         local: typing.Optional[bool] = OMIT,
         session_id: typing.Optional[str] = OMIT,
         max_steps: typing.Optional[int] = OMIT,
-        stream: typing.Optional[bool] = OMIT,
         include_screenshot: typing.Optional[bool] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> BrowseOutput:
         """
         Allows for browsing the web using detailed natural language instructions. The function supports multi-step command execution based on the `CONTINUE` status.
 
         Parameters:
-            - cmd: str. The command for the agent to carry out (Default: www.google.com)
+            - cmd: str. A specific natural language instruction for the agent to execute
 
-            - url: str. The URL to start or continue browsing from.
+            - url: typing.Optional[str]. The URL to start or continue browsing from. (Default: google.com)
 
             - local: typing.Optional[bool]. Boolean flag to indicate if session to be run locally or in the cloud (Default: False)
 
-            - session_id: typing.Optional[str].
+            - session_id: typing.Optional[str]. Continues the session with session_id if provided.
 
             - max_steps: typing.Optional[int]. Maximum number of steps to execute. (Default: 20)
 
-            - stream: typing.Optional[bool]. Boolean flag to stream results back to the client (Default: False)
-
-            - include_screenshot: typing.Optional[bool].
+            - include_screenshot: typing.Optional[bool]. Boolean flag to include a screenshot of the final page.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from multion.client import AsyncMultiOn
 
         client = AsyncMultiOn(
             api_key="YOUR_API_KEY",
         )
         await client.browse(
             cmd="cmd",
-            url="url",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"cmd": cmd, "url": url}
+        _request: typing.Dict[str, typing.Any] = {"cmd": cmd}
+        if url is not OMIT:
+            _request["url"] = url
         if local is not OMIT:
             _request["local"] = local
         if session_id is not OMIT:
             _request["session_id"] = session_id
         if max_steps is not OMIT:
             _request["max_steps"] = max_steps
-        if stream is not OMIT:
-            _request["stream"] = stream
         if include_screenshot is not OMIT:
             _request["include_screenshot"] = include_screenshot
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "browse"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
@@ -298,18 +304,26 @@
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic_v1.parse_obj_as(BrowseOutput, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequestResponse, _response.json()))  # type: ignore
+        if _response.status_code == 401:
+            raise UnauthorizedError(pydantic_v1.parse_obj_as(UnauthorizedResponse, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(
                 pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
             )
+        if _response.status_code == 500:
+            raise InternalServerError(
+                pydantic_v1.parse_obj_as(InternalServerErrorResponse, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `multion-0.4.5/src/multion/core/__init__.py` & `multion-0.5.0/src/multion/core/__init__.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.5/src/multion/core/client_wrapper.py` & `multion-0.5.0/src/multion/core/client_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "multion",
-            "X-Fern-SDK-Version": "0.4.5",
+            "X-Fern-SDK-Version": "0.5.0",
         }
         headers["X_MULTION_API_KEY"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `multion-0.4.5/src/multion/core/datetime_utils.py` & `multion-0.5.0/src/multion/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.5/src/multion/core/file.py` & `multion-0.5.0/src/multion/core/file.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.5/src/multion/core/http_client.py` & `multion-0.5.0/src/multion/core/http_client.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.5/src/multion/core/jsonable_encoder.py` & `multion-0.5.0/src/multion/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.5/src/multion/core/request_options.py` & `multion-0.5.0/src/multion/core/request_options.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.5/src/multion/sessions/client.py` & `multion-0.5.0/src/multion/sessions/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,59 +9,78 @@
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.pydantic_utilities import pydantic_v1
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.http_validation_error import HttpValidationError
 from ..types.session_created import SessionCreated
-from ..types.session_input import SessionInput
 from ..types.session_step_success import SessionStepSuccess
+from .types.create_session_input_browser_params import CreateSessionInputBrowserParams
 from .types.sessions_close_response import SessionsCloseResponse
 from .types.sessions_list_response import SessionsListResponse
 from .types.sessions_screenshot_response import SessionsScreenshotResponse
+from .types.step_session_input_browser_params import StepSessionInputBrowserParams
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class SessionsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def create(
-        self, *, request: SessionInput, request_options: typing.Optional[RequestOptions] = None
+        self,
+        *,
+        url: str,
+        local: typing.Optional[bool] = OMIT,
+        browser_params: typing.Optional[CreateSessionInputBrowserParams] = OMIT,
+        include_screenshot: typing.Optional[bool] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
     ) -> SessionCreated:
         """
         Creates a new session and returns session details including a unique session ID.
 
         Parameters:
-            - request: SessionInput.
+            - url: str. The URL to create or continue session from.
+
+            - local: typing.Optional[bool]. Boolean flag to indicate if session to be run locally or in the cloud (Default: False)
+
+            - browser_params: typing.Optional[CreateSessionInputBrowserParams]. Object containing height and width for the browser screen size.
+
+            - include_screenshot: typing.Optional[bool].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from multion import SessionInput
         from multion.client import MultiOn
 
         client = MultiOn(
             api_key="YOUR_API_KEY",
         )
         client.sessions.create(
-            request=SessionInput(),
+            url="url",
         )
         """
+        _request: typing.Dict[str, typing.Any] = {"url": url}
+        if local is not OMIT:
+            _request["local"] = local
+        if browser_params is not OMIT:
+            _request["browser_params"] = browser_params
+        if include_screenshot is not OMIT:
+            _request["include_screenshot"] = include_screenshot
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "session"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(request)
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(request),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -83,45 +102,71 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def step(
-        self, session_id: str, *, request: SessionInput, request_options: typing.Optional[RequestOptions] = None
+        self,
+        session_id: str,
+        *,
+        cmd: str,
+        url: typing.Optional[str] = OMIT,
+        stream: typing.Optional[bool] = OMIT,
+        browser_params: typing.Optional[StepSessionInputBrowserParams] = OMIT,
+        include_screenshot: typing.Optional[bool] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
     ) -> SessionStepSuccess:
         """
+        Allows for browsing the web using detailed natural language instructions in a step mode for a session with a given session ID
+
         Parameters:
             - session_id: str.
 
-            - request: SessionInput.
+            - cmd: str. A specific natural language instruction for the next step.
+
+            - url: typing.Optional[str]. The URL to create or continue session from.
+
+            - stream: typing.Optional[bool]. Boolean flag to stream results back to the client (Default: False)
+
+            - browser_params: typing.Optional[StepSessionInputBrowserParams]. Object containing height and width for the browser screen size.
+
+            - include_screenshot: typing.Optional[bool].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from multion import SessionInput
         from multion.client import MultiOn
 
         client = MultiOn(
             api_key="YOUR_API_KEY",
         )
         client.sessions.step(
             session_id="session_id",
-            request=SessionInput(),
+            cmd="cmd",
         )
         """
+        _request: typing.Dict[str, typing.Any] = {"cmd": cmd}
+        if url is not OMIT:
+            _request["url"] = url
+        if stream is not OMIT:
+            _request["stream"] = stream
+        if browser_params is not OMIT:
+            _request["browser_params"] = browser_params
+        if include_screenshot is not OMIT:
+            _request["include_screenshot"] = include_screenshot
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"session/{jsonable_encoder(session_id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(request)
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(request),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -146,14 +191,16 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def close(
         self, session_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> SessionsCloseResponse:
         """
+        Closes the session.
+
         Parameters:
             - session_id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from multion.client import MultiOn
 
@@ -196,15 +243,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def screenshot(
         self, session_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> SessionsScreenshotResponse:
         """
-        This function is used to get a screenshot for a website.
+        Retrieve the screenshot of the session.
 
         Parameters:
             - session_id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from multion.client import MultiOn
@@ -248,14 +295,16 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> SessionsListResponse:
         """
+        Retrieve a list of active session IDs.
+
         Parameters:
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from multion.client import MultiOn
 
         client = MultiOn(
             api_key="YOUR_API_KEY",
@@ -292,44 +341,62 @@
 
 
 class AsyncSessionsClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def create(
-        self, *, request: SessionInput, request_options: typing.Optional[RequestOptions] = None
+        self,
+        *,
+        url: str,
+        local: typing.Optional[bool] = OMIT,
+        browser_params: typing.Optional[CreateSessionInputBrowserParams] = OMIT,
+        include_screenshot: typing.Optional[bool] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
     ) -> SessionCreated:
         """
         Creates a new session and returns session details including a unique session ID.
 
         Parameters:
-            - request: SessionInput.
+            - url: str. The URL to create or continue session from.
+
+            - local: typing.Optional[bool]. Boolean flag to indicate if session to be run locally or in the cloud (Default: False)
+
+            - browser_params: typing.Optional[CreateSessionInputBrowserParams]. Object containing height and width for the browser screen size.
+
+            - include_screenshot: typing.Optional[bool].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from multion import SessionInput
         from multion.client import AsyncMultiOn
 
         client = AsyncMultiOn(
             api_key="YOUR_API_KEY",
         )
         await client.sessions.create(
-            request=SessionInput(),
+            url="url",
         )
         """
+        _request: typing.Dict[str, typing.Any] = {"url": url}
+        if local is not OMIT:
+            _request["local"] = local
+        if browser_params is not OMIT:
+            _request["browser_params"] = browser_params
+        if include_screenshot is not OMIT:
+            _request["include_screenshot"] = include_screenshot
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "session"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(request)
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(request),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -351,45 +418,71 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def step(
-        self, session_id: str, *, request: SessionInput, request_options: typing.Optional[RequestOptions] = None
+        self,
+        session_id: str,
+        *,
+        cmd: str,
+        url: typing.Optional[str] = OMIT,
+        stream: typing.Optional[bool] = OMIT,
+        browser_params: typing.Optional[StepSessionInputBrowserParams] = OMIT,
+        include_screenshot: typing.Optional[bool] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
     ) -> SessionStepSuccess:
         """
+        Allows for browsing the web using detailed natural language instructions in a step mode for a session with a given session ID
+
         Parameters:
             - session_id: str.
 
-            - request: SessionInput.
+            - cmd: str. A specific natural language instruction for the next step.
+
+            - url: typing.Optional[str]. The URL to create or continue session from.
+
+            - stream: typing.Optional[bool]. Boolean flag to stream results back to the client (Default: False)
+
+            - browser_params: typing.Optional[StepSessionInputBrowserParams]. Object containing height and width for the browser screen size.
+
+            - include_screenshot: typing.Optional[bool].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from multion import SessionInput
         from multion.client import AsyncMultiOn
 
         client = AsyncMultiOn(
             api_key="YOUR_API_KEY",
         )
         await client.sessions.step(
             session_id="session_id",
-            request=SessionInput(),
+            cmd="cmd",
         )
         """
+        _request: typing.Dict[str, typing.Any] = {"cmd": cmd}
+        if url is not OMIT:
+            _request["url"] = url
+        if stream is not OMIT:
+            _request["stream"] = stream
+        if browser_params is not OMIT:
+            _request["browser_params"] = browser_params
+        if include_screenshot is not OMIT:
+            _request["include_screenshot"] = include_screenshot
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"session/{jsonable_encoder(session_id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(request)
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(request),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -414,14 +507,16 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def close(
         self, session_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> SessionsCloseResponse:
         """
+        Closes the session.
+
         Parameters:
             - session_id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from multion.client import AsyncMultiOn
 
@@ -464,15 +559,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def screenshot(
         self, session_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> SessionsScreenshotResponse:
         """
-        This function is used to get a screenshot for a website.
+        Retrieve the screenshot of the session.
 
         Parameters:
             - session_id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from multion.client import AsyncMultiOn
@@ -516,14 +611,16 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> SessionsListResponse:
         """
+        Retrieve a list of active session IDs.
+
         Parameters:
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from multion.client import AsyncMultiOn
 
         client = AsyncMultiOn(
             api_key="YOUR_API_KEY",
```

### Comparing `multion-0.4.5/src/multion/sessions/types/sessions_close_response.py` & `multion-0.5.0/src/multion/sessions/types/sessions_close_response.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.5/src/multion/sessions/types/sessions_list_response.py` & `multion-0.5.0/src/multion/sessions/types/sessions_list_response.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.5/src/multion/sessions/types/sessions_screenshot_response.py` & `multion-0.5.0/src/multion/sessions/types/sessions_screenshot_response.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.5/src/multion/types/browse_output.py` & `multion-0.5.0/src/multion/types/browse_output.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,19 +19,14 @@
     """
 
     url: str = pydantic_v1.Field()
     """
     The current URL of the session.
     """
 
-    page_content: str = pydantic_v1.Field()
-    """
-    Extracted text content from the current page.
-    """
-
     screenshot: str = pydantic_v1.Field()
     """
     image url of the screenshot taken during the session.
     """
 
     session_id: str = pydantic_v1.Field()
     """
```

### Comparing `multion-0.4.5/src/multion/types/http_validation_error.py` & `multion-0.5.0/src/multion/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.5/src/multion/types/remote_value.py` & `multion-0.5.0/src/multion/types/remote_value.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.5/src/multion/types/retrieve_output.py` & `multion-0.5.0/src/multion/types/retrieve_output.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.5/src/multion/types/session_created.py` & `multion-0.5.0/src/multion/types/session_created.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.5/src/multion/types/session_input.py` & `multion-0.5.0/src/multion/types/unauthorized_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .session_input_browser_params import SessionInputBrowserParams
 
 
-class SessionInput(pydantic_v1.BaseModel):
-    cmd: typing.Optional[str] = pydantic_v1.Field(default=None)
-    """
-    A specific natural language instruction for the next step.
-    """
-
-    url: typing.Optional[str] = None
-    local: typing.Optional[bool] = pydantic_v1.Field(default=None)
-    """
-    Boolean flag to indicate if session to be run locally or in the cloud (Default: False)
-    """
-
-    stream: typing.Optional[bool] = pydantic_v1.Field(default=None)
-    """
-    Boolean flag to stream results back to the client (Default: False)
-    """
-
-    browser_params: typing.Optional[SessionInputBrowserParams] = pydantic_v1.Field(default=None)
-    """
-    Object containing height and width for the browser screen size.
-    """
-
-    include_screenshot: typing.Optional[bool] = None
+class UnauthorizedResponse(pydantic_v1.BaseModel):
+    status_code: typing.Optional[int] = pydantic_v1.Field(alias="statusCode", default=None)
+    error: typing.Optional[str] = None
+    message: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `multion-0.4.5/src/multion/types/session_input_browser_params.py` & `multion-0.5.0/src/multion/sessions/types/create_session_input_browser_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
 
-class SessionInputBrowserParams(pydantic_v1.BaseModel):
+class CreateSessionInputBrowserParams(pydantic_v1.BaseModel):
     """
     Object containing height and width for the browser screen size.
     """
 
     height: typing.Optional[float] = None
     width: typing.Optional[float] = None
```

### Comparing `multion-0.4.5/src/multion/types/session_step_success.py` & `multion-0.5.0/src/multion/types/session_step_success.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.5/src/multion/types/validation_error.py` & `multion-0.5.0/src/multion/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.5/PKG-INFO` & `multion-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multion
-Version: 0.4.5
+Version: 0.5.0
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

