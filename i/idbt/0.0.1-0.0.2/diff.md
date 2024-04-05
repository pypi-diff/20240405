# Comparing `tmp/idbt-0.0.1.tar.gz` & `tmp/idbt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idbt-0.0.1.tar", last modified: Wed Mar 27 03:45:04 2024, max compression
+gzip compressed data, was "idbt-0.0.2.tar", last modified: Fri Apr  5 02:56:50 2024, max compression
```

## Comparing `idbt-0.0.1.tar` & `idbt-0.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 03:45:04.825405 idbt-0.0.1/
--rw-r--r--   0 root         (0) root         (0)      875 2024-03-27 03:45:04.825405 idbt-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-21 08:25:20.000000 idbt-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 03:45:04.825405 idbt-0.0.1/idbt/
--rw-r--r--   0 root         (0) root         (0)      340 2024-03-21 08:42:30.000000 idbt-0.0.1/idbt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 03:45:04.825405 idbt-0.0.1/idbt/compiler/
--rw-r--r--   0 root         (0) root         (0)     1217 2024-03-23 09:26:53.000000 idbt-0.0.1/idbt/compiler/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 03:45:04.825405 idbt-0.0.1/idbt/context/
--rw-r--r--   0 root         (0) root         (0)      467 2024-03-26 08:12:43.000000 idbt-0.0.1/idbt/context/i_unit_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 03:45:04.825405 idbt-0.0.1/idbt/events/
--rw-r--r--   0 root         (0) root         (0)     1164 2024-03-26 10:30:58.000000 idbt-0.0.1/idbt/events/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 03:45:04.825405 idbt-0.0.1/idbt/graph/
--rw-r--r--   0 root         (0) root         (0)     1310 2024-03-25 08:02:44.000000 idbt-0.0.1/idbt/graph/selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 03:45:04.825405 idbt-0.0.1/idbt/loader/
--rw-r--r--   0 root         (0) root         (0)     1464 2024-03-27 02:22:53.000000 idbt-0.0.1/idbt/loader/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1398 2024-03-27 02:19:05.000000 idbt-0.0.1/idbt/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 03:45:04.825405 idbt-0.0.1/idbt/manifest/
--rw-r--r--   0 root         (0) root         (0)      838 2024-03-27 02:28:06.000000 idbt-0.0.1/idbt/manifest/__init__.py
--rw-r--r--   0 root         (0) root         (0)       75 2024-03-22 04:44:29.000000 idbt-0.0.1/idbt/manifest/base.py
--rw-r--r--   0 root         (0) root         (0)     1352 2024-03-27 03:27:03.000000 idbt-0.0.1/idbt/manifest/i_unit_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 03:45:04.825405 idbt-0.0.1/idbt/parser/
--rw-r--r--   0 root         (0) root         (0)      282 2024-03-22 03:44:12.000000 idbt-0.0.1/idbt/parser/base.py
--rw-r--r--   0 root         (0) root         (0)     1653 2024-03-27 03:25:45.000000 idbt-0.0.1/idbt/parser/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 03:45:04.825405 idbt-0.0.1/idbt/task/
--rw-r--r--   0 root         (0) root         (0)    13275 2024-03-27 03:41:13.000000 idbt-0.0.1/idbt/task/i_unit_test.py
--rw-r--r--   0 root         (0) root         (0)     2296 2024-03-26 10:28:26.000000 idbt-0.0.1/idbt/task/seed.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 03:45:04.825405 idbt-0.0.1/idbt/unittest_func_hook/
--rw-r--r--   0 root         (0) root         (0)     2187 2024-03-21 08:11:56.000000 idbt-0.0.1/idbt/unittest_func_hook/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 03:45:04.825405 idbt-0.0.1/idbt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      875 2024-03-27 03:45:04.000000 idbt-0.0.1/idbt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      570 2024-03-27 03:45:04.000000 idbt-0.0.1/idbt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 03:45:04.000000 idbt-0.0.1/idbt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-03-27 03:45:04.000000 idbt-0.0.1/idbt.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 03:45:04.000000 idbt-0.0.1/idbt.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       16 2024-03-27 03:45:04.000000 idbt-0.0.1/idbt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-03-27 03:45:04.000000 idbt-0.0.1/idbt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-27 03:45:04.825405 idbt-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2289 2024-03-22 10:31:30.000000 idbt-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 02:56:50.413177 idbt-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)      875 2024-04-05 02:56:50.413177 idbt-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-21 08:25:20.000000 idbt-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 02:56:50.413177 idbt-0.0.2/idbt/
+-rw-r--r--   0 root         (0) root         (0)      340 2024-03-21 08:42:30.000000 idbt-0.0.2/idbt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 02:56:50.413177 idbt-0.0.2/idbt/compiler/
+-rw-r--r--   0 root         (0) root         (0)     1217 2024-03-23 09:26:53.000000 idbt-0.0.2/idbt/compiler/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 02:56:50.413177 idbt-0.0.2/idbt/context/
+-rw-r--r--   0 root         (0) root         (0)      467 2024-03-26 08:12:43.000000 idbt-0.0.2/idbt/context/i_unit_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 02:56:50.413177 idbt-0.0.2/idbt/events/
+-rw-r--r--   0 root         (0) root         (0)     1353 2024-03-28 02:46:30.000000 idbt-0.0.2/idbt/events/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 02:56:50.413177 idbt-0.0.2/idbt/graph/
+-rw-r--r--   0 root         (0) root         (0)     1310 2024-03-25 08:02:44.000000 idbt-0.0.2/idbt/graph/selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 02:56:50.413177 idbt-0.0.2/idbt/loader/
+-rw-r--r--   0 root         (0) root         (0)     1464 2024-03-27 02:22:53.000000 idbt-0.0.2/idbt/loader/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1398 2024-03-27 02:19:05.000000 idbt-0.0.2/idbt/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 02:56:50.413177 idbt-0.0.2/idbt/manifest/
+-rw-r--r--   0 root         (0) root         (0)      838 2024-03-27 02:28:06.000000 idbt-0.0.2/idbt/manifest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       75 2024-03-22 04:44:29.000000 idbt-0.0.2/idbt/manifest/base.py
+-rw-r--r--   0 root         (0) root         (0)     1352 2024-03-27 03:27:03.000000 idbt-0.0.2/idbt/manifest/i_unit_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 02:56:50.413177 idbt-0.0.2/idbt/parser/
+-rw-r--r--   0 root         (0) root         (0)      282 2024-03-22 03:44:12.000000 idbt-0.0.2/idbt/parser/base.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2024-03-27 03:25:45.000000 idbt-0.0.2/idbt/parser/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 02:56:50.413177 idbt-0.0.2/idbt/task/
+-rw-r--r--   0 root         (0) root         (0)    15204 2024-03-28 03:06:12.000000 idbt-0.0.2/idbt/task/i_unit_test.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2024-03-26 10:28:26.000000 idbt-0.0.2/idbt/task/seed.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 02:56:50.413177 idbt-0.0.2/idbt/unittest_func_hook/
+-rw-r--r--   0 root         (0) root         (0)     2187 2024-03-21 08:11:56.000000 idbt-0.0.2/idbt/unittest_func_hook/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 02:56:50.413177 idbt-0.0.2/idbt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      875 2024-04-05 02:56:50.000000 idbt-0.0.2/idbt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      570 2024-04-05 02:56:50.000000 idbt-0.0.2/idbt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 02:56:50.000000 idbt-0.0.2/idbt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-05 02:56:50.000000 idbt-0.0.2/idbt.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 03:45:04.000000 idbt-0.0.2/idbt.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-05 02:56:50.000000 idbt-0.0.2/idbt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-05 02:56:50.000000 idbt-0.0.2/idbt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 02:56:50.413177 idbt-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2311 2024-04-05 02:55:14.000000 idbt-0.0.2/setup.py
```

### Comparing `idbt-0.0.1/PKG-INFO` & `idbt-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbt
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is inter-k internal tool to help data practice becomes more testable
 Home-page: https://gitlab.inter-k.com/inter-k/internal-software/rnd/idbt
 Author: Bảo Phan
 Author-email: bao.phan1441@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `idbt-0.0.1/idbt/compiler/__init__.py` & `idbt-0.0.2/idbt/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.1/idbt/events/types.py` & `idbt-0.0.2/idbt/events/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,28 +14,36 @@
 }
 
 
 def color(text: str, color_code: str) -> str:
     return "{}{}{}".format(color_code, text, COLORS["reset_all"])
 
 
+def yellow(text: str) -> str:
+    return color(text, COLORS["yellow"])
+
+
 def red(text: str) -> str:
     return color(text, COLORS["red"])
 
 
 def blue(text: str) -> str:
     return color(text, COLORS["blue"])
 
 
 class LogModelResult(InfoLevel):
     def code(self) -> str:
         return "IK001"
 
     def message(self) -> str:
-        if self.status == "error":
+
+        if self.index == 0 and self.total == 0:
+            info = "OK"
+            status = yellow("NONE TEST")
+        elif self.status == "error":
             info = "ERROR creating"
             status = red("UNIT TEST")
         else:
             info = "OK created"
             status = blue("UNIT TEST")
 
         msg = f"{info} {self.description}"
```

### Comparing `idbt-0.0.1/idbt/graph/selector.py` & `idbt-0.0.2/idbt/graph/selector.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.1/idbt/loader/__init__.py` & `idbt-0.0.2/idbt/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.1/idbt/main.py` & `idbt-0.0.2/idbt/main.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.1/idbt/manifest/__init__.py` & `idbt-0.0.2/idbt/manifest/__init__.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.1/idbt/manifest/i_unit_test.py` & `idbt-0.0.2/idbt/manifest/i_unit_test.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.1/idbt/parser/yaml_parser.py` & `idbt-0.0.2/idbt/parser/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.1/idbt/task/i_unit_test.py` & `idbt-0.0.2/idbt/task/i_unit_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from dataclasses import dataclass
+from datetime import datetime
+import time
 from typing import AbstractSet, List, Optional
 from dbt.task.run import RunTask, ModelRunner, fire_event
 from dbt.contracts.graph.manifest import Manifest
 from dbt.graph import UniqueId
 from dbt.contracts.graph.nodes import ModelNode, SeedNode
 from idbt.context.i_unit_test import IUnitTestContext
 from dbt.config.runtime import RuntimeConfig
@@ -17,14 +19,16 @@
 )
 from dbt.contracts.results import NodeStatus, RunResult
 from dbt.events.types import (
     LogStartLine,
 )
 from dbt.events.base_types import EventLevel
 from idbt.events.types import LogModelResult as LogIUnitTestResult
+from dbt.contracts.results import RunStatus
+from dbt.adapters.factory import get_adapter
 
 PARAMETER_PREFIX = "unittest_param"
 
 
 @dataclass
 class TestInputFilesMapper:
     key: str
@@ -40,26 +44,23 @@
     def __init__(self, config, adapter, node, node_index, num_nodes) -> None:
         super().__init__(config, adapter, node, node_index, num_nodes)
 
     def compile_and_execute(self, manifest: Manifest, ctx):
         """
         This hook is to load the IDBT manifest before execute each model
         """
-        try:
-            runtime_config: RuntimeConfig = self.config
-            self.idbt_manifest = FileLoader().load(runtime_config.model_paths)
-            self.seednodes = []
-            for key in manifest.nodes:
-                node = manifest.nodes[key]
-                if isinstance(node, SeedNode):
-                    self.seednodes.append(node)
-            result = super().compile_and_execute(manifest, ctx)
-            return result
-        finally:
-            self._delete_unused_schemas()
+        runtime_config: RuntimeConfig = self.config
+        self.idbt_manifest = FileLoader().load(runtime_config.model_paths)
+        self.seednodes = []
+        for key in manifest.nodes:
+            node = manifest.nodes[key]
+            if isinstance(node, SeedNode):
+                self.seednodes.append(node)
+        result = super().compile_and_execute(manifest, ctx)
+        return result
 
     def execute(self, model: ModelNode, manifest: Manifest):
         result: RunResult = None
         is_fail_test = False
         if model.identifier in self.idbt_manifest.i_unit_test:
             unit_test_definitions = self.idbt_manifest.i_unit_test[model.identifier]
 
@@ -70,29 +71,57 @@
                     model,
                     test_index,
                     unit_test_definitions.__len__(),
                 )
                 result = compiled_model_result
                 is_fail_test = True if assert_result == False else is_fail_test
 
+        if result == None:
+            return RunResult(
+                status=RunStatus.Success,
+                thread_id="thread_id",
+                execution_time=0,
+                timing=[],
+                message="NOT_FOUND_UNIT_TEST",
+                node=model,
+                adapter_response={},
+                failures=None,
+            )
         result.status = NodeStatus.Error if is_fail_test else result.status
         return result
 
-    def print_result_line(self, result):
+    def print_result_line(self, result: RunResult):
         """
-        This hook is to skip model success print
+        This hook is to skip model success print and print a warn message for models don't have unittest
         """
+        if result.message == "NOT_FOUND_UNIT_TEST":
+            fire_event(
+                LogIUnitTestResult(
+                    description=f"""Not found any unittest for model: {self.node.identifier}""",
+                    status=result.status,
+                    index=0,
+                    total=0,
+                    execution_time=result.execution_time,
+                    node_info=self.node.node_info,
+                ),
+                level=EventLevel.INFO,
+            )
         if result.status == NodeStatus.Success:
             return
         super().print_result_line(result)
 
     def describe_node(self):
         """This hook is to change describe of loging"""
         return f"""All unittests for model: {self.node.identifier}"""
 
+    def after_execute(self, result):
+        """This hook is to skip handle NodeResult return in execute function if it's None"""
+        if result != None:
+            super().after_execute(result)
+
     def _execute_unit_test(
         self,
         unit_test_definition: IUnitTestDefinition,
         manifest: Manifest,
         model: ModelNode,
         test_index: int,
         total_test_case: int,
@@ -165,19 +194,14 @@
                 description=self._get_unit_test_description(unit_test_definition),
                 index=test_index,
                 total=total_test_case,
                 node_info=self.node.node_info,
             )
         )
 
-    def _delete_unused_schemas(self):
-        with self.adapter.connection_named(f"unit_test_delete_unused_schemas"):
-            for relation in self.i_unit_test_context.required_schemas:
-                self.adapter.drop_schema(relation)
-
     def _execute_assert_macro(
         self,
         unit_test_definition: IUnitTestDefinition,
         manifest: Manifest,
         model: ModelNode,
         expected_output_seednode: SeedNode,
     ) -> bool:
@@ -242,15 +266,15 @@
     ):
         """
         Execute the SeedTask with overiding flags
         Used editted manifest to ensure that the seednodes' schema is changed
         """
 
         flags = copy.deepcopy(self.i_unit_test_context.flags)
-        flags.__setattr__("show", False)
+        object.__setattr__(flags, "show", False)
         # EVENT_MANAGER is inialized globally, so reset flag log level won't work
         # flags.__setattr__("QUIET", True)
         # flags.__setattr__("quiet", True)
         # flags.__setattr__("log_level", "error")
         # flags.__setattr__("LOG_LEVEL", "error")
         task = IUnitTestSeedTask(
             flags,
@@ -340,7 +364,33 @@
         """
         This hook is to get the required_schemas and assign it into IUnitTestContext
         """
         required_schemas = self.get_model_schemas(adapter, selected_uids)
         for required_schema in required_schemas:
             self.i_unit_test_context.required_schemas.add(required_schema)
         super().before_run(adapter, selected_uids)
+
+    def _delete_unusage_schemas(self, adapter):
+        with adapter.connection_named(f"unit_test_delete_unused_schemas"):
+            for relation in self.i_unit_test_context.required_schemas:
+                adapter.drop_schema(relation)
+
+    def execute_with_hooks(self, selected_uids: AbstractSet[str]):
+        """
+        This hook is to delete unusage schema in finally block of code
+        """
+        adapter = get_adapter(self.config)
+        self.started_at = time.time()
+        try:
+            self.before_run(adapter, selected_uids)
+            res = self.execute_nodes()
+            self.after_run(adapter, res)
+        finally:
+            self._delete_unusage_schemas(adapter)
+            adapter.cleanup_connections()
+            elapsed = time.time() - self.started_at
+            self.print_results_line(self.node_results, elapsed)
+            result = self.get_result(
+                results=self.node_results, elapsed_time=elapsed, generated_at=datetime.utcnow()
+            )
+
+        return result
```

### Comparing `idbt-0.0.1/idbt/task/seed.py` & `idbt-0.0.2/idbt/task/seed.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.1/idbt/unittest_func_hook/__init__.py` & `idbt-0.0.2/idbt/unittest_func_hook/__init__.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.1/idbt.egg-info/PKG-INFO` & `idbt-0.0.2/idbt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbt
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is inter-k internal tool to help data practice becomes more testable
 Home-page: https://gitlab.inter-k.com/inter-k/internal-software/rnd/idbt
 Author: Bảo Phan
 Author-email: bao.phan1441@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `idbt-0.0.1/idbt.egg-info/SOURCES.txt` & `idbt-0.0.2/idbt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idbt-0.0.1/setup.py` & `idbt-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 
 package_name = "idbt"
-package_version = "0.0.1"
+package_version = os.environ["PACKAGE_VERSION"]
 description = """This is inter-k internal tool to help data practice becomes more testable"""
 
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
```

