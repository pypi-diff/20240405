# Comparing `tmp/py-partiql-parser-0.5.2.tar.gz` & `tmp/py-partiql-parser-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-partiql-parser-0.5.2.tar", last modified: Sat Mar 23 13:53:27 2024, max compression
+gzip compressed data, was "py-partiql-parser-0.5.3.tar", last modified: Fri Apr  5 20:39:33 2024, max compression
```

## Comparing `py-partiql-parser-0.5.2.tar` & `py-partiql-parser-0.5.3.tar`

### file list

```diff
@@ -1,48 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:53:27.974252 py-partiql-parser-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-03-23 13:53:27.974252 py-partiql-parser-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:53:27.966252 py-partiql-parser-0.5.2/py_partiql_parser/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:53:27.970252 py-partiql-parser-0.5.2/py_partiql_parser/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_internal/clause_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_internal/csv_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_internal/delete_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_internal/from_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_internal/insert_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_internal/json_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8250 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_internal/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_internal/select_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_internal/update_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12947 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_internal/where_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:53:27.970252 py-partiql-parser-0.5.2/py_partiql_parser/_packages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:53:27.970252 py-partiql-parser-0.5.2/py_partiql_parser/_packages/boto3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_packages/boto3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_packages/boto3/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:53:27.974252 py-partiql-parser-0.5.2/py_partiql_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-03-23 13:53:27.000000 py-partiql-parser-0.5.2/py_partiql_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-03-23 13:53:27.000000 py-partiql-parser-0.5.2/py_partiql_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 13:53:27.000000 py-partiql-parser-0.5.2/py_partiql_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-23 13:53:27.000000 py-partiql-parser-0.5.2/py_partiql_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-23 13:53:27.000000 py-partiql-parser-0.5.2/py_partiql_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-23 13:53:25.000000 py-partiql-parser-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-23 13:53:27.974252 py-partiql-parser-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:53:27.974252 py-partiql-parser-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/tests/test_csv_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12601 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/tests/test_dynamodb_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/tests/test_from_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/tests/test_json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/tests/test_json_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/tests/test_query_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/tests/test_s3_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/tests/test_select_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/tests/test_select_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/tests/test_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/tests/test_where_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:39:33.471206 py-partiql-parser-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-05 20:39:22.000000 py-partiql-parser-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-05 20:39:22.000000 py-partiql-parser-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-05 20:39:33.471206 py-partiql-parser-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-05 20:39:22.000000 py-partiql-parser-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:39:33.467206 py-partiql-parser-0.5.3/py_partiql_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-05 20:39:22.000000 py-partiql-parser-0.5.3/py_partiql_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-05 20:39:22.000000 py-partiql-parser-0.5.3/py_partiql_parser/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:39:33.471206 py-partiql-parser-0.5.3/py_partiql_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-05 20:39:33.000000 py-partiql-parser-0.5.3/py_partiql_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-05 20:39:33.000000 py-partiql-parser-0.5.3/py_partiql_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 20:39:33.000000 py-partiql-parser-0.5.3/py_partiql_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-05 20:39:33.000000 py-partiql-parser-0.5.3/py_partiql_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 20:39:33.000000 py-partiql-parser-0.5.3/py_partiql_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-05 20:39:31.000000 py-partiql-parser-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-05 20:39:33.471206 py-partiql-parser-0.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:39:33.471206 py-partiql-parser-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-05 20:39:22.000000 py-partiql-parser-0.5.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-05 20:39:22.000000 py-partiql-parser-0.5.3/tests/test_csv_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12601 2024-04-05 20:39:22.000000 py-partiql-parser-0.5.3/tests/test_dynamodb_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-05 20:39:22.000000 py-partiql-parser-0.5.3/tests/test_from_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-05 20:39:22.000000 py-partiql-parser-0.5.3/tests/test_json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-05 20:39:22.000000 py-partiql-parser-0.5.3/tests/test_json_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-05 20:39:22.000000 py-partiql-parser-0.5.3/tests/test_query_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-05 20:39:22.000000 py-partiql-parser-0.5.3/tests/test_s3_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-05 20:39:22.000000 py-partiql-parser-0.5.3/tests/test_select_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-05 20:39:22.000000 py-partiql-parser-0.5.3/tests/test_select_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-05 20:39:22.000000 py-partiql-parser-0.5.3/tests/test_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-05 20:39:22.000000 py-partiql-parser-0.5.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-04-05 20:39:22.000000 py-partiql-parser-0.5.3/tests/test_where_parser.py
```

### Comparing `py-partiql-parser-0.5.2/LICENSE` & `py-partiql-parser-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.2/PKG-INFO` & `py-partiql-parser-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-partiql-parser
-Version: 0.5.2
+Version: 0.5.3
 Summary: Pure Python PartiQL Parser
 Author-email: Bert Blommers <info@bertblommers.nl>
 License: MIT
 Project-URL: Homepage, https://github.com/getmoto/py-partiql-parser
 Project-URL: Bug Tracker, https://github.com/getmoto/py-partiql-parser/issues
 Project-URL: ChangeLog, https://github.com/getmoto/py-partiql-parser/blob/main/CHANGELOG.md
 Keywords: pypartiql,parser
```

### Comparing `py-partiql-parser-0.5.2/README.md` & `py-partiql-parser-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.2/py_partiql_parser.egg-info/PKG-INFO` & `py-partiql-parser-0.5.3/py_partiql_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-partiql-parser
-Version: 0.5.2
+Version: 0.5.3
 Summary: Pure Python PartiQL Parser
 Author-email: Bert Blommers <info@bertblommers.nl>
 License: MIT
 Project-URL: Homepage, https://github.com/getmoto/py-partiql-parser
 Project-URL: Bug Tracker, https://github.com/getmoto/py-partiql-parser/issues
 Project-URL: ChangeLog, https://github.com/getmoto/py-partiql-parser/blob/main/CHANGELOG.md
 Keywords: pypartiql,parser
```

### Comparing `py-partiql-parser-0.5.2/py_partiql_parser.egg-info/SOURCES.txt` & `py-partiql-parser-0.5.3/py_partiql_parser.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -6,29 +6,14 @@
 py_partiql_parser/__init__.py
 py_partiql_parser/exceptions.py
 py_partiql_parser.egg-info/PKG-INFO
 py_partiql_parser.egg-info/SOURCES.txt
 py_partiql_parser.egg-info/dependency_links.txt
 py_partiql_parser.egg-info/requires.txt
 py_partiql_parser.egg-info/top_level.txt
-py_partiql_parser/_internal/__init__.py
-py_partiql_parser/_internal/clause_tokenizer.py
-py_partiql_parser/_internal/csv_converter.py
-py_partiql_parser/_internal/delete_parser.py
-py_partiql_parser/_internal/from_parser.py
-py_partiql_parser/_internal/insert_parser.py
-py_partiql_parser/_internal/json_parser.py
-py_partiql_parser/_internal/parser.py
-py_partiql_parser/_internal/select_parser.py
-py_partiql_parser/_internal/update_parser.py
-py_partiql_parser/_internal/utils.py
-py_partiql_parser/_internal/where_parser.py
-py_partiql_parser/_packages/__init__.py
-py_partiql_parser/_packages/boto3/__init__.py
-py_partiql_parser/_packages/boto3/types.py
 tests/__init__.py
 tests/test_csv_converter.py
 tests/test_dynamodb_examples.py
 tests/test_from_parser.py
 tests/test_json_encoder.py
 tests/test_json_parser.py
 tests/test_query_metadata.py
```

### Comparing `py-partiql-parser-0.5.2/pyproject.toml` & `py-partiql-parser-0.5.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 [project]
 name = "py-partiql-parser"
-version = "0.5.2"
+version = "0.5.3"
 description = "Pure Python PartiQL Parser"
 readme = "README.md"
 keywords = ["pypartiql", "parser"]
 license = {text = "MIT"}
 authors = [{name="Bert Blommers", email="info@bertblommers.nl"}]
 
 dependencies = []
 
+[tool.setuptools]
+packages = ["py_partiql_parser"]
+
 [project.urls]
 "Homepage" = "https://github.com/getmoto/py-partiql-parser"
 "Bug Tracker" = "https://github.com/getmoto/py-partiql-parser/issues"
 "ChangeLog" = "https://github.com/getmoto/py-partiql-parser/blob/main/CHANGELOG.md"
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `py-partiql-parser-0.5.2/tests/__init__.py` & `py-partiql-parser-0.5.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.2/tests/test_csv_converter.py` & `py-partiql-parser-0.5.3/tests/test_csv_converter.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.2/tests/test_dynamodb_examples.py` & `py-partiql-parser-0.5.3/tests/test_dynamodb_examples.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.2/tests/test_from_parser.py` & `py-partiql-parser-0.5.3/tests/test_from_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.2/tests/test_json_encoder.py` & `py-partiql-parser-0.5.3/tests/test_json_encoder.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.2/tests/test_json_parser.py` & `py-partiql-parser-0.5.3/tests/test_json_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.2/tests/test_query_metadata.py` & `py-partiql-parser-0.5.3/tests/test_query_metadata.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.2/tests/test_s3_examples.py` & `py-partiql-parser-0.5.3/tests/test_s3_examples.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.2/tests/test_select_functions.py` & `py-partiql-parser-0.5.3/tests/test_select_functions.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.2/tests/test_select_parser.py` & `py-partiql-parser-0.5.3/tests/test_select_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.2/tests/test_tokenizer.py` & `py-partiql-parser-0.5.3/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.2/tests/test_utils.py` & `py-partiql-parser-0.5.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.2/tests/test_where_parser.py` & `py-partiql-parser-0.5.3/tests/test_where_parser.py`

 * *Files identical despite different names*

