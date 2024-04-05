# Comparing `tmp/sse_starlette-1.8.2.tar.gz` & `tmp/sse_starlette-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sse_starlette-1.8.2.tar", last modified: Sat Nov 25 09:53:43 2023, max compression
+gzip compressed data, was "sse_starlette-2.0.0.tar", last modified: Thu Jan 25 18:47:59 2024, max compression
```

## Comparing `sse_starlette-1.8.2.tar` & `sse_starlette-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0      395 2022-12-16 17:29:08.125024 sse_starlette-1.8.2/AUTHORS
--rw-r--r--   0        0        0     1892 2023-03-11 18:12:47.645028 sse_starlette-1.8.2/CHANGELOG.md
--rw-r--r--   0        0        0     1511 2022-12-16 17:29:08.125878 sse_starlette-1.8.2/LICENSE
--rw-r--r--   0        0        0     1511 2022-12-16 17:29:08.125878 sse_starlette-1.8.2/LICENSE
--rw-r--r--   0        0        0     4500 2023-09-16 08:49:33.252125 sse_starlette-1.8.2/README.md
--rw-r--r--   0        0        0     4500 2023-09-16 08:49:33.252125 sse_starlette-1.8.2/README.md
--rw-r--r--   0        0        0     2695 2023-11-25 09:53:43.563906 sse_starlette-1.8.2/pyproject.toml
--rw-r--r--   0        0        0      143 2023-11-25 09:53:18.907460 sse_starlette-1.8.2/sse_starlette/__init__.py
--rw-r--r--   0        0        0        0 2022-12-16 17:29:08.136356 sse_starlette-1.8.2/sse_starlette/py.typed
--rw-r--r--   0        0        0    11710 2023-11-25 09:53:03.339200 sse_starlette-1.8.2/sse_starlette/sse.py
--rw-r--r--   0        0        0     2564 2023-09-16 08:49:33.265564 sse_starlette-1.8.2/tests/conftest.py
--rw-r--r--   0        0        0      865 2023-05-21 10:08:33.120835 sse_starlette-1.8.2/tests/integration/README.md
--rw-r--r--   0        0        0      861 2023-05-21 10:01:43.588202 sse_starlette-1.8.2/tests/integration/integration_testing.http
--rw-r--r--   0        0        0      884 2023-09-16 08:49:33.269301 sse_starlette-1.8.2/tests/integration/main_endless.py
--rw-r--r--   0        0        0     2019 2023-09-16 08:49:33.271118 sse_starlette-1.8.2/tests/integration/main_endless_conditional.py
--rw-r--r--   0        0        0      289 2023-09-16 08:49:33.273161 sse_starlette-1.8.2/tests/integration/test_conditional_yielding_endpoint.py
--rw-r--r--   0        0        0     6053 2023-09-16 08:49:33.275369 sse_starlette-1.8.2/tests/integration/test_multiple_consumers.py
--rw-r--r--   0        0        0     4911 2023-09-30 09:32:26.974760 sse_starlette-1.8.2/tests/test_event_source_response.py
--rw-r--r--   0        0        0     3542 2023-09-16 08:49:33.279894 sse_starlette-1.8.2/tests/test_sse.py
--rw-r--r--   0        0        0      807 2023-11-19 17:43:09.772139 sse_starlette-1.8.2/tox.ini
--rw-r--r--   0        0        0     5398 1970-01-01 00:00:00.000000 sse_starlette-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0      395 2022-12-16 17:29:08.125024 sse_starlette-2.0.0/AUTHORS
+-rw-r--r--   0        0        0     1892 2023-03-11 18:12:47.645028 sse_starlette-2.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1511 2022-12-16 17:29:08.125878 sse_starlette-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1511 2022-12-16 17:29:08.125878 sse_starlette-2.0.0/LICENSE
+-rw-r--r--   0        0        0     4500 2023-09-16 08:49:33.252125 sse_starlette-2.0.0/README.md
+-rw-r--r--   0        0        0     4500 2023-09-16 08:49:33.252125 sse_starlette-2.0.0/README.md
+-rw-r--r--   0        0        0     2743 2024-01-25 18:47:59.263606 sse_starlette-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      143 2024-01-25 18:30:49.171417 sse_starlette-2.0.0/sse_starlette/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-16 17:29:08.136356 sse_starlette-2.0.0/sse_starlette/py.typed
+-rw-r--r--   0        0        0    12085 2024-01-25 17:55:21.827560 sse_starlette-2.0.0/sse_starlette/sse.py
+-rw-r--r--   0        0        0      992 2024-01-25 17:55:21.827883 sse_starlette-2.0.0/tests/anyio_compat.py
+-rw-r--r--   0        0        0     2565 2024-01-25 18:37:49.308924 sse_starlette-2.0.0/tests/conftest.py
+-rw-r--r--   0        0        0      865 2023-05-21 10:08:33.120835 sse_starlette-2.0.0/tests/integration/README.md
+-rw-r--r--   0        0        0     1135 2024-01-25 18:37:49.324343 sse_starlette-2.0.0/tests/integration/frozen_client.py
+-rw-r--r--   0        0        0      861 2023-05-21 10:01:43.588202 sse_starlette-2.0.0/tests/integration/integration_testing.http
+-rw-r--r--   0        0        0      885 2024-01-25 18:37:49.318749 sse_starlette-2.0.0/tests/integration/main_endless.py
+-rw-r--r--   0        0        0     2020 2024-01-25 18:37:49.327932 sse_starlette-2.0.0/tests/integration/main_endless_conditional.py
+-rw-r--r--   0        0        0      290 2024-01-25 18:37:49.332256 sse_starlette-2.0.0/tests/integration/test_conditional_yielding_endpoint.py
+-rw-r--r--   0        0        0     6053 2023-09-16 08:49:33.275369 sse_starlette-2.0.0/tests/integration/test_multiple_consumers.py
+-rw-r--r--   0        0        0     5838 2024-01-25 18:37:48.787548 sse_starlette-2.0.0/tests/test_event_source_response.py
+-rw-r--r--   0        0        0     3543 2024-01-25 18:37:49.316228 sse_starlette-2.0.0/tests/test_sse.py
+-rw-r--r--   0        0        0      799 2024-01-25 17:55:21.829586 sse_starlette-2.0.0/tox.ini
+-rw-r--r--   0        0        0     5444 1970-01-01 00:00:00.000000 sse_starlette-2.0.0/PKG-INFO
```

### Comparing `sse_starlette-1.8.2/CHANGELOG.md` & `sse_starlette-2.0.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `sse_starlette-1.8.2/LICENSE` & `sse_starlette-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sse_starlette-1.8.2/README.md` & `sse_starlette-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `sse_starlette-1.8.2/pyproject.toml` & `sse_starlette-2.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "sse-starlette"
-version = "1.8.2"
+version = "2.0.0"
 description = "SSE plugin for Starlette"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
     { name = "sysid", email = "sysid@gmx.de" },
 ]
 url = "https://github.com/sysid/sse-starlette"
@@ -26,26 +26,30 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Internet :: WWW/HTTP",
 ]
 dependencies = [
     "starlette",
     "uvicorn",
-    "fastapi",
     "anyio",
 ]
 
 [project.license]
 text = "BSD-3-Clause"
 
 [project.urls]
 Source = "https://github.com/sysid/sse-starlette"
 
+[project.optional-dependencies]
+examples = [
+    "fastapi",
+]
+
 [tool.bumpversion]
-current_version = "1.8.2"
+current_version = "2.0.0"
 commit = true
 tag = false
 message = "Bump version to {new_version}"
 files = [
     { filename = "VERSION" },
     { filename = "pyproject.toml" },
     { filename = "sse_starlette/__init__.py" },
```

### Comparing `sse_starlette-1.8.2/sse_starlette/sse.py` & `sse_starlette-2.0.0/sse_starlette/sse.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 from starlette.concurrency import iterate_in_threadpool
 from starlette.responses import Response
 from starlette.types import Receive, Scope, Send
 
 _log = logging.getLogger(__name__)
 
 
+class SendTimeoutError(TimeoutError):
+    pass
+
+
 # https://stackoverflow.com/questions/58133694/graceful-shutdown-of-uvicorn-starlette-app-with-websockets
 class AppStatus:
     """helper for monkey-patching the signal-handler of uvicorn"""
 
     should_exit = False
     should_exit_event: Union[anyio.Event, None] = None
 
@@ -167,14 +171,15 @@
         background: Optional[BackgroundTask] = None,
         ping: Optional[int] = None,
         sep: Optional[str] = None,
         ping_message_factory: Optional[Callable[[], ServerSentEvent]] = None,
         data_sender_callable: Optional[
             Callable[[], Coroutine[None, None, None]]
         ] = None,
+        send_timeout: Optional[float] = None,
     ) -> None:
         if sep is not None and sep not in ["\r\n", "\r", "\n"]:
             raise ValueError(f"sep must be one of: \\r\\n, \\r, \\n, got: {sep}")
         self.DEFAULT_SEPARATOR = "\r\n"
         self.sep = sep if sep is not None else self.DEFAULT_SEPARATOR
 
         self.ping_message_factory = ping_message_factory
@@ -183,14 +188,15 @@
             self.body_iterator = content
         else:
             self.body_iterator = iterate_in_threadpool(content)
         self.status_code = status_code
         self.media_type = self.media_type if media_type is None else media_type
         self.background = background
         self.data_sender_callable = data_sender_callable
+        self.send_timeout = send_timeout
 
         _headers: dict[str, str] = {}
         if headers is not None:  # pragma: no cover
             _headers.update(headers)
 
         # mandatory for servers-sent events headers
         # allow cache control header to be set by user to support fan out proxies
@@ -241,15 +247,21 @@
                 "status": self.status_code,
                 "headers": self.raw_headers,
             }
         )
         async for data in self.body_iterator:
             chunk = ensure_bytes(data, self.sep)
             _log.debug(f"chunk: {chunk.decode()}")
-            await send({"type": "http.response.body", "body": chunk, "more_body": True})
+            with anyio.move_on_after(self.send_timeout) as timeout:
+                await send(
+                    {"type": "http.response.body", "body": chunk, "more_body": True}
+                )
+            if timeout.cancel_called:
+                await self.body_iterator.aclose()
+                raise SendTimeoutError()
 
         async with self._send_lock:
             self.active = False
             await send({"type": "http.response.body", "body": b"", "more_body": False})
 
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         async with anyio.create_task_group() as task_group:
```

### Comparing `sse_starlette-1.8.2/tests/conftest.py` & `sse_starlette-2.0.0/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import asyncio
 import logging
 
 import httpx
 import pytest
 from asgi_lifespan import LifespanManager
-from sse_starlette import EventSourceResponse
-from sse_starlette.sse import AppStatus
 from starlette.applications import Starlette
 from starlette.requests import Request
 from starlette.responses import PlainTextResponse
 from starlette.routing import Route
 from starlette.testclient import TestClient
 
+from sse_starlette import EventSourceResponse
+from sse_starlette.sse import AppStatus
+
 _log = logging.getLogger(__name__)
 log_fmt = r"%(asctime)-15s %(levelname)s %(name)s %(funcName)s:%(lineno)d %(message)s"
 datefmt = "%Y-%m-%d %H:%M:%S"
 logging.basicConfig(format=log_fmt, level=logging.DEBUG, datefmt=datefmt)
 
 logging.getLogger("httpx").setLevel(logging.INFO)
 logging.getLogger("httpcore").setLevel(logging.INFO)
```

### Comparing `sse_starlette-1.8.2/tests/integration/README.md` & `sse_starlette-2.0.0/tests/integration/README.md`

 * *Files identical despite different names*

### Comparing `sse_starlette-1.8.2/tests/integration/integration_testing.http` & `sse_starlette-2.0.0/tests/integration/integration_testing.http`

 * *Files identical despite different names*

### Comparing `sse_starlette-1.8.2/tests/integration/main_endless.py` & `sse_starlette-2.0.0/tests/integration/main_endless.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # main.py
 import asyncio
 import logging
 
-from sse_starlette import EventSourceResponse
 from starlette.applications import Starlette
 from starlette.requests import Request
 from starlette.routing import Route
 
+from sse_starlette import EventSourceResponse
+
 _log = logging.getLogger(__name__)
 
 
 async def endless(req: Request):
     async def event_publisher():
         i = 0
         try:
```

### Comparing `sse_starlette-1.8.2/tests/integration/main_endless_conditional.py` & `sse_starlette-2.0.0/tests/integration/main_endless_conditional.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # main.py
 import asyncio
 import logging
 
 import uvicorn
-from sse_starlette import EventSourceResponse
 from starlette.applications import Starlette
 from starlette.requests import Request
 from starlette.routing import Route
 
+from sse_starlette import EventSourceResponse
+
 """
 example by: justindujardin
 4efaffc2365a85f132ab8fc405110120c9c9e36a, https://github.com/sysid/sse-starlette/pull/13
 
 tests proper shutdown in case no messages are yielded:
 - in a streaming endpoint that reports only on "new" data, it is possible to get into a state
     where no no yields are expected to happen in the near future.
```

### Comparing `sse_starlette-1.8.2/tests/integration/test_multiple_consumers.py` & `sse_starlette-2.0.0/tests/integration/test_multiple_consumers.py`

 * *Files identical despite different names*

### Comparing `sse_starlette-1.8.2/tests/test_event_source_response.py` & `sse_starlette-2.0.0/tests/test_event_source_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 import logging
 import math
 from functools import partial
 
 import anyio
 import anyio.lowlevel
 import pytest
-from sse_starlette import EventSourceResponse
 from starlette.testclient import TestClient
 
+from sse_starlette import EventSourceResponse
+from sse_starlette.sse import SendTimeoutError
+from tests.anyio_compat import collapse_excgroups
+
 _log = logging.getLogger(__name__)
 
 
 @pytest.mark.parametrize(
     "input,sep,expected",
     [
         ("integer", "\r\n", b"data: 1\r\n\r\n"),
@@ -120,23 +123,51 @@
         # noinspection PyAsyncCall
         lock.release()
 
     async def receive():
         await anyio.lowlevel.checkpoint()
         return {"type": "something"}
 
+    response = EventSourceResponse(event_publisher(), ping=1)
     with pytest.raises(anyio.WouldBlock) as e:
-        response = EventSourceResponse(event_publisher(), ping=1)
+        with collapse_excgroups():
+            await response({}, receive, send)
 
-        await response({}, receive, send)
 
-
-def test_header_charset():
+def test_header_charset(reset_appstatus_event):
     async def numbers(minimum, maximum):
         for i in range(minimum, maximum + 1):
-            await asyncio.sleep(0.1)
+            await anyio.sleep(0.1)
             yield i
 
     generator = numbers(1, 5)
     response = EventSourceResponse(generator, ping=0.2)  # type: ignore
     content_type = [h for h in response.raw_headers if h[0].decode() == "content-type"]
     assert content_type == [(b"content-type", b"text/event-stream; charset=utf-8")]
+
+
+@pytest.mark.anyio
+async def test_send_timeout(reset_appstatus_event):
+    # Timeout is set to 0.5s, but `send` will take 1s. Expect SendTimeoutError.
+    cleanup = False
+
+    async def event_publisher():
+        try:
+            yield {"event": "some", "data": "any"}
+            assert False  # never reached
+        finally:
+            nonlocal cleanup
+            cleanup = True
+
+    async def send(*args, **kwargs):
+        await anyio.sleep(1.0)
+
+    async def receive():
+        await anyio.lowlevel.checkpoint()
+        return {"type": "something"}
+
+    response = EventSourceResponse(event_publisher(), send_timeout=0.5)
+    with pytest.raises(SendTimeoutError):
+        with collapse_excgroups():
+            await response({}, receive, send)
+
+    assert cleanup
```

### Comparing `sse_starlette-1.8.2/tests/test_sse.py` & `sse_starlette-2.0.0/tests/test_sse.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+
 from sse_starlette.sse import EventSourceResponse, ServerSentEvent, ensure_bytes
 
 
 def test_compression_not_implemented():
     response = EventSourceResponse(0)
     with pytest.raises(NotImplementedError):
         response.enable_compression()
```

### Comparing `sse_starlette-1.8.2/PKG-INFO` & `sse_starlette-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sse-starlette
-Version: 1.8.2
+Version: 2.0.0
 Summary: SSE plugin for Starlette
 Author-Email: sysid <sysid@gmx.de>
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -15,16 +15,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Project-URL: Source, https://github.com/sysid/sse-starlette
 Requires-Python: >=3.8
 Requires-Dist: starlette
 Requires-Dist: uvicorn
-Requires-Dist: fastapi
 Requires-Dist: anyio
+Requires-Dist: fastapi; extra == "examples"
+Provides-Extra: examples
 Description-Content-Type: text/markdown
 
 # Server Sent Events for [Starlette](https://github.com/encode/starlette) and [FastAPI](https://fastapi.tiangolo.com/)
 
 [![PyPI Version][pypi-image]][pypi-url]
 [![Build Status][build-image]][build-url]
 [![Code Coverage][coverage-image]][coverage-url]
```

