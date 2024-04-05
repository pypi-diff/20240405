# Comparing `tmp/linien-client-1.0.2rc1.tar.gz` & `tmp/linien-client-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien-client-1.0.2rc1.tar", last modified: Fri Apr  5 08:31:41 2024, max compression
+gzip compressed data, was "linien-client-2.0.0rc1.tar", last modified: Fri Apr  5 13:10:32 2024, max compression
```

## Comparing `linien-client-1.0.2rc1.tar` & `linien-client-2.0.0rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:41.527799 linien-client-1.0.2rc1/
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-05 08:31:41.527799 linien-client-1.0.2rc1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:41.523799 linien-client-1.0.2rc1/linien_client/
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-05 08:31:26.000000 linien-client-1.0.2rc1/linien_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-05 08:31:26.000000 linien-client-1.0.2rc1/linien_client/communication.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-05 08:31:26.000000 linien-client-1.0.2rc1/linien_client/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-04-05 08:31:26.000000 linien-client-1.0.2rc1/linien_client/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-05 08:31:26.000000 linien-client-1.0.2rc1/linien_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-04-05 08:31:26.000000 linien-client-1.0.2rc1/linien_client/remote_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:41.527799 linien-client-1.0.2rc1/linien_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-05 08:31:41.000000 linien-client-1.0.2rc1/linien_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-05 08:31:41.000000 linien-client-1.0.2rc1/linien_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 08:31:41.000000 linien-client-1.0.2rc1/linien_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-05 08:31:41.000000 linien-client-1.0.2rc1/linien_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 08:31:41.000000 linien-client-1.0.2rc1/linien_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 08:31:41.527799 linien-client-1.0.2rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-05 08:31:26.000000 linien-client-1.0.2rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:10:32.776642 linien-client-2.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-05 13:10:32.776642 linien-client-2.0.0rc1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:10:32.772642 linien-client-2.0.0rc1/linien_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-05 13:10:16.000000 linien-client-2.0.0rc1/linien_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-04-05 13:10:16.000000 linien-client-2.0.0rc1/linien_client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-05 13:10:16.000000 linien-client-2.0.0rc1/linien_client/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-05 13:10:16.000000 linien-client-2.0.0rc1/linien_client/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-05 13:10:16.000000 linien-client-2.0.0rc1/linien_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9070 2024-04-05 13:10:16.000000 linien-client-2.0.0rc1/linien_client/remote_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:10:32.776642 linien-client-2.0.0rc1/linien_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-05 13:10:32.000000 linien-client-2.0.0rc1/linien_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-05 13:10:32.000000 linien-client-2.0.0rc1/linien_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:10:32.000000 linien-client-2.0.0rc1/linien_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-05 13:10:32.000000 linien-client-2.0.0rc1/linien_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 13:10:32.000000 linien-client-2.0.0rc1/linien_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-05 13:10:16.000000 linien-client-2.0.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:10:32.776642 linien-client-2.0.0rc1/setup.cfg
```

### Comparing `linien-client-1.0.2rc1/PKG-INFO` & `linien-client-2.0.0rc1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: linien-client
-Version: 1.0.2rc1
+Version: 2.0.0rc1
 Summary: Client components of the Linien spectroscopy lock application.
-Home-page: https://github.com/linien-org/linien/
-Author: Benjamin Wiegand
-Author-email: highwaychile@posteo.de
-Maintainer: Bastian Leykauf
-Maintainer-email: leykauf@physik.hu-berlin.de
+Author-email: Benjamin Wiegand <benjamin.wiegand@physik.hu-berlin.de>, Bastian Leykauf <leykauf@physik.hu-berlin.de>, Robert Jördens <rj@quartiq.de>, Christian Freier <christian.freier@gmail.com>, Doron Behar <doron.behar@gmail.com>
+Maintainer-email: Bastian Leykauf <leykauf@physik.hu-berlin.de>
+Project-URL: Homepage, https://github.com/linien-org/linien/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: fabric>=2.7.0
-Requires-Dist: typing_extensions>=4.5.0
-Requires-Dist: linien-common==1.0.2rc1
+Requires-Dist: fabric<3.0,>=2.7.0
+Requires-Dist: typing_extensions<5.0,>=4.5.0
+Requires-Dist: linien-common==2.0.0rc1
 
 Have a look at the [project repository](https://github.com/linien-org/linien) for installation instructions.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `linien-client-1.0.2rc1/linien_client/__init__.py` & `linien-client-2.0.0rc1/linien_client/__init__.py`

 * *Files identical despite different names*

### Comparing `linien-client-1.0.2rc1/linien_client/connection.py` & `linien-client-2.0.0rc1/linien_client/connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright 2018-2022 Benjamin Wiegand <benjamin.wiegand@physik.hu-berlin.de>
-# Copyright 2021-2022 Bastian Leykauf <leykauf@physik.hu-berlin.de>
+# Copyright 2021-2023 Bastian Leykauf <leykauf@physik.hu-berlin.de>
 #
 # This file is part of Linien and based on redpid.
 #
 # Linien is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -13,93 +13,77 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 import logging
-import random
-import string
 from socket import gaierror
 from time import sleep
 from traceback import print_exc
 from typing import Callable, Optional
 
 import rpyc
-from linien_common.config import DEFAULT_SERVER_PORT
+from linien_common.communication import LinienControlService
 
 from . import __version__
-from .communication import LinienControlService
 from .deploy import hash_username_and_password, start_remote_server
+from .device import Device, generate_random_key
 from .exceptions import (
     GeneralConnectionError,
     InvalidServerVersionException,
     RPYCAuthenticationException,
     ServerNotRunningException,
 )
 from .remote_parameters import RemoteParameters
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 
 class ServiceWithAuth(rpyc.Service):
-    def __init__(self, uuid: str, user: str, password: str) -> None:
+    def __init__(self, uuid: str, device: Device) -> None:
         super().__init__()
         self.exposed_uuid = uuid
-        self.auth_hash = hash_username_and_password(user, password).encode("utf-8")
+        self.auth_hash = hash_username_and_password(
+            device.username, device.password
+        ).encode("utf-8")
 
     def _connect(self, channel, config):
         channel.stream.sock.send(self.auth_hash)  # send hash before rpyc takes over
+        logger.debug("Sent authentication hash")
         return super()._connect(channel, config)
 
 
 class LinienClient:
-    def __init__(
-        self,
-        host: str,
-        user: str,
-        password: str,
-        port: int = DEFAULT_SERVER_PORT,
-        name: str = "",
-    ):
+    def __init__(self, device: Device) -> None:
         """Connect to a RedPitaya that runs linien server."""
-        self.host = host
-        self.user = user
-        self.password = password
-        self.port = port
-        self.name = name
-
-        if self.host in ("localhost", "127.0.0.1"):
-            # RP is configured such that "localhost" doesn't point to 127.0.0.1 in all
-            # cases
-            self.host = "127.0.0.1"
-
-        self.uuid = "".join(random.choice(string.ascii_lowercase) for _ in range(10))
+        self.device = device
+        self.uuid = generate_random_key()
 
         # for exposing client's uuid to server
-        self.client_service = ServiceWithAuth(self.uuid, self.user, self.password)
+        self.client_service = ServiceWithAuth(self.uuid, self.device)
 
     def connect(
         self,
         autostart_server: bool,
         use_parameter_cache: bool,
         call_on_error: Optional[Callable] = None,
     ) -> None:
         self.connection = None
 
         i = -1
         while True:
             i += 1
             try:
-                logger.info(f"Try to connect to {self.host}:{self.port}")
+                logger.info(f"Try to connect to {self.device.host}:{self.device.port}")
 
                 self.connection = rpyc.connect(
-                    self.host,
-                    self.port,
+                    self.device.host,
+                    self.device.port,
                     service=self.client_service,
                     config={"allow_pickle": True},
                 )
 
                 cls = RemoteParameters
                 if call_on_error:
                     cls = self._catch_network_errors(cls, call_on_error)
@@ -108,26 +92,26 @@
                     self.connection.root, self.uuid, use_parameter_cache
                 )
 
                 self.control: LinienControlService = self.connection.root
                 break
             except gaierror:
                 # host not found
-                logger.error(f"Error: host {self.host} not found")
+                logger.error(f"Error: host {self.device.host} not found")
                 break
             except EOFError:
                 logger.error("EOFError! Probably authentication failed")
                 raise RPYCAuthenticationException()
             except ConnectionRefusedError:
                 if not autostart_server:
                     raise ServerNotRunningException()
 
                 if i == 0:
                     logger.error("Server is not running. Launching it!")
-                    start_remote_server(self.host, self.user, self.password)
+                    start_remote_server(self.device)
                     sleep(3)
                 else:
                     if i < 20:
                         logger.info(
                             "Server still not running, waiting (may take some time)."
                         )
                         sleep(1)
```

### Comparing `linien-client-1.0.2rc1/linien_client/deploy.py` & `linien-client-2.0.0rc1/linien_client/deploy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright 2018-2022 Benjamin Wiegand <benjamin.wiegand@physik.hu-berlin.de>
-# Copyright 2021-2022 Bastian Leykauf <leykauf@physik.hu-berlin.de>
+# Copyright 2021-2023 Bastian Leykauf <leykauf@physik.hu-berlin.de>
 #
 # This file is part of Linien and based on redpid.
 #
 # Linien is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -24,99 +24,109 @@
 from fabric import Connection
 from linien_client.exceptions import (
     InvalidServerVersionException,
     ServerNotInstalledException,
 )
 from linien_common.communication import hash_username_and_password
 
+from .device import Device
+
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 
 def read_remote_version(
-    host: str, user: str, password: str, port: int = 22, out_stream=sys.stdout
+    device: Device, ssh_port: int = 22, out_stream=sys.stdout
 ) -> str:
     """Read the remote version of linien."""
 
     if not out_stream:
         # sys.stdout is not available in the pyinstaller build, redirect it to avoid
         # AttributeError: 'NoneType' object has no attribute 'write'
         out_stream = open(os.devnull, "w")
 
     with Connection(
-        host, user=user, port=port, connect_kwargs={"password": password}
+        device.host,
+        user=device.username,
+        port=ssh_port,
+        connect_kwargs={"password": device.password},
     ) as conn:
         result = conn.run(
             'python3 -c "import linien_server; print(linien_server.__version__);"',
             out_stream=out_stream,
             err_stream=out_stream,
             warn=True,
         )
     if result.ok:
         return result.stdout.strip()
     else:
         raise ServerNotInstalledException()
 
 
 def start_remote_server(
-    host: str, user: str, password: str, port: int = 22, out_stream=sys.stdout
+    device: Device, ssh_port: int = 22, out_stream=sys.stdout
 ) -> None:
     """Start the remote linien server."""
 
     if not out_stream:
         # sys.stdout is not available in the pyinstaller build, redirect it to avoid
         # AttributeError: 'NoneType' object has no attribute 'write'
         out_stream = open(os.devnull, "w")
 
     with Connection(
-        host, user=user, port=port, connect_kwargs={"password": password}
+        device.host,
+        user=device.username,
+        port=ssh_port,
+        connect_kwargs={"password": device.password},
     ) as conn:
         local_version = linien_client.__version__.split("+")[0]
-        remote_version = read_remote_version(host, user, password, port).split("+")[0]
+        remote_version = read_remote_version(device, ssh_port).split("+")[0]
 
         if (local_version != remote_version) and not ("dev" in local_version):
             raise InvalidServerVersionException(local_version, remote_version)
 
         logger.debug("Sending credentials")
         conn.run(
             'python3 -c "from linien_common.communication import write_hash_to_file;'
-            f"write_hash_to_file('{hash_username_and_password(user, password)}')\"",
+            f"write_hash_to_file('{hash_username_and_password(device.username, device.password)}')\"",  # noqa E501
             out_stream=out_stream,
             err_stream=out_stream,
             warn=True,
         )
 
         logger.debug("Starting server")
         conn.run(
-            "linien_start_server.sh",
+            "linien-server start",
             out_stream=out_stream,
             err_stream=out_stream,
             warn=True,
         )
 
 
 def install_remote_server(
-    host: str, user: str, password: str, port: int = 22, out_stream=sys.stdout
-):
+    device: Device, ssh_port: int = 22, out_stream=sys.stdout
+) -> None:
     """Install the remote linien server."""
 
     if not out_stream:
         # sys.stdout is not available in the pyinstaller build
         out_stream = open(os.devnull, "w")
 
     with Connection(
-        host, user=user, port=port, connect_kwargs={"password": password}
+        device.host,
+        user=device.username,
+        port=ssh_port,
+        connect_kwargs={"password": device.password},
     ) as conn:
         local_version = linien_client.__version__.split("+")[0]
         cmds = [
-            "linien_stop_server.sh",
+            "linien-server stop",
             "pip3 uninstall linien-server -y",
             "pip3 uninstall linien-common -y",
             f"pip3 install linien-server=={local_version} --no-cache-dir",
-            "linien_install_requirements.sh",
         ]
         for cmd in cmds:
             out_stream.write(f">> {cmd}\n")
             result = conn.run(
                 cmd, out_stream=out_stream, err_stream=out_stream, warn=True
             )
             if result.ok:
```

### Comparing `linien-client-1.0.2rc1/linien_client/exceptions.py` & `linien-client-2.0.0rc1/linien_client/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,16 +35,15 @@
 
 class InvalidServerVersionException(Exception):
     def __init__(self, client_version, remote_version):
         self.client_version = client_version
         self.remote_version = remote_version
 
         super().__init__(
-            "Version mismatch: Client is %s and server is %s"
-            % (client_version, remote_version)
+            f"Version mismatch: Client is {client_version}, server is {remote_version}"
         )
 
 
 class ServerNotInstalledException(Exception):
     pass
```

### Comparing `linien-client-1.0.2rc1/linien_client/remote_parameters.py` & `linien-client-2.0.0rc1/linien_client/remote_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,18 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from typing import Any, Callable, Dict, Iterator, List, Tuple, Union
 
-from linien_common.communication import pack, unpack
+from linien_common.communication import LinienControlService, pack, unpack
 from rpyc import async_
 from rpyc.core.async_ import AsyncResult
 
-from .communication import LinienControlService
-
 
 class RemoteParameter:
     """A helper class for `RemoteParameters`, representing a single remote parameter."""
 
     def __init__(
         self,
         parent: "RemoteParameters",
@@ -60,28 +58,28 @@
     def log(self) -> bool:
         return self.parent.remote.exposed_get_parameter_log(self.name)
 
     @log.setter
     def log(self, value: bool) -> None:
         self.parent.remote.exposed_set_parameter_log(self.name, value)
 
-    def add_callback(self, callback: Callable, call_with_first_value: bool = True):
+    def add_callback(self, callback: Callable, call_immediately: bool = False):
         """
         Register a callback function that is called whenever the parameter changes.
         """
 
         if self.name not in self.parent._callbacks and not self.use_cache:
             # Make sure that the server knows that we want to be notified about changes.
             # Parameters that use the cache are already registered, see `__init__`.
             self.parent._listeners_pending_remote_registration.append(self.name)
 
         self.parent._callbacks.setdefault(self.name, [])
         self.parent._callbacks[self.name].append(callback)
 
-        if call_with_first_value:
+        if call_immediately:
             callback(self.value)
 
     def reset(self) -> None:
         """Reset the value to its initial value"""
         self.parent.remote.exposed_reset_param(self.name)
 
     def update_cache(self, value: Any) -> None:
@@ -108,15 +106,15 @@
         self._async_changed_parameters_queue: Union[AsyncResult, None] = None
         self._async_listener_registering: Union[AsyncResult, None] = None
 
         self._listeners_pending_remote_registration: List[str] = []
         self._callbacks: Dict[str, List[Callable]] = {}
 
         # mimic functionality of `parameters.Parameters`:
-        all_parameters = unpack(self.remote.exposed_init_parameter_sync(self.uuid))
+        all_parameters = self.remote.exposed_init_parameter_sync(self.uuid)
         for name, value, can_be_cached, restorable, loggable, log in all_parameters:
             param = RemoteParameter(
                 parent=self,
                 name=name,
                 use_cache=use_cache and can_be_cached,
                 restorable=restorable,
                 loggable=loggable,
@@ -184,17 +182,15 @@
                 self._listeners_pending_remote_registration.clear()
 
         if (
             self._async_changed_parameters_queue is not None
             and self._async_changed_parameters_queue.ready
         ):
             # We have a result.
-            queue: List[Tuple[str, Any]] = unpack(
-                self._async_changed_parameters_queue.value
-            )
+            queue: List[Tuple[str, Any]] = self._async_changed_parameters_queue.value
 
             # Now that we have our result, we can start the next call.
             self._async_changed_parameters_queue = async_(
                 self.remote.exposed_get_changed_parameters_queue
             )(self.uuid)
 
             # Before calling listeners, we update cache for all received parameters at
```

### Comparing `linien-client-1.0.2rc1/linien_client.egg-info/PKG-INFO` & `linien-client-2.0.0rc1/linien_client.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: linien-client
-Version: 1.0.2rc1
+Version: 2.0.0rc1
 Summary: Client components of the Linien spectroscopy lock application.
-Home-page: https://github.com/linien-org/linien/
-Author: Benjamin Wiegand
-Author-email: highwaychile@posteo.de
-Maintainer: Bastian Leykauf
-Maintainer-email: leykauf@physik.hu-berlin.de
+Author-email: Benjamin Wiegand <benjamin.wiegand@physik.hu-berlin.de>, Bastian Leykauf <leykauf@physik.hu-berlin.de>, Robert Jördens <rj@quartiq.de>, Christian Freier <christian.freier@gmail.com>, Doron Behar <doron.behar@gmail.com>
+Maintainer-email: Bastian Leykauf <leykauf@physik.hu-berlin.de>
+Project-URL: Homepage, https://github.com/linien-org/linien/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: fabric>=2.7.0
-Requires-Dist: typing_extensions>=4.5.0
-Requires-Dist: linien-common==1.0.2rc1
+Requires-Dist: fabric<3.0,>=2.7.0
+Requires-Dist: typing_extensions<5.0,>=4.5.0
+Requires-Dist: linien-common==2.0.0rc1
 
 Have a look at the [project repository](https://github.com/linien-org/linien) for installation instructions.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

