# Comparing `tmp/opentelemetry_resource_detector_azure-0.1.3.tar.gz` & `tmp/opentelemetry_resource_detector_azure-0.1.4.tar.gz`

## Comparing `opentelemetry_resource_detector_azure-0.1.3.tar` & `opentelemetry_resource_detector_azure-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.3/src/opentelemetry/resource/detector/azure/app_service.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.3/src/opentelemetry/resource/detector/azure/version.py
--rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.3/src/opentelemetry/resource/detector/azure/vm.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     6397 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.3/tests/test_app_service.py
--rw-r--r--   0        0        0    14123 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.3/tests/test_vm.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.3/.gitignore
--rw-r--r--   0        0        0    11551 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.3/LICENSE
--rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.3/README.rst
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4642 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.4/src/opentelemetry/resource/detector/azure/app_service.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.4/src/opentelemetry/resource/detector/azure/version.py
+-rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.4/src/opentelemetry/resource/detector/azure/vm.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     6397 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.4/tests/test_app_service.py
+-rw-r--r--   0        0        0    14075 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.4/tests/test_vm.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.4/.gitignore
+-rw-r--r--   0        0        0    11551 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.4/README.rst
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 opentelemetry_resource_detector_azure-0.1.4/PKG-INFO
```

### Comparing `opentelemetry_resource_detector_azure-0.1.3/src/opentelemetry/resource/detector/azure/app_service.py` & `opentelemetry_resource_detector_azure-0.1.4/src/opentelemetry/resource/detector/azure/app_service.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_resource_detector_azure-0.1.3/src/opentelemetry/resource/detector/azure/version.py` & `opentelemetry_resource_detector_azure-0.1.4/src/opentelemetry/resource/detector/azure/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
```

### Comparing `opentelemetry_resource_detector_azure-0.1.3/src/opentelemetry/resource/detector/azure/vm.py` & `opentelemetry_resource_detector_azure-0.1.4/src/opentelemetry/resource/detector/azure/vm.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,20 @@
 # limitations under the License.
 
 from json import loads
 from logging import getLogger
 from urllib.error import URLError
 from urllib.request import Request, urlopen
 
+from opentelemetry.context import (
+    _SUPPRESS_INSTRUMENTATION_KEY,
+    attach,
+    detach,
+    set_value,
+)
 from opentelemetry.sdk.resources import Resource, ResourceDetector
 from opentelemetry.semconv.resource import (
     CloudPlatformValues,
     CloudProviderValues,
     ResourceAttributes,
 )
 
@@ -45,68 +51,62 @@
 ]
 
 
 class AzureVMResourceDetector(ResourceDetector):
     # pylint: disable=no-self-use
     def detect(self) -> "Resource":
         attributes = {}
-        metadata_json = (
-            _AzureVMMetadataServiceRequestor().get_azure_vm_metadata()
-        )
+        token = attach(set_value(_SUPPRESS_INSTRUMENTATION_KEY, True))
+        metadata_json = _get_azure_vm_metadata()
         if not metadata_json:
             return Resource(attributes)
         for attribute_key in EXPECTED_AZURE_AMS_ATTRIBUTES:
-            attributes[
-                attribute_key
-            ] = _AzureVMMetadataServiceRequestor().get_attribute_from_metadata(
+            attributes[attribute_key] = _get_attribute_from_metadata(
                 metadata_json, attribute_key
             )
+        detach(token)
         return Resource(attributes)
 
 
-class _AzureVMMetadataServiceRequestor:
-    def get_azure_vm_metadata(self):  # pylint: disable=no-self-use
-        request = Request(_AZURE_VM_METADATA_ENDPOINT)
-        request.add_header("Metadata", "True")
-        try:
-            # TODO: Changed to 4s to fit into OTel SDK's 5 second timeout.
-            # Lengthen or allow user input if issue is resolved.
-            # See https://github.com/open-telemetry/opentelemetry-python/issues/3644
-            with urlopen(request, timeout=4) as response:
-                return loads(response.read())
-        except URLError:
-            # Not on Azure VM
-            return None
-        except Exception as e:  # pylint: disable=broad-except,invalid-name
-            _logger.exception("Failed to receive Azure VM metadata: %s", e)
-            return None
-
-    def get_attribute_from_metadata(
-        self, metadata_json, attribute_key
-    ):  # pylint: disable=no-self-use
-        ams_value = ""
-        if attribute_key == _AZURE_VM_SCALE_SET_NAME_ATTRIBUTE:
-            ams_value = metadata_json["vmScaleSetName"]
-        elif attribute_key == _AZURE_VM_SKU_ATTRIBUTE:
-            ams_value = metadata_json["sku"]
-        elif attribute_key == ResourceAttributes.CLOUD_PLATFORM:
-            ams_value = CloudPlatformValues.AZURE_VM.value
-        elif attribute_key == ResourceAttributes.CLOUD_PROVIDER:
-            ams_value = CloudProviderValues.AZURE.value
-        elif attribute_key == ResourceAttributes.CLOUD_REGION:
-            ams_value = metadata_json["location"]
-        elif attribute_key == ResourceAttributes.CLOUD_RESOURCE_ID:
-            ams_value = metadata_json["resourceId"]
-        elif attribute_key in (
-            ResourceAttributes.HOST_ID,
-            ResourceAttributes.SERVICE_INSTANCE_ID,
-        ):
-            ams_value = metadata_json["vmId"]
-        elif attribute_key == ResourceAttributes.HOST_NAME:
-            ams_value = metadata_json["name"]
-        elif attribute_key == ResourceAttributes.HOST_TYPE:
-            ams_value = metadata_json["vmSize"]
-        elif attribute_key == ResourceAttributes.OS_TYPE:
-            ams_value = metadata_json["osType"]
-        elif attribute_key == ResourceAttributes.OS_VERSION:
-            ams_value = metadata_json["version"]
-        return ams_value
+def _get_azure_vm_metadata():
+    request = Request(_AZURE_VM_METADATA_ENDPOINT)
+    request.add_header("Metadata", "True")
+    try:
+        # VM metadata service should not take more than 200ms on success case
+        with urlopen(request, timeout=0.2) as response:
+            return loads(response.read())
+    except URLError:
+        # Not on Azure VM
+        return None
+    except Exception as e:  # pylint: disable=broad-except,invalid-name
+        _logger.exception("Failed to receive Azure VM metadata: %s", e)
+        return None
+
+
+def _get_attribute_from_metadata(metadata_json, attribute_key):
+    ams_value = ""
+    if attribute_key == _AZURE_VM_SCALE_SET_NAME_ATTRIBUTE:
+        ams_value = metadata_json["vmScaleSetName"]
+    elif attribute_key == _AZURE_VM_SKU_ATTRIBUTE:
+        ams_value = metadata_json["sku"]
+    elif attribute_key == ResourceAttributes.CLOUD_PLATFORM:
+        ams_value = CloudPlatformValues.AZURE_VM.value
+    elif attribute_key == ResourceAttributes.CLOUD_PROVIDER:
+        ams_value = CloudProviderValues.AZURE.value
+    elif attribute_key == ResourceAttributes.CLOUD_REGION:
+        ams_value = metadata_json["location"]
+    elif attribute_key == ResourceAttributes.CLOUD_RESOURCE_ID:
+        ams_value = metadata_json["resourceId"]
+    elif attribute_key in (
+        ResourceAttributes.HOST_ID,
+        ResourceAttributes.SERVICE_INSTANCE_ID,
+    ):
+        ams_value = metadata_json["vmId"]
+    elif attribute_key == ResourceAttributes.HOST_NAME:
+        ams_value = metadata_json["name"]
+    elif attribute_key == ResourceAttributes.HOST_TYPE:
+        ams_value = metadata_json["vmSize"]
+    elif attribute_key == ResourceAttributes.OS_TYPE:
+        ams_value = metadata_json["osType"]
+    elif attribute_key == ResourceAttributes.OS_VERSION:
+        ams_value = metadata_json["version"]
+    return ams_value
```

### Comparing `opentelemetry_resource_detector_azure-0.1.3/tests/__init__.py` & `opentelemetry_resource_detector_azure-0.1.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_resource_detector_azure-0.1.3/tests/test_app_service.py` & `opentelemetry_resource_detector_azure-0.1.4/tests/test_app_service.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_resource_detector_azure-0.1.3/tests/test_vm.py` & `opentelemetry_resource_detector_azure-0.1.4/tests/test_vm.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import unittest
-from unittest.mock import Mock, patch
+from unittest.mock import patch
 
 # pylint: disable=no-name-in-module
 from opentelemetry.resource.detector.azure.vm import AzureVMResourceDetector
 
 LINUX_JSON = """
 {
     "additionalCapabilities": {
@@ -359,22 +359,22 @@
     "service.instance.id": "02aab8a4-74ef-476e-8182-f6d2ba4166a6",
 }
 
 
 class TestAzureVMResourceDetector(unittest.TestCase):
     @patch("opentelemetry.resource.detector.azure.vm.urlopen")
     def test_linux(self, mock_urlopen):
-        mock_response = Mock()
-        mock_urlopen.return_value = mock_response
-        mock_response.read.return_value = LINUX_JSON
+        mock_urlopen.return_value.__enter__.return_value.read.return_value = (
+            LINUX_JSON
+        )
         attributes = AzureVMResourceDetector().detect().attributes
         for attribute_key, attribute_value in LINUX_ATTRIBUTES.items():
             self.assertEqual(attributes[attribute_key], attribute_value)
 
     @patch("opentelemetry.resource.detector.azure.vm.urlopen")
     def test_windows(self, mock_urlopen):
-        mock_response = Mock()
-        mock_urlopen.return_value = mock_response
-        mock_response.read.return_value = WINDOWS_JSON
+        mock_urlopen.return_value.__enter__.return_value.read.return_value = (
+            WINDOWS_JSON
+        )
         attributes = AzureVMResourceDetector().detect().attributes
-        for attribute_key, attribute_value in LINUX_ATTRIBUTES.items():
+        for attribute_key, attribute_value in WINDOWS_ATTRIBUTES.items():
             self.assertEqual(attributes[attribute_key], attribute_value)
```

### Comparing `opentelemetry_resource_detector_azure-0.1.3/.gitignore` & `opentelemetry_resource_detector_azure-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `opentelemetry_resource_detector_azure-0.1.3/LICENSE` & `opentelemetry_resource_detector_azure-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_resource_detector_azure-0.1.3/README.rst` & `opentelemetry_resource_detector_azure-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_resource_detector_azure-0.1.3/pyproject.toml` & `opentelemetry_resource_detector_azure-0.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -4,37 +4,33 @@
 
 [project]
 name = "opentelemetry-resource-detector-azure"
 dynamic = ["version"]
 description = "Azure Resource Detector for OpenTelemetry"
 readme = "README.rst"
 license = "Apache-2.0"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 authors = [
   { name = "OpenTelemetry Authors", email = "cncf-opentelemetry-contributors@lists.cncf.io" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
   "opentelemetry-sdk ~= 1.21",
 ]
 
-[project.optional-dependencies]
-test = []
-
 [project.entry-points.opentelemetry_resource_detector]
 azure_app_service = "opentelemetry.resource.detector.azure.app_service:AzureAppServiceResourceDetector"
 azure_vm = "opentelemetry.resource.detector.azure.vm:AzureVMResourceDetector"
 
 [project.urls]
 Homepage = "https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/resource/opentelemetry-resource-detector-azure"
```

### Comparing `opentelemetry_resource_detector_azure-0.1.3/PKG-INFO` & `opentelemetry_resource_detector_azure-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: opentelemetry-resource-detector-azure
-Version: 0.1.3
+Version: 0.1.4
 Summary: Azure Resource Detector for OpenTelemetry
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/resource/opentelemetry-resource-detector-azure
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: opentelemetry-sdk~=1.21
-Provides-Extra: test
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Resource detectors for Azure
 ==========================================
 
 |pypi|
```

