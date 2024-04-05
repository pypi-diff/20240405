# Comparing `tmp/parsagon-0.9.8.tar.gz` & `tmp/parsagon-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsagon-0.9.8.tar", last modified: Wed Aug 30 00:07:05 2023, max compression
+gzip compressed data, was "parsagon-0.9.9.tar", last modified: Wed Aug 30 01:56:14 2023, max compression
```

## Comparing `parsagon-0.9.8.tar` & `parsagon-0.9.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-30 00:07:05.783379 parsagon-0.9.8/
--rw-r--r--   0 amsuh    (10002)    18010     1711 2023-08-30 00:07:05.782481 parsagon-0.9.8/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010     1321 2023-07-07 07:03:35.000000 parsagon-0.9.8/README.md
--rw-r--r--   0 amsuh    (10002)    18010     1184 2023-08-30 00:02:39.000000 parsagon-0.9.8/pyproject.toml
--rw-r--r--   0 amsuh    (10002)    18010       38 2023-08-30 00:07:05.783627 parsagon-0.9.8/setup.cfg
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-30 00:07:05.756681 parsagon-0.9.8/src/
--rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.9.8/src/__init__.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-30 00:07:05.763929 parsagon-0.9.8/src/parsagon/
--rw-r--r--   0 amsuh    (10002)    18010       75 2023-08-29 23:28:04.000000 parsagon-0.9.8/src/parsagon/__init__.py
--rw-r--r--   0 amsuh    (10002)    18010     6421 2023-08-29 23:30:31.000000 parsagon-0.9.8/src/parsagon/api.py
--rw-r--r--   0 amsuh    (10002)    18010      770 2023-06-19 04:58:01.000000 parsagon-0.9.8/src/parsagon/custom_function.py
--rw-r--r--   0 amsuh    (10002)    18010      819 2023-07-07 07:03:35.000000 parsagon-0.9.8/src/parsagon/exceptions.py
--rw-r--r--   0 amsuh    (10002)    18010    15759 2023-08-23 01:01:06.000000 parsagon-0.9.8/src/parsagon/executor.py
--rw-r--r--   0 amsuh    (10002)    18010    14871 2023-08-04 23:48:32.000000 parsagon-0.9.8/src/parsagon/highlights.js
--rw-r--r--   0 amsuh    (10002)    18010    12196 2023-08-29 23:27:15.000000 parsagon-0.9.8/src/parsagon/main.py
--rw-r--r--   0 amsuh    (10002)    18010     2947 2023-07-18 08:23:24.000000 parsagon-0.9.8/src/parsagon/settings.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-30 00:07:05.780719 parsagon-0.9.8/src/parsagon/tests/
--rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.9.8/src/parsagon/tests/__init__.py
--rw-r--r--   0 amsuh    (10002)    18010     3127 2023-07-07 07:03:35.000000 parsagon-0.9.8/src/parsagon/tests/api_mocks.py
--rw-r--r--   0 amsuh    (10002)    18010      327 2023-07-07 07:03:35.000000 parsagon-0.9.8/src/parsagon/tests/cli_mocks.py
--rw-r--r--   0 amsuh    (10002)    18010      428 2023-07-07 07:03:35.000000 parsagon-0.9.8/src/parsagon/tests/conftest.py
--rw-r--r--   0 amsuh    (10002)    18010      645 2023-07-30 02:55:30.000000 parsagon-0.9.8/src/parsagon/tests/test_executor.py
--rw-r--r--   0 amsuh    (10002)    18010      676 2023-07-07 07:03:35.000000 parsagon-0.9.8/src/parsagon/tests/test_invalid_args.py
--rw-r--r--   0 amsuh    (10002)    18010     1089 2023-07-07 07:03:35.000000 parsagon-0.9.8/src/parsagon/tests/test_pipeline_operations.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-30 00:07:05.771257 parsagon-0.9.8/src/parsagon.egg-info/
--rw-r--r--   0 amsuh    (10002)    18010     1711 2023-08-30 00:07:05.000000 parsagon-0.9.8/src/parsagon.egg-info/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010      709 2023-08-30 00:07:05.000000 parsagon-0.9.8/src/parsagon.egg-info/SOURCES.txt
--rw-r--r--   0 amsuh    (10002)    18010        1 2023-08-30 00:07:05.000000 parsagon-0.9.8/src/parsagon.egg-info/dependency_links.txt
--rw-r--r--   0 amsuh    (10002)    18010       48 2023-08-30 00:07:05.000000 parsagon-0.9.8/src/parsagon.egg-info/entry_points.txt
--rw-r--r--   0 amsuh    (10002)    18010      282 2023-08-30 00:07:05.000000 parsagon-0.9.8/src/parsagon.egg-info/requires.txt
--rw-r--r--   0 amsuh    (10002)    18010        9 2023-08-30 00:07:05.000000 parsagon-0.9.8/src/parsagon.egg-info/top_level.txt
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-30 01:56:14.469862 parsagon-0.9.9/
+-rw-r--r--   0 amsuh    (10002)    18010     1711 2023-08-30 01:56:14.469529 parsagon-0.9.9/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010     1321 2023-07-07 07:03:35.000000 parsagon-0.9.9/README.md
+-rw-r--r--   0 amsuh    (10002)    18010     1184 2023-08-30 01:55:32.000000 parsagon-0.9.9/pyproject.toml
+-rw-r--r--   0 amsuh    (10002)    18010       38 2023-08-30 01:56:14.469976 parsagon-0.9.9/setup.cfg
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-30 01:56:14.453830 parsagon-0.9.9/src/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.9.9/src/__init__.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-30 01:56:14.460297 parsagon-0.9.9/src/parsagon/
+-rw-r--r--   0 amsuh    (10002)    18010       75 2023-08-29 23:28:04.000000 parsagon-0.9.9/src/parsagon/__init__.py
+-rw-r--r--   0 amsuh    (10002)    18010     6421 2023-08-29 23:30:31.000000 parsagon-0.9.9/src/parsagon/api.py
+-rw-r--r--   0 amsuh    (10002)    18010      770 2023-06-19 04:58:01.000000 parsagon-0.9.9/src/parsagon/custom_function.py
+-rw-r--r--   0 amsuh    (10002)    18010      819 2023-07-07 07:03:35.000000 parsagon-0.9.9/src/parsagon/exceptions.py
+-rw-r--r--   0 amsuh    (10002)    18010    15759 2023-08-23 01:01:06.000000 parsagon-0.9.9/src/parsagon/executor.py
+-rw-r--r--   0 amsuh    (10002)    18010    14871 2023-08-04 23:48:32.000000 parsagon-0.9.9/src/parsagon/highlights.js
+-rw-r--r--   0 amsuh    (10002)    18010    12197 2023-08-30 01:55:04.000000 parsagon-0.9.9/src/parsagon/main.py
+-rw-r--r--   0 amsuh    (10002)    18010     2947 2023-07-18 08:23:24.000000 parsagon-0.9.9/src/parsagon/settings.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-30 01:56:14.468895 parsagon-0.9.9/src/parsagon/tests/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.9.9/src/parsagon/tests/__init__.py
+-rw-r--r--   0 amsuh    (10002)    18010     3127 2023-07-07 07:03:35.000000 parsagon-0.9.9/src/parsagon/tests/api_mocks.py
+-rw-r--r--   0 amsuh    (10002)    18010      327 2023-07-07 07:03:35.000000 parsagon-0.9.9/src/parsagon/tests/cli_mocks.py
+-rw-r--r--   0 amsuh    (10002)    18010      428 2023-07-07 07:03:35.000000 parsagon-0.9.9/src/parsagon/tests/conftest.py
+-rw-r--r--   0 amsuh    (10002)    18010      645 2023-07-30 02:55:30.000000 parsagon-0.9.9/src/parsagon/tests/test_executor.py
+-rw-r--r--   0 amsuh    (10002)    18010      676 2023-07-07 07:03:35.000000 parsagon-0.9.9/src/parsagon/tests/test_invalid_args.py
+-rw-r--r--   0 amsuh    (10002)    18010     1089 2023-07-07 07:03:35.000000 parsagon-0.9.9/src/parsagon/tests/test_pipeline_operations.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-30 01:56:14.464093 parsagon-0.9.9/src/parsagon.egg-info/
+-rw-r--r--   0 amsuh    (10002)    18010     1711 2023-08-30 01:56:14.000000 parsagon-0.9.9/src/parsagon.egg-info/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010      709 2023-08-30 01:56:14.000000 parsagon-0.9.9/src/parsagon.egg-info/SOURCES.txt
+-rw-r--r--   0 amsuh    (10002)    18010        1 2023-08-30 01:56:14.000000 parsagon-0.9.9/src/parsagon.egg-info/dependency_links.txt
+-rw-r--r--   0 amsuh    (10002)    18010       48 2023-08-30 01:56:14.000000 parsagon-0.9.9/src/parsagon.egg-info/entry_points.txt
+-rw-r--r--   0 amsuh    (10002)    18010      282 2023-08-30 01:56:14.000000 parsagon-0.9.9/src/parsagon.egg-info/requires.txt
+-rw-r--r--   0 amsuh    (10002)    18010        9 2023-08-30 01:56:14.000000 parsagon-0.9.9/src/parsagon.egg-info/top_level.txt
```

### Comparing `parsagon-0.9.8/PKG-INFO` & `parsagon-0.9.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsagon
-Version: 0.9.8
+Version: 0.9.9
 Summary: Allows you to create browser automations with natural language
 Author-email: Sandy Suh <sandy@parsagon.io>
 Project-URL: Homepage, https://parsagon.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `parsagon-0.9.8/README.md` & `parsagon-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.8/pyproject.toml` & `parsagon-0.9.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 parsagon = ["highlights.js"]
 
 [tool.black]
 line-length = 120
 
 [project]
 name = "parsagon"
-version = "0.9.8"
+version = "0.9.9"
 description = "Allows you to create browser automations with natural language"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
   { name="Sandy Suh", email="sandy@parsagon.io" },
 ]
 classifiers = [
```

### Comparing `parsagon-0.9.8/src/parsagon/api.py` & `parsagon-0.9.9/src/parsagon/api.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.8/src/parsagon/custom_function.py` & `parsagon-0.9.9/src/parsagon/custom_function.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.8/src/parsagon/exceptions.py` & `parsagon-0.9.9/src/parsagon/exceptions.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.8/src/parsagon/executor.py` & `parsagon-0.9.9/src/parsagon/executor.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.8/src/parsagon/highlights.js` & `parsagon-0.9.9/src/parsagon/highlights.js`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.8/src/parsagon/main.py` & `parsagon-0.9.9/src/parsagon/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,10 +357,10 @@
 def get_product(url, timeout=300):
     start_time = time.time()
     with Halo(text="Extracting data...", spinner="dots"):
         while time.time() - start_time <= timeout:
             result = poll_product(url)
             if result["done"]:
                 return result["result"]
-            time.sleep(5)
+            time.sleep(15)
     logger.info("No data found")
     return None
```

### Comparing `parsagon-0.9.8/src/parsagon/settings.py` & `parsagon-0.9.9/src/parsagon/settings.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.8/src/parsagon/tests/api_mocks.py` & `parsagon-0.9.9/src/parsagon/tests/api_mocks.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.8/src/parsagon/tests/test_executor.py` & `parsagon-0.9.9/src/parsagon/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.8/src/parsagon/tests/test_invalid_args.py` & `parsagon-0.9.9/src/parsagon/tests/test_invalid_args.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.8/src/parsagon/tests/test_pipeline_operations.py` & `parsagon-0.9.9/src/parsagon/tests/test_pipeline_operations.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.8/src/parsagon.egg-info/PKG-INFO` & `parsagon-0.9.9/src/parsagon.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsagon
-Version: 0.9.8
+Version: 0.9.9
 Summary: Allows you to create browser automations with natural language
 Author-email: Sandy Suh <sandy@parsagon.io>
 Project-URL: Homepage, https://parsagon.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `parsagon-0.9.8/src/parsagon.egg-info/SOURCES.txt` & `parsagon-0.9.9/src/parsagon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

