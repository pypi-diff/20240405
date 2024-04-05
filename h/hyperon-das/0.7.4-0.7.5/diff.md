# Comparing `tmp/hyperon_das-0.7.4.tar.gz` & `tmp/hyperon_das-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperon_das-0.7.4.tar", max compression
+gzip compressed data, was "hyperon_das-0.7.5.tar", max compression
```

## Comparing `hyperon_das-0.7.4.tar` & `hyperon_das-0.7.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1081 2024-04-04 20:34:42.802366 hyperon_das-0.7.4/LICENCE
--rw-r--r--   0        0        0    12442 2024-04-04 20:34:42.802366 hyperon_das-0.7.4/README.md
--rw-r--r--   0        0        0      108 2024-04-04 20:34:42.846366 hyperon_das-0.7.4/hyperon_das/__init__.py
--rw-r--r--   0        0        0    20544 2024-04-04 20:34:42.846366 hyperon_das-0.7.4/hyperon_das/cache.py
--rw-r--r--   0        0        0     6621 2024-04-04 20:34:42.846366 hyperon_das-0.7.4/hyperon_das/client.py
--rw-r--r--   0        0        0      127 2024-04-04 20:34:42.846366 hyperon_das-0.7.4/hyperon_das/constants.py
--rw-r--r--   0        0        0    25387 2024-04-04 20:34:42.846366 hyperon_das-0.7.4/hyperon_das/das.py
--rw-r--r--   0        0        0     1830 2024-04-04 20:34:42.846366 hyperon_das-0.7.4/hyperon_das/decorators.py
--rw-r--r--   0        0        0     1012 2024-04-04 20:34:42.846366 hyperon_das-0.7.4/hyperon_das/exceptions.py
--rw-r--r--   0        0        0     1072 2024-04-04 20:34:42.846366 hyperon_das-0.7.4/hyperon_das/logger.py
--rw-r--r--   0        0        0       39 2024-04-04 20:34:42.846366 hyperon_das-0.7.4/hyperon_das/pattern_matcher/__init__.py
--rw-r--r--   0        0        0      274 2024-04-04 20:34:42.846366 hyperon_das-0.7.4/hyperon_das/pattern_matcher/constants.py
--rw-r--r--   0        0        0    31913 2024-04-04 20:34:42.846366 hyperon_das-0.7.4/hyperon_das/pattern_matcher/pattern_matcher.py
--rw-r--r--   0        0        0    21024 2024-04-04 20:34:42.846366 hyperon_das-0.7.4/hyperon_das/query_engines.py
--rw-r--r--   0        0        0     1685 2024-04-04 20:34:42.846366 hyperon_das-0.7.4/hyperon_das/traverse_engines.py
--rw-r--r--   0        0        0     5992 2024-04-04 20:34:42.846366 hyperon_das-0.7.4/hyperon_das/utils.py
--rw-r--r--   0        0        0     1315 2024-04-04 20:34:51.294336 hyperon_das-0.7.4/pyproject.toml
--rw-r--r--   0        0        0    13311 1970-01-01 00:00:00.000000 hyperon_das-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-05 20:48:53.845745 hyperon_das-0.7.5/LICENCE
+-rw-r--r--   0        0        0    12442 2024-04-05 20:48:53.845745 hyperon_das-0.7.5/README.md
+-rw-r--r--   0        0        0      108 2024-04-05 20:48:53.885745 hyperon_das-0.7.5/hyperon_das/__init__.py
+-rw-r--r--   0        0        0    20522 2024-04-05 20:48:53.885745 hyperon_das-0.7.5/hyperon_das/cache.py
+-rw-r--r--   0        0        0     6871 2024-04-05 20:48:53.885745 hyperon_das-0.7.5/hyperon_das/client.py
+-rw-r--r--   0        0        0      127 2024-04-05 20:48:53.885745 hyperon_das-0.7.5/hyperon_das/constants.py
+-rw-r--r--   0        0        0    30899 2024-04-05 20:48:53.885745 hyperon_das-0.7.5/hyperon_das/das.py
+-rw-r--r--   0        0        0     1830 2024-04-05 20:48:53.885745 hyperon_das-0.7.5/hyperon_das/decorators.py
+-rw-r--r--   0        0        0     1012 2024-04-05 20:48:53.885745 hyperon_das-0.7.5/hyperon_das/exceptions.py
+-rw-r--r--   0        0        0     1072 2024-04-05 20:48:53.885745 hyperon_das-0.7.5/hyperon_das/logger.py
+-rw-r--r--   0        0        0       39 2024-04-05 20:48:53.885745 hyperon_das-0.7.5/hyperon_das/pattern_matcher/__init__.py
+-rw-r--r--   0        0        0      274 2024-04-05 20:48:53.885745 hyperon_das-0.7.5/hyperon_das/pattern_matcher/constants.py
+-rw-r--r--   0        0        0    31913 2024-04-05 20:48:53.889745 hyperon_das-0.7.5/hyperon_das/pattern_matcher/pattern_matcher.py
+-rw-r--r--   0        0        0    21093 2024-04-05 20:48:53.889745 hyperon_das-0.7.5/hyperon_das/query_engines.py
+-rw-r--r--   0        0        0     1685 2024-04-05 20:48:53.889745 hyperon_das-0.7.5/hyperon_das/traverse_engines.py
+-rw-r--r--   0        0        0     6086 2024-04-05 20:48:53.889745 hyperon_das-0.7.5/hyperon_das/utils.py
+-rw-r--r--   0        0        0     1315 2024-04-05 20:49:05.625804 hyperon_das-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0    13311 1970-01-01 00:00:00.000000 hyperon_das-0.7.5/PKG-INFO
```

### Comparing `hyperon_das-0.7.4/LICENCE` & `hyperon_das-0.7.5/LICENCE`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.4/README.md` & `hyperon_das-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.4/hyperon_das/cache.py` & `hyperon_das-0.7.5/hyperon_das/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -487,15 +487,15 @@
         if self.target_type:
             if not any(target['named_type'] == self.target_type for target in targets):
                 return False
 
         if self.custom_filter and callable(self.custom_filter) and not self.targets_only:
             ret = self.custom_filter(link)
             if not isinstance(ret, bool):
-                raise TypeError('The function must return a boolean')
+                raise TypeError('Filter must return bool')
             if ret is False:
                 return False
 
         return True
 
     def is_empty(self) -> bool:
         return not self.current_value
@@ -552,15 +552,15 @@
             and (self.target_type == target['named_type'] or not self.target_type)
         ):
             return False
 
         if self.source.custom_filter and callable(self.source.custom_filter):
             ret = self.source.custom_filter(target)
             if not isinstance(ret, bool):
-                raise TypeError('The function must return a boolean')
+                raise TypeError('Filter must return bool')
             if ret is False:
                 return False
 
         return True
 
     def is_empty(self) -> bool:
         return not self.current_value
```

### Comparing `hyperon_das-0.7.4/hyperon_das/client.py` & `hyperon_das-0.7.5/hyperon_das/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from hyperon_das_atomdb import AtomDoesNotExist, LinkDoesNotExist, NodeDoesNotExist
 from requests import exceptions, sessions
 
 from hyperon_das.exceptions import ConnectionError, HTTPError, RequestError, TimeoutError
 from hyperon_das.logger import logger
-from hyperon_das.utils import connect_to_server, deserialize, serialize
+from hyperon_das.utils import connect_to_server, das_error, deserialize, serialize
 
 
 class FunctionsClient:
     def __init__(self, host: str, port: int, server_count: int = 0, name: Optional[str] = None):
-        if not host:
-            raise ValueError('Host is required')
+        if not host or not port:
+            das_error(ValueError("'host' and 'port' are mandatory parameters"))
 
         self.url = connect_to_server(host, port)
 
         if not name:
             self.name = f'server-{server_count}'
 
     def _send_request(self, payload) -> Any:
@@ -33,73 +33,81 @@
                 )
 
             response.raise_for_status()
 
             try:
                 response_data = deserialize(response.content)
             except pickle.UnpicklingError as e:
-                raise Exception(f"Unpickling error: {str(e)}")
+                das_error(Exception(f"Unpickling error: {str(e)}"))
 
             if response.status_code == 200:
                 return response_data
             else:
                 return response_data.get(
                     'error', f'Unknown error with status code {response.status_code}'
                 )
         except exceptions.ConnectionError as e:
-            raise ConnectionError(
-                message=f"Connection error for URL: '{self.url}' with payload: '{payload}'",
-                details=str(e),
+            das_error(
+                ConnectionError(
+                    message=f"Connection error for URL: '{self.url}' with payload: '{payload}'",
+                    details=str(e),
+                )
             )
         except exceptions.Timeout as e:
-            raise TimeoutError(
-                message=f"Request timed out for URL: '{self.url}' with payload: '{payload}'",
-                details=str(e),
+            das_error(
+                TimeoutError(
+                    message=f"Request timed out for URL: '{self.url}' with payload: '{payload}'",
+                    details=str(e),
+                )
             )
         except exceptions.HTTPError as e:
             with contextlib.suppress(pickle.UnpicklingError):
                 return deserialize(response.content).get('error')
-            raise HTTPError(
-                message=f"HTTP error occurred for URL: '{self.url}' with payload: '{payload}'",
-                details=str(e),
+            das_error(
+                HTTPError(
+                    message=f"HTTP error for URL: '{self.url}' with payload: '{payload}'",
+                    details=str(e),
+                )
             )
         except exceptions.RequestException as e:
-            raise RequestError(
-                message=f"Request exception occurred for URL: '{self.url}' with payload: '{payload}'.",
-                details=str(e),
+            das_error(
+                RequestError(
+                    message=f"Request exception for URL: '{self.url}' with payload: '{payload}'.",
+                    details=str(e),
+                )
             )
 
     def get_atom(self, handle: str, **kwargs) -> Union[str, Dict]:
         payload = {
             'action': 'get_atom',
             'input': {'handle': handle},
         }
         response = self._send_request(payload)
-        if 'not exist' in response:
-            raise AtomDoesNotExist('error')
+        if 'Nonexistent' in response:
+            das_error(AtomDoesNotExist('error'))
         return response
 
     def get_node(self, node_type: str, node_name: str) -> Union[str, Dict]:
         payload = {
             'action': 'get_node',
             'input': {'node_type': node_type, 'node_name': node_name},
         }
         response = self._send_request(payload)
-        if 'not exist' in response:
-            raise NodeDoesNotExist('error')
+        if 'Nonexistent' in response:
+            das_error(NodeDoesNotExist('error'))
         return response
 
     def get_link(self, link_type: str, link_targets: List[str]) -> Dict[str, Any]:
         payload = {
             'action': 'get_link',
             'input': {'link_type': link_type, 'link_targets': link_targets},
         }
         response = self._send_request(payload)
-        if 'not exist' in response:
-            raise LinkDoesNotExist('error')
+        if 'Nonexistent' in response:
+            das_error(LinkDoesNotExist('error'))
         return response
 
     def get_links(
         self,
         link_type: str,
         target_types: List[str] = None,
         link_targets: List[str] = None,
```

### Comparing `hyperon_das-0.7.4/hyperon_das/das.py` & `hyperon_das-0.7.5/hyperon_das/das.py`

 * *Files 25% similar despite different names*

```diff
@@ -25,32 +25,32 @@
 
         if atomdb == "ram":
             self.backend = InMemoryDB()
         elif atomdb == "redis_mongo":
             self.backend = RedisMongoDB(**kwargs)
             if query_engine != "local":
                 raise InvalidDASParameters(
-                    message="'redis_mongo' backend requires local query engine ('query_engine=local')"
+                    message="'redis_mongo' AtomDB requires local query engine (i.e. 'query_engine=local')"
                 )
         else:
             raise InvalidAtomDB(message="Invalid AtomDB type. Choose either 'ram' or 'redis_mongo'")
 
         kwargs.update({'cache_manager': CacheManager(self.backend)})
 
         if query_engine == 'local':
             self._das_type = 'local_ram_only' if atomdb == 'ram' else 'local_redis_mongo'
             self.query_engine = LocalQueryEngine(self.backend, self.system_parameters, kwargs)
-            logger().info('Initialized local Das')
-        elif query_engine == "remote":
+            logger().info('Started local DAS')
+        elif query_engine == 'remote':
             self._das_type = 'remote'
             self.query_engine = RemoteQueryEngine(self.backend, self.system_parameters, kwargs)
-            logger().info('Initialized remote Das')
+            logger().info('Started remote DAS')
         else:
             raise InvalidQueryEngine(
-                message='The possible values are: `local` or `remote`',
+                message="Use either 'local' or 'remote'",
                 details=f'query_engine={query_engine}',
             )
 
     def _set_default_system_parameters(self) -> None:
         if not self.system_parameters.get('running_on_server'):
             self.system_parameters['running_on_server'] = False
 
@@ -68,92 +68,103 @@
                 'summary': 'Persistence layer for Distributed AtomSpace',
             },
         }
 
     @staticmethod
     def get_node_handle(node_type: str, node_name: str) -> str:
         """
-        This method retrieves a handle from the node parameters
+        Computes the handle of a node, given its type and name.
+
+        Note that this is a static method which don't actually query the stored atomspace
+        in order to compute the handle. Instead, it just run a MD5 hashing algorithm on
+        the parameters that uniquely identify nodes (i.e. type and name) This means e.g.
+        that two nodes with the same type and the same name are considered to be the exact
+        same entity as they will have the same handle.
 
         Args:
-            node_type (str): The type of the node being queried.
-            node_name (str): The name of the specific node being queried.
+            node_type (str): Node type
+            node_name (str): Node name
 
         Returns:
-            str: A handle
+            str: Node's handle
 
         Examples:
             >>> result = das.get_node_handle(node_type='Concept', node_name='human')
             >>> print(result)
             "af12f10f9ae2002a1607ba0b47ba8407"
         """
         return AtomDB.node_handle(node_type, node_name)
 
     @staticmethod
     def get_link_handle(link_type: str, link_targets: List[str]) -> str:
         """
-        This method retrieves a handle from the link parameters.
+        Computes the handle of a link, given its type and targets' handles.
+
+        Note that this is a static method which don't actually query the stored atomspace
+        in order to compute the handle. Instead, it just run a MD5 hashing algorithm on
+        the parameters that uniquely identify links (i.e. type and list of targets) This
+        means e.g. that two links with the same type and the same targets are considered
+        to be the exact same entity as they will have the same handle.
 
         Args:
-            link_type (str): The type of the link being queried.
-            link_targets (List[str]): A list of target identifiers that the link is associated with.
+            link_type (str): Link type.
+            link_targets (List[str]): List with the target handles.
 
         Returns:
-           str: A handle
+           str: Link's handle.
 
         Examples:
-            >>> result = das.get_link(link_type='Similarity', targets=['af12f10f9ae2002a1607ba0b47ba8407', '1cdffc6b0b89ff41d68bec237481d1e1'])
+            >>> human_handle = das.get_node_handle(node_type='Concept', node_name='human')
+            >>> monkey_handle = das.get_node_handle(node_type='Concept', node_name='monkey')
+            >>> result = das.get_link_handle(link_type='Similarity', targets=[human_handle, monkey_handle])
             >>> print(result)
             "bad7472f41a0e7d601ca294eb4607c3a"
 
         """
         return AtomDB.link_handle(link_type, link_targets)
 
-    def get_atom(self, handle: str, **kwargs) -> Union[Dict[str, Any], None]:
+    def get_atom(self, handle: str, **kwargs) -> Dict[str, Any]:
         """
-        Retrieve information about an Atom using its handle.
-
-        This method retrieves information about an Atom from the database
-        based on the provided handle.
+        Retrieve an atom given its handle.
 
         Args:
-            handle (str): The unique handle of the atom.
+            handle (str): Atom's handle.
 
         Returns:
-            Union[Dict, None]: A dictionary containing detailed Atom information
+            Dict: A Python dict with all atom data.
 
         Raises:
-            AtomDoesNotExist: If invalid parameter is provided.
+            AtomDoesNotExist: If the corresponding atom doesn't exist.
 
         Examples:
-            >>> result = das.get_atom(handle="af12f10f9ae2002a1607ba0b47ba8407")
+            >>> human_handle = das.get_node_handle(node_type='Concept', node_name='human')
+            >>> result = das.get_atom(human_handle)
             >>> print(result)
             {
                 'handle': 'af12f10f9ae2002a1607ba0b47ba8407',
                 'composite_type_hash': 'd99a604c79ce3c2e76a2f43488d5d4c3',
                 'name': 'human',
                 'named_type': 'Concept'
             }
         """
         return self.query_engine.get_atom(handle, **kwargs)
 
-    def get_node(self, node_type: str, node_name: str) -> Union[Dict[str, Any], None]:
+    def get_node(self, node_type: str, node_name: str) -> Dict[str, Any]:
         """
-        This method retrieves information about a Node from the database
-        based on its type and name.
+        Retrieve a node given its type and name.
 
         Args:
-            node_type (str): The type of the node being queried.
-            node_name (str): The name of the specific node being queried.
+            node_type (str): Node type
+            node_name (str): Node name
 
         Returns:
-            Union[Dict, None]: A dictionary containing detailed node information
+            Dict: A Python dict with all node data.
 
         Raises:
-            NodeDoesNotExist: If invalid parameters are provided.
+            NodeDoesNotExist: If the corresponding node doesn't exist.
 
         Examples:
             >>> result = das.get_node(
                     node_type='Concept',
                     node_name='human'
                 )
             >>> print(result)
@@ -162,31 +173,27 @@
                 'composite_type_hash': 'd99a604c79ce3c2e76a2f43488d5d4c3',
                 'name': 'human',
                 'named_type': 'Concept'
             }
         """
         return self.query_engine.get_node(node_type, node_name)
 
-    def get_link(self, link_type: str, link_targets: List[str]) -> Union[Dict[str, Any], None]:
+    def get_link(self, link_type: str, link_targets: List[str]) -> Dict[str, Any]:
         """
-        This method retrieves information about a link from the database based on
-        type with given targets.
+        Retrieve a link given its type and list of targets.
 
         Args:
-            link_type (str): The type of the link being queried.
-            link_targets (List[str]): A list of target identifiers that the link is associated with.
+            link_type (str): Link type
+            link_targets (List[str]): List of target handles.
 
         Returns:
-            Union[Dict, None]: A dictionary containing detailed link information
+            Dict: A Python dict with all link data.
 
         Raises:
-            LinkDoesNotExist: If invalid parameters are provided.
-
-        Note:
-            If the specified link or targets do not exist, the method returns None.
+            LinkDoesNotExist: If the corresponding link doesn't exist.
 
         Examples:
             >>> human_handle = das.get_node_handle('Concept', 'human')
             >>> monkey_handle = das.get_node_handle('Concept', 'monkey')
             >>> result = das.get_link(
                     link_type='Similarity',
                     link_targets=[human_handle, monkey_handle],
@@ -204,82 +211,119 @@
                 'named_type': 'Similarity',
                 'named_type_hash': 'a9dea78180588431ec64d6bc4872fdbc',
                 'targets': [
                     'af12f10f9ae2002a1607ba0b47ba8407',
                     '1cdffc6b0b89ff41d68bec237481d1e1'
                 ]
             }
-
         """
         return self.query_engine.get_link(link_type, link_targets)
 
     def get_links(
         self,
         link_type: str,
         target_types: List[str] = None,
         link_targets: List[str] = None,
         **kwargs,
-    ) -> Union[List[str], List[Dict]]:
+    ) -> Union[Iterator, List[Dict[str, Any]]]:
         """
-        Retrieve information about Links based on specified criteria.
+        Retrieve all links that match the passed search criteria.
+
+        This method can be used in four different ways.
+
+        1. Retrieve all the links of a given type
 
-        This method retrieves information about links from the database based on the provided criteria.
-        The criteria includes the link type, and can include target types and specific target identifiers.
-        The retrieved links information can be presented in different output formats as specified
-        by the output_format parameter.
+            Set link_type to the desired type and set target_types=None and
+            link_targets=None.
+
+        2. Retrieve all the links of a given type whose targets are of given types.
+
+            Set link_type to the disered type and target_types to a list with the desired
+            types os each target.
+
+        3. Retrieve all the links of a given type whose targets match a given list of
+           handles
+
+            Set link_type to the desired type (or pass link_type='*' to retrieve links
+            of any type) and set link_targets to a list of handles. Any handle in this
+            list can be '*' meaning that any handle in that position of the targets list
+            is a match for the query. Set target_types=None.
 
         Args:
-            link_type (str): The type of links being queried.
-            target_types (List[str], optional): The type(s) of targets being queried. Defaults to None.
-            link_targets (List[str], optional): A list of target identifiers that the links are associated with.
-                Defaults to None.
+            link_type (str): Link type being searched (can be '*' when link_targets is not None).
+            target_types (List[str], optional): Template of target types being searched.
+            link_targets (List[str], optional): Template of targets being searched (handles or '*').
 
         Returns:
-            Union[List[str], List[Dict]]: A list of dictionaries containing detailed information of the links
+            Union[Iterator, List[Dict[str, Any]]]: A list of dictionaries containing detailed
+            information of the links
 
         Examples:
-            >>> result = das.get_links(
-                    link_type='Similarity',
-                    target_types=['Concept', 'Concept']
-                )
-            >>> print(result)
-            [
-                {
-                    'handle': 'a45af31b43ee5ea271214338a5a5bd61',
-                    'type': 'Similarity',
-                    'template': ['Similarity', 'Concept', 'Concept'],
-                    'targets': [...]
-                },
-                {
-                    'handle': '2d7abd27644a9c08a7ca2c8d68338579',
-                    'type': 'Similarity',
-                    'template': ['Similarity', 'Concept', 'Concept'],
-                    'targets': [...]
-                },
+
+            1. Retrieve all the links of a given type
+
+                >>> links = das.get_links(link_type='Inheritance')
+                >>> for link in links:
+                >>>     print(link['type'], link['targets'])
+                Inheritance ['5b34c54bee150c04f9fa584b899dc030', 'bdfe4e7a431f73386f37c6448afe5840']
+                Inheritance ['b94941d8cd1c0ee4ad3dd3dcab52b964', '80aff30094874e75028033a38ce677bb']
+                Inheritance ['bb34ce95f161a6b37ff54b3d4c817857', '0a32b476852eeb954979b87f5f6cb7af']
                 ...
-            ]
+
+            2. Retrieve all the links of a given type whose targets are of given types.
+
+                >>> links = das.get_links(link_type='Inheritance', target_types=['Concept', 'Concept'])
+                >>> for link in links:
+                >>>     print(link['type'], link['targets'])
+                Inheritance ['5b34c54bee150c04f9fa584b899dc030', 'bdfe4e7a431f73386f37c6448afe5840']
+                Inheritance ['b94941d8cd1c0ee4ad3dd3dcab52b964', '80aff30094874e75028033a38ce677bb']
+                Inheritance ['bb34ce95f161a6b37ff54b3d4c817857', '0a32b476852eeb954979b87f5f6cb7af']
+                ...
+
+            3. Retrieve all the links of a given type whose targets match a given list of
+               handles
+
+                >>> snake = das.get_node_handle('Concept', 'snake')
+                >>> links = das.get_links(link_type='Similarity', link_targets=[snake, '*'])
+                >>> for link in links:
+                >>>     print(link['type'], link['targets'])
+                Similarity ['c1db9b517073e51eb7ef6fed608ec204', 'b94941d8cd1c0ee4ad3dd3dcab52b964']
+                Similarity ['c1db9b517073e51eb7ef6fed608ec204', 'bb34ce95f161a6b37ff54b3d4c817857']
         """
         return self.query_engine.get_links(link_type, target_types, link_targets, **kwargs)
 
     def get_incoming_links(self, atom_handle: str, **kwargs) -> List[Union[Dict[str, Any], str]]:
-        """Retrieve all links pointing to Atom
+        """
+        Retrieve all links which has the passed handle as one of its targets.
 
         Args:
-            atom_handle (str): The unique handle of the atom
+            atom_handle (str): Atom's handle
 
         Returns:
             List[Dict[str, Any]]: A list of dictionaries containing detailed information of the atoms
             or a list of strings containing the atom handles
+
+        Examples:
+            >>> rhino = das.get_node_handle('Concept', 'rhino')
+            >>> links = das.get_incoming_links(rhino)
+            >>> for link in links:
+            >>>     print(link['type'], link['targets'])
+            Similarity ['d03e59654221c1e8fcda404fd5c8d6cb', '99d18c702e813b07260baf577c60c455']
+            Similarity ['99d18c702e813b07260baf577c60c455', 'd03e59654221c1e8fcda404fd5c8d6cb']
+            Inheritance ['99d18c702e813b07260baf577c60c455', 'bdfe4e7a431f73386f37c6448afe5840']
         """
         return self.query_engine.get_incoming_links(atom_handle, **kwargs)
 
     def count_atoms(self) -> Tuple[int, int]:
         """
-        This method is useful for returning the count of atoms in the database.
-        It's also useful for ensuring that the knowledge base load went off without problems.
+        Count nodes and links in DAS.
+
+        In the case of remote DAS, count the total number of nodes and links stored locally and
+        remotelly. If there are more than one instance of the same atom (local and remote), it's
+        counted only once.
 
         Returns:
             Tuple[int, int]: (node_count, link_count)
         """
         return self.query_engine.count_atoms()
 
     def query(
@@ -287,36 +331,37 @@
         query: Union[List[Dict[str, Any]], Dict[str, Any]],
         parameters: Optional[Dict[str, Any]] = {},
     ) -> Union[QueryAnswerIterator, List[Tuple[Assignment, Dict[str, str]]]]:
         """
         Perform a query on the knowledge base using a dict as input and return an
         iterator of QueryAnswer objects. Each such object carries the resulting mapping
         of variables in the query and the corresponding subgraph which is the result
-        of ap[plying such mapping to rewrite the query.
+        of applying such mapping to rewrite the query.
 
         The input dict is a link, used as a pattern to make the query.
         Variables can be used as link targets as well as nodes. Nested links are
         allowed as well.
 
         Args:
-            query (Union[List[Dict[str, Any]], Dict[str, Any]]): A pattern described as a link (possibly with nested links)
-                with nodes and variables used to query the knowledge base.
-                If the query is represented as a list of dictionaries, it should be interpreted as a conjunction (AND) of all queries within the list
+            query (Union[List[Dict[str, Any]], Dict[str, Any]]): A pattern described as a
+                link (possibly with nested links) with nodes and variables used to query
+                the knowledge base. If the query is represented as a list of dictionaries,
+                it is interpreted as a conjunction (AND) of all queries within the list.
             parameters (Dict[str, Any], optional): query optional parameters
 
         Returns:
             QueryAnswerIterator: An iterator of QueryAnswer objects, which have a field 'assignment',
                 with a mapping from variables to handles and another field 'subgraph',
                 with the resulting subgraph after applying 'assignment' to rewrite the query.
 
         Raises:
             UnexpectedQueryFormat: If query resolution lead to an invalid state
 
         Notes:
-            - No logical connectors (AND, OR, NOT) are allowed
+            - Logical connectors OR and NOT are not implemented yet.
             - If no match is found for the query, an empty list is returned.
 
         Examples:
 
             >>> das.add_link({
                 "type": "Expression",
                 "targets": [
@@ -372,87 +417,121 @@
                 }
             ]
         """
         return self.query_engine.query(query, parameters)
 
     def custom_query(self, index_id: str, **kwargs) -> Union[Iterator, List[Dict[str, Any]]]:
         """
-        Perform a custom query on the knowledge base using a custom index id and return an iterator.
-        If no_iterator is set to True, the method returns a list of dict containing detailed atom information
-        (But this way only works with Local Das RedisMongo).
+        Perform a query using a previously created custom index.
+
+        Actual query parameters can be passed as kwargs according to the type of the previously
+        created filter.
 
         Args:
-            index_id (str): the custom index id to be used in the query
+            index_id (str): custom index id to be used in the query.
 
         Raises:
-            NotImplementedError: If the custom_query method is called for the Local DAS in Ram only
+            NotImplementedError: If called from Local DAS in RAM only.
 
         Returns:
-            Union[Iterator, List[Dict[str, Any]]]: An iterator or list of dict containing detailed atom information
+            Union[Iterator, List[Dict[str, Any]]]: An iterator or list of dict containing atom data.
 
         Examples:
-            >>> das.custom_query(index_id='index_123456789', tag='DAS')
-            >>> das.custom_query(index_id='index_123456789', tag='DAS', no_iterator=True)
+            >>> das.custom_query(index_id='index_123', tag='DAS')
+            >>> das.custom_query(index_id='index_123', tag='DAS', no_iterator=True)
         """
         if isinstance(self.query_engine, LocalQueryEngine) and isinstance(self.backend, InMemoryDB):
-            raise NotImplementedError(
-                "The custom_query method is not implemented for the Local DAS in Ram only"
-            )
+            raise NotImplementedError("custom_query() is not implemented for Local DAS in RAM only")
 
         return self.query_engine.custom_query(index_id, **kwargs)
 
     def commit_changes(self):
-        """This method applies changes made locally to the remote server"""
+        """
+        Commit changes (atom addition/deletion/change) to the databases or to
+        the remote DAS Server, depending on the type of DAS being used.
+
+        The behavior of this method depends on the type of DAS being used.
+
+        1. When called in a DAS instantiated with query_engine=remote
+
+            This is called a "Remote DAS" in the documentation. Remote DAS is
+            connected to a remote DAS Server which is used to make queries,
+            traversing, etc but it also keeps a local Atomspace in RAM which is
+            used as a cache. Atom changes are made initially in this local cache.
+            When commit_changes() is called in this type of DAS, these changes are
+            propagated to the remote DAS Server.
+
+        2. When called in a DAS instantiated with query_engine=local and
+           atomdb='ram'.
+
+            No effect.
+
+        3. When called in a DAS instantiated with query_engine=local and
+           atomdb='redis_mongo'
+
+            The AtomDB keeps buffers of changes which are not actually written in the
+            DBs until commit_changes() is called (or until that buffers size reach a
+            threshold).
+        """
         self.query_engine.commit()
 
     def add_node(self, node_params: Dict[str, Any]) -> Dict[str, Any]:
         """
-        Adds a node to the database.
+        Adds a node to DAS.
 
-        This method allows you to add a node to the database
-        with the specified node parameters. A node must have 'type' and
-        'name' fields in the node_params dictionary.
+        A node is represented by a Python dict which may contain any number of keys associated to
+        values of any type (including lists, sets, nested dicts, etc) , which are all
+        recorded with the node, but must contain at least the keys "type" and "name"
+        mapping to strings which define the node uniquely, i.e. two nodes with the same
+        "type" and "name" are considered to be the same entity.
 
         Args:
-            node_params (Dict[str, Any]): A dictionary containing node parameters. It should have the following keys:
-                - 'type': The type of the node.
-                - 'name': The name of the node.
+            node_params (Dict[str, Any]): A dictionary with node data. The following keys are mandatory:
+                - 'type': Node type
+                - 'name': Node name
 
         Returns:
-            Dict[str, Any]: The information about the added node, including its unique key and other details.
+            Dict[str, Any]: The information about the added node, including its unique handle and
+            other fields used internally in DAS.
 
         Raises:
-            AddNodeException: If the 'type' or 'name' fields are missing in node_params.
+            AddNodeException: If 'type' or 'name' fields are missing or invalid somehow.
 
         Examples:
             >>> node_params = {
                     'type': 'Reactome',
                     'name': 'Reactome:R-HSA-164843',
                 }
             >>> das.add_node(node_params)
         """
         return self.backend.add_node(node_params)
 
     def add_link(self, link_params: Dict[str, Any]) -> Dict[str, Any]:
         """
-        Adds a link to the database.
+        Adds a link to DAS.
 
-        This method allows to add a link to the database with the specified link parameters.
-        A link must have a 'type' and 'targets' field in the link_params dictionary.
+        A link is represented by a Python dict which may contain any number of keys associated to
+        values of any type (including lists, sets, nested dicts, etc) , which are all
+        recorded with the link, but must contain at least the keys "type" and "targets".
+        "type" shpould map to a string and "targets" to a list of Python dict, each of them being
+        itself a representation of either a node or a nested link. "type" and "targets" define the
+        link uniquely, i.e. two links with the same "type" and "targets" are considered to be the
+        same entity.
 
         Args:
-            link_params (Dict[str, Any]): A dictionary containing link parameters. It should have the following keys:
+            link_params (Dict[str, Any]): A dictionary with link data. The following keys are mandatory:
                 - 'type': The type of the link.
                 - 'targets': A list of target elements.
 
         Returns:
-            Dict[str, Any]: The information about the added link, including its unique key and other details.
+            Dict[str, Any]: The information about the added link, including its unique handle and
+            other fields used internally in DAS.
 
         Raises:
-            AddLinkException: If the 'type' or 'targets' fields are missing in link_params.
+            AddLinkException: If the 'type' or 'targets' fields are missing or invalid somehow.
 
         Examples:
             >>> link_params = {
                     'type': 'Evaluation',
                     'targets': [
                         {'type': 'Predicate', 'name': 'Predicate:has_name'},
                         {
@@ -525,93 +604,121 @@
 
                     *(handle1, handle2)
                     Similarity(handle1, *)
         """
         return self.query_engine.reindex(pattern_index_templates)
 
     def clear(self) -> None:
-        """Clear all data"""
+        """
+        Delete all atoms and custom indexes.
+        """
         self.backend.clear_database()
         logger().debug('The database has been cleaned.')
 
     def get_traversal_cursor(self, handle: str, **kwargs) -> TraverseEngine:
-        """Create an instance of the TraverseEngine
+        """
+        Create and return a TraverseEngine, an object that can be used to traverse the
+        atomspace hypergraph.
+
+        A TraverseEngine is like a cusor which points to an atom in the hypergraph and
+        can be used to probe for links and neighboring atoms and then move on by
+        following links. It's functioning is closely tied to the cache system in order
+        to optimize the order in which atoms are presented to the caller when probing
+        the neighborhood and to use cache's "atom paging" capabilities to minimize
+        latency when used in remote DAS.
 
         Args:
-            handle (str): atom handle
+            handle (str): Atom's handle
 
         Raises:
-            GetTraversalCursorException: If Atom does not exist
+            GetTraversalCursorException: If passed handle is invalid, somehow (e.g. if
+            the corresponding atom doesn't exist).
 
         Returns:
-            TraverseEngine: The object that allows traversal of the hypergraph
+            TraverseEngine: The object that allows traversal of the hypergraph.
         """
         try:
             return TraverseEngine(handle, das=self, **kwargs)
         except AtomDoesNotExist:
             raise GetTraversalCursorException(message="Cannot start Traversal. Atom does not exist")
 
     def create_field_index(
         self,
         atom_type: str,
         field: str,
         type: Optional[str] = None,
         composite_type: Optional[List[Any]] = None,
     ) -> str:
-        """Create an index for a field for all Atoms of the specified type
+        """
+        Create a custom index on the passed field of all atoms of the passed type.
+
+        Remote DAS allow creation of custom indexes based on custom fields in
+        nodes or links. These indexes can be used to make subsequent custom queries.
 
         Args:
-            atom_type (str): Type of the Atom. Could be 'link' or 'node'
-            field (str): field where the index will be created
-            type (str, optional): Only atoms of the passed type will be indexed. Defaults to None.
-            composite_type (List[Any], optional): Only Atoms type of the passed composite type will be indexed. Defaults to None.
+            atom_type (str): Either 'link' or 'node', if the index is to be created for
+                links or nodes.
+            field (str): field where the index will be created upon
+            type (str, optional): Only atoms of the passed type will be indexed. Defaults
+                to None, meaning that atom type doesn't matter.
+            composite_type (List[Any], optional): Only Atoms type of the passed composite
+                type will be indexed. Defaults to None.
 
         Raises:
-            ValueError: If the type of the Atom is not a string or if both type and composite_type are specified
+            ValueError: If parameters are invalid somehow.
 
         Returns:
-            str: The index ID. This ID should be used to make queries that should use the newly created index.
+            str: The index ID. This ID should be used to make subsequent queries using this
+                newly created index.
 
         Examples:
             >>> index_id = das.create_field_index('link', 'tag', type='Expression')
             >>> index_id = das.create_field_index('link', 'tag', composite_type=['Expression', 'Symbol', 'Symbol', ['Expression', 'Symbol', 'Symbol', 'Symbol']])
         """
-
         if type and composite_type:
-            raise ValueError("Only one of 'type' or 'composite_type' can be specified")
+            raise ValueError("'type' and 'composite_type' can't be specified simultaneously")
 
         if type and not isinstance(type, str):
-            raise ValueError('The type of the Atom must be a string')
+            raise ValueError("'atom_type' should be str")
 
         return self.query_engine.create_field_index(
             atom_type, field, type=type, composite_type=composite_type
         )
 
     def fetch(
         self,
         query: Union[List[dict], dict],
         host: Optional[str] = None,
         port: Optional[int] = None,
         **kwargs,
     ) -> Any:
-        """Fetch data from the remote server using the a query as input and load it locally.
-        If it is a local DAS, the host and port must be sent.
+        """
+        Fetch, from a DAS Server,  all links that match the passed query.
 
-        The input dict is a link, used as a pattern to make the query.
+        Instead of adding atoms by calling add_node() and add_link() directly,
+        it's possible to fetch all or part of the contents from a DAS server using the
+        method fetch(). This method doesn't create a lasting connection with the DAS
+        server, it will just fetch the atoms once and close the connection so any
+        subsequent changes or queries will not be propagated to the server in any way.
+        After fetching the atoms, all queries will be made locally. It's possible to
+        call fetch() multiple times fetching from the same DAS Server or from different
+        ones.
+
+        The input query is a link, used as a pattern to make the query.
         Variables can be used as link targets as well as nodes. Nested links are
         allowed as well.
 
         Args:
             query (Union[List[dict], dict]): A pattern described as a link (possibly with nested links)
                 with nodes and variables used to query the knowledge base.
             host (Optional[str], optional): Address to remote server. Defaults to None.
             port (Optional[int], optional): Port to remote server. Defaults to None.
 
         Raises:
-            ValueError: If the 'host' and 'port' parameters are not sent to DAS local
+            ValueError: If parameters ar somehow invalid.
 
         Examples:
             >>> query = {
                     "atom_type": "link",
                     "type": "Expression",
                     "targets": [
                         {"atom_type": "node", "type": "Symbol", "name": "Inheritance"},
@@ -621,10 +728,10 @@
                 }
                 das = DistributedAtomSpace()
                 das.fetch(query, host='123.4.5.6', port=8080)
         """
 
         if not self.system_parameters.get('running_on_server'):
             if self._das_type != 'remote' and (not host or not port):
-                raise ValueError("The 'host' and 'port' parameters must be sent to DAS local")
+                raise ValueError("'host' and 'port' are mandatory parameters to local DAS")
 
         return self.query_engine.fetch(query, host, port, **kwargs)
```

### Comparing `hyperon_das-0.7.4/hyperon_das/decorators.py` & `hyperon_das-0.7.5/hyperon_das/decorators.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.4/hyperon_das/exceptions.py` & `hyperon_das-0.7.5/hyperon_das/exceptions.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.4/hyperon_das/logger.py` & `hyperon_das-0.7.5/hyperon_das/logger.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.4/hyperon_das/pattern_matcher/pattern_matcher.py` & `hyperon_das-0.7.5/hyperon_das/pattern_matcher/pattern_matcher.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.4/hyperon_das/query_engines.py` & `hyperon_das-0.7.5/hyperon_das/query_engines.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from hyperon_das.client import FunctionsClient
 from hyperon_das.exceptions import (
     InvalidDASParameters,
     QueryParametersException,
     UnexpectedQueryFormat,
 )
 from hyperon_das.logger import logger
-from hyperon_das.utils import Assignment, QueryAnswer
+from hyperon_das.utils import Assignment, QueryAnswer, das_error
 
 
 class QueryEngine(ABC):
     @abstractmethod
     def get_atom(self, handle: str) -> Union[Dict[str, Any], None]:
         ...  # pragma no cover
 
@@ -95,18 +95,14 @@
     def __init__(
         self, backend, system_parameters: Dict[str, Any], kwargs: Optional[dict] = {}
     ) -> None:
         self.system_parameters = system_parameters
         self.cache_manager: CacheManager = kwargs.get('cache_manager')
         self.local_backend = backend
 
-    def _error(self, exception: Exception):
-        logger().error(str(exception))
-        raise exception
-
     def _recursive_query(
         self,
         query: Union[Dict[str, Any], List[Dict[str, Any]]],
         mappings: Set[Assignment] = None,
         parameters: Optional[Dict[str, Any]] = None,
     ) -> QueryAnswerIterator:
         if isinstance(query, list):
@@ -126,23 +122,23 @@
                 if target["atom_type"] == "node" or target["atom_type"] == "link":
                     matched = self._recursive_query(target, mappings, parameters)
                     if matched:
                         matched_targets.append(matched)
                 elif target["atom_type"] == "variable":
                     matched_targets.append(ListIterator([QueryAnswer(target, None)]))
                 else:
-                    self._error(
+                    das_error(
                         UnexpectedQueryFormat(
                             message="Query processing reached an unexpected state",
                             details=f'link: {str(query)} link target: {str(query)}',
                         )
                     )
             return LazyQueryEvaluator(query["type"], matched_targets, self, parameters)
         else:
-            self._error(
+            das_error(
                 UnexpectedQueryFormat(
                     message="Query processing reached an unexpected state",
                     details=f'query: {str(query)}',
                 )
             )
 
     def _to_link_dict_list(self, db_answer: Union[List[str], List[Dict]]) -> List[Dict]:
@@ -170,15 +166,19 @@
             try:
                 return self.local_backend.get_matched_links(link_type, link_targets, **kwargs)
             except LinkDoesNotExist:
                 return None, [] if kwargs.get('cursor') is not None else []
         elif link_type != WILDCARD:
             return self.local_backend.get_matched_type(link_type, **kwargs)
         else:
-            self._error(ValueError("Invalid parameters"))
+            das_error(
+                ValueError(
+                    f"Invalid parameters. link_type = {link_type} target_types = {target_types} link_targets = {link_targets}"
+                )
+            )
 
     def _process_node(self, query: dict) -> List[dict]:
         try:
             handle = self.local_backend.node_handle(query["type"], query["name"])
             return [self.local_backend.get_atom(handle, no_target_format=True)]
         except AtomDoesNotExist:
             return []
@@ -242,33 +242,33 @@
                 if re.search(AtomDB.key_pattern, key):
                     answer.append(self._handle_to_atoms(value))
             return answer
 
     def get_atom(self, handle: str, **kwargs) -> Union[Dict[str, Any], None]:
         try:
             return self.local_backend.get_atom(handle, **kwargs)
-        except AtomDoesNotExist as e:
-            raise e
+        except AtomDoesNotExist as exception:
+            das_error(exception)
 
     def get_node(self, node_type: str, node_name: str) -> Union[Dict[str, Any], None]:
         try:
             node_handle = self.local_backend.node_handle(node_type, node_name)
             return self.local_backend.get_atom(node_handle)
         except AtomDoesNotExist:
-            raise NodeDoesNotExist(
-                message='This node does not exist', details=f'{node_type}:{node_name}'
+            das_error(
+                NodeDoesNotExist(message="Nonexistent node.", details=f'{node_type}:{node_name}')
             )
 
     def get_link(self, link_type: str, link_targets: List[str]) -> Union[Dict[str, Any], None]:
         try:
             link_handle = self.local_backend.link_handle(link_type, link_targets)
             return self.local_backend.get_atom(link_handle)
         except AtomDoesNotExist:
-            raise LinkDoesNotExist(
-                message='This link does not exist', details=f'{link_type}:{link_targets}'
+            das_error(
+                LinkDoesNotExist(message='Nonexistent link', details=f'{link_type}:{link_targets}')
             )
 
     def get_links(
         self,
         link_type: str,
         target_types: List[str] = None,
         link_targets: List[str] = None,
@@ -373,71 +373,67 @@
         **kwargs,
     ) -> Any:
         if not self.system_parameters.get('running_on_server'):  # Local
             documents = self.cache_manager.fetch_data(query=query, host=host, port=port, **kwargs)
             self.cache_manager.bulk_insert(documents)
         else:
             if 'atom_type' not in query:
-                raise ValueError('Invalid query: missing atom_type')
+                das_error(ValueError('Invalid query: missing atom_type'))
 
             atom_type = query['atom_type']
 
             if atom_type == 'node':
                 return self._process_node(query)
             elif atom_type == 'link':
                 return self._process_link(query)
             else:
-                raise ValueError('Invalid atom type')
+                das_error(
+                    ValueError("Invalid atom type: {atom_type}. Use 'node' or 'link' instead.")
+                )
 
 
 class RemoteQueryEngine(QueryEngine):
     def __init__(self, backend, system_parameters: Dict[str, Any], kwargs: Optional[dict] = {}):
         self.system_parameters = system_parameters
         self.cache_manager: CacheManager = kwargs.get('cache_manager')
         self.local_query_engine = LocalQueryEngine(backend, kwargs)
         self.host = kwargs.get('host')
         self.port = kwargs.get('port')
-        if not self.host:
-            raise InvalidDASParameters(message='Send `host` parameter to connect in a remote DAS')
+        if not self.host or not self.port:
+            das_error(InvalidDASParameters(message="'host' and 'port' are mandatory parameters"))
         self.remote_das = FunctionsClient(self.host, self.port)
 
     def get_atom(self, handle: str, **kwargs) -> Dict[str, Any]:
         try:
             atom = self.local_query_engine.get_atom(handle, **kwargs)
         except AtomDoesNotExist:
             try:
                 atom = self.remote_das.get_atom(handle, **kwargs)
-            except AtomDoesNotExist:
-                raise AtomDoesNotExist(
-                    message='This atom does not exist', details=f'handle:{handle}'
-                )
+            except AtomDoesNotExist as exception:
+                das_error(exception)
         return atom
 
     def get_node(self, node_type: str, node_name: str) -> Dict[str, Any]:
         try:
             node = self.local_query_engine.get_node(node_type, node_name)
         except NodeDoesNotExist:
             try:
                 node = self.remote_das.get_node(node_type, node_name)
-            except NodeDoesNotExist:
-                raise NodeDoesNotExist(
-                    message='This node does not exist', details=f'{node_type}:{node_name}'
-                )
+            except NodeDoesNotExist as exception:
+                das_error(exception)
         return node
 
     def get_link(self, link_type: str, link_targets: List[str]) -> Dict[str, Any]:
         try:
             link = self.local_query_engine.get_link(link_type, link_targets)
         except LinkDoesNotExist:
             try:
                 link = self.remote_das.get_link(link_type, link_targets)
-            except LinkDoesNotExist:
-                raise LinkDoesNotExist(
-                    message='This link does not exist', details=f'{link_type}:{link_targets}'
-                )
+            except LinkDoesNotExist as exception:
+                das_error(exception)
         return link
 
     def get_links(
         self,
         link_type: str,
         target_types: List[str] = None,
         link_targets: List[str] = None,
@@ -494,32 +490,37 @@
             previous_value = parameters.get('no_iterator', False)
             parameters['no_iterator'] = True
             answer = self.remote_das.query(query, parameters)
             parameters['no_iterator'] = previous_value
         elif query_scope == 'local_only':
             answer = self.local_query_engine.query(query, parameters)
         elif query_scope == 'local_and_remote':
-            # This type is not available yet
-            raise QueryParametersException
+            das_error(
+                QueryParametersException(
+                    message=f"Invalid value for parameter 'query_scope': '{query_scope}'. This type of query scope is not implemented yet"
+                )
+            )
         else:
-            raise QueryParametersException(
-                message=f'Invalid value for parameter "query_scope": "{query_scope}"'
+            das_error(
+                QueryParametersException(
+                    message=f'Invalid value for "query_scope": "{query_scope}"'
+                )
             )
         return answer
 
     def count_atoms(self) -> Tuple[int, int]:
         local_answer = self.local_query_engine.count_atoms()
         remote_answer = self.remote_das.count_atoms()
         return tuple([x + y for x, y in zip(local_answer, remote_answer)])
 
     def commit(self):
         return self.remote_das.commit_changes()
 
     def reindex(self, pattern_index_templates: Optional[Dict[str, Dict[str, Any]]]):
-        raise NotImplementedError()
+        das_error(NotImplementedError())
 
     def create_field_index(
         self,
         atom_type: str,
         field: str,
         type: Optional[str] = None,
         composite_type: Optional[List[Any]] = None,
```

### Comparing `hyperon_das-0.7.4/hyperon_das/traverse_engines.py` & `hyperon_das-0.7.5/hyperon_das/traverse_engines.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.4/hyperon_das/utils.py` & `hyperon_das-0.7.5/hyperon_das/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,19 @@
 )
 
 from hyperon_das.decorators import retry
 from hyperon_das.exceptions import InvalidAssignment
 from hyperon_das.logger import logger
 
 
+def das_error(exception: Exception):
+    logger().error(str(exception))
+    raise exception
+
+
 class Assignment:
     @staticmethod
     def compose(components: List["Assignment"]) -> Optional["Assignment"]:
         answer = Assignment()
         for component in components:
             if not answer.merge(component):
                 return None
```

### Comparing `hyperon_das-0.7.4/pyproject.toml` & `hyperon_das-0.7.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "hyperon-das"
-version = "0.7.4"
+version = "0.7.5"
 description = "Query Engine API for Distributed AtomSpace"
 authors = ["marcocapozzoli <marcocapozzoli90@gmail.com>"]
 readme = "README.md"
 packages = [{include = "hyperon_das"}]
 
 [tool.poetry.urls]
 "Documentation" = "https://singnet.github.io/das-query-engine"
 "Code" = "https://github.com/singnet/das-query-engine"
 "Bug Tracker" = "https://github.com/singnet/das-query-engine/issues"
 "Releases" = "https://github.com/singnet/das-query-engine/releases"
 
 [tool.poetry.dependencies]
 python = "^3.8.5"
-hyperon-das-atomdb = "0.6.3"
+hyperon-das-atomdb = "0.6.4"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
 flake8 = "^6.1.0"
 black = "^23.9.1"
 pytest = "^7.4.2"
```

### Comparing `hyperon_das-0.7.4/PKG-INFO` & `hyperon_das-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: hyperon-das
-Version: 0.7.4
+Version: 0.7.5
 Summary: Query Engine API for Distributed AtomSpace
 Author: marcocapozzoli
 Author-email: marcocapozzoli90@gmail.com
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: hyperon-das-atomdb (==0.6.3)
+Requires-Dist: hyperon-das-atomdb (==0.6.4)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/singnet/das-query-engine/issues
 Project-URL: Code, https://github.com/singnet/das-query-engine
 Project-URL: Documentation, https://singnet.github.io/das-query-engine
 Project-URL: Releases, https://github.com/singnet/das-query-engine/releases
 Description-Content-Type: text/markdown
```

