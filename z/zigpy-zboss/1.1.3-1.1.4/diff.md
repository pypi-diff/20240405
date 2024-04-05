# Comparing `tmp/zigpy-zboss-1.1.3.tar.gz` & `tmp/zigpy-zboss-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zigpy-zboss-1.1.3.tar", last modified: Fri Feb 16 05:29:46 2024, max compression
+gzip compressed data, was "zigpy-zboss-1.1.4.tar", last modified: Fri Apr  5 10:49:36 2024, max compression
```

## Comparing `zigpy-zboss-1.1.3.tar` & `zigpy-zboss-1.1.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 05:29:46.979858 zigpy-zboss-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11691 2024-02-16 05:29:46.979858 zigpy-zboss-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10779 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-02-16 05:29:46.979858 zigpy-zboss-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 05:29:46.971859 zigpy-zboss-1.1.3/zigpy_zboss/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11280 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/checksum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 05:29:46.975859 zigpy-zboss-1.1.3/zigpy_zboss/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/commands/af.py
--rw-r--r--   0 runner    (1001) docker     (127)     9344 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/commands/aps.py
--rw-r--r--   0 runner    (1001) docker     (127)    16128 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/commands/ncp_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/commands/nwk_mgmt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/commands/security.py
--rw-r--r--   0 runner    (1001) docker     (127)    16178 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/commands/zdo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10916 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/frames.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/nvram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 05:29:46.975859 zigpy-zboss-1.1.3/zigpy_zboss/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/tools/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/tools/factory_reset_ncp.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/tools/get_ncp_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 05:29:46.975859 zigpy-zboss-1.1.3/zigpy_zboss/types/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/types/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    21891 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/types/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/types/cstruct.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/types/named.py
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/types/nvids.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/types/structs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10569 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/uart.py
--rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 05:29:46.975859 zigpy-zboss-1.1.3/zigpy_zboss/zigbee/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/zigbee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24783 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/zigbee/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     8634 2024-02-16 05:29:39.000000 zigpy-zboss-1.1.3/zigpy_zboss/zigbee/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 05:29:46.975859 zigpy-zboss-1.1.3/zigpy_zboss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11691 2024-02-16 05:29:46.000000 zigpy-zboss-1.1.3/zigpy_zboss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-02-16 05:29:46.000000 zigpy-zboss-1.1.3/zigpy_zboss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 05:29:46.000000 zigpy-zboss-1.1.3/zigpy_zboss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-02-16 05:29:46.000000 zigpy-zboss-1.1.3/zigpy_zboss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-16 05:29:46.000000 zigpy-zboss-1.1.3/zigpy_zboss.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:49:36.929142 zigpy-zboss-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12661 2024-04-05 10:49:36.929142 zigpy-zboss-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-05 10:49:36.929142 zigpy-zboss-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:49:36.921142 zigpy-zboss-1.1.4/zigpy_zboss/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11280 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/checksum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:49:36.925142 zigpy-zboss-1.1.4/zigpy_zboss/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/commands/af.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9344 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/commands/aps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16128 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/commands/ncp_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/commands/nwk_mgmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/commands/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16178 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/commands/zdo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10916 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/frames.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/nvram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:49:36.925142 zigpy-zboss-1.1.4/zigpy_zboss/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/tools/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/tools/factory_reset_ncp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/tools/get_ncp_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:49:36.925142 zigpy-zboss-1.1.4/zigpy_zboss/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/types/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21891 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/types/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/types/cstruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/types/named.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/types/nvids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/types/structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10569 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/uart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:49:36.925142 zigpy-zboss-1.1.4/zigpy_zboss/zigbee/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/zigbee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25054 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/zigbee/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10932 2024-04-05 10:49:31.000000 zigpy-zboss-1.1.4/zigpy_zboss/zigbee/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:49:36.925142 zigpy-zboss-1.1.4/zigpy_zboss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12661 2024-04-05 10:49:36.000000 zigpy-zboss-1.1.4/zigpy_zboss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-05 10:49:36.000000 zigpy-zboss-1.1.4/zigpy_zboss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 10:49:36.000000 zigpy-zboss-1.1.4/zigpy_zboss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-05 10:49:36.000000 zigpy-zboss-1.1.4/zigpy_zboss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 10:49:36.000000 zigpy-zboss-1.1.4/zigpy_zboss.egg-info/top_level.txt
```

### Comparing `zigpy-zboss-1.1.3/COPYING` & `zigpy-zboss-1.1.4/COPYING`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/LICENSE` & `zigpy-zboss-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/PKG-INFO` & `zigpy-zboss-1.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigpy-zboss
-Version: 1.1.3
+Version: 1.1.4
 Summary: A library for zigpy which communicates with Nordic nRF52 radios
 Home-page: https://github.com/kardia-as/zigpy-zboss
 Author: Damien Kastner
 Author-email: damien.kastner@kardia.no
 License: GPL-3.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
@@ -26,14 +26,22 @@
 
 # zigpy-zboss
 
 **zigpy-zboss** is a Python library project that adds support for common Nordic Semiconductor nRF modules to **[zigpy (a open source Python Zigbee stack project)](https://github.com/zigpy/)** and other Network Co-Processor radios that uses firmware based on **[ZOI (ZBOSS Open Initiative) by DSR](https://dsr-zoi.com/)**.
 
 Together with the zigpy library and a home automation software application with compatible Zigbee gateway implementation, (such as for example the **[Home Assistant's ZHA integration component](https://www.home-assistant.io/integrations/zha/)**), you can directly control Zigbee devices from most product manufacturers, like; IKEA, Philips Hue, Inovelli, LEDVANCE/OSRAM, SmartThings/Samsung, SALUS/Computime, SONOFF/ITEAD, Xiaomi/Aqara, and many more.
 
+# Back-story and use cases
+
+This is currently an 'as-is' independent and unofficial implementation radio library for zigpy, as such should be considered experimental and you should only expect best-effort support from volunteers in the open-source community!
+
+Zigbee NCP support for ZOI (ZBOSS Open Initiative) based Zigbee radios compatible with ZBOSS NCP firmware for zigpy based Zigbee gateway implementation is still in very early development. 
+
+Development is initially focused on Zigbee Coordinator functionality Nordic Semiconductor's development kit hardware which has been tested to be compatible. Those also officially recognized as Zigbee-Compliant platforms by the CSA (Connectivity Standards Alliance, formerly the Zigbee Alliance), of which both [DSR Cooperation](https://pt.dsr-corporation.com/news/zboss-open-initiative-in-2021/) and [Nordic Semiconductor](https://developer.nordicsemi.com/nRF_Connect_SDK/doc/zboss/) are board and promoter members of.
+
 # Hardware requirements
 
 Nordic Semi USB adapters and development kits/boards based on nRF52840 SoC are used as reference hardware in the zigpy-zboss project:
 
 - **[nRF52840 dongle](https://www.nordicsemi.com/Products/Development-hardware/nrf52840-dongle)**
 - **[nRF52840 development kit](https://www.nordicsemi.com/Products/Development-hardware/nrf52840-dk)**
```

### Comparing `zigpy-zboss-1.1.3/README.md` & `zigpy-zboss-1.1.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 # zigpy-zboss
 
 **zigpy-zboss** is a Python library project that adds support for common Nordic Semiconductor nRF modules to **[zigpy (a open source Python Zigbee stack project)](https://github.com/zigpy/)** and other Network Co-Processor radios that uses firmware based on **[ZOI (ZBOSS Open Initiative) by DSR](https://dsr-zoi.com/)**.
 
 Together with the zigpy library and a home automation software application with compatible Zigbee gateway implementation, (such as for example the **[Home Assistant's ZHA integration component](https://www.home-assistant.io/integrations/zha/)**), you can directly control Zigbee devices from most product manufacturers, like; IKEA, Philips Hue, Inovelli, LEDVANCE/OSRAM, SmartThings/Samsung, SALUS/Computime, SONOFF/ITEAD, Xiaomi/Aqara, and many more.
 
+# Back-story and use cases
+
+This is currently an 'as-is' independent and unofficial implementation radio library for zigpy, as such should be considered experimental and you should only expect best-effort support from volunteers in the open-source community!
+
+Zigbee NCP support for ZOI (ZBOSS Open Initiative) based Zigbee radios compatible with ZBOSS NCP firmware for zigpy based Zigbee gateway implementation is still in very early development. 
+
+Development is initially focused on Zigbee Coordinator functionality Nordic Semiconductor's development kit hardware which has been tested to be compatible. Those also officially recognized as Zigbee-Compliant platforms by the CSA (Connectivity Standards Alliance, formerly the Zigbee Alliance), of which both [DSR Cooperation](https://pt.dsr-corporation.com/news/zboss-open-initiative-in-2021/) and [Nordic Semiconductor](https://developer.nordicsemi.com/nRF_Connect_SDK/doc/zboss/) are board and promoter members of.
+
 # Hardware requirements
 
 Nordic Semi USB adapters and development kits/boards based on nRF52840 SoC are used as reference hardware in the zigpy-zboss project:
 
 - **[nRF52840 dongle](https://www.nordicsemi.com/Products/Development-hardware/nrf52840-dongle)**
 - **[nRF52840 development kit](https://www.nordicsemi.com/Products/Development-hardware/nrf52840-dk)**
```

### Comparing `zigpy-zboss-1.1.3/pyproject.toml` & `zigpy-zboss-1.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/setup.cfg` & `zigpy-zboss-1.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss/api.py` & `zigpy-zboss-1.1.4/zigpy_zboss/api.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss/checksum.py` & `zigpy-zboss-1.1.4/zigpy_zboss/checksum.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss/commands/__init__.py` & `zigpy-zboss-1.1.4/zigpy_zboss/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss/commands/af.py` & `zigpy-zboss-1.1.4/zigpy_zboss/commands/af.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss/commands/aps.py` & `zigpy-zboss-1.1.4/zigpy_zboss/commands/aps.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss/commands/ncp_config.py` & `zigpy-zboss-1.1.4/zigpy_zboss/commands/ncp_config.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss/commands/nwk_mgmt.py` & `zigpy-zboss-1.1.4/zigpy_zboss/commands/nwk_mgmt.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss/commands/security.py` & `zigpy-zboss-1.1.4/zigpy_zboss/commands/security.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss/commands/zdo.py` & `zigpy-zboss-1.1.4/zigpy_zboss/commands/zdo.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss/config.py` & `zigpy-zboss-1.1.4/zigpy_zboss/config.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss/debug.py` & `zigpy-zboss-1.1.4/zigpy_zboss/debug.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss/frames.py` & `zigpy-zboss-1.1.4/zigpy_zboss/frames.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss/logger.py` & `zigpy-zboss-1.1.4/zigpy_zboss/logger.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss/nvram.py` & `zigpy-zboss-1.1.4/zigpy_zboss/nvram.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss/tools/config.py` & `zigpy-zboss-1.1.4/zigpy_zboss/tools/config.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss/tools/factory_reset_ncp.py` & `zigpy-zboss-1.1.4/zigpy_zboss/tools/factory_reset_ncp.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss/tools/get_ncp_version.py` & `zigpy-zboss-1.1.4/zigpy_zboss/tools/get_ncp_version.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss/types/basic.py` & `zigpy-zboss-1.1.4/zigpy_zboss/types/basic.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss/types/commands.py` & `zigpy-zboss-1.1.4/zigpy_zboss/types/commands.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss/types/cstruct.py` & `zigpy-zboss-1.1.4/zigpy_zboss/types/cstruct.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss/types/named.py` & `zigpy-zboss-1.1.4/zigpy_zboss/types/named.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss/types/nvids.py` & `zigpy-zboss-1.1.4/zigpy_zboss/types/nvids.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss/types/structs.py` & `zigpy-zboss-1.1.4/zigpy_zboss/types/structs.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss/uart.py` & `zigpy-zboss-1.1.4/zigpy_zboss/uart.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss/utils.py` & `zigpy-zboss-1.1.4/zigpy_zboss/utils.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss/zigbee/application.py` & `zigpy-zboss-1.1.4/zigpy_zboss/zigbee/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -459,14 +459,18 @@
                 TSN=self.get_sequence(),
                 DestNWK=t.NWK(0x0000),
                 PermitDuration=t.uint8_t(time_s),
                 TCSignificance=t.uint8_t(0x01),
             )
         )
 
+    def permit_with_key(self, node, code, time_s=60):
+        """Permit with key."""
+        raise NotImplementedError
+
     def permit_with_link_key(self, node, link_key, time_s=60):
         """Permit with link key."""
         raise NotImplementedError
 
     @property
     def zboss_config(self) -> conf.ConfigType:
         """Shortcut property to access the ZBOSS radio config."""
@@ -623,14 +627,18 @@
         """Send packets."""
         if self._api is None:
             raise DeliveryError(
                 "Coordinator is disconnected, cannot send request")
 
         LOGGER.debug("Sending packet %r", packet)
 
+        if zigpy.zdo.ZDO_ENDPOINT in (packet.src_ep, packet.dst_ep):
+            await self._device.zdo.zboss_specific_cmd(packet)
+            return
+
         options = c.aps.TransmitOptions.NONE
 
         if t.TransmitOptions.ACK in packet.tx_options:
             options |= c.aps.TransmitOptions.ACK_ENABLED
 
         if t.TransmitOptions.APS_Encryption in packet.tx_options:
             options |= c.aps.TransmitOptions.SECURITY_ENABLED
```

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss/zigbee/device.py` & `zigpy-zboss-1.1.4/zigpy_zboss/zigbee/device.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 """Zigbee device object."""
 import logging
 import zigpy.util
 import zigpy.device
 import zigpy.endpoint
 import zigpy.types as t
 import zigpy_zboss.types as t_zboss
+from typing import Any
 from zigpy_zboss import commands as c
 from zigpy.zdo import types as zdo_t
 from zigpy.zdo import ZDO as ZigpyZDO
 
 
+LOGGER = logging.getLogger(__name__)
+
+
 class ZbossZDO(ZigpyZDO):
-    """The ZDO endpoint of a device."""
+    """The ZDO endpoint of a ZBOSS device."""
 
     def handle_mgmt_permit_joining_req(
         self,
         permit_duration: int,
         tc_significance: int,
     ):
         """Handle ZDO permit joining request."""
@@ -220,14 +224,80 @@
                 DstNWK=t.NWK(0x0000),
             )
         )
         if res.StatusCode != 0:
             return (None, None, None, None, None)
         return (None, res.ScannedChannels, None, None, res.EnergyValues)
 
+    async def zboss_specific_cmd(self, packet: t.ZigbeePacket) -> None:
+        """Reroute ZDO packet sent over APSDE to custom ZBOSS ZDO commands."""
+        try:
+            zdo_hdr, zdo_args = self.deserialize(
+                cluster_id=packet.cluster_id, data=packet.data.serialize()
+            )
+        except ValueError:
+            LOGGER.debug("Could not parse ZDO message from packet")
+            return
+
+        if zdo_hdr.command_id == zdo_t.ZDOCmd.IEEE_addr_req:
+            await self._IEEE_addr_req(packet, zdo_hdr, zdo_args)
+
+    async def _IEEE_addr_req(
+            self,
+            packet: t.ZigbeePacket,
+            zdo_hdr: zdo_t.ZDOHeader,
+            zdo_args: tuple[Any]) -> None:
+        """Send ZDO IEEE addr request and handle the response."""
+        tsn = zdo_hdr.tsn
+        nwki, req_type, index = zdo_args
+        res = await self._api.request(
+            c.ZDO.IeeeAddrReq.Req(
+                TSN=tsn,
+                DstNWK=packet.dst.address,
+                NWKtoMatch=nwki,
+                RequestType=req_type,
+                StartIndex=index,
+                )
+        )
+
+        if res.StatusCode:
+            # ZDO command failed, use dummy values.
+            ieee = t.EUI64([0xff, 0xff, 0xff, 0xff, 0xff, 0xff, 0xff, 0xff])
+            nwki = t.NWK(0xffff)
+        else:
+            ieee = res.RemoteDevIEEE
+            nwki = res.RemoteDevNWK
+
+        status = zdo_t.Status(res.StatusCode)
+        data = tsn.serialize() \
+            + status.serialize() \
+            + ieee.serialize() \
+            + nwki.serialize()
+
+        packet = t.ZigbeePacket(
+            src=t.AddrModeAddress(
+                addr_mode=t.AddrMode.NWK,
+                address=res.RemoteDevNWK,
+            ),
+            src_ep=0,
+            dst=t.AddrModeAddress(
+                addr_mode=t.AddrMode.NWK,
+                address=self.state.node_info.nwk,
+            ),
+            dst_ep=0,
+            tsn=tsn,
+            profile_id=0,
+            cluster_id=zdo_t.ZDOCmd.IEEE_addr_rsp,
+            data=t.SerializableBytes(data),
+            tx_options=t.TransmitOptions.NONE,
+            lqi=None,
+            rssi=None
+        )
+        self._device._application.packet_received(packet)
+
 
 class ZbossDevice(zigpy.device.Device):
     """Class representing an nRF device."""
 
     def __init__(self, *args, **kwargs):
         """Initialize instance."""
         super().__init__(*args, **kwargs)
```

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss.egg-info/PKG-INFO` & `zigpy-zboss-1.1.4/zigpy_zboss.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigpy-zboss
-Version: 1.1.3
+Version: 1.1.4
 Summary: A library for zigpy which communicates with Nordic nRF52 radios
 Home-page: https://github.com/kardia-as/zigpy-zboss
 Author: Damien Kastner
 Author-email: damien.kastner@kardia.no
 License: GPL-3.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
@@ -26,14 +26,22 @@
 
 # zigpy-zboss
 
 **zigpy-zboss** is a Python library project that adds support for common Nordic Semiconductor nRF modules to **[zigpy (a open source Python Zigbee stack project)](https://github.com/zigpy/)** and other Network Co-Processor radios that uses firmware based on **[ZOI (ZBOSS Open Initiative) by DSR](https://dsr-zoi.com/)**.
 
 Together with the zigpy library and a home automation software application with compatible Zigbee gateway implementation, (such as for example the **[Home Assistant's ZHA integration component](https://www.home-assistant.io/integrations/zha/)**), you can directly control Zigbee devices from most product manufacturers, like; IKEA, Philips Hue, Inovelli, LEDVANCE/OSRAM, SmartThings/Samsung, SALUS/Computime, SONOFF/ITEAD, Xiaomi/Aqara, and many more.
 
+# Back-story and use cases
+
+This is currently an 'as-is' independent and unofficial implementation radio library for zigpy, as such should be considered experimental and you should only expect best-effort support from volunteers in the open-source community!
+
+Zigbee NCP support for ZOI (ZBOSS Open Initiative) based Zigbee radios compatible with ZBOSS NCP firmware for zigpy based Zigbee gateway implementation is still in very early development. 
+
+Development is initially focused on Zigbee Coordinator functionality Nordic Semiconductor's development kit hardware which has been tested to be compatible. Those also officially recognized as Zigbee-Compliant platforms by the CSA (Connectivity Standards Alliance, formerly the Zigbee Alliance), of which both [DSR Cooperation](https://pt.dsr-corporation.com/news/zboss-open-initiative-in-2021/) and [Nordic Semiconductor](https://developer.nordicsemi.com/nRF_Connect_SDK/doc/zboss/) are board and promoter members of.
+
 # Hardware requirements
 
 Nordic Semi USB adapters and development kits/boards based on nRF52840 SoC are used as reference hardware in the zigpy-zboss project:
 
 - **[nRF52840 dongle](https://www.nordicsemi.com/Products/Development-hardware/nrf52840-dongle)**
 - **[nRF52840 development kit](https://www.nordicsemi.com/Products/Development-hardware/nrf52840-dk)**
```

### Comparing `zigpy-zboss-1.1.3/zigpy_zboss.egg-info/SOURCES.txt` & `zigpy-zboss-1.1.4/zigpy_zboss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

