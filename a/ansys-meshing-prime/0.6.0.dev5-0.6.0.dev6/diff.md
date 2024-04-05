# Comparing `tmp/ansys_meshing_prime-0.6.0.dev5.tar.gz` & `tmp/ansys_meshing_prime-0.6.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_meshing_prime-0.6.0.dev5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_meshing_prime-0.6.0.dev6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_meshing_prime-0.6.0.dev5.tar` & `ansys_meshing_prime-0.6.0.dev6.tar`

### file list

```diff
@@ -1,131 +1,131 @@
--rw-r--r--   0        0        0     1090 2024-03-19 15:03:30.890977 ansys_meshing_prime-0.6.0.dev5/LICENSE
--rw-r--r--   0        0        0     4090 2024-03-19 15:03:30.890977 ansys_meshing_prime-0.6.0.dev5/README.md
--rw-r--r--   0        0        0     2408 2024-03-19 15:03:30.970976 ansys_meshing_prime-0.6.0.dev5/pyproject.toml
--rw-r--r--   0        0        0     6218 2024-03-19 15:03:30.970976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/__init__.py
--rw-r--r--   0        0        0      428 2024-03-19 15:03:30.970976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/_version.py
--rw-r--r--   0        0        0     2654 2024-03-19 15:03:30.970976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/automesh.py
--rw-r--r--   0        0        0    61369 2024-03-19 15:03:30.970976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/automeshstructs.py
--rw-r--r--   0        0        0    11093 2024-03-19 15:03:30.970976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/autoquadmesher.py
--rw-r--r--   0        0        0   165219 2024-03-19 15:03:30.970976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/autoquadmesherstructs.py
--rw-r--r--   0        0        0     6123 2024-03-19 15:03:30.970976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/boundaryfittednurbs.py
--rw-r--r--   0        0        0     3977 2024-03-19 15:03:30.970976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/collapsetool.py
--rw-r--r--   0        0        0    14791 2024-03-19 15:03:30.970976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/collapsetoolstructs.py
--rw-r--r--   0        0        0    26643 2024-03-19 15:03:30.970976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/commonstructs.py
--rw-r--r--   0        0        0     3875 2024-03-19 15:03:30.970976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/commontypes.py
--rw-r--r--   0        0        0    14928 2024-03-19 15:03:30.970976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/connect.py
--rw-r--r--   0        0        0    95082 2024-03-19 15:03:30.970976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/connectstructs.py
--rw-r--r--   0        0        0    12218 2024-03-19 15:03:30.970976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/controldata.py
--rw-r--r--   0        0        0    91621 2024-03-19 15:03:30.970976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/controlstructs.py
--rw-r--r--   0        0        0      714 2024-03-19 15:03:30.970976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/coreobject.py
--rw-r--r--   0        0        0     3433 2024-03-19 15:03:30.970976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/deletetool.py
--rw-r--r--   0        0        0    14080 2024-03-19 15:03:30.970976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/deletetoolstructs.py
--rw-r--r--   0        0        0     5585 2024-03-19 15:03:30.970976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/featureextraction.py
--rw-r--r--   0        0        0    35361 2024-03-19 15:03:30.970976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/featureextractionstructs.py
--rw-r--r--   0        0        0    31259 2024-03-19 15:03:30.970976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/fileio.py
--rw-r--r--   0        0        0   162937 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/fileiostructs.py
--rw-r--r--   0        0        0    71909 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/igastructs.py
--rw-r--r--   0        0        0     4136 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/materialpointmanager.py
--rw-r--r--   0        0        0    16431 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/materialpointmanagerstructs.py
--rw-r--r--   0        0        0     4866 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/meshinfo.py
--rw-r--r--   0        0        0    60305 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/meshinfostructs.py
--rw-r--r--   0        0        0    16840 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/model.py
--rw-r--r--   0        0        0    27452 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/modelstructs.py
--rw-r--r--   0        0        0     3803 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/morpher.py
--rw-r--r--   0        0        0     7876 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/morpherbcsstructs.py
--rw-r--r--   0        0        0    24470 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/morpherstructs.py
--rw-r--r--   0        0        0     7869 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/multizonecontrol.py
--rw-r--r--   0        0        0    59442 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/part.py
--rw-r--r--   0        0        0   168878 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/partstructs.py
--rw-r--r--   0        0        0     7671 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/periodiccontrol.py
--rw-r--r--   0        0        0    13543 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/periodiccontrolstructs.py
--rw-r--r--   0        0        0    33934 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/primeconfig.py
--rw-r--r--   0        0        0     5733 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/prismcontrol.py
--rw-r--r--   0        0        0    14608 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/prismcontrolstructs.py
--rw-r--r--   0        0        0     2937 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/quadtospline.py
--rw-r--r--   0        0        0     7253 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/scaffolder.py
--rw-r--r--   0        0        0    38220 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/scaffolderstructs.py
--rw-r--r--   0        0        0    18400 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/sizecontrol.py
--rw-r--r--   0        0        0    53218 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/sizecontrolstructs.py
--rw-r--r--   0        0        0     2794 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/sizefield.py
--rw-r--r--   0        0        0    19028 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/sizefieldstructs.py
--rw-r--r--   0        0        0     4286 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/splittoolstructs.py
--rw-r--r--   0        0        0    21687 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/surfacesearch.py
--rw-r--r--   0        0        0   124157 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/surfacesearchstructs.py
--rw-r--r--   0        0        0    25421 2024-03-19 15:03:30.974976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/surfaceutilities.py
--rw-r--r--   0        0        0   153390 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/surfaceutilitystructs.py
--rw-r--r--   0        0        0     7198 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/surfer.py
--rw-r--r--   0        0        0    45142 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/surferstructs.py
--rw-r--r--   0        0        0     4454 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/thinvolumecontrol.py
--rw-r--r--   0        0        0     7117 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/thinvolumecontrolstructs.py
--rw-r--r--   0        0        0    10182 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/topodata.py
--rw-r--r--   0        0        0     9409 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/topodatastructs.py
--rw-r--r--   0        0        0     1761 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/toposearchstructs.py
--rw-r--r--   0        0        0     2650 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/topoutilities.py
--rw-r--r--   0        0        0    13257 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/topoutilitystructs.py
--rw-r--r--   0        0        0     2966 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/transform.py
--rw-r--r--   0        0        0     8817 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/transformstructs.py
--rw-r--r--   0        0        0     5986 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/volumecontrol.py
--rw-r--r--   0        0        0     6304 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/volumecontrolstructs.py
--rw-r--r--   0        0        0     6962 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/volumemeshtool.py
--rw-r--r--   0        0        0    29781 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/volumemeshtoolstructs.py
--rw-r--r--   0        0        0     2763 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/volumesearch.py
--rw-r--r--   0        0        0    25627 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/volumesearchstructs.py
--rw-r--r--   0        0        0     4896 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/volumesweeper.py
--rw-r--r--   0        0        0    25625 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/volumesweeperstructs.py
--rw-r--r--   0        0        0     2927 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/vtcomposer.py
--rw-r--r--   0        0        0     8476 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/vtcomposerstructs.py
--rw-r--r--   0        0        0     7270 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/wrapper.py
--rw-r--r--   0        0        0    10832 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/wrappercontrol.py
--rw-r--r--   0        0        0    89981 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/wrapperstructs.py
--rw-r--r--   0        0        0    15856 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/controldata.py
--rw-r--r--   0        0        0   121829 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/dynaexportutils.py
--rw-r--r--   0        0        0    20701 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/fileio.py
--rw-r--r--   0        0        0   161431 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/mapdlcdbexportutils.py
--rw-r--r--   0        0        0    11168 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/model.py
--rw-r--r--   0        0        0      767 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/multizonecontrol.py
--rw-r--r--   0        0        0     4181 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/part.py
--rw-r--r--   0        0        0     2287 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/periodiccontrol.py
--rw-r--r--   0        0        0     2208 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/sizecontrol.py
--rw-r--r--   0        0        0     4069 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/surfaceutilities.py
--rw-r--r--   0        0        0     4664 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/surfer.py
--rw-r--r--   0        0        0     2309 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/volumecontrol.py
--rw-r--r--   0        0        0     3064 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/volumesweeper.py
--rw-r--r--   0        0        0     7289 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/wrapper.py
--rw-r--r--   0        0        0     2115 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/wrappercontrol.py
--rw-r--r--   0        0        0     1269 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/examples/__init__.py
--rw-r--r--   0        0        0     4566 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/examples/download_utilities.py
--rw-r--r--   0        0        0    47227 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/examples/examples.py
--rw-r--r--   0        0        0     1514 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/examples/unit_test_examples.py
--rw-r--r--   0        0        0       59 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/graphics/__init__.py
--rw-r--r--   0        0        0    41774 2024-03-19 15:03:30.978976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/graphics/graphics.py
--rw-r--r--   0        0        0     2234 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/graphics/images/bin.png
--rw-r--r--   0        0        0     1708 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/graphics/images/invert_visibility.png
--rw-r--r--   0        0        0     2510 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/graphics/images/parts.png
--rw-r--r--   0        0        0     1297 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/graphics/images/selectioninfo.png
--rw-r--r--   0        0        0     2440 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/graphics/images/show_edges.png
--rw-r--r--   0        0        0      203 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/graphics/images/show_ruler.png
--rw-r--r--   0        0        0     1547 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/graphics/images/surface_body.png
--rw-r--r--   0        0        0     1612 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/graphics/trame_gui.py
--rw-r--r--   0        0        0     5692 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/internals/client.py
--rw-r--r--   0        0        0      626 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/internals/comm_manager.py
--rw-r--r--   0        0        0     1881 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/internals/communicator.py
--rw-r--r--   0        0        0     5045 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/internals/config.py
--rw-r--r--   0        0        0     3121 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/internals/defaults.py
--rw-r--r--   0        0        0    40389 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/internals/error_handling.py
--rw-r--r--   0        0        0     8935 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/internals/grpc_communicator.py
--rw-r--r--   0        0        0      951 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/internals/grpc_utils.py
--rw-r--r--   0        0        0     2319 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/internals/json_utils.py
--rw-r--r--   0        0        0     8307 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/internals/launcher.py
--rw-r--r--   0        0        0     2586 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/internals/logger.py
--rw-r--r--   0        0        0     3182 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/internals/prime_communicator.py
--rw-r--r--   0        0        0    12333 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/internals/utils.py
--rw-r--r--   0        0        0      143 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/lucid/__init__.py
--rw-r--r--   0        0        0    69861 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/lucid/mesh_util.py
--rw-r--r--   0        0        0     7532 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/lucid/scope.py
--rw-r--r--   0        0        0     1493 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/lucid/utils.py
--rw-r--r--   0        0        0     2346 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/params/primestructs.py
--rw-r--r--   0        0        0     4369 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/relaxed_json/__init__.py
--rw-r--r--   0        0        0    13490 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/relaxed_json/decoder.py
--rw-r--r--   0        0        0    13168 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/relaxed_json/encoder.py
--rw-r--r--   0        0        0     3024 2024-03-19 15:03:30.982976 ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/relaxed_json/scanner.py
--rw-r--r--   0        0        0     6089 1970-01-01 00:00:00.000000 ansys_meshing_prime-0.6.0.dev5/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-03-22 13:13:42.920885 ansys_meshing_prime-0.6.0.dev6/LICENSE
+-rw-r--r--   0        0        0     4090 2024-03-22 13:13:42.920885 ansys_meshing_prime-0.6.0.dev6/README.md
+-rw-r--r--   0        0        0     2408 2024-03-22 13:13:43.000886 ansys_meshing_prime-0.6.0.dev6/pyproject.toml
+-rw-r--r--   0        0        0     6218 2024-03-22 13:13:43.000886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/__init__.py
+-rw-r--r--   0        0        0      428 2024-03-22 13:13:43.000886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/_version.py
+-rw-r--r--   0        0        0     2654 2024-03-22 13:13:43.000886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/automesh.py
+-rw-r--r--   0        0        0    61369 2024-03-22 13:13:43.000886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/automeshstructs.py
+-rw-r--r--   0        0        0    11093 2024-03-22 13:13:43.000886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/autoquadmesher.py
+-rw-r--r--   0        0        0   165219 2024-03-22 13:13:43.000886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/autoquadmesherstructs.py
+-rw-r--r--   0        0        0     6123 2024-03-22 13:13:43.000886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/boundaryfittednurbs.py
+-rw-r--r--   0        0        0     3977 2024-03-22 13:13:43.000886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/collapsetool.py
+-rw-r--r--   0        0        0    14791 2024-03-22 13:13:43.000886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/collapsetoolstructs.py
+-rw-r--r--   0        0        0    28002 2024-03-22 13:13:43.000886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/commonstructs.py
+-rw-r--r--   0        0        0     3875 2024-03-22 13:13:43.000886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/commontypes.py
+-rw-r--r--   0        0        0    14928 2024-03-22 13:13:43.000886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/connect.py
+-rw-r--r--   0        0        0    95082 2024-03-22 13:13:43.000886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/connectstructs.py
+-rw-r--r--   0        0        0    12218 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/controldata.py
+-rw-r--r--   0        0        0    91621 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/controlstructs.py
+-rw-r--r--   0        0        0      714 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/coreobject.py
+-rw-r--r--   0        0        0     3433 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/deletetool.py
+-rw-r--r--   0        0        0    14080 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/deletetoolstructs.py
+-rw-r--r--   0        0        0     5585 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/featureextraction.py
+-rw-r--r--   0        0        0    35361 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/featureextractionstructs.py
+-rw-r--r--   0        0        0    31259 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/fileio.py
+-rw-r--r--   0        0        0   162937 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/fileiostructs.py
+-rw-r--r--   0        0        0    71909 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/igastructs.py
+-rw-r--r--   0        0        0     4136 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/materialpointmanager.py
+-rw-r--r--   0        0        0    16431 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/materialpointmanagerstructs.py
+-rw-r--r--   0        0        0     4866 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/meshinfo.py
+-rw-r--r--   0        0        0    60305 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/meshinfostructs.py
+-rw-r--r--   0        0        0    16840 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/model.py
+-rw-r--r--   0        0        0    27452 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/modelstructs.py
+-rw-r--r--   0        0        0     3803 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/morpher.py
+-rw-r--r--   0        0        0     7876 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/morpherbcsstructs.py
+-rw-r--r--   0        0        0    24470 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/morpherstructs.py
+-rw-r--r--   0        0        0     7869 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/multizonecontrol.py
+-rw-r--r--   0        0        0    59442 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/part.py
+-rw-r--r--   0        0        0   168878 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/partstructs.py
+-rw-r--r--   0        0        0     7671 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/periodiccontrol.py
+-rw-r--r--   0        0        0    13543 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/periodiccontrolstructs.py
+-rw-r--r--   0        0        0    33934 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/primeconfig.py
+-rw-r--r--   0        0        0     5733 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/prismcontrol.py
+-rw-r--r--   0        0        0    14608 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/prismcontrolstructs.py
+-rw-r--r--   0        0        0     2937 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/quadtospline.py
+-rw-r--r--   0        0        0     7253 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/scaffolder.py
+-rw-r--r--   0        0        0    38220 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/scaffolderstructs.py
+-rw-r--r--   0        0        0    18400 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/sizecontrol.py
+-rw-r--r--   0        0        0    53218 2024-03-22 13:13:43.004886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/sizecontrolstructs.py
+-rw-r--r--   0        0        0     2794 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/sizefield.py
+-rw-r--r--   0        0        0    19028 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/sizefieldstructs.py
+-rw-r--r--   0        0        0     4286 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/splittoolstructs.py
+-rw-r--r--   0        0        0    21687 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/surfacesearch.py
+-rw-r--r--   0        0        0   124157 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/surfacesearchstructs.py
+-rw-r--r--   0        0        0    25421 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/surfaceutilities.py
+-rw-r--r--   0        0        0   153390 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/surfaceutilitystructs.py
+-rw-r--r--   0        0        0     7198 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/surfer.py
+-rw-r--r--   0        0        0    45142 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/surferstructs.py
+-rw-r--r--   0        0        0     4454 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/thinvolumecontrol.py
+-rw-r--r--   0        0        0     7117 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/thinvolumecontrolstructs.py
+-rw-r--r--   0        0        0    10182 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/topodata.py
+-rw-r--r--   0        0        0     9409 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/topodatastructs.py
+-rw-r--r--   0        0        0     1761 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/toposearchstructs.py
+-rw-r--r--   0        0        0     2650 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/topoutilities.py
+-rw-r--r--   0        0        0    13257 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/topoutilitystructs.py
+-rw-r--r--   0        0        0     2966 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/transform.py
+-rw-r--r--   0        0        0     8817 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/transformstructs.py
+-rw-r--r--   0        0        0     5986 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/volumecontrol.py
+-rw-r--r--   0        0        0     6304 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/volumecontrolstructs.py
+-rw-r--r--   0        0        0     6962 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/volumemeshtool.py
+-rw-r--r--   0        0        0    29781 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/volumemeshtoolstructs.py
+-rw-r--r--   0        0        0     2763 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/volumesearch.py
+-rw-r--r--   0        0        0    25627 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/volumesearchstructs.py
+-rw-r--r--   0        0        0     4896 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/volumesweeper.py
+-rw-r--r--   0        0        0    25625 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/volumesweeperstructs.py
+-rw-r--r--   0        0        0     2927 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/vtcomposer.py
+-rw-r--r--   0        0        0     8476 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/vtcomposerstructs.py
+-rw-r--r--   0        0        0     7270 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/wrapper.py
+-rw-r--r--   0        0        0    10832 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/wrappercontrol.py
+-rw-r--r--   0        0        0    89981 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/wrapperstructs.py
+-rw-r--r--   0        0        0    15856 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/controldata.py
+-rw-r--r--   0        0        0   121829 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/dynaexportutils.py
+-rw-r--r--   0        0        0    20701 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/fileio.py
+-rw-r--r--   0        0        0   161431 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/mapdlcdbexportutils.py
+-rw-r--r--   0        0        0    11168 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/model.py
+-rw-r--r--   0        0        0      767 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/multizonecontrol.py
+-rw-r--r--   0        0        0     4181 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/part.py
+-rw-r--r--   0        0        0     2287 2024-03-22 13:13:43.008886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/periodiccontrol.py
+-rw-r--r--   0        0        0     2208 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/sizecontrol.py
+-rw-r--r--   0        0        0     4069 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/surfaceutilities.py
+-rw-r--r--   0        0        0     4664 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/surfer.py
+-rw-r--r--   0        0        0     2309 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/volumecontrol.py
+-rw-r--r--   0        0        0     3064 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/volumesweeper.py
+-rw-r--r--   0        0        0     7289 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/wrapper.py
+-rw-r--r--   0        0        0     2115 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/wrappercontrol.py
+-rw-r--r--   0        0        0     1269 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/examples/__init__.py
+-rw-r--r--   0        0        0     4566 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/examples/download_utilities.py
+-rw-r--r--   0        0        0    47227 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/examples/examples.py
+-rw-r--r--   0        0        0     1514 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/examples/unit_test_examples.py
+-rw-r--r--   0        0        0       59 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/graphics/__init__.py
+-rw-r--r--   0        0        0    41774 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/graphics/graphics.py
+-rw-r--r--   0        0        0     2234 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/graphics/images/bin.png
+-rw-r--r--   0        0        0     1708 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/graphics/images/invert_visibility.png
+-rw-r--r--   0        0        0     2510 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/graphics/images/parts.png
+-rw-r--r--   0        0        0     1297 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/graphics/images/selectioninfo.png
+-rw-r--r--   0        0        0     2440 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/graphics/images/show_edges.png
+-rw-r--r--   0        0        0      203 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/graphics/images/show_ruler.png
+-rw-r--r--   0        0        0     1547 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/graphics/images/surface_body.png
+-rw-r--r--   0        0        0     1612 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/graphics/trame_gui.py
+-rw-r--r--   0        0        0     5692 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/internals/client.py
+-rw-r--r--   0        0        0      626 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/internals/comm_manager.py
+-rw-r--r--   0        0        0     1881 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/internals/communicator.py
+-rw-r--r--   0        0        0     5045 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/internals/config.py
+-rw-r--r--   0        0        0     3121 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/internals/defaults.py
+-rw-r--r--   0        0        0    40389 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/internals/error_handling.py
+-rw-r--r--   0        0        0     8935 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/internals/grpc_communicator.py
+-rw-r--r--   0        0        0      951 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/internals/grpc_utils.py
+-rw-r--r--   0        0        0     2319 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/internals/json_utils.py
+-rw-r--r--   0        0        0     8307 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/internals/launcher.py
+-rw-r--r--   0        0        0     2586 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/internals/logger.py
+-rw-r--r--   0        0        0     3182 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/internals/prime_communicator.py
+-rw-r--r--   0        0        0    12339 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/internals/utils.py
+-rw-r--r--   0        0        0      143 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/lucid/__init__.py
+-rw-r--r--   0        0        0    70047 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/lucid/mesh_util.py
+-rw-r--r--   0        0        0     7532 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/lucid/scope.py
+-rw-r--r--   0        0        0     1493 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/lucid/utils.py
+-rw-r--r--   0        0        0     2346 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/params/primestructs.py
+-rw-r--r--   0        0        0     4369 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/relaxed_json/__init__.py
+-rw-r--r--   0        0        0    13490 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/relaxed_json/decoder.py
+-rw-r--r--   0        0        0    13168 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/relaxed_json/encoder.py
+-rw-r--r--   0        0        0     3024 2024-03-22 13:13:43.012886 ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/relaxed_json/scanner.py
+-rw-r--r--   0        0        0     6089 1970-01-01 00:00:00.000000 ansys_meshing_prime-0.6.0.dev6/PKG-INFO
```

### Comparing `ansys_meshing_prime-0.6.0.dev5/LICENSE` & `ansys_meshing_prime-0.6.0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/README.md` & `ansys_meshing_prime-0.6.0.dev6/README.md`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/pyproject.toml` & `ansys_meshing_prime-0.6.0.dev6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "ansys-meshing-prime"
-version = "0.6.0.dev5"
+version = "0.6.0.dev6"
 description = "PyPrimeMesh is a Python client to Ansys Prime Server, which delivers core Ansys meshing technology."
 readme = "README.md"
 requires-python = ">=3.8,<4"
 license = {file = "LICENSE"}
 authors = [{name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"}]
 maintainers =  [{name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"}]
 classifiers = [
```

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/__init__.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/automesh.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/automesh.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/automeshstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/automeshstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/autoquadmesher.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/autoquadmesher.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/autoquadmesherstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/autoquadmesherstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/boundaryfittednurbs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/boundaryfittednurbs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/collapsetool.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/collapsetool.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/collapsetoolstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/collapsetoolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/commonstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/commonstructs.py`

 * *Files 9% similar despite different names*

```diff
@@ -383,68 +383,80 @@
 class CopyZoneletsParams(CoreObject):
     """Parameters to copy zonelets.
     """
     _default_params = {}
 
     def __initialize(
             self,
+            copy_labels: bool,
             copy_zones: bool):
+        self._copy_labels = copy_labels
         self._copy_zones = copy_zones
 
     def __init__(
             self,
             model: CommunicationManager=None,
+            copy_labels: bool = None,
             copy_zones: bool = None,
             json_data : dict = None,
              **kwargs):
         """Initialize a ``CopyZoneletsParams`` object.
 
         Parameters
         ----------
         model: Model
             Model to create a ``CopyZoneletsParams`` object with default parameters.
+        copy_labels: bool, optional
+            Option to copy labels of input zonelets to the corresponding copied zonelets.
+            This is a beta parameter. The behavior and name may change in the future.
         copy_zones: bool, optional
             Option to copy zones of input zonelets to corresponding copied zonelets.
         json_data: dict, optional
             JSON dictionary to create a ``CopyZoneletsParams`` object with provided parameters.
 
         Examples
         --------
         >>> copy_zonelets_params = prime.CopyZoneletsParams(model = model)
         """
         if json_data:
             self.__initialize(
+                json_data["copyLabels"] if "copyLabels" in json_data else None,
                 json_data["copyZones"] if "copyZones" in json_data else None)
         else:
-            all_field_specified = all(arg is not None for arg in [copy_zones])
+            all_field_specified = all(arg is not None for arg in [copy_labels, copy_zones])
             if all_field_specified:
                 self.__initialize(
+                    copy_labels,
                     copy_zones)
             else:
                 if model is None:
                     raise ValueError("Invalid assignment. Either pass a model or specify all properties.")
                 else:
                     param_json = model._communicator.initialize_params(model, "CopyZoneletsParams")
                     json_data = param_json["CopyZoneletsParams"] if "CopyZoneletsParams" in param_json else {}
                     self.__initialize(
+                        copy_labels if copy_labels is not None else ( CopyZoneletsParams._default_params["copy_labels"] if "copy_labels" in CopyZoneletsParams._default_params else (json_data["copyLabels"] if "copyLabels" in json_data else None)),
                         copy_zones if copy_zones is not None else ( CopyZoneletsParams._default_params["copy_zones"] if "copy_zones" in CopyZoneletsParams._default_params else (json_data["copyZones"] if "copyZones" in json_data else None)))
         self._custom_params = kwargs
         if model is not None:
             [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
         [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
         lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
         self._freeze()
 
     @staticmethod
     def set_default(
+            copy_labels: bool = None,
             copy_zones: bool = None):
         """Set the default values of the ``CopyZoneletsParams`` object.
 
         Parameters
         ----------
+        copy_labels: bool, optional
+            Option to copy labels of input zonelets to the corresponding copied zonelets.
         copy_zones: bool, optional
             Option to copy zones of input zonelets to corresponding copied zonelets.
         """
         args = locals()
         [CopyZoneletsParams._default_params.update({ key: value }) for key, value in args.items() if value is not None]
 
     @staticmethod
@@ -457,25 +469,38 @@
         """
         message = ""
         message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in CopyZoneletsParams._default_params.items())
         print(message)
 
     def _jsonify(self) -> Dict[str, Any]:
         json_data = {}
+        if self._copy_labels is not None:
+            json_data["copyLabels"] = self._copy_labels
         if self._copy_zones is not None:
             json_data["copyZones"] = self._copy_zones
         [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
         return json_data
 
     def __str__(self) -> str:
-        message = "copy_zones :  %s" % (self._copy_zones)
+        message = "copy_labels :  %s\ncopy_zones :  %s" % (self._copy_labels, self._copy_zones)
         message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
         return message
 
     @property
+    def copy_labels(self) -> bool:
+        """Option to copy labels of input zonelets to the corresponding copied zonelets.
+        This is a beta parameter. The behavior and name may change in the future.
+        """
+        return self._copy_labels
+
+    @copy_labels.setter
+    def copy_labels(self, value: bool):
+        self._copy_labels = value
+
+    @property
     def copy_zones(self) -> bool:
         """Option to copy zones of input zonelets to corresponding copied zonelets.
         """
         return self._copy_zones
 
     @copy_zones.setter
     def copy_zones(self, value: bool):
```

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/commontypes.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/commontypes.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/connect.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/connect.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/connectstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/connectstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/controldata.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/controldata.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/controlstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/controlstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/coreobject.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/coreobject.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/deletetool.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/deletetool.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/deletetoolstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/deletetoolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/featureextraction.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/featureextraction.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/featureextractionstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/featureextractionstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/fileio.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/fileio.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/fileiostructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/fileiostructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/igastructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/igastructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/materialpointmanager.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/materialpointmanager.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/materialpointmanagerstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/materialpointmanagerstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/meshinfo.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/meshinfo.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/meshinfostructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/meshinfostructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/model.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/model.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/modelstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/modelstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/morpher.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/morpher.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/morpherbcsstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/morpherbcsstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/morpherstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/morpherstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/multizonecontrol.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/multizonecontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/part.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/part.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/partstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/partstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/periodiccontrol.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/periodiccontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/periodiccontrolstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/periodiccontrolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/primeconfig.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/primeconfig.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/prismcontrol.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/prismcontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/prismcontrolstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/prismcontrolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/quadtospline.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/quadtospline.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/scaffolder.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/scaffolder.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/scaffolderstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/scaffolderstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/sizecontrol.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/sizecontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/sizecontrolstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/sizecontrolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/sizefield.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/sizefield.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/sizefieldstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/sizefieldstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/splittoolstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/splittoolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/surfacesearch.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/surfacesearch.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/surfacesearchstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/surfacesearchstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/surfaceutilities.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/surfaceutilities.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/surfaceutilitystructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/surfaceutilitystructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/surfer.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/surfer.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/surferstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/surferstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/thinvolumecontrol.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/thinvolumecontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/thinvolumecontrolstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/thinvolumecontrolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/topodata.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/topodata.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/topodatastructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/topodatastructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/toposearchstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/toposearchstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/topoutilities.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/topoutilities.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/topoutilitystructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/topoutilitystructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/transform.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/transform.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/transformstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/transformstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/volumecontrol.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/volumecontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/volumecontrolstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/volumecontrolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/volumemeshtool.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/volumemeshtool.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/volumemeshtoolstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/volumemeshtoolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/volumesearch.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/volumesearch.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/volumesearchstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/volumesearchstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/volumesweeper.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/volumesweeper.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/volumesweeperstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/volumesweeperstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/vtcomposer.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/vtcomposer.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/vtcomposerstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/vtcomposerstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/wrapper.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/wrapper.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/wrappercontrol.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/wrappercontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/autogen/wrapperstructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/autogen/wrapperstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/controldata.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/controldata.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/dynaexportutils.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/dynaexportutils.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/fileio.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/fileio.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/mapdlcdbexportutils.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/mapdlcdbexportutils.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/model.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/model.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/multizonecontrol.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/multizonecontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/part.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/part.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/periodiccontrol.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/periodiccontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/sizecontrol.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/sizecontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/surfaceutilities.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/surfaceutilities.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/surfer.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/surfer.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/volumecontrol.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/volumecontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/volumesweeper.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/volumesweeper.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/wrapper.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/core/wrappercontrol.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/core/wrappercontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/examples/__init__.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/examples/download_utilities.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/examples/download_utilities.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/examples/examples.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/examples/examples.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/examples/unit_test_examples.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/examples/unit_test_examples.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/graphics/graphics.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/graphics/graphics.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/graphics/images/bin.png` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/graphics/images/bin.png`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/graphics/images/invert_visibility.png` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/graphics/images/invert_visibility.png`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/graphics/images/parts.png` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/graphics/images/parts.png`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/graphics/images/selectioninfo.png` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/graphics/images/selectioninfo.png`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/graphics/images/show_edges.png` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/graphics/images/show_edges.png`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/graphics/images/surface_body.png` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/graphics/images/surface_body.png`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/graphics/trame_gui.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/graphics/trame_gui.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/internals/client.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/internals/client.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/internals/comm_manager.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/internals/comm_manager.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/internals/communicator.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/internals/communicator.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/internals/config.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/internals/config.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/internals/defaults.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/internals/defaults.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/internals/error_handling.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/internals/error_handling.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/internals/grpc_communicator.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/internals/grpc_communicator.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/internals/grpc_utils.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/internals/grpc_utils.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/internals/json_utils.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/internals/json_utils.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/internals/launcher.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/internals/launcher.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/internals/logger.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/internals/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/internals/prime_communicator.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/internals/prime_communicator.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/internals/utils.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/internals/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -333,17 +333,20 @@
 
     Returns
     -------
     int
         First available port.
     """
     port = init_port
-    while port_in_use(port) or port in _LOCAL_PORTS:
-        port += 1
-    _LOCAL_PORTS.append(port)
+    import socket
+
+    s = socket.socket()
+    s.bind(("", 0))
+    port = s.getsockname()[1]
+    s.close()
     return port
 
 
 @contextmanager
 def file_read_context_list(model, file_names: List[str]):
     """Upload context.
```

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/lucid/mesh_util.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/lucid/mesh_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,14 +114,18 @@
 
         """
         filename, fileext = os.path.splitext(file_name)
         if fileext == ".cdb":
             prime.FileIO(self._model).export_mapdl_cdb(
                 file_name, prime.ExportMapdlCdbParams(self._model)
             )
+        elif fileext == ".k":
+            prime.FileIO(self._model).export_lsdyna_keyword_file(
+                file_name, prime.ExportLSDynaKeywordFileParams(self._model)
+            )
         elif fileext == ".cas" or file_name[-7:] == ".cas.gz":
             prime.FileIO(self._model).export_fluent_case(
                 file_name, prime.ExportFluentCaseParams(self._model, cff_format=False)
             )
         elif file_name[-7:] == ".cas.h5":
             prime.FileIO(self._model).export_fluent_case(
                 file_name, prime.ExportFluentCaseParams(self._model, cff_format=True)
```

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/lucid/scope.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/lucid/scope.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/lucid/utils.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/lucid/utils.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/params/primestructs.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/params/primestructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/relaxed_json/__init__.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/relaxed_json/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/relaxed_json/decoder.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/relaxed_json/decoder.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/relaxed_json/encoder.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/relaxed_json/encoder.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/src/ansys/meshing/prime/relaxed_json/scanner.py` & `ansys_meshing_prime-0.6.0.dev6/src/ansys/meshing/prime/relaxed_json/scanner.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev5/PKG-INFO` & `ansys_meshing_prime-0.6.0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-meshing-prime
-Version: 0.6.0.dev5
+Version: 0.6.0.dev6
 Summary: PyPrimeMesh is a Python client to Ansys Prime Server, which delivers core Ansys meshing technology.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

