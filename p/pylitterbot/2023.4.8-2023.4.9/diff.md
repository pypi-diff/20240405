# Comparing `tmp/pylitterbot-2023.4.8.tar.gz` & `tmp/pylitterbot-2023.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylitterbot-2023.4.8.tar", max compression
+gzip compressed data, was "pylitterbot-2023.4.9.tar", max compression
```

## Comparing `pylitterbot-2023.4.8.tar` & `pylitterbot-2023.4.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1076 2023-08-29 18:00:27.877727 pylitterbot-2023.4.8/LICENSE
--rw-r--r--   0        0        0     3168 2023-08-29 18:00:27.877727 pylitterbot-2023.4.8/README.md
--rw-r--r--   0        0        0      403 2023-08-29 18:00:45.986001 pylitterbot-2023.4.8/pylitterbot/__init__.py
--rw-r--r--   0        0        0     8594 2023-08-29 18:00:27.881727 pylitterbot-2023.4.8/pylitterbot/account.py
--rw-r--r--   0        0        0     1118 2023-08-29 18:00:27.881727 pylitterbot-2023.4.8/pylitterbot/activity.py
--rw-r--r--   0        0        0     4597 2023-08-29 18:00:27.881727 pylitterbot-2023.4.8/pylitterbot/enums.py
--rw-r--r--   0        0        0     1149 2023-08-29 18:00:27.881727 pylitterbot-2023.4.8/pylitterbot/event.py
--rw-r--r--   0        0        0      348 2023-08-29 18:00:27.881727 pylitterbot-2023.4.8/pylitterbot/exceptions.py
--rw-r--r--   0        0        0        0 2023-08-29 18:00:27.881727 pylitterbot-2023.4.8/pylitterbot/py.typed
--rw-r--r--   0        0        0     6170 2023-08-29 18:00:27.881727 pylitterbot-2023.4.8/pylitterbot/robot/__init__.py
--rw-r--r--   0        0        0    10446 2023-08-29 18:00:27.881727 pylitterbot-2023.4.8/pylitterbot/robot/feederrobot.py
--rw-r--r--   0        0        0     7187 2023-08-29 18:00:27.881727 pylitterbot-2023.4.8/pylitterbot/robot/litterrobot.py
--rw-r--r--   0        0        0    11704 2023-08-29 18:00:27.881727 pylitterbot-2023.4.8/pylitterbot/robot/litterrobot3.py
--rw-r--r--   0        0        0    25838 2023-08-29 18:00:27.881727 pylitterbot-2023.4.8/pylitterbot/robot/litterrobot4.py
--rw-r--r--   0        0        0     2364 2023-08-29 18:00:27.881727 pylitterbot-2023.4.8/pylitterbot/robot/models.py
--rw-r--r--   0        0        0     9365 2023-08-29 18:00:27.881727 pylitterbot-2023.4.8/pylitterbot/session.py
--rw-r--r--   0        0        0     4170 2023-08-29 18:00:27.881727 pylitterbot-2023.4.8/pylitterbot/utils.py
--rw-r--r--   0        0        0     5148 2023-08-29 18:00:27.881727 pylitterbot-2023.4.8/pylitterbot/ws_monitor.py
--rw-r--r--   0        0        0     1161 2023-08-29 18:00:45.982001 pylitterbot-2023.4.8/pyproject.toml
--rw-r--r--   0        0        0     4088 1970-01-01 00:00:00.000000 pylitterbot-2023.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-10-02 17:29:25.010079 pylitterbot-2023.4.9/LICENSE
+-rw-r--r--   0        0        0     3168 2023-10-02 17:29:25.010079 pylitterbot-2023.4.9/README.md
+-rw-r--r--   0        0        0      403 2023-10-02 17:29:45.826167 pylitterbot-2023.4.9/pylitterbot/__init__.py
+-rw-r--r--   0        0        0     8594 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/account.py
+-rw-r--r--   0        0        0     1118 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/activity.py
+-rw-r--r--   0        0        0     4597 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/enums.py
+-rw-r--r--   0        0        0     1149 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/event.py
+-rw-r--r--   0        0        0      348 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/exceptions.py
+-rw-r--r--   0        0        0        0 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/py.typed
+-rw-r--r--   0        0        0     6170 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/robot/__init__.py
+-rw-r--r--   0        0        0    10446 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/robot/feederrobot.py
+-rw-r--r--   0        0        0     7187 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/robot/litterrobot.py
+-rw-r--r--   0        0        0    11704 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/robot/litterrobot3.py
+-rw-r--r--   0        0        0    25838 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/robot/litterrobot4.py
+-rw-r--r--   0        0        0     2364 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/robot/models.py
+-rw-r--r--   0        0        0     9337 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/session.py
+-rw-r--r--   0        0        0     4170 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/utils.py
+-rw-r--r--   0        0        0     5148 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/ws_monitor.py
+-rw-r--r--   0        0        0     1176 2023-10-02 17:29:45.826167 pylitterbot-2023.4.9/pyproject.toml
+-rw-r--r--   0        0        0     4088 1970-01-01 00:00:00.000000 pylitterbot-2023.4.9/PKG-INFO
```

### Comparing `pylitterbot-2023.4.8/LICENSE` & `pylitterbot-2023.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.8/README.md` & `pylitterbot-2023.4.9/README.md`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.8/pylitterbot/account.py` & `pylitterbot-2023.4.9/pylitterbot/account.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.8/pylitterbot/activity.py` & `pylitterbot-2023.4.9/pylitterbot/activity.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.8/pylitterbot/enums.py` & `pylitterbot-2023.4.9/pylitterbot/enums.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.8/pylitterbot/event.py` & `pylitterbot-2023.4.9/pylitterbot/event.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.8/pylitterbot/robot/__init__.py` & `pylitterbot-2023.4.9/pylitterbot/robot/__init__.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.8/pylitterbot/robot/feederrobot.py` & `pylitterbot-2023.4.9/pylitterbot/robot/feederrobot.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.8/pylitterbot/robot/litterrobot.py` & `pylitterbot-2023.4.9/pylitterbot/robot/litterrobot.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.8/pylitterbot/robot/litterrobot3.py` & `pylitterbot-2023.4.9/pylitterbot/robot/litterrobot3.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.8/pylitterbot/robot/litterrobot4.py` & `pylitterbot-2023.4.9/pylitterbot/robot/litterrobot4.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.8/pylitterbot/robot/models.py` & `pylitterbot-2023.4.9/pylitterbot/robot/models.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.8/pylitterbot/session.py` & `pylitterbot-2023.4.9/pylitterbot/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Session handling for litter-robot endpoint."""
 from __future__ import annotations
 
 import logging
 from abc import ABC, abstractmethod
-from threading import Lock
+from asyncio import Lock
 from types import TracebackType
 from typing import Any, TypeVar, cast
 
 import jwt
 from aiohttp import ClientSession
 
 from .event import EVENT_UPDATE, Event
@@ -75,19 +75,19 @@
     def is_token_valid(self) -> bool:
         """Return `True` if the token is stills valid."""
 
     async def refresh_token(self, ignore_unexpired: bool = False) -> None:
         """Refresh the access token."""
         if self._token is None:
             return None
-        with self._lock:
+        async with self._lock:
             if not ignore_unexpired and self.is_token_valid():
                 return
             self._token = await self._refresh_token()
-            self.emit(EVENT_UPDATE)
+        self.emit(EVENT_UPDATE)
 
     @abstractmethod
     async def _refresh_token(self) -> dict:
         """Actual implementation to refresh the access token."""
 
     async def get_bearer_authorization(self) -> str | None:
         """Get the bearer authorization."""
@@ -163,15 +163,14 @@
         self, token: dict | None = None, websession: ClientSession | None = None
     ) -> None:
         """Initialize the session."""
         super().__init__(websession=websession)
 
         self._token = token
         self._custom_args: dict = {}
-        self._lock = Lock()
 
     def generate_args(self, url: str, **kwargs: Any) -> dict[str, Any]:
         """Generate args."""
         for key, value in next(
             (value for key, value in self._custom_args.items() if url.startswith(key)),
             {},
         ).items():
```

### Comparing `pylitterbot-2023.4.8/pylitterbot/utils.py` & `pylitterbot-2023.4.9/pylitterbot/utils.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.8/pylitterbot/ws_monitor.py` & `pylitterbot-2023.4.9/pylitterbot/ws_monitor.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.8/pyproject.toml` & `pylitterbot-2023.4.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylitterbot"
-version = "2023.4.8"
+version = "2023.4.9"
 description = "Python package for controlling Whisker automatic robots."
 authors = ["Nathan Spencer <natekspencer@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/natekspencer/pylitterbot"
 repository = "https://github.com/natekspencer/pylitterbot"
 keywords = ["Whisker", "Litter-Robot", "Feeder-Robot", "litter box", "pet feeder", "asynchronous"]
@@ -29,14 +29,14 @@
 flake8 = ">=5.0.4,<7.0.0"
 pylint = "^2.17.4"
 tox = ">=3.28,<5.0"
 pydocstyle = "^6.3.0"
 pytest-timeout = "^2.1.0"
 
 [tool.poetry-dynamic-versioning]
-enable = true
+enable = false
 vcs = "git"
 style = "semver"
 
 [build-system]
-requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `pylitterbot-2023.4.8/PKG-INFO` & `pylitterbot-2023.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylitterbot
-Version: 2023.4.8
+Version: 2023.4.9
 Summary: Python package for controlling Whisker automatic robots.
 Home-page: https://github.com/natekspencer/pylitterbot
 License: MIT
 Keywords: Whisker,Litter-Robot,Feeder-Robot,litter box,pet feeder,asynchronous
 Author: Nathan Spencer
 Author-email: natekspencer@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

