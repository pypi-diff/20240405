# Comparing `tmp/dirigera-1.0.9.tar.gz` & `tmp/dirigera-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dirigera-1.0.9.tar", last modified: Thu Feb 22 08:07:21 2024, max compression
+gzip compressed data, was "dirigera-1.1.0.tar", last modified: Fri Apr  5 16:38:49 2024, max compression
```

## Comparing `dirigera-1.0.9.tar` & `dirigera-1.1.0.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 08:07:21.334338 dirigera-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-02-22 08:07:07.000000 dirigera-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14278 2024-02-22 08:07:21.330338 dirigera-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-02-22 08:07:07.000000 dirigera-1.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-02-22 08:07:07.000000 dirigera-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 08:07:21.334338 dirigera-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-22 08:07:07.000000 dirigera-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 08:07:21.326338 dirigera-1.0.9/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 08:07:21.326338 dirigera-1.0.9/src/dirigera/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 08:07:21.330338 dirigera-1.0.9/src/dirigera/devices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/devices/air_purifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/devices/base_ikea_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/devices/blinds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/devices/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/devices/environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/devices/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/devices/motion_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/devices/open_close_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/devices/outlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/devices/scene.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 08:07:21.330338 dirigera-1.0.9/src/dirigera/hub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/hub/abstract_smart_home_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10537 2024-02-22 08:07:07.000000 dirigera-1.0.9/src/dirigera/hub/hub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 08:07:21.330338 dirigera-1.0.9/src/dirigera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14278 2024-02-22 08:07:21.000000 dirigera-1.0.9/src/dirigera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-22 08:07:21.000000 dirigera-1.0.9/src/dirigera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 08:07:21.000000 dirigera-1.0.9/src/dirigera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-22 08:07:21.000000 dirigera-1.0.9/src/dirigera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-22 08:07:21.000000 dirigera-1.0.9/src/dirigera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-22 08:07:21.000000 dirigera-1.0.9/src/dirigera.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 08:07:21.330338 dirigera-1.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-02-22 08:07:07.000000 dirigera-1.0.9/tests/test_air_purifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-02-22 08:07:07.000000 dirigera-1.0.9/tests/test_blinds.py
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-02-22 08:07:07.000000 dirigera-1.0.9/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-02-22 08:07:07.000000 dirigera-1.0.9/tests/test_environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12981 2024-02-22 08:07:07.000000 dirigera-1.0.9/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-02-22 08:07:07.000000 dirigera-1.0.9/tests/test_motion_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-02-22 08:07:07.000000 dirigera-1.0.9/tests/test_open_close_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-02-22 08:07:07.000000 dirigera-1.0.9/tests/test_outlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-02-22 08:07:07.000000 dirigera-1.0.9/tests/test_scenes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:38:49.585303 dirigera-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-05 16:38:42.000000 dirigera-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-04-05 16:38:49.585303 dirigera-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13314 2024-04-05 16:38:42.000000 dirigera-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-05 16:38:42.000000 dirigera-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:38:49.585303 dirigera-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-05 16:38:42.000000 dirigera-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:38:49.577303 dirigera-1.1.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:38:49.577303 dirigera-1.1.0/src/dirigera/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:38:49.581303 dirigera-1.1.0/src/dirigera/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/devices/air_purifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/devices/base_ikea_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/devices/blinds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/devices/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/devices/environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/devices/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/devices/motion_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/devices/open_close_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/devices/outlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/devices/scene.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:38:49.581303 dirigera-1.1.0/src/dirigera/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/hub/abstract_smart_home_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14755 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/hub/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/hub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:38:49.585303 dirigera-1.1.0/src/dirigera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-04-05 16:38:49.000000 dirigera-1.1.0/src/dirigera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-05 16:38:49.000000 dirigera-1.1.0/src/dirigera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:38:49.000000 dirigera-1.1.0/src/dirigera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 16:38:49.000000 dirigera-1.1.0/src/dirigera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-05 16:38:49.000000 dirigera-1.1.0/src/dirigera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 16:38:49.000000 dirigera-1.1.0/src/dirigera.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:38:49.585303 dirigera-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-05 16:38:42.000000 dirigera-1.1.0/tests/test_air_purifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-05 16:38:42.000000 dirigera-1.1.0/tests/test_blinds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-05 16:38:42.000000 dirigera-1.1.0/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-05 16:38:42.000000 dirigera-1.1.0/tests/test_environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12981 2024-04-05 16:38:42.000000 dirigera-1.1.0/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-05 16:38:42.000000 dirigera-1.1.0/tests/test_motion_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-05 16:38:42.000000 dirigera-1.1.0/tests/test_open_close_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-04-05 16:38:42.000000 dirigera-1.1.0/tests/test_outlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-05 16:38:42.000000 dirigera-1.1.0/tests/test_scenes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-05 16:38:42.000000 dirigera-1.1.0/tests/test_utils.py
```

### Comparing `dirigera-1.0.9/LICENSE` & `dirigera-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.9/PKG-INFO` & `dirigera-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 1.0.9
+Version: 1.1.0
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -58,14 +58,15 @@
 - [outlet control](#controlling-outlets)
 - [air purifier control](#controlling-air-purifier)
 - [blinds control](#controlling-blinds)
 - [remote controllers](#remote-controllers) (tested with STYRBAR)
 - [environment sensor](#environment-sensor) (tested with VINDSTYRKA)
 - [scene](#scene)
 - [motion sensor](#motion-sensor)
+- [open/close sensor](#open-close-sensor)
 - [event listener](#event-listener) for hub events
 
 Support for other features will be added in the future and your input in form of issues and PRs is greatly appreciated.
 
 ## Installation
 
 ```bash
@@ -264,15 +265,14 @@
 air_purifier.set_motor_state(motor_state=42)
 
 air_purifier.set_child_lock(child_lock=True)
 
 air_purifier.set_status_light(light_state=False)
 ```
 
-
 ## [Controlling Blinds](./src/dirigera/devices/blinds.py)
 
 To get information about the available blinds, you can use the `get_blinds()` method:
 
 ```python
 blinds = dirigera_hub.get_blinds()
 ```
@@ -325,15 +325,15 @@
 ```python
 sensors = dirigera_hub.get_environment_sensors()
 ```
 
 The environment sensor object has the following attributes (additional to the core attributes):
 
 ```python
-current_temperature: int
+current_temperature: float
 current_r_h: int # current humidity
 current_p_m25: int # current particulate matter 2.5
 max_measured_p_m25: int # maximum measurable particulate matter 2.5
 min_measured_p_m25: int # minimum measurable particulate matter 2.5
 voc_index: int # current volatile organic compound
 ```
 
@@ -351,35 +351,84 @@
 scenes = dirigera_hub.get_scenes()
 ```
 
 The scene object has the following attributes:
 
 ```python
 id: str
-type: str
+type: SceneType
 info: Info
 triggers: List[Trigger]
 actions: List[Action]
 created_at: datetime.datetime
-last_completed: datetime.datetime
-last_triggered: datetime.datetime
-last_undo: datetime.datetime
+last_completed: Optional[datetime.datetime] = None
+last_triggered: Optional[datetime.datetime] = None
+last_undo: Optional[datetime.datetime] = None
 commands: List[str]
 undo_allowed_duration: int
 ```
 
 Details to the Trigger, Action and Info class can be found in [scene.py](./src/dirigera/devices/scene.py)
 
 Available methods for scene are:
 
 ```python
 scene.trigger()
 scene.undo()
 ```
 
+### Creating a Scene
+
+To create a scene use the `create_scene()` function.  
+Example how to create an empty scene:
+
+```python
+scene = dirigera_hub.create_scene(
+    info=Info(name="This is empty", icon=Icon.SCENES_BOOK),
+)
+```
+
+Actions look like this:
+
+```python
+class Action(BaseIkeaModel):
+    id: str
+    type: str
+    enabled: Optional[bool] = None
+    attributes: Optional[ActionAttributes] = None
+```
+
+Example how create scene with action:
+
+```python
+from dirigera.devices.scene import Info, Icon, SceneType, Action, ActionAttributes
+
+light = dirigera_hub.get_light_by_name("kitchen_lamp")
+
+scene = dirigera_hub.create_scene(
+    info=Info(name="Scene with action", icon=Icon.SCENES_BOOK),
+    scene_type=SceneType.USER_SCENE,
+    triggers=[],
+    actions=[Action(id=light.id, type="device", enabled=True, attributes=ActionAttributes(is_on=False))],
+)
+```
+
+Triggers look like this:
+
+```python
+class Trigger(BaseIkeaModel):
+    id: str
+    type: str
+    triggered_at: Optional[datetime.datetime] = None
+    disabled: bool
+
+```
+
+All available icons can be found here: [Icons](./src/dirigera/devices/scene.py)
+
 ## [Motion Sensor](./src/dirigera/devices/motion_sensor.py)
 
 To get information about the available motion sensors, you can use the `get_motion_sensors()` method:
 
 ```python
 motions_sensors = dirigera_hub.get_motion_sensors()
 ```
@@ -394,17 +443,17 @@
 
 Available methods for outlet are:
 
 ```python
 motions_sensor.set_name(name="kitchen sensor 1")
 ```
 
-## [Open/Close Sensor](./src/dirigera/devices/open_close_sensor.py)
+## [Open Close Sensor](./src/dirigera/devices/open_close_sensor.py)
 
-To get information about the available motion sensors, you can use the `get_open_close_sensors()` method:
+To get information about the available open/close sensors, you can use the `get_open_close_sensors()` method:
 
 ```python
 open_close_sensors = dirigera_hub.get_open_close_sensors()
 ```
 
 The open_close_sensor object has the following attributes (additional to the core attributes):
 
@@ -447,14 +496,15 @@
 
 ## Motivation
 
 The primary motivation for this project was to provide users with the ability to control the startup behavior of their smart home lamps when there is a power outage.  
 The default behavior of the hub is to turn on all lights when power is restored, which can be problematic if the user is away from home or on vacation, and a small power fluctuation causes all lights to turn on and stay on. Unfortunately, the IKEA app does not offer a way to change this default behavior.  
 The `set_startup_behaviour()` function enables users to override the default behavior and choose the startup behavior that best suits their needs (START_ON = turn on light when power is back, START_OFF = light stays off when power is back).  
 I can not guarantee that all IKEA lamps offer this functionality.
+EDIT: This is now an exposed feature in the app.
 
 ## Contributing
 
 Contributions are welcome! If you have an idea for a new feature or a bug fix, please post and issue or submit a pull request.
 
 ### Setup of dev
```

### Comparing `dirigera-1.0.9/README.md` & `dirigera-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 - [outlet control](#controlling-outlets)
 - [air purifier control](#controlling-air-purifier)
 - [blinds control](#controlling-blinds)
 - [remote controllers](#remote-controllers) (tested with STYRBAR)
 - [environment sensor](#environment-sensor) (tested with VINDSTYRKA)
 - [scene](#scene)
 - [motion sensor](#motion-sensor)
+- [open/close sensor](#open-close-sensor)
 - [event listener](#event-listener) for hub events
 
 Support for other features will be added in the future and your input in form of issues and PRs is greatly appreciated.
 
 ## Installation
 
 ```bash
@@ -217,15 +218,14 @@
 air_purifier.set_motor_state(motor_state=42)
 
 air_purifier.set_child_lock(child_lock=True)
 
 air_purifier.set_status_light(light_state=False)
 ```
 
-
 ## [Controlling Blinds](./src/dirigera/devices/blinds.py)
 
 To get information about the available blinds, you can use the `get_blinds()` method:
 
 ```python
 blinds = dirigera_hub.get_blinds()
 ```
@@ -278,15 +278,15 @@
 ```python
 sensors = dirigera_hub.get_environment_sensors()
 ```
 
 The environment sensor object has the following attributes (additional to the core attributes):
 
 ```python
-current_temperature: int
+current_temperature: float
 current_r_h: int # current humidity
 current_p_m25: int # current particulate matter 2.5
 max_measured_p_m25: int # maximum measurable particulate matter 2.5
 min_measured_p_m25: int # minimum measurable particulate matter 2.5
 voc_index: int # current volatile organic compound
 ```
 
@@ -304,35 +304,84 @@
 scenes = dirigera_hub.get_scenes()
 ```
 
 The scene object has the following attributes:
 
 ```python
 id: str
-type: str
+type: SceneType
 info: Info
 triggers: List[Trigger]
 actions: List[Action]
 created_at: datetime.datetime
-last_completed: datetime.datetime
-last_triggered: datetime.datetime
-last_undo: datetime.datetime
+last_completed: Optional[datetime.datetime] = None
+last_triggered: Optional[datetime.datetime] = None
+last_undo: Optional[datetime.datetime] = None
 commands: List[str]
 undo_allowed_duration: int
 ```
 
 Details to the Trigger, Action and Info class can be found in [scene.py](./src/dirigera/devices/scene.py)
 
 Available methods for scene are:
 
 ```python
 scene.trigger()
 scene.undo()
 ```
 
+### Creating a Scene
+
+To create a scene use the `create_scene()` function.  
+Example how to create an empty scene:
+
+```python
+scene = dirigera_hub.create_scene(
+    info=Info(name="This is empty", icon=Icon.SCENES_BOOK),
+)
+```
+
+Actions look like this:
+
+```python
+class Action(BaseIkeaModel):
+    id: str
+    type: str
+    enabled: Optional[bool] = None
+    attributes: Optional[ActionAttributes] = None
+```
+
+Example how create scene with action:
+
+```python
+from dirigera.devices.scene import Info, Icon, SceneType, Action, ActionAttributes
+
+light = dirigera_hub.get_light_by_name("kitchen_lamp")
+
+scene = dirigera_hub.create_scene(
+    info=Info(name="Scene with action", icon=Icon.SCENES_BOOK),
+    scene_type=SceneType.USER_SCENE,
+    triggers=[],
+    actions=[Action(id=light.id, type="device", enabled=True, attributes=ActionAttributes(is_on=False))],
+)
+```
+
+Triggers look like this:
+
+```python
+class Trigger(BaseIkeaModel):
+    id: str
+    type: str
+    triggered_at: Optional[datetime.datetime] = None
+    disabled: bool
+
+```
+
+All available icons can be found here: [Icons](./src/dirigera/devices/scene.py)
+
 ## [Motion Sensor](./src/dirigera/devices/motion_sensor.py)
 
 To get information about the available motion sensors, you can use the `get_motion_sensors()` method:
 
 ```python
 motions_sensors = dirigera_hub.get_motion_sensors()
 ```
@@ -347,17 +396,17 @@
 
 Available methods for outlet are:
 
 ```python
 motions_sensor.set_name(name="kitchen sensor 1")
 ```
 
-## [Open/Close Sensor](./src/dirigera/devices/open_close_sensor.py)
+## [Open Close Sensor](./src/dirigera/devices/open_close_sensor.py)
 
-To get information about the available motion sensors, you can use the `get_open_close_sensors()` method:
+To get information about the available open/close sensors, you can use the `get_open_close_sensors()` method:
 
 ```python
 open_close_sensors = dirigera_hub.get_open_close_sensors()
 ```
 
 The open_close_sensor object has the following attributes (additional to the core attributes):
 
@@ -400,14 +449,15 @@
 
 ## Motivation
 
 The primary motivation for this project was to provide users with the ability to control the startup behavior of their smart home lamps when there is a power outage.  
 The default behavior of the hub is to turn on all lights when power is restored, which can be problematic if the user is away from home or on vacation, and a small power fluctuation causes all lights to turn on and stay on. Unfortunately, the IKEA app does not offer a way to change this default behavior.  
 The `set_startup_behaviour()` function enables users to override the default behavior and choose the startup behavior that best suits their needs (START_ON = turn on light when power is back, START_OFF = light stays off when power is back).  
 I can not guarantee that all IKEA lamps offer this functionality.
+EDIT: This is now an exposed feature in the app.
 
 ## Contributing
 
 Contributions are welcome! If you have an idea for a new feature or a bug fix, please post and issue or submit a pull request.
 
 ### Setup of dev
```

### Comparing `dirigera-1.0.9/pyproject.toml` & `dirigera-1.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dirigera"
-version = "1.0.9"
+version = "1.1.0"
 description = "An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub"
 readme = "README.md"
 authors = [{ name = "Leggin", email = "legginsun@gmail.com" }]
 license = { file = "LICENSE" }
 keywords = [
     "python",
     "iot",
```

### Comparing `dirigera-1.0.9/src/dirigera/devices/air_purifier.py` & `dirigera-1.1.0/src/dirigera/devices/air_purifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 from enum import Enum
 from typing import Any, Dict
 from .device import Attributes, Device
 from ..hub.abstract_smart_home_hub import AbstractSmartHomeHub
 
 class FanModeEnum(Enum):
+    OFF = "off"
     LOW = "low"
     MEDIUM = "medium"
     HIGH = "high"
     AUTO = "auto"
 
 class AirPurifierAttributes(Attributes):
     """canReceive"""
```

### Comparing `dirigera-1.0.9/src/dirigera/devices/blinds.py` & `dirigera-1.1.0/src/dirigera/devices/blinds.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from ..hub.abstract_smart_home_hub import AbstractSmartHomeHub
 
 
 class BlindAttributes(Attributes):
     blinds_current_level: Optional[int] = None
     blinds_target_level: Optional[int] = None
     blinds_state: Optional[str] = None
+    battery_percentage: Optional[int] = None
 
 
 class Blind(Device):
     dirigera_client: AbstractSmartHomeHub
     attributes: BlindAttributes
 
     def reload(self) -> Blind:
```

### Comparing `dirigera-1.0.9/src/dirigera/devices/controller.py` & `dirigera-1.1.0/src/dirigera/devices/controller.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.9/src/dirigera/devices/device.py` & `dirigera-1.1.0/src/dirigera/devices/device.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,14 +45,14 @@
     type: str
     device_type: str
     created_at: datetime.datetime
     is_reachable: bool
     last_seen: datetime.datetime
     attributes: Attributes
     capabilities: Capabilities
-    room: Room
+    room: Optional[Room] = None
     device_set: List
     remote_links: List[str]
     is_hidden: Optional[bool] = None
 
     def _reload(self, data: Dict[str, Any]) -> Device:
         return Device(**data)
```

### Comparing `dirigera-1.0.9/src/dirigera/devices/environment_sensor.py` & `dirigera-1.1.0/src/dirigera/devices/environment_sensor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 from .device import Attributes, Device
 from ..hub.abstract_smart_home_hub import AbstractSmartHomeHub
 
 
 class EnvironmentSensorAttributes(Attributes):
-    current_temperature: int
+    current_temperature: float
     current_r_h: int
-    current_p_m25: int
-    max_measured_p_m25: int
-    min_measured_p_m25: int
-    voc_index: int
+    current_p_m25: Optional[int]
+    max_measured_p_m25: Optional[int]
+    min_measured_p_m25: Optional[int]
+    voc_index: Optional[int]
 
 
 class EnvironmentSensor(Device):
     dirigera_client: AbstractSmartHomeHub
     attributes: EnvironmentSensorAttributes
 
     def reload(self) -> EnvironmentSensor:
```

### Comparing `dirigera-1.0.9/src/dirigera/devices/light.py` & `dirigera-1.1.0/src/dirigera/devices/light.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.9/src/dirigera/devices/motion_sensor.py` & `dirigera-1.1.0/src/dirigera/devices/motion_sensor.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from .device import Attributes, Device
 from ..hub.abstract_smart_home_hub import AbstractSmartHomeHub
 
 
 class MotionSensorAttributes(Attributes):
     battery_percentage: int
     is_on: bool
-    light_level: Optional[float]
+    light_level: Optional[float] = None
+    is_detected: Optional[bool] = False
 
 
 class MotionSensor(Device):
     dirigera_client: AbstractSmartHomeHub
     attributes: MotionSensorAttributes
 
     def reload(self) -> MotionSensor:
```

### Comparing `dirigera-1.0.9/src/dirigera/devices/open_close_sensor.py` & `dirigera-1.1.0/src/dirigera/devices/open_close_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.9/src/dirigera/devices/outlet.py` & `dirigera-1.1.0/src/dirigera/devices/outlet.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.9/src/dirigera/hub/abstract_smart_home_hub.py` & `dirigera-1.1.0/src/dirigera/hub/abstract_smart_home_hub.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,25 +11,33 @@
     def get(self, route: str) -> Any:
         raise NotImplementedError
 
     @abc.abstractmethod
     def post(self, route: str, data: Optional[Dict[str, Any]] = None) -> Any:
         raise NotImplementedError
 
+    @abc.abstractmethod
+    def delete(self, route: str, data: Optional[Dict[str, Any]] = None) -> Any:
+        raise NotImplementedError
+
 
 class FakeDirigeraHub(AbstractSmartHomeHub):
     def __init__(self) -> None:
         self.patch_actions: List = []
         self.post_actions: List = []
         self.get_actions: List = []
         self.get_action_replys: Dict = {}
+        self.delete_actions: List = []
 
     def patch(self, route: str, data: List[Dict[str, Any]]) -> Any:
         self.patch_actions.append({"route": route, "data": data})
         return {"route": route, "data": data}
 
     def get(self, route: str) -> Any:
         self.get_actions.append({"route": route})
         return self.get_action_replys[route]
 
     def post(self, route: str, data: Optional[Dict[str, Any]] = None) -> Any:
         self.post_actions.append({"route": route, "data": data})
+
+    def delete(self, route: str, data: Optional[Dict[str, Any]] = None) -> Any:
+        self.delete_actions.append({"route": route, "data": data})
```

### Comparing `dirigera-1.0.9/src/dirigera/hub/auth.py` & `dirigera-1.1.0/src/dirigera/hub/auth.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.9/src/dirigera.egg-info/PKG-INFO` & `dirigera-1.1.0/src/dirigera.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 1.0.9
+Version: 1.1.0
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -58,14 +58,15 @@
 - [outlet control](#controlling-outlets)
 - [air purifier control](#controlling-air-purifier)
 - [blinds control](#controlling-blinds)
 - [remote controllers](#remote-controllers) (tested with STYRBAR)
 - [environment sensor](#environment-sensor) (tested with VINDSTYRKA)
 - [scene](#scene)
 - [motion sensor](#motion-sensor)
+- [open/close sensor](#open-close-sensor)
 - [event listener](#event-listener) for hub events
 
 Support for other features will be added in the future and your input in form of issues and PRs is greatly appreciated.
 
 ## Installation
 
 ```bash
@@ -264,15 +265,14 @@
 air_purifier.set_motor_state(motor_state=42)
 
 air_purifier.set_child_lock(child_lock=True)
 
 air_purifier.set_status_light(light_state=False)
 ```
 
-
 ## [Controlling Blinds](./src/dirigera/devices/blinds.py)
 
 To get information about the available blinds, you can use the `get_blinds()` method:
 
 ```python
 blinds = dirigera_hub.get_blinds()
 ```
@@ -325,15 +325,15 @@
 ```python
 sensors = dirigera_hub.get_environment_sensors()
 ```
 
 The environment sensor object has the following attributes (additional to the core attributes):
 
 ```python
-current_temperature: int
+current_temperature: float
 current_r_h: int # current humidity
 current_p_m25: int # current particulate matter 2.5
 max_measured_p_m25: int # maximum measurable particulate matter 2.5
 min_measured_p_m25: int # minimum measurable particulate matter 2.5
 voc_index: int # current volatile organic compound
 ```
 
@@ -351,35 +351,84 @@
 scenes = dirigera_hub.get_scenes()
 ```
 
 The scene object has the following attributes:
 
 ```python
 id: str
-type: str
+type: SceneType
 info: Info
 triggers: List[Trigger]
 actions: List[Action]
 created_at: datetime.datetime
-last_completed: datetime.datetime
-last_triggered: datetime.datetime
-last_undo: datetime.datetime
+last_completed: Optional[datetime.datetime] = None
+last_triggered: Optional[datetime.datetime] = None
+last_undo: Optional[datetime.datetime] = None
 commands: List[str]
 undo_allowed_duration: int
 ```
 
 Details to the Trigger, Action and Info class can be found in [scene.py](./src/dirigera/devices/scene.py)
 
 Available methods for scene are:
 
 ```python
 scene.trigger()
 scene.undo()
 ```
 
+### Creating a Scene
+
+To create a scene use the `create_scene()` function.  
+Example how to create an empty scene:
+
+```python
+scene = dirigera_hub.create_scene(
+    info=Info(name="This is empty", icon=Icon.SCENES_BOOK),
+)
+```
+
+Actions look like this:
+
+```python
+class Action(BaseIkeaModel):
+    id: str
+    type: str
+    enabled: Optional[bool] = None
+    attributes: Optional[ActionAttributes] = None
+```
+
+Example how create scene with action:
+
+```python
+from dirigera.devices.scene import Info, Icon, SceneType, Action, ActionAttributes
+
+light = dirigera_hub.get_light_by_name("kitchen_lamp")
+
+scene = dirigera_hub.create_scene(
+    info=Info(name="Scene with action", icon=Icon.SCENES_BOOK),
+    scene_type=SceneType.USER_SCENE,
+    triggers=[],
+    actions=[Action(id=light.id, type="device", enabled=True, attributes=ActionAttributes(is_on=False))],
+)
+```
+
+Triggers look like this:
+
+```python
+class Trigger(BaseIkeaModel):
+    id: str
+    type: str
+    triggered_at: Optional[datetime.datetime] = None
+    disabled: bool
+
+```
+
+All available icons can be found here: [Icons](./src/dirigera/devices/scene.py)
+
 ## [Motion Sensor](./src/dirigera/devices/motion_sensor.py)
 
 To get information about the available motion sensors, you can use the `get_motion_sensors()` method:
 
 ```python
 motions_sensors = dirigera_hub.get_motion_sensors()
 ```
@@ -394,17 +443,17 @@
 
 Available methods for outlet are:
 
 ```python
 motions_sensor.set_name(name="kitchen sensor 1")
 ```
 
-## [Open/Close Sensor](./src/dirigera/devices/open_close_sensor.py)
+## [Open Close Sensor](./src/dirigera/devices/open_close_sensor.py)
 
-To get information about the available motion sensors, you can use the `get_open_close_sensors()` method:
+To get information about the available open/close sensors, you can use the `get_open_close_sensors()` method:
 
 ```python
 open_close_sensors = dirigera_hub.get_open_close_sensors()
 ```
 
 The open_close_sensor object has the following attributes (additional to the core attributes):
 
@@ -447,14 +496,15 @@
 
 ## Motivation
 
 The primary motivation for this project was to provide users with the ability to control the startup behavior of their smart home lamps when there is a power outage.  
 The default behavior of the hub is to turn on all lights when power is restored, which can be problematic if the user is away from home or on vacation, and a small power fluctuation causes all lights to turn on and stay on. Unfortunately, the IKEA app does not offer a way to change this default behavior.  
 The `set_startup_behaviour()` function enables users to override the default behavior and choose the startup behavior that best suits their needs (START_ON = turn on light when power is back, START_OFF = light stays off when power is back).  
 I can not guarantee that all IKEA lamps offer this functionality.
+EDIT: This is now an exposed feature in the app.
 
 ## Contributing
 
 Contributions are welcome! If you have an idea for a new feature or a bug fix, please post and issue or submit a pull request.
 
 ### Setup of dev
```

### Comparing `dirigera-1.0.9/src/dirigera.egg-info/SOURCES.txt` & `dirigera-1.1.0/src/dirigera.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,18 @@
 src/dirigera/devices/open_close_sensor.py
 src/dirigera/devices/outlet.py
 src/dirigera/devices/scene.py
 src/dirigera/hub/__init__.py
 src/dirigera/hub/abstract_smart_home_hub.py
 src/dirigera/hub/auth.py
 src/dirigera/hub/hub.py
+src/dirigera/hub/utils.py
 tests/test_air_purifier.py
 tests/test_blinds.py
 tests/test_controller.py
 tests/test_environment_sensor.py
 tests/test_light.py
 tests/test_motion_sensor.py
 tests/test_open_close_sensor.py
 tests/test_outlet.py
-tests/test_scenes.py
+tests/test_scenes.py
+tests/test_utils.py
```

### Comparing `dirigera-1.0.9/tests/test_air_purifier.py` & `dirigera-1.1.0/tests/test_air_purifier.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.9/tests/test_blinds.py` & `dirigera-1.1.0/tests/test_blinds.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.9/tests/test_controller.py` & `dirigera-1.1.0/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.9/tests/test_environment_sensor.py` & `dirigera-1.1.0/tests/test_environment_sensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             "customName": "Envsensor",
             "model": "VINDSTYRKA",
             "manufacturer": "IKEA of Sweden",
             "firmwareVersion": "1.0.11",
             "hardwareVersion": "1",
             "serialNumber": "F4B3B1FFFE00101E",
             "productCode": "E2112",
-            "currentTemperature": 21,
+            "currentTemperature": 21.1,
             "currentRH": 61,
             "currentPM25": 1,
             "maxMeasuredPM25": 999,
             "minMeasuredPM25": 0,
             "vocIndex": 63,
             "identifyStarted": "2000-01-01T00:00:00.000Z",
             "otaStatus": "upToDate",
```

### Comparing `dirigera-1.0.9/tests/test_light.py` & `dirigera-1.1.0/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.9/tests/test_motion_sensor.py` & `dirigera-1.1.0/tests/test_motion_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.9/tests/test_open_close_sensor.py` & `dirigera-1.1.0/tests/test_open_close_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.9/tests/test_outlet.py` & `dirigera-1.1.0/tests/test_outlet.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.0.9/tests/test_scenes.py` & `dirigera-1.1.0/tests/test_scenes.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,11 +83,11 @@
         "undoAllowedDuration": 30,
         "lastUndo": "2023-08-27T10:29:33.049Z",
     }
 
     scene = dict_to_scene(data, fake_client)
     assert scene.id == TEST_ID
     assert scene.info.name == TEST_NAME
-    assert scene.info.icon == TEST_ICON
+    assert scene.info.icon.value == TEST_ICON
     assert scene.last_completed == datetime.datetime.strptime(
         TEST_LAST_COMPLETED, "%Y-%m-%dT%H:%M:%S.%f%z"
     )
```

