# Comparing `tmp/context_python-0.8.0.tar.gz` & `tmp/context_python-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "context_python-0.8.0.tar", max compression
+gzip compressed data, was "context_python-0.9.0.tar", max compression
```

## Comparing `context_python-0.8.0.tar` & `context_python-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1067 2023-06-01 15:29:28.188846 context_python-0.8.0/LICENSE.md
--rw-r--r--   0        0        0     2899 2023-09-29 19:25:28.210751 context_python-0.8.0/README.md
--rw-r--r--   0        0        0       43 2023-06-01 14:40:09.995595 context_python-0.8.0/getcontext/__init__.py
--rw-r--r--   0        0        0      708 2023-11-16 17:03:22.304826 context_python-0.8.0/getcontext/generated/__init__.py
--rw-r--r--   0        0        0     4249 2023-11-30 13:46:15.179412 context_python-0.8.0/getcontext/generated/_client.py
--rw-r--r--   0        0        0     2579 2023-11-16 17:03:22.305181 context_python-0.8.0/getcontext/generated/_configuration.py
--rw-r--r--   0        0        0      674 2023-10-25 11:13:51.466853 context_python-0.8.0/getcontext/generated/_patch.py
--rw-r--r--   0        0        0    79052 2023-11-16 17:03:22.305601 context_python-0.8.0/getcontext/generated/_serialization.py
--rw-r--r--   0        0        0      861 2023-11-16 17:03:22.305859 context_python-0.8.0/getcontext/generated/_vendor.py
--rw-r--r--   0        0        0      708 2023-11-16 17:03:22.306046 context_python-0.8.0/getcontext/generated/aio/__init__.py
--rw-r--r--   0        0        0     4399 2023-11-30 13:46:15.179612 context_python-0.8.0/getcontext/generated/aio/_client.py
--rw-r--r--   0        0        0     2621 2023-11-16 17:03:22.306438 context_python-0.8.0/getcontext/generated/aio/_configuration.py
--rw-r--r--   0        0        0      674 2023-10-25 11:13:51.466881 context_python-0.8.0/getcontext/generated/aio/_patch.py
--rw-r--r--   0        0        0      872 2023-11-16 17:03:22.306589 context_python-0.8.0/getcontext/generated/aio/_vendor.py
--rw-r--r--   0        0        0      748 2023-11-30 13:46:15.179806 context_python-0.8.0/getcontext/generated/aio/operations/__init__.py
--rw-r--r--   0        0        0    54602 2023-11-30 13:46:15.180022 context_python-0.8.0/getcontext/generated/aio/operations/_operations.py
--rw-r--r--   0        0        0      674 2023-10-25 11:13:51.466944 context_python-0.8.0/getcontext/generated/aio/operations/_patch.py
--rw-r--r--   0        0        0     4759 2023-11-30 13:46:15.180223 context_python-0.8.0/getcontext/generated/models/__init__.py
--rw-r--r--   0        0        0     1735 2023-11-30 13:46:15.180359 context_python-0.8.0/getcontext/generated/models/_enums.py
--rw-r--r--   0        0        0    42881 2023-11-30 13:46:15.180543 context_python-0.8.0/getcontext/generated/models/_models.py
--rw-r--r--   0        0        0      674 2023-10-25 11:13:51.467069 context_python-0.8.0/getcontext/generated/models/_patch.py
--rw-r--r--   0        0        0      748 2023-11-30 13:46:15.180676 context_python-0.8.0/getcontext/generated/operations/__init__.py
--rw-r--r--   0        0        0    68269 2023-11-30 13:46:15.180892 context_python-0.8.0/getcontext/generated/operations/_operations.py
--rw-r--r--   0        0        0      674 2023-10-25 11:13:51.466898 context_python-0.8.0/getcontext/generated/operations/_patch.py
--rw-r--r--   0        0        0       26 2023-10-25 11:13:50.083412 context_python-0.8.0/getcontext/generated/py.typed
--rw-r--r--   0        0        0      691 2023-07-03 17:14:16.935162 context_python-0.8.0/getcontext/token.py
--rw-r--r--   0        0        0      551 2023-11-30 13:46:15.181048 context_python-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3560 1970-01-01 00:00:00.000000 context_python-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-01 15:29:28.188846 context_python-0.9.0/LICENSE.md
+-rw-r--r--   0        0        0     2899 2023-09-29 19:25:28.210751 context_python-0.9.0/README.md
+-rw-r--r--   0        0        0       43 2023-06-01 14:40:09.995595 context_python-0.9.0/getcontext/__init__.py
+-rw-r--r--   0        0        0      709 2024-01-10 14:45:46.531114 context_python-0.9.0/getcontext/generated/__init__.py
+-rw-r--r--   0        0        0     4513 2024-01-10 14:45:46.531330 context_python-0.9.0/getcontext/generated/_client.py
+-rw-r--r--   0        0        0     2580 2024-01-10 14:45:46.531524 context_python-0.9.0/getcontext/generated/_configuration.py
+-rw-r--r--   0        0        0      674 2023-10-25 11:13:51.466853 context_python-0.9.0/getcontext/generated/_patch.py
+-rw-r--r--   0        0        0    79092 2024-01-10 14:45:46.531835 context_python-0.9.0/getcontext/generated/_serialization.py
+-rw-r--r--   0        0        0      862 2024-01-10 14:45:46.532012 context_python-0.9.0/getcontext/generated/_vendor.py
+-rw-r--r--   0        0        0      709 2024-01-10 14:45:46.532173 context_python-0.9.0/getcontext/generated/aio/__init__.py
+-rw-r--r--   0        0        0     4667 2024-01-10 14:45:46.532364 context_python-0.9.0/getcontext/generated/aio/_client.py
+-rw-r--r--   0        0        0     2622 2024-01-10 14:45:46.532523 context_python-0.9.0/getcontext/generated/aio/_configuration.py
+-rw-r--r--   0        0        0      674 2023-10-25 11:13:51.466881 context_python-0.9.0/getcontext/generated/aio/_patch.py
+-rw-r--r--   0        0        0      873 2024-01-10 14:45:46.532663 context_python-0.9.0/getcontext/generated/aio/_vendor.py
+-rw-r--r--   0        0        0      825 2024-01-10 14:45:46.532808 context_python-0.9.0/getcontext/generated/aio/operations/__init__.py
+-rw-r--r--   0        0        0    62928 2024-01-10 14:45:46.533005 context_python-0.9.0/getcontext/generated/aio/operations/_operations.py
+-rw-r--r--   0        0        0      674 2023-10-25 11:13:51.466944 context_python-0.9.0/getcontext/generated/aio/operations/_patch.py
+-rw-r--r--   0        0        0     5818 2024-01-10 14:45:46.533241 context_python-0.9.0/getcontext/generated/models/__init__.py
+-rw-r--r--   0        0        0     2192 2024-01-10 14:45:46.533404 context_python-0.9.0/getcontext/generated/models/_enums.py
+-rw-r--r--   0        0        0    55790 2024-01-10 14:45:46.533716 context_python-0.9.0/getcontext/generated/models/_models.py
+-rw-r--r--   0        0        0      674 2023-10-25 11:13:51.467069 context_python-0.9.0/getcontext/generated/models/_patch.py
+-rw-r--r--   0        0        0      825 2024-01-10 14:45:46.534012 context_python-0.9.0/getcontext/generated/operations/__init__.py
+-rw-r--r--   0        0        0    78009 2024-01-10 14:45:46.534229 context_python-0.9.0/getcontext/generated/operations/_operations.py
+-rw-r--r--   0        0        0      674 2023-10-25 11:13:51.466898 context_python-0.9.0/getcontext/generated/operations/_patch.py
+-rw-r--r--   0        0        0       26 2023-10-25 11:13:50.083412 context_python-0.9.0/getcontext/generated/py.typed
+-rw-r--r--   0        0        0      691 2023-07-03 17:14:16.935162 context_python-0.9.0/getcontext/token.py
+-rw-r--r--   0        0        0      551 2024-01-10 14:45:46.535214 context_python-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3560 1970-01-01 00:00:00.000000 context_python-0.9.0/PKG-INFO
```

### Comparing `context_python-0.8.0/LICENSE.md` & `context_python-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `context_python-0.8.0/README.md` & `context_python-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `context_python-0.8.0/getcontext/generated/__init__.py` & `context_python-0.9.0/getcontext/generated/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.9.9)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.12.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._client import ContextAPI
 
 try:
     from ._patch import __all__ as _patch_all
```

### Comparing `context_python-0.8.0/getcontext/generated/_client.py` & `context_python-0.9.0/getcontext/generated/_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.9.9)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.12.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any, TYPE_CHECKING
 
 from azure.core import PipelineClient
 from azure.core.pipeline import policies
 from azure.core.rest import HttpRequest, HttpResponse
 
 from . import models as _models
 from ._configuration import ContextAPIConfiguration
 from ._serialization import Deserializer, Serializer
-from .operations import ContextAPIOperationsMixin, LogOperations
+from .operations import ContextAPIOperationsMixin, EvaluationsOperations, LogOperations
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
 
 
 class ContextAPI(ContextAPIOperationsMixin):  # pylint: disable=client-accepts-api-version-keyword
     """ContextAPI.
 
+    :ivar evaluations: EvaluationsOperations operations
+    :vartype evaluations: context_api.operations.EvaluationsOperations
     :ivar log: LogOperations operations
     :vartype log: context_api.operations.LogOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
     :keyword endpoint: Service URL. Default value is "https://api.context.ai".
     :paramtype endpoint: str
     """
@@ -55,14 +57,15 @@
             ]
         self._client: PipelineClient = PipelineClient(base_url=endpoint, policies=_policies, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
+        self.evaluations = EvaluationsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.log = LogOperations(self._client, self._config, self._serialize, self._deserialize)
 
     def send_request(self, request: HttpRequest, *, stream: bool = False, **kwargs: Any) -> HttpResponse:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
```

### Comparing `context_python-0.8.0/getcontext/generated/_configuration.py` & `context_python-0.9.0/getcontext/generated/_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.9.9)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.12.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any, TYPE_CHECKING
 
 from azure.core.pipeline import policies
```

### Comparing `context_python-0.8.0/getcontext/generated/_patch.py` & `context_python-0.9.0/getcontext/generated/_patch.py`

 * *Files identical despite different names*

### Comparing `context_python-0.8.0/getcontext/generated/_serialization.py` & `context_python-0.9.0/getcontext/generated/_serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -741,15 +741,15 @@
     def query(self, name, data, data_type, **kwargs):
         """Serialize data intended for a URL query.
 
         :param data: The data to be serialized.
         :param str data_type: The type to be serialized from.
         :keyword bool skip_quote: Whether to skip quote the serialized result.
         Defaults to False.
-        :rtype: str
+        :rtype: str, list
         :raises: TypeError if serialization fails.
         :raises: ValueError if data is None
         """
         try:
             # Treat the list aside, since we don't want to encode the div separator
             if data_type.startswith("["):
                 internal_data_type = data_type[1:-1]
@@ -1856,15 +1856,15 @@
         :param str attr: response string to be deserialized.
         :rtype: Decimal
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
-            return decimal.Decimal(attr)  # type: ignore
+            return decimal.Decimal(str(attr))  # type: ignore
         except decimal.DecimalException as err:
             msg = "Invalid decimal {}".format(attr)
             raise DeserializationError(msg) from err
 
     @staticmethod
     def deserialize_long(attr):
         """Deserialize string into long (Py2) or int (Py3).
@@ -1992,13 +1992,14 @@
         :param int attr: Object to be serialized.
         :rtype: Datetime
         :raises: DeserializationError if format invalid
         """
         if isinstance(attr, ET.Element):
             attr = int(attr.text)  # type: ignore
         try:
+            attr = int(attr)
             date_obj = datetime.datetime.fromtimestamp(attr, TZ_UTC)
         except ValueError as err:
             msg = "Cannot deserialize to unix datetime object."
             raise DeserializationError(msg) from err
         else:
             return date_obj
```

### Comparing `context_python-0.8.0/getcontext/generated/_vendor.py` & `context_python-0.9.0/getcontext/generated/_vendor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.9.9)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.12.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from abc import ABC
 from typing import TYPE_CHECKING
 
 from ._configuration import ContextAPIConfiguration
```

### Comparing `context_python-0.8.0/getcontext/generated/aio/__init__.py` & `context_python-0.9.0/getcontext/generated/aio/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.9.9)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.12.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._client import ContextAPI
 
 try:
     from ._patch import __all__ as _patch_all
```

### Comparing `context_python-0.8.0/getcontext/generated/aio/_client.py` & `context_python-0.9.0/getcontext/generated/aio/_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.9.9)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.12.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any, Awaitable, TYPE_CHECKING
 
 from azure.core import AsyncPipelineClient
 from azure.core.pipeline import policies
 from azure.core.rest import AsyncHttpResponse, HttpRequest
 
 from .. import models as _models
 from .._serialization import Deserializer, Serializer
 from ._configuration import ContextAPIConfiguration
-from .operations import ContextAPIOperationsMixin, LogOperations
+from .operations import ContextAPIOperationsMixin, EvaluationsOperations, LogOperations
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 
 class ContextAPI(ContextAPIOperationsMixin):  # pylint: disable=client-accepts-api-version-keyword
     """ContextAPI.
 
+    :ivar evaluations: EvaluationsOperations operations
+    :vartype evaluations: context_api.aio.operations.EvaluationsOperations
     :ivar log: LogOperations operations
     :vartype log: context_api.aio.operations.LogOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :keyword endpoint: Service URL. Default value is "https://api.context.ai".
     :paramtype endpoint: str
     """
@@ -55,14 +57,15 @@
             ]
         self._client: AsyncPipelineClient = AsyncPipelineClient(base_url=endpoint, policies=_policies, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
+        self.evaluations = EvaluationsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.log = LogOperations(self._client, self._config, self._serialize, self._deserialize)
 
     def send_request(
         self, request: HttpRequest, *, stream: bool = False, **kwargs: Any
     ) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
```

### Comparing `context_python-0.8.0/getcontext/generated/aio/_configuration.py` & `context_python-0.9.0/getcontext/generated/aio/_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.9.9)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.12.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any, TYPE_CHECKING
 
 from azure.core.pipeline import policies
```

### Comparing `context_python-0.8.0/getcontext/generated/aio/_patch.py` & `context_python-0.9.0/getcontext/generated/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `context_python-0.8.0/getcontext/generated/aio/_vendor.py` & `context_python-0.9.0/getcontext/generated/aio/_vendor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.9.9)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.12.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from abc import ABC
 from typing import TYPE_CHECKING
 
 from ._configuration import ContextAPIConfiguration
```

### Comparing `context_python-0.8.0/getcontext/generated/aio/operations/__init__.py` & `context_python-0.9.0/getcontext/generated/aio/operations/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.9.9)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.12.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._operations import ContextAPIOperationsMixin
+from ._operations import EvaluationsOperations
 from ._operations import LogOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "ContextAPIOperationsMixin",
+    "EvaluationsOperations",
     "LogOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

### Comparing `context_python-0.8.0/getcontext/generated/aio/operations/_operations.py` & `context_python-0.9.0/getcontext/generated/aio/operations/_operations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.9.9)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.12.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
@@ -28,14 +28,16 @@
     build_context_api_estimated_cost_request,
     build_context_api_rating_request,
     build_context_api_sentiment_request,
     build_context_api_suggested_topic_conversations_request,
     build_context_api_suggested_topic_statistics_request,
     build_context_api_suggested_topics_request,
     build_context_api_volume_request,
+    build_evaluations_result_request,
+    build_evaluations_run_request,
     build_log_conversation_request,
     build_log_conversation_thread_request,
     build_log_conversation_upsert_request,
     build_log_test_sets_request,
 )
 from .._vendor import ContextAPIMixinABC
 
@@ -797,14 +799,226 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
 
+class EvaluationsOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~context_api.aio.ContextAPI`'s
+        :attr:`evaluations` attribute.
+    """
+
+    models = _models
+
+    def __init__(self, *args, **kwargs) -> None:
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
+
+    @overload
+    async def run(
+        self,
+        body: Optional[_models.VersionRunParams] = None,
+        *,
+        authorization: Optional[str] = None,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.Paths2XppqwApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchema:
+        """Submits a test run request.
+
+        Submits a test run request.
+
+        :param body: Default value is None.
+        :type body: ~context_api.models.VersionRunParams
+        :keyword authorization: Default value is None.
+        :paramtype authorization: str
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: Paths2XppqwApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchema
+        :rtype:
+         ~context_api.models.Paths2XppqwApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchema
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def run(
+        self,
+        body: Optional[IO[bytes]] = None,
+        *,
+        authorization: Optional[str] = None,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.Paths2XppqwApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchema:
+        """Submits a test run request.
+
+        Submits a test run request.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword authorization: Default value is None.
+        :paramtype authorization: str
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: Paths2XppqwApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchema
+        :rtype:
+         ~context_api.models.Paths2XppqwApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchema
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def run(
+        self,
+        body: Optional[Union[_models.VersionRunParams, IO[bytes]]] = None,
+        *,
+        authorization: Optional[str] = None,
+        **kwargs: Any
+    ) -> _models.Paths2XppqwApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchema:
+        """Submits a test run request.
+
+        Submits a test run request.
+
+        :param body: Is either a VersionRunParams type or a IO[bytes] type. Default value is None.
+        :type body: ~context_api.models.VersionRunParams or IO[bytes]
+        :keyword authorization: Default value is None.
+        :paramtype authorization: str
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :return: Paths2XppqwApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchema
+        :rtype:
+         ~context_api.models.Paths2XppqwApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchema
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.Paths2XppqwApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchema] = kwargs.pop(
+            "cls", None
+        )
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "VersionRunParams")
+            else:
+                _json = None
+
+        _request = build_evaluations_run_request(
+            authorization=authorization,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [202]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize(
+            "Paths2XppqwApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchema", pipeline_response
+        )
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @distributed_trace_async
+    async def result(
+        self, id: str, *, authorization: Optional[str] = None, **kwargs: Any
+    ) -> _models.EvaluationsRunResponse:
+        """Polls a test run for updates and results.
+
+        Polls a test run for updates and results.
+
+        :param id: Required.
+        :type id: str
+        :keyword authorization: Default value is None.
+        :paramtype authorization: str
+        :return: EvaluationsRunResponse
+        :rtype: ~context_api.models.EvaluationsRunResponse
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[_models.EvaluationsRunResponse] = kwargs.pop("cls", None)
+
+        _request = build_evaluations_result_request(
+            id=id,
+            authorization=authorization,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("EvaluationsRunResponse", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
+
 class LogOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~context_api.aio.ContextAPI`'s
@@ -845,56 +1059,56 @@
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def conversation(  # pylint: disable=inconsistent-return-statements
         self,
-        body: Optional[IO] = None,
+        body: Optional[IO[bytes]] = None,
         *,
         authorization: Optional[str] = None,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> None:
         """Ingests a conversation.
 
         Ingests a conversation.
 
         :param body: Default value is None.
-        :type body: IO
+        :type body: IO[bytes]
         :keyword authorization: Default value is None.
         :paramtype authorization: str
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def conversation(  # pylint: disable=inconsistent-return-statements
         self,
         body: Optional[
-            Union[_models.PathsLi5TynApiV1LogConversationPostRequestbodyContentApplicationJsonSchema, IO]
+            Union[_models.PathsLi5TynApiV1LogConversationPostRequestbodyContentApplicationJsonSchema, IO[bytes]]
         ] = None,
         *,
         authorization: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """Ingests a conversation.
 
         Ingests a conversation.
 
         :param body: Is either a
-         PathsLi5TynApiV1LogConversationPostRequestbodyContentApplicationJsonSchema type or a IO type.
-         Default value is None.
+         PathsLi5TynApiV1LogConversationPostRequestbodyContentApplicationJsonSchema type or a IO[bytes]
+         type. Default value is None.
         :type body:
          ~context_api.models.PathsLi5TynApiV1LogConversationPostRequestbodyContentApplicationJsonSchema
-         or IO
+         or IO[bytes]
         :keyword authorization: Default value is None.
         :paramtype authorization: str
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: None
         :rtype: None
@@ -978,56 +1192,56 @@
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def conversation_upsert(  # pylint: disable=inconsistent-return-statements
         self,
-        body: Optional[IO] = None,
+        body: Optional[IO[bytes]] = None,
         *,
         authorization: Optional[str] = None,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> None:
         """Ingests or updates conversation.
 
         Ingests or updates conversation.
 
         :param body: Default value is None.
-        :type body: IO
+        :type body: IO[bytes]
         :keyword authorization: Default value is None.
         :paramtype authorization: str
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def conversation_upsert(  # pylint: disable=inconsistent-return-statements
         self,
         body: Optional[
-            Union[_models.PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema, IO]
+            Union[_models.PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema, IO[bytes]]
         ] = None,
         *,
         authorization: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """Ingests or updates conversation.
 
         Ingests or updates conversation.
 
         :param body: Is either a
-         PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema type or a IO
-         type. Default value is None.
+         PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema type or a
+         IO[bytes] type. Default value is None.
         :type body:
          ~context_api.models.PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema
-         or IO
+         or IO[bytes]
         :keyword authorization: Default value is None.
         :paramtype authorization: str
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: None
         :rtype: None
@@ -1114,26 +1328,26 @@
          ~context_api.models.PathsDo7Pm8ApiV1LogConversationThreadPostResponses201ContentApplicationJsonSchema
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def conversation_thread(
         self,
-        body: Optional[IO] = None,
+        body: Optional[IO[bytes]] = None,
         *,
         authorization: Optional[str] = None,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.PathsDo7Pm8ApiV1LogConversationThreadPostResponses201ContentApplicationJsonSchema:
         """Ingests or updates a thread.
 
         Ingests or updates a thread.
 
         :param body: Default value is None.
-        :type body: IO
+        :type body: IO[bytes]
         :keyword authorization: Default value is None.
         :paramtype authorization: str
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :return: PathsDo7Pm8ApiV1LogConversationThreadPostResponses201ContentApplicationJsonSchema
         :rtype:
@@ -1141,30 +1355,30 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def conversation_thread(
         self,
         body: Optional[
-            Union[_models.Paths1S2Rf6XApiV1LogConversationThreadPostRequestbodyContentApplicationJsonSchema, IO]
+            Union[_models.Paths1S2Rf6XApiV1LogConversationThreadPostRequestbodyContentApplicationJsonSchema, IO[bytes]]
         ] = None,
         *,
         authorization: Optional[str] = None,
         **kwargs: Any
     ) -> _models.PathsDo7Pm8ApiV1LogConversationThreadPostResponses201ContentApplicationJsonSchema:
         """Ingests or updates a thread.
 
         Ingests or updates a thread.
 
         :param body: Is either a
-         Paths1S2Rf6XApiV1LogConversationThreadPostRequestbodyContentApplicationJsonSchema type or a IO
-         type. Default value is None.
+         Paths1S2Rf6XApiV1LogConversationThreadPostRequestbodyContentApplicationJsonSchema type or a
+         IO[bytes] type. Default value is None.
         :type body:
          ~context_api.models.Paths1S2Rf6XApiV1LogConversationThreadPostRequestbodyContentApplicationJsonSchema
-         or IO
+         or IO[bytes]
         :keyword authorization: Default value is None.
         :paramtype authorization: str
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: PathsDo7Pm8ApiV1LogConversationThreadPostResponses201ContentApplicationJsonSchema
         :rtype:
@@ -1261,27 +1475,27 @@
         :rtype: ~context_api.models.TestSetParams
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def test_sets(
         self,
-        body: Optional[IO] = None,
+        body: Optional[IO[bytes]] = None,
         *,
         authorization: Optional[str] = None,
         copy_test_cases_from: Optional[str] = None,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.TestSetParams:
         """Returns test set and version details.
 
         Returns test set and version details.
 
         :param body: Default value is None.
-        :type body: IO
+        :type body: IO[bytes]
         :keyword authorization: Default value is None.
         :paramtype authorization: str
         :keyword copy_test_cases_from: If none, all test cases will be replaced with the ones provided
          in the request.:code:`<br />`If prior_version, only the test cases with the same name will be
          replaced and new test cases will be appended.:code:`<br />`. Default value is None.
         :paramtype copy_test_cases_from: str
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
@@ -1291,26 +1505,26 @@
         :rtype: ~context_api.models.TestSetParams
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def test_sets(
         self,
-        body: Optional[Union[_models.TestSet, IO]] = None,
+        body: Optional[Union[_models.TestSet, IO[bytes]]] = None,
         *,
         authorization: Optional[str] = None,
         copy_test_cases_from: Optional[str] = None,
         **kwargs: Any
     ) -> _models.TestSetParams:
         """Returns test set and version details.
 
         Returns test set and version details.
 
-        :param body: Is either a TestSet type or a IO type. Default value is None.
-        :type body: ~context_api.models.TestSet or IO
+        :param body: Is either a TestSet type or a IO[bytes] type. Default value is None.
+        :type body: ~context_api.models.TestSet or IO[bytes]
         :keyword authorization: Default value is None.
         :paramtype authorization: str
         :keyword copy_test_cases_from: If none, all test cases will be replaced with the ones provided
          in the request.:code:`<br />`If prior_version, only the test cases with the same name will be
          replaced and new test cases will be appended.:code:`<br />`. Default value is None.
         :paramtype copy_test_cases_from: str
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
```

### Comparing `context_python-0.8.0/getcontext/generated/aio/operations/_patch.py` & `context_python-0.9.0/getcontext/generated/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `context_python-0.8.0/getcontext/generated/models/__init__.py` & `context_python-0.9.0/getcontext/generated/models/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,110 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.9.9)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.12.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._models import Conversation
 from ._models import ConversationResponse
+from ._models import Evaluation
+from ._models import EvaluationsRunResponse
+from ._models import EvaluationsRunResponseDetails
+from ._models import EvaluationsRunResponseProgress
+from ._models import Evaluator
 from ._models import Message
 from ._models import MessageResponse
 from ._models import Pagination
 from ._models import Paths11Gsqt2ApiV1TopicSuggestionsIdStatisticsGetResponses200ContentApplicationJsonSchema
+from ._models import Paths14Bf6A5ApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchemaPropertiesData
 from ._models import Paths1AqjttjApiV1ConversationsSeriesSentimentGetResponses200ContentApplicationJsonSchema
 from ._models import Paths1J9XfjaApiV1ConversationsSeriesEstimatedCostGetResponses200ContentApplicationJsonSchema
 from ._models import (
     Paths1MjxjdtApiV1TopicSuggestionsIdStatisticsGetResponses200ContentApplicationJsonSchemaPropertiesStatistics,
 )
 from ._models import Paths1O34Sy5ApiV1LogConversationThreadPostResponses201ContentApplicationJsonSchemaPropertiesData
 from ._models import Paths1Ola7DlApiV1ConversationsSeriesVolumeGetResponses200ContentApplicationJsonSchema
 from ._models import Paths1S2Rf6XApiV1LogConversationThreadPostRequestbodyContentApplicationJsonSchema
 from ._models import Paths1TzwckqApiV1TopicSuggestionsIdConversationsGetResponses200ContentApplicationJsonSchema
 from ._models import Paths1U893W0ApiV1TopicSuggestionsGetResponses200ContentApplicationJsonSchema
+from ._models import Paths2XppqwApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchema
 from ._models import PathsDo7Pm8ApiV1LogConversationThreadPostResponses201ContentApplicationJsonSchema
 from ._models import PathsLi5TynApiV1LogConversationPostRequestbodyContentApplicationJsonSchema
 from ._models import PathsPixtmzApiV1ConversationsSeriesGetResponses200ContentApplicationJsonSchema
 from ._models import PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema
 from ._models import PathsXq2NqjApiV1ConversationsSeriesRatingGetResponses200ContentApplicationJsonSchema
 from ._models import PathsY5Azv9ApiV1ConversationsGetResponses200ContentApplicationJsonSchema
 from ._models import SeriesItem
 from ._models import TestCase
+from ._models import TestCaseDetails
 from ._models import TestCaseMessage
+from ._models import TestCaseRun
 from ._models import TestSet
 from ._models import TestSetParams
 from ._models import Thread
 from ._models import Topic
 from ._models import TopicWithSamples
+from ._models import VersionRunParams
 
 from ._enums import ConversationSentimentTrend
+from ._enums import EvaluationOutcome
+from ._enums import EvaluationsRunResponseStatus
 from ._enums import MessageParamsRole
 from ._enums import MessageParamsType
 from ._enums import MessageRole
 from ._enums import MessageType
 from ._enums import Rating
 from ._enums import TestCaseFrom
 from ._enums import TestCaseMessageRole
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "Conversation",
     "ConversationResponse",
+    "Evaluation",
+    "EvaluationsRunResponse",
+    "EvaluationsRunResponseDetails",
+    "EvaluationsRunResponseProgress",
+    "Evaluator",
     "Message",
     "MessageResponse",
     "Pagination",
     "Paths11Gsqt2ApiV1TopicSuggestionsIdStatisticsGetResponses200ContentApplicationJsonSchema",
+    "Paths14Bf6A5ApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchemaPropertiesData",
     "Paths1AqjttjApiV1ConversationsSeriesSentimentGetResponses200ContentApplicationJsonSchema",
     "Paths1J9XfjaApiV1ConversationsSeriesEstimatedCostGetResponses200ContentApplicationJsonSchema",
     "Paths1MjxjdtApiV1TopicSuggestionsIdStatisticsGetResponses200ContentApplicationJsonSchemaPropertiesStatistics",
     "Paths1O34Sy5ApiV1LogConversationThreadPostResponses201ContentApplicationJsonSchemaPropertiesData",
     "Paths1Ola7DlApiV1ConversationsSeriesVolumeGetResponses200ContentApplicationJsonSchema",
     "Paths1S2Rf6XApiV1LogConversationThreadPostRequestbodyContentApplicationJsonSchema",
     "Paths1TzwckqApiV1TopicSuggestionsIdConversationsGetResponses200ContentApplicationJsonSchema",
     "Paths1U893W0ApiV1TopicSuggestionsGetResponses200ContentApplicationJsonSchema",
+    "Paths2XppqwApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchema",
     "PathsDo7Pm8ApiV1LogConversationThreadPostResponses201ContentApplicationJsonSchema",
     "PathsLi5TynApiV1LogConversationPostRequestbodyContentApplicationJsonSchema",
     "PathsPixtmzApiV1ConversationsSeriesGetResponses200ContentApplicationJsonSchema",
     "PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema",
     "PathsXq2NqjApiV1ConversationsSeriesRatingGetResponses200ContentApplicationJsonSchema",
     "PathsY5Azv9ApiV1ConversationsGetResponses200ContentApplicationJsonSchema",
     "SeriesItem",
     "TestCase",
+    "TestCaseDetails",
     "TestCaseMessage",
+    "TestCaseRun",
     "TestSet",
     "TestSetParams",
     "Thread",
     "Topic",
     "TopicWithSamples",
+    "VersionRunParams",
     "ConversationSentimentTrend",
+    "EvaluationOutcome",
+    "EvaluationsRunResponseStatus",
     "MessageParamsRole",
     "MessageParamsType",
     "MessageRole",
     "MessageType",
     "Rating",
     "TestCaseFrom",
     "TestCaseMessageRole",
```

### Comparing `context_python-0.8.0/getcontext/generated/models/_enums.py` & `context_python-0.9.0/getcontext/generated/models/_enums.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.9.9)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.12.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from enum import Enum
 from azure.core import CaseInsensitiveEnumMeta
 
 
@@ -12,14 +12,32 @@
     """ConversationSentimentTrend."""
 
     UP = "up"
     FLAT = "flat"
     DOWN = "down"
 
 
+class EvaluationOutcome(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """EvaluationOutcome."""
+
+    NEGATIVE = "negative"
+    POSITIVE = "positive"
+    INCONCLUSIVE = "inconclusive"
+    PARTIALLY_PASSED = "partially_passed"
+
+
+class EvaluationsRunResponseStatus(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """EvaluationsRunResponseStatus."""
+
+    PENDING = "pending"
+    RUNNING = "running"
+    COMPLETED = "completed"
+    ERRORED = "errored"
+
+
 class MessageParamsRole(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """MessageParamsRole."""
 
     SYSTEM = "system"
     ASSISTANT = "assistant"
     USER = "user"
```

### Comparing `context_python-0.8.0/getcontext/generated/models/_models.py` & `context_python-0.9.0/getcontext/generated/models/_models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding=utf-8
 # pylint: disable=too-many-lines
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.9.9)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.12.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 import datetime
 import sys
 from typing import Any, Dict, List, Optional, TYPE_CHECKING, Union
 
@@ -121,14 +121,209 @@
         self.metadata = metadata
         self.sentiment_trend = sentiment_trend
         self.topics = topics
         self.suggested_topics = suggested_topics
         self.messages = messages
 
 
+class Evaluation(_serialization.Model):
+    """Evaluation.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar evaluator_name: Required.
+    :vartype evaluator_name: str
+    :ivar outcome: Required. Known values are: "negative", "positive", "inconclusive", and
+     "partially_passed".
+    :vartype outcome: str or ~context_api.models.EvaluationOutcome
+    :ivar reasoning:
+    :vartype reasoning: str
+    """
+
+    _validation = {
+        "evaluator_name": {"required": True},
+        "outcome": {"required": True},
+    }
+
+    _attribute_map = {
+        "evaluator_name": {"key": "evaluator_name", "type": "str"},
+        "outcome": {"key": "outcome", "type": "str"},
+        "reasoning": {"key": "reasoning", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        evaluator_name: str,
+        outcome: Union[str, "_models.EvaluationOutcome"],
+        reasoning: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword evaluator_name: Required.
+        :paramtype evaluator_name: str
+        :keyword outcome: Required. Known values are: "negative", "positive", "inconclusive", and
+         "partially_passed".
+        :paramtype outcome: str or ~context_api.models.EvaluationOutcome
+        :keyword reasoning:
+        :paramtype reasoning: str
+        """
+        super().__init__(**kwargs)
+        self.evaluator_name = evaluator_name
+        self.outcome = outcome
+        self.reasoning = reasoning
+
+
+class EvaluationsRunResponse(_serialization.Model):
+    """EvaluationsRunResponse.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar id: Required.
+    :vartype id: str
+    :ivar status: Required. Known values are: "pending", "running", "completed", and "errored".
+    :vartype status: str or ~context_api.models.EvaluationsRunResponseStatus
+    :ivar progress: Required.
+    :vartype progress: ~context_api.models.EvaluationsRunResponseProgress
+    :ivar started_at:
+    :vartype started_at: ~datetime.datetime
+    :ivar details: Required.
+    :vartype details: ~context_api.models.EvaluationsRunResponseDetails
+    :ivar results:
+    :vartype results: list[~context_api.models.TestCaseRun]
+    """
+
+    _validation = {
+        "id": {"required": True},
+        "status": {"required": True},
+        "progress": {"required": True},
+        "details": {"required": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "status": {"key": "status", "type": "str"},
+        "progress": {"key": "progress", "type": "EvaluationsRunResponseProgress"},
+        "started_at": {"key": "started_at", "type": "iso-8601"},
+        "details": {"key": "details", "type": "EvaluationsRunResponseDetails"},
+        "results": {"key": "results", "type": "[TestCaseRun]"},
+    }
+
+    def __init__(
+        self,
+        *,
+        id: str,  # pylint: disable=redefined-builtin
+        status: Union[str, "_models.EvaluationsRunResponseStatus"],
+        progress: "_models.EvaluationsRunResponseProgress",
+        details: "_models.EvaluationsRunResponseDetails",
+        started_at: Optional[datetime.datetime] = None,
+        results: Optional[List["_models.TestCaseRun"]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword id: Required.
+        :paramtype id: str
+        :keyword status: Required. Known values are: "pending", "running", "completed", and "errored".
+        :paramtype status: str or ~context_api.models.EvaluationsRunResponseStatus
+        :keyword progress: Required.
+        :paramtype progress: ~context_api.models.EvaluationsRunResponseProgress
+        :keyword started_at:
+        :paramtype started_at: ~datetime.datetime
+        :keyword details: Required.
+        :paramtype details: ~context_api.models.EvaluationsRunResponseDetails
+        :keyword results:
+        :paramtype results: list[~context_api.models.TestCaseRun]
+        """
+        super().__init__(**kwargs)
+        self.id = id
+        self.status = status
+        self.progress = progress
+        self.started_at = started_at
+        self.details = details
+        self.results = results
+
+
+class EvaluationsRunResponseDetails(_serialization.Model):
+    """EvaluationsRunResponseDetails.
+
+    :ivar test_set_name:
+    :vartype test_set_name: str
+    :ivar version:
+    :vartype version: int
+    """
+
+    _attribute_map = {
+        "test_set_name": {"key": "test_set_name", "type": "str"},
+        "version": {"key": "version", "type": "int"},
+    }
+
+    def __init__(self, *, test_set_name: Optional[str] = None, version: Optional[int] = None, **kwargs: Any) -> None:
+        """
+        :keyword test_set_name:
+        :paramtype test_set_name: str
+        :keyword version:
+        :paramtype version: int
+        """
+        super().__init__(**kwargs)
+        self.test_set_name = test_set_name
+        self.version = version
+
+
+class EvaluationsRunResponseProgress(_serialization.Model):
+    """EvaluationsRunResponseProgress.
+
+    :ivar completed:
+    :vartype completed: int
+    :ivar pending:
+    :vartype pending: int
+    """
+
+    _attribute_map = {
+        "completed": {"key": "completed", "type": "int"},
+        "pending": {"key": "pending", "type": "int"},
+    }
+
+    def __init__(self, *, completed: Optional[int] = None, pending: Optional[int] = None, **kwargs: Any) -> None:
+        """
+        :keyword completed:
+        :paramtype completed: int
+        :keyword pending:
+        :paramtype pending: int
+        """
+        super().__init__(**kwargs)
+        self.completed = completed
+        self.pending = pending
+
+
+class Evaluator(_serialization.Model):
+    """Evaluator.
+
+    :ivar evaluator:
+    :vartype evaluator: str
+    :ivar options: Any object.
+    :vartype options: JSON
+    """
+
+    _attribute_map = {
+        "evaluator": {"key": "evaluator", "type": "str"},
+        "options": {"key": "options", "type": "object"},
+    }
+
+    def __init__(self, *, evaluator: Optional[str] = None, options: Optional[JSON] = None, **kwargs: Any) -> None:
+        """
+        :keyword evaluator:
+        :paramtype evaluator: str
+        :keyword options: Any object.
+        :paramtype options: JSON
+        """
+        super().__init__(**kwargs)
+        self.evaluator = evaluator
+        self.options = options
+
+
 class Message(_serialization.Model):
     """Message.
 
     :ivar role: Known values are: "system", "assistant", and "user".
     :vartype role: str or ~context_api.models.MessageParamsRole
     :ivar message:
     :vartype message: str
@@ -386,15 +581,17 @@
         self.per_page = per_page
         self.current_page = current_page
         self.previous_page = previous_page
         self.next_page = next_page
         self.page_count = page_count
 
 
-class Paths11Gsqt2ApiV1TopicSuggestionsIdStatisticsGetResponses200ContentApplicationJsonSchema(_serialization.Model):
+class Paths11Gsqt2ApiV1TopicSuggestionsIdStatisticsGetResponses200ContentApplicationJsonSchema(
+    _serialization.Model
+):  # pylint: disable=name-too-long
     """Paths11Gsqt2ApiV1TopicSuggestionsIdStatisticsGetResponses200ContentApplicationJsonSchema.
 
     All required parameters must be populated in order to send to server.
 
     :ivar topic: Required.
     :vartype topic: ~context_api.models.Topic
     :ivar statistics: Required.
@@ -430,15 +627,39 @@
          ~context_api.models.Paths1MjxjdtApiV1TopicSuggestionsIdStatisticsGetResponses200ContentApplicationJsonSchemaPropertiesStatistics  # pylint: disable=line-too-long
         """
         super().__init__(**kwargs)
         self.topic = topic
         self.statistics = statistics
 
 
-class Paths1AqjttjApiV1ConversationsSeriesSentimentGetResponses200ContentApplicationJsonSchema(_serialization.Model):
+class Paths14Bf6A5ApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchemaPropertiesData(
+    _serialization.Model
+):  # pylint: disable=name-too-long
+    """Paths14Bf6A5ApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchemaPropertiesData.
+
+    :ivar run_id:
+    :vartype run_id: str
+    """
+
+    _attribute_map = {
+        "run_id": {"key": "run_id", "type": "str"},
+    }
+
+    def __init__(self, *, run_id: Optional[str] = None, **kwargs: Any) -> None:
+        """
+        :keyword run_id:
+        :paramtype run_id: str
+        """
+        super().__init__(**kwargs)
+        self.run_id = run_id
+
+
+class Paths1AqjttjApiV1ConversationsSeriesSentimentGetResponses200ContentApplicationJsonSchema(
+    _serialization.Model
+):  # pylint: disable=name-too-long
     """Paths1AqjttjApiV1ConversationsSeriesSentimentGetResponses200ContentApplicationJsonSchema.
 
     All required parameters must be populated in order to send to server.
 
     :ivar series: Required.
     :vartype series: list[~context_api.models.SeriesItem]
     :ivar type: Required.
@@ -495,15 +716,15 @@
         self.period = period
         self.start_time = start_time
         self.end_time = end_time
 
 
 class Paths1J9XfjaApiV1ConversationsSeriesEstimatedCostGetResponses200ContentApplicationJsonSchema(
     _serialization.Model
-):
+):  # pylint: disable=name-too-long
     """Paths1J9XfjaApiV1ConversationsSeriesEstimatedCostGetResponses200ContentApplicationJsonSchema.
 
     All required parameters must be populated in order to send to server.
 
     :ivar series: Required.
     :vartype series: list[~context_api.models.SeriesItem]
     :ivar type: Required.
@@ -560,15 +781,15 @@
         self.period = period
         self.start_time = start_time
         self.end_time = end_time
 
 
 class Paths1MjxjdtApiV1TopicSuggestionsIdStatisticsGetResponses200ContentApplicationJsonSchemaPropertiesStatistics(
     _serialization.Model
-):
+):  # pylint: disable=name-too-long
     """Paths1MjxjdtApiV1TopicSuggestionsIdStatisticsGetResponses200ContentApplicationJsonSchemaPropertiesStatistics.
 
     All required parameters must be populated in order to send to server.
 
     :ivar conversation_count: Required.
     :vartype conversation_count: int
     :ivar user_message_count: Required.
@@ -625,15 +846,15 @@
         self.assistant_message_count = assistant_message_count
         self.mean_sentiment = mean_sentiment
         self.mean_user_rating = mean_user_rating
 
 
 class Paths1O34Sy5ApiV1LogConversationThreadPostResponses201ContentApplicationJsonSchemaPropertiesData(
     _serialization.Model
-):
+):  # pylint: disable=name-too-long
     """Paths1O34Sy5ApiV1LogConversationThreadPostResponses201ContentApplicationJsonSchemaPropertiesData.
 
     :ivar id:
     :vartype id: str
     """
 
     _attribute_map = {
@@ -645,15 +866,17 @@
         :keyword id:
         :paramtype id: str
         """
         super().__init__(**kwargs)
         self.id = id
 
 
-class Paths1Ola7DlApiV1ConversationsSeriesVolumeGetResponses200ContentApplicationJsonSchema(_serialization.Model):
+class Paths1Ola7DlApiV1ConversationsSeriesVolumeGetResponses200ContentApplicationJsonSchema(
+    _serialization.Model
+):  # pylint: disable=name-too-long
     """Paths1Ola7DlApiV1ConversationsSeriesVolumeGetResponses200ContentApplicationJsonSchema.
 
     All required parameters must be populated in order to send to server.
 
     :ivar series: Required.
     :vartype series: list[~context_api.models.SeriesItem]
     :ivar type: Required.
@@ -708,15 +931,17 @@
         self.series = series
         self.type = type
         self.period = period
         self.start_time = start_time
         self.end_time = end_time
 
 
-class Paths1S2Rf6XApiV1LogConversationThreadPostRequestbodyContentApplicationJsonSchema(_serialization.Model):
+class Paths1S2Rf6XApiV1LogConversationThreadPostRequestbodyContentApplicationJsonSchema(
+    _serialization.Model
+):  # pylint: disable=name-too-long
     """Paths1S2Rf6XApiV1LogConversationThreadPostRequestbodyContentApplicationJsonSchema.
 
     :ivar conversation:
     :vartype conversation: ~context_api.models.Thread
     """
 
     _attribute_map = {
@@ -728,15 +953,17 @@
         :keyword conversation:
         :paramtype conversation: ~context_api.models.Thread
         """
         super().__init__(**kwargs)
         self.conversation = conversation
 
 
-class Paths1TzwckqApiV1TopicSuggestionsIdConversationsGetResponses200ContentApplicationJsonSchema(_serialization.Model):
+class Paths1TzwckqApiV1TopicSuggestionsIdConversationsGetResponses200ContentApplicationJsonSchema(
+    _serialization.Model
+):  # pylint: disable=name-too-long
     """Paths1TzwckqApiV1TopicSuggestionsIdConversationsGetResponses200ContentApplicationJsonSchema.
 
     All required parameters must be populated in order to send to server.
 
     :ivar conversations: Required.
     :vartype conversations: list[~context_api.models.ConversationResponse]
     :ivar pagination: Required.
@@ -763,15 +990,17 @@
         :paramtype pagination: ~context_api.models.Pagination
         """
         super().__init__(**kwargs)
         self.conversations = conversations
         self.pagination = pagination
 
 
-class Paths1U893W0ApiV1TopicSuggestionsGetResponses200ContentApplicationJsonSchema(_serialization.Model):
+class Paths1U893W0ApiV1TopicSuggestionsGetResponses200ContentApplicationJsonSchema(
+    _serialization.Model
+):  # pylint: disable=name-too-long
     """Paths1U893W0ApiV1TopicSuggestionsGetResponses200ContentApplicationJsonSchema.
 
     All required parameters must be populated in order to send to server.
 
     :ivar topics: Required.
     :vartype topics: list[~context_api.models.TopicWithSamples]
     :ivar pagination: Required.
@@ -798,15 +1027,58 @@
         :paramtype pagination: ~context_api.models.Pagination
         """
         super().__init__(**kwargs)
         self.topics = topics
         self.pagination = pagination
 
 
-class PathsDo7Pm8ApiV1LogConversationThreadPostResponses201ContentApplicationJsonSchema(_serialization.Model):
+class Paths2XppqwApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchema(
+    _serialization.Model
+):  # pylint: disable=name-too-long
+    """Paths2XppqwApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchema.
+
+    :ivar status:
+    :vartype status: str
+    :ivar data:
+    :vartype data:
+     ~context_api.models.Paths14Bf6A5ApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchemaPropertiesData
+    """
+
+    _attribute_map = {
+        "status": {"key": "status", "type": "str"},
+        "data": {
+            "key": "data",
+            "type": "Paths14Bf6A5ApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchemaPropertiesData",
+        },
+    }
+
+    def __init__(
+        self,
+        *,
+        status: Optional[str] = None,
+        data: Optional[
+            "_models.Paths14Bf6A5ApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchemaPropertiesData"
+        ] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword status:
+        :paramtype status: str
+        :keyword data:
+        :paramtype data:
+         ~context_api.models.Paths14Bf6A5ApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchemaPropertiesData
+        """
+        super().__init__(**kwargs)
+        self.status = status
+        self.data = data
+
+
+class PathsDo7Pm8ApiV1LogConversationThreadPostResponses201ContentApplicationJsonSchema(
+    _serialization.Model
+):  # pylint: disable=name-too-long
     """PathsDo7Pm8ApiV1LogConversationThreadPostResponses201ContentApplicationJsonSchema.
 
     :ivar status:
     :vartype status: str
     :ivar data:
     :vartype data:
      ~context_api.models.Paths1O34Sy5ApiV1LogConversationThreadPostResponses201ContentApplicationJsonSchemaPropertiesData  # pylint: disable=line-too-long
@@ -837,15 +1109,17 @@
          ~context_api.models.Paths1O34Sy5ApiV1LogConversationThreadPostResponses201ContentApplicationJsonSchemaPropertiesData  # pylint: disable=line-too-long
         """
         super().__init__(**kwargs)
         self.status = status
         self.data = data
 
 
-class PathsLi5TynApiV1LogConversationPostRequestbodyContentApplicationJsonSchema(_serialization.Model):
+class PathsLi5TynApiV1LogConversationPostRequestbodyContentApplicationJsonSchema(
+    _serialization.Model
+):  # pylint: disable=name-too-long
     """PathsLi5TynApiV1LogConversationPostRequestbodyContentApplicationJsonSchema.
 
     :ivar conversation:
     :vartype conversation: ~context_api.models.Conversation
     """
 
     _attribute_map = {
@@ -857,15 +1131,17 @@
         :keyword conversation:
         :paramtype conversation: ~context_api.models.Conversation
         """
         super().__init__(**kwargs)
         self.conversation = conversation
 
 
-class PathsPixtmzApiV1ConversationsSeriesGetResponses200ContentApplicationJsonSchema(_serialization.Model):
+class PathsPixtmzApiV1ConversationsSeriesGetResponses200ContentApplicationJsonSchema(
+    _serialization.Model
+):  # pylint: disable=name-too-long
     """PathsPixtmzApiV1ConversationsSeriesGetResponses200ContentApplicationJsonSchema.
 
     All required parameters must be populated in order to send to server.
 
     :ivar available: Required.
     :vartype available: list[str]
     """
@@ -883,15 +1159,17 @@
         :keyword available: Required.
         :paramtype available: list[str]
         """
         super().__init__(**kwargs)
         self.available = available
 
 
-class PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema(_serialization.Model):
+class PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema(
+    _serialization.Model
+):  # pylint: disable=name-too-long
     """PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema.
 
     :ivar conversation:
     :vartype conversation: ~context_api.models.Conversation
     """
 
     _attribute_map = {
@@ -903,15 +1181,17 @@
         :keyword conversation:
         :paramtype conversation: ~context_api.models.Conversation
         """
         super().__init__(**kwargs)
         self.conversation = conversation
 
 
-class PathsXq2NqjApiV1ConversationsSeriesRatingGetResponses200ContentApplicationJsonSchema(_serialization.Model):
+class PathsXq2NqjApiV1ConversationsSeriesRatingGetResponses200ContentApplicationJsonSchema(
+    _serialization.Model
+):  # pylint: disable=name-too-long
     """PathsXq2NqjApiV1ConversationsSeriesRatingGetResponses200ContentApplicationJsonSchema.
 
     All required parameters must be populated in order to send to server.
 
     :ivar series: Required.
     :vartype series: list[~context_api.models.SeriesItem]
     :ivar type: Required.
@@ -966,15 +1246,17 @@
         self.series = series
         self.type = type
         self.period = period
         self.start_time = start_time
         self.end_time = end_time
 
 
-class PathsY5Azv9ApiV1ConversationsGetResponses200ContentApplicationJsonSchema(_serialization.Model):
+class PathsY5Azv9ApiV1ConversationsGetResponses200ContentApplicationJsonSchema(
+    _serialization.Model
+):  # pylint: disable=name-too-long
     """PathsY5Azv9ApiV1ConversationsGetResponses200ContentApplicationJsonSchema.
 
     All required parameters must be populated in order to send to server.
 
     :ivar conversations: Required.
     :vartype conversations: list[~context_api.models.ConversationResponse]
     :ivar pagination: Required.
@@ -1045,41 +1327,102 @@
 
     :ivar name: Required.
     :vartype name: str
     :ivar model: Required.
     :vartype model: str
     :ivar messages: Required.
     :vartype messages: list[~context_api.models.TestCaseMessage]
+    :ivar evaluators:
+    :vartype evaluators: list[~context_api.models.Evaluator]
     """
 
     _validation = {
         "name": {"required": True},
         "model": {"required": True},
         "messages": {"required": True},
     }
 
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
         "model": {"key": "model", "type": "str"},
         "messages": {"key": "messages", "type": "[TestCaseMessage]"},
+        "evaluators": {"key": "evaluators", "type": "[Evaluator]"},
     }
 
-    def __init__(self, *, name: str, model: str, messages: List["_models.TestCaseMessage"], **kwargs: Any) -> None:
+    def __init__(
+        self,
+        *,
+        name: str,
+        model: str,
+        messages: List["_models.TestCaseMessage"],
+        evaluators: Optional[List["_models.Evaluator"]] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name: Required.
         :paramtype name: str
         :keyword model: Required.
         :paramtype model: str
         :keyword messages: Required.
         :paramtype messages: list[~context_api.models.TestCaseMessage]
+        :keyword evaluators:
+        :paramtype evaluators: list[~context_api.models.Evaluator]
         """
         super().__init__(**kwargs)
         self.name = name
         self.model = model
         self.messages = messages
+        self.evaluators = evaluators
+
+
+class TestCaseDetails(_serialization.Model):
+    """TestCaseDetails.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar name: Required.
+    :vartype name: str
+    :ivar input: Required.
+    :vartype input: list[~context_api.models.TestCaseMessage]
+    :ivar output: Required.
+    :vartype output: list[~context_api.models.TestCaseMessage]
+    """
+
+    _validation = {
+        "name": {"required": True},
+        "input": {"required": True},
+        "output": {"required": True},
+    }
+
+    _attribute_map = {
+        "name": {"key": "name", "type": "str"},
+        "input": {"key": "input", "type": "[TestCaseMessage]"},
+        "output": {"key": "output", "type": "[TestCaseMessage]"},
+    }
+
+    def __init__(
+        self,
+        *,
+        name: str,
+        input: List["_models.TestCaseMessage"],
+        output: List["_models.TestCaseMessage"],
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword name: Required.
+        :paramtype name: str
+        :keyword input: Required.
+        :paramtype input: list[~context_api.models.TestCaseMessage]
+        :keyword output: Required.
+        :paramtype output: list[~context_api.models.TestCaseMessage]
+        """
+        super().__init__(**kwargs)
+        self.name = name
+        self.input = input
+        self.output = output
 
 
 class TestCaseMessage(_serialization.Model):
     """TestCaseMessage.
 
     All required parameters must be populated in order to send to server.
 
@@ -1107,45 +1450,93 @@
         :paramtype role: str or ~context_api.models.TestCaseMessageRole
         """
         super().__init__(**kwargs)
         self.message = message
         self.role = role
 
 
+class TestCaseRun(_serialization.Model):
+    """TestCaseRun.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar test_case: Required.
+    :vartype test_case: ~context_api.models.TestCaseDetails
+    :ivar evaluations: Required.
+    :vartype evaluations: list[~context_api.models.Evaluation]
+    """
+
+    _validation = {
+        "test_case": {"required": True},
+        "evaluations": {"required": True},
+    }
+
+    _attribute_map = {
+        "test_case": {"key": "test_case", "type": "TestCaseDetails"},
+        "evaluations": {"key": "evaluations", "type": "[Evaluation]"},
+    }
+
+    def __init__(
+        self, *, test_case: "_models.TestCaseDetails", evaluations: List["_models.Evaluation"], **kwargs: Any
+    ) -> None:
+        """
+        :keyword test_case: Required.
+        :paramtype test_case: ~context_api.models.TestCaseDetails
+        :keyword evaluations: Required.
+        :paramtype evaluations: list[~context_api.models.Evaluation]
+        """
+        super().__init__(**kwargs)
+        self.test_case = test_case
+        self.evaluations = evaluations
+
+
 class TestSet(_serialization.Model):
     """TestSet.
 
     All required parameters must be populated in order to send to server.
 
     :ivar name: Required.
     :vartype name: str
     :ivar test_cases: Required.
     :vartype test_cases: list[~context_api.models.TestCase]
+    :ivar evaluators:
+    :vartype evaluators: list[~context_api.models.Evaluator]
     """
 
     _validation = {
         "name": {"required": True},
         "test_cases": {"required": True},
     }
 
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
         "test_cases": {"key": "test_cases", "type": "[TestCase]"},
+        "evaluators": {"key": "evaluators", "type": "[Evaluator]"},
     }
 
-    def __init__(self, *, name: str, test_cases: List["_models.TestCase"], **kwargs: Any) -> None:
+    def __init__(
+        self,
+        *,
+        name: str,
+        test_cases: List["_models.TestCase"],
+        evaluators: Optional[List["_models.Evaluator"]] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name: Required.
         :paramtype name: str
         :keyword test_cases: Required.
         :paramtype test_cases: list[~context_api.models.TestCase]
+        :keyword evaluators:
+        :paramtype evaluators: list[~context_api.models.Evaluator]
         """
         super().__init__(**kwargs)
         self.name = name
         self.test_cases = test_cases
+        self.evaluators = evaluators
 
 
 class TestSetParams(_serialization.Model):
     """TestSetParams.
 
     All required parameters must be populated in order to send to server.
 
@@ -1296,7 +1687,40 @@
         :keyword conversations_sample: Required.
         :paramtype conversations_sample: list[~context_api.models.ConversationResponse]
         """
         super().__init__(**kwargs)
         self.id = id
         self.name = name
         self.conversations_sample = conversations_sample
+
+
+class VersionRunParams(_serialization.Model):
+    """VersionRunParams.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar test_set_name: Required.
+    :vartype test_set_name: str
+    :ivar version: Required.
+    :vartype version: int
+    """
+
+    _validation = {
+        "test_set_name": {"required": True},
+        "version": {"required": True},
+    }
+
+    _attribute_map = {
+        "test_set_name": {"key": "test_set_name", "type": "str"},
+        "version": {"key": "version", "type": "int"},
+    }
+
+    def __init__(self, *, test_set_name: str, version: int, **kwargs: Any) -> None:
+        """
+        :keyword test_set_name: Required.
+        :paramtype test_set_name: str
+        :keyword version: Required.
+        :paramtype version: int
+        """
+        super().__init__(**kwargs)
+        self.test_set_name = test_set_name
+        self.version = version
```

### Comparing `context_python-0.8.0/getcontext/generated/models/_patch.py` & `context_python-0.9.0/getcontext/generated/models/_patch.py`

 * *Files identical despite different names*

### Comparing `context_python-0.8.0/getcontext/generated/operations/__init__.py` & `context_python-0.9.0/getcontext/generated/operations/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.9.9)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.12.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._operations import ContextAPIOperationsMixin
+from ._operations import EvaluationsOperations
 from ._operations import LogOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "ContextAPIOperationsMixin",
+    "EvaluationsOperations",
     "LogOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

### Comparing `context_python-0.8.0/getcontext/generated/operations/_operations.py` & `context_python-0.9.0/getcontext/generated/operations/_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.9.9)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.12.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
@@ -335,14 +335,54 @@
     if authorization is not None:
         _headers["Authorization"] = _SERIALIZER.header("authorization", authorization, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
+def build_evaluations_run_request(*, authorization: Optional[str] = None, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/api/v1/evaluations/run"
+
+    # Construct headers
+    if authorization is not None:
+        _headers["Authorization"] = _SERIALIZER.header("authorization", authorization, "str")
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
+def build_evaluations_result_request(id: str, *, authorization: Optional[str] = None, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/api/v1/evaluations/run/{id}"
+    path_format_arguments = {
+        "id": _SERIALIZER.url("id", id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    if authorization is not None:
+        _headers["Authorization"] = _SERIALIZER.header("authorization", authorization, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
+
+
 def build_log_conversation_request(*, authorization: Optional[str] = None, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     # Construct URL
     _url = "/api/v1/log/conversation"
 
@@ -1170,14 +1210,224 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
 
+class EvaluationsOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~context_api.ContextAPI`'s
+        :attr:`evaluations` attribute.
+    """
+
+    models = _models
+
+    def __init__(self, *args, **kwargs):
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
+
+    @overload
+    def run(
+        self,
+        body: Optional[_models.VersionRunParams] = None,
+        *,
+        authorization: Optional[str] = None,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.Paths2XppqwApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchema:
+        """Submits a test run request.
+
+        Submits a test run request.
+
+        :param body: Default value is None.
+        :type body: ~context_api.models.VersionRunParams
+        :keyword authorization: Default value is None.
+        :paramtype authorization: str
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: Paths2XppqwApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchema
+        :rtype:
+         ~context_api.models.Paths2XppqwApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchema
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def run(
+        self,
+        body: Optional[IO[bytes]] = None,
+        *,
+        authorization: Optional[str] = None,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.Paths2XppqwApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchema:
+        """Submits a test run request.
+
+        Submits a test run request.
+
+        :param body: Default value is None.
+        :type body: IO[bytes]
+        :keyword authorization: Default value is None.
+        :paramtype authorization: str
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: Paths2XppqwApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchema
+        :rtype:
+         ~context_api.models.Paths2XppqwApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchema
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def run(
+        self,
+        body: Optional[Union[_models.VersionRunParams, IO[bytes]]] = None,
+        *,
+        authorization: Optional[str] = None,
+        **kwargs: Any
+    ) -> _models.Paths2XppqwApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchema:
+        """Submits a test run request.
+
+        Submits a test run request.
+
+        :param body: Is either a VersionRunParams type or a IO[bytes] type. Default value is None.
+        :type body: ~context_api.models.VersionRunParams or IO[bytes]
+        :keyword authorization: Default value is None.
+        :paramtype authorization: str
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :return: Paths2XppqwApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchema
+        :rtype:
+         ~context_api.models.Paths2XppqwApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchema
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.Paths2XppqwApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchema] = kwargs.pop(
+            "cls", None
+        )
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "VersionRunParams")
+            else:
+                _json = None
+
+        _request = build_evaluations_run_request(
+            authorization=authorization,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [202]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize(
+            "Paths2XppqwApiV1EvaluationsRunPostResponses202ContentApplicationJsonSchema", pipeline_response
+        )
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @distributed_trace
+    def result(self, id: str, *, authorization: Optional[str] = None, **kwargs: Any) -> _models.EvaluationsRunResponse:
+        """Polls a test run for updates and results.
+
+        Polls a test run for updates and results.
+
+        :param id: Required.
+        :type id: str
+        :keyword authorization: Default value is None.
+        :paramtype authorization: str
+        :return: EvaluationsRunResponse
+        :rtype: ~context_api.models.EvaluationsRunResponse
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[_models.EvaluationsRunResponse] = kwargs.pop("cls", None)
+
+        _request = build_evaluations_result_request(
+            id=id,
+            authorization=authorization,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("EvaluationsRunResponse", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
+
 class LogOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~context_api.ContextAPI`'s
@@ -1218,56 +1468,56 @@
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def conversation(  # pylint: disable=inconsistent-return-statements
         self,
-        body: Optional[IO] = None,
+        body: Optional[IO[bytes]] = None,
         *,
         authorization: Optional[str] = None,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> None:
         """Ingests a conversation.
 
         Ingests a conversation.
 
         :param body: Default value is None.
-        :type body: IO
+        :type body: IO[bytes]
         :keyword authorization: Default value is None.
         :paramtype authorization: str
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def conversation(  # pylint: disable=inconsistent-return-statements
         self,
         body: Optional[
-            Union[_models.PathsLi5TynApiV1LogConversationPostRequestbodyContentApplicationJsonSchema, IO]
+            Union[_models.PathsLi5TynApiV1LogConversationPostRequestbodyContentApplicationJsonSchema, IO[bytes]]
         ] = None,
         *,
         authorization: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """Ingests a conversation.
 
         Ingests a conversation.
 
         :param body: Is either a
-         PathsLi5TynApiV1LogConversationPostRequestbodyContentApplicationJsonSchema type or a IO type.
-         Default value is None.
+         PathsLi5TynApiV1LogConversationPostRequestbodyContentApplicationJsonSchema type or a IO[bytes]
+         type. Default value is None.
         :type body:
          ~context_api.models.PathsLi5TynApiV1LogConversationPostRequestbodyContentApplicationJsonSchema
-         or IO
+         or IO[bytes]
         :keyword authorization: Default value is None.
         :paramtype authorization: str
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: None
         :rtype: None
@@ -1351,56 +1601,56 @@
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def conversation_upsert(  # pylint: disable=inconsistent-return-statements
         self,
-        body: Optional[IO] = None,
+        body: Optional[IO[bytes]] = None,
         *,
         authorization: Optional[str] = None,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> None:
         """Ingests or updates conversation.
 
         Ingests or updates conversation.
 
         :param body: Default value is None.
-        :type body: IO
+        :type body: IO[bytes]
         :keyword authorization: Default value is None.
         :paramtype authorization: str
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def conversation_upsert(  # pylint: disable=inconsistent-return-statements
         self,
         body: Optional[
-            Union[_models.PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema, IO]
+            Union[_models.PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema, IO[bytes]]
         ] = None,
         *,
         authorization: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """Ingests or updates conversation.
 
         Ingests or updates conversation.
 
         :param body: Is either a
-         PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema type or a IO
-         type. Default value is None.
+         PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema type or a
+         IO[bytes] type. Default value is None.
         :type body:
          ~context_api.models.PathsRai0VpApiV1LogConversationUpsertPostRequestbodyContentApplicationJsonSchema
-         or IO
+         or IO[bytes]
         :keyword authorization: Default value is None.
         :paramtype authorization: str
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: None
         :rtype: None
@@ -1487,26 +1737,26 @@
          ~context_api.models.PathsDo7Pm8ApiV1LogConversationThreadPostResponses201ContentApplicationJsonSchema
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def conversation_thread(
         self,
-        body: Optional[IO] = None,
+        body: Optional[IO[bytes]] = None,
         *,
         authorization: Optional[str] = None,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.PathsDo7Pm8ApiV1LogConversationThreadPostResponses201ContentApplicationJsonSchema:
         """Ingests or updates a thread.
 
         Ingests or updates a thread.
 
         :param body: Default value is None.
-        :type body: IO
+        :type body: IO[bytes]
         :keyword authorization: Default value is None.
         :paramtype authorization: str
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :return: PathsDo7Pm8ApiV1LogConversationThreadPostResponses201ContentApplicationJsonSchema
         :rtype:
@@ -1514,30 +1764,30 @@
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def conversation_thread(
         self,
         body: Optional[
-            Union[_models.Paths1S2Rf6XApiV1LogConversationThreadPostRequestbodyContentApplicationJsonSchema, IO]
+            Union[_models.Paths1S2Rf6XApiV1LogConversationThreadPostRequestbodyContentApplicationJsonSchema, IO[bytes]]
         ] = None,
         *,
         authorization: Optional[str] = None,
         **kwargs: Any
     ) -> _models.PathsDo7Pm8ApiV1LogConversationThreadPostResponses201ContentApplicationJsonSchema:
         """Ingests or updates a thread.
 
         Ingests or updates a thread.
 
         :param body: Is either a
-         Paths1S2Rf6XApiV1LogConversationThreadPostRequestbodyContentApplicationJsonSchema type or a IO
-         type. Default value is None.
+         Paths1S2Rf6XApiV1LogConversationThreadPostRequestbodyContentApplicationJsonSchema type or a
+         IO[bytes] type. Default value is None.
         :type body:
          ~context_api.models.Paths1S2Rf6XApiV1LogConversationThreadPostRequestbodyContentApplicationJsonSchema
-         or IO
+         or IO[bytes]
         :keyword authorization: Default value is None.
         :paramtype authorization: str
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: PathsDo7Pm8ApiV1LogConversationThreadPostResponses201ContentApplicationJsonSchema
         :rtype:
@@ -1634,27 +1884,27 @@
         :rtype: ~context_api.models.TestSetParams
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def test_sets(
         self,
-        body: Optional[IO] = None,
+        body: Optional[IO[bytes]] = None,
         *,
         authorization: Optional[str] = None,
         copy_test_cases_from: Optional[str] = None,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.TestSetParams:
         """Returns test set and version details.
 
         Returns test set and version details.
 
         :param body: Default value is None.
-        :type body: IO
+        :type body: IO[bytes]
         :keyword authorization: Default value is None.
         :paramtype authorization: str
         :keyword copy_test_cases_from: If none, all test cases will be replaced with the ones provided
          in the request.:code:`<br />`If prior_version, only the test cases with the same name will be
          replaced and new test cases will be appended.:code:`<br />`. Default value is None.
         :paramtype copy_test_cases_from: str
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
@@ -1664,26 +1914,26 @@
         :rtype: ~context_api.models.TestSetParams
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def test_sets(
         self,
-        body: Optional[Union[_models.TestSet, IO]] = None,
+        body: Optional[Union[_models.TestSet, IO[bytes]]] = None,
         *,
         authorization: Optional[str] = None,
         copy_test_cases_from: Optional[str] = None,
         **kwargs: Any
     ) -> _models.TestSetParams:
         """Returns test set and version details.
 
         Returns test set and version details.
 
-        :param body: Is either a TestSet type or a IO type. Default value is None.
-        :type body: ~context_api.models.TestSet or IO
+        :param body: Is either a TestSet type or a IO[bytes] type. Default value is None.
+        :type body: ~context_api.models.TestSet or IO[bytes]
         :keyword authorization: Default value is None.
         :paramtype authorization: str
         :keyword copy_test_cases_from: If none, all test cases will be replaced with the ones provided
          in the request.:code:`<br />`If prior_version, only the test cases with the same name will be
          replaced and new test cases will be appended.:code:`<br />`. Default value is None.
         :paramtype copy_test_cases_from: str
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
```

### Comparing `context_python-0.8.0/getcontext/generated/operations/_patch.py` & `context_python-0.9.0/getcontext/generated/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `context_python-0.8.0/getcontext/token.py` & `context_python-0.9.0/getcontext/token.py`

 * *Files identical despite different names*

### Comparing `context_python-0.8.0/pyproject.toml` & `context_python-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "context-python"
-version = "0.8.0"
+version = "0.9.0"
 description = "Python SDK for the Context API"
 authors = ["Alex Gamble <alex@context.ai>", "Alec Barber <alec@context.ai>", "Amisha Singh <amisha@context.ai>"]
 readme = "README.md"
 license = "LICENSE.md"
 keywords = ["context", "api", "sdk"]
 packages = [{include = "getcontext"}]
```

### Comparing `context_python-0.8.0/PKG-INFO` & `context_python-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: context-python
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python SDK for the Context API
 License: LICENSE.md
 Keywords: context,api,sdk
 Author: Alex Gamble
 Author-email: alex@context.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

