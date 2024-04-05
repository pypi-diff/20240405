# Comparing `tmp/pyprland-2.1.4.tar.gz` & `tmp/pyprland-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprland-2.1.4.tar", max compression
+gzip compressed data, was "pyprland-2.2.0.tar", max compression
```

## Comparing `pyprland-2.1.4.tar` & `pyprland-2.2.0.tar`

### file list

```diff
@@ -1,69 +1,33 @@
--rw-r--r--   0        0        0     1070 2024-02-16 16:53:56.731771 pyprland-2.1.4/LICENSE
--rw-r--r--   0        0        0     5338 2024-03-31 23:50:07.712880 pyprland-2.1.4/README.md
--rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.1.4/pyprland/__init__.py
--rw-r--r--   0        0        0        0 2024-03-02 14:42:00.069047 pyprland-2.1.4/pyprland/__init__.py,cover
--rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.1.4/pyprland/adapters/__init__.py
--rw-r--r--   0        0        0        0 2024-03-02 14:42:00.069047 pyprland-2.1.4/pyprland/adapters/__init__.py,cover
--rw-r--r--   0        0        0      165 2024-03-03 01:49:11.929817 pyprland-2.1.4/pyprland/adapters/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     7499 2024-03-03 11:48:19.793333 pyprland-2.1.4/pyprland/adapters/__pycache__/menus.cpython-311.pyc
--rw-r--r--   0        0        0     4377 2024-03-03 01:47:24.894367 pyprland-2.1.4/pyprland/adapters/menus.py
--rw-r--r--   0        0        0     4703 2024-03-02 14:42:00.072380 pyprland-2.1.4/pyprland/adapters/menus.py,cover
--rwxr-xr-x   0        0        0    15373 2024-04-03 21:51:25.315300 pyprland-2.1.4/pyprland/command.py
--rw-r--r--   0        0        0    15442 2024-03-02 14:42:00.079047 pyprland-2.1.4/pyprland/command.py,cover
--rwxr-xr-x   0        0        0    15518 2024-03-30 19:02:09.575863 pyprland-2.1.4/pyprland/command.py.orig
--rw-r--r--   0        0        0     4133 2024-03-03 01:47:24.921035 pyprland-2.1.4/pyprland/common.py
--rw-r--r--   0        0        0     4409 2024-03-02 14:42:00.079047 pyprland-2.1.4/pyprland/common.py,cover
--rw-r--r--   0        0        0     5948 2024-03-31 20:05:57.091220 pyprland-2.1.4/pyprland/ipc.py
--rw-r--r--   0        0        0     6104 2024-03-02 14:42:00.082381 pyprland-2.1.4/pyprland/ipc.py,cover
--rw-r--r--   0        0        0       45 2024-03-03 01:47:24.897701 pyprland-2.1.4/pyprland/plugins/__init__.py
--rw-r--r--   0        0        0       49 2024-03-02 14:42:00.082381 pyprland-2.1.4/pyprland/plugins/__init__.py,cover
--rw-r--r--   0        0        0      227 2024-03-03 01:49:11.929817 pyprland-2.1.4/pyprland/plugins/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2902 2024-03-03 11:48:21.296667 pyprland-2.1.4/pyprland/plugins/__pycache__/expose.cpython-311.pyc
--rw-r--r--   0        0        0     3207 2024-03-30 18:24:39.387692 pyprland-2.1.4/pyprland/plugins/__pycache__/fetch_client_menu.cpython-311.pyc
--rw-r--r--   0        0        0     3905 2024-03-03 01:50:19.494487 pyprland-2.1.4/pyprland/plugins/__pycache__/interface.cpython-311.pyc
--rw-r--r--   0        0        0    14058 2024-03-03 11:48:21.256667 pyprland-2.1.4/pyprland/plugins/__pycache__/layout_center.cpython-311.pyc
--rw-r--r--   0        0        0     3740 2024-03-03 11:48:21.256667 pyprland-2.1.4/pyprland/plugins/__pycache__/lost_windows.cpython-311.pyc
--rw-r--r--   0        0        0     1814 2024-04-03 21:48:46.484412 pyprland-2.1.4/pyprland/plugins/__pycache__/magnify.cpython-311.pyc
--rw-r--r--   0        0        0    13040 2024-03-31 17:52:50.637188 pyprland-2.1.4/pyprland/plugins/__pycache__/monitors.cpython-311.pyc
--rw-r--r--   0        0        0     2817 2024-03-03 11:48:19.756667 pyprland-2.1.4/pyprland/plugins/__pycache__/pyprland.cpython-311.pyc
--rw-r--r--   0        0        0    54691 2024-04-03 21:46:08.496667 pyprland-2.1.4/pyprland/plugins/__pycache__/scratchpads.cpython-311.pyc
--rw-r--r--   0        0        0     2600 2024-03-03 11:48:21.263333 pyprland-2.1.4/pyprland/plugins/__pycache__/shift_monitors.cpython-311.pyc
--rw-r--r--   0        0        0     7268 2024-03-03 11:48:19.790000 pyprland-2.1.4/pyprland/plugins/__pycache__/shortcuts_menu.cpython-311.pyc
--rw-r--r--   0        0        0     5631 2024-03-03 11:48:19.803333 pyprland-2.1.4/pyprland/plugins/__pycache__/system_notifier.cpython-311.pyc
--rw-r--r--   0        0        0     1582 2024-03-03 11:48:21.296667 pyprland-2.1.4/pyprland/plugins/__pycache__/toggle_dpms.cpython-311.pyc
--rw-r--r--   0        0        0     1916 2024-03-03 11:48:19.803333 pyprland-2.1.4/pyprland/plugins/__pycache__/toggle_special.cpython-311.pyc
--rw-r--r--   0        0        0     5090 2024-03-03 11:48:21.296667 pyprland-2.1.4/pyprland/plugins/__pycache__/workspaces_follow_focus.cpython-311.pyc
--rw-r--r--   0        0        0      106 2024-03-03 01:47:24.897701 pyprland-2.1.4/pyprland/plugins/experimental.py
--rw-r--r--   0        0        0     1647 2024-03-03 01:47:24.914368 pyprland-2.1.4/pyprland/plugins/expose.py
--rw-r--r--   0        0        0     1733 2024-03-02 14:42:00.082381 pyprland-2.1.4/pyprland/plugins/expose.py,cover
--rw-r--r--   0        0        0     1386 2024-03-30 16:09:04.631012 pyprland-2.1.4/pyprland/plugins/fetch_client_menu.py
--rw-r--r--   0        0        0      978 2024-03-02 14:42:00.082381 pyprland-2.1.4/pyprland/plugins/fetch_client_menu.py,cover
--rw-r--r--   0        0        0     2601 2024-03-03 01:47:24.901034 pyprland-2.1.4/pyprland/plugins/interface.py
--rw-r--r--   0        0        0     2771 2024-03-02 14:42:00.085714 pyprland-2.1.4/pyprland/plugins/interface.py,cover
--rw-r--r--   0        0        0     7972 2024-03-03 01:47:24.917701 pyprland-2.1.4/pyprland/plugins/layout_center.py
--rw-r--r--   0        0        0     8414 2024-03-02 14:42:00.085714 pyprland-2.1.4/pyprland/plugins/layout_center.py,cover
--rw-r--r--   0        0        0     1677 2024-03-03 01:47:24.901034 pyprland-2.1.4/pyprland/plugins/lost_windows.py
--rw-r--r--   0        0        0     1765 2024-03-02 14:42:00.089047 pyprland-2.1.4/pyprland/plugins/lost_windows.py,cover
--rw-r--r--   0        0        0     1239 2024-04-03 21:48:38.877707 pyprland-2.1.4/pyprland/plugins/magnify.py
--rw-r--r--   0        0        0      801 2024-03-02 14:42:00.089047 pyprland-2.1.4/pyprland/plugins/magnify.py,cover
--rw-r--r--   0        0        0     8684 2024-03-31 17:52:13.879696 pyprland-2.1.4/pyprland/plugins/monitors.py
--rw-r--r--   0        0        0    12264 2024-03-02 14:42:00.092381 pyprland-2.1.4/pyprland/plugins/monitors.py,cover
--rw-r--r--   0        0        0     8720 2024-03-30 19:02:09.575863 pyprland-2.1.4/pyprland/plugins/monitors.py.orig
--rw-r--r--   0        0        0     3922 2024-03-03 01:47:24.904368 pyprland-2.1.4/pyprland/plugins/monitors_v0.py
--rw-r--r--   0        0        0     1218 2024-03-03 01:47:24.907701 pyprland-2.1.4/pyprland/plugins/pyprland.py
--rw-r--r--   0        0        0     1286 2024-03-02 14:42:00.092381 pyprland-2.1.4/pyprland/plugins/pyprland.py,cover
--rw-r--r--   0        0        0    35404 2024-04-03 18:49:20.111659 pyprland-2.1.4/pyprland/plugins/scratchpads.py
--rw-r--r--   0        0        0    36868 2024-03-02 14:42:00.102381 pyprland-2.1.4/pyprland/plugins/scratchpads.py,cover
--rw-r--r--   0        0        0     1058 2024-03-03 01:47:24.907701 pyprland-2.1.4/pyprland/plugins/shift_monitors.py
--rw-r--r--   0        0        0     1126 2024-03-02 14:42:00.105714 pyprland-2.1.4/pyprland/plugins/shift_monitors.py,cover
--rw-r--r--   0        0        0     4122 2024-03-03 01:47:24.917701 pyprland-2.1.4/pyprland/plugins/shortcuts_menu.py
--rw-r--r--   0        0        0     4340 2024-03-02 14:42:00.105714 pyprland-2.1.4/pyprland/plugins/shortcuts_menu.py,cover
--rw-r--r--   0        0        0     3124 2024-03-03 01:47:24.911034 pyprland-2.1.4/pyprland/plugins/system_notifier.py
--rw-r--r--   0        0        0      519 2024-03-03 01:47:24.911034 pyprland-2.1.4/pyprland/plugins/toggle_dpms.py
--rw-r--r--   0        0        0      549 2024-03-02 14:42:00.105714 pyprland-2.1.4/pyprland/plugins/toggle_dpms.py,cover
--rw-r--r--   0        0        0     1063 2024-03-03 01:47:24.917701 pyprland-2.1.4/pyprland/plugins/toggle_special.py
--rw-r--r--   0        0        0     1117 2024-03-02 14:42:00.105714 pyprland-2.1.4/pyprland/plugins/toggle_special.py,cover
--rw-r--r--   0        0        0     2589 2024-03-03 01:47:24.911034 pyprland-2.1.4/pyprland/plugins/workspaces_follow_focus.py
--rw-r--r--   0        0        0     2731 2024-03-02 14:42:00.109048 pyprland-2.1.4/pyprland/plugins/workspaces_follow_focus.py,cover
--rw-r--r--   0        0        0      725 2024-04-03 21:51:25.295300 pyprland-2.1.4/pyproject.toml
--rw-r--r--   0        0        0     5877 1970-01-01 00:00:00.000000 pyprland-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-02-16 16:53:56.731771 pyprland-2.2.0/LICENSE
+-rw-r--r--   0        0        0     5366 2024-04-03 21:58:48.932070 pyprland-2.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.0/pyprland/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.0/pyprland/adapters/__init__.py
+-rw-r--r--   0        0        0      400 2024-04-05 20:13:47.397221 pyprland-2.2.0/pyprland/adapters/colors.py
+-rw-r--r--   0        0        0     4377 2024-03-03 01:47:24.894367 pyprland-2.2.0/pyprland/adapters/menus.py
+-rwxr-xr-x   0        0        0    15685 2024-04-05 21:22:04.241803 pyprland-2.2.0/pyprland/command.py
+-rwxr-xr-x   0        0        0    15815 2024-04-05 21:08:59.846455 pyprland-2.2.0/pyprland/command.py.orig
+-rw-r--r--   0        0        0     4133 2024-03-03 01:47:24.921035 pyprland-2.2.0/pyprland/common.py
+-rw-r--r--   0        0        0     5948 2024-03-31 20:05:57.091220 pyprland-2.2.0/pyprland/ipc.py
+-rw-r--r--   0        0        0       45 2024-03-03 01:47:24.897701 pyprland-2.2.0/pyprland/plugins/__init__.py
+-rw-r--r--   0        0        0      106 2024-03-03 01:47:24.897701 pyprland-2.2.0/pyprland/plugins/experimental.py
+-rw-r--r--   0        0        0     1647 2024-03-03 01:47:24.914368 pyprland-2.2.0/pyprland/plugins/expose.py
+-rw-r--r--   0        0        0     1386 2024-03-30 16:09:04.631012 pyprland-2.2.0/pyprland/plugins/fetch_client_menu.py
+-rw-r--r--   0        0        0     2601 2024-03-03 01:47:24.901034 pyprland-2.2.0/pyprland/plugins/interface.py
+-rw-r--r--   0        0        0     7972 2024-03-03 01:47:24.917701 pyprland-2.2.0/pyprland/plugins/layout_center.py
+-rw-r--r--   0        0        0     1677 2024-03-03 01:47:24.901034 pyprland-2.2.0/pyprland/plugins/lost_windows.py
+-rw-r--r--   0        0        0     1239 2024-04-03 21:48:38.877707 pyprland-2.2.0/pyprland/plugins/magnify.py
+-rw-r--r--   0        0        0     8684 2024-03-31 17:52:13.879696 pyprland-2.2.0/pyprland/plugins/monitors.py
+-rw-r--r--   0        0        0     8720 2024-03-30 19:02:09.575863 pyprland-2.2.0/pyprland/plugins/monitors.py.orig
+-rw-r--r--   0        0        0     3922 2024-03-03 01:47:24.904368 pyprland-2.2.0/pyprland/plugins/monitors_v0.py
+-rw-r--r--   0        0        0        0 2024-04-04 16:21:22.101700 pyprland-2.2.0/pyprland/plugins/nohup.out
+-rw-r--r--   0        0        0     1218 2024-03-03 01:47:24.907701 pyprland-2.2.0/pyprland/plugins/pyprland.py
+-rw-r--r--   0        0        0    35284 2024-04-05 11:26:39.264749 pyprland-2.2.0/pyprland/plugins/scratchpads.py
+-rw-r--r--   0        0        0     1058 2024-03-03 01:47:24.907701 pyprland-2.2.0/pyprland/plugins/shift_monitors.py
+-rw-r--r--   0        0        0     4122 2024-03-03 01:47:24.917701 pyprland-2.2.0/pyprland/plugins/shortcuts_menu.py
+-rw-r--r--   0        0        0     3983 2024-04-05 20:13:47.397221 pyprland-2.2.0/pyprland/plugins/system_notifier.py
+-rw-r--r--   0        0        0      519 2024-03-03 01:47:24.911034 pyprland-2.2.0/pyprland/plugins/toggle_dpms.py
+-rw-r--r--   0        0        0     1063 2024-03-03 01:47:24.917701 pyprland-2.2.0/pyprland/plugins/toggle_special.py
+-rw-r--r--   0        0        0     3764 2024-04-05 20:13:47.397221 pyprland-2.2.0/pyprland/plugins/wallpapers.py
+-rw-r--r--   0        0        0     2589 2024-03-03 01:47:24.911034 pyprland-2.2.0/pyprland/plugins/workspaces_follow_focus.py
+-rw-r--r--   0        0        0      725 2024-04-05 21:21:12.163408 pyprland-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5905 1970-01-01 00:00:00.000000 pyprland-2.2.0/PKG-INFO
```

### Comparing `pyprland-2.1.4/LICENSE` & `pyprland-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.4/README.md` & `pyprland-2.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 Check the [Releases change log](https://github.com/hyprland-community/pyprland/releases) for more information
 
 
 ### 2.1
 
 - Requires Hyprland >= 0.37
 - [monitors](https://github.com/hyprland-community/pyprland/wiki//monitors)
-  - Drops the `wlr-randr` dependency
+  - Drops the `wlr-randr` dependency (used in `monitors` plugin)
   - simplified the syntax, no need for `()` around a screen name (will try matching the exact name first, then partial description)
 
 ### 2.0
 
 - New dependency: [aiofiles](https://pypi.org/project/aiofiles/)
     - fully asynchronous plugins, including file operations
 - Added [hysteresis](https://github.com/hyprland-community/pyprland/wiki/scratchpads#hysteresis-optional) support for [scratchpads](https://github.com/hyprland-community/pyprland/wiki/scratchpads) in 2.0.1, only active if `unfocus="hide"` is set.
```

### Comparing `pyprland-2.1.4/pyprland/adapters/menus.py` & `pyprland-2.2.0/pyprland/adapters/menus.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.4/pyprland/command.py` & `pyprland-2.2.0/pyprland/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,54 +82,69 @@
                     "No config file found, create one at ~/.config/hypr/pyprland.json with a valid pyprland.plugins list"
                 )
                 raise PyprError() from e
         else:
             self.log.critical("No Config file found ! Please create %s", CONFIG_FILE)
             raise PyprError()
 
+    async def _load_single_plugin(self, name, init) -> bool:
+        "Load a single plugin, optionally calling `init`"
+        if "." in name:
+            modname = name
+        elif "external:" in name:
+            modname = name.replace("external:", "")
+        else:
+            modname = f"pyprland.plugins.{name}"
+        try:
+            plug = importlib.import_module(modname).Extension(name)
+            if init:
+                await plug.init()
+                self.queues[name] = asyncio.Queue()
+                if self.tasks:
+                    self.tasks.create_task(self._plugin_runner_loop(name))
+            self.plugins[name] = plug
+        except ModuleNotFoundError as e:
+            self.log.error("Unable to locate plugin called '%s'", name)
+            await notify_info(
+                f'Config requires plugin "{name}" but pypr can\'t find it: {e}'
+            )
+            return False
+        except Exception as e:
+            await notify_info(f"Error loading plugin {name}: {e}")
+            self.log.error("Error loading plugin %s:", name, exc_info=True)
+            raise PyprError() from e
+        return True
+
     async def __load_plugins_config(self, init=True):
         """Loads the plugins mentioned in the config.
         If init is `True`, call the `init()` method on each plugin.
         """
+
+        sys.path.extend(self.config["pyprland"].get("plugins_paths", []))
+
         init_pyprland = "pyprland" not in self.plugins
+
         for name in ["pyprland"] + self.config["pyprland"]["plugins"]:
             if name not in self.plugins:
-                modname = name if "." in name else f"pyprland.plugins.{name}"
-                try:
-                    plug = importlib.import_module(modname).Extension(name)
-                    if init:
-                        await plug.init()
-                        self.queues[name] = asyncio.Queue()
-                        if self.tasks:
-                            self.tasks.create_task(self._plugin_runner_loop(name))
-                    self.plugins[name] = plug
-                except ModuleNotFoundError as e:
-                    self.log.error("Unable to locate plugin called '%s'", name)
-                    await notify_info(
-                        f'Config requires plugin "{name}" but pypr can\'t find it: {e}'
-                    )
+                if not await self._load_single_plugin(name, init):
                     continue
-                except Exception as e:
-                    await notify_info(f"Error loading plugin {name}: {e}")
-                    self.log.error("Error loading plugin %s:", name, exc_info=True)
-                    raise PyprError() from e
             if init:
                 try:
                     await self.plugins[name].load_config(self.config)
                     await self.plugins[name].on_reload()
                     self.plugins[name].log.info("configured")
                 except PyprError:
                     raise
                 except Exception as e:
                     await notify_info(f"Error initializing plugin {name}: {e}")
                     self.log.error("Error initializing plugin %s:", name, exc_info=True)
                     raise PyprError() from e
         if init_pyprland:
             plug = self.plugins["pyprland"]
-            plug.set_commands(reload=self.load_config)
+            plug.set_commands(reload=self.load_config)  # type: ignore
 
     async def load_config(self, init=True):
         """loads the configuration (new plugins will be added & config updated)
 
         if `init` is true, also initializes the plugins"""
 
         await self.__open_config()
@@ -329,15 +344,15 @@
 
 
 async def run_client():
     "Runs the client (CLI)"
     manager = Pyprland()
 
     if sys.argv[1] == "version":
-        print('2.1.4-1')  # Automatically updated version
+        print("2.1.4-23")  # Automatically updated version
         return
 
     if sys.argv[1] in ("--help", "-h", "help"):
         await manager.load_config(init=False)
 
         def format_doc(txt):
             return txt.split("\n")[0]
```

### Comparing `pyprland-2.1.4/pyprland/command.py,cover` & `pyprland-2.2.0/pyprland/command.py.orig`

 * *Files 18% similar despite different names*

```diff
@@ -1,411 +1,451 @@
-  #!/bin/env python
-> """ Pyprland - an Hyprland companion app (cli client & daemon) """
-> import asyncio
-> import importlib
-> import itertools
-> from functools import partial
-> from typing import Self
-> import tomllib
-> import json
-> import os
-> import sys
-  
-> from pyprland.common import PyprError, get_logger, init_logger
-> from pyprland.ipc import get_event_stream, notify_error, notify_fatal, notify_info
-> from pyprland.ipc import init as ipc_init
-> from pyprland.plugins.interface import Plugin
-  
-> try:
->     CONTROL = f'/tmp/hypr/{ os.environ["HYPRLAND_INSTANCE_SIGNATURE"] }/.pyprland.sock'
-! except KeyError:
-!     print(
-!         "This is a fatal error, assuming we are running documentation generation hence ignoring it"
-!     )
-  
-> OLD_CONFIG_FILE = "~/.config/hypr/pyprland.json"
-> CONFIG_FILE = "~/.config/hypr/pyprland.toml"
-  
-> PYPR_DEMO = os.environ.get("PYPR_DEMO", False)
-  
-> __all__: list[str] = []
-  
-  
-> class Pyprland:
->     "Main app object"
->     server: asyncio.Server
->     event_reader: asyncio.StreamReader
->     stopped = False
->     config: dict[str, dict] = {}
->     tasks: None | asyncio.TaskGroup = None
->     instance: Self | None = None
-  
->     @classmethod
->     def _set_instance(cls, instance):
->         "Set instance reference into class (for testing/debugging only)"
->         cls.instance = instance
-  
->     def __init__(self):
->         self.config = {}
->         self.plugins: dict[str, Plugin] = {}
->         self.log = get_logger()
->         self.queues = {}
->         self._set_instance(self)
-  
->     async def initialize(self):
->         "Initializes the main structures"
->         await self.load_config()  # ensure sockets are connected first
-  
->     async def __open_config(self):
->         """Loads config file as self.config"""
->         if os.path.exists(OLD_CONFIG_FILE) and not os.path.exists(CONFIG_FILE):
-!             self.log.warning("Consider changing your configuration to TOML format.")
-  
->         self.config.clear()
->         fname = os.path.expanduser(CONFIG_FILE)
->         if os.path.exists(fname):
->             self.log.info("Loading %s", fname)
->             try:
->                 with open(fname, "rb") as f:
->                     self.config.update(tomllib.load(f))
-!             except FileNotFoundError as e:
-!                 self.log.critical(
-!                     "No config file found, create one at ~/.config/hypr/pyprland.json with a valid pyprland.plugins list"
-!                 )
-!                 raise PyprError() from e
-!         elif os.path.exists(os.path.expanduser(OLD_CONFIG_FILE)):
-!             self.log.info("Loading %s", OLD_CONFIG_FILE)
-!             try:
-!                 with open(os.path.expanduser(OLD_CONFIG_FILE), encoding="utf-8") as f:
-!                     self.config.update(json.loads(f.read()))
-!             except FileNotFoundError as e:
-!                 self.log.critical(
-!                     "No config file found, create one at ~/.config/hypr/pyprland.json with a valid pyprland.plugins list"
-!                 )
-!                 raise PyprError() from e
-!         else:
-!             self.log.critical("No Config file found ! Please create %s", CONFIG_FILE)
-!             raise PyprError()
-  
->     async def __load_plugins_config(self, init=True):
->         """Loads the plugins mentioned in the config.
->         If init is `True`, call the `init()` method on each plugin.
->         """
->         init_pyprland = "pyprland" not in self.plugins
->         for name in ["pyprland"] + self.config["pyprland"]["plugins"]:
->             if name not in self.plugins:
->                 modname = name if "." in name else f"pyprland.plugins.{name}"
->                 try:
->                     plug = importlib.import_module(modname).Extension(name)
->                     if init:
->                         await plug.init()
->                         self.queues[name] = asyncio.Queue()
->                         if self.tasks:
-!                             self.tasks.create_task(self._plugin_runner_loop(name))
->                     self.plugins[name] = plug
-!                 except ModuleNotFoundError as e:
-!                     self.log.error("Unable to locate plugin called '%s'", name)
-!                     await notify_info(
-!                         f'Config requires plugin "{name}" but pypr can\'t find it: {e}'
-!                     )
-!                     continue
-!                 except Exception as e:
-!                     await notify_info(f"Error loading plugin {name}: {e}")
-!                     self.log.error("Error loading plugin %s:", name, exc_info=True)
-!                     raise PyprError() from e
->             if init:
->                 try:
->                     await self.plugins[name].load_config(self.config)
->                     await self.plugins[name].on_reload()
->                     self.plugins[name].log.info("configured")
-!                 except PyprError:
-!                     raise
-!                 except Exception as e:
-!                     await notify_info(f"Error initializing plugin {name}: {e}")
-!                     self.log.error("Error initializing plugin %s:", name, exc_info=True)
-!                     raise PyprError() from e
->         if init_pyprland:
->             plug = self.plugins["pyprland"]
->             plug.set_commands(reload=self.load_config)
-  
->     async def load_config(self, init=True):
->         """loads the configuration (new plugins will be added & config updated)
-  
->         if `init` is true, also initializes the plugins"""
-  
->         await self.__open_config()
->         assert self.config
->         await self.__load_plugins_config(init=init)
-  
->     async def _run_plugin_handler(self, plugin, full_name, params):
->         "Runs a single handler on a plugin"
->         color = 33 if full_name.startswith("run_") else 30
->         plugin.log.debug(f"\033[{color};1m%s%s\033[0m", full_name, params)
->         try:
->             await getattr(plugin, full_name)(*params)
->         except AssertionError as e:
-!             self.log.error(
-!                 "This could be a bug in Pyprland, if you think so, report on https://github.com/fdev31/pyprland/issues"
-!             )
-!             self.log.exception(e)
-!             await notify_error(
-!                 f"Pypr integrity check failed on {plugin.name}::{full_name}: {e}"
-!             )
->         except Exception as e:  # pylint: disable=W0718
-!             self.log.warning("%s::%s(%s) failed:", plugin.name, full_name, params)
-!             self.log.exception(e)
-!             await notify_error(f"Pypr error {plugin.name}::{full_name}: {e}")
-  
->     async def _callHandler(self, full_name, *params, notify=""):
->         "Call an event handler with params"
->         handled = False
->         for plugin in self.plugins.values():
->             if hasattr(plugin, full_name):
->                 handled = True
->                 task = partial(self._run_plugin_handler, plugin, full_name, params)
->                 if plugin == "pyprland":
-!                     await task()
->                 else:
->                     await self.queues[plugin.name].put(task)
->         if notify and not handled:
->             await notify_info(f'"{notify}" not found')
->         return handled
-  
->     async def read_events_loop(self):
->         "Consumes the event loop and calls corresponding handlers"
->         while not self.stopped:
->             try:
->                 data = (await self.event_reader.readline()).decode()
->             except RuntimeError as e:
-!                 self.log.error("Aborting event loop: %s", e)
-!                 return
->             except UnicodeDecodeError:
-!                 self.log.error("Invalid unicode while reading events")
-!                 continue
->             if not data:
-!                 self.log.critical("Reader starved")
-!                 return
->             cmd, params = data.split(">>", 1)
->             full_name = f"event_{cmd}"
-  
-              # self.log.debug("[%s] %s", cmd, params.strip())
->             await self._callHandler(full_name, params.rstrip("\n"))
-  
->     async def read_command(self, reader, writer) -> None:
->         "Receives a socket command"
->         data = (await reader.readline()).decode()
->         if not data:
-!             self.log.critical("Server starved")
-!             data = "exit"
->         data = data.strip()
->         if data == "exit":
-!             self.stopped = True
-!             writer.close()
-!             await writer.wait_closed()
-!             self.server.close()
-!             return
->         args = data.split(None, 1)
->         if len(args) == 1:
->             cmd = args[0]
->             args = []
->         else:
->             cmd = args[0]
->             args = args[1:]
-  
->         full_name = f"run_{cmd}"
-  
->         if PYPR_DEMO:
-!             os.system(f"notify-send -t 4000 '{data}'")
-  
->         if not await self._callHandler(full_name, *args, notify=cmd):
->             self.log.warning("No such command: %s", cmd)
-  
->     async def serve(self):
->         "Runs the server"
->         try:
->             async with self.server:
->                 await self.server.serve_forever()
->         finally:
->             await asyncio.gather(*(plugin.exit() for plugin in self.plugins.values()))
-  
->     async def _plugin_runner_loop(self, name):
->         "Runs tasks for a given plugin indefinitely"
->         q = self.queues[name]
-  
->         while not self.stopped:
->             try:
->                 task = await q.get()
->             except RuntimeError as e:
-!                 self.log.error("Aborting [%s] loop: %s", name, e)
-!                 return
->             try:
->                 await task()
->             except Exception as e:  # pylint: disable=W0718
-!                 self.log.error(
-!                     "Unhandled error running plugin %s::%s: %s", name, task, e
-!                 )
-  
->     async def plugins_runner(self):
->         "Runs plugins' task using the created `tasks` TaskGroup attribute"
->         async with asyncio.TaskGroup() as group:
->             self.tasks = group
->             for name in self.plugins:
->                 group.create_task(self._plugin_runner_loop(name))
-  
->     async def run(self):
->         "Runs the server and the event listener"
->         await asyncio.gather(
->             asyncio.create_task(self.serve()),
->             asyncio.create_task(self.read_events_loop()),
->             asyncio.create_task(self.plugins_runner()),
->         )
-  
-  
-> async def run_daemon():
->     "Runs the server / daemon"
->     manager = Pyprland()
->     err_count = itertools.count()
->     manager.server = await asyncio.start_unix_server(manager.read_command, CONTROL)
->     max_retry = 10
->     while True:
->         attempt = next(err_count)
->         try:
->             events_reader, events_writer = await get_event_stream()
-!         except Exception as e:  # pylint: disable=W0718
-!             if attempt > max_retry:
-!                 manager.log.critical("Failed to open hyprland event stream: %s.", e)
-!                 await notify_fatal("Failed to open hyprland event stream")
-!                 raise PyprError() from e
-!             manager.log.warning(
-!                 "Failed to get event stream: %s, retry %s/%s...", e, attempt, max_retry
-!             )
-!             await asyncio.sleep(1)
->         else:
->             break
-  
->     manager.event_reader = events_reader
-  
->     try:
->         await manager.initialize()
-!     except PyprError as e:
-!         if bool(str(e)):
-!             await notify_fatal(f"Pypr failed to start: {e}")
-!         else:
-!             await notify_fatal("Pypr failed to start!")
-  
-!         raise SystemExit(1) from e
-!     except Exception as e:
-!         manager.log.critical("Failed to load config.", exc_info=True)
-!         await notify_fatal(f"Pypr couldn't load config: {e}")
-!         raise SystemExit(1) from e
-  
->     manager.log.debug("[ initialized ]".center(80, "="))
->     try:
->         await manager.run()
->     except KeyboardInterrupt:
-!         print("Interrupted")
->     except asyncio.CancelledError:
->         manager.log.critical("cancelled")
->     finally:
->         events_writer.close()
->         await events_writer.wait_closed()
->         manager.server.close()
->         await manager.server.wait_closed()
-  
-  
-> async def run_client():
->     "Runs the client (CLI)"
-!     manager = Pyprland()
-!     if sys.argv[1] in ("--help", "-h", "help"):
-!         await manager.load_config(init=False)
-  
-!         def format_doc(txt):
-!             return txt.split("\n")[0]
-  
-!         print(
-!             """Syntax: pypr [command]
-  
-! If the command is ommited, runs the daemon which will start every configured plugin.
-  
-! Available commands:
-! """
-!         )
-!         for plug in manager.plugins.values():
-!             for name in dir(plug):
-!                 if name.startswith("run_"):
-!                     fn = getattr(plug, name)
-!                     if callable(fn):
-!                         print(
-!                             f" {name[4:]:20s} {format_doc(fn.__doc__) if fn.__doc__ else 'N/A'} [{plug.name}]"
-!                         )
-  
-!         return
-  
-!     try:
-!         _, writer = await asyncio.open_unix_connection(CONTROL)
-!     except (ConnectionRefusedError, FileNotFoundError) as e:
-!         manager.log.critical("Failed to open control socket, is pypr daemon running ?")
-!         await notify_error("Pypr can't connect, is daemon running ?")
-!         raise PyprError() from e
-  
-!     args = sys.argv[1:]
-!     args[0] = args[0].replace("-", "_")
-!     writer.write((" ".join(args)).encode())
-!     await writer.drain()
-!     writer.close()
-!     await writer.wait_closed()
-  
-  
-> def use_param(txt):
->     """Checks if parameter `txt` is in sys.argv
->     if found, removes it from sys.argv & returns the argument value
->     """
-!     v = ""
-!     if txt in sys.argv:
-!         i = sys.argv.index(txt)
-!         v = sys.argv[i + 1]
-!         del sys.argv[i : i + 2]
-!     return v
-  
-  
-> def main():
->     "runs the command"
-!     debug_flag = use_param("--debug")
-!     if debug_flag:
-!         init_logger(filename=debug_flag, force_debug=True)
-!     else:
-!         init_logger()
-!     ipc_init()
-!     log = get_logger("startup")
-  
-!     config_override = use_param("--config")
-!     if config_override:
-!         global CONFIG_FILE
-!         CONFIG_FILE = config_override
-  
-!     invoke_daemon = len(sys.argv) <= 1
-!     if invoke_daemon and os.path.exists(CONTROL):
-!         asyncio.run(notify_fatal("Trying to run pypr more than once ?"))
-!         log.critical(
-!             """%s exists,
-! is pypr already running ?
-! If that's not the case, delete this file and run again.""",
-!             CONTROL,
-!         )
-!     else:
-!         try:
-!             asyncio.run(run_daemon() if invoke_daemon else run_client())
-!         except KeyboardInterrupt:
-!             pass
-!         except PyprError:
-!             log.critical("Command failed.")
-!         except json.decoder.JSONDecodeError as e:
-!             log.critical("Invalid JSON syntax in the config file: %s", e.args[0])
-!         except Exception:  # pylint: disable=W0718
-!             log.critical("Unhandled exception:", exc_info=True)
-!         finally:
-!             if invoke_daemon:
-!                 os.unlink(CONTROL)
-  
-  
-> if __name__ == "__main__":
-!     main()
+#!/bin/env python
+""" Pyprland - an Hyprland companion app (cli client & daemon) """
+import asyncio
+import importlib
+import itertools
+from functools import partial
+from typing import Self
+import tomllib
+import json
+import os
+import sys
+
+from pyprland.common import PyprError, get_logger, init_logger
+from pyprland.ipc import get_event_stream, notify_error, notify_fatal, notify_info
+from pyprland.ipc import init as ipc_init
+from pyprland.plugins.interface import Plugin
+
+try:
+    CONTROL = f'/tmp/hypr/{ os.environ["HYPRLAND_INSTANCE_SIGNATURE"] }/.pyprland.sock'
+except KeyError:
+    print(
+        "This is a fatal error, assuming we are running documentation generation hence ignoring it"
+    )
+
+OLD_CONFIG_FILE = "~/.config/hypr/pyprland.json"
+CONFIG_FILE = "~/.config/hypr/pyprland.toml"
+
+PYPR_DEMO = os.environ.get("PYPR_DEMO", False)
+
+__all__: list[str] = []
+
+
+class Pyprland:
+    "Main app object"
+    server: asyncio.Server
+    event_reader: asyncio.StreamReader
+    stopped = False
+    config: dict[str, dict] = {}
+    tasks: None | asyncio.TaskGroup = None
+    instance: Self | None = None
+
+    @classmethod
+    def _set_instance(cls, instance):
+        "Set instance reference into class (for testing/debugging only)"
+        cls.instance = instance
+
+    def __init__(self):
+        self.config = {}
+        self.plugins: dict[str, Plugin] = {}
+        self.log = get_logger()
+        self.queues = {}
+        self._set_instance(self)
+
+    async def initialize(self):
+        "Initializes the main structures"
+        await self.load_config()  # ensure sockets are connected first
+
+    async def __open_config(self):
+        """Loads config file as self.config"""
+        if os.path.exists(OLD_CONFIG_FILE) and not os.path.exists(CONFIG_FILE):
+            self.log.warning("Consider changing your configuration to TOML format.")
+
+        self.config.clear()
+        fname = os.path.expanduser(CONFIG_FILE)
+        if os.path.exists(fname):
+            self.log.info("Loading %s", fname)
+            try:
+                with open(fname, "rb") as f:
+                    self.config.update(tomllib.load(f))
+            except FileNotFoundError as e:
+                self.log.critical(
+                    "No config file found, create one at ~/.config/hypr/pyprland.json with a valid pyprland.plugins list"
+                )
+                raise PyprError() from e
+        elif os.path.exists(os.path.expanduser(OLD_CONFIG_FILE)):
+            self.log.info("Loading %s", OLD_CONFIG_FILE)
+            try:
+                with open(os.path.expanduser(OLD_CONFIG_FILE), encoding="utf-8") as f:
+                    self.config.update(json.loads(f.read()))
+            except FileNotFoundError as e:
+                self.log.critical(
+                    "No config file found, create one at ~/.config/hypr/pyprland.json with a valid pyprland.plugins list"
+                )
+                raise PyprError() from e
+        else:
+            self.log.critical("No Config file found ! Please create %s", CONFIG_FILE)
+            raise PyprError()
+
+    async def _load_single_plugin(self, name, init) -> bool:
+        "Load a single plugin, optionally calling `init`"
+        if "." in name:
+            modname = name
+        elif "external:" in name:
+            modname = name.replace("external:", "")
+        else:
+            modname = f"pyprland.plugins.{name}"
+        try:
+            plug = importlib.import_module(modname).Extension(name)
+            if init:
+                await plug.init()
+                self.queues[name] = asyncio.Queue()
+                if self.tasks:
+                    self.tasks.create_task(self._plugin_runner_loop(name))
+            self.plugins[name] = plug
+        except ModuleNotFoundError as e:
+            self.log.error("Unable to locate plugin called '%s'", name)
+            await notify_info(
+                f'Config requires plugin "{name}" but pypr can\'t find it: {e}'
+            )
+            return False
+        except Exception as e:
+            await notify_info(f"Error loading plugin {name}: {e}")
+            self.log.error("Error loading plugin %s:", name, exc_info=True)
+            raise PyprError() from e
+        return True
+
+    async def __load_plugins_config(self, init=True):
+        """Loads the plugins mentioned in the config.
+        If init is `True`, call the `init()` method on each plugin.
+        """
+
+        sys.path.extend(self.config["pyprland"].get("plugins_paths", []))
+
+        init_pyprland = "pyprland" not in self.plugins
+
+        for name in ["pyprland"] + self.config["pyprland"]["plugins"]:
+            if name not in self.plugins:
+                if not await self._load_single_plugin(name, init):
+                    continue
+            if init:
+                try:
+                    await self.plugins[name].load_config(self.config)
+                    await self.plugins[name].on_reload()
+                    self.plugins[name].log.info("configured")
+                except PyprError:
+                    raise
+                except Exception as e:
+                    await notify_info(f"Error initializing plugin {name}: {e}")
+                    self.log.error("Error initializing plugin %s:", name, exc_info=True)
+                    raise PyprError() from e
+        if init_pyprland:
+            plug = self.plugins["pyprland"]
+            plug.set_commands(reload=self.load_config)  # type: ignore
+
+    async def load_config(self, init=True):
+        """loads the configuration (new plugins will be added & config updated)
+
+        if `init` is true, also initializes the plugins"""
+
+        await self.__open_config()
+        assert self.config
+        await self.__load_plugins_config(init=init)
+        if self.config["pyprland"].get("colored_handlers_log", True):
+            self.log_handler = (  # pylint: disable=attribute-defined-outside-init
+                self.colored_log_handler
+            )
+        else:
+            self.log_handler = (  # pylint: disable=attribute-defined-outside-init
+                self.plain_log_handler
+            )
+
+    def plain_log_handler(self, plugin, name, params):
+        "log a handler method without color"
+        plugin.log.debug(f"{name}{params}")
+
+    def colored_log_handler(self, plugin, name, params):
+        "log a handler method with color"
+        color = 33 if name.startswith("run_") else 30
+        plugin.log.debug(f"\033[{color};1m%s%s\033[0m", name, params)
+
+    async def _run_plugin_handler(self, plugin, full_name, params):
+        "Runs a single handler on a plugin"
+        self.log_handler(plugin, full_name, params)
+        try:
+            await getattr(plugin, full_name)(*params)
+        except AssertionError as e:
+            self.log.error(
+                "This could be a bug in Pyprland, if you think so, report on https://github.com/fdev31/pyprland/issues"
+            )
+            self.log.exception(e)
+            await notify_error(
+                f"Pypr integrity check failed on {plugin.name}::{full_name}: {e}"
+            )
+        except Exception as e:  # pylint: disable=W0718
+            self.log.warning("%s::%s(%s) failed:", plugin.name, full_name, params)
+            self.log.exception(e)
+            await notify_error(f"Pypr error {plugin.name}::{full_name}: {e}")
+
+    async def _callHandler(self, full_name, *params, notify=""):
+        "Call an event handler with params"
+        handled = False
+        for plugin in self.plugins.values():
+            if hasattr(plugin, full_name):
+                handled = True
+                task = partial(self._run_plugin_handler, plugin, full_name, params)
+                if plugin == "pyprland":
+                    await task()
+                else:
+                    await self.queues[plugin.name].put(task)
+        if notify and not handled:
+            await notify_info(f'"{notify}" not found')
+        return handled
+
+    async def read_events_loop(self):
+        "Consumes the event loop and calls corresponding handlers"
+        while not self.stopped:
+            try:
+                data = (await self.event_reader.readline()).decode()
+            except RuntimeError as e:
+                self.log.error("Aborting event loop: %s", e)
+                return
+            except UnicodeDecodeError:
+                self.log.error("Invalid unicode while reading events")
+                continue
+            if not data:
+                self.log.critical("Reader starved")
+                return
+            cmd, params = data.split(">>", 1)
+            full_name = f"event_{cmd}"
+
+            # self.log.debug("[%s] %s", cmd, params.strip())
+            await self._callHandler(full_name, params.rstrip("\n"))
+
+    async def read_command(self, reader, writer) -> None:
+        "Receives a socket command"
+        data = (await reader.readline()).decode()
+        if not data:
+            self.log.critical("Server starved")
+            data = "exit"
+        data = data.strip()
+        if data == "exit":
+            self.stopped = True
+            writer.close()
+            await writer.wait_closed()
+            self.server.close()
+            return
+        args = data.split(None, 1)
+        if len(args) == 1:
+            cmd = args[0]
+            args = []
+        else:
+            cmd = args[0]
+            args = args[1:]
+
+        full_name = f"run_{cmd}"
+
+        if PYPR_DEMO:
+            os.system(f"notify-send -t 4000 '{data}'")
+
+        if not await self._callHandler(full_name, *args, notify=cmd):
+            self.log.warning("No such command: %s", cmd)
+
+    async def serve(self):
+        "Runs the server"
+        try:
+            async with self.server:
+                await self.server.serve_forever()
+        finally:
+            await asyncio.gather(*(plugin.exit() for plugin in self.plugins.values()))
+
+    async def _plugin_runner_loop(self, name):
+        "Runs tasks for a given plugin indefinitely"
+        q = self.queues[name]
+
+        while not self.stopped:
+            try:
+                task = await q.get()
+            except RuntimeError as e:
+                self.log.error("Aborting [%s] loop: %s", name, e)
+                return
+            try:
+                await task()
+            except Exception as e:  # pylint: disable=W0718
+                self.log.error(
+                    "Unhandled error running plugin %s::%s: %s", name, task, e
+                )
+
+    async def plugins_runner(self):
+        "Runs plugins' task using the created `tasks` TaskGroup attribute"
+        async with asyncio.TaskGroup() as group:
+            self.tasks = group
+            for name in self.plugins:
+                group.create_task(self._plugin_runner_loop(name))
+
+    async def run(self):
+        "Runs the server and the event listener"
+        await asyncio.gather(
+            asyncio.create_task(self.serve()),
+            asyncio.create_task(self.read_events_loop()),
+            asyncio.create_task(self.plugins_runner()),
+        )
+
+
+async def run_daemon():
+    "Runs the server / daemon"
+    manager = Pyprland()
+    err_count = itertools.count()
+    manager.server = await asyncio.start_unix_server(manager.read_command, CONTROL)
+    max_retry = 10
+    while True:
+        attempt = next(err_count)
+        try:
+            events_reader, events_writer = await get_event_stream()
+        except Exception as e:  # pylint: disable=W0718
+            if attempt > max_retry:
+                manager.log.critical("Failed to open hyprland event stream: %s.", e)
+                await notify_fatal("Failed to open hyprland event stream")
+                raise PyprError() from e
+            manager.log.warning(
+                "Failed to get event stream: %s, retry %s/%s...", e, attempt, max_retry
+            )
+            await asyncio.sleep(1)
+        else:
+            break
+
+    manager.event_reader = events_reader
+
+    try:
+        await manager.initialize()
+    except PyprError as e:
+        if bool(str(e)):
+            await notify_fatal(f"Pypr failed to start: {e}")
+        else:
+            await notify_fatal("Pypr failed to start!")
+
+        raise SystemExit(1) from e
+    except Exception as e:
+        manager.log.critical("Failed to load config.", exc_info=True)
+        await notify_fatal(f"Pypr couldn't load config: {e}")
+        raise SystemExit(1) from e
+
+    manager.log.debug("[ initialized ]".center(80, "="))
+    try:
+        await manager.run()
+    except KeyboardInterrupt:
+        print("Interrupted")
+    except asyncio.CancelledError:
+        manager.log.critical("cancelled")
+    finally:
+        events_writer.close()
+        await events_writer.wait_closed()
+        manager.server.close()
+        await manager.server.wait_closed()
+
+
+async def run_client():
+    "Runs the client (CLI)"
+    manager = Pyprland()
+
+    if sys.argv[1] == "version":
+<<<<<<< HEAD
+        print("2.2.0")  # Automatically updated version
+=======
+        print("2.1.4-19")  # Automatically updated version
+>>>>>>> fb8d25b (mitigate code complexity - release)
+        return
+
+    if sys.argv[1] in ("--help", "-h", "help"):
+        await manager.load_config(init=False)
+
+        def format_doc(txt):
+            return txt.split("\n")[0]
+
+        print(
+            """Syntax: pypr [command]
+
+If the command is ommited, runs the daemon which will start every configured plugin.
+
+Available commands:
+"""
+        )
+        for plug in manager.plugins.values():
+            for name in dir(plug):
+                if name.startswith("run_"):
+                    fn = getattr(plug, name)
+                    if callable(fn):
+                        print(
+                            f" {name[4:]:20s} {format_doc(fn.__doc__) if fn.__doc__ else 'N/A'} [{plug.name}]"
+                        )
+
+        return
+
+    try:
+        _, writer = await asyncio.open_unix_connection(CONTROL)
+    except (ConnectionRefusedError, FileNotFoundError) as e:
+        manager.log.critical("Failed to open control socket, is pypr daemon running ?")
+        await notify_error("Pypr can't connect, is daemon running ?")
+        raise PyprError() from e
+
+    args = sys.argv[1:]
+    args[0] = args[0].replace("-", "_")
+    writer.write((" ".join(args)).encode())
+    await writer.drain()
+    writer.close()
+    await writer.wait_closed()
+
+
+def use_param(txt):
+    """Checks if parameter `txt` is in sys.argv
+    if found, removes it from sys.argv & returns the argument value
+    """
+    v = ""
+    if txt in sys.argv:
+        i = sys.argv.index(txt)
+        v = sys.argv[i + 1]
+        del sys.argv[i : i + 2]
+    return v
+
+
+def main():
+    "runs the command"
+    debug_flag = use_param("--debug")
+    if debug_flag:
+        init_logger(filename=debug_flag, force_debug=True)
+    else:
+        init_logger()
+    ipc_init()
+    log = get_logger("startup")
+
+    config_override = use_param("--config")
+    if config_override:
+        global CONFIG_FILE
+        CONFIG_FILE = config_override
+
+    invoke_daemon = len(sys.argv) <= 1
+    if invoke_daemon and os.path.exists(CONTROL):
+        asyncio.run(notify_fatal("Trying to run pypr more than once ?"))
+        log.critical(
+            """%s exists,
+is pypr already running ?
+If that's not the case, delete this file and run again.""",
+            CONTROL,
+        )
+    else:
+        try:
+            asyncio.run(run_daemon() if invoke_daemon else run_client())
+        except KeyboardInterrupt:
+            pass
+        except PyprError:
+            log.critical("Command failed.")
+        except json.decoder.JSONDecodeError as e:
+            log.critical("Invalid JSON syntax in the config file: %s", e.args[0])
+        except Exception:  # pylint: disable=W0718
+            log.critical("Unhandled exception:", exc_info=True)
+        finally:
+            if invoke_daemon:
+                os.unlink(CONTROL)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `pyprland-2.1.4/pyprland/common.py` & `pyprland-2.2.0/pyprland/common.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.4/pyprland/ipc.py` & `pyprland-2.2.0/pyprland/ipc.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.4/pyprland/plugins/expose.py` & `pyprland-2.2.0/pyprland/plugins/expose.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.4/pyprland/plugins/expose.py,cover` & `pyprland-2.2.0/pyprland/plugins/fetch_client_menu.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-> """ expose Brings every client window to screen for selection
-> """
-  
-> from .interface import Plugin
-> from ..common import state, CastBoolMixin
-  
-  
-> class Extension(CastBoolMixin, Plugin):  # pylint: disable=missing-class-docstring
->     exposed: list[dict] = []
-  
->     @property
->     def exposed_clients(self):
->         "Returns the list of clients currently using exposed mode"
-!         if self.cast_bool(self.config.get("include_special"), False):
-!             return self.exposed
-!         return [c for c in self.exposed if c["workspace"]["id"] > 0]
-  
->     async def run_expose(self):
->         """Expose every client on the active workspace.
->         If expose is active restores everything and move to the focused window"""
-!         if self.exposed:
-!             commands = []
-!             for client in self.exposed_clients:
-!                 commands.append(
-!                     f"movetoworkspacesilent {client['workspace']['id']},address:{client['address']}"
-!                 )
-!             commands.extend(
-!                 [
-!                     "togglespecialworkspace exposed",
-!                     f"focuswindow address:{state.active_window}",
-!                 ]
-!             )
-!             await self.hyprctl(commands)
-!             self.exposed = []
-!         else:
-!             self.exposed = await self.get_clients(workspace_bl=state.active_workspace)
-!             commands = []
-!             for client in self.exposed_clients:
-!                 commands.append(
-!                     f"movetoworkspacesilent special:exposed,address:{client['address']}"
-!                 )
-!             commands.append("togglespecialworkspace exposed")
-!             await self.hyprctl(commands)
+" Select a client window and move it to the active workspace"
+
+from .interface import Plugin
+from ..adapters.menus import MenuMixin
+from ..common import state
+
+
+class Extension(MenuMixin, Plugin):
+    "Shows a menu with shortcuts"
+
+    _windows_origins: dict[str, str] = {}
+
+    # Commands
+
+    async def run_unfetch_client(self):
+        "Returns a window back to its origin"
+        addr = state.active_window
+        try:
+            origin = self._windows_origins[addr]
+        except KeyError:
+            await self.notify_error("unknown window origin")
+        else:
+            await self.hyprctl(f"movetoworkspacesilent {origin},address:{addr}")
+
+    async def run_fetch_client_menu(self):
+        "Select a client window and move it to the active workspace"
+        await self.ensure_menu_configured()
+
+        clients = await self.get_clients(workspace_bl=state.active_workspace)
+
+        separator = self.config.get("separator", "|")
+
+        choice = await self.menu.run(
+            [f"{i+1} {separator} {c['title']}" for i, c in enumerate(clients)]
+        )
+
+        if choice:
+            num = int(choice.split(None, 1)[0]) - 1
+            addr = clients[num]["address"]
+            self._windows_origins[addr] = clients[num]["workspace"]["name"]
+            await self.hyprctl(
+                f"movetoworkspace {state.active_workspace},address:{addr}"
+            )
```

### Comparing `pyprland-2.1.4/pyprland/plugins/interface.py` & `pyprland-2.2.0/pyprland/plugins/interface.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.4/pyprland/plugins/layout_center.py` & `pyprland-2.2.0/pyprland/plugins/layout_center.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.4/pyprland/plugins/lost_windows.py` & `pyprland-2.2.0/pyprland/plugins/lost_windows.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.4/pyprland/plugins/magnify.py` & `pyprland-2.2.0/pyprland/plugins/magnify.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.4/pyprland/plugins/monitors.py` & `pyprland-2.2.0/pyprland/plugins/monitors.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.4/pyprland/plugins/monitors.py.orig` & `pyprland-2.2.0/pyprland/plugins/monitors.py.orig`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.4/pyprland/plugins/monitors_v0.py` & `pyprland-2.2.0/pyprland/plugins/monitors_v0.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.4/pyprland/plugins/pyprland.py` & `pyprland-2.2.0/pyprland/plugins/pyprland.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.4/pyprland/plugins/scratchpads.py` & `pyprland-2.2.0/pyprland/plugins/scratchpads.py`

 * *Files 0% similar despite different names*

```diff
@@ -449,21 +449,17 @@
             )
             width, height = convert_coords(
                 self.log, scratch.conf.get("size", "80% 80%"), monitor
             )
 
             ipc_commands = [
                 f"windowrule float,^({defined_class})$",
+                f"windowrule workspace special:scratch_{scratch.uid} silent,^({defined_class})$",
             ]
 
-            if not self.cast_bool(scratch.conf.get("lazy")):
-                ipc_commands.append(
-                    f"windowrule workspace special:scratch_{scratch.uid} silent,^({defined_class})$"
-                )
-
             if not self.cast_bool(scratch.conf.get("preserve_aspect")):
                 if animation_type:
                     margin_x = (monitor["width"] - width) // 2
                     margin_y = (monitor["height"] - height) // 2
 
                     t_pos = {
                         "fromtop": f"{margin_x} -200%",
```

### Comparing `pyprland-2.1.4/pyprland/plugins/shift_monitors.py` & `pyprland-2.2.0/pyprland/plugins/shift_monitors.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.4/pyprland/plugins/shortcuts_menu.py` & `pyprland-2.2.0/pyprland/plugins/shortcuts_menu.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.4/pyprland/plugins/system_notifier.py` & `pyprland-2.2.0/pyprland/plugins/system_notifier.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 " Add system notifications based on journal logs "
 import re
 import asyncio
 from typing import cast
 from copy import deepcopy
 from .interface import Plugin
 from ..common import apply_filter
+from ..adapters.colors import convert_color
 
 builtin_parsers = {
     "journal": [
         {
-            "pattern": r".*systemd-networkd\[\d+\]: ([a-z0-9]+): Link (UP|DOWN)$",
-            "filter": r"s/.*\[\d+\]: ([a-z0-9]+): Link (UP|DOWN)/\1 is \2/",
+            "pattern": r"([a-z0-9]+): Link UP$",
+            "filter": r"s/.*\[\d+\]: ([a-z0-9]+): Link.*/\1 is active/",
+            "color": "#00aa00",
         },
         {
-            "pattern": r".*systemd-coredump\[\d+\]: .* Process \d+ \(([^)])\) of .* dumped core.$",
-            "filter": r"s/.*Process \d+ \(([^)])\) of .* dumped core./\1 dumped core/",
+            "pattern": r"([a-z0-9]+): Link DOWN$",
+            "filter": r"s/.*\[\d+\]: ([a-z0-9]+): Link.*/\1 is inactive/",
+            "color": "#ff8800",
         },
         {
-            "pattern": r".*usb \d+-[0-9.]+: Product: (.*)",
+            "pattern": r"Process \d+ \(.*\) of .* dumped core.$",
+            "filter": r"s/.*Process \d+ \((.*)\) of .* dumped core./\1 dumped core/",
+            "color": "#aa0000",
+        },
+        {
+            "pattern": r"usb \d+-[0-9.]+: Product: ",
             "filter": r"s/.*usb \d+-[0-9.]+: Product: (.*)/USB plugged: \1/",
         },
     ]
 }
 
 
 class Extension(Plugin):
@@ -40,52 +48,69 @@
         parsers = deepcopy(builtin_parsers)
         parsers.update(self.config.get("parsers", {}))
         for name, pprops in parsers.items():
             self.tasks.append(asyncio.create_task(self.start_parser(name, pprops)))
             self.parsers[name] = asyncio.Queue()
             self.log.debug("Loaded parser %s", name)
 
-        for name, props in self.config.get("source", {}).items():
+        for props in self.config.get("sources", []):
             assert (
                 props["parser"] in self.parsers
             ), f"{props['parser']} was not found in {self.parsers}"
-            self.log.debug("Loaded source %s", name)
-            self.tasks.append(asyncio.create_task(self.start_source(name, props)))
+            self.log.debug("Loaded source %s => %s", props["command"], props["parser"])
+            self.tasks.append(asyncio.create_task(self.start_source(props)))
 
     async def exit(self):
         "empty exit function"
         self.running = False
         for task in self.tasks:
             task.cancel()
             await task
+        for source in self.sources.values():
+            if source.pid is not None:
+                source.kill()
         self.tasks[:] = []
 
-    async def start_source(self, name, props):
+    async def start_source(self, props):
         "Start a source loop"
-        q = self.parsers[props["parser"]]
+
+        parsers = (
+            [props["parser"]] if isinstance(props["parser"], str) else props["parser"]
+        )
+        queues = [self.parsers[p] for p in parsers]
         proc = await asyncio.create_subprocess_shell(
             props["command"], stdout=asyncio.subprocess.PIPE
         )
-        self.sources[name] = proc
+
+        self.sources[props["command"]] = proc
         assert proc.stdout
+        await asyncio.sleep(1)
         # Read stdout line by line and push to parser
-        while self.running:
+        while proc.returncode is None and self.running:
             line = (await proc.stdout.readline()).decode().strip()
             if line:
-                await q.put(line)
+                for q in queues:
+                    await q.put(line)
 
     async def start_parser(self, name, props: list):
         "Start a parser loop"
         q = self.parsers[name]
-        rules = {}
+        rules = []
+        default_color = self.config.get("default_color", "#5555AA")
         for prop in props:
-            rules["pattern"] = re.compile(prop["pattern"])
-            rules["filter"] = prop["filter"]
+            rules.append(
+                {
+                    "pattern": re.compile(prop["pattern"]),
+                    "filter": prop.get("filter"),
+                    "color": convert_color(prop.get("color", default_color)),
+                }
+            )
         while self.running:
             content = await q.get()
-            for prop in rules:
-                if rules["pattern"].match(content):
-                    if "filter" in rules:
-                        text = apply_filter(content, cast(str, rules["filter"]))
+            for rule in rules:
+                if rule["pattern"].search(content):
+                    if rule["filter"]:
+                        text = apply_filter(content, cast(str, rule["filter"]))
                     else:
                         text = content
-                    await self.notify(text)
+                    await self.notify(text, color=rule["color"])
+                    await asyncio.sleep(0.01)
```

### Comparing `pyprland-2.1.4/pyprland/plugins/toggle_dpms.py` & `pyprland-2.2.0/pyprland/plugins/toggle_dpms.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.4/pyprland/plugins/toggle_special.py` & `pyprland-2.2.0/pyprland/plugins/toggle_special.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.4/pyprland/plugins/workspaces_follow_focus.py` & `pyprland-2.2.0/pyprland/plugins/workspaces_follow_focus.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.4/pyproject.toml` & `pyprland-2.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyprland"
-version = "2.1.4"
+version = "2.2.0"
 description = "Hyperland plugin system - batteries included"
 authors = ["fdev31 <fdev31@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pyprland"}]
 homepage = "https://github.com/hyprland-community/pyprland/"
```

### Comparing `pyprland-2.1.4/PKG-INFO` & `pyprland-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprland
-Version: 2.1.4
+Version: 2.2.0
 Summary: Hyperland plugin system - batteries included
 Home-page: https://github.com/hyprland-community/pyprland/
 License: MIT
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -55,15 +55,15 @@
 Check the [Releases change log](https://github.com/hyprland-community/pyprland/releases) for more information
 
 
 ### 2.1
 
 - Requires Hyprland >= 0.37
 - [monitors](https://github.com/hyprland-community/pyprland/wiki//monitors)
-  - Drops the `wlr-randr` dependency
+  - Drops the `wlr-randr` dependency (used in `monitors` plugin)
   - simplified the syntax, no need for `()` around a screen name (will try matching the exact name first, then partial description)
 
 ### 2.0
 
 - New dependency: [aiofiles](https://pypi.org/project/aiofiles/)
     - fully asynchronous plugins, including file operations
 - Added [hysteresis](https://github.com/hyprland-community/pyprland/wiki/scratchpads#hysteresis-optional) support for [scratchpads](https://github.com/hyprland-community/pyprland/wiki/scratchpads) in 2.0.1, only active if `unfocus="hide"` is set.
```

