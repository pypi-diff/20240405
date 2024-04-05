# Comparing `tmp/coveragespace-6.0.2.tar.gz` & `tmp/coveragespace-6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coveragespace-6.0.2.tar", max compression
+gzip compressed data, was "coveragespace-6.1.tar", max compression
```

## Comparing `coveragespace-6.0.2.tar` & `coveragespace-6.1.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1088 2021-04-18 18:02:51.280685 coveragespace-6.0.2/LICENSE.md
--rw-r--r--   0        0        0     1795 2022-08-14 15:53:33.653518 coveragespace-6.0.2/README.md
--rw-r--r--   0        0        0      330 2022-11-09 20:29:07.853625 coveragespace-6.0.2/coveragespace/__init__.py
--rw-r--r--   0        0        0      949 2022-08-14 15:53:33.654829 coveragespace-6.0.2/coveragespace/api.py
--rw-r--r--   0        0        0     1709 2021-04-18 18:02:51.281962 coveragespace-6.0.2/coveragespace/cache.py
--rw-r--r--   0        0        0     3740 2021-04-18 18:02:51.282077 coveragespace-6.0.2/coveragespace/cli.py
--rw-r--r--   0        0        0     3256 2022-08-14 15:53:33.655297 coveragespace-6.0.2/coveragespace/coverage.py
--rw-r--r--   0        0        0      502 2022-08-14 15:53:33.655680 coveragespace-6.0.2/coveragespace/environments.py
--rw-r--r--   0        0        0     1613 2022-11-23 20:46:18.605537 coveragespace-6.0.2/coveragespace/repository.py
--rw-r--r--   0        0        0       50 2021-04-18 18:02:51.282548 coveragespace-6.0.2/coveragespace/tests/__init__.py
--rw-r--r--   0        0        0      267 2021-04-18 18:02:51.282687 coveragespace-6.0.2/coveragespace/tests/conftest.py
--rw-r--r--   0        0        0     1590 2021-04-18 18:02:51.282909 coveragespace-6.0.2/coveragespace/tests/test_cache.py
--rw-r--r--   0        0        0      719 2021-04-18 18:02:51.283049 coveragespace-6.0.2/coveragespace/tests/test_cli.py
--rw-r--r--   0        0        0     2239 2021-04-18 18:02:51.283173 coveragespace-6.0.2/coveragespace/tests/test_coverage.py
--rw-r--r--   0        0        0      676 2021-04-18 18:02:51.283281 coveragespace-6.0.2/coveragespace/tests/test_environments.py
--rw-r--r--   0        0        0     1046 2022-11-23 20:42:54.494065 coveragespace-6.0.2/coveragespace/tests/test_repository.py
--rw-r--r--   0        0        0     1864 2022-11-23 20:47:31.429150 coveragespace-6.0.2/pyproject.toml
--rw-r--r--   0        0        0     2726 2022-11-23 20:49:37.196581 coveragespace-6.0.2/setup.py
--rw-r--r--   0        0        0     3097 2022-11-23 20:49:37.196848 coveragespace-6.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1088 2021-04-18 18:02:51.280685 coveragespace-6.1/LICENSE.md
+-rw-r--r--   0        0        0     1651 2024-04-05 00:04:22.805587 coveragespace-6.1/README.md
+-rw-r--r--   0        0        0      330 2022-11-09 20:29:07.853625 coveragespace-6.1/coveragespace/__init__.py
+-rw-r--r--   0        0        0      949 2022-08-14 15:53:33.654829 coveragespace-6.1/coveragespace/api.py
+-rw-r--r--   0        0        0     1709 2021-04-18 18:02:51.281962 coveragespace-6.1/coveragespace/cache.py
+-rw-r--r--   0        0        0     4078 2024-04-05 00:28:46.961900 coveragespace-6.1/coveragespace/cli.py
+-rw-r--r--   0        0        0     3473 2024-04-05 00:30:27.002253 coveragespace-6.1/coveragespace/coverage.py
+-rw-r--r--   0        0        0      502 2022-08-14 15:53:33.655680 coveragespace-6.1/coveragespace/environments.py
+-rw-r--r--   0        0        0     1613 2022-11-23 20:46:18.605537 coveragespace-6.1/coveragespace/repository.py
+-rw-r--r--   0        0        0       50 2021-04-18 18:02:51.282548 coveragespace-6.1/coveragespace/tests/__init__.py
+-rw-r--r--   0        0        0      267 2021-04-18 18:02:51.282687 coveragespace-6.1/coveragespace/tests/conftest.py
+-rw-r--r--   0        0        0     1590 2021-04-18 18:02:51.282909 coveragespace-6.1/coveragespace/tests/test_cache.py
+-rw-r--r--   0        0        0      719 2021-04-18 18:02:51.283049 coveragespace-6.1/coveragespace/tests/test_cli.py
+-rw-r--r--   0        0        0     2239 2021-04-18 18:02:51.283173 coveragespace-6.1/coveragespace/tests/test_coverage.py
+-rw-r--r--   0        0        0      676 2021-04-18 18:02:51.283281 coveragespace-6.1/coveragespace/tests/test_environments.py
+-rw-r--r--   0        0        0     1046 2022-11-23 20:42:54.494065 coveragespace-6.1/coveragespace/tests/test_repository.py
+-rw-r--r--   0        0        0     1868 2024-04-05 00:21:32.870604 coveragespace-6.1/pyproject.toml
+-rw-r--r--   0        0        0     3053 1970-01-01 00:00:00.000000 coveragespace-6.1/PKG-INFO
```

### Comparing `coveragespace-6.0.2/LICENSE.md` & `coveragespace-6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `coveragespace-6.0.2/README.md` & `coveragespace-6.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Overview
 
 The official command-line client for [The Coverage Space](http://coverage.space).
 
-[![Unix Build Status](https://img.shields.io/travis/jacebrowning/coverage-space-cli/main.svg?label=unix)](https://travis-ci.org/jacebrowning/coverage-space-cli)
-[![Windows Build Status](https://img.shields.io/appveyor/ci/jacebrowning/coverage-space-cli/main.svg?label=window)](https://ci.appveyor.com/project/jacebrowning/coverage-space-cli)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/jacebrowning/coverage-space-cli/main.yml?branch=main&label=build)](https://github.com/jacebrowning/coverage-space-cli/actions)
 [![Coverage Status](https://img.shields.io/coveralls/jacebrowning/coverage-space-cli/main.svg)](https://coveralls.io/r/jacebrowning/coverage-space-cli)
 [![Scrutinizer Code Quality](https://img.shields.io/scrutinizer/g/jacebrowning/coverage-space-cli.svg)](https://scrutinizer-ci.com/g/jacebrowning/coverage-space-cli/?branch=main)
 [![PyPI Version](https://img.shields.io/pypi/v/coveragespace.svg)](https://pypi.org/project/coveragespace)
 [![PyPI License](https://img.shields.io/pypi/l/coveragespace.svg)](https://pypi.org/project/coveragespace)
 
 # Setup
```

### Comparing `coveragespace-6.0.2/coveragespace/api.py` & `coveragespace-6.1/coveragespace/api.py`

 * *Files identical despite different names*

### Comparing `coveragespace-6.0.2/coveragespace/cache.py` & `coveragespace-6.1/coveragespace/cache.py`

 * *Files identical despite different names*

### Comparing `coveragespace-6.0.2/coveragespace/cli.py` & `coveragespace-6.1/coveragespace/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -73,27 +73,38 @@
         response = api.delete(slug)
     else:
         data = {metric: value or coverage.get_coverage(always=launch)}
         response = api.put(slug, data)
 
     if response.status_code == 200:
         if verbose or launch:
-            display("coverage updated", response.json(), colorama.Fore.GREEN)
+            data = response.json()
+            report = coverage.get_report()
+            if report:
+                data["report"] = report
+            display("coverage updated", data, colorama.Fore.GREEN)
         if launch:
             coverage.launch_report(always=True)
         return True
 
     if response.status_code == 202:
-        display("coverage reset", response.json(), colorama.Fore.BLUE)
+        data = response.json()
+        report = coverage.get_report()
+        if report:
+            data["report"] = report
+        display("coverage reset", data, colorama.Fore.BLUE)
         return True
 
     if response.status_code == 422:
         color = colorama.Fore.RED if hardfail else colorama.Fore.YELLOW
         data = response.json()
         prefix = "poetry run " if environments.poetry() else ""
+        report = coverage.get_report()
+        if report:
+            data["report"] = report
         data["help"] = f"To reset metrics, run: ^{prefix}coveragespace reset$"  # type: ignore
         display("coverage decreased", data, color)
         coverage.launch_report(always=launch)
         return False
 
     try:
         data = response.json()
```

### Comparing `coveragespace-6.0.2/coveragespace/coverage.py` & `coveragespace-6.1/coveragespace/coverage.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,23 @@
     if plugin is None:
         return 0.0
 
     percentage = plugin.get_coverage(cwd)
     return round(percentage, 1)
 
 
+def get_report(cwd=None):
+    """Get the full path to the coverage report.."""
+    cwd = cwd or os.getcwd()
+
+    plugin = _find_plugin(cwd, allow_missing=True)
+
+    return plugin.get_report(cwd) if plugin else None
+
+
 def launch_report(cwd=None, *, always=False):
     """Open the generated coverage report in a web browser."""
     cwd = cwd or os.getcwd()
 
     plugin = _find_plugin(cwd, allow_missing=True)
 
     if plugin:
```

### Comparing `coveragespace-6.0.2/coveragespace/repository.py` & `coveragespace-6.1/coveragespace/repository.py`

 * *Files identical despite different names*

### Comparing `coveragespace-6.0.2/coveragespace/tests/test_cache.py` & `coveragespace-6.1/coveragespace/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `coveragespace-6.0.2/coveragespace/tests/test_cli.py` & `coveragespace-6.1/coveragespace/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `coveragespace-6.0.2/coveragespace/tests/test_coverage.py` & `coveragespace-6.1/coveragespace/tests/test_coverage.py`

 * *Files identical despite different names*

### Comparing `coveragespace-6.0.2/coveragespace/tests/test_environments.py` & `coveragespace-6.1/coveragespace/tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `coveragespace-6.0.2/coveragespace/tests/test_repository.py` & `coveragespace-6.1/coveragespace/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `coveragespace-6.0.2/pyproject.toml` & `coveragespace-6.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "coveragespace"
-version = "6.0.2"
+version = "6.1"
 description = "A place to track your code coverage metrics."
 
 license = "MIT"
 
 authors = ["Jace Browning <jacebrowning@gmail.com>"]
 
 readme = "README.md"
@@ -48,15 +48,15 @@
 [tool.poetry.dev-dependencies]
 
 # Formatters
 black = "^22.6"
 isort = "^5.10"
 
 # Linters
-mypy = "*"
+mypy = "^1.7.1"
 pydocstyle = "*"
 pylint = "^2.6"
 types-requests = "*"
 types-setuptools = "*"
 
 # Testing
 pytest = "^7.0"
@@ -64,15 +64,15 @@
 pytest-describe = "^2.0"
 pytest-expecter = "*"
 pytest-random = "*"
 scripttest = "*"
 
 # Documentation
 mkdocs = "^1.4"
-pygments = "^2.9"
+pygments = "^2.15"
 
 # Tooling
 pyinstaller = "*"
 sniffer = "*"
 MacFSEvents = { version = "*", platform = "darwin" }
 pync = { version = "*", platform = "darwin" }
```

### Comparing `coveragespace-6.0.2/PKG-INFO` & `coveragespace-6.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coveragespace
-Version: 6.0.2
+Version: 6.1
 Summary: A place to track your code coverage metrics.
 Home-page: https://coverage.space/client/
 License: MIT
 Keywords: coverage,testing,command-line
 Author: Jace Browning
 Author-email: jacebrowning@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -12,17 +12,19 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Requires-Dist: colorama (>=0.4)
 Requires-Dist: coverage (>=4.0)
 Requires-Dist: docopt (>=0.6)
 Requires-Dist: minilog (>=2.0)
@@ -31,16 +33,15 @@
 Project-URL: Repository, https://github.com/jacebrowning/coverage-space-cli
 Description-Content-Type: text/markdown
 
 # Overview
 
 The official command-line client for [The Coverage Space](http://coverage.space).
 
-[![Unix Build Status](https://img.shields.io/travis/jacebrowning/coverage-space-cli/main.svg?label=unix)](https://travis-ci.org/jacebrowning/coverage-space-cli)
-[![Windows Build Status](https://img.shields.io/appveyor/ci/jacebrowning/coverage-space-cli/main.svg?label=window)](https://ci.appveyor.com/project/jacebrowning/coverage-space-cli)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/jacebrowning/coverage-space-cli/main.yml?branch=main&label=build)](https://github.com/jacebrowning/coverage-space-cli/actions)
 [![Coverage Status](https://img.shields.io/coveralls/jacebrowning/coverage-space-cli/main.svg)](https://coveralls.io/r/jacebrowning/coverage-space-cli)
 [![Scrutinizer Code Quality](https://img.shields.io/scrutinizer/g/jacebrowning/coverage-space-cli.svg)](https://scrutinizer-ci.com/g/jacebrowning/coverage-space-cli/?branch=main)
 [![PyPI Version](https://img.shields.io/pypi/v/coveragespace.svg)](https://pypi.org/project/coveragespace)
 [![PyPI License](https://img.shields.io/pypi/l/coveragespace.svg)](https://pypi.org/project/coveragespace)
 
 # Setup
```

