# Comparing `tmp/processing-pypelines-0.0.53.tar.gz` & `tmp/processing-pypelines-0.0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processing-pypelines-0.0.53.tar", last modified: Thu Apr  4 21:45:29 2024, max compression
+gzip compressed data, was "processing-pypelines-0.0.54.tar", last modified: Thu Apr  4 23:51:47 2024, max compression
```

## Comparing `processing-pypelines-0.0.53.tar` & `processing-pypelines-0.0.54.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:45:29.278367 processing-pypelines-0.0.53/
--rw-rw-rw-   0 root         (0) root         (0)     1073 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 21:45:29.274367 processing-pypelines-0.0.53/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1132 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/requirements-celery.txt
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 21:45:29.278367 processing-pypelines-0.0.53/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:45:29.270367 processing-pypelines-0.0.53/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:45:29.274367 processing-pypelines-0.0.53/src/processing_pypelines.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 21:45:29.000000 processing-pypelines-0.0.53/src/processing_pypelines.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      742 2024-04-04 21:45:29.000000 processing-pypelines-0.0.53/src/processing_pypelines.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 21:45:29.000000 processing-pypelines-0.0.53/src/processing_pypelines.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      306 2024-04-04 21:45:29.000000 processing-pypelines-0.0.53/src/processing_pypelines.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-04 21:45:29.000000 processing-pypelines-0.0.53/src/processing_pypelines.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:45:29.274367 processing-pypelines-0.0.53/src/pypelines/
--rw-rw-rw-   0 root         (0) root         (0)      206 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2365 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/accessors.py
--rw-rw-rw-   0 root         (0) root         (0)     3191 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/arguments.py
--rw-rw-rw-   0 root         (0) root         (0)    21401 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/celery_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     7301 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/disk.py
--rw-rw-rw-   0 root         (0) root         (0)     2901 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/examples.py
--rw-rw-rw-   0 root         (0) root         (0)     4650 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/graphs.py
--rw-rw-rw-   0 root         (0) root         (0)    15517 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/loggs.py
--rw-rw-rw-   0 root         (0) root         (0)     3386 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/multisession.py
--rw-rw-rw-   0 root         (0) root         (0)    14910 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/pickle_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     5461 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/pipelines.py
--rw-rw-rw-   0 root         (0) root         (0)     5669 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/pipes.py
--rw-rw-rw-   0 root         (0) root         (0)     1692 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/sessions.py
--rw-rw-rw-   0 root         (0) root         (0)    29008 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/steps.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     4326 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/versions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:45:29.274367 processing-pypelines-0.0.53/tests/
--rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/tests/tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:51:47.385151 processing-pypelines-0.0.54/
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2024-04-04 23:51:37.000000 processing-pypelines-0.0.54/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 23:51:47.385151 processing-pypelines-0.0.54/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-04-04 23:51:37.000000 processing-pypelines-0.0.54/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1132 2024-04-04 23:51:37.000000 processing-pypelines-0.0.54/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-04 23:51:37.000000 processing-pypelines-0.0.54/requirements-celery.txt
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-04 23:51:37.000000 processing-pypelines-0.0.54/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 23:51:47.385151 processing-pypelines-0.0.54/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:51:47.377152 processing-pypelines-0.0.54/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:51:47.381152 processing-pypelines-0.0.54/src/processing_pypelines.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 23:51:47.000000 processing-pypelines-0.0.54/src/processing_pypelines.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      742 2024-04-04 23:51:47.000000 processing-pypelines-0.0.54/src/processing_pypelines.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 23:51:47.000000 processing-pypelines-0.0.54/src/processing_pypelines.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      306 2024-04-04 23:51:47.000000 processing-pypelines-0.0.54/src/processing_pypelines.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-04 23:51:47.000000 processing-pypelines-0.0.54/src/processing_pypelines.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:51:47.381152 processing-pypelines-0.0.54/src/pypelines/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2024-04-04 23:51:37.000000 processing-pypelines-0.0.54/src/pypelines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2365 2024-04-04 23:51:37.000000 processing-pypelines-0.0.54/src/pypelines/accessors.py
+-rw-rw-rw-   0 root         (0) root         (0)     3191 2024-04-04 23:51:37.000000 processing-pypelines-0.0.54/src/pypelines/arguments.py
+-rw-rw-rw-   0 root         (0) root         (0)    22325 2024-04-04 23:51:37.000000 processing-pypelines-0.0.54/src/pypelines/celery_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     7301 2024-04-04 23:51:37.000000 processing-pypelines-0.0.54/src/pypelines/disk.py
+-rw-rw-rw-   0 root         (0) root         (0)     2901 2024-04-04 23:51:37.000000 processing-pypelines-0.0.54/src/pypelines/examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     4650 2024-04-04 23:51:37.000000 processing-pypelines-0.0.54/src/pypelines/graphs.py
+-rw-rw-rw-   0 root         (0) root         (0)    15517 2024-04-04 23:51:37.000000 processing-pypelines-0.0.54/src/pypelines/loggs.py
+-rw-rw-rw-   0 root         (0) root         (0)     3386 2024-04-04 23:51:37.000000 processing-pypelines-0.0.54/src/pypelines/multisession.py
+-rw-rw-rw-   0 root         (0) root         (0)    14910 2024-04-04 23:51:37.000000 processing-pypelines-0.0.54/src/pypelines/pickle_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     5461 2024-04-04 23:51:37.000000 processing-pypelines-0.0.54/src/pypelines/pipelines.py
+-rw-rw-rw-   0 root         (0) root         (0)     5669 2024-04-04 23:51:37.000000 processing-pypelines-0.0.54/src/pypelines/pipes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1692 2024-04-04 23:51:37.000000 processing-pypelines-0.0.54/src/pypelines/sessions.py
+-rw-rw-rw-   0 root         (0) root         (0)    29008 2024-04-04 23:51:37.000000 processing-pypelines-0.0.54/src/pypelines/steps.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2024-04-04 23:51:37.000000 processing-pypelines-0.0.54/src/pypelines/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     4326 2024-04-04 23:51:37.000000 processing-pypelines-0.0.54/src/pypelines/versions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:51:47.381152 processing-pypelines-0.0.54/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-04 23:51:37.000000 processing-pypelines-0.0.54/tests/tests.py
```

### Comparing `processing-pypelines-0.0.53/LICENSE` & `processing-pypelines-0.0.54/LICENSE`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.53/PKG-INFO` & `processing-pypelines-0.0.54/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processing-pypelines
-Version: 0.0.53
+Version: 0.0.54
 Summary: Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api
 Author-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 Maintainer-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 License: MIT
 Project-URL: homepage, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: repository, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: documentation, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
```

### Comparing `processing-pypelines-0.0.53/pyproject.toml` & `processing-pypelines-0.0.54/pyproject.toml`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.53/src/processing_pypelines.egg-info/PKG-INFO` & `processing-pypelines-0.0.54/src/processing_pypelines.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processing-pypelines
-Version: 0.0.53
+Version: 0.0.54
 Summary: Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api
 Author-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 Maintainer-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 License: MIT
 Project-URL: homepage, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: repository, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: documentation, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
```

### Comparing `processing-pypelines-0.0.53/src/processing_pypelines.egg-info/SOURCES.txt` & `processing-pypelines-0.0.54/src/processing_pypelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.53/src/pypelines/accessors.py` & `processing-pypelines-0.0.54/src/pypelines/accessors.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.53/src/pypelines/arguments.py` & `processing-pypelines-0.0.54/src/pypelines/arguments.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.53/src/pypelines/celery_tasks.py` & `processing-pypelines-0.0.54/src/pypelines/celery_tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,14 +232,33 @@
 
         response_handle = app.send_task(name=task_name, kwargs={"task_id": task_dict["id"], "extra": extra})
 
         return CeleryTaskRecord(
             task_dict["id"], task_infos_dict=task_dict, response_handle=response_handle, session=session
         )
 
+    @staticmethod
+    def create_from_model(
+        app: "Celery", task_model: type, task_name: str, pipeline_name: str, session: object, extra=None, **kwargs
+    ):
+
+        new_task = task_model(
+            name=task_name, session=session, arguments=kwargs, status="Waiting", executable=pipeline_name
+        )
+        new_task.save()
+
+        task_dict = new_task.__dict__.copy()
+        task_dict.pop("_state", None)
+
+        response_handle = app.send_task(name=task_name, kwargs={"task_id": task_dict["id"], "extra": extra})
+
+        return CeleryTaskRecord(
+            task_dict["id"], task_infos_dict=task_dict, response_handle=response_handle, session=session
+        )
+
 
 class CeleryTaskBackend(BaseTaskBackend):
     app: "Celery"
     task_manager_class = CeleryAlyxTaskManager
 
     def __init__(self, parent: Pipeline, app: "Celery | None" = None):
         super().__init__(parent)
@@ -498,18 +517,25 @@
                     app_task_data["refresh_time"] = now + failed_refresh_retry_time
                 setattr(self, "task_data", app_task_data)
             else:
                 delta = (app_task_data["refresh_time"] - now).total_seconds()
                 logger.warning(f"Returned cached task_data. Next refresh will happen in at least {delta} seconds")
         return app_task_data["task_data"] if app_task_data is not None else None
 
-    def launch_named_task_remotely(self, session_id, task_name, extra=None, kwargs={}):
-        task_record = CeleryTaskRecord.create_from_task_name(
-            self, task_name, app_name, session_id, extra=extra, **kwargs
-        )
+    def launch_named_task_remotely(self, session_id, task_name, task_model=None, extra=None, kwargs={}):
+
+        if task_model is None:
+            task_record = CeleryTaskRecord.create_from_task_name(
+                self, task_name, app_name, session_id, extra=extra, **kwargs
+            )
+        else:
+            task_record = CeleryTaskRecord.create_from_model(
+                self, task_model, task_name, app_name, session_id, extra=extra, **kwargs
+            )
+
         return task_record
 
     def is_hand_shaken(self):
         try:
             result = self.tasks[f"{app_name}.handshake"].delay().get(timeout=1)
             logger.warning(f"Handshake result : {result}")
             return True
```

### Comparing `processing-pypelines-0.0.53/src/pypelines/disk.py` & `processing-pypelines-0.0.54/src/pypelines/disk.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.53/src/pypelines/examples.py` & `processing-pypelines-0.0.54/src/pypelines/examples.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.53/src/pypelines/graphs.py` & `processing-pypelines-0.0.54/src/pypelines/graphs.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.53/src/pypelines/loggs.py` & `processing-pypelines-0.0.54/src/pypelines/loggs.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.53/src/pypelines/multisession.py` & `processing-pypelines-0.0.54/src/pypelines/multisession.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.53/src/pypelines/pickle_backend.py` & `processing-pypelines-0.0.54/src/pypelines/pickle_backend.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.53/src/pypelines/pipelines.py` & `processing-pypelines-0.0.54/src/pypelines/pipelines.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.53/src/pypelines/pipes.py` & `processing-pypelines-0.0.54/src/pypelines/pipes.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.53/src/pypelines/sessions.py` & `processing-pypelines-0.0.54/src/pypelines/sessions.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.53/src/pypelines/steps.py` & `processing-pypelines-0.0.54/src/pypelines/steps.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.53/src/pypelines/tasks.py` & `processing-pypelines-0.0.54/src/pypelines/tasks.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.53/src/pypelines/versions.py` & `processing-pypelines-0.0.54/src/pypelines/versions.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.53/tests/tests.py` & `processing-pypelines-0.0.54/tests/tests.py`

 * *Files identical despite different names*

