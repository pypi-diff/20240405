# Comparing `tmp/xarg-python-1.4.tar.gz` & `tmp/xarg-python-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarg-python-1.4.tar", last modified: Mon Apr  1 16:54:31 2024, max compression
+gzip compressed data, was "xarg-python-1.4.1.tar", last modified: Fri Apr  5 16:55:07 2024, max compression
```

## Comparing `xarg-python-1.4.tar` & `xarg-python-1.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 16:54:31.816936 xarg-python-1.4/
--rw-r--r--   0 root         (0) root         (0)     1093 2023-08-28 15:46:08.000000 xarg-python-1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1267 2024-04-01 16:54:31.816936 xarg-python-1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      656 2023-11-23 15:08:18.000000 xarg-python-1.4/README.md
--rw-r--r--   0 root         (0) root         (0)      523 2024-04-01 16:54:31.816936 xarg-python-1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      779 2024-03-31 14:51:50.000000 xarg-python-1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 16:54:31.806936 xarg-python-1.4/xarg/
--rw-r--r--   0 root         (0) root         (0)      463 2024-04-01 15:33:01.000000 xarg-python-1.4/xarg/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22737 2024-04-01 16:48:28.000000 xarg-python-1.4/xarg/actuator.py
--rw-r--r--   0 root         (0) root         (0)      477 2024-04-01 16:53:51.000000 xarg-python-1.4/xarg/attribute.py
--rw-r--r--   0 root         (0) root         (0)     6327 2024-04-01 15:33:01.000000 xarg-python-1.4/xarg/colorful.py
--rw-r--r--   0 root         (0) root         (0)     8184 2024-03-31 14:53:08.000000 xarg-python-1.4/xarg/complete.py
--rw-r--r--   0 root         (0) root         (0)     8479 2024-03-31 14:51:50.000000 xarg-python-1.4/xarg/parser.py
--rw-r--r--   0 root         (0) root         (0)     2216 2024-03-31 14:25:54.000000 xarg-python-1.4/xarg/safefile.py
--rw-r--r--   0 root         (0) root         (0)     8482 2024-03-31 14:49:33.000000 xarg-python-1.4/xarg/scanner.py
--rw-r--r--   0 root         (0) root         (0)     1236 2024-03-31 15:00:43.000000 xarg-python-1.4/xarg/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 16:54:31.816936 xarg-python-1.4/xarg_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1267 2024-04-01 16:54:31.000000 xarg-python-1.4/xarg_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      425 2024-04-01 16:54:31.000000 xarg-python-1.4/xarg_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 16:54:31.000000 xarg-python-1.4/xarg_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-04-01 16:54:31.000000 xarg-python-1.4/xarg_python.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-04-01 16:54:31.000000 xarg-python-1.4/xarg_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-01 16:54:31.000000 xarg-python-1.4/xarg_python.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 16:54:31.000000 xarg-python-1.4/xarg_python.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:55:07.698812 xarg-python-1.4.1/
+-rw-r--r--   0 root         (0) root         (0)     1093 2023-08-28 15:46:08.000000 xarg-python-1.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1320 2024-04-05 16:55:07.698812 xarg-python-1.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      656 2023-11-23 15:08:18.000000 xarg-python-1.4.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      579 2024-04-05 16:55:07.698812 xarg-python-1.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      779 2024-03-31 14:51:50.000000 xarg-python-1.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:55:07.698812 xarg-python-1.4.1/xarg/
+-rw-r--r--   0 root         (0) root         (0)      463 2024-04-01 15:33:01.000000 xarg-python-1.4.1/xarg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22952 2024-04-02 15:42:25.000000 xarg-python-1.4.1/xarg/actuator.py
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-05 16:53:41.000000 xarg-python-1.4.1/xarg/attribute.py
+-rw-r--r--   0 root         (0) root         (0)     9216 2024-04-05 16:52:06.000000 xarg-python-1.4.1/xarg/colorful.py
+-rw-r--r--   0 root         (0) root         (0)     8184 2024-03-31 14:53:08.000000 xarg-python-1.4.1/xarg/complete.py
+-rw-r--r--   0 root         (0) root         (0)     8479 2024-03-31 14:51:50.000000 xarg-python-1.4.1/xarg/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2024-03-31 14:25:54.000000 xarg-python-1.4.1/xarg/safefile.py
+-rw-r--r--   0 root         (0) root         (0)     8482 2024-03-31 14:49:33.000000 xarg-python-1.4.1/xarg/scanner.py
+-rw-r--r--   0 root         (0) root         (0)     1236 2024-03-31 15:00:43.000000 xarg-python-1.4.1/xarg/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:55:07.698812 xarg-python-1.4.1/xarg_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1320 2024-04-05 16:55:07.000000 xarg-python-1.4.1/xarg_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      425 2024-04-05 16:55:07.000000 xarg-python-1.4.1/xarg_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 16:55:07.000000 xarg-python-1.4.1/xarg_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-04-05 16:55:07.000000 xarg-python-1.4.1/xarg_python.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-04-05 16:55:07.000000 xarg-python-1.4.1/xarg_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-05 16:55:07.000000 xarg-python-1.4.1/xarg_python.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 16:55:07.000000 xarg-python-1.4.1/xarg_python.egg-info/zip-safe
```

### Comparing `xarg-python-1.4/LICENSE` & `xarg-python-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4/PKG-INFO` & `xarg-python-1.4.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: xarg-python
-Version: 1.4
+Version: 1.4.1
 Summary: Simple command-line tool based on argparse.
 Home-page: https://github.com/bondbox/xarg-python/
 Author: Mingzhe Zou
 Author-email: zoumingzhe@outlook.com
 License: MIT
 Project-URL: Source Code, https://github.com/bondbox/xarg-python/
 Project-URL: Bug Tracker, https://github.com/bondbox/xarg-python/issues
 Project-URL: Documentation, https://github.com/bondbox/xarg-python/
-Keywords: command,command-line,argparse,xarg
+Keywords: command,command-line,argparse,argcomplete,completion,xarg,colorama,colorlog,termainal
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 xarg
```

### Comparing `xarg-python-1.4/README.md` & `xarg-python-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4/setup.cfg` & `xarg-python-1.4.1/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-keywords = command, command-line, argparse, xarg
+keywords = command, command-line, argparse, argcomplete, completion, xarg, colorama, colorlog, termainal
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 license_files = LICENSE
 platforms = any
 classifiers = 
 	Programming Language :: Python
```

### Comparing `xarg-python-1.4/setup.py` & `xarg-python-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4/xarg/actuator.py` & `xarg-python-1.4.1/xarg/actuator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # coding:utf-8
 
 from argparse import Namespace
 from errno import EINTR
 from errno import ENOENT
 import logging
+import os
 import sys
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 
 from colorlog import ColoredFormatter
 
 from .parser import argp
 from .util import singleton
 
-
 DEFAULT_LOG_FORMAT = "%(log_color)s%(message)s"
 DEFAULT_LOG_COLORS = {
     "DEBUG": "black",
     "INFO": "white",
     "WARNING": "yellow",
     "ERROR": "red",
     "CRITICAL": "light_red",
@@ -550,15 +550,19 @@
             self.logger.addHandler(handler)
 
         if hasattr(args, "_log_console_") and args._log_console_ is not None:
             addHandler(logging.StreamHandler(stream=args._log_console_))
 
         if hasattr(args, "_log_files_"):
             for filename in args._log_files_:
-                assert isinstance(filename, str)
+                assert isinstance(filename, str), \
+                    f"Unexpected type: {type(filename)}"
+                dirname: str = os.path.dirname(filename)
+                if not os.path.exists(dirname):
+                    os.makedirs(dirname)
                 addHandler(logging.FileHandler(filename))
 
     def __add_parser(self, _map: Dict[add_command, argp],
                      arg_root: argp, cmd_root: add_command, **kwargs):
         assert isinstance(cmd_root, add_command)
         assert cmd_root not in _map
         _map[cmd_root] = arg_root
```

### Comparing `xarg-python-1.4/xarg/complete.py` & `xarg-python-1.4.1/xarg/complete.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4/xarg/parser.py` & `xarg-python-1.4.1/xarg/parser.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4/xarg/safefile.py` & `xarg-python-1.4.1/xarg/safefile.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4/xarg/scanner.py` & `xarg-python-1.4.1/xarg/scanner.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4/xarg/util.py` & `xarg-python-1.4.1/xarg/util.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4/xarg_python.egg-info/PKG-INFO` & `xarg-python-1.4.1/xarg_python.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: xarg-python
-Version: 1.4
+Version: 1.4.1
 Summary: Simple command-line tool based on argparse.
 Home-page: https://github.com/bondbox/xarg-python/
 Author: Mingzhe Zou
 Author-email: zoumingzhe@outlook.com
 License: MIT
 Project-URL: Source Code, https://github.com/bondbox/xarg-python/
 Project-URL: Bug Tracker, https://github.com/bondbox/xarg-python/issues
 Project-URL: Documentation, https://github.com/bondbox/xarg-python/
-Keywords: command,command-line,argparse,xarg
+Keywords: command,command-line,argparse,argcomplete,completion,xarg,colorama,colorlog,termainal
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 xarg
```

