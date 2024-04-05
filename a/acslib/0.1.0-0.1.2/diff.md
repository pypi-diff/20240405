# Comparing `tmp/acslib-0.1.0.tar.gz` & `tmp/acslib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acslib-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "acslib-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `acslib-0.1.0.tar` & `acslib-0.1.2.tar`

### file list

```diff
@@ -1,47 +1,50 @@
--rw-r--r--   0        0        0      163 2023-10-24 15:48:19.427776 acslib-0.1.0/.coveragerc
--rw-r--r--   0        0        0      104 2023-10-24 15:48:19.423776 acslib-0.1.0/.dockerignore
--rw-r--r--   0        0        0      292 2023-10-24 15:48:19.431776 acslib-0.1.0/.editorconfig
--rw-r--r--   0        0        0     5737 2023-10-24 15:48:19.443776 acslib-0.1.0/.github/workflows/dev.yml
--rw-r--r--   0        0        0     3216 2023-10-24 15:48:19.443776 acslib-0.1.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1352 2023-10-24 15:48:19.435776 acslib-0.1.0/.gitignore
--rw-r--r--   0        0        0       81 2023-10-24 15:48:19.439777 acslib-0.1.0/.isort.cfg
--rw-r--r--   0        0        0      875 2023-10-24 15:48:19.423776 acslib-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      118 2023-10-24 15:48:19.411776 acslib-0.1.0/AUTHORS.md
--rw-r--r--   0        0        0      212 2023-10-24 15:57:17.064897 acslib-0.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      473 2023-10-24 15:48:19.423776 acslib-0.1.0/Dockerfile
--rw-r--r--   0        0        0       59 2023-10-24 15:48:19.431776 acslib-0.1.0/HISTORY.md
--rw-r--r--   0        0        0     1089 2023-10-24 15:57:17.060897 acslib-0.1.0/LICENSE
--rw-r--r--   0        0        0      589 2023-10-24 15:48:19.443776 acslib-0.1.0/Makefile
--rw-r--r--   0        0        0      704 2024-01-11 18:55:00.490990 acslib-0.1.0/README.md
--rw-r--r--   0        0        0      188 2024-01-11 18:55:00.490990 acslib-0.1.0/acslib/__init__.py
--rw-r--r--   0        0        0      218 2024-01-11 18:55:00.490990 acslib-0.1.0/acslib/base/__init__.py
--rw-r--r--   0        0        0      266 2024-01-11 18:55:00.490990 acslib-0.1.0/acslib/base/acs.py
--rw-r--r--   0        0        0      173 2024-01-11 18:55:00.490990 acslib-0.1.0/acslib/base/config.py
--rw-r--r--   0        0        0     7749 2024-01-11 18:55:00.490990 acslib-0.1.0/acslib/base/connection.py
--rw-r--r--   0        0        0      277 2024-01-11 18:55:00.490990 acslib-0.1.0/acslib/base/search.py
--rw-r--r--   0        0        0     6113 2024-01-11 18:55:00.490990 acslib-0.1.0/acslib/base/status.py
--rw-r--r--   0        0        0     4201 2024-01-11 18:55:00.490990 acslib-0.1.0/acslib/ccure/__init__.py
--rw-r--r--   0        0        0     9029 2024-01-11 18:55:00.490990 acslib-0.1.0/acslib/ccure/base.py
--rw-r--r--   0        0        0     2916 2024-01-11 18:55:00.490990 acslib-0.1.0/acslib/ccure/config.py
--rw-r--r--   0        0        0     1260 2024-01-11 18:55:00.490990 acslib-0.1.0/acslib/ccure/endpoints.py
--rw-r--r--   0        0        0     4431 2024-01-11 18:55:00.490990 acslib-0.1.0/acslib/ccure/search.py
--rw-r--r--   0        0        0       36 2024-01-11 18:55:00.490990 acslib-0.1.0/acslib/ccure/tests/__init__.py
--rw-r--r--   0        0        0     1839 2024-01-11 18:55:00.490990 acslib-0.1.0/acslib/ccure/tests/conftest.py
--rw-r--r--   0        0        0     1820 2024-01-11 18:55:00.490990 acslib-0.1.0/acslib/ccure/tests/test_base.py
--rw-r--r--   0        0        0     2800 2024-01-11 18:55:00.490990 acslib-0.1.0/acslib/ccure/tests/test_config.py
--rw-r--r--   0        0        0     2111 2024-01-11 18:55:00.490990 acslib-0.1.0/acslib/ccure/tests/test_connection.py
--rw-r--r--   0        0        0     2105 2024-01-11 18:55:00.490990 acslib-0.1.0/acslib/ccure/tests/test_search.py
--rw-r--r--   0        0        0       11 2023-10-24 15:48:19.451777 acslib-0.1.0/docs/api.md
--rw-r--r--   0        0        0       41 2023-10-24 15:48:19.451777 acslib-0.1.0/docs/authors.md
--rw-r--r--   0        0        0       46 2023-10-24 15:48:19.447776 acslib-0.1.0/docs/contributing.md
--rw-r--r--   0        0        0       41 2023-10-24 15:48:19.455777 acslib-0.1.0/docs/history.md
--rw-r--r--   0        0        0       42 2023-10-24 15:48:19.447776 acslib-0.1.0/docs/index.md
--rw-r--r--   0        0        0     1188 2023-10-24 15:48:19.455777 acslib-0.1.0/docs/installation.md
--rw-r--r--   0        0        0       87 2023-10-24 15:48:19.451777 acslib-0.1.0/docs/usage.md
--rw-r--r--   0        0        0       20 2023-10-24 15:48:19.431776 acslib-0.1.0/envrc_sample
--rw-r--r--   0        0        0     1949 2023-10-24 15:48:19.419776 acslib-0.1.0/mkdocs.yml
--rw-r--r--   0        0        0     2589 2024-01-11 18:55:00.490990 acslib-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      219 2024-01-11 18:55:00.490990 acslib-0.1.0/pytest.ini
--rw-r--r--   0        0        0      926 2024-01-11 18:55:00.494990 acslib-0.1.0/requirements/base/base.txt
--rw-r--r--   0        0        0     4618 2024-01-11 18:55:00.494990 acslib-0.1.0/requirements/dev/dev.txt
--rw-r--r--   0        0        0     2223 1970-01-01 00:00:00.000000 acslib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      163 2024-04-04 21:08:04.029199 acslib-0.1.2/.coveragerc
+-rw-r--r--   0        0        0      104 2024-04-04 21:08:04.029199 acslib-0.1.2/.dockerignore
+-rw-r--r--   0        0        0      292 2024-04-04 21:08:04.029199 acslib-0.1.2/.editorconfig
+-rw-r--r--   0        0        0      296 2024-04-04 21:08:04.029199 acslib-0.1.2/.github/pr_template.md
+-rw-r--r--   0        0        0     9176 2024-04-04 21:08:04.029199 acslib-0.1.2/.github/workflows/test_publish_release..yml
+-rw-r--r--   0        0        0     1388 2024-04-04 21:08:04.029199 acslib-0.1.2/.gitignore
+-rw-r--r--   0        0        0       81 2024-04-04 21:08:04.029199 acslib-0.1.2/.isort.cfg
+-rw-r--r--   0        0        0      875 2024-04-04 21:08:04.029199 acslib-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      118 2024-04-04 21:08:04.029199 acslib-0.1.2/AUTHORS.md
+-rw-r--r--   0        0        0      212 2024-04-04 21:08:04.029199 acslib-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      473 2024-04-04 21:08:04.029199 acslib-0.1.2/Dockerfile
+-rw-r--r--   0        0        0       59 2024-04-04 21:08:04.029199 acslib-0.1.2/HISTORY.md
+-rw-r--r--   0        0        0     1089 2024-04-04 21:08:04.029199 acslib-0.1.2/LICENSE
+-rw-r--r--   0        0        0      589 2024-04-04 21:08:04.029199 acslib-0.1.2/Makefile
+-rw-r--r--   0        0        0     2468 2024-04-04 21:08:04.029199 acslib-0.1.2/README.md
+-rw-r--r--   0        0        0      148 2024-04-04 21:08:04.029199 acslib-0.1.2/acslib/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 21:08:04.029199 acslib-0.1.2/acslib/base/__init__.py
+-rw-r--r--   0        0        0      270 2024-04-04 21:08:04.029199 acslib-0.1.2/acslib/base/acs.py
+-rw-r--r--   0        0        0      172 2024-04-04 21:08:04.029199 acslib-0.1.2/acslib/base/config.py
+-rw-r--r--   0        0        0     6294 2024-04-04 21:08:04.029199 acslib-0.1.2/acslib/base/connection.py
+-rw-r--r--   0        0        0      272 2024-04-04 21:08:04.029199 acslib-0.1.2/acslib/base/search.py
+-rw-r--r--   0        0        0     6113 2024-04-04 21:08:04.029199 acslib-0.1.2/acslib/base/status.py
+-rw-r--r--   0        0        0        0 2024-04-04 21:08:04.029199 acslib-0.1.2/acslib/ccure/__init__.py
+-rw-r--r--   0        0        0      599 2024-04-04 21:08:04.029199 acslib-0.1.2/acslib/ccure/base.py
+-rw-r--r--   0        0        0     2923 2024-04-04 21:08:04.029199 acslib-0.1.2/acslib/ccure/config.py
+-rw-r--r--   0        0        0     7308 2024-04-04 21:08:04.029199 acslib-0.1.2/acslib/ccure/connection.py
+-rw-r--r--   0        0        0     8957 2024-04-04 21:08:04.029199 acslib-0.1.2/acslib/ccure/crud.py
+-rw-r--r--   0        0        0      956 2024-04-04 21:08:04.029199 acslib-0.1.2/acslib/ccure/endpoints.py
+-rw-r--r--   0        0        0     6302 2024-04-04 21:08:04.029199 acslib-0.1.2/acslib/ccure/search.py
+-rw-r--r--   0        0        0       36 2024-04-04 21:08:04.029199 acslib-0.1.2/acslib/ccure/tests/__init__.py
+-rw-r--r--   0        0        0     1845 2024-04-04 21:08:04.029199 acslib-0.1.2/acslib/ccure/tests/conftest.py
+-rw-r--r--   0        0        0     2036 2024-04-04 21:08:04.029199 acslib-0.1.2/acslib/ccure/tests/test_base.py
+-rw-r--r--   0        0        0     2808 2024-04-04 21:08:04.029199 acslib-0.1.2/acslib/ccure/tests/test_config.py
+-rw-r--r--   0        0        0     2122 2024-04-04 21:08:04.029199 acslib-0.1.2/acslib/ccure/tests/test_connection.py
+-rw-r--r--   0        0        0     2587 2024-04-04 21:08:04.029199 acslib-0.1.2/acslib/ccure/tests/test_search.py
+-rw-r--r--   0        0        0      576 2024-04-04 21:08:04.029199 acslib-0.1.2/acslib/ccure/types.py
+-rw-r--r--   0        0        0       11 2024-04-04 21:08:04.029199 acslib-0.1.2/docs/api.md
+-rw-r--r--   0        0        0       41 2024-04-04 21:08:04.029199 acslib-0.1.2/docs/authors.md
+-rw-r--r--   0        0        0       46 2024-04-04 21:08:04.029199 acslib-0.1.2/docs/contributing.md
+-rw-r--r--   0        0        0       41 2024-04-04 21:08:04.029199 acslib-0.1.2/docs/history.md
+-rw-r--r--   0        0        0       42 2024-04-04 21:08:04.029199 acslib-0.1.2/docs/index.md
+-rw-r--r--   0        0        0     1188 2024-04-04 21:08:04.029199 acslib-0.1.2/docs/installation.md
+-rw-r--r--   0        0        0       87 2024-04-04 21:08:04.029199 acslib-0.1.2/docs/usage.md
+-rw-r--r--   0        0        0       20 2024-04-04 21:08:04.029199 acslib-0.1.2/envrc_sample
+-rw-r--r--   0        0        0     1949 2024-04-04 21:08:04.033199 acslib-0.1.2/mkdocs.yml
+-rw-r--r--   0        0        0     2652 2024-04-04 21:08:04.033199 acslib-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      219 2024-04-04 21:08:04.033199 acslib-0.1.2/pytest.ini
+-rw-r--r--   0        0        0      926 2024-04-04 21:08:04.033199 acslib-0.1.2/requirements/base/base.txt
+-rw-r--r--   0        0        0     4618 2024-04-04 21:08:04.033199 acslib-0.1.2/requirements/dev/dev.txt
+-rw-r--r--   0        0        0     4020 1970-01-01 00:00:00.000000 acslib-0.1.2/PKG-INFO
```

### Comparing `acslib-0.1.0/.gitignore` & `acslib-0.1.2/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -97,9 +97,11 @@
 .idea/
 .envrc
 
 # mkdocs
 site/
 .history/
 
+# repo pulled in for CI/CD
+actions/
 
 Access Control Systems
```

### Comparing `acslib-0.1.0/.pre-commit-config.yaml` & `acslib-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `acslib-0.1.0/LICENSE` & `acslib-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `acslib-0.1.0/Makefile` & `acslib-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `acslib-0.1.0/acslib/base/connection.py` & `acslib-0.1.2/acslib/base/connection.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import json
 from abc import ABC, abstractmethod
 from enum import Enum
 from typing import Any, Optional
 
 import requests
-from pydantic import BaseModel, Field
+from pydantic import BaseModel
 
 from acslib.base import status
 
 
 class ACSConnectionException(Exception):
     pass
 
@@ -49,17 +48,21 @@
         return len(self.json)
 
 
 class ACSRequestData(BaseModel):
     """Kwargs used in requests get/post/etc methods"""
 
     url: str
-    headers: Optional[dict] = None
-    data: Optional[dict] = None
+    # query params:
+    params: Optional[dict] = None
+    # body x-www-form-urlencoded data:
+    data: Optional[dict | str] = None
+    # body raw json:
     request_json: Optional[dict] = None
+    headers: Optional[dict] = None
 
 
 class ACSConnection(ABC):
     REQUEST_TYPE = {
         ACSRequestMethod.GET: requests.get,
         ACSRequestMethod.POST: requests.post,
         ACSRequestMethod.PUT: requests.put,
@@ -76,55 +79,14 @@
     def login(self):
         pass
 
     @abstractmethod
     def logout(self):
         pass
 
-    @staticmethod
-    def _encode_data(data: dict) -> str:
-        """
-        Encode a dictionary of form data as a string for requests
-
-        Parameters:
-            data: form data for the request
-
-        Returns: the string of encoded data
-        """
-
-        def get_form_entries(data: dict, prefix: str = "") -> list[str]:
-            """
-            Convert the data dict into a list of form entries
-
-            Parameters:
-                data: data about the new clearance assignment
-
-            Returns: list of strings representing key/value pairs
-            """
-            entries = []
-            for key, val in data.items():
-                if isinstance(val, (int, str)):
-                    if prefix:
-                        entries.append(f"{prefix}[{key}]={val}")
-                    else:
-                        entries.append(f"{key}={val}")
-                elif isinstance(val, list):
-                    for i, list_item in enumerate(val):
-                        if isinstance(list_item, dict):
-                            entries.extend(
-                                get_form_entries(data=list_item, prefix=prefix + f"{key}[{i}]")
-                            )
-                        elif prefix:
-                            entries.append(f"{prefix}[{key}][]={list_item}")
-                        else:
-                            entries.append(f"{key}[]={list_item}")
-            return entries
-
-        return "&".join(get_form_entries(data))
-
     def _make_request(self, requests_method: ACSRequestMethod, request_data_map: dict):
         if req := self.REQUEST_TYPE.get(requests_method):
             return req(**request_data_map, timeout=self.timeout)
         raise ACSConnectionException(f"Invalid request method: {requests_method}")
 
     def request(
         self, requests_method: ACSRequestMethod, request_data: ACSRequestData
@@ -133,24 +95,23 @@
         Process requests to remote servers.
         Either return a response with the resulting status code, json data, and headers,
         or raise an exception with the appropriate status code
 
         Parameters:
             requests_method: A method from the requests module. requests.get, requests.post, etc
             request_data: Data used as kwargs for the requests_method
-            timeout: Maximum time to wait for a server response, in seconds
 
         Returns: An object with status_code, json, and headers attributes
         """
 
         try:
-            # remove request_data_map properties with None values
-            request_data_map = dict(request_data)
+            request_data_map = request_data.model_dump()
             request_data_map["json"] = request_data_map.pop("request_json", None)
             request_data_map["data"] = request_data_map.get("data", {})
+            # remove request_data_map properties with None values
             request_data_map = {k: v for k, v in request_data_map.items() if v is not None}
             response = self._make_request(requests_method, request_data_map)
         except requests.HTTPError:
             # An HTTP error occurred.
             raise ACSRequestException(
                 status_code=status.HTTP_400_BAD_REQUEST,
                 log_message="An error occurred with this request",
```

### Comparing `acslib-0.1.0/acslib/base/status.py` & `acslib-0.1.2/acslib/base/status.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.0/acslib/ccure/base.py` & `acslib-0.1.2/acslib/ccure/connection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 import logging
 from numbers import Number
-from typing import Optional
 
-from acslib.base import (
-    AccessControlSystem,
+from acslib.base import status
+from acslib.base.connection import (
     ACSConnection,
     ACSRequestData,
     ACSRequestException,
+    ACSRequestMethod,
     ACSRequestResponse,
-    status,
 )
-from acslib.base.connection import ACSRequestMethod
-from acslib.base.search import ACSFilter
 from acslib.ccure.config import CcureConfigFactory
-from acslib.ccure.search import PersonnelFilter, ClearanceFilter, SearchTypes, FUZZ
-
-logger = logging.getLogger(__name__)
 
 
 class CcureConnection(ACSConnection):
     def __init__(self, **kwargs):
         """
         A connection object to the CCure Server.
         Parameters:
         :param kwargs:
         """
         self.session_id = None
         if con_logger := kwargs.get("logger"):
             self.logger = con_logger
         else:
-            self.logger = logger
+            self.logger = logging.getLogger(__name__)
+
         if not kwargs.get("config"):
             kwargs["config"] = CcureConfigFactory()
         self.logger.info("Initializing CCure connection")
         super().__init__(**kwargs)
 
     @property
-    def headers(self):
+    def base_headers(self):
         """."""
         return {
             "session-id": self.get_session_id(),
             "Access-Control-Expose-Headers": "session-id",
         }
 
+    @property
+    def header_for_form_data(self):
+        return {"Content-Type": "application/x-www-form-urlencoded"}
+
     def login(self):
         """."""
         try:
             response = self.request(
                 ACSRequestMethod.POST,
                 request_data=ACSRequestData(
                     url=self.config.base_url + self.config.endpoints.LOGIN,
@@ -152,90 +151,47 @@
                 request_data=ACSRequestData(url=version_url),
             ).json
             self.logger.debug(f"CCure webservice version: {response.get('webServiceVersion')}")
             self.logger.debug(f"CCure app server version: {response.get('appServerVersion')}")
         except ACSRequestException as e:
             self.logger.debug(f"Could not get CCure api version number: {e}")
 
+    @staticmethod
+    def encode_data(data: dict) -> str:
+        """
+        Encode a dictionary of form data as a string for requests
 
-class CcureACS(AccessControlSystem):
-    """."""
-
-    def __init__(self, connection: Optional[CcureConnection] = None):
-        """."""
-        super().__init__(connection=connection)
-        if not self.connection:
-            self.connection = CcureConnection()
-        self.logger = self.connection.logger
-        self.request_options = {}
-        self.search_filter = None
-
-    @property
-    def config(self):
-        """."""
-        return self.connection.config
-
-    def _search_people(self, terms: list, search_filter: Optional[ACSFilter] = None) -> ACSRequestResponse:
-        if not search_filter:
-            search_filter = PersonnelFilter()
-        request_json = {
-            "TypeFullName": "Personnel",
-            "DisplayProperties": search_filter.display_properties,
-            "pageSize": self.connection.config.page_size,
-            "pageNumber": 1,
-            "WhereClause": search_filter.filter(terms),
-        }
-        if not search_filter.display_properties:
-            del request_json["DisplayProperties"]
-
-        return self.connection.request(
-            ACSRequestMethod.POST,
-            request_data=ACSRequestData(
-                url=self.connection.config.base_url
-                + self.connection.config.endpoints.FIND_OBJS_W_CRITERIA,
-                request_json=request_json,
-                headers=self.connection.headers,
-            ),
-        )
-
-    def _search_clearances(self, terms: list, search_filter: Optional[ACSFilter] = None) -> ACSRequestResponse:
-        if not search_filter:
-            search_filter = ClearanceFilter()
-        request_json = {
-            "partitionList": [],
-            "propertyList": search_filter.display_properties,
-            "pageSize": self.connection.config.page_size,
-            "pageNumber": 1,
-            "whereClause": search_filter.filter(terms),
-            "sortColumnName": "",
-            "whereArgList": [],
-            "explicitPropertyList": [],
-        }
-        if not search_filter.display_properties:
-            del request_json["DisplayProperties"]
+        Parameters:
+            data: form data for the request
 
-        response = self.connection.request(
-            ACSRequestMethod.POST,
-            request_data=ACSRequestData(
-                url=self.connection.config.base_url
-                + self.connection.config.endpoints.CLEARANCES_FOR_ASSIGNMENT,
-                request_json=request_json,
-                headers=self.connection.headers,
-            ),
-        )
-        if response.json:
-            response.json = response.json[1:]
+        Returns: the string of encoded data
+        """
 
-        return response
+        def get_form_entries(data: dict, prefix: str = "") -> list[str]:
+            """
+            Convert the data dict into a list of form entries
+
+            Parameters:
+                data: data about the new clearance assignment
+
+            Returns: list of strings representing key/value pairs
+            """
+            entries = []
+            for key, val in data.items():
+                if isinstance(val, (int, str)):
+                    if prefix:
+                        entries.append(f"{prefix}[{key}]={val}")
+                    else:
+                        entries.append(f"{key}={val}")
+                elif isinstance(val, list):
+                    for i, list_item in enumerate(val):
+                        if isinstance(list_item, dict):
+                            entries.extend(
+                                get_form_entries(data=list_item, prefix=prefix + f"{key}[{i}]")
+                            )
+                        elif prefix:
+                            entries.append(f"{prefix}[{key}][]={list_item}")
+                        else:
+                            entries.append(f"{key}[]={list_item}")
+            return entries
 
-    def search(
-        self, search_type: SearchTypes, terms: list, search_filter: Optional[ACSFilter] = None
-    ) -> ACSRequestResponse:
-        match search_type:
-            case SearchTypes.PERSONNEL.value:
-                self.logger.info("Searching for personnel")
-                return self._search_people(terms, search_filter)
-            case SearchTypes.CLEARANCE.value:
-                self.logger.info("Searching for clearances")
-                return self._search_clearances(terms, search_filter)
-            case _:
-                raise ValueError(f"Invalid search type: {search_type}")
+        return "&".join(get_form_entries(data))
```

### Comparing `acslib-0.1.0/acslib/ccure/config.py` & `acslib-0.1.2/acslib/ccure/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-from acslib.base import ACSConfig, ACSConfigException
+from acslib.base.config import ACSConfig, ACSConfigException
 from acslib.ccure.endpoints import V2Endpoints
 
 
 class CcureConfig(ACSConfig):
     """
     CcureConfig returns an object that implements the ACSConfig interface.
     It expects the following variables to be set either in the environment or passed as kwargs:
```

### Comparing `acslib-0.1.0/acslib/ccure/search.py` & `acslib-0.1.2/acslib/ccure/search.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from enum import Enum
+from typing import Optional
 
 from acslib.base.search import ACSFilter, BooleanOperators, TermOperators
 
 
 def left_fuzz(term):
     return f"%{term}"
 
@@ -22,107 +23,150 @@
 LFUZZ = left_fuzz
 RFUZZ = right_fuzz
 FUZZ = full_fuzz
 NFUZZ = no_fuzz
 
 PERSONNEL_LOOKUP_FIELDS = {"FirstName": FUZZ, "LastName": FUZZ}
 CLEARANCE_LOOKUP_FIELDS = {"Name": FUZZ}
+CREDENTIAL_LOOKUP_FIELDS = {"Name": FUZZ}
 
 
 class SearchTypes(Enum):
     PERSONNEL = "personnel"
     CLEARANCE = "clearance"
+    CREDENTIAL = "credential"
 
 
 class BaseCcureFilter(ACSFilter):
     """Base CCure Filter
-    :param lookups: List of tuples containing the field name and the lookup function
+    :param lookups: Dict containing searchable field names and their lookup functions
     :param outer_bool: Boolean operator to use between search terms
     :param inner_bool: Boolean operator to use between lookups
     :param term_operator: Term operator to use between field and a search term
     :attribute
     """
 
     def __init__(
         self,
-        lookups: list[tuple[str, callable]] = None,
+        lookups: dict[str, callable] = None,
         outer_bool=BooleanOperators.AND,
         inner_bool=BooleanOperators.OR,
         term_operator=TermOperators.FUZZY,
     ):
         self.filter_fields = lookups
         self.outer_bool = outer_bool.value
         self.inner_bool = inner_bool.value
         self.term_operator = term_operator.value
         #: List of properties from CCURE to be included in the CCURE response
-        self.display_properties = ["FirstName", "MiddleName", "LastName", "ObjectID"]
+        self.display_properties = []
 
-    def _compile_term(self, term: str) -> str:
+    def _compile_term(self, term) -> str:
         """Get all parts of the query for one search term"""
         fields = [(field_name, lookup(term)) for field_name, lookup in self.filter_fields.items()]
-        field_queries = [f"{field_name} {self.term_operator} '{lookup}'" for field_name, lookup in fields]
+        field_queries = [
+            f"{field_name} {self.term_operator} '{lookup}'" for field_name, lookup in fields
+        ]
         return f"({self.inner_bool.join(field_queries)})"
 
     def update_display_properties(self, properties: list[str]):
         if not isinstance(properties, list):
             raise TypeError("Properties must be a list of strings")
         self.display_properties += properties
 
     def filter(self, search):
         pass
 
 
 class PersonnelFilter(BaseCcureFilter):
     """Basic CCure Personnel Filter
-    :param lookups: List of tuples containing the field name and the lookup function
+    :param lookups: Dict containing searchable field names and their lookup functions
     :param outer_bool: Boolean operator to use between search terms
     :param inner_bool: Boolean operator to use between lookups
     :param term_operator: Term operator to use between field and a search term
+    :param display_properties: List of properties from CCure to be included in the CCure response
     :attribute
     """
 
     def __init__(
         self,
-        lookups: dict[str, callable] = [],
+        lookups: Optional[dict[str, callable]] = None,
         outer_bool=BooleanOperators.AND,
         inner_bool=BooleanOperators.OR,
         term_operator=TermOperators.FUZZY,
+        display_properties: Optional[list[str]] = None,
     ):
-        self.filter_fields = lookups if lookups else PERSONNEL_LOOKUP_FIELDS
+        self.filter_fields = lookups or PERSONNEL_LOOKUP_FIELDS
         self.outer_bool = f" {outer_bool.value} "
         self.inner_bool = f" {inner_bool.value} "
         self.term_operator = term_operator.value
-        self.display_properties = ["FirstName", "MiddleName", "LastName"]
+        self.display_properties = ["FirstName", "MiddleName", "LastName", "ObjectID"]
+        if display_properties is not None:
+            self.display_properties = display_properties
 
     def filter(self, search: list[str]) -> str:
         if not isinstance(search, list):
             raise TypeError("Search must be a list of strings")
         return self.outer_bool.join(self._compile_term(term) for term in search)
 
 
 class ClearanceFilter(BaseCcureFilter):
     """Basic CCure Clearance Filter
-    :param lookups: List of tuples containing the field name and the lookup function
+    :param lookups: Dict containing searchable field names and their lookup functions
     :param outer_bool: Boolean operator to use between search terms
     :param inner_bool: Boolean operator to use between lookups
     :param term_operator: Term operator to use between field and a search term
+    :param display_properties: List of properties from CCure to be included in the CCure response
     :attribute
     """
 
     def __init__(
         self,
-        lookups: dict[str, callable] = [],
+        lookups: Optional[dict[str, callable]] = None,
         outer_bool=BooleanOperators.AND,
         inner_bool=BooleanOperators.OR,
         term_operator=TermOperators.FUZZY,
+        display_properties: Optional[list[str]] = None,
     ):
-        self.filter_fields = lookups if lookups else CLEARANCE_LOOKUP_FIELDS
+        self.filter_fields = lookups or CLEARANCE_LOOKUP_FIELDS
         self.outer_bool = f" {outer_bool.value} "
         self.inner_bool = f" {inner_bool.value} "
         self.term_operator = term_operator.value
-        # List of properties from CCURE to be included in the CCURE response
         self.display_properties = ["Name"]
+        if display_properties is not None:
+            self.display_properties = display_properties
 
     def filter(self, search: list[str]) -> str:
         if not isinstance(search, list):
             raise TypeError("Search must be a list of strings")
         return self.outer_bool.join(self._compile_term(term) for term in search)
+
+
+class CredentialFilter(BaseCcureFilter):
+    """Basic CCure Credential Filter
+    :param lookups: Dict containing searchable field names and their lookup functions
+    :param outer_bool: Boolean operator to use between search terms
+    :param inner_bool: Boolean operator to use between lookups
+    :param term_operator: Term operator to use between field and a search term
+    :param display_properties: List of properties from CCure to be included in the CCure response
+    :attribute
+    """
+
+    def __init__(
+        self,
+        lookups: Optional[dict[str, callable]] = None,
+        outer_bool=BooleanOperators.AND,
+        inner_bool=BooleanOperators.OR,
+        term_operator=TermOperators.FUZZY,
+        display_properties: Optional[list[str]] = None,
+    ):
+        self.filter_fields = lookups or CREDENTIAL_LOOKUP_FIELDS
+        self.outer_bool = f" {outer_bool.value} "
+        self.inner_bool = f" {inner_bool.value} "
+        self.term_operator = term_operator.value
+        self.display_properties = ["Name"]
+        if display_properties is not None:
+            self.display_properties = display_properties
+
+    def filter(self, search: list) -> str:
+        if not isinstance(search, list):
+            raise TypeError("`search` must be a list of search terms")
+        return self.outer_bool.join(self._compile_term(term) for term in search)
```

### Comparing `acslib-0.1.0/acslib/ccure/tests/conftest.py` & `acslib-0.1.2/acslib/ccure/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import random
 from dataclasses import dataclass, field
 
 import pytest
 from faker import Faker
 
-from acslib.ccure.base import CcureConnection
 from acslib.ccure.config import CcureConfigFactory
+from acslib.ccure.connection import CcureConnection
 
 fake = Faker()
 
 BASE_CONFIG = {
     "CCURE_USERNAME": "test",
     "CCURE_PASSWORD": "test",
     "CCURE_BASE_URL": "https://example.com/ccure",
```

### Comparing `acslib-0.1.0/acslib/ccure/tests/test_base.py` & `acslib-0.1.2/acslib/ccure/tests/test_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,49 +7,52 @@
 from acslib.ccure.search import PersonnelFilter, SearchTypes
 
 
 def test_default_ccure_acs(env_config, caplog):
     """Default picks up env vars."""
     ccure = CcureACS()
     assert ccure.config.base_url == "https://example.com/ccure"
-    assert ccure.logger.name == "acslib.ccure.base"
-    assert "acslib.ccure.base" in caplog.text
+    assert ccure.logger.name == "acslib.ccure.connection"
+    assert "acslib.ccure.connection" in caplog.text
 
 
 def test_user_supplied_logger(env_config, caplog):
     """."""
     import logging
 
     cc_conn = CcureConnection(logger=logging.getLogger("test"))
     ccure = CcureACS(connection=cc_conn)
     assert ccure.logger.name == "test"
-    assert "test:base" in caplog.text
+    assert "test:connection" in caplog.text
 
 
+@pytest.mark.skip(reason="ccure search no longer works this way")
 def test_default_ccure_search(env_config, personnel_response, caplog):
     ccure = CcureACS()
     with patch(
         "acslib.ccure.base.CcureACS._search_people", return_value=personnel_response
     ) as mock_search:
         ccure.search(search_type=SearchTypes.PERSONNEL, terms=["test"])
         mock_search.assert_called_with(["test"])
     assert "Searching for personnel" in caplog.text
 
 
+@pytest.mark.skip(reason="ccure search no longer works this way")
 def test_ccure_search_with_filter(env_config, personnel_response, caplog):
     ccure = CcureACS()
     filter = PersonnelFilter()
     with patch(
         "acslib.ccure.base.CcureACS._search_people", return_value=personnel_response
     ) as mock_search:
         ccure.search(search_type=SearchTypes.PERSONNEL, terms=["test"], search_filter=filter)
         mock_search.assert_called_with(["test"], filter)
     assert "Searching for personnel" in caplog.text
 
 
+@pytest.mark.skip(reason="ccure search no longer works this way")
 def test_invalid_search_type(env_config):
     class NewTypes(Enum):
         NEW = "new"
         PERSONNEL = "personnel"
 
     ccure = CcureACS()
     with pytest.raises(ValueError):
```

### Comparing `acslib-0.1.0/acslib/ccure/tests/test_config.py` & `acslib-0.1.2/acslib/ccure/tests/test_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
+
 import pytest
 
-from acslib.base import ACSConfigException
+from acslib.base.config import ACSConfigException
 from acslib.ccure.config import CcureConfigFactory
 
 
 def test_ccure_config_with_kwargs(config):
     """."""
     assert config.base_url == "https://example.com/ccure"
     assert config.connection_data == {
```

### Comparing `acslib-0.1.0/acslib/ccure/tests/test_connection.py` & `acslib-0.1.2/acslib/ccure/tests/test_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from unittest.mock import patch
 
 import pytest
 import requests
 
-from acslib.base import ACSRequestException
+from acslib.base.connection import ACSRequestException
 
 
 def test_ccure_connection(ccure_connection, response_w_session):
     """."""
     with patch(
         "acslib.base.connection.ACSConnection._make_request", return_value=response_w_session
     ):
```

### Comparing `acslib-0.1.0/acslib/ccure/tests/test_search.py` & `acslib-0.1.2/acslib/ccure/tests/test_search.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,53 @@
 import pytest
 
 from acslib.base.search import BooleanOperators, TermOperators
 from acslib.ccure.search import (
+    CLEARANCE_LOOKUP_FIELDS,
     FUZZ,
     LFUZZ,
     NFUZZ,
     PERSONNEL_LOOKUP_FIELDS,
     RFUZZ,
+    ClearanceFilter,
     PersonnelFilter,
 )
 
 
 def test_default_instance():
-    filter = PersonnelFilter()
-    assert filter.filter_fields == PERSONNEL_LOOKUP_FIELDS
-    assert filter.outer_bool == "AND"
-    assert filter.inner_bool == "OR"
-    assert filter.term_operator == "LIKE"
-    assert filter.display_properties == ["FirstName", "MiddleName", "LastName"]
+    personnel_filter = PersonnelFilter()
+    assert personnel_filter.filter_fields == PERSONNEL_LOOKUP_FIELDS
+    assert personnel_filter.outer_bool == " AND "
+    assert personnel_filter.inner_bool == " OR "
+    assert personnel_filter.term_operator == "LIKE"
+    assert personnel_filter.display_properties == [
+        "FirstName",
+        "MiddleName",
+        "LastName",
+        "ObjectID",
+    ]
+
+    clearance_filter = ClearanceFilter()
+    assert clearance_filter.filter_fields == CLEARANCE_LOOKUP_FIELDS
+    assert clearance_filter.outer_bool == " AND "
+    assert clearance_filter.inner_bool == " OR "
+    assert clearance_filter.term_operator == "LIKE"
+    assert clearance_filter.display_properties == ["Name"]
 
 
 def test_custom_instance():
     filter = PersonnelFilter(
-        lookups=[("Text1", NFUZZ), ("Tex14", NFUZZ)],
+        lookups={"Text1": NFUZZ, "Tex14": NFUZZ},
         outer_bool=BooleanOperators.OR,
         inner_bool=BooleanOperators.AND,
         term_operator=TermOperators.EQUALS,
     )
-    assert filter.filter_fields == [("Text1", NFUZZ), ("Tex14", NFUZZ)]
-    assert filter.outer_bool == "OR"
-    assert filter.inner_bool == "AND"
+    assert filter.filter_fields == {"Text1": NFUZZ, "Tex14": NFUZZ}
+    assert filter.outer_bool == " OR "
+    assert filter.inner_bool == " AND "
     assert filter.term_operator == "="
 
 
 def test_single_search_term():
     filter = PersonnelFilter()
     search = filter.filter(["test"])
     assert search == "(FirstName LIKE '%test%' OR LastName LIKE '%test%')"
@@ -53,15 +67,15 @@
         == "(FirstName LIKE '%test%' OR LastName LIKE '%test%') AND (FirstName LIKE '%test2%' OR LastName LIKE '%test2%')"
     )
 
 
 def test_update_display_properties():
     filter = PersonnelFilter()
     filter.update_display_properties(["EmailAddress"])
-    assert len(filter.display_properties) == 4
+    assert len(filter.display_properties) == 5
     assert "EmailAddress" in filter.display_properties
 
 
 def test_update_display_properties_not_list():
     filter = PersonnelFilter()
     with pytest.raises(TypeError):
         filter.update_display_properties("EmailAddress")
```

### Comparing `acslib-0.1.0/docs/installation.md` & `acslib-0.1.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `acslib-0.1.0/mkdocs.yml` & `acslib-0.1.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `acslib-0.1.0/pyproject.toml` & `acslib-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [build-system]
 requires = ["flit_core>=3.2, <4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "acslib"
-version = "0.1.0"
+version = "0.1.2"
 authors = [
     { name="Jeremy Gibson", email="jmgibso3@ncsu.edu" },
+    { name="Luc Sanchez", email="lgsanche@ncsu.edu" },
 ]
 description = "A library for interacting with Access Control Systems like Genetec or Ccure9k"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.10"
 
 dependencies = [
@@ -52,15 +53,15 @@
 line-length = 100
 include = '\.pyi?$'
 
 [tool.ruff]
 # Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
 select = ["E", "F", "W", "I001"]
 src = ["acslib"]
-ignore = ["E501"]
+ignore = ["E501", "F401"]
 fix = true
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
 fixable = ["A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W", "ANN", "ARG", "BLE", "COM", "DJ", "DTZ", "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"]
 unfixable = []
```

### Comparing `acslib-0.1.0/requirements/base/base.txt` & `acslib-0.1.2/requirements/base/base.txt`

 * *Files identical despite different names*

### Comparing `acslib-0.1.0/requirements/dev/dev.txt` & `acslib-0.1.2/requirements/dev/dev.txt`

 * *Files identical despite different names*

