# Comparing `tmp/eswrap-0.5.1.tar.gz` & `tmp/eswrap-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eswrap-0.5.1.tar", last modified: Tue Oct 10 08:25:42 2023, max compression
+gzip compressed data, was "eswrap-0.5.2.tar", last modified: Fri Apr  5 06:35:41 2024, max compression
```

## Comparing `eswrap-0.5.1.tar` & `eswrap-0.5.2.tar`

### file list

```diff
@@ -1,19 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 08:25:42.264227 eswrap-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2023-10-10 08:25:42.264227 eswrap-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-10 08:25:28.000000 eswrap-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 08:25:42.264227 eswrap-0.5.1/eswrap/
--rw-r--r--   0 runner    (1001) docker     (127)    34509 2023-10-10 08:25:28.000000 eswrap-0.5.1/eswrap/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-10 08:25:41.000000 eswrap-0.5.1/eswrap/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2023-10-10 08:25:28.000000 eswrap-0.5.1/eswrap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 08:25:42.264227 eswrap-0.5.1/eswrap/common/
--rw-r--r--   0 runner    (1001) docker     (127)     8180 2023-10-10 08:25:28.000000 eswrap-0.5.1/eswrap/common/EsHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-10 08:25:28.000000 eswrap-0.5.1/eswrap/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5053 2023-10-10 08:25:28.000000 eswrap-0.5.1/eswrap/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 08:25:42.264227 eswrap-0.5.1/eswrap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2023-10-10 08:25:42.000000 eswrap-0.5.1/eswrap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      284 2023-10-10 08:25:42.000000 eswrap-0.5.1/eswrap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-10 08:25:42.000000 eswrap-0.5.1/eswrap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-10 08:25:42.000000 eswrap-0.5.1/eswrap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-10 08:25:42.000000 eswrap-0.5.1/eswrap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-10 08:25:42.264227 eswrap-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2023-10-10 08:25:28.000000 eswrap-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:35:41.182516 eswrap-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-05 06:35:41.182516 eswrap-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 06:35:31.000000 eswrap-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:35:41.178516 eswrap-0.5.2/eswrap/
+-rw-r--r--   0 runner    (1001) docker     (127)    34509 2024-04-05 06:35:31.000000 eswrap-0.5.2/eswrap/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-05 06:35:41.000000 eswrap-0.5.2/eswrap/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-05 06:35:31.000000 eswrap-0.5.2/eswrap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:35:41.178516 eswrap-0.5.2/eswrap/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 06:35:31.000000 eswrap-0.5.2/eswrap/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:35:41.178516 eswrap-0.5.2/eswrap/core/es_handler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 06:35:31.000000 eswrap-0.5.2/eswrap/core/es_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14157 2024-04-05 06:35:31.000000 eswrap-0.5.2/eswrap/core/es_handler/es_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:35:41.178516 eswrap-0.5.2/eswrap/core/es_index/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 06:35:31.000000 eswrap-0.5.2/eswrap/core/es_index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-05 06:35:31.000000 eswrap-0.5.2/eswrap/core/es_index/es_index.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:35:41.178516 eswrap-0.5.2/eswrap/core/index_list/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 06:35:31.000000 eswrap-0.5.2/eswrap/core/index_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-05 06:35:31.000000 eswrap-0.5.2/eswrap/core/index_list/index_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:35:41.178516 eswrap-0.5.2/eswrap/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 06:35:31.000000 eswrap-0.5.2/eswrap/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-05 06:35:31.000000 eswrap-0.5.2/eswrap/errors/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-05 06:35:31.000000 eswrap-0.5.2/eswrap/errors/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-04-05 06:35:31.000000 eswrap-0.5.2/eswrap/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:35:41.182516 eswrap-0.5.2/eswrap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-05 06:35:41.000000 eswrap-0.5.2/eswrap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-05 06:35:41.000000 eswrap-0.5.2/eswrap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 06:35:41.000000 eswrap-0.5.2/eswrap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-05 06:35:41.000000 eswrap-0.5.2/eswrap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 06:35:41.000000 eswrap-0.5.2/eswrap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 06:35:41.182516 eswrap-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-05 06:35:31.000000 eswrap-0.5.2/setup.py
```

### Comparing `eswrap-0.5.1/PKG-INFO` & `eswrap-0.5.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: eswrap
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python wrapper for simple elasticsearch queries
 Home-page: 
 Author: Paul Tikken
 Author-email: paul.tikken@gmail.com
 License: GNU General Public License v3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Requires-Dist: elasticsearch>=8.10.0
 
 # ESWRAP
```

### Comparing `eswrap-0.5.1/eswrap/LICENSE` & `eswrap-0.5.2/eswrap/LICENSE`

 * *Files identical despite different names*

### Comparing `eswrap-0.5.1/eswrap/__init__.py` & `eswrap-0.5.2/eswrap/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import re
 import subprocess
 
 from .main import EsWrap
 
-
 _PKG_DIR = os.path.dirname(__file__)
 
 
 def _version_from_git_describe():
     """
 
     Read the version from ``git describe``. It returns the latest tag with an
```

### Comparing `eswrap-0.5.1/eswrap/main.py` & `eswrap-0.5.2/eswrap/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+import collections
 import logging
 import os
-from typing import Optional
+from typing import Optional, List
 
-import elastic_transport
 import urllib3
 from elasticsearch import Elasticsearch
 from urllib3.exceptions import InsecureRequestWarning
 
-from eswrap.common.EsHandler import EsHandler
+from eswrap.core.es_handler.es_handler import EsHandler
+from eswrap.core.es_index.es_index import EsIndex
+from eswrap.core.index_list.index_list import IndexList
+from eswrap.errors.indexes import IndexNotFoundError
 
 urllib3.disable_warnings(InsecureRequestWarning)
 
 try:
     from version import VERSION
 except ModuleNotFoundError:
     _PKG_DIR = os.path.dirname(__file__)
@@ -23,14 +26,15 @@
 class EsWrap(object):
     def __init__(
         self,
         host: str = "localhost",
         port: int = 9200,
         scheme: str = "http",
         connection_details: list[str] | list[dict] = None,
+        auto_init_index_handlers: bool = False,
         **kwargs,
     ):
         """
         connection_details should facilitate all connection options as stated in the API documentation of the
         Elasticsearch library.
         E.g.
         [
@@ -56,73 +60,94 @@
         else:
             self.connection_details = connection_details
 
         self.logger = logging.getLogger(__name__)
 
         self.__es_client = Elasticsearch(self.connection_details, **kwargs)
 
-        try:
-            for each in self.__es_client.indices.get(index="*").keys():
-                if not each.startswith("."):
-                    setattr(
-                        self,
-                        each,
-                        EsHandler(es_connection=self.__es_client, index=each),
-                    )
-                else:
-                    # workaround for handling system indexes; needs further troubleshooting
-                    setattr(
-                        self,
-                        each[1:].split("-")[0],
-                        EsHandler(es_connection=self.__es_client, index=each),
-                    )
-        except elastic_transport.ConnectionError as err:
-            self.logger.warning(
-                f"Cannot connect to elasticsearch, error encountered: {err}"
-            )
-        except Exception as err:
-            self.logger.error(f"Uncaught exception encountered: {err}")
+        self.__index_list = IndexList(es_client=self.es_client)
+        self.__index_dict = {}
+        self.__indexes = []
+
+        if auto_init_index_handlers:
+            self.setup_handlers_for_indexes()
 
     @property
     def es_client(self):
         return self.__es_client
 
     @property
     def version(self):
         """Property returning current version"""
         return self.__version
 
     @property
-    def indices(self):
-        return list(self.es_client.indices.get(index="*").keys())
+    def index_list(self) -> IndexList:
+        return self.__index_list
+
+    @property
+    def index_dict(self) -> dict:
+        return self.__index_dict
+
+    @index_dict.setter
+    def index_dict(self, val: dict) -> None:
+        self.__index_dict = val
+
+    @property
+    def indexes(self) -> List[EsIndex]:
+        return self.index_list.indexes
 
     @property
     def info(self):
         return self.es_client.info()
 
+    def get_index_handler(self, index_name: str) -> EsHandler:
+        if len(self.indexes) == 0:
+            self.setup_handlers_for_indexes()
+
+        try:
+            index_handler = [
+                x for x in self.index_list.indexes if x.name == index_name
+            ][0]()
+            return index_handler
+        except IndexError:
+            raise IndexNotFoundError
+
+    def setup_handlers_for_indexes(self):
+        self.index_list.fill_index_list()
+
+        index_coldict = collections.defaultdict()
+
+        for index in self.indexes:
+            index_coldict[index.name] = index
+
+        self.index_dict = dict(index_coldict)
+
     def index(self, index_name: str, data: dict, doc_id: Optional[str] = None):
-        if not hasattr(self, index_name):
-            setattr(
-                self,
-                index_name,
-                EsHandler(es_connection=self.__es_client, index=index_name),
-            )
 
-        return self.es_client.index(index=index_name, document=data, id=doc_id)
+        ret_data = self.es_client.index(index=index_name, document=data, id=doc_id)
+
+        if index_name not in self.index_dict.keys():
+            self.setup_handlers_for_indexes()
+
+        return ret_data
+
+    def search(self, index_name: str):
+
+        return self.get_index_handler(index_name).search()
 
     def delete_index(self, index_name: str):
 
         ret_val = self.es_client.options(ignore_status=[400, 404]).indices.delete(
             index=index_name
         )
 
         try:
             if ret_val["acknowledged"]:
-                if hasattr(self, index_name):
-                    delattr(self, index_name)
+                self.setup_handlers_for_indexes()
                 return True
         except KeyError:
             # failed somehow, assuming the given index does not exist
             self.logger.warning(
                 f"The index {index_name} cannot not be deleted; reason -> {ret_val}"
             )
         except Exception as err:
@@ -134,30 +159,25 @@
 
         ret_val = self.es_client.options(ignore_status=[400, 404]).indices.create(
             index=index_name
         )
 
         try:
             if ret_val["acknowledged"]:
-                if not hasattr(self, index_name):
-                    setattr(
-                        self,
-                        index_name,
-                        EsHandler(es_connection=self.__es_client, index=index_name),
-                    )
+                self.setup_handlers_for_indexes()
                 return True
         except KeyError:
             # failed somehow, assuming the given index does not exist
             self.logger.warning(
                 f"The index {index_name} cannot not be created; reason -> {ret_val}"
             )
         except Exception as err:
             self.logger.error(f"Uncaught exception encountered: {err}")
 
         return False
 
     def __del__(self):
-        self.__es_client.close()
+        self.es_client.close()
 
     def __repr__(self):
         """String representation of object"""
         return "<< EsWrap:{} >>".format(self.version)
```

### Comparing `eswrap-0.5.1/eswrap.egg-info/PKG-INFO` & `eswrap-0.5.2/eswrap.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: eswrap
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python wrapper for simple elasticsearch queries
 Home-page: 
 Author: Paul Tikken
 Author-email: paul.tikken@gmail.com
 License: GNU General Public License v3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Requires-Dist: elasticsearch>=8.10.0
 
 # ESWRAP
```

### Comparing `eswrap-0.5.1/setup.py` & `eswrap-0.5.2/setup.py`

 * *Files identical despite different names*

