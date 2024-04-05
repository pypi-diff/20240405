# Comparing `tmp/diblob-1.0.7.tar.gz` & `tmp/diblob-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diblob-1.0.7.tar", last modified: Wed Apr  3 17:44:04 2024, max compression
+gzip compressed data, was "diblob-1.0.9.tar", last modified: Fri Apr  5 15:54:56 2024, max compression
```

## Comparing `diblob-1.0.7.tar` & `diblob-1.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jakub      (501) staff       (20)        0 2024-04-03 17:44:04.149492 diblob-1.0.7/
--rw-r--r--   0 jakub      (501) staff       (20)    23332 2024-04-03 17:44:04.149165 diblob-1.0.7/PKG-INFO
--rw-r--r--   0 jakub      (501) staff       (20)    22908 2024-03-24 13:32:23.000000 diblob-1.0.7/README.md
--rw-r--r--   0 jakub      (501) staff       (20)       38 2024-04-03 17:44:04.149529 diblob-1.0.7/setup.cfg
--rw-r--r--   0 jakub      (501) staff       (20)      675 2024-04-03 17:43:02.000000 diblob-1.0.7/setup.py
-drwxr-xr-x   0 jakub      (501) staff       (20)        0 2024-04-03 17:44:04.143990 diblob-1.0.7/src/
-drwxr-xr-x   0 jakub      (501) staff       (20)        0 2024-04-03 17:44:04.147031 diblob-1.0.7/src/diblob/
--rw-r--r--   0 jakub      (501) staff       (20)      126 2024-04-03 17:30:37.000000 diblob-1.0.7/src/diblob/__init__.py
--rw-r--r--   0 jakub      (501) staff       (20)     3964 2024-02-22 17:41:02.000000 diblob-1.0.7/src/diblob/algorithms.py
--rw-r--r--   0 jakub      (501) staff       (20)     4134 2024-02-22 17:19:30.000000 diblob-1.0.7/src/diblob/components.py
--rw-r--r--   0 jakub      (501) staff       (20)    21469 2024-04-03 17:30:58.000000 diblob-1.0.7/src/diblob/digraph_manager.py
--rw-r--r--   0 jakub      (501) staff       (20)     2546 2024-04-03 16:40:02.000000 diblob-1.0.7/src/diblob/exceptions.py
--rw-r--r--   0 jakub      (501) staff       (20)     5171 2024-03-24 13:32:23.000000 diblob-1.0.7/src/diblob/factory.py
--rw-r--r--   0 jakub      (501) staff       (20)     6725 2024-04-03 16:40:02.000000 diblob-1.0.7/src/diblob/generators.py
--rw-r--r--   0 jakub      (501) staff       (20)     3090 2024-04-03 17:15:55.000000 diblob-1.0.7/src/diblob/tools.py
-drwxr-xr-x   0 jakub      (501) staff       (20)        0 2024-04-03 17:44:04.147569 diblob-1.0.7/src/diblob.egg-info/
--rw-r--r--   0 jakub      (501) staff       (20)    23332 2024-04-03 17:44:04.000000 diblob-1.0.7/src/diblob.egg-info/PKG-INFO
--rw-r--r--   0 jakub      (501) staff       (20)      463 2024-04-03 17:44:04.000000 diblob-1.0.7/src/diblob.egg-info/SOURCES.txt
--rw-r--r--   0 jakub      (501) staff       (20)        1 2024-04-03 17:44:04.000000 diblob-1.0.7/src/diblob.egg-info/dependency_links.txt
--rw-r--r--   0 jakub      (501) staff       (20)        7 2024-04-03 17:44:04.000000 diblob-1.0.7/src/diblob.egg-info/top_level.txt
-drwxr-xr-x   0 jakub      (501) staff       (20)        0 2024-04-03 17:44:04.148797 diblob-1.0.7/tests/
--rw-r--r--   0 jakub      (501) staff       (20)     1958 2024-02-18 17:18:38.000000 diblob-1.0.7/tests/test_components.py
--rw-r--r--   0 jakub      (501) staff       (20)    12368 2024-03-24 13:32:23.000000 diblob-1.0.7/tests/test_digraph_manager.py
--rw-r--r--   0 jakub      (501) staff       (20)     6876 2024-02-19 19:23:58.000000 diblob-1.0.7/tests/test_exploratory_unit_tests.py
--rw-r--r--   0 jakub      (501) staff       (20)    11271 2024-03-24 13:32:23.000000 diblob-1.0.7/tests/test_factory.py
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2024-04-05 15:54:56.707583 diblob-1.0.9/
+-rw-r--r--   0 jakub      (501) staff       (20)    23712 2024-04-05 15:54:56.707358 diblob-1.0.9/PKG-INFO
+-rw-r--r--   0 jakub      (501) staff       (20)    23288 2024-04-05 15:52:19.000000 diblob-1.0.9/README.md
+-rw-r--r--   0 jakub      (501) staff       (20)       38 2024-04-05 15:54:56.707633 diblob-1.0.9/setup.cfg
+-rw-r--r--   0 jakub      (501) staff       (20)      675 2024-04-05 15:52:30.000000 diblob-1.0.9/setup.py
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2024-04-05 15:54:56.702862 diblob-1.0.9/src/
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2024-04-05 15:54:56.705140 diblob-1.0.9/src/diblob/
+-rw-r--r--   0 jakub      (501) staff       (20)      126 2024-04-05 15:52:19.000000 diblob-1.0.9/src/diblob/__init__.py
+-rw-r--r--   0 jakub      (501) staff       (20)     3964 2024-02-22 17:41:02.000000 diblob-1.0.9/src/diblob/algorithms.py
+-rw-r--r--   0 jakub      (501) staff       (20)     4134 2024-02-22 17:19:30.000000 diblob-1.0.9/src/diblob/components.py
+-rw-r--r--   0 jakub      (501) staff       (20)    21557 2024-04-05 15:52:19.000000 diblob-1.0.9/src/diblob/digraph_manager.py
+-rw-r--r--   0 jakub      (501) staff       (20)     2546 2024-04-03 16:40:02.000000 diblob-1.0.9/src/diblob/exceptions.py
+-rw-r--r--   0 jakub      (501) staff       (20)     5171 2024-03-24 13:32:23.000000 diblob-1.0.9/src/diblob/factory.py
+-rw-r--r--   0 jakub      (501) staff       (20)     7203 2024-04-05 15:52:19.000000 diblob-1.0.9/src/diblob/generators.py
+-rw-r--r--   0 jakub      (501) staff       (20)     3090 2024-04-03 17:15:55.000000 diblob-1.0.9/src/diblob/tools.py
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2024-04-05 15:54:56.705865 diblob-1.0.9/src/diblob.egg-info/
+-rw-r--r--   0 jakub      (501) staff       (20)    23712 2024-04-05 15:54:56.000000 diblob-1.0.9/src/diblob.egg-info/PKG-INFO
+-rw-r--r--   0 jakub      (501) staff       (20)      463 2024-04-05 15:54:56.000000 diblob-1.0.9/src/diblob.egg-info/SOURCES.txt
+-rw-r--r--   0 jakub      (501) staff       (20)        1 2024-04-05 15:54:56.000000 diblob-1.0.9/src/diblob.egg-info/dependency_links.txt
+-rw-r--r--   0 jakub      (501) staff       (20)        7 2024-04-05 15:54:56.000000 diblob-1.0.9/src/diblob.egg-info/top_level.txt
+drwxr-xr-x   0 jakub      (501) staff       (20)        0 2024-04-05 15:54:56.706964 diblob-1.0.9/tests/
+-rw-r--r--   0 jakub      (501) staff       (20)     1958 2024-02-18 17:18:38.000000 diblob-1.0.9/tests/test_components.py
+-rw-r--r--   0 jakub      (501) staff       (20)    12368 2024-03-24 13:32:23.000000 diblob-1.0.9/tests/test_digraph_manager.py
+-rw-r--r--   0 jakub      (501) staff       (20)     6876 2024-02-19 19:23:58.000000 diblob-1.0.9/tests/test_exploratory_unit_tests.py
+-rw-r--r--   0 jakub      (501) staff       (20)    11271 2024-03-24 13:32:23.000000 diblob-1.0.9/tests/test_factory.py
```

### Comparing `diblob-1.0.7/PKG-INFO` & `diblob-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diblob
-Version: 1.0.7
+Version: 1.0.9
 Summary: A simple example package
 Home-page: https://github.com/JakubZelek/Diblob
 Author: Jakub Zelek
 Author-email: jakub.zelek@doctoral.uj.edu.pl
 License: MIT
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -448,7 +448,18 @@
 Tools deliver following functions:
 - `display_digraph(d: dict, indent=0)`: Enables printing dict in json format (work as print).
 - `cut_outgoing_edges(digraph_manager, diblob_id: str)`: Cuts outgoing nodes of the Digraph (can be used with GraphManager `__call__`)
 - `sort_outgoing_nodes_in_dict_repr(node_lst: list)`: Sorts outgoing nodes.
 <br> Example: `['C', 'B', 'A', {'G1': ['A', 'C', 'B']}] -> ['A', 'B', 'C', {'G1': ['A', 'B', 'C']}]`
 - `list_groupby`: Works like groupby from itertools (no need data to be sorted).
 
+  
+## Generators
+Random digraphs can be generated using generators module. 
+Digraphs which can be generated:
+- random cycle
+- random directed acyclic graph
+- random strongly connected graph (as a sum of cycles)
+- random graph as a combination of DAG and the others (injection)
+
+example of usage can be found in notebooks: 
+https://github.com/JakubZelek/Diblob/tree/main/notebooks
```

### Comparing `diblob-1.0.7/README.md` & `diblob-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -434,7 +434,18 @@
 Tools deliver following functions:
 - `display_digraph(d: dict, indent=0)`: Enables printing dict in json format (work as print).
 - `cut_outgoing_edges(digraph_manager, diblob_id: str)`: Cuts outgoing nodes of the Digraph (can be used with GraphManager `__call__`)
 - `sort_outgoing_nodes_in_dict_repr(node_lst: list)`: Sorts outgoing nodes.
 <br> Example: `['C', 'B', 'A', {'G1': ['A', 'C', 'B']}] -> ['A', 'B', 'C', {'G1': ['A', 'B', 'C']}]`
 - `list_groupby`: Works like groupby from itertools (no need data to be sorted).
 
+  
+## Generators
+Random digraphs can be generated using generators module. 
+Digraphs which can be generated:
+- random cycle
+- random directed acyclic graph
+- random strongly connected graph (as a sum of cycles)
+- random graph as a combination of DAG and the others (injection)
+
+example of usage can be found in notebooks: 
+https://github.com/JakubZelek/Diblob/tree/main/notebooks
```

### Comparing `diblob-1.0.7/setup.py` & `diblob-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='diblob',
-    version='1.0.7',
+    version='1.0.9',
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
     description='A simple example package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Jakub Zelek',
     author_email='jakub.zelek@doctoral.uj.edu.pl',
```

### Comparing `diblob-1.0.7/src/diblob/algorithms.py` & `diblob-1.0.9/src/diblob/algorithms.py`

 * *Files identical despite different names*

### Comparing `diblob-1.0.7/src/diblob/components.py` & `diblob-1.0.9/src/diblob/components.py`

 * *Files identical despite different names*

### Comparing `diblob-1.0.7/src/diblob/digraph_manager.py` & `diblob-1.0.9/src/diblob/digraph_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -535,16 +535,16 @@
     def inject(self, digraph_manager: "DigraphManager", node_id: str):
         """
         Replace node by diblob.
         """
         namespace = (set(digraph_manager.diblobs) & set(self.diblobs)) |\
                     (set(digraph_manager.nodes) & set(self.nodes))
         if namespace:
-            raise CommonResourcesInjection(f"Injection can be performed only with new id namespace.\
-                                           Common {namespace=}")
+            raise CommonResourcesInjection(f"Injection can be performed only with new ID\
+                                            (not occupied). Common {namespace=}")
 
         node = self[node_id]
 
         injected_diblob_root_id = digraph_manager.root_diblob_id
         self.diblobs |= digraph_manager.diblobs
         self.nodes |= digraph_manager.nodes
         self.edges |= digraph_manager.edges
@@ -552,18 +552,23 @@
         self[injected_diblob_root_id].parent_id = node.diblob_id
         self[node.diblob_id]._add_children(injected_diblob_root_id)
         self[node.diblob_id]._add_nodes(injected_diblob_root_id)
 
 
         for injected_node_id in digraph_manager[injected_diblob_root_id].nodes:
 
-            self.connect_nodes(*[(incoming_node_id, injected_node_id)
-                               for incoming_node_id in node.incoming_nodes])
-            self.connect_nodes(*[(injected_node_id, outgoing_node_id)
-                               for outgoing_node_id in node.outgoing_nodes])
+
+            if isinstance(digraph_manager[injected_node_id], Node):
+
+                self.connect_nodes(*[(incoming_node_id, injected_node_id)
+                                for incoming_node_id in node.incoming_nodes])
+
+                self.connect_nodes(*[(injected_node_id, outgoing_node_id)
+                                for outgoing_node_id in node.outgoing_nodes])
+
 
         self.remove_nodes(node)
 
 
     def join_diblobs(self, diblob_fst_id: str, diblob_snd_id: str, join_id: str):
         """
         Join two diblobs to diblob with join_id.
```

### Comparing `diblob-1.0.7/src/diblob/exceptions.py` & `diblob-1.0.9/src/diblob/exceptions.py`

 * *Files identical despite different names*

### Comparing `diblob-1.0.7/src/diblob/factory.py` & `diblob-1.0.9/src/diblob/factory.py`

 * *Files identical despite different names*

### Comparing `diblob-1.0.7/src/diblob/generators.py` & `diblob-1.0.9/src/diblob/generators.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,26 @@
                                             dict_y.get(key, [])))
                                             for key in set(dict_x) | set(dict_y)}})
         return RandomBase(digraph_manager)
 
     def __str__(self) -> str:
         return str(self.digraph_manager)
 
+    def remove_isolated_nodes(self):
+        """
+        Removes isolated nodes.
+        """
+        occupied_nodes = set(edge[0] for edge in self.digraph_manager.edges.keys()) |\
+                         set(edge[1] for edge in self.digraph_manager.edges.keys())
+
+        nodes_to_remove = [self.digraph_manager[node_id] for node_id in
+                           self.digraph_manager.nodes.keys() - occupied_nodes]
+
+        self.digraph_manager.remove_nodes(*nodes_to_remove)
+
 
 class RandomCycle(RandomBase):
     """
     Generates random cycle with delivered size which is embedded in node_space.
     """
 
     def __init__(self, node_space: list[str], cycle_size: int,
@@ -138,15 +150,15 @@
     Generates random digraph by delivered list of digraphs injection.
     - uses dag as the base of the graph.
     - replace random nodes by elements of the list with digraphs.
     """
 
     def __init__(self,
                  dag_digraph: RandomDigraph,
-                 inj_digraphs: list[RandomSCC],
+                 inj_digraphs: list[RandomBase],
                  injection_drop_probability: float = 0.2):
 
 
         dag = dag_digraph.digraph_manager
         if len(dag.diblobs) > 1:
             raise RootDiblobException('DAG in generator should be and digraphs\
                                        with just one diblob (root)!')
@@ -172,8 +184,7 @@
 
 
             dag_digraph.digraph_manager.remove_edges(*[dag_digraph.digraph_manager[drop_id][0]
                                                        for drop_id in edges_to_drop
                                             if random.random() < injection_drop_probability])
 
         super().__init__(dag_digraph)
-
```

### Comparing `diblob-1.0.7/src/diblob/tools.py` & `diblob-1.0.9/src/diblob/tools.py`

 * *Files identical despite different names*

### Comparing `diblob-1.0.7/src/diblob.egg-info/PKG-INFO` & `diblob-1.0.9/src/diblob.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diblob
-Version: 1.0.7
+Version: 1.0.9
 Summary: A simple example package
 Home-page: https://github.com/JakubZelek/Diblob
 Author: Jakub Zelek
 Author-email: jakub.zelek@doctoral.uj.edu.pl
 License: MIT
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -448,7 +448,18 @@
 Tools deliver following functions:
 - `display_digraph(d: dict, indent=0)`: Enables printing dict in json format (work as print).
 - `cut_outgoing_edges(digraph_manager, diblob_id: str)`: Cuts outgoing nodes of the Digraph (can be used with GraphManager `__call__`)
 - `sort_outgoing_nodes_in_dict_repr(node_lst: list)`: Sorts outgoing nodes.
 <br> Example: `['C', 'B', 'A', {'G1': ['A', 'C', 'B']}] -> ['A', 'B', 'C', {'G1': ['A', 'B', 'C']}]`
 - `list_groupby`: Works like groupby from itertools (no need data to be sorted).
 
+  
+## Generators
+Random digraphs can be generated using generators module. 
+Digraphs which can be generated:
+- random cycle
+- random directed acyclic graph
+- random strongly connected graph (as a sum of cycles)
+- random graph as a combination of DAG and the others (injection)
+
+example of usage can be found in notebooks: 
+https://github.com/JakubZelek/Diblob/tree/main/notebooks
```

### Comparing `diblob-1.0.7/tests/test_components.py` & `diblob-1.0.9/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `diblob-1.0.7/tests/test_digraph_manager.py` & `diblob-1.0.9/tests/test_digraph_manager.py`

 * *Files identical despite different names*

### Comparing `diblob-1.0.7/tests/test_exploratory_unit_tests.py` & `diblob-1.0.9/tests/test_exploratory_unit_tests.py`

 * *Files identical despite different names*

### Comparing `diblob-1.0.7/tests/test_factory.py` & `diblob-1.0.9/tests/test_factory.py`

 * *Files identical despite different names*

