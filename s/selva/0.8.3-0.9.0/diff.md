# Comparing `tmp/selva-0.8.3.tar.gz` & `tmp/selva-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selva-0.8.3.tar", max compression
+gzip compressed data, was "selva-0.9.0.tar", max compression
```

## Comparing `selva-0.8.3.tar` & `selva-0.9.0.tar`

### file list

```diff
@@ -1,54 +1,61 @@
--rw-r--r--   0        0        0     1070 2023-12-18 12:24:56.136863 selva-0.8.3/LICENSE
--rw-r--r--   0        0        0      948 2023-12-18 12:24:56.136863 selva-0.8.3/README.md
--rw-r--r--   0        0        0     2317 2023-12-18 12:24:56.140863 selva-0.8.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/__init__.py
--rw-r--r--   0        0        0        0 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/_util/__init__.py
--rw-r--r--   0        0        0     1045 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/_util/base_types.py
--rw-r--r--   0        0        0      185 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/_util/dotenv.py
--rw-r--r--   0        0        0      547 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/_util/import_item.py
--rw-r--r--   0        0        0      658 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/_util/maybe_async.py
--rw-r--r--   0        0        0     1522 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/_util/package_scan.py
--rw-r--r--   0        0        0       36 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/_util/pydantic/__init__.py
--rw-r--r--   0        0        0     1990 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/_util/pydantic/dotted_path.py
--rw-r--r--   0        0        0       50 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/configuration/__init__.py
--rw-r--r--   0        0        0      367 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/configuration/defaults.py
--rw-r--r--   0        0        0     2791 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/configuration/environment.py
--rw-r--r--   0        0        0     3452 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/configuration/settings.py
--rw-r--r--   0        0        0       74 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/di/__init__.py
--rw-r--r--   0        0        0     8102 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/di/container.py
--rw-r--r--   0        0        0     2689 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/di/decorator.py
--rw-r--r--   0        0        0     2216 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/di/error.py
--rw-r--r--   0        0        0      119 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/di/inject.py
--rw-r--r--   0        0        0      202 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/di/interceptor.py
--rw-r--r--   0        0        0        0 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/di/service/__init__.py
--rw-r--r--   0        0        0      556 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/di/service/model.py
--rw-r--r--   0        0        0     4332 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/di/service/parse.py
--rw-r--r--   0        0        0     2297 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/di/service/registry.py
--rw-r--r--   0        0        0        0 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/logging/__init__.py
--rw-r--r--   0        0        0      402 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/logging/logfmt.py
--rw-r--r--   0        0        0     1561 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/logging/setup.py
--rw-r--r--   0        0        0      858 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/logging/stdlib.py
--rw-r--r--   0        0        0        0 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/py.typed
--rw-r--r--   0        0        0      188 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/run.py
--rw-r--r--   0        0        0      328 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/web/__init__.py
--rw-r--r--   0        0        0    10608 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/web/application.py
--rw-r--r--   0        0        0        0 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/web/converter/__init__.py
--rw-r--r--   0        0        0      962 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/web/converter/decorator.py
--rw-r--r--   0        0        0     1106 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/web/converter/error.py
--rw-r--r--   0        0        0     1028 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/web/converter/from_request.py
--rw-r--r--   0        0        0     2244 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/web/converter/from_request_impl.py
--rw-r--r--   0        0        0      578 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/web/converter/param_converter.py
--rw-r--r--   0        0        0     1891 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/web/converter/param_converter_impl.py
--rw-r--r--   0        0        0      295 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/web/converter/param_extractor.py
--rw-r--r--   0        0        0     2559 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/web/converter/param_extractor_impl.py
--rw-r--r--   0        0        0      893 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/web/exception.py
--rw-r--r--   0        0        0      547 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/web/exception_handler.py
--rw-r--r--   0        0        0      347 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/web/middleware.py
--rw-r--r--   0        0        0        0 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/web/routing/__init__.py
--rw-r--r--   0        0        0     3122 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/web/routing/decorator.py
--rw-r--r--   0        0        0     3267 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/web/routing/route.py
--rw-r--r--   0        0        0     3193 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/web/routing/router.py
--rw-r--r--   0        0        0       50 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/web/templates/__init__.py
--rw-r--r--   0        0        0     3836 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/web/templates/jinja.py
--rw-r--r--   0        0        0      676 2023-12-18 12:24:56.140863 selva-0.8.3/src/selva/web/templates/template.py
--rw-r--r--   0        0        0     2277 1970-01-01 00:00:00.000000 selva-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-02-08 17:10:14.534513 selva-0.9.0/LICENSE
+-rw-r--r--   0        0        0      948 2024-02-08 17:10:14.534513 selva-0.9.0/README.md
+-rw-r--r--   0        0        0     2535 2024-02-08 17:10:14.538513 selva-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/_util/__init__.py
+-rw-r--r--   0        0        0     1045 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/_util/base_types.py
+-rw-r--r--   0        0        0      185 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/_util/dotenv.py
+-rw-r--r--   0        0        0      797 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/_util/import_item.py
+-rw-r--r--   0        0        0      658 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/_util/maybe_async.py
+-rw-r--r--   0        0        0     1522 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/_util/package_scan.py
+-rw-r--r--   0        0        0       77 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/_util/pydantic/__init__.py
+-rw-r--r--   0        0        0     1979 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/_util/pydantic/dotted_path.py
+-rw-r--r--   0        0        0       91 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/configuration/__init__.py
+-rw-r--r--   0        0        0      417 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/configuration/defaults.py
+-rw-r--r--   0        0        0     2791 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/configuration/environment.py
+-rw-r--r--   0        0        0     4010 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/configuration/settings.py
+-rw-r--r--   0        0        0      156 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/di/__init__.py
+-rw-r--r--   0        0        0     8150 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/di/container.py
+-rw-r--r--   0        0        0     2731 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/di/decorator.py
+-rw-r--r--   0        0        0     2216 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/di/error.py
+-rw-r--r--   0        0        0      119 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/di/inject.py
+-rw-r--r--   0        0        0      202 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/di/interceptor.py
+-rw-r--r--   0        0        0        0 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/di/service/__init__.py
+-rw-r--r--   0        0        0      556 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/di/service/model.py
+-rw-r--r--   0        0        0     4472 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/di/service/parse.py
+-rw-r--r--   0        0        0     2297 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/di/service/registry.py
+-rw-r--r--   0        0        0        0 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/ext/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/ext/data/__init__.py
+-rw-r--r--   0        0        0      618 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/ext/data/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     1036 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/ext/data/sqlalchemy/service.py
+-rw-r--r--   0        0        0     4401 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/ext/data/sqlalchemy/settings.py
+-rw-r--r--   0        0        0        0 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/ext/templates/__init__.py
+-rw-r--r--   0        0        0      694 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/ext/templates/jinja/__init__.py
+-rw-r--r--   0        0        0     2227 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/ext/templates/jinja/service.py
+-rw-r--r--   0        0        0     1683 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/ext/templates/jinja/settings.py
+-rw-r--r--   0        0        0        0 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/logging/__init__.py
+-rw-r--r--   0        0        0      402 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/logging/logfmt.py
+-rw-r--r--   0        0        0     1561 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/logging/setup.py
+-rw-r--r--   0        0        0      858 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/logging/stdlib.py
+-rw-r--r--   0        0        0        0 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/py.typed
+-rw-r--r--   0        0        0      188 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/run.py
+-rw-r--r--   0        0        0      369 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/web/__init__.py
+-rw-r--r--   0        0        0    11085 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/web/application.py
+-rw-r--r--   0        0        0        0 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/web/converter/__init__.py
+-rw-r--r--   0        0        0      962 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/web/converter/decorator.py
+-rw-r--r--   0        0        0     1106 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/web/converter/error.py
+-rw-r--r--   0        0        0     1028 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/web/converter/from_request.py
+-rw-r--r--   0        0        0     2176 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/web/converter/from_request_impl.py
+-rw-r--r--   0        0        0      578 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/web/converter/param_converter.py
+-rw-r--r--   0        0        0     1891 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/web/converter/param_converter_impl.py
+-rw-r--r--   0        0        0      295 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/web/converter/param_extractor.py
+-rw-r--r--   0        0        0     2559 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/web/converter/param_extractor_impl.py
+-rw-r--r--   0        0        0      893 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/web/exception.py
+-rw-r--r--   0        0        0      547 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/web/exception_handler.py
+-rw-r--r--   0        0        0      347 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/web/middleware.py
+-rw-r--r--   0        0        0        0 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/web/routing/__init__.py
+-rw-r--r--   0        0        0     3122 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/web/routing/decorator.py
+-rw-r--r--   0        0        0     3267 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/web/routing/route.py
+-rw-r--r--   0        0        0     3193 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/web/routing/router.py
+-rw-r--r--   0        0        0      676 2024-02-08 17:10:14.538513 selva-0.9.0/src/selva/web/templates.py
+-rw-r--r--   0        0        0     2370 1970-01-01 00:00:00.000000 selva-0.9.0/PKG-INFO
```

### Comparing `selva-0.8.3/LICENSE` & `selva-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `selva-0.8.3/README.md` & `selva-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `selva-0.8.3/pyproject.toml` & `selva-0.9.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "selva"
-version = "0.8.3"
+version = "0.9.0"
 description = "ASGI Web Framework with Dependency Injection"
 authors = ["Livio Ribeiro <livioribeiro@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/livioribeiro/selva"
 keywords = ["asgi", "framework", "asyncio", "web"]
 classifiers = [
@@ -25,49 +25,53 @@
     { include = "selva", from = "src" },
     { include = "selva/py.typed", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 asgikit = "^0.6"
-pydantic = "^2.5"
+pydantic = "^2.6"
 loguru = "^0.7"
 python-dotenv = "^1.0"
-strictyaml = "^1.7"
+"ruamel.yaml" = "^0.18"
 jinja2 = { version = "^3.1", optional = true }
+SQLAlchemy = { version = "^2.0", optional = true }
 
 [tool.poetry.extras]
 jinja = ["jinja2"]
+sqlalchemy = ["SQLAlchemy"]
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 uvicorn = { version = "^0.23", extras = ["standard"] }
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.4"
-pytest-asyncio = "^0.21"
-pytest-cov = "^4.1"
-coverage = { version = "^7.3", extras = ["toml"] }
-httpx = "^0.25"
+pytest = "^8"
+# TODO: remove "allow-prereleases" once pytest-asyncio supports pytest 8
+pytest-asyncio = { version = "^0.23", allow-prereleases = true }
+pytest-cov = "^4"
+coverage = { version = "^7", extras = ["toml"] }
+httpx = "^0.26"
+aiosqlite = "^0.19"
 
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 pylint = "^3.0"
-black = "^23.10"
-isort = "^5.12"
-flake8 = "^6.1"
-mypy = "^1.6"
-ruff = "^0.1"
+black = "^24.1"
+isort = "^5.13"
+flake8 = "^7.0"
+mypy = "^1.8"
+ruff = "^0.2"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.4"
 
@@ -84,13 +88,13 @@
 disable = ["C0114", "C0115", "C0116"] # ignore missing docstrings
 
 [tool.mypy]
 ignore_missing_imports = true
 
 [tool.black]
 line-length = 88
-target-version = ['py310']
+target-version = ["py311", "py312"]
 extend-exclude = "^/tests/configuration/invalid_settings/configuration/settings\\.py"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `selva-0.8.3/src/selva/_util/base_types.py` & `selva-0.9.0/src/selva/_util/base_types.py`

 * *Files identical despite different names*

### Comparing `selva-0.8.3/src/selva/_util/maybe_async.py` & `selva-0.9.0/src/selva/_util/maybe_async.py`

 * *Files identical despite different names*

### Comparing `selva-0.8.3/src/selva/_util/package_scan.py` & `selva-0.9.0/src/selva/_util/package_scan.py`

 * *Files identical despite different names*

### Comparing `selva-0.8.3/src/selva/_util/pydantic/dotted_path.py` & `selva-0.9.0/src/selva/_util/pydantic/dotted_path.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,19 @@
     ) -> core_schema.CoreSchema:
         origin = typing.get_origin(source_type)
         if origin is None:  # used as `x: Owner` without params
             item_tp = Any
         else:
             item_tp = typing.get_args(source_type)[0]
 
-        item_schema = handler.generate_schema(item_tp)
+        item_schema = handler.generate_schema(Any)
 
         def validate_from_str(
             value: str, function_handler: ValidatorFunctionWrapHandler
-        ) -> DottedPath[item_tp]:
+        ) -> item_tp:
             try:
                 item = import_item(value)
             except ImportError as e:
                 raise PydanticCustomError(
                     "invalid_dotted_path",
                     "unable to import '{path}': {error}",
                     {"path": value, "error": e.msg},
@@ -53,10 +53,10 @@
                 [
                     core_schema.is_subclass_schema(str),
                     from_str_schema,
                 ]
             ),
             serialization=core_schema.plain_serializer_function_ser_schema(
                 lambda instance: f"{instance.__module__}.{instance.__qualname__}",
-                when_used="unless-none",
+                when_used="json-unless-none",
             ),
         )
```

### Comparing `selva-0.8.3/src/selva/configuration/environment.py` & `selva-0.9.0/src/selva/configuration/environment.py`

 * *Files identical despite different names*

### Comparing `selva-0.8.3/src/selva/di/container.py` & `selva-0.9.0/src/selva/di/container.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from types import FunctionType, ModuleType
 from typing import Any, Type, TypeVar
 
 from loguru import logger
 
 from selva._util.maybe_async import maybe_async
 from selva._util.package_scan import scan_packages
-from selva.di.decorator import DI_SERVICE_ATTRIBUTE
+from selva.di.decorator import DI_ATTRIBUTE_SERVICE
 from selva.di.error import (
     DependencyLoopError,
     ServiceNotFoundError,
     ServiceWithoutDecoratorError,
 )
 from selva.di.interceptor import Interceptor
 from selva.di.service.model import InjectableType, ServiceDependency, ServiceSpec
@@ -31,15 +31,15 @@
 
     def register(
         self, service: InjectableType, *, provides: type = None, name: str = None
     ):
         self._register_service_spec(service, provides, name)
 
     def service(self, service: type):
-        service_info = getattr(service, DI_SERVICE_ATTRIBUTE, None)
+        service_info = getattr(service, DI_ATTRIBUTE_SERVICE, None)
 
         if not service_info:
             raise ServiceWithoutDecoratorError(service)
 
         provides, name = service_info
         self._register_service_spec(service, provides, name)
 
@@ -82,23 +82,23 @@
             name=f"{interceptor.__module__}.{interceptor.__qualname__}",
         )
         self.interceptors.append(interceptor)
 
         logger.trace("interceptor registered: {}", interceptor.__qualname__)
 
     def scan(self, *packages: str | ModuleType):
-        def predicate(item: Any):
-            return hasattr(item, DI_SERVICE_ATTRIBUTE)
+        def predicate_services(item: Any):
+            return hasattr(item, DI_ATTRIBUTE_SERVICE)
 
-        for service in scan_packages(packages, predicate):
-            provides, name = getattr(service, DI_SERVICE_ATTRIBUTE)
+        for service in scan_packages(packages, predicate_services):
+            provides, name = getattr(service, DI_ATTRIBUTE_SERVICE)
             self.register(service, provides=provides, name=name)
 
-    def has(self, service: type) -> bool:
-        definition = self.registry.get(service)
+    def has(self, service: type, name: str = None) -> bool:
+        definition = self.registry.get(service, name=name)
         return definition is not None
 
     def iter_service(
         self, key: type
     ) -> Iterable[tuple[type | FunctionType, str | None]]:
         record = self.registry.services.get(key)
         if not record:
@@ -222,12 +222,12 @@
     async def _run_interceptors(self, instance: Any, service_type: type):
         for cls in self.interceptors:
             interceptor = await self.get(
                 Interceptor, name=f"{cls.__module__}.{cls.__qualname__}"
             )
             await maybe_async(interceptor.intercept, instance, service_type)
 
-    async def run_finalizers(self):
+    async def _run_finalizers(self):
         for finalizer in reversed(self.finalizers):
             await finalizer
 
         self.finalizers.clear()
```

### Comparing `selva-0.8.3/src/selva/di/decorator.py` & `selva-0.9.0/src/selva/di/decorator.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import typing
 from collections.abc import Callable
 from typing import Annotated, TypeVar, dataclass_transform
 
 from selva.di.inject import Inject
 from selva.di.service.model import InjectableType, ServiceInfo
 
-__all__ = ("service", "DI_SERVICE_ATTRIBUTE")
+__all__ = ("service", "DI_ATTRIBUTE_SERVICE")
 
-DI_SERVICE_ATTRIBUTE = "__selva_di_service__"
+DI_ATTRIBUTE_SERVICE = "__selva_di_service__"
 
 T = TypeVar("T")
 
 
 def _is_inject(value) -> bool:
     origin = typing.get_origin(value)
     if not origin or origin is not Annotated:
@@ -30,28 +30,28 @@
 ) -> T | Callable[[T], T]:
     """Declare a class or function as a service
 
     For classes, a constructor will be generated to help create instances
     outside the dependency injection context
     """
 
-    def inner(injectable: InjectableType) -> T:
-        setattr(injectable, DI_SERVICE_ATTRIBUTE, ServiceInfo(provides, name))
+    def inner(inner_injectable: InjectableType) -> T:
+        setattr(inner_injectable, DI_ATTRIBUTE_SERVICE, ServiceInfo(provides, name))
 
-        if inspect.isclass(injectable):
+        if inspect.isclass(inner_injectable):
             dependencies = [
                 dependency
                 for dependency, annotation in inspect.get_annotations(
-                    injectable
+                    inner_injectable
                 ).items()
                 if _is_inject(annotation)
             ]
 
             # save a reference to the original constructor
-            original_init = getattr(injectable, "__init__", None)
+            original_init = getattr(inner_injectable, "__init__", None)
 
             def init(self, *args, **kwargs):
                 """Generated init method for service
 
                 Positional and keyword arguments will be set to declared dependencies.
                 Dependencies without an argument to set their value will be None.
                 Remaining arguments will be ignored.
@@ -72,12 +72,12 @@
                 # the rest of the dependencies will be set to None
                 param_keys = values.keys()
                 values |= {d: None for d in dependencies if d not in param_keys}
 
                 for k, v in values.items():
                     setattr(self, k, v)
 
-            setattr(injectable, "__init__", init)
+            setattr(inner_injectable, "__init__", init)
 
-        return injectable
+        return inner_injectable
 
     return inner(injectable) if injectable else inner
```

### Comparing `selva-0.8.3/src/selva/di/error.py` & `selva-0.9.0/src/selva/di/error.py`

 * *Files identical despite different names*

### Comparing `selva-0.8.3/src/selva/di/service/model.py` & `selva-0.9.0/src/selva/di/service/model.py`

 * *Files identical despite different names*

### Comparing `selva-0.8.3/src/selva/di/service/parse.py` & `selva-0.9.0/src/selva/di/service/parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,25 +46,28 @@
     arg_type, arg_meta = typing.get_args(hint)[0:2]
     if not isinstance(arg_meta, Inject) and arg_meta is not Inject:
         return None
 
     return arg_type, arg_meta
 
 
-def _get_service_signature(service: InjectableType) -> Iterable[str, type, Any]:
+def _get_service_signature(service: InjectableType) -> Iterable[tuple[str, type, Any]]:
     if inspect.isclass(service):
         for name, hint in typing.get_type_hints(service, include_extras=True).items():
             if params := _get_injectable_params(hint):
                 arg_type, arg_meta = params
                 yield name, arg_type, arg_meta
     elif inspect.isfunction(service):
         for name, param in inspect.signature(service).parameters.items():
             hint = param.annotation
-            value = param.default
-            yield name, hint, value
+            if params := _get_injectable_params(hint):
+                arg_type, arg_meta = params
+                yield name, arg_type, arg_meta
+            else:
+                yield name, hint, None
     else:
         raise InvalidServiceTypeError(service)
 
 
 def get_dependencies(
     service: InjectableType,
 ) -> Iterable[tuple[str, ServiceDependency]]:
```

### Comparing `selva-0.8.3/src/selva/di/service/registry.py` & `selva-0.9.0/src/selva/di/service/registry.py`

 * *Files identical despite different names*

### Comparing `selva-0.8.3/src/selva/logging/setup.py` & `selva-0.9.0/src/selva/logging/setup.py`

 * *Files identical despite different names*

### Comparing `selva-0.8.3/src/selva/logging/stdlib.py` & `selva-0.9.0/src/selva/logging/stdlib.py`

 * *Files identical despite different names*

### Comparing `selva-0.8.3/src/selva/web/application.py` & `selva-0.9.0/src/selva/web/application.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import functools
 import inspect
 import typing
 from http import HTTPStatus
-from importlib.util import find_spec
 from typing import Any
 from uuid import uuid4
 
 from asgikit.errors.websocket import WebSocketDisconnectError, WebSocketError
 from asgikit.requests import Request
 from asgikit.responses import respond_status
 from asgikit.websockets import WebSocket
 from loguru import logger
 
 from selva._util.base_types import get_base_types
 from selva._util.import_item import import_item
 from selva._util.maybe_async import maybe_async
 from selva.configuration.settings import Settings
 from selva.di.container import Container
-from selva.di.decorator import DI_SERVICE_ATTRIBUTE
+from selva.di.decorator import DI_ATTRIBUTE_SERVICE
 from selva.web.converter import (
     from_request_impl,
     param_converter_impl,
     param_extractor_impl,
 )
 from selva.web.converter.error import (
     MissingFromRequestImplError,
@@ -39,15 +38,15 @@
 
 
 def _is_controller(arg) -> bool:
     return inspect.isclass(arg) and hasattr(arg, CONTROLLER_ATTRIBUTE)
 
 
 def _is_service(arg) -> bool:
-    return hasattr(arg, DI_SERVICE_ATTRIBUTE)
+    return hasattr(arg, DI_ATTRIBUTE_SERVICE)
 
 
 def _is_module(arg) -> bool:
     return inspect.ismodule(arg) or isinstance(arg, str)
 
 
 class Selva:
@@ -55,21 +54,23 @@
 
     Will try to automatically import and register a module called "application".
     Other modules and classes can be registered using the "register" method
     """
 
     def __init__(self, settings: Settings):
         self.di = Container()
+        self.di.define(Container, self.di)
+
         self.router = Router()
-        self.handler = self._process_request
+        self.di.define(Router, self.router)
 
         self.settings = settings
         self.di.define(Settings, self.settings)
 
-        self.di.define(Router, self.router)
+        self.handler = self._process_request
 
         self._register_modules()
 
         setup_logger = import_item(self.settings.logging.setup)
         setup_logger(self.settings)
 
     async def __call__(self, scope, receive, send):
@@ -79,35 +80,44 @@
                     await self._handle_request(scope, receive, send)
             case "lifespan":
                 await self._handle_lifespan(scope, receive, send)
             case _:
                 raise RuntimeError(f"unknown scope '{scope['type']}'")
 
     def _register_modules(self):
-        try:
-            self.di.scan(self.settings.application)
-        except ModuleNotFoundError:
-            if not self.settings.modules:
-                raise
+        self.di.scan()
 
         self.di.scan(
             from_request_impl,
             param_extractor_impl,
             param_converter_impl,
         )
 
-        self.di.scan(*self.settings.modules)
-
-        if find_spec("jinja2") is not None:
-            self.di.scan("selva.web.templates")
+        self.di.scan(self.settings.application)
 
         for _iface, impl, _name in self.di.iter_all_services():
             if _is_controller(impl):
                 self.router.route(impl)
 
+    async def _initialize_extensions(self):
+        for extension_name in self.settings.extensions:
+            try:
+                extension_module = import_item(extension_name)
+            except ImportError:
+                raise TypeError(f"Extension '{extension_name}' not found")
+
+            try:
+                extension_init = getattr(extension_module, "selva_extension")
+            except AttributeError:
+                raise TypeError(
+                    f"Extension '{extension_name}' is missing the 'selva_extension()' function"
+                )
+
+            await maybe_async(extension_init, self.di, self.settings)
+
     async def _initialize_middleware(self):
         middleware = self.settings.middleware
         if len(middleware) == 0:
             return
 
         middleware = [import_item(name) for name in middleware]
 
@@ -120,18 +130,19 @@
 
         for cls in reversed(middleware):
             mid = await self.di.create(cls)
             chain = functools.partial(mid, self.handler)
             self.handler = chain
 
     async def _lifespan_startup(self):
+        await self._initialize_extensions()
         await self._initialize_middleware()
 
     async def _lifespan_shutdown(self):
-        await self.di.run_finalizers()
+        await self.di._run_finalizers()
 
     async def _handle_lifespan(self, _scope, receive, send):
         while True:
             message = await receive()
             if message["type"] == "lifespan.startup":
                 logger.trace("Handling lifespan startup")
                 try:
@@ -169,16 +180,16 @@
                 await self.handler(request)
             except Exception as err:
                 if handler := await self.di.get(
                     ExceptionHandler[type(err)], optional=True
                 ):
                     logger.trace(
                         "Handling exception with handler {}.{}",
-                        handler.__module__,
-                        handler.__qualname__,
+                        handler.__class__.__module__,
+                        handler.__class__.__qualname__,
                     )
                     await handler.handle_exception(request, err)
                 else:
                     raise
         except WebSocketException as err:
             await request.websocket.close(err.code, err.reason)
         except (WebSocketDisconnectError, WebSocketError):
```

### Comparing `selva-0.8.3/src/selva/web/converter/decorator.py` & `selva-0.9.0/src/selva/web/converter/decorator.py`

 * *Files identical despite different names*

### Comparing `selva-0.8.3/src/selva/web/converter/error.py` & `selva-0.9.0/src/selva/web/converter/error.py`

 * *Files identical despite different names*

### Comparing `selva-0.8.3/src/selva/web/converter/from_request.py` & `selva-0.9.0/src/selva/web/converter/from_request.py`

 * *Files identical despite different names*

### Comparing `selva-0.8.3/src/selva/web/converter/from_request_impl.py` & `selva-0.9.0/src/selva/web/converter/from_request_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
         self,
         request: Request,
         original_type: Type[PydanticModel],
         _parameter_name,
         _metadata=None,
     ) -> PydanticModel:
         if request.method not in (HTTPMethod.POST, HTTPMethod.PUT, HTTPMethod.PATCH):
-            # TODO: improve error
             raise TypeError(
                 "Pydantic model parameter on method that does not accept body"
             )
 
         # TODO: make request body decoding extensible
         if "application/json" in request.content_type:
             data = await read_json(request)
@@ -44,15 +43,14 @@
         self,
         request: Request,
         original_type: Type[list[PydanticModel]],
         _parameter_name,
         _metadata=None,
     ) -> list[PydanticModel]:
         if request.method not in (HTTPMethod.POST, HTTPMethod.PUT, HTTPMethod.PATCH):
-            # TODO: improve error
             raise TypeError("Pydantic parameter on method that does not accept body")
 
         if "application/json" in request.content_type:
             data = await read_json(request)
         else:
             raise HTTPException(status=HTTPStatus.UNSUPPORTED_MEDIA_TYPE)
```

### Comparing `selva-0.8.3/src/selva/web/converter/param_converter.py` & `selva-0.9.0/src/selva/web/converter/param_converter.py`

 * *Files identical despite different names*

### Comparing `selva-0.8.3/src/selva/web/converter/param_converter_impl.py` & `selva-0.9.0/src/selva/web/converter/param_converter_impl.py`

 * *Files identical despite different names*

### Comparing `selva-0.8.3/src/selva/web/converter/param_extractor_impl.py` & `selva-0.9.0/src/selva/web/converter/param_extractor_impl.py`

 * *Files identical despite different names*

### Comparing `selva-0.8.3/src/selva/web/exception.py` & `selva-0.9.0/src/selva/web/exception.py`

 * *Files identical despite different names*

### Comparing `selva-0.8.3/src/selva/web/exception_handler.py` & `selva-0.9.0/src/selva/web/exception_handler.py`

 * *Files identical despite different names*

### Comparing `selva-0.8.3/src/selva/web/routing/decorator.py` & `selva-0.9.0/src/selva/web/routing/decorator.py`

 * *Files identical despite different names*

### Comparing `selva-0.8.3/src/selva/web/routing/route.py` & `selva-0.9.0/src/selva/web/routing/route.py`

 * *Files identical despite different names*

### Comparing `selva-0.8.3/src/selva/web/routing/router.py` & `selva-0.9.0/src/selva/web/routing/router.py`

 * *Files identical despite different names*

### Comparing `selva-0.8.3/src/selva/web/templates/template.py` & `selva-0.9.0/src/selva/web/templates.py`

 * *Files identical despite different names*

### Comparing `selva-0.8.3/PKG-INFO` & `selva-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selva
-Version: 0.8.3
+Version: 0.9.0
 Summary: ASGI Web Framework with Dependency Injection
 Home-page: https://github.com/livioribeiro/selva
 License: MIT
 Keywords: asgi,framework,asyncio,web
 Author: Livio Ribeiro
 Author-email: livioribeiro@outlook.com
 Requires-Python: >=3.11,<4.0
@@ -18,20 +18,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Provides-Extra: jinja
+Provides-Extra: sqlalchemy
+Requires-Dist: SQLAlchemy (>=2.0,<3.0) ; extra == "sqlalchemy"
 Requires-Dist: asgikit (>=0.6,<0.7)
 Requires-Dist: jinja2 (>=3.1,<4.0) ; extra == "jinja"
 Requires-Dist: loguru (>=0.7,<0.8)
-Requires-Dist: pydantic (>=2.5,<3.0)
+Requires-Dist: pydantic (>=2.6,<3.0)
 Requires-Dist: python-dotenv (>=1.0,<2.0)
-Requires-Dist: strictyaml (>=1.7,<2.0)
+Requires-Dist: ruamel.yaml (>=0.18,<0.19)
 Project-URL: Repository, https://github.com/livioribeiro/selva
 Description-Content-Type: text/markdown
 
 # Project Selva
 
 Documentation: https://livioribeiro.github.io/selva/
```

