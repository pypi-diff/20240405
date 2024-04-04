# Comparing `tmp/feno-0.0.9.tar.gz` & `tmp/feno-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feno-0.0.9.tar", last modified: Wed Apr  3 18:17:38 2024, max compression
+gzip compressed data, was "feno-0.1.1.tar", last modified: Thu Apr  4 23:45:13 2024, max compression
```

## Comparing `feno-0.0.9.tar` & `feno-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 18:17:38.693213 feno-0.0.9/
--rw-r--r--   0 lion      (1000) lion      (1000)     1043 2024-03-26 18:23:42.000000 feno-0.0.9/LICENSE
--rw-r--r--   0 lion      (1000) lion      (1000)      191 2024-03-26 18:23:42.000000 feno-0.0.9/MANIFEST.in
--rw-r--r--   0 lion      (1000) lion      (1000)      918 2024-04-03 18:17:38.693213 feno-0.0.9/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)       46 2024-03-27 17:52:43.000000 feno-0.0.9/README.md
--rw-r--r--   0 lion      (1000) lion      (1000)      469 2024-04-03 18:17:27.000000 feno-0.0.9/changelog.md
--rw-r--r--   0 lion      (1000) lion      (1000)      310 2024-03-27 17:54:40.000000 feno-0.0.9/requirements.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-03 18:17:38.693213 feno-0.0.9/setup.cfg
--rw-r--r--   0 lion      (1000) lion      (1000)     3107 2024-04-01 17:24:14.000000 feno-0.0.9/setup.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 18:17:38.666546 feno-0.0.9/src/
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 18:17:38.689880 feno-0.0.9/src/feno/
--rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-03 18:12:54.000000 feno-0.0.9/src/feno/__init__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1861 2024-04-02 01:57:25.000000 feno-0.0.9/src/feno/__main__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5130 2024-04-02 12:05:39.000000 feno-0.0.9/src/feno/actions.py
--rw-r--r--   0 lion      (1000) lion      (1000)      550 2024-03-26 19:17:45.000000 feno-0.0.9/src/feno/cases.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1699 2024-04-01 17:39:49.000000 feno-0.0.9/src/feno/check.py
--rw-r--r--   0 lion      (1000) lion      (1000)      938 2024-03-26 19:19:40.000000 feno-0.0.9/src/feno/css_style.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5382 2024-04-03 18:14:31.000000 feno-0.0.9/src/feno/filter.py
--rw-r--r--   0 lion      (1000) lion      (1000)     6915 2024-04-02 01:52:43.000000 feno-0.0.9/src/feno/html.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2494 2024-03-27 13:44:12.000000 feno-0.0.9/src/feno/indexer.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3326 2024-03-27 13:09:44.000000 feno-0.0.9/src/feno/jsontools.py
--rw-r--r--   0 lion      (1000) lion      (1000)      393 2024-04-01 23:10:29.000000 feno-0.0.9/src/feno/log.py
--rw-r--r--   0 lion      (1000) lion      (1000)    11193 2024-04-03 15:47:37.000000 feno-0.0.9/src/feno/mdpp.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4989 2024-04-01 23:31:38.000000 feno-0.0.9/src/feno/remote_md.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1846 2024-04-03 01:37:08.000000 feno-0.0.9/src/feno/tree.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 18:17:38.689880 feno-0.0.9/src/feno.egg-info/
--rw-r--r--   0 lion      (1000) lion      (1000)      918 2024-04-03 18:17:38.000000 feno-0.0.9/src/feno.egg-info/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)      542 2024-04-03 18:17:38.000000 feno-0.0.9/src/feno.egg-info/SOURCES.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-03 18:17:38.000000 feno-0.0.9/src/feno.egg-info/dependency_links.txt
--rw-r--r--   0 lion      (1000) lion      (1000)      144 2024-04-03 18:17:38.000000 feno-0.0.9/src/feno.egg-info/entry_points.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       55 2024-04-03 18:17:38.000000 feno-0.0.9/src/feno.egg-info/requires.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        5 2024-04-03 18:17:38.000000 feno-0.0.9/src/feno.egg-info/top_level.txt
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-04 23:45:13.342985 feno-0.1.1/
+-rw-r--r--   0 lion      (1000) lion      (1000)     1043 2024-03-26 18:23:42.000000 feno-0.1.1/LICENSE
+-rw-r--r--   0 lion      (1000) lion      (1000)      191 2024-03-26 18:23:42.000000 feno-0.1.1/MANIFEST.in
+-rw-r--r--   0 lion      (1000) lion      (1000)      899 2024-04-04 23:45:13.342985 feno-0.1.1/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)       46 2024-03-27 17:52:43.000000 feno-0.1.1/README.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      558 2024-04-04 23:38:13.000000 feno-0.1.1/changelog.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      306 2024-04-04 23:06:44.000000 feno-0.1.1/requirements.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-04 23:45:13.342985 feno-0.1.1/setup.cfg
+-rw-r--r--   0 lion      (1000) lion      (1000)     3107 2024-04-01 17:24:14.000000 feno-0.1.1/setup.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-04 23:45:13.329652 feno-0.1.1/src/
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-04 23:45:13.339652 feno-0.1.1/src/feno/
+-rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-04 23:26:18.000000 feno-0.1.1/src/feno/__init__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1994 2024-04-04 23:24:21.000000 feno-0.1.1/src/feno/__main__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5184 2024-04-04 23:40:16.000000 feno-0.1.1/src/feno/actions.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      550 2024-03-26 19:17:45.000000 feno-0.1.1/src/feno/cases.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1699 2024-04-01 17:39:49.000000 feno-0.1.1/src/feno/check.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      938 2024-03-26 19:19:40.000000 feno-0.1.1/src/feno/css_style.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5382 2024-04-03 18:14:31.000000 feno-0.1.1/src/feno/filter.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     8485 2024-04-04 23:00:46.000000 feno-0.1.1/src/feno/html.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2494 2024-03-27 13:44:12.000000 feno-0.1.1/src/feno/indexer.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3435 2024-04-04 23:36:07.000000 feno-0.1.1/src/feno/jsontools.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      393 2024-04-01 23:10:29.000000 feno-0.1.1/src/feno/log.py
+-rw-r--r--   0 lion      (1000) lion      (1000)    11201 2024-04-04 23:37:02.000000 feno-0.1.1/src/feno/mdpp.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4976 2024-04-04 23:15:36.000000 feno-0.1.1/src/feno/remote_md.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1375 2024-04-04 23:31:11.000000 feno-0.1.1/src/feno/tree.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-04 23:45:13.342985 feno-0.1.1/src/feno.egg-info/
+-rw-r--r--   0 lion      (1000) lion      (1000)      899 2024-04-04 23:45:13.000000 feno-0.1.1/src/feno.egg-info/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)      542 2024-04-04 23:45:13.000000 feno-0.1.1/src/feno.egg-info/SOURCES.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-04 23:45:13.000000 feno-0.1.1/src/feno.egg-info/dependency_links.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)      144 2024-04-04 23:45:13.000000 feno-0.1.1/src/feno.egg-info/entry_points.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       51 2024-04-04 23:45:13.000000 feno-0.1.1/src/feno.egg-info/requires.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        5 2024-04-04 23:45:13.000000 feno-0.1.1/src/feno.egg-info/top_level.txt
```

### Comparing `feno-0.0.9/LICENSE` & `feno-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `feno-0.0.9/PKG-INFO` & `feno-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feno
-Version: 0.0.9
+Version: 0.1.1
 Summary: feno: Flexible Exercise Notation Organizer
 Home-page: https://github.com/senapk/feno
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/feno/issues
 Project-URL: Source, https://github.com/senapk/feno/
 Keywords: programming,learning
@@ -12,15 +12,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Education
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: tko
 Requires-Dist: build
 Requires-Dist: twine
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
```

### Comparing `feno-0.0.9/setup.py` & `feno-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.9/src/feno/__main__.py` & `feno-0.1.1/src/feno/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,56 +5,59 @@
 from .actions import Actions
 from .__init__ import __version__
 from .log import Log
 
 
 def main():
     parser = argparse.ArgumentParser()
-    parser.add_argument('targets', metavar='T', type=str, nargs='*', help='Readmes or folders')
+    parser.add_argument('targets', metavar='T', type=str, nargs='*', help='folders')
     parser.add_argument("--check", "-c", action="store_true", help="Check if the file needs to be rebuilt")
-    parser.add_argument("--preamble", "-p", action="store_true", help="disable qxcode preamble")
-    parser.add_argument("--version", action="store_true", help="Prints the version")
-    parser.add_argument("--verbose", "-v", action="store_true", help="Verbose mode")
-    parser.add_argument("--keep", "-k", action="store_true", help="Keep the cache files")
-    parser.add_argument("--remote", "-r", type=str, help="remote config file")
+    parser.add_argument("--version", "-v", action="store_true", help="Prints the version")
+
+    parser.add_argument("--brief", "-b", action="store_true", help="Brief mode")
+    parser.add_argument("--erase", "-e", action="store_true", help="Erase .html and .tio temp files")
+    parser.add_argument("--remote", "-r", action="store_true", help="Search for remote.cfg file and create absolute links")
+    parser.add_argument("--tko", "-t", action="store_true", help="Insert tko preamble")
     
+
     args = parser.parse_args()
-    Log.set_verbose(args.verbose)
+    Log.set_verbose(not args.brief)
     
     if args.version:
         print(__version__)
         sys.exit(0)
 
     if len(args.targets) == 0:
         print("fail: No targets specified")
         exit(1)
 
     for target in args.targets:
         hook = os.path.basename(os.path.abspath(target))
 
-        actions = Actions(target, args.remote)
+        actions = Actions(target, args.remote, args.tko)
         Log.resume(hook, end=": [ ")
-        Log.verbose(hook, end=": ")
+        Log.verbose(hook)
 
         if not actions.validate():
             continue
 
         actions.load_title()
         actions.create_cache()
         actions.update_markdown()
 
         if not args.check or actions.need_rebuild():
             actions.recreate_cache() # erase .cache
-            actions.remote_md(args.preamble)
+            actions.copy_drafts()
+            actions.update_markdown() # se os drafts tiverem mudado o markdown precisa ser atualizado
+            actions.remote_md()
             actions.html()
             actions.build_cases()
-            actions.copy_drafts()
             actions.run_local_sh()
             actions.init_vpl()
             actions.create_mapi()
-            actions.clean(args.keep)
+            actions.clean(args.erase)
 
         Log.resume("]")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `feno-0.0.9/src/feno/actions.py` & `feno-0.1.1/src/feno/actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 import os
 import shutil
 
 def norm_join(*args):
     return os.path.normpath(os.path.join(*args))
 
 class Actions:
-    def __init__(self, source_dir, remote_config: Optional[str]=None):
+    def __init__(self, source_dir, make_remote: bool, insert_tko_preamble: bool):
         self.cache = norm_join(source_dir, ".cache")
         self.target = norm_join(self.cache, "mapi.json")
         self.source_dir = source_dir
         self.hook = os.path.basename(os.path.abspath(source_dir))
         self.source_readme = norm_join(self.source_dir, "Readme.md")
         self.remote_readme = norm_join(self.cache, "Readme.md")
         self.target_html = norm_join(self.cache, "q.html")
         self.title = ""
         self.cases = norm_join(self.cache, "q.tio")
         self.config_json = norm_join(self.source_dir, "config.json")
         self.mapi_json = norm_join(self.cache, "mapi.json")
-        self.draft_tree = {}
         self.cache_src = norm_join(self.cache, "lang")
         self.vpl = None
-        self.remote_config: Optional[str] = remote_config
+        self.make_remote: bool = make_remote
+        self.insert_tko_preamble: bool = insert_tko_preamble
 
     def validate(self):
         if not os.path.isdir(self.source_dir):
             print(f"\n    fail: {self.source_dir} is not a directory")
             return False
         if not os.path.isfile(self.source_readme):
             print(f"\n    fail: {self.source_readme} not found")
@@ -60,28 +60,30 @@
             Log.resume("Changes ", end="")
             Log.verbose(f"changes in {self.source_dir}")
             return True
             
         Log.verbose("")
         return False
     
-    def remote_md(self, disable_preamble=False):
+    def remote_md(self):
         cfg = RemoteCfg()
-        if self.remote_config is not None:
-            cfg.read(self.remote_config)
-        else:
+        found = False
+        if self.make_remote:
             cfg_path = RemoteCfg.search_cfg_path(self.source_dir)
             if cfg_path is None:
                 print("\n    fail: no remote.cfg found in the parent folders")
                 print("\n    fail: proceeding without make absolute links")
             else:
+                found = True
                 Log.verbose(f"    remote.cfg: {cfg_path}")
                 cfg.read(cfg_path)
-        RemoteMd.run(cfg, self.source_readme, self.remote_readme, self.hook, disable_preamble)
-        Log.resume("AbsoluteMd ", end="")
+        RemoteMd.run(cfg, self.source_readme, self.remote_readme, self.hook, self.insert_tko_preamble)
+        if self.make_remote and found:
+            Log.resume("AbsoluteMd ", end="")
+        Log.verbose(f"    RemoteFile: {self.remote_readme}")
     
     # uses pandoc to generate html from markdown
     def html(self):
         title = Title.extract_title(self.source_readme)
         HTML.generate_html_with_pandoc(title, self.remote_readme, self.target_html, True)
         Log.resume("HTML ", end="")
         Log.verbose(f"    HTML  file: {self.target_html}")
@@ -93,15 +95,15 @@
         Log.verbose(f"    Cases file: {self.cases}")
 
     def copy_drafts(self):
         source_src = norm_join(self.source_dir, "src")
         if os.path.isdir(source_src):
             Log.resume("Drafts ", end="")
             Log.verbose(f"    Drafts dir: {source_src}")
-            Tree.deep_filter_copy(source_src, self.cache_src, self.draft_tree, 5)
+            Tree.deep_filter_copy(source_src, self.cache_src, 5)
 
     def run_local_sh(self):
         local_sh = norm_join(self.source_dir, "local.sh")
         actual_chdir = os.getcwd()
         if os.path.isfile(local_sh):
             os.chdir(self.source_dir)
             subprocess.run("bash local.sh", shell=True)
@@ -110,25 +112,25 @@
             Log.verbose(f"    local.sh executed")
 
     def init_vpl(self):
         self.vpl = JsonVPL(self.title, open(self.target_html).read())
         self.vpl.set_cases(self.cases)
         if self.vpl.load_config_json(self.config_json, self.source_dir):
             Log.resume("Required ", end="")
-            Log.verbose(f"    Config mapi file: {self.config_json}")
-        if self.vpl.load_draft_tree(self.draft_tree, self.cache_src):
+            Log.verbose(f"    CfgVplJson: {self.config_json}")
+        if self.vpl.load_drafts(self.cache_src):
             Log.resume("Drafts ", end="")
 
     def create_mapi(self):
         open(self.mapi_json, "w").write(str(self.vpl) + "\n")
         Log.resume("Mapi ", end="")
         Log.verbose(f"    Mapi  file: {self.mapi_json}")
 
-    def clean(self, keep: bool):
-        if not keep:
+    def clean(self, erase: bool):
+        if erase:
             Log.resume("Cleaning ", end="")
             Log.verbose("    Cleaning  : html and cases files")
             os.remove(self.cases)
             os.remove(self.target_html)
 
     # run mdpp script on source readme
     def update_markdown(self):
```

### Comparing `feno-0.0.9/src/feno/cases.py` & `feno-0.1.1/src/feno/cases.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.9/src/feno/check.py` & `feno-0.1.1/src/feno/check.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.9/src/feno/css_style.py` & `feno-0.1.1/src/feno/css_style.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.9/src/feno/filter.py` & `feno-0.1.1/src/feno/filter.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.9/src/feno/html.py` & `feno-0.1.1/src/feno/html.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import subprocess
 from subprocess import PIPE
-
+# import markdown
 from .css_style import CssStyle
 
 class HTML:
 
     @staticmethod
     def generate_html_with_pandoc(title: str, input_file: str, output_file: str, enable_latex: bool):
         fulltitle = title.replace('!', '\\!').replace('?', '\\?')
@@ -100,31 +100,63 @@
 # .codehilite .vi { color: #19177C } /* Name.Variable.Instance */
 # .codehilite .vm { color: #19177C } /* Name.Variable.Magic */
 # .codehilite .il { color: #666666 } /* Literal.Number.Integer.Long */
 
 # </style>
 # """
 
+#     @staticmethod
+#     def fix_markdown_indentation(content):
+#         last: int = -1
+#         dist: int = -1
+#         step: int = 0
+#         inside_fences = False
+#         output = []
+#         for line in content.split("\n"):
+#             line_init = line.lstrip()
+#             line_dist = len(line) - len(line_init)
+#             if not inside_fences and (line_init.startswith("- ") or line_init.startswith("* ")):
+#                 if line_dist == 0: # primeiro
+#                     last = 0
+#                     dist = 0
+#                 elif line_dist > dist:
+#                     if last == 0: # segundo level
+#                         step = line_dist
+#                     last += 1 # proximo level
+#                     dist = line_dist
+#                 elif line_dist < dist:
+#                     last -= int((dist - line_dist) / step)
+#                     dist = line_dist
+#                 line = " " * (4 * last) + line_init
+#             if line.startswith("```"):
+#                 inside_fences = not inside_fences
+#             output.append(line)
+#         return "\n".join(output)
+
+#     @staticmethod
+#     def generate_html_with_python(title: str, input_file: str, output_file: str):
+#         with open(input_file) as f:
+#             content = f.read()
+#         lines = content.split("\n")
+#         output = []
+#         itemize = False
+#         for line in lines:
+#             if line.startswith("  - "):
+#                 output.append("  " + line)
+#             elif line.startswith("    - "):
+#                 output.append("    " + line)
+#             elif line.startswith("      - "):
+#                 output.append("      " + line)
+#             else:
+#                 output.append(line)
+#         content = "\n".join(output)
+#         data = markdown.markdown(content,
+#                                   extensions=['markdown_katex', 'md_in_html', 'fenced_code', 'codehilite', 'extra', 'nl2br', 'sane_lists', 'wikilinks', 'toc'],
+#                                     extension_configs={
+#                                         'markdown_katex': {
+#                                             'no_inline_svg': True,  # fix for WeasyPrint
+#                                             'insert_fonts_css': True,
+#                                         },
+#                                     })
 
-
-
-
-    # @staticmethod
-    # def generate_html_with_python(title: str, input_file: str, output_file: str):
-    #     with open(input_file) as f:
-    #         content = f.read()
-    #     lines = content.split("\n")
-    #     output = []
-    #     itemize = False
-    #     for line in lines:
-    #         if line.startswith("  - "):
-    #             output.append("  " + line)
-    #         elif line.startswith("    - "):
-    #             output.append("    " + line)
-    #         elif line.startswith("      - "):
-    #             output.append("      " + line)
-    #         else:
-    #             output.append(line)
-    #     content = "\n".join(output)
-    #     data = markdown.markdown(content, extensions=['fenced_code', 'codehilite', 'extra', 'nl2br', 'sane_lists', 'wikilinks', 'toc'])
-    #     with open(output_file, "w") as f:
-    #         f.write(data + HTML.codehilite_css)
+#         with open(output_file, "w") as f:
+#             f.write(data + HTML.codehilite_css)
```

### Comparing `feno-0.0.9/src/feno/indexer.py` & `feno-0.1.1/src/feno/indexer.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.9/src/feno/jsontools.py` & `feno-0.1.1/src/feno/jsontools.py`

 * *Files 8% similar despite different names*

```diff
@@ -81,21 +81,23 @@
                         self.add_keep(norm_join(source, file))
                 if "required" in cfg:
                     for file in cfg["required"]:
                         self.add_required(norm_join(source, file))
             return True
         return False
     
-    def load_draft_tree(self, draft_tree: Dict[str, List[str]], cache_draft: str):
-        if len(draft_tree) == 0:
-            return False
-        
-        for ext in draft_tree:
-            for file in draft_tree[ext]:
-                self.add_draft(ext, norm_join(cache_draft, ext, file))
-        return True
+    def load_drafts(self, cache_draft: str):
+        found = False
+        for lang in os.listdir(cache_draft):
+            lang_path = norm_join(cache_draft, lang)
+            if os.path.isdir(lang_path):
+                for file in os.listdir(lang_path):
+                    file_path = norm_join(lang_path, file)
+                    self.add_draft(lang, file_path)
+                    found = True
+        return found
 
     def __str__(self):
         return self.to_json()
```

### Comparing `feno-0.0.9/src/feno/mdpp.py` & `feno-0.1.1/src/feno/mdpp.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         return re.sub(regex, subst, content, 0, re.MULTILINE | re.DOTALL)
 
 class Drafts:
 
     @staticmethod
     def load_drafts(readme_path):
         folder = os.path.dirname(readme_path)
-        origin = os.path.join(folder, "src")
+        origin = os.path.join(folder, ".cache/lang")
         output = ""
         if os.path.isdir(origin):
             # create a markdown list os links with all files under .cache/src
             entries = sorted(os.listdir(origin))
             for lang in entries:
                 output += "- " + lang + "\n"
                 for file in sorted(os.listdir(os.path.join(origin, lang))):
```

### Comparing `feno-0.0.9/src/feno/remote_md.py` & `feno-0.1.1/src/feno/remote_md.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 
         config = configparser.ConfigParser()
         config.read(cfg_path)
 
         self.user = config["DEFAULT"]["user"]
         self.repo = config["DEFAULT"]["rep"]
         self.base = config["DEFAULT"]["base"]
-        if "branch" in config["DEFAULT"]:
-            self.branch = config["DEFAULT"]["branch"]
+        self.branch = config["DEFAULT"]["branch"]
+        self.tag = config["DEFAULT"]["tag"]
 
     @staticmethod
     def search_cfg_path(source_dir) -> Optional[str]:
         # look for the remote.cfg file in the current folder
         # if not found, look for it in the parent folder
         # if not found, look for it in the parent's parent folder ...
 
@@ -111,23 +111,23 @@
 
     @staticmethod
     def insert_qxcode_preamble(cfg: RemoteCfg, content: str, hook) -> str:
         base_hook = os.path.join(cfg.base, hook)
 
         lines = content.split("\n")
         online_readme_link = os.path.join("https://github.com", cfg.user, cfg.repo, "blob", cfg.branch, base_hook, "Readme.md")
-        tkodown = "tko down " + cfg.user[6:] + " " + hook
+        tkodown = "tko down " + cfg.tag + " " + hook
         lines = RemoteMd.insert_preamble(lines, online_readme_link, tkodown)
         return "\n".join(lines)
 
     @staticmethod
-    def run(remote_cfg: RemoteCfg, source: str, target: str, hook, disable_preamble: bool) -> bool:    
+    def run(remote_cfg: RemoteCfg, source: str, target: str, hook, insert_preamble: bool) -> bool:    
         content = open(source).read()
         if remote_cfg is not None:
-            if not disable_preamble:
+            if insert_preamble:
                 content = RemoteMd.insert_qxcode_preamble(remote_cfg, content, hook)
             content = Absolute.relative_to_absolute(content, remote_cfg, hook)
         open(target, "w").write(content)
 
 if __name__ == "__main__":
     remote_cfg = RemoteCfg()
     remote_cfg.read(RemoteCfg.get_default_cfg_path())
```

### Comparing `feno-0.0.9/src/feno/tree.py` & `feno-0.1.1/src/feno/tree.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,35 @@
 import os
 
 from .log import Log
 from .filter import Filter
 
 class Tree:
-
-    @staticmethod
-    def add_file_to_tree(source, dict_tree):
-        pieces = source.split(os.sep)
-        if len(pieces) >= 3:
-            if pieces[-3] == "src":
-                if pieces[-2] not in dict_tree: # new language
-                    dict_tree[pieces[-2]] = []
-                dict_tree[pieces[-2]].append(pieces[-1])
-
     @staticmethod
-    def deep_filter_copy(source, destiny, dict_tree, deep: int):
+    def deep_filter_copy(source, destiny, deep: int):
         if deep == 0:
             return
         if os.path.isdir(source):
             chain = source.split(os.sep)
             if len(chain) > 1 and chain[-1].startswith("."):
                 return
             if not os.path.isdir(destiny):
                 os.makedirs(destiny)
             for file in sorted(os.listdir(source)):
-                Tree.deep_filter_copy(os.path.join(source, file), os.path.join(destiny, file), dict_tree, deep - 1)
+                Tree.deep_filter_copy(os.path.join(source, file), os.path.join(destiny, file), deep - 1)
         else:
             filename = os.path.basename(source)
             text_extensions = [".md", ".c", ".cpp", ".h", ".hpp", ".py", ".java", ".js", ".ts", ".hs", ".txt"]
             if not any([filename.endswith(ext) for ext in text_extensions]):
                 return
             content = open(source, "r").read()
             processed = Filter(filename).process(content)
             if processed == content:
                 Log.verbose("         =====: ", end="")
                 open(destiny, "w").write(processed)
-                Tree.add_file_to_tree(source, dict_tree)
             elif processed == "" or processed == "\n":
                 Log.verbose("         empty: ", end="")
             else:
                 Log.verbose("         draft: ", end="")
                 open(destiny, "w").write(processed)
-                Tree.add_file_to_tree(source, dict_tree)
             Log.verbose(destiny)
```

### Comparing `feno-0.0.9/src/feno.egg-info/PKG-INFO` & `feno-0.1.1/src/feno.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feno
-Version: 0.0.9
+Version: 0.1.1
 Summary: feno: Flexible Exercise Notation Organizer
 Home-page: https://github.com/senapk/feno
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/feno/issues
 Project-URL: Source, https://github.com/senapk/feno/
 Keywords: programming,learning
@@ -12,15 +12,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Education
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: tko
 Requires-Dist: build
 Requires-Dist: twine
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
```

### Comparing `feno-0.0.9/src/feno.egg-info/SOURCES.txt` & `feno-0.1.1/src/feno.egg-info/SOURCES.txt`

 * *Files identical despite different names*

