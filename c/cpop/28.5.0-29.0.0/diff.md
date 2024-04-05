# Comparing `tmp/cpop-28.5.0.tar.gz` & `tmp/cpop-29.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpop-28.5.0.tar", last modified: Thu Apr  4 16:12:41 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `cpop-28.5.0.tar` & `cpop-29.0.0.tar`

### file list

```diff
@@ -1,40 +1,21 @@
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-04 16:12:41.315384 cpop-28.5.0/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    11348 2024-03-24 19:08:30.000000 cpop-28.5.0/LICENSE
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      116 2024-04-04 16:09:52.000000 cpop-28.5.0/MANIFEST.in
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4996 2024-04-04 16:12:41.315384 cpop-28.5.0/PKG-INFO
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4411 2024-04-01 23:16:48.000000 cpop-28.5.0/README.rst
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-04 16:12:41.311384 cpop-28.5.0/cpop.egg-info/
--rw-r--r--   0 akmod     (1000) akmod     (1000)     4996 2024-04-04 16:12:41.000000 cpop-28.5.0/cpop.egg-info/PKG-INFO
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      559 2024-04-04 16:12:41.000000 cpop-28.5.0/cpop.egg-info/SOURCES.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)        1 2024-04-04 16:12:41.000000 cpop-28.5.0/cpop.egg-info/dependency_links.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)       42 2024-04-04 16:12:41.000000 cpop-28.5.0/cpop.egg-info/entry_points.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      128 2024-04-04 16:12:41.000000 cpop-28.5.0/cpop.egg-info/requires.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)        8 2024-04-04 16:12:41.000000 cpop-28.5.0/cpop.egg-info/top_level.txt
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-04 16:12:41.311384 cpop-28.5.0/hub/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:07:30.000000 cpop-28.5.0/hub/__init__.py
--rwxrwxr-x   0 akmod     (1000) akmod     (1000)     4277 2024-04-03 15:09:20.000000 cpop-28.5.0/hub/__main__.py
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-04 16:12:41.315384 cpop-28.5.0/pop/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     2465 2024-04-03 15:48:23.000000 cpop-28.5.0/pop/config.yaml
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4417 2024-04-02 15:16:07.000000 cpop-28.5.0/pop/dirs.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1573 2024-03-24 19:08:30.000000 cpop-28.5.0/pop/exc.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    23470 2024-04-02 21:09:20.000000 cpop-28.5.0/pop/hub.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    11471 2024-04-03 16:53:30.000000 cpop-28.5.0/pop/loader.py
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-04 16:12:41.315384 cpop-28.5.0/pop/log/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     5219 2024-04-02 15:16:07.000000 cpop-28.5.0/pop/log/async.py
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-04 16:12:41.311384 cpop-28.5.0/pop/mods/
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-04 16:12:41.315384 cpop-28.5.0/pop/mods/pop/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     7501 2024-04-03 15:16:56.000000 cpop-28.5.0/pop/mods/pop/config.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      570 2024-04-01 16:10:17.000000 cpop-28.5.0/pop/mods/pop/contract.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      234 2024-04-01 16:10:17.000000 cpop-28.5.0/pop/mods/pop/dyne.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     6993 2024-04-01 22:18:05.000000 cpop-28.5.0/pop/mods/pop/sub.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      861 2024-04-01 19:09:27.000000 cpop-28.5.0/pop/mods/pop/test.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)   955794 2024-04-04 16:12:20.000000 cpop-28.5.0/pop/pop.contract.c
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     8478 2024-04-04 16:10:05.000000 cpop-28.5.0/pop/pop.contract.pyx
--rw-rw-r--   0 akmod     (1000) akmod     (1000)   878107 2024-04-04 16:12:20.000000 cpop-28.5.0/pop/pop.data.c
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     6101 2024-04-04 16:10:05.000000 cpop-28.5.0/pop/pop.data.pyx
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      555 2024-04-01 17:31:50.000000 cpop-28.5.0/pop/ref.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1176 2024-04-04 16:09:52.000000 cpop-28.5.0/pop/scanner.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     7642 2024-03-24 19:08:30.000000 cpop-28.5.0/pop/verify.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1361 2024-04-04 16:11:59.000000 cpop-28.5.0/pyproject.toml
--rw-rw-r--   0 akmod     (1000) akmod     (1000)       38 2024-04-04 16:12:41.315384 cpop-28.5.0/setup.cfg
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      315 2024-04-04 16:09:52.000000 cpop-28.5.0/setup.py
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 cpop-29.0.0/cpop/contract.pyx
+-rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 cpop-29.0.0/cpop/data.pyx
+-rwxr-xr-x   0        0        0     4280 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/__main__.py
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/config.yaml
+-rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/dirs.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/exc.py
+-rw-r--r--   0        0        0    23473 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/hub.py
+-rw-r--r--   0        0        0    11479 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/loader.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/ref.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/scanner.py
+-rw-r--r--   0        0        0     7642 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/verify.py
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/log/async.py
+-rw-r--r--   0        0        0     7505 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/mods/config.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/mods/contract.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/mods/dyne.py
+-rw-r--r--   0        0        0     6993 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/mods/sub.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/mods/test.py
+-rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 cpop-29.0.0/.gitignore
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 cpop-29.0.0/README.rst
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 cpop-29.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5532 2020-02-02 00:00:00.000000 cpop-29.0.0/PKG-INFO
```

### Comparing `cpop-28.5.0/PKG-INFO` & `cpop-29.0.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: cpop
-Version: 28.5.0
-Summary: The Cython-Optimized Plugin Oriented Programming System
-Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch@saltstack.com>
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.10
-Description-Content-Type: text/x-rst
-Provides-Extra: test
-Provides-Extra: build
-License-File: LICENSE
-
 ====
 cPOP
 ====
 
 cPop is used to express the Plugin Oriented Programming Paradigm. The Plugin
 Oriented Programming Paradigm has been designed to make pluggable software
 easy to write and easy to extend.
@@ -144,15 +128,15 @@
 .. code-block:: yaml
 
     # The default location is in ~/.pop/config.yaml
     # But you can change that by setting the POP_CONFIG environment variable
 
     pop_cli:
         # Setting this option will make your hub persist on the cli between calls
-        hub_state: ~/.pop/hub.msgpack
+        hub_state: ~/.pop/hub.pkl
     log:
         log_plugin: async
 
 From the above example, all arguments would be loaded onto the namespace under hub.OPT.my_namesapce.
 One config.yaml can add config options to multiple namespaces.
 They are all merged together in the order they are found in sys.path
 
@@ -175,14 +159,26 @@
 Run the tests in your cloned fork of cPop:
 
 .. code-block:: bash
 
     pytest tests
 
 
+Release
+=======
+
+.. code-block:: bash
+
+    pip install .\[build\]
+    hatch build
+    export HATCH_INDEX_USER="__token__"
+    export HATCH_INDEX_AUTH="pypi-api-token"
+    hatch publish
+
+
 Documentation
 =============
 
 Check out the docs for more information:
 
 https://pop.readthedocs.io
```

### Comparing `cpop-28.5.0/README.rst` & `cpop-29.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: cpop
+Version: 29.0.0
+Summary: The Cython-Optimized Plugin Oriented Programming System
+Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch@saltstack.com>
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
+Requires-Dist: aiofiles
+Requires-Dist: aiologger
+Requires-Dist: argparse
+Requires-Dist: pyyaml
+Provides-Extra: build
+Requires-Dist: cython; extra == 'build'
+Requires-Dist: hatch-cython; extra == 'build'
+Provides-Extra: test
+Requires-Dist: nest-asyncio; extra == 'test'
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-asyncio; extra == 'test'
+Description-Content-Type: text/x-rst
+
 ====
 cPOP
 ====
 
 cPop is used to express the Plugin Oriented Programming Paradigm. The Plugin
 Oriented Programming Paradigm has been designed to make pluggable software
 easy to write and easy to extend.
@@ -128,15 +153,15 @@
 .. code-block:: yaml
 
     # The default location is in ~/.pop/config.yaml
     # But you can change that by setting the POP_CONFIG environment variable
 
     pop_cli:
         # Setting this option will make your hub persist on the cli between calls
-        hub_state: ~/.pop/hub.msgpack
+        hub_state: ~/.pop/hub.pkl
     log:
         log_plugin: async
 
 From the above example, all arguments would be loaded onto the namespace under hub.OPT.my_namesapce.
 One config.yaml can add config options to multiple namespaces.
 They are all merged together in the order they are found in sys.path
 
@@ -159,14 +184,26 @@
 Run the tests in your cloned fork of cPop:
 
 .. code-block:: bash
 
     pytest tests
 
 
+Release
+=======
+
+.. code-block:: bash
+
+    pip install .\[build\]
+    hatch build
+    export HATCH_INDEX_USER="__token__"
+    export HATCH_INDEX_AUTH="pypi-api-token"
+    hatch publish
+
+
 Documentation
 =============
 
 Check out the docs for more information:
 
 https://pop.readthedocs.io
```

### Comparing `cpop-28.5.0/hub/__main__.py` & `cpop-29.0.0/pop/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import asyncio
 import pathlib
 import pickle
 from collections.abc import Callable
 from collections.abc import Iterable
 from pprint import pprint
 
-import pop.contract
-import pop.data
+import cpop.contract
+import cpop.data
 import pop.hub
 
 
 def save_hub_state(hub, state_file: pathlib.Path):
     # Manually retrieve the state using __getstate__
     state = hub.__getstate__()
     state_file.parent.mkdir(parents=True, exist_ok=True)
@@ -34,15 +34,15 @@
 def main():
     # Create the hub, loading all dynes and starting the loop
     hub = pop.hub.Hub(cli="pop_cli")
 
     original_opt = hub.OPT
     ref = original_opt.pop_cli.ref
 
-    safe_env = {"hub": pop.data.NamespaceDict(lib=hub.lib)}
+    safe_env = {"hub":cpop.data.NamespaceDict(lib=hub.lib)}
 
     # Try to get a saved hub
     if original_opt.pop_cli.hub_state:
         hub_state = original_opt.pop_cli.hub_state
         if hub_state.startswith('f"'):
             hub_state = eval(hub_state, safe_env)
 
@@ -106,15 +106,15 @@
                     raise
 
     # Call the named reference on the hub
     # This allows you to do
     # $ pop idem.init.cli
     # This way you can have multiple entrypoints, or even alias the above command to "idem"
     if asyncio.iscoroutinefunction(finder) or isinstance(
-        finder, (Callable, pop.contract.Contracted)
+        finder, (Callable, cpop.contract.Contracted)
     ):
         ret = finder(*args, **kwargs)
         while asyncio.iscoroutine(ret):
             ret = hub._synchronize(ret)
     else:
         ret = finder
```

### Comparing `cpop-28.5.0/pop/config.yaml` & `cpop-29.0.0/pop/config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     cli:
       help: The namespace to use as the authoritative CLI
     args:
       help: Any additional arguments to forward to the next cli
       positional: True
       nargs: "..."
     hub_state:
-      help: The location of a msgpack file that has a re-usable hub object
+      help: The location of a pickle file that has a re-usable hub object
   pop:
     config:
       help: The config file used for POP
       options:
         - -c
       subcommands:
         - __global__
@@ -98,12 +98,12 @@
   - asyncio
   - collections
   - importlib
   - importlib.resources
   - os
   - pathlib
   - pop.exc
-  - pop.contract
-  - pop.data
+  - cpop.contract
+  - cpop.data
   - pop.hub
   - sys
   - yaml
```

### Comparing `cpop-28.5.0/pop/dirs.py` & `cpop-29.0.0/pop/dirs.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import sys
 from collections import defaultdict
 from collections.abc import Iterable
 from typing import Any
 
 import yaml
 
-import pop.data
+import cpop.data
 
 
 def dir_list(pypath: list[str] = None, static: list[str] = None) -> list[pathlib.Path]:
     """
     Return the directories to look for modules in, pypath specifies files
     relative to an installed python package, static is for static dirs
     :param pypath: One or many python paths which will be imported
@@ -65,49 +65,49 @@
             if sub.endswith(".egg-link"):
                 with open(full) as rfh:
                     dirs.add(pathlib.Path(rfh.read().strip()))
             elif full.is_dir():
                 dirs.add(full)
 
     # Set up the _dynamic return
-    ret = pop.data.NamespaceDict(
-        dyne=pop.data.NamespaceDict(),
-        config=pop.data.NamespaceDict(),
-        imports=pop.data.NamespaceDict(),
+    ret =cpop.data.NamespaceDict(
+        dyne=cpop.data.NamespaceDict(),
+        config=cpop.data.NamespaceDict(),
+        imports=cpop.data.NamespaceDict(),
     )
 
     # Iterate over namespaces in sys.path
     for dir_ in dirs:
         config_file = dir_ / "config.yaml"
         try:
             if not config_file.is_file():
                 continue
         except:
             continue
         dynes, configs, imports = parse_config(config_file)
         if dynes:
-            pop.data.update(ret.dyne, dynes, merge_lists=True)
+           cpop.data.update(ret.dyne, dynes, merge_lists=True)
         if configs:
-            pop.data.update(ret.config, configs, merge_lists=True)
+           cpop.data.update(ret.config, configs, merge_lists=True)
         if imports:
-            pop.data.update(ret.imports, imports)
+           cpop.data.update(ret.imports, imports)
 
     return ret
 
 
 def parse_config(
     config_file: str,
 ) -> tuple[dict[str, object], dict[str, object], set[str]]:
-    dyne = defaultdict(lambda: pop.data.NamespaceDict(paths=set()))
-    config = pop.data.NamespaceDict(
-        config=pop.data.NamespaceDict(),
-        cli_config=pop.data.NamespaceDict(),
-        subcommands=pop.data.NamespaceDict(),
+    dyne = defaultdict(lambda:cpop.data.NamespaceDict(paths=set()))
+    config =cpop.data.NamespaceDict(
+        config=cpop.data.NamespaceDict(),
+        cli_config=cpop.data.NamespaceDict(),
+        subcommands=cpop.data.NamespaceDict(),
     )
-    imports = pop.data.NamespaceDict()
+    imports =cpop.data.NamespaceDict()
 
     config_file = pathlib.Path(config_file)
     if not config_file.is_file():
         return dyne, config, imports
     with open(config_file) as f:
         pop_config = yaml.safe_load(f) or {}
 
@@ -121,15 +121,15 @@
     for section in ["config", "cli_config", "subcommands"]:
         section_data = pop_config.get(section)
         if not isinstance(section_data, dict):
             continue
         for namespace, data in section_data.items():
             if data is None:
                 continue
-            config[section].setdefault(namespace, pop.data.NamespaceDict()).update(data)
+            config[section].setdefault(namespace,cpop.data.NamespaceDict()).update(data)
 
     # Handle python imports
     for imp in pop_config.get("import", []):
         base = imp.split(".", 1)[0]
         if base not in imports:
             imports[base] = importlib.import_module(base)
         if "." in imp:
```

### Comparing `cpop-28.5.0/pop/exc.py` & `cpop-29.0.0/pop/exc.py`

 * *Files identical despite different names*

### Comparing `cpop-28.5.0/pop/hub.py` & `cpop-29.0.0/pop/hub.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import secrets
 import sys
 from collections.abc import Coroutine
 from collections.abc import Iterable
 from types import ModuleType
 from typing import Any
 
-import pop.contract
-import pop.data
+import cpop.contract
+import cpop.data
 import pop.dirs
 import pop.exc
 import pop.loader
 import pop.ref
 import pop.scanner
 import pop.verify
 
@@ -26,15 +26,15 @@
         return path.split(",")
     elif isinstance(path, list):
         return path
     else:
         return []
 
 
-class PopMeta(pop.data.MultidictCache):
+class PopMeta(cpop.data.MultidictCache):
     def __init__(self, data: list[dict[str, any]]):
         attrs = {}
         data.append(attrs)
         super().__init__(data)
         object.__setattr__(self, "_attrs", attrs)
 
     def __setattr__(self, item: str, value):
@@ -72,15 +72,15 @@
     async def __self(self):
         return self
 
     def __call__(self, *args, **kwargs):
         if not self._target:
             return self.__self
 
-        if isinstance(self._target, pop.contract.Contracted):
+        if isinstance(self._target, cpop.contract.Contracted):
             coroutine = self._target(*args, **kwargs)
             return self._hub._synchronize(coroutine)
         else:
             raise TypeError(f"{self._target} is not a coroutine function")
 
 
 class Hub(PopMeta):
@@ -134,15 +134,15 @@
                 base: mod
                 for base, mod in sys.modules.items()
                 if not base.startswith("_") and "." not in base
             }
         )
 
         if pop_mods is None:
-            pop_mods = ["pop.mods.pop"]
+            pop_mods = ["pop.mods"]
 
         # Add the pop sub to the hub, this should always use pypath and
         # Should never be made dynamic. This is a core system sub and should
         # NOT be app-merged
         self._subs["pop"] = await AsyncSub(self, subname="pop", pypath=pop_mods)
         await self._subs["pop"]._load_all()
 
@@ -200,15 +200,15 @@
             elif isinstance(v, Iterable):
                 if all(isinstance(v2, pop.loader.BASE_TYPES) for v2 in v):
                     attrs[k] = v
         return dict(
             init_kwargs=self._init_kwargs,
             subs={name: sub.__getstate__() for name, sub in self._subs.items()},
             aliases=self._sub_alias,
-            OPT=pop.data.unfreeze(self._opt),
+            OPT=cpop.data.unfreeze(self._opt),
             imports={subname: mod.__name__ for subname, mod in self._imports.items()},
             attrs=attrs,
         )
 
     def __setstate__(self, state: dict):
         subs = state["subs"]
         opt = state["OPT"]
@@ -217,15 +217,15 @@
         for subname, modname in state["imports"].items():
             try:
                 self._imports[subname] = importlib.import_module(modname)
             except ModuleNotFoundError:
                 ...
         self._attrs.update(state["attrs"])
         self._sub_alias.update(aliases)
-        self._opt = pop.data.freeze(opt)
+        self._opt =cpop.data.freeze(opt)
         for name, data in subs.items():
             if name in self._subs:
                 sub = self._subs[name]
             else:
                 sub = Sub(hub=self, root=self, **data["init_kwargs"])
                 self._subs[name] = sub
 
@@ -605,22 +605,22 @@
 
         if self._process_vret(vret):
             return
 
         contracts = []
         for contract_sub in self._contract_subs:
             contracts.extend(
-                pop.contract.load_contract(
+                cpop.contract.load_contract(
                     contract_sub, self._default_contracts, mod, vret["name"]
                 )
             )
         recursive_contracts = []
         for recursive_contract_sub in self._recursive_contract_subs:
             recursive_contracts.extend(
-                pop.contract.load_contract(
+                cpop.contract.load_contract(
                     recursive_contract_sub,
                     self._default_recursive_contracts,
                     mod,
                     vret["name"],
                 )
             )
         name = vret["name"]
```

### Comparing `cpop-28.5.0/pop/loader.py` & `cpop-29.0.0/pop/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 import os
 import sys
 import types
 from collections.abc import Callable
 from typing import Any
 from typing import List
 
-import pop.contract
-import pop.data
+import cpop.contract
+import cpop.data
 import pop.exc
 
 BASE_TYPES = (int, float, str, bytes, bool, type(None))
 
 
 class LoadError(Exception):
     """
@@ -167,15 +167,15 @@
     """
     Process module's __init__ function if defined
     :param sub: The pop object that contains the loaded module data
     :param mod: A loader modul
     :param mod_name: The name of the module to get from the loader
     """
     if "__init__" in dir(mod):
-        init = pop.contract.Contracted(
+        init = cpop.contract.Contracted(
             sub._hub,
             contracts=[],
             func=mod.__init__,
             ref=f"{sub._subname}.{mod_name}",
             name="__init__",
         )
         await init()
@@ -194,16 +194,16 @@
             this_sub._alias = alias
 
 
 async def prep_loaded_mod(
     this_sub: "pop.hub.Sub",
     mod: "LoadedMod",
     mod_name: str,
-    contracts: "List[pop.contract.Wrapper]",
-    recursive_contracts: "List[pop.contract.Wrapper]",
+    contracts: "List[cpop.contract.Wrapper]",
+    recursive_contracts: "List[cpop.contract.Wrapper]",
 ) -> "LoadedMod":
     """
     Read the attributes of a python module and create a LoadedMod, which resolves
     aliases and omits objects that should not be exposed.
     :param this_sub: The pop object that contains the loaded module data
     :param mod: A loader module
     :param mod_name: The name of the module to get from the loader
@@ -249,15 +249,15 @@
         if attr.endswith(tuple(this_sub._omit_end)):
             continue
         if (
             inspect.isfunction(func)
             or inspect.isbuiltin(func)
             or type(func).__name__ == "cython_function_or_method"
         ):
-            obj = pop.contract.create_contracted(
+            obj = cpop.contract.create_contracted(
                 this_sub._hub,
                 ordered_contracts,
                 func,
                 ref,
                 name,
             )
             if not this_sub._omit_func:
@@ -273,18 +273,18 @@
                 # imported classes
                 if not klass.__module__.startswith(mod.__name__):
                     continue
                 lmod._classes[name] = klass
 
     # Add external aliased functions to the loaded mod
     for attr, func_alias in __func_alias__.items():
-        if isinstance(func_alias, pop.contract.Contracted):
+        if isinstance(func_alias, cpop.contract.Contracted):
             obj = func_alias
         elif isinstance(func_alias, Callable):
-            obj = pop.contract.create_contracted(
+            obj = cpop.contract.create_contracted(
                 this_sub._hub,
                 ordered_contracts,
                 func_alias,
                 ref,
                 attr,
                 implicit_hub=False,
             )
@@ -303,15 +303,15 @@
     """
 
     def __init__(self, name: str):
         super().__init__(name)
         vars = {}
         funcs = {}
         classes = {}
-        self._attrs = pop.data.MultidictCache([funcs, classes, vars])
+        self._attrs =cpop.data.MultidictCache([funcs, classes, vars])
         self._vars = vars
         self._funcs = funcs
         self._classes = classes
 
     def __getattr__(self, item: str):
         if item.startswith("_"):
             return self.__getattribute__(item)
```

### Comparing `cpop-28.5.0/pop/log/async.py` & `cpop-29.0.0/pop/log/async.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import inspect
 import sys
 
-import pop.contract
+import cpop.contract
 
 
 async def __init__(hub):
     hub.log.LOGGER = {}
     hub.log.FILE_HANDLER = None
     hub.log.STREAM_HANDLER = None
     hub.log.LEVEL = {
@@ -38,15 +38,15 @@
         for frame_info in inspect.stack(context=0)[relative_start:]:
             yield frame_info.frame
 
 
 def _get_hub_ref():
     # Minimize lookup time by starting at frame 5, it will be at least that far back
     for frame in _stack_frames(5):
-        if isinstance(frame.f_locals.get("self"), pop.contract.Contracted):
+        if isinstance(frame.f_locals.get("self"), cpop.contract.Contracted):
             contracted = frame.f_locals["self"]
             return contracted, frame.f_lineno
 
     # Default to the root reference
     return None, 0
```

### Comparing `cpop-28.5.0/pop/mods/pop/config.py` & `cpop-29.0.0/pop/mods/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pop.data
+import cpop.data
 
 
 async def load(
     hub: "pop.hub.Hub",
     cli: str = None,
     cli_config: dict[str, object] = None,
     config: dict[str, object] = None,
@@ -66,15 +66,15 @@
         cli=cli,
         cli_opts=cli_opts,
         config=config,
         config_file_data=config_data,
         global_clis=global_clis,
     )
 
-    return pop.data.freeze(OPT)
+    return cpop.data.freeze(OPT)
 
 
 async def parse_cli(
     hub,
     cli: str,
     active_cli: dict[str, object],
     subcommands: dict[str, object],
@@ -157,28 +157,28 @@
                         subparsers[subcommand].add_argument_group(group_name),
                     )
                     if group_name
                     else subparsers[subcommand]
                 )
                 subparser_group.add_argument(cli_name, *options, **opts)
 
-    return pop.data.NamespaceDict(parser.parse_args(args=parser_args).__dict__)
+    return cpop.data.NamespaceDict(parser.parse_args(args=parser_args).__dict__)
 
 
 PLACEHOLDER = object()
 
 
 async def prioritize(
     hub,
     cli: str,
     cli_opts: dict[str, any],
     config: dict[str, any],
     config_file_data: dict[str, any],
     global_clis: list[str],
-) -> pop.data.ImmutableNamespaceDict:
+) ->cpop.data.ImmutableNamespaceDict:
     """
     Prioritize configuration data from various sources.
 
     The order of priority is:
     1. CLI options (highest priority)
     2. Configuration file data
     3. OS environment variables
@@ -188,15 +188,15 @@
         hub: The POP hub instance.
         cli (str): The name of the CLI being prioritized.
         cli_opts (dict): The parsed CLI options.
         config (dict): The configuration dictionary.
         config_file_data (dict): The data from the configuration file.
 
     Returns:
-        pop.data.ImmutableNamespaceDict: The prioritized configuration options.
+       cpop.data.ImmutableNamespaceDict: The prioritized configuration options.
     """
     OPT = hub.lib.collections.defaultdict(dict)
     for namespace, args in config.items():
         for arg, data in args.items():
             # Initialize value to None
             value = None
 
@@ -220,8 +220,8 @@
             if value is PLACEHOLDER:
                 value = data.get("default")
 
             # Set the value in the OPT dictionary
             OPT[namespace][arg] = value
 
     OPT["SUBPARSER"] = cli_opts.get("SUBPARSER", "")
-    return pop.data.freeze(OPT)
+    return cpop.data.freeze(OPT)
```

### Comparing `cpop-28.5.0/pop/mods/pop/contract.py` & `cpop-29.0.0/pop/mods/contract.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections.abc import Callable
 
 import pop.exc
 
 
 async def process_pre_result(
-    hub, pre_ret, pre: Callable, cn: "pop.contract.Contracted"
+    hub, pre_ret, pre: Callable, cn: "cpop.contract.Contracted"
 ):
     if pre_ret is None:
         return
 
     if isinstance(pre_ret, bool):
         status = pre_ret
         msg = None
```

### Comparing `cpop-28.5.0/pop/mods/pop/sub.py` & `cpop-29.0.0/pop/mods/sub.py`

 * *Files identical despite different names*

### Comparing `cpop-28.5.0/pop/mods/pop/test.py` & `cpop-29.0.0/pop/mods/test.py`

 * *Files identical despite different names*

### Comparing `cpop-28.5.0/pop/pop.contract.pyx` & `cpop-29.0.0/cpop/contract.pyx`

 * *Files identical despite different names*

### Comparing `cpop-28.5.0/pop/pop.data.pyx` & `cpop-29.0.0/cpop/data.pyx`

 * *Files identical despite different names*

### Comparing `cpop-28.5.0/pop/ref.py` & `cpop-29.0.0/pop/ref.py`

 * *Files identical despite different names*

### Comparing `cpop-28.5.0/pop/scanner.py` & `cpop-29.0.0/pop/scanner.py`

 * *Files identical despite different names*

### Comparing `cpop-28.5.0/pop/verify.py` & `cpop-29.0.0/pop/verify.py`

 * *Files identical despite different names*

### Comparing `cpop-28.5.0/pyproject.toml` & `cpop-29.0.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,77 +1,88 @@
 [build-system]
-requires = ["setuptools >= 61.0", "wheel", "Cython"]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling", "hatch-cython"]
+build-backend = "hatchling.build"
 
 [project]
 name = "cpop"
-version = "28.5.0"
+version = "29.0.0"
 description = "The Cython-Optimized Plugin Oriented Programming System"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
     {name = "Thomas Hatch", email = "thatch@saltstack.com"},
 ]
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Development Status :: 5 - Production/Stable",
+    "License :: OSI Approved :: Apache Software License",
 ]
 requires-python = ">=3.10"
-
-
 dependencies = [
-  "aiofiles",
-  "aiologger",
-  "argparse",
-  "PyYaml",
+    "aiofiles",
+    "aiologger",
+    "argparse",
+    "PyYaml",
 ]
 
 [project.optional-dependencies]
 test = [
-  "nest-asyncio",
-  "pytest",
-  "pytest-asyncio",
+    "nest-asyncio",
+    "pytest",
+    "pytest-asyncio",
 ]
-
 build = [
-  "auditwheel",
-  "Cython",
-  "setuptools",
-  "wheel",
-  "twine",
+    "Cython",
+    "hatch-cython",
 ]
 
-[tool.setuptools]
-packages = ["hub", "pop"]
+[tool.hatch.build.targets.wheel]
+packages = [
+    "src/pop",
+    "src/cpop",
+]
 
+[tool.hatch.build.targets.sdist]
+packages = [
+    "src/pop",
+    "src/cpop",
+]
 
 [project.scripts]
-hub = "hub.__main__:main"
+hub = "pop.__main__:main"
+
+[tool.hatch.build.targets.wheel.hooks.cython.options]
+include_numpy = false
+include_pyarrow = false
+include_pythran = false
+
+directives = { boundscheck = false, nonecheck = false, language_level = 3, binding = true }
+
 
 [tool.black]
 line-length = 88
-target-version = ['py310']
+target-version = ['py310', 'py311', 'py312']
 include = '\.pyi?$'
 exclude = '''
 (
-  /(
-      \.eggs
+/(
+    \.eggs
     | \.git
     | \.hg
     | \.mypy_cache
     | \.tox
     | \.venv
     | _build
     | buck-out
     | build
     | dist
-  )/
+)/
 )
 '''
 
 [tool.pytest.ini_options]
 testpaths = "tests"
-addopts = "--tb native --full-trace --color=no -vv"
+addopts = "--tb native --full-trace --color=yes -vv"
 asyncio_mode = "auto"
```

