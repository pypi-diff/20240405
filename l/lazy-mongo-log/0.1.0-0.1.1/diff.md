# Comparing `tmp/lazy_mongo_log-0.1.0.tar.gz` & `tmp/lazy_mongo_log-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_mongo_log-0.1.0.tar", max compression
+gzip compressed data, was "lazy_mongo_log-0.1.1.tar", max compression
```

## Comparing `lazy_mongo_log-0.1.0.tar` & `lazy_mongo_log-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-04-05 03:06:13.339284 lazy_mongo_log-0.1.0/README.md
--rw-r--r--   0        0        0       41 2024-04-05 04:53:06.661714 lazy_mongo_log-0.1.0/lazy_mongo_log/__init__.py
--rw-r--r--   0        0        0     4452 2024-04-05 04:55:50.472055 lazy_mongo_log-0.1.0/lazy_mongo_log/lazy_mongo_log.py
--rw-r--r--   0        0        0      199 2024-04-05 03:29:29.197277 lazy_mongo_log-0.1.0/lazy_mongo_log/schemas.py
--rw-r--r--   0        0        0      323 2024-04-05 03:07:42.665889 lazy_mongo_log-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 lazy_mongo_log-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-05 03:06:13.339284 lazy_mongo_log-0.1.1/README.md
+-rw-r--r--   0        0        0       41 2024-04-05 04:53:06.661714 lazy_mongo_log-0.1.1/lazy_mongo_log/__init__.py
+-rw-r--r--   0        0        0     4447 2024-04-05 05:02:43.264981 lazy_mongo_log-0.1.1/lazy_mongo_log/lazy_mongo_log.py
+-rw-r--r--   0        0        0      199 2024-04-05 03:29:29.197277 lazy_mongo_log-0.1.1/lazy_mongo_log/schemas.py
+-rw-r--r--   0        0        0      323 2024-04-05 05:02:48.641039 lazy_mongo_log-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 lazy_mongo_log-0.1.1/PKG-INFO
```

### Comparing `lazy_mongo_log-0.1.0/lazy_mongo_log/lazy_mongo_log.py` & `lazy_mongo_log-0.1.1/lazy_mongo_log/lazy_mongo_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class LazyMongoLog:
     def __init__(
         self,
         collection: Collection = None,  # type: ignore
         type: str = "info",
         keyword: Optional[str] = None,
         use_console: bool = True,
-        log_selector: Callable[[dict, ...], dict] = None,  # type: ignore
+        log_selector: Callable[[dict], dict] = None,  # type: ignore
     ):
         self.collection = collection
         self.type = type
         self.keyword = keyword
         self.use_console = use_console
         self.log_selector = log_selector
```

### Comparing `lazy_mongo_log-0.1.0/PKG-INFO` & `lazy_mongo_log-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-mongo-log
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: MisterNyan
 Author-email: michael.edmund.wong@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

