# Comparing `tmp/colmena-0.6.0.tar.gz` & `tmp/colmena-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colmena-0.6.0.tar", last modified: Tue Mar 12 17:08:54 2024, max compression
+gzip compressed data, was "colmena-0.6.1.tar", last modified: Fri Apr  5 15:33:23 2024, max compression
```

## Comparing `colmena-0.6.0.tar` & `colmena-0.6.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:08:54.846720 colmena-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-03-12 17:08:47.000000 colmena-0.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19264 2024-03-12 17:08:54.846720 colmena-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-03-12 17:08:47.000000 colmena-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:08:54.838720 colmena-0.6.0/colmena/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:08:54.838720 colmena-0.6.0/colmena/models/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14267 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/models/methods.py
--rw-r--r--   0 runner    (1001) docker     (127)    20785 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/models/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:08:54.842720 colmena-0.6.0/colmena/queue/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13648 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/queue/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/queue/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/queue/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:08:54.842720 colmena-0.6.0/colmena/queue/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/queue/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/queue/tests/test_queues.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:08:54.842720 colmena-0.6.0/colmena/task_server/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/task_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/task_server/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/task_server/globus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/task_server/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    18993 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/task_server/parsl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:08:54.842720 colmena-0.6.0/colmena/task_server/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/task_server/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/task_server/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/task_server/tests/test_globus.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/task_server/tests/test_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/task_server/tests/test_parsl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:08:54.842720 colmena-0.6.0/colmena/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/tests/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/tests/test_task_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:08:54.842720 colmena-0.6.0/colmena/thinker/
--rw-r--r--   0 runner    (1001) docker     (127)    19328 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/thinker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13241 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/thinker/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:08:54.842720 colmena-0.6.0/colmena/thinker/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/thinker/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/thinker/tests/test_thinker.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-12 17:08:47.000000 colmena-0.6.0/colmena/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:08:54.842720 colmena-0.6.0/colmena.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19264 2024-03-12 17:08:54.000000 colmena-0.6.0/colmena.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-12 17:08:54.000000 colmena-0.6.0/colmena.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 17:08:54.000000 colmena-0.6.0/colmena.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-12 17:08:54.000000 colmena-0.6.0/colmena.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-12 17:08:54.000000 colmena-0.6.0/colmena.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-03-12 17:08:47.000000 colmena-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 17:08:54.846720 colmena-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:33:23.164440 colmena-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-05 15:33:16.000000 colmena-0.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19264 2024-04-05 15:33:23.164440 colmena-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-05 15:33:16.000000 colmena-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:33:23.160441 colmena-0.6.1/colmena/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:33:23.160441 colmena-0.6.1/colmena/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14016 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/models/methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20785 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/models/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:33:23.160441 colmena-0.6.1/colmena/queue/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13648 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/queue/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/queue/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/queue/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:33:23.160441 colmena-0.6.1/colmena/queue/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/queue/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/queue/tests/test_queues.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:33:23.164440 colmena-0.6.1/colmena/task_server/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/task_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/task_server/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/task_server/globus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/task_server/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18995 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/task_server/parsl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:33:23.164440 colmena-0.6.1/colmena/task_server/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/task_server/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/task_server/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/task_server/tests/test_globus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/task_server/tests/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/task_server/tests/test_parsl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:33:23.164440 colmena-0.6.1/colmena/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/tests/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/tests/test_task_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:33:23.164440 colmena-0.6.1/colmena/thinker/
+-rw-r--r--   0 runner    (1001) docker     (127)    19328 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/thinker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13241 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/thinker/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:33:23.164440 colmena-0.6.1/colmena/thinker/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/thinker/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/thinker/tests/test_thinker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-05 15:33:16.000000 colmena-0.6.1/colmena/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:33:23.164440 colmena-0.6.1/colmena.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19264 2024-04-05 15:33:23.000000 colmena-0.6.1/colmena.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-05 15:33:23.000000 colmena-0.6.1/colmena.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:33:23.000000 colmena-0.6.1/colmena.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-05 15:33:23.000000 colmena-0.6.1/colmena.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 15:33:23.000000 colmena-0.6.1/colmena.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-05 15:33:16.000000 colmena-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 15:33:23.164440 colmena-0.6.1/setup.cfg
```

### Comparing `colmena-0.6.0/LICENSE.txt` & `colmena-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `colmena-0.6.0/PKG-INFO` & `colmena-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colmena
-Version: 0.6.0
+Version: 0.6.1
 Summary: colmena: Intelligent Steerable Pipelines on HPC
 Author-email: Globus Labs <labs@globus.org>, Logan Ward <lward@anl.gov>, Greg Pauloski <jgpauloski@uchicago.edu>, Yadu Babuji <yadudoc1729@gmail.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `colmena-0.6.0/README.md` & `colmena-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `colmena-0.6.0/colmena/models/methods.py` & `colmena-0.6.1/colmena/models/methods.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import logging
 import platform
 from io import StringIO
 from pathlib import Path
 from subprocess import run
 from tempfile import TemporaryDirectory
 from time import perf_counter
-from inspect import signature, isgeneratorfunction
-from typing import Any, Dict, List, Tuple, Optional, Callable, Generator
+from inspect import signature
+from typing import Any, Dict, List, Tuple, Optional, Callable, Generator, Union, Iterable
 
 from colmena.models.results import ResourceRequirements, Result, FailureInformation
 from colmena.proxy import resolve_proxies_async, store_proxy_stats
 from colmena.queue import ColmenaQueues
 
 
 logger = logging.getLogger(__name__)
@@ -112,16 +112,14 @@
         function: Generator function to be executed
         name: Name of the function. Defaults to `function.__name__`
     """
 
     function: Callable
 
     def __init__(self, function: Callable, name: Optional[str] = None) -> None:
-        if isgeneratorfunction(function):
-            raise ValueError('Function is a generator function. Use `PythonGeneratorTask` instead.')
         self.name = name or function.__name__
         self.function = function
 
 
 class PythonGeneratorMethod(ColmenaMethod):
     """Python function which runs on a single worker and generates results iteratively
 
@@ -132,30 +130,28 @@
         function: Generator function to be executed
         name: Name of the function. Defaults to `function.__name__`
         store_return_value: Whether to capture the `return value <https://docs.python.org/3/reference/simple_stmts.html#the-return-statement>`_
             of the generator and store it in the Result object.
     """
 
     def __init__(self,
-                 function: Callable[..., Generator],
+                 function: Callable[..., Union[Generator, Iterable]],
                  name: Optional[str] = None,
                  store_return_value: bool = False,
                  streaming_queue: Optional[ColmenaQueues] = None) -> None:
-        if not isgeneratorfunction(function):
-            raise ValueError('Function is not a generator function. Use `PythonTask` instead.')
         self._function = function
         self.name = name or function.__name__
         self.store_return_value = store_return_value
         self.streaming_queue = streaming_queue
 
     def stream_result(self, y: Any, result: Result, start_time: float):
         """Send an intermediate result using the task queue
 
         Args:
-            y: Intermediate result
+            y: Yielded data from the generator function
             result: Result package carrying task metadata
             start_time: Start time of the algorithm, used to report
         """
 
         # Store the intermediate result in a copy of the input object
         result = result.copy(deep=True)
         result.set_result(
```

### Comparing `colmena-0.6.0/colmena/models/results.py` & `colmena-0.6.1/colmena/models/results.py`

 * *Files identical despite different names*

### Comparing `colmena-0.6.0/colmena/proxy.py` & `colmena-0.6.1/colmena/proxy.py`

 * *Files identical despite different names*

### Comparing `colmena-0.6.0/colmena/queue/base.py` & `colmena-0.6.1/colmena/queue/base.py`

 * *Files identical despite different names*

### Comparing `colmena-0.6.0/colmena/queue/python.py` & `colmena-0.6.1/colmena/queue/python.py`

 * *Files identical despite different names*

### Comparing `colmena-0.6.0/colmena/queue/redis.py` & `colmena-0.6.1/colmena/queue/redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,27 +70,25 @@
         self.port = port
         self.redis_client = None
         self.prefix = prefix
         assert not any("{" in t for t in self.topics)
         self.connect()
 
     def __setstate__(self, state):
-        self.__dict__ = state
+        super().__setstate__(state)
 
-        # If you find the RedisClient placeholder,
-        #  attempt to reconnect
+        # If you find the RedisClient placeholder, attempt to reconnect
         if self.redis_client == 'connected':
             self.redis_client = None
             self.connect()
 
     def __getstate__(self):
         state = super().__getstate__()
 
-        # If connected, remove the unpicklable RedisClient and
-        #  put a placeholder instead
+        # If connected, remove the unpicklable RedisClient and put a placeholder instead
         if self.is_connected:
             state['redis_client'] = 'connected'
         return state
 
     def connect(self):
         """Connect to the Redis server"""
         try:
```

### Comparing `colmena-0.6.0/colmena/queue/tests/test_base.py` & `colmena-0.6.1/colmena/queue/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `colmena-0.6.0/colmena/queue/tests/test_queues.py` & `colmena-0.6.1/colmena/queue/tests/test_queues.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Tests across different queue implementations"""
 from multiprocessing import Pool
+import pickle as pkl
 
 from pytest import fixture, raises, mark
 from redis import Redis, ConnectionError
 
 from colmena.exceptions import TimeoutException, KillSignalException
 from colmena.queue.base import ColmenaQueues
 from colmena.queue.python import PipeQueues
@@ -75,7 +76,16 @@
 
 
 @mark.timeout(5)
 def test_kill_signal(queue):
     queue.send_kill_signal()
     with raises(KillSignalException):
         queue.get_task()
+
+
+def test_pickle(queue):
+    """Ensure that we can still send and receive after pickling"""
+    queue: ColmenaQueues = pkl.loads(pkl.dumps(queue))
+
+    queue.send_inputs(1, method='test')
+    _, task = queue.get_task()
+    assert task.method == 'test'
```

### Comparing `colmena-0.6.0/colmena/task_server/base.py` & `colmena-0.6.1/colmena/task_server/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,13 +166,16 @@
 
     Args:
         function: User-provided function
     Returns:
         Function as appropriate subclasses of Colmena Task wrapper
     """
 
+    name = function.__name__
     if isinstance(function, ColmenaMethod):
         return function
     elif isgeneratorfunction(function):
+        logger.info(f'Assigned a PythonGeneratorMethod wrapper to {name}')
         return PythonGeneratorMethod(function)
     else:
+        logger.info(f'Assigned a PythonMethod wrapper to {name}')
         return PythonMethod(function)
```

### Comparing `colmena-0.6.0/colmena/task_server/globus.py` & `colmena-0.6.1/colmena/task_server/globus.py`

 * *Files identical despite different names*

### Comparing `colmena-0.6.0/colmena/task_server/local.py` & `colmena-0.6.1/colmena/task_server/local.py`

 * *Files identical despite different names*

### Comparing `colmena-0.6.0/colmena/task_server/parsl.py` & `colmena-0.6.1/colmena/task_server/parsl.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,15 +349,15 @@
                 function, options = method
             else:
                 function = method
                 options = {'executors': default_executors}
                 logger.info(f'Using default executors for {function.__name__}: {default_executors}')
 
             # Convert the function to a Colmena task
-            function = convert_to_colmena_method(method)
+            function = convert_to_colmena_method(function)
             name = function.name
 
             # If the function is not an executable, submit it as a single task
             if not isinstance(function, ExecutableMethod):
                 app = PythonApp(function, **options)
                 self.methods_[name] = (app, 'basic')
             else:
```

### Comparing `colmena-0.6.0/colmena/task_server/tests/test_base.py` & `colmena-0.6.1/colmena/task_server/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `colmena-0.6.0/colmena/task_server/tests/test_globus.py` & `colmena-0.6.1/colmena/task_server/tests/test_globus.py`

 * *Files identical despite different names*

### Comparing `colmena-0.6.0/colmena/task_server/tests/test_local.py` & `colmena-0.6.1/colmena/task_server/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `colmena-0.6.0/colmena/task_server/tests/test_parsl.py` & `colmena-0.6.1/colmena/task_server/tests/test_parsl.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         yield store
         unregister_store(store.name)
 
 
 @fixture(autouse=True)
 def server_and_queue(config, store) -> Tuple[ParslTaskServer, ColmenaQueues]:
     queues = PipeQueues(proxystore_name='store', proxystore_threshold=5000, serialization_method='pickle')
-    server = ParslTaskServer([f, capitalize, bad_task, EchoTask(), FakeMPITask(), count_nodes], queues, config)
+    server = ParslTaskServer([(f, {'executors': 'all'}), capitalize, bad_task, EchoTask(), FakeMPITask(), count_nodes], queues, config)
     yield server, queues
     if server.is_alive():
         queues.send_kill_signal()
         server.join(timeout=30)
 
 
 @mark.timeout(30)
```

### Comparing `colmena-0.6.0/colmena/tests/test_model.py` & `colmena-0.6.1/colmena/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `colmena-0.6.0/colmena/tests/test_proxy.py` & `colmena-0.6.1/colmena/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `colmena-0.6.0/colmena/tests/test_task_model.py` & `colmena-0.6.1/colmena/tests/test_task_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Tuple, List, Optional, Dict, Any, Iterator
+from functools import lru_cache, update_wrapper
 from pathlib import Path
 from math import isnan
 
 from pytest import fixture
 from proxystore.connectors.file import FileConnector
 from proxystore.store import Store
 from proxystore.store import register_store
@@ -163,7 +164,21 @@
     assert result.time.deserialize_inputs > 0
     assert result.time.serialize_results > 0
     assert result.timestamp.compute_ended >= result.timestamp.compute_started
 
     # Make sure we have stats for both proxies
     assert len(result.time.proxy) == 2
     assert all('store.proxy' in v['times'] for v in result.time.proxy.values())
+
+
+def test_with_decorator(result):
+    """Ensure streaming still works with decorators"""
+
+    dec = lru_cache()(generator)
+    update_wrapper(dec, generator)
+    task = PythonGeneratorMethod(function=generator, store_return_value=True)
+    assert task.name == 'generator'
+
+    result = task(result)
+    assert result.success, result.failure_info.traceback
+    result.deserialize()
+    assert result.value == [[0], 'done']
```

### Comparing `colmena-0.6.0/colmena/thinker/__init__.py` & `colmena-0.6.1/colmena/thinker/__init__.py`

 * *Files identical despite different names*

### Comparing `colmena-0.6.0/colmena/thinker/resources.py` & `colmena-0.6.1/colmena/thinker/resources.py`

 * *Files identical despite different names*

### Comparing `colmena-0.6.0/colmena/thinker/tests/test_resources.py` & `colmena-0.6.1/colmena/thinker/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `colmena-0.6.0/colmena/thinker/tests/test_thinker.py` & `colmena-0.6.1/colmena/thinker/tests/test_thinker.py`

 * *Files identical despite different names*

### Comparing `colmena-0.6.0/colmena.egg-info/PKG-INFO` & `colmena-0.6.1/colmena.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colmena
-Version: 0.6.0
+Version: 0.6.1
 Summary: colmena: Intelligent Steerable Pipelines on HPC
 Author-email: Globus Labs <labs@globus.org>, Logan Ward <lward@anl.gov>, Greg Pauloski <jgpauloski@uchicago.edu>, Yadu Babuji <yadudoc1729@gmail.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `colmena-0.6.0/colmena.egg-info/SOURCES.txt` & `colmena-0.6.1/colmena.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `colmena-0.6.0/pyproject.toml` & `colmena-0.6.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "colmena"
-version = "0.6.0"
+version = "0.6.1"
 authors = [
     { name = "Globus Labs", email = "labs@globus.org" },
     { name = "Logan Ward", email = "lward@anl.gov" },
     { name = "Greg Pauloski", email = "jgpauloski@uchicago.edu" },
     { name = "Yadu Babuji", email = "yadudoc1729@gmail.com" },
 ]
 description = 'colmena: Intelligent Steerable Pipelines on HPC'
```

