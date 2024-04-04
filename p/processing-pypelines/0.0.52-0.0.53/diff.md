# Comparing `tmp/processing-pypelines-0.0.52.tar.gz` & `tmp/processing-pypelines-0.0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processing-pypelines-0.0.52.tar", last modified: Thu Apr  4 21:28:55 2024, max compression
+gzip compressed data, was "processing-pypelines-0.0.53.tar", last modified: Thu Apr  4 21:45:29 2024, max compression
```

## Comparing `processing-pypelines-0.0.52.tar` & `processing-pypelines-0.0.53.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:28:55.686454 processing-pypelines-0.0.52/
--rw-rw-rw-   0 root         (0) root         (0)     1073 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 21:28:55.682454 processing-pypelines-0.0.52/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1132 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/requirements-celery.txt
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 21:28:55.686454 processing-pypelines-0.0.52/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:28:55.678454 processing-pypelines-0.0.52/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:28:55.682454 processing-pypelines-0.0.52/src/processing_pypelines.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 21:28:55.000000 processing-pypelines-0.0.52/src/processing_pypelines.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      742 2024-04-04 21:28:55.000000 processing-pypelines-0.0.52/src/processing_pypelines.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 21:28:55.000000 processing-pypelines-0.0.52/src/processing_pypelines.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      306 2024-04-04 21:28:55.000000 processing-pypelines-0.0.52/src/processing_pypelines.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-04 21:28:55.000000 processing-pypelines-0.0.52/src/processing_pypelines.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:28:55.682454 processing-pypelines-0.0.52/src/pypelines/
--rw-rw-rw-   0 root         (0) root         (0)      206 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2365 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/accessors.py
--rw-rw-rw-   0 root         (0) root         (0)     3191 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/arguments.py
--rw-rw-rw-   0 root         (0) root         (0)    21250 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/celery_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     7301 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/disk.py
--rw-rw-rw-   0 root         (0) root         (0)     2901 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/examples.py
--rw-rw-rw-   0 root         (0) root         (0)     4650 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/graphs.py
--rw-rw-rw-   0 root         (0) root         (0)    15517 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/loggs.py
--rw-rw-rw-   0 root         (0) root         (0)     3386 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/multisession.py
--rw-rw-rw-   0 root         (0) root         (0)    14910 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/pickle_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     5461 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/pipelines.py
--rw-rw-rw-   0 root         (0) root         (0)     5669 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/pipes.py
--rw-rw-rw-   0 root         (0) root         (0)     1692 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/sessions.py
--rw-rw-rw-   0 root         (0) root         (0)    29008 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/steps.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     4326 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/versions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:28:55.682454 processing-pypelines-0.0.52/tests/
--rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/tests/tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:45:29.278367 processing-pypelines-0.0.53/
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 21:45:29.274367 processing-pypelines-0.0.53/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1132 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/requirements-celery.txt
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 21:45:29.278367 processing-pypelines-0.0.53/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:45:29.270367 processing-pypelines-0.0.53/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:45:29.274367 processing-pypelines-0.0.53/src/processing_pypelines.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 21:45:29.000000 processing-pypelines-0.0.53/src/processing_pypelines.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      742 2024-04-04 21:45:29.000000 processing-pypelines-0.0.53/src/processing_pypelines.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 21:45:29.000000 processing-pypelines-0.0.53/src/processing_pypelines.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      306 2024-04-04 21:45:29.000000 processing-pypelines-0.0.53/src/processing_pypelines.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-04 21:45:29.000000 processing-pypelines-0.0.53/src/processing_pypelines.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:45:29.274367 processing-pypelines-0.0.53/src/pypelines/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2365 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/accessors.py
+-rw-rw-rw-   0 root         (0) root         (0)     3191 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/arguments.py
+-rw-rw-rw-   0 root         (0) root         (0)    21401 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/celery_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     7301 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/disk.py
+-rw-rw-rw-   0 root         (0) root         (0)     2901 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     4650 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/graphs.py
+-rw-rw-rw-   0 root         (0) root         (0)    15517 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/loggs.py
+-rw-rw-rw-   0 root         (0) root         (0)     3386 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/multisession.py
+-rw-rw-rw-   0 root         (0) root         (0)    14910 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/pickle_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     5461 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/pipelines.py
+-rw-rw-rw-   0 root         (0) root         (0)     5669 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/pipes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1692 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/sessions.py
+-rw-rw-rw-   0 root         (0) root         (0)    29008 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/steps.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     4326 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/src/pypelines/versions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:45:29.274367 processing-pypelines-0.0.53/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-04 21:45:19.000000 processing-pypelines-0.0.53/tests/tests.py
```

### Comparing `processing-pypelines-0.0.52/LICENSE` & `processing-pypelines-0.0.53/LICENSE`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.52/PKG-INFO` & `processing-pypelines-0.0.53/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processing-pypelines
-Version: 0.0.52
+Version: 0.0.53
 Summary: Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api
 Author-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 Maintainer-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 License: MIT
 Project-URL: homepage, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: repository, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: documentation, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
```

### Comparing `processing-pypelines-0.0.52/pyproject.toml` & `processing-pypelines-0.0.53/pyproject.toml`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.52/src/processing_pypelines.egg-info/PKG-INFO` & `processing-pypelines-0.0.53/src/processing_pypelines.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processing-pypelines
-Version: 0.0.52
+Version: 0.0.53
 Summary: Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api
 Author-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 Maintainer-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 License: MIT
 Project-URL: homepage, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: repository, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: documentation, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
```

### Comparing `processing-pypelines-0.0.52/src/processing_pypelines.egg-info/SOURCES.txt` & `processing-pypelines-0.0.53/src/processing_pypelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.52/src/pypelines/accessors.py` & `processing-pypelines-0.0.53/src/pypelines/accessors.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.52/src/pypelines/arguments.py` & `processing-pypelines-0.0.53/src/pypelines/arguments.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.52/src/pypelines/celery_tasks.py` & `processing-pypelines-0.0.53/src/pypelines/celery_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -447,26 +447,28 @@
             for worker, tasks in registered_tasks.items():
                 workers.append(worker)
                 for task in tasks:
                     task_names.append(task)
 
         return {"workers": workers, "task_names": task_names}
 
-    def get_celery_app_tasks(self, refresh=False):
+    def get_celery_app_tasks(
+        self, refresh=False, auto_refresh=3600 * 24, failed_refresh=60 * 5, initial_timeout=10, refresh_timeout=2
+    ):
 
         from datetime import datetime, timedelta
 
-        auto_refresh_time = timedelta(0, (3600 * 24))  # a full day (24 hours of 3600 seconds)
-        failed_refresh_retry_time = timedelta(0, (60 * 5))  # try to refresh after 5 minutes
+        auto_refresh_time = timedelta(0, seconds=auto_refresh)  # a full day (24 hours of 3600 seconds)
+        failed_refresh_retry_time = timedelta(0, failed_refresh)  # try to refresh after 5 minutes
 
         app_task_data = getattr(self, "task_data", None)
 
         if app_task_data is None:
             try:
-                task_data = self.tasks[f"{app_name}.tasks_infos"].delay(app_name).get(timeout=10)
+                task_data = self.tasks[f"{app_name}.tasks_infos"].delay(app_name).get(timeout=initial_timeout)
                 # we set timeout to 10 sec if the task data doesn't exist.
                 # It's long to wait for a webpage to load, but sometimes the workers take time to come out of sleep
                 app_task_data = {"task_data": task_data, "refresh_time": datetime.now() + auto_refresh_time}
                 setattr(self, "task_data", app_task_data)
                 logger.warning("Got tasks data for the first time since django server relaunched")
             except Exception as e:
                 logger.warning(f"Could not get tasks from app. {e}")
@@ -480,15 +482,15 @@
                     "Time has come to auto refresh app_task_data. "
                     f"refresh_time was {app_task_data['refresh_time']} and now is {now}"
                 )
                 refresh = True
 
             if refresh:
                 try:
-                    task_data = self.tasks[f"{app_name}.tasks_infos"].delay(app_name).get(timeout=2)
+                    task_data = self.tasks[f"{app_name}.tasks_infos"].delay(app_name).get(timeout=refresh_timeout)
                     # if the data needs to be refreshed, we don't wait for as long as for a first get of infos.
                     app_task_data = {"task_data": task_data, "refresh_time": now + auto_refresh_time}
                     logger.warning("Refreshed celery tasks data sucessfully")
                 except Exception as e:
                     logger.warning(
                         "Could not refresh tasks data from remote celery worker. All workers are is probably running. "
                         f"{e}"
@@ -507,16 +509,16 @@
         return task_record
 
     def is_hand_shaken(self):
         try:
             result = self.tasks[f"{app_name}.handshake"].delay().get(timeout=1)
             logger.warning(f"Handshake result : {result}")
             return True
-        except ValueError:
-            logger.error("No handshake result. All workers are busy ?")
+        except Exception as e:
+            logger.error(f"No handshake result. All workers are busy ? {e}")
             return False
 
     settings_files = get_setting_files_path(conf_path)
 
     if len(settings_files) == 0:
         logger.warning(f"{failure_message} Could not find celery toml config files.")
         return None
```

### Comparing `processing-pypelines-0.0.52/src/pypelines/disk.py` & `processing-pypelines-0.0.53/src/pypelines/disk.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.52/src/pypelines/examples.py` & `processing-pypelines-0.0.53/src/pypelines/examples.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.52/src/pypelines/graphs.py` & `processing-pypelines-0.0.53/src/pypelines/graphs.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.52/src/pypelines/loggs.py` & `processing-pypelines-0.0.53/src/pypelines/loggs.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.52/src/pypelines/multisession.py` & `processing-pypelines-0.0.53/src/pypelines/multisession.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.52/src/pypelines/pickle_backend.py` & `processing-pypelines-0.0.53/src/pypelines/pickle_backend.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.52/src/pypelines/pipelines.py` & `processing-pypelines-0.0.53/src/pypelines/pipelines.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.52/src/pypelines/pipes.py` & `processing-pypelines-0.0.53/src/pypelines/pipes.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.52/src/pypelines/sessions.py` & `processing-pypelines-0.0.53/src/pypelines/sessions.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.52/src/pypelines/steps.py` & `processing-pypelines-0.0.53/src/pypelines/steps.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.52/src/pypelines/tasks.py` & `processing-pypelines-0.0.53/src/pypelines/tasks.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.52/src/pypelines/versions.py` & `processing-pypelines-0.0.53/src/pypelines/versions.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.52/tests/tests.py` & `processing-pypelines-0.0.53/tests/tests.py`

 * *Files identical despite different names*

