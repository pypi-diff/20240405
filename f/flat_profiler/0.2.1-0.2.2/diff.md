# Comparing `tmp/flat_profiler-0.2.1.tar.gz` & `tmp/flat_profiler-0.2.2.tar.gz`

## Comparing `flat_profiler-0.2.1.tar` & `flat_profiler-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 flat_profiler-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 flat_profiler-0.2.1/example/simple.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 flat_profiler-0.2.1/flat_profiler/__about__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 flat_profiler-0.2.1/flat_profiler/__init__.py
--rw-r--r--   0        0        0     7493 2020-02-02 00:00:00.000000 flat_profiler-0.2.1/flat_profiler/flat_profiler.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 flat_profiler-0.2.1/flat_profiler/performance.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flat_profiler-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 flat_profiler-0.2.1/tests/test_flat_profiler.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 flat_profiler-0.2.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 flat_profiler-0.2.1/LICENSE
--rw-r--r--   0        0        0     7224 2020-02-02 00:00:00.000000 flat_profiler-0.2.1/README.md
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 flat_profiler-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     8284 2020-02-02 00:00:00.000000 flat_profiler-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 flat_profiler-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 flat_profiler-0.2.2/example/simple.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 flat_profiler-0.2.2/flat_profiler/__about__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 flat_profiler-0.2.2/flat_profiler/__init__.py
+-rw-r--r--   0        0        0     7493 2020-02-02 00:00:00.000000 flat_profiler-0.2.2/flat_profiler/flat_profiler.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 flat_profiler-0.2.2/flat_profiler/performance.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flat_profiler-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 flat_profiler-0.2.2/tests/test_flat_profiler.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 flat_profiler-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 flat_profiler-0.2.2/LICENSE
+-rw-r--r--   0        0        0     7228 2020-02-02 00:00:00.000000 flat_profiler-0.2.2/README.md
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 flat_profiler-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     8288 2020-02-02 00:00:00.000000 flat_profiler-0.2.2/PKG-INFO
```

### Comparing `flat_profiler-0.2.1/.pre-commit-config.yaml` & `flat_profiler-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `flat_profiler-0.2.1/example/simple.py` & `flat_profiler-0.2.2/example/simple.py`

 * *Files identical despite different names*

### Comparing `flat_profiler-0.2.1/flat_profiler/flat_profiler.py` & `flat_profiler-0.2.2/flat_profiler/flat_profiler.py`

 * *Files identical despite different names*

### Comparing `flat_profiler-0.2.1/flat_profiler/performance.py` & `flat_profiler-0.2.2/flat_profiler/performance.py`

 * *Files identical despite different names*

### Comparing `flat_profiler-0.2.1/tests/test_flat_profiler.py` & `flat_profiler-0.2.2/tests/test_flat_profiler.py`

 * *Files identical despite different names*

### Comparing `flat_profiler-0.2.1/LICENSE` & `flat_profiler-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flat_profiler-0.2.1/README.md` & `flat_profiler-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Flat Profiler
 
 This package provides a flat profiler, which collects execution time information for only the decorated function or method.
 
 
 # Installation
 
-`pip install flat_profile`
+`pip install flat_profiler`
 
 
 # Usage
 
-This decorator uses call wrapping from [Recompyle](https://github.com/DanWehr/recompyle) to record the execution times of all calls, of the decorated function. A time limit must be provided, and if the total time is below/above that limit then below/above callbacks will execute.
+This decorator uses call wrapping from [Recompyle](https://github.com/DanWehr/recompyle) to record the execution times of all calls within the decorated function. A time limit must be provided, and if the total time is below/above that limit then below/above callbacks will execute.
 
 The default `below` callback will create a log message with only the total time. The default `above` callback will log the total as well as all call execution times, sorted by highest duration first.
 
 Multiple call times for the same name (e.g. from multiple `int()` calls) will be summed together for the default logging. Custom callbacks used instead of the default ones will receive the times of all individual calls.
 
 ```python
 import logging
```

### Comparing `flat_profiler-0.2.1/pyproject.toml` & `flat_profiler-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flat_profiler-0.2.1/PKG-INFO` & `flat_profiler-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flat_profiler
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python flat profiling tool.
 Project-URL: Homepage, https://github.com/DanWehr/flat_profiler
 Project-URL: Documentation, https://github.com/DanWehr/flat_profiler#readme
 Project-URL: Issues, https://github.com/DanWehr/flat_profiler/issues
 Project-URL: Repository, https://github.com/DanWehr/flat_profiler.git
 Author-email: Daniel Wehr <danwehr@gmail.com>
 License-Expression: MIT
@@ -26,20 +26,20 @@
 # Flat Profiler
 
 This package provides a flat profiler, which collects execution time information for only the decorated function or method.
 
 
 # Installation
 
-`pip install flat_profile`
+`pip install flat_profiler`
 
 
 # Usage
 
-This decorator uses call wrapping from [Recompyle](https://github.com/DanWehr/recompyle) to record the execution times of all calls, of the decorated function. A time limit must be provided, and if the total time is below/above that limit then below/above callbacks will execute.
+This decorator uses call wrapping from [Recompyle](https://github.com/DanWehr/recompyle) to record the execution times of all calls within the decorated function. A time limit must be provided, and if the total time is below/above that limit then below/above callbacks will execute.
 
 The default `below` callback will create a log message with only the total time. The default `above` callback will log the total as well as all call execution times, sorted by highest duration first.
 
 Multiple call times for the same name (e.g. from multiple `int()` calls) will be summed together for the default logging. Custom callbacks used instead of the default ones will receive the times of all individual calls.
 
 ```python
 import logging
```

