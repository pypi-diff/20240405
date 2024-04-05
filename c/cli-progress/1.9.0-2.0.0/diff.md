# Comparing `tmp/cli_progress-1.9.0.tar.gz` & `tmp/cli_progress-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli_progress-1.9.0.tar", last modified: Mon Apr  1 15:09:06 2024, max compression
+gzip compressed data, was "cli_progress-2.0.0.tar", last modified: Fri Apr  5 10:21:17 2024, max compression
```

## Comparing `cli_progress-1.9.0.tar` & `cli_progress-2.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:09:06.225836 cli_progress-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-01 15:08:54.000000 cli_progress-1.9.0/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:08:54.000000 cli_progress-1.9.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-01 15:08:54.000000 cli_progress-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-01 15:08:54.000000 cli_progress-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-01 15:09:06.225836 cli_progress-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-04-01 15:08:54.000000 cli_progress-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:09:06.221836 cli_progress-1.9.0/cli_progress/
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-01 15:08:54.000000 cli_progress-1.9.0/cli_progress/ANSIWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-01 15:08:54.000000 cli_progress-1.9.0/cli_progress/BackgroundWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-01 15:08:54.000000 cli_progress-1.9.0/cli_progress/LogListWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 15:08:54.000000 cli_progress-1.9.0/cli_progress/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:08:54.000000 cli_progress-1.9.0/cli_progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-01 15:08:54.000000 cli_progress-1.9.0/cli_progress/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-04-01 15:08:54.000000 cli_progress-1.9.0/cli_progress/progress_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:09:06.221836 cli_progress-1.9.0/cli_progress.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-01 15:09:06.000000 cli_progress-1.9.0/cli_progress.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-01 15:09:06.000000 cli_progress-1.9.0/cli_progress.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:09:06.000000 cli_progress-1.9.0/cli_progress.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-01 15:09:06.000000 cli_progress-1.9.0/cli_progress.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-01 15:09:06.000000 cli_progress-1.9.0/cli_progress.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-01 15:09:06.000000 cli_progress-1.9.0/cli_progress.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:09:06.225836 cli_progress-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-01 15:08:54.000000 cli_progress-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:09:06.221836 cli_progress-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:08:54.000000 cli_progress-1.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-01 15:08:54.000000 cli_progress-1.9.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-01 15:08:54.000000 cli_progress-1.9.0/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:21:17.480252 cli_progress-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-05 10:21:09.000000 cli_progress-2.0.0/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:21:09.000000 cli_progress-2.0.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-05 10:21:09.000000 cli_progress-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-05 10:21:09.000000 cli_progress-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-05 10:21:17.480252 cli_progress-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-04-05 10:21:09.000000 cli_progress-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:21:17.476252 cli_progress-2.0.0/cli_progress/
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-05 10:21:09.000000 cli_progress-2.0.0/cli_progress/ANSIWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-05 10:21:09.000000 cli_progress-2.0.0/cli_progress/BackgroundWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-05 10:21:09.000000 cli_progress-2.0.0/cli_progress/LogListWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 10:21:09.000000 cli_progress-2.0.0/cli_progress/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:21:09.000000 cli_progress-2.0.0/cli_progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-05 10:21:09.000000 cli_progress-2.0.0/cli_progress/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-04-05 10:21:09.000000 cli_progress-2.0.0/cli_progress/progress_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:21:17.476252 cli_progress-2.0.0/cli_progress.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-05 10:21:17.000000 cli_progress-2.0.0/cli_progress.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-05 10:21:17.000000 cli_progress-2.0.0/cli_progress.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 10:21:17.000000 cli_progress-2.0.0/cli_progress.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-05 10:21:17.000000 cli_progress-2.0.0/cli_progress.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-05 10:21:17.000000 cli_progress-2.0.0/cli_progress.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 10:21:17.000000 cli_progress-2.0.0/cli_progress.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 10:21:17.480252 cli_progress-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-05 10:21:09.000000 cli_progress-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:21:17.476252 cli_progress-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:21:09.000000 cli_progress-2.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-05 10:21:09.000000 cli_progress-2.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-05 10:21:09.000000 cli_progress-2.0.0/tests/test_base.py
```

### Comparing `cli_progress-1.9.0/LICENSE` & `cli_progress-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cli_progress-1.9.0/PKG-INFO` & `cli_progress-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: cli_progress
-Version: 1.9.0
+Version: 2.0.0
 Summary: Awesome cli_progress created by hiddify
 Home-page: https://github.com/hiddify/cli_progress/
 Author: hiddify
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: urwid==2.6.10
-Requires-Dist: Twisted==24.3.0
-Requires-Dist: pyOpenSSL==24.1.0
-Requires-Dist: service-identity==24.1.0
 Requires-Dist: argparse==1.4.0
+Requires-Dist: asyncio
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: isort; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
```

### Comparing `cli_progress-1.9.0/README.md` & `cli_progress-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cli_progress-1.9.0/cli_progress/ANSIWidget.py` & `cli_progress-2.0.0/cli_progress/ANSIWidget.py`

 * *Files identical despite different names*

### Comparing `cli_progress-1.9.0/cli_progress/BackgroundWidget.py` & `cli_progress-2.0.0/cli_progress/BackgroundWidget.py`

 * *Files identical despite different names*

### Comparing `cli_progress-1.9.0/cli_progress/LogListWidget.py` & `cli_progress-2.0.0/cli_progress/LogListWidget.py`

 * *Files identical despite different names*

### Comparing `cli_progress-1.9.0/cli_progress/__main__.py` & `cli_progress-2.0.0/cli_progress/__main__.py`

 * *Files identical despite different names*

### Comparing `cli_progress-1.9.0/cli_progress/progress_ui.py` & `cli_progress-2.0.0/cli_progress/progress_ui.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 
 import re
 import signal
 import subprocess
 import sys
 import os
 from pathlib import Path
-
+import asyncio
 import urwid
-from twisted.internet import threads
 
 from .BackgroundWidget import BackgroundView
 from .LogListWidget import LogListBox
 
-main_event_loop = urwid.TwistedEventLoop()
+main_event_loop = urwid.AsyncioEventLoop(loop=asyncio.get_event_loop())
 
 palette = [
     ("screen edge", "light blue", "dark blue"),
     ("main shadow", "dark gray", "black"),
     ("body", "default", "default"),
     ("foot", "dark cyan", "dark blue", "bold"),
     ("key", "light cyan", "dark blue", "underline"),
@@ -132,32 +131,39 @@
         self.progressbar_header.set_text(
             [
                 ("progress_header_title", title),
                 (" "),
                 ("progress_header_descr", subtitle),
             ]
         )
-
-    def start(self):
-        os.makedirs(Path(self.logpath).parent.absolute(),exist_ok=True)
-        with open(self.logpath, "w") as self.logfile:
-            self.proc = subprocess.Popen(
-                self.cmds,
+    async def execute_command(self):
+        self.proc = await asyncio.create_subprocess_exec(
+                *self.cmds,
                 stdout=self.write_fd,
                 stderr=self.write_fd_err,
                 close_fds=True,
             )
+
+        # Wait for the process to finish
+        await self.proc.wait()
+        
+        self.exit_loop(self.proc.returncode)
+        
+    def start(self):
+        os.makedirs(Path(self.logpath).parent.absolute(),exist_ok=True)
+        asyncio.get_event_loop().add_signal_handler(signal.SIGINT,self.exit_handler, asyncio.get_event_loop())
+        asyncio.get_event_loop().add_signal_handler(signal.SIGTERM, self.exit_handler, asyncio.get_event_loop())
+        with open(self.logpath, "w") as self.logfile:
             
-            d = threads.deferToThread(self.proc.wait)
-            d.addCallback(self.exit_loop)
-            # try:
+            asyncio.get_event_loop().create_task(self.execute_command())
             self.loop.run()
-            # except:
-            #     pass
-            self.proc.send_signal(signal.SIGTERM)
+            try:
+                self.proc.send_signal(signal.SIGTERM)
+            except:
+                pass
             sys.exit(self.exit_code)
 
     def exit_loop_finish_proceess(self, exit_code):
         # self.handle_line("Process Finished... To Exit Press Q",False)
         self.exit_code = exit_code
         if exit_code:
             self.progressbar.normal = "progressbar_error"
@@ -171,14 +177,27 @@
             if self.listbox.is_focus_end():
                 main_event_loop.alarm(1, self.exit_loop_exception)
 
     def exit_loop_exception(self):
         if self.listbox.is_focus_end():
             raise urwid.ExitMainLoop
 
-    @main_event_loop.handle_exit
+    # @main_event_loop.handle_exit
     def exit_loop(self, exit_code):
         main_event_loop.alarm(0, lambda: self.exit_loop_finish_proceess(exit_code))
+        # asyncio.get_event_loop().stop()
+    def exit_handler(self, loop):
+        try:
+            self.proc.send_signal(signal.SIGINT)
+        except:
+            try:
+                self.proc.send_signal(signal.SIGTERM)
+            except:
+                sys.exit(-2)
+
+        # main_event_loop.alarm(0, lambda: self.exit_loop_finish_proceess("by CTRL+C... press CTRL+C again to exit"))
+
     def exit_on_enter(self,key):
+        
         if key in ("q", "Q"):
-            self.proc.send_signal(signal.SIGTERM)
+            self.exit_handler(0)
             raise urwid.ExitMainLoop()
```

### Comparing `cli_progress-1.9.0/cli_progress.egg-info/PKG-INFO` & `cli_progress-2.0.0/cli_progress.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: cli_progress
-Version: 1.9.0
+Version: 2.0.0
 Summary: Awesome cli_progress created by hiddify
 Home-page: https://github.com/hiddify/cli_progress/
 Author: hiddify
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: urwid==2.6.10
-Requires-Dist: Twisted==24.3.0
-Requires-Dist: pyOpenSSL==24.1.0
-Requires-Dist: service-identity==24.1.0
 Requires-Dist: argparse==1.4.0
+Requires-Dist: asyncio
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: isort; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
```

### Comparing `cli_progress-1.9.0/cli_progress.egg-info/SOURCES.txt` & `cli_progress-2.0.0/cli_progress.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cli_progress-1.9.0/setup.py` & `cli_progress-2.0.0/setup.py`

 * *Files identical despite different names*

