# Comparing `tmp/pyrob-0.6.1.tar.gz` & `tmp/pyrob-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrob-0.6.1.tar", last modified: Mon Mar 18 00:16:51 2024, max compression
+gzip compressed data, was "pyrob-0.8.1.tar", last modified: Fri Apr  5 14:45:24 2024, max compression
```

## Comparing `pyrob-0.6.1.tar` & `pyrob-0.8.1.tar`

### file list

```diff
@@ -1,32 +1,45 @@
-drwxr-xr-x   0 r0b       (1000) r0b       (1000)        0 2024-03-18 00:16:51.188200 pyrob-0.6.1/
--rw-r--r--   0 r0b       (1000) r0b       (1000)     1069 2024-03-13 20:05:30.000000 pyrob-0.6.1/LICENSE
--rw-r--r--   0 r0b       (1000) r0b       (1000)     3242 2024-03-18 00:16:51.188200 pyrob-0.6.1/PKG-INFO
--rw-r--r--   0 r0b       (1000) r0b       (1000)     1668 2024-03-17 21:44:43.000000 pyrob-0.6.1/README.md
--rw-r--r--   0 r0b       (1000) r0b       (1000)      622 2024-03-17 04:24:55.000000 pyrob-0.6.1/pyproject.toml
--rw-r--r--   0 r0b       (1000) r0b       (1000)       38 2024-03-18 00:16:51.188200 pyrob-0.6.1/setup.cfg
-drwxr-xr-x   0 r0b       (1000) r0b       (1000)        0 2024-03-18 00:16:51.188200 pyrob-0.6.1/src/
-drwxr-xr-x   0 r0b       (1000) r0b       (1000)        0 2024-03-18 00:16:51.188200 pyrob-0.6.1/src/pyrob/
--rw-r--r--   0 r0b       (1000) r0b       (1000)       60 2024-03-18 00:16:40.000000 pyrob-0.6.1/src/pyrob/__init__.py
--rw-r--r--   0 r0b       (1000) r0b       (1000)     1134 2024-03-17 03:40:41.000000 pyrob-0.6.1/src/pyrob/cli.py
-drwxr-xr-x   0 r0b       (1000) r0b       (1000)        0 2024-03-18 00:16:51.188200 pyrob-0.6.1/src/pyrob/commands/
--rw-r--r--   0 r0b       (1000) r0b       (1000)      130 2024-03-17 03:37:05.000000 pyrob-0.6.1/src/pyrob/commands/__init__.py
--rw-r--r--   0 r0b       (1000) r0b       (1000)     1462 2024-03-17 03:37:02.000000 pyrob-0.6.1/src/pyrob/commands/init.py
--rw-r--r--   0 r0b       (1000) r0b       (1000)     1998 2024-03-17 03:36:59.000000 pyrob-0.6.1/src/pyrob/commands/install.py
--rw-r--r--   0 r0b       (1000) r0b       (1000)      793 2024-03-17 03:36:57.000000 pyrob-0.6.1/src/pyrob/commands/run.py
--rw-r--r--   0 r0b       (1000) r0b       (1000)      794 2024-03-17 03:15:04.000000 pyrob-0.6.1/src/pyrob/commands/uninstall.py
-drwxr-xr-x   0 r0b       (1000) r0b       (1000)        0 2024-03-18 00:16:51.188200 pyrob-0.6.1/src/pyrob/config/
--rw-r--r--   0 r0b       (1000) r0b       (1000)       21 2024-03-17 03:36:51.000000 pyrob-0.6.1/src/pyrob/config/__init__.py
--rw-r--r--   0 r0b       (1000) r0b       (1000)      103 2024-03-17 03:36:48.000000 pyrob-0.6.1/src/pyrob/config/vars.py
-drwxr-xr-x   0 r0b       (1000) r0b       (1000)        0 2024-03-18 00:16:51.188200 pyrob-0.6.1/src/pyrob/utils/
--rw-r--r--   0 r0b       (1000) r0b       (1000)      430 2024-03-17 03:36:44.000000 pyrob-0.6.1/src/pyrob/utils/__init__.py
--rw-r--r--   0 r0b       (1000) r0b       (1000)      313 2024-03-17 03:36:41.000000 pyrob-0.6.1/src/pyrob/utils/git.py
--rw-r--r--   0 r0b       (1000) r0b       (1000)      948 2024-03-17 03:36:39.000000 pyrob-0.6.1/src/pyrob/utils/meta.py
--rw-r--r--   0 r0b       (1000) r0b       (1000)     1073 2024-03-17 03:36:36.000000 pyrob-0.6.1/src/pyrob/utils/pip.py
-drwxr-xr-x   0 r0b       (1000) r0b       (1000)        0 2024-03-18 00:16:51.188200 pyrob-0.6.1/src/pyrob.egg-info/
--rw-r--r--   0 r0b       (1000) r0b       (1000)     3242 2024-03-18 00:16:51.000000 pyrob-0.6.1/src/pyrob.egg-info/PKG-INFO
--rw-r--r--   0 r0b       (1000) r0b       (1000)      556 2024-03-18 00:16:51.000000 pyrob-0.6.1/src/pyrob.egg-info/SOURCES.txt
--rw-r--r--   0 r0b       (1000) r0b       (1000)        1 2024-03-18 00:16:51.000000 pyrob-0.6.1/src/pyrob.egg-info/dependency_links.txt
--rw-r--r--   0 r0b       (1000) r0b       (1000)       41 2024-03-18 00:16:51.000000 pyrob-0.6.1/src/pyrob.egg-info/entry_points.txt
--rw-r--r--   0 r0b       (1000) r0b       (1000)        6 2024-03-18 00:16:51.000000 pyrob-0.6.1/src/pyrob.egg-info/top_level.txt
-drwxr-xr-x   0 r0b       (1000) r0b       (1000)        0 2024-03-18 00:16:51.188200 pyrob-0.6.1/tests/
--rw-r--r--   0 r0b       (1000) r0b       (1000)      630 2024-03-17 03:17:31.000000 pyrob-0.6.1/tests/test_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:45:23.998848 pyrob-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-05 14:45:02.000000 pyrob-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-05 14:45:23.998848 pyrob-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-05 14:45:02.000000 pyrob-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-05 14:45:02.000000 pyrob-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:45:23.998848 pyrob-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:45:23.990848 pyrob-0.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:45:23.990848 pyrob-0.8.1/src/pyrob/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-05 14:45:02.000000 pyrob-0.8.1/src/pyrob/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:45:23.990848 pyrob-0.8.1/src/pyrob/__template__/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:45:23.990848 pyrob-0.8.1/src/pyrob/__template__/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:45:23.994848 pyrob-0.8.1/src/pyrob/__template__/src/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:45:02.000000 pyrob-0.8.1/src/pyrob/__template__/src/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-05 14:45:02.000000 pyrob-0.8.1/src/pyrob/__template__/src/app/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:45:23.994848 pyrob-0.8.1/src/pyrob/__template__/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:45:02.000000 pyrob-0.8.1/src/pyrob/__template__/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:45:02.000000 pyrob-0.8.1/src/pyrob/__template__/tests/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-05 14:45:02.000000 pyrob-0.8.1/src/pyrob/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:45:23.994848 pyrob-0.8.1/src/pyrob/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-05 14:45:02.000000 pyrob-0.8.1/src/pyrob/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-05 14:45:02.000000 pyrob-0.8.1/src/pyrob/commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-05 14:45:02.000000 pyrob-0.8.1/src/pyrob/commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-05 14:45:02.000000 pyrob-0.8.1/src/pyrob/commands/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-05 14:45:02.000000 pyrob-0.8.1/src/pyrob/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-05 14:45:02.000000 pyrob-0.8.1/src/pyrob/commands/uninstall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:45:23.994848 pyrob-0.8.1/src/pyrob/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 14:45:02.000000 pyrob-0.8.1/src/pyrob/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-05 14:45:02.000000 pyrob-0.8.1/src/pyrob/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:45:23.994848 pyrob-0.8.1/src/pyrob/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-05 14:45:02.000000 pyrob-0.8.1/src/pyrob/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-05 14:45:02.000000 pyrob-0.8.1/src/pyrob/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-05 14:45:02.000000 pyrob-0.8.1/src/pyrob/utils/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-05 14:45:02.000000 pyrob-0.8.1/src/pyrob/utils/pip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-05 14:45:02.000000 pyrob-0.8.1/src/pyrob/utils/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-05 14:45:02.000000 pyrob-0.8.1/src/pyrob/utils/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:45:23.994848 pyrob-0.8.1/src/pyrob.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-05 14:45:23.000000 pyrob-0.8.1/src/pyrob.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-05 14:45:23.000000 pyrob-0.8.1/src/pyrob.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:45:23.000000 pyrob-0.8.1/src/pyrob.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 14:45:23.000000 pyrob-0.8.1/src/pyrob.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 14:45:23.000000 pyrob-0.8.1/src/pyrob.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:45:23.994848 pyrob-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-05 14:45:02.000000 pyrob-0.8.1/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-05 14:45:02.000000 pyrob-0.8.1/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-05 14:45:02.000000 pyrob-0.8.1/tests/test_utils.py
```

### Comparing `pyrob-0.6.1/LICENSE` & `pyrob-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrob-0.6.1/PKG-INFO` & `pyrob-0.8.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrob
-Version: 0.6.1
+Version: 0.8.1
 Summary: A CLI to manage dependencies in a Python project
 Author-email: Robert Adams <r0b4dams@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Robert Adams
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -34,29 +34,33 @@
 
 ```bash
 pip install pyrob
 ```
 
 ## Usage
 
-| Command                     | Description                                           |
-| --------------------------- | ----------------------------------------------------- |
-| `pyrm init [-y]`            | Initialize a new project                              |
-| `pyrm run [script]`         | Run the given command defined in project.json         |
-| `pyrm install [pkgs ...]`   | Install the given packages to virtual environment     |
-| `pyrm uninstall [pkgs ...]` | Uninstall the given packages from virtual environment |
+| Command                      | Description                                           |
+| ---------------------------- | ----------------------------------------------------- |
+| `pyrob init [-y]`            | Initialize a new project                              |
+| `pyrob run [script]`         | Run the given command defined in project.json         |
+| `pyrob install [pkgs ...]`   | Install the given packages to virtual environment     |
+| `pyrob uninstall [pkgs ...]` | Uninstall the given packages from virtual environment |
+| `pyrob clean`                | Remove cache artifacts (e.g. `__pycache__`)           |
 
 ## Development
 
 A Makefile is included with targets to handle dev actions
 
-| Command          | Description                                          |
-| ---------------- | ---------------------------------------------------- |
-| `make venv`      | Create a virtual environment with `venv` module      |
-| `make test`      | Run unit tests with `pytest`                         |
-| `make lint`      | Lint using `pylint`                                  |
-| `make format`    | Format using `black`                                 |
-| `make typecheck` | Typecheck using `mypy`                               |
-| `make build`     | Build a binary wheel and a source tarball            |
-| `make install`   | Install the package globally                         |
-| `make uninstall` | Uninstall package                                    |
-| `make clean`     | Delete virtual environment and build/cache artifacts |
+| Command                 | Description                                                  |
+| ----------------------- | ------------------------------------------------------------ |
+| `make venv`             | Create a virtual environment with `venv` module              |
+| `make test`             | Run unit tests with `pytest`                                 |
+| `make lint`             | Lint using `pylint`                                          |
+| `make format`           | Format using `black`                                         |
+| `make typecheck`        | Typecheck using `mypy`                                       |
+| `make build`            | Build a binary wheel and a source tarball                    |
+| `make release`          | Push a new tag, create a GitHub release, and publish to PyPI |
+| `make install`          | Install the package globally                                 |
+| `make uninstall`        | Uninstall package globally                                   |
+| `make clean`            | Delete virtual environment and build/cache artifacts         |
+| `make testpypi`         | Publishes current build to TestPyPI                          |
+| `make install_testpypi` | Install from TestPyPI                                        |
```

### Comparing `pyrob-0.6.1/README.md` & `pyrob-0.8.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -12,29 +12,33 @@
 
 ```bash
 pip install pyrob
 ```
 
 ## Usage
 
-| Command                     | Description                                           |
-| --------------------------- | ----------------------------------------------------- |
-| `pyrm init [-y]`            | Initialize a new project                              |
-| `pyrm run [script]`         | Run the given command defined in project.json         |
-| `pyrm install [pkgs ...]`   | Install the given packages to virtual environment     |
-| `pyrm uninstall [pkgs ...]` | Uninstall the given packages from virtual environment |
+| Command                      | Description                                           |
+| ---------------------------- | ----------------------------------------------------- |
+| `pyrob init [-y]`            | Initialize a new project                              |
+| `pyrob run [script]`         | Run the given command defined in project.json         |
+| `pyrob install [pkgs ...]`   | Install the given packages to virtual environment     |
+| `pyrob uninstall [pkgs ...]` | Uninstall the given packages from virtual environment |
+| `pyrob clean`                | Remove cache artifacts (e.g. `__pycache__`)           |
 
 ## Development
 
 A Makefile is included with targets to handle dev actions
 
-| Command          | Description                                          |
-| ---------------- | ---------------------------------------------------- |
-| `make venv`      | Create a virtual environment with `venv` module      |
-| `make test`      | Run unit tests with `pytest`                         |
-| `make lint`      | Lint using `pylint`                                  |
-| `make format`    | Format using `black`                                 |
-| `make typecheck` | Typecheck using `mypy`                               |
-| `make build`     | Build a binary wheel and a source tarball            |
-| `make install`   | Install the package globally                         |
-| `make uninstall` | Uninstall package                                    |
-| `make clean`     | Delete virtual environment and build/cache artifacts |
+| Command                 | Description                                                  |
+| ----------------------- | ------------------------------------------------------------ |
+| `make venv`             | Create a virtual environment with `venv` module              |
+| `make test`             | Run unit tests with `pytest`                                 |
+| `make lint`             | Lint using `pylint`                                          |
+| `make format`           | Format using `black`                                         |
+| `make typecheck`        | Typecheck using `mypy`                                       |
+| `make build`            | Build a binary wheel and a source tarball                    |
+| `make release`          | Push a new tag, create a GitHub release, and publish to PyPI |
+| `make install`          | Install the package globally                                 |
+| `make uninstall`        | Uninstall package globally                                   |
+| `make clean`            | Delete virtual environment and build/cache artifacts         |
+| `make testpypi`         | Publishes current build to TestPyPI                          |
+| `make install_testpypi` | Install from TestPyPI                                        |
```

### Comparing `pyrob-0.6.1/pyproject.toml` & `pyrob-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyrob-0.6.1/src/pyrob/cli.py` & `pyrob-0.8.1/src/pyrob/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """
 pyrob.cli
 """
 
+import os
+import sys
 from argparse import ArgumentParser
-from pyrob import commands, __pkg_name__, __version__
+from pyrob import commands, __version__
 
 
 def main():
     """
     entrypoint
     """
     parser = ArgumentParser(
-        prog=__pkg_name__,
+        prog=os.path.basename(sys.argv[0]),
         description="A CLI to manage dependencies in a Python project",
     )
     parser.add_argument(
         "-v", "--version", action="version", version=f"%(prog)s {__version__}"
     )
 
-    subparsers = parser.add_subparsers()
+    subparsers = parser.add_subparsers(title="command")
 
     init = subparsers.add_parser("init")
     init.add_argument("-y", action="store_true")
     init.set_defaults(func=commands.init)
 
     install = subparsers.add_parser("install")
     install.add_argument("pkgs", nargs="*")
@@ -32,14 +34,16 @@
     uninstall.add_argument("pkgs", nargs="+")
     uninstall.set_defaults(func=commands.uninstall)
 
     run = subparsers.add_parser("run")
     run.add_argument("script", nargs="?")
     run.set_defaults(func=commands.run)
 
-    parser.parse_args()
+    clean = subparsers.add_parser("clean")
+    clean.set_defaults(func=commands.clean)
+
     args = parser.parse_args()
 
     if hasattr(args, "func"):
         args.func(args)
     else:
         parser.print_help()
```

### Comparing `pyrob-0.6.1/src/pyrob/commands/init.py` & `pyrob-0.8.1/src/pyrob/commands/init.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,76 @@
 """
 pyrob.commands.init
 """
 
 import os
-from argparse import Namespace
-from pyrob.utils import meta, git
-from pyrob.config.vars import PROJECT_JSON
+import shutil
+import tempfile
+import argparse
+from pyrob.utils import git, meta, project
+from pyrob.config.vars import VENV, DEFAULT_REQS
+from pyrob.commands.install import install_from_args
 
 
-def init(args: Namespace) -> None:
+def init(args: argparse.Namespace) -> None:
     """
     Initialize a new project and generate a project.json file.
 
     Args:
         args: Command line arguments from argparse
     """
     try:
+        print("Initializing project...")
+
         base = from_default()
         data = base if args.y else with_prompts(base)
-        meta.write(PROJECT_JSON, data)
+
+        git.init()
+
+        src = os.path.join(os.path.dirname(__file__), "../", "__template__")
+        dst = os.getcwd()
+        ignore = shutil.ignore_patterns("__pycache__*")
+
+        with tempfile.TemporaryDirectory() as tmp:
+            git.get_gitignore(tmp)
+            meta.write(f"{tmp}/project.json", data)
+            shutil.copytree(src, tmp, dirs_exist_ok=True, ignore=ignore)
+            shutil.copytree(tmp, dst, dirs_exist_ok=True)
+
+        project.make_venv(VENV)
+        install_from_args(DEFAULT_REQS)
+
+        print("Project initialized! Happy hacking!")
 
     except (KeyboardInterrupt, EOFError):
         print("\nexit init")
 
 
 def from_default() -> dict:
     """
     Generate a base dict to serve as project.json shape.
 
     Returns:
         dict with default project.json values
     """
     user, email = git.get_config()
-    *_, current_folder_name = os.path.split(os.getcwd())
+    _, current_folder_name = os.path.split(os.getcwd())
 
     return {
         "name": current_folder_name,
         "version": "0.0.1",
         "author": f"{user} <{email}>",
         "description": "A new project!",
-        "scripts": {"foo": "echo foo bar baz"},
+        "scripts": {
+            "start": "python3 src/app/main.py",
+            "lint": "pylint src",
+            "test": "pytest tests -v",
+            "typecheck": "mypy src",
+            "format": "black src",
+        },
     }
 
 
 def with_prompts(default: dict) -> dict:
     """
     Prompt user to override default project metadata
```

### Comparing `pyrob-0.6.1/src/pyrob/commands/install.py` & `pyrob-0.8.1/src/pyrob/commands/install.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 pyrob.commands.install
 """
 
 import os
 import sys
 import tempfile
 from argparse import Namespace
-from pyrob.utils import create_venv, meta, pip
+from pyrob.utils import project, meta, pip
 from pyrob.config.vars import VENV, PROJECT_JSON
 
 
 def install(args: Namespace) -> None:
     """
     Install dependencies to virtual environment
 
     Args:
         args: Command line arguments from argparse
     """
     if not os.path.exists(VENV):
-        create_venv(VENV)
+        project.make_venv(VENV)
+
+    print("Installing packages...")
 
     if len(args.pkgs) > 0:
         install_from_args(args.pkgs)
     else:
         install_from_meta()
 
 
@@ -39,16 +41,16 @@
     try:
         doc = meta.read(PROJECT_JSON)
     except FileNotFoundError:
         pass
 
     pip.install_from_args(*pkgs)
     doc["requirements"] = pip.requirements()
-
     meta.write(PROJECT_JSON, doc)
+    print("Installed:", *pkgs)
 
 
 def install_from_meta() -> None:
     """
     Install packages from requirements in project.json.
 
     Raises:
```

### Comparing `pyrob-0.6.1/src/pyrob/commands/uninstall.py` & `pyrob-0.8.1/src/pyrob/commands/uninstall.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """pyrob.commands.uninstall"""
 
 import os
 import sys
 import json
-from argparse import Namespace
+import argparse
 from pyrob.utils import meta, pip
 from pyrob.config.vars import VENV, PROJECT_JSON
 
 
-def uninstall(args: Namespace) -> None:
+def uninstall(args: argparse.Namespace) -> None:
     """
     Uninstall packages from virtual environment.
 
     Args:
         args: Command line arguments from argparse
 
     Raises:
```

### Comparing `pyrob-0.6.1/src/pyrob/utils/meta.py` & `pyrob-0.8.1/src/pyrob/utils/meta.py`

 * *Files identical despite different names*

### Comparing `pyrob-0.6.1/src/pyrob/utils/pip.py` & `pyrob-0.8.1/src/pyrob/utils/pip.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 pyrob.utils.pip
 """
 
-from . import run
-from ..config.vars import PYTHON
+from pyrob.config.vars import PYTHON
+from .run import run
 
 
 def install_from_reqs(path: str) -> None:
     """
     Install packages to virtual environment from a requirements file.
 
     Args:
@@ -34,14 +34,14 @@
         pkgs: sequence of packages to uninstall
     """
     run([PYTHON, "-m", "pip", "uninstall", "-y", *pkgs])
 
 
 def requirements() -> dict:
     """
-    Cast pip freeze result to dict for package.json.
+    Cast pip freeze result to dict for project.json.
 
     Returns:
         A dict containing packages and their versions
     """
     reqs = run([PYTHON, "-m", "pip", "freeze"])
     return dict([pkg.split("==") for pkg in reqs.splitlines() if "==" in pkg])
```

### Comparing `pyrob-0.6.1/src/pyrob.egg-info/PKG-INFO` & `pyrob-0.8.1/src/pyrob.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrob
-Version: 0.6.1
+Version: 0.8.1
 Summary: A CLI to manage dependencies in a Python project
 Author-email: Robert Adams <r0b4dams@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Robert Adams
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -34,29 +34,33 @@
 
 ```bash
 pip install pyrob
 ```
 
 ## Usage
 
-| Command                     | Description                                           |
-| --------------------------- | ----------------------------------------------------- |
-| `pyrm init [-y]`            | Initialize a new project                              |
-| `pyrm run [script]`         | Run the given command defined in project.json         |
-| `pyrm install [pkgs ...]`   | Install the given packages to virtual environment     |
-| `pyrm uninstall [pkgs ...]` | Uninstall the given packages from virtual environment |
+| Command                      | Description                                           |
+| ---------------------------- | ----------------------------------------------------- |
+| `pyrob init [-y]`            | Initialize a new project                              |
+| `pyrob run [script]`         | Run the given command defined in project.json         |
+| `pyrob install [pkgs ...]`   | Install the given packages to virtual environment     |
+| `pyrob uninstall [pkgs ...]` | Uninstall the given packages from virtual environment |
+| `pyrob clean`                | Remove cache artifacts (e.g. `__pycache__`)           |
 
 ## Development
 
 A Makefile is included with targets to handle dev actions
 
-| Command          | Description                                          |
-| ---------------- | ---------------------------------------------------- |
-| `make venv`      | Create a virtual environment with `venv` module      |
-| `make test`      | Run unit tests with `pytest`                         |
-| `make lint`      | Lint using `pylint`                                  |
-| `make format`    | Format using `black`                                 |
-| `make typecheck` | Typecheck using `mypy`                               |
-| `make build`     | Build a binary wheel and a source tarball            |
-| `make install`   | Install the package globally                         |
-| `make uninstall` | Uninstall package                                    |
-| `make clean`     | Delete virtual environment and build/cache artifacts |
+| Command                 | Description                                                  |
+| ----------------------- | ------------------------------------------------------------ |
+| `make venv`             | Create a virtual environment with `venv` module              |
+| `make test`             | Run unit tests with `pytest`                                 |
+| `make lint`             | Lint using `pylint`                                          |
+| `make format`           | Format using `black`                                         |
+| `make typecheck`        | Typecheck using `mypy`                                       |
+| `make build`            | Build a binary wheel and a source tarball                    |
+| `make release`          | Push a new tag, create a GitHub release, and publish to PyPI |
+| `make install`          | Install the package globally                                 |
+| `make uninstall`        | Uninstall package globally                                   |
+| `make clean`            | Delete virtual environment and build/cache artifacts         |
+| `make testpypi`         | Publishes current build to TestPyPI                          |
+| `make install_testpypi` | Install from TestPyPI                                        |
```

### Comparing `pyrob-0.6.1/src/pyrob.egg-info/SOURCES.txt` & `pyrob-0.8.1/src/pyrob.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,28 @@
 src/pyrob/__init__.py
 src/pyrob/cli.py
 src/pyrob.egg-info/PKG-INFO
 src/pyrob.egg-info/SOURCES.txt
 src/pyrob.egg-info/dependency_links.txt
 src/pyrob.egg-info/entry_points.txt
 src/pyrob.egg-info/top_level.txt
+src/pyrob/__template__/src/app/__init__.py
+src/pyrob/__template__/src/app/main.py
+src/pyrob/__template__/tests/__init__.py
+src/pyrob/__template__/tests/test_example.py
 src/pyrob/commands/__init__.py
+src/pyrob/commands/clean.py
 src/pyrob/commands/init.py
 src/pyrob/commands/install.py
 src/pyrob/commands/run.py
 src/pyrob/commands/uninstall.py
 src/pyrob/config/__init__.py
 src/pyrob/config/vars.py
 src/pyrob/utils/__init__.py
 src/pyrob/utils/git.py
 src/pyrob/utils/meta.py
 src/pyrob/utils/pip.py
-tests/test_meta.py
+src/pyrob/utils/project.py
+src/pyrob/utils/run.py
+tests/test_meta.py
+tests/test_run.py
+tests/test_utils.py
```

### Comparing `pyrob-0.6.1/tests/test_meta.py` & `pyrob-0.8.1/tests/test_meta.py`

 * *Files identical despite different names*

