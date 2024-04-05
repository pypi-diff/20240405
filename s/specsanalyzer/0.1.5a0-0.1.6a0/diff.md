# Comparing `tmp/specsanalyzer-0.1.5a0.tar.gz` & `tmp/specsanalyzer-0.1.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specsanalyzer-0.1.5a0.tar", max compression
+gzip compressed data, was "specsanalyzer-0.1.6a0.tar", max compression
```

## Comparing `specsanalyzer-0.1.5a0.tar` & `specsanalyzer-0.1.6a0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0     1067 2024-03-12 21:02:23.984980 specsanalyzer-0.1.5a0/LICENSE
--rw-r--r--   0        0        0     4279 2024-03-12 21:02:23.988980 specsanalyzer-0.1.5a0/README.md
--rw-r--r--   0        0        0     2631 2024-03-12 21:02:40.124994 specsanalyzer-0.1.5a0/pyproject.toml
--rwxr-xr-x   0        0        0      145 2024-03-12 21:02:23.988980 specsanalyzer-0.1.5a0/specsanalyzer/__init__.py
--rw-r--r--   0        0        0      695 2024-03-12 21:02:23.988980 specsanalyzer-0.1.5a0/specsanalyzer/config/default.yaml
--rwxr-xr-x   0        0        0      411 2024-03-12 21:02:23.988980 specsanalyzer-0.1.5a0/specsanalyzer/config/phoibos150.calib2d
--rwxr-xr-x   0        0        0     8973 2024-03-12 21:02:23.988980 specsanalyzer-0.1.5a0/specsanalyzer/config.py
--rwxr-xr-x   0        0        0    19345 2024-03-12 21:02:23.988980 specsanalyzer-0.1.5a0/specsanalyzer/convert.py
--rwxr-xr-x   0        0        0    22117 2024-03-12 21:02:23.988980 specsanalyzer-0.1.5a0/specsanalyzer/core.py
--rwxr-xr-x   0        0        0     4103 2024-03-12 21:02:23.992980 specsanalyzer-0.1.5a0/specsanalyzer/img_tools.py
--rwxr-xr-x   0        0        0    18805 2024-03-12 21:02:23.992980 specsanalyzer-0.1.5a0/specsanalyzer/io.py
--rwxr-xr-x   0        0        0      133 2024-03-12 21:02:23.992980 specsanalyzer-0.1.5a0/specsscan/__init__.py
--rw-r--r--   0        0        0    15202 2024-03-12 21:02:23.992980 specsanalyzer-0.1.5a0/specsscan/config/NXmpes_arpes_config.json
--rw-r--r--   0        0        0      556 2024-03-12 21:02:23.992980 specsanalyzer-0.1.5a0/specsscan/config/default.yaml
--rw-r--r--   0        0        0     3434 2024-03-12 21:02:23.992980 specsanalyzer-0.1.5a0/specsscan/config/example_config_FHI.yaml
--rwxr-xr-x   0        0        0    21413 2024-03-12 21:02:23.992980 specsanalyzer-0.1.5a0/specsscan/core.py
--rw-r--r--   0        0        0    20070 2024-03-12 21:02:23.992980 specsanalyzer-0.1.5a0/specsscan/helpers.py
--rw-r--r--   0        0        0     5621 1970-01-01 00:00:00.000000 specsanalyzer-0.1.5a0/setup.py
--rw-r--r--   0        0        0     5771 1970-01-01 00:00:00.000000 specsanalyzer-0.1.5a0/PKG-INFO
+-rwxr-xr-x   0        0        0     1067 2024-04-05 11:47:33.377485 specsanalyzer-0.1.6a0/LICENSE
+-rw-r--r--   0        0        0     4279 2024-04-05 11:47:33.377485 specsanalyzer-0.1.6a0/README.md
+-rw-r--r--   0        0        0     2631 2024-04-05 11:47:57.769663 specsanalyzer-0.1.6a0/pyproject.toml
+-rwxr-xr-x   0        0        0      145 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsanalyzer/__init__.py
+-rw-r--r--   0        0        0      695 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsanalyzer/config/default.yaml
+-rwxr-xr-x   0        0        0      411 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsanalyzer/config/phoibos150.calib2d
+-rwxr-xr-x   0        0        0     8973 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsanalyzer/config.py
+-rwxr-xr-x   0        0        0    19345 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsanalyzer/convert.py
+-rwxr-xr-x   0        0        0    22117 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsanalyzer/core.py
+-rwxr-xr-x   0        0        0     4103 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsanalyzer/img_tools.py
+-rwxr-xr-x   0        0        0    18805 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsanalyzer/io.py
+-rwxr-xr-x   0        0        0      133 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsscan/__init__.py
+-rwxr-xr-x   0        0        0    15200 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsscan/config/NXmpes_arpes_config.json
+-rw-r--r--   0        0        0      556 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsscan/config/default.yaml
+-rw-r--r--   0        0        0     3434 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsscan/config/example_config_FHI.yaml
+-rwxr-xr-x   0        0        0    21413 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsscan/core.py
+-rw-r--r--   0        0        0    20070 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsscan/helpers.py
+-rw-r--r--   0        0        0     5621 1970-01-01 00:00:00.000000 specsanalyzer-0.1.6a0/setup.py
+-rw-r--r--   0        0        0     5771 1970-01-01 00:00:00.000000 specsanalyzer-0.1.6a0/PKG-INFO
```

### Comparing `specsanalyzer-0.1.5a0/LICENSE` & `specsanalyzer-0.1.6a0/LICENSE`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.5a0/README.md` & `specsanalyzer-0.1.6a0/README.md`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.5a0/pyproject.toml` & `specsanalyzer-0.1.6a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "specsanalyzer"
 packages = [
     {include = "specsanalyzer"},
     {include = "specsscan"},
 ]
-version = "0.1.5a0"
+version = "0.1.6a0"
 description = "Python package for loading and converting SPECS Phoibos analyzer data."
 authors = [
     "Laurenz Rettig <rettig@fhi-berlin.mpg.de>",
     "Michele Puppin <michele.puppin@epfl.ch>",
     "Abeer Arora <arora@fhi-berlin.mpg.de>",
 ]
 readme = "README.md"
```

### Comparing `specsanalyzer-0.1.5a0/specsanalyzer/config/default.yaml` & `specsanalyzer-0.1.6a0/specsanalyzer/config/default.yaml`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.5a0/specsanalyzer/config.py` & `specsanalyzer-0.1.6a0/specsanalyzer/config.py`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.5a0/specsanalyzer/convert.py` & `specsanalyzer-0.1.6a0/specsanalyzer/convert.py`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.5a0/specsanalyzer/core.py` & `specsanalyzer-0.1.6a0/specsanalyzer/core.py`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.5a0/specsanalyzer/img_tools.py` & `specsanalyzer-0.1.6a0/specsanalyzer/img_tools.py`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.5a0/specsanalyzer/io.py` & `specsanalyzer-0.1.6a0/specsanalyzer/io.py`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.5a0/specsscan/config/NXmpes_arpes_config.json` & `specsanalyzer-0.1.6a0/specsscan/config/NXmpes_arpes_config.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999938905180841%*

 * *Differences: {"'/ENTRY[entry]/SAMPLE[sample]'": "{'transformations': {'offset_polar': -9}}"}*

```diff
@@ -328,15 +328,15 @@
             "offset_azimuth/@transformation_type": "rotation",
             "offset_azimuth/@units": "degrees",
             "offset_azimuth/@vector": [
                 0,
                 0,
                 1
             ],
-            "offset_polar": -321,
+            "offset_polar": -9,
             "offset_polar/@depends_on": "sample_polar",
             "offset_polar/@transformation_type": "rotation",
             "offset_polar/@units": "degrees",
             "offset_polar/@vector": [
                 0,
                 1,
                 0
```

### Comparing `specsanalyzer-0.1.5a0/specsscan/config/default.yaml` & `specsanalyzer-0.1.6a0/specsscan/config/default.yaml`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.5a0/specsscan/config/example_config_FHI.yaml` & `specsanalyzer-0.1.6a0/specsscan/config/example_config_FHI.yaml`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.5a0/specsscan/core.py` & `specsanalyzer-0.1.6a0/specsscan/core.py`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.5a0/specsscan/helpers.py` & `specsanalyzer-0.1.6a0/specsscan/helpers.py`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.5a0/setup.py` & `specsanalyzer-0.1.6a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 extras_require = \
 {'notebook': ['jupyter[notebook]>=1.0.0',
               'ipykernel[notebook]>=6.9.1',
               'jupyterlab-h5web[notebook]>=7.0.0']}
 
 setup_kwargs = {
     'name': 'specsanalyzer',
-    'version': '0.1.5a0',
+    'version': '0.1.6a0',
     'description': 'Python package for loading and converting SPECS Phoibos analyzer data.',
     'long_description': '[![Documentation Status](https://github.com/OpenCOMPES/specsanalyzer/actions/workflows/documentation.yml/badge.svg)](https://opencompes.github.io/specsanalyzer/)\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)\n![](https://github.com/OpenCOMPES/specsanalyzer/actions/workflows/linting.yml/badge.svg)\n![](https://github.com/OpenCOMPES/specsanalyzer/actions/workflows/testing_multiversion.yml/badge.svg?branch=main)\n![](https://img.shields.io/pypi/pyversions/specsanalyzer)\n![](https://img.shields.io/pypi/l/specsanalyzer)\n[![](https://img.shields.io/pypi/v/specsanalyzer)](https://pypi.org/project/specsanalyzer)\n[![Coverage Status](https://coveralls.io/repos/github/OpenCOMPES/specsanalyzer/badge.svg?branch=main&kill_cache=1)](https://coveralls.io/github/OpenCOMPES/specsanalyzer?branch=main)\n\n# specsanalyzer\nThis is the package `specsanalyzer` for conversion and handling of SPECS Phoibos analyzer data.\n\nThis package contains two modules:\n`specsanalyzer` is a package to import and convert MCP analyzer images from SPECS Phoibos analyzers into energy and emission angle/physical coordinates.\n`specsscan` is a Python package for loading Specs Phoibos scans accquired with the labview software developed at FHI/EPFL\n\nTutorials for usage and the API documentation can be found in the [Documentation](https://opencompes.github.io/specsanalyzer/)\n\n## Installation\n\n### Pip (for users)\n\n- Create a new virtual environment using either venv, pyenv, conda, etc. See below for an example.\n\n```bash\npython -m venv .specs-venv\n```\n\n- Activate your environment:\n\n```bash\nsource .specs-venv/bin/activate\n```\n\n- Install `specsanalyzer` from PyPI:\n\n```bash\npip install specsanalyzer\n```\n\n- This should install all the requirements to run `specsanalyzer` and `specsscan`in your environment.\n\n- If you intend to work with Jupyter notebooks, it is helpful to install a Jupyter kernel for your environment. This can be done, once your environment is activated, by typing:\n\n```bash\npython -m ipykernel install --user --name=specs_kernel\n```\n\n#### Configuration and calib2d file\nThe conversion procedures require to set up several configuration parameters in a config file. An example config file is provided as part of the package (see documentation). Configuration files can either be passed to the class constructures, or are read from system-wide or user-defined locations (see documentation).\n\nMost importantly, conversion of analyzer data to energy/angular coordinates requires detector calibration data provided by the manufacturer. The corresponding *.calib2d file (e.g. phoibos150.calbid2d) are provided together with the spectrometer software, and need to be set in the config file.\n\n### For Contributors\n\nTo contribute to the development of `specsanalyzer`, you can follow these steps:\n\n1. Clone the repository:\n\n```bash\ngit clone https://github.com/OpenCOMPES/specsanalyzer.git\ncd specsanalyzer\n```\n\n2. Check out test data (optional, requires access rights):\n\n```bash\ngit submodule sync --recursive\ngit submodule update --init --recursive\n```\n\n2. Install the repository in editable mode:\n\n```bash\npip install -e .\n```\n\nNow you have the development version of `specsanalyzer` installed in your local environment. Feel free to make changes and submit pull requests.\n\n### Poetry (for maintainers)\n\n- Prerequisites:\n  + Poetry: https://python-poetry.org/docs/\n\n- Create a virtual environment by typing:\n\n```bash\npoetry shell\n```\n\n- A new shell will be spawned with the new environment activated.\n\n- Install the dependencies from the `pyproject.toml` by typing:\n\n```bash\npoetry install --with dev, docs\n```\n\n- If you wish to use the virtual environment created by Poetry to work in a Jupyter notebook, you first need to install the optional notebook dependencies and then create a Jupyter kernel for that.\n\n  + Install the optional dependencies `ipykernel` and `jupyter`:\n\n  ```bash\n  poetry install -E notebook\n  ```\n\n  + Make sure to run the command below within your virtual environment (`poetry run` ensures this) by typing:\n\n  ```bash\n  poetry run ipython kernel install --user --name=specs_poetry\n  ```\n\n  + The new kernel will now be available in your Jupyter kernels list.\n',
     'author': 'Laurenz Rettig',
     'author_email': 'rettig@fhi-berlin.mpg.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mpes-kit/specsanalyzer',
```

### Comparing `specsanalyzer-0.1.5a0/PKG-INFO` & `specsanalyzer-0.1.6a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specsanalyzer
-Version: 0.1.5a0
+Version: 0.1.6a0
 Summary: Python package for loading and converting SPECS Phoibos analyzer data.
 Home-page: https://github.com/mpes-kit/specsanalyzer
 License: MIT
 Keywords: specs,phoibos,arpes
 Author: Laurenz Rettig
 Author-email: rettig@fhi-berlin.mpg.de
 Requires-Python: >=3.8,<3.12
```

