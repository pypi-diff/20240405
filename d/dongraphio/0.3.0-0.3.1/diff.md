# Comparing `tmp/dongraphio-0.3.0.tar.gz` & `tmp/dongraphio-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dongraphio-0.3.0.tar", max compression
+gzip compressed data, was "dongraphio-0.3.1.tar", max compression
```

## Comparing `dongraphio-0.3.0.tar` & `dongraphio-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1418 2024-04-01 09:59:57.088394 dongraphio-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1395 2024-03-13 09:15:32.791323 dongraphio-0.3.0/README.md
--rw-r--r--   0        0        0      262 2024-04-01 09:14:48.789528 dongraphio-0.3.0/src/dongraphio/__init__.py
--rw-r--r--   0        0        0      133 2024-04-01 09:14:48.791527 dongraphio-0.3.0/src/dongraphio/base_models/__init__.py
--rw-r--r--   0        0        0    14979 2024-04-01 09:14:48.792530 dongraphio-0.3.0/src/dongraphio/base_models/grapher_logic.py
--rw-r--r--   0        0        0     5383 2024-04-01 09:14:48.793529 dongraphio-0.3.0/src/dongraphio/base_models/isochrones_logic.py
--rw-r--r--   0        0        0     2273 2024-04-01 09:14:48.793529 dongraphio-0.3.0/src/dongraphio/base_models/matrix_logic.py
--rw-r--r--   0        0        0     6150 2024-04-01 09:14:48.794528 dongraphio-0.3.0/src/dongraphio/dongraphio.py
--rw-r--r--   0        0        0     1056 2024-03-13 09:15:32.794322 dongraphio-0.3.0/src/dongraphio/enums.py
--rw-r--r--   0        0        0      559 2024-04-01 09:14:48.796532 dongraphio-0.3.0/src/dongraphio/utils/__init__.py
--rw-r--r--   0        0        0     1262 2024-03-29 09:52:53.311030 dongraphio-0.3.0/src/dongraphio/utils/geometry_utils.py
--rw-r--r--   0        0        0    19283 2024-04-01 09:14:48.797530 dongraphio-0.3.0/src/dongraphio/utils/graph_utils.py
--rw-r--r--   0        0        0     2283 2024-04-01 09:14:48.798529 dongraphio-0.3.0/src/dongraphio/utils/matrix_utils.py
--rw-r--r--   0        0        0     1713 2024-03-13 09:15:32.797336 dongraphio-0.3.0/src/dongraphio/utils/osm_worker.py
--rw-r--r--   0        0        0     1647 2024-04-01 09:14:48.799528 dongraphio-0.3.0/src/dongraphio/utils/tsp_solver.py
--rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 dongraphio-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1418 2024-04-05 16:39:32.861939 dongraphio-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1395 2024-03-13 09:15:32.791323 dongraphio-0.3.1/README.md
+-rw-r--r--   0        0        0      262 2024-04-05 16:39:32.853935 dongraphio-0.3.1/src/dongraphio/__init__.py
+-rw-r--r--   0        0        0      133 2024-04-01 09:14:48.791527 dongraphio-0.3.1/src/dongraphio/base_models/__init__.py
+-rw-r--r--   0        0        0    14979 2024-04-01 09:14:48.792530 dongraphio-0.3.1/src/dongraphio/base_models/grapher_logic.py
+-rw-r--r--   0        0        0     5383 2024-04-01 09:14:48.793529 dongraphio-0.3.1/src/dongraphio/base_models/isochrones_logic.py
+-rw-r--r--   0        0        0     2519 2024-04-05 16:37:52.018036 dongraphio-0.3.1/src/dongraphio/base_models/matrix_logic.py
+-rw-r--r--   0        0        0     6150 2024-04-01 09:14:48.794528 dongraphio-0.3.1/src/dongraphio/dongraphio.py
+-rw-r--r--   0        0        0     1056 2024-03-13 09:15:32.794322 dongraphio-0.3.1/src/dongraphio/enums.py
+-rw-r--r--   0        0        0      559 2024-04-01 09:14:48.796532 dongraphio-0.3.1/src/dongraphio/utils/__init__.py
+-rw-r--r--   0        0        0     1262 2024-03-29 09:52:53.311030 dongraphio-0.3.1/src/dongraphio/utils/geometry_utils.py
+-rw-r--r--   0        0        0    19283 2024-04-01 09:14:48.797530 dongraphio-0.3.1/src/dongraphio/utils/graph_utils.py
+-rw-r--r--   0        0        0     2602 2024-04-04 09:04:56.734596 dongraphio-0.3.1/src/dongraphio/utils/matrix_utils.py
+-rw-r--r--   0        0        0     1713 2024-03-13 09:15:32.797336 dongraphio-0.3.1/src/dongraphio/utils/osm_worker.py
+-rw-r--r--   0        0        0     1647 2024-04-01 09:14:48.799528 dongraphio-0.3.1/src/dongraphio/utils/tsp_solver.py
+-rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 dongraphio-0.3.1/PKG-INFO
```

### Comparing `dongraphio-0.3.0/pyproject.toml` & `dongraphio-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dongraphio"
-version = "0.3.0"
+version = "0.3.1"
 description = "Small utility library containing graph algorighms used in other projects"
 authors = ["Danila <63115678+DDonnyy@users.noreply.github.com>"]
 readme = "README.md"
 
 packages = [{ include = "dongraphio", from = "src" }]
 
 [tool.poetry.dependencies]
```

### Comparing `dongraphio-0.3.0/README.md` & `dongraphio-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.0/src/dongraphio/base_models/grapher_logic.py` & `dongraphio-0.3.1/src/dongraphio/base_models/grapher_logic.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.0/src/dongraphio/base_models/isochrones_logic.py` & `dongraphio-0.3.1/src/dongraphio/base_models/isochrones_logic.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.0/src/dongraphio/base_models/matrix_logic.py` & `dongraphio-0.3.1/src/dongraphio/base_models/matrix_logic.py`

 * *Files 12% similar despite different names*

```diff
@@ -51,11 +51,15 @@
             mobility_sub_graph,
             from_index,
             to_index,
             weight=self.weight,
         )
 
         distance_matrix_result = distance_matrix_result.apply(pd.to_numeric, errors="coerce")
-        distance_matrix.update(distance_matrix_result)
+        def update_value(ind, col):
+            if ind in distance_matrix_result.index and col in distance_matrix_result.columns:
+                return distance_matrix_result.loc[ind, col]
+
+        distance_matrix = distance_matrix.apply(lambda x: x.index.map(lambda ind: update_value(ind, x.name)))
         distance_matrix.index = self.gdf_from.index
         distance_matrix.columns = self.gdf_to.index
         return distance_matrix
```

### Comparing `dongraphio-0.3.0/src/dongraphio/dongraphio.py` & `dongraphio-0.3.1/src/dongraphio/dongraphio.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.0/src/dongraphio/enums.py` & `dongraphio-0.3.1/src/dongraphio/enums.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.0/src/dongraphio/utils/__init__.py` & `dongraphio-0.3.1/src/dongraphio/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.0/src/dongraphio/utils/geometry_utils.py` & `dongraphio-0.3.1/src/dongraphio/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.0/src/dongraphio/utils/graph_utils.py` & `dongraphio-0.3.1/src/dongraphio/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.0/src/dongraphio/utils/matrix_utils.py` & `dongraphio-0.3.1/src/dongraphio/utils/matrix_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,8 +49,15 @@
     del spsp
     return distance_matrix
 
 
 def get_dist_matrix_for_tsp(graph: nx.DiGraph, route_nodes: list[tuple]) -> (pd.DataFrame, pd.DataFrame):
     route_nodes_ind = [x[0] for x in route_nodes]
     distance_matrix, route_matrix = get_dist_matrix(graph, route_nodes_ind, route_nodes_ind, True)
+    mean_value = distance_matrix.values.mean()
+    for i in route_nodes:
+        node_1, n1_1, n2_1 = i
+        for j in route_nodes:
+            node_2, n1_2, n2_2 = j
+            if (n1_1, n2_1) == (n2_2, n1_2):
+                distance_matrix.loc[node_1, node_2] = (mean_value+distance_matrix.loc[node_1, node_2])/3
     return distance_matrix, route_matrix
```

### Comparing `dongraphio-0.3.0/src/dongraphio/utils/osm_worker.py` & `dongraphio-0.3.1/src/dongraphio/utils/osm_worker.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.0/src/dongraphio/utils/tsp_solver.py` & `dongraphio-0.3.1/src/dongraphio/utils/tsp_solver.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.0/PKG-INFO` & `dongraphio-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dongraphio
-Version: 0.3.0
+Version: 0.3.1
 Summary: Small utility library containing graph algorighms used in other projects
 Author: Danila
 Author-email: 63115678+DDonnyy@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

