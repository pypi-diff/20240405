# Comparing `tmp/gluepy-1.1.0.tar.gz` & `tmp/gluepy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gluepy-1.1.0.tar", last modified: Mon Apr  1 13:40:50 2024, max compression
+gzip compressed data, was "gluepy-1.1.1.tar", last modified: Fri Apr  5 15:12:20 2024, max compression
```

## Comparing `gluepy-1.1.0.tar` & `gluepy-1.1.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:40:50.892107 gluepy-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-01 13:40:42.000000 gluepy-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 13:40:42.000000 gluepy-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-01 13:40:50.892107 gluepy-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-01 13:40:42.000000 gluepy-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:40:50.884107 gluepy-1.1.0/gluepy/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:40:50.888107 gluepy-1.1.0/gluepy/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/bin/gluepy-cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:40:50.888107 gluepy-1.1.0/gluepy/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/commands/airflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/commands/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/commands/gluepy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/commands/startmodule.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/commands/startproject.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/commands/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:40:50.888107 gluepy-1.1.0/gluepy/conf/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/conf/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/conf/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:40:50.888107 gluepy-1.1.0/gluepy/exec/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/exec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/exec/boot.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/exec/dags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/exec/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:40:50.888107 gluepy-1.1.0/gluepy/files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:40:50.892107 gluepy-1.1.0/gluepy/files/data/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/files/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/files/data/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/files/data/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:40:50.892107 gluepy-1.1.0/gluepy/files/storages/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/files/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/files/storages/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/files/storages/google.py
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/files/storages/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/files/storages/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/files/storages/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:40:50.892107 gluepy-1.1.0/gluepy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/utils/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-01 13:40:42.000000 gluepy-1.1.0/gluepy/utils/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:40:50.892107 gluepy-1.1.0/gluepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-01 13:40:50.000000 gluepy-1.1.0/gluepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-01 13:40:50.000000 gluepy-1.1.0/gluepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 13:40:50.000000 gluepy-1.1.0/gluepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 13:40:50.000000 gluepy-1.1.0/gluepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-01 13:40:50.000000 gluepy-1.1.0/gluepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 13:40:50.000000 gluepy-1.1.0/gluepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 13:40:50.892107 gluepy-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-01 13:40:42.000000 gluepy-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:40:50.892107 gluepy-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-01 13:40:42.000000 gluepy-1.1.0/tests/test_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:12:20.050551 gluepy-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-05 15:12:08.000000 gluepy-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:12:08.000000 gluepy-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-05 15:12:20.046551 gluepy-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-05 15:12:08.000000 gluepy-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:12:20.042551 gluepy-1.1.1/gluepy/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:12:20.042551 gluepy-1.1.1/gluepy/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/bin/gluepy-cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:12:20.042551 gluepy-1.1.1/gluepy/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/commands/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/commands/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/commands/gluepy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/commands/startmodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/commands/startproject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/commands/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:12:20.046551 gluepy-1.1.1/gluepy/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/conf/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/conf/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:12:20.046551 gluepy-1.1.1/gluepy/exec/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/exec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/exec/boot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/exec/dags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/exec/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:12:20.046551 gluepy-1.1.1/gluepy/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:12:20.046551 gluepy-1.1.1/gluepy/files/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/files/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/files/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/files/data/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:12:20.046551 gluepy-1.1.1/gluepy/files/storages/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/files/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/files/storages/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/files/storages/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/files/storages/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/files/storages/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/files/storages/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:12:20.046551 gluepy-1.1.1/gluepy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-05 15:12:08.000000 gluepy-1.1.1/gluepy/utils/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:12:20.046551 gluepy-1.1.1/gluepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-05 15:12:19.000000 gluepy-1.1.1/gluepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-05 15:12:20.000000 gluepy-1.1.1/gluepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:12:19.000000 gluepy-1.1.1/gluepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 15:12:19.000000 gluepy-1.1.1/gluepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-05 15:12:19.000000 gluepy-1.1.1/gluepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 15:12:19.000000 gluepy-1.1.1/gluepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 15:12:20.050551 gluepy-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-05 15:12:08.000000 gluepy-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:12:20.046551 gluepy-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-05 15:12:08.000000 gluepy-1.1.1/tests/test_sample.py
```

### Comparing `gluepy-1.1.0/LICENSE` & `gluepy-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.0/PKG-INFO` & `gluepy-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gluepy
-Version: 1.1.0
+Version: 1.1.1
 Summary: A framework for data scientists
 Home-page: https://github.com/gluepy/gluepy
 Author: Marcus Lind
 Author-email: marcuslind90@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gluepy-1.1.0/gluepy/commands/airflow.py` & `gluepy-1.1.1/gluepy/commands/airflow.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.0/gluepy/commands/base.py` & `gluepy-1.1.1/gluepy/commands/base.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.0/gluepy/commands/dag.py` & `gluepy-1.1.1/gluepy/commands/dag.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import logging
 from typing import List, Optional
 import time
 import click
 from gluepy.conf import default_context_manager
+from gluepy.files.storages import default_storage
 from . import cli
 
 logger = logging.getLogger(__name__)
 
 
 @cli.command()
 @click.option("--task", type=str)
@@ -20,21 +21,27 @@
     retry: Optional[str] = None,
     patch: Optional[List[str]] = None,
     from_task: Optional[str] = None,
     task: Optional[str] = None,
 ):
     DAG = _get_dag_by_label(label)
     assert not (from_task and task), "Only one of --from-task or --task can be set."
+    retry = retry if retry is None else retry.strip(default_storage.separator)
 
-    if retry:
+    if retry and default_storage.exists(os.path.join(retry, "context.yaml")):
         default_context_manager.load_context(
             os.path.join(retry, "context.yaml"), patches=list(patch)
         )
+    elif retry:
+        # Retry a run folder path that does not exist by creating it.
+        default_context_manager.create_context(
+            run_id=os.path.basename(retry), run_folder=retry, evaluate_lazy=True
+        )
     elif patch:
-        default_context_manager.create_context(patches=list(patch))
+        default_context_manager.create_context(patches=list(patch), evaluate_lazy=True)
 
     tasks = DAG().inject_tasks()
 
     if task:
         tasks = [_get_task_by_label(task)]
 
     if from_task:
```

### Comparing `gluepy-1.1.0/gluepy/commands/gluepy.py` & `gluepy-1.1.1/gluepy/commands/gluepy.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.0/gluepy/commands/task.py` & `gluepy-1.1.1/gluepy/commands/task.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.0/gluepy/conf/context.py` & `gluepy-1.1.1/gluepy/conf/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         self._ctx = None
 
     def create_context(
         self,
         run_id: Optional[str] = None,
         run_folder: Optional[str] = None,
         patches: Optional[List[str]] = None,
+        evaluate_lazy: bool = False,
     ):
         # Imported here to avoid circular import.
         from gluepy.files.storages import default_storage
 
         patches = patches or []
         if patches:
             for i, path in enumerate(patches):
@@ -80,18 +81,22 @@
                 Loader=yaml.SafeLoader,
             )
             for y in yamls
         ] + patches
 
         patches += [self.get_run_meta(run_id=run_id, run_folder=run_folder)]
 
-        return Context(
+        ctx = Context(
             data=reduce(lambda config, patch: merge(config, patch), patches, {})
         )
 
+        if evaluate_lazy:
+            self._ctx = ctx
+        return ctx
+
     def load_context(self, path: str, patches: Optional[List[str]] = None):
         # Imported here to avoid circular import.
         from gluepy.files.storages import default_storage
 
         patches = patches or []
         # Reformat folder name to be valid.
         path_formatted = re.sub(r"[:\+\s]+", "-", os.path.dirname(path))
```

### Comparing `gluepy-1.1.0/gluepy/exec/dags.py` & `gluepy-1.1.1/gluepy/exec/dags.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.0/gluepy/exec/tasks.py` & `gluepy-1.1.1/gluepy/exec/tasks.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.0/gluepy/files/data/pandas.py` & `gluepy-1.1.1/gluepy/files/data/pandas.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.0/gluepy/files/storages/base.py` & `gluepy-1.1.1/gluepy/files/storages/base.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.0/gluepy/files/storages/google.py` & `gluepy-1.1.1/gluepy/files/storages/google.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,15 @@
 
         Returns:
             bool: True/False if path is directory or not
         """
         # Ensure always ending with `/`.
         path = self.abspath(path).rstrip(self.separator) + self.separator
         return self.bucket.blob(path).exists() or bool(
-            self.client.list_blobs(self.bucket, prefix=path, max_results=1)
+            list(self.client.list_blobs(self.bucket, prefix=path, max_results=1))
         )
 
     def isfile(self, path: str) -> bool:
         """Check if path is a file or not.
 
         Args:
             path (str): Path we want to check
```

### Comparing `gluepy-1.1.0/gluepy/files/storages/local.py` & `gluepy-1.1.1/gluepy/files/storages/local.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.0/gluepy/files/storages/s3.py` & `gluepy-1.1.1/gluepy/files/storages/s3.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.0/gluepy/utils/dict.py` & `gluepy-1.1.1/gluepy/utils/dict.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.0/gluepy/utils/loading.py` & `gluepy-1.1.1/gluepy/utils/loading.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.0/gluepy.egg-info/PKG-INFO` & `gluepy-1.1.1/gluepy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gluepy
-Version: 1.1.0
+Version: 1.1.1
 Summary: A framework for data scientists
 Home-page: https://github.com/gluepy/gluepy
 Author: Marcus Lind
 Author-email: marcuslind90@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gluepy-1.1.0/gluepy.egg-info/SOURCES.txt` & `gluepy-1.1.1/gluepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.0/setup.py` & `gluepy-1.1.1/setup.py`

 * *Files identical despite different names*

