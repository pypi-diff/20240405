# Comparing `tmp/one4all_iop_models-0.1.2.tar.gz` & `tmp/one4all_iop_models-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one4all_iop_models-0.1.2.tar", max compression
+gzip compressed data, was "one4all_iop_models-0.1.3.tar", max compression
```

## Comparing `one4all_iop_models-0.1.2.tar` & `one4all_iop_models-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      364 2024-04-05 10:37:33.308274 one4all_iop_models-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-04-05 10:37:33.308274 one4all_iop_models-0.1.2/one4all_iop_models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 10:37:33.308274 one4all_iop_models-0.1.2/one4all_iop_models/ros_models/__init__.py
--rw-r--r--   0        0        0     2891 2024-04-05 10:37:33.308274 one4all_iop_models-0.1.2/one4all_iop_models/ros_models/robot.py
--rw-r--r--   0        0        0      547 2024-04-05 10:37:33.308274 one4all_iop_models-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 one4all_iop_models-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      364 2024-04-05 11:00:15.355243 one4all_iop_models-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 11:00:15.355243 one4all_iop_models-0.1.3/one4all_iop_models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 11:00:15.355243 one4all_iop_models-0.1.3/one4all_iop_models/ros_models/__init__.py
+-rw-r--r--   0        0        0     2892 2024-04-05 11:00:15.359243 one4all_iop_models-0.1.3/one4all_iop_models/ros_models/robot.py
+-rw-r--r--   0        0        0      547 2024-04-05 11:00:15.359243 one4all_iop_models-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 one4all_iop_models-0.1.3/PKG-INFO
```

### Comparing `one4all_iop_models-0.1.2/one4all_iop_models/ros_models/robot.py` & `one4all_iop_models-0.1.3/one4all_iop_models/ros_models/robot.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     name: str = "carte"
     x: float = confloat(ge=-1, le=1)
     y: float = confloat(ge=-1, le=1)
     z: float = confloat(ge=-1, le=1)
 
     @validator('name')
     def validate_name(cls, v):
-        if v != "joint":
+        if v != "carte":
             raise ValueError("name must be 'carte'")
         return v
 
     def __init__(self, x, y, z):
         self.x = x
         self.y = y
         self.z = z
@@ -91,15 +91,15 @@
 class Increm(RobotActionBase):
     name: str = "increm"
     axis: Literal["x", "y", "z"]
     delta: float
 
     @validator('name')
     def validate_name(cls, v):
-        if v != "joint":
+        if v != "increm":
             raise ValueError("name must be 'increm'")
         return v
 
     def __init__(self, axis, delta):
         self.axis = axis
         self.delta = delta
```

### Comparing `one4all_iop_models-0.1.2/pyproject.toml` & `one4all_iop_models-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "one4all-iop-models"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Ignacio Jimenez <ignacio.jimenez@idener.ai>"]
 readme = "README.md"
 packages = [{include = "one4all_iop_models"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `one4all_iop_models-0.1.2/PKG-INFO` & `one4all_iop_models-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one4all-iop-models
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Ignacio Jimenez
 Author-email: ignacio.jimenez@idener.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

