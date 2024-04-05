# Comparing `tmp/pybricks-3.4.1.tar.gz` & `tmp/pybricks-3.5.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybricks-3.4.1.tar", max compression
+gzip compressed data, was "pybricks-3.5.0b1.tar", max compression
```

## Comparing `pybricks-3.4.1.tar` & `pybricks-3.5.0b1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      213 2024-03-11 15:30:24.717508 pybricks-3.4.1/AUTHORS.md
--rw-r--r--   0        0        0     1082 2024-03-11 15:30:24.717508 pybricks-3.4.1/LICENSE
--rw-r--r--   0        0        0     1185 2024-03-11 15:30:24.717508 pybricks-3.4.1/README.rst
--rw-r--r--   0        0        0     1357 2024-03-11 15:30:24.841509 pybricks-3.4.1/pyproject.toml
--rw-r--r--   0        0        0     4264 2024-03-11 15:30:24.841509 pybricks-3.4.1/src/micropython/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 15:30:24.841509 pybricks-3.4.1/src/micropython/py.typed
--rw-r--r--   0        0        0      122 2024-03-11 15:30:24.841509 pybricks-3.4.1/src/pybricks/__init__.py
--rw-r--r--   0        0        0    45466 2024-03-11 15:30:24.841509 pybricks-3.4.1/src/pybricks/_common.py
--rw-r--r--   0        0        0     4511 2024-03-11 15:30:24.841509 pybricks-3.4.1/src/pybricks/ev3dev/_speaker.py
--rw-r--r--   0        0        0     6619 2024-03-11 15:30:24.841509 pybricks-3.4.1/src/pybricks/ev3devices.py
--rw-r--r--   0        0        0     8556 2024-03-11 15:30:24.841509 pybricks-3.4.1/src/pybricks/hubs.py
--rw-r--r--   0        0        0    10511 2024-03-11 15:30:24.841509 pybricks-3.4.1/src/pybricks/iodevices.py
--rw-r--r--   0        0        0        0 2024-03-11 15:30:24.841509 pybricks-3.4.1/src/pybricks/media/__init__.py
--rw-r--r--   0        0        0    20861 2024-03-11 15:30:24.841509 pybricks-3.4.1/src/pybricks/media/ev3dev.py
--rw-r--r--   0        0        0        0 2024-03-11 15:30:24.841509 pybricks-3.4.1/src/pybricks/media/py.typed
--rw-r--r--   0        0        0     6524 2024-03-11 15:30:24.841509 pybricks-3.4.1/src/pybricks/messaging.py
--rw-r--r--   0        0        0     6671 2024-03-11 15:30:24.841509 pybricks-3.4.1/src/pybricks/nxtdevices.py
--rw-r--r--   0        0        0    12635 2024-03-11 15:30:24.845509 pybricks-3.4.1/src/pybricks/parameters.py
--rw-r--r--   0        0        0    13076 2024-03-11 15:30:24.845509 pybricks-3.4.1/src/pybricks/pupdevices.py
--rw-r--r--   0        0        0        0 2024-03-11 15:30:24.845509 pybricks-3.4.1/src/pybricks/py.typed
--rw-r--r--   0        0        0    10716 2024-03-11 15:30:24.845509 pybricks-3.4.1/src/pybricks/robotics.py
--rw-r--r--   0        0        0     7920 2024-03-11 15:30:24.845509 pybricks-3.4.1/src/pybricks/tools.py
--rw-r--r--   0        0        0     1409 2024-03-11 15:30:24.845509 pybricks-3.4.1/src/uerrno/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 15:30:24.845509 pybricks-3.4.1/src/uerrno/py.typed
--rw-r--r--   0        0        0     2523 2024-03-11 15:30:24.845509 pybricks-3.4.1/src/uio/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 15:30:24.845509 pybricks-3.4.1/src/uio/py.typed
--rw-r--r--   0        0        0     2007 2024-03-11 15:30:24.845509 pybricks-3.4.1/src/ujson/__init__.py
--rw-r--r--   0        0        0     6378 2024-03-11 15:30:24.845509 pybricks-3.4.1/src/umath/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 15:30:24.845509 pybricks-3.4.1/src/umath/py.typed
--rw-r--r--   0        0        0     3153 2024-03-11 15:30:24.845509 pybricks-3.4.1/src/urandom/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 15:30:24.845509 pybricks-3.4.1/src/urandom/py.typed
--rw-r--r--   0        0        0     4952 2024-03-11 15:30:24.845509 pybricks-3.4.1/src/uselect/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 15:30:24.845509 pybricks-3.4.1/src/uselect/py.typed
--rw-r--r--   0        0        0     2280 2024-03-11 15:30:24.845509 pybricks-3.4.1/src/ustruct/__init__.py
--rw-r--r--   0        0        0     1402 2024-03-11 15:30:24.845509 pybricks-3.4.1/src/usys/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 15:30:24.845509 pybricks-3.4.1/src/usys/py.typed
--rw-r--r--   0        0        0     2089 1970-01-01 00:00:00.000000 pybricks-3.4.1/PKG-INFO
+-rw-r--r--   0        0        0      213 2024-03-21 18:18:23.553122 pybricks-3.5.0b1/AUTHORS.md
+-rw-r--r--   0        0        0     1082 2024-03-21 18:18:23.553122 pybricks-3.5.0b1/LICENSE
+-rw-r--r--   0        0        0     1185 2024-03-21 18:18:23.553122 pybricks-3.5.0b1/README.rst
+-rw-r--r--   0        0        0     1360 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/pyproject.toml
+-rw-r--r--   0        0        0     4264 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/micropython/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/micropython/py.typed
+-rw-r--r--   0        0        0      122 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/__init__.py
+-rw-r--r--   0        0        0    45572 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/_common.py
+-rw-r--r--   0        0        0     4511 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/ev3dev/_speaker.py
+-rw-r--r--   0        0        0     6619 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/ev3devices.py
+-rw-r--r--   0        0        0     8556 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/hubs.py
+-rw-r--r--   0        0        0    12138 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/iodevices.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/media/__init__.py
+-rw-r--r--   0        0        0    20861 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/media/ev3dev.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/media/py.typed
+-rw-r--r--   0        0        0     6524 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/messaging.py
+-rw-r--r--   0        0        0     6671 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/nxtdevices.py
+-rw-r--r--   0        0        0    12635 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/parameters.py
+-rw-r--r--   0        0        0    13076 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/pupdevices.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/py.typed
+-rw-r--r--   0        0        0    10716 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/robotics.py
+-rw-r--r--   0        0        0     7920 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/tools.py
+-rw-r--r--   0        0        0     1409 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/uerrno/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/uerrno/py.typed
+-rw-r--r--   0        0        0     2523 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/uio/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/uio/py.typed
+-rw-r--r--   0        0        0     2007 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/ujson/__init__.py
+-rw-r--r--   0        0        0     6378 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/umath/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/umath/py.typed
+-rw-r--r--   0        0        0     3153 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/urandom/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/urandom/py.typed
+-rw-r--r--   0        0        0     4952 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/uselect/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/uselect/py.typed
+-rw-r--r--   0        0        0     2280 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/ustruct/__init__.py
+-rw-r--r--   0        0        0     1402 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/usys/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/usys/py.typed
+-rw-r--r--   0        0        0     2091 1970-01-01 00:00:00.000000 pybricks-3.5.0b1/PKG-INFO
```

### Comparing `pybricks-3.4.1/LICENSE` & `pybricks-3.5.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pybricks-3.4.1/README.rst` & `pybricks-3.5.0b1/README.rst`

 * *Files identical despite different names*

### Comparing `pybricks-3.4.1/pyproject.toml` & `pybricks-3.5.0b1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybricks"
-version = "3.4.1"
+version = "v3.5.0b1"
 description = "Documentation and user-API stubs for Pybricks MicroPython"
 authors = ["The Pybricks Authors <team@pybricks.com>"]
 maintainers = ["Laurens Valk <laurens@pybricks.com>", "David Lechner <david@pybricks.com>" ]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://pybricks.com"
 repository = "https://github.com/pybricks/pybricks-api"
```

### Comparing `pybricks-3.4.1/src/micropython/__init__.py` & `pybricks-3.5.0b1/src/micropython/__init__.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.4.1/src/pybricks/_common.py` & `pybricks-3.5.0b1/src/pybricks/_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,16 @@
         change or disable this behavior in order to use the button for other
         purposes.
 
         Arguments:
             button (Button): A button such
                 as :attr:`Button.CENTER <pybricks.parameters.Button.CENTER>`,
                 or a tuple of multiple buttons. Choose ``None`` to disable the
-                stop button altogether.
+                stop button altogether. If you do, you can still turn the hub
+                off by holding the center button for three seconds.
         """
 
     def shutdown(self) -> None:
         """shutdown()
 
         Stops your program and shuts the hub down."""
```

### Comparing `pybricks-3.4.1/src/pybricks/ev3dev/_speaker.py` & `pybricks-3.5.0b1/src/pybricks/ev3dev/_speaker.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.4.1/src/pybricks/ev3devices.py` & `pybricks-3.5.0b1/src/pybricks/ev3devices.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.4.1/src/pybricks/hubs.py` & `pybricks-3.5.0b1/src/pybricks/hubs.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.4.1/src/pybricks/iodevices.py` & `pybricks-3.5.0b1/src/pybricks/iodevices.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing import Dict, Tuple, Optional, overload, TYPE_CHECKING
 
 from . import _common
 from .parameters import Port as _Port
 
 if TYPE_CHECKING:
     from ._common import MaybeAwaitable, MaybeAwaitableTuple
+    from .parameters import Number
 
 
 class PUPDevice:
     """Powered Up motor or sensor."""
 
     def __init__(self, port: _Port):
         """PUPDevice(port)
@@ -380,30 +381,66 @@
         Returns:
             Tuple of left and right trigger positions.
         """
 
     def dpad(self) -> int:
         """dpad() -> int
 
-        Gets the direction-pad position. ``1`` is up, ``2`` is up-right,
-        ``3`` is right, ``4`` is down-right, ``5`` is down, ``6`` is
-        down-left, ``7`` is left, ``8`` is up-left, and ``0`` is not pressed.
+        Gets the direction-pad value. ``1`` is up, ``2`` is up-right, ``3``
+        is right, ``4`` is down-right, ``5`` is down, ``6`` is down-left,
+        ``7`` is left, ``8`` is up-left, and ``0`` is not pressed.
+
+        This is essentially the same as reading the state of the
+        ``Button.UP``, ``Button.RIGHT``, ``Button.DOWN``, and ``Button.LEFT``
+        buttons, but this method conveniently returns a number that indicates
+        a direction.
 
         Returns:
-            Direction-pad position.
+            Direction-pad position, indicating a direction.
         """
 
     def profile(self) -> int:
         """profile() -> int
 
         Gets the current profile of the controller. Only available on the
         Xbox Elite Controller Series 2.
 
         Returns:
             Profile number.
         """
 
+    def rumble(
+        self,
+        power: Number | Tuple[Number, Number, Number, Number] = 100,
+        duration: int = 200,
+        count: int = 1,
+        delay: int = 100,
+    ) -> MaybeAwaitable:
+        """rumble(power=100, duration=200, count=1, delay=100)
+
+        Makes the builtin actuators rumble, creating force feedback.
+
+        If you give a single ``power`` value, the left and right main actuators
+        will both rumble with that power. For more fine-grained control, set
+        ``power`` as a tuple of four values, which control the left main
+        actuator, right main actuator, left trigger actuator, and the right
+        trigger actuator, respectively. For example, ``power=(0, 0, 100, 0)``
+        makes the left trigger rumble at full power.
+
+        The rumble runs in the background while your program continues. To
+        make your program wait, just pause the program for a matching duration.
+        For one rumble, this equals ``duration``. For multiple rumbles, this
+        equals ``count * (duration + delay)``.
+
+        Arguments:
+            power (Number, % or tuple): Rumble power.
+            duration (Number, ms): Rumble duration.
+            count (int): Rumble count.
+            delay (Number, ms): Delay before each rumble. Only if ``count > 1``.
+        """
+
 
 # hide from jedi
 if TYPE_CHECKING:
     del MaybeAwaitable
     del MaybeAwaitableTuple
+    del Number
```

### Comparing `pybricks-3.4.1/src/pybricks/media/ev3dev.py` & `pybricks-3.5.0b1/src/pybricks/media/ev3dev.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.4.1/src/pybricks/messaging.py` & `pybricks-3.5.0b1/src/pybricks/messaging.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.4.1/src/pybricks/nxtdevices.py` & `pybricks-3.5.0b1/src/pybricks/nxtdevices.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.4.1/src/pybricks/parameters.py` & `pybricks-3.5.0b1/src/pybricks/parameters.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.4.1/src/pybricks/pupdevices.py` & `pybricks-3.5.0b1/src/pybricks/pupdevices.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.4.1/src/pybricks/robotics.py` & `pybricks-3.5.0b1/src/pybricks/robotics.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.4.1/src/pybricks/tools.py` & `pybricks-3.5.0b1/src/pybricks/tools.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.4.1/src/uerrno/__init__.py` & `pybricks-3.5.0b1/src/uerrno/__init__.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.4.1/src/uio/__init__.py` & `pybricks-3.5.0b1/src/uio/__init__.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.4.1/src/ujson/__init__.py` & `pybricks-3.5.0b1/src/ujson/__init__.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.4.1/src/umath/__init__.py` & `pybricks-3.5.0b1/src/umath/__init__.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.4.1/src/urandom/__init__.py` & `pybricks-3.5.0b1/src/urandom/__init__.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.4.1/src/uselect/__init__.py` & `pybricks-3.5.0b1/src/uselect/__init__.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.4.1/src/ustruct/__init__.py` & `pybricks-3.5.0b1/src/ustruct/__init__.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.4.1/src/usys/__init__.py` & `pybricks-3.5.0b1/src/usys/__init__.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.4.1/PKG-INFO` & `pybricks-3.5.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybricks
-Version: 3.4.1
+Version: 3.5.0b1
 Summary: Documentation and user-API stubs for Pybricks MicroPython
 Home-page: https://pybricks.com
 License: MIT
 Author: The Pybricks Authors
 Author-email: team@pybricks.com
 Maintainer: Laurens Valk
 Maintainer-email: laurens@pybricks.com
```

