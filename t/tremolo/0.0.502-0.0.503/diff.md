# Comparing `tmp/tremolo-0.0.502.tar.gz` & `tmp/tremolo-0.0.503.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/tux/tremolo/dist/.tmp-8xhf1ves/tremolo-0.0.502.tar", last modified: Sun Mar 17 03:14:58 2024, max compression
+gzip compressed data, was "/home/tux/tremolo/dist/.tmp-mk54b5aq/tremolo-0.0.503.tar", last modified: Thu Apr  4 22:18:14 2024, max compression
```

## Comparing `tremolo-0.0.502.tar` & `tremolo-0.0.503.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-03-17 03:14:58.000000 tremolo-0.0.502/
--rw-r--r--   0 tux       (1000) users      (100)     1063 2024-02-01 14:00:19.000000 tremolo-0.0.502/LICENSE.txt
--rw-r--r--   0 tux       (1000) users      (100)       63 2024-03-16 12:09:02.000000 tremolo-0.0.502/MANIFEST.in
--rw-r--r--   0 tux       (1000) users      (100)     6473 2024-03-17 03:14:58.000000 tremolo-0.0.502/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)     5683 2024-02-01 14:00:19.000000 tremolo-0.0.502/README.md
--rw-r--r--   0 tux       (1000) users      (100)     1016 2024-03-16 12:09:02.000000 tremolo-0.0.502/pyproject.toml
--rw-r--r--   0 tux       (1000) users      (100)       38 2024-03-17 03:14:58.000000 tremolo-0.0.502/setup.cfg
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-03-17 03:14:58.000000 tremolo-0.0.502/tremolo/
--rw-r--r--   0 tux       (1000) users      (100)      308 2024-03-17 03:12:57.000000 tremolo-0.0.502/tremolo/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)     7213 2024-02-05 09:58:51.000000 tremolo-0.0.502/tremolo/__main__.py
--rw-r--r--   0 tux       (1000) users      (100)     2674 2024-02-20 23:07:43.000000 tremolo-0.0.502/tremolo/asgi_lifespan.py
--rw-r--r--   0 tux       (1000) users      (100)     9909 2024-03-17 03:05:42.000000 tremolo-0.0.502/tremolo/asgi_server.py
--rw-r--r--   0 tux       (1000) users      (100)      681 2024-02-01 14:00:19.000000 tremolo-0.0.502/tremolo/exceptions.py
--rw-r--r--   0 tux       (1000) users      (100)     1139 2024-02-01 14:00:19.000000 tremolo-0.0.502/tremolo/handlers.py
--rw-r--r--   0 tux       (1000) users      (100)    11708 2024-03-17 03:05:59.000000 tremolo-0.0.502/tremolo/http_server.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-03-17 03:14:58.000000 tremolo-0.0.502/tremolo/lib/
--rw-r--r--   0 tux       (1000) users      (100)        0 2024-02-01 14:00:19.000000 tremolo-0.0.502/tremolo/lib/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)      603 2024-02-01 14:00:19.000000 tremolo-0.0.502/tremolo/lib/connections.py
--rw-r--r--   0 tux       (1000) users      (100)      671 2024-02-05 09:57:05.000000 tremolo-0.0.502/tremolo/lib/contexts.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-03-17 03:14:58.000000 tremolo-0.0.502/tremolo/lib/h1parser/
--rw-r--r--   0 tux       (1000) users      (100)       52 2024-02-01 14:00:19.000000 tremolo-0.0.502/tremolo/lib/h1parser/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)     6101 2024-03-05 06:08:34.000000 tremolo-0.0.502/tremolo/lib/h1parser/parse_header.py
--rw-r--r--   0 tux       (1000) users      (100)     2084 2024-02-01 14:00:19.000000 tremolo-0.0.502/tremolo/lib/http_exception.py
--rw-r--r--   0 tux       (1000) users      (100)    18343 2024-03-16 12:09:02.000000 tremolo-0.0.502/tremolo/lib/http_protocol.py
--rw-r--r--   0 tux       (1000) users      (100)    12797 2024-03-08 01:51:43.000000 tremolo-0.0.502/tremolo/lib/http_request.py
--rw-r--r--   0 tux       (1000) users      (100)    15565 2024-03-17 03:05:59.000000 tremolo-0.0.502/tremolo/lib/http_response.py
--rw-r--r--   0 tux       (1000) users      (100)     1896 2024-02-01 14:00:19.000000 tremolo-0.0.502/tremolo/lib/locks.py
--rw-r--r--   0 tux       (1000) users      (100)      919 2024-03-05 03:41:31.000000 tremolo-0.0.502/tremolo/lib/pools.py
--rw-r--r--   0 tux       (1000) users      (100)     1170 2024-02-25 01:31:07.000000 tremolo-0.0.502/tremolo/lib/queue.py
--rw-r--r--   0 tux       (1000) users      (100)     1199 2024-03-08 01:52:01.000000 tremolo-0.0.502/tremolo/lib/request.py
--rw-r--r--   0 tux       (1000) users      (100)     1465 2024-02-01 14:00:19.000000 tremolo-0.0.502/tremolo/lib/response.py
--rw-r--r--   0 tux       (1000) users      (100)      534 2024-02-01 14:00:19.000000 tremolo-0.0.502/tremolo/lib/tasks.py
--rw-r--r--   0 tux       (1000) users      (100)     6064 2024-02-01 14:00:19.000000 tremolo-0.0.502/tremolo/lib/websocket.py
--rw-r--r--   0 tux       (1000) users      (100)    28041 2024-02-05 09:58:51.000000 tremolo-0.0.502/tremolo/tremolo.py
--rw-r--r--   0 tux       (1000) users      (100)     1076 2024-02-05 09:58:51.000000 tremolo-0.0.502/tremolo/utils.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-03-17 03:14:58.000000 tremolo-0.0.502/tremolo.egg-info/
--rw-r--r--   0 tux       (1000) users      (100)     6473 2024-03-17 03:14:58.000000 tremolo-0.0.502/tremolo.egg-info/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)      778 2024-03-17 03:14:58.000000 tremolo-0.0.502/tremolo.egg-info/SOURCES.txt
--rw-r--r--   0 tux       (1000) users      (100)        1 2024-03-17 03:14:58.000000 tremolo-0.0.502/tremolo.egg-info/dependency_links.txt
--rw-r--r--   0 tux       (1000) users      (100)        8 2024-03-17 03:14:58.000000 tremolo-0.0.502/tremolo.egg-info/top_level.txt
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-04 22:18:14.000000 tremolo-0.0.503/
+-rw-r--r--   0 tux       (1000) users      (100)     1063 2024-02-01 14:00:19.000000 tremolo-0.0.503/LICENSE.txt
+-rw-r--r--   0 tux       (1000) users      (100)       63 2024-03-16 12:09:02.000000 tremolo-0.0.503/MANIFEST.in
+-rw-r--r--   0 tux       (1000) users      (100)     6473 2024-04-04 22:18:14.000000 tremolo-0.0.503/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)     5683 2024-02-01 14:00:19.000000 tremolo-0.0.503/README.md
+-rw-r--r--   0 tux       (1000) users      (100)     1016 2024-03-16 12:09:02.000000 tremolo-0.0.503/pyproject.toml
+-rw-r--r--   0 tux       (1000) users      (100)       38 2024-04-04 22:18:14.000000 tremolo-0.0.503/setup.cfg
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-04 22:18:14.000000 tremolo-0.0.503/tremolo/
+-rw-r--r--   0 tux       (1000) users      (100)      308 2024-04-04 22:17:18.000000 tremolo-0.0.503/tremolo/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)     7213 2024-02-05 09:58:51.000000 tremolo-0.0.503/tremolo/__main__.py
+-rw-r--r--   0 tux       (1000) users      (100)     2674 2024-02-20 23:07:43.000000 tremolo-0.0.503/tremolo/asgi_lifespan.py
+-rw-r--r--   0 tux       (1000) users      (100)     9894 2024-03-30 10:03:11.000000 tremolo-0.0.503/tremolo/asgi_server.py
+-rw-r--r--   0 tux       (1000) users      (100)      681 2024-02-01 14:00:19.000000 tremolo-0.0.503/tremolo/exceptions.py
+-rw-r--r--   0 tux       (1000) users      (100)     1139 2024-02-01 14:00:19.000000 tremolo-0.0.503/tremolo/handlers.py
+-rw-r--r--   0 tux       (1000) users      (100)    11708 2024-03-27 21:22:49.000000 tremolo-0.0.503/tremolo/http_server.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-04 22:18:14.000000 tremolo-0.0.503/tremolo/lib/
+-rw-r--r--   0 tux       (1000) users      (100)        0 2024-02-01 14:00:19.000000 tremolo-0.0.503/tremolo/lib/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)      603 2024-02-01 14:00:19.000000 tremolo-0.0.503/tremolo/lib/connections.py
+-rw-r--r--   0 tux       (1000) users      (100)      671 2024-02-05 09:57:05.000000 tremolo-0.0.503/tremolo/lib/contexts.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-04 22:18:14.000000 tremolo-0.0.503/tremolo/lib/h1parser/
+-rw-r--r--   0 tux       (1000) users      (100)       52 2024-02-01 14:00:19.000000 tremolo-0.0.503/tremolo/lib/h1parser/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)     6101 2024-03-05 06:08:34.000000 tremolo-0.0.503/tremolo/lib/h1parser/parse_header.py
+-rw-r--r--   0 tux       (1000) users      (100)     2084 2024-02-01 14:00:19.000000 tremolo-0.0.503/tremolo/lib/http_exception.py
+-rw-r--r--   0 tux       (1000) users      (100)    18343 2024-03-16 12:09:02.000000 tremolo-0.0.503/tremolo/lib/http_protocol.py
+-rw-r--r--   0 tux       (1000) users      (100)    12797 2024-03-08 01:51:43.000000 tremolo-0.0.503/tremolo/lib/http_request.py
+-rw-r--r--   0 tux       (1000) users      (100)    15760 2024-04-04 21:42:22.000000 tremolo-0.0.503/tremolo/lib/http_response.py
+-rw-r--r--   0 tux       (1000) users      (100)     1896 2024-02-01 14:00:19.000000 tremolo-0.0.503/tremolo/lib/locks.py
+-rw-r--r--   0 tux       (1000) users      (100)      919 2024-03-05 03:41:31.000000 tremolo-0.0.503/tremolo/lib/pools.py
+-rw-r--r--   0 tux       (1000) users      (100)     1170 2024-02-25 01:31:07.000000 tremolo-0.0.503/tremolo/lib/queue.py
+-rw-r--r--   0 tux       (1000) users      (100)     1199 2024-03-08 01:52:01.000000 tremolo-0.0.503/tremolo/lib/request.py
+-rw-r--r--   0 tux       (1000) users      (100)     1460 2024-04-01 02:53:44.000000 tremolo-0.0.503/tremolo/lib/response.py
+-rw-r--r--   0 tux       (1000) users      (100)      534 2024-02-01 14:00:19.000000 tremolo-0.0.503/tremolo/lib/tasks.py
+-rw-r--r--   0 tux       (1000) users      (100)     6064 2024-02-01 14:00:19.000000 tremolo-0.0.503/tremolo/lib/websocket.py
+-rw-r--r--   0 tux       (1000) users      (100)    28028 2024-04-04 22:17:18.000000 tremolo-0.0.503/tremolo/tremolo.py
+-rw-r--r--   0 tux       (1000) users      (100)     1095 2024-04-04 21:42:22.000000 tremolo-0.0.503/tremolo/utils.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-04 22:18:14.000000 tremolo-0.0.503/tremolo.egg-info/
+-rw-r--r--   0 tux       (1000) users      (100)     6473 2024-04-04 22:18:14.000000 tremolo-0.0.503/tremolo.egg-info/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)      778 2024-04-04 22:18:14.000000 tremolo-0.0.503/tremolo.egg-info/SOURCES.txt
+-rw-r--r--   0 tux       (1000) users      (100)        1 2024-04-04 22:18:14.000000 tremolo-0.0.503/tremolo.egg-info/dependency_links.txt
+-rw-r--r--   0 tux       (1000) users      (100)        8 2024-04-04 22:18:14.000000 tremolo-0.0.503/tremolo.egg-info/top_level.txt
```

### Comparing `tremolo-0.0.502/LICENSE.txt` & `tremolo-0.0.503/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.502/PKG-INFO` & `tremolo-0.0.503/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.502
+Version: 0.0.503
 Summary: Tremolo is a stream-oriented, asynchronous, programmable HTTP server written in pure Python. It can also serve as an ASGI server.
 Author-email: nggit <contact@anggit.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/nggit/tremolo
 Project-URL: Source, https://github.com/nggit/tremolo
 Project-URL: Funding, https://github.com/sponsors/nggit
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tremolo-0.0.502/README.md` & `tremolo-0.0.503/README.md`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.502/pyproject.toml` & `tremolo-0.0.503/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.502/tremolo/__main__.py` & `tremolo-0.0.503/tremolo/__main__.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.502/tremolo/asgi_lifespan.py` & `tremolo-0.0.503/tremolo/asgi_lifespan.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.502/tremolo/asgi_server.py` & `tremolo-0.0.503/tremolo/asgi_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,17 @@
 
         self._scope['type'] = 'websocket'
         self._scope['scheme'] = _WS_OR_WSS[self.request.scheme == b'https']
         self._scope['subprotocols'] = [
             value.decode('latin-1') for value in
             self.request.headers.getlist(b'sec-websocket-protocol')]
 
-    async def _handle_http(self):
+    def _handle_http(self):
+        self._read = self.request.stream()
+
         self._scope['type'] = 'http'
         self._scope['method'] = self.request.method.decode('latin-1')
         self._scope['scheme'] = self.request.scheme.decode('latin-1')
 
     async def headers_received(self):
         if not self.request.is_valid:
             await error_400(request=self.request, response=self.response)
@@ -71,16 +73,15 @@
 
         if (self.options['ws'] and b'upgrade' in self.request.headers and
                 b'connection' in self.request.headers and
                 b'sec-websocket-key' in self.request.headers and
                 self.request.headers[b'upgrade'].lower() == b'websocket'):
             self._handle_websocket()
         else:
-            await self._handle_http()
-            self._read = self.request.stream()
+            self._handle_http()
 
         # the current task is done
         # update the handler with the ASGI main task
         self.handler = self.loop.create_task(self.main())
 
     async def handle_error_500(self, exc):
         return await error_500(
```

### Comparing `tremolo-0.0.502/tremolo/exceptions.py` & `tremolo-0.0.503/tremolo/exceptions.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.502/tremolo/handlers.py` & `tremolo-0.0.503/tremolo/handlers.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.502/tremolo/http_server.py` & `tremolo-0.0.503/tremolo/http_server.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.502/tremolo/lib/connections.py` & `tremolo-0.0.503/tremolo/lib/connections.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.502/tremolo/lib/contexts.py` & `tremolo-0.0.503/tremolo/lib/contexts.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.502/tremolo/lib/h1parser/parse_header.py` & `tremolo-0.0.503/tremolo/lib/h1parser/parse_header.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.502/tremolo/lib/http_exception.py` & `tremolo-0.0.503/tremolo/lib/http_exception.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.502/tremolo/lib/http_protocol.py` & `tremolo-0.0.503/tremolo/lib/http_protocol.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.502/tremolo/lib/http_request.py` & `tremolo-0.0.503/tremolo/lib/http_request.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.502/tremolo/lib/http_response.py` & `tremolo-0.0.503/tremolo/lib/http_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) 2023 nggit
 
 import os
 import time
 
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 from urllib.parse import quote
 
 from .http_exception import (
     BadRequest, ExpectationFailed, InternalServerError, RangeNotSatisfiable
 )
 from .response import Response
 
@@ -89,17 +89,19 @@
             httponly=False,
             samesite=None
             ):
         if isinstance(name, str):
             name = name.encode('latin-1')
 
         value = quote(value).encode('latin-1')
-        date_expired = ((datetime.utcnow() + timedelta(seconds=expires))
-                        .strftime('%a, %d %b %Y %H:%M:%S GMT')
-                        .encode('latin-1'))
+        date_expired = (
+            (datetime.now(timezone.utc) + timedelta(seconds=expires))
+            .strftime('%a, %d %b %Y %H:%M:%S GMT')
+            .encode('latin-1')
+        )
         path = quote(path).encode('latin-1')
 
         cookie = bytearray(
             b'%s=%s; expires=%s; max-age=%d; path=%s' % (
                 name, value, date_expired, expires, path)
         )
 
@@ -223,27 +225,26 @@
                     data), throttle=False, **kwargs
             )
 
             self.headers_sent(True)
 
         self.close(keepalive=keepalive)
 
-    async def write(self, data, buffer_size=16 * 1024, **kwargs):
+    async def write(self, data, chunked=None, buffer_size=16 * 1024, **kwargs):
         kwargs['buffer_size'] = buffer_size
 
         if not self.headers_sent():
             if b'_line' not in self.headers:
                 # this block is executed when write() is called outside the
                 # handler/middleware. e.g. ASGI server
                 self.set_base_header()
 
                 status = self.get_status()
                 no_content = (status[0] in (204, 205, 304) or
                               100 <= status[0] < 200)
-                chunked = kwargs.get('chunked')
 
                 if chunked is None:
                     self.http_chunked = (self._request.version == b'1.1' and
                                          not no_content)
                 else:
                     self.http_chunked = chunked
 
@@ -298,16 +299,18 @@
             await self.send(data, **kwargs)
 
     async def sendfile(
             self,
             path,
             file_size=None,
             buffer_size=16 * 1024,
-            content_type=b'application/octet-stream'
-            ):
+            content_type=b'application/octet-stream',
+            **kwargs):
+        kwargs['buffer_size'] = buffer_size
+
         try:
             handle = self._request.context.RESPONSE_SENDFILE_HANDLE
         except AttributeError:
             handle = open(path, 'rb')
             self._request.context.RESPONSE_SENDFILE_HANDLE = handle
 
             self._request.context.tasks.append(
@@ -332,15 +335,15 @@
                 self.set_header(b'Accept-Ranges', b'bytes')
 
                 data = True
 
                 while data:
                     data = handle.read(buffer_size)
 
-                    await self.write(data, chunked=False)
+                    await self.write(data, chunked=False, **kwargs)
 
                 self.close(keepalive=True)
                 return
 
             _range = self._request.headers[b'range']
 
             if isinstance(_range, list):
@@ -403,15 +406,15 @@
                     b'Content-Range', b'bytes %d-%d/%d' % (
                         start, end, file_size)
                 )
                 handle.seek(start)
 
                 while size > 0:
                     await self.write(handle.read(min(size, buffer_size)),
-                                     chunked=False)
+                                     chunked=False, **kwargs)
                     size -= buffer_size
             else:
                 client = self._request.client
 
                 if client is None:
                     fileno = self._request.socket.fileno()
                     client = (str(fileno), fileno)
@@ -428,26 +431,29 @@
                     b'multipart/byteranges; boundary=%s' % boundary
                 )
 
                 for start, end, size in ranges:
                     await self.write(
                         b'--%s\r\nContent-Type: %s\r\n'
                         b'Content-Range: bytes %d-%d/%d\r\n\r\n' % (
-                            boundary, content_type, start, end, file_size)
+                            boundary, content_type, start, end, file_size),
+                        **kwargs
                     )
                     handle.seek(start)
 
                     while size > 0:
-                        await self.write(handle.read(min(size, buffer_size)))
+                        await self.write(
+                            handle.read(min(size, buffer_size)), **kwargs
+                        )
                         size -= buffer_size
 
-                    await self.write(b'\r\n')
+                    await self.write(b'\r\n', **kwargs)
 
-                await self.write(b'--%s--\r\n' % boundary)
-                await self.write(b'')
+                await self.write(b'--%s--\r\n' % boundary, **kwargs)
+                await self.write(b'', **kwargs)
         else:
             if (b'if-modified-since' in self._request.headers and
                     self._request.headers[b'if-modified-since'] == mdate):
                 self.set_status(304, b'Not Modified')
                 await self.write(None)
                 return
 
@@ -459,10 +465,10 @@
                 self.set_header(b'Accept-Ranges', b'bytes')
 
             data = True
 
             while data:
                 data = handle.read(buffer_size)
 
-                await self.write(data, chunked=False)
+                await self.write(data, chunked=False, **kwargs)
 
         self.close(keepalive=True)
```

### Comparing `tremolo-0.0.502/tremolo/lib/locks.py` & `tremolo-0.0.503/tremolo/lib/locks.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.502/tremolo/lib/pools.py` & `tremolo-0.0.503/tremolo/lib/pools.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.502/tremolo/lib/queue.py` & `tremolo-0.0.503/tremolo/lib/queue.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.502/tremolo/lib/request.py` & `tremolo-0.0.503/tremolo/lib/request.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.502/tremolo/lib/response.py` & `tremolo-0.0.503/tremolo/lib/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     async def send(
             self,
             data,
             throttle=True,
             rate=1048576,
             buffer_size=16 * 1024,
-            buffer_min_size=None, **_
+            buffer_min_size=None
             ):
         if data is None:
             __class__.close(self)
             return
 
         if not isinstance(data, (bytes, bytearray)):
             raise TypeError('expected None or bytes-like object')
```

### Comparing `tremolo-0.0.502/tremolo/lib/tasks.py` & `tremolo-0.0.503/tremolo/lib/tasks.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.502/tremolo/lib/websocket.py` & `tremolo-0.0.503/tremolo/lib/websocket.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.502/tremolo/tremolo.py` & `tremolo-0.0.503/tremolo/tremolo.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,15 +306,15 @@
             )
             print(
                 getattr(options['app'], '__name__',
                         options['app'].__class__.__name__)
             )
 
             if server_name != b'':
-                server_name = server_name + b' (ASGI)'
+                server_name += b' (ASGI)'
 
             lifespan = ASGILifespan(options['app'],
                                     loop=self._loop, logger=self._logger)
 
             lifespan.startup()
             exc = await lifespan.exception()
```

### Comparing `tremolo-0.0.502/tremolo/utils.py` & `tremolo-0.0.503/tremolo/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 __all__ = (
     'file_signature', 'html_escape', 'log_date', 'memory_usage', 'server_date'
 )
 
 import os  # noqa: E402
 import stat  # noqa: E402
 
-from datetime import datetime  # noqa: E402
+from datetime import datetime, timezone  # noqa: E402
 from html import escape  # noqa: E402
 
 
 def file_signature(path):
     st = os.stat(path)
 
     return (stat.S_IFMT(st.st_mode), st.st_size, st.st_mtime)
@@ -40,9 +40,9 @@
             return int(f.read().split()[1]) * os.sysconf('SC_PAGESIZE') // 1024
     except FileNotFoundError:
         # non-Linux
         return -1
 
 
 def server_date():
-    return datetime.utcnow().strftime(
+    return datetime.now(timezone.utc).strftime(
         '%a, %d %b %Y %H:%M:%S GMT').encode('latin-1')
```

### Comparing `tremolo-0.0.502/tremolo.egg-info/PKG-INFO` & `tremolo-0.0.503/tremolo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.502
+Version: 0.0.503
 Summary: Tremolo is a stream-oriented, asynchronous, programmable HTTP server written in pure Python. It can also serve as an ASGI server.
 Author-email: nggit <contact@anggit.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/nggit/tremolo
 Project-URL: Source, https://github.com/nggit/tremolo
 Project-URL: Funding, https://github.com/sponsors/nggit
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tremolo-0.0.502/tremolo.egg-info/SOURCES.txt` & `tremolo-0.0.503/tremolo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

