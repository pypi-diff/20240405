# Comparing `tmp/pynobo-1.8.0.tar.gz` & `tmp/pynobo-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynobo-1.8.0.tar", last modified: Wed Mar 27 19:43:11 2024, max compression
+gzip compressed data, was "pynobo-1.8.1.tar", last modified: Fri Apr  5 19:39:46 2024, max compression
```

## Comparing `pynobo-1.8.0.tar` & `pynobo-1.8.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:43:11.769453 pynobo-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-03-27 19:43:07.000000 pynobo-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-27 19:43:07.000000 pynobo-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-03-27 19:43:11.769453 pynobo-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-03-27 19:43:07.000000 pynobo-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:43:11.769453 pynobo-1.8.0/pynobo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-03-27 19:43:11.000000 pynobo-1.8.0/pynobo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-27 19:43:11.000000 pynobo-1.8.0/pynobo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 19:43:11.000000 pynobo-1.8.0/pynobo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-27 19:43:11.000000 pynobo-1.8.0/pynobo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    53879 2024-03-27 19:43:07.000000 pynobo-1.8.0/pynobo.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-27 19:43:11.769453 pynobo-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-03-27 19:43:07.000000 pynobo-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:39:46.655311 pynobo-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-05 19:39:39.000000 pynobo-1.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-05 19:39:39.000000 pynobo-1.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-04-05 19:39:46.655311 pynobo-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-05 19:39:39.000000 pynobo-1.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:39:46.655311 pynobo-1.8.1/pynobo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-04-05 19:39:46.000000 pynobo-1.8.1/pynobo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-05 19:39:46.000000 pynobo-1.8.1/pynobo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:39:46.000000 pynobo-1.8.1/pynobo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 19:39:46.000000 pynobo-1.8.1/pynobo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    53996 2024-04-05 19:39:39.000000 pynobo-1.8.1/pynobo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-05 19:39:46.655311 pynobo-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-04-05 19:39:39.000000 pynobo-1.8.1/setup.py
```

### Comparing `pynobo-1.8.0/LICENSE` & `pynobo-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynobo-1.8.0/PKG-INFO` & `pynobo-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynobo
-Version: 1.8.0
+Version: 1.8.1
 Summary: Nobø Hub / Nobø Energy Control TCP/IP Interface
 Home-page: https://github.com/echoromeo/pynobo
 Author: echoromeo, capelevy, oyvindwe
 License: GPLv3+
 Project-URL: Bug Reports, https://github.com/echoromeo/pynobo/issues
 Project-URL: Source, https://github.com/echoromeo/pynobo/blob/master/pynobo.py
 Keywords: hvac nobø heating automation
```

### Comparing `pynobo-1.8.0/README.md` & `pynobo-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `pynobo-1.8.0/pynobo.egg-info/PKG-INFO` & `pynobo-1.8.1/pynobo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynobo
-Version: 1.8.0
+Version: 1.8.1
 Summary: Nobø Hub / Nobø Energy Control TCP/IP Interface
 Home-page: https://github.com/echoromeo/pynobo
 Author: echoromeo, capelevy, oyvindwe
 License: GPLv3+
 Project-URL: Bug Reports, https://github.com/echoromeo/pynobo/issues
 Project-URL: Source, https://github.com/echoromeo/pynobo/blob/master/pynobo.py
 Keywords: hvac nobø heating automation
```

### Comparing `pynobo-1.8.0/pynobo.py` & `pynobo-1.8.1/pynobo.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,32 +159,30 @@
 
         DICT_OVERRIDE_MODE_TO_NAME = {OVERRIDE_MODE_NORMAL : NAME_NORMAL, OVERRIDE_MODE_COMFORT : NAME_COMFORT, OVERRIDE_MODE_ECO : NAME_ECO, OVERRIDE_MODE_AWAY : NAME_AWAY}
         DICT_WEEK_PROFILE_STATUS_TO_NAME = {WEEK_PROFILE_STATE_ECO : NAME_ECO, WEEK_PROFILE_STATE_COMFORT : NAME_COMFORT, WEEK_PROFILE_STATE_AWAY : NAME_AWAY, WEEK_PROFILE_STATE_OFF : NAME_OFF}
         DICT_NAME_TO_OVERRIDE_MODE = {NAME_NORMAL : OVERRIDE_MODE_NORMAL, NAME_COMFORT : OVERRIDE_MODE_COMFORT, NAME_ECO : OVERRIDE_MODE_ECO, NAME_AWAY : OVERRIDE_MODE_AWAY}
         DICT_NAME_TO_WEEK_PROFILE_STATUS = {NAME_ECO : WEEK_PROFILE_STATE_ECO, NAME_COMFORT : WEEK_PROFILE_STATE_COMFORT, NAME_AWAY : WEEK_PROFILE_STATE_AWAY, NAME_OFF : WEEK_PROFILE_STATE_OFF}
 
         def is_valid_datetime(timestamp: str):
-            try:
-                datetime.datetime.strptime(timestamp, '%Y%m%d%H%M')
-            except ValueError:
+            if len(timestamp) != 12:
+                # Leading zero is optional for some of the fields below, but we require it.
                 return False
-            return True
-
-        def is_valid_time(time_of_day: str):
             try:
-                datetime.datetime.strptime(time_of_day, '%H%M')
+                datetime.datetime.strptime(timestamp, '%Y%m%d%H%M')
             except ValueError:
                 return False
             return True
 
         def time_is_quarter(minutes: str):
             return int(minutes) % 15 == 0
 
-        def validate_temperature(temperature: str):
-            if not temperature.isdigit():
+        def validate_temperature(temperature: Union[int, str]):
+            if type(temperature) not in (int, str):
+                raise TypeError('Temperature must be integer or string')
+            if isinstance(temperature, str) and not temperature.isdigit():
                 raise ValueError(f'Temperature "{temperature}" must be digits')
             temperature_int = int(temperature)
             if temperature_int < 7:
                 raise ValueError(f'Min temperature is 7°C')
             if temperature_int > 30:
                 raise ValueError(f'Max temperature is 30°C')
```

### Comparing `pynobo-1.8.0/setup.py` & `pynobo-1.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.8.0',
+    version='1.8.1',
     description='Nobø Hub / Nobø Energy Control TCP/IP Interface',
 
     license='GPLv3+',
     
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

