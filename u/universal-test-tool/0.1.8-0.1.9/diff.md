# Comparing `tmp/universal-test-tool-0.1.8.tar.gz` & `tmp/universal-test-tool-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "universal-test-tool-0.1.8.tar", last modified: Sun Jan 28 10:03:40 2024, max compression
+gzip compressed data, was "universal-test-tool-0.1.9.tar", last modified: Sun Jan 28 14:42:45 2024, max compression
```

## Comparing `universal-test-tool-0.1.8.tar` & `universal-test-tool-0.1.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 10:03:40.342658 universal-test-tool-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13289 2024-01-28 10:03:40.342658 universal-test-tool-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12372 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-28 10:03:40.342658 universal-test-tool-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 10:03:40.334658 universal-test-tool-0.1.8/test_tool/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12667 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool/test_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 10:03:40.334658 universal-test-tool-0.1.8/test_tool_assert_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool_assert_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool_assert_plugin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool_assert_plugin/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 10:03:40.334658 universal-test-tool-0.1.8/test_tool_copy_files_ssh_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool_copy_files_ssh_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool_copy_files_ssh_plugin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool_copy_files_ssh_plugin/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 10:03:40.334658 universal-test-tool-0.1.8/test_tool_jdbc_sql_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool_jdbc_sql_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool_jdbc_sql_plugin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool_jdbc_sql_plugin/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 10:03:40.338658 universal-test-tool-0.1.8/test_tool_read_jar_manifest_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool_read_jar_manifest_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool_read_jar_manifest_plugin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool_read_jar_manifest_plugin/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 10:03:40.338658 universal-test-tool-0.1.8/test_tool_rest_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool_rest_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool_rest_plugin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13439 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool_rest_plugin/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 10:03:40.338658 universal-test-tool-0.1.8/test_tool_run_process_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool_run_process_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool_run_process_plugin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool_run_process_plugin/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 10:03:40.338658 universal-test-tool-0.1.8/test_tool_selenium_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool_selenium_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool_selenium_plugin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool_selenium_plugin/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 10:03:40.338658 universal-test-tool-0.1.8/test_tool_sql_plus_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool_sql_plus_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool_sql_plus_plugin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool_sql_plus_plugin/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 10:03:40.338658 universal-test-tool-0.1.8/test_tool_ssh_cmd_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool_ssh_cmd_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool_ssh_cmd_plugin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/test_tool_ssh_cmd_plugin/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 10:03:40.338658 universal-test-tool-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-28 10:03:30.000000 universal-test-tool-0.1.8/tests/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 10:03:40.342658 universal-test-tool-0.1.8/universal_test_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13289 2024-01-28 10:03:40.000000 universal-test-tool-0.1.8/universal_test_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-01-28 10:03:40.000000 universal-test-tool-0.1.8/universal_test_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-28 10:03:40.000000 universal-test-tool-0.1.8/universal_test_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-01-28 10:03:40.000000 universal-test-tool-0.1.8/universal_test_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-01-28 10:03:40.000000 universal-test-tool-0.1.8/universal_test_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-01-28 10:03:40.000000 universal-test-tool-0.1.8/universal_test_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:42:45.856227 universal-test-tool-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13289 2024-01-28 14:42:45.856227 universal-test-tool-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12372 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-28 14:42:45.856227 universal-test-tool-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:42:45.848227 universal-test-tool-0.1.9/test_tool/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12667 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool/test_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:42:45.852227 universal-test-tool-0.1.9/test_tool_assert_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool_assert_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool_assert_plugin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool_assert_plugin/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:42:45.852227 universal-test-tool-0.1.9/test_tool_copy_files_ssh_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool_copy_files_ssh_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool_copy_files_ssh_plugin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool_copy_files_ssh_plugin/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:42:45.852227 universal-test-tool-0.1.9/test_tool_jdbc_sql_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool_jdbc_sql_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool_jdbc_sql_plugin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool_jdbc_sql_plugin/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:42:45.852227 universal-test-tool-0.1.9/test_tool_read_jar_manifest_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool_read_jar_manifest_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool_read_jar_manifest_plugin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool_read_jar_manifest_plugin/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:42:45.852227 universal-test-tool-0.1.9/test_tool_rest_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool_rest_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool_rest_plugin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16392 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool_rest_plugin/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:42:45.852227 universal-test-tool-0.1.9/test_tool_run_process_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool_run_process_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool_run_process_plugin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool_run_process_plugin/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:42:45.852227 universal-test-tool-0.1.9/test_tool_selenium_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool_selenium_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool_selenium_plugin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool_selenium_plugin/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:42:45.852227 universal-test-tool-0.1.9/test_tool_sql_plus_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool_sql_plus_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool_sql_plus_plugin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool_sql_plus_plugin/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:42:45.856227 universal-test-tool-0.1.9/test_tool_ssh_cmd_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool_ssh_cmd_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool_ssh_cmd_plugin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/test_tool_ssh_cmd_plugin/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:42:45.856227 universal-test-tool-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-28 14:42:35.000000 universal-test-tool-0.1.9/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:42:45.856227 universal-test-tool-0.1.9/universal_test_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13289 2024-01-28 14:42:45.000000 universal-test-tool-0.1.9/universal_test_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-01-28 14:42:45.000000 universal-test-tool-0.1.9/universal_test_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-28 14:42:45.000000 universal-test-tool-0.1.9/universal_test_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-01-28 14:42:45.000000 universal-test-tool-0.1.9/universal_test_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-01-28 14:42:45.000000 universal-test-tool-0.1.9/universal_test_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-01-28 14:42:45.000000 universal-test-tool-0.1.9/universal_test_tool.egg-info/top_level.txt
```

### Comparing `universal-test-tool-0.1.8/HISTORY.md` & `universal-test-tool-0.1.9/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Feat: modify rest plugin. [Jakob Graf]
+- Release: version 0.1.8 🚀 [Jakob Graf]
+
+
+0.1.8 (2024-01-28)
+------------------
+- Release: version 0.1.8 🚀 [Jakob Graf]
 - Bug: line numbers. [Jakob Graf]
 
 
 0.1.7 (2024-01-17)
 ------------------
 - Release: version 0.1.7 🚀 [Jakob Graf]
 - Bug: formatting. [Jakob Graf]
```

### Comparing `universal-test-tool-0.1.8/LICENSE` & `universal-test-tool-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `universal-test-tool-0.1.8/PKG-INFO` & `universal-test-tool-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: universal-test-tool
-Version: 0.1.8
+Version: 0.1.9
 Summary: Awesome universal-test-tool to make tests configurable with a yaml file.
 Home-page: https://github.com/jackovsky8/universal-test-tool/
 Author: jackovsky8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: types-PyYAML
 Requires-Dist: python-dotenv
```

### Comparing `universal-test-tool-0.1.8/README.md` & `universal-test-tool-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `universal-test-tool-0.1.8/setup.py` & `universal-test-tool-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `universal-test-tool-0.1.8/test_tool/base.py` & `universal-test-tool-0.1.9/test_tool/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,15 +289,15 @@
             )
             # Augment the call with the data from the config
             LOADED_CALL_TYPES[test["type"]]["augment_call"](call, data, path)
             # Make the call
             LOADED_CALL_TYPES[test["type"]]["make_call"](call, data)
         except AssertionError as e:
             test_tool_logger.error(
-                "Assertion error for test from line %s: %s", call["line"], e
+                "Assertion error for test from line %s: %s", test["line"], e
             )
             errors += 1
         except Exception as e:  # pylint: disable=broad-except
             test_tool_logger.error(
                 'Exception "%s" occured for test from line %s '
                 + "(This might be a problem with the plugin or config).",
                 e,
```

### Comparing `universal-test-tool-0.1.8/test_tool/test_tool.py` & `universal-test-tool-0.1.9/test_tool/test_tool.py`

 * *Files identical despite different names*

### Comparing `universal-test-tool-0.1.8/test_tool_assert_plugin/main.py` & `universal-test-tool-0.1.9/test_tool_assert_plugin/main.py`

 * *Files identical despite different names*

### Comparing `universal-test-tool-0.1.8/test_tool_copy_files_ssh_plugin/main.py` & `universal-test-tool-0.1.9/test_tool_copy_files_ssh_plugin/main.py`

 * *Files identical despite different names*

### Comparing `universal-test-tool-0.1.8/test_tool_jdbc_sql_plugin/main.py` & `universal-test-tool-0.1.9/test_tool_jdbc_sql_plugin/main.py`

 * *Files identical despite different names*

### Comparing `universal-test-tool-0.1.8/test_tool_read_jar_manifest_plugin/main.py` & `universal-test-tool-0.1.9/test_tool_read_jar_manifest_plugin/main.py`

 * *Files identical despite different names*

### Comparing `universal-test-tool-0.1.8/test_tool_rest_plugin/main.py` & `universal-test-tool-0.1.9/test_tool_rest_plugin/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 This is the main file of the plugin. It is called by the test tool and
 contains the main function.
 """
 from enum import Enum
-from json import JSONDecodeError, dumps
+import json
 from logging import error, info
 from pathlib import Path
 from typing import IO, Any, Dict, List, Optional, Tuple, TypedDict
 from xml.dom.minidom import parseString
 
 from requests import delete, get, post, put
 
@@ -26,14 +26,80 @@
     This class represents a certificate.
     """
 
     path: Path
     key: Optional[str]
 
 
+class BodyType(Enum):
+    """
+    This class represents the type of the request body.
+    """
+    TEXT_PLAIN = 'text/plain'
+    MULTIPART_FORM_DATA = 'multipart/form-data'
+    APPLICATION_JSON = 'application/json'
+    APPLICATION_XML = 'application/xml'
+    APPLICATION_OCTET_STREAM = 'application/octet-stream'
+    APPLICATION_PDF = 'application/pdf'
+    APPLICATION_ZIP = 'application/zip'
+    APPLICATION_GZIP = 'application/gzip'
+    APPLICATION_TAR = 'application/tar'
+    APPLICATION_XHTML_XML = 'application/xhtml+xml'
+    APPLICATION_XML_DTD = 'application/xml-dtd'
+    APPLICATION_XOP_XML = 'application/xop+xml'
+    APPLICATION_X_TAR = 'application/x-tar'
+    APPLICATION_X_GZIP = 'application/x-gzip'
+    APPLICATION_X_BZIP2 = 'application/x-bzip2'
+    APPLICATION_X_7Z_COMPRESSED = 'application/x-7z-compressed'
+    APPLICATION_X_RAR_COMPRESSED = 'application/x-rar-compressed'
+    APPLICATION_X_JAVA_ARCHIVE = 'application/x-java-archive'
+    APPLICATION_X_RAR = 'application/x-rar'
+    APPLICATION_X_SHOCKWAVE_FLASH = 'application/x-shockwave-flash'
+    APPLICATION_X_SQLITE3 = 'application/x-sqlite3'
+    APPLICATION_X_WWW_FORM_URLENCODED = 'application/x-www-form-urlencoded'
+    AUDIO_MPEG = 'audio/mpeg'
+    AUDIO_X_MS_WMA = 'audio/x-ms-wma'
+    AUDIO_X_WAV = 'audio/x-wav'
+    IMAGE_GIF = 'image/gif'
+    IMAGE_JPEG = 'image/jpeg'
+    IMAGE_PNG = 'image/png'
+    IMAGE_SVG_XML = 'image/svg+xml'
+    IMAGE_TIFF = 'image/tiff'
+    IMAGE_VND_MICROSOFT_ICON = 'image/vnd.microsoft.icon'
+    IMAGE_X_ICON = 'image/x-icon'
+    IMAGE_X_MS_BMP = 'image/x-ms-bmp'
+    TEXT_CSS = 'text/css'
+    TEXT_CSV = 'text/csv'
+    TEXT_HTML = 'text/html'
+    TEXT_JAVASCRIPT = 'text/javascript'
+    TEXT_XML = 'text/xml'
+    VIDEO_3GPP = 'video/3gpp'
+    VIDEO_3GPP2 = 'video/3gpp2'
+    VIDEO_MPEG = 'video/mpeg'
+    VIDEO_QUICKTIME = 'video/quicktime'
+    VIDEO_X_MSVIDEO = 'video/x-msvideo'
+    VIDEO_X_SGI_MOVIE = 'video/x-sgi-movie'
+    VIDEO_X_WEBM = 'video/x-webm'
+    VIDEO_X_FLV = 'video/x-flv'
+    VIDEO_X_MATROSKA = 'video/x-matroska'
+    VIDEO_X_MS_WMV = 'video/x-ms-wmv'
+    VIDEO_X_MS_ASF = 'video/x-ms-asf'
+    VIDEO_X_M4V = 'video/x-m4v'
+    VIDEO_X_MSVID = 'video/x-msvid'
+
+
+class Body(TypedDict):
+    """
+    This class represents the body of the request.
+    """
+
+    type: BodyType
+    data: Any
+
+
 class Method(Enum):
     """
     This class represents the method of the request.
     """
 
     POST = 1
     GET = 2
@@ -72,15 +138,15 @@
 
     # URL
     base_url: str
     path: str
     url: str
     # Request
     method: Method
-    data: Optional[str | Dict[str, Any]]
+    body: Optional[Body]
     files: Optional[Dict[str, File | LoadedFile | EmptyFile]]
     multipart: Optional[Dict[str, Tuple[None, str, str]]]
     # payload: Optional[Dict[str, str]]
     # To request
     timeout: int
     headers: Dict
     verify: bool
@@ -93,15 +159,15 @@
 
 
 default_rest_call: RestCall = {
     "base_url": "${REST_BASE_URL}",
     "path": "${REST_PATH}",
     "url": None,  # type: ignore
     "method": "GET",  # type: ignore
-    "data": None,
+    "body": None,
     "files": None,
     "multipart": None,
     # "payload": None,
     # Special
     "timeout": 0,
     "headers": {},
     "verify": False,
@@ -125,48 +191,53 @@
     # hooks: _HooksInput | None = ...,
     # stream: bool | None = ...,
     # verify: _Verify | None = ...,
     # cert: _Cert | None = ...,
     # json: Any | None = ...
 }
 
+default_request_body: Dict[str, Any] = {
+    "type": BodyType.TEXT_PLAIN,
+    "value": None
+}
+
 
-def pretty_xml(xml: str) -> str:
+def pretty_xml(string: str) -> str:
     """
     Return a pretty printed xml string.
 
     Parameters
     ----------
     xml : str
         The xml string.
 
     Returns
     -------
     str
         The pretty printed xml string.
     """
-    dom = parseString(xml)
+    dom = parseString(string)
     return dom.toprettyxml()
 
 
-def pretty_json(json: str) -> str:
+def pretty_json(string: str) -> str:
     """
     Return a pretty printed json string.
 
     Parameters
     ----------
     json : str
         The json string.
 
     Returns
     -------
     str
         The pretty printed json string.
     """
-    return dumps(json, indent=2)
+    return json.dumps(string, indent=2)
 
 
 # def multipartify(
 #     data, parent_key=None, formatter: Optional[Callable] = None
 # ) -> dict:
 #     if formatter is None:
 
@@ -229,24 +300,38 @@
             for key, value in call["multipart"].items():
                 call["files"][key] = value
 
     # Add data or files
     if call["files"]:
         data["files"] = call["files"]
         del data["headers"]["Content-Type"]
-    elif call["data"] is not None:
-        data["data"] = dumps(call["data"])
 
     # Add timeout
     if call["timeout"]:
         data["timeout"] = call["timeout"]
 
     # Add verify
     data["verify"] = call["verify"]
 
+    # Add body
+    if call["body"] and "data" in call["body"]:
+        # Default body type
+        if "type" not in call["body"] or not call["body"]["type"]:
+            call["body"]["type"] = BodyType.TEXT_PLAIN
+        else:
+            call["body"]["type"] = BodyType(call["body"]["type"])  # type: ignore
+
+        # Add body
+        if call["body"]["type"] == BodyType.APPLICATION_JSON:
+            data["json"] = call["body"]["data"]
+        elif call["body"]["type"] == BodyType.TEXT_PLAIN:
+            data["data"] = call["body"]["data"]
+        else:
+            raise ValueError("Body type not supported.")
+
     # url: str | bytes,
     # params: _Params | None = None,
     # *,
     # data: _Data | None = ...,
     # headers: _HeadersMapping | None = ...,
     # cookies: RequestsCookieJar | _TextMapping | None = ...,
     # files: _Files | None = ...,
@@ -268,16 +353,16 @@
         response = put(url, timeout=10, **data)
     elif call["method"] == Method.DELETE:
         response = delete(url, timeout=10, **data)
 
     info(f"Response Status: {response.status_code}")
     if call["hide_logs"] is False:
         try:
-            info(f"Response:\n{dumps(response.json(), indent=2)}")
-        except JSONDecodeError:
+            info(f"Response:\n{json.dumps(response.json(), indent=2)}")
+        except json.JSONDecodeError:
             info(f'Response: "{response.text}"')
 
     assert response.status_code in call["status_codes"]
 
     # Compare the response
     if call["assertion"] is not None:
         if isinstance(call["assertion"]["value"], str):
@@ -394,15 +479,16 @@
                     file["media"],
                 )
             else:
                 raise ValueError("File is not a dict.")
     # Multipart
     if call["multipart"] is not None:
         for key, part in call["multipart"].items():
-            call["multipart"][key] = (None, dumps(part), "application/json")
+            call["multipart"][key] = (
+                None, json.dumps(part), "application/json")
 
     # Payload
     # if call['payload'] is not None:
     #     call["payload"] = multipartify(call["payload"])
 
     # Timeout
     if not isinstance(call["timeout"], int):
```

### Comparing `universal-test-tool-0.1.8/test_tool_run_process_plugin/main.py` & `universal-test-tool-0.1.9/test_tool_run_process_plugin/main.py`

 * *Files identical despite different names*

### Comparing `universal-test-tool-0.1.8/test_tool_selenium_plugin/main.py` & `universal-test-tool-0.1.9/test_tool_selenium_plugin/main.py`

 * *Files identical despite different names*

### Comparing `universal-test-tool-0.1.8/test_tool_sql_plus_plugin/main.py` & `universal-test-tool-0.1.9/test_tool_sql_plus_plugin/main.py`

 * *Files identical despite different names*

### Comparing `universal-test-tool-0.1.8/test_tool_ssh_cmd_plugin/main.py` & `universal-test-tool-0.1.9/test_tool_ssh_cmd_plugin/main.py`

 * *Files identical despite different names*

### Comparing `universal-test-tool-0.1.8/universal_test_tool.egg-info/PKG-INFO` & `universal-test-tool-0.1.9/universal_test_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: universal-test-tool
-Version: 0.1.8
+Version: 0.1.9
 Summary: Awesome universal-test-tool to make tests configurable with a yaml file.
 Home-page: https://github.com/jackovsky8/universal-test-tool/
 Author: jackovsky8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: types-PyYAML
 Requires-Dist: python-dotenv
```

### Comparing `universal-test-tool-0.1.8/universal_test_tool.egg-info/SOURCES.txt` & `universal-test-tool-0.1.9/universal_test_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `universal-test-tool-0.1.8/universal_test_tool.egg-info/entry_points.txt` & `universal-test-tool-0.1.9/universal_test_tool.egg-info/entry_points.txt`

 * *Files identical despite different names*

