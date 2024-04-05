# Comparing `tmp/labtech-0.5.0.tar.gz` & `tmp/labtech-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labtech-0.5.0.tar", max compression
+gzip compressed data, was "labtech-0.5.1.tar", max compression
```

## Comparing `labtech-0.5.0.tar` & `labtech-0.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-09-13 02:58:38.522441 labtech-0.5.0/LICENSE
--rw-r--r--   0        0        0     5998 2024-04-03 07:44:55.423715 labtech-0.5.0/README.md
--rw-r--r--   0        0        0      706 2024-04-03 08:02:18.143240 labtech-0.5.0/labtech/__init__.py
--rw-r--r--   0        0        0     6688 2024-04-03 08:01:09.692172 labtech-0.5.0/labtech/cache.py
--rw-r--r--   0        0        0     6554 2024-04-03 08:25:41.385705 labtech-0.5.0/labtech/diagram.py
--rw-r--r--   0        0        0      741 2023-09-13 02:58:38.538441 labtech-0.5.0/labtech/exceptions.py
--rw-r--r--   0        0        0     1396 2024-04-03 08:25:57.589634 labtech-0.5.0/labtech/executors.py
--rw-r--r--   0        0        0    22346 2024-04-03 08:01:09.692172 labtech-0.5.0/labtech/lab.py
--rw-r--r--   0        0        0     4059 2024-04-03 08:27:41.813199 labtech-0.5.0/labtech/mypy_plugin.py
--rw-r--r--   0        0        0        0 2024-02-13 05:01:34.041748 labtech-0.5.0/labtech/py.typed
--rw-r--r--   0        0        0     4630 2024-02-06 01:46:44.484931 labtech-0.5.0/labtech/serialization.py
--rw-r--r--   0        0        0     2455 2024-03-31 09:09:14.445769 labtech-0.5.0/labtech/storage.py
--rw-r--r--   0        0        0     9763 2024-04-03 08:01:09.696173 labtech-0.5.0/labtech/tasks.py
--rw-r--r--   0        0        0     5230 2024-04-03 08:41:02.359333 labtech-0.5.0/labtech/types.py
--rw-r--r--   0        0        0     3090 2024-02-06 01:43:13.057829 labtech-0.5.0/labtech/utils.py
--rw-r--r--   0        0        0     1025 2024-04-03 08:18:31.776056 labtech-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     6949 1970-01-01 00:00:00.000000 labtech-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-09-13 02:58:38.522441 labtech-0.5.1/LICENSE
+-rw-r--r--   0        0        0     6074 2024-04-05 07:15:21.269246 labtech-0.5.1/README.md
+-rw-r--r--   0        0        0      706 2024-04-05 07:21:09.988779 labtech-0.5.1/labtech/__init__.py
+-rw-r--r--   0        0        0     6688 2024-04-03 08:01:09.692172 labtech-0.5.1/labtech/cache.py
+-rw-r--r--   0        0        0     6914 2024-04-05 07:20:35.553228 labtech-0.5.1/labtech/diagram.py
+-rw-r--r--   0        0        0      741 2023-09-13 02:58:38.538441 labtech-0.5.1/labtech/exceptions.py
+-rw-r--r--   0        0        0     1396 2024-04-03 08:25:57.589634 labtech-0.5.1/labtech/executors.py
+-rw-r--r--   0        0        0    22346 2024-04-03 08:01:09.692172 labtech-0.5.1/labtech/lab.py
+-rw-r--r--   0        0        0     4059 2024-04-03 08:27:41.813199 labtech-0.5.1/labtech/mypy_plugin.py
+-rw-r--r--   0        0        0        0 2024-02-13 05:01:34.041748 labtech-0.5.1/labtech/py.typed
+-rw-r--r--   0        0        0     4630 2024-02-06 01:46:44.484931 labtech-0.5.1/labtech/serialization.py
+-rw-r--r--   0        0        0     2455 2024-03-31 09:09:14.445769 labtech-0.5.1/labtech/storage.py
+-rw-r--r--   0        0        0     9763 2024-04-03 08:01:09.696173 labtech-0.5.1/labtech/tasks.py
+-rw-r--r--   0        0        0     5230 2024-04-03 08:41:02.359333 labtech-0.5.1/labtech/types.py
+-rw-r--r--   0        0        0     3090 2024-02-06 01:43:13.057829 labtech-0.5.1/labtech/utils.py
+-rw-r--r--   0        0        0     1025 2024-04-05 07:21:16.020700 labtech-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     7025 1970-01-01 00:00:00.000000 labtech-0.5.1/PKG-INFO
```

### Comparing `labtech-0.5.0/LICENSE` & `labtech-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `labtech-0.5.0/README.md` & `labtech-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 # Decorate your task class with @labtech.task:
 @labtech.task
 class Experiment:
     # Each Experiment task instance will take `base` and `power` parameters:
     base: int
     power: int
 
-    def run(self):
+    def run(self) -> int:
         # Define the task's run() method to return the result of the experiment:
         labtech.logger.info(f'Raising {self.base} to the power of {self.power}')
         sleep(1)
         return self.base ** self.power
 
 def main():
     # Configure Experiment parameter permutations
@@ -109,24 +109,24 @@
 
 import labtech
 
 @labtech.task
 class SlowTask:
     base: int
 
-    def run(self):
+    def run(self) -> int:
         sleep(5)
         return self.base ** 2
 
 @labtech.task
 class DependentTask:
     slow_task: SlowTask
     multiplier: int
 
-    def run(self):
+    def run(self) -> int:
         return self.multiplier * self.slow_task.result
 
 def main():
     some_slow_task = SlowTask(base=42)
     dependent_tasks = [
         DependentTask(
             slow_task=some_slow_task,
@@ -164,17 +164,19 @@
 ```mermaid
 classDiagram
     direction BT
 
     class DependentTask
     DependentTask : SlowTask slow_task
     DependentTask : int multiplier
+    DependentTask : run() int
 
     class SlowTask
     SlowTask : int base
+    SlowTask : run() int
 
 
     DependentTask <-- SlowTask: slow_task
 ```
 
 To learn more, dive into the following resources:
```

### Comparing `labtech-0.5.0/labtech/__init__.py` & `labtech-0.5.1/labtech/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 results = lab.run_tasks(experiments)
 print(results)
 
 ```
 
 """
 
-__version__ = '0.5.0'
+__version__ = '0.5.1'
 
 from .types import is_task, is_task_type
 from .tasks import task
 from .lab import Lab
 from .utils import logger
 
 __all__ = [
```

### Comparing `labtech-0.5.0/labtech/cache.py` & `labtech-0.5.1/labtech/cache.py`

 * *Files identical despite different names*

### Comparing `labtech-0.5.0/labtech/diagram.py` & `labtech-0.5.1/labtech/diagram.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass, fields
 from textwrap import indent
-from typing import Dict, Sequence, Type, get_origin, get_args
+from typing import Dict, Sequence, Type, get_origin, get_args, get_type_hints
 
 from .types import Task, is_task
 from .tasks import find_tasks_in_param
 
 
 @dataclass(frozen=True)
 class TaskRelKey:
@@ -89,21 +89,26 @@
     else:
         # For generic types, format each type argument
         args_str = ', '.join([format_type(arg_t) for arg_t in get_args(t)])
         return f'{origin.__name__}[{args_str}]'
 
 
 def diagram_task_type(task_type: Type[Task]) -> str:
+    run_return_type = get_type_hints(task_type.run).get('return')
+    run_return = (
+        '' if run_return_type is None else f' {format_type(run_return_type)}'
+    )
     return '\n'.join([
-        f'class {task_type.__name__}',
+        f'class {format_type(task_type)}',
         *[
             f'{format_type(task_type)} : {format_type(field.type)} {field.name}'
             for field in fields(task_type)
             if field
-        ]
+        ],
+        f'{format_type(task_type)} : run(){run_return}'
     ])
 
 
 def diagram_task_relationship(from_task_type: Type[Task], relationships: Dict[TaskRelKey, TaskRelInfo]) -> str:
 
     def format_many(multi_cardinality: bool) -> str:
         if multi_cardinality:
@@ -136,14 +141,17 @@
     )
 
 
 def build_task_diagram(tasks: Sequence[Task], *, direction: str = 'BT') -> str:
     """Returns a [Mermaid diagram](https://mermaid.js.org/syntax/classDiagram.html)
     representing the task types and dependencies of the given tasks.
 
+    Each task type lists its parameters (with their return types) and
+    its run method (with its return type).
+
     Arrows between task types point from a dependency task type to the
     task type that depends on it, and are labelled with the dependent
     task's parameter that references the dependency task type.
 
     Args:
         tasks: A collection of tasks to diagram.
         direction: Direction that task types should be laid out, from dependent
```

### Comparing `labtech-0.5.0/labtech/exceptions.py` & `labtech-0.5.1/labtech/exceptions.py`

 * *Files identical despite different names*

### Comparing `labtech-0.5.0/labtech/executors.py` & `labtech-0.5.1/labtech/executors.py`

 * *Files identical despite different names*

### Comparing `labtech-0.5.0/labtech/lab.py` & `labtech-0.5.1/labtech/lab.py`

 * *Files identical despite different names*

### Comparing `labtech-0.5.0/labtech/mypy_plugin.py` & `labtech-0.5.1/labtech/mypy_plugin.py`

 * *Files identical despite different names*

### Comparing `labtech-0.5.0/labtech/serialization.py` & `labtech-0.5.1/labtech/serialization.py`

 * *Files identical despite different names*

### Comparing `labtech-0.5.0/labtech/storage.py` & `labtech-0.5.1/labtech/storage.py`

 * *Files identical despite different names*

### Comparing `labtech-0.5.0/labtech/tasks.py` & `labtech-0.5.1/labtech/tasks.py`

 * *Files identical despite different names*

### Comparing `labtech-0.5.0/labtech/types.py` & `labtech-0.5.1/labtech/types.py`

 * *Files identical despite different names*

### Comparing `labtech-0.5.0/labtech/utils.py` & `labtech-0.5.1/labtech/utils.py`

 * *Files identical despite different names*

### Comparing `labtech-0.5.0/pyproject.toml` & `labtech-0.5.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "labtech"
-version = "0.5.0"
+version = "0.5.1"
 license = "GPL-3.0-only"
 description = "Easily run experiment permutations with multi-processing and caching."
 authors = ["Ben Denham <ben@denham.nz>"]
 readme = "README.md"
 repository = "https://github.com/ben-denham/labtech"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

### Comparing `labtech-0.5.0/PKG-INFO` & `labtech-0.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labtech
-Version: 0.5.0
+Version: 0.5.1
 Summary: Easily run experiment permutations with multi-processing and caching.
 Home-page: https://github.com/ben-denham/labtech
 License: GPL-3.0-only
 Author: Ben Denham
 Author-email: ben@denham.nz
 Requires-Python: >=3.10
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -70,15 +70,15 @@
 # Decorate your task class with @labtech.task:
 @labtech.task
 class Experiment:
     # Each Experiment task instance will take `base` and `power` parameters:
     base: int
     power: int
 
-    def run(self):
+    def run(self) -> int:
         # Define the task's run() method to return the result of the experiment:
         labtech.logger.info(f'Raising {self.base} to the power of {self.power}')
         sleep(1)
         return self.base ** self.power
 
 def main():
     # Configure Experiment parameter permutations
@@ -132,24 +132,24 @@
 
 import labtech
 
 @labtech.task
 class SlowTask:
     base: int
 
-    def run(self):
+    def run(self) -> int:
         sleep(5)
         return self.base ** 2
 
 @labtech.task
 class DependentTask:
     slow_task: SlowTask
     multiplier: int
 
-    def run(self):
+    def run(self) -> int:
         return self.multiplier * self.slow_task.result
 
 def main():
     some_slow_task = SlowTask(base=42)
     dependent_tasks = [
         DependentTask(
             slow_task=some_slow_task,
@@ -187,17 +187,19 @@
 ```mermaid
 classDiagram
     direction BT
 
     class DependentTask
     DependentTask : SlowTask slow_task
     DependentTask : int multiplier
+    DependentTask : run() int
 
     class SlowTask
     SlowTask : int base
+    SlowTask : run() int
 
 
     DependentTask <-- SlowTask: slow_task
 ```
 
 To learn more, dive into the following resources:
```

