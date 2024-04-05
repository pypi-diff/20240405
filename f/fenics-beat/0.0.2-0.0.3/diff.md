# Comparing `tmp/fenics-beat-0.0.2.tar.gz` & `tmp/fenics-beat-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenics-beat-0.0.2.tar", last modified: Mon Oct 23 08:41:35 2023, max compression
+gzip compressed data, was "fenics-beat-0.0.3.tar", last modified: Fri Apr  5 11:50:22 2024, max compression
```

## Comparing `fenics-beat-0.0.2.tar` & `fenics-beat-0.0.3.tar`

### file list

```diff
@@ -1,33 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 08:41:35.197661 fenics-beat-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-10-23 08:41:24.000000 fenics-beat-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2023-10-23 08:41:35.197661 fenics-beat-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      450 2023-10-23 08:41:24.000000 fenics-beat-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2023-10-23 08:41:24.000000 fenics-beat-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-23 08:41:35.197661 fenics-beat-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 08:41:35.189661 fenics-beat-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 08:41:35.193661 fenics-beat-0.0.2/src/beat/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2023-10-23 08:41:24.000000 fenics-beat-0.0.2/src/beat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9635 2023-10-23 08:41:24.000000 fenics-beat-0.0.2/src/beat/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2023-10-23 08:41:24.000000 fenics-beat-0.0.2/src/beat/bidomain_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 08:41:35.193661 fenics-beat-0.0.2/src/beat/cellmodels/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2023-10-23 08:41:24.000000 fenics-beat-0.0.2/src/beat/cellmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14596 2023-10-23 08:41:24.000000 fenics-beat-0.0.2/src/beat/cellmodels/beeler_reuter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8723 2023-10-23 08:41:24.000000 fenics-beat-0.0.2/src/beat/cellmodels/fitzhughnagumo.py
--rw-r--r--   0 runner    (1001) docker     (127)    70034 2023-10-23 08:41:24.000000 fenics-beat-0.0.2/src/beat/cellmodels/tentusscher_panfilov_2006_M_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)    70699 2023-10-23 08:41:24.000000 fenics-beat-0.0.2/src/beat/cellmodels/tentusscher_panfilov_2006_epi_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2023-10-23 08:41:24.000000 fenics-beat-0.0.2/src/beat/ecg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2023-10-23 08:41:24.000000 fenics-beat-0.0.2/src/beat/monodomain_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2023-10-23 08:41:24.000000 fenics-beat-0.0.2/src/beat/monodomain_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2023-10-23 08:41:24.000000 fenics-beat-0.0.2/src/beat/odesolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 08:41:35.193661 fenics-beat-0.0.2/src/fenics_beat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2023-10-23 08:41:35.000000 fenics-beat-0.0.2/src/fenics_beat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      743 2023-10-23 08:41:35.000000 fenics-beat-0.0.2/src/fenics_beat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-23 08:41:35.000000 fenics-beat-0.0.2/src/fenics_beat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      277 2023-10-23 08:41:35.000000 fenics-beat-0.0.2/src/fenics_beat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-23 08:41:35.000000 fenics-beat-0.0.2/src/fenics_beat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 08:41:35.197661 fenics-beat-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2023-10-23 08:41:24.000000 fenics-beat-0.0.2/tests/test_bidomain_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2023-10-23 08:41:24.000000 fenics-beat-0.0.2/tests/test_ecg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2023-10-23 08:41:24.000000 fenics-beat-0.0.2/tests/test_monodomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2023-10-23 08:41:24.000000 fenics-beat-0.0.2/tests/test_monodomain_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2023-10-23 08:41:24.000000 fenics-beat-0.0.2/tests/test_odesolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:22.547421 fenics-beat-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-05 11:50:22.547421 fenics-beat-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 11:50:22.547421 fenics-beat-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:22.539420 fenics-beat-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:22.539420 fenics-beat-0.0.3/src/beat/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/bidomain_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:22.539420 fenics-beat-0.0.3/src/beat/cellmodels/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/cellmodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22810 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/cellmodels/beeler_reuter_1977.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8725 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/cellmodels/fitzhughnagumo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:22.543420 fenics-beat-0.0.3/src/beat/cellmodels/tentusscher_panfilov_2006/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/cellmodels/tentusscher_panfilov_2006/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69974 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/cellmodels/tentusscher_panfilov_2006/endo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70079 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/cellmodels/tentusscher_panfilov_2006/epi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70062 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/cellmodels/tentusscher_panfilov_2006/mid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:22.543420 fenics-beat-0.0.3/src/beat/cellmodels/torord_dyn_chloride/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/cellmodels/torord_dyn_chloride/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   294950 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/cellmodels/torord_dyn_chloride/endo.py
+-rw-r--r--   0 runner    (1001) docker     (127)   294986 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/cellmodels/torord_dyn_chloride/epi.py
+-rw-r--r--   0 runner    (1001) docker     (127)   294943 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/cellmodels/torord_dyn_chloride/mid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/ecg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/monodomain_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/monodomain_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7433 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/odesolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/src/beat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:22.547421 fenics-beat-0.0.3/src/fenics_beat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-05 11:50:22.000000 fenics-beat-0.0.3/src/fenics_beat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-05 11:50:22.000000 fenics-beat-0.0.3/src/fenics_beat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 11:50:22.000000 fenics-beat-0.0.3/src/fenics_beat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-05 11:50:22.000000 fenics-beat-0.0.3/src/fenics_beat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-05 11:50:22.000000 fenics-beat-0.0.3/src/fenics_beat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:22.543420 fenics-beat-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/tests/test_bidomain_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/tests/test_cellmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/tests/test_ecg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/tests/test_monodomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/tests/test_monodomain_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7106 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/tests/test_odesolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-05 11:50:19.000000 fenics-beat-0.0.3/tests/test_utils.py
```

### Comparing `fenics-beat-0.0.2/LICENSE` & `fenics-beat-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fenics-beat-0.0.2/PKG-INFO` & `fenics-beat-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenics-beat
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library to run cardiac EP simulations
 Author-email: Henrik Finsberg <henriknf@simula.no>
 License: MIT
 Project-URL: Homepage, https://finsberg.github.io/fenics-beat
 Project-URL: Documentation, https://finsberg.github.io/fenics-beat
 Project-URL: Source, https://github.com/finsberg/fenics-beat
 Project-URL: Tracker, https://github.com/finsberg/fenics-beat/issues
@@ -23,14 +23,15 @@
 Requires-Dist: bump2version; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: pypi
 Requires-Dist: twine; extra == "pypi"
 Requires-Dist: build; extra == "pypi"
 Provides-Extra: demos
 Requires-Dist: cardiac-geometries; extra == "demos"
+Requires-Dist: ldrb; extra == "demos"
 Provides-Extra: docs
 Requires-Dist: jupyter-book; extra == "docs"
 Requires-Dist: jupytext; extra == "docs"
 Requires-Dist: fenics-beat[demos]; extra == "docs"
 Provides-Extra: all
 Requires-Dist: fenics-beat[test]; extra == "all"
 Requires-Dist: fenics-beat[docs]; extra == "all"
```

### Comparing `fenics-beat-0.0.2/pyproject.toml` & `fenics-beat-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system] # Require setuptool version due to https://github.com/pypa/setuptools/issues/2938
 requires = ["setuptools>=61.0.0", "wheel"]
 
 [project]
 name = "fenics-beat"
-version = "0.0.2"
+version = "0.0.3"
 description = "Library to run cardiac EP simulations"
 authors = [{name = "Henrik Finsberg", email = "henriknf@simula.no"}]
 license = {text = "MIT"}
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["cardiac", "electrophysiology"]
 dependencies = [
@@ -34,14 +34,15 @@
 ]
 pypi = [
     "twine",
     "build"
 ]
 demos = [
    "cardiac-geometries",
+   "ldrb",
 ]
 docs = [
    "jupyter-book",
    "jupytext",
    "fenics-beat[demos]"
 ]
 all = [
```

### Comparing `fenics-beat-0.0.2/src/beat/__init__.py` & `fenics-beat-0.0.3/src/beat/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,15 @@
     monodomain_model,
     monodomain_solver,
     bidomain_model,
     base_model,
     cellmodels,
     odesolver,
     ecg,
+    utils,
 )
 
 from .monodomain_model import MonodomainModel
 from .bidomain_model import BidomainModel
 from .monodomain_solver import MonodomainSplittingSolver
 
 
@@ -20,8 +21,9 @@
     "odesolver",
     "base_model",
     "MonodomainModel",
     "BidomainModel",
     "monodomain_solver",
     "MonodomainSplittingSolver",
     "ecg",
+    "utils",
 ]
```

### Comparing `fenics-beat-0.0.2/src/beat/base_model.py` & `fenics-beat-0.0.3/src/beat/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 class Stimulus(NamedTuple):
     dz: dolfin.Measure
     expr: dolfin.Expression
 
 
-class BaseModel:
+class BaseModel(abc.ABC):
     def __init__(
         self,
         time: dolfin.Constant,
         mesh: dolfin.Mesh,
         params: dict[str, Any] | None = None,
         I_s: Stimulus | ufl.Coefficient | None = None,
     ) -> None:
```

### Comparing `fenics-beat-0.0.2/src/beat/bidomain_model.py` & `fenics-beat-0.0.3/src/beat/bidomain_model.py`

 * *Files identical despite different names*

### Comparing `fenics-beat-0.0.2/src/beat/cellmodels/beeler_reuter.py` & `fenics-beat-0.0.3/src/beat/cellmodels/beeler_reuter_1977.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,129 +1,12 @@
-"""This module contains a Beeler_reuter_1977 cardiac cell model
+# Gotran generated code for the "beeler_reuter_1977" model
 
-The module was autogenerated from a gotran ode file
-"""
-
-# from collections import OrderedDict
 import numpy as np
 
 
-def rhs(states, t, parameters, values):
-    """
-    Compute the right hand side of the beeler_reuter_1977 ODE
-    """
-
-    # Assign states
-    # assert len(states) == 8
-    m, h, j, Cai, d, f, x1, V = states
-
-    # Assign parameters
-    # assert len(parameters) == 10
-    E_Na = parameters[0]
-    g_Na = parameters[1]
-    g_Nac = parameters[2]
-    g_s = parameters[3]
-    IstimAmplitude = parameters[4]
-    IstimPulseDuration = parameters[7]
-    IstimStart = parameters[8]
-    C = parameters[9]
-
-    # # Init return args
-    # if values is None:
-    #     values = np.zeros((8,), dtype=np.float_)
-    # else:
-    #     assert isinstance(values, np.ndarray) and values.shape == (8,)
-
-    # Expressions for the Sodium current component
-    i_Na = (g_Nac + g_Na * (m * m * m) * h * j) * (-E_Na + V)
-
-    # Expressions for the Sodium current m gate component
-    alpha_m = (-47 - V) / (-1 + 0.009095277101695816 * np.exp(-0.1 * V))
-    beta_m = 0.7095526727489909 * np.exp(-0.056 * V)
-    values[0] = (1 - m) * alpha_m - beta_m * m
-
-    # Expressions for the Sodium current h gate component
-    alpha_h = 5.497962438709065e-10 * np.exp(-0.25 * V)
-    beta_h = 1.7 / (1 + 0.1580253208896478 * np.exp(-0.082 * V))
-    values[1] = (1 - h) * alpha_h - beta_h * h
-
-    # Expressions for the Sodium current j gate component
-    alpha_j = (
-        1.8690473007222892e-10
-        * np.exp(-0.25 * V)
-        / (1 + 1.6788275299956603e-07 * np.exp(-0.2 * V))
-    )
-    beta_j = 0.3 / (1 + 0.040762203978366204 * np.exp(-0.1 * V))
-    values[2] = (1 - j) * alpha_j - beta_j * j
-
-    # Expressions for the Slow inward current component
-    E_s = -82.3 - 13.0287 * np.log(0.001 * Cai)
-    i_s = g_s * (-E_s + V) * d * f
-    values[3] = 7.000000000000001e-06 - 0.07 * Cai - 0.01 * i_s
-
-    # Expressions for the Slow inward current d gate component
-    alpha_d = (
-        0.095
-        * np.exp(1 / 20 - V / 100)
-        / (1 + 1.4332881385696572 * np.exp(-0.07199424046076314 * V))
-    )
-    beta_d = 0.07 * np.exp(-44 / 59 - V / 59) / (1 + np.exp(11 / 5 + V / 20))
-    values[4] = (1 - d) * alpha_d - beta_d * d
-
-    # Expressions for the Slow inward current f gate component
-    alpha_f = (
-        0.012
-        * np.exp(-28 / 125 - V / 125)
-        / (1 + 66.5465065250986 * np.exp(0.14992503748125938 * V))
-    )
-    beta_f = 0.0065 * np.exp(-3 / 5 - V / 50) / (1 + np.exp(-6 - V / 5))
-    values[5] = (1 - f) * alpha_f - beta_f * f
-
-    # Expressions for the Time dependent outward current component
-    i_x1 = (
-        0.0019727757115328517
-        * (-1 + 21.75840239619708 * np.exp(0.04 * V))
-        * np.exp(-0.04 * V)
-        * x1
-    )
-
-    # Expressions for the Time dependent outward current x1 gate component
-    alpha_x1 = (
-        0.031158410986342627
-        * np.exp(0.08264462809917356 * V)
-        / (1 + 17.41170806332765 * np.exp(0.05714285714285714 * V))
-    )
-    beta_x1 = (
-        0.0003916464405623223
-        * np.exp(-0.05998800239952009 * V)
-        / (1 + np.exp(-4 / 5 - V / 25))
-    )
-    values[6] = (1 - x1) * alpha_x1 - beta_x1 * x1
-
-    # Expressions for the Time independent outward current component
-    i_K1 = 0.0035 * (4.6000000000000005 + 0.2 * V) / (
-        1 - 0.39851904108451414 * np.exp(-0.04 * V)
-    ) + 0.0035 * (-4 + 119.85640018958804 * np.exp(0.04 * V)) / (
-        8.331137487687693 * np.exp(0.04 * V) + 69.4078518387552 * np.exp(0.08 * V)
-    )
-
-    # Expressions for the Stimulus protocol component
-    Istim = np.where(
-        np.logical_and(t >= IstimStart, t <= IstimPulseDuration + IstimStart),
-        IstimAmplitude,
-        0,
-    )
-
-    # Expressions for the Membrane component
-    values[7] = (-i_K1 - i_Na - i_s - i_x1 + Istim) / C
-
-    # Return results
-    return values
-
-
 def init_state_values(**values):
     """
     Initialize state values
     """
     # Init values
     # m=0.011, h=0.988, j=0.975, Cai=0.0001, d=0.003, f=0.994, x1=0.0001,
     # V=-84.624
@@ -191,29 +74,14 @@
 
         # Assign value
         init_values[ind] = value
 
     return init_values
 
 
-def init_parameters():
-    return {
-        "E_Na": 50.0,
-        "g_Na": 0.04,
-        "g_Nac": 3e-05,
-        "g_s": 0.0009,
-        "IstimAmplitude": 0.0,
-        "IstimEnd": 50000.0,
-        "IstimPeriod": 1000.0,
-        "IstimPulseDuration": 1.0,
-        "IstimStart": 1.0,
-        "C": 0.01,
-    }
-
-
 def state_indices(*states):
     """
     State indices
     """
     state_inds = dict(
         [
             ("m", 0),
@@ -264,43 +132,424 @@
         indices.append(param_inds[param])
     if len(indices) > 1:
         return indices
     else:
         return indices[0]
 
 
-# @numba.jit(nopython=True, fastmath=True)
+def monitor_indices(*monitored):
+    """
+    Monitor indices
+    """
+    monitor_inds = dict(
+        [
+            ("i_Na", 0),
+            ("alpha_m", 1),
+            ("beta_m", 2),
+            ("alpha_h", 3),
+            ("beta_h", 4),
+            ("alpha_j", 5),
+            ("beta_j", 6),
+            ("E_s", 7),
+            ("i_s", 8),
+            ("alpha_d", 9),
+            ("beta_d", 10),
+            ("alpha_f", 11),
+            ("beta_f", 12),
+            ("i_x1", 13),
+            ("alpha_x1", 14),
+            ("beta_x1", 15),
+            ("Istim", 16),
+            ("i_K1", 17),
+            ("dm_dt", 18),
+            ("dh_dt", 19),
+            ("dj_dt", 20),
+            ("dCai_dt", 21),
+            ("dd_dt", 22),
+            ("df_dt", 23),
+            ("dx1_dt", 24),
+            ("dV_dt", 25),
+        ]
+    )
+
+    indices = []
+    for monitor in monitored:
+        if monitor not in monitor_inds:
+            raise ValueError("Unknown monitored: '{0}'".format(monitor))
+        indices.append(monitor_inds[monitor])
+    if len(indices) > 1:
+        return indices
+    else:
+        return indices[0]
+
+
+def rhs(states, t, parameters, values=None):
+    """
+    Compute the right hand side of the beeler_reuter_1977 ODE
+    """
+
+    # Assign states
+    assert len(states) == 8
+    m, h, j, Cai, d, f, x1, V = states
+
+    # Assign parameters
+    assert len(parameters) == 10
+    E_Na = parameters[0]
+    g_Na = parameters[1]
+    g_Nac = parameters[2]
+    g_s = parameters[3]
+    IstimAmplitude = parameters[4]
+    IstimPulseDuration = parameters[7]
+    IstimStart = parameters[8]
+    C = parameters[9]
+
+    # Init return args
+    if values is None:
+        values = np.zeros((8,), dtype=np.float_)
+    else:
+        assert isinstance(values, np.ndarray) and values.shape == (8,)
+
+    # Expressions for the Sodium current component
+    i_Na = (g_Nac + g_Na * (m * m * m) * h * j) * (-E_Na + V)
+
+    # Expressions for the Sodium current m gate component
+    alpha_m = (-47 - V) / (-1 + 0.009095277101695816 * np.exp(-0.1 * V))
+    beta_m = 0.7095526727489909 * np.exp(-0.056 * V)
+    values[0] = (1 - m) * alpha_m - beta_m * m
+
+    # Expressions for the Sodium current h gate component
+    alpha_h = 5.497962438709065e-10 * np.exp(-0.25 * V)
+    beta_h = 1.7 / (1 + 0.1580253208896478 * np.exp(-0.082 * V))
+    values[1] = (1 - h) * alpha_h - beta_h * h
+
+    # Expressions for the Sodium current j gate component
+    alpha_j = (
+        1.8690473007222892e-10
+        * np.exp(-0.25 * V)
+        / (1 + 1.6788275299956603e-07 * np.exp(-0.2 * V))
+    )
+    beta_j = 0.3 / (1 + 0.040762203978366204 * np.exp(-0.1 * V))
+    values[2] = (1 - j) * alpha_j - beta_j * j
+
+    # Expressions for the Slow inward current component
+    E_s = -82.3 - 13.0287 * np.log(0.001 * Cai)
+    i_s = g_s * (-E_s + V) * d * f
+    values[3] = 7.000000000000001e-06 - 0.07 * Cai - 0.01 * i_s
+
+    # Expressions for the Slow inward current d gate component
+    alpha_d = (
+        0.095
+        * np.exp(1 / 20 - V / 100)
+        / (1 + 1.4332881385696572 * np.exp(-0.07199424046076314 * V))
+    )
+    beta_d = 0.07 * np.exp(-44 / 59 - V / 59) / (1 + np.exp(11 / 5 + V / 20))
+    values[4] = (1 - d) * alpha_d - beta_d * d
+
+    # Expressions for the Slow inward current f gate component
+    alpha_f = (
+        0.012
+        * np.exp(-28 / 125 - V / 125)
+        / (1 + 66.5465065250986 * np.exp(0.14992503748125938 * V))
+    )
+    beta_f = 0.0065 * np.exp(-3 / 5 - V / 50) / (1 + np.exp(-6 - V / 5))
+    values[5] = (1 - f) * alpha_f - beta_f * f
+
+    # Expressions for the Time dependent outward current component
+    i_x1 = (
+        0.0019727757115328517
+        * (-1 + 21.75840239619708 * np.exp(0.04 * V))
+        * np.exp(-0.04 * V)
+        * x1
+    )
+
+    # Expressions for the Time dependent outward current x1 gate component
+    alpha_x1 = (
+        0.031158410986342627
+        * np.exp(0.08264462809917356 * V)
+        / (1 + 17.41170806332765 * np.exp(0.05714285714285714 * V))
+    )
+    beta_x1 = (
+        0.0003916464405623223
+        * np.exp(-0.05998800239952009 * V)
+        / (1 + np.exp(-4 / 5 - V / 25))
+    )
+    values[6] = (1 - x1) * alpha_x1 - beta_x1 * x1
+
+    # Expressions for the Time independent outward current component
+    i_K1 = 0.0035 * (4.6000000000000005 + 0.2 * V) / (
+        1 - 0.39851904108451414 * np.exp(-0.04 * V)
+    ) + 0.0035 * (-4 + 119.85640018958804 * np.exp(0.04 * V)) / (
+        8.331137487687693 * np.exp(0.04 * V) + 69.4078518387552 * np.exp(0.08 * V)
+    )
+
+    # Expressions for the Stimulus protocol component
+    Istim = np.where(
+        np.logical_and(t >= IstimStart, t <= IstimPulseDuration + IstimStart),
+        IstimAmplitude,
+        0,
+    )
+
+    # Expressions for the Membrane component
+    values[7] = (-i_K1 - i_Na - i_s - i_x1 + Istim) / C
+
+    # Return results
+    return values
+
+
+def monitor(states, t, parameters, monitored=None):
+    """
+    Computes monitored expressions of the beeler_reuter_1977 ODE
+    """
+
+    # Assign states
+    assert len(states) == 8
+    m, h, j, Cai, d, f, x1, V = states
+
+    # Assign parameters
+    assert len(parameters) == 10
+    E_Na = parameters[0]
+    g_Na = parameters[1]
+    g_Nac = parameters[2]
+    g_s = parameters[3]
+    IstimAmplitude = parameters[4]
+    IstimPulseDuration = parameters[7]
+    IstimStart = parameters[8]
+    C = parameters[9]
+
+    # Init return args
+    if monitored is None:
+        monitored = np.zeros((26,), dtype=np.float_)
+    else:
+        assert isinstance(monitored, np.ndarray) and monitored.shape == (26,)
+
+    # Expressions for the Sodium current component
+    monitored[0] = (g_Nac + g_Na * (m * m * m) * h * j) * (-E_Na + V)
+
+    # Expressions for the Sodium current m gate component
+    monitored[1] = (-47 - V) / (-1 + 0.009095277101695816 * np.exp(-0.1 * V))
+    monitored[2] = 0.7095526727489909 * np.exp(-0.056 * V)
+    monitored[18] = (1 - m) * monitored[1] - m * monitored[2]
+
+    # Expressions for the Sodium current h gate component
+    monitored[3] = 5.497962438709065e-10 * np.exp(-0.25 * V)
+    monitored[4] = 1.7 / (1 + 0.1580253208896478 * np.exp(-0.082 * V))
+    monitored[19] = (1 - h) * monitored[3] - h * monitored[4]
+
+    # Expressions for the Sodium current j gate component
+    monitored[5] = (
+        1.8690473007222892e-10
+        * np.exp(-0.25 * V)
+        / (1 + 1.6788275299956603e-07 * np.exp(-0.2 * V))
+    )
+    monitored[6] = 0.3 / (1 + 0.040762203978366204 * np.exp(-0.1 * V))
+    monitored[20] = (1 - j) * monitored[5] - j * monitored[6]
+
+    # Expressions for the Slow inward current component
+    monitored[7] = -82.3 - 13.0287 * np.log(0.001 * Cai)
+    monitored[8] = g_s * (-monitored[7] + V) * d * f
+    monitored[21] = 7.000000000000001e-06 - 0.07 * Cai - 0.01 * monitored[8]
+
+    # Expressions for the Slow inward current d gate component
+    monitored[9] = (
+        0.095
+        * np.exp(1 / 20 - V / 100)
+        / (1 + 1.4332881385696572 * np.exp(-0.07199424046076314 * V))
+    )
+    monitored[10] = 0.07 * np.exp(-44 / 59 - V / 59) / (1 + np.exp(11 / 5 + V / 20))
+    monitored[22] = (1 - d) * monitored[9] - d * monitored[10]
+
+    # Expressions for the Slow inward current f gate component
+    monitored[11] = (
+        0.012
+        * np.exp(-28 / 125 - V / 125)
+        / (1 + 66.5465065250986 * np.exp(0.14992503748125938 * V))
+    )
+    monitored[12] = 0.0065 * np.exp(-3 / 5 - V / 50) / (1 + np.exp(-6 - V / 5))
+    monitored[23] = (1 - f) * monitored[11] - f * monitored[12]
+
+    # Expressions for the Time dependent outward current component
+    monitored[13] = (
+        0.0019727757115328517
+        * (-1 + 21.75840239619708 * np.exp(0.04 * V))
+        * np.exp(-0.04 * V)
+        * x1
+    )
+
+    # Expressions for the Time dependent outward current x1 gate component
+    monitored[14] = (
+        0.031158410986342627
+        * np.exp(0.08264462809917356 * V)
+        / (1 + 17.41170806332765 * np.exp(0.05714285714285714 * V))
+    )
+    monitored[15] = (
+        0.0003916464405623223
+        * np.exp(-0.05998800239952009 * V)
+        / (1 + np.exp(-4 / 5 - V / 25))
+    )
+    monitored[24] = (1 - x1) * monitored[14] - monitored[15] * x1
+
+    # Expressions for the Time independent outward current component
+    monitored[17] = 0.0035 * (4.6000000000000005 + 0.2 * V) / (
+        1 - 0.39851904108451414 * np.exp(-0.04 * V)
+    ) + 0.0035 * (-4 + 119.85640018958804 * np.exp(0.04 * V)) / (
+        8.331137487687693 * np.exp(0.04 * V) + 69.4078518387552 * np.exp(0.08 * V)
+    )
+
+    # Expressions for the Stimulus protocol component
+    monitored[16] = np.where(
+        np.logical_and(t >= IstimStart, t <= IstimPulseDuration + IstimStart),
+        IstimAmplitude,
+        0,
+    )
+
+    # Expressions for the Membrane component
+    monitored[25] = (
+        -monitored[0] - monitored[13] - monitored[17] - monitored[8] + monitored[16]
+    ) / C
+
+    # Return results
+    return monitored
+
+
+def forward_explicit_euler(states, t, dt, parameters):
+    """
+    Compute a forward step using the explicit Euler scheme to the\
+        beeler_reuter_1977 ODE
+    """
+
+    # Assign states
+    assert len(states) == 8
+    m, h, j, Cai, d, f, x1, V = states
+
+    # Assign parameters
+    assert len(parameters) == 10
+    E_Na = parameters[0]
+    g_Na = parameters[1]
+    g_Nac = parameters[2]
+    g_s = parameters[3]
+    IstimAmplitude = parameters[4]
+    IstimPulseDuration = parameters[7]
+    IstimStart = parameters[8]
+    C = parameters[9]
+
+    # Expressions for the Sodium current component
+    i_Na = (g_Nac + g_Na * (m * m * m) * h * j) * (-E_Na + V)
+
+    # Expressions for the Sodium current m gate component
+    alpha_m = (-47 - V) / (-1 + 0.009095277101695816 * np.exp(-0.1 * V))
+    beta_m = 0.7095526727489909 * np.exp(-0.056 * V)
+    dm_dt = (1 - m) * alpha_m - beta_m * m
+    states[0] = dt * dm_dt + m
+
+    # Expressions for the Sodium current h gate component
+    alpha_h = 5.497962438709065e-10 * np.exp(-0.25 * V)
+    beta_h = 1.7 / (1 + 0.1580253208896478 * np.exp(-0.082 * V))
+    dh_dt = (1 - h) * alpha_h - beta_h * h
+    states[1] = dt * dh_dt + h
+
+    # Expressions for the Sodium current j gate component
+    alpha_j = (
+        1.8690473007222892e-10
+        * np.exp(-0.25 * V)
+        / (1 + 1.6788275299956603e-07 * np.exp(-0.2 * V))
+    )
+    beta_j = 0.3 / (1 + 0.040762203978366204 * np.exp(-0.1 * V))
+    dj_dt = (1 - j) * alpha_j - beta_j * j
+    states[2] = dt * dj_dt + j
+
+    # Expressions for the Slow inward current component
+    E_s = -82.3 - 13.0287 * np.log(0.001 * Cai)
+    i_s = g_s * (-E_s + V) * d * f
+    dCai_dt = 7.000000000000001e-06 - 0.07 * Cai - 0.01 * i_s
+    states[3] = dt * dCai_dt + Cai
+
+    # Expressions for the Slow inward current d gate component
+    alpha_d = (
+        0.095
+        * np.exp(1 / 20 - V / 100)
+        / (1 + 1.4332881385696572 * np.exp(-0.07199424046076314 * V))
+    )
+    beta_d = 0.07 * np.exp(-44 / 59 - V / 59) / (1 + np.exp(11 / 5 + V / 20))
+    dd_dt = (1 - d) * alpha_d - beta_d * d
+    states[4] = dt * dd_dt + d
+
+    # Expressions for the Slow inward current f gate component
+    alpha_f = (
+        0.012
+        * np.exp(-28 / 125 - V / 125)
+        / (1 + 66.5465065250986 * np.exp(0.14992503748125938 * V))
+    )
+    beta_f = 0.0065 * np.exp(-3 / 5 - V / 50) / (1 + np.exp(-6 - V / 5))
+    df_dt = (1 - f) * alpha_f - beta_f * f
+    states[5] = dt * df_dt + f
+
+    # Expressions for the Time dependent outward current component
+    i_x1 = (
+        0.0019727757115328517
+        * (-1 + 21.75840239619708 * np.exp(0.04 * V))
+        * np.exp(-0.04 * V)
+        * x1
+    )
+
+    # Expressions for the Time dependent outward current x1 gate component
+    alpha_x1 = (
+        0.031158410986342627
+        * np.exp(0.08264462809917356 * V)
+        / (1 + 17.41170806332765 * np.exp(0.05714285714285714 * V))
+    )
+    beta_x1 = (
+        0.0003916464405623223
+        * np.exp(-0.05998800239952009 * V)
+        / (1 + np.exp(-4 / 5 - V / 25))
+    )
+    dx1_dt = (1 - x1) * alpha_x1 - beta_x1 * x1
+    states[6] = dt * dx1_dt + x1
+
+    # Expressions for the Time independent outward current component
+    i_K1 = 0.0035 * (4.6000000000000005 + 0.2 * V) / (
+        1 - 0.39851904108451414 * np.exp(-0.04 * V)
+    ) + 0.0035 * (-4 + 119.85640018958804 * np.exp(0.04 * V)) / (
+        8.331137487687693 * np.exp(0.04 * V) + 69.4078518387552 * np.exp(0.08 * V)
+    )
+
+    # Expressions for the Stimulus protocol component
+    Istim = np.where(
+        np.logical_and(t >= IstimStart, t <= IstimPulseDuration + IstimStart),
+        IstimAmplitude,
+        0,
+    )
+
+    # Expressions for the Membrane component
+    dV_dt = (-i_K1 - i_Na - i_s - i_x1 + Istim) / C
+    states[7] = dt * dV_dt + V
+
+    # Return results
+    return states
+
+
 def forward_generalized_rush_larsen(states, t, dt, parameters):
     """
     Compute a forward step using the generalised Rush-Larsen (GRL1) scheme to\
         the beeler_reuter_1977 ODE
     """
 
     # Assign states
-    # assert len(states) == 8
+    assert len(states) == 8
     m, h, j, Cai, d, f, x1, V = states
 
     # Assign parameters
-    # assert len(parameters) == 10
+    assert len(parameters) == 10
     E_Na = parameters[0]
     g_Na = parameters[1]
     g_Nac = parameters[2]
     g_s = parameters[3]
     IstimAmplitude = parameters[4]
     IstimPulseDuration = parameters[7]
     IstimStart = parameters[8]
     C = parameters[9]
-    # E_Na = parameters["E_Na"]
-    # g_Na = parameters["g_Na"]
-    # g_Nac = parameters["g_Nac"]
-    # g_s = parameters["g_s"]
-    # IstimAmplitude = parameters["IstimAmplitude"]
-    # IstimPulseDuration = parameters["IstimPulseDuration"]
-    # IstimStart = parameters["IstimStart"]
-    # C = parameters["C"]
 
     # Expressions for the Sodium current component
     i_Na = (g_Nac + g_Na * (m * m * m) * h * j) * (-E_Na + V)
 
     # Expressions for the Sodium current m gate component
     alpha_m = (-47 - V) / (-1 + 0.009095277101695816 * np.exp(-0.1 * V))
     beta_m = 0.7095526727489909 * np.exp(-0.056 * V)
```

### Comparing `fenics-beat-0.0.2/src/beat/cellmodels/fitzhughnagumo.py` & `fenics-beat-0.0.3/src/beat/cellmodels/fitzhughnagumo.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,19 +26,19 @@
 
 
 def init_parameter_values(**values):
     """
     Initialize parameter values
     """
     # Param values
-    # a=0.13, b=0.013, c_1=0.26, c_2=0.1, c_3=1.0, stim_amplitude=0,
+    # a=0.13, b=0.013, c_1=0.26, c_2=0.1, c_3=1.0, stim_amplitude=50,
     # stim_duration=1, stim_period=1000, stim_start=1, v_peak=40.0,
     # v_rest=-85.0
     init_values = np.array(
-        [0.13, 0.013, 0.26, 0.1, 1.0, 0, 1, 1000, 1, 40.0, -85.0], dtype=np.float_
+        [0.13, 0.013, 0.26, 0.1, 1.0, 50, 1, 1000, 1, 40.0, -85.0], dtype=np.float_
     )
 
     # Parameter indices and limit checker
     param_ind = dict(
         [
             ("a", 0),
             ("b", 1),
```

### Comparing `fenics-beat-0.0.2/src/beat/cellmodels/tentusscher_panfilov_2006_M_cell.py` & `fenics-beat-0.0.3/src/beat/cellmodels/tentusscher_panfilov_2006/epi.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# Gotran generated code for the "tentusscher_panfilov_2006_M_cell" model
+# Gotran generated code for the "tentusscher_panfilov_2006_epi_cell" model
 
 import numpy as np
 
 
 def init_state_values(**values):
     """
     Initialize state values
     """
     # Init values
-    # Xr1=0.0165, Xr2=0.473, Xs=0.0174, m=0.00165, h=0.749, j=0.6788,
-    # d=3.288e-05, f=0.7026, f2=0.9526, fCass=0.9942, s=0.999998,
-    # r=2.347e-08, Ca_i=0.000153, R_prime=0.8978, Ca_SR=4.272,
-    # Ca_ss=0.00042, Na_i=10.132, V=-85.423, K_i=138.52
+    # Xr1=0.00621, Xr2=0.4712, Xs=0.0095, m=0.00172, h=0.7444, j=0.7045,
+    # d=3.373e-05, f=0.7888, f2=0.9755, fCass=0.9953, s=0.999998,
+    # r=2.42e-08, Ca_i=0.000126, R_prime=0.9073, Ca_SR=3.64,
+    # Ca_ss=0.00036, Na_i=8.604, V=-85.23, K_i=136.89
     init_values = np.array(
         [
-            0.0165,
-            0.473,
-            0.0174,
-            0.00165,
-            0.749,
-            0.6788,
-            3.288e-05,
-            0.7026,
-            0.9526,
-            0.9942,
+            0.00621,
+            0.4712,
+            0.0095,
+            0.00172,
+            0.7444,
+            0.7045,
+            3.373e-05,
+            0.7888,
+            0.9755,
+            0.9953,
             0.999998,
-            2.347e-08,
-            0.000153,
-            0.8978,
-            4.272,
-            0.00042,
-            10.132,
-            -85.423,
-            138.52,
+            2.42e-08,
+            0.000126,
+            0.9073,
+            3.64,
+            0.00036,
+            8.604,
+            -85.23,
+            136.89,
         ],
         dtype=np.float_,
     )
 
     # State indices and limit checker
     state_ind = dict(
         [
@@ -74,80 +74,80 @@
 
 
 def init_parameter_values(**values):
     """
     Initialize parameter values
     """
     # Param values
-    # P_kna=0.03, g_K1=5.405, g_Kr=0.153, g_Ks=0.098, g_Na=14.838,
-    # g_bna=0.00029, g_CaL=3.98e-05, g_bca=0.000592, g_to=0.294,
-    # K_mNa=40, K_mk=1, P_NaK=2.724, K_NaCa=1000, K_sat=0.1,
+    # P_kna=0.03, g_K1=5.405, g_Kr=0.153, g_Ks=0.392, g_Na=14.838,
+    # g_bna=0.00029, g_CaL=0.0398, g_bca=0.000592, g_to=0.294,
+    # K_mNa=40.0, K_mk=1.0, P_NaK=2.724, K_NaCa=1000.0, K_sat=0.1,
     # Km_Ca=1.38, Km_Nai=87.5, alpha=2.5, gamma=0.35, K_pCa=0.0005,
-    # g_pCa=0.1238, g_pK=0.0146, Buf_c=0.2, Buf_sr=10, Buf_ss=0.4,
-    # Ca_o=2, EC=1.5, K_buf_c=0.001, K_buf_sr=0.3, K_buf_ss=0.00025,
-    # K_up=0.00025, V_leak=0.00036, V_rel=0.102, V_sr=0.001094,
-    # V_ss=5.468e-05, V_xfer=0.0038, Vmax_up=0.006375, k1_prime=0.15,
+    # g_pCa=0.1238, g_pK=0.0146, Buf_c=0.2, Buf_sr=10.0, Buf_ss=0.4,
+    # Ca_o=2.0, EC=1.5, K_buf_c=0.001, K_buf_sr=0.3, K_buf_ss=0.00025,
+    # K_up=0.00025, V_leak=0.00036, V_rel=0.102, V_sr=1094.0,
+    # V_ss=54.68, V_xfer=0.0038, Vmax_up=0.006375, k1_prime=0.15,
     # k2_prime=0.045, k3=0.06, k4=0.005, max_sr=2.5, min_sr=1,
-    # Na_o=140, Cm=0.185, F=96485.3415, R=8314.472, T=310,
-    # V_c=0.016404, stim_amplitude=0, stim_duration=1, stim_period=1000,
-    # stim_start=1, K_o=5.4
+    # Na_o=140.0, Cm=185.0, F=96.485, R=8.314, T=310.0, V_c=16404.0,
+    # stim_amplitude=-52.0, stim_duration=1.0, stim_period=1000.0,
+    # stim_start=10.0, K_o=5.4
     init_values = np.array(
         [
             0.03,
             5.405,
             0.153,
-            0.098,
+            0.392,
             14.838,
             0.00029,
-            3.98e-05,
+            0.0398,
             0.000592,
             0.294,
-            40,
-            1,
+            40.0,
+            1.0,
             2.724,
-            1000,
+            1000.0,
             0.1,
             1.38,
             87.5,
             2.5,
             0.35,
             0.0005,
             0.1238,
             0.0146,
             0.2,
-            10,
+            10.0,
             0.4,
-            2,
+            2.0,
             1.5,
             0.001,
             0.3,
             0.00025,
             0.00025,
             0.00036,
             0.102,
-            0.001094,
-            5.468e-05,
+            1094.0,
+            54.68,
             0.0038,
             0.006375,
             0.15,
             0.045,
             0.06,
             0.005,
             2.5,
             1,
-            140,
-            0.185,
-            96485.3415,
-            8314.472,
-            310,
-            0.016404,
-            0,
-            1,
-            1000,
-            1,
+            140.0,
+            185.0,
+            96.485,
+            8.314,
+            310.0,
+            16404.0,
+            -52.0,
+            1.0,
+            1000.0,
+            10.0,
             5.4,
         ],
         dtype=np.float_,
     )
 
     # Parameter indices and limit checker
     param_ind = dict(
@@ -395,41 +395,44 @@
             ("i_NaCa", 55),
             ("i_p_Ca", 56),
             ("i_p_K", 57),
             ("i_up", 58),
             ("i_leak", 59),
             ("i_xfer", 60),
             ("kcasr", 61),
-            ("Ca_i_bufc", 62),
-            ("Ca_sr_bufsr", 63),
-            ("Ca_ss_bufss", 64),
-            ("k1", 65),
-            ("k2", 66),
-            ("O", 67),
-            ("i_rel", 68),
-            ("i_Stim", 69),
-            ("dXr1_dt", 70),
-            ("dXr2_dt", 71),
-            ("dXs_dt", 72),
-            ("dm_dt", 73),
-            ("dh_dt", 74),
-            ("dj_dt", 75),
-            ("dd_dt", 76),
-            ("df_dt", 77),
-            ("df2_dt", 78),
-            ("dfCass_dt", 79),
-            ("ds_dt", 80),
-            ("dr_dt", 81),
-            ("dCa_i_dt", 82),
-            ("dR_prime_dt", 83),
-            ("dCa_SR_dt", 84),
-            ("dCa_ss_dt", 85),
-            ("dNa_i_dt", 86),
-            ("dV_dt", 87),
-            ("dK_i_dt", 88),
+            ("ddt_Ca_i_total", 62),
+            ("f_JCa_i_free", 63),
+            ("f_JCa_sr_free", 64),
+            ("f_JCa_ss_free", 65),
+            ("k1", 66),
+            ("k2", 67),
+            ("O", 68),
+            ("i_rel", 69),
+            ("ddt_Ca_sr_total", 70),
+            ("ddt_Ca_ss_total", 71),
+            ("i_Stim", 72),
+            ("dXr1_dt", 73),
+            ("dXr2_dt", 74),
+            ("dXs_dt", 75),
+            ("dm_dt", 76),
+            ("dh_dt", 77),
+            ("dj_dt", 78),
+            ("dd_dt", 79),
+            ("df_dt", 80),
+            ("df2_dt", 81),
+            ("dfCass_dt", 82),
+            ("ds_dt", 83),
+            ("dr_dt", 84),
+            ("dCa_i_dt", 85),
+            ("dR_prime_dt", 86),
+            ("dCa_SR_dt", 87),
+            ("dCa_ss_dt", 88),
+            ("dNa_i_dt", 89),
+            ("dV_dt", 90),
+            ("dK_i_dt", 91),
         ]
     )
 
     indices = []
     for monitor in monitored:
         if monitor not in monitor_inds:
             raise ValueError("Unknown monitored: '{0}'".format(monitor))
@@ -438,15 +441,15 @@
         return indices
     else:
         return indices[0]
 
 
 def rhs(states, t, parameters, values=None):
     """
-    Compute the right hand side of the tentusscher_panfilov_2006_M_cell ODE
+    Compute the right hand side of the tentusscher_panfilov_2006_epi_cell ODE
     """
 
     # Assign states
     assert len(states) == 19
     (
         Xr1,
         Xr2,
@@ -467,63 +470,69 @@
         Na_i,
         V,
         K_i,
     ) = states
 
     # Assign parameters
     assert len(parameters) == 53
-    P_kna = parameters[0]
-    g_K1 = parameters[1]
-    g_Kr = parameters[2]
-    g_Ks = parameters[3]
-    g_Na = parameters[4]
-    g_bna = parameters[5]
-    g_CaL = parameters[6]
-    g_bca = parameters[7]
-    g_to = parameters[8]
-    K_mNa = parameters[9]
-    K_mk = parameters[10]
-    P_NaK = parameters[11]
-    K_NaCa = parameters[12]
-    K_sat = parameters[13]
-    Km_Ca = parameters[14]
-    Km_Nai = parameters[15]
-    alpha = parameters[16]
-    gamma = parameters[17]
-    K_pCa = parameters[18]
-    g_pCa = parameters[19]
-    g_pK = parameters[20]
-    Buf_c = parameters[21]
-    Buf_sr = parameters[22]
-    Buf_ss = parameters[23]
-    Ca_o = parameters[24]
-    EC = parameters[25]
-    K_buf_c = parameters[26]
-    K_buf_sr = parameters[27]
-    K_buf_ss = parameters[28]
-    K_up = parameters[29]
-    V_leak = parameters[30]
-    V_rel = parameters[31]
-    V_sr = parameters[32]
-    V_ss = parameters[33]
-    V_xfer = parameters[34]
-    Vmax_up = parameters[35]
-    k1_prime = parameters[36]
-    k2_prime = parameters[37]
-    k3 = parameters[38]
-    k4 = parameters[39]
-    max_sr = parameters[40]
-    min_sr = parameters[41]
-    Na_o = parameters[42]
-    Cm = parameters[43]
-    F = parameters[44]
-    R = parameters[45]
-    T = parameters[46]
-    V_c = parameters[47]
-    K_o = parameters[52]
+    (
+        P_kna,
+        g_K1,
+        g_Kr,
+        g_Ks,
+        g_Na,
+        g_bna,
+        g_CaL,
+        g_bca,
+        g_to,
+        K_mNa,
+        K_mk,
+        P_NaK,
+        K_NaCa,
+        K_sat,
+        Km_Ca,
+        Km_Nai,
+        alpha,
+        gamma,
+        K_pCa,
+        g_pCa,
+        g_pK,
+        Buf_c,
+        Buf_sr,
+        Buf_ss,
+        Ca_o,
+        EC,
+        K_buf_c,
+        K_buf_sr,
+        K_buf_ss,
+        K_up,
+        V_leak,
+        V_rel,
+        V_sr,
+        V_ss,
+        V_xfer,
+        Vmax_up,
+        k1_prime,
+        k2_prime,
+        k3,
+        k4,
+        max_sr,
+        min_sr,
+        Na_o,
+        Cm,
+        F,
+        R,
+        T,
+        V_c,
+        stim_amplitude,
+        stim_duration,
+        stim_period,
+        stim_start,
+        K_o,
+    ) = parameters
 
     # Init return args
     if values is None:
         values = np.zeros((19,), dtype=np.float_)
     else:
         assert isinstance(values, np.ndarray) and values.shape == (19,)
 
@@ -727,69 +736,80 @@
     )
 
     # Expressions for the Calcium dynamics component
     i_up = Vmax_up / (1 + (K_up * K_up) / (Ca_i * Ca_i))
     i_leak = V_leak * (-Ca_i + Ca_SR)
     i_xfer = V_xfer * (-Ca_i + Ca_ss)
     kcasr = max_sr - (max_sr - min_sr) / (1 + (EC * EC) / (Ca_SR * Ca_SR))
-    Ca_i_bufc = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
-    Ca_sr_bufsr = 1.0 / (
+    ddt_Ca_i_total = (
+        V_sr * (-i_up + i_leak) / V_c
+        + Cm * (-i_b_Ca - i_p_Ca + 2 * i_NaCa) / (2 * F * V_c)
+        + i_xfer
+    )
+    f_JCa_i_free = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
+    f_JCa_sr_free = 1.0 / (
         1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR))
     )
-    Ca_ss_bufss = 1.0 / (
+    f_JCa_ss_free = 1.0 / (
         1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss))
     )
-    values[12] = (
-        V_sr * (-i_up + i_leak) / V_c
-        - Cm * (-2 * i_NaCa + i_b_Ca + i_p_Ca) / (2 * F * V_c)
-        + i_xfer
-    ) * Ca_i_bufc
+    values[12] = ddt_Ca_i_total * f_JCa_i_free
     k1 = k1_prime / kcasr
     k2 = k2_prime * kcasr
     O = (Ca_ss * Ca_ss) * R_prime * k1 / (k3 + (Ca_ss * Ca_ss) * k1)
     values[13] = k4 * (1 - R_prime) - Ca_ss * R_prime * k2
     i_rel = V_rel * (-Ca_ss + Ca_SR) * O
-    values[14] = (-i_leak - i_rel + i_up) * Ca_sr_bufsr
-    values[15] = (
+    ddt_Ca_sr_total = -i_leak - i_rel + i_up
+    ddt_Ca_ss_total = (
         V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
-    ) * Ca_ss_bufss
+    )
+    values[14] = ddt_Ca_sr_total * f_JCa_sr_free
+    values[15] = ddt_Ca_ss_total * f_JCa_ss_free
 
     # Expressions for the Sodium dynamics component
     values[16] = Cm * (-i_Na - i_b_Na - 3 * i_NaCa - 3 * i_NaK) / (F * V_c)
 
     # Expressions for the Membrane component
-    i_Stim = 0
+    i_Stim = np.where(
+        np.logical_and(
+            t - stim_period * np.floor(t / stim_period) >= stim_start,
+            t - stim_period * np.floor(t / stim_period) <= stim_duration + stim_start,
+        ),
+        stim_amplitude,
+        0,
+    )
     values[17] = (
-        -i_Stim
-        - i_CaL
+        -i_CaL
         - i_K1
         - i_Kr
         - i_Ks
         - i_Na
         - i_NaCa
         - i_NaK
+        - i_Stim
         - i_b_Ca
         - i_b_Na
         - i_p_Ca
         - i_p_K
         - i_to
     )
 
     # Expressions for the Potassium dynamics component
     values[18] = (
-        Cm * (-i_Stim - i_K1 - i_Kr - i_Ks - i_p_K - i_to + 2 * i_NaK) / (F * V_c)
+        Cm * (-i_K1 - i_Kr - i_Ks - i_Stim - i_p_K - i_to + 2 * i_NaK) / (F * V_c)
     )
 
     # Return results
     return values
 
 
 def monitor(states, t, parameters, monitored=None):
     """
-    Computes monitored expressions of the tentusscher_panfilov_2006_M_cell ODE
+    Computes monitored expressions of the tentusscher_panfilov_2006_epi_cell\
+        ODE
     """
 
     # Assign states
     assert len(states) == 19
     (
         Xr1,
         Xr2,
@@ -810,69 +830,75 @@
         Na_i,
         V,
         K_i,
     ) = states
 
     # Assign parameters
     assert len(parameters) == 53
-    P_kna = parameters[0]
-    g_K1 = parameters[1]
-    g_Kr = parameters[2]
-    g_Ks = parameters[3]
-    g_Na = parameters[4]
-    g_bna = parameters[5]
-    g_CaL = parameters[6]
-    g_bca = parameters[7]
-    g_to = parameters[8]
-    K_mNa = parameters[9]
-    K_mk = parameters[10]
-    P_NaK = parameters[11]
-    K_NaCa = parameters[12]
-    K_sat = parameters[13]
-    Km_Ca = parameters[14]
-    Km_Nai = parameters[15]
-    alpha = parameters[16]
-    gamma = parameters[17]
-    K_pCa = parameters[18]
-    g_pCa = parameters[19]
-    g_pK = parameters[20]
-    Buf_c = parameters[21]
-    Buf_sr = parameters[22]
-    Buf_ss = parameters[23]
-    Ca_o = parameters[24]
-    EC = parameters[25]
-    K_buf_c = parameters[26]
-    K_buf_sr = parameters[27]
-    K_buf_ss = parameters[28]
-    K_up = parameters[29]
-    V_leak = parameters[30]
-    V_rel = parameters[31]
-    V_sr = parameters[32]
-    V_ss = parameters[33]
-    V_xfer = parameters[34]
-    Vmax_up = parameters[35]
-    k1_prime = parameters[36]
-    k2_prime = parameters[37]
-    k3 = parameters[38]
-    k4 = parameters[39]
-    max_sr = parameters[40]
-    min_sr = parameters[41]
-    Na_o = parameters[42]
-    Cm = parameters[43]
-    F = parameters[44]
-    R = parameters[45]
-    T = parameters[46]
-    V_c = parameters[47]
-    K_o = parameters[52]
+    (
+        P_kna,
+        g_K1,
+        g_Kr,
+        g_Ks,
+        g_Na,
+        g_bna,
+        g_CaL,
+        g_bca,
+        g_to,
+        K_mNa,
+        K_mk,
+        P_NaK,
+        K_NaCa,
+        K_sat,
+        Km_Ca,
+        Km_Nai,
+        alpha,
+        gamma,
+        K_pCa,
+        g_pCa,
+        g_pK,
+        Buf_c,
+        Buf_sr,
+        Buf_ss,
+        Ca_o,
+        EC,
+        K_buf_c,
+        K_buf_sr,
+        K_buf_ss,
+        K_up,
+        V_leak,
+        V_rel,
+        V_sr,
+        V_ss,
+        V_xfer,
+        Vmax_up,
+        k1_prime,
+        k2_prime,
+        k3,
+        k4,
+        max_sr,
+        min_sr,
+        Na_o,
+        Cm,
+        F,
+        R,
+        T,
+        V_c,
+        stim_amplitude,
+        stim_duration,
+        stim_period,
+        stim_start,
+        K_o,
+    ) = parameters
 
     # Init return args
     if monitored is None:
-        monitored = np.zeros((89,), dtype=np.float_)
+        monitored = np.zeros((92,), dtype=np.float_)
     else:
-        assert isinstance(monitored, np.ndarray) and monitored.shape == (89,)
+        assert isinstance(monitored, np.ndarray) and monitored.shape == (92,)
 
     # Expressions for the Reversal potentials component
     monitored[0] = R * T * np.log(Na_o / Na_i) / F
     monitored[1] = R * T * np.log(K_o / K_i) / F
     monitored[2] = R * T * np.log((K_o + Na_o * P_kna) / (P_kna * Na_i + K_i)) / F
     monitored[3] = 0.5 * R * T * np.log(Ca_o / Ca_i) / F
 
@@ -895,45 +921,45 @@
     )
 
     # Expressions for the Xr1 gate component
     monitored[9] = 1.0 / (1 + np.exp(-26 / 7 - V / 7))
     monitored[10] = 450 / (1 + np.exp(-9 / 2 - V / 10))
     monitored[11] = 6 / (1 + 13.581324522578193 * np.exp(0.08695652173913043 * V))
     monitored[12] = monitored[10] * monitored[11]
-    monitored[70] = (-Xr1 + monitored[9]) / monitored[12]
+    monitored[73] = (-Xr1 + monitored[9]) / monitored[12]
 
     # Expressions for the Xr2 gate component
     monitored[13] = 1.0 / (1 + np.exp(11 / 3 + V / 24))
     monitored[14] = 3 / (1 + np.exp(-3 - V / 20))
     monitored[15] = 1.12 / (1 + np.exp(-3 + V / 20))
     monitored[16] = monitored[14] * monitored[15]
-    monitored[71] = (-Xr2 + monitored[13]) / monitored[16]
+    monitored[74] = (-Xr2 + monitored[13]) / monitored[16]
 
     # Expressions for the Slow time dependent potassium current component
     monitored[17] = g_Ks * (Xs * Xs) * (-monitored[2] + V)
 
     # Expressions for the Xs gate component
     monitored[18] = 1.0 / (1 + np.exp(-5 / 14 - V / 14))
     monitored[19] = 1400 / np.sqrt(1 + np.exp(5 / 6 - V / 6))
     monitored[20] = 1.0 / (1 + np.exp(-7 / 3 + V / 15))
     monitored[21] = 80 + monitored[19] * monitored[20]
-    monitored[72] = (-Xs + monitored[18]) / monitored[21]
+    monitored[75] = (-Xs + monitored[18]) / monitored[21]
 
     # Expressions for the Fast sodium current component
     monitored[22] = g_Na * (m * m * m) * (-monitored[0] + V) * h * j
 
     # Expressions for the m gate component
     monitored[23] = 1.0 / (
         (1 + 0.0018422115811651339 * np.exp(-0.1107419712070875 * V))
         * (1 + 0.0018422115811651339 * np.exp(-0.1107419712070875 * V))
     )
     monitored[24] = 1.0 / (1 + np.exp(-12 - V / 5))
     monitored[25] = 0.1 / (1 + np.exp(7 + V / 5)) + 0.1 / (1 + np.exp(-1 / 4 + V / 200))
     monitored[26] = monitored[24] * monitored[25]
-    monitored[73] = (-m + monitored[23]) / monitored[26]
+    monitored[76] = (-m + monitored[23]) / monitored[26]
 
     # Expressions for the h gate component
     monitored[27] = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
     )
     monitored[28] = np.where(
@@ -941,15 +967,15 @@
     )
     monitored[29] = np.where(
         V < -40,
         310000 * np.exp(0.3485 * V) + 2.7 * np.exp(0.079 * V),
         0.77 / (0.13 + 0.049758141083938695 * np.exp(-0.0900900900900901 * V)),
     )
     monitored[30] = 1.0 / (monitored[28] + monitored[29])
-    monitored[74] = (-h + monitored[27]) / monitored[30]
+    monitored[77] = (-h + monitored[27]) / monitored[30]
 
     # Expressions for the j gate component
     monitored[31] = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
     )
     monitored[32] = np.where(
@@ -963,15 +989,15 @@
         V < -40,
         0.02424
         * np.exp(-0.01052 * V)
         / (1 + 0.003960868339904256 * np.exp(-0.1378 * V)),
         0.6 * np.exp(0.057 * V) / (1 + 0.040762203978366204 * np.exp(-0.1 * V)),
     )
     monitored[34] = 1.0 / (monitored[32] + monitored[33])
-    monitored[75] = (-j + monitored[31]) / monitored[34]
+    monitored[78] = (-j + monitored[31]) / monitored[34]
 
     # Expressions for the Sodium background current component
     monitored[35] = g_bna * (-monitored[0] + V)
 
     # Expressions for the L_type Ca current component
     monitored[36] = (
         4
@@ -988,57 +1014,57 @@
 
     # Expressions for the d gate component
     monitored[37] = 1.0 / (1 + 0.34415378686541237 * np.exp(-0.13333333333333333 * V))
     monitored[38] = 0.25 + 1.4 / (1 + np.exp(-35 / 13 - V / 13))
     monitored[39] = 1.4 / (1 + np.exp(1 + V / 5))
     monitored[40] = 1.0 / (1 + np.exp(5 / 2 - V / 20))
     monitored[41] = monitored[38] * monitored[39] + monitored[40]
-    monitored[76] = (-d + monitored[37]) / monitored[41]
+    monitored[79] = (-d + monitored[37]) / monitored[41]
 
     # Expressions for the f gate component
     monitored[42] = 1.0 / (1 + np.exp(20 / 7 + V / 7))
     monitored[43] = (
         20
         + 180 / (1 + np.exp(3 + V / 10))
         + 200 / (1 + np.exp(13 / 10 - V / 10))
         + 1102.5 * np.exp(-((27 + V) * (27 + V)) / 225)
     )
-    monitored[77] = (-f + monitored[42]) / monitored[43]
+    monitored[80] = (-f + monitored[42]) / monitored[43]
 
     # Expressions for the F2 gate component
     monitored[44] = 0.33 + 0.67 / (1 + np.exp(5 + V / 7))
     monitored[45] = (
         31 / (1 + np.exp(5 / 2 - V / 10))
         + 80 / (1 + np.exp(3 + V / 10))
         + 562 * np.exp(-((27 + V) * (27 + V)) / 240)
     )
-    monitored[78] = (-f2 + monitored[44]) / monitored[45]
+    monitored[81] = (-f2 + monitored[44]) / monitored[45]
 
     # Expressions for the FCass gate component
     monitored[46] = 0.4 + 0.6 / (1 + 400.0 * (Ca_ss * Ca_ss))
     monitored[47] = 2 + 80 / (1 + 400.0 * (Ca_ss * Ca_ss))
-    monitored[79] = (-fCass + monitored[46]) / monitored[47]
+    monitored[82] = (-fCass + monitored[46]) / monitored[47]
 
     # Expressions for the Calcium background current component
     monitored[48] = g_bca * (-monitored[3] + V)
 
     # Expressions for the Transient outward current component
     monitored[49] = g_to * (-monitored[1] + V) * r * s
 
     # Expressions for the s gate component
     monitored[50] = 1.0 / (1 + np.exp(4 + V / 5))
     monitored[51] = (
         3 + 5 / (1 + np.exp(-4 + V / 5)) + 85 * np.exp(-((45 + V) * (45 + V)) / 320)
     )
-    monitored[80] = (-s + monitored[50]) / monitored[51]
+    monitored[83] = (-s + monitored[50]) / monitored[51]
 
     # Expressions for the r gate component
     monitored[52] = 1.0 / (1 + np.exp(10 / 3 - V / 6))
     monitored[53] = 0.8 + 9.5 * np.exp(-((40 + V) * (40 + V)) / 1800)
-    monitored[81] = (-r + monitored[52]) / monitored[53]
+    monitored[84] = (-r + monitored[52]) / monitored[53]
 
     # Expressions for the Sodium potassium pump current component
     monitored[54] = (
         K_o
         * P_NaK
         * Na_i
         / (
@@ -1080,91 +1106,101 @@
     )
 
     # Expressions for the Calcium dynamics component
     monitored[58] = Vmax_up / (1 + (K_up * K_up) / (Ca_i * Ca_i))
     monitored[59] = V_leak * (-Ca_i + Ca_SR)
     monitored[60] = V_xfer * (-Ca_i + Ca_ss)
     monitored[61] = max_sr - (max_sr - min_sr) / (1 + (EC * EC) / (Ca_SR * Ca_SR))
-    monitored[62] = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
-    monitored[63] = 1.0 / (
-        1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR))
+    monitored[62] = (
+        V_sr * (-monitored[58] + monitored[59]) / V_c
+        + Cm * (-monitored[48] - monitored[56] + 2 * monitored[55]) / (2 * F * V_c)
+        + monitored[60]
     )
+    monitored[63] = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
     monitored[64] = 1.0 / (
+        1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR))
+    )
+    monitored[65] = 1.0 / (
         1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss))
     )
-    monitored[82] = (
-        V_sr * (-monitored[58] + monitored[59]) / V_c
-        - Cm * (-2 * monitored[55] + monitored[48] + monitored[56]) / (2 * F * V_c)
-        + monitored[60]
-    ) * monitored[62]
-    monitored[65] = k1_prime / monitored[61]
-    monitored[66] = k2_prime * monitored[61]
-    monitored[67] = (
+    monitored[85] = monitored[62] * monitored[63]
+    monitored[66] = k1_prime / monitored[61]
+    monitored[67] = k2_prime * monitored[61]
+    monitored[68] = (
         (Ca_ss * Ca_ss)
         * R_prime
-        * monitored[65]
-        / (k3 + (Ca_ss * Ca_ss) * monitored[65])
+        * monitored[66]
+        / (k3 + (Ca_ss * Ca_ss) * monitored[66])
     )
-    monitored[83] = k4 * (1 - R_prime) - Ca_ss * R_prime * monitored[66]
-    monitored[68] = V_rel * (-Ca_ss + Ca_SR) * monitored[67]
-    monitored[84] = (-monitored[59] - monitored[68] + monitored[58]) * monitored[63]
-    monitored[85] = (
-        V_sr * monitored[68] / V_ss
+    monitored[86] = k4 * (1 - R_prime) - Ca_ss * R_prime * monitored[67]
+    monitored[69] = V_rel * (-Ca_ss + Ca_SR) * monitored[68]
+    monitored[70] = -monitored[59] - monitored[69] + monitored[58]
+    monitored[71] = (
+        V_sr * monitored[69] / V_ss
         - V_c * monitored[60] / V_ss
         - Cm * monitored[36] / (2 * F * V_ss)
-    ) * monitored[64]
+    )
+    monitored[87] = monitored[64] * monitored[70]
+    monitored[88] = monitored[65] * monitored[71]
 
     # Expressions for the Sodium dynamics component
-    monitored[86] = (
+    monitored[89] = (
         Cm
         * (-monitored[22] - monitored[35] - 3 * monitored[54] - 3 * monitored[55])
         / (F * V_c)
     )
 
     # Expressions for the Membrane component
-    monitored[69] = 0
-    monitored[87] = (
-        -monitored[69]
-        - monitored[17]
+    monitored[72] = np.where(
+        np.logical_and(
+            t - stim_period * np.floor(t / stim_period) >= stim_start,
+            t - stim_period * np.floor(t / stim_period) <= stim_duration + stim_start,
+        ),
+        stim_amplitude,
+        0,
+    )
+    monitored[90] = (
+        -monitored[17]
         - monitored[22]
         - monitored[35]
         - monitored[36]
         - monitored[48]
         - monitored[49]
         - monitored[54]
         - monitored[55]
         - monitored[56]
         - monitored[57]
+        - monitored[72]
         - monitored[7]
         - monitored[8]
     )
 
     # Expressions for the Potassium dynamics component
-    monitored[88] = (
+    monitored[91] = (
         Cm
         * (
-            -monitored[69]
-            - monitored[17]
+            -monitored[17]
             - monitored[49]
             - monitored[57]
+            - monitored[72]
             - monitored[7]
             - monitored[8]
             + 2 * monitored[54]
         )
         / (F * V_c)
     )
 
     # Return results
     return monitored
 
 
 def forward_explicit_euler(states, t, dt, parameters):
     """
     Compute a forward step using the explicit Euler scheme to the\
-        tentusscher_panfilov_2006_M_cell ODE
+        tentusscher_panfilov_2006_epi_cell ODE
     """
 
     # Assign states
     assert len(states) == 19
     (
         Xr1,
         Xr2,
@@ -1185,63 +1221,69 @@
         Na_i,
         V,
         K_i,
     ) = states
 
     # Assign parameters
     assert len(parameters) == 53
-    P_kna = parameters[0]
-    g_K1 = parameters[1]
-    g_Kr = parameters[2]
-    g_Ks = parameters[3]
-    g_Na = parameters[4]
-    g_bna = parameters[5]
-    g_CaL = parameters[6]
-    g_bca = parameters[7]
-    g_to = parameters[8]
-    K_mNa = parameters[9]
-    K_mk = parameters[10]
-    P_NaK = parameters[11]
-    K_NaCa = parameters[12]
-    K_sat = parameters[13]
-    Km_Ca = parameters[14]
-    Km_Nai = parameters[15]
-    alpha = parameters[16]
-    gamma = parameters[17]
-    K_pCa = parameters[18]
-    g_pCa = parameters[19]
-    g_pK = parameters[20]
-    Buf_c = parameters[21]
-    Buf_sr = parameters[22]
-    Buf_ss = parameters[23]
-    Ca_o = parameters[24]
-    EC = parameters[25]
-    K_buf_c = parameters[26]
-    K_buf_sr = parameters[27]
-    K_buf_ss = parameters[28]
-    K_up = parameters[29]
-    V_leak = parameters[30]
-    V_rel = parameters[31]
-    V_sr = parameters[32]
-    V_ss = parameters[33]
-    V_xfer = parameters[34]
-    Vmax_up = parameters[35]
-    k1_prime = parameters[36]
-    k2_prime = parameters[37]
-    k3 = parameters[38]
-    k4 = parameters[39]
-    max_sr = parameters[40]
-    min_sr = parameters[41]
-    Na_o = parameters[42]
-    Cm = parameters[43]
-    F = parameters[44]
-    R = parameters[45]
-    T = parameters[46]
-    V_c = parameters[47]
-    K_o = parameters[52]
+    (
+        P_kna,
+        g_K1,
+        g_Kr,
+        g_Ks,
+        g_Na,
+        g_bna,
+        g_CaL,
+        g_bca,
+        g_to,
+        K_mNa,
+        K_mk,
+        P_NaK,
+        K_NaCa,
+        K_sat,
+        Km_Ca,
+        Km_Nai,
+        alpha,
+        gamma,
+        K_pCa,
+        g_pCa,
+        g_pK,
+        Buf_c,
+        Buf_sr,
+        Buf_ss,
+        Ca_o,
+        EC,
+        K_buf_c,
+        K_buf_sr,
+        K_buf_ss,
+        K_up,
+        V_leak,
+        V_rel,
+        V_sr,
+        V_ss,
+        V_xfer,
+        Vmax_up,
+        k1_prime,
+        k2_prime,
+        k3,
+        k4,
+        max_sr,
+        min_sr,
+        Na_o,
+        Cm,
+        F,
+        R,
+        T,
+        V_c,
+        stim_amplitude,
+        stim_duration,
+        stim_period,
+        stim_start,
+        K_o,
+    ) = parameters
 
     # Expressions for the Reversal potentials component
     E_Na = R * T * np.log(Na_o / Na_i) / F
     E_K = R * T * np.log(K_o / K_i) / F
     E_Ks = R * T * np.log((K_o + Na_o * P_kna) / (P_kna * Na_i + K_i)) / F
     E_Ca = 0.5 * R * T * np.log(Ca_o / Ca_i) / F
 
@@ -1451,75 +1493,85 @@
     )
 
     # Expressions for the Calcium dynamics component
     i_up = Vmax_up / (1 + (K_up * K_up) / (Ca_i * Ca_i))
     i_leak = V_leak * (-Ca_i + Ca_SR)
     i_xfer = V_xfer * (-Ca_i + Ca_ss)
     kcasr = max_sr - (max_sr - min_sr) / (1 + (EC * EC) / (Ca_SR * Ca_SR))
-    Ca_i_bufc = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
-    Ca_sr_bufsr = 1.0 / (
+    ddt_Ca_i_total = (
+        V_sr * (-i_up + i_leak) / V_c
+        + Cm * (-i_b_Ca - i_p_Ca + 2 * i_NaCa) / (2 * F * V_c)
+        + i_xfer
+    )
+    f_JCa_i_free = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
+    f_JCa_sr_free = 1.0 / (
         1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR))
     )
-    Ca_ss_bufss = 1.0 / (
+    f_JCa_ss_free = 1.0 / (
         1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss))
     )
-    dCa_i_dt = (
-        V_sr * (-i_up + i_leak) / V_c
-        - Cm * (-2 * i_NaCa + i_b_Ca + i_p_Ca) / (2 * F * V_c)
-        + i_xfer
-    ) * Ca_i_bufc
+    dCa_i_dt = ddt_Ca_i_total * f_JCa_i_free
     states[12] = dt * dCa_i_dt + Ca_i
     k1 = k1_prime / kcasr
     k2 = k2_prime * kcasr
     O = (Ca_ss * Ca_ss) * R_prime * k1 / (k3 + (Ca_ss * Ca_ss) * k1)
     dR_prime_dt = k4 * (1 - R_prime) - Ca_ss * R_prime * k2
     states[13] = dt * dR_prime_dt + R_prime
     i_rel = V_rel * (-Ca_ss + Ca_SR) * O
-    dCa_SR_dt = (-i_leak - i_rel + i_up) * Ca_sr_bufsr
-    states[14] = dt * dCa_SR_dt + Ca_SR
-    dCa_ss_dt = (
+    ddt_Ca_sr_total = -i_leak - i_rel + i_up
+    ddt_Ca_ss_total = (
         V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
-    ) * Ca_ss_bufss
+    )
+    dCa_SR_dt = ddt_Ca_sr_total * f_JCa_sr_free
+    states[14] = dt * dCa_SR_dt + Ca_SR
+    dCa_ss_dt = ddt_Ca_ss_total * f_JCa_ss_free
     states[15] = dt * dCa_ss_dt + Ca_ss
 
     # Expressions for the Sodium dynamics component
     dNa_i_dt = Cm * (-i_Na - i_b_Na - 3 * i_NaCa - 3 * i_NaK) / (F * V_c)
     states[16] = dt * dNa_i_dt + Na_i
 
     # Expressions for the Membrane component
-    i_Stim = 0
+    i_Stim = np.where(
+        np.logical_and(
+            t - stim_period * np.floor(t / stim_period) >= stim_start,
+            t - stim_period * np.floor(t / stim_period) <= stim_duration + stim_start,
+        ),
+        stim_amplitude,
+        0,
+    )
     dV_dt = (
-        -i_Stim
-        - i_CaL
+        -i_CaL
         - i_K1
         - i_Kr
         - i_Ks
         - i_Na
         - i_NaCa
         - i_NaK
+        - i_Stim
         - i_b_Ca
         - i_b_Na
         - i_p_Ca
         - i_p_K
         - i_to
     )
     states[17] = dt * dV_dt + V
 
     # Expressions for the Potassium dynamics component
-    dK_i_dt = Cm * (-i_Stim - i_K1 - i_Kr - i_Ks - i_p_K - i_to + 2 * i_NaK) / (F * V_c)
+    dK_i_dt = Cm * (-i_K1 - i_Kr - i_Ks - i_Stim - i_p_K - i_to + 2 * i_NaK) / (F * V_c)
     states[18] = dt * dK_i_dt + K_i
 
     # Return results
     return states
 
 
 def forward_generalized_rush_larsen(states, t, dt, parameters):
     """
     Compute a forward step using the generalised Rush-Larsen (GRL1) scheme to\
-        the tentusscher_panfilov_2006_M_cell ODE
+        the tentusscher_panfilov_2006_epi_cell ODE
     """
 
     # Assign states
     assert len(states) == 19
     (
         Xr1,
         Xr2,
@@ -1540,63 +1592,69 @@
         Na_i,
         V,
         K_i,
     ) = states
 
     # Assign parameters
     assert len(parameters) == 53
-    P_kna = parameters[0]
-    g_K1 = parameters[1]
-    g_Kr = parameters[2]
-    g_Ks = parameters[3]
-    g_Na = parameters[4]
-    g_bna = parameters[5]
-    g_CaL = parameters[6]
-    g_bca = parameters[7]
-    g_to = parameters[8]
-    K_mNa = parameters[9]
-    K_mk = parameters[10]
-    P_NaK = parameters[11]
-    K_NaCa = parameters[12]
-    K_sat = parameters[13]
-    Km_Ca = parameters[14]
-    Km_Nai = parameters[15]
-    alpha = parameters[16]
-    gamma = parameters[17]
-    K_pCa = parameters[18]
-    g_pCa = parameters[19]
-    g_pK = parameters[20]
-    Buf_c = parameters[21]
-    Buf_sr = parameters[22]
-    Buf_ss = parameters[23]
-    Ca_o = parameters[24]
-    EC = parameters[25]
-    K_buf_c = parameters[26]
-    K_buf_sr = parameters[27]
-    K_buf_ss = parameters[28]
-    K_up = parameters[29]
-    V_leak = parameters[30]
-    V_rel = parameters[31]
-    V_sr = parameters[32]
-    V_ss = parameters[33]
-    V_xfer = parameters[34]
-    Vmax_up = parameters[35]
-    k1_prime = parameters[36]
-    k2_prime = parameters[37]
-    k3 = parameters[38]
-    k4 = parameters[39]
-    max_sr = parameters[40]
-    min_sr = parameters[41]
-    Na_o = parameters[42]
-    Cm = parameters[43]
-    F = parameters[44]
-    R = parameters[45]
-    T = parameters[46]
-    V_c = parameters[47]
-    K_o = parameters[52]
+    (
+        P_kna,
+        g_K1,
+        g_Kr,
+        g_Ks,
+        g_Na,
+        g_bna,
+        g_CaL,
+        g_bca,
+        g_to,
+        K_mNa,
+        K_mk,
+        P_NaK,
+        K_NaCa,
+        K_sat,
+        Km_Ca,
+        Km_Nai,
+        alpha,
+        gamma,
+        K_pCa,
+        g_pCa,
+        g_pK,
+        Buf_c,
+        Buf_sr,
+        Buf_ss,
+        Ca_o,
+        EC,
+        K_buf_c,
+        K_buf_sr,
+        K_buf_ss,
+        K_up,
+        V_leak,
+        V_rel,
+        V_sr,
+        V_ss,
+        V_xfer,
+        Vmax_up,
+        k1_prime,
+        k2_prime,
+        k3,
+        k4,
+        max_sr,
+        min_sr,
+        Na_o,
+        Cm,
+        F,
+        R,
+        T,
+        V_c,
+        stim_amplitude,
+        stim_duration,
+        stim_period,
+        stim_start,
+        K_o,
+    ) = parameters
 
     # Expressions for the Reversal potentials component
     E_Na = R * T * np.log(Na_o / Na_i) / F
     E_K = R * T * np.log(K_o / K_i) / F
     E_Ks = R * T * np.log((K_o + Na_o * P_kna) / (P_kna * Na_i + K_i)) / F
     E_Ca = 0.5 * R * T * np.log(Ca_o / Ca_i) / F
 
@@ -1824,39 +1882,45 @@
     )
 
     # Expressions for the Calcium dynamics component
     i_up = Vmax_up / (1 + (K_up * K_up) / (Ca_i * Ca_i))
     i_leak = V_leak * (-Ca_i + Ca_SR)
     i_xfer = V_xfer * (-Ca_i + Ca_ss)
     kcasr = max_sr - (max_sr - min_sr) / (1 + (EC * EC) / (Ca_SR * Ca_SR))
-    Ca_i_bufc = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
-    Ca_sr_bufsr = 1.0 / (
+    ddt_Ca_i_total = (
+        V_sr * (-i_up + i_leak) / V_c
+        + Cm * (-i_b_Ca - i_p_Ca + 2 * i_NaCa) / (2 * F * V_c)
+        + i_xfer
+    )
+    f_JCa_i_free = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
+    f_JCa_sr_free = 1.0 / (
         1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR))
     )
-    Ca_ss_bufss = 1.0 / (
+    f_JCa_ss_free = 1.0 / (
         1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss))
     )
-    dCa_i_dt = (
-        V_sr * (-i_up + i_leak) / V_c
-        - Cm * (-2 * i_NaCa + i_b_Ca + i_p_Ca) / (2 * F * V_c)
-        + i_xfer
-    ) * Ca_i_bufc
-    dCa_i_bufc_dCa_i = (
+    dCa_i_dt = ddt_Ca_i_total * f_JCa_i_free
+    dE_Ca_dCa_i = -0.5 * R * T / (F * Ca_i)
+    dddt_Ca_i_total_di_NaCa = Cm / (F * V_c)
+    dddt_Ca_i_total_di_b_Ca = -Cm / (2 * F * V_c)
+    dddt_Ca_i_total_di_leak = V_sr / V_c
+    dddt_Ca_i_total_di_p_Ca = -Cm / (2 * F * V_c)
+    dddt_Ca_i_total_di_up = -V_sr / V_c
+    df_JCa_i_free_dCa_i = (
         2
         * Buf_c
         * K_buf_c
         / (
             (
                 (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
                 * (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
             )
             * ((K_buf_c + Ca_i) * (K_buf_c + Ca_i) * (K_buf_c + Ca_i))
         )
     )
-    dE_Ca_dCa_i = -0.5 * R * T / (F * Ca_i)
     di_NaCa_dCa_i = (
         -K_NaCa
         * alpha
         * (Na_o * Na_o * Na_o)
         * np.exp(F * (-1 + gamma) * V / (R * T))
         / (
             (1 + K_sat * np.exp(F * (-1 + gamma) * V / (R * T)))
@@ -1874,23 +1938,20 @@
         / (
             ((1 + (K_up * K_up) / (Ca_i * Ca_i)) * (1 + (K_up * K_up) / (Ca_i * Ca_i)))
             * (Ca_i * Ca_i * Ca_i)
         )
     )
     dCa_i_dt_linearized = (
         -V_xfer
-        + V_sr * (-V_leak - di_up_dCa_i) / V_c
-        - Cm
-        * (-2 * di_NaCa_dCa_i - g_bca * dE_Ca_dCa_i + di_p_Ca_dCa_i)
-        / (2 * F * V_c)
-    ) * Ca_i_bufc + (
-        V_sr * (-i_up + i_leak) / V_c
-        - Cm * (-2 * i_NaCa + i_b_Ca + i_p_Ca) / (2 * F * V_c)
-        + i_xfer
-    ) * dCa_i_bufc_dCa_i
+        + dddt_Ca_i_total_di_NaCa * di_NaCa_dCa_i
+        + dddt_Ca_i_total_di_p_Ca * di_p_Ca_dCa_i
+        + dddt_Ca_i_total_di_up * di_up_dCa_i
+        - V_leak * dddt_Ca_i_total_di_leak
+        - g_bca * dE_Ca_dCa_i * dddt_Ca_i_total_di_b_Ca
+    ) * f_JCa_i_free + ddt_Ca_i_total * df_JCa_i_free_dCa_i
     states[12] = Ca_i + np.where(
         np.abs(dCa_i_dt_linearized) > 1e-08,
         (-1 + np.exp(dt * dCa_i_dt_linearized)) * dCa_i_dt / dCa_i_dt_linearized,
         dt * dCa_i_dt,
     )
     k1 = k1_prime / kcasr
     k2 = k2_prime * kcasr
@@ -1904,30 +1965,34 @@
             * dR_prime_dt
             / dR_prime_dt_linearized,
             dt * dR_prime_dt,
         )
         + R_prime
     )
     i_rel = V_rel * (-Ca_ss + Ca_SR) * O
-    dCa_SR_dt = (-i_leak - i_rel + i_up) * Ca_sr_bufsr
-    dCa_sr_bufsr_dCa_SR = (
+    ddt_Ca_sr_total = -i_leak - i_rel + i_up
+    ddt_Ca_ss_total = (
+        V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
+    )
+    dCa_SR_dt = ddt_Ca_sr_total * f_JCa_sr_free
+    dO_dk1 = (Ca_ss * Ca_ss) * R_prime / (k3 + (Ca_ss * Ca_ss) * k1) - np.power(
+        Ca_ss, 4
+    ) * R_prime * k1 / ((k3 + (Ca_ss * Ca_ss) * k1) * (k3 + (Ca_ss * Ca_ss) * k1))
+    df_JCa_sr_free_dCa_SR = (
         2
         * Buf_sr
         * K_buf_sr
         / (
             (
                 (1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR)))
                 * (1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR)))
             )
             * ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR))
         )
     )
-    dO_dk1 = (Ca_ss * Ca_ss) * R_prime / (k3 + (Ca_ss * Ca_ss) * k1) - np.power(
-        Ca_ss, 4
-    ) * R_prime * k1 / ((k3 + (Ca_ss * Ca_ss) * k1) * (k3 + (Ca_ss * Ca_ss) * k1))
     dk1_dkcasr = -k1_prime / (kcasr * kcasr)
     dkcasr_dCa_SR = (
         -2
         * (EC * EC)
         * (max_sr - min_sr)
         / (
             ((1 + (EC * EC) / (Ca_SR * Ca_SR)) * (1 + (EC * EC) / (Ca_SR * Ca_SR)))
@@ -1936,58 +2001,57 @@
     )
     di_rel_dCa_SR = (
         V_rel * O + V_rel * (-Ca_ss + Ca_SR) * dO_dk1 * dk1_dkcasr * dkcasr_dCa_SR
     )
     di_rel_dO = V_rel * (-Ca_ss + Ca_SR)
     dCa_SR_dt_linearized = (
         -V_leak - di_rel_dCa_SR - dO_dk1 * di_rel_dO * dk1_dkcasr * dkcasr_dCa_SR
-    ) * Ca_sr_bufsr + (-i_leak - i_rel + i_up) * dCa_sr_bufsr_dCa_SR
+    ) * f_JCa_sr_free + ddt_Ca_sr_total * df_JCa_sr_free_dCa_SR
     states[14] = Ca_SR + np.where(
         np.abs(dCa_SR_dt_linearized) > 1e-08,
         (-1 + np.exp(dt * dCa_SR_dt_linearized)) * dCa_SR_dt / dCa_SR_dt_linearized,
         dt * dCa_SR_dt,
     )
-    dCa_ss_dt = (
-        V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
-    ) * Ca_ss_bufss
-    dCa_ss_bufss_dCa_ss = (
+    dCa_ss_dt = ddt_Ca_ss_total * f_JCa_ss_free
+    dO_dCa_ss = -2 * (Ca_ss * Ca_ss * Ca_ss) * (k1 * k1) * R_prime / (
+        (k3 + (Ca_ss * Ca_ss) * k1) * (k3 + (Ca_ss * Ca_ss) * k1)
+    ) + 2 * Ca_ss * R_prime * k1 / (k3 + (Ca_ss * Ca_ss) * k1)
+    dddt_Ca_ss_total_di_CaL = -Cm / (2 * F * V_ss)
+    dddt_Ca_ss_total_di_rel = V_sr / V_ss
+    dddt_Ca_ss_total_di_xfer = -V_c / V_ss
+    df_JCa_ss_free_dCa_ss = (
         2
         * Buf_ss
         * K_buf_ss
         / (
             (
                 (1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss)))
                 * (1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss)))
             )
             * ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss))
         )
     )
-    dO_dCa_ss = -2 * (Ca_ss * Ca_ss * Ca_ss) * (k1 * k1) * R_prime / (
-        (k3 + (Ca_ss * Ca_ss) * k1) * (k3 + (Ca_ss * Ca_ss) * k1)
-    ) + 2 * Ca_ss * R_prime * k1 / (k3 + (Ca_ss * Ca_ss) * k1)
     di_CaL_dCa_ss = (
         1.0
         * g_CaL
         * (F * F)
         * (-15 + V)
         * d
         * np.exp(F * (-30 + 2 * V) / (R * T))
         * f
         * f2
         * fCass
         / (R * T * (-1 + np.exp(F * (-30 + 2 * V) / (R * T))))
     )
     di_rel_dCa_ss = -V_rel * O + V_rel * (-Ca_ss + Ca_SR) * dO_dCa_ss
     dCa_ss_dt_linearized = (
-        V_sr * (dO_dCa_ss * di_rel_dO + di_rel_dCa_ss) / V_ss
-        - V_c * V_xfer / V_ss
-        - Cm * di_CaL_dCa_ss / (2 * F * V_ss)
-    ) * Ca_ss_bufss + (
-        V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
-    ) * dCa_ss_bufss_dCa_ss
+        V_xfer * dddt_Ca_ss_total_di_xfer
+        + (dO_dCa_ss * di_rel_dO + di_rel_dCa_ss) * dddt_Ca_ss_total_di_rel
+        + dddt_Ca_ss_total_di_CaL * di_CaL_dCa_ss
+    ) * f_JCa_ss_free + ddt_Ca_ss_total * df_JCa_ss_free_dCa_ss
     states[15] = Ca_ss + np.where(
         np.abs(dCa_ss_dt_linearized) > 1e-08,
         (-1 + np.exp(dt * dCa_ss_dt_linearized)) * dCa_ss_dt / dCa_ss_dt_linearized,
         dt * dCa_ss_dt,
     )
 
     # Expressions for the Sodium dynamics component
@@ -2036,24 +2100,31 @@
     states[16] = Na_i + np.where(
         np.abs(dNa_i_dt_linearized) > 1e-08,
         (-1 + np.exp(dt * dNa_i_dt_linearized)) * dNa_i_dt / dNa_i_dt_linearized,
         dt * dNa_i_dt,
     )
 
     # Expressions for the Membrane component
-    i_Stim = 0
+    i_Stim = np.where(
+        np.logical_and(
+            t - stim_period * np.floor(t / stim_period) >= stim_start,
+            t - stim_period * np.floor(t / stim_period) <= stim_duration + stim_start,
+        ),
+        stim_amplitude,
+        0,
+    )
     dV_dt = (
-        -i_Stim
-        - i_CaL
+        -i_CaL
         - i_K1
         - i_Kr
         - i_Ks
         - i_Na
         - i_NaCa
         - i_NaK
+        - i_Stim
         - i_b_Ca
         - i_b_Na
         - i_p_Ca
         - i_p_K
         - i_to
     )
     dalpha_K1_dV = (
@@ -2216,15 +2287,15 @@
             (-1 + np.exp(dt * dV_dt_linearized)) * dV_dt / dV_dt_linearized,
             dt * dV_dt,
         )
         + V
     )
 
     # Expressions for the Potassium dynamics component
-    dK_i_dt = Cm * (-i_Stim - i_K1 - i_Kr - i_Ks - i_p_K - i_to + 2 * i_NaK) / (F * V_c)
+    dK_i_dt = Cm * (-i_K1 - i_Kr - i_Ks - i_Stim - i_p_K - i_to + 2 * i_NaK) / (F * V_c)
     dE_K_dK_i = -R * T / (F * K_i)
     dE_Ks_dK_i = -R * T / (F * (P_kna * Na_i + K_i))
     dalpha_K1_dE_K = (
         3.686527411996926e-08
         * np.exp(0.06 * V - 0.06 * E_K)
         / (
             (1 + 6.14421235332821e-06 * np.exp(0.06 * V - 0.06 * E_K))
```

### Comparing `fenics-beat-0.0.2/src/beat/cellmodels/tentusscher_panfilov_2006_epi_cell.py` & `fenics-beat-0.0.3/src/beat/cellmodels/tentusscher_panfilov_2006/mid.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# Gotran generated code for the "tentusscher_panfilov_2006_epi_cell" model
+# Gotran generated code for the "tentusscher_panfilov_2006_M_cell" model
 
 import numpy as np
 
 
 def init_state_values(**values):
     """
     Initialize state values
     """
     # Init values
-    # Xr1=0.00621, Xr2=0.4712, Xs=0.0095, m=0.00172, h=0.7444, j=0.7045,
-    # d=3.373e-05, f=0.7888, f2=0.9755, fCass=0.9953, s=0.999998,
-    # r=2.42e-08, Ca_i=0.000126, R_prime=0.9073, Ca_SR=3.64,
-    # Ca_ss=0.00036, Na_i=8.604, V=-85.23, K_i=136.89
+    # Xr1=0.0165, Xr2=0.473, Xs=0.0174, m=0.00165, h=0.749, j=0.6788,
+    # d=3.288e-05, f=0.7026, f2=0.9526, fCass=0.9942, s=0.999998,
+    # r=2.347e-08, Ca_i=0.000153, R_prime=0.8978, Ca_SR=4.272,
+    # Ca_ss=0.00042, Na_i=10.132, V=-85.423, K_i=138.52
     init_values = np.array(
         [
-            0.00621,
-            0.4712,
-            0.0095,
-            0.00172,
-            0.7444,
-            0.7045,
-            3.373e-05,
-            0.7888,
-            0.9755,
-            0.9953,
+            0.0165,
+            0.473,
+            0.0174,
+            0.00165,
+            0.749,
+            0.6788,
+            3.288e-05,
+            0.7026,
+            0.9526,
+            0.9942,
             0.999998,
-            2.42e-08,
-            0.000126,
-            0.9073,
-            3.64,
-            0.00036,
-            8.604,
-            -85.23,
-            136.89,
+            2.347e-08,
+            0.000153,
+            0.8978,
+            4.272,
+            0.00042,
+            10.132,
+            -85.423,
+            138.52,
         ],
         dtype=np.float_,
     )
 
     # State indices and limit checker
     state_ind = dict(
         [
@@ -74,80 +74,80 @@
 
 
 def init_parameter_values(**values):
     """
     Initialize parameter values
     """
     # Param values
-    # P_kna=0.03, g_K1=5.405, g_Kr=0.153, g_Ks=0.392, g_Na=14.838,
-    # g_bna=0.00029, g_CaL=3.98e-05, g_bca=0.000592, g_to=0.294,
-    # K_mNa=40, K_mk=1, P_NaK=2.724, K_NaCa=1000, K_sat=0.1,
+    # P_kna=0.03, g_K1=5.405, g_Kr=0.153, g_Ks=0.098, g_Na=14.838,
+    # g_bna=0.00029, g_CaL=0.0398, g_bca=0.000592, g_to=0.294,
+    # K_mNa=40.0, K_mk=1.0, P_NaK=2.724, K_NaCa=1000.0, K_sat=0.1,
     # Km_Ca=1.38, Km_Nai=87.5, alpha=2.5, gamma=0.35, K_pCa=0.0005,
-    # g_pCa=0.1238, g_pK=0.0146, Buf_c=0.2, Buf_sr=10, Buf_ss=0.4,
-    # Ca_o=2, EC=1.5, K_buf_c=0.001, K_buf_sr=0.3, K_buf_ss=0.00025,
-    # K_up=0.00025, V_leak=0.00036, V_rel=0.102, V_sr=0.001094,
-    # V_ss=5.468e-05, V_xfer=0.0038, Vmax_up=0.006375, k1_prime=0.15,
+    # g_pCa=0.1238, g_pK=0.0146, Buf_c=0.2, Buf_sr=10.0, Buf_ss=0.4,
+    # Ca_o=2.0, EC=1.5, K_buf_c=0.001, K_buf_sr=0.3, K_buf_ss=0.00025,
+    # K_up=0.00025, V_leak=0.00036, V_rel=0.102, V_sr=1094.0,
+    # V_ss=54.68, V_xfer=0.0038, Vmax_up=0.006375, k1_prime=0.15,
     # k2_prime=0.045, k3=0.06, k4=0.005, max_sr=2.5, min_sr=1,
-    # Na_o=140, Cm=0.185, F=96485.3415, R=8314.472, T=310,
-    # V_c=0.016404, stim_amplitude=0, stim_duration=1, stim_period=1000,
-    # stim_start=10, K_o=5.4
+    # Na_o=140.0, Cm=185.0, F=96.485, R=8.314, T=310.0, V_c=16404.0,
+    # stim_amplitude=-52.0, stim_duration=1.0, stim_period=1000.0,
+    # stim_start=10.0, K_o=5.4
     init_values = np.array(
         [
             0.03,
             5.405,
             0.153,
-            0.392,
+            0.098,
             14.838,
             0.00029,
-            3.98e-05,
+            0.0398,
             0.000592,
             0.294,
-            40,
-            1,
+            40.0,
+            1.0,
             2.724,
-            1000,
+            1000.0,
             0.1,
             1.38,
             87.5,
             2.5,
             0.35,
             0.0005,
             0.1238,
             0.0146,
             0.2,
-            10,
+            10.0,
             0.4,
-            2,
+            2.0,
             1.5,
             0.001,
             0.3,
             0.00025,
             0.00025,
             0.00036,
             0.102,
-            0.001094,
-            5.468e-05,
+            1094.0,
+            54.68,
             0.0038,
             0.006375,
             0.15,
             0.045,
             0.06,
             0.005,
             2.5,
             1,
-            140,
-            0.185,
-            96485.3415,
-            8314.472,
-            310,
-            0.016404,
-            0,
-            1,
-            1000,
-            10,
+            140.0,
+            185.0,
+            96.485,
+            8.314,
+            310.0,
+            16404.0,
+            -52.0,
+            1.0,
+            1000.0,
+            10.0,
             5.4,
         ],
         dtype=np.float_,
     )
 
     # Parameter indices and limit checker
     param_ind = dict(
@@ -395,41 +395,44 @@
             ("i_NaCa", 55),
             ("i_p_Ca", 56),
             ("i_p_K", 57),
             ("i_up", 58),
             ("i_leak", 59),
             ("i_xfer", 60),
             ("kcasr", 61),
-            ("Ca_i_bufc", 62),
-            ("Ca_sr_bufsr", 63),
-            ("Ca_ss_bufss", 64),
-            ("k1", 65),
-            ("k2", 66),
-            ("O", 67),
-            ("i_rel", 68),
-            ("i_Stim", 69),
-            ("dXr1_dt", 70),
-            ("dXr2_dt", 71),
-            ("dXs_dt", 72),
-            ("dm_dt", 73),
-            ("dh_dt", 74),
-            ("dj_dt", 75),
-            ("dd_dt", 76),
-            ("df_dt", 77),
-            ("df2_dt", 78),
-            ("dfCass_dt", 79),
-            ("ds_dt", 80),
-            ("dr_dt", 81),
-            ("dCa_i_dt", 82),
-            ("dR_prime_dt", 83),
-            ("dCa_SR_dt", 84),
-            ("dCa_ss_dt", 85),
-            ("dNa_i_dt", 86),
-            ("dV_dt", 87),
-            ("dK_i_dt", 88),
+            ("ddt_Ca_i_total", 62),
+            ("f_JCa_i_free", 63),
+            ("f_JCa_sr_free", 64),
+            ("f_JCa_ss_free", 65),
+            ("k1", 66),
+            ("k2", 67),
+            ("O", 68),
+            ("i_rel", 69),
+            ("ddt_Ca_sr_total", 70),
+            ("ddt_Ca_ss_total", 71),
+            ("i_Stim", 72),
+            ("dXr1_dt", 73),
+            ("dXr2_dt", 74),
+            ("dXs_dt", 75),
+            ("dm_dt", 76),
+            ("dh_dt", 77),
+            ("dj_dt", 78),
+            ("dd_dt", 79),
+            ("df_dt", 80),
+            ("df2_dt", 81),
+            ("dfCass_dt", 82),
+            ("ds_dt", 83),
+            ("dr_dt", 84),
+            ("dCa_i_dt", 85),
+            ("dR_prime_dt", 86),
+            ("dCa_SR_dt", 87),
+            ("dCa_ss_dt", 88),
+            ("dNa_i_dt", 89),
+            ("dV_dt", 90),
+            ("dK_i_dt", 91),
         ]
     )
 
     indices = []
     for monitor in monitored:
         if monitor not in monitor_inds:
             raise ValueError("Unknown monitored: '{0}'".format(monitor))
@@ -438,15 +441,15 @@
         return indices
     else:
         return indices[0]
 
 
 def rhs(states, t, parameters, values=None):
     """
-    Compute the right hand side of the tentusscher_panfilov_2006_epi_cell ODE
+    Compute the right hand side of the tentusscher_panfilov_2006_M_cell ODE
     """
 
     # Assign states
     assert len(states) == 19
     (
         Xr1,
         Xr2,
@@ -467,63 +470,69 @@
         Na_i,
         V,
         K_i,
     ) = states
 
     # Assign parameters
     assert len(parameters) == 53
-    P_kna = parameters[0]
-    g_K1 = parameters[1]
-    g_Kr = parameters[2]
-    g_Ks = parameters[3]
-    g_Na = parameters[4]
-    g_bna = parameters[5]
-    g_CaL = parameters[6]
-    g_bca = parameters[7]
-    g_to = parameters[8]
-    K_mNa = parameters[9]
-    K_mk = parameters[10]
-    P_NaK = parameters[11]
-    K_NaCa = parameters[12]
-    K_sat = parameters[13]
-    Km_Ca = parameters[14]
-    Km_Nai = parameters[15]
-    alpha = parameters[16]
-    gamma = parameters[17]
-    K_pCa = parameters[18]
-    g_pCa = parameters[19]
-    g_pK = parameters[20]
-    Buf_c = parameters[21]
-    Buf_sr = parameters[22]
-    Buf_ss = parameters[23]
-    Ca_o = parameters[24]
-    EC = parameters[25]
-    K_buf_c = parameters[26]
-    K_buf_sr = parameters[27]
-    K_buf_ss = parameters[28]
-    K_up = parameters[29]
-    V_leak = parameters[30]
-    V_rel = parameters[31]
-    V_sr = parameters[32]
-    V_ss = parameters[33]
-    V_xfer = parameters[34]
-    Vmax_up = parameters[35]
-    k1_prime = parameters[36]
-    k2_prime = parameters[37]
-    k3 = parameters[38]
-    k4 = parameters[39]
-    max_sr = parameters[40]
-    min_sr = parameters[41]
-    Na_o = parameters[42]
-    Cm = parameters[43]
-    F = parameters[44]
-    R = parameters[45]
-    T = parameters[46]
-    V_c = parameters[47]
-    K_o = parameters[52]
+    (
+        P_kna,
+        g_K1,
+        g_Kr,
+        g_Ks,
+        g_Na,
+        g_bna,
+        g_CaL,
+        g_bca,
+        g_to,
+        K_mNa,
+        K_mk,
+        P_NaK,
+        K_NaCa,
+        K_sat,
+        Km_Ca,
+        Km_Nai,
+        alpha,
+        gamma,
+        K_pCa,
+        g_pCa,
+        g_pK,
+        Buf_c,
+        Buf_sr,
+        Buf_ss,
+        Ca_o,
+        EC,
+        K_buf_c,
+        K_buf_sr,
+        K_buf_ss,
+        K_up,
+        V_leak,
+        V_rel,
+        V_sr,
+        V_ss,
+        V_xfer,
+        Vmax_up,
+        k1_prime,
+        k2_prime,
+        k3,
+        k4,
+        max_sr,
+        min_sr,
+        Na_o,
+        Cm,
+        F,
+        R,
+        T,
+        V_c,
+        stim_amplitude,
+        stim_duration,
+        stim_period,
+        stim_start,
+        K_o,
+    ) = parameters
 
     # Init return args
     if values is None:
         values = np.zeros((19,), dtype=np.float_)
     else:
         assert isinstance(values, np.ndarray) and values.shape == (19,)
 
@@ -727,70 +736,79 @@
     )
 
     # Expressions for the Calcium dynamics component
     i_up = Vmax_up / (1 + (K_up * K_up) / (Ca_i * Ca_i))
     i_leak = V_leak * (-Ca_i + Ca_SR)
     i_xfer = V_xfer * (-Ca_i + Ca_ss)
     kcasr = max_sr - (max_sr - min_sr) / (1 + (EC * EC) / (Ca_SR * Ca_SR))
-    Ca_i_bufc = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
-    Ca_sr_bufsr = 1.0 / (
+    ddt_Ca_i_total = (
+        V_sr * (-i_up + i_leak) / V_c
+        + Cm * (-i_b_Ca - i_p_Ca + 2 * i_NaCa) / (2 * F * V_c)
+        + i_xfer
+    )
+    f_JCa_i_free = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
+    f_JCa_sr_free = 1.0 / (
         1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR))
     )
-    Ca_ss_bufss = 1.0 / (
+    f_JCa_ss_free = 1.0 / (
         1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss))
     )
-    values[12] = (
-        V_sr * (-i_up + i_leak) / V_c
-        - Cm * (-2 * i_NaCa + i_b_Ca + i_p_Ca) / (2 * F * V_c)
-        + i_xfer
-    ) * Ca_i_bufc
+    values[12] = ddt_Ca_i_total * f_JCa_i_free
     k1 = k1_prime / kcasr
     k2 = k2_prime * kcasr
     O = (Ca_ss * Ca_ss) * R_prime * k1 / (k3 + (Ca_ss * Ca_ss) * k1)
     values[13] = k4 * (1 - R_prime) - Ca_ss * R_prime * k2
     i_rel = V_rel * (-Ca_ss + Ca_SR) * O
-    values[14] = (-i_leak - i_rel + i_up) * Ca_sr_bufsr
-    values[15] = (
+    ddt_Ca_sr_total = -i_leak - i_rel + i_up
+    ddt_Ca_ss_total = (
         V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
-    ) * Ca_ss_bufss
+    )
+    values[14] = ddt_Ca_sr_total * f_JCa_sr_free
+    values[15] = ddt_Ca_ss_total * f_JCa_ss_free
 
     # Expressions for the Sodium dynamics component
     values[16] = Cm * (-i_Na - i_b_Na - 3 * i_NaCa - 3 * i_NaK) / (F * V_c)
 
     # Expressions for the Membrane component
-    i_Stim = 0
+    i_Stim = np.where(
+        np.logical_and(
+            t - stim_period * np.floor(t / stim_period) >= stim_start,
+            t - stim_period * np.floor(t / stim_period) <= stim_duration + stim_start,
+        ),
+        stim_amplitude,
+        0,
+    )
     values[17] = (
-        -1.0 * i_Stim
-        - 1.0 * i_CaL
-        - 1.0 * i_K1
-        - 1.0 * i_Kr
-        - 1.0 * i_Ks
-        - 1.0 * i_Na
-        - 1.0 * i_NaCa
-        - 1.0 * i_NaK
-        - 1.0 * i_b_Ca
-        - 1.0 * i_b_Na
-        - 1.0 * i_p_Ca
-        - 1.0 * i_p_K
-        - 1.0 * i_to
+        -i_CaL
+        - i_K1
+        - i_Kr
+        - i_Ks
+        - i_Na
+        - i_NaCa
+        - i_NaK
+        - i_Stim
+        - i_b_Ca
+        - i_b_Na
+        - i_p_Ca
+        - i_p_K
+        - i_to
     )
 
     # Expressions for the Potassium dynamics component
     values[18] = (
-        Cm * (-i_Stim - i_K1 - i_Kr - i_Ks - i_p_K - i_to + 2 * i_NaK) / (F * V_c)
+        Cm * (-i_K1 - i_Kr - i_Ks - i_Stim - i_p_K - i_to + 2 * i_NaK) / (F * V_c)
     )
 
     # Return results
     return values
 
 
 def monitor(states, t, parameters, monitored=None):
     """
-    Computes monitored expressions of the tentusscher_panfilov_2006_epi_cell\
-        ODE
+    Computes monitored expressions of the tentusscher_panfilov_2006_M_cell ODE
     """
 
     # Assign states
     assert len(states) == 19
     (
         Xr1,
         Xr2,
@@ -811,69 +829,75 @@
         Na_i,
         V,
         K_i,
     ) = states
 
     # Assign parameters
     assert len(parameters) == 53
-    P_kna = parameters[0]
-    g_K1 = parameters[1]
-    g_Kr = parameters[2]
-    g_Ks = parameters[3]
-    g_Na = parameters[4]
-    g_bna = parameters[5]
-    g_CaL = parameters[6]
-    g_bca = parameters[7]
-    g_to = parameters[8]
-    K_mNa = parameters[9]
-    K_mk = parameters[10]
-    P_NaK = parameters[11]
-    K_NaCa = parameters[12]
-    K_sat = parameters[13]
-    Km_Ca = parameters[14]
-    Km_Nai = parameters[15]
-    alpha = parameters[16]
-    gamma = parameters[17]
-    K_pCa = parameters[18]
-    g_pCa = parameters[19]
-    g_pK = parameters[20]
-    Buf_c = parameters[21]
-    Buf_sr = parameters[22]
-    Buf_ss = parameters[23]
-    Ca_o = parameters[24]
-    EC = parameters[25]
-    K_buf_c = parameters[26]
-    K_buf_sr = parameters[27]
-    K_buf_ss = parameters[28]
-    K_up = parameters[29]
-    V_leak = parameters[30]
-    V_rel = parameters[31]
-    V_sr = parameters[32]
-    V_ss = parameters[33]
-    V_xfer = parameters[34]
-    Vmax_up = parameters[35]
-    k1_prime = parameters[36]
-    k2_prime = parameters[37]
-    k3 = parameters[38]
-    k4 = parameters[39]
-    max_sr = parameters[40]
-    min_sr = parameters[41]
-    Na_o = parameters[42]
-    Cm = parameters[43]
-    F = parameters[44]
-    R = parameters[45]
-    T = parameters[46]
-    V_c = parameters[47]
-    K_o = parameters[52]
+    (
+        P_kna,
+        g_K1,
+        g_Kr,
+        g_Ks,
+        g_Na,
+        g_bna,
+        g_CaL,
+        g_bca,
+        g_to,
+        K_mNa,
+        K_mk,
+        P_NaK,
+        K_NaCa,
+        K_sat,
+        Km_Ca,
+        Km_Nai,
+        alpha,
+        gamma,
+        K_pCa,
+        g_pCa,
+        g_pK,
+        Buf_c,
+        Buf_sr,
+        Buf_ss,
+        Ca_o,
+        EC,
+        K_buf_c,
+        K_buf_sr,
+        K_buf_ss,
+        K_up,
+        V_leak,
+        V_rel,
+        V_sr,
+        V_ss,
+        V_xfer,
+        Vmax_up,
+        k1_prime,
+        k2_prime,
+        k3,
+        k4,
+        max_sr,
+        min_sr,
+        Na_o,
+        Cm,
+        F,
+        R,
+        T,
+        V_c,
+        stim_amplitude,
+        stim_duration,
+        stim_period,
+        stim_start,
+        K_o,
+    ) = parameters
 
     # Init return args
     if monitored is None:
-        monitored = np.zeros((89,), dtype=np.float_)
+        monitored = np.zeros((92,), dtype=np.float_)
     else:
-        assert isinstance(monitored, np.ndarray) and monitored.shape == (89,)
+        assert isinstance(monitored, np.ndarray) and monitored.shape == (92,)
 
     # Expressions for the Reversal potentials component
     monitored[0] = R * T * np.log(Na_o / Na_i) / F
     monitored[1] = R * T * np.log(K_o / K_i) / F
     monitored[2] = R * T * np.log((K_o + Na_o * P_kna) / (P_kna * Na_i + K_i)) / F
     monitored[3] = 0.5 * R * T * np.log(Ca_o / Ca_i) / F
 
@@ -896,45 +920,45 @@
     )
 
     # Expressions for the Xr1 gate component
     monitored[9] = 1.0 / (1 + np.exp(-26 / 7 - V / 7))
     monitored[10] = 450 / (1 + np.exp(-9 / 2 - V / 10))
     monitored[11] = 6 / (1 + 13.581324522578193 * np.exp(0.08695652173913043 * V))
     monitored[12] = monitored[10] * monitored[11]
-    monitored[70] = (-Xr1 + monitored[9]) / monitored[12]
+    monitored[73] = (-Xr1 + monitored[9]) / monitored[12]
 
     # Expressions for the Xr2 gate component
     monitored[13] = 1.0 / (1 + np.exp(11 / 3 + V / 24))
     monitored[14] = 3 / (1 + np.exp(-3 - V / 20))
     monitored[15] = 1.12 / (1 + np.exp(-3 + V / 20))
     monitored[16] = monitored[14] * monitored[15]
-    monitored[71] = (-Xr2 + monitored[13]) / monitored[16]
+    monitored[74] = (-Xr2 + monitored[13]) / monitored[16]
 
     # Expressions for the Slow time dependent potassium current component
     monitored[17] = g_Ks * (Xs * Xs) * (-monitored[2] + V)
 
     # Expressions for the Xs gate component
     monitored[18] = 1.0 / (1 + np.exp(-5 / 14 - V / 14))
     monitored[19] = 1400 / np.sqrt(1 + np.exp(5 / 6 - V / 6))
     monitored[20] = 1.0 / (1 + np.exp(-7 / 3 + V / 15))
     monitored[21] = 80 + monitored[19] * monitored[20]
-    monitored[72] = (-Xs + monitored[18]) / monitored[21]
+    monitored[75] = (-Xs + monitored[18]) / monitored[21]
 
     # Expressions for the Fast sodium current component
     monitored[22] = g_Na * (m * m * m) * (-monitored[0] + V) * h * j
 
     # Expressions for the m gate component
     monitored[23] = 1.0 / (
         (1 + 0.0018422115811651339 * np.exp(-0.1107419712070875 * V))
         * (1 + 0.0018422115811651339 * np.exp(-0.1107419712070875 * V))
     )
     monitored[24] = 1.0 / (1 + np.exp(-12 - V / 5))
     monitored[25] = 0.1 / (1 + np.exp(7 + V / 5)) + 0.1 / (1 + np.exp(-1 / 4 + V / 200))
     monitored[26] = monitored[24] * monitored[25]
-    monitored[73] = (-m + monitored[23]) / monitored[26]
+    monitored[76] = (-m + monitored[23]) / monitored[26]
 
     # Expressions for the h gate component
     monitored[27] = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
     )
     monitored[28] = np.where(
@@ -942,15 +966,15 @@
     )
     monitored[29] = np.where(
         V < -40,
         310000 * np.exp(0.3485 * V) + 2.7 * np.exp(0.079 * V),
         0.77 / (0.13 + 0.049758141083938695 * np.exp(-0.0900900900900901 * V)),
     )
     monitored[30] = 1.0 / (monitored[28] + monitored[29])
-    monitored[74] = (-h + monitored[27]) / monitored[30]
+    monitored[77] = (-h + monitored[27]) / monitored[30]
 
     # Expressions for the j gate component
     monitored[31] = 1.0 / (
         (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
         * (1 + 15212.593285654404 * np.exp(0.13458950201884254 * V))
     )
     monitored[32] = np.where(
@@ -964,15 +988,15 @@
         V < -40,
         0.02424
         * np.exp(-0.01052 * V)
         / (1 + 0.003960868339904256 * np.exp(-0.1378 * V)),
         0.6 * np.exp(0.057 * V) / (1 + 0.040762203978366204 * np.exp(-0.1 * V)),
     )
     monitored[34] = 1.0 / (monitored[32] + monitored[33])
-    monitored[75] = (-j + monitored[31]) / monitored[34]
+    monitored[78] = (-j + monitored[31]) / monitored[34]
 
     # Expressions for the Sodium background current component
     monitored[35] = g_bna * (-monitored[0] + V)
 
     # Expressions for the L_type Ca current component
     monitored[36] = (
         4
@@ -989,57 +1013,57 @@
 
     # Expressions for the d gate component
     monitored[37] = 1.0 / (1 + 0.34415378686541237 * np.exp(-0.13333333333333333 * V))
     monitored[38] = 0.25 + 1.4 / (1 + np.exp(-35 / 13 - V / 13))
     monitored[39] = 1.4 / (1 + np.exp(1 + V / 5))
     monitored[40] = 1.0 / (1 + np.exp(5 / 2 - V / 20))
     monitored[41] = monitored[38] * monitored[39] + monitored[40]
-    monitored[76] = (-d + monitored[37]) / monitored[41]
+    monitored[79] = (-d + monitored[37]) / monitored[41]
 
     # Expressions for the f gate component
     monitored[42] = 1.0 / (1 + np.exp(20 / 7 + V / 7))
     monitored[43] = (
         20
         + 180 / (1 + np.exp(3 + V / 10))
         + 200 / (1 + np.exp(13 / 10 - V / 10))
         + 1102.5 * np.exp(-((27 + V) * (27 + V)) / 225)
     )
-    monitored[77] = (-f + monitored[42]) / monitored[43]
+    monitored[80] = (-f + monitored[42]) / monitored[43]
 
     # Expressions for the F2 gate component
     monitored[44] = 0.33 + 0.67 / (1 + np.exp(5 + V / 7))
     monitored[45] = (
         31 / (1 + np.exp(5 / 2 - V / 10))
         + 80 / (1 + np.exp(3 + V / 10))
         + 562 * np.exp(-((27 + V) * (27 + V)) / 240)
     )
-    monitored[78] = (-f2 + monitored[44]) / monitored[45]
+    monitored[81] = (-f2 + monitored[44]) / monitored[45]
 
     # Expressions for the FCass gate component
     monitored[46] = 0.4 + 0.6 / (1 + 400.0 * (Ca_ss * Ca_ss))
     monitored[47] = 2 + 80 / (1 + 400.0 * (Ca_ss * Ca_ss))
-    monitored[79] = (-fCass + monitored[46]) / monitored[47]
+    monitored[82] = (-fCass + monitored[46]) / monitored[47]
 
     # Expressions for the Calcium background current component
     monitored[48] = g_bca * (-monitored[3] + V)
 
     # Expressions for the Transient outward current component
     monitored[49] = g_to * (-monitored[1] + V) * r * s
 
     # Expressions for the s gate component
     monitored[50] = 1.0 / (1 + np.exp(4 + V / 5))
     monitored[51] = (
         3 + 5 / (1 + np.exp(-4 + V / 5)) + 85 * np.exp(-((45 + V) * (45 + V)) / 320)
     )
-    monitored[80] = (-s + monitored[50]) / monitored[51]
+    monitored[83] = (-s + monitored[50]) / monitored[51]
 
     # Expressions for the r gate component
     monitored[52] = 1.0 / (1 + np.exp(10 / 3 - V / 6))
     monitored[53] = 0.8 + 9.5 * np.exp(-((40 + V) * (40 + V)) / 1800)
-    monitored[81] = (-r + monitored[52]) / monitored[53]
+    monitored[84] = (-r + monitored[52]) / monitored[53]
 
     # Expressions for the Sodium potassium pump current component
     monitored[54] = (
         K_o
         * P_NaK
         * Na_i
         / (
@@ -1081,91 +1105,101 @@
     )
 
     # Expressions for the Calcium dynamics component
     monitored[58] = Vmax_up / (1 + (K_up * K_up) / (Ca_i * Ca_i))
     monitored[59] = V_leak * (-Ca_i + Ca_SR)
     monitored[60] = V_xfer * (-Ca_i + Ca_ss)
     monitored[61] = max_sr - (max_sr - min_sr) / (1 + (EC * EC) / (Ca_SR * Ca_SR))
-    monitored[62] = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
-    monitored[63] = 1.0 / (
-        1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR))
+    monitored[62] = (
+        V_sr * (-monitored[58] + monitored[59]) / V_c
+        + Cm * (-monitored[48] - monitored[56] + 2 * monitored[55]) / (2 * F * V_c)
+        + monitored[60]
     )
+    monitored[63] = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
     monitored[64] = 1.0 / (
+        1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR))
+    )
+    monitored[65] = 1.0 / (
         1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss))
     )
-    monitored[82] = (
-        V_sr * (-monitored[58] + monitored[59]) / V_c
-        - Cm * (-2 * monitored[55] + monitored[48] + monitored[56]) / (2 * F * V_c)
-        + monitored[60]
-    ) * monitored[62]
-    monitored[65] = k1_prime / monitored[61]
-    monitored[66] = k2_prime * monitored[61]
-    monitored[67] = (
+    monitored[85] = monitored[62] * monitored[63]
+    monitored[66] = k1_prime / monitored[61]
+    monitored[67] = k2_prime * monitored[61]
+    monitored[68] = (
         (Ca_ss * Ca_ss)
         * R_prime
-        * monitored[65]
-        / (k3 + (Ca_ss * Ca_ss) * monitored[65])
+        * monitored[66]
+        / (k3 + (Ca_ss * Ca_ss) * monitored[66])
     )
-    monitored[83] = k4 * (1 - R_prime) - Ca_ss * R_prime * monitored[66]
-    monitored[68] = V_rel * (-Ca_ss + Ca_SR) * monitored[67]
-    monitored[84] = (-monitored[59] - monitored[68] + monitored[58]) * monitored[63]
-    monitored[85] = (
-        V_sr * monitored[68] / V_ss
+    monitored[86] = k4 * (1 - R_prime) - Ca_ss * R_prime * monitored[67]
+    monitored[69] = V_rel * (-Ca_ss + Ca_SR) * monitored[68]
+    monitored[70] = -monitored[59] - monitored[69] + monitored[58]
+    monitored[71] = (
+        V_sr * monitored[69] / V_ss
         - V_c * monitored[60] / V_ss
         - Cm * monitored[36] / (2 * F * V_ss)
-    ) * monitored[64]
+    )
+    monitored[87] = monitored[64] * monitored[70]
+    monitored[88] = monitored[65] * monitored[71]
 
     # Expressions for the Sodium dynamics component
-    monitored[86] = (
+    monitored[89] = (
         Cm
         * (-monitored[22] - monitored[35] - 3 * monitored[54] - 3 * monitored[55])
         / (F * V_c)
     )
 
     # Expressions for the Membrane component
-    monitored[69] = 0
-    monitored[87] = (
-        -1.0 * monitored[69]
-        - 1.0 * monitored[17]
-        - 1.0 * monitored[22]
-        - 1.0 * monitored[35]
-        - 1.0 * monitored[36]
-        - 1.0 * monitored[48]
-        - 1.0 * monitored[49]
-        - 1.0 * monitored[54]
-        - 1.0 * monitored[55]
-        - 1.0 * monitored[56]
-        - 1.0 * monitored[57]
-        - 1.0 * monitored[7]
-        - 1.0 * monitored[8]
+    monitored[72] = np.where(
+        np.logical_and(
+            t - stim_period * np.floor(t / stim_period) >= stim_start,
+            t - stim_period * np.floor(t / stim_period) <= stim_duration + stim_start,
+        ),
+        stim_amplitude,
+        0,
+    )
+    monitored[90] = (
+        -monitored[17]
+        - monitored[22]
+        - monitored[35]
+        - monitored[36]
+        - monitored[48]
+        - monitored[49]
+        - monitored[54]
+        - monitored[55]
+        - monitored[56]
+        - monitored[57]
+        - monitored[72]
+        - monitored[7]
+        - monitored[8]
     )
 
     # Expressions for the Potassium dynamics component
-    monitored[88] = (
+    monitored[91] = (
         Cm
         * (
-            -monitored[69]
-            - monitored[17]
+            -monitored[17]
             - monitored[49]
             - monitored[57]
+            - monitored[72]
             - monitored[7]
             - monitored[8]
             + 2 * monitored[54]
         )
         / (F * V_c)
     )
 
     # Return results
     return monitored
 
 
 def forward_explicit_euler(states, t, dt, parameters):
     """
     Compute a forward step using the explicit Euler scheme to the\
-        tentusscher_panfilov_2006_epi_cell ODE
+        tentusscher_panfilov_2006_M_cell ODE
     """
 
     # Assign states
     assert len(states) == 19
     (
         Xr1,
         Xr2,
@@ -1186,63 +1220,69 @@
         Na_i,
         V,
         K_i,
     ) = states
 
     # Assign parameters
     assert len(parameters) == 53
-    P_kna = parameters[0]
-    g_K1 = parameters[1]
-    g_Kr = parameters[2]
-    g_Ks = parameters[3]
-    g_Na = parameters[4]
-    g_bna = parameters[5]
-    g_CaL = parameters[6]
-    g_bca = parameters[7]
-    g_to = parameters[8]
-    K_mNa = parameters[9]
-    K_mk = parameters[10]
-    P_NaK = parameters[11]
-    K_NaCa = parameters[12]
-    K_sat = parameters[13]
-    Km_Ca = parameters[14]
-    Km_Nai = parameters[15]
-    alpha = parameters[16]
-    gamma = parameters[17]
-    K_pCa = parameters[18]
-    g_pCa = parameters[19]
-    g_pK = parameters[20]
-    Buf_c = parameters[21]
-    Buf_sr = parameters[22]
-    Buf_ss = parameters[23]
-    Ca_o = parameters[24]
-    EC = parameters[25]
-    K_buf_c = parameters[26]
-    K_buf_sr = parameters[27]
-    K_buf_ss = parameters[28]
-    K_up = parameters[29]
-    V_leak = parameters[30]
-    V_rel = parameters[31]
-    V_sr = parameters[32]
-    V_ss = parameters[33]
-    V_xfer = parameters[34]
-    Vmax_up = parameters[35]
-    k1_prime = parameters[36]
-    k2_prime = parameters[37]
-    k3 = parameters[38]
-    k4 = parameters[39]
-    max_sr = parameters[40]
-    min_sr = parameters[41]
-    Na_o = parameters[42]
-    Cm = parameters[43]
-    F = parameters[44]
-    R = parameters[45]
-    T = parameters[46]
-    V_c = parameters[47]
-    K_o = parameters[52]
+    (
+        P_kna,
+        g_K1,
+        g_Kr,
+        g_Ks,
+        g_Na,
+        g_bna,
+        g_CaL,
+        g_bca,
+        g_to,
+        K_mNa,
+        K_mk,
+        P_NaK,
+        K_NaCa,
+        K_sat,
+        Km_Ca,
+        Km_Nai,
+        alpha,
+        gamma,
+        K_pCa,
+        g_pCa,
+        g_pK,
+        Buf_c,
+        Buf_sr,
+        Buf_ss,
+        Ca_o,
+        EC,
+        K_buf_c,
+        K_buf_sr,
+        K_buf_ss,
+        K_up,
+        V_leak,
+        V_rel,
+        V_sr,
+        V_ss,
+        V_xfer,
+        Vmax_up,
+        k1_prime,
+        k2_prime,
+        k3,
+        k4,
+        max_sr,
+        min_sr,
+        Na_o,
+        Cm,
+        F,
+        R,
+        T,
+        V_c,
+        stim_amplitude,
+        stim_duration,
+        stim_period,
+        stim_start,
+        K_o,
+    ) = parameters
 
     # Expressions for the Reversal potentials component
     E_Na = R * T * np.log(Na_o / Na_i) / F
     E_K = R * T * np.log(K_o / K_i) / F
     E_Ks = R * T * np.log((K_o + Na_o * P_kna) / (P_kna * Na_i + K_i)) / F
     E_Ca = 0.5 * R * T * np.log(Ca_o / Ca_i) / F
 
@@ -1452,89 +1492,89 @@
     )
 
     # Expressions for the Calcium dynamics component
     i_up = Vmax_up / (1 + (K_up * K_up) / (Ca_i * Ca_i))
     i_leak = V_leak * (-Ca_i + Ca_SR)
     i_xfer = V_xfer * (-Ca_i + Ca_ss)
     kcasr = max_sr - (max_sr - min_sr) / (1 + (EC * EC) / (Ca_SR * Ca_SR))
-    Ca_i_bufc = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
-    Ca_sr_bufsr = 1.0 / (
+    ddt_Ca_i_total = (
+        V_sr * (-i_up + i_leak) / V_c
+        + Cm * (-i_b_Ca - i_p_Ca + 2 * i_NaCa) / (2 * F * V_c)
+        + i_xfer
+    )
+    f_JCa_i_free = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
+    f_JCa_sr_free = 1.0 / (
         1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR))
     )
-    Ca_ss_bufss = 1.0 / (
+    f_JCa_ss_free = 1.0 / (
         1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss))
     )
-    dCa_i_dt = (
-        V_sr * (-i_up + i_leak) / V_c
-        - Cm * (-2 * i_NaCa + i_b_Ca + i_p_Ca) / (2 * F * V_c)
-        + i_xfer
-    ) * Ca_i_bufc
+    dCa_i_dt = ddt_Ca_i_total * f_JCa_i_free
     states[12] = dt * dCa_i_dt + Ca_i
     k1 = k1_prime / kcasr
     k2 = k2_prime * kcasr
     O = (Ca_ss * Ca_ss) * R_prime * k1 / (k3 + (Ca_ss * Ca_ss) * k1)
     dR_prime_dt = k4 * (1 - R_prime) - Ca_ss * R_prime * k2
     states[13] = dt * dR_prime_dt + R_prime
     i_rel = V_rel * (-Ca_ss + Ca_SR) * O
-    dCa_SR_dt = (-i_leak - i_rel + i_up) * Ca_sr_bufsr
-    states[14] = dt * dCa_SR_dt + Ca_SR
-    dCa_ss_dt = (
+    ddt_Ca_sr_total = -i_leak - i_rel + i_up
+    ddt_Ca_ss_total = (
         V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
-    ) * Ca_ss_bufss
+    )
+    dCa_SR_dt = ddt_Ca_sr_total * f_JCa_sr_free
+    states[14] = dt * dCa_SR_dt + Ca_SR
+    dCa_ss_dt = ddt_Ca_ss_total * f_JCa_ss_free
     states[15] = dt * dCa_ss_dt + Ca_ss
 
     # Expressions for the Sodium dynamics component
     dNa_i_dt = Cm * (-i_Na - i_b_Na - 3 * i_NaCa - 3 * i_NaK) / (F * V_c)
     states[16] = dt * dNa_i_dt + Na_i
 
     # Expressions for the Membrane component
-    i_Stim = 0
+    i_Stim = np.where(
+        np.logical_and(
+            t - stim_period * np.floor(t / stim_period) >= stim_start,
+            t - stim_period * np.floor(t / stim_period) <= stim_duration + stim_start,
+        ),
+        stim_amplitude,
+        0,
+    )
     dV_dt = (
-        -1.0 * i_Stim
-        - 1.0 * i_CaL
-        - 1.0 * i_K1
-        - 1.0 * i_Kr
-        - 1.0 * i_Ks
-        - 1.0 * i_Na
-        - 1.0 * i_NaCa
-        - 1.0 * i_NaK
-        - 1.0 * i_b_Ca
-        - 1.0 * i_b_Na
-        - 1.0 * i_p_Ca
-        - 1.0 * i_p_K
-        - 1.0 * i_to
+        -i_CaL
+        - i_K1
+        - i_Kr
+        - i_Ks
+        - i_Na
+        - i_NaCa
+        - i_NaK
+        - i_Stim
+        - i_b_Ca
+        - i_b_Na
+        - i_p_Ca
+        - i_p_K
+        - i_to
     )
     states[17] = dt * dV_dt + V
 
     # Expressions for the Potassium dynamics component
-    dK_i_dt = Cm * (-i_Stim - i_K1 - i_Kr - i_Ks - i_p_K - i_to + 2 * i_NaK) / (F * V_c)
+    dK_i_dt = Cm * (-i_K1 - i_Kr - i_Ks - i_Stim - i_p_K - i_to + 2 * i_NaK) / (F * V_c)
     states[18] = dt * dK_i_dt + K_i
 
     # Return results
     return states
 
 
-# import numba
-
-
-# @numba.njit(parallel=True)
-# def forward_generalized_rush_larsen(states, t, dt, parameters):
-#     for i in numba.prange(states.shape[1]):
-#         _forward_generalized_rush_larsen(states[:, i], t, dt, parameters)
-
-
-# @numba.njit
 def forward_generalized_rush_larsen(states, t, dt, parameters):
     """
     Compute a forward step using the generalised Rush-Larsen (GRL1) scheme to\
-        the tentusscher_panfilov_2006_epi_cell ODE
+        the tentusscher_panfilov_2006_M_cell ODE
     """
 
     # Assign states
-    # assert len(states) == 19
+    assert len(states) == 19
     (
         Xr1,
         Xr2,
         Xs,
         m,
         h,
         j,
@@ -1550,64 +1590,70 @@
         Ca_ss,
         Na_i,
         V,
         K_i,
     ) = states
 
     # Assign parameters
-    # assert len(parameters) == 53
-    P_kna = parameters[0]
-    g_K1 = parameters[1]
-    g_Kr = parameters[2]
-    g_Ks = parameters[3]
-    g_Na = parameters[4]
-    g_bna = parameters[5]
-    g_CaL = parameters[6]
-    g_bca = parameters[7]
-    g_to = parameters[8]
-    K_mNa = parameters[9]
-    K_mk = parameters[10]
-    P_NaK = parameters[11]
-    K_NaCa = parameters[12]
-    K_sat = parameters[13]
-    Km_Ca = parameters[14]
-    Km_Nai = parameters[15]
-    alpha = parameters[16]
-    gamma = parameters[17]
-    K_pCa = parameters[18]
-    g_pCa = parameters[19]
-    g_pK = parameters[20]
-    Buf_c = parameters[21]
-    Buf_sr = parameters[22]
-    Buf_ss = parameters[23]
-    Ca_o = parameters[24]
-    EC = parameters[25]
-    K_buf_c = parameters[26]
-    K_buf_sr = parameters[27]
-    K_buf_ss = parameters[28]
-    K_up = parameters[29]
-    V_leak = parameters[30]
-    V_rel = parameters[31]
-    V_sr = parameters[32]
-    V_ss = parameters[33]
-    V_xfer = parameters[34]
-    Vmax_up = parameters[35]
-    k1_prime = parameters[36]
-    k2_prime = parameters[37]
-    k3 = parameters[38]
-    k4 = parameters[39]
-    max_sr = parameters[40]
-    min_sr = parameters[41]
-    Na_o = parameters[42]
-    Cm = parameters[43]
-    F = parameters[44]
-    R = parameters[45]
-    T = parameters[46]
-    V_c = parameters[47]
-    K_o = parameters[52]
+    assert len(parameters) == 53
+    (
+        P_kna,
+        g_K1,
+        g_Kr,
+        g_Ks,
+        g_Na,
+        g_bna,
+        g_CaL,
+        g_bca,
+        g_to,
+        K_mNa,
+        K_mk,
+        P_NaK,
+        K_NaCa,
+        K_sat,
+        Km_Ca,
+        Km_Nai,
+        alpha,
+        gamma,
+        K_pCa,
+        g_pCa,
+        g_pK,
+        Buf_c,
+        Buf_sr,
+        Buf_ss,
+        Ca_o,
+        EC,
+        K_buf_c,
+        K_buf_sr,
+        K_buf_ss,
+        K_up,
+        V_leak,
+        V_rel,
+        V_sr,
+        V_ss,
+        V_xfer,
+        Vmax_up,
+        k1_prime,
+        k2_prime,
+        k3,
+        k4,
+        max_sr,
+        min_sr,
+        Na_o,
+        Cm,
+        F,
+        R,
+        T,
+        V_c,
+        stim_amplitude,
+        stim_duration,
+        stim_period,
+        stim_start,
+        K_o,
+    ) = parameters
 
     # Expressions for the Reversal potentials component
     E_Na = R * T * np.log(Na_o / Na_i) / F
     E_K = R * T * np.log(K_o / K_i) / F
     E_Ks = R * T * np.log((K_o + Na_o * P_kna) / (P_kna * Na_i + K_i)) / F
     E_Ca = 0.5 * R * T * np.log(Ca_o / Ca_i) / F
 
@@ -1835,39 +1881,45 @@
     )
 
     # Expressions for the Calcium dynamics component
     i_up = Vmax_up / (1 + (K_up * K_up) / (Ca_i * Ca_i))
     i_leak = V_leak * (-Ca_i + Ca_SR)
     i_xfer = V_xfer * (-Ca_i + Ca_ss)
     kcasr = max_sr - (max_sr - min_sr) / (1 + (EC * EC) / (Ca_SR * Ca_SR))
-    Ca_i_bufc = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
-    Ca_sr_bufsr = 1.0 / (
+    ddt_Ca_i_total = (
+        V_sr * (-i_up + i_leak) / V_c
+        + Cm * (-i_b_Ca - i_p_Ca + 2 * i_NaCa) / (2 * F * V_c)
+        + i_xfer
+    )
+    f_JCa_i_free = 1.0 / (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
+    f_JCa_sr_free = 1.0 / (
         1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR))
     )
-    Ca_ss_bufss = 1.0 / (
+    f_JCa_ss_free = 1.0 / (
         1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss))
     )
-    dCa_i_dt = (
-        V_sr * (-i_up + i_leak) / V_c
-        - Cm * (-2 * i_NaCa + i_b_Ca + i_p_Ca) / (2 * F * V_c)
-        + i_xfer
-    ) * Ca_i_bufc
-    dCa_i_bufc_dCa_i = (
+    dCa_i_dt = ddt_Ca_i_total * f_JCa_i_free
+    dE_Ca_dCa_i = -0.5 * R * T / (F * Ca_i)
+    dddt_Ca_i_total_di_NaCa = Cm / (F * V_c)
+    dddt_Ca_i_total_di_b_Ca = -Cm / (2 * F * V_c)
+    dddt_Ca_i_total_di_leak = V_sr / V_c
+    dddt_Ca_i_total_di_p_Ca = -Cm / (2 * F * V_c)
+    dddt_Ca_i_total_di_up = -V_sr / V_c
+    df_JCa_i_free_dCa_i = (
         2
         * Buf_c
         * K_buf_c
         / (
             (
                 (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
                 * (1 + Buf_c * K_buf_c / ((K_buf_c + Ca_i) * (K_buf_c + Ca_i)))
             )
             * ((K_buf_c + Ca_i) * (K_buf_c + Ca_i) * (K_buf_c + Ca_i))
         )
     )
-    dE_Ca_dCa_i = -0.5 * R * T / (F * Ca_i)
     di_NaCa_dCa_i = (
         -K_NaCa
         * alpha
         * (Na_o * Na_o * Na_o)
         * np.exp(F * (-1 + gamma) * V / (R * T))
         / (
             (1 + K_sat * np.exp(F * (-1 + gamma) * V / (R * T)))
@@ -1885,23 +1937,20 @@
         / (
             ((1 + (K_up * K_up) / (Ca_i * Ca_i)) * (1 + (K_up * K_up) / (Ca_i * Ca_i)))
             * (Ca_i * Ca_i * Ca_i)
         )
     )
     dCa_i_dt_linearized = (
         -V_xfer
-        + V_sr * (-V_leak - di_up_dCa_i) / V_c
-        - Cm
-        * (-2 * di_NaCa_dCa_i - g_bca * dE_Ca_dCa_i + di_p_Ca_dCa_i)
-        / (2 * F * V_c)
-    ) * Ca_i_bufc + (
-        V_sr * (-i_up + i_leak) / V_c
-        - Cm * (-2 * i_NaCa + i_b_Ca + i_p_Ca) / (2 * F * V_c)
-        + i_xfer
-    ) * dCa_i_bufc_dCa_i
+        + dddt_Ca_i_total_di_NaCa * di_NaCa_dCa_i
+        + dddt_Ca_i_total_di_p_Ca * di_p_Ca_dCa_i
+        + dddt_Ca_i_total_di_up * di_up_dCa_i
+        - V_leak * dddt_Ca_i_total_di_leak
+        - g_bca * dE_Ca_dCa_i * dddt_Ca_i_total_di_b_Ca
+    ) * f_JCa_i_free + ddt_Ca_i_total * df_JCa_i_free_dCa_i
     states[12] = Ca_i + np.where(
         np.abs(dCa_i_dt_linearized) > 1e-08,
         (-1 + np.exp(dt * dCa_i_dt_linearized)) * dCa_i_dt / dCa_i_dt_linearized,
         dt * dCa_i_dt,
     )
     k1 = k1_prime / kcasr
     k2 = k2_prime * kcasr
@@ -1915,30 +1964,34 @@
             * dR_prime_dt
             / dR_prime_dt_linearized,
             dt * dR_prime_dt,
         )
         + R_prime
     )
     i_rel = V_rel * (-Ca_ss + Ca_SR) * O
-    dCa_SR_dt = (-i_leak - i_rel + i_up) * Ca_sr_bufsr
-    dCa_sr_bufsr_dCa_SR = (
+    ddt_Ca_sr_total = -i_leak - i_rel + i_up
+    ddt_Ca_ss_total = (
+        V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
+    )
+    dCa_SR_dt = ddt_Ca_sr_total * f_JCa_sr_free
+    dO_dk1 = (Ca_ss * Ca_ss) * R_prime / (k3 + (Ca_ss * Ca_ss) * k1) - np.power(
+        Ca_ss, 4
+    ) * R_prime * k1 / ((k3 + (Ca_ss * Ca_ss) * k1) * (k3 + (Ca_ss * Ca_ss) * k1))
+    df_JCa_sr_free_dCa_SR = (
         2
         * Buf_sr
         * K_buf_sr
         / (
             (
                 (1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR)))
                 * (1 + Buf_sr * K_buf_sr / ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR)))
             )
             * ((K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR) * (K_buf_sr + Ca_SR))
         )
     )
-    dO_dk1 = (Ca_ss * Ca_ss) * R_prime / (k3 + (Ca_ss * Ca_ss) * k1) - np.power(
-        Ca_ss, 4
-    ) * R_prime * k1 / ((k3 + (Ca_ss * Ca_ss) * k1) * (k3 + (Ca_ss * Ca_ss) * k1))
     dk1_dkcasr = -k1_prime / (kcasr * kcasr)
     dkcasr_dCa_SR = (
         -2
         * (EC * EC)
         * (max_sr - min_sr)
         / (
             ((1 + (EC * EC) / (Ca_SR * Ca_SR)) * (1 + (EC * EC) / (Ca_SR * Ca_SR)))
@@ -1947,58 +2000,57 @@
     )
     di_rel_dCa_SR = (
         V_rel * O + V_rel * (-Ca_ss + Ca_SR) * dO_dk1 * dk1_dkcasr * dkcasr_dCa_SR
     )
     di_rel_dO = V_rel * (-Ca_ss + Ca_SR)
     dCa_SR_dt_linearized = (
         -V_leak - di_rel_dCa_SR - dO_dk1 * di_rel_dO * dk1_dkcasr * dkcasr_dCa_SR
-    ) * Ca_sr_bufsr + (-i_leak - i_rel + i_up) * dCa_sr_bufsr_dCa_SR
+    ) * f_JCa_sr_free + ddt_Ca_sr_total * df_JCa_sr_free_dCa_SR
     states[14] = Ca_SR + np.where(
         np.abs(dCa_SR_dt_linearized) > 1e-08,
         (-1 + np.exp(dt * dCa_SR_dt_linearized)) * dCa_SR_dt / dCa_SR_dt_linearized,
         dt * dCa_SR_dt,
     )
-    dCa_ss_dt = (
-        V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
-    ) * Ca_ss_bufss
-    dCa_ss_bufss_dCa_ss = (
+    dCa_ss_dt = ddt_Ca_ss_total * f_JCa_ss_free
+    dO_dCa_ss = -2 * (Ca_ss * Ca_ss * Ca_ss) * (k1 * k1) * R_prime / (
+        (k3 + (Ca_ss * Ca_ss) * k1) * (k3 + (Ca_ss * Ca_ss) * k1)
+    ) + 2 * Ca_ss * R_prime * k1 / (k3 + (Ca_ss * Ca_ss) * k1)
+    dddt_Ca_ss_total_di_CaL = -Cm / (2 * F * V_ss)
+    dddt_Ca_ss_total_di_rel = V_sr / V_ss
+    dddt_Ca_ss_total_di_xfer = -V_c / V_ss
+    df_JCa_ss_free_dCa_ss = (
         2
         * Buf_ss
         * K_buf_ss
         / (
             (
                 (1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss)))
                 * (1 + Buf_ss * K_buf_ss / ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss)))
             )
             * ((K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss) * (K_buf_ss + Ca_ss))
         )
     )
-    dO_dCa_ss = -2 * (Ca_ss * Ca_ss * Ca_ss) * (k1 * k1) * R_prime / (
-        (k3 + (Ca_ss * Ca_ss) * k1) * (k3 + (Ca_ss * Ca_ss) * k1)
-    ) + 2 * Ca_ss * R_prime * k1 / (k3 + (Ca_ss * Ca_ss) * k1)
     di_CaL_dCa_ss = (
         1.0
         * g_CaL
         * (F * F)
         * (-15 + V)
         * d
         * np.exp(F * (-30 + 2 * V) / (R * T))
         * f
         * f2
         * fCass
         / (R * T * (-1 + np.exp(F * (-30 + 2 * V) / (R * T))))
     )
     di_rel_dCa_ss = -V_rel * O + V_rel * (-Ca_ss + Ca_SR) * dO_dCa_ss
     dCa_ss_dt_linearized = (
-        V_sr * (dO_dCa_ss * di_rel_dO + di_rel_dCa_ss) / V_ss
-        - V_c * V_xfer / V_ss
-        - Cm * di_CaL_dCa_ss / (2 * F * V_ss)
-    ) * Ca_ss_bufss + (
-        V_sr * i_rel / V_ss - V_c * i_xfer / V_ss - Cm * i_CaL / (2 * F * V_ss)
-    ) * dCa_ss_bufss_dCa_ss
+        V_xfer * dddt_Ca_ss_total_di_xfer
+        + (dO_dCa_ss * di_rel_dO + di_rel_dCa_ss) * dddt_Ca_ss_total_di_rel
+        + dddt_Ca_ss_total_di_CaL * di_CaL_dCa_ss
+    ) * f_JCa_ss_free + ddt_Ca_ss_total * df_JCa_ss_free_dCa_ss
     states[15] = Ca_ss + np.where(
         np.abs(dCa_ss_dt_linearized) > 1e-08,
         (-1 + np.exp(dt * dCa_ss_dt_linearized)) * dCa_ss_dt / dCa_ss_dt_linearized,
         dt * dCa_ss_dt,
     )
 
     # Expressions for the Sodium dynamics component
@@ -2047,29 +2099,36 @@
     states[16] = Na_i + np.where(
         np.abs(dNa_i_dt_linearized) > 1e-08,
         (-1 + np.exp(dt * dNa_i_dt_linearized)) * dNa_i_dt / dNa_i_dt_linearized,
         dt * dNa_i_dt,
     )
 
     # Expressions for the Membrane component
-    i_Stim = 0
+    i_Stim = np.where(
+        np.logical_and(
+            t - stim_period * np.floor(t / stim_period) >= stim_start,
+            t - stim_period * np.floor(t / stim_period) <= stim_duration + stim_start,
+        ),
+        stim_amplitude,
+        0,
+    )
     dV_dt = (
-        -1.0 * i_Stim
-        - 1.0 * i_CaL
-        - 1.0 * i_K1
-        - 1.0 * i_Kr
-        - 1.0 * i_Ks
-        - 1.0 * i_Na
-        - 1.0 * i_NaCa
-        - 1.0 * i_NaK
-        - 1.0 * i_b_Ca
-        - 1.0 * i_b_Na
-        - 1.0 * i_p_Ca
-        - 1.0 * i_p_K
-        - 1.0 * i_to
+        -i_CaL
+        - i_K1
+        - i_Kr
+        - i_Ks
+        - i_Na
+        - i_NaCa
+        - i_NaK
+        - i_Stim
+        - i_b_Ca
+        - i_b_Na
+        - i_p_Ca
+        - i_p_K
+        - i_to
     )
     dalpha_K1_dV = (
         -3.686527411996926e-08
         * np.exp(0.06 * V - 0.06 * E_K)
         / (
             (1 + 6.14421235332821e-06 * np.exp(0.06 * V - 0.06 * E_K))
             * (1 + 6.14421235332821e-06 * np.exp(0.06 * V - 0.06 * E_K))
@@ -2203,40 +2262,39 @@
         1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V)
     ) + 10.937327047146876 * g_pK * (-E_K + V) * np.exp(-0.16722408026755853 * V) / (
         (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
         * (1 + 65.40521574193832 * np.exp(-0.16722408026755853 * V))
     )
     di_to_dV = g_to * r * s
     dV_dt_linearized = (
-        -1.0 * g_bca
-        - 1.0 * g_bna
-        - 1.0 * di_CaL_dV
-        - 1.0 * di_K1_dV
-        - 1.0 * di_Kr_dV
-        - 1.0 * di_Ks_dV
-        - 1.0 * di_NaCa_dV
-        - 1.0 * di_NaK_dV
-        - 1.0 * di_Na_dV
-        - 1.0 * di_p_K_dV
-        - 1.0 * di_to_dV
-        - 1.0
-        * (dalpha_K1_dV * dxK1_inf_dalpha_K1 + dbeta_K1_dV * dxK1_inf_dbeta_K1)
+        -g_bca
+        - g_bna
+        - di_CaL_dV
+        - di_K1_dV
+        - di_Kr_dV
+        - di_Ks_dV
+        - di_NaCa_dV
+        - di_NaK_dV
+        - di_Na_dV
+        - di_p_K_dV
+        - di_to_dV
+        - (dalpha_K1_dV * dxK1_inf_dalpha_K1 + dbeta_K1_dV * dxK1_inf_dbeta_K1)
         * di_K1_dxK1_inf
     )
     states[17] = (
         np.where(
             np.abs(dV_dt_linearized) > 1e-08,
             (-1 + np.exp(dt * dV_dt_linearized)) * dV_dt / dV_dt_linearized,
             dt * dV_dt,
         )
         + V
     )
 
     # Expressions for the Potassium dynamics component
-    dK_i_dt = Cm * (-i_Stim - i_K1 - i_Kr - i_Ks - i_p_K - i_to + 2 * i_NaK) / (F * V_c)
+    dK_i_dt = Cm * (-i_K1 - i_Kr - i_Ks - i_Stim - i_p_K - i_to + 2 * i_NaK) / (F * V_c)
     dE_K_dK_i = -R * T / (F * K_i)
     dE_Ks_dK_i = -R * T / (F * (P_kna * Na_i + K_i))
     dalpha_K1_dE_K = (
         3.686527411996926e-08
         * np.exp(0.06 * V - 0.06 * E_K)
         / (
             (1 + 6.14421235332821e-06 * np.exp(0.06 * V - 0.06 * E_K))
```

### Comparing `fenics-beat-0.0.2/src/beat/ecg.py` & `fenics-beat-0.0.3/src/beat/ecg.py`

 * *Files identical despite different names*

### Comparing `fenics-beat-0.0.2/src/beat/monodomain_model.py` & `fenics-beat-0.0.3/src/beat/monodomain_model.py`

 * *Files identical despite different names*

### Comparing `fenics-beat-0.0.2/src/beat/monodomain_solver.py` & `fenics-beat-0.0.3/src/beat/monodomain_solver.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,43 @@
 import logging
 import numpy as np
+from typing import Protocol
 from dataclasses import dataclass
 from .monodomain_model import MonodomainModel
-from .odesolver import DolfinODESolver
 
 logger = logging.getLogger(__name__)
 EPS = 1e-12
 
 
+class ODESolver(Protocol):
+    def to_dolfin(self) -> None:
+        ...
+
+    def from_dolfin(self) -> None:
+        ...
+
+    def ode_to_pde(self) -> None:
+        ...
+
+    def pde_to_ode(self) -> None:
+        ...
+
+    def step(self, t0: float, t1: float) -> None:
+        ...
+
+
 @dataclass
 class MonodomainSplittingSolver:
     pde: MonodomainModel
-    ode: DolfinODESolver
+    ode: ODESolver
     theta: float = 0.5
 
     def __post_init__(self) -> None:
-        self.ode.to_dolfin()
+        self.ode.to_dolfin()  # numpy array (ODE solver) -> dolfin function
+        self.ode.ode_to_pde()  # dolfin function in ODE space (quad?) -> CG1 dolfin function
         self.pde.assign_previous()
 
     def solve(self, interval, dt):
         (T0, T) = interval
         if dt is None:
             dt = T - T0
         t0 = T0
@@ -34,38 +52,45 @@
 
     def step(self, interval):
         # Extract some parameters for readability
         theta = self.theta
 
         # Extract time domain
         (t0, t1) = interval
+        logger.info(f"Stepping from {t0} to {t1} using theta = {theta}")
         dt = t1 - t0
         t = t0 + theta * dt
 
-        logger.info("Tentative ODE step")
+        logger.info(f"Tentative ODE step with t0={t0:.5f} dt={theta * dt:.5f}")
 
         # Solve ODE
-        self.ode.step(t0, theta * dt)
+        self.ode.step(t0=t0, dt=theta * dt)
         # Move voltage to FEniCS
-        self.ode.to_dolfin()
+        self.ode.to_dolfin()  # numpy array (ODE solver) -> dolfin function
+        self.ode.ode_to_pde()  # dolfin function in ODE space (quad?) -> CG1 dolfin function
+        self.pde.assign_previous()
 
         logger.info("PDE step")
         # Solve PDE
         self.pde.step((t0, t1))
 
+        self.ode.pde_to_ode()  # CG1 dolfin function -> dolfin function in ODE space (quad?)
         # Copy voltage from PDE to ODE
         self.ode.from_dolfin()
 
         # If first order splitting, we are done.
         if np.isclose(theta, 1.0):
             # But first update previous value in PDE
             self.pde.assign_previous()
             return
 
         # Otherwise, we do another ode_step:
-        logger.info("Corrective ODE step")
+        logger.info(
+            f"Corrective ODE step with t0={t:5f} and dt={(1.0 - theta) * dt:.5f}"
+        )
 
         # To the correction step
         self.ode.step(t, (1.0 - theta) * dt)
         # And copy the solution back to FEniCS
-        self.ode.to_dolfin()
+        self.ode.to_dolfin()  # numpy array (ODE solver) -> dolfin function
+        self.ode.ode_to_pde()  # dolfin function in ODE space (quad?) -> CG1 dolfin function
         self.pde.assign_previous()
```

### Comparing `fenics-beat-0.0.2/src/fenics_beat.egg-info/PKG-INFO` & `fenics-beat-0.0.3/src/fenics_beat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenics-beat
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library to run cardiac EP simulations
 Author-email: Henrik Finsberg <henriknf@simula.no>
 License: MIT
 Project-URL: Homepage, https://finsberg.github.io/fenics-beat
 Project-URL: Documentation, https://finsberg.github.io/fenics-beat
 Project-URL: Source, https://github.com/finsberg/fenics-beat
 Project-URL: Tracker, https://github.com/finsberg/fenics-beat/issues
@@ -23,14 +23,15 @@
 Requires-Dist: bump2version; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: pypi
 Requires-Dist: twine; extra == "pypi"
 Requires-Dist: build; extra == "pypi"
 Provides-Extra: demos
 Requires-Dist: cardiac-geometries; extra == "demos"
+Requires-Dist: ldrb; extra == "demos"
 Provides-Extra: docs
 Requires-Dist: jupyter-book; extra == "docs"
 Requires-Dist: jupytext; extra == "docs"
 Requires-Dist: fenics-beat[demos]; extra == "docs"
 Provides-Extra: all
 Requires-Dist: fenics-beat[test]; extra == "all"
 Requires-Dist: fenics-beat[docs]; extra == "all"
```

### Comparing `fenics-beat-0.0.2/src/fenics_beat.egg-info/SOURCES.txt` & `fenics-beat-0.0.3/src/fenics_beat.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -4,22 +4,31 @@
 src/beat/__init__.py
 src/beat/base_model.py
 src/beat/bidomain_model.py
 src/beat/ecg.py
 src/beat/monodomain_model.py
 src/beat/monodomain_solver.py
 src/beat/odesolver.py
+src/beat/utils.py
 src/beat/cellmodels/__init__.py
-src/beat/cellmodels/beeler_reuter.py
+src/beat/cellmodels/beeler_reuter_1977.py
 src/beat/cellmodels/fitzhughnagumo.py
-src/beat/cellmodels/tentusscher_panfilov_2006_M_cell.py
-src/beat/cellmodels/tentusscher_panfilov_2006_epi_cell.py
+src/beat/cellmodels/tentusscher_panfilov_2006/__init__.py
+src/beat/cellmodels/tentusscher_panfilov_2006/endo.py
+src/beat/cellmodels/tentusscher_panfilov_2006/epi.py
+src/beat/cellmodels/tentusscher_panfilov_2006/mid.py
+src/beat/cellmodels/torord_dyn_chloride/__init__.py
+src/beat/cellmodels/torord_dyn_chloride/endo.py
+src/beat/cellmodels/torord_dyn_chloride/epi.py
+src/beat/cellmodels/torord_dyn_chloride/mid.py
 src/fenics_beat.egg-info/PKG-INFO
 src/fenics_beat.egg-info/SOURCES.txt
 src/fenics_beat.egg-info/dependency_links.txt
 src/fenics_beat.egg-info/requires.txt
 src/fenics_beat.egg-info/top_level.txt
 tests/test_bidomain_model.py
+tests/test_cellmodels.py
 tests/test_ecg.py
 tests/test_monodomain.py
 tests/test_monodomain_solver.py
-tests/test_odesolver.py
+tests/test_odesolver.py
+tests/test_utils.py
```

### Comparing `fenics-beat-0.0.2/tests/test_bidomain_model.py` & `fenics-beat-0.0.3/tests/test_bidomain_model.py`

 * *Files identical despite different names*

### Comparing `fenics-beat-0.0.2/tests/test_ecg.py` & `fenics-beat-0.0.3/tests/test_ecg.py`

 * *Files identical despite different names*

### Comparing `fenics-beat-0.0.2/tests/test_monodomain.py` & `fenics-beat-0.0.3/tests/test_monodomain.py`

 * *Files identical despite different names*

### Comparing `fenics-beat-0.0.2/tests/test_monodomain_solver.py` & `fenics-beat-0.0.3/tests/test_monodomain_solver.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,19 +3,32 @@
 import pytest
 
 import beat
 
 
 def simple_ode_forward_euler(states, t, dt, parameters):
     v, s = states
-    states[0] = v - s * dt
-    states[1] = s + v * dt
-
-
-def test_monodomain_splitting_analytic():
+    values = np.zeros_like(states)
+    values[0] = v - s * dt
+    values[1] = s + v * dt
+    return values
+
+
+@pytest.mark.parametrize(
+    "odespace",
+    [
+        "CG_1",
+        "CG_2",
+        "DG_0",
+        "DG_1",
+        "Quadrature_2",
+        "Quadrature_4",
+    ],
+)
+def test_monodomain_splitting_analytic(odespace):
     # Exact solutions
     v_exact_str = "cos(2*pi*x[0])*cos(2*pi*x[1])*sin(t)"
     s_exact_str = "-cos(2*pi*x[0])*cos(2*pi*x[1])*cos(t)"
 
     # Source term
     ac_str = "8*pow(pi, 2)*cos(2*pi*x[0])*cos(2*pi*x[1])*sin(t)"
     s_exact = dolfin.Expression(s_exact_str, t=0, degree=1)
@@ -36,38 +49,58 @@
         "family": family,
         "degree": degree,
         "linear_solver_type": "direct",
     }
 
     pde = beat.MonodomainModel(time=time, mesh=mesh, M=M, I_s=I_s, params=params)
 
-    s = dolfin.interpolate(s_exact, pde.V)
+    family, degree = odespace.split("_")
+    element = dolfin.FiniteElement(
+        family, mesh.ufl_cell(), int(degree), quad_scheme="default"
+    )
+    V_ode = dolfin.FunctionSpace(mesh, element)
+    v_ode = dolfin.Function(V_ode)
+
+    s = dolfin.interpolate(s_exact, V_ode)
     s_arr = s.vector().get_local()
     init_states = np.zeros((2, s_arr.size))
     init_states[1, :] = s_arr
 
     ode = beat.odesolver.DolfinODESolver(
-        pde.state,
+        v_ode=v_ode,
+        v_pde=pde.state,
         fun=simple_ode_forward_euler,
         init_states=init_states,
         parameters=None,
         num_states=2,
         v_index=0,
     )
     solver = beat.MonodomainSplittingSolver(pde=pde, ode=ode)
     solver.solve((t0, T), dt=dt)
 
     v_exact = dolfin.Expression(v_exact_str, t=T, degree=3)
     v_error = dolfin.errornorm(v_exact, pde.state, "L2", degree_rise=2)
     # dolfin.File("v_exact.pvd") << dolfin.interpolate(v_exact, pde.V)
     # dolfin.File("v.pvd") << pde.state
+    print(v_error)
     assert v_error < 0.002
 
 
-def test_monodomain_splitting_spatial_convergence():
+@pytest.mark.parametrize(
+    "odespace",
+    [
+        "CG_1",
+        "CG_2",
+        "DG_0",
+        "DG_1",
+        "Quadrature_2",
+        "Quadrature_4",
+    ],
+)
+def test_monodomain_splitting_spatial_convergence(odespace):
     # Exact solutions
     v_exact_str = "cos(2*pi*x[0])*cos(2*pi*x[1])*sin(t)"
     s_exact_str = "-cos(2*pi*x[0])*cos(2*pi*x[1])*cos(t)"
 
     # Source term
     ac_str = "8*pow(pi, 2)*cos(2*pi*x[0])*cos(2*pi*x[1])*sin(t)"
 
@@ -84,48 +117,56 @@
     params = {
         "family": family,
         "degree": degree,
         "linear_solver_type": "direct",
     }
 
     errors = []
+    ode_family, ode_degree = odespace.split("_")
     Ns = [2**level for level in (3, 4, 5)]
     for N in Ns:
         mesh = dolfin.UnitSquareMesh(N, N)
         time = dolfin.Constant(0.0)
         I_s = dolfin.Expression(ac_str, t=time, degree=5)
 
         pde = beat.MonodomainModel(time=time, mesh=mesh, M=M, I_s=I_s, params=params)
         s_exact = dolfin.Expression(s_exact_str, t=0, degree=1)
-        s = dolfin.interpolate(s_exact, pde.V)
+
+        element = dolfin.FiniteElement(
+            ode_family, mesh.ufl_cell(), int(ode_degree), quad_scheme="default"
+        )
+        V_ode = dolfin.FunctionSpace(mesh, element)
+        v_ode = dolfin.Function(V_ode)
+
+        s = dolfin.interpolate(s_exact, V_ode)
         s_arr = s.vector().get_local()
         init_states = np.zeros((2, s_arr.size))
         init_states[1, :] = s_arr
 
         ode = beat.odesolver.DolfinODESolver(
-            pde.state,
+            v_ode=v_ode,
+            v_pde=pde.state,
             fun=simple_ode_forward_euler,
             init_states=init_states,
             num_states=2,
             parameters=None,
             v_index=0,
         )
         solver = beat.MonodomainSplittingSolver(pde=pde, ode=ode)
         solver.solve((t0, T), dt=dt)
 
         v_exact = dolfin.Expression(v_exact_str, t=T, degree=3)
         v_error = dolfin.errornorm(v_exact, pde.state, "L2", degree_rise=2)
         errors.append(v_error)
 
     rates = [np.log(e1 / e2) / np.log(2) for e1, e2 in zip(errors[:-1], errors[1:])]
-    # FIXME: This should be 2
-    assert all(rate >= 1.77 for rate in rates)
+    cvg_rate = sum(rates) / len(rates)
+    assert np.isclose(cvg_rate, degree + 1, rtol=0.1)
 
 
-@pytest.mark.xfail(reason="Don't know why this does not work")
 def test_monodomain_splitting_temporal_convergence():
     # Exact solutions
     v_exact_str = "cos(2*pi*x[0])*cos(2*pi*x[1])*sin(t)"
     s_exact_str = "-cos(2*pi*x[0])*cos(2*pi*x[1])*cos(t)"
 
     # Source term
     ac_str = "8*pow(pi, 2)*cos(2*pi*x[0])*cos(2*pi*x[1])*sin(t)"
@@ -144,37 +185,110 @@
         "family": family,
         "degree": degree,
         "linear_solver_type": "direct",
     }
 
     errors = []
     mesh = dolfin.UnitSquareMesh(150, 150)
-    dts = [1.0 / (2**level) for level in (0, 1, 2, 3)]
+    dts = [1.0 / (2**level) for level in (2, 3, 4)]
     for dt in dts:
         time = dolfin.Constant(0.0)
         I_s = dolfin.Expression(ac_str, t=time, degree=5)
 
         pde = beat.MonodomainModel(time=time, mesh=mesh, M=M, I_s=I_s, params=params)
         s_exact = dolfin.Expression(s_exact_str, t=0, degree=1)
         s = dolfin.interpolate(s_exact, pde.V)
         s_arr = s.vector().get_local()
         init_states = np.zeros((2, s_arr.size))
         init_states[1, :] = s_arr
 
         ode = beat.odesolver.DolfinODESolver(
-            pde.state,
+            v_ode=dolfin.Function(pde.V),
+            v_pde=pde.state,
             fun=simple_ode_forward_euler,
             init_states=init_states,
             num_states=2,
             parameters=None,
             v_index=0,
         )
         solver = beat.MonodomainSplittingSolver(pde=pde, ode=ode)
         solver.solve((t0, T), dt=dt)
 
         v_exact = dolfin.Expression(v_exact_str, t=T, degree=3)
         v_error = dolfin.errornorm(v_exact, pde.state, "L2", degree_rise=2)
         errors.append(v_error)
 
     rates = [np.log(e1 / e2) / np.log(2) for e1, e2 in zip(errors[:-1], errors[1:])]
+    cvg_rate = sum(rates) / len(rates)
+    # Forward Euler has error of order one in time
+    assert np.greater_equal(cvg_rate, 0.99)
+
+
+@pytest.mark.parametrize(
+    "odespace",
+    [
+        "CG_1",
+        "CG_2",
+        "DG_0",
+        "DG_1",
+        "Quadrature_2",
+        "Quadrature_4",
+    ],
+)
+def test_monodomain_splitting_analytic_multiODE(odespace):
+    # Exact solutions
+    v_exact_str = "cos(2*pi*x[0])*cos(2*pi*x[1])*sin(t)"
+    s_exact_str = "-cos(2*pi*x[0])*cos(2*pi*x[1])*cos(t)"
+
+    # Source term
+    ac_str = "8*pow(pi, 2)*cos(2*pi*x[0])*cos(2*pi*x[1])*sin(t)"
+    s_exact = dolfin.Expression(s_exact_str, t=0, degree=1)
+
+    family = "Lagrange"
+    degree = 1
+    N = 50
+    mesh = dolfin.UnitSquareMesh(N, N)
+    time = dolfin.Constant(0.0)
+    I_s = dolfin.Expression(ac_str, t=time, degree=5)
+    M = 1.0
+    # T = 4.0
+    dt = 0.01
+    T = dt
+    t0 = 0.0
+
+    params = {
+        "family": family,
+        "degree": degree,
+        "linear_solver_type": "direct",
+    }
+
+    pde = beat.MonodomainModel(time=time, mesh=mesh, M=M, I_s=I_s, params=params)
+
+    family, degree = odespace.split("_")
+    element = dolfin.FiniteElement(
+        family, mesh.ufl_cell(), int(degree), quad_scheme="default"
+    )
+    V_ode = dolfin.FunctionSpace(mesh, element)
+    v_ode = dolfin.Function(V_ode)
+
+    s = dolfin.interpolate(s_exact, V_ode)
+    s_arr = s.vector().get_local()
+    init_states = np.zeros((2, s_arr.size))
+    init_states[1, :] = s_arr
+
+    ode = beat.odesolver.DolfinODESolver(
+        v_ode=v_ode,
+        v_pde=pde.state,
+        fun=simple_ode_forward_euler,
+        init_states=init_states,
+        parameters=None,
+        num_states=2,
+        v_index=0,
+    )
+    solver = beat.MonodomainSplittingSolver(pde=pde, ode=ode)
+    solver.solve((t0, T), dt=dt)
 
-    assert all(rate >= 1.73 for rate in rates)
+    v_exact = dolfin.Expression(v_exact_str, t=T, degree=3)
+    v_error = dolfin.errornorm(v_exact, pde.state, "L2", degree_rise=2)
+    # dolfin.File("v_exact.pvd") << dolfin.interpolate(v_exact, pde.V)
+    # dolfin.File("v.pvd") << pde.state
+    assert v_error < 0.002
```

