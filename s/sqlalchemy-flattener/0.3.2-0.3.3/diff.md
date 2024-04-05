# Comparing `tmp/sqlalchemy_flattener-0.3.2.tar.gz` & `tmp/sqlalchemy_flattener-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_flattener-0.3.2.tar", max compression
+gzip compressed data, was "sqlalchemy_flattener-0.3.3.tar", max compression
```

## Comparing `sqlalchemy_flattener-0.3.2.tar` & `sqlalchemy_flattener-0.3.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2024-03-20 14:00:01.483890 sqlalchemy_flattener-0.3.2/LICENSE
--rw-r--r--   0        0        0       67 2024-03-20 14:00:01.483890 sqlalchemy_flattener-0.3.2/README.md
--rw-r--r--   0        0        0      597 2024-03-20 14:00:01.483890 sqlalchemy_flattener-0.3.2/pyproject.toml
--rw-r--r--   0        0        0       78 2024-03-20 14:00:01.483890 sqlalchemy_flattener-0.3.2/sqlalchemy_flattener/__init__.py
--rw-r--r--   0        0        0     1670 2024-03-20 14:00:01.483890 sqlalchemy_flattener-0.3.2/sqlalchemy_flattener/__main__.py
--rw-r--r--   0        0        0     7298 2024-03-20 14:00:01.483890 sqlalchemy_flattener-0.3.2/sqlalchemy_flattener/flattener.py
--rw-r--r--   0        0        0     1518 2024-03-20 14:00:01.483890 sqlalchemy_flattener-0.3.2/sqlalchemy_flattener/writers.py
--rw-r--r--   0        0        0      722 1970-01-01 00:00:00.000000 sqlalchemy_flattener-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-05 11:40:58.747221 sqlalchemy_flattener-0.3.3/LICENSE
+-rw-r--r--   0        0        0       67 2024-04-05 11:40:58.747221 sqlalchemy_flattener-0.3.3/README.md
+-rw-r--r--   0        0        0      597 2024-04-05 11:40:58.751221 sqlalchemy_flattener-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-04-05 11:40:58.751221 sqlalchemy_flattener-0.3.3/sqlalchemy_flattener/__init__.py
+-rw-r--r--   0        0        0     1848 2024-04-05 11:40:58.751221 sqlalchemy_flattener-0.3.3/sqlalchemy_flattener/__main__.py
+-rw-r--r--   0        0        0     7298 2024-04-05 11:40:58.751221 sqlalchemy_flattener-0.3.3/sqlalchemy_flattener/flattener.py
+-rw-r--r--   0        0        0     1518 2024-04-05 11:40:58.751221 sqlalchemy_flattener-0.3.3/sqlalchemy_flattener/writers.py
+-rw-r--r--   0        0        0      722 1970-01-01 00:00:00.000000 sqlalchemy_flattener-0.3.3/PKG-INFO
```

### Comparing `sqlalchemy_flattener-0.3.2/LICENSE` & `sqlalchemy_flattener-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_flattener-0.3.2/pyproject.toml` & `sqlalchemy_flattener-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqlalchemy-flattener"
-version = "0.3.2"
+version = "0.3.3"
 description = "Flatten SQLAlchemy model trees to raw data"
 authors = ["Michael Bosch <michael@lonelyviking.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `sqlalchemy_flattener-0.3.2/sqlalchemy_flattener/__main__.py` & `sqlalchemy_flattener-0.3.3/sqlalchemy_flattener/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import argparse
 import importlib
+import sys
+from collections.abc import Callable
+from pathlib import Path
 
 from sqlalchemy_flattener.flattener import SQLAlchemyFlattener
 from sqlalchemy_flattener.writers import write_as_dict, write_as_sql
 
 
 def main() -> None:
     parser = argparse.ArgumentParser(description="Flatten SQLAlchemy ORM instances.")
@@ -27,17 +30,21 @@
         type=str,
         default="sql",
         choices=["dict", "sql"],
         help="The format to write the data in.",
     )
 
     args = parser.parse_args()
+
+    sys.path.append(Path.cwd())
     instance_path, instance_var = args.instances.rsplit(".", 1)
     module = importlib.import_module(instance_path)
     instances = getattr(module, instance_var)
+    if isinstance(instances, Callable):
+        instances = instances()
 
     order_path, order_var = args.order.rsplit(".", 1)
     module = importlib.import_module(order_path)
     order = getattr(module, order_var)
 
     flattener = SQLAlchemyFlattener()
     unordered_data = flattener.flatten(instances)
```

### Comparing `sqlalchemy_flattener-0.3.2/sqlalchemy_flattener/flattener.py` & `sqlalchemy_flattener-0.3.3/sqlalchemy_flattener/flattener.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_flattener-0.3.2/sqlalchemy_flattener/writers.py` & `sqlalchemy_flattener-0.3.3/sqlalchemy_flattener/writers.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_flattener-0.3.2/PKG-INFO` & `sqlalchemy_flattener-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-flattener
-Version: 0.3.2
+Version: 0.3.3
 Summary: Flatten SQLAlchemy model trees to raw data
 License: MIT
 Author: Michael Bosch
 Author-email: michael@lonelyviking.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

