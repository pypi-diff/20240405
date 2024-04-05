# Comparing `tmp/py-partiql-parser-0.5.1.tar.gz` & `tmp/py-partiql-parser-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-partiql-parser-0.5.1.tar", last modified: Thu Feb  1 21:31:51 2024, max compression
+gzip compressed data, was "py-partiql-parser-0.5.2.tar", last modified: Sat Mar 23 13:53:27 2024, max compression
```

## Comparing `py-partiql-parser-0.5.1.tar` & `py-partiql-parser-0.5.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:31:51.731569 py-partiql-parser-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-02-01 21:31:51.731569 py-partiql-parser-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:31:51.723569 py-partiql-parser-0.5.1/py_partiql_parser/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/py_partiql_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:31:51.727569 py-partiql-parser-0.5.1/py_partiql_parser/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/py_partiql_parser/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/py_partiql_parser/_internal/clause_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/py_partiql_parser/_internal/csv_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/py_partiql_parser/_internal/delete_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/py_partiql_parser/_internal/from_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/py_partiql_parser/_internal/insert_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/py_partiql_parser/_internal/json_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8250 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/py_partiql_parser/_internal/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/py_partiql_parser/_internal/select_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/py_partiql_parser/_internal/update_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/py_partiql_parser/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12947 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/py_partiql_parser/_internal/where_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:31:51.727569 py-partiql-parser-0.5.1/py_partiql_parser/_packages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/py_partiql_parser/_packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:31:51.727569 py-partiql-parser-0.5.1/py_partiql_parser/_packages/boto3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/py_partiql_parser/_packages/boto3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/py_partiql_parser/_packages/boto3/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/py_partiql_parser/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:31:51.731569 py-partiql-parser-0.5.1/py_partiql_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-02-01 21:31:51.000000 py-partiql-parser-0.5.1/py_partiql_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-02-01 21:31:51.000000 py-partiql-parser-0.5.1/py_partiql_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 21:31:51.000000 py-partiql-parser-0.5.1/py_partiql_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-01 21:31:51.000000 py-partiql-parser-0.5.1/py_partiql_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-01 21:31:51.000000 py-partiql-parser-0.5.1/py_partiql_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-02-01 21:31:46.000000 py-partiql-parser-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-01 21:31:51.731569 py-partiql-parser-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:31:51.731569 py-partiql-parser-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/tests/test_csv_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12601 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/tests/test_dynamodb_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/tests/test_from_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/tests/test_json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/tests/test_json_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/tests/test_query_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/tests/test_s3_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/tests/test_select_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/tests/test_select_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/tests/test_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-02-01 21:31:37.000000 py-partiql-parser-0.5.1/tests/test_where_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:53:27.974252 py-partiql-parser-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-03-23 13:53:27.974252 py-partiql-parser-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:53:27.966252 py-partiql-parser-0.5.2/py_partiql_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:53:27.970252 py-partiql-parser-0.5.2/py_partiql_parser/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_internal/clause_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_internal/csv_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_internal/delete_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_internal/from_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_internal/insert_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_internal/json_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8250 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_internal/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_internal/select_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_internal/update_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12947 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_internal/where_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:53:27.970252 py-partiql-parser-0.5.2/py_partiql_parser/_packages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:53:27.970252 py-partiql-parser-0.5.2/py_partiql_parser/_packages/boto3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_packages/boto3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/_packages/boto3/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/py_partiql_parser/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:53:27.974252 py-partiql-parser-0.5.2/py_partiql_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-03-23 13:53:27.000000 py-partiql-parser-0.5.2/py_partiql_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-03-23 13:53:27.000000 py-partiql-parser-0.5.2/py_partiql_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 13:53:27.000000 py-partiql-parser-0.5.2/py_partiql_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-23 13:53:27.000000 py-partiql-parser-0.5.2/py_partiql_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-23 13:53:27.000000 py-partiql-parser-0.5.2/py_partiql_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-23 13:53:25.000000 py-partiql-parser-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-23 13:53:27.974252 py-partiql-parser-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:53:27.974252 py-partiql-parser-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/tests/test_csv_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12601 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/tests/test_dynamodb_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/tests/test_from_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/tests/test_json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/tests/test_json_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/tests/test_query_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/tests/test_s3_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/tests/test_select_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/tests/test_select_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/tests/test_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-03-23 13:53:17.000000 py-partiql-parser-0.5.2/tests/test_where_parser.py
```

### Comparing `py-partiql-parser-0.5.1/LICENSE` & `py-partiql-parser-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.1/PKG-INFO` & `py-partiql-parser-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-partiql-parser
-Version: 0.5.1
+Version: 0.5.2
 Summary: Pure Python PartiQL Parser
 Author-email: Bert Blommers <info@bertblommers.nl>
 License: MIT
 Project-URL: Homepage, https://github.com/getmoto/py-partiql-parser
 Project-URL: Bug Tracker, https://github.com/getmoto/py-partiql-parser/issues
 Project-URL: ChangeLog, https://github.com/getmoto/py-partiql-parser/blob/main/CHANGELOG.md
 Keywords: pypartiql,parser
```

### Comparing `py-partiql-parser-0.5.1/README.md` & `py-partiql-parser-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.1/py_partiql_parser/_internal/clause_tokenizer.py` & `py-partiql-parser-0.5.2/py_partiql_parser/_internal/clause_tokenizer.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.1/py_partiql_parser/_internal/csv_converter.py` & `py-partiql-parser-0.5.2/py_partiql_parser/_internal/csv_converter.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from typing import List
+from typing import Any, Dict, List
 
 
 def csv_to_json(input: str, headers_included: bool = False) -> str:
     output = ""
     headers: List[str] = []
     for line in input.split("\n"):
         values = line.split(",")
@@ -14,7 +14,18 @@
             else:
                 headers = [f"_{x}" for x in range(1, len(values) + 1)]
         line = json.dumps({f"{headers[idx]}": key for idx, key in enumerate(values)})
         output += f"{line}\n"
     if output.endswith("\n"):
         output = output.rstrip("\n")
     return output
+
+
+def json_to_csv(
+    input: List[Dict[str, Any]], field_delimiter: str, record_delimiter: str
+) -> str:
+    result = ""
+    for row in input:
+        result += (
+            field_delimiter.join([f"{v}" for v in row.values()]) + record_delimiter
+        )
+    return result
```

### Comparing `py-partiql-parser-0.5.1/py_partiql_parser/_internal/delete_parser.py` & `py-partiql-parser-0.5.2/py_partiql_parser/_internal/delete_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.1/py_partiql_parser/_internal/from_parser.py` & `py-partiql-parser-0.5.2/py_partiql_parser/_internal/from_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.1/py_partiql_parser/_internal/insert_parser.py` & `py-partiql-parser-0.5.2/py_partiql_parser/_internal/insert_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.1/py_partiql_parser/_internal/json_parser.py` & `py-partiql-parser-0.5.2/py_partiql_parser/_internal/json_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.1/py_partiql_parser/_internal/parser.py` & `py-partiql-parser-0.5.2/py_partiql_parser/_internal/parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.1/py_partiql_parser/_internal/select_parser.py` & `py-partiql-parser-0.5.2/py_partiql_parser/_internal/select_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.1/py_partiql_parser/_internal/update_parser.py` & `py-partiql-parser-0.5.2/py_partiql_parser/_internal/update_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.1/py_partiql_parser/_internal/utils.py` & `py-partiql-parser-0.5.2/py_partiql_parser/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.1/py_partiql_parser/_internal/where_parser.py` & `py-partiql-parser-0.5.2/py_partiql_parser/_internal/where_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.1/py_partiql_parser/_packages/boto3/types.py` & `py-partiql-parser-0.5.2/py_partiql_parser/_packages/boto3/types.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.1/py_partiql_parser.egg-info/PKG-INFO` & `py-partiql-parser-0.5.2/py_partiql_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-partiql-parser
-Version: 0.5.1
+Version: 0.5.2
 Summary: Pure Python PartiQL Parser
 Author-email: Bert Blommers <info@bertblommers.nl>
 License: MIT
 Project-URL: Homepage, https://github.com/getmoto/py-partiql-parser
 Project-URL: Bug Tracker, https://github.com/getmoto/py-partiql-parser/issues
 Project-URL: ChangeLog, https://github.com/getmoto/py-partiql-parser/blob/main/CHANGELOG.md
 Keywords: pypartiql,parser
```

### Comparing `py-partiql-parser-0.5.1/py_partiql_parser.egg-info/SOURCES.txt` & `py-partiql-parser-0.5.2/py_partiql_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.1/pyproject.toml` & `py-partiql-parser-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "py-partiql-parser"
-version = "0.5.1"
+version = "0.5.2"
 description = "Pure Python PartiQL Parser"
 readme = "README.md"
 keywords = ["pypartiql", "parser"]
 license = {text = "MIT"}
 authors = [{name="Bert Blommers", email="info@bertblommers.nl"}]
 
 dependencies = []
```

### Comparing `py-partiql-parser-0.5.1/tests/__init__.py` & `py-partiql-parser-0.5.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.1/tests/test_dynamodb_examples.py` & `py-partiql-parser-0.5.2/tests/test_dynamodb_examples.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.1/tests/test_from_parser.py` & `py-partiql-parser-0.5.2/tests/test_from_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.1/tests/test_json_encoder.py` & `py-partiql-parser-0.5.2/tests/test_json_encoder.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.1/tests/test_json_parser.py` & `py-partiql-parser-0.5.2/tests/test_json_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.1/tests/test_query_metadata.py` & `py-partiql-parser-0.5.2/tests/test_query_metadata.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.1/tests/test_s3_examples.py` & `py-partiql-parser-0.5.2/tests/test_s3_examples.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.1/tests/test_select_functions.py` & `py-partiql-parser-0.5.2/tests/test_select_functions.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.1/tests/test_select_parser.py` & `py-partiql-parser-0.5.2/tests/test_select_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.1/tests/test_tokenizer.py` & `py-partiql-parser-0.5.2/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.1/tests/test_utils.py` & `py-partiql-parser-0.5.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.5.1/tests/test_where_parser.py` & `py-partiql-parser-0.5.2/tests/test_where_parser.py`

 * *Files identical despite different names*

