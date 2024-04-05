# Comparing `tmp/janus_core-0.1.0b5.tar.gz` & `tmp/janus_core-0.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "janus_core-0.1.0b5.tar", max compression
+gzip compressed data, was "janus_core-0.2.0b0.tar", max compression
```

## Comparing `janus_core-0.1.0b5.tar` & `janus_core-0.2.0b0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1533 2024-03-26 17:33:53.343868 janus_core-0.1.0b5/LICENSE
--rw-r--r--   0        0        0     6606 2024-03-26 17:33:53.343868 janus_core-0.1.0b5/README.md
--rw-r--r--   0        0        0       80 2024-03-26 17:33:53.347868 janus_core-0.1.0b5/janus_core/__init__.py
--rw-r--r--   0        0        0    22384 2024-03-26 17:33:53.347868 janus_core-0.1.0b5/janus_core/cli.py
--rw-r--r--   0        0        0     4778 2024-03-26 17:33:53.347868 janus_core-0.1.0b5/janus_core/geom_opt.py
--rw-r--r--   0        0        0     1664 2024-03-26 17:33:53.347868 janus_core-0.1.0b5/janus_core/janus_types.py
--rw-r--r--   0        0        0     1627 2024-03-26 17:33:53.347868 janus_core-0.1.0b5/janus_core/log.py
--rw-r--r--   0        0        0    29081 2024-03-26 17:33:53.347868 janus_core-0.1.0b5/janus_core/md.py
--rw-r--r--   0        0        0     3518 2024-03-26 17:33:53.347868 janus_core-0.1.0b5/janus_core/mlip_calculators.py
--rw-r--r--   0        0        0    12111 2024-03-26 17:33:53.347868 janus_core-0.1.0b5/janus_core/single_point.py
--rw-r--r--   0        0        0      545 2024-03-26 17:33:53.347868 janus_core-0.1.0b5/janus_core/utils.py
--rw-r--r--   0        0        0     2510 2024-03-26 17:33:53.347868 janus_core-0.1.0b5/pyproject.toml
--rw-r--r--   0        0        0     7581 1970-01-01 00:00:00.000000 janus_core-0.1.0b5/PKG-INFO
+-rw-r--r--   0        0        0     1533 2024-04-05 07:46:42.906659 janus_core-0.2.0b0/LICENSE
+-rw-r--r--   0        0        0     6606 2024-04-05 07:46:42.906659 janus_core-0.2.0b0/README.md
+-rw-r--r--   0        0        0       80 2024-04-05 07:46:42.906659 janus_core-0.2.0b0/janus_core/__init__.py
+-rw-r--r--   0        0        0    22384 2024-04-05 07:46:42.906659 janus_core-0.2.0b0/janus_core/cli.py
+-rw-r--r--   0        0        0     4778 2024-04-05 07:46:42.906659 janus_core-0.2.0b0/janus_core/geom_opt.py
+-rw-r--r--   0        0        0     1664 2024-04-05 07:46:42.906659 janus_core-0.2.0b0/janus_core/janus_types.py
+-rw-r--r--   0        0        0     1627 2024-04-05 07:46:42.906659 janus_core-0.2.0b0/janus_core/log.py
+-rw-r--r--   0        0        0    29067 2024-04-05 07:46:42.906659 janus_core-0.2.0b0/janus_core/md.py
+-rw-r--r--   0        0        0     3514 2024-04-05 07:46:42.906659 janus_core-0.2.0b0/janus_core/mlip_calculators.py
+-rw-r--r--   0        0        0    12111 2024-04-05 07:46:42.906659 janus_core-0.2.0b0/janus_core/single_point.py
+-rw-r--r--   0        0        0     3293 2024-04-05 07:46:42.906659 janus_core-0.2.0b0/janus_core/stats.py
+-rw-r--r--   0        0        0      545 2024-04-05 07:46:42.906659 janus_core-0.2.0b0/janus_core/utils.py
+-rw-r--r--   0        0        0     2510 2024-04-05 07:46:42.906659 janus_core-0.2.0b0/pyproject.toml
+-rw-r--r--   0        0        0     7581 1970-01-01 00:00:00.000000 janus_core-0.2.0b0/PKG-INFO
```

### Comparing `janus_core-0.1.0b5/LICENSE` & `janus_core-0.2.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `janus_core-0.1.0b5/README.md` & `janus_core-0.2.0b0/README.md`

 * *Files identical despite different names*

### Comparing `janus_core-0.1.0b5/janus_core/cli.py` & `janus_core-0.2.0b0/janus_core/cli.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.1.0b5/janus_core/geom_opt.py` & `janus_core-0.2.0b0/janus_core/geom_opt.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.1.0b5/janus_core/janus_types.py` & `janus_core-0.2.0b0/janus_core/janus_types.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.1.0b5/janus_core/log.py` & `janus_core-0.2.0b0/janus_core/log.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.1.0b5/janus_core/md.py` & `janus_core-0.2.0b0/janus_core/md.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,18 +340,17 @@
 
         Returns
         -------
         str
             Header for molecular dynamics log.
         """
         log_header = (
-            "Step | real time[s] | Time [fs] | Epot/N [eV] | Ekin/N [eV] | "
-            "c_T [eV/K] | Etot/N [eV] | Density [g/cm^3] | Volume [A^3] | "
-            "Pressure [bar] | Pxx [bar] | Pyy [bar] | Pzz[bar] | Pyz[bar] | "
-            "Pxz[bar] | Pxy[bar]"
+            "Step | Real Time [s] | Time [fs] | Epot/N [eV] | Ekin/N [eV] | "
+            "T [K] | Etot/N [eV] | Density [g/cm^3] | Volume [A^3] | P [bar] | "
+            "Pxx [bar] | Pyy [bar] | Pzz [bar] | Pyz [bar] | Pxz [bar] | Pxy [bar]"
         )
 
         return log_header
 
     def get_log_stats(self) -> str:
         """
         Get thermodynamical statistics to be written to molecular dynamics log.
@@ -359,15 +358,15 @@
         Returns
         -------
         str
             Thermodynamical statistics to be written out.
         """
         e_pot = self.dyn.atoms.get_potential_energy() / self.n_atoms
         e_kin = self.dyn.atoms.get_kinetic_energy() / self.n_atoms
-        c_T = e_kin / (1.5 * units.kB)  # pylint: disable=invalid-name
+        current_temp = e_kin / (1.5 * units.kB)
 
         time = self.offset * self.timestep + self.dyn.get_time() / units.fs
         step = self.offset + self.dyn.nsteps
         self.dyn.atoms.info["time_fs"] = time
         self.dyn.atoms.info["step"] = step
 
         time_now = clock.datetime.now()
@@ -397,15 +396,15 @@
             volume = 0.0
             pressure = 0.0
             density = 0.0
             pressure_tensor = np.zeros(6)
 
         log_stats = (
             f"{step:10d} {real_time.total_seconds():.3f} {time:13.2f} {e_pot:.3e} "
-            f"{e_kin:.3e} {c_T:.3f} {e_pot + e_kin:.3e} {density:.3f} "
+            f"{e_kin:.3e} {current_temp:.3f} {e_pot + e_kin:.3e} {density:.3f} "
             f"{volume:.3e} {pressure:.3e} {pressure_tensor[0]:.3e} "
             f"{pressure_tensor[1]:.3e} {pressure_tensor[2]:.3e} "
             f"{pressure_tensor[3]:.3e} {pressure_tensor[4]:.3e} "
             f"{pressure_tensor[5]:.3e}"
         )
 
         return log_stats
@@ -607,15 +606,15 @@
 
         Returns
         -------
         str
             Header for molecular dynamics log.
         """
         log_header = MolecularDynamics.get_log_header()
-        return log_header + " | Pressure[bar] | T [K]"
+        return log_header + " | Target P [bar] | Target T [K]"
 
 
 class NVT(MolecularDynamics):
     """
     Configure NVT simulation.
 
     Parameters
@@ -685,15 +684,15 @@
 
         Returns
         -------
         str
             Header for molecular dynamics log.
         """
         log_header = MolecularDynamics.get_log_header()
-        return log_header + " | T [K]"
+        return log_header + " | Target T [K]"
 
 
 class NVE(MolecularDynamics):
     """
     Configure NVE simulation.
 
     Parameters
@@ -796,15 +795,15 @@
 
         Returns
         -------
         str
             Header for molecular dynamics log.
         """
         log_header = MolecularDynamics.get_log_header()
-        return log_header + " | T [K]"
+        return log_header + " | Target T [K]"
 
 
 class NPH(NPT):
     """
     Configure NPH simulation.
 
     Parameters
```

### Comparing `janus_core-0.1.0b5/janus_core/mlip_calculators.py` & `janus_core-0.2.0b0/janus_core/mlip_calculators.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,17 +47,17 @@
         raise ValueError("Please specify either `model` or `model_paths`")
 
     if architecture == "mace":
         from mace import __version__
         from mace.calculators import MACECalculator
 
         # `model_paths` is keyword for path to model, so take from kwargs if specified
-        # Otherwise, take `model` if specified, then default to `None`, which will
+        # Otherwise, take `model` if specified, then default to `""`, which will
         # raise a ValueError
-        kwargs.setdefault("model_paths", kwargs.pop("model", None))
+        kwargs.setdefault("model_paths", kwargs.pop("model", ""))
         kwargs.setdefault("default_dtype", "float64")
         calculator = MACECalculator(device=device, **kwargs)
 
     elif architecture == "mace_mp":
         from mace import __version__
         from mace.calculators import mace_mp
```

### Comparing `janus_core-0.1.0b5/janus_core/single_point.py` & `janus_core-0.2.0b0/janus_core/single_point.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.1.0b5/janus_core/utils.py` & `janus_core-0.2.0b0/janus_core/utils.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.1.0b5/pyproject.toml` & `janus_core-0.2.0b0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "janus-core"
-version = "0.1.0b5"
+version = "0.2.0b0"
 description = "Tools for machine learnt interatomic potentials"
 authors = [
     "Elliott Kasoar",
     "Federica Zanca",
     "Patrick Austin",
     "David Mason",
     "Jacob Wilkins",
```

### Comparing `janus_core-0.1.0b5/PKG-INFO` & `janus_core-0.2.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janus-core
-Version: 0.1.0b5
+Version: 0.2.0b0
 Summary: Tools for machine learnt interatomic potentials
 Home-page: https://github.com/stfc/janus-core/
 Author: Elliott Kasoar
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

