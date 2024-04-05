# Comparing `tmp/akasaka-0.1.3.tar.gz` & `tmp/akasaka-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akasaka-0.1.3.tar", last modified: Thu Apr  4 05:47:09 2024, max compression
+gzip compressed data, was "akasaka-0.1.4.tar", last modified: Fri Apr  5 01:52:30 2024, max compression
```

## Comparing `akasaka-0.1.3.tar` & `akasaka-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:47:09.071745 akasaka-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-04 05:46:59.000000 akasaka-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-04 05:47:09.071745 akasaka-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-04 05:46:59.000000 akasaka-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:47:09.071745 akasaka-0.1.3/akasaka/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-04 05:46:59.000000 akasaka-0.1.3/akasaka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-04 05:46:59.000000 akasaka-0.1.3/akasaka/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-04 05:46:59.000000 akasaka-0.1.3/akasaka/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-04 05:46:59.000000 akasaka-0.1.3/akasaka/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-04 05:46:59.000000 akasaka-0.1.3/akasaka/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-04 05:46:59.000000 akasaka-0.1.3/akasaka/torch_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-04 05:46:59.000000 akasaka-0.1.3/akasaka/torch_task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:47:09.071745 akasaka-0.1.3/akasaka/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 05:46:59.000000 akasaka-0.1.3/akasaka/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-04 05:46:59.000000 akasaka-0.1.3/akasaka/utils/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-04 05:46:59.000000 akasaka-0.1.3/akasaka/utils/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:47:09.071745 akasaka-0.1.3/akasaka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-04 05:47:09.000000 akasaka-0.1.3/akasaka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-04 05:47:09.000000 akasaka-0.1.3/akasaka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 05:47:09.000000 akasaka-0.1.3/akasaka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-04 05:47:09.000000 akasaka-0.1.3/akasaka.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 05:47:09.000000 akasaka-0.1.3/akasaka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 05:47:09.000000 akasaka-0.1.3/akasaka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 05:47:09.071745 akasaka-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-04 05:46:59.000000 akasaka-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:52:30.606449 akasaka-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-05 01:52:19.000000 akasaka-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-05 01:52:30.606449 akasaka-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-05 01:52:19.000000 akasaka-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:52:30.602449 akasaka-0.1.4/akasaka/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-05 01:52:19.000000 akasaka-0.1.4/akasaka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-05 01:52:19.000000 akasaka-0.1.4/akasaka/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-05 01:52:19.000000 akasaka-0.1.4/akasaka/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-05 01:52:19.000000 akasaka-0.1.4/akasaka/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-05 01:52:19.000000 akasaka-0.1.4/akasaka/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-05 01:52:19.000000 akasaka-0.1.4/akasaka/torch_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-05 01:52:19.000000 akasaka-0.1.4/akasaka/torch_task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:52:30.606449 akasaka-0.1.4/akasaka/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 01:52:19.000000 akasaka-0.1.4/akasaka/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-05 01:52:19.000000 akasaka-0.1.4/akasaka/utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-05 01:52:19.000000 akasaka-0.1.4/akasaka/utils/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:52:30.606449 akasaka-0.1.4/akasaka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-05 01:52:30.000000 akasaka-0.1.4/akasaka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-05 01:52:30.000000 akasaka-0.1.4/akasaka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 01:52:30.000000 akasaka-0.1.4/akasaka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-05 01:52:30.000000 akasaka-0.1.4/akasaka.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-05 01:52:30.000000 akasaka-0.1.4/akasaka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 01:52:30.000000 akasaka-0.1.4/akasaka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 01:52:30.606449 akasaka-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-05 01:52:19.000000 akasaka-0.1.4/setup.py
```

### Comparing `akasaka-0.1.3/LICENSE` & `akasaka-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `akasaka-0.1.3/PKG-INFO` & `akasaka-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akasaka
-Version: 0.1.3
+Version: 0.1.4
 Summary: Dynamic mutiprocess preprocessing task loader and dispatcher
 Home-page: https://github.com/JeffersonQin/akasaka
 Author: Haoyun Qin
 Author-email: qhy.cis@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `akasaka-0.1.3/README.md` & `akasaka-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `akasaka-0.1.3/akasaka/executor.py` & `akasaka-0.1.4/akasaka/executor.py`

 * *Files identical despite different names*

### Comparing `akasaka-0.1.3/akasaka/loader.py` & `akasaka-0.1.4/akasaka/loader.py`

 * *Files identical despite different names*

### Comparing `akasaka-0.1.3/akasaka/main.py` & `akasaka-0.1.4/akasaka/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,11 +38,11 @@
         chunksize = args.chunksize
         akasaka_execute(akasaka_task, num_process, chunksize)
         return
 
     if issubclass(loaded_class, AkasakaTorchTask):
         from .torch_executor import akasaka_torch_execute
         devices = args.devices
-        akasaka_torch_execute(akasaka_task, module_path, args, devices)
+        akasaka_torch_execute(akasaka_task, module_path, remaining_args, devices)
         return
 
     raise ValueError("The loaded class should be a subclass of 'AkasakaTask' or 'AkasakaTorchTask'.")
```

### Comparing `akasaka-0.1.3/akasaka/task.py` & `akasaka-0.1.4/akasaka/task.py`

 * *Files identical despite different names*

### Comparing `akasaka-0.1.3/akasaka/torch_executor.py` & `akasaka-0.1.4/akasaka/torch_executor.py`

 * *Files identical despite different names*

### Comparing `akasaka-0.1.3/akasaka/torch_task.py` & `akasaka-0.1.4/akasaka/torch_task.py`

 * *Files identical despite different names*

### Comparing `akasaka-0.1.3/akasaka/utils/io.py` & `akasaka-0.1.4/akasaka/utils/io.py`

 * *Files identical despite different names*

### Comparing `akasaka-0.1.3/akasaka.egg-info/PKG-INFO` & `akasaka-0.1.4/akasaka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akasaka
-Version: 0.1.3
+Version: 0.1.4
 Summary: Dynamic mutiprocess preprocessing task loader and dispatcher
 Home-page: https://github.com/JeffersonQin/akasaka
 Author: Haoyun Qin
 Author-email: qhy.cis@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `akasaka-0.1.3/setup.py` & `akasaka-0.1.4/setup.py`

 * *Files identical despite different names*

