# Comparing `tmp/ul-data-aggregator-sdk-9.5.2.tar.gz` & `tmp/ul-data-aggregator-sdk-9.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ul-data-aggregator-sdk-9.5.2.tar", last modified: Fri Apr  5 07:32:48 2024, max compression
+gzip compressed data, was "ul-data-aggregator-sdk-9.6.0.tar", last modified: Tue Mar 26 06:45:34 2024, max compression
```

## Comparing `ul-data-aggregator-sdk-9.5.2.tar` & `ul-data-aggregator-sdk-9.6.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 07:32:48.417692 ul-data-aggregator-sdk-9.5.2/
--rw-r--r--   0 root         (0) root         (0)     1603 2024-04-05 07:32:48.417692 ul-data-aggregator-sdk-9.5.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1038 2022-01-14 08:29:36.000000 ul-data-aggregator-sdk-9.5.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 07:32:48.417692 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-03-16 11:00:25.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 07:32:48.417692 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 07:32:42.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1161 2023-04-20 13:55:49.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/__tests__/test_integration_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 07:32:48.417692 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/brokers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 07:32:42.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/brokers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2022-07-04 09:50:04.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/brokers/data_aggregator_input_broker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 07:32:48.417692 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/constants/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 07:32:42.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/constants/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      297 2022-07-04 09:50:04.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/constants/annotations.py
--rw-rw-rw-   0 root         (0) root         (0)     3777 2023-03-29 07:59:52.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/constants/clock_timezones.py
--rw-rw-rw-   0 root         (0) root         (0)    49433 2024-04-04 07:36:55.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/constants/enums.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2022-07-04 09:50:04.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/constants/names.py
--rw-rw-rw-   0 root         (0) root         (0)      675 2022-08-05 17:06:54.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/dag.yml
--rw-rw-rw-   0 root         (0) root         (0)    83548 2024-04-04 07:36:55.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/data_aggregator_api_sdk.py
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-06-28 08:33:52.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/data_aggregator_api_sdk_config.py
--rw-rw-rw-   0 root         (0) root         (0)      826 2022-07-04 09:50:04.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/data_aggregator_sdk.py
--rw-rw-rw-   0 root         (0) root         (0)       95 2022-07-04 09:50:04.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/data_aggregator_sdk_config.py
--rw-rw-rw-   0 root         (0) root         (0)      991 2022-08-17 11:37:58.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/errors.py
--rw-rw-rw-   0 root         (0) root         (0)    45951 2024-03-07 08:32:02.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/integration_message.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-07-04 09:50:04.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/lib.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 07:32:42.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-07-04 09:50:04.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/runtime_conf.py
--rw-rw-rw-   0 root         (0) root         (0)      169 2022-08-03 16:22:45.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/self_logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 07:32:48.417692 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/types/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 07:32:42.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3200 2023-06-28 08:33:52.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/types/device.py
--rw-rw-rw-   0 root         (0) root         (0)     3401 2023-06-28 08:33:52.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/types/get_data_gateway_network_device_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 07:32:48.417692 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 07:32:42.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2022-07-04 09:50:04.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/utils/devices_info_box_to_json.py
--rw-rw-rw-   0 root         (0) root         (0)     1335 2023-06-28 08:33:52.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/utils/internal_api_error_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     1426 2023-06-28 08:33:52.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/utils/internal_api_error_handler_old.py
--rw-rw-rw-   0 root         (0) root         (0)      685 2022-08-03 16:22:45.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/utils/query_params.py
--rw-rw-rw-   0 root         (0) root         (0)      287 2023-09-06 12:40:42.000000 ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/utils/round_dt.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 07:32:48.417692 ul-data-aggregator-sdk-9.5.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1430 2024-04-04 07:43:00.000000 ul-data-aggregator-sdk-9.5.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 07:32:48.417692 ul-data-aggregator-sdk-9.5.2/ul_data_aggregator_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1603 2024-04-05 07:32:48.000000 ul-data-aggregator-sdk-9.5.2/ul_data_aggregator_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1544 2024-04-05 07:32:48.000000 ul-data-aggregator-sdk-9.5.2/ul_data_aggregator_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 07:32:48.000000 ul-data-aggregator-sdk-9.5.2/ul_data_aggregator_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2024-04-05 07:32:48.000000 ul-data-aggregator-sdk-9.5.2/ul_data_aggregator_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-04-05 07:32:48.000000 ul-data-aggregator-sdk-9.5.2/ul_data_aggregator_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 06:45:34.191981 ul-data-aggregator-sdk-9.6.0/
+-rw-r--r--   0 root         (0) root         (0)     1603 2024-03-26 06:45:34.191981 ul-data-aggregator-sdk-9.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1038 2022-01-14 08:30:24.000000 ul-data-aggregator-sdk-9.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 06:45:34.191981 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-03-16 13:49:41.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 06:45:34.191981 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-26 06:45:29.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1161 2023-04-20 16:17:36.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/__tests__/test_integration_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 06:45:34.191981 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/brokers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-26 06:45:29.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/brokers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      270 2022-07-04 09:51:07.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/brokers/data_aggregator_input_broker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 06:45:34.191981 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/constants/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-26 06:45:29.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/constants/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      297 2022-07-04 09:51:07.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/constants/annotations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3777 2023-04-10 10:54:47.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/constants/clock_timezones.py
+-rw-rw-rw-   0 root         (0) root         (0)    25573 2024-03-26 06:45:29.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/constants/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2022-07-04 09:51:07.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/constants/names.py
+-rw-rw-rw-   0 root         (0) root         (0)      675 2022-08-05 17:09:13.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/dag.yml
+-rw-rw-rw-   0 root         (0) root         (0)    83460 2024-03-26 06:45:29.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/data_aggregator_api_sdk.py
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-06-27 08:17:20.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/data_aggregator_api_sdk_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      826 2022-07-04 09:51:07.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/data_aggregator_sdk.py
+-rw-rw-rw-   0 root         (0) root         (0)       95 2022-07-04 09:51:07.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/data_aggregator_sdk_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      991 2022-08-17 10:55:03.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    45951 2024-03-07 08:32:17.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/integration_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2022-07-04 09:51:07.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-26 06:45:29.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-07-04 09:51:07.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/runtime_conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      169 2022-08-02 22:29:19.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/self_logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 06:45:34.191981 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/types/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-26 06:45:29.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3200 2023-06-27 08:17:20.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/types/device.py
+-rw-rw-rw-   0 root         (0) root         (0)     3401 2023-06-27 08:17:20.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/types/get_data_gateway_network_device_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 06:45:34.191981 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-26 06:45:29.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      257 2022-07-04 09:51:07.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/utils/devices_info_box_to_json.py
+-rw-rw-rw-   0 root         (0) root         (0)     1335 2023-06-27 08:17:20.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/utils/internal_api_error_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1426 2023-06-27 08:17:20.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/utils/internal_api_error_handler_old.py
+-rw-rw-rw-   0 root         (0) root         (0)      685 2022-08-02 22:29:19.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/utils/query_params.py
+-rw-rw-rw-   0 root         (0) root         (0)      287 2023-09-06 07:25:46.000000 ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/utils/round_dt.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-26 06:45:34.191981 ul-data-aggregator-sdk-9.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1430 2024-03-26 06:45:29.000000 ul-data-aggregator-sdk-9.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 06:45:34.191981 ul-data-aggregator-sdk-9.6.0/ul_data_aggregator_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1603 2024-03-26 06:45:34.000000 ul-data-aggregator-sdk-9.6.0/ul_data_aggregator_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1544 2024-03-26 06:45:34.000000 ul-data-aggregator-sdk-9.6.0/ul_data_aggregator_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 06:45:34.000000 ul-data-aggregator-sdk-9.6.0/ul_data_aggregator_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2024-03-26 06:45:34.000000 ul-data-aggregator-sdk-9.6.0/ul_data_aggregator_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-03-26 06:45:34.000000 ul-data-aggregator-sdk-9.6.0/ul_data_aggregator_sdk.egg-info/top_level.txt
```

### Comparing `ul-data-aggregator-sdk-9.5.2/PKG-INFO` & `ul-data-aggregator-sdk-9.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-data-aggregator-sdk
-Version: 9.5.2
+Version: 9.6.0
 Summary: Data aggregator sdk
 Author: Unic-lab
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ul-data-aggregator-sdk-9.5.2/README.md` & `ul-data-aggregator-sdk-9.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/__init__.py` & `ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/__tests__/test_integration_message.py` & `ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/__tests__/test_integration_message.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/constants/clock_timezones.py` & `ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/constants/clock_timezones.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/dag.yml` & `ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/dag.yml`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/data_aggregator_api_sdk.py` & `ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/data_aggregator_api_sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -615,16 +615,14 @@
     uplink_encryption_type: EncryptionType
     downlink_encryption_type: EncryptionType
 
 
 class ApiDataGatewayNetworkDeviceShortResponse(JsonApiResponsePayload):
     id: UUID4
     mac: int
-    downlink_encryption_key: Optional[str]
-    downlink_encryption_type: EncryptionType
 
 
 class ApiBSUplinkSignalResponse(JsonApiResponsePayload):
     id: UUID4
     date_created: datetime
     user_created_id: UUID4
```

### Comparing `ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/data_aggregator_sdk.py` & `ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/data_aggregator_sdk.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/errors.py` & `ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/errors.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/integration_message.py` & `ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/integration_message.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/types/device.py` & `ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/types/device.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/types/get_data_gateway_network_device_list.py` & `ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/types/get_data_gateway_network_device_list.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/utils/internal_api_error_handler.py` & `ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/utils/internal_api_error_handler.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/utils/internal_api_error_handler_old.py` & `ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/utils/internal_api_error_handler_old.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-9.5.2/data_aggregator_sdk/utils/query_params.py` & `ul-data-aggregator-sdk-9.6.0/data_aggregator_sdk/utils/query_params.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-9.5.2/setup.py` & `ul-data-aggregator-sdk-9.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='ul-data-aggregator-sdk',
-    version='9.5.2',
+    version='9.6.0',
     description='Data aggregator sdk',
     author='Unic-lab',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_data={
         '': ['*.yml'],
         'data_aggregator_sdk': ['py.typed'],
@@ -34,15 +34,15 @@
     platforms='any',
     install_requires=[
         'requests>=2.26.0',
         'unipipeline>=1.4.3',
         'ul-api-utils>=7.3.4',
         'wtforms==3.0.1',
         'wtforms-alchemy==0.18.0',
-        # "ul-api-utils==7.8.4",
+        # "ul-api-utils==7.8.2",
         # 'ul-pyncp==1.0.5',
         # 'ul-pysmp==1.0.3',
         # 'ul-data-gateway-sdk==0.4.11',
         # 'ul-py-tool==1.15.42',
         # 'ul-db-utils==3.0.1'
     ],
 )
```

### Comparing `ul-data-aggregator-sdk-9.5.2/ul_data_aggregator_sdk.egg-info/PKG-INFO` & `ul-data-aggregator-sdk-9.6.0/ul_data_aggregator_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-data-aggregator-sdk
-Version: 9.5.2
+Version: 9.6.0
 Summary: Data aggregator sdk
 Author: Unic-lab
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ul-data-aggregator-sdk-9.5.2/ul_data_aggregator_sdk.egg-info/SOURCES.txt` & `ul-data-aggregator-sdk-9.6.0/ul_data_aggregator_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

