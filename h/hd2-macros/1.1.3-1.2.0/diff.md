# Comparing `tmp/hd2_macros-1.1.3.tar.gz` & `tmp/hd2_macros-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hd2_macros-1.1.3.tar", last modified: Fri Mar 29 20:31:52 2024, max compression
+gzip compressed data, was "hd2_macros-1.2.0.tar", last modified: Fri Apr  5 08:07:44 2024, max compression
```

## Comparing `hd2_macros-1.1.3.tar` & `hd2_macros-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 20:31:52.038641 hd2_macros-1.1.3/
--rw-rw-rw-   0        0        0     1099 2024-03-29 20:31:24.000000 hd2_macros-1.1.3/LICENSE
--rw-rw-rw-   0        0        0       91 2024-03-29 20:31:24.000000 hd2_macros-1.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     5605 2024-03-29 20:31:52.038641 hd2_macros-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4526 2024-03-29 20:31:24.000000 hd2_macros-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-03-29 20:31:52.038641 hd2_macros-1.1.3/hd2_macros/
--rw-rw-rw-   0        0        0       23 2024-03-29 20:31:24.000000 hd2_macros-1.1.3/hd2_macros/__init__.py
--rw-rw-rw-   0        0        0       95 2024-03-29 20:31:24.000000 hd2_macros-1.1.3/hd2_macros/__main__.py
--rw-rw-rw-   0        0        0     2425 2024-03-29 20:31:24.000000 hd2_macros-1.1.3/hd2_macros/config.py
--rw-rw-rw-   0        0        0     1283 2024-03-29 20:31:24.000000 hd2_macros-1.1.3/hd2_macros/config.toml
--rw-rw-rw-   0        0        0     5355 2024-03-29 20:31:24.000000 hd2_macros-1.1.3/hd2_macros/constants.py
--rw-rw-rw-   0        0        0     4888 2024-03-29 20:31:24.000000 hd2_macros-1.1.3/hd2_macros/macro.py
--rw-rw-rw-   0        0        0        0 2024-03-29 20:31:24.000000 hd2_macros-1.1.3/hd2_macros/py.typed
-drwxrwxrwx   0        0        0        0 2024-03-29 20:31:52.038641 hd2_macros-1.1.3/hd2_macros.egg-info/
--rw-rw-rw-   0        0        0     5605 2024-03-29 20:31:52.000000 hd2_macros-1.1.3/hd2_macros.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2024-03-29 20:31:52.000000 hd2_macros-1.1.3/hd2_macros.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 20:31:52.000000 hd2_macros-1.1.3/hd2_macros.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-03-29 20:31:52.000000 hd2_macros-1.1.3/hd2_macros.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-29 20:31:52.000000 hd2_macros-1.1.3/hd2_macros.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       48 2024-03-29 20:31:24.000000 hd2_macros-1.1.3/pyproject.toml
--rw-rw-rw-   0        0        0     1179 2024-03-29 20:31:52.038641 hd2_macros-1.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 08:07:44.201389 hd2_macros-1.2.0/
+-rw-rw-rw-   0        0        0     1099 2024-04-05 08:07:19.000000 hd2_macros-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0       91 2024-04-05 08:07:19.000000 hd2_macros-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6058 2024-04-05 08:07:44.201389 hd2_macros-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4972 2024-04-05 08:07:19.000000 hd2_macros-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 08:07:44.201389 hd2_macros-1.2.0/hd2_macros/
+-rw-rw-rw-   0        0        0       23 2024-04-05 08:07:19.000000 hd2_macros-1.2.0/hd2_macros/__init__.py
+-rw-rw-rw-   0        0        0       95 2024-04-05 08:07:19.000000 hd2_macros-1.2.0/hd2_macros/__main__.py
+-rw-rw-rw-   0        0        0     2569 2024-04-05 08:07:19.000000 hd2_macros-1.2.0/hd2_macros/config.py
+-rw-rw-rw-   0        0        0     1967 2024-04-05 08:07:19.000000 hd2_macros-1.2.0/hd2_macros/config.toml
+-rw-rw-rw-   0        0        0     5355 2024-04-05 08:07:19.000000 hd2_macros-1.2.0/hd2_macros/constants.py
+-rw-rw-rw-   0        0        0     6472 2024-04-05 08:07:19.000000 hd2_macros-1.2.0/hd2_macros/macro.py
+-rw-rw-rw-   0        0        0        0 2024-04-05 08:07:19.000000 hd2_macros-1.2.0/hd2_macros/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-05 08:07:44.201389 hd2_macros-1.2.0/hd2_macros.egg-info/
+-rw-rw-rw-   0        0        0     6058 2024-04-05 08:07:44.000000 hd2_macros-1.2.0/hd2_macros.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2024-04-05 08:07:44.000000 hd2_macros-1.2.0/hd2_macros.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 08:07:44.000000 hd2_macros-1.2.0/hd2_macros.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-04-05 08:07:44.000000 hd2_macros-1.2.0/hd2_macros.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-05 08:07:44.000000 hd2_macros-1.2.0/hd2_macros.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       48 2024-04-05 08:07:19.000000 hd2_macros-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1186 2024-04-05 08:07:44.201389 hd2_macros-1.2.0/setup.cfg
```

### Comparing `hd2_macros-1.1.3/LICENSE` & `hd2_macros-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hd2_macros-1.1.3/PKG-INFO` & `hd2_macros-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hd2_macros
-Version: 1.1.3
+Version: 1.2.0
 Summary: Helldivers 2 macros
 Home-page: https://github.com/spyoungtech/helldivers2-macros
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Project-URL: Documentation, https://github.com/spyoungtech/helldivers2-macros
 Project-URL: Source, https://github.com/spyoungtech/helldivers2-macros
 Project-URL: Tracker, https://github.com/spyoungtech/helldivers2-macros/issues
@@ -15,15 +15,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ahk
+Requires-Dist: ahk>=1.6.1
 Requires-Dist: pydantic
 Provides-Extra: binary
 Requires-Dist: ahk-binary==2023.9.0; extra == "binary"
 
 # Helldivers2 Stratagem Macro
 
 This is software for macroing stratagem inputs in Helldivers2.
@@ -69,28 +69,37 @@
 
 ```toml
 # General settings apply for all loadouts
 [general]
 # How long to wait for the helldivers window before exiting
 win_wait = 120
 
-
 # Delay in seconds between when the hotkey pressed and beginning of WASD inputs
 # Intended to allow you enough time to ensure the strategem menu is up and ready for input
 hotkey_start_delay = 1.0
-
-log_level = "DEBUG" # Change logging verbosity (valid values are "DEBUG", "INFO", "WARNING", "ERROR")
+# Change logging verbosity (valid values are "DEBUG", "INFO", "WARNING", "ERROR")
+log_level = "DEBUG"
 
 # Hide the system tray icon for the application
 no_tray_icon = false
 
 # Define a hotkey that can be used to stop the program
 # By default, bound to Windows key + Q
 exit_hotkey = "#q"
 
+# The time in between key UP/DOWN events when inputting macros.
+# Lowering this value will make inputs faster, but may cause inputs to be dropped.
+key_delay = 0.1
+
+# If you have AutoHotkey in a non-default location, you may specify it by uncommenting this line:
+# autohotkey_executable_path = "C:\Path\To\AutoHotkey64.exe"
+
+# You can explicitly specify the version of AutoHotkey. Usually, this is not necessary.
+# autohotkey_version = ""
+
 
 
 # A Loadout provides a mapping of Strategems to hotkeys. Each loadout specifies a hotkey used to switch to that loadout.
 # For hotkey/modifiers syntax, see https://www.autohotkey.com/docs/v2/Hotkeys.htm and https://www.autohotkey.com/docs/v2/KeyList.htm
 
 # The default loadout is the loadout used at program starts
 [ default_loadout ]
```

### Comparing `hd2_macros-1.1.3/README.md` & `hd2_macros-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -43,28 +43,37 @@
 
 ```toml
 # General settings apply for all loadouts
 [general]
 # How long to wait for the helldivers window before exiting
 win_wait = 120
 
-
 # Delay in seconds between when the hotkey pressed and beginning of WASD inputs
 # Intended to allow you enough time to ensure the strategem menu is up and ready for input
 hotkey_start_delay = 1.0
-
-log_level = "DEBUG" # Change logging verbosity (valid values are "DEBUG", "INFO", "WARNING", "ERROR")
+# Change logging verbosity (valid values are "DEBUG", "INFO", "WARNING", "ERROR")
+log_level = "DEBUG"
 
 # Hide the system tray icon for the application
 no_tray_icon = false
 
 # Define a hotkey that can be used to stop the program
 # By default, bound to Windows key + Q
 exit_hotkey = "#q"
 
+# The time in between key UP/DOWN events when inputting macros.
+# Lowering this value will make inputs faster, but may cause inputs to be dropped.
+key_delay = 0.1
+
+# If you have AutoHotkey in a non-default location, you may specify it by uncommenting this line:
+# autohotkey_executable_path = "C:\Path\To\AutoHotkey64.exe"
+
+# You can explicitly specify the version of AutoHotkey. Usually, this is not necessary.
+# autohotkey_version = ""
+
 
 
 # A Loadout provides a mapping of Strategems to hotkeys. Each loadout specifies a hotkey used to switch to that loadout.
 # For hotkey/modifiers syntax, see https://www.autohotkey.com/docs/v2/Hotkeys.htm and https://www.autohotkey.com/docs/v2/KeyList.htm
 
 # The default loadout is the loadout used at program starts
 [ default_loadout ]
```

### Comparing `hd2_macros-1.1.3/hd2_macros/config.py` & `hd2_macros-1.2.0/hd2_macros/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,15 +25,18 @@
 
 
 class GeneralSection(pydantic.BaseModel):
     log_level: Literal['DEBUG', 'INFO', 'WARNING', 'ERROR'] = 'INFO'
     no_tray_icon: bool = False
     win_wait: int = 120
     hotkey_start_delay: int | float = 1.0
+    key_delay: int | float = 0.1
     exit_hotkey: str = '#q'
+    autohotkey_executable_path: str | None = None
+    autohotkey_version: Literal['v1', 'v2'] | None = None
 
 
 class MacroConfig(pydantic.BaseModel):
     general: GeneralSection = pydantic.Field(..., description='General settings')
     loadouts_: dict[str, Loadout] = pydantic.Field(default_factory=dict, alias='loadouts')
     default_loadout: Loadout = pydantic.Field(..., description='The loadout that is used by default at startup')
```

### Comparing `hd2_macros-1.1.3/hd2_macros/config.toml` & `hd2_macros-1.2.0/hd2_macros/config.toml`

 * *Files 26% similar despite different names*

```diff
@@ -12,25 +12,40 @@
 # Hide the system tray icon for the application
 no_tray_icon = false
 
 # Define a hotkey that can be used to stop the program
 # By default, bound to Windows key + Q
 exit_hotkey = "#q"
 
+# The time in between key UP/DOWN events when inputting macros.
+# Lowering this value will make inputs faster, but may cause inputs to be dropped.
+key_delay = 0.1
+
+# If you have AutoHotkey in a non-default location, you may specify it by uncommenting this line:
+# autohotkey_executable_path = "C:\Path\To\AutoHotkey64.exe"
+
+# You can explicitly specify the version of AutoHotkey. Usually, this is not necessary.
+# autohotkey_version = ""
+
 
 
 # A Loadout provides a mapping of Strategems to hotkeys. Each loadout specifies a hotkey used to switch to that loadout.
-# For hotkey key syntax, see https://www.autohotkey.com/docs/v2/KeyList.htm
+# For hotkey/modifiers syntax, see https://www.autohotkey.com/docs/v2/Hotkeys.htm and https://www.autohotkey.com/docs/v2/KeyList.htm
 
 # The default loadout is the loadout used at program starts
 [ default_loadout ]
-switch_hotkey = "#1"
+switch_hotkey = "#1"  # press Win+1 to load this loadout
 [ default_loadout.hotkeys ]
 # Maps the orbital precision strike strategem to "Windows key + n"
 # All stratagem names are lowercase
 "orbital precision strike" = "#n"
 
 # Add separate sets of loadouts using `[ loadouts.<NAME> ]`
 [ loadouts.secondary ]
-switch_hotkey = "#2"
+switch_hotkey = "#2" # press Win+2 to load this loadout
 [ loadouts.secondary.hotkeys ]
 "orbital precision strike" = "#b"
+"mortar sentry" = "#s"
+"eagle cluster bomb" = "#c"
+
+# You can add as many loadouts as you want.
+# ...
```

### Comparing `hd2_macros-1.1.3/hd2_macros/constants.py` & `hd2_macros-1.2.0/hd2_macros/constants.py`

 * *Files identical despite different names*

### Comparing `hd2_macros-1.1.3/hd2_macros/macro.py` & `hd2_macros-1.2.0/hd2_macros/macro.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,71 @@
 import logging
 import time
 from typing import Any
 from typing import Callable
+from typing import Literal
+from typing import Type
 
 from ahk import AHK
 from ahk import Window
+from ahk.directives import Directive
+from ahk.directives import NoTrayIcon
+from ahk.exceptions import AhkExecutableNotFoundError
 
 from hd2_macros.config import find_config_file
+from hd2_macros.config import MacroConfig
 from hd2_macros.config import read_config
 from hd2_macros.constants import INPUT_MAPPING
 from hd2_macros.constants import STRATAGEMS
 from hd2_macros.constants import T_Stratagems
 
 logger = logging.getLogger('hd2-macros')
 logger.propagate = False
 
-ahk = AHK()
+ahk: AHK[Any] | None = None
+
+
+def _set_ahk_global(config: MacroConfig) -> None:
+    global ahk
+
+    executable_path = config.general.autohotkey_executable_path or ''
+    version: Literal['v1', 'v2'] | None
+
+    if config.general.autohotkey_version == 'v1':
+        version = 'v1'
+    elif config.general.autohotkey_version == 'v2':
+        version = 'v2'
+    elif config.general.autohotkey_version is None:
+        version = None
+    else:
+        raise Exception('Unexpected configuration value for autohotkey_version')
+    directives: list[Directive | Type[Directive]] | None
+    if config.general.no_tray_icon is True:
+        directives = [NoTrayIcon(apply_to_hotkeys_process=True)]
+    else:
+        directives = None
+    try:
+        ahk = AHK(executable_path=executable_path, version=version, directives=directives)
+    except AhkExecutableNotFoundError:
+        if not executable_path and version is None:
+            ahk = AHK(version='v2', directives=directives)
+        else:
+            raise
+    return None
 
 
 def find_helldivers_window() -> Window | None:
+    assert ahk is not None
     for window in ahk.list_windows(blocking=False).result():
-        if 'helldivers2' in window.process_path.lower():
+        try:
+            process_path = window.process_path.lower()
+        except Exception as e:
+            logging.debug(f'error in getting window process path {e}')
+            continue
+        if 'helldivers2' in process_path:
             return window
     return None
 
 
 def do_strat_input(strat: T_Stratagems, target: Window, startup_delay: float | int = 1, key_delay: float = 0.1) -> None:
     time.sleep(startup_delay)
     input_code = STRATAGEMS[strat]
@@ -61,14 +102,16 @@
 
 
 def main() -> int:
     print('Looking for config file.')
     config_file = find_config_file()
     print('Found', config_file)
     config = read_config(config_file)
+    _set_ahk_global(config)
+    assert ahk is not None
     _start = time.time()
     logger.setLevel(level=getattr(logging, config.general.log_level))
     handler = logging.StreamHandler()
     handler.setFormatter(logging.Formatter(fmt='%(asctime)s %(levelname)-8s %(message)s'))
     logger.addHandler(handler)
     logger.info('Looking for Helldivers2 window')
     logger.debug(repr(config))
@@ -87,15 +130,15 @@
 
     def create_loadout_switcher(this_name: str, hotkeys: dict[T_Stratagems, str]) -> Callable[[], None]:
         def switch_loadout() -> None:
             logger.info('Switching to loadout %s', this_name)
             ahk.stop_hotkeys()
             ahk.clear_hotkeys()
             for strat, hotkey in hotkeys.items():
-                callback = create_macro_function(strat, hd, config.general.hotkey_start_delay)
+                callback = create_macro_function(strat, hd, config.general.hotkey_start_delay, config.general.key_delay)
                 ahk.add_hotkey(hotkey, callback, ex_handler=error_handler)
             for name, loadout_config in config.loadouts.items():
                 switch_callback = create_loadout_switcher(name, loadout_config.hotkeys)
                 ahk.add_hotkey(loadout_config.switch_hotkey, switch_callback, ex_handler=error_handler)
             ahk.add_hotkey(config.general.exit_hotkey, _exit, ex_handler=error_handler)
             ahk.start_hotkeys()
             return None
@@ -105,15 +148,15 @@
     for loadout_name, loadout in config.loadouts.items():
         logger.debug(f'Initializing loader {loadout_name}')
         callback = create_loadout_switcher(loadout_name, loadout.hotkeys)
         ahk.add_hotkey(loadout.switch_hotkey, callback, ex_handler=error_handler)
 
     for strat, hotkey in config.default_loadout.hotkeys.items():
         logger.debug('Initializing default loadout')
-        callback = create_macro_function(strat, hd, config.general.hotkey_start_delay)
+        callback = create_macro_function(strat, hd, config.general.hotkey_start_delay, config.general.key_delay)
         ahk.add_hotkey(hotkey, callback, ex_handler=error_handler)
 
     ahk.add_hotkey(config.general.exit_hotkey, _exit, ex_handler=error_handler)
 
     ahk.start_hotkeys()
     logger.info('hotkey listener started')
     try:
```

### Comparing `hd2_macros-1.1.3/hd2_macros.egg-info/PKG-INFO` & `hd2_macros-1.2.0/hd2_macros.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hd2_macros
-Version: 1.1.3
+Version: 1.2.0
 Summary: Helldivers 2 macros
 Home-page: https://github.com/spyoungtech/helldivers2-macros
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Project-URL: Documentation, https://github.com/spyoungtech/helldivers2-macros
 Project-URL: Source, https://github.com/spyoungtech/helldivers2-macros
 Project-URL: Tracker, https://github.com/spyoungtech/helldivers2-macros/issues
@@ -15,15 +15,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ahk
+Requires-Dist: ahk>=1.6.1
 Requires-Dist: pydantic
 Provides-Extra: binary
 Requires-Dist: ahk-binary==2023.9.0; extra == "binary"
 
 # Helldivers2 Stratagem Macro
 
 This is software for macroing stratagem inputs in Helldivers2.
@@ -69,28 +69,37 @@
 
 ```toml
 # General settings apply for all loadouts
 [general]
 # How long to wait for the helldivers window before exiting
 win_wait = 120
 
-
 # Delay in seconds between when the hotkey pressed and beginning of WASD inputs
 # Intended to allow you enough time to ensure the strategem menu is up and ready for input
 hotkey_start_delay = 1.0
-
-log_level = "DEBUG" # Change logging verbosity (valid values are "DEBUG", "INFO", "WARNING", "ERROR")
+# Change logging verbosity (valid values are "DEBUG", "INFO", "WARNING", "ERROR")
+log_level = "DEBUG"
 
 # Hide the system tray icon for the application
 no_tray_icon = false
 
 # Define a hotkey that can be used to stop the program
 # By default, bound to Windows key + Q
 exit_hotkey = "#q"
 
+# The time in between key UP/DOWN events when inputting macros.
+# Lowering this value will make inputs faster, but may cause inputs to be dropped.
+key_delay = 0.1
+
+# If you have AutoHotkey in a non-default location, you may specify it by uncommenting this line:
+# autohotkey_executable_path = "C:\Path\To\AutoHotkey64.exe"
+
+# You can explicitly specify the version of AutoHotkey. Usually, this is not necessary.
+# autohotkey_version = ""
+
 
 
 # A Loadout provides a mapping of Strategems to hotkeys. Each loadout specifies a hotkey used to switch to that loadout.
 # For hotkey/modifiers syntax, see https://www.autohotkey.com/docs/v2/Hotkeys.htm and https://www.autohotkey.com/docs/v2/KeyList.htm
 
 # The default loadout is the loadout used at program starts
 [ default_loadout ]
```

### Comparing `hd2_macros-1.1.3/setup.cfg` & `hd2_macros-1.2.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2068 6432 5f6d 6163 726f 730d 0a76   = hd2_macros..v
-00000020: 6572 7369 6f6e 203d 2031 2e31 2e33 0d0a  ersion = 1.1.3..
+00000020: 6572 7369 6f6e 203d 2031 2e32 2e30 0d0a  ersion = 1.2.0..
 00000030: 6175 7468 6f72 5f65 6d61 696c 203d 2073  author_email = s
 00000040: 7065 6e63 6572 2e79 6f75 6e67 4073 7079  pencer.young@spy
 00000050: 6f75 6e67 2e63 6f6d 0d0a 6175 7468 6f72  oung.com..author
 00000060: 203d 2053 7065 6e63 6572 2059 6f75 6e67   = Spencer Young
 00000070: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000080: 4865 6c6c 6469 7665 7273 2032 206d 6163  Helldivers 2 mac
 00000090: 726f 730d 0a6c 6f6e 675f 6465 7363 7269  ros..long_descri
@@ -56,19 +56,20 @@
 00000370: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
 00000380: 7974 686f 6e20 3a3a 2033 2e31 320d 0a0d  ython :: 3.12...
 00000390: 0a5b 6f70 7469 6f6e 735d 0d0a 696e 636c  .[options]..incl
 000003a0: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
 000003b0: 203d 2054 7275 650d 0a70 6163 6b61 6765   = True..package
 000003c0: 7320 3d20 0d0a 0968 6432 5f6d 6163 726f  s = ...hd2_macro
 000003d0: 730d 0a69 6e73 7461 6c6c 5f72 6571 7569  s..install_requi
-000003e0: 7265 7320 3d20 0d0a 0961 686b 0d0a 0970  res = ...ahk...p
-000003f0: 7964 616e 7469 630d 0a0d 0a5b 6f70 7469  ydantic....[opti
-00000400: 6f6e 732e 6578 7472 6173 5f72 6571 7569  ons.extras_requi
-00000410: 7265 5d0d 0a62 696e 6172 7920 3d20 6168  re]..binary = ah
-00000420: 6b2d 6269 6e61 7279 3d3d 3230 3233 2e39  k-binary==2023.9
-00000430: 2e30 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  .0....[options.p
-00000440: 6163 6b61 6765 5f64 6174 615d 0d0a 6168  ackage_data]..ah
-00000450: 6b20 3d20 0d0a 0970 792e 7479 7065 640d  k = ...py.typed.
-00000460: 0a09 636f 6e66 6967 2e74 6f6d 6c0d 0a0d  ..config.toml...
-00000470: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-00000480: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-00000490: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+000003e0: 7265 7320 3d20 0d0a 0961 686b 3e3d 312e  res = ...ahk>=1.
+000003f0: 362e 310d 0a09 7079 6461 6e74 6963 0d0a  6.1...pydantic..
+00000400: 0d0a 5b6f 7074 696f 6e73 2e65 7874 7261  ..[options.extra
+00000410: 735f 7265 7175 6972 655d 0d0a 6269 6e61  s_require]..bina
+00000420: 7279 203d 2061 686b 2d62 696e 6172 793d  ry = ahk-binary=
+00000430: 3d32 3032 332e 392e 300d 0a0d 0a5b 6f70  =2023.9.0....[op
+00000440: 7469 6f6e 732e 7061 636b 6167 655f 6461  tions.package_da
+00000450: 7461 5d0d 0a61 686b 203d 200d 0a09 7079  ta]..ahk = ...py
+00000460: 2e74 7970 6564 0d0a 0963 6f6e 6669 672e  .typed...config.
+00000470: 746f 6d6c 0d0a 0d0a 5b65 6767 5f69 6e66  toml....[egg_inf
+00000480: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
+00000490: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
+000004a0: 0d0a                                     ..
```

