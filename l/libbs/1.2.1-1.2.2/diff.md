# Comparing `tmp/libbs-1.2.1.tar.gz` & `tmp/libbs-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libbs-1.2.1.tar", last modified: Wed Apr  3 06:21:29 2024, max compression
+gzip compressed data, was "libbs-1.2.2.tar", last modified: Fri Apr  5 00:50:29 2024, max compression
```

## Comparing `libbs-1.2.1.tar` & `libbs-1.2.2.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.279162 libbs-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-03 06:21:25.000000 libbs-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-04-03 06:21:29.279162 libbs-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-03 06:21:25.000000 libbs-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.267162 libbs-1.2.1/libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.271162 libbs-1.2.1/libbs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/api/artifact_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/api/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)    26006 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/api/decompiler_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/api/type_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.271162 libbs-1.2.1/libbs/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/artifacts/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/artifacts/comment.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/artifacts/decompilation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/artifacts/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/artifacts/func.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/artifacts/global_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/artifacts/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/artifacts/stack_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/artifacts/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.271162 libbs-1.2.1/libbs/decompiler_stubs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompiler_stubs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.271162 libbs-1.2.1/libbs/decompiler_stubs/angr_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompiler_stubs/angr_libbs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.271162 libbs-1.2.1/libbs/decompiler_stubs/binja_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompiler_stubs/binja_libbs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.275162 libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_mainthread_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_shutdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.275162 libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.275162 libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    89858 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompiler_stubs/ida_libbs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.275162 libbs-1.2.1/libbs/decompilers/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.275162 libbs-1.2.1/libbs/decompilers/angr/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/angr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/angr/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/angr/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/angr/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.275162 libbs-1.2.1/libbs/decompilers/binja/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/binja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/binja/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/binja/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    20930 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/binja/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.279162 libbs-1.2.1/libbs/decompilers/ghidra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/ghidra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/ghidra/artifact_lifter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.279162 libbs-1.2.1/libbs/decompilers/ghidra/compat/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/ghidra/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/ghidra/compat/ghidra_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/ghidra/compat/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/ghidra/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    31335 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/ghidra/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.279162 libbs-1.2.1/libbs/decompilers/ida/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/ida/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)    30549 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/ida/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/ida/hooks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12593 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/ida/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/plugin_installer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.279162 libbs-1.2.1/libbs/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/ui/qt_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/ui/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/ui/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.279162 libbs-1.2.1/libbs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-04-03 06:21:29.000000 libbs-1.2.1/libbs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-03 06:21:29.000000 libbs-1.2.1/libbs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 06:21:29.000000 libbs-1.2.1/libbs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-03 06:21:29.000000 libbs-1.2.1/libbs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 06:21:29.000000 libbs-1.2.1/libbs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 06:21:29.000000 libbs-1.2.1/libbs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-03 06:21:29.283162 libbs-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-03 06:21:25.000000 libbs-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.279162 libbs-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-03 06:21:25.000000 libbs-1.2.1/tests/test_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-03 06:21:25.000000 libbs-1.2.1/tests/test_decompilers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.882559 libbs-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-05 00:50:25.000000 libbs-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-05 00:50:29.882559 libbs-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-05 00:50:25.000000 libbs-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.870559 libbs-1.2.2/libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.874559 libbs-1.2.2/libbs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/api/artifact_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/api/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26006 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/api/decompiler_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/api/type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.874559 libbs-1.2.2/libbs/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/artifacts/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/artifacts/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/artifacts/decompilation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/artifacts/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/artifacts/func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/artifacts/global_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/artifacts/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/artifacts/stack_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/artifacts/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.874559 libbs-1.2.2/libbs/decompiler_stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompiler_stubs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.874559 libbs-1.2.2/libbs/decompiler_stubs/angr_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompiler_stubs/angr_libbs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.874559 libbs-1.2.2/libbs/decompiler_stubs/binja_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompiler_stubs/binja_libbs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.878559 libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_mainthread_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_shutdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.878559 libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.878559 libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89858 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompiler_stubs/ida_libbs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.878559 libbs-1.2.2/libbs/decompilers/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.878559 libbs-1.2.2/libbs/decompilers/angr/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/angr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/angr/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/angr/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/angr/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.878559 libbs-1.2.2/libbs/decompilers/binja/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/binja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/binja/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/binja/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20930 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/binja/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.878559 libbs-1.2.2/libbs/decompilers/ghidra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/ghidra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/ghidra/artifact_lifter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.882559 libbs-1.2.2/libbs/decompilers/ghidra/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/ghidra/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/ghidra/compat/ghidra_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/ghidra/compat/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/ghidra/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32537 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/ghidra/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.882559 libbs-1.2.2/libbs/decompilers/ida/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/ida/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30549 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/ida/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/ida/hooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12593 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/decompilers/ida/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/plugin_installer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.882559 libbs-1.2.2/libbs/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/ui/qt_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/ui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-05 00:50:25.000000 libbs-1.2.2/libbs/ui/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.882559 libbs-1.2.2/libbs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-05 00:50:29.000000 libbs-1.2.2/libbs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-05 00:50:29.000000 libbs-1.2.2/libbs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 00:50:29.000000 libbs-1.2.2/libbs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-05 00:50:29.000000 libbs-1.2.2/libbs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-05 00:50:29.000000 libbs-1.2.2/libbs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 00:50:29.000000 libbs-1.2.2/libbs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-05 00:50:29.882559 libbs-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-05 00:50:25.000000 libbs-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:50:29.882559 libbs-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-05 00:50:25.000000 libbs-1.2.2/tests/test_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-05 00:50:25.000000 libbs-1.2.2/tests/test_decompilers.py
```

### Comparing `libbs-1.2.1/LICENSE` & `libbs-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/PKG-INFO` & `libbs-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: libbs
-Version: 1.2.1
+Version: 1.2.2
 Summary: Your Only Decompiler API Lib - A generic API to script in and out of decompilers
 Home-page: https://github.com/binsync/libbs
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: toml
 Requires-Dist: pycparser
 Requires-Dist: setuptools
 Requires-Dist: prompt_toolkit
 Requires-Dist: tqdm
+Requires-Dist: jfx_bridge
 Requires-Dist: ghidra_bridge
 Requires-Dist: psutil
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: angr; extra == "test"
 
 # LibBS
```

### Comparing `libbs-1.2.1/README.md` & `libbs-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/__main__.py` & `libbs-1.2.2/libbs/__main__.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/api/artifact_dict.py` & `libbs-1.2.2/libbs/api/artifact_dict.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/api/artifact_lifter.py` & `libbs-1.2.2/libbs/api/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/api/decompiler_interface.py` & `libbs-1.2.2/libbs/api/decompiler_interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/api/type_parser.py` & `libbs-1.2.2/libbs/api/type_parser.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/api/utils.py` & `libbs-1.2.2/libbs/api/utils.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/artifacts/artifact.py` & `libbs-1.2.2/libbs/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/artifacts/comment.py` & `libbs-1.2.2/libbs/artifacts/comment.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/artifacts/decompilation.py` & `libbs-1.2.2/libbs/artifacts/decompilation.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/artifacts/enum.py` & `libbs-1.2.2/libbs/artifacts/enum.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/artifacts/func.py` & `libbs-1.2.2/libbs/artifacts/func.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/artifacts/global_variable.py` & `libbs-1.2.2/libbs/artifacts/global_variable.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/artifacts/patch.py` & `libbs-1.2.2/libbs/artifacts/patch.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/artifacts/stack_variable.py` & `libbs-1.2.2/libbs/artifacts/stack_variable.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/artifacts/struct.py` & `libbs-1.2.2/libbs/artifacts/struct.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py` & `libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py` & `libbs-1.2.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/decompilers/angr/artifact_lifter.py` & `libbs-1.2.2/libbs/decompilers/angr/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/decompilers/angr/compat.py` & `libbs-1.2.2/libbs/decompilers/angr/compat.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/decompilers/angr/interface.py` & `libbs-1.2.2/libbs/decompilers/angr/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/decompilers/binja/artifact_lifter.py` & `libbs-1.2.2/libbs/decompilers/binja/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/decompilers/binja/hooks.py` & `libbs-1.2.2/libbs/decompilers/binja/hooks.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/decompilers/binja/interface.py` & `libbs-1.2.2/libbs/decompilers/binja/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/decompilers/ghidra/artifact_lifter.py` & `libbs-1.2.2/libbs/decompilers/ghidra/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/decompilers/ghidra/compat/ghidra_api.py` & `libbs-1.2.2/libbs/decompilers/ghidra/compat/ghidra_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import time
 import logging
 
 import ghidra_bridge
+from jfx_bridge.bridge import BridgedObject
 
 _l = logging.getLogger(__name__)
 
 
 class GhidraAPIWrapper:
     def __init__(self, controller, connection_timeout=10):
         self._controller = controller
@@ -71,8 +72,16 @@
         if self.bridge is not None:
             try:
                 self.bridge.remote_eval("True")
                 connected = True
             except Exception:
                 pass
 
-        return connected
+        return connected
+
+    @staticmethod
+    def isinstance(obj, cls):
+        """
+        A proxy isinstance function that can handle BridgedObjects. This is necessary because the `isinstance` function
+        in the remote namespace will not recognize BridgedObjects as instances of classes in the local namespace.
+        """
+        return obj._bridge_isinstance(cls) if isinstance(obj, BridgedObject) else isinstance(obj, cls)
```

### Comparing `libbs-1.2.1/libbs/decompilers/ghidra/hooks.py` & `libbs-1.2.2/libbs/decompilers/ghidra/hooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,36 +50,41 @@
                 oldValue = record.getOldValue()
                 obj = record.getObject()
 
                 if changeType in funcEvents:
                     pass
                 elif changeType in typeEvents:
                     try:
-                        struct = self._interface.structs['/'+newValue.name]
+                        struct = self._interface.structs[newValue.name]
                         # TODO: access old name indicate deletion
                         #self._interface.struct_changed(Struct(None, None, None), deleted=True)
                         self._interface.struct_changed(struct)
                     except KeyError:
                         pass
 
                     try:
-                        enum = self._interface.enums['/'+newValue.name]
+                        enum = self._interface.enums[newValue.name]
                         #self._interface.enum_changed(Enum(None, None), deleted=True)
                         self._interface.enum_changed(enum)
                     except KeyError:
                         pass
 
                 elif changeType in symDelEvents:
                     # Currently unused and unsupported
                     pass
                 elif changeType in symChgEvents:
                     if obj is None and newValue is not None:
                         obj = newValue
                     if "VariableSymbolDB" in str(type(obj)):
-                        if oldValue and newValue and obj.parentNamespace is not None:
+                        parent_namespace = obj.getParentNamespace()
+                        storage = obj.getVariableStorage()
+                        if (
+                            (newValue is not None) and (storage is not None) and bool(storage.isStackStorage())
+                            and (parent_namespace is not None)
+                        ):
                             self._interface.stack_variable_changed(
                                 self._interface.art_lifter.lift(
                                     StackVariable(
                                         int(obj.variableStorage.stackOffset),
                                         newValue,
                                         None,
                                         None,
```

### Comparing `libbs-1.2.1/libbs/decompilers/ghidra/interface.py` & `libbs-1.2.2/libbs/decompilers/ghidra/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -386,15 +386,15 @@
             changes = True
 
         return changes
 
     @ghidra_transaction
     def _set_struct(self, struct: Struct, header=True, members=True, **kwargs) -> bool:
         struct: Struct = struct
-        old_ghidra_struct = self._get_struct_by_name('/' + struct.name)
+        old_ghidra_struct = self._get_struct_by_name(struct.name)
         data_manager = self.ghidra.currentProgram.getDataTypeManager()
         handler = self.ghidra.import_module_object("ghidra.program.model.data", "DataTypeConflictHandler")
         structType = self.ghidra.import_module_object("ghidra.program.model.data", "StructureDataType")
         byteType = self.ghidra.import_module_object("ghidra.program.model.data", "ByteDataType")
         ghidra_struct = structType(struct.name, 0)
         for offset in struct.members:
             member = struct.members[offset]
@@ -404,35 +404,37 @@
                 if dtc.getFieldName() == member.name:
                     gtype = self.typestr_to_gtype(member.type if member.type else 'undefined' + str(member.size))
                     for i in range(offset, offset + member.size):
                         ghidra_struct.clearAtOffset(i)
                     ghidra_struct.replaceAtOffset(offset, gtype, member.size, member.name, "")
                     break
         try:
-            if old_ghidra_struct:
+            if old_ghidra_struct is not None:
                 data_manager.replaceDataType(old_ghidra_struct, ghidra_struct, True)
             else:
                 data_manager.addDataType(ghidra_struct, handler.DEFAULT_HANDLER)
             return True
         except Exception as ex:
             print(f'Error filling struct {struct.name}: {ex}')
             return False
 
     def _get_struct(self, name) -> Optional[Struct]:
         ghidra_struct = self._get_struct_by_name(name)
-        bs_struct = Struct(ghidra_struct.getName(), ghidra_struct.getLength(), self._struct_members_from_gstruct(name))
-        return bs_struct
+        if ghidra_struct is None:
+            return None
+
+        return Struct(ghidra_struct.getName(), ghidra_struct.getLength(), self._struct_members_from_gstruct(name))
 
     def _structs(self) -> Dict[str, Struct]:
         name_sizes: Optional[List[Tuple[str, int]]] = self.ghidra.bridge.remote_eval(
             "[(s.getPathName(), s.getLength())"
             "for s in currentProgram.getDataTypeManager().getAllStructures()]"
         )
         return {
-            name: Struct(name, size, members=self._struct_members_from_gstruct(name)) for name, size in name_sizes
+            name[1:]: Struct(name[1:], size, members=self._struct_members_from_gstruct(name[1:])) for name, size in name_sizes
         } if name_sizes else {}
 
     @ghidra_transaction
     def _set_comment(self, comment: Comment, **kwargs) -> bool:
         CodeUnit = self.ghidra.import_module_object("ghidra.program.model.listing", "CodeUnit")
         SetCommentCmd = self.ghidra.import_module_object("ghidra.app.cmd.comments", "SetCommentCmd")
         cmt_type = CodeUnit.PRE_COMMENT if comment.decompiled else CodeUnit.EOL_COMMENT
@@ -488,28 +490,45 @@
                 data_manager.addDataType(ghidra_enum, handler.DEFAULT_HANDLER)
             return True
         except Exception as ex:
             print(f'Error adding enum {enum.name}: {ex}')
             return False
 
     def _get_enum(self, name) -> Optional[Enum]:
-        members = self._get_enum_members('/' + name)
+        is_valid_enum = self._get_ghidra_enum(name)
+        if is_valid_enum is None:
+            return None
+
+        members = self._get_enum_members(name)
         return Enum(name, members) if members else None
 
     def _enums(self) -> Dict[str, Enum]:
         names: Optional[List[str]] = self.ghidra.bridge.remote_eval(
             "[dType.getPathName() "
             "for dType in currentProgram.getDataTypeManager().getAllDataTypes()"
             "if str(type(dType)) == \"<type 'ghidra.program.database.data.EnumDB'>\"]"
         )
-        return {name[1:]: Enum(name[1:], self._get_enum_members(name)) for name in names if
-                name.count('/') == 1} if names else {}
+        enums = {}
+        for name in names:
+            # XXX: we dont really know why this is here, but we assume its because you cant have
+            # an enum nested in a folder in ghidra
+            if name.count("/") != 1:
+                continue
+
+            enum_name = name[1:]
+            is_valid_enum = self._get_ghidra_enum(enum_name)
+            if is_valid_enum is None:
+                continue
+
+            enums[enum_name] = Enum(enum_name, self._get_enum_members(enum_name))
+
+        return enums
 
     @ghidra_transaction
-    def fill_global_var(self, var_addr, user=None, artifact=None, **kwargs):
+    def _set_global_variable(self, var_addr, user=None, artifact=None, **kwargs):
         """
         TODO: remove me and implement me properly as setters and getters
         """
 
         changes = False
         global_var: GlobalVariable = artifact
         all_global_vars = self._global_vars()
@@ -632,33 +651,42 @@
     def _get_local_variable_symbols(self, func: Function) -> Dict[str, "HighSymbol"]:
         high_func = func.dec_obj.getHighFunction()
         return self.ghidra.bridge.remote_eval(
             "{sym.name: sym for sym in high_func.getLocalSymbolMap().getSymbols() if sym.name}",
             high_func=high_func
         )
 
-    def _get_struct_by_name(self, name: str) -> "GhidraStructure":
-        return self.ghidra.currentProgram.getDataTypeManager().getDataType(name)
+    def _get_struct_by_name(self, name: str) -> Optional["StructureDB"]:
+        """
+        Returns None if the struct does not exist or is not a struct.
+        """
+        StructureDBType = self.ghidra.import_module_object("ghidra.program.database.data", "StructureDB")
+        struct = self.ghidra.currentProgram.getDataTypeManager().getDataType("/" + name)
+        return struct if self.ghidra.isinstance(struct, StructureDBType) else None
 
     def _struct_members_from_gstruct(self, name: str) -> Dict[int, StructMember]:
         ghidra_struct = self._get_struct_by_name(name)
+        if ghidra_struct is None:
+            return {}
+
         members: Optional[List[Tuple[str, int, str, int]]] = self.ghidra.bridge.remote_eval(
             "[(m.getFieldName(), m.getOffset(), m.getDataType().getName(), m.getLength()) if m.getFieldName() else "
             "('field_'+hex(m.getOffset())[2:], m.getOffset(), m.getDataType().getName(), m.getLength()) "
             "for m in ghidra_struct.getComponents()]",
             ghidra_struct=ghidra_struct
         )
         return {
             offset: StructMember(name, offset, typestr, size) for name, offset, typestr, size in members
         } if members else {}
 
     def _get_enum_members(self, name: str) -> Optional[Dict[str, int]]:
-        ghidra_enum = self.ghidra.currentProgram.getDataTypeManager().getDataType(name)
-        if not ghidra_enum:
-            return None
+        ghidra_enum = self._get_ghidra_enum(name)
+        if ghidra_enum is None:
+            return {}
+
         name_vals: Optional[List[Tuple[str, int]]] = self.ghidra.bridge.remote_eval(
             "[(name, ghidra_enum.getValue(name))"
             "for name in ghidra_enum.getNames()]",
             ghidra_enum=ghidra_enum
         )
         return {name: value for name, value in name_vals} if name_vals else {}
 
@@ -756,7 +784,12 @@
 
     def _run_until_server_closed(self, sleep_interval=30):
         while True:
             if not self.ghidra.ping():
                 break
 
             time.sleep(sleep_interval)
+
+    def _get_ghidra_enum(self, enum_name: str) -> Optional["EnumDB"]:
+        ghidra_enum = self.ghidra.currentProgram.getDataTypeManager().getDataType("/" + enum_name)
+        EnumDBType = self.ghidra.import_module_object("ghidra.program.database.data", "EnumDB")
+        return ghidra_enum if self.ghidra.isinstance(ghidra_enum, EnumDBType) else None
```

### Comparing `libbs-1.2.1/libbs/decompilers/ida/artifact_lifter.py` & `libbs-1.2.2/libbs/decompilers/ida/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/decompilers/ida/compat.py` & `libbs-1.2.2/libbs/decompilers/ida/compat.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/decompilers/ida/hooks.py` & `libbs-1.2.2/libbs/decompilers/ida/hooks.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/decompilers/ida/interface.py` & `libbs-1.2.2/libbs/decompilers/ida/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/logger.py` & `libbs-1.2.2/libbs/logger.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/plugin_installer.py` & `libbs-1.2.2/libbs/plugin_installer.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/ui/__init__.py` & `libbs-1.2.2/libbs/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/ui/qt_objects.py` & `libbs-1.2.2/libbs/ui/qt_objects.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs/ui/utils.py` & `libbs-1.2.2/libbs/ui/utils.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/libbs.egg-info/PKG-INFO` & `libbs-1.2.2/libbs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: libbs
-Version: 1.2.1
+Version: 1.2.2
 Summary: Your Only Decompiler API Lib - A generic API to script in and out of decompilers
 Home-page: https://github.com/binsync/libbs
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: toml
 Requires-Dist: pycparser
 Requires-Dist: setuptools
 Requires-Dist: prompt_toolkit
 Requires-Dist: tqdm
+Requires-Dist: jfx_bridge
 Requires-Dist: ghidra_bridge
 Requires-Dist: psutil
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: angr; extra == "test"
 
 # LibBS
```

### Comparing `libbs-1.2.1/libbs.egg-info/SOURCES.txt` & `libbs-1.2.2/libbs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/setup.cfg` & `libbs-1.2.2/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 [options]
 install_requires = 
 	toml
 	pycparser
 	setuptools
 	prompt_toolkit
 	tqdm
+	jfx_bridge
 	ghidra_bridge
 	psutil
 python_requires = >= 3.8
 include_package_data = True
 packages = find:
 
 [options.entry_points]
```

### Comparing `libbs-1.2.1/tests/test_artifacts.py` & `libbs-1.2.2/tests/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.1/tests/test_decompilers.py` & `libbs-1.2.2/tests/test_decompilers.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 class TestHeadlessInterfaces(unittest.TestCase):
     def setUp(self):
         self._generic_renamed_name = "binsync_main"
         self._fauxware_path = TEST_BINARY_DIR / "fauxware"
 
     def test_ghidra(self):
+        # TODO: Add test cases for structs and enums
         # useful command for testing, kills all Headless-Ghidra:
         # kill $(ps aux | grep 'Ghidra-Headless' | awk '{print $2}')
         deci = DecompilerInterface.discover(
             force_decompiler=GHIDRA_DECOMPILER,
             headless=True,
             headless_dec_path=DEC_TO_HEADLESS[GHIDRA_DECOMPILER],
             binary_path=self._fauxware_path,
@@ -49,14 +50,40 @@
         func_args[0].size = 4   # set manually to avoid resetting the size in the caller
         func_args[1].name = "new_name_2"
         func_args[1].type = "double"
         func_args[1].size = 8
         deci.functions[func_addr] = main
         assert deci.functions[func_addr].header.args == func_args
 
+        struct = deci.structs['eh_frame_hdr']
+        struct.name = "my_struct_name"
+        struct.members[0].type = 'undefined'
+        struct.members[1].type = 'undefined'
+        deci.structs['eh_frame_hdr'] = struct
+        updated = deci.structs[struct.name]
+        assert updated.name == struct.name
+        assert updated.members[0].type == 'undefined'
+        assert updated.members[1].type == 'undefined'
+
+        enum = Enum("my_enum", {"member1": 0, "member2": 1})
+        deci.enums[enum.name] = enum
+        assert deci.enums[enum.name] == enum
+
+        # gvar_addr = deci.art_lifter.lift_addr(0x4008e0)
+        # g1 = deci.global_vars[gvar_addr]
+        # g1.name = "gvar1"
+        # deci.global_vars[gvar_addr] = g1
+        # assert deci.global_vars[gvar_addr] == g1
+
+        stack_var = main.stack_vars[-24]
+        stack_var.name = "named_char_array"
+        stack_var.type = 'double'
+        deci.functions[func_addr] = main
+        assert deci.functions[func_addr].stack_vars[-24] == stack_var
+
         #
         # Test Artifact Watchers
         #
 
         hits = defaultdict(list)
         def func_hit(*args, **kwargs): hits[args[0].__class__].append(args[0])
 
@@ -75,21 +102,24 @@
 
         first_changed_func = hits[FunctionHeader][0]
         assert first_changed_func.name == "changed"
         assert first_changed_func.addr == func_addr
         assert len(hits[FunctionHeader]) == 2
 
         # TODO: Fix CI for below
-        # main.stack_vars[-24].name = "named_char_array"
-        # main.stack_vars[-12].name = "named_int"
-        # deci.functions[func_addr] = main
+        main.stack_vars[-24].name = "named_char_array"
+        main.stack_vars[-12].name = "named_int"
+        deci.functions[func_addr] = main
+        #first_changed_sv = hits[StackVariable][0]
+        #assert first_changed_sv.name == main.stack_vars[-24].name
+        #assert len(hits[StackVariable]) == 2
 
-        # struct = deci.structs['/eh_frame_hdr']
+        # struct = deci.structs['eh_frame_hdr']
         # struct.name = "my_struct_name"
-        # deci.structs['/eh_frame_hdr'] = struct
+        # deci.structs['eh_frame_hdr'] = struct
 
         # TODO: add argument naming
         # func_args = main.header.args
         # func_args[0].name = "changed_name"
         # func_args[1].name = "changed_name2"
         # deci.functions[func_addr] = main
 
@@ -97,15 +127,14 @@
         # g1 = deci.global_vars[0x4008e0]
         # g2 = deci.global_vars[0x601048]
         # g1.name = "gvar1"
         # g2.name = "gvar2"
         # deci.global_vars[0x4008e0] = g1
         # deci.global_vars[0x601048] = g2
 
-        #assert hits[StackVariable] == 2
         #assert hits[Struct] == 2 # One change results in 2 hits because the struct is first removed and then added again.
         #assert hits[GlobalVariable] == 2
 
         deci.shutdown()
 
     def test_angr(self):
         deci = DecompilerInterface.discover(
```

