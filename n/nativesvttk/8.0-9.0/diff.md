# Comparing `tmp/nativesvttk-8.0.tar.gz` & `tmp/nativesvttk-9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nativesvttk-8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "nativesvttk-9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nativesvttk-8.0.tar` & `nativesvttk-9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      406 2024-03-28 01:04:46.516609 nativesvttk-8.0/README.md
--rw-r--r--   0        0        0   186675 2024-03-29 21:17:58.615967 nativesvttk-8.0/nativesvttk/Blank.ico
--rw-r--r--   0        0        0     3460 2024-03-31 00:58:43.114272 nativesvttk-8.0/nativesvttk/__init__.py
--rw-r--r--   0        0        0     3302 2024-03-31 01:22:26.894298 nativesvttk-8.0/nativesvttk/messagebox.py
--rw-r--r--   0        0        0        0 2024-03-27 23:40:19.708805 nativesvttk-8.0/nativesvttk/py.typed
--rw-r--r--   0        0        0     5035 2024-03-27 23:40:19.708805 nativesvttk-8.0/nativesvttk/sv.tcl
--rw-r--r--   0        0        0    16159 2024-03-27 23:40:19.708805 nativesvttk-8.0/nativesvttk/theme/dark.tcl
--rw-r--r--   0        0        0    16282 2024-03-27 23:40:19.708805 nativesvttk-8.0/nativesvttk/theme/light.tcl
--rw-r--r--   0        0        0     3045 2024-03-27 23:40:19.708805 nativesvttk-8.0/nativesvttk/theme/sprites_dark.tcl
--rw-r--r--   0        0        0     3045 2024-03-27 23:40:19.708805 nativesvttk-8.0/nativesvttk/theme/sprites_light.tcl
--rw-r--r--   0        0        0    18371 2024-03-27 23:40:19.708805 nativesvttk-8.0/nativesvttk/theme/spritesheet_dark.png
--rw-r--r--   0        0        0    18388 2024-03-27 23:40:19.708805 nativesvttk-8.0/nativesvttk/theme/spritesheet_light.png
--rw-r--r--   0        0        0      776 2024-03-31 01:22:44.390298 nativesvttk-8.0/pyproject.toml
--rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 nativesvttk-8.0/PKG-INFO
+-rw-r--r--   0        0        0      406 2024-03-28 01:04:46.516609 nativesvttk-9.0/README.md
+-rw-r--r--   0        0        0   186675 2024-03-29 21:17:58.615967 nativesvttk-9.0/nativesvttk/Blank.ico
+-rw-r--r--   0        0        0     3772 2024-03-31 01:31:16.494308 nativesvttk-9.0/nativesvttk/__init__.py
+-rw-r--r--   0        0        0     3302 2024-03-31 01:22:26.894298 nativesvttk-9.0/nativesvttk/messagebox.py
+-rw-r--r--   0        0        0        0 2024-03-27 23:40:19.708805 nativesvttk-9.0/nativesvttk/py.typed
+-rw-r--r--   0        0        0     5035 2024-03-27 23:40:19.708805 nativesvttk-9.0/nativesvttk/sv.tcl
+-rw-r--r--   0        0        0    16159 2024-03-27 23:40:19.708805 nativesvttk-9.0/nativesvttk/theme/dark.tcl
+-rw-r--r--   0        0        0    16282 2024-03-27 23:40:19.708805 nativesvttk-9.0/nativesvttk/theme/light.tcl
+-rw-r--r--   0        0        0     3045 2024-03-27 23:40:19.708805 nativesvttk-9.0/nativesvttk/theme/sprites_dark.tcl
+-rw-r--r--   0        0        0     3045 2024-03-27 23:40:19.708805 nativesvttk-9.0/nativesvttk/theme/sprites_light.tcl
+-rw-r--r--   0        0        0    18371 2024-03-27 23:40:19.708805 nativesvttk-9.0/nativesvttk/theme/spritesheet_dark.png
+-rw-r--r--   0        0        0    18388 2024-03-27 23:40:19.708805 nativesvttk-9.0/nativesvttk/theme/spritesheet_light.png
+-rw-r--r--   0        0        0      776 2024-03-31 01:32:24.594309 nativesvttk-9.0/pyproject.toml
+-rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 nativesvttk-9.0/PKG-INFO
```

### Comparing `nativesvttk-8.0/nativesvttk/Blank.ico` & `nativesvttk-9.0/nativesvttk/Blank.ico`

 * *Files identical despite different names*

### Comparing `nativesvttk-8.0/nativesvttk/__init__.py` & `nativesvttk-9.0/nativesvttk/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 import tkinter
 from functools import partial
 from pathlib import Path
 from tkinter import ttk
 import ctypes as ct
 import os
 os.system("pip install darkdetect")
+os.system("pip install platform")
 import darkdetect
+import platform
 
 TCL_THEME_FILE_PATH = Path(__file__).with_name("sv.tcl").absolute()
 
 def center(win):
     """
     centers a tkinter window
     :param win: the main window or Toplevel window to center
@@ -95,12 +97,16 @@
     if is_dark:
         titlebar(root,"dark")
         toggle_theme()
     else:
         titlebar(root,"light")
     center(root)
 
-
+def system_check():
+    if platform.system() == "Windows":
+        print("All functionality available")
+    else:
+        print("Some features are ristricted.\nTheese features include:messagebox, native theme, and titlebar.\nPlease do not use theese functions.")
 use_dark_theme = partial(set_theme, "dark")
 use_light_theme = partial(set_theme, "light")
```

### Comparing `nativesvttk-8.0/nativesvttk/messagebox.py` & `nativesvttk-9.0/nativesvttk/messagebox.py`

 * *Files identical despite different names*

### Comparing `nativesvttk-8.0/nativesvttk/sv.tcl` & `nativesvttk-9.0/nativesvttk/sv.tcl`

 * *Files identical despite different names*

### Comparing `nativesvttk-8.0/nativesvttk/theme/dark.tcl` & `nativesvttk-9.0/nativesvttk/theme/dark.tcl`

 * *Files identical despite different names*

### Comparing `nativesvttk-8.0/nativesvttk/theme/light.tcl` & `nativesvttk-9.0/nativesvttk/theme/light.tcl`

 * *Files identical despite different names*

### Comparing `nativesvttk-8.0/nativesvttk/theme/sprites_dark.tcl` & `nativesvttk-9.0/nativesvttk/theme/sprites_dark.tcl`

 * *Files identical despite different names*

### Comparing `nativesvttk-8.0/nativesvttk/theme/sprites_light.tcl` & `nativesvttk-9.0/nativesvttk/theme/sprites_light.tcl`

 * *Files identical despite different names*

### Comparing `nativesvttk-8.0/nativesvttk/theme/spritesheet_dark.png` & `nativesvttk-9.0/nativesvttk/theme/spritesheet_dark.png`

 * *Files identical despite different names*

### Comparing `nativesvttk-8.0/nativesvttk/theme/spritesheet_light.png` & `nativesvttk-9.0/nativesvttk/theme/spritesheet_light.png`

 * *Files identical despite different names*

### Comparing `nativesvttk-8.0/pyproject.toml` & `nativesvttk-9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]  # Specify Flit as the build backend
 build-backend = "flit_core.buildapi"
 
 # Project metadata (PEP 621 standard)
 [project]
 name = "nativesvttk"  # Your package name on PyPI
-version = "8.0"  # Version number
+version = "9.0"  # Version number
 requires-python = ">=3.8"  # Required Python version
 authors = [
     {name = "Johnny", email = "johnny@johnnytech.net"},
 ]  # List of authors
 
 # Optional metadata fields
 description = "Even more windows 11-like! With custom titlebars, Making themed apps is now so easy!"
```

### Comparing `nativesvttk-8.0/PKG-INFO` & `nativesvttk-9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nativesvttk
-Version: 8.0
+Version: 9.0
 Summary: Even more windows 11-like! With custom titlebars, Making themed apps is now so easy!
 Author-email: Johnny <johnny@johnnytech.net>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 
 <div text-align=center>
```

