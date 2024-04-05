# Comparing `tmp/httpx_ws-0.5.2.tar.gz` & `tmp/httpx_ws-0.6.0.tar.gz`

## Comparing `httpx_ws-0.5.2.tar` & `httpx_ws-0.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/.all-contributorsrc
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/.editorconfig
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/mkdocs.yml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/.github/FUNDING.yml
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/.github/workflows/build.yml
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/.github/workflows/docs.yml
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/.vscode/settings.json
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/docs/index.md
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/docs/reference/httpx_ws.md
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/docs/usage/asgi.md
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/docs/usage/quickstart.md
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/docs/usage/subprotocols.md
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/httpx_ws/__init__.py
--rw-r--r--   0        0        0    45843 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/httpx_ws/_api.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/httpx_ws/_exceptions.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/httpx_ws/_ping.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/httpx_ws/py.typed
--rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/httpx_ws/transport.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/tests/__init__.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/tests/conftest.py
--rw-r--r--   0        0        0    32573 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/tests/test_api.py
--rw-r--r--   0        0        0     8064 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/tests/test_transport.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/LICENSE
--rw-r--r--   0        0        0     6472 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/README.md
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     7464 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/PKG-INFO
--rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 httpx_ws-0.5.2/setup.py
+-rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/.all-contributorsrc
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/.editorconfig
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/mkdocs.yml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/.vscode/settings.json
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/docs/index.md
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/docs/reference/httpx_ws.md
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/docs/usage/asgi.md
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/docs/usage/quickstart.md
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/docs/usage/subprotocols.md
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/httpx_ws/__init__.py
+-rw-r--r--   0        0        0    46325 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/httpx_ws/_api.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/httpx_ws/_exceptions.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/httpx_ws/_ping.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/httpx_ws/py.typed
+-rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/httpx_ws/transport.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/tests/conftest.py
+-rw-r--r--   0        0        0    32873 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/tests/test_api.py
+-rw-r--r--   0        0        0     8064 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/tests/test_transport.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/LICENSE
+-rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/README.md
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     7870 2020-02-02 00:00:00.000000 httpx_ws-0.6.0/setup.py
```

### Comparing `httpx_ws-0.5.2/.all-contributorsrc` & `httpx_ws-0.6.0/.all-contributorsrc`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9962121212121212%*

 * *Differences: {"'contributors'": "{insert: [(10, OrderedDict([('login', 'WSH032'), ('name', 'Sean Wang'), "*

 * *                   "('avatar_url', 'https://avatars.githubusercontent.com/u/126865849?v=4'), "*

 * *                   "('profile', 'https://github.com/WSH032'), ('contributions', ['code'])]))]}"}*

```diff
@@ -93,14 +93,23 @@
             "avatar_url": "https://avatars.githubusercontent.com/u/35119617?v=4",
             "contributions": [
                 "bug"
             ],
             "login": "dmontagu",
             "name": "David Montague",
             "profile": "https://github.com/dmontagu"
+        },
+        {
+            "avatar_url": "https://avatars.githubusercontent.com/u/126865849?v=4",
+            "contributions": [
+                "code"
+            ],
+            "login": "WSH032",
+            "name": "Sean Wang",
+            "profile": "https://github.com/WSH032"
         }
     ],
     "contributorsPerLine": 7,
     "files": [
         "README.md"
     ],
     "imageSize": 100,
```

### Comparing `httpx_ws-0.5.2/mkdocs.yml` & `httpx_ws-0.6.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.5.2/.github/ISSUE_TEMPLATE/bug_report.md` & `httpx_ws-0.6.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.5.2/.github/workflows/build.yml` & `httpx_ws-0.6.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.5.2/.github/workflows/docs.yml` & `httpx_ws-0.6.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.5.2/.vscode/settings.json` & `httpx_ws-0.6.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.5.2/docs/usage/asgi.md` & `httpx_ws-0.6.0/docs/usage/asgi.md`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.5.2/docs/usage/quickstart.md` & `httpx_ws-0.6.0/docs/usage/quickstart.md`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.5.2/docs/usage/subprotocols.md` & `httpx_ws-0.6.0/docs/usage/subprotocols.md`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.5.2/httpx_ws/__init__.py` & `httpx_ws-0.6.0/httpx_ws/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.5.2"
+__version__ = "0.6.0"
 
 from ._api import (
     AsyncWebSocketSession,
     JSONMode,
     WebSocketSession,
     aconnect_ws,
     connect_ws,
```

### Comparing `httpx_ws-0.5.2/httpx_ws/_api.py` & `httpx_ws-0.6.0/httpx_ws/_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,35 +41,42 @@
 class WebSocketSession:
     """
     Sync context manager representing an opened WebSocket session.
 
     Attributes:
         subprotocol (typing.Optional[str]):
             Optional protocol that has been accepted by the server.
+        response (typing.Optional[httpx.Response]):
+            The webSocket handshake response.
     """
 
     subprotocol: typing.Optional[str]
+    response: typing.Optional[httpx.Response]
 
     def __init__(
         self,
         stream: NetworkStream,
         *,
         max_message_size_bytes: int = DEFAULT_MAX_MESSAGE_SIZE_BYTES,
         queue_size: int = DEFAULT_QUEUE_SIZE,
         keepalive_ping_interval_seconds: typing.Optional[
             float
         ] = DEFAULT_KEEPALIVE_PING_INTERVAL_SECONDS,
         keepalive_ping_timeout_seconds: typing.Optional[
             float
         ] = DEFAULT_KEEPALIVE_PING_TIMEOUT_SECONDS,
-        subprotocol: typing.Optional[str] = None,
+        response: typing.Optional[httpx.Response] = None,
     ) -> None:
         self.stream = stream
         self.connection = wsproto.connection.Connection(wsproto.ConnectionType.CLIENT)
-        self.subprotocol = subprotocol
+        self.response = response
+        if self.response is not None:
+            self.subprotocol = self.response.headers.get("sec-websocket-protocol")
+        else:
+            self.subprotocol = None
 
         self._events: queue.Queue[
             typing.Union[wsproto.events.Event, HTTPXWSException]
         ] = queue.Queue(queue_size)
 
         self._ping_manager = PingManager()
         self._should_close = threading.Event()
@@ -529,35 +536,42 @@
 class AsyncWebSocketSession:
     """
     Async context manager representing an opened WebSocket session.
 
     Attributes:
         subprotocol (typing.Optional[str]):
             Optional protocol that has been accepted by the server.
+        response (typing.Optional[httpx.Response]):
+            The webSocket handshake response.
     """
 
     subprotocol: typing.Optional[str]
+    response: typing.Optional[httpx.Response]
 
     def __init__(
         self,
         stream: AsyncNetworkStream,
         *,
         max_message_size_bytes: int = DEFAULT_MAX_MESSAGE_SIZE_BYTES,
         queue_size: int = DEFAULT_QUEUE_SIZE,
         keepalive_ping_interval_seconds: typing.Optional[
             float
         ] = DEFAULT_KEEPALIVE_PING_INTERVAL_SECONDS,
         keepalive_ping_timeout_seconds: typing.Optional[
             float
         ] = DEFAULT_KEEPALIVE_PING_TIMEOUT_SECONDS,
-        subprotocol: typing.Optional[str] = None,
+        response: typing.Optional[httpx.Response] = None,
     ) -> None:
         self.stream = stream
         self.connection = wsproto.connection.Connection(wsproto.ConnectionType.CLIENT)
-        self.subprotocol = subprotocol
+        self.response = response
+        if self.response is not None:
+            self.subprotocol = self.response.headers.get("sec-websocket-protocol")
+        else:
+            self.subprotocol = None
 
         self._send_event, self._receive_event = anyio.create_memory_object_stream[
             typing.Union[wsproto.events.Event, HTTPXWSException]
         ]()
 
         self._ping_manager = AsyncPingManager()
         self._should_close = anyio.Event()
@@ -1031,23 +1045,21 @@
     headers = kwargs.pop("headers", {})
     headers.update(_get_headers(subprotocols))
 
     with client.stream("GET", url, headers=headers, **kwargs) as response:
         if response.status_code != 101:
             raise WebSocketUpgradeError(response)
 
-        subprotocol = response.headers.get("sec-websocket-protocol")
-
         with WebSocketSession(
             response.extensions["network_stream"],
             max_message_size_bytes=max_message_size_bytes,
             queue_size=queue_size,
             keepalive_ping_interval_seconds=keepalive_ping_interval_seconds,
             keepalive_ping_timeout_seconds=keepalive_ping_timeout_seconds,
-            subprotocol=subprotocol,
+            response=response,
         ) as session:
             yield session
 
 
 @contextlib.contextmanager
 def connect_ws(
     url: str,
@@ -1166,23 +1178,21 @@
     headers = kwargs.pop("headers", {})
     headers.update(_get_headers(subprotocols))
 
     async with client.stream("GET", url, headers=headers, **kwargs) as response:
         if response.status_code != 101:
             raise WebSocketUpgradeError(response)
 
-        subprotocol = response.headers.get("sec-websocket-protocol")
-
         async with AsyncWebSocketSession(
             response.extensions["network_stream"],
             max_message_size_bytes=max_message_size_bytes,
             queue_size=queue_size,
             keepalive_ping_interval_seconds=keepalive_ping_interval_seconds,
             keepalive_ping_timeout_seconds=keepalive_ping_timeout_seconds,
-            subprotocol=subprotocol,
+            response=response,
         ) as session:
             yield session
 
 
 @contextlib.asynccontextmanager
 async def aconnect_ws(
     url: str,
```

### Comparing `httpx_ws-0.5.2/httpx_ws/_exceptions.py` & `httpx_ws-0.6.0/httpx_ws/_exceptions.py`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.5.2/httpx_ws/_ping.py` & `httpx_ws-0.6.0/httpx_ws/_ping.py`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.5.2/httpx_ws/transport.py` & `httpx_ws-0.6.0/httpx_ws/transport.py`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.5.2/tests/conftest.py` & `httpx_ws-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.5.2/tests/test_api.py` & `httpx_ws-0.6.0/tests/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -842,15 +842,15 @@
     mock_aconnect_ws.assert_called_once()
     httpx_client = mock_aconnect_ws.call_args[1]["client"]
     assert isinstance(httpx_client, httpx.AsyncClient)
     assert httpx_client.is_closed
 
 
 @pytest.mark.anyio
-async def test_subprotocol():
+async def test_subprotocol_and_response():
     def handler(request):
         assert (
             request.headers["sec-websocket-protocol"]
             == "custom_protocol, unsupported_protocol"
         )
 
         return httpx.Response(
@@ -875,18 +875,22 @@
         base_url="http://localhost:8000", transport=httpx.MockTransport(handler)
     ) as client:
         with connect_ws(
             "http://socket/ws",
             client,
             subprotocols=["custom_protocol", "unsupported_protocol"],
         ) as ws:
+            assert isinstance(ws.response, httpx.Response)
             assert ws.subprotocol == "custom_protocol"
+            assert ws.response.headers["sec-websocket-protocol"] == ws.subprotocol
 
     async with httpx.AsyncClient(
         base_url="http://localhost:8000", transport=httpx.MockTransport(async_handler)
     ) as client:
         async with aconnect_ws(
             "http://socket/ws",
             client,
             subprotocols=["custom_protocol", "unsupported_protocol"],
         ) as aws:
+            assert isinstance(aws.response, httpx.Response)
             assert aws.subprotocol == "custom_protocol"
+            assert aws.response.headers["sec-websocket-protocol"] == aws.subprotocol
```

### Comparing `httpx_ws-0.5.2/tests/test_transport.py` & `httpx_ws-0.6.0/tests/test_transport.py`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.5.2/.gitignore` & `httpx_ws-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.5.2/LICENSE` & `httpx_ws-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.5.2/README.md` & `httpx_ws-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
       <td align="center" valign="top" width="14.28%"><a href="http://maparent.ca/"><img src="https://avatars.githubusercontent.com/u/202691?v=4?s=100" width="100px;" alt="Marc-Antoine Parent"/><br /><sub><b>Marc-Antoine Parent</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3Amaparent" title="Bug reports">🐛</a> <a href="https://github.com/frankie567/httpx-ws/commits?author=maparent" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.fastapiexpert.com/"><img src="https://avatars.githubusercontent.com/u/7353520?v=4?s=100" width="100px;" alt="Marcelo Trylesinski"/><br /><sub><b>Marcelo Trylesinski</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3AKludex" title="Bug reports">🐛</a> <a href="#research-Kludex" title="Research">🔬</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://lit.link/MtkN1"><img src="https://avatars.githubusercontent.com/u/51289448?v=4?s=100" width="100px;" alt="MtkN1"/><br /><sub><b>MtkN1</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3AMtkN1" title="Bug reports">🐛</a> <a href="#research-MtkN1" title="Research">🔬</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://www.tomchristie.com/"><img src="https://avatars.githubusercontent.com/u/647359?v=4?s=100" width="100px;" alt="Tom Christie"/><br /><sub><b>Tom Christie</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3Atomchristie" title="Bug reports">🐛</a> <a href="#research-tomchristie" title="Research">🔬</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/dmontagu"><img src="https://avatars.githubusercontent.com/u/35119617?v=4?s=100" width="100px;" alt="David Montague"/><br /><sub><b>David Montague</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3Admontagu" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/WSH032"><img src="https://avatars.githubusercontent.com/u/126865849?v=4?s=100" width="100px;" alt="Sean Wang"/><br /><sub><b>Sean Wang</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/commits?author=WSH032" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -15,24 +15,26 @@
 httpx-ws ``` ## Features * [X] Sync and async client * [X] Helper methods to
 send text, binary and JSON data * [X] Helper methods to receive text, binary
 and JSON data * [X] Automatic ping/pong answers * [X] HTTPX transport to test
 WebSockets defined in ASGI apps * [X] Automatic keepalive ping * [X] `asyncio`
 and [Trio](https://trio.readthedocs.io/) support through [AnyIO](https://
 anyio.readthedocs.io/) ## Contributors â¨ Thanks goes to these wonderful
 people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
-_[_F_r_a_n_Ã_§_o_i_s   _[_K_o_u_s_i_k     _[_D_a_v_i_d   _[_y_s_m_u_]    _[_S_a_m     _[_M_a_r_c_-_A_n_t_o_i_n_e   _[_M_a_r_c_e_l_o
-  _V_o_r_o_n_]      _M_i_t_r_a_]    _B_r_o_c_h_a_r_t_]  _yy_ss_mm_uu   _F_o_r_e_m_a_n_]      _P_a_r_e_n_t_]    _T_r_y_l_e_s_i_n_s_k_i_]
-_FF_rr_aa_nn_?Ã_?§_oo_ii_ss  _KK_oo_uu_ss_ii_kk_ _MM_ii_tt_rr_aa   _DD_aa_vv_ii_dd    _ð___  _SS_aa_mm_ _FF_oo_rr_ee_mm_aa_nn _MM_aa_rr_cc_--_AA_nn_tt_oo_ii_nn_ee    _MM_aa_rr_cc_ee_ll_oo
-  _VV_oo_rr_oo_nn        _ð___»     _BB_rr_oo_cc_hh_aa_rr_tt            _ð___        _PP_aa_rr_ee_nn_tt     _TT_rr_yy_ll_ee_ss_ii_nn_ss_kk_ii
-_ð___§ _ð___»                 _ð___¦                         _ð___ _ð___»    _ð___ _ð___¬
- _[_M_t_k_N_1_]       _[_T_o_m      _[_D_a_v_i_d
-  _MM_tt_kk_NN_11     _C_h_r_i_s_t_i_e_]   _M_o_n_t_a_g_u_e_]
-_ð___ _ð___¬  _TT_oo_mm_ _CC_hh_rr_ii_ss_tt_ii_ee   _DD_aa_vv_ii_dd
-            _ð___ _ð___¬   _MM_oo_nn_tt_aa_gg_uu_ee
-                          _ð___
+_[_F_r_a_n_Ã_§_o_i_s  _[_K_o_u_s_i_k   _[_D_a_v_i_d      _[_y_s_m_u_]      _[_S_a_m      _[_M_a_r_c_-     _[_M_a_r_c_e_l_o
+  _V_o_r_o_n_]    _M_i_t_r_a_]   _B_r_o_c_h_a_r_t_]     _yy_ss_mm_uu     _F_o_r_e_m_a_n_]    _A_n_t_o_i_n_e  _T_r_y_l_e_s_i_n_s_k_i_]
+_FF_rr_aa_nn_?Ã_?§_oo_ii_ss   _KK_oo_uu_ss_ii_kk     _DD_aa_vv_ii_dd       _ð___    _SS_aa_mm_ _FF_oo_rr_ee_mm_aa_nn  _P_a_r_e_n_t_]    _MM_aa_rr_cc_ee_ll_oo
+  _VV_oo_rr_oo_nn      _MM_ii_tt_rr_aa   _BB_rr_oo_cc_hh_aa_rr_tt                 _ð___       _MM_aa_rr_cc_--   _TT_rr_yy_ll_ee_ss_ii_nn_ss_kk_ii
+_ð___§ _ð___»    _ð___»      _ð___¦                             _AA_nn_tt_oo_ii_nn_ee   _ð___ _ð___¬
+                                                        _PP_aa_rr_ee_nn_tt
+                                                       _ð___ _ð___»
+ _[_M_t_k_N_1_]     _[_T_o_m     _[_D_a_v_i_d   _[_S_e_a_n_ _W_a_n_g_]
+  _MM_tt_kk_NN_11    _C_h_r_i_s_t_i_e_] _M_o_n_t_a_g_u_e_]  _SS_ee_aa_nn_ _WW_aa_nn_gg
+_ð___ _ð___¬     _TT_oo_mm      _DD_aa_vv_ii_dd      _ð___»
+           _CC_hh_rr_ii_ss_tt_ii_ee  _MM_oo_nn_tt_aa_gg_uu_ee
+           _ð___ _ð___¬   _ð___
 This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome! ## Development ### Setup environment We use [Hatch](https://
 hatch.pypa.io/latest/install/) to manage the development environment and
 production build. Ensure it's installed on your system. ### Run unit tests You
 can run all the tests with: ```bash hatch run test ``` ### Format the code
 Execute the following command to apply linting and check typing: ```bash hatch
```

### Comparing `httpx_ws-0.5.2/pyproject.toml` & `httpx_ws-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.5.2/PKG-INFO` & `httpx_ws-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: httpx-ws
-Version: 0.5.2
+Version: 0.6.0
 Summary: WebSockets support for HTTPX
 Project-URL: Documentation, https://frankie567.github.io/httpx-ws/
 Project-URL: Source, https://github.com/frankie567/httpx-ws
 Author-email: François Voron <fvoron@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
@@ -87,14 +87,15 @@
       <td align="center" valign="top" width="14.28%"><a href="http://maparent.ca/"><img src="https://avatars.githubusercontent.com/u/202691?v=4?s=100" width="100px;" alt="Marc-Antoine Parent"/><br /><sub><b>Marc-Antoine Parent</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3Amaparent" title="Bug reports">🐛</a> <a href="https://github.com/frankie567/httpx-ws/commits?author=maparent" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.fastapiexpert.com/"><img src="https://avatars.githubusercontent.com/u/7353520?v=4?s=100" width="100px;" alt="Marcelo Trylesinski"/><br /><sub><b>Marcelo Trylesinski</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3AKludex" title="Bug reports">🐛</a> <a href="#research-Kludex" title="Research">🔬</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://lit.link/MtkN1"><img src="https://avatars.githubusercontent.com/u/51289448?v=4?s=100" width="100px;" alt="MtkN1"/><br /><sub><b>MtkN1</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3AMtkN1" title="Bug reports">🐛</a> <a href="#research-MtkN1" title="Research">🔬</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://www.tomchristie.com/"><img src="https://avatars.githubusercontent.com/u/647359?v=4?s=100" width="100px;" alt="Tom Christie"/><br /><sub><b>Tom Christie</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3Atomchristie" title="Bug reports">🐛</a> <a href="#research-tomchristie" title="Research">🔬</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/dmontagu"><img src="https://avatars.githubusercontent.com/u/35119617?v=4?s=100" width="100px;" alt="David Montague"/><br /><sub><b>David Montague</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3Admontagu" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/WSH032"><img src="https://avatars.githubusercontent.com/u/126865849?v=4?s=100" width="100px;" alt="Sean Wang"/><br /><sub><b>Sean Wang</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/commits?author=WSH032" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: httpx-ws Version: 0.5.2 Summary: WebSockets support
+Metadata-Version: 2.3 Name: httpx-ws Version: 0.6.0 Summary: WebSockets support
 for HTTPX Project-URL: Documentation, https://frankie567.github.io/httpx-ws/
 Project-URL: Source, https://github.com/frankie567/httpx-ws Author-email:
 FranÃ§ois Voron
 gmail.com> License-File: LICENSE Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
@@ -28,24 +28,26 @@
 httpx-ws ``` ## Features * [X] Sync and async client * [X] Helper methods to
 send text, binary and JSON data * [X] Helper methods to receive text, binary
 and JSON data * [X] Automatic ping/pong answers * [X] HTTPX transport to test
 WebSockets defined in ASGI apps * [X] Automatic keepalive ping * [X] `asyncio`
 and [Trio](https://trio.readthedocs.io/) support through [AnyIO](https://
 anyio.readthedocs.io/) ## Contributors â¨ Thanks goes to these wonderful
 people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
-_[_F_r_a_n_Ã_§_o_i_s   _[_K_o_u_s_i_k     _[_D_a_v_i_d   _[_y_s_m_u_]    _[_S_a_m     _[_M_a_r_c_-_A_n_t_o_i_n_e   _[_M_a_r_c_e_l_o
-  _V_o_r_o_n_]      _M_i_t_r_a_]    _B_r_o_c_h_a_r_t_]  _yy_ss_mm_uu   _F_o_r_e_m_a_n_]      _P_a_r_e_n_t_]    _T_r_y_l_e_s_i_n_s_k_i_]
-_FF_rr_aa_nn_?Ã_?§_oo_ii_ss  _KK_oo_uu_ss_ii_kk_ _MM_ii_tt_rr_aa   _DD_aa_vv_ii_dd    _ð___  _SS_aa_mm_ _FF_oo_rr_ee_mm_aa_nn _MM_aa_rr_cc_--_AA_nn_tt_oo_ii_nn_ee    _MM_aa_rr_cc_ee_ll_oo
-  _VV_oo_rr_oo_nn        _ð___»     _BB_rr_oo_cc_hh_aa_rr_tt            _ð___        _PP_aa_rr_ee_nn_tt     _TT_rr_yy_ll_ee_ss_ii_nn_ss_kk_ii
-_ð___§ _ð___»                 _ð___¦                         _ð___ _ð___»    _ð___ _ð___¬
- _[_M_t_k_N_1_]       _[_T_o_m      _[_D_a_v_i_d
-  _MM_tt_kk_NN_11     _C_h_r_i_s_t_i_e_]   _M_o_n_t_a_g_u_e_]
-_ð___ _ð___¬  _TT_oo_mm_ _CC_hh_rr_ii_ss_tt_ii_ee   _DD_aa_vv_ii_dd
-            _ð___ _ð___¬   _MM_oo_nn_tt_aa_gg_uu_ee
-                          _ð___
+_[_F_r_a_n_Ã_§_o_i_s  _[_K_o_u_s_i_k   _[_D_a_v_i_d      _[_y_s_m_u_]      _[_S_a_m      _[_M_a_r_c_-     _[_M_a_r_c_e_l_o
+  _V_o_r_o_n_]    _M_i_t_r_a_]   _B_r_o_c_h_a_r_t_]     _yy_ss_mm_uu     _F_o_r_e_m_a_n_]    _A_n_t_o_i_n_e  _T_r_y_l_e_s_i_n_s_k_i_]
+_FF_rr_aa_nn_?Ã_?§_oo_ii_ss   _KK_oo_uu_ss_ii_kk     _DD_aa_vv_ii_dd       _ð___    _SS_aa_mm_ _FF_oo_rr_ee_mm_aa_nn  _P_a_r_e_n_t_]    _MM_aa_rr_cc_ee_ll_oo
+  _VV_oo_rr_oo_nn      _MM_ii_tt_rr_aa   _BB_rr_oo_cc_hh_aa_rr_tt                 _ð___       _MM_aa_rr_cc_--   _TT_rr_yy_ll_ee_ss_ii_nn_ss_kk_ii
+_ð___§ _ð___»    _ð___»      _ð___¦                             _AA_nn_tt_oo_ii_nn_ee   _ð___ _ð___¬
+                                                        _PP_aa_rr_ee_nn_tt
+                                                       _ð___ _ð___»
+ _[_M_t_k_N_1_]     _[_T_o_m     _[_D_a_v_i_d   _[_S_e_a_n_ _W_a_n_g_]
+  _MM_tt_kk_NN_11    _C_h_r_i_s_t_i_e_] _M_o_n_t_a_g_u_e_]  _SS_ee_aa_nn_ _WW_aa_nn_gg
+_ð___ _ð___¬     _TT_oo_mm      _DD_aa_vv_ii_dd      _ð___»
+           _CC_hh_rr_ii_ss_tt_ii_ee  _MM_oo_nn_tt_aa_gg_uu_ee
+           _ð___ _ð___¬   _ð___
 This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome! ## Development ### Setup environment We use [Hatch](https://
 hatch.pypa.io/latest/install/) to manage the development environment and
 production build. Ensure it's installed on your system. ### Run unit tests You
 can run all the tests with: ```bash hatch run test ``` ### Format the code
 Execute the following command to apply linting and check typing: ```bash hatch
```

### Comparing `httpx_ws-0.5.2/setup.py` & `httpx_ws-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 setup(
     name='httpx-ws',
-    version='0.5.2',
+    version='0.6.0',
     description='WebSockets support for HTTPX',
-    long_description='# HTTPX WS\n\n<p align="center">\n    <em>WebSockets support for HTTPX</em>\n</p>\n\n[![build](https://github.com/frankie567/httpx-ws/workflows/Build/badge.svg)](https://github.com/frankie567/httpx-ws/actions)\n[![codecov](https://codecov.io/gh/frankie567/httpx-ws/branch/main/graph/badge.svg?token=fL49kIvrj6)](https://codecov.io/gh/frankie567/httpx-ws)\n[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)\n[![PyPI version](https://badge.fury.io/py/httpx-ws.svg)](https://badge.fury.io/py/httpx-ws)\n[![Downloads](https://pepy.tech/badge/httpx-ws)](https://pepy.tech/project/httpx-ws)\n\n<p align="center">\n<a href="https://polar.sh/frankie567">\n<picture>\n  <source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/subscribe.svg?org=frankie567&darkmode=1">\n  <img alt="Subscribe" src="https://polar.sh/embed/subscribe.svg?org=frankie567">\n</picture>\n</a>\n</p>\n\n---\n\n**Documentation**: <a href="https://frankie567.github.io/httpx-ws/" target="_blank">https://frankie567.github.io/httpx-ws/</a>\n\n**Source Code**: <a href="https://github.com/frankie567/httpx-ws" target="_blank">https://github.com/frankie567/httpx-ws</a>\n\n---\n\n## Installation\n\n```bash\npip install httpx-ws\n```\n\n## Features\n\n* [X] Sync and async client\n* [X] Helper methods to send text, binary and JSON data\n* [X] Helper methods to receive text, binary and JSON data\n* [X] Automatic ping/pong answers\n* [X] HTTPX transport to test WebSockets defined in ASGI apps\n* [X] Automatic keepalive ping\n* [X] `asyncio` and [Trio](https://trio.readthedocs.io/) support through [AnyIO](https://anyio.readthedocs.io/)\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tbody>\n    <tr>\n      <td align="center" valign="top" width="14.28%"><a href="http://francoisvoron.com"><img src="https://avatars.githubusercontent.com/u/1144727?v=4?s=100" width="100px;" alt="François Voron"/><br /><sub><b>François Voron</b></sub></a><br /><a href="#maintenance-frankie567" title="Maintenance">🚧</a> <a href="https://github.com/frankie567/httpx-ws/commits?author=frankie567" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="http://kousikmitra.github.io"><img src="https://avatars.githubusercontent.com/u/15109533?v=4?s=100" width="100px;" alt="Kousik Mitra"/><br /><sub><b>Kousik Mitra</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/commits?author=kousikmitra" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/davidbrochart"><img src="https://avatars.githubusercontent.com/u/4711805?v=4?s=100" width="100px;" alt="David Brochart"/><br /><sub><b>David Brochart</b></sub></a><br /><a href="#platform-davidbrochart" title="Packaging/porting to new platform">📦</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ysmu"><img src="https://avatars.githubusercontent.com/u/17018576?v=4?s=100" width="100px;" alt="ysmu"/><br /><sub><b>ysmu</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3Aysmu" title="Bug reports">🐛</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://samforeman.me"><img src="https://avatars.githubusercontent.com/u/5234251?v=4?s=100" width="100px;" alt="Sam Foreman"/><br /><sub><b>Sam Foreman</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3Asaforem2" title="Bug reports">🐛</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="http://maparent.ca/"><img src="https://avatars.githubusercontent.com/u/202691?v=4?s=100" width="100px;" alt="Marc-Antoine Parent"/><br /><sub><b>Marc-Antoine Parent</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3Amaparent" title="Bug reports">🐛</a> <a href="https://github.com/frankie567/httpx-ws/commits?author=maparent" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://www.fastapiexpert.com/"><img src="https://avatars.githubusercontent.com/u/7353520?v=4?s=100" width="100px;" alt="Marcelo Trylesinski"/><br /><sub><b>Marcelo Trylesinski</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3AKludex" title="Bug reports">🐛</a> <a href="#research-Kludex" title="Research">🔬</a></td>\n    </tr>\n    <tr>\n      <td align="center" valign="top" width="14.28%"><a href="https://lit.link/MtkN1"><img src="https://avatars.githubusercontent.com/u/51289448?v=4?s=100" width="100px;" alt="MtkN1"/><br /><sub><b>MtkN1</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3AMtkN1" title="Bug reports">🐛</a> <a href="#research-MtkN1" title="Research">🔬</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="http://www.tomchristie.com/"><img src="https://avatars.githubusercontent.com/u/647359?v=4?s=100" width="100px;" alt="Tom Christie"/><br /><sub><b>Tom Christie</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3Atomchristie" title="Bug reports">🐛</a> <a href="#research-tomchristie" title="Research">🔬</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/dmontagu"><img src="https://avatars.githubusercontent.com/u/35119617?v=4?s=100" width="100px;" alt="David Montague"/><br /><sub><b>David Montague</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3Admontagu" title="Bug reports">🐛</a></td>\n    </tr>\n  </tbody>\n</table>\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Development\n\n### Setup environment\n\nWe use [Hatch](https://hatch.pypa.io/latest/install/) to manage the development environment and production build. Ensure it\'s installed on your system.\n\n### Run unit tests\n\nYou can run all the tests with:\n\n```bash\nhatch run test\n```\n\n### Format the code\n\nExecute the following command to apply linting and check typing:\n\n```bash\nhatch run lint\n```\n\n## License\n\nThis project is licensed under the terms of the MIT license.\n',
+    long_description='# HTTPX WS\n\n<p align="center">\n    <em>WebSockets support for HTTPX</em>\n</p>\n\n[![build](https://github.com/frankie567/httpx-ws/workflows/Build/badge.svg)](https://github.com/frankie567/httpx-ws/actions)\n[![codecov](https://codecov.io/gh/frankie567/httpx-ws/branch/main/graph/badge.svg?token=fL49kIvrj6)](https://codecov.io/gh/frankie567/httpx-ws)\n[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)\n[![PyPI version](https://badge.fury.io/py/httpx-ws.svg)](https://badge.fury.io/py/httpx-ws)\n[![Downloads](https://pepy.tech/badge/httpx-ws)](https://pepy.tech/project/httpx-ws)\n\n<p align="center">\n<a href="https://polar.sh/frankie567">\n<picture>\n  <source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/subscribe.svg?org=frankie567&darkmode=1">\n  <img alt="Subscribe" src="https://polar.sh/embed/subscribe.svg?org=frankie567">\n</picture>\n</a>\n</p>\n\n---\n\n**Documentation**: <a href="https://frankie567.github.io/httpx-ws/" target="_blank">https://frankie567.github.io/httpx-ws/</a>\n\n**Source Code**: <a href="https://github.com/frankie567/httpx-ws" target="_blank">https://github.com/frankie567/httpx-ws</a>\n\n---\n\n## Installation\n\n```bash\npip install httpx-ws\n```\n\n## Features\n\n* [X] Sync and async client\n* [X] Helper methods to send text, binary and JSON data\n* [X] Helper methods to receive text, binary and JSON data\n* [X] Automatic ping/pong answers\n* [X] HTTPX transport to test WebSockets defined in ASGI apps\n* [X] Automatic keepalive ping\n* [X] `asyncio` and [Trio](https://trio.readthedocs.io/) support through [AnyIO](https://anyio.readthedocs.io/)\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tbody>\n    <tr>\n      <td align="center" valign="top" width="14.28%"><a href="http://francoisvoron.com"><img src="https://avatars.githubusercontent.com/u/1144727?v=4?s=100" width="100px;" alt="François Voron"/><br /><sub><b>François Voron</b></sub></a><br /><a href="#maintenance-frankie567" title="Maintenance">🚧</a> <a href="https://github.com/frankie567/httpx-ws/commits?author=frankie567" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="http://kousikmitra.github.io"><img src="https://avatars.githubusercontent.com/u/15109533?v=4?s=100" width="100px;" alt="Kousik Mitra"/><br /><sub><b>Kousik Mitra</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/commits?author=kousikmitra" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/davidbrochart"><img src="https://avatars.githubusercontent.com/u/4711805?v=4?s=100" width="100px;" alt="David Brochart"/><br /><sub><b>David Brochart</b></sub></a><br /><a href="#platform-davidbrochart" title="Packaging/porting to new platform">📦</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ysmu"><img src="https://avatars.githubusercontent.com/u/17018576?v=4?s=100" width="100px;" alt="ysmu"/><br /><sub><b>ysmu</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3Aysmu" title="Bug reports">🐛</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://samforeman.me"><img src="https://avatars.githubusercontent.com/u/5234251?v=4?s=100" width="100px;" alt="Sam Foreman"/><br /><sub><b>Sam Foreman</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3Asaforem2" title="Bug reports">🐛</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="http://maparent.ca/"><img src="https://avatars.githubusercontent.com/u/202691?v=4?s=100" width="100px;" alt="Marc-Antoine Parent"/><br /><sub><b>Marc-Antoine Parent</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3Amaparent" title="Bug reports">🐛</a> <a href="https://github.com/frankie567/httpx-ws/commits?author=maparent" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://www.fastapiexpert.com/"><img src="https://avatars.githubusercontent.com/u/7353520?v=4?s=100" width="100px;" alt="Marcelo Trylesinski"/><br /><sub><b>Marcelo Trylesinski</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3AKludex" title="Bug reports">🐛</a> <a href="#research-Kludex" title="Research">🔬</a></td>\n    </tr>\n    <tr>\n      <td align="center" valign="top" width="14.28%"><a href="https://lit.link/MtkN1"><img src="https://avatars.githubusercontent.com/u/51289448?v=4?s=100" width="100px;" alt="MtkN1"/><br /><sub><b>MtkN1</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3AMtkN1" title="Bug reports">🐛</a> <a href="#research-MtkN1" title="Research">🔬</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="http://www.tomchristie.com/"><img src="https://avatars.githubusercontent.com/u/647359?v=4?s=100" width="100px;" alt="Tom Christie"/><br /><sub><b>Tom Christie</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3Atomchristie" title="Bug reports">🐛</a> <a href="#research-tomchristie" title="Research">🔬</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/dmontagu"><img src="https://avatars.githubusercontent.com/u/35119617?v=4?s=100" width="100px;" alt="David Montague"/><br /><sub><b>David Montague</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3Admontagu" title="Bug reports">🐛</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/WSH032"><img src="https://avatars.githubusercontent.com/u/126865849?v=4?s=100" width="100px;" alt="Sean Wang"/><br /><sub><b>Sean Wang</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/commits?author=WSH032" title="Code">💻</a></td>\n    </tr>\n  </tbody>\n</table>\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Development\n\n### Setup environment\n\nWe use [Hatch](https://hatch.pypa.io/latest/install/) to manage the development environment and production build. Ensure it\'s installed on your system.\n\n### Run unit tests\n\nYou can run all the tests with:\n\n```bash\nhatch run test\n```\n\n### Format the code\n\nExecute the following command to apply linting and check typing:\n\n```bash\nhatch run lint\n```\n\n## License\n\nThis project is licensed under the terms of the MIT license.\n',
     author_email='François Voron <fvoron@gmail.com>',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Framework :: AsyncIO',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3 :: Only',
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*- from setuptools import setup setup( name='httpx-ws',
-version='0.5.2', description='WebSockets support for HTTPX',
+version='0.6.0', description='WebSockets support for HTTPX',
 long_description='# HTTPX WS\n\n
                        \n WWeebbSSoocckkeettss ssuuppppoorrtt ffoorr HHTTTTPPXX\n
 \n\n[![build](https://github.com/frankie567/httpx-ws/workflows/Build/
 badge.svg)](https://github.com/frankie567/httpx-ws/actions)\n[![codecov](https:
 //codecov.io/gh/frankie567/httpx-ws/branch/main/graph/
 badge.svg?token=fL49kIvrj6)](https://codecov.io/gh/frankie567/httpx-ws)\n[![All
 Contributors](https://img.shields.io/badge/all_contributors-2-
@@ -18,24 +18,26 @@
 and async client\n* [X] Helper methods to send text, binary and JSON data\n*
 [X] Helper methods to receive text, binary and JSON data\n* [X] Automatic ping/
 pong answers\n* [X] HTTPX transport to test WebSockets defined in ASGI apps\n*
 [X] Automatic keepalive ping\n* [X] `asyncio` and [Trio](https://
 trio.readthedocs.io/) support through [AnyIO](https://anyio.readthedocs.io/
 )\n\n## Contributors â¨\n\nThanks goes to these wonderful people ([emoji key]
 (https://allcontributors.org/docs/en/emoji-key)):\n\n\n\n\n
-_[_F_r_a_n_Ã_§_o_i_s   _[_K_o_u_s_i_k     _[_D_a_v_i_d   _[_y_s_m_u_]    _[_S_a_m     _[_M_a_r_c_-_A_n_t_o_i_n_e   _[_M_a_r_c_e_l_o
-  _V_o_r_o_n_]      _M_i_t_r_a_]    _B_r_o_c_h_a_r_t_]  _yy_ss_mm_uu   _F_o_r_e_m_a_n_]      _P_a_r_e_n_t_]    _T_r_y_l_e_s_i_n_s_k_i_]
-_FF_rr_aa_nn_?Ã_?§_oo_ii_ss  _KK_oo_uu_ss_ii_kk_ _MM_ii_tt_rr_aa   _DD_aa_vv_ii_dd    _ð___  _SS_aa_mm_ _FF_oo_rr_ee_mm_aa_nn _MM_aa_rr_cc_--_AA_nn_tt_oo_ii_nn_ee    _MM_aa_rr_cc_ee_ll_oo
-  _VV_oo_rr_oo_nn        _ð___»     _BB_rr_oo_cc_hh_aa_rr_tt            _ð___        _PP_aa_rr_ee_nn_tt     _TT_rr_yy_ll_ee_ss_ii_nn_ss_kk_ii
-_ð___§ _ð___»                 _ð___¦                         _ð___ _ð___»    _ð___ _ð___¬
- _[_M_t_k_N_1_]       _[_T_o_m      _[_D_a_v_i_d
-  _MM_tt_kk_NN_11     _C_h_r_i_s_t_i_e_]   _M_o_n_t_a_g_u_e_]
-_ð___ _ð___¬  _TT_oo_mm_ _CC_hh_rr_ii_ss_tt_ii_ee   _DD_aa_vv_ii_dd
-            _ð___ _ð___¬   _MM_oo_nn_tt_aa_gg_uu_ee
-                          _ð___
+_[_F_r_a_n_Ã_§_o_i_s  _[_K_o_u_s_i_k   _[_D_a_v_i_d      _[_y_s_m_u_]      _[_S_a_m      _[_M_a_r_c_-     _[_M_a_r_c_e_l_o
+  _V_o_r_o_n_]    _M_i_t_r_a_]   _B_r_o_c_h_a_r_t_]     _yy_ss_mm_uu     _F_o_r_e_m_a_n_]    _A_n_t_o_i_n_e  _T_r_y_l_e_s_i_n_s_k_i_]
+_FF_rr_aa_nn_?Ã_?§_oo_ii_ss   _KK_oo_uu_ss_ii_kk     _DD_aa_vv_ii_dd       _ð___    _SS_aa_mm_ _FF_oo_rr_ee_mm_aa_nn  _P_a_r_e_n_t_]    _MM_aa_rr_cc_ee_ll_oo
+  _VV_oo_rr_oo_nn      _MM_ii_tt_rr_aa   _BB_rr_oo_cc_hh_aa_rr_tt                 _ð___       _MM_aa_rr_cc_--   _TT_rr_yy_ll_ee_ss_ii_nn_ss_kk_ii
+_ð___§ _ð___»    _ð___»      _ð___¦                             _AA_nn_tt_oo_ii_nn_ee   _ð___ _ð___¬
+                                                        _PP_aa_rr_ee_nn_tt
+                                                       _ð___ _ð___»
+ _[_M_t_k_N_1_]     _[_T_o_m     _[_D_a_v_i_d   _[_S_e_a_n_ _W_a_n_g_]
+  _MM_tt_kk_NN_11    _C_h_r_i_s_t_i_e_] _M_o_n_t_a_g_u_e_]  _SS_ee_aa_nn_ _WW_aa_nn_gg
+_ð___ _ð___¬     _TT_oo_mm      _DD_aa_vv_ii_dd      _ð___»
+           _CC_hh_rr_ii_ss_tt_ii_ee  _MM_oo_nn_tt_aa_gg_uu_ee
+           _ð___ _ð___¬   _ð___
 \n\n\n\n\n\n\nThis project follows the [all-contributors](https://github.com/
 all-contributors/all-contributors) specification. Contributions of any kind
 welcome!\n\n## Development\n\n### Setup environment\n\nWe use [Hatch](https://
 hatch.pypa.io/latest/install/) to manage the development environment and
 production build. Ensure it\'s installed on your system.\n\n### Run unit
 tests\n\nYou can run all the tests with:\n\n```bash\nhatch run test\n```\n\n###
 Format the code\n\nExecute the following command to apply linting and check
```

