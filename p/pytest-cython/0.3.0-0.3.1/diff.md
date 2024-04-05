# Comparing `tmp/pytest-cython-0.3.0.tar.gz` & `tmp/pytest-cython-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-cython-0.3.0.tar", last modified: Mon Apr  1 10:58:02 2024, max compression
+gzip compressed data, was "pytest-cython-0.3.1.tar", last modified: Fri Apr  5 14:23:28 2024, max compression
```

## Comparing `pytest-cython-0.3.0.tar` & `pytest-cython-0.3.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:58:02.660092 pytest-cython-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-01 10:58:02.660092 pytest-cython-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:58:02.656092 pytest-cython-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-01 10:58:02.660092 pytest-cython-0.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1580 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:58:02.652092 pytest-cython-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:58:02.656092 pytest-cython-0.3.0/src/pytest_cython/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/src/pytest_cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/src/pytest_cython/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:58:02.656092 pytest-cython-0.3.0/src/pytest_cython.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-01 10:58:02.000000 pytest-cython-0.3.0/src/pytest_cython.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-01 10:58:02.000000 pytest-cython-0.3.0/src/pytest_cython.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 10:58:02.000000 pytest-cython-0.3.0/src/pytest_cython.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-01 10:58:02.000000 pytest-cython-0.3.0/src/pytest_cython.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 10:58:02.000000 pytest-cython-0.3.0/src/pytest_cython.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 10:58:02.000000 pytest-cython-0.3.0/src/pytest_cython.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 10:58:02.000000 pytest-cython-0.3.0/src/pytest_cython.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:58:02.656092 pytest-cython-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:58:02.656092 pytest-cython-0.3.0/tests/example-project/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/tests/example-project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/tests/example-project/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:58:02.652092 pytest-cython-0.3.0/tests/example-project/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:58:02.656092 pytest-cython-0.3.0/tests/example-project/src/clib/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/tests/example-project/src/clib/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/tests/example-project/src/clib/sqrc.c
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/tests/example-project/src/clib/sqrcpp.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:58:02.656092 pytest-cython-0.3.0/tests/example-project/src/pypackage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/tests/example-project/src/pypackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/tests/example-project/src/pypackage/cython_ext_module.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/tests/example-project/src/pypackage/cython_ext_module.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/tests/example-project/src/pypackage/pure_py_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/tests/example-project/src/pypackage/wrap_c_ext_module.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/tests/example-project/src/pypackage/wrap_cpp_ext_module.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-01 10:57:58.000000 pytest-cython-0.3.0/tests/test_pytest_cython.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:23:28.302485 pytest-cython-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-05 14:23:28.302485 pytest-cython-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:23:28.298485 pytest-cython-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-05 14:23:28.302485 pytest-cython-0.3.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1580 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:23:28.294485 pytest-cython-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:23:28.298485 pytest-cython-0.3.1/src/pytest_cython/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/src/pytest_cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/src/pytest_cython/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:23:28.302485 pytest-cython-0.3.1/src/pytest_cython.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-05 14:23:28.000000 pytest-cython-0.3.1/src/pytest_cython.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-05 14:23:28.000000 pytest-cython-0.3.1/src/pytest_cython.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:23:28.000000 pytest-cython-0.3.1/src/pytest_cython.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-05 14:23:28.000000 pytest-cython-0.3.1/src/pytest_cython.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:23:28.000000 pytest-cython-0.3.1/src/pytest_cython.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 14:23:28.000000 pytest-cython-0.3.1/src/pytest_cython.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 14:23:28.000000 pytest-cython-0.3.1/src/pytest_cython.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:23:28.298485 pytest-cython-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:23:28.298485 pytest-cython-0.3.1/tests/example-project/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/tests/example-project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/tests/example-project/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:23:28.294485 pytest-cython-0.3.1/tests/example-project/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:23:28.302485 pytest-cython-0.3.1/tests/example-project/src/clib/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/tests/example-project/src/clib/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/tests/example-project/src/clib/sqrc.c
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/tests/example-project/src/clib/sqrcpp.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:23:28.302485 pytest-cython-0.3.1/tests/example-project/src/pypackage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/tests/example-project/src/pypackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/tests/example-project/src/pypackage/cython_ext_module.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/tests/example-project/src/pypackage/cython_ext_module.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/tests/example-project/src/pypackage/pure_py_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/tests/example-project/src/pypackage/wrap_c_ext_module.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/tests/example-project/src/pypackage/wrap_cpp_ext_module.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-05 14:23:23.000000 pytest-cython-0.3.1/tests/test_pytest_cython.py
```

### Comparing `pytest-cython-0.3.0/CHANGELOG.md` & `pytest-cython-0.3.1/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 0.2.2 Onwards
+
+Please see the [GitHub releases](https://github.com/lgpage/pytest-cython/releases) for what has changed
+
 ## 0.2.1
 
 The full list of merged changes is:
 
 - #26: fix: pytest_collect_file to take into account pytest fspath deprecation in Node constructors
 - #29: chore: use GitHub workflows in place of Travis
 - #30: chore: use markdown project files
```

### Comparing `pytest-cython-0.3.0/CODE_OF_CONDUCT.md` & `pytest-cython-0.3.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pytest-cython-0.3.0/CONTRIBUTING.md` & `pytest-cython-0.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pytest-cython-0.3.0/LICENSE.md` & `pytest-cython-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pytest-cython-0.3.0/PKG-INFO` & `pytest-cython-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-cython
-Version: 0.3.0
+Version: 0.3.1
 Summary: A plugin for testing Cython extension modules
 Home-page: https://github.com/lgpage/pytest-cython
 Author: Logan Page
 Author-email: page.lg@gmail.com
 License: MIT
 Keywords: pytest,py.test,cython,doctest
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pytest-cython-0.3.0/README.md` & `pytest-cython-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest-cython-0.3.0/docs/conf.py` & `pytest-cython-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytest-cython-0.3.0/noxfile.py` & `pytest-cython-0.3.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `pytest-cython-0.3.0/setup.cfg` & `pytest-cython-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest-cython-0.3.0/setup.py` & `pytest-cython-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 with open(path.join(this_directory, 'README.md')) as readme_file:
     long_description = readme_file.read()
 
 
 setup(
     name='pytest-cython',
-    version='0.3.0',
+    version='0.3.1',
     description='A plugin for testing Cython extension modules',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Logan Page',
     author_email='page.lg@gmail.com',
     license='MIT',
     url='https://github.com/lgpage/pytest-cython',
```

### Comparing `pytest-cython-0.3.0/src/pytest_cython/plugin.py` & `pytest-cython-0.3.1/src/pytest_cython/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import pathlib
 import re
 import sysconfig
 
 import pytest
 
-from typing import Any, Iterable
+from typing import Any, Iterable, Union
 
 from _pytest.nodes import Collector
 from _pytest.doctest import skip, DoctestModule, DoctestItem
 from _pytest.pathlib import resolve_package_path, ImportMode
 
 
 CYTHON_SUFFIXES = ['.py', '.pyx']
@@ -70,15 +70,15 @@
                 skip("unable to import module %r" % self.path)
             else:
                 raise
 
         return _add_line_numbers(module, items)
 
 
-def _without_suffixes(path: str | pathlib.Path) -> pathlib.Path:
+def _without_suffixes(path: Union[str, pathlib.Path]) -> pathlib.Path:
     path = pathlib.Path(path)
     return path.with_name(path.name.split('.')[0]).with_suffix('')
 
 
 def _get_module_name(path: pathlib.Path) -> str:
     pkg_path = resolve_package_path(path)
     if pkg_path is not None:
```

### Comparing `pytest-cython-0.3.0/src/pytest_cython.egg-info/PKG-INFO` & `pytest-cython-0.3.1/src/pytest_cython.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-cython
-Version: 0.3.0
+Version: 0.3.1
 Summary: A plugin for testing Cython extension modules
 Home-page: https://github.com/lgpage/pytest-cython
 Author: Logan Page
 Author-email: page.lg@gmail.com
 License: MIT
 Keywords: pytest,py.test,cython,doctest
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pytest-cython-0.3.0/src/pytest_cython.egg-info/SOURCES.txt` & `pytest-cython-0.3.1/src/pytest_cython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-cython-0.3.0/tests/example-project/setup.py` & `pytest-cython-0.3.1/tests/example-project/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,14 @@
 
     extensions = [
         Extension('*', ['src/pypackage/*.pyx'])
     ]
 
     setup(
         name='pytest-cython',
-        version='0.3.0',
+        version='0.3.1',
         description="Example Cython project for pytest-cython tests",
         package_dir={'': 'src'},
         packages=['pypackage'],
         zip_safe=False,
         ext_modules=cythonize(extensions, compiler_directives=directives)
     )
```

### Comparing `pytest-cython-0.3.0/tests/example-project/src/pypackage/cython_ext_module.pyx` & `pytest-cython-0.3.1/tests/example-project/src/pypackage/cython_ext_module.pyx`

 * *Files identical despite different names*

### Comparing `pytest-cython-0.3.0/tests/test_pytest_cython.py` & `pytest-cython-0.3.1/tests/test_pytest_cython.py`

 * *Files identical despite different names*

