# Comparing `tmp/typedspark-1.3.2.tar.gz` & `tmp/typedspark-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedspark-1.3.2.tar", last modified: Tue Feb 27 21:07:34 2024, max compression
+gzip compressed data, was "typedspark-1.3.3.tar", last modified: Fri Apr  5 16:05:17 2024, max compression
```

## Comparing `typedspark-1.3.2.tar` & `typedspark-1.3.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:07:34.210382 typedspark-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-27 21:07:19.000000 typedspark-1.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-02-27 21:07:34.210382 typedspark-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-02-27 21:07:19.000000 typedspark-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-02-27 21:07:19.000000 typedspark-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 21:07:34.210382 typedspark-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-02-27 21:07:19.000000 typedspark-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:07:34.206382 typedspark-1.3.2/typedspark/
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-02-27 21:07:19.000000 typedspark-1.3.2/typedspark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:07:34.206382 typedspark-1.3.2/typedspark/_core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 21:07:19.000000 typedspark-1.3.2/typedspark/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-02-27 21:07:19.000000 typedspark-1.3.2/typedspark/_core/column.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-02-27 21:07:19.000000 typedspark-1.3.2/typedspark/_core/column_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    11036 2024-02-27 21:07:19.000000 typedspark-1.3.2/typedspark/_core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-02-27 21:07:19.000000 typedspark-1.3.2/typedspark/_core/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-02-27 21:07:19.000000 typedspark-1.3.2/typedspark/_core/literaltype.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-02-27 21:07:19.000000 typedspark-1.3.2/typedspark/_core/validate_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:07:34.210382 typedspark-1.3.2/typedspark/_schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 21:07:19.000000 typedspark-1.3.2/typedspark/_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-02-27 21:07:19.000000 typedspark-1.3.2/typedspark/_schema/dlt_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-02-27 21:07:19.000000 typedspark-1.3.2/typedspark/_schema/get_schema_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-02-27 21:07:19.000000 typedspark-1.3.2/typedspark/_schema/get_schema_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-02-27 21:07:19.000000 typedspark-1.3.2/typedspark/_schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-02-27 21:07:19.000000 typedspark-1.3.2/typedspark/_schema/structfield.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:07:34.210382 typedspark-1.3.2/typedspark/_transforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 21:07:19.000000 typedspark-1.3.2/typedspark/_transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-02-27 21:07:19.000000 typedspark-1.3.2/typedspark/_transforms/rename_duplicate_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-02-27 21:07:19.000000 typedspark-1.3.2/typedspark/_transforms/structtype_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-02-27 21:07:19.000000 typedspark-1.3.2/typedspark/_transforms/transform_to_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-02-27 21:07:19.000000 typedspark-1.3.2/typedspark/_transforms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:07:34.210382 typedspark-1.3.2/typedspark/_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 21:07:19.000000 typedspark-1.3.2/typedspark/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-02-27 21:07:19.000000 typedspark-1.3.2/typedspark/_utils/camelcase.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-02-27 21:07:19.000000 typedspark-1.3.2/typedspark/_utils/create_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-02-27 21:07:19.000000 typedspark-1.3.2/typedspark/_utils/create_dataset_from_structtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-02-27 21:07:19.000000 typedspark-1.3.2/typedspark/_utils/databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-02-27 21:07:19.000000 typedspark-1.3.2/typedspark/_utils/load_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-02-27 21:07:19.000000 typedspark-1.3.2/typedspark/_utils/register_schema_to_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 21:07:19.000000 typedspark-1.3.2/typedspark/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:07:34.210382 typedspark-1.3.2/typedspark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-02-27 21:07:34.000000 typedspark-1.3.2/typedspark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-02-27 21:07:34.000000 typedspark-1.3.2/typedspark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 21:07:34.000000 typedspark-1.3.2/typedspark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-27 21:07:34.000000 typedspark-1.3.2/typedspark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-27 21:07:34.000000 typedspark-1.3.2/typedspark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:05:17.355920 typedspark-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 16:05:04.000000 typedspark-1.3.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-05 16:05:17.355920 typedspark-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-05 16:05:04.000000 typedspark-1.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-05 16:05:04.000000 typedspark-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:05:17.355920 typedspark-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-05 16:05:04.000000 typedspark-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:05:17.351920 typedspark-1.3.3/typedspark/
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-05 16:05:04.000000 typedspark-1.3.3/typedspark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:05:17.351920 typedspark-1.3.3/typedspark/_core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:05:04.000000 typedspark-1.3.3/typedspark/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-05 16:05:04.000000 typedspark-1.3.3/typedspark/_core/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-05 16:05:04.000000 typedspark-1.3.3/typedspark/_core/column_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11036 2024-04-05 16:05:04.000000 typedspark-1.3.3/typedspark/_core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-05 16:05:04.000000 typedspark-1.3.3/typedspark/_core/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-05 16:05:04.000000 typedspark-1.3.3/typedspark/_core/literaltype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-05 16:05:04.000000 typedspark-1.3.3/typedspark/_core/validate_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:05:17.351920 typedspark-1.3.3/typedspark/_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:05:04.000000 typedspark-1.3.3/typedspark/_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-05 16:05:04.000000 typedspark-1.3.3/typedspark/_schema/dlt_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-04-05 16:05:04.000000 typedspark-1.3.3/typedspark/_schema/get_schema_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-04-05 16:05:04.000000 typedspark-1.3.3/typedspark/_schema/get_schema_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-04-05 16:05:04.000000 typedspark-1.3.3/typedspark/_schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-05 16:05:04.000000 typedspark-1.3.3/typedspark/_schema/structfield.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:05:17.351920 typedspark-1.3.3/typedspark/_transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:05:04.000000 typedspark-1.3.3/typedspark/_transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-04-05 16:05:04.000000 typedspark-1.3.3/typedspark/_transforms/rename_duplicate_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-05 16:05:04.000000 typedspark-1.3.3/typedspark/_transforms/structtype_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-05 16:05:04.000000 typedspark-1.3.3/typedspark/_transforms/transform_to_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-05 16:05:04.000000 typedspark-1.3.3/typedspark/_transforms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:05:17.355920 typedspark-1.3.3/typedspark/_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:05:04.000000 typedspark-1.3.3/typedspark/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-05 16:05:04.000000 typedspark-1.3.3/typedspark/_utils/camelcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-05 16:05:04.000000 typedspark-1.3.3/typedspark/_utils/create_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-05 16:05:04.000000 typedspark-1.3.3/typedspark/_utils/create_dataset_from_structtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-04-05 16:05:04.000000 typedspark-1.3.3/typedspark/_utils/databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-05 16:05:04.000000 typedspark-1.3.3/typedspark/_utils/load_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-05 16:05:04.000000 typedspark-1.3.3/typedspark/_utils/register_schema_to_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:05:04.000000 typedspark-1.3.3/typedspark/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:05:17.355920 typedspark-1.3.3/typedspark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-05 16:05:17.000000 typedspark-1.3.3/typedspark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-05 16:05:17.000000 typedspark-1.3.3/typedspark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:05:17.000000 typedspark-1.3.3/typedspark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-05 16:05:17.000000 typedspark-1.3.3/typedspark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 16:05:17.000000 typedspark-1.3.3/typedspark.egg-info/top_level.txt
```

### Comparing `typedspark-1.3.2/LICENSE.txt` & `typedspark-1.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `typedspark-1.3.2/PKG-INFO` & `typedspark-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: typedspark
-Version: 1.3.2
+Version: 1.3.3
 Summary: Column-wise type annotations for pyspark DataFrames
 Home-page: https://github.com/kaiko-ai/typedspark
 Author: Nanne Aben
 Author-email: nanne@kaiko.ai
 License: Apache-2.0
 Keywords: pyspark spark typing type checking annotations
 Classifier: Programming Language :: Python
 Classifier: Typing :: Typed
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: typing-extensions<=4.10.0
+Requires-Dist: typing-extensions<=4.11.0
 Provides-Extra: pyspark
 Requires-Dist: pyspark; extra == "pyspark"
 
 # Typedspark: column-wise type annotations for pyspark DataFrames
 
 We love Spark! But in production code we're wary when we see:
```

### Comparing `typedspark-1.3.2/README.md` & `typedspark-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `typedspark-1.3.2/pyproject.toml` & `typedspark-1.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typedspark-1.3.2/setup.py` & `typedspark-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.3.2/typedspark/__init__.py` & `typedspark-1.3.3/typedspark/__init__.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.3.2/typedspark/_core/column.py` & `typedspark-1.3.3/typedspark/_core/column.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.3.2/typedspark/_core/column_meta.py` & `typedspark-1.3.3/typedspark/_core/column_meta.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.3.2/typedspark/_core/dataset.py` & `typedspark-1.3.3/typedspark/_core/dataset.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.3.2/typedspark/_core/datatypes.py` & `typedspark-1.3.3/typedspark/_core/datatypes.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.3.2/typedspark/_core/literaltype.py` & `typedspark-1.3.3/typedspark/_core/literaltype.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.3.2/typedspark/_core/validate_schema.py` & `typedspark-1.3.3/typedspark/_core/validate_schema.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.3.2/typedspark/_schema/get_schema_definition.py` & `typedspark-1.3.3/typedspark/_schema/get_schema_definition.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.3.2/typedspark/_schema/get_schema_imports.py` & `typedspark-1.3.3/typedspark/_schema/get_schema_imports.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.3.2/typedspark/_schema/schema.py` & `typedspark-1.3.3/typedspark/_schema/schema.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.3.2/typedspark/_schema/structfield.py` & `typedspark-1.3.3/typedspark/_schema/structfield.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.3.2/typedspark/_transforms/rename_duplicate_columns.py` & `typedspark-1.3.3/typedspark/_transforms/rename_duplicate_columns.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.3.2/typedspark/_transforms/structtype_column.py` & `typedspark-1.3.3/typedspark/_transforms/structtype_column.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.3.2/typedspark/_transforms/transform_to_schema.py` & `typedspark-1.3.3/typedspark/_transforms/transform_to_schema.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.3.2/typedspark/_transforms/utils.py` & `typedspark-1.3.3/typedspark/_transforms/utils.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.3.2/typedspark/_utils/create_dataset.py` & `typedspark-1.3.3/typedspark/_utils/create_dataset.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.3.2/typedspark/_utils/create_dataset_from_structtype.py` & `typedspark-1.3.3/typedspark/_utils/create_dataset_from_structtype.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.3.2/typedspark/_utils/databases.py` & `typedspark-1.3.3/typedspark/_utils/databases.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.3.2/typedspark/_utils/load_table.py` & `typedspark-1.3.3/typedspark/_utils/load_table.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.3.2/typedspark/_utils/register_schema_to_dataset.py` & `typedspark-1.3.3/typedspark/_utils/register_schema_to_dataset.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.3.2/typedspark.egg-info/PKG-INFO` & `typedspark-1.3.3/typedspark.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: typedspark
-Version: 1.3.2
+Version: 1.3.3
 Summary: Column-wise type annotations for pyspark DataFrames
 Home-page: https://github.com/kaiko-ai/typedspark
 Author: Nanne Aben
 Author-email: nanne@kaiko.ai
 License: Apache-2.0
 Keywords: pyspark spark typing type checking annotations
 Classifier: Programming Language :: Python
 Classifier: Typing :: Typed
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: typing-extensions<=4.10.0
+Requires-Dist: typing-extensions<=4.11.0
 Provides-Extra: pyspark
 Requires-Dist: pyspark; extra == "pyspark"
 
 # Typedspark: column-wise type annotations for pyspark DataFrames
 
 We love Spark! But in production code we're wary when we see:
```

### Comparing `typedspark-1.3.2/typedspark.egg-info/SOURCES.txt` & `typedspark-1.3.3/typedspark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

