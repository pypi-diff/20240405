# Comparing `tmp/types-Flask-Cors-4.0.0.20240106.tar.gz` & `tmp/types-Flask-Cors-4.0.0.20240405.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-Flask-Cors-4.0.0.20240106.tar", last modified: Sat Jan  6 02:22:24 2024, max compression
+gzip compressed data, was "types-Flask-Cors-4.0.0.20240405.tar", last modified: Fri Apr  5 02:14:54 2024, max compression
```

## Comparing `types-Flask-Cors-4.0.0.20240106.tar` & `types-Flask-Cors-4.0.0.20240405.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 02:22:24.487877 types-Flask-Cors-4.0.0.20240106/
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-01-06 02:22:24.000000 types-Flask-Cors-4.0.0.20240106/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-06 02:22:24.000000 types-Flask-Cors-4.0.0.20240106/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-01-06 02:22:24.487877 types-Flask-Cors-4.0.0.20240106/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 02:22:24.487877 types-Flask-Cors-4.0.0.20240106/flask_cors-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-01-06 02:22:24.000000 types-Flask-Cors-4.0.0.20240106/flask_cors-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-01-06 02:18:46.000000 types-Flask-Cors-4.0.0.20240106/flask_cors-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-01-06 02:18:46.000000 types-Flask-Cors-4.0.0.20240106/flask_cors-stubs/core.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-01-06 02:18:46.000000 types-Flask-Cors-4.0.0.20240106/flask_cors-stubs/decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-01-06 02:18:46.000000 types-Flask-Cors-4.0.0.20240106/flask_cors-stubs/extension.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-06 02:22:24.000000 types-Flask-Cors-4.0.0.20240106/flask_cors-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-06 02:18:46.000000 types-Flask-Cors-4.0.0.20240106/flask_cors-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-06 02:22:24.487877 types-Flask-Cors-4.0.0.20240106/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-01-06 02:22:24.000000 types-Flask-Cors-4.0.0.20240106/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 02:22:24.487877 types-Flask-Cors-4.0.0.20240106/types_Flask_Cors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-01-06 02:22:24.000000 types-Flask-Cors-4.0.0.20240106/types_Flask_Cors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-01-06 02:22:24.000000 types-Flask-Cors-4.0.0.20240106/types_Flask_Cors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-06 02:22:24.000000 types-Flask-Cors-4.0.0.20240106/types_Flask_Cors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-06 02:22:24.000000 types-Flask-Cors-4.0.0.20240106/types_Flask_Cors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-06 02:22:24.000000 types-Flask-Cors-4.0.0.20240106/types_Flask_Cors.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:14:54.714166 types-Flask-Cors-4.0.0.20240405/
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-05 02:14:54.000000 types-Flask-Cors-4.0.0.20240405/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 02:14:54.000000 types-Flask-Cors-4.0.0.20240405/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-05 02:14:54.714166 types-Flask-Cors-4.0.0.20240405/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:14:54.714166 types-Flask-Cors-4.0.0.20240405/flask_cors-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-05 02:14:54.000000 types-Flask-Cors-4.0.0.20240405/flask_cors-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-05 02:14:36.000000 types-Flask-Cors-4.0.0.20240405/flask_cors-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-05 02:14:36.000000 types-Flask-Cors-4.0.0.20240405/flask_cors-stubs/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-05 02:14:36.000000 types-Flask-Cors-4.0.0.20240405/flask_cors-stubs/decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-05 02:14:36.000000 types-Flask-Cors-4.0.0.20240405/flask_cors-stubs/extension.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 02:14:54.000000 types-Flask-Cors-4.0.0.20240405/flask_cors-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 02:14:36.000000 types-Flask-Cors-4.0.0.20240405/flask_cors-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 02:14:54.714166 types-Flask-Cors-4.0.0.20240405/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-05 02:14:54.000000 types-Flask-Cors-4.0.0.20240405/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:14:54.714166 types-Flask-Cors-4.0.0.20240405/types_Flask_Cors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-05 02:14:54.000000 types-Flask-Cors-4.0.0.20240405/types_Flask_Cors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-05 02:14:54.000000 types-Flask-Cors-4.0.0.20240405/types_Flask_Cors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:14:54.000000 types-Flask-Cors-4.0.0.20240405/types_Flask_Cors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 02:14:54.000000 types-Flask-Cors-4.0.0.20240405/types_Flask_Cors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 02:14:54.000000 types-Flask-Cors-4.0.0.20240405/types_Flask_Cors.egg-info/top_level.txt
```

### Comparing `types-Flask-Cors-4.0.0.20240106/CHANGELOG.md` & `types-Flask-Cors-4.0.0.20240405/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 4.0.0.20240405 (2024-04-05)
+
+Improve `flask-cors` stubs (#11708)
+
 ## 4.0.0.20240106 (2024-01-06)
 
 Update typing_extensions imports in third-party stubs (#11245)
 
 ## 4.0.0.2 (2023-11-24)
 
 Third-party stubs: remove unused `type: ignore`s (#11063)
```

### Comparing `types-Flask-Cors-4.0.0.20240106/PKG-INFO` & `types-Flask-Cors-4.0.0.20240405/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Flask-Cors
-Version: 4.0.0.20240106
+Version: 4.0.0.20240405
 Summary: Typing stubs for Flask-Cors
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Flask-Cors.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -32,10 +32,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `1de5830a2703936a96a126248227d5c7db883674` and was tested
-with mypy 1.8.0, pyright 1.1.342, and
-pytype 2023.12.18.
+This package was generated from typeshed commit `130a04905c0cab48604ac7be1f3d18ce96567c68` and was tested
+with mypy 1.9.0, pyright 1.1.357, and
+pytype 2024.3.19.
```

### Comparing `types-Flask-Cors-4.0.0.20240106/flask_cors-stubs/core.pyi` & `types-Flask-Cors-4.0.0.20240405/flask_cors-stubs/core.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections.abc import Iterable
 from datetime import timedelta
 from logging import Logger
 from re import Pattern
-from typing import Any, TypedDict, TypeVar, overload
+from typing import Any, Literal, TypedDict, TypeVar, overload
 from typing_extensions import TypeAlias
 
 import flask
 
 _IterableT = TypeVar("_IterableT", bound=Iterable[Any])
 _T = TypeVar("_T")
 _MultiDict: TypeAlias = Any  # werkzeug is not part of typeshed
@@ -42,15 +42,18 @@
 
 def parse_resources(resources: dict[str, _Options] | Iterable[str] | str | Pattern[str]) -> list[tuple[str, _Options]]: ...
 def get_regexp_pattern(regexp: str | Pattern[str]) -> str: ...
 def get_cors_origins(options: _Options, request_origin: str | None) -> list[str] | None: ...
 def get_allow_headers(options: _Options, acl_request_headers: str | None) -> str | None: ...
 def get_cors_headers(options: _Options, request_headers: dict[str, Any], request_method: str) -> _MultiDict: ...
 def set_cors_headers(resp: flask.Response, options: _Options) -> flask.Response: ...
-def probably_regex(maybe_regex: str | Pattern[str]) -> bool: ...
+@overload
+def probably_regex(maybe_regex: Pattern[str]) -> Literal[True]: ...
+@overload
+def probably_regex(maybe_regex: str) -> bool: ...
 def re_fix(reg: str) -> str: ...
 def try_match_any(inst: str, patterns: Iterable[str | Pattern[str]]) -> bool: ...
 def try_match(request_origin: str, maybe_regex: str | Pattern[str]) -> bool: ...
 def get_cors_options(appInstance: flask.Flask | None, *dicts: _Options) -> _Options: ...
 def get_app_kwarg_dict(appInstance: flask.Flask | None = None) -> _Options: ...
 def flexible_str(obj: object) -> str | None: ...
 def serialize_option(options_dict: _Options, key: str, upper: bool = False) -> None: ...
```

### Comparing `types-Flask-Cors-4.0.0.20240106/flask_cors-stubs/decorator.pyi` & `types-Flask-Cors-4.0.0.20240405/flask_cors-stubs/decorator.pyi`

 * *Files identical despite different names*

### Comparing `types-Flask-Cors-4.0.0.20240106/flask_cors-stubs/extension.pyi` & `types-Flask-Cors-4.0.0.20240405/flask_cors-stubs/extension.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from _typeshed import Incomplete
 from collections.abc import Callable, Iterable
 from datetime import timedelta
 from logging import Logger
 from typing import Any
 
 import flask
 
 LOG: Logger
 
 class CORS:
     def __init__(
         self,
-        app: Incomplete | None = None,
+        app: flask.Flask | None = None,
         *,
         resources: dict[str, dict[str, Any]] | list[str] | str | None = ...,
         origins: str | list[str] | None = ...,
         methods: str | list[str] | None = ...,
         expose_headers: str | list[str] | None = ...,
         allow_headers: str | list[str] | None = ...,
         supports_credentials: bool | None = ...,
```

### Comparing `types-Flask-Cors-4.0.0.20240106/setup.py` & `types-Flask-Cors-4.0.0.20240405/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `1de5830a2703936a96a126248227d5c7db883674` and was tested
-with mypy 1.8.0, pyright 1.1.342, and
-pytype 2023.12.18.
+This package was generated from typeshed commit `130a04905c0cab48604ac7be1f3d18ce96567c68` and was tested
+with mypy 1.9.0, pyright 1.1.357, and
+pytype 2024.3.19.
 '''.lstrip()
 
 setup(name=name,
-      version="4.0.0.20240106",
+      version="4.0.0.20240405",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Flask-Cors.md",
```

### Comparing `types-Flask-Cors-4.0.0.20240106/types_Flask_Cors.egg-info/PKG-INFO` & `types-Flask-Cors-4.0.0.20240405/types_Flask_Cors.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Flask-Cors
-Version: 4.0.0.20240106
+Version: 4.0.0.20240405
 Summary: Typing stubs for Flask-Cors
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Flask-Cors.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -32,10 +32,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `1de5830a2703936a96a126248227d5c7db883674` and was tested
-with mypy 1.8.0, pyright 1.1.342, and
-pytype 2023.12.18.
+This package was generated from typeshed commit `130a04905c0cab48604ac7be1f3d18ce96567c68` and was tested
+with mypy 1.9.0, pyright 1.1.357, and
+pytype 2024.3.19.
```

