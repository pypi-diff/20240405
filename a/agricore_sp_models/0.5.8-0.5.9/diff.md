# Comparing `tmp/agricore_sp_models-0.5.8.tar.gz` & `tmp/agricore_sp_models-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agricore_sp_models-0.5.8.tar", max compression
+gzip compressed data, was "agricore_sp_models-0.5.9.tar", max compression
```

## Comparing `agricore_sp_models-0.5.8.tar` & `agricore_sp_models-0.5.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       38 2023-12-15 17:13:26.330229 agricore_sp_models-0.5.8/README.md
--rw-r--r--   0        0        0        0 2023-12-15 17:13:26.330229 agricore_sp_models-0.5.8/agricore_sp_models/__init__.py
--rw-r--r--   0        0        0    16922 2023-12-15 17:13:26.330229 agricore_sp_models-0.5.8/agricore_sp_models/abm_interface.py
--rw-r--r--   0        0        0     5388 2023-12-15 17:13:26.330229 agricore_sp_models-0.5.8/agricore_sp_models/agricore_sp_models.py
--rw-r--r--   0        0        0     1922 2023-12-15 17:13:26.330229 agricore_sp_models-0.5.8/agricore_sp_models/logging.py
--rw-r--r--   0        0        0        0 2023-12-15 17:13:26.330229 agricore_sp_models-0.5.8/agricore_sp_models/py.typed
--rw-r--r--   0        0        0     1157 2023-12-15 17:13:26.330229 agricore_sp_models-0.5.8/agricore_sp_models/simulation_models.py
--rw-r--r--   0        0        0      525 2023-12-15 17:13:26.330229 agricore_sp_models-0.5.8/pyproject.toml
--rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 agricore_sp_models-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0       38 2023-12-20 19:04:02.844984 agricore_sp_models-0.5.9/README.md
+-rw-r--r--   0        0        0        0 2023-12-20 19:04:02.844984 agricore_sp_models-0.5.9/agricore_sp_models/__init__.py
+-rw-r--r--   0        0        0    16922 2023-12-20 19:04:02.844984 agricore_sp_models-0.5.9/agricore_sp_models/abm_interface.py
+-rw-r--r--   0        0        0     5520 2023-12-20 19:04:02.844984 agricore_sp_models-0.5.9/agricore_sp_models/agricore_sp_models.py
+-rw-r--r--   0        0        0     1922 2023-12-20 19:04:02.844984 agricore_sp_models-0.5.9/agricore_sp_models/logging.py
+-rw-r--r--   0        0        0        0 2023-12-20 19:04:02.848984 agricore_sp_models-0.5.9/agricore_sp_models/py.typed
+-rw-r--r--   0        0        0     1157 2023-12-20 19:04:02.848984 agricore_sp_models-0.5.9/agricore_sp_models/simulation_models.py
+-rw-r--r--   0        0        0      525 2023-12-20 19:04:02.848984 agricore_sp_models-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 agricore_sp_models-0.5.9/PKG-INFO
```

### Comparing `agricore_sp_models-0.5.8/agricore_sp_models/abm_interface.py` & `agricore_sp_models-0.5.9/agricore_sp_models/abm_interface.py`

 * *Files identical despite different names*

### Comparing `agricore_sp_models-0.5.8/agricore_sp_models/agricore_sp_models.py` & `agricore_sp_models-0.5.9/agricore_sp_models/agricore_sp_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,7 +208,14 @@
     arableProductGroupsNames: List[str]
 
 class IntermediateValueFromLP(BaseModel):
     farmId: int
     averageHAPrice: float
     previousAgriculturalLand: float
     result: dict
+
+class LandTransaction(BaseModel):
+    productionId: int
+    farmId: int
+    yearId: int
+    percentage: float
+    salePrice: float
```

### Comparing `agricore_sp_models-0.5.8/agricore_sp_models/logging.py` & `agricore_sp_models-0.5.9/agricore_sp_models/logging.py`

 * *Files identical despite different names*

### Comparing `agricore_sp_models-0.5.8/agricore_sp_models/simulation_models.py` & `agricore_sp_models-0.5.9/agricore_sp_models/simulation_models.py`

 * *Files identical despite different names*

### Comparing `agricore_sp_models-0.5.8/pyproject.toml` & `agricore_sp_models-0.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agricore_sp_models"
-version = "0.5.8"
+version = "0.5.9"
 description = ""
 authors = [
     "Antonio Gomez <antonio.gomez@idener.es>",
     "Carlos Leyva <carlos.leyva@idener.es>"
 ]
 readme = "README.md"
 repository = "https://github.com/idener/AGRICORE-synthetic-population-models"
```

### Comparing `agricore_sp_models-0.5.8/PKG-INFO` & `agricore_sp_models-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agricore_sp_models
-Version: 0.5.8
+Version: 0.5.9
 Summary: 
 Home-page: https://github.com/idener/AGRICORE-synthetic-population-models
 Author: Antonio Gomez
 Author-email: antonio.gomez@idener.es
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

