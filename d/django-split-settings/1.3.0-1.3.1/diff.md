# Comparing `tmp/django_split_settings-1.3.0.tar.gz` & `tmp/django_split_settings-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_split_settings-1.3.0.tar", max compression
+gzip compressed data, was "django_split_settings-1.3.1.tar", max compression
```

## Comparing `django_split_settings-1.3.0.tar` & `django_split_settings-1.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1535 2024-03-09 08:09:05.949046 django_split_settings-1.3.0/LICENSE
--rw-r--r--   0        0        0     4935 2024-03-09 08:50:09.961364 django_split_settings-1.3.0/README.md
--rw-r--r--   0        0        0     1995 2024-03-09 08:50:09.962139 django_split_settings-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      151 2024-03-09 08:09:05.950688 django_split_settings-1.3.0/split_settings/__init__.py
--rw-r--r--   0        0        0        0 2024-03-09 08:09:05.950714 django_split_settings-1.3.0/split_settings/py.typed
--rw-r--r--   0        0        0     3892 2024-03-09 08:50:09.962466 django_split_settings-1.3.0/split_settings/tools.py
--rw-r--r--   0        0        0     6430 1970-01-01 00:00:00.000000 django_split_settings-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1535 2024-04-05 07:05:54.287901 django_split_settings-1.3.1/LICENSE
+-rw-r--r--   0        0        0     4958 2024-04-05 07:05:54.288006 django_split_settings-1.3.1/README.md
+-rw-r--r--   0        0        0     2001 2024-04-05 07:06:07.941212 django_split_settings-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      151 2024-04-05 07:05:54.289649 django_split_settings-1.3.1/split_settings/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 07:05:54.289677 django_split_settings-1.3.1/split_settings/py.typed
+-rw-r--r--   0        0        0     3888 2024-04-05 07:05:54.289762 django_split_settings-1.3.1/split_settings/tools.py
+-rw-r--r--   0        0        0     6453 1970-01-01 00:00:00.000000 django_split_settings-1.3.1/PKG-INFO
```

### Comparing `django_split_settings-1.3.0/LICENSE` & `django_split_settings-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_split_settings-1.3.0/README.md` & `django_split_settings-1.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   <img src="https://raw.githubusercontent.com/sobolevn/django-split-settings/master/docs/_static/logo-black.png"
        alt="django-split-settings logo">
 </p>
 
 ---
 
 [![wemake.services](https://img.shields.io/badge/%20-wemake.services-green.svg?label=%20&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAABGdBTUEAALGPC%2FxhBQAAAAFzUkdCAK7OHOkAAAAbUExURQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAP%2F%2F%2F5TvxDIAAAAIdFJOUwAjRA8xXANAL%2Bv0SAAAADNJREFUGNNjYCAIOJjRBdBFWMkVQeGzcHAwksJnAPPZGOGAASzPzAEHEGVsLExQwE7YswCb7AFZSF3bbAAAAABJRU5ErkJggg%3D%3D)](https://wemake.services)
-[![test](https://github.com/sobolevn/django-split-settings/workflows/test/badge.svg?branch=master&event=push)](https://github.com/sobolevn/django-split-settings/actions?query=workflow%3Atest)
+[![test](https://github.com/wemake-services/django-split-settings/actions/workflows/test.yml/badge.svg?branch=master&event=push)](https://github.com/wemake-services/django-split-settings/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/sobolevn/django-split-settings/branch/master/graph/badge.svg)](https://codecov.io/gh/sobolevn/django-split-settings)
 [![Docs](https://readthedocs.org/projects/django-split-settings/badge/?version=latest)](http://django-split-settings.readthedocs.io/en/latest/?badge=latest)
 [![Python Version](https://img.shields.io/pypi/pyversions/django-split-settings.svg)](https://pypi.org/project/django-split-settings/)
 [![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide)
```

### Comparing `django_split_settings-1.3.0/pyproject.toml` & `django_split_settings-1.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-split-settings"
-version = "1.3.0"
+version = "1.3.1"
 description = "Organize Django settings into multiple files and directories. Easily override and modify settings. Use wildcards and optional settings files."
 authors = [
   "sobolevn <mail@sobolevn.me>",
   "Visa Kopu",
   "Antti Kaihola",
 ]
 license = "BSD-2-Clause"
@@ -57,15 +57,15 @@
 wemake-python-styleguide = "^0.18"
 flake8-pytest-style = "^1.5"
 nitpick = "^0.35"
 
 doc8 = "^1.1"
 
 pytest = "^8.0"
-pytest-cov = "^4.1"
+pytest-cov = ">=4.1,<6.0"
 pytest-randomly = "^3.12"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = ">=5.1,<8.0"
```

### Comparing `django_split_settings-1.3.0/split_settings/tools.py` & `django_split_settings-1.3.1/split_settings/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 Easily override and modify settings. Use wildcards and optional
 settings files.
 """
 
 from __future__ import annotations
 
 import glob
-import inspect
 import os
 import sys
 import typing
 from importlib.util import module_from_spec, spec_from_file_location
 
 __all__ = ('optional', 'include')  # noqa: WPS410
 
@@ -72,15 +71,15 @@
 
             scope=globals(),  # optional scope
         )
 
     """
     # we are getting globals() from previous frame
     # globals - it is caller's globals()
-    scope = scope or inspect.stack()[1][0].f_globals
+    scope = scope or sys._getframe(1).f_globals  # noqa: WPS437
 
     scope.setdefault('__included_files__', [])
     included_files = scope.get('__included_files__', [])
 
     including_file = scope.get(
         _INCLUDED_FILE,
         scope['__file__'].rstrip('c'),
```

### Comparing `django_split_settings-1.3.0/PKG-INFO` & `django_split_settings-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-split-settings
-Version: 1.3.0
+Version: 1.3.1
 Summary: Organize Django settings into multiple files and directories. Easily override and modify settings. Use wildcards and optional settings files.
 Home-page: https://django-split-settings.readthedocs.io
 License: BSD-2-Clause
 Keywords: django,settings,configuration,config
 Author: sobolevn
 Author-email: mail@sobolevn.me
 Requires-Python: >=3.9,<4.0
@@ -35,15 +35,15 @@
   <img src="https://raw.githubusercontent.com/sobolevn/django-split-settings/master/docs/_static/logo-black.png"
        alt="django-split-settings logo">
 </p>
 
 ---
 
 [![wemake.services](https://img.shields.io/badge/%20-wemake.services-green.svg?label=%20&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAABGdBTUEAALGPC%2FxhBQAAAAFzUkdCAK7OHOkAAAAbUExURQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAP%2F%2F%2F5TvxDIAAAAIdFJOUwAjRA8xXANAL%2Bv0SAAAADNJREFUGNNjYCAIOJjRBdBFWMkVQeGzcHAwksJnAPPZGOGAASzPzAEHEGVsLExQwE7YswCb7AFZSF3bbAAAAABJRU5ErkJggg%3D%3D)](https://wemake.services)
-[![test](https://github.com/sobolevn/django-split-settings/workflows/test/badge.svg?branch=master&event=push)](https://github.com/sobolevn/django-split-settings/actions?query=workflow%3Atest)
+[![test](https://github.com/wemake-services/django-split-settings/actions/workflows/test.yml/badge.svg?branch=master&event=push)](https://github.com/wemake-services/django-split-settings/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/sobolevn/django-split-settings/branch/master/graph/badge.svg)](https://codecov.io/gh/sobolevn/django-split-settings)
 [![Docs](https://readthedocs.org/projects/django-split-settings/badge/?version=latest)](http://django-split-settings.readthedocs.io/en/latest/?badge=latest)
 [![Python Version](https://img.shields.io/pypi/pyversions/django-split-settings.svg)](https://pypi.org/project/django-split-settings/)
 [![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide)
```

