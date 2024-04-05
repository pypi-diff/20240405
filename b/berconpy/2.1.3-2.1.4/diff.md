# Comparing `tmp/berconpy-2.1.3.tar.gz` & `tmp/berconpy-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "berconpy-2.1.3.tar", last modified: Tue Sep 12 06:24:32 2023, max compression
+gzip compressed data, was "berconpy-2.1.4.tar", last modified: Fri Apr  5 16:16:03 2024, max compression
```

## Comparing `berconpy-2.1.3.tar` & `berconpy-2.1.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 06:24:32.952221 berconpy-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-09-12 06:24:23.000000 berconpy-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-09-12 06:24:23.000000 berconpy-2.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2023-09-12 06:24:32.952221 berconpy-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2023-09-12 06:24:23.000000 berconpy-2.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2023-09-12 06:24:23.000000 berconpy-2.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-12 06:24:32.952221 berconpy-2.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 06:24:32.948221 berconpy-2.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 06:24:32.948221 berconpy-2.1.3/src/berconpy/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2023-09-12 06:24:23.000000 berconpy-2.1.3/src/berconpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 06:24:32.952221 berconpy-2.1.3/src/berconpy/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2023-09-12 06:24:23.000000 berconpy-2.1.3/src/berconpy/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-09-12 06:24:23.000000 berconpy-2.1.3/src/berconpy/asyncio/ban.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2023-09-12 06:24:23.000000 berconpy-2.1.3/src/berconpy/asyncio/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     7767 2023-09-12 06:24:23.000000 berconpy-2.1.3/src/berconpy/asyncio/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5601 2023-09-12 06:24:23.000000 berconpy-2.1.3/src/berconpy/asyncio/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    20178 2023-09-12 06:24:23.000000 berconpy-2.1.3/src/berconpy/asyncio/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2023-09-12 06:24:23.000000 berconpy-2.1.3/src/berconpy/asyncio/player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2023-09-12 06:24:23.000000 berconpy-2.1.3/src/berconpy/ban.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2023-09-12 06:24:23.000000 berconpy-2.1.3/src/berconpy/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    14406 2023-09-12 06:24:23.000000 berconpy-2.1.3/src/berconpy/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12157 2023-09-12 06:24:23.000000 berconpy-2.1.3/src/berconpy/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2023-09-12 06:24:23.000000 berconpy-2.1.3/src/berconpy/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 06:24:32.948221 berconpy-2.1.3/src/berconpy/ext/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 06:24:32.952221 berconpy-2.1.3/src/berconpy/ext/arma/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-09-12 06:24:23.000000 berconpy-2.1.3/src/berconpy/ext/arma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2023-09-12 06:24:23.000000 berconpy-2.1.3/src/berconpy/ext/arma/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2023-09-12 06:24:23.000000 berconpy-2.1.3/src/berconpy/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4531 2023-09-12 06:24:23.000000 berconpy-2.1.3/src/berconpy/player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 06:24:32.952221 berconpy-2.1.3/src/berconpy/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2023-09-12 06:24:23.000000 berconpy-2.1.3/src/berconpy/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2023-09-12 06:24:23.000000 berconpy-2.1.3/src/berconpy/protocol/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2023-09-12 06:24:23.000000 berconpy-2.1.3/src/berconpy/protocol/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     8197 2023-09-12 06:24:23.000000 berconpy-2.1.3/src/berconpy/protocol/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2023-09-12 06:24:23.000000 berconpy-2.1.3/src/berconpy/protocol/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2023-09-12 06:24:23.000000 berconpy-2.1.3/src/berconpy/protocol/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    15511 2023-09-12 06:24:23.000000 berconpy-2.1.3/src/berconpy/protocol/packet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7451 2023-09-12 06:24:23.000000 berconpy-2.1.3/src/berconpy/protocol/server.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-12 06:24:23.000000 berconpy-2.1.3/src/berconpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2023-09-12 06:24:23.000000 berconpy-2.1.3/src/berconpy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 06:24:32.948221 berconpy-2.1.3/src/berconpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2023-09-12 06:24:32.000000 berconpy-2.1.3/src/berconpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      985 2023-09-12 06:24:32.000000 berconpy-2.1.3/src/berconpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-12 06:24:32.000000 berconpy-2.1.3/src/berconpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-09-12 06:24:32.000000 berconpy-2.1.3/src/berconpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-09-12 06:24:32.000000 berconpy-2.1.3/src/berconpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:16:03.066998 berconpy-2.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-05 16:15:53.000000 berconpy-2.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 16:15:53.000000 berconpy-2.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-05 16:16:03.066998 berconpy-2.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-05 16:15:53.000000 berconpy-2.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-05 16:15:53.000000 berconpy-2.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:16:03.066998 berconpy-2.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:16:03.058998 berconpy-2.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:16:03.062998 berconpy-2.1.4/src/berconpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-05 16:15:53.000000 berconpy-2.1.4/src/berconpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:16:03.062998 berconpy-2.1.4/src/berconpy/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-05 16:15:53.000000 berconpy-2.1.4/src/berconpy/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-05 16:15:53.000000 berconpy-2.1.4/src/berconpy/asyncio/ban.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-04-05 16:15:53.000000 berconpy-2.1.4/src/berconpy/asyncio/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-04-05 16:15:53.000000 berconpy-2.1.4/src/berconpy/asyncio/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-04-05 16:15:53.000000 berconpy-2.1.4/src/berconpy/asyncio/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20562 2024-04-05 16:15:53.000000 berconpy-2.1.4/src/berconpy/asyncio/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-05 16:15:53.000000 berconpy-2.1.4/src/berconpy/asyncio/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-05 16:15:53.000000 berconpy-2.1.4/src/berconpy/ban.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-05 16:15:53.000000 berconpy-2.1.4/src/berconpy/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14406 2024-04-05 16:15:53.000000 berconpy-2.1.4/src/berconpy/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12157 2024-04-05 16:15:53.000000 berconpy-2.1.4/src/berconpy/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-05 16:15:53.000000 berconpy-2.1.4/src/berconpy/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:16:03.058998 berconpy-2.1.4/src/berconpy/ext/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:16:03.062998 berconpy-2.1.4/src/berconpy/ext/arma/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-05 16:15:53.000000 berconpy-2.1.4/src/berconpy/ext/arma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-05 16:15:53.000000 berconpy-2.1.4/src/berconpy/ext/arma/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-05 16:15:53.000000 berconpy-2.1.4/src/berconpy/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-04-05 16:15:53.000000 berconpy-2.1.4/src/berconpy/player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:16:03.066998 berconpy-2.1.4/src/berconpy/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-05 16:15:53.000000 berconpy-2.1.4/src/berconpy/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-05 16:15:53.000000 berconpy-2.1.4/src/berconpy/protocol/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-05 16:15:53.000000 berconpy-2.1.4/src/berconpy/protocol/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-04-05 16:15:53.000000 berconpy-2.1.4/src/berconpy/protocol/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-05 16:15:53.000000 berconpy-2.1.4/src/berconpy/protocol/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-05 16:15:53.000000 berconpy-2.1.4/src/berconpy/protocol/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15511 2024-04-05 16:15:53.000000 berconpy-2.1.4/src/berconpy/protocol/packet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7451 2024-04-05 16:15:53.000000 berconpy-2.1.4/src/berconpy/protocol/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:15:53.000000 berconpy-2.1.4/src/berconpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-05 16:15:53.000000 berconpy-2.1.4/src/berconpy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:16:03.066998 berconpy-2.1.4/src/berconpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-05 16:16:03.000000 berconpy-2.1.4/src/berconpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-05 16:16:03.000000 berconpy-2.1.4/src/berconpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:16:03.000000 berconpy-2.1.4/src/berconpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-05 16:16:03.000000 berconpy-2.1.4/src/berconpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 16:16:03.000000 berconpy-2.1.4/src/berconpy.egg-info/top_level.txt
```

### Comparing `berconpy-2.1.3/LICENSE` & `berconpy-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.3/PKG-INFO` & `berconpy-2.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: berconpy
-Version: 2.1.3
+Version: 2.1.4
 Summary: An async wrapper for the BattlEye RCON protocol
 Author: thegamecracks
 License: MIT
 Project-URL: Homepage, https://github.com/thegamecracks/berconpy
 Project-URL: Documentation, http://berconpy.readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/thegamecracks/berconpy/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `berconpy-2.1.3/README.md` & `berconpy-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.3/pyproject.toml` & `berconpy-2.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.3/src/berconpy/__init__.py` & `berconpy-2.1.4/src/berconpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     ServerAuthEvent,
     ServerCommandEvent,
     ServerEvent,
     ServerMessageEvent,
     ServerState,
 )
 
-__version__ = "2.1.3"
+__version__ = "2.1.4"
```

### Comparing `berconpy-2.1.3/src/berconpy/asyncio/ban.py` & `berconpy-2.1.4/src/berconpy/asyncio/ban.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.3/src/berconpy/asyncio/cache.py` & `berconpy-2.1.4/src/berconpy/asyncio/cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,14 +72,18 @@
             log.warning(
                 "did not receive admin_login event within 10 seconds; "
                 "client id will not be available"
             )
         else:
             self.admin_id = admin_id
 
+            if len(self._players) > 0:
+                # The user had already fetched players before us
+                return
+
             try:
                 await self.client.fetch_players()
             except RCONCommandError:
                 log.warning(
                     "failed to receive players from server; "
                     "player cache will not be available"
                 )
```

### Comparing `berconpy-2.1.3/src/berconpy/asyncio/client.py` & `berconpy-2.1.4/src/berconpy/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.3/src/berconpy/asyncio/dispatch.py` & `berconpy-2.1.4/src/berconpy/asyncio/dispatch.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,17 +36,17 @@
     def __call__(self, event: str, *args):
         log.debug(f"dispatching event (on_){event}")
         event = "on_" + event
 
         for func in self._event_listeners[event]:
             asyncio.create_task(maybe_coro(func, *args), name=f"berconpy-{event}")
 
-        for fut, pred in self._temporary_listeners[event]:
+        for fut, check in self._temporary_listeners[event]:
             asyncio.create_task(
-                self._try_dispatch_temporary(event, fut, pred, *args),
+                self._try_dispatch_temporary(event, fut, check, *args),
                 name=f"berconpy-temp-{event}",
             )
 
     def add_listener(self, event: str, func: MaybeCoroFunc[..., Any]):
         self._event_listeners[event].append(func)
 
     def remove_listener(self, event: str, func: MaybeCoroFunc[..., Any]):
@@ -90,60 +90,58 @@
         fut = self._add_temporary_listener(event, check)
 
         try:
             return await asyncio.wait_for(fut, timeout=timeout)
         except asyncio.TimeoutError:
             fut.cancel()
             raise
+        finally:
+            self._remove_temporary_listener(event, fut, check)
 
     def _add_temporary_listener(
         self,
         event: str,
-        predicate: MaybeCoroFunc[..., Any],
+        check: MaybeCoroFunc[..., Any],
     ) -> asyncio.Future:
         fut = asyncio.get_running_loop().create_future()
-        self._temporary_listeners[event].append((fut, predicate))
+        self._temporary_listeners[event].append((fut, check))
         return fut
 
     def _remove_temporary_listener(
         self,
         event: str,
         fut: asyncio.Future,
-        pred: MaybeCoroFunc[..., Any],
+        check: MaybeCoroFunc[..., Any],
     ) -> None:
         listeners = self._temporary_listeners[event]
-        e = (fut, pred)
+        e = (fut, check)
 
         try:
             listeners.remove(e)
         except ValueError:
             pass
 
     async def _try_dispatch_temporary(
         self,
         event: str,
         fut: asyncio.Future,
-        pred: MaybeCoroFunc[..., Any],
+        check: MaybeCoroFunc[..., Any],
         *args,
     ):
         if fut.done():
-            return self._remove_temporary_listener(event, fut, pred)
+            return
 
         try:
-            result = await maybe_coro(pred, *args)
+            check_accepted = await maybe_coro(check, *args)
         except Exception as e:
             if not fut.done():
                 fut.set_exception(e)
-            self._remove_temporary_listener(event, fut, pred)
         else:
-            if not result or fut.done():
-                return
-
-            fut.set_result(args)
-            self._remove_temporary_listener(event, fut, pred)
+            if check_accepted and not fut.done():
+                fut.set_result(args)
 
     # Specific events to provide type inference
 
     @typed_event
     @staticmethod
     @copy_doc(EventDispatcher.on_player_connect)
     def on_player_connect(player: Player, /) -> Any:
```

### Comparing `berconpy-2.1.3/src/berconpy/asyncio/io.py` & `berconpy-2.1.4/src/berconpy/asyncio/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     ClientAuthEvent,
     ClientEvent,
     ClientCommandPacket,
     ClientPacket,
     ClientCommandEvent,
     RCONClientProtocol,
     ClientMessageEvent,
+    ClientState,
 )
 
 log = logging.getLogger(__name__)
 
 if TYPE_CHECKING:
     from .client import AsyncRCONClient
 
@@ -132,32 +133,41 @@
         command_interval: float = 1.0,
     ) -> None:
         self.io_layer = None
         self.proto_layer = None
 
         self.command_attempts = command_attempts
         self.command_interval = command_interval
-        self.reset()
+
+        self._command_futures = {}
 
     def cancel_command(self, sequence: int) -> None:
         """Cancels a command in the protocol along with its associated future.
 
+        If the protocol is not logged in, usually due to a timeout
+        or the client closing, this is a no-op. Cancellation should
+        instead be handled by calling :py:meth:`reset()`.
+
         If the command sequence was not queued before, this is a no-op.
 
         """
         if self.proto_layer is None:
             raise RuntimeError("proto_layer must be assigned")
+        if self.proto_layer.state != ClientState.LOGGED_IN:
+            return
 
         self.proto_layer.invalidate_command(sequence)
         fut = self._command_futures.pop(sequence, None)
         if fut is not None:
             fut.cancel()
 
     def reset(self) -> None:
-        self._command_futures = {}
+        for fut in self._command_futures.values():
+            fut.cancel()
+        self._command_futures.clear()
 
     def set_command(self, sequence: int, message: str) -> None:
         """Notifies the future waiting on a command response packet.
 
         An alternative message may be given if the packet itself does
         not contain the full message (i.e. multipart packet).
```

### Comparing `berconpy-2.1.3/src/berconpy/asyncio/player.py` & `berconpy-2.1.4/src/berconpy/asyncio/player.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.3/src/berconpy/ban.py` & `berconpy-2.1.4/src/berconpy/ban.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.3/src/berconpy/cache.py` & `berconpy-2.1.4/src/berconpy/cache.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.3/src/berconpy/client.py` & `berconpy-2.1.4/src/berconpy/client.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.3/src/berconpy/dispatch.py` & `berconpy-2.1.4/src/berconpy/dispatch.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.3/src/berconpy/ext/arma/client.py` & `berconpy-2.1.4/src/berconpy/ext/arma/client.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.3/src/berconpy/parser.py` & `berconpy-2.1.4/src/berconpy/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,17 @@
             kwargs[k] = int(v)
 
     return kwargs
 
 
 def is_expected_message(message: str) -> bool:
     """Determines if a server message is expected."""
+    if message.startswith("Config entry:"):
+        return True
+
     return message in (
         "Ban check timed out, no response from BE Master",
         "Connected to BE Master",
         "Disconnected from BE Master",
         "Failed to resolve BE Master DNS name(s)",
     )
```

### Comparing `berconpy-2.1.3/src/berconpy/player.py` & `berconpy-2.1.4/src/berconpy/player.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.3/src/berconpy/protocol/__init__.py` & `berconpy-2.1.4/src/berconpy/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.3/src/berconpy/protocol/base.py` & `berconpy-2.1.4/src/berconpy/protocol/base.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.3/src/berconpy/protocol/check.py` & `berconpy-2.1.4/src/berconpy/protocol/check.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.3/src/berconpy/protocol/client.py` & `berconpy-2.1.4/src/berconpy/protocol/client.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.3/src/berconpy/protocol/errors.py` & `berconpy-2.1.4/src/berconpy/protocol/errors.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.3/src/berconpy/protocol/events.py` & `berconpy-2.1.4/src/berconpy/protocol/events.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.3/src/berconpy/protocol/packet.py` & `berconpy-2.1.4/src/berconpy/protocol/packet.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.3/src/berconpy/protocol/server.py` & `berconpy-2.1.4/src/berconpy/protocol/server.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.3/src/berconpy/utils.py` & `berconpy-2.1.4/src/berconpy/utils.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.3/src/berconpy.egg-info/PKG-INFO` & `berconpy-2.1.4/src/berconpy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: berconpy
-Version: 2.1.3
+Version: 2.1.4
 Summary: An async wrapper for the BattlEye RCON protocol
 Author: thegamecracks
 License: MIT
 Project-URL: Homepage, https://github.com/thegamecracks/berconpy
 Project-URL: Documentation, http://berconpy.readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/thegamecracks/berconpy/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `berconpy-2.1.3/src/berconpy.egg-info/SOURCES.txt` & `berconpy-2.1.4/src/berconpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

