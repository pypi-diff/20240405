# Comparing `tmp/hyperon_das_atomdb-0.6.3.tar.gz` & `tmp/hyperon_das_atomdb-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperon_das_atomdb-0.6.3.tar", max compression
+gzip compressed data, was "hyperon_das_atomdb-0.6.4.tar", max compression
```

## Comparing `hyperon_das_atomdb-0.6.3.tar` & `hyperon_das_atomdb-0.6.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1081 2024-04-04 20:08:15.849037 hyperon_das_atomdb-0.6.3/LICENCE
--rw-r--r--   0        0        0     2687 2024-04-04 20:08:15.849037 hyperon_das_atomdb-0.6.3/README.md
--rw-r--r--   0        0        0      306 2024-04-04 20:08:15.853037 hyperon_das_atomdb-0.6.3/hyperon_das_atomdb/__init__.py
--rw-r--r--   0        0        0      116 2024-04-04 20:08:15.853037 hyperon_das_atomdb-0.6.3/hyperon_das_atomdb/adapters/__init__.py
--rw-r--r--   0        0        0    20316 2024-04-04 20:08:15.853037 hyperon_das_atomdb-0.6.3/hyperon_das_atomdb/adapters/ram_only.py
--rw-r--r--   0        0        0    36893 2024-04-04 20:08:15.853037 hyperon_das_atomdb-0.6.3/hyperon_das_atomdb/adapters/redis_mongo_db.py
--rw-r--r--   0        0        0    19708 2024-04-04 20:08:15.853037 hyperon_das_atomdb-0.6.3/hyperon_das_atomdb/database.py
--rw-r--r--   0        0        0      877 2024-04-04 20:08:15.853037 hyperon_das_atomdb-0.6.3/hyperon_das_atomdb/exceptions.py
--rw-r--r--   0        0        0     1122 2024-04-04 20:08:15.853037 hyperon_das_atomdb-0.6.3/hyperon_das_atomdb/index.py
--rw-r--r--   0        0        0     1052 2024-04-04 20:08:15.853037 hyperon_das_atomdb-0.6.3/hyperon_das_atomdb/logger.py
--rw-r--r--   0        0        0        0 2024-04-04 20:08:15.853037 hyperon_das_atomdb-0.6.3/hyperon_das_atomdb/utils/__init__.py
--rw-r--r--   0        0        0     1947 2024-04-04 20:08:15.853037 hyperon_das_atomdb-0.6.3/hyperon_das_atomdb/utils/expression_hasher.py
--rw-r--r--   0        0        0     1388 2024-04-04 20:08:15.853037 hyperon_das_atomdb-0.6.3/hyperon_das_atomdb/utils/patterns.py
--rw-r--r--   0        0        0       65 2024-04-04 20:08:15.853037 hyperon_das_atomdb-0.6.3/hyperon_das_atomdb/utils/settings.py
--rw-r--r--   0        0        0     1161 2024-04-04 20:08:25.669225 hyperon_das_atomdb-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     3605 1970-01-01 00:00:00.000000 hyperon_das_atomdb-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-05 20:46:52.669988 hyperon_das_atomdb-0.6.4/LICENCE
+-rw-r--r--   0        0        0     2687 2024-04-05 20:46:52.673987 hyperon_das_atomdb-0.6.4/README.md
+-rw-r--r--   0        0        0      306 2024-04-05 20:46:52.673987 hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/__init__.py
+-rw-r--r--   0        0        0      116 2024-04-05 20:46:52.673987 hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/adapters/__init__.py
+-rw-r--r--   0        0        0    20238 2024-04-05 20:46:52.673987 hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/adapters/ram_only.py
+-rw-r--r--   0        0        0    36861 2024-04-05 20:46:52.673987 hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/adapters/redis_mongo_db.py
+-rw-r--r--   0        0        0    19708 2024-04-05 20:46:52.677987 hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/database.py
+-rw-r--r--   0        0        0      877 2024-04-05 20:46:52.677987 hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/exceptions.py
+-rw-r--r--   0        0        0     1122 2024-04-05 20:46:52.677987 hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/index.py
+-rw-r--r--   0        0        0     1052 2024-04-05 20:46:52.677987 hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/logger.py
+-rw-r--r--   0        0        0        0 2024-04-05 20:46:52.677987 hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/utils/__init__.py
+-rw-r--r--   0        0        0     1947 2024-04-05 20:46:52.677987 hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/utils/expression_hasher.py
+-rw-r--r--   0        0        0     1388 2024-04-05 20:46:52.677987 hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/utils/patterns.py
+-rw-r--r--   0        0        0       65 2024-04-05 20:46:52.677987 hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/utils/settings.py
+-rw-r--r--   0        0        0     1161 2024-04-05 20:47:02.089933 hyperon_das_atomdb-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     3605 1970-01-01 00:00:00.000000 hyperon_das_atomdb-0.6.4/PKG-INFO
```

### Comparing `hyperon_das_atomdb-0.6.3/LICENCE` & `hyperon_das_atomdb-0.6.4/LICENCE`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.3/README.md` & `hyperon_das_atomdb-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.3/hyperon_das_atomdb/adapters/ram_only.py` & `hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/adapters/ram_only.py`

 * *Files 5% similar despite different names*

```diff
@@ -187,15 +187,15 @@
     def _update_atom_indexes(self, documents: Iterable[Dict[str, any]], **kwargs) -> None:
         for document in documents:
             self._update_index(document, **kwargs)
 
     def _update_index(self, atom: Dict[str, Any], **kwargs):
         if kwargs.get('delete_atom', False):
             if atom is None:
-                raise LinkDoesNotExist('link not exist')
+                raise LinkDoesNotExist('Nonexistent link')
 
             link_handle = atom['_id']
 
             handles = self.db.incoming_set.pop(link_handle, None)
 
             if handles:
                 for handle in handles:
@@ -237,38 +237,38 @@
         if node_handle in self.db.node:
             return node_handle
         else:
             logger().error(
                 f'Failed to retrieve node handle for {node_type}:{node_name}. This node may not exist.'
             )
             raise NodeDoesNotExist(
-                message='This node does not exist',
+                message='Nonexistent node',
                 details=f'{node_type}:{node_name}',
             )
 
     def get_node_name(self, node_handle: str) -> str:
         node = self.db.node.get(node_handle)
         if node is None:
             logger().error(
                 f'Failed to retrieve node name for handle: {node_handle}. This node may not exist.'
             )
             raise NodeDoesNotExist(
-                message='This node does not exist',
+                message='Nonexistent node',
                 details=f'node_handle: {node_handle}',
             )
         return node['name']
 
     def get_node_type(self, node_handle: str) -> str:
         node = self.db.node.get(node_handle)
         if node is None:
             logger().error(
                 f'Failed to retrieve node type for handle: {node_handle}. This node may not exist.'
             )
             raise NodeDoesNotExist(
-                message='This node does not exist',
+                message='Nonexistent node',
                 details=f'node_handle: {node_handle}',
             )
         return node['named_type']
 
     def get_matched_node_name(self, node_type: str, substring: Optional[str] = '') -> str:
         node_type_hash = ExpressionHasher.named_type_hash(node_type)
 
@@ -306,53 +306,53 @@
         if link_handle in self.db.link:
             return link_handle
         else:
             logger().error(
                 f'Failed to retrieve link handle for {link_type}:{target_handles}. This link may not exist.'
             )
             raise LinkDoesNotExist(
-                message='This link does not exist',
+                message='Nonexistent link',
                 details=f'{link_type}:{target_handles}',
             )
 
     def get_link_type(self, link_handle: str) -> str:
         link = self._get_link(link_handle)
         if link is not None:
             return link['named_type']
         else:
             logger().error(
                 f'Failed to retrieve link type for {link_handle}. This link may not exist.'
             )
             raise LinkDoesNotExist(
-                message='This link does not exist',
+                message='Nonexistent link',
                 details=f'link_handle: {link_handle}',
             )
 
     def get_link_targets(self, link_handle: str) -> List[str]:
         answer = self.db.outgoing_set.get(link_handle)
         if answer is None:
             logger().error(
                 f'Failed to retrieve link targets for {link_handle}. This link may not exist.'
             )
             raise LinkDoesNotExist(
-                message='This link does not exist',
+                message='Nonexistent link',
                 details=f'link_handle: {link_handle}',
             )
         return answer
 
     def is_ordered(self, link_handle: str) -> bool:
         link = self._get_link(link_handle)
         if link is not None:
             return True
         else:
             logger().error(
                 'Failed to retrieve document for link handle: {link_handle}. The link may not exist.'
             )
             raise LinkDoesNotExist(
-                message='This link does not exist',
+                message='Nonexistent link',
                 details=f'link_handle: {link_handle}',
             )
 
     def get_matched_links(self, link_type: str, target_handles: List[str], **kwargs) -> list:
         if link_type != WILDCARD and WILDCARD not in target_handles:
             link_handle = self.get_link_handle(link_type, target_handles)
             return [link_handle]
@@ -415,15 +415,15 @@
             else:
                 return document
         else:
             logger().error(
                 f'Failed to retrieve atom for handle: {handle}. This link may not exist. - Details: {kwargs}'
             )
             raise AtomDoesNotExist(
-                message='This atom does not exist',
+                message='Nonexistent atom',
                 details=f'handle: {handle}',
             )
 
     def get_atom_type(self, handle: str) -> str:
         atom = self.db.node.get(handle)
 
         if atom is None:
@@ -445,15 +445,15 @@
             return {
                 'handle': atom['_id'],
                 'type': atom['named_type'],
                 'targets': self._build_targets_list(atom),
             }
         logger().error(f'Failed to retrieve atom for handle: {handle}. This link may not exist.')
         raise AtomDoesNotExist(
-            message='This atom does not exist',
+            message='Nonexistent atom',
             details=f'handle: {handle}',
         )
 
     def count_atoms(self) -> Tuple[int, int]:
         return (len(self.db.node), len(self.db.link))
 
     def clear_database(self) -> None:
@@ -497,15 +497,15 @@
             try:
                 self._delete_link_and_update_index(handle)
             except LinkDoesNotExist:
                 logger().error(
                     f'Failed to delete atom for handle: {handle}. This atom may not exist. - Details: {kwargs}'
                 )
                 raise AtomDoesNotExist(
-                    message='This atom does not exist',
+                    message='Nonexistent atom',
                     details=f'handle: {handle}',
                 )
 
     def create_field_index(
         self,
         atom_type: str,
         field: str,
```

### Comparing `hyperon_das_atomdb-0.6.3/hyperon_das_atomdb/adapters/redis_mongo_db.py` & `hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/adapters/redis_mongo_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -333,15 +333,15 @@
         if document is not None:
             return document[MongoFieldNames.ID_HASH]
         else:
             logger().error(
                 f'Failed to retrieve node handle for {node_type}:{node_name}. This node may not exist.'
             )
             raise NodeDoesNotExist(
-                message="This node does not exist",
+                message="Nonexistent node",
                 details=f"{node_type}:{node_name}",
             )
 
     def get_node_name(self, node_handle: str) -> str:
         answer = self._retrieve_name(node_handle)
         if not answer:
             logger().error(
@@ -394,15 +394,15 @@
         if document is not None:
             return document[MongoFieldNames.ID_HASH]
         else:
             logger().error(
                 f'Failed to retrieve link handle for {link_type}:{target_handles}. This link may not exist.'
             )
             raise LinkDoesNotExist(
-                message="This link does not exist",
+                message="Nonexistent link",
                 details=f"{link_type}:{target_handles}",
             )
 
     def get_link_targets(self, link_handle: str) -> List[str]:
         answer = self._retrieve_outgoing_set(link_handle)
         if not answer:
             logger().error(
@@ -497,15 +497,15 @@
             else:
                 return document
         else:
             logger().error(
                 f'Failed to retrieve atom for handle: {handle}. This link may not exist. - Details: {kwargs}'
             )
             raise AtomDoesNotExist(
-                message='This atom does not exist',
+                message='Nonexistent atom',
                 details=f'handle: {handle}',
             )
 
     def get_atom_type(self, handle: str) -> str:
         atom = self._retrieve_mongo_document(handle)
         if atom is not None:
             return atom['named_type']
@@ -865,15 +865,15 @@
         document = self.mongo_atoms_collection.find_one_and_delete(mongo_filter)
 
         if not document:
             logger().error(
                 f'Failed to delete atom for handle: {handle}. This atom may not exist. - Details: {kwargs}'
             )
             raise AtomDoesNotExist(
-                message='This atom does not exist',
+                message='Nonexistent atom',
                 details=f'handle: {handle}',
             )
         self._update_atom_indexes([document], delete_atom=True)
 
     def create_field_index(
         self,
         atom_type: str,
```

### Comparing `hyperon_das_atomdb-0.6.3/hyperon_das_atomdb/database.py` & `hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/database.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.3/hyperon_das_atomdb/exceptions.py` & `hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.3/hyperon_das_atomdb/index.py` & `hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/index.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.3/hyperon_das_atomdb/logger.py` & `hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/logger.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.3/hyperon_das_atomdb/utils/expression_hasher.py` & `hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/utils/expression_hasher.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.3/hyperon_das_atomdb/utils/patterns.py` & `hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/utils/patterns.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.3/pyproject.toml` & `hyperon_das_atomdb-0.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperon-das-atomdb"
-version = "0.6.3"
+version = "0.6.4"
 description = "Persistence layer for Distributed AtomSpace"
 authors = ["marcocapozzoli <marcocapozzoli90@gmail.com>"]
 readme = "README.md"
 packages = [{include = "hyperon_das_atomdb"}]
 
 [tool.poetry.urls]
 "Code" = "https://github.com/singnet/das-atom-db"
```

### Comparing `hyperon_das_atomdb-0.6.3/PKG-INFO` & `hyperon_das_atomdb-0.6.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperon-das-atomdb
-Version: 0.6.3
+Version: 0.6.4
 Summary: Persistence layer for Distributed AtomSpace
 Author: marcocapozzoli
 Author-email: marcocapozzoli90@gmail.com
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

