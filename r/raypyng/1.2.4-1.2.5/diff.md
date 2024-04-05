# Comparing `tmp/raypyng-1.2.4.tar.gz` & `tmp/raypyng-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raypyng-1.2.4.tar", last modified: Tue Mar 12 09:13:30 2024, max compression
+gzip compressed data, was "raypyng-1.2.5.tar", last modified: Fri Apr  5 06:43:04 2024, max compression
```

## Comparing `raypyng-1.2.4.tar` & `raypyng-1.2.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-03-12 09:13:30.287234 raypyng-1.2.4/
--rwxrwxr-x   0 simone    (1000) simone    (1000)     1107 2024-01-13 15:27:58.000000 raypyng-1.2.4/LICENSE
--rw-r--r--   0 simone    (1000) simone    (1000)     2310 2024-03-12 09:13:30.287234 raypyng-1.2.4/PKG-INFO
--rwxrwxr-x   0 simone    (1000) simone    (1000)      306 2024-01-13 15:27:58.000000 raypyng-1.2.4/README.md
--rwxrwxr-x   0 simone    (1000) simone    (1000)      747 2024-03-12 09:12:49.000000 raypyng-1.2.4/pyproject.toml
--rw-rw-r--   0 simone    (1000) simone    (1000)       38 2024-03-12 09:13:30.287234 raypyng-1.2.4/setup.cfg
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-03-12 09:13:30.287234 raypyng-1.2.4/src/
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-03-12 09:13:30.287234 raypyng-1.2.4/src/raypyng/
--rwxrwxr-x   0 simone    (1000) simone    (1000)       74 2024-01-13 15:28:00.000000 raypyng-1.2.4/src/raypyng/__init__.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)    12577 2024-03-04 22:36:05.000000 raypyng-1.2.4/src/raypyng/beamwaist.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)     8687 2024-01-13 15:28:00.000000 raypyng-1.2.4/src/raypyng/collections.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)      212 2024-01-13 15:28:00.000000 raypyng-1.2.4/src/raypyng/config.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)      126 2024-01-13 15:28:00.000000 raypyng-1.2.4/src/raypyng/errors.py
--rw-rw-r--   0 simone    (1000) simone    (1000)    17231 2024-03-07 14:35:51.000000 raypyng-1.2.4/src/raypyng/postprocessing.py
--rw-rw-r--   0 simone    (1000) simone    (1000)    12242 2024-03-06 08:13:34.000000 raypyng-1.2.4/src/raypyng/recipes.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)     4420 2024-01-13 15:28:00.000000 raypyng-1.2.4/src/raypyng/rml.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)    11767 2024-01-13 15:28:00.000000 raypyng-1.2.4/src/raypyng/runner.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)    43216 2024-03-12 09:12:35.000000 raypyng-1.2.4/src/raypyng/simulate.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)     6206 2024-01-13 15:28:00.000000 raypyng-1.2.4/src/raypyng/wave_helper.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-03-12 09:13:30.287234 raypyng-1.2.4/src/raypyng/xmltools/
--rwxrwxr-x   0 simone    (1000) simone    (1000)     1694 2024-01-13 15:28:00.000000 raypyng-1.2.4/src/raypyng/xmltools/__init__.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)     1518 2024-01-13 15:28:00.000000 raypyng-1.2.4/src/raypyng/xmltools/attributes.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)     1088 2024-01-13 15:28:00.000000 raypyng-1.2.4/src/raypyng/xmltools/dictionaries.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)     6942 2024-01-13 15:28:00.000000 raypyng-1.2.4/src/raypyng/xmltools/elements.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)     2782 2024-01-13 15:28:00.000000 raypyng-1.2.4/src/raypyng/xmltools/parser.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-03-12 09:13:30.287234 raypyng-1.2.4/src/raypyng.egg-info/
--rw-r--r--   0 simone    (1000) simone    (1000)     2310 2024-03-12 09:13:30.000000 raypyng-1.2.4/src/raypyng.egg-info/PKG-INFO
--rw-rw-r--   0 simone    (1000) simone    (1000)      743 2024-03-12 09:13:30.000000 raypyng-1.2.4/src/raypyng.egg-info/SOURCES.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)        1 2024-03-12 09:13:30.000000 raypyng-1.2.4/src/raypyng.egg-info/dependency_links.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)       75 2024-03-12 09:13:30.000000 raypyng-1.2.4/src/raypyng.egg-info/requires.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)        8 2024-03-12 09:13:30.000000 raypyng-1.2.4/src/raypyng.egg-info/top_level.txt
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-03-12 09:13:30.287234 raypyng-1.2.4/tests/
--rw-rw-r--   0 simone    (1000) simone    (1000)     3999 2024-01-13 15:28:03.000000 raypyng-1.2.4/tests/test_analyze.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     4879 2024-01-13 15:28:03.000000 raypyng-1.2.4/tests/test_no_analyze.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1181 2024-01-13 15:28:03.000000 raypyng-1.2.4/tests/test_simulation_class.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      497 2024-01-13 15:28:03.000000 raypyng-1.2.4/tests/test_waveHelper.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-05 06:43:04.006887 raypyng-1.2.5/
+-rwxrwxr-x   0 simone    (1000) simone    (1000)     1107 2024-01-13 15:27:58.000000 raypyng-1.2.5/LICENSE
+-rw-r--r--   0 simone    (1000) simone    (1000)     2348 2024-04-05 06:43:04.006887 raypyng-1.2.5/PKG-INFO
+-rwxrwxr-x   0 simone    (1000) simone    (1000)      306 2024-01-13 15:27:58.000000 raypyng-1.2.5/README.md
+-rwxrwxr-x   0 simone    (1000) simone    (1000)      786 2024-04-05 06:41:21.000000 raypyng-1.2.5/pyproject.toml
+-rw-rw-r--   0 simone    (1000) simone    (1000)       38 2024-04-05 06:43:04.006887 raypyng-1.2.5/setup.cfg
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-05 06:43:04.006887 raypyng-1.2.5/src/
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-05 06:43:04.006887 raypyng-1.2.5/src/raypyng/
+-rwxrwxr-x   0 simone    (1000) simone    (1000)       74 2024-01-13 15:28:00.000000 raypyng-1.2.5/src/raypyng/__init__.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)    12577 2024-03-04 22:36:05.000000 raypyng-1.2.5/src/raypyng/beamwaist.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)     8687 2024-01-13 15:28:00.000000 raypyng-1.2.5/src/raypyng/collections.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)      212 2024-01-13 15:28:00.000000 raypyng-1.2.5/src/raypyng/config.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)      126 2024-01-13 15:28:00.000000 raypyng-1.2.5/src/raypyng/errors.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    17231 2024-03-07 14:35:51.000000 raypyng-1.2.5/src/raypyng/postprocessing.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    12242 2024-03-06 08:13:34.000000 raypyng-1.2.5/src/raypyng/recipes.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)     4420 2024-01-13 15:28:00.000000 raypyng-1.2.5/src/raypyng/rml.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)    11767 2024-01-13 15:28:00.000000 raypyng-1.2.5/src/raypyng/runner.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)    48757 2024-04-05 06:37:24.000000 raypyng-1.2.5/src/raypyng/simulate.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)     6206 2024-01-13 15:28:00.000000 raypyng-1.2.5/src/raypyng/wave_helper.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-05 06:43:04.006887 raypyng-1.2.5/src/raypyng/xmltools/
+-rwxrwxr-x   0 simone    (1000) simone    (1000)     1694 2024-01-13 15:28:00.000000 raypyng-1.2.5/src/raypyng/xmltools/__init__.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)     1518 2024-01-13 15:28:00.000000 raypyng-1.2.5/src/raypyng/xmltools/attributes.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)     1088 2024-01-13 15:28:00.000000 raypyng-1.2.5/src/raypyng/xmltools/dictionaries.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)     6942 2024-01-13 15:28:00.000000 raypyng-1.2.5/src/raypyng/xmltools/elements.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)     2782 2024-01-13 15:28:00.000000 raypyng-1.2.5/src/raypyng/xmltools/parser.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-05 06:43:04.006887 raypyng-1.2.5/src/raypyng.egg-info/
+-rw-r--r--   0 simone    (1000) simone    (1000)     2348 2024-04-05 06:43:04.000000 raypyng-1.2.5/src/raypyng.egg-info/PKG-INFO
+-rw-rw-r--   0 simone    (1000) simone    (1000)      743 2024-04-05 06:43:04.000000 raypyng-1.2.5/src/raypyng.egg-info/SOURCES.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)        1 2024-04-05 06:43:04.000000 raypyng-1.2.5/src/raypyng.egg-info/dependency_links.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)       80 2024-04-05 06:43:04.000000 raypyng-1.2.5/src/raypyng.egg-info/requires.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)        8 2024-04-05 06:43:04.000000 raypyng-1.2.5/src/raypyng.egg-info/top_level.txt
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-05 06:43:04.006887 raypyng-1.2.5/tests/
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3999 2024-01-13 15:28:03.000000 raypyng-1.2.5/tests/test_analyze.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     4879 2024-01-13 15:28:03.000000 raypyng-1.2.5/tests/test_no_analyze.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1181 2024-01-13 15:28:03.000000 raypyng-1.2.5/tests/test_simulation_class.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      497 2024-01-13 15:28:03.000000 raypyng-1.2.5/tests/test_waveHelper.py
```

### Comparing `raypyng-1.2.4/LICENSE` & `raypyng-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `raypyng-1.2.4/PKG-INFO` & `raypyng-1.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: raypyng
-Version: 1.2.4
+Version: 1.2.5
 Summary: Python interface for RAY-UI x-ray tracing program
-Author-email: "Simone Vadilonga, Ruslan Ovsyannikov" <simone.vadilonga@helmholtz-berlin.de>
+Author-email: "Simone Vadilonga, Ruslan Ovsyannikov, Sebastian Sachse" <simone.vadilonga@helmholtz-berlin.de>
 License: The MIT License (MIT)
         
         Copyright (c) <2022> <Simone Vadilonga, Ruslan Ovsyannikov>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -34,14 +34,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.22.0
 Requires-Dist: psutil>=5.9.1
 Requires-Dist: joblib>=1.1.0
 Requires-Dist: matplotlib>=3.5.1
 Requires-Dist: natsort>=8.2.0
+Requires-Dist: tqdm
 
 ## Project Description
 raypyng provides a simple API to work with RAY-UI, a software for optical simulation of synchrotron beamlines and x-ray systems developed by Helmholtz-Zentrum Berlin.
 
 raypyng works only under linux distributions.
 
 [Documentation](https://raypyng.readthedocs.io/en/latest/index.html)
```

### Comparing `raypyng-1.2.4/pyproject.toml` & `raypyng-1.2.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "raypyng"
-version = "1.2.4"
+version = "1.2.5"
 
 authors = [
-  { name="Simone Vadilonga, Ruslan Ovsyannikov", email="simone.vadilonga@helmholtz-berlin.de" },
+  { name="Simone Vadilonga, Ruslan Ovsyannikov, Sebastian Sachse", email="simone.vadilonga@helmholtz-berlin.de" },
 ]
 description = "Python interface for RAY-UI x-ray tracing program"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -15,14 +15,15 @@
 ]
 
 dependencies = [
             'numpy>=1.22.0',
             'psutil>=5.9.1',
             'joblib>=1.1.0',
             'matplotlib>=3.5.1',
-            'natsort>=8.2.0 '
+            'natsort>=8.2.0 ', 
+            'tqdm'
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/hz-b/raypyng/"
 "Bug Tracker" = "https://github.com/hz-b/raypyng/issues"
 "Documentation" = "https://raypyng.readthedocs.io"
```

### Comparing `raypyng-1.2.4/src/raypyng/beamwaist.py` & `raypyng-1.2.5/src/raypyng/beamwaist.py`

 * *Files identical despite different names*

### Comparing `raypyng-1.2.4/src/raypyng/collections.py` & `raypyng-1.2.5/src/raypyng/collections.py`

 * *Files identical despite different names*

### Comparing `raypyng-1.2.4/src/raypyng/postprocessing.py` & `raypyng-1.2.5/src/raypyng/postprocessing.py`

 * *Files identical despite different names*

### Comparing `raypyng-1.2.4/src/raypyng/recipes.py` & `raypyng-1.2.5/src/raypyng/recipes.py`

 * *Files identical despite different names*

### Comparing `raypyng-1.2.4/src/raypyng/rml.py` & `raypyng-1.2.5/src/raypyng/rml.py`

 * *Files identical despite different names*

### Comparing `raypyng-1.2.4/src/raypyng/runner.py` & `raypyng-1.2.5/src/raypyng/runner.py`

 * *Files identical despite different names*

### Comparing `raypyng-1.2.4/src/raypyng/simulate.py` & `raypyng-1.2.5/src/raypyng/simulate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import itertools
 import os 
+import sys
+import re
 import numpy as np
 from tqdm import tqdm
 import time
 import csv
 from concurrent.futures import ProcessPoolExecutor, as_completed
+import logging
 
 from .rml import RMLFile
 from .rml import ObjectElement,ParamElement, BeamlineElement
 from .runner import RayUIAPI,RayUIRunner
 from .recipes import SimulationRecipe
 from .postprocessing import PostProcess
 
@@ -284,25 +287,28 @@
                 self._rml = rml
             else: # assume that parameter is the file name as required for RMLFile
                 self._rml = RMLFile(None,template=rml)
         else:
             raise Exception("rml file must be defined")
         
 
+        
         self._rml = rml if isinstance(rml, RMLFile) else RMLFile(None, template=rml) if rml else None
         self.path = None  # Path for simulation execution
         self.prefix = 'RAYPy_Simulation'  # Simulation prefix
         self._hide = hide  # Hide GUI leftovers
         self.analyze = True  # Enable RAY-UI analysis
         self._repeat = 1  # Number of simulation repeats
         self.raypyng_analysis = False  # Enable RAYPyNG analysis
         self.ray_path = ray_path  # RAY-UI installation path
         self.overwrite_rml = True  # Overwrite RML files
         self._sim_folder = None  # Simulation folder name
-        self.batch_size = 1000
+        self.batch_size = 50#1e6
+        self._simulation_timeout = 60
+        self._batch_number = None
         
         self._simulation_name = None  # Custom simulation name
         self._exports = []  # Files to export after simulation
         self._exports_list = []  # Processed list of exports
         self._exported_obj_names_list = [] # List containing the names of the objects to export
         self.sp = None  # SimulationParams instance
         self.sim_list_path = []  # Paths to RML files
@@ -762,17 +768,17 @@
         minutes, seconds = divmod(int(seconds), 60)
         if days > 0:
             return f"{days} day(s), {int(hours):02d}h:{int(minutes):02d}min"
         else:
             return f"{int(hours):02d}h:{int(minutes):02d}min"
 
     
-    def _initialize_progress_bar(self, total_simulations):
+    def _initialize_progress_bar(self, total_simulations, description="Simulations Completed"):
         bar_format = '{desc}: {percentage:3.0f}%|{bar}| {n_fmt}/{total_fmt} {postfix}]'
-        progress_bar = tqdm(total=total_simulations, bar_format=bar_format, desc="Simulations Completed")
+        progress_bar = tqdm(total=total_simulations, bar_format=bar_format, desc=description)
         return progress_bar
     
     def _print_simulations_info(self):
         total_simulations = self.sp._calc_number_sim() * self.repeat
         
         # Prepare data for printing
         data = [
@@ -794,15 +800,22 @@
         print("-" * (sum(col_widths) + 3))  # for the separator and spaces
         for row in data[0:]:
             print(f"{row[0]:<{col_widths[0]}} | {row[1]:>{col_widths[1]}}")
 
         print("-" * (sum(col_widths) + 3))  # for the separator and spaces
         print()
 
-
+    def _init_logging(self):
+        """Initializes logging for the simulation."""
+        log_filename = os.path.join(self.sim_path,'simulation.log')
+        logging.basicConfig(filename=log_filename, filemode='a', level=logging.DEBUG,
+                            format='%(asctime)s - %(levelname)s - %(message)s')
+        self.logger = logging.getLogger(__name__)
+        self.logger.info(f'Simulation started, using {self._workers} workers')
+        
     def run(self, recipe=None, multiprocessing=1, force=False, overwrite_rml=True):
         """
         Execute simulations with optional recipe, multiprocessing, and file management options.
 
         This method orchestrates the setup and execution of simulations, managing multiprocessing,
         file generation, and progress tracking.
 
@@ -810,23 +823,37 @@
             recipe (SimulationRecipe, optional): Recipe for simulation setup. Defaults to None.
             multiprocessing (int, optional): Number of processes for parallel execution. Defaults to 1.
             force (bool, optional): Force re-execution of simulations. Defaults to False.
             overwrite_rml (bool, optional): Overwrite existing RML files. Defaults to True.
         """
         if not isinstance(multiprocessing, int) or multiprocessing < 1:
             raise ValueError("The 'multiprocessing' argument must be an integer greater than 0.")
+        self._batch_number = 0
+        self._workers = multiprocessing
+        self.batch_size = int(self._workers)*5  
         self._prepare_simulation_environment(recipe, overwrite_rml)
+        self._init_logging()
         total_simulations = self.sp._calc_number_sim() * self.repeat
+        self.simulations_checked = False
 
-        pbar = self._initialize_progress_bar(total_simulations)
-        self._execute_simulations(multiprocessing, force, total_simulations, pbar)
+        pbar = self._initialize_progress_bar(total_simulations, description='Simulations Completed')
+        try:
+            self._execute_simulations(multiprocessing, force, total_simulations, pbar)
+            pbar.close()
+            self.logger.info('Simulation completed successfully.')
+        except Exception as e:
+            self.logger.error('Simulation failed.', exc_info=True) 
         if self.raypyng_analysis:
+            self.logger.info('Starting cleanup')
             pp = PostProcess()
             pp.cleanup(self.sim_path, self.repeat, self._exported_obj_names_list)
-        pbar.close()
+            self.logger.info('Done with the cleanup')
+        self.logger.info('Brute force exit')
+        os._exit(0) # exit brute force
+        
 
     def _remove_recap_files(self,):
 
         # Filter files ending with ".csv" or ".data"
         files_to_remove = ['looper.csv', 'looper.txt']
 
         # Remove filtered files
@@ -858,31 +885,66 @@
             multiprocessing (int): Number of processes for parallel execution.
             force (bool): Force re-execution of simulations.
             total_simulations (int): Total number of simulations to be executed.
             pbar (tqdm): Progress bar object for tracking simulation progress.
         """
         simulations_durations = []  # Track durations of all simulations for average calculation
 
-        with ProcessPoolExecutor(max_workers=multiprocessing) as executor:
-            simulation_params_batch = []
-            batch_length = 0
-            remaining_simulations = total_simulations
-            for round_number in range(self.repeat):
-                for sim_number, params in enumerate(self.sp.simulation_parameters_generator()):
-                    if round_number==0:
-                        self._update_simulation_recap_files(params, sim_number)
-                    if self._is_simulation_missing(sim_number, round_number) or force:
-                        self._prepare_and_submit_simulation(params, sim_number, round_number, simulation_params_batch, executor, force)       
-                    else:
-                        pbar.update(1)  # If not missing or forced, update progress bar directly
-                    batch_length += 1
-                    remaining_simulations -= 1
-                    if batch_length == self.batch_size or remaining_simulations == 0:
-                        self._wait_for_simulation_batch(simulations_durations, simulation_params_batch, executor, pbar)
-                        batch_length = 0
+        try:
+            with ProcessPoolExecutor(max_workers=multiprocessing) as executor:
+                simulation_params_batch = []
+                batch_length = 0
+                remaining_simulations = total_simulations
+                for round_number in range(self.repeat):
+                    self.logger.info(f'Start round {round_number}')
+                    for sim_number, params in enumerate(self.sp.simulation_parameters_generator()):
+                        if round_number==0:
+                            self._update_simulation_recap_files(params, sim_number)
+                        if self._is_simulation_missing(sim_number, round_number) or force:
+                            self._prepare_and_submit_simulation(params, sim_number, round_number, simulation_params_batch, executor, force)       
+                        else:
+                            pbar.update(1)  # If not missing or forced, update progress bar directly
+                        batch_length += 1
+                        remaining_simulations -= 1
+                        if batch_length == self.batch_size or remaining_simulations == 0:
+                            self._wait_for_simulation_batch(simulations_durations, simulation_params_batch, executor, pbar)
+                            self.logger.info(f'Waiting For batch, {self.batch_size} simulations to go')
+                            batch_length = 0
+                        if remaining_simulations == 0:
+                            self.logger.info(f'Remaning Simulations {remaining_simulations}, stop the simulations loop')
+                            self._final_check_on_simulations_and_shutdown(executor, pbar)
+                            break 
+        except Exception as e:
+            self.logger.info(f'Error in _execute simulations: {e}')
+            executor.shutdown(wait=False)
+            self.logger.info('Executor shutdown completed.')
+        
+        
+
+    def _final_check_on_simulations_and_shutdown(self, executor, old_pbar):
+
+        #check that all simulatins are completed:
+        self.logger.info(f'Checking that all simulations are completed before stopping the ProcessPoolExecutor')
+        missing_sim = []
+        for round_number in range(self.repeat):
+            for sim_number, params in enumerate(self.sp.simulation_parameters_generator()):
+                if self._is_simulation_missing(sim_number, round_number):
+                    self.logger.info(f'This simulation is missing: round {round_number}, number {sim_number}')
+                    missing_sim.append({'round': round_number, 'sim_number':sim_number})
+
+        executor.shutdown(wait=False)
+        self.logger.info('Executor shutdown completed.')
+
+        if len(missing_sim) >=1 and self.simulations_checked==False:
+            self.logger.info('Finish missing simulations')
+            total_simulations = self.sp._calc_number_sim() * self.repeat
+            old_pbar.close()
+            pbar = self._initialize_progress_bar(total_simulations,description='Checking Simulations')
+            self.simulations_checked = True
+            self._execute_simulations(self._workers, False, total_simulations, pbar)
 
     def _prepare_and_submit_simulation(self, params, sim_number, round_number, simulation_params_batch, executor, force):
         """
         Prepares and submits a single simulation for execution.
 
         Args:
             params (dict): Parameters for the current simulation.
@@ -892,47 +954,85 @@
             executor (ProcessPoolExecutor): Executor for multiprocessing.
             force (bool): Force re-execution of simulations.
         """
         rml_file_path = self._generate_rml_file(sim_number, round_number, params)
         exp_list = self._make_exports_list(sim_number, round_number)
         simulation_params = ((rml_file_path, self._hide, self.analyze, self.raypyng_analysis, self.ray_path), exp_list)
         simulation_params_batch.append(simulation_params)
+        self.logger.info(f'Prepared sim number: {sim_number}: {rml_file_path}')
+
 
     def _wait_for_simulation_batch(self, simulations_durations, simulation_params_batch, executor, pbar):
         """
         Waits for a batch of simulations to complete and updates the progress bar.
 
         Args:
             simulations_durations (list): List to track durations of completed simulations.
             simulation_params_batch (list): Batch of simulation parameters that were submitted.
             executor (ProcessPoolExecutor): Executor for multiprocessing.
             pbar (tqdm): Progress bar object for tracking simulation progress.
         """
         futures = {executor.submit(run_rml_func, sim_params): sim_params for sim_params in simulation_params_batch}
-        for future in as_completed(futures):
-            try:
-                sim_duration = future.result()
+        completed_sim = 0
+        remaining_simulations = self.batch_size
+        self.logger.info(f'Waiting for batch number: {self._batch_number}, timeout: {self._simulation_timeout}s')
+        self._batch_number += 1
+        try:
+            for future in as_completed(futures, timeout=self._simulation_timeout):
+                sim_duration, rml_filename = future.result()
                 simulations_durations.append(sim_duration)
+                self._simulation_timeout = (np.mean(simulations_durations)*self.batch_size/self._workers*1.2)
                 self._update_progress_bar(simulations_durations, pbar)
+                completed_sim += 1
+                remaining_simulations -= 1
+                self.logger.info(f'Completed: {completed_sim}, remaining: {remaining_simulations}, {rml_filename}')
+                # if remaining_simulations == 1:
+                #     break
+        except Exception as e:
+            self.logger.info(f'Exception during simulation: {e}')
+            try:
+                for sim in simulation_params_batch:
+                    _,exp_list = sim
+                    # self.logger.info(f'Extracting exp_list {type(exp_list)}, {exp_list}')
+                    exp = exp_list[0]
+                    # self.logger.info(f'Extracting exp {type(exp)}, {exp}')
+                    # self.logger.info(f'Extracting exp[-2] {type(exp[-2])}, {exp[-2]}')
+                    # self.logger.info(f'Extracting exp[-1] {type(exp[-1])}, {exp[-1]}')
+                    round_n = int(re.findall(r'\d+', exp[-2])[0])
+                    # self.logger.info('Extracting sim_n')
+                    sim_n = int(re.findall(r'\d+', exp[-1])[0])
+                    # self.logger.info(f'round_n: {round_n}')
+                    # self.logger.info(f'sim_n: {sim_n}')
+                    sim_file = sim[0][0]
+                    # self.logger.info(f'Waiting for {sim_file}')
+                    while self._is_simulation_missing(sim_n, round_n)==False:
+                        time.sleep(5)
+                        self.logger.info(f'Waiting for file {sim_file}')
             except Exception as e:
-                print(f"Exception during simulation: {e}")
+                self.logger.info(f'Exception checking simulations: {e}')
+            self.logger.info(f'Found all simulations of the batch, futures missed {remaining_simulations} simulations')
+            for i in range(remaining_simulations):
+                self._update_progress_bar(simulations_durations, pbar)
+            self.logger.info('Updated progress bar')
+            
         simulation_params_batch.clear()  # Reset batch for next set of simulations
+        self.logger.info(f'Batch Completed')
 
     def _update_progress_bar(self, simulations_durations, pbar):
         """
         Updates the progress bar based on completed simulations.
 
         Args:
             simulations_durations (list): List of durations for completed simulations.
             pbar (tqdm): Progress bar object for tracking simulation progress.
         """
         avg_duration = sum(simulations_durations) / len(simulations_durations)
         last_duration = simulations_durations[-1]
         remaining_simulations = pbar.total - pbar.n
-        eta_seconds = avg_duration * remaining_simulations
+        eta_seconds = avg_duration * remaining_simulations / self._workers
         eta_str = self._format_eta(eta_seconds)
         pbar.set_postfix_str(f"ETA: {eta_str}, Last: {last_duration:.2f}s, Avg: {avg_duration:.2f}s/it", refresh=True)
         pbar.update(1)
 
     def _setup_simulation_environment(self, recipe):
         """
         Sets up the simulation environment based on the provided recipe.
@@ -999,9 +1099,9 @@
         try:
             api.quit()
         except Exception as e:
             print(f"WARNING! Got exception while quitting API for {rml_filename}, the error was: {e}")
         runner.kill()
     et = time.time()
     simulation_duration = et-st
-    return simulation_duration
+    return simulation_duration, rml_filename
```

### Comparing `raypyng-1.2.4/src/raypyng/wave_helper.py` & `raypyng-1.2.5/src/raypyng/wave_helper.py`

 * *Files identical despite different names*

### Comparing `raypyng-1.2.4/src/raypyng/xmltools/__init__.py` & `raypyng-1.2.5/src/raypyng/xmltools/__init__.py`

 * *Files identical despite different names*

### Comparing `raypyng-1.2.4/src/raypyng/xmltools/attributes.py` & `raypyng-1.2.5/src/raypyng/xmltools/attributes.py`

 * *Files identical despite different names*

### Comparing `raypyng-1.2.4/src/raypyng/xmltools/dictionaries.py` & `raypyng-1.2.5/src/raypyng/xmltools/dictionaries.py`

 * *Files identical despite different names*

### Comparing `raypyng-1.2.4/src/raypyng/xmltools/elements.py` & `raypyng-1.2.5/src/raypyng/xmltools/elements.py`

 * *Files identical despite different names*

### Comparing `raypyng-1.2.4/src/raypyng/xmltools/parser.py` & `raypyng-1.2.5/src/raypyng/xmltools/parser.py`

 * *Files identical despite different names*

### Comparing `raypyng-1.2.4/src/raypyng.egg-info/PKG-INFO` & `raypyng-1.2.5/src/raypyng.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: raypyng
-Version: 1.2.4
+Version: 1.2.5
 Summary: Python interface for RAY-UI x-ray tracing program
-Author-email: "Simone Vadilonga, Ruslan Ovsyannikov" <simone.vadilonga@helmholtz-berlin.de>
+Author-email: "Simone Vadilonga, Ruslan Ovsyannikov, Sebastian Sachse" <simone.vadilonga@helmholtz-berlin.de>
 License: The MIT License (MIT)
         
         Copyright (c) <2022> <Simone Vadilonga, Ruslan Ovsyannikov>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -34,14 +34,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.22.0
 Requires-Dist: psutil>=5.9.1
 Requires-Dist: joblib>=1.1.0
 Requires-Dist: matplotlib>=3.5.1
 Requires-Dist: natsort>=8.2.0
+Requires-Dist: tqdm
 
 ## Project Description
 raypyng provides a simple API to work with RAY-UI, a software for optical simulation of synchrotron beamlines and x-ray systems developed by Helmholtz-Zentrum Berlin.
 
 raypyng works only under linux distributions.
 
 [Documentation](https://raypyng.readthedocs.io/en/latest/index.html)
```

### Comparing `raypyng-1.2.4/src/raypyng.egg-info/SOURCES.txt` & `raypyng-1.2.5/src/raypyng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raypyng-1.2.4/tests/test_analyze.py` & `raypyng-1.2.5/tests/test_analyze.py`

 * *Files identical despite different names*

### Comparing `raypyng-1.2.4/tests/test_no_analyze.py` & `raypyng-1.2.5/tests/test_no_analyze.py`

 * *Files identical despite different names*

### Comparing `raypyng-1.2.4/tests/test_simulation_class.py` & `raypyng-1.2.5/tests/test_simulation_class.py`

 * *Files identical despite different names*

