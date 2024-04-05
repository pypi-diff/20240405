# Comparing `tmp/robotframework_openapitools-0.1.2.tar.gz` & `tmp/robotframework_openapitools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_openapitools-0.1.2.tar", max compression
+gzip compressed data, was "robotframework_openapitools-0.1.3.tar", max compression
```

## Comparing `robotframework_openapitools-0.1.2.tar` & `robotframework_openapitools-0.1.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rwxr-xr-x   0        0        0    11558 2024-02-12 15:55:24.206229 robotframework_openapitools-0.1.2/LICENSE
--rwxr-xr-x   0        0        0      185 2024-03-08 15:13:37.215159 robotframework_openapitools-0.1.2/docs/README.md
--rwxr-xr-x   0        0        0     3371 2024-03-15 20:29:07.512002 robotframework_openapitools-0.1.2/pyproject.toml
--rwxr-xr-x   0        0        0     1331 2024-03-06 16:35:05.537954 robotframework_openapitools-0.1.2/src/OpenApiDriver/__init__.py
--rwxr-xr-x   0        0        0    32615 2024-03-15 15:30:54.583733 robotframework_openapitools-0.1.2/src/OpenApiDriver/openapi_executors.py
--rwxr-xr-x   0        0        0     4652 2024-03-15 20:22:54.832269 robotframework_openapitools-0.1.2/src/OpenApiDriver/openapi_reader.py
--rwxr-xr-x   0        0        0    27138 2024-03-15 20:27:50.562656 robotframework_openapitools-0.1.2/src/OpenApiDriver/openapidriver.libspec
--rwxr-xr-x   0        0        0    15546 2024-03-15 20:22:54.832269 robotframework_openapitools-0.1.2/src/OpenApiDriver/openapidriver.py
--rwxr-xr-x   0        0        0        0 2024-01-31 08:42:12.630853 robotframework_openapitools-0.1.2/src/OpenApiDriver/py.typed
--rwxr-xr-x   0        0        0     1591 2024-02-12 14:16:27.194996 robotframework_openapitools-0.1.2/src/OpenApiLibCore/__init__.py
--rwxr-xr-x   0        0        0    12080 2024-02-12 14:16:27.195985 robotframework_openapitools-0.1.2/src/OpenApiLibCore/dto_base.py
--rwxr-xr-x   0        0        0     2903 2024-02-12 14:16:27.196984 robotframework_openapitools-0.1.2/src/OpenApiLibCore/dto_utils.py
--rwxr-xr-x   0        0        0      112 2024-03-06 08:33:13.925424 robotframework_openapitools-0.1.2/src/OpenApiLibCore/oas_cache.py
--rwxr-xr-x   0        0        0    33102 2024-03-15 20:27:49.952028 robotframework_openapitools-0.1.2/src/OpenApiLibCore/openapi_libcore.libspec
--rwxr-xr-x   0        0        0    63045 2024-03-15 20:22:54.832269 robotframework_openapitools-0.1.2/src/OpenApiLibCore/openapi_libcore.py
--rwxr-xr-x   0        0        0        0 2024-01-31 08:43:45.640076 robotframework_openapitools-0.1.2/src/OpenApiLibCore/py.typed
--rwxr-xr-x   0        0        0    18145 2024-01-31 08:43:45.640833 robotframework_openapitools-0.1.2/src/OpenApiLibCore/value_utils.py
--rwxr-xr-x   0        0        0      223 2024-03-06 16:35:05.808004 robotframework_openapitools-0.1.2/src/roboswag/__init__.py
--rwxr-xr-x   0        0        0       35 2024-02-12 15:55:24.208754 robotframework_openapitools-0.1.2/src/roboswag/__main__.py
--rwxr-xr-x   0        0        0     1323 2024-03-06 16:35:03.918414 robotframework_openapitools-0.1.2/src/roboswag/auth.py
--rwxr-xr-x   0        0        0     2216 2024-03-06 16:35:05.748050 robotframework_openapitools-0.1.2/src/roboswag/cli.py
--rwxr-xr-x   0        0        0     2870 2024-03-06 16:35:03.983780 robotframework_openapitools-0.1.2/src/roboswag/core.py
--rwxr-xr-x   0        0        0       59 2024-02-12 15:55:24.222947 robotframework_openapitools-0.1.2/src/roboswag/generate/__init__.py
--rwxr-xr-x   0        0        0     4706 2024-03-06 16:35:04.067930 robotframework_openapitools-0.1.2/src/roboswag/generate/generate.py
--rwxr-xr-x   0        0        0        0 2024-02-12 15:55:24.223963 robotframework_openapitools-0.1.2/src/roboswag/generate/models/__init__.py
--rwxr-xr-x   0        0        0     8528 2024-03-06 16:35:04.137359 robotframework_openapitools-0.1.2/src/roboswag/generate/models/api.py
--rwxr-xr-x   0        0        0      841 2024-03-06 16:35:03.958474 robotframework_openapitools-0.1.2/src/roboswag/generate/models/definition.py
--rwxr-xr-x   0        0        0     2304 2024-03-06 16:35:04.024928 robotframework_openapitools-0.1.2/src/roboswag/generate/models/endpoint.py
--rwxr-xr-x   0        0        0      682 2024-03-06 16:35:03.991681 robotframework_openapitools-0.1.2/src/roboswag/generate/models/parameter.py
--rwxr-xr-x   0        0        0      257 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.2/src/roboswag/generate/models/response.py
--rwxr-xr-x   0        0        0      561 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.2/src/roboswag/generate/models/tag.py
--rwxr-xr-x   0        0        0     1550 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.2/src/roboswag/generate/models/utils.py
--rwxr-xr-x   0        0        0      621 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.2/src/roboswag/generate/templates/api_init.jinja
--rwxr-xr-x   0        0        0      357 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.2/src/roboswag/generate/templates/models.jinja
--rwxr-xr-x   0        0        0     3191 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.2/src/roboswag/generate/templates/paths.jinja
--rwxr-xr-x   0        0        0     1025 2024-03-06 16:35:04.038806 robotframework_openapitools-0.1.2/src/roboswag/logger.py
--rwxr-xr-x   0        0        0      188 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.2/src/roboswag/validate/__init__.py
--rwxr-xr-x   0        0        0       84 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.2/src/roboswag/validate/core.py
--rwxr-xr-x   0        0        0      711 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.2/src/roboswag/validate/schema.py
--rwxr-xr-x   0        0        0      527 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.2/src/roboswag/validate/text_response.py
--rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 robotframework_openapitools-0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0    11558 2024-02-12 15:55:24.206229 robotframework_openapitools-0.1.3/LICENSE
+-rwxr-xr-x   0        0        0      185 2024-03-08 15:13:37.215159 robotframework_openapitools-0.1.3/docs/README.md
+-rwxr-xr-x   0        0        0     3371 2024-04-05 14:46:36.513338 robotframework_openapitools-0.1.3/pyproject.toml
+-rwxr-xr-x   0        0        0     1331 2024-03-06 16:35:05.537954 robotframework_openapitools-0.1.3/src/OpenApiDriver/__init__.py
+-rw-r--r--   0        0        0    31970 2024-04-05 14:38:46.773098 robotframework_openapitools-0.1.3/src/OpenApiDriver/openapi_executors.py
+-rwxr-xr-x   0        0        0     4652 2024-03-15 20:22:54.832269 robotframework_openapitools-0.1.3/src/OpenApiDriver/openapi_reader.py
+-rwxr-xr-x   0        0        0    27138 2024-04-05 14:47:48.776430 robotframework_openapitools-0.1.3/src/OpenApiDriver/openapidriver.libspec
+-rwxr-xr-x   0        0        0    15546 2024-03-15 20:22:54.832269 robotframework_openapitools-0.1.3/src/OpenApiDriver/openapidriver.py
+-rwxr-xr-x   0        0        0        0 2024-01-31 08:42:12.630853 robotframework_openapitools-0.1.3/src/OpenApiDriver/py.typed
+-rwxr-xr-x   0        0        0     1591 2024-02-12 14:16:27.194996 robotframework_openapitools-0.1.3/src/OpenApiLibCore/__init__.py
+-rwxr-xr-x   0        0        0    12080 2024-02-12 14:16:27.195985 robotframework_openapitools-0.1.3/src/OpenApiLibCore/dto_base.py
+-rwxr-xr-x   0        0        0     2903 2024-02-12 14:16:27.196984 robotframework_openapitools-0.1.3/src/OpenApiLibCore/dto_utils.py
+-rwxr-xr-x   0        0        0      112 2024-03-06 08:33:13.925424 robotframework_openapitools-0.1.3/src/OpenApiLibCore/oas_cache.py
+-rwxr-xr-x   0        0        0    33102 2024-04-05 14:47:48.144349 robotframework_openapitools-0.1.3/src/OpenApiLibCore/openapi_libcore.libspec
+-rw-r--r--   0        0        0    62223 2024-04-05 14:05:14.902473 robotframework_openapitools-0.1.3/src/OpenApiLibCore/openapi_libcore.py
+-rwxr-xr-x   0        0        0        0 2024-01-31 08:43:45.640076 robotframework_openapitools-0.1.3/src/OpenApiLibCore/py.typed
+-rwxr-xr-x   0        0        0    18145 2024-01-31 08:43:45.640833 robotframework_openapitools-0.1.3/src/OpenApiLibCore/value_utils.py
+-rwxr-xr-x   0        0        0      223 2024-03-06 16:35:05.808004 robotframework_openapitools-0.1.3/src/roboswag/__init__.py
+-rwxr-xr-x   0        0        0       35 2024-02-12 15:55:24.208754 robotframework_openapitools-0.1.3/src/roboswag/__main__.py
+-rwxr-xr-x   0        0        0     1323 2024-03-06 16:35:03.918414 robotframework_openapitools-0.1.3/src/roboswag/auth.py
+-rwxr-xr-x   0        0        0     2216 2024-03-06 16:35:05.748050 robotframework_openapitools-0.1.3/src/roboswag/cli.py
+-rwxr-xr-x   0        0        0     2870 2024-03-06 16:35:03.983780 robotframework_openapitools-0.1.3/src/roboswag/core.py
+-rwxr-xr-x   0        0        0       59 2024-02-12 15:55:24.222947 robotframework_openapitools-0.1.3/src/roboswag/generate/__init__.py
+-rwxr-xr-x   0        0        0     4706 2024-03-06 16:35:04.067930 robotframework_openapitools-0.1.3/src/roboswag/generate/generate.py
+-rwxr-xr-x   0        0        0        0 2024-02-12 15:55:24.223963 robotframework_openapitools-0.1.3/src/roboswag/generate/models/__init__.py
+-rwxr-xr-x   0        0        0     8528 2024-03-06 16:35:04.137359 robotframework_openapitools-0.1.3/src/roboswag/generate/models/api.py
+-rwxr-xr-x   0        0        0      841 2024-03-06 16:35:03.958474 robotframework_openapitools-0.1.3/src/roboswag/generate/models/definition.py
+-rwxr-xr-x   0        0        0     2304 2024-03-06 16:35:04.024928 robotframework_openapitools-0.1.3/src/roboswag/generate/models/endpoint.py
+-rwxr-xr-x   0        0        0      682 2024-03-06 16:35:03.991681 robotframework_openapitools-0.1.3/src/roboswag/generate/models/parameter.py
+-rwxr-xr-x   0        0        0      257 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.3/src/roboswag/generate/models/response.py
+-rwxr-xr-x   0        0        0      561 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.3/src/roboswag/generate/models/tag.py
+-rwxr-xr-x   0        0        0     1550 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.3/src/roboswag/generate/models/utils.py
+-rwxr-xr-x   0        0        0      621 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.3/src/roboswag/generate/templates/api_init.jinja
+-rwxr-xr-x   0        0        0      357 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.3/src/roboswag/generate/templates/models.jinja
+-rwxr-xr-x   0        0        0     3191 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.3/src/roboswag/generate/templates/paths.jinja
+-rwxr-xr-x   0        0        0     1025 2024-03-06 16:35:04.038806 robotframework_openapitools-0.1.3/src/roboswag/logger.py
+-rwxr-xr-x   0        0        0      188 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.3/src/roboswag/validate/__init__.py
+-rwxr-xr-x   0        0        0       84 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.3/src/roboswag/validate/core.py
+-rwxr-xr-x   0        0        0      711 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.3/src/roboswag/validate/schema.py
+-rwxr-xr-x   0        0        0      527 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.3/src/roboswag/validate/text_response.py
+-rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 robotframework_openapitools-0.1.3/PKG-INFO
```

### Comparing `robotframework_openapitools-0.1.2/LICENSE` & `robotframework_openapitools-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.2/pyproject.toml` & `robotframework_openapitools-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name="robotframework-openapitools"
-version = "0.1.2"
+version = "0.1.3"
 description = "A set of Robot Framework libraries to test APIs for which the OAS is available."
 license = "Apache-2.0"
 authors = [
     "Bartlomiej Hirsz <bartek.hirsz@gmail.com>",
     "Mateusz Nojek <matnojek@gmail.com>",
     "Robin Mackaij <r.a.mackaij@gmail.com>"
 ]
```

### Comparing `robotframework_openapitools-0.1.2/src/OpenApiDriver/__init__.py` & `robotframework_openapitools-0.1.3/src/OpenApiDriver/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.2/src/OpenApiDriver/openapi_executors.py` & `robotframework_openapitools-0.1.3/src/OpenApiDriver/openapi_executors.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,744 +1,748 @@
-"""Module containing the classes to perform automatic OpenAPI contract validation."""
-
-import json as _json
-from enum import Enum
-from logging import getLogger
-from pathlib import Path
-from random import choice
-from typing import Any, Dict, List, Optional, Tuple, Union
-
-from openapi_core.contrib.requests import (
-    RequestsOpenAPIRequest,
-    RequestsOpenAPIResponse,
-)
-from openapi_core.exceptions import OpenAPIError
-from openapi_core.validation.exceptions import ValidationError
-from openapi_core.validation.response.exceptions import InvalidData
-from openapi_core.validation.schemas.exceptions import InvalidSchemaValue
-from requests import Response
-from requests.auth import AuthBase
-from requests.cookies import RequestsCookieJar as CookieJar
-from robot.api import Failure, SkipExecution
-from robot.api.deco import keyword, library
-from robot.libraries.BuiltIn import BuiltIn
-
-from OpenApiLibCore import OpenApiLibCore, RequestData, RequestValues, resolve_schema
-
-run_keyword = BuiltIn().run_keyword
-
-
-logger = getLogger(__name__)
-
-
-class ValidationLevel(str, Enum):
-    """The available levels for the response_validation parameter."""
-
-    DISABLED = "DISABLED"
-    INFO = "INFO"
-    WARN = "WARN"
-    STRICT = "STRICT"
-
-
-@library(scope="TEST SUITE", doc_format="ROBOT")
-class OpenApiExecutors(OpenApiLibCore):  # pylint: disable=too-many-instance-attributes
-    """Main class providing the keywords and core logic to perform endpoint validations."""
-
-    def __init__(  # pylint: disable=too-many-arguments
-        self,
-        source: str,
-        origin: str = "",
-        base_path: str = "",
-        response_validation: ValidationLevel = ValidationLevel.WARN,
-        disable_server_validation: bool = True,
-        mappings_path: Union[str, Path] = "",
-        invalid_property_default_response: int = 422,
-        default_id_property_name: str = "id",
-        faker_locale: Optional[Union[str, List[str]]] = None,
-        require_body_for_invalid_url: bool = False,
-        recursion_limit: int = 1,
-        recursion_default: Any = {},
-        username: str = "",
-        password: str = "",
-        security_token: str = "",
-        auth: Optional[AuthBase] = None,
-        cert: Optional[Union[str, Tuple[str, str]]] = None,
-        verify_tls: Optional[Union[bool, str]] = True,
-        extra_headers: Optional[Dict[str, str]] = None,
-        cookies: Optional[Union[Dict[str, str], CookieJar]] = None,
-        proxies: Optional[Dict[str, str]] = None,
-    ) -> None:
-        super().__init__(
-            source=source,
-            origin=origin,
-            base_path=base_path,
-            mappings_path=mappings_path,
-            default_id_property_name=default_id_property_name,
-            faker_locale=faker_locale,
-            recursion_limit=recursion_limit,
-            recursion_default=recursion_default,
-            username=username,
-            password=password,
-            security_token=security_token,
-            auth=auth,
-            cert=cert,
-            verify_tls=verify_tls,
-            extra_headers=extra_headers,
-            cookies=cookies,
-            proxies=proxies,
-        )
-        self.response_validation = response_validation
-        self.disable_server_validation = disable_server_validation
-        self.require_body_for_invalid_url = require_body_for_invalid_url
-        self.invalid_property_default_response = invalid_property_default_response
-
-    @keyword
-    def test_unauthorized(self, path: str, method: str) -> None:
-        """
-        Perform a request for `method` on the `path`, with no authorization.
-
-        This keyword only passes if the response code is 401: Unauthorized.
-
-        Any authorization parameters used to initialize the library are
-        ignored for this request.
-        > Note: No headers or (json) body are send with the request. For security
-        reasons, the authorization validation should be checked first.
-        """
-        url: str = run_keyword("get_valid_url", path, method)
-        response = self.session.request(
-            method=method,
-            url=url,
-            verify=False,
-        )
-        assert response.status_code == 401
-
-    @keyword
-    def test_invalid_url(
-        self, path: str, method: str, expected_status_code: int = 404
-    ) -> None:
-        """
-        Perform a request for the provided 'path' and 'method' where the url for
-        the `path` is invalidated.
-
-        This keyword will be `SKIPPED` if the path contains no parts that
-        can be invalidated.
-
-        The optional `expected_status_code` parameter (default: 404) can be set to the
-        expected status code for APIs that do not return a 404 on invalid urls.
-
-        > Note: Depending on API design, the url may be validated before or after
-        validation of headers, query parameters and / or (json) body. By default, no
-        parameters are send with the request. The `require_body_for_invalid_url`
-        parameter can be set to `True` if needed.
-        """
-        valid_url: str = run_keyword("get_valid_url", path, method)
-
-        if not (url := run_keyword("get_invalidated_url", valid_url)):
-            raise SkipExecution(
-                f"Path {path} does not contain resource references that "
-                f"can be invalidated."
-            )
-
-        params, headers, json_data = None, None, None
-        if self.require_body_for_invalid_url:
-            request_data = self.get_request_data(method=method, endpoint=path)
-            params = request_data.params
-            headers = request_data.headers
-            dto = request_data.dto
-            json_data = dto.as_dict()
-        response: Response = run_keyword(
-            "authorized_request", url, method, params, headers, json_data
-        )
-        if response.status_code != expected_status_code:
-            raise AssertionError(
-                f"Response {response.status_code} was not {expected_status_code}"
-            )
-
-    @keyword
-    def test_endpoint(self, path: str, method: str, status_code: int) -> None:
-        """
-        Validate that performing the `method` operation on `path` results in a
-        `status_code` response.
-
-        This is the main keyword to be used in the `Test Template` keyword when using
-        the OpenApiDriver.
-
-        The keyword calls other keywords to generate the neccesary data to perform
-        the desired operation and validate the response against the openapi document.
-        """
-        json_data: Optional[Dict[str, Any]] = None
-        original_data = None
-
-        url: str = run_keyword("get_valid_url", path, method)
-        request_data: RequestData = self.get_request_data(method=method, endpoint=path)
-        params = request_data.params
-        headers = request_data.headers
-        if request_data.has_body:
-            json_data = request_data.dto.as_dict()
-        # when patching, get the original data to check only patched data has changed
-        if method == "PATCH":
-            original_data = self.get_original_data(url=url)
-        # in case of a status code indicating an error, ensure the error occurs
-        if status_code >= 400:
-            invalidation_keyword_data = {
-                "get_invalid_json_data": [
-                    "get_invalid_json_data",
-                    url,
-                    method,
-                    status_code,
-                    request_data,
-                ],
-                "get_invalidated_parameters": [
-                    "get_invalidated_parameters",
-                    status_code,
-                    request_data,
-                ],
-            }
-            invalidation_keywords = []
-
-            if request_data.dto.get_relations_for_error_code(status_code):
-                invalidation_keywords.append("get_invalid_json_data")
-            if request_data.dto.get_parameter_relations_for_error_code(status_code):
-                invalidation_keywords.append("get_invalidated_parameters")
-            if invalidation_keywords:
-                if (
-                    invalidation_keyword := choice(invalidation_keywords)
-                ) == "get_invalid_json_data":
-                    json_data = run_keyword(
-                        *invalidation_keyword_data[invalidation_keyword]
-                    )
-                else:
-                    params, headers = run_keyword(
-                        *invalidation_keyword_data[invalidation_keyword]
-                    )
-            # if there are no relations to invalide and the status_code is the default
-            # response_code for invalid properties, invalidate properties instead
-            elif status_code == self.invalid_property_default_response:
-                if (
-                    request_data.params_that_can_be_invalidated
-                    or request_data.headers_that_can_be_invalidated
-                ):
-                    params, headers = run_keyword(
-                        *invalidation_keyword_data["get_invalidated_parameters"]
-                    )
-                    if request_data.dto_schema:
-                        json_data = run_keyword(
-                            *invalidation_keyword_data["get_invalid_json_data"]
-                        )
-                elif request_data.dto_schema:
-                    json_data = run_keyword(
-                        *invalidation_keyword_data["get_invalid_json_data"]
-                    )
-                else:
-                    raise SkipExecution(
-                        "No properties or parameters can be invalidated."
-                    )
-            else:
-                raise AssertionError(
-                    f"No Dto mapping found to cause status_code {status_code}."
-                )
-        run_keyword(
-            "perform_validated_request",
-            path,
-            status_code,
-            RequestValues(
-                url=url,
-                method=method,
-                params=params,
-                headers=headers,
-                json_data=json_data,
-            ),
-            original_data,
-        )
-        if status_code < 300 and (
-            request_data.has_optional_properties
-            or request_data.has_optional_params
-            or request_data.has_optional_headers
-        ):
-            logger.info("Performing request without optional properties and parameters")
-            url = run_keyword("get_valid_url", path, method)
-            request_data = self.get_request_data(method=method, endpoint=path)
-            params = request_data.get_required_params()
-            headers = request_data.get_required_headers()
-            json_data = request_data.get_required_properties_dict()
-            original_data = None
-            if method == "PATCH":
-                original_data = self.get_original_data(url=url)
-            run_keyword(
-                "perform_validated_request",
-                path,
-                status_code,
-                RequestValues(
-                    url=url,
-                    method=method,
-                    params=params,
-                    headers=headers,
-                    json_data=json_data,
-                ),
-                original_data,
-            )
-
-    def get_original_data(self, url: str) -> Optional[Dict[str, Any]]:
-        """
-        Attempt to GET the current data for the given url and return it.
-
-        If the GET request fails, None is returned.
-        """
-        original_data = None
-        path = self.get_parameterized_endpoint_from_url(url)
-        get_request_data = self.get_request_data(endpoint=path, method="GET")
-        get_params = get_request_data.params
-        get_headers = get_request_data.headers
-        response: Response = run_keyword(
-            "authorized_request", url, "GET", get_params, get_headers
-        )
-        if response.ok:
-            original_data = response.json()
-        return original_data
-
-    @keyword
-    def perform_validated_request(
-        self,
-        path: str,
-        status_code: int,
-        request_values: RequestValues,
-        original_data: Optional[Dict[str, Any]] = None,
-    ) -> None:
-        """
-        This keyword first calls the Authorized Request keyword, then the Validate
-        Response keyword and finally validates, for `DELETE` operations, whether
-        the target resource was indeed deleted (OK response) or not (error responses).
-        """
-        response = run_keyword(
-            "authorized_request",
-            request_values.url,
-            request_values.method,
-            request_values.params,
-            request_values.headers,
-            request_values.json_data,
-        )
-        if response.status_code != status_code:
-            try:
-                response_json = response.json()
-            except Exception as _:  # pylint: disable=broad-except
-                logger.info(
-                    f"Failed to get json content from response. "
-                    f"Response text was: {response.text}"
-                )
-                response_json = {}
-            if not response.ok:
-                if description := response_json.get("detail"):
-                    pass
-                else:
-                    description = response_json.get(
-                        "message", "response contains no message or detail."
-                    )
-                logger.error(f"{response.reason}: {description}")
-
-            logger.debug(
-                f"\nSend: {_json.dumps(request_values.json_data, indent=4, sort_keys=True)}"
-                f"\nGot: {_json.dumps(response_json, indent=4, sort_keys=True)}"
-            )
-            raise AssertionError(
-                f"Response status_code {response.status_code} was not {status_code}"
-            )
-
-        run_keyword("validate_response", path, response, original_data)
-
-        if request_values.method == "DELETE":
-            get_request_data = self.get_request_data(endpoint=path, method="GET")
-            get_params = get_request_data.params
-            get_headers = get_request_data.headers
-            get_response = run_keyword(
-                "authorized_request", request_values.url, "GET", get_params, get_headers
-            )
-            if response.ok:
-                if get_response.ok:
-                    raise AssertionError(
-                        f"Resource still exists after deletion. Url was {request_values.url}"
-                    )
-                # if the path supports GET, 404 is expected, if not 405 is expected
-                if get_response.status_code not in [404, 405]:
-                    logger.warning(
-                        f"Unexpected response after deleting resource: Status_code "
-                        f"{get_response.status_code} was received after trying to get {request_values.url} "
-                        f"after sucessfully deleting it."
-                    )
-            elif not get_response.ok:
-                raise AssertionError(
-                    f"Resource could not be retrieved after failed deletion. "
-                    f"Url was {request_values.url}, status_code was {get_response.status_code}"
-                )
-
-    @keyword
-    def validate_response(
-        self,
-        path: str,
-        response: Response,
-        original_data: Optional[Dict[str, Any]] = None,
-    ) -> None:
-        """
-        Validate the `response` by performing the following validations:
-        - validate the `response` against the openapi schema for the `endpoint`
-        - validate that the response does not contain extra properties
-        - validate that a href, if present, refers to the correct resource
-        - validate that the value for a property that is in the response is equal to
-            the property value that was send
-        - validate that no `original_data` is preserved when performing a PUT operation
-        - validate that a PATCH operation only updates the provided properties
-        """
-        if response.status_code == 204:
-            assert not response.content
-            return None
-
-        try:
-            self._validate_response_against_spec(response)
-        except OpenAPIError:
-            raise Failure("Response did not pass schema validation.")
-
-        request_method = response.request.method
-        if request_method is None:
-            logger.warning(
-                f"Could not validate response for path {path}; no method found "
-                f"on the request property of the provided response."
-            )
-            return None
-
-        response_spec = self._get_response_spec(
-            path=path,
-            method=request_method,
-            status_code=response.status_code,
-        )
-
-        content_type_from_response = response.headers.get("Content-Type", "unknown")
-        mime_type_from_response, _, _ = content_type_from_response.partition(";")
-
-        if not response_spec.get("content"):
-            logger.warning(
-                "The response cannot be validated: 'content' not specified in the OAS."
-            )
-            return None
-
-        # multiple content types can be specified in the OAS
-        content_types = list(response_spec["content"].keys())
-        supported_types = [
-            ct for ct in content_types if ct.partition(";")[0].endswith("json")
-        ]
-        if not supported_types:
-            raise NotImplementedError(
-                f"The content_types '{content_types}' are not supported. "
-                f"Only json types are currently supported."
-            )
-        content_type = supported_types[0]
-        mime_type = content_type.partition(";")[0]
-
-        if mime_type != mime_type_from_response:
-            raise ValueError(
-                f"Content-Type '{content_type_from_response}' of the response "
-                f"does not match '{mime_type}' as specified in the OpenAPI document."
-            )
-
-        json_response = response.json()
-        response_schema = resolve_schema(
-            response_spec["content"][content_type]["schema"]
-        )
-        if list_item_schema := response_schema.get("items"):
-            if not isinstance(json_response, list):
-                raise AssertionError(
-                    f"Response schema violation: the schema specifies an array as "
-                    f"response type but the response was of type {type(json_response)}."
-                )
-            type_of_list_items = list_item_schema.get("type")
-            if type_of_list_items == "object":
-                for resource in json_response:
-                    run_keyword(
-                        "validate_resource_properties", resource, list_item_schema
-                    )
-            else:
-                for item in json_response:
-                    self._validate_value_type(
-                        value=item, expected_type=type_of_list_items
-                    )
-            # no further validation; value validation of individual resources should
-            # be performed on the endpoints for the specific resource
-            return None
-
-        run_keyword("validate_resource_properties", json_response, response_schema)
-        # ensure the href is valid if present in the response
-        if href := json_response.get("href"):
-            self._assert_href_is_valid(href, json_response)
-        # every property that was sucessfully send and that is in the response
-        # schema must have the value that was send
-        if response.ok and response.request.method in ["POST", "PUT", "PATCH"]:
-            run_keyword("validate_send_response", response, original_data)
-        return None
-
-    def _assert_href_is_valid(self, href: str, json_response: Dict[str, Any]) -> None:
-        url = f"{self.origin}{href}"
-        path = url.replace(self.base_url, "")
-        request_data = self.get_request_data(endpoint=path, method="GET")
-        params = request_data.params
-        headers = request_data.headers
-        get_response = run_keyword("authorized_request", url, "GET", params, headers)
-        assert (
-            get_response.json() == json_response
-        ), f"{get_response.json()} not equal to original {json_response}"
-
-    def _validate_response_against_spec(self, response: Response) -> None:
-        try:
-            self.validate_response_vs_spec(
-                request=RequestsOpenAPIRequest(response.request),
-                response=RequestsOpenAPIResponse(response),
-            )
-        except InvalidData as exception:
-            errors: List[InvalidSchemaValue] = exception.__cause__
-            validation_errors: Optional[List[ValidationError]] = getattr(
-                errors, "schema_errors", None
-            )
-            if validation_errors:
-                error_message = "\n".join(
-                    [
-                        f"{list(error.schema_path)}: {error.message}"
-                        for error in validation_errors
-                    ]
-                )
-            else:
-                error_message = str(exception)
-
-            if response.status_code == self.invalid_property_default_response:
-                logger.debug(error_message)
-                return
-            if self.response_validation == ValidationLevel.STRICT:
-                logger.error(error_message)
-                raise exception
-            if self.response_validation == ValidationLevel.WARN:
-                logger.warning(error_message)
-            elif self.response_validation == ValidationLevel.INFO:
-                logger.info(error_message)
-
-    @keyword
-    def validate_resource_properties(
-        self, resource: Dict[str, Any], schema: Dict[str, Any]
-    ) -> None:
-        """
-        Validate that the `resource` does not contain any properties that are not
-        defined in the `schema_properties`.
-        """
-        schema_properties = schema.get("properties", {})
-        property_names_from_schema = set(schema_properties.keys())
-        property_names_in_resource = set(resource.keys())
-
-        if property_names_from_schema != property_names_in_resource:
-            # The additionalProperties property determines whether properties with
-            # unspecified names are allowed. This property can be boolean or an object
-            # (dict) that specifies the type of any additional properties.
-            additional_properties = schema.get("additionalProperties", True)
-            if isinstance(additional_properties, bool):
-                allow_additional_properties = additional_properties
-                allowed_additional_properties_type = None
-            else:
-                allow_additional_properties = True
-                allowed_additional_properties_type = additional_properties["type"]
-
-            extra_property_names = property_names_in_resource.difference(
-                property_names_from_schema
-            )
-            if allow_additional_properties:
-                # If a type is defined for extra properties, validate them
-                if allowed_additional_properties_type:
-                    extra_properties = {
-                        key: value
-                        for key, value in resource.items()
-                        if key in extra_property_names
-                    }
-                    self._validate_type_of_extra_properties(
-                        extra_properties=extra_properties,
-                        expected_type=allowed_additional_properties_type,
-                    )
-                # If allowed, validation should not fail on extra properties
-                extra_property_names = set()
-
-            required_properties = set(schema.get("required", []))
-            missing_properties = required_properties.difference(
-                property_names_in_resource
-            )
-
-            if extra_property_names or missing_properties:
-                extra = (
-                    f"\n\tExtra properties in response: {extra_property_names}"
-                    if extra_property_names
-                    else ""
-                )
-                missing = (
-                    f"\n\tRequired properties missing in response: {missing_properties}"
-                    if missing_properties
-                    else ""
-                )
-                raise AssertionError(
-                    f"Response schema violation: the response contains properties that are "
-                    f"not specified in the schema or does not contain properties that are "
-                    f"required according to the schema."
-                    f"\n\tReceived in the response: {property_names_in_resource}"
-                    f"\n\tDefined in the schema:    {property_names_from_schema}"
-                    f"{extra}{missing}"
-                )
-
-    @staticmethod
-    def _validate_value_type(value: Any, expected_type: str) -> None:
-        type_mapping = {
-            "string": str,
-            "number": float,
-            "integer": int,
-            "boolean": bool,
-            "array": list,
-            "object": dict,
-        }
-        python_type = type_mapping.get(expected_type, None)
-        if python_type is None:
-            raise AssertionError(
-                f"Validation of type '{expected_type}' is not supported."
-            )
-        if not isinstance(value, python_type):
-            raise AssertionError(f"{value} is not of type {expected_type}")
-
-    @staticmethod
-    def _validate_type_of_extra_properties(
-        extra_properties: Dict[str, Any], expected_type: str
-    ) -> None:
-        type_mapping = {
-            "string": str,
-            "number": float,
-            "integer": int,
-            "boolean": bool,
-            "array": list,
-            "object": dict,
-        }
-
-        python_type = type_mapping.get(expected_type, None)
-        if python_type is None:
-            logger.warning(
-                f"Additonal properties were not validated: "
-                f"type '{expected_type}' is not supported."
-            )
-            return
-
-        invalid_extra_properties = {
-            key: value
-            for key, value in extra_properties.items()
-            if not isinstance(value, python_type)
-        }
-        if invalid_extra_properties:
-            raise AssertionError(
-                f"Response contains invalid additionalProperties: "
-                f"{invalid_extra_properties} are not of type {expected_type}."
-            )
-
-    @staticmethod
-    @keyword
-    def validate_send_response(
-        response: Response, original_data: Optional[Dict[str, Any]] = None
-    ) -> None:
-        """
-        Validate that each property that was send that is in the response has the value
-        that was send.
-        In case a PATCH request, validate that only the properties that were patched
-        have changed and that other properties are still at their pre-patch values.
-        """
-
-        def validate_list_response(
-            send_list: List[Any], received_list: List[Any]
-        ) -> None:
-            for item in send_list:
-                if item not in received_list:
-                    raise AssertionError(
-                        f"Received value '{received_list}' does "
-                        f"not contain '{item}' in the {response.request.method} request."
-                        f"\nSend: {_json.dumps(send_json, indent=4, sort_keys=True)}"
-                        f"\nGot: {_json.dumps(response_data, indent=4, sort_keys=True)}"
-                    )
-
-        def validate_dict_response(
-            send_dict: Dict[str, Any], received_dict: Dict[str, Any]
-        ) -> None:
-            for send_property_name, send_property_value in send_dict.items():
-                # sometimes, a property in the request is not in the response, e.g. a password
-                if send_property_name not in received_dict.keys():
-                    continue
-                if send_property_value is not None:
-                    # if a None value is send, the target property should be cleared or
-                    # reverted to the default value (which cannot be specified in the
-                    # openapi document)
-                    received_value = received_dict[send_property_name]
-                    # In case of lists / arrays, the send values are often appended to
-                    # existing data
-                    if isinstance(received_value, list):
-                        validate_list_response(
-                            send_list=send_property_value, received_list=received_value
-                        )
-                        continue
-
-                    # when dealing with objects, we'll need to iterate the properties
-                    if isinstance(received_value, dict):
-                        validate_dict_response(
-                            send_dict=send_property_value, received_dict=received_value
-                        )
-                        continue
-
-                    assert received_value == send_property_value, (
-                        f"Received value for {send_property_name} '{received_value}' does not "
-                        f"match '{send_property_value}' in the {response.request.method} request."
-                        f"\nSend: {_json.dumps(send_json, indent=4, sort_keys=True)}"
-                        f"\nGot: {_json.dumps(response_data, indent=4, sort_keys=True)}"
-                    )
-
-        if response.request.body is None:
-            logger.warning(
-                "Could not validate send response; the body of the request property "
-                "on the provided response was None."
-            )
-            return None
-        if isinstance(response.request.body, bytes):
-            send_json = _json.loads(response.request.body.decode("UTF-8"))
-        else:
-            send_json = _json.loads(response.request.body)
-
-        response_data = response.json()
-        # POST on /resource_type/{id}/array_item/ will return the updated {id} resource
-        # instead of a newly created resource. In this case, the send_json must be
-        # in the array of the 'array_item' property on {id}
-        send_path: str = response.request.path_url
-        response_path = response_data.get("href", None)
-        if response_path and send_path not in response_path:
-            property_to_check = send_path.replace(response_path, "")[1:]
-            if response_data.get(property_to_check) and isinstance(
-                response_data[property_to_check], list
-            ):
-                item_list: List[Dict[str, Any]] = response_data[property_to_check]
-                # Use the (mandatory) id to get the POSTed resource from the list
-                [response_data] = [
-                    item for item in item_list if item["id"] == send_json["id"]
-                ]
-
-        # incoming arguments are dictionaries, so they can be validated as such
-        validate_dict_response(send_dict=send_json, received_dict=response_data)
-
-        # In case of PATCH requests, ensure that only send properties have changed
-        if original_data:
-            for send_property_name, send_value in original_data.items():
-                if send_property_name not in send_json.keys():
-                    assert send_value == response_data[send_property_name], (
-                        f"Received value for {send_property_name} '{response_data[send_property_name]}' does not "
-                        f"match '{send_value}' in the pre-patch data"
-                        f"\nPre-patch: {_json.dumps(original_data, indent=4, sort_keys=True)}"
-                        f"\nGot: {_json.dumps(response_data, indent=4, sort_keys=True)}"
-                    )
-        return None
-
-    def _get_response_spec(
-        self, path: str, method: str, status_code: int
-    ) -> Dict[str, Any]:
-        method = method.lower()
-        status = str(status_code)
-        spec: Dict[str, Any] = {**self.openapi_spec}["paths"][path][method][
-            "responses"
-        ][status]
-        return spec
+"""Module containing the classes to perform automatic OpenAPI contract validation."""
+
+import json as _json
+from enum import Enum
+from logging import getLogger
+from pathlib import Path
+from random import choice
+from typing import Any, Dict, List, Optional, Tuple, Union
+
+from openapi_core.contrib.requests import (
+    RequestsOpenAPIRequest,
+    RequestsOpenAPIResponse,
+)
+from openapi_core.exceptions import OpenAPIError
+from openapi_core.validation.exceptions import ValidationError
+from openapi_core.validation.response.exceptions import InvalidData
+from openapi_core.validation.schemas.exceptions import InvalidSchemaValue
+from requests import Response
+from requests.auth import AuthBase
+from requests.cookies import RequestsCookieJar as CookieJar
+from robot.api import Failure, SkipExecution
+from robot.api.deco import keyword, library
+from robot.libraries.BuiltIn import BuiltIn
+
+from OpenApiLibCore import OpenApiLibCore, RequestData, RequestValues, resolve_schema
+
+run_keyword = BuiltIn().run_keyword
+
+
+logger = getLogger(__name__)
+
+
+class ValidationLevel(str, Enum):
+    """The available levels for the response_validation parameter."""
+
+    DISABLED = "DISABLED"
+    INFO = "INFO"
+    WARN = "WARN"
+    STRICT = "STRICT"
+
+
+@library(scope="TEST SUITE", doc_format="ROBOT")
+class OpenApiExecutors(OpenApiLibCore):  # pylint: disable=too-many-instance-attributes
+    """Main class providing the keywords and core logic to perform endpoint validations."""
+
+    def __init__(  # pylint: disable=too-many-arguments
+        self,
+        source: str,
+        origin: str = "",
+        base_path: str = "",
+        response_validation: ValidationLevel = ValidationLevel.WARN,
+        disable_server_validation: bool = True,
+        mappings_path: Union[str, Path] = "",
+        invalid_property_default_response: int = 422,
+        default_id_property_name: str = "id",
+        faker_locale: Optional[Union[str, List[str]]] = None,
+        require_body_for_invalid_url: bool = False,
+        recursion_limit: int = 1,
+        recursion_default: Any = {},
+        username: str = "",
+        password: str = "",
+        security_token: str = "",
+        auth: Optional[AuthBase] = None,
+        cert: Optional[Union[str, Tuple[str, str]]] = None,
+        verify_tls: Optional[Union[bool, str]] = True,
+        extra_headers: Optional[Dict[str, str]] = None,
+        cookies: Optional[Union[Dict[str, str], CookieJar]] = None,
+        proxies: Optional[Dict[str, str]] = None,
+    ) -> None:
+        super().__init__(
+            source=source,
+            origin=origin,
+            base_path=base_path,
+            mappings_path=mappings_path,
+            default_id_property_name=default_id_property_name,
+            faker_locale=faker_locale,
+            recursion_limit=recursion_limit,
+            recursion_default=recursion_default,
+            username=username,
+            password=password,
+            security_token=security_token,
+            auth=auth,
+            cert=cert,
+            verify_tls=verify_tls,
+            extra_headers=extra_headers,
+            cookies=cookies,
+            proxies=proxies,
+        )
+        self.response_validation = response_validation
+        self.disable_server_validation = disable_server_validation
+        self.require_body_for_invalid_url = require_body_for_invalid_url
+        self.invalid_property_default_response = invalid_property_default_response
+
+    @keyword
+    def test_unauthorized(self, path: str, method: str) -> None:
+        """
+        Perform a request for `method` on the `path`, with no authorization.
+
+        This keyword only passes if the response code is 401: Unauthorized.
+
+        Any authorization parameters used to initialize the library are
+        ignored for this request.
+        > Note: No headers or (json) body are send with the request. For security
+        reasons, the authorization validation should be checked first.
+        """
+        url: str = run_keyword("get_valid_url", path, method)
+        response = self.session.request(
+            method=method,
+            url=url,
+            verify=False,
+        )
+        assert response.status_code == 401
+
+    @keyword
+    def test_invalid_url(
+        self, path: str, method: str, expected_status_code: int = 404
+    ) -> None:
+        """
+        Perform a request for the provided 'path' and 'method' where the url for
+        the `path` is invalidated.
+
+        This keyword will be `SKIPPED` if the path contains no parts that
+        can be invalidated.
+
+        The optional `expected_status_code` parameter (default: 404) can be set to the
+        expected status code for APIs that do not return a 404 on invalid urls.
+
+        > Note: Depending on API design, the url may be validated before or after
+        validation of headers, query parameters and / or (json) body. By default, no
+        parameters are send with the request. The `require_body_for_invalid_url`
+        parameter can be set to `True` if needed.
+        """
+        valid_url: str = run_keyword("get_valid_url", path, method)
+
+        if not (url := run_keyword("get_invalidated_url", valid_url)):
+            raise SkipExecution(
+                f"Path {path} does not contain resource references that "
+                f"can be invalidated."
+            )
+
+        params, headers, json_data = None, None, None
+        if self.require_body_for_invalid_url:
+            request_data = self.get_request_data(method=method, endpoint=path)
+            params = request_data.params
+            headers = request_data.headers
+            dto = request_data.dto
+            json_data = dto.as_dict()
+        response: Response = run_keyword(
+            "authorized_request", url, method, params, headers, json_data
+        )
+        if response.status_code != expected_status_code:
+            raise AssertionError(
+                f"Response {response.status_code} was not {expected_status_code}"
+            )
+
+    @keyword
+    def test_endpoint(self, path: str, method: str, status_code: int) -> None:
+        """
+        Validate that performing the `method` operation on `path` results in a
+        `status_code` response.
+
+        This is the main keyword to be used in the `Test Template` keyword when using
+        the OpenApiDriver.
+
+        The keyword calls other keywords to generate the neccesary data to perform
+        the desired operation and validate the response against the openapi document.
+        """
+        json_data: Optional[Dict[str, Any]] = None
+        original_data = None
+
+        url: str = run_keyword("get_valid_url", path, method)
+        request_data: RequestData = self.get_request_data(method=method, endpoint=path)
+        params = request_data.params
+        headers = request_data.headers
+        if request_data.has_body:
+            json_data = request_data.dto.as_dict()
+        # when patching, get the original data to check only patched data has changed
+        if method == "PATCH":
+            original_data = self.get_original_data(url=url)
+        # in case of a status code indicating an error, ensure the error occurs
+        if status_code >= 400:
+            invalidation_keyword_data = {
+                "get_invalid_json_data": [
+                    "get_invalid_json_data",
+                    url,
+                    method,
+                    status_code,
+                    request_data,
+                ],
+                "get_invalidated_parameters": [
+                    "get_invalidated_parameters",
+                    status_code,
+                    request_data,
+                ],
+            }
+            invalidation_keywords = []
+
+            if request_data.dto.get_relations_for_error_code(status_code):
+                invalidation_keywords.append("get_invalid_json_data")
+            if request_data.dto.get_parameter_relations_for_error_code(status_code):
+                invalidation_keywords.append("get_invalidated_parameters")
+            if invalidation_keywords:
+                if (
+                    invalidation_keyword := choice(invalidation_keywords)
+                ) == "get_invalid_json_data":
+                    json_data = run_keyword(
+                        *invalidation_keyword_data[invalidation_keyword]
+                    )
+                else:
+                    params, headers = run_keyword(
+                        *invalidation_keyword_data[invalidation_keyword]
+                    )
+            # if there are no relations to invalide and the status_code is the default
+            # response_code for invalid properties, invalidate properties instead
+            elif status_code == self.invalid_property_default_response:
+                if (
+                    request_data.params_that_can_be_invalidated
+                    or request_data.headers_that_can_be_invalidated
+                ):
+                    params, headers = run_keyword(
+                        *invalidation_keyword_data["get_invalidated_parameters"]
+                    )
+                    if request_data.dto_schema:
+                        json_data = run_keyword(
+                            *invalidation_keyword_data["get_invalid_json_data"]
+                        )
+                elif request_data.dto_schema:
+                    json_data = run_keyword(
+                        *invalidation_keyword_data["get_invalid_json_data"]
+                    )
+                else:
+                    raise SkipExecution(
+                        "No properties or parameters can be invalidated."
+                    )
+            else:
+                raise AssertionError(
+                    f"No Dto mapping found to cause status_code {status_code}."
+                )
+        run_keyword(
+            "perform_validated_request",
+            path,
+            status_code,
+            RequestValues(
+                url=url,
+                method=method,
+                params=params,
+                headers=headers,
+                json_data=json_data,
+            ),
+            original_data,
+        )
+        if status_code < 300 and (
+            request_data.has_optional_properties
+            or request_data.has_optional_params
+            or request_data.has_optional_headers
+        ):
+            logger.info("Performing request without optional properties and parameters")
+            url = run_keyword("get_valid_url", path, method)
+            request_data = self.get_request_data(method=method, endpoint=path)
+            params = request_data.get_required_params()
+            headers = request_data.get_required_headers()
+            json_data = (
+                request_data.get_required_properties_dict()
+                if request_data.has_body
+                else None
+            )
+            original_data = None
+            if method == "PATCH":
+                original_data = self.get_original_data(url=url)
+            run_keyword(
+                "perform_validated_request",
+                path,
+                status_code,
+                RequestValues(
+                    url=url,
+                    method=method,
+                    params=params,
+                    headers=headers,
+                    json_data=json_data,
+                ),
+                original_data,
+            )
+
+    def get_original_data(self, url: str) -> Optional[Dict[str, Any]]:
+        """
+        Attempt to GET the current data for the given url and return it.
+
+        If the GET request fails, None is returned.
+        """
+        original_data = None
+        path = self.get_parameterized_endpoint_from_url(url)
+        get_request_data = self.get_request_data(endpoint=path, method="GET")
+        get_params = get_request_data.params
+        get_headers = get_request_data.headers
+        response: Response = run_keyword(
+            "authorized_request", url, "GET", get_params, get_headers
+        )
+        if response.ok:
+            original_data = response.json()
+        return original_data
+
+    @keyword
+    def perform_validated_request(
+        self,
+        path: str,
+        status_code: int,
+        request_values: RequestValues,
+        original_data: Optional[Dict[str, Any]] = None,
+    ) -> None:
+        """
+        This keyword first calls the Authorized Request keyword, then the Validate
+        Response keyword and finally validates, for `DELETE` operations, whether
+        the target resource was indeed deleted (OK response) or not (error responses).
+        """
+        response = run_keyword(
+            "authorized_request",
+            request_values.url,
+            request_values.method,
+            request_values.params,
+            request_values.headers,
+            request_values.json_data,
+        )
+        if response.status_code != status_code:
+            try:
+                response_json = response.json()
+            except Exception as _:  # pylint: disable=broad-except
+                logger.info(
+                    f"Failed to get json content from response. "
+                    f"Response text was: {response.text}"
+                )
+                response_json = {}
+            if not response.ok:
+                if description := response_json.get("detail"):
+                    pass
+                else:
+                    description = response_json.get(
+                        "message", "response contains no message or detail."
+                    )
+                logger.error(f"{response.reason}: {description}")
+
+            logger.debug(
+                f"\nSend: {_json.dumps(request_values.json_data, indent=4, sort_keys=True)}"
+                f"\nGot: {_json.dumps(response_json, indent=4, sort_keys=True)}"
+            )
+            raise AssertionError(
+                f"Response status_code {response.status_code} was not {status_code}"
+            )
+
+        run_keyword("validate_response", path, response, original_data)
+
+        if request_values.method == "DELETE":
+            get_request_data = self.get_request_data(endpoint=path, method="GET")
+            get_params = get_request_data.params
+            get_headers = get_request_data.headers
+            get_response = run_keyword(
+                "authorized_request", request_values.url, "GET", get_params, get_headers
+            )
+            if response.ok:
+                if get_response.ok:
+                    raise AssertionError(
+                        f"Resource still exists after deletion. Url was {request_values.url}"
+                    )
+                # if the path supports GET, 404 is expected, if not 405 is expected
+                if get_response.status_code not in [404, 405]:
+                    logger.warning(
+                        f"Unexpected response after deleting resource: Status_code "
+                        f"{get_response.status_code} was received after trying to get {request_values.url} "
+                        f"after sucessfully deleting it."
+                    )
+            elif not get_response.ok:
+                raise AssertionError(
+                    f"Resource could not be retrieved after failed deletion. "
+                    f"Url was {request_values.url}, status_code was {get_response.status_code}"
+                )
+
+    @keyword
+    def validate_response(
+        self,
+        path: str,
+        response: Response,
+        original_data: Optional[Dict[str, Any]] = None,
+    ) -> None:
+        """
+        Validate the `response` by performing the following validations:
+        - validate the `response` against the openapi schema for the `endpoint`
+        - validate that the response does not contain extra properties
+        - validate that a href, if present, refers to the correct resource
+        - validate that the value for a property that is in the response is equal to
+            the property value that was send
+        - validate that no `original_data` is preserved when performing a PUT operation
+        - validate that a PATCH operation only updates the provided properties
+        """
+        if response.status_code == 204:
+            assert not response.content
+            return None
+
+        try:
+            self._validate_response_against_spec(response)
+        except OpenAPIError:
+            raise Failure("Response did not pass schema validation.")
+
+        request_method = response.request.method
+        if request_method is None:
+            logger.warning(
+                f"Could not validate response for path {path}; no method found "
+                f"on the request property of the provided response."
+            )
+            return None
+
+        response_spec = self._get_response_spec(
+            path=path,
+            method=request_method,
+            status_code=response.status_code,
+        )
+
+        content_type_from_response = response.headers.get("Content-Type", "unknown")
+        mime_type_from_response, _, _ = content_type_from_response.partition(";")
+
+        if not response_spec.get("content"):
+            logger.warning(
+                "The response cannot be validated: 'content' not specified in the OAS."
+            )
+            return None
+
+        # multiple content types can be specified in the OAS
+        content_types = list(response_spec["content"].keys())
+        supported_types = [
+            ct for ct in content_types if ct.partition(";")[0].endswith("json")
+        ]
+        if not supported_types:
+            raise NotImplementedError(
+                f"The content_types '{content_types}' are not supported. "
+                f"Only json types are currently supported."
+            )
+        content_type = supported_types[0]
+        mime_type = content_type.partition(";")[0]
+
+        if mime_type != mime_type_from_response:
+            raise ValueError(
+                f"Content-Type '{content_type_from_response}' of the response "
+                f"does not match '{mime_type}' as specified in the OpenAPI document."
+            )
+
+        json_response = response.json()
+        response_schema = resolve_schema(
+            response_spec["content"][content_type]["schema"]
+        )
+        if list_item_schema := response_schema.get("items"):
+            if not isinstance(json_response, list):
+                raise AssertionError(
+                    f"Response schema violation: the schema specifies an array as "
+                    f"response type but the response was of type {type(json_response)}."
+                )
+            type_of_list_items = list_item_schema.get("type")
+            if type_of_list_items == "object":
+                for resource in json_response:
+                    run_keyword(
+                        "validate_resource_properties", resource, list_item_schema
+                    )
+            else:
+                for item in json_response:
+                    self._validate_value_type(
+                        value=item, expected_type=type_of_list_items
+                    )
+            # no further validation; value validation of individual resources should
+            # be performed on the endpoints for the specific resource
+            return None
+
+        run_keyword("validate_resource_properties", json_response, response_schema)
+        # ensure the href is valid if present in the response
+        if href := json_response.get("href"):
+            self._assert_href_is_valid(href, json_response)
+        # every property that was sucessfully send and that is in the response
+        # schema must have the value that was send
+        if response.ok and response.request.method in ["POST", "PUT", "PATCH"]:
+            run_keyword("validate_send_response", response, original_data)
+        return None
+
+    def _assert_href_is_valid(self, href: str, json_response: Dict[str, Any]) -> None:
+        url = f"{self.origin}{href}"
+        path = url.replace(self.base_url, "")
+        request_data = self.get_request_data(endpoint=path, method="GET")
+        params = request_data.params
+        headers = request_data.headers
+        get_response = run_keyword("authorized_request", url, "GET", params, headers)
+        assert (
+            get_response.json() == json_response
+        ), f"{get_response.json()} not equal to original {json_response}"
+
+    def _validate_response_against_spec(self, response: Response) -> None:
+        try:
+            self.validate_response_vs_spec(
+                request=RequestsOpenAPIRequest(response.request),
+                response=RequestsOpenAPIResponse(response),
+            )
+        except InvalidData as exception:
+            errors: List[InvalidSchemaValue] = exception.__cause__
+            validation_errors: Optional[List[ValidationError]] = getattr(
+                errors, "schema_errors", None
+            )
+            if validation_errors:
+                error_message = "\n".join(
+                    [
+                        f"{list(error.schema_path)}: {error.message}"
+                        for error in validation_errors
+                    ]
+                )
+            else:
+                error_message = str(exception)
+
+            if response.status_code == self.invalid_property_default_response:
+                logger.debug(error_message)
+                return
+            if self.response_validation == ValidationLevel.STRICT:
+                logger.error(error_message)
+                raise exception
+            if self.response_validation == ValidationLevel.WARN:
+                logger.warning(error_message)
+            elif self.response_validation == ValidationLevel.INFO:
+                logger.info(error_message)
+
+    @keyword
+    def validate_resource_properties(
+        self, resource: Dict[str, Any], schema: Dict[str, Any]
+    ) -> None:
+        """
+        Validate that the `resource` does not contain any properties that are not
+        defined in the `schema_properties`.
+        """
+        schema_properties = schema.get("properties", {})
+        property_names_from_schema = set(schema_properties.keys())
+        property_names_in_resource = set(resource.keys())
+
+        if property_names_from_schema != property_names_in_resource:
+            # The additionalProperties property determines whether properties with
+            # unspecified names are allowed. This property can be boolean or an object
+            # (dict) that specifies the type of any additional properties.
+            additional_properties = schema.get("additionalProperties", True)
+            if isinstance(additional_properties, bool):
+                allow_additional_properties = additional_properties
+                allowed_additional_properties_type = None
+            else:
+                allow_additional_properties = True
+                allowed_additional_properties_type = additional_properties["type"]
+
+            extra_property_names = property_names_in_resource.difference(
+                property_names_from_schema
+            )
+            if allow_additional_properties:
+                # If a type is defined for extra properties, validate them
+                if allowed_additional_properties_type:
+                    extra_properties = {
+                        key: value
+                        for key, value in resource.items()
+                        if key in extra_property_names
+                    }
+                    self._validate_type_of_extra_properties(
+                        extra_properties=extra_properties,
+                        expected_type=allowed_additional_properties_type,
+                    )
+                # If allowed, validation should not fail on extra properties
+                extra_property_names = set()
+
+            required_properties = set(schema.get("required", []))
+            missing_properties = required_properties.difference(
+                property_names_in_resource
+            )
+
+            if extra_property_names or missing_properties:
+                extra = (
+                    f"\n\tExtra properties in response: {extra_property_names}"
+                    if extra_property_names
+                    else ""
+                )
+                missing = (
+                    f"\n\tRequired properties missing in response: {missing_properties}"
+                    if missing_properties
+                    else ""
+                )
+                raise AssertionError(
+                    f"Response schema violation: the response contains properties that are "
+                    f"not specified in the schema or does not contain properties that are "
+                    f"required according to the schema."
+                    f"\n\tReceived in the response: {property_names_in_resource}"
+                    f"\n\tDefined in the schema:    {property_names_from_schema}"
+                    f"{extra}{missing}"
+                )
+
+    @staticmethod
+    def _validate_value_type(value: Any, expected_type: str) -> None:
+        type_mapping = {
+            "string": str,
+            "number": float,
+            "integer": int,
+            "boolean": bool,
+            "array": list,
+            "object": dict,
+        }
+        python_type = type_mapping.get(expected_type, None)
+        if python_type is None:
+            raise AssertionError(
+                f"Validation of type '{expected_type}' is not supported."
+            )
+        if not isinstance(value, python_type):
+            raise AssertionError(f"{value} is not of type {expected_type}")
+
+    @staticmethod
+    def _validate_type_of_extra_properties(
+        extra_properties: Dict[str, Any], expected_type: str
+    ) -> None:
+        type_mapping = {
+            "string": str,
+            "number": float,
+            "integer": int,
+            "boolean": bool,
+            "array": list,
+            "object": dict,
+        }
+
+        python_type = type_mapping.get(expected_type, None)
+        if python_type is None:
+            logger.warning(
+                f"Additonal properties were not validated: "
+                f"type '{expected_type}' is not supported."
+            )
+            return
+
+        invalid_extra_properties = {
+            key: value
+            for key, value in extra_properties.items()
+            if not isinstance(value, python_type)
+        }
+        if invalid_extra_properties:
+            raise AssertionError(
+                f"Response contains invalid additionalProperties: "
+                f"{invalid_extra_properties} are not of type {expected_type}."
+            )
+
+    @staticmethod
+    @keyword
+    def validate_send_response(
+        response: Response, original_data: Optional[Dict[str, Any]] = None
+    ) -> None:
+        """
+        Validate that each property that was send that is in the response has the value
+        that was send.
+        In case a PATCH request, validate that only the properties that were patched
+        have changed and that other properties are still at their pre-patch values.
+        """
+
+        def validate_list_response(
+            send_list: List[Any], received_list: List[Any]
+        ) -> None:
+            for item in send_list:
+                if item not in received_list:
+                    raise AssertionError(
+                        f"Received value '{received_list}' does "
+                        f"not contain '{item}' in the {response.request.method} request."
+                        f"\nSend: {_json.dumps(send_json, indent=4, sort_keys=True)}"
+                        f"\nGot: {_json.dumps(response_data, indent=4, sort_keys=True)}"
+                    )
+
+        def validate_dict_response(
+            send_dict: Dict[str, Any], received_dict: Dict[str, Any]
+        ) -> None:
+            for send_property_name, send_property_value in send_dict.items():
+                # sometimes, a property in the request is not in the response, e.g. a password
+                if send_property_name not in received_dict.keys():
+                    continue
+                if send_property_value is not None:
+                    # if a None value is send, the target property should be cleared or
+                    # reverted to the default value (which cannot be specified in the
+                    # openapi document)
+                    received_value = received_dict[send_property_name]
+                    # In case of lists / arrays, the send values are often appended to
+                    # existing data
+                    if isinstance(received_value, list):
+                        validate_list_response(
+                            send_list=send_property_value, received_list=received_value
+                        )
+                        continue
+
+                    # when dealing with objects, we'll need to iterate the properties
+                    if isinstance(received_value, dict):
+                        validate_dict_response(
+                            send_dict=send_property_value, received_dict=received_value
+                        )
+                        continue
+
+                    assert received_value == send_property_value, (
+                        f"Received value for {send_property_name} '{received_value}' does not "
+                        f"match '{send_property_value}' in the {response.request.method} request."
+                        f"\nSend: {_json.dumps(send_json, indent=4, sort_keys=True)}"
+                        f"\nGot: {_json.dumps(response_data, indent=4, sort_keys=True)}"
+                    )
+
+        if response.request.body is None:
+            logger.warning(
+                "Could not validate send response; the body of the request property "
+                "on the provided response was None."
+            )
+            return None
+        if isinstance(response.request.body, bytes):
+            send_json = _json.loads(response.request.body.decode("UTF-8"))
+        else:
+            send_json = _json.loads(response.request.body)
+
+        response_data = response.json()
+        # POST on /resource_type/{id}/array_item/ will return the updated {id} resource
+        # instead of a newly created resource. In this case, the send_json must be
+        # in the array of the 'array_item' property on {id}
+        send_path: str = response.request.path_url
+        response_path = response_data.get("href", None)
+        if response_path and send_path not in response_path:
+            property_to_check = send_path.replace(response_path, "")[1:]
+            if response_data.get(property_to_check) and isinstance(
+                response_data[property_to_check], list
+            ):
+                item_list: List[Dict[str, Any]] = response_data[property_to_check]
+                # Use the (mandatory) id to get the POSTed resource from the list
+                [response_data] = [
+                    item for item in item_list if item["id"] == send_json["id"]
+                ]
+
+        # incoming arguments are dictionaries, so they can be validated as such
+        validate_dict_response(send_dict=send_json, received_dict=response_data)
+
+        # In case of PATCH requests, ensure that only send properties have changed
+        if original_data:
+            for send_property_name, send_value in original_data.items():
+                if send_property_name not in send_json.keys():
+                    assert send_value == response_data[send_property_name], (
+                        f"Received value for {send_property_name} '{response_data[send_property_name]}' does not "
+                        f"match '{send_value}' in the pre-patch data"
+                        f"\nPre-patch: {_json.dumps(original_data, indent=4, sort_keys=True)}"
+                        f"\nGot: {_json.dumps(response_data, indent=4, sort_keys=True)}"
+                    )
+        return None
+
+    def _get_response_spec(
+        self, path: str, method: str, status_code: int
+    ) -> Dict[str, Any]:
+        method = method.lower()
+        status = str(status_code)
+        spec: Dict[str, Any] = {**self.openapi_spec}["paths"][path][method][
+            "responses"
+        ][status]
+        return spec
```

### Comparing `robotframework_openapitools-0.1.2/src/OpenApiDriver/openapi_reader.py` & `robotframework_openapitools-0.1.3/src/OpenApiDriver/openapi_reader.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.2/src/OpenApiDriver/openapidriver.libspec` & `robotframework_openapitools-0.1.3/src/OpenApiDriver/openapidriver.libspec`

 * *Files 0% similar despite different names*

#### Comparing `robotframework_openapitools-0.1.2/src/OpenApiDriver/openapidriver.libspec` & `robotframework_openapitools-0.1.3/src/OpenApiDriver/openapidriver.libspec`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
-<keywordspec name="OpenApiDriver" type="LIBRARY" format="HTML" scope="SUITE" generated="2024-03-15T20:27:51+00:00" specversion="5" source="/workspaces/robotframework-openapitools/src/OpenApiDriver/openapidriver.py" lineno="352">
-  <version>0.1.2</version>
+<keywordspec name="OpenApiDriver" type="LIBRARY" format="HTML" scope="SUITE" generated="2024-04-05T14:47:49+00:00" specversion="5" source="/workspaces/robotframework-openapitools/src/OpenApiDriver/openapidriver.py" lineno="352">
+  <version>0.1.3</version>
   <doc>&lt;p&gt;Visit the &lt;a href=&quot;https://github.com/MarketSquare/robotframework-openapidriver&quot;&gt;library page&lt;/a&gt; for an introduction and examples.&lt;/p&gt;</doc>
   <tags/>
   <inits>
     <init name="__init__" lineno="144">
       <arguments repr="source: str, origin: str = , base_path: str = , included_paths: Iterable[str] | None = None, ignored_paths: Iterable[str] | None = None, ignored_responses: Iterable[int] | None = None, ignored_testcases: Iterable[Tuple[str, str, int]] | None = None, response_validation: ValidationLevel = WARN, disable_server_validation: bool = True, mappings_path: str | Path = , invalid_property_default_response: int = 422, default_id_property_name: str = id, faker_locale: str | List[str] | None = None, require_body_for_invalid_url: bool = False, recursion_limit: int = 1, recursion_default: Any = {}, username: str = , password: str = , security_token: str = , auth: AuthBase | None = None, cert: str | Tuple[str, str] | None = None, verify_tls: bool | str | None = True, extra_headers: Dict[str, str] | None = None, cookies: Dict[str, str] | RequestsCookieJar | None = None, proxies: Dict[str, str] | None = None">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="source: str">
           <name>source</name>
```

### Comparing `robotframework_openapitools-0.1.2/src/OpenApiDriver/openapidriver.py` & `robotframework_openapitools-0.1.3/src/OpenApiDriver/openapidriver.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.2/src/OpenApiLibCore/__init__.py` & `robotframework_openapitools-0.1.3/src/OpenApiLibCore/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.2/src/OpenApiLibCore/dto_base.py` & `robotframework_openapitools-0.1.3/src/OpenApiLibCore/dto_base.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.2/src/OpenApiLibCore/dto_utils.py` & `robotframework_openapitools-0.1.3/src/OpenApiLibCore/dto_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.2/src/OpenApiLibCore/openapi_libcore.libspec` & `robotframework_openapitools-0.1.3/src/OpenApiLibCore/openapi_libcore.libspec`

 * *Files 0% similar despite different names*

#### Comparing `robotframework_openapitools-0.1.2/src/OpenApiLibCore/openapi_libcore.libspec` & `robotframework_openapitools-0.1.3/src/OpenApiLibCore/openapi_libcore.libspec`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
-<keywordspec name="OpenApiLibCore" type="LIBRARY" format="HTML" scope="SUITE" generated="2024-03-15T20:27:50+00:00" specversion="5" source="/workspaces/robotframework-openapitools/src/OpenApiLibCore/openapi_libcore.py" lineno="377">
-  <version>0.1.2</version>
+<keywordspec name="OpenApiLibCore" type="LIBRARY" format="HTML" scope="SUITE" generated="2024-04-05T14:47:48+00:00" specversion="5" source="/workspaces/robotframework-openapitools/src/OpenApiLibCore/openapi_libcore.py" lineno="377">
+  <version>0.1.3</version>
   <doc>&lt;p&gt;Main class providing the keywords and core logic to interact with an OpenAPI server.&lt;/p&gt;
 &lt;p&gt;Visit the &lt;a href=&quot;https://github.com/MarketSquare/robotframework-openapi-libcore&quot;&gt;library page&lt;/a&gt; for an introduction.&lt;/p&gt;</doc>
   <tags/>
   <inits>
     <init name="__init__" lineno="385">
       <arguments repr="source: str, origin: str = , base_path: str = , mappings_path: str | Path = , invalid_property_default_response: int = 422, default_id_property_name: str = id, faker_locale: str | List[str] | None = None, recursion_limit: int = 1, recursion_default: Any = {}, username: str = , password: str = , security_token: str = , auth: AuthBase | None = None, cert: str | Tuple[str, str] | None = None, verify_tls: bool | str | None = True, extra_headers: Dict[str, str] | None = None, cookies: Dict[str, str] | RequestsCookieJar | None = None, proxies: Dict[str, str] | None = None">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="source: str">
@@ -194,15 +194,15 @@
 &lt;p&gt;A dictionary or &lt;a href=&quot;https://docs.python.org/3/library/http.cookiejar.html#http.cookiejar.CookieJar&quot;&gt;CookieJar object&lt;/a&gt; to send with all requests.&lt;/p&gt;
 &lt;h4&gt;proxies&lt;/h4&gt;
 &lt;p&gt;A dictionary of 'protocol': 'proxy url' to use for all requests.&lt;/p&gt;</doc>
       <shortdoc>== Base parameters ==</shortdoc>
     </init>
   </inits>
   <keywords>
-    <kw name="Authorized Request" lineno="1477">
+    <kw name="Authorized Request" lineno="1490">
       <arguments repr="url: str, method: str, params: Dict[str, Any] | None = None, headers: Dict[str, str] | None = None, json_data: Dict[str, Dict[str, ForwardRef('JSON')] | List[ForwardRef('JSON')] | str | int | float | bool | None] | List[Dict[str, ForwardRef('JSON')] | List[ForwardRef('JSON')] | str | int | float | bool | None] | str | int | float | bool | None = None">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -288,39 +288,39 @@
           <default>None</default>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Perform a request using the security token or authentication set in the library.&lt;/p&gt;
 &lt;p&gt;&amp;gt; Note: provided username / password or auth objects take precedence over token based security&lt;/p&gt;</doc>
       <shortdoc>Perform a request using the security token or authentication set in the library.</shortdoc>
     </kw>
-    <kw name="Ensure In Use" lineno="1381">
+    <kw name="Ensure In Use" lineno="1394">
       <arguments repr="url: str, resource_relation: IdReference">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="resource_relation: IdReference">
           <name>resource_relation</name>
           <type name="IdReference">IdReference</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Ensure that the (right-most) &lt;span class=&quot;name&quot;&gt;id&lt;/span&gt; of the resource referenced by the &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt; is used by the resource defined by the &lt;span class=&quot;name&quot;&gt;resource_relation&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Ensure that the (right-most) `id` of the resource referenced by the `url` is used by the resource defined by the `resource_relation`.</shortdoc>
     </kw>
-    <kw name="Get Ids From Url" lineno="779">
+    <kw name="Get Ids From Url" lineno="783">
       <arguments repr="url: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Perform a GET request on the &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt; and return the list of resource &lt;span class=&quot;name&quot;&gt;ids&lt;/span&gt; from the response.&lt;/p&gt;</doc>
       <shortdoc>Perform a GET request on the `url` and return the list of resource `ids` from the response.</shortdoc>
     </kw>
-    <kw name="Get Invalid Json Data" lineno="1158">
+    <kw name="Get Invalid Json Data" lineno="1171">
       <arguments repr="url: str, method: str, status_code: int, request_data: RequestData">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -335,40 +335,40 @@
           <type name="RequestData">RequestData</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return &lt;span class=&quot;name&quot;&gt;json_data&lt;/span&gt; based on the &lt;span class=&quot;name&quot;&gt;dto&lt;/span&gt; on the &lt;span class=&quot;name&quot;&gt;request_data&lt;/span&gt; that will cause the provided &lt;span class=&quot;name&quot;&gt;status_code&lt;/span&gt; for the &lt;span class=&quot;name&quot;&gt;method&lt;/span&gt; operation on the &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt;.&lt;/p&gt;
 &lt;p&gt;&amp;gt; Note: applicable UniquePropertyValueConstraint and IdReference Relations are considered before changes to &lt;span class=&quot;name&quot;&gt;json_data&lt;/span&gt; are made.&lt;/p&gt;</doc>
       <shortdoc>Return `json_data` based on the `dto` on the `request_data` that will cause the provided `status_code` for the `method` operation on the `url`.</shortdoc>
     </kw>
-    <kw name="Get Invalidated Parameters" lineno="1206">
+    <kw name="Get Invalidated Parameters" lineno="1219">
       <arguments repr="status_code: int, request_data: RequestData">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="status_code: int">
           <name>status_code</name>
           <type name="int" typedoc="integer">int</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="request_data: RequestData">
           <name>request_data</name>
           <type name="RequestData">RequestData</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Returns a version of &lt;span class=&quot;name&quot;&gt;params, headers&lt;/span&gt; as present on &lt;span class=&quot;name&quot;&gt;request_data&lt;/span&gt; that has been modified to cause the provided &lt;span class=&quot;name&quot;&gt;status_code&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Returns a version of `params, headers` as present on `request_data` that has been modified to cause the provided `status_code`.</shortdoc>
     </kw>
-    <kw name="Get Invalidated Url" lineno="1124">
+    <kw name="Get Invalidated Url" lineno="1137">
       <arguments repr="valid_url: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="valid_url: str">
           <name>valid_url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return an url with all the path parameters in the &lt;span class=&quot;name&quot;&gt;valid_url&lt;/span&gt; replaced by a random UUID.&lt;/p&gt;
 &lt;p&gt;Raises ValueError if the valid_url cannot be invalidated.&lt;/p&gt;</doc>
       <shortdoc>Return an url with all the path parameters in the `valid_url` replaced by a random UUID.</shortdoc>
     </kw>
-    <kw name="Get Json Data For Dto Class" lineno="1027">
+    <kw name="Get Json Data For Dto Class" lineno="1031">
       <arguments repr="schema: Dict[str, Any], dto_class: Dto | Type[Dto], operation_id: str = ">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="schema: Dict[str, Any]">
           <name>schema</name>
           <type name="Dict" typedoc="dictionary">
             Dict[str, Any]
             <type name="str" typedoc="string">str</type>
             <type name="Any" typedoc="Any">Any</type>
@@ -390,15 +390,15 @@
           <type name="str" typedoc="string">str</type>
           <default/>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Generate a valid (json-compatible) dict for all the &lt;span class=&quot;name&quot;&gt;dto_class&lt;/span&gt; properties.&lt;/p&gt;</doc>
       <shortdoc>Generate a valid (json-compatible) dict for all the `dto_class` properties.</shortdoc>
     </kw>
-    <kw name="Get Json Data With Conflict" lineno="1425">
+    <kw name="Get Json Data With Conflict" lineno="1438">
       <arguments repr="url: str, method: str, dto: Dto, conflict_status_code: int">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -412,54 +412,54 @@
           <name>conflict_status_code</name>
           <type name="int" typedoc="integer">int</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return &lt;span class=&quot;name&quot;&gt;json_data&lt;/span&gt; based on the &lt;span class=&quot;name&quot;&gt;UniquePropertyValueConstraint&lt;/span&gt; that must be returned by the &lt;span class=&quot;name&quot;&gt;get_relations&lt;/span&gt; implementation on the &lt;span class=&quot;name&quot;&gt;dto&lt;/span&gt; for the given &lt;span class=&quot;name&quot;&gt;conflict_status_code&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Return `json_data` based on the `UniquePropertyValueConstraint` that must be returned by the `get_relations` implementation on the `dto` for the given `conflict_status_code`.</shortdoc>
     </kw>
-    <kw name="Get Parameterized Endpoint From Url" lineno="1146">
+    <kw name="Get Parameterized Endpoint From Url" lineno="1159">
       <arguments repr="url: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return the endpoint as found in the &lt;span class=&quot;name&quot;&gt;paths&lt;/span&gt; section based on the given &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Return the endpoint as found in the `paths` section based on the given `url`.</shortdoc>
     </kw>
-    <kw name="Get Request Data" lineno="819">
+    <kw name="Get Request Data" lineno="823">
       <arguments repr="endpoint: str, method: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="endpoint: str">
           <name>endpoint</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
           <type name="str" typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return an object with valid request data for body, headers and query params.&lt;/p&gt;</doc>
       <shortdoc>Return an object with valid request data for body, headers and query params.</shortdoc>
     </kw>
-    <kw name="Get Valid Id For Endpoint" lineno="683">
+    <kw name="Get Valid Id For Endpoint" lineno="687">
       <arguments repr="endpoint: str, method: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="endpoint: str">
           <name>endpoint</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
           <type name="str" typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Support keyword that returns the &lt;span class=&quot;name&quot;&gt;id&lt;/span&gt; for an existing resource at &lt;span class=&quot;name&quot;&gt;endpoint&lt;/span&gt;.&lt;/p&gt;
 &lt;p&gt;To prevent resource conflicts with other test cases, a new resource is created (POST) if possible.&lt;/p&gt;</doc>
       <shortdoc>Support keyword that returns the `id` for an existing resource at `endpoint`.</shortdoc>
     </kw>
-    <kw name="Get Valid Url" lineno="643">
+    <kw name="Get Valid Url" lineno="647">
       <arguments repr="endpoint: str, method: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="endpoint: str">
           <name>endpoint</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
```

### Comparing `robotframework_openapitools-0.1.2/src/OpenApiLibCore/openapi_libcore.py` & `robotframework_openapitools-0.1.3/src/OpenApiLibCore/openapi_libcore.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,1512 +1,1525 @@
-"""
-# OpenApiLibCore for Robot Framework
-
-The OpenApiLibCore library is a utility library that is meant to simplify creation
-of other Robot Framework libraries for API testing based on the information in
-an OpenAPI document (also known as Swagger document).
-This document explains how to use the OpenApiLibCore library.
-
-My RoboCon 2022 talk about OpenApiDriver and OpenApiLibCore can be found
-[here](https://www.youtube.com/watch?v=7YWZEHxk9Ps)
-
-For more information about Robot Framework, see http://robotframework.org.
-
----
-
-> Note: OpenApiLibCore is still being developed so there are currently
-restrictions / limitations that you may encounter when using this library to run
-tests against an API. See [Limitations](#limitations) for details.
-
----
-
-## Installation
-
-If you already have Python >= 3.8 with pip installed, you can simply run:
-
-`pip install --upgrade robotframework-openapi-libcore`
-
----
-
-## OpenAPI (aka Swagger)
-
-The OpenAPI Specification (OAS) defines a standard, language-agnostic interface
-to RESTful APIs, see https://swagger.io/specification/
-
-The OpenApiLibCore implements a number of Robot Framework keywords that make it
-easy to interact with an OpenAPI implementation by using the information in the
-openapi document (Swagger file), for examply by automatic generation of valid values
-for requests based on the schema information in the document.
-
-> Note: OpenApiLibCore is designed for APIs based on the OAS v3
-The library has not been tested for APIs based on the OAS v2.
-
----
-
-## Getting started
-
-Before trying to use the keywords exposed by OpenApiLibCore on the target API
-it's recommended to first ensure that the openapi document for the API is valid
-under the OpenAPI Specification.
-
-This can be done using the command line interface of a package that is installed as
-a prerequisite for OpenApiLibCore.
-Both a local openapi.json or openapi.yaml file or one hosted by the API server
-can be checked using the `prance validate <reference_to_file>` shell command:
-
-```shell
-prance validate --backend=openapi-spec-validator http://localhost:8000/openapi.json
-Processing "http://localhost:8000/openapi.json"...
- -> Resolving external references.
-Validates OK as OpenAPI 3.0.2!
-
-prance validate --backend=openapi-spec-validator /tests/files/petstore_openapi.yaml
-Processing "/tests/files/petstore_openapi.yaml"...
- -> Resolving external references.
-Validates OK as OpenAPI 3.0.2!
-```
-
-You'll have to change the url or file reference to the location of the openapi
-document for your API.
-
-> Note: Although recursion is technically allowed under the OAS, tool support is limited
-and changing the OAS to not use recursion is recommended.
-OpenApiLibCore has limited support for parsing OpenAPI documents with
-recursion in them. See the `recursion_limit` and `recursion_default` parameters.
-
-If the openapi document passes this validation, the next step is trying to do a test
-run with a minimal test suite.
-The example below can be used, with `source`, `origin` and 'endpoint' altered to
-fit your situation.
-
-``` robotframework
-*** Settings ***
-Library            OpenApiLibCore
-...                    source=http://localhost:8000/openapi.json
-...                    origin=http://localhost:8000
-
-*** Test Cases ***
-Getting Started
-    ${url}=    Get Valid Url    endpoint=/employees/{employee_id}   method=get
-
-```
-
-Running the above suite for the first time may result in an error / failed test.
-You should look at the Robot Framework `log.html` to determine the reasons
-for the failing tests.
-Depending on the reasons for the failures, different solutions are possible.
-
-Details about the OpenApiLibCore library parameters and keywords that you may need can be found
-[here](https://marketsquare.github.io/robotframework-openapi-libcore/openapi_libcore.html).
-
-The OpenApiLibCore also support handling of relations between resources within the scope
-of the API being validated as well as handling dependencies on resources outside the
-scope of the API. In addition there is support for handling restrictions on the values
-of parameters and properties.
-
-Details about the `mappings_path` variable usage can be found
-[here](https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html).
-
----
-
-## Limitations
-
-There are currently a number of limitations to supported API structures, supported
-data types and properties. The following list details the most important ones:
-- Only JSON request and response bodies are supported.
-- No support for per-endpoint authorization levels.
-- Parsing of OAS 3.1 documents is supported by the parsing tools, but runtime behavior is untested.
-
-"""
-
-import json as _json
-import re
-import sys
-from copy import deepcopy
-from dataclasses import Field, dataclass, field, make_dataclass
-from functools import cached_property
-from itertools import zip_longest
-from logging import getLogger
-from pathlib import Path
-from random import choice
-from typing import Any, Dict, List, Optional, Set, Tuple, Type, Union
-from uuid import uuid4
-
-from openapi_core import Spec, validate_response
-from openapi_core.contrib.requests import (
-    RequestsOpenAPIRequest,
-    RequestsOpenAPIResponse,
-)
-from prance import ResolvingParser, ValidationError
-from prance.util.url import ResolutionError
-from requests import Response, Session
-from requests.auth import AuthBase, HTTPBasicAuth
-from requests.cookies import RequestsCookieJar as CookieJar
-from robot.api.deco import keyword, library
-from robot.libraries.BuiltIn import BuiltIn
-
-from OpenApiLibCore import value_utils
-from OpenApiLibCore.dto_base import (
-    NOT_SET,
-    Dto,
-    IdDependency,
-    IdReference,
-    PathPropertiesConstraint,
-    PropertyValueConstraint,
-    Relation,
-    UniquePropertyValueConstraint,
-    resolve_schema,
-)
-from OpenApiLibCore.dto_utils import (
-    DEFAULT_ID_PROPERTY_NAME,
-    DefaultDto,
-    get_dto_class,
-    get_id_property_name,
-)
-from OpenApiLibCore.oas_cache import PARSER_CACHE
-from OpenApiLibCore.value_utils import FAKE, IGNORE, JSON
-
-run_keyword = BuiltIn().run_keyword
-
-logger = getLogger(__name__)
-
-
-def get_safe_key(key: str) -> str:
-    """
-    Helper function to convert a valid JSON property name to a string that can be used
-    as a Python variable or function / method name.
-    """
-    key = key.replace("-", "_")
-    key = key.replace("@", "_")
-    if key[0].isdigit():
-        key = f"_{key}"
-    return key
-
-
-@dataclass
-class RequestValues:
-    """Helper class to hold parameter values needed to make a request."""
-
-    url: str
-    method: str
-    params: Optional[Dict[str, Any]]
-    headers: Optional[Dict[str, str]]
-    json_data: Optional[Dict[str, Any]]
-
-
-@dataclass
-class RequestData:
-    """Helper class to manage parameters used when making requests."""
-
-    dto: Union[Dto, DefaultDto] = field(default_factory=DefaultDto)
-    dto_schema: Dict[str, Any] = field(default_factory=dict)
-    parameters: List[Dict[str, Any]] = field(default_factory=list)
-    params: Dict[str, Any] = field(default_factory=dict)
-    headers: Dict[str, Any] = field(default_factory=dict)
-    has_body: bool = True
-
-    def __post_init__(self) -> None:
-        # prevent modification by reference
-        self.dto_schema = deepcopy(self.dto_schema)
-        self.parameters = deepcopy(self.parameters)
-        self.params = deepcopy(self.params)
-        self.headers = deepcopy(self.headers)
-
-    @property
-    def has_optional_properties(self) -> bool:
-        """Whether or not the dto data (json data) contains optional properties."""
-
-        def is_required_property(property_name: str) -> bool:
-            return property_name in self.dto_schema.get("required", [])
-
-        properties = (self.dto.as_dict()).keys()
-        return not all(map(is_required_property, properties))
-
-    @property
-    def has_optional_params(self) -> bool:
-        """Whether or not any of the query parameters are optional."""
-
-        def is_optional_param(query_param: str) -> bool:
-            optional_params = [
-                p.get("name")
-                for p in self.parameters
-                if p.get("in") == "query" and not p.get("required")
-            ]
-            return query_param in optional_params
-
-        return any(map(is_optional_param, self.params))
-
-    @cached_property
-    def params_that_can_be_invalidated(self) -> Set[str]:
-        """
-        The query parameters that can be invalidated by violating data
-        restrictions, data type or by not providing them in a request.
-        """
-        result = set()
-        params = [h for h in self.parameters if h.get("in") == "query"]
-        for param in params:
-            # required params can be omitted to invalidate a request
-            if param["required"]:
-                result.add(param["name"])
-                continue
-
-            schema = resolve_schema(param["schema"])
-            if schema.get("type", None):
-                param_types = [schema]
-            else:
-                param_types = schema["types"]
-            for param_type in param_types:
-                # any basic non-string type except "null" can be invalidated by
-                # replacing it with a string
-                if param_type["type"] not in ["string", "array", "object", "null"]:
-                    result.add(param["name"])
-                    continue
-                # enums, strings and arrays with boundaries can be invalidated
-                if set(param_type.keys()).intersection(
-                    {
-                        "enum",
-                        "minLength",
-                        "maxLength",
-                        "minItems",
-                        "maxItems",
-                    }
-                ):
-                    result.add(param["name"])
-                    continue
-                # an array of basic non-string type can be invalidated by replacing the
-                # items in the array with strings
-                if param_type["type"] == "array" and param_type["items"][
-                    "type"
-                ] not in [
-                    "string",
-                    "array",
-                    "object",
-                    "null",
-                ]:
-                    result.add(param["name"])
-        return result
-
-    @property
-    def has_optional_headers(self) -> bool:
-        """Whether or not any of the headers are optional."""
-
-        def is_optional_header(header: str) -> bool:
-            optional_headers = [
-                p.get("name")
-                for p in self.parameters
-                if p.get("in") == "header" and not p.get("required")
-            ]
-            return header in optional_headers
-
-        return any(map(is_optional_header, self.headers))
-
-    @cached_property
-    def headers_that_can_be_invalidated(self) -> Set[str]:
-        """
-        The header parameters that can be invalidated by violating data
-        restrictions or by not providing them in a request.
-        """
-        result = set()
-        headers = [h for h in self.parameters if h.get("in") == "header"]
-        for header in headers:
-            # required headers can be omitted to invalidate a request
-            if header["required"]:
-                result.add(header["name"])
-                continue
-
-            schema = resolve_schema(header["schema"])
-            if schema.get("type", None):
-                header_types = [schema]
-            else:
-                header_types = schema["types"]
-            for header_type in header_types:
-                # any basic non-string type except "null" can be invalidated by
-                # replacing it with a string
-                if header_type["type"] not in ["string", "array", "object", "null"]:
-                    result.add(header["name"])
-                    continue
-                # enums, strings and arrays with boundaries can be invalidated
-                if set(header_type.keys()).intersection(
-                    {
-                        "enum",
-                        "minLength",
-                        "maxLength",
-                        "minItems",
-                        "maxItems",
-                    }
-                ):
-                    result.add(header["name"])
-                    continue
-                # an array of basic non-string type can be invalidated by replacing the
-                # items in the array with strings
-                if header_type["type"] == "array" and header_type["items"][
-                    "type"
-                ] not in [
-                    "string",
-                    "array",
-                    "object",
-                    "null",
-                ]:
-                    result.add(header["name"])
-        return result
-
-    def get_required_properties_dict(self) -> Dict[str, Any]:
-        """Get the json-compatible dto data containing only the required properties."""
-        required_properties = self.dto_schema.get("required", [])
-        required_properties_dict: Dict[str, Any] = {}
-        for key, value in (self.dto.as_dict()).items():
-            if key in required_properties:
-                required_properties_dict[key] = value
-        return required_properties_dict
-
-    def get_required_params(self) -> Dict[str, str]:
-        """Get the params dict containing only the required query parameters."""
-        required_parameters = [
-            p.get("name") for p in self.parameters if p.get("required")
-        ]
-        return {k: v for k, v in self.params.items() if k in required_parameters}
-
-    def get_required_headers(self) -> Dict[str, str]:
-        """Get the headers dict containing only the required headers."""
-        required_parameters = [
-            p.get("name") for p in self.parameters if p.get("required")
-        ]
-        return {k: v for k, v in self.headers.items() if k in required_parameters}
-
-
-@library(scope="TEST SUITE", doc_format="ROBOT")
-class OpenApiLibCore:  # pylint: disable=too-many-instance-attributes
-    """
-    Main class providing the keywords and core logic to interact with an OpenAPI server.
-
-    Visit the [https://github.com/MarketSquare/robotframework-openapi-libcore | library page]
-    for an introduction.
-    """
-
-    def __init__(  # pylint: disable=too-many-arguments, too-many-locals, dangerous-default-value
-        self,
-        source: str,
-        origin: str = "",
-        base_path: str = "",
-        mappings_path: Union[str, Path] = "",
-        invalid_property_default_response: int = 422,
-        default_id_property_name: str = "id",
-        faker_locale: Optional[Union[str, List[str]]] = None,
-        recursion_limit: int = 1,
-        recursion_default: Any = {},
-        username: str = "",
-        password: str = "",
-        security_token: str = "",
-        auth: Optional[AuthBase] = None,
-        cert: Optional[Union[str, Tuple[str, str]]] = None,
-        verify_tls: Optional[Union[bool, str]] = True,
-        extra_headers: Optional[Dict[str, str]] = None,
-        cookies: Optional[Union[Dict[str, str], CookieJar]] = None,
-        proxies: Optional[Dict[str, str]] = None,
-    ) -> None:
-        """
-        == Base parameters ==
-
-        === source ===
-        An absolute path to an openapi.json or openapi.yaml file or an url to such a file.
-
-        === origin ===
-        The server (and port) of the target server. E.g. ``https://localhost:8000``
-
-        === base_path ===
-        The routing between ``origin`` and the endpoints as found in the ``paths``
-        section in the openapi document.
-        E.g. ``/petshop/v2``.
-
-        == API-specific configurations ==
-
-        === mappings_path ===
-        See [https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html | this page]
-        for an in-depth explanation.
-
-        === invalid_property_default_response ===
-        The default response code for requests with a JSON body that does not comply
-        with the schema.
-        Example: a value outside the specified range or a string value
-        for a property defined as integer in the schema.
-
-        === default_id_property_name ===
-        The default name for the property that identifies a resource (i.e. a unique
-        entity) within the API.
-        The default value for this property name is ``id``.
-        If the target API uses a different name for all the resources within the API,
-        you can configure it globally using this property.
-
-        If different property names are used for the unique identifier for different
-        types of resources, an ``ID_MAPPING`` can be implemented using the ``mappings_path``.
-
-        === faker_locale ===
-        A locale string or list of locale strings to pass to the Faker library to be
-        used in generation of string data for supported format types.
-
-        == Parsing parameters ==
-
-        === recursion_limit ===
-        The recursion depth to which to fully parse recursive references before the
-        `recursion_default` is used to end the recursion.
-
-        === recursion_default ===
-        The value that is used instead of the referenced schema when the
-        `recursion_limit` has been reached.
-        The default `{}` represents an empty object in JSON.
-        Depending on schema definitions, this may cause schema validation errors.
-        If this is the case, 'None' (``${NONE}`` in Robot Framework) or an empty list
-        can be tried as an alternative.
-
-        == Security-related parameters ==
-        _Note: these parameters are equivalent to those in the ``requests`` library._
-
-        === username ===
-        The username to be used for Basic Authentication.
-
-        === password ===
-        The password to be used for Basic Authentication.
-
-        === security_token ===
-        The token to be used for token based security using the ``Authorization`` header.
-
-        === auth ===
-        A [https://requests.readthedocs.io/en/latest/api/#authentication | requests ``AuthBase`` instance]
-        to be used for authentication instead of the ``username`` and ``password``.
-
-        === cert ===
-        The SSL certificate to use with all requests.
-        If string: the path to ssl client cert file (.pem).
-        If tuple: the ('cert', 'key') pair.
-
-        === verify_tls ===
-        Whether or not to verify the TLS / SSL certificate of the server.
-        If boolean: whether or not to verify the server TLS certificate.
-        If string: path to a CA bundle to use for verification.
-
-        === extra_headers ===
-        A dictionary with extra / custom headers that will be send with every request.
-        This parameter can be used to send headers that are not documented in the
-        openapi document or to provide an API-key.
-
-        === cookies ===
-        A dictionary or
-        [https://docs.python.org/3/library/http.cookiejar.html#http.cookiejar.CookieJar | CookieJar object]
-        to send with all requests.
-
-        === proxies ===
-        A dictionary of 'protocol': 'proxy url' to use for all requests.
-        """
-        self._source = source
-        self._origin = origin
-        self._base_path = base_path
-        self._recursion_limit = recursion_limit
-        self._recursion_default = recursion_default
-        self.session = Session()
-        # only username and password, security_token or auth object should be provided
-        # if multiple are provided, username and password take precedence
-        self.security_token = security_token
-        self.auth = auth
-        if username and password:
-            self.auth = HTTPBasicAuth(username, password)
-        # Robot Framework does not allow users to create tuples and requests
-        # does not accept lists, so perform the conversion here
-        if isinstance(cert, list):
-            cert = tuple(cert)
-        self.cert = cert
-        self.verify = verify_tls
-        self.extra_headers = extra_headers
-        self.cookies = cookies
-        self.proxies = proxies
-        self.invalid_property_default_response = invalid_property_default_response
-        if mappings_path and str(mappings_path) != ".":
-            mappings_path = Path(mappings_path)
-            if not mappings_path.is_file():
-                logger.warning(
-                    f"mappings_path '{mappings_path}' is not a Python module."
-                )
-            # intermediate variable to ensure path.append is possible so we'll never
-            # path.pop a location that we didn't append
-            mappings_folder = str(mappings_path.parent)
-            sys.path.append(mappings_folder)
-            mappings_module_name = mappings_path.stem
-            self.get_dto_class = get_dto_class(
-                mappings_module_name=mappings_module_name
-            )
-            self.get_id_property_name = get_id_property_name(
-                mappings_module_name=mappings_module_name
-            )
-            sys.path.pop()
-        else:
-            self.get_dto_class = get_dto_class(mappings_module_name="no mapping")
-            self.get_id_property_name = get_id_property_name(
-                mappings_module_name="no mapping"
-            )
-        if faker_locale:
-            FAKE.set_locale(locale=faker_locale)
-        # update the globally available DEFAULT_ID_PROPERTY_NAME to the provided value
-        DEFAULT_ID_PROPERTY_NAME.id_property_name = default_id_property_name
-
-    @property
-    def origin(self) -> str:
-        return self._origin
-
-    @keyword
-    def set_origin(self, origin: str) -> None:
-        """
-        Update the `origin` after the library is imported.
-
-        This can be done during the `Suite setup` when using DataDriver in situations
-        where the OpenAPI document is available on disk but the target host address is
-        not known before the test starts.
-
-        In combination with OpenApiLibCore, the `origin` can be used at any point to
-        target another server that hosts an API that complies to the same OAS.
-        """
-        self._origin = origin
-
-    @property
-    def base_url(self) -> str:
-        return f"{self.origin}{self._base_path}"
-
-    @cached_property
-    def validation_spec(self) -> Spec:
-        return Spec.from_dict(self.openapi_spec)
-
-    @property
-    def openapi_spec(self) -> Dict[str, Any]:
-        """Return a deepcopy of the parsed openapi document."""
-        # protect the parsed openapi spec from being mutated by reference
-        return deepcopy(self._openapi_spec)
-
-    @cached_property
-    def _openapi_spec(self) -> Dict[str, Any]:
-        parser = self._load_parser()
-        return parser.specification
-
-    def read_paths(self) -> Dict[str, Any]:
-        return self.openapi_spec["paths"]
-
-    def _load_parser(self) -> ResolvingParser:
-        try:
-
-            def recursion_limit_handler(
-                limit: int, refstring: str, recursions: Any
-            ) -> Any:
-                return self._recursion_default
-
-            # Since parsing of the OAS and creating the Spec can take a long time,
-            # they are cached. This is done by storing them in an imported module that
-            # will have a global scope due to how the Python import system works. This
-            # ensures that in a Suite of Suites where multiple Suites use the same
-            # `source`, that OAS is only parsed / loaded once.
-            parser = PARSER_CACHE.get(self._source, None)
-            if parser is None:
-                parser = ResolvingParser(
-                    self._source,
-                    backend="openapi-spec-validator",
-                    recursion_limit=self._recursion_limit,
-                    recursion_limit_handler=recursion_limit_handler,
-                )
-
-                if parser.specification is None:  # pragma: no cover
-                    BuiltIn().fatal_error(
-                        "Source was loaded, but no specification was present after parsing."
-                    )
-
-                PARSER_CACHE[self._source] = parser
-
-            return parser
-
-        except ResolutionError as exception:
-            BuiltIn().fatal_error(
-                f"ResolutionError while trying to load openapi spec: {exception}"
-            )
-        except ValidationError as exception:
-            BuiltIn().fatal_error(
-                f"ValidationError while trying to load openapi spec: {exception}"
-            )
-
-    def validate_response_vs_spec(
-        self, request: RequestsOpenAPIRequest, response: RequestsOpenAPIResponse
-    ) -> None:
-        """
-        Validate the reponse for a given request against the OpenAPI Spec that is
-        loaded during library initialization.
-        """
-        _ = validate_response(
-            spec=self.validation_spec,
-            request=request,
-            response=response,
-        )
-
-    @keyword
-    def get_valid_url(self, endpoint: str, method: str) -> str:
-        """
-        This keyword returns a valid url for the given `endpoint` and `method`.
-
-        If the `endpoint` contains path parameters the Get Valid Id For Endpoint
-        keyword will be executed to retrieve valid ids for the path parameters.
-
-        > Note: if valid ids cannot be retrieved within the scope of the API, the
-        `PathPropertiesConstraint` Relation can be used. More information can be found
-        [https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html | here].
-        """
-        method = method.lower()
-        try:
-            # endpoint can be partially resolved or provided by a PathPropertiesConstraint
-            parametrized_endpoint = self.get_parametrized_endpoint(endpoint=endpoint)
-            _ = self.openapi_spec["paths"][parametrized_endpoint]
-        except KeyError:
-            raise ValueError(
-                f"{endpoint} not found in paths section of the OpenAPI document."
-            ) from None
-        dto_class = self.get_dto_class(endpoint=endpoint, method=method)
-        relations = dto_class.get_relations()
-        paths = [p.path for p in relations if isinstance(p, PathPropertiesConstraint)]
-        if paths:
-            url = f"{self.base_url}{choice(paths)}"
-            return url
-        endpoint_parts = list(endpoint.split("/"))
-        for index, part in enumerate(endpoint_parts):
-            if part.startswith("{") and part.endswith("}"):
-                type_endpoint_parts = endpoint_parts[slice(index)]
-                type_endpoint = "/".join(type_endpoint_parts)
-                existing_id: Union[str, int, float] = run_keyword(
-                    "get_valid_id_for_endpoint", type_endpoint, method
-                )
-                endpoint_parts[index] = str(existing_id)
-        resolved_endpoint = "/".join(endpoint_parts)
-        url = f"{self.base_url}{resolved_endpoint}"
-        return url
-
-    @keyword
-    def get_valid_id_for_endpoint(
-        self, endpoint: str, method: str
-    ) -> Union[str, int, float]:
-        """
-        Support keyword that returns the `id` for an existing resource at `endpoint`.
-
-        To prevent resource conflicts with other test cases, a new resource is created
-        (POST) if possible.
-        """
-
-        def dummy_transformer(
-            valid_id: Union[str, int, float]
-        ) -> Union[str, int, float]:
-            return valid_id
-
-        method = method.lower()
-        url: str = run_keyword("get_valid_url", endpoint, method)
-        # Try to create a new resource to prevent conflicts caused by
-        # operations performed on the same resource by other test cases
-        request_data = self.get_request_data(endpoint=endpoint, method="post")
-
-        response: Response = run_keyword(
-            "authorized_request",
-            url,
-            "post",
-            request_data.get_required_params(),
-            request_data.get_required_headers(),
-            request_data.get_required_properties_dict(),
-        )
-
-        # determine the id property name for this path and whether or not a transformer is used
-        mapping = self.get_id_property_name(endpoint=endpoint)
-        if isinstance(mapping, str):
-            id_property = mapping
-            # set the transformer to a dummy callable that returns the original value so
-            # the transformer can be applied on any returned id
-            id_transformer = dummy_transformer
-        else:
-            id_property, id_transformer = mapping
-
-        if not response.ok:
-            # If a new resource cannot be created using POST, try to retrieve a
-            # valid id using a GET request.
-            try:
-                valid_id = choice(run_keyword("get_ids_from_url", url))
-                return id_transformer(valid_id)
-            except Exception as exception:
-                raise AssertionError(
-                    f"Failed to get a valid id using GET on {url}"
-                ) from exception
-
-        response_data = response.json()
-        if prepared_body := response.request.body:
-            if isinstance(prepared_body, bytes):
-                send_json = _json.loads(prepared_body.decode("UTF-8"))
-            else:
-                send_json = _json.loads(prepared_body)
-        else:
-            send_json = None
-
-        # no support for retrieving an id from an array returned on a POST request
-        if isinstance(response_data, list):
-            raise NotImplementedError(
-                f"Unexpected response body for POST request: expected an object but "
-                f"received an array ({response_data})"
-            )
-
-        # POST on /resource_type/{id}/array_item/ will return the updated {id} resource
-        # instead of a newly created resource. In this case, the send_json must be
-        # in the array of the 'array_item' property on {id}
-        send_path: str = response.request.path_url
-        response_href: Optional[str] = response_data.get("href", None)
-        if response_href and (send_path not in response_href) and send_json:
-            try:
-                property_to_check = send_path.replace(response_href, "")[1:]
-                item_list: List[Dict[str, Any]] = response_data[property_to_check]
-                # Use the (mandatory) id to get the POSTed resource from the list
-                [valid_id] = [
-                    item[id_property]
-                    for item in item_list
-                    if item[id_property] == send_json[id_property]
-                ]
-            except Exception as exception:
-                raise AssertionError(
-                    f"Failed to get a valid id from {response_href}"
-                ) from exception
-        else:
-            try:
-                valid_id = response_data[id_property]
-            except KeyError:
-                raise AssertionError(
-                    f"Failed to get a valid id from {response_data}"
-                ) from None
-        return id_transformer(valid_id)
-
-    @keyword
-    def get_ids_from_url(self, url: str) -> List[str]:
-        """
-        Perform a GET request on the `url` and return the list of resource
-        `ids` from the response.
-        """
-        endpoint = self.get_parameterized_endpoint_from_url(url)
-        request_data = self.get_request_data(endpoint=endpoint, method="get")
-        response = run_keyword(
-            "authorized_request",
-            url,
-            "get",
-            request_data.get_required_params(),
-            request_data.get_required_headers(),
-        )
-        response.raise_for_status()
-        response_data: Union[Dict[str, Any], List[Dict[str, Any]]] = response.json()
-
-        # determine the property name to use
-        mapping = self.get_id_property_name(endpoint=endpoint)
-        if isinstance(mapping, str):
-            id_property = mapping
-        else:
-            id_property, _ = mapping
-
-        if isinstance(response_data, list):
-            valid_ids: List[str] = [item[id_property] for item in response_data]
-            return valid_ids
-        # if the response is an object (dict), check if it's hal+json
-        if embedded := response_data.get("_embedded"):
-            # there should be 1 item in the dict that has a value that's a list
-            for value in embedded.values():
-                if isinstance(value, list):
-                    valid_ids = [item[id_property] for item in value]
-                    return valid_ids
-        if (valid_id := response_data.get(id_property)) is not None:
-            return [valid_id]
-        valid_ids = [item[id_property] for item in response_data["items"]]
-        return valid_ids
-
-    @keyword
-    def get_request_data(self, endpoint: str, method: str) -> RequestData:
-        """Return an object with valid request data for body, headers and query params."""
-        method = method.lower()
-        dto_cls_name = self._get_dto_cls_name(endpoint=endpoint, method=method)
-        # The endpoint can contain already resolved Ids that have to be matched
-        # against the parametrized endpoints in the paths section.
-        spec_endpoint = self.get_parametrized_endpoint(endpoint)
-        dto_class = self.get_dto_class(endpoint=spec_endpoint, method=method)
-        try:
-            method_spec = self.openapi_spec["paths"][spec_endpoint][method]
-        except KeyError:
-            logger.info(
-                f"method '{method}' not supported on '{spec_endpoint}, using empty spec."
-            )
-            method_spec = {}
-
-        parameters, params, headers = self.get_request_parameters(
-            dto_class=dto_class, method_spec=method_spec
-        )
-        if (body_spec := method_spec.get("requestBody", None)) is None:
-            if dto_class == DefaultDto:
-                dto_instance: Dto = DefaultDto()
-            else:
-                dto_class = make_dataclass(
-                    cls_name=method_spec.get("operationId", dto_cls_name),
-                    fields=[],
-                    bases=(dto_class,),
-                )
-                dto_instance = dto_class()
-            return RequestData(
-                dto=dto_instance,
-                parameters=parameters,
-                params=params,
-                headers=headers,
-                has_body=False,
-            )
-        content_schema = resolve_schema(self.get_content_schema(body_spec))
-        headers.update({"content-type": self.get_content_type(body_spec)})
-        dto_data = self.get_json_data_for_dto_class(
-            schema=content_schema,
-            dto_class=dto_class,
-            operation_id=method_spec.get("operationId", ""),
-        )
-        if dto_data is None:
-            dto_instance = DefaultDto()
-        else:
-            fields = self.get_fields_from_dto_data(content_schema, dto_data)
-            dto_class = make_dataclass(
-                cls_name=method_spec.get("operationId", dto_cls_name),
-                fields=fields,
-                bases=(dto_class,),
-            )
-            dto_data = {get_safe_key(key): value for key, value in dto_data.items()}
-            dto_instance = dto_class(**dto_data)
-        return RequestData(
-            dto=dto_instance,
-            dto_schema=content_schema,
-            parameters=parameters,
-            params=params,
-            headers=headers,
-        )
-
-    @staticmethod
-    def _get_dto_cls_name(endpoint: str, method: str) -> str:
-        method = method.capitalize()
-        path = endpoint.translate({ord(i): None for i in "{}"})
-        path_parts = path.split("/")
-        path_parts = [p.capitalize() for p in path_parts]
-        result = "".join([method, *path_parts])
-        return result
-
-    @staticmethod
-    def get_fields_from_dto_data(
-        content_schema: Dict[str, Any], dto_data: Dict[str, Any]
-    ):
-        # FIXME: annotation is not Pyhon 3.8-compatible
-        # ) -> List[Union[str, Tuple[str, Type[Any]], Tuple[str, Type[Any], Field[Any]]]]:
-        """Get a dataclasses fields list based on the content_schema and dto_data."""
-        fields: List[
-            Union[str, Tuple[str, Type[Any]], Tuple[str, Type[Any], Field[Any]]]
-        ] = []
-        for key, value in dto_data.items():
-            required_properties = content_schema.get("required", [])
-            safe_key = get_safe_key(key)
-            metadata = {"original_property_name": key}
-            if key in required_properties:
-                # The fields list is used to create a dataclass, so non-default fields
-                # must go before fields with a default
-                fields.insert(0, (safe_key, type(value), field(metadata=metadata)))
-            else:
-                fields.append((safe_key, type(value), field(default=None, metadata=metadata)))  # type: ignore[arg-type]
-        return fields
-
-    def get_request_parameters(
-        self, dto_class: Union[Dto, Type[Dto]], method_spec: Dict[str, Any]
-    ) -> Tuple[List[Dict[str, Any]], Dict[str, Any], Dict[str, str]]:
-        """Get the methods parameter spec and params and headers with valid data."""
-        parameters = method_spec.get("parameters", [])
-        parameter_relations = dto_class.get_parameter_relations()
-        query_params = [p for p in parameters if p.get("in") == "query"]
-        header_params = [p for p in parameters if p.get("in") == "header"]
-        params = self.get_parameter_data(query_params, parameter_relations)
-        headers = self.get_parameter_data(header_params, parameter_relations)
-        return parameters, params, headers
-
-    @classmethod
-    def get_content_schema(cls, body_spec: Dict[str, Any]) -> Dict[str, Any]:
-        """Get the content schema from the requestBody spec."""
-        content_type = cls.get_content_type(body_spec)
-        content_schema = body_spec["content"][content_type]["schema"]
-        return resolve_schema(content_schema)
-
-    @staticmethod
-    def get_content_type(body_spec: Dict[str, Any]) -> str:
-        """Get and validate the first supported content type from the requested body spec
-
-        Should be application/json like content type,
-        e.g "application/json;charset=utf-8" or "application/merge-patch+json"
-        """
-        content_types: List[str] = body_spec["content"].keys()
-        json_regex = r"application/([a-z\-]+\+)?json(;\s?charset=(.+))?"
-        for content_type in content_types:
-            if re.search(json_regex, content_type):
-                return content_type
-
-        # At present no supported for other types.
-        raise NotImplementedError(
-            f"Only content types like 'application/json' are supported. "
-            f"Content types definded in the spec are '{content_types}'."
-        )
-
-    def get_parametrized_endpoint(self, endpoint: str) -> str:
-        """
-        Get the parametrized endpoint as found in the `paths` section of the openapi
-        document from a (partially) resolved endpoint.
-        """
-
-        def match_parts(parts: List[str], spec_parts: List[str]) -> bool:
-            for part, spec_part in zip_longest(parts, spec_parts, fillvalue="Filler"):
-                if part == "Filler" or spec_part == "Filler":
-                    return False
-                if part != spec_part and not spec_part.startswith("{"):
-                    return False
-            return True
-
-        endpoint_parts = endpoint.split("/")
-        # if the last part is empty, the path has a trailing `/` that
-        # should be ignored during matching
-        if endpoint_parts[-1] == "":
-            _ = endpoint_parts.pop(-1)
-
-        spec_endpoints: List[str] = {**self.openapi_spec}["paths"].keys()
-
-        candidates: List[str] = []
-
-        for spec_endpoint in spec_endpoints:
-            spec_endpoint_parts = spec_endpoint.split("/")
-            # ignore trailing `/` the same way as for endpoint_parts
-            if spec_endpoint_parts[-1] == "":
-                _ = spec_endpoint_parts.pop(-1)
-            if match_parts(endpoint_parts, spec_endpoint_parts):
-                candidates.append(spec_endpoint)
-
-        if not candidates:
-            raise ValueError(
-                f"{endpoint} not found in paths section of the OpenAPI document."
-            )
-
-        if len(candidates) == 1:
-            return candidates[0]
-        # Multiple matches can happen in APIs with overloaded endpoints, e.g.
-        # /users/me
-        # /users/${user_id}
-        # In this case, find the closest (or exact) match
-        exact_match = [c for c in candidates if c == endpoint]
-        if exact_match:
-            return exact_match[0]
-        # TODO: Implement a decision mechanism when real-world examples become available
-        # In the face of ambiguity, refuse the temptation to guess.
-        raise ValueError(f"{endpoint} matched to multiple paths: {candidates}")
-
-    @staticmethod
-    def get_parameter_data(
-        parameters: List[Dict[str, Any]],
-        parameter_relations: List[Relation],
-    ) -> Dict[str, str]:
-        """Generate a valid list of key-value pairs for all parameters."""
-        result: Dict[str, str] = {}
-        value: Any = None
-        for parameter in parameters:
-            parameter_name = parameter["name"]
-            parameter_schema = resolve_schema(parameter["schema"])
-            relations = [
-                r for r in parameter_relations if r.property_name == parameter_name
-            ]
-            if constrained_values := [
-                r.values for r in relations if isinstance(r, PropertyValueConstraint)
-            ]:
-                value = choice(*constrained_values)
-                if value is IGNORE:
-                    continue
-                result[parameter_name] = value
-                continue
-            value = value_utils.get_valid_value(parameter_schema)
-            result[parameter_name] = value
-        return result
-
-    @keyword
-    def get_json_data_for_dto_class(
-        self,
-        schema: Dict[str, Any],
-        dto_class: Union[Dto, Type[Dto]],
-        operation_id: str = "",
-    ) -> Optional[Dict[str, Any]]:
-        """
-        Generate a valid (json-compatible) dict for all the `dto_class` properties.
-        """
-
-        def get_constrained_values(property_name: str) -> List[Any]:
-            relations = dto_class.get_relations()
-            values_list = [
-                c.values
-                for c in relations
-                if (
-                    isinstance(c, PropertyValueConstraint)
-                    and c.property_name == property_name
-                )
-            ]
-            # values should be empty or contain 1 list of allowed values
-            return values_list.pop() if values_list else []
-
-        def get_dependent_id(
-            property_name: str, operation_id: str
-        ) -> Optional[Union[str, int, float]]:
-            relations = dto_class.get_relations()
-            # multiple get paths are possible based on the operation being performed
-            id_get_paths = [
-                (d.get_path, d.operation_id)
-                for d in relations
-                if (isinstance(d, IdDependency) and d.property_name == property_name)
-            ]
-            if not id_get_paths:
-                return None
-            if len(id_get_paths) == 1:
-                id_get_path, _ = id_get_paths.pop()
-            else:
-                try:
-                    [id_get_path] = [
-                        path
-                        for path, operation in id_get_paths
-                        if operation == operation_id
-                    ]
-                # There could be multiple get_paths, but not one for the current operation
-                except ValueError:
-                    return None
-            valid_id = self.get_valid_id_for_endpoint(
-                endpoint=id_get_path, method="get"
-            )
-            logger.debug(f"get_dependent_id for {id_get_path} returned {valid_id}")
-            return valid_id
-
-        json_data: Dict[str, Any] = {}
-
-        for property_name in schema.get("properties", []):
-            properties_schema = schema["properties"][property_name]
-
-            property_type = properties_schema.get("type")
-            if not property_type:
-                selected_type_schema = choice(properties_schema["types"])
-                property_type = selected_type_schema["type"]
-            if properties_schema.get("readOnly", False):
-                continue
-            if constrained_values := get_constrained_values(property_name):
-                # do not add properties that are configured to be ignored
-                if IGNORE in constrained_values:
-                    continue
-                json_data[property_name] = choice(constrained_values)
-                continue
-            if (
-                dependent_id := get_dependent_id(
-                    property_name=property_name, operation_id=operation_id
-                )
-            ) is not None:
-                json_data[property_name] = dependent_id
-                continue
-            if property_type == "object":
-                object_data = self.get_json_data_for_dto_class(
-                    schema=properties_schema,
-                    dto_class=DefaultDto,
-                    operation_id="",
-                )
-                json_data[property_name] = object_data
-                continue
-            if property_type == "array":
-                array_data = self.get_json_data_for_dto_class(
-                    schema=properties_schema["items"],
-                    dto_class=DefaultDto,
-                    operation_id=operation_id,
-                )
-                json_data[property_name] = [array_data]
-                continue
-            json_data[property_name] = value_utils.get_valid_value(properties_schema)
-        return json_data
-
-    @keyword
-    def get_invalidated_url(self, valid_url: str) -> Optional[str]:
-        """
-        Return an url with all the path parameters in the `valid_url` replaced by a
-        random UUID.
-
-        Raises ValueError if the valid_url cannot be invalidated.
-        """
-        parameterized_endpoint = self.get_parameterized_endpoint_from_url(valid_url)
-        parameterized_url = self.base_url + parameterized_endpoint
-        valid_url_parts = list(reversed(valid_url.split("/")))
-        parameterized_parts = reversed(parameterized_url.split("/"))
-        for index, (parameterized_part, _) in enumerate(
-            zip(parameterized_parts, valid_url_parts)
-        ):
-            if parameterized_part.startswith("{") and parameterized_part.endswith("}"):
-                valid_url_parts[index] = uuid4().hex
-                valid_url_parts.reverse()
-                invalid_url = "/".join(valid_url_parts)
-                return invalid_url
-        raise ValueError(f"{parameterized_endpoint} could not be invalidated.")
-
-    @keyword
-    def get_parameterized_endpoint_from_url(self, url: str) -> str:
-        """
-        Return the endpoint as found in the `paths` section based on the given `url`.
-        """
-        endpoint = url.replace(self.base_url, "")
-        endpoint_parts = endpoint.split("/")
-        # first part will be '' since an endpoint starts with /
-        endpoint_parts.pop(0)
-        parameterized_endpoint = self.get_parametrized_endpoint(endpoint=endpoint)
-        return parameterized_endpoint
-
-    @keyword
-    def get_invalid_json_data(
-        self,
-        url: str,
-        method: str,
-        status_code: int,
-        request_data: RequestData,
-    ) -> Dict[str, Any]:
-        """
-        Return `json_data` based on the `dto` on the `request_data` that will cause
-        the provided `status_code` for the `method` operation on the `url`.
-
-        > Note: applicable UniquePropertyValueConstraint and IdReference Relations are
-            considered before changes to `json_data` are made.
-        """
-        method = method.lower()
-        data_relations = request_data.dto.get_relations_for_error_code(status_code)
-        if not data_relations:
-            if not request_data.dto_schema:
-                raise ValueError(
-                    "Failed to invalidate: no data_relations and empty schema."
-                )
-            json_data = request_data.dto.get_invalidated_data(
-                schema=request_data.dto_schema,
-                status_code=status_code,
-                invalid_property_default_code=self.invalid_property_default_response,
-            )
-            return json_data
-        resource_relation = choice(data_relations)
-        if isinstance(resource_relation, UniquePropertyValueConstraint):
-            json_data = run_keyword(
-                "get_json_data_with_conflict",
-                url,
-                method,
-                request_data.dto,
-                status_code,
-            )
-        elif isinstance(resource_relation, IdReference):
-            run_keyword("ensure_in_use", url, resource_relation)
-            json_data = request_data.dto.as_dict()
-        else:
-            json_data = request_data.dto.get_invalidated_data(
-                schema=request_data.dto_schema,
-                status_code=status_code,
-                invalid_property_default_code=self.invalid_property_default_response,
-            )
-        return json_data
-
-    @keyword
-    def get_invalidated_parameters(
-        self,
-        status_code: int,
-        request_data: RequestData,
-    ) -> Tuple[Dict[str, Any], Dict[str, str]]:
-        """
-        Returns a version of `params, headers` as present on `request_data` that has
-        been modified to cause the provided `status_code`.
-        """
-        if not request_data.parameters:
-            raise ValueError("No params or headers to invalidate.")
-
-        # ensure the status_code can be triggered
-        relations = request_data.dto.get_parameter_relations_for_error_code(status_code)
-        relations_for_status_code = [
-            r
-            for r in relations
-            if isinstance(r, PropertyValueConstraint)
-            and (
-                r.error_code == status_code or r.invalid_value_error_code == status_code
-            )
-        ]
-        parameters_to_ignore = {
-            r.property_name
-            for r in relations_for_status_code
-            if r.invalid_value_error_code == status_code and r.invalid_value == IGNORE
-        }
-        relation_property_names = {r.property_name for r in relations_for_status_code}
-        if not relation_property_names:
-            if status_code != self.invalid_property_default_response:
-                raise ValueError(
-                    f"No relations to cause status_code {status_code} found."
-                )
-
-        # ensure we're not modifying mutable properties
-        params = deepcopy(request_data.params)
-        headers = deepcopy(request_data.headers)
-
-        if status_code == self.invalid_property_default_response:
-            # take the params and headers that can be invalidated based on data type
-            # and expand the set with properties that can be invalided by relations
-            parameter_names = set(request_data.params_that_can_be_invalidated).union(
-                request_data.headers_that_can_be_invalidated
-            )
-            parameter_names.update(relation_property_names)
-            if not parameter_names:
-                raise ValueError(
-                    "None of the query parameters and headers can be invalidated."
-                )
-        else:
-            # non-default status_codes can only be the result of a Relation
-            parameter_names = relation_property_names
-
-        # Dto mappings may contain generic mappings for properties that are not present
-        # in this specific schema
-        request_data_parameter_names = [p.get("name") for p in request_data.parameters]
-        additional_relation_property_names = {
-            n for n in relation_property_names if n not in request_data_parameter_names
-        }
-        if additional_relation_property_names:
-            logger.warning(
-                f"get_parameter_relations_for_error_code yielded properties that are "
-                f"not defined in the schema: {additional_relation_property_names}\n"
-                f"These properties will be ignored for parameter invalidation."
-            )
-            parameter_names = parameter_names - additional_relation_property_names
-
-        if not parameter_names:
-            raise ValueError(
-                f"No parameter can be changed to cause status_code {status_code}."
-            )
-
-        parameter_names = parameter_names - parameters_to_ignore
-        parameter_to_invalidate = choice(tuple(parameter_names))
-
-        # check for invalid parameters in the provided request_data
-        try:
-            [parameter_data] = [
-                data
-                for data in request_data.parameters
-                if data["name"] == parameter_to_invalidate
-            ]
-        except Exception:
-            raise ValueError(
-                f"{parameter_to_invalidate} not found in provided parameters."
-            ) from None
-
-        # get the invalid_value for the chosen parameter
-        try:
-            [invalid_value_for_error_code] = [
-                r.invalid_value
-                for r in relations_for_status_code
-                if r.property_name == parameter_to_invalidate
-                and r.invalid_value_error_code == status_code
-            ]
-        except ValueError:
-            invalid_value_for_error_code = NOT_SET
-
-        # get the constraint values if available for the chosen parameter
-        try:
-            [values_from_constraint] = [
-                r.values
-                for r in relations_for_status_code
-                if r.property_name == parameter_to_invalidate
-            ]
-        except ValueError:
-            values_from_constraint = []
-
-        # if the parameter was not provided, add it to params / headers
-        params, headers = self.ensure_parameter_in_parameters(
-            parameter_to_invalidate=parameter_to_invalidate,
-            params=params,
-            headers=headers,
-            parameter_data=parameter_data,
-            values_from_constraint=values_from_constraint,
-        )
-
-        # determine the invalid_value
-        if invalid_value_for_error_code != NOT_SET:
-            invalid_value = invalid_value_for_error_code
-        else:
-            if parameter_to_invalidate in params.keys():
-                valid_value = params[parameter_to_invalidate]
-            else:
-                valid_value = headers[parameter_to_invalidate]
-
-            value_schema = resolve_schema(parameter_data["schema"])
-            invalid_value = value_utils.get_invalid_value(
-                value_schema=value_schema,
-                current_value=valid_value,
-                values_from_constraint=values_from_constraint,
-            )
-        logger.debug(f"{parameter_to_invalidate} changed to {invalid_value}")
-
-        # update the params / headers and return
-        if parameter_to_invalidate in params.keys():
-            params[parameter_to_invalidate] = invalid_value
-        else:
-            headers[parameter_to_invalidate] = invalid_value
-        return params, headers
-
-    @staticmethod
-    def ensure_parameter_in_parameters(
-        parameter_to_invalidate: str,
-        params: Dict[str, Any],
-        headers: Dict[str, str],
-        parameter_data: Dict[str, Any],
-        values_from_constraint: List[Any],
-    ) -> Tuple[Dict[str, Any], Dict[str, str]]:
-        """
-        Returns the params, headers tuple with parameter_to_invalidate with a valid
-        value to params or headers if not originally present.
-        """
-        if (
-            parameter_to_invalidate not in params.keys()
-            and parameter_to_invalidate not in headers.keys()
-        ):
-            if values_from_constraint:
-                valid_value = choice(values_from_constraint)
-            else:
-                parameter_schema = resolve_schema(parameter_data["schema"])
-                valid_value = value_utils.get_valid_value(parameter_schema)
-            if (
-                parameter_data["in"] == "query"
-                and parameter_to_invalidate not in params.keys()
-            ):
-                params[parameter_to_invalidate] = valid_value
-            if (
-                parameter_data["in"] == "header"
-                and parameter_to_invalidate not in headers.keys()
-            ):
-                headers[parameter_to_invalidate] = valid_value
-        return params, headers
-
-    @keyword
-    def ensure_in_use(self, url: str, resource_relation: IdReference) -> None:
-        """
-        Ensure that the (right-most) `id` of the resource referenced by the `url`
-        is used by the resource defined by the `resource_relation`.
-        """
-        resource_id = ""
-
-        endpoint = url.replace(self.base_url, "")
-        endpoint_parts = endpoint.split("/")
-        parameterized_endpoint = self.get_parametrized_endpoint(endpoint=endpoint)
-        parameterized_endpoint_parts = parameterized_endpoint.split("/")
-        for part, param_part in zip(
-            reversed(endpoint_parts), reversed(parameterized_endpoint_parts)
-        ):
-            if param_part.endswith("}"):
-                resource_id = part
-                break
-        if not resource_id:
-            raise ValueError(f"The provided url ({url}) does not contain an id.")
-        request_data = self.get_request_data(
-            method="post", endpoint=resource_relation.post_path
-        )
-        json_data = request_data.dto.as_dict()
-        json_data[resource_relation.property_name] = resource_id
-        post_url: str = run_keyword(
-            "get_valid_url",
-            resource_relation.post_path,
-            "post",
-        )
-        response: Response = run_keyword(
-            "authorized_request",
-            post_url,
-            "post",
-            request_data.params,
-            request_data.headers,
-            json_data,
-        )
-        if not response.ok:
-            logger.debug(
-                f"POST on {post_url} with json {json_data} failed: {response.json()}"
-            )
-            response.raise_for_status()
-
-    @keyword
-    def get_json_data_with_conflict(
-        self, url: str, method: str, dto: Dto, conflict_status_code: int
-    ) -> Dict[str, Any]:
-        """
-        Return `json_data` based on the `UniquePropertyValueConstraint` that must be
-        returned by the `get_relations` implementation on the `dto` for the given
-        `conflict_status_code`.
-        """
-        method = method.lower()
-        json_data = dto.as_dict()
-        unique_property_value_constraints = [
-            r
-            for r in dto.get_relations()
-            if isinstance(r, UniquePropertyValueConstraint)
-        ]
-        for relation in unique_property_value_constraints:
-            json_data[relation.property_name] = relation.value
-            # create a new resource that the original request will conflict with
-            if method in ["patch", "put"]:
-                post_url_parts = url.split("/")[:-1]
-                post_url = "/".join(post_url_parts)
-                # the PATCH or PUT may use a different dto than required for POST
-                # so a valid POST dto must be constructed
-                endpoint = post_url.replace(self.base_url, "")
-                request_data = self.get_request_data(endpoint=endpoint, method="post")
-                post_json = request_data.dto.as_dict()
-                for key in post_json.keys():
-                    if key in json_data:
-                        post_json[key] = json_data.get(key)
-            else:
-                post_url = url
-                post_json = json_data
-            endpoint = post_url.replace(self.base_url, "")
-            request_data = self.get_request_data(endpoint=endpoint, method="post")
-            response: Response = run_keyword(
-                "authorized_request",
-                post_url,
-                "post",
-                request_data.params,
-                request_data.headers,
-                post_json,
-            )
-            # conflicting resource may already exist
-            assert (
-                response.ok or response.status_code == conflict_status_code
-            ), f"get_json_data_with_conflict received {response.status_code}: {response.json()}"
-            return json_data
-        raise ValueError(
-            f"No UniquePropertyValueConstraint in the get_relations list on dto {dto}."
-        )
-
-    @keyword
-    def authorized_request(  # pylint: disable=too-many-arguments
-        self,
-        url: str,
-        method: str,
-        params: Optional[Dict[str, Any]] = None,
-        headers: Optional[Dict[str, str]] = None,
-        json_data: Optional[JSON] = None,
-    ) -> Response:
-        """
-        Perform a request using the security token or authentication set in the library.
-
-        > Note: provided username / password or auth objects take precedence over token
-            based security
-        """
-        headers = headers if headers else {}
-        if self.extra_headers:
-            headers.update(self.extra_headers)
-        # if both an auth object and a token are available, auth takes precedence
-        if self.security_token and not self.auth:
-            security_header = {"Authorization": self.security_token}
-            headers.update(security_header)
-        headers = {k: str(v) for k, v in headers.items()}
-        response = self.session.request(
-            url=url,
-            method=method,
-            params=params,
-            headers=headers,
-            json=json_data,
-            cookies=self.cookies,
-            auth=self.auth,
-            proxies=self.proxies,
-            verify=self.verify,
-            cert=self.cert,
-        )
-        logger.debug(f"Response text: {response.text}")
-        return response
+"""
+# OpenApiLibCore for Robot Framework
+
+The OpenApiLibCore library is a utility library that is meant to simplify creation
+of other Robot Framework libraries for API testing based on the information in
+an OpenAPI document (also known as Swagger document).
+This document explains how to use the OpenApiLibCore library.
+
+My RoboCon 2022 talk about OpenApiDriver and OpenApiLibCore can be found
+[here](https://www.youtube.com/watch?v=7YWZEHxk9Ps)
+
+For more information about Robot Framework, see http://robotframework.org.
+
+---
+
+> Note: OpenApiLibCore is still being developed so there are currently
+restrictions / limitations that you may encounter when using this library to run
+tests against an API. See [Limitations](#limitations) for details.
+
+---
+
+## Installation
+
+If you already have Python >= 3.8 with pip installed, you can simply run:
+
+`pip install --upgrade robotframework-openapi-libcore`
+
+---
+
+## OpenAPI (aka Swagger)
+
+The OpenAPI Specification (OAS) defines a standard, language-agnostic interface
+to RESTful APIs, see https://swagger.io/specification/
+
+The OpenApiLibCore implements a number of Robot Framework keywords that make it
+easy to interact with an OpenAPI implementation by using the information in the
+openapi document (Swagger file), for examply by automatic generation of valid values
+for requests based on the schema information in the document.
+
+> Note: OpenApiLibCore is designed for APIs based on the OAS v3
+The library has not been tested for APIs based on the OAS v2.
+
+---
+
+## Getting started
+
+Before trying to use the keywords exposed by OpenApiLibCore on the target API
+it's recommended to first ensure that the openapi document for the API is valid
+under the OpenAPI Specification.
+
+This can be done using the command line interface of a package that is installed as
+a prerequisite for OpenApiLibCore.
+Both a local openapi.json or openapi.yaml file or one hosted by the API server
+can be checked using the `prance validate <reference_to_file>` shell command:
+
+```shell
+prance validate --backend=openapi-spec-validator http://localhost:8000/openapi.json
+Processing "http://localhost:8000/openapi.json"...
+ -> Resolving external references.
+Validates OK as OpenAPI 3.0.2!
+
+prance validate --backend=openapi-spec-validator /tests/files/petstore_openapi.yaml
+Processing "/tests/files/petstore_openapi.yaml"...
+ -> Resolving external references.
+Validates OK as OpenAPI 3.0.2!
+```
+
+You'll have to change the url or file reference to the location of the openapi
+document for your API.
+
+> Note: Although recursion is technically allowed under the OAS, tool support is limited
+and changing the OAS to not use recursion is recommended.
+OpenApiLibCore has limited support for parsing OpenAPI documents with
+recursion in them. See the `recursion_limit` and `recursion_default` parameters.
+
+If the openapi document passes this validation, the next step is trying to do a test
+run with a minimal test suite.
+The example below can be used, with `source`, `origin` and 'endpoint' altered to
+fit your situation.
+
+``` robotframework
+*** Settings ***
+Library            OpenApiLibCore
+...                    source=http://localhost:8000/openapi.json
+...                    origin=http://localhost:8000
+
+*** Test Cases ***
+Getting Started
+    ${url}=    Get Valid Url    endpoint=/employees/{employee_id}   method=get
+
+```
+
+Running the above suite for the first time may result in an error / failed test.
+You should look at the Robot Framework `log.html` to determine the reasons
+for the failing tests.
+Depending on the reasons for the failures, different solutions are possible.
+
+Details about the OpenApiLibCore library parameters and keywords that you may need can be found
+[here](https://marketsquare.github.io/robotframework-openapi-libcore/openapi_libcore.html).
+
+The OpenApiLibCore also support handling of relations between resources within the scope
+of the API being validated as well as handling dependencies on resources outside the
+scope of the API. In addition there is support for handling restrictions on the values
+of parameters and properties.
+
+Details about the `mappings_path` variable usage can be found
+[here](https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html).
+
+---
+
+## Limitations
+
+There are currently a number of limitations to supported API structures, supported
+data types and properties. The following list details the most important ones:
+- Only JSON request and response bodies are supported.
+- No support for per-endpoint authorization levels.
+- Parsing of OAS 3.1 documents is supported by the parsing tools, but runtime behavior is untested.
+
+"""
+
+import json as _json
+import re
+import sys
+from copy import deepcopy
+from dataclasses import Field, dataclass, field, make_dataclass
+from functools import cached_property
+from itertools import zip_longest
+from logging import getLogger
+from pathlib import Path
+from random import choice
+from typing import Any, Dict, List, Optional, Set, Tuple, Type, Union
+from uuid import uuid4
+
+from openapi_core import Config, OpenAPI, Spec
+from openapi_core.contrib.requests import (
+    RequestsOpenAPIRequest,
+    RequestsOpenAPIResponse,
+)
+from prance import ResolvingParser, ValidationError
+from prance.util.url import ResolutionError
+from requests import Response, Session
+from requests.auth import AuthBase, HTTPBasicAuth
+from requests.cookies import RequestsCookieJar as CookieJar
+from robot.api.deco import keyword, library
+from robot.libraries.BuiltIn import BuiltIn
+
+from OpenApiLibCore import value_utils
+from OpenApiLibCore.dto_base import (
+    NOT_SET,
+    Dto,
+    IdDependency,
+    IdReference,
+    PathPropertiesConstraint,
+    PropertyValueConstraint,
+    Relation,
+    UniquePropertyValueConstraint,
+    resolve_schema,
+)
+from OpenApiLibCore.dto_utils import (
+    DEFAULT_ID_PROPERTY_NAME,
+    DefaultDto,
+    get_dto_class,
+    get_id_property_name,
+)
+from OpenApiLibCore.oas_cache import PARSER_CACHE
+from OpenApiLibCore.value_utils import FAKE, IGNORE, JSON
+
+run_keyword = BuiltIn().run_keyword
+
+logger = getLogger(__name__)
+
+
+def get_safe_key(key: str) -> str:
+    """
+    Helper function to convert a valid JSON property name to a string that can be used
+    as a Python variable or function / method name.
+    """
+    key = key.replace("-", "_")
+    key = key.replace("@", "_")
+    if key[0].isdigit():
+        key = f"_{key}"
+    return key
+
+
+@dataclass
+class RequestValues:
+    """Helper class to hold parameter values needed to make a request."""
+
+    url: str
+    method: str
+    params: Optional[Dict[str, Any]]
+    headers: Optional[Dict[str, str]]
+    json_data: Optional[Dict[str, Any]]
+
+
+@dataclass
+class RequestData:
+    """Helper class to manage parameters used when making requests."""
+
+    dto: Union[Dto, DefaultDto] = field(default_factory=DefaultDto)
+    dto_schema: Dict[str, Any] = field(default_factory=dict)
+    parameters: List[Dict[str, Any]] = field(default_factory=list)
+    params: Dict[str, Any] = field(default_factory=dict)
+    headers: Dict[str, Any] = field(default_factory=dict)
+    has_body: bool = True
+
+    def __post_init__(self) -> None:
+        # prevent modification by reference
+        self.dto_schema = deepcopy(self.dto_schema)
+        self.parameters = deepcopy(self.parameters)
+        self.params = deepcopy(self.params)
+        self.headers = deepcopy(self.headers)
+
+    @property
+    def has_optional_properties(self) -> bool:
+        """Whether or not the dto data (json data) contains optional properties."""
+
+        def is_required_property(property_name: str) -> bool:
+            return property_name in self.dto_schema.get("required", [])
+
+        properties = (self.dto.as_dict()).keys()
+        return not all(map(is_required_property, properties))
+
+    @property
+    def has_optional_params(self) -> bool:
+        """Whether or not any of the query parameters are optional."""
+
+        def is_optional_param(query_param: str) -> bool:
+            optional_params = [
+                p.get("name")
+                for p in self.parameters
+                if p.get("in") == "query" and not p.get("required")
+            ]
+            return query_param in optional_params
+
+        return any(map(is_optional_param, self.params))
+
+    @cached_property
+    def params_that_can_be_invalidated(self) -> Set[str]:
+        """
+        The query parameters that can be invalidated by violating data
+        restrictions, data type or by not providing them in a request.
+        """
+        result = set()
+        params = [h for h in self.parameters if h.get("in") == "query"]
+        for param in params:
+            # required params can be omitted to invalidate a request
+            if param["required"]:
+                result.add(param["name"])
+                continue
+
+            schema = resolve_schema(param["schema"])
+            if schema.get("type", None):
+                param_types = [schema]
+            else:
+                param_types = schema["types"]
+            for param_type in param_types:
+                # any basic non-string type except "null" can be invalidated by
+                # replacing it with a string
+                if param_type["type"] not in ["string", "array", "object", "null"]:
+                    result.add(param["name"])
+                    continue
+                # enums, strings and arrays with boundaries can be invalidated
+                if set(param_type.keys()).intersection(
+                    {
+                        "enum",
+                        "minLength",
+                        "maxLength",
+                        "minItems",
+                        "maxItems",
+                    }
+                ):
+                    result.add(param["name"])
+                    continue
+                # an array of basic non-string type can be invalidated by replacing the
+                # items in the array with strings
+                if param_type["type"] == "array" and param_type["items"][
+                    "type"
+                ] not in [
+                    "string",
+                    "array",
+                    "object",
+                    "null",
+                ]:
+                    result.add(param["name"])
+        return result
+
+    @property
+    def has_optional_headers(self) -> bool:
+        """Whether or not any of the headers are optional."""
+
+        def is_optional_header(header: str) -> bool:
+            optional_headers = [
+                p.get("name")
+                for p in self.parameters
+                if p.get("in") == "header" and not p.get("required")
+            ]
+            return header in optional_headers
+
+        return any(map(is_optional_header, self.headers))
+
+    @cached_property
+    def headers_that_can_be_invalidated(self) -> Set[str]:
+        """
+        The header parameters that can be invalidated by violating data
+        restrictions or by not providing them in a request.
+        """
+        result = set()
+        headers = [h for h in self.parameters if h.get("in") == "header"]
+        for header in headers:
+            # required headers can be omitted to invalidate a request
+            if header["required"]:
+                result.add(header["name"])
+                continue
+
+            schema = resolve_schema(header["schema"])
+            if schema.get("type", None):
+                header_types = [schema]
+            else:
+                header_types = schema["types"]
+            for header_type in header_types:
+                # any basic non-string type except "null" can be invalidated by
+                # replacing it with a string
+                if header_type["type"] not in ["string", "array", "object", "null"]:
+                    result.add(header["name"])
+                    continue
+                # enums, strings and arrays with boundaries can be invalidated
+                if set(header_type.keys()).intersection(
+                    {
+                        "enum",
+                        "minLength",
+                        "maxLength",
+                        "minItems",
+                        "maxItems",
+                    }
+                ):
+                    result.add(header["name"])
+                    continue
+                # an array of basic non-string type can be invalidated by replacing the
+                # items in the array with strings
+                if header_type["type"] == "array" and header_type["items"][
+                    "type"
+                ] not in [
+                    "string",
+                    "array",
+                    "object",
+                    "null",
+                ]:
+                    result.add(header["name"])
+        return result
+
+    def get_required_properties_dict(self) -> Dict[str, Any]:
+        """Get the json-compatible dto data containing only the required properties."""
+        required_properties = self.dto_schema.get("required", [])
+        required_properties_dict: Dict[str, Any] = {}
+        for key, value in (self.dto.as_dict()).items():
+            if key in required_properties:
+                required_properties_dict[key] = value
+        return required_properties_dict
+
+    def get_required_params(self) -> Dict[str, str]:
+        """Get the params dict containing only the required query parameters."""
+        required_parameters = [
+            p.get("name") for p in self.parameters if p.get("required")
+        ]
+        return {k: v for k, v in self.params.items() if k in required_parameters}
+
+    def get_required_headers(self) -> Dict[str, str]:
+        """Get the headers dict containing only the required headers."""
+        required_parameters = [
+            p.get("name") for p in self.parameters if p.get("required")
+        ]
+        return {k: v for k, v in self.headers.items() if k in required_parameters}
+
+
+@library(scope="TEST SUITE", doc_format="ROBOT")
+class OpenApiLibCore:  # pylint: disable=too-many-instance-attributes
+    """
+    Main class providing the keywords and core logic to interact with an OpenAPI server.
+
+    Visit the [https://github.com/MarketSquare/robotframework-openapi-libcore | library page]
+    for an introduction.
+    """
+
+    def __init__(  # pylint: disable=too-many-arguments, too-many-locals, dangerous-default-value
+        self,
+        source: str,
+        origin: str = "",
+        base_path: str = "",
+        mappings_path: Union[str, Path] = "",
+        invalid_property_default_response: int = 422,
+        default_id_property_name: str = "id",
+        faker_locale: Optional[Union[str, List[str]]] = None,
+        recursion_limit: int = 1,
+        recursion_default: Any = {},
+        username: str = "",
+        password: str = "",
+        security_token: str = "",
+        auth: Optional[AuthBase] = None,
+        cert: Optional[Union[str, Tuple[str, str]]] = None,
+        verify_tls: Optional[Union[bool, str]] = True,
+        extra_headers: Optional[Dict[str, str]] = None,
+        cookies: Optional[Union[Dict[str, str], CookieJar]] = None,
+        proxies: Optional[Dict[str, str]] = None,
+    ) -> None:
+        """
+        == Base parameters ==
+
+        === source ===
+        An absolute path to an openapi.json or openapi.yaml file or an url to such a file.
+
+        === origin ===
+        The server (and port) of the target server. E.g. ``https://localhost:8000``
+
+        === base_path ===
+        The routing between ``origin`` and the endpoints as found in the ``paths``
+        section in the openapi document.
+        E.g. ``/petshop/v2``.
+
+        == API-specific configurations ==
+
+        === mappings_path ===
+        See [https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html | this page]
+        for an in-depth explanation.
+
+        === invalid_property_default_response ===
+        The default response code for requests with a JSON body that does not comply
+        with the schema.
+        Example: a value outside the specified range or a string value
+        for a property defined as integer in the schema.
+
+        === default_id_property_name ===
+        The default name for the property that identifies a resource (i.e. a unique
+        entity) within the API.
+        The default value for this property name is ``id``.
+        If the target API uses a different name for all the resources within the API,
+        you can configure it globally using this property.
+
+        If different property names are used for the unique identifier for different
+        types of resources, an ``ID_MAPPING`` can be implemented using the ``mappings_path``.
+
+        === faker_locale ===
+        A locale string or list of locale strings to pass to the Faker library to be
+        used in generation of string data for supported format types.
+
+        == Parsing parameters ==
+
+        === recursion_limit ===
+        The recursion depth to which to fully parse recursive references before the
+        `recursion_default` is used to end the recursion.
+
+        === recursion_default ===
+        The value that is used instead of the referenced schema when the
+        `recursion_limit` has been reached.
+        The default `{}` represents an empty object in JSON.
+        Depending on schema definitions, this may cause schema validation errors.
+        If this is the case, 'None' (``${NONE}`` in Robot Framework) or an empty list
+        can be tried as an alternative.
+
+        == Security-related parameters ==
+        _Note: these parameters are equivalent to those in the ``requests`` library._
+
+        === username ===
+        The username to be used for Basic Authentication.
+
+        === password ===
+        The password to be used for Basic Authentication.
+
+        === security_token ===
+        The token to be used for token based security using the ``Authorization`` header.
+
+        === auth ===
+        A [https://requests.readthedocs.io/en/latest/api/#authentication | requests ``AuthBase`` instance]
+        to be used for authentication instead of the ``username`` and ``password``.
+
+        === cert ===
+        The SSL certificate to use with all requests.
+        If string: the path to ssl client cert file (.pem).
+        If tuple: the ('cert', 'key') pair.
+
+        === verify_tls ===
+        Whether or not to verify the TLS / SSL certificate of the server.
+        If boolean: whether or not to verify the server TLS certificate.
+        If string: path to a CA bundle to use for verification.
+
+        === extra_headers ===
+        A dictionary with extra / custom headers that will be send with every request.
+        This parameter can be used to send headers that are not documented in the
+        openapi document or to provide an API-key.
+
+        === cookies ===
+        A dictionary or
+        [https://docs.python.org/3/library/http.cookiejar.html#http.cookiejar.CookieJar | CookieJar object]
+        to send with all requests.
+
+        === proxies ===
+        A dictionary of 'protocol': 'proxy url' to use for all requests.
+        """
+        self._source = source
+        self._origin = origin
+        self._base_path = base_path
+        self._recursion_limit = recursion_limit
+        self._recursion_default = recursion_default
+        self.session = Session()
+        # only username and password, security_token or auth object should be provided
+        # if multiple are provided, username and password take precedence
+        self.security_token = security_token
+        self.auth = auth
+        if username and password:
+            self.auth = HTTPBasicAuth(username, password)
+        # Robot Framework does not allow users to create tuples and requests
+        # does not accept lists, so perform the conversion here
+        if isinstance(cert, list):
+            cert = tuple(cert)
+        self.cert = cert
+        self.verify = verify_tls
+        self.extra_headers = extra_headers
+        self.cookies = cookies
+        self.proxies = proxies
+        self.invalid_property_default_response = invalid_property_default_response
+        if mappings_path and str(mappings_path) != ".":
+            mappings_path = Path(mappings_path)
+            if not mappings_path.is_file():
+                logger.warning(
+                    f"mappings_path '{mappings_path}' is not a Python module."
+                )
+            # intermediate variable to ensure path.append is possible so we'll never
+            # path.pop a location that we didn't append
+            mappings_folder = str(mappings_path.parent)
+            sys.path.append(mappings_folder)
+            mappings_module_name = mappings_path.stem
+            self.get_dto_class = get_dto_class(
+                mappings_module_name=mappings_module_name
+            )
+            self.get_id_property_name = get_id_property_name(
+                mappings_module_name=mappings_module_name
+            )
+            sys.path.pop()
+        else:
+            self.get_dto_class = get_dto_class(mappings_module_name="no mapping")
+            self.get_id_property_name = get_id_property_name(
+                mappings_module_name="no mapping"
+            )
+        if faker_locale:
+            FAKE.set_locale(locale=faker_locale)
+        # update the globally available DEFAULT_ID_PROPERTY_NAME to the provided value
+        DEFAULT_ID_PROPERTY_NAME.id_property_name = default_id_property_name
+
+    @property
+    def origin(self) -> str:
+        return self._origin
+
+    @keyword
+    def set_origin(self, origin: str) -> None:
+        """
+        Update the `origin` after the library is imported.
+
+        This can be done during the `Suite setup` when using DataDriver in situations
+        where the OpenAPI document is available on disk but the target host address is
+        not known before the test starts.
+
+        In combination with OpenApiLibCore, the `origin` can be used at any point to
+        target another server that hosts an API that complies to the same OAS.
+        """
+        self._origin = origin
+
+    @property
+    def base_url(self) -> str:
+        return f"{self.origin}{self._base_path}"
+
+    @cached_property
+    def validation_spec(self) -> Spec:
+        return Spec.from_dict(self.openapi_spec)
+
+    @property
+    def openapi_spec(self) -> Dict[str, Any]:
+        """Return a deepcopy of the parsed openapi document."""
+        # protect the parsed openapi spec from being mutated by reference
+        return deepcopy(self._openapi_spec)
+
+    @cached_property
+    def _openapi_spec(self) -> Dict[str, Any]:
+        parser = self._load_parser()
+        return parser.specification
+
+    def read_paths(self) -> Dict[str, Any]:
+        return self.openapi_spec["paths"]
+
+    def _load_parser(self) -> ResolvingParser:
+        try:
+
+            def recursion_limit_handler(
+                limit: int, refstring: str, recursions: Any
+            ) -> Any:
+                return self._recursion_default
+
+            # Since parsing of the OAS and creating the Spec can take a long time,
+            # they are cached. This is done by storing them in an imported module that
+            # will have a global scope due to how the Python import system works. This
+            # ensures that in a Suite of Suites where multiple Suites use the same
+            # `source`, that OAS is only parsed / loaded once.
+            parser = PARSER_CACHE.get(self._source, None)
+            if parser is None:
+                parser = ResolvingParser(
+                    self._source,
+                    backend="openapi-spec-validator",
+                    recursion_limit=self._recursion_limit,
+                    recursion_limit_handler=recursion_limit_handler,
+                )
+
+                if parser.specification is None:  # pragma: no cover
+                    BuiltIn().fatal_error(
+                        "Source was loaded, but no specification was present after parsing."
+                    )
+
+                PARSER_CACHE[self._source] = parser
+
+            return parser
+
+        except ResolutionError as exception:
+            BuiltIn().fatal_error(
+                f"ResolutionError while trying to load openapi spec: {exception}"
+            )
+        except ValidationError as exception:
+            BuiltIn().fatal_error(
+                f"ValidationError while trying to load openapi spec: {exception}"
+            )
+
+    def validate_response_vs_spec(
+        self, request: RequestsOpenAPIRequest, response: RequestsOpenAPIResponse
+    ) -> None:
+        """
+        Validate the reponse for a given request against the OpenAPI Spec that is
+        loaded during library initialization.
+        """
+        if response.content_type == "application/json":
+            config = None
+        else:
+            extra_deserializer = {response.content_type: _json.loads}
+            config = Config(extra_media_type_deserializers=extra_deserializer)
+
+        OpenAPI(spec=self.validation_spec, config=config).validate_response(
+            request, response
+        )
+
+    @keyword
+    def get_valid_url(self, endpoint: str, method: str) -> str:
+        """
+        This keyword returns a valid url for the given `endpoint` and `method`.
+
+        If the `endpoint` contains path parameters the Get Valid Id For Endpoint
+        keyword will be executed to retrieve valid ids for the path parameters.
+
+        > Note: if valid ids cannot be retrieved within the scope of the API, the
+        `PathPropertiesConstraint` Relation can be used. More information can be found
+        [https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html | here].
+        """
+        method = method.lower()
+        try:
+            # endpoint can be partially resolved or provided by a PathPropertiesConstraint
+            parametrized_endpoint = self.get_parametrized_endpoint(endpoint=endpoint)
+            _ = self.openapi_spec["paths"][parametrized_endpoint]
+        except KeyError:
+            raise ValueError(
+                f"{endpoint} not found in paths section of the OpenAPI document."
+            ) from None
+        dto_class = self.get_dto_class(endpoint=endpoint, method=method)
+        relations = dto_class.get_relations()
+        paths = [p.path for p in relations if isinstance(p, PathPropertiesConstraint)]
+        if paths:
+            url = f"{self.base_url}{choice(paths)}"
+            return url
+        endpoint_parts = list(endpoint.split("/"))
+        for index, part in enumerate(endpoint_parts):
+            if part.startswith("{") and part.endswith("}"):
+                type_endpoint_parts = endpoint_parts[slice(index)]
+                type_endpoint = "/".join(type_endpoint_parts)
+                existing_id: Union[str, int, float] = run_keyword(
+                    "get_valid_id_for_endpoint", type_endpoint, method
+                )
+                endpoint_parts[index] = str(existing_id)
+        resolved_endpoint = "/".join(endpoint_parts)
+        url = f"{self.base_url}{resolved_endpoint}"
+        return url
+
+    @keyword
+    def get_valid_id_for_endpoint(
+        self, endpoint: str, method: str
+    ) -> Union[str, int, float]:
+        """
+        Support keyword that returns the `id` for an existing resource at `endpoint`.
+
+        To prevent resource conflicts with other test cases, a new resource is created
+        (POST) if possible.
+        """
+
+        def dummy_transformer(
+            valid_id: Union[str, int, float]
+        ) -> Union[str, int, float]:
+            return valid_id
+
+        method = method.lower()
+        url: str = run_keyword("get_valid_url", endpoint, method)
+        # Try to create a new resource to prevent conflicts caused by
+        # operations performed on the same resource by other test cases
+        request_data = self.get_request_data(endpoint=endpoint, method="post")
+
+        response: Response = run_keyword(
+            "authorized_request",
+            url,
+            "post",
+            request_data.get_required_params(),
+            request_data.get_required_headers(),
+            request_data.get_required_properties_dict(),
+        )
+
+        # determine the id property name for this path and whether or not a transformer is used
+        mapping = self.get_id_property_name(endpoint=endpoint)
+        if isinstance(mapping, str):
+            id_property = mapping
+            # set the transformer to a dummy callable that returns the original value so
+            # the transformer can be applied on any returned id
+            id_transformer = dummy_transformer
+        else:
+            id_property, id_transformer = mapping
+
+        if not response.ok:
+            # If a new resource cannot be created using POST, try to retrieve a
+            # valid id using a GET request.
+            try:
+                valid_id = choice(run_keyword("get_ids_from_url", url))
+                return id_transformer(valid_id)
+            except Exception as exception:
+                raise AssertionError(
+                    f"Failed to get a valid id using GET on {url}"
+                ) from exception
+
+        response_data = response.json()
+        if prepared_body := response.request.body:
+            if isinstance(prepared_body, bytes):
+                send_json = _json.loads(prepared_body.decode("UTF-8"))
+            else:
+                send_json = _json.loads(prepared_body)
+        else:
+            send_json = None
+
+        # no support for retrieving an id from an array returned on a POST request
+        if isinstance(response_data, list):
+            raise NotImplementedError(
+                f"Unexpected response body for POST request: expected an object but "
+                f"received an array ({response_data})"
+            )
+
+        # POST on /resource_type/{id}/array_item/ will return the updated {id} resource
+        # instead of a newly created resource. In this case, the send_json must be
+        # in the array of the 'array_item' property on {id}
+        send_path: str = response.request.path_url
+        response_href: Optional[str] = response_data.get("href", None)
+        if response_href and (send_path not in response_href) and send_json:
+            try:
+                property_to_check = send_path.replace(response_href, "")[1:]
+                item_list: List[Dict[str, Any]] = response_data[property_to_check]
+                # Use the (mandatory) id to get the POSTed resource from the list
+                [valid_id] = [
+                    item[id_property]
+                    for item in item_list
+                    if item[id_property] == send_json[id_property]
+                ]
+            except Exception as exception:
+                raise AssertionError(
+                    f"Failed to get a valid id from {response_href}"
+                ) from exception
+        else:
+            try:
+                valid_id = response_data[id_property]
+            except KeyError:
+                raise AssertionError(
+                    f"Failed to get a valid id from {response_data}"
+                ) from None
+        return id_transformer(valid_id)
+
+    @keyword
+    def get_ids_from_url(self, url: str) -> List[str]:
+        """
+        Perform a GET request on the `url` and return the list of resource
+        `ids` from the response.
+        """
+        endpoint = self.get_parameterized_endpoint_from_url(url)
+        request_data = self.get_request_data(endpoint=endpoint, method="get")
+        response = run_keyword(
+            "authorized_request",
+            url,
+            "get",
+            request_data.get_required_params(),
+            request_data.get_required_headers(),
+        )
+        response.raise_for_status()
+        response_data: Union[Dict[str, Any], List[Dict[str, Any]]] = response.json()
+
+        # determine the property name to use
+        mapping = self.get_id_property_name(endpoint=endpoint)
+        if isinstance(mapping, str):
+            id_property = mapping
+        else:
+            id_property, _ = mapping
+
+        if isinstance(response_data, list):
+            valid_ids: List[str] = [item[id_property] for item in response_data]
+            return valid_ids
+        # if the response is an object (dict), check if it's hal+json
+        if embedded := response_data.get("_embedded"):
+            # there should be 1 item in the dict that has a value that's a list
+            for value in embedded.values():
+                if isinstance(value, list):
+                    valid_ids = [item[id_property] for item in value]
+                    return valid_ids
+        if (valid_id := response_data.get(id_property)) is not None:
+            return [valid_id]
+        valid_ids = [item[id_property] for item in response_data["items"]]
+        return valid_ids
+
+    @keyword
+    def get_request_data(self, endpoint: str, method: str) -> RequestData:
+        """Return an object with valid request data for body, headers and query params."""
+        method = method.lower()
+        dto_cls_name = self._get_dto_cls_name(endpoint=endpoint, method=method)
+        # The endpoint can contain already resolved Ids that have to be matched
+        # against the parametrized endpoints in the paths section.
+        spec_endpoint = self.get_parametrized_endpoint(endpoint)
+        dto_class = self.get_dto_class(endpoint=spec_endpoint, method=method)
+        try:
+            method_spec = self.openapi_spec["paths"][spec_endpoint][method]
+        except KeyError:
+            logger.info(
+                f"method '{method}' not supported on '{spec_endpoint}, using empty spec."
+            )
+            method_spec = {}
+
+        parameters, params, headers = self.get_request_parameters(
+            dto_class=dto_class, method_spec=method_spec
+        )
+        if (body_spec := method_spec.get("requestBody", None)) is None:
+            if dto_class == DefaultDto:
+                dto_instance: Dto = DefaultDto()
+            else:
+                dto_class = make_dataclass(
+                    cls_name=method_spec.get("operationId", dto_cls_name),
+                    fields=[],
+                    bases=(dto_class,),
+                )
+                dto_instance = dto_class()
+            return RequestData(
+                dto=dto_instance,
+                parameters=parameters,
+                params=params,
+                headers=headers,
+                has_body=False,
+            )
+        content_schema = resolve_schema(self.get_content_schema(body_spec))
+        headers.update({"content-type": self.get_content_type(body_spec)})
+        dto_data = self.get_json_data_for_dto_class(
+            schema=content_schema,
+            dto_class=dto_class,
+            operation_id=method_spec.get("operationId", ""),
+        )
+        if dto_data is None:
+            dto_instance = DefaultDto()
+        else:
+            fields = self.get_fields_from_dto_data(content_schema, dto_data)
+            dto_class = make_dataclass(
+                cls_name=method_spec.get("operationId", dto_cls_name),
+                fields=fields,
+                bases=(dto_class,),
+            )
+            dto_data = {get_safe_key(key): value for key, value in dto_data.items()}
+            dto_instance = dto_class(**dto_data)
+        return RequestData(
+            dto=dto_instance,
+            dto_schema=content_schema,
+            parameters=parameters,
+            params=params,
+            headers=headers,
+        )
+
+    @staticmethod
+    def _get_dto_cls_name(endpoint: str, method: str) -> str:
+        method = method.capitalize()
+        path = endpoint.translate({ord(i): None for i in "{}"})
+        path_parts = path.split("/")
+        path_parts = [p.capitalize() for p in path_parts]
+        result = "".join([method, *path_parts])
+        return result
+
+    @staticmethod
+    def get_fields_from_dto_data(
+        content_schema: Dict[str, Any], dto_data: Dict[str, Any]
+    ):
+        # FIXME: annotation is not Pyhon 3.8-compatible
+        # ) -> List[Union[str, Tuple[str, Type[Any]], Tuple[str, Type[Any], Field[Any]]]]:
+        """Get a dataclasses fields list based on the content_schema and dto_data."""
+        fields: List[
+            Union[str, Tuple[str, Type[Any]], Tuple[str, Type[Any], Field[Any]]]
+        ] = []
+        for key, value in dto_data.items():
+            required_properties = content_schema.get("required", [])
+            safe_key = get_safe_key(key)
+            metadata = {"original_property_name": key}
+            if key in required_properties:
+                # The fields list is used to create a dataclass, so non-default fields
+                # must go before fields with a default
+                fields.insert(0, (safe_key, type(value), field(metadata=metadata)))
+            else:
+                fields.append((safe_key, type(value), field(default=None, metadata=metadata)))  # type: ignore[arg-type]
+        return fields
+
+    def get_request_parameters(
+        self, dto_class: Union[Dto, Type[Dto]], method_spec: Dict[str, Any]
+    ) -> Tuple[List[Dict[str, Any]], Dict[str, Any], Dict[str, str]]:
+        """Get the methods parameter spec and params and headers with valid data."""
+        parameters = method_spec.get("parameters", [])
+        parameter_relations = dto_class.get_parameter_relations()
+        query_params = [p for p in parameters if p.get("in") == "query"]
+        header_params = [p for p in parameters if p.get("in") == "header"]
+        params = self.get_parameter_data(query_params, parameter_relations)
+        headers = self.get_parameter_data(header_params, parameter_relations)
+        return parameters, params, headers
+
+    @classmethod
+    def get_content_schema(cls, body_spec: Dict[str, Any]) -> Dict[str, Any]:
+        """Get the content schema from the requestBody spec."""
+        content_type = cls.get_content_type(body_spec)
+        content_schema = body_spec["content"][content_type]["schema"]
+        return resolve_schema(content_schema)
+
+    @staticmethod
+    def get_content_type(body_spec: Dict[str, Any]) -> str:
+        """Get and validate the first supported content type from the requested body spec
+
+        Should be application/json like content type,
+        e.g "application/json;charset=utf-8" or "application/merge-patch+json"
+        """
+        content_types: List[str] = body_spec["content"].keys()
+        json_regex = r"application/([a-z\-]+\+)?json(;\s?charset=(.+))?"
+        for content_type in content_types:
+            if re.search(json_regex, content_type):
+                return content_type
+
+        # At present no supported for other types.
+        raise NotImplementedError(
+            f"Only content types like 'application/json' are supported. "
+            f"Content types definded in the spec are '{content_types}'."
+        )
+
+    def get_parametrized_endpoint(self, endpoint: str) -> str:
+        """
+        Get the parametrized endpoint as found in the `paths` section of the openapi
+        document from a (partially) resolved endpoint.
+        """
+
+        def match_parts(parts: List[str], spec_parts: List[str]) -> bool:
+            for part, spec_part in zip_longest(parts, spec_parts, fillvalue="Filler"):
+                if part == "Filler" or spec_part == "Filler":
+                    return False
+                if part != spec_part and not spec_part.startswith("{"):
+                    return False
+            return True
+
+        endpoint_parts = endpoint.split("/")
+        # if the last part is empty, the path has a trailing `/` that
+        # should be ignored during matching
+        if endpoint_parts[-1] == "":
+            _ = endpoint_parts.pop(-1)
+
+        spec_endpoints: List[str] = {**self.openapi_spec}["paths"].keys()
+
+        candidates: List[str] = []
+
+        for spec_endpoint in spec_endpoints:
+            spec_endpoint_parts = spec_endpoint.split("/")
+            # ignore trailing `/` the same way as for endpoint_parts
+            if spec_endpoint_parts[-1] == "":
+                _ = spec_endpoint_parts.pop(-1)
+            if match_parts(endpoint_parts, spec_endpoint_parts):
+                candidates.append(spec_endpoint)
+
+        if not candidates:
+            raise ValueError(
+                f"{endpoint} not found in paths section of the OpenAPI document."
+            )
+
+        if len(candidates) == 1:
+            return candidates[0]
+        # Multiple matches can happen in APIs with overloaded endpoints, e.g.
+        # /users/me
+        # /users/${user_id}
+        # In this case, find the closest (or exact) match
+        exact_match = [c for c in candidates if c == endpoint]
+        if exact_match:
+            return exact_match[0]
+        # TODO: Implement a decision mechanism when real-world examples become available
+        # In the face of ambiguity, refuse the temptation to guess.
+        raise ValueError(f"{endpoint} matched to multiple paths: {candidates}")
+
+    @staticmethod
+    def get_parameter_data(
+        parameters: List[Dict[str, Any]],
+        parameter_relations: List[Relation],
+    ) -> Dict[str, str]:
+        """Generate a valid list of key-value pairs for all parameters."""
+        result: Dict[str, str] = {}
+        value: Any = None
+        for parameter in parameters:
+            parameter_name = parameter["name"]
+            parameter_schema = resolve_schema(parameter["schema"])
+            relations = [
+                r for r in parameter_relations if r.property_name == parameter_name
+            ]
+            if constrained_values := [
+                r.values for r in relations if isinstance(r, PropertyValueConstraint)
+            ]:
+                value = choice(*constrained_values)
+                if value is IGNORE:
+                    continue
+                result[parameter_name] = value
+                continue
+            value = value_utils.get_valid_value(parameter_schema)
+            result[parameter_name] = value
+        return result
+
+    @keyword
+    def get_json_data_for_dto_class(
+        self,
+        schema: Dict[str, Any],
+        dto_class: Union[Dto, Type[Dto]],
+        operation_id: str = "",
+    ) -> Optional[Dict[str, Any]]:
+        """
+        Generate a valid (json-compatible) dict for all the `dto_class` properties.
+        """
+
+        def get_constrained_values(property_name: str) -> List[Any]:
+            relations = dto_class.get_relations()
+            values_list = [
+                c.values
+                for c in relations
+                if (
+                    isinstance(c, PropertyValueConstraint)
+                    and c.property_name == property_name
+                )
+            ]
+            # values should be empty or contain 1 list of allowed values
+            return values_list.pop() if values_list else []
+
+        def get_dependent_id(
+            property_name: str, operation_id: str
+        ) -> Optional[Union[str, int, float]]:
+            relations = dto_class.get_relations()
+            # multiple get paths are possible based on the operation being performed
+            id_get_paths = [
+                (d.get_path, d.operation_id)
+                for d in relations
+                if (isinstance(d, IdDependency) and d.property_name == property_name)
+            ]
+            if not id_get_paths:
+                return None
+            if len(id_get_paths) == 1:
+                id_get_path, _ = id_get_paths.pop()
+            else:
+                try:
+                    [id_get_path] = [
+                        path
+                        for path, operation in id_get_paths
+                        if operation == operation_id
+                    ]
+                # There could be multiple get_paths, but not one for the current operation
+                except ValueError:
+                    return None
+            valid_id = self.get_valid_id_for_endpoint(
+                endpoint=id_get_path, method="get"
+            )
+            logger.debug(f"get_dependent_id for {id_get_path} returned {valid_id}")
+            return valid_id
+
+        json_data: Dict[str, Any] = {}
+
+        for property_name in schema.get("properties", []):
+            properties_schema = schema["properties"][property_name]
+
+            property_type = properties_schema.get("type")
+            if property_type is None:
+                property_types = properties_schema.get("types")
+                if property_types is None:
+                    if properties_schema.get("properties") is not None:
+                        nested_data = self.get_json_data_for_dto_class(
+                            schema=properties_schema,
+                            dto_class=DefaultDto,
+                        )
+                        json_data[property_name] = nested_data
+                        continue
+                selected_type_schema = choice(property_types)
+                property_type = selected_type_schema["type"]
+            if properties_schema.get("readOnly", False):
+                continue
+            if constrained_values := get_constrained_values(property_name):
+                # do not add properties that are configured to be ignored
+                if IGNORE in constrained_values:
+                    continue
+                json_data[property_name] = choice(constrained_values)
+                continue
+            if (
+                dependent_id := get_dependent_id(
+                    property_name=property_name, operation_id=operation_id
+                )
+            ) is not None:
+                json_data[property_name] = dependent_id
+                continue
+            if property_type == "object":
+                object_data = self.get_json_data_for_dto_class(
+                    schema=properties_schema,
+                    dto_class=DefaultDto,
+                    operation_id="",
+                )
+                json_data[property_name] = object_data
+                continue
+            if property_type == "array":
+                array_data = self.get_json_data_for_dto_class(
+                    schema=properties_schema["items"],
+                    dto_class=DefaultDto,
+                    operation_id=operation_id,
+                )
+                json_data[property_name] = [array_data]
+                continue
+            json_data[property_name] = value_utils.get_valid_value(properties_schema)
+        return json_data
+
+    @keyword
+    def get_invalidated_url(self, valid_url: str) -> Optional[str]:
+        """
+        Return an url with all the path parameters in the `valid_url` replaced by a
+        random UUID.
+
+        Raises ValueError if the valid_url cannot be invalidated.
+        """
+        parameterized_endpoint = self.get_parameterized_endpoint_from_url(valid_url)
+        parameterized_url = self.base_url + parameterized_endpoint
+        valid_url_parts = list(reversed(valid_url.split("/")))
+        parameterized_parts = reversed(parameterized_url.split("/"))
+        for index, (parameterized_part, _) in enumerate(
+            zip(parameterized_parts, valid_url_parts)
+        ):
+            if parameterized_part.startswith("{") and parameterized_part.endswith("}"):
+                valid_url_parts[index] = uuid4().hex
+                valid_url_parts.reverse()
+                invalid_url = "/".join(valid_url_parts)
+                return invalid_url
+        raise ValueError(f"{parameterized_endpoint} could not be invalidated.")
+
+    @keyword
+    def get_parameterized_endpoint_from_url(self, url: str) -> str:
+        """
+        Return the endpoint as found in the `paths` section based on the given `url`.
+        """
+        endpoint = url.replace(self.base_url, "")
+        endpoint_parts = endpoint.split("/")
+        # first part will be '' since an endpoint starts with /
+        endpoint_parts.pop(0)
+        parameterized_endpoint = self.get_parametrized_endpoint(endpoint=endpoint)
+        return parameterized_endpoint
+
+    @keyword
+    def get_invalid_json_data(
+        self,
+        url: str,
+        method: str,
+        status_code: int,
+        request_data: RequestData,
+    ) -> Dict[str, Any]:
+        """
+        Return `json_data` based on the `dto` on the `request_data` that will cause
+        the provided `status_code` for the `method` operation on the `url`.
+
+        > Note: applicable UniquePropertyValueConstraint and IdReference Relations are
+            considered before changes to `json_data` are made.
+        """
+        method = method.lower()
+        data_relations = request_data.dto.get_relations_for_error_code(status_code)
+        if not data_relations:
+            if not request_data.dto_schema:
+                raise ValueError(
+                    "Failed to invalidate: no data_relations and empty schema."
+                )
+            json_data = request_data.dto.get_invalidated_data(
+                schema=request_data.dto_schema,
+                status_code=status_code,
+                invalid_property_default_code=self.invalid_property_default_response,
+            )
+            return json_data
+        resource_relation = choice(data_relations)
+        if isinstance(resource_relation, UniquePropertyValueConstraint):
+            json_data = run_keyword(
+                "get_json_data_with_conflict",
+                url,
+                method,
+                request_data.dto,
+                status_code,
+            )
+        elif isinstance(resource_relation, IdReference):
+            run_keyword("ensure_in_use", url, resource_relation)
+            json_data = request_data.dto.as_dict()
+        else:
+            json_data = request_data.dto.get_invalidated_data(
+                schema=request_data.dto_schema,
+                status_code=status_code,
+                invalid_property_default_code=self.invalid_property_default_response,
+            )
+        return json_data
+
+    @keyword
+    def get_invalidated_parameters(
+        self,
+        status_code: int,
+        request_data: RequestData,
+    ) -> Tuple[Dict[str, Any], Dict[str, str]]:
+        """
+        Returns a version of `params, headers` as present on `request_data` that has
+        been modified to cause the provided `status_code`.
+        """
+        if not request_data.parameters:
+            raise ValueError("No params or headers to invalidate.")
+
+        # ensure the status_code can be triggered
+        relations = request_data.dto.get_parameter_relations_for_error_code(status_code)
+        relations_for_status_code = [
+            r
+            for r in relations
+            if isinstance(r, PropertyValueConstraint)
+            and (
+                r.error_code == status_code or r.invalid_value_error_code == status_code
+            )
+        ]
+        parameters_to_ignore = {
+            r.property_name
+            for r in relations_for_status_code
+            if r.invalid_value_error_code == status_code and r.invalid_value == IGNORE
+        }
+        relation_property_names = {r.property_name for r in relations_for_status_code}
+        if not relation_property_names:
+            if status_code != self.invalid_property_default_response:
+                raise ValueError(
+                    f"No relations to cause status_code {status_code} found."
+                )
+
+        # ensure we're not modifying mutable properties
+        params = deepcopy(request_data.params)
+        headers = deepcopy(request_data.headers)
+
+        if status_code == self.invalid_property_default_response:
+            # take the params and headers that can be invalidated based on data type
+            # and expand the set with properties that can be invalided by relations
+            parameter_names = set(request_data.params_that_can_be_invalidated).union(
+                request_data.headers_that_can_be_invalidated
+            )
+            parameter_names.update(relation_property_names)
+            if not parameter_names:
+                raise ValueError(
+                    "None of the query parameters and headers can be invalidated."
+                )
+        else:
+            # non-default status_codes can only be the result of a Relation
+            parameter_names = relation_property_names
+
+        # Dto mappings may contain generic mappings for properties that are not present
+        # in this specific schema
+        request_data_parameter_names = [p.get("name") for p in request_data.parameters]
+        additional_relation_property_names = {
+            n for n in relation_property_names if n not in request_data_parameter_names
+        }
+        if additional_relation_property_names:
+            logger.warning(
+                f"get_parameter_relations_for_error_code yielded properties that are "
+                f"not defined in the schema: {additional_relation_property_names}\n"
+                f"These properties will be ignored for parameter invalidation."
+            )
+            parameter_names = parameter_names - additional_relation_property_names
+
+        if not parameter_names:
+            raise ValueError(
+                f"No parameter can be changed to cause status_code {status_code}."
+            )
+
+        parameter_names = parameter_names - parameters_to_ignore
+        parameter_to_invalidate = choice(tuple(parameter_names))
+
+        # check for invalid parameters in the provided request_data
+        try:
+            [parameter_data] = [
+                data
+                for data in request_data.parameters
+                if data["name"] == parameter_to_invalidate
+            ]
+        except Exception:
+            raise ValueError(
+                f"{parameter_to_invalidate} not found in provided parameters."
+            ) from None
+
+        # get the invalid_value for the chosen parameter
+        try:
+            [invalid_value_for_error_code] = [
+                r.invalid_value
+                for r in relations_for_status_code
+                if r.property_name == parameter_to_invalidate
+                and r.invalid_value_error_code == status_code
+            ]
+        except ValueError:
+            invalid_value_for_error_code = NOT_SET
+
+        # get the constraint values if available for the chosen parameter
+        try:
+            [values_from_constraint] = [
+                r.values
+                for r in relations_for_status_code
+                if r.property_name == parameter_to_invalidate
+            ]
+        except ValueError:
+            values_from_constraint = []
+
+        # if the parameter was not provided, add it to params / headers
+        params, headers = self.ensure_parameter_in_parameters(
+            parameter_to_invalidate=parameter_to_invalidate,
+            params=params,
+            headers=headers,
+            parameter_data=parameter_data,
+            values_from_constraint=values_from_constraint,
+        )
+
+        # determine the invalid_value
+        if invalid_value_for_error_code != NOT_SET:
+            invalid_value = invalid_value_for_error_code
+        else:
+            if parameter_to_invalidate in params.keys():
+                valid_value = params[parameter_to_invalidate]
+            else:
+                valid_value = headers[parameter_to_invalidate]
+
+            value_schema = resolve_schema(parameter_data["schema"])
+            invalid_value = value_utils.get_invalid_value(
+                value_schema=value_schema,
+                current_value=valid_value,
+                values_from_constraint=values_from_constraint,
+            )
+        logger.debug(f"{parameter_to_invalidate} changed to {invalid_value}")
+
+        # update the params / headers and return
+        if parameter_to_invalidate in params.keys():
+            params[parameter_to_invalidate] = invalid_value
+        else:
+            headers[parameter_to_invalidate] = invalid_value
+        return params, headers
+
+    @staticmethod
+    def ensure_parameter_in_parameters(
+        parameter_to_invalidate: str,
+        params: Dict[str, Any],
+        headers: Dict[str, str],
+        parameter_data: Dict[str, Any],
+        values_from_constraint: List[Any],
+    ) -> Tuple[Dict[str, Any], Dict[str, str]]:
+        """
+        Returns the params, headers tuple with parameter_to_invalidate with a valid
+        value to params or headers if not originally present.
+        """
+        if (
+            parameter_to_invalidate not in params.keys()
+            and parameter_to_invalidate not in headers.keys()
+        ):
+            if values_from_constraint:
+                valid_value = choice(values_from_constraint)
+            else:
+                parameter_schema = resolve_schema(parameter_data["schema"])
+                valid_value = value_utils.get_valid_value(parameter_schema)
+            if (
+                parameter_data["in"] == "query"
+                and parameter_to_invalidate not in params.keys()
+            ):
+                params[parameter_to_invalidate] = valid_value
+            if (
+                parameter_data["in"] == "header"
+                and parameter_to_invalidate not in headers.keys()
+            ):
+                headers[parameter_to_invalidate] = valid_value
+        return params, headers
+
+    @keyword
+    def ensure_in_use(self, url: str, resource_relation: IdReference) -> None:
+        """
+        Ensure that the (right-most) `id` of the resource referenced by the `url`
+        is used by the resource defined by the `resource_relation`.
+        """
+        resource_id = ""
+
+        endpoint = url.replace(self.base_url, "")
+        endpoint_parts = endpoint.split("/")
+        parameterized_endpoint = self.get_parametrized_endpoint(endpoint=endpoint)
+        parameterized_endpoint_parts = parameterized_endpoint.split("/")
+        for part, param_part in zip(
+            reversed(endpoint_parts), reversed(parameterized_endpoint_parts)
+        ):
+            if param_part.endswith("}"):
+                resource_id = part
+                break
+        if not resource_id:
+            raise ValueError(f"The provided url ({url}) does not contain an id.")
+        request_data = self.get_request_data(
+            method="post", endpoint=resource_relation.post_path
+        )
+        json_data = request_data.dto.as_dict()
+        json_data[resource_relation.property_name] = resource_id
+        post_url: str = run_keyword(
+            "get_valid_url",
+            resource_relation.post_path,
+            "post",
+        )
+        response: Response = run_keyword(
+            "authorized_request",
+            post_url,
+            "post",
+            request_data.params,
+            request_data.headers,
+            json_data,
+        )
+        if not response.ok:
+            logger.debug(
+                f"POST on {post_url} with json {json_data} failed: {response.json()}"
+            )
+            response.raise_for_status()
+
+    @keyword
+    def get_json_data_with_conflict(
+        self, url: str, method: str, dto: Dto, conflict_status_code: int
+    ) -> Dict[str, Any]:
+        """
+        Return `json_data` based on the `UniquePropertyValueConstraint` that must be
+        returned by the `get_relations` implementation on the `dto` for the given
+        `conflict_status_code`.
+        """
+        method = method.lower()
+        json_data = dto.as_dict()
+        unique_property_value_constraints = [
+            r
+            for r in dto.get_relations()
+            if isinstance(r, UniquePropertyValueConstraint)
+        ]
+        for relation in unique_property_value_constraints:
+            json_data[relation.property_name] = relation.value
+            # create a new resource that the original request will conflict with
+            if method in ["patch", "put"]:
+                post_url_parts = url.split("/")[:-1]
+                post_url = "/".join(post_url_parts)
+                # the PATCH or PUT may use a different dto than required for POST
+                # so a valid POST dto must be constructed
+                endpoint = post_url.replace(self.base_url, "")
+                request_data = self.get_request_data(endpoint=endpoint, method="post")
+                post_json = request_data.dto.as_dict()
+                for key in post_json.keys():
+                    if key in json_data:
+                        post_json[key] = json_data.get(key)
+            else:
+                post_url = url
+                post_json = json_data
+            endpoint = post_url.replace(self.base_url, "")
+            request_data = self.get_request_data(endpoint=endpoint, method="post")
+            response: Response = run_keyword(
+                "authorized_request",
+                post_url,
+                "post",
+                request_data.params,
+                request_data.headers,
+                post_json,
+            )
+            # conflicting resource may already exist
+            assert (
+                response.ok or response.status_code == conflict_status_code
+            ), f"get_json_data_with_conflict received {response.status_code}: {response.json()}"
+            return json_data
+        raise ValueError(
+            f"No UniquePropertyValueConstraint in the get_relations list on dto {dto}."
+        )
+
+    @keyword
+    def authorized_request(  # pylint: disable=too-many-arguments
+        self,
+        url: str,
+        method: str,
+        params: Optional[Dict[str, Any]] = None,
+        headers: Optional[Dict[str, str]] = None,
+        json_data: Optional[JSON] = None,
+    ) -> Response:
+        """
+        Perform a request using the security token or authentication set in the library.
+
+        > Note: provided username / password or auth objects take precedence over token
+            based security
+        """
+        headers = headers if headers else {}
+        if self.extra_headers:
+            headers.update(self.extra_headers)
+        # if both an auth object and a token are available, auth takes precedence
+        if self.security_token and not self.auth:
+            security_header = {"Authorization": self.security_token}
+            headers.update(security_header)
+        headers = {k: str(v) for k, v in headers.items()}
+        response = self.session.request(
+            url=url,
+            method=method,
+            params=params,
+            headers=headers,
+            json=json_data,
+            cookies=self.cookies,
+            auth=self.auth,
+            proxies=self.proxies,
+            verify=self.verify,
+            cert=self.cert,
+        )
+        logger.debug(f"Response text: {response.text}")
+        return response
```

### Comparing `robotframework_openapitools-0.1.2/src/OpenApiLibCore/value_utils.py` & `robotframework_openapitools-0.1.3/src/OpenApiLibCore/value_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.2/src/roboswag/auth.py` & `robotframework_openapitools-0.1.3/src/roboswag/auth.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.2/src/roboswag/cli.py` & `robotframework_openapitools-0.1.3/src/roboswag/cli.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.2/src/roboswag/core.py` & `robotframework_openapitools-0.1.3/src/roboswag/core.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.2/src/roboswag/generate/generate.py` & `robotframework_openapitools-0.1.3/src/roboswag/generate/generate.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.2/src/roboswag/generate/models/api.py` & `robotframework_openapitools-0.1.3/src/roboswag/generate/models/api.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.2/src/roboswag/generate/models/definition.py` & `robotframework_openapitools-0.1.3/src/roboswag/generate/models/definition.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.2/src/roboswag/generate/models/endpoint.py` & `robotframework_openapitools-0.1.3/src/roboswag/generate/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.2/src/roboswag/generate/models/parameter.py` & `robotframework_openapitools-0.1.3/src/roboswag/generate/models/parameter.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.2/src/roboswag/generate/models/tag.py` & `robotframework_openapitools-0.1.3/src/roboswag/generate/models/tag.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.2/src/roboswag/generate/models/utils.py` & `robotframework_openapitools-0.1.3/src/roboswag/generate/models/utils.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.2/src/roboswag/generate/templates/api_init.jinja` & `robotframework_openapitools-0.1.3/src/roboswag/generate/templates/api_init.jinja`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.2/src/roboswag/generate/templates/paths.jinja` & `robotframework_openapitools-0.1.3/src/roboswag/generate/templates/paths.jinja`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.2/src/roboswag/logger.py` & `robotframework_openapitools-0.1.3/src/roboswag/logger.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.2/src/roboswag/validate/schema.py` & `robotframework_openapitools-0.1.3/src/roboswag/validate/schema.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.2/src/roboswag/validate/text_response.py` & `robotframework_openapitools-0.1.3/src/roboswag/validate/text_response.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.2/PKG-INFO` & `robotframework_openapitools-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-openapitools
-Version: 0.1.2
+Version: 0.1.3
 Summary: A set of Robot Framework libraries to test APIs for which the OAS is available.
 Home-page: https://github.com/MarketSquare/robotframework-openapitools
 License: Apache-2.0
 Author: Bartlomiej Hirsz
 Author-email: bartek.hirsz@gmail.com
 Maintainer: Robin Mackaij
 Maintainer-email: r.a.mackaij@gmail.com
```

