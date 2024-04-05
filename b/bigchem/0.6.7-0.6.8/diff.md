# Comparing `tmp/bigchem-0.6.7.tar.gz` & `tmp/bigchem-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigchem-0.6.7.tar", max compression
+gzip compressed data, was "bigchem-0.6.8.tar", max compression
```

## Comparing `bigchem-0.6.7.tar` & `bigchem-0.6.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1079 2024-03-30 00:07:12.369462 bigchem-0.6.7/LICENSE
--rw-r--r--   0        0        0    39427 2024-03-30 00:07:12.369462 bigchem-0.6.7/README.md
--rw-r--r--   0        0        0      213 2024-03-30 00:07:12.373462 bigchem-0.6.7/bigchem/__init__.py
--rw-r--r--   0        0        0     4068 2024-03-30 00:07:12.373462 bigchem-0.6.7/bigchem/algos.py
--rw-r--r--   0        0        0     1540 2024-03-30 00:07:12.373462 bigchem-0.6.7/bigchem/app.py
--rw-r--r--   0        0        0      164 2024-03-30 00:07:12.373462 bigchem-0.6.7/bigchem/canvas.py
--rw-r--r--   0        0        0     1982 2024-03-30 00:07:12.373462 bigchem-0.6.7/bigchem/config.py
--rw-r--r--   0        0        0     6718 2024-03-30 00:07:12.373462 bigchem-0.6.7/bigchem/tasks.py
--rw-r--r--   0        0        0     1504 2024-03-30 00:07:12.373462 bigchem-0.6.7/bigchem/utils.py
--rw-r--r--   0        0        0     1912 2024-03-30 00:07:12.373462 bigchem-0.6.7/pyproject.toml
--rw-r--r--   0        0        0    40419 1970-01-01 00:00:00.000000 bigchem-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-05 21:10:21.632775 bigchem-0.6.8/LICENSE
+-rw-r--r--   0        0        0    39427 2024-04-05 21:10:21.632775 bigchem-0.6.8/README.md
+-rw-r--r--   0        0        0      213 2024-04-05 21:10:21.632775 bigchem-0.6.8/bigchem/__init__.py
+-rw-r--r--   0        0        0     4093 2024-04-05 21:10:21.632775 bigchem-0.6.8/bigchem/algos.py
+-rw-r--r--   0        0        0     1540 2024-04-05 21:10:21.632775 bigchem-0.6.8/bigchem/app.py
+-rw-r--r--   0        0        0      164 2024-04-05 21:10:21.632775 bigchem-0.6.8/bigchem/canvas.py
+-rw-r--r--   0        0        0     1982 2024-04-05 21:10:21.636775 bigchem-0.6.8/bigchem/config.py
+-rw-r--r--   0        0        0     6718 2024-04-05 21:10:21.636775 bigchem-0.6.8/bigchem/tasks.py
+-rw-r--r--   0        0        0     1504 2024-04-05 21:10:21.636775 bigchem-0.6.8/bigchem/utils.py
+-rw-r--r--   0        0        0     1909 2024-04-05 21:10:21.636775 bigchem-0.6.8/pyproject.toml
+-rw-r--r--   0        0        0    40441 1970-01-01 00:00:00.000000 bigchem-0.6.8/PKG-INFO
```

### Comparing `bigchem-0.6.7/LICENSE` & `bigchem-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bigchem-0.6.7/README.md` & `bigchem-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `bigchem-0.6.7/bigchem/algos.py` & `bigchem-0.6.8/bigchem/algos.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,16 @@
     Params:
         program: Program to use for gradient calculations to generate hessian
         prog_input: ProgramInput object.
         dh: Displacement for finite difference computation of hessian
         kwargs: Keywords passed to geomeTRIC's frequency_analysis function
             temperature: float - Temperature passed to the harmonic free energy module;
                 default: 300.0
-            pressure: float - Pressure passed to the harmonic free energy module;
+            pressure: float - Pressure passed to the harmonic free energy module (in
+                bar);
                 default: 1.0
 
     """
     hessian_inp = prog_input.model_dump()
     # So parallel_hessian doesn't raise error
     hessian_inp["calctype"] = CalcType.hessian
     hessian_sig = parallel_hessian(program, ProgramInput(**hessian_inp), dh)
```

### Comparing `bigchem-0.6.7/bigchem/app.py` & `bigchem-0.6.8/bigchem/app.py`

 * *Files identical despite different names*

### Comparing `bigchem-0.6.7/bigchem/config.py` & `bigchem-0.6.8/bigchem/config.py`

 * *Files identical despite different names*

### Comparing `bigchem-0.6.7/bigchem/tasks.py` & `bigchem-0.6.8/bigchem/tasks.py`

 * *Files identical despite different names*

### Comparing `bigchem-0.6.7/bigchem/utils.py` & `bigchem-0.6.8/bigchem/utils.py`

 * *Files identical despite different names*

### Comparing `bigchem-0.6.7/pyproject.toml` & `bigchem-0.6.8/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "bigchem"
-version = "0.6.7"
+version = "0.6.8"
 description = "A distributed system for scaling and parallelizing quantum chemistry calculations"
 authors = ["Colton Hicks <github@coltonhicks.com>"]
 readme = "README.md"
 homepage = "https://github.com/mtzgroup/bigchem"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
-celery = { extras = ["redis"], version = "^5.2.7" }
-pydantic = ">=2.0.0"
+celery = { version = "^5.3.4", extras = ["redis"] }
+pydantic = "^2.0.0"
 qcio = ">=0.8.1"
 pydantic-settings = "^2.0.3"
 # A list of all of the optional dependencies, some of which are included in the below
 # `extras`. They can be opted into by apps. Clients should not need to install these.
-geometric = { version = ">=1.0.1", optional = true }
-qcengine = { version = ">=0.27.0", optional = true }
+geometric = { version = "^1.0.1", optional = true }
+qcengine = { version = "^0.27.0", optional = true }
 qcop = ">=0.5.1"
 
 [tool.poetry.extras]
 geometric = ["geometric"]
 qcengine = ["qcengine"]
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `bigchem-0.6.7/PKG-INFO` & `bigchem-0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: bigchem
-Version: 0.6.7
+Version: 0.6.8
 Summary: A distributed system for scaling and parallelizing quantum chemistry calculations
 Home-page: https://github.com/mtzgroup/bigchem
 License: MIT
 Author: Colton Hicks
 Author-email: github@coltonhicks.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: geometric
 Provides-Extra: qcengine
-Requires-Dist: celery[redis] (>=5.2.7,<6.0.0)
-Requires-Dist: geometric (>=1.0.1) ; extra == "geometric"
-Requires-Dist: pydantic (>=2.0.0)
+Requires-Dist: celery[redis] (>=5.3.4,<6.0.0)
+Requires-Dist: geometric (>=1.0.1,<2.0.0) ; extra == "geometric"
+Requires-Dist: pydantic (>=2.0.0,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.0.3,<3.0.0)
-Requires-Dist: qcengine (>=0.27.0) ; extra == "qcengine"
+Requires-Dist: qcengine (>=0.27.0,<0.28.0) ; extra == "qcengine"
 Requires-Dist: qcio (>=0.8.1)
 Requires-Dist: qcop (>=0.5.1)
 Description-Content-Type: text/markdown
 
 # BigChem
 
 A distributed system for scaling and parallelizing quantum chemistry calculations.
```

