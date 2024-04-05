# Comparing `tmp/motion-lake-client-0.0.1.tar.gz` & `tmp/motion-lake-client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion-lake-client-0.0.1.tar", last modified: Fri Apr  5 16:27:43 2024, max compression
+gzip compressed data, was "motion-lake-client-0.0.2.tar", last modified: Fri Apr  5 16:51:46 2024, max compression
```

## Comparing `motion-lake-client-0.0.1.tar` & `motion-lake-client-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-05 16:27:43.782750 motion-lake-client-0.0.1/
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      516 2024-04-05 16:21:57.000000 motion-lake-client-0.0.1/LICENSE
--rw-r--r--   0 gaspard   (1000) gaspard   (1000)     1181 2024-04-05 16:27:43.782750 motion-lake-client-0.0.1/PKG-INFO
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      744 2024-04-05 16:26:52.000000 motion-lake-client-0.0.1/pyproject.toml
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       38 2024-04-05 16:27:43.782750 motion-lake-client-0.0.1/setup.cfg
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       37 2024-04-05 16:27:42.000000 motion-lake-client-0.0.1/setup.py
-drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-05 16:27:43.782750 motion-lake-client-0.0.1/src/
-drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-05 16:27:43.782750 motion-lake-client-0.0.1/src/motion_lake_client/
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       22 2024-04-05 16:23:48.000000 motion-lake-client-0.0.1/src/motion_lake_client/__init__.py
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)     6947 2024-04-05 16:23:48.000000 motion-lake-client-0.0.1/src/motion_lake_client/client.py
-drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-05 16:27:43.782750 motion-lake-client-0.0.1/src/motion_lake_client.egg-info/
--rw-r--r--   0 gaspard   (1000) gaspard   (1000)     1181 2024-04-05 16:27:43.000000 motion-lake-client-0.0.1/src/motion_lake_client.egg-info/PKG-INFO
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      328 2024-04-05 16:27:43.000000 motion-lake-client-0.0.1/src/motion_lake_client.egg-info/SOURCES.txt
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)        1 2024-04-05 16:27:43.000000 motion-lake-client-0.0.1/src/motion_lake_client.egg-info/dependency_links.txt
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)        9 2024-04-05 16:27:43.000000 motion-lake-client-0.0.1/src/motion_lake_client.egg-info/requires.txt
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       19 2024-04-05 16:27:43.000000 motion-lake-client-0.0.1/src/motion_lake_client.egg-info/top_level.txt
+drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-05 16:51:46.381407 motion-lake-client-0.0.2/
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      516 2024-04-05 16:21:57.000000 motion-lake-client-0.0.2/LICENSE
+-rw-r--r--   0 gaspard   (1000) gaspard   (1000)     3024 2024-04-05 16:51:46.381407 motion-lake-client-0.0.2/PKG-INFO
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)     1841 2024-04-05 16:26:12.000000 motion-lake-client-0.0.2/README.md
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      744 2024-04-05 16:51:35.000000 motion-lake-client-0.0.2/pyproject.toml
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       38 2024-04-05 16:51:46.381407 motion-lake-client-0.0.2/setup.cfg
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       37 2024-04-05 16:27:42.000000 motion-lake-client-0.0.2/setup.py
+drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-05 16:51:46.381407 motion-lake-client-0.0.2/src/
+drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-05 16:51:46.381407 motion-lake-client-0.0.2/src/motion_lake_client/
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       22 2024-04-05 16:23:48.000000 motion-lake-client-0.0.2/src/motion_lake_client/__init__.py
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)     7302 2024-04-05 16:48:59.000000 motion-lake-client-0.0.2/src/motion_lake_client/client.py
+drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-05 16:51:46.381407 motion-lake-client-0.0.2/src/motion_lake_client.egg-info/
+-rw-r--r--   0 gaspard   (1000) gaspard   (1000)     3024 2024-04-05 16:51:46.000000 motion-lake-client-0.0.2/src/motion_lake_client.egg-info/PKG-INFO
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      338 2024-04-05 16:51:46.000000 motion-lake-client-0.0.2/src/motion_lake_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)        1 2024-04-05 16:51:46.000000 motion-lake-client-0.0.2/src/motion_lake_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)        9 2024-04-05 16:51:46.000000 motion-lake-client-0.0.2/src/motion_lake_client.egg-info/requires.txt
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       19 2024-04-05 16:51:46.000000 motion-lake-client-0.0.2/src/motion_lake_client.egg-info/top_level.txt
```

### Comparing `motion-lake-client-0.0.1/LICENSE` & `motion-lake-client-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `motion-lake-client-0.0.1/pyproject.toml` & `motion-lake-client-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "motion-lake-client"
-version = "0.0.1"
+version = "0.0.2"
 description = "Motion Lake Client, a client for the Motion Lake API (a Mobility Data Lake)"
 readme = "README.md"
 authors = [{ name = "Gaspard Merten", email = "gaspard.mp.work@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: Other/Proprietary License",
     "Programming Language :: Python",
```

### Comparing `motion-lake-client-0.0.1/src/motion_lake_client/client.py` & `motion-lake-client-0.0.2/src/motion_lake_client/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import dataclasses
 from datetime import datetime
 from typing import Protocol, Dict, Any, List
 
 import requests
 
+__all__ = ['Item', 'Collection', 'NetworkClient', 'RequestsClient', 'InnerClient', 'BaseClient']
+
+
 @dataclasses.dataclass
 class Item:
     """
     A data item in the collection.
     """
     timestamp: datetime
     data: bytes
@@ -62,26 +65,29 @@
         """
         Create a new collection with the given name.
         :param collection_name: The name of the collection to create
         :return: None
         """
         return self.network_client.post(f"/collection/", {"name": collection_name})
 
-    def store(self, collection_name: str, data: bytes, timestamp: int, content_type: str = None) -> dict:
+    def store(self, collection_name: str, data: bytes, timestamp: int, content_type: str = None,
+              create_collection: bool = False) -> dict:
         """
         Store the given data in the collection with the given name.
         :param collection_name: The name of the collection to store the data in
         :param data: The data to store
         :param timestamp: The timestamp to associate with the data
         :param content_type: The type of the data
+        :param create_collection: Whether to create the collection if it does not exist
         :return: None
         """
         return self.network_client.post(
             f"/store/{collection_name}/",
-            {"data": data.hex(), "timestamp": timestamp, "content_type": content_type}
+            {"data": data.hex(), "timestamp": timestamp, "content_type": content_type,
+             "create_collection": create_collection, }
         )
 
     def query(self, collection_name: str, min_timestamp: int, max_timestamp: int, ascending: bool,
               limit: int = None, offset: int = None) -> dict:
         """
         Query the data in the collection with the given name.
         :param collection_name: The name of the collection to query
@@ -142,16 +148,17 @@
             )
             for item in results
         ]
 
     def create_collection(self, collection_name: str) -> dict:
         return self.inner_client.create_collection(collection_name)
 
-    def store(self, collection_name: str, data: bytes, timestamp: int, content_type: str = None) -> dict:
-        return self.inner_client.store(collection_name, data, timestamp, content_type)
+    def store(self, collection_name: str, data: bytes, timestamp: int, content_type: str = None,
+              create_collection: bool = False) -> dict:
+        return self.inner_client.store(collection_name, data, timestamp, content_type, create_collection)
 
     def query(self, collection_name: str, min_timestamp: int, max_timestamp: int, ascending: bool,
               limit: int = None, offset: int = 0) -> dict:
         return self.inner_client.query(collection_name, min_timestamp, max_timestamp, ascending, limit, offset)
 
     def get_last_items(self, collection_name: str, limit: int) -> List[Item]:
         response = self.query(collection_name, 0, int(datetime.now().timestamp()), False, limit)
```

