# Comparing `tmp/tui_dsmt-202404021248.tar.gz` & `tmp/tui_dsmt-202404051439.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tui_dsmt-202404021248.tar", last modified: Tue Apr  2 12:48:35 2024, max compression
+gzip compressed data, was "tui_dsmt-202404051439.tar", last modified: Fri Apr  5 14:39:42 2024, max compression
```

## Comparing `tui_dsmt-202404021248.tar` & `tui_dsmt-202404051439.tar`

### file list

```diff
@@ -1,51 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 12:48:35.815340 tui_dsmt-202404021248/
--rw-r--r--   0 root         (0) root         (0)      761 2024-04-02 12:48:35.815340 tui_dsmt-202404021248/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 12:48:35.815340 tui_dsmt-202404021248/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1101 2024-04-02 09:59:49.000000 tui_dsmt-202404021248/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 12:48:35.807340 tui_dsmt-202404021248/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 12:48:35.807340 tui_dsmt-202404021248/src/tui_dsmt/
--rw-rw-rw-   0 root         (0) root         (0)      569 2024-03-26 11:20:40.000000 tui_dsmt-202404021248/src/tui_dsmt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 12:48:35.807340 tui_dsmt-202404021248/src/tui_dsmt/clustering/
--rw-rw-rw-   0 root         (0) root         (0)      210 2024-04-02 12:48:28.000000 tui_dsmt-202404021248/src/tui_dsmt/clustering/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2691 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/clustering/animation.py
--rw-rw-rw-   0 root         (0) root         (0)    18964 2024-04-02 12:48:28.000000 tui_dsmt-202404021248/src/tui_dsmt/clustering/datasets.py
--rw-rw-rw-   0 root         (0) root         (0)      260 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/clustering/draw.py
--rw-rw-rw-   0 root         (0) root         (0)     1749 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/clustering/evaluation.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/clustering/interactive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 12:48:35.811340 tui_dsmt-202404021248/src/tui_dsmt/fpm/
--rw-rw-rw-   0 root         (0) root         (0)    14098 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/fpm/BruteForceFI.py
--rw-rw-rw-   0 root         (0) root         (0)     4055 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/fpm/ConditionalFPTree.py
--rw-rw-rw-   0 root         (0) root         (0)     5522 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/fpm/ConditionalPatternBase.py
--rw-rw-rw-   0 root         (0) root         (0)    10145 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/fpm/FPTree.py
--rw-rw-rw-   0 root         (0) root         (0)     1380 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/fpm/Itemset.py
--rw-rw-rw-   0 root         (0) root         (0)     3036 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/fpm/ItemsetGrid.py
--rw-rw-rw-   0 root         (0) root         (0)     5942 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/fpm/ItemsetGridApriori.py
--rw-rw-rw-   0 root         (0) root         (0)     5865 2024-03-26 11:20:40.000000 tui_dsmt-202404021248/src/tui_dsmt/fpm/ItemsetGridECLAT.py
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/fpm/SequentialDatabase.py
--rw-rw-rw-   0 root         (0) root         (0)     1129 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/fpm/SequentialItemset.py
--rw-rw-rw-   0 root         (0) root         (0)     1181 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/fpm/TransactionDatabase.py
--rw-rw-rw-   0 root         (0) root         (0)     2028 2024-03-14 12:42:03.000000 tui_dsmt-202404021248/src/tui_dsmt/fpm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 12:48:35.815340 tui_dsmt-202404021248/src/tui_dsmt/graph/
--rw-rw-rw-   0 root         (0) root         (0)     3894 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/BFS.py
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/BipartiteFlow.py
--rw-rw-rw-   0 root         (0) root         (0)     3478 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/DFS.py
--rw-rw-rw-   0 root         (0) root         (0)     5843 2024-03-26 11:20:40.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/Dijkstra.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/EdmondsKarp.py
--rw-rw-rw-   0 root         (0) root         (0)     4747 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/FordFulkerson.py
--rw-rw-rw-   0 root         (0) root         (0)     4461 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/Hall.py
--rw-rw-rw-   0 root         (0) root         (0)     2095 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/InteractiveGraph.py
--rw-rw-rw-   0 root         (0) root         (0)     3142 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/Kruskal.py
--rw-rw-rw-   0 root         (0) root         (0)     2234 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/MaximumFlow.py
--rw-rw-rw-   0 root         (0) root         (0)   419077 2024-03-26 11:20:40.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5267 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/game.py
--rw-rw-rw-   0 root         (0) root         (0)     5403 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/html.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/representation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 12:48:35.815340 tui_dsmt-202404021248/src/tui_dsmt/jpanim/
--rw-rw-rw-   0 root         (0) root         (0)     2063 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/jpanim/JupyterAnimation.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/jpanim/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 12:48:35.815340 tui_dsmt-202404021248/src/tui_dsmt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      761 2024-04-02 12:48:35.000000 tui_dsmt-202404021248/src/tui_dsmt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1366 2024-04-02 12:48:35.000000 tui_dsmt-202404021248/src/tui_dsmt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 12:48:35.000000 tui_dsmt-202404021248/src/tui_dsmt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      118 2024-04-02 12:48:35.000000 tui_dsmt-202404021248/src/tui_dsmt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-02 12:48:35.000000 tui_dsmt-202404021248/src/tui_dsmt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 14:39:42.598329 tui_dsmt-202404051439/
+-rw-r--r--   0 root         (0) root         (0)      761 2024-04-05 14:39:42.598329 tui_dsmt-202404051439/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 14:39:42.598329 tui_dsmt-202404051439/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1101 2024-04-05 14:39:32.000000 tui_dsmt-202404051439/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 14:39:42.582329 tui_dsmt-202404051439/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 14:39:42.586329 tui_dsmt-202404051439/src/tui_dsmt/
+-rw-rw-rw-   0 root         (0) root         (0)      569 2024-04-05 14:39:32.000000 tui_dsmt-202404051439/src/tui_dsmt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 14:39:42.586329 tui_dsmt-202404051439/src/tui_dsmt/clustering/
+-rw-rw-rw-   0 root         (0) root         (0)      210 2024-04-03 14:18:27.000000 tui_dsmt-202404051439/src/tui_dsmt/clustering/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2691 2024-03-08 12:22:54.000000 tui_dsmt-202404051439/src/tui_dsmt/clustering/animation.py
+-rw-rw-rw-   0 root         (0) root         (0)    18964 2024-04-03 14:18:27.000000 tui_dsmt-202404051439/src/tui_dsmt/clustering/datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)      260 2024-03-08 12:22:54.000000 tui_dsmt-202404051439/src/tui_dsmt/clustering/draw.py
+-rw-rw-rw-   0 root         (0) root         (0)     1749 2024-03-08 12:22:54.000000 tui_dsmt-202404051439/src/tui_dsmt/clustering/evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2024-03-08 12:22:54.000000 tui_dsmt-202404051439/src/tui_dsmt/clustering/interactive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 14:39:42.594329 tui_dsmt-202404051439/src/tui_dsmt/fpm/
+-rw-rw-rw-   0 root         (0) root         (0)    14098 2024-03-08 12:22:54.000000 tui_dsmt-202404051439/src/tui_dsmt/fpm/BruteForceFI.py
+-rw-rw-rw-   0 root         (0) root         (0)     4055 2024-03-08 12:22:54.000000 tui_dsmt-202404051439/src/tui_dsmt/fpm/ConditionalFPTree.py
+-rw-rw-rw-   0 root         (0) root         (0)     5522 2024-03-08 12:22:54.000000 tui_dsmt-202404051439/src/tui_dsmt/fpm/ConditionalPatternBase.py
+-rw-rw-rw-   0 root         (0) root         (0)    10145 2024-03-08 12:22:54.000000 tui_dsmt-202404051439/src/tui_dsmt/fpm/FPTree.py
+-rw-rw-rw-   0 root         (0) root         (0)    18908 2024-04-05 13:18:03.000000 tui_dsmt-202404051439/src/tui_dsmt/fpm/HashTree.py
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-04-03 14:18:27.000000 tui_dsmt-202404051439/src/tui_dsmt/fpm/Itemset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3036 2024-03-08 12:22:54.000000 tui_dsmt-202404051439/src/tui_dsmt/fpm/ItemsetGrid.py
+-rw-rw-rw-   0 root         (0) root         (0)     5942 2024-03-08 12:22:54.000000 tui_dsmt-202404051439/src/tui_dsmt/fpm/ItemsetGridApriori.py
+-rw-rw-rw-   0 root         (0) root         (0)     5865 2024-04-05 14:39:32.000000 tui_dsmt-202404051439/src/tui_dsmt/fpm/ItemsetGridECLAT.py
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-03-08 12:22:54.000000 tui_dsmt-202404051439/src/tui_dsmt/fpm/SequentialDatabase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2024-03-08 12:22:54.000000 tui_dsmt-202404051439/src/tui_dsmt/fpm/SequentialItemset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-03-08 12:22:54.000000 tui_dsmt-202404051439/src/tui_dsmt/fpm/TransactionDatabase.py
+-rw-rw-rw-   0 root         (0) root         (0)     2059 2024-04-05 14:39:32.000000 tui_dsmt-202404051439/src/tui_dsmt/fpm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 14:39:42.598329 tui_dsmt-202404051439/src/tui_dsmt/graph/
+-rw-rw-rw-   0 root         (0) root         (0)     3894 2024-03-08 12:22:54.000000 tui_dsmt-202404051439/src/tui_dsmt/graph/BFS.py
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-03-08 12:22:54.000000 tui_dsmt-202404051439/src/tui_dsmt/graph/BipartiteFlow.py
+-rw-rw-rw-   0 root         (0) root         (0)     3478 2024-03-08 12:22:54.000000 tui_dsmt-202404051439/src/tui_dsmt/graph/DFS.py
+-rw-rw-rw-   0 root         (0) root         (0)     5843 2024-04-05 14:39:32.000000 tui_dsmt-202404051439/src/tui_dsmt/graph/Dijkstra.py
+-rw-rw-rw-   0 root         (0) root         (0)      175 2024-03-08 12:22:54.000000 tui_dsmt-202404051439/src/tui_dsmt/graph/EdmondsKarp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4747 2024-03-08 12:22:54.000000 tui_dsmt-202404051439/src/tui_dsmt/graph/FordFulkerson.py
+-rw-rw-rw-   0 root         (0) root         (0)     4461 2024-03-08 12:22:54.000000 tui_dsmt-202404051439/src/tui_dsmt/graph/Hall.py
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2024-03-08 12:22:54.000000 tui_dsmt-202404051439/src/tui_dsmt/graph/InteractiveGraph.py
+-rw-rw-rw-   0 root         (0) root         (0)     3142 2024-03-08 12:22:54.000000 tui_dsmt-202404051439/src/tui_dsmt/graph/Kruskal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2024-03-08 12:22:54.000000 tui_dsmt-202404051439/src/tui_dsmt/graph/MaximumFlow.py
+-rw-rw-rw-   0 root         (0) root         (0)   419077 2024-04-05 14:39:32.000000 tui_dsmt-202404051439/src/tui_dsmt/graph/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5267 2024-03-08 12:22:54.000000 tui_dsmt-202404051439/src/tui_dsmt/graph/game.py
+-rw-rw-rw-   0 root         (0) root         (0)     5403 2024-03-08 12:22:54.000000 tui_dsmt-202404051439/src/tui_dsmt/graph/html.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2024-03-08 12:22:54.000000 tui_dsmt-202404051439/src/tui_dsmt/graph/representation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 14:39:42.598329 tui_dsmt-202404051439/src/tui_dsmt/jpanim/
+-rw-rw-rw-   0 root         (0) root         (0)     2302 2024-04-04 10:55:10.000000 tui_dsmt-202404051439/src/tui_dsmt/jpanim/JupyterAnimation.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-03-08 12:22:54.000000 tui_dsmt-202404051439/src/tui_dsmt/jpanim/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 14:39:42.598329 tui_dsmt-202404051439/src/tui_dsmt/util/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-03 14:18:27.000000 tui_dsmt-202404051439/src/tui_dsmt/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 14:39:42.598329 tui_dsmt-202404051439/src/tui_dsmt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      761 2024-04-05 14:39:42.000000 tui_dsmt-202404051439/src/tui_dsmt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1425 2024-04-05 14:39:42.000000 tui_dsmt-202404051439/src/tui_dsmt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 14:39:42.000000 tui_dsmt-202404051439/src/tui_dsmt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      118 2024-04-05 14:39:42.000000 tui_dsmt-202404051439/src/tui_dsmt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-05 14:39:42.000000 tui_dsmt-202404051439/src/tui_dsmt.egg-info/top_level.txt
```

### Comparing `tui_dsmt-202404021248/PKG-INFO` & `tui_dsmt-202404051439/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui_dsmt
-Version: 202404021248
+Version: 202404051439
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-methoden-und-techniken
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tui_dsmt-202404021248/setup.py` & `tui_dsmt-202404051439/setup.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/__init__.py` & `tui_dsmt-202404051439/src/tui_dsmt/__init__.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/clustering/animation.py` & `tui_dsmt-202404051439/src/tui_dsmt/clustering/animation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/clustering/datasets.py` & `tui_dsmt-202404051439/src/tui_dsmt/clustering/datasets.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/clustering/evaluation.py` & `tui_dsmt-202404051439/src/tui_dsmt/clustering/evaluation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/clustering/interactive.py` & `tui_dsmt-202404051439/src/tui_dsmt/clustering/interactive.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/fpm/BruteForceFI.py` & `tui_dsmt-202404051439/src/tui_dsmt/fpm/BruteForceFI.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/fpm/ConditionalFPTree.py` & `tui_dsmt-202404051439/src/tui_dsmt/fpm/ConditionalFPTree.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/fpm/ConditionalPatternBase.py` & `tui_dsmt-202404051439/src/tui_dsmt/fpm/ConditionalPatternBase.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/fpm/FPTree.py` & `tui_dsmt-202404051439/src/tui_dsmt/fpm/FPTree.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/fpm/Itemset.py` & `tui_dsmt-202404051439/src/tui_dsmt/fpm/Itemset.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,18 +15,21 @@
         else:
             return super().__getitem__(key)
 
     @property
     def set(self):
         return set(self)
 
+    def is_subset(self, transaction):
+        return self.set.issubset(transaction)
+
     def count_in(self, transactions):
         c = 0
         for _, items in transactions:
-            if self.set.issubset(items):
+            if self.is_subset(items):
                 c += 1
 
         return c
 
     def support_in(self, transactions):
         return self.count_in(transactions) / len(transactions)
```

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/fpm/ItemsetGrid.py` & `tui_dsmt-202404051439/src/tui_dsmt/fpm/ItemsetGrid.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/fpm/ItemsetGridApriori.py` & `tui_dsmt-202404051439/src/tui_dsmt/fpm/ItemsetGridApriori.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/fpm/ItemsetGridECLAT.py` & `tui_dsmt-202404051439/src/tui_dsmt/fpm/ItemsetGridECLAT.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/fpm/SequentialDatabase.py` & `tui_dsmt-202404051439/src/tui_dsmt/fpm/SequentialDatabase.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/fpm/SequentialItemset.py` & `tui_dsmt-202404051439/src/tui_dsmt/fpm/SequentialItemset.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/fpm/TransactionDatabase.py` & `tui_dsmt-202404051439/src/tui_dsmt/fpm/TransactionDatabase.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/fpm/__init__.py` & `tui_dsmt-202404051439/src/tui_dsmt/fpm/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .BruteForceFI import BruteForceFI
 from .FPTree import FPTree
+from .HashTree import HashTree
 from .Itemset import Itemset
 from .ItemsetGrid import ItemsetGrid
 from .ItemsetGridApriori import ItemsetGridApriori
 from .ItemsetGridECLAT import ItemsetGridECLAT
 from .SequentialDatabase import SequentialDatabase
 from .SequentialItemset import SequentialItemset
 from .TransactionDatabase import TransactionDatabase
```

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/graph/BFS.py` & `tui_dsmt-202404051439/src/tui_dsmt/graph/BFS.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/graph/BipartiteFlow.py` & `tui_dsmt-202404051439/src/tui_dsmt/graph/BipartiteFlow.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/graph/DFS.py` & `tui_dsmt-202404051439/src/tui_dsmt/graph/DFS.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/graph/Dijkstra.py` & `tui_dsmt-202404051439/src/tui_dsmt/graph/Dijkstra.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/graph/FordFulkerson.py` & `tui_dsmt-202404051439/src/tui_dsmt/graph/FordFulkerson.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/graph/Hall.py` & `tui_dsmt-202404051439/src/tui_dsmt/graph/Hall.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/graph/InteractiveGraph.py` & `tui_dsmt-202404051439/src/tui_dsmt/graph/InteractiveGraph.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/graph/Kruskal.py` & `tui_dsmt-202404051439/src/tui_dsmt/graph/Kruskal.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/graph/MaximumFlow.py` & `tui_dsmt-202404051439/src/tui_dsmt/graph/MaximumFlow.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/graph/__init__.py` & `tui_dsmt-202404051439/src/tui_dsmt/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/graph/game.py` & `tui_dsmt-202404051439/src/tui_dsmt/graph/game.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/graph/html.py` & `tui_dsmt-202404051439/src/tui_dsmt/graph/html.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/graph/representation.py` & `tui_dsmt-202404051439/src/tui_dsmt/graph/representation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404021248/src/tui_dsmt/jpanim/JupyterAnimation.py` & `tui_dsmt-202404051439/src/tui_dsmt/jpanim/JupyterAnimation.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,23 +5,28 @@
 
 from IPython.core.display import HTML
 
 __location__ = os.path.realpath(os.path.join(os.getcwd(), os.path.dirname(__file__)))
 
 
 class JupyterAnimation(HTML):
-    def __init__(self, html: str, frames: Dict[str, Dict], style: Optional[List[str] | str] = None):
+    def __init__(self, html: str, frames: Dict[str, Dict], style: List[str] | str = None, js: List[str] | str = None):
         self._html: str = html
         self._frames: Dict[str, Dict] = frames
 
         if isinstance(style, list):
             self._style: str = '\n'.join(style)
         else:
             self._style: str = style or ''
 
+        if isinstance(js, list):
+            self._js: str = '\n'.join(js)
+        else:
+            self._js: str = js or ''
+
         self._id: str = str(uuid4()).replace('-', '')
 
         super().__init__(self._construct())
 
     def _construct(self) -> str:
         # read templates from file
         with open(os.path.join(__location__, 'resources', 'style.css')) as css_file:
@@ -32,14 +37,17 @@
                 html = html_file.read()
         else:
             html = ''
 
         with open(os.path.join(__location__, 'resources', 'script.js')) as js_file:
             js = js_file.read()
 
+        # inject additional javascript
+        js = js.replace('// <injected js>', self._js)
+
         # convert frame data to json
         frames = json.dumps([{
             '__key': key,
             **frame
         } for key, frame in self._frames.items()], indent=4)
 
         # return string containing the content
```

### Comparing `tui_dsmt-202404021248/src/tui_dsmt.egg-info/PKG-INFO` & `tui_dsmt-202404051439/src/tui_dsmt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui_dsmt
-Version: 202404021248
+Version: 202404051439
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-methoden-und-techniken
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tui_dsmt-202404021248/src/tui_dsmt.egg-info/SOURCES.txt` & `tui_dsmt-202404051439/src/tui_dsmt.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 src/tui_dsmt/clustering/draw.py
 src/tui_dsmt/clustering/evaluation.py
 src/tui_dsmt/clustering/interactive.py
 src/tui_dsmt/fpm/BruteForceFI.py
 src/tui_dsmt/fpm/ConditionalFPTree.py
 src/tui_dsmt/fpm/ConditionalPatternBase.py
 src/tui_dsmt/fpm/FPTree.py
+src/tui_dsmt/fpm/HashTree.py
 src/tui_dsmt/fpm/Itemset.py
 src/tui_dsmt/fpm/ItemsetGrid.py
 src/tui_dsmt/fpm/ItemsetGridApriori.py
 src/tui_dsmt/fpm/ItemsetGridECLAT.py
 src/tui_dsmt/fpm/SequentialDatabase.py
 src/tui_dsmt/fpm/SequentialItemset.py
 src/tui_dsmt/fpm/TransactionDatabase.py
@@ -34,8 +35,9 @@
 src/tui_dsmt/graph/Kruskal.py
 src/tui_dsmt/graph/MaximumFlow.py
 src/tui_dsmt/graph/__init__.py
 src/tui_dsmt/graph/game.py
 src/tui_dsmt/graph/html.py
 src/tui_dsmt/graph/representation.py
 src/tui_dsmt/jpanim/JupyterAnimation.py
-src/tui_dsmt/jpanim/__init__.py
+src/tui_dsmt/jpanim/__init__.py
+src/tui_dsmt/util/__init__.py
```

