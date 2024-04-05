# Comparing `tmp/crosslab_api_client-0.2.6.tar.gz` & `tmp/crosslab_api_client-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslab_api_client-0.2.6.tar", last modified: Thu Feb  8 15:22:54 2024, max compression
+gzip compressed data, was "crosslab_api_client-0.2.7.tar", last modified: Fri Apr  5 09:16:55 2024, max compression
```

## Comparing `crosslab_api_client-0.2.6.tar` & `crosslab_api_client-0.2.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:22:54.951321 crosslab_api_client-0.2.6/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      418 2024-02-08 15:22:54.951321 crosslab_api_client-0.2.6/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:39.000000 crosslab_api_client-0.2.6/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-11-08 12:05:40.000000 crosslab_api_client-0.2.6/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)      624 2024-02-08 15:22:54.951321 crosslab_api_client-0.2.6/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)       37 2023-11-08 12:05:39.000000 crosslab_api_client-0.2.6/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:22:54.947321 crosslab_api_client-0.2.6/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:22:54.947321 crosslab_api_client-0.2.6/src/crosslab/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:22:54.947321 crosslab_api_client-0.2.6/src/crosslab/api_client/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       58 2023-11-08 12:05:40.000000 crosslab_api_client-0.2.6/src/crosslab/api_client/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    43474 2024-02-08 15:22:48.000000 crosslab_api_client-0.2.6/src/crosslab/api_client/client.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       50 2023-11-08 12:05:40.000000 crosslab_api_client-0.2.6/src/crosslab/api_client/exceptions.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      804 2023-11-08 12:05:40.000000 crosslab_api_client-0.2.6/src/crosslab/api_client/improved_client.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_api_client-0.2.6/src/crosslab/api_client/py.typed
--rw-r--r--   0 vscode    (1000) vscode    (1000)   107292 2024-02-08 15:22:48.000000 crosslab_api_client-0.2.6/src/crosslab/api_client/schemas.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:22:54.951321 crosslab_api_client-0.2.6/src/crosslab_api_client.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      418 2024-02-08 15:22:54.000000 crosslab_api_client-0.2.6/src/crosslab_api_client.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      548 2024-02-08 15:22:54.000000 crosslab_api_client-0.2.6/src/crosslab_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-02-08 15:22:54.000000 crosslab_api_client-0.2.6/src/crosslab_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       42 2024-02-08 15:22:54.000000 crosslab_api_client-0.2.6/src/crosslab_api_client.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2024-02-08 15:22:54.000000 crosslab_api_client-0.2.6/src/crosslab_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:22:54.951321 crosslab_api_client-0.2.6/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      722 2023-11-08 12:05:40.000000 crosslab_api_client-0.2.6/tests/test_improved_client.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)   390623 2024-02-08 15:22:52.000000 crosslab_api_client-0.2.6/tests/test_openapi.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:16:55.774510 crosslab_api_client-0.2.7/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      418 2024-04-05 09:16:55.774510 crosslab_api_client-0.2.7/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:39.000000 crosslab_api_client-0.2.7/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-11-08 12:05:40.000000 crosslab_api_client-0.2.7/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      624 2024-04-05 09:16:55.774510 crosslab_api_client-0.2.7/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       37 2023-11-08 12:05:39.000000 crosslab_api_client-0.2.7/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:16:55.770510 crosslab_api_client-0.2.7/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:16:55.770510 crosslab_api_client-0.2.7/src/crosslab/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:16:55.770510 crosslab_api_client-0.2.7/src/crosslab/api_client/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       58 2023-11-08 12:05:40.000000 crosslab_api_client-0.2.7/src/crosslab/api_client/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    43474 2024-04-05 09:16:48.000000 crosslab_api_client-0.2.7/src/crosslab/api_client/client.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       50 2023-11-08 12:05:40.000000 crosslab_api_client-0.2.7/src/crosslab/api_client/exceptions.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      804 2023-11-08 12:05:40.000000 crosslab_api_client-0.2.7/src/crosslab/api_client/improved_client.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_api_client-0.2.7/src/crosslab/api_client/py.typed
+-rw-r--r--   0 vscode    (1000) vscode    (1000)   107554 2024-04-05 09:16:48.000000 crosslab_api_client-0.2.7/src/crosslab/api_client/schemas.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:16:55.774510 crosslab_api_client-0.2.7/src/crosslab_api_client.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      418 2024-04-05 09:16:55.000000 crosslab_api_client-0.2.7/src/crosslab_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      548 2024-04-05 09:16:55.000000 crosslab_api_client-0.2.7/src/crosslab_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-04-05 09:16:55.000000 crosslab_api_client-0.2.7/src/crosslab_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       42 2024-04-05 09:16:55.000000 crosslab_api_client-0.2.7/src/crosslab_api_client.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2024-04-05 09:16:55.000000 crosslab_api_client-0.2.7/src/crosslab_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:16:55.770510 crosslab_api_client-0.2.7/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      722 2023-11-08 12:05:40.000000 crosslab_api_client-0.2.7/tests/test_improved_client.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)   390588 2024-04-05 09:16:52.000000 crosslab_api_client-0.2.7/tests/test_openapi.py
```

### Comparing `crosslab_api_client-0.2.6/setup.cfg` & `crosslab_api_client-0.2.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosslab_api_client
-version = 0.2.6
+version = 0.2.7
 author = Johannes Nau
 author_email = johannes.nau@tu-ilmenau.de
 description = The CrossLab API Client
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Other/Proprietary License
 	Operating System :: OS Independent
```

### Comparing `crosslab_api_client-0.2.6/src/crosslab/api_client/client.py` & `crosslab_api_client-0.2.7/src/crosslab/api_client/client.py`

 * *Files identical despite different names*

### Comparing `crosslab_api_client-0.2.6/src/crosslab/api_client/improved_client.py` & `crosslab_api_client-0.2.7/src/crosslab/api_client/improved_client.py`

 * *Files identical despite different names*

### Comparing `crosslab_api_client-0.2.6/src/crosslab/api_client/schemas.py` & `crosslab_api_client-0.2.7/src/crosslab/api_client/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1593,15 +1593,27 @@
     - messageType
     - configuration
     """
     messageType: Literal["configuration"]
     configuration: SendSignalingMessageRequestAlt4Configuration
 
 
-SendSignalingMessageRequest = Union[SendSignalingMessageRequestAlt1, SendSignalingMessageRequestAlt2, SendSignalingMessageRequestAlt3, SendSignalingMessageRequestAlt4]
+class SendSignalingMessageRequestAlt5(TypedDict):
+    """
+    Properties:
+    - messageType
+    - status
+    - message
+    """
+    messageType: Literal["experiment-status-changed"]
+    status: str
+    message: NotRequired[str]
+
+
+SendSignalingMessageRequest = Union[SendSignalingMessageRequestAlt1, SendSignalingMessageRequestAlt2, SendSignalingMessageRequestAlt3, SendSignalingMessageRequestAlt4, SendSignalingMessageRequestAlt5]
 
 
 SendSignalingMessageResponse: TypeAlias = None
 
 
 class ListPeerconnectionsResponse200ItemsDevicesItems(TypedDict):
     """
```

### Comparing `crosslab_api_client-0.2.6/src/crosslab_api_client.egg-info/SOURCES.txt` & `crosslab_api_client-0.2.7/src/crosslab_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crosslab_api_client-0.2.6/tests/test_improved_client.py` & `crosslab_api_client-0.2.7/tests/test_improved_client.py`

 * *Files identical despite different names*

### Comparing `crosslab_api_client-0.2.6/tests/test_openapi.py` & `crosslab_api_client-0.2.7/tests/test_openapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -2637,15 +2637,15 @@
 
 @pytest.mark.asyncio
 async def test_send_signaling_message(aioresponses: aioresponses):
     url = r'/devices/c799cc2e-cdc5-4143-973a-6f56a5afa82c/signaling'
     url_variant = r'devices/c799cc2e-cdc5-4143-973a-6f56a5afa82c/signaling'
     full_url = BASE_URL+r'/devices/c799cc2e-cdc5-4143-973a-6f56a5afa82c/signaling'
 
-    request = json.loads(r'{"messageType":"command","command":"closePeerconnection","connectionUrl":"http://XuAPamxDhfIsAsnxNretlqneCY.avbkCVtwesEEf,Dkiw.md"}')
+    request = json.loads(r'{"messageType":"experiment-status-changed","status":"tempor","message":"dolore anim ipsum quis"}')
 
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200)
         async with APIClient(BASE_URL) as client:
             resp = await client.send_signaling_message(url=url, body=request, **parameters)
```

