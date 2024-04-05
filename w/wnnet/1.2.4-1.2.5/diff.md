# Comparing `tmp/wnnet-1.2.4.tar.gz` & `tmp/wnnet-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wnnet-1.2.4.tar", last modified: Thu Mar  7 21:20:24 2024, max compression
+gzip compressed data, was "wnnet-1.2.5.tar", last modified: Fri Apr  5 21:38:31 2024, max compression
```

## Comparing `wnnet-1.2.4.tar` & `wnnet-1.2.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2024-03-07 21:20:24.899716 wnnet-1.2.4/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    35147 2023-01-19 23:05:37.000000 wnnet-1.2.4/LICENSE.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      188 2023-02-20 16:56:48.000000 wnnet-1.2.4/MANIFEST.in
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1782 2024-03-07 21:20:24.899027 wnnet-1.2.4/PKG-INFO
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      837 2023-03-18 14:20:36.000000 wnnet-1.2.4/README.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      107 2024-03-07 21:20:24.901018 wnnet-1.2.4/setup.cfg
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     6056 2023-03-18 14:18:12.000000 wnnet-1.2.4/setup.py
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2024-03-07 21:20:24.883993 wnnet-1.2.4/wnnet/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      302 2024-03-07 21:18:31.000000 wnnet-1.2.4/wnnet/__about__.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      197 2023-03-18 14:18:12.000000 wnnet-1.2.4/wnnet/__init__.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      993 2023-02-20 16:43:35.000000 wnnet-1.2.4/wnnet/consts.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    15695 2024-03-07 21:17:52.000000 wnnet-1.2.4/wnnet/flows.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    47918 2024-03-07 21:17:52.000000 wnnet-1.2.4/wnnet/graph.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     8551 2024-03-07 21:18:31.000000 wnnet-1.2.4/wnnet/net.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     4207 2024-03-07 21:17:52.000000 wnnet-1.2.4/wnnet/nuc.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     3553 2024-03-07 21:17:52.000000 wnnet-1.2.4/wnnet/reac.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      864 2023-01-19 23:05:37.000000 wnnet-1.2.4/wnnet/zones.py
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2024-03-07 21:20:24.896642 wnnet-1.2.4/wnnet.egg-info/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1782 2024-03-07 21:20:24.000000 wnnet-1.2.4/wnnet.egg-info/PKG-INFO
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      335 2024-03-07 21:20:24.000000 wnnet-1.2.4/wnnet.egg-info/SOURCES.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)        1 2024-03-07 21:20:24.000000 wnnet-1.2.4/wnnet.egg-info/dependency_links.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)       66 2024-03-07 21:20:24.000000 wnnet-1.2.4/wnnet.egg-info/requires.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)        6 2024-03-07 21:20:24.000000 wnnet-1.2.4/wnnet.egg-info/top_level.txt
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2024-04-05 21:38:31.679807 wnnet-1.2.5/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    35147 2023-01-19 23:05:37.000000 wnnet-1.2.5/LICENSE.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      188 2023-02-20 16:56:48.000000 wnnet-1.2.5/MANIFEST.in
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1782 2024-04-05 21:38:31.679278 wnnet-1.2.5/PKG-INFO
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      837 2023-03-18 14:20:36.000000 wnnet-1.2.5/README.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      107 2024-04-05 21:38:31.680890 wnnet-1.2.5/setup.cfg
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     6056 2023-03-18 14:18:12.000000 wnnet-1.2.5/setup.py
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2024-04-05 21:38:31.668801 wnnet-1.2.5/wnnet/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      302 2024-04-05 21:36:33.000000 wnnet-1.2.5/wnnet/__about__.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      197 2023-03-18 14:18:12.000000 wnnet-1.2.5/wnnet/__init__.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      993 2023-02-20 16:43:35.000000 wnnet-1.2.5/wnnet/consts.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    15695 2024-03-07 21:17:52.000000 wnnet-1.2.5/wnnet/flows.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    47912 2024-04-05 21:36:33.000000 wnnet-1.2.5/wnnet/graph.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     8551 2024-03-07 21:18:31.000000 wnnet-1.2.5/wnnet/net.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     4207 2024-03-07 21:17:52.000000 wnnet-1.2.5/wnnet/nuc.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     3553 2024-03-07 21:17:52.000000 wnnet-1.2.5/wnnet/reac.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      864 2023-01-19 23:05:37.000000 wnnet-1.2.5/wnnet/zones.py
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2024-04-05 21:38:31.677673 wnnet-1.2.5/wnnet.egg-info/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1782 2024-04-05 21:38:31.000000 wnnet-1.2.5/wnnet.egg-info/PKG-INFO
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      335 2024-04-05 21:38:31.000000 wnnet-1.2.5/wnnet.egg-info/SOURCES.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)        1 2024-04-05 21:38:31.000000 wnnet-1.2.5/wnnet.egg-info/dependency_links.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)       66 2024-04-05 21:38:31.000000 wnnet-1.2.5/wnnet.egg-info/requires.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)        6 2024-04-05 21:38:31.000000 wnnet-1.2.5/wnnet.egg-info/top_level.txt
```

### Comparing `wnnet-1.2.4/LICENSE.txt` & `wnnet-1.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wnnet-1.2.4/PKG-INFO` & `wnnet-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wnnet
-Version: 1.2.4
+Version: 1.2.5
 Summary: Python project to handle webnucleo reaction networks
 Home-page: https://github.com/mbradle/wnnet
 Author: Clemson University
 Author-email: mbradle@g.clemson.edu
 License: GPLv3+
 Project-URL: Bug Reports, https://github.com/mbradle/wnnet/issues
 Project-URL: Source, https://github.com/mbradle/wnnet/
```

### Comparing `wnnet-1.2.4/README.rst` & `wnnet-1.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `wnnet-1.2.4/setup.py` & `wnnet-1.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `wnnet-1.2.4/wnnet/consts.py` & `wnnet-1.2.5/wnnet/consts.py`

 * *Files identical despite different names*

### Comparing `wnnet-1.2.4/wnnet/flows.py` & `wnnet-1.2.5/wnnet/flows.py`

 * *Files identical despite different names*

### Comparing `wnnet-1.2.4/wnnet/graph.py` & `wnnet-1.2.5/wnnet/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -476,22 +476,23 @@
             for reaction in net.get_reactions(reac_xpath=color_tup[0]):
                 color[reaction] = color_tup[1]
 
         for edge in G.edges:
             G.edges[edge]["color"] = color[G.edges[edge]["reaction"]]
 
 
-def _get_pos_string(net, name, state_scaling):
+def _get_pos(net, name, state_scaling):
     z, a, state = net.xml.get_z_a_state_from_nuclide_name(name)
     n = a - z
     if state == "g":
         z -= state_scaling
     elif state == "m":
         z += state_scaling
-    return str(n) + "," + str(z) + "!"
+    return (n, z)
+    # return str(n) + ".," + str(z) + ".!"
 
 
 def _get_subset_and_anchors(net, induced_nuc_xpath):
     val = []
     dict = {}
     z_dict = {}
     nuclides = net.get_nuclides()
@@ -711,15 +712,15 @@
             DG.add_node(anchor, style="invis")
 
     # Get new subset
 
     S2 = nx.subgraph(DG, subset_nuclides)
 
     for node in S2.nodes:
-        S2.nodes[node]["pos"] = _get_pos_string(net, node, state_scaling)
+        S2.nodes[node]["pos"] = _get_pos(net, node, state_scaling)
         S2.nodes[node]["label"] = node_label_func(node)
 
     # Title
 
     DG.graph["label"] = title_func(f_max)
 
     _color_edges(S2, net, reaction_color_tuples)
@@ -1171,15 +1172,15 @@
     if node_label_func:
         _node_label_func = node_label_func
     else:
         g_names = net.xml.get_graphviz_names(list(S.nodes.keys()))
         _node_label_func = lambda name: make_node_label(name, g_names)
 
     for node in S.nodes:
-        S.nodes[node]["pos"] = _get_pos_string(net, node, state_scaling)
+        S.nodes[node]["pos"] = _get_pos(net, node, state_scaling)
         S.nodes[node]["label"] = _node_label_func(node)
 
     _color_edges(S, net, reaction_color_tuples)
 
     return S
 
 
@@ -1315,15 +1316,15 @@
             DG.add_node(anchor, style="invis")
 
     # Get new subset
 
     S2 = nx.subgraph(DG, subset_nuclides)
 
     for node in S2.nodes:
-        S2.nodes[node]["pos"] = _get_pos_string(net, node, state_scaling)
+        S2.nodes[node]["pos"] = _get_pos(net, node, state_scaling)
         S2.nodes[node]["label"] = zone_node_label_func(node)
 
     DG.graph["label"] = title_func(f_max)
 
     _color_edges(S2, net, reaction_color_tuples)
 
     return S2
```

### Comparing `wnnet-1.2.4/wnnet/net.py` & `wnnet-1.2.5/wnnet/net.py`

 * *Files identical despite different names*

### Comparing `wnnet-1.2.4/wnnet/nuc.py` & `wnnet-1.2.5/wnnet/nuc.py`

 * *Files identical despite different names*

### Comparing `wnnet-1.2.4/wnnet/reac.py` & `wnnet-1.2.5/wnnet/reac.py`

 * *Files identical despite different names*

### Comparing `wnnet-1.2.4/wnnet/zones.py` & `wnnet-1.2.5/wnnet/zones.py`

 * *Files identical despite different names*

### Comparing `wnnet-1.2.4/wnnet.egg-info/PKG-INFO` & `wnnet-1.2.5/wnnet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wnnet
-Version: 1.2.4
+Version: 1.2.5
 Summary: Python project to handle webnucleo reaction networks
 Home-page: https://github.com/mbradle/wnnet
 Author: Clemson University
 Author-email: mbradle@g.clemson.edu
 License: GPLv3+
 Project-URL: Bug Reports, https://github.com/mbradle/wnnet/issues
 Project-URL: Source, https://github.com/mbradle/wnnet/
```

