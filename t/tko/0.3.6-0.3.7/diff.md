# Comparing `tmp/tko-0.3.6.tar.gz` & `tmp/tko-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tko-0.3.6.tar", last modified: Wed Apr  3 16:44:33 2024, max compression
+gzip compressed data, was "tko-0.3.7.tar", last modified: Fri Apr  5 15:55:27 2024, max compression
```

## Comparing `tko-0.3.6.tar` & `tko-0.3.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 16:44:33.336644 tko-0.3.6/
--rw-r--r--   0 lion      (1000) lion      (1000)     1043 2023-08-02 17:52:17.000000 tko-0.3.6/LICENSE
--rw-r--r--   0 lion      (1000) lion      (1000)      191 2023-08-02 17:33:10.000000 tko-0.3.6/MANIFEST.in
--rw-r--r--   0 lion      (1000) lion      (1000)     6765 2024-04-03 16:44:33.336644 tko-0.3.6/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)     5911 2024-04-02 11:33:20.000000 tko-0.3.6/Readme.md
--rw-r--r--   0 lion      (1000) lion      (1000)     2991 2024-04-03 02:01:18.000000 tko-0.3.6/changelog.md
--rw-r--r--   0 lion      (1000) lion      (1000)      298 2023-08-02 17:36:39.000000 tko-0.3.6/requirements.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-03 16:44:33.336644 tko-0.3.6/setup.cfg
--rw-r--r--   0 lion      (1000) lion      (1000)     3969 2024-04-02 11:33:20.000000 tko-0.3.6/setup.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 16:44:33.323311 tko-0.3.6/src/
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 16:44:33.329978 tko-0.3.6/src/tko/
--rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-03 12:38:49.000000 tko-0.3.6/src/tko/__init__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     9370 2024-04-03 12:42:46.000000 tko-0.3.6/src/tko/__main__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     6667 2024-04-03 12:43:36.000000 tko-0.3.6/src/tko/actions.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4516 2024-04-03 12:42:24.000000 tko-0.3.6/src/tko/basic.py
--rw-r--r--   0 lion      (1000) lion      (1000)    10034 2023-10-19 13:10:37.000000 tko-0.3.6/src/tko/diff.py
--rw-r--r--   0 lion      (1000) lion      (1000)     7521 2024-03-21 14:49:39.000000 tko-0.3.6/src/tko/down.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4997 2024-04-03 01:50:45.000000 tko-0.3.6/src/tko/filter.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5747 2023-10-07 23:37:00.000000 tko-0.3.6/src/tko/format.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2727 2024-03-13 17:39:00.000000 tko-0.3.6/src/tko/guide.py
--rw-r--r--   0 lion      (1000) lion      (1000)     8104 2024-04-02 18:12:46.000000 tko-0.3.6/src/tko/loader.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2567 2023-08-03 03:39:13.000000 tko-0.3.6/src/tko/pattern.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1803 2023-10-19 18:36:35.000000 tko-0.3.6/src/tko/runner.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5609 2024-03-20 21:47:04.000000 tko-0.3.6/src/tko/settings.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4426 2024-03-22 11:32:02.000000 tko-0.3.6/src/tko/solver.py
--rw-r--r--   0 lion      (1000) lion      (1000)     7124 2024-04-02 11:33:20.000000 tko-0.3.6/src/tko/wdir.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3177 2024-04-02 11:33:20.000000 tko-0.3.6/src/tko/writer.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 16:44:33.333311 tko-0.3.6/src/tko.egg-info/
--rw-r--r--   0 lion      (1000) lion      (1000)     6765 2024-04-03 16:44:33.000000 tko-0.3.6/src/tko.egg-info/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)      554 2024-04-03 16:44:33.000000 tko-0.3.6/src/tko.egg-info/SOURCES.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-03 16:44:33.000000 tko-0.3.6/src/tko.egg-info/dependency_links.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       47 2024-04-03 16:44:33.000000 tko-0.3.6/src/tko.egg-info/entry_points.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       59 2024-04-03 16:44:33.000000 tko-0.3.6/src/tko.egg-info/requires.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        4 2024-04-03 16:44:33.000000 tko-0.3.6/src/tko.egg-info/top_level.txt
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-05 15:55:27.236359 tko-0.3.7/
+-rw-r--r--   0 lion      (1000) lion      (1000)     1043 2023-08-02 17:52:17.000000 tko-0.3.7/LICENSE
+-rw-r--r--   0 lion      (1000) lion      (1000)      191 2023-08-02 17:33:10.000000 tko-0.3.7/MANIFEST.in
+-rw-r--r--   0 lion      (1000) lion      (1000)     6765 2024-04-05 15:55:27.236359 tko-0.3.7/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)     5911 2024-04-02 11:33:20.000000 tko-0.3.7/Readme.md
+-rw-r--r--   0 lion      (1000) lion      (1000)     3107 2024-04-05 15:53:53.000000 tko-0.3.7/changelog.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      298 2023-08-02 17:36:39.000000 tko-0.3.7/requirements.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-05 15:55:27.239693 tko-0.3.7/setup.cfg
+-rw-r--r--   0 lion      (1000) lion      (1000)     3969 2024-04-02 11:33:20.000000 tko-0.3.7/setup.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-05 15:55:27.213026 tko-0.3.7/src/
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-05 15:55:27.229693 tko-0.3.7/src/tko/
+-rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-05 15:13:21.000000 tko-0.3.7/src/tko/__init__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     9417 2024-04-05 15:52:20.000000 tko-0.3.7/src/tko/__main__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     8001 2024-04-05 15:51:48.000000 tko-0.3.7/src/tko/actions.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4516 2024-04-03 12:42:24.000000 tko-0.3.7/src/tko/basic.py
+-rw-r--r--   0 lion      (1000) lion      (1000)    10034 2023-10-19 13:10:37.000000 tko-0.3.7/src/tko/diff.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     7521 2024-03-21 14:49:39.000000 tko-0.3.7/src/tko/down.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4997 2024-04-03 01:50:45.000000 tko-0.3.7/src/tko/filter.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5747 2023-10-07 23:37:00.000000 tko-0.3.7/src/tko/format.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2727 2024-03-13 17:39:00.000000 tko-0.3.7/src/tko/guide.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     8104 2024-04-02 18:12:46.000000 tko-0.3.7/src/tko/loader.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2567 2023-08-03 03:39:13.000000 tko-0.3.7/src/tko/pattern.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1803 2023-10-19 18:36:35.000000 tko-0.3.7/src/tko/runner.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5609 2024-03-20 21:47:04.000000 tko-0.3.7/src/tko/settings.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4426 2024-03-22 11:32:02.000000 tko-0.3.7/src/tko/solver.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     7124 2024-04-02 11:33:20.000000 tko-0.3.7/src/tko/wdir.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3177 2024-04-02 11:33:20.000000 tko-0.3.7/src/tko/writer.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-05 15:55:27.236359 tko-0.3.7/src/tko.egg-info/
+-rw-r--r--   0 lion      (1000) lion      (1000)     6765 2024-04-05 15:55:27.000000 tko-0.3.7/src/tko.egg-info/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)      554 2024-04-05 15:55:27.000000 tko-0.3.7/src/tko.egg-info/SOURCES.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-05 15:55:27.000000 tko-0.3.7/src/tko.egg-info/dependency_links.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       47 2024-04-05 15:55:27.000000 tko-0.3.7/src/tko.egg-info/entry_points.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       59 2024-04-05 15:55:27.000000 tko-0.3.7/src/tko.egg-info/requires.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        4 2024-04-05 15:55:27.000000 tko-0.3.7/src/tko.egg-info/top_level.txt
```

### Comparing `tko-0.3.6/LICENSE` & `tko-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tko-0.3.6/PKG-INFO` & `tko-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tko
-Version: 0.3.6
+Version: 0.3.7
 Summary: tko: Test Kit Operations
 Home-page: https://github.com/senapk/tko
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/tko/issues
 Project-URL: Source, https://github.com/senapk/tko/
 Keywords: programming,learning
```

### Comparing `tko-0.3.6/Readme.md` & `tko-0.3.7/Readme.md`

 * *Files identical despite different names*

### Comparing `tko-0.3.6/changelog.md` & `tko-0.3.7/changelog.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+- 0.3.7
+  - fix: filter mode with empty files
+  - fix: action class to poo mode
+- 0.3.6
+  - add compact mode to run
 - 0.3.5:
   - update filter mode
 - 0.3.4:
   - cio mode update parser
 - 0.3.3:
   - improved filter mode for fun
   - fixed bud in grade reduction show for build a .tio file
```

### Comparing `tko-0.3.6/setup.py` & `tko-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.6/src/tko/__main__.py` & `tko-0.3.7/src/tko/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import argparse
 import sys
 
-from .actions import Actions
+from .actions import Run, Build
 from .basic import Param
 from .pattern import PatternLoader
 from .basic import DiffMode
 from .format import Report, Colored
 from .down import Down
 from .settings import SettingsParser
 from .guide import tko_guide
@@ -39,21 +39,23 @@
             updown = not SettingsParser().get_hdiff()
             size_too_short = Report.get_terminal_size() < SettingsParser().get_hdiffmin()
             param.set_up_down(updown or size_too_short)
         elif args.sideby:
             param.set_up_down(False)
         elif args.updown:
             param.set_up_down(True)
-        Actions.run(args.target_list, args.cmd, param)
+        run = Run(args.target_list, args.cmd, param)
+        run.execute()
 
     @staticmethod
     def build(args):
         PatternLoader.pattern = args.pattern
         manip = Param.Manip().set_unlabel(args.unlabel).set_to_sort(args.sort).set_to_number(args.number)
-        Actions.build(args.target, args.target_list, manip, args.force)
+        build = Build(args.target, args.target_list, manip, args.force)
+        build.execute()
     
     @staticmethod
     def settings(args):
         sp = SettingsParser()
         
         if args.ascii:
             sp.set_ascii(True)
```

### Comparing `tko-0.3.6/src/tko/actions.py` & `tko-0.3.7/src/tko/actions.py`

 * *Files 17% similar despite different names*

```diff
@@ -47,20 +47,24 @@
             text_extensions = [".md", ".c", ".cpp", ".h", ".hpp", ".py", ".java", ".js", ".ts", ".hs"]
 
             if not any([filename.endswith(ext) for ext in text_extensions]):
                 return
             
             content = open(source, "r").read()
             processed = Filter(filename).process(content)
-            with open(destiny, "w") as f:
-                f.write(processed)
+            if processed != "":
+                with open(destiny, "w") as f:
+                    f.write(processed)
             
             line = "";
             if processed != content:
-                line += "(filtered): "
+                if processed == "":
+                    line += "(disabled): "
+                else:
+                    line += "(filtered): "
             else:
                 line += "(        ): "
             line += destiny
             print(line)
 
     @staticmethod
     def deep_copy_and_change_dir():
@@ -78,110 +82,146 @@
             print("fail: verify your permissions, or if there is a file with the same name.")
         
         FilterMode.deep_filter_copy(".", filter_path)
 
         os.chdir(filter_path)
 
 
-class Actions:
+class Run:
 
-    def __init__(self):
-        pass
+    def __init__(self, target_list: List[str], exec_cmd: Optional[str], param: Param.Basic):
+        self.target_list = target_list
+        self.exec_cmd = exec_cmd
+        self.param = param
+        self.wdir = None
 
-    @staticmethod
-    def run(target_list: List[str], exec_cmd: Optional[str], param: Param.Basic) -> int:
-        
+
+    def change_targets_to_filter_mode(self):
         # modo de filtragem, antes de processar os dados, copiar tudo para o diretório temp fixo
         # filtrar os solvers para então continuar com a execução
-        if param.filter:
+        if self.param.filter:
             old_dir = os.getcwd()
 
             print(Report.centralize(" Entering in filter mode ", "═"))
             FilterMode.deep_copy_and_change_dir()  
             # search for target outside . dir and redirect target
             new_target_list = []
-            for target in target_list:
+            for target in self.target_list:
                 if ".." in target:
                     new_target_list.append(os.path.normpath(os.path.join(old_dir, target)))
-                else:
+                elif os.path.exists(target):
                     new_target_list.append(target)
-            target_list = new_target_list
-
-        try:
-            wdir = Wdir().set_target_list(target_list).set_cmd(exec_cmd).build().filter(param)
-        except CompilerError as e:
-            print(e)
-            return 0
-        except FileNotFoundError as e:
-            print(e)
-            return 0
+            self.target_list = new_target_list
 
-        if wdir.solver is None and len(wdir.unit_list) == 0:
-            print(Colored.paint("fail: ", Color.RED) + "No solver or tests found.")
-            return 0
-
-        if wdir.solver is None and len(wdir.unit_list) > 0:
-            print(Report.centralize(" No solvers found. Listing Test Cases ", "╌"), flush=True)
-            print(wdir.resume())
-            print(wdir.unit_list_resume())
-            return
-
-        if wdir.solver is not None and len(wdir.unit_list) == 0:
-            print(Report.centralize(" No test cases found. Running: " + wdir.solver.executable + " ", symbols.hbar), flush=True)
-            # force print to terminal
-
-            Runner.free_run(wdir.solver.executable)
-            return
-        
-        print(Report.centralize(" Running solver against test cases ", "═"))
-
-        ## print top line
-        print(wdir.resume(), end="")
+    def print_top_line(self):
+        print(self.wdir.resume(), end="")
         print(" [", end="", flush=True)
         first = True
-        for unit in wdir.unit_list:
+        for unit in self.wdir.unit_list:
             if first:
                 first = False
             else:
                 print(" ", end="", flush=True)
-            unit.result = Execution.run_unit(wdir.solver, unit)
+            unit.result = Execution.run_unit(self.wdir.solver, unit)
             print(ExecutionResult.get_symbol(unit.result), end="", flush=True)
         print("]")
 
-        if param.diff_mode == DiffMode.QUIET:
+    def print_diff(self):
+        if self.param.diff_mode == DiffMode.QUIET:
             return
         
-        results = [unit.result for unit in wdir.unit_list]
+        results = [unit.result for unit in self.wdir.unit_list]
         if not ExecutionResult.EXECUTION_ERROR in results and not ExecutionResult.WRONG_OUTPUT in results:
             return
         
-        if not param.compact:
-            print(wdir.unit_list_resume())
+        if not self.param.compact:
+            print(self.wdir.unit_list_resume())
         
-        if param.diff_mode == DiffMode.FIRST:
+        if self.param.diff_mode == DiffMode.FIRST:
         # printing only the first wrong case
-            wrong = [unit for unit in wdir.unit_list if unit.result != ExecutionResult.SUCCESS][0]
-            if param.is_up_down:
+            wrong = [unit for unit in self.wdir.unit_list if unit.result != ExecutionResult.SUCCESS][0]
+            if self.param.is_up_down:
                 print(Diff.mount_up_down_diff(wrong))
             else:
                 print(Diff.mount_side_by_side_diff(wrong))
             return
 
-        if param.diff_mode == DiffMode.ALL:
-            for unit in wdir.unit_list:
+        if self.param.diff_mode == DiffMode.ALL:
+            for unit in self.wdir.unit_list:
                 if unit.result != ExecutionResult.SUCCESS:
-                    if param.is_up_down:
+                    if self.param.is_up_down:
                         print(Diff.mount_up_down_diff(unit))
                     else:
                         print(Diff.mount_side_by_side_diff(unit))
+
+    def build_wdir(self) -> bool:
+        try:
+            self.wdir = Wdir().set_target_list(self.target_list).set_cmd(self.exec_cmd).build().filter(self.param)
+        except CompilerError as e:
+            print(e)
+            return False
+        except FileNotFoundError as e:
+            print(e)
+            return False
+        return True
+
+    def missing_target(self) -> bool:
+        # no solver and no test cases
+        if self.wdir.solver is None and len(self.wdir.unit_list) == 0:
+            print(Colored.paint("fail: ", Color.RED) + "No solver or tests found.")
+            return True
+        return False
+    
+    def list_mode(self) -> bool:
+        # list mode
+        if self.wdir.solver is None and len(self.wdir.unit_list) > 0:
+            print(Report.centralize(" No solvers found. Listing Test Cases ", "╌"), flush=True)
+            print(self.wdir.resume())
+            print(self.wdir.unit_list_resume())
+            return True
+        return False
+
+    def free_run(self) -> bool:
+        # free run mode
+        if self.wdir.solver is not None and len(self.wdir.unit_list) == 0:
+            print(Report.centralize(" No test cases found. Running: " + self.wdir.solver.executable + " ", symbols.hbar), flush=True)
+            # force print to terminal
+            Runner.free_run(self.wdir.solver.executable)
+            return True
+        return False
+
+    def diff_mode(self) -> bool:
+        print(Report.centralize(" Running solver against test cases ", "═"))
+        self.print_top_line()
+        self.print_diff()
+
+    def execute(self):
+        self.change_targets_to_filter_mode()
+        if not self.build_wdir():
+            return
+        if self.missing_target():
+            return
+        if self.list_mode():
+            return
+        if self.free_run():
+            return
+        self.diff_mode()
         return
 
-    @staticmethod
-    def build(target_out: str, source_list: List[str], param: Param.Manip, to_force: bool) -> bool:
+class Build:
+
+    def __init__(self, target_out: str, source_list: List[str], param: Param.Manip, to_force: bool):
+        self.target_out = target_out
+        self.source_list = source_list
+        self.param = param
+        self.to_force = to_force
+
+    def execute(self):
         try:
-            wdir = Wdir().set_sources(source_list).build()
-            wdir.manipulate(param)
-            Writer.save_target(target_out, wdir.unit_list, to_force)
+            wdir = Wdir().set_sources(self.source_list).build()
+            wdir.manipulate(self.param)
+            Writer.save_target(self.target_out, wdir.unit_list, self.to_force)
         except FileNotFoundError as e:
             print(str(e))
             return False
         return True
+
```

### Comparing `tko-0.3.6/src/tko/basic.py` & `tko-0.3.7/src/tko/basic.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.6/src/tko/diff.py` & `tko-0.3.7/src/tko/diff.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.6/src/tko/down.py` & `tko-0.3.7/src/tko/down.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.6/src/tko/filter.py` & `tko-0.3.7/src/tko/filter.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.6/src/tko/format.py` & `tko-0.3.7/src/tko/format.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.6/src/tko/guide.py` & `tko-0.3.7/src/tko/guide.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.6/src/tko/loader.py` & `tko-0.3.7/src/tko/loader.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.6/src/tko/pattern.py` & `tko-0.3.7/src/tko/pattern.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.6/src/tko/runner.py` & `tko-0.3.7/src/tko/runner.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.6/src/tko/settings.py` & `tko-0.3.7/src/tko/settings.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.6/src/tko/solver.py` & `tko-0.3.7/src/tko/solver.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.6/src/tko/wdir.py` & `tko-0.3.7/src/tko/wdir.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.6/src/tko/writer.py` & `tko-0.3.7/src/tko/writer.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.6/src/tko.egg-info/PKG-INFO` & `tko-0.3.7/src/tko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tko
-Version: 0.3.6
+Version: 0.3.7
 Summary: tko: Test Kit Operations
 Home-page: https://github.com/senapk/tko
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/tko/issues
 Project-URL: Source, https://github.com/senapk/tko/
 Keywords: programming,learning
```

### Comparing `tko-0.3.6/src/tko.egg-info/SOURCES.txt` & `tko-0.3.7/src/tko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

