# Comparing `tmp/crosslab_soa_client-0.2.6.tar.gz` & `tmp/crosslab_soa_client-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslab_soa_client-0.2.6.tar", last modified: Thu Feb  8 15:24:14 2024, max compression
+gzip compressed data, was "crosslab_soa_client-0.2.7.tar", last modified: Fri Apr  5 09:16:59 2024, max compression
```

## Comparing `crosslab_soa_client-0.2.6.tar` & `crosslab_soa_client-0.2.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:24:14.327665 crosslab_soa_client-0.2.6/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      397 2024-02-08 15:24:14.327665 crosslab_soa_client-0.2.6/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2494 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.6/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.6/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)      617 2024-02-08 15:24:14.327665 crosslab_soa_client-0.2.6/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)       37 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.6/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:24:14.323665 crosslab_soa_client-0.2.6/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:24:14.323665 crosslab_soa_client-0.2.6/src/crosslab/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:24:14.323665 crosslab_soa_client-0.2.6/src/crosslab/soa_client/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.6/src/crosslab/soa_client/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1774 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.6/src/crosslab/soa_client/connection.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10234 2023-12-11 21:52:54.000000 crosslab_soa_client-0.2.6/src/crosslab/soa_client/connection_webrtc.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7367 2024-02-07 11:14:28.000000 crosslab_soa_client-0.2.6/src/crosslab/soa_client/device_handler.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:24:14.323665 crosslab_soa_client-0.2.6/src/crosslab/soa_client/media/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.6/src/crosslab/soa_client/media/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      395 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.6/src/crosslab/soa_client/media/gst_track.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      557 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.6/src/crosslab/soa_client/media/udp_track.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.6/src/crosslab/soa_client/message_handling.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1400 2024-02-07 11:14:28.000000 crosslab_soa_client-0.2.6/src/crosslab/soa_client/messages.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.6/src/crosslab/soa_client/py.typed
--rw-r--r--   0 vscode    (1000) vscode    (1000)      778 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.6/src/crosslab/soa_client/service.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:24:14.323665 crosslab_soa_client-0.2.6/src/crosslab/soa_client/test_helper/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       81 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.6/src/crosslab/soa_client/test_helper/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1051 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.6/src/crosslab/soa_client/test_helper/connection_stub.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      787 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.6/src/crosslab/soa_client/test_helper/dummy_track.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4331 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.6/src/crosslab/soa_client/test_helper/service_stub.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:24:14.327665 crosslab_soa_client-0.2.6/src/crosslab_soa_client.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      397 2024-02-08 15:24:14.000000 crosslab_soa_client-0.2.6/src/crosslab_soa_client.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      981 2024-02-08 15:24:14.000000 crosslab_soa_client-0.2.6/src/crosslab_soa_client.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-02-08 15:24:14.000000 crosslab_soa_client-0.2.6/src/crosslab_soa_client.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       36 2024-02-08 15:24:14.000000 crosslab_soa_client-0.2.6/src/crosslab_soa_client.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2024-02-08 15:24:14.000000 crosslab_soa_client-0.2.6/src/crosslab_soa_client.egg-info/top_level.txt
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:24:14.327665 crosslab_soa_client-0.2.6/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2046 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.6/tests/test_device_handler.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5239 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.6/tests/test_webrtc_connection.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:16:59.030526 crosslab_soa_client-0.2.7/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      397 2024-04-05 09:16:59.030526 crosslab_soa_client-0.2.7/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2494 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      617 2024-04-05 09:16:59.030526 crosslab_soa_client-0.2.7/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       37 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:16:59.026526 crosslab_soa_client-0.2.7/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:16:59.026526 crosslab_soa_client-0.2.7/src/crosslab/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:16:59.030526 crosslab_soa_client-0.2.7/src/crosslab/soa_client/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1774 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/connection.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10234 2023-12-11 21:52:54.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/connection_webrtc.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7790 2024-03-01 08:08:11.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/device_handler.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:16:59.030526 crosslab_soa_client-0.2.7/src/crosslab/soa_client/media/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/media/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      395 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/media/gst_track.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      557 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/media/udp_track.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/message_handling.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1623 2024-03-01 08:08:11.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/messages.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/py.typed
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      778 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/service.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:16:59.030526 crosslab_soa_client-0.2.7/src/crosslab/soa_client/test_helper/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       81 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/test_helper/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1051 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/test_helper/connection_stub.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      787 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/test_helper/dummy_track.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4331 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/src/crosslab/soa_client/test_helper/service_stub.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:16:59.030526 crosslab_soa_client-0.2.7/src/crosslab_soa_client.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      397 2024-04-05 09:16:59.000000 crosslab_soa_client-0.2.7/src/crosslab_soa_client.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      981 2024-04-05 09:16:59.000000 crosslab_soa_client-0.2.7/src/crosslab_soa_client.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-04-05 09:16:59.000000 crosslab_soa_client-0.2.7/src/crosslab_soa_client.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       36 2024-04-05 09:16:59.000000 crosslab_soa_client-0.2.7/src/crosslab_soa_client.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2024-04-05 09:16:59.000000 crosslab_soa_client-0.2.7/src/crosslab_soa_client.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:16:59.030526 crosslab_soa_client-0.2.7/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2046 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/tests/test_device_handler.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5239 2023-11-08 12:05:40.000000 crosslab_soa_client-0.2.7/tests/test_webrtc_connection.py
```

### Comparing `crosslab_soa_client-0.2.6/README.md` & `crosslab_soa_client-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.6/setup.cfg` & `crosslab_soa_client-0.2.7/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosslab_soa_client
-version = 0.2.6
+version = 0.2.7
 author = Johannes Nau
 author_email = johannes.nau@tu-ilmenau.de
 description = The CrossLab SOA Client
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Other/Proprietary License
 	Operating System :: OS Independent
```

### Comparing `crosslab_soa_client-0.2.6/src/crosslab/soa_client/connection.py` & `crosslab_soa_client-0.2.7/src/crosslab/soa_client/connection.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.6/src/crosslab/soa_client/connection_webrtc.py` & `crosslab_soa_client-0.2.7/src/crosslab/soa_client/connection_webrtc.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.6/src/crosslab/soa_client/device_handler.py` & `crosslab_soa_client-0.2.7/src/crosslab/soa_client/device_handler.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from crosslab.soa_client.connection_webrtc import WebRTCPeerConnection
 from crosslab.soa_client.messages import (
     AuthenticationMessage,
     ClosePeerConnectionMessage,
     ConfigurationMessage,
     ConnectionStateChangedMessage,
     CreatePeerConnectionMessage,
+    ExperimentStatusChangedMessage,
     SignalingMessage,
 )
 from crosslab.soa_client.service import Service
 
 
 async def receiveMessage(ws: aiohttp.ClientWebSocketResponse):
     msg = await ws.receive()
@@ -128,14 +129,16 @@
                 and msg["command"] == "closePeerconnection"
             ):
                 await self._on_close_peerconnection(msg)
             elif msg["messageType"] == "signaling":
                 await self._on_signaling_message(msg)
             elif msg["messageType"] == "configuration":
                 await self._on_configuration_message(msg)
+            elif msg["messageType"] == "experiment-status-changed":
+                await self._on_experiment_status_changed_message(msg)
             else:
                 pass  # Do not raise any Exception here, so we are forward compatible for new message types
 
     async def _on_create_peerconnection(self, msg: CreatePeerConnectionMessage):
         assert msg["connectionUrl"] not in self._connections
         if msg["connectionType"] == "webrtc":
             connection = WebRTCPeerConnection()
@@ -185,7 +188,15 @@
     async def _on_signaling_message(self, msg: SignalingMessage):
         connection = self._connections.get(msg["connectionUrl"], None)
         assert connection is not None  # TODO: Error handling
         await connection.handleSignalingMessage(msg)
 
     async def _on_configuration_message(self, msg: ConfigurationMessage):
         self.emit("configuration", msg["configuration"])
+
+    async def _on_experiment_status_changed_message(
+        self, msg: ExperimentStatusChangedMessage
+    ):
+        self.emit(
+            "experimentStatusChanged",
+            {"status": msg["status"], "message": msg.get("message")},
+        )
```

### Comparing `crosslab_soa_client-0.2.6/src/crosslab/soa_client/media/udp_track.py` & `crosslab_soa_client-0.2.7/src/crosslab/soa_client/media/udp_track.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.6/src/crosslab/soa_client/messages.py` & `crosslab_soa_client-0.2.7/src/crosslab/soa_client/messages.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Literal, TypedDict
+from typing import List, Literal, TypedDict, Optional
 
 
 class Message(TypedDict):
     messageType: str
 
 
 class CommandMessage(TypedDict):
@@ -53,7 +53,13 @@
     connectionUrl: str
     status: Literal["new", "connecting", "connected", "disconnected", "failed", "closed"]
 
 
 class ConfigurationMessage(TypedDict):
     messageType: Literal["configuration"]
     configuration: dict
+
+
+class ExperimentStatusChangedMessage(TypedDict):
+    messageType: Literal["experiment-status-changed"]
+    status: Literal["created", "booked", "setup", "running", "failed", "closed"]
+    message: Optional[str]
```

### Comparing `crosslab_soa_client-0.2.6/src/crosslab/soa_client/service.py` & `crosslab_soa_client-0.2.7/src/crosslab/soa_client/service.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.6/src/crosslab/soa_client/test_helper/connection_stub.py` & `crosslab_soa_client-0.2.7/src/crosslab/soa_client/test_helper/connection_stub.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.6/src/crosslab/soa_client/test_helper/dummy_track.py` & `crosslab_soa_client-0.2.7/src/crosslab/soa_client/test_helper/dummy_track.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.6/src/crosslab/soa_client/test_helper/service_stub.py` & `crosslab_soa_client-0.2.7/src/crosslab/soa_client/test_helper/service_stub.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.6/src/crosslab_soa_client.egg-info/SOURCES.txt` & `crosslab_soa_client-0.2.7/src/crosslab_soa_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.6/tests/test_device_handler.py` & `crosslab_soa_client-0.2.7/tests/test_device_handler.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_client-0.2.6/tests/test_webrtc_connection.py` & `crosslab_soa_client-0.2.7/tests/test_webrtc_connection.py`

 * *Files identical despite different names*

