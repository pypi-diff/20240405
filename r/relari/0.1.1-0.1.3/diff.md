# Comparing `tmp/relari-0.1.1.tar.gz` & `tmp/relari-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relari-0.1.1.tar", max compression
+gzip compressed data, was "relari-0.1.3.tar", max compression
```

## Comparing `relari-0.1.1.tar` & `relari-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     2100 2024-02-29 01:27:03.863704 relari-0.1.1/README.md
--rw-r--r--   0        0        0      467 2024-02-29 07:11:37.100114 relari-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       45 2024-02-29 01:11:53.776218 relari-0.1.1/relari/__init__.py
--rw-r--r--   0        0        0      199 2024-02-29 01:11:53.776623 relari-0.1.1/relari/eval/__init__.py
--rw-r--r--   0        0        0     5142 2024-02-29 01:11:53.776972 relari-0.1.1/relari/eval/dataset.py
--rw-r--r--   0        0        0     4656 2024-02-29 01:11:53.777323 relari-0.1.1/relari/eval/manager.py
--rw-r--r--   0        0        0     1669 2024-02-29 01:11:53.777735 relari-0.1.1/relari/eval/modules.py
--rw-r--r--   0        0        0     3413 2024-02-29 01:11:53.778019 relari-0.1.1/relari/eval/pipeline.py
--rw-r--r--   0        0        0     1771 2024-02-29 01:11:53.778261 relari-0.1.1/relari/eval/result_types.py
--rw-r--r--   0        0        0      123 2024-02-29 01:11:53.778488 relari-0.1.1/relari/eval/types.py
--rw-r--r--   0        0        0     1106 2024-02-29 01:11:53.779119 relari-0.1.1/relari/eval/utils.py
--rw-r--r--   0        0        0     1858 2024-02-29 07:11:37.101160 relari-0.1.1/relari/relari_client.py
--rw-r--r--   0        0        0     2668 1970-01-01 00:00:00.000000 relari-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2100 2024-02-29 01:27:03.863704 relari-0.1.3/README.md
+-rw-r--r--   0        0        0      464 2024-04-05 01:40:29.931180 relari-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-02-29 01:11:53.776218 relari-0.1.3/relari/__init__.py
+-rw-r--r--   0        0        0      199 2024-02-29 01:11:53.776623 relari-0.1.3/relari/eval/__init__.py
+-rw-r--r--   0        0        0     5142 2024-02-29 01:11:53.776972 relari-0.1.3/relari/eval/dataset.py
+-rw-r--r--   0        0        0     4790 2024-02-29 07:20:41.559538 relari-0.1.3/relari/eval/manager.py
+-rw-r--r--   0        0        0     1669 2024-02-29 01:11:53.777735 relari-0.1.3/relari/eval/modules.py
+-rw-r--r--   0        0        0     3413 2024-02-29 01:11:53.778019 relari-0.1.3/relari/eval/pipeline.py
+-rw-r--r--   0        0        0     1771 2024-02-29 01:11:53.778261 relari-0.1.3/relari/eval/result_types.py
+-rw-r--r--   0        0        0      123 2024-02-29 01:11:53.778488 relari-0.1.3/relari/eval/types.py
+-rw-r--r--   0        0        0     1106 2024-02-29 01:11:53.779119 relari-0.1.3/relari/eval/utils.py
+-rw-r--r--   0        0        0     3920 2024-04-05 01:17:20.592928 relari-0.1.3/relari/relari_client.py
+-rw-r--r--   0        0        0     2665 1970-01-01 00:00:00.000000 relari-0.1.3/PKG-INFO
```

### Comparing `relari-0.1.1/README.md` & `relari-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `relari-0.1.1/relari/eval/dataset.py` & `relari-0.1.3/relari/eval/dataset.py`

 * *Files identical despite different names*

### Comparing `relari-0.1.1/relari/eval/manager.py` & `relari-0.1.3/relari/eval/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,19 +52,20 @@
 
     def set_metadata(self, metadata: dict):
         self._metadata = metadata
 
     def is_running(self) -> bool:
         return self._is_running
 
-    def start_run(self, metadata: dict = dict()):
+    def start_run(self, metadata: Optional[dict] = None):
         self._idx = 0
         self._is_running = True
         self._eval_results = EvaluationResults(self._pipeline)
-        self.set_metadata(metadata)
+        if metadata is not None:
+            self.set_metadata(metadata)
 
     @property
     def curr_sample(self):
         if self._pipeline is None:
             raise ValueError("Pipeline not set")
         if self._idx >= len(self.dataset.data):
             self._is_running = False
@@ -77,22 +78,23 @@
         if self._idx >= len(self.dataset.data):
             self._is_running = False
         else:
             self._idx += 1
         return self.curr_sample
 
     # Context manager
-    def new_experiment(self):
+    def new_experiment(self, metadata: Optional[dict] = None):
         class ExperimentContext:
             def __init__(self, manager):
                 self._manager = manager
+                self._metadata = metadata
 
             def __enter__(self):
                 # Initialize the session
-                self._manager.start_run()
+                self._manager.start_run(self._metadata)
                 return (
                     self  # Return the session object itself to be used as an iterator
                 )
 
             def __exit__(self, exc_type, exc_val, exc_tb):
                 # Clean up the session
                 self._manager._is_running = False
```

### Comparing `relari-0.1.1/relari/eval/modules.py` & `relari-0.1.3/relari/eval/modules.py`

 * *Files identical despite different names*

### Comparing `relari-0.1.1/relari/eval/pipeline.py` & `relari-0.1.3/relari/eval/pipeline.py`

 * *Files identical despite different names*

### Comparing `relari-0.1.1/relari/eval/result_types.py` & `relari-0.1.3/relari/eval/result_types.py`

 * *Files identical despite different names*

### Comparing `relari-0.1.1/relari/eval/utils.py` & `relari-0.1.3/relari/eval/utils.py`

 * *Files identical despite different names*

### Comparing `relari-0.1.1/PKG-INFO` & `relari-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: relari
-Version: 0.1.1
+Version: 0.1.3
 Summary: 
 Author: Pasquale Antonante
-Author-email: p.antonante@gmail.com
+Author-email: pasquale@relari.ai
 Requires-Python: >=3.9.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
```

