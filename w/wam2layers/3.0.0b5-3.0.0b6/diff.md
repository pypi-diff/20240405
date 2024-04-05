# Comparing `tmp/wam2layers-3.0.0b5.tar.gz` & `tmp/wam2layers-3.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wam2layers-3.0.0b5.tar", last modified: Fri Jul 21 14:39:21 2023, max compression
+gzip compressed data, was "wam2layers-3.0.0b6.tar", last modified: Fri Dec 22 15:56:21 2023, max compression
```

## Comparing `wam2layers-3.0.0b5.tar` & `wam2layers-3.0.0b6.tar`

### file list

```diff
@@ -1,37 +1,46 @@
-drwxr-xr-x   0 benedicti (58930) benedicti (58450)        0 2023-07-21 14:39:21.071417 wam2layers-3.0.0b5/
--rw-r--r--   0 benedicti (58930) benedicti (58450)    11357 2022-08-29 13:06:00.000000 wam2layers-3.0.0b5/LICENSE
--rw-r--r--   0 benedicti (58930) benedicti (58450)     3430 2023-07-21 14:39:21.070751 wam2layers-3.0.0b5/PKG-INFO
--rw-r--r--   0 benedicti (58930) benedicti (58450)     2640 2023-07-21 09:55:28.000000 wam2layers-3.0.0b5/README.md
--rw-r--r--   0 benedicti (58930) benedicti (58450)     1422 2023-07-21 14:38:17.000000 wam2layers-3.0.0b5/pyproject.toml
--rw-r--r--   0 benedicti (58930) benedicti (58450)       38 2023-07-21 14:39:21.071551 wam2layers-3.0.0b5/setup.cfg
-drwxr-xr-x   0 benedicti (58930) benedicti (58450)        0 2023-07-21 14:39:21.046168 wam2layers-3.0.0b5/src/
-drwxr-xr-x   0 benedicti (58930) benedicti (58450)        0 2023-07-21 14:39:21.052935 wam2layers-3.0.0b5/src/wam2layers/
--rw-r--r--   0 benedicti (58930) benedicti (58450)        0 2022-09-20 13:04:20.000000 wam2layers-3.0.0b5/src/wam2layers/__init__.py
-drwxr-xr-x   0 benedicti (58930) benedicti (58450)        0 2023-07-21 14:39:21.059237 wam2layers-3.0.0b5/src/wam2layers/analysis/
--rw-r--r--   0 benedicti (58930) benedicti (58450)        0 2022-09-20 13:04:20.000000 wam2layers-3.0.0b5/src/wam2layers/analysis/__init__.py
--rw-rw----   0 benedicti (58930) benedicti (58450)     5181 2022-12-23 15:27:06.000000 wam2layers-3.0.0b5/src/wam2layers/analysis/checks.py
--rw-r--r--   0 benedicti (58930) benedicti (58450)     8326 2023-07-21 14:38:17.000000 wam2layers-3.0.0b5/src/wam2layers/analysis/visualization.py
--rw-rw----   0 benedicti (58930) benedicti (58450)      492 2022-12-23 15:27:06.000000 wam2layers-3.0.0b5/src/wam2layers/cli.py
--rw-r--r--   0 benedicti (58930) benedicti (58450)     8578 2023-07-21 14:36:06.000000 wam2layers-3.0.0b5/src/wam2layers/config.py
-drwxr-xr-x   0 benedicti (58930) benedicti (58450)        0 2023-07-21 14:39:21.064039 wam2layers-3.0.0b5/src/wam2layers/preprocessing/
--rw-r--r--   0 benedicti (58930) benedicti (58450)        0 2022-09-20 13:04:20.000000 wam2layers-3.0.0b5/src/wam2layers/preprocessing/__init__.py
--rw-rw----   0 benedicti (58930) benedicti (58450)      216 2022-12-23 15:27:06.000000 wam2layers-3.0.0b5/src/wam2layers/preprocessing/cli.py
--rw-r--r--   0 benedicti (58930) benedicti (58450)    12555 2023-07-21 14:38:17.000000 wam2layers-3.0.0b5/src/wam2layers/preprocessing/era5.py
--rw-r--r--   0 benedicti (58930) benedicti (58450)     9801 2023-07-21 14:36:06.000000 wam2layers-3.0.0b5/src/wam2layers/preprocessing/shared.py
--rw-r--r--   0 benedicti (58930) benedicti (58450)    10385 2022-09-20 13:04:20.000000 wam2layers-3.0.0b5/src/wam2layers/preprocessing/tableERA5model_to_pressure.csv
-drwxr-xr-x   0 benedicti (58930) benedicti (58450)        0 2023-07-21 14:39:21.065957 wam2layers-3.0.0b5/src/wam2layers/tracking/
--rw-r--r--   0 benedicti (58930) benedicti (58450)        0 2022-09-20 13:04:20.000000 wam2layers-3.0.0b5/src/wam2layers/tracking/__init__.py
--rw-r--r--   0 benedicti (58930) benedicti (58450)    17268 2023-07-21 09:55:28.000000 wam2layers-3.0.0b5/src/wam2layers/tracking/backtrack.py
-drwxr-xr-x   0 benedicti (58930) benedicti (58450)        0 2023-07-21 14:39:21.068892 wam2layers-3.0.0b5/src/wam2layers/utils/
--rw-rw----   0 benedicti (58930) benedicti (58450)        0 2022-11-18 10:00:46.000000 wam2layers-3.0.0b5/src/wam2layers/utils/__init__.py
--rw-rw----   0 benedicti (58930) benedicti (58450)     2458 2022-12-23 15:27:06.000000 wam2layers-3.0.0b5/src/wam2layers/utils/profiling.py
--rw-r--r--   0 benedicti (58930) benedicti (58450)    11727 2023-07-21 14:36:06.000000 wam2layers-3.0.0b5/src/wam2layers/utils/source_region.py
-drwxr-xr-x   0 benedicti (58930) benedicti (58450)        0 2023-07-21 14:39:21.056499 wam2layers-3.0.0b5/src/wam2layers.egg-info/
--rw-r--r--   0 benedicti (58930) benedicti (58450)     3430 2023-07-21 14:39:21.053706 wam2layers-3.0.0b5/src/wam2layers.egg-info/PKG-INFO
--rw-r--r--   0 benedicti (58930) benedicti (58450)      859 2023-07-21 14:39:21.054161 wam2layers-3.0.0b5/src/wam2layers.egg-info/SOURCES.txt
--rw-r--r--   0 benedicti (58930) benedicti (58450)        1 2023-07-21 14:39:21.054652 wam2layers-3.0.0b5/src/wam2layers.egg-info/dependency_links.txt
--rw-r--r--   0 benedicti (58930) benedicti (58450)       50 2023-07-21 14:39:21.055310 wam2layers-3.0.0b5/src/wam2layers.egg-info/entry_points.txt
--rw-r--r--   0 benedicti (58930) benedicti (58450)      208 2023-07-21 14:39:21.056002 wam2layers-3.0.0b5/src/wam2layers.egg-info/requires.txt
--rw-r--r--   0 benedicti (58930) benedicti (58450)       11 2023-07-21 14:39:21.056619 wam2layers-3.0.0b5/src/wam2layers.egg-info/top_level.txt
-drwxr-xr-x   0 benedicti (58930) benedicti (58450)        0 2023-07-21 14:39:21.069981 wam2layers-3.0.0b5/tests/
--rw-r--r--   0 benedicti (58930) benedicti (58450)      442 2023-07-21 09:36:37.000000 wam2layers-3.0.0b5/tests/test_config.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-12-22 15:56:21.474485 wam2layers-3.0.0b6/
+-rw-r--r--   0 peter     (1000) peter     (1000)    11357 2023-03-06 16:45:46.000000 wam2layers-3.0.0b6/LICENSE
+-rw-r--r--   0 peter     (1000) peter     (1000)     4461 2023-12-22 15:56:21.474485 wam2layers-3.0.0b6/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)     2810 2023-12-22 15:33:44.000000 wam2layers-3.0.0b6/README.md
+-rw-r--r--   0 peter     (1000) peter     (1000)     1472 2023-12-22 15:55:52.000000 wam2layers-3.0.0b6/pyproject.toml
+-rw-r--r--   0 peter     (1000) peter     (1000)       38 2023-12-22 15:56:21.474485 wam2layers-3.0.0b6/setup.cfg
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-12-22 15:56:21.464485 wam2layers-3.0.0b6/src/
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-12-22 15:56:21.464485 wam2layers-3.0.0b6/src/wam2layers/
+-rw-r--r--   0 peter     (1000) peter     (1000)        0 2023-03-06 16:45:46.000000 wam2layers-3.0.0b6/src/wam2layers/__init__.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-12-22 15:56:21.474485 wam2layers-3.0.0b6/src/wam2layers/analysis/
+-rw-r--r--   0 peter     (1000) peter     (1000)        0 2023-03-06 16:45:46.000000 wam2layers-3.0.0b6/src/wam2layers/analysis/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5181 2023-10-05 13:20:15.000000 wam2layers-3.0.0b6/src/wam2layers/analysis/checks.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     7479 2023-12-22 15:33:44.000000 wam2layers-3.0.0b6/src/wam2layers/analysis/visualization.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5839 2023-12-22 15:25:52.000000 wam2layers-3.0.0b6/src/wam2layers/cli.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    10379 2023-12-22 15:33:44.000000 wam2layers-3.0.0b6/src/wam2layers/config.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      814 2023-10-06 06:10:07.000000 wam2layers-3.0.0b6/src/wam2layers/grid.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-12-22 15:56:21.474485 wam2layers-3.0.0b6/src/wam2layers/preprocessing/
+-rw-r--r--   0 peter     (1000) peter     (1000)        0 2023-03-06 16:45:46.000000 wam2layers-3.0.0b6/src/wam2layers/preprocessing/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    12195 2023-12-22 15:25:52.000000 wam2layers-3.0.0b6/src/wam2layers/preprocessing/era5.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    15890 2023-12-22 15:33:44.000000 wam2layers-3.0.0b6/src/wam2layers/preprocessing/shared.py
+-rw-r--r--   0 peter     (1000) peter     (1000)       32 2023-04-21 09:11:52.000000 wam2layers-3.0.0b6/src/wam2layers/preprocessing/sum.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    10386 2023-11-14 15:55:17.000000 wam2layers-3.0.0b6/src/wam2layers/preprocessing/tableERA5model_to_pressure.csv
+-rw-r--r--   0 peter     (1000) peter     (1000)     1613 2023-12-22 15:25:52.000000 wam2layers-3.0.0b6/src/wam2layers/preprocessing/xarray_append.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-12-22 15:56:21.474485 wam2layers-3.0.0b6/src/wam2layers/tracking/
+-rw-r--r--   0 peter     (1000) peter     (1000)        0 2023-03-06 16:45:46.000000 wam2layers-3.0.0b6/src/wam2layers/tracking/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     9001 2023-12-22 15:33:44.000000 wam2layers-3.0.0b6/src/wam2layers/tracking/backtrack.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4098 2023-12-18 09:40:36.000000 wam2layers-3.0.0b6/src/wam2layers/tracking/core.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     9306 2023-12-22 15:33:44.000000 wam2layers-3.0.0b6/src/wam2layers/tracking/forwardtrack.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3012 2023-12-22 15:33:44.000000 wam2layers-3.0.0b6/src/wam2layers/tracking/io.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1135 2023-12-22 15:33:44.000000 wam2layers-3.0.0b6/src/wam2layers/tracking/shared.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-12-22 15:56:21.474485 wam2layers-3.0.0b6/src/wam2layers/utils/
+-rw-r--r--   0 peter     (1000) peter     (1000)        0 2023-12-22 15:25:52.000000 wam2layers-3.0.0b6/src/wam2layers/utils/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      268 2023-10-03 11:19:29.000000 wam2layers-3.0.0b6/src/wam2layers/utils/grids.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5480 2023-12-22 15:33:44.000000 wam2layers-3.0.0b6/src/wam2layers/utils/profiling.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    19145 2023-12-22 15:41:42.000000 wam2layers-3.0.0b6/src/wam2layers/utils/tagging_region.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-12-22 15:56:21.474485 wam2layers-3.0.0b6/src/wam2layers.egg-info/
+-rw-r--r--   0 peter     (1000) peter     (1000)     4461 2023-12-22 15:56:21.000000 wam2layers-3.0.0b6/src/wam2layers.egg-info/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)     1135 2023-12-22 15:56:21.000000 wam2layers-3.0.0b6/src/wam2layers.egg-info/SOURCES.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2023-12-22 15:56:21.000000 wam2layers-3.0.0b6/src/wam2layers.egg-info/dependency_links.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       50 2023-12-22 15:56:21.000000 wam2layers-3.0.0b6/src/wam2layers.egg-info/entry_points.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)      219 2023-12-22 15:56:21.000000 wam2layers-3.0.0b6/src/wam2layers.egg-info/requires.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       11 2023-12-22 15:56:21.000000 wam2layers-3.0.0b6/src/wam2layers.egg-info/top_level.txt
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-12-22 15:56:21.474485 wam2layers-3.0.0b6/tests/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2971 2023-12-22 15:33:44.000000 wam2layers-3.0.0b6/tests/test_config.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1154 2023-12-22 15:33:44.000000 wam2layers-3.0.0b6/tests/test_io.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4115 2023-12-22 15:33:44.000000 wam2layers-3.0.0b6/tests/test_workflow.py
```

### Comparing `wam2layers-3.0.0b5/LICENSE` & `wam2layers-3.0.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `wam2layers-3.0.0b5/PKG-INFO` & `wam2layers-3.0.0b6/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,73 +1,53 @@
-Metadata-Version: 2.1
-Name: wam2layers
-Version: 3.0.0b5
-Summary: Atmospheric moisture tracking model
-License: Apache 2.0
-Project-URL: Documentation, https://wam2layers.readthedocs.io/en/latest
-Project-URL: Source code, https://github.com/WAM2layers/WAM2layers
-Keywords: atmospheric rivers,hydrological cycle,meteorology,moisture recycling,moisture tracking
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
-Classifier: Topic :: Scientific/Engineering :: Hydrology
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: develop
-License-File: LICENSE
-
 [![DOI](https://zenodo.org/badge/471007521.svg)](https://zenodo.org/badge/latestdoi/471007521)
 [![Documentation Status](https://readthedocs.org/projects/wam2layers/badge/?version=latest)](https://wam2layers.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/wam2layers)](https://pypi.org/project/wam2layers/)
 
 # Atmospheric moisture tracking
 
 https://user-images.githubusercontent.com/17080502/233834536-a82ca96d-e303-4592-a588-472097ebe6c5.mp4
 
 This repository contains the source code of the WAM2layers moisture tracking
 code. It can be used to determine where
 precipitation originally evaporated (backtracking), or where evaporated moisture
-eventually ends up (forward tracking). 
+eventually ends up (forward tracking).
 
-The animation above illustrates the concept of backtracking: you first see the water 
-content and fluxes move forward in time (left panel). Midway through, the animation 
+The animation above illustrates the concept of backtracking: you first see the water
+content and fluxes move forward in time (left panel). Midway through, the animation
 reverses and the moisture from the "source region" is tracked backward in time (right panel).
 
 
 This code is currently developed by a core team:
 Ruud van der Ent (Delft University of Technology)
 Imme Benedict (Wageningen University)
 Chris Weijenborg (Wageningen University)
-Vincent de Feiter (Wageningen University)
 Peter Kalverla (Netherlands eScienceCenter)
 
 # How to use
 See the [documentation](https://wam2layers.readthedocs.io/en/latest/) for a more detailed description. Still questions? Follow the flowchart below.
 
 ![FlowChart GitHub](https://github.com/WAM2layers/WAM2layers/assets/123247866/f5cbcf8f-a45f-4e73-b304-00956b4e2ee5)
 
 
 # Other versions
 
 This is the official codebase for the WAM-2layers moisture tracking model as of
-18/03/2022, but there are still several other older versions around:
+18/03/2022, but there are still several other (older) versions around:
 
 - [Original Python code for ERA-Interim by Ruud van der Ent](https://github.com/ruudvdent/WAM2layersPython)
 - [Adapted version for EC-Earth by Imme Benedict](https://github.com/Imme1992/moisture_tracking_mississippi)
 - [Adapted version for MERRA2 by Pat Keys](https://github.com/pkeys/WAM2layersPythonMerra2)
 - [Adapted version for ERA5 pressure levels by Mingzhong Xiao](https://zenodo.org/record/4796962#.Y25d1-TMIVA)
+- [Adapted version for ERA5 by Theo Carr](https://github.com/ktcarr/WAM2layers_ERA5)
 
 # Reuse and acknowledgement
 
 We are actively developing the code at the moment, so it may be subject to
-change. We encourage anyone who is interested in re-using the code to get in
-touch. We may be able to help.
+change. We aim for backward compatability from v3.0.0 onward. We encourage anyone who is interested in re-using the code to get in
+touch on the discussion pages. We may be able to help and you may be able to help us getting rid off bugs.
 
 If you use the code for a publication, please cite it using the [DOI of the
 appropriate release](https://doi.org/10.5281/zenodo.7010594) and the
-following paper: 
+following paper:
 [Contrasting roles of interception and transpiration in the
 hydrological cycle - Part 2: Moisture
 recycling](https://doi.org/10.5194/esd-5-471-2014)
-
```

### Comparing `wam2layers-3.0.0b5/pyproject.toml` & `wam2layers-3.0.0b6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wam2layers"
 description = "Atmospheric moisture tracking model"
-version = "3.0.0-beta.5"
+version = "3.0.0-beta.6"
 readme = "README.md"
 license = { text = "Apache 2.0" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
@@ -48,21 +48,25 @@
     "cffconvert",
     "isort",
     "myst-nb",
     "sphinx_rtd_theme",
     "sphinx",
     "myst-nb",
     "pytest",
+    "pre-commit",
     "flake8",
     "build",
     "twine",
 ]
 
 [project.urls]
 Documentation = "https://wam2layers.readthedocs.io/en/latest"
 "Source code" = "https://github.com/WAM2layers/WAM2layers"
 
 [project.scripts]
 wam2layers = "wam2layers.cli:cli"
 
 [tool.setuptools.package-data]
 "wam2layers.preprocessing" = ["*.csv"]
+
+[tool.isort]
+profile = "black"
```

### Comparing `wam2layers-3.0.0b5/src/wam2layers/analysis/checks.py` & `wam2layers-3.0.0b6/src/wam2layers/analysis/checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 def _warning_on_one_line(message, category, filename, lineno, file=None, line=None):
     """A more compact warning format.
 
     https://stackoverflow.com/a/26433913
     """
-    short_path = Path(filename).relative_to(Path(filename).parents[2])
+    short_path = Path(filename).relative_to(Path(filename).parents[0])
     return f"{short_path}:{lineno}: {category.__name__}: {message}\n"
 
 
 # Override the format with which warnings are printed
 warnings.formatwarning = _warning_on_one_line
```

### Comparing `wam2layers-3.0.0b5/src/wam2layers/analysis/visualization.py` & `wam2layers-3.0.0b6/src/wam2layers/analysis/visualization.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+import logging
 from pathlib import Path
 
-import click
 import matplotlib.pyplot as plt
 import pandas as pd
 import xarray as xr
 from cmocean import cm
 
 from wam2layers.config import Config
 from wam2layers.preprocessing.shared import get_grid_info
-from wam2layers.tracking.backtrack import input_path, load_region, output_path
+from wam2layers.tracking.io import input_path, load_tagging_region, output_path
+
+logger = logging.getLogger(__name__)
 
 
 def try_import_cartopy():
     """Import cartopy if it is available; else raise."""
     from importlib import import_module
 
     global crs
@@ -32,15 +34,15 @@
     ax.set_xlim(region.longitude.min(), region.longitude.max())
     ax.set_ylim(region.latitude.min(), region.latitude.max())
 
 
 def _plot_precip(config, ax):
     """Return subplot with precip."""
     # Load config and some usful stuf.
-    region = load_region(config)
+    region = load_tagging_region(config)
 
     # Load data
     dates = pd.date_range(
         start=config.preprocess_start_date,
         end=config.preprocess_end_date,
         freq=config.output_frequency,  # Should be output frequency, since this is used to save the data
         inclusive="left",
@@ -48,51 +50,55 @@
 
     input_files = []
     for date in dates:
         input_files.append(input_path(date, config))
 
     ds = xr.open_mfdataset(input_files, combine="nested", concat_dim="time")
     # TODO: make region time-dependent
-    start = config.event_start_date
-    end = config.event_end_date
+    start = config.tagging_start_date
+    end = config.tagging_end_date
     subset = ds.precip.sel(time=slice(start, end))
     precip = (subset * region * 3600).sum("time").compute()
 
     # Make figure
     precip.plot(ax=ax, cmap=cm.rain, cbar_kwargs=dict(fraction=0.05, shrink=0.5))
     ax.set_title("Cumulative precipitation during event [mm]", loc="left")
     polish(ax, region.where(region > 0, drop=True))
 
 
 def _plot_evap(config, ax):
     """Return subplot with tracked evaporation."""
-    region = load_region(config)
+    region = load_tagging_region(config)
     a_gridcell, lx, ly = get_grid_info(region)
 
     # Load data
     dates = pd.date_range(
-        start=config.track_start_date,
-        end=config.track_end_date,
+        start=config.tracking_start_date,
+        end=config.tracking_end_date,
         freq=config.output_frequency,
         inclusive="left",
-    )
+    )[1:]
 
     output_files = []
     for date in dates:
-        output_files.append(output_path(date, config))
+        output_files.append(output_path(date, config, mode="backtrack"))
 
     ds = xr.open_mfdataset(output_files, combine="nested", concat_dim="time")
     e_track = ds.e_track.sum("time").compute() * 1000 / a_gridcell[:, None]
 
     # Make figure
     e_track.plot(
-        ax=ax, vmin=0, cmap=cm.rain, cbar_kwargs=dict(fraction=0.05, shrink=0.5)
+        ax=ax,
+        vmin=0,
+        robust=True,
+        cmap=cm.rain,
+        cbar_kwargs=dict(fraction=0.05, shrink=0.5),
     )
     e_track.plot.contour(ax=ax, levels=[0.1, 1], colors=["lightgrey", "grey"])
-    ax.set_title("Moisture source of extreme precip [mm]", loc="left")
+    ax.set_title("Accumulated tracked moisture [mm]", loc="left")
 
     # Add source region outline
     region.plot.contour(ax=ax, levels=[1], colors="k")
     polish(ax, region)
 
 
 def visualize_input_data(config_file):
@@ -107,54 +113,60 @@
     ax = fig.add_subplot(111, projection=crs.PlateCarree())
 
     _plot_precip(config, ax)
 
     # Save
     out_dir = Path(config.output_folder) / "figures"
     out_dir.mkdir(exist_ok=True, parents=True)
-    fig.savefig(out_dir / "input_event.png", dpi=200)
+    path_to_fig = out_dir / "input_event.png"
+    fig.savefig(path_to_fig, dpi=200)
+    logger.info(f"Figure of cumulative moisture inputs written to {path_to_fig}.")
 
 
 def visualize_output_data(config_file):
     """An figure showing the cumulative moisture origins.
 
     TODO: make figure creation independent of case.
     """
-    # Load config and some usful stuf.
+    # Load config and some useful stuf.
     config = Config.from_yaml(config_file)
 
     # Make figure
     fig = plt.figure(figsize=(16, 10))
     ax = fig.add_subplot(111, projection=crs.PlateCarree())
 
     _plot_evap(config, ax)
 
     # Save
     out_dir = Path(config.output_folder) / "figures"
     out_dir.mkdir(exist_ok=True, parents=True)
-    fig.savefig(out_dir / "cumulative_sources.png", dpi=200)
+    path_to_fig = out_dir / "cumulative_sources.png"
+    fig.savefig(path_to_fig, dpi=200)
+    logger.info(f"Figure of cumulative moisture origins written to {path_to_fig}.")
 
 
 def visualize_both(config_file):
     """Diagnostic figure with four subplots combining input and output data."""
-    # Load config and some usful stuf.
+    # Load config and some useful stuf.
     config = Config.from_yaml(config_file)
 
     # Make figure
     fig, [ax1, ax2] = plt.subplots(
         2, 1, figsize=(16, 10), subplot_kw=dict(projection=crs.PlateCarree())
     )
 
     _plot_precip(config, ax1)
     _plot_evap(config, ax2)
 
     # Save
     out_dir = Path(config.output_folder) / "figures"
     out_dir.mkdir(exist_ok=True, parents=True)
-    fig.savefig(out_dir / "summary_subplots.png", dpi=200)
+    path_to_fig = out_dir / "summary_subplots.png"
+    fig.savefig(path_to_fig, dpi=200)
+    logger.info(f"Diagnostic figure of input and output data written to {path_to_fig}.")
 
 
 def visualize_snapshots(config_file):
     """Diagnostic figure with four subplots combining input and output data."""
     config = Config.from_yaml(config_file)
     dates = pd.date_range(
         start=config.track_start_date,
@@ -165,29 +177,29 @@
     region = load_region(config)
     a_gridcell, lx, ly = get_grid_info(region)
 
     out_dir = Path(config.output_folder) / "figures"
     out_dir.mkdir(exist_ok=True, parents=True)
 
     for date in dates:
-        print(date)
+        logger.info(date)
         ds_in = xr.open_dataset(input_path(date, config))
         ds_out = xr.open_dataset(output_path(date, config))
 
         # Make figure
         fig, [[ax1, ax2], [ax3, ax4]] = plt.subplots(
             2, 2, subplot_kw=dict(projection=crs.PlateCarree()), figsize=(14, 8)
         )
 
-        ax1.set_title("Tracked precipitation" + date.strftime("%Y%m%d"))
+        ax1.set_title("Tagged moisture" + date.strftime("%Y%m%d"))
         precip = ds_in.precip.sum("time") * region / a_gridcell[:, None] * 1000
         precip.plot(ax=ax1, cmap="Blues")
         polish(ax1, region)
 
-        ax2.set_title("Moisture source")
+        ax2.set_title("Tracked moisture")
         e_track = ds_out.e_track / a_gridcell[:, None] * 1000
         e_track.plot(ax=ax2, cmap="GnBu")
         polish(ax2, region)
 
         ax3.set_title("S track upper layer")
         s_track_upper = ds_out.s_track_upper_restart / a_gridcell[:, None] * 1000
         s_track_upper.plot(ax=ax3, cmap="YlOrRd")
@@ -214,57 +226,8 @@
         )
         polish(ax4, region)
 
         # Save
         output_file = out_dir / f"input_output_{date.strftime('%Y%m%d')}.png"
         fig.savefig(output_file)
         plt.close()
-
-
-###########################################################################
-# The code below makes it possible to run wam2layers from the command line:
-# >>> python visualization.py input path/to/cases/era5_2021.yaml
-# or even:
-# >>> wam2layers visualize output path/to/cases/era5_2021.yaml
-###########################################################################
-
-
-@click.group()
-def cli():
-    """Visualize input or output data of a WAM2layers experiment"""
-    pass
-
-
-@cli.command()
-@click.argument("config_file", type=click.Path(exists=True))
-def input(config_file):
-    """Visualize input data for experiment."""
-    try_import_cartopy()
-    visualize_input_data(config_file)
-
-
-@cli.command()
-@click.argument("config_file", type=click.Path(exists=True))
-def output(config_file):
-    """Visualize output data for experiment."""
-    try_import_cartopy()
-    visualize_output_data(config_file)
-
-
-@cli.command()
-@click.argument("config_file", type=click.Path(exists=True))
-def both(config_file):
-    """Visualize both input and output data for experiment."""
-    try_import_cartopy()
-    visualize_both(config_file)
-
-
-@cli.command()
-@click.argument("config_file", type=click.Path(exists=True))
-def snapshots(config_file):
-    """Visualize input and output snapshots for experiment."""
-    try_import_cartopy()
-    visualize_snapshots(config_file)
-
-
-if __name__ == "__main__":
-    cli()
+        logger.info(f"Snapshot figure written to {output_file}.")
```

### Comparing `wam2layers-3.0.0b5/src/wam2layers/config.py` & `wam2layers-3.0.0b6/src/wam2layers/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,47 @@
+import logging
 from datetime import datetime
 from pathlib import Path
-from typing import Dict, List, Literal, Optional, Union
+from typing import Dict, List, Literal, NamedTuple, Optional, Union
 
 import yaml
-from pydantic import BaseModel, ConfigDict, FilePath, field_validator, model_validator
+from pydantic import (
+    AfterValidator,
+    BaseModel,
+    ConfigDict,
+    Field,
+    FilePath,
+    field_validator,
+    model_validator,
+)
+from typing_extensions import Annotated
+
+logger = logging.getLogger(__name__)
+
+
+class BoundingBox(NamedTuple):
+    west: Annotated[float, Field(ge=-180, le=180)]
+    south: Annotated[float, Field(ge=-80, le=80)]
+    east: Annotated[float, Field(ge=-180, le=180)]
+    north: Annotated[float, Field(ge=-80, le=80)]
+
+
+def validate_region(region):
+    """Check if region is existing path or valid bbox."""
+    if isinstance(region, Path):
+        return region.absolute()
+
+    assert -180 <= region.west <= 180, "longitude should be between -180 and 180"
+    assert -180 <= region.east <= 180, "longitude should be between -180 and 180"
+    assert -80 <= region.north <= 80, "latitude should be between -80 and 80"
+    assert -80 <= region.south <= 80, "latitude should be between -80 and 80"
+    assert region.south < region.north, "south should be smaller than north"
+    if region.west > region.east:
+        logger.info("west > east, coordinates will be rolled around meridian")
+    return region
 
 
 class Config(BaseModel):
     # Pydantic configuration
     model_config = ConfigDict(validate_assignment=True)
 
     # Configuration settings
@@ -42,24 +76,59 @@
 
     .. code-block:: yaml
 
         preprocessed_data_folder: ~/floodcase_202107/preprocessed_data
 
     """
 
-    region: FilePath
-    """Location where the region mask is stored.
+    tagging_region: Annotated[
+        Union[FilePath, BoundingBox], AfterValidator(validate_region)
+    ]
+    """Subdomain delimiting the source/sink regions for tagged moisture.
 
-    The file should exist.
+    You can either specify a path that contains a netcdf file, or a bounding box
+    of the form [west, south, east, north].
+
+    The bounding box should be inside -180, -80, 180, 80; if west > south, the
+    coordinates will be rolled to retain a continous longitude.
+
+    The file should exist. If it has a time dimension, the nearest field will be
+    used as tagging region, and the time should still be between
+    tagging_start_date and tagging_end_date
+
+    For example:
+
+    .. code-block:: yaml
+
+        tagging_region: /data/volume_2/era5_2021/tagging_region_global.nc
+        tagging_region: [0, 50, 10, 55]
+    """
+
+    tracking_domain: Optional[
+        Annotated[BoundingBox, AfterValidator(validate_region)]
+    ] = None
+    """Subdomain delimiting the region considered during tracking.
+
+    This is useful when you have global pre-processed data but you don't need
+    global tracking.
+
+    You can specify a bounding box of the form [west, south, east, north].
+
+    The bounding box should be inside -180, -80, 180, 80; if west > south, the
+    coordinates will be rolled to retain a continous longitude.
+
+    If it is set to `null`, then it will use full domain of preprocessed data.
+
+    Note that you should always set period to False if you use a subdomain.
 
     For example:
 
     .. code-block:: yaml
 
-        region: /data/volume_2/era5_2021/source_region_global.nc
+        tracking_domain: [0, 50, 10, 55]
 
     """
 
     output_folder: Path
     """Location where output of tracking and analysis should be written.
 
     For example:
@@ -93,77 +162,77 @@
     For example:
 
     .. code-block:: yaml
 
         preprocess_end_date: "2021-07-15T23:00"
     """
 
-    track_start_date: datetime
+    tracking_start_date: datetime
     """Start date for tracking.
 
     Should be formatted as: `"YYYY-MM-DD[T]HH:MM"`. Start date < end date, even if
     backtracking.
-    When backward tracking the track_start_date is not given as output date.
+    When backward tracking the tracking_start_date is not given as output date.
 
     For example:
 
     .. code-block:: yaml
 
-        track_start_date: "2021-07-01T00:00"
+        tracking_start_date: "2021-07-01T00:00"
 
     """
 
-    track_end_date: datetime
+    tracking_end_date: datetime
     """Start date for tracking.
 
     Should be formatted as: `"YYYY-MM-DD[T]HH:MM"`. Start date < end date, even if
     backtracking.
 
     For example:
 
     .. code-block:: yaml
 
-        track_end_date: "2021-07-15T23:00"
+        tracking_end_date: "2021-07-15T23:00"
     """
 
-    event_start_date: datetime
-    """Start date for event.
+    tagging_start_date: datetime
+    """Start date for tagging.
 
     For tracking individual (e.g. heavy precipitation) events, you can set the
-    start and end date of the event to something different than the total
-    tracking start and end date, you can also indicate the hours that you want to track.
-    The event_start_date is included in the event tracking.
+    start and end date to something different than the total tracking start and
+    end date, you can also indicate the hours that you want to track. The
+    start date is included.
 
     Should be formatted as: `"YYYY-MM-DD[T]HH:MM"`. Start date < end date, even if
     backtracking.
 
     For example:
 
     .. code-block:: yaml
 
-        event_start_date: "2021-07-13T00:00"
+        tagging_start_date: "2021-07-13T00:00"
 
     """
 
-    event_end_date: datetime
-    """Start date for event.
+    tagging_end_date: datetime
+    """End date for tagging.
 
     For tracking individual (e.g. heavy precipitation) events, you can set the
-    start and end date of the event to something different than the total
-    tracking start and end date, you can also indicate the hours that you want to track.
-    The event_end_date is included in the event tracking.
+    start and end date to something different than the total tracking start and
+    end date, you can also indicate the hours that you want to track. The
+    end date is included.
 
     Should be formatted as: `"YYYY-MM-DD[T]HH:MM"`. Start date < end date, even if
     backtracking.
 
     For example:
 
     .. code-block:: yaml
 
-        event_end_date: "2021-07-14T23:00"
+        tagging_end_date: "2021-07-14T23:00"
 
     """
 
     input_frequency: str
     """Frequency of the raw input data.
 
     Used to calculated water volumes.
@@ -226,24 +295,14 @@
 
     .. code-block:: yaml
 
         levels: [20,40,60,80,90,95,100,105,110,115,120,123,125,128,130,131,132,133,134,135,136,137]
 
     """
 
-    log_level: Literal["debug", "info", "warning", "error", "critical"]
-    """Verbosity of the output messages.
-
-    For example:
-
-    .. code-block:: yaml
-
-        log_level: info
-    """
-
     restart: bool
     """Whether to restart from previous run.
 
     If set to `true`, this will attempt to read the output from a previous model
     run and continue from there. The output from the previous timestep must be
     available for this to work.
 
@@ -274,39 +333,14 @@
 
     .. code-block:: yaml
 
         kvf: 3
 
     """
 
-    chunks: Optional[Dict[str, int]]
-    """Whether to use dask.
-
-    Using dask can help process large datasets without memory issues, but its
-    performance is quite sensitive to the chunk configuration.
-
-    Some examples:
-
-    .. code-block:: yaml
-
-        # don't use dask:
-        chunks: null
-
-        # process one time step at a time
-        chunks: {time: 1}
-
-        # set chunking for all individual dims
-        chunks:
-            level: -1
-            time: 1  # don't set time to auto, as it will be different for surface and 3d vars
-            latitude: auto
-            longitude: auto
-
-    """
-
     @classmethod
     def from_yaml(cls, config_file):
         """Read settings from a configuration.yaml file.
 
         For example:
 
         .. highlight:: python
@@ -317,34 +351,41 @@
 
         """
         with open(config_file) as f:
             settings = yaml.safe_load(f)
 
         return cls(**settings)
 
-    @field_validator("preprocessed_data_folder", "region", "output_folder")
+    @field_validator("preprocessed_data_folder", "output_folder")
     @classmethod
     def _expanduser(cls, path):
         """Resolve ~ in input paths."""
-        return path.expanduser()
+        return path.absolute()
 
     @field_validator("preprocessed_data_folder", "output_folder")
     @classmethod
     def _make_dir(cls, path):
         """Create output dirs if they don't exist yet."""
         if not path.exists():
-            print(f"Creating output folder {path}")
+            logger.info(f"Creating output folder {path}")
             path.mkdir(parents=True)
         return path
 
     @model_validator(mode="after")
     def check_date_order(self):
-        if self.track_start_date > self.track_end_date:
-            raise ValueError("track_end_date should be later than track_start_date")
-        if self.event_start_date > self.event_end_date:
-            raise ValueError("event_end_date should be later than event_start_date")
+        if self.tracking_start_date > self.tracking_end_date:
+            raise ValueError(
+                "tracking_end_date should be later than tracking_start_date"
+            )
+        if self.tagging_start_date > self.tagging_end_date:
+            raise ValueError("tagging_end_date should be later than tagging_start_date")
         if self.preprocess_start_date > self.preprocess_end_date:
             raise ValueError(
                 "preprocess_end_date should be later than preprocess_start_date"
             )
 
+        if self.tracking_domain is not None and self.periodic_boundary:
+            logger.warning(
+                "Periodic boundary set to true while using a subdomain. Are you sure?"
+            )
+
         return self
```

### Comparing `wam2layers-3.0.0b5/src/wam2layers/preprocessing/era5.py` & `wam2layers-3.0.0b6/src/wam2layers/preprocessing/era5.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,37 @@
+import logging
+from functools import lru_cache
 from pathlib import Path
 
-import click
 import numpy as np
 import pandas as pd
 import xarray as xr
-import yaml
 
-from wam2layers.analysis.checks import check_input
 from wam2layers.config import Config
 from wam2layers.preprocessing.shared import (
     accumulation_to_flux,
     calculate_humidity,
     insert_level,
     interpolate,
     sortby_ndarray,
 )
+from wam2layers.preprocessing.xarray_append import append_to_netcdf
 
+logger = logging.getLogger(__name__)
 
-def load_data(variable, date, config):
+
+@lru_cache(10)
+def log_once(logger, msg: str):
+    """Keep track of 10 different messages and then warn again.
+
+    Adapted from: https://stackoverflow.com/a/66062313"""
+    logger.info(msg)
+
+
+def load_data(variable, datetime, config):
     """Load data for given variable and date."""
     template = config.filename_template
 
     # If it's a 4d variable, we need to set the level type
     if variable in ["u", "v", "q"]:
         if config.level_type == "model_levels":
             prefix = "_ml"
@@ -29,49 +39,49 @@
             prefix = "_pl"
     # If it's a 3d variable we do not need to set the level type
     else:
         prefix = ""
 
     # Load data
     filepath = template.format(
-        year=date.year,
-        month=date.month,
-        day=date.day,
+        year=datetime.year,
+        month=datetime.month,
+        day=datetime.day,
+        hour=datetime.hour,
+        minute=datetime.minute,
         levtype=prefix,
         variable=variable,
     )
-    da = xr.open_dataset(filepath, chunks=config.chunks).sel(
-        time=date.strftime("%Y%m%d")
-    )[variable]
+    da = xr.open_dataarray(filepath).sel(time=datetime.strftime("%Y%m%d%H%M"))
 
     if "lev" in da.coords:
         da = da.rename(lev="level")
 
     # If it's 4d data we want to select a subset of the levels
     if variable in ["u", "v", "q"] and isinstance(config.levels, list):
         return da.sel(level=config.levels)
 
     return da
 
 
-def preprocess_precip_and_evap(date, config):
+def preprocess_precip_and_evap(datetime, config):
     """Load and pre-process precipitation and evaporation."""
     # All incoming units are accumulations (in m) since previous time step
-    evap = load_data("e", date, config)
-    precip = load_data("tp", date, config)  # total precipitation
+    evap = load_data("e", datetime, config)
+    precip = load_data("tp", datetime, config)  # total precipitation
 
     # Transfer negative (originally positive) values of evap to precip
     precip = np.maximum(precip, 0) + np.maximum(evap, 0)
     precip = precip
 
     # Change sign convention to all positive,
     evap = np.abs(np.minimum(evap, 0))
 
-    precip = accumulation_to_flux(precip)
-    evap = accumulation_to_flux(evap)
+    precip = accumulation_to_flux(precip, input_frequency=config.input_frequency)
+    evap = accumulation_to_flux(evap, input_frequency=config.input_frequency)
     return precip, evap
 
 
 def load_era5_ab():
     """Load a and b coefficients."""
     table = Path(__file__).parent / "tableERA5model_to_pressure.csv"
     df = pd.read_csv(table)
@@ -169,15 +179,15 @@
     u = u.assign_coords(level=np.arange(nlev))
     v = v.assign_coords(level=np.arange(nlev))
     q = q.assign_coords(level=np.arange(nlev))
     p = p.assign_coords(level=np.arange(nlev))
 
     # Calculate pressure jump
     dp = p.diff("level")
-    assert np.all(dp > 0), "Pressure levels should increase monotonically"
+    assert np.all(dp >= 0), "Pressure levels should increase monotonically"
 
     # Interpolate to midpoints
     midpoints = 0.5 * (u.level.values[1:] + u.level.values[:-1])
     dp = dp.assign_coords(level=midpoints)
     u = u.interp(level=midpoints)
     v = v.interp(level=midpoints)
     q = q.interp(level=midpoints)
@@ -194,15 +204,15 @@
 
 
 def get_input_dates(config):
     """Dates for pre-processing."""
     return pd.date_range(
         start=config.preprocess_start_date,
         end=config.preprocess_end_date,
-        freq="1d",
+        freq=config.input_frequency,
     )
 
 
 def prep_experiment(config_file):
     """Pre-process all data for a given config file.
 
     This function expects the following configuration settings:
@@ -221,53 +231,55 @@
       variable name and add _ml for model level data. E.g. with prefix =
       "FloodCase_202107" this function will be able to find
       FloodCase_202107_ml_u.nc or FloodCase_202107_u.nc and
       FloodCase_202107_sp.nc
     """
     config = Config.from_yaml(config_file)
 
-    if config.chunks is not None:
-        print("Starting dask cluster")
-        from dask.distributed import Client
-
-        client = Client()
-        print(f"To see the dask dashboard, go to {client.dashboard_link}")
-
-    for date in get_input_dates(config):
-        print(date)
+    for datetime in get_input_dates(config):
+        is_new_day = datetime == datetime.floor("1d")
+        logger.info(datetime)
 
         # 4d fields
         levels = config.levels
-        q = load_data("q", date, config)  # in kg kg-1
-        u = load_data("u", date, config)  # in m/s
-        v = load_data("v", date, config)  # in m/s
-        sp = load_data("sp", date, config)  # in Pa
+        q = load_data("q", datetime, config)  # in kg kg-1
+        u = load_data("u", datetime, config)  # in m/s
+        v = load_data("v", datetime, config)  # in m/s
+        sp = load_data("sp", datetime, config)  # in Pa
 
         if config.level_type == "model_levels":
             dp = get_dp_modellevels(sp, levels)
 
         if config.level_type == "pressure_levels":
-            d2m = load_data("d2m", date, config)  # Dew point in K
+            d2m = load_data("d2m", datetime, config)  # Dew point in K
             q2m = calculate_humidity(d2m, sp)  # kg kg-1
-            u10 = load_data("u10", date, config)  # in m/s
-            v10 = load_data("v10", date, config)  # in m/s
+            u10 = load_data("u10", datetime, config)  # in m/s
+            v10 = load_data("v10", datetime, config)  # in m/s
             dp, p, q, u, v, pb = get_dp_pressurelevels(q, u, v, sp, q2m, u10, v10)
 
         # Calculate column water vapour
         g = 9.80665  # gravitational accelleration [m/s2]
         cwv = q * dp / g  # (kg/m2)
 
         try:
             # Calculate column water instead of column water vapour
-            tcw = load_data("tcw", date, config)  # kg/m2
-            cw = (tcw / cwv.sum(dim="level")) * cwv  # column water (kg/m2)
-            # TODO: warning if cw >> cwv
+            tcw = load_data("tcw", datetime, config)  # kg/m2
+            correction = tcw / cwv.sum(dim="level")
+            cw = correction * cwv  # column water (kg/m2)
+            if is_new_day:
+                logger.info(
+                    f"Total column water correction: mean over grid for this timestep {correction.mean().item():.4f}"
+                )
+
         except FileNotFoundError:
             # Fluxes will be calculated based on the column water vapour
             cw = cwv
+            log_once(
+                logger, f"Total column water not available; using water vapour only"
+            )
 
         # Determine the fluxes
         fx = u * cw  # eastward atmospheric moisture flux (kg m-1 s-1)
         fy = v * cw  # northward atmospheric moisture flux (kg m-1 s-1)
 
         # Integrate fluxes and states to upper and lower layer
         if config.level_type == "model_levels":
@@ -290,67 +302,37 @@
 
         # Vertically integrate fluxes over two layers
         fx_lower = fx.where(lower_layer).sum(dim="level")  # kg m-1 s-1
         fy_lower = fy.where(lower_layer).sum(dim="level")  # kg m-1 s-1
         fx_upper = fx.where(upper_layer).sum(dim="level")  # kg m-1 s-1
         fy_upper = fy.where(upper_layer).sum(dim="level")  # kg m-1 s-1
 
-        precip, evap = preprocess_precip_and_evap(date, config)
+        precip, evap = preprocess_precip_and_evap(datetime, config)
 
         # Combine everything into one dataset
-        ds = xr.Dataset(
-            {
-                "fx_upper": fx_upper.assign_attrs(units="kg m-1 s-1"),
-                "fy_upper": fy_upper.assign_attrs(units="kg m-1 s-1"),
-                "fx_lower": fx_lower.assign_attrs(units="kg m-1 s-1"),
-                "fy_lower": fy_lower.assign_attrs(units="kg m-1 s-1"),
-                "s_upper": s_upper.assign_attrs(units="kg m-2"),
-                "s_lower": s_lower.assign_attrs(units="kg m-2"),
-                "evap": evap,
-                "precip": precip,
-            }
+        ds = (
+            xr.Dataset(
+                {
+                    "fx_upper": fx_upper.assign_attrs(units="kg m-1 s-1"),
+                    "fy_upper": fy_upper.assign_attrs(units="kg m-1 s-1"),
+                    "fx_lower": fx_lower.assign_attrs(units="kg m-1 s-1"),
+                    "fy_lower": fy_lower.assign_attrs(units="kg m-1 s-1"),
+                    "s_upper": s_upper.assign_attrs(units="kg m-2"),
+                    "s_lower": s_lower.assign_attrs(units="kg m-2"),
+                    "evap": evap,
+                    "precip": precip,
+                }
+            )
+            .expand_dims("time")
+            .astype("float32")
         )
 
         # Verify that the data meets all the requirements for the model
         # check_input(ds)
 
         # Save preprocessed data
-        filename = f"{date.strftime('%Y-%m-%d')}_fluxes_storages.nc"
+        filename = f"{datetime.strftime('%Y-%m-%d')}_fluxes_storages.nc"
         output_path = config.preprocessed_data_folder / filename
-        ds.astype("float32").to_netcdf(output_path)
-
-    # Close the dask cluster when done
-    if config.chunks is not None:
-        client.shutdown()
-
-
-################################################################################
-# To run this script interactively in e.g. Spyder, uncomment the following line:
-# prep_experiment("../../cases/era5_2021.yaml")
-################################################################################
-
-###########################################################################
-# The code below makes it possible to run wam2layers from the command line:
-# >>> python backtrack.py path/to/cases/era5_2021.yaml
-# or even:
-# >>> wam2layers backtrack path/to/cases/era5_2021.yaml
-###########################################################################
-
-
-@click.command()
-@click.argument("config_file", type=click.Path(exists=True))
-def cli(config_file):
-    """Preprocess ERA5 data for WAM2layers tracking experiments.
-
-    CONFIG_FILE: Path to WAM2layers experiment configuration file.
-
-    Usage examples:
-
-        \b
-        - python path/to/preprocessing/era5.py path/to/cases/era5_2021.yaml
-        - wam2layers preprocess era5 path/to/cases/era5_2021.yaml
-    """
-    prep_experiment(config_file)
-
-
-if __name__ == "__main__":
-    cli()
+        if is_new_day:
+            ds.to_netcdf(output_path, unlimited_dims=["time"], mode="w")
+        else:
+            append_to_netcdf(output_path, ds, expanding_dim="time")
```

### Comparing `wam2layers-3.0.0b5/src/wam2layers/preprocessing/tableERA5model_to_pressure.csv` & `wam2layers-3.0.0b6/src/wam2layers/preprocessing/tableERA5model_to_pressure.csv`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -132,8 +132,8 @@
 130,302.476563,0.975078,991.0230,988.8133,205.44,205.44,286.81,1.201001
 131,202.484375,0.980072,995.0824,993.0527,169.50,169.51,287.05,1.205168
 132,122.101563,0.984542,998.8081,996.9452,136.62,136.62,287.26,1.208992
 133,62.781250,0.988500,1002.2250,1000.5165,106.54,106.54,287.46,1.212498
 134,22.835938,0.991984,1005.3562,1003.7906,79.04,79.04,287.64,1.215710
 135,3.757813,0.995003,1008.2239,1006.7900,53.92,53.92,287.80,1.218650
 136,0.000000,0.997630,1010.8487,1009.5363,30.96,30.96,287.95,1.221341
-137,0.000000,1.000000,1013.2500,1012.0494,10.00,10.00,288.09,1.223803
+137,0.000000,1.000000,1013.2500,1012.0494,10.00,10.00,288.09,1.223803
```

### Comparing `wam2layers-3.0.0b5/src/wam2layers/utils/source_region.py` & `wam2layers-3.0.0b6/src/wam2layers/utils/tagging_region.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 """
-WAM-2layers Source Region Designer functions
+WAM2layers Tagging Region Designer functions
 
-@author: Vincent de Feiter (vincent.defeiter@wur.nl) | GitHub: vincentdefeiter
+@author: Vincent de Feiter | GitHub: vincentdefeiter
 
-Version 4.0 | 25-05-2023
+Adapted by Chris Weijenborg
 
 """
+import logging
 
 # Import
 import cartopy.crs as ccrs  # used for plotting on a map
 import geopandas as gpd  # reading shapefiles
 import matplotlib.patheffects as pe  # additional plotting functionalities
 import matplotlib.pyplot as plt  # used for plotting purposes
 import numpy as np  # used for array calculations
 import regionmask  # used for region mapping
 import xarray as xr  # used to read .nc files
 from cartopy import feature as cfeature
 
+logger = logging.getLogger(__name__)
 
-def mask_with_regionmask(region_source, regions, input_file, output_file, return_plot):
-    """Source region by using a named region from regionmask.
 
-    This function builds a source region based on available regions from the Region Mask Python Package.
+def mask_with_regionmask(region_source, regions, input_file, output_dir, return_plot):
+    """tagging region by using a named region from regionmask.
+
+    This function builds a tagging region based on available regions from the Region Mask Python Package.
 
     Args:
         region_source (str): indicate here a region source from the Region Mask Python Package (Giorgi, SREX, AR6, PRUDENCE).
         regions (list): single or multiple regions as list.
         reference_file: a reference file of the preprocessing which is used to
             extract the dimensions of the data used.
-        output_file: path where to store the regionmask file.
-        return_plot: if true, return a plot that shows the source region on a map.
+        output_dir: path where to store the created tagging region.
+        return_plot: if true, return a plot that shows the tagging region on a map.
 
     Returns:
         axes on which the region is plotted if `return_plot` is True
 
     """
 
     # Retrieve file dimensions
@@ -60,47 +63,59 @@
                 'region_source not specified correctly, please check the "regionmask.defined_regions" options in the Region Mask documentation for more details'
             )
 
     # create (a) mask(s) of the required region(s):
     mask = getattr(available_regions, "mask_3D")(longitude, latitude)
 
     # Specify region ID - what to store
-    region_ids = np.array(regions) - 1
+    region_ids = np.array(regions)
+
+    if (
+        "srex" in region_source
+        or "giorgi" in region_source
+        or "prudence" in region_source
+    ):
+        region_ids = region_ids - 1
+    if "ocean" in region_source or "land" in region_source:
+        raise KeyError(
+            "Entry for ar6 not recognized. Please only use the ar6.all options to make the selection. This option ensures proper indexing of the region."
+        )
+
     region_ids = region_ids.tolist()
 
     if type(region_ids) == int:
         raise KeyError(
-            "regions not specified correctly, please check whether your input is provided as a list [...,...], even if it is a single source region!"
+            "regions not specified correctly, please check whether your input is provided as a list [...,...], even if it is a single tagging region!"
         )
 
     new_masks = mask.isel(region=region_ids).values
 
-    # Make WAM2Layers fitting
+    # Make WAM2layers fitting
     new_masks = np.where(
         new_masks == False, 0, 1
     )  # Replace True and False by 1 and 0's
     new_masks = np.nanmean(new_masks, axis=0)  # Multiple masks into 1D array
 
-    # Export as source region for WAM2Layers
+    # Export as tagging region for WAM2layers
 
     # create xarray dataset
     data = new_masks
 
     export = xr.Dataset(
-        {"source_region": (["latitude", "longitude"], data.astype(float))}
+        {"tagging_region": (["latitude", "longitude"], data.astype(float))}
     )
 
     # set coordinates
     export["longitude"] = ("longitude", longitude)
     export["latitude"] = ("latitude", latitude)
 
     # save to NetCDF file
-    export.to_netcdf(output_file)
+    export.to_netcdf(output_dir)
 
-    print(f"Stored source region in {output_file}.")
+    logger.info(f"Stored tagging region in {output_dir}.")
 
     # Plot as a check
     if return_plot:
         # Visualise all regions available
 
         fontsizes = 10
         pads = 20
@@ -112,43 +127,49 @@
             fontsize=8,
         )
 
         ax = available_regions.plot(
             projection=ccrs.PlateCarree(), add_ocean=True, text_kws=text_kws
         )
 
+        plt.rcParams["figure.dpi"] = 200  # Set the DPI to 300 (adjust as needed)
+
         mask_plot = new_masks
 
-        ax.contourf(longitude, latitude, mask_plot, levels=[0.1, 1])
-        ax.set_ylim(latitude[0], latitude[-1])
-        ax.set_xlim(longitude[0], longitude[-1])
-        ax.invert_yaxis()
+        indices = export.where(export.tagging_region > 0, drop=True)
+
+        ax.contourf(
+            longitude, latitude, mask_plot, levels=[0.1, 1], zorder=5, alpha=0.8
+        )
+
+        if "prudence" in region_source:
+            ax.set_extent([-20, 40, 30, 70])
 
         # Grid
         gl = ax.gridlines(draw_labels=True, alpha=0.5, linestyle=":", color="k")
         gl.top_labels = False
         gl.right_labels = False
         gl.xlabel_style = {"size": fontsizes}
         gl.ylabel_style = {"size": fontsizes}
 
-    return ax
+        return ax
 
 
-def mask_with_shapefile(shapefile, regions, reference_file, output_file, return_plot):
-    """Mask source region using a shapefile.
+def mask_with_shapefile(shapefile, regions, reference_file, output_dir, return_plot):
+    """Mask tagging region using a shapefile.
 
-    This function builds a source region based on an existing shapefile and stores the output file.
+    This function builds a tagging region based on an existing shapefile and stores the output file.
 
     Args:
         shapefile: name of the shapefile. Include: .dbf, .prj, .sbn, .sbx, .shp, .shp.xml and .shx files in the input directory.
         regions: if build up of multiple regions, indicate as list (int), otherwise FALSE.
         reference_file: a reference file of the preprocessing which is used to
             extract the dimensions of the data used.
-        output_file: path where to store the regionmask file.
-        return_plot: if true, return a plot that shows the source region on a map.
+        output_dir: path where to store the created tagging region.
+        return_plot: if true, return a plot that shows the tagging region on a map.
 
     Returns:
         axes on which the region is plotted if 'return_plot' is True.
     """
 
     # Retrieve file dimensions
     file = xr.open_dataset(reference_file)
@@ -165,58 +186,60 @@
     # Specify region ID - what to store
     if regions != False:
         region_ids = np.array(regions)
         region_ids = region_ids.tolist()
 
         if type(region_ids) == int:
             raise KeyError(
-                "regions not specified correctly, please check whether your input is provided as a list [...,...], even if it is a single source region!"
+                "regions not specified correctly, please check whether your input is provided as a list [...,...], even if it is a single tagging region!"
             )
 
         new_masks = mask.isel(region=region_ids).values
 
-        # Make WAM2Layers fitting
+        # Make WAM2layers fitting
         new_masks = np.where(
             new_masks == False, 0, 1
         )  # Replace True and False by 1 and 0's
         new_masks = np.nanmean(new_masks, axis=0)  # Multiple masks into 1D array
     else:
         new_masks = mask.isel(region=[0]).values
 
-        # Make WAM2Layers fitting
+        # Make WAM2layers fitting
         new_masks = np.where(
             new_masks == False, 0, 1
         )  # Replace True and False by 1 and 0's
         new_masks = np.nanmean(new_masks, axis=0)  # Multiple masks into 1D array
 
-    # Export as source region for WAM2Layers
+    # Export as tagging region for WAM2layers
 
     # create xarray dataset
     data = new_masks
 
     export = xr.Dataset(
-        {"source_region": (["latitude", "longitude"], data.astype(float))}
+        {"tagging_region": (["latitude", "longitude"], data.astype(float))}
     )
 
     # set coordinates
     export["longitude"] = ("longitude", longitude)
     export["latitude"] = ("latitude", latitude)
 
     # save to NetCDF file
-    export.to_netcdf(output_file + "source_region.nc")
 
-    print(f"Stored source region in {output_file}.")
+    export.to_netcdf(output_dir)
+
+    logger.info(f"Stored tagging region in {output_dir}.")
 
     if return_plot:
         # Visualise all regions available
 
         fontsizes = 10
         pads = 20
 
-        fig = plt.figure(figsize=(16, 10))
+        # Zoomed-in
+        fig = plt.figure(figsize=(16, 10), dpi=200)
         ax = fig.add_subplot(111, projection=ccrs.PlateCarree())
 
         # Make figure
         ax.add_feature(cfeature.LAND, zorder=1, edgecolor="k", facecolor="w")
 
         ax.add_feature(cfeature.COASTLINE, zorder=2, linewidth=0.8)
         ax.add_feature(cfeature.BORDERS, zorder=2, linewidth=0.2, alpha=0.5)
@@ -228,47 +251,117 @@
             linewidth=0.8,
             edgecolor="k",
             alpha=0.5,
             facecolor="w",
         )
         mask_plot = new_masks
 
-        ax.contourf(longitude, latitude, mask_plot, levels=[0.1, 1])
-        ax.set_ylim(latitude[0], latitude[-1])
-        ax.set_xlim(longitude[0], longitude[-1])
-        ax.invert_yaxis()
+        indices = export.where(export.tagging_region > 0, drop=True)
+        lon_indices = indices.longitude
+        lon_indices_c = []
+        for i in lon_indices:
+            if i <= 180:
+                item = i * -1
+                lon_indices_c.append(item)
+            else:
+                lon_indices_c.append(i)
+
+        ax.contourf(
+            longitude, latitude, mask_plot, levels=[0.1, 1], zorder=5, alpha=0.8
+        )
+        ax.set_extent(
+            [
+                min(lon_indices_c) - 1,
+                max(lon_indices_c) + 1,
+                indices.latitude.min() - 1,
+                indices.latitude.max() + 1,
+            ]
+        )
+        ax.set_title("Zoomed-in", fontsize=fontsizes)
 
         # Grid
         gl = ax.gridlines(draw_labels=True, alpha=0.5, linestyle=":", color="k")
         gl.top_labels = False
         gl.right_labels = False
-        gl.xlabel_style = {"size": fontsizes}
-        gl.ylabel_style = {"size": fontsizes}
-        return ax
+        gl.xlabel_style = {"size": fontsizes * 2}
+        gl.ylabel_style = {"size": fontsizes * 2}
+
+        # Zoomed-out
+        fig = plt.figure(figsize=(16, 10), dpi=200)
+        ax2 = fig.add_subplot(111, projection=ccrs.PlateCarree())
+
+        # Make figure
+        ax2.add_feature(cfeature.LAND, zorder=1, edgecolor="k", facecolor="w")
+
+        ax2.add_feature(cfeature.COASTLINE, zorder=2, linewidth=0.8)
+        ax2.add_feature(cfeature.BORDERS, zorder=2, linewidth=0.2, alpha=0.5)
+        ax2.add_feature(cfeature.RIVERS, zorder=2, linewidth=3, alpha=0.5)
+        ax2.add_feature(cfeature.STATES, zorder=2, facecolor="w")
+        ax2.add_feature(
+            cfeature.LAKES,
+            zorder=2,
+            linewidth=0.8,
+            edgecolor="k",
+            alpha=0.5,
+            facecolor="w",
+        )
+        mask_plot = new_masks
+
+        indices = export.where(export.tagging_region > 0, drop=True)
+        lon_indices = indices.longitude
+        lon_indices_c = []
+        for i in lon_indices:
+            if i <= 180:
+                item = i * -1
+                lon_indices_c.append(item)
+            else:
+                lon_indices_c.append(i)
+
+        ax2.contourf(
+            longitude, latitude, mask_plot, levels=[0.1, 1], zorder=5, alpha=0.8
+        )
+        ax2.set_extent(
+            [
+                min(lon_indices_c) - 20,
+                max(lon_indices_c) + 20,
+                indices.latitude.min() - 20,
+                indices.latitude.max() + 20,
+            ]
+        )
+        ax2.set_title("Zoomed-out", fontsize=fontsizes)
+
+        # Grid
+        gl = ax2.gridlines(draw_labels=True, alpha=0.5, linestyle=":", color="k")
+        gl.top_labels = False
+        gl.right_labels = False
+        gl.xlabel_style = {"size": fontsizes * 2}
+        gl.ylabel_style = {"size": fontsizes * 2}
+
+        return ax, ax2
 
 
 def mask_around_point(
     centerpoint,
     radius,
     reference_file,
-    output_file="source_region.nc",
-    return_plot=False,
+    output_dir,
+    return_plot,
 ):
-    """Mask source region using a center point with a given radius.
+    """Mask tagging region using a center point with a given radius.
 
-    This function builds a square source region based on given coordinates and
+    This function builds a square tagging region based on given coordinates and
     radius and stores it the output file.
 
     Args:
         centerpoint: Coordinates of the central point (latitude, longitude).
         radius (int): distance from center to edges of square box in degrees.
         reference_file: a reference file of the preprocessing which is used to
             extract the dimensions of the data used.
-        output_file: path where to store the regionmask file.
-        return_plot: if true, return a plot that shows the source region on a map.
+        output_dir: path where to store the created tagging region.
+        return_plot: if true, return a plot that shows the tagging region on a map.
 
     Returns:
         axes on which the region is plotted if `return_plot' is True
     """
 
     # Retrieve file dimensions
     file = xr.open_dataset(reference_file)
@@ -285,39 +378,170 @@
     # Set the square region of value 1 in the mask
     mask = (np.abs(latitude - center_lat) <= radius) & (
         np.abs(longitude - center_lon) <= radius
     )
 
     new_masks = np.where(mask == False, 0, 1)  # Replace True and False by 1 and 0's
 
-    # Export as source region for WAM2Layers
+    # Export as tagging region for WAM2layers
 
     # create xarray dataset
     data = new_masks
 
     export = xr.Dataset(
-        {"source_region": (["latitude", "longitude"], data.astype(float))}
+        {"tagging_region": (["latitude", "longitude"], data.astype(float))}
     )
 
     # set coordinates
     export["longitude"] = ("longitude", longitude_r)
     export["latitude"] = ("latitude", latitude_r)
 
     # save to NetCDF file
+    export.to_netcdf(output_dir)
+
+    logger.info(f"Stored tagging region in {output_dir}.")
+
+    if return_plot:
+        # Visualise all regions available
+
+        fontsizes = 10
+        pads = 20
+
+        fig = plt.figure(figsize=(16, 10), dpi=200)
+        ax = fig.add_subplot(111, projection=ccrs.PlateCarree())
+
+        # Make figure
+        ax.add_feature(cfeature.LAND, zorder=1, edgecolor="k", facecolor="w")
+
+        ax.add_feature(cfeature.COASTLINE, zorder=2, linewidth=0.8)
+        ax.add_feature(cfeature.BORDERS, zorder=2, linewidth=0.2, alpha=0.5)
+        ax.add_feature(cfeature.RIVERS, zorder=2, linewidth=3, alpha=0.5)
+        ax.add_feature(cfeature.STATES, zorder=2, facecolor="w")
+        ax.add_feature(
+            cfeature.LAKES,
+            zorder=2,
+            linewidth=0.8,
+            edgecolor="k",
+            alpha=0.5,
+            facecolor="w",
+        )
+        mask_plot = new_masks
+
+        ax.contourf(longitude_r, latitude_r, mask_plot, levels=[0.1, 1])
+
+        indices = export.where(export.tagging_region > 0, drop=True)
+        ax.contourf(
+            longitude, latitude, mask_plot, levels=[0.1, 1], zorder=5, alpha=0.8
+        )
+        ax.set_extent(
+            [
+                indices.longitude.min() - 10,
+                indices.longitude.max() + 10,
+                indices.latitude.min() - 10,
+                indices.latitude.max() + 10,
+            ]
+        )
+
+        ax.plot(
+            center_lon,
+            center_lat,
+            marker="o",
+            markerfacecolor="r",
+            markeredgecolor="k",
+            linestyle="None",
+            markersize=radius * 0.5,
+            zorder=6,
+        )
+
+        # Grid
+        gl = ax.gridlines(draw_labels=True, alpha=0.5, linestyle=":", color="k")
+        gl.top_labels = False
+        gl.right_labels = False
+        gl.xlabel_style = {"size": fontsizes * 2}
+        gl.ylabel_style = {"size": fontsizes * 2}
+        return ax
+
+
+def mask_around_track(
+    centerpoints,
+    times,
+    radius,
+    reference_file,
+    output_file,
+    return_plot,
+):
+    """Mask tagging region using a track of center points with a given radius (currently in degrees).
+
+    This function builds a square source region based on given coordinates and
+    radius and stores it the output file.
+
+    Args:
+        centerpoints: List of coordinates of the central points, changing over time [(lat1, lon1), ....,lat_final, lon_final)] .
+        radius (int): distance from center to edges of square box in degrees.
+        reference_file: a reference file of the preprocessing which is used to
+            extract the dimensions of the data used.
+        output_file: path where to store the created source region.
+        return_plot: if true, return a plot that shows the source region on a map.
+
+    Returns:
+        axes on which the region is plotted if `return_plot' is True
+    """
+
+    # Retrieve file dimensions
+    file = xr.open_dataset(reference_file)
+
+    longitude_r = np.array(file.longitude)
+    latitude_r = np.array(file.latitude)
+
+    # Create a grid of latitudes and longitudes
+    longitude, latitude = np.meshgrid(longitude_r, latitude_r)
+
+    # Initiate result array
+    new_masks = np.zeros((len(centerpoints), len(latitude_r), len(longitude_r)))
+
+    # loop over times
+    for t in range(len(centerpoints)):
+        centerpoint = centerpoints[t]
+        # retrieve latitude and longitude from ceterpoint
+        center_lat, center_lon = centerpoint
+
+        # Set the square region of value 1 in the mask
+        mask = (np.abs(latitude - center_lat) <= radius) & (
+            np.abs(longitude - center_lon) <= radius
+        )
+
+        new_masks[t, ::] = np.where(
+            mask == False, 0, 1
+        )  # Replace True and False by 1 and 0's
+
+    # Export as source region for WAM2layers
+    # create xarray dataset
+    data = new_masks
+
+    export = xr.Dataset(
+        {"source_region": (["time", "latitude", "longitude"], data.astype(float))}
+    )
+
+    # set coordinates
+    export["longitude"] = ("longitude", longitude_r)
+    export["latitude"] = ("latitude", latitude_r)
+    export["time"] = ("time", times)
+
+    # save to NetCDF file
     export.to_netcdf(output_file)
 
-    print(f"Stored source region in {output_file}.")
+    logger.info(f"Stored source region in {output_file}.")
 
     if return_plot:
         # Visualise all regions available
 
         fontsizes = 10
         pads = 20
 
-        fig = plt.figure(figsize=(16, 10))
+        fig = plt.figure(figsize=(16, 10), dpi=200)
         ax = fig.add_subplot(111, projection=ccrs.PlateCarree())
 
         # Make figure
         ax.add_feature(cfeature.LAND, zorder=1, edgecolor="k", facecolor="w")
 
         ax.add_feature(cfeature.COASTLINE, zorder=2, linewidth=0.8)
         ax.add_feature(cfeature.BORDERS, zorder=2, linewidth=0.2, alpha=0.5)
@@ -330,28 +554,39 @@
             edgecolor="k",
             alpha=0.5,
             facecolor="w",
         )
         mask_plot = new_masks
 
         ax.contourf(longitude_r, latitude_r, mask_plot, levels=[0.1, 1])
-        ax.set_ylim(latitude_r[0], latitude_r[-1])
-        ax.set_xlim(longitude_r[0], longitude_r[-1])
-        ax.invert_yaxis()
+
+        indices = export.where(export.source_region == 1, drop=True)
+        ax.contourf(
+            longitude, latitude, mask_plot, levels=[0.1, 1], zorder=5, alpha=0.8
+        )
+        ax.set_extent(
+            [
+                indices.longitude.min() - 10,
+                indices.longitude.max() + 10,
+                indices.latitude.min() - 10,
+                indices.latitude.max() + 10,
+            ]
+        )
 
         ax.plot(
             center_lon,
             center_lat,
             marker="o",
             markerfacecolor="r",
             markeredgecolor="k",
             linestyle="None",
             markersize=radius * 0.5,
+            zorder=6,
         )
 
         # Grid
         gl = ax.gridlines(draw_labels=True, alpha=0.5, linestyle=":", color="k")
         gl.top_labels = False
         gl.right_labels = False
-        gl.xlabel_style = {"size": fontsizes}
-        gl.ylabel_style = {"size": fontsizes}
+        gl.xlabel_style = {"size": fontsizes * 2}
+        gl.ylabel_style = {"size": fontsizes * 2}
         return ax
```

### Comparing `wam2layers-3.0.0b5/src/wam2layers.egg-info/SOURCES.txt` & `wam2layers-3.0.0b6/src/wam2layers.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 LICENSE
 README.md
 pyproject.toml
 src/wam2layers/__init__.py
 src/wam2layers/cli.py
 src/wam2layers/config.py
+src/wam2layers/grid.py
 src/wam2layers.egg-info/PKG-INFO
 src/wam2layers.egg-info/SOURCES.txt
 src/wam2layers.egg-info/dependency_links.txt
 src/wam2layers.egg-info/entry_points.txt
 src/wam2layers.egg-info/requires.txt
 src/wam2layers.egg-info/top_level.txt
 src/wam2layers/analysis/__init__.py
 src/wam2layers/analysis/checks.py
 src/wam2layers/analysis/visualization.py
 src/wam2layers/preprocessing/__init__.py
-src/wam2layers/preprocessing/cli.py
 src/wam2layers/preprocessing/era5.py
 src/wam2layers/preprocessing/shared.py
+src/wam2layers/preprocessing/sum.py
 src/wam2layers/preprocessing/tableERA5model_to_pressure.csv
+src/wam2layers/preprocessing/xarray_append.py
 src/wam2layers/tracking/__init__.py
 src/wam2layers/tracking/backtrack.py
+src/wam2layers/tracking/core.py
+src/wam2layers/tracking/forwardtrack.py
+src/wam2layers/tracking/io.py
+src/wam2layers/tracking/shared.py
 src/wam2layers/utils/__init__.py
+src/wam2layers/utils/grids.py
 src/wam2layers/utils/profiling.py
-src/wam2layers/utils/source_region.py
-tests/test_config.py
+src/wam2layers/utils/tagging_region.py
+tests/test_config.py
+tests/test_io.py
+tests/test_workflow.py
```

