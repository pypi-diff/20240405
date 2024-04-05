# Comparing `tmp/daves-dev-tools-2.1.1.tar.gz` & `tmp/daves-dev-tools-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daves-dev-tools-2.1.1.tar", last modified: Sun Feb 18 16:51:00 2024, max compression
+gzip compressed data, was "daves-dev-tools-2.1.2.tar", last modified: Fri Apr  5 19:15:50 2024, max compression
```

## Comparing `daves-dev-tools-2.1.1.tar` & `daves-dev-tools-2.1.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 16:51:00.331186 daves-dev-tools-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    13249 2024-02-18 16:51:00.331186 daves-dev-tools-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12753 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 16:51:00.327186 daves-dev-tools-2.1.1/daves_dev_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/daves_dev_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/daves_dev_tools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/daves_dev_tools/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/daves_dev_tools/distribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/daves_dev_tools/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 16:51:00.327186 daves-dev-tools-2.1.1/daves_dev_tools/git/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/daves_dev_tools/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/daves_dev_tools/git/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/daves_dev_tools/git/download.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/daves_dev_tools/git/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/daves_dev_tools/git/tag_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    14780 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/daves_dev_tools/install_editable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/daves_dev_tools/make_typed.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/daves_dev_tools/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 16:51:00.331186 daves-dev-tools-2.1.1/daves_dev_tools/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/daves_dev_tools/requirements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/daves_dev_tools/requirements/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/daves_dev_tools/requirements/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/daves_dev_tools/requirements/freeze.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/daves_dev_tools/requirements/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/daves_dev_tools/requirements/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/daves_dev_tools/requirements/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/daves_dev_tools/uninstall_all.py
--rw-r--r--   0 runner    (1001) docker     (127)    17935 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/daves_dev_tools/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 16:51:00.331186 daves-dev-tools-2.1.1/daves_dev_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13249 2024-02-18 16:51:00.000000 daves-dev-tools-2.1.1/daves_dev_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-02-18 16:51:00.000000 daves-dev-tools-2.1.1/daves_dev_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-18 16:51:00.000000 daves-dev-tools-2.1.1/daves_dev_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-18 16:51:00.000000 daves-dev-tools-2.1.1/daves_dev_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-18 16:51:00.000000 daves-dev-tools-2.1.1/daves_dev_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-18 16:51:00.000000 daves-dev-tools-2.1.1/daves_dev_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-02-18 16:51:00.331186 daves-dev-tools-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 16:51:00.331186 daves-dev-tools-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/tests/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/tests/test_distribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/tests/test_git_download.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/tests/test_install_editable.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/tests/test_make_typed.py
--rw-r--r--   0 runner    (1001) docker     (127)     7507 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/tests/test_requirements_update.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/tests/test_uninstall_all.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-02-18 16:50:43.000000 daves-dev-tools-2.1.1/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:15:50.507318 daves-dev-tools-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    13249 2024-04-05 19:15:50.507318 daves-dev-tools-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12753 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:15:50.503318 daves-dev-tools-2.1.2/daves_dev_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/daves_dev_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/daves_dev_tools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/daves_dev_tools/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/daves_dev_tools/distribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/daves_dev_tools/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:15:50.507318 daves-dev-tools-2.1.2/daves_dev_tools/git/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/daves_dev_tools/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/daves_dev_tools/git/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/daves_dev_tools/git/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/daves_dev_tools/git/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/daves_dev_tools/git/tag_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14780 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/daves_dev_tools/install_editable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/daves_dev_tools/make_typed.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/daves_dev_tools/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:15:50.507318 daves-dev-tools-2.1.2/daves_dev_tools/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/daves_dev_tools/requirements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/daves_dev_tools/requirements/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/daves_dev_tools/requirements/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/daves_dev_tools/requirements/freeze.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/daves_dev_tools/requirements/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/daves_dev_tools/requirements/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/daves_dev_tools/requirements/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/daves_dev_tools/uninstall_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17935 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/daves_dev_tools/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:15:50.507318 daves-dev-tools-2.1.2/daves_dev_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13249 2024-04-05 19:15:50.000000 daves-dev-tools-2.1.2/daves_dev_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-05 19:15:50.000000 daves-dev-tools-2.1.2/daves_dev_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:15:50.000000 daves-dev-tools-2.1.2/daves_dev_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-05 19:15:50.000000 daves-dev-tools-2.1.2/daves_dev_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-05 19:15:50.000000 daves-dev-tools-2.1.2/daves_dev_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 19:15:50.000000 daves-dev-tools-2.1.2/daves_dev_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-05 19:15:50.507318 daves-dev-tools-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:15:50.507318 daves-dev-tools-2.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/tests/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/tests/test_distribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/tests/test_git_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/tests/test_install_editable.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/tests/test_make_typed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7507 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/tests/test_requirements_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/tests/test_uninstall_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-05 19:15:30.000000 daves-dev-tools-2.1.2/tests/test_utilities.py
```

### Comparing `daves-dev-tools-2.1.1/PKG-INFO` & `daves-dev-tools-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daves-dev-tools
-Version: 2.1.1
+Version: 2.1.2
 Summary: Dave's developer tools
 Home-page: https://github.com/enorganic/daves-dev-tools
 Author-email: david@belais.me
 License: MIT
 Keywords: dave,dev,tools
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
```

### Comparing `daves-dev-tools-2.1.1/README.md` & `daves-dev-tools-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `daves-dev-tools-2.1.1/daves_dev_tools/__main__.py` & `daves-dev-tools-2.1.2/daves_dev_tools/__main__.py`

 * *Files identical despite different names*

### Comparing `daves-dev-tools-2.1.1/daves_dev_tools/clean.py` & `daves-dev-tools-2.1.2/daves_dev_tools/clean.py`

 * *Files identical despite different names*

### Comparing `daves-dev-tools-2.1.1/daves_dev_tools/distribute.py` & `daves-dev-tools-2.1.2/daves_dev_tools/distribute.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,80 +1,78 @@
 import functools
 import os
 import re
 import sys
-from subprocess import check_call, check_output, list2cmdline
+import tempfile
+from subprocess import check_output
 from time import time
 from typing import Any, Callable, FrozenSet, Iterable, List, Tuple
 
+from setuptools import build_meta  # type: ignore
+
 from .utilities import run_module_as_main, sys_argv_pop
 
 lru_cache: Callable[..., Any] = functools.lru_cache
+_SYS_ARGV: Tuple[str, ...] = tuple(sys.argv)
 
 
-def _list_dist(
+def _list_modified(
     directory: str, modified_at_or_after: float = 0.0
 ) -> FrozenSet[str]:
-    dist_root: str = os.path.join(directory, "dist")
     dist_file: str
     dist_sub_directories: List[str]
     dist_files: Iterable[str]
     try:
-        dist_root, dist_sub_directories, dist_files = next(
-            iter(os.walk(dist_root))
+        directory, dist_sub_directories, dist_files = next(
+            iter(os.walk(directory))
         )
     except StopIteration:
         raise FileNotFoundError(
-            f"No distributions could be found in {dist_root}"
+            f"No distributions could be found in {directory}"
         )
-    dist_files = (
-        os.path.join(dist_root, dist_file) for dist_file in dist_files
+    dist_files = tuple(
+        os.path.join(directory, dist_file) for dist_file in dist_files
     )
     if modified_at_or_after:
         dist_files = filter(
             lambda dist_file: (  # noqa
                 os.path.getmtime(dist_file) >= modified_at_or_after
             ),
             dist_files,
         )
     try:
         return frozenset(dist_files)
     except (NotADirectoryError, FileNotFoundError):
         return frozenset()
 
 
-def _run_setup(script_name: str, script_args: Tuple[str, ...] = ()) -> None:
-    """
-    This function replaces `distutils.core.run_setup`
-    """
-    command: Tuple[str, ...] = (sys.executable, script_name) + script_args
-    print(list2cmdline(command))
-    check_call(command)
-
-
 def _setup(directory: str) -> FrozenSet[str]:
     start_time: float = time()
     current_directory: str = os.path.abspath(os.path.curdir)
     os.chdir(directory)
     try:
-        abs_setup: str = os.path.join(directory, "setup.py")
-        setup_args: Tuple[str, ...] = ("sdist", "bdist_wheel")
-        _run_setup(abs_setup, setup_args)
+        metadata_directory: str = tempfile.mkdtemp()
+        dist_directory: str = tempfile.mkdtemp()
+        build_meta.build_sdist(dist_directory)
+        build_meta.prepare_metadata_for_build_wheel(metadata_directory)
+        build_meta.build_wheel(
+            dist_directory, metadata_directory=metadata_directory
+        )
     finally:
         os.chdir(current_directory)
-    return _list_dist(directory, modified_at_or_after=start_time)
+    return _list_modified(dist_directory, modified_at_or_after=start_time)
 
 
 def _get_help() -> bool:
     """
     If `-h` or `--help` keyword arguments are provided,
     retrieve the repository credentials and store them in the "TWINE_USERNAME"
     and "TWINE_PASSWORD" environment variables.
     """
-    if set(sys.argv) & {"-h", "--help", "-H", "--HELP"}:
+    if set(_SYS_ARGV) & {"-h", "--help", "-H", "--HELP"}:
         help_: str = check_output(
             (sys.executable, "-m", "twine", "upload", "-h"),
             encoding="utf-8",
             universal_newlines=True,
         ).strip()
         help_ = re.sub(
             r"\btwine upload\b",
@@ -99,36 +97,27 @@
         return True
     return False
 
 
 def _dist(
     directory: str, distributions: FrozenSet[str], echo: bool = True
 ) -> None:
+    arguments: Tuple[str, ...] = (
+        ("upload",) + tuple(_SYS_ARGV[1:]) + tuple(sorted(distributions))
+    )
     run_module_as_main(
         "twine",
-        arguments=(["upload"] + sys.argv[1:] + list(sorted(distributions))),
+        arguments=arguments,
         directory=directory,
         echo=False,
     )
 
 
-def _cleanup(directory: str) -> None:
-    current_directory: str = os.path.abspath(os.path.curdir)
-    os.chdir(directory)
-    try:
-        _run_setup(os.path.join(directory, "setup.py"), ("clean", "--all"))
-    finally:
-        os.chdir(current_directory)
-
-
 def main() -> None:
     if not _get_help():
         directory: str = sys_argv_pop(depth=2, default=".")  # type: ignore
         directory = os.path.abspath(directory).rstrip("/")
-        try:
-            _dist(directory, _setup(directory))
-        finally:
-            _cleanup(directory)
+        _dist(directory, _setup(directory))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `daves-dev-tools-2.1.1/daves_dev_tools/errors.py` & `daves-dev-tools-2.1.2/daves_dev_tools/errors.py`

 * *Files identical despite different names*

### Comparing `daves-dev-tools-2.1.1/daves_dev_tools/git/__main__.py` & `daves-dev-tools-2.1.2/daves_dev_tools/git/__main__.py`

 * *Files identical despite different names*

### Comparing `daves-dev-tools-2.1.1/daves_dev_tools/git/download.py` & `daves-dev-tools-2.1.2/daves_dev_tools/git/download.py`

 * *Files identical despite different names*

### Comparing `daves-dev-tools-2.1.1/daves_dev_tools/git/tag_version.py` & `daves-dev-tools-2.1.2/daves_dev_tools/git/tag_version.py`

 * *Files identical despite different names*

### Comparing `daves-dev-tools-2.1.1/daves_dev_tools/install_editable.py` & `daves-dev-tools-2.1.2/daves_dev_tools/install_editable.py`

 * *Files identical despite different names*

### Comparing `daves-dev-tools-2.1.1/daves_dev_tools/make_typed.py` & `daves-dev-tools-2.1.2/daves_dev_tools/make_typed.py`

 * *Files identical despite different names*

### Comparing `daves-dev-tools-2.1.1/daves_dev_tools/requirements/__main__.py` & `daves-dev-tools-2.1.2/daves_dev_tools/requirements/__main__.py`

 * *Files identical despite different names*

### Comparing `daves-dev-tools-2.1.1/daves_dev_tools/requirements/utilities.py` & `daves-dev-tools-2.1.2/daves_dev_tools/requirements/utilities.py`

 * *Files identical despite different names*

### Comparing `daves-dev-tools-2.1.1/daves_dev_tools/uninstall_all.py` & `daves-dev-tools-2.1.2/daves_dev_tools/uninstall_all.py`

 * *Files identical despite different names*

### Comparing `daves-dev-tools-2.1.1/daves_dev_tools/utilities.py` & `daves-dev-tools-2.1.2/daves_dev_tools/utilities.py`

 * *Files identical despite different names*

### Comparing `daves-dev-tools-2.1.1/daves_dev_tools.egg-info/PKG-INFO` & `daves-dev-tools-2.1.2/daves_dev_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daves-dev-tools
-Version: 2.1.1
+Version: 2.1.2
 Summary: Dave's developer tools
 Home-page: https://github.com/enorganic/daves-dev-tools
 Author-email: david@belais.me
 License: MIT
 Keywords: dave,dev,tools
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
```

### Comparing `daves-dev-tools-2.1.1/daves_dev_tools.egg-info/SOURCES.txt` & `daves-dev-tools-2.1.2/daves_dev_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `daves-dev-tools-2.1.1/setup.cfg` & `daves-dev-tools-2.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = daves-dev-tools
-version = 2.1.1
+version = 2.1.2
 author_email = david@belais.me
 description = Dave's developer tools
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = dave, dev, tools
 license = MIT
 url = https://github.com/enorganic/daves-dev-tools
```

### Comparing `daves-dev-tools-2.1.1/tests/test_git_download.py` & `daves-dev-tools-2.1.2/tests/test_git_download.py`

 * *Files identical despite different names*

### Comparing `daves-dev-tools-2.1.1/tests/test_requirements_update.py` & `daves-dev-tools-2.1.2/tests/test_requirements_update.py`

 * *Files identical despite different names*

### Comparing `daves-dev-tools-2.1.1/tests/test_utilities.py` & `daves-dev-tools-2.1.2/tests/test_utilities.py`

 * *Files identical despite different names*

