# Comparing `tmp/livekit-api-0.4.3.tar.gz` & `tmp/livekit-api-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit-api-0.4.3.tar", last modified: Wed Mar 27 17:01:03 2024, max compression
+gzip compressed data, was "livekit-api-0.4.4.tar", last modified: Fri Apr  5 00:30:50 2024, max compression
```

## Comparing `livekit-api-0.4.3.tar` & `livekit-api-0.4.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:01:03.233644 livekit-api-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-27 17:01:03.233644 livekit-api-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-27 17:00:52.000000 livekit-api-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:01:03.229644 livekit-api-0.4.3/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:01:03.229644 livekit-api-0.4.3/livekit/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-27 17:00:52.000000 livekit-api-0.4.3/livekit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-27 17:00:52.000000 livekit-api-0.4.3/livekit/api/_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-03-27 17:00:52.000000 livekit-api-0.4.3/livekit/api/access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-03-27 17:00:52.000000 livekit-api-0.4.3/livekit/api/egress_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-03-27 17:00:52.000000 livekit-api-0.4.3/livekit/api/ingress_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-27 17:00:52.000000 livekit-api-0.4.3/livekit/api/livekit_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 17:00:52.000000 livekit-api-0.4.3/livekit/api/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-03-27 17:00:52.000000 livekit-api-0.4.3/livekit/api/room_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-03-27 17:00:52.000000 livekit-api-0.4.3/livekit/api/twirp_client.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-27 17:00:52.000000 livekit-api-0.4.3/livekit/api/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-27 17:00:52.000000 livekit-api-0.4.3/livekit/api/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:01:03.233644 livekit-api-0.4.3/livekit_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-27 17:01:03.000000 livekit-api-0.4.3/livekit_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-27 17:01:03.000000 livekit-api-0.4.3/livekit_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 17:01:03.000000 livekit-api-0.4.3/livekit_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-27 17:01:03.000000 livekit-api-0.4.3/livekit_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-27 17:01:03.000000 livekit-api-0.4.3/livekit_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-27 17:00:52.000000 livekit-api-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 17:01:03.233644 livekit-api-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-03-27 17:00:52.000000 livekit-api-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:01:03.233644 livekit-api-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-03-27 17:00:52.000000 livekit-api-0.4.3/tests/test_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-03-27 17:00:52.000000 livekit-api-0.4.3/tests/test_webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:30:50.982386 livekit-api-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-05 00:30:50.982386 livekit-api-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-05 00:30:38.000000 livekit-api-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:30:50.978386 livekit-api-0.4.4/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:30:50.982386 livekit-api-0.4.4/livekit/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-05 00:30:38.000000 livekit-api-0.4.4/livekit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-05 00:30:38.000000 livekit-api-0.4.4/livekit/api/_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-04-05 00:30:38.000000 livekit-api-0.4.4/livekit/api/access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-05 00:30:38.000000 livekit-api-0.4.4/livekit/api/egress_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-05 00:30:38.000000 livekit-api-0.4.4/livekit/api/ingress_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-05 00:30:38.000000 livekit-api-0.4.4/livekit/api/livekit_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:30:38.000000 livekit-api-0.4.4/livekit/api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-05 00:30:38.000000 livekit-api-0.4.4/livekit/api/room_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-05 00:30:38.000000 livekit-api-0.4.4/livekit/api/twirp_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-05 00:30:38.000000 livekit-api-0.4.4/livekit/api/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-05 00:30:38.000000 livekit-api-0.4.4/livekit/api/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:30:50.982386 livekit-api-0.4.4/livekit_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-05 00:30:50.000000 livekit-api-0.4.4/livekit_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-05 00:30:50.000000 livekit-api-0.4.4/livekit_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 00:30:50.000000 livekit-api-0.4.4/livekit_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-05 00:30:50.000000 livekit-api-0.4.4/livekit_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 00:30:50.000000 livekit-api-0.4.4/livekit_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-05 00:30:38.000000 livekit-api-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 00:30:50.982386 livekit-api-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-05 00:30:38.000000 livekit-api-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:30:50.982386 livekit-api-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-05 00:30:38.000000 livekit-api-0.4.4/tests/test_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-05 00:30:38.000000 livekit-api-0.4.4/tests/test_webhook.py
```

### Comparing `livekit-api-0.4.3/PKG-INFO` & `livekit-api-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-api
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python Server API for LiveKit
 Home-page: https://github.com/livekit/python-sdks
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/python-sdks/
 Keywords: webrtc,realtime,audio,video,livekit
@@ -21,12 +21,12 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Requires-Dist: pyjwt>=2.0.0
 Requires-Dist: aiohttp>=3.9.0
 Requires-Dist: protobuf>=3
 Requires-Dist: types-protobuf<5,>=4
-Requires-Dist: livekit-protocol~=0.3.0
+Requires-Dist: livekit-protocol<1,>=0.3.0
 
 # LiveKit Server APIs
 
 Access LiveKit server APIs and generate access tokens.
```

### Comparing `livekit-api-0.4.3/livekit/api/__init__.py` & `livekit-api-0.4.4/livekit/api/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit-api-0.4.3/livekit/api/_service.py` & `livekit-api-0.4.4/livekit/api/_service.py`

 * *Files identical despite different names*

### Comparing `livekit-api-0.4.3/livekit/api/access_token.py` & `livekit-api-0.4.4/livekit/api/access_token.py`

 * *Files identical despite different names*

### Comparing `livekit-api-0.4.3/livekit/api/egress_service.py` & `livekit-api-0.4.4/livekit/api/egress_service.py`

 * *Files identical despite different names*

### Comparing `livekit-api-0.4.3/livekit/api/ingress_service.py` & `livekit-api-0.4.4/livekit/api/ingress_service.py`

 * *Files identical despite different names*

### Comparing `livekit-api-0.4.3/livekit/api/livekit_api.py` & `livekit-api-0.4.4/livekit/api/livekit_api.py`

 * *Files identical despite different names*

### Comparing `livekit-api-0.4.3/livekit/api/room_service.py` & `livekit-api-0.4.4/livekit/api/room_service.py`

 * *Files identical despite different names*

### Comparing `livekit-api-0.4.3/livekit/api/twirp_client.py` & `livekit-api-0.4.4/livekit/api/twirp_client.py`

 * *Files identical despite different names*

### Comparing `livekit-api-0.4.3/livekit/api/webhook.py` & `livekit-api-0.4.4/livekit/api/webhook.py`

 * *Files identical despite different names*

### Comparing `livekit-api-0.4.3/livekit_api.egg-info/PKG-INFO` & `livekit-api-0.4.4/livekit_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-api
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python Server API for LiveKit
 Home-page: https://github.com/livekit/python-sdks
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/python-sdks/
 Keywords: webrtc,realtime,audio,video,livekit
@@ -21,12 +21,12 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Requires-Dist: pyjwt>=2.0.0
 Requires-Dist: aiohttp>=3.9.0
 Requires-Dist: protobuf>=3
 Requires-Dist: types-protobuf<5,>=4
-Requires-Dist: livekit-protocol~=0.3.0
+Requires-Dist: livekit-protocol<1,>=0.3.0
 
 # LiveKit Server APIs
 
 Access LiveKit server APIs and generate access tokens.
```

### Comparing `livekit-api-0.4.3/livekit_api.egg-info/SOURCES.txt` & `livekit-api-0.4.4/livekit_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `livekit-api-0.4.3/setup.py` & `livekit-api-0.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     packages=setuptools.find_namespace_packages(include=["livekit.*"]),
     python_requires=">=3.8.0",
     install_requires=[
         "pyjwt>=2.0.0",
         "aiohttp>=3.9.0",
         "protobuf>=3",
         "types-protobuf>=4,<5",
-        "livekit-protocol~=0.3.0",
+        "livekit-protocol>=0.3.0,<1",
     ],
     package_data={
         "livekit.api": ["py.typed", "*.pyi", "**/*.pyi"],
     },
     project_urls={
         "Documentation": "https://docs.livekit.io",
         "Website": "https://livekit.io/",
```

### Comparing `livekit-api-0.4.3/tests/test_access_token.py` & `livekit-api-0.4.4/tests/test_access_token.py`

 * *Files identical despite different names*

### Comparing `livekit-api-0.4.3/tests/test_webhook.py` & `livekit-api-0.4.4/tests/test_webhook.py`

 * *Files identical despite different names*

