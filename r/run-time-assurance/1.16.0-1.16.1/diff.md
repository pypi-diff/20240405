# Comparing `tmp/run_time_assurance-1.16.0.tar.gz` & `tmp/run_time_assurance-1.16.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "run_time_assurance-1.16.0.tar", max compression
+gzip compressed data, was "run_time_assurance-1.16.1.tar", max compression
```

## Comparing `run_time_assurance-1.16.0.tar` & `run_time_assurance-1.16.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0       34 2024-03-26 14:40:37.592849 run_time_assurance-1.16.0/LICENSE
--rw-r--r--   0        0        0     4153 2024-03-26 14:40:37.592849 run_time_assurance-1.16.0/README.md
--rw-r--r--   0        0        0     3434 2024-03-26 14:40:37.592849 run_time_assurance-1.16.0/docs/RTA/asif.md
--rw-r--r--   0        0        0     1417 2024-03-26 14:40:37.592849 run_time_assurance-1.16.0/docs/RTA/discrete_asif.md
--rw-r--r--   0        0        0     2132 2024-03-26 14:40:37.592849 run_time_assurance-1.16.0/docs/RTA/explicit_asif.md
--rw-r--r--   0        0        0      917 2024-03-26 14:40:37.592849 run_time_assurance-1.16.0/docs/RTA/explicit_simplex.md
--rw-r--r--   0        0        0    17624 2024-03-26 14:40:37.656850 run_time_assurance-1.16.0/docs/RTA/figures/Optimization.png
--rw-r--r--   0        0        0     6706 2024-03-26 14:40:37.656850 run_time_assurance-1.16.0/docs/RTA/figures/RTA_Filter.png
--rw-r--r--   0        0        0    18606 2024-03-26 14:40:37.656850 run_time_assurance-1.16.0/docs/RTA/figures/Switching.png
--rw-r--r--   0        0        0     1768 2024-03-26 14:40:37.656850 run_time_assurance-1.16.0/docs/RTA/implicit_asif.md
--rw-r--r--   0        0        0      974 2024-03-26 14:40:37.656850 run_time_assurance-1.16.0/docs/RTA/implicit_simplex.md
--rw-r--r--   0        0        0     2030 2024-03-26 14:40:37.656850 run_time_assurance-1.16.0/docs/RTA/index.md
--rw-r--r--   0        0        0     3656 2024-03-26 14:40:37.656850 run_time_assurance-1.16.0/docs/RTA/safety.md
--rw-r--r--   0        0        0     1233 2024-03-26 14:40:37.656850 run_time_assurance-1.16.0/docs/RTA/simplex.md
--rw-r--r--   0        0        0      181 2024-03-26 14:40:37.656850 run_time_assurance-1.16.0/docs/api/index.md
--rw-r--r--   0        0        0      257 2024-03-26 14:40:37.656850 run_time_assurance-1.16.0/docs/api/rta/index.md
--rw-r--r--   0        0        0      201 2024-03-26 14:40:37.656850 run_time_assurance-1.16.0/docs/api/utils/index.md
--rw-r--r--   0        0        0      465 2024-03-26 14:40:37.656850 run_time_assurance-1.16.0/docs/api/zoo/cwh/index.md
--rw-r--r--   0        0        0      200 2024-03-26 14:40:37.656850 run_time_assurance-1.16.0/docs/api/zoo/index.md
--rw-r--r--   0        0        0      154 2024-03-26 14:40:37.656850 run_time_assurance-1.16.0/docs/api/zoo/integrators/index.md
--rw-r--r--   0        0        0     1304 2024-03-26 14:40:37.656850 run_time_assurance-1.16.0/docs/developer-guide.md
--rw-r--r--   0        0        0      671 2024-03-26 14:40:37.656850 run_time_assurance-1.16.0/docs/gen_ref_nav.py
--rw-r--r--   0        0        0       44 2024-03-26 14:40:37.656850 run_time_assurance-1.16.0/docs/index.md
--rw-r--r--   0        0        0     1802 2024-03-26 14:40:37.656850 run_time_assurance-1.16.0/docs/install.md
--rw-r--r--   0        0        0      685 2024-03-26 14:40:37.660850 run_time_assurance-1.16.0/docs/usage.md
--rw-r--r--   0        0        0     1970 2024-03-26 14:40:37.660850 run_time_assurance-1.16.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-26 14:40:37.660850 run_time_assurance-1.16.0/run_time_assurance/__init__.py
--rw-r--r--   0        0        0    20465 2024-03-26 14:40:37.660850 run_time_assurance-1.16.0/run_time_assurance/constraint.py
--rw-r--r--   0        0        0     7040 2024-03-26 14:40:37.660850 run_time_assurance-1.16.0/run_time_assurance/controller.py
--rw-r--r--   0        0        0      467 2024-03-26 14:40:37.660850 run_time_assurance-1.16.0/run_time_assurance/rta/__init__.py
--rw-r--r--   0        0        0    44412 2024-03-26 14:40:37.660850 run_time_assurance-1.16.0/run_time_assurance/rta/asif.py
--rw-r--r--   0        0        0    15970 2024-03-26 14:40:37.660850 run_time_assurance-1.16.0/run_time_assurance/rta/base.py
--rw-r--r--   0        0        0    11573 2024-03-26 14:40:37.660850 run_time_assurance-1.16.0/run_time_assurance/rta/simplex.py
--rw-r--r--   0        0        0      697 2024-03-26 14:40:37.660850 run_time_assurance-1.16.0/run_time_assurance/state.py
--rw-r--r--   0        0        0       98 2024-03-26 14:40:37.660850 run_time_assurance-1.16.0/run_time_assurance/utils/__init__.py
--rw-r--r--   0        0        0    13390 2024-03-26 14:40:37.660850 run_time_assurance-1.16.0/run_time_assurance/utils/sample_testing.py
--rw-r--r--   0        0        0     2527 2024-03-26 14:40:37.660850 run_time_assurance-1.16.0/run_time_assurance/utils/utils.py
--rw-r--r--   0        0        0        0 2024-03-26 14:40:37.660850 run_time_assurance-1.16.0/run_time_assurance/zoo/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 14:40:37.660850 run_time_assurance-1.16.0/run_time_assurance/zoo/cwh/__init__.py
--rw-r--r--   0        0        0    22566 2024-03-26 14:40:37.660850 run_time_assurance-1.16.0/run_time_assurance/zoo/cwh/docking_2d.py
--rw-r--r--   0        0        0    23795 2024-03-26 14:40:37.660850 run_time_assurance-1.16.0/run_time_assurance/zoo/cwh/docking_3d.py
--rw-r--r--   0        0        0    35628 2024-03-26 14:40:37.660850 run_time_assurance-1.16.0/run_time_assurance/zoo/cwh/inspection_1v1.py
--rw-r--r--   0        0        0    18340 2024-03-26 14:40:37.660850 run_time_assurance-1.16.0/run_time_assurance/zoo/cwh/inspection_3d.py
--rw-r--r--   0        0        0     3522 2024-03-26 14:40:37.664850 run_time_assurance-1.16.0/run_time_assurance/zoo/cwh/random_sample_testing.py
--rw-r--r--   0        0        0        0 2024-03-26 14:40:37.664850 run_time_assurance-1.16.0/run_time_assurance/zoo/integrators/__init__.py
--rw-r--r--   0        0        0    14723 2024-03-26 14:40:37.664850 run_time_assurance-1.16.0/run_time_assurance/zoo/integrators/integrator_1d.py
--rw-r--r--   0        0        0     5246 1970-01-01 00:00:00.000000 run_time_assurance-1.16.0/PKG-INFO
+-rw-r--r--   0        0        0       34 2024-04-05 19:44:43.939876 run_time_assurance-1.16.1/LICENSE
+-rw-r--r--   0        0        0     4153 2024-04-05 19:44:43.939876 run_time_assurance-1.16.1/README.md
+-rw-r--r--   0        0        0     3434 2024-04-05 19:44:43.943876 run_time_assurance-1.16.1/docs/RTA/asif.md
+-rw-r--r--   0        0        0     1417 2024-04-05 19:44:43.943876 run_time_assurance-1.16.1/docs/RTA/discrete_asif.md
+-rw-r--r--   0        0        0     2132 2024-04-05 19:44:43.943876 run_time_assurance-1.16.1/docs/RTA/explicit_asif.md
+-rw-r--r--   0        0        0      917 2024-04-05 19:44:43.943876 run_time_assurance-1.16.1/docs/RTA/explicit_simplex.md
+-rw-r--r--   0        0        0    17624 2024-04-05 19:44:44.599869 run_time_assurance-1.16.1/docs/RTA/figures/Optimization.png
+-rw-r--r--   0        0        0     6706 2024-04-05 19:44:44.599869 run_time_assurance-1.16.1/docs/RTA/figures/RTA_Filter.png
+-rw-r--r--   0        0        0    18606 2024-04-05 19:44:44.599869 run_time_assurance-1.16.1/docs/RTA/figures/Switching.png
+-rw-r--r--   0        0        0     1768 2024-04-05 19:44:44.603869 run_time_assurance-1.16.1/docs/RTA/implicit_asif.md
+-rw-r--r--   0        0        0      974 2024-04-05 19:44:44.603869 run_time_assurance-1.16.1/docs/RTA/implicit_simplex.md
+-rw-r--r--   0        0        0     2030 2024-04-05 19:44:44.603869 run_time_assurance-1.16.1/docs/RTA/index.md
+-rw-r--r--   0        0        0     3656 2024-04-05 19:44:44.603869 run_time_assurance-1.16.1/docs/RTA/safety.md
+-rw-r--r--   0        0        0     1233 2024-04-05 19:44:44.603869 run_time_assurance-1.16.1/docs/RTA/simplex.md
+-rw-r--r--   0        0        0      181 2024-04-05 19:44:44.603869 run_time_assurance-1.16.1/docs/api/index.md
+-rw-r--r--   0        0        0      257 2024-04-05 19:44:44.603869 run_time_assurance-1.16.1/docs/api/rta/index.md
+-rw-r--r--   0        0        0      201 2024-04-05 19:44:44.603869 run_time_assurance-1.16.1/docs/api/utils/index.md
+-rw-r--r--   0        0        0      465 2024-04-05 19:44:44.603869 run_time_assurance-1.16.1/docs/api/zoo/cwh/index.md
+-rw-r--r--   0        0        0      200 2024-04-05 19:44:44.603869 run_time_assurance-1.16.1/docs/api/zoo/index.md
+-rw-r--r--   0        0        0      154 2024-04-05 19:44:44.603869 run_time_assurance-1.16.1/docs/api/zoo/integrators/index.md
+-rw-r--r--   0        0        0     1304 2024-04-05 19:44:44.603869 run_time_assurance-1.16.1/docs/developer-guide.md
+-rw-r--r--   0        0        0      671 2024-04-05 19:44:44.603869 run_time_assurance-1.16.1/docs/gen_ref_nav.py
+-rw-r--r--   0        0        0       44 2024-04-05 19:44:44.603869 run_time_assurance-1.16.1/docs/index.md
+-rw-r--r--   0        0        0     1802 2024-04-05 19:44:44.603869 run_time_assurance-1.16.1/docs/install.md
+-rw-r--r--   0        0        0      685 2024-04-05 19:44:44.603869 run_time_assurance-1.16.1/docs/usage.md
+-rw-r--r--   0        0        0     2001 2024-04-05 19:44:44.603869 run_time_assurance-1.16.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-05 19:44:44.603869 run_time_assurance-1.16.1/run_time_assurance/__init__.py
+-rw-r--r--   0        0        0    20465 2024-04-05 19:44:44.603869 run_time_assurance-1.16.1/run_time_assurance/constraint.py
+-rw-r--r--   0        0        0     7040 2024-04-05 19:44:44.603869 run_time_assurance-1.16.1/run_time_assurance/controller.py
+-rw-r--r--   0        0        0      467 2024-04-05 19:44:44.603869 run_time_assurance-1.16.1/run_time_assurance/rta/__init__.py
+-rw-r--r--   0        0        0    44412 2024-04-05 19:44:44.603869 run_time_assurance-1.16.1/run_time_assurance/rta/asif.py
+-rw-r--r--   0        0        0    15970 2024-04-05 19:44:44.607869 run_time_assurance-1.16.1/run_time_assurance/rta/base.py
+-rw-r--r--   0        0        0    11573 2024-04-05 19:44:44.607869 run_time_assurance-1.16.1/run_time_assurance/rta/simplex.py
+-rw-r--r--   0        0        0      697 2024-04-05 19:44:44.607869 run_time_assurance-1.16.1/run_time_assurance/state.py
+-rw-r--r--   0        0        0       98 2024-04-05 19:44:44.607869 run_time_assurance-1.16.1/run_time_assurance/utils/__init__.py
+-rw-r--r--   0        0        0    13390 2024-04-05 19:44:44.607869 run_time_assurance-1.16.1/run_time_assurance/utils/sample_testing.py
+-rw-r--r--   0        0        0     2527 2024-04-05 19:44:44.607869 run_time_assurance-1.16.1/run_time_assurance/utils/utils.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:44:44.607869 run_time_assurance-1.16.1/run_time_assurance/zoo/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:44:44.607869 run_time_assurance-1.16.1/run_time_assurance/zoo/cwh/__init__.py
+-rw-r--r--   0        0        0    22566 2024-04-05 19:44:44.607869 run_time_assurance-1.16.1/run_time_assurance/zoo/cwh/docking_2d.py
+-rw-r--r--   0        0        0    23795 2024-04-05 19:44:44.607869 run_time_assurance-1.16.1/run_time_assurance/zoo/cwh/docking_3d.py
+-rw-r--r--   0        0        0    35628 2024-04-05 19:44:44.607869 run_time_assurance-1.16.1/run_time_assurance/zoo/cwh/inspection_1v1.py
+-rw-r--r--   0        0        0    18340 2024-04-05 19:44:44.607869 run_time_assurance-1.16.1/run_time_assurance/zoo/cwh/inspection_3d.py
+-rw-r--r--   0        0        0     3522 2024-04-05 19:44:44.607869 run_time_assurance-1.16.1/run_time_assurance/zoo/cwh/random_sample_testing.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:44:44.607869 run_time_assurance-1.16.1/run_time_assurance/zoo/integrators/__init__.py
+-rw-r--r--   0        0        0    14723 2024-04-05 19:44:44.607869 run_time_assurance-1.16.1/run_time_assurance/zoo/integrators/integrator_1d.py
+-rw-r--r--   0        0        0     5252 1970-01-01 00:00:00.000000 run_time_assurance-1.16.1/PKG-INFO
```

### Comparing `run_time_assurance-1.16.0/README.md` & `run_time_assurance-1.16.1/README.md`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/docs/RTA/asif.md` & `run_time_assurance-1.16.1/docs/RTA/asif.md`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/docs/RTA/discrete_asif.md` & `run_time_assurance-1.16.1/docs/RTA/discrete_asif.md`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/docs/RTA/explicit_asif.md` & `run_time_assurance-1.16.1/docs/RTA/explicit_asif.md`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/docs/RTA/explicit_simplex.md` & `run_time_assurance-1.16.1/docs/RTA/explicit_simplex.md`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/docs/RTA/figures/Optimization.png` & `run_time_assurance-1.16.1/docs/RTA/figures/Optimization.png`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/docs/RTA/figures/RTA_Filter.png` & `run_time_assurance-1.16.1/docs/RTA/figures/RTA_Filter.png`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/docs/RTA/figures/Switching.png` & `run_time_assurance-1.16.1/docs/RTA/figures/Switching.png`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/docs/RTA/implicit_asif.md` & `run_time_assurance-1.16.1/docs/RTA/implicit_asif.md`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/docs/RTA/implicit_simplex.md` & `run_time_assurance-1.16.1/docs/RTA/implicit_simplex.md`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/docs/RTA/index.md` & `run_time_assurance-1.16.1/docs/RTA/index.md`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/docs/RTA/safety.md` & `run_time_assurance-1.16.1/docs/RTA/safety.md`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/docs/RTA/simplex.md` & `run_time_assurance-1.16.1/docs/RTA/simplex.md`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/docs/developer-guide.md` & `run_time_assurance-1.16.1/docs/developer-guide.md`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/docs/gen_ref_nav.py` & `run_time_assurance-1.16.1/docs/gen_ref_nav.py`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/docs/install.md` & `run_time_assurance-1.16.1/docs/install.md`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/docs/usage.md` & `run_time_assurance-1.16.1/docs/usage.md`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/pyproject.toml` & `run_time_assurance-1.16.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "run-time-assurance"
-version = "1.16.0"
+version = "1.16.1"
 description = "The run-time-assurance library provides an interface and implementations for Run Time Assurance (RTA) safety filters."
 authors = [
     "Charles Keating <Charles.Keating@udri.udayton.edu>",
 ]
 license = ""
 readme = "README.md"
 homepage = "https://github.com/act3-ace/run-time-assurance.git"
@@ -19,16 +19,16 @@
 packages = [
         {include = "run_time_assurance"},
     ]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.13"
 scipy = ">=1.10.0"
-safe-autonomy-dynamics = "^1.2.0"
-jax = { version = "0.4.3", extras = ["cpu"] }
+safe-autonomy-dynamics = { version="^1.2.0", extras = ["jax"] }
+jax = { version = "0.4.26", extras = ["cpu"] }
 numpy = "^1.23.5"
 matplotlib = "^3.8.0"
 quadprog = "^0.1.11"
 
 [tool.poetry.group.lint.dependencies]
 pylint = "2.15.4"
 flake8 = "3.9.2"
```

### Comparing `run_time_assurance-1.16.0/run_time_assurance/constraint.py` & `run_time_assurance-1.16.1/run_time_assurance/constraint.py`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/run_time_assurance/controller.py` & `run_time_assurance-1.16.1/run_time_assurance/controller.py`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/run_time_assurance/rta/asif.py` & `run_time_assurance-1.16.1/run_time_assurance/rta/asif.py`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/run_time_assurance/rta/base.py` & `run_time_assurance-1.16.1/run_time_assurance/rta/base.py`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/run_time_assurance/rta/simplex.py` & `run_time_assurance-1.16.1/run_time_assurance/rta/simplex.py`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/run_time_assurance/state.py` & `run_time_assurance-1.16.1/run_time_assurance/state.py`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/run_time_assurance/utils/sample_testing.py` & `run_time_assurance-1.16.1/run_time_assurance/utils/sample_testing.py`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/run_time_assurance/utils/utils.py` & `run_time_assurance-1.16.1/run_time_assurance/utils/utils.py`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/run_time_assurance/zoo/cwh/docking_2d.py` & `run_time_assurance-1.16.1/run_time_assurance/zoo/cwh/docking_2d.py`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/run_time_assurance/zoo/cwh/docking_3d.py` & `run_time_assurance-1.16.1/run_time_assurance/zoo/cwh/docking_3d.py`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/run_time_assurance/zoo/cwh/inspection_1v1.py` & `run_time_assurance-1.16.1/run_time_assurance/zoo/cwh/inspection_1v1.py`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/run_time_assurance/zoo/cwh/inspection_3d.py` & `run_time_assurance-1.16.1/run_time_assurance/zoo/cwh/inspection_3d.py`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/run_time_assurance/zoo/cwh/random_sample_testing.py` & `run_time_assurance-1.16.1/run_time_assurance/zoo/cwh/random_sample_testing.py`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/run_time_assurance/zoo/integrators/integrator_1d.py` & `run_time_assurance-1.16.1/run_time_assurance/zoo/integrators/integrator_1d.py`

 * *Files identical despite different names*

### Comparing `run_time_assurance-1.16.0/PKG-INFO` & `run_time_assurance-1.16.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: run-time-assurance
-Version: 1.16.0
+Version: 1.16.1
 Summary: The run-time-assurance library provides an interface and implementations for Run Time Assurance (RTA) safety filters.
 Home-page: https://github.com/act3-ace/run-time-assurance.git
 Author: Charles Keating
 Author-email: Charles.Keating@udri.udayton.edu
 Requires-Python: >=3.9,<3.13
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: jax[cpu] (==0.4.3)
+Requires-Dist: jax[cpu] (==0.4.26)
 Requires-Dist: matplotlib (>=3.8.0,<4.0.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: quadprog (>=0.1.11,<0.2.0)
-Requires-Dist: safe-autonomy-dynamics (>=1.2.0,<2.0.0)
+Requires-Dist: safe-autonomy-dynamics[jax] (>=1.2.0,<2.0.0)
 Requires-Dist: scipy (>=1.10.0)
 Project-URL: Documentation, https://github.com/act3-ace/run-time-assurance/docs
 Project-URL: Repository, https://github.com/act3-ace/run-time-assurance.git
 Description-Content-Type: text/markdown
 
 # Run Time Assurance
```

