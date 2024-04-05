# Comparing `tmp/openttdlab-0.0.8.tar.gz` & `tmp/openttdlab-0.0.9.tar.gz`

## Comparing `openttdlab-0.0.8.tar` & `openttdlab-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     5927 2020-02-02 00:00:00.000000 openttdlab-0.0.8/openttdlab.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 openttdlab-0.0.8/.gitignore
--rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 openttdlab-0.0.8/LICENSE
--rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 openttdlab-0.0.8/README.md
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 openttdlab-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4447 2020-02-02 00:00:00.000000 openttdlab-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     5927 2020-02-02 00:00:00.000000 openttdlab-0.0.9/openttdlab.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 openttdlab-0.0.9/.gitignore
+-rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 openttdlab-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 openttdlab-0.0.9/README.md
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 openttdlab-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 openttdlab-0.0.9/PKG-INFO
```

### Comparing `openttdlab-0.0.8/openttdlab.py` & `openttdlab-0.0.9/openttdlab.py`

 * *Files identical despite different names*

### Comparing `openttdlab-0.0.8/LICENSE` & `openttdlab-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openttdlab-0.0.8/README.md` & `openttdlab-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <p align="center">
-  <img alt="OpenTTDLab logo" width="256" height="254" src="./docs/assets/openttdlab-logo.svg">
+  <img alt="OpenTTDLab logo" width="256" height="254" src="https://raw.githubusercontent.com/michalc/OpenTTDLab/main/docs/assets/openttdlab-logo.svg">
 </p>
 
-<p align="center"><strong>OpenTTDLab</strong> - <em>Run reproducible experiments on OpenTTD</em></p>
+<p align="center"><strong>OpenTTDLab</strong> - <em>Run reproducible experiments using OpenTTD</em></p>
 
 <p align="center">
     <a href="https://pypi.org/project/OpenTTDLab/"><img alt="PyPI package" src="https://img.shields.io/pypi/v/OpenTTDLab?label=PyPI%20package"></a>
     <a href="https://github.com/michalc/OpenTTDLab/actions/workflows/test.yml"><img alt="Test suite" src="https://img.shields.io/github/actions/workflow/status/michalc/OpenTTDLab/test.yml?label=Test%20suite"></a>
     <a href="https://app.codecov.io/gh/michalc/OpenTTDLab"><img alt="Code coverage" src="https://img.shields.io/codecov/c/github/michalc/OpenTTDLab?label=Code%20coverage"></a>
 </p>
 
 ---
 
-OpenTTD is a Python framework for running reproducible experiments using OpenTTD. An _experiment_ in OpenTTDLab terms is the combination of:
+OpenTTD is a Python framework for running reproducible experiments using OpenTTD, and extracting results from them. An _experiment_ in OpenTTDLab terms is the combination of:
 
 - Exact version of OpenTTD, any AIs used, and OpenTTDLab itself
 - Ranges of values for OpenTTD config settings, command line arguments and random seed
 - Granularity of output
 
 This can be configured/extracted for each experiment in either machine or human readable forms, for use in code or publishing respectively.
```

#### html2text {}

```diff
@@ -1,37 +1,37 @@
                                [OpenTTDLab logo]
-             OOppeennTTTTDDLLaabb - RRuunn rreepprroodduucciibbllee eexxppeerriimmeennttss oonn OOppeennTTTTDD
+            OOppeennTTTTDDLLaabb - RRuunn rreepprroodduucciibbllee eexxppeerriimmeennttss uussiinngg OOppeennTTTTDD
                    _[_P_y_P_I_ _p_a_c_k_a_g_e_]_[_T_e_s_t_ _s_u_i_t_e_]_[_C_o_d_e_ _c_o_v_e_r_a_g_e_]
 --- OpenTTD is a Python framework for running reproducible experiments using
-OpenTTD. An _experiment_ in OpenTTDLab terms is the combination of: - Exact
-version of OpenTTD, any AIs used, and OpenTTDLab itself - Ranges of values for
-OpenTTD config settings, command line arguments and random seed - Granularity
-of output This can be configured/extracted for each experiment in either
-machine or human readable forms, for use in code or publishing respectively.
-OpenTTDLab is based on [TrueBrain's OpenTTD Savegame Reader](https://
-github.com/TrueBrain/OpenTTD-savegame-reader), but it is not affiliated with
-OpenTTD. > [!NOTE] > Work in progress. This README serves as a rough design
-spec. ## Installation ```shell python -m pip install OpenTTDLab ``` On macOS,
-OpenTTDLab requires [7-zip](https://www.7-zip.org/), but this is not installed
-automatically. To install 7-zip on macOS, first install [Homebrew](https://
-brew.sh/), and then use Homebrew to install the p7zip package that contains 7-
-zip. ```shell brew install p7zip ``` ## Running an experiment The core function
-of OpenTTD is the `setup_experiment` function. ```python from openttdlab import
-setup_experiment, save_config # If necessary, this will download the latest
-OpenTTD run_experiment, get_config = setup_experiment() # Run the experiment
-and get results. This may take time results = run_experiment() print(results) #
-The information needed to reproduce the experiment config = get_config() print
-(config) # Which can be saved to a file and then shared save_config('my-
-config.yml', config) ``` ## Reproducing an experiment If you have the config
-from a previous experiment, you can pass it into `setup_experiment` to exactly
-reproduce ```python from openttdlab import setup_experiment, load_config # Load
-the config from file config = load_config('my-config.yml') #
-allow_platform_difference=True will allow experiments from a platform other
-than the one # the original experiments were performed on. Otherwise,
-setup_experiment may error because # the exact same OpenTTD will not be able to
-be run on this platform run_experiment, get_config = setup_experiment
-(config=config, allow_platform_difference=True) # Run the experiment and get
-results results = run_experiment() print(results) ``` ## API design
-considerations - Mutability is avoided - Impure functions are avoided - In
-terms of the user-facing API, keeping it mostly OOP-free, and deliberately
+OpenTTD, and extracting results from them. An _experiment_ in OpenTTDLab terms
+is the combination of: - Exact version of OpenTTD, any AIs used, and OpenTTDLab
+itself - Ranges of values for OpenTTD config settings, command line arguments
+and random seed - Granularity of output This can be configured/extracted for
+each experiment in either machine or human readable forms, for use in code or
+publishing respectively. OpenTTDLab is based on [TrueBrain's OpenTTD Savegame
+Reader](https://github.com/TrueBrain/OpenTTD-savegame-reader), but it is not
+affiliated with OpenTTD. > [!NOTE] > Work in progress. This README serves as a
+rough design spec. ## Installation ```shell python -m pip install OpenTTDLab
+``` On macOS, OpenTTDLab requires [7-zip](https://www.7-zip.org/), but this is
+not installed automatically. To install 7-zip on macOS, first install
+[Homebrew](https://brew.sh/), and then use Homebrew to install the p7zip
+package that contains 7-zip. ```shell brew install p7zip ``` ## Running an
+experiment The core function of OpenTTD is the `setup_experiment` function.
+```python from openttdlab import setup_experiment, save_config # If necessary,
+this will download the latest OpenTTD run_experiment, get_config =
+setup_experiment() # Run the experiment and get results. This may take time
+results = run_experiment() print(results) # The information needed to reproduce
+the experiment config = get_config() print(config) # Which can be saved to a
+file and then shared save_config('my-config.yml', config) ``` ## Reproducing an
+experiment If you have the config from a previous experiment, you can pass it
+into `setup_experiment` to exactly reproduce ```python from openttdlab import
+setup_experiment, load_config # Load the config from file config = load_config
+('my-config.yml') # allow_platform_difference=True will allow experiments from
+a platform other than the one # the original experiments were performed on.
+Otherwise, setup_experiment may error because # the exact same OpenTTD will not
+be able to be run on this platform run_experiment, get_config =
+setup_experiment(config=config, allow_platform_difference=True) # Run the
+experiment and get results results = run_experiment() print(results) ``` ## API
+design considerations - Mutability is avoided - Impure functions are avoided -
+In terms of the user-facing API, keeping it mostly OOP-free, and deliberately
 focused on key behaviour - Designed so if type checking were in place and
 passes, API misuse should be close to impossible
```

### Comparing `openttdlab-0.0.8/pyproject.toml` & `openttdlab-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "OpenTTDLab"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Michal Charemza", email="michal@charemza.name" },
   # Author of https://github.com/TrueBrain/OpenTTD-savegame-reader, which OpenTTDLab is a fork of
   { name="Patric Stout", email="truebrain@openttd.org" },
 ]
 description = "Python framework for running reproducible experiments using OpenTTD"
 readme = "README.md"
```

### Comparing `openttdlab-0.0.8/PKG-INFO` & `openttdlab-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenTTDLab
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python framework for running reproducible experiments using OpenTTD
 Project-URL: Source, https://github.com/michalc/OpenTTDLab
 Author-email: Michal Charemza <michal@charemza.name>, Patric Stout <truebrain@openttd.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -22,28 +22,28 @@
 Provides-Extra: dev
 Requires-Dist: coverage>=7.4.0; extra == 'dev'
 Requires-Dist: pytest-cov>=4.1.0; extra == 'dev'
 Requires-Dist: pytest>=7.4.4; extra == 'dev'
 Description-Content-Type: text/markdown
 
 <p align="center">
-  <img alt="OpenTTDLab logo" width="256" height="254" src="./docs/assets/openttdlab-logo.svg">
+  <img alt="OpenTTDLab logo" width="256" height="254" src="https://raw.githubusercontent.com/michalc/OpenTTDLab/main/docs/assets/openttdlab-logo.svg">
 </p>
 
-<p align="center"><strong>OpenTTDLab</strong> - <em>Run reproducible experiments on OpenTTD</em></p>
+<p align="center"><strong>OpenTTDLab</strong> - <em>Run reproducible experiments using OpenTTD</em></p>
 
 <p align="center">
     <a href="https://pypi.org/project/OpenTTDLab/"><img alt="PyPI package" src="https://img.shields.io/pypi/v/OpenTTDLab?label=PyPI%20package"></a>
     <a href="https://github.com/michalc/OpenTTDLab/actions/workflows/test.yml"><img alt="Test suite" src="https://img.shields.io/github/actions/workflow/status/michalc/OpenTTDLab/test.yml?label=Test%20suite"></a>
     <a href="https://app.codecov.io/gh/michalc/OpenTTDLab"><img alt="Code coverage" src="https://img.shields.io/codecov/c/github/michalc/OpenTTDLab?label=Code%20coverage"></a>
 </p>
 
 ---
 
-OpenTTD is a Python framework for running reproducible experiments using OpenTTD. An _experiment_ in OpenTTDLab terms is the combination of:
+OpenTTD is a Python framework for running reproducible experiments using OpenTTD, and extracting results from them. An _experiment_ in OpenTTDLab terms is the combination of:
 
 - Exact version of OpenTTD, any AIs used, and OpenTTDLab itself
 - Ranges of values for OpenTTD config settings, command line arguments and random seed
 - Granularity of output
 
 This can be configured/extracted for each experiment in either machine or human readable forms, for use in code or publishing respectively.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: OpenTTDLab Version: 0.0.8 Summary: Python framework
+Metadata-Version: 2.1 Name: OpenTTDLab Version: 0.0.9 Summary: Python framework
 for running reproducible experiments using OpenTTD Project-URL: Source, https:/
 /github.com/michalc/OpenTTDLab Author-email: Michal Charemza
 charemza.name>, Patric Stout
 openttd.org> License-File: LICENSE Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Requires-Python:
 >=3.8.0 Requires-Dist: httpx>=0.26.0 Requires-Dist: platformdirs>=4.1.0
@@ -10,43 +10,43 @@
 extra == 'ci' Requires-Dist: httpx==0.26.0; extra == 'ci' Requires-Dist:
 platformdirs==4.1.0; extra == 'ci' Requires-Dist: pytest-cov==4.1.0; extra ==
 'ci' Requires-Dist: pytest==7.4.4; extra == 'ci' Requires-Dist: pyyaml==6.0.1;
 extra == 'ci' Provides-Extra: dev Requires-Dist: coverage>=7.4.0; extra ==
 'dev' Requires-Dist: pytest-cov>=4.1.0; extra == 'dev' Requires-Dist:
 pytest>=7.4.4; extra == 'dev' Description-Content-Type: text/markdown
                                [OpenTTDLab logo]
-             OOppeennTTTTDDLLaabb - RRuunn rreepprroodduucciibbllee eexxppeerriimmeennttss oonn OOppeennTTTTDD
+            OOppeennTTTTDDLLaabb - RRuunn rreepprroodduucciibbllee eexxppeerriimmeennttss uussiinngg OOppeennTTTTDD
                    _[_P_y_P_I_ _p_a_c_k_a_g_e_]_[_T_e_s_t_ _s_u_i_t_e_]_[_C_o_d_e_ _c_o_v_e_r_a_g_e_]
 --- OpenTTD is a Python framework for running reproducible experiments using
-OpenTTD. An _experiment_ in OpenTTDLab terms is the combination of: - Exact
-version of OpenTTD, any AIs used, and OpenTTDLab itself - Ranges of values for
-OpenTTD config settings, command line arguments and random seed - Granularity
-of output This can be configured/extracted for each experiment in either
-machine or human readable forms, for use in code or publishing respectively.
-OpenTTDLab is based on [TrueBrain's OpenTTD Savegame Reader](https://
-github.com/TrueBrain/OpenTTD-savegame-reader), but it is not affiliated with
-OpenTTD. > [!NOTE] > Work in progress. This README serves as a rough design
-spec. ## Installation ```shell python -m pip install OpenTTDLab ``` On macOS,
-OpenTTDLab requires [7-zip](https://www.7-zip.org/), but this is not installed
-automatically. To install 7-zip on macOS, first install [Homebrew](https://
-brew.sh/), and then use Homebrew to install the p7zip package that contains 7-
-zip. ```shell brew install p7zip ``` ## Running an experiment The core function
-of OpenTTD is the `setup_experiment` function. ```python from openttdlab import
-setup_experiment, save_config # If necessary, this will download the latest
-OpenTTD run_experiment, get_config = setup_experiment() # Run the experiment
-and get results. This may take time results = run_experiment() print(results) #
-The information needed to reproduce the experiment config = get_config() print
-(config) # Which can be saved to a file and then shared save_config('my-
-config.yml', config) ``` ## Reproducing an experiment If you have the config
-from a previous experiment, you can pass it into `setup_experiment` to exactly
-reproduce ```python from openttdlab import setup_experiment, load_config # Load
-the config from file config = load_config('my-config.yml') #
-allow_platform_difference=True will allow experiments from a platform other
-than the one # the original experiments were performed on. Otherwise,
-setup_experiment may error because # the exact same OpenTTD will not be able to
-be run on this platform run_experiment, get_config = setup_experiment
-(config=config, allow_platform_difference=True) # Run the experiment and get
-results results = run_experiment() print(results) ``` ## API design
-considerations - Mutability is avoided - Impure functions are avoided - In
-terms of the user-facing API, keeping it mostly OOP-free, and deliberately
+OpenTTD, and extracting results from them. An _experiment_ in OpenTTDLab terms
+is the combination of: - Exact version of OpenTTD, any AIs used, and OpenTTDLab
+itself - Ranges of values for OpenTTD config settings, command line arguments
+and random seed - Granularity of output This can be configured/extracted for
+each experiment in either machine or human readable forms, for use in code or
+publishing respectively. OpenTTDLab is based on [TrueBrain's OpenTTD Savegame
+Reader](https://github.com/TrueBrain/OpenTTD-savegame-reader), but it is not
+affiliated with OpenTTD. > [!NOTE] > Work in progress. This README serves as a
+rough design spec. ## Installation ```shell python -m pip install OpenTTDLab
+``` On macOS, OpenTTDLab requires [7-zip](https://www.7-zip.org/), but this is
+not installed automatically. To install 7-zip on macOS, first install
+[Homebrew](https://brew.sh/), and then use Homebrew to install the p7zip
+package that contains 7-zip. ```shell brew install p7zip ``` ## Running an
+experiment The core function of OpenTTD is the `setup_experiment` function.
+```python from openttdlab import setup_experiment, save_config # If necessary,
+this will download the latest OpenTTD run_experiment, get_config =
+setup_experiment() # Run the experiment and get results. This may take time
+results = run_experiment() print(results) # The information needed to reproduce
+the experiment config = get_config() print(config) # Which can be saved to a
+file and then shared save_config('my-config.yml', config) ``` ## Reproducing an
+experiment If you have the config from a previous experiment, you can pass it
+into `setup_experiment` to exactly reproduce ```python from openttdlab import
+setup_experiment, load_config # Load the config from file config = load_config
+('my-config.yml') # allow_platform_difference=True will allow experiments from
+a platform other than the one # the original experiments were performed on.
+Otherwise, setup_experiment may error because # the exact same OpenTTD will not
+be able to be run on this platform run_experiment, get_config =
+setup_experiment(config=config, allow_platform_difference=True) # Run the
+experiment and get results results = run_experiment() print(results) ``` ## API
+design considerations - Mutability is avoided - Impure functions are avoided -
+In terms of the user-facing API, keeping it mostly OOP-free, and deliberately
 focused on key behaviour - Designed so if type checking were in place and
 passes, API misuse should be close to impossible
```

