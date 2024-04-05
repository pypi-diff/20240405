# Comparing `tmp/aioairzone-cloud-0.4.7.tar.gz` & `tmp/aioairzone-cloud-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioairzone-cloud-0.4.7.tar", last modified: Wed Apr  3 16:39:10 2024, max compression
+gzip compressed data, was "aioairzone-cloud-0.5.0.tar", last modified: Fri Apr  5 08:22:11 2024, max compression
```

## Comparing `aioairzone-cloud-0.4.7.tar` & `aioairzone-cloud-0.5.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2024-04-03 16:39:10.896730 aioairzone-cloud-0.4.7/
--rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2023-12-27 17:30:29.000000 aioairzone-cloud-0.4.7/LICENSE
--rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2023-12-27 17:30:29.000000 aioairzone-cloud-0.4.7/MANIFEST.in
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1551 2024-04-03 16:39:10.896730 aioairzone-cloud-0.4.7/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      746 2023-12-27 17:30:29.000000 aioairzone-cloud-0.4.7/README.md
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2024-04-03 16:39:10.896730 aioairzone-cloud-0.4.7/aioairzone_cloud/
--rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2023-12-27 17:30:29.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/__init__.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     3306 2024-04-03 16:34:41.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/aidoo.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    30073 2024-04-03 16:04:15.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/cloudapi.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2777 2024-04-03 16:28:32.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/common.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     9556 2024-02-28 17:57:26.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/const.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     8796 2024-04-03 16:34:41.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/device.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    10924 2024-02-28 08:54:11.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/device_group.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     3081 2024-02-28 14:34:38.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/entity.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      807 2024-02-28 08:54:11.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/exceptions.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      925 2024-04-03 16:08:52.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/group.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    25143 2024-04-03 16:34:41.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/hvac.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1821 2024-04-03 16:08:59.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/installation.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2023-12-27 17:30:29.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/py.typed
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1463 2024-04-03 16:09:19.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/system.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2495 2024-02-28 12:49:43.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/token.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     5948 2024-04-03 16:34:41.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/webserver.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     8581 2024-04-03 16:04:15.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/websockets.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     3483 2024-04-03 16:34:41.000000 aioairzone-cloud-0.4.7/aioairzone_cloud/zone.py
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2024-04-03 16:39:10.896730 aioairzone-cloud-0.4.7/aioairzone_cloud.egg-info/
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1551 2024-04-03 16:39:10.000000 aioairzone-cloud-0.4.7/aioairzone_cloud.egg-info/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      803 2024-04-03 16:39:10.000000 aioairzone-cloud-0.4.7/aioairzone_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2024-04-03 16:39:10.000000 aioairzone-cloud-0.4.7/aioairzone_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2024-04-03 16:39:10.000000 aioairzone-cloud-0.4.7/aioairzone_cloud.egg-info/not-zip-safe
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2024-04-03 16:39:10.000000 aioairzone-cloud-0.4.7/aioairzone_cloud.egg-info/requires.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2024-04-03 16:39:10.000000 aioairzone-cloud-0.4.7/aioairzone_cloud.egg-info/top_level.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2327 2024-04-03 16:35:39.000000 aioairzone-cloud-0.4.7/pyproject.toml
--rw-r--r--   0 noltari   (1000) noltari   (1000)       77 2023-12-27 17:30:29.000000 aioairzone-cloud-0.4.7/requirements.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)       38 2024-04-03 16:39:10.896730 aioairzone-cloud-0.4.7/setup.cfg
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2024-04-05 08:22:11.442738 aioairzone-cloud-0.5.0/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2024-01-05 18:10:25.000000 aioairzone-cloud-0.5.0/LICENSE
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2024-01-05 18:10:25.000000 aioairzone-cloud-0.5.0/MANIFEST.in
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1551 2024-04-05 08:22:11.442738 aioairzone-cloud-0.5.0/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      746 2024-01-05 18:10:25.000000 aioairzone-cloud-0.5.0/README.md
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2024-04-05 08:22:11.442738 aioairzone-cloud-0.5.0/aioairzone_cloud/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2024-01-05 18:10:25.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/__init__.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3530 2024-04-05 06:43:24.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/aidoo.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    32279 2024-04-05 08:04:13.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/cloudapi.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2777 2024-04-05 06:43:24.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/common.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    10182 2024-04-05 08:15:56.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/const.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     8852 2024-04-05 08:10:42.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/device.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    11288 2024-04-05 07:36:49.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/device_group.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3081 2024-03-10 20:15:29.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/entity.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      807 2024-02-29 06:57:16.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/exceptions.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      925 2024-04-05 06:43:19.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/group.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     5368 2024-04-05 07:45:36.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/hotwater.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    26050 2024-04-05 06:43:24.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/hvac.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1821 2024-04-05 06:43:19.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/installation.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2024-01-05 18:10:25.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/py.typed
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1463 2024-04-05 06:43:19.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/system.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2495 2024-02-29 06:57:16.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/token.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     5948 2024-04-05 06:43:24.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/webserver.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     8581 2024-04-05 06:43:24.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/websockets.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3707 2024-04-05 06:43:24.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/zone.py
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2024-04-05 08:22:11.442738 aioairzone-cloud-0.5.0/aioairzone_cloud.egg-info/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1551 2024-04-05 08:22:11.000000 aioairzone-cloud-0.5.0/aioairzone_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      832 2024-04-05 08:22:11.000000 aioairzone-cloud-0.5.0/aioairzone_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2024-04-05 08:22:11.000000 aioairzone-cloud-0.5.0/aioairzone_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2024-04-05 08:22:11.000000 aioairzone-cloud-0.5.0/aioairzone_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2024-04-05 08:22:11.000000 aioairzone-cloud-0.5.0/aioairzone_cloud.egg-info/requires.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2024-04-05 08:22:11.000000 aioairzone-cloud-0.5.0/aioairzone_cloud.egg-info/top_level.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2327 2024-04-05 08:21:31.000000 aioairzone-cloud-0.5.0/pyproject.toml
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       77 2024-01-05 18:10:25.000000 aioairzone-cloud-0.5.0/requirements.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       38 2024-04-05 08:22:11.442738 aioairzone-cloud-0.5.0/setup.cfg
```

### Comparing `aioairzone-cloud-0.4.7/LICENSE` & `aioairzone-cloud-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.4.7/PKG-INFO` & `aioairzone-cloud-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.4.7
+Version: 0.5.0
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.4.7/README.md` & `aioairzone-cloud-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.4.7/aioairzone_cloud/aidoo.py` & `aioairzone-cloud-0.5.0/aioairzone_cloud/aidoo.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 from .common import SpeedType, parse_int, parse_str
 from .const import (
     API_MODE,
     API_NAME,
     API_POWER,
     API_SETPOINT,
+    API_SP_AIR_COOL,
+    API_SP_AIR_HEAT,
     API_SPEED_CONF,
     API_SPEED_TYPE,
     API_SPEED_VALUES,
     API_VALUE,
     AZD_SPEED,
     AZD_SPEED_TYPE,
     AZD_SPEEDS,
@@ -80,14 +82,18 @@
         """Update device parameter from API request."""
         if param == API_MODE:
             self.set_mode(data[API_VALUE])
         elif param == API_POWER:
             self.set_power(data[API_VALUE])
         elif param == API_SETPOINT:
             self.set_setpoint(data[API_VALUE])
+        elif param == API_SP_AIR_COOL:
+            self.set_setpoint_cool(data[API_VALUE])
+        elif param == API_SP_AIR_HEAT:
+            self.set_setpoint_heat(data[API_VALUE])
         elif param == API_SPEED_CONF:
             self.set_speed(data[API_VALUE])
 
     def update_data(self, update: EntityUpdate) -> None:
         """Update Aidoo data."""
         super().update_data(update)
```

### Comparing `aioairzone-cloud-0.4.7/aioairzone_cloud/cloudapi.py` & `aioairzone-cloud-0.5.0/aioairzone_cloud/cloudapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 from aiohttp import ClientConnectorError, ClientResponseError, ClientSession
 
 from .aidoo import Aidoo
 from .common import ConnectionOptions, OperationMode
 from .const import (
     API_AUTH_LOGIN,
     API_AUTH_REFRESH_TOKEN,
+    API_AZ_ACS,
     API_AZ_AIDOO,
+    API_AZ_AIDOO_ACS,
     API_AZ_AIDOO_PRO,
     API_AZ_SYSTEM,
     API_AZ_ZONE,
     API_CONFIG,
     API_DEVICE_ID,
     API_DEVICE_TYPE,
     API_DEVICES,
@@ -41,14 +43,15 @@
     API_USER_LOGOUT,
     API_V1,
     API_VALUE,
     API_WS,
     API_WS_ID,
     AZD_AIDOOS,
     AZD_GROUPS,
+    AZD_HOT_WATERS,
     AZD_INSTALLATIONS,
     AZD_SYSTEMS,
     AZD_WEBSERVERS,
     AZD_ZONES,
     HTTP_CALL_TIMEOUT,
     HTTP_MAX_REQUESTS,
     RAW_DEVICES_CONFIG,
@@ -66,14 +69,15 @@
     APIError,
     AuthError,
     LoginError,
     TokenRefreshError,
     TooManyRequests,
 )
 from .group import Group
+from .hotwater import HotWater
 from .installation import Installation
 from .system import System
 from .token import AirzoneCloudToken
 from .webserver import WebServer
 from .websockets import AirzoneCloudIWS
 from .zone import Zone
 
@@ -100,14 +104,15 @@
             RAW_WEBSERVERS: {},
         }
         self._api_semaphore: Semaphore = Semaphore(HTTP_MAX_REQUESTS)
         self.aidoos: dict[str, Aidoo] = {}
         self.callback_function = None
         self.callback_lock = Lock()
         self.devices: dict[str, Device] = {}
+        self.dhws: dict[str, HotWater] = {}
         self.groups: dict[str, Group] = {}
         self.installations: dict[str, Installation] = {}
         self.options = options
         self.session: ClientSession | None = session
         self.systems: dict[str, System] = {}
         self.token: AirzoneCloudToken = AirzoneCloudToken()
         self.webservers: dict[str, WebServer] = {}
@@ -396,14 +401,20 @@
         self, device_id: str, params: dict[str, Any]
     ) -> None:
         """Set device parameters."""
         device = self.get_device_id(device_id)
         if device is not None:
             await self.api_set_device_params(device, params)
 
+    async def api_set_dhw_id_params(self, dhw_id: str, params: dict[str, Any]) -> None:
+        """Set dhw parameters."""
+        dhw = self.get_dhw_id(dhw_id)
+        if dhw is not None:
+            await self.api_set_device_params(dhw, params)
+
     async def api_set_group_id_params(
         self, group_id: str, params: dict[str, Any]
     ) -> None:
         """Set group parameters."""
         group = self.get_group_id(group_id)
         if group is not None:
             await self.api_set_group_params(group, params)
@@ -483,14 +494,20 @@
 
         if len(self.aidoos) > 0:
             aidoos: dict[str, Any] = {}
             for key, aidoo in self.aidoos.items():
                 aidoos[key] = aidoo.data()
             data[AZD_AIDOOS] = aidoos
 
+        if len(self.dhws) > 0:
+            dhws: dict[str, Any] = {}
+            for key, dhw in self.dhws.items():
+                dhws[key] = dhw.data()
+            data[AZD_HOT_WATERS] = dhws
+
         if len(self.groups) > 0:
             groups: dict[str, Any] = {}
             for key, group in self.groups.items():
                 groups[key] = group.data()
             data[AZD_GROUPS] = groups
 
         if len(self.installations) > 0:
@@ -526,14 +543,19 @@
 
     def add_device(self, device: Device) -> None:
         """Add Airzone Cloud Device."""
         dev_id = device.get_id()
         if dev_id not in self.devices:
             self.devices[dev_id] = device
 
+    def add_dhw(self, dhw: HotWater) -> None:
+        """Add Airzone Cloud Domestic Hot Water."""
+        self.dhws[dhw.get_id()] = dhw
+        self.add_device(dhw)
+
     def add_system(self, system: System) -> None:
         """Add Airzone Cloud System."""
         self.systems[system.get_id()] = system
         self.add_device(system)
 
     def add_zone(self, zone: Zone) -> None:
         """Add Airzone Cloud System."""
@@ -546,14 +568,18 @@
 
     def get_device_id(self, dev_id: str | None) -> Device | None:
         """Return Airzone Cloud Device by ID."""
         if dev_id is not None:
             return self.devices.get(dev_id)
         return None
 
+    def get_dhw_id(self, dhw_id: str) -> HotWater | None:
+        """Return Airzone Cloud DHW by ID."""
+        return self.dhws.get(dhw_id)
+
     def get_group_id(self, group_id: str) -> Group | None:
         """Return Airzone Cloud Group by ID."""
         return self.groups.get(group_id)
 
     def get_installation_id(self, inst_id: str) -> Installation | None:
         """Return Airzone Cloud Installation by ID."""
         return self.installations.get(inst_id)
@@ -635,14 +661,31 @@
         tasks = []
 
         for aidoo in self.aidoos.values():
             tasks += [self.update_aidoo(aidoo)]
 
         await asyncio.gather(*tasks)
 
+    async def update_dhw(self, dhw: HotWater) -> None:
+        """Update Airzone Cloud DHW from API."""
+        device_data = await self.api_get_device_status(dhw)
+
+        update = EntityUpdate(UpdateType.API_FULL, device_data)
+
+        await dhw.update(update)
+
+    async def update_dhws(self) -> None:
+        """Update all Airzone Cloud DHWs."""
+        tasks = []
+
+        for dhw in self.dhws.values():
+            tasks += [self.update_dhw(dhw)]
+
+        await asyncio.gather(*tasks)
+
     def connect_installation_websockets(self, inst_id: str) -> None:
         """Connect installation WebSockets."""
         if not self.options.websockets:
             return
 
         inst_ws = self.websockets.get(inst_id)
         if inst_ws is not None:
@@ -676,14 +719,21 @@
                 elif device_type in [API_AZ_AIDOO, API_AZ_AIDOO_PRO]:
                     if self.get_aidoo_id(device_id) is None:
                         aidoo = Aidoo(inst_id, device_data[API_WS_ID], device_data)
                         if aidoo is not None:
                             self.add_aidoo(aidoo)
                             group.add_aidoo(aidoo)
                             inst.add_aidoo(aidoo)
+                elif device_type in [API_AZ_ACS, API_AZ_AIDOO_ACS]:
+                    if self.get_dhw_id(device_id) is None:
+                        dhw = HotWater(inst_id, device_data[API_WS_ID], device_data)
+                        if HotWater is not None:
+                            self.add_dhw(dhw)
+                            group.add_dhw(dhw)
+                            inst.add_dhw(dhw)
 
         self.connect_installation_websockets(inst_id)
 
     async def update_installations(self) -> None:
         """Update Airzone Cloud installations from API."""
         installations_data = await self.api_get_installations()
         for installation_data in installations_data[API_INSTALLATIONS]:
@@ -763,14 +813,21 @@
                 elif device_type in [API_AZ_AIDOO, API_AZ_AIDOO_PRO]:
                     if self.get_aidoo_id(device_id) is None:
                         aidoo = Aidoo(ws.get_installation(), ws_id, device_data)
                         if aidoo is not None:
                             self.add_aidoo(aidoo)
                             if inst is not None:
                                 inst.add_aidoo(aidoo)
+                elif device_type in [API_AZ_ACS, API_AZ_AIDOO_ACS]:
+                    if self.get_dhw_id(device_id) is None:
+                        dhw = HotWater(ws.get_installation(), ws_id, device_data)
+                        if dhw is not None:
+                            self.add_dhw(dhw)
+                            if inst is not None:
+                                inst.add_dhw(dhw)
 
     async def update_webserver_id(self, ws_id: str, devices: bool) -> None:
         """Update Airzone Cloud WebServer by ID."""
         ws = self.get_webserver_id(ws_id)
         if ws is not None:
             await self.update_webserver(ws, devices)
 
@@ -811,14 +868,15 @@
 
     async def _update_polling(self) -> None:
         """Perform a polling update of Airzone Cloud data."""
         tasks = [
             self.update_webservers(False),
             self.update_systems_zones(),
             self.update_aidoos(),
+            self.update_dhws(),
         ]
 
         await asyncio.gather(*tasks)
         self._api_init_done = True
 
     async def _update_websockets(self) -> bool:
         """Perform a websockets update of Airzone Cloud data."""
```

### Comparing `aioairzone-cloud-0.4.7/aioairzone_cloud/common.py` & `aioairzone-cloud-0.5.0/aioairzone_cloud/common.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.4.7/aioairzone_cloud/const.py` & `aioairzone-cloud-0.5.0/aioairzone_cloud/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,47 +21,53 @@
 API_CITY: Final[str] = "city"
 API_CONFIG: Final[str] = "config"
 API_CONNECTION_DATE: Final[str] = "connection_date"
 API_DEVICE_ID: Final[str] = "device_id"
 API_DEVICE_TYPE: Final[str] = "device_type"
 API_DEVICES: Final[str] = "devices"
 API_DISCONNECTION_DATE: Final[str] = "disconnection_date"
+API_DOUBLE_SET_POINT: Final[str] = "double_sp"
 API_ECO_CONF: Final[str] = "eco_conf"
 API_EMAIL: Final[str] = "email"
 API_ERRORS: Final[str] = "errors"
 API_FAH: Final[str] = "fah"
 API_GROUP: Final[str] = "group"
 API_GROUP_ID: Final[str] = "group_id"
 API_GROUPS: Final[str] = "groups"
 API_HUMIDITY: Final[str] = "humidity"
 API_INSTALLATION_ID: Final[str] = "installation_id"
 API_INSTALLATIONS: Final[str] = "installations"
 API_IS_CONNECTED: Final[str] = "isConnected"
 API_LOCAL_TEMP: Final[str] = "local_temp"
 API_LOCATION_ID: Final[str] = "location_id"
+API_MACHINE_READY: Final[str] = "machineready"
 API_META: Final[str] = "meta"
 API_MODE: Final[str] = "mode"
 API_MODE_AVAIL: Final[str] = "mode_available"
 API_NAME: Final[str] = "name"
 API_OLD_ID: Final[str] = "_id"
 API_OPTS: Final[str] = "opts"
 API_PARAM: Final[str] = "param"
 API_PARAMS: Final[str] = "params"
 API_PASSWORD: Final[str] = "password"
 API_PIN: Final[str] = "pin"
 API_POWER: Final[str] = "power"
+API_POWERFUL_MODE: Final[str] = "powerful_mode"
+API_RAD_ACTIVE: Final[str] = "rad_active"
 API_RANGE_MAX_AIR: Final[str] = "range_air_max"
 API_RANGE_MIN_AIR: Final[str] = "range_air_min"
+API_RANGE_SP_MAX_ACS: Final[str] = "range_sp_acs_max"
 API_RANGE_SP_MAX_AUTO_AIR: Final[str] = "range_sp_auto_air_max"
 API_RANGE_SP_MAX_COOL_AIR: Final[str] = "range_sp_cool_air_max"
 API_RANGE_SP_MAX_DRY_AIR: Final[str] = "range_sp_dry_air_max"
 API_RANGE_SP_MAX_EMERHEAT_AIR: Final[str] = "range_sp_emerheat_air_max"
 API_RANGE_SP_MAX_HOT_AIR: Final[str] = "range_sp_hot_air_max"
 API_RANGE_SP_MAX_STOP_AIR: Final[str] = "range_sp_stop_air_max"
 API_RANGE_SP_MAX_VENT_AIR: Final[str] = "range_sp_vent_air_max"
+API_RANGE_SP_MIN_ACS: Final[str] = "range_sp_acs_min"
 API_RANGE_SP_MIN_AUTO_AIR: Final[str] = "range_sp_auto_air_min"
 API_RANGE_SP_MIN_COOL_AIR: Final[str] = "range_sp_cool_air_min"
 API_RANGE_SP_MIN_DRY_AIR: Final[str] = "range_sp_dry_air_min"
 API_RANGE_SP_MIN_EMERHEAT_AIR: Final[str] = "range_sp_emerheat_air_min"
 API_RANGE_SP_MIN_HOT_AIR: Final[str] = "range_sp_hot_air_min"
 API_RANGE_SP_MIN_STOP_AIR: Final[str] = "range_sp_stop_air_min"
 API_RANGE_SP_MIN_VENT_AIR: Final[str] = "range_sp_vent_air_min"
@@ -81,14 +87,16 @@
 API_STAT_CHANNEL: Final[str] = "stat_channel"
 API_STAT_QUALITY: Final[str] = "stat_quality"
 API_STAT_RSSI: Final[str] = "stat_rssi"
 API_STAT_SSID: Final[str] = "stat_ssid"
 API_STATUS: Final[str] = "status"
 API_STEP: Final[str] = "step"
 API_SYSTEM_NUMBER: Final[str] = "system_number"
+API_TANK_TEMP: Final[str] = "tank_temp"
+API_TT_UNITS: Final[str] = "tt_units"
 API_TIMER: Final[str] = "timer"
 API_TOKEN: Final[str] = "token"
 API_TYPE: Final[str] = "type"
 API_UNITS: Final[str] = "units"
 API_URL: Final[str] = f"https://{AIRZONE_SERVER}"
 API_USER: Final[str] = "user"
 API_USER_ID: Final[str] = "user_id"
@@ -107,19 +115,22 @@
 
 API_AQ_STATUS: Final[dict[str, int]] = {
     "good": 1,
     "regular": 151,
     "bad": 301,
 }
 API_AZ_AIDOO: Final[str] = "aidoo"
+API_AZ_AIDOO_ACS: Final[str] = "aidoo_acs"
 API_AZ_AIDOO_PRO: Final[str] = "aidoo_it"
+API_AZ_ACS: Final[str] = "az_acs"
 API_AZ_SYSTEM: Final[str] = "az_system"
 API_AZ_ZONE: Final[str] = "az_zone"
 
 API_DEFAULT_TEMP_STEP: Final[float] = 0.5
+API_DEFAULT_TEMP_STEP_ACS: Final[int] = 1
 
 AZD_ACTION: Final[str] = "action"
 AZD_ACTIVE: Final[str] = "active"
 AZD_AIDOOS: Final[str] = "aidoos"
 AZD_AQ_ACTIVE: Final[str] = "aq-active"
 AZD_AQ_INDEX: Final[str] = "aq-index"
 AZD_AQ_MODE_CONF: Final[str] = "aq-mode-conf"
@@ -128,30 +139,33 @@
 AZD_AQ_PM_2P5: Final[str] = "aq-pm-2.5"
 AZD_AQ_PM_10: Final[str] = "aq-pm-10"
 AZD_AQ_PRESENT: Final[str] = "aq-present"
 AZD_AQ_STATUS: Final[str] = "aq-status"
 AZD_AVAILABLE: Final[str] = "available"
 AZD_CONNECTION_DATE: Final[str] = "connection-date"
 AZD_DISCONNECTION_DATE: Final[str] = "disconnection-date"
+AZD_DOUBLE_SET_POINT: Final[str] = "double-set-point"
 AZD_ERRORS: Final[str] = "errors"
 AZD_FIRMWARE: Final[str] = "firmware"
 AZD_GROUPS: Final[str] = "groups"
 AZD_HUMIDITY: Final[str] = "humidity"
+AZD_HOT_WATERS: Final[str] = "hot-water"
 AZD_ID: Final[str] = "id"
 AZD_INSTALLATION: Final[str] = "installation"
 AZD_INSTALLATIONS: Final[str] = "installations"
 AZD_IS_CONNECTED: Final[str] = "is-connected"
 AZD_MASTER: Final[str] = "master"
 AZD_MODE: Final[str] = "mode"
 AZD_MODE_AUTO: Final[str] = "mode-auto"
 AZD_MODES: Final[str] = "modes"
 AZD_NAME: Final[str] = "name"
 AZD_NUM_DEVICES: Final[str] = "num-devices"
 AZD_NUM_GROUPS: Final[str] = "num-groups"
 AZD_POWER: Final[str] = "power"
+AZD_POWER_MODE: Final[str] = "power-mode"
 AZD_PROBLEMS: Final[str] = "problems"
 AZD_SPEED: Final[str] = "speed"
 AZD_SPEEDS: Final[str] = "speeds"
 AZD_SPEED_TYPE: Final[str] = "speed-type"
 AZD_SYSTEM: Final[str] = "system"
 AZD_SYSTEM_ID: Final[str] = "system-id"
 AZD_SYSTEMS: Final[str] = "systems"
```

### Comparing `aioairzone-cloud-0.4.7/aioairzone_cloud/device.py` & `aioairzone-cloud-0.5.0/aioairzone_cloud/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,14 @@
     def data(self) -> dict[str, Any]:
         """Return Device data."""
         data: dict[str, Any] = {
             AZD_AVAILABLE: self.get_available(),
             AZD_ID: self.get_id(),
             AZD_INSTALLATION: self.get_installation(),
             AZD_IS_CONNECTED: self.get_is_connected(),
-            AZD_MODE: self.get_mode(),
             AZD_NAME: self.get_name(),
             AZD_PROBLEMS: self.get_problems(),
             AZD_WEBSERVER: self.get_webserver(),
             AZD_WS_CONNECTED: self.get_ws_connected(),
         }
 
         aq_index = self.get_aq_index()
@@ -130,14 +129,18 @@
         if aq_status is not None:
             data[AZD_AQ_STATUS] = aq_status
 
         errors = self.get_errors()
         if len(errors) > 0:
             data[AZD_ERRORS] = errors
 
+        mode = self.get_mode()
+        if mode is not None:
+            data[AZD_MODE] = mode
+
         mode_auto = self.get_mode_auto()
         if mode_auto is not None:
             data[AZD_MODE_AUTO] = mode_auto
 
         modes = self.get_modes()
         if modes is not None:
             data[AZD_MODES] = modes
```

### Comparing `aioairzone-cloud-0.4.7/aioairzone_cloud/device_group.py` & `aioairzone-cloud-0.5.0/aioairzone_cloud/device_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     API_DEFAULT_TEMP_STEP,
     API_PARAMS,
     API_VALUE,
     AZD_ACTION,
     AZD_ACTIVE,
     AZD_AIDOOS,
     AZD_AVAILABLE,
+    AZD_HOT_WATERS,
     AZD_HUMIDITY,
     AZD_ID,
     AZD_MODE,
     AZD_MODES,
     AZD_NAME,
     AZD_NUM_DEVICES,
     AZD_POWER,
@@ -27,37 +28,41 @@
     AZD_TEMP,
     AZD_TEMP_SET,
     AZD_TEMP_SET_MAX,
     AZD_TEMP_SET_MIN,
     AZD_TEMP_STEP,
     AZD_ZONES,
 )
+from .hotwater import HotWater
 from .system import System
 from .zone import Zone
 
 
 class DeviceGroup(ABC):
     """Airzone Cloud DeviceGroup."""
 
     id: str
     name: str
 
     def __init__(self) -> None:
         """Airzone Cloud DeviceGroup init."""
 
         self.aidoos: dict[str, Aidoo] = {}
+        self.dhws: dict[str, HotWater] = {}
         self.systems: dict[str, System] = {}
         self.zones: dict[str, Zone] = {}
 
     def data(self) -> dict[str, Any]:
         """Return DeviceGroup data."""
         data: dict[str, Any] = {}
 
         if len(self.aidoos) > 0:
             data[AZD_AIDOOS] = list(self.aidoos)
+        if len(self.dhws) > 0:
+            data[AZD_HOT_WATERS] = list(self.dhws)
         if len(self.systems) > 0:
             data[AZD_SYSTEMS] = list(self.systems)
         if len(self.zones) > 0:
             data[AZD_ZONES] = list(self.zones)
 
         data[AZD_ACTION] = self.get_action()
         data[AZD_ACTIVE] = self.get_active()
@@ -131,14 +136,20 @@
 
     def add_aidoo(self, aidoo: Aidoo) -> None:
         """Add Aidoo to DeviceGroup."""
         aidoo_id = aidoo.get_id()
         if aidoo_id not in self.aidoos:
             self.aidoos[aidoo_id] = aidoo
 
+    def add_dhw(self, dhw: HotWater) -> None:
+        """Add DHW to DeviceGroup."""
+        dhw_id = dhw.get_id()
+        if dhw_id not in self.dhws:
+            self.dhws[dhw_id] = dhw
+
     def add_system(self, system: System) -> None:
         """Add System to DeviceGroup."""
         system_id = system.get_id()
         if system_id not in self.systems:
             self.systems[system_id] = system
 
     def add_zone(self, zone: Zone) -> None:
```

### Comparing `aioairzone-cloud-0.4.7/aioairzone_cloud/entity.py` & `aioairzone-cloud-0.5.0/aioairzone_cloud/entity.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.4.7/aioairzone_cloud/exceptions.py` & `aioairzone-cloud-0.5.0/aioairzone_cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.4.7/aioairzone_cloud/group.py` & `aioairzone-cloud-0.5.0/aioairzone_cloud/group.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.4.7/aioairzone_cloud/hvac.py` & `aioairzone-cloud-0.5.0/aioairzone_cloud/hvac.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from .const import (
     API_ACTIVE,
     API_AQ_ACTIVE,
     API_AQ_MODE_CONF,
     API_AQ_MODE_VALUES,
     API_CELSIUS,
     API_DEFAULT_TEMP_STEP,
+    API_DOUBLE_SET_POINT,
     API_HUMIDITY,
     API_LOCAL_TEMP,
     API_POWER,
     API_RANGE_MAX_AIR,
     API_RANGE_MIN_AIR,
     API_RANGE_SP_MAX_AUTO_AIR,
     API_RANGE_SP_MAX_COOL_AIR,
@@ -45,14 +46,15 @@
     API_SP_AIR_VENT,
     API_STEP,
     AZD_ACTION,
     AZD_ACTIVE,
     AZD_AQ_ACTIVE,
     AZD_AQ_MODE_CONF,
     AZD_AQ_MODE_VALUES,
+    AZD_DOUBLE_SET_POINT,
     AZD_HUMIDITY,
     AZD_POWER,
     AZD_TEMP,
     AZD_TEMP_SET,
     AZD_TEMP_SET_AUTO_AIR,
     AZD_TEMP_SET_COOL_AIR,
     AZD_TEMP_SET_DRY_AIR,
@@ -88,14 +90,15 @@
         """Airzone Cloud HVAC device init."""
         super().__init__(inst_id, ws_id, device_data)
 
         self.active: bool | None = None
         self.aq_active: bool | None = None
         self.aq_mode_conf: AirQualityMode | None = None
         self.aq_mode_values: list[AirQualityMode] | None = None
+        self.double_set_point: bool | None = None
         self.humidity: int | None = None
         self.name: str = "HVAC"
         self.power: bool | None = None
         self.temp_set_max: float | None = None
         self.temp_set_max_auto_air: float | None = None
         self.temp_set_max_cool_air: float | None = None
         self.temp_set_max_dry_air: float | None = None
@@ -122,14 +125,15 @@
 
     def data(self) -> dict[str, Any]:
         """Return HVAC device data."""
         data = super().data()
 
         data[AZD_ACTION] = self.get_action()
         data[AZD_ACTIVE] = self.get_active()
+        data[AZD_DOUBLE_SET_POINT] = self.get_double_set_point()
         data[AZD_POWER] = self.get_power()
         data[AZD_TEMP] = self.get_temperature()
         data[AZD_TEMP_STEP] = self.get_temp_step()
 
         aq_active = self.get_aq_active()
         if aq_active is not None:
             data[AZD_AQ_ACTIVE] = aq_active
@@ -275,14 +279,20 @@
 
     def get_aq_mode_values(self) -> list[AirQualityMode] | None:
         """Return HVAC device Air Quality mode values."""
         if self.aq_mode_values is not None and len(self.aq_mode_values) > 0:
             return self.aq_mode_values
         return None
 
+    def get_double_set_point(self) -> bool:
+        """Return HVAC double set point."""
+        if self.double_set_point is not None:
+            return self.double_set_point
+        return False
+
     def get_humidity(self) -> int | None:
         """Return HVAC device humidity."""
         return self.humidity
 
     def get_power(self) -> bool | None:
         """Return HVAC device power."""
         return self.power
@@ -495,14 +505,24 @@
         if self.temp_set_hot_air is not None:
             self.temp_set_hot_air = setpoint
         if self.temp_set_stop_air is not None:
             self.temp_set_stop_air = setpoint
         if self.temp_set_vent_air is not None:
             self.temp_set_vent_air = setpoint
 
+    def set_setpoint_cool(self, setpoint: float) -> None:
+        """Set HVAC cool setpoint."""
+        if self.temp_set_cool_air is not None:
+            self.temp_set_cool_air = setpoint
+
+    def set_setpoint_heat(self, setpoint: float) -> None:
+        """Set HVAC heat setpoint."""
+        if self.temp_set_hot_air is not None:
+            self.temp_set_hot_air = setpoint
+
     def update_data(self, update: EntityUpdate) -> None:
         """Update HVAC device data."""
         super().update_data(update)
 
         data = update.get_data()
 
         if API_ACTIVE in data:
@@ -526,14 +546,18 @@
 
         aq_mode_values = data.get(API_AQ_MODE_VALUES)
         if aq_mode_values is not None:
             self.aq_mode_values = []
             for aq_mode_value in aq_mode_values:
                 self.aq_mode_values += [AirQualityMode(aq_mode_value)]
 
+        double_set_point = parse_bool(data.get(API_DOUBLE_SET_POINT))
+        if double_set_point is not None:
+            self.double_set_point = double_set_point
+
         humidity = parse_int(data.get(API_HUMIDITY))
         if humidity is not None:
             self.humidity = humidity
 
         local_temp = parse_float(data.get(API_LOCAL_TEMP, {}).get(API_CELSIUS))
         if local_temp is not None:
             self.temp = local_temp
```

### Comparing `aioairzone-cloud-0.4.7/aioairzone_cloud/installation.py` & `aioairzone-cloud-0.5.0/aioairzone_cloud/installation.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.4.7/aioairzone_cloud/system.py` & `aioairzone-cloud-0.5.0/aioairzone_cloud/system.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.4.7/aioairzone_cloud/token.py` & `aioairzone-cloud-0.5.0/aioairzone_cloud/token.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.4.7/aioairzone_cloud/webserver.py` & `aioairzone-cloud-0.5.0/aioairzone_cloud/webserver.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.4.7/aioairzone_cloud/websockets.py` & `aioairzone-cloud-0.5.0/aioairzone_cloud/websockets.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.4.7/aioairzone_cloud/zone.py` & `aioairzone-cloud-0.5.0/aioairzone_cloud/zone.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from .const import (
     API_AQ_MODE_CONF,
     API_MODE,
     API_MODE_AVAIL,
     API_NAME,
     API_POWER,
     API_SETPOINT,
+    API_SP_AIR_COOL,
+    API_SP_AIR_HEAT,
     API_SYSTEM_NUMBER,
     API_VALUE,
     API_ZONE_NUMBER,
     AZD_MASTER,
     AZD_SYSTEM,
     AZD_SYSTEM_ID,
     AZD_ZONE,
@@ -101,14 +103,18 @@
                 self.system.set_param(param, data)
             else:
                 self.set_mode(data[API_VALUE])
         elif param == API_POWER:
             self.set_power(data[API_VALUE])
         elif param == API_SETPOINT:
             self.set_setpoint(data[API_VALUE])
+        elif param == API_SP_AIR_COOL:
+            self.set_setpoint_cool(data[API_VALUE])
+        elif param == API_SP_AIR_HEAT:
+            self.set_setpoint_heat(data[API_VALUE])
 
     def set_system(self, system: System) -> None:
         """Set System."""
         self.system = system
 
     def update_data(self, update: EntityUpdate) -> None:
         """Update Zone data."""
```

### Comparing `aioairzone-cloud-0.4.7/aioairzone_cloud.egg-info/PKG-INFO` & `aioairzone-cloud-0.5.0/aioairzone_cloud.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.4.7
+Version: 0.5.0
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.4.7/aioairzone_cloud.egg-info/SOURCES.txt` & `aioairzone-cloud-0.5.0/aioairzone_cloud.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 aioairzone_cloud/common.py
 aioairzone_cloud/const.py
 aioairzone_cloud/device.py
 aioairzone_cloud/device_group.py
 aioairzone_cloud/entity.py
 aioairzone_cloud/exceptions.py
 aioairzone_cloud/group.py
+aioairzone_cloud/hotwater.py
 aioairzone_cloud/hvac.py
 aioairzone_cloud/installation.py
 aioairzone_cloud/py.typed
 aioairzone_cloud/system.py
 aioairzone_cloud/token.py
 aioairzone_cloud/webserver.py
 aioairzone_cloud/websockets.py
```

### Comparing `aioairzone-cloud-0.4.7/pyproject.toml` & `aioairzone-cloud-0.5.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aioairzone-cloud"
-version = "0.4.7"
+version = "0.5.0"
 description = "Library to control Airzone Cloud devices"
 readme = "README.md"
 requires-python = ">=3.11"
 license = {text = "Apache-2.0"}
 keywords = ["airzone", "cloud", "hvac", "home"] 
 authors = [
   {name = "Álvaro Fernández Rojas", email = "noltari@gmail.com" }
```

