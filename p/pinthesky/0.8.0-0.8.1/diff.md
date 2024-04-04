# Comparing `tmp/pinthesky-0.8.0.tar.gz` & `tmp/pinthesky-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinthesky-0.8.0.tar", last modified: Sun Mar 17 21:38:31 2024, max compression
+gzip compressed data, was "pinthesky-0.8.1.tar", last modified: Thu Apr  4 23:13:12 2024, max compression
```

## Comparing `pinthesky-0.8.0.tar` & `pinthesky-0.8.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:38:31.800564 pinthesky-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-17 21:38:27.000000 pinthesky-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-03-17 21:38:31.800564 pinthesky-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-03-17 21:38:27.000000 pinthesky-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:38:31.796564 pinthesky-0.8.0/pinthesky/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-17 21:38:27.000000 pinthesky-0.8.0/pinthesky/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-03-17 21:38:27.000000 pinthesky-0.8.0/pinthesky/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9345 2024-03-17 21:38:27.000000 pinthesky-0.8.0/pinthesky/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)    11676 2024-03-17 21:38:27.000000 pinthesky-0.8.0/pinthesky/cloudwatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-17 21:38:27.000000 pinthesky-0.8.0/pinthesky/combiner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-03-17 21:38:27.000000 pinthesky-0.8.0/pinthesky/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-03-17 21:38:27.000000 pinthesky-0.8.0/pinthesky/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-03-17 21:38:27.000000 pinthesky-0.8.0/pinthesky/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-03-17 21:38:27.000000 pinthesky-0.8.0/pinthesky/health.py
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-03-17 21:38:27.000000 pinthesky-0.8.0/pinthesky/input.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-17 21:38:27.000000 pinthesky-0.8.0/pinthesky/motion_detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-17 21:38:27.000000 pinthesky-0.8.0/pinthesky/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-03-17 21:38:27.000000 pinthesky-0.8.0/pinthesky/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-03-17 21:38:27.000000 pinthesky-0.8.0/pinthesky/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:38:31.800564 pinthesky-0.8.0/pinthesky.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-03-17 21:38:31.000000 pinthesky-0.8.0/pinthesky.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-17 21:38:31.000000 pinthesky-0.8.0/pinthesky.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 21:38:31.000000 pinthesky-0.8.0/pinthesky.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-17 21:38:31.000000 pinthesky-0.8.0/pinthesky.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-17 21:38:31.000000 pinthesky-0.8.0/pinthesky.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-17 21:38:31.000000 pinthesky-0.8.0/pinthesky.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-17 21:38:31.800564 pinthesky-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-03-17 21:38:27.000000 pinthesky-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:38:31.800564 pinthesky-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-03-17 21:38:27.000000 pinthesky-0.8.0/tests/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-03-17 21:38:27.000000 pinthesky-0.8.0/tests/test_cloudwatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-17 21:38:27.000000 pinthesky-0.8.0/tests/test_combiner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-03-17 21:38:27.000000 pinthesky-0.8.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-03-17 21:38:27.000000 pinthesky-0.8.0/tests/test_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-03-17 21:38:27.000000 pinthesky-0.8.0/tests/test_health.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-03-17 21:38:27.000000 pinthesky-0.8.0/tests/test_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-03-17 21:38:27.000000 pinthesky-0.8.0/tests/test_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-03-17 21:38:27.000000 pinthesky-0.8.0/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-03-17 21:38:27.000000 pinthesky-0.8.0/tests/test_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:13:12.372517 pinthesky-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 23:13:08.000000 pinthesky-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-04-04 23:13:12.372517 pinthesky-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-04 23:13:08.000000 pinthesky-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:13:12.368517 pinthesky-0.8.1/pinthesky/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9345 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11676 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/cloudwatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/combiner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/motion_detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-04 23:13:08.000000 pinthesky-0.8.1/pinthesky/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:13:12.368517 pinthesky-0.8.1/pinthesky.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-04-04 23:13:12.000000 pinthesky-0.8.1/pinthesky.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-04 23:13:12.000000 pinthesky-0.8.1/pinthesky.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 23:13:12.000000 pinthesky-0.8.1/pinthesky.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-04 23:13:12.000000 pinthesky-0.8.1/pinthesky.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-04 23:13:12.000000 pinthesky-0.8.1/pinthesky.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 23:13:12.000000 pinthesky-0.8.1/pinthesky.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-04 23:13:12.372517 pinthesky-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-04 23:13:08.000000 pinthesky-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:13:12.368517 pinthesky-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-04-04 23:13:08.000000 pinthesky-0.8.1/tests/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-04-04 23:13:08.000000 pinthesky-0.8.1/tests/test_cloudwatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-04 23:13:08.000000 pinthesky-0.8.1/tests/test_combiner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-04-04 23:13:08.000000 pinthesky-0.8.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-04 23:13:08.000000 pinthesky-0.8.1/tests/test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-04 23:13:08.000000 pinthesky-0.8.1/tests/test_health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-04 23:13:08.000000 pinthesky-0.8.1/tests/test_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-04 23:13:08.000000 pinthesky-0.8.1/tests/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-04 23:13:08.000000 pinthesky-0.8.1/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-04-04 23:13:08.000000 pinthesky-0.8.1/tests/test_upload.py
```

### Comparing `pinthesky-0.8.0/LICENSE` & `pinthesky-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.0/PKG-INFO` & `pinthesky-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinthesky
-Version: 0.8.0
+Version: 0.8.1
 Summary: Simple Pi In The Sky device Integration
 Home-page: https://github.com/philcali/pits-device
 Author: Philip Cali
 Author-email: philip.cali@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -182,15 +182,15 @@
 The `pitsctl` entry point can handle three targets:
 
 - `install`: Installs or updates software and agents for running the camera control
 - `remove`: Removes all configuration, cloud resources, software and agents
 - `view`: Inpects the installation on the device
 
 ```
-Usage: pitsctl - v0.8.0: Install or manage pinthesky software
+Usage: pitsctl - v0.8.1: Install or manage pinthesky software
   -h,--help:    Prints out this help message
   -m,--host:    Client machine connection details
   -t,--text:    Enable a no color, text only view of the application
   -r,--root:    Assume root permission for management
   -l,--level:   Changes the logging verbosity for pitsctl
   -v,--version: Prints the version and exists
 ```
```

### Comparing `pinthesky-0.8.0/README.md` & `pinthesky-0.8.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 The `pitsctl` entry point can handle three targets:
 
 - `install`: Installs or updates software and agents for running the camera control
 - `remove`: Removes all configuration, cloud resources, software and agents
 - `view`: Inpects the installation on the device
 
 ```
-Usage: pitsctl - v0.8.0: Install or manage pinthesky software
+Usage: pitsctl - v0.8.1: Install or manage pinthesky software
   -h,--help:    Prints out this help message
   -m,--host:    Client machine connection details
   -t,--text:    Enable a no color, text only view of the application
   -r,--root:    Assume root permission for management
   -l,--level:   Changes the logging verbosity for pitsctl
   -v,--version: Prints the version and exists
 ```
```

### Comparing `pinthesky-0.8.0/pinthesky/__init__.py` & `pinthesky-0.8.1/pinthesky/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-VERSION = "0.8.0"
+VERSION = "0.8.1"
 
 
 def set_stream_logger(name="pinthesky", level=logging.DEBUG, fmt_string=None):
     if fmt_string is None:
         fmt_string = "%(asctime)s %(name)s [%(levelname)s] %(message)s"
 
     logger = logging.getLogger(name)
```

### Comparing `pinthesky-0.8.0/pinthesky/__main__.py` & `pinthesky-0.8.1/pinthesky/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
     event_input_handler = input.InputHandler(events=event_thread)
     cloudwatch_manager = CloudWatchManager(
         session=auth_session,
         log_level=parsed.log_level,
         delineate_stream=not parsed.disable_cloudwatch_stream_split,
         threaded=parsed.cloudwatch_thread,
         enabled=parsed.cloudwatch,
-        log_group_name=parsed.cloudwatch_log_stream,
+        log_group_name=parsed.cloudwatch_log_group,
         namespace=parsed.cloudwatch_metric_namespace,
         event_type=parsed.cloudwatch_event_type)
     event_thread.on(camera_thread)
     event_thread.on(video_combiner)
     event_thread.on(video_uploader)
     event_thread.on(event_output)
     event_thread.on(event_input_handler)
```

### Comparing `pinthesky-0.8.0/pinthesky/camera.py` & `pinthesky-0.8.1/pinthesky/camera.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.0/pinthesky/cloudwatch.py` & `pinthesky-0.8.1/pinthesky/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.0/pinthesky/combiner.py` & `pinthesky-0.8.1/pinthesky/combiner.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.0/pinthesky/config.py` & `pinthesky-0.8.1/pinthesky/config.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.0/pinthesky/events.py` & `pinthesky-0.8.1/pinthesky/events.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.0/pinthesky/handler.py` & `pinthesky-0.8.1/pinthesky/handler.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.0/pinthesky/health.py` & `pinthesky-0.8.1/pinthesky/health.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.0/pinthesky/input.py` & `pinthesky-0.8.1/pinthesky/input.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.0/pinthesky/motion_detect.py` & `pinthesky-0.8.1/pinthesky/motion_detect.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.0/pinthesky/output.py` & `pinthesky-0.8.1/pinthesky/output.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.0/pinthesky/session.py` & `pinthesky-0.8.1/pinthesky/session.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.0/pinthesky/upload.py` & `pinthesky-0.8.1/pinthesky/upload.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.0/pinthesky.egg-info/PKG-INFO` & `pinthesky-0.8.1/pinthesky.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinthesky
-Version: 0.8.0
+Version: 0.8.1
 Summary: Simple Pi In The Sky device Integration
 Home-page: https://github.com/philcali/pits-device
 Author: Philip Cali
 Author-email: philip.cali@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -182,15 +182,15 @@
 The `pitsctl` entry point can handle three targets:
 
 - `install`: Installs or updates software and agents for running the camera control
 - `remove`: Removes all configuration, cloud resources, software and agents
 - `view`: Inpects the installation on the device
 
 ```
-Usage: pitsctl - v0.8.0: Install or manage pinthesky software
+Usage: pitsctl - v0.8.1: Install or manage pinthesky software
   -h,--help:    Prints out this help message
   -m,--host:    Client machine connection details
   -t,--text:    Enable a no color, text only view of the application
   -r,--root:    Assume root permission for management
   -l,--level:   Changes the logging verbosity for pitsctl
   -v,--version: Prints the version and exists
 ```
```

### Comparing `pinthesky-0.8.0/pinthesky.egg-info/SOURCES.txt` & `pinthesky-0.8.1/pinthesky.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.0/setup.cfg` & `pinthesky-0.8.1/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pinthesky
-version = 0.8.0
+version = 0.8.1
 author = philcali
 author_email = philcali@gmail.com
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/philcali/pits-device
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `pinthesky-0.8.0/setup.py` & `pinthesky-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="pinthesky",
-    version="0.8.0",
+    version="0.8.1",
     description="Simple Pi In The Sky device Integration",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Philip Cali",
     author_email="philip.cali@gmail.com",
     url="https://github.com/philcali/pits-device",
     license="Apache License 2.0",
```

### Comparing `pinthesky-0.8.0/tests/test_camera.py` & `pinthesky-0.8.1/tests/test_camera.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.0/tests/test_cloudwatch.py` & `pinthesky-0.8.1/tests/test_cloudwatch.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.0/tests/test_combiner.py` & `pinthesky-0.8.1/tests/test_combiner.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.0/tests/test_config.py` & `pinthesky-0.8.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.0/tests/test_handler.py` & `pinthesky-0.8.1/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.0/tests/test_health.py` & `pinthesky-0.8.1/tests/test_health.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.0/tests/test_input.py` & `pinthesky-0.8.1/tests/test_input.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.0/tests/test_output.py` & `pinthesky-0.8.1/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.0/tests/test_session.py` & `pinthesky-0.8.1/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `pinthesky-0.8.0/tests/test_upload.py` & `pinthesky-0.8.1/tests/test_upload.py`

 * *Files identical despite different names*

