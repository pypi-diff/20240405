# Comparing `tmp/tonic_ragas_logger-1.2.0.tar.gz` & `tmp/tonic_ragas_logger-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonic_ragas_logger-1.2.0.tar", max compression
+gzip compressed data, was "tonic_ragas_logger-1.2.1.tar", max compression
```

## Comparing `tonic_ragas_logger-1.2.0.tar` & `tonic_ragas_logger-1.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1063 2024-04-02 20:17:54.022697 tonic_ragas_logger-1.2.0/LICENSE
--rw-r--r--   0        0        0     2463 2024-04-02 20:17:54.022697 tonic_ragas_logger-1.2.0/README.md
--rw-r--r--   0        0        0      448 2024-04-02 20:17:54.022697 tonic_ragas_logger-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       81 2024-04-02 20:17:54.026697 tonic_ragas_logger-1.2.0/tonic_ragas_logger/__init__.py
--rw-r--r--   0        0        0      343 2024-04-02 20:17:54.026697 tonic_ragas_logger-1.2.0/tonic_ragas_logger/config.py
--rw-r--r--   0        0        0     4027 2024-04-02 20:17:54.026697 tonic_ragas_logger-1.2.0/tonic_ragas_logger/ragas_validate_api.py
--rw-r--r--   0        0        0        0 2024-04-02 20:17:54.026697 tonic_ragas_logger-1.2.0/tonic_ragas_logger/utils/__init__.py
--rw-r--r--   0        0        0     2880 2024-04-02 20:17:54.026697 tonic_ragas_logger-1.2.0/tonic_ragas_logger/utils/http_client.py
--rw-r--r--   0        0        0     3036 1970-01-01 00:00:00.000000 tonic_ragas_logger-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-05 20:03:04.436477 tonic_ragas_logger-1.2.1/LICENSE
+-rw-r--r--   0        0        0     2463 2024-04-05 20:03:04.436477 tonic_ragas_logger-1.2.1/README.md
+-rw-r--r--   0        0        0      448 2024-04-05 20:03:04.440477 tonic_ragas_logger-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0       81 2024-04-05 20:03:04.440477 tonic_ragas_logger-1.2.1/tonic_ragas_logger/__init__.py
+-rw-r--r--   0        0        0      343 2024-04-05 20:03:04.440477 tonic_ragas_logger-1.2.1/tonic_ragas_logger/config.py
+-rw-r--r--   0        0        0     3995 2024-04-05 20:03:04.440477 tonic_ragas_logger-1.2.1/tonic_ragas_logger/ragas_validate_api.py
+-rw-r--r--   0        0        0        0 2024-04-05 20:03:04.440477 tonic_ragas_logger-1.2.1/tonic_ragas_logger/utils/__init__.py
+-rw-r--r--   0        0        0     2880 2024-04-05 20:03:04.440477 tonic_ragas_logger-1.2.1/tonic_ragas_logger/utils/http_client.py
+-rw-r--r--   0        0        0     3036 1970-01-01 00:00:00.000000 tonic_ragas_logger-1.2.1/PKG-INFO
```

### Comparing `tonic_ragas_logger-1.2.0/LICENSE` & `tonic_ragas_logger-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tonic_ragas_logger-1.2.0/README.md` & `tonic_ragas_logger-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tonic_ragas_logger-1.2.0/tonic_ragas_logger/ragas_validate_api.py` & `tonic_ragas_logger-1.2.1/tonic_ragas_logger/ragas_validate_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,10 +110,9 @@
                     llm_context=results.dataset["contexts"][i],
                 )
             )
 
         return Run(
             overall_scores=overall_scores,
             run_data=run_data,
-            llm_evaluator=None,
             id=None,
         )
```

### Comparing `tonic_ragas_logger-1.2.0/tonic_ragas_logger/utils/http_client.py` & `tonic_ragas_logger-1.2.1/tonic_ragas_logger/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `tonic_ragas_logger-1.2.0/PKG-INFO` & `tonic_ragas_logger-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonic-ragas-logger
-Version: 1.2.0
+Version: 1.2.1
 Summary: Uploads results from ragas to Tonic Validate.
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

