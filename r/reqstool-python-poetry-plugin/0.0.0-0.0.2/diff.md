# Comparing `tmp/reqstool_python_poetry_plugin-0.0.0.tar.gz` & `tmp/reqstool_python_poetry_plugin-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reqstool_python_poetry_plugin-0.0.0.tar", max compression
+gzip compressed data, was "reqstool_python_poetry_plugin-0.0.2.tar", max compression
```

## Comparing `reqstool_python_poetry_plugin-0.0.0.tar` & `reqstool_python_poetry_plugin-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1060 2024-03-26 15:05:22.015888 reqstool_python_poetry_plugin-0.0.0/LICENSE
--rw-r--r--   0        0        0     3149 2024-03-26 15:05:22.015888 reqstool_python_poetry_plugin-0.0.0/README.md
--rw-r--r--   0        0        0     1650 2024-03-26 15:05:22.015888 reqstool_python_poetry_plugin-0.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-26 15:05:22.015888 reqstool_python_poetry_plugin-0.0.0/src/reqstool_python_poetry_plugin/__init__.py
--rw-r--r--   0        0        0      844 2024-03-26 15:05:22.015888 reqstool_python_poetry_plugin-0.0.0/src/reqstool_python_poetry_plugin/plugin.py
--rw-r--r--   0        0        0     4097 1970-01-01 00:00:00.000000 reqstool_python_poetry_plugin-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-04-05 09:08:29.760857 reqstool_python_poetry_plugin-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3149 2024-04-05 09:08:29.760857 reqstool_python_poetry_plugin-0.0.2/README.md
+-rw-r--r--   0        0        0     1643 2024-04-05 09:08:44.040896 reqstool_python_poetry_plugin-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-05 09:08:29.760857 reqstool_python_poetry_plugin-0.0.2/src/reqstool_python_poetry_plugin/__init__.py
+-rw-r--r--   0        0        0      844 2024-04-05 09:08:29.760857 reqstool_python_poetry_plugin-0.0.2/src/reqstool_python_poetry_plugin/plugin.py
+-rw-r--r--   0        0        0     4148 1970-01-01 00:00:00.000000 reqstool_python_poetry_plugin-0.0.2/PKG-INFO
```

### Comparing `reqstool_python_poetry_plugin-0.0.0/LICENSE` & `reqstool_python_poetry_plugin-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reqstool_python_poetry_plugin-0.0.0/README.md` & `reqstool_python_poetry_plugin-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `reqstool_python_poetry_plugin-0.0.0/pyproject.toml` & `reqstool_python_poetry_plugin-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
-build-backend = 'poetry_dynamic_versioning.backend'
+build-backend = "poetry_dynamic_versioning.backend"
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
 
 
 [tool.poetry]
 name = "reqstool-python-poetry-plugin"
-version = "0.0.0"
+version = "0.0.2"
 description = "Reqstool Python Poetry Plugin"
 authors = ["LFV SYSDEV <sysdev@lfv.com>"]
 license = "MIT License"
 readme = "README.md"
 repository = "https://github.com/Luftfartsverket/reqstool-python-poetry-plugin.git"
 homepage = "https://github.com/Luftfartsverket/reqstool-python-poetry-plugin.git"
 documentation = "https://github.com/Luftfartsverket/reqstool-python-poetry-plugin.git"
@@ -21,23 +21,24 @@
 ]
 
 [project.scripts]
 # section needed for poetry convertion
 
 [tool.poetry.dependencies]
 python = "^3.10"
-poetry = "^1.7.1"
-reqstool-python-decorators = "0.0.3" #Change later when proper release is made. 
+poetry = "1.7.1"
+reqstool-python-decorators = "0.0.4"
+poetry-dynamic-versioning = "^1.2.0"
 
 [tool.poetry.group.dev.dependencies]
-black = { version = "24.2.0" }
+black = { version = "24.3.0" }
 flake8 = { version = "7.0.0" }
 flake8-pyproject = { version = "1.2.3" }
 pytest = { version = "8.1.1" }
-pytest-cov = { version = "4.1.0" }
+pytest-cov = { version = "5.0.0" }
 
 [tool.poetry.plugins."poetry.plugin"]
 reqstool = "reqstool_python_poetry_plugin.plugin:DecoratorsPlugin"
 
 [tool.pytest.ini_options]
 addopts = ["-s", "--import-mode=importlib"]
 pythonpath = [".", "src", "tests"]
@@ -50,10 +51,10 @@
 [tool.flake8]
 ignore = ["W503"]
 max-line-length = 120
 max-complexity = 10
 
 
 [tool.poetry-dynamic-versioning]
-enable = true
+enable = false
 vcs = "git"
 style = "pep440"
```

### Comparing `reqstool_python_poetry_plugin-0.0.0/src/reqstool_python_poetry_plugin/plugin.py` & `reqstool_python_poetry_plugin-0.0.2/src/reqstool_python_poetry_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `reqstool_python_poetry_plugin-0.0.0/PKG-INFO` & `reqstool_python_poetry_plugin-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: reqstool-python-poetry-plugin
-Version: 0.0.0
+Version: 0.0.2
 Summary: Reqstool Python Poetry Plugin
 Home-page: https://github.com/Luftfartsverket/reqstool-python-poetry-plugin.git
 License: MIT
 Author: LFV SYSDEV
 Author-email: sysdev@lfv.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: poetry (>=1.7.1,<2.0.0)
-Requires-Dist: reqstool-python-decorators (==0.0.3)
+Requires-Dist: poetry (==1.7.1)
+Requires-Dist: poetry-dynamic-versioning (>=1.2.0,<2.0.0)
+Requires-Dist: reqstool-python-decorators (==0.0.4)
 Project-URL: Documentation, https://github.com/Luftfartsverket/reqstool-python-poetry-plugin.git
 Project-URL: Repository, https://github.com/Luftfartsverket/reqstool-python-poetry-plugin.git
 Description-Content-Type: text/markdown
 
 
 [![Commit Activity](https://img.shields.io/github/commit-activity/m/Luftfartsverket/reqstool-python-poetry-plugin?label=commits&style=for-the-badge)](https://github.com/Luftfartsverket/reqstool-python-poetry-plugin/pulse)
 [![GitHub Issues](https://img.shields.io/github/issues/Luftfartsverket/reqstool-python-poetry-plugin?style=for-the-badge&logo=github)](https://github.com/Luftfartsverket/reqstool-python-poetry-plugin/issues)
```

