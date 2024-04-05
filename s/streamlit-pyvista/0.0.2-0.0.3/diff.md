# Comparing `tmp/streamlit_pyvista-0.0.2.tar.gz` & `tmp/streamlit_pyvista-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_pyvista-0.0.2.tar", max compression
+gzip compressed data, was "streamlit_pyvista-0.0.3.tar", max compression
```

## Comparing `streamlit_pyvista-0.0.2.tar` & `streamlit_pyvista-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      104 2024-04-04 10:31:45.971112 streamlit_pyvista-0.0.2/README.md
--rw-r--r--   0        0        0     1806 2024-04-04 10:31:51.643100 streamlit_pyvista-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3671 2024-04-04 10:31:45.972112 streamlit_pyvista-0.0.2/streamlit_pyvista/MeshViewerComponent.py
--rw-r--r--   0        0        0       89 2024-04-04 10:31:45.972112 streamlit_pyvista-0.0.2/streamlit_pyvista/__init__.py
--rw-r--r--   0        0        0    17116 2024-04-04 10:31:45.972112 streamlit_pyvista-0.0.2/streamlit_pyvista/trame_viewer.py
--rw-r--r--   0        0        0      208 2024-04-04 10:31:45.973112 streamlit_pyvista-0.0.2/streamlit_pyvista/utils.py
--rw-r--r--   0        0        0     2982 1970-01-01 00:00:00.000000 streamlit_pyvista-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      104 2024-04-04 15:24:24.628601 streamlit_pyvista-0.0.3/README.md
+-rw-r--r--   0        0        0     1808 2024-04-04 15:24:30.241540 streamlit_pyvista-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5972 2024-04-04 15:24:24.629601 streamlit_pyvista-0.0.3/streamlit_pyvista/MeshViewerComponent.py
+-rw-r--r--   0        0        0       89 2024-04-04 15:24:24.629601 streamlit_pyvista-0.0.3/streamlit_pyvista/__init__.py
+-rw-r--r--   0        0        0    17555 2024-04-04 15:24:24.629601 streamlit_pyvista-0.0.3/streamlit_pyvista/trame_viewer.py
+-rw-r--r--   0        0        0      208 2024-04-04 15:24:24.630601 streamlit_pyvista-0.0.3/streamlit_pyvista/utils.py
+-rw-r--r--   0        0        0     2986 1970-01-01 00:00:00.000000 streamlit_pyvista-0.0.3/PKG-INFO
```

### Comparing `streamlit_pyvista-0.0.2/pyproject.toml` & `streamlit_pyvista-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "streamlit-pyvista"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["Maxime Rochat <rochat.max@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9.12"
 aiohttp = "3.9.3"
 aiosignal = "1.3.1"
 altair = "5.2.0"
 async-timeout = "4.0.3"
 attrs = "23.2.0"
 blinker = "1.7.0"
 cachetools = "5.3.2"
```

### Comparing `streamlit_pyvista-0.0.2/streamlit_pyvista/trame_viewer.py` & `streamlit_pyvista-0.0.3/streamlit_pyvista/trame_viewer.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 from trame.app import get_server
 from trame.ui.vuetify3 import VAppLayout
 from trame.widgets import vuetify3 as vuetify
 from trame.widgets import html
 from aiohttp import web
 from trame.decorators import TrameApp, change, controller
 
+import logging
 import os
 import numpy as np
 import time, threading
 import asyncio
 from abc import ABC, abstractmethod
 
 from typing import Dict
 
+root_logger = logging.getLogger("solidipes")
+root_logger.propagate = True
+root_logger.setLevel(logging.INFO)
+if "FULL_SOLIDIPES_LOG" not in os.environ:
+    root_logger.setLevel(logging.INFO)
 
 @TrameApp()
 class MeshViewer:
 
     def __init__(self, mesh=None, plotter=None, server=None, port=8080):
-
+        root_logger.info("Server started")
         pv.OFF_SCREEN = True
         self.scalar_bar_exist = None
         if server is None:
             self.server = get_server(port=port)
         else:
             self.server = server
         self.slider_playing = False
@@ -388,17 +394,18 @@
         return warper
 
     def build_mesh_control_layout(self):
         layout = html.Div()
         with (layout):
             with vuetify.VRow(dense=True):
                 with vuetify.VCol(cols="6"):
-                    if self.state.options[0] is not None:
+                    if self.state.options[0] is not None and len(self.state.options) > 1:
                         self.option_dropdown()
-                self.build_warper()
+                if len(self.state.options) > 1:
+                    self.build_warper()
             vuetify.VCheckbox(v_model=("wireframe_on",), label="Wireframe on")
             if self.sequence_bounds[1] != 1:
                 self.build_slider()
 
             with vuetify.VBtn(click=self.request_full, style="position: absolute; bottom:25px; right:25px;", icon=True):
                 vuetify.VIcon("mdi-fullscreen" if not self.state.is_full_screen else "mdi-fullscreen-exit")
         return layout
@@ -476,11 +483,12 @@
     def render(self):
         pass
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description='Launch a trame server instance')
     parser.add_argument('--port', type=int, help='Specify the port of the server')
+    parser.add_argument('--server', action="store_true",help='Specify if the trame is opened as a server')
     args = parser.parse_args()
     mv = MeshViewer(port=args.port)
     mv.start_server()
```

### Comparing `streamlit_pyvista-0.0.2/PKG-INFO` & `streamlit_pyvista-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: streamlit-pyvista
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Author: Maxime Rochat
 Author-email: rochat.max@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9.12,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (==3.9.3)
 Requires-Dist: aiosignal (==1.3.1)
 Requires-Dist: altair (==5.2.0)
```

