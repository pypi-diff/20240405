# Comparing `tmp/lidipy-0.1.1.tar.gz` & `tmp/lidipy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lidipy-0.1.1.tar", max compression
+gzip compressed data, was "lidipy-0.2.0.tar", max compression
```

## Comparing `lidipy-0.1.1.tar` & `lidipy-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-06-01 10:35:45.704356 lidipy-0.1.1/LICENSE
--rw-r--r--   0        0        0     4075 2023-06-01 10:35:45.704356 lidipy-0.1.1/README.md
--rw-r--r--   0        0        0      973 2023-06-01 10:35:45.704356 lidipy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       36 2023-06-01 10:35:45.704356 lidipy-0.1.1/src/lidipy/__init__.py
--rw-r--r--   0        0        0     1446 2023-06-01 10:35:45.704356 lidipy-0.1.1/src/lidipy/container.py
--rw-r--r--   0        0        0       96 2023-06-01 10:35:45.704356 lidipy-0.1.1/src/lidipy/exceptions.py
--rw-r--r--   0        0        0     4470 1970-01-01 00:00:00.000000 lidipy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-05 11:16:57.679618 lidipy-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4722 2024-04-05 11:16:57.679618 lidipy-0.2.0/README.md
+-rw-r--r--   0        0        0     1185 2024-04-05 11:16:57.679618 lidipy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       36 2024-04-05 11:16:57.679618 lidipy-0.2.0/src/lidipy/__init__.py
+-rw-r--r--   0        0        0     3733 2024-04-05 11:16:57.679618 lidipy-0.2.0/src/lidipy/container.py
+-rw-r--r--   0        0        0      333 2024-04-05 11:16:57.679618 lidipy-0.2.0/src/lidipy/exceptions.py
+-rw-r--r--   0        0        0     5168 1970-01-01 00:00:00.000000 lidipy-0.2.0/PKG-INFO
```

### Comparing `lidipy-0.1.1/LICENSE` & `lidipy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lidipy-0.1.1/README.md` & `lidipy-0.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,13 @@
+[![Build status](https://github.com/altosterino/lidi/actions/workflows/push-test.yml/badge.svg)](https://github.com/altosterino/lidi/)
 [![Coverage Status](https://coveralls.io/repos/github/AlTosterino/Lidi/badge.svg?branch=main)](https://coveralls.io/github/AlTosterino/Lidi?branch=main)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 
 # Lidi (LIghtweight Dependency Injector)
 
 Lidi is a lightweight dependency injector designed to simplify dependency management in your Python projects.
 It provides a simple and intuitive API for binding classes and resolving dependencies.
 
 ## Installation
```

### Comparing `lidipy-0.1.1/pyproject.toml` & `lidipy-0.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "lidipy"
-version = "0.1.1"
+version = "0.2.0"
 description = "Lidi is a lightweight dependency injector designed to simplify dependency management in your Python projects."
 authors = ["AlTosterino <altosterino@gmail.com>"]
 readme = "README.md"
 packages = [{include = "lidipy", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.0.261"
-black = "^23.3.0"
-pytest = "^7.3.0"
-mypy = "^1.2.0"
+ruff = "~0"
+black = "~24"
+pytest = "~8"
+mypy = "~1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 # THIRD PARTY
@@ -35,10 +35,17 @@
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 check_untyped_defs = true
 ignore_missing_imports = true
 
 [tool.ruff]
-select = ["E", "F", "I", "PL"]
-line-length = 100
-target-version = "py311"
+line-length = 110
+target-version = "py311"
+
+[tool.ruff.lint]
+select = ["E", "F", "I", "PL", "N", "S", "B", "A", "TD", "FIX", "PERF", "PT"]
+ignore = ["D107", "D203", "D211"]
+
+[tool.ruff.lint.per-file-ignores]
+"__init__.py" = ["E402", "D104"]
+"**/{tests,docs,tools}/**" = ["D100", "D101", "D103", "S101"]
```

### Comparing `lidipy-0.1.1/PKG-INFO` & `lidipy-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 Metadata-Version: 2.1
 Name: lidipy
-Version: 0.1.1
+Version: 0.2.0
 Summary: Lidi is a lightweight dependency injector designed to simplify dependency management in your Python projects.
 Author: AlTosterino
 Author-email: altosterino@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
+[![Build status](https://github.com/altosterino/lidi/actions/workflows/push-test.yml/badge.svg)](https://github.com/altosterino/lidi/)
 [![Coverage Status](https://coveralls.io/repos/github/AlTosterino/Lidi/badge.svg?branch=main)](https://coveralls.io/github/AlTosterino/Lidi?branch=main)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 
 # Lidi (LIghtweight Dependency Injector)
 
 Lidi is a lightweight dependency injector designed to simplify dependency management in your Python projects.
 It provides a simple and intuitive API for binding classes and resolving dependencies.
 
 ## Installation
```

