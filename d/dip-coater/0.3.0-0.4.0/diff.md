# Comparing `tmp/dip-coater-0.3.0.tar.gz` & `tmp/dip-coater-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dip-coater-0.3.0.tar", last modified: Fri Apr  5 10:32:28 2024, max compression
+gzip compressed data, was "dip-coater-0.4.0.tar", last modified: Fri Apr  5 11:08:58 2024, max compression
```

## Comparing `dip-coater-0.3.0.tar` & `dip-coater-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 10:32:28.946227 dip-coater-0.3.0/
--rw-r--r--   0 rik      (459800007) staff       (20)      100 2024-04-05 10:30:51.000000 dip-coater-0.3.0/MANIFEST.in
--rw-r--r--   0 rik      (459800007) staff       (20)      269 2024-04-05 10:32:28.946051 dip-coater-0.3.0/PKG-INFO
--rw-r--r--   0 rik      (459800007) staff       (20)      531 2024-04-05 10:32:26.000000 dip-coater-0.3.0/pyproject.toml
--rw-r--r--   0 rik      (459800007) staff       (20)       38 2024-04-05 10:32:28.946276 dip-coater-0.3.0/setup.cfg
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 10:32:28.943965 dip-coater-0.3.0/src/
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 10:32:28.944787 dip-coater-0.3.0/src/dip_coater/
--rw-r--r--   0 rik      (459800007) staff       (20)        0 2024-04-05 10:07:42.000000 dip-coater-0.3.0/src/dip_coater/__init__.py
--rw-r--r--   0 rik      (459800007) staff       (20)     4293 2024-04-04 11:06:11.000000 dip-coater-0.3.0/src/dip_coater/motor.py
--rw-r--r--   0 rik      (459800007) staff       (20)     8631 2024-04-05 10:10:36.000000 dip-coater-0.3.0/src/dip_coater/tui.py
--rw-r--r--   0 rik      (459800007) staff       (20)     1443 2024-04-05 09:18:29.000000 dip-coater-0.3.0/src/dip_coater/tui.tcss
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 10:32:28.945793 dip-coater-0.3.0/src/dip_coater.egg-info/
--rw-r--r--   0 rik      (459800007) staff       (20)      269 2024-04-05 10:32:28.000000 dip-coater-0.3.0/src/dip_coater.egg-info/PKG-INFO
--rw-r--r--   0 rik      (459800007) staff       (20)      353 2024-04-05 10:32:28.000000 dip-coater-0.3.0/src/dip_coater.egg-info/SOURCES.txt
--rw-r--r--   0 rik      (459800007) staff       (20)        1 2024-04-05 10:32:28.000000 dip-coater-0.3.0/src/dip_coater.egg-info/dependency_links.txt
--rw-r--r--   0 rik      (459800007) staff       (20)       51 2024-04-05 10:32:28.000000 dip-coater-0.3.0/src/dip_coater.egg-info/entry_points.txt
--rw-r--r--   0 rik      (459800007) staff       (20)       48 2024-04-05 10:32:28.000000 dip-coater-0.3.0/src/dip_coater.egg-info/requires.txt
--rw-r--r--   0 rik      (459800007) staff       (20)       15 2024-04-05 10:32:28.000000 dip-coater-0.3.0/src/dip_coater.egg-info/top_level.txt
+drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 11:08:58.207521 dip-coater-0.4.0/
+-rw-r--r--   0 rik      (459800007) staff       (20)      100 2024-04-05 10:30:51.000000 dip-coater-0.4.0/MANIFEST.in
+-rw-r--r--   0 rik      (459800007) staff       (20)      269 2024-04-05 11:08:58.207287 dip-coater-0.4.0/PKG-INFO
+-rw-r--r--   0 rik      (459800007) staff       (20)      531 2024-04-05 11:08:53.000000 dip-coater-0.4.0/pyproject.toml
+-rw-r--r--   0 rik      (459800007) staff       (20)       38 2024-04-05 11:08:58.207589 dip-coater-0.4.0/setup.cfg
+drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 11:08:58.204728 dip-coater-0.4.0/src/
+drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 11:08:58.205312 dip-coater-0.4.0/src/MyRPi/
+drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 11:08:58.205432 dip-coater-0.4.0/src/MyRPi/GPIO/
+-rw-r--r--   0 rik      (459800007) staff       (20)       26 2024-04-05 10:42:43.000000 dip-coater-0.4.0/src/MyRPi/GPIO/__init__.py
+-rw-r--r--   0 rik      (459800007) staff       (20)      220 2024-04-04 11:42:49.000000 dip-coater-0.4.0/src/MyRPi/_GPIO.py
+-rw-r--r--   0 rik      (459800007) staff       (20)        0 2024-04-04 11:31:25.000000 dip-coater-0.4.0/src/MyRPi/__init__.py
+drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 11:08:58.206057 dip-coater-0.4.0/src/dip_coater/
+-rw-r--r--   0 rik      (459800007) staff       (20)        0 2024-04-05 10:07:42.000000 dip-coater-0.4.0/src/dip_coater/__init__.py
+-rw-r--r--   0 rik      (459800007) staff       (20)     4253 2024-04-05 10:58:01.000000 dip-coater-0.4.0/src/dip_coater/motor.py
+-rw-r--r--   0 rik      (459800007) staff       (20)     8836 2024-04-05 11:06:49.000000 dip-coater-0.4.0/src/dip_coater/tui.py
+-rw-r--r--   0 rik      (459800007) staff       (20)     1443 2024-04-05 09:18:29.000000 dip-coater-0.4.0/src/dip_coater/tui.tcss
+drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-05 11:08:58.206995 dip-coater-0.4.0/src/dip_coater.egg-info/
+-rw-r--r--   0 rik      (459800007) staff       (20)      269 2024-04-05 11:08:58.000000 dip-coater-0.4.0/src/dip_coater.egg-info/PKG-INFO
+-rw-r--r--   0 rik      (459800007) staff       (20)      421 2024-04-05 11:08:58.000000 dip-coater-0.4.0/src/dip_coater.egg-info/SOURCES.txt
+-rw-r--r--   0 rik      (459800007) staff       (20)        1 2024-04-05 11:08:58.000000 dip-coater-0.4.0/src/dip_coater.egg-info/dependency_links.txt
+-rw-r--r--   0 rik      (459800007) staff       (20)       51 2024-04-05 11:08:58.000000 dip-coater-0.4.0/src/dip_coater.egg-info/entry_points.txt
+-rw-r--r--   0 rik      (459800007) staff       (20)       48 2024-04-05 11:08:58.000000 dip-coater-0.4.0/src/dip_coater.egg-info/requires.txt
+-rw-r--r--   0 rik      (459800007) staff       (20)       17 2024-04-05 11:08:58.000000 dip-coater-0.4.0/src/dip_coater.egg-info/top_level.txt
```

### Comparing `dip-coater-0.3.0/pyproject.toml` & `dip-coater-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dip-coater"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
     {name="Rik Huygen", email="rik.huygen@kuleuven.be"}
 ]
 requires-python = ">=3.8, <4.0"
 
 dependencies = [
     "textual",
```

### Comparing `dip-coater-0.3.0/src/dip_coater/motor.py` & `dip-coater-0.4.0/src/dip_coater/motor.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,29 +34,29 @@
     step_distances = {
         "Full": 0.045,
         "Half": 0.0225,
         "1/4": 0.01125,
         "1/8": 0.005625,
         "1/16": 0.0028125
     }
-    
+
     distance_per_step = step_distances[step_mode]
     steps = int(distance_mm / distance_per_step)
     steps_per_second = speed_mm_s / distance_per_step
     delay = 1 / steps_per_second
     return steps, delay
 
 def init_motor_driver():
     global EN_pin, motor_driver
-    
+
     # Define the GPIO pins
     direction_pin = 7  # Direction (DIR) GPIO Pin
     step_pin = 21      # Step GPIO Pin
     EN_pin = 16        # enable pin (LOW to enable)
-    
+
     # Declare a instance of class pass GPIO pins numbers and the motor type
     motor_driver = RpiMotorLib.A4988Nema(direction_pin, step_pin, (-1,-1,-1), "DRV8825")
     GPIO.setup(EN_pin, GPIO.OUT) # set enable pin as output
 
 def enable_motor():
     """ Arm the motor"""
     GPIO.output(EN_pin, GPIO.LOW)
@@ -67,60 +67,60 @@
 
 def drive_motor(distance_mm, speed_mm_s, step_mode, clockwise=False, verbose=False):
     steps, step_delay = calculate_steps_and_delay(speed_mm_s, distance_mm, step_mode)
     motor_driver.motor_go(clockwise, # True=Clockwise, False=Counter-Clockwise
                      step_mode , # Step type (Full,Half,1/4,1/8,1/16,1/32)
                      steps, # number of steps
                      step_delay, # step delay [sec]
-                     verbose, # True = print verbose output 
+                     verbose, # True = print verbose output
                      0.05) # initial delay [sec]
 
 def move_up(distance_mm, speed_mm_s, step_mode, verbose=False):
     """
     Move up <distance> mm at <speed> mm/s using <step_mode> step mode..
     """
     drive_motor(distance_mm, speed_mm_s, step_mode, False, verbose)
 
 def move_down(distance_mm, speed_mm_s, step_mode, verbose=False):
     """
     Move down <distance> mm at <speed> mm/s using <step_mode> step mode.
     """
     drive_motor(distance_mm, speed_mm_s, step_mode, True, verbose)
-    
+
 if __name__ == "__main__":
     # Step mode ('Full', 'Half', '1/4', '1/8' or '1/16')
     # Lower step modes have a more smooth progression, but
     # we have a cheap knock-off driver which can't handle
     # too low modes.
     step_mode = "1/4"
     print("Adjust the driver's DIP switches according to step mode", step_mode, "!!!")
     print(get_DIP_positions_for_mode(step_mode))
     #input("Verify the DIP switches. Press 'Enter' to continue...")
-    
+
     # Movement speed in mm/s
     speed_up = 10
     speed_down = 10
 
     # Time to wait (in s) between going up and down
-    wait_time = 1   
+    wait_time = 1
 
     # Vertical travel distance in mm
     distance_up = 50
     distance_down = 50
-    
+
     # ======== INIT ========
     init_motor_driver()
 
     enable_motor()
 
     # ======== MOVE DOWN ========
     move_down(distance_down, speed_down, step_mode)
-    
+
     # ======== WAIT ========
     time.sleep(wait_time)
-    
+
     # ======== MOVE UP ========
     move_up(distance_up, speed_up, step_mode)
-    
+
     disable_motor()
 
     GPIO.cleanup() # clear GPIO allocations after run
```

### Comparing `dip-coater-0.3.0/src/dip_coater/tui.py` & `dip-coater-0.4.0/src/dip_coater/tui.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,26 @@
 from textual.widgets import Header
 from textual.widgets import Label
 from textual.widgets import RadioButton
 from textual.widgets import RadioSet
 from textual.widgets import RichLog
 from textual.widgets import Static
 
+# Mock the import of RPi when the package is not available
+try:
+    import RPi
+except ModuleNotFoundError:
+    import sys
+    from importlib import reload
+    import MyRPi
+    sys.modules["RPi"] = MyRPi
+
 import dip_coater.motor as motor
 
+
 STEP_MODE_WRITE_TO_LOG = False
 
 DEFAULT_SPEED_STEP = 10
 MAX_SPEED = 100
 MIN_SPEED = 1
 
 DEFAULT_DISTANCE = 50
```

### Comparing `dip-coater-0.3.0/src/dip_coater/tui.tcss` & `dip-coater-0.4.0/src/dip_coater/tui.tcss`

 * *Files identical despite different names*

