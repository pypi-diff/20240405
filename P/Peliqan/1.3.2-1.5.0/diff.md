# Comparing `tmp/Peliqan-1.3.2.tar.gz` & `tmp/Peliqan-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Peliqan-1.3.2.tar", last modified: Thu Mar  7 13:23:49 2024, max compression
+gzip compressed data, was "Peliqan-1.5.0.tar", last modified: Fri Apr  5 12:54:53 2024, max compression
```

## Comparing `Peliqan-1.3.2.tar` & `Peliqan-1.5.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-03-07 13:23:49.945353 Peliqan-1.3.2/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2024-03-07 13:23:49.945218 Peliqan-1.3.2/PKG-INFO
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-03-07 13:23:49.941277 Peliqan-1.3.2/Peliqan.egg-info/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2024-03-07 13:23:49.000000 Peliqan-1.3.2/Peliqan.egg-info/PKG-INFO
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      415 2024-03-07 13:23:49.000000 Peliqan-1.3.2/Peliqan.egg-info/SOURCES.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        1 2024-03-07 13:23:49.000000 Peliqan-1.3.2/Peliqan.egg-info/dependency_links.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       16 2024-03-07 13:23:49.000000 Peliqan-1.3.2/Peliqan.egg-info/requires.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        8 2024-03-07 13:23:49.000000 Peliqan-1.3.2/Peliqan.egg-info/top_level.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1411 2023-08-02 11:35:09.000000 Peliqan-1.3.2/README.md
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-03-07 13:23:49.942427 Peliqan-1.3.2/peliqan/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      872 2024-03-07 11:43:04.000000 Peliqan-1.3.2/peliqan/__init__.py
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-03-07 13:23:49.944692 Peliqan-1.3.2/peliqan/client/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      421 2023-11-07 06:42:14.000000 Peliqan-1.3.2/peliqan/client/__init__.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    15079 2024-02-10 08:34:52.000000 Peliqan-1.3.2/peliqan/client/backend_service.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     2657 2024-02-19 09:48:17.000000 Peliqan-1.3.2/peliqan/client/base.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    10609 2024-03-07 11:43:04.000000 Peliqan-1.3.2/peliqan/client/dbclient.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      928 2023-09-12 06:13:12.000000 Peliqan-1.3.2/peliqan/client/sftpclient.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     4664 2023-12-14 11:19:29.000000 Peliqan-1.3.2/peliqan/client/writeback.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    25740 2024-02-12 11:08:52.000000 Peliqan-1.3.2/peliqan/core.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      393 2024-02-16 11:30:10.000000 Peliqan-1.3.2/peliqan/exceptions.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       23 2024-02-12 11:08:52.000000 Peliqan-1.3.2/peliqan/utils.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       38 2024-03-07 13:23:49.945404 Peliqan-1.3.2/setup.cfg
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1371 2024-02-19 09:48:17.000000 Peliqan-1.3.2/setup.py
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-04-05 12:54:53.420385 Peliqan-1.5.0/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2024-04-05 12:54:53.420256 Peliqan-1.5.0/PKG-INFO
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-04-05 12:54:53.416301 Peliqan-1.5.0/Peliqan.egg-info/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2024-04-05 12:54:53.000000 Peliqan-1.5.0/Peliqan.egg-info/PKG-INFO
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      437 2024-04-05 12:54:53.000000 Peliqan-1.5.0/Peliqan.egg-info/SOURCES.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        1 2024-04-05 12:54:53.000000 Peliqan-1.5.0/Peliqan.egg-info/dependency_links.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       16 2024-04-05 12:54:53.000000 Peliqan-1.5.0/Peliqan.egg-info/requires.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        8 2024-04-05 12:54:53.000000 Peliqan-1.5.0/Peliqan.egg-info/top_level.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1411 2023-08-02 11:35:09.000000 Peliqan-1.5.0/README.md
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-04-05 12:54:53.418156 Peliqan-1.5.0/peliqan/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      872 2024-04-05 12:21:53.000000 Peliqan-1.5.0/peliqan/__init__.py
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-04-05 12:54:53.419964 Peliqan-1.5.0/peliqan/client/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      421 2023-11-07 06:42:14.000000 Peliqan-1.5.0/peliqan/client/__init__.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    15754 2024-04-05 12:21:53.000000 Peliqan-1.5.0/peliqan/client/backend_service.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     2657 2024-02-19 09:48:17.000000 Peliqan-1.5.0/peliqan/client/base.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    10609 2024-03-13 12:08:36.000000 Peliqan-1.5.0/peliqan/client/dbclient.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      928 2023-09-12 06:13:12.000000 Peliqan-1.5.0/peliqan/client/sftpclient.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     4549 2024-04-05 12:21:53.000000 Peliqan-1.5.0/peliqan/client/writeback.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    26493 2024-04-05 12:21:53.000000 Peliqan-1.5.0/peliqan/core.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      393 2024-02-16 11:30:10.000000 Peliqan-1.5.0/peliqan/exceptions.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    20342 2024-03-21 07:17:47.000000 Peliqan-1.5.0/peliqan/local_test.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       23 2024-02-12 11:08:52.000000 Peliqan-1.5.0/peliqan/utils.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       38 2024-04-05 12:54:53.420456 Peliqan-1.5.0/setup.cfg
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1371 2024-02-19 09:48:17.000000 Peliqan-1.5.0/setup.py
```

### Comparing `Peliqan-1.3.2/PKG-INFO` & `Peliqan-1.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Peliqan
-Version: 1.3.2
+Version: 1.5.0
 Summary: This package is an sdk that allows any python client to connect with a Peliqan environment.
 Home-page: https://peliqan.io/
 Author: Peliqan.io
 Author-email: dev@peliqan.io
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Peliqan-1.3.2/Peliqan.egg-info/PKG-INFO` & `Peliqan-1.5.0/Peliqan.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Peliqan
-Version: 1.3.2
+Version: 1.5.0
 Summary: This package is an sdk that allows any python client to connect with a Peliqan environment.
 Home-page: https://peliqan.io/
 Author: Peliqan.io
 Author-email: dev@peliqan.io
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Peliqan-1.3.2/README.md` & `Peliqan-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `Peliqan-1.3.2/peliqan/__init__.py` & `Peliqan-1.5.0/peliqan/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.3.2"
+__version__ = "1.5.0"
 __author__ = 'Peliqan.io'
 __credits__ = 'Peliqan.io'
 
 __all__ = [
     "Peliqan",
     "BasePeliqanClient"
 ]
```

### Comparing `Peliqan-1.3.2/peliqan/client/backend_service.py` & `Peliqan-1.5.0/peliqan/client/backend_service.py`

 * *Files 9% similar despite different names*

```diff
@@ -314,14 +314,19 @@
         return response_dict
 
     def get_databases(self):
         url = f"{self.BACKEND_URL}/api/applications"
         response_dict = self.call_backend("get", url)
         return response_dict
 
+    def get_table(self, table_id):
+        url = f"{self.BACKEND_URL}/api/database/tables/{table_id}/"
+        response_dict = self.call_backend("get", url)
+        return response_dict
+
     def update_table(self, id, name=None, table_type=None, query=None, external=None, primary_field_id=None,
                      settings=None):
         url = f"{self.BACKEND_URL}/api/database/tables/%s/" % id
         data = {}
         if name:
             data["name"] = name
         if table_type:
@@ -376,10 +381,20 @@
         return data.get('state', '')
 
     def set_interface_state(self, interface_id, state):
         url = f"{self.BACKEND_URL}/api/interfaces/{interface_id}/"
         data = {'state': state}
         return self.call_backend("patch", url, json=data)
 
-    def get_logs(self, connection_id):
-        url = f"{self.BACKEND_URL}/api/servers/{connection_id}/logs"
+    def get_pipeline_logs(self, pipeline_run_id):
+        if not pipeline_run_id:
+            raise PeliqanClientException("'pipeline_run_id' must be provided")
+
+        url = f"{self.BACKEND_URL}/api/pipeline_runs/{pipeline_run_id}/logs"
+        return self.call_backend("get", url)
+
+    def get_pipeline_runs(self, connection_id=None, page=1, per_page=10):
+        if connection_id:
+            url = f"{self.BACKEND_URL}/api/servers/{connection_id}/runs/?page={page}&per_page={per_page}"
+        else:
+            url = f"{self.BACKEND_URL}/api/pipeline_runs/?page={page}&per_page={per_page}"
         return self.call_backend("get", url)
```

### Comparing `Peliqan-1.3.2/peliqan/client/base.py` & `Peliqan-1.5.0/peliqan/client/base.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.3.2/peliqan/client/dbclient.py` & `Peliqan-1.5.0/peliqan/client/dbclient.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.3.2/peliqan/client/sftpclient.py` & `Peliqan-1.5.0/peliqan/client/sftpclient.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.3.2/peliqan/client/writeback.py` & `Peliqan-1.5.0/peliqan/client/writeback.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,20 @@
         kwargs = self.args_to_kwargs(args, kwargs)
         response_dict = self.request_endpoint_via_proxy(object_name, 'get', **kwargs)
         if "detail" in response_dict:
             return response_dict["detail"]
         else:
             return response_dict
 
-    def findone(self, object_name, **kwargs):
+    def findone(self, object_name, *args, **kwargs):
+        kwargs = self.args_to_kwargs(args, kwargs)
         if "searchterm" not in kwargs:
             raise PeliqanClientException(
-                f"Parameter searchterm is required and searchfield is sometimes required for function 'findone'.")
+                f"Parameter searchterm is required and searchfield is sometimes required for function 'findone'."
+            )
         response_dict = self.request_endpoint_via_proxy(object_name, 'findone', **kwargs)
         if "detail" in response_dict:
             detail = response_dict["detail"]
             if not isinstance(detail, dict):  # replace empty string response "" (if no record found) with {}
                 detail = {}
             return detail
         else:
@@ -63,17 +65,15 @@
         # pq.update("contact", name='John', city='NY') or pq.update("contact", contact_obj)
         kwargs = self.args_to_kwargs(args, kwargs)
         if "searchterm" not in kwargs:
             raise PeliqanClientException(
                 f"Parameter searchterm is required and searchfield is sometimes required for function 'upsert'.")
         if "searchfield" not in kwargs:
             kwargs["searchfield"] = None
-        response_dict_findone = self.request_endpoint_via_proxy(object_name, 'findone',
-                                                                searchfield=kwargs["searchfield"],
-                                                                searchterm=kwargs["searchterm"])
+        response_dict_findone = self.request_endpoint_via_proxy(object_name, 'findone', **kwargs)
         kwargs.pop('searchfield', None)
         kwargs.pop('searchterm', None)
         if "detail" in response_dict_findone and "id" in response_dict_findone["detail"]:
             kwargs["id"] = response_dict_findone["detail"]["id"]
             response_dict = self.request_endpoint_via_proxy(object_name, 'update', **kwargs)
         else:
             response_dict = self.request_endpoint_via_proxy(object_name, 'add', **kwargs)
```

### Comparing `Peliqan-1.3.2/peliqan/core.py` & `Peliqan-1.5.0/peliqan/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
             )
             field_name = lookup_data['table_id']['field_name']
 
         if not field_name:
             raise PeliqanClientException("field_id or field_name must be provided as kwargs")
 
         # set the final url
-        if type(table_id) != int:
+        if isinstance(table_id, int):
             raise PeliqanClientException("table_id could not be resolved, please check provided arguments.")
 
         # set table_id to base url
         url = base_url % table_id
 
         data = {
             'pk': row_pk,
@@ -179,14 +179,15 @@
                 interval = 10
 
             response = refresh_func()
             running = response.get('running', True)
             if not running:
                 return {
                     'task_id': response['task_id'],
+                    'run_id': response['run_id'],
                     'detail': 'The sync task has completed.',
                     'syncing': False
                 }
 
             time.sleep(interval)
             count += 1
 
@@ -414,14 +415,22 @@
         """
         Returns a list of all databases in the account including tables and fields in tables.
 
         :return: list of databases
         """
         return self.__service_client__.get_databases()
 
+    def get_table(self, table_id):
+        """
+            Returns all meta-data for a table including fields.
+
+            :return: list of databases
+        """
+        return self.__service_client__.get_table(table_id)
+
     def update_field(self, id, description=None, tags=None):
         """
         Updates a field (column).
 
         :param id: required, integer, id of the field to update
         :param description: optional, string, description of the field (data catalog metadata)
         :param tags: optional, array of strings, tags assigned to the field (data catalog metadata)
@@ -554,15 +563,27 @@
 
         :param interface_id: The id of the interface.
         :param state: The data that will be stored as the state value for an interface.
         :return:
         """
         return self.__service_client__.set_interface_state(interface_id, state)
 
-    def get_logs(self, connection_id):
+    def get_pipeline_logs(self, pipeline_run_id):
         """
         Retrieves the pipeline logs of a SaaS connection.
 
-        :param connection_id: required, integer, id of the source connection.
+        :param pipeline_run_id: id of the pipeline run.
+
         :return: logs of the pipeline
         """
-        return self.__service_client__.get_logs(connection_id)
+        return self.__service_client__.get_pipeline_logs(pipeline_run_id)
+
+    def get_pipeline_runs(self, connection_id=None, page=1, per_page=10):
+        """
+        Retrieves the pipeline logs of a SaaS connection.
+
+        :param connection_id: integer, id of the source connection.
+        :param page: integer, the page number to fetch.
+        :param per_page: integer, the number of results per page.
+        :return: list of pipeline runs
+        """
+        return self.__service_client__.get_pipeline_runs(connection_id, page, per_page)
```

### Comparing `Peliqan-1.3.2/setup.py` & `Peliqan-1.5.0/setup.py`

 * *Files identical despite different names*

