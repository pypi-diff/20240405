# Comparing `tmp/dip-coater-0.1.0.tar.gz` & `tmp/dip-coater-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dip-coater-0.1.0.tar", last modified: Fri Apr  5 09:41:17 2024, max compression
+gzip compressed data, was "dip-coater-0.2.0.tar", last modified: Fri Apr  5 10:26:20 2024, max compression
```

## Comparing `dip-coater-0.1.0.tar` & `dip-coater-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 09:41:17.469347 dip-coater-0.1.0/
--rw-r--r--   0 rik      (459800007) staff       (20)       89 2024-04-05 09:39:07.000000 dip-coater-0.1.0/MANIFEST.in
--rw-r--r--   0 rik      (459800007) staff       (20)      233 2024-04-05 09:41:17.469165 dip-coater-0.1.0/PKG-INFO
--rw-r--r--   0 rik      (459800007) staff       (20)      440 2024-04-05 09:41:13.000000 dip-coater-0.1.0/pyproject.toml
--rw-r--r--   0 rik      (459800007) staff       (20)       38 2024-04-05 09:41:17.469398 dip-coater-0.1.0/setup.cfg
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 09:41:17.467395 dip-coater-0.1.0/src/
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 09:41:17.468944 dip-coater-0.1.0/src/dip_coater.egg-info/
--rw-r--r--   0 rik      (459800007) staff       (20)      233 2024-04-05 09:41:17.000000 dip-coater-0.1.0/src/dip_coater.egg-info/PKG-INFO
--rw-r--r--   0 rik      (459800007) staff       (20)      252 2024-04-05 09:41:17.000000 dip-coater-0.1.0/src/dip_coater.egg-info/SOURCES.txt
--rw-r--r--   0 rik      (459800007) staff       (20)        1 2024-04-05 09:41:17.000000 dip-coater-0.1.0/src/dip_coater.egg-info/dependency_links.txt
--rw-r--r--   0 rik      (459800007) staff       (20)       41 2024-04-05 09:41:17.000000 dip-coater-0.1.0/src/dip_coater.egg-info/requires.txt
--rw-r--r--   0 rik      (459800007) staff       (20)        4 2024-04-05 09:41:17.000000 dip-coater-0.1.0/src/dip_coater.egg-info/top_level.txt
--rw-r--r--   0 rik      (459800007) staff       (20)     4293 2024-04-04 11:06:11.000000 dip-coater-0.1.0/src/motor.py
--rw-r--r--   0 rik      (459800007) staff       (20)     8586 2024-04-05 09:16:29.000000 dip-coater-0.1.0/src/tui.py
--rw-r--r--   0 rik      (459800007) staff       (20)     1443 2024-04-05 09:18:29.000000 dip-coater-0.1.0/src/tui.tcss
+drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 10:26:20.733638 dip-coater-0.2.0/
+-rw-r--r--   0 rik      (459800007) staff       (20)       89 2024-04-05 09:39:07.000000 dip-coater-0.2.0/MANIFEST.in
+-rw-r--r--   0 rik      (459800007) staff       (20)      269 2024-04-05 10:26:20.733451 dip-coater-0.2.0/PKG-INFO
+-rw-r--r--   0 rik      (459800007) staff       (20)      531 2024-04-05 10:26:14.000000 dip-coater-0.2.0/pyproject.toml
+-rw-r--r--   0 rik      (459800007) staff       (20)       38 2024-04-05 10:26:20.733693 dip-coater-0.2.0/setup.cfg
+drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 10:26:20.731168 dip-coater-0.2.0/src/
+drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 10:26:20.731934 dip-coater-0.2.0/src/dip_coater/
+-rw-r--r--   0 rik      (459800007) staff       (20)        0 2024-04-05 10:07:42.000000 dip-coater-0.2.0/src/dip_coater/__init__.py
+-rw-r--r--   0 rik      (459800007) staff       (20)     4293 2024-04-04 11:06:11.000000 dip-coater-0.2.0/src/dip_coater/motor.py
+-rw-r--r--   0 rik      (459800007) staff       (20)     8631 2024-04-05 10:10:36.000000 dip-coater-0.2.0/src/dip_coater/tui.py
+drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 10:26:20.733169 dip-coater-0.2.0/src/dip_coater.egg-info/
+-rw-r--r--   0 rik      (459800007) staff       (20)      269 2024-04-05 10:26:20.000000 dip-coater-0.2.0/src/dip_coater.egg-info/PKG-INFO
+-rw-r--r--   0 rik      (459800007) staff       (20)      329 2024-04-05 10:26:20.000000 dip-coater-0.2.0/src/dip_coater.egg-info/SOURCES.txt
+-rw-r--r--   0 rik      (459800007) staff       (20)        1 2024-04-05 10:26:20.000000 dip-coater-0.2.0/src/dip_coater.egg-info/dependency_links.txt
+-rw-r--r--   0 rik      (459800007) staff       (20)       51 2024-04-05 10:26:20.000000 dip-coater-0.2.0/src/dip_coater.egg-info/entry_points.txt
+-rw-r--r--   0 rik      (459800007) staff       (20)       48 2024-04-05 10:26:20.000000 dip-coater-0.2.0/src/dip_coater.egg-info/requires.txt
+-rw-r--r--   0 rik      (459800007) staff       (20)       15 2024-04-05 10:26:20.000000 dip-coater-0.2.0/src/dip_coater.egg-info/top_level.txt
```

### Comparing `dip-coater-0.1.0/src/motor.py` & `dip-coater-0.2.0/src/dip_coater/motor.py`

 * *Files identical despite different names*

### Comparing `dip-coater-0.1.0/src/tui.py` & `dip-coater-0.2.0/src/dip_coater/tui.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from textual.widgets import Header
 from textual.widgets import Label
 from textual.widgets import RadioButton
 from textual.widgets import RadioSet
 from textual.widgets import RichLog
 from textual.widgets import Static
 
-import motor
+import dip_coater.motor as motor
 
 STEP_MODE_WRITE_TO_LOG = False
 
 DEFAULT_SPEED_STEP = 10
 MAX_SPEED = 100
 MIN_SPEED = 1
 
@@ -253,10 +253,14 @@
 
     def action_request_quit(self) -> None:
         motor.disable_motor()
         motor.GPIO.cleanup()
         self.app.exit()
 
 
-if __name__ == '__main__':
+def main():
     app = DipCoaterApp()
     app.run()
+
+
+if __name__ == '__main__':
+    main()
```

