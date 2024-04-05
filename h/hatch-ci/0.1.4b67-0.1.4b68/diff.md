# Comparing `tmp/hatch-ci-0.1.4b67.tar.gz` & `tmp/hatch-ci-0.1.4b68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hatch-ci-0.1.4b67.tar", last modified: Fri Apr  5 16:14:37 2024, max compression
+gzip compressed data, was "hatch-ci-0.1.4b68.tar", last modified: Fri Apr  5 19:02:43 2024, max compression
```

## Comparing `hatch-ci-0.1.4b67.tar` & `hatch-ci-0.1.4b68.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:14:37.774263 hatch-ci-0.1.4b67/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-04-05 16:14:37.770263 hatch-ci-0.1.4b67/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-05 16:14:35.000000 hatch-ci-0.1.4b67/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:14:37.774263 hatch-ci-0.1.4b67/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:14:37.766263 hatch-ci-0.1.4b67/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:14:37.770263 hatch-ci-0.1.4b67/src/hatch_ci/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/code.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/fileos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/hook_build.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/hook_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/hook_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8277 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/scm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/script.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/text.py
--rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:14:37.770263 hatch-ci-0.1.4b67/src/hatch_ci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-04-05 16:14:37.000000 hatch-ci-0.1.4b67/src/hatch_ci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-05 16:14:37.000000 hatch-ci-0.1.4b67/src/hatch_ci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:14:37.000000 hatch-ci-0.1.4b67/src/hatch_ci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-05 16:14:37.000000 hatch-ci-0.1.4b67/src/hatch_ci.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 16:14:37.000000 hatch-ci-0.1.4b67/src/hatch_ci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 16:14:37.000000 hatch-ci-0.1.4b67/src/hatch_ci.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:14:37.770263 hatch-ci-0.1.4b67/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/tests/test_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/tests/test_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/tests/test_fileos.py
--rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/tests/test_script.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     9536 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:02:43.363867 hatch-ci-0.1.4b68/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-05 19:02:04.000000 hatch-ci-0.1.4b68/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-05 19:02:43.363867 hatch-ci-0.1.4b68/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-04-05 19:02:41.000000 hatch-ci-0.1.4b68/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-05 19:02:41.000000 hatch-ci-0.1.4b68/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 19:02:43.363867 hatch-ci-0.1.4b68/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:02:43.355867 hatch-ci-0.1.4b68/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:02:43.359867 hatch-ci-0.1.4b68/src/hatch_ci/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 19:02:04.000000 hatch-ci-0.1.4b68/src/hatch_ci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-05 19:02:04.000000 hatch-ci-0.1.4b68/src/hatch_ci/_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-05 19:02:04.000000 hatch-ci-0.1.4b68/src/hatch_ci/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-05 19:02:04.000000 hatch-ci-0.1.4b68/src/hatch_ci/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-05 19:02:04.000000 hatch-ci-0.1.4b68/src/hatch_ci/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-05 19:02:04.000000 hatch-ci-0.1.4b68/src/hatch_ci/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-05 19:02:04.000000 hatch-ci-0.1.4b68/src/hatch_ci/fileos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-05 19:02:04.000000 hatch-ci-0.1.4b68/src/hatch_ci/hook_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:02:04.000000 hatch-ci-0.1.4b68/src/hatch_ci/hook_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-05 19:02:04.000000 hatch-ci-0.1.4b68/src/hatch_ci/hook_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-05 19:02:04.000000 hatch-ci-0.1.4b68/src/hatch_ci/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8277 2024-04-05 19:02:04.000000 hatch-ci-0.1.4b68/src/hatch_ci/scm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-05 19:02:04.000000 hatch-ci-0.1.4b68/src/hatch_ci/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-05 19:02:04.000000 hatch-ci-0.1.4b68/src/hatch_ci/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-04-05 19:02:04.000000 hatch-ci-0.1.4b68/src/hatch_ci/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:02:43.363867 hatch-ci-0.1.4b68/src/hatch_ci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-05 19:02:43.000000 hatch-ci-0.1.4b68/src/hatch_ci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-05 19:02:43.000000 hatch-ci-0.1.4b68/src/hatch_ci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:02:43.000000 hatch-ci-0.1.4b68/src/hatch_ci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-05 19:02:43.000000 hatch-ci-0.1.4b68/src/hatch_ci.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 19:02:43.000000 hatch-ci-0.1.4b68/src/hatch_ci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 19:02:43.000000 hatch-ci-0.1.4b68/src/hatch_ci.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:02:43.363867 hatch-ci-0.1.4b68/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-05 19:02:04.000000 hatch-ci-0.1.4b68/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-05 19:02:04.000000 hatch-ci-0.1.4b68/tests/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-05 19:02:04.000000 hatch-ci-0.1.4b68/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-04-05 19:02:04.000000 hatch-ci-0.1.4b68/tests/test_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-05 19:02:04.000000 hatch-ci-0.1.4b68/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-05 19:02:04.000000 hatch-ci-0.1.4b68/tests/test_fileos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-04-05 19:02:04.000000 hatch-ci-0.1.4b68/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-05 19:02:04.000000 hatch-ci-0.1.4b68/tests/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-05 19:02:04.000000 hatch-ci-0.1.4b68/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9536 2024-04-05 19:02:04.000000 hatch-ci-0.1.4b68/tests/test_tools.py
```

### Comparing `hatch-ci-0.1.4b67/LICENSE.txt` & `hatch-ci-0.1.4b68/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b67/PKG-INFO` & `hatch-ci-0.1.4b68/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-ci
-Version: 0.1.4b67
+Version: 0.1.4b68
 Summary: Hatch plugin for ci system versioning
 Author-email: Antonio Cavallo <a.cavallo@cavallinux.eu>
 License: MIT
 Project-URL: Issues, https://github.com/cav71/hatch-ci/issues
 Project-URL: Source, https://github.com/cav71/hatch-ci
 Keywords: git,hatch,plugin,scm,version
 Classifier: Development Status :: 4 - Beta
@@ -25,16 +25,16 @@
 
 # hatch-ci
 
 [![PyPI version](https://img.shields.io/pypi/v/hatch-ci.svg?color=blue)](https://pypi.org/project/hatch-ci)
 [![Python versions](https://img.shields.io/pypi/pyversions/hatch-ci.svg)](https://pypi.org/project/hatch-ci)
 [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/)
 
-[![Build](https://github.com/cav71/hatch-ci/actions/workflows/master.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions/runs/0)
-[![codecov](https://codecov.io/gh/cav71/hatch-ci/branch/master/graph/badge.svg?token=521FB9K5KT)](https://codecov.io/gh/cav71/hatch-ci/branch/master)
+[![Build](https://github.com/cav71/hatch-ci/actions/workflows/beta/0.1.4.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions/runs/0)
+[![codecov](https://codecov.io/gh/cav71/hatch-ci/branch/beta%2F0.1.4/graph/badge.svg?token=521FB9K5KT)](https://codecov.io/gh/cav71/hatch-ci/branch/beta%2F0.1.4)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 > **NOTE** This is a beta branch!
 
@@ -164,11 +164,16 @@
 
 | Option | Type | Default | Description                                          |
 | --- | --- |---------|------------------------------------------------------|
 | `version-file` | `str` | None    | A file where to write __version__/__hash__ variables |
 | `paths` | `list[str]|str` | None | A list of paths to process |
 | `fixers` | `list[dict[str,str]]` | None | A list of dict, each key is a string to replace with the value |
 
+### Borrowed ideas/code
+
+- [hatch-fancy-pypi-readme](https://github.com/hynek/hatch-fancy-pypi-readme)
+- [hatch-vcs](https://github.com/ofek/hatch-vcs)
+
 
 ## License
 
 `hatch-ci` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `hatch-ci-0.1.4b67/README.md` & `hatch-ci-0.1.4b68/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # hatch-ci
 
 [![PyPI version](https://img.shields.io/pypi/v/hatch-ci.svg?color=blue)](https://pypi.org/project/hatch-ci)
 [![Python versions](https://img.shields.io/pypi/pyversions/hatch-ci.svg)](https://pypi.org/project/hatch-ci)
 [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/)
 
-[![Build](https://github.com/cav71/hatch-ci/actions/workflows/master.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions/runs/0)
-[![codecov](https://codecov.io/gh/cav71/hatch-ci/branch/master/graph/badge.svg?token=521FB9K5KT)](https://codecov.io/gh/cav71/hatch-ci/branch/master)
+[![Build](https://github.com/cav71/hatch-ci/actions/workflows/beta/0.1.4.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions/runs/0)
+[![codecov](https://codecov.io/gh/cav71/hatch-ci/branch/beta%2F0.1.4/graph/badge.svg?token=521FB9K5KT)](https://codecov.io/gh/cav71/hatch-ci/branch/beta%2F0.1.4)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 > **NOTE** This is a beta branch!
 
@@ -139,11 +139,16 @@
 
 | Option | Type | Default | Description                                          |
 | --- | --- |---------|------------------------------------------------------|
 | `version-file` | `str` | None    | A file where to write __version__/__hash__ variables |
 | `paths` | `list[str]|str` | None | A list of paths to process |
 | `fixers` | `list[dict[str,str]]` | None | A list of dict, each key is a string to replace with the value |
 
+### Borrowed ideas/code
+
+- [hatch-fancy-pypi-readme](https://github.com/hynek/hatch-fancy-pypi-readme)
+- [hatch-vcs](https://github.com/ofek/hatch-vcs)
+
 
 ## License
 
 `hatch-ci` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `hatch-ci-0.1.4b67/pyproject.toml` & `hatch-ci-0.1.4b68/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-__version__ = "0.1.4"
-__hash__ = "0.1.4"
+__version__ = "0.1.4b68"
+__hash__ = "08cf5396b9db6075277dad51c20a63416592a9d5"
 build-backend = "hatchling.build"
 
 [project]
 name = "hatch-ci"
-version = "0.1.4b67"
+version = "0.1.4b68"
 description = "Hatch plugin for ci system versioning"
 readme = "README.md"
 license = { text = "MIT" }
 requires-python = ">= 3.8"
 keywords = [
   "git",
   "hatch",
```

### Comparing `hatch-ci-0.1.4b67/src/hatch_ci/_support.py` & `hatch-ci-0.1.4b68/src/hatch_ci/_support.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b67/src/hatch_ci/cli.py` & `hatch-ci-0.1.4b68/src/hatch_ci/cli.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b67/src/hatch_ci/code.py` & `hatch-ci-0.1.4b68/src/hatch_ci/code.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b67/src/hatch_ci/exceptions.py` & `hatch-ci-0.1.4b68/src/hatch_ci/exceptions.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b67/src/hatch_ci/fileos.py` & `hatch-ci-0.1.4b68/src/hatch_ci/fileos.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b67/src/hatch_ci/hook_build.py` & `hatch-ci-0.1.4b68/src/hatch_ci/hook_build.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b67/src/hatch_ci/hook_version.py` & `hatch-ci-0.1.4b68/src/hatch_ci/hook_version.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b67/src/hatch_ci/scm.py` & `hatch-ci-0.1.4b68/src/hatch_ci/scm.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b67/src/hatch_ci/script.py` & `hatch-ci-0.1.4b68/src/hatch_ci/script.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b67/src/hatch_ci/text.py` & `hatch-ci-0.1.4b68/src/hatch_ci/text.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b67/src/hatch_ci/tools.py` & `hatch-ci-0.1.4b68/src/hatch_ci/tools.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b67/src/hatch_ci.egg-info/PKG-INFO` & `hatch-ci-0.1.4b68/src/hatch_ci.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-ci
-Version: 0.1.4b67
+Version: 0.1.4b68
 Summary: Hatch plugin for ci system versioning
 Author-email: Antonio Cavallo <a.cavallo@cavallinux.eu>
 License: MIT
 Project-URL: Issues, https://github.com/cav71/hatch-ci/issues
 Project-URL: Source, https://github.com/cav71/hatch-ci
 Keywords: git,hatch,plugin,scm,version
 Classifier: Development Status :: 4 - Beta
@@ -25,16 +25,16 @@
 
 # hatch-ci
 
 [![PyPI version](https://img.shields.io/pypi/v/hatch-ci.svg?color=blue)](https://pypi.org/project/hatch-ci)
 [![Python versions](https://img.shields.io/pypi/pyversions/hatch-ci.svg)](https://pypi.org/project/hatch-ci)
 [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/)
 
-[![Build](https://github.com/cav71/hatch-ci/actions/workflows/master.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions/runs/0)
-[![codecov](https://codecov.io/gh/cav71/hatch-ci/branch/master/graph/badge.svg?token=521FB9K5KT)](https://codecov.io/gh/cav71/hatch-ci/branch/master)
+[![Build](https://github.com/cav71/hatch-ci/actions/workflows/beta/0.1.4.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions/runs/0)
+[![codecov](https://codecov.io/gh/cav71/hatch-ci/branch/beta%2F0.1.4/graph/badge.svg?token=521FB9K5KT)](https://codecov.io/gh/cav71/hatch-ci/branch/beta%2F0.1.4)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 > **NOTE** This is a beta branch!
 
@@ -164,11 +164,16 @@
 
 | Option | Type | Default | Description                                          |
 | --- | --- |---------|------------------------------------------------------|
 | `version-file` | `str` | None    | A file where to write __version__/__hash__ variables |
 | `paths` | `list[str]|str` | None | A list of paths to process |
 | `fixers` | `list[dict[str,str]]` | None | A list of dict, each key is a string to replace with the value |
 
+### Borrowed ideas/code
+
+- [hatch-fancy-pypi-readme](https://github.com/hynek/hatch-fancy-pypi-readme)
+- [hatch-vcs](https://github.com/ofek/hatch-vcs)
+
 
 ## License
 
 `hatch-ci` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `hatch-ci-0.1.4b67/src/hatch_ci.egg-info/SOURCES.txt` & `hatch-ci-0.1.4b68/src/hatch_ci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b67/tests/test_cli.py` & `hatch-ci-0.1.4b68/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b67/tests/test_code.py` & `hatch-ci-0.1.4b68/tests/test_code.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b67/tests/test_conftest.py` & `hatch-ci-0.1.4b68/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b67/tests/test_e2e.py` & `hatch-ci-0.1.4b68/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b67/tests/test_exceptions.py` & `hatch-ci-0.1.4b68/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b67/tests/test_fileos.py` & `hatch-ci-0.1.4b68/tests/test_fileos.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b67/tests/test_scm.py` & `hatch-ci-0.1.4b68/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b67/tests/test_script.py` & `hatch-ci-0.1.4b68/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b67/tests/test_text.py` & `hatch-ci-0.1.4b68/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b67/tests/test_tools.py` & `hatch-ci-0.1.4b68/tests/test_tools.py`

 * *Files identical despite different names*

