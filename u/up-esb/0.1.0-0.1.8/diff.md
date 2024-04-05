# Comparing `tmp/up_esb-0.1.0.tar.gz` & `tmp/up_esb-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "up_esb-0.1.0.tar", last modified: Thu Nov 30 09:44:41 2023, max compression
+gzip compressed data, was "up_esb-0.1.8.tar", last modified: Fri Apr  5 17:53:40 2024, max compression
```

## Comparing `up_esb-0.1.0.tar` & `up_esb-0.1.8.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 09:44:41.733435 up_esb-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 09:44:41.725436 up_esb-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 09:44:41.725436 up_esb-0.1.0/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2023-11-30 09:44:28.000000 up_esb-0.1.0/.github/scripts/update_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 09:44:41.725436 up_esb-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2023-11-30 09:44:28.000000 up_esb-0.1.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2023-11-30 09:44:28.000000 up_esb-0.1.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2023-11-30 09:44:28.000000 up_esb-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2023-11-30 09:44:28.000000 up_esb-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-30 09:44:28.000000 up_esb-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2023-11-30 09:44:41.733435 up_esb-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2023-11-30 09:44:28.000000 up_esb-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 09:44:41.725436 up_esb-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2023-11-30 09:44:28.000000 up_esb-0.1.0/docs/callable_interface.md
--rw-r--r--   0 runner    (1001) docker     (127)    37750 2023-11-30 09:44:28.000000 up_esb-0.1.0/docs/create_action_interface.drawio.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 09:44:41.729436 up_esb-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     5326 2023-11-30 09:44:28.000000 up_esb-0.1.0/examples/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2023-11-30 09:44:28.000000 up_esb-0.1.0/examples/partialorderplan.py
--rw-r--r--   0 runner    (1001) docker     (127)     8120 2023-11-30 09:44:28.000000 up_esb-0.1.0/examples/robot_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2023-11-30 09:44:28.000000 up_esb-0.1.0/examples/sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2023-11-30 09:44:28.000000 up_esb-0.1.0/examples/time_triggered.py
--rw-r--r--   0 runner    (1001) docker     (127)    16382 2023-11-30 09:44:28.000000 up_esb-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-30 09:44:41.733435 up_esb-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      127 2023-11-30 09:44:28.000000 up_esb-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 09:44:41.729436 up_esb-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2023-11-30 09:44:28.000000 up_esb-0.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 09:44:41.729436 up_esb-0.1.0/tests/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 09:44:28.000000 up_esb-0.1.0/tests/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5573 2023-11-30 09:44:28.000000 up_esb-0.1.0/tests/components/test_expression_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 09:44:41.729436 up_esb-0.1.0/tests/execution/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 09:44:28.000000 up_esb-0.1.0/tests/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2023-11-30 09:44:28.000000 up_esb-0.1.0/tests/execution/test_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 09:44:41.729436 up_esb-0.1.0/tests/plexmo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 09:44:28.000000 up_esb-0.1.0/tests/plexmo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2023-11-30 09:44:28.000000 up_esb-0.1.0/tests/plexmo/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2023-11-30 09:44:28.000000 up_esb-0.1.0/tests/plexmo/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    23631 2023-11-30 09:44:28.000000 up_esb-0.1.0/tests/test_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     8911 2023-11-30 09:44:28.000000 up_esb-0.1.0/tests/test_create_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2023-11-30 09:44:28.000000 up_esb-0.1.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8512 2023-11-30 09:44:28.000000 up_esb-0.1.0/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-11-30 09:44:28.000000 up_esb-0.1.0/tests/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 09:44:41.729436 up_esb-0.1.0/up_esb/
--rw-r--r--   0 runner    (1001) docker     (127)      687 2023-11-30 09:44:28.000000 up_esb-0.1.0/up_esb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20047 2023-11-30 09:44:28.000000 up_esb-0.1.0/up_esb/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 09:44:41.733435 up_esb-0.1.0/up_esb/components/
--rw-r--r--   0 runner    (1001) docker     (127)      804 2023-11-30 09:44:28.000000 up_esb-0.1.0/up_esb/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2023-11-30 09:44:28.000000 up_esb-0.1.0/up_esb/components/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4769 2023-11-30 09:44:28.000000 up_esb-0.1.0/up_esb/components/expression_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     8746 2023-11-30 09:44:28.000000 up_esb-0.1.0/up_esb/components/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2023-11-30 09:44:28.000000 up_esb-0.1.0/up_esb/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 09:44:41.733435 up_esb-0.1.0/up_esb/execution/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2023-11-30 09:44:28.000000 up_esb-0.1.0/up_esb/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12061 2023-11-30 09:44:28.000000 up_esb-0.1.0/up_esb/execution/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2023-11-30 09:44:28.000000 up_esb-0.1.0/up_esb/execution/parallel_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2023-11-30 09:44:28.000000 up_esb-0.1.0/up_esb/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 09:44:41.733435 up_esb-0.1.0/up_esb/plexmo/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2023-11-30 09:44:28.000000 up_esb-0.1.0/up_esb/plexmo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8272 2023-11-30 09:44:28.000000 up_esb-0.1.0/up_esb/plexmo/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2023-11-30 09:44:28.000000 up_esb-0.1.0/up_esb/plexmo/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2023-11-30 09:44:28.000000 up_esb-0.1.0/up_esb/status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 09:44:41.733435 up_esb-0.1.0/up_esb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2023-11-30 09:44:41.000000 up_esb-0.1.0/up_esb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2023-11-30 09:44:41.000000 up_esb-0.1.0/up_esb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-30 09:44:41.000000 up_esb-0.1.0/up_esb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-11-30 09:44:41.000000 up_esb-0.1.0/up_esb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-30 09:44:41.000000 up_esb-0.1.0/up_esb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:40.006049 up_esb-0.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:39.994049 up_esb-0.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:39.998049 up_esb-0.1.8/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-05 17:53:29.000000 up_esb-0.1.8/.github/scripts/update_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:39.998049 up_esb-0.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-05 17:53:29.000000 up_esb-0.1.8/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-05 17:53:29.000000 up_esb-0.1.8/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-05 17:53:29.000000 up_esb-0.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-05 17:53:29.000000 up_esb-0.1.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 17:53:29.000000 up_esb-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-05 17:53:40.006049 up_esb-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-05 17:53:29.000000 up_esb-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:39.998049 up_esb-0.1.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-05 17:53:29.000000 up_esb-0.1.8/docs/callable_interface.md
+-rw-r--r--   0 runner    (1001) docker     (127)    37750 2024-04-05 17:53:29.000000 up_esb-0.1.8/docs/create_action_interface.drawio.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:39.998049 up_esb-0.1.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-04-05 17:53:29.000000 up_esb-0.1.8/examples/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-04-05 17:53:29.000000 up_esb-0.1.8/examples/partialorderplan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-04-05 17:53:29.000000 up_esb-0.1.8/examples/robot_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-05 17:53:29.000000 up_esb-0.1.8/examples/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-04-05 17:53:29.000000 up_esb-0.1.8/examples/time_triggered.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16382 2024-04-05 17:53:29.000000 up_esb-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 17:53:40.006049 up_esb-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-05 17:53:29.000000 up_esb-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:39.998049 up_esb-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-04-05 17:53:29.000000 up_esb-0.1.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:39.998049 up_esb-0.1.8/tests/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:29.000000 up_esb-0.1.8/tests/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-04-05 17:53:29.000000 up_esb-0.1.8/tests/components/test_expression_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:40.002049 up_esb-0.1.8/tests/execution/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:29.000000 up_esb-0.1.8/tests/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-05 17:53:29.000000 up_esb-0.1.8/tests/execution/test_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:40.002049 up_esb-0.1.8/tests/plexmo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:29.000000 up_esb-0.1.8/tests/plexmo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-05 17:53:29.000000 up_esb-0.1.8/tests/plexmo/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-05 17:53:29.000000 up_esb-0.1.8/tests/plexmo/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23631 2024-04-05 17:53:29.000000 up_esb-0.1.8/tests/test_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-04-05 17:53:29.000000 up_esb-0.1.8/tests/test_create_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-04-05 17:53:29.000000 up_esb-0.1.8/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9054 2024-04-05 17:53:29.000000 up_esb-0.1.8/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-05 17:53:29.000000 up_esb-0.1.8/tests/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:40.002049 up_esb-0.1.8/up_esb/
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-05 17:53:29.000000 up_esb-0.1.8/up_esb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20284 2024-04-05 17:53:29.000000 up_esb-0.1.8/up_esb/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:40.002049 up_esb-0.1.8/up_esb/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-05 17:53:29.000000 up_esb-0.1.8/up_esb/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-05 17:53:29.000000 up_esb-0.1.8/up_esb/components/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-04-05 17:53:29.000000 up_esb-0.1.8/up_esb/components/expression_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8892 2024-04-05 17:53:29.000000 up_esb-0.1.8/up_esb/components/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-05 17:53:29.000000 up_esb-0.1.8/up_esb/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:40.002049 up_esb-0.1.8/up_esb/execution/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-05 17:53:29.000000 up_esb-0.1.8/up_esb/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12062 2024-04-05 17:53:29.000000 up_esb-0.1.8/up_esb/execution/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-05 17:53:29.000000 up_esb-0.1.8/up_esb/execution/parallel_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-05 17:53:29.000000 up_esb-0.1.8/up_esb/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:40.002049 up_esb-0.1.8/up_esb/plexmo/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-05 17:53:29.000000 up_esb-0.1.8/up_esb/plexmo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-04-05 17:53:29.000000 up_esb-0.1.8/up_esb/plexmo/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-05 17:53:29.000000 up_esb-0.1.8/up_esb/plexmo/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-05 17:53:29.000000 up_esb-0.1.8/up_esb/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:53:40.006049 up_esb-0.1.8/up_esb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-05 17:53:39.000000 up_esb-0.1.8/up_esb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-05 17:53:39.000000 up_esb-0.1.8/up_esb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:53:39.000000 up_esb-0.1.8/up_esb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-05 17:53:39.000000 up_esb-0.1.8/up_esb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 17:53:39.000000 up_esb-0.1.8/up_esb.egg-info/top_level.txt
```

### Comparing `up_esb-0.1.0/.github/scripts/update_version.py` & `up_esb-0.1.8/.github/scripts/update_version.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/.github/workflows/deploy.yml` & `up_esb-0.1.8/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/.gitignore` & `up_esb-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/.pre-commit-config.yaml` & `up_esb-0.1.8/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
       python: $(python3 --version | cut -d' ' -f2)
       pyproject_toml: ./pyproject.toml
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/psf/black
-    rev: 23.11.0
+    rev: 24.3.0
     hooks:
       - id: black
         args: [--config=pyproject.toml]
   - repo: https://github.com/pre-commit/mirrors-pylint
     rev: v3.0.0a5
     hooks:
       - id: pylint
@@ -22,19 +22,19 @@
             --rcfile=pyproject.toml,
             --fail-under=8.0,
             --jobs=0,
             --output-format=colorized,
             --disable=import-error,
           ]
   - repo: https://github.com/pycqa/isort
-    rev: 5.12.0
+    rev: 5.13.2
     hooks:
       - id: isort
         files: "\\.(py)$"
         args: [--settings-path=pyproject.toml]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: "v1.7.1" # Use the sha / tag you want to point at
+    rev: "v1.9.0" # Use the sha / tag you want to point at
     hooks:
       - id: mypy
         files: "up_esb/.*\\.py$"
         args: [--ignore-missing-imports]
```

### Comparing `up_esb-0.1.0/LICENSE` & `up_esb-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/PKG-INFO` & `up_esb-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: up_esb
-Version: 0.1.0
+Version: 0.1.8
 Summary: General functionalities for using unified-planning in robotic applications
 License: Apache-2.0 License
 Project-URL: Homepage, https://www.aiplan4eu-project.eu/
 Project-URL: Repository, https://github.com/aiplan4eu/embedded-systems-bridge
 Keywords: unified-planning,embedded-systems-bridge
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: unified-planning==1.0.0
+Requires-Dist: unified-planning>=1.0.0
 Requires-Dist: networkx
 Requires-Dist: matplotlib
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `up_esb-0.1.0/README.md` & `up_esb-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/docs/callable_interface.md` & `up_esb-0.1.8/docs/callable_interface.md`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/docs/create_action_interface.drawio.png` & `up_esb-0.1.8/docs/create_action_interface.drawio.png`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/examples/parallel.py` & `up_esb-0.1.8/examples/parallel.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/examples/partialorderplan.py` & `up_esb-0.1.8/examples/partialorderplan.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/examples/robot_example.py` & `up_esb-0.1.8/examples/robot_example.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/examples/sequential.py` & `up_esb-0.1.8/examples/sequential.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/examples/time_triggered.py` & `up_esb-0.1.8/examples/time_triggered.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/pyproject.toml` & `up_esb-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 requires = ["setuptools>=61.0.0", "setuptools-scm", "pip>=22.3"]
 
 [project]
 classifiers = [
   "Programming Language :: Python :: 3",
 ]
 dependencies = [
-  "unified-planning==1.0.0",
+  "unified-planning>=1.0.0",
   "networkx",
   "matplotlib",
 ]
 description = "General functionalities for using unified-planning in robotic applications"
 keywords = ["unified-planning", "embedded-systems-bridge"]
 license = {text = "Apache-2.0 License"}
 name = "up_esb"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.1.0"
+version = "0.1.8"
 
 [project.urls]
 Homepage = "https://www.aiplan4eu-project.eu/"
 Repository = "https://github.com/aiplan4eu/embedded-systems-bridge"
 
 [project.optional-dependencies]
 dev = ["black", "mypy", "pylint", "pytest", "pre-commit"]
```

### Comparing `up_esb-0.1.0/tests/__init__.py` & `up_esb-0.1.8/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 def get_example_plans() -> Union[List[SequentialPlan], List[TimeTriggeredPlan]]:
     """Gain access to the example plans."""
     example_problems = get_example_problems()
 
     plans = {}
     for element in example_problems:
         if element in available_plans:
-            plans[element] = example_problems[element].plan
+            plans[element] = example_problems[element].valid_plans[-1]
 
     return plans
 
 
 class ContextManager:
     """Convert plan to executable functions for testing purposes."""
```

### Comparing `up_esb-0.1.0/tests/components/test_expression_manager.py` & `up_esb-0.1.8/tests/components/test_expression_manager.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/tests/execution/test_executor.py` & `up_esb-0.1.8/tests/execution/test_executor.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/tests/plexmo/test_dispatcher.py` & `up_esb-0.1.8/tests/plexmo/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/tests/plexmo/test_monitor.py` & `up_esb-0.1.8/tests/plexmo/test_monitor.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/tests/test_bridge.py` & `up_esb-0.1.8/tests/test_bridge.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/tests/test_create_action.py` & `up_esb-0.1.8/tests/test_create_action.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/tests/test_exceptions.py` & `up_esb-0.1.8/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/tests/test_graph.py` & `up_esb-0.1.8/tests/test_graph.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,49 +15,52 @@
 import unittest
 
 import unified_planning as up
 from unified_planning.plans import SequentialPlan, TimeTriggeredPlan
 from unified_planning.plans.partial_order_plan import PartialOrderPlan
 from unified_planning.shortcuts import *  # pylint: disable=unused-wildcard-import
 from unified_planning.test.examples import get_example_problems
-from unified_planning.test.examples.realistic import get_example_problems
 
 from up_esb.components.graph import plan_to_dependency_graph
 
 # pylint: disable=all
 
 
 class TestPartialOrderPlanGeneration(unittest.TestCase):
     def test_partial_order_plan_to_dependency_graph(self):
         example_problems = get_example_problems()
-        problem, plan = example_problems["robot_fluent_of_user_type"]
+        problem = example_problems["robot_fluent_of_user_type"].problem
+        plan = example_problems["robot_fluent_of_user_type"].valid_plans[-1]
         pop = plan.convert_to(PlanKind.PARTIAL_ORDER_PLAN, problem)
         assert isinstance(pop, PartialOrderPlan)
         dep_graph = plan_to_dependency_graph(pop)
 
         # Partial Orders are not ordered in the graph. Therefore, we can only check if all actions are in the graph
         actions = [str(action) for action in plan.actions] + ["start", "end"]
         for node in dep_graph.nodes(data=True):
             self.assertTrue(node[1]["node_name"] in actions)
 
 
 class TestSequentialPlanTranslation(unittest.TestCase):
     def test_simple_translation(self):
         problems = get_example_problems()
 
-        for _, plan in problems.values():
-            if isinstance(plan, SequentialPlan):
-                dep_graph = plan_to_dependency_graph(plan)
-                actions = ["start"] + [str(action) for action in plan.actions] + ["end"]
-                graph_actions = []
-                for node in dep_graph.nodes(data=True):
-                    graph_actions.append(node[1]["node_name"])
+        for test_case in problems.values():
+            if not test_case.valid_plans:
+                continue
+            for plan in test_case.valid_plans:
+                if isinstance(plan, SequentialPlan):
+                    dep_graph = plan_to_dependency_graph(plan)
+                    actions = ["start"] + [str(action) for action in plan.actions] + ["end"]
+                    graph_actions = []
+                    for node in dep_graph.nodes(data=True):
+                        graph_actions.append(node[1]["node_name"])
 
-                # Check if all actions are ordered correctly
-                self.assertEqual(actions, graph_actions)
+                    # Check if all actions are ordered correctly
+                    self.assertEqual(actions, graph_actions)
 
     def test_special_cases(self):
         """Test translation for special cases."""
         Location = UserType("Location")
         robot_at = Fluent("robot_at", BoolType(), position=Location)
         battery_charge = Fluent("battery_charge", RealType(0, 100))
         move = InstantaneousAction("move", l_from=Location, l_to=Location)
@@ -94,26 +97,35 @@
         self.test_special_cases()
 
 
 class TestTimeTriggeredPlanTrasnslation(unittest.TestCase):
     def test_simple_translation(self):
         problems = get_example_problems()
 
-        for _, plan in problems.values():
-            if isinstance(plan, TimeTriggeredPlan):
-                dep_graph = plan_to_dependency_graph(plan)
-                actions = ["start"] + [str(action) for _, action, _ in plan.timed_actions] + ["end"]
-                graph_actions = []
-                for node in dep_graph.nodes(data=True):
-                    node_name = node[1]["node_name"]
-                    if node_name not in ["start", "end"]:
-                        node_name = node[1]["node_name"].split(")")[0] + ")"
-                    graph_actions.append(node_name)
+        for test_case in problems.values():
+            if not test_case.valid_plans:
+                continue
+
+            for plan in test_case.valid_plans:
+                if isinstance(plan, TimeTriggeredPlan):
+                    dep_graph = plan_to_dependency_graph(plan)
+                    actions = (
+                        ["start"] + [str(action) for _, action, _ in plan.timed_actions] + ["end"]
+                    )
+                    graph_actions = []
+                    for node in dep_graph.nodes(data=True):
+                        node_name = node[1]["node_name"]
+                        if node_name not in ["start", "end"]:
+                            node_name = node[1]["node_name"].split(")")[0]
+                            # FIXME: This is a hack to remove the time from the action name
+                            if "(" in node_name:
+                                node_name += ")"
+                        graph_actions.append(node_name)
 
-                self.assertEqual(actions, graph_actions)
+                    self.assertEqual(actions, graph_actions)
 
     def test_special_cases(self):
         Location = UserType("Location")
         is_connected = Fluent("is_connected", BoolType(), location_1=Location, location_2=Location)
         is_at = Fluent("is_at", BoolType(), position=Location)
         dur_move = DurativeAction("move", l_from=Location, l_to=Location)
         l_from = dur_move.parameter("l_from")
```

### Comparing `up_esb-0.1.0/tests/test_logger.py` & `up_esb-0.1.8/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/up_esb/__init__.py` & `up_esb-0.1.8/up_esb/__init__.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/up_esb/bridge.py` & `up_esb-0.1.8/up_esb/bridge.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,19 +165,23 @@
          and no return type is given in signature.
         Optionally, provide a callable which calculates the fluent's values for problem
          initialization. Otherwise, you must set it later.
         """
         assert name not in self._fluents, f"Fluent {name} already exists!"
         self._fluents[name] = Fluent(
             name,
-            self.get_type(result_api_type)
-            if result_api_type
-            else self.get_type(signature["return"])
-            if signature and "return" in signature.keys()
-            else BoolType(),
+            (
+                self.get_type(result_api_type)
+                if result_api_type
+                else (
+                    self.get_type(signature["return"])
+                    if signature and "return" in signature.keys()
+                    else BoolType()
+                )
+            ),
             OrderedDict(
                 (parameter_name, self.get_type(api_type))
                 for parameter_name, api_type in (
                     dict(signature, **kwargs) if signature else kwargs
                 ).items()
                 if parameter_name != "return"
             ),
@@ -190,14 +194,16 @@
     def create_fluent_from_function(
         self, function: Callable[..., object], set_callable: bool = True
     ) -> Fluent:
         """
         Create UP fluent based on function, which calculates the fluent's values
          for problem initialization. If function is a class method and a corresponding UP
          representation exists for its defining class, implicitly use the later as first parameter.
+         The function's result type will be used for the fluent's type, or BoolType() by default
+         if no type annotation is provided.
         If set_callable is True, also set function as the fluent function's callable. Otherwise,
          you must set it later.
         """
         name, signature = self.get_name_and_signature(function)
         return self.create_fluent(
             name, signature=signature, _callable=function if set_callable else None
         )
```

### Comparing `up_esb-0.1.0/up_esb/components/__init__.py` & `up_esb-0.1.8/up_esb/components/__init__.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/up_esb/components/actions.py` & `up_esb-0.1.8/up_esb/components/actions.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/up_esb/components/expression_manager.py` & `up_esb-0.1.8/up_esb/components/expression_manager.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/up_esb/components/graph.py` & `up_esb-0.1.8/up_esb/components/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,17 +155,21 @@
         # TODO: Handle None Durations as Instantaneous Action Node
         if duration:
             duration = float(duration.numerator) / float(duration.denominator)
         else:
             duration = 0.0
         parameters, preconditions, postconditions = _process_action(action)
 
+        # TODO: Check this logic with respect to UP
+        node_name = f"{str(action)}({duration})"
+        if duration <= 1.0:
+            node_name = str(action)
         dependency_graph.add_node(
             child_id,
-            node_name=f"{str(action)}({duration})",
+            node_name=node_name,
             action=action.action.name,
             parameters=parameters,
             preconditions=preconditions,
             postconditions=postconditions,
         )
 
     dependency_graph.add_node(
```

### Comparing `up_esb-0.1.0/up_esb/exceptions.py` & `up_esb-0.1.8/up_esb/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Exceptions for the execution module"""
+
 from up_esb.execution import ActionResult
 from up_esb.status import ActionNodeStatus, ConditionStatus
 
 
 class UPESBException(Exception):
     """Raised when an exception occurs"""
```

### Comparing `up_esb-0.1.0/up_esb/execution/executor.py` & `up_esb-0.1.8/up_esb/execution/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Executor for executing tasks."""
+
 from threading import Condition, Lock, Thread
 from typing import NamedTuple
 
 import networkx as nx
 from unified_planning.plans import Plan, SequentialPlan, TimeTriggeredPlan
 from unified_planning.shortcuts import EndTiming, StartTiming, TimeInterval
```

### Comparing `up_esb-0.1.0/up_esb/execution/parallel_executor.py` & `up_esb-0.1.8/up_esb/execution/parallel_executor.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/up_esb/logger.py` & `up_esb-0.1.8/up_esb/logger.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/up_esb/plexmo/__init__.py` & `up_esb-0.1.8/up_esb/plexmo/__init__.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/up_esb/plexmo/dispatcher.py` & `up_esb-0.1.8/up_esb/plexmo/dispatcher.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/up_esb/plexmo/monitor.py` & `up_esb-0.1.8/up_esb/plexmo/monitor.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.1.0/up_esb/status.py` & `up_esb-0.1.8/up_esb/status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Status Enum for up_esb"""
+
 from enum import Enum, auto
 
 
 class ActionNodeStatus(Enum):
     """ActionNode Enum"""
 
     NOT_STARTED = auto()
```

### Comparing `up_esb-0.1.0/up_esb.egg-info/PKG-INFO` & `up_esb-0.1.8/up_esb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: up-esb
-Version: 0.1.0
+Name: up_esb
+Version: 0.1.8
 Summary: General functionalities for using unified-planning in robotic applications
 License: Apache-2.0 License
 Project-URL: Homepage, https://www.aiplan4eu-project.eu/
 Project-URL: Repository, https://github.com/aiplan4eu/embedded-systems-bridge
 Keywords: unified-planning,embedded-systems-bridge
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: unified-planning==1.0.0
+Requires-Dist: unified-planning>=1.0.0
 Requires-Dist: networkx
 Requires-Dist: matplotlib
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `up_esb-0.1.0/up_esb.egg-info/SOURCES.txt` & `up_esb-0.1.8/up_esb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

