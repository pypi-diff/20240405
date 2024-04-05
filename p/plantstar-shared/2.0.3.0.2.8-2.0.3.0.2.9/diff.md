# Comparing `tmp/plantstar-shared-2.0.3.0.2.8.tar.gz` & `tmp/plantstar-shared-2.0.3.0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plantstar-shared-2.0.3.0.2.8.tar", last modified: Thu Jan 18 07:01:13 2024, max compression
+gzip compressed data, was "plantstar-shared-2.0.3.0.2.9.tar", last modified: Wed Feb 28 19:27:10 2024, max compression
```

## Comparing `plantstar-shared-2.0.3.0.2.8.tar` & `plantstar-shared-2.0.3.0.2.9.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 07:01:13.201108 plantstar-shared-2.0.3.0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-01-18 07:01:13.201108 plantstar-shared-2.0.3.0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-18 07:00:59.000000 plantstar-shared-2.0.3.0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 07:01:13.201108 plantstar-shared-2.0.3.0.2.8/plantstar_shared/
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-01-18 07:00:59.000000 plantstar-shared-2.0.3.0.2.8/plantstar_shared/DataCollectionModuleProcessNames.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-01-18 07:00:59.000000 plantstar-shared-2.0.3.0.2.8/plantstar_shared/HuskyInterfacePacketTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-01-18 07:00:59.000000 plantstar-shared-2.0.3.0.2.8/plantstar_shared/MockRawDataProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-01-18 07:00:59.000000 plantstar-shared-2.0.3.0.2.8/plantstar_shared/RawDataProcessorInterfaceActions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-01-18 07:00:59.000000 plantstar-shared-2.0.3.0.2.8/plantstar_shared/SysconType.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 07:00:59.000000 plantstar-shared-2.0.3.0.2.8/plantstar_shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-01-18 07:00:59.000000 plantstar-shared-2.0.3.0.2.8/plantstar_shared/add_size_onto_string_and_return.py
--rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-01-18 07:00:59.000000 plantstar-shared-2.0.3.0.2.8/plantstar_shared/api_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-01-18 07:00:59.000000 plantstar-shared-2.0.3.0.2.8/plantstar_shared/convert_bytes_to_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-01-18 07:00:59.000000 plantstar-shared-2.0.3.0.2.8/plantstar_shared/convert_object_to_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-01-18 07:00:59.000000 plantstar-shared-2.0.3.0.2.8/plantstar_shared/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-01-18 07:00:59.000000 plantstar-shared-2.0.3.0.2.8/plantstar_shared/global_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-01-18 07:00:59.000000 plantstar-shared-2.0.3.0.2.8/plantstar_shared/is_valid_signed_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-01-18 07:00:59.000000 plantstar-shared-2.0.3.0.2.8/plantstar_shared/obtain_raw_data_processor_function_for_action_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-01-18 07:00:59.000000 plantstar-shared-2.0.3.0.2.8/plantstar_shared/syscon_image_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-01-18 07:00:59.000000 plantstar-shared-2.0.3.0.2.8/plantstar_shared/syscon_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-01-18 07:00:59.000000 plantstar-shared-2.0.3.0.2.8/plantstar_shared/tcp_socket_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 07:01:13.201108 plantstar-shared-2.0.3.0.2.8/plantstar_shared.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-01-18 07:01:13.000000 plantstar-shared-2.0.3.0.2.8/plantstar_shared.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-01-18 07:01:13.000000 plantstar-shared-2.0.3.0.2.8/plantstar_shared.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 07:01:13.000000 plantstar-shared-2.0.3.0.2.8/plantstar_shared.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-01-18 07:01:13.000000 plantstar-shared-2.0.3.0.2.8/plantstar_shared.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-18 07:01:13.000000 plantstar-shared-2.0.3.0.2.8/plantstar_shared.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 07:01:13.201108 plantstar-shared-2.0.3.0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-01-18 07:00:59.000000 plantstar-shared-2.0.3.0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:27:10.273219 plantstar-shared-2.0.3.0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-28 19:27:10.273219 plantstar-shared-2.0.3.0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-28 19:27:00.000000 plantstar-shared-2.0.3.0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:27:10.269219 plantstar-shared-2.0.3.0.2.9/plantstar_shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-02-28 19:27:00.000000 plantstar-shared-2.0.3.0.2.9/plantstar_shared/DataCollectionModuleProcessNames.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-02-28 19:27:00.000000 plantstar-shared-2.0.3.0.2.9/plantstar_shared/HmiKeyConstants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-02-28 19:27:00.000000 plantstar-shared-2.0.3.0.2.9/plantstar_shared/HuskyInterfacePacketTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-02-28 19:27:00.000000 plantstar-shared-2.0.3.0.2.9/plantstar_shared/MockRawDataProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-02-28 19:27:00.000000 plantstar-shared-2.0.3.0.2.9/plantstar_shared/RawDataProcessorInterfaceActions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-02-28 19:27:00.000000 plantstar-shared-2.0.3.0.2.9/plantstar_shared/SysconType.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 19:27:00.000000 plantstar-shared-2.0.3.0.2.9/plantstar_shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-02-28 19:27:00.000000 plantstar-shared-2.0.3.0.2.9/plantstar_shared/add_size_onto_string_and_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-02-28 19:27:00.000000 plantstar-shared-2.0.3.0.2.9/plantstar_shared/api_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-02-28 19:27:00.000000 plantstar-shared-2.0.3.0.2.9/plantstar_shared/convert_bytes_to_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-28 19:27:00.000000 plantstar-shared-2.0.3.0.2.9/plantstar_shared/convert_object_to_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-02-28 19:27:00.000000 plantstar-shared-2.0.3.0.2.9/plantstar_shared/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-02-28 19:27:00.000000 plantstar-shared-2.0.3.0.2.9/plantstar_shared/global_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-28 19:27:00.000000 plantstar-shared-2.0.3.0.2.9/plantstar_shared/is_valid_signed_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-02-28 19:27:00.000000 plantstar-shared-2.0.3.0.2.9/plantstar_shared/obtain_raw_data_processor_function_for_action_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-02-28 19:27:00.000000 plantstar-shared-2.0.3.0.2.9/plantstar_shared/syscon_image_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-02-28 19:27:00.000000 plantstar-shared-2.0.3.0.2.9/plantstar_shared/syscon_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-02-28 19:27:00.000000 plantstar-shared-2.0.3.0.2.9/plantstar_shared/tcp_socket_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:27:10.273219 plantstar-shared-2.0.3.0.2.9/plantstar_shared.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-28 19:27:10.000000 plantstar-shared-2.0.3.0.2.9/plantstar_shared.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-02-28 19:27:10.000000 plantstar-shared-2.0.3.0.2.9/plantstar_shared.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 19:27:10.000000 plantstar-shared-2.0.3.0.2.9/plantstar_shared.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-28 19:27:10.000000 plantstar-shared-2.0.3.0.2.9/plantstar_shared.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-28 19:27:10.000000 plantstar-shared-2.0.3.0.2.9/plantstar_shared.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 19:27:10.273219 plantstar-shared-2.0.3.0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-02-28 19:27:00.000000 plantstar-shared-2.0.3.0.2.9/setup.py
```

### Comparing `plantstar-shared-2.0.3.0.2.8/PKG-INFO` & `plantstar-shared-2.0.3.0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plantstar-shared
-Version: 2.0.3.0.2.8
+Version: 2.0.3.0.2.9
 Summary: Shared code used in plantstar_apu and plantstar_dcm
 Home-page: https://github.com/SYSCON-International/plantstar_shared
 Author: SYSCON International
 Author-email: dev@syscon-intl.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `plantstar-shared-2.0.3.0.2.8/plantstar_shared/HuskyInterfacePacketTypes.py` & `plantstar-shared-2.0.3.0.2.9/plantstar_shared/HuskyInterfacePacketTypes.py`

 * *Files identical despite different names*

### Comparing `plantstar-shared-2.0.3.0.2.8/plantstar_shared/MockRawDataProcessor.py` & `plantstar-shared-2.0.3.0.2.9/plantstar_shared/MockRawDataProcessor.py`

 * *Files identical despite different names*

### Comparing `plantstar-shared-2.0.3.0.2.8/plantstar_shared/RawDataProcessorInterfaceActions.py` & `plantstar-shared-2.0.3.0.2.9/plantstar_shared/RawDataProcessorInterfaceActions.py`

 * *Files identical despite different names*

### Comparing `plantstar-shared-2.0.3.0.2.8/plantstar_shared/SysconType.py` & `plantstar-shared-2.0.3.0.2.9/plantstar_shared/SysconType.py`

 * *Files identical despite different names*

### Comparing `plantstar-shared-2.0.3.0.2.8/plantstar_shared/api_types.py` & `plantstar-shared-2.0.3.0.2.9/plantstar_shared/api_types.py`

 * *Files 14% similar despite different names*

```diff
@@ -97,7 +97,14 @@
 class ApuApiTypes(SysconType):
     SET_IS_INITIALIZING_STATUS = ("data_collection_module_manager/set_is_initializing_status", "data_collection_module_manager/set_is_initializing_status", True)
     SET_IS_COLDBOOTING_STATUS = ("data_collection_module_manager/set_is_coldbooting_status", "data_collection_module_manager/set_is_coldbooting_status", True)
 
 
 class CosmosApiTypes(SysconType):
     SEND_DATA_DICTIONARY = ("send_data_dictionary", "send_data_dictionary", True)
+
+
+class HmiApiTypes(SysconType):
+    GET_HMI_SYSTEM_INFORMATION = ("get_hmi_system_information", "get_hmi_system_information", True)
+    SET_HMI_SYSTEM_INFORMATION = ("set_hmi_system_information", "set_hmi_system_information", True)
+    REBOOT_HMI = ("reboot_hmi", "reboot_hmi", True)
+
```

### Comparing `plantstar-shared-2.0.3.0.2.8/plantstar_shared/global_definitions.py` & `plantstar-shared-2.0.3.0.2.9/plantstar_shared/global_definitions.py`

 * *Files identical despite different names*

### Comparing `plantstar-shared-2.0.3.0.2.8/plantstar_shared/obtain_raw_data_processor_function_for_action_name.py` & `plantstar-shared-2.0.3.0.2.9/plantstar_shared/obtain_raw_data_processor_function_for_action_name.py`

 * *Files identical despite different names*

### Comparing `plantstar-shared-2.0.3.0.2.8/plantstar_shared/syscon_json.py` & `plantstar-shared-2.0.3.0.2.9/plantstar_shared/syscon_json.py`

 * *Files identical despite different names*

### Comparing `plantstar-shared-2.0.3.0.2.8/plantstar_shared/tcp_socket_utils.py` & `plantstar-shared-2.0.3.0.2.9/plantstar_shared/tcp_socket_utils.py`

 * *Files identical despite different names*

### Comparing `plantstar-shared-2.0.3.0.2.8/plantstar_shared.egg-info/PKG-INFO` & `plantstar-shared-2.0.3.0.2.9/plantstar_shared.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plantstar-shared
-Version: 2.0.3.0.2.8
+Version: 2.0.3.0.2.9
 Summary: Shared code used in plantstar_apu and plantstar_dcm
 Home-page: https://github.com/SYSCON-International/plantstar_shared
 Author: SYSCON International
 Author-email: dev@syscon-intl.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `plantstar-shared-2.0.3.0.2.8/plantstar_shared.egg-info/SOURCES.txt` & `plantstar-shared-2.0.3.0.2.9/plantstar_shared.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.md
 setup.py
 plantstar_shared/DataCollectionModuleProcessNames.py
+plantstar_shared/HmiKeyConstants.py
 plantstar_shared/HuskyInterfacePacketTypes.py
 plantstar_shared/MockRawDataProcessor.py
 plantstar_shared/RawDataProcessorInterfaceActions.py
 plantstar_shared/SysconType.py
 plantstar_shared/__init__.py
 plantstar_shared/add_size_onto_string_and_return.py
 plantstar_shared/api_types.py
```

### Comparing `plantstar-shared-2.0.3.0.2.8/setup.py` & `plantstar-shared-2.0.3.0.2.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as file_handle:
     long_description = file_handle.read()
 
 setuptools.setup(
     name="plantstar-shared",
     # MAJOR_MILESTONE_VERSION.MINOR_MILESTONE_VERSION.MAJOR_VERSION.MINOR_VERSION.HOTFIX_VERSION.SUBVERSION
     # The main version should stay as v2.0.3.0.x until we have passed that in the plantstar_apu/plantstar_dcm projects
-    version="2.0.3.0.2.8",
+    version="2.0.3.0.2.9",
     author="SYSCON International",
     author_email="dev@syscon-intl.com",
     description="Shared code used in plantstar_apu and plantstar_dcm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SYSCON-International/plantstar_shared",
     packages=setuptools.find_packages(),
```

