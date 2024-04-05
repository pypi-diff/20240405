# Comparing `tmp/42-taskmaster-1.0.0.tar.gz` & `tmp/42-taskmaster-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "42-taskmaster-1.0.0.tar", last modified: Wed Apr  3 14:45:00 2024, max compression
+gzip compressed data, was "42-taskmaster-1.0.1.tar", last modified: Fri Apr  5 08:54:22 2024, max compression
```

## Comparing `42-taskmaster-1.0.0.tar` & `42-taskmaster-1.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:45:00.635348 42-taskmaster-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:45:00.635348 42-taskmaster-1.0.0/42_taskmaster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-03 14:45:00.000000 42-taskmaster-1.0.0/42_taskmaster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-03 14:45:00.000000 42-taskmaster-1.0.0/42_taskmaster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:45:00.000000 42-taskmaster-1.0.0/42_taskmaster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 14:45:00.000000 42-taskmaster-1.0.0/42_taskmaster.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 14:45:00.000000 42-taskmaster-1.0.0/42_taskmaster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 14:45:00.000000 42-taskmaster-1.0.0/42_taskmaster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-03 14:45:00.635348 42-taskmaster-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-03 14:44:53.000000 42-taskmaster-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-03 14:44:53.000000 42-taskmaster-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 14:44:53.000000 42-taskmaster-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:45:00.635348 42-taskmaster-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:45:00.631348 42-taskmaster-1.0.0/taskmaster/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:44:53.000000 42-taskmaster-1.0.0/taskmaster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:45:00.631348 42-taskmaster-1.0.0/taskmaster/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:44:53.000000 42-taskmaster-1.0.0/taskmaster/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7727 2024-04-03 14:44:53.000000 42-taskmaster-1.0.0/taskmaster/gui/_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-03 14:44:53.000000 42-taskmaster-1.0.0/taskmaster/gui/_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-04-03 14:44:53.000000 42-taskmaster-1.0.0/taskmaster/gui/_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     8944 2024-04-03 14:44:53.000000 42-taskmaster-1.0.0/taskmaster/gui/_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-03 14:44:53.000000 42-taskmaster-1.0.0/taskmaster/gui/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-03 14:44:53.000000 42-taskmaster-1.0.0/taskmaster/gui/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-03 14:44:53.000000 42-taskmaster-1.0.0/taskmaster/gui/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    28363 2024-04-03 14:44:53.000000 42-taskmaster-1.0.0/taskmaster/service.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3641 2024-04-03 14:44:53.000000 42-taskmaster-1.0.0/taskmaster/taskmaster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:45:00.635348 42-taskmaster-1.0.0/taskmaster/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:44:53.000000 42-taskmaster-1.0.0/taskmaster/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7963 2024-04-03 14:44:53.000000 42-taskmaster-1.0.0/taskmaster/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-03 14:44:53.000000 42-taskmaster-1.0.0/taskmaster/utils/email.py
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-03 14:44:53.000000 42-taskmaster-1.0.0/taskmaster/utils/log_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-03 14:44:53.000000 42-taskmaster-1.0.0/taskmaster/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:45:00.635348 42-taskmaster-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-04-03 14:44:53.000000 42-taskmaster-1.0.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-03 14:44:53.000000 42-taskmaster-1.0.0/tests/test_log_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    19039 2024-04-03 14:44:53.000000 42-taskmaster-1.0.0/tests/test_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    11786 2024-04-03 14:44:53.000000 42-taskmaster-1.0.0/tests/test_service_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9201 2024-04-03 14:44:53.000000 42-taskmaster-1.0.0/tests/test_subprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:54:22.881981 42-taskmaster-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:54:22.881981 42-taskmaster-1.0.1/42_taskmaster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-05 08:54:22.000000 42-taskmaster-1.0.1/42_taskmaster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-05 08:54:22.000000 42-taskmaster-1.0.1/42_taskmaster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 08:54:22.000000 42-taskmaster-1.0.1/42_taskmaster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 08:54:22.000000 42-taskmaster-1.0.1/42_taskmaster.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 08:54:22.000000 42-taskmaster-1.0.1/42_taskmaster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 08:54:22.000000 42-taskmaster-1.0.1/42_taskmaster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-05 08:54:22.881981 42-taskmaster-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 08:54:22.881981 42-taskmaster-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:54:22.877982 42-taskmaster-1.0.1/taskmaster/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:54:22.881981 42-taskmaster-1.0.1/taskmaster/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7727 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/gui/_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/gui/_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/gui/_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8944 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/gui/_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/gui/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/gui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/gui/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28363 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/service.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3712 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/taskmaster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:54:22.881981 42-taskmaster-1.0.1/taskmaster/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7963 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/utils/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/utils/log_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:54:22.881981 42-taskmaster-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/tests/test_log_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19039 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/tests/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11786 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/tests/test_service_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9201 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/tests/test_subprocess.py
```

### Comparing `42-taskmaster-1.0.0/42_taskmaster.egg-info/PKG-INFO` & `42-taskmaster-1.0.1/42_taskmaster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 42-taskmaster
-Version: 1.0.0
+Version: 1.0.1
 Summary: A process manager project for 42
 Author-email: Timothee Lafay <tlafay@student.42lyon.fr>, Theo Nard <tnard@student.42lyon.fr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: 42-taskmaster Version: 1.0.0 Summary: A process
+Metadata-Version: 2.1 Name: 42-taskmaster Version: 1.0.1 Summary: A process
 manager project for 42 Author-email: Timothee Lafay
 student.42lyon.fr>, Theo Nard
 student.42lyon.fr> Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.11 Description-Content-Type: text/markdown
 Requires-Dist: Cerberus==1.3.5 Requires-Dist: PyYAML==6.0.1
                                     _[_L_o_g_o_]
```

### Comparing `42-taskmaster-1.0.0/42_taskmaster.egg-info/SOURCES.txt` & `42-taskmaster-1.0.1/42_taskmaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.0/PKG-INFO` & `42-taskmaster-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 42-taskmaster
-Version: 1.0.0
+Version: 1.0.1
 Summary: A process manager project for 42
 Author-email: Timothee Lafay <tlafay@student.42lyon.fr>, Theo Nard <tnard@student.42lyon.fr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: 42-taskmaster Version: 1.0.0 Summary: A process
+Metadata-Version: 2.1 Name: 42-taskmaster Version: 1.0.1 Summary: A process
 manager project for 42 Author-email: Timothee Lafay
 student.42lyon.fr>, Theo Nard
 student.42lyon.fr> Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.11 Description-Content-Type: text/markdown
 Requires-Dist: Cerberus==1.3.5 Requires-Dist: PyYAML==6.0.1
                                     _[_L_o_g_o_]
```

### Comparing `42-taskmaster-1.0.0/README.md` & `42-taskmaster-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.0/pyproject.toml` & `42-taskmaster-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "42-taskmaster"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     { name = "Timothee Lafay", email = "tlafay@student.42lyon.fr" },
     { name = "Theo Nard", email = "tnard@student.42lyon.fr" },
 ]
 description = "A process manager project for 42"
 requires-python = ">=3.11"
 readme = "README.md"
```

### Comparing `42-taskmaster-1.0.0/taskmaster/gui/_configuration.py` & `42-taskmaster-1.0.1/taskmaster/gui/_configuration.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.0/taskmaster/gui/_default.py` & `42-taskmaster-1.0.1/taskmaster/gui/_default.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,21 +52,13 @@
         elif key == 10:  # Enter
             # Open the selected page
             if self.win_data["default"]["selected"] == "services":
                 self.services()
             elif self.win_data["default"]["selected"] == "config":
                 self.configuration()
             elif self.win_data["default"]["selected"] == "reload":
-                try:
-                    config = Config(self.config.path)
-                    self.config = config
-                    # ici reload service handler
-                    self.service_handler.config = dict({"services": config.services})
-                    self.configuration_success()
-                    self.default()
-                except Exception as e:
-                    self.configuration_error(e)
+                self.need_reload = True
             return True
         self.default()
     except curses.error as e:
         logger.error(f"[Default] Failed to navigate. {e}")
         return 0
```

### Comparing `42-taskmaster-1.0.0/taskmaster/gui/_log.py` & `42-taskmaster-1.0.1/taskmaster/gui/_log.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.0/taskmaster/gui/_services.py` & `42-taskmaster-1.0.1/taskmaster/gui/_services.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.0/taskmaster/gui/_utils.py` & `42-taskmaster-1.0.1/taskmaster/gui/_utils.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.0/taskmaster/gui/gui.py` & `42-taskmaster-1.0.1/taskmaster/gui/gui.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         # Initialize the screen
 
         logger.debug("Initializing screen.")
         try:
             self.stdscr = curses.initscr()
             self.stdscr.keypad(True)
             self.stdscr.clear()
+            self.need_reload = False
             curses.noecho()
             curses.cbreak()
             curses.curs_set(0)
             self.height, self.width = self.stdscr.getmaxyx()
             logger.debug(f"Screen size: {self.height}x{self.width}")
             while self.height < 20 or self.width < 90:
                 self.screen_too_small()
```

### Comparing `42-taskmaster-1.0.0/taskmaster/gui/table.py` & `42-taskmaster-1.0.1/taskmaster/gui/table.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.0/taskmaster/service.py` & `42-taskmaster-1.0.1/taskmaster/service.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.0/taskmaster/taskmaster.py` & `42-taskmaster-1.0.1/taskmaster/taskmaster.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,16 +61,17 @@
                 continue
             elif interface.services_nav(key) == -1:
                 break
             elif interface.config_nav(key) == -1:
                 break
             elif interface.log_nav(key) == -1:
                 break
-            if need_reload:
+            if need_reload or interface.need_reload:
                 need_reload = False
+                interface.need_reload = False
                 config = Config(config.path)
                 if config.email:
                     email = Email(config)
                 interface.service_handler.config = dict({"services": config.services})
                 asyncio.create_task(interface.service_handler.reload(email=email))
                 interface.config = config
                 interface.configuration_success()
```

### Comparing `42-taskmaster-1.0.0/taskmaster/utils/config.py` & `42-taskmaster-1.0.1/taskmaster/utils/config.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.0/taskmaster/utils/email.py` & `42-taskmaster-1.0.1/taskmaster/utils/email.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.0/taskmaster/utils/log_reader.py` & `42-taskmaster-1.0.1/taskmaster/utils/log_reader.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.0/taskmaster/utils/logger.py` & `42-taskmaster-1.0.1/taskmaster/utils/logger.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.0/tests/test_config.py` & `42-taskmaster-1.0.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.0/tests/test_log_reader.py` & `42-taskmaster-1.0.1/tests/test_log_reader.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.0/tests/test_service.py` & `42-taskmaster-1.0.1/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.0/tests/test_service_handler.py` & `42-taskmaster-1.0.1/tests/test_service_handler.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.0/tests/test_subprocess.py` & `42-taskmaster-1.0.1/tests/test_subprocess.py`

 * *Files identical despite different names*

