# Comparing `tmp/linien-gui-1.0.2rc1.tar.gz` & `tmp/linien-gui-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien-gui-1.0.2rc1.tar", last modified: Fri Apr  5 08:31:45 2024, max compression
+gzip compressed data, was "linien-gui-2.0.0rc1.tar", last modified: Fri Apr  5 13:10:37 2024, max compression
```

## Comparing `linien-gui-1.0.2rc1.tar` & `linien-gui-2.0.0rc1.tar`

### file list

```diff
@@ -1,52 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:45.819801 linien-gui-1.0.2rc1/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-05 08:31:45.819801 linien-gui-1.0.2rc1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:45.811801 linien-gui-1.0.2rc1/linien_gui/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)   410598 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:45.819801 linien-gui-1.0.2rc1/linien_gui/ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/device_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/device_manager.ui
--rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/general_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)    26298 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/general_panel.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/lock_status_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/locking_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)    39236 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/locking_panel.ui
--rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/logging_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/logging_panel.ui
--rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/main_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    42563 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/main_window.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/modulation_sweep_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/modulation_sweep_panel.ui
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/new_device_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/new_device_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/optimization_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)    16567 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/optimization_panel.ui
--rw-r--r--   0 runner    (1001) docker     (127)    30707 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/plot_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/psd_plot_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/psd_table_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/psd_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/psd_window.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/right_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/spectroscopy_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11752 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/spectroscopy_panel.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/spin_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/sweep_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/version_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/view_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     9840 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/view_panel.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:45.819801 linien-gui-1.0.2rc1/linien_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-05 08:31:45.000000 linien-gui-1.0.2rc1/linien_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-05 08:31:45.000000 linien-gui-1.0.2rc1/linien_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 08:31:45.000000 linien-gui-1.0.2rc1/linien_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 08:31:45.000000 linien-gui-1.0.2rc1/linien_gui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-05 08:31:45.000000 linien-gui-1.0.2rc1/linien_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 08:31:45.000000 linien-gui-1.0.2rc1/linien_gui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 08:31:45.819801 linien-gui-1.0.2rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:10:37.600631 linien-gui-2.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-05 13:10:37.600631 linien-gui-2.0.0rc1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:10:37.592631 linien-gui-2.0.0rc1/linien_gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-05 13:10:16.000000 linien-gui-2.0.0rc1/linien_gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-04-05 13:10:16.000000 linien-gui-2.0.0rc1/linien_gui/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-05 13:10:16.000000 linien-gui-2.0.0rc1/linien_gui/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-04-05 13:10:16.000000 linien-gui-2.0.0rc1/linien_gui/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-04-05 13:10:16.000000 linien-gui-2.0.0rc1/linien_gui/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:10:37.600631 linien-gui-2.0.0rc1/linien_gui/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:10:16.000000 linien-gui-2.0.0rc1/linien_gui/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10338 2024-04-05 13:10:16.000000 linien-gui-2.0.0rc1/linien_gui/ui/device_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9626 2024-04-05 13:10:16.000000 linien-gui-2.0.0rc1/linien_gui/ui/general_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-04-05 13:10:16.000000 linien-gui-2.0.0rc1/linien_gui/ui/lock_status_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-04-05 13:10:16.000000 linien-gui-2.0.0rc1/linien_gui/ui/locking_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-04-05 13:10:16.000000 linien-gui-2.0.0rc1/linien_gui/ui/logging_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10705 2024-04-05 13:10:16.000000 linien-gui-2.0.0rc1/linien_gui/ui/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-04-05 13:10:16.000000 linien-gui-2.0.0rc1/linien_gui/ui/modulation_sweep_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-05 13:10:16.000000 linien-gui-2.0.0rc1/linien_gui/ui/new_device_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8784 2024-04-05 13:10:16.000000 linien-gui-2.0.0rc1/linien_gui/ui/optimization_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30707 2024-04-05 13:10:16.000000 linien-gui-2.0.0rc1/linien_gui/ui/plot_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7807 2024-04-05 13:10:16.000000 linien-gui-2.0.0rc1/linien_gui/ui/psd_plot_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-05 13:10:16.000000 linien-gui-2.0.0rc1/linien_gui/ui/psd_table_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-04-05 13:10:16.000000 linien-gui-2.0.0rc1/linien_gui/ui/psd_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-05 13:10:16.000000 linien-gui-2.0.0rc1/linien_gui/ui/right_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-04-05 13:10:16.000000 linien-gui-2.0.0rc1/linien_gui/ui/spectroscopy_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-05 13:10:16.000000 linien-gui-2.0.0rc1/linien_gui/ui/spin_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-04-05 13:10:16.000000 linien-gui-2.0.0rc1/linien_gui/ui/sweep_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-05 13:10:16.000000 linien-gui-2.0.0rc1/linien_gui/ui/version_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-04-05 13:10:16.000000 linien-gui-2.0.0rc1/linien_gui/ui/view_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-04-05 13:10:16.000000 linien-gui-2.0.0rc1/linien_gui/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:10:37.600631 linien-gui-2.0.0rc1/linien_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-05 13:10:37.000000 linien-gui-2.0.0rc1/linien_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-05 13:10:37.000000 linien-gui-2.0.0rc1/linien_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:10:37.000000 linien-gui-2.0.0rc1/linien_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-05 13:10:37.000000 linien-gui-2.0.0rc1/linien_gui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-05 13:10:37.000000 linien-gui-2.0.0rc1/linien_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 13:10:37.000000 linien-gui-2.0.0rc1/linien_gui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-05 13:10:16.000000 linien-gui-2.0.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:10:37.600631 linien-gui-2.0.0rc1/setup.cfg
```

### Comparing `linien-gui-1.0.2rc1/linien_gui/__init__.py` & `linien-gui-2.0.0rc1/linien_gui/__init__.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2rc1/linien_gui/app.py` & `linien-gui-2.0.0rc1/linien_gui/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,23 +15,22 @@
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 import logging
 import signal
 import sys
 
-import click
+import fire
 from linien_client.connection import LinienClient
 from linien_gui import __version__
-from linien_gui.config import load_settings
+from linien_gui.config import UI_PATH, load_settings
 from linien_gui.ui.device_manager import DeviceManager
 from linien_gui.ui.main_window import MainWindow
 from linien_gui.ui.psd_window import PSDWindow
 from linien_gui.ui.version_checker import VersionCheckerThread
-from linien_gui.widgets import UI_PATH
 from PyQt5 import QtWidgets
 from PyQt5.QtCore import pyqtSignal
 from pyqtgraph.Qt import QtCore
 
 sys.path += [str(UI_PATH)]
 
 logger = logging.getLogger(__name__)
@@ -51,15 +50,15 @@
         self.psd_window = PSDWindow()
         self.device_manager.show()
 
         self.aboutToQuit.connect(self.quit)
 
     def client_connected(self, client: LinienClient):
         self.device_manager.hide()
-        self.main_window.show(client.host, client.name)
+        self.main_window.show(client.device.host, client.device.name)
 
         self.client = client
         self.control = client.control
         self.parameters = client.parameters
 
         self.connection_established.emit()
 
@@ -105,22 +104,28 @@
             logger.info("New version available")
             self.main_window.show_new_version_available()
         else:
             logger.info("No new version available")
             QtCore.QTimer.singleShot(1000 * 60 * 60, self.check_for_new_version)
 
 
-# ignore type, otherwise "Argument 1 has incompatible type "Callable[[int, bool, str |
-# None, bool], Any]"; expected <nothing>" is raised for click 8.1.4.
-@click.command("linien")  # type: ignore[arg-type]
-@click.version_option(__version__)
-def run_application():
-    app = LinienApp(sys.argv)
-    logger.info("Starting Linien GUI")
-
-    # catch ctrl-c and shutdown
-    signal.signal(signal.SIGINT, signal.SIG_DFL)
-    sys.exit(app.exec_())
+class LinienGUI:
+    def version(self) -> str:
+        """Return the version of the Linien GUI."""
+        return __version__
+
+    def run(self):
+        """Start the Linien GUI."""
+        app = LinienApp(sys.argv)
+        logger.info("Starting Linien GUI")
+
+        # catch ctrl-c and shutdown
+        signal.signal(signal.SIGINT, signal.SIG_DFL)
+        sys.exit(app.exec_())
+
+
+def main() -> None:
+    fire.Fire(LinienGUI)
 
 
 if __name__ == "__main__":
-    run_application()
+    main()
```

### Comparing `linien-gui-1.0.2rc1/linien_gui/config.py` & `linien-gui-2.0.0rc1/linien_gui/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # Copyright 2018-2022 Benjamin Wiegand <benjamin.wiegand@physik.hu-berlin.de>
+# Copyright 2023 Bastian Leykauf <leykauf@physik.hu-berlin.de>
+
 #
 # This file is part of Linien and based on redpid.
 #
 # Linien is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -13,24 +15,25 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 import json
 import logging
-import pickle
 from enum import Enum
-from typing import Callable, Iterator, List, Tuple
+from pathlib import Path
+from typing import Callable, Iterator, Tuple
 
-import rpyc
 from linien_common.config import USER_DATA_PATH
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
+UI_PATH = Path(__file__).parents[0].resolve() / "ui"
+
 # don't plot more often than once per `DEFAULT_PLOT_RATE_LIMIT` seconds
 DEFAULT_PLOT_RATE_LIMIT = 0.1
 
 DEFAULT_COLORS = [
     (200, 0, 0, 200),
     (0, 200, 0, 200),
     (0, 0, 200, 200),
@@ -76,18 +79,18 @@
         self._value = value
 
         # We copy it because a listener could remove a listener --> this would cause an
         # error in this loop.
         for callback in self._callbacks.copy():
             callback(value)
 
-    def add_callback(self, function: Callable, call_with_first_value: bool = True):
+    def add_callback(self, function: Callable, call_immediatly: bool = True):
         self._callbacks.add(function)
 
-        if call_with_first_value:
+        if call_immediatly:
             if self._value is not None:
                 function(self._value)
 
     def remove_callback(self, function):
         if function in self._callbacks:
             self._callbacks.remove(function)
 
@@ -101,17 +104,15 @@
         self.plot_color_1 = Setting(start=DEFAULT_COLORS[1])
         self.plot_color_2 = Setting(start=DEFAULT_COLORS[2])
         self.plot_color_3 = Setting(start=DEFAULT_COLORS[3])
         self.plot_color_4 = Setting(start=DEFAULT_COLORS[4])
 
         # save changed settings to disk
         for _, setting in self:
-            setting.add_callback(
-                lambda _: save_settings(self), call_with_first_value=False
-            )
+            setting.add_callback(lambda _: save_settings(self), call_immediatly=False)
 
     def __iter__(self) -> Iterator[Tuple[str, Setting]]:
         for name, setting in self.__dict__.items():
             if isinstance(setting, Setting):
                 yield name, setting
 
 
@@ -129,52 +130,7 @@
             for name, value in data.items():
                 if name in settings.__dict__:
                     getattr(settings, name).value = value
     except FileNotFoundError:
         save_settings(settings)
 
     return settings
-
-
-def save_device_data(devices) -> None:
-    with open(USER_DATA_PATH / "devices", "wb") as f:
-        pickle.dump(devices, f)
-
-
-def load_device_data() -> List[dict]:
-    try:
-        with open(USER_DATA_PATH / "devices", "rb") as f:
-            devices = pickle.load(f)
-    except (FileNotFoundError, pickle.UnpicklingError, EOFError):
-        devices = []
-
-    return devices
-
-
-def save_parameter(
-    device_key: dict, param_name: str, value: object, delete: bool = False
-):
-    devices = load_device_data()
-    device = [d for d in devices if d["key"] == device_key][0]
-    device.setdefault("params", {})
-
-    if not delete:
-        # FIXME: This is the only part where rpyc is used in linien-gui. Remove it if
-        # possible. rpyc obtain is for ensuring that we don't try to save a netref here
-        try:
-            device["params"][param_name] = rpyc.classic.obtain(value)
-        except Exception:
-            logger.exception("unable to obtain and save parameter %s" % param_name)
-    else:
-        try:
-            del device["params"][param_name]
-        except KeyError:
-            pass
-
-    save_device_data(devices)
-
-
-def get_saved_parameters(device_key: dict):
-    devices = load_device_data()
-    device = [d for d in devices if d["key"] == device_key][0]
-    device.setdefault("params", {})
-    return device["params"]
```

### Comparing `linien-gui-1.0.2rc1/linien_gui/dialogs.py` & `linien-gui-2.0.0rc1/linien_gui/dialogs.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from typing import Callable
 
+from linien_client.device import Device
 from PyQt5.QtCore import pyqtSignal
 from PyQt5.QtWidgets import (
     QDialog,
     QListWidget,
     QMessageBox,
     QPushButton,
     QVBoxLayout,
@@ -52,15 +53,15 @@
     def on_thread_finished(self):
         self.addItem("\nFinished.")
         self.scrollToBottom()
         self.command_finished.emit()
 
 
 def show_installation_progress_widget(
-    parent: QWidget, device: dict, callback: Callable
+    parent: QWidget, device: Device, callback: Callable
 ):
     window = QDialog(parent)
     window.setWindowTitle("Deploying Linien Server")
     window.resize(800, 600)
     window_layout = QVBoxLayout(window)
     widget = SSHCommandOutputWidget(parent)
     button = QPushButton("Continue")
```

### Comparing `linien-gui-1.0.2rc1/linien_gui/threads.py` & `linien-gui-2.0.0rc1/linien_gui/threads.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,28 +14,29 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 import logging
 import traceback
+from typing import Dict, Tuple
 
 from linien_client.connection import LinienClient
 from linien_client.deploy import install_remote_server
+from linien_client.device import Device, update_device
 from linien_client.exceptions import (
     GeneralConnectionError,
     InvalidServerVersionException,
     RPYCAuthenticationException,
     ServerNotInstalledException,
 )
-from linien_common.config import DEFAULT_SERVER_PORT
+from linien_client.remote_parameters import RemoteParameter
+from linien_common.communication import RestorableParameterValues
 from PyQt5.QtCore import QObject, QThread, pyqtSignal
 
-from .config import get_saved_parameters, save_parameter
-
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 
 class RemoteOutStream(QObject):
     new_item = pyqtSignal(str)
 
@@ -46,71 +47,60 @@
         pass
 
     def flush(self):
         pass
 
 
 class RemoteServerInstallationThread(QThread):
-    def __init__(self, device: dict):
+    def __init__(self, device: Device) -> None:
         """A thread that installs the linien server on a remote machine."""
         super(RemoteServerInstallationThread, self).__init__()
         self.device = device
 
     out_stream = RemoteOutStream()
 
-    def run(self):
-        install_remote_server(
-            host=self.device["host"],
-            user=self.device["username"],
-            password=self.device["password"],
-            out_stream=self.out_stream,
-        )
+    def run(self) -> None:
+        install_remote_server(self.device, out_stream=self.out_stream)
 
 
 class ConnectionThread(QThread):
-    def __init__(self, device: dict):
+    def __init__(self, device: Device) -> None:
         super(ConnectionThread, self).__init__()
         self.device = device
 
     client_connected = pyqtSignal(object)
     server_not_installed_exception_raised = pyqtSignal()
     invalid_server_version_exception_raised = pyqtSignal(str, str)
     authentication_exception_raised = pyqtSignal()
     general_connection_exception_raised = pyqtSignal()
     other_exception_raised = pyqtSignal(str)
     connection_lost = pyqtSignal()
-    ask_for_parameter_restore = pyqtSignal()
+    parameter_difference = pyqtSignal(dict)
 
-    def run(self):
+    def run(self) -> None:
         try:
-            self.client = LinienClient(
-                host=self.device["host"],
-                user=self.device["username"],
-                password=self.device["password"],
-                port=self.device.get("port", DEFAULT_SERVER_PORT),
-                name=self.device.get("name", ""),
-            )
+            self.client = LinienClient(self.device)
             self.client.connect(
                 autostart_server=True,
                 use_parameter_cache=True,
                 call_on_error=self.on_connection_lost,
             )
             self.client_connected.emit(self.client)
 
             # Check for locally cached settings for this server
-            parameters_differ = self.restore_parameters(dry_run=True)
-            if parameters_differ:
-                self.ask_for_parameter_restore.emit()
+            param_diff = self.compare_local_and_remote_parameters()
+            if param_diff:
+                self.parameter_difference.emit(param_diff)
             else:
                 # if parameters don't differ, we can start monitoring remote parameter
                 # changes and write them to disk. We don't do this if parameters differ
                 # because we don't want to override our local settings with the remote
                 # one --> we wait until user has answered whether local parameters or
                 # remote ones should be used.
-                self.write_restorable_parameters_to_disk_on_change()
+                self.add_callbacks_to_write_parameters_to_disk_on_change()
 
         except ServerNotInstalledException:
             self.server_not_installed_exception_raised.emit()
 
         except InvalidServerVersionException as e:
             self.invalid_server_version_exception_raised.emit(
                 e.remote_version, e.client_version
@@ -122,66 +112,64 @@
         except GeneralConnectionError:
             self.general_connection_exception_raised.emit()
 
         except Exception:
             traceback.print_exc()
             self.other_exception_raised.emit(traceback.format_exc())
 
-    def on_connection_lost(self):
+    def on_connection_lost(self) -> None:
         self.connection_lost.emit()
 
-    def answer_whether_to_restore_parameters(self, should_restore):
-        if should_restore:
-            self.restore_parameters(dry_run=False)
-
-        self.write_restorable_parameters_to_disk_on_change()
-
-    def restore_parameters(self, dry_run=False):
-        """
-        Reads settings for a server that were cached locally. Sends them to the server.
-        If `dry_run` is...
-
-            * `True`, this function returns a boolean indicating whether the
-              local parameters differ from the ones on the server
-            * `False`, the local parameters are uploaded to the server
-        """
-        params = get_saved_parameters(self.device["key"])
-        logger.info("Restoring parameters")
-
-        differences = False
-
-        for k, v in params.items():
-            if hasattr(self.client.parameters, k):
-                param = getattr(self.client.parameters, k)
-                if param.value != v:
-                    if dry_run:
-                        logger.info(f"parameter {k} differs")
-                        differences = True
-                        break
-                    else:
-                        param.value = v
-            else:
-                # This may happen if the settings were written with a different version
-                # of linien.
-                logger.warning(
-                    f"Unable to restore parameter {k}. Delete the cached value."
+    def compare_local_and_remote_parameters(
+        self,
+    ) -> Dict[str, Tuple[RestorableParameterValues, RestorableParameterValues]]:
+        """Get differences between local and remote parameters."""
+        differences = {}
+        for local_param_name, local_param_value in self.device.parameters.items():
+            if hasattr(self.client.parameters, local_param_name):
+                remote_param: RemoteParameter = getattr(
+                    self.client.parameters, local_param_name
                 )
-                save_parameter(self.device["key"], k, None, delete=True)
-
-        if not dry_run:
-            self.client.control.write_registers()
-
+                if remote_param.value != local_param_value:
+                    logger.info(
+                        f"Parameter {local_param_name} differs: "
+                        f"local={local_param_value}, remote={remote_param.value}"
+                    )
+                    differences[local_param_name] = (
+                        local_param_value,
+                        remote_param.value,
+                    )
         return differences
 
-    def write_restorable_parameters_to_disk_on_change(self):
+    def restore_parameters(
+        self,
+        differences: Dict[
+            str, Tuple[RestorableParameterValues, RestorableParameterValues]
+        ],
+    ) -> None:
+        """Restore the remote parameters with the local ones."""
+        logger.info("Restoring parameters...")
+        for param_name, (local_value, remote_value) in differences.items():
+            remote_param: RemoteParameter = getattr(self.client.parameters, param_name)
+            remote_param.value = local_value
+        self.client.control.exposed_write_registers()
+        logger.info("Parameters restored.")
+
+    def add_callbacks_to_write_parameters_to_disk_on_change(self) -> None:
         """
         Listens for changes of some parameters and permanently saves their values on the
         client's disk. This data can be used to restore the status later, if the client
         tries to connect to the server but it doesn't run anymore.
         """
-        for parameter_name, parameter in self.client.parameters:
-            if parameter.restorable:
+        for param_name, param in self.client.parameters:
+            if param.restorable:
 
-                def on_change(value, parameter_name: str = parameter_name) -> None:
-                    save_parameter(self.device["key"], parameter_name, value)
+                def on_change(value, parameter_name: str = param_name) -> None:
+                    logger.debug(f"Parameter {parameter_name} changed to {value}")
+                    if (
+                        parameter_name not in self.device.parameters
+                        or self.device.parameters[parameter_name] != value
+                    ):
+                        self.device.parameters[parameter_name] = value
+                        update_device(self.device)
 
-                parameter.add_callback(on_change)
+                param.add_callback(on_change)
```

### Comparing `linien-gui-1.0.2rc1/linien_gui/ui/device_manager.py` & `linien-gui-2.0.0rc1/linien_gui/ui/device_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,74 +12,72 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Dict, Tuple
+
 import linien_gui
-from linien_gui.config import load_device_data, save_device_data
+from linien_client.device import Device, delete_device, load_device_list, move_device
+from linien_common.communication import RestorableParameterValues
+from linien_gui.config import UI_PATH
 from linien_gui.dialogs import (
     LoadingDialog,
     ask_for_parameter_restore_dialog,
     error_dialog,
     question_dialog,
     show_installation_progress_widget,
 )
 from linien_gui.threads import ConnectionThread
 from linien_gui.ui.new_device_dialog import NewDeviceDialog
 from linien_gui.utils import get_linien_app_instance, set_window_icon
-from linien_gui.widgets import UI_PATH
 from PyQt5 import QtCore, QtWidgets, uic
-from PyQt5.QtWidgets import QPushButton
+from PyQt5.QtWidgets import QListWidget, QPushButton
 
 
 class DeviceManager(QtWidgets.QMainWindow):
     addButton: QPushButton
     connectButton: QPushButton
+    deviceList: QListWidget
     editButton: QPushButton
     moveDownButton: QPushButton
     moveUpButton: QPushButton
     removeButton: QPushButton
 
     def __init__(self, *args, **kwargs):
         super(DeviceManager, self).__init__(*args, **kwargs)
         uic.loadUi(UI_PATH / "device_manager.ui", self)
         self.setWindowTitle(f"Linien spectroscopy lock v{linien_gui.__version__}")
         set_window_icon(self)
         self.app = get_linien_app_instance()
-        QtCore.QTimer.singleShot(100, lambda: self.load_device_data(autoload=True))
+        QtCore.QTimer.singleShot(100, lambda: self.populate_device_list())
 
     def keyPressEvent(self, event):
         key = event.key()
 
         if key in (QtCore.Qt.Key_Enter, QtCore.Qt.Key_Return):
             self.connect()
 
-    def load_device_data(self, autoload=False):
-        devices = load_device_data()
-        lst = self.deviceList
-        lst.clear()
-
-        for device in devices:
-            lst.addItem("{} ({})".format(device["name"], device["host"]))
-
-        if autoload and len(devices) == 1:
-            self.connect_to_device(devices[0])
+    def populate_device_list(self):
+        self.devices = load_device_list()
 
-    def connect(self):
-        devices = load_device_data()
+        self.deviceList.clear()
+        for device in self.devices:
+            self.deviceList.addItem(f"{device.name} ({device.host})")
 
-        if not devices:
+    def connect(self) -> None:
+        if not self.devices:
             return
         else:
-            self.connect_to_device(devices[self.get_list_index()])
+            self.connect_to_device(self.devices[self.get_list_index()])
 
-    def connect_to_device(self, device: dict):
-        loading_dialog = LoadingDialog(self, device["host"])
+    def connect_to_device(self, device: Device):
+        loading_dialog = LoadingDialog(self, device.host)
         loading_dialog.show()
 
         aborted = {}
 
         self.connection_thread = ConnectionThread(device)
 
         def was_aborted(*args):
@@ -150,27 +148,33 @@
             loading_dialog.hide()
             if not aborted:
                 display_error = (
                     f"Exception occurred when connecting to the device:\n\n {exception}"
                 )
                 error_dialog(self, display_error)
 
-        def ask_for_parameter_restore():
+        def ask_for_parameter_restore(
+            parameter_difference: Dict[
+                str, Tuple[RestorableParameterValues, RestorableParameterValues]
+            ]
+        ) -> None:
             question = (
                 "Linien on RedPitaya is running with different parameters than the "
                 "ones saved locally on this machine. Do you want to upload the local "
                 "parameters or keep the remote ones? Note that remote parameters are "
                 "only saved if Linien server was shut down properly, not when "
                 "unplugging the power plug. In this case, you should update your local "
                 "parameters."
             )
             should_restore = ask_for_parameter_restore_dialog(
                 self, question, "Restore parameters?"
             )
-            self.connection_thread.answer_whether_to_restore_parameters(should_restore)
+            if should_restore:
+                self.connection_thread.restore_parameters(parameter_difference)
+            self.connection_thread.add_callbacks_to_write_parameters_to_disk_on_change()
 
         def handle_connection_lost():
             error_dialog(self, "Lost connection to the server!")
             self.app.quit()
 
         # Connect slots to signals -----------------------------------------------------
         self.connection_thread.client_connected.connect(on_client_connected)
@@ -184,100 +188,76 @@
         self.connection_thread.authentication_exception_raised.connect(
             handle_authentication_exception
         )
         self.connection_thread.general_connection_exception_raised.connect(
             handle_general_connection_error
         )
         self.connection_thread.other_exception_raised.connect(handle_other_exception)
-        self.connection_thread.ask_for_parameter_restore.connect(
-            ask_for_parameter_restore
-        )
+        self.connection_thread.parameter_difference.connect(ask_for_parameter_restore)
         self.connection_thread.connection_lost.connect(handle_connection_lost)
 
         # Start the worker -------------------------------------------------------------
         self.connection_thread.start()
 
-    def new_device(self):
+    def get_list_index(self):
+        """Get the currently selected device index from the device list."""
+        return self.deviceList.currentIndex().row()
+
+    def reload_device_data(self) -> None:
+        # not very elegant...
+        QtCore.QTimer.singleShot(100, self.populate_device_list)
+
+    def new_device(self) -> None:
+        """Open the dialog to create a new device."""
         self.dialog = NewDeviceDialog()
         self.dialog.setModal(True)
         self.dialog.show()
+        self.dialog.accepted.connect(self.reload_device_data)
 
-        def reload_device_data():
-            # not very elegant...
-            QtCore.QTimer.singleShot(100, self.load_device_data)
-
-        self.dialog.accepted.connect(reload_device_data)
-
-    def edit_device(self):
-        devices = load_device_data()
-
-        if not devices:
-            return
-
-        device = devices[self.get_list_index()]
+    def edit_device(self) -> None:
+        """Open the dialog to edit the currently selected device."""
+        device = self.devices[self.get_list_index()]
 
         self.dialog = NewDeviceDialog(device)
         self.dialog.setModal(True)
         self.dialog.show()
+        self.dialog.accepted.connect(self.reload_device_data)
 
-        def reload_device_data():
-            # not very elegant...
-            QtCore.QTimer.singleShot(100, self.load_device_data)
-
-        self.dialog.accepted.connect(reload_device_data)
-
-    def move_device_up(self):
-        self.move_device(-1)
-
-    def move_device_down(self):
-        self.move_device(1)
-
-    def move_device(self, direction):
-        devices = load_device_data()
-
-        if not devices:
-            return
-
-        current_index = self.get_list_index()
-        new_index = current_index + direction
-
-        if new_index < 0 or new_index > len(devices) - 1:
-            return
-
-        device = devices.pop(current_index)
-        devices = devices[:new_index] + [device] + devices[new_index:]
-        save_device_data(devices)
-        self.load_device_data()
-        self.deviceList.setCurrentRow(new_index)
-
-    def get_list_index(self):
-        return self.deviceList.currentIndex().row()
-
-    def remove_device(self):
-        devices = load_device_data()
-
-        if not devices:
-            return
-
-        devices.pop(self.get_list_index())
-        save_device_data(devices)
-        self.load_device_data()
-
-    def selected_device_changed(self):
-        idx = self.get_list_index()
+    def move_device_up(self) -> None:
+        """Move the currently selected device up in the list."""
+        self.move_device_in_list(-1)
+
+    def move_device_down(self) -> None:
+        """Move the currently selected device down in the list."""
+        self.move_device_in_list(1)
+
+    def move_device_in_list(self, direction: int) -> None:
+        """Move the currently selected device in the list by the given direction."""
+        selected_index = self.get_list_index()
+        selected_device = self.devices[selected_index]
+        move_device(selected_device, direction)
+        self.populate_device_list()
+        self.deviceList.setCurrentRow(selected_index + direction)
+
+    def remove_device(self) -> None:
+        """
+        Remove the currently selected device from the list and save new list to disk.
+        """
+        selected_device = self.devices[self.get_list_index()]
+        delete_device(selected_device)
+        self.populate_device_list()
 
+    def selected_device_changed(self) -> None:
         disable_buttons = True
 
-        if idx >= 0:
-            devices = load_device_data()
-
-            if devices:
+        if self.get_list_index() >= 0:
+            if self.devices:
                 disable_buttons = False
 
-        for btn in [
+        for button in [
             self.connectButton,
             self.removeButton,
             self.editButton,
             self.moveUpButton,
             self.moveDownButton,
         ]:
-            btn.setEnabled(not disable_buttons)
+            button.setEnabled(not disable_buttons)
```

### Comparing `linien-gui-1.0.2rc1/linien_gui/ui/general_panel.py` & `linien-gui-2.0.0rc1/linien_gui/ui/general_panel.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from linien_common.common import (
     ANALOG_OUT_V,
     OutputChannel,
     convert_channel_mixing_value,
 )
+from linien_gui.config import UI_PATH
 from linien_gui.ui.spin_box import CustomDoubleSpinBoxNoSign
 from linien_gui.utils import get_linien_app_instance, param2ui
-from linien_gui.widgets import UI_PATH
 from PyQt5 import QtWidgets, uic
 
 
 class GeneralPanel(QtWidgets.QWidget):
     analogOutComboBox1: CustomDoubleSpinBoxNoSign
     analogOutComboBox2: CustomDoubleSpinBoxNoSign
     analogOutComboBox3: CustomDoubleSpinBoxNoSign
```

### Comparing `linien-gui-1.0.2rc1/linien_gui/ui/lock_status_panel.py` & `linien-gui-2.0.0rc1/linien_gui/ui/lock_status_panel.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2rc1/linien_gui/ui/locking_panel.py` & `linien-gui-2.0.0rc1/linien_gui/ui/locking_panel.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from linien_common.common import AutolockMode
+from linien_gui.config import UI_PATH
 from linien_gui.ui.lock_status_panel import LockStatusPanel
 from linien_gui.ui.spin_box import CustomSpinBox
 from linien_gui.utils import get_linien_app_instance, param2ui
-from linien_gui.widgets import UI_PATH
 from PyQt5 import QtWidgets, uic
 
 
 class LockingPanel(QtWidgets.QWidget):
     kpSpinBox: CustomSpinBox
     kiSpinBox: CustomSpinBox
     kdSpinBox: CustomSpinBox
```

### Comparing `linien-gui-1.0.2rc1/linien_gui/ui/logging_panel.py` & `linien-gui-2.0.0rc1/linien_gui/ui/logging_panel.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,20 +12,19 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 import logging
-import pickle
 
 from linien_client.remote_parameters import RemoteParameters
 from linien_common.influxdb import InfluxDBCredentials
+from linien_gui.config import UI_PATH
 from linien_gui.utils import get_linien_app_instance
-from linien_gui.widgets import UI_PATH
 from PyQt5 import QtWidgets, uic
 from PyQt5.QtCore import pyqtSignal
 
 START_LOG_BUTTON_TEXT = "Start Logging"
 STOP_LOG_BUTTON_TEXT = "Stop Logging"
 
 logger = logging.getLogger(__name__)
@@ -67,15 +66,15 @@
             self.on_parameter_log_status_changed
         )
         self.logPushButton.clicked.connect(self.on_logging_button_clicked)
         self.influxUpdateButton.clicked.connect(self.on_influx_update_button_clicked)
         self.influx_credentials_update.connect(self.on_influxdb_credentials_updated)
 
         # getting the influxdb credentials from the remote
-        credentials = pickle.loads(self.control.exposed_get_influxdb_credentials())
+        credentials = self.control.exposed_get_influxdb_credentials()
         logger.debug("Received InfluxDB credentials from server.")
         self.lineEditURL.setText(credentials.url)
         self.lineEditOrg.setText(credentials.org)
         self.lineEditToken.setText(credentials.token)
         self.lineEditBucket.setText(credentials.bucket)
         self.lineEditMeas.setText(credentials.measurement)
```

### Comparing `linien-gui-1.0.2rc1/linien_gui/ui/main_window.py` & `linien-gui-2.0.0rc1/linien_gui/ui/main_window.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,30 +12,28 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
-import json
 import logging
 import pickle
 from math import log
-from time import time
 
 import linien_gui
 import numpy as np
+from linien_client.device import add_device, load_device, update_device
 from linien_common.common import check_plot_data
-from linien_gui.config import N_COLORS, Color
+from linien_gui.config import N_COLORS, UI_PATH, Color
 from linien_gui.ui.plot_widget import INVALID_POWER
 from linien_gui.ui.right_panel import RightPanel
 from linien_gui.ui.spin_box import CustomDoubleSpinBox
 from linien_gui.ui.sweep_control import SweepControlWidget, SweepSlider
 from linien_gui.utils import color_to_hex, get_linien_app_instance, set_window_icon
-from linien_gui.widgets import UI_PATH
 from PyQt5 import QtWidgets, uic
 
 ZOOM_STEP = 0.9
 MAX_ZOOM = 50
 MIN_ZOOM = 0
 
 logger = logging.getLogger(__name__)
@@ -65,16 +63,16 @@
     error_std: QtWidgets.QLabel
     legend_control_signal: QtWidgets.QLabel
     legend_control_signal_history: QtWidgets.QLabel
     legend_error_signal: QtWidgets.QLabel
     legend_monitor_signal_history: QtWidgets.QLabel
     legend_slow_signal_history: QtWidgets.QLabel
     rightPanel: RightPanel
-    export_parameters_button: QtWidgets.QPushButton
-    import_parameters_button: QtWidgets.QPushButton
+    exportParametersButton: QtWidgets.QPushButton
+    importParametersButton: QtWidgets.QPushButton
     newVersionAvailableLabel: QtWidgets.QLabel
     pid_parameter_optimization_button: QtWidgets.QPushButton
     settings_toolbox: QtWidgets.QToolBox
     generalPanel: QtWidgets.QWidget
     modSpectroscopyPanel: QtWidgets.QWidget
     optimizationPanel: QtWidgets.QWidget
     loggingPanel: QtWidgets.QWidget
@@ -92,18 +90,16 @@
         self.app.connection_established.connect(self.on_connection_established)
 
         self.reset_std_history()
 
         # handle keyboard events
         self.setFocus()
 
-        self.export_parameters_button.clicked.connect(
-            self.export_parameters_select_file
-        )
-        self.import_parameters_button.clicked.connect(self.import_parameters)
+        self.exportParametersButton.clicked.connect(self.export_parameters)
+        self.importParametersButton.clicked.connect(self.import_parameters)
 
         def display_power(power, element):
             if power == INVALID_POWER:
                 element.hide()
             else:
                 element.show()
                 element.setText(f"{power:.2f}")
@@ -205,67 +201,60 @@
         self.app.close_all_secondary_windows()
         super().closeEvent(*args, **kwargs)
 
     def show_new_version_available(self):
         self.newVersionAvailableLabel.show()
 
     def handle_key_press(self, key):
-        logger.debug("key pressed %s" % key)
+        logger.debug(f"key pressed {key}")
 
-    def export_parameters_select_file(self):
+    def export_parameters(self):
         options = QtWidgets.QFileDialog.Options()
         # options |= QtWidgets.QFileDialog.DontUseNativeDialog
         default_ext = ".json"
         fn, _ = QtWidgets.QFileDialog.getSaveFileName(
             self,
             "QFileDialog.getSaveFileName()",
             "",
-            "JSON (*%s)" % default_ext,
+            f"JSON (*{default_ext})",
             options=options,
         )
         if fn:
             if not fn.endswith(default_ext):
                 fn = fn + default_ext
 
-            with open(fn, "w") as f:
-                json.dump(
-                    {
-                        "linien-version": linien_gui.__version__,
-                        "time": time(),
-                        "parameters": {
-                            name: param.value
-                            for name, param in self.parameters
-                            if param.restorable
-                        },
-                    },
-                    f,
+            try:
+                add_device(self.app.client.device, path=fn)
+            except KeyError:
+                logger.warning(
+                    f"Device with key {self.app.client.device.key} already exists in"
+                    f"{fn}. Updating the device instead."
                 )
+                update_device(self.app.client.device, path=fn)
 
     def import_parameters(self):
         options = QtWidgets.QFileDialog.Options()
         fn, _ = QtWidgets.QFileDialog.getOpenFileName(
             self,
             "QFileDialog.getSaveFileName()",
             "",
             "JSON (*.json)",
             options=options,
         )
         if fn:
-            with open(fn, "r") as f:
-                data = json.load(f)
-
-            if "linien-version" not in data:
-                raise Exception("invalid parameter file")
-
-            for name, value in data["parameters"].items():
-                param = getattr(self.parameters, name)
-                if param.restorable:
+            try:
+                self.app.client.device = load_device(
+                    self.app.client.device.key, path=fn
+                )
+                for name, value in self.app.client.device.parameters.items():
+                    param = getattr(self.app.client.parameters, name)
                     param.value = value
-
-            self.control.write_registers()
+                self.control.exposed_write_registers()
+            except KeyError:
+                logger.error("Unable to load device from file. Key doesn't exist.")
 
     def update_std(self, to_plot, max_std_history_length=10):
         if self.parameters.lock.value and to_plot:
             to_plot = pickle.loads(to_plot)
             if to_plot and check_plot_data(True, to_plot):
                 error_signal = to_plot.get("error_signal")
                 control_signal = to_plot.get("control_signal")
@@ -277,13 +266,13 @@
                     -max_std_history_length:
                 ]
                 self.control_std_history = self.control_std_history[
                     -max_std_history_length:
                 ]
 
                 if error_signal is not None and control_signal is not None:
-                    self.error_std.setText("%.2f" % np.mean(self.error_std_history))
+                    self.error_std.setText(f"{np.mean(self.error_std_history):.2f}")
                     self.control_std.setText(f"{np.mean(self.control_std_history):.2f}")
 
     def reset_std_history(self):
         self.error_std_history = []
         self.control_std_history = []
```

### Comparing `linien-gui-1.0.2rc1/linien_gui/ui/modulation_sweep_panel.py` & `linien-gui-2.0.0rc1/linien_gui/ui/modulation_sweep_panel.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from linien_common.common import MHz, Vpp
+from linien_gui.config import UI_PATH
 from linien_gui.ui.spin_box import CustomDoubleSpinBoxNoSign
 from linien_gui.utils import get_linien_app_instance, param2ui
-from linien_gui.widgets import UI_PATH
 from PyQt5 import QtWidgets, uic
 
 
 class ModulationAndSweepPanel(QtWidgets.QWidget):
     sweepSpeedComboBox: QtWidgets.QGroupBox
     modulation_amplitude_group = QtWidgets.QGroupBox
     modulationAmplitudeSpinBox: CustomDoubleSpinBoxNoSign
```

### Comparing `linien-gui-1.0.2rc1/linien_gui/ui/optimization_panel.py` & `linien-gui-2.0.0rc1/linien_gui/ui/optimization_panel.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from linien_common.common import MHz, Vpp
+from linien_gui.config import UI_PATH
 from linien_gui.ui.spin_box import CustomDoubleSpinBoxNoSign
 from linien_gui.utils import get_linien_app_instance, param2ui
-from linien_gui.widgets import UI_PATH
 from PyQt5 import QtWidgets, uic
 
 
 class OptimizationPanel(QtWidgets.QWidget):
     optimization_failed: QtWidgets.QWidget
     optimization_reset_failed_state: QtWidgets.QPushButton
     optimization_not_running_container: QtWidgets.QWidget
@@ -118,35 +118,31 @@
 
         self.parameters.optimization_selection.add_callback(opt_selection_changed)
 
         def mod_param_changed(_):
             dual_channel = self.parameters.dual_channel.value
             channel = self.parameters.optimization_channel.value
             optimized = self.parameters.optimization_optimized_parameters.value
-
+            mod_phase = (
+                self.parameters.demodulation_phase_a,
+                self.parameters.demodulation_phase_b,
+            )[0 if not dual_channel else (0, 1)[channel]].value
             self.optimization_display_parameters.setText(
                 (
                     "<br />\n"
                     "<b>current parameters</b>: "
-                    " %.2f&nbsp;MHz, %.2f&nbsp;Vpp, %.2f&nbsp;deg<br />\n"
+                    f"{self.parameters.modulation_frequency.value / MHz:.2f}&nbsp;MHz, "
+                    f"{self.parameters.modulation_amplitude.value / Vpp:.2f}&nbsp;Vpp, "
+                    f"{mod_phase:.2f}&nbsp;deg<br />\n"
                     "<b>optimized parameters</b>: "
-                    "%.2f&nbsp;MHz, %.2f&nbsp;Vpp, %.2f&nbsp;deg\n"
+                    f"{optimized[0] / MHz:.2f}&nbsp;MHz, "
+                    f"{optimized[1] / Vpp:.2f}&nbsp;Vpp, "
+                    f"{optimized[2]:.2f}&nbsp;deg\n"
                     "<br />"
                 )
-                % (
-                    self.parameters.modulation_frequency.value / MHz,
-                    self.parameters.modulation_amplitude.value / Vpp,
-                    (
-                        self.parameters.demodulation_phase_a,
-                        self.parameters.demodulation_phase_b,
-                    )[0 if not dual_channel else (0, 1)[channel]].value,
-                    optimized[0] / MHz,
-                    optimized[1] / Vpp,
-                    optimized[2],
-                )
             )
 
         for param in (
             self.parameters.modulation_amplitude,
             self.parameters.modulation_frequency,
             self.parameters.demodulation_phase_a,
         ):
```

### Comparing `linien-gui-1.0.2rc1/linien_gui/ui/plot_widget.py` & `linien-gui-2.0.0rc1/linien_gui/ui/plot_widget.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2rc1/linien_gui/ui/psd_plot_widget.py` & `linien-gui-2.0.0rc1/linien_gui/ui/psd_plot_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     def __init__(self, *args, **kwargs):
         pg.AxisItem.__init__(self, *args, **kwargs)
 
     def logTickStrings(self, values, scale, spacing):
         # this method is mainly taken from pyqtgraph, just taking care that negative
         # exponents are also displayed in scientific notation
         estrings = [
-            "%0.1e" % x for x in 10 ** np.array(values).astype(float) * np.array(scale)
+            f"{x:0.1e}" for x in 10 ** np.array(values).astype(float) * np.array(scale)
         ]
 
         convdict = {
             "0": "⁰",
             "1": "¹",
             "2": "²",
             "3": "³",
@@ -77,15 +77,15 @@
     def __init__(self, *args, **kwargs):
         super(PSDPlotWidget, self).__init__(
             *args,
             axisItems={
                 "bottom": CustomLogAxis(orientation="bottom"),
                 "left": CustomLogAxis(orientation="left"),
             },
-            **kwargs
+            **kwargs,
         )
         self.app = get_linien_app_instance()
         self.app.connection_established.connect(self.on_connection_established)
 
         self.curves = {}
 
         self.setLogMode(x=True, y=True)
@@ -189,15 +189,15 @@
         if self.sceneBoundingRect().contains(pos):
             mousePoint = self.plotItem.vb.mapSceneToView(pos)
             x = mousePoint.x()
             y = mousePoint.y()
 
             # if index > 0 and index < self.MFmax:
             self.cursor_label.setHtml(
-                "<span style='font-size: 12pt'>(%.1e,%.1e)</span>" % (10**x, 10**y)
+                f"<span style='font-size: 12pt'>({10**x:.1e},{10**y:.1e})</span>"
             )
             # this determines whether cursor label is on right or left side of
             # crosshair
             self.cursor_label.setAnchor((1 if x > self._x_max / 2 else 0, 1))
             self.cursor_label.setPos(x, y)
             self.vertical_line.setPos(x)
             self.horizontal_line.setPos(y)
```

### Comparing `linien-gui-1.0.2rc1/linien_gui/ui/psd_table_widget.py` & `linien-gui-2.0.0rc1/linien_gui/ui/psd_table_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             "%Y-%m-%d %H:%M:%S"
         )
         self.setItem(row_count, 2, create_item(time_formatted))
 
         self.setItem(row_count, 3, create_item(data["p"]))
         self.setItem(row_count, 4, create_item(data["i"]))
         self.setItem(row_count, 5, create_item(data["d"]))
-        self.setItem(row_count, 6, create_item("%.4f" % data["fitness"]))
+        self.setItem(row_count, 6, create_item(f"{data['fitness']:.4f}"))
 
         self.resizeColumnsToContents()
 
     def delete_selected_curve(self):
         current = self.currentRow()
         if not self.uuids or current == -1:
             return
```

### Comparing `linien-gui-1.0.2rc1/linien_gui/ui/psd_window.py` & `linien-gui-2.0.0rc1/linien_gui/ui/psd_window.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 import pickle
 from time import time
 
 import linien_gui
 from linien_common.common import PSDAlgorithm
+from linien_gui.config import UI_PATH
 from linien_gui.dialogs import error_dialog
 from linien_gui.utils import (
     RandomColorChoser,
     get_linien_app_instance,
     param2ui,
     set_window_icon,
 )
-from linien_gui.widgets import UI_PATH
 from PyQt5 import QtWidgets, uic
 
 
 class PSDWindow(QtWidgets.QMainWindow):
     def __init__(self, *args, **kwargs):
         super(PSDWindow, self).__init__(*args, **kwargs)
         uic.loadUi(UI_PATH / "psd_window.ui", self)
@@ -74,19 +74,15 @@
         )
 
         param2ui(
             self.parameters.psd_acquisition_max_decimation,
             self.maximum_measurement_time,
             lambda max_decimation: max_decimation - 12,
         )
-        param2ui(
-            self.parameters.psd_algorithm,
-            self.psd_algorithm,
-            lambda algo: {PSDAlgorithm.LPSD: 0, PSDAlgorithm.WELCH: 1}[algo],
-        )
+        param2ui(self.parameters.psd_algorithm, self.psd_algorithm)
 
         def update_status(_):
             psd_running = self.parameters.psd_acquisition_running.value
             if psd_running:
                 self.container_psd_running.show()
                 self.container_psd_not_running.hide()
             else:
@@ -163,15 +159,15 @@
         options = QtWidgets.QFileDialog.Options()
         # options |= QtWidgets.QFileDialog.DontUseNativeDialog
         default_ext = ".pickle"
         fn, _ = QtWidgets.QFileDialog.getSaveFileName(
             self,
             "QFileDialog.getSaveFileName()",
             "",
-            "PICKLE (*%s)" % default_ext,
+            f"PICKLE (*{default_ext})",
             options=options,
         )
         if fn:
             if not fn.endswith(default_ext):
                 fn = fn + default_ext
 
             with open(fn, "wb") as f:
@@ -188,15 +184,15 @@
         options = QtWidgets.QFileDialog.Options()
         # options |= QtWidgets.QFileDialog.DontUseNativeDialog
         default_ext = ".pickle"
         fn, _ = QtWidgets.QFileDialog.getOpenFileName(
             self,
             "QFileDialog.getSaveFileName()",
             "",
-            "JSON (*%s)" % default_ext,
+            f"JSON (*{default_ext})",
             options=options,
         )
         if fn:
             with open(fn, "rb") as f:
                 data = pickle.load(f)
 
             assert "linien-version" in data, "invalid parameter file"
```

### Comparing `linien-gui-1.0.2rc1/linien_gui/ui/right_panel.py` & `linien-gui-2.0.0rc1/linien_gui/ui/right_panel.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2rc1/linien_gui/ui/spectroscopy_panel.py` & `linien-gui-2.0.0rc1/linien_gui/ui/spectroscopy_panel.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from typing import Union
 
 from linien_client.remote_parameters import RemoteParameter
 from linien_common.common import FilterType
+from linien_gui.config import UI_PATH
 from linien_gui.ui.spin_box import CustomDoubleSpinBox, CustomDoubleSpinBoxNoSign
 from linien_gui.utils import get_linien_app_instance, param2ui
-from linien_gui.widgets import UI_PATH
 from PyQt5 import QtWidgets, uic
 
 
 class SpectroscopyPanel(QtWidgets.QWidget):
     CHANNEL: Union[str, None] = None
 
     automaticFilterCheckBox: QtWidgets.QCheckBox
@@ -78,25 +78,26 @@
         self.demodulationPhaseSpinBox.setKeyboardTracking(False)
         self.demodulationPhaseSpinBox.valueChanged.connect(self.change_demod_phase)
         self.demodulationFrequencyComboBox.currentIndexChanged.connect(
             self.change_demod_multiplier
         )
 
         for filter_i in [1, 2]:
-            _get = lambda parent, attr, filter_i=filter_i: getattr(
-                parent, attr.format(filter_i)
-            )
-            _get(self, "filter_{}_enabled").stateChanged.connect(
-                _get(self, "change_filter_{}_enabled")
+
+            def get_(parent, attr, filter_i=filter_i):
+                return getattr(parent, attr.format(filter_i))
+
+            get_(self, "filter_{}_enabled").stateChanged.connect(
+                get_(self, "change_filter_{}_enabled")
             )
-            freq_input = _get(self, "filter_{}_frequency")
+            freq_input = get_(self, "filter_{}_frequency")
             freq_input.setKeyboardTracking(False)
-            freq_input.valueChanged.connect(_get(self, "change_filter_{}_frequency"))
-            _get(self, "filter_{}_type").currentIndexChanged.connect(
-                _get(self, "change_filter_{}_type")
+            freq_input.valueChanged.connect(get_(self, "change_filter_{}_frequency"))
+            get_(self, "filter_{}_type").currentIndexChanged.connect(
+                get_(self, "change_filter_{}_type")
             )
 
         def automatic_changed(value):
             self.get_param("filter_automatic").value = value
             self.control.exposed_write_registers()
 
         self.automaticFilterCheckBox.stateChanged.connect(automatic_changed)
@@ -148,17 +149,17 @@
         return getattr(self.parameters, f"{name}_{self.CHANNEL}")
 
     def change_signal_offset(self):
         self.get_param("offset").value = self.signalOffsetSpinBox.value() * 8191
         self.control.exposed_write_registers()
 
     def change_demod_phase(self):
-        self.get_param(
-            "demodulation_phase"
-        ).value = self.demodulationPhaseSpinBox.value()
+        self.get_param("demodulation_phase").value = (
+            self.demodulationPhaseSpinBox.value()
+        )
         self.control.exposed_write_registers()
 
     def change_demod_multiplier(self, idx):
         self.get_param("demodulation_multiplier").value = idx + 1
         self.control.exposed_write_registers()
```

### Comparing `linien-gui-1.0.2rc1/linien_gui/ui/spin_box.py` & `linien-gui-2.0.0rc1/linien_gui/ui/spin_box.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2rc1/linien_gui/ui/sweep_control.py` & `linien-gui-2.0.0rc1/linien_gui/ui/sweep_control.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2rc1/linien_gui/ui/version_checker.py` & `linien-gui-2.0.0rc1/linien_gui/ui/version_checker.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2rc1/linien_gui/ui/view_panel.py` & `linien-gui-2.0.0rc1/linien_gui/ui/view_panel.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,18 +17,17 @@
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 import json
 import pickle
 from os import path
 
 import numpy as np
-from linien_gui.config import N_COLORS
+from linien_gui.config import N_COLORS, UI_PATH
 from linien_gui.ui.spin_box import CustomDoubleSpinBoxNoSign, CustomSpinBox
 from linien_gui.utils import color_to_hex, get_linien_app_instance, param2ui
-from linien_gui.widgets import UI_PATH
 from PyQt5 import QtGui, QtWidgets, uic
 
 
 class ViewPanel(QtWidgets.QWidget):
     plot_line_width: CustomDoubleSpinBoxNoSign
     plot_line_opacity: CustomSpinBox
     plot_fill_opacity: CustomSpinBox
```

### Comparing `linien-gui-1.0.2rc1/linien_gui/utils.py` & `linien-gui-2.0.0rc1/linien_gui/utils.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2rc1/linien_gui.egg-info/SOURCES.txt` & `linien-gui-2.0.0rc1/linien_gui.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,33 @@
-setup.py
+pyproject.toml
 linien_gui/__init__.py
 linien_gui/app.py
 linien_gui/config.py
 linien_gui/dialogs.py
-linien_gui/icon.ico
 linien_gui/threads.py
 linien_gui/utils.py
-linien_gui/widgets.py
 linien_gui.egg-info/PKG-INFO
 linien_gui.egg-info/SOURCES.txt
 linien_gui.egg-info/dependency_links.txt
 linien_gui.egg-info/entry_points.txt
 linien_gui.egg-info/requires.txt
 linien_gui.egg-info/top_level.txt
 linien_gui/ui/__init__.py
 linien_gui/ui/device_manager.py
-linien_gui/ui/device_manager.ui
 linien_gui/ui/general_panel.py
-linien_gui/ui/general_panel.ui
 linien_gui/ui/lock_status_panel.py
 linien_gui/ui/locking_panel.py
-linien_gui/ui/locking_panel.ui
 linien_gui/ui/logging_panel.py
-linien_gui/ui/logging_panel.ui
 linien_gui/ui/main_window.py
-linien_gui/ui/main_window.ui
 linien_gui/ui/modulation_sweep_panel.py
-linien_gui/ui/modulation_sweep_panel.ui
 linien_gui/ui/new_device_dialog.py
-linien_gui/ui/new_device_dialog.ui
 linien_gui/ui/optimization_panel.py
-linien_gui/ui/optimization_panel.ui
 linien_gui/ui/plot_widget.py
 linien_gui/ui/psd_plot_widget.py
 linien_gui/ui/psd_table_widget.py
 linien_gui/ui/psd_window.py
-linien_gui/ui/psd_window.ui
 linien_gui/ui/right_panel.py
 linien_gui/ui/spectroscopy_panel.py
-linien_gui/ui/spectroscopy_panel.ui
 linien_gui/ui/spin_box.py
 linien_gui/ui/sweep_control.py
 linien_gui/ui/version_checker.py
-linien_gui/ui/view_panel.py
-linien_gui/ui/view_panel.ui
+linien_gui/ui/view_panel.py
```

