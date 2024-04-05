# Comparing `tmp/dashbar-1.1.tar.gz` & `tmp/dashbar-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dashbar-1.1.tar", last modified: Fri Mar  1 19:04:10 2024, max compression
+gzip compressed data, was "dashbar-2.0.tar", last modified: Fri Apr  5 20:17:59 2024, max compression
```

## Comparing `dashbar-1.1.tar` & `dashbar-2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-03-01 19:04:10.670848 dashbar-1.1/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1062 2024-02-23 07:55:01.000000 dashbar-1.1/LICENSE
--rw-r--r--   0 xyz       (1000) xyz       (1000)     2035 2024-03-01 19:04:10.670848 dashbar-1.1/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1625 2024-03-01 19:01:58.000000 dashbar-1.1/README.md
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-03-01 19:04:10.669848 dashbar-1.1/dashbar/
--rw-r--r--   0 xyz       (1000) xyz       (1000)      292 2024-03-01 18:46:24.000000 dashbar-1.1/dashbar/__init__.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)      798 2024-02-23 07:55:01.000000 dashbar-1.1/dashbar/_dashBuilder.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1420 2024-02-23 07:55:01.000000 dashbar-1.1/dashbar/_dashbarElements.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)      551 2024-02-23 07:55:01.000000 dashbar-1.1/dashbar/demo.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)     5515 2024-03-01 11:54:50.000000 dashbar-1.1/dashbar/main.py
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-03-01 19:04:10.670848 dashbar-1.1/dashbar.egg-info/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     2035 2024-03-01 19:04:10.000000 dashbar-1.1/dashbar.egg-info/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)      254 2024-03-01 19:04:10.000000 dashbar-1.1/dashbar.egg-info/SOURCES.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-03-01 19:04:10.000000 dashbar-1.1/dashbar.egg-info/dependency_links.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)        8 2024-03-01 19:04:10.000000 dashbar-1.1/dashbar.egg-info/top_level.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-03-01 19:04:10.670848 dashbar-1.1/setup.cfg
--rw-r--r--   0 xyz       (1000) xyz       (1000)      634 2024-03-01 18:52:11.000000 dashbar-1.1/setup.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-05 20:17:59.655410 dashbar-2.0/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1062 2024-02-23 07:55:01.000000 dashbar-2.0/LICENSE
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     2284 2024-04-05 20:17:59.655410 dashbar-2.0/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1494 2024-04-05 20:02:57.000000 dashbar-2.0/README.md
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-05 20:17:59.653410 dashbar-2.0/dashbar/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     5796 2024-04-05 20:17:45.000000 dashbar-2.0/dashbar/__init__.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      798 2024-02-23 07:55:01.000000 dashbar-2.0/dashbar/_dashBuilder.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1714 2024-04-05 19:44:45.000000 dashbar-2.0/dashbar/_dashbarElements.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      551 2024-02-23 07:55:01.000000 dashbar-2.0/dashbar/demo.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      165 2024-04-05 18:04:02.000000 dashbar-2.0/dashbar/exceptions.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-05 20:17:59.655410 dashbar-2.0/dashbar.egg-info/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     2284 2024-04-05 20:17:59.000000 dashbar-2.0/dashbar.egg-info/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      260 2024-04-05 20:17:59.000000 dashbar-2.0/dashbar.egg-info/SOURCES.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-04-05 20:17:59.000000 dashbar-2.0/dashbar.egg-info/dependency_links.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)        8 2024-04-05 20:17:59.000000 dashbar-2.0/dashbar.egg-info/top_level.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-04-05 20:17:59.655410 dashbar-2.0/setup.cfg
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      961 2024-04-05 17:29:08.000000 dashbar-2.0/setup.py
```

### Comparing `dashbar-1.1/LICENSE` & `dashbar-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dashbar-1.1/PKG-INFO` & `dashbar-2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,77 +1,58 @@
-Metadata-Version: 2.1
-Name: dashbar
-Version: 1.1
-Summary: A progress-bar designed to be useful and easy to use.
-Home-page: https://github.com/xyzpw/dashbar/
-Author: xyzpw
-Maintainer: xyzpw
-License: MIT
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Topic :: Utilities
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # dashbar
 ![PyPI - Version](https://img.shields.io/pypi/v/dashbar)
-![Pepy Total Downlods](https://img.shields.io/pepy/dt/dashbar?color=red)
+![Pepy Total Downloads](https://img.shields.io/pepy/dt/dashbar?color=red)
 ![GitHub repo size](https://img.shields.io/github/repo-size/xyzpw/dashbar)<br/><br/>
 A progress-bar designed to be useful and easy to use.<br/><br/>
 ![dashbar-demo-preview](https://github.com/xyzpw/dashbar/assets/76017734/d5a3bd52-2bc5-455d-ba63-fe28249defe8)
-# Usage
-Firstly, you need to install `dashbar`<br>
-```bash
-$ pip3 install dashbar
-```
-For this example, we will also need the `time` module
-```python
-import dashbar, time
-```
-## Iterating
-To start dashbar, execute the following code
+## Usage
+### Iterating
+To start dashbar, execute the following code:
 ```python
 for i in dashbar.dash(10, dash_type="pipe", desc="example"):
     time.sleep(1/10) #completion after one second
     if i == 5:
         dashbar.status("half-way complete")
 ```
-If the progress is large, the `autodash` function can be used, which adjusts the step count to fit the terminal
+If the progress is large, the `autodash` function can be used, which adjusts the step count to fit the terminal:
 ```python
 for i in dashbar.autodash(10):
     time.sleep(1/10)
     if i == 8:
         dashbar.log("eighty percent complete")
 ```
-## Customizing dashbar
+
+### Customizing dashbar
 Dashbars can be customized with the following code:
 ```python
 dashbar.customize(element="filler", value=" ")
 ```
 List of dashbars:
 - classic
 - arrow
 - box
 - circle_charger
 - box_charger
 - striped
 - dollar
 - box_shade
 - pipe
+- heart
+- radioactive
 - custom
 
 List of dashbar elements:
 - start
 - head
 - trail
 - filler
 - finish
-## Building a Dashbar
-Dashbars can be built via the `Build` class
+
+### Building a Dashbar
+Dashbars can be built via the `Dashbar` class:
 ```python
-bar = dashbar.Build(10, "box_shade")
+bar = dashbar.Dashbar(10, "box_shade")
 for i in range(100):
     if i%10 == 0:
         bar.update(1, display=True)
     time.sleep(1/20) #completion after five seconds
 ```
```

### Comparing `dashbar-1.1/dashbar/_dashBuilder.py` & `dashbar-2.0/dashbar/_dashBuilder.py`

 * *Files identical despite different names*

### Comparing `dashbar-1.1/dashbar/_dashbarElements.py` & `dashbar-2.0/dashbar/_dashbarElements.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,14 +58,28 @@
     "pipe": {
         "start": "[",
         "head": "|",
         "trail": "|",
         "filler": " ",
         "finish": "]",
     },
+    "heart": {
+        "start": "|",
+        "head": "\u2665",
+        "trail":"\u2665",
+        "filler":"\u2661",
+        "finish":"|",
+    },
+    "radioactive": {
+        "start": "|",
+        "head": "\u2622",
+        "trail": "\u2622",
+        "filler": " ",
+        "finish": "|",
+    },
     "custom": {
         "start": "[",
         "head": "#",
         "trail": "#",
         "filler": ".",
         "finish": "]",
     },
```

### Comparing `dashbar-1.1/dashbar/demo.py` & `dashbar-2.0/dashbar/demo.py`

 * *Files identical despite different names*

### Comparing `dashbar-1.1/dashbar/main.py` & `dashbar-2.0/dashbar/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,47 @@
+"""A progress-bar designed to be useful and easy to use."""
+
 from . import _dashBuilder
 from . import _dashbarElements
 import shutil
+from .exceptions import *
+
+__all__ = [
+    "customize",
+    "log",
+    "status",
+    "dash",
+    "autodash",
+    "Dashbar",
+]
+
+__version__ = "2.0"
+__description__ = "A progress-bar designed to be useful and easy to use."
+__author__ = "xyzpw"
 global all_bars
 all_bars = dict(_dashbarElements.all_bars)
 
 def customize(element: str, value: str) -> None:
-    """
-    Customizable dashbar is equivalent to 'classic' dashbar by default.
+    """Customizable dashbar is equivalent to 'classic' dashbar by default.
+
     Elements:
         start
         head
         trail
         filler
-        finish
-    """
+        finish"""
     global all_bars
     if not isinstance(element, str) or not isinstance(value, str):
-        raise TypeError("both parameters must type string")
+        raise DashbarError("both parameters must type string")
     if element in all_bars["custom"]:
         if len(value) != 1:
-            raise ValueError("value must be type char")
+            raise DashbarError("customizable element must be type char")
         all_bars["custom"][element] = value
         return
-    raise ValueError("dashbar element not found")
+    raise DashbarError("customizable element does not exist")
 
 spinner_parts = ['|', '/', '\u2013', '\\']
 
 def log(text: str):
     global mydash
     try:
         print(f"\x1b[2K\r{text}\n{mydash}", end='', flush=True)
@@ -88,15 +103,15 @@
             mydash += " " + str(int(progress/count*100)) + "%"
         if bool(desc):
             print(f"\x1b[2K\r{desc} {mydash}", end='', flush=True)
         else:
             print(f"\x1b[2K\r{mydash}", end='', flush=True)
     del mydash
 
-class Build:
+class Dashbar:
     def __init__(self, steps: int, dash_type: str = "classic",
                  desc: str = None, percent: bool = False, spinner: bool = False):
         self.steps = steps
         self.dash_type = dash_type
         self.desc = desc
         self.percent = percent
         self.spinner = spinner
@@ -126,25 +141,24 @@
     def update(self, count: int = 1, display: bool = False):
         if self.progress + count >= self.steps and not self.iscomplete:
             self.complete()
             if display:
                 self.display()
             return
         elif self.iscomplete:
-            raise Exception("could not update dashbar: dashbar is already complete")
+            raise DashbarError("dashbar is already complete")
         self.progress += count
         self.dashbar = _dashBuilder.buildFromProgress(self.dash_type, self.progress, self.steps)
         self.build_dashbar()
         if display:
             self.display()
     def display(self):
         print(f"\x1b[2K\r{self.dashbar}", end='', flush=True)
         if self.iscomplete:
             print("\n", end='', flush=True)
     def set_status(self, text: str = None) -> str:
         if self.iscomplete:
-            raise Exception("could not update dashbar: dashbar is already complete")
+            raise DashbarError("dashbar is already complete")
         self.status = text
         self.build_dashbar()
     def log(self, text: str):
         print(f"\x1b[2K\r{text}\n{self.dashbar}", end='', flush=True)
-
```

### Comparing `dashbar-1.1/dashbar.egg-info/PKG-INFO` & `dashbar-2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,81 @@
 Metadata-Version: 2.1
 Name: dashbar
-Version: 1.1
+Version: 2.0
 Summary: A progress-bar designed to be useful and easy to use.
 Home-page: https://github.com/xyzpw/dashbar/
 Author: xyzpw
 Maintainer: xyzpw
 License: MIT
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Environment :: Console :: Curses
+Classifier: Environment :: Console
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dashbar
 ![PyPI - Version](https://img.shields.io/pypi/v/dashbar)
-![Pepy Total Downlods](https://img.shields.io/pepy/dt/dashbar?color=red)
+![Pepy Total Downloads](https://img.shields.io/pepy/dt/dashbar?color=red)
 ![GitHub repo size](https://img.shields.io/github/repo-size/xyzpw/dashbar)<br/><br/>
 A progress-bar designed to be useful and easy to use.<br/><br/>
 ![dashbar-demo-preview](https://github.com/xyzpw/dashbar/assets/76017734/d5a3bd52-2bc5-455d-ba63-fe28249defe8)
-# Usage
-Firstly, you need to install `dashbar`<br>
-```bash
-$ pip3 install dashbar
-```
-For this example, we will also need the `time` module
-```python
-import dashbar, time
-```
-## Iterating
-To start dashbar, execute the following code
+## Usage
+### Iterating
+To start dashbar, execute the following code:
 ```python
 for i in dashbar.dash(10, dash_type="pipe", desc="example"):
     time.sleep(1/10) #completion after one second
     if i == 5:
         dashbar.status("half-way complete")
 ```
-If the progress is large, the `autodash` function can be used, which adjusts the step count to fit the terminal
+If the progress is large, the `autodash` function can be used, which adjusts the step count to fit the terminal:
 ```python
 for i in dashbar.autodash(10):
     time.sleep(1/10)
     if i == 8:
         dashbar.log("eighty percent complete")
 ```
-## Customizing dashbar
+
+### Customizing dashbar
 Dashbars can be customized with the following code:
 ```python
 dashbar.customize(element="filler", value=" ")
 ```
 List of dashbars:
 - classic
 - arrow
 - box
 - circle_charger
 - box_charger
 - striped
 - dollar
 - box_shade
 - pipe
+- heart
+- radioactive
 - custom
 
 List of dashbar elements:
 - start
 - head
 - trail
 - filler
 - finish
-## Building a Dashbar
-Dashbars can be built via the `Build` class
+
+### Building a Dashbar
+Dashbars can be built via the `Dashbar` class:
 ```python
-bar = dashbar.Build(10, "box_shade")
+bar = dashbar.Dashbar(10, "box_shade")
 for i in range(100):
     if i%10 == 0:
         bar.update(1, display=True)
     time.sleep(1/20) #completion after five seconds
 ```
```

