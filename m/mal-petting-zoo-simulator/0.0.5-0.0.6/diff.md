# Comparing `tmp/mal-petting-zoo-simulator-0.0.5.tar.gz` & `tmp/mal-petting-zoo-simulator-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mal-petting-zoo-simulator-0.0.5.tar", last modified: Fri Mar  1 11:12:36 2024, max compression
+gzip compressed data, was "mal-petting-zoo-simulator-0.0.6.tar", last modified: Fri Mar  1 11:22:30 2024, max compression
```

## Comparing `mal-petting-zoo-simulator-0.0.5.tar` & `mal-petting-zoo-simulator-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 11:12:36.960508 mal-petting-zoo-simulator-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-01 11:12:32.000000 mal-petting-zoo-simulator-0.0.5/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-01 11:12:32.000000 mal-petting-zoo-simulator-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-03-01 11:12:36.960508 mal-petting-zoo-simulator-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-01 11:12:32.000000 mal-petting-zoo-simulator-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 11:12:36.960508 mal-petting-zoo-simulator-0.0.5/mal_petting_zoo_simulator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-03-01 11:12:36.000000 mal-petting-zoo-simulator-0.0.5/mal_petting_zoo_simulator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-01 11:12:36.000000 mal-petting-zoo-simulator-0.0.5/mal_petting_zoo_simulator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 11:12:36.000000 mal-petting-zoo-simulator-0.0.5/mal_petting_zoo_simulator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-01 11:12:36.000000 mal-petting-zoo-simulator-0.0.5/mal_petting_zoo_simulator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-01 11:12:36.000000 mal-petting-zoo-simulator-0.0.5/mal_petting_zoo_simulator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 11:12:36.960508 mal-petting-zoo-simulator-0.0.5/malpzsim/
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-01 11:12:32.000000 mal-petting-zoo-simulator-0.0.5/malpzsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 11:12:36.960508 mal-petting-zoo-simulator-0.0.5/malpzsim/agents/
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-03-01 11:12:32.000000 mal-petting-zoo-simulator-0.0.5/malpzsim/agents/keyboard_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-03-01 11:12:32.000000 mal-petting-zoo-simulator-0.0.5/malpzsim/agents/searchers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 11:12:36.960508 mal-petting-zoo-simulator-0.0.5/malpzsim/sims/
--rw-r--r--   0 runner    (1001) docker     (127)    22749 2024-03-01 11:12:32.000000 mal-petting-zoo-simulator-0.0.5/malpzsim/sims/mal_petting_zoo_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 11:12:36.960508 mal-petting-zoo-simulator-0.0.5/malpzsim/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-03-01 11:12:32.000000 mal-petting-zoo-simulator-0.0.5/malpzsim/wrappers/gym_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-03-01 11:12:32.000000 mal-petting-zoo-simulator-0.0.5/malpzsim/wrappers/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-03-01 11:12:32.000000 mal-petting-zoo-simulator-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 11:12:36.960508 mal-petting-zoo-simulator-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 11:22:30.680621 mal-petting-zoo-simulator-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-01 11:22:25.000000 mal-petting-zoo-simulator-0.0.6/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-01 11:22:25.000000 mal-petting-zoo-simulator-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-03-01 11:22:30.680621 mal-petting-zoo-simulator-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-01 11:22:25.000000 mal-petting-zoo-simulator-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 11:22:30.680621 mal-petting-zoo-simulator-0.0.6/mal_petting_zoo_simulator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-03-01 11:22:30.000000 mal-petting-zoo-simulator-0.0.6/mal_petting_zoo_simulator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-01 11:22:30.000000 mal-petting-zoo-simulator-0.0.6/mal_petting_zoo_simulator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 11:22:30.000000 mal-petting-zoo-simulator-0.0.6/mal_petting_zoo_simulator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-01 11:22:30.000000 mal-petting-zoo-simulator-0.0.6/mal_petting_zoo_simulator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-01 11:22:30.000000 mal-petting-zoo-simulator-0.0.6/mal_petting_zoo_simulator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 11:22:30.680621 mal-petting-zoo-simulator-0.0.6/malpzsim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-01 11:22:25.000000 mal-petting-zoo-simulator-0.0.6/malpzsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 11:22:30.680621 mal-petting-zoo-simulator-0.0.6/malpzsim/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-03-01 11:22:25.000000 mal-petting-zoo-simulator-0.0.6/malpzsim/agents/keyboard_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-03-01 11:22:25.000000 mal-petting-zoo-simulator-0.0.6/malpzsim/agents/searchers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 11:22:30.680621 mal-petting-zoo-simulator-0.0.6/malpzsim/sims/
+-rw-r--r--   0 runner    (1001) docker     (127)    22749 2024-03-01 11:22:25.000000 mal-petting-zoo-simulator-0.0.6/malpzsim/sims/mal_petting_zoo_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 11:22:30.680621 mal-petting-zoo-simulator-0.0.6/malpzsim/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-03-01 11:22:25.000000 mal-petting-zoo-simulator-0.0.6/malpzsim/wrappers/gym_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-03-01 11:22:25.000000 mal-petting-zoo-simulator-0.0.6/malpzsim/wrappers/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-03-01 11:22:25.000000 mal-petting-zoo-simulator-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 11:22:30.680621 mal-petting-zoo-simulator-0.0.6/setup.cfg
```

### Comparing `mal-petting-zoo-simulator-0.0.5/LICENSE` & `mal-petting-zoo-simulator-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mal-petting-zoo-simulator-0.0.5/PKG-INFO` & `mal-petting-zoo-simulator-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mal-petting-zoo-simulator
-Version: 0.0.5
+Version: 0.0.6
 Summary: A MAL compliant petting zoo simulator.
 Author-email: Andrei Buhaiu <buhaiu@kth.se>, Jakob Nyberg <jaknyb@kth.se>
 License: Apache Software License
 Project-URL: Homepage, https://github.com/mal-lang/mal-petting-zoo-simulator
 Project-URL: Bug Tracker, https://github.com/mal-lang/mal-petting-zoo-simulator/issues
 Project-URL: Repository, https://github.com/mal-lang/mal-petting-zoo-simulator
 Keywords: mal
```

### Comparing `mal-petting-zoo-simulator-0.0.5/mal_petting_zoo_simulator.egg-info/PKG-INFO` & `mal-petting-zoo-simulator-0.0.6/mal_petting_zoo_simulator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mal-petting-zoo-simulator
-Version: 0.0.5
+Version: 0.0.6
 Summary: A MAL compliant petting zoo simulator.
 Author-email: Andrei Buhaiu <buhaiu@kth.se>, Jakob Nyberg <jaknyb@kth.se>
 License: Apache Software License
 Project-URL: Homepage, https://github.com/mal-lang/mal-petting-zoo-simulator
 Project-URL: Bug Tracker, https://github.com/mal-lang/mal-petting-zoo-simulator/issues
 Project-URL: Repository, https://github.com/mal-lang/mal-petting-zoo-simulator
 Keywords: mal
```

### Comparing `mal-petting-zoo-simulator-0.0.5/malpzsim/__init__.py` & `mal-petting-zoo-simulator-0.0.6/malpzsim/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- encoding: utf-8 -*-
-# MAL Petting Zoo Simulator v0.0.5
+# MAL Petting Zoo Simulator v0.0.6
 # Copyright 2024, Andrei Buhaiu.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
@@ -18,15 +18,15 @@
 from malpzsim.wrappers.wrapper import LazyWrapper
 from malpzsim.wrappers.gym_wrapper import AttackerEnv, DefenderEnv
 """
 MAL Petting Zoo Simulator
 """
 
 __title__ = 'malpzsim'
-__version__ = '0.0.5'
+__version__ = '0.0.6'
 __authors__ = ['Andrei Buhaiu',
     'Jakob Nyberg']
 __license__ = 'Apache 2.0'
 __docformat__ = 'restructuredtext en'
 
 __all__ = ('LazyWrapper', 'AttackerEnv', 'DefenderEnv')
```

### Comparing `mal-petting-zoo-simulator-0.0.5/malpzsim/agents/keyboard_input.py` & `mal-petting-zoo-simulator-0.0.6/malpzsim/agents/keyboard_input.py`

 * *Files identical despite different names*

### Comparing `mal-petting-zoo-simulator-0.0.5/malpzsim/agents/searchers.py` & `mal-petting-zoo-simulator-0.0.6/malpzsim/agents/searchers.py`

 * *Files identical despite different names*

### Comparing `mal-petting-zoo-simulator-0.0.5/malpzsim/sims/mal_petting_zoo_simulator.py` & `mal-petting-zoo-simulator-0.0.6/malpzsim/sims/mal_petting_zoo_simulator.py`

 * *Files identical despite different names*

### Comparing `mal-petting-zoo-simulator-0.0.5/malpzsim/wrappers/gym_wrapper.py` & `mal-petting-zoo-simulator-0.0.6/malpzsim/wrappers/gym_wrapper.py`

 * *Files identical despite different names*

### Comparing `mal-petting-zoo-simulator-0.0.5/malpzsim/wrappers/wrapper.py` & `mal-petting-zoo-simulator-0.0.6/malpzsim/wrappers/wrapper.py`

 * *Files identical despite different names*

### Comparing `mal-petting-zoo-simulator-0.0.5/pyproject.toml` & `mal-petting-zoo-simulator-0.0.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mal-petting-zoo-simulator"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Andrei Buhaiu", email="buhaiu@kth.se" },
   { name="Jakob Nyberg", email="jaknyb@kth.se"}
 ]
 description = "A MAL compliant petting zoo simulator."
 readme = "README.md"
 requires-python = ">=3.10"
```

