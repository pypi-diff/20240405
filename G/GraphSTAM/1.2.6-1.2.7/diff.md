# Comparing `tmp/GraphSTAM-1.2.6.tar.gz` & `tmp/GraphSTAM-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GraphSTAM-1.2.6.tar", last modified: Fri Feb 16 04:28:31 2024, max compression
+gzip compressed data, was "GraphSTAM-1.2.7.tar", last modified: Wed Mar  6 02:29:07 2024, max compression
```

## Comparing `GraphSTAM-1.2.6.tar` & `GraphSTAM-1.2.7.tar`

### file list

```diff
@@ -1,73 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:28:31.085053 GraphSTAM-1.2.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:28:31.077053 GraphSTAM-1.2.6/BasicGraph/
--rw-r--r--   0 runner    (1001) docker     (127)    95732 2024-02-16 04:28:22.000000 GraphSTAM-1.2.6/BasicGraph/GraphModelLib_v6_Simplified.py
--rw-r--r--   0 runner    (1001) docker     (127)    93802 2024-02-16 04:28:22.000000 GraphSTAM-1.2.6/BasicGraph/GraphModelLib_v6_Simplified_LSTMTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)    97627 2024-02-16 04:28:22.000000 GraphSTAM-1.2.6/BasicGraph/GraphModelLib_v6_Simplified_LSTMTransform_Oneshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    86239 2024-02-16 04:28:22.000000 GraphSTAM-1.2.6/BasicGraph/GraphModelLib_v6_Simplified_LSTMTransform_v0.1.2.py
--rw-r--r--   0 runner    (1001) docker     (127)    96046 2024-02-16 04:28:22.000000 GraphSTAM-1.2.6/BasicGraph/GraphModelLib_v6_Simplified_Oneshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    88802 2024-02-16 04:28:22.000000 GraphSTAM-1.2.6/BasicGraph/GraphModelLib_v6_Simplified_v0.1.2.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-02-16 04:28:22.000000 GraphSTAM-1.2.6/BasicGraph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:28:31.085053 GraphSTAM-1.2.6/GraphSTAM.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-02-16 04:28:31.000000 GraphSTAM-1.2.6/GraphSTAM.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-02-16 04:28:31.000000 GraphSTAM-1.2.6/GraphSTAM.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 04:28:31.000000 GraphSTAM-1.2.6/GraphSTAM.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-16 04:28:31.000000 GraphSTAM-1.2.6/GraphSTAM.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-02-16 04:28:31.085053 GraphSTAM-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:28:31.077053 GraphSTAM-1.2.6/SpatialTemporalGraph/
--rw-r--r--   0 runner    (1001) docker     (127)   116524 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/SpatialTemporalGraph/GraphModelLib_v5_SpatialTemporal.py
--rw-r--r--   0 runner    (1001) docker     (127)   113449 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/SpatialTemporalGraph/GraphModelLib_v5_SpatialTemporal_v0.1.2.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/SpatialTemporalGraph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:28:31.081053 GraphSTAM-1.2.6/TemporalSpatialGraph/
--rw-r--r--   0 runner    (1001) docker     (127)   111273 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/TemporalSpatialGraph/GraphModelLib_v6_TemporalSpatial.py
--rw-r--r--   0 runner    (1001) docker     (127)   110716 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/TemporalSpatialGraph/GraphModelLib_v6_TemporalSpatial_Large.py
--rw-r--r--   0 runner    (1001) docker     (127)   103980 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/TemporalSpatialGraph/GraphModelLib_v6_TemporalSpatial_Large_v0.1.2.py
--rw-r--r--   0 runner    (1001) docker     (127)   104502 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/TemporalSpatialGraph/GraphModelLib_v6_TemporalSpatial_v0.1.2.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/TemporalSpatialGraph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:28:31.081053 GraphSTAM-1.2.6/graphstam/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/graphstam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    57749 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/graphstam/graphstam.py
--rw-r--r--   0 runner    (1001) docker     (127)    31583 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/graphstam/graphstam_bkp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:28:31.073053 GraphSTAM-1.2.6/optimized/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:28:31.081053 GraphSTAM-1.2.6/optimized/BasicGraph/
--rw-r--r--   0 runner    (1001) docker     (127)    83727 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/optimized/BasicGraph/GraphModelLib_Simplified_LSTMTransform_Optimized.py
--rw-r--r--   0 runner    (1001) docker     (127)    84991 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/optimized/BasicGraph/GraphModelLib_Simplified_Optimized.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/optimized/BasicGraph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:28:31.081053 GraphSTAM-1.2.6/optimized/SpatialTemporalGraph/
--rw-r--r--   0 runner    (1001) docker     (127)   116524 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/optimized/SpatialTemporalGraph/GraphModelLib_SpatialTemporal_Optimized.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/optimized/SpatialTemporalGraph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:28:31.081053 GraphSTAM-1.2.6/optimized/TemporalSpatialGraph/
--rw-r--r--   0 runner    (1001) docker     (127)   110703 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/optimized/TemporalSpatialGraph/GraphModelLib_TemporalSpatial_Large_Optimized.py
--rw-r--r--   0 runner    (1001) docker     (127)   111248 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/optimized/TemporalSpatialGraph/GraphModelLib_TemporalSpatial_Optimized.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/optimized/TemporalSpatialGraph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:28:31.081053 GraphSTAM-1.2.6/optimized/graphstam/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/optimized/graphstam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    58158 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/optimized/graphstam/graphstam.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:28:31.073053 GraphSTAM-1.2.6/probabilistic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:28:31.085053 GraphSTAM-1.2.6/probabilistic/BasicGraph/
--rw-r--r--   0 runner    (1001) docker     (127)    86208 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/probabilistic/BasicGraph/GraphModelLib_Simplified_LGSSM.py
--rw-r--r--   0 runner    (1001) docker     (127)    85158 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/probabilistic/BasicGraph/GraphModelLib_Simplified_LSTMTransform_LGSSM.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/probabilistic/BasicGraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/probabilistic/BasicGraph/lgssm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/probabilistic/BasicGraph/lgssm_alt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:28:31.085053 GraphSTAM-1.2.6/probabilistic/graphstam/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/probabilistic/graphstam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    58183 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/probabilistic/graphstam/graphstam.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 04:28:31.085053 GraphSTAM-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:28:31.073053 GraphSTAM-1.2.6/smallgraph/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:28:31.085053 GraphSTAM-1.2.6/smallgraph/BasicGraph/
--rw-r--r--   0 runner    (1001) docker     (127)    84836 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/smallgraph/BasicGraph/GraphModelLib_Simplified_LSTMTransform_Optimized.py
--rw-r--r--   0 runner    (1001) docker     (127)    86088 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/smallgraph/BasicGraph/GraphModelLib_Simplified_Optimized.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/smallgraph/BasicGraph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:28:31.085053 GraphSTAM-1.2.6/smallgraph/graphstam/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/smallgraph/graphstam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    58163 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/smallgraph/graphstam/graphstam.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:28:31.073053 GraphSTAM-1.2.6/subgraphsampling/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:28:31.085053 GraphSTAM-1.2.6/subgraphsampling/BasicGraph/
--rw-r--r--   0 runner    (1001) docker     (127)    86007 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/subgraphsampling/BasicGraph/GraphModelLib_Simplified_LSTMTransform_Optimized.py
--rw-r--r--   0 runner    (1001) docker     (127)    87138 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/subgraphsampling/BasicGraph/GraphModelLib_Simplified_Optimized.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/subgraphsampling/BasicGraph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:28:31.085053 GraphSTAM-1.2.6/subgraphsampling/graphstam/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/subgraphsampling/graphstam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    58193 2024-02-16 04:28:23.000000 GraphSTAM-1.2.6/subgraphsampling/graphstam/graphstam.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 02:29:07.474420 GraphSTAM-1.2.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 02:29:07.462420 GraphSTAM-1.2.7/BasicGraph/
+-rw-r--r--   0 runner    (1001) docker     (127)    95732 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/BasicGraph/GraphModelLib_v6_Simplified.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93802 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/BasicGraph/GraphModelLib_v6_Simplified_LSTMTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97627 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/BasicGraph/GraphModelLib_v6_Simplified_LSTMTransform_Oneshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86239 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/BasicGraph/GraphModelLib_v6_Simplified_LSTMTransform_v0.1.2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96046 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/BasicGraph/GraphModelLib_v6_Simplified_Oneshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88802 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/BasicGraph/GraphModelLib_v6_Simplified_v0.1.2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/BasicGraph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 02:29:07.474420 GraphSTAM-1.2.7/GraphSTAM.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-06 02:29:07.000000 GraphSTAM-1.2.7/GraphSTAM.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-03-06 02:29:07.000000 GraphSTAM-1.2.7/GraphSTAM.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 02:29:07.000000 GraphSTAM-1.2.7/GraphSTAM.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-06 02:29:07.000000 GraphSTAM-1.2.7/GraphSTAM.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-06 02:29:07.474420 GraphSTAM-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 02:29:07.466420 GraphSTAM-1.2.7/SpatialTemporalGraph/
+-rw-r--r--   0 runner    (1001) docker     (127)   116524 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/SpatialTemporalGraph/GraphModelLib_v5_SpatialTemporal.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113449 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/SpatialTemporalGraph/GraphModelLib_v5_SpatialTemporal_v0.1.2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/SpatialTemporalGraph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 02:29:07.466420 GraphSTAM-1.2.7/TemporalSpatialGraph/
+-rw-r--r--   0 runner    (1001) docker     (127)   111273 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/TemporalSpatialGraph/GraphModelLib_v6_TemporalSpatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)   110716 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/TemporalSpatialGraph/GraphModelLib_v6_TemporalSpatial_Large.py
+-rw-r--r--   0 runner    (1001) docker     (127)   103980 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/TemporalSpatialGraph/GraphModelLib_v6_TemporalSpatial_Large_v0.1.2.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104502 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/TemporalSpatialGraph/GraphModelLib_v6_TemporalSpatial_v0.1.2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/TemporalSpatialGraph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 02:29:07.466420 GraphSTAM-1.2.7/graphstam/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/graphstam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57749 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/graphstam/graphstam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31583 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/graphstam/graphstam_bkp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 02:29:07.458420 GraphSTAM-1.2.7/hierarchical/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 02:29:07.470420 GraphSTAM-1.2.7/hierarchical/BasicGraph/
+-rw-r--r--   0 runner    (1001) docker     (127)    95079 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/hierarchical/BasicGraph/GraphModelLib_Simplified_LSTMTransform_Optimized.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89589 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/hierarchical/BasicGraph/GraphModelLib_Simplified_LSTMTransform_Optimized_gscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95442 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/hierarchical/BasicGraph/GraphModelLib_Simplified_LSTMTransform_Optimized_localscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86367 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/hierarchical/BasicGraph/GraphModelLib_Simplified_Optimized.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/hierarchical/BasicGraph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 02:29:07.470420 GraphSTAM-1.2.7/hierarchical/graphstam/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/hierarchical/graphstam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58173 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/hierarchical/graphstam/graphstam.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 02:29:07.462420 GraphSTAM-1.2.7/optimized/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 02:29:07.470420 GraphSTAM-1.2.7/optimized/BasicGraph/
+-rw-r--r--   0 runner    (1001) docker     (127)    85329 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/optimized/BasicGraph/GraphModelLib_Simplified_LSTMTransform_Optimized.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84991 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/optimized/BasicGraph/GraphModelLib_Simplified_Optimized.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/optimized/BasicGraph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 02:29:07.470420 GraphSTAM-1.2.7/optimized/SpatialTemporalGraph/
+-rw-r--r--   0 runner    (1001) docker     (127)   116524 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/optimized/SpatialTemporalGraph/GraphModelLib_SpatialTemporal_Optimized.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/optimized/SpatialTemporalGraph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 02:29:07.470420 GraphSTAM-1.2.7/optimized/TemporalSpatialGraph/
+-rw-r--r--   0 runner    (1001) docker     (127)   110703 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/optimized/TemporalSpatialGraph/GraphModelLib_TemporalSpatial_Large_Optimized.py
+-rw-r--r--   0 runner    (1001) docker     (127)   111248 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/optimized/TemporalSpatialGraph/GraphModelLib_TemporalSpatial_Optimized.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/optimized/TemporalSpatialGraph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 02:29:07.470420 GraphSTAM-1.2.7/optimized/graphstam/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/optimized/graphstam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58158 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/optimized/graphstam/graphstam.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 02:29:07.462420 GraphSTAM-1.2.7/probabilistic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 02:29:07.474420 GraphSTAM-1.2.7/probabilistic/BasicGraph/
+-rw-r--r--   0 runner    (1001) docker     (127)    86208 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/probabilistic/BasicGraph/GraphModelLib_Simplified_LGSSM.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85158 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/probabilistic/BasicGraph/GraphModelLib_Simplified_LSTMTransform_LGSSM.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/probabilistic/BasicGraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/probabilistic/BasicGraph/lgssm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/probabilistic/BasicGraph/lgssm_alt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 02:29:07.474420 GraphSTAM-1.2.7/probabilistic/graphstam/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/probabilistic/graphstam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58183 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/probabilistic/graphstam/graphstam.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 02:29:07.474420 GraphSTAM-1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 02:29:07.462420 GraphSTAM-1.2.7/smallgraph/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 02:29:07.474420 GraphSTAM-1.2.7/smallgraph/BasicGraph/
+-rw-r--r--   0 runner    (1001) docker     (127)    86695 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/smallgraph/BasicGraph/GraphModelLib_Simplified_LSTMTransform_Optimized.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86367 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/smallgraph/BasicGraph/GraphModelLib_Simplified_Optimized.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/smallgraph/BasicGraph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 02:29:07.474420 GraphSTAM-1.2.7/smallgraph/graphstam/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/smallgraph/graphstam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58163 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/smallgraph/graphstam/graphstam.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 02:29:07.462420 GraphSTAM-1.2.7/subgraphsampling/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 02:29:07.474420 GraphSTAM-1.2.7/subgraphsampling/BasicGraph/
+-rw-r--r--   0 runner    (1001) docker     (127)    86007 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/subgraphsampling/BasicGraph/GraphModelLib_Simplified_LSTMTransform_Optimized.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87138 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/subgraphsampling/BasicGraph/GraphModelLib_Simplified_Optimized.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/subgraphsampling/BasicGraph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 02:29:07.474420 GraphSTAM-1.2.7/subgraphsampling/graphstam/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/subgraphsampling/graphstam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58193 2024-03-06 02:29:02.000000 GraphSTAM-1.2.7/subgraphsampling/graphstam/graphstam.py
```

### Comparing `GraphSTAM-1.2.6/BasicGraph/GraphModelLib_v6_Simplified.py` & `GraphSTAM-1.2.7/BasicGraph/GraphModelLib_v6_Simplified.py`

 * *Files identical despite different names*

### Comparing `GraphSTAM-1.2.6/BasicGraph/GraphModelLib_v6_Simplified_LSTMTransform.py` & `GraphSTAM-1.2.7/BasicGraph/GraphModelLib_v6_Simplified_LSTMTransform.py`

 * *Files identical despite different names*

### Comparing `GraphSTAM-1.2.6/BasicGraph/GraphModelLib_v6_Simplified_LSTMTransform_Oneshot.py` & `GraphSTAM-1.2.7/BasicGraph/GraphModelLib_v6_Simplified_LSTMTransform_Oneshot.py`

 * *Files identical despite different names*

### Comparing `GraphSTAM-1.2.6/BasicGraph/GraphModelLib_v6_Simplified_LSTMTransform_v0.1.2.py` & `GraphSTAM-1.2.7/BasicGraph/GraphModelLib_v6_Simplified_LSTMTransform_v0.1.2.py`

 * *Files identical despite different names*

### Comparing `GraphSTAM-1.2.6/BasicGraph/GraphModelLib_v6_Simplified_Oneshot.py` & `GraphSTAM-1.2.7/BasicGraph/GraphModelLib_v6_Simplified_Oneshot.py`

 * *Files identical despite different names*

### Comparing `GraphSTAM-1.2.6/BasicGraph/GraphModelLib_v6_Simplified_v0.1.2.py` & `GraphSTAM-1.2.7/BasicGraph/GraphModelLib_v6_Simplified_v0.1.2.py`

 * *Files identical despite different names*

### Comparing `GraphSTAM-1.2.6/GraphSTAM.egg-info/PKG-INFO` & `GraphSTAM-1.2.7/GraphSTAM.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GraphSTAM
-Version: 1.2.6
+Version: 1.2.7
 Summary: Graph Based Spatio-Temporal Attention Models For Demand Forecasting
 Author: Rahul Sinha
 Author-email: rahul.sinha@unilever.com
 Description-Content-Type: text/markdown
 
 # GraphSTAM
 Graph Based Spatio-Temporal Attention Models
```

### Comparing `GraphSTAM-1.2.6/GraphSTAM.egg-info/SOURCES.txt` & `GraphSTAM-1.2.7/GraphSTAM.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,21 @@
 TemporalSpatialGraph/GraphModelLib_v6_TemporalSpatial_Large.py
 TemporalSpatialGraph/GraphModelLib_v6_TemporalSpatial_Large_v0.1.2.py
 TemporalSpatialGraph/GraphModelLib_v6_TemporalSpatial_v0.1.2.py
 TemporalSpatialGraph/__init__.py
 graphstam/__init__.py
 graphstam/graphstam.py
 graphstam/graphstam_bkp.py
+hierarchical/BasicGraph/GraphModelLib_Simplified_LSTMTransform_Optimized.py
+hierarchical/BasicGraph/GraphModelLib_Simplified_LSTMTransform_Optimized_gscale.py
+hierarchical/BasicGraph/GraphModelLib_Simplified_LSTMTransform_Optimized_localscale.py
+hierarchical/BasicGraph/GraphModelLib_Simplified_Optimized.py
+hierarchical/BasicGraph/__init__.py
+hierarchical/graphstam/__init__.py
+hierarchical/graphstam/graphstam.py
 optimized/BasicGraph/GraphModelLib_Simplified_LSTMTransform_Optimized.py
 optimized/BasicGraph/GraphModelLib_Simplified_Optimized.py
 optimized/BasicGraph/__init__.py
 optimized/SpatialTemporalGraph/GraphModelLib_SpatialTemporal_Optimized.py
 optimized/SpatialTemporalGraph/__init__.py
 optimized/TemporalSpatialGraph/GraphModelLib_TemporalSpatial_Large_Optimized.py
 optimized/TemporalSpatialGraph/GraphModelLib_TemporalSpatial_Optimized.py
```

### Comparing `GraphSTAM-1.2.6/PKG-INFO` & `GraphSTAM-1.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GraphSTAM
-Version: 1.2.6
+Version: 1.2.7
 Summary: Graph Based Spatio-Temporal Attention Models For Demand Forecasting
 Author: Rahul Sinha
 Author-email: rahul.sinha@unilever.com
 Description-Content-Type: text/markdown
 
 # GraphSTAM
 Graph Based Spatio-Temporal Attention Models
```

### Comparing `GraphSTAM-1.2.6/README.md` & `GraphSTAM-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `GraphSTAM-1.2.6/SpatialTemporalGraph/GraphModelLib_v5_SpatialTemporal.py` & `GraphSTAM-1.2.7/SpatialTemporalGraph/GraphModelLib_v5_SpatialTemporal.py`

 * *Files identical despite different names*

### Comparing `GraphSTAM-1.2.6/SpatialTemporalGraph/GraphModelLib_v5_SpatialTemporal_v0.1.2.py` & `GraphSTAM-1.2.7/SpatialTemporalGraph/GraphModelLib_v5_SpatialTemporal_v0.1.2.py`

 * *Files identical despite different names*

### Comparing `GraphSTAM-1.2.6/TemporalSpatialGraph/GraphModelLib_v6_TemporalSpatial.py` & `GraphSTAM-1.2.7/TemporalSpatialGraph/GraphModelLib_v6_TemporalSpatial.py`

 * *Files identical despite different names*

### Comparing `GraphSTAM-1.2.6/TemporalSpatialGraph/GraphModelLib_v6_TemporalSpatial_Large.py` & `GraphSTAM-1.2.7/TemporalSpatialGraph/GraphModelLib_v6_TemporalSpatial_Large.py`

 * *Files identical despite different names*

### Comparing `GraphSTAM-1.2.6/TemporalSpatialGraph/GraphModelLib_v6_TemporalSpatial_Large_v0.1.2.py` & `GraphSTAM-1.2.7/TemporalSpatialGraph/GraphModelLib_v6_TemporalSpatial_Large_v0.1.2.py`

 * *Files identical despite different names*

### Comparing `GraphSTAM-1.2.6/TemporalSpatialGraph/GraphModelLib_v6_TemporalSpatial_v0.1.2.py` & `GraphSTAM-1.2.7/TemporalSpatialGraph/GraphModelLib_v6_TemporalSpatial_v0.1.2.py`

 * *Files identical despite different names*

### Comparing `GraphSTAM-1.2.6/graphstam/graphstam.py` & `GraphSTAM-1.2.7/graphstam/graphstam.py`

 * *Files identical despite different names*

### Comparing `GraphSTAM-1.2.6/graphstam/graphstam_bkp.py` & `GraphSTAM-1.2.7/graphstam/graphstam_bkp.py`

 * *Files identical despite different names*

### Comparing `GraphSTAM-1.2.6/optimized/BasicGraph/GraphModelLib_Simplified_LSTMTransform_Optimized.py` & `GraphSTAM-1.2.7/subgraphsampling/BasicGraph/GraphModelLib_Simplified_LSTMTransform_Optimized.py`

 * *Files 2% similar despite different names*

```diff
@@ -1423,15 +1423,15 @@
         
         # for each split create graph dataset iterator
         print("gather snapshot graphs...")
         datasets = {}
         for df_type, df in df_dict.items():
             
             snap_periods_list = sorted(df[self.time_index_col].unique(), reverse=False)
-            
+
             # restrict samples for very large datasets based on interleaving
             if df_type == 'train':
                 snap_periods_list = snap_periods_list[int(self.max_lags - 1):]
 
             if (self.interleave > 1) and (df_type == 'train'):
                 snap_periods_list = snap_periods_list[0::self.interleave] + [snap_periods_list[-1]]
             
@@ -1655,14 +1655,18 @@
     def train(self, 
               lr, 
               min_epochs, 
               max_epochs, 
               patience, 
               min_delta, 
               model_prefix,
+              nloader_batch_size=500,
+              nloader_shuffle=True,
+              nloader_droplast=False,
+              nloader_directed=False,
               loss_type = 'Quantile',
               delta = 1.0,
               use_lr_scheduler=True, 
               scheduler_params={'factor':0.5, 'patience':3, 'threshold':0.0001, 'min_lr':0.00001},
               sample_weights=False):
         
         self.loss_type = loss_type
@@ -1694,76 +1698,36 @@
         train_loss_hist = []
         val_loss_hist = []
 
         def train_fn():
             self.model.train(True)
             total_examples = 0 
             total_loss = 0
-            for i, batch in enumerate(self.train_dataset):
-                if not self.grad_accum:
-                    optimizer.zero_grad()
-
-                batch = batch.to(self.device)
-                batch_size = batch.num_graphs
-                out = self.model(batch.x_dict, batch.edge_index_dict)
-                
-                # compute loss masking out N/A targets -- last snapshot
-                if self.loss_type == 'Quantile':
-                    try:
-                        loss = loss_fn.loss(out, batch[self.target_col].y)
-                    except:
-                        loss = loss_fn.loss(torch.unsqueeze(out, dim=1), batch[self.target_col].y)
-                    mask = torch.unsqueeze(batch[self.target_col].y_mask, dim=2)
-                elif self.loss_type == 'Huber':
-                    try:
-                        loss = loss_fn(out[:, -1, :], batch[self.target_col].y)
-                    except:
-                        loss = loss_fn(out, batch[self.target_col].y)
-                    mask = batch[self.target_col].y_mask
-                else:
-                    try:
-                        loss = loss_fn.loss(out[:, -1, :], batch[self.target_col].y)
-                    except:
-                        loss = loss_fn.loss(out, batch[self.target_col].y)
-                    mask = batch[self.target_col].y_mask
-                
-                if sample_weights:
-                    wt = batch[self.target_col].y_weight
-                else:
-                    wt = 1
-                
-                loss = torch.mean(loss*mask*wt)
+            for i, snap in enumerate(self.train_dataset):
+                # subgraph samples
+                loader = NeighborLoader(snap,
+                                        num_neighbors={key: [-1] for key in snap.edge_types},
+                                        shuffle=nloader_shuffle,
+                                        drop_last=nloader_droplast,
+                                        batch_size=nloader_batch_size,
+                                        directed=nloader_directed,
+                                        input_nodes=(self.target_col, torch.tensor(
+                                            np.random.randint(low=0, high=snap[self.target_col].num_nodes,
+                                                              size=snap[self.target_col].num_nodes).tolist()).type(
+                                            torch.long))
+                                        )
 
-                # normalize loss to account for batch accumulation
-                if self.grad_accum:
-                    loss = loss / self.accum_iter
-                    loss.backward()
-                    # weights update
-                    if ((i + 1) % self.accum_iter == 0) or (i + 1 == len(self.train_dataset)):
-                        optimizer.step()
+                for j, batch in enumerate(loader):
+                    if not self.grad_accum:
                         optimizer.zero_grad()
-                else:
-                    loss.backward()
-                    optimizer.step()
 
-                total_examples += batch_size
-                total_loss += float(loss)
-                
-            return total_loss / total_examples
-        
-        def test_fn():
-            self.model.train(False)
-            total_examples = 0 
-            total_loss = 0
-            with torch.no_grad(): 
-                for i, batch in enumerate(self.test_dataset):
-                    batch_size = batch.num_graphs
                     batch = batch.to(self.device)
+                    batch_size = batch.num_graphs
                     out = self.model(batch.x_dict, batch.edge_index_dict)
-                    
+
                     # compute loss masking out N/A targets -- last snapshot
                     if self.loss_type == 'Quantile':
                         try:
                             loss = loss_fn.loss(out, batch[self.target_col].y)
                         except:
                             loss = loss_fn.loss(torch.unsqueeze(out, dim=1), batch[self.target_col].y)
                         mask = torch.unsqueeze(batch[self.target_col].y_mask, dim=2)
@@ -1775,24 +1739,97 @@
                         mask = batch[self.target_col].y_mask
                     else:
                         try:
                             loss = loss_fn.loss(out[:, -1, :], batch[self.target_col].y)
                         except:
                             loss = loss_fn.loss(out, batch[self.target_col].y)
                         mask = batch[self.target_col].y_mask
-                    
+
                     if sample_weights:
                         wt = batch[self.target_col].y_weight
                     else:
                         wt = 1
-                    
-                    loss = torch.mean(loss*mask*wt) 
+
+                    loss = torch.mean(loss * mask * wt)
+
+                    # normalize loss to account for batch accumulation
+                    if self.grad_accum:
+                        loss = loss / self.accum_iter
+                        loss.backward()
+                        # weights update
+                        if ((j + 1) % self.accum_iter == 0) or (j + 1 == len(self.train_dataset)):
+                            optimizer.step()
+                            optimizer.zero_grad()
+                    else:
+                        loss.backward()
+                        optimizer.step()
+
                     total_examples += batch_size
                     total_loss += float(loss)
-                    
+
+                del loader
+                gc.collect()
+                
+            return total_loss / total_examples
+        
+        def test_fn():
+            self.model.train(False)
+            total_examples = 0 
+            total_loss = 0
+            with torch.no_grad(): 
+                for i, snap in enumerate(self.test_dataset):
+                    # subgraph samples
+                    loader = NeighborLoader(snap,
+                                            num_neighbors={key: [-1] for key in snap.edge_types},
+                                            shuffle=nloader_shuffle,
+                                            drop_last=nloader_droplast,
+                                            batch_size=nloader_batch_size,
+                                            directed=nloader_directed,
+                                            input_nodes=(self.target_col, torch.tensor(
+                                                np.random.randint(low=0, high=snap[self.target_col].num_nodes,
+                                                                  size=snap[self.target_col].num_nodes).tolist()).type(
+                                                torch.long))
+                                            )
+                    for j, batch in enumerate(loader):
+                        batch_size = batch.num_graphs
+                        batch = batch.to(self.device)
+                        out = self.model(batch.x_dict, batch.edge_index_dict)
+
+                        # compute loss masking out N/A targets -- last snapshot
+                        if self.loss_type == 'Quantile':
+                            try:
+                                loss = loss_fn.loss(out, batch[self.target_col].y)
+                            except:
+                                loss = loss_fn.loss(torch.unsqueeze(out, dim=1), batch[self.target_col].y)
+                            mask = torch.unsqueeze(batch[self.target_col].y_mask, dim=2)
+                        elif self.loss_type == 'Huber':
+                            try:
+                                loss = loss_fn(out[:, -1, :], batch[self.target_col].y)
+                            except:
+                                loss = loss_fn(out, batch[self.target_col].y)
+                            mask = batch[self.target_col].y_mask
+                        else:
+                            try:
+                                loss = loss_fn.loss(out[:, -1, :], batch[self.target_col].y)
+                            except:
+                                loss = loss_fn.loss(out, batch[self.target_col].y)
+                            mask = batch[self.target_col].y_mask
+
+                        if sample_weights:
+                            wt = batch[self.target_col].y_weight
+                        else:
+                            wt = 1
+
+                        loss = torch.mean(loss * mask * wt)
+                        total_examples += batch_size
+                        total_loss += float(loss)
+
+                    del loader
+                    gc.collect()
+
             return total_loss / total_examples
         
         for epoch in range(max_epochs):
             
             loss = train_fn()
             val_loss = test_fn()
```

### Comparing `GraphSTAM-1.2.6/optimized/BasicGraph/GraphModelLib_Simplified_Optimized.py` & `GraphSTAM-1.2.7/optimized/BasicGraph/GraphModelLib_Simplified_Optimized.py`

 * *Files identical despite different names*

### Comparing `GraphSTAM-1.2.6/optimized/SpatialTemporalGraph/GraphModelLib_SpatialTemporal_Optimized.py` & `GraphSTAM-1.2.7/optimized/SpatialTemporalGraph/GraphModelLib_SpatialTemporal_Optimized.py`

 * *Files identical despite different names*

### Comparing `GraphSTAM-1.2.6/optimized/TemporalSpatialGraph/GraphModelLib_TemporalSpatial_Large_Optimized.py` & `GraphSTAM-1.2.7/optimized/TemporalSpatialGraph/GraphModelLib_TemporalSpatial_Large_Optimized.py`

 * *Files identical despite different names*

### Comparing `GraphSTAM-1.2.6/optimized/TemporalSpatialGraph/GraphModelLib_TemporalSpatial_Optimized.py` & `GraphSTAM-1.2.7/optimized/TemporalSpatialGraph/GraphModelLib_TemporalSpatial_Optimized.py`

 * *Files identical despite different names*

### Comparing `GraphSTAM-1.2.6/optimized/graphstam/graphstam.py` & `GraphSTAM-1.2.7/optimized/graphstam/graphstam.py`

 * *Files identical despite different names*

### Comparing `GraphSTAM-1.2.6/probabilistic/BasicGraph/GraphModelLib_Simplified_LGSSM.py` & `GraphSTAM-1.2.7/probabilistic/BasicGraph/GraphModelLib_Simplified_LGSSM.py`

 * *Files identical despite different names*

### Comparing `GraphSTAM-1.2.6/probabilistic/BasicGraph/GraphModelLib_Simplified_LSTMTransform_LGSSM.py` & `GraphSTAM-1.2.7/probabilistic/BasicGraph/GraphModelLib_Simplified_LSTMTransform_LGSSM.py`

 * *Files identical despite different names*

### Comparing `GraphSTAM-1.2.6/probabilistic/BasicGraph/lgssm.py` & `GraphSTAM-1.2.7/probabilistic/BasicGraph/lgssm.py`

 * *Files identical despite different names*

### Comparing `GraphSTAM-1.2.6/probabilistic/BasicGraph/lgssm_alt.py` & `GraphSTAM-1.2.7/probabilistic/BasicGraph/lgssm_alt.py`

 * *Files identical despite different names*

### Comparing `GraphSTAM-1.2.6/probabilistic/graphstam/graphstam.py` & `GraphSTAM-1.2.7/probabilistic/graphstam/graphstam.py`

 * *Files identical despite different names*

### Comparing `GraphSTAM-1.2.6/setup.py` & `GraphSTAM-1.2.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 # The directory containing this file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="GraphSTAM",
-    version="1.2.6",
+    version="1.2.7",
     description="Graph Based Spatio-Temporal Attention Models For Demand Forecasting",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Rahul Sinha",
     author_email="rahul.sinha@unilever.com",
     packages=["graphstam", "BasicGraph", "SpatialTemporalGraph", "TemporalSpatialGraph", "optimized.graphstam",
               "optimized.BasicGraph", "optimized.SpatialTemporalGraph", "optimized.TemporalSpatialGraph",
               "probabilistic.graphstam", "probabilistic.BasicGraph", "subgraphsampling.graphstam", "subgraphsampling.BasicGraph",
-              "smallgraph.graphstam", "smallgraph.BasicGraph"],
+              "smallgraph.graphstam", "smallgraph.BasicGraph", "hierarchical.graphstam", "hierarchical.BasicGraph"],
     include_package_data=True,
     install_requires=[]
 )
```

### Comparing `GraphSTAM-1.2.6/smallgraph/BasicGraph/GraphModelLib_Simplified_LSTMTransform_Optimized.py` & `GraphSTAM-1.2.7/smallgraph/BasicGraph/GraphModelLib_Simplified_LSTMTransform_Optimized.py`

 * *Files 2% similar despite different names*

```diff
@@ -842,14 +842,16 @@
                  scaling_method = 'mean_scaling',
                  iqr_high = 0.75,
                  iqr_low = 0.25,
                  categorical_onehot_encoding = True,
                  directed_graph = True,
                  shuffle = True,
                  interleave = 1,
+                 recency_weights=False,
+                 recency_alpha=0,
                  PARALLEL_DATA_JOBS = 4, 
                  PARALLEL_DATA_JOBS_BATCHSIZE = 128):
         """
         col_dict: dictionary of various column groups {id_col:'',
                                                        target_col:'',
                                                        time_index_col:'',
                                                        global_context_col_list:[],
@@ -891,14 +893,16 @@
         self.scaling_method = scaling_method
         self.iqr_high = iqr_high
         self.iqr_low = iqr_low
         self.categorical_onehot_encoding = categorical_onehot_encoding
         self.directed_graph = directed_graph
         self.shuffle = shuffle
         self.interleave = interleave
+        self.recency_weights = recency_weights
+        self.recency_alpha = recency_alpha
         self.PARALLEL_DATA_JOBS = PARALLEL_DATA_JOBS
         self.PARALLEL_DATA_JOBS_BATCHSIZE = PARALLEL_DATA_JOBS_BATCHSIZE
         
         self.pad_constant = 0 #if self.scaling_method == 'mean_scaling' else -1
        
         # extract columnsets from col_dict
         self.id_col = self.col_dict.get('id_col', None)
@@ -1199,14 +1203,26 @@
         groups = df.groupby([self.id_col])
         padded_gdfs = Parallel(n_jobs=self.PARALLEL_DATA_JOBS, batch_size=self.PARALLEL_DATA_JOBS_BATCHSIZE, backend=backend, timeout=timeout)(delayed(self.pad_dataframe)(gdf, dateindex) for _, gdf in groups)
         gdf = pd.concat(padded_gdfs, axis=0)
         gdf = gdf.reset_index(drop=True)
         get_reusable_executor().shutdown(wait=True)
         return gdf
 
+    def get_relative_time_index(self, df):
+        """
+        Obtain a numeric feature indicating recency of a timestamp. This feature is also used to impl. recency_weights.
+        Ensure to run this after dataframe padding.
+        """
+        num_unique_ts = int(df[self.time_index_col].nunique())
+        df['relative_time_index'] = df.groupby(self.id_col)[self.time_index_col].transform(lambda x: np.arange(num_unique_ts))
+        df['relative_time_index'] = df['relative_time_index']/num_unique_ts
+        df['recency_weights'] = np.exp(self.recency_alpha * df['relative_time_index'])
+
+        return df
+
     def preprocess(self, data):
         
         print("   preprocessing dataframe - check for null columns...")
         # check null
         null_status, null_cols = self.check_null(data)
         
         if null_status:
@@ -1295,15 +1311,17 @@
         
         # get node features
 
         data[self.target_col].x = torch.tensor(df_snap[self.lead_lag_features_dict[self.target_col]].to_numpy(), dtype=torch.float)
         data[self.target_col].y = torch.tensor(df_snap[self.target_col].to_numpy().reshape(-1,1), dtype=torch.float)
         data[self.target_col].y_weight = torch.tensor(df_snap['Key_Weight'].to_numpy().reshape(-1,1), dtype=torch.float)
         data[self.target_col].y_mask = torch.tensor(df_snap['y_mask'].to_numpy().reshape(-1,1), dtype=torch.float)
-        
+        if self.recency_weights:
+            data[self.target_col].recency_weight = torch.tensor(df_snap['recency_weights'].to_numpy().reshape(-1, 1), dtype=torch.float)
+
         # store snapshot period
         data[self.target_col].time_attr = period
         
         for col in self.temporal_known_num_col_list:
             data[col].x = torch.tensor(df_snap[self.lead_lag_features_dict[col]].to_numpy(), dtype=torch.float)
             
         for col in self.temporal_unknown_num_col_list:
@@ -1403,15 +1421,19 @@
     def onetime_dataprep(self, df):
         # preprocess
         print("preprocessing dataframe...")
         df = self.preprocess(df)
 
         # pad dataframe if required (will return df unchanged if not)
         print("padding dataframe...")
-        self.onetime_prep_df = self.parallel_pad_dataframe(df)  # self.pad_dataframe(df)
+        df = self.parallel_pad_dataframe(df)  # self.pad_dataframe(df)
+        print("creating relative time index & recency weights...")
+        self.onetime_prep_df = self.get_relative_time_index(df)
+        # add 'relative time index' to self.temporal_known_num_col_list
+        self.temporal_known_num_col_list = self.temporal_known_num_col_list + ['relative_time_index']
 
     def create_train_test_dataset(self, df):
 
         # create lagged features
         print("create lead & lag features...")
         df = self.create_lead_lag_features(df)
 
@@ -1740,16 +1762,21 @@
                         loss = loss_fn.loss(out, batch[self.target_col].y)
                     mask = batch[self.target_col].y_mask
                 
                 if sample_weights:
                     wt = batch[self.target_col].y_weight
                 else:
                     wt = 1
+
+                if self.recency_weights:
+                    recency_wt = batch[self.target_col].recency_weight
+                else:
+                    recency_wt = 1
                 
-                loss = torch.mean(loss*mask*wt)
+                loss = torch.mean(loss*mask*wt*recency_wt)
 
                 # normalize loss to account for batch accumulation
                 if self.grad_accum:
                     loss = loss / self.accum_iter
                     loss.backward()
                     # weights update
                     if ((i + 1) % self.accum_iter == 0) or (i + 1 == len(self.train_dataset)):
@@ -1794,16 +1821,21 @@
                             loss = loss_fn.loss(out, batch[self.target_col].y)
                         mask = batch[self.target_col].y_mask
                     
                     if sample_weights:
                         wt = batch[self.target_col].y_weight
                     else:
                         wt = 1
+
+                    if self.recency_weights:
+                        recency_wt = batch[self.target_col].recency_weight
+                    else:
+                        recency_wt = 1
                     
-                    loss = torch.mean(loss*mask*wt) 
+                    loss = torch.mean(loss*mask*wt*recency_wt)
                     total_examples += batch_size
                     total_loss += float(loss)
                     
             return total_loss / total_examples
         
         for epoch in range(max_epochs):
             
@@ -1851,14 +1883,19 @@
                         try:
                             shutil.rmtree(m)
                         except:
                             pass
 
             if ((time_since_improvement > patience) and (epoch > min_epochs)) or (epoch == max_epochs - 1):
                 print("Terminating Training. Best Model: {}".format(self.best_model))
+                print("clearing gpu memory: ")
+                del self.train_dataset, self.test_dataset
+                gc.collect()
+                torch.cuda.empty_cache()
+
                 break
 
     def change_device(self, device='cpu'):
         self.device = torch.device(device)
         self.model.load_state_dict(torch.load(self.best_model, map_location=self.device))
 
     def disable_cuda_backend(self,):
@@ -1897,15 +1934,19 @@
             if not self.categorical_onehot_encoding:
                 self.temporal_known_num_col_list = list(set(self.temporal_known_num_col_list) - set(self.label_encoded_col_list))
                 self.temporal_unknown_num_col_list = list(set(self.temporal_unknown_num_col_list) - set(self.label_encoded_col_list))
         
             # infer dataset creation 
             infer_df, infer_dataset = self.create_infer_dataset(base_df, infer_till=t)
             output = infer_fn(self.model, self.best_model, infer_dataset)
-            
+
+            del infer_dataset
+            gc.collect()
+            torch.cuda.empty_cache()
+
             # select output quantile
             output_arr = output[0]
             output_arr = output_arr.cpu().numpy()
             
             # quantile selection
             min_qtile, max_qtile = min(self.forecast_quantiles), max(self.forecast_quantiles)
```

### Comparing `GraphSTAM-1.2.6/smallgraph/BasicGraph/GraphModelLib_Simplified_Optimized.py` & `GraphSTAM-1.2.7/hierarchical/BasicGraph/GraphModelLib_Simplified_Optimized.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 import torch_geometric.transforms as T
 from torch_geometric.utils import to_networkx
 
 # core data imports
 import pandas as pd
 import numpy as np
 import itertools
+import random
 from sklearn import preprocessing
 import warnings
 warnings.filterwarnings("ignore")
 
 # utilities imports
 from joblib import Parallel, delayed
 from joblib.externals.loky import get_reusable_executor
@@ -1126,15 +1127,15 @@
                     self.lead_lag_features_dict[col].append(f'{col}_lead_{lead}')
 
             if col in [self.target_col]:
                 self.node_features_label[col] = self.lead_lag_features_dict[col] + self.rolling_stat_cols
             else:
                 self.node_features_label[col] = self.lead_lag_features_dict[col]
 
-        # drop rows with NaNs in lag/lead cols
+        # don't drop rows with NaNs in lag/lead cols
         self.all_lead_lag_cols = list(itertools.chain.from_iterable([feat_col_list for col, feat_col_list in self.lead_lag_features_dict.items()]))
 
         return df
 
     def pad_dataframe(self, df, dateindex):
         # this ensures num nodes in a graph don't change from period to period. Essentially, we introduce dummy nodes.
         
@@ -1431,15 +1432,15 @@
         # split into train,test,infer
         print("splitting dataframe for training & testing...")
         train_df, test_df = self.split_train_test(df)
         
         df_dict = {'train': train_df, 'test': test_df}
 
         def parallel_snapshot_graphs(df, period):
-            df_snap = df[df[self.time_index_col]==period].reset_index(drop=True)
+            df_snap = df[df[self.time_index_col] == period].reset_index(drop=True)
             snapshot_graph = self.create_snapshot_graph(df_snap, period)
             return snapshot_graph
         
         # for each split create graph dataset iterator
         print("gather snapshot graphs...")
         datasets = {}
         for df_type, df in df_dict.items():
@@ -1860,14 +1861,19 @@
                         try:
                             shutil.rmtree(m)
                         except:
                             pass
 
             if ((time_since_improvement > patience) and (epoch > min_epochs)) or (epoch == max_epochs - 1):
                 print("Terminating Training. Best Model: {}".format(self.best_model))
+                print("clearing gpu memory: ")
+                del self.train_dataset, self.test_dataset
+                gc.collect()
+                torch.cuda.empty_cache()
+
                 break
     
     def infer(self, infer_start, infer_end, select_quantile, compute_mape=False):
         
         base_df = self.onetime_prep_df.copy()
 
         # get list of infer periods
@@ -1902,15 +1908,19 @@
             if not self.categorical_onehot_encoding:
                 self.temporal_known_num_col_list = list(set(self.temporal_known_num_col_list) - set(self.label_encoded_col_list))
                 self.temporal_unknown_num_col_list = list(set(self.temporal_unknown_num_col_list) - set(self.label_encoded_col_list))
         
             # infer dataset creation 
             infer_df, infer_dataset = self.create_infer_dataset(base_df, infer_till=t)
             output = infer_fn(self.model, self.best_model, infer_dataset)
-            
+
+            del infer_dataset
+            gc.collect()
+            torch.cuda.empty_cache()
+
             # select output quantile
             output_arr = output[0]
             output_arr = output_arr.cpu().numpy()
             
             # quantile selection
             min_qtile, max_qtile = min(self.forecast_quantiles), max(self.forecast_quantiles)
```

### Comparing `GraphSTAM-1.2.6/smallgraph/graphstam/graphstam.py` & `GraphSTAM-1.2.7/smallgraph/graphstam/graphstam.py`

 * *Files identical despite different names*

### Comparing `GraphSTAM-1.2.6/subgraphsampling/BasicGraph/GraphModelLib_Simplified_LSTMTransform_Optimized.py` & `GraphSTAM-1.2.7/optimized/BasicGraph/GraphModelLib_Simplified_LSTMTransform_Optimized.py`

 * *Files 2% similar despite different names*

```diff
@@ -841,14 +841,16 @@
                  scaling_method = 'mean_scaling',
                  iqr_high = 0.75,
                  iqr_low = 0.25,
                  categorical_onehot_encoding = True,
                  directed_graph = True,
                  shuffle = True,
                  interleave = 1,
+                 recency_weights=False,
+                 recency_alpha=0,
                  PARALLEL_DATA_JOBS = 4, 
                  PARALLEL_DATA_JOBS_BATCHSIZE = 128):
         """
         col_dict: dictionary of various column groups {id_col:'',
                                                        target_col:'',
                                                        time_index_col:'',
                                                        global_context_col_list:[],
@@ -888,14 +890,16 @@
         self.scaling_method = scaling_method
         self.iqr_high = iqr_high
         self.iqr_low = iqr_low
         self.categorical_onehot_encoding = categorical_onehot_encoding
         self.directed_graph = directed_graph
         self.shuffle = shuffle
         self.interleave = interleave
+        self.recency_weights = recency_weights
+        self.recency_alpha = recency_alpha
         self.PARALLEL_DATA_JOBS = PARALLEL_DATA_JOBS
         self.PARALLEL_DATA_JOBS_BATCHSIZE = PARALLEL_DATA_JOBS_BATCHSIZE
         
         self.pad_constant = 0 #if self.scaling_method == 'mean_scaling' else -1
        
         # extract columnsets from col_dict
         self.id_col = self.col_dict.get('id_col', None)
@@ -1194,14 +1198,26 @@
         groups = df.groupby([self.id_col])
         padded_gdfs = Parallel(n_jobs=self.PARALLEL_DATA_JOBS, batch_size=self.PARALLEL_DATA_JOBS_BATCHSIZE, backend=backend, timeout=timeout)(delayed(self.pad_dataframe)(gdf, dateindex) for _, gdf in groups)
         gdf = pd.concat(padded_gdfs, axis=0)
         gdf = gdf.reset_index(drop=True)
         get_reusable_executor().shutdown(wait=True)
         return gdf
 
+    def get_relative_time_index(self, df):
+        """
+        Obtain a numeric feature indicating recency of a timestamp. This feature is also used to impl. recency_weights.
+        Ensure to run this after dataframe padding.
+        """
+        num_unique_ts = int(df[self.time_index_col].nunique())
+        df['relative_time_index'] = df.groupby(self.id_col)[self.time_index_col].transform(lambda x: np.arange(num_unique_ts))
+        df['relative_time_index'] = df['relative_time_index']/num_unique_ts
+        df['recency_weights'] = np.exp(self.recency_alpha * df['relative_time_index'])
+
+        return df
+
     def preprocess(self, data):
         
         print("   preprocessing dataframe - check for null columns...")
         # check null
         null_status, null_cols = self.check_null(data)
         
         if null_status:
@@ -1290,15 +1306,17 @@
         
         # get node features
 
         data[self.target_col].x = torch.tensor(df_snap[self.lead_lag_features_dict[self.target_col]].to_numpy(), dtype=torch.float)
         data[self.target_col].y = torch.tensor(df_snap[self.target_col].to_numpy().reshape(-1,1), dtype=torch.float)
         data[self.target_col].y_weight = torch.tensor(df_snap['Key_Weight'].to_numpy().reshape(-1,1), dtype=torch.float)
         data[self.target_col].y_mask = torch.tensor(df_snap['y_mask'].to_numpy().reshape(-1,1), dtype=torch.float)
-        
+        if self.recency_weights:
+            data[self.target_col].recency_weight = torch.tensor(df_snap['recency_weights'].to_numpy().reshape(-1, 1), dtype=torch.float)
+
         # store snapshot period
         data[self.target_col].time_attr = period
         
         for col in self.temporal_known_num_col_list:
             data[col].x = torch.tensor(df_snap[self.lead_lag_features_dict[col]].to_numpy(), dtype=torch.float)
             
         for col in self.temporal_unknown_num_col_list:
@@ -1398,15 +1416,19 @@
     def onetime_dataprep(self, df):
         # preprocess
         print("preprocessing dataframe...")
         df = self.preprocess(df)
 
         # pad dataframe if required (will return df unchanged if not)
         print("padding dataframe...")
-        self.onetime_prep_df = self.parallel_pad_dataframe(df)  # self.pad_dataframe(df)
+        df = self.parallel_pad_dataframe(df)  # self.pad_dataframe(df)
+        print("creating relative time index & recency weights...")
+        self.onetime_prep_df = self.get_relative_time_index(df)
+        # add 'relative time index' to self.temporal_known_num_col_list
+        self.temporal_known_num_col_list = self.temporal_known_num_col_list + ['relative_time_index']
 
     def create_train_test_dataset(self, df):
 
         # create lagged features
         print("create lead & lag features...")
         df = self.create_lead_lag_features(df)
 
@@ -1423,15 +1445,15 @@
         
         # for each split create graph dataset iterator
         print("gather snapshot graphs...")
         datasets = {}
         for df_type, df in df_dict.items():
             
             snap_periods_list = sorted(df[self.time_index_col].unique(), reverse=False)
-
+            
             # restrict samples for very large datasets based on interleaving
             if df_type == 'train':
                 snap_periods_list = snap_periods_list[int(self.max_lags - 1):]
 
             if (self.interleave > 1) and (df_type == 'train'):
                 snap_periods_list = snap_periods_list[0::self.interleave] + [snap_periods_list[-1]]
             
@@ -1655,18 +1677,14 @@
     def train(self, 
               lr, 
               min_epochs, 
               max_epochs, 
               patience, 
               min_delta, 
               model_prefix,
-              nloader_batch_size=500,
-              nloader_shuffle=True,
-              nloader_droplast=False,
-              nloader_directed=False,
               loss_type = 'Quantile',
               delta = 1.0,
               use_lr_scheduler=True, 
               scheduler_params={'factor':0.5, 'patience':3, 'threshold':0.0001, 'min_lr':0.00001},
               sample_weights=False):
         
         self.loss_type = loss_type
@@ -1698,36 +1716,81 @@
         train_loss_hist = []
         val_loss_hist = []
 
         def train_fn():
             self.model.train(True)
             total_examples = 0 
             total_loss = 0
-            for i, snap in enumerate(self.train_dataset):
-                # subgraph samples
-                loader = NeighborLoader(snap,
-                                        num_neighbors={key: [-1] for key in snap.edge_types},
-                                        shuffle=nloader_shuffle,
-                                        drop_last=nloader_droplast,
-                                        batch_size=nloader_batch_size,
-                                        directed=nloader_directed,
-                                        input_nodes=(self.target_col, torch.tensor(
-                                            np.random.randint(low=0, high=snap[self.target_col].num_nodes,
-                                                              size=snap[self.target_col].num_nodes).tolist()).type(
-                                            torch.long))
-                                        )
+            for i, batch in enumerate(self.train_dataset):
+                if not self.grad_accum:
+                    optimizer.zero_grad()
+
+                batch = batch.to(self.device)
+                batch_size = batch.num_graphs
+                out = self.model(batch.x_dict, batch.edge_index_dict)
+                
+                # compute loss masking out N/A targets -- last snapshot
+                if self.loss_type == 'Quantile':
+                    try:
+                        loss = loss_fn.loss(out, batch[self.target_col].y)
+                    except:
+                        loss = loss_fn.loss(torch.unsqueeze(out, dim=1), batch[self.target_col].y)
+                    mask = torch.unsqueeze(batch[self.target_col].y_mask, dim=2)
+                elif self.loss_type == 'Huber':
+                    try:
+                        loss = loss_fn(out[:, -1, :], batch[self.target_col].y)
+                    except:
+                        loss = loss_fn(out, batch[self.target_col].y)
+                    mask = batch[self.target_col].y_mask
+                else:
+                    try:
+                        loss = loss_fn.loss(out[:, -1, :], batch[self.target_col].y)
+                    except:
+                        loss = loss_fn.loss(out, batch[self.target_col].y)
+                    mask = batch[self.target_col].y_mask
+                
+                if sample_weights:
+                    wt = batch[self.target_col].y_weight
+                else:
+                    wt = 1
+
+                if self.recency_weights:
+                    recency_wt = batch[self.target_col].recency_weight
+                else:
+                    recency_wt = 1
+                
+                loss = torch.mean(loss*mask*wt*recency_wt)
 
-                for j, batch in enumerate(loader):
-                    if not self.grad_accum:
+                # normalize loss to account for batch accumulation
+                if self.grad_accum:
+                    loss = loss / self.accum_iter
+                    loss.backward()
+                    # weights update
+                    if ((i + 1) % self.accum_iter == 0) or (i + 1 == len(self.train_dataset)):
+                        optimizer.step()
                         optimizer.zero_grad()
+                else:
+                    loss.backward()
+                    optimizer.step()
 
-                    batch = batch.to(self.device)
+                total_examples += batch_size
+                total_loss += float(loss)
+                
+            return total_loss / total_examples
+        
+        def test_fn():
+            self.model.train(False)
+            total_examples = 0 
+            total_loss = 0
+            with torch.no_grad(): 
+                for i, batch in enumerate(self.test_dataset):
                     batch_size = batch.num_graphs
+                    batch = batch.to(self.device)
                     out = self.model(batch.x_dict, batch.edge_index_dict)
-
+                    
                     # compute loss masking out N/A targets -- last snapshot
                     if self.loss_type == 'Quantile':
                         try:
                             loss = loss_fn.loss(out, batch[self.target_col].y)
                         except:
                             loss = loss_fn.loss(torch.unsqueeze(out, dim=1), batch[self.target_col].y)
                         mask = torch.unsqueeze(batch[self.target_col].y_mask, dim=2)
@@ -1739,97 +1802,29 @@
                         mask = batch[self.target_col].y_mask
                     else:
                         try:
                             loss = loss_fn.loss(out[:, -1, :], batch[self.target_col].y)
                         except:
                             loss = loss_fn.loss(out, batch[self.target_col].y)
                         mask = batch[self.target_col].y_mask
-
+                    
                     if sample_weights:
                         wt = batch[self.target_col].y_weight
                     else:
                         wt = 1
 
-                    loss = torch.mean(loss * mask * wt)
-
-                    # normalize loss to account for batch accumulation
-                    if self.grad_accum:
-                        loss = loss / self.accum_iter
-                        loss.backward()
-                        # weights update
-                        if ((j + 1) % self.accum_iter == 0) or (j + 1 == len(self.train_dataset)):
-                            optimizer.step()
-                            optimizer.zero_grad()
+                    if self.recency_weights:
+                        recency_wt = batch[self.target_col].recency_weight
                     else:
-                        loss.backward()
-                        optimizer.step()
-
+                        recency_wt = 1
+                    
+                    loss = torch.mean(loss*mask*wt*recency_wt)
                     total_examples += batch_size
                     total_loss += float(loss)
-
-                del loader
-                gc.collect()
-                
-            return total_loss / total_examples
-        
-        def test_fn():
-            self.model.train(False)
-            total_examples = 0 
-            total_loss = 0
-            with torch.no_grad(): 
-                for i, snap in enumerate(self.test_dataset):
-                    # subgraph samples
-                    loader = NeighborLoader(snap,
-                                            num_neighbors={key: [-1] for key in snap.edge_types},
-                                            shuffle=nloader_shuffle,
-                                            drop_last=nloader_droplast,
-                                            batch_size=nloader_batch_size,
-                                            directed=nloader_directed,
-                                            input_nodes=(self.target_col, torch.tensor(
-                                                np.random.randint(low=0, high=snap[self.target_col].num_nodes,
-                                                                  size=snap[self.target_col].num_nodes).tolist()).type(
-                                                torch.long))
-                                            )
-                    for j, batch in enumerate(loader):
-                        batch_size = batch.num_graphs
-                        batch = batch.to(self.device)
-                        out = self.model(batch.x_dict, batch.edge_index_dict)
-
-                        # compute loss masking out N/A targets -- last snapshot
-                        if self.loss_type == 'Quantile':
-                            try:
-                                loss = loss_fn.loss(out, batch[self.target_col].y)
-                            except:
-                                loss = loss_fn.loss(torch.unsqueeze(out, dim=1), batch[self.target_col].y)
-                            mask = torch.unsqueeze(batch[self.target_col].y_mask, dim=2)
-                        elif self.loss_type == 'Huber':
-                            try:
-                                loss = loss_fn(out[:, -1, :], batch[self.target_col].y)
-                            except:
-                                loss = loss_fn(out, batch[self.target_col].y)
-                            mask = batch[self.target_col].y_mask
-                        else:
-                            try:
-                                loss = loss_fn.loss(out[:, -1, :], batch[self.target_col].y)
-                            except:
-                                loss = loss_fn.loss(out, batch[self.target_col].y)
-                            mask = batch[self.target_col].y_mask
-
-                        if sample_weights:
-                            wt = batch[self.target_col].y_weight
-                        else:
-                            wt = 1
-
-                        loss = torch.mean(loss * mask * wt)
-                        total_examples += batch_size
-                        total_loss += float(loss)
-
-                    del loader
-                    gc.collect()
-
+                    
             return total_loss / total_examples
         
         for epoch in range(max_epochs):
             
             loss = train_fn()
             val_loss = test_fn()
```

### Comparing `GraphSTAM-1.2.6/subgraphsampling/BasicGraph/GraphModelLib_Simplified_Optimized.py` & `GraphSTAM-1.2.7/subgraphsampling/BasicGraph/GraphModelLib_Simplified_Optimized.py`

 * *Files identical despite different names*

### Comparing `GraphSTAM-1.2.6/subgraphsampling/graphstam/graphstam.py` & `GraphSTAM-1.2.7/subgraphsampling/graphstam/graphstam.py`

 * *Files identical despite different names*

