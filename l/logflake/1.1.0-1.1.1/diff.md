# Comparing `tmp/logflake-1.1.0.tar.gz` & `tmp/logflake-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logflake-1.1.0.tar", last modified: Fri Apr  5 13:50:29 2024, max compression
+gzip compressed data, was "logflake-1.1.1.tar", last modified: Fri Apr  5 15:23:49 2024, max compression
```

## Comparing `logflake-1.1.0.tar` & `logflake-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dedo1911   (501) staff       (20)        0 2024-04-05 13:50:29.054196 logflake-1.1.0/
--rw-r--r--   0 dedo1911   (501) staff       (20)     1743 2024-04-05 13:50:29.053998 logflake-1.1.0/PKG-INFO
--rw-r--r--   0 dedo1911   (501) staff       (20)     1359 2024-04-05 13:48:02.000000 logflake-1.1.0/README.md
-drwxr-xr-x   0 dedo1911   (501) staff       (20)        0 2024-04-05 13:50:29.053041 logflake-1.1.0/logflake/
--rw-r--r--   0 dedo1911   (501) staff       (20)        0 2024-02-05 16:12:08.000000 logflake-1.1.0/logflake/__init__.py
--rw-r--r--   0 dedo1911   (501) staff       (20)     5879 2024-04-05 13:44:47.000000 logflake-1.1.0/logflake/logflake.py
-drwxr-xr-x   0 dedo1911   (501) staff       (20)        0 2024-04-05 13:50:29.053784 logflake-1.1.0/logflake.egg-info/
--rw-r--r--   0 dedo1911   (501) staff       (20)     1743 2024-04-05 13:50:29.000000 logflake-1.1.0/logflake.egg-info/PKG-INFO
--rw-r--r--   0 dedo1911   (501) staff       (20)      225 2024-04-05 13:50:29.000000 logflake-1.1.0/logflake.egg-info/SOURCES.txt
--rw-r--r--   0 dedo1911   (501) staff       (20)        1 2024-04-05 13:50:29.000000 logflake-1.1.0/logflake.egg-info/dependency_links.txt
--rw-r--r--   0 dedo1911   (501) staff       (20)       26 2024-04-05 13:50:29.000000 logflake-1.1.0/logflake.egg-info/requires.txt
--rw-r--r--   0 dedo1911   (501) staff       (20)        9 2024-04-05 13:50:29.000000 logflake-1.1.0/logflake.egg-info/top_level.txt
--rw-r--r--   0 dedo1911   (501) staff       (20)      500 2024-04-05 13:45:27.000000 logflake-1.1.0/pyproject.toml
--rw-r--r--   0 dedo1911   (501) staff       (20)       38 2024-04-05 13:50:29.054230 logflake-1.1.0/setup.cfg
+drwxr-xr-x   0 dedo1911   (501) staff       (20)        0 2024-04-05 15:23:49.206165 logflake-1.1.1/
+-rw-r--r--   0 dedo1911   (501) staff       (20)     2422 2024-04-05 15:23:49.205986 logflake-1.1.1/PKG-INFO
+-rw-r--r--   0 dedo1911   (501) staff       (20)     2038 2024-04-05 15:21:57.000000 logflake-1.1.1/README.md
+drwxr-xr-x   0 dedo1911   (501) staff       (20)        0 2024-04-05 15:23:49.205075 logflake-1.1.1/logflake/
+-rw-r--r--   0 dedo1911   (501) staff       (20)        0 2024-02-05 16:12:08.000000 logflake-1.1.1/logflake/__init__.py
+-rw-r--r--   0 dedo1911   (501) staff       (20)     6260 2024-04-05 15:23:32.000000 logflake-1.1.1/logflake/logflake.py
+drwxr-xr-x   0 dedo1911   (501) staff       (20)        0 2024-04-05 15:23:49.205768 logflake-1.1.1/logflake.egg-info/
+-rw-r--r--   0 dedo1911   (501) staff       (20)     2422 2024-04-05 15:23:49.000000 logflake-1.1.1/logflake.egg-info/PKG-INFO
+-rw-r--r--   0 dedo1911   (501) staff       (20)      225 2024-04-05 15:23:49.000000 logflake-1.1.1/logflake.egg-info/SOURCES.txt
+-rw-r--r--   0 dedo1911   (501) staff       (20)        1 2024-04-05 15:23:49.000000 logflake-1.1.1/logflake.egg-info/dependency_links.txt
+-rw-r--r--   0 dedo1911   (501) staff       (20)       26 2024-04-05 15:23:49.000000 logflake-1.1.1/logflake.egg-info/requires.txt
+-rw-r--r--   0 dedo1911   (501) staff       (20)        9 2024-04-05 15:23:49.000000 logflake-1.1.1/logflake.egg-info/top_level.txt
+-rw-r--r--   0 dedo1911   (501) staff       (20)      500 2024-04-05 14:26:58.000000 logflake-1.1.1/pyproject.toml
+-rw-r--r--   0 dedo1911   (501) staff       (20)       38 2024-04-05 15:23:49.206201 logflake-1.1.1/setup.cfg
```

### Comparing `logflake-1.1.0/logflake/logflake.py` & `logflake-1.1.1/logflake/logflake.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+import logging
 import os
 import threading
 from logging import Handler
 from json import dumps
 from enum import Enum
 from queue import Queue
 from sys import exc_info
@@ -64,38 +64,41 @@
 
     def stop(self):
         duration = time() - self.start_time
         self.instance.send_performance(self.label, duration)
 
 
 class LogFlake:
-    def __init__(self, app_id, log_flake_server=Servers.PRODUCTION.value):
+    def __init__(self, app_id, log_flake_server=Servers.PRODUCTION.value, show_greeting=True):
         if not app_id:
             raise LogFlakeException("appId missing")
 
         self.server = log_flake_server.rstrip('/')
         self._hostname = node()
         self.app_id = app_id
         self._logs_queue = Queue()
         self._process_logs = threading.Event()
         self.failed_post_retries = 3
         self.post_timeout_seconds = 3
         self.is_shutting_down = False
+        self.show_greeting = show_greeting
         self._logs_processor_thread = threading.Thread(target=self._logs_processor)
         self._logs_processor_thread.start()
 
     def __del__(self):
         self.shutdown()
 
     def shutdown(self):
         self.is_shutting_down = True
         self._logs_processor_thread.join()
 
     def _logs_processor(self):
-        self.send_log(level=LogLevels.DEBUG, correlation=None, content=f"LogFlake started on {self.get_hostname()}")
+        if self.show_greeting:
+            self.send_log(level=LogLevels.DEBUG, correlation=None, content=f"LogFlake started on {self.get_hostname()}")
+
         self._process_logs.wait()
 
         while not self._logs_queue.empty():
             log = self._logs_queue.get()
             log.retries += 1
 
             success = self._post(log.queue_name, log.json_string)
@@ -171,16 +174,18 @@
         dumps(x)
         return True
     except:
         return False
 
 
 class LogFlakeHandler(Handler):
-    def __init(self, app_id, log_flake_server=Servers.PRODUCTION.value) -> None:
-        self.log_flake = LogFlake(app_id, log_flake_server)
+    def __init__(self, app_id, level=logging.INFO, server=Servers.PRODUCTION.value) -> None:
+        logging.Handler.__init__(self)
+        self.setLevel(level)
+        self.log_flake = LogFlake(app_id, server, show_greeting=False)
         self.log_level_mapping = {
             'DEBUG': LogLevels.DEBUG,
             'INFO': LogLevels.INFO,
             'WARNING': LogLevels.WARN,
             'ERROR': LogLevels.ERROR,
             'CRITICAL': LogLevels.FATAL,
             'EXCEPTION': LogLevels.EXCEPTION
@@ -189,17 +194,25 @@
     def emit(self, record):
         try:
             self.format(record)
 
             if record.exc_info:
                 self.log_flake.send_exception()
 
+            params = record.args
+            if is_jsonable(params):
+                params_json = {
+                    "args": dumps(params)
+                }
+            else:
+                params_json = None
+
             self.log_flake.send_log(
                 level=self.log_level_mapping[record.levelname],
                 content=self.format(record),
                 correlation=None,
-                params=record.args if is_jsonable(record.args) else None
+                params=params_json
             )
 
         except:
             self.log_flake.send_exception()
             self.handleError(record)
```

