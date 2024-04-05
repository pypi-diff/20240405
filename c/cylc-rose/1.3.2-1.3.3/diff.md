# Comparing `tmp/cylc-rose-1.3.2.tar.gz` & `tmp/cylc-rose-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cylc-rose-1.3.2.tar", last modified: Fri Jan 19 10:11:53 2024, max compression
+gzip compressed data, was "cylc-rose-1.3.3.tar", last modified: Fri Apr  5 14:59:53 2024, max compression
```

## Comparing `cylc-rose-1.3.2.tar` & `cylc-rose-1.3.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 10:11:53.845994 cylc-rose-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-01-19 10:11:49.000000 cylc-rose-1.3.2/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-01-19 10:11:53.845994 cylc-rose-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-01-19 10:11:49.000000 cylc-rose-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 10:11:53.841994 cylc-rose-1.3.2/cylc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 10:11:53.845994 cylc-rose-1.3.2/cylc/rose/
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-01-19 10:11:49.000000 cylc-rose-1.3.2/cylc/rose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-01-19 10:11:49.000000 cylc-rose-1.3.2/cylc/rose/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     9764 2024-01-19 10:11:49.000000 cylc-rose-1.3.2/cylc/rose/jinja2_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-01-19 10:11:49.000000 cylc-rose-1.3.2/cylc/rose/platform_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21197 2024-01-19 10:11:49.000000 cylc-rose-1.3.2/cylc/rose/stem.py
--rw-r--r--   0 runner    (1001) docker     (127)    27151 2024-01-19 10:11:49.000000 cylc-rose-1.3.2/cylc/rose/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 10:11:53.845994 cylc-rose-1.3.2/cylc_rose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-01-19 10:11:53.000000 cylc-rose-1.3.2/cylc_rose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-01-19 10:11:53.000000 cylc-rose-1.3.2/cylc_rose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 10:11:53.000000 cylc-rose-1.3.2/cylc_rose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-01-19 10:11:53.000000 cylc-rose-1.3.2/cylc_rose.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-01-19 10:11:53.000000 cylc-rose-1.3.2/cylc_rose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-19 10:11:53.000000 cylc-rose-1.3.2/cylc_rose.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-01-19 10:11:53.845994 cylc-rose-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-01-19 10:11:49.000000 cylc-rose-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:59:53.801746 cylc-rose-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-05 14:59:50.000000 cylc-rose-1.3.3/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-04-05 14:59:53.801746 cylc-rose-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-05 14:59:50.000000 cylc-rose-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:59:53.801746 cylc-rose-1.3.3/cylc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:59:53.801746 cylc-rose-1.3.3/cylc/rose/
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-04-05 14:59:50.000000 cylc-rose-1.3.3/cylc/rose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-04-05 14:59:50.000000 cylc-rose-1.3.3/cylc/rose/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9764 2024-04-05 14:59:50.000000 cylc-rose-1.3.3/cylc/rose/jinja2_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-04-05 14:59:50.000000 cylc-rose-1.3.3/cylc/rose/platform_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21197 2024-04-05 14:59:50.000000 cylc-rose-1.3.3/cylc/rose/stem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27151 2024-04-05 14:59:50.000000 cylc-rose-1.3.3/cylc/rose/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:59:53.801746 cylc-rose-1.3.3/cylc_rose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-04-05 14:59:53.000000 cylc-rose-1.3.3/cylc_rose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-05 14:59:53.000000 cylc-rose-1.3.3/cylc_rose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:59:53.000000 cylc-rose-1.3.3/cylc_rose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-05 14:59:53.000000 cylc-rose-1.3.3/cylc_rose.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-05 14:59:53.000000 cylc-rose-1.3.3/cylc_rose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-05 14:59:53.000000 cylc-rose-1.3.3/cylc_rose.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-05 14:59:53.805746 cylc-rose-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-05 14:59:50.000000 cylc-rose-1.3.3/setup.py
```

### Comparing `cylc-rose-1.3.2/COPYING` & `cylc-rose-1.3.3/COPYING`

 * *Files identical despite different names*

### Comparing `cylc-rose-1.3.2/PKG-INFO` & `cylc-rose-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cylc-rose
-Version: 1.3.2
+Version: 1.3.3
 Summary: A Cylc plugin providing support for the Rose rose-suite.conf file.
 Home-page: https://cylc.github.io/cylc-doc/latest/html/plugins/cylc-rose.html
 Author: British Crown (Met Office) & Contributors
 Author-email: metomi@metoffice.gov.uk
 License: GPL
 Keywords: cylc,rose,workflow,configuration,workflow-engine,workflow-automation,workflow-management
 Platform: any
```

### Comparing `cylc-rose-1.3.2/README.md` & `cylc-rose-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `cylc-rose-1.3.2/cylc/rose/__init__.py` & `cylc-rose-1.3.3/cylc/rose/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,8 +201,8 @@
    To reinstall a rose stem suite use ``cylc reinstall``.  Cylc can get any
    options you do not change from the ``rose-suite-cylc-install.conf``` file.
    Using ``rose stem`` a second time will attempt install a new copy
    of your rose stem suite.
 
 """
 
-__version__ = '1.3.2'
+__version__ = '1.3.3'
```

### Comparing `cylc-rose-1.3.2/cylc/rose/entry_points.py` & `cylc-rose-1.3.3/cylc/rose/entry_points.py`

 * *Files identical despite different names*

### Comparing `cylc-rose-1.3.2/cylc/rose/jinja2_parser.py` & `cylc-rose-1.3.3/cylc/rose/jinja2_parser.py`

 * *Files identical despite different names*

### Comparing `cylc-rose-1.3.2/cylc/rose/platform_utils.py` & `cylc-rose-1.3.3/cylc/rose/platform_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,19 @@
 from optparse import Values
 import sqlite3
 from time import sleep
 from typing import Any, Dict
 
 from cylc.flow.config import WorkflowConfig
 from cylc.flow.id_cli import parse_id
-from cylc.flow.pathutil import get_workflow_run_pub_db_path
+from cylc.flow.pathutil import (
+    get_workflow_run_config_log_dir,
+    get_workflow_run_pub_db_path,
+)
+from cylc.flow.workflow_files import WorkflowFiles
 from cylc.flow.platforms import (
     HOST_REC_COMMAND,
     get_platform,
     is_platform_definition_subshell
 )
 from cylc.flow.rundb import CylcWorkflowDAO
 
@@ -43,15 +47,19 @@
     Args:
         flow: The name of the Cylc flow to be queried.
         task: The name of the task to be queried.
 
     Returns:
         Platform Dictionary.
     """
-    _, _, flow_file = parse_id(flow, constraint='workflows', src=True)
+    workflow_id, _, _ = parse_id(flow, constraint='workflows', src=True)
+    flow_file = get_workflow_run_config_log_dir(
+        workflow_id,
+        WorkflowFiles.FLOW_FILE_PROCESSED,
+    )
     config = WorkflowConfig(flow, flow_file, Values())
     # Get entire task spec to allow Cylc 7 platform from host guessing.
     task_spec = config.pcfg.get(['runtime', task])
     # check for subshell and evaluate
     if (
         task_spec.get('platform')
         and is_platform_definition_subshell(task_spec['platform'])
```

### Comparing `cylc-rose-1.3.2/cylc/rose/stem.py` & `cylc-rose-1.3.3/cylc/rose/stem.py`

 * *Files identical despite different names*

### Comparing `cylc-rose-1.3.2/cylc/rose/utilities.py` & `cylc-rose-1.3.3/cylc/rose/utilities.py`

 * *Files identical despite different names*

### Comparing `cylc-rose-1.3.2/cylc_rose.egg-info/PKG-INFO` & `cylc-rose-1.3.3/cylc_rose.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cylc-rose
-Version: 1.3.2
+Version: 1.3.3
 Summary: A Cylc plugin providing support for the Rose rose-suite.conf file.
 Home-page: https://cylc.github.io/cylc-doc/latest/html/plugins/cylc-rose.html
 Author: British Crown (Met Office) & Contributors
 Author-email: metomi@metoffice.gov.uk
 License: GPL
 Keywords: cylc,rose,workflow,configuration,workflow-engine,workflow-automation,workflow-management
 Platform: any
```

### Comparing `cylc-rose-1.3.2/cylc_rose.egg-info/requires.txt` & `cylc-rose-1.3.3/cylc_rose.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `cylc-rose-1.3.2/setup.cfg` & `cylc-rose-1.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `cylc-rose-1.3.2/setup.py` & `cylc-rose-1.3.3/setup.py`

 * *Files identical despite different names*

