# Comparing `tmp/sinol_make-1.6.0.dev2.tar.gz` & `tmp/sinol_make-1.6.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinol_make-1.6.0.dev2.tar", last modified: Thu Apr  4 21:08:04 2024, max compression
+gzip compressed data, was "sinol_make-1.6.0.dev3.tar", last modified: Thu Apr  4 21:18:57 2024, max compression
```

## Comparing `sinol_make-1.6.0.dev2.tar` & `sinol_make-1.6.0.dev3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.576036 sinol_make-1.6.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-04 21:08:04.576036 sinol_make-1.6.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-04 21:08:04.576036 sinol_make-1.6.0.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.564036 sinol_make-1.6.0.dev2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.568036 sinol_make-1.6.0.dev2/src/sinol_make/
--rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.564036 sinol_make-1.6.0.dev2/src/sinol_make/commands/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.568036 sinol_make-1.6.0.dev2/src/sinol_make/commands/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/commands/doc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.568036 sinol_make-1.6.0.dev2/src/sinol_make/commands/export/
--rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/commands/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.568036 sinol_make-1.6.0.dev2/src/sinol_make/commands/gen/
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/commands/gen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.568036 sinol_make-1.6.0.dev2/src/sinol_make/commands/ingen/
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/commands/ingen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/commands/ingen/ingen_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.568036 sinol_make-1.6.0.dev2/src/sinol_make/commands/init/
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/commands/init/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.568036 sinol_make-1.6.0.dev2/src/sinol_make/commands/inwer/
--rw-r--r--   0 runner    (1001) docker     (127)     9543 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/commands/inwer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/commands/inwer/inwer_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.568036 sinol_make-1.6.0.dev2/src/sinol_make/commands/outgen/
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/commands/outgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/commands/outgen/outgen_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.572036 sinol_make-1.6.0.dev2/src/sinol_make/commands/run/
--rw-r--r--   0 runner    (1001) docker     (127)    57981 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/commands/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.572036 sinol_make-1.6.0.dev2/src/sinol_make/commands/verify/
--rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/commands/verify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.572036 sinol_make-1.6.0.dev2/src/sinol_make/contest_types/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/contest_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/contest_types/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/contest_types/icpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/contest_types/oi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.572036 sinol_make-1.6.0.dev2/src/sinol_make/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/helpers/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/helpers/compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/helpers/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    14656 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/helpers/package_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/helpers/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/helpers/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/helpers/printer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.572036 sinol_make-1.6.0.dev2/src/sinol_make/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/interfaces/BaseCommand.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/interfaces/Errors.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.572036 sinol_make-1.6.0.dev2/src/sinol_make/oiejq/
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/oiejq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/oiejq/perf_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.572036 sinol_make-1.6.0.dev2/src/sinol_make/structs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/structs/cache_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/structs/compiler_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/structs/gen_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/structs/inwer_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/structs/run_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/structs/status_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13853 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.576036 sinol_make-1.6.0.dev2/src/sinol_make.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-04 21:08:04.000000 sinol_make-1.6.0.dev2/src/sinol_make.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-04 21:08:04.000000 sinol_make-1.6.0.dev2/src/sinol_make.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 21:08:04.000000 sinol_make-1.6.0.dev2/src/sinol_make.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-04 21:08:04.000000 sinol_make-1.6.0.dev2/src/sinol_make.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-04 21:08:04.000000 sinol_make-1.6.0.dev2/src/sinol_make.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 21:08:04.000000 sinol_make-1.6.0.dev2/src/sinol_make.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.576036 sinol_make-1.6.0.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/tests/test_multiple_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/tests/test_oiejq.py
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.391683 sinol_make-1.6.0.dev3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-04 21:18:57.391683 sinol_make-1.6.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-04 21:18:57.391683 sinol_make-1.6.0.dev3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.379683 sinol_make-1.6.0.dev3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.379683 sinol_make-1.6.0.dev3/src/sinol_make/
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.379683 sinol_make-1.6.0.dev3/src/sinol_make/commands/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.383683 sinol_make-1.6.0.dev3/src/sinol_make/commands/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/commands/doc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.383683 sinol_make-1.6.0.dev3/src/sinol_make/commands/export/
+-rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/commands/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.383683 sinol_make-1.6.0.dev3/src/sinol_make/commands/gen/
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/commands/gen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.383683 sinol_make-1.6.0.dev3/src/sinol_make/commands/ingen/
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/commands/ingen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/commands/ingen/ingen_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.383683 sinol_make-1.6.0.dev3/src/sinol_make/commands/init/
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/commands/init/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.383683 sinol_make-1.6.0.dev3/src/sinol_make/commands/inwer/
+-rw-r--r--   0 runner    (1001) docker     (127)     9543 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/commands/inwer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/commands/inwer/inwer_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.383683 sinol_make-1.6.0.dev3/src/sinol_make/commands/outgen/
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/commands/outgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/commands/outgen/outgen_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.383683 sinol_make-1.6.0.dev3/src/sinol_make/commands/run/
+-rw-r--r--   0 runner    (1001) docker     (127)    57981 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/commands/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.383683 sinol_make-1.6.0.dev3/src/sinol_make/commands/verify/
+-rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/commands/verify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.383683 sinol_make-1.6.0.dev3/src/sinol_make/contest_types/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/contest_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/contest_types/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/contest_types/icpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/contest_types/oi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.387683 sinol_make-1.6.0.dev3/src/sinol_make/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/helpers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/helpers/compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/helpers/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14656 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/helpers/package_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/helpers/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/helpers/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/helpers/printer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.387683 sinol_make-1.6.0.dev3/src/sinol_make/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/interfaces/BaseCommand.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/interfaces/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.387683 sinol_make-1.6.0.dev3/src/sinol_make/oiejq/
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/oiejq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/oiejq/perf_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.387683 sinol_make-1.6.0.dev3/src/sinol_make/structs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/structs/cache_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/structs/compiler_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/structs/gen_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/structs/inwer_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/structs/run_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/structs/status_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13924 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/src/sinol_make/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.387683 sinol_make-1.6.0.dev3/src/sinol_make.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-04 21:18:57.000000 sinol_make-1.6.0.dev3/src/sinol_make.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-04 21:18:57.000000 sinol_make-1.6.0.dev3/src/sinol_make.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 21:18:57.000000 sinol_make-1.6.0.dev3/src/sinol_make.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-04 21:18:57.000000 sinol_make-1.6.0.dev3/src/sinol_make.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-04 21:18:57.000000 sinol_make-1.6.0.dev3/src/sinol_make.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 21:18:57.000000 sinol_make-1.6.0.dev3/src/sinol_make.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:18:57.387683 sinol_make-1.6.0.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/tests/test_multiple_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/tests/test_oiejq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-04 21:18:52.000000 sinol_make-1.6.0.dev3/tests/test_util.py
```

### Comparing `sinol_make-1.6.0.dev2/LICENSE` & `sinol_make-1.6.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/PKG-INFO` & `sinol_make-1.6.0.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinol_make
-Version: 1.6.0.dev2
+Version: 1.6.0.dev3
 Summary: CLI tool for creating sio2 task packages
 Author: Mateusz Masiarz
 Author-email: m.masiarz@fri.edu.pl
 Maintainer: Tomasz Nowak, Mateusz Masiarz
 Maintainer-email: tomasz.nowak@tonowak.com, m.masiarz@fri.edu.pl
 Project-URL: Bug Tracker, https://github.com/sio2project/sinol-make/issues
 Project-URL: Homepage, https://github.com/sio2project/sinol-make
```

### Comparing `sinol_make-1.6.0.dev2/README.md` & `sinol_make-1.6.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/setup.cfg` & `sinol_make-1.6.0.dev3/setup.cfg`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/__init__.py` & `sinol_make-1.6.0.dev3/src/sinol_make/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import argparse
 import traceback
 import argcomplete
 
 from sinol_make import util, oiejq
 
-__version__ = "1.6.0.dev2"
+__version__ = "1.6.0.dev3"
 
 
 def configure_parsers():
     parser = argparse.ArgumentParser(
         prog='sinol-make',
         description='Tool for creating and testing sio2 tasks',
     )
```

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/commands/doc/__init__.py` & `sinol_make-1.6.0.dev3/src/sinol_make/commands/doc/__init__.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/commands/export/__init__.py` & `sinol_make-1.6.0.dev3/src/sinol_make/commands/export/__init__.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/commands/gen/__init__.py` & `sinol_make-1.6.0.dev3/src/sinol_make/commands/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/commands/ingen/__init__.py` & `sinol_make-1.6.0.dev3/src/sinol_make/commands/ingen/__init__.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/commands/ingen/ingen_util.py` & `sinol_make-1.6.0.dev3/src/sinol_make/commands/ingen/ingen_util.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/commands/init/__init__.py` & `sinol_make-1.6.0.dev3/src/sinol_make/commands/init/__init__.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/commands/inwer/__init__.py` & `sinol_make-1.6.0.dev3/src/sinol_make/commands/inwer/__init__.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/commands/inwer/inwer_util.py` & `sinol_make-1.6.0.dev3/src/sinol_make/commands/inwer/inwer_util.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/commands/outgen/__init__.py` & `sinol_make-1.6.0.dev3/src/sinol_make/commands/outgen/__init__.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/commands/outgen/outgen_util.py` & `sinol_make-1.6.0.dev3/src/sinol_make/commands/outgen/outgen_util.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/commands/run/__init__.py` & `sinol_make-1.6.0.dev3/src/sinol_make/commands/run/__init__.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/commands/verify/__init__.py` & `sinol_make-1.6.0.dev3/src/sinol_make/commands/verify/__init__.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/contest_types/__init__.py` & `sinol_make-1.6.0.dev3/src/sinol_make/contest_types/__init__.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/contest_types/default.py` & `sinol_make-1.6.0.dev3/src/sinol_make/contest_types/default.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/contest_types/icpc.py` & `sinol_make-1.6.0.dev3/src/sinol_make/contest_types/icpc.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/contest_types/oi.py` & `sinol_make-1.6.0.dev3/src/sinol_make/contest_types/oi.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/helpers/cache.py` & `sinol_make-1.6.0.dev3/src/sinol_make/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/helpers/compile.py` & `sinol_make-1.6.0.dev3/src/sinol_make/helpers/compile.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/helpers/compiler.py` & `sinol_make-1.6.0.dev3/src/sinol_make/helpers/compiler.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/helpers/package_util.py` & `sinol_make-1.6.0.dev3/src/sinol_make/helpers/package_util.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/helpers/parsers.py` & `sinol_make-1.6.0.dev3/src/sinol_make/helpers/parsers.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/helpers/paths.py` & `sinol_make-1.6.0.dev3/src/sinol_make/helpers/paths.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/helpers/printer.py` & `sinol_make-1.6.0.dev3/src/sinol_make/helpers/printer.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/oiejq/__init__.py` & `sinol_make-1.6.0.dev3/src/sinol_make/oiejq/__init__.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/structs/cache_structs.py` & `sinol_make-1.6.0.dev3/src/sinol_make/structs/cache_structs.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/structs/compiler_structs.py` & `sinol_make-1.6.0.dev3/src/sinol_make/structs/compiler_structs.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/structs/inwer_structs.py` & `sinol_make-1.6.0.dev3/src/sinol_make/structs/inwer_structs.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/structs/run_structs.py` & `sinol_make-1.6.0.dev3/src/sinol_make/structs/run_structs.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/structs/status_structs.py` & `sinol_make-1.6.0.dev3/src/sinol_make/structs/status_structs.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make/util.py` & `sinol_make-1.6.0.dev3/src/sinol_make/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,17 @@
     except requests.exceptions.RequestException:
         return
 
     if request.status_code != 200:
         return
 
     data = request.json()
-    latest_version = data["info"]["version"]
+    versions = list(data["releases"].keys())
+    versions.sort(key=parse_version)
+    latest_version = versions[-1]
 
     version_file = importlib.files("sinol_make").joinpath("data/version")
     try:
         version_file.write_text(latest_version)
     except PermissionError:
         if find_and_chdir_package():
             try:
```

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make.egg-info/PKG-INFO` & `sinol_make-1.6.0.dev3/src/sinol_make.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinol_make
-Version: 1.6.0.dev2
+Version: 1.6.0.dev3
 Summary: CLI tool for creating sio2 task packages
 Author: Mateusz Masiarz
 Author-email: m.masiarz@fri.edu.pl
 Maintainer: Tomasz Nowak, Mateusz Masiarz
 Maintainer-email: tomasz.nowak@tonowak.com, m.masiarz@fri.edu.pl
 Project-URL: Bug Tracker, https://github.com/sio2project/sinol-make/issues
 Project-URL: Homepage, https://github.com/sio2project/sinol-make
```

### Comparing `sinol_make-1.6.0.dev2/src/sinol_make.egg-info/SOURCES.txt` & `sinol_make-1.6.0.dev3/src/sinol_make.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/tests/test_multiple_arguments.py` & `sinol_make-1.6.0.dev3/tests/test_multiple_arguments.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/tests/test_oiejq.py` & `sinol_make-1.6.0.dev3/tests/test_oiejq.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev2/tests/test_util.py` & `sinol_make-1.6.0.dev3/tests/test_util.py`

 * *Files identical despite different names*

