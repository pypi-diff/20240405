# Comparing `tmp/airbyte_source_salesforce-2.4.1.dev202403282031.tar.gz` & `tmp/airbyte_source_salesforce-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_salesforce-2.4.1.dev202403282031.tar", max compression
+gzip compressed data, was "airbyte_source_salesforce-2.4.2.tar", max compression
```

## Comparing `airbyte_source_salesforce-2.4.1.dev202403282031.tar` & `airbyte_source_salesforce-2.4.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     4568 2024-03-28 20:28:28.059880 airbyte_source_salesforce-2.4.1.dev202403282031/README.md
--rw-r--r--   0        0        0      842 2024-03-28 20:31:15.005513 airbyte_source_salesforce-2.4.1.dev202403282031/pyproject.toml
--rw-r--r--   0        0        0      131 2024-03-28 20:28:28.059880 airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/__init__.py
--rw-r--r--   0        0        0    16806 2024-03-28 20:28:28.059880 airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/api.py
--rw-r--r--   0        0        0     1667 2024-03-28 20:28:28.059880 airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/availability_strategy.py
--rw-r--r--   0        0        0      808 2024-03-28 20:28:28.059880 airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/exceptions.py
--rw-r--r--   0        0        0     3633 2024-03-28 20:28:28.059880 airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/rate_limiting.py
--rw-r--r--   0        0        0     1619 2024-03-28 20:28:28.059880 airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/run.py
--rw-r--r--   0        0        0     9747 2024-03-28 20:28:28.059880 airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/schemas/Describe.json
--rw-r--r--   0        0        0    14130 2024-03-28 20:28:28.059880 airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/source.py
--rw-r--r--   0        0        0     4769 2024-03-28 20:28:28.059880 airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/spec.yaml
--rw-r--r--   0        0        0    40453 2024-03-28 20:28:28.059880 airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/streams.py
--rw-r--r--   0        0        0     1024 2024-03-28 20:28:28.059880 airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/utils.py
--rw-r--r--   0        0        0     5329 1970-01-01 00:00:00.000000 airbyte_source_salesforce-2.4.1.dev202403282031/PKG-INFO
+-rw-r--r--   0        0        0     4568 2024-04-05 17:03:13.000000 airbyte_source_salesforce-2.4.2/README.md
+-rw-r--r--   0        0        0      826 2024-04-05 17:44:52.993992 airbyte_source_salesforce-2.4.2/pyproject.toml
+-rw-r--r--   0        0        0      131 2024-04-05 17:03:13.000000 airbyte_source_salesforce-2.4.2/source_salesforce/__init__.py
+-rw-r--r--   0        0        0    16870 2024-04-05 17:03:13.000000 airbyte_source_salesforce-2.4.2/source_salesforce/api.py
+-rw-r--r--   0        0        0     1667 2024-04-05 17:03:13.000000 airbyte_source_salesforce-2.4.2/source_salesforce/availability_strategy.py
+-rw-r--r--   0        0        0      808 2024-04-05 17:03:13.000000 airbyte_source_salesforce-2.4.2/source_salesforce/exceptions.py
+-rw-r--r--   0        0        0     3946 2024-04-05 17:03:13.000000 airbyte_source_salesforce-2.4.2/source_salesforce/rate_limiting.py
+-rw-r--r--   0        0        0     1619 2024-04-05 17:03:13.000000 airbyte_source_salesforce-2.4.2/source_salesforce/run.py
+-rw-r--r--   0        0        0     9747 2024-04-05 17:03:13.000000 airbyte_source_salesforce-2.4.2/source_salesforce/schemas/Describe.json
+-rw-r--r--   0        0        0    14130 2024-04-05 17:03:13.000000 airbyte_source_salesforce-2.4.2/source_salesforce/source.py
+-rw-r--r--   0        0        0     4769 2024-04-05 17:03:13.000000 airbyte_source_salesforce-2.4.2/source_salesforce/spec.yaml
+-rw-r--r--   0        0        0    41131 2024-04-05 17:03:13.000000 airbyte_source_salesforce-2.4.2/source_salesforce/streams.py
+-rw-r--r--   0        0        0     1024 2024-04-05 17:03:13.000000 airbyte_source_salesforce-2.4.2/source_salesforce/utils.py
+-rw-r--r--   0        0        0     5313 1970-01-01 00:00:00.000000 airbyte_source_salesforce-2.4.2/PKG-INFO
```

### Comparing `airbyte_source_salesforce-2.4.1.dev202403282031/README.md` & `airbyte_source_salesforce-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.1.dev202403282031/pyproject.toml` & `airbyte_source_salesforce-2.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.4.1.dev202403282031"
+version = "2.4.2"
 name = "airbyte-source-salesforce"
 description = "Source implementation for Salesforce."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
```

### Comparing `airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/api.py` & `airbyte_source_salesforce-2.4.2/source_salesforce/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import concurrent.futures
 import logging
 from typing import Any, List, Mapping, Optional, Tuple
 
+import backoff
 import requests  # type: ignore[import]
 from airbyte_cdk.models import ConfiguredAirbyteCatalog
 from airbyte_cdk.utils import AirbyteTracedException
 from airbyte_protocol.models import FailureType
 from requests import adapters as request_adapters
 from requests.exceptions import HTTPError, RequestException  # type: ignore[import]
 
@@ -296,15 +297,15 @@
                     streams_list=stream_names, search_word=stream_criteria["value"], search_criteria=stream_criteria["criteria"]
                 )
             stream_names = list(set(filtered_stream_list))
 
         validated_streams = [stream_name for stream_name in stream_names if self.filter_streams(stream_name)]
         return {stream_name: sobject_options for stream_name, sobject_options in stream_objects.items() if stream_name in validated_streams}
 
-    @default_backoff_handler(max_tries=5, factor=5)
+    @default_backoff_handler(max_tries=5, backoff_method=backoff.expo, backoff_params={"factor": 5})
     def _make_request(
         self, http_method: str, url: str, headers: dict = None, body: dict = None, stream: bool = False, params: dict = None
     ) -> requests.models.Response:
         try:
             if http_method == "GET":
                 resp = self.session.get(url, headers=headers, stream=stream, params=params)
             elif http_method == "POST":
```

### Comparing `airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/availability_strategy.py` & `airbyte_source_salesforce-2.4.2/source_salesforce/availability_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/exceptions.py` & `airbyte_source_salesforce-2.4.2/source_salesforce/exceptions.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/rate_limiting.py` & `airbyte_source_salesforce-2.4.2/source_salesforce/rate_limiting.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,50 +22,60 @@
     # Without much more information, we will make it retryable hoping that performing the same request will work.
     exceptions.ChunkedEncodingError,
     # We've had examples where the response from Salesforce was not a JSON response. Those cases where error cases though. For example:
     # https://github.com/airbytehq/airbyte-internal-issues/issues/6855. We will assume that this is an edge issue and that retry should help
     exceptions.JSONDecodeError,
 )
 
-_RETRYABLE_400_STATUS_CODE = {
+_RETRYABLE_400_STATUS_CODES = {
     # Using debug mode and breakpointing on the issue, we were able to validate that there issues are retryable. We've also opened a case
     # with Salesforce to try to understand what is causing that as the response does not have a body.
     406,
     # Most of the time, they don't have a body but there was one from the Salesforce Edge mentioning "We are setting things up. This process
     # can take a few minutes. This page will auto-refresh when ready. If it takes too long, please contact support or visit our <a>status
     # page</a> for more information." We therefore assume this is a transient error and will retry on it.
     420,
     codes.too_many_requests,
 }
 
 
 logger = logging.getLogger("airbyte")
 
 
-def default_backoff_handler(max_tries: int, backoff_method={"method": backoff.expo, "params": {"factor": 15}}, **kwargs):
+def default_backoff_handler(max_tries: int, backoff_method=None, backoff_params=None):
+    if backoff_method is None or backoff_params is None:
+        if not (backoff_method is None and backoff_params is None):
+            raise ValueError("Both `backoff_method` and `backoff_params` need to be provided if one is provided")
+        backoff_method = backoff.expo
+        backoff_params = {"factor": 15}
+
     def log_retry_attempt(details):
         _, exc, _ = sys.exc_info()
         logger.info(str(exc))
         logger.info(f"Caught retryable error after {details['tries']} tries. Waiting {details['wait']} seconds then retrying...")
 
     def should_give_up(exc):
-        give_up = exc.response is not None and exc.response.status_code not in _RETRYABLE_400_STATUS_CODE and 400 <= exc.response.status_code < 500
+        give_up = (
+            exc.response is not None
+            and exc.response.status_code not in _RETRYABLE_400_STATUS_CODES
+            and 400 <= exc.response.status_code < 500
+        )
 
         # Salesforce can return an error with a limit using a 403 code error.
         if exc.response is not None and exc.response.status_code == codes.forbidden:
             error_data = exc.response.json()[0]
             if error_data.get("errorCode", "") == "REQUEST_LIMIT_EXCEEDED":
                 give_up = True
 
         if give_up:
             logger.info(f"Giving up for returned HTTP status: {exc.response.status_code}, body: {exc.response.text}")
         return give_up
 
     return backoff.on_exception(
-        backoff_method["method"],
+        backoff_method,
         TRANSIENT_EXCEPTIONS,
         jitter=None,
         on_backoff=log_retry_attempt,
         giveup=should_give_up,
         max_tries=max_tries,
-        **backoff_method["params"],
+        **backoff_params,
     )
```

### Comparing `airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/run.py` & `airbyte_source_salesforce-2.4.2/source_salesforce/run.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/schemas/Describe.json` & `airbyte_source_salesforce-2.4.2/source_salesforce/schemas/Describe.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/source.py` & `airbyte_source_salesforce-2.4.2/source_salesforce/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/spec.yaml` & `airbyte_source_salesforce-2.4.2/source_salesforce/spec.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/streams.py` & `airbyte_source_salesforce-2.4.2/source_salesforce/streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import math
 import os
 import time
 import urllib.parse
 import uuid
 from abc import ABC
 from contextlib import closing
-from typing import Any, Callable, Iterable, List, Mapping, MutableMapping, Optional, Tuple, Type, Union
+from typing import Any, Callable, Dict, Iterable, List, Mapping, MutableMapping, Optional, Tuple, Type, Union
 
 import backoff
 import pandas as pd
 import pendulum
 import requests  # type: ignore[import]
 from airbyte_cdk.models import ConfiguredAirbyteCatalog, FailureType, SyncMode
 from airbyte_cdk.sources.streams.availability_strategy import AvailabilityStrategy
@@ -36,14 +36,15 @@
 
 # https://stackoverflow.com/a/54517228
 CSV_FIELD_SIZE_LIMIT = int(ctypes.c_ulong(-1).value // 2)
 csv.field_size_limit(CSV_FIELD_SIZE_LIMIT)
 
 DEFAULT_ENCODING = "utf-8"
 LOOKBACK_SECONDS = 600  # based on https://trailhead.salesforce.com/trailblazer-community/feed/0D54V00007T48TASAZ
+_JOB_TRANSIENT_ERRORS_MAX_RETRY = 1
 
 
 class SalesforceStream(HttpStream, ABC):
     state_converter = IsoMillisConcurrentStreamStateConverter()
     page_size = 2000
     transformer = TypeTransformer(TransformConfig.DefaultSchemaNormalization)
     encoding = DEFAULT_ENCODING
@@ -348,15 +349,15 @@
     MAX_RETRY_NUMBER = 3
 
     def path(self, next_page_token: Mapping[str, Any] = None, **kwargs: Any) -> str:
         return f"/services/data/{self.sf_api.version}/jobs/query"
 
     transformer = TypeTransformer(TransformConfig.CustomSchemaNormalization | TransformConfig.DefaultSchemaNormalization)
 
-    @default_backoff_handler(max_tries=5, backoff_method={"method": backoff.expo, "params": {"factor": 15}})
+    @default_backoff_handler(max_tries=5, backoff_method=backoff.expo, backoff_params={"factor": 15})
     def _send_http_request(self, method: str, url: str, json: dict = None, headers: dict = None, stream: bool = False):
         """
         This method should be used when you don't have to read data from the HTTP body. Else, you will have to retry when you actually read
         the response buffer (which is either by calling `json` or `iter_content`)
         """
         return self._non_retryable_send_http_request(method, url, json, headers, stream)
 
@@ -364,15 +365,15 @@
         headers = self.authenticator.get_auth_header() if not headers else headers | self.authenticator.get_auth_header()
         response = self._session.request(method, url=url, headers=headers, json=json, stream=stream)
         if response.status_code not in [200, 204]:
             self.logger.error(f"error body: {response.text}, sobject options: {self.sobject_options}")
         response.raise_for_status()
         return response
 
-    @default_backoff_handler(max_tries=5, backoff_method={"method": backoff.expo, "params": {"factor": 15}})
+    @default_backoff_handler(max_tries=5, backoff_method=backoff.expo, backoff_params={"factor": 15})
     def _create_stream_job(self, query: str, url: str) -> Optional[str]:
         json = {"operation": "queryAll", "query": query, "contentType": "CSV", "columnDelimiter": "COMMA", "lineEnding": "LF"}
         response = self._non_retryable_send_http_request("POST", url, json=json)
         job_id: str = response.json()["id"]
         return job_id
 
     def create_stream_job(self, query: str, url: str) -> Optional[str]:
@@ -394,17 +395,15 @@
                 # 2) Access to a sobject(stream) is not available
                 # 3) sobject is not queryable. It means this sobject can't be called directly.
                 #    We can call it as part of response from another sobject only.  E.g.:
                 #        initial query: "Select Id, Subject from ActivityHistory" -> error
                 #        updated query: "Select Name, (Select Subject,ActivityType from ActivityHistories) from Contact"
                 #    The second variant forces customisation for every case (ActivityHistory, ActivityHistories etc).
                 #    And the main problem is these subqueries doesn't support CSV response format.
-                error_data = error.response.json()[0]
-                error_code = error_data.get("errorCode")
-                error_message = error_data.get("message", "")
+                error_code, error_message = self._extract_error_code_and_message(error.response)
                 if error_message == "Selecting compound data not supported in Bulk Query" or (
                     error_code == "INVALIDENTITY" and "is not supported by the Bulk API" in error_message
                 ):
                     self.logger.error(
                         f"Cannot receive data for stream '{self.name}' using BULK API, "
                         f"sobject options: {self.sobject_options}, error message: '{error_message}'"
                     )
@@ -412,15 +411,15 @@
                     self.logger.error(
                         f"Cannot receive data for stream '{self.name}' ,"
                         f"sobject options: {self.sobject_options}, error message: '{error_message}'"
                     )
                 elif error.response.status_code == codes.FORBIDDEN and error_code == "REQUEST_LIMIT_EXCEEDED":
                     self.logger.error(
                         f"Cannot receive data for stream '{self.name}' ,"
-                        f"sobject options: {self.sobject_options}, Error message: '{error_data.get('message')}'"
+                        f"sobject options: {self.sobject_options}, Error message: '{error_message}'"
                     )
                 elif error.response.status_code == codes.BAD_REQUEST and error_message.endswith("does not support query"):
                     self.logger.error(
                         f"The stream '{self.name}' is not queryable, "
                         f"sobject options: {self.sobject_options}, error message: '{error_message}'"
                     )
                 elif (
@@ -448,17 +447,15 @@
         # minimal starting delay is 0.5 seconds.
         # this value was received empirically
         time.sleep(0.5)
         while pendulum.now() < expiration_time:
             try:
                 job_info = self._send_http_request("GET", url=url).json()
             except exceptions.HTTPError as error:
-                error_data = error.response.json()[0]
-                error_code = error_data.get("errorCode")
-                error_message = error_data.get("message", "")
+                error_code, error_message = self._extract_error_code_and_message(error.response)
                 if (
                     "We can't complete the action because enabled transaction security policies took too long to complete." in error_message
                     and error_code == "TXN_SECURITY_METERING_ERROR"
                 ):
                     message = 'A transient authentication error occurred. To prevent future syncs from failing, assign the "Exempt from Transaction Security" user permission to the authenticated user.'
                     raise AirbyteTracedException(message=message, failure_type=FailureType.config_error, exception=error)
                 else:
@@ -484,14 +481,27 @@
             self.logger.info(
                 f"Sleeping {delay_timeout} seconds while waiting for Job: {self.name}/{job_id} to complete. Current state: {job_status}"
             )
 
         self.logger.warning(f"Not wait the {self.name} data for {self.DEFAULT_WAIT_TIMEOUT_SECONDS} seconds, data: {job_info}!!")
         return job_status
 
+    def _extract_error_code_and_message(self, response: requests.Response) -> tuple[Optional[str], str]:
+        try:
+            error_data = response.json()[0]
+            return error_data.get("errorCode"), error_data.get("message", "")
+        except exceptions.JSONDecodeError:
+            self.logger.warning(f"The response for `{response.request.url}` is not a JSON but was `{response.content}`")
+        except IndexError:
+            self.logger.warning(
+                f"The response for `{response.request.url}` was expected to be a list with at least one element but was `{response.content}`"
+            )
+
+        return None, ""
+
     def execute_job(self, query: str, url: str) -> Tuple[Optional[str], Optional[str]]:
         job_status = "Failed"
         for i in range(0, self.MAX_RETRY_NUMBER):
             job_id = self.create_stream_job(query=query, url=url)
             if not job_id:
                 return None, job_status
             job_full_url = f"{url}/{job_id}"
@@ -531,15 +541,15 @@
         content_type, params = requests.utils._parse_content_type_header(content_type)
 
         if "charset" in params:
             return params["charset"].strip("'\"")
 
         return self.encoding
 
-    @default_backoff_handler(max_tries=5, backoff_method={"method": backoff.constant, "params": {"interval": 5}})
+    @default_backoff_handler(max_tries=5, backoff_method=backoff.constant, backoff_params={"interval": 5})
     def download_data(self, url: str, chunk_size: int = 1024) -> tuple[str, str, dict]:
         """
         Retrieves binary data result from successfully `executed_job`, using chunks, to avoid local memory limitations.
         @ url: string - the url of the `executed_job`
         @ chunk_size: int - the buffer size for each chunk to fetch from stream, in bytes, default: 1024 bytes
         Return the tuple containing string with file path of downloaded binary data (Saved temporarily) and file encoding.
         """
@@ -659,18 +669,19 @@
         salesforce_bulk_api_locator = None
         while True:
             req = PreparedRequest()
             req.prepare_url(f"{job_full_url}/results", {"locator": salesforce_bulk_api_locator})
             try:
                 tmp_file, response_encoding, response_headers = self.download_data(url=req.url)
             except TRANSIENT_EXCEPTIONS as exception:
-                if call_count != 0:
+                if call_count >= _JOB_TRANSIENT_ERRORS_MAX_RETRY:
+                    self.logger.error(f"Downloading data failed even after {call_count} retries. Stopping retry and raising exception")
                     raise exception
+                self.logger.warning(f"Downloading data failed after {call_count} retries. Retrying the whole job...")
                 call_count += 1
-                self.logger.warning("Downloading data failed even after retries. Retrying the whole job...")
                 yield from self.read_records(sync_mode, cursor_field, stream_slice, stream_state, call_count=call_count)
                 return
 
             for record in self.read_with_chunks(tmp_file, response_encoding):
                 yield record
 
             if response_headers.get("Sforce-Locator", "null") == "null":
```

### Comparing `airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/utils.py` & `airbyte_source_salesforce-2.4.2/source_salesforce/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.1.dev202403282031/PKG-INFO` & `airbyte_source_salesforce-2.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-salesforce
-Version: 2.4.1.dev202403282031
+Version: 2.4.2
 Summary: Source implementation for Salesforce.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

