# Comparing `tmp/HPW_Tracing-0.1.1.tar.gz` & `tmp/HPW_Tracing-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HPW_Tracing-0.1.1.tar", last modified: Thu Mar 28 01:17:46 2024, max compression
+gzip compressed data, was "HPW_Tracing-0.1.2.tar", last modified: Thu Apr  4 21:10:10 2024, max compression
```

## Comparing `HPW_Tracing-0.1.1.tar` & `HPW_Tracing-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 01:17:46.208011 HPW_Tracing-0.1.1/
-drwxrwxrwx   0        0        0        0 2024-03-28 01:17:46.111734 HPW_Tracing-0.1.1/HPW_Tracing/
-drwxrwxrwx   0        0        0        0 2024-03-28 01:17:46.135811 HPW_Tracing-0.1.1/HPW_Tracing/Build_graphs/
--rw-rw-rw-   0        0        0       43 2024-03-27 18:04:26.000000 HPW_Tracing-0.1.1/HPW_Tracing/Build_graphs/__init__.py
--rw-rw-rw-   0        0        0     2296 2024-03-27 21:49:39.000000 HPW_Tracing-0.1.1/HPW_Tracing/Build_graphs/make_graph.py
-drwxrwxrwx   0        0        0        0 2024-03-28 01:17:46.160093 HPW_Tracing-0.1.1/HPW_Tracing/Tracing/
--rw-rw-rw-   0        0        0     8402 2024-03-27 21:49:39.000000 HPW_Tracing-0.1.1/HPW_Tracing/Tracing/Tracing_with_distance.py
--rw-rw-rw-   0        0        0      121 2024-03-27 18:47:51.000000 HPW_Tracing-0.1.1/HPW_Tracing/Tracing/__init__.py
--rw-rw-rw-   0        0        0      152 2024-03-27 20:05:48.000000 HPW_Tracing-0.1.1/HPW_Tracing/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 01:17:46.119904 HPW_Tracing-0.1.1/HPW_Tracing.egg-info/
--rw-rw-rw-   0        0        0      297 2024-03-28 01:17:45.000000 HPW_Tracing-0.1.1/HPW_Tracing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      501 2024-03-28 01:17:46.000000 HPW_Tracing-0.1.1/HPW_Tracing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 01:17:45.000000 HPW_Tracing-0.1.1/HPW_Tracing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-03-28 01:17:45.000000 HPW_Tracing-0.1.1/HPW_Tracing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-28 01:17:45.000000 HPW_Tracing-0.1.1/HPW_Tracing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      297 2024-03-28 01:17:46.204709 HPW_Tracing-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-03-28 01:17:46.208011 HPW_Tracing-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      485 2024-03-28 01:17:39.000000 HPW_Tracing-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-28 01:17:46.201571 HPW_Tracing-0.1.1/test/
--rw-rw-rw-   0        0        0      586 2024-03-27 19:25:12.000000 HPW_Tracing-0.1.1/test/test_1_tracing_with_nodes.py
--rw-rw-rw-   0        0        0      303 2024-03-27 19:28:52.000000 HPW_Tracing-0.1.1/test/test_2_tracing_with_links.py
--rw-rw-rw-   0        0        0      294 2024-03-27 19:33:05.000000 HPW_Tracing-0.1.1/test/test_3_tracing_between_nodes.py
--rw-rw-rw-   0        0        0      190 2024-03-27 19:40:19.000000 HPW_Tracing-0.1.1/test/test_4_tracing_between_links.py
+drwxrwxrwx   0        0        0        0 2024-04-04 21:10:10.488945 HPW_Tracing-0.1.2/
+drwxrwxrwx   0        0        0        0 2024-04-04 21:10:10.367181 HPW_Tracing-0.1.2/HPW_Tracing/
+drwxrwxrwx   0        0        0        0 2024-04-04 21:10:10.382301 HPW_Tracing-0.1.2/HPW_Tracing/Build_graphs/
+-rw-rw-rw-   0        0        0       48 2024-04-04 21:09:08.000000 HPW_Tracing-0.1.2/HPW_Tracing/Build_graphs/__init__.py
+-rw-rw-rw-   0        0        0     2679 2024-04-04 21:09:08.000000 HPW_Tracing-0.1.2/HPW_Tracing/Build_graphs/make_graph.py
+-rw-rw-rw-   0        0        0    13216 2024-04-04 19:25:14.000000 HPW_Tracing-0.1.2/HPW_Tracing/Build_graphs/network_correction.py
+drwxrwxrwx   0        0        0        0 2024-04-04 21:10:10.402174 HPW_Tracing-0.1.2/HPW_Tracing/Load_data/
+-rw-rw-rw-   0        0        0       32 2024-04-04 14:56:41.000000 HPW_Tracing-0.1.2/HPW_Tracing/Load_data/__init__.py
+-rw-rw-rw-   0        0        0     2486 2024-04-04 19:19:16.000000 HPW_Tracing-0.1.2/HPW_Tracing/Load_data/load_data.py
+drwxrwxrwx   0        0        0        0 2024-04-04 21:10:10.426309 HPW_Tracing-0.1.2/HPW_Tracing/Tracing/
+-rw-rw-rw-   0        0        0     7356 2024-04-04 20:36:27.000000 HPW_Tracing-0.1.2/HPW_Tracing/Tracing/Tracing_with_distance.py
+-rw-rw-rw-   0        0        0      176 2024-04-04 19:19:16.000000 HPW_Tracing-0.1.2/HPW_Tracing/Tracing/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-04-04 20:11:50.000000 HPW_Tracing-0.1.2/HPW_Tracing/Tracing/mh_name_ufid_lookup.py
+-rw-rw-rw-   0        0        0        8 2024-04-04 18:50:07.000000 HPW_Tracing-0.1.2/HPW_Tracing/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 21:10:10.377301 HPW_Tracing-0.1.2/HPW_Tracing.egg-info/
+-rw-rw-rw-   0        0        0      362 2024-04-04 21:10:10.000000 HPW_Tracing-0.1.2/HPW_Tracing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2024-04-04 21:10:10.000000 HPW_Tracing-0.1.2/HPW_Tracing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 21:10:10.000000 HPW_Tracing-0.1.2/HPW_Tracing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2024-04-04 21:10:10.000000 HPW_Tracing-0.1.2/HPW_Tracing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-04 21:10:10.000000 HPW_Tracing-0.1.2/HPW_Tracing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      362 2024-04-04 21:10:10.485917 HPW_Tracing-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-04 21:10:10.488945 HPW_Tracing-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      485 2024-04-04 20:49:36.000000 HPW_Tracing-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 21:10:10.483329 HPW_Tracing-0.1.2/test/
+-rw-rw-rw-   0        0        0      671 2024-04-04 20:21:14.000000 HPW_Tracing-0.1.2/test/test.py
+-rw-rw-rw-   0        0        0      586 2024-03-27 19:25:12.000000 HPW_Tracing-0.1.2/test/test_1_tracing_with_nodes.py
+-rw-rw-rw-   0        0        0      303 2024-03-27 19:28:52.000000 HPW_Tracing-0.1.2/test/test_2_tracing_with_links.py
+-rw-rw-rw-   0        0        0      294 2024-03-27 19:33:05.000000 HPW_Tracing-0.1.2/test/test_3_tracing_between_nodes.py
+-rw-rw-rw-   0        0        0      190 2024-03-27 19:40:19.000000 HPW_Tracing-0.1.2/test/test_4_tracing_between_links.py
+-rw-rw-rw-   0        0        0     1810 2024-04-04 13:52:51.000000 HPW_Tracing-0.1.2/test/test_load_gis_data_from_warehouse.py
```

### Comparing `HPW_Tracing-0.1.1/HPW_Tracing/Tracing/Tracing_with_distance.py` & `HPW_Tracing-0.1.2/HPW_Tracing/Tracing/Tracing_with_distance.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,22 @@
 import networkx as nx
 from collections import deque
 import pickle
 from typing import Tuple, Set, Dict
 import os
 import pandas as pd
 
+def _get_node_mapping(unitID_MHNUM_dict: pd.DataFrame, node, from_col, to_col) -> str:
 
-db_folder = r'//10.120.148.123/hwDataLakeWWIP_s3/HPW-TOOLS/Tracing-tool-db'
-network_parquet = os.path.join(db_folder, 'nnn_link_gdf.parquet')
-
-
-def _map_unitID_MHNUM() -> pd.DataFrame:
-
-    # Read in the data
-    man_df = pd.read_parquet(os.path.join(db_folder, 'Manholes.parquet'))
-    columns = ['MH_NUMBER', 'UNIT_ID']
-    MH_UNITID_map = man_df[columns]
-
-    # Drop any rows with missing values
-    MH_UNITID_map_copy = MH_UNITID_map.dropna()
-
-    return MH_UNITID_map_copy
-
+    if node in unitID_MHNUM_dict[to_col].values:
+        return node
+    elif node in unitID_MHNUM_dict[from_col].values:
+        return unitID_MHNUM_dict.set_index(from_col)[to_col].to_dict()[node]
+    else:
+        raise ValueError(f'Node {node} not found in the graph')
 
 def tracing_with_node_short_distance(graph: nx.Graph, start_node: str, direction: str, distance: int = None) -> Tuple[
     Dict[str, float], pd.DataFrame]:
     """
     Find all links in the specified direction for a given node using BFS.
     :param graph: directed graph of the network
     :param start_node: the node from which to start the search
@@ -33,15 +24,15 @@
     :param distance: the maximum distance to search
     :return: two dictionaries with nodes and edges with their distances from the start node
     """
     print('Tracing has started...')
     print('Please be patient, this may take a while if the search distance is large.')
     queue = deque([(start_node, 0)])
     visited = {start_node: 0}
-    edges = pd.DataFrame(columns=['edgeID', 'distance', 'linkID'])
+    edges = pd.DataFrame(columns=['edgeID', 'distance', 'UFID'])
 
     while queue:
         current_node, current_distance = queue.popleft()
         if distance is not None and current_distance > distance:
             continue
         if direction == 'upstream':
             neighbors = graph.pred[current_node]
@@ -49,121 +40,105 @@
             neighbors = graph.succ[current_node]
         else:
             raise ValueError('Invalid direction. Must be "upstream" or "downstream"')
 
         for neighbor in neighbors:
             if neighbor not in visited:
                 edge = (neighbor, current_node) if direction == 'upstream' else (current_node, neighbor)
-                edge_distance = current_distance + graph.edges[edge]['Length']
+                edge_distance = current_distance + graph.edges[edge]['length']
                 visited[neighbor] = edge_distance
-                link_id = graph.edges[edge]['linkID']
+                link_id = graph.edges[edge]['UFID']
                 if distance is None or edge_distance <= distance:
-                    edges.loc[len(edges)] = {'edgeID': edge, 'distance': edge_distance, 'linkID': link_id}
+                    edges.loc[len(edges)] = {'edgeID': edge, 'distance': edge_distance, 'UFID': link_id}
                     queue.append((neighbor, edge_distance))
                 else:
                     continue
 
     return visited, edges
 
 
-def tracing_with_node(graph: nx.Graph, start_node, direction: str, distance: int = None) -> Tuple[Dict[str, float], pd.DataFrame]:
+def tracing_with_node(graph: nx.Graph, dict: pd.DataFrame, start_node, direction: str, distance: int = None) -> Tuple[Dict[str, float], pd.DataFrame]:
     """
     Find all links in the specified direction for a given node using BFS.
     :param graph:
     :param start_node:
     :param direction:
     :param distance:
     :return:
     """
 
-    unitID_MHNUM_dict = _map_unitID_MHNUM()
+    unitID_MHNUM_dict = dict
 
-    #convert start_node from ufid to mh_num
-    if start_node in unitID_MHNUM_dict['UNIT_ID'].values:
-        start_node = unitID_MHNUM_dict.set_index('UNIT_ID')['MH_NUMBER'].to_dict()[start_node]
-    elif start_node in unitID_MHNUM_dict['MH_NUMBER'].values:
-        pass
-    else:
-        raise ValueError(f'Node {start_node} not found in the graph')
+    #convert start_node from uh_num to ufid if mh_num is provided
+    start_node = _get_node_mapping(unitID_MHNUM_dict, start_node, 'MH_NUMBER', 'UFID')
 
-    # network_parquet_gdf['us_Node'] = network_parquet_gdf['us_Node'].map(map_dict.set_index('MH_NUMBER')['UNIT_ID'].to_dict())
-    # network_parquet_gdf['ds_Node'] = network_parquet_gdf['ds_Node'].map(map_dict.set_index('MH_NUMBER')['UNIT_ID'].to_dict())
 
     if distance:
         if distance < 2000:
             return tracing_with_node_short_distance(graph, start_node, direction, distance)
 
     # Reverse the graph if tracing upstream
     if direction == 'upstream':
         graph = graph.reverse()
 
     # Perform BFS in the specified direction
     bfs_edges = list(nx.bfs_edges(graph, start_node))
-    node_distances = nx.single_source_dijkstra_path_length(graph, start_node, weight='Length')
+    node_distances = nx.single_source_dijkstra_path_length(graph, start_node, weight='length')
 
     # Filter edges based on distance condition
     if distance is not None:
         bfs_edges = [edge for edge in bfs_edges if node_distances[edge[1]] <= distance]
         node_distances = {node: distance_node for node, distance_node in node_distances.items() if distance_node <= distance}
 
-    edges_df = pd.DataFrame([(edge, node_distances[edge[1]], graph.edges[edge]['linkID']) for edge in bfs_edges],
-                            columns=['edgeID', 'distance', 'linkID'])
+    edges_df = pd.DataFrame([(edge, node_distances[edge[1]], graph.edges[edge]['UFID']) for edge in bfs_edges],
+                            columns=['edgeID', 'distance', 'UFID'])
 
     # Reverse the edges if tracing upstream
     if direction == 'upstream':
         edges_df['edgeID'] = edges_df['edgeID'].apply(lambda x: (x[1], x[0]))
 
-    # convert nodes_instances to ufid
-    unitID_MHNUM_dict = unitID_MHNUM_dict.set_index('MH_NUMBER')['UNIT_ID'].to_dict()
+    # check if the node is in the unitID_MHNUM_dict
+    # if not, mark it as "non"
+    node_distances_marked = {node: distance if node in unitID_MHNUM_dict['UFID'].values else 'nan' for node, distance in
+                                node_distances.items()}
 
-    # Mark nodes that don't exist in unitID_MHNUM_dict as "non"
-    node_distances_marked = {node: distance if node in unitID_MHNUM_dict else 'nan' for node, distance in
-                             node_distances.items()}
 
     # Remove nodes marked as "non"
     node_distances_filtered = {node: distance for node, distance in node_distances_marked.items() if distance != 'nan'}
 
-    # convert nodes_instances to ufid
-    node_distances_filtered = {unitID_MHNUM_dict[node]: distance for node, distance in node_distances_filtered.items()}
-
-
     return node_distances_filtered, edges_df
 
-def tracing_with_link(graph: nx.Graph, start_link, direction: str, distance: int = None) -> Tuple[
+def tracing_with_link(graph: nx.Graph, dict:pd.DataFrame ,start_link_ufid, direction: str, distance: int = None) -> Tuple[
     Dict[str, float], pd.DataFrame]:
 
-    start_link = [edge for edge in graph.edges if graph.edges[edge]['linkID'] == start_link]
+
+    start_link = [edge for edge in graph.edges if graph.edges[edge]['UFID'] == start_link_ufid]
     if not start_link:
         raise ValueError(f'Link {start_link} not found in the graph')
 
     start_link = start_link[0]
     start_node = start_link[0] if direction == 'upstream' else start_link[1]
-    return tracing_with_node(graph, start_node, direction, distance)
+    noded_dic, edge_df = tracing_with_node(graph, dict, start_node, direction, distance)
+
+    # add the start_link to the edge_df
+    start_link_row = pd.DataFrame({'edgeID': [start_link], 'distance': [0], 'UFID': [start_link_ufid]})
+
+    edge_df = pd.concat([start_link_row, edge_df], ignore_index=True)
 
+    return noded_dic, edge_df
 
-def tracing_between_nodes(graph: nx.Graph, start, end) -> Tuple[
+
+def tracing_between_nodes(graph: nx.Graph, dict:pd.DataFrame, start, end) -> Tuple[
     Dict[str, float], pd.DataFrame]:
 
-    unitID_MHNUM_dict = _map_unitID_MHNUM()
+    UFID_MHNUM_dict = dict
 
-    #convert start_node from ufid to mh_num
-    if start in unitID_MHNUM_dict['UNIT_ID'].values:
-        start = unitID_MHNUM_dict.set_index('UNIT_ID')['MH_NUMBER'].to_dict()[start]
-    elif start in unitID_MHNUM_dict['MH_NUMBER'].values:
-        pass
-    else:
-        raise ValueError(f'Node {start} not found in the graph')
+    start = _get_node_mapping(UFID_MHNUM_dict, start, 'MH_NUMBER', 'UFID')
 
-    #convert end_node from ufid to mh_num
-    if end in unitID_MHNUM_dict['UNIT_ID'].values:
-        end = unitID_MHNUM_dict.set_index('UNIT_ID')['MH_NUMBER'].to_dict()[end]
-    elif end in unitID_MHNUM_dict['MH_NUMBER'].values:
-        pass
-    else:
-        raise ValueError(f'Node {end} not found in the graph')
+    end = _get_node_mapping(UFID_MHNUM_dict, end, 'MH_NUMBER', 'UFID')
 
 
     # Get all simple paths between start_node and end_node
     all_paths = list(nx.all_simple_paths(graph, start, end))
 
     if not all_paths:
         raise ValueError(f'No paths found between {start} and {end}')
@@ -174,36 +149,35 @@
 
     # Iterate over all paths to extract the edges and find the distance from the start_node
     for path in all_paths:
         distance = 0
         for i in range(len(path) - 1):
             edge = (path[i], path[i + 1])
             all_nodes[path[i]] = distance
-            distance += graph.edges[edge]['Length']
-            link_id = graph.edges[edge]['linkID']
+            distance += graph.edges[edge]['length']
+            link_id = graph.edges[edge]['UFID']
             all_nodes[path[i + 1]] = distance
             all_edges.loc[len(all_edges)] = {'edgeID': edge, 'distance': distance, 'linkID': link_id}
 
     return all_nodes, all_edges
 
-
-def tracing_between_links(graph: nx.Graph, start_link, end_link) -> Tuple[
+def tracing_between_links(graph: nx.Graph, dict, start_link, end_link) -> Tuple[
     Dict[str, float], pd.DataFrame]:
 
-    start_link = [edge for edge in graph.edges if graph.edges[edge]['linkID'] == start_link]
+    start_link = [edge for edge in graph.edges if graph.edges[edge]['UFID'] == start_link]
     if not start_link:
         raise ValueError(f'Link {start_link} not found in the graph')
-    end_link = [edge for edge in graph.edges if graph.edges[edge]['linkID'] == end_link]
+    end_link = [edge for edge in graph.edges if graph.edges[edge]['UFID'] == end_link]
     if not end_link:
         raise ValueError(f'Link {end_link} not found in the graph')
 
     start_link = start_link[0]
     end_link = end_link[0]
 
     start_node = start_link[0]
     end_node = end_link[1]
-    return tracing_between_nodes(graph, start_node, end_node)
+    return tracing_between_nodes(graph, dict, start_node, end_node)
```

### Comparing `HPW_Tracing-0.1.1/test/test_1_tracing_with_nodes.py` & `HPW_Tracing-0.1.2/test/test_1_tracing_with_nodes.py`

 * *Files identical despite different names*

