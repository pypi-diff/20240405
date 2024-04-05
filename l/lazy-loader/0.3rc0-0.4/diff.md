# Comparing `tmp/lazy_loader-0.3rc0.tar.gz` & `tmp/lazy_loader-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_loader-0.3rc0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lazy_loader-0.4.tar", last modified: Fri Apr  5 13:03:04 2024, max compression
```

## Comparing `lazy_loader-0.3rc0.tar` & `lazy_loader-0.4.tar`

### file list

```diff
@@ -1,18 +1,24 @@
--rw-r--r--   0        0        0      207 2023-06-28 01:54:21.971546 lazy_loader-0.3rc0/.github/dependabot.yml
--rw-r--r--   0        0        0      998 2023-06-08 18:17:17.686092 lazy_loader-0.3rc0/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      830 2023-06-08 18:17:17.686092 lazy_loader-0.3rc0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      994 2023-06-27 19:28:19.549616 lazy_loader-0.3rc0/.github/workflows/test.yml
--rw-r--r--   0        0        0      318 2023-06-08 18:17:17.686092 lazy_loader-0.3rc0/.gitignore
--rw-r--r--   0        0        0     1025 2023-06-28 01:54:21.971546 lazy_loader-0.3rc0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     6916 2023-06-30 20:16:43.694958 lazy_loader-0.3rc0/CHANGELOG.md
--rw-r--r--   0        0        0     1539 2023-06-08 18:17:17.686092 lazy_loader-0.3rc0/LICENSE.md
--rw-r--r--   0        0        0     3361 2023-06-28 01:54:21.971546 lazy_loader-0.3rc0/README.md
--rw-r--r--   0        0        0     1419 2023-06-08 18:17:17.686092 lazy_loader-0.3rc0/RELEASE.md
--rw-r--r--   0        0        0     8555 2023-06-28 01:54:21.972546 lazy_loader-0.3rc0/lazy_loader/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 18:17:17.686092 lazy_loader-0.3rc0/lazy_loader/tests/__init__.py
--rw-r--r--   0        0        0      136 2023-06-08 18:17:17.687091 lazy_loader-0.3rc0/lazy_loader/tests/fake_pkg/__init__.py
--rw-r--r--   0        0        0       33 2023-06-27 20:26:36.582245 lazy_loader-0.3rc0/lazy_loader/tests/fake_pkg/__init__.pyi
--rw-r--r--   0        0        0       74 2023-06-08 18:17:17.687091 lazy_loader-0.3rc0/lazy_loader/tests/fake_pkg/some_func.py
--rw-r--r--   0        0        0     4468 2023-06-28 01:54:21.972546 lazy_loader-0.3rc0/lazy_loader/tests/test_lazy_loader.py
--rw-r--r--   0        0        0     1192 2023-06-30 20:17:15.640112 lazy_loader-0.3rc0/pyproject.toml
--rw-r--r--   0        0        0     4312 1970-01-01 00:00:00.000000 lazy_loader-0.3rc0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:03:04.227013 lazy_loader-0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    12593 2024-04-05 13:02:52.000000 lazy_loader-0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-05 13:02:52.000000 lazy_loader-0.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 13:02:52.000000 lazy_loader-0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-05 13:03:04.227013 lazy_loader-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-04-05 13:02:52.000000 lazy_loader-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:03:04.227013 lazy_loader-0.4/lazy_loader/
+-rw-r--r--   0 runner    (1001) docker     (127)    10952 2024-04-05 13:02:52.000000 lazy_loader-0.4/lazy_loader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:03:04.227013 lazy_loader-0.4/lazy_loader/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:02:52.000000 lazy_loader-0.4/lazy_loader/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:03:04.227013 lazy_loader-0.4/lazy_loader/tests/fake_pkg/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-05 13:02:52.000000 lazy_loader-0.4/lazy_loader/tests/fake_pkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 13:02:52.000000 lazy_loader-0.4/lazy_loader/tests/fake_pkg/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-05 13:02:52.000000 lazy_loader-0.4/lazy_loader/tests/fake_pkg/some_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-05 13:02:52.000000 lazy_loader-0.4/lazy_loader/tests/import_np_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-05 13:02:52.000000 lazy_loader-0.4/lazy_loader/tests/test_lazy_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:03:04.227013 lazy_loader-0.4/lazy_loader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-05 13:03:04.000000 lazy_loader-0.4/lazy_loader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-05 13:03:04.000000 lazy_loader-0.4/lazy_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:03:04.000000 lazy_loader-0.4/lazy_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-05 13:03:04.000000 lazy_loader-0.4/lazy_loader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 13:03:04.000000 lazy_loader-0.4/lazy_loader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-05 13:02:52.000000 lazy_loader-0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:03:04.227013 lazy_loader-0.4/setup.cfg
```

### Comparing `lazy_loader-0.3rc0/LICENSE.md` & `lazy_loader-0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lazy_loader-0.3rc0/lazy_loader/__init__.py` & `lazy_loader-0.4/lazy_loader/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 """
 lazy_loader
 ===========
 
 Makes it easy to load subpackages and functions on demand.
 """
+
 import ast
 import importlib
 import importlib.util
-import inspect
 import os
 import sys
+import threading
 import types
 import warnings
 
+__version__ = "0.4"
 __all__ = ["attach", "load", "attach_stub"]
 
 
+threadlock = threading.Lock()
+
+
 def attach(package_name, submodules=None, submod_attrs=None):
     """Attach lazily loaded submodules, functions, or other attributes.
 
     Typically, modules import submodules and attributes as follows::
 
       import mysubmodule
       import anothersubmodule
@@ -95,32 +100,33 @@
         for attr in set(attr_to_modules.keys()) | submodules:
             __getattr__(attr)
 
     return __getattr__, __dir__, list(__all__)
 
 
 class DelayedImportErrorModule(types.ModuleType):
-    def __init__(self, frame_data, *args, **kwargs):
+    def __init__(self, frame_data, *args, message, **kwargs):
         self.__frame_data = frame_data
+        self.__message = message
         super().__init__(*args, **kwargs)
 
     def __getattr__(self, x):
-        if x in ("__class__", "__file__", "__frame_data"):
+        if x in ("__class__", "__file__", "__frame_data", "__message"):
             super().__getattr__(x)
         else:
             fd = self.__frame_data
             raise ModuleNotFoundError(
-                f"No module named '{fd['spec']}'\n\n"
+                f"{self.__message}\n\n"
                 "This error is lazily reported, having originally occured in\n"
                 f'  File {fd["filename"]}, line {fd["lineno"]}, in {fd["function"]}\n\n'
-                f'----> {"".join(fd["code_context"]).strip()}'
+                f'----> {"".join(fd["code_context"] or "").strip()}'
             )
 
 
-def load(fullname, error_on_import=False):
+def load(fullname, *, require=None, error_on_import=False):
     """Return a lazily imported proxy for a module.
 
     We often see the following pattern::
 
       def myfunc():
           import numpy as np
           np.norm(...)
@@ -156,80 +162,152 @@
     Parameters
     ----------
     fullname : str
         The full name of the module or submodule to import.  For example::
 
           sp = lazy.load('scipy')  # import scipy as sp
 
+    require : str
+        A dependency requirement as defined in PEP-508.  For example::
+
+          "numpy >=1.24"
+
+        If defined, the proxy module will raise an error if the installed
+        version does not satisfy the requirement.
+
     error_on_import : bool
         Whether to postpone raising import errors until the module is accessed.
         If set to `True`, import errors are raised as soon as `load` is called.
 
     Returns
     -------
     pm : importlib.util._LazyModule
         Proxy module.  Can be used like any regularly imported module.
         Actual loading of the module occurs upon first attribute request.
 
     """
-    try:
-        return sys.modules[fullname]
-    except KeyError:
-        pass
-
-    if "." in fullname:
-        msg = (
-            "subpackages can technically be lazily loaded, but it causes the "
-            "package to be eagerly loaded even if it is already lazily loaded."
-            "So, you probably shouldn't use subpackages with this lazy feature."
-        )
-        warnings.warn(msg, RuntimeWarning)
-
-    spec = importlib.util.find_spec(fullname)
-    if spec is None:
-        if error_on_import:
-            raise ModuleNotFoundError(f"No module named '{fullname}'")
-        else:
+    with threadlock:
+        module = sys.modules.get(fullname)
+        have_module = module is not None
+
+        # Most common, short-circuit
+        if have_module and require is None:
+            return module
+
+        if "." in fullname:
+            msg = (
+                "subpackages can technically be lazily loaded, but it causes the "
+                "package to be eagerly loaded even if it is already lazily loaded."
+                "So, you probably shouldn't use subpackages with this lazy feature."
+            )
+            warnings.warn(msg, RuntimeWarning)
+
+        spec = None
+
+        if not have_module:
+            spec = importlib.util.find_spec(fullname)
+            have_module = spec is not None
+
+        if not have_module:
+            not_found_message = f"No module named '{fullname}'"
+        elif require is not None:
+            try:
+                have_module = _check_requirement(require)
+            except ModuleNotFoundError as e:
+                raise ValueError(
+                    f"Found module '{fullname}' but cannot test "
+                    "requirement '{require}'. "
+                    "Requirements must match distribution name, not module name."
+                ) from e
+
+            not_found_message = f"No distribution can be found matching '{require}'"
+
+        if not have_module:
+            if error_on_import:
+                raise ModuleNotFoundError(not_found_message)
+            import inspect
+
             try:
                 parent = inspect.stack()[1]
                 frame_data = {
-                    "spec": fullname,
                     "filename": parent.filename,
                     "lineno": parent.lineno,
                     "function": parent.function,
                     "code_context": parent.code_context,
                 }
-                return DelayedImportErrorModule(frame_data, "DelayedImportErrorModule")
+                return DelayedImportErrorModule(
+                    frame_data,
+                    "DelayedImportErrorModule",
+                    message=not_found_message,
+                )
             finally:
                 del parent
 
-    module = importlib.util.module_from_spec(spec)
-    sys.modules[fullname] = module
+        if spec is not None:
+            module = importlib.util.module_from_spec(spec)
+            sys.modules[fullname] = module
 
-    loader = importlib.util.LazyLoader(spec.loader)
-    loader.exec_module(module)
+            loader = importlib.util.LazyLoader(spec.loader)
+            loader.exec_module(module)
 
     return module
 
 
+def _check_requirement(require: str) -> bool:
+    """Verify that a package requirement is satisfied
+
+    If the package is required, a ``ModuleNotFoundError`` is raised
+    by ``importlib.metadata``.
+
+    Parameters
+    ----------
+    require : str
+        A dependency requirement as defined in PEP-508
+
+    Returns
+    -------
+    satisfied : bool
+        True if the installed version of the dependency matches
+        the specified version, False otherwise.
+    """
+    import packaging.requirements
+
+    try:
+        import importlib.metadata as importlib_metadata
+    except ImportError:  # PY37
+        import importlib_metadata
+
+    req = packaging.requirements.Requirement(require)
+    return req.specifier.contains(
+        importlib_metadata.version(req.name),
+        prereleases=True,
+    )
+
+
 class _StubVisitor(ast.NodeVisitor):
     """AST visitor to parse a stub file for submodules and submod_attrs."""
 
     def __init__(self):
         self._submodules = set()
         self._submod_attrs = {}
 
     def visit_ImportFrom(self, node: ast.ImportFrom):
         if node.level != 1:
             raise ValueError(
                 "Only within-module imports are supported (`from .* import`)"
             )
         if node.module:
             attrs: list = self._submod_attrs.setdefault(node.module, [])
-            attrs.extend(alias.name for alias in node.names)
+            aliases = [alias.name for alias in node.names]
+            if "*" in aliases:
+                raise ValueError(
+                    "lazy stub loader does not support star import "
+                    f"`from {node.module} import *`"
+                )
+            attrs.extend(aliases)
         else:
             self._submodules.update(alias.name for alias in node.names)
 
 
 def attach_stub(package_name: str, filename: str):
     """Attach lazily loaded submodules, functions from a type stub.
```

### Comparing `lazy_loader-0.3rc0/pyproject.toml` & `lazy_loader-0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,50 @@
 [build-system]
-requires = ["flit_core >=3.8,<4"]
-build-backend = "flit_core.buildapi"
+requires = ["setuptools>=61.2"]
+build-backend = "setuptools.build_meta"
 
 [project]
 name = "lazy_loader"
-version = "0.3rc0"
 requires-python = ">=3.7"
 authors = [{name = "Scientific Python Developers"}]
 readme = "README.md"
 license = {file = "LICENSE.md"}
+dynamic = ['version']
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: BSD License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
-dynamic = ["description"]
-
+description = "Makes it easy to load subpackages and functions on demand."
+dependencies = [
+  "packaging",
+  "importlib_metadata; python_version < '3.8'",
+]
 
 [project.optional-dependencies]
 test = ["pytest >= 7.4", "pytest-cov >= 4.1"]
-lint = ["pre-commit >= 3.3"]
+lint = ["pre-commit == 3.7.0"]
+dev = ["changelist == 0.5"]
 
 [project.urls]
 Home = "https://scientific-python.org/specs/spec-0001/"
 Source = "https://github.com/scientific-python/lazy_loader"
 
-[tool.flit.sdist]
-exclude = ["tests/*"]
+
+[tool.changelist]
+ignored_user_logins = ["dependabot[bot]", "pre-commit-ci[bot]", "web-flow"]
+
+[tool.setuptools.dynamic.version]
+attr = 'lazy_loader.__version__'
 
 [tool.ruff]
 line-length = 88
 target-version = "py37"
 select = [
     "C",
     "E",
```

### Comparing `lazy_loader-0.3rc0/PKG-INFO` & `lazy_loader-0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: lazy_loader
-Version: 0.3rc0
-Summary: lazy_loader
-Author: Scientific Python Developers
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pre-commit >= 3.3 ; extra == "lint"
-Requires-Dist: pytest >= 7.4 ; extra == "test"
-Requires-Dist: pytest-cov >= 4.1 ; extra == "test"
-Project-URL: Home, https://scientific-python.org/specs/spec-0001/
-Project-URL: Source, https://github.com/scientific-python/lazy_loader
-Provides-Extra: lint
-Provides-Extra: test
-
 [![PyPI](https://img.shields.io/pypi/v/lazy_loader)](https://pypi.org/project/lazy_loader/)
 [![Test status](https://github.com/scientific-python/lazy_loader/workflows/test/badge.svg?branch=main)](https://github.com/scientific-python/lazy_loader/actions?query=workflow%3A%22test%22)
 [![Test coverage](https://codecov.io/gh/scientific-python/lazy_loader/branch/main/graph/badge.svg)](https://app.codecov.io/gh/scientific-python/lazy_loader/branch/main)
 
 `lazy_loader` makes it easy to load subpackages and functions on demand.
 
 ## Motivation
@@ -37,14 +13,19 @@
 
 ## Installation
 
 ```
 pip install -U lazy_loader
 ```
 
+We recommend using `lazy_loader` with Python >= 3.11.
+If using Python 3.11, please upgrade to 3.11.9 or later.
+If using Python 3.12, please upgrade to 3.12.3 or later.
+These versions [avoid](https://github.com/python/cpython/pull/114781) a [known race condition](https://github.com/python/cpython/issues/114763).
+
 ## Usage
 
 ### Lazily load subpackages
 
 Consider the `__init__.py` from [scikit-image](https://scikit-image.org):
 
 ```python
@@ -135,11 +116,33 @@
 _Note that lazily importing *sub*packages,
 i.e. `load('scipy.linalg')` will cause the package containing the
 subpackage to be imported immediately; thus, this usage is
 discouraged._
 
 You can ask `lazy.load` to raise import errors as soon as it is called:
 
-```
+```python
 linalg = lazy.load('scipy.linalg', error_on_import=True)
 ```
 
+#### Optional requirements
+
+One use for lazy loading is for loading optional dependencies, with
+`ImportErrors` only arising when optional functionality is accessed. If optional
+functionality depends on a specific version, a version requirement can
+be set:
+
+```python
+np = lazy.load("numpy", require="numpy >=1.24")
+```
+
+In this case, if `numpy` is installed, but the version is less than 1.24,
+the `np` module returned will raise an error on attribute access. Using
+this feature is not all-or-nothing: One module may rely on one version of
+numpy, while another module may not set any requirement.
+
+_Note that the requirement must use the package [distribution name][] instead
+of the module [import name][]. For example, the `pyyaml` distribution provides
+the `yaml` module for import._
+
+[distribution name]: https://packaging.python.org/en/latest/glossary/#term-Distribution-Package
+[import name]: https://packaging.python.org/en/latest/glossary/#term-Import-Package
```

