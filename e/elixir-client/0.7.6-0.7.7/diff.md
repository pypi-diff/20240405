# Comparing `tmp/elixir-client-0.7.6.tar.gz` & `tmp/elixir-client-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elixir-client-0.7.6.tar", last modified: Thu Mar 14 01:41:04 2024, max compression
+gzip compressed data, was "elixir-client-0.7.7.tar", last modified: Fri Apr  5 00:02:55 2024, max compression
```

## Comparing `elixir-client-0.7.6.tar` & `elixir-client-0.7.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-03-14 01:41:04.743939 elixir-client-0.7.6/
--rw-r--r--   0 stevehiehn   (501) staff       (20)    35140 2024-03-13 21:22:47.000000 elixir-client-0.7.6/LICENSE.md
--rw-r--r--   0 stevehiehn   (501) staff       (20)     6252 2024-03-14 01:41:04.743733 elixir-client-0.7.6/PKG-INFO
--rw-r--r--   0 stevehiehn   (501) staff       (20)     5888 2024-03-14 01:39:16.000000 elixir-client-0.7.6/README.md
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-03-14 01:41:04.740624 elixir-client-0.7.6/elixir_client/
--rw-r--r--   0 stevehiehn   (501) staff       (20)      558 2024-03-13 21:22:47.000000 elixir-client-0.7.6/elixir_client/__init__.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)      537 2024-03-13 21:22:47.000000 elixir-client-0.7.6/elixir_client/config.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)    30384 2024-03-13 21:22:47.000000 elixir-client-0.7.6/elixir_client/core.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)      277 2024-03-13 21:22:47.000000 elixir-client-0.7.6/elixir_client/decorators.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     4446 2024-03-13 21:22:47.000000 elixir-client-0.7.6/elixir_client/dn_tracer.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     1404 2024-03-13 21:22:47.000000 elixir-client-0.7.6/elixir_client/file_uploader.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-03-14 01:41:04.741784 elixir-client-0.7.6/elixir_client/output/
--rw-r--r--   0 stevehiehn   (501) staff       (20)       63 2024-03-13 21:22:47.000000 elixir-client-0.7.6/elixir_client/output/__init__.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     6412 2024-03-13 21:22:47.000000 elixir-client-0.7.6/elixir_client/output/results_handler.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-03-14 01:41:04.742293 elixir-client-0.7.6/elixir_client/utils/
--rw-r--r--   0 stevehiehn   (501) staff       (20)       61 2024-03-13 21:22:47.000000 elixir-client-0.7.6/elixir_client/utils/__init__.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     3060 2024-03-13 21:22:47.000000 elixir-client-0.7.6/elixir_client/utils/audio_utils.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)      572 2024-03-13 21:22:47.000000 elixir-client-0.7.6/elixir_client/utils/file_type_classifier.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-03-14 01:41:04.741476 elixir-client-0.7.6/elixir_client.egg-info/
--rw-r--r--   0 stevehiehn   (501) staff       (20)     6252 2024-03-14 01:41:04.000000 elixir-client-0.7.6/elixir_client.egg-info/PKG-INFO
--rw-r--r--   0 stevehiehn   (501) staff       (20)      715 2024-03-14 01:41:04.000000 elixir-client-0.7.6/elixir_client.egg-info/SOURCES.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)        1 2024-03-14 01:41:04.000000 elixir-client-0.7.6/elixir_client.egg-info/dependency_links.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       58 2024-03-14 01:41:04.000000 elixir-client-0.7.6/elixir_client.egg-info/entry_points.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       72 2024-03-14 01:41:04.000000 elixir-client-0.7.6/elixir_client.egg-info/requires.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       20 2024-03-14 01:41:04.000000 elixir-client-0.7.6/elixir_client.egg-info/top_level.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       38 2024-03-14 01:41:04.743975 elixir-client-0.7.6/setup.cfg
--rw-r--r--   0 stevehiehn   (501) staff       (20)     1560 2024-03-14 01:39:16.000000 elixir-client-0.7.6/setup.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-03-14 01:41:04.743430 elixir-client-0.7.6/tests/
--rw-r--r--   0 stevehiehn   (501) staff       (20)        0 2024-03-13 21:22:47.000000 elixir-client-0.7.6/tests/__init__.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     5372 2024-03-13 21:50:56.000000 elixir-client-0.7.6/tests/test_audio_utils.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     6956 2024-03-13 21:50:43.000000 elixir-client-0.7.6/tests/test_core.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)    13192 2024-03-13 21:50:43.000000 elixir-client-0.7.6/tests/test_registration.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)      683 2024-03-13 21:50:56.000000 elixir-client-0.7.6/tests/test_results_handler.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-05 00:02:55.688419 elixir-client-0.7.7/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    35140 2024-03-13 21:22:47.000000 elixir-client-0.7.7/LICENSE.md
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     6144 2024-04-05 00:02:55.688290 elixir-client-0.7.7/PKG-INFO
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     5780 2024-04-04 23:51:24.000000 elixir-client-0.7.7/README.md
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-05 00:02:55.685174 elixir-client-0.7.7/elixir_client/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      558 2024-03-13 21:22:47.000000 elixir-client-0.7.7/elixir_client/__init__.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      559 2024-03-18 00:34:15.000000 elixir-client-0.7.7/elixir_client/config.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    30699 2024-04-04 23:51:24.000000 elixir-client-0.7.7/elixir_client/core.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      277 2024-03-13 21:22:47.000000 elixir-client-0.7.7/elixir_client/decorators.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     4446 2024-03-13 21:22:47.000000 elixir-client-0.7.7/elixir_client/dn_tracer.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     1404 2024-03-13 21:22:47.000000 elixir-client-0.7.7/elixir_client/file_uploader.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-05 00:02:55.686279 elixir-client-0.7.7/elixir_client/output/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       63 2024-03-13 21:22:47.000000 elixir-client-0.7.7/elixir_client/output/__init__.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     6412 2024-03-13 21:22:47.000000 elixir-client-0.7.7/elixir_client/output/results_handler.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-05 00:02:55.686769 elixir-client-0.7.7/elixir_client/utils/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       61 2024-03-13 21:22:47.000000 elixir-client-0.7.7/elixir_client/utils/__init__.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     3060 2024-03-13 21:22:47.000000 elixir-client-0.7.7/elixir_client/utils/audio_utils.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      572 2024-03-13 21:22:47.000000 elixir-client-0.7.7/elixir_client/utils/file_type_classifier.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-05 00:02:55.685989 elixir-client-0.7.7/elixir_client.egg-info/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     6144 2024-04-05 00:02:55.000000 elixir-client-0.7.7/elixir_client.egg-info/PKG-INFO
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      715 2024-04-05 00:02:55.000000 elixir-client-0.7.7/elixir_client.egg-info/SOURCES.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)        1 2024-04-05 00:02:55.000000 elixir-client-0.7.7/elixir_client.egg-info/dependency_links.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       58 2024-04-05 00:02:55.000000 elixir-client-0.7.7/elixir_client.egg-info/entry_points.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       72 2024-04-05 00:02:55.000000 elixir-client-0.7.7/elixir_client.egg-info/requires.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       20 2024-04-05 00:02:55.000000 elixir-client-0.7.7/elixir_client.egg-info/top_level.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       38 2024-04-05 00:02:55.688459 elixir-client-0.7.7/setup.cfg
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     1560 2024-04-04 23:51:24.000000 elixir-client-0.7.7/setup.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-05 00:02:55.688012 elixir-client-0.7.7/tests/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)        0 2024-03-13 21:22:47.000000 elixir-client-0.7.7/tests/__init__.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     5372 2024-03-13 21:50:56.000000 elixir-client-0.7.7/tests/test_audio_utils.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     6956 2024-03-13 21:50:43.000000 elixir-client-0.7.7/tests/test_core.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    13192 2024-03-13 21:50:43.000000 elixir-client-0.7.7/tests/test_registration.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      683 2024-03-13 21:50:56.000000 elixir-client-0.7.7/tests/test_results_handler.py
```

### Comparing `elixir-client-0.7.6/LICENSE.md` & `elixir-client-0.7.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `elixir-client-0.7.6/PKG-INFO` & `elixir-client-0.7.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,20 @@
-Metadata-Version: 2.1
-Name: elixir-client
-Version: 0.7.6
-Summary: Elixir client enables remote execution of python code triggered from a Crucible Plugin on the Signals & Sorcery platform.
-Home-page: https://dawnet.tools
-Author: Steve Hiehn
-Author-email: stevehiehn@gmail.com
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
+# Signals & Sorcery
 
-# Elixir Client
-
-`DAWNet` is a DAW (digit audio workstation) plugin that connects to a remote Google Colab or Script.  A user can send audio files from the plugin for remote processing. Hence, perform computationally expensive tasks such as text-2-audio or stem separation without leaving the DAW. 
+Signals & Socery is a platform for that connects Elixir AIs to Crucible plugins.
 
 For more information:
 
-- [https://dawnet.tools/](https://dawnet.tools/)
+- [Signals & Sorcery DOCS](https://signalsandsorcery.com/)
 
 - [Community Discord](https://discord.gg/UcHCjfpRkV)
 
 # elixir-client
 
-The `DAWNet client` (this repo) is a python3 pip package.  It is used to create `DAWNet remotes`.  The client is responsible for moving data and files backand forth from the plugin (and server).   The client allows a user to register python functions with the DAWNet discovery server. After a function has been registered it can then be triggered remotely from `DAWNet plugin.   
-
-::: warning
-NOTE: The plugin is in an active, pre-alpha state.  It has only been tested on Ableton 11 on MAC M1.
-:::
+The Elixir Client (this repo) is a python3 pip package.  It is used to create Elixir AIs.  Elixir AIs are [Jupyter Notebooks](https://jupyter.org/) scripted using the elixir client and packaged as containers. The client is responsible for moving data and files backand forth from the plugin (and server).   The client allows a user to register python functions with the Signals & Sorcery discovery server. After a function has been registered it can then be triggered remotely from any of the [Crucible plugins](https://signalsandsorcery.com/crucible-plugins/).   
 
 ## Installation
 
 ```python
 pip install elixir-client --upgrade
 ```
 
@@ -116,15 +101,15 @@
 
 
 ## CONFIGURATION:
 
 *Note:* If the following environment variables are not set, the client will use the default values.  The default values will point to the public DAWNet server.  If you wish to host your own instance you will need to configure the following environment variables. 
 
 ```
-export DN_CLIENT_API_BASE_URL='http://localhost:8081'
+export DN_CLIENT_API_BASE_URL='https://signalsandsorceryapi.com/'
 export DN_CLIENT_SOCKET_IP='0.0.0.0'
 export DN_CLIENT_SOCKET_PORT='8765'
 export DN_CLIENT_SENTRY_API_KEY='XXX'
 "DN_CLIENT_STORAGE_BUCKET", "https://storage.googleapis.com/your_gcp_bucket/"
 ```
 
 *Note:* If the env var `DN_CLIENT_TOKEN` is set it will override the set_token() function.
```

### Comparing `elixir-client-0.7.6/README.md` & `elixir-client-0.7.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,31 @@
-# Elixir Client
+Metadata-Version: 2.1
+Name: elixir-client
+Version: 0.7.7
+Summary: Elixir client enables remote execution of python code triggered from a Crucible Plugin on the Signals & Sorcery platform.
+Home-page: https://dawnet.tools
+Author: Steve Hiehn
+Author-email: stevehiehn@gmail.com
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
 
-`DAWNet` is a DAW (digit audio workstation) plugin that connects to a remote Google Colab or Script.  A user can send audio files from the plugin for remote processing. Hence, perform computationally expensive tasks such as text-2-audio or stem separation without leaving the DAW. 
+# Signals & Sorcery
+
+Signals & Socery is a platform for that connects Elixir AIs to Crucible plugins.
 
 For more information:
 
-- [https://dawnet.tools/](https://dawnet.tools/)
+- [Signals & Sorcery DOCS](https://signalsandsorcery.com/)
 
 - [Community Discord](https://discord.gg/UcHCjfpRkV)
 
 # elixir-client
 
-The `DAWNet client` (this repo) is a python3 pip package.  It is used to create `DAWNet remotes`.  The client is responsible for moving data and files backand forth from the plugin (and server).   The client allows a user to register python functions with the DAWNet discovery server. After a function has been registered it can then be triggered remotely from `DAWNet plugin.   
-
-::: warning
-NOTE: The plugin is in an active, pre-alpha state.  It has only been tested on Ableton 11 on MAC M1.
-:::
+The Elixir Client (this repo) is a python3 pip package.  It is used to create Elixir AIs.  Elixir AIs are [Jupyter Notebooks](https://jupyter.org/) scripted using the elixir client and packaged as containers. The client is responsible for moving data and files backand forth from the plugin (and server).   The client allows a user to register python functions with the Signals & Sorcery discovery server. After a function has been registered it can then be triggered remotely from any of the [Crucible plugins](https://signalsandsorcery.com/crucible-plugins/).   
 
 ## Installation
 
 ```python
 pip install elixir-client --upgrade
 ```
 
@@ -105,15 +112,15 @@
 
 
 ## CONFIGURATION:
 
 *Note:* If the following environment variables are not set, the client will use the default values.  The default values will point to the public DAWNet server.  If you wish to host your own instance you will need to configure the following environment variables. 
 
 ```
-export DN_CLIENT_API_BASE_URL='http://localhost:8081'
+export DN_CLIENT_API_BASE_URL='https://signalsandsorceryapi.com/'
 export DN_CLIENT_SOCKET_IP='0.0.0.0'
 export DN_CLIENT_SOCKET_PORT='8765'
 export DN_CLIENT_SENTRY_API_KEY='XXX'
 "DN_CLIENT_STORAGE_BUCKET", "https://storage.googleapis.com/your_gcp_bucket/"
 ```
 
 *Note:* If the env var `DN_CLIENT_TOKEN` is set it will override the set_token() function.
```

### Comparing `elixir-client-0.7.6/elixir_client/__init__.py` & `elixir-client-0.7.7/elixir_client/__init__.py`

 * *Files identical despite different names*

### Comparing `elixir-client-0.7.6/elixir_client/config.py` & `elixir-client-0.7.7/elixir_client/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import os
 
 # --------- PRODUCTION SETTINGS ----------------
-SOCKET_IP = os.getenv("DN_CLIENT_SOCKET_IP", "34.135.228.111")
-API_BASE_URL = os.getenv("DN_CLIENT_API_BASE_URL", "http://34.135.228.111:8081")
+SOCKET_IP = os.getenv("DN_CLIENT_SOCKET_IP", "signalsandsorceryapi.com")
+API_BASE_URL = os.getenv("DN_CLIENT_API_BASE_URL", "https://signalsandsorceryapi.com")
 SENTRY_API_KEY = os.getenv(
     "DN_CLIENT_SENTRY_API_KEY",
     "https://dbbf2855a707e0448957ad77111449c3@o4506379662131200.ingest.sentry.io/4506379670847488",
 )
 SOCKET_PORT = os.getenv("DN_CLIENT_SOCKET_PORT", "8765")
-STORAGE_BUCKET_PATH = os.getenv("DN_CLIENT_STORAGE_BUCKET", "https://storage.googleapis.com/byoc-file-transfer/")
+STORAGE_BUCKET_PATH = os.getenv(
+    "DN_CLIENT_STORAGE_BUCKET", "https://storage.googleapis.com/byoc-file-transfer/"
+)
```

### Comparing `elixir-client-0.7.6/elixir_client/core.py` & `elixir-client-0.7.7/elixir_client/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,18 +310,23 @@
 
         method_name = method.__name__
         params = await self.validate_and_process_parameters(method)
         method_details = self.create_json_payload(method_name, params)
         self.method_details[method_name] = method_details
         self.method_registry = {method_name: method}
 
-        #TODO: there should be a better way to do this:
+        # TODO: there should be a better way to do this:
         self.dawnet_token = self.generate_uuid(
-            str(method_details) + str(self.master_token) + str(self.name) + str(self.version) + str(self.author) + str(
-                self.description))
+            str(method_details)
+            + str(self.master_token)
+            + str(self.name)
+            + str(self.version)
+            + str(self.author)
+            + str(self.description)
+        )
 
         await self.connect()  # Ensure we're connected
 
         self.dn_tracer.log_event(
             self.dawnet_token,
             {
                 DNTag.DNMsgStage.value: DNMsgStage.CLIENT_REG_METHOD.value,
@@ -421,15 +426,15 @@
     async def download_gcp_files(self, obj, session):
         """
         Recursively search for GCP URLs in a JSON object and download the files.
         """
         if isinstance(obj, dict):
             for key, value in obj.items():
                 if isinstance(value, str) and value.startswith(
-                        "https://storage.googleapis.com"
+                    "https://storage.googleapis.com"
                 ):
                     # Download and replace the URL with a local file path
                     try:
                         obj[key] = await self.download_file(value, session)
 
                         self.dn_tracer.log_event(
                             self.dawnet_token,
@@ -530,16 +535,18 @@
                             _client.dawnet_token,
                             {
                                 DNTag.DNMsgStage.value: DNMsgStage.CLIENT_DOWNLOAD_ASSET.value,
                                 DNTag.DNMsg.value: f"Error downloading GCP files: {e}",
                             },
                         )
 
-                    if 'type' in msg:
+                    if "type" in msg:
+                        print("HANDLE MSG TYPE: " + str(msg))
                         if msg["type"] == "run_method":
+                            print("RUN METHOD RECEIVED")
                             # Check if the status is already "running"
                             if run_status.status == "running":
                                 await self.websocket.send("Plugin already started!")
                             else:
                                 self.results.clear_outputs()  # Clear previous outputs before running the method
                                 self.message_id = msg["message_id"]
                                 self.results.set_message_id(self.message_id)
@@ -547,20 +554,24 @@
                                 self.daw_sample_rate = msg["sample_rate"]
 
                                 data = msg["data"]
                                 method_name = data["method_name"]
                                 # Extract 'value' for each parameter to build kwargs
                                 params = {
                                     param_name: param_details["value"]
-                                    for param_name, param_details in data["params"].items()
+                                    for param_name, param_details in data[
+                                        "params"
+                                    ].items()
                                 }
 
                                 # Now you can call run_method using argument unpacking
-                                asyncio.create_task(self.run_method(method_name, **params))
-                        elif msg['type'] == 'close_connection':
+                                asyncio.create_task(
+                                    self.run_method(method_name, **params)
+                                )
+                        elif msg["type"] == "close_connection":
                             try:
                                 await self.websocket.close()
                             except Exception as e:
                                 print("Error closing connection: ", e)
 
                             print("Connection closed by server")
                             break  # Exit the while loop
@@ -647,15 +658,14 @@
             raise ValueError
     except ValueError:
         raise ValueError(f"Invalid token: '{token}'. Token must be a valid UUID.")
 
     _client.set_token(token)
 
 
-
 async def _register_method(method):
     await _client.register_method(method)
 
 
 def register_method(method):
     try:
         asyncio.run(_register_method(method))
```

### Comparing `elixir-client-0.7.6/elixir_client/dn_tracer.py` & `elixir-client-0.7.7/elixir_client/dn_tracer.py`

 * *Files identical despite different names*

### Comparing `elixir-client-0.7.6/elixir_client/file_uploader.py` & `elixir-client-0.7.7/elixir_client/file_uploader.py`

 * *Files identical despite different names*

### Comparing `elixir-client-0.7.6/elixir_client/output/results_handler.py` & `elixir-client-0.7.7/elixir_client/output/results_handler.py`

 * *Files identical despite different names*

### Comparing `elixir-client-0.7.6/elixir_client/utils/audio_utils.py` & `elixir-client-0.7.7/elixir_client/utils/audio_utils.py`

 * *Files identical despite different names*

### Comparing `elixir-client-0.7.6/elixir_client/utils/file_type_classifier.py` & `elixir-client-0.7.7/elixir_client/utils/file_type_classifier.py`

 * *Files identical despite different names*

### Comparing `elixir-client-0.7.6/elixir_client.egg-info/PKG-INFO` & `elixir-client-0.7.7/elixir_client.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 Metadata-Version: 2.1
 Name: elixir-client
-Version: 0.7.6
+Version: 0.7.7
 Summary: Elixir client enables remote execution of python code triggered from a Crucible Plugin on the Signals & Sorcery platform.
 Home-page: https://dawnet.tools
 Author: Steve Hiehn
 Author-email: stevehiehn@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# Elixir Client
+# Signals & Sorcery
 
-`DAWNet` is a DAW (digit audio workstation) plugin that connects to a remote Google Colab or Script.  A user can send audio files from the plugin for remote processing. Hence, perform computationally expensive tasks such as text-2-audio or stem separation without leaving the DAW. 
+Signals & Socery is a platform for that connects Elixir AIs to Crucible plugins.
 
 For more information:
 
-- [https://dawnet.tools/](https://dawnet.tools/)
+- [Signals & Sorcery DOCS](https://signalsandsorcery.com/)
 
 - [Community Discord](https://discord.gg/UcHCjfpRkV)
 
 # elixir-client
 
-The `DAWNet client` (this repo) is a python3 pip package.  It is used to create `DAWNet remotes`.  The client is responsible for moving data and files backand forth from the plugin (and server).   The client allows a user to register python functions with the DAWNet discovery server. After a function has been registered it can then be triggered remotely from `DAWNet plugin.   
-
-::: warning
-NOTE: The plugin is in an active, pre-alpha state.  It has only been tested on Ableton 11 on MAC M1.
-:::
+The Elixir Client (this repo) is a python3 pip package.  It is used to create Elixir AIs.  Elixir AIs are [Jupyter Notebooks](https://jupyter.org/) scripted using the elixir client and packaged as containers. The client is responsible for moving data and files backand forth from the plugin (and server).   The client allows a user to register python functions with the Signals & Sorcery discovery server. After a function has been registered it can then be triggered remotely from any of the [Crucible plugins](https://signalsandsorcery.com/crucible-plugins/).   
 
 ## Installation
 
 ```python
 pip install elixir-client --upgrade
 ```
 
@@ -116,15 +112,15 @@
 
 
 ## CONFIGURATION:
 
 *Note:* If the following environment variables are not set, the client will use the default values.  The default values will point to the public DAWNet server.  If you wish to host your own instance you will need to configure the following environment variables. 
 
 ```
-export DN_CLIENT_API_BASE_URL='http://localhost:8081'
+export DN_CLIENT_API_BASE_URL='https://signalsandsorceryapi.com/'
 export DN_CLIENT_SOCKET_IP='0.0.0.0'
 export DN_CLIENT_SOCKET_PORT='8765'
 export DN_CLIENT_SENTRY_API_KEY='XXX'
 "DN_CLIENT_STORAGE_BUCKET", "https://storage.googleapis.com/your_gcp_bucket/"
 ```
 
 *Note:* If the env var `DN_CLIENT_TOKEN` is set it will override the set_token() function.
```

### Comparing `elixir-client-0.7.6/elixir_client.egg-info/SOURCES.txt` & `elixir-client-0.7.7/elixir_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elixir-client-0.7.6/setup.py` & `elixir-client-0.7.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 """
 
 if not is_ffmpeg_installed():
     print(ffmpeg_warning_msg)
 
 setup(
     name="elixir-client",
-    version="0.7.6",
+    version="0.7.7",
     packages=find_packages(),
     install_requires=[
         "aiohttp",
         "websockets",
         "nest-asyncio",
         "sentry-sdk",
         "pydub",
```

### Comparing `elixir-client-0.7.6/tests/test_audio_utils.py` & `elixir-client-0.7.7/tests/test_audio_utils.py`

 * *Files identical despite different names*

### Comparing `elixir-client-0.7.6/tests/test_core.py` & `elixir-client-0.7.7/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `elixir-client-0.7.6/tests/test_registration.py` & `elixir-client-0.7.7/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `elixir-client-0.7.6/tests/test_results_handler.py` & `elixir-client-0.7.7/tests/test_results_handler.py`

 * *Files identical despite different names*

