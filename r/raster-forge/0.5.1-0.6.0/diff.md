# Comparing `tmp/raster-forge-0.5.1.tar.gz` & `tmp/raster-forge-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raster-forge-0.5.1.tar", last modified: Tue Feb 20 10:59:20 2024, max compression
+gzip compressed data, was "raster-forge-0.6.0.tar", last modified: Fri Apr  5 11:00:14 2024, max compression
```

## Comparing `raster-forge-0.5.1.tar` & `raster-forge-0.6.0.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:59:20.294030 raster-forge-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-20 10:59:14.000000 raster-forge-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-02-20 10:59:20.294030 raster-forge-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-02-20 10:59:14.000000 raster-forge-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-02-20 10:59:14.000000 raster-forge-0.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:59:20.290030 raster-forge-0.5.1/raster_forge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-02-20 10:59:20.000000 raster-forge-0.5.1/raster_forge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-02-20 10:59:20.000000 raster-forge-0.5.1/raster_forge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 10:59:20.000000 raster-forge-0.5.1/raster_forge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-20 10:59:20.000000 raster-forge-0.5.1/raster_forge.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-20 10:59:20.000000 raster-forge-0.5.1/raster_forge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-20 10:59:20.000000 raster-forge-0.5.1/raster_forge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:59:20.286029 raster-forge-0.5.1/rforge/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:59:20.286029 raster-forge-0.5.1/rforge/containers/
--rw-r--r--   0 runner    (1001) docker     (127)    12842 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/containers/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/containers/raster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:59:20.286029 raster-forge-0.5.1/rforge/gui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:59:20.286029 raster-forge-0.5.1/rforge/gui/common/
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/gui/common/adaptative_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/gui/common/layer_information.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/gui/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/gui/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:59:20.286029 raster-forge-0.5.1/rforge/gui/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/gui/layers/import_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/gui/layers/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/gui/main_window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:59:20.286029 raster-forge-0.5.1/rforge/gui/processes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:59:20.290030 raster-forge-0.5.1/rforge/gui/processes/panels/
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/gui/processes/panels/composites.py
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/gui/processes/panels/distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/gui/processes/panels/fuel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/gui/processes/panels/height.py
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/gui/processes/panels/indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/gui/processes/panels/topography.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/gui/processes/process_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/gui/processes/processes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:59:20.290030 raster-forge-0.5.1/rforge/gui/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    28480 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/gui/resources/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:59:20.290030 raster-forge-0.5.1/rforge/gui/viewer/
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/gui/viewer/save_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)    14089 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/gui/viewer/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:59:20.290030 raster-forge-0.5.1/rforge/processes/
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/processes/composite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/processes/distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/processes/fuel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/processes/height.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/processes/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/processes/topography.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:59:20.290030 raster-forge-0.5.1/rforge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/tools/data_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/tools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-02-20 10:59:14.000000 raster-forge-0.5.1/rforge/tools/rescale_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 10:59:20.294030 raster-forge-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.821838 raster-forge-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-05 11:00:09.000000 raster-forge-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-05 11:00:14.821838 raster-forge-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-05 11:00:09.000000 raster-forge-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-05 11:00:09.000000 raster-forge-0.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.821838 raster-forge-0.6.0/raster_forge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-05 11:00:14.000000 raster-forge-0.6.0/raster_forge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-05 11:00:14.000000 raster-forge-0.6.0/raster_forge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 11:00:14.000000 raster-forge-0.6.0/raster_forge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 11:00:14.000000 raster-forge-0.6.0/raster_forge.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-05 11:00:14.000000 raster-forge-0.6.0/raster_forge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 11:00:14.000000 raster-forge-0.6.0/raster_forge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.817838 raster-forge-0.6.0/rforge/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.817838 raster-forge-0.6.0/rforge/gui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.817838 raster-forge-0.6.0/rforge/gui/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/common/adaptative_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/common/layer_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.817838 raster-forge-0.6.0/rforge/gui/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     9412 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/layers/import_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/layers/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/main_window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.817838 raster-forge-0.6.0/rforge/gui/processes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.817838 raster-forge-0.6.0/rforge/gui/processes/panels/
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/processes/panels/composites.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/processes/panels/distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/processes/panels/fuel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/processes/panels/height.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/processes/panels/indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/processes/panels/topography.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/processes/process_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/processes/processes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.817838 raster-forge-0.6.0/rforge/gui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    28480 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/resources/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.817838 raster-forge-0.6.0/rforge/gui/viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/viewer/save_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14089 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/gui/viewer/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.813838 raster-forge-0.6.0/rforge/library/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.817838 raster-forge-0.6.0/rforge/library/containers/
+-rw-r--r--   0 runner    (1001) docker     (127)    14726 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/library/containers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/library/containers/raster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.821838 raster-forge-0.6.0/rforge/library/processes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/library/processes/composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/library/processes/distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/library/processes/fuel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/library/processes/height.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/library/processes/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/library/processes/topography.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:00:14.821838 raster-forge-0.6.0/rforge/library/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/library/tools/data_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/library/tools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-05 11:00:09.000000 raster-forge-0.6.0/rforge/library/tools/rescale_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 11:00:14.821838 raster-forge-0.6.0/setup.cfg
```

### Comparing `raster-forge-0.5.1/LICENSE` & `raster-forge-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `raster-forge-0.5.1/PKG-INFO` & `raster-forge-0.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: raster-forge
-Version: 0.5.1
+Version: 0.6.0
 Summary: Raster Forge is an package for the manipulation of raster data. It includes a library and a graphical user interface (GUI) application.
 Author-email: Afonso Oliveira <afe.oliveira@campus.fct.unl.pt>
 License: MIT
 Keywords: raster, gui
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: PySide6
 Requires-Dist: numpy
 Requires-Dist: rasterio
 Requires-Dist: spyndex
 Requires-Dist: opencv-python
-Requires-Dist: matplotlib
+Requires-Dist: dask[dataframe]
+Provides-Extra: gui
+Requires-Dist: matplotlib; extra == "gui"
+Requires-Dist: PySide6; extra == "gui"
 Provides-Extra: devel
 Requires-Dist: black; extra == "devel"
 Requires-Dist: coverage; extra == "devel"
 Requires-Dist: flake8; extra == "devel"
 Requires-Dist: flake8-black; extra == "devel"
 Requires-Dist: flake8-builtins; extra == "devel"
 Requires-Dist: flake8-bugbear; extra == "devel"
@@ -25,14 +27,17 @@
 Requires-Dist: flake8-isort; extra == "devel"
 Requires-Dist: Flake8-pyproject; extra == "devel"
 Requires-Dist: isort; extra == "devel"
 Requires-Dist: pre-commit; extra == "devel"
 Requires-Dist: pytest>=7.0.0; extra == "devel"
 Requires-Dist: pytest-cov; extra == "devel"
 Requires-Dist: pytest-qt; extra == "devel"
+Requires-Dist: Sphinx; extra == "devel"
+Requires-Dist: sphinx-design; extra == "devel"
+Requires-Dist: pydata-sphinx-theme; extra == "devel"
 
 <p align="center">
   <a href="https://github.com/afe-oliveira/raster-forge"><img src="https://raw.githubusercontent.com/afe-oliveira/raster-forge/main/docs/_static/raster-forge.png" alt="spyndex"></a>
 </p>
 
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/afe-oliveira/raster-forge/test.yml?style=flat&logo=Github&label=Tests&labelColor=%23dbad3e&color=%235A5A5A)
 ![Codecov](https://img.shields.io/codecov/c/github/afe-oliveira/raster-forge?style=flat&logo=Codecov&logoColor=%23ffffff&label=Codecov&labelColor=%23dbad3e&color=%235A5A5A)
@@ -42,15 +47,15 @@
 
 ---
 
 Raster Forge is a Python library with an intuitive graphical user interface (GUI), designed for raster data manipulation.
 
 - **GitHub:** https://github.com/afe-oliveira/raster-forge
 - **PyPI:** https://pypi.org/project/raster-forge/
-- **Documentation:** [PLACEHOLDER]
+- **Documentation:** https://afe-oliveira.github.io/raster-forge/
 
 ---
 
 ## Instalation
 
 To install the package, use the following **_pip_** command:
 ```bash
```

#### html2text {}

```diff
@@ -1,34 +1,37 @@
-Metadata-Version: 2.1 Name: raster-forge Version: 0.5.1 Summary: Raster Forge
+Metadata-Version: 2.1 Name: raster-forge Version: 0.6.0 Summary: Raster Forge
 is an package for the manipulation of raster data. It includes a library and a
 graphical user interface (GUI) application. Author-email: Afonso Oliveira
 campus.fct.unl.pt> License: MIT Keywords: raster, gui Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-PySide6 Requires-Dist: numpy Requires-Dist: rasterio Requires-Dist: spyndex
-Requires-Dist: opencv-python Requires-Dist: matplotlib Provides-Extra: devel
-Requires-Dist: black; extra == "devel" Requires-Dist: coverage; extra ==
-"devel" Requires-Dist: flake8; extra == "devel" Requires-Dist: flake8-black;
-extra == "devel" Requires-Dist: flake8-builtins; extra == "devel" Requires-
-Dist: flake8-bugbear; extra == "devel" Requires-Dist: flake8-docstrings; extra
-== "devel" Requires-Dist: flake8-isort; extra == "devel" Requires-Dist: Flake8-
-pyproject; extra == "devel" Requires-Dist: isort; extra == "devel" Requires-
-Dist: pre-commit; extra == "devel" Requires-Dist: pytest>=7.0.0; extra ==
-"devel" Requires-Dist: pytest-cov; extra == "devel" Requires-Dist: pytest-qt;
-extra == "devel"
+numpy Requires-Dist: rasterio Requires-Dist: spyndex Requires-Dist: opencv-
+python Requires-Dist: dask[dataframe] Provides-Extra: gui Requires-Dist:
+matplotlib; extra == "gui" Requires-Dist: PySide6; extra == "gui" Provides-
+Extra: devel Requires-Dist: black; extra == "devel" Requires-Dist: coverage;
+extra == "devel" Requires-Dist: flake8; extra == "devel" Requires-Dist: flake8-
+black; extra == "devel" Requires-Dist: flake8-builtins; extra == "devel"
+Requires-Dist: flake8-bugbear; extra == "devel" Requires-Dist: flake8-
+docstrings; extra == "devel" Requires-Dist: flake8-isort; extra == "devel"
+Requires-Dist: Flake8-pyproject; extra == "devel" Requires-Dist: isort; extra
+== "devel" Requires-Dist: pre-commit; extra == "devel" Requires-Dist:
+pytest>=7.0.0; extra == "devel" Requires-Dist: pytest-cov; extra == "devel"
+Requires-Dist: pytest-qt; extra == "devel" Requires-Dist: Sphinx; extra ==
+"devel" Requires-Dist: sphinx-design; extra == "devel" Requires-Dist: pydata-
+sphinx-theme; extra == "devel"
                                    _[_s_p_y_n_d_e_x_]
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/
 workflow/status/afe-oliveira/raster-forge/
 test.yml?style=flat&logo=Github&label=Tests&labelColor=%23dbad3e&color=%235A5A5A)
 ![Codecov](https://img.shields.io/codecov/c/github/afe-oliveira/raster-
 forge?style=flat&logo=Codecov&logoColor=%23ffffff&label=Codecov&labelColor=%23dbad3e&color=%235A5A5A)
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/
 workflow/status/afe-oliveira/raster-forge/
 docs.yml?style=flat&logo=Github&label=Documentation&labelColor=%23dbad3e&color=%235A5A5A)
 ![GitHub License](https://img.shields.io/github/license/afe-oliveira/raster-
 forge?style=flat&label=License&labelColor=%23405853&color=%235A5A5A) --- Raster
 Forge is a Python library with an intuitive graphical user interface (GUI),
 designed for raster data manipulation. - **GitHub:** https://github.com/afe-
 oliveira/raster-forge - **PyPI:** https://pypi.org/project/raster-forge/ -
-**Documentation:** [PLACEHOLDER] --- ## Instalation To install the package, use
-the following **_pip_** command: ```bash pip install raster-forge ``` ##
-Library ## Graphical User Interface (GUI) To launch the GUI, execute the
-following command: ```bash rforge ```
+**Documentation:** https://afe-oliveira.github.io/raster-forge/ --- ##
+Instalation To install the package, use the following **_pip_** command:
+```bash pip install raster-forge ``` ## Library ## Graphical User Interface
+(GUI) To launch the GUI, execute the following command: ```bash rforge ```
```

### Comparing `raster-forge-0.5.1/README.md` & `raster-forge-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 ---
 
 Raster Forge is a Python library with an intuitive graphical user interface (GUI), designed for raster data manipulation.
 
 - **GitHub:** https://github.com/afe-oliveira/raster-forge
 - **PyPI:** https://pypi.org/project/raster-forge/
-- **Documentation:** [PLACEHOLDER]
+- **Documentation:** https://afe-oliveira.github.io/raster-forge/
 
 ---
 
 ## Instalation
 
 To install the package, use the following **_pip_** command:
 ```bash
```

#### html2text {}

```diff
@@ -8,11 +8,11 @@
 workflow/status/afe-oliveira/raster-forge/
 docs.yml?style=flat&logo=Github&label=Documentation&labelColor=%23dbad3e&color=%235A5A5A)
 ![GitHub License](https://img.shields.io/github/license/afe-oliveira/raster-
 forge?style=flat&label=License&labelColor=%23405853&color=%235A5A5A) --- Raster
 Forge is a Python library with an intuitive graphical user interface (GUI),
 designed for raster data manipulation. - **GitHub:** https://github.com/afe-
 oliveira/raster-forge - **PyPI:** https://pypi.org/project/raster-forge/ -
-**Documentation:** [PLACEHOLDER] --- ## Instalation To install the package, use
-the following **_pip_** command: ```bash pip install raster-forge ``` ##
-Library ## Graphical User Interface (GUI) To launch the GUI, execute the
-following command: ```bash rforge ```
+**Documentation:** https://afe-oliveira.github.io/raster-forge/ --- ##
+Instalation To install the package, use the following **_pip_** command:
+```bash pip install raster-forge ``` ## Library ## Graphical User Interface
+(GUI) To launch the GUI, execute the following command: ```bash rforge ```
```

### Comparing `raster-forge-0.5.1/pyproject.toml` & `raster-forge-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "raster-forge"
-version = "0.5.1"
+version = "0.6.0"
 description = "Raster Forge is an package for the manipulation of raster data. It includes a library and a graphical user interface (GUI) application."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["raster, gui"]
 license = {text = "MIT"}
 authors = [ { name = "Afonso Oliveira", email = "afe.oliveira@campus.fct.unl.pt" } ]
 dependencies = [
-    "PySide6",
     "numpy",
     "rasterio",
     "spyndex",
     "opencv-python",
-    "matplotlib",
+    "dask[dataframe]",
 ]
 
 [project.optional-dependencies]
+gui = [
+    "matplotlib",
+    "PySide6",
+]
+
 devel = [
     "black",
     "coverage",
     "flake8",
     "flake8-black",
     "flake8-builtins",
     "flake8-bugbear",
@@ -32,26 +36,29 @@
     "flake8-isort",
     "Flake8-pyproject",
     "isort",
     "pre-commit",
     "pytest >= 7.0.0",
     "pytest-cov",
     "pytest-qt",
+    "Sphinx",
+    "sphinx-design",
+    "pydata-sphinx-theme"
 ]
 
 [project.gui-scripts]
 rforge = "rforge.gui.gui:gui"
 
 [tool.black]
 line-length = 88
 target-version = ['py38']
 
 [tool.isort]
 profile = "black"
-src_paths = ["raster-forge", "tests"]
+src_paths = ["rforge", "tests"]
 line_length = 88
 skip_gitignore = "True"
 
 [tool.flake8]
 max-line-length = 88
 max-doc-length = 88
 ignore = [
```

### Comparing `raster-forge-0.5.1/raster_forge.egg-info/PKG-INFO` & `raster-forge-0.6.0/raster_forge.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: raster-forge
-Version: 0.5.1
+Version: 0.6.0
 Summary: Raster Forge is an package for the manipulation of raster data. It includes a library and a graphical user interface (GUI) application.
 Author-email: Afonso Oliveira <afe.oliveira@campus.fct.unl.pt>
 License: MIT
 Keywords: raster, gui
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: PySide6
 Requires-Dist: numpy
 Requires-Dist: rasterio
 Requires-Dist: spyndex
 Requires-Dist: opencv-python
-Requires-Dist: matplotlib
+Requires-Dist: dask[dataframe]
+Provides-Extra: gui
+Requires-Dist: matplotlib; extra == "gui"
+Requires-Dist: PySide6; extra == "gui"
 Provides-Extra: devel
 Requires-Dist: black; extra == "devel"
 Requires-Dist: coverage; extra == "devel"
 Requires-Dist: flake8; extra == "devel"
 Requires-Dist: flake8-black; extra == "devel"
 Requires-Dist: flake8-builtins; extra == "devel"
 Requires-Dist: flake8-bugbear; extra == "devel"
@@ -25,14 +27,17 @@
 Requires-Dist: flake8-isort; extra == "devel"
 Requires-Dist: Flake8-pyproject; extra == "devel"
 Requires-Dist: isort; extra == "devel"
 Requires-Dist: pre-commit; extra == "devel"
 Requires-Dist: pytest>=7.0.0; extra == "devel"
 Requires-Dist: pytest-cov; extra == "devel"
 Requires-Dist: pytest-qt; extra == "devel"
+Requires-Dist: Sphinx; extra == "devel"
+Requires-Dist: sphinx-design; extra == "devel"
+Requires-Dist: pydata-sphinx-theme; extra == "devel"
 
 <p align="center">
   <a href="https://github.com/afe-oliveira/raster-forge"><img src="https://raw.githubusercontent.com/afe-oliveira/raster-forge/main/docs/_static/raster-forge.png" alt="spyndex"></a>
 </p>
 
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/afe-oliveira/raster-forge/test.yml?style=flat&logo=Github&label=Tests&labelColor=%23dbad3e&color=%235A5A5A)
 ![Codecov](https://img.shields.io/codecov/c/github/afe-oliveira/raster-forge?style=flat&logo=Codecov&logoColor=%23ffffff&label=Codecov&labelColor=%23dbad3e&color=%235A5A5A)
@@ -42,15 +47,15 @@
 
 ---
 
 Raster Forge is a Python library with an intuitive graphical user interface (GUI), designed for raster data manipulation.
 
 - **GitHub:** https://github.com/afe-oliveira/raster-forge
 - **PyPI:** https://pypi.org/project/raster-forge/
-- **Documentation:** [PLACEHOLDER]
+- **Documentation:** https://afe-oliveira.github.io/raster-forge/
 
 ---
 
 ## Instalation
 
 To install the package, use the following **_pip_** command:
 ```bash
```

#### html2text {}

```diff
@@ -1,34 +1,37 @@
-Metadata-Version: 2.1 Name: raster-forge Version: 0.5.1 Summary: Raster Forge
+Metadata-Version: 2.1 Name: raster-forge Version: 0.6.0 Summary: Raster Forge
 is an package for the manipulation of raster data. It includes a library and a
 graphical user interface (GUI) application. Author-email: Afonso Oliveira
 campus.fct.unl.pt> License: MIT Keywords: raster, gui Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-PySide6 Requires-Dist: numpy Requires-Dist: rasterio Requires-Dist: spyndex
-Requires-Dist: opencv-python Requires-Dist: matplotlib Provides-Extra: devel
-Requires-Dist: black; extra == "devel" Requires-Dist: coverage; extra ==
-"devel" Requires-Dist: flake8; extra == "devel" Requires-Dist: flake8-black;
-extra == "devel" Requires-Dist: flake8-builtins; extra == "devel" Requires-
-Dist: flake8-bugbear; extra == "devel" Requires-Dist: flake8-docstrings; extra
-== "devel" Requires-Dist: flake8-isort; extra == "devel" Requires-Dist: Flake8-
-pyproject; extra == "devel" Requires-Dist: isort; extra == "devel" Requires-
-Dist: pre-commit; extra == "devel" Requires-Dist: pytest>=7.0.0; extra ==
-"devel" Requires-Dist: pytest-cov; extra == "devel" Requires-Dist: pytest-qt;
-extra == "devel"
+numpy Requires-Dist: rasterio Requires-Dist: spyndex Requires-Dist: opencv-
+python Requires-Dist: dask[dataframe] Provides-Extra: gui Requires-Dist:
+matplotlib; extra == "gui" Requires-Dist: PySide6; extra == "gui" Provides-
+Extra: devel Requires-Dist: black; extra == "devel" Requires-Dist: coverage;
+extra == "devel" Requires-Dist: flake8; extra == "devel" Requires-Dist: flake8-
+black; extra == "devel" Requires-Dist: flake8-builtins; extra == "devel"
+Requires-Dist: flake8-bugbear; extra == "devel" Requires-Dist: flake8-
+docstrings; extra == "devel" Requires-Dist: flake8-isort; extra == "devel"
+Requires-Dist: Flake8-pyproject; extra == "devel" Requires-Dist: isort; extra
+== "devel" Requires-Dist: pre-commit; extra == "devel" Requires-Dist:
+pytest>=7.0.0; extra == "devel" Requires-Dist: pytest-cov; extra == "devel"
+Requires-Dist: pytest-qt; extra == "devel" Requires-Dist: Sphinx; extra ==
+"devel" Requires-Dist: sphinx-design; extra == "devel" Requires-Dist: pydata-
+sphinx-theme; extra == "devel"
                                    _[_s_p_y_n_d_e_x_]
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/
 workflow/status/afe-oliveira/raster-forge/
 test.yml?style=flat&logo=Github&label=Tests&labelColor=%23dbad3e&color=%235A5A5A)
 ![Codecov](https://img.shields.io/codecov/c/github/afe-oliveira/raster-
 forge?style=flat&logo=Codecov&logoColor=%23ffffff&label=Codecov&labelColor=%23dbad3e&color=%235A5A5A)
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/
 workflow/status/afe-oliveira/raster-forge/
 docs.yml?style=flat&logo=Github&label=Documentation&labelColor=%23dbad3e&color=%235A5A5A)
 ![GitHub License](https://img.shields.io/github/license/afe-oliveira/raster-
 forge?style=flat&label=License&labelColor=%23405853&color=%235A5A5A) --- Raster
 Forge is a Python library with an intuitive graphical user interface (GUI),
 designed for raster data manipulation. - **GitHub:** https://github.com/afe-
 oliveira/raster-forge - **PyPI:** https://pypi.org/project/raster-forge/ -
-**Documentation:** [PLACEHOLDER] --- ## Instalation To install the package, use
-the following **_pip_** command: ```bash pip install raster-forge ``` ##
-Library ## Graphical User Interface (GUI) To launch the GUI, execute the
-following command: ```bash rforge ```
+**Documentation:** https://afe-oliveira.github.io/raster-forge/ --- ##
+Instalation To install the package, use the following **_pip_** command:
+```bash pip install raster-forge ``` ## Library ## Graphical User Interface
+(GUI) To launch the GUI, execute the following command: ```bash rforge ```
```

### Comparing `raster-forge-0.5.1/rforge/containers/layer.py` & `raster-forge-0.6.0/rforge/library/containers/layer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import rasterio
-from rforge.tools.exceptions import Errors
-from rforge.tools.rescale_dataset import _rescale_dataset
+from rforge.library.tools.exceptions import Errors
+from rforge.library.tools.rescale_dataset import rescale_dataset
 
 ERROR_MESSAGES = {
     "no_file": "Error: The file {file_path} does not exist.",
     "array": "ERROR: 'array' argument is {array_type}, but it must be a NumPy array of numeric type.",
     "bounds_type": (
         "ERROR: 'bounds' argument is {bounds_type}, but it must be a dictionary."
     ),
@@ -19,14 +19,47 @@
     "no_data": "ERROR: 'no_data' argument is {no_data_type}, but it must be an integer or float.",
     "transform": "ERROR: 'transform' argument is {transform_type}, but it must be a tuple of six floats.",
     "units": "ERROR: 'units' argument is {units_type}, but it must be a string.",
 }
 
 
 class Layer:
+    """Represents a data layer in a geospatial dataset.
+
+    Attributes:
+        _array (Optional[np.ndarray[np.int32]]): The array data of the layer.
+        _bounds (Optional[Dict[str, float]]): The spatial bounds of the layer.
+        _crs (Optional[str]): The coordinate reference system (CRS) of the layer.
+        _driver (Optional[str]): The driver used for data storage.
+        _no_data (Optional[Union[int, float]]): The value representing no data in the layer.
+        _transform (Optional[Tuple[float, float, float, float, float, float]]): Affine transformation parameters.
+        _units (Optional[str]): The units of the layer data.
+
+    Methods:
+        __init__: Initializes a Layer instance.
+        __eq__: Checks equality between two Layer instances or a Layer and a numpy array.
+        __str__: Returns a string representation of the layer attributes.
+        import_layer: Imports layer data from a file.
+        array: Getter and setter for the layer array data.
+        bounds: Getter and setter for the spatial bounds.
+        crs: Getter and setter for the CRS.
+        driver: Getter and setter for the driver.
+        no_data: Getter and setter for the no_data value.
+        transform: Getter and setter for the affine transformation parameters.
+        units: Getter and setter for the units.
+        resolution: Computes the resolution of the layer.
+        width: Computes the width of the layer.
+        height: Computes the height of the layer.
+        count: Computes the number of bands in the layer.
+        mean: Computes the mean value(s) of the layer data.
+        median: Computes the median value(s) of the layer data.
+        min: Computes the minimum value(s) of the layer data.
+        max: Computes the maximum value(s) of the layer data.
+        std_dev: Computes the standard deviation value(s) of the layer data.
+    """
     _array: Optional[np.ndarray[Union[np.uint8, np.int32]]] = None
 
     _bounds: Optional[Dict[str, float]] = None
     _crs: Optional[str] = None
     _driver: Optional[str] = None
     _no_data: Optional[Union[int, float]] = None
     _transform: Optional[Tuple[float, float, float, float, float, float]] = None
@@ -144,15 +177,15 @@
 
     def import_layer(self, path: str, id: int = 1, scale: Optional[int] = None):
         if not os.path.exists(path):
             raise FileNotFoundError(ERROR_MESSAGES["no_file"].format(file_path=path))
 
         with rasterio.open(path) as dataset:
             if scale is not None:
-                dataset = _rescale_dataset(dataset, scale)
+                dataset = rescale_dataset(dataset, scale)
 
             array = dataset.read(id)
 
             bounds = {
                 "left": dataset.bounds[0],
                 "bottom": dataset.bounds[1],
                 "right": dataset.bounds[2],
```

### Comparing `raster-forge-0.5.1/rforge/containers/raster.py` & `raster-forge-0.6.0/rforge/library/containers/raster.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,41 @@
 import os
 from typing import Dict, Optional, TypedDict
 
 import rasterio
-from rforge.tools.rescale_dataset import _rescale_dataset
 
-from ..tools.exceptions import Errors
-from .layer import Layer
+from rforge.library.tools.rescale_dataset import rescale_dataset
+from rforge.library.tools.exceptions import Errors
+
+from rforge.library.containers.layer import Layer
 
 
 class RasterImportConfig(TypedDict):
     id: int
     name: str
 
 
 class Raster:
+    """Represents a collection of layers in a geospatial dataset.
+
+    Attributes:
+        _layers (Dict[str, Layer]): Dictionary mapping layer names to Layer instances.
+        _scale (int): The scale factor of the raster dataset.
+
+    Methods:
+        __init__: Initializes a Raster instance.
+        __str__: Returns a string representation of the raster dataset.
+        layers: Getter for the layers dictionary.
+        count: Computes the number of layers in the dataset.
+        scale: Getter for the scale factor.
+        import_layers: Imports layers from a raster file.
+        add_layer: Adds a layer to the raster dataset.
+        remove_layer: Removes a layer from the raster dataset.
+        edit_layer: Renames a layer in the raster dataset.
+    """
     _layers: Dict[str, Layer]
     _scale: int
 
     def __init__(self, scale: int, layers: Optional[Dict[str, Layer]] = None):
         if not isinstance(scale, int) or (isinstance(scale, int) and scale <= 0):
             raise TypeError(
                 Errors.bad_input(name="scale", expected_type="an integer larger than 0")
@@ -53,21 +71,21 @@
         return len(self._layers)
 
     @property
     def scale(self) -> int:
         return self._scale
 
     def import_layers(
-        self, path: str, config: Optional[list[RasterImportConfig]] = None
+        self, path: str, config: Optional[list[Dict[str, str | int]]] = None
     ):
         if not os.path.exists(path):
             raise FileNotFoundError(Errors.file_not_found(file_path=path))
 
         with rasterio.open(path) as dataset:
-            dataset = _rescale_dataset(dataset, self.scale)
+            dataset = rescale_dataset(dataset, self.scale)
 
             if config is None:
                 config = []
                 for id in range(1, dataset.count + 1):
                     aux_config = {}
                     aux_config["name"] = f"Layer {id}"
                     aux_config["id"] = id
```

### Comparing `raster-forge-0.5.1/rforge/gui/common/adaptative_elements.py` & `raster-forge-0.6.0/rforge/gui/common/adaptative_elements.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.5.1/rforge/gui/common/layer_information.py` & `raster-forge-0.6.0/rforge/gui/common/layer_information.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.5.1/rforge/gui/gui.py` & `raster-forge-0.6.0/rforge/gui/gui.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import sys
 
-from PySide6.QtCore import QFile, QTextStream, QTimer
-from PySide6.QtWidgets import QApplication
-
-from .main_window import _MainWindow
-from .resources import resources
+try:
+    from PySide6.QtCore import QFile, QTextStream, QTimer
+    from PySide6.QtWidgets import QApplication
+
+    from .main_window import _MainWindow
+    from .resources import resources
+
+    GUI_COMPONENT = True
+except ImportError:
+    GUI_COMPONENT = False
 
 
 def _cleanup(main_window):
     main_window.close()
 
 
 def _show_main_window(main_window):
@@ -26,24 +31,27 @@
     style_file.close()
 
     return app
 
 
 def gui():
     """Launches the Raster Forge Graphical User Interface (GUI)."""
-    global main_window
-    try:
-        app = _initialize_application()
-        main_window = _MainWindow()
-
-        # Connect the Cleanup Function
-        app.aboutToQuit.connect(lambda: _cleanup(main_window))
-
-        # Delay Showing the Main Window
-        QTimer.singleShot(1000, lambda: _show_main_window(main_window))
-
-        sys.exit(app.exec_())
-
-    except Exception as e:
-        print(f"An Error Occurred During Initialization: {e}")
-    finally:
-        _cleanup(main_window)
+    if GUI_COMPONENT:
+        global main_window
+        try:
+            app = _initialize_application()
+            main_window = _MainWindow()
+
+            # Connect the Cleanup Function
+            app.aboutToQuit.connect(lambda: _cleanup(main_window))
+
+            # Delay Showing the Main Window
+            QTimer.singleShot(1000, lambda: _show_main_window(main_window))
+
+            sys.exit(app.exec_())
+
+        except Exception as e:
+            print(f"An Error Occurred During Initialization: {e}")
+        finally:
+            _cleanup(main_window)
+    else:
+        print("ERROR: GUI COMPONENT NOT INSTALLED")
```

### Comparing `raster-forge-0.5.1/rforge/gui/layers/import_layers.py` & `raster-forge-0.6.0/rforge/gui/layers/import_layers.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     QProgressBar,
     QPushButton,
     QScrollArea,
     QSpinBox,
     QVBoxLayout,
     QWidget,
 )
-from rforge.containers.raster import Raster
+from rforge.library.containers.raster import Raster
 from rforge.gui.data import _data
-from rforge.tools.rescale_dataset import _rescale_dataset_preview
+from rforge.library.tools.rescale_dataset import rescale_dataset_preview
 
 
 class _ImportWorkerSignals(QObject):
     finished = Signal()
 
 
 class _ImportWorker(QRunnable):
@@ -207,15 +207,15 @@
                     )
                     self._preview_callback()
                     self._populate_bands_checklist(num_bands)
 
     def _preview_callback(self):
         if self.selected_file_path is not None:
             with rasterio.open(self.selected_file_path) as dataset:
-                new_width, new_height = _rescale_dataset_preview(
+                new_width, new_height = rescale_dataset_preview(
                     dataset, self.scale_spinbox.value()
                 )
 
                 self.new_width.setText(str(new_width))
                 self.new_height.setText(str(new_height))
 
     def _populate_bands_checklist(self, num_bands):
```

### Comparing `raster-forge-0.5.1/rforge/gui/layers/layers.py` & `raster-forge-0.6.0/rforge/gui/layers/layers.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.5.1/rforge/gui/main_window.py` & `raster-forge-0.6.0/rforge/gui/main_window.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.5.1/rforge/gui/processes/panels/composites.py` & `raster-forge-0.6.0/rforge/gui/processes/panels/composites.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from typing import Type
 
 import numpy as np
-from matplotlib.colors import Normalize
-from rforge.containers.layer import Layer
 from rforge.gui.common.adaptative_elements import _adaptative_input
 from rforge.gui.data import _data
 from rforge.gui.processes.process_panel import _ProcessPanel
-from rforge.processes.composite import PRESET_COMPOSITES, composite
+from rforge.library.processes.composite import PRESET_COMPOSITES, composite
 
 ARRAY_TYPE: Type[np.ndarray] = np.ndarray
 
 
 class _CompositesPanel(_ProcessPanel):
     def __init__(self, name=None, selector=False, parent=None):
         super().__init__(name=name, selector=selector, parent=parent)
```

### Comparing `raster-forge-0.5.1/rforge/gui/processes/panels/distance.py` & `raster-forge-0.6.0/rforge/gui/processes/panels/distance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Type
 
 import numpy as np
-from rforge.containers.layer import Layer
+from rforge.library.containers.layer import Layer
 from rforge.gui.common.adaptative_elements import _adaptative_input
 from rforge.gui.data import _data
 from rforge.gui.processes.process_panel import _ProcessPanel
-from rforge.processes.distance import distance
+from rforge.library.processes.distance import distance
 
 ARRAY_TYPE: Type[np.ndarray] = np.ndarray
 
 
 class _DistanceFieldPanel(_ProcessPanel):
     def __init__(self, name=None, selector=False, parent=None):
         super().__init__(name=name, selector=selector, parent=parent)
```

### Comparing `raster-forge-0.5.1/rforge/gui/processes/panels/fuel.py` & `raster-forge-0.6.0/rforge/gui/processes/panels/fuel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Type
 
 import numpy as np
-from rforge.containers.layer import Layer
 from rforge.gui.common.adaptative_elements import _adaptative_input
 from rforge.gui.data import _data
 from rforge.gui.processes.process_panel import _ProcessPanel
-from rforge.processes.fuel import fuel
+from rforge.library.processes.fuel import fuel
 
 ARRAY_TYPE: Type[np.ndarray] = np.ndarray
 
 
 class _FuelMapPanel(_ProcessPanel):
     def __init__(self, name=None, selector=False, parent=None):
         super().__init__(name=name, selector=selector, parent=parent)
```

### Comparing `raster-forge-0.5.1/rforge/gui/processes/panels/height.py` & `raster-forge-0.6.0/rforge/gui/processes/panels/height.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Type
 
 import numpy as np
-from rforge.containers.layer import Layer
+from rforge.library.containers.layer import Layer
 from rforge.gui.common.adaptative_elements import _adaptative_input
 from rforge.gui.data import _data
 from rforge.gui.processes.process_panel import _ProcessPanel
-from rforge.processes.height import height
+from rforge.library.processes.height import height
 
 ARRAY_TYPE: Type[np.ndarray] = np.ndarray
 
 
 class _HeightPanel(_ProcessPanel):
     def __init__(self, name=None, selector=False, parent=None):
         super().__init__(name=name, selector=selector, parent=parent)
```

### Comparing `raster-forge-0.5.1/rforge/gui/processes/panels/indices.py` & `raster-forge-0.6.0/rforge/gui/processes/panels/indices.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Type
 
 import numpy as np
 import spyndex
-from rforge.containers.layer import Layer
+from rforge.library.containers.layer import Layer
 from rforge.gui.common.adaptative_elements import _adaptative_input
 from rforge.gui.data import _data
 from rforge.gui.processes.process_panel import _ProcessPanel
-from rforge.processes.index import index
+from rforge.library.processes.index import index
 
 ARRAY_TYPE: Type[np.ndarray] = np.ndarray
 
 
 class _IndicesPanel(_ProcessPanel):
     def __init__(self, name=None, selector=False, parent=None):
         super().__init__(name=name, selector=selector, parent=parent)
```

### Comparing `raster-forge-0.5.1/rforge/gui/processes/panels/topography.py` & `raster-forge-0.6.0/rforge/gui/processes/panels/topography.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Type
 
 import numpy as np
-from rforge.containers.layer import Layer
+from rforge.library.containers.layer import Layer
 from rforge.gui.common.adaptative_elements import _adaptative_input
 from rforge.gui.data import _data
 from rforge.gui.processes.process_panel import _ProcessPanel
-from rforge.processes.topography import aspect, slope
+from rforge.library.processes.topography import aspect, slope
 
 ARRAY_TYPE: Type[np.ndarray] = np.ndarray
 
 
 class _TopographyPanel(_ProcessPanel):
     def __init__(self, name=None, selector=False, parent=None):
         super().__init__(name=name, selector=selector, parent=parent)
```

### Comparing `raster-forge-0.5.1/rforge/gui/processes/process_panel.py` & `raster-forge-0.6.0/rforge/gui/processes/process_panel.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.5.1/rforge/gui/processes/processes.py` & `raster-forge-0.6.0/rforge/gui/processes/processes.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.5.1/rforge/gui/resources/resources.py` & `raster-forge-0.6.0/rforge/gui/resources/resources.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.5.1/rforge/gui/viewer/save_operations.py` & `raster-forge-0.6.0/rforge/gui/viewer/save_operations.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.5.1/rforge/gui/viewer/viewer.py` & `raster-forge-0.6.0/rforge/gui/viewer/viewer.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.5.1/rforge/processes/composite.py` & `raster-forge-0.6.0/rforge/library/processes/composite.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional, Union
 
 import numpy as np
-from rforge.containers.layer import Layer
-from rforge.tools.data_validation import check_layer
-from rforge.tools.exceptions import Errors
+from rforge.library.containers.layer import Layer
+from rforge.library.tools.data_validation import check_layer
+from rforge.library.tools.exceptions import Errors
 
 PRESET_COMPOSITES = {
     "True Color": ["Red", "Green", "Blue"],
     "CIR": ["NIR", "Red", "Green"],
 }
```

### Comparing `raster-forge-0.5.1/rforge/processes/distance.py` & `raster-forge-0.6.0/rforge/library/processes/distance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional, Union
 
 import cv2
 import numpy as np
-from rforge.containers.layer import Layer
-from rforge.tools.data_validation import check_layer
-from rforge.tools.exceptions import Errors
+from rforge.library.containers.layer import Layer
+from rforge.library.tools.data_validation import check_layer
+from rforge.library.tools.exceptions import Errors
 
 
 def distance(
     layer: Union[Layer, np.ndarray],
     alpha: Optional[Union[Layer, np.ndarray]] = None,
     thresholds: Optional[Union[list, tuple]] = None,
     invert: bool = False,
```

### Comparing `raster-forge-0.5.1/rforge/processes/fuel.py` & `raster-forge-0.6.0/rforge/library/processes/fuel.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import math
 from typing import Optional, Union
 
 import numpy as np
-from rforge.containers.layer import Layer
-from rforge.tools.data_validation import check_layer
-from rforge.tools.exceptions import Errors
+from rforge.library.containers.layer import Layer
+from rforge.library.tools.data_validation import check_layer
+from rforge.library.tools.exceptions import Errors
 
 
 def fuel(
     coverage: Union[Layer, np.ndarray],
     height: Union[Layer, np.ndarray],
     distance: Union[Layer, np.ndarray],
     water: Union[Layer, np.ndarray],
```

### Comparing `raster-forge-0.5.1/rforge/processes/height.py` & `raster-forge-0.6.0/rforge/library/processes/height.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional, Union
 
 import numpy as np
-from rforge.containers.layer import Layer
-from rforge.tools.data_validation import check_layer
-from rforge.tools.exceptions import Errors
+from rforge.library.containers.layer import Layer
+from rforge.library.tools.data_validation import check_layer
+from rforge.library.tools.exceptions import Errors
 
 
 def height(
     dtm: Union[Layer, np.ndarray],
     dsm: Union[Layer, np.ndarray],
     alpha: Optional[Union[Layer, np.ndarray]] = None,
     as_array: bool = False,
```

### Comparing `raster-forge-0.5.1/rforge/processes/index.py` & `raster-forge-0.6.0/rforge/library/processes/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional, Union
 
 import numpy as np
 import spyndex
-from rforge.containers.layer import Layer
-from rforge.tools.data_validation import check_layer
-from rforge.tools.exceptions import Errors
+from rforge.library.containers.layer import Layer
+from rforge.library.tools.data_validation import check_layer
+from rforge.library.tools.exceptions import Errors
 
 
 def index(
     index_id: str,
     parameters: dict,
     alpha: Optional[Union[Layer, np.ndarray]] = None,
     thresholds: Optional[Union[list, tuple]] = None,
```

### Comparing `raster-forge-0.5.1/rforge/processes/topography.py` & `raster-forge-0.6.0/rforge/library/processes/topography.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional, Union
 
 import numpy as np
-from rforge.containers.layer import Layer
-from rforge.tools.data_validation import check_layer
-from rforge.tools.exceptions import Errors
+from rforge.library.containers.layer import Layer
+from rforge.library.tools.data_validation import check_layer
+from rforge.library.tools.exceptions import Errors
 
 
 def slope(
     dem: Union[Layer, np.ndarray],
     units: str = "degrees",
     alpha: Optional[Union[Layer, np.ndarray]] = None,
     as_array: bool = False,
```

### Comparing `raster-forge-0.5.1/rforge/tools/data_validation.py` & `raster-forge-0.6.0/rforge/library/tools/data_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Union
 
 import numpy as np
-from rforge.containers.layer import Layer
+from rforge.library.containers.layer import Layer
 
 
 def check_layer(layer: Union[Layer, np.ndarray]):
     """
     Check if a given input, which can be either a Layer object or a NumPy array, is numerical and non-empty.
 
     Args:
```

### Comparing `raster-forge-0.5.1/rforge/tools/exceptions.py` & `raster-forge-0.6.0/rforge/library/tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `raster-forge-0.5.1/rforge/tools/rescale_dataset.py` & `raster-forge-0.6.0/rforge/library/tools/rescale_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import numpy as np
 import rasterio
 from rasterio import MemoryFile
 from rasterio.enums import Resampling
 
 
-def _rescale_dataset_preview(dataset, pixel_size):
+def rescale_dataset_preview(dataset, pixel_size):
     resampling_factor_x = dataset.res[0] / pixel_size
     resampling_factor_y = dataset.res[1] / pixel_size
 
     new_width = max(int(dataset.width * resampling_factor_x), 1)
     new_height = max(int(dataset.height * resampling_factor_y), 1)
 
     return new_width, new_height
 
 
-def _rescale_dataset(dataset, pixel_size):
+def rescale_dataset(dataset, pixel_size):
     resampling_factor_x = dataset.res[0] / pixel_size
     resampling_factor_y = dataset.res[1] / pixel_size
 
     new_width = max(int(dataset.width * resampling_factor_x), 1)
     new_height = max(int(dataset.height * resampling_factor_y), 1)
 
     new_transform = dataset.transform * rasterio.Affine.scale(
```

