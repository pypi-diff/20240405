# Comparing `tmp/indipydriver-1.1.2.tar.gz` & `tmp/indipydriver-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indipydriver-1.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "indipydriver-1.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `indipydriver-1.1.2.tar` & `indipydriver-1.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-07-31 15:52:08.000000 indipydriver-1.1.2/LICENSE
--rw-r--r--   0        0        0     2411 2023-07-11 05:27:01.000000 indipydriver-1.1.2/README.md
--rw-r--r--   0        0        0      573 2024-03-21 12:54:46.000000 indipydriver-1.1.2/indipydriver/__init__.py
--rw-r--r--   0        0        0    19033 2024-03-21 12:23:56.000000 indipydriver-1.1.2/indipydriver/comms.py
--rw-r--r--   0        0        0    21399 2024-01-06 13:04:44.000000 indipydriver-1.1.2/indipydriver/events.py
--rw-r--r--   0        0        0    21465 2024-02-08 21:56:03.000000 indipydriver-1.1.2/indipydriver/ipydriver.py
--rw-r--r--   0        0        0    12064 2024-02-07 20:19:44.000000 indipydriver-1.1.2/indipydriver/ipyserver.py
--rw-r--r--   0        0        0    12236 2024-02-23 14:46:47.000000 indipydriver-1.1.2/indipydriver/propertymembers.py
--rw-r--r--   0        0        0    43405 2024-02-23 14:49:50.000000 indipydriver-1.1.2/indipydriver/propertyvectors.py
--rw-r--r--   0        0        0      814 2024-03-21 12:54:06.000000 indipydriver-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     3124 1970-01-01 00:00:00.000000 indipydriver-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-31 15:52:08.000000 indipydriver-1.1.3/LICENSE
+-rw-r--r--   0        0        0     2411 2023-07-11 05:27:01.000000 indipydriver-1.1.3/README.md
+-rw-r--r--   0        0        0      573 2024-04-05 12:16:24.000000 indipydriver-1.1.3/indipydriver/__init__.py
+-rw-r--r--   0        0        0    19033 2024-03-21 12:23:56.000000 indipydriver-1.1.3/indipydriver/comms.py
+-rw-r--r--   0        0        0    21399 2024-01-06 13:04:44.000000 indipydriver-1.1.3/indipydriver/events.py
+-rw-r--r--   0        0        0    21349 2024-04-05 12:04:08.000000 indipydriver-1.1.3/indipydriver/ipydriver.py
+-rw-r--r--   0        0        0    12064 2024-02-07 20:19:44.000000 indipydriver-1.1.3/indipydriver/ipyserver.py
+-rw-r--r--   0        0        0    12236 2024-02-23 14:46:47.000000 indipydriver-1.1.3/indipydriver/propertymembers.py
+-rw-r--r--   0        0        0    43405 2024-02-23 14:49:50.000000 indipydriver-1.1.3/indipydriver/propertyvectors.py
+-rw-r--r--   0        0        0      814 2024-04-05 12:16:14.000000 indipydriver-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3124 1970-01-01 00:00:00.000000 indipydriver-1.1.3/PKG-INFO
```

### Comparing `indipydriver-1.1.2/LICENSE` & `indipydriver-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `indipydriver-1.1.2/README.md` & `indipydriver-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `indipydriver-1.1.2/indipydriver/__init__.py` & `indipydriver-1.1.3/indipydriver/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 
 from .ipydriver import IPyDriver, Device
 from .propertyvectors import SwitchVector, LightVector, TextVector, BLOBVector, NumberVector
 from .propertymembers import SwitchMember, LightMember, TextMember, BLOBMember, NumberMember
 from .events import getProperties, enableBLOB, newSwitchVector, newTextVector, newNumberVector, newBLOBVector, Message, delProperty, defSwitchVector, defTextVector, defNumberVector, defLightVector, defBLOBVector, setSwitchVector, setTextVector, setNumberVector, setLightVector, setBLOBVector
 from .ipyserver import IPyServer
 
-version = "1.1.2"
+version = "1.1.3"
```

### Comparing `indipydriver-1.1.2/indipydriver/comms.py` & `indipydriver-1.1.3/indipydriver/comms.py`

 * *Files identical despite different names*

### Comparing `indipydriver-1.1.2/indipydriver/events.py` & `indipydriver-1.1.3/indipydriver/events.py`

 * *Files identical despite different names*

### Comparing `indipydriver-1.1.2/indipydriver/ipydriver.py` & `indipydriver-1.1.3/indipydriver/ipydriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,45 +41,43 @@
             # negative is True, if the value is negative
             value = value.strip()
             negative = value.startswith("-")
             if negative:
                 value = value.lstrip("-")
             # Is the number provided in sexagesimal form?
             if value == "":
-                parts = [0, 0, 0]
+                parts = ["0", "0", "0"]
             elif " " in value:
                 parts = value.split(" ")
             elif ":" in value:
                 parts = value.split(":")
             elif ";" in value:
                 parts = value.split(";")
             else:
                 # not sexagesimal
                 parts = [value, "0", "0"]
+            if len(parts) > 3:
+                raise TypeError
             # Any missing parts should have zero
+            if len(parts) == 1:
+                parts.append("0")
+                parts.append("0")
             if len(parts) == 2:
-                # assume seconds are missing, set to zero
                 parts.append("0")
             assert len(parts) == 3
-            number_strings = list(x if x else "0" for x in parts)
-            # convert strings to integers or floats
-            number_list = []
-            for part in number_strings:
-                try:
-                    num = int(part)
-                except ValueError:
-                    num = float(part)
-                number_list.append(num)
-            floatvalue = number_list[0] + (number_list[1]/60) + (number_list[2]/360)
+            # a part could be empty string, ie if 2:5: is given
+            numbers = list(float(x) if x else 0.0 for x in parts)
+            floatvalue = numbers[0] + (numbers[1]/60) + (numbers[2]/3600)
             if negative:
                 floatvalue = -1 * floatvalue
         except:
-            raise TypeError("Unable to parse the value")
+            raise TypeError("Error: Unable to parse number value")
         return floatvalue
 
+
     def __init__(self, devices, tasks=[], **driverdata):
         super().__init__()
 
         # this is a dictionary of device name to device this driver owns
         self.devices = {d.devicename:d for d in devices}
 
         for device in self.devices.values():
```

### Comparing `indipydriver-1.1.2/indipydriver/ipyserver.py` & `indipydriver-1.1.3/indipydriver/ipyserver.py`

 * *Files identical despite different names*

### Comparing `indipydriver-1.1.2/indipydriver/propertymembers.py` & `indipydriver-1.1.3/indipydriver/propertymembers.py`

 * *Files identical despite different names*

### Comparing `indipydriver-1.1.2/indipydriver/propertyvectors.py` & `indipydriver-1.1.3/indipydriver/propertyvectors.py`

 * *Files identical despite different names*

### Comparing `indipydriver-1.1.2/pyproject.toml` & `indipydriver-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indipydriver"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License", "Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "1.1.2"
+version = "1.1.3"
 description="Pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords=['indi', 'driver', 'astronomy', 'instrument']
 
 [project.urls]
 Documentation = "https://indipydriver.readthedocs.io"
```

### Comparing `indipydriver-1.1.2/PKG-INFO` & `indipydriver-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indipydriver
-Version: 1.1.2
+Version: 1.1.3
 Summary: Pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver.
 Keywords: indi,driver,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

