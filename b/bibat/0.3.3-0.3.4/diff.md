# Comparing `tmp/bibat-0.3.3.tar.gz` & `tmp/bibat-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibat-0.3.3.tar", last modified: Wed Feb 28 13:47:16 2024, max compression
+gzip compressed data, was "bibat-0.3.4.tar", last modified: Fri Apr  5 10:02:34 2024, max compression
```

## Comparing `bibat-0.3.3.tar` & `bibat-0.3.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 13:47:16.454224 bibat-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-02-28 13:47:00.000000 bibat-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-02-28 13:47:16.454224 bibat-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-02-28 13:47:00.000000 bibat-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 13:47:16.454224 bibat-0.3.3/bibat/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-28 13:47:00.000000 bibat-0.3.3/bibat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-02-28 13:47:00.000000 bibat-0.3.3/bibat/fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-02-28 13:47:00.000000 bibat-0.3.3/bibat/fitting_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-02-28 13:47:00.000000 bibat-0.3.3/bibat/inference_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-28 13:47:00.000000 bibat-0.3.3/bibat/prepared_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-02-28 13:47:00.000000 bibat-0.3.3/bibat/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 13:47:16.454224 bibat-0.3.3/bibat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-02-28 13:47:16.000000 bibat-0.3.3/bibat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-02-28 13:47:16.000000 bibat-0.3.3/bibat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 13:47:16.000000 bibat-0.3.3/bibat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-28 13:47:16.000000 bibat-0.3.3/bibat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-28 13:47:16.000000 bibat-0.3.3/bibat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-02-28 13:47:00.000000 bibat-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 13:47:16.454224 bibat-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:02:34.203845 bibat-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-05 10:02:26.000000 bibat-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-04-05 10:02:34.203845 bibat-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-05 10:02:26.000000 bibat-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:02:34.203845 bibat-0.3.4/bibat/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-05 10:02:26.000000 bibat-0.3.4/bibat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-05 10:02:26.000000 bibat-0.3.4/bibat/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-04-05 10:02:26.000000 bibat-0.3.4/bibat/fitting_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-05 10:02:26.000000 bibat-0.3.4/bibat/inference_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-05 10:02:26.000000 bibat-0.3.4/bibat/prepared_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-05 10:02:26.000000 bibat-0.3.4/bibat/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:02:34.203845 bibat-0.3.4/bibat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-04-05 10:02:34.000000 bibat-0.3.4/bibat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-05 10:02:34.000000 bibat-0.3.4/bibat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 10:02:34.000000 bibat-0.3.4/bibat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-05 10:02:34.000000 bibat-0.3.4/bibat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 10:02:34.000000 bibat-0.3.4/bibat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-05 10:02:27.000000 bibat-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 10:02:34.203845 bibat-0.3.4/setup.cfg
```

### Comparing `bibat-0.3.3/LICENSE` & `bibat-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bibat-0.3.3/PKG-INFO` & `bibat-0.3.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibat
-Version: 0.3.3
+Version: 0.3.4
 Summary: Batteries-included Bayesian analysis template
 Author-email: Teddy Groves <tedgro@dtu.dk>
 License: GNU General Public License version 3
 Project-URL: homepage, https://github.com/teddygroves/bibat
 Project-URL: download, https://pypi.org/project/bibat
 Project-URL: documentation, https://bibat.readthedocs.io/
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -22,15 +22,17 @@
 Requires-Dist: cmdstanpy
 Requires-Dist: copier
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pandera
 Requires-Dist: pip>=20
 Requires-Dist: pydantic
+Requires-Dist: pyyaml-include<2
 Requires-Dist: scikit-learn
+Requires-Dist: scipy<1.13
 Requires-Dist: stanio
 Requires-Dist: toml
 Requires-Dist: xarray
 Requires-Dist: zarr
 Provides-Extra: development
 Requires-Dist: black; extra == "development"
 Requires-Dist: pre-commit; extra == "development"
@@ -136,23 +138,25 @@
 
 Bibat's development dependencies (install these by running `pip install
 bibat'[development]'`):
 
 - black
 - pre-commit
 - codecov
+- mkdocs
+- mkdocs-material
+- mkdocstrings
+- mkdocstrings-python
+- pymdown-extensions
 - pytest
 - pytest-cov
 - tox
-- sphinx
-- sphinx-click
 - ruff
-- furo
 
-Projects created by bibat have Python dependencies listed in their [pyproject.toml] file](https://github.com/teddygroves/bibat/blob/main/template/pyproject.toml.jinja). The additional ones are as follows:
+Projects created by bibat have Python dependencies listed in their [pyproject.toml file](https://github.com/teddygroves/bibat/blob/main/template/pyproject.toml.jinja). The additional ones are as follows:
 
 - bibat
 - jupyter
 
 In addition, the following Python packages may be installed, depending on how
 the user answers bibat's questionnaire:
```

### Comparing `bibat-0.3.3/README.md` & `bibat-0.3.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -89,23 +89,25 @@
 
 Bibat's development dependencies (install these by running `pip install
 bibat'[development]'`):
 
 - black
 - pre-commit
 - codecov
+- mkdocs
+- mkdocs-material
+- mkdocstrings
+- mkdocstrings-python
+- pymdown-extensions
 - pytest
 - pytest-cov
 - tox
-- sphinx
-- sphinx-click
 - ruff
-- furo
 
-Projects created by bibat have Python dependencies listed in their [pyproject.toml] file](https://github.com/teddygroves/bibat/blob/main/template/pyproject.toml.jinja). The additional ones are as follows:
+Projects created by bibat have Python dependencies listed in their [pyproject.toml file](https://github.com/teddygroves/bibat/blob/main/template/pyproject.toml.jinja). The additional ones are as follows:
 
 - bibat
 - jupyter
 
 In addition, the following Python packages may be installed, depending on how
 the user answers bibat's questionnaire:
```

### Comparing `bibat-0.3.3/bibat/fitting.py` & `bibat-0.3.4/bibat/fitting.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     InferenceConfiguration,
     load_inference_configuration,
 )
 from bibat.prepared_data import PreparedData
 
 
 class IdataSaveFormat(str, Enum):
-    """An enum for choosing the group that a fitting mode writes to."""
+    """An enum for choosing the format in which inferences are saved."""
 
     zarr = "prior"
     json = "json"
 
 
 def run_all_inferences(  # noqa: PLR0913
     inferences_dir: Path,
```

### Comparing `bibat-0.3.3/bibat/fitting_mode.py` & `bibat-0.3.4/bibat/fitting_mode.py`

 * *Files identical despite different names*

### Comparing `bibat-0.3.3/bibat/inference_configuration.py` & `bibat-0.3.4/bibat/inference_configuration.py`

 * *Files identical despite different names*

### Comparing `bibat-0.3.3/bibat/util.py` & `bibat-0.3.4/bibat/util.py`

 * *Files identical despite different names*

### Comparing `bibat-0.3.3/bibat.egg-info/PKG-INFO` & `bibat-0.3.4/bibat.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibat
-Version: 0.3.3
+Version: 0.3.4
 Summary: Batteries-included Bayesian analysis template
 Author-email: Teddy Groves <tedgro@dtu.dk>
 License: GNU General Public License version 3
 Project-URL: homepage, https://github.com/teddygroves/bibat
 Project-URL: download, https://pypi.org/project/bibat
 Project-URL: documentation, https://bibat.readthedocs.io/
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -22,15 +22,17 @@
 Requires-Dist: cmdstanpy
 Requires-Dist: copier
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pandera
 Requires-Dist: pip>=20
 Requires-Dist: pydantic
+Requires-Dist: pyyaml-include<2
 Requires-Dist: scikit-learn
+Requires-Dist: scipy<1.13
 Requires-Dist: stanio
 Requires-Dist: toml
 Requires-Dist: xarray
 Requires-Dist: zarr
 Provides-Extra: development
 Requires-Dist: black; extra == "development"
 Requires-Dist: pre-commit; extra == "development"
@@ -136,23 +138,25 @@
 
 Bibat's development dependencies (install these by running `pip install
 bibat'[development]'`):
 
 - black
 - pre-commit
 - codecov
+- mkdocs
+- mkdocs-material
+- mkdocstrings
+- mkdocstrings-python
+- pymdown-extensions
 - pytest
 - pytest-cov
 - tox
-- sphinx
-- sphinx-click
 - ruff
-- furo
 
-Projects created by bibat have Python dependencies listed in their [pyproject.toml] file](https://github.com/teddygroves/bibat/blob/main/template/pyproject.toml.jinja). The additional ones are as follows:
+Projects created by bibat have Python dependencies listed in their [pyproject.toml file](https://github.com/teddygroves/bibat/blob/main/template/pyproject.toml.jinja). The additional ones are as follows:
 
 - bibat
 - jupyter
 
 In addition, the following Python packages may be installed, depending on how
 the user answers bibat's questionnaire:
```

### Comparing `bibat-0.3.3/pyproject.toml` & `bibat-0.3.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bibat"
 authors = [
     {name = "Teddy Groves", email = "tedgro@dtu.dk"},
 ]
-version = "0.3.3"
+version = "0.3.4"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Natural Language :: English",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows :: Windows 10",
@@ -27,15 +27,17 @@
     "cmdstanpy",
     "copier",
     "numpy",
     "pandas",
     "pandera",
     "pip >= 20",
     "pydantic",
+    "pyyaml-include<2",  # temporary fix: see https://github.com/copier-org/copier/issues/1568
     "scikit-learn",
+    "scipy<1.13",  # temporary fix: see https://github.com/arviz-devs/arviz/issues/2336
     "stanio",
     "toml",
     "xarray",
     "zarr",
 ]
 
 [project.optional-dependencies]
```

