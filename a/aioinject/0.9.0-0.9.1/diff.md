# Comparing `tmp/aioinject-0.9.0.tar.gz` & `tmp/aioinject-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioinject-0.9.0.tar", last modified: Fri Jul 14 06:25:03 2023, max compression
+gzip compressed data, was "aioinject-0.9.1.tar", last modified: Fri Jul 14 06:29:50 2023, max compression
```

## Comparing `aioinject-0.9.0.tar` & `aioinject-0.9.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      429 2023-07-14 06:24:56.549521 aioinject-0.9.0/aioinject/__init__.py
--rw-r--r--   0        0        0     2675 2023-06-19 05:47:22.420243 aioinject-0.9.0/aioinject/containers.py
--rw-r--r--   0        0        0     6161 2023-06-19 05:44:42.043586 aioinject-0.9.0/aioinject/context.py
--rw-r--r--   0        0        0     3198 2023-02-19 10:45:20.646472 aioinject-0.9.0/aioinject/decorators.py
--rw-r--r--   0        0        0        0 2022-06-21 12:45:09.224983 aioinject-0.9.0/aioinject/ext/__init__.py
--rw-r--r--   0        0        0     1142 2023-02-19 10:46:32.417782 aioinject-0.9.0/aioinject/ext/fastapi.py
--rw-r--r--   0        0        0      866 2023-03-25 23:51:07.879400 aioinject-0.9.0/aioinject/ext/strawberry.py
--rw-r--r--   0        0        0      154 2022-02-14 23:34:38.786956 aioinject-0.9.0/aioinject/markers.py
--rw-r--r--   0        0        0     6659 2023-07-14 06:23:14.536779 aioinject-0.9.0/aioinject/providers.py
--rw-r--r--   0        0        0     2276 2023-07-14 06:24:08.912644 aioinject-0.9.0/aioinject/utils.py
--rw-r--r--   0        0        0     1063 2022-02-10 14:33:31.888253 aioinject-0.9.0/LICENSE
--rw-r--r--   0        0        0     1966 2023-07-14 06:24:56.576520 aioinject-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     5266 2022-05-25 14:51:11.254512 aioinject-0.9.0/readme.md
--rw-r--r--   0        0        0        0 2022-02-10 14:33:31.896255 aioinject-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524000 aioinject-0.9.0/tests/container/__init__.py
--rw-r--r--   0        0        0     3302 2023-06-15 07:30:36.661079 aioinject-0.9.0/tests/container/test_container.py
--rw-r--r--   0        0        0      489 2023-02-18 10:15:01.863109 aioinject-0.9.0/tests/container/test_override.py
--rw-r--r--   0        0        0        0 2022-02-14 23:35:15.649789 aioinject-0.9.0/tests/context/__init__.py
--rw-r--r--   0        0        0      500 2023-02-18 10:10:22.057657 aioinject-0.9.0/tests/context/conftest.py
--rw-r--r--   0        0        0     2022 2023-02-18 10:10:14.586441 aioinject-0.9.0/tests/context/test_context.py
--rw-r--r--   0        0        0     4256 2023-06-17 18:05:12.793704 aioinject-0.9.0/tests/context/test_context_managers.py
--rw-r--r--   0        0        0     2060 2023-02-18 11:02:03.522559 aioinject-0.9.0/tests/context/test_execute.py
--rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524000 aioinject-0.9.0/tests/ext/__init__.py
--rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524000 aioinject-0.9.0/tests/ext/strawberry/__init__.py
--rw-r--r--   0        0        0      976 2023-07-14 06:24:07.464642 aioinject-0.9.0/tests/ext/strawberry/test_inject_decorator.py
--rw-r--r--   0        0        0        0 2022-02-10 14:33:31.897254 aioinject-0.9.0/tests/providers/__init__.py
--rw-r--r--   0        0        0     4257 2023-06-15 08:40:10.535168 aioinject-0.9.0/tests/providers/test_callable.py
--rw-r--r--   0        0        0     1139 2023-02-18 11:02:25.628622 aioinject-0.9.0/tests/providers/test_object.py
--rw-r--r--   0        0        0      686 2023-02-18 09:50:26.751944 aioinject-0.9.0/tests/providers/test_singleton.py
--rw-r--r--   0        0        0     3845 2023-02-19 10:03:00.125198 aioinject-0.9.0/tests/test_inject.py
--rw-r--r--   0        0        0       39 2022-08-16 11:16:21.152175 aioinject-0.9.0/tests/utils/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2022-08-16 11:16:21.153175 aioinject-0.9.0/tests/utils/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2022-08-16 11:16:21.152175 aioinject-0.9.0/tests/utils/.pytest_cache/README.md
--rw-r--r--   0        0        0       43 2022-08-16 11:16:21.153175 aioinject-0.9.0/tests/utils/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2022-08-16 11:16:21.154175 aioinject-0.9.0/tests/utils/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524819 aioinject-0.9.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     1562 2023-06-15 08:40:10.557168 aioinject-0.9.0/tests/utils/test_guess_impl.py
--rw-r--r--   0        0        0      520 2023-02-18 11:01:50.087958 aioinject-0.9.0/tests/utils/test_utils.py
--rw-r--r--   0        0        0     5443 1970-01-01 00:00:00.000000 aioinject-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      429 2023-07-14 06:29:46.862621 aioinject-0.9.1/aioinject/__init__.py
+-rw-r--r--   0        0        0     2675 2023-06-19 05:47:22.420243 aioinject-0.9.1/aioinject/containers.py
+-rw-r--r--   0        0        0     6161 2023-06-19 05:44:42.043586 aioinject-0.9.1/aioinject/context.py
+-rw-r--r--   0        0        0     3198 2023-02-19 10:45:20.646472 aioinject-0.9.1/aioinject/decorators.py
+-rw-r--r--   0        0        0        0 2022-06-21 12:45:09.224983 aioinject-0.9.1/aioinject/ext/__init__.py
+-rw-r--r--   0        0        0     1142 2023-02-19 10:46:32.417782 aioinject-0.9.1/aioinject/ext/fastapi.py
+-rw-r--r--   0        0        0      866 2023-03-25 23:51:07.879400 aioinject-0.9.1/aioinject/ext/strawberry.py
+-rw-r--r--   0        0        0      154 2022-02-14 23:34:38.786956 aioinject-0.9.1/aioinject/markers.py
+-rw-r--r--   0        0        0     6659 2023-07-14 06:23:14.536779 aioinject-0.9.1/aioinject/providers.py
+-rw-r--r--   0        0        0     2275 2023-07-14 06:29:37.596102 aioinject-0.9.1/aioinject/utils.py
+-rw-r--r--   0        0        0     1063 2022-02-10 14:33:31.888253 aioinject-0.9.1/LICENSE
+-rw-r--r--   0        0        0     1966 2023-07-14 06:29:46.890621 aioinject-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     5266 2022-05-25 14:51:11.254512 aioinject-0.9.1/readme.md
+-rw-r--r--   0        0        0        0 2022-02-10 14:33:31.896255 aioinject-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524000 aioinject-0.9.1/tests/container/__init__.py
+-rw-r--r--   0        0        0     3302 2023-06-15 07:30:36.661079 aioinject-0.9.1/tests/container/test_container.py
+-rw-r--r--   0        0        0      489 2023-02-18 10:15:01.863109 aioinject-0.9.1/tests/container/test_override.py
+-rw-r--r--   0        0        0        0 2022-02-14 23:35:15.649789 aioinject-0.9.1/tests/context/__init__.py
+-rw-r--r--   0        0        0      500 2023-02-18 10:10:22.057657 aioinject-0.9.1/tests/context/conftest.py
+-rw-r--r--   0        0        0     2022 2023-02-18 10:10:14.586441 aioinject-0.9.1/tests/context/test_context.py
+-rw-r--r--   0        0        0     4256 2023-06-17 18:05:12.793704 aioinject-0.9.1/tests/context/test_context_managers.py
+-rw-r--r--   0        0        0     2060 2023-02-18 11:02:03.522559 aioinject-0.9.1/tests/context/test_execute.py
+-rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524000 aioinject-0.9.1/tests/ext/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524000 aioinject-0.9.1/tests/ext/strawberry/__init__.py
+-rw-r--r--   0        0        0      976 2023-07-14 06:24:07.464642 aioinject-0.9.1/tests/ext/strawberry/test_inject_decorator.py
+-rw-r--r--   0        0        0        0 2022-02-10 14:33:31.897254 aioinject-0.9.1/tests/providers/__init__.py
+-rw-r--r--   0        0        0     4257 2023-06-15 08:40:10.535168 aioinject-0.9.1/tests/providers/test_callable.py
+-rw-r--r--   0        0        0     1139 2023-02-18 11:02:25.628622 aioinject-0.9.1/tests/providers/test_object.py
+-rw-r--r--   0        0        0      686 2023-02-18 09:50:26.751944 aioinject-0.9.1/tests/providers/test_singleton.py
+-rw-r--r--   0        0        0     3845 2023-02-19 10:03:00.125198 aioinject-0.9.1/tests/test_inject.py
+-rw-r--r--   0        0        0       39 2022-08-16 11:16:21.152175 aioinject-0.9.1/tests/utils/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2022-08-16 11:16:21.153175 aioinject-0.9.1/tests/utils/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2022-08-16 11:16:21.152175 aioinject-0.9.1/tests/utils/.pytest_cache/README.md
+-rw-r--r--   0        0        0       43 2022-08-16 11:16:21.153175 aioinject-0.9.1/tests/utils/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2022-08-16 11:16:21.154175 aioinject-0.9.1/tests/utils/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524819 aioinject-0.9.1/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1562 2023-06-15 08:40:10.557168 aioinject-0.9.1/tests/utils/test_guess_impl.py
+-rw-r--r--   0        0        0      520 2023-02-18 11:01:50.087958 aioinject-0.9.1/tests/utils/test_utils.py
+-rw-r--r--   0        0        0     5443 1970-01-01 00:00:00.000000 aioinject-0.9.1/PKG-INFO
```

### Comparing `aioinject-0.9.0/aioinject/containers.py` & `aioinject-0.9.1/aioinject/containers.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.9.0/aioinject/context.py` & `aioinject-0.9.1/aioinject/context.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.9.0/aioinject/decorators.py` & `aioinject-0.9.1/aioinject/decorators.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.9.0/aioinject/ext/fastapi.py` & `aioinject-0.9.1/aioinject/ext/fastapi.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.9.0/aioinject/ext/strawberry.py` & `aioinject-0.9.1/aioinject/ext/strawberry.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.9.0/aioinject/providers.py` & `aioinject-0.9.1/aioinject/providers.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.9.0/aioinject/utils.py` & `aioinject-0.9.1/aioinject/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,9 +73,9 @@
 @contextlib.contextmanager
 def remove_annotation(
     annotations: dict[str, Any],
     name: str,
 ) -> Iterator[None]:
     annotation = annotations.pop(name, _sentinel)
     yield
-    if annotations is not _sentinel:
+    if annotation is not _sentinel:
         annotations[name] = annotation
```

### Comparing `aioinject-0.9.0/LICENSE` & `aioinject-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aioinject-0.9.0/pyproject.toml` & `aioinject-0.9.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 composite = [
     "coverage run",
     "coverage report",
 ]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.9.0"
+version = "0.9.1"
 version_files = [
     "aioinject/__init__.py",
     "pyproject.toml:version",
 ]
 
 [tool.coverage.run]
 source = [
@@ -108,15 +108,15 @@
 ]
 staticmethod-decorators = [
     "staticmethod",
 ]
 
 [project]
 name = "aioinject"
-version = "0.9.0"
+version = "0.9.1"
 description = ""
 authors = [
     { name = "Doctor", email = "thirvondukr@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.10"
 readme = "readme.md"
```

### Comparing `aioinject-0.9.0/readme.md` & `aioinject-0.9.1/readme.md`

 * *Files identical despite different names*

### Comparing `aioinject-0.9.0/tests/container/test_container.py` & `aioinject-0.9.1/tests/container/test_container.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.9.0/tests/context/test_context.py` & `aioinject-0.9.1/tests/context/test_context.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.9.0/tests/context/test_context_managers.py` & `aioinject-0.9.1/tests/context/test_context_managers.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.9.0/tests/context/test_execute.py` & `aioinject-0.9.1/tests/context/test_execute.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.9.0/tests/ext/strawberry/test_inject_decorator.py` & `aioinject-0.9.1/tests/ext/strawberry/test_inject_decorator.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.9.0/tests/providers/test_callable.py` & `aioinject-0.9.1/tests/providers/test_callable.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.9.0/tests/providers/test_object.py` & `aioinject-0.9.1/tests/providers/test_object.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.9.0/tests/providers/test_singleton.py` & `aioinject-0.9.1/tests/providers/test_singleton.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.9.0/tests/test_inject.py` & `aioinject-0.9.1/tests/test_inject.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.9.0/tests/utils/test_guess_impl.py` & `aioinject-0.9.1/tests/utils/test_guess_impl.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.9.0/tests/utils/test_utils.py` & `aioinject-0.9.1/tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.9.0/PKG-INFO` & `aioinject-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioinject
-Version: 0.9.0
+Version: 0.9.1
 License: MIT
 Author-email: Doctor <thirvondukr@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 Async-first dependency injection library based on python type hints
```

