# Comparing `tmp/feagi_connector-0.0.2.tar.gz` & `tmp/feagi_connector-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feagi_connector-0.0.2.tar", last modified: Fri Mar 29 14:35:16 2024, max compression
+gzip compressed data, was "feagi_connector-0.0.3.tar", last modified: Fri Apr  5 14:32:43 2024, max compression
```

## Comparing `feagi_connector-0.0.2.tar` & `feagi_connector-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:35:16.350300 feagi_connector-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-03-29 14:35:06.000000 feagi_connector-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-03-29 14:35:16.350300 feagi_connector-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-03-29 14:35:06.000000 feagi_connector-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:35:16.350300 feagi_connector-0.0.2/feagi_connector/
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-03-29 14:35:06.000000 feagi_connector-0.0.2/feagi_connector/PIL_retina.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 14:35:06.000000 feagi_connector-0.0.2/feagi_connector/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6091 2024-03-29 14:35:06.000000 feagi_connector-0.0.2/feagi_connector/actuators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-03-29 14:35:06.000000 feagi_connector-0.0.2/feagi_connector/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    17539 2024-03-29 14:35:06.000000 feagi_connector-0.0.2/feagi_connector/feagi_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    20046 2024-03-29 14:35:06.000000 feagi_connector-0.0.2/feagi_connector/pns_gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    25199 2024-03-29 14:35:06.000000 feagi_connector-0.0.2/feagi_connector/retina.py
--rw-r--r--   0 runner    (1001) docker     (127)    14205 2024-03-29 14:35:06.000000 feagi_connector-0.0.2/feagi_connector/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:35:16.350300 feagi_connector-0.0.2/feagi_connector/sensorimotor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 14:35:06.000000 feagi_connector-0.0.2/feagi_connector/sensorimotor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-03-29 14:35:06.000000 feagi_connector-0.0.2/feagi_connector/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-29 14:35:06.000000 feagi_connector-0.0.2/feagi_connector/testing_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-29 14:35:06.000000 feagi_connector-0.0.2/feagi_connector/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-29 14:35:06.000000 feagi_connector-0.0.2/feagi_connector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:35:16.350300 feagi_connector-0.0.2/feagi_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-03-29 14:35:16.000000 feagi_connector-0.0.2/feagi_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-29 14:35:16.000000 feagi_connector-0.0.2/feagi_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 14:35:16.000000 feagi_connector-0.0.2/feagi_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-29 14:35:16.000000 feagi_connector-0.0.2/feagi_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-29 14:35:16.000000 feagi_connector-0.0.2/feagi_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-29 14:35:06.000000 feagi_connector-0.0.2/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      766 2024-03-29 14:35:16.350300 feagi_connector-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:32:43.190604 feagi_connector-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-05 14:32:43.190604 feagi_connector-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:32:43.190604 feagi_connector-0.0.3/feagi_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/feagi_connector/PIL_retina.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/feagi_connector/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6091 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/feagi_connector/actuators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/feagi_connector/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18257 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/feagi_connector/feagi_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20054 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/feagi_connector/pns_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25199 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/feagi_connector/retina.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11686 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/feagi_connector/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:32:43.190604 feagi_connector-0.0.3/feagi_connector/sensorimotor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/feagi_connector/sensorimotor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/feagi_connector/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/feagi_connector/testing_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/feagi_connector/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/feagi_connector/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:32:43.190604 feagi_connector-0.0.3/feagi_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-05 14:32:43.000000 feagi_connector-0.0.3/feagi_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-05 14:32:43.000000 feagi_connector-0.0.3/feagi_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:32:43.000000 feagi_connector-0.0.3/feagi_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-05 14:32:43.000000 feagi_connector-0.0.3/feagi_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 14:32:43.000000 feagi_connector-0.0.3/feagi_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-05 14:32:30.000000 feagi_connector-0.0.3/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      766 2024-04-05 14:32:43.194604 feagi_connector-0.0.3/setup.cfg
```

### Comparing `feagi_connector-0.0.2/LICENSE` & `feagi_connector-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.2/PKG-INFO` & `feagi_connector-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feagi_connector
-Version: 0.0.2
+Version: 0.0.3
 Summary: Feagi agent to work with general and simulation robots
 Home-page: https://github.com/feagi/feagi-connector
 Author: Neuraville Inc.
 Author-email: info@feagi.org
 Project-URL: Bug Tracker, https://github.com/feagi/feagi/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `feagi_connector-0.0.2/README.md` & `feagi_connector-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.2/feagi_connector/PIL_retina.py` & `feagi_connector-0.0.3/feagi_connector/PIL_retina.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.2/feagi_connector/actuators.py` & `feagi_connector-0.0.3/feagi_connector/actuators.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.2/feagi_connector/configuration.py` & `feagi_connector-0.0.3/feagi_connector/configuration.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.2/feagi_connector/feagi_interface.py` & `feagi_connector-0.0.3/feagi_connector/feagi_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 import traceback
 from feagi_connector import router
 from feagi_connector import pns_gateway as pns
 from feagi_connector.version import __version__
 from time import sleep
 import requests
 import socket
+import threading
+
 
 
 def pub_initializer(ipu_address, bind=True):
     return router.Pub(address=ipu_address, bind=bind)
 
 
 def sub_initializer(opu_address, flags=router.zmq.NOBLOCK):
     return router.Sub(address=opu_address, flags=flags)
 
 
 def feagi_registration(feagi_auth_url, feagi_settings, agent_settings, capabilities,
-                       controller_version):
+                       controller_version, magic_link=''):
     host_info = router.app_host_info()
     runtime_data = {
         "host_network": {},
         "feagi_state": None
     }
     runtime_data["host_network"]["host_name"] = host_info["host_name"]
     runtime_data["host_network"]["ip_address"] = host_info["ip_address"]
     agent_settings['agent_ip'] = host_info["ip_address"]
 
     while runtime_data["feagi_state"] is None:
         print("\nAwaiting registration with FEAGI...")
         try:
             runtime_data["feagi_state"] = \
                 router.register_with_feagi(feagi_auth_url, feagi_settings, agent_settings,
-                                           capabilities, controller_version, __version__)
+                                           capabilities, controller_version, __version__, magic_link)
         except Exception as e:
             print("ERROR__: ", e, traceback.print_exc())
             pass
         sleep(1)
     print("\nversion: ", controller_version, "\n")
     print("\nagent version: ", __version__, "\n")
     return runtime_data["feagi_state"]
@@ -316,43 +318,56 @@
                 configuration.capabilities["position"][position_index]["z"] = \
                     float(control_data['robot_starting_position'][position_index][2])
         return configuration.capabilities["motor"]["power_coefficient"], \
                configuration.capabilities["position"]
 
 
 def connect_to_feagi(feagi_settings, runtime_data, agent_settings, capabilities, current_version,
-                     bind_flag=False):
+                     bind_flag=False, magic_link=''):
     print("Connecting to FEAGI resources...")
     feagi_auth_url = feagi_settings.pop('feagi_auth_url', None)
     runtime_data["feagi_state"] = feagi_registration(feagi_auth_url=feagi_auth_url,
                                                      feagi_settings=feagi_settings,
                                                      agent_settings=agent_settings,
                                                      capabilities=capabilities,
-                                                     controller_version=current_version)
+                                                     controller_version=current_version,
+                                                     magic_link=magic_link)
     api_address = runtime_data['feagi_state']["feagi_url"]
     router.global_api_address = api_address
     agent_data_port = str(runtime_data["feagi_state"]['agent_state']['agent_data_port'])
     print("** **", runtime_data["feagi_state"])
     feagi_settings['feagi_burst_speed'] = float(runtime_data["feagi_state"]['burst_duration'])
-    if bind_flag:
-        ipu_channel_address = "tcp://*:" + agent_data_port # This is for godot to work due to
-        # bind unable to use the dns.
+    if magic_link == '':
+        if bind_flag:
+            ipu_channel_address = "tcp://*:" + agent_data_port  # This is for godot to work due to
+            # bind unable to use the dns.
+        else:
+            ipu_channel_address = feagi_outbound(feagi_settings['feagi_host'], agent_data_port)
+
+        print("IPU_channel_address=", ipu_channel_address)
+        opu_channel_address = feagi_outbound(feagi_settings['feagi_host'],
+                                             runtime_data["feagi_state"]['feagi_opu_port'])
+
+        # ip = '172.28.0.2'
+        # opu_channel_address = 'tcp://' + str(ip) + ':3000'
+        # ipu_channel_address = 'tcp://' + str(ip) + ':3000'
+        feagi_ipu_channel = pub_initializer(ipu_channel_address, bind=bind_flag)
+        feagi_opu_channel = sub_initializer(opu_address=opu_channel_address)
+        router.global_feagi_opu_channel = feagi_opu_channel
+        threading.Thread(target=pns.feagi_listener, args=(feagi_opu_channel,), daemon=True).start()
     else:
-        ipu_channel_address = feagi_outbound(feagi_settings['feagi_host'], agent_data_port)
+        feagi_ipu_channel = None
+        feagi_opu_channel = None
+        print("websocket testing")
+        websocket_url = feagi_settings['feagi_dns'].replace("https", "wss") + str("/p9053")
+        print(websocket_url)
+        router.websocket_client_initalize('192.168.50.192', '9053', dns=websocket_url)
+        threading.Thread(target=router.websocket_recieve, daemon=True).start()
+
 
-    print("IPU_channel_address=", ipu_channel_address)
-    opu_channel_address = feagi_outbound(feagi_settings['feagi_host'],
-                                         runtime_data["feagi_state"]['feagi_opu_port'])
-
-    # ip = '172.28.0.2'
-    # opu_channel_address = 'tcp://' + str(ip) + ':3000'
-    # ipu_channel_address = 'tcp://' + str(ip) + ':3000'
-    feagi_ipu_channel = pub_initializer(ipu_channel_address, bind=bind_flag)
-    feagi_opu_channel = sub_initializer(opu_address=opu_channel_address)
-    router.global_feagi_opu_channel = feagi_opu_channel
     return feagi_settings, runtime_data, api_address, feagi_ipu_channel, feagi_opu_channel
 
 
 def build_up_from_mctl(id):
     action_map = {
         (0, 0): "move_left",
         (0, 1): "roll_left",
```

### Comparing `feagi_connector-0.0.2/feagi_connector/pns_gateway.py` & `feagi_connector-0.0.3/feagi_connector/pns_gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -398,16 +398,16 @@
                 "threshold_default": [50, 255, 130, 51],  # min #1, max #1, min #2, max #2,
                 "threshold_range": [1, 255],
                 "threshold_type": {},
                 # simple thresholding types. see the retina.threshold_detect function
                 "threshold_name": 0,  # Binary_threshold as a default
                 "mirror": True,  # flip the image
                 "blink": [],  # cv2 ndarray raw data of an image. Controlled by blink OPU in genome
-                "gaze_control": {0: 1, 1: 1},  # Controlled by gaze_control in genome
-                "pupil_control": {0: 99, 1: 99},  # Controlled by pupil_control in genome
+                "gaze_control": {'0': 1, '1': 1},  # Controlled by gaze_control in genome
+                "pupil_control": {'0': 99, '1': 99},  # Controlled by pupil_control in genome
                 "vision_range": [1, 99],  # min, max
                 "size_list": [],  # To get the size in real time based on genome's change/update
                 "enhancement": {},  # Enable ov_enh OPU on inside the genome
                 "percentage_to_allow_data" : 0.5 # this will be percentage for the full data.
                 # Currently set to 0.5 to allow data go through otherwise discard it fully.
             }
         }
```

### Comparing `feagi_connector-0.0.2/feagi_connector/retina.py` & `feagi_connector-0.0.3/feagi_connector/retina.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.2/feagi_connector/router.py` & `feagi_connector-0.0.3/feagi_connector/router.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,23 +12,24 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ==============================================================================
 """
 import zmq
-import zmq.asyncio
 import json
 import socket
 import pickle
 import asyncio
 import requests
+import threading
 import lz4.frame
 import traceback
 import websockets
+import zmq.asyncio
 from time import sleep
 from feagi_connector import pns_gateway as pns
 from websockets.sync.client import connect
 
 global_feagi_opu_channel = ''  # Updated by feagi.connect_to_feagi()
 global_api_address = ''  # Updated by feagi.connect_to_feagi
 global_websocket_address = ''  # Just a full address stored
@@ -121,15 +122,14 @@
 
 def feagi_listener(feagi_opu_channel):
     while True:
         data = fetch_feagi(feagi_opu_channel)
         if data is not None:
             pns.message_from_feagi = data
         sleep(0.001)  # hardcoded and max second that it can run up to
-        # print("inside router: ", pns.message_from_feagi['opu_data']['o__gaz'])
 
 
 def send_feagi(message_to_feagi, feagi_ipu_channel, agent_settings):
     """
     send data to FEAGI
     """
     if agent_settings['compression']:
@@ -154,71 +154,14 @@
             get(global_api_address + '/v1/cortical_area/cortical_area/geometry').json()
         return list_dimesions
     except Exception as e:
         print("e: ", e)
         return []
 
 
-# def register_with_feagi(feagi_ip, feagi_api_port, agent_type: str, agent_id: str, agent_ip: str, agent_data_port: int,
-#                         agent_capabilities):
-#     """
-#     To trade information between FEAGI and Controller
-
-#     Controller                      <--     FEAGI(IPU/OPU socket info)
-#     Controller (Capabilities)       -->     FEAGI
-#     """
-#     api_address = 'http://' + feagi_ip + ':' + feagi_api_port
-#     network_endpoint = '/v1/network'
-#     stimulation_period_endpoint = '/v1/burst_engine/stimulation_period'
-#     burst_counter_endpoint = '/v1/burst_engine/burst_counter'
-#     registration_endpoint = '/v1/agent/register'
-
-#     registration_complete = False
-#     feagi_settings = dict()
-#     while not registration_complete:
-#         try:
-#             feagi_settings = requests.get(api_address + network_endpoint).json()
-#             if feagi_settings:
-#                 print("Data from FEAGI::", feagi_settings)
-#             else:
-#                 print("No feagi settings!")
-
-#             agent_registration_data = dict()
-#             agent_registration_data["agent_type"] = str(agent_type)
-#             agent_registration_data["agent_id"] = str(agent_id)
-#             agent_registration_data["agent_ip"] = str(agent_ip)
-#             agent_registration_data["agent_data_port"] = int(agent_data_port)
-
-#             response = requests.post(api_address + registration_endpoint, params=agent_registration_data)
-#             if response.status_code == 200:
-#                 feagi_settings['agent_info'] =  response.json()
-#                 print("Agent successfully registered with FEAGI!")
-#                 # Receive FEAGI settings
-#                 feagi_settings['burst_duration'] = requests.get(api_address + stimulation_period_endpoint).json()
-#                 feagi_settings['burst_counter'] = requests.get(api_address + burst_counter_endpoint).json()
-
-
-#                 if feagi_settings and feagi_settings['burst_duration'] and feagi_settings['burst_counter']:
-#                     print("\n\n\n\nRegistration is complete....")
-#                     registration_complete = True
-#         except Exception as e:
-#             print("Trying to register with FEAGI at ", api_address)
-#         sleep(1)
-
-#     print("feagi_ip:agent_data_port", feagi_ip, agent_data_port)
-#     # Transmit Controller Capabilities
-#     # address, bind = f"tcp://*:{agent_data_port}", True
-#     address, bind = f"tcp://{feagi_ip}:{agent_data_port}", False
-
-#     publisher = Pub(address, bind)
-#     publisher.send(agent_capabilities)
-
-#     return feagi_settings
-
-
 def feagi_settings_from_composer(feagi_auth_url, feagi_settings):
     """
     Generate all needed information and return the full data to make it easier to connect with
     FEAGI
     """
     if feagi_auth_url is not None:
         print(f"Updating feagi settings using feagi_auth_url: {feagi_auth_url}")
@@ -236,15 +179,15 @@
     else:
         feagi_settings[
             'feagi_url'] = f"http://{feagi_settings['feagi_host']}:{feagi_settings['feagi_api_port']}"
     return feagi_settings
 
 
 def register_with_feagi(feagi_auth_url, feagi_settings, agent_settings, agent_capabilities,
-                        controller_version, agent_version):
+                        controller_version, agent_version, magic_link=''):
     """
     To trade information between FEAGI and Controller
 
     Controller                      <--     FEAGI(IPU/OPU socket info)
     Controller (Capabilities)       -->     FEAGI
     """
     network_endpoint = '/v1/network/network'
@@ -255,61 +198,62 @@
     registration_complete = False
     while not registration_complete:
         try:
             print(f"Original Feagi Settings ---- {feagi_settings}")
             feagi_settings = feagi_settings_from_composer(feagi_auth_url, feagi_settings)
             feagi_url = feagi_settings['feagi_url']
 
+            print("feagiurl: ", feagi_url, " network endpoint: ", network_endpoint)
+
             network_output = requests.get(feagi_url + network_endpoint).json()
             # print(f"network_output ---- {network_output}")
-            feagi_settings['feagi_opu_port'] = network_output['feagi_opu_port']
+            if magic_link == '':
+                feagi_settings['feagi_opu_port'] = network_output['feagi_opu_port']
             if feagi_settings:
                 print("Data from FEAGI::", feagi_settings)
             else:
                 print("No feagi settings!")
 
             agent_registration_data = dict()
             agent_registration_data["agent_type"] = str(agent_settings['agent_type'])
             agent_registration_data["agent_id"] = str(agent_settings['agent_id'])
-            agent_registration_data["agent_ip"] = str(agent_settings['agent_ip'])#str("127.0.0.1")
+            agent_registration_data["agent_ip"] = str(agent_settings['agent_ip'])  # str("127.0.0.1")
             agent_registration_data["agent_data_port"] = int(agent_settings['agent_data_port'])
             agent_registration_data["controller_version"] = str(controller_version)
             agent_registration_data["agent_version"] = str(agent_version)
 
             response = requests.post(feagi_url + registration_endpoint,
                                      params=agent_registration_data)
             if response.status_code == 200:
                 feagi_settings['agent_state'] = response.json()
                 print("Agent successfully registered with FEAGI!")
                 # Receive FEAGI settings
-                feagi_settings['burst_duration'] = requests.get(
-                    feagi_url + stimulation_period_endpoint).json()
-                feagi_settings['burst_counter'] = requests.get(
-                    feagi_url + burst_counter_endpoint).json()
+                feagi_settings['burst_duration'] = requests.get(feagi_url + stimulation_period_endpoint).json()
+                feagi_settings['burst_counter'] = requests.get(feagi_url + burst_counter_endpoint).json()
 
-                if feagi_settings and feagi_settings['burst_duration'] and feagi_settings[
-                    'burst_counter']:
+                if feagi_settings and feagi_settings['burst_duration'] and feagi_settings['burst_counter']:
                     print("\n\n\n\nRegistration is complete....")
                     registration_complete = True
         except Exception as e:
             print("Registeration failed with FEAGI: ", e)
             # traceback.print_exc()
         sleep(2)
 
-    # feagi_settings['agent_state']['agent_ip'] = "127.0.0.1"
-    print(f"Final Feagi Settings ---- {feagi_settings}")
-    feagi_ip = feagi_settings['feagi_host']
-    agent_data_port = feagi_settings['agent_state']['agent_data_port']
-    print("feagi_ip:agent_data_port", feagi_ip, agent_data_port)
-    # Transmit Controller Capabilities
-    # address, bind = f"tcp://*:{agent_data_port}", True
-    address, bind = f"tcp://{feagi_ip}:{agent_data_port}", False
+    if magic_link == '':
+        # feagi_settings['agent_state']['agent_ip'] = "127.0.0.1"
+        print(f"Final Feagi Settings ---- {feagi_settings}")
+        feagi_ip = feagi_settings['feagi_host']
+        agent_data_port = feagi_settings['agent_state']['agent_data_port']
+        print("feagi_ip:agent_data_port", feagi_ip, agent_data_port)
+        # Transmit Controller Capabilities
+        # address, bind = f"tcp://*:{agent_data_port}", True
+        address, bind = f"tcp://{feagi_ip}:{agent_data_port}", False
 
-    publisher = Pub(address, bind)
-    publisher.send(agent_capabilities)
+        publisher = Pub(address, bind)
+        publisher.send(agent_capabilities)
 
     return feagi_settings
 
 
 # # Websocket section # #
 async def main(function, ip, port):
     """
@@ -377,14 +321,9 @@
 
 def websocket_recieve():
     global websocket, global_websocket_address
     while True:
         try:
             pns.message_from_feagi = pickle.loads(websocket.recv())
         except Exception as e:
-            print("error: ", e)
+            print("error in websocket recieve: ", e)
             websocket = connect(global_websocket_address)
-
-
-
-
-
```

### Comparing `feagi_connector-0.0.2/feagi_connector/sensors.py` & `feagi_connector-0.0.3/feagi_connector/sensors.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.2/feagi_connector/testing_mode.py` & `feagi_connector-0.0.3/feagi_connector/testing_mode.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.2/feagi_connector/trainer.py` & `feagi_connector-0.0.3/feagi_connector/trainer.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.2/feagi_connector.egg-info/PKG-INFO` & `feagi_connector-0.0.3/feagi_connector.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feagi_connector
-Version: 0.0.2
+Version: 0.0.3
 Summary: Feagi agent to work with general and simulation robots
 Home-page: https://github.com/feagi/feagi-connector
 Author: Neuraville Inc.
 Author-email: info@feagi.org
 Project-URL: Bug Tracker, https://github.com/feagi/feagi/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `feagi_connector-0.0.2/feagi_connector.egg-info/SOURCES.txt` & `feagi_connector-0.0.3/feagi_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.2/setup.cfg` & `feagi_connector-0.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = feagi_connector
-version = 0.0.2
+version = 0.0.3
 author = Neuraville Inc.
 author_email = info@feagi.org
 description = Feagi agent to work with general and simulation robots
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/feagi/feagi-connector
 project_urls =
```

