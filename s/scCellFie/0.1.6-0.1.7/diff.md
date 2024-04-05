# Comparing `tmp/scCellFie-0.1.6.tar.gz` & `tmp/scCellFie-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scCellFie-0.1.6.tar", last modified: Tue Apr  2 13:52:05 2024, max compression
+gzip compressed data, was "scCellFie-0.1.7.tar", last modified: Fri Apr  5 09:05:17 2024, max compression
```

## Comparing `scCellFie-0.1.6.tar` & `scCellFie-0.1.7.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.964008 scCellFie-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-02 13:52:01.000000 scCellFie-0.1.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-02 13:52:05.960008 scCellFie-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-02 13:52:01.000000 scCellFie-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.960008 scCellFie-0.1.6/scCellFie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-02 13:52:05.000000 scCellFie-0.1.6/scCellFie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-02 13:52:05.000000 scCellFie-0.1.6/scCellFie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:52:05.000000 scCellFie-0.1.6/scCellFie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-02 13:52:05.000000 scCellFie-0.1.6/scCellFie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 13:52:05.000000 scCellFie-0.1.6/scCellFie.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.956008 scCellFie-0.1.6/sccellfie/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.956008 scCellFie-0.1.6/sccellfie/expression/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/expression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/expression/aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.956008 scCellFie-0.1.6/sccellfie/expression/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/expression/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/expression/tests/test_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13213 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/expression/tests/test_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)     9981 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/expression/thresholds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.956008 scCellFie-0.1.6/sccellfie/external/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.956008 scCellFie-0.1.6/sccellfie/external/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/external/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/external/tests/test_tf_idf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/external/tf_idf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/gene_score.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.956008 scCellFie-0.1.6/sccellfie/io/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/io/load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/io/save_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.956008 scCellFie-0.1.6/sccellfie/io/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/io/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/io/tests/test_load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/io/tests/test_save_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/metabolic_task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.956008 scCellFie-0.1.6/sccellfie/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/preprocessing/prepare_inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.960008 scCellFie-0.1.6/sccellfie/preprocessing/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/preprocessing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/preprocessing/tests/test_prepare_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/reaction_activity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.960008 scCellFie-0.1.6/sccellfie/spatial/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/spatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/spatial/assortativity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/spatial/hotspots.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/spatial/knn_network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.960008 scCellFie-0.1.6/sccellfie/spatial/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/spatial/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/spatial/tests/test_assortativity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/spatial/tests/test_hotspots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/spatial/tests/test_knn_network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.960008 scCellFie-0.1.6/sccellfie/stats/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/stats/markers_from_task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.960008 scCellFie-0.1.6/sccellfie/stats/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/stats/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/stats/tests/test_markers_from_task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.960008 scCellFie-0.1.6/sccellfie/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/tests/test_gene_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/tests/test_metabolic_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/tests/test_reaction_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/tests/toy_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 13:52:05.964008 scCellFie-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-02 13:52:01.000000 scCellFie-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.843825 scCellFie-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-05 09:05:08.000000 scCellFie-0.1.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-05 09:05:17.843825 scCellFie-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-05 09:05:08.000000 scCellFie-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.843825 scCellFie-0.1.7/scCellFie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-05 09:05:17.000000 scCellFie-0.1.7/scCellFie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-05 09:05:17.000000 scCellFie-0.1.7/scCellFie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 09:05:17.000000 scCellFie-0.1.7/scCellFie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-05 09:05:17.000000 scCellFie-0.1.7/scCellFie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 09:05:17.000000 scCellFie-0.1.7/scCellFie.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.835825 scCellFie-0.1.7/sccellfie/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.835825 scCellFie-0.1.7/sccellfie/expression/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/expression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/expression/aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.835825 scCellFie-0.1.7/sccellfie/expression/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/expression/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/expression/tests/test_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13213 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/expression/tests/test_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9981 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/expression/thresholds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.835825 scCellFie-0.1.7/sccellfie/external/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.835825 scCellFie-0.1.7/sccellfie/external/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/external/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/external/tests/test_tf_idf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/external/tf_idf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/gene_score.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.839825 scCellFie-0.1.7/sccellfie/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/io/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/io/save_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.839825 scCellFie-0.1.7/sccellfie/io/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/io/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/io/tests/test_load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/io/tests/test_save_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/metabolic_task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.839825 scCellFie-0.1.7/sccellfie/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/preprocessing/prepare_inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.839825 scCellFie-0.1.7/sccellfie/preprocessing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/preprocessing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/preprocessing/tests/test_prepare_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/reaction_activity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.839825 scCellFie-0.1.7/sccellfie/spatial/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/spatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/spatial/assortativity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/spatial/hotspots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/spatial/knn_network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.839825 scCellFie-0.1.7/sccellfie/spatial/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/spatial/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/spatial/tests/test_assortativity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/spatial/tests/test_hotspots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/spatial/tests/test_knn_network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.843825 scCellFie-0.1.7/sccellfie/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/stats/markers_from_task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.843825 scCellFie-0.1.7/sccellfie/stats/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/stats/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/stats/tests/test_markers_from_task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.843825 scCellFie-0.1.7/sccellfie/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/tests/test_gene_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/tests/test_metabolic_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/tests/test_reaction_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/tests/toy_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 09:05:17.843825 scCellFie-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-05 09:05:08.000000 scCellFie-0.1.7/setup.py
```

### Comparing `scCellFie-0.1.6/LICENSE.txt` & `scCellFie-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/PKG-INFO` & `scCellFie-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scCellFie
-Version: 0.1.6
+Version: 0.1.7
 Summary: A tool for studying metabolic tasks from single-cell and spatial transcriptomics
 Home-page: https://github.com/earmingol/scCellFie
 Author: Erick Armingol
 Author-email: erickarmingol@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `scCellFie-0.1.6/README.md` & `scCellFie-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/scCellFie.egg-info/PKG-INFO` & `scCellFie-0.1.7/scCellFie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scCellFie
-Version: 0.1.6
+Version: 0.1.7
 Summary: A tool for studying metabolic tasks from single-cell and spatial transcriptomics
 Home-page: https://github.com/earmingol/scCellFie
 Author: Erick Armingol
 Author-email: erickarmingol@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `scCellFie-0.1.6/scCellFie.egg-info/SOURCES.txt` & `scCellFie-0.1.7/scCellFie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/sccellfie/expression/aggregation.py` & `scCellFie-0.1.7/sccellfie/expression/aggregation.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 
     gene_symbols : str or list, optional (default: None)
         Gene names to include in the aggregation. If a string is provided,
         it is converted to a single-element list. If `None`, all genes are included.
 
     agg_func : str, optional  (default: 'mean')
         The aggregation function to apply. Options are 'mean', 'median',
-        '25p' (25th percentile), and '75p' (75th percentile). The function
-        must be one of the keys in the `AGG_FUNC` dictionary.
+        '25p' (25th percentile), '75p' (75th percentile), and 'trimean' (0.5*Q2 + 0.25(Q1+Q3)).
+        The function must be one of the keys in the `AGG_FUNC` dictionary.
 
     use_raw : bool, optional  (default: False)
         Whether to use the data in adata.raw.X (True) or in adata.X (False).
 
     Returns
     -------
     agg_expression : pandas.DataFrame
@@ -91,8 +91,9 @@
     return agg_expression.transpose()
 
 
 AGG_FUNC = {'mean' : np.nanmean,
             'median' : np.nanmedian,
             '25p' : lambda x, axis: np.percentile(x, q=25, axis=axis),
             '75p' : lambda x, axis: np.percentile(x, q=75, axis=axis),
-            }
+            'trimean' : lambda x, axis: 0.5*np.percentile(x, q=50, axis=axis) + 0.25*(np.percentile(x, q=25, axis=axis) + np.percentile(x, q=75, axis=axis))
+            }
```

### Comparing `scCellFie-0.1.6/sccellfie/expression/tests/test_aggregation.py` & `scCellFie-0.1.7/sccellfie/expression/tests/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/sccellfie/expression/tests/test_threshold.py` & `scCellFie-0.1.7/sccellfie/expression/tests/test_threshold.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/sccellfie/expression/thresholds.py` & `scCellFie-0.1.7/sccellfie/expression/thresholds.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/sccellfie/external/tests/test_tf_idf.py` & `scCellFie-0.1.7/sccellfie/external/tests/test_tf_idf.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/sccellfie/external/tf_idf.py` & `scCellFie-0.1.7/sccellfie/external/tf_idf.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/sccellfie/gene_score.py` & `scCellFie-0.1.7/sccellfie/gene_score.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     if isinstance(gpr, cobra.core.gene.GPR):
         return compute_gpr_gene_score(gpr.body, gene_scores)
     elif isinstance(gpr, ast.Name):
         return gene_scores.get(gpr.id, 0), gpr.id  # Returns a default score of 0 if not found
     elif isinstance(gpr, ast.BoolOp):
         op = gpr.op
         if isinstance(op, ast.Or):
-            max_score = 0
+            max_score = float('-inf')
             max_gene = None
             for value in gpr.values:
                 score, gene = compute_gpr_gene_score(value, gene_scores)
                 if score > max_score:  # Find the maximum score
                     max_score, max_gene = score, gene
             return max_score, max_gene  # Return the maximum score and corresponding gene
         elif isinstance(op, ast.And):
```

### Comparing `scCellFie-0.1.6/sccellfie/io/load_data.py` & `scCellFie-0.1.7/sccellfie/io/load_data.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/sccellfie/io/save_data.py` & `scCellFie-0.1.7/sccellfie/io/save_data.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/sccellfie/io/tests/test_load_data.py` & `scCellFie-0.1.7/sccellfie/io/tests/test_load_data.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/sccellfie/io/tests/test_save_data.py` & `scCellFie-0.1.7/sccellfie/io/tests/test_save_data.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/sccellfie/metabolic_task.py` & `scCellFie-0.1.7/sccellfie/metabolic_task.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/sccellfie/preprocessing/prepare_inputs.py` & `scCellFie-0.1.7/sccellfie/preprocessing/prepare_inputs.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/sccellfie/preprocessing/tests/test_prepare_inputs.py` & `scCellFie-0.1.7/sccellfie/preprocessing/tests/test_prepare_inputs.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/sccellfie/reaction_activity.py` & `scCellFie-0.1.7/sccellfie/reaction_activity.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/sccellfie/spatial/assortativity.py` & `scCellFie-0.1.7/sccellfie/spatial/assortativity.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/sccellfie/spatial/hotspots.py` & `scCellFie-0.1.7/sccellfie/spatial/hotspots.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/sccellfie/spatial/knn_network.py` & `scCellFie-0.1.7/sccellfie/spatial/knn_network.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/sccellfie/spatial/tests/test_assortativity.py` & `scCellFie-0.1.7/sccellfie/spatial/tests/test_assortativity.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/sccellfie/spatial/tests/test_hotspots.py` & `scCellFie-0.1.7/sccellfie/spatial/tests/test_hotspots.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/sccellfie/spatial/tests/test_knn_network.py` & `scCellFie-0.1.7/sccellfie/spatial/tests/test_knn_network.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/sccellfie/stats/markers_from_task.py` & `scCellFie-0.1.7/sccellfie/stats/markers_from_task.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/sccellfie/stats/tests/test_markers_from_task.py` & `scCellFie-0.1.7/sccellfie/stats/tests/test_markers_from_task.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/sccellfie/tests/test_gene_score.py` & `scCellFie-0.1.7/sccellfie/tests/test_gene_score.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/sccellfie/tests/test_metabolic_task.py` & `scCellFie-0.1.7/sccellfie/tests/test_metabolic_task.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/sccellfie/tests/test_reaction_activity.py` & `scCellFie-0.1.7/sccellfie/tests/test_reaction_activity.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/sccellfie/tests/toy_inputs.py` & `scCellFie-0.1.7/sccellfie/tests/toy_inputs.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.6/setup.py` & `scCellFie-0.1.7/setup.py`

 * *Files identical despite different names*

