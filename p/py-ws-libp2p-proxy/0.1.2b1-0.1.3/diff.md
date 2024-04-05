# Comparing `tmp/py_ws_libp2p_proxy-0.1.2b1.tar.gz` & `tmp/py_ws_libp2p_proxy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ws_libp2p_proxy-0.1.2b1.tar", max compression
+gzip compressed data, was "py_ws_libp2p_proxy-0.1.3.tar", max compression
```

## Comparing `py_ws_libp2p_proxy-0.1.2b1.tar` & `py_ws_libp2p_proxy-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11344 2024-04-02 11:52:10.396510 py_ws_libp2p_proxy-0.1.2b1/LICENSE
--rw-r--r--   0        0        0      257 2024-04-02 11:52:10.396510 py_ws_libp2p_proxy-0.1.2b1/README.md
--rw-r--r--   0        0        0      524 2024-04-02 11:52:10.396510 py_ws_libp2p_proxy-0.1.2b1/pyproject.toml
--rw-r--r--   0        0        0     3877 2024-04-02 11:52:10.396510 py_ws_libp2p_proxy-0.1.2b1/pyproxy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 11:52:10.396510 py_ws_libp2p_proxy-0.1.2b1/pyproxy/utils/__init__.py
--rw-r--r--   0        0        0     2358 2024-04-02 11:52:10.396510 py_ws_libp2p_proxy-0.1.2b1/pyproxy/utils/decorators.py
--rw-r--r--   0        0        0       53 2024-04-02 11:52:10.396510 py_ws_libp2p_proxy-0.1.2b1/pyproxy/utils/logger.py
--rw-r--r--   0        0        0      780 2024-04-02 11:52:10.396510 py_ws_libp2p_proxy-0.1.2b1/pyproxy/utils/message.py
--rw-r--r--   0        0        0      663 2024-04-02 11:52:10.396510 py_ws_libp2p_proxy-0.1.2b1/pyproxy/utils/protocols_manager.py
--rw-r--r--   0        0        0     3452 2024-04-02 11:52:10.396510 py_ws_libp2p_proxy-0.1.2b1/pyproxy/utils/websocket.py
--rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 py_ws_libp2p_proxy-0.1.2b1/PKG-INFO
+-rw-r--r--   0        0        0    11344 2024-04-05 14:43:53.036234 py_ws_libp2p_proxy-0.1.3/LICENSE
+-rw-r--r--   0        0        0      257 2024-04-05 14:43:53.036234 py_ws_libp2p_proxy-0.1.3/README.md
+-rw-r--r--   0        0        0      517 2024-04-05 14:43:53.036234 py_ws_libp2p_proxy-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3877 2024-04-05 14:43:53.036234 py_ws_libp2p_proxy-0.1.3/pyproxy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 14:43:53.036234 py_ws_libp2p_proxy-0.1.3/pyproxy/utils/__init__.py
+-rw-r--r--   0        0        0     2358 2024-04-05 14:43:53.036234 py_ws_libp2p_proxy-0.1.3/pyproxy/utils/decorators.py
+-rw-r--r--   0        0        0       53 2024-04-05 14:43:53.036234 py_ws_libp2p_proxy-0.1.3/pyproxy/utils/logger.py
+-rw-r--r--   0        0        0      794 2024-04-05 14:43:53.036234 py_ws_libp2p_proxy-0.1.3/pyproxy/utils/message.py
+-rw-r--r--   0        0        0      663 2024-04-05 14:43:53.036234 py_ws_libp2p_proxy-0.1.3/pyproxy/utils/protocols_manager.py
+-rw-r--r--   0        0        0     3452 2024-04-05 14:43:53.036234 py_ws_libp2p_proxy-0.1.3/pyproxy/utils/websocket.py
+-rw-r--r--   0        0        0      992 1970-01-01 00:00:00.000000 py_ws_libp2p_proxy-0.1.3/PKG-INFO
```

### Comparing `py_ws_libp2p_proxy-0.1.2b1/LICENSE` & `py_ws_libp2p_proxy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ws_libp2p_proxy-0.1.2b1/pyproject.toml` & `py_ws_libp2p_proxy-0.1.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-ws-libp2p-proxy"
-version = "0.1.2-beta-1"
+version = "0.1.3"
 description = "API for libp2p-ws-proxy"
 authors = [
     "Mariia Livshits <m.bystramovich@gmail.com>",
 ]
 license = "Apache-2.0"
 
 repository = "https://github.com/tubleronchik/py-libp2p-proxy"
```

### Comparing `py_ws_libp2p_proxy-0.1.2b1/pyproxy/__init__.py` & `py_ws_libp2p_proxy-0.1.3/pyproxy/__init__.py`

 * *Files identical despite different names*

### Comparing `py_ws_libp2p_proxy-0.1.2b1/pyproxy/utils/decorators.py` & `py_ws_libp2p_proxy-0.1.3/pyproxy/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `py_ws_libp2p_proxy-0.1.2b1/pyproxy/utils/message.py` & `py_ws_libp2p_proxy-0.1.3/pyproxy/utils/message.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         json_obj = json.loads(data)
         message = {
             "protocol": protocol,
             "serverPeerId": server_peer_id,
             "save_data": save_data,
             "data": {"data": json_obj},
         }
-    except Exception as e:
+    except json.decoder.JSONDecodeError:
         message = {"protocol": protocol, "serverPeerId": server_peer_id, "save_data": save_data, "data": {"data": data}}
     return json.dumps(message)
 
 
 def format_msg_for_subscribing(protocols: list) -> str:
     msg = {"protocols_to_listen": protocols}
     return json.dumps(msg)
```

### Comparing `py_ws_libp2p_proxy-0.1.2b1/pyproxy/utils/protocols_manager.py` & `py_ws_libp2p_proxy-0.1.3/pyproxy/utils/protocols_manager.py`

 * *Files identical despite different names*

### Comparing `py_ws_libp2p_proxy-0.1.2b1/pyproxy/utils/websocket.py` & `py_ws_libp2p_proxy-0.1.3/pyproxy/utils/websocket.py`

 * *Files identical despite different names*

### Comparing `py_ws_libp2p_proxy-0.1.2b1/PKG-INFO` & `py_ws_libp2p_proxy-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ws-libp2p-proxy
-Version: 0.1.2b1
+Version: 0.1.3
 Summary: API for libp2p-ws-proxy
 Home-page: https://github.com/tubleronchik/py-libp2p-proxy
 License: Apache-2.0
 Author: Mariia Livshits
 Author-email: m.bystramovich@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

