# Comparing `tmp/hat_gateway-0.5.9-cp38.cp39-none-any.whl.zip` & `tmp/hat_gateway-0.6.0-cp310.cp311.cp312-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,34 @@
-Zip file size: 21806 bytes, number of entries: 19
--rw-r--r--  2.0 unx       14 b- defN 21-Feb-19 20:16 hat/gateway/__init__.py
--rw-r--r--  2.0 unx      128 b- defN 21-Apr-08 11:27 hat/gateway/__main__.py
--rw-r--r--  2.0 unx     2615 b- defN 21-Feb-22 22:26 hat/gateway/common.py
--rw-r--r--  2.0 unx     7801 b- defN 21-Nov-13 00:02 hat/gateway/engine.py
--rw-r--r--  2.0 unx     4801 b- defN 21-Nov-29 22:12 hat/gateway/json_schema_repo.json
--rw-r--r--  2.0 unx     3728 b- defN 21-Nov-10 14:31 hat/gateway/main.py
--rw-r--r--  2.0 unx       22 b- defN 21-Feb-19 20:16 hat/gateway/devices/__init__.py
--rw-r--r--  2.0 unx       21 b- defN 21-May-19 00:33 hat/gateway/devices/modbus/__init__.py
--rw-r--r--  2.0 unx      353 b- defN 21-Aug-10 11:19 hat/gateway/devices/modbus/master/__init__.py
--rw-r--r--  2.0 unx     5843 b- defN 21-May-25 14:28 hat/gateway/devices/modbus/master/connection.py
--rw-r--r--  2.0 unx     8408 b- defN 21-Dec-02 20:31 hat/gateway/devices/modbus/master/device.py
--rw-r--r--  2.0 unx     5007 b- defN 21-May-26 23:27 hat/gateway/devices/modbus/master/event_client.py
--rw-r--r--  2.0 unx    12777 b- defN 21-Dec-16 17:48 hat/gateway/devices/modbus/master/remote_device.py
--rw-r--r--  2.0 unx    11358 b- defN 21-Dec-16 17:50 hat_gateway-0.5.9.dist-info/LICENSE
--rw-r--r--  2.0 unx     2232 b- defN 21-Dec-16 17:50 hat_gateway-0.5.9.dist-info/METADATA
--rw-r--r--  2.0 unx      112 b- defN 21-Dec-16 17:50 hat_gateway-0.5.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       71 b- defN 21-Dec-16 17:50 hat_gateway-0.5.9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 21-Dec-16 17:50 hat_gateway-0.5.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1683 b- defN 21-Dec-16 17:50 hat_gateway-0.5.9.dist-info/RECORD
-19 files, 66978 bytes uncompressed, 19008 bytes compressed:  71.6%
+Zip file size: 51678 bytes, number of entries: 32
+?rw-------  2.0 unx       22 b- defN 24-Mar-24 23:49 hat/gateway/devices/__init__.py
+?rw-------  2.0 unx    17668 b- defN 24-Mar-24 23:49 hat/gateway/devices/iec101/slave.py
+?rw-------  2.0 unx       30 b- defN 24-Mar-24 23:49 hat/gateway/devices/iec103/__init__.py
+?rw-------  2.0 unx     2405 b- defN 24-Mar-24 23:49 hat/gateway/common.py
+?rw-------  2.0 unx    19355 b- defN 24-Mar-24 23:49 hat/gateway/devices/iec101/master.py
+?rw-------  2.0 unx    16472 b- defN 24-Mar-24 23:49 hat/gateway/devices/modbus/master/remote_device.py
+?rw-------  2.0 unx     8067 b- defN 24-Mar-24 23:49 hat/gateway/devices/modbus/master/connection.py
+?rw-------  2.0 unx       30 b- defN 24-Mar-24 23:49 hat/gateway/devices/iec104/__init__.py
+?rw-------  2.0 unx       21 b- defN 24-Mar-24 23:49 hat/gateway/devices/modbus/__init__.py
+?rw-------  2.0 unx    10349 b- defN 24-Mar-24 23:49 hat/gateway/devices/snmp/manager.py
+?rw-------  2.0 unx      349 b- defN 24-Mar-24 23:49 hat/gateway/devices/modbus/master/__init__.py
+?rw-------  2.0 unx       14 b- defN 24-Mar-24 23:49 hat/gateway/__init__.py
+?rw-------  2.0 unx    15260 b- defN 24-Mar-24 23:49 hat/gateway/devices/iec103/master.py
+?rw-------  2.0 unx     5434 b- defN 24-Mar-24 23:49 hat/gateway/devices/modbus/master/eventer_client.py
+?rw-------  2.0 unx    16277 b- defN 24-Mar-24 23:49 hat/gateway/devices/iec101/common.py
+?rw-------  2.0 unx     7162 b- defN 24-Mar-24 23:49 hat/gateway/engine.py
+?rw-------  2.0 unx    14768 b- defN 24-Mar-24 23:49 hat/gateway/devices/iec104/slave.py
+?rw-------  2.0 unx    33538 b- defN 24-Mar-24 23:49 hat/gateway/json_schema_repo.json
+?rw-------  2.0 unx       30 b- defN 24-Mar-24 23:49 hat/gateway/devices/iec101/__init__.py
+?rw-------  2.0 unx      128 b- defN 24-Mar-24 23:49 hat/gateway/__main__.py
+?rw-------  2.0 unx     7864 b- defN 24-Mar-24 23:49 hat/gateway/devices/modbus/master/device.py
+?rw-------  2.0 unx    13561 b- defN 24-Mar-24 23:49 hat/gateway/devices/iec104/master.py
+?rw-------  2.0 unx     4251 b- defN 24-Mar-24 23:49 hat/gateway/devices/iec104/ssl.py
+?rw-------  2.0 unx     3973 b- defN 24-Mar-24 23:49 hat/gateway/runner.py
+?rw-------  2.0 unx       56 b- defN 24-Mar-24 23:49 hat/gateway/devices/iec104/common.py
+?rw-------  2.0 unx     1991 b- defN 24-Mar-24 23:49 hat/gateway/main.py
+?rw-------  2.0 unx       19 b- defN 24-Mar-24 23:49 hat/gateway/devices/snmp/__init__.py
+?rw-------  2.0 unx    11358 b- defN 24-Mar-24 23:49 hat_gateway-0.6.0.dist-info/LICENSE
+?rw-------  2.0 unx       54 b- defN 24-Mar-24 23:49 hat_gateway-0.6.0.dist-info/entry_points.txt
+?rw-------  2.0 unx     2826 b- defN 24-Mar-24 23:49 hat_gateway-0.6.0.dist-info/METADATA
+?rw-------  2.0 unx      118 b- defN 24-Mar-24 23:49 hat_gateway-0.6.0.dist-info/WHEEL
+?rw-------  2.0 unx     2875 b- defN 24-Mar-24 23:49 hat_gateway-0.6.0.dist-info/RECORD
+32 files, 216325 bytes uncompressed, 46992 bytes compressed:  78.3%
```

## zipnote {}

```diff
@@ -1,58 +1,97 @@
-Filename: hat/gateway/__init__.py
+Filename: hat/gateway/devices/__init__.py
 Comment: 
 
-Filename: hat/gateway/__main__.py
+Filename: hat/gateway/devices/iec101/slave.py
+Comment: 
+
+Filename: hat/gateway/devices/iec103/__init__.py
 Comment: 
 
 Filename: hat/gateway/common.py
 Comment: 
 
-Filename: hat/gateway/engine.py
+Filename: hat/gateway/devices/iec101/master.py
 Comment: 
 
-Filename: hat/gateway/json_schema_repo.json
+Filename: hat/gateway/devices/modbus/master/remote_device.py
 Comment: 
 
-Filename: hat/gateway/main.py
+Filename: hat/gateway/devices/modbus/master/connection.py
 Comment: 
 
-Filename: hat/gateway/devices/__init__.py
+Filename: hat/gateway/devices/iec104/__init__.py
 Comment: 
 
 Filename: hat/gateway/devices/modbus/__init__.py
 Comment: 
 
+Filename: hat/gateway/devices/snmp/manager.py
+Comment: 
+
 Filename: hat/gateway/devices/modbus/master/__init__.py
 Comment: 
 
-Filename: hat/gateway/devices/modbus/master/connection.py
+Filename: hat/gateway/__init__.py
+Comment: 
+
+Filename: hat/gateway/devices/iec103/master.py
+Comment: 
+
+Filename: hat/gateway/devices/modbus/master/eventer_client.py
+Comment: 
+
+Filename: hat/gateway/devices/iec101/common.py
+Comment: 
+
+Filename: hat/gateway/engine.py
+Comment: 
+
+Filename: hat/gateway/devices/iec104/slave.py
+Comment: 
+
+Filename: hat/gateway/json_schema_repo.json
+Comment: 
+
+Filename: hat/gateway/devices/iec101/__init__.py
+Comment: 
+
+Filename: hat/gateway/__main__.py
 Comment: 
 
 Filename: hat/gateway/devices/modbus/master/device.py
 Comment: 
 
-Filename: hat/gateway/devices/modbus/master/event_client.py
+Filename: hat/gateway/devices/iec104/master.py
 Comment: 
 
-Filename: hat/gateway/devices/modbus/master/remote_device.py
+Filename: hat/gateway/devices/iec104/ssl.py
+Comment: 
+
+Filename: hat/gateway/runner.py
+Comment: 
+
+Filename: hat/gateway/devices/iec104/common.py
+Comment: 
+
+Filename: hat/gateway/main.py
 Comment: 
 
-Filename: hat_gateway-0.5.9.dist-info/LICENSE
+Filename: hat/gateway/devices/snmp/__init__.py
 Comment: 
 
-Filename: hat_gateway-0.5.9.dist-info/METADATA
+Filename: hat_gateway-0.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: hat_gateway-0.5.9.dist-info/WHEEL
+Filename: hat_gateway-0.6.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: hat_gateway-0.5.9.dist-info/entry_points.txt
+Filename: hat_gateway-0.6.0.dist-info/METADATA
 Comment: 
 
-Filename: hat_gateway-0.5.9.dist-info/top_level.txt
+Filename: hat_gateway-0.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: hat_gateway-0.5.9.dist-info/RECORD
+Filename: hat_gateway-0.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hat/gateway/common.py

```diff
@@ -1,81 +1,78 @@
 """Common gateway interfaces"""
 
-from pathlib import Path
+from collections.abc import Collection
 import abc
+import importlib.resources
 import typing
 
 from hat import aio
 from hat import json
 import hat.event.common
+import hat.event.eventer
 import hat.monitor.common
 
 
-json_schema_repo: json.SchemaRepository = json.SchemaRepository(
-    json.json_schema_repo,
-    hat.monitor.common.json_schema_repo,
-    json.SchemaRepository.from_json(Path(__file__).parent /
-                                    'json_schema_repo.json'))
-"""JSON schema repository"""
+with importlib.resources.as_file(importlib.resources.files(__package__) /
+                                 'json_schema_repo.json') as _path:
+    json_schema_repo: json.SchemaRepository = json.SchemaRepository(
+        json.json_schema_repo,
+        json.SchemaRepository.from_json(_path))
+    """JSON schema repository"""
 
-DeviceConf = json.Data
+
+class Device(aio.Resource):
+    """Device interface"""
+
+    @abc.abstractmethod
+    async def process_events(self,
+                             events: Collection[hat.event.common.Event]):
+        """Process received events
+
+        This method can be coroutine or regular function.
+
+        """
+
+
+DeviceConf: typing.TypeAlias = json.Data
 """Device configuration"""
 
-EventTypePrefix = hat.event.common.EventType
+EventTypePrefix: typing.TypeAlias = tuple[hat.event.common.EventTypeSegment,
+                                          hat.event.common.EventTypeSegment,
+                                          hat.event.common.EventTypeSegment,
+                                          hat.event.common.EventTypeSegment]
 """Event type prefix"""
 
-CreateDevice = aio.AsyncCallable[
-    [DeviceConf, 'DeviceEventClient', EventTypePrefix],
-    'Device']
+CreateDevice: typing.TypeAlias = aio.AsyncCallable[[DeviceConf,
+                                                    hat.event.eventer.Client,
+                                                    EventTypePrefix],
+                                                   'Device']
 """Create device callable"""
 
 
-class Device(aio.Resource):
-    """Device interface
+class DeviceInfo(typing.NamedTuple):
+    """Device info
 
     Device is implemented as python module which is dynamically imported.
-    It is expected that this module implements:
+    It is expected that this module contains `info` which is instance of
+    `DeviceInfo`.
 
-        * device_type (str): device type identification
-        * json_schema_id (Optional[str]): JSON schema id
-        * json_schema_repo (Optional[json.SchemaRepository]): JSON schema repo
-        * create (CreateDevice): creating new device instance
-
-    If module defines JSON schema repositoy and JSON schema id, JSON schema
+    If device defines JSON schema repository and JSON schema id, JSON schema
     repository will be used for additional validation of device configuration
     with JSON schema id.
 
-    `create` is called with device configuration, appropriate instance of
-    `DeviceEventClient` and event type prefix. Event type prefix is defined
-    as [``gateway``, `<gateway_name>`, `<device_type>`, `<device_name>`].
-
     """
+    type: str
+    create: CreateDevice
+    json_schema_id: str | None = None
+    json_schema_repo: json.SchemaRepository | None = None
 
 
-class DeviceEventClient(aio.Resource):
-    """Device's event client interface"""
-
-    @abc.abstractmethod
-    async def receive(self) -> typing.List[hat.event.common.Event]:
-        """Receive device events"""
-
-    @abc.abstractmethod
-    def register(self, events: typing.List[hat.event.common.RegisterEvent]):
-        """Register device events"""
-
-    @abc.abstractmethod
-    async def register_with_response(self,
-                                     events: typing.List[hat.event.common.RegisterEvent]  # NOQA
-                                     ) -> typing.List[typing.Optional[hat.event.common.Event]]:  # NOQA
-        """Register device events
-
-        Each `RegisterEvent` from `events` is paired with results `Event` if
-        new event was successfully created or `None` is new event could not be
-        created.
+def import_device_info(py_module_str: str) -> DeviceInfo:
+    """Import module info"""
+    py_module = importlib.import_module(py_module_str)
+    info = py_module.info
 
-        """
+    if not isinstance(info, DeviceInfo):
+        raise Exception('invalid device implementation')
 
-    @abc.abstractmethod
-    async def query(self,
-                    data: hat.event.common.QueryData
-                    ) -> typing.List[hat.event.common.Event]:
-        """Query device events from server"""
+    return info
```

## hat/gateway/engine.py

```diff
@@ -1,248 +1,212 @@
 """Gateway engine"""
 
+from collections.abc import Collection, Iterable
+import asyncio
 import collections
+import contextlib
 import importlib
 import logging
 
 from hat import aio
 from hat import json
-from hat.gateway import common
-import hat.event.client
 import hat.event.common
+import hat.event.eventer
+
+from hat.gateway import common
 
 
 mlog: logging.Logger = logging.getLogger(__name__)
 """Module logger"""
 
 
-async def create_engine(conf: json.Data,
-                        client: hat.event.client.Client
-                        ) -> 'Engine':
-    """Create gateway engine"""
-    engine = Engine()
-    engine._client = client
-    engine._devices = {}
-
-    try:
-        for device_conf in conf['devices']:
-            device = _DeviceProxy(device_conf, client, conf['gateway_name'])
-            if device.event_type_prefix in engine._devices:
-                raise Exception(f'duplicate device identifier: '
-                                f'{device.event_type_prefix}')
-            engine._devices[device.event_type_prefix] = device
-
-        engine.async_group.spawn(engine._read_loop)
-
-    except BaseException:
-        await aio.uncancellable(engine.async_close())
-        raise
+class Engine(aio.Resource):
+    """Gateway engine"""
 
-    return engine
+    def __init__(self,
+                 conf: json.Data,
+                 eventer_client: hat.event.eventer.Client,
+                 events_queue_size: int = 1024):
+        self._eventer_client = eventer_client
+        self._async_group = aio.Group()
+        self._events_queue = aio.Queue(events_queue_size)
+        self._devices = {}
 
+        for device_conf in conf['devices']:
+            module = importlib.import_module(device_conf['module'])
+            event_type_prefix = ('gateway',
+                                 conf['gateway_name'],
+                                 module.info.type,
+                                 device_conf['name'])
+
+            self._devices[event_type_prefix] = _DeviceProxy(
+                conf=device_conf,
+                eventer_client=eventer_client,
+                event_type_prefix=event_type_prefix,
+                async_group=self.async_group,
+                create_device=module.info.create,
+                events_queue_size=events_queue_size)
 
-class Engine(aio.Resource):
-    """Gateway engine"""
+        self.async_group.spawn(self._run)
 
     @property
     def async_group(self) -> aio.Group:
         """Async group"""
-        return self._client.async_group
+        return self._async_group
+
+    async def process_events(self, events: Iterable[hat.event.common.Event]):
+        await self._events_queue.put(events)
 
-    async def _read_loop(self):
+    async def _run(self):
         try:
-            events = []
+            event_types = [(*event_type_prefix, 'system', 'enable')
+                           for event_type_prefix in self._devices.keys()]
+            params = hat.event.common.QueryLatestParams(event_types)
+            result = await self._eventer_client.query(params)
+
+            for event in result.events:
+                event_type_prefix = event.type[:4]
+                device = self._devices.get(event_type_prefix)
+                if not device or event.type[4:] != ('system', 'enable'):
+                    continue
 
-            if self._devices:
-                event_types = [(*device.event_type_prefix, 'system', 'enable')
-                               for device in self._devices.values()]
-                query = hat.event.common.QueryData(event_types=event_types,
-                                                   unique_type=True)
-                events = await self._client.query(query)
+                device.set_enable(
+                    isinstance(event.payload,
+                               hat.event.common.EventPayloadJson) and
+                    event.payload.data is True)
 
             while True:
-                device_events = {}
+                events = await self._events_queue.get()
+
+                device_events = collections.defaultdict(collections.deque)
 
                 for event in events:
-                    event_type_prefix = event.event_type[:4]
+                    event_type_prefix = event.type[:4]
                     device = self._devices.get(event_type_prefix)
                     if not device:
+                        mlog.warning("received invalid event type prefix %s",
+                                     event_type_prefix)
                         continue
 
-                    if device not in device_events:
-                        device_events[device] = collections.deque()
-                    device_events[device].append(event)
-
-                for device, events in device_events.items():
-                    device.receive_queue.put_nowait(events)
+                    if event.type[4:] == ('system', 'enable'):
+                        device.set_enable(
+                            isinstance(event.payload,
+                                       hat.event.common.EventPayloadJson) and
+                            event.payload.data is True)
 
-                events = await self._client.receive()
+                    else:
+                        device_events[device].append(event)
 
-        except ConnectionError:
-            pass
+                for device, dev_events in device_events.items():
+                    await device.process_events(dev_events)
 
         except Exception as e:
-            mlog.error('read loop error: %s', e, exc_info=e)
+            mlog.error("engine run error: %s", e, exc_info=e)
 
         finally:
             self.close()
+            self._events_queue.close()
 
 
 class _DeviceProxy(aio.Resource):
 
-    def __init__(self, conf, client, gateway_name):
+    def __init__(self,
+                 conf: json.Data,
+                 eventer_client: hat.event.eventer.Client,
+                 event_type_prefix: common.EventTypePrefix,
+                 async_group: aio.Group,
+                 create_device: common.CreateDevice,
+                 events_queue_size: int = 1024):
         self._conf = conf
-        self._client = client
-        self._receive_queue = aio.Queue()
-        self._events_queues_queue = aio.Queue()
-        self._device_module = importlib.import_module(conf['module'])
-        self._event_type_prefix = ('gateway', gateway_name,
-                                   self._device_module.device_type,
-                                   conf['name'])
+        self._eventer_client = eventer_client
+        self._event_type_prefix = event_type_prefix
+        self._async_group = async_group
+        self._create_device = create_device
+        self._events_queue_size = events_queue_size
+        self._events_queue = None
+        self._enable_event = asyncio.Event()
 
-        self.async_group.spawn(self._read_loop)
-        self.async_group.spawn(self._device_loop)
+        self.async_group.spawn(self._run)
 
     @property
-    def async_group(self):
-        return self._client.async_group
+    def async_group(self) -> aio.Group:
+        return self._async_group
 
-    @property
-    def event_type_prefix(self):
-        return self._event_type_prefix
+    def set_enable(self, enable: bool):
+        if enable:
+            if self._events_queue is not None:
+                return
 
-    @property
-    def receive_queue(self):
-        return self._receive_queue
+            self._events_queue = aio.Queue(self._events_queue_size)
+            self._enable_event.set()
 
-    async def _read_loop(self):
-        try:
-            events = collections.deque()
-            enabled = False
+        else:
+            if self._events_queue is None:
+                return
 
+            self._events_queue.close()
+            self._events_queue = None
+            self._enable_event.set()
+
+    async def process_events(self, events: Collection[hat.event.common.Event]):
+        if self._events_queue is None:
+            mlog.warning("device not enabled - ignoring %s events",
+                         len(events))
+            return
+
+        await self._events_queue.put(events)
+
+    async def _run(self):
+        try:
             while True:
-                while True:
-                    while events and not enabled:
-                        event = events.popleft()
-                        if event.event_type[5:] == ('enable', ):
-                            enabled = _is_enable_event(event)
+                self._enable_event.clear()
 
-                    if enabled:
-                        break
+                if self._events_queue is None:
+                    await self._enable_event.wait()
+                    continue
 
-                    events = await self._receive_queue.get()
+                events_queue = self._events_queue
+                device = await aio.call(self._create_device, self._conf,
+                                        self._eventer_client,
+                                        self._event_type_prefix)
 
-                events_queue = aio.Queue()
                 try:
-                    self._events_queues_queue.put_nowait(events_queue)
+                    device.async_group.spawn(aio.call_on_cancel,
+                                             events_queue.close)
+                    await self._register_running(True)
 
                     while True:
-                        filtered_events = collections.deque()
+                        events = await events_queue.get()
 
-                        while events and enabled:
-                            event = events.popleft()
-                            if event.event_type[5:] == ('enable', ):
-                                enabled = _is_enable_event(event)
-                            else:
-                                filtered_events.append(event)
+                        if not device.is_open:
+                            raise Exception('device closed')
 
-                        if filtered_events and not events_queue.is_closed:
-                            events_queue.put_nowait(list(filtered_events))
+                        await aio.call(device.process_events, events)
 
-                        if not enabled:
-                            break
+                except aio.QueueClosedError:
+                    if not events_queue.is_closed:
+                        raise
 
-                        events = await self._receive_queue.get()
+                    if not device.is_open:
+                        raise Exception('device closed')
 
                 finally:
-                    events_queue.close()
+                    await aio.uncancellable(self._close_device(device))
 
         except Exception as e:
-            mlog.error('read loop error: %s', e, exc_info=e)
+            mlog.error("device proxy run error: %s", e, exc_info=e)
 
         finally:
             self.close()
 
-    async def _device_loop(self):
-        try:
-            self._register_running(False)
-            while True:
-                events_queue = await self._events_queues_queue.get()
-                if events_queue.is_closed:
-                    continue
-
-                async with self.async_group.create_subgroup() as subgroup:
-                    client = _DeviceEventClient(self._client)
-                    device = await aio.call(self._device_module.create,
-                                            self._conf, client,
-                                            self._event_type_prefix)
-
-                    subgroup.spawn(aio.call_on_cancel, device.async_close)
-                    subgroup.spawn(aio.call_on_cancel, events_queue.close)
-                    subgroup.spawn(aio.call_on_done, device.wait_closing(),
-                                   subgroup.close)
-
-                    try:
-                        self._register_running(True)
-                        while True:
-                            events = await events_queue.get()
-                            client.receive_queue.put_nowait(events)
-
-                    except aio.QueueClosedError:
-                        if not device.is_open:
-                            break
-
-                    finally:
-                        self._register_running(False)
-
-        except Exception as e:
-            mlog.error('device loop error: %s', e, exc_info=e)
-
-        finally:
-            self.close()
-
-    def _register_running(self, is_running):
-        self._client.register([hat.event.common.RegisterEvent(
-            event_type=(*self._event_type_prefix, 'gateway', 'running'),
-            source_timestamp=hat.event.common.now(),
-            payload=hat.event.common.EventPayload(
-                type=hat.event.common.EventPayloadType.JSON,
-                data=is_running))])
-
-
-class _DeviceEventClient(common.DeviceEventClient):
-
-    def __init__(self, client):
-        self._client = client
-        self._receive_queue = aio.Queue()
-
-        self.async_group.spawn(aio.call_on_cancel, self._receive_queue.close)
-
-    @property
-    def async_group(self):
-        return self._client.async_group
-
-    @property
-    def receive_queue(self):
-        return self._receive_queue
-
-    async def receive(self):
-        try:
-            return await self._receive_queue.get()
-
-        except aio.QueueClosedError:
-            raise ConnectionError()
-
-    def register(self, events):
-        self._client.register(events)
-
-    async def register_with_response(self, events):
-        return await self._client.register_with_response(events)
-
-    async def query(self, data):
-        return await self._client.query(data)
+    async def _close_device(self, device):
+        await device.async_close()
 
+        with contextlib.suppress(ConnectionError):
+            await self._register_running(False)
 
-def _is_enable_event(event):
-    return (event.payload and
-            event.payload.type == hat.event.common.EventPayloadType.JSON and
-            event.payload.data is True)
+    async def _register_running(self, is_running):
+        await self._eventer_client.register([
+            hat.event.common.RegisterEvent(
+                type=(*self._event_type_prefix, 'gateway', 'running'),
+                source_timestamp=hat.event.common.now(),
+                payload=hat.event.common.EventPayloadJson(is_running))])
```

## hat/gateway/json_schema_repo.json

### Pretty-printed

 * *Similarity: 0.6304910447862413%*

 * *Differences: {"'hat-gateway'": "{'modbus.yaml': {'definitions': {'master': {'properties': {'connection': "*

 * *                  "{'required': {insert: [(5, 'request_delay'), (6, "*

 * *                  "'request_retry_immediate_count'), (7, 'request_retry_delayed_count')], delete: "*

 * *                  "[5]}, 'properties': {'request_retry_delay': {'description': 'Delay (in seconds) "*

 * *                  "between two consecutive delayed\\nrequest retries\\n'}, 'request_delay': "*

 * *                  "OrderedDict([('type', 'number'), ( […]*

```diff
@@ -1,76 +1,1874 @@
 {
     "hat-gateway": {
-        "main.yaml": {
-            "$schema": "http://json-schema.org/draft-07/schema#",
-            "allOf": [
-                {
+        "iec101.yaml": {
+            "definitions": {
+                "causes": {
+                    "command": {
+                        "req": {
+                            "oneOf": [
+                                {
+                                    "enum": [
+                                        "ACTIVATION",
+                                        "DEACTIVATION"
+                                    ]
+                                },
+                                {
+                                    "description": "other cause in range [0, 63]\n",
+                                    "type": "integer"
+                                }
+                            ]
+                        },
+                        "res": {
+                            "oneOf": [
+                                {
+                                    "enum": [
+                                        "ACTIVATION_CONFIRMATION",
+                                        "DEACTIVATION_CONFIRMATION",
+                                        "ACTIVATION_TERMINATION",
+                                        "UNKNOWN_TYPE",
+                                        "UNKNOWN_CAUSE",
+                                        "UNKNOWN_ASDU_ADDRESS",
+                                        "UNKNOWN_IO_ADDRESS"
+                                    ]
+                                },
+                                {
+                                    "description": "other cause in range [0, 63]\n",
+                                    "type": "integer"
+                                }
+                            ]
+                        }
+                    },
+                    "data": {
+                        "res": {
+                            "oneOf": [
+                                {
+                                    "enum": [
+                                        "PERIODIC",
+                                        "BACKGROUND_SCAN",
+                                        "SPONTANEOUS",
+                                        "REQUEST",
+                                        "REMOTE_COMMAND",
+                                        "LOCAL_COMMAND",
+                                        "INTERROGATED"
+                                    ]
+                                },
+                                {
+                                    "description": "other cause in range [0, 63]\n",
+                                    "type": "integer"
+                                }
+                            ]
+                        }
+                    }
+                },
+                "commands": {
+                    "bitstring": {
+                        "properties": {
+                            "value": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/values/bitstring"
+                            }
+                        },
+                        "required": [
+                            "value"
+                        ],
+                        "type": "object"
+                    },
+                    "double": {
+                        "properties": {
+                            "qualifier": {
+                                "description": "qualifier in range [0, 31]\n",
+                                "type": "integer"
+                            },
+                            "select": {
+                                "type": "boolean"
+                            },
+                            "value": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/values/double"
+                            }
+                        },
+                        "required": [
+                            "value",
+                            "select",
+                            "qualifier"
+                        ],
+                        "type": "object"
+                    },
+                    "floating": {
+                        "properties": {
+                            "select": {
+                                "type": "boolean"
+                            },
+                            "value": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/values/floating"
+                            }
+                        },
+                        "required": [
+                            "value",
+                            "select"
+                        ],
+                        "type": "object"
+                    },
+                    "normalized": {
+                        "properties": {
+                            "select": {
+                                "type": "boolean"
+                            },
+                            "value": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/values/normalized"
+                            }
+                        },
+                        "required": [
+                            "value",
+                            "select"
+                        ],
+                        "type": "object"
+                    },
+                    "regulating": {
+                        "properties": {
+                            "qualifier": {
+                                "description": "qualifier in range [0, 31]\n",
+                                "type": "integer"
+                            },
+                            "select": {
+                                "type": "boolean"
+                            },
+                            "value": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/values/regulating"
+                            }
+                        },
+                        "required": [
+                            "value",
+                            "select",
+                            "qualifier"
+                        ],
+                        "type": "object"
+                    },
+                    "scaled": {
+                        "properties": {
+                            "select": {
+                                "type": "boolean"
+                            },
+                            "value": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/values/scaled"
+                            }
+                        },
+                        "required": [
+                            "value",
+                            "select"
+                        ],
+                        "type": "object"
+                    },
+                    "single": {
+                        "properties": {
+                            "qualifier": {
+                                "description": "qualifier in range [0, 31]\n",
+                                "type": "integer"
+                            },
+                            "select": {
+                                "type": "boolean"
+                            },
+                            "value": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/values/single"
+                            }
+                        },
+                        "required": [
+                            "value",
+                            "select",
+                            "qualifier"
+                        ],
+                        "type": "object"
+                    }
+                },
+                "data": {
+                    "binary_counter": {
+                        "properties": {
+                            "quality": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/qualities/counter"
+                            },
+                            "value": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/values/binary_counter"
+                            }
+                        },
+                        "required": [
+                            "value",
+                            "quality"
+                        ],
+                        "type": "object"
+                    },
+                    "bitstring": {
+                        "properties": {
+                            "quality": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/qualities/measurement"
+                            },
+                            "value": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/values/bitstring"
+                            }
+                        },
+                        "required": [
+                            "value",
+                            "quality"
+                        ],
+                        "type": "object"
+                    },
+                    "double": {
+                        "properties": {
+                            "quality": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/qualities/indication"
+                            },
+                            "value": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/values/double"
+                            }
+                        },
+                        "required": [
+                            "value",
+                            "quality"
+                        ],
+                        "type": "object"
+                    },
+                    "floating": {
+                        "properties": {
+                            "quality": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/qualities/measurement"
+                            },
+                            "value": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/values/floating"
+                            }
+                        },
+                        "required": [
+                            "value",
+                            "quality"
+                        ],
+                        "type": "object"
+                    },
+                    "normalized": {
+                        "properties": {
+                            "quality": {
+                                "oneOf": [
+                                    {
+                                        "type": "null"
+                                    },
+                                    {
+                                        "$ref": "hat-gateway://iec101.yaml#/definitions/qualities/measurement"
+                                    }
+                                ]
+                            },
+                            "value": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/values/normalized"
+                            }
+                        },
+                        "required": [
+                            "value",
+                            "quality"
+                        ],
+                        "type": "object"
+                    },
+                    "protection": {
+                        "properties": {
+                            "elapsed_time": {
+                                "description": "elapsed_time in range [0, 65535]\n",
+                                "type": "integer"
+                            },
+                            "quality": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/qualities/protection"
+                            },
+                            "value": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/values/protection"
+                            }
+                        },
+                        "required": [
+                            "value",
+                            "quality",
+                            "elapsed_time"
+                        ],
+                        "type": "object"
+                    },
+                    "protection_command": {
+                        "properties": {
+                            "operating_time": {
+                                "description": "operating_time in range [0, 65535]\n",
+                                "type": "integer"
+                            },
+                            "quality": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/qualities/protection"
+                            },
+                            "value": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/values/protection_command"
+                            }
+                        },
+                        "required": [
+                            "value",
+                            "quality",
+                            "operating_time"
+                        ],
+                        "type": "object"
+                    },
+                    "protection_start": {
+                        "properties": {
+                            "duration_time": {
+                                "description": "duration_time in range [0, 65535]\n",
+                                "type": "integer"
+                            },
+                            "quality": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/qualities/protection"
+                            },
+                            "value": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/values/protection_start"
+                            }
+                        },
+                        "required": [
+                            "value",
+                            "quality",
+                            "duration_time"
+                        ],
+                        "type": "object"
+                    },
+                    "scaled": {
+                        "properties": {
+                            "quality": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/qualities/measurement"
+                            },
+                            "value": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/values/scaled"
+                            }
+                        },
+                        "required": [
+                            "value",
+                            "quality"
+                        ],
+                        "type": "object"
+                    },
+                    "single": {
+                        "properties": {
+                            "quality": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/qualities/indication"
+                            },
+                            "value": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/values/single"
+                            }
+                        },
+                        "required": [
+                            "value",
+                            "quality"
+                        ],
+                        "type": "object"
+                    },
+                    "status": {
+                        "properties": {
+                            "quality": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/qualities/measurement"
+                            },
+                            "value": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/values/status"
+                            }
+                        },
+                        "required": [
+                            "value",
+                            "quality"
+                        ],
+                        "type": "object"
+                    },
+                    "step_position": {
+                        "properties": {
+                            "quality": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/qualities/measurement"
+                            },
+                            "value": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/values/step_position"
+                            }
+                        },
+                        "required": [
+                            "value",
+                            "quality"
+                        ],
+                        "type": "object"
+                    }
+                },
+                "events": {
+                    "master": {
+                        "gateway": {
+                            "command": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/messages/command/res"
+                            },
+                            "counter_interrogation": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/messages/counter_interrogation/res"
+                            },
+                            "data": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/messages/data/res"
+                            },
+                            "interrogation": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/messages/interrogation/res"
+                            },
+                            "status": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/messages/status"
+                            }
+                        },
+                        "system": {
+                            "command": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/messages/command/req"
+                            },
+                            "counter_interrogation": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/messages/counter_interrogation/req"
+                            },
+                            "enable": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/messages/enable"
+                            },
+                            "interrogation": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/messages/interrogation/req"
+                            }
+                        }
+                    },
+                    "slave": {
+                        "gateway": {
+                            "command": {
+                                "allOf": [
+                                    {
+                                        "properties": {
+                                            "connection_id": {
+                                                "type": "integer"
+                                            }
+                                        },
+                                        "required": [
+                                            "connection_id"
+                                        ],
+                                        "type": "object"
+                                    },
+                                    {
+                                        "$ref": "hat-gateway://iec101.yaml#/definitions/messages/command/req"
+                                    }
+                                ]
+                            },
+                            "connections": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/messages/connections"
+                            }
+                        },
+                        "system": {
+                            "command": {
+                                "allOf": [
+                                    {
+                                        "properties": {
+                                            "connection_id": {
+                                                "type": "integer"
+                                            }
+                                        },
+                                        "required": [
+                                            "connection_id"
+                                        ],
+                                        "type": "object"
+                                    },
+                                    {
+                                        "$ref": "hat-gateway://iec101.yaml#/definitions/messages/command/res"
+                                    }
+                                ]
+                            },
+                            "data": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/messages/data/res"
+                            }
+                        }
+                    }
+                },
+                "master": {
                     "properties": {
-                        "devices": {
+                        "asdu_address_size": {
+                            "enum": [
+                                "ONE",
+                                "TWO"
+                            ]
+                        },
+                        "baudrate": {
+                            "type": "integer"
+                        },
+                        "bytesize": {
+                            "enum": [
+                                "FIVEBITS",
+                                "SIXBITS",
+                                "SEVENBITS",
+                                "EIGHTBITS"
+                            ]
+                        },
+                        "cause_size": {
+                            "enum": [
+                                "ONE",
+                                "TWO"
+                            ]
+                        },
+                        "device_address_size": {
+                            "enum": [
+                                "ONE",
+                                "TWO"
+                            ]
+                        },
+                        "flow_control": {
+                            "properties": {
+                                "dsrdtr": {
+                                    "type": "boolean"
+                                },
+                                "rtscts": {
+                                    "type": "boolean"
+                                },
+                                "xonxoff": {
+                                    "type": "boolean"
+                                }
+                            },
+                            "required": [
+                                "xonxoff",
+                                "rtscts",
+                                "dsrdtr"
+                            ],
+                            "type": "object"
+                        },
+                        "io_address_size": {
+                            "enum": [
+                                "ONE",
+                                "TWO",
+                                "THREE"
+                            ]
+                        },
+                        "parity": {
+                            "enum": [
+                                "NONE",
+                                "EVEN",
+                                "ODD",
+                                "MARK",
+                                "SPACE"
+                            ]
+                        },
+                        "port": {
+                            "type": "string"
+                        },
+                        "reconnect_delay": {
+                            "type": "number"
+                        },
+                        "remote_devices": {
                             "items": {
-                                "$ref": "hat-gateway://main.yaml#/definitions/device"
+                                "properties": {
+                                    "address": {
+                                        "type": "integer"
+                                    },
+                                    "poll_class1_delay": {
+                                        "type": [
+                                            "null",
+                                            "number"
+                                        ]
+                                    },
+                                    "poll_class2_delay": {
+                                        "type": [
+                                            "null",
+                                            "number"
+                                        ]
+                                    },
+                                    "reconnect_delay": {
+                                        "type": "number"
+                                    },
+                                    "response_timeout": {
+                                        "type": "number"
+                                    },
+                                    "send_retry_count": {
+                                        "type": "integer"
+                                    },
+                                    "time_sync_delay": {
+                                        "type": [
+                                            "null",
+                                            "number"
+                                        ]
+                                    }
+                                },
+                                "required": [
+                                    "address",
+                                    "response_timeout",
+                                    "send_retry_count",
+                                    "poll_class1_delay",
+                                    "poll_class2_delay",
+                                    "reconnect_delay",
+                                    "time_sync_delay"
+                                ],
+                                "type": "object"
                             },
                             "type": "array"
                         },
-                        "gateway_name": {
-                            "type": "string"
+                        "silent_interval": {
+                            "type": "number"
                         },
-                        "log": {
-                            "$ref": "hat-json://logging.yaml#"
+                        "stopbits": {
+                            "enum": [
+                                "ONE",
+                                "ONE_POINT_FIVE",
+                                "TWO"
+                            ]
+                        }
+                    },
+                    "required": [
+                        "port",
+                        "baudrate",
+                        "bytesize",
+                        "parity",
+                        "stopbits",
+                        "flow_control",
+                        "silent_interval",
+                        "device_address_size",
+                        "cause_size",
+                        "asdu_address_size",
+                        "io_address_size",
+                        "reconnect_delay",
+                        "remote_devices"
+                    ],
+                    "type": "object"
+                },
+                "messages": {
+                    "command": {
+                        "req": {
+                            "properties": {
+                                "cause": {
+                                    "$ref": "hat-gateway://iec101.yaml#/definitions/causes/command/req"
+                                },
+                                "command": {
+                                    "oneOf": [
+                                        {
+                                            "$ref": "hat-gateway://iec101.yaml#/definitions/commands/single"
+                                        },
+                                        {
+                                            "$ref": "hat-gateway://iec101.yaml#/definitions/commands/double"
+                                        },
+                                        {
+                                            "$ref": "hat-gateway://iec101.yaml#/definitions/commands/regulating"
+                                        },
+                                        {
+                                            "$ref": "hat-gateway://iec101.yaml#/definitions/commands/normalized"
+                                        },
+                                        {
+                                            "$ref": "hat-gateway://iec101.yaml#/definitions/commands/scaled"
+                                        },
+                                        {
+                                            "$ref": "hat-gateway://iec101.yaml#/definitions/commands/floating"
+                                        },
+                                        {
+                                            "$ref": "hat-gateway://iec101.yaml#/definitions/commands/bitstring"
+                                        }
+                                    ]
+                                },
+                                "is_test": {
+                                    "type": "boolean"
+                                }
+                            },
+                            "required": [
+                                "is_test",
+                                "cause",
+                                "command"
+                            ],
+                            "type": "object"
                         },
-                        "type": {
-                            "description": "configuration type identification",
+                        "res": {
+                            "properties": {
+                                "cause": {
+                                    "$ref": "hat-gateway://iec101.yaml#/definitions/causes/command/res"
+                                },
+                                "command": {
+                                    "oneOf": [
+                                        {
+                                            "$ref": "hat-gateway://iec101.yaml#/definitions/commands/single"
+                                        },
+                                        {
+                                            "$ref": "hat-gateway://iec101.yaml#/definitions/commands/double"
+                                        },
+                                        {
+                                            "$ref": "hat-gateway://iec101.yaml#/definitions/commands/regulating"
+                                        },
+                                        {
+                                            "$ref": "hat-gateway://iec101.yaml#/definitions/commands/normalized"
+                                        },
+                                        {
+                                            "$ref": "hat-gateway://iec101.yaml#/definitions/commands/scaled"
+                                        },
+                                        {
+                                            "$ref": "hat-gateway://iec101.yaml#/definitions/commands/floating"
+                                        },
+                                        {
+                                            "$ref": "hat-gateway://iec101.yaml#/definitions/commands/bitstring"
+                                        }
+                                    ]
+                                },
+                                "is_negative_confirm": {
+                                    "type": "boolean"
+                                },
+                                "is_test": {
+                                    "type": "boolean"
+                                }
+                            },
+                            "required": [
+                                "is_test",
+                                "is_negative_confirm",
+                                "cause",
+                                "command"
+                            ],
+                            "type": "object"
+                        }
+                    },
+                    "connections": {
+                        "items": {
+                            "properties": {
+                                "address": {
+                                    "type": "integer"
+                                },
+                                "connection_id": {
+                                    "type": "integer"
+                                }
+                            },
+                            "required": [
+                                "connection_id",
+                                "address"
+                            ],
+                            "type": "object"
+                        },
+                        "type": "array"
+                    },
+                    "counter_interrogation": {
+                        "req": {
+                            "allOf": [
+                                {
+                                    "properties": {
+                                        "freeze": {
+                                            "enum": [
+                                                "READ",
+                                                "FREEZE",
+                                                "FREEZE_AND_RESET",
+                                                "RESET"
+                                            ]
+                                        }
+                                    },
+                                    "required": [
+                                        "freeze"
+                                    ],
+                                    "type": "object"
+                                },
+                                {
+                                    "$ref": "hat-gateway://iec101.yaml#/definitions/messages/interrogation/req"
+                                }
+                            ]
+                        },
+                        "res": {
+                            "allOf": [
+                                {
+                                    "properties": {
+                                        "freeze": {
+                                            "enum": [
+                                                "READ",
+                                                "FREEZE",
+                                                "FREEZE_AND_RESET",
+                                                "RESET"
+                                            ]
+                                        }
+                                    },
+                                    "required": [
+                                        "freeze"
+                                    ],
+                                    "type": "object"
+                                },
+                                {
+                                    "$ref": "hat-gateway://iec101.yaml#/definitions/messages/interrogation/res"
+                                }
+                            ]
+                        }
+                    },
+                    "data": {
+                        "res": {
+                            "properties": {
+                                "cause": {
+                                    "$ref": "hat-gateway://iec101.yaml#/definitions/causes/data/res"
+                                },
+                                "data": {
+                                    "oneOf": [
+                                        {
+                                            "$ref": "hat-gateway://iec101.yaml#/definitions/data/single"
+                                        },
+                                        {
+                                            "$ref": "hat-gateway://iec101.yaml#/definitions/data/double"
+                                        },
+                                        {
+                                            "$ref": "hat-gateway://iec101.yaml#/definitions/data/step_position"
+                                        },
+                                        {
+                                            "$ref": "hat-gateway://iec101.yaml#/definitions/data/bitstring"
+                                        },
+                                        {
+                                            "$ref": "hat-gateway://iec101.yaml#/definitions/data/normalized"
+                                        },
+                                        {
+                                            "$ref": "hat-gateway://iec101.yaml#/definitions/data/scaled"
+                                        },
+                                        {
+                                            "$ref": "hat-gateway://iec101.yaml#/definitions/data/floating"
+                                        },
+                                        {
+                                            "$ref": "hat-gateway://iec101.yaml#/definitions/data/binary_counter"
+                                        },
+                                        {
+                                            "$ref": "hat-gateway://iec101.yaml#/definitions/data/protection"
+                                        },
+                                        {
+                                            "$ref": "hat-gateway://iec101.yaml#/definitions/data/protection_start"
+                                        },
+                                        {
+                                            "$ref": "hat-gateway://iec101.yaml#/definitions/data/protection_command"
+                                        },
+                                        {
+                                            "$ref": "hat-gateway://iec101.yaml#/definitions/data/status"
+                                        }
+                                    ]
+                                },
+                                "is_test": {
+                                    "type": "boolean"
+                                }
+                            },
+                            "required": [
+                                "is_test",
+                                "cause",
+                                "data"
+                            ],
+                            "type": "object"
+                        }
+                    },
+                    "enable": {
+                        "type": "boolean"
+                    },
+                    "interrogation": {
+                        "req": {
+                            "properties": {
+                                "cause": {
+                                    "$ref": "hat-gateway://iec101.yaml#/definitions/causes/command/req"
+                                },
+                                "is_test": {
+                                    "type": "boolean"
+                                },
+                                "request": {
+                                    "description": "request in range [0, 255]\n",
+                                    "type": "integer"
+                                }
+                            },
+                            "required": [
+                                "is_test",
+                                "request",
+                                "cause"
+                            ],
+                            "type": "object"
+                        },
+                        "res": {
+                            "properties": {
+                                "cause": {
+                                    "$ref": "hat-gateway://iec101.yaml#/definitions/causes/command/res"
+                                },
+                                "is_negative_confirm": {
+                                    "type": "boolean"
+                                },
+                                "is_test": {
+                                    "type": "boolean"
+                                },
+                                "request": {
+                                    "description": "request in range [0, 255]\n",
+                                    "type": "integer"
+                                }
+                            },
+                            "required": [
+                                "is_test",
+                                "is_negative_confirm",
+                                "request",
+                                "cause"
+                            ],
+                            "type": "object"
+                        }
+                    },
+                    "status": {
+                        "enum": [
+                            "CONNECTING",
+                            "CONNECTED",
+                            "DISCONNECTED"
+                        ]
+                    }
+                },
+                "qualities": {
+                    "counter": {
+                        "properties": {
+                            "adjusted": {
+                                "type": "boolean"
+                            },
+                            "invalid": {
+                                "type": "boolean"
+                            },
+                            "overflow": {
+                                "type": "boolean"
+                            },
+                            "sequence": {
+                                "type": "boolean"
+                            }
+                        },
+                        "required": [
+                            "invalid",
+                            "adjusted",
+                            "overflow",
+                            "sequence"
+                        ],
+                        "type": "object"
+                    },
+                    "indication": {
+                        "properties": {
+                            "blocked": {
+                                "type": "boolean"
+                            },
+                            "invalid": {
+                                "type": "boolean"
+                            },
+                            "not_topical": {
+                                "type": "boolean"
+                            },
+                            "substituted": {
+                                "type": "boolean"
+                            }
+                        },
+                        "required": [
+                            "invalid",
+                            "not_topical",
+                            "substituted",
+                            "blocked"
+                        ],
+                        "type": "object"
+                    },
+                    "measurement": {
+                        "properties": {
+                            "blocked": {
+                                "type": "boolean"
+                            },
+                            "invalid": {
+                                "type": "boolean"
+                            },
+                            "not_topical": {
+                                "type": "boolean"
+                            },
+                            "overflow": {
+                                "type": "boolean"
+                            },
+                            "substituted": {
+                                "type": "boolean"
+                            }
+                        },
+                        "required": [
+                            "invalid",
+                            "not_topical",
+                            "substituted",
+                            "blocked",
+                            "overflow"
+                        ],
+                        "type": "object"
+                    },
+                    "protection": {
+                        "properties": {
+                            "blocked": {
+                                "type": "boolean"
+                            },
+                            "invalid": {
+                                "type": "boolean"
+                            },
+                            "not_topical": {
+                                "type": "boolean"
+                            },
+                            "substituted": {
+                                "type": "boolean"
+                            },
+                            "time_invalid": {
+                                "type": "boolean"
+                            }
+                        },
+                        "required": [
+                            "invalid",
+                            "not_topical",
+                            "substituted",
+                            "blocked",
+                            "time_invalid"
+                        ],
+                        "type": "object"
+                    }
+                },
+                "slave": {
+                    "properties": {
+                        "addresses": {
+                            "items": {
+                                "type": "integer"
+                            },
+                            "type": "array"
+                        },
+                        "asdu_address_size": {
+                            "enum": [
+                                "ONE",
+                                "TWO"
+                            ]
+                        },
+                        "baudrate": {
+                            "type": "integer"
+                        },
+                        "buffers": {
+                            "items": {
+                                "properties": {
+                                    "name": {
+                                        "type": "string"
+                                    },
+                                    "size": {
+                                        "type": "integer"
+                                    }
+                                },
+                                "required": [
+                                    "name",
+                                    "size"
+                                ],
+                                "type": "object"
+                            },
+                            "type": "array"
+                        },
+                        "bytesize": {
+                            "enum": [
+                                "FIVEBITS",
+                                "SIXBITS",
+                                "SEVENBITS",
+                                "EIGHTBITS"
+                            ]
+                        },
+                        "cause_size": {
+                            "enum": [
+                                "ONE",
+                                "TWO"
+                            ]
+                        },
+                        "data": {
+                            "items": {
+                                "properties": {
+                                    "asdu_address": {
+                                        "type": "integer"
+                                    },
+                                    "buffer": {
+                                        "type": [
+                                            "null",
+                                            "string"
+                                        ]
+                                    },
+                                    "data_type": {
+                                        "enum": [
+                                            "SINGLE",
+                                            "DOUBLE",
+                                            "STEP_POSITION",
+                                            "BITSTRING",
+                                            "NORMALIZED",
+                                            "SCALED",
+                                            "FLOATING",
+                                            "BINARY_COUNTER",
+                                            "PROTECTION",
+                                            "PROTECTION_START",
+                                            "PROTECTION_COMMAND",
+                                            "STATUS"
+                                        ]
+                                    },
+                                    "io_address": {
+                                        "type": "integer"
+                                    }
+                                },
+                                "required": [
+                                    "data_type",
+                                    "asdu_address",
+                                    "io_address",
+                                    "buffer"
+                                ],
+                                "type": "object"
+                            },
+                            "type": "array"
+                        },
+                        "device_address_size": {
+                            "enum": [
+                                "ONE",
+                                "TWO"
+                            ]
+                        },
+                        "flow_control": {
+                            "properties": {
+                                "dsrdtr": {
+                                    "type": "boolean"
+                                },
+                                "rtscts": {
+                                    "type": "boolean"
+                                },
+                                "xonxoff": {
+                                    "type": "boolean"
+                                }
+                            },
+                            "required": [
+                                "xonxoff",
+                                "rtscts",
+                                "dsrdtr"
+                            ],
+                            "type": "object"
+                        },
+                        "io_address_size": {
                             "enum": [
-                                "gateway"
+                                "ONE",
+                                "TWO",
+                                "THREE"
                             ]
                         },
-                        "version": {
-                            "description": "component version",
+                        "keep_alive_timeout": {
+                            "type": "number"
+                        },
+                        "parity": {
+                            "enum": [
+                                "NONE",
+                                "EVEN",
+                                "ODD",
+                                "MARK",
+                                "SPACE"
+                            ]
+                        },
+                        "port": {
                             "type": "string"
+                        },
+                        "silent_interval": {
+                            "type": "number"
+                        },
+                        "stopbits": {
+                            "enum": [
+                                "ONE",
+                                "ONE_POINT_FIVE",
+                                "TWO"
+                            ]
                         }
                     },
                     "required": [
-                        "type",
-                        "log",
-                        "gateway_name",
-                        "devices"
+                        "port",
+                        "addresses",
+                        "baudrate",
+                        "bytesize",
+                        "parity",
+                        "stopbits",
+                        "flow_control",
+                        "silent_interval",
+                        "device_address_size",
+                        "keep_alive_timeout",
+                        "cause_size",
+                        "asdu_address_size",
+                        "io_address_size",
+                        "buffers",
+                        "data"
                     ],
                     "type": "object"
                 },
-                {
-                    "oneOf": [
-                        {
+                "values": {
+                    "binary_counter": {
+                        "description": "value in range [-2^31, 2^31-1]\n",
+                        "type": "integer"
+                    },
+                    "bitstring": {
+                        "description": "bitstring encoded as 4 bytes\n",
+                        "items": {
+                            "type": "integer"
+                        },
+                        "type": "array"
+                    },
+                    "double": {
+                        "enum": [
+                            "INTERMEDIATE",
+                            "OFF",
+                            "ON",
+                            "FAULT"
+                        ]
+                    },
+                    "floating": {
+                        "type": "number"
+                    },
+                    "normalized": {
+                        "description": "value in range [-1.0, 1.0)\n",
+                        "type": "number"
+                    },
+                    "protection": {
+                        "enum": [
+                            "OFF",
+                            "ON"
+                        ]
+                    },
+                    "protection_command": {
+                        "properties": {
+                            "general": {
+                                "type": "boolean"
+                            },
+                            "l1": {
+                                "type": "boolean"
+                            },
+                            "l2": {
+                                "type": "boolean"
+                            },
+                            "l3": {
+                                "type": "boolean"
+                            }
+                        },
+                        "required": [
+                            "general",
+                            "l1",
+                            "l2",
+                            "l3"
+                        ],
+                        "type": "object"
+                    },
+                    "protection_start": {
+                        "properties": {
+                            "general": {
+                                "type": "boolean"
+                            },
+                            "ie": {
+                                "type": "boolean"
+                            },
+                            "l1": {
+                                "type": "boolean"
+                            },
+                            "l2": {
+                                "type": "boolean"
+                            },
+                            "l3": {
+                                "type": "boolean"
+                            },
+                            "reverse": {
+                                "type": "boolean"
+                            }
+                        },
+                        "required": [
+                            "general",
+                            "l1",
+                            "l2",
+                            "l3",
+                            "ie",
+                            "reverse"
+                        ],
+                        "type": "object"
+                    },
+                    "regulating": {
+                        "enum": [
+                            "LOWER",
+                            "HIGHER"
+                        ]
+                    },
+                    "scaled": {
+                        "description": "value in range [-2^15, 2^15-1]\n",
+                        "type": "integer"
+                    },
+                    "single": {
+                        "enum": [
+                            "OFF",
+                            "ON"
+                        ]
+                    },
+                    "status": {
+                        "properties": {
+                            "change": {
+                                "description": "change length is 16\n",
+                                "items": {
+                                    "type": "boolean"
+                                },
+                                "type": "array"
+                            },
+                            "value": {
+                                "description": "value length is 16\n",
+                                "items": {
+                                    "type": "boolean"
+                                },
+                                "type": "array"
+                            }
+                        },
+                        "required": [
+                            "value",
+                            "change"
+                        ],
+                        "type": "object"
+                    },
+                    "step_position": {
+                        "properties": {
+                            "transient": {
+                                "type": "boolean"
+                            },
+                            "value": {
+                                "description": "value in range [-64, 63]\n",
+                                "type": "integer"
+                            }
+                        },
+                        "required": [
+                            "value",
+                            "transient"
+                        ],
+                        "type": "object"
+                    }
+                }
+            },
+            "id": "hat-gateway://iec101.yaml#"
+        },
+        "iec103.yaml": {
+            "definitions": {
+                "events": {
+                    "master": {
+                        "gateway": {
+                            "command": {
+                                "properties": {
+                                    "success": {
+                                        "type": "boolean"
+                                    }
+                                },
+                                "required": [
+                                    "session_id",
+                                    "success"
+                                ],
+                                "type": "object"
+                            },
+                            "data": {
+                                "properties": {
+                                    "cause": {
+                                        "oneOf": [
+                                            {
+                                                "enum": [
+                                                    "SPONTANEOUS",
+                                                    "CYCLIC",
+                                                    "TEST_MODE",
+                                                    "GENERAL_INTERROGATION",
+                                                    "LOCAL_OPERATION",
+                                                    "REMOTE_OPERATION"
+                                                ]
+                                            },
+                                            {
+                                                "description": "other cause in range [0, 255]\n",
+                                                "type": "integer"
+                                            }
+                                        ]
+                                    },
+                                    "value": {
+                                        "oneOf": [
+                                            {
+                                                "$ref": "hat-gateway://iec103.yaml#/definitions/values/double"
+                                            },
+                                            {
+                                                "$ref": "hat-gateway://iec103.yaml#/definitions/values/measurand"
+                                            }
+                                        ]
+                                    }
+                                },
+                                "required": [
+                                    "cause",
+                                    "value"
+                                ],
+                                "type": "object"
+                            },
+                            "status": {
+                                "enum": [
+                                    "CONNECTING",
+                                    "CONNECTED",
+                                    "DISCONNECTED"
+                                ]
+                            }
+                        },
+                        "system": {
+                            "command": {
+                                "properties": {
+                                    "value": {
+                                        "$ref": "hat-gateway://iec103.yaml#/definitions/values/double"
+                                    }
+                                },
+                                "required": [
+                                    "session_id",
+                                    "value"
+                                ],
+                                "type": "object"
+                            },
+                            "enable": {
+                                "type": "boolean"
+                            }
+                        }
+                    }
+                },
+                "master": {
+                    "properties": {
+                        "baudrate": {
+                            "type": "integer"
+                        },
+                        "bytesize": {
+                            "enum": [
+                                "FIVEBITS",
+                                "SIXBITS",
+                                "SEVENBITS",
+                                "EIGHTBITS"
+                            ]
+                        },
+                        "flow_control": {
                             "properties": {
-                                "event_server_group": {
-                                    "type": "string"
+                                "dsrdtr": {
+                                    "type": "boolean"
+                                },
+                                "rtscts": {
+                                    "type": "boolean"
                                 },
-                                "monitor": {
-                                    "$ref": "hat-monitor://client.yaml#"
+                                "xonxoff": {
+                                    "type": "boolean"
                                 }
                             },
                             "required": [
-                                "monitor",
-                                "event_server_group"
+                                "xonxoff",
+                                "rtscts",
+                                "dsrdtr"
                             ],
                             "type": "object"
                         },
-                        {
+                        "parity": {
+                            "enum": [
+                                "NONE",
+                                "EVEN",
+                                "ODD",
+                                "MARK",
+                                "SPACE"
+                            ]
+                        },
+                        "port": {
+                            "type": "string"
+                        },
+                        "reconnect_delay": {
+                            "type": "number"
+                        },
+                        "remote_devices": {
+                            "items": {
+                                "properties": {
+                                    "address": {
+                                        "type": "integer"
+                                    },
+                                    "poll_class1_delay": {
+                                        "type": [
+                                            "null",
+                                            "number"
+                                        ]
+                                    },
+                                    "poll_class2_delay": {
+                                        "type": [
+                                            "null",
+                                            "number"
+                                        ]
+                                    },
+                                    "reconnect_delay": {
+                                        "type": "number"
+                                    },
+                                    "response_timeout": {
+                                        "type": "number"
+                                    },
+                                    "send_retry_count": {
+                                        "type": "integer"
+                                    },
+                                    "time_sync_delay": {
+                                        "type": [
+                                            "null",
+                                            "number"
+                                        ]
+                                    }
+                                },
+                                "required": [
+                                    "address",
+                                    "response_timeout",
+                                    "send_retry_count",
+                                    "poll_class1_delay",
+                                    "poll_class2_delay",
+                                    "reconnect_delay",
+                                    "time_sync_delay"
+                                ],
+                                "type": "object"
+                            },
+                            "type": "array"
+                        },
+                        "silent_interval": {
+                            "type": "number"
+                        },
+                        "stopbits": {
+                            "enum": [
+                                "ONE",
+                                "ONE_POINT_FIVE",
+                                "TWO"
+                            ]
+                        }
+                    },
+                    "required": [
+                        "port",
+                        "baudrate",
+                        "bytesize",
+                        "parity",
+                        "stopbits",
+                        "flow_control",
+                        "silent_interval",
+                        "reconnect_delay",
+                        "remote_devices"
+                    ],
+                    "type": "object"
+                },
+                "values": {
+                    "double": {
+                        "enum": [
+                            "TRANSIENT",
+                            "OFF",
+                            "ON",
+                            "ERROR"
+                        ]
+                    },
+                    "measurand": {
+                        "properties": {
+                            "invalid": {
+                                "type": "boolean"
+                            },
+                            "overflow": {
+                                "type": "boolean"
+                            },
+                            "value": {
+                                "type": "number"
+                            }
+                        },
+                        "required": [
+                            "overflow",
+                            "invalid",
+                            "value"
+                        ],
+                        "type": "object"
+                    }
+                }
+            },
+            "id": "hat-gateway://iec103.yaml#"
+        },
+        "iec104.yaml": {
+            "definitions": {
+                "events": {
+                    "master": {
+                        "gateway": {
+                            "command": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/events/master/gateway/command"
+                            },
+                            "counter_interrogation": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/events/master/gateway/counter_interrogation"
+                            },
+                            "data": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/events/master/gateway/data"
+                            },
+                            "interrogation": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/events/master/gateway/interrogation"
+                            },
+                            "status": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/events/master/gateway/status"
+                            }
+                        },
+                        "system": {
+                            "command": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/events/master/system/command"
+                            },
+                            "counter_interrogation": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/events/master/system/counter_interrogation"
+                            },
+                            "interrogation": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/events/master/system/interrogation"
+                            }
+                        }
+                    },
+                    "slave": {
+                        "gateway": {
+                            "command": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/events/slave/gateway/command"
+                            },
+                            "connections": {
+                                "$ref": "hat-gateway://iec104.yaml#/definitions/messages/connections"
+                            }
+                        },
+                        "system": {
+                            "command": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/events/slave/system/command"
+                            },
+                            "data": {
+                                "$ref": "hat-gateway://iec101.yaml#/definitions/events/slave/system/data"
+                            }
+                        }
+                    }
+                },
+                "master": {
+                    "properties": {
+                        "receive_window_size": {
+                            "type": "integer"
+                        },
+                        "reconnect_delay": {
+                            "type": "number"
+                        },
+                        "remote_addresses": {
+                            "items": {
+                                "properties": {
+                                    "host": {
+                                        "type": "string"
+                                    },
+                                    "port": {
+                                        "type": "integer"
+                                    }
+                                },
+                                "required": [
+                                    "host",
+                                    "port"
+                                ],
+                                "type": "object"
+                            },
+                            "type": "array"
+                        },
+                        "response_timeout": {
+                            "type": "number"
+                        },
+                        "security": {
+                            "oneOf": [
+                                {
+                                    "type": "null"
+                                },
+                                {
+                                    "$ref": "hat-gateway://iec104.yaml#/definitions/security"
+                                }
+                            ]
+                        },
+                        "send_window_size": {
+                            "type": "integer"
+                        },
+                        "supervisory_timeout": {
+                            "type": "number"
+                        },
+                        "test_timeout": {
+                            "type": "number"
+                        },
+                        "time_sync_delay": {
+                            "type": [
+                                "null",
+                                "number"
+                            ]
+                        }
+                    },
+                    "required": [
+                        "remote_addresses",
+                        "response_timeout",
+                        "supervisory_timeout",
+                        "test_timeout",
+                        "send_window_size",
+                        "receive_window_size",
+                        "reconnect_delay",
+                        "time_sync_delay",
+                        "security"
+                    ],
+                    "type": "object"
+                },
+                "messages": {
+                    "connections": {
+                        "items": {
                             "properties": {
-                                "event_server_address": {
-                                    "type": "string"
+                                "connection_id": {
+                                    "type": "integer"
+                                },
+                                "local": {
+                                    "properties": {
+                                        "host": {
+                                            "type": "string"
+                                        },
+                                        "port": {
+                                            "type": "integer"
+                                        }
+                                    },
+                                    "required": [
+                                        "host",
+                                        "port"
+                                    ],
+                                    "type": "object"
+                                },
+                                "remote": {
+                                    "properties": {
+                                        "host": {
+                                            "type": "string"
+                                        },
+                                        "port": {
+                                            "type": "integer"
+                                        }
+                                    },
+                                    "required": [
+                                        "host",
+                                        "port"
+                                    ],
+                                    "type": "object"
                                 }
                             },
                             "required": [
-                                "event_server_address"
+                                "connection_id",
+                                "local",
+                                "remote"
                             ],
                             "type": "object"
+                        },
+                        "type": "array"
+                    }
+                },
+                "security": {
+                    "properties": {
+                        "ca_path": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "cert_path": {
+                            "type": "string"
+                        },
+                        "key_path": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "renegotiate_delay": {
+                            "type": [
+                                "null",
+                                "number"
+                            ]
+                        },
+                        "strict_mode": {
+                            "type": "boolean"
+                        },
+                        "verify_cert": {
+                            "type": "boolean"
                         }
-                    ]
+                    },
+                    "required": [
+                        "cert_path",
+                        "key_path",
+                        "verify_cert",
+                        "ca_path"
+                    ],
+                    "type": "object"
+                },
+                "slave": {
+                    "properties": {
+                        "buffers": {
+                            "items": {
+                                "properties": {
+                                    "name": {
+                                        "type": "string"
+                                    },
+                                    "size": {
+                                        "type": "integer"
+                                    }
+                                },
+                                "required": [
+                                    "name",
+                                    "size"
+                                ],
+                                "type": "object"
+                            },
+                            "type": "array"
+                        },
+                        "data": {
+                            "items": {
+                                "properties": {
+                                    "asdu_address": {
+                                        "type": "integer"
+                                    },
+                                    "buffer": {
+                                        "type": [
+                                            "null",
+                                            "string"
+                                        ]
+                                    },
+                                    "data_type": {
+                                        "enum": [
+                                            "SINGLE",
+                                            "DOUBLE",
+                                            "STEP_POSITION",
+                                            "BITSTRING",
+                                            "NORMALIZED",
+                                            "SCALED",
+                                            "FLOATING",
+                                            "BINARY_COUNTER",
+                                            "PROTECTION",
+                                            "PROTECTION_START",
+                                            "PROTECTION_COMMAND",
+                                            "STATUS"
+                                        ]
+                                    },
+                                    "io_address": {
+                                        "type": "integer"
+                                    }
+                                },
+                                "required": [
+                                    "data_type",
+                                    "asdu_address",
+                                    "io_address",
+                                    "buffer"
+                                ],
+                                "type": "object"
+                            },
+                            "type": "array"
+                        },
+                        "local_host": {
+                            "type": "string"
+                        },
+                        "local_port": {
+                            "type": "integer"
+                        },
+                        "max_connections": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "receive_window_size": {
+                            "type": "integer"
+                        },
+                        "remote_hosts": {
+                            "description": "if null, all remote hosts are allowed\n",
+                            "items": {
+                                "type": "string"
+                            },
+                            "type": [
+                                "array",
+                                "null"
+                            ]
+                        },
+                        "response_timeout": {
+                            "type": "number"
+                        },
+                        "security": {
+                            "oneOf": [
+                                {
+                                    "type": "null"
+                                },
+                                {
+                                    "$ref": "hat-gateway://iec104.yaml#/definitions/security"
+                                }
+                            ]
+                        },
+                        "send_window_size": {
+                            "type": "integer"
+                        },
+                        "supervisory_timeout": {
+                            "type": "number"
+                        },
+                        "test_timeout": {
+                            "type": "number"
+                        }
+                    },
+                    "required": [
+                        "local_host",
+                        "local_port",
+                        "remote_hosts",
+                        "max_connections",
+                        "response_timeout",
+                        "supervisory_timeout",
+                        "test_timeout",
+                        "send_window_size",
+                        "receive_window_size",
+                        "security",
+                        "buffers",
+                        "data"
+                    ],
+                    "type": "object"
                 }
-            ],
+            },
+            "id": "hat-gateway://iec104.yaml#"
+        },
+        "main.yaml": {
             "definitions": {
                 "device": {
                     "description": "structure of device configuration depends on device type\n",
                     "properties": {
                         "module": {
                             "description": "full python module name that implements device\n",
                             "type": "string"
@@ -84,19 +1882,199 @@
                         "name"
                     ],
                     "type": "object"
                 }
             },
             "description": "Gateway's configuration",
             "id": "hat-gateway://main.yaml#",
-            "title": "Gateway"
+            "properties": {
+                "devices": {
+                    "items": {
+                        "$ref": "hat-gateway://main.yaml#/definitions/device"
+                    },
+                    "type": "array"
+                },
+                "event_server": {
+                    "oneOf": [
+                        {
+                            "properties": {
+                                "monitor_component": {
+                                    "properties": {
+                                        "event_server_group": {
+                                            "type": "string"
+                                        },
+                                        "gateway_group": {
+                                            "type": "string"
+                                        },
+                                        "host": {
+                                            "default": "127.0.0.1",
+                                            "type": "string"
+                                        },
+                                        "port": {
+                                            "default": 23010,
+                                            "type": "integer"
+                                        }
+                                    },
+                                    "required": [
+                                        "host",
+                                        "port",
+                                        "gateway_group",
+                                        "event_server_group"
+                                    ],
+                                    "type": "object"
+                                }
+                            },
+                            "required": [
+                                "monitor_component"
+                            ],
+                            "type": "object"
+                        },
+                        {
+                            "properties": {
+                                "eventer_server": {
+                                    "properties": {
+                                        "host": {
+                                            "default": "127.0.0.1",
+                                            "type": "string"
+                                        },
+                                        "port": {
+                                            "default": 23012,
+                                            "type": "integer"
+                                        }
+                                    },
+                                    "required": [
+                                        "host",
+                                        "port"
+                                    ],
+                                    "type": "object"
+                                }
+                            },
+                            "required": [
+                                "eventer_server"
+                            ],
+                            "type": "object"
+                        }
+                    ]
+                },
+                "gateway_name": {
+                    "type": "string"
+                },
+                "log": {
+                    "$ref": "hat-json://logging.yaml#"
+                },
+                "type": {
+                    "description": "configuration type identification",
+                    "enum": [
+                        "gateway"
+                    ]
+                },
+                "version": {
+                    "description": "component version",
+                    "type": "string"
+                }
+            },
+            "required": [
+                "gateway_name",
+                "event_server",
+                "devices"
+            ],
+            "title": "Gateway",
+            "type": "object"
         },
         "modbus.yaml": {
-            "$schema": "http://json-schema.org/draft-07/schema#",
             "definitions": {
+                "events": {
+                    "master": {
+                        "gateway": {
+                            "read": {
+                                "properties": {
+                                    "cause": {
+                                        "enum": [
+                                            "INTERROGATE",
+                                            "CHANGE"
+                                        ]
+                                    },
+                                    "result": {
+                                        "enum": [
+                                            "SUCCESS",
+                                            "INVALID_FUNCTION_CODE",
+                                            "INVALID_DATA_ADDRESS",
+                                            "INVALID_DATA_VALUE",
+                                            "FUNCTION_ERROR"
+                                        ]
+                                    },
+                                    "value": {
+                                        "type": "integer"
+                                    }
+                                },
+                                "required": [
+                                    "result"
+                                ],
+                                "type": "object"
+                            },
+                            "remote_device_status": {
+                                "enum": [
+                                    "DISABLED",
+                                    "CONNECTING",
+                                    "CONNECTED",
+                                    "DISCONNECTED"
+                                ]
+                            },
+                            "status": {
+                                "enum": [
+                                    "DISCONNECTED",
+                                    "CONNECTING",
+                                    "CONNECTED"
+                                ]
+                            },
+                            "write": {
+                                "properties": {
+                                    "request_id": {
+                                        "type": "string"
+                                    },
+                                    "result": {
+                                        "enum": [
+                                            "SUCCESS",
+                                            "INVALID_FUNCTION_CODE",
+                                            "INVALID_DATA_ADDRESS",
+                                            "INVALID_DATA_VALUE",
+                                            "FUNCTION_ERROR",
+                                            "TIMEOUT"
+                                        ]
+                                    }
+                                },
+                                "required": [
+                                    "request_id",
+                                    "result"
+                                ],
+                                "type": "object"
+                            }
+                        },
+                        "system": {
+                            "enable": {
+                                "type": "boolean"
+                            },
+                            "write": {
+                                "properties": {
+                                    "request_id": {
+                                        "type": "string"
+                                    },
+                                    "value": {
+                                        "type": "integer"
+                                    }
+                                },
+                                "required": [
+                                    "request_id",
+                                    "value"
+                                ],
+                                "type": "object"
+                            }
+                        }
+                    }
+                },
                 "master": {
                     "properties": {
                         "connection": {
                             "properties": {
                                 "connect_delay": {
                                     "description": "Delay (in seconds) between two consecutive connection\nestablishment attempts\n",
                                     "type": "number"
@@ -109,22 +2087,30 @@
                                     "description": "Modbus message encoding type\n",
                                     "enum": [
                                         "TCP",
                                         "RTU",
                                         "ASCII"
                                     ]
                                 },
-                                "request_retry_count": {
-                                    "description": "Number of request retries before remote data is considered\nunavailable\n",
-                                    "type": "integer"
+                                "request_delay": {
+                                    "description": "Delay (in seconds) between two consecutive requests\n(minimal duration between response and next request)\n",
+                                    "type": "number"
                                 },
                                 "request_retry_delay": {
-                                    "description": "Delay (in seconds) between two consecutive request retries\n",
+                                    "description": "Delay (in seconds) between two consecutive delayed\nrequest retries\n",
                                     "type": "number"
                                 },
+                                "request_retry_delayed_count": {
+                                    "description": "Number of delayed request retries before remote data\nis considered unavailable. Total number\nof retries is request_retry_immediate_count *\nrequest_retry_delayed_count.\n",
+                                    "type": "integer"
+                                },
+                                "request_retry_immediate_count": {
+                                    "description": "Number of immediate request retries before remote\ndata is considered unavailable. Total number\nof retries is request_retry_immediate_count *\nrequest_retry_delayed_count.\n",
+                                    "type": "integer"
+                                },
                                 "request_timeout": {
                                     "description": "Maximum duration (in seconds) of read or write\nrequest/response exchange.\n",
                                     "type": "number"
                                 },
                                 "transport": {
                                     "oneOf": [
                                         {
@@ -233,15 +2219,17 @@
                             },
                             "required": [
                                 "modbus_type",
                                 "transport",
                                 "connect_timeout",
                                 "connect_delay",
                                 "request_timeout",
-                                "request_retry_count",
+                                "request_delay",
+                                "request_retry_immediate_count",
+                                "request_retry_delayed_count",
                                 "request_retry_delay"
                             ],
                             "type": "object"
                         },
                         "remote_devices": {
                             "items": {
                                 "properties": {
@@ -293,18 +2281,23 @@
                                             "type": "object"
                                         },
                                         "type": "array"
                                     },
                                     "device_id": {
                                         "description": "Modbus device identifier\n",
                                         "type": "integer"
+                                    },
+                                    "timeout_poll_delay": {
+                                        "description": "Delay (in seconds) after read timeout and\nbefore device polling is resumed\n",
+                                        "type": "number"
                                     }
                                 },
                                 "required": [
                                     "device_id",
+                                    "timeout_poll_delay",
                                     "data"
                                 ],
                                 "type": "object"
                             },
                             "type": "array"
                         }
                     },
@@ -314,10 +2307,252 @@
                     ],
                     "title": "Modbus master",
                     "type": "object"
                 }
             },
             "id": "hat-gateway://modbus.yaml#",
             "title": "Modbus devices"
+        },
+        "snmp.yaml": {
+            "definitions": {
+                "data": {
+                    "oneOf": [
+                        {
+                            "properties": {
+                                "type": {
+                                    "enum": [
+                                        "INTEGER",
+                                        "UNSIGNED",
+                                        "COUNTER",
+                                        "BIG_COUNTER",
+                                        "TIME_TICKS"
+                                    ]
+                                },
+                                "value": {
+                                    "type": "integer"
+                                }
+                            },
+                            "required": [
+                                "type",
+                                "value"
+                            ],
+                            "type": "object"
+                        },
+                        {
+                            "properties": {
+                                "type": {
+                                    "enum": [
+                                        "STRING",
+                                        "OBJECT_ID",
+                                        "IP_ADDRESS",
+                                        "ARBITRARY"
+                                    ]
+                                },
+                                "value": {
+                                    "type": "string"
+                                }
+                            },
+                            "required": [
+                                "type",
+                                "value"
+                            ],
+                            "type": "object"
+                        },
+                        {
+                            "properties": {
+                                "type": {
+                                    "const": "ERROR"
+                                },
+                                "value": {
+                                    "enum": [
+                                        "TOO_BIG",
+                                        "NO_SUCH_NAME",
+                                        "BAD_VALUE",
+                                        "READ_ONLY",
+                                        "GEN_ERR",
+                                        "NO_ACCESS",
+                                        "WRONG_TYPE",
+                                        "WRONG_LENGTH",
+                                        "WRONG_ENCODING",
+                                        "WRONG_VALUE",
+                                        "NO_CREATION",
+                                        "INCONSISTENT_VALUE",
+                                        "RESOURCE_UNAVAILABLE",
+                                        "COMMIT_FAILED",
+                                        "UNDO_FAILED",
+                                        "AUTHORIZATION_ERROR",
+                                        "NOT_WRITABLE",
+                                        "INCONSISTENT_NAME",
+                                        "EMPTY",
+                                        "UNSPECIFIED",
+                                        "NO_SUCH_OBJECT",
+                                        "NO_SUCH_INSTANCE",
+                                        "END_OF_MIB_VIEW"
+                                    ]
+                                }
+                            },
+                            "required": [
+                                "type",
+                                "value"
+                            ],
+                            "type": "object"
+                        }
+                    ]
+                },
+                "events": {
+                    "manager": {
+                        "gateway": {
+                            "read": {
+                                "properties": {
+                                    "cause": [
+                                        "INTERROGATE",
+                                        "CHANGE",
+                                        "REQUESTED"
+                                    ],
+                                    "data": {
+                                        "$ref": "hat-gateway://snmp.yaml#/definitions/data"
+                                    },
+                                    "session_id": {
+                                        "oneOf": [
+                                            {
+                                                "description": "In case of INTERROGATE or CHANGE cause\n",
+                                                "type": "null"
+                                            },
+                                            {
+                                                "description": "In case of REQUESTED cause\n"
+                                            }
+                                        ]
+                                    }
+                                },
+                                "required": [
+                                    "session_id",
+                                    "cause",
+                                    "data"
+                                ],
+                                "type": "object"
+                            },
+                            "status": {
+                                "enum": [
+                                    "CONNECTING",
+                                    "CONNECTED",
+                                    "DISCONNECTED"
+                                ]
+                            },
+                            "write": {
+                                "properties": {
+                                    "success": {
+                                        "type": "boolean"
+                                    }
+                                },
+                                "required": [
+                                    "session_id",
+                                    "success"
+                                ],
+                                "type": "object"
+                            }
+                        },
+                        "system": {
+                            "read": {
+                                "required": [
+                                    "session_id"
+                                ],
+                                "type": "object"
+                            },
+                            "write": {
+                                "properties": {
+                                    "data": {
+                                        "$ref": "hat-gateway://snmp.yaml#/definitions/data"
+                                    }
+                                },
+                                "required": [
+                                    "session_id",
+                                    "data"
+                                ],
+                                "type": "object"
+                            }
+                        }
+                    }
+                },
+                "manager": {
+                    "properties": {
+                        "connect_delay": {
+                            "description": "Delay (in seconds) between two consecutive connection\nestablishment attempts\n",
+                            "type": "number"
+                        },
+                        "polling_delay": {
+                            "description": "Delay (in seconds) between two consecutive polling cycles\n",
+                            "type": "number"
+                        },
+                        "polling_oids": {
+                            "description": "List of OIDs read during polling cycle\n",
+                            "items": {
+                                "type": "string"
+                            },
+                            "type": "array"
+                        },
+                        "remote_host": {
+                            "description": "Remote hostname or IP address\n",
+                            "type": "string"
+                        },
+                        "remote_port": {
+                            "description": "Remote UDP port\n",
+                            "type": "integer"
+                        },
+                        "request_retry_count": {
+                            "description": "Number of request retries before remote data is considered\nunavailable\n",
+                            "type": "integer"
+                        },
+                        "request_retry_delay": {
+                            "description": "Delay (in seconds) between two consecutive request retries\n",
+                            "type": "number"
+                        },
+                        "request_timeout": {
+                            "description": "Maximum duration (in seconds) of request/response exchange\n",
+                            "type": "number"
+                        },
+                        "snmp_context": {
+                            "properties": {
+                                "engine_id": {
+                                    "description": "Available only in case of V3 version\n",
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "name": {
+                                    "description": "Used as community name in case of V1 or V2C version\n",
+                                    "type": "string"
+                                }
+                            },
+                            "required": [
+                                "engine_id",
+                                "name"
+                            ],
+                            "type": "object"
+                        },
+                        "snmp_version": {
+                            "enum": [
+                                "V1",
+                                "V2C",
+                                "V3"
+                            ]
+                        }
+                    },
+                    "required": [
+                        "snmp_version",
+                        "snmp_context",
+                        "remote_host",
+                        "remote_port",
+                        "connect_delay",
+                        "request_timeout",
+                        "request_retry_count",
+                        "request_retry_delay",
+                        "polling_delay",
+                        "polling_oids"
+                    ],
+                    "type": "object"
+                }
+            },
+            "id": "hat-gateway://snmp.yaml#"
         }
     }
 }
```

## hat/gateway/main.py

```diff
@@ -1,124 +1,80 @@
 """Gateway main"""
 
 from pathlib import Path
+import argparse
 import asyncio
 import contextlib
-import functools
-import importlib
 import logging.config
 import sys
-import typing
 
 import appdirs
-import click
 
 from hat import aio
 from hat import json
+
 from hat.gateway import common
-from hat.gateway.engine import create_engine
-import hat.event.client
-import hat.event.common
-import hat.monitor.client
+from hat.gateway.runner import MainRunner
+
 
+mlog: logging.Logger = logging.getLogger('hat.gateway.main')
+"""Module logger"""
 
 user_conf_dir: Path = Path(appdirs.user_config_dir('hat'))
 """User configuration directory path"""
 
 
-@click.command()
-@click.option('--conf', default=None, metavar='PATH', type=Path,
-              help="configuration defined by hat-gateway://main.yaml# "
-                   "(default $XDG_CONFIG_HOME/hat/gateway.{yaml|yml|json})")
-def main(conf: typing.Optional[Path]):
-    """Gateway"""
-    if not conf:
-        for suffix in ('.yaml', '.yml', '.json'):
-            conf = (user_conf_dir / 'gateway').with_suffix(suffix)
-            if conf.exists():
-                break
-
-    if conf == Path('-'):
-        conf = json.decode_stream(sys.stdin)
-    else:
-        conf = json.decode_file(conf)
+def create_argument_parser() -> argparse.ArgumentParser:
+    """Create argument parser"""
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
+        '--conf', metavar='PATH', type=Path, default=None,
+        help="configuration defined by hat-gateway://main.yaml# "
+             "(default $XDG_CONFIG_HOME/hat/gateway.{yaml|yml|toml|json})")
+    return parser
+
 
+def main():
+    """Gateway"""
+    parser = create_argument_parser()
+    args = parser.parse_args()
+    conf = json.read_conf(args.conf, user_conf_dir / 'gateway')
     sync_main(conf)
 
 
 def sync_main(conf: json.Data):
     """Sync main entry point"""
     aio.init_asyncio()
 
     common.json_schema_repo.validate('hat-gateway://main.yaml#', conf)
 
     for device_conf in conf['devices']:
-        module = importlib.import_module(device_conf['module'])
-        if module.json_schema_repo and module.json_schema_id:
-            module.json_schema_repo.validate(module.json_schema_id,
-                                             device_conf)
-
-    logging.config.dictConfig(conf['log'])
+        info = common.import_device_info(device_conf['module'])
+        if info.json_schema_repo and info.json_schema_id:
+            info.json_schema_repo.validate(info.json_schema_id, device_conf)
+
+    log_conf = conf.get('log')
+    if log_conf:
+        logging.config.dictConfig(log_conf)
 
     with contextlib.suppress(asyncio.CancelledError):
         aio.run_asyncio(async_main(conf))
 
 
 async def async_main(conf: json.Data):
     """Async main entry point"""
-    async_group = aio.Group()
-
-    try:
-        subscriptions = [('gateway', conf['gateway_name'], '?', '?',
-                          'system', '*')]
+    main_runner = MainRunner(conf)
 
-        if 'monitor' in conf:
-            monitor = await hat.monitor.client.connect(conf['monitor'])
-            _bind_resource(async_group, monitor)
-
-            component = hat.monitor.client.Component(
-                monitor, run_with_monitor, conf, monitor, subscriptions)
-            component.set_enabled(True)
-            _bind_resource(async_group, component)
-
-            await async_group.wait_closing()
-
-        else:
-            client = await hat.event.client.connect(
-                conf['event_server_address'], subscriptions)
-            _bind_resource(async_group, client)
+    async def cleanup():
+        await main_runner.async_close()
+        await asyncio.sleep(0.1)
 
-            await async_group.spawn(run_with_event, conf, client)
-
-    finally:
-        await aio.uncancellable(async_group.async_close())
-
-
-async def run_with_monitor(component: hat.monitor.client.Component,
-                           conf: json.Data,
-                           monitor: hat.monitor.client.Client,
-                           subscriptions: typing.List[hat.event.common.EventType]):  # NOQA
-    """Run monitor component"""
-    run_cb = functools.partial(run_with_event, conf)
-    await hat.event.client.run_client(monitor, conf['event_server_group'],
-                                      run_cb, subscriptions)
-
-
-async def run_with_event(conf: json.Data,
-                         client: hat.event.client.Client):
-    """Run event client"""
-    engine = await create_engine(conf, client)
     try:
-        await engine.wait_closing()
-    finally:
-        await aio.uncancellable(engine.async_close())
-
+        await main_runner.wait_closing()
 
-def _bind_resource(async_group, resource):
-    async_group.spawn(aio.call_on_cancel, resource.async_close)
-    async_group.spawn(aio.call_on_done, resource.wait_closing(),
-                      async_group.close)
+    finally:
+        await aio.uncancellable(cleanup())
 
 
 if __name__ == '__main__':
     sys.argv[0] = 'hat-gateway'
     sys.exit(main())
```

## hat/gateway/devices/modbus/master/__init__.py

```diff
@@ -1,14 +1,11 @@
 """Modbus master device"""
 
-from hat import json
 from hat.gateway import common
-from hat.gateway.devices.modbus.master import device
+from hat.gateway.devices.modbus.master.device import ModbusMasterDevice
 
 
-device_type: str = "modbus_master"
-
-json_schema_id: str = "hat-gateway://modbus.yaml#/definitions/master"
-
-json_schema_repo: json.SchemaRepository = common.json_schema_repo
-
-create: common.CreateDevice = device.create
+info: common.DeviceInfo = common.DeviceInfo(
+    type="modbus_master",
+    create=ModbusMasterDevice,
+    json_schema_id="hat-gateway://modbus.yaml#/definitions/master",
+    json_schema_repo=common.json_schema_repo)
```

## hat/gateway/devices/modbus/master/connection.py

```diff
@@ -1,42 +1,47 @@
 import asyncio
-import contextlib
 import enum
 import logging
+import time
 import typing
 
 from hat import json
 from hat import aio
 from hat.drivers import modbus
 from hat.drivers import serial
 from hat.drivers import tcp
 
 
 mlog = logging.getLogger(__name__)
 
 
-DataType = modbus.DataType
+DataType: typing.TypeAlias = modbus.DataType
 
 
 Error = enum.Enum('Error', [
     'INVALID_FUNCTION_CODE',
     'INVALID_DATA_ADDRESS',
     'INVALID_DATA_VALUE',
     'FUNCTION_ERROR',
     'TIMEOUT'])
 
 
-async def connect(conf: json.Data) -> 'Connection':
+async def connect(conf: json.Data,
+                  log_prefix: str,
+                  request_queue_size: int = 1024
+                  ) -> 'Connection':
     transport_conf = conf['transport']
     modbus_type = modbus.ModbusType[conf['modbus_type']]
 
     if transport_conf['type'] == 'TCP':
         addr = tcp.Address(transport_conf['host'], transport_conf['port'])
-        master = await modbus.create_tcp_master(modbus_type=modbus_type,
-                                                addr=addr)
+        master = await modbus.create_tcp_master(
+            modbus_type=modbus_type,
+            addr=addr,
+            response_timeout=conf['request_timeout'])
 
     elif transport_conf['type'] == 'SERIAL':
         port = transport_conf['port']
         baudrate = transport_conf['baudrate']
         bytesize = serial.ByteSize[transport_conf['bytesize']]
         parity = serial.Parity[transport_conf['parity']]
         stopbits = serial.StopBits[transport_conf['stopbits']]
@@ -50,130 +55,178 @@
             baudrate=baudrate,
             bytesize=bytesize,
             parity=parity,
             stopbits=stopbits,
             xonxoff=xonxoff,
             rtscts=rtscts,
             dsrdtr=dsrdtr,
-            silent_interval=silent_interval)
+            silent_interval=silent_interval,
+            response_timeout=conf['request_timeout'])
 
     else:
         raise ValueError('unsupported link type')
 
-    conn = Connection()
-    conn._conf = conf
-    conn._master = master
-    conn._request_queue = aio.Queue()
+    return Connection(conf=conf,
+                      master=master,
+                      log_prefix=log_prefix,
+                      request_queue_size=request_queue_size)
 
-    conn.async_group.spawn(conn._request_loop)
 
-    return conn
+class Connection(aio.Resource):
 
+    def __init__(self,
+                 conf: json.Data,
+                 master: modbus.Master,
+                 log_prefix: str,
+                 request_queue_size: int):
+        self._conf = conf
+        self._log_prefix = log_prefix
+        self._master = master
+        self._request_queue = aio.Queue(request_queue_size)
 
-class Connection(aio.Resource):
+        self.async_group.spawn(self._request_loop)
 
     @property
     def async_group(self) -> aio.Group:
         return self._master.async_group
 
     async def read(self,
                    device_id: int,
                    data_type: modbus.DataType,
                    start_address: int,
                    quantity: int
-                   ) -> typing.Union[typing.List[int], Error]:
-        mlog.debug('enqueuing read request')
+                   ) -> list[int] | Error:
+        self._log(logging.DEBUG, 'enqueuing read request')
         return await self._request(self._master.read, device_id, data_type,
                                    start_address, quantity)
 
     async def write(self,
                     device_id: int,
                     data_type: modbus.DataType,
                     start_address: int,
-                    values: typing.List[int]
-                    ) -> typing.Optional[Error]:
-        mlog.debug('enqueuing write request')
+                    values: list[int]
+                    ) -> Error | None:
+        self._log(logging.DEBUG, 'enqueuing write request')
         return await self._request(self._master.write, device_id, data_type,
                                    start_address, values)
 
     async def write_mask(self,
                          device_id: int,
                          address: int,
                          and_mask: int,
                          or_mask: int
-                         ) -> typing.Optional[Error]:
-        mlog.debug('enqueuing write mask request')
+                         ) -> Error | None:
+        self._log(logging.DEBUG, 'enqueuing write mask request')
         return await self._request(self._master.write_mask, device_id,
                                    address, and_mask, or_mask)
 
     async def _request_loop(self):
         future = None
+        result_t = None
 
         try:
-            mlog.debug('starting request loop')
+            self._log(logging.DEBUG, 'starting request loop')
             while True:
-                fn, args, future = await self._request_queue.get()
-                mlog.debug('dequed request')
+                fn, args, delayed_count, future = await self._request_queue.get()  # NOQA
+                self._log(logging.DEBUG, 'dequed request')
+
+                if result_t is not None and self._conf['request_delay'] > 0:
+                    dt = time.monotonic() - result_t
+                    if dt < self._conf['request_delay']:
+                        await asyncio.sleep(self._conf['request_delay'] - dt)
 
                 if future.done():
                     continue
 
-                try:
-                    result = await self._communicate(fn, *args)
-                    if not future.done():
-                        mlog.debug('setting request result')
-                        future.set_result(result)
-                except Exception as e:
-                    mlog.debug('setting request exception')
-                    future.set_exception(e)
-                    raise
+                delayed_count -= 1
+                immediate_count = (
+                    self._conf['request_retry_immediate_count'] + 1)
+
+                while True:
+                    try:
+                        immediate_count -= 1
+                        result = await fn(*args)
+                        result_t = time.monotonic()
+
+                        self._log(logging.DEBUG, 'received result %s', result)
+                        if isinstance(result, modbus.Error):
+                            result = Error[result.name]
+
+                        if not future.done():
+                            self._log(logging.DEBUG, 'setting request result')
+                            future.set_result(result)
+
+                        break
+
+                    except TimeoutError:
+                        self._log(logging.DEBUG, 'single request timeout')
+
+                        if immediate_count > 0:
+                            self._log(logging.DEBUG, 'immediate request retry')
+                            continue
+
+                        if delayed_count > 0:
+                            self._log(logging.DEBUG, 'delayed request retry')
+                            self.async_group.spawn(self._delay_request, fn,
+                                                   args, delayed_count, future)
+                            future = None
+
+                        elif not future.done():
+                            self._log(logging.DEBUG,
+                                      'request resulting in timeout')
+                            future.set_result(Error.TIMEOUT)
+
+                        break
+
+                    except Exception as e:
+                        self._log(logging.DEBUG, 'setting request exception')
+                        if not future.done():
+                            future.set_exception(e)
+                        raise
 
         except ConnectionError:
-            mlog.debug('connection closed')
+            self._log(logging.DEBUG, 'connection closed')
 
         except Exception as e:
-            mlog.error('request loop error: %s', e, exc_info=e)
+            self._log(logging.ERROR, 'request loop error: %s', e, exc_info=e)
 
         finally:
-            mlog.debug('closing request loop')
+            self._log(logging.DEBUG, 'closing request loop')
             self.close()
             self._request_queue.close()
-            if future and not future.done():
-                future.set_exception(ConnectionError())
-            while not self._request_queue.empty():
-                _, __, future = self._request_queue.get_nowait()
-                if not future.done():
+
+            while True:
+                if future and not future.done():
                     future.set_exception(ConnectionError())
+                if self._request_queue.empty():
+                    break
+                _, __, ___, future = self._request_queue.get_nowait()
 
     async def _request(self, fn, *args):
         try:
             future = asyncio.Future()
-            self._request_queue.put_nowait((fn, args, future))
+            delayed_count = self._conf['request_retry_delayed_count'] + 1
+            await self._request_queue.put((fn, args, delayed_count, future))
+
             return await future
 
         except aio.QueueClosedError:
             raise ConnectionError()
 
-    async def _communicate(self, fn, *args):
-        count = 0
-        while True:
-            mlog.debug('sending request')
-            with contextlib.suppress(asyncio.TimeoutError):
-                result = await aio.wait_for(fn(*args),
-                                            self._conf['request_timeout'])
-                mlog.debug('received result %s', result)
-
-                if isinstance(result, modbus.Error):
-                    return Error[result.name]
-
-                return result
-
-            mlog.debug('single request timeout')
-            count += 1
-            if count >= self._conf['request_retry_count']:
-                break
-
-            mlog.debug('waiting for request retry')
+    async def _delay_request(self, fn, args, delayed_count, future):
+        try:
             await asyncio.sleep(self._conf['request_retry_delay'])
+            await self._request_queue.put((fn, args, delayed_count, future))
+            future = None
+
+        except aio.QueueClosedError:
+            pass
+
+        finally:
+            if future and not future.done():
+                future.set_exception(ConnectionError())
+
+    def _log(self, level, msg, *args, **kwargs):
+        if not mlog.isEnabledFor(level):
+            return
 
-        mlog.debug('request resulting in timeout')
-        return Error.TIMEOUT
+        mlog.log(level, f"{self._log_prefix}: {msg}", *args, **kwargs)
```

## hat/gateway/devices/modbus/master/device.py

```diff
@@ -1,218 +1,206 @@
+from collections.abc import Collection
 import asyncio
 import contextlib
 import logging
 
 from hat import aio
+import hat.event.common
+import hat.event.eventer
+
 from hat.gateway import common
 from hat.gateway.devices.modbus.master.connection import connect
-from hat.gateway.devices.modbus.master.event_client import (RemoteDeviceEnableReq,  # NOQA
-                                                            RemoteDeviceWriteReq,  # NOQA
-                                                            StatusRes,
-                                                            RemoteDeviceStatusRes,  # NOQA
-                                                            RemoteDeviceWriteRes,  # NOQA
-                                                            EventClientProxy)
-from hat.gateway.devices.modbus.master.remote_device import (RemoteDevice,
-                                                             RemoteDeviceReader)  # NOQA
-import hat.event.common
+from hat.gateway.devices.modbus.master.eventer_client import (RemoteDeviceEnableReq,  # NOQA
+                                                              RemoteDeviceWriteReq,  # NOQA
+                                                              StatusRes,
+                                                              RemoteDeviceStatusRes,  # NOQA
+                                                              RemoteDeviceWriteRes,  # NOQA
+                                                              EventerClientProxy)  # NOQA
+from hat.gateway.devices.modbus.master.remote_device import RemoteDevice
 
 
 mlog = logging.getLogger(__name__)
 
 
-async def create(conf: common.DeviceConf,
-                 event_client: common.DeviceEventClient,
-                 event_type_prefix: common.EventTypePrefix
-                 ) -> 'ModbusMasterDevice':
-    device = ModbusMasterDevice()
-    device._enabled_devices = await _query_enabled_devices(event_client,
-                                                           event_type_prefix)
-    device._conf = conf
-    device._event_client = EventClientProxy(event_client, event_type_prefix)
-    device._status = None
-    device._conn = None
-    device._devices = {}
-    device._device_readers = {}
-    device._async_group = aio.Group()
-
-    device._async_group.spawn(aio.call_on_cancel,
-                              device._event_client.async_close)
-    device._async_group.spawn(device._event_client_loop)
-    device._async_group.spawn(device._connection_loop)
-    return device
+class ModbusMasterDevice(aio.Resource):
 
+    def __init__(self,
+                 conf: common.DeviceConf,
+                 eventer_client: hat.event.eventer.Client,
+                 event_type_prefix: common.EventTypePrefix):
+        self._conf = conf
+        self._log_prefix = f"gateway device {conf['name']}"
+        self._eventer_client = EventerClientProxy(eventer_client,
+                                                  event_type_prefix,
+                                                  self._log_prefix)
+        self._enabled_devices = set()
+        self._status = None
+        self._conn = None
+        self._devices = {}
+        self._readers = {}
+        self._async_group = aio.Group()
 
-class ModbusMasterDevice(aio.Resource):
+        self.async_group.spawn(self._connection_loop)
 
     @property
     def async_group(self) -> aio.Group:
         return self._async_group
 
-    async def _event_client_loop(self):
+    async def process_events(self, events: Collection[hat.event.common.Event]):
         try:
-            mlog.debug('starting event client loop')
-            while True:
-                request = await self._event_client.read()
-
+            for request in self._eventer_client.process_events(events):
                 if isinstance(request, RemoteDeviceEnableReq):
-                    mlog.debug('received remote device enable request')
+                    self._log(logging.DEBUG,
+                              'received remote device enable request')
                     if request.enable:
                         self._enable_remote_device(request.device_id)
                     else:
                         await self._disable_remote_device(request.device_id)
 
                 elif isinstance(request, RemoteDeviceWriteReq):
-                    mlog.debug('received remote device write request')
+                    self._log(logging.DEBUG,
+                              'received remote device write request')
                     if self._conn and self._conn.is_open:
                         self._conn.async_group.spawn(
                             self._write, request.device_id, request.data_name,
                             request.request_id, request.value)
 
                 else:
                     raise ValueError('invalid request')
 
-        except ConnectionError:
-            mlog.debug('event client connection closed')
-
         except Exception as e:
-            mlog.error('event client loop error: %s', e, exc_info=e)
-
-        finally:
-            mlog.debug('closing event client loop')
+            self._log(logging.ERROR, 'process events error: %s', e, exc_info=e)
             self.close()
 
     async def _connection_loop(self):
+
+        async def cleanup():
+            if self._conn:
+                await self._conn.async_close()
+
+            with contextlib.suppress(Exception):
+                await self._set_status('DISCONNECTED')
+
         try:
-            mlog.debug('starting connection loop')
+            self._log(logging.DEBUG, 'starting connection loop')
+
+            enabled_devices = await self._eventer_client.query_enabled_devices()  # NOQA
+            self._enabled_devices.update(enabled_devices)
+
             while True:
-                self._set_status('CONNECTING')
+                await self._set_status('CONNECTING')
 
                 try:
                     self._conn = await aio.wait_for(
-                        connect(self._conf['connection']),
+                        connect(self._conf['connection'],
+                                self._log_prefix),
                         self._conf['connection']['connect_timeout'])
+
                 except aio.CancelledWithResultError as e:
                     self._conn = e.result
                     raise
+
                 except Exception as e:
-                    mlog.info('connecting error: %s', e, exc_info=e)
-                    self._set_status('DISCONNECTED')
+                    self._log(logging.INFO, 'connecting error: %s', e,
+                              exc_info=e)
+                    await self._set_status('DISCONNECTED')
                     await asyncio.sleep(
                         self._conf['connection']['connect_delay'])
                     continue
 
-                self._set_status('CONNECTED')
+                await self._set_status('CONNECTED')
                 self._devices = {}
-                self._device_readers = {}
+                self._readers = {}
 
-                mlog.debug('creating remote devices')
+                self._log(logging.DEBUG, 'creating remote devices')
                 for device_conf in self._conf['remote_devices']:
-                    device = RemoteDevice(device_conf, self._conn)
+                    device = RemoteDevice(device_conf, self._conn,
+                                          self._log_prefix)
                     self._devices[device.device_id] = device
 
                     if device.device_id in self._enabled_devices:
                         self._enable_remote_device(device.device_id)
+
                     else:
-                        self._notify_response(RemoteDeviceStatusRes(
+                        await self._notify_response(RemoteDeviceStatusRes(
                             device_id=device.device_id,
                             status='DISABLED'))
 
                 await self._conn.wait_closing()
                 await self._conn.async_close()
-                self._set_status('DISCONNECTED')
+
+                await self._set_status('DISCONNECTED')
 
         except Exception as e:
-            mlog.error('connection loop error: %s', e, exc_info=e)
+            self._log(logging.ERROR, 'connection loop error: %s', e,
+                      exc_info=e)
 
         finally:
-            mlog.debug('closing connection loop')
+            self._log(logging.DEBUG, 'closing connection loop')
             self.close()
-            if self._conn:
-                await aio.uncancellable(self._conn.async_close())
-            with contextlib.suppress(ConnectionError):
-                self._set_status('DISCONNECTED')
+            await aio.uncancellable(cleanup())
 
-    def _notify_response(self, response):
-        self._event_client.write([response])
+    async def _notify_response(self, response):
+        await self._eventer_client.write([response])
 
-    def _set_status(self, status):
+    async def _set_status(self, status):
         if self._status == status:
             return
-        mlog.debug('changing status: %s -> %s', self._status, status)
+
+        self._log(logging.DEBUG, 'changing status: %s -> %s',
+                  self._status, status)
         self._status = status
-        self._notify_response(StatusRes(status))
+        await self._notify_response(StatusRes(status))
 
     def _enable_remote_device(self, device_id):
-        mlog.debug('enabling device %s', device_id)
+        self._log(logging.DEBUG, 'enabling device %s', device_id)
         self._enabled_devices.add(device_id)
 
         device = self._devices.get(device_id)
         if not device:
-            mlog.debug('device %s is not available', device_id)
+            self._log(logging.DEBUG, 'device %s is not available', device_id)
             return
         if not device.conn.is_open:
-            mlog.debug('connection is not available')
+            self._log(logging.DEBUG, 'connection is not available')
             return
 
-        device_reader = self._device_readers.get(device_id)
-        if device_reader and device_reader.is_open:
-            mlog.debug('device reader %s is already running', device_id)
+        reader = self._readers.get(device_id)
+        if reader and reader.is_open:
+            self._log(logging.DEBUG, 'reader %s is already running', device_id)
             return
 
-        mlog.debug('creating reader for device %s', device_id)
-        self._device_readers[device.device_id] = \
-            RemoteDeviceReader(device, self._notify_response)
+        self._log(logging.DEBUG, 'creating reader for device %s', device_id)
+        reader = device.create_reader(self._notify_response)
+        self._readers[device.device_id] = reader
 
     async def _disable_remote_device(self, device_id):
-        mlog.debug('disabling device %s', device_id)
+        self._log(logging.DEBUG, 'disabling device %s', device_id)
         self._enabled_devices.discard(device_id)
 
-        device_reader = self._device_readers.pop(device_id, None)
-        if not device_reader:
-            mlog.debug('device reader %s is not available', device_id)
+        reader = self._readers.pop(device_id, None)
+        if not reader:
+            self._log(logging.DEBUG, 'device reader %s is not available',
+                      device_id)
             return
 
-        await device_reader.async_close()
+        await reader.async_close()
 
     async def _write(self, device_id, data_name, request_id, value):
-        mlog.debug('writing (device_id: %s; data_name: %s; value: %s)',
-                   device_id, data_name, value)
+        self._log(logging.DEBUG,
+                  'writing (device_id: %s; data_name: %s; value: %s)',
+                  device_id, data_name, value)
 
         device = self._devices.get(device_id)
         if not device:
-            mlog.debug('device %s is not available', device_id)
+            self._log(logging.DEBUG, 'device %s is not available', device_id)
             return
 
-        data = device.data.get(data_name)
-        if not data:
-            mlog.debug('data %s is not available', data_name)
-            return
-
-        result = await data.write(value)
-        result = result.name if result else 'SUCCESS'
-        mlog.debug('writing result: %s', result)
-        self._notify_response(RemoteDeviceWriteRes(device_id=device_id,
-                                                   data_name=data_name,
-                                                   request_id=request_id,
-                                                   result=result))
-
-
-async def _query_enabled_devices(event_client, event_type_prefix):
-    mlog.debug('querying enabled devices')
-    enabled_devices = set()
+        response = await device.write(data_name, request_id, value)
+        if response:
+            self._log(logging.DEBUG, 'writing result: %s', response.result)
+            await self._notify_response(response)
 
-    events = await event_client.query(hat.event.common.QueryData(
-        event_types=[(*event_type_prefix, 'system', 'remote_device', '?',
-                      'enable')],
-        unique_type=True))
-    mlog.debug('received %s events', len(events))
-
-    for event in events:
-        if not event.payload or not bool(event.payload.data):
-            continue
-
-        device_id_str = event.event_type[6]
-        with contextlib.suppress(ValueError):
-            enabled_devices.add(int(device_id_str))
+    def _log(self, level, msg, *args, **kwargs):
+        if not mlog.isEnabledFor(level):
+            return
 
-    mlog.debug('detected %s enabled devices', len(enabled_devices))
-    return enabled_devices
+        mlog.log(level, f"{self._log_prefix}: {msg}", *args, **kwargs)
```

## hat/gateway/devices/modbus/master/remote_device.py

```diff
@@ -1,345 +1,422 @@
 import asyncio
 import collections
+import contextlib
+import enum
+import functools
 import itertools
 import logging
 import math
+import time
 import typing
 
 from hat import aio
 from hat import json
+
 from hat.gateway.devices.modbus.master.connection import (DataType,
                                                           Error,
                                                           Connection)
-from hat.gateway.devices.modbus.master.event_client import (RemoteDeviceStatusRes,  # NOQA
-                                                            RemoteDeviceReadRes,  # NOQA
-                                                            Response)
+from hat.gateway.devices.modbus.master.eventer_client import (RemoteDeviceStatusRes,  # NOQA
+                                                              RemoteDeviceReadRes,  # NOQA
+                                                              RemoteDeviceWriteRes,  # NOQA
+                                                              Response)
 
 
 mlog = logging.getLogger(__name__)
 
 
-ResponseCb = typing.Callable[[Response], None]
+ResponseCb: typing.TypeAlias = aio.AsyncCallable[[Response], None]
+
+
+class _Status(enum.Enum):
+    CONNECTING = 'CONNECTING'
+    CONNECTED = 'CONNECTED'
+    DISCONNECTED = 'DISCONNECTED'
+    DISABLED = 'DISABLED'
+
+
+class _DataInfo(typing.NamedTuple):
+    data_type: DataType
+    register_size: int
+    start_address: int
+    bit_count: int
+    bit_offset: int
+    quantity: int
+    interval: float | None
+    name: str
+
+
+class _DataGroup(typing.NamedTuple):
+    data_infos: list[_DataInfo]
+    interval: float
+    data_type: DataType
+    start_address: int
+    quantity: int
 
 
 class RemoteDevice:
 
     def __init__(self,
                  conf: json.Data,
-                 conn: Connection):
+                 conn: Connection,
+                 log_prefix: str):
         self._conn = conn
         self._device_id = conf['device_id']
-        self._data = {i['name']: Data(i, self._device_id, conn)
-                      for i in conf['data']}
+        self._timeout_poll_delay = conf['timeout_poll_delay']
+        self._log_prefix = f"{log_prefix}: remote device id {self._device_id}"
+        self._data_infos = {data_info.name: data_info
+                            for data_info in _get_data_infos(conf)}
+        self._data_groups = list(_group_data_infos(self._data_infos.values()))
 
     @property
     def conn(self) -> Connection:
         return self._conn
 
     @property
     def device_id(self) -> int:
         return self._device_id
 
-    @property
-    def data(self) -> typing.Dict[int, 'Data']:
-        return self._data
+    def create_reader(self, response_cb: ResponseCb) -> aio.Resource:
+        return _Reader(conn=self._conn,
+                       device_id=self._device_id,
+                       timeout_poll_delay=self._timeout_poll_delay,
+                       data_groups=self._data_groups,
+                       response_cb=response_cb,
+                       log_prefix=self._log_prefix)
+
+    async def write(self,
+                    data_name: str,
+                    request_id: str,
+                    value: int
+                    ) -> RemoteDeviceWriteRes | None:
+        data_info = self._data_infos.get(data_name)
+        if not data_info:
+            self._log(logging.DEBUG, 'data %s is not available', data_name)
+            return
 
+        if data_info.data_type == DataType.COIL:
+            result = await self._write_coil(data_info, value)
 
-class RemoteDeviceReader(aio.Resource):
+        elif data_info.data_type == DataType.HOLDING_REGISTER:
+            result = await self._write_holding_register(data_info, value)
 
-    def __init__(self,
-                 remote_device: RemoteDevice,
-                 response_cb: ResponseCb):
-        self._response_cb = response_cb
-        self._device_id = remote_device.device_id
-        self._async_group = remote_device.conn.async_group.create_subgroup()
-        self._status = None
-        self._data_readers = collections.deque()
+        else:
+            self._log(logging.DEBUG, 'write unsupported for %s',
+                      data_info.data_type)
+            return
 
-        reader_data = {}
-        for data in remote_device.data.values():
-            if data.interval is None:
-                continue
-            key = (data.data_type, data.start_address, data.quantity,
-                   data.interval)
-            reader_data.setdefault(key, []).append(data)
-
-        for key, data in reader_data.items():
-            data_type, start_address, quantity, interval = key
-            data_reader = _DataReader(self._async_group, remote_device.conn,
-                                      data, remote_device.device_id, data_type,
-                                      start_address, quantity, interval,
-                                      self._on_response)
-            self._data_readers.append(data_reader)
+        return RemoteDeviceWriteRes(
+            device_id=self._device_id,
+            data_name=data_name,
+            request_id=request_id,
+            result=result.name if result else 'SUCCESS')
+
+    async def _write_coil(self, data_info, value):
+        address = data_info.start_address + data_info.bit_offset
+        registers = [(value >> (data_info.bit_count - i - 1)) & 1
+                     for i in range(data_info.bit_count)]
+        return await self._conn.write(device_id=self._device_id,
+                                      data_type=data_info.data_type,
+                                      start_address=address,
+                                      values=registers)
+
+    async def _write_holding_register(self, data_info, value):
+        address = data_info.start_address + (data_info.bit_offset // 16)
+        bit_count = data_info.bit_count
+        bit_offset = data_info.bit_offset % 16
+
+        if bit_offset:
+            mask_prefix_size = bit_offset
+            mask_suffix_size = max(16 - bit_offset - bit_count, 0)
+            mask_size = 16 - mask_prefix_size - mask_suffix_size
+            and_mask = (((0xFFFF << (16 - mask_prefix_size)) & 0xFFFF) |
+                        ((0xFFFF << mask_suffix_size) >> 16))
+            or_mask = (((value >> (bit_count - mask_size)) &
+                        ((1 << mask_size) - 1)) <<
+                       mask_suffix_size)
+            result = await self._conn.write_mask(device_id=self._device_id,
+                                                 address=address,
+                                                 and_mask=and_mask,
+                                                 or_mask=or_mask)
+            if result:
+                return result
+            address += 1
+            bit_count -= mask_size
 
-        self._async_group.spawn(aio.call_on_cancel, self._eval_status)
-        self._eval_status()
+        register_count = bit_count // 16
+        if register_count:
+            registers = [(value >> (bit_count - 16 * (i + 1))) & 0xFFFF
+                         for i in range(register_count)]
+            result = await self._conn.write(device_id=self._device_id,
+                                            data_type=data_info.data_type,
+                                            start_address=address,
+                                            values=registers)
+            if result:
+                return result
+            address += register_count
+            bit_count -= 16 * register_count
 
-    @property
-    def async_group(self) -> aio.Group:
-        return self._async_group
+        if not bit_count:
+            return
 
-    def _on_response(self, res):
-        self._response_cb(res)
-        self._eval_status()
-
-    def _eval_status(self):
-        if not self.is_open:
-            status = 'DISABLED'
-        elif all(i.is_connected for i in self._data_readers):
-            status = 'CONNECTED'
-        else:
-            status = 'CONNECTING'
+        and_mask = (0xFFFF << (16 - bit_count)) >> 16
+        or_mask = (value & ((1 << bit_count) - 1)) << (16 - bit_count)
+        return await self._conn.write_mask(device_id=self._device_id,
+                                           address=address,
+                                           and_mask=and_mask,
+                                           or_mask=or_mask)
 
-        if self._status == status:
+    def _log(self, level, msg, *args, **kwargs):
+        if not mlog.isEnabledFor(level):
             return
 
-        mlog.debug('changing remote device status: %s -> %s', self._status,
-                   status)
-        self._status = status
-        self._response_cb(RemoteDeviceStatusRes(device_id=self._device_id,
-                                                status=status))
+        mlog.log(level, f"{self._log_prefix}: {msg}", *args, **kwargs)
 
 
-class Data:
+class _Reader(aio.Resource):
 
-    def __init__(self,
-                 conf: json.Data,
-                 device_id: int,
-                 conn: Connection):
-        self._device_id = device_id
+    def __init__(self, conn, device_id, timeout_poll_delay, data_groups,
+                 response_cb, log_prefix):
         self._conn = conn
-        self._data_type = DataType[conf['data_type']]
-        self._register_size = _get_register_size(self._data_type)
-        self._start_address = conf['start_address']
-        self._bit_count = conf['bit_count']
-        self._bit_offset = conf['bit_offset']
-        self._quantity = math.ceil((self._bit_count + self._bit_offset) /
-                                   self._register_size)
-        self._interval = conf['interval']
-        self._name = conf['name']
+        self._device_id = device_id
+        self._timeout_poll_delay = timeout_poll_delay
+        self._response_cb = response_cb
+        self._log_prefix = log_prefix
+        self._status = None
+        self._async_group = conn.async_group.create_subgroup()
 
-    @property
-    def device_id(self) -> int:
-        return self._device_id
+        self.async_group.spawn(self._read_loop, data_groups)
 
     @property
-    def conn(self) -> Connection:
-        return self._conn
+    def async_group(self) -> aio.Group:
+        return self._async_group
 
-    @property
-    def data_type(self) -> DataType:
-        return self._data_type
+    async def _read_loop(self, data_groups):
+        try:
+            self._log(logging.DEBUG, 'starting read loop')
+            loop = asyncio.get_running_loop()
 
-    @property
-    def register_size(self) -> int:
-        return self._register_size
+            if not data_groups:
+                await self._set_status(_Status.CONNECTED)
+                await loop.create_future()
+
+            last_read_times = [None for _ in data_groups]
+            last_responses = {}
+            await self._set_status(_Status.CONNECTING)
 
-    @property
-    def start_address(self) -> int:
-        return self._start_address
+            while True:
+                now = time.monotonic()
+                sleep_dt = None
+                read_data_groups = collections.deque()
+
+                for i, data_group in enumerate(data_groups):
+                    last_read_time = last_read_times[i]
+                    if last_read_time is not None:
+                        dt = data_group.interval - now + last_read_time
+                        if dt > 0:
+                            if sleep_dt is None or dt < sleep_dt:
+                                sleep_dt = dt
+                            continue
+
+                    read_data_groups.append(data_group)
+                    last_read_times[i] = now
+
+                if not read_data_groups:
+                    await asyncio.sleep(sleep_dt)
+                    continue
+
+                timeout = False
+
+                self._log(logging.DEBUG, 'reading data')
+                for data_group in read_data_groups:
+                    result = await self._conn.read(
+                        device_id=self._device_id,
+                        data_type=data_group.data_type,
+                        start_address=data_group.start_address,
+                        quantity=data_group.quantity)
+
+                    if isinstance(result, Error) and result.name == 'TIMEOUT':
+                        timeout = True
+                        break
+
+                    for data_info in data_group.data_infos:
+                        last_response = last_responses.get(data_info.name)
+
+                        response = self._process_read_result(
+                            data_info, data_group.start_address,
+                            result, last_response)
+
+                        if response:
+                            last_responses[data_info.name] = response
+                            await aio.call(self._response_cb, response)
+
+                if timeout:
+                    await self._set_status(_Status.DISCONNECTED)
+                    await asyncio.sleep(self._timeout_poll_delay)
+
+                    last_read_times = [None for _ in data_groups]
+                    last_responses = {}
+                    await self._set_status(_Status.CONNECTING)
 
-    @property
-    def bit_count(self) -> int:
-        return self._bit_count
+                elif all(t is not None for t in last_read_times):
+                    await self._set_status(_Status.CONNECTED)
 
-    @property
-    def bit_offset(self) -> int:
-        return self._bit_offset
+        except ConnectionError:
+            self._log(logging.DEBUG, 'connection closed')
 
-    @property
-    def quantity(self) -> int:
-        return self._quantity
+        except Exception as e:
+            self._log(logging.ERROR, 'read loop error: %s', e, exc_info=e)
 
-    @property
-    def interval(self) -> typing.Optional[float]:
-        return self._interval
+        finally:
+            self._log(logging.DEBUG, 'closing read loop')
+            self.close()
 
-    @property
-    def name(self) -> str:
-        return self._name
+            with contextlib.suppress(Exception):
+                await aio.uncancellable(self._set_status(_Status.DISABLED))
 
-    async def write(self, value: int) -> typing.Optional[Error]:
-        if self._data_type == DataType.COIL:
-            address = self._start_address + self._bit_offset
-            registers = [(value >> (self._bit_count - i - 1)) & 1
-                         for i in range(self._bit_count)]
-            result = await self._conn.write(self._device_id, self._data_type,
-                                            address, registers)
-            return result
-
-        elif self._data_type == DataType.HOLDING_REGISTER:
-            address = self._start_address + (self._bit_offset // 16)
-            bit_count = self._bit_count
-            bit_offset = self._bit_offset % 16
-
-            if bit_offset:
-                mask_prefix_size = bit_offset
-                mask_suffix_size = max(16 - bit_offset - bit_count, 0)
-                mask_size = 16 - mask_prefix_size - mask_suffix_size
-                and_mask = (((0xFFFF << (16 - mask_prefix_size)) & 0xFFFF) |
-                            ((0xFFFF << mask_suffix_size) >> 16))
-                or_mask = (((value >> (bit_count - mask_size)) &
-                            ((1 << mask_size) - 1)) <<
-                           mask_suffix_size)
-                result = await self._conn.write_mask(self._device_id, address,
-                                                     and_mask, or_mask)
-                if result:
-                    return result
-                address += 1
-                bit_count -= mask_size
-
-            register_count = bit_count // 16
-            if register_count:
-                registers = [(value >> (bit_count - 16 * (i + 1))) & 0xFFFF
-                             for i in range(register_count)]
-                result = await self._conn.write(self._device_id,
-                                                self._data_type,
-                                                address, registers)
-                if result:
-                    return result
-                address += register_count
-                bit_count -= 16 * register_count
-
-            if bit_count:
-                and_mask = (0xFFFF << (16 - bit_count)) >> 16
-                or_mask = (value & ((1 << bit_count) - 1)) << (16 - bit_count)
-                result = await self._conn.write_mask(self._device_id, address,
-                                                     and_mask, or_mask)
-                return result
+    def _process_read_result(self, data_info, start_address, result,
+                             last_response):
+        if isinstance(result, Error):
+            self._log(logging.DEBUG, 'data name %s: error response %s',
+                      data_info.name, result)
+            return RemoteDeviceReadRes(device_id=self._device_id,
+                                       data_name=data_info.name,
+                                       result=result.name,
+                                       value=None,
+                                       cause=None)
+
+        offset = data_info.start_address - start_address
+        value = _get_registers_value(
+            data_info.register_size, data_info.bit_offset,
+            data_info.bit_count,
+            result[offset:offset+data_info.quantity])
+
+        if last_response is None or last_response.result != 'SUCCESS':
+            self._log(logging.DEBUG, 'data name %s: initial value %s',
+                      data_info.name, value)
+            return RemoteDeviceReadRes(device_id=self._device_id,
+                                       data_name=data_info.name,
+                                       result='SUCCESS',
+                                       value=value,
+                                       cause='INTERROGATE')
+
+        if last_response.value != value:
+            self._log(logging.DEBUG, 'data name %s: value change %s -> %s',
+                      data_info.name, last_response.value, value)
+            return RemoteDeviceReadRes(device_id=self._device_id,
+                                       data_name=data_info.name,
+                                       result='SUCCESS',
+                                       value=value,
+                                       cause='CHANGE')
+
+        self._log(logging.DEBUG, 'data name %s: no value change',
+                  data_info.name)
 
+    async def _set_status(self, status):
+        if self._status == status:
             return
 
-        raise Exception(f'write unsupported for {self._data_type}')
+        self._log(logging.DEBUG, 'changing remote device status %s -> %s',
+                  self._status, status)
+        self._status = status
 
-    async def read(self) -> typing.Union[int, Error]:
-        result = await self._conn.read(self._device_id, self._data_type,
-                                       self._start_address, self._quantity)
-        if isinstance(result, Error):
-            return result
-        return _get_registers_value(self._register_size, self._bit_offset,
-                                    self._bit_count, result)
+        res = RemoteDeviceStatusRes(device_id=self._device_id,
+                                    status=status.name)
+        await aio.call(self._response_cb, res)
 
+    def _log(self, level, msg, *args, **kwargs):
+        if not mlog.isEnabledFor(level):
+            return
 
-class _DataReader(aio.Resource):
+        mlog.log(level, f"{self._log_prefix}: {msg}", *args, **kwargs)
 
-    def __init__(self,
-                 async_group: aio.Group,
-                 conn: Connection,
-                 data: typing.List[Data],
-                 device_id: int,
-                 data_type: DataType,
-                 start_address: int,
-                 quantity: int,
-                 interval: float,
-                 response_cb: ResponseCb):
-        self._async_group = async_group
-        self._conn = conn
-        self._data = data
-        self._device_id = device_id
-        self._data_type = data_type
-        self._start_address = start_address
-        self._quantity = quantity
-        self._interval = interval
-        self._response_cb = response_cb
-        self._is_connected = False
 
-        async_group.spawn(self._read_loop)
+def _get_data_infos(conf):
+    for i in conf['data']:
+        data_type = DataType[i['data_type']]
+        register_size = _get_register_size(data_type)
+        bit_count = i['bit_count']
+        bit_offset = i['bit_offset']
 
-    @property
-    def async_group(self):
-        return self._async_group
+        yield _DataInfo(
+            data_type=data_type,
+            register_size=register_size,
+            start_address=i['start_address'],
+            bit_count=bit_count,
+            bit_offset=bit_offset,
+            quantity=math.ceil((bit_count + bit_offset) / register_size),
+            interval=i['interval'],
+            name=i['name'])
 
-    @property
-    def is_connected(self):
-        return self._is_connected
 
-    async def _read_loop(self):
-        try:
-            mlog.debug('starting read loop')
-            last_responses = {data: None for data in self._data}
+def _group_data_infos(data_infos):
+    type_interval_infos_dict = collections.defaultdict(
+        functools.partial(collections.defaultdict, collections.deque))
 
-            while True:
-                mlog.debug('reading data')
-                result = await self._conn.read(
-                    self._device_id, self._data_type, self._start_address,
-                    self._quantity)
-                mlog.debug('received response (device_id: %s; data_type: %s; '
-                           'start_address: %s; quantity: %s): %s',
-                           self._device_id, self._data_type,
-                           self._start_address, self._quantity, result)
-
-                self._is_connected = not (isinstance(result, Error) and
-                                          result.name == 'TIMEOUT')
-
-                for data in self._data:
-                    last_response = last_responses[data]
-
-                    if isinstance(result, Error):
-                        value = None
-
-                    else:
-                        offset = data.start_address - self._start_address
-                        value = _get_registers_value(
-                            data.register_size, data.bit_offset,
-                            data.bit_count,
-                            result[offset:offset+data.quantity])
-
-                    if isinstance(result, Error):
-                        mlog.debug('received error response (device_id: %s; '
-                                   'data_name: %s): %s',
-                                   data.device_id, data.name, result)
-                        response = _create_read_response(
-                            data, result.name, None, None)
-
-                    elif (last_response is None or
-                            last_response.result != 'SUCCESS'):
-                        mlog.debug('received initial value (device_id: %s; '
-                                   'data_name: %s): %s',
-                                   data.device_id, data.name, value)
-                        response = _create_read_response(
-                            data, 'SUCCESS', value, 'INTERROGATE')
-
-                    elif last_response.value != value:
-                        mlog.debug('data value change value (device_id: %s; '
-                                   'data_name: %s): %s -> %s',
-                                   data.device_id, data.name,
-                                   last_response.value, value)
-                        response = _create_read_response(
-                            data, 'SUCCESS', value, 'CHANGE')
-
-                    else:
-                        mlog.debug('no data change')
-                        response = None
-
-                    if response:
-                        last_responses[data] = response
-                        self._response_cb(response)
+    for data_info in data_infos:
+        data_type = data_info.data_type
+        interval = data_info.interval
 
-                mlog.debug('waiting poll interval: %s', self._interval)
-                await asyncio.sleep(self._interval)
+        if interval is None:
+            continue
 
-        except ConnectionError:
-            mlog.debug('connection closed')
+        type_interval_infos_dict[data_type][interval].append(data_info)
 
-        except Exception as e:
-            mlog.error('read loop error: %s', e, exc_info=e)
+    for data_type, interval_infos_dict in type_interval_infos_dict.items():
+        for interval, data_infos_queue in interval_infos_dict.items():
+            yield from _group_data_infos_with_type_interval(
+                data_infos_queue, data_type, interval)
 
-        finally:
-            mlog.debug('closing read loop')
-            self.close()
 
+def _group_data_infos_with_type_interval(data_infos, data_type, interval):
+    data_infos_queue = sorted(data_infos,
+                              key=lambda i: (i.start_address, i.quantity))
+    data_infos_queue = collections.deque(data_infos_queue)
+
+    while data_infos_queue:
+        max_quantity = _get_max_quantity(data_type)
+        start_address = None
+        quantity = None
+        data_infos = collections.deque()
+
+        while data_infos_queue:
+            data_info = data_infos_queue.popleft()
+
+            if start_address is None:
+                start_address = data_info.start_address
+
+            if quantity is None:
+                quantity = data_info.quantity
+
+            elif data_info.start_address > start_address + quantity:
+                data_infos_queue.appendleft(data_info)
+                break
+
+            else:
+                new_quantity = (data_info.quantity +
+                                data_info.start_address -
+                                start_address)
+
+                if new_quantity > max_quantity:
+                    data_infos_queue.appendleft(data_info)
+                    break
+
+                if new_quantity > quantity:
+                    quantity = new_quantity
+
+            data_infos.append(data_info)
 
-def _create_read_response(data, result, value, cause):
-    return RemoteDeviceReadRes(
-        device_id=data.device_id,
-        data_name=data.name,
-        result=result,
-        value=value,
-        cause=cause)
+        if start_address is None or quantity is None:
+            continue
+
+        yield _DataGroup(data_infos=data_infos,
+                         interval=interval,
+                         data_type=data_type,
+                         start_address=start_address,
+                         quantity=quantity)
 
 
 def _get_register_size(data_type):
     if data_type in (DataType.COIL,
                      DataType.DISCRETE_INPUT):
         return 1
 
@@ -347,14 +424,29 @@
                      DataType.INPUT_REGISTER,
                      DataType.QUEUE):
         return 16
 
     raise ValueError('invalid data type')
 
 
+def _get_max_quantity(data_type):
+    if data_type in (DataType.COIL,
+                     DataType.DISCRETE_INPUT):
+        return 2000
+
+    if data_type in (DataType.HOLDING_REGISTER,
+                     DataType.INPUT_REGISTER):
+        return 125
+
+    if data_type == DataType.QUEUE:
+        return 1
+
+    raise ValueError('invalid data type')
+
+
 def _get_registers_value(register_size, bit_offset, bit_count, values):
     result = 0
     bits = itertools.chain(_get_registers_bits(register_size, values),
                            itertools.repeat(0))
     for i in itertools.islice(bits, bit_offset, bit_offset + bit_count):
         result = (result << 1) | i
     return result
```

## Comparing `hat/gateway/devices/modbus/master/event_client.py` & `hat/gateway/devices/modbus/master/eventer_client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+from collections.abc import Collection, Iterable
+import contextlib
 import logging
 import typing
 
 from hat import aio
-from hat.gateway import common
 import hat.event.common
+import hat.event.eventer
+
+from hat.gateway import common
 
 
 mlog = logging.getLogger(__name__)
 
 
 class RemoteDeviceEnableReq(typing.NamedTuple):
     device_id: int
@@ -17,16 +21,15 @@
 class RemoteDeviceWriteReq(typing.NamedTuple):
     device_id: int
     data_name: str
     request_id: str
     value: int
 
 
-Request = typing.Union[RemoteDeviceEnableReq,
-                       RemoteDeviceWriteReq]
+Request: typing.TypeAlias = RemoteDeviceEnableReq | RemoteDeviceWriteReq
 
 
 class StatusRes(typing.NamedTuple):
     status: str
 
 
 class RemoteDeviceStatusRes(typing.NamedTuple):
@@ -34,88 +37,93 @@
     status: str
 
 
 class RemoteDeviceReadRes(typing.NamedTuple):
     device_id: int
     data_name: str
     result: str
-    value: typing.Optional[int]
-    cause: typing.Optional[str]
+    value: int | None
+    cause: str | None
 
 
 class RemoteDeviceWriteRes(typing.NamedTuple):
     device_id: int
     data_name: str
     request_id: str
     result: str
 
 
-Response = typing.Union[StatusRes,
-                        RemoteDeviceStatusRes,
-                        RemoteDeviceReadRes,
-                        RemoteDeviceWriteRes]
+Response: typing.TypeAlias = (StatusRes |
+                              RemoteDeviceStatusRes |
+                              RemoteDeviceReadRes |
+                              RemoteDeviceWriteRes)
 
 
-class EventClientProxy(aio.Resource):
+class EventerClientProxy(aio.Resource):
 
     def __init__(self,
-                 event_client: common.DeviceEventClient,
-                 event_type_prefix: common.EventTypePrefix):
-        self._event_client = event_client
+                 eventer_client: hat.event.eventer.Client,
+                 event_type_prefix: common.EventTypePrefix,
+                 log_prefix: str):
+        self._eventer_client = eventer_client
         self._event_type_prefix = event_type_prefix
-        self._async_group = event_client.async_group.create_subgroup()
-        self._read_queue = aio.Queue()
-        self.async_group.spawn(self._read_loop)
+        self._log_prefix = log_prefix
 
     @property
     def async_group(self) -> aio.Group:
-        return self._async_group
+        return self._eventer_client.async_group
+
+    def process_events(self,
+                       events: Collection[hat.event.common.Event]
+                       ) -> Iterable[Request]:
+        self._log(logging.DEBUG, 'received %s events', len(events))
+        for event in events:
+            try:
+                yield _request_from_event(event)
+
+            except Exception as e:
+                self._log(logging.INFO, 'received invalid event: %s', e,
+                          exc_info=e)
+
+    async def write(self, responses: Iterable[Response]):
+        events = [_response_to_register_event(self._event_type_prefix, i)
+                  for i in responses]
+        await self._eventer_client.register(events)
+
+    async def query_enabled_devices(self) -> set[int]:
+        self._log(logging.DEBUG, 'querying enabled devices')
+        enabled_devices = set()
+
+        event_type = (*self._event_type_prefix, 'system', 'remote_device',
+                      '?', 'enable')
+        params = hat.event.common.QueryLatestParams([event_type])
+        result = await self._eventer_client.query(params)
+        self._log(logging.DEBUG, 'received %s events', len(result.events))
+
+        for event in result.events:
+            if not event.payload or not bool(event.payload.data):
+                continue
+
+            device_id_str = event.type[6]
+            with contextlib.suppress(ValueError):
+                enabled_devices.add(int(device_id_str))
+
+        self._log(logging.DEBUG, 'detected %s enabled devices',
+                  len(enabled_devices))
+        return enabled_devices
+
+    def _log(self, level, msg, *args, **kwargs):
+        if not mlog.isEnabledFor(level):
+            return
 
-    def write(self, responses: typing.List[Response]):
-        register_events = [
-            _response_to_register_event(self._event_type_prefix, i)
-            for i in responses]
-        self._event_client.register(register_events)
-
-    async def read(self) -> Request:
-        try:
-            return await self._read_queue.get()
-
-        except aio.QueueClosedError:
-            raise ConnectionError()
-
-    async def _read_loop(self):
-        try:
-            mlog.debug('starting read loop')
-            while True:
-                events = await self._event_client.receive()
-                mlog.debug('received %s events', len(events))
-
-                for event in events:
-                    try:
-                        req = _request_from_event(event)
-                        self._read_queue.put_nowait(req)
-
-                    except Exception as e:
-                        mlog.info('received invalid event: %s', e, exc_info=e)
-
-        except ConnectionError:
-            mlog.debug('connection closed')
-
-        except Exception as e:
-            mlog.error('read loop error: %s', e, exc_info=e)
-
-        finally:
-            mlog.debug('closing read loop')
-            self.close()
-            self._read_queue.close()
+        mlog.log(level, f"{self._log_prefix}: {msg}", *args, **kwargs)
 
 
 def _request_from_event(event):
-    event_type_suffix = event.event_type[5:]
+    event_type_suffix = event.type[5:]
 
     if event_type_suffix[0] != 'remote_device':
         raise Exception('unsupported event type')
 
     device_id = int(event_type_suffix[1])
 
     if event_type_suffix[2] == 'enable':
@@ -160,12 +168,10 @@
         payload = {'request_id': res.request_id,
                    'result': res.result}
 
     else:
         raise ValueError('invalid response type')
 
     return hat.event.common.RegisterEvent(
-        event_type=event_type,
+        type=event_type,
         source_timestamp=None,
-        payload=hat.event.common.EventPayload(
-            type=hat.event.common.EventPayloadType.JSON,
-            data=payload))
+        payload=hat.event.common.EventPayloadJson(payload))
```

## Comparing `hat_gateway-0.5.9.dist-info/LICENSE` & `hat_gateway-0.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hat_gateway-0.5.9.dist-info/METADATA` & `hat_gateway-0.6.0.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,107 @@
 Metadata-Version: 2.1
 Name: hat-gateway
-Version: 0.5.9
+Version: 0.6.0
 Summary: Hat gateway
-Home-page: https://github.com/hat-open/hat-gateway
-License: Apache-2.0
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: appdirs (~=1.4.4)
-Requires-Dist: click (~=8.0.1)
-Requires-Dist: hat-aio (>=0.5.1)
-Requires-Dist: hat-chatter (>=0.5.1)
-Requires-Dist: hat-drivers (>=0.5.1)
-Requires-Dist: hat-event (~=0.6.2)
-Requires-Dist: hat-json (>=0.5.2)
-Requires-Dist: hat-monitor (>=0.5.1)
-Requires-Dist: hat-sbs (>=0.5.1)
-Requires-Dist: hat-util (>=0.5.4)
+License: Apache-2.0
+Provides-Extra: dev
+Requires-Dist: appdirs ~=1.4.4
+Requires-Dist: cryptography >=3.3.2
+Requires-Dist: hat-aio ~=0.7.9
+Requires-Dist: hat-drivers ~=0.7.10
+Requires-Dist: hat-event ~=0.9.0
+Requires-Dist: hat-json ~=0.5.26
+Requires-Dist: hat-monitor ~=0.8.5
+Requires-Dist: hat-util ~=0.6.13
+Requires-Dist: hat-doit ~=0.15.11; extra == 'dev'
+Requires-Dist: psutil >=5.9.8; extra == 'dev'
+Requires-Dist: sphinxcontrib-plantuml >=0.27; extra == 'dev'
+Requires-Dist: sphinxcontrib-programoutput >=0.17; extra == 'dev'
+Requires-Python: >=3.10
+Project-URL: Homepage, http://hat-open.com
+Project-URL: Repository, https://github.com/hat-open/hat-gateway.git
+Project-URL: Documentation, http://hat-gateway.hat-open.com
+
+.. _online documentation: https://hat-gateway.hat-open.com
+.. _git repository: https://github.com/hat-open/hat-gateway.git
+.. _PyPI project: https://pypi.org/project/hat-gateway
+.. _pydoit: https://pydoit.org
+.. _Hat Open: https://hat-open.com
+.. _Končar Digital: https://www.koncar.hr/en
+
 
 hat-gateway - Communication gateway
 ===================================
 
-This component is part of Hat Open project - open-source framework of tools and
-libraries for developing applications used for remote monitoring, control and
-management of intelligent electronic devices such as IoT devices, PLCs,
-industrial automation or home automation systems.
-
-Development of Hat Open and associated repositories is sponsored by
-Končar - Power Plant and Electric Traction Engineering Inc.
-(Končar KET - `<https://www.koncar-ket.hr>`_).
-
 For more information see:
 
-    * hat-gateway documentation - `<https://hat-gateway.hat-open.com>`_
-    * hat-gateway git repository - `<https://github.com/hat-open/hat-gateway.git>`_
-    * Hat Open homepage - `<https://hat-open.com>`_
+* `online documentation`_
+* `git repository`_
 
-.. warning::
 
-    This project is currently in state of active development. Features,
-    functionality and API are unstable.
+Runtime requirements
+--------------------
+
+* python >=3.10
 
 
 Install
 -------
 
-::
+`hat-gateway` is available as `PyPI project`_::
 
     $ pip install hat-gateway
 
 
+Build
+-----
+
+To install editable installation, together with python development
+dependencies, run::
+
+    $ pip install -e '.[dev]'
+
+To install only python development dependencies, run::
+
+    $ pip install -r requirements.pip.txt
+
+Build tool used for `hat-gateway` is `pydoit`_. For listing available doit
+tasks, use::
+
+    $ doit list
+
+Default task::
+
+    $ doit
+
+creates wheel package inside `build` directory.
+
+
+Hat Open
+--------
+
+`hat-gateway` is part of `Hat Open`_ project - open-source framework of
+tools and libraries for developing applications used for remote monitoring,
+control and management of intelligent electronic devices such as IoT devices,
+PLCs, industrial automation or home automation systems.
+
+Development of Hat Open and associated repositories is sponsored by
+`Končar Digital`_.
+
+
 License
 -------
 
-Copyright 2020-2021 Hat Open AUTHORS
+Copyright 2020-2024 Hat Open AUTHORS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
-
```

## Comparing `hat_gateway-0.5.9.dist-info/RECORD` & `hat_gateway-0.6.0.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,32 @@
-hat/gateway/__init__.py,sha256=vuNOQ_jKGdSIKdmWWpMvCgT0LjO-QJexse1ll3mQcKM,14
-hat/gateway/__main__.py,sha256=5Zfrpb9VC6maLavrF6TYOPhr5ZkjE6wRIia7GiolzFI,128
-hat/gateway/common.py,sha256=BbHLmjWraiaS-nXnBEt0ofMG2cLoZ17FlY97AYwSh2M,2615
-hat/gateway/engine.py,sha256=h10osV4M4HxbQKlOydSFBB04VWqmAo14YaSJgARDv1Q,7801
-hat/gateway/json_schema_repo.json,sha256=4irC2uzEJfYLaAqfdcGL1nMqRxV1Qcmo6MWpZW9336A,4801
-hat/gateway/main.py,sha256=IOSd4_5TPRmVQuMZlwMGjnrCC_BAVPm7A8jTk0E-VYM,3728
 hat/gateway/devices/__init__.py,sha256=bUTqbQdM8I9F9P-5OeD47kNlvVgC0zG27UYJPYg3srw,22
+hat/gateway/devices/iec101/slave.py,sha256=GoVstBvVD7C1GoKZQ1LL1Wusi_xF4uKF0XNcroVbZIQ,17668
+hat/gateway/devices/iec103/__init__.py,sha256=eESWgb-0qevhIyxgprW4nqjV9HtSHF5so-N3EXbnlRw,30
+hat/gateway/common.py,sha256=9o3tP3pXG0_qp7KKo0QSTxRLVBVDvn8T-qnoDl0JXu8,2405
+hat/gateway/devices/iec101/master.py,sha256=eL8h1e16fYzizyWdaygNc-YKPwmIpHZWgZVVwA37nVc,19355
+hat/gateway/devices/modbus/master/remote_device.py,sha256=4KZHbyi1RzHVBEgXSYG2mJtz78WrAEjfn9mdU6ub5yg,16472
+hat/gateway/devices/modbus/master/connection.py,sha256=F6f55Z0UHTV4Ean8yAQVI7EpZtzmaLiw9uCwZiEBz0I,8067
+hat/gateway/devices/iec104/__init__.py,sha256=Kr52XUBE9Ks5LZRXxz6E-auvK8VgGapdSUj_zF9E_fQ,30
 hat/gateway/devices/modbus/__init__.py,sha256=uONGhCvVvD1gP07Vf2KLqLNbDWsaGaHm9SZRL241_Dc,21
-hat/gateway/devices/modbus/master/__init__.py,sha256=LNuZz0hSI9F5jLQwKzSB41xJZcb7gVV_NcpOeOe5xMU,353
-hat/gateway/devices/modbus/master/connection.py,sha256=jywuNeRwUbRBcRr3lRJ5Wuc9ZNI5TzuI6m7JYHxN6fA,5843
-hat/gateway/devices/modbus/master/device.py,sha256=gQ8Lmw_-vLGtwQwzGTkfSSQoZ7LNYraqRloAT17WB5A,8408
-hat/gateway/devices/modbus/master/event_client.py,sha256=vEQXJ0R5OCwrLs5C8ulM8xsAOm60UffuiZtGnrGosEI,5007
-hat/gateway/devices/modbus/master/remote_device.py,sha256=5IiNwDkms4mV9nwkmLIYM-bbWJ1raZ1_a-I2ikMKfzs,12777
-hat_gateway-0.5.9.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-hat_gateway-0.5.9.dist-info/METADATA,sha256=dGIGi7jjS5gWwIxEeoX578zr5h-Uw1gn9oJy76pZsIk,2232
-hat_gateway-0.5.9.dist-info/WHEEL,sha256=0r8MCP1NVHT-mKGu5LgjJWwiuNvYPN3jw2sVhuFc1nc,112
-hat_gateway-0.5.9.dist-info/entry_points.txt,sha256=79AsAZGTl0THv4jP9B7uKVdhXNFh76ILoyaXfG1wvE8,71
-hat_gateway-0.5.9.dist-info/top_level.txt,sha256=3RuRoRsaXQZNKwr3T2RE9XepBRTk4YpnXUbMiH5nes8,4
-hat_gateway-0.5.9.dist-info/RECORD,,
+hat/gateway/devices/snmp/manager.py,sha256=FER3aqFO-yqBxBhpmoft2B8UKuyKNVOr7LfWjZEn4OI,10349
+hat/gateway/devices/modbus/master/__init__.py,sha256=NkIYsRjZ68o4qmGtUEGVdmW78f8QIfANRpv9bGbuaos,349
+hat/gateway/__init__.py,sha256=vuNOQ_jKGdSIKdmWWpMvCgT0LjO-QJexse1ll3mQcKM,14
+hat/gateway/devices/iec103/master.py,sha256=TVR-q4Bzr5lr2om4cptqKZtfg4kQYjuvY7LeqRkAq-k,15260
+hat/gateway/devices/modbus/master/eventer_client.py,sha256=vV78SlnRfCQw9KqZDkqJI8UEEBg2QnFwkZRB2ci8SL0,5434
+hat/gateway/devices/iec101/common.py,sha256=qoBB7fp9xtJpykic4cdCSEbm95kidA1XkoyxGChSjgw,16277
+hat/gateway/engine.py,sha256=LGApmAMW78vWP34J9vcFtEvlRj9KtTRyYDU_GcmkJjM,7162
+hat/gateway/devices/iec104/slave.py,sha256=TXTgDx-QopBz7K3I9V8xRdPWtcpC1whAODrmkNtq1QY,14768
+hat/gateway/json_schema_repo.json,sha256=W16FNUqyr0y6R_S1gxSInYxAr88kCpsosCunE7x92E0,33538
+hat/gateway/devices/iec101/__init__.py,sha256=9gkje8fhWD8ISFkPyPf_I8UlpUaA9i3yqH7ByhMd2IM,30
+hat/gateway/__main__.py,sha256=5Zfrpb9VC6maLavrF6TYOPhr5ZkjE6wRIia7GiolzFI,128
+hat/gateway/devices/modbus/master/device.py,sha256=znw47mDgChz96gvya44txQA6jhhooBz2B5o3Wlbq9_4,7864
+hat/gateway/devices/iec104/master.py,sha256=E5R8GY9croNZxD8Jq2Ay9cDxGsPwM8TGr_kJbB9pkkg,13561
+hat/gateway/devices/iec104/ssl.py,sha256=TF60PvhNM847TAqFaJB2NQ15goquQBo4_RGkoNu6p1U,4251
+hat/gateway/runner.py,sha256=kbEqYn4OYMRAW8-alLofvV0uRloyhuJ7Z4hOla7zd_Y,3973
+hat/gateway/devices/iec104/common.py,sha256=_pOe4bZ_fdACUDApaLm4Ff_URfvyBZbJ5JbIms5Sy3Y,56
+hat/gateway/main.py,sha256=DMsqaVoPgcraj_WP2zOULZ0y29jndAqGbEcFlpix5gw,1991
+hat/gateway/devices/snmp/__init__.py,sha256=VxObCQT37feiEdRN4Dsytv3ZaSCgWRLg-egFNfaKm4E,19
+hat_gateway-0.6.0.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+hat_gateway-0.6.0.dist-info/entry_points.txt,sha256=pTfcSj53hqfPE3NE7NIquXiNNY2qw4mvZ-4kI9H370k,54
+hat_gateway-0.6.0.dist-info/METADATA,sha256=hpekXa9OBN422EAGmGeU7L2bQt9VFIHL9czX2V6zrCU,2826
+hat_gateway-0.6.0.dist-info/WHEEL,sha256=jZazLaBxpUW5RTRFGTDEenHxZxNK0hI9pc4G7DVP3Ws,118
+hat_gateway-0.6.0.dist-info/RECORD,,
```

