# Comparing `tmp/one4all_iop_models-0.1.0.tar.gz` & `tmp/one4all_iop_models-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one4all_iop_models-0.1.0.tar", max compression
+gzip compressed data, was "one4all_iop_models-0.1.1.tar", max compression
```

## Comparing `one4all_iop_models-0.1.0.tar` & `one4all_iop_models-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      364 2024-04-04 08:57:20.944872 one4all_iop_models-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-04 08:57:20.944872 one4all_iop_models-0.1.0/one4all_iop_models/__init__.py
--rw-r--r--   0        0        0     2487 2024-04-04 08:57:20.944872 one4all_iop_models-0.1.0/one4all_iop_models/robot.py
--rw-r--r--   0        0        0      547 2024-04-04 08:57:20.944872 one4all_iop_models-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 one4all_iop_models-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      364 2024-04-05 06:19:55.797106 one4all_iop_models-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 06:19:55.797106 one4all_iop_models-0.1.1/one4all_iop_models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:19:55.797106 one4all_iop_models-0.1.1/one4all_iop_models/ros_models/__init__.py
+-rw-r--r--   0        0        0     2505 2024-04-05 06:19:55.801106 one4all_iop_models-0.1.1/one4all_iop_models/ros_models/robot.py
+-rw-r--r--   0        0        0      547 2024-04-05 06:19:55.801106 one4all_iop_models-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 one4all_iop_models-0.1.1/PKG-INFO
```

### Comparing `one4all_iop_models-0.1.0/one4all_iop_models/robot.py` & `one4all_iop_models-0.1.1/one4all_iop_models/ros_models/robot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-import pandas as pd
-from pydantic import BaseModel, parse_obj_as, Field
 from typing import List, Union
-from datetime import datetime
+
+import pandas as pd
+from pydantic import BaseModel, Field
 
 
-class PositionUpdates (BaseModel):
-    #timestamp: datetime
+class RobotPositionBase (BaseModel):
     PoseWithCovariance_PositionX: float
     PoseWithCovariance_PositionY: float
     PoseWithCovariance_PositionZ: float
     PoseWithCovariance_OrientationX: float
     PoseWithCovariance_OrientationY: float
     PoseWithCovariance_OrientationZ: float
     PoseWithCovariance_OrientationW: float
@@ -33,57 +32,65 @@
     Path_OrientationY: List[float]
     Path_OrientationZ: List[float]
     Path_OrientationW: List[float]
 
     @classmethod
     def from_dataframe(cls, df: pd.DataFrame):
         parsed_data = df.to_dict(orient='records')
-        return parse_obj_as(List[PositionUpdates], parsed_data)
-    
+        models = []
+        for row in parsed_data:
+            model = cls(**row)
+            models.append(model)
+        return models
+
 
 class RobotActionBase(BaseModel):
     name: str
 
+
 class AWCombo(RobotActionBase):
     x: float = Field(ge=-5, le=5)
     y: float = Field(ge=-5, le=5)
     angle: float = Field(ge=0, le=360)
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.name = "awcombo"
 
+
 class Joint(RobotActionBase):
     j1: float = Field(ge=-1, le=1)
     j2: float = Field(ge=-1, le=1)
     j3: float = Field(ge=-1, le=1)
     j4: float = Field(ge=-1, le=1)
     j5: float = Field(ge=-1, le=1)
     j6: float = Field(ge=-1, le=1)
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.name = "joint"
 
+
 class Carte(RobotActionBase):
     x: float = Field(ge=-1, le=1)
     y: float = Field(ge=-1, le=1)
     z: float = Field(ge=-1, le=1)
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.name = "carte"
 
+
 class Increm(RobotActionBase):
-    axis: str = Field(choices=["x","y","z"])
+    axis: str = Field(choices=["x", "y", "z"])
     delta: float
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.name = "increm"
 
-RobotActionsTypes = Union[Increm,AWCombo,Carte]
 
-class SubTask(BaseModel):
-    actions: List[RobotActionsTypes]
+RobotActionsTypes = Union[Increm, AWCombo, Carte, Joint]
 
 
+class SubTask(BaseModel):
+    actions: List[RobotActionsTypes]
```

### Comparing `one4all_iop_models-0.1.0/pyproject.toml` & `one4all_iop_models-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "one4all-iop-models"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Ignacio Jimenez <ignacio.jimenez@idener.ai>"]
 readme = "README.md"
 packages = [{include = "one4all_iop_models"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `one4all_iop_models-0.1.0/PKG-INFO` & `one4all_iop_models-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one4all-iop-models
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Ignacio Jimenez
 Author-email: ignacio.jimenez@idener.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

