# Comparing `tmp/hypatorch-0.2.4.tar.gz` & `tmp/hypatorch-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypatorch-0.2.4.tar", last modified: Wed Mar 27 11:23:06 2024, max compression
+gzip compressed data, was "hypatorch-0.2.5.tar", last modified: Fri Apr  5 13:34:19 2024, max compression
```

## Comparing `hypatorch-0.2.4.tar` & `hypatorch-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 paulkrug   (502) staff       (20)        0 2024-03-27 11:23:06.149679 hypatorch-0.2.4/
--rw-r--r--   0 paulkrug   (502) staff       (20)    11357 2024-03-18 15:51:00.000000 hypatorch-0.2.4/LICENSE
--rw-r--r--   0 paulkrug   (502) staff       (20)      779 2024-03-27 11:23:06.149433 hypatorch-0.2.4/PKG-INFO
--rw-r--r--   0 paulkrug   (502) staff       (20)      403 2024-03-18 20:05:31.000000 hypatorch-0.2.4/README.md
-drwxr-xr-x   0 paulkrug   (502) staff       (20)        0 2024-03-27 11:23:06.148090 hypatorch-0.2.4/hypatorch/
--rw-r--r--   0 paulkrug   (502) staff       (20)      258 2024-03-27 11:14:03.000000 hypatorch-0.2.4/hypatorch/__init__.py
--rw-r--r--   0 paulkrug   (502) staff       (20)     4729 2024-03-20 14:26:18.000000 hypatorch-0.2.4/hypatorch/assessments.py
--rw-r--r--   0 paulkrug   (502) staff       (20)    22664 2024-03-25 17:53:56.000000 hypatorch-0.2.4/hypatorch/core.py
--rw-r--r--   0 paulkrug   (502) staff       (20)     2544 2024-03-18 20:05:31.000000 hypatorch-0.2.4/hypatorch/losses.py
--rw-r--r--   0 paulkrug   (502) staff       (20)     7421 2024-03-27 10:39:37.000000 hypatorch-0.2.4/hypatorch/utils.py
-drwxr-xr-x   0 paulkrug   (502) staff       (20)        0 2024-03-27 11:23:06.149196 hypatorch-0.2.4/hypatorch.egg-info/
--rw-r--r--   0 paulkrug   (502) staff       (20)      779 2024-03-27 11:23:06.000000 hypatorch-0.2.4/hypatorch.egg-info/PKG-INFO
--rw-r--r--   0 paulkrug   (502) staff       (20)      294 2024-03-27 11:23:06.000000 hypatorch-0.2.4/hypatorch.egg-info/SOURCES.txt
--rw-r--r--   0 paulkrug   (502) staff       (20)        1 2024-03-27 11:23:06.000000 hypatorch-0.2.4/hypatorch.egg-info/dependency_links.txt
--rw-r--r--   0 paulkrug   (502) staff       (20)       37 2024-03-27 11:23:06.000000 hypatorch-0.2.4/hypatorch.egg-info/requires.txt
--rw-r--r--   0 paulkrug   (502) staff       (20)       10 2024-03-27 11:23:06.000000 hypatorch-0.2.4/hypatorch.egg-info/top_level.txt
--rw-r--r--   0 paulkrug   (502) staff       (20)       38 2024-03-27 11:23:06.149740 hypatorch-0.2.4/setup.cfg
--rw-r--r--   0 paulkrug   (502) staff       (20)      807 2024-03-19 10:48:19.000000 hypatorch-0.2.4/setup.py
+drwxr-xr-x   0 paulkrug   (502) staff       (20)        0 2024-04-05 13:34:19.480176 hypatorch-0.2.5/
+-rw-r--r--   0 paulkrug   (502) staff       (20)    11357 2024-03-18 15:51:00.000000 hypatorch-0.2.5/LICENSE
+-rw-r--r--   0 paulkrug   (502) staff       (20)      779 2024-04-05 13:34:19.479976 hypatorch-0.2.5/PKG-INFO
+-rw-r--r--   0 paulkrug   (502) staff       (20)      403 2024-03-18 20:05:31.000000 hypatorch-0.2.5/README.md
+drwxr-xr-x   0 paulkrug   (502) staff       (20)        0 2024-04-05 13:34:19.478722 hypatorch-0.2.5/hypatorch/
+-rw-r--r--   0 paulkrug   (502) staff       (20)      258 2024-04-05 13:32:38.000000 hypatorch-0.2.5/hypatorch/__init__.py
+-rw-r--r--   0 paulkrug   (502) staff       (20)     4729 2024-03-20 14:26:18.000000 hypatorch-0.2.5/hypatorch/assessments.py
+-rw-r--r--   0 paulkrug   (502) staff       (20)    23013 2024-04-05 13:32:21.000000 hypatorch-0.2.5/hypatorch/core.py
+-rw-r--r--   0 paulkrug   (502) staff       (20)     2544 2024-03-18 20:05:31.000000 hypatorch-0.2.5/hypatorch/losses.py
+-rw-r--r--   0 paulkrug   (502) staff       (20)     7421 2024-03-27 10:39:37.000000 hypatorch-0.2.5/hypatorch/utils.py
+drwxr-xr-x   0 paulkrug   (502) staff       (20)        0 2024-04-05 13:34:19.479742 hypatorch-0.2.5/hypatorch.egg-info/
+-rw-r--r--   0 paulkrug   (502) staff       (20)      779 2024-04-05 13:34:19.000000 hypatorch-0.2.5/hypatorch.egg-info/PKG-INFO
+-rw-r--r--   0 paulkrug   (502) staff       (20)      294 2024-04-05 13:34:19.000000 hypatorch-0.2.5/hypatorch.egg-info/SOURCES.txt
+-rw-r--r--   0 paulkrug   (502) staff       (20)        1 2024-04-05 13:34:19.000000 hypatorch-0.2.5/hypatorch.egg-info/dependency_links.txt
+-rw-r--r--   0 paulkrug   (502) staff       (20)       37 2024-04-05 13:34:19.000000 hypatorch-0.2.5/hypatorch.egg-info/requires.txt
+-rw-r--r--   0 paulkrug   (502) staff       (20)       10 2024-04-05 13:34:19.000000 hypatorch-0.2.5/hypatorch.egg-info/top_level.txt
+-rw-r--r--   0 paulkrug   (502) staff       (20)       38 2024-04-05 13:34:19.480219 hypatorch-0.2.5/setup.cfg
+-rw-r--r--   0 paulkrug   (502) staff       (20)      807 2024-03-19 10:48:19.000000 hypatorch-0.2.5/setup.py
```

### Comparing `hypatorch-0.2.4/LICENSE` & `hypatorch-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hypatorch-0.2.4/PKG-INFO` & `hypatorch-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypatorch
-Version: 0.2.4
+Version: 0.2.5
 Summary: HypaTorch: A library for abstract and visual model configuration
 Home-page: https://github.com/Altavo/hypatorch/
 Author: Altavo GmbH
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
```

### Comparing `hypatorch-0.2.4/hypatorch/assessments.py` & `hypatorch-0.2.5/hypatorch/assessments.py`

 * *Files identical despite different names*

### Comparing `hypatorch-0.2.4/hypatorch/core.py` & `hypatorch-0.2.5/hypatorch/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -662,14 +662,25 @@
                 
             output_dict = self._handle_operation_output(
                 x = operation_out,
                 output_dict = output_dict,
                 operation_name = operation_name,
                 )
             
+            # handle metrics
+            self._handle_assessments(
+                assessments = self.metrics,
+                data_dict = shared_dict(
+                    input_dict,
+                    output_dict,
+                    ),
+                operation_name = operation_name,
+                mode = mode,
+                )
+            
             
         data_dict = shared_dict(
             input_dict,
             output_dict,
             )
             
         return data_dict
```

### Comparing `hypatorch-0.2.4/hypatorch/losses.py` & `hypatorch-0.2.5/hypatorch/losses.py`

 * *Files identical despite different names*

### Comparing `hypatorch-0.2.4/hypatorch/utils.py` & `hypatorch-0.2.5/hypatorch/utils.py`

 * *Files identical despite different names*

### Comparing `hypatorch-0.2.4/hypatorch.egg-info/PKG-INFO` & `hypatorch-0.2.5/hypatorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypatorch
-Version: 0.2.4
+Version: 0.2.5
 Summary: HypaTorch: A library for abstract and visual model configuration
 Home-page: https://github.com/Altavo/hypatorch/
 Author: Altavo GmbH
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
```

### Comparing `hypatorch-0.2.4/setup.py` & `hypatorch-0.2.5/setup.py`

 * *Files identical despite different names*

