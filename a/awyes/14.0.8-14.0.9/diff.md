# Comparing `tmp/awyes-14.0.8.tar.gz` & `tmp/awyes-14.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awyes-14.0.8.tar", last modified: Mon Mar 11 04:43:12 2024, max compression
+gzip compressed data, was "awyes-14.0.9.tar", last modified: Tue Mar 12 05:31:51 2024, max compression
```

## Comparing `awyes-14.0.8.tar` & `awyes-14.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 04:43:12.594775 awyes-14.0.8/
--rw-r--r--   0 root         (0) root         (0)      765 2024-03-11 04:43:12.594775 awyes-14.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5835 2024-03-11 04:42:55.000000 awyes-14.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 04:43:12.590775 awyes-14.0.8/awyes/
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-11 04:43:07.000000 awyes-14.0.8/awyes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3740 2024-03-11 04:42:55.000000 awyes-14.0.8/awyes/awyes.py
--rw-r--r--   0 root         (0) root         (0)      357 2024-03-11 04:42:55.000000 awyes-14.0.8/awyes/constants.py
--rw-r--r--   0 root         (0) root         (0)     4715 2024-03-11 04:42:55.000000 awyes-14.0.8/awyes/deploy.py
--rw-r--r--   0 root         (0) root         (0)      852 2024-03-11 04:42:55.000000 awyes-14.0.8/awyes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 04:43:12.594775 awyes-14.0.8/awyes.egg-info/
--rw-r--r--   0 root         (0) root         (0)      765 2024-03-11 04:43:12.000000 awyes-14.0.8/awyes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      277 2024-03-11 04:43:12.000000 awyes-14.0.8/awyes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-11 04:43:12.000000 awyes-14.0.8/awyes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-03-11 04:43:12.000000 awyes-14.0.8/awyes.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-03-11 04:43:12.000000 awyes-14.0.8/awyes.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-03-11 04:43:12.000000 awyes-14.0.8/awyes.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-11 04:43:12.594775 awyes-14.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      947 2024-03-11 04:42:55.000000 awyes-14.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 05:31:51.660224 awyes-14.0.9/
+-rw-r--r--   0 root         (0) root         (0)      765 2024-03-12 05:31:51.660224 awyes-14.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5835 2024-03-12 05:31:34.000000 awyes-14.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 05:31:51.656224 awyes-14.0.9/awyes/
+-rw-r--r--   0 root         (0) root         (0)       23 2024-03-12 05:31:46.000000 awyes-14.0.9/awyes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3740 2024-03-12 05:31:34.000000 awyes-14.0.9/awyes/awyes.py
+-rw-r--r--   0 root         (0) root         (0)      395 2024-03-12 05:31:34.000000 awyes-14.0.9/awyes/constants.py
+-rw-r--r--   0 root         (0) root         (0)     4827 2024-03-12 05:31:34.000000 awyes-14.0.9/awyes/deploy.py
+-rw-r--r--   0 root         (0) root         (0)      852 2024-03-12 05:31:34.000000 awyes-14.0.9/awyes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 05:31:51.660224 awyes-14.0.9/awyes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      765 2024-03-12 05:31:51.000000 awyes-14.0.9/awyes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      277 2024-03-12 05:31:51.000000 awyes-14.0.9/awyes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-12 05:31:51.000000 awyes-14.0.9/awyes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-03-12 05:31:51.000000 awyes-14.0.9/awyes.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-03-12 05:31:51.000000 awyes-14.0.9/awyes.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-03-12 05:31:51.000000 awyes-14.0.9/awyes.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-12 05:31:51.660224 awyes-14.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      947 2024-03-12 05:31:34.000000 awyes-14.0.9/setup.py
```

### Comparing `awyes-14.0.8/PKG-INFO` & `awyes-14.0.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awyes
-Version: 14.0.8
+Version: 14.0.9
 Summary: A package for easy setup and management of resources on AWS
 Home-page: https://github.com/bb-labs/awyes
 Author: Truman Purnell
 Author-email: truman.purnell@gmail.com
 Keywords: aws resources manager setup management automation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `awyes-14.0.8/README.md` & `awyes-14.0.9/README.md`

 * *Files identical despite different names*

### Comparing `awyes-14.0.8/awyes/awyes.py` & `awyes-14.0.9/awyes/awyes.py`

 * *Files identical despite different names*

### Comparing `awyes-14.0.8/awyes/deploy.py` & `awyes-14.0.9/awyes/deploy.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 import types
 import textwrap
 import traceback
 import collections
 
 from .utils import rgetattr, rsetattr, Colors
 from .constants import (
+    X,
+    CHECK,
+    ARROW,
     DOT,
     MATCH_REF,
     CACHE_REGEX,
     USER_CLIENT_MODULE_NAME,
 )
 
 
@@ -44,15 +47,16 @@
 
     def find_recursive_actions(self, args):
         """Look through the args dict and find all actions for cache references."""
         return [
             action
             for cache_reference in re.findall(CACHE_REGEX, json.dumps(args))
             for action_prefixes in [
-                cache_reference.split(DOT)[:i]
+                # Generate all prefixes of the cache reference to find matching actions
+                cache_reference.split(DOT)[: i + 1]
                 for i in range(len(cache_reference.split(DOT)))
             ]
             if (action := DOT.join(action_prefixes)) in self.config
         ]
 
     def run(self, actions):
         """Run the deployment."""
@@ -86,36 +90,36 @@
                 (
                     fn_name
                     if client_name == USER_CLIENT_MODULE_NAME
                     else f"{client_name}.{fn_name}"
                 ),
             )
         except Exception as e:
-            self.print_status("Could not resolve function", Colors.FAIL, "✗")
+            self.print_status("Could not resolve function", Colors.FAIL, X)
             traceback.print_exception(e)
             return
 
         # If we're not quiet and are dry running, print the unresolved args
         if self.flags.dry:
             if not self.flags.quiet:
-                self.print_status(self.config[action], Colors.OKBLUE, "→")
+                self.print_status(self.config[action], Colors.OKBLUE, ARROW)
             return
 
         # Try to resolve the args
         try:
             args = self.resolve(self.config[action])
         except Exception as e:
-            self.print_status("Could not resolve args", Colors.FAIL, "✗")
-            self.print_status(self.config[action], Colors.FAIL, "✗")
+            self.print_status("Could not resolve args", Colors.FAIL, X)
+            self.print_status(self.config[action], Colors.FAIL, X)
             traceback.print_exception(e)
             return
 
         # If we're not quiet, print the resolved args
         if not self.flags.quiet and args:
-            self.print_status(args, Colors.OKBLUE, "→")
+            self.print_status(args, Colors.OKBLUE, ARROW)
 
         # Try to execute the function
         try:
             if isinstance(args, dict):
                 value = fn(**args)
             elif isinstance(args, list):
                 value = fn(*args)
@@ -124,22 +128,22 @@
             else:
                 value = fn()
 
             # Auto-unpack generator results
             if isinstance(value, types.GeneratorType):
                 value = list(value)
         except Exception as e:
-            self.print_status("Could not execute function", Colors.FAIL, "✗")
+            self.print_status("Could not execute function", Colors.FAIL, X)
             traceback.print_exception(e)
             return
 
         # If we're not quiet, print the result
-        if not self.flags.quiet:
-            self.print_status(value, Colors.OKGREEN, "✓")
+        if not self.flags.quiet and value:
+            self.print_status(value, Colors.OKGREEN, CHECK)
 
         # Try to cache the result
         try:
             rsetattr(self.cache, id, json.loads(json.dumps(value, default=str)))
         except Exception as e:
-            self.print_status("Could not cache result", Colors.FAIL, "✗")
+            self.print_status("Could not cache result", Colors.FAIL, X)
             traceback.print_exception(e)
             return
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `awyes-14.0.8/awyes/utils.py` & `awyes-14.0.9/awyes/utils.py`

 * *Files identical despite different names*

### Comparing `awyes-14.0.8/awyes.egg-info/PKG-INFO` & `awyes-14.0.9/awyes.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awyes
-Version: 14.0.8
+Version: 14.0.9
 Summary: A package for easy setup and management of resources on AWS
 Home-page: https://github.com/bb-labs/awyes
 Author: Truman Purnell
 Author-email: truman.purnell@gmail.com
 Keywords: aws resources manager setup management automation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `awyes-14.0.8/setup.py` & `awyes-14.0.9/setup.py`

 * *Files identical despite different names*

