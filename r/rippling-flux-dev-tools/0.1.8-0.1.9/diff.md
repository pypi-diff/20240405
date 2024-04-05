# Comparing `tmp/rippling_flux_dev_tools-0.1.8.tar.gz` & `tmp/rippling_flux_dev_tools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rippling_flux_dev_tools-0.1.8.tar", max compression
+gzip compressed data, was "rippling_flux_dev_tools-0.1.9.tar", max compression
```

## Comparing `rippling_flux_dev_tools-0.1.8.tar` & `rippling_flux_dev_tools-0.1.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2023-09-27 21:10:06.685741 rippling_flux_dev_tools-0.1.8/LICENSE
--rw-r--r--   0        0        0      998 2023-09-27 21:10:06.685741 rippling_flux_dev_tools-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-09-27 21:10:06.685741 rippling_flux_dev_tools-0.1.8/flux_dev_tools/server/__init__.py
--rw-r--r--   0        0        0      970 2023-09-27 21:10:06.685741 rippling_flux_dev_tools-0.1.8/flux_dev_tools/server/flask.py
--rw-r--r--   0        0        0     1603 2023-09-27 21:10:06.685741 rippling_flux_dev_tools-0.1.8/flux_dev_tools/server/invoke.py
--rw-r--r--   0        0        0     6799 2023-09-27 21:10:06.685741 rippling_flux_dev_tools-0.1.8/flux_dev_tools/server/serialization.py
--rw-r--r--   0        0        0     5251 2023-09-27 21:10:06.685741 rippling_flux_dev_tools-0.1.8/flux_dev_tools/server/tests/serialization.py
--rw-r--r--   0        0        0      444 2023-09-27 21:10:14.945941 rippling_flux_dev_tools-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1607 1970-01-01 00:00:00.000000 rippling_flux_dev_tools-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-09-29 18:19:54.886578 rippling_flux_dev_tools-0.1.9/LICENSE
+-rw-r--r--   0        0        0      998 2023-09-29 18:19:54.886578 rippling_flux_dev_tools-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-09-29 18:19:54.886578 rippling_flux_dev_tools-0.1.9/flux_dev_tools/server/__init__.py
+-rw-r--r--   0        0        0      970 2023-09-29 18:19:54.886578 rippling_flux_dev_tools-0.1.9/flux_dev_tools/server/flask.py
+-rw-r--r--   0        0        0     1603 2023-09-29 18:19:54.886578 rippling_flux_dev_tools-0.1.9/flux_dev_tools/server/invoke.py
+-rw-r--r--   0        0        0     6827 2023-09-29 18:19:54.886578 rippling_flux_dev_tools-0.1.9/flux_dev_tools/server/serialization.py
+-rw-r--r--   0        0        0     5251 2023-09-29 18:19:54.886578 rippling_flux_dev_tools-0.1.9/flux_dev_tools/server/tests/serialization.py
+-rw-r--r--   0        0        0      422 2023-09-29 18:20:02.218678 rippling_flux_dev_tools-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1564 1970-01-01 00:00:00.000000 rippling_flux_dev_tools-0.1.9/PKG-INFO
```

### Comparing `rippling_flux_dev_tools-0.1.8/LICENSE` & `rippling_flux_dev_tools-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rippling_flux_dev_tools-0.1.8/README.md` & `rippling_flux_dev_tools-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `rippling_flux_dev_tools-0.1.8/flux_dev_tools/server/flask.py` & `rippling_flux_dev_tools-0.1.9/flux_dev_tools/server/flask.py`

 * *Files identical despite different names*

### Comparing `rippling_flux_dev_tools-0.1.8/flux_dev_tools/server/invoke.py` & `rippling_flux_dev_tools-0.1.9/flux_dev_tools/server/invoke.py`

 * *Files identical despite different names*

### Comparing `rippling_flux_dev_tools-0.1.8/flux_dev_tools/server/serialization.py` & `rippling_flux_dev_tools-0.1.9/flux_dev_tools/server/serialization.py`

 * *Files 5% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     def _convert_object(self, obj, target_type):
         if get_origin(target_type) is list:
             target_type = get_args(target_type)[0]
         if isinstance(obj, list):
             return [self._convert_object(item, target_type) for item in obj]
 
         if target_type is not None:
-            if obj is None or type(obj) is get_origin(target_type):
+            if obj is None or type(obj) is get_origin(target_type) or type(obj) is target_type:
                 return obj
             elif target_type is Decimal:
                 return Decimal(obj)
             elif target_type is datetime:
                 return datetime.fromisoformat(obj)
             elif target_type is date:
                 return date.fromisoformat(obj)
```

### Comparing `rippling_flux_dev_tools-0.1.8/flux_dev_tools/server/tests/serialization.py` & `rippling_flux_dev_tools-0.1.9/flux_dev_tools/server/tests/serialization.py`

 * *Files identical despite different names*

### Comparing `rippling_flux_dev_tools-0.1.8/PKG-INFO` & `rippling_flux_dev_tools-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: rippling-flux-dev-tools
-Version: 0.1.8
+Version: 0.1.9
 Summary: Rippling Flux App development tools.
 Author: Rippling Apps
 Author-email: apps@rippling.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Flask (>=2.3.3,<3.0.0)
-Requires-Dist: jsonpickle (>=3.0.2,<4.0.0)
 Requires-Dist: rippling-flux-sdk (>=0.0.1,<0.0.2)
 Requires-Dist: werkzeug (>=2.3.7,<3.0.0)
 Description-Content-Type: text/markdown
 
 # rippling-flux-dev-tools
 
 A Python package with modules useful for local Flux app development.
```

