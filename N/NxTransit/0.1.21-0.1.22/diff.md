# Comparing `tmp/NxTransit-0.1.21.tar.gz` & `tmp/NxTransit-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NxTransit-0.1.21.tar", last modified: Mon Apr  1 15:15:17 2024, max compression
+gzip compressed data, was "NxTransit-0.1.22.tar", last modified: Fri Apr  5 11:09:42 2024, max compression
```

## Comparing `NxTransit-0.1.21.tar` & `NxTransit-0.1.22.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 15:15:17.652983 NxTransit-0.1.21/
--rw-rw-rw-   0        0        0     1101 2024-02-20 06:07:02.000000 NxTransit-0.1.21/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-01 15:15:17.643965 NxTransit-0.1.21/NxTransit.egg-info/
--rw-rw-rw-   0        0        0     3290 2024-04-01 15:15:17.000000 NxTransit-0.1.21/NxTransit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2024-04-01 15:15:17.000000 NxTransit-0.1.21/NxTransit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 15:15:17.000000 NxTransit-0.1.21/NxTransit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      156 2024-04-01 15:15:17.000000 NxTransit-0.1.21/NxTransit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-01 15:15:17.000000 NxTransit-0.1.21/NxTransit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3290 2024-04-01 15:15:17.646972 NxTransit-0.1.21/PKG-INFO
--rw-rw-rw-   0        0        0     2032 2024-03-26 18:30:04.000000 NxTransit-0.1.21/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 15:15:17.638964 NxTransit-0.1.21/nxtransit/
--rw-rw-rw-   0        0        0     1991 2024-04-01 15:10:34.000000 NxTransit-0.1.21/nxtransit/__init__.py
--rw-rw-rw-   0        0        0    15200 2024-04-01 13:47:17.000000 NxTransit-0.1.21/nxtransit/accessibility.py
--rw-rw-rw-   0        0        0     5868 2024-03-25 19:57:15.000000 NxTransit-0.1.21/nxtransit/connectors.py
--rw-rw-rw-   0        0        0     1156 2024-03-25 12:26:14.000000 NxTransit-0.1.21/nxtransit/converters.py
--rw-rw-rw-   0        0        0     7555 2024-03-29 17:16:04.000000 NxTransit-0.1.21/nxtransit/frequency.py
--rw-rw-rw-   0        0        0    13028 2024-03-29 17:42:08.000000 NxTransit-0.1.21/nxtransit/functions.py
--rw-rw-rw-   0        0        0    17492 2024-03-29 21:20:45.000000 NxTransit-0.1.21/nxtransit/loaders.py
--rw-rw-rw-   0        0        0      441 2024-03-29 20:28:51.000000 NxTransit-0.1.21/nxtransit/other.py
--rw-rw-rw-   0        0        0     5977 2024-02-25 22:09:23.000000 NxTransit-0.1.21/nxtransit/prism.py
--rw-rw-rw-   0        0        0    14318 2024-03-28 09:51:45.000000 NxTransit-0.1.21/nxtransit/routers.py
--rw-rw-rw-   0        0        0     1462 2024-03-29 17:11:31.000000 NxTransit-0.1.21/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-01 15:15:17.652983 NxTransit-0.1.21/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-01 15:15:17.641969 NxTransit-0.1.21/tests/
--rw-rw-rw-   0        0        0     2361 2024-03-29 17:46:46.000000 NxTransit-0.1.21/tests/test_functions.py
--rw-rw-rw-   0        0        0     2823 2024-03-20 15:12:08.000000 NxTransit-0.1.21/tests/test_routers.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:09:42.058535 NxTransit-0.1.22/
+-rw-rw-rw-   0        0        0     1101 2024-02-20 06:07:02.000000 NxTransit-0.1.22/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-05 11:09:42.054539 NxTransit-0.1.22/NxTransit.egg-info/
+-rw-rw-rw-   0        0        0     3329 2024-04-05 11:09:41.000000 NxTransit-0.1.22/NxTransit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2024-04-05 11:09:42.000000 NxTransit-0.1.22/NxTransit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 11:09:41.000000 NxTransit-0.1.22/NxTransit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      156 2024-04-05 11:09:41.000000 NxTransit-0.1.22/NxTransit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-05 11:09:41.000000 NxTransit-0.1.22/NxTransit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3329 2024-04-05 11:09:42.056536 NxTransit-0.1.22/PKG-INFO
+-rw-rw-rw-   0        0        0     2032 2024-03-26 18:30:04.000000 NxTransit-0.1.22/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 11:09:42.047538 NxTransit-0.1.22/nxtransit/
+-rw-rw-rw-   0        0        0     1991 2024-04-05 09:00:51.000000 NxTransit-0.1.22/nxtransit/__init__.py
+-rw-rw-rw-   0        0        0    15458 2024-04-04 19:11:30.000000 NxTransit-0.1.22/nxtransit/accessibility.py
+-rw-rw-rw-   0        0        0     5457 2024-04-04 19:18:18.000000 NxTransit-0.1.22/nxtransit/connectors.py
+-rw-rw-rw-   0        0        0     1156 2024-03-25 12:26:14.000000 NxTransit-0.1.22/nxtransit/converters.py
+-rw-rw-rw-   0        0        0     7555 2024-03-29 17:16:04.000000 NxTransit-0.1.22/nxtransit/frequency.py
+-rw-rw-rw-   0        0        0    13352 2024-04-05 08:53:54.000000 NxTransit-0.1.22/nxtransit/functions.py
+-rw-rw-rw-   0        0        0    18894 2024-04-04 19:48:53.000000 NxTransit-0.1.22/nxtransit/loaders.py
+-rw-rw-rw-   0        0        0      441 2024-03-29 20:28:51.000000 NxTransit-0.1.22/nxtransit/other.py
+-rw-rw-rw-   0        0        0     5977 2024-02-25 22:09:23.000000 NxTransit-0.1.22/nxtransit/prism.py
+-rw-rw-rw-   0        0        0    14548 2024-04-05 08:50:08.000000 NxTransit-0.1.22/nxtransit/routers.py
+-rw-rw-rw-   0        0        0     1496 2024-04-05 09:03:31.000000 NxTransit-0.1.22/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 11:09:42.058535 NxTransit-0.1.22/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 11:09:42.051535 NxTransit-0.1.22/tests/
+-rw-rw-rw-   0        0        0     2361 2024-03-29 17:46:46.000000 NxTransit-0.1.22/tests/test_functions.py
+-rw-rw-rw-   0        0        0     2823 2024-03-20 15:12:08.000000 NxTransit-0.1.22/tests/test_routers.py
```

### Comparing `NxTransit-0.1.21/LICENSE` & `NxTransit-0.1.22/LICENSE`

 * *Files identical despite different names*

### Comparing `NxTransit-0.1.21/NxTransit.egg-info/PKG-INFO` & `NxTransit-0.1.22/NxTransit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: NxTransit
-Version: 0.1.21
+Version: 0.1.22
 Summary: Construct and analyze time-dependent transit networks from GTFS data
 Author: Chingiz Zhanarbaev
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Visualization
```

### Comparing `NxTransit-0.1.21/PKG-INFO` & `NxTransit-0.1.22/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: NxTransit
-Version: 0.1.21
+Version: 0.1.22
 Summary: Construct and analyze time-dependent transit networks from GTFS data
 Author: Chingiz Zhanarbaev
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Visualization
```

### Comparing `NxTransit-0.1.21/README.md` & `NxTransit-0.1.22/README.md`

 * *Files identical despite different names*

### Comparing `NxTransit-0.1.21/nxtransit/__init__.py` & `NxTransit-0.1.22/nxtransit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 It uses General Transit Feed Specification (GTFS) data to construct the graph and perform various time-dependent calculations.
 
 Key Features:
 - Multimodal Graph Creation: NxTransit can generate a graph that integrates different modes of transportation with street network.
 - Time-Dependent Calculations: The package allows for the analysis of transit dynamics by considering the time-dependency of transit schedules. This includes calculating shortest paths with departure times, travel time matrices, and service frequency.
 - GTFS Data Support: NxTransit uses GTFS data, a common format for public transportation schedules and associated geographic information, as the basis for graph construction and analysis.
 """
-__version__ = "0.1.21"
+__version__ = "0.1.22"
 
 from .loaders import feed_to_graph
 from .loaders import load_stops_gdf
 
 from .routers import time_dependent_dijkstra
 from .routers import single_source_time_dependent_dijkstra
```

### Comparing `NxTransit-0.1.21/nxtransit/accessibility.py` & `NxTransit-0.1.22/nxtransit/accessibility.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from shapely.geometry import Point
 
 from .functions import determine_utm_zone
 from .routers import single_source_time_dependent_dijkstra
 
 
 def calculate_od_matrix(
-    graph, nodes: list, departure_time: int, hashtable: dict = None, algorithm="sorted"
+    graph: DiGraph, nodes: list, departure_time: float, hashtable: dict = None, algorithm="sorted"
 ):
     """
     Calculates the Origin-Destination (OD) matrix for a given graph, nodes, and departure time.
 
     Parameters
     ----------
     graph : networkx.DiGraph
@@ -100,16 +100,21 @@
         }
         for dest_node in nodes_list
         if dest_node in arrival_times
     ]
 
 
 def calculate_od_matrix_parallel(
-    graph, nodes, departure_time, target_nodes=None, num_processes=2, hashtable=None
-):
+    graph: DiGraph,
+    nodes,
+    departure_time: float,
+    target_nodes: list = None,
+    num_processes: int = 2,
+    hashtable: dict = None,
+) -> pd.DataFrame:
     """
     Calculates the Origin-Destination (OD) matrix for a given graph,
     nodes, and departure time using parallel processing.
 
     Parameters
     ----------
     graph : networkx.DiGraph
@@ -282,24 +287,24 @@
     ].unary_union
     result_gdf = gpd.GeoDataFrame({"geometry": [vectorized_result]}, crs="EPSG:4087")
 
     return result_gdf
 
 
 def percent_access_service_area(
-    graph,
-    source,
-    start_time,
-    end_time,
-    sample_interval,
-    cutoff,
-    buffer_radius,
-    threshold,
-    algorithm="sorted",
-    hashtable=None,
+    graph: DiGraph,
+    source: Any,
+    start_time: int,
+    end_time: int,
+    sample_interval: int,
+    cutoff: int,
+    buffer_radius: float,
+    threshold: float,
+    algorithm: str = "sorted",
+    hashtable: Optional[Dict] = None,
 ) -> gpd.GeoDataFrame:
     """
     Calculate service area reachable with specified chance within the given time period.
 
     This tool rasterize service areas for each time step and overlays them.
     Part of the raster that is covered by at least the threshold of
     the service areas is returned as a vectorized GeoDataFrame.
@@ -346,23 +351,23 @@
         for timestamp in range(start_time, end_time, sample_interval)
     ]
 
     return _rasterize_service_areas(service_areas=service_areas, threshold=threshold)
 
 
 def service_area_multiple_sources(
-    graph,
-    sources,
-    start_time,
-    cutoff,
-    buffer_radius,
-    algorithm="sorted",
-    hashtable=None,
-    num_processes=6,
-):
+    graph: DiGraph,
+    sources: list,
+    start_time: int,
+    cutoff: int,
+    buffer_radius: float,
+    algorithm: str = "sorted",
+    hashtable: Optional[Dict] = None,
+    num_processes: int = 6,
+) -> gpd.GeoDataFrame:
     """
     Calculates service areas for multiple sources using multiprocessing, returning a combined service area polygon.
 
     Parameters
     ----------
     graph : networkx.DiGraph
         NetworkX graph representing the transportation network.
@@ -400,15 +405,15 @@
     combined_service_area = gpd.GeoDataFrame(
         pd.concat(results, ignore_index=True), crs="EPSG:4087"
     )
 
     return combined_service_area
 
 
-def last_service(graph):
+def last_service(graph: DiGraph):
     """
     Calculate the last service time for each stop in the graph.
     Populates the 'last_service' attribute of each transit stop.
 
     Parameters
     ----------
     graph : networkx.DiGraph
```

### Comparing `NxTransit-0.1.21/nxtransit/connectors.py` & `NxTransit-0.1.22/nxtransit/connectors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Tools for connecting GTFS stops to the nearest street node in the graph."""
 import pandas as pd
 import shapely.geometry
 from scipy.spatial import KDTree
 from pyproj import Transformer, CRS
+from geopandas import GeoDataFrame
+from networkx import DiGraph
 
 
-def _fill_coordinates(graph):
+def _fill_coordinates(graph: DiGraph):
     """
     Transforms the coordinates of nodes in the graph from EPSG:4326 to EPSG:4087.
     Populates 'metric_X' and 'metric_Y' attributes of the nodes.
 
     Raises
     ------
     Exception
@@ -26,48 +28,44 @@
 
             graph.nodes[node]['metric_X'] = coords[0]
             graph.nodes[node]['metric_Y'] = coords[1]
         except Exception as e:
             raise Exception(f'{e} occurred for node {node}')
 
 
-def connect_stops_to_streets(graph, stops: pd.DataFrame):
+def connect_stops_to_streets(graph: DiGraph, stops: pd.DataFrame):
     """
     Connects GTFS stops to the nearest street node in the graph
     using projected coordinates in EPSG:4087.
     """
     # Create a list of street node tuples (x, y, node_id)
-    node_data = [(data['metric_X'], data['metric_Y'], idx)
-                 for idx, data in graph.nodes(data=True)
-                 if 'metric_X' in data and 'metric_Y' in data
-                 and data['type'] == 'street']
-
-    node_data_wgs = [(data['x'], data['y'], idx)
-                     for idx, data in graph.nodes(data=True)
-                     if 'y' in data and 'x' in data
-                     and data['type'] == 'street']
+    node_data = [
+        (data["metric_X"], data["metric_Y"], idx, data["x"], data["y"])
+        for idx, data in graph.nodes(data=True)
+        if data["type"] == "street"
+    ]
 
     # Create a KD-tree for nearest neighbor search
     # The tree is created from a list of street node tuples (x, y, node_id)
-    tree = KDTree([(x, y) for x, y, _ in node_data])
+    tree = KDTree([(x, y) for x, y, _, _, _ in node_data])
 
     for index, stop in stops.iterrows():
 
         stop_wgs = (stop['stop_lon'], stop['stop_lat'])
         x, y = graph.nodes[stop['stop_id']]['metric_X'], graph.nodes[stop['stop_id']]['metric_Y']
         stop_coords = (x, y)
 
         # query returns the distance to the nearest neighbor and its index in the tree
         distance, idx = tree.query(stop_coords)
         nearest_street_node = node_data[idx][2]
 
         # Add a connector edge to the graph
         # Create a LineString geometry for the connector edge
         stop_geom = shapely.geometry.Point(stop_wgs)
-        street_geom = shapely.geometry.Point((node_data_wgs[idx][0], node_data_wgs[idx][1]))
+        street_geom = shapely.geometry.Point((node_data[idx][3], node_data[idx][4]))
         linestring = shapely.geometry.LineString([stop_geom, street_geom])
 
         walk_time = distance / 1.39  # walk speed in m/s
 
         graph.add_edge(stop['stop_id'], nearest_street_node,
                         weight=walk_time,
                         type='connector',
@@ -76,73 +74,62 @@
         graph.add_edge(nearest_street_node, stop['stop_id'],
                         weight=walk_time,
                         type='connector',
                         geometry=linestring
                         )
 
 
-def snap_points_to_network(graph, points):
+def snap_points_to_network(graph: DiGraph, points: GeoDataFrame):
     """
     Snaps point features from GeoDataFrame to the nearest street node in the graph.
 
     Parameters
     ----------
         graph : networkx.Graph
             NetworkX graph representing the transit system.
         points : geopandas.GeoDataFrame
             GeoDataFrame containing point geometries.
 
     Returns
     -------
         None. The input graph is modified in-place with added snapped points as nodes.
-    
-    Notes
-    -----
-    points CRS must be EPSG:4326
     """
     # Create a list of street node tuples (x, y, node_id)
-    node_data_wgs = [
-        (data['x'], data['y'], n)
-        for n, data in graph.nodes(data=True)
-        if 'y' in data and 'x' in data
-        and data['type'] == 'street'
-    ]
-
-    node_data_metric = [
-        (data['metric_X'], data['metric_Y'], n)
-        for n, data in graph.nodes(data=True)
-        if 'metric_X' in data and 'metric_Y' in data
-        and data['type'] == 'street'
+    node_data = [
+        (data["metric_X"], data["metric_Y"], idx, data["x"], data["y"])
+        for idx, data in graph.nodes(data=True)
+        if data["type"] == "street"
     ]
 
     # Create a KD-tree for nearest neighbor search
     # The tree is created from a list of street node tuples (x, y, node_id)
-    tree = KDTree([(x, y) for x, y, _ in node_data_metric])
+    tree = KDTree([(x, y) for x, y, _, _, _ in node_data])
     
-    crs_4326 = CRS.from_epsg(4326)
+    input_epsg = points.crs.to_epsg()
+    crs_input = CRS.from_epsg(input_epsg)
     crs_4087 = CRS.from_epsg(4087)
-    transformer = Transformer.from_crs(crs_4326, crs_4087)
+    transformer = Transformer.from_crs(crs_input, crs_4087)
     
     if 'origin_id' not in points.columns:
         points['origin_id'] = points.index
 
     for index, row in points.iterrows():
 
         geometry = row['geometry']
         point_id = row['origin_id']
-        pnt_x, pnt_y = transformer.transform(geometry.y, geometry.x)
+        pnt_x, pnt_y = transformer.transform(xx=geometry.x, yy=geometry.y)
 
         # query returns the distance to the nearest neighbor and its index in the tree
         distance, idx = tree.query((pnt_x, pnt_y))
-        nearest_street_node = node_data_metric[idx][2]
+        nearest_street_node = node_data[idx][2]
 
         # Add a connector edge to the graph
         # Create a LineString geometry for the connector edge
-        street_geom = shapely.geometry.Point((node_data_wgs[idx][0],
-                                                node_data_wgs[idx][1]))
+        street_geom = shapely.geometry.Point((node_data[idx][3],
+                                                node_data[idx][4]))
         linestring = shapely.geometry.LineString([geometry, street_geom])
 
         walk_time = distance / 1.39  # walk speed in m/s
 
         graph.add_node(point_id, x=geometry.x, y=geometry.y, type='snapped')
 
         graph.add_edge(point_id, nearest_street_node,
```

### Comparing `NxTransit-0.1.21/nxtransit/converters.py` & `NxTransit-0.1.22/nxtransit/converters.py`

 * *Files identical despite different names*

### Comparing `NxTransit-0.1.21/nxtransit/frequency.py` & `NxTransit-0.1.22/nxtransit/frequency.py`

 * *Files identical despite different names*

### Comparing `NxTransit-0.1.21/nxtransit/functions.py` & `NxTransit-0.1.22/nxtransit/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import math
 import os
+import warnings
 
 import geopandas as gpd
 import pandas as pd
 from shapely.geometry import Polygon
 
 
-def determine_utm_zone(gdf) -> str:
+def determine_utm_zone(gdf: gpd.GeoDataFrame) -> str:
     """
     Determines the UTM zone for a GeoDataFrame based on its centroid.
     
     Parameters
     ----------
     gdf : GeoDataFrame
         The input geospatial data.
@@ -76,24 +77,24 @@
             grid_indices.append(f"grid_{index}")  # Add the current index to the list
             index += 1  # Increment the index for the next cell
 
     # Create the initial grid GeoDataFrame
     grid = gpd.GeoDataFrame({'id': grid_indices, 'geometry': grid_cells}, crs=utm_crs)
 
     # Perform a spatial join between the grid and the original GeoDataFrame
-    filtered_grid = gpd.sjoin(grid, gdf_utm, how='inner')
+    filtered_grid = gpd.sjoin(grid, gdf_utm[['geometry']], how='inner')
 
     # Drop duplicates to ensure each cell is unique, keeping only 'geometry' and 'grid_index'
     filtered_grid = filtered_grid[['geometry', 'id']].drop_duplicates(subset=['id'])
     filtered_grid.reset_index(drop=True, inplace=True)
 
     return filtered_grid
 
 
-def create_centroids_dataframe(polygon_gdf) -> gpd.GeoDataFrame:
+def create_centroids_dataframe(polygon_gdf: gpd.GeoDataFrame) -> gpd.GeoDataFrame:
     """
     Creates a GeoDataFrame with the centroids of polygons from the given GeoDataFrame.
 
     Parameters
     ----------
     polygon_gdf : gpd.GeoDataFrame
         GeoDataFrame containing polygons.
@@ -129,25 +130,28 @@
         Path to the GTFS dataset directory.
 
     Returns
     -------
     bool
         True if the GTFS feed is valid, False otherwise.
     """
+    if not os.path.isdir(gtfs_path):
+        warnings.warn("Invalid GTFS path.")
+        return False
 
     # List of required GTFS files
     required_files = [
         "agency.txt", "stops.txt", "routes.txt",
         "trips.txt", "stop_times.txt", "calendar.txt"
     ]
 
     # Check for the existence of required GTFS files
     for file in required_files:
         if not os.path.isfile(os.path.join(gtfs_path, file)):
-            print(f"Missing required file: {file}")
+            warnings.warn(f"Missing required file: {file}")
             return False
 
     try:
         # Load GTFS files
         agency_df = pd.read_csv(os.path.join(gtfs_path, "agency.txt"))
         stops_df = pd.read_csv(os.path.join(gtfs_path, "stops.txt"))
         routes_df = pd.read_csv(os.path.join(gtfs_path, "routes.txt"))
@@ -187,25 +191,29 @@
         # Validate stop_times.txt
         if stop_times_df.empty or 'trip_id' not in stop_times_df.columns or 'stop_id' not in stop_times_df.columns:
             print("stop_times.txt is invalid or missing required columns.")
             critical_errors = True
 
         if not set(stop_times_df['trip_id']).issubset(set(trips_df['trip_id'])):
             print("Mismatch in trip IDs between stop_times and trips files.")
+            critical_errors = True
 
         if not set(stop_times_df['stop_id']).issubset(set(stops_df['stop_id'])):
             print("Mismatch in stop IDs between stop_times and stops files.")
+            critical_errors = True
 
         # Validate calendar.txt
         if calendar_df.empty:
             print("calendar.txt is invalid or empty.")
+            critical_errors = True
 
         # Validate stop_times.txt for blank times and format of times
         if 'departure_time' not in stop_times_df.columns or 'arrival_time' not in stop_times_df.columns:
             print("stop_times.txt is missing required time columns.")
+            critical_errors = True
 
         # Check for blank times
         if stop_times_df['departure_time'].isnull().any() or stop_times_df['arrival_time'].isnull().any():
             print("Blank departure or arrival times found in stop_times.txt.")
 
         # Validate time format (HH:MM:SS)
         time_format_regex = r'^(\d{2}):([0-5]\d):([0-5]\d)$'  # check for HH:MM:SS format
```

### Comparing `NxTransit-0.1.21/nxtransit/loaders.py` & `NxTransit-0.1.22/nxtransit/loaders.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Load combined GTFS and OSM data into a graph."""
 import multiprocessing as mp
 import os
+from functools import partial
 
 import geopandas as gpd
 import networkx as nx
-import numpy as np
 import osmnx as ox
 import pandas as pd
 from shapely.geometry import LineString, Point
 
 from .connectors import _fill_coordinates, connect_stops_to_streets
 from .converters import parse_time_to_seconds
+from .functions import validate_feed
 from .other import logger
 
 
 def _preprocess_schedules(graph: nx.DiGraph):
     """
     Sorts the schedules on each edge for faster lookup.
     """
@@ -78,73 +79,120 @@
     # For each pair of consecutive stops in the group, add an edge to the graph
     for i in range(len(group) - 1):
         start_stop, end_stop = group.iloc[i], group.iloc[i + 1]
         departure, arrival = (
             parse_time_to_seconds(start_stop["departure_time"]),
             parse_time_to_seconds(end_stop["arrival_time"]),
         )
+        if departure > arrival:
+            raise ValueError(
+                f"Departure time {departure} is greater than arrival time {arrival} for edge {start_stop['stop_id']} -> {end_stop['stop_id']}\n"
+                "Negative travel time not allowed\n"
+                "Check the GTFS feed for errors in stop_times.txt or calendar.txt, or adjust the departure time\n"
+            )
+
         trip_id = start_stop["trip_id"]
         route_id = trip_route_mapping.get(trip_id)
         wheelchair_accessible = trip_wheelchair_mapping.get(trip_id, None)
-
         schedule_info = (departure, arrival, route_id, wheelchair_accessible)
-    
+
         # If read_shapes is True, use the shape geometry from shapes.txt
         geometry = None
         if read_shapes:
             shape_id = trip_to_shape_map.get(trip_id)
             geometry = shapes.get(shape_id)
         # Otherwise, use the stop coordinates to create a simple LineString geometry
         else:
             start_coords, end_coords = (
                 stop_coords_mapping.get(start_stop["stop_id"]),
-                stop_coords_mapping.get(end_stop["stop_id"])
+                stop_coords_mapping.get(end_stop["stop_id"]),
+            )
+            geometry = LineString(
+                [
+                    (start_coords["stop_lon"], start_coords["stop_lat"]),
+                    (end_coords["stop_lon"], end_coords["stop_lat"]),
+                ]
             )
-            if start_coords and end_coords:
-                geometry = LineString(
-                    [
-                        (start_coords["stop_lon"], start_coords["stop_lat"]),
-                        (end_coords["stop_lon"], end_coords["stop_lat"]),
-                    ]
-                )
 
-        _add_edge_with_geometry(graph, start_stop, end_stop, schedule_info, geometry)
+        _add_edge_with_geometry(
+            graph=graph,
+            start_stop=start_stop,
+            end_stop=end_stop,
+            schedule_info=schedule_info,
+            geometry=geometry,
+        )
 
 
 def _add_edges_parallel(
-    graph, trips_chunks, trips_df, shapes, read_shapes, trip_to_shape_map, stops_df
+    trips_chunks, graph, trips_df, shapes, read_shapes, trip_to_shape_map, stops_df
 ):
     """
     Adds edges to the graph for chunks of trips in parallel.
     """
     local_graph = graph.copy()
     for _, group in trips_chunks.groupby(["trip_id"]):
         sorted_group = group.sort_values("stop_sequence")
         _process_trip_group(
-            sorted_group,
-            local_graph,
-            trips_df,
-            shapes,
-            trip_to_shape_map,
-            stops_df,
-            read_shapes,
+            group=sorted_group,
+            graph=local_graph,
+            trips_df=trips_df,
+            shapes=shapes,
+            trip_to_shape_map=trip_to_shape_map,
+            stops_df=stops_df,
+            read_shapes=read_shapes,
         )
     return local_graph
 
 
 def _filter_stop_times_by_time(stop_times: pd.DataFrame, departure_time: int, duration_seconds: int):
     """Filters stop_times to only include trips that occur within a specified time window."""
 
     stop_times['departure_time_seconds'] = stop_times['departure_time'].apply(parse_time_to_seconds)
     return stop_times[
         (stop_times['departure_time_seconds'] >= departure_time) &
         (stop_times['departure_time_seconds'] <= departure_time + duration_seconds)
     ]
 
 
+def _split_dataframe(df: pd.DataFrame, n_splits: int) -> list[pd.DataFrame]:
+    """
+    Splits a DataFrame into n equal parts by rows.
+    This function replaces np.split_array which will be deprecated soon.
+    
+    Parameters
+    ----------
+    df : pandas DataFrame
+        The DataFrame to be split.
+    n_splits : int
+        The number of parts to split the DataFrame into.
+    
+    Returns
+    -------
+    list of pandas DataFrames
+        A list of DataFrame parts.
+    """
+    # Calculate split sizes
+    total_rows = len(df)
+    base_size = total_rows // n_splits
+    remainder = total_rows % n_splits
+
+    # Determine the number of rows each split will have
+    split_sizes = [
+        base_size + 1 if i < remainder 
+        else base_size for i in range(n_splits)
+    ]
+    # Calculate the start indices for each split
+    start_indices = [sum(split_sizes[:i]) for i in range(n_splits)]
+
+    return [
+        df.iloc[start : start + size] for start, size 
+        in zip(start_indices, split_sizes)
+    ]
+
+
 def _load_GTFS(
         GTFSpath: str,
         departure_time_input: str,
         day_of_week: str,
         duration_seconds,
         read_shapes=False,
         multiprocessing=False
@@ -171,32 +219,31 @@
     tuple
         A tuple containing:
             - nx.DiGraph: Graph representing GTFS data.
             - pd.DataFrame: DataFrame containing stop information.
     """
     # Initialize the graph and read data files.
     G = nx.DiGraph()
-
-    stops_df = pd.read_csv(os.path.join(GTFSpath, "stops.txt"),
-                           usecols=['stop_id', 'stop_lat', 'stop_lon'])
-
-    stop_times_df = pd.read_csv(os.path.join(GTFSpath, "stop_times.txt"),
-                                usecols=['departure_time',
-                                         'trip_id',
-                                         'stop_id',
-                                         'stop_sequence',
-                                         'arrival_time'])
-
+    stops_df = pd.read_csv(
+        os.path.join(GTFSpath, "stops.txt"), 
+        usecols=["stop_id", "stop_lat", "stop_lon"]
+    )
+    stop_times_df = pd.read_csv(
+        os.path.join(GTFSpath, "stop_times.txt"),
+        usecols=["departure_time", "trip_id", "stop_id", "stop_sequence", "arrival_time"]
+    )
+    routes = pd.read_csv(
+        os.path.join(GTFSpath, "routes.txt"), usecols=["route_id", "route_short_name"]
+    )
     trips_df = pd.read_csv(os.path.join(GTFSpath, "trips.txt"))
-
-    routes = pd.read_csv(os.path.join(GTFSpath, "routes.txt"), 
-                         usecols=['route_id', 'route_short_name'])
-
+    calendar_df = pd.read_csv(os.path.join(GTFSpath, "calendar.txt"))
+    
     # Load shapes.txt if read_shapes is True
     if read_shapes:
+        logger.warning("Reading shapes is currently not working as intended")
         if "shapes.txt" not in os.listdir(GTFSpath):
             raise FileNotFoundError("shapes.txt not found")
 
         shapes_df = pd.read_csv(os.path.join(GTFSpath, "shapes.txt"))
         # Group geometry by shape_id, resulting in a Pandas Series
         # with trip_id (shape_id ?) as keys and LineString geometries as values
         # This is definitely not working as intended
@@ -206,40 +253,32 @@
         # Mapping trip_id to shape_id for faster lookup
         trip_to_shape_map = trips_df.set_index("trip_id")["shape_id"].to_dict()
 
     else:
         shapes = None
         trip_to_shape_map = None
 
-    # Join route information to trips``
+    # Join route information to trips
     trips_df = trips_df.merge(routes, on="route_id")
+    # Filter trips by day of the week
+    service_ids = calendar_df[calendar_df[day_of_week] == 1]["service_id"]
+    trips_df = trips_df[trips_df["service_id"].isin(service_ids)]
 
-    # Check if calendar.txt exists in GTFS directory
-    # If it does, filter by day of the week, otherwise raise an error
-    if "calendar.txt" in os.listdir(GTFSpath):
-        calendar_df = pd.read_csv(os.path.join(GTFSpath, "calendar.txt"))
-        # Filter for the day of the week
-        service_ids = calendar_df[calendar_df[day_of_week] == 1]["service_id"]
-        trips_df = trips_df[trips_df["service_id"].isin(service_ids)]
-    else:
-        raise FileNotFoundError("Required file calendar.txt not found")
-
-    # Filter stop_times to only include trips that occur within a specified time window
+    # Filter stop_times by valid trips
     valid_trips = stop_times_df['trip_id'].isin(trips_df['trip_id'])
     stop_times_df = stop_times_df[valid_trips].dropna()
 
     # Convert departure_time from HH:MM:SS o seconds
     departure_time_seconds = parse_time_to_seconds(departure_time_input)
     # Filtering stop_times by time window
-    filtered_stops = _filter_stop_times_by_time(stop_times_df,
-                                                departure_time_seconds,
-                                                duration_seconds
-                                                )
+    filtered_stops = _filter_stop_times_by_time(
+        stop_times_df, departure_time_seconds, duration_seconds
+    )
 
-    print(f'GTFS data loaded\n{len(filtered_stops)} of {len(stop_times_df)} trips retained')
+    print(f'{len(filtered_stops)} of {len(stop_times_df)} trips retained')
 
     # Adding stops as nodes to the graph
     for _, stop in stops_df.iterrows():
         G.add_node(
             stop["stop_id"],
             type="transit",
             pos=(stop["stop_lon"], stop["stop_lat"]),
@@ -248,29 +287,31 @@
         )
 
     if multiprocessing:
         print("Building graph in parallel")
         # Divide filtered_stops into chunks for parallel processing
         # Use half of the available CPU logical cores
         # (likely equal to the number of physical cores)
-        num_cores = int(mp.cpu_count() / 2)
-        chunks = np.array_split(filtered_stops, num_cores)
+        num_cores = int(mp.cpu_count() / 2) if mp.cpu_count() > 1 else 1
+        chunks = _split_dataframe(filtered_stops, num_cores)
 
         # Create a pool of processes
         with mp.Pool(processes=num_cores) as pool:
             # Create a subgraph in each process
             # Each will return a graph with edges for a subset of trips
             # The results will be combined into a single graph
-            results = pool.starmap(
-                _add_edges_parallel,
-                [
-                    (G, chunk, trips_df, shapes, read_shapes, trip_to_shape_map, stops_df)
-                    for chunk in chunks
-                ],
+            add_edges_partial = partial(_add_edges_parallel,
+                graph=G,
+                trips_df=trips_df,
+                shapes=shapes,
+                read_shapes=read_shapes,
+                trip_to_shape_map=trip_to_shape_map,
+                stops_df=stops_df
             )
+            results = pool.map(add_edges_partial, chunks)
 
         # Merge results from all processes
         merged_graph = nx.DiGraph()
 
         for graph in results:
             merged_graph.add_nodes_from(graph.nodes(data=True))
         # Add edges from subgraphs to the merged graph
@@ -293,26 +334,25 @@
 
         return merged_graph, stops_df
 
     else:
         for trip_id, group in filtered_stops.groupby("trip_id"):
             sorted_group = group.sort_values("stop_sequence")
             _process_trip_group(
-                sorted_group,
-                G,
-                trips_df,
-                shapes,
-                trip_to_shape_map,
-                stops_df,
-                read_shapes,
+                group=sorted_group,
+                graph=G,
+                trips_df=trips_df,
+                shapes=shapes,
+                trip_to_shape_map=trip_to_shape_map,
+                stops_df=stops_df,
+                read_shapes=read_shapes,
             )
 
         # Sorting schedules for faster lookup using binary search
-        _preprocess_schedules(G)
-
+        _preprocess_schedules(graph=G)
         logger.info("Transit graph created")
 
         return G, stops_df
 
 
 def _load_osm(stops, save_graphml, path) -> nx.DiGraph:
     """
@@ -330,25 +370,26 @@
 
     Returns
     -------
     G_city : networkx.DiGraph
         A street network graph with walking times as edge weights.
     """
     # Building a convex hull from stop coordinates for OSM loading
-    stops_gdf = gpd.GeoDataFrame(stops, geometry=gpd.points_from_xy(stops.stop_lon, stops.stop_lat))
+    stops_gdf = gpd.GeoDataFrame(
+        stops, geometry=gpd.points_from_xy(stops.stop_lon, stops.stop_lat)
+    )
     boundary = stops_gdf.unary_union.convex_hull
 
     logger.info("Loading OSM graph via OSMNX")
     # Loading OSM data within the convex hull
     G_city = ox.graph_from_polygon(boundary, network_type="walk", simplify=True)
-    
+
     attributes_to_keep = {"length", "highway", "name"}
     for u, v, key, data in G_city.edges(keys=True, data=True):
         # Clean extra attributes
-        
         for attribute in list(data):
             if attribute not in attributes_to_keep:
                 del data[attribute]
 
         # Calculate walking time in seconds
         data["weight"] = data["length"] / 1.39
         data["type"] = "street"
@@ -407,14 +448,19 @@
         Flag for loading the OSM graph from a GraphML file. Default is False.
 
     Returns
     -------
     G_combined : nx.DiGraph
         Combined multimodal graph representing transit network.
     """
+    # Validate the GTFS feed
+    bool_feed_valid = validate_feed(GTFSpath)
+    if not bool_feed_valid:
+        raise ValueError("The GTFS feed is not valid")
+    
     G_transit, stops = _load_GTFS(
         GTFSpath,
         departure_time_input,
         day_of_week,
         duration_seconds,
         read_shapes=read_shapes,
         multiprocessing=multiprocessing,
@@ -430,15 +476,14 @@
         # Import OSM data
         G_city = _load_osm(stops, save_graphml, output_graph_path)
 
     # Combining OSM and GTFS data
     G_combined = nx.compose(G_transit, G_city)
     # Filling projected coordinates for graph nodes
     _fill_coordinates(G_combined)
-
     # Connecting stops to OSM streets
     connect_stops_to_streets(G_combined, stops)
 
     logger.info(
         f"Nodes: {G_combined.number_of_nodes()}, Edges: {G_combined.number_of_edges()}"
     )
```

### Comparing `NxTransit-0.1.21/nxtransit/prism.py` & `NxTransit-0.1.22/nxtransit/prism.py`

 * *Files identical despite different names*

### Comparing `NxTransit-0.1.21/nxtransit/routers.py` & `NxTransit-0.1.22/nxtransit/routers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Main routing algorithms for time-dependent graphs."""
-from heapq import heappop, heappush
 import bisect
+from heapq import heappop, heappush
+
+from networkx import DiGraph
 
 
 def _calculate_delay_sorted_nr(graph, from_node, to_node, current_time, wheelchair=False):
     """
     Calculates the delay and route for a given graph, from_node, to_node, and current_time.
     Used in the time-dependent Dijkstra algorithm.
     This version does not return the route, and is used for the single_source_time_dependent_dijkstra_sorted function.
@@ -34,14 +36,15 @@
     if 'sorted_schedules' in edge:
         schedules = edge['sorted_schedules']
         departure_times = edge['departure_times']
         idx = bisect.bisect_left(departure_times, current_time)
         
         if idx < len(schedules):
             next_departure, next_arrival, route, wheelchair_acc = schedules[idx]
+            # Not very much explicit but best way to reduce computational overhead
             if not wheelchair or wheelchair_acc == 1:
                 return next_departure - current_time + (next_arrival - next_departure), route
         
         return float('inf'), None
     else:
         return edge.get('weight', float('inf')), None
 
@@ -298,15 +301,17 @@
                 heappush(queue, (new_arrival_time, neighbor))
 
                 travel_times[neighbor] = new_arrival_time - start_time
 
     return arrival_times, predecessors, travel_times
 
 
-def single_source_time_dependent_dijkstra(graph, source, start_time: int, hashtable: dict = None, algorithm='sorted'):
+def single_source_time_dependent_dijkstra(
+    graph: DiGraph, source, start_time: int, hashtable: dict = None, algorithm="sorted"
+) -> tuple[dict, dict, dict]:
     """
     Compute the shortest paths and travel times from a single source node to all other nodes in a time-dependent graph.
     You can use the `process_graph_to_hash_table` function to create the hash table.
 
     Parameters
     ----------
     graph : nx.DiGraph
@@ -325,20 +330,22 @@
     Returns
     -------
     tuple
         A tuple containing three dictionaries:
             - arrival_times: A dictionary mapping each node to the earliest arrival time from the source node.
             - predecessors: A dictionary mapping each node to its predecessor on the shortest path from the source node.
             - travel_times: A dictionary mapping each node to the travel time from the source node.
-            
+
     See Also
     --------
     nxtransit.functions.process_graph_to_hash_table : Create a hash table for quick access to sorted schedules.
     """
     if algorithm == "sorted":
-        return single_source_time_dependent_dijkstra_sorted(graph, source, start_time)
+        return single_source_time_dependent_dijkstra_sorted(
+            graph=graph, source=source, start_time=start_time
+        )
     elif algorithm == "hashed":
         return single_source_time_dependent_dijkstra_hashed(
-            graph, source, start_time, hashtable
+            graph=graph, source=source, start_time=start_time, hashtable=hashtable
         )
     else:
         raise (ValueError, "Invalid algorithm. Use 'sorted' or 'hashed'")
```

### Comparing `NxTransit-0.1.21/pyproject.toml` & `NxTransit-0.1.22/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 readme = "README.md" 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
+    "Operating System :: MacOS",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering :: GIS",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Visualization",
```

### Comparing `NxTransit-0.1.21/tests/test_functions.py` & `NxTransit-0.1.22/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `NxTransit-0.1.21/tests/test_routers.py` & `NxTransit-0.1.22/tests/test_routers.py`

 * *Files identical despite different names*

