# Comparing `tmp/FlowKit-1.0.1.tar.gz` & `tmp/FlowKit-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlowKit-1.0.1.tar", last modified: Mon May  8 23:00:34 2023, max compression
+gzip compressed data, was "FlowKit-1.1.0.tar", last modified: Fri Apr  5 04:46:34 2024, max compression
```

## Comparing `FlowKit-1.0.1.tar` & `FlowKit-1.1.0.tar`

### file list

```diff
@@ -1,52 +1,55 @@
-drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-05-08 23:00:34.459097 FlowKit-1.0.1/
-drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-05-08 23:00:34.451097 FlowKit-1.0.1/FlowKit.egg-info/
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     9746 2023-05-08 23:00:34.000000 FlowKit-1.0.1/FlowKit.egg-info/PKG-INFO
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     1264 2023-05-08 23:00:34.000000 FlowKit-1.0.1/FlowKit.egg-info/SOURCES.txt
--rw-rw-r--   0 swhite    (1000) swhite    (1000)        1 2023-05-08 23:00:34.000000 FlowKit-1.0.1/FlowKit.egg-info/dependency_links.txt
--rw-rw-r--   0 swhite    (1000) swhite    (1000)      169 2023-05-08 23:00:34.000000 FlowKit-1.0.1/FlowKit.egg-info/requires.txt
--rw-rw-r--   0 swhite    (1000) swhite    (1000)        8 2023-05-08 23:00:34.000000 FlowKit-1.0.1/FlowKit.egg-info/top_level.txt
--rw-r--r--   0 swhite    (1000) swhite    (1000)     1511 2019-08-08 15:30:26.000000 FlowKit-1.0.1/LICENSE
--rw-rw-r--   0 swhite    (1000) swhite    (1000)       69 2022-07-18 16:34:26.000000 FlowKit-1.0.1/MANIFEST.in
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     9746 2023-05-08 23:00:34.459097 FlowKit-1.0.1/PKG-INFO
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     9320 2023-05-08 14:38:48.000000 FlowKit-1.0.1/README.md
-drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-05-08 23:00:34.451097 FlowKit-1.0.1/flowkit/
--rw-rw-r--   0 swhite    (1000) swhite    (1000)      978 2023-01-24 14:08:16.000000 FlowKit-1.0.1/flowkit/__init__.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)      769 2022-07-18 16:34:27.000000 FlowKit-1.0.1/flowkit/_conf.py
-drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-05-08 23:00:34.455097 FlowKit-1.0.1/flowkit/_models/
--rw-rw-r--   0 swhite    (1000) swhite    (1000)       36 2022-07-18 16:34:27.000000 FlowKit-1.0.1/flowkit/_models/__init__.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     5252 2022-10-12 15:57:40.000000 FlowKit-1.0.1/flowkit/_models/dimension.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     3274 2023-01-24 14:08:16.000000 FlowKit-1.0.1/flowkit/_models/gate_node.py
-drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-05-08 23:00:34.455097 FlowKit-1.0.1/flowkit/_models/gates/
--rw-rw-r--   0 swhite    (1000) swhite    (1000)      251 2022-07-18 16:34:27.000000 FlowKit-1.0.1/flowkit/_models/gates/__init__.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     1174 2023-01-24 14:08:16.000000 FlowKit-1.0.1/flowkit/_models/gates/_base_gate.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)    15888 2023-01-24 14:08:16.000000 FlowKit-1.0.1/flowkit/_models/gates/_gates.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)    13786 2023-01-24 14:08:16.000000 FlowKit-1.0.1/flowkit/_models/gates/_gml_gates.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     9766 2023-01-24 14:08:16.000000 FlowKit-1.0.1/flowkit/_models/gates/_wsp_gates.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     6399 2022-07-18 16:34:27.000000 FlowKit-1.0.1/flowkit/_models/gating_results.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)    37951 2023-05-08 22:51:18.000000 FlowKit-1.0.1/flowkit/_models/gating_strategy.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)    51529 2023-02-22 22:15:26.000000 FlowKit-1.0.1/flowkit/_models/sample.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)    32867 2023-02-22 22:15:26.000000 FlowKit-1.0.1/flowkit/_models/session.py
-drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-05-08 23:00:34.455097 FlowKit-1.0.1/flowkit/_models/transforms/
--rw-rw-r--   0 swhite    (1000) swhite    (1000)      446 2022-07-18 16:34:27.000000 FlowKit-1.0.1/flowkit/_models/transforms/__init__.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     1515 2023-01-24 14:08:16.000000 FlowKit-1.0.1/flowkit/_models/transforms/_base_transform.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)    10923 2023-02-22 22:15:26.000000 FlowKit-1.0.1/flowkit/_models/transforms/_gml_transforms.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     4292 2023-05-08 22:51:18.000000 FlowKit-1.0.1/flowkit/_models/transforms/_matrix.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)    11735 2022-07-18 16:34:27.000000 FlowKit-1.0.1/flowkit/_models/transforms/_transforms.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     8240 2022-10-11 20:08:25.000000 FlowKit-1.0.1/flowkit/_models/transforms/_wsp_transforms.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)    37605 2023-02-22 22:15:26.000000 FlowKit-1.0.1/flowkit/_models/workspace.py
-drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-05-08 23:00:34.455097 FlowKit-1.0.1/flowkit/_resources/
--rw-r--r--   0 swhite    (1000) swhite    (1000)     4954 2019-08-08 15:31:13.000000 FlowKit-1.0.1/flowkit/_resources/DataTypes.v2.0.xsd
--rw-r--r--   0 swhite    (1000) swhite    (1000)    11745 2019-08-08 15:31:13.000000 FlowKit-1.0.1/flowkit/_resources/Gating-ML.v2.0.xsd
--rw-r--r--   0 swhite    (1000) swhite    (1000)     9405 2019-08-08 15:31:13.000000 FlowKit-1.0.1/flowkit/_resources/Transformations.v2.0.xsd
--rw-rw-r--   0 swhite    (1000) swhite    (1000)      814 2022-09-01 17:34:53.000000 FlowKit-1.0.1/flowkit/_resources/__init__.py
-drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-05-08 23:00:34.459097 FlowKit-1.0.1/flowkit/_utils/
--rw-rw-r--   0 swhite    (1000) swhite    (1000)       21 2022-07-18 16:34:27.000000 FlowKit-1.0.1/flowkit/_utils/__init__.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     4790 2023-01-24 14:08:16.000000 FlowKit-1.0.1/flowkit/_utils/gating_utils.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)    14764 2023-02-22 22:15:26.000000 FlowKit-1.0.1/flowkit/_utils/plot_utils.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     2337 2023-02-22 22:15:26.000000 FlowKit-1.0.1/flowkit/_utils/sample_utils.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)    45011 2023-02-22 22:15:26.000000 FlowKit-1.0.1/flowkit/_utils/wsp_utils.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)    30404 2023-02-22 22:15:26.000000 FlowKit-1.0.1/flowkit/_utils/xml_utils.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)       46 2023-05-08 22:52:05.000000 FlowKit-1.0.1/flowkit/_version.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)      946 2023-02-22 22:15:26.000000 FlowKit-1.0.1/flowkit/exceptions.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)       38 2023-05-08 23:00:34.459097 FlowKit-1.0.1/setup.cfg
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     1404 2023-02-22 22:15:26.000000 FlowKit-1.0.1/setup.py
+drwxr-xr-x   0 swhite   (957844952) domain users (957800513)        0 2024-04-05 04:46:34.151234 FlowKit-1.1.0/
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     1511 2019-08-08 15:30:26.000000 FlowKit-1.1.0/LICENSE
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)       48 2024-04-02 17:50:51.000000 FlowKit-1.1.0/MANIFEST.in
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    10601 2024-04-05 04:46:34.151234 FlowKit-1.1.0/PKG-INFO
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     9802 2024-04-02 17:50:51.000000 FlowKit-1.1.0/README.md
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)       88 2024-04-02 17:50:52.000000 FlowKit-1.1.0/pyproject.toml
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)       38 2024-04-05 04:46:34.151234 FlowKit-1.1.0/setup.cfg
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     1475 2024-04-04 16:10:48.000000 FlowKit-1.1.0/setup.py
+drwxr-xr-x   0 swhite   (957844952) domain users (957800513)        0 2024-04-05 04:46:34.151234 FlowKit-1.1.0/src/
+drwxr-xr-x   0 swhite   (957844952) domain users (957800513)        0 2024-04-05 04:46:34.151234 FlowKit-1.1.0/src/FlowKit.egg-info/
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    10601 2024-04-05 04:46:34.000000 FlowKit-1.1.0/src/FlowKit.egg-info/PKG-INFO
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     1446 2024-04-05 04:46:34.000000 FlowKit-1.1.0/src/FlowKit.egg-info/SOURCES.txt
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)        1 2024-04-05 04:46:34.000000 FlowKit-1.1.0/src/FlowKit.egg-info/dependency_links.txt
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)      156 2024-04-05 04:46:34.000000 FlowKit-1.1.0/src/FlowKit.egg-info/requires.txt
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)        8 2024-04-05 04:46:34.000000 FlowKit-1.1.0/src/FlowKit.egg-info/top_level.txt
+drwxr-xr-x   0 swhite   (957844952) domain users (957800513)        0 2024-04-05 04:46:34.151234 FlowKit-1.1.0/src/flowkit/
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     1061 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/__init__.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)      769 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_conf.py
+drwxr-xr-x   0 swhite   (957844952) domain users (957800513)        0 2024-04-05 04:46:34.151234 FlowKit-1.1.0/src/flowkit/_models/
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)       36 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/__init__.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     5252 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/dimension.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     3274 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/gate_node.py
+drwxr-xr-x   0 swhite   (957844952) domain users (957800513)        0 2024-04-05 04:46:34.151234 FlowKit-1.1.0/src/flowkit/_models/gates/
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)      251 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/gates/__init__.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     1174 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/gates/_base_gate.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    15888 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/gates/_gates.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    13806 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/gates/_gml_gates.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     9766 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/gates/_wsp_gates.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     6399 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/gating_results.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    37938 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/gating_strategy.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    54529 2024-04-04 21:42:11.000000 FlowKit-1.1.0/src/flowkit/_models/sample.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    26532 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/session.py
+drwxr-xr-x   0 swhite   (957844952) domain users (957800513)        0 2024-04-05 04:46:34.151234 FlowKit-1.1.0/src/flowkit/_models/transforms/
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)      446 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/transforms/__init__.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     1515 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/transforms/_base_transform.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     5307 2024-04-04 21:42:11.000000 FlowKit-1.1.0/src/flowkit/_models/transforms/_matrix.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    11735 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/transforms/_transforms.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     8353 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/transforms/_wsp_transforms.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    32166 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/workspace.py
+drwxr-xr-x   0 swhite   (957844952) domain users (957800513)        0 2024-04-05 04:46:34.151234 FlowKit-1.1.0/src/flowkit/_resources/
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     4837 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_resources/DataTypes.v2.0.xsd
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    11485 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_resources/Gating-ML.v2.0.xsd
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     9210 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_resources/Transformations.v2.0.xsd
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)      814 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_resources/__init__.py
+drwxr-xr-x   0 swhite   (957844952) domain users (957800513)        0 2024-04-05 04:46:34.151234 FlowKit-1.1.0/src/flowkit/_utils/
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)       21 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_utils/__init__.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     4790 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_utils/gating_utils.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    12097 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_utils/gml_write.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    31092 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_utils/plot_utils.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     4693 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_utils/sample_utils.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    46376 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_utils/wsp_utils.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     2303 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_utils/xml_common.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    21437 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_utils/xml_utils.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)       46 2024-04-04 23:47:31.000000 FlowKit-1.1.0/src/flowkit/_version.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)      954 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/exceptions.py
```

### Comparing `FlowKit-1.0.1/FlowKit.egg-info/PKG-INFO` & `FlowKit-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,23 @@
-Metadata-Version: 2.1
-Name: FlowKit
-Version: 1.0.1
-Summary: Flow Cytometry Toolkit
-Home-page: https://github.com/whitews/flowkit
-Author: Scott White
-License: BSD
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # FlowKit
 
 [!["FlowKit"](https://raw.githubusercontent.com/whitews/FlowKit/master/docs/_static/flowkit.png)](https://github.com/whitews/flowkit)
 
 [![PyPI license](https://img.shields.io/pypi/l/flowkit.svg?colorB=dodgerblue)](https://pypi.python.org/pypi/flowkit/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/flowkit.svg)](https://pypi.python.org/pypi/flowkit/)
 [![PyPI version](https://img.shields.io/pypi/v/flowkit.svg?colorB=blue)](https://pypi.python.org/pypi/flowkit/)
 [![DOI](https://zenodo.org/badge/138655889.svg)](https://zenodo.org/badge/latestdoi/138655889)
 
 
-[![Build & test (master)](https://github.com/whitews/FlowKit/actions/workflows/tests_master.yml/badge.svg)](https://github.com/whitews/FlowKit/actions/workflows/tests_master.yml)
-[![Build & test (develop)](https://github.com/whitews/FlowKit/actions/workflows/tests_develop.yml/badge.svg)](https://github.com/whitews/FlowKit/actions/workflows/tests_develop.yml)
+[![Test (master)](https://github.com/whitews/FlowKit/actions/workflows/tests_master.yml/badge.svg)](https://github.com/whitews/FlowKit/actions/workflows/tests_master.yml)
+[![Test (develop)](https://github.com/whitews/FlowKit/actions/workflows/tests_develop.yml/badge.svg)](https://github.com/whitews/FlowKit/actions/workflows/tests_develop.yml)
 [![codecov](https://codecov.io/gh/whitews/flowkit/branch/master/graph/badge.svg?token=joeOIVWmHi)](https://codecov.io/gh/whitews/flowkit)
 [![Documentation Status](https://readthedocs.org/projects/flowkit/badge/?version=latest)](https://flowkit.readthedocs.io/en/latest/?badge=latest)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/flowkit)
+
 
 * [Overview](#overview)
 * [Features](#features)
 * [Requirements](#requirements)
 * [Installation](#installation)
 * [Documentation](#documentation)
   * [Tutorials](#tutorials)
@@ -81,35 +69,36 @@
   * Contour density plot of two channels
   * Interactive scatter plot of two channels
   * Interactive scatter plot matrix of any combination of channels
   * Interactive scatter plots of gates with sample events
 
 ## Requirements
 
-FlowKit supports Python version 3.7 - 3.10. All dependencies are installable 
+FlowKit supports Python version 3.8 - 3.12. All dependencies are installable 
 via pip, and are listed below.
 
-> **NOTE**: FlowUtils uses C extensions for significant performance improvements. For most platforms and Python versions, pre-built binaries are available in PyPI (i.e. installable via `pip`). 
->
-> If a pre-built binary of FlowUtils is not available for your environment, the C extensions must be compiled using the source package. NumPy >=1.19 must be installed prior to compiling FlowUtils. If compiling using `gcc`, version 5 or later is required.
+> **NOTE**: FlowUtils uses C extensions for significant performance 
+> improvements. For most platforms and Python versions, pre-built 
+> binaries of FlowUtils are available in PyPI (i.e. installable via 
+> `pip`). If a pre-built binary is not available for your environment, 
+> the C extensions must be compiled using the source package.
 
 Required Python dependencies:
 
-* [flowio](https://github.com/whitews/flowio) == 1.1.1
-* [flowutils](https://github.com/whitews/flowutils) == 1.0.0
-* anytree >= 2.6
-* bokeh >= 2.4, <3.0
-* lxml >= 4.7
-* matplotlib >= 3.5
-* networkx >= 2.3
-* numpy >= 1.20
-* pandas >= 1.2
+* [flowio](https://github.com/whitews/flowio) >= 1.3.0
+* [flowutils](https://github.com/whitews/flowutils) >= 1.1.0
+* anytree >= 2.9
+* bokeh >= 3.1
+* contourpy >= 1.1.0
+* lxml >= 4.9
+* networkx >= 3.1
+* numpy >= 1.22, <2
+* pandas >= 2.0
 * psutils >= 5.8
-* scipy >= 1.6
-* seaborn >= 0.11, <0.12
+* scipy >= 1.8
 
 ## Installation
 
 > **NOTE**: For macOS users running on Apple Silicon, the version of `pip` may need to be upgraded prior to installing FlowKit in order to install the required dependencies.
 
 ### From PyPI
 
@@ -149,16 +138,16 @@
 * [Part 5 - Session Class](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/flowkit-tutorial-part05-session-class.ipynb)
 * [Part 6 - Workspace Class](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/flowkit-tutorial-part06-workspace-class.ipynb)
 
 ### Advanced Examples
 
 Below are more advanced and practical examples for using FlowKit. If you have an example you would like to submit for consideration in this list (preferably with data), please [submit an issue](https://github.com/whitews/FlowKit/issues/new/).
 
-* [Compare mean fluorescence intensity (MFI) in gated populations](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/flowkit-session-compare-mfi-of-gated-events.ipynb)
-* [Importing a FlowJo 10 WSP file & replicating analysis in FlowKit](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/flowkit-session-replicate-flowjo-wsp.ipynb)
+* [Compare mean fluorescence intensity (MFI) in gated populations](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/compare-mfi-of-gated-events.ipynb)
+* [Importing a FlowJo 10 WSP file & replicating analysis in FlowKit](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/replicate-flowjo-wsp.ipynb)
 * [Dimension reduction on gated populations](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/dimension_reduction_on_gated_populations.ipynb)
 * [Comparison between Leiden & Louvain clustering](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/clustering_comparison_leiden_vs_louvain.ipynb)
 * [Saving Flow Analysis Data as AnnData objects for ScanPy](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/scanpy_creating_and_using_AnnData_objects.ipynb)
 
 ## Contributing
 
 Want to get involved in the development of FlowKit? 
@@ -169,9 +158,11 @@
 
 [White, S., Quinn, J., Enzor, J., Staats, J., Mosier, S. M., Almarode, J., Denny, T. N., Weinhold, K. J., Ferrari, G., & Chan, C. (2021). FlowKit: A Python toolkit for integrated manual and automated cytometry analysis workflows. Frontiers in Immunology, 12. https://doi.org/10.3389/fimmu.2021.768541](https://www.frontiersin.org/articles/10.3389/fimmu.2021.768541/full)
 
 ## Projects & Research Using FlowKit 
 
 The following projects and publications have utilized FlowKit. If you have a package or publication where FlowKit was used, and you want it listed here, feel free to [submit an issue](https://github.com/whitews/FlowKit/issues/new/) letting me know.
 
+* Mortelecque, Justine et al. "A selection and optimization strategy for single-domain antibodies targeting the PHF6 linear peptide within the Tau intrinsically disordered protein." Journal of Biological Chemistry (2024), [doi:10.1016/j.jbc.2024.107163](https://www.jbc.org/article/S0021-9258(24)01658-2/fulltext)
+* Schmidt, Florian et al. "In-depth analysis of human virus-specific CD8+ T cells delineates unique phenotypic signatures for T cell specificity prediction." Cell Reports vol. 42,10 (2023), [doi:10.1016/j.celrep.2023.113250](https://www.cell.com/cell-reports/fulltext/S2211-1247(23)01262-7)
 * Schuster, Jonas et al. “Combining real-time fluorescence spectroscopy and flow cytometry to reveal new insights in DOC and cell characterization of drinking water.” Frontiers in Environmental Chemistry (2022), [doi:10.3389/fenvc.2022.931067](https://www.frontiersin.org/articles/10.3389/fenvc.2022.931067/full)
 * Rendeiro, André F et al. "Profiling of immune dysfunction in COVID-19 patients allows early prediction of disease progression." Life science alliance vol. 4,2 e202000955. 24 Dec. 2020, [doi:10.26508/lsa.202000955](https://www.life-science-alliance.org/content/4/2/e202000955.full)
```

### Comparing `FlowKit-1.0.1/FlowKit.egg-info/SOURCES.txt` & `FlowKit-1.1.0/src/FlowKit.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
-FlowKit.egg-info/PKG-INFO
-FlowKit.egg-info/SOURCES.txt
-FlowKit.egg-info/dependency_links.txt
-FlowKit.egg-info/requires.txt
-FlowKit.egg-info/top_level.txt
-flowkit/__init__.py
-flowkit/_conf.py
-flowkit/_version.py
-flowkit/exceptions.py
-flowkit/_models/__init__.py
-flowkit/_models/dimension.py
-flowkit/_models/gate_node.py
-flowkit/_models/gating_results.py
-flowkit/_models/gating_strategy.py
-flowkit/_models/sample.py
-flowkit/_models/session.py
-flowkit/_models/workspace.py
-flowkit/_models/gates/__init__.py
-flowkit/_models/gates/_base_gate.py
-flowkit/_models/gates/_gates.py
-flowkit/_models/gates/_gml_gates.py
-flowkit/_models/gates/_wsp_gates.py
-flowkit/_models/transforms/__init__.py
-flowkit/_models/transforms/_base_transform.py
-flowkit/_models/transforms/_gml_transforms.py
-flowkit/_models/transforms/_matrix.py
-flowkit/_models/transforms/_transforms.py
-flowkit/_models/transforms/_wsp_transforms.py
-flowkit/_resources/DataTypes.v2.0.xsd
-flowkit/_resources/Gating-ML.v2.0.xsd
-flowkit/_resources/Transformations.v2.0.xsd
-flowkit/_resources/__init__.py
-flowkit/_utils/__init__.py
-flowkit/_utils/gating_utils.py
-flowkit/_utils/plot_utils.py
-flowkit/_utils/sample_utils.py
-flowkit/_utils/wsp_utils.py
-flowkit/_utils/xml_utils.py
+src/FlowKit.egg-info/PKG-INFO
+src/FlowKit.egg-info/SOURCES.txt
+src/FlowKit.egg-info/dependency_links.txt
+src/FlowKit.egg-info/requires.txt
+src/FlowKit.egg-info/top_level.txt
+src/flowkit/__init__.py
+src/flowkit/_conf.py
+src/flowkit/_version.py
+src/flowkit/exceptions.py
+src/flowkit/_models/__init__.py
+src/flowkit/_models/dimension.py
+src/flowkit/_models/gate_node.py
+src/flowkit/_models/gating_results.py
+src/flowkit/_models/gating_strategy.py
+src/flowkit/_models/sample.py
+src/flowkit/_models/session.py
+src/flowkit/_models/workspace.py
+src/flowkit/_models/gates/__init__.py
+src/flowkit/_models/gates/_base_gate.py
+src/flowkit/_models/gates/_gates.py
+src/flowkit/_models/gates/_gml_gates.py
+src/flowkit/_models/gates/_wsp_gates.py
+src/flowkit/_models/transforms/__init__.py
+src/flowkit/_models/transforms/_base_transform.py
+src/flowkit/_models/transforms/_matrix.py
+src/flowkit/_models/transforms/_transforms.py
+src/flowkit/_models/transforms/_wsp_transforms.py
+src/flowkit/_resources/DataTypes.v2.0.xsd
+src/flowkit/_resources/Gating-ML.v2.0.xsd
+src/flowkit/_resources/Transformations.v2.0.xsd
+src/flowkit/_resources/__init__.py
+src/flowkit/_utils/__init__.py
+src/flowkit/_utils/gating_utils.py
+src/flowkit/_utils/gml_write.py
+src/flowkit/_utils/plot_utils.py
+src/flowkit/_utils/sample_utils.py
+src/flowkit/_utils/wsp_utils.py
+src/flowkit/_utils/xml_common.py
+src/flowkit/_utils/xml_utils.py
```

### Comparing `FlowKit-1.0.1/LICENSE` & `FlowKit-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.1/PKG-INFO` & `FlowKit-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,49 @@
 Metadata-Version: 2.1
 Name: FlowKit
-Version: 1.0.1
+Version: 1.1.0
 Summary: Flow Cytometry Toolkit
 Home-page: https://github.com/whitews/flowkit
 Author: Scott White
 License: BSD
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: anytree>=2.9
+Requires-Dist: bokeh>=3.1
+Requires-Dist: contourpy>=1.1.0
+Requires-Dist: flowio<1.4,>=1.3.0
+Requires-Dist: flowutils<1.2,>=1.1.0
+Requires-Dist: lxml>=4.9
+Requires-Dist: networkx>=3.1
+Requires-Dist: numpy<2,>=1.22
+Requires-Dist: pandas>=2.0
+Requires-Dist: psutil>=5.8
+Requires-Dist: scipy>=1.8
 
 # FlowKit
 
 [!["FlowKit"](https://raw.githubusercontent.com/whitews/FlowKit/master/docs/_static/flowkit.png)](https://github.com/whitews/flowkit)
 
 [![PyPI license](https://img.shields.io/pypi/l/flowkit.svg?colorB=dodgerblue)](https://pypi.python.org/pypi/flowkit/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/flowkit.svg)](https://pypi.python.org/pypi/flowkit/)
 [![PyPI version](https://img.shields.io/pypi/v/flowkit.svg?colorB=blue)](https://pypi.python.org/pypi/flowkit/)
 [![DOI](https://zenodo.org/badge/138655889.svg)](https://zenodo.org/badge/latestdoi/138655889)
 
 
-[![Build & test (master)](https://github.com/whitews/FlowKit/actions/workflows/tests_master.yml/badge.svg)](https://github.com/whitews/FlowKit/actions/workflows/tests_master.yml)
-[![Build & test (develop)](https://github.com/whitews/FlowKit/actions/workflows/tests_develop.yml/badge.svg)](https://github.com/whitews/FlowKit/actions/workflows/tests_develop.yml)
+[![Test (master)](https://github.com/whitews/FlowKit/actions/workflows/tests_master.yml/badge.svg)](https://github.com/whitews/FlowKit/actions/workflows/tests_master.yml)
+[![Test (develop)](https://github.com/whitews/FlowKit/actions/workflows/tests_develop.yml/badge.svg)](https://github.com/whitews/FlowKit/actions/workflows/tests_develop.yml)
 [![codecov](https://codecov.io/gh/whitews/flowkit/branch/master/graph/badge.svg?token=joeOIVWmHi)](https://codecov.io/gh/whitews/flowkit)
 [![Documentation Status](https://readthedocs.org/projects/flowkit/badge/?version=latest)](https://flowkit.readthedocs.io/en/latest/?badge=latest)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/flowkit)
+
 
 * [Overview](#overview)
 * [Features](#features)
 * [Requirements](#requirements)
 * [Installation](#installation)
 * [Documentation](#documentation)
   * [Tutorials](#tutorials)
@@ -81,35 +95,36 @@
   * Contour density plot of two channels
   * Interactive scatter plot of two channels
   * Interactive scatter plot matrix of any combination of channels
   * Interactive scatter plots of gates with sample events
 
 ## Requirements
 
-FlowKit supports Python version 3.7 - 3.10. All dependencies are installable 
+FlowKit supports Python version 3.8 - 3.12. All dependencies are installable 
 via pip, and are listed below.
 
-> **NOTE**: FlowUtils uses C extensions for significant performance improvements. For most platforms and Python versions, pre-built binaries are available in PyPI (i.e. installable via `pip`). 
->
-> If a pre-built binary of FlowUtils is not available for your environment, the C extensions must be compiled using the source package. NumPy >=1.19 must be installed prior to compiling FlowUtils. If compiling using `gcc`, version 5 or later is required.
+> **NOTE**: FlowUtils uses C extensions for significant performance 
+> improvements. For most platforms and Python versions, pre-built 
+> binaries of FlowUtils are available in PyPI (i.e. installable via 
+> `pip`). If a pre-built binary is not available for your environment, 
+> the C extensions must be compiled using the source package.
 
 Required Python dependencies:
 
-* [flowio](https://github.com/whitews/flowio) == 1.1.1
-* [flowutils](https://github.com/whitews/flowutils) == 1.0.0
-* anytree >= 2.6
-* bokeh >= 2.4, <3.0
-* lxml >= 4.7
-* matplotlib >= 3.5
-* networkx >= 2.3
-* numpy >= 1.20
-* pandas >= 1.2
+* [flowio](https://github.com/whitews/flowio) >= 1.3.0
+* [flowutils](https://github.com/whitews/flowutils) >= 1.1.0
+* anytree >= 2.9
+* bokeh >= 3.1
+* contourpy >= 1.1.0
+* lxml >= 4.9
+* networkx >= 3.1
+* numpy >= 1.22, <2
+* pandas >= 2.0
 * psutils >= 5.8
-* scipy >= 1.6
-* seaborn >= 0.11, <0.12
+* scipy >= 1.8
 
 ## Installation
 
 > **NOTE**: For macOS users running on Apple Silicon, the version of `pip` may need to be upgraded prior to installing FlowKit in order to install the required dependencies.
 
 ### From PyPI
 
@@ -149,16 +164,16 @@
 * [Part 5 - Session Class](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/flowkit-tutorial-part05-session-class.ipynb)
 * [Part 6 - Workspace Class](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/flowkit-tutorial-part06-workspace-class.ipynb)
 
 ### Advanced Examples
 
 Below are more advanced and practical examples for using FlowKit. If you have an example you would like to submit for consideration in this list (preferably with data), please [submit an issue](https://github.com/whitews/FlowKit/issues/new/).
 
-* [Compare mean fluorescence intensity (MFI) in gated populations](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/flowkit-session-compare-mfi-of-gated-events.ipynb)
-* [Importing a FlowJo 10 WSP file & replicating analysis in FlowKit](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/flowkit-session-replicate-flowjo-wsp.ipynb)
+* [Compare mean fluorescence intensity (MFI) in gated populations](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/compare-mfi-of-gated-events.ipynb)
+* [Importing a FlowJo 10 WSP file & replicating analysis in FlowKit](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/replicate-flowjo-wsp.ipynb)
 * [Dimension reduction on gated populations](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/dimension_reduction_on_gated_populations.ipynb)
 * [Comparison between Leiden & Louvain clustering](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/clustering_comparison_leiden_vs_louvain.ipynb)
 * [Saving Flow Analysis Data as AnnData objects for ScanPy](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/scanpy_creating_and_using_AnnData_objects.ipynb)
 
 ## Contributing
 
 Want to get involved in the development of FlowKit? 
@@ -169,9 +184,11 @@
 
 [White, S., Quinn, J., Enzor, J., Staats, J., Mosier, S. M., Almarode, J., Denny, T. N., Weinhold, K. J., Ferrari, G., & Chan, C. (2021). FlowKit: A Python toolkit for integrated manual and automated cytometry analysis workflows. Frontiers in Immunology, 12. https://doi.org/10.3389/fimmu.2021.768541](https://www.frontiersin.org/articles/10.3389/fimmu.2021.768541/full)
 
 ## Projects & Research Using FlowKit 
 
 The following projects and publications have utilized FlowKit. If you have a package or publication where FlowKit was used, and you want it listed here, feel free to [submit an issue](https://github.com/whitews/FlowKit/issues/new/) letting me know.
 
+* Mortelecque, Justine et al. "A selection and optimization strategy for single-domain antibodies targeting the PHF6 linear peptide within the Tau intrinsically disordered protein." Journal of Biological Chemistry (2024), [doi:10.1016/j.jbc.2024.107163](https://www.jbc.org/article/S0021-9258(24)01658-2/fulltext)
+* Schmidt, Florian et al. "In-depth analysis of human virus-specific CD8+ T cells delineates unique phenotypic signatures for T cell specificity prediction." Cell Reports vol. 42,10 (2023), [doi:10.1016/j.celrep.2023.113250](https://www.cell.com/cell-reports/fulltext/S2211-1247(23)01262-7)
 * Schuster, Jonas et al. “Combining real-time fluorescence spectroscopy and flow cytometry to reveal new insights in DOC and cell characterization of drinking water.” Frontiers in Environmental Chemistry (2022), [doi:10.3389/fenvc.2022.931067](https://www.frontiersin.org/articles/10.3389/fenvc.2022.931067/full)
 * Rendeiro, André F et al. "Profiling of immune dysfunction in COVID-19 patients allows early prediction of disease progression." Life science alliance vol. 4,2 e202000955. 24 Dec. 2020, [doi:10.26508/lsa.202000955](https://www.life-science-alliance.org/content/4/2/e202000955.full)
```

### Comparing `FlowKit-1.0.1/README.md` & `FlowKit-1.1.0/src/FlowKit.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,49 @@
+Metadata-Version: 2.1
+Name: FlowKit
+Version: 1.1.0
+Summary: Flow Cytometry Toolkit
+Home-page: https://github.com/whitews/flowkit
+Author: Scott White
+License: BSD
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: anytree>=2.9
+Requires-Dist: bokeh>=3.1
+Requires-Dist: contourpy>=1.1.0
+Requires-Dist: flowio<1.4,>=1.3.0
+Requires-Dist: flowutils<1.2,>=1.1.0
+Requires-Dist: lxml>=4.9
+Requires-Dist: networkx>=3.1
+Requires-Dist: numpy<2,>=1.22
+Requires-Dist: pandas>=2.0
+Requires-Dist: psutil>=5.8
+Requires-Dist: scipy>=1.8
+
 # FlowKit
 
 [!["FlowKit"](https://raw.githubusercontent.com/whitews/FlowKit/master/docs/_static/flowkit.png)](https://github.com/whitews/flowkit)
 
 [![PyPI license](https://img.shields.io/pypi/l/flowkit.svg?colorB=dodgerblue)](https://pypi.python.org/pypi/flowkit/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/flowkit.svg)](https://pypi.python.org/pypi/flowkit/)
 [![PyPI version](https://img.shields.io/pypi/v/flowkit.svg?colorB=blue)](https://pypi.python.org/pypi/flowkit/)
 [![DOI](https://zenodo.org/badge/138655889.svg)](https://zenodo.org/badge/latestdoi/138655889)
 
 
-[![Build & test (master)](https://github.com/whitews/FlowKit/actions/workflows/tests_master.yml/badge.svg)](https://github.com/whitews/FlowKit/actions/workflows/tests_master.yml)
-[![Build & test (develop)](https://github.com/whitews/FlowKit/actions/workflows/tests_develop.yml/badge.svg)](https://github.com/whitews/FlowKit/actions/workflows/tests_develop.yml)
+[![Test (master)](https://github.com/whitews/FlowKit/actions/workflows/tests_master.yml/badge.svg)](https://github.com/whitews/FlowKit/actions/workflows/tests_master.yml)
+[![Test (develop)](https://github.com/whitews/FlowKit/actions/workflows/tests_develop.yml/badge.svg)](https://github.com/whitews/FlowKit/actions/workflows/tests_develop.yml)
 [![codecov](https://codecov.io/gh/whitews/flowkit/branch/master/graph/badge.svg?token=joeOIVWmHi)](https://codecov.io/gh/whitews/flowkit)
 [![Documentation Status](https://readthedocs.org/projects/flowkit/badge/?version=latest)](https://flowkit.readthedocs.io/en/latest/?badge=latest)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/flowkit)
+
 
 * [Overview](#overview)
 * [Features](#features)
 * [Requirements](#requirements)
 * [Installation](#installation)
 * [Documentation](#documentation)
   * [Tutorials](#tutorials)
@@ -67,35 +95,36 @@
   * Contour density plot of two channels
   * Interactive scatter plot of two channels
   * Interactive scatter plot matrix of any combination of channels
   * Interactive scatter plots of gates with sample events
 
 ## Requirements
 
-FlowKit supports Python version 3.7 - 3.10. All dependencies are installable 
+FlowKit supports Python version 3.8 - 3.12. All dependencies are installable 
 via pip, and are listed below.
 
-> **NOTE**: FlowUtils uses C extensions for significant performance improvements. For most platforms and Python versions, pre-built binaries are available in PyPI (i.e. installable via `pip`). 
->
-> If a pre-built binary of FlowUtils is not available for your environment, the C extensions must be compiled using the source package. NumPy >=1.19 must be installed prior to compiling FlowUtils. If compiling using `gcc`, version 5 or later is required.
+> **NOTE**: FlowUtils uses C extensions for significant performance 
+> improvements. For most platforms and Python versions, pre-built 
+> binaries of FlowUtils are available in PyPI (i.e. installable via 
+> `pip`). If a pre-built binary is not available for your environment, 
+> the C extensions must be compiled using the source package.
 
 Required Python dependencies:
 
-* [flowio](https://github.com/whitews/flowio) == 1.1.1
-* [flowutils](https://github.com/whitews/flowutils) == 1.0.0
-* anytree >= 2.6
-* bokeh >= 2.4, <3.0
-* lxml >= 4.7
-* matplotlib >= 3.5
-* networkx >= 2.3
-* numpy >= 1.20
-* pandas >= 1.2
+* [flowio](https://github.com/whitews/flowio) >= 1.3.0
+* [flowutils](https://github.com/whitews/flowutils) >= 1.1.0
+* anytree >= 2.9
+* bokeh >= 3.1
+* contourpy >= 1.1.0
+* lxml >= 4.9
+* networkx >= 3.1
+* numpy >= 1.22, <2
+* pandas >= 2.0
 * psutils >= 5.8
-* scipy >= 1.6
-* seaborn >= 0.11, <0.12
+* scipy >= 1.8
 
 ## Installation
 
 > **NOTE**: For macOS users running on Apple Silicon, the version of `pip` may need to be upgraded prior to installing FlowKit in order to install the required dependencies.
 
 ### From PyPI
 
@@ -135,16 +164,16 @@
 * [Part 5 - Session Class](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/flowkit-tutorial-part05-session-class.ipynb)
 * [Part 6 - Workspace Class](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/flowkit-tutorial-part06-workspace-class.ipynb)
 
 ### Advanced Examples
 
 Below are more advanced and practical examples for using FlowKit. If you have an example you would like to submit for consideration in this list (preferably with data), please [submit an issue](https://github.com/whitews/FlowKit/issues/new/).
 
-* [Compare mean fluorescence intensity (MFI) in gated populations](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/flowkit-session-compare-mfi-of-gated-events.ipynb)
-* [Importing a FlowJo 10 WSP file & replicating analysis in FlowKit](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/flowkit-session-replicate-flowjo-wsp.ipynb)
+* [Compare mean fluorescence intensity (MFI) in gated populations](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/compare-mfi-of-gated-events.ipynb)
+* [Importing a FlowJo 10 WSP file & replicating analysis in FlowKit](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/replicate-flowjo-wsp.ipynb)
 * [Dimension reduction on gated populations](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/dimension_reduction_on_gated_populations.ipynb)
 * [Comparison between Leiden & Louvain clustering](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/clustering_comparison_leiden_vs_louvain.ipynb)
 * [Saving Flow Analysis Data as AnnData objects for ScanPy](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/scanpy_creating_and_using_AnnData_objects.ipynb)
 
 ## Contributing
 
 Want to get involved in the development of FlowKit? 
@@ -155,9 +184,11 @@
 
 [White, S., Quinn, J., Enzor, J., Staats, J., Mosier, S. M., Almarode, J., Denny, T. N., Weinhold, K. J., Ferrari, G., & Chan, C. (2021). FlowKit: A Python toolkit for integrated manual and automated cytometry analysis workflows. Frontiers in Immunology, 12. https://doi.org/10.3389/fimmu.2021.768541](https://www.frontiersin.org/articles/10.3389/fimmu.2021.768541/full)
 
 ## Projects & Research Using FlowKit 
 
 The following projects and publications have utilized FlowKit. If you have a package or publication where FlowKit was used, and you want it listed here, feel free to [submit an issue](https://github.com/whitews/FlowKit/issues/new/) letting me know.
 
+* Mortelecque, Justine et al. "A selection and optimization strategy for single-domain antibodies targeting the PHF6 linear peptide within the Tau intrinsically disordered protein." Journal of Biological Chemistry (2024), [doi:10.1016/j.jbc.2024.107163](https://www.jbc.org/article/S0021-9258(24)01658-2/fulltext)
+* Schmidt, Florian et al. "In-depth analysis of human virus-specific CD8+ T cells delineates unique phenotypic signatures for T cell specificity prediction." Cell Reports vol. 42,10 (2023), [doi:10.1016/j.celrep.2023.113250](https://www.cell.com/cell-reports/fulltext/S2211-1247(23)01262-7)
 * Schuster, Jonas et al. “Combining real-time fluorescence spectroscopy and flow cytometry to reveal new insights in DOC and cell characterization of drinking water.” Frontiers in Environmental Chemistry (2022), [doi:10.3389/fenvc.2022.931067](https://www.frontiersin.org/articles/10.3389/fenvc.2022.931067/full)
 * Rendeiro, André F et al. "Profiling of immune dysfunction in COVID-19 patients allows early prediction of disease progression." Life science alliance vol. 4,2 e202000955. 24 Dec. 2020, [doi:10.26508/lsa.202000955](https://www.life-science-alliance.org/content/4/2/e202000955.full)
```

### Comparing `FlowKit-1.0.1/flowkit/__init__.py` & `FlowKit-1.1.0/src/flowkit/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 from ._models.transforms._matrix import Matrix
 from ._models import transforms
 from ._models import gates
 from ._models.gating_strategy import GatingStrategy
 from ._models.session import Session
 from ._models.workspace import Workspace
 from ._models.dimension import Dimension, RatioDimension, QuadrantDivider
-from ._utils.xml_utils import parse_gating_xml, export_gatingml
+from ._utils.xml_utils import parse_gating_xml
+from ._utils.gml_write import export_gatingml
 from ._utils.wsp_utils import parse_wsp, extract_wsp_sample_data
-from ._utils.sample_utils import load_samples
+from ._utils.sample_utils import load_samples, read_multi_dataset_fcs
 from . import exceptions
 
 from ._version import __version__
 
 __all__ = [
     'Sample',
     'Session',
@@ -29,9 +30,10 @@
     'gates',
     'transforms',
     'parse_gating_xml',
     'export_gatingml',
     'parse_wsp',
     'extract_wsp_sample_data',
     'load_samples',
+    'read_multi_dataset_fcs',
     'exceptions'
 ]
```

### Comparing `FlowKit-1.0.1/flowkit/_conf.py` & `FlowKit-1.1.0/src/flowkit/_conf.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.1/flowkit/_models/dimension.py` & `FlowKit-1.1.0/src/flowkit/_models/dimension.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.1/flowkit/_models/gate_node.py` & `FlowKit-1.1.0/src/flowkit/_models/gate_node.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.1/flowkit/_models/gates/_base_gate.py` & `FlowKit-1.1.0/src/flowkit/_models/gates/_base_gate.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.1/flowkit/_models/gates/_gates.py` & `FlowKit-1.1.0/src/flowkit/_models/gates/_gates.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.1/flowkit/_models/gates/_gml_gates.py` & `FlowKit-1.1.0/src/flowkit/_models/gates/_gml_gates.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 GatingML elements to an intermediate Gate subclass. GML gates differ from
 their parent class in that they retain a parent gate reference which is
 used to assemble the gate tree. They also each provide a
 `convert_to_parent_class` for converting them to their parent class for
 public interaction in a GatingStrategy.
 """
 from .. import gates
-from ..._utils import xml_utils
+from ..._utils import xml_utils, xml_common
 
 
 class GMLRectangleGate(gates.RectangleGate):
     """
     Represents a GatingML Rectangle Gate
 
     A RectangleGate can have one or more dimensions, and each dimension must
@@ -144,15 +144,15 @@
 
         if len(coord_els) == 1:
             raise ValueError(
                 'Ellipsoids must have at least 2 dimensions (line %d)' % gate_element.sourceline
             )
 
         for coord_el in coord_els:
-            value = xml_utils.find_attribute_value(coord_el, data_type_namespace, 'value')
+            value = xml_common.find_attribute_value(coord_el, data_type_namespace, 'value')
             if value is None:
                 raise ValueError(
                     'A coordinate must have only 1 value (line %d)' % coord_el.sourceline
                 )
 
             coordinates.append(float(value))
 
@@ -174,15 +174,15 @@
             row_entry_els = row_el.findall(
                 '%s:entry' % gating_namespace,
                 namespaces=gate_element.nsmap
             )
 
             entry_values = []
             for entry_el in row_entry_els:
-                value = xml_utils.find_attribute_value(entry_el, data_type_namespace, 'value')
+                value = xml_common.find_attribute_value(entry_el, data_type_namespace, 'value')
                 entry_values.append(float(value))
 
             if len(entry_values) != len(coordinates):
                 raise ValueError(
                     'Covariance row entry value count must match # of dimensions (line %d)' % row_el.sourceline
                 )
 
@@ -191,15 +191,15 @@
         # Finally, get the distance square, which is a simple element w/
         # a single value attribute
         distance_square_el = gate_element.find(
             '%s:distanceSquare' % gating_namespace,
             namespaces=gate_element.nsmap
         )
 
-        dist_square_value = xml_utils.find_attribute_value(distance_square_el, data_type_namespace, 'value')
+        dist_square_value = xml_common.find_attribute_value(distance_square_el, data_type_namespace, 'value')
         distance_square = float(dist_square_value)
 
         super().__init__(
             gate_name,
             dimensions,
             coordinates,
             covariance_matrix,
@@ -257,27 +257,27 @@
             '%s:Quadrant' % gating_namespace,
             namespaces=gate_element.nsmap
         )
 
         quadrants = []
 
         for quadrant_el in quadrant_els:
-            quad_id = xml_utils.find_attribute_value(quadrant_el, gating_namespace, 'id')
+            quad_id = xml_common.find_attribute_value(quadrant_el, gating_namespace, 'id')
 
             position_els = quadrant_el.findall(
                 '%s:position' % gating_namespace,
                 namespaces=gate_element.nsmap
             )
 
             divider_refs = []
             divider_ranges = []
 
             for pos_el in position_els:
-                divider_ref = xml_utils.find_attribute_value(pos_el, gating_namespace, 'divider_ref')
-                location = xml_utils.find_attribute_value(pos_el, gating_namespace, 'location')
+                divider_ref = xml_common.find_attribute_value(pos_el, gating_namespace, 'divider_ref')
+                location = xml_common.find_attribute_value(pos_el, gating_namespace, 'location')
                 location = float(location)
                 q_min = None
                 q_max = None
                 dim_id = None
 
                 for div in dividers:
                     if div.id != divider_ref:
@@ -380,21 +380,21 @@
             '%s:gateReference' % gating_namespace,
             namespaces=gate_element.nsmap
         )
 
         gate_refs = []
 
         for gate_ref_el in gate_ref_els:
-            gate_ref = xml_utils.find_attribute_value(gate_ref_el, gating_namespace, 'ref')
+            gate_ref = xml_common.find_attribute_value(gate_ref_el, gating_namespace, 'ref')
             if gate_ref is None:
                 raise ValueError(
                     "Boolean gate reference must specify a 'ref' attribute (line %d)" % gate_ref_el.sourceline
                 )
 
-            use_complement = xml_utils.find_attribute_value(gate_ref_el, gating_namespace, 'use-as-complement')
+            use_complement = xml_common.find_attribute_value(gate_ref_el, gating_namespace, 'use-as-complement')
             if use_complement is not None:
                 use_complement = use_complement == 'true'
             else:
                 use_complement = False
 
             # TODO: see if 'gate_refs' list of dictionaries can be to something more easily documented
             gate_refs.append(
```

### Comparing `FlowKit-1.0.1/flowkit/_models/gates/_wsp_gates.py` & `FlowKit-1.1.0/src/flowkit/_models/gates/_wsp_gates.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.1/flowkit/_models/gating_results.py` & `FlowKit-1.1.0/src/flowkit/_models/gating_results.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.1/flowkit/_models/gating_strategy.py` & `FlowKit-1.1.0/src/flowkit/_models/gating_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,22 +109,22 @@
                 # raise a GateTreeError if it already exists.
                 node.add_custom_gate(sample_id, gate)
         else:
             # We need to create a new node in the tree.
             GateNode(gate, parent_node)
             self._rebuild_dag()
 
-    def is_custom_gate(self, gate_name, gate_path=None, sample_id=None):
+    def is_custom_gate(self, sample_id, gate_name, gate_path=None):
         """
         Determine if a custom gate exists for a sample ID.
 
+        :param sample_id: Sample ID string
         :param gate_name: text string of a gate name
         :param gate_path: complete ordered tuple of gate names for unique set of gate ancestors.
             Required if gate_name is ambiguous
-        :param sample_id: Sample ID string
         :return: Boolean value for whether the sample ID has a custom gate
         """
         node = self._get_gate_node(gate_name, gate_path)
 
         return node.is_custom_gate(sample_id)
 
     def get_gate(self, gate_name, gate_path=None, sample_id=None):
@@ -134,17 +134,16 @@
         exists.
 
         :param gate_name: text string of a gate name
         :param gate_path: complete ordered tuple of gate names for unique set of gate ancestors.
             Required if gate_name is ambiguous
         :param sample_id: Sample ID string to lookup custom gate. If None or not found, template gate is returned
         :return: Subclass of a Gate object
-        :raises
-            GateReferenceError: if gate ID is not found in gating strategy
-            QuadrantReferenceError: if gate ID references a single Quadrant (specify the QuadrantGate ID instead)
+        :raises GateReferenceError: if gate ID is not found in gating strategy
+        :raises QuadrantReferenceError: if gate ID references a single Quadrant (specify the QuadrantGate ID instead)
         """
         node = self._get_gate_node(gate_name, gate_path)
 
         if isinstance(node.gate, fk_gates.Quadrant):
             # A Quadrant isn't a true gate, raise error indicating to call its QuadrantGate
             raise QuadrantReferenceError(
                 "%s references a Quadrant, specify the owning QuadrantGate %s instead" % (gate_name, node.parent)
@@ -846,15 +845,15 @@
             # main QuadrantGate
             try:
                 gate = self.get_gate(g_id, g_path, sample_id=sample_id)
             except QuadrantReferenceError:
                 continue
 
             if verbose:
-                is_custom_gate = self.is_custom_gate(g_id, g_path, sample_id)
+                is_custom_gate = self.is_custom_gate(sample_id, g_id, g_path)
                 if is_custom_gate:
                     custom_gate_str = ' [custom]'
                 else:
                     custom_gate_str = ''
 
                 print("%s: processing gate %s%s" % (sample_id, g_id, custom_gate_str))
```

### Comparing `FlowKit-1.0.1/flowkit/_models/sample.py` & `FlowKit-1.1.0/src/flowkit/_models/sample.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,24 +7,23 @@
 import flowio
 import os
 from pathlib import Path
 import io
 from tempfile import TemporaryFile
 import numpy as np
 import pandas as pd
-import matplotlib.pyplot as plt
-import seaborn
 from bokeh.layouts import gridplot
-from bokeh.models import Title
+from bokeh.models import Title, Range1d
 import warnings
 # noinspection PyProtectedMember
 from .._models.transforms import _transforms
 # noinspection PyProtectedMember
 from .._models.transforms._matrix import Matrix
 from .._utils import plot_utils
+from ..exceptions import FlowKitException
 
 
 @total_ordering
 class Sample(object):
     """
     Represents a single FCS sample from an FCS file, NumPy array or pandas
     DataFrame.
@@ -73,18 +72,18 @@
 
         - Matrix instance
         - NumPy array
         - CSV file path
         - pathlib Path object to a CSV or TSV file
         - string of CSV text
 
-    :param null_channel_list: List of PnN labels for channels that were collected
-        but do not contain useful data. Note, this should only be used if there were
-        truly no fluorochromes used targeting those detectors and the channels
-        do not contribute to compensation.
+    :param null_channel_list: List of PnN labels for acquired channels that do not contain
+        useful data. Note, this should only be used if no fluorochromes were used to target
+        those detectors. Null channels do not contribute to compensation and should not be
+        included in a compensation matrix for this sample.
 
     :param ignore_offset_error: option to ignore data offset error (see above note), default is False
 
     :param ignore_offset_discrepancy: option to ignore discrepancy between the HEADER
         and TEXT values for the DATA byte offset location, default is False
 
     :param use_header_offsets: use the HEADER section for the data offset locations, default is False.
@@ -180,15 +179,20 @@
             raise ValueError("'fcs_path_or_data' is not a supported type")
 
         try:
             self.version = flow_data.header['version']
         except KeyError:
             self.version = None
 
-        self.null_channels = null_channel_list
+        # Ensure null channels is a list for checking later
+        if null_channel_list is None:
+            self.null_channels = []
+        else:
+            self.null_channels = null_channel_list
+
         self.event_count = flow_data.event_count
 
         # make a temp channels dict, self.channels will be a DataFrame built from it
         tmp_channels = flow_data.channels
         self.pnn_labels = list()
         self.pns_labels = list()
         self.fluoro_indices = list()
@@ -226,15 +230,19 @@
                 ]
                 if log0 == 0 and decades != 0:
                     log0 = 1.0  # FCS std states to use 1.0 for invalid 0 value
                 channel_lin_log.append((decades, log0))
             else:
                 channel_lin_log.append((0.0, 0.0))
 
-            if channel_label.lower()[:4] not in ['fsc-', 'ssc-', 'time']:
+            # Determine fluoro vs scatter vs time channels
+            # Null channels are excluded from any category.
+            if channel_label in self.null_channels:
+                pass
+            elif channel_label.lower()[:4] not in ['fsc-', 'ssc-', 'time']:
                 self.fluoro_indices.append(n - 1)
             elif channel_label.lower()[:4] in ['fsc-', 'ssc-']:
                 self.scatter_indices.append(n - 1)
             elif channel_label.lower() == 'time':
                 self.time_index = n - 1
 
             if 'PnS' in tmp_channels[str(n)]:
@@ -465,15 +473,17 @@
         self.subsample_indices = shuffled_indices[:self._subsample_count]
 
     def apply_compensation(self, compensation, comp_id='custom_spill'):
         """
         Applies given compensation matrix to Sample events. If any
         transformation has been applied, it will be re-applied after
         compensation. Compensated events can be retrieved afterward
-        by calling `get_events` with `source='comp'`.
+        by calling `get_events` with `source='comp'`. Note, if the
+        sample specifies null channels then these must not be present
+        in the compensation matrix.
 
         :param compensation: Compensation matrix, which can be a:
 
                 - Matrix instance
                 - NumPy array
                 - CSV file path
                 - pathlib Path object to a CSV or TSV file
@@ -482,112 +492,100 @@
             If a string, both multi-line traditional CSV, and the single
             line FCS spill formats are supported. If a NumPy array, we
             assume the columns are in the same order as the channel labels.
         :param comp_id: text ID for identifying compensation matrix (not used if compensation was a Matrix instance)
         :return: None
         """
         if isinstance(compensation, Matrix):
-            self.compensation = compensation
-            self._comp_events = self.compensation.apply(self)
+            tmp_matrix = compensation
         elif compensation is not None:
             detectors = [self.pnn_labels[i] for i in self.fluoro_indices]
             fluorochromes = [self.pns_labels[i] for i in self.fluoro_indices]
-            self.compensation = Matrix(comp_id, compensation, detectors, fluorochromes)
-            self._comp_events = self.compensation.apply(self)
+            tmp_matrix = Matrix(comp_id, compensation, detectors, fluorochromes)
         else:
-            # compensation must be None so clear any matrix and comp events
-            self.compensation = None
+            # compensation must be None, we'll clear any stored comp events later
+            tmp_matrix = None
+
+        if tmp_matrix is not None:
+            # We don't check null channels b/c Matrix.apply will catch them.
+            # tmp_matrix ensures we don't store comp events or compensation
+            # unless apply succeeds.
+            self._comp_events = tmp_matrix.apply(self)
+            self.compensation = tmp_matrix
+        else:
+            # compensation given was None, clear any matrix and comp events
             self._comp_events = None
+            self.compensation = None
 
         # Re-apply transform if set
         if self.transform is not None:
             self._transformed_events = self._transform(self.transform, self._include_scatter_option)
 
     def get_metadata(self):
         """
         Retrieve FCS metadata.
 
         :return: Dictionary of FCS metadata
         """
         return self.metadata
 
-    def _get_orig_events(self, subsample=False):
+    def _get_orig_events(self):
         """
         Returns 'original' events, i.e. not pre-processed, compensated,
         or transformed.
 
-        :param subsample: Whether to return all events or just the sub-sampled
-            events. Default is False (all events)
         :return: NumPy array of original events
         """
         if self._orig_events is None:
             raise ValueError(
                 "Original events were not cached, to retrieve them create a "
                 "Sample instance with cache_original_events=True"
             )
 
-        if subsample:
-            return self._orig_events[self.subsample_indices]
-        else:
-            return self._orig_events
+        return self._orig_events
 
-    def _get_raw_events(self, subsample=False):
+    def _get_raw_events(self):
         """
         Returns 'raw' events that have been pre-processed to adjust for channel
         gain and lin/log display, but have not been compensated or transformed.
 
-        :param subsample: Whether to return all events or just the sub-sampled
-            events. Default is False (all events)
         :return: NumPy array of raw events
         """
-        if subsample:
-            return self._raw_events[self.subsample_indices]
-        else:
-            return self._raw_events
+        return self._raw_events
 
-    def _get_comp_events(self, subsample=False):
+    def _get_comp_events(self):
         """
         Returns compensated events, (not transformed)
 
-        :param subsample: Whether to return all events or just the sub-sampled
-            events. Default is False (all events)
         :return: NumPy array of compensated events or None if no compensation
             matrix has been applied.
         """
         if self._comp_events is None:
             raise AttributeError(
                 "Compensated events were requested but do not exist.\n"
                 "Call a apply_compensation method prior to retrieving compensated events."
             )
 
-        if subsample:
-            return self._comp_events[self.subsample_indices]
-        else:
-            return self._comp_events
+        return self._comp_events
 
-    def _get_transformed_events(self, subsample=False):
+    def _get_transformed_events(self):
         """
         Returns transformed events. Note, if a compensation matrix has been
         applied then the events returned will be compensated and transformed.
 
-        :param subsample: Whether to return all events or just the sub-sampled
-            events. Default is False (all events)
         :return: NumPy array of transformed events or None if no transform
             has been applied.
         """
         if self._transformed_events is None:
             raise AttributeError(
                 "Transformed events were requested but do not exist.\n"
                 "Call a transform method prior to retrieving transformed events."
             )
 
-        if subsample:
-            return self._transformed_events[self.subsample_indices]
-        else:
-            return self._transformed_events
+        return self._transformed_events
 
     def get_events(self, source='xform', subsample=False):
         """
         Returns a NumPy array of event data.
 
         Note: This method returns the array directly, not a copy of the array. Be careful if you
         are planning to modify returned event data, and make a copy of the array when appropriate.
@@ -596,23 +594,26 @@
             raw (orig + gain), compensated (raw + comp), or transformed (comp + xform) events will
             be returned
         :param subsample: Whether to return all events or just the sub-sampled
             events. Default is False (all events)
         :return: NumPy array of event data
         """
         if source == 'xform':
-            events = self._get_transformed_events(subsample=subsample)
+            events = self._get_transformed_events()
         elif source == 'comp':
-            events = self._get_comp_events(subsample=subsample)
+            events = self._get_comp_events()
         elif source == 'raw':
-            events = self._get_raw_events(subsample=subsample)
+            events = self._get_raw_events()
         elif source == 'orig':
-            events = self._get_orig_events(subsample=subsample)
+            events = self._get_orig_events()
         else:
             raise ValueError("source must be one of 'orig', 'raw', 'comp', or 'xform'")
+        
+        if subsample:
+            events = events[self.subsample_indices]
 
         return events
 
     def as_dataframe(self, source='xform', subsample=False, col_order=None, col_names=None):
         """
         Returns a pandas DataFrame of event data.
 
@@ -642,15 +643,15 @@
 
     def get_channel_number_by_label(self, label):
         """
         Returns the channel number for the given PnN label. Note, this is the
         channel number, as defined in the FCS data (not the channel index), so
         the 1st channel's number is 1 (not 0).
 
-        :param label: PnN label of a channel
+        :param label: PnN channel label
         :return: Channel number (not index)
         """
         if label in self.pnn_labels:
             return self.pnn_labels.index(label) + 1
         else:
             # as a last resort we can try the FJ labels and fail if no match
             return self._flowjo_pnn_labels.index(label) + 1
@@ -725,77 +726,119 @@
             )
 
         return transformed_events
 
     def apply_transform(self, transform, include_scatter=False):
         """
         Applies given transform to Sample events, and overwrites the `transform` attribute.
-        By default, only the fluorescent channels are transformed. For fully customized transformations
-        per channel, the `transform` can be specified as a dictionary mapping PnN labels to an instance
-        of the Transform subclass. If a dictionary of transforms is specified, the `include_scatter`
-        option is ignored and only the channels explicitly included in the transform dictionary will
-        be transformed.
+        By default, only the fluorescent channels are transformed (and excludes null channels).
+        For fully customized transformations per channel, the `transform` can be specified as a
+        dictionary mapping PnN labels to an instance of the Transform subclass. If a dictionary
+        of transforms is specified, the `include_scatter` option is ignored and only the channels
+        explicitly included in the transform dictionary will be transformed.
 
         :param transform: an instance of a Transform subclass or a dictionary where the keys correspond
             to the PnN labels and the value is an instance of a Transform subclass.
         :param include_scatter: Whether to transform the scatter channel in addition to the
             fluorescent channels. Default is False.
         """
         self._transformed_events = self._transform(transform, include_scatter=include_scatter)
         self._include_scatter_option = include_scatter
         self.transform = transform
 
-    def plot_channel(self, channel_label_or_number, source='xform', flag_events=False):
+    def plot_channel(
+            self,
+            channel_label_or_number,
+            source='xform',
+            subsample=True,
+            color_density=True,
+            bin_width=4,
+            event_mask=None,
+            highlight_mask=None,
+            x_min=None,
+            x_max=None,
+            y_min=None,
+            y_max=None
+    ):
         """
         Plot a 2-D histogram of the specified channel data with the x-axis as the event index.
         This is similar to plotting a channel vs Time, except the events are equally
         distributed along the x-axis.
 
         :param channel_label_or_number: A channel's PnN label or number
         :param source: 'raw', 'comp', 'xform' for whether the raw, compensated
             or transformed events are used for plotting
-        :param flag_events: whether to flag events using stored flagged_event indices.
-            Flagged event regions will be highlighted in red. Default is False.
-        :return: Matplotlib Figure instance
+        :param subsample: Whether to use all events for plotting or just the
+            sub-sampled events. Default is True (sub-sampled events). Plotting
+            sub-sampled events is much faster.
+        :param color_density: Whether to color the events by density, similar
+            to a heat map. Default is True.
+        :param bin_width: Bin size to use for the color density, in units of
+            event point size. Larger values produce smoother gradients.
+            Default is 4 for a 4x4 grid size.
+        :param event_mask: Boolean array of events to plot. Takes precedence
+            over highlight_mask (i.e. events marked False in event_mask will
+            never be plotted).
+        :param highlight_mask: Boolean array of event indices to highlight
+            in color. Non-highlighted events will be light grey.
+        :param x_min: Lower bound of x-axis. If None, channel's min value will
+            be used with some padding to keep events off the edge of the plot.
+        :param x_max: Upper bound of x-axis. If None, channel's max value will
+            be used with some padding to keep events off the edge of the plot.
+        :param y_min: Lower bound of y-axis. If None, channel's min value will
+            be used with some padding to keep events off the edge of the plot.
+        :param y_max: Upper bound of y-axis. If None, channel's max value will
+            be used with some padding to keep events off the edge of the plot.
+        :return: A Bokeh Figure object containing the interactive channel plot.
         """
         channel_index = self.get_channel_index(channel_label_or_number)
-        channel_data = self.get_channel_events(channel_index, source=source, subsample=False)
-
-        pnn_label = self.pnn_labels[channel_index]
-        pns_label = self.pns_labels[channel_index]
+        channel_data = self.get_channel_events(channel_index, source=source, subsample=subsample)
 
-        plot_title = " - ".join([pnn_label, pns_label]) if pns_label != '' else pnn_label
+        if subsample:
+            x_idx = self.subsample_indices
+        else:
+            x_idx = np.arange(self.event_count)
 
-        if flag_events and self.flagged_indices is not None:
-            flagged_events = np.zeros(self.event_count)
-            flagged_events[self.flagged_indices] = 1
+        if self.pns_labels[channel_index] != '':
+            channel_label = '%s (%s)' % (self.pns_labels[channel_index], self.pnn_labels[channel_index])
         else:
-            flagged_events = None
+            channel_label = self.pnn_labels[channel_index]
 
-        fig = plt.figure(figsize=(16, 4))
-        ax = fig.add_subplot(1, 1, 1)
+        fig = plot_utils.plot_scatter(
+            x_idx,
+            channel_data,
+            x_label='Events',
+            y_label=channel_label,
+            color_density=color_density,
+            bin_width=bin_width,
+            event_mask=event_mask,
+            highlight_mask=highlight_mask,
+            x_min=x_min,
+            x_max=x_max,
+            y_min=y_min,
+            y_max=y_max
+        )
 
-        plot_utils.plot_channel(channel_data, plot_title, ax, xform=None, flagged_events=flagged_events)
+        fig.aspect_ratio = 3
+        fig.width = 1000
 
         return fig
 
     def plot_contour(
             self,
             x_label_or_number,
             y_label_or_number,
             source='xform',
             subsample=True,
-            plot_contour=True,
             plot_events=False,
+            fill=False,
             x_min=None,
             x_max=None,
             y_min=None,
-            y_max=None,
-            fill=False,
-            fig_size=(8, 8)
+            y_max=None
     ):
         """
         Returns a contour plot of the specified channel events, available
         as raw, compensated, or transformed data.
 
         :param x_label_or_number:  A channel's PnN label or number for x-axis
             data
@@ -803,83 +846,69 @@
             data
         :param source: 'raw', 'comp', 'xform' for whether the raw, compensated
             or transformed events are used for plotting
         :param subsample: Whether to use all events for plotting or just the
             sub-sampled events. Default is True (sub-sampled events). Running
             with all events is not recommended, as the Kernel Density
             Estimation is computationally demanding.
-        :param plot_contour: Whether to display the contour lines. Default is True.
         :param plot_events: Whether to display the event data points in
             addition to the contours. Default is False.
         :param x_min: Lower bound of x-axis. If None, channel's min value will
             be used with some padding to keep events off the edge of the plot.
         :param x_max: Upper bound of x-axis. If None, channel's max value will
             be used with some padding to keep events off the edge of the plot.
         :param y_min: Lower bound of y-axis. If None, channel's min value will
             be used with some padding to keep events off the edge of the plot.
         :param y_max: Upper bound of y-axis. If None, channel's max value will
             be used with some padding to keep events off the edge of the plot.
         :param fill: Whether to fill in color between contour lines. D default
             is False.
-        :param fig_size: Tuple of 2 values specifying the size of the returned
-            figure. Values are in Matplotlib size units.
-        :return: Matplotlib figure of the contour plot
+        :return: A Bokeh figure of the contour plot
         """
         x_index = self.get_channel_index(x_label_or_number)
         y_index = self.get_channel_index(y_label_or_number)
 
         x = self.get_channel_events(x_index, source=source, subsample=subsample)
         y = self.get_channel_events(y_index, source=source, subsample=subsample)
 
-        # noinspection PyProtectedMember
-        x_min, x_max = plot_utils._calculate_extent(x, d_min=x_min, d_max=x_max, pad=0.02)
-        # noinspection PyProtectedMember
-        y_min, y_max = plot_utils._calculate_extent(y, d_min=y_min, d_max=y_max, pad=0.02)
-
-        fig, ax = plt.subplots(figsize=fig_size)
-        ax.set_title(self.id)
-
-        ax.set_xlim([x_min, x_max])
-        ax.set_ylim([y_min, y_max])
-        ax.set_xlabel(self.pnn_labels[x_index])
-        ax.set_ylabel(self.pnn_labels[y_index])
-
-        if plot_events:
-            seaborn.scatterplot(
-                x=x,
-                y=y,
-                palette=plot_utils.new_jet,
-                legend=False,
-                s=6,
-                linewidth=0,
-                alpha=0.4
-            )
+        if self.pns_labels[x_index] != '':
+            x_label = '%s (%s)' % (self.pns_labels[x_index], self.pnn_labels[x_index])
+        else:
+            x_label = self.pnn_labels[x_index]
 
-        if plot_contour:
-            seaborn.kdeplot(
-                x=x,
-                y=y,
-                bw_method='scott',
-                cmap=plot_utils.new_jet,
-                linewidths=2 if not fill else None,
-                alpha=0.6,
-                fill=fill
-            )
+        if self.pns_labels[y_index] != '':
+            y_label = '%s (%s)' % (self.pns_labels[y_index], self.pnn_labels[y_index])
+        else:
+            y_label = self.pnn_labels[y_index]
+
+        fig = plot_utils.plot_contours(
+            x,
+            y,
+            x_label=x_label,
+            y_label=y_label,
+            x_min=x_min,
+            x_max=x_max,
+            y_min=y_min,
+            y_max=y_max,
+            plot_events=plot_events,
+            fill=fill
+        )
 
         return fig
 
     def plot_scatter(
             self,
             x_label_or_number,
             y_label_or_number,
             source='xform',
             subsample=True,
             color_density=True,
             bin_width=4,
-            highlight_indices=None,
+            event_mask=None,
+            highlight_mask=None,
             x_min=None,
             x_max=None,
             y_min=None,
             y_max=None
     ):
         """
         Returns an interactive scatter plot for the specified channel data.
@@ -894,15 +923,18 @@
             sub-sampled events. Default is True (sub-sampled events). Plotting
             sub-sampled events is much faster.
         :param color_density: Whether to color the events by density, similar
             to a heat map. Default is True.
         :param bin_width: Bin size to use for the color density, in units of
             event point size. Larger values produce smoother gradients.
             Default is 4 for a 4x4 grid size.
-        :param highlight_indices: Boolean array of event indices to highlight
+        :param event_mask: Boolean array of events to plot. Takes precedence
+            over highlight_mask (i.e. events marked False in event_mask will
+            never be plotted).
+        :param highlight_mask: Boolean array of event indices to highlight
             in color. Non-highlighted events will be light grey.
         :param x_min: Lower bound of x-axis. If None, channel's min value will
             be used with some padding to keep events off the edge of the plot.
         :param x_max: Upper bound of x-axis. If None, channel's max value will
             be used with some padding to keep events off the edge of the plot.
         :param y_min: Lower bound of y-axis. If None, channel's min value will
             be used with some padding to keep events off the edge of the plot.
@@ -911,51 +943,60 @@
         :return: A Bokeh Figure object containing the interactive scatter plot.
         """
         x_index = self.get_channel_index(x_label_or_number)
         y_index = self.get_channel_index(y_label_or_number)
 
         x = self.get_channel_events(x_index, source=source, subsample=subsample)
         y = self.get_channel_events(y_index, source=source, subsample=subsample)
-        if highlight_indices is not None and subsample:
-            highlight_indices = highlight_indices[self.subsample_indices]
-
-        dim_ids = []
+        if highlight_mask is not None and subsample:
+            highlight_mask = highlight_mask[self.subsample_indices]
+        if event_mask is not None:
+            if subsample:
+                event_mask = event_mask[self.subsample_indices]
+
+            # Verify event_mask has events to show
+            if event_mask.sum() == 0:
+                raise FlowKitException("There are no events to plot for the specified options")
 
         if self.pns_labels[x_index] != '':
-            dim_ids.append('%s (%s)' % (self.pns_labels[x_index], self.pnn_labels[x_index]))
+            x_label = '%s (%s)' % (self.pns_labels[x_index], self.pnn_labels[x_index])
         else:
-            dim_ids.append(self.pnn_labels[x_index])
+            x_label = self.pnn_labels[x_index]
 
         if self.pns_labels[y_index] != '':
-            dim_ids.append('%s (%s)' % (self.pns_labels[y_index], self.pnn_labels[y_index]))
+            y_label = '%s (%s)' % (self.pns_labels[y_index], self.pnn_labels[y_index])
         else:
-            dim_ids.append(self.pnn_labels[y_index])
+            y_label = self.pnn_labels[y_index]
 
         p = plot_utils.plot_scatter(
             x,
             y,
-            dim_ids,
+            x_label=x_label,
+            y_label=y_label,
+            event_mask=event_mask,
+            highlight_mask=highlight_mask,
             x_min=x_min,
             x_max=x_max,
             y_min=y_min,
             y_max=y_max,
             color_density=color_density,
-            bin_width=bin_width,
-            highlight_indices=highlight_indices
+            bin_width=bin_width
         )
 
         p.title = Title(text=self.id, align='center')
 
         return p
 
     def plot_scatter_matrix(
             self,
             channel_labels_or_numbers=None,
             source='xform',
             subsample=True,
+            event_mask=None,
+            highlight_mask=None,
             color_density=False,
             plot_height=256,
             plot_width=256
     ):
         """
         Returns an interactive scatter plot matrix for all channel combinations
         except for the Time channel.
@@ -964,14 +1005,19 @@
             numbers to use for the scatter plot matrix. If None, then all
             channels will be plotted (except Time).
         :param source: 'raw', 'comp', 'xform' for whether the raw, compensated
             or transformed events are used for plotting
         :param subsample: Whether to use all events for plotting or just the
             sub-sampled events. Default is True (sub-sampled events). Plotting
             sub-sampled events is much faster.
+        :param event_mask: Boolean array of events to plot. Takes precedence
+            over highlight_mask (i.e. events marked False in event_mask will
+            never be plotted).
+        :param highlight_mask: Boolean array of event indices to highlight
+            in color. Non-highlighted events will be light grey.
         :param color_density: Whether to color the events by density, similar
             to a heat map. Default is False.
         :param plot_height: Height of plot in pixels (screen units)
         :param plot_width: Width of plot in pixels (screen units)
         :return: A Bokeh Figure object containing the interactive scatter plot
             matrix.
         """
@@ -992,65 +1038,92 @@
             if channel_y == 'Time':
                 continue
             row = []
             for channel_x in channels:
                 if channel_x == 'Time':
                     continue
 
-                plot = self.plot_scatter(
-                    channel_x,
-                    channel_y,
-                    source=source,
-                    subsample=subsample,
-                    color_density=color_density
-                )
+                # check if we're at the diagonal,
+                # don't plot past to avoid duplicates
+                if channel_x == channel_y:
+                    # plot histogram instead of scatter plot
+                    plot = self.plot_histogram(
+                        channel_x, source=source, subsample=subsample
+                    )
+                else:
+                    plot = self.plot_scatter(
+                        channel_x,
+                        channel_y,
+                        source=source,
+                        subsample=subsample,
+                        event_mask=event_mask,
+                        highlight_mask=highlight_mask,
+                        color_density=color_density
+                    )
+
                 plot.height = plot_height
                 plot.width = plot_width
                 row.append(plot)
+
             plots.append(row)
 
         grid = gridplot(plots)
 
         return grid
 
     def plot_histogram(
             self,
             channel_label_or_number,
             source='xform',
             subsample=False,
-            bins=None
+            bins=None,
+            data_min=None,
+            data_max=None,
+            x_range=None
     ):
         """
-        Returns a histogram plot of the specified channel events, available
-        as raw, compensated, or transformed data. Plot also contains a curve
-        of the gaussian kernel density estimate.
+        Returns a histogram plot of the specified channel events
 
         :param channel_label_or_number:  A channel's PnN label or number to use
             for plotting the histogram
         :param source: 'raw', 'comp', 'xform' for whether the raw, compensated
             or transformed events are used for plotting
         :param subsample: Whether to use all events for plotting or just the
             sub-sampled events. Default is False (all events).
         :param bins: Number of bins to use for the histogram or a string compatible
             with the NumPy histogram function. If None, the number of bins is
             determined by the square root rule.
-        :return: Matplotlib figure of the histogram plot with KDE curve.
+        :param data_min: filter event data, removing events below specified value
+        :param data_max: filter event data, removing events above specified value
+        :param x_range: Tuple of lower & upper bounds of x-axis. Used for modifying
+            plot view, doesn't filter event data.
+        :return: Bokeh figure of the histogram plot.
         """
 
         channel_index = self.get_channel_index(channel_label_or_number)
         channel_data = self.get_channel_events(channel_index, source=source, subsample=subsample)
 
+        if data_min is not None:
+            channel_data = channel_data[channel_data >= data_min]
+
+        if data_max is not None:
+            channel_data = channel_data[channel_data <= data_max]
+
         p = plot_utils.plot_histogram(
             channel_data,
             x_label=self.pnn_labels[channel_index],
             bins=bins
         )
 
         p.title = Title(text=self.id, align='center')
 
+        if x_range is not None:
+            x_range = Range1d(x_range[0], x_range[1])
+            p.x_range = x_range
+
         return p
 
     def _get_metadata_for_export(self, source, include_all=False):
         metadata_dict = {}
         ignore_keywords = ['timestep']
 
         # If the original events were requested, need to make sure
@@ -1138,17 +1211,17 @@
             used for exporting
         :param exclude_neg_scatter: Whether to exclude negative scatter events. Default is False.
         :param exclude_flagged: Whether to exclude flagged events. Default is False.
         :param exclude_normal: Whether to exclude "normal" events. This is useful for retrieving all
              the "bad" events (neg scatter and/or flagged events). Default is False.
         :param subsample: Whether to export all events or just the sub-sampled events.
             Default is False (all events).
-        :param include_metadata: Whether to include all key/value pairs in self.metadata in the output
-            FCS file. Only valid for .fcs file extension. If False, only the minimum amount of
-            metadata will be included in the output FCS file. Default is False.
+        :param include_metadata: Whether to include all key/value pairs from the metadata attribute
+            in the output FCS file. Only valid for .fcs file extension. If False, only the minimum
+            amount of metadata will be included in the output FCS file. Default is False.
         :param directory: Directory path where the exported file will be saved. If None, the file
             will be saved in the current working directory.
         :return: None
         """
         # get the requested file type (either .fcs or .csv)
         ext = os.path.splitext(filename)[-1].lower()
```

### Comparing `FlowKit-1.0.1/flowkit/_models/session.py` & `FlowKit-1.1.0/src/flowkit/_models/workspace.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,316 +1,432 @@
 """
-Session class
+Workspace class
 """
 import gc
-import io
 import copy
+import os
 import numpy as np
 import pandas as pd
 from bokeh.models import Title
 from .._conf import debug
-from .._models.gating_strategy import GatingStrategy
-from .._models import gates, dimension
-from .._utils import plot_utils, xml_utils, wsp_utils, sample_utils, gating_utils
-from ..exceptions import GateReferenceError
+from .._utils import plot_utils, wsp_utils, sample_utils, gating_utils
+from ..exceptions import FlowKitException, GateReferenceError
 import warnings
 
 
-class Session(object):
+class Workspace(object):
     """
-    The Session class enables the programmatic creation of a gating strategy or for importing
-    GatingML compliant documents. A Session combines multiple Sample instances with a single
-    GatingStrategy. The gates in the gating strategy can be customized per sample.
+    A Workspace represents an imported FlowJo workspace (.wsp file).
 
+    :param wsp_file_path: FlowJo WSP file as a file name/path, file object, or file-like object
     :param fcs_samples: str or list. If given a string, it can be a directory path or a file path.
-            If a directory, any .fcs files in the directory will be loaded. If a list, then it must
-            be a list of file paths or a list of Sample instances. Lists of mixed types are not
-            supported.
+        If a directory, any .fcs files in the directory will be found. If a list, then it must
+        be a list of file paths or a list of Sample instances. Lists of mixed types are not
+        supported. Note that only FCS files matching the ones referenced in the .wsp file will
+        be retained in the Workspace.
+    :param ignore_missing_files: Controls behavior for missing FCS files. If True, gate data for
+        missing FCS files (i.e. not in fcs_samples arg) will still be loaded. If False, warnings
+        are issued for FCS files found in the WSP file that were not loaded in the Workspace and
+        gate data for these missing files will not be retained. Default is False.
+    :param find_fcs_files_from_wsp: Controls whether to search for FCS files based on `URI` params within the FlowJo
+        workspace file.
     """
-    def __init__(self, gating_strategy=None, fcs_samples=None):
-        self.sample_lut = {}
+    def __init__(self, wsp_file_path, fcs_samples=None, ignore_missing_files=False, find_fcs_files_from_wsp=False):
+        # The sample LUT holds sample IDs (keys) only for loaded samples.
+        # The values are the Sample instances
+        self._sample_lut = {}
+
+        # The sample data LUT holds sample IDs (keys) for all samples
+        # that have WSP gating data whether the sample is loaded or not.
+        # The value is a dict containing the following items:
+        #   - 'keywords': dict of FCS metadata found in WSP file
+        #   - 'compensation' dict of spill info found in WSP file
+        #   - 'transforms': dict of channel transforms found in WSP file
+        #   - 'custom_gate_ids': set of gate paths for custom gates
+        #   - 'gating_strategy': GatingStrategy assembled from WSP file
+        self._sample_data_lut = {}
+
+        # The group LUT keys are the available sample group names.
+        # The values are dicts with keys 'gates' & 'samples'.
+        # 'gates' has the common group Gate instances (not a
+        # full GatingStrategy though) and 'samples' is a list
+        # of the sample IDs belonging to the group.
+        self._group_lut = {}
+
+        # For storing GatingResults for analyzed samples.
+        # Keys are sample IDs. We could put these in the
+        # sample_lut but sample_lut is meant to be created
+        # and complete within this constructor. Plus, this
+        # makes it easier to determine which samples have
+        # been analyzed.
         self._results_lut = {}
+        
+        # load samples we were given, we'll cross-reference against wsp below
+        tmp_sample_lut = {s.id: s for s in sample_utils.load_samples(fcs_samples)}
+        self._sample_lut = {}
+
+        wsp_data = wsp_utils.parse_wsp(wsp_file_path)
+
+        # find samples in wsp file. in wsp_data['samples'], each item is a dict which has a key `sample_uri`
+        if find_fcs_files_from_wsp:
+            if fcs_samples is not None:
+                warnings.warn("When `find_fcs_files_from_wsp` is True, `fcs_samples` will be ignored.")
+
+            tmp_sample_lut = {}
+    
+            for sample_name in wsp_data['samples']:
+                sample_data = wsp_data['samples'][sample_name]
+                sample_uri = sample_data['sample_uri']
+
+                # Convert the URI to a path
+                # noinspection PyProtectedMember
+                path = wsp_utils._uri_to_path(sample_uri, wsp_file_path)
+
+                # Test whether file exists at path and if not present
+                # warn user with message indicating the path.
+                if not os.path.exists(path):
+                    warnings.warn("Sample file not found at path: {}".format(path))
+                    continue
+
+                # Read in the sample file
+                sample_filedata = sample_utils.load_samples(path)[0]
+
+                # Update the ID of the loaded data (otherwise analysis breaks)
+                sample_filedata.id = sample_name
+
+                tmp_sample_lut[sample_name] = sample_filedata
+
+        # save group sample membership, we'll filter by loaded samples next
+        group_lut = wsp_data['groups']
+
+        # save sample data, including the GatingStrategy & Sample instance
+        for sample_id, sample_dict in wsp_data['samples'].items():
+            if sample_id in tmp_sample_lut:
+                # retain sample and add to sample data
+                self._sample_lut[sample_id] = tmp_sample_lut[sample_id]
+                self._sample_data_lut[sample_id] = sample_dict
+            else:
+                # we have gating info for a sample that wasn't loaded
+                if ignore_missing_files:
+                    # we're instructed to ignore missing files, so we'll still
+                    # save the gate info for retrieval purposes
+                    self._sample_data_lut[sample_id] = sample_dict
+                else:
+                    # we won't ignore missing files, issue a warning
+                    # and remove any references to the sample
+                    msg = "WSP references %s, but sample was not loaded." % sample_id
+                    warnings.warn(msg)
+
+                    # search for this missing sample ID in group data & remove
+                    for group_name, group_dict in group_lut.items():
+                        if sample_id in group_dict['samples']:
+                            group_dict['samples'].remove(sample_id)
 
-        if isinstance(gating_strategy, GatingStrategy):
-            gating_strategy = gating_strategy
-        elif isinstance(gating_strategy, str) or isinstance(gating_strategy, io.IOBase):
-            # assume a path to an XML file representing a GatingML document
-            gating_strategy = xml_utils.parse_gating_xml(gating_strategy)
-        elif gating_strategy is None:
-            gating_strategy = GatingStrategy()
-        else:
-            raise ValueError(
-                "'gating_strategy' must be a GatingStrategy instance, GatingML document path, or None"
-            )
-
-        self.gating_strategy = gating_strategy
-
-        self.add_samples(fcs_samples)
+        self._group_lut = group_lut
 
     def __repr__(self):
-        sample_count = len(self.sample_lut)
+        sample_count = len(self._sample_lut)
+        sample_group_count = len(self._group_lut)
 
         return (
             f'{self.__class__.__name__}('
-            f'{sample_count} samples)'
+            f'{sample_count} samples loaded, '
+            f'{sample_group_count} sample groups)'
         )
 
-    def add_samples(self, fcs_samples):
+    def summary(self):
         """
-        Adds FCS samples to the session.
+        Retrieve a summary of Workspace information, including a list of
+        sample groups defined, along with the sample and gate counts
+        for those sample groups.
+
+        :return: Pandas DataFrame containing Workspace summary information
+        """
+        sg_list = []
+
+        for group_name, group_dict in self._group_lut.items():
+            group_sample_ids = group_dict['samples']
+            sample_count = len(group_sample_ids)
+
+            loaded_sample_count = 0
+            for g_sample_id in group_sample_ids:
+                if g_sample_id in self._sample_lut:
+                    loaded_sample_count += 1
+
+            if sample_count > 0:
+                # There's at least one sample, so grab the first one
+                # as the prototype for the gating strategy. A WSP
+                # group isn't guaranteed to have template gates for
+                # the complete gate tree, this is the best we can do.
+                example_sample_id = group_dict['samples'][0]
+                gs = self.get_gating_strategy(example_sample_id)
 
-        :param fcs_samples: str or list. If given a string, it can be a directory path or a file path.
-            If a directory, any .fcs files in the directory will be loaded. If a list, then it must
-            be a list of file paths or a list of Sample instances. Lists of mixed types are not
-            supported.
-        :return: None
-        """
-        new_samples = sample_utils.load_samples(fcs_samples)
-        for s in new_samples:
-            if s.id in self.sample_lut:
-                warnings.warn("A sample with ID %s already exists...skipping" % s.id)
-                continue
-            self.sample_lut[s.id] = s
-
-    def get_sample_ids(self):
-        """
-        Retrieve the list of Sample IDs in the Session.
+                gate_count = len(gs.get_gate_ids())
+                gate_depth = gs.get_max_depth()
+            else:
+                gate_count = 0
+                gate_depth = 0
 
+            sg_info = {
+                'group_name': group_name,
+                'samples': sample_count,
+                'loaded_samples': loaded_sample_count,
+                'gates': gate_count,
+                'max_gate_depth': gate_depth
+            }
+
+            sg_list.append(sg_info)
+
+        df = pd.DataFrame(sg_list)
+        df.set_index('group_name', inplace=True)
+
+        return df
+
+    def get_sample_ids(self, group_name=None, loaded_only=True):
+        """
+        Retrieve the list of Sample IDs that in the Workspace, optionally
+        filtered by sample group and/or loaded status. Default is all loaded
+        samples.
+
+        :param group_name: Filter returned sample IDs by a sample group. If None, all sample IDs are returned
+        :param loaded_only: Filter returned sample IDs for only loaded samples. If False, all the samples will
+            be returned, including any missing sample IDs referenced in the workspace. Default is True for
+            returning only loaded sample IDs.
         :return: list of Sample ID strings
         """
-        return list(self.sample_lut.keys())
-
-    def get_gate_ids(self):
-        """
-        Retrieve the list of gate IDs defined for the Session's gating
-        strategy. The gate ID is a 2-item tuple where the first item
-        is a string representing the gate name and the second item is
-        a tuple of the gate path.
-
-        :return: list of gate ID tuples
-        """
-        return self.gating_strategy.get_gate_ids()
-
-    def add_gate(self, gate, gate_path, sample_id=None):
-        """
-        Add a Gate instance to the gating strategy. The gate ID and gate path
-        must be unique in the gating strategy. Custom sample gates may be added
-        by specifying an optional sample ID. Note, the gate & gate path must
-        already exist prior to adding custom sample gates.
-
-        :param gate: an instance of a Gate subclass
-        :param gate_path: complete tuple of gate IDs for unique set of gate ancestors
-        :param sample_id: text string for specifying given gate as a custom Sample gate
-        :return: None
-        """
-        self.gating_strategy.add_gate(copy.deepcopy(gate), gate_path=gate_path, sample_id=sample_id)
-
-    def remove_gate(self, gate_name, gate_path=None, keep_children=False):
-        """
-        Remove a gate from the gate tree. Any descendant gates will also be removed
-        unless keep_children=True. In all cases, if a BooleanGate exists that references
-        the gate to remove, a GateTreeError will be thrown indicating the BooleanGate
-        must be removed prior to removing the gate.
+        if group_name is not None:
+            # group LUT contains all group sample IDs incl. missing ones
+            sample_ids = set(self._group_lut[group_name]['samples'])
+        else:
+            # No group name specified so give user all sample IDs
+            # sample data LUT contains all sample IDs, incl. missing IDs
+            # referenced in the wsp (if ignore_missing_files was True)
+            sample_ids = set(self._sample_data_lut.keys())
+
+        # check if only loaded samples were requested
+        if loaded_only:
+            # sample LUT contains all the loaded sample IDs
+            loaded_sample_ids = set(self._sample_lut.keys())
 
-        :param gate_name: text string of a gate name
-        :param gate_path: complete tuple of gate IDs for unique set of gate ancestors.
-            Required if gate_name is ambiguous
-        :param keep_children: Whether to keep child gates. If True, the child gates will be
-            remapped to the removed gate's parent. Default is False, which will delete all
-            descendant gates.
-        :return: None
-        """
-        self.gating_strategy.remove_gate(gate_name, gate_path=gate_path, keep_children=keep_children)
+            # cross-reference sample_ids with loaded_sample_ids
+            sample_ids = sample_ids.intersection(loaded_sample_ids)
 
-    def add_transform(self, transform):
-        """
-        Add a Transform instance to use in the gating strategy.
+        return sorted(list(sample_ids))
 
-        :param transform: an instance of a Transform subclass
-        :return: None
-        """
-        self.gating_strategy.add_transform(copy.deepcopy(transform))
-
-    def get_transforms(self):
+    def get_sample(self, sample_id):
         """
-        Retrieve the list of Transform instances stored in the gating strategy.
+        Retrieve a Sample instance from the Workspace.
 
-        :return: list of Transform instances
+        :param sample_id: a text string representing the sample
+        :return: a Sample instance
         """
+        return self._sample_lut[sample_id]
 
-        return list(self.gating_strategy.transformations.values())
-
-    def get_transform(self, transform_id):
+    def get_samples(self, group_name=None):
         """
-        Retrieve a Transform stored in the gating strategy by its ID.
+        Retrieve list of Sample instances, optionally filtered by sample group.
 
-        :param transform_id: a text string representing a Transform ID
-        :return: an instance of a Transform subclass
+        :param group_name: Filter returned samples by a sample group. If None, all samples are returned
+        :return: list of Sample instances
         """
-        return self.gating_strategy.get_transform(transform_id)
+        # don't return samples that haven't been loaded
+        sample_ids = self.get_sample_ids(group_name=group_name)
 
-    def add_comp_matrix(self, matrix):
-        """
-        Add a Matrix instance to use in the gating strategy.
+        samples = []
+        for s_id in sample_ids:
+            samples.append(self._sample_lut[s_id])
 
-        :param matrix: an instance of the Matrix class
-        :return: None
-        """
-        self.gating_strategy.add_comp_matrix(copy.deepcopy(matrix))
+        return samples
 
-    def get_comp_matrices(self):
+    def get_sample_groups(self):
         """
-        Retrieve the list of compensation Matrix instances stored in the gating strategy.
+        Retrieve the list of sample group names defined in the Workspace.
 
-        :return: list of Matrix instances
+        :return: list of sample group ID strings
         """
-        return list(self.gating_strategy.comp_matrices.values())
+        return list(self._group_lut.keys())
 
-    def get_comp_matrix(self, matrix_id):
+    def get_gate_ids(self, sample_id):
         """
-        Retrieve a compensation Matrix instance stored in the gating strategy by its ID.
+        Retrieve the list of gate IDs defined for the specified sample.
+        The gate ID is a 2-item tuple where the first item is a string
+        representing the gate name and the second item is a tuple of
+        the gate path.
 
-        :param matrix_id: a text string representing a Matrix ID
-        :return: a Matrix instance
+        :param sample_id: a text string representing a Sample instance
+        :return: list of gate ID tuples
         """
-        return self.gating_strategy.get_comp_matrix(matrix_id)
+        gs = self._sample_data_lut[sample_id]['gating_strategy']
+        return gs.get_gate_ids()
 
-    def find_matching_gate_paths(self, gate_name):
+    def find_matching_gate_paths(self, sample_id, gate_name):
         """
-        Find all gate paths in the gating strategy matching the given gate name.
+        Find all gate paths in the gating strategy for the given Sample
+        matching the given gate name.
 
+        :param sample_id: a text string representing a Sample instance
         :param gate_name: text string of a gate name
         :return: list of gate paths (list of tuples)
         """
-        return self.gating_strategy.find_matching_gate_paths(gate_name)
+        gs = self._sample_data_lut[sample_id]['gating_strategy']
+        return gs.find_matching_gate_paths(gate_name)
 
-    def get_child_gate_ids(self, gate_name, gate_path=None):
+    def get_child_gate_ids(self, sample_id, gate_name, gate_path=None):
         """
-        Retrieve list of child gate IDs given the parent gate name (and path if ambiguous)
-        in the gating strategy.
+        Retrieve list of child gate IDs for a sample given the parent
+        gate name (and path if ambiguous) in the gating strategy.
 
+        :param sample_id: a text string representing a Sample instance
         :param gate_name: text string of a gate name
         :param gate_path: complete tuple of gate IDs for unique set of gate ancestors.
             Required if gate.gate_name is ambiguous
         :return: list of Gate IDs (tuple of gate name plus gate path). Returns an empty
             list if no child gates exist.
         :raises GateReferenceError: if gate ID is not found in gating strategy or if gate
             name is ambiguous
         """
-        return self.gating_strategy.get_child_gate_ids(gate_name, gate_path)
+        gs = self._sample_data_lut[sample_id]['gating_strategy']
+        child_gate_ids = gs.get_child_gate_ids(gate_name, gate_path)
 
-    def get_gate(self, gate_name, gate_path=None, sample_id=None):
+        return child_gate_ids
+
+    def get_gate_hierarchy(self, sample_id, output='ascii', **kwargs):
         """
-        Retrieve a gate instance by its gate ID (and sample ID for custom sample gates).
+        Retrieve the hierarchy of gates in the sample's gating strategy. Output is available
+        in several formats, including text, dictionary, or JSON. If output == 'json', extra
+        keyword arguments are passed to json.dumps
 
-        :param gate_name: text string of a gate ID
-        :param gate_path: tuple of gate IDs for unique set of gate ancestors. Required if gate_name is ambiguous
-        :param sample_id: a text string representing a Sample instance. If None, the template gate is returned.
-        :return: Subclass of a Gate object
+        :param sample_id: a text string representing a Sample instance
+        :param output: Determines format of hierarchy returned, either 'ascii',
+            'dict', or 'JSON' (default is 'ascii')
+        :return: gate hierarchy as a text string or a dictionary
         """
-        return self.gating_strategy.get_gate(gate_name, gate_path=gate_path, sample_id=sample_id)
+        gs = self._sample_data_lut[sample_id]['gating_strategy']
+        return gs.get_gate_hierarchy(output, **kwargs)
 
-    def get_sample_gates(self, sample_id):
+    def get_gating_strategy(self, sample_id):
         """
-        Retrieve all gates for a sample in the gating strategy. This returns custom sample
-        gates for the specified sample ID.
+        Retrieve a copy of the GatingStrategy for a specific sample. sample_id is required as
+        each sample may have customized gates
 
         :param sample_id: a text string representing a Sample instance
-        :return: list of Gate subclass instances
+        :return: a copy of the GatingStrategy instance
         """
-        gate_tuples = self.gating_strategy.get_gate_ids()
+        return copy.deepcopy(self._sample_data_lut[sample_id]['gating_strategy'])
 
-        sample_gates = []
+    def get_comp_matrix(self, sample_id):
+        """
+        Retrieve the compensation matrix for a specific sample.
 
-        for gate_name, ancestors in gate_tuples:
-            gate = self.gating_strategy.get_gate(gate_name, gate_path=ancestors, sample_id=sample_id)
-            sample_gates.append(gate)
+        :param sample_id: a text string representing a Sample instance
+        :return: a copy of a Matrix instance
+        """
+        sample_dict = self._sample_data_lut[sample_id]
 
-        return sample_gates
+        if sample_dict['compensation'] is not None:
+            comp_matrix = copy.deepcopy(sample_dict['compensation']['matrix'])
+        else:
+            comp_matrix = None
 
-    def get_gate_hierarchy(self, output='ascii', **kwargs):
-        """
-        Retrieve the hierarchy of gates in the gating strategy. Output is available
-        in several formats, including text, dictionary, or JSON. If output == 'json', extra
-        keyword arguments are passed to json.dumps
+        return comp_matrix
 
-        :param output: Determines format of hierarchy returned, either 'ascii',
-            'dict', or 'JSON' (default is 'ascii')
-        :return: gate hierarchy as a text string or a dictionary
+    def get_transform(self, sample_id, transform_id):
         """
-        return self.gating_strategy.get_gate_hierarchy(output, **kwargs)
+        Retrieve a single transform for a sample using the transform ID. Transform
+        IDs in the Workspace class correspond to a channel label in the sample.
 
-    def export_gml(self, file_handle, sample_id=None):
+        :param sample_id: a text string representing a Sample instance
+        :param transform_id: a text string representing a Transform instance
+        :return:
         """
-        Export a GatingML 2.0 file for the gating strategy. Specify the sample ID to use
-        that sample's custom gates in the exported file, otherwise the template gates
-        will be exported.
+        sample_dict = self._sample_data_lut[sample_id]
 
-        :param file_handle: file handle for exporting data
-        :param sample_id: an optional text string representing a Sample instance
-        :return: None
-        """
-        xml_utils.export_gatingml(self.gating_strategy, file_handle, sample_id=sample_id)
+        if sample_dict['transforms'] is not None:
+            xform = copy.deepcopy(sample_dict['transforms'][transform_id])
+        else:
+            xform = None
 
-    def export_wsp(self, file_handle, group_name):
+        return xform
+
+    def get_transforms(self, sample_id):
         """
-        Export a FlowJo 10 workspace file (.wsp) for the gating strategy.
+        Retrieve the list of transformations for a specific sample.
 
-        :param file_handle: file handle for exporting data
-        :param group_name: a text string representing the sample group to add to the WSP file
-        :return: None
+        :param sample_id: a text string representing a Sample instance
+        :return: a list of Transform instances
         """
-        samples = self.sample_lut.values()
+        sample_dict = self._sample_data_lut[sample_id]
 
-        wsp_utils.export_flowjo_wsp(self.gating_strategy, group_name, samples, file_handle)
+        if sample_dict['transforms'] is not None:
+            xforms = copy.deepcopy(list(sample_dict['transforms'].values()))
+        else:
+            xforms = None
 
-    def get_sample(self, sample_id):
+        return xforms
+
+    def get_gate(self, sample_id, gate_name, gate_path=None):
         """
-        Retrieve a Sample instance from the Session.
+        Retrieve a gate instance for a sample by its gate ID.
 
-        :param sample_id: a text string representing the sample
-        :return: Sample instance
+        :param sample_id: a text string representing a Sample instance.
+        :param gate_name: text string of a gate ID
+        :param gate_path: tuple of gate IDs for unique set of gate ancestors. Required if gate_name is ambiguous
+        :return: Subclass of a Gate object
         """
-        return self.sample_lut[sample_id]
+        gs = self._sample_data_lut[sample_id]['gating_strategy']
+        return gs.get_gate(gate_name, gate_path=gate_path)
 
-    def analyze_samples(self, sample_id=None, cache_events=False, use_mp=True, verbose=False):
+    def analyze_samples(self, group_name=None, sample_id=None, cache_events=False, use_mp=True, verbose=False):
         """
-        Process gating strategy for samples. After running, results can be retrieved
-        using the `get_gating_results`, `get_report`, and  `get_gate_membership`,
-        methods.
+        Process gates for samples. Samples to analyze can be filtered by group name or sample ID.
+        After running, results can be retrieved using the `get_gating_results`, `get_group_report`,
+        and  `get_gate_membership`, methods.
 
-        :param sample_id: optional sample ID, if specified only this sample will be processed
+        :param group_name: optional group name, if specified only samples in this group will be processed
+        :param sample_id: optional sample ID, if specified only this sample will be processed (overrides group filter)
         :param cache_events: Whether to cache pre-processed events (compensated and transformed). This can
             be useful to speed up processing of gates that share the same pre-processing instructions for
             the same channel data, but can consume significantly more memory space. See the related
             clear_cache method for additional information. Default is False.
         :param use_mp: Controls whether multiprocessing is used to gate samples (default is True).
             Multiprocessing can fail for large workloads (lots of samples & gates) due to running out of
             memory. If encountering memory errors, set use_mp to False (processing will take longer,
             but will use significantly less memory).
         :param verbose: if True, print a line for every gate processed (default is False)
         :return: None
         """
         # Don't save just the DataFrame report, save the entire
         # GatingResults objects for each sample, since we'll need the gate
         # indices for each sample.
-        samples = self.sample_lut.values()
-        if len(samples) == 0:
-            warnings.warn("No samples have been loaded in the Session")
-            return
-
         if sample_id is not None:
-            samples = [self.get_sample(sample_id)]
+            sample_ids = [sample_id]
+        else:
+            # If group name is specified, get_sample_ids will return the
+            # group sample IDs. If not then it will return all sample IDs.
+            sample_ids = self.get_sample_ids(group_name=group_name)
+
+        if len(sample_ids) == 0:
+            warnings.warn("No samples were found to analyze")
+            return
 
         sample_data_to_run = []
-        for s in samples:
+        for s_id in sample_ids:
+            if s_id not in self._sample_data_lut:
+                # sample ID provided isn't present in Workspace
+                # or was referenced but has no gate data.
+                warnings.warn("Sample %s has no gate data" % s_id)
+                continue
+
+            sample = self._sample_lut[s_id]
+            gating_strategy = self._sample_data_lut[s_id]['gating_strategy']
+
             sample_data_to_run.append(
                 {
-                    'gating_strategy': self.gating_strategy,
-                    'sample': s
+                    'gating_strategy': gating_strategy,
+                    'sample': sample
                 }
             )
 
             # clear any existing results
             if sample_id in self._results_lut:
                 del self._results_lut[sample_id]
                 gc.collect()
@@ -318,98 +434,131 @@
         results = gating_utils.gate_samples(
             sample_data_to_run,
             cache_events,
             verbose,
             use_mp=False if debug else use_mp
         )
 
+        # save the results in results LUT
         for r in results:
             self._results_lut[r.sample_id] = r
 
     def get_gating_results(self, sample_id):
         """
         Retrieve analyzed gating results gates for a sample.
 
         :param sample_id: a text string representing a Sample instance
         :return: GatingResults instance
         """
         try:
             gating_result = self._results_lut[sample_id]
         except KeyError:
             raise KeyError(
-                "No results for %s. Have you run `analyze_samples`?" % sample_id
+                "No results found for %s. Have you run `analyze_samples`?" % sample_id
             )
         return copy.deepcopy(gating_result)
 
-    def get_analysis_report(self):
+    def get_analysis_report(self, group_name=None):
         """
         Retrieve the report for the analyzed samples as a pandas DataFrame.
 
+        :param group_name: optional group name, if specified only results
+            from samples in this group will be processed, otherwise results
+            from all analyzed samples will be returned
         :return: pandas DataFrame
         """
         all_reports = []
+        group_s_ids = self.get_sample_ids(group_name)
+
+        for s_id in group_s_ids:
+            try:
+                result = self._results_lut[s_id]
+            except KeyError:
+                continue
+
+            # avoid Pandas warning about concatenating empty DataFrame instances
+            if len(result.report) == 0:
+                continue
 
-        for s_id, result in self._results_lut.items():
             all_reports.append(result.report)
 
-        return copy.deepcopy(pd.concat(all_reports))
+        # Explicitly setting copy=True even though the default in case
+        # it ever changes. Used to do our own deep copy but Pandas was
+        # already doing this, so it was getting deep copied twice.
+        return pd.concat(all_reports, ignore_index=True, copy=True)
+
+    def _get_processed_events(self, sample_id):
+        """
+        Retrieve a pandas DataFrame containing processed events for specified sample.
+        Compensation and transforms will be applied according to the WSP file.
+
+        :param sample_id: a text string representing a Sample instance
+        :return: pandas DataFrame containing the processed sample events
+        """
+        sample = self.get_sample(sample_id)
+        comp_matrix = self.get_comp_matrix(sample_id)
+        xforms = self.get_transforms(sample_id)
+
+        xform_lut = {xform.id: xform for xform in xforms if not xform.id.startswith('Comp')}
+
+        # default is 'raw' events
+        event_source = 'raw'
+
+        if comp_matrix is not None:
+            sample.apply_compensation(comp_matrix)
+            event_source = 'comp'
+        if xforms is not None:
+            sample.apply_transform(xform_lut)
+            event_source = 'xform'
+
+        events_df = sample.as_dataframe(source=event_source)
+
+        return events_df
 
     def get_gate_membership(self, sample_id, gate_name, gate_path=None):
         """
         Retrieve a boolean array indicating gate membership for the events in the
         specified sample. Note, the same gate ID may be found in multiple gate paths,
         i.e. the gate ID can be ambiguous. In this case, specify the full gate path
         to retrieve gate indices.
 
         :param sample_id: a text string representing a Sample instance
         :param gate_name: text string of a gate name
         :param gate_path: complete tuple of gate IDs for unique set of gate ancestors.
             Required if gate_name is ambiguous
         :return: NumPy boolean array (length of sample event count)
         """
-        gating_result = self._results_lut[sample_id]
+        gating_result = self.get_gating_results(sample_id)
         return gating_result.get_gate_membership(gate_name, gate_path=gate_path)
 
-    def get_gate_events(self, sample_id, gate_name=None, gate_path=None, matrix=None, transform=None):
+    def get_gate_events(self, sample_id, gate_name=None, gate_path=None):
         """
-        Retrieve a pandas DataFrame containing only the events within the specified gate.
-        If an optional compensation matrix and/or a transform is provided, the returned
-        event data will be compensated or transformed. If both a compensation matrix and
-        a transform is provided the event data will be both compensated and transformed.
+        Retrieve gated events for a specific gate & sample as a pandas DataFrame.
+        Gated events are processed according to the sample's compensation &
+        channel transforms.
 
         :param sample_id: a text string representing a Sample instance
-        :param gate_name: text string of a gate name. If None, all Sample events will be returned (i.e. un-gated)
+        :param gate_name: text string of a gate ID. If None, all Sample events will be returned (i.e. un-gated)
         :param gate_path: complete tuple of gate IDs for unique set of gate ancestors.
             Required if gate_name is ambiguous
-        :param matrix: an instance of the Matrix class
-        :param transform: an instance of a Transform subclass
-        :return: pandas DataFrame containing only the events within the specified gate
+        :return: a pandas DataFrames with the gated events, compensated & transformed according
+            to the group's compensation matrix and transforms
         """
-        # TODO: re-evaluate whether this method should be removed or modified...the
-        #   ambiguous transforms per channel make this tricky to implement.
-        sample = self.get_sample(sample_id)
-        sample = copy.deepcopy(sample)
-
-        # default is 'raw' events
-        event_source = 'raw'
-
-        if matrix is not None:
-            sample.apply_compensation(matrix)
-            event_source = 'comp'
-        if transform is not None:
-            sample.apply_transform(transform)
-            event_source = 'xform'
-
-        events_df = sample.as_dataframe(source=event_source)
+        df_events = self._get_processed_events(sample_id)
 
         if gate_name is not None:
             gate_idx = self.get_gate_membership(sample_id, gate_name, gate_path)
-            events_df = events_df[gate_idx]
+            df_events = df_events[gate_idx]
 
-        return events_df
+        # TODO: maybe make an optional kwarg to control column label format
+        df_events.columns = [' '.join(col).strip() for col in df_events.columns]
+
+        df_events.insert(0, 'sample_id', sample_id)
+
+        return df_events
 
     def plot_gate(
             self,
             sample_id,
             gate_name,
             gate_path=None,
             subsample_count=10000,
@@ -448,248 +597,78 @@
         :param bin_width: Bin size to use for the color density, in units of
             event point size. Larger values produce smoother gradients.
             Default is 4 for a 4x4 grid size.
         :return: A Bokeh Figure object containing the interactive scatter plot.
         """
         if gate_path is None:
             # verify the gate_name isn't ambiguous
-            gate_paths = self.find_matching_gate_paths(gate_name)
+            gate_paths = self.find_matching_gate_paths(sample_id, gate_name)
             if len(gate_paths) > 1:
                 raise GateReferenceError(
                     "Multiple gates exist with gate name '%s'. Specify a gate_path to disambiguate." % gate_name
                 )
             gate_path = gate_paths[0]
 
-        gate = self.gating_strategy.get_gate(gate_name, gate_path=gate_path, sample_id=sample_id)
-
-        # check for a boolean gate, there's no reasonable way to plot these
-        if isinstance(gate, gates.BooleanGate):
-            raise TypeError("Plotting Boolean gates is not allowed (gate %s)" % gate.gate_name)
-
+        gate_id = (gate_name, gate_path)
         parent_gate_name = gate_path[-1]
         parent_gate_path = gate_path[:-1]
 
-        dim_ids_ordered = []
-        dim_is_ratio = []
-        dim_comp_refs = []
-        dim_min = []
-        dim_max = []
-        for i, dim in enumerate(gate.dimensions):
-            if isinstance(dim, dimension.RatioDimension):
-                dim_ids_ordered.append(dim.ratio_ref)
-                tmp_dim_min = dim.min
-                tmp_dim_max = dim.max
-                is_ratio = True
-            elif isinstance(dim, dimension.QuadrantDivider):
-                dim_ids_ordered.append(dim.dimension_ref)
-                tmp_dim_min = None
-                tmp_dim_max = None
-                is_ratio = False
-            else:
-                dim_ids_ordered.append(dim.id)
-                tmp_dim_min = dim.min
-                tmp_dim_max = dim.max
-                is_ratio = False
-
-            dim_min.append(tmp_dim_min)
-            dim_max.append(tmp_dim_max)
-            dim_is_ratio.append(is_ratio)
-            dim_comp_refs.append(dim.compensation_ref)
-
-        # dim count determines if we need a histogram, scatter, or multi-scatter
-        dim_count = len(dim_ids_ordered)
-        if dim_count == 1:
-            gate_type = 'hist'
-        elif dim_count == 2:
-            gate_type = 'scatter'
-        elif dim_count > 2:
-            raise NotImplementedError("Plotting of gates with >2 dimensions is not supported")
-        else:
-            # there are no dimensions
-            raise ValueError("Gate %s appears to not reference any dimensions" % gate_name)
-
-        # Get Sample instance and apply requested subsampling
-        sample_to_plot = self.get_sample(sample_id)
-        sample_to_plot.subsample_events(subsample_count=subsample_count, random_seed=random_seed)
-        # noinspection PyProtectedMember
-        events = self.gating_strategy._preprocess_sample_events(
-            sample_to_plot,
-            gate
-        )
+        # Get Sample instance and its GatingStrategy
+        sample = self.get_sample(sample_id)
+        gating_strategy = self.get_gating_strategy(sample_id)
 
         # get parent gate results to display only those events
         if parent_gate_name != 'root':
             # TODO:  make it clear to call analyze_samples prior to calling this method
-            is_parent_event = self.get_gate_membership(sample_id, parent_gate_name, parent_gate_path)
-            is_subsample = np.zeros(sample_to_plot.event_count, dtype=bool)
-            is_subsample[sample_to_plot.subsample_indices] = True
-            idx_to_plot = np.logical_and(is_parent_event, is_subsample)
+            parent_event_mask = self.get_gate_membership(sample_id, parent_gate_name, parent_gate_path)
         else:
-            idx_to_plot = sample_to_plot.subsample_indices
-
-        x = events.loc[idx_to_plot, dim_ids_ordered[0]].values
-
-        dim_ids = []
-
-        if dim_is_ratio[0]:
-            dim_ids.append(dim_ids_ordered[0])
-            x_pnn_label = None
-        else:
-            try:
-                x_index = sample_to_plot.get_channel_index(dim_ids_ordered[0])
-            except ValueError:
-                # might be a label reference in the comp matrix
-                matrix = self.gating_strategy.get_comp_matrix(dim_comp_refs[0])
-                try:
-                    matrix_dim_idx = matrix.fluorochomes.index(dim_ids_ordered[0])
-                except ValueError:
-                    raise ValueError("%s not found in list of matrix fluorochromes" % dim_ids_ordered[0])
-                detector = matrix.detectors[matrix_dim_idx]
-                x_index = sample_to_plot.get_channel_index(detector)
-
-            x_pnn_label = sample_to_plot.pnn_labels[x_index]
+            parent_event_mask = None
 
-            if sample_to_plot.pns_labels[x_index] != '':
-                dim_ids.append('%s (%s)' % (sample_to_plot.pns_labels[x_index], x_pnn_label))
-            else:
-                dim_ids.append(sample_to_plot.pnn_labels[x_index])
-
-        y_pnn_label = None
-
-        if dim_count > 1:
-            if dim_is_ratio[1]:
-                dim_ids.append(dim_ids_ordered[1])
-
-            else:
-                try:
-                    y_index = sample_to_plot.get_channel_index(dim_ids_ordered[1])
-                except ValueError:
-                    # might be a label reference in the comp matrix
-                    matrix = self.gating_strategy.get_comp_matrix(dim_comp_refs[1])
-                    try:
-                        matrix_dim_idx = matrix.fluorochomes.index(dim_ids_ordered[1])
-                    except ValueError:
-                        raise ValueError("%s not found in list of matrix fluorochromes" % dim_ids_ordered[1])
-                    detector = matrix.detectors[matrix_dim_idx]
-                    y_index = sample_to_plot.get_channel_index(detector)
-
-                y_pnn_label = sample_to_plot.pnn_labels[y_index]
-
-                if sample_to_plot.pns_labels[y_index] != '':
-                    dim_ids.append('%s (%s)' % (sample_to_plot.pns_labels[y_index], y_pnn_label))
-                else:
-                    dim_ids.append(sample_to_plot.pnn_labels[y_index])
-
-        if gate_type == 'scatter':
-            y = events.loc[idx_to_plot, dim_ids_ordered[1]].values
-
-            p = plot_utils.plot_scatter(
-                x,
-                y,
-                dim_ids,
-                x_min=x_min,
-                x_max=x_max,
-                y_min=y_min,
-                y_max=y_max,
-                color_density=color_density,
-                bin_width=bin_width
-            )
-        elif gate_type == 'hist':
-            p = plot_utils.plot_histogram(x, dim_ids[0])
-        else:
-            raise NotImplementedError("Only histograms and scatter plots are supported in this version of FlowKit")
-
-        if isinstance(gate, gates.PolygonGate):
-            source, glyph = plot_utils.render_polygon(gate.vertices)
-            p.add_glyph(source, glyph)
-        elif isinstance(gate, gates.EllipsoidGate):
-            ellipse = plot_utils.render_ellipse(
-                gate.coordinates[0],
-                gate.coordinates[1],
-                gate.covariance_matrix,
-                gate.distance_square
-            )
-            p.add_glyph(ellipse)
-        elif isinstance(gate, gates.RectangleGate):
-            # rectangle gates in GatingML may not actually be rectangles, as the min/max for the dimensions
-            # are options. So, if any of the dim min/max values are missing it is essentially a set of ranges.
-
-            if None in dim_min or None in dim_max or dim_count == 1:
-                renderers = plot_utils.render_ranges(dim_min, dim_max)
-
-                p.renderers.extend(renderers)
-            else:
-                # a true rectangle
-                rect = plot_utils.render_rectangle(dim_min, dim_max)
-                p.add_glyph(rect)
-        elif isinstance(gate, gates.QuadrantGate):
-            x_locations = []
-            y_locations = []
-
-            for div in gate.dimensions:
-                if div.dimension_ref == x_pnn_label:
-                    x_locations.extend(div.values)
-                elif div.dimension_ref == y_pnn_label and y_pnn_label is not None:
-                    y_locations.extend(div.values)
-
-            renderers = plot_utils.render_dividers(x_locations, y_locations)
-            p.renderers.extend(renderers)
-        else:
-            raise NotImplementedError(
-                "Plotting of %s gates is not supported in this version of FlowKit" % gate.__class__
-            )
-
-        if gate_path is not None:
-            full_gate_path = gate_path[1:]  # omit 'root'
-            full_gate_path = full_gate_path + (gate_name,)
-            sub_title = ' > '.join(full_gate_path)
-
-            # truncate beginning of long gate paths
-            if len(sub_title) > 72:
-                sub_title = '...' + sub_title[-69:]
-            p.add_layout(
-                Title(text=sub_title, text_font_style="italic", text_font_size="1em", align='center'),
-                'above'
-            )
-        else:
-            p.add_layout(
-                Title(text=gate_name, text_font_style="italic", text_font_size="1em", align='center'),
-                'above'
-            )
-
-        plot_title = "%s" % sample_id
-        p.add_layout(
-            Title(text=plot_title, text_font_size="1.1em", align='center'),
-            'above'
+        p = plot_utils.plot_gate(
+            gate_id,
+            gating_strategy,
+            sample,
+            subsample_count=subsample_count,
+            random_seed=random_seed,
+            event_mask=parent_event_mask,
+            x_min=x_min,
+            x_max=x_max,
+            y_min=y_min,
+            y_max=y_max,
+            color_density=color_density,
+            bin_width=bin_width
         )
 
         return p
 
     def plot_scatter(
             self,
             sample_id,
-            x_dim,
-            y_dim,
+            x_label,
+            y_label,
             gate_name=None,
+            gate_path=None,
             subsample_count=10000,
             random_seed=1,
             color_density=True,
             bin_width=4,
             x_min=None,
             x_max=None,
             y_min=None,
             y_max=None
     ):
         """
         Returns an interactive scatter plot for the specified channel data.
 
         :param sample_id: The sample ID for the FCS sample to plot
-        :param x_dim:  Dimension instance to use for the x-axis data
-        :param y_dim: Dimension instance to use for the y-axis data
+        :param x_label: channel label (PnN) to use for the x-axis data
+        :param y_label: channel label (PnN) to use for the y-axis data
         :param gate_name: Gate name to filter events (only events within the given gate will be plotted)
+        :param gate_path: tuple of gate names for full set of gate ancestors.
+            Required if gate_name is ambiguous
         :param subsample_count: Number of events to use as a sub-sample. If the number of
             events in the Sample is less than the requested sub-sample count, then the
             maximum number of available events is used for the sub-sample.
         :param random_seed: Random seed used for sub-sampling events
         :param color_density: Whether to color the events by density, similar
             to a heat map. Default is True.
         :param bin_width: Bin size to use for the color density, in units of
@@ -705,77 +684,70 @@
             be used with some padding to keep events off the edge of the plot.
         :return: A Bokeh Figure object containing the interactive scatter plot.
         """
         # Get Sample instance and apply requested subsampling
         sample = self.get_sample(sample_id)
         sample.subsample_events(subsample_count=subsample_count, random_seed=random_seed)
 
-        x_index = sample.get_channel_index(x_dim.id)
-        y_index = sample.get_channel_index(y_dim.id)
-
-        x_comp_ref = x_dim.compensation_ref
-        x_xform_ref = x_dim.transformation_ref
+        # Build Dimension instances for the requested x & y labels from
+        # the dedicated comp matrix & transform set for this sample.
+        comp_matrix = self.get_comp_matrix(sample_id)
+        x_xform = self.get_transform(sample_id, x_label)
+        y_xform = self.get_transform(sample_id, y_label)
 
-        y_comp_ref = y_dim.compensation_ref
-        y_xform_ref = y_dim.transformation_ref
+        x_index = sample.get_channel_index(x_label)
+        y_index = sample.get_channel_index(y_label)
 
-        if x_comp_ref is not None and x_comp_ref != 'uncompensated':
-            x_comp = self.gating_strategy.get_comp_matrix(x_dim.compensation_ref)
-            comp_events = x_comp.apply(sample)
+        if comp_matrix is not None:
+            comp_events = comp_matrix.apply(sample)
             x = comp_events[:, x_index]
-        else:
-            # not doing sub-sample here, will do later with bool AND
-            x = sample.get_channel_events(x_index, source='raw', subsample=False)
-
-        if y_comp_ref is not None and x_comp_ref != 'uncompensated':
-            # this is likely unnecessary as the x & y comp should be the same,
-            # but requires more conditionals to cover
-            y_comp = self.gating_strategy.get_comp_matrix(x_dim.compensation_ref)
-            comp_events = y_comp.apply(sample)
             y = comp_events[:, y_index]
         else:
             # not doing sub-sample here, will do later with bool AND
+            x = sample.get_channel_events(x_index, source='raw', subsample=False)
             y = sample.get_channel_events(y_index, source='raw', subsample=False)
 
-        if x_xform_ref is not None:
-            x_xform = self.gating_strategy.get_transform(x_xform_ref)
-            x = x_xform.apply(x.reshape(-1, 1))[:, 0]
-        if y_xform_ref is not None:
-            y_xform = self.gating_strategy.get_transform(y_xform_ref)
-            y = y_xform.apply(y.reshape(-1, 1))[:, 0]
+        if x_xform is not None:
+            x = x_xform.apply(x)
+        if y_xform is not None:
+            y = y_xform.apply(y)
 
         if gate_name is not None:
             gate_results = self.get_gating_results(sample_id=sample_id)
-            is_gate_event = gate_results.get_gate_membership(gate_name)
+            is_gate_event = gate_results.get_gate_membership(gate_name, gate_path)
         else:
             is_gate_event = np.ones(sample.event_count, dtype=bool)
 
         is_subsample = np.zeros(sample.event_count, dtype=bool)
         is_subsample[sample.subsample_indices] = True
 
         idx_to_plot = np.logical_and(is_gate_event, is_subsample)
+
+        # check if there are any events to plot
+        if idx_to_plot.sum() == 0:
+            raise FlowKitException("There are no events to plot for the specified options")
+
         x = x[idx_to_plot]
         y = y[idx_to_plot]
 
-        dim_ids = []
-
         if sample.pns_labels[x_index] != '':
-            dim_ids.append('%s (%s)' % (sample.pns_labels[x_index], sample.pnn_labels[x_index]))
+            x_label = '%s (%s)' % (sample.pns_labels[x_index], sample.pnn_labels[x_index])
         else:
-            dim_ids.append(sample.pnn_labels[x_index])
+            x_label = sample.pnn_labels[x_index]
 
         if sample.pns_labels[y_index] != '':
-            dim_ids.append('%s (%s)' % (sample.pns_labels[y_index], sample.pnn_labels[y_index]))
+            y_label = '%s (%s)' % (sample.pns_labels[y_index], sample.pnn_labels[y_index])
         else:
-            dim_ids.append(sample.pnn_labels[y_index])
+            y_label = sample.pnn_labels[y_index]
 
         p = plot_utils.plot_scatter(
             x,
             y,
-            dim_ids,
+            x_label=x_label,
+            y_label=y_label,
             x_min=x_min,
             x_max=x_max,
             y_min=y_min,
             y_max=y_max,
             color_density=color_density,
             bin_width=bin_width
         )
```

### Comparing `FlowKit-1.0.1/flowkit/_models/transforms/_base_transform.py` & `FlowKit-1.1.0/src/flowkit/_models/transforms/_base_transform.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.1/flowkit/_models/transforms/_matrix.py` & `FlowKit-1.1.0/src/flowkit/_models/transforms/_matrix.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Matrix class
 """
+from copy import copy
 import numpy as np
 import pandas as pd
 import flowutils
+from ...exceptions import FlowKitException
 
 
 class Matrix(object):
     """
     Represents a single compensation matrix from a CSV/TSV file, NumPy array or pandas
     DataFrame.
 
@@ -36,28 +38,39 @@
         if matrix_id == 'uncompensated' or matrix_id.lower() == 'fcs':
             raise ValueError(
                 "Matrix IDs 'uncompensated' and 'FCS' are reserved compensation references " +
                 "used in Dimension instances to specify that channel data should either be " +
                 "uncompensated or compensated using the spill value from a Sample's metadata"
             )
 
+        # Copy detectors b/c it may be modified
+        detectors = copy(detectors)
+
         if isinstance(spill_data_or_file, np.ndarray):
             spill = spill_data_or_file
         else:
             spill = flowutils.compensate.parse_compensation_matrix(
                 spill_data_or_file,
                 detectors,
                 null_channels=null_channels
             )
             spill = spill[1:, :]
 
         self.id = matrix_id
         self.matrix = spill
-        # TODO: Should we use a different name other than 'fluorochromes'? They are typically antibodies or markers.
+
+        # Remove any null channels from detector list
+        if null_channels is not None:
+            for nc in null_channels:
+                if nc in detectors:
+                    detectors.remove(nc)
+
         self.detectors = detectors
+
+        # TODO: Should we use a different name other than 'fluorochromes'? They are typically antibodies or markers.
         # Note: fluorochromes attribute is required for compatibility with GatingML exports,
         #       as the GatingML 2.0 requires both the set of detectors and fluorochromes.
         if fluorochromes is None:
             fluorochromes = ['' for _ in detectors]
 
         self.fluorochomes = fluorochromes
 
@@ -70,14 +83,20 @@
     def apply(self, sample):
         """
         Apply compensation matrix to given Sample instance.
 
         :param sample: Sample instance with matching set of detectors
         :return: NumPy array of compensated events
         """
+        # Check that sample fluoro channels match the
+        # matrix detectors
+        sample_fluoro_labels = [sample.pnn_labels[i] for i in sample.fluoro_indices]
+        if not set(self.detectors).issubset(sample_fluoro_labels):
+            raise FlowKitException("Detectors must be a subset of the Sample's fluorochomes")
+
         indices = [
             sample.get_channel_index(d) for d in self.detectors
         ]
         events = sample.get_events(source='raw')
 
         return flowutils.compensate.compensate(
             events,
@@ -88,14 +107,20 @@
     def inverse(self, sample):
         """
         Apply compensation matrix to given Sample instance.
 
         :param sample: Sample instance with matching set of detectors
         :return: NumPy array of compensated events
         """
+        # Check that sample fluoro channels match the
+        # matrix detectors
+        sample_fluoro_labels = [sample.pnn_labels[i] for i in sample.fluoro_indices]
+        if not set(self.detectors).issubset(sample_fluoro_labels):
+            raise FlowKitException("Detectors must be a subset of the Sample's fluorochomes")
+
         indices = [
             sample.get_channel_index(d) for d in self.detectors
         ]
         events = sample.get_events(source='comp')
 
         return flowutils.compensate.inverse_compensate(
             events,
```

### Comparing `FlowKit-1.0.1/flowkit/_models/transforms/_transforms.py` & `FlowKit-1.1.0/src/flowkit/_models/transforms/_transforms.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -275,17 +275,17 @@
     The Logicle transformation was originally defined in the publication:
 
     Moore WA and Parks DR. Update for the logicle data scale including operational
     code implementations. Cytometry A., 2012:81A(4):273–277.
 
     :param transform_id: A string identifying the transform
     :param param_t: parameter for the top of the linear scale (e.g. 262144)
+    :param param_w: parameter for the approximate number of decades in the linear region
     :param param_m: parameter for the number of decades the true logarithmic scale
         approaches at the high end of the scale
-    :param param_w: parameter for the approximate number of decades in the linear region
     :param param_a: parameter for the additional number of negative decades
     """
     def __init__(
         self,
         transform_id,
         param_t,
         param_w,
```

### Comparing `FlowKit-1.0.1/flowkit/_models/transforms/_wsp_transforms.py` & `FlowKit-1.1.0/src/flowkit/_models/transforms/_wsp_transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,29 +207,31 @@
         positive=4.418540,
         max_value=262144.000029
     ):
         Transform.__init__(self, transform_id)
 
         self.negative = negative
         self.width = width
+        self.positive = positive
+        self.max_value = max_value
 
         x, y = generate_biex_lut(neg=self.negative, width_basis=self.width, pos=positive, max_value=max_value)
 
         # create interpolation function with any values outside the range set to the min / max of LUT
         self._lut_func = interpolate.interp1d(
             x, y, kind='linear', bounds_error=False, fill_value=(np.min(y), np.max(y))
         )
         self._inverse_lut_func = interpolate.interp1d(
             y, x, kind='linear', bounds_error=False, fill_value=(np.min(x), np.max(x))
         )
 
     def __repr__(self):
         return (
             f'{self.__class__.__name__}('
-            f'{self.id}, width: {self.width}, neg: {self.negative})'
+            f'{self.id}, width: {self.width}, neg: {self.negative}, pos: {self.positive}, top: {self.max_value})'
         )
 
     def apply(self, events):
         """
         Apply transform to given events.
 
         :param events: NumPy array of FCS event data
```

### Comparing `FlowKit-1.0.1/flowkit/_models/workspace.py` & `FlowKit-1.1.0/src/flowkit/_utils/plot_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,891 +1,844 @@
 """
-Workspace class
+Utility functions related to plotting
 """
-import gc
-import copy
 import numpy as np
-import pandas as pd
-from bokeh.models import Title
-from .._conf import debug
+from scipy.interpolate import interpn
+import contourpy
+from bokeh.plotting import figure
+from bokeh.models import Ellipse, Patch, Span, BoxAnnotation, Rect, ColumnDataSource, Title
+from scipy.stats import gaussian_kde
 from .._models import gates, dimension
-from .._utils import plot_utils, wsp_utils, sample_utils, gating_utils
-from ..exceptions import FlowKitException, GateReferenceError
-import warnings
-
-
-class Workspace(object):
-    """
-    A Workspace represents an imported FlowJo workspace (.wsp file).
-
-    :param wsp_file_path: FlowJo WSP file as a file name/path, file object, or file-like object
-    :param fcs_samples: str or list. If given a string, it can be a directory path or a file path.
-        If a directory, any .fcs files in the directory will be found. If a list, then it must
-        be a list of file paths or a list of Sample instances. Lists of mixed types are not
-        supported. Note that only FCS files matching the ones referenced in the .wsp file will
-        be retained in the Workspace.
-    :param ignore_missing_files: Controls behavior for missing FCS files. If True, gate data for
-        missing FCS files (i.e. not in fcs_samples arg) will still be loaded. If False, warnings
-        are issued for FCS files found in the WSP file that were not loaded in the Workspace and
-        gate data for these missing files will not be retained. Default is False.
-    """
-    def __init__(self, wsp_file_path, fcs_samples=None, ignore_missing_files=False):
-        # The sample LUT holds sample IDs (keys) only for loaded samples.
-        # The values are the Sample instances
-        self._sample_lut = {}
-
-        # The sample data LUT holds sample IDs (keys) for all samples
-        # that have WSP gating data whether the sample is loaded or not.
-        # The value is a dict containing the following items:
-        #   - 'keywords': dict of FCS metadata found in WSP file
-        #   - 'compensation' dict of spill info found in WSP file
-        #   - 'transforms': dict of channel transforms found in WSP file
-        #   - 'custom_gate_ids': set of gate paths for custom gates
-        #   - 'gating_strategy': GatingStrategy assembled from WSP file
-        self._sample_data_lut = {}
-
-        # The group LUT keys are the available sample group names.
-        # The values are dicts with keys 'gates' & 'samples'.
-        # 'gates' has the common group Gate instances (not a
-        # full GatingStrategy though) and 'samples' is a list
-        # of the sample IDs belonging to the group.
-        self._group_lut = {}
-
-        # For storing GatingResults for analyzed samples.
-        # Keys are sample IDs. We could put these in the
-        # sample_lut but sample_lut is meant to be created
-        # and complete within this constructor. Plus, this
-        # makes it easier to determine which samples have
-        # been analyzed.
-        self._results_lut = {}
-
-        # load samples we were given, we'll cross-reference against wsp below
-        tmp_sample_lut = {s.id: s for s in sample_utils.load_samples(fcs_samples)}
-        self._sample_lut = {}
-
-        wsp_data = wsp_utils.parse_wsp(wsp_file_path)
-
-        # save group sample membership, we'll filter by loaded samples next
-        group_lut = wsp_data['groups']
-
-        # save sample data, including the GatingStrategy & Sample instance
-        for sample_id, sample_dict in wsp_data['samples'].items():
-            if sample_id in tmp_sample_lut:
-                # retain sample and add to sample data
-                self._sample_lut[sample_id] = tmp_sample_lut[sample_id]
-                self._sample_data_lut[sample_id] = sample_dict
-            else:
-                # we have gating info for a sample that wasn't loaded
-                if ignore_missing_files:
-                    # we're instructed to ignore missing files, so we'll still
-                    # save the gate info for retrieval purposes
-                    self._sample_data_lut[sample_id] = sample_dict
-                else:
-                    # we won't ignore missing files, issue a warning
-                    # and remove any references to the sample
-                    msg = "WSP references %s, but sample was not loaded." % sample_id
-                    warnings.warn(msg)
-
-                    # search for this missing sample ID in group data & remove
-                    for group_name, group_dict in group_lut.items():
-                        if sample_id in group_dict['samples']:
-                            group_dict['samples'].remove(sample_id)
-
-        self._group_lut = group_lut
-
-    def __repr__(self):
-        sample_count = len(self._sample_lut)
-        sample_group_count = len(self._group_lut)
-
-        return (
-            f'{self.__class__.__name__}('
-            f'{sample_count} samples loaded, '
-            f'{sample_group_count} sample groups)'
-        )
-
-    def summary(self):
-        """
-        Retrieve a summary of Workspace information, including a list of
-        sample groups defined, along with the sample and gate counts
-        for those sample groups.
-
-        :return: Pandas DataFrame containing Workspace summary information
-        """
-        sg_list = []
-
-        for group_name, group_dict in self._group_lut.items():
-            group_sample_ids = group_dict['samples']
-            sample_count = len(group_sample_ids)
-
-            loaded_sample_count = 0
-            for g_sample_id in group_sample_ids:
-                if g_sample_id in self._sample_lut:
-                    loaded_sample_count += 1
-
-            if sample_count > 0:
-                # There's at least one sample, so grab the first one
-                # as the prototype for the gating strategy. A WSP
-                # group isn't guaranteed to have template gates for
-                # the complete gate tree, this is the best we can do.
-                example_sample_id = group_dict['samples'][0]
-                gs = self.get_gating_strategy(example_sample_id)
+from .._models.gating_strategy import GatingStrategy
 
-                gate_count = len(gs.get_gate_ids())
-                gate_depth = gs.get_max_depth()
-            else:
-                gate_count = 0
-                gate_depth = 0
 
-            sg_info = {
-                'group_name': group_name,
-                'samples': sample_count,
-                'loaded_samples': loaded_sample_count,
-                'gates': gate_count,
-                'max_gate_depth': gate_depth
-            }
-
-            sg_list.append(sg_info)
-
-        df = pd.DataFrame(sg_list)
-        df.set_index('group_name', inplace=True)
-
-        return df
-
-    def get_sample_ids(self, group_name=None, loaded_only=True):
-        """
-        Retrieve the list of Sample IDs that in the Workspace, optionally
-        filtered by sample group and/or loaded status. Default is all loaded
-        samples.
-
-        :param group_name: Filter returned sample IDs by a sample group. If None, all sample IDs are returned
-        :param loaded_only: Filter returned sample IDs for only loaded samples. If False, all the samples will
-            be returned, including any missing sample IDs referenced in the workspace. Default is True for
-            returning only loaded sample IDs.
-        :return: list of Sample ID strings
-        """
-        if group_name is not None:
-            # group LUT contains all group sample IDs incl. missing ones
-            sample_ids = set(self._group_lut[group_name]['samples'])
-        else:
-            # No group name specified so give user all sample IDs
-            # sample data LUT contains all sample IDs, incl. missing IDs
-            # referenced in the wsp (if ignore_missing_files was True)
-            sample_ids = set(self._sample_data_lut.keys())
-
-        # check if only loaded samples were requested
-        if loaded_only:
-            # sample LUT contains all the loaded sample IDs
-            loaded_sample_ids = set(self._sample_lut.keys())
-
-            # cross-reference sample_ids with loaded_sample_ids
-            sample_ids = sample_ids.intersection(loaded_sample_ids)
-
-        return sorted(list(sample_ids))
-
-    def get_sample(self, sample_id):
-        """
-        Retrieve a Sample instance from the Workspace.
-
-        :param sample_id: a text string representing the sample
-        :return: a Sample instance
-        """
-        return self._sample_lut[sample_id]
-
-    def get_samples(self, group_name=None):
-        """
-        Retrieve list of Sample instances, optionally filtered by sample group.
-
-        :param group_name: Filter returned samples by a sample group. If None, all samples are returned
-        :return: list of Sample instances
-        """
-        # don't return samples that haven't been loaded
-        sample_ids = self.get_sample_ids(group_name=group_name)
-
-        samples = []
-        for s_id in sample_ids:
-            samples.append(self._sample_lut[s_id])
-
-        return samples
-
-    def get_sample_groups(self):
-        """
-        Retrieve the list of sample group names defined in the Workspace.
-
-        :return: list of sample group ID strings
-        """
-        return list(self._group_lut.keys())
-
-    def get_gate_ids(self, sample_id):
-        """
-        Retrieve the list of gate IDs defined for the specified sample.
-        The gate ID is a 2-item tuple where the first item is a string
-        representing the gate name and the second item is a tuple of
-        the gate path.
-
-        :param sample_id: a text string representing a Sample instance
-        :return: list of gate ID tuples
-        """
-        gs = self._sample_data_lut[sample_id]['gating_strategy']
-        return gs.get_gate_ids()
-
-    def find_matching_gate_paths(self, sample_id, gate_name):
-        """
-        Find all gate paths in the gating strategy for the given Sample
-        matching the given gate name.
-
-        :param sample_id: a text string representing a Sample instance
-        :param gate_name: text string of a gate name
-        :return: list of gate paths (list of tuples)
-        """
-        gs = self._sample_data_lut[sample_id]['gating_strategy']
-        return gs.find_matching_gate_paths(gate_name)
-
-    def get_child_gate_ids(self, sample_id, gate_name, gate_path=None):
-        """
-        Retrieve list of child gate IDs for a sample given the parent
-        gate name (and path if ambiguous) in the gating strategy.
-
-        :param sample_id: a text string representing a Sample instance
-        :param gate_name: text string of a gate name
-        :param gate_path: complete tuple of gate IDs for unique set of gate ancestors.
-            Required if gate.gate_name is ambiguous
-        :return: list of Gate IDs (tuple of gate name plus gate path). Returns an empty
-            list if no child gates exist.
-        :raises GateReferenceError: if gate ID is not found in gating strategy or if gate
-            name is ambiguous
-        """
-        gs = self._sample_data_lut[sample_id]['gating_strategy']
-        child_gate_ids = gs.get_child_gate_ids(gate_name, gate_path)
-
-        return child_gate_ids
-
-    def get_gate_hierarchy(self, sample_id, output='ascii', **kwargs):
-        """
-        Retrieve the hierarchy of gates in the sample's gating strategy. Output is available
-        in several formats, including text, dictionary, or JSON. If output == 'json', extra
-        keyword arguments are passed to json.dumps
-
-        :param sample_id: a text string representing a Sample instance
-        :param output: Determines format of hierarchy returned, either 'ascii',
-            'dict', or 'JSON' (default is 'ascii')
-        :return: gate hierarchy as a text string or a dictionary
-        """
-        gs = self._sample_data_lut[sample_id]['gating_strategy']
-        return gs.get_gate_hierarchy(output, **kwargs)
-
-    def get_gating_strategy(self, sample_id):
-        """
-        Retrieve a copy of the GatingStrategy for a specific sample. sample_id is required as
-        each sample may have customized gates
-
-        :param sample_id: a text string representing a Sample instance
-        :return: a copy of the GatingStrategy instance
-        """
-        return copy.deepcopy(self._sample_data_lut[sample_id]['gating_strategy'])
-
-    def get_comp_matrix(self, sample_id):
-        """
-        Retrieve the compensation matrix for a specific sample.
-
-        :param sample_id: a text string representing a Sample instance
-        :return: a copy of a Matrix instance
-        """
-        sample_dict = self._sample_data_lut[sample_id]
+LINE_COLOR_DEFAULT = "#1F77B4"
+LINE_COLOR_CONTRAST = "#73D587"
+LINE_WIDTH_DEFAULT = 3
+FILL_COLOR_DEFAULT = 'lime'
+FILL_ALPHA_DEFAULT = 0.08
+
+
+custom_heat_palette = [
+    '#000020', '#000021', '#000022', '#000023', '#000024', '#000025', '#000026', '#000027',
+    '#000028', '#000029', '#00002a', '#00002b', '#00002c', '#00002d', '#00002e', '#00002f',
+    '#000030', '#000031', '#000032', '#000033', '#000034', '#000035', '#000036', '#000037',
+    '#000038', '#00003a', '#00003c', '#00003f', '#000042', '#000045', '#000048', '#00004b',
+    '#00004e', '#000151', '#000254', '#000357', '#00045a', '#00045d', '#000560', '#000662',
+    '#000964', '#000c66', '#000f68', '#00126a', '#00166d', '#001a6f', '#001e72', '#002274',
+    '#002677', '#002a79', '#002e7b', '#00327e', '#003680', '#003a83', '#003e85', '#004287',
+    '#00468a', '#004a8c', '#004e8e', '#005290', '#005692', '#005a94', '#005e96', '#006298',
+    '#006699', '#006a9a', '#006f9b', '#00749c', '#007a9d', '#00809e', '#00869f', '#008ca0',
+    '#0091a1', '#0096a2', '#009aa3', '#009ea4', '#00a2a5', '#00a6a6', '#00aaa5', '#00ada4',
+    '#00b0a2', '#00b2a0', '#00b49d', '#00b69a', '#00b797', '#00b894', '#00b991', '#00ba8e',
+    '#00bb8b', '#00bc88', '#00bd85', '#00be82', '#00bf7f', '#00c07c', '#00c179', '#00c276',
+    '#00c373', '#00c470', '#00c56d', '#00c56a', '#00c667', '#00c764', '#00c860', '#00c95b',
+    '#00ca55', '#00cb4e', '#00cb47', '#00cc40', '#00cd39', '#00ce32', '#00ce2b', '#00cf24',
+    '#02d01f', '#07d11a', '#0cd116', '#12d212', '#17d20e', '#1cd30a', '#22d406', '#27d402',
+    '#2dd500', '#34d500', '#3ad600', '#41d600', '#48d700', '#4ed700', '#55d800', '#5cd800',
+    '#62d900', '#68d900', '#6eda00', '#74da00', '#7ada00', '#7fdb00', '#85db00', '#8bdc00',
+    '#90dc00', '#95dc00', '#9add00', '#9edd00', '#a3dd00', '#a8de00', '#acde00', '#b1de00',
+    '#b4de00', '#b6df00', '#b8df00', '#badf00', '#bcdf00', '#bedf00', '#c0df00', '#c2df00',
+    '#c4df00', '#c5df00', '#c7e000', '#c9e000', '#cbe000', '#cce000', '#cee000', '#d0e000',
+    '#d2df00', '#d3de00', '#d5dd00', '#d7db00', '#d9da00', '#dbd900', '#dcd800', '#ded600',
+    '#dfd500', '#dfd300', '#dfd100', '#e0cf00', '#e0cd00', '#e0cc00', '#e0ca00', '#e1c800',
+    '#e1c600', '#e1c500', '#e1c300', '#e1c100', '#e1c000', '#e1be00', '#e1bc00', '#e1bb00',
+    '#e1b900', '#e1b700', '#e1b600', '#e1b400', '#e1b200', '#e1b100', '#e1af00', '#e1ae00',
+    '#e1ac00', '#e1aa00', '#e1a900', '#e1a700', '#e1a500', '#e1a400', '#e1a200', '#e1a000',
+    '#e19f00', '#e09d00', '#e09b00', '#e09900', '#e09800', '#e09600', '#e09400', '#e09300',
+    '#e09100', '#e08f00', '#e08e00', '#e08c00', '#e08a00', '#e08900', '#e08700', '#df8500',
+    '#df8400', '#df8200', '#df8000', '#df7f00', '#df7d00', '#df7b00', '#df7900', '#df7800',
+    '#de7600', '#de7400', '#dd7200', '#dc7000', '#dc6e00', '#db6c00', '#da6a00', '#da6800',
+    '#d76200', '#d45b00', '#d05300', '#cd4c00', '#ca4500', '#c63e00', '#c33700', '#c03000',
+    '#bc2a00', '#b72400', '#b31f00', '#ae1900', '#aa1300', '#a50e00', '#a10800', '#9d0200',
+    '#990200', '#950100', '#920100', '#8e0100', '#8b0000', '#870000', '#840000', '#800000'
+]
+
+
+def _get_false_bounds(bool_array):
+    diff = np.diff(np.hstack((0, bool_array, 0)))
+
+    start = np.where(diff == 1)
+    end = np.where(diff == -1)
+
+    return start[0], end[0]
+
+
+def _calculate_extent(data_1d, d_min=None, d_max=None, pad=0.0):
+    data_min = np.min(data_1d)
+    data_max = np.max(data_1d)
+
+    # determine padding to keep min/max events off the edge
+    pad_d = max(abs(data_min), abs(data_max)) * pad
+
+    if d_min is None:
+        d_min = data_min - pad_d
+    if d_max is None:
+        d_max = data_max + pad_d
+
+    return d_min, d_max
+
+
+def _quantiles_to_levels(data, quantiles):
+    """Return data levels corresponding to quantile cuts of mass."""
+    # Make sure quantiles is a NumPy array
+    quantiles = np.array(quantiles)
+    values = np.ravel(data)
+    sorted_values = np.sort(values)[::-1]
+
+    normalized_values = np.cumsum(sorted_values) / values.sum()
+
+    idx = np.searchsorted(normalized_values, 1 - quantiles)
+    levels = np.take(sorted_values, idx, mode="clip")
+
+    return levels
+
+
+def _calculate_2d_gaussian_kde(x, y, bw_method='scott', grid_size=200, pad_factor=3):
+    """Calculate a 2D PDF from a Gaussian KDE"""
+    # First get the KDE, so we can get the calculated bandwidths
+    # for each dimension to use for padding the grid.
+    kernel = gaussian_kde([x, y], bw_method=bw_method)
+    bw_x, bw_y = np.sqrt(np.diag(kernel.covariance).squeeze())
+
+    min_x, max_x = x.min(), x.max()
+    min_y, max_y = y.min(), y.max()
+
+    # need to pad data edges for the grid calculation
+    grid_min_x = min_x - bw_x * pad_factor
+    grid_max_x = max_x + bw_x * pad_factor
+
+    grid_min_y = min_y - bw_y * pad_factor
+    grid_max_y = max_y + bw_y * pad_factor
+
+    # create meshgrid
+    meshgrid_x, meshgrid_y = np.meshgrid(
+        np.linspace(grid_min_x, grid_max_x, grid_size),
+        np.linspace(grid_min_y, grid_max_y, grid_size)
+    )
+    positions = np.vstack([meshgrid_x.flatten(), meshgrid_y.flatten()])
+
+    # this is the bottleneck step
+    estimated_pdf = np.reshape(kernel(positions).T, meshgrid_x.shape)
+
+    return meshgrid_x, meshgrid_y, estimated_pdf
+
+
+def _build_contour_generator(mesh_x, mesh_y, estimated_pdf):
+    c_gen = contourpy.contour_generator(x=mesh_x, y=mesh_y, z=estimated_pdf)
+
+    return c_gen
+
+
+def render_polygon(
+        vertices,
+        line_color=LINE_COLOR_CONTRAST,
+        line_width=LINE_WIDTH_DEFAULT,
+        fill_color=FILL_COLOR_DEFAULT,
+        fill_alpha=FILL_ALPHA_DEFAULT
+):
+    """
+    Renders a Bokeh polygon for plotting
+    :param vertices: list of 2-D coordinates representing vertices of the polygon
+    :param line_color: Color for the polygon boundary (as RGB hex string or CSS color name)
+    :param line_width: Line width in pixels for the polygon boundary
+    :param fill_color: Color for the polygon interior (as RGB hex string or CSS color name)
+    :param fill_alpha: Opacity of the polygon as a float from 0 (transparent) to 1 (opaque)
+    :return: tuple containing the Bokeh ColumnDataSource and polygon glyphs (as Patch object)
+    """
+    x_coords, y_coords = list(zip(*[v for v in vertices]))
 
-        if sample_dict['compensation'] is not None:
-            comp_matrix = copy.deepcopy(sample_dict['compensation']['matrix'])
-        else:
-            comp_matrix = None
+    source = ColumnDataSource(dict(x=x_coords, y=y_coords))
 
-        return comp_matrix
+    poly = Patch(
+        x='x',
+        y='y',
+        fill_color=fill_color,
+        fill_alpha=fill_alpha,
+        line_width=line_width,
+        line_color=line_color
+    )
 
-    def get_transform(self, sample_id, transform_id):
-        """
-        Retrieve a single transform for a sample using the transform ID. Transform
-        IDs in the Workspace class correspond to a channel label in the sample.
-
-        :param sample_id: a text string representing a Sample instance
-        :param transform_id: a text string representing a Transform instance
-        :return:
-        """
-        sample_dict = self._sample_data_lut[sample_id]
+    return source, poly
 
-        if sample_dict['transforms'] is not None:
-            xform = copy.deepcopy(sample_dict['transforms'][transform_id])
-        else:
-            xform = None
 
-        return xform
+def render_ranges(dim_minimums, dim_maximums):
+    """
+    Renders Bokeh Span & BoxAnnotation objects for plotting simple range gates, essentially divider lines.
+    There should be no more than 3 items total between dim_minimums & dim_maximums, else the object should
+    be rendered as a rectangle.
+
+    :param dim_minimums: list of minimum divider values (max of 2)
+    :param dim_maximums: list of maximum divider values (max of 2)
+    :return: tuple of Span objects for every item in dim_minimums & dim_maximums
+    """
+    renderers = []
+    left = None
+    right = None
+    bottom = None
+    top = None
+
+    if dim_minimums[0] is not None:
+        left = dim_minimums[0]
+        renderers.append(
+            Span(location=left, dimension='height', line_width=LINE_WIDTH_DEFAULT, line_color=LINE_COLOR_DEFAULT)
+        )
+    if dim_maximums[0] is not None:
+        right = dim_maximums[0]
+        renderers.append(
+            Span(location=right, dimension='height', line_width=LINE_WIDTH_DEFAULT, line_color=LINE_COLOR_DEFAULT)
+        )
+    if len(dim_minimums) > 1:
+        if dim_minimums[1] is not None:
+            bottom = dim_minimums[1]
+            renderers.append(
+                Span(location=bottom, dimension='width', line_width=LINE_WIDTH_DEFAULT, line_color=LINE_COLOR_DEFAULT)
+            )
+        if dim_maximums[1] is not None:
+            top = dim_maximums[1]
+            renderers.append(
+                Span(location=top, dimension='width', line_width=LINE_WIDTH_DEFAULT, line_color=LINE_COLOR_DEFAULT)
+            )
 
-    def get_transforms(self, sample_id):
-        """
-        Retrieve the list of transformations for a specific sample.
+    mid_box = BoxAnnotation(
+        left=left,
+        right=right,
+        bottom=bottom,
+        top=top,
+        fill_alpha=FILL_ALPHA_DEFAULT,
+        fill_color=FILL_COLOR_DEFAULT
+    )
+    renderers.append(mid_box)
 
-        :param sample_id: a text string representing a Sample instance
-        :return: a list of Transform instances
-        """
-        sample_dict = self._sample_data_lut[sample_id]
+    return renderers
 
-        if sample_dict['transforms'] is not None:
-            xforms = copy.deepcopy(list(sample_dict['transforms'].values()))
-        else:
-            xforms = None
 
-        return xforms
+def render_rectangle(dim_minimums, dim_maximums):
+    """
+    Renders Bokeh Rect object for plotting a rectangle gate.
 
-    def get_gate(self, sample_id, gate_name, gate_path=None):
-        """
-        Retrieve a gate instance for a sample by its gate ID.
-
-        :param sample_id: a text string representing a Sample instance.
-        :param gate_name: text string of a gate ID
-        :param gate_path: tuple of gate IDs for unique set of gate ancestors. Required if gate_name is ambiguous
-        :return: Subclass of a Gate object
-        """
-        gs = self._sample_data_lut[sample_id]['gating_strategy']
-        return gs.get_gate(gate_name, gate_path=gate_path)
-
-    def analyze_samples(self, group_name=None, sample_id=None, cache_events=False, use_mp=True, verbose=False):
-        """
-        Process gates for samples. Samples to analyze can be filtered by group name or sample ID.
-        After running, results can be retrieved using the `get_gating_results`, `get_group_report`,
-        and  `get_gate_membership`, methods.
-
-        :param group_name: optional group name, if specified only samples in this group will be processed
-        :param sample_id: optional sample ID, if specified only this sample will be processed (overrides group filter)
-        :param cache_events: Whether to cache pre-processed events (compensated and transformed). This can
-            be useful to speed up processing of gates that share the same pre-processing instructions for
-            the same channel data, but can consume significantly more memory space. See the related
-            clear_cache method for additional information. Default is False.
-        :param use_mp: Controls whether multiprocessing is used to gate samples (default is True).
-            Multiprocessing can fail for large workloads (lots of samples & gates) due to running out of
-            memory. If encountering memory errors, set use_mp to False (processing will take longer,
-            but will use significantly less memory).
-        :param verbose: if True, print a line for every gate processed (default is False)
-        :return: None
-        """
-        # Don't save just the DataFrame report, save the entire
-        # GatingResults objects for each sample, since we'll need the gate
-        # indices for each sample.
-        if sample_id is not None:
-            sample_ids = [sample_id]
-        else:
-            # If group name is specified, get_sample_ids will return the
-            # group sample IDs. If not then it will return all sample IDs.
-            sample_ids = self.get_sample_ids(group_name=group_name)
-
-        if len(sample_ids) == 0:
-            warnings.warn("No samples were found to analyze")
-            return
-
-        sample_data_to_run = []
-        for s_id in sample_ids:
-            if s_id not in self._sample_data_lut:
-                # sample ID provided isn't present in Workspace
-                # or was referenced but has no gate data.
-                warnings.warn("Sample %s has no gate data" % s_id)
-                continue
-
-            sample = self._sample_lut[s_id]
-            gating_strategy = self._sample_data_lut[s_id]['gating_strategy']
-
-            sample_data_to_run.append(
-                {
-                    'gating_strategy': gating_strategy,
-                    'sample': sample
-                }
-            )
+    :param dim_minimums: list of 2 values representing the lower left corner of a rectangle
+    :param dim_maximums: list of 2 values representing the upper right corner of a rectangle
+    :return: Bokeh Rect object
+    """
+    x_center = (dim_minimums[0] + dim_maximums[0]) / 2.0
+    y_center = (dim_minimums[1] + dim_maximums[1]) / 2.0
+    x_width = dim_maximums[0] - dim_minimums[0]
+    y_height = dim_maximums[1] - dim_minimums[1]
+    rect = Rect(
+        x=x_center,
+        y=y_center,
+        width=x_width,
+        height=y_height,
+        fill_color=FILL_COLOR_DEFAULT,
+        fill_alpha=FILL_ALPHA_DEFAULT,
+        line_width=LINE_WIDTH_DEFAULT
+    )
 
-            # clear any existing results
-            if sample_id in self._results_lut:
-                del self._results_lut[sample_id]
-                gc.collect()
-
-        results = gating_utils.gate_samples(
-            sample_data_to_run,
-            cache_events,
-            verbose,
-            use_mp=False if debug else use_mp
-        )
-
-        # save the results in results LUT
-        for r in results:
-            self._results_lut[r.sample_id] = r
-
-    def get_gating_results(self, sample_id):
-        """
-        Retrieve analyzed gating results gates for a sample.
-
-        :param sample_id: a text string representing a Sample instance
-        :return: GatingResults instance
-        """
-        try:
-            gating_result = self._results_lut[sample_id]
-        except KeyError:
-            raise KeyError(
-                "No results found for %s. Have you run `analyze_samples`?" % sample_id
-            )
-        return copy.deepcopy(gating_result)
+    return rect
 
-    def get_analysis_report(self, group_name=None):
-        """
-        Retrieve the report for the analyzed samples as a pandas DataFrame.
-
-        :param group_name: optional group name, if specified only results
-            from samples in this group will be processed, otherwise results
-            from all analyzed samples will be returned
-        :return: pandas DataFrame
-        """
-        all_reports = []
-        group_s_ids = self.get_sample_ids(group_name)
 
-        for s_id in group_s_ids:
-            try:
-                result = self._results_lut[s_id]
-            except KeyError:
-                continue
-
-            all_reports.append(result.report)
-
-        return copy.deepcopy(pd.concat(all_reports))
-
-    def _get_processed_events(self, sample_id):
-        """
-        Retrieve a pandas DataFrame containing processed events for specified sample.
-        Compensation and transforms will be applied according to the WSP file.
-
-        :param sample_id: a text string representing a Sample instance
-        :return: pandas DataFrame containing the processed sample events
-        """
-        sample = self.get_sample(sample_id)
-        comp_matrix = self.get_comp_matrix(sample_id)
-        xforms = self.get_transforms(sample_id)
-
-        xform_lut = {xform.id: xform for xform in xforms if not xform.id.startswith('Comp')}
-
-        # default is 'raw' events
-        event_source = 'raw'
-
-        if comp_matrix is not None:
-            sample.apply_compensation(comp_matrix)
-            event_source = 'comp'
-        if xforms is not None:
-            sample.apply_transform(xform_lut)
-            event_source = 'xform'
-
-        events_df = sample.as_dataframe(source=event_source)
-
-        return events_df
-
-    def get_gate_membership(self, sample_id, gate_name, gate_path=None):
-        """
-        Retrieve a boolean array indicating gate membership for the events in the
-        specified sample. Note, the same gate ID may be found in multiple gate paths,
-        i.e. the gate ID can be ambiguous. In this case, specify the full gate path
-        to retrieve gate indices.
-
-        :param sample_id: a text string representing a Sample instance
-        :param gate_name: text string of a gate name
-        :param gate_path: complete tuple of gate IDs for unique set of gate ancestors.
-            Required if gate_name is ambiguous
-        :return: NumPy boolean array (length of sample event count)
-        """
-        gating_result = self.get_gating_results(sample_id)
-        return gating_result.get_gate_membership(gate_name, gate_path=gate_path)
-
-    def get_gate_events(self, sample_id, gate_name=None, gate_path=None):
-        """
-        Retrieve gated events for a specific gate & sample as a pandas DataFrame.
-        Gated events are processed according to the sample's compensation &
-        channel transforms.
-
-        :param sample_id: a text string representing a Sample instance
-        :param gate_name: text string of a gate ID. If None, all Sample events will be returned (i.e. un-gated)
-        :param gate_path: complete tuple of gate IDs for unique set of gate ancestors.
-            Required if gate_name is ambiguous
-        :return: a pandas DataFrames with the gated events, compensated & transformed according
-            to the group's compensation matrix and transforms
-        """
-        df_events = self._get_processed_events(sample_id)
-
-        if gate_name is not None:
-            gate_idx = self.get_gate_membership(sample_id, gate_name, gate_path)
-            df_events = df_events[gate_idx]
-
-        # TODO: maybe make an optional kwarg to control column label format
-        df_events.columns = [' '.join(col).strip() for col in df_events.columns]
-
-        df_events.insert(0, 'sample_id', sample_id)
-
-        return df_events
-
-    def plot_gate(
-            self,
-            sample_id,
-            gate_name,
-            gate_path=None,
-            subsample_count=10000,
-            random_seed=1,
-            x_min=None,
-            x_max=None,
-            y_min=None,
-            y_max=None,
-            color_density=True,
-            bin_width=4
-    ):
-        """
-        Returns an interactive plot for the specified gate. The type of plot is
-        determined by the number of dimensions used to define the gate: single
-        dimension gates will be histograms, 2-D gates will be returned as a
-        scatter plot.
-
-        :param sample_id: The sample ID for the FCS sample to plot
-        :param gate_name: Gate name to filter events (only events within the given gate will be plotted)
-        :param gate_path: tuple of gate names for full set of gate ancestors.
-            Required if gate_name is ambiguous
-        :param subsample_count: Number of events to use as a sub-sample. If the number of
-            events in the Sample is less than the requested sub-sample count, then the
-            maximum number of available events is used for the sub-sample.
-        :param random_seed: Random seed used for sub-sampling events
-        :param x_min: Lower bound of x-axis. If None, channel's min value will
-            be used with some padding to keep events off the edge of the plot.
-        :param x_max: Upper bound of x-axis. If None, channel's max value will
-            be used with some padding to keep events off the edge of the plot.
-        :param y_min: Lower bound of y-axis. If None, channel's min value will
-            be used with some padding to keep events off the edge of the plot.
-        :param y_max: Upper bound of y-axis. If None, channel's max value will
-            be used with some padding to keep events off the edge of the plot.
-        :param color_density: Whether to color the events by density, similar
-            to a heat map. Default is True.
-        :param bin_width: Bin size to use for the color density, in units of
-            event point size. Larger values produce smoother gradients.
-            Default is 4 for a 4x4 grid size.
-        :return: A Bokeh Figure object containing the interactive scatter plot.
-        """
-        if gate_path is None:
-            # verify the gate_name isn't ambiguous
-            gate_paths = self.find_matching_gate_paths(sample_id, gate_name)
-            if len(gate_paths) > 1:
-                raise GateReferenceError(
-                    "Multiple gates exist with gate name '%s'. Specify a gate_path to disambiguate." % gate_name
-                )
-            gate_path = gate_paths[0]
-
-        gate = self.get_gate(sample_id, gate_name, gate_path=gate_path)
-
-        # check for a boolean gate, there's no reasonable way to plot these
-        if isinstance(gate, gates.BooleanGate):
-            raise TypeError("Plotting Boolean gates is not allowed (gate %s)" % gate.gate_name)
-
-        parent_gate_name = gate_path[-1]
-        parent_gate_path = gate_path[:-1]
-
-        dim_ids_ordered = []
-        dim_is_ratio = []
-        dim_comp_refs = []
-        dim_min = []
-        dim_max = []
-        for i, dim in enumerate(gate.dimensions):
-            if isinstance(dim, dimension.RatioDimension):
-                dim_ids_ordered.append(dim.ratio_ref)
-                tmp_dim_min = dim.min
-                tmp_dim_max = dim.max
-                is_ratio = True
-            elif isinstance(dim, dimension.QuadrantDivider):
-                dim_ids_ordered.append(dim.dimension_ref)
-                tmp_dim_min = None
-                tmp_dim_max = None
-                is_ratio = False
-            else:
-                dim_ids_ordered.append(dim.id)
-                tmp_dim_min = dim.min
-                tmp_dim_max = dim.max
-                is_ratio = False
-
-            dim_min.append(tmp_dim_min)
-            dim_max.append(tmp_dim_max)
-            dim_is_ratio.append(is_ratio)
-            dim_comp_refs.append(dim.compensation_ref)
-
-        # dim count determines if we need a histogram, scatter, or multi-scatter
-        dim_count = len(dim_ids_ordered)
-        if dim_count == 1:
-            gate_type = 'hist'
-        elif dim_count == 2:
-            gate_type = 'scatter'
-        elif dim_count > 2:
-            raise NotImplementedError("Plotting of gates with >2 dimensions is not supported")
-        else:
-            # there are no dimensions
-            raise ValueError("Gate %s appears to not reference any dimensions" % gate_name)
+def render_dividers(x_locs, y_locs):
+    """
+    Renders lines for divider boundaries (2-D only)
+    :param x_locs: list of divider locations in x-axis
+    :param y_locs: list of divider locations in y-axis
+    :return: list of Bokeh renderer objects
+    """
+    renderers = []
 
-        # Get Sample instance and apply requested subsampling
-        sample_to_plot = self.get_sample(sample_id)
-        sample_to_plot.subsample_events(subsample_count=subsample_count, random_seed=random_seed)
-        gating_strategy = self.get_gating_strategy(sample_id)
-        # noinspection PyProtectedMember
-        events = gating_strategy._preprocess_sample_events(
-            sample_to_plot,
-            gate
-        )
-
-        # get parent gate results to display only those events
-        if parent_gate_name != 'root':
-            # TODO:  make it clear to call analyze_samples prior to calling this method
-            is_parent_event = self.get_gate_membership(sample_id, parent_gate_name, parent_gate_path)
-            is_subsample = np.zeros(sample_to_plot.event_count, dtype=bool)
-            is_subsample[sample_to_plot.subsample_indices] = True
-            idx_to_plot = np.logical_and(is_parent_event, is_subsample)
-        else:
-            idx_to_plot = sample_to_plot.subsample_indices
+    for x_loc in x_locs:
+        renderers.append(
+            Span(location=x_loc, dimension='height', line_width=LINE_WIDTH_DEFAULT, line_color=LINE_COLOR_DEFAULT)
+        )
+    for y_loc in y_locs:
+        renderers.append(
+            Span(location=y_loc, dimension='width', line_width=LINE_WIDTH_DEFAULT, line_color=LINE_COLOR_DEFAULT)
+        )
 
-        x = events.loc[idx_to_plot, dim_ids_ordered[0]].values
+    return renderers
 
-        dim_ids = []
 
-        if dim_is_ratio[0]:
-            dim_ids.append(dim_ids_ordered[0])
-            x_pnn_label = None
-        else:
-            try:
-                x_index = sample_to_plot.get_channel_index(dim_ids_ordered[0])
-            except ValueError:
-                # might be a label reference in the comp matrix
-                matrix = gating_strategy.get_comp_matrix(dim_comp_refs[0])
-                try:
-                    matrix_dim_idx = matrix.fluorochomes.index(dim_ids_ordered[0])
-                except ValueError:
-                    raise ValueError("%s not found in list of matrix fluorochromes" % dim_ids_ordered[0])
-                detector = matrix.detectors[matrix_dim_idx]
-                x_index = sample_to_plot.get_channel_index(detector)
+def render_ellipse(center_x, center_y, covariance_matrix, distance_square):
+    """
+    Renders a Bokeh Ellipse object given the ellipse center point, covariance, and distance square
 
-            x_pnn_label = sample_to_plot.pnn_labels[x_index]
+    :param center_x: x-coordinate of ellipse center
+    :param center_y: y-coordinate of ellipse center
+    :param covariance_matrix: NumPy array containing the covariance matrix of the ellipse
+    :param distance_square: value for distance square of ellipse
+    :return: Bokeh Ellipse object
+    """
+    values, vectors = np.linalg.eigh(covariance_matrix)
+    order = values.argsort()[::-1]
+    values = values[order]
+    vectors = vectors[:, order]
+
+    angle_rads = np.arctan2(*vectors[:, 0][::-1])
+
+    # Width and height are full width (the axes lengths are thus multiplied by 2.0 here)
+    width, height = 2.0 * np.sqrt(values * distance_square)
+
+    ellipse = Ellipse(
+        x=center_x,
+        y=center_y,
+        width=width,
+        height=height,
+        angle=angle_rads,
+        line_width=LINE_WIDTH_DEFAULT,
+        line_color=LINE_COLOR_DEFAULT,
+        fill_color=FILL_COLOR_DEFAULT,
+        fill_alpha=FILL_ALPHA_DEFAULT
+    )
 
-            if sample_to_plot.pns_labels[x_index] != '':
-                dim_ids.append('%s (%s)' % (sample_to_plot.pns_labels[x_index], x_pnn_label))
-            else:
-                dim_ids.append(sample_to_plot.pnn_labels[x_index])
+    return ellipse
 
-        y_pnn_label = None
 
-        if dim_count > 1:
-            if dim_is_ratio[1]:
-                dim_ids.append(dim_ids_ordered[1])
+def plot_histogram(x, x_label='x', bins=None):
+    """
+    Creates a Bokeh histogram plot of the given 1-D data array.
 
-            else:
-                try:
-                    y_index = sample_to_plot.get_channel_index(dim_ids_ordered[1])
-                except ValueError:
-                    # might be a label reference in the comp matrix
-                    matrix = gating_strategy.get_comp_matrix(dim_comp_refs[1])
-                    try:
-                        matrix_dim_idx = matrix.fluorochomes.index(dim_ids_ordered[1])
-                    except ValueError:
-                        raise ValueError("%s not found in list of matrix fluorochromes" % dim_ids_ordered[1])
-                    detector = matrix.detectors[matrix_dim_idx]
-                    y_index = sample_to_plot.get_channel_index(detector)
-
-                y_pnn_label = sample_to_plot.pnn_labels[y_index]
-
-                if sample_to_plot.pns_labels[y_index] != '':
-                    dim_ids.append('%s (%s)' % (sample_to_plot.pns_labels[y_index], y_pnn_label))
-                else:
-                    dim_ids.append(sample_to_plot.pnn_labels[y_index])
-
-        if gate_type == 'scatter':
-            y = events.loc[idx_to_plot, dim_ids_ordered[1]].values
-
-            p = plot_utils.plot_scatter(
-                x,
-                y,
-                dim_ids,
-                x_min=x_min,
-                x_max=x_max,
-                y_min=y_min,
-                y_max=y_max,
-                color_density=color_density,
-                bin_width=bin_width
-            )
-        elif gate_type == 'hist':
-            p = plot_utils.plot_histogram(x, dim_ids[0])
-        else:
-            raise NotImplementedError("Only histograms and scatter plots are supported in this version of FlowKit")
+    :param x: 1-D array of data values
+    :param x_label: Label to use for the x-axis
+    :param bins: Number of bins to use for the histogram or a string compatible
+            with the NumPy histogram function. If None, the number of bins is
+            determined by the square root rule.
+    :return: Bokeh Figure object containing the histogram
+    """
+    if bins is None:
+        bins = 'sqrt'
 
-        if isinstance(gate, gates.PolygonGate):
-            source, glyph = plot_utils.render_polygon(gate.vertices)
-            p.add_glyph(source, glyph)
-        elif isinstance(gate, gates.EllipsoidGate):
-            ellipse = plot_utils.render_ellipse(
-                gate.coordinates[0],
-                gate.coordinates[1],
-                gate.covariance_matrix,
-                gate.distance_square
-            )
-            p.add_glyph(ellipse)
-        elif isinstance(gate, gates.RectangleGate):
-            # rectangle gates in GatingML may not actually be rectangles, as the min/max for the dimensions
-            # are options. So, if any of the dim min/max values are missing it is essentially a set of ranges.
+    hist, edges = np.histogram(x, density=False, bins=bins)
 
-            if None in dim_min or None in dim_max or dim_count == 1:
-                renderers = plot_utils.render_ranges(dim_min, dim_max)
+    tools = "crosshair,hover,pan,zoom_in,zoom_out,box_zoom,undo,redo,reset,save,"
 
-                p.renderers.extend(renderers)
-            else:
-                # a true rectangle
-                rect = plot_utils.render_rectangle(dim_min, dim_max)
-                p.add_glyph(rect)
-        elif isinstance(gate, gates.QuadrantGate):
-            x_locations = []
-            y_locations = []
-
-            for div in gate.dimensions:
-                if div.dimension_ref == x_pnn_label:
-                    x_locations.extend(div.values)
-                elif div.dimension_ref == y_pnn_label and y_pnn_label is not None:
-                    y_locations.extend(div.values)
+    p = figure(tools=tools)
+    p.title.align = 'center'
+    p.quad(
+        top=hist,
+        bottom=0,
+        left=edges[:-1],
+        right=edges[1:],
+        alpha=0.5
+    )
+
+    p.y_range.start = 0
+    p.xaxis.axis_label = x_label
+    p.yaxis.axis_label = 'Event Count'
+
+    # set padding to match scatter plot
+    # scatter has 0.02, but we need to account for the bar width
+    # so doubling that looks about right
+    p.x_range.range_padding = 0.04
+
+    return p
+
+
+def plot_scatter(
+        x,
+        y,
+        x_label=None,
+        y_label=None,
+        event_mask=None,
+        highlight_mask=None,
+        x_min=None,
+        x_max=None,
+        y_min=None,
+        y_max=None,
+        color_density=True,
+        bin_width=4
+):
+    """
+    Creates a Bokeh scatter plot from the two 1-D data arrays.
 
-            renderers = plot_utils.render_dividers(x_locations, y_locations)
-            p.renderers.extend(renderers)
-        else:
-            raise NotImplementedError(
-                "Plotting of %s gates is not supported in this version of FlowKit" % gate.__class__
-            )
+    :param x: 1-D array of data values for the x-axis
+    :param y: 1-D array of data values for the y-axis
+    :param x_label: Label for the x-axis
+    :param y_label: Label for the y-axis
+    :param event_mask: Boolean array of events to plot. Takes precedence
+            over highlight_mask (i.e. events marked False in event_mask will
+            never be plotted).
+    :param highlight_mask: Boolean array of event indices to highlight
+        in color. Non-highlighted events will be light grey.
+    :param x_min: Lower bound of x-axis. If None, channel's min value will
+        be used with some padding to keep events off the edge of the plot.
+    :param x_max: Upper bound of x-axis. If None, channel's max value will
+        be used with some padding to keep events off the edge of the plot.
+    :param y_min: Lower bound of y-axis. If None, channel's min value will
+        be used with some padding to keep events off the edge of the plot.
+    :param y_max: Upper bound of y-axis. If None, channel's max value will
+        be used with some padding to keep events off the edge of the plot.
+    :param color_density: Whether to color the events by density, similar
+        to a heat map. Default is True.
+    :param bin_width: Bin size to use for the color density, in units of
+        event point size. Larger values produce smoother gradients.
+        Default is 4 for a 4x4 grid size.
+    :return: A Bokeh Figure object containing the interactive scatter plot.
+    """
+    # before anything, check for event_mask
+    if event_mask is not None:
+        # filter x & y
+        x = x[event_mask]
+        y = y[event_mask]
+
+        # sync highlight_mask if given
+        if highlight_mask is not None:
+            highlight_mask = highlight_mask[event_mask]
+
+    if len(x) > 0:
+        x_min, x_max = _calculate_extent(x, d_min=x_min, d_max=x_max, pad=0.02)
+    if len(y) > 0:
+        y_min, y_max = _calculate_extent(y, d_min=y_min, d_max=y_max, pad=0.02)
+
+    if y_max > x_max:
+        radius_dimension = 'y'
+        radius = 0.003 * y_max
+    else:
+        radius_dimension = 'x'
+        radius = 0.003 * x_max
+
+    if color_density:
+        # bin size set to cover NxN radius (radius size is percent of view)
+        # can be set by user via bin_width kwarg
+        bin_count = int(1 / (bin_width * 0.003))
+
+        # But that's just the bins needed for the requested plot ranges.
+        # We need to extend those bins to the full data range
+        x_view_range = x_max - x_min
+        y_view_range = y_max - y_min
+
+        x_data_min = np.min(x)
+        x_data_max = np.max(x)
+        y_data_min = np.min(y)
+        y_data_max = np.max(y)
+        x_data_range = x_data_max - x_data_min
+        y_data_range = y_data_max - y_data_min
+
+        x_bin_multiplier = x_data_range / x_view_range
+        x_bin_count = int(x_bin_multiplier * bin_count)
+        y_bin_multiplier = y_data_range / y_view_range
+        y_bin_count = int(y_bin_multiplier * bin_count)
+
+        # avoid bin count of zero
+        if x_bin_count <= 0:
+            x_bin_count = 1
+        if y_bin_count <= 0:
+            y_bin_count = 1
+
+        cd_x_min = x_data_min - (x_data_range / x_bin_count)
+        cd_x_max = x_data_max + (x_data_range / x_bin_count)
+        cd_y_min = y_data_min - (y_data_range / y_bin_count)
+        cd_y_max = y_data_max + (y_data_range / y_bin_count)
 
-        if gate_path is not None:
-            full_gate_path = gate_path[1:]  # omit 'root'
-            full_gate_path = full_gate_path + (gate_name,)
-            sub_title = ' > '.join(full_gate_path)
-
-            # truncate beginning of long gate paths
-            if len(sub_title) > 72:
-                sub_title = '...' + sub_title[-69:]
-            p.add_layout(
-                Title(text=sub_title, text_font_style="italic", text_font_size="1em", align='center'),
-                'above'
-            )
-        else:
-            p.add_layout(
-                Title(text=gate_name, text_font_style="italic", text_font_size="1em", align='center'),
-                'above'
-            )
+        # noinspection PyTypeChecker
+        hist_data, x_edges, y_edges = np.histogram2d(
+            x,
+            y,
+            bins=[x_bin_count, y_bin_count],
+            range=[[cd_x_min, cd_x_max], [cd_y_min, cd_y_max]]
+        )
+        z = interpn(
+            (0.5 * (x_edges[1:] + x_edges[:-1]), 0.5 * (y_edges[1:] + y_edges[:-1])),
+            hist_data,
+            np.vstack([x, y]).T,
+            method="linear",  # use linear not spline, spline tends to overshoot into negative values
+            bounds_error=False
+        )
+        z[np.isnan(z)] = 0
 
-        plot_title = "%s" % sample_id
-        p.add_layout(
-            Title(text=plot_title, text_font_size="1.1em", align='center'),
-            'above'
+        # sort by density (z) so the more dense points are on top for better
+        # color display
+        idx = z.argsort()
+        x, y, z = x[idx], y[idx], z[idx]
+        if highlight_mask is not None:
+            # re-order the highlight indices to match
+            highlight_mask = highlight_mask[idx]
+
+        z_norm = (z - z.min()) / (z.max() - z.min())
+    else:
+        z_norm = np.zeros(len(x))
+
+    z_colors = np.array([custom_heat_palette[int(z * 255)] for z in z_norm])
+
+    if highlight_mask is not None:
+        z_colors[~highlight_mask] = "#d3d3d3"
+        fill_alpha = np.zeros(len(z_colors))
+        fill_alpha[~highlight_mask] = 0.3
+        fill_alpha[highlight_mask] = 0.4
+
+        highlight_idx = np.flatnonzero(highlight_mask)
+        non_light_idx = np.flatnonzero(~highlight_mask)
+        final_idx = np.concatenate([non_light_idx, highlight_idx])
+
+        x = x[final_idx]
+        y = y[final_idx]
+        z_colors = z_colors[final_idx]
+        fill_alpha = fill_alpha[final_idx]
+    else:
+        fill_alpha = 0.4
+
+    tools = "crosshair,hover,pan,zoom_in,zoom_out,box_zoom,undo,redo,reset,save,"
+    p = figure(
+        tools=tools,
+        x_range=(x_min, x_max),
+        y_range=(y_min, y_max)
+    )
+
+    p.xaxis.axis_label = x_label
+    p.yaxis.axis_label = y_label
+
+    p.circle(
+        x,
+        y,
+        radius=radius,
+        radius_dimension=radius_dimension,
+        fill_color=z_colors,
+        fill_alpha=fill_alpha,
+        line_color=None
+    )
+
+    return p
+
+
+def plot_contours(
+        x,
+        y,
+        x_label=None,
+        y_label=None,
+        x_min=None,
+        x_max=None,
+        y_min=None,
+        y_max=None,
+        plot_events=False,
+        fill=False
+):
+    """
+    Create a Bokeh plot of contours from the two 1-D data arrays.
+
+    :param x: 1-D array of data values for the x-axis
+    :param y: 1-D array of data values for the y-axis
+    :param x_label: Label for the x-axis
+    :param y_label: Label for the y-axis
+    :param x_min: Lower bound of x-axis. If None, channel's min value will
+        be used with some padding to keep events off the edge of the plot.
+    :param x_max: Upper bound of x-axis. If None, channel's max value will
+        be used with some padding to keep events off the edge of the plot.
+    :param y_min: Lower bound of y-axis. If None, channel's min value will
+        be used with some padding to keep events off the edge of the plot.
+    :param y_max: Upper bound of y-axis. If None, channel's max value will
+        be used with some padding to keep events off the edge of the plot.
+    :param plot_events: Whether to plot the events as a scatter plot in
+        addition to the contours.
+    :param fill: Whether to color fill contours by density, similar
+        to a heat map. Default is False.
+    :return: A Bokeh Figure object containing the interactive scatter plot.
+    """
+    # Calculate Gaussian KDE, using default bandwidth & grid size (maybe expose these later?)
+    mesh_x, mesh_y, est_pdf = _calculate_2d_gaussian_kde(x, y)
+
+    # Get contour generator from our PDF on our grid
+    c_gen = _build_contour_generator(mesh_x, mesh_y, est_pdf)
+
+    # Generate a modest set of quantiles to plot (not too many as it gets crowded easily).
+    # And, don't start at 0 (there's not really a contour there).
+    quantiles = list(np.linspace(0.04, 1, 9).round(2))
+
+    # Convert quantiles to corresponding levels in our PDF
+    levels = _quantiles_to_levels(est_pdf, quantiles)
+
+    # Unless user set them, set our axis bounds based on contour bounds
+    # instead of the data ranges b/c the contours can be wider.
+    if x_min is None:
+        x_min = mesh_x.min()
+    if x_max is None:
+        x_max = mesh_x.max()
+    if y_min is None:
+        y_min = mesh_y.min()
+    if y_max is None:
+        y_max = mesh_y.max()
+
+    # if we are plotting events, get the Bokeh figure from plot_scatter,
+    # else we'll make a new one
+    if plot_events:
+        fig = plot_scatter(
+            x, y,
+            x_label=x_label, y_label=y_label,
+            x_min=x_min, x_max=x_max,
+            y_min=y_min, y_max=y_max
+        )
+    else:
+        tools = "crosshair,hover,pan,zoom_in,zoom_out,box_zoom,undo,redo,reset,save,"
+        fig = figure(
+            tools=tools,
+            x_range=(x_min, x_max),
+            y_range=(y_min, y_max)
         )
 
-        return p
+        fig.xaxis.axis_label = x_label
+        fig.yaxis.axis_label = y_label
 
-    def plot_scatter(
-            self,
-            sample_id,
-            x_label,
-            y_label,
-            gate_name=None,
-            subsample_count=10000,
-            random_seed=1,
-            color_density=True,
-            bin_width=4,
-            x_min=None,
-            x_max=None,
-            y_min=None,
-            y_max=None
-    ):
-        """
-        Returns an interactive scatter plot for the specified channel data.
-
-        :param sample_id: The sample ID for the FCS sample to plot
-        :param x_label: channel label (PnN) to use for the x-axis data
-        :param y_label: channel label (PnN) to use for the y-axis data
-        :param gate_name: Gate name to filter events (only events within the given gate will be plotted)
-        :param subsample_count: Number of events to use as a sub-sample. If the number of
-            events in the Sample is less than the requested sub-sample count, then the
-            maximum number of available events is used for the sub-sample.
-        :param random_seed: Random seed used for sub-sampling events
-        :param color_density: Whether to color the events by density, similar
-            to a heat map. Default is True.
-        :param bin_width: Bin size to use for the color density, in units of
-            event point size. Larger values produce smoother gradients.
-            Default is 4 for a 4x4 grid size.
-        :param x_min: Lower bound of x-axis. If None, channel's min value will
-            be used with some padding to keep events off the edge of the plot.
-        :param x_max: Upper bound of x-axis. If None, channel's max value will
-            be used with some padding to keep events off the edge of the plot.
-        :param y_min: Lower bound of y-axis. If None, channel's min value will
-            be used with some padding to keep events off the edge of the plot.
-        :param y_max: Upper bound of y-axis. If None, channel's max value will
-            be used with some padding to keep events off the edge of the plot.
-        :return: A Bokeh Figure object containing the interactive scatter plot.
-        """
-        # Get Sample instance and apply requested subsampling
-        sample = self.get_sample(sample_id)
-        sample.subsample_events(subsample_count=subsample_count, random_seed=random_seed)
-
-        # Build Dimension instances for the requested x & y labels from
-        # the dedicated comp matrix & transform set for this sample.
-        comp_matrix = self.get_comp_matrix(sample_id)
-        x_xform = self.get_transform(sample_id, x_label)
-        y_xform = self.get_transform(sample_id, y_label)
-
-        x_index = sample.get_channel_index(x_label)
-        y_index = sample.get_channel_index(y_label)
-
-        if comp_matrix is not None:
-            comp_events = comp_matrix.apply(sample)
-            x = comp_events[:, x_index]
-            y = comp_events[:, y_index]
-        else:
-            # not doing sub-sample here, will do later with bool AND
-            x = sample.get_channel_events(x_index, source='raw', subsample=False)
-            y = sample.get_channel_events(y_index, source='raw', subsample=False)
-
-        if x_xform is not None:
-            x = x_xform.apply(x)
-        if y_xform is not None:
-            y = y_xform.apply(y)
-
-        if gate_name is not None:
-            gate_results = self.get_gating_results(sample_id=sample_id)
-            is_gate_event = gate_results.get_gate_membership(gate_name)
-        else:
-            is_gate_event = np.ones(sample.event_count, dtype=bool)
+    # Add the sets of contours as polygons to the figure
+    for i, level in enumerate(levels):
+        poly_lines = c_gen.lines(level)
+
+        if fill:
+            fill_color = custom_heat_palette[int(quantiles[i] * 255)]
+            fill_alpha = min(quantiles[i] * 2, 1)
+            line_color = None
+        else:
+            fill_color = None
+            fill_alpha = 0
+            line_color = LINE_COLOR_DEFAULT
+
+        for poly in poly_lines:
+            source, glyph = render_polygon(
+                poly, line_color=line_color, fill_color=fill_color, fill_alpha=fill_alpha
+            )
+            fig.add_glyph(source, glyph)
 
-        is_subsample = np.zeros(sample.event_count, dtype=bool)
-        is_subsample[sample.subsample_indices] = True
+    return fig
 
-        idx_to_plot = np.logical_and(is_gate_event, is_subsample)
 
-        # check if there are any events to plot
-        if idx_to_plot.sum() == 0:
-            raise FlowKitException("There are no events to plot for the specified options")
+def plot_gate(
+        gate_id,
+        gating_strategy: GatingStrategy,
+        sample,
+        subsample_count=10000,
+        random_seed=1,
+        event_mask=None,
+        x_min=None,
+        x_max=None,
+        y_min=None,
+        y_max=None,
+        color_density=True,
+        bin_width=4
+):
+    """
+    Returns an interactive plot for the specified gate. The type of plot is
+    determined by the number of dimensions used to define the gate: single
+    dimension gates will be histograms, 2-D gates will be returned as a
+    scatter plot.
+
+    :param gate_id: tuple of gate name and gate path (also a tuple)
+    :param gating_strategy: GatingStrategy containing gate_id
+    :param sample: Sample instance to plot
+    :param subsample_count: Number of events to use as a sub-sample. If the number of
+        events in the Sample is less than the requested sub-sample count, then the
+        maximum number of available events is used for the sub-sample.
+    :param random_seed: Random seed used for sub-sampling events
+    :param event_mask: Boolean array of events to plot (i.e. parent gate event membership)
+    :param x_min: Lower bound of x-axis. If None, channel's min value will
+        be used with some padding to keep events off the edge of the plot.
+    :param x_max: Upper bound of x-axis. If None, channel's max value will
+        be used with some padding to keep events off the edge of the plot.
+    :param y_min: Lower bound of y-axis. If None, channel's min value will
+        be used with some padding to keep events off the edge of the plot.
+    :param y_max: Upper bound of y-axis. If None, channel's max value will
+        be used with some padding to keep events off the edge of the plot.
+    :param color_density: Whether to color the events by density, similar
+        to a heat map. Default is True.
+    :param bin_width: Bin size to use for the color density, in units of
+        event point size. Larger values produce smoother gradients.
+        Default is 4 for a 4x4 grid size.
+    :return: A Bokeh Figure object containing the interactive scatter plot.
+    """
+    (gate_name, gate_path) = gate_id
+    sample_id = sample.id
+    gate = gating_strategy.get_gate(gate_name, gate_path=gate_path, sample_id=sample_id)
+
+    # check for a boolean gate, there's no reasonable way to plot these
+    if isinstance(gate, gates.BooleanGate):
+        raise TypeError("Plotting Boolean gates is not allowed (gate %s)" % gate.gate_name)
+
+    dim_ids_ordered = []
+    dim_is_ratio = []
+    dim_comp_refs = []
+    dim_min = []
+    dim_max = []
+    for i, dim in enumerate(gate.dimensions):
+        if isinstance(dim, dimension.RatioDimension):
+            dim_ids_ordered.append(dim.ratio_ref)
+            tmp_dim_min = dim.min
+            tmp_dim_max = dim.max
+            is_ratio = True
+        elif isinstance(dim, dimension.QuadrantDivider):
+            dim_ids_ordered.append(dim.dimension_ref)
+            tmp_dim_min = None
+            tmp_dim_max = None
+            is_ratio = False
+        else:
+            dim_ids_ordered.append(dim.id)
+            tmp_dim_min = dim.min
+            tmp_dim_max = dim.max
+            is_ratio = False
+
+        dim_min.append(tmp_dim_min)
+        dim_max.append(tmp_dim_max)
+        dim_is_ratio.append(is_ratio)
+        dim_comp_refs.append(dim.compensation_ref)
+
+    # dim count determines if we need a histogram, scatter, or multi-scatter
+    dim_count = len(dim_ids_ordered)
+    if dim_count == 1:
+        gate_type = 'hist'
+    elif dim_count == 2:
+        gate_type = 'scatter'
+    elif dim_count > 2:
+        raise NotImplementedError("Plotting of gates with >2 dimensions is not supported")
+    else:
+        # there are no dimensions
+        raise ValueError("Gate %s appears to not reference any dimensions" % gate_name)
+
+    # Apply requested subsampling
+    sample.subsample_events(subsample_count=subsample_count, random_seed=random_seed)
+    # noinspection PyProtectedMember
+    events = gating_strategy._preprocess_sample_events(
+        sample,
+        gate
+    )
 
-        x = x[idx_to_plot]
-        y = y[idx_to_plot]
+    # Use event mask, if given
+    if event_mask is not None:
+        is_subsample = np.zeros(sample.event_count, dtype=bool)
+        is_subsample[sample.subsample_indices] = True
+        idx_to_plot = np.logical_and(event_mask, is_subsample)
+    else:
+        idx_to_plot = sample.subsample_indices
+
+    x = events.loc[idx_to_plot, dim_ids_ordered[0]].values
+
+    dim_ids = []
+
+    if dim_is_ratio[0]:
+        dim_ids.append(dim_ids_ordered[0])
+        x_pnn_label = None
+    else:
+        try:
+            x_index = sample.get_channel_index(dim_ids_ordered[0])
+        except ValueError:
+            # might be a label reference in the comp matrix
+            matrix = gating_strategy.get_comp_matrix(dim_comp_refs[0])
+            try:
+                matrix_dim_idx = matrix.fluorochomes.index(dim_ids_ordered[0])
+            except ValueError:
+                raise ValueError("%s not found in list of matrix fluorochromes" % dim_ids_ordered[0])
+            detector = matrix.detectors[matrix_dim_idx]
+            x_index = sample.get_channel_index(detector)
 
-        dim_ids = []
+        x_pnn_label = sample.pnn_labels[x_index]
 
         if sample.pns_labels[x_index] != '':
-            dim_ids.append('%s (%s)' % (sample.pns_labels[x_index], sample.pnn_labels[x_index]))
+            dim_ids.append('%s (%s)' % (sample.pns_labels[x_index], x_pnn_label))
         else:
             dim_ids.append(sample.pnn_labels[x_index])
 
-        if sample.pns_labels[y_index] != '':
-            dim_ids.append('%s (%s)' % (sample.pns_labels[y_index], sample.pnn_labels[y_index]))
+    y_pnn_label = None
+
+    if dim_count > 1:
+        if dim_is_ratio[1]:
+            dim_ids.append(dim_ids_ordered[1])
+
         else:
-            dim_ids.append(sample.pnn_labels[y_index])
+            try:
+                y_index = sample.get_channel_index(dim_ids_ordered[1])
+            except ValueError:
+                # might be a label reference in the comp matrix
+                matrix = gating_strategy.get_comp_matrix(dim_comp_refs[1])
+                try:
+                    matrix_dim_idx = matrix.fluorochomes.index(dim_ids_ordered[1])
+                except ValueError:
+                    raise ValueError("%s not found in list of matrix fluorochromes" % dim_ids_ordered[1])
+                detector = matrix.detectors[matrix_dim_idx]
+                y_index = sample.get_channel_index(detector)
+
+            y_pnn_label = sample.pnn_labels[y_index]
+
+            if sample.pns_labels[y_index] != '':
+                dim_ids.append('%s (%s)' % (sample.pns_labels[y_index], y_pnn_label))
+            else:
+                dim_ids.append(sample.pnn_labels[y_index])
+
+    if gate_type == 'scatter':
+        y = events.loc[idx_to_plot, dim_ids_ordered[1]].values
 
-        p = plot_utils.plot_scatter(
+        p = plot_scatter(
             x,
             y,
-            dim_ids,
+            x_label=dim_ids[0],
+            y_label=dim_ids[1],
             x_min=x_min,
             x_max=x_max,
             y_min=y_min,
             y_max=y_max,
             color_density=color_density,
             bin_width=bin_width
         )
+    elif gate_type == 'hist':
+        p = plot_histogram(x, dim_ids[0])
+    else:
+        raise NotImplementedError("Only histograms and scatter plots are supported in this version of FlowKit")
+
+    if isinstance(gate, gates.PolygonGate):
+        source, glyph = render_polygon(gate.vertices)
+        p.add_glyph(source, glyph)
+    elif isinstance(gate, gates.EllipsoidGate):
+        ellipse = render_ellipse(
+            gate.coordinates[0],
+            gate.coordinates[1],
+            gate.covariance_matrix,
+            gate.distance_square
+        )
+        p.add_glyph(ellipse)
+    elif isinstance(gate, gates.RectangleGate):
+        # rectangle gates in GatingML may not actually be rectangles, as the min/max for the dimensions
+        # are options. So, if any of the dim min/max values are missing it is essentially a set of ranges.
+
+        if None in dim_min or None in dim_max or dim_count == 1:
+            renderers = render_ranges(dim_min, dim_max)
+
+            p.renderers.extend(renderers)
+        else:
+            # a true rectangle
+            rect = render_rectangle(dim_min, dim_max)
+            p.add_glyph(rect)
+    elif isinstance(gate, gates.QuadrantGate):
+        x_locations = []
+        y_locations = []
+
+        for div in gate.dimensions:
+            if div.dimension_ref == x_pnn_label:
+                x_locations.extend(div.values)
+            elif div.dimension_ref == y_pnn_label and y_pnn_label is not None:
+                y_locations.extend(div.values)
+
+        renderers = render_dividers(x_locations, y_locations)
+        p.renderers.extend(renderers)
+    else:
+        raise NotImplementedError(
+            "Plotting of %s gates is not supported in this version of FlowKit" % gate.__class__
+        )
+
+    if gate_path is not None:
+        full_gate_path = gate_path[1:]  # omit 'root'
+        full_gate_path = full_gate_path + (gate_name,)
+        sub_title = ' > '.join(full_gate_path)
+
+        # truncate beginning of long gate paths
+        if len(sub_title) > 72:
+            sub_title = '...' + sub_title[-69:]
+        p.add_layout(
+            Title(text=sub_title, text_font_style="italic", text_font_size="1em", align='center'),
+            'above'
+        )
+    else:
+        p.add_layout(
+            Title(text=gate_name, text_font_style="italic", text_font_size="1em", align='center'),
+            'above'
+        )
 
-        p.title = Title(text=sample.id, align='center')
+    plot_title = "%s" % sample_id
+    p.add_layout(
+        Title(text=plot_title, text_font_size="1.1em", align='center'),
+        'above'
+    )
 
-        return p
+    return p
```

### Comparing `FlowKit-1.0.1/flowkit/_resources/DataTypes.v2.0.xsd` & `FlowKit-1.1.0/src/flowkit/_resources/DataTypes.v2.0.xsd`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text, with CRLF line terminators*

 * *Files 22% similar despite different names*

```diff
@@ -1,310 +1,303 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
-00000020: 462d 3822 3f3e 0d0a 0d0a 3c73 6368 656d  F-8"?>....<schem
-00000030: 6120 786d 6c6e 733d 2268 7474 703a 2f2f  a xmlns="http://
-00000040: 7777 772e 7733 2e6f 7267 2f32 3030 312f  www.w3.org/2001/
-00000050: 584d 4c53 6368 656d 6122 0d0a 2020 2020  XMLSchema"..    
-00000060: 786d 6c6e 733a 6461 7461 2d74 7970 653d  xmlns:data-type=
-00000070: 2268 7474 703a 2f2f 7777 772e 6973 6163  "http://www.isac
-00000080: 2d6e 6574 2e6f 7267 2f73 7464 2f47 6174  -net.org/std/Gat
-00000090: 696e 672d 4d4c 2f76 322e 302f 6461 7461  ing-ML/v2.0/data
-000000a0: 7479 7065 7322 0d0a 2020 2020 786d 6c6e  types"..    xmln
-000000b0: 733a 7472 616e 7366 6f72 6d73 3d22 6874  s:transforms="ht
-000000c0: 7470 3a2f 2f77 7777 2e69 7361 632d 6e65  tp://www.isac-ne
-000000d0: 742e 6f72 672f 7374 642f 4761 7469 6e67  t.org/std/Gating
-000000e0: 2d4d 4c2f 7632 2e30 2f74 7261 6e73 666f  -ML/v2.0/transfo
-000000f0: 726d 6174 696f 6e73 220d 0a20 2020 2074  rmations"..    t
-00000100: 6172 6765 744e 616d 6573 7061 6365 3d22  argetNamespace="
-00000110: 6874 7470 3a2f 2f77 7777 2e69 7361 632d  http://www.isac-
-00000120: 6e65 742e 6f72 672f 7374 642f 4761 7469  net.org/std/Gati
-00000130: 6e67 2d4d 4c2f 7632 2e30 2f64 6174 6174  ng-ML/v2.0/datat
-00000140: 7970 6573 220d 0a20 2020 2065 6c65 6d65  ypes"..    eleme
-00000150: 6e74 466f 726d 4465 6661 756c 743d 2271  ntFormDefault="q
-00000160: 7561 6c69 6669 6564 2220 6174 7472 6962  ualified" attrib
-00000170: 7574 6546 6f72 6d44 6566 6175 6c74 3d22  uteFormDefault="
-00000180: 7175 616c 6966 6965 6422 2076 6572 7369  qualified" versi
-00000190: 6f6e 3d22 322e 302e 3132 3132 3037 223e  on="2.0.121207">
-000001a0: 0d0a 0d0a 2020 2020 3c61 6e6e 6f74 6174  ....    <annotat
-000001b0: 696f 6e3e 0d0a 2020 2020 2020 2020 3c61  ion>..        <a
-000001c0: 7070 696e 666f 2073 6f75 7263 653d 2268  ppinfo source="h
-000001d0: 7474 703a 2f2f 666c 6f77 6379 742e 736f  ttp://flowcyt.so
-000001e0: 7572 6365 666f 7267 652e 6e65 742f 223e  urceforge.net/">
-000001f0: 4465 6669 6e69 7469 6f6e 206f 6620 6461  Definition of da
-00000200: 7461 2074 7970 6573 2072 6575 7365 6420  ta types reused 
-00000210: 696e 2058 4d4c 2d62 6173 6564 2073 7461  in XML-based sta
-00000220: 6e64 6172 6473 2073 7563 6820 6173 2047  ndards such as G
-00000230: 6174 696e 672d 4d4c 2058 4d4c 2073 6368  ating-ML XML sch
-00000240: 656d 612e 3c2f 6170 7069 6e66 6f3e 0d0a  ema.</appinfo>..
-00000250: 2020 2020 2020 2020 3c64 6f63 756d 656e          <documen
-00000260: 7461 7469 6f6e 2078 6d6c 3a6c 616e 673d  tation xml:lang=
-00000270: 2265 6e22 2073 6f75 7263 653d 2268 7474  "en" source="htt
-00000280: 703a 2f2f 666c 6f77 6379 742e 736f 7572  p://flowcyt.sour
-00000290: 6365 666f 7267 652e 6e65 742f 223e 0d0a  ceforge.net/">..
-000002a0: 2020 2020 2020 2020 2020 2020 3c61 7574              <aut
-000002b0: 686f 723e 0d0a 2020 2020 2020 2020 2020  hor>..          
-000002c0: 2020 2020 2020 3c6e 616d 653e 4a6f 7365        <name>Jose
-000002d0: 6620 5370 6964 6c65 6e3c 2f6e 616d 653e  f Spidlen</name>
-000002e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000002f0: 2020 3c65 6d61 696c 3e6a 7370 6964 6c65    <email>jspidle
-00000300: 6e40 6263 6372 632e 6361 3c2f 656d 6169  n@bccrc.ca</emai
-00000310: 6c3e 0d0a 2020 2020 2020 2020 2020 2020  l>..            
-00000320: 3c2f 6175 7468 6f72 3e0d 0a20 2020 2020  </author>..     
-00000330: 2020 2020 2020 203c 636f 7079 7269 6768         <copyrigh
-00000340: 743e 0d0a 2020 2020 2020 2020 2020 2020  t>..            
-00000350: 2020 2020 436f 7079 7269 6768 7420 2863      Copyright (c
-00000360: 2920 3230 3038 2d32 3031 3420 4953 4143  ) 2008-2014 ISAC
-00000370: 2028 496e 7465 726e 6174 696f 6e61 6c20   (International 
-00000380: 536f 6369 6574 7920 666f 7220 4164 7661  Society for Adva
-00000390: 6e63 656d 656e 7420 6f66 0d0a 2020 2020  ncement of..    
-000003a0: 2020 2020 2020 2020 2020 2020 4379 746f              Cyto
-000003b0: 6d65 7472 7929 2e20 4672 6565 206f 6620  metry). Free of 
-000003c0: 6368 6172 6765 2064 6973 7472 6962 7574  charge distribut
-000003d0: 696f 6e20 616e 6420 7265 6164 2d6f 6e6c  ion and read-onl
-000003e0: 7920 7573 6167 6520 7065 726d 6974 6564  y usage permited
-000003f0: 2e20 4d6f 6469 6669 6361 7469 6f6e 0d0a  . Modification..
-00000400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000410: 616e 6420 616c 6c20 6f74 6865 7220 7269  and all other ri
-00000420: 6768 7473 2072 6573 6572 7665 642e 2046  ghts reserved. F
-00000430: 6f72 2061 6c6c 206f 7468 6572 2075 7365  or all other use
-00000440: 7320 706c 6561 7365 2063 6f6e 7461 6374  s please contact
-00000450: 2049 5341 432e 0d0a 2020 2020 2020 2020   ISAC...        
-00000460: 2020 2020 3c2f 636f 7079 7269 6768 743e      </copyright>
-00000470: 0d0a 2020 2020 2020 2020 3c2f 646f 6375  ..        </docu
-00000480: 6d65 6e74 6174 696f 6e3e 0d0a 2020 2020  mentation>..    
-00000490: 3c2f 616e 6e6f 7461 7469 6f6e 3e0d 0a0d  </annotation>...
-000004a0: 0a20 2020 203c 7369 6d70 6c65 5479 7065  .    <simpleType
-000004b0: 206e 616d 653d 2255 466c 6f61 7436 345f   name="UFloat64_
-000004c0: 5479 7065 223e 0d0a 2020 2020 2020 2020  Type">..        
-000004d0: 3c61 6e6e 6f74 6174 696f 6e3e 0d0a 2020  <annotation>..  
-000004e0: 2020 2020 2020 2020 2020 3c64 6f63 756d            <docum
-000004f0: 656e 7461 7469 6f6e 2078 6d6c 3a6c 616e  entation xml:lan
-00000500: 673d 2265 6e22 3e55 6e73 6967 6e65 6420  g="en">Unsigned 
-00000510: 666c 6f61 7436 342c 2069 2e65 2c20 6120  float64, i.e, a 
-00000520: 646f 7562 6c65 2028 666c 6f61 7436 3429  double (float64)
-00000530: 2074 6861 7420 6973 2067 7265 6174 6572   that is greater
-00000540: 206f 7220 6571 7561 6c20 302e 3c2f 646f   or equal 0.</do
-00000550: 6375 6d65 6e74 6174 696f 6e3e 0d0a 2020  cumentation>..  
-00000560: 2020 2020 2020 3c2f 616e 6e6f 7461 7469        </annotati
-00000570: 6f6e 3e0d 0a20 2020 2020 2020 203c 7265  on>..        <re
-00000580: 7374 7269 6374 696f 6e20 6261 7365 3d22  striction base="
-00000590: 646f 7562 6c65 223e 0d0a 2020 2020 2020  double">..      
-000005a0: 2020 2020 2020 3c6d 696e 496e 636c 7573        <minInclus
-000005b0: 6976 6520 7661 6c75 653d 2230 2e30 2220  ive value="0.0" 
-000005c0: 2f3e 0d0a 2020 2020 2020 2020 3c2f 7265  />..        </re
-000005d0: 7374 7269 6374 696f 6e3e 0d0a 2020 2020  striction>..    
-000005e0: 3c2f 7369 6d70 6c65 5479 7065 3e0d 0a0d  </simpleType>...
-000005f0: 0a20 2020 203c 7369 6d70 6c65 5479 7065  .    <simpleType
-00000600: 206e 616d 653d 2250 466c 6f61 7436 345f   name="PFloat64_
-00000610: 5479 7065 223e 0d0a 2020 2020 2020 2020  Type">..        
-00000620: 3c61 6e6e 6f74 6174 696f 6e3e 0d0a 2020  <annotation>..  
-00000630: 2020 2020 2020 2020 2020 3c64 6f63 756d            <docum
-00000640: 656e 7461 7469 6f6e 2078 6d6c 3a6c 616e  entation xml:lan
-00000650: 673d 2265 6e22 3e50 6f73 6974 6976 6520  g="en">Positive 
-00000660: 666c 6f61 7436 342c 2069 2e65 2e2c 2061  float64, i.e., a
-00000670: 2064 6f75 626c 6520 2866 6c6f 6174 3634   double (float64
-00000680: 2920 7468 6174 2069 7320 6772 6561 7465  ) that is greate
-00000690: 7220 7468 616e 2030 2e3c 2f64 6f63 756d  r than 0.</docum
-000006a0: 656e 7461 7469 6f6e 3e0d 0a20 2020 2020  entation>..     
-000006b0: 2020 203c 2f61 6e6e 6f74 6174 696f 6e3e     </annotation>
-000006c0: 0d0a 2020 2020 2020 2020 3c72 6573 7472  ..        <restr
-000006d0: 6963 7469 6f6e 2062 6173 653d 2264 6f75  iction base="dou
-000006e0: 626c 6522 3e0d 0a20 2020 2020 2020 2020  ble">..         
-000006f0: 2020 203c 6d69 6e45 7863 6c75 7369 7665     <minExclusive
-00000700: 2076 616c 7565 3d22 302e 3022 202f 3e0d   value="0.0" />.
-00000710: 0a20 2020 2020 2020 203c 2f72 6573 7472  .        </restr
-00000720: 6963 7469 6f6e 3e0d 0a20 2020 203c 2f73  iction>..    </s
-00000730: 696d 706c 6554 7970 653e 0d0a 0d0a 2020  impleType>....  
-00000740: 2020 3c73 696d 706c 6554 7970 6520 6e61    <simpleType na
-00000750: 6d65 3d22 466c 6f61 7436 345f 5479 7065  me="Float64_Type
-00000760: 223e 0d0a 2020 2020 2020 2020 3c61 6e6e  ">..        <ann
-00000770: 6f74 6174 696f 6e3e 0d0a 2020 2020 2020  otation>..      
-00000780: 2020 2020 2020 3c64 6f63 756d 656e 7461        <documenta
-00000790: 7469 6f6e 2078 6d6c 3a6c 616e 673d 2265  tion xml:lang="e
-000007a0: 6e22 3e46 6c6f 6174 3634 2c20 692e 652e  n">Float64, i.e.
-000007b0: 2c20 6120 646f 7562 6c65 2028 666c 6f61  , a double (floa
-000007c0: 7436 3429 2e3c 2f64 6f63 756d 656e 7461  t64).</documenta
-000007d0: 7469 6f6e 3e0d 0a20 2020 2020 2020 203c  tion>..        <
-000007e0: 2f61 6e6e 6f74 6174 696f 6e3e 0d0a 2020  /annotation>..  
-000007f0: 2020 2020 2020 3c72 6573 7472 6963 7469        <restricti
-00000800: 6f6e 2062 6173 653d 2264 6f75 626c 6522  on base="double"
-00000810: 202f 3e0d 0a20 2020 203c 2f73 696d 706c   />..    </simpl
-00000820: 6554 7970 653e 0d0a 2020 2020 0d0a 2020  eType>..    ..  
-00000830: 2020 3c63 6f6d 706c 6578 5479 7065 206e    <complexType n
-00000840: 616d 653d 224e 6f6e 456d 7074 794e 616d  ame="NonEmptyNam
-00000850: 655f 5479 7065 223e 0d0a 2020 2020 2020  e_Type">..      
-00000860: 2020 3c61 6e6e 6f74 6174 696f 6e3e 0d0a    <annotation>..
-00000870: 2020 2020 2020 2020 2020 2020 3c64 6f63              <doc
-00000880: 756d 656e 7461 7469 6f6e 2078 6d6c 3a6c  umentation xml:l
-00000890: 616e 673d 2265 6e22 3e41 2063 6f6d 706c  ang="en">A compl
-000008a0: 6578 2074 7970 6520 7769 7468 2061 206e  ex type with a n
-000008b0: 6f6e 2065 6d70 7479 2073 7472 696e 6720  on empty string 
-000008c0: 6174 7472 6962 7574 6520 6361 6c65 6420  attribute caled 
-000008d0: 6e61 6d65 2e20 5468 6973 2074 7970 6520  name. This type 
-000008e0: 6973 2075 7365 6420 746f 2072 6566 6572  is used to refer
-000008f0: 656e 6365 2046 4353 2064 696d 656e 7369  ence FCS dimensi
-00000900: 6f6e 732e 3c2f 646f 6375 6d65 6e74 6174  ons.</documentat
-00000910: 696f 6e3e 0d0a 2020 2020 2020 2020 3c2f  ion>..        </
-00000920: 616e 6e6f 7461 7469 6f6e 3e0d 0a20 2020  annotation>..   
-00000930: 2020 2020 203c 6174 7472 6962 7574 6520       <attribute 
-00000940: 6e61 6d65 3d22 6e61 6d65 2220 7573 653d  name="name" use=
-00000950: 2272 6571 7569 7265 6422 2074 7970 653d  "required" type=
-00000960: 2264 6174 612d 7479 7065 3a4e 6f6e 456d  "data-type:NonEm
-00000970: 7074 7953 7472 696e 675f 5479 7065 2220  ptyString_Type" 
-00000980: 2f3e 0d0a 2020 2020 3c2f 636f 6d70 6c65  />..    </comple
-00000990: 7854 7970 653e 0d0a 0d0a 2020 2020 3c73  xType>....    <s
-000009a0: 696d 706c 6554 7970 6520 6e61 6d65 3d22  impleType name="
-000009b0: 4e6f 6e45 6d70 7479 5374 7269 6e67 5f54  NonEmptyString_T
-000009c0: 7970 6522 3e0d 0a20 2020 2020 2020 203c  ype">..        <
-000009d0: 7265 7374 7269 6374 696f 6e20 6261 7365  restriction base
-000009e0: 3d22 7374 7269 6e67 223e 0d0a 2020 2020  ="string">..    
-000009f0: 2020 2020 2020 2020 3c6d 696e 4c65 6e67          <minLeng
-00000a00: 7468 2076 616c 7565 3d22 3122 202f 3e0d  th value="1" />.
-00000a10: 0a20 2020 2020 2020 203c 2f72 6573 7472  .        </restr
-00000a20: 6963 7469 6f6e 3e0d 0a20 2020 203c 2f73  iction>..    </s
-00000a30: 696d 706c 6554 7970 653e 0d0a 0d0a 2020  impleType>....  
-00000a40: 2020 3c63 6f6d 706c 6578 5479 7065 206e    <complexType n
-00000a50: 616d 653d 2256 616c 7565 4174 7472 6962  ame="ValueAttrib
-00000a60: 7574 655f 5479 7065 223e 0d0a 2020 2020  ute_Type">..    
-00000a70: 2020 2020 3c61 6e6e 6f74 6174 696f 6e3e      <annotation>
-00000a80: 0d0a 2020 2020 2020 2020 2020 2020 3c64  ..            <d
-00000a90: 6f63 756d 656e 7461 7469 6f6e 3e41 2073  ocumentation>A s
-00000aa0: 696e 676c 6520 7661 6c75 6520 6174 7472  ingle value attr
-00000ab0: 6962 7574 6520 6f66 2074 6865 2074 7970  ibute of the typ
-00000ac0: 6520 646f 7562 6c65 2028 666c 6f61 7436  e double (float6
-00000ad0: 3429 2e3c 2f64 6f63 756d 656e 7461 7469  4).</documentati
-00000ae0: 6f6e 3e0d 0a20 2020 2020 2020 203c 2f61  on>..        </a
-00000af0: 6e6e 6f74 6174 696f 6e3e 0d0a 2020 2020  nnotation>..    
-00000b00: 2020 2020 3c61 7474 7269 6275 7465 206e      <attribute n
-00000b10: 616d 653d 2276 616c 7565 2220 7479 7065  ame="value" type
-00000b20: 3d22 646f 7562 6c65 2220 7573 653d 2272  ="double" use="r
-00000b30: 6571 7569 7265 6422 2069 643d 2276 616c  equired" id="val
-00000b40: 7565 2220 2f3e 0d0a 2020 2020 3c2f 636f  ue" />..    </co
-00000b50: 6d70 6c65 7854 7970 653e 0d0a 0d0a 0d0a  mplexType>......
-00000b60: 2020 2020 3c63 6f6d 706c 6578 5479 7065      <complexType
-00000b70: 206e 616d 653d 2255 5661 6c75 6541 7474   name="UValueAtt
-00000b80: 7269 6275 7465 5f54 7970 6522 3e0d 0a20  ribute_Type">.. 
-00000b90: 2020 2020 2020 203c 616e 6e6f 7461 7469         <annotati
-00000ba0: 6f6e 3e0d 0a20 2020 2020 2020 2020 2020  on>..           
-00000bb0: 203c 646f 6375 6d65 6e74 6174 696f 6e3e   <documentation>
-00000bc0: 4120 7369 6e67 6c65 2076 616c 7565 2061  A single value a
-00000bd0: 7474 7269 6275 7465 206f 6620 7468 6520  ttribute of the 
-00000be0: 7479 7065 2064 6f75 626c 6520 2866 6c6f  type double (flo
-00000bf0: 6174 3634 2920 7468 6174 2069 7320 3e3d  at64) that is >=
-00000c00: 2030 2e64 3c2f 646f 6375 6d65 6e74 6174   0.d</documentat
-00000c10: 696f 6e3e 0d0a 2020 2020 2020 2020 3c2f  ion>..        </
-00000c20: 616e 6e6f 7461 7469 6f6e 3e0d 0a20 2020  annotation>..   
-00000c30: 2020 2020 203c 636f 6d70 6c65 7843 6f6e       <complexCon
-00000c40: 7465 6e74 3e0d 0a20 2020 2020 2020 2020  tent>..         
-00000c50: 2020 203c 7265 7374 7269 6374 696f 6e20     <restriction 
-00000c60: 6261 7365 3d22 6461 7461 2d74 7970 653a  base="data-type:
-00000c70: 5661 6c75 6541 7474 7269 6275 7465 5f54  ValueAttribute_T
-00000c80: 7970 6522 3e0d 0a20 2020 2020 2020 2020  ype">..         
-00000c90: 2020 2020 2020 203c 6174 7472 6962 7574         <attribut
-00000ca0: 6520 6e61 6d65 3d22 7661 6c75 6522 2074  e name="value" t
-00000cb0: 7970 653d 2264 6174 612d 7479 7065 3a55  ype="data-type:U
-00000cc0: 466c 6f61 7436 345f 5479 7065 2220 7573  Float64_Type" us
-00000cd0: 653d 2272 6571 7569 7265 6422 202f 3e0d  e="required" />.
-00000ce0: 0a20 2020 2020 2020 2020 2020 203c 2f72  .            </r
-00000cf0: 6573 7472 6963 7469 6f6e 3e0d 0a20 2020  estriction>..   
-00000d00: 2020 2020 203c 2f63 6f6d 706c 6578 436f       </complexCo
-00000d10: 6e74 656e 743e 0d0a 2020 2020 3c2f 636f  ntent>..    </co
-00000d20: 6d70 6c65 7854 7970 653e 0d0a 0d0a 2020  mplexType>....  
-00000d30: 2020 3c67 726f 7570 206e 616d 653d 2244    <group name="D
-00000d40: 696d 656e 7369 6f6e 735f 4772 6f75 7022  imensions_Group"
-00000d50: 3e0d 0a20 2020 2020 2020 203c 616e 6e6f  >..        <anno
-00000d60: 7461 7469 6f6e 3e0d 0a20 2020 2020 2020  tation>..       
-00000d70: 2020 2020 203c 646f 6375 6d65 6e74 6174       <documentat
-00000d80: 696f 6e20 786d 6c3a 6c61 6e67 3d22 656e  ion xml:lang="en
-00000d90: 223e 4120 6469 6d65 6e73 696f 6e20 6672  ">A dimension fr
-00000da0: 6f6d 2074 6865 2046 4353 2066 696c 653b  om the FCS file;
-00000db0: 2074 6869 7320 7368 616c 6c20 636f 7272   this shall corr
-00000dc0: 6573 706f 6e64 2074 6f20 7468 6520 7661  espond to the va
-00000dd0: 6c75 6520 6f66 2074 6865 2024 506e 4e20  lue of the $PnN 
-00000de0: 6b65 7977 6f72 6420 696e 2046 4353 2066  keyword in FCS f
-00000df0: 696c 6573 2c20 6f72 2061 206e 6577 6c79  iles, or a newly
-00000e00: 2063 7265 6174 6564 2064 696d 656e 7369   created dimensi
-00000e10: 6f6e 2e3c 2f64 6f63 756d 656e 7461 7469  on.</documentati
-00000e20: 6f6e 3e0d 0a20 2020 2020 2020 203c 2f61  on>..        </a
-00000e30: 6e6e 6f74 6174 696f 6e3e 0d0a 2020 2020  nnotation>..    
-00000e40: 2020 2020 3c63 686f 6963 653e 0d0a 2020      <choice>..  
-00000e50: 2020 2020 2020 2020 2020 3c65 6c65 6d65            <eleme
-00000e60: 6e74 206e 616d 653d 2266 6373 2d64 696d  nt name="fcs-dim
-00000e70: 656e 7369 6f6e 2220 7479 7065 3d22 6461  ension" type="da
-00000e80: 7461 2d74 7970 653a 4e6f 6e45 6d70 7479  ta-type:NonEmpty
-00000e90: 4e61 6d65 5f54 7970 6522 202f 3e0d 0a20  Name_Type" />.. 
-00000ea0: 2020 2020 2020 2020 2020 203c 656c 656d             <elem
-00000eb0: 656e 7420 6e61 6d65 3d22 6e65 772d 6469  ent name="new-di
-00000ec0: 6d65 6e73 696f 6e22 2074 7970 653d 2264  mension" type="d
-00000ed0: 6174 612d 7479 7065 3a54 7261 6e73 666f  ata-type:Transfo
-00000ee0: 726d 6174 696f 6e52 6566 6572 656e 6365  rmationReference
-00000ef0: 5f54 7970 6522 202f 3e0d 0a20 2020 2020  _Type" />..     
-00000f00: 2020 203c 2f63 686f 6963 653e 0d0a 2020     </choice>..  
-00000f10: 2020 3c2f 6772 6f75 703e 0d0a 0d0a 2020    </group>....  
-00000f20: 2020 3c67 726f 7570 206e 616d 653d 2246    <group name="F
-00000f30: 4353 4469 6d65 6e73 696f 6e73 5f47 726f  CSDimensions_Gro
-00000f40: 7570 223e 0d0a 2020 2020 2020 2020 3c61  up">..        <a
-00000f50: 6e6e 6f74 6174 696f 6e3e 0d0a 2020 2020  nnotation>..    
-00000f60: 2020 2020 2020 2020 3c64 6f63 756d 656e          <documen
-00000f70: 7461 7469 6f6e 2078 6d6c 3a6c 616e 673d  tation xml:lang=
-00000f80: 2265 6e22 3e41 2064 696d 656e 7369 6f6e  "en">A dimension
-00000f90: 2066 726f 6d20 7468 6520 4643 5320 6669   from the FCS fi
-00000fa0: 6c65 3b20 7468 6973 2073 6861 6c6c 2063  le; this shall c
-00000fb0: 6f72 7265 7370 6f6e 6420 746f 2074 6865  orrespond to the
-00000fc0: 2076 616c 7565 206f 6620 7468 6520 2450   value of the $P
-00000fd0: 6e4e 206b 6579 776f 7264 2069 6e20 4643  nN keyword in FC
-00000fe0: 5320 6669 6c65 732e 3c2f 646f 6375 6d65  S files.</docume
-00000ff0: 6e74 6174 696f 6e3e 0d0a 2020 2020 2020  ntation>..      
-00001000: 2020 3c2f 616e 6e6f 7461 7469 6f6e 3e0d    </annotation>.
-00001010: 0a20 2020 2020 2020 203c 7365 7175 656e  .        <sequen
-00001020: 6365 3e0d 0a20 2020 2020 2020 2020 2020  ce>..           
-00001030: 203c 656c 656d 656e 7420 6e61 6d65 3d22   <element name="
-00001040: 6663 732d 6469 6d65 6e73 696f 6e22 2074  fcs-dimension" t
-00001050: 7970 653d 2264 6174 612d 7479 7065 3a4e  ype="data-type:N
-00001060: 6f6e 456d 7074 794e 616d 655f 5479 7065  onEmptyName_Type
-00001070: 2220 2f3e 0d0a 2020 2020 2020 2020 3c2f  " />..        </
-00001080: 7365 7175 656e 6365 3e0d 0a20 2020 203c  sequence>..    <
-00001090: 2f67 726f 7570 3e0d 0a20 2020 200d 0a0d  /group>..    ...
-000010a0: 0a20 2020 203c 636f 6d70 6c65 7854 7970  .    <complexTyp
-000010b0: 6520 6e61 6d65 3d22 5472 616e 7366 6f72  e name="Transfor
-000010c0: 6d61 7469 6f6e 5265 6665 7265 6e63 655f  mationReference_
-000010d0: 5479 7065 223e 0d0a 2020 2020 2020 2020  Type">..        
-000010e0: 3c61 6e6e 6f74 6174 696f 6e3e 0d0a 2020  <annotation>..  
-000010f0: 2020 2020 2020 2020 2020 3c64 6f63 756d            <docum
-00001100: 656e 7461 7469 6f6e 2078 6d6c 3a6c 616e  entation xml:lan
-00001110: 673d 2265 6e22 3e41 2063 6f6d 706c 6578  g="en">A complex
-00001120: 2074 7970 6520 7769 7468 2061 206e 6f6e   type with a non
-00001130: 2065 6d70 7479 2073 7472 696e 6720 6174   empty string at
-00001140: 7472 6962 7574 6520 6361 6c65 6420 6e61  tribute caled na
-00001150: 6d65 2e20 5468 6973 2074 7970 6520 6973  me. This type is
-00001160: 2075 7365 6420 746f 2072 6566 6572 656e   used to referen
-00001170: 6365 2046 4353 2064 696d 656e 7369 6f6e  ce FCS dimension
-00001180: 732e 3c2f 646f 6375 6d65 6e74 6174 696f  s.</documentatio
-00001190: 6e3e 0d0a 2020 2020 2020 2020 3c2f 616e  n>..        </an
-000011a0: 6e6f 7461 7469 6f6e 3e0d 0a20 2020 2020  notation>..     
-000011b0: 2020 203c 6174 7472 6962 7574 6520 6e61     <attribute na
-000011c0: 6d65 3d22 7472 616e 7366 6f72 6d61 7469  me="transformati
-000011d0: 6f6e 2d72 6566 2220 7573 653d 2272 6571  on-ref" use="req
-000011e0: 7569 7265 6422 2074 7970 653d 2249 4452  uired" type="IDR
-000011f0: 4546 2220 2f3e 0d0a 2020 2020 3c2f 636f  EF" />..    </co
-00001200: 6d70 6c65 7854 7970 653e 0d0a 2020 2020  mplexType>..    
-00001210: 2020 2020 0d0a 2020 2020 3c67 726f 7570      ..    <group
-00001220: 206e 616d 653d 2243 7573 746f 6d5f 4772   name="Custom_Gr
-00001230: 6f75 7022 3e0d 0a20 2020 2020 2020 203c  oup">..        <
-00001240: 616e 6e6f 7461 7469 6f6e 3e0d 0a20 2020  annotation>..   
-00001250: 2020 2020 2020 2020 203c 646f 6375 6d65           <docume
-00001260: 6e74 6174 696f 6e20 786d 6c3a 6c61 6e67  ntation xml:lang
-00001270: 3d22 656e 223e 4375 7272 656e 746c 792c  ="en">Currently,
-00001280: 2074 6865 2063 686f 6963 6520 6973 206c   the choice is l
-00001290: 696d 6974 6564 2074 6f20 7468 6520 6375  imited to the cu
-000012a0: 7374 6f6d 5f69 6e66 6f20 656c 656d 656e  stom_info elemen
-000012b0: 742e 3c2f 646f 6375 6d65 6e74 6174 696f  t.</documentatio
-000012c0: 6e3e 0d0a 2020 2020 2020 2020 3c2f 616e  n>..        </an
-000012d0: 6e6f 7461 7469 6f6e 3e0d 0a20 2020 2020  notation>..     
-000012e0: 2020 203c 6368 6f69 6365 3e0d 0a20 2020     <choice>..   
-000012f0: 2020 2020 2020 2020 203c 656c 656d 656e           <elemen
-00001300: 7420 6e61 6d65 3d22 6375 7374 6f6d 5f69  t name="custom_i
-00001310: 6e66 6f22 2074 7970 653d 2261 6e79 5479  nfo" type="anyTy
-00001320: 7065 2220 2f3e 0d0a 2020 2020 2020 2020  pe" />..        
-00001330: 3c2f 6368 6f69 6365 3e0d 0a20 2020 203c  </choice>..    <
-00001340: 2f67 726f 7570 3e0d 0a20 2020 200d 0a3c  /group>..    ..<
-00001350: 2f73 6368 656d 613e 0d0a                 /schema>..
+00000020: 462d 3822 3f3e 0a0a 3c73 6368 656d 6120  F-8"?>..<schema 
+00000030: 786d 6c6e 733d 2268 7474 703a 2f2f 7777  xmlns="http://ww
+00000040: 772e 7733 2e6f 7267 2f32 3030 312f 584d  w.w3.org/2001/XM
+00000050: 4c53 6368 656d 6122 0a20 2020 2078 6d6c  LSchema".    xml
+00000060: 6e73 3a64 6174 612d 7479 7065 3d22 6874  ns:data-type="ht
+00000070: 7470 3a2f 2f77 7777 2e69 7361 632d 6e65  tp://www.isac-ne
+00000080: 742e 6f72 672f 7374 642f 4761 7469 6e67  t.org/std/Gating
+00000090: 2d4d 4c2f 7632 2e30 2f64 6174 6174 7970  -ML/v2.0/datatyp
+000000a0: 6573 220a 2020 2020 786d 6c6e 733a 7472  es".    xmlns:tr
+000000b0: 616e 7366 6f72 6d73 3d22 6874 7470 3a2f  ansforms="http:/
+000000c0: 2f77 7777 2e69 7361 632d 6e65 742e 6f72  /www.isac-net.or
+000000d0: 672f 7374 642f 4761 7469 6e67 2d4d 4c2f  g/std/Gating-ML/
+000000e0: 7632 2e30 2f74 7261 6e73 666f 726d 6174  v2.0/transformat
+000000f0: 696f 6e73 220a 2020 2020 7461 7267 6574  ions".    target
+00000100: 4e61 6d65 7370 6163 653d 2268 7474 703a  Namespace="http:
+00000110: 2f2f 7777 772e 6973 6163 2d6e 6574 2e6f  //www.isac-net.o
+00000120: 7267 2f73 7464 2f47 6174 696e 672d 4d4c  rg/std/Gating-ML
+00000130: 2f76 322e 302f 6461 7461 7479 7065 7322  /v2.0/datatypes"
+00000140: 0a20 2020 2065 6c65 6d65 6e74 466f 726d  .    elementForm
+00000150: 4465 6661 756c 743d 2271 7561 6c69 6669  Default="qualifi
+00000160: 6564 2220 6174 7472 6962 7574 6546 6f72  ed" attributeFor
+00000170: 6d44 6566 6175 6c74 3d22 7175 616c 6966  mDefault="qualif
+00000180: 6965 6422 2076 6572 7369 6f6e 3d22 322e  ied" version="2.
+00000190: 302e 3132 3132 3037 223e 0a0a 2020 2020  0.121207">..    
+000001a0: 3c61 6e6e 6f74 6174 696f 6e3e 0a20 2020  <annotation>.   
+000001b0: 2020 2020 203c 6170 7069 6e66 6f20 736f       <appinfo so
+000001c0: 7572 6365 3d22 6874 7470 3a2f 2f66 6c6f  urce="http://flo
+000001d0: 7763 7974 2e73 6f75 7263 6566 6f72 6765  wcyt.sourceforge
+000001e0: 2e6e 6574 2f22 3e44 6566 696e 6974 696f  .net/">Definitio
+000001f0: 6e20 6f66 2064 6174 6120 7479 7065 7320  n of data types 
+00000200: 7265 7573 6564 2069 6e20 584d 4c2d 6261  reused in XML-ba
+00000210: 7365 6420 7374 616e 6461 7264 7320 7375  sed standards su
+00000220: 6368 2061 7320 4761 7469 6e67 2d4d 4c20  ch as Gating-ML 
+00000230: 584d 4c20 7363 6865 6d61 2e3c 2f61 7070  XML schema.</app
+00000240: 696e 666f 3e0a 2020 2020 2020 2020 3c64  info>.        <d
+00000250: 6f63 756d 656e 7461 7469 6f6e 2078 6d6c  ocumentation xml
+00000260: 3a6c 616e 673d 2265 6e22 2073 6f75 7263  :lang="en" sourc
+00000270: 653d 2268 7474 703a 2f2f 666c 6f77 6379  e="http://flowcy
+00000280: 742e 736f 7572 6365 666f 7267 652e 6e65  t.sourceforge.ne
+00000290: 742f 223e 0a20 2020 2020 2020 2020 2020  t/">.           
+000002a0: 203c 6175 7468 6f72 3e0a 2020 2020 2020   <author>.      
+000002b0: 2020 2020 2020 2020 2020 3c6e 616d 653e            <name>
+000002c0: 4a6f 7365 6620 5370 6964 6c65 6e3c 2f6e  Josef Spidlen</n
+000002d0: 616d 653e 0a20 2020 2020 2020 2020 2020  ame>.           
+000002e0: 2020 2020 203c 656d 6169 6c3e 6a73 7069       <email>jspi
+000002f0: 646c 656e 4062 6363 7263 2e63 613c 2f65  dlen@bccrc.ca</e
+00000300: 6d61 696c 3e0a 2020 2020 2020 2020 2020  mail>.          
+00000310: 2020 3c2f 6175 7468 6f72 3e0a 2020 2020    </author>.    
+00000320: 2020 2020 2020 2020 3c63 6f70 7972 6967          <copyrig
+00000330: 6874 3e0a 2020 2020 2020 2020 2020 2020  ht>.            
+00000340: 2020 2020 436f 7079 7269 6768 7420 2863      Copyright (c
+00000350: 2920 3230 3038 2d32 3031 3420 4953 4143  ) 2008-2014 ISAC
+00000360: 2028 496e 7465 726e 6174 696f 6e61 6c20   (International 
+00000370: 536f 6369 6574 7920 666f 7220 4164 7661  Society for Adva
+00000380: 6e63 656d 656e 7420 6f66 0a20 2020 2020  ncement of.     
+00000390: 2020 2020 2020 2020 2020 2043 7974 6f6d             Cytom
+000003a0: 6574 7279 292e 2046 7265 6520 6f66 2063  etry). Free of c
+000003b0: 6861 7267 6520 6469 7374 7269 6275 7469  harge distributi
+000003c0: 6f6e 2061 6e64 2072 6561 642d 6f6e 6c79  on and read-only
+000003d0: 2075 7361 6765 2070 6572 6d69 7465 642e   usage permited.
+000003e0: 204d 6f64 6966 6963 6174 696f 6e0a 2020   Modification.  
+000003f0: 2020 2020 2020 2020 2020 2020 2020 616e                an
+00000400: 6420 616c 6c20 6f74 6865 7220 7269 6768  d all other righ
+00000410: 7473 2072 6573 6572 7665 642e 2046 6f72  ts reserved. For
+00000420: 2061 6c6c 206f 7468 6572 2075 7365 7320   all other uses 
+00000430: 706c 6561 7365 2063 6f6e 7461 6374 2049  please contact I
+00000440: 5341 432e 0a20 2020 2020 2020 2020 2020  SAC..           
+00000450: 203c 2f63 6f70 7972 6967 6874 3e0a 2020   </copyright>.  
+00000460: 2020 2020 2020 3c2f 646f 6375 6d65 6e74        </document
+00000470: 6174 696f 6e3e 0a20 2020 203c 2f61 6e6e  ation>.    </ann
+00000480: 6f74 6174 696f 6e3e 0a0a 2020 2020 3c73  otation>..    <s
+00000490: 696d 706c 6554 7970 6520 6e61 6d65 3d22  impleType name="
+000004a0: 5546 6c6f 6174 3634 5f54 7970 6522 3e0a  UFloat64_Type">.
+000004b0: 2020 2020 2020 2020 3c61 6e6e 6f74 6174          <annotat
+000004c0: 696f 6e3e 0a20 2020 2020 2020 2020 2020  ion>.           
+000004d0: 203c 646f 6375 6d65 6e74 6174 696f 6e20   <documentation 
+000004e0: 786d 6c3a 6c61 6e67 3d22 656e 223e 556e  xml:lang="en">Un
+000004f0: 7369 676e 6564 2066 6c6f 6174 3634 2c20  signed float64, 
+00000500: 692e 652c 2061 2064 6f75 626c 6520 2866  i.e, a double (f
+00000510: 6c6f 6174 3634 2920 7468 6174 2069 7320  loat64) that is 
+00000520: 6772 6561 7465 7220 6f72 2065 7175 616c  greater or equal
+00000530: 2030 2e3c 2f64 6f63 756d 656e 7461 7469   0.</documentati
+00000540: 6f6e 3e0a 2020 2020 2020 2020 3c2f 616e  on>.        </an
+00000550: 6e6f 7461 7469 6f6e 3e0a 2020 2020 2020  notation>.      
+00000560: 2020 3c72 6573 7472 6963 7469 6f6e 2062    <restriction b
+00000570: 6173 653d 2264 6f75 626c 6522 3e0a 2020  ase="double">.  
+00000580: 2020 2020 2020 2020 2020 3c6d 696e 496e            <minIn
+00000590: 636c 7573 6976 6520 7661 6c75 653d 2230  clusive value="0
+000005a0: 2e30 2220 2f3e 0a20 2020 2020 2020 203c  .0" />.        <
+000005b0: 2f72 6573 7472 6963 7469 6f6e 3e0a 2020  /restriction>.  
+000005c0: 2020 3c2f 7369 6d70 6c65 5479 7065 3e0a    </simpleType>.
+000005d0: 0a20 2020 203c 7369 6d70 6c65 5479 7065  .    <simpleType
+000005e0: 206e 616d 653d 2250 466c 6f61 7436 345f   name="PFloat64_
+000005f0: 5479 7065 223e 0a20 2020 2020 2020 203c  Type">.        <
+00000600: 616e 6e6f 7461 7469 6f6e 3e0a 2020 2020  annotation>.    
+00000610: 2020 2020 2020 2020 3c64 6f63 756d 656e          <documen
+00000620: 7461 7469 6f6e 2078 6d6c 3a6c 616e 673d  tation xml:lang=
+00000630: 2265 6e22 3e50 6f73 6974 6976 6520 666c  "en">Positive fl
+00000640: 6f61 7436 342c 2069 2e65 2e2c 2061 2064  oat64, i.e., a d
+00000650: 6f75 626c 6520 2866 6c6f 6174 3634 2920  ouble (float64) 
+00000660: 7468 6174 2069 7320 6772 6561 7465 7220  that is greater 
+00000670: 7468 616e 2030 2e3c 2f64 6f63 756d 656e  than 0.</documen
+00000680: 7461 7469 6f6e 3e0a 2020 2020 2020 2020  tation>.        
+00000690: 3c2f 616e 6e6f 7461 7469 6f6e 3e0a 2020  </annotation>.  
+000006a0: 2020 2020 2020 3c72 6573 7472 6963 7469        <restricti
+000006b0: 6f6e 2062 6173 653d 2264 6f75 626c 6522  on base="double"
+000006c0: 3e0a 2020 2020 2020 2020 2020 2020 3c6d  >.            <m
+000006d0: 696e 4578 636c 7573 6976 6520 7661 6c75  inExclusive valu
+000006e0: 653d 2230 2e30 2220 2f3e 0a20 2020 2020  e="0.0" />.     
+000006f0: 2020 203c 2f72 6573 7472 6963 7469 6f6e     </restriction
+00000700: 3e0a 2020 2020 3c2f 7369 6d70 6c65 5479  >.    </simpleTy
+00000710: 7065 3e0a 0a20 2020 203c 7369 6d70 6c65  pe>..    <simple
+00000720: 5479 7065 206e 616d 653d 2246 6c6f 6174  Type name="Float
+00000730: 3634 5f54 7970 6522 3e0a 2020 2020 2020  64_Type">.      
+00000740: 2020 3c61 6e6e 6f74 6174 696f 6e3e 0a20    <annotation>. 
+00000750: 2020 2020 2020 2020 2020 203c 646f 6375             <docu
+00000760: 6d65 6e74 6174 696f 6e20 786d 6c3a 6c61  mentation xml:la
+00000770: 6e67 3d22 656e 223e 466c 6f61 7436 342c  ng="en">Float64,
+00000780: 2069 2e65 2e2c 2061 2064 6f75 626c 6520   i.e., a double 
+00000790: 2866 6c6f 6174 3634 292e 3c2f 646f 6375  (float64).</docu
+000007a0: 6d65 6e74 6174 696f 6e3e 0a20 2020 2020  mentation>.     
+000007b0: 2020 203c 2f61 6e6e 6f74 6174 696f 6e3e     </annotation>
+000007c0: 0a20 2020 2020 2020 203c 7265 7374 7269  .        <restri
+000007d0: 6374 696f 6e20 6261 7365 3d22 646f 7562  ction base="doub
+000007e0: 6c65 2220 2f3e 0a20 2020 203c 2f73 696d  le" />.    </sim
+000007f0: 706c 6554 7970 653e 0a20 2020 200a 2020  pleType>.    .  
+00000800: 2020 3c63 6f6d 706c 6578 5479 7065 206e    <complexType n
+00000810: 616d 653d 224e 6f6e 456d 7074 794e 616d  ame="NonEmptyNam
+00000820: 655f 5479 7065 223e 0a20 2020 2020 2020  e_Type">.       
+00000830: 203c 616e 6e6f 7461 7469 6f6e 3e0a 2020   <annotation>.  
+00000840: 2020 2020 2020 2020 2020 3c64 6f63 756d            <docum
+00000850: 656e 7461 7469 6f6e 2078 6d6c 3a6c 616e  entation xml:lan
+00000860: 673d 2265 6e22 3e41 2063 6f6d 706c 6578  g="en">A complex
+00000870: 2074 7970 6520 7769 7468 2061 206e 6f6e   type with a non
+00000880: 2065 6d70 7479 2073 7472 696e 6720 6174   empty string at
+00000890: 7472 6962 7574 6520 6361 6c65 6420 6e61  tribute caled na
+000008a0: 6d65 2e20 5468 6973 2074 7970 6520 6973  me. This type is
+000008b0: 2075 7365 6420 746f 2072 6566 6572 656e   used to referen
+000008c0: 6365 2046 4353 2064 696d 656e 7369 6f6e  ce FCS dimension
+000008d0: 732e 3c2f 646f 6375 6d65 6e74 6174 696f  s.</documentatio
+000008e0: 6e3e 0a20 2020 2020 2020 203c 2f61 6e6e  n>.        </ann
+000008f0: 6f74 6174 696f 6e3e 0a20 2020 2020 2020  otation>.       
+00000900: 203c 6174 7472 6962 7574 6520 6e61 6d65   <attribute name
+00000910: 3d22 6e61 6d65 2220 7573 653d 2272 6571  ="name" use="req
+00000920: 7569 7265 6422 2074 7970 653d 2264 6174  uired" type="dat
+00000930: 612d 7479 7065 3a4e 6f6e 456d 7074 7953  a-type:NonEmptyS
+00000940: 7472 696e 675f 5479 7065 2220 2f3e 0a20  tring_Type" />. 
+00000950: 2020 203c 2f63 6f6d 706c 6578 5479 7065     </complexType
+00000960: 3e0a 0a20 2020 203c 7369 6d70 6c65 5479  >..    <simpleTy
+00000970: 7065 206e 616d 653d 224e 6f6e 456d 7074  pe name="NonEmpt
+00000980: 7953 7472 696e 675f 5479 7065 223e 0a20  yString_Type">. 
+00000990: 2020 2020 2020 203c 7265 7374 7269 6374         <restrict
+000009a0: 696f 6e20 6261 7365 3d22 7374 7269 6e67  ion base="string
+000009b0: 223e 0a20 2020 2020 2020 2020 2020 203c  ">.            <
+000009c0: 6d69 6e4c 656e 6774 6820 7661 6c75 653d  minLength value=
+000009d0: 2231 2220 2f3e 0a20 2020 2020 2020 203c  "1" />.        <
+000009e0: 2f72 6573 7472 6963 7469 6f6e 3e0a 2020  /restriction>.  
+000009f0: 2020 3c2f 7369 6d70 6c65 5479 7065 3e0a    </simpleType>.
+00000a00: 0a20 2020 203c 636f 6d70 6c65 7854 7970  .    <complexTyp
+00000a10: 6520 6e61 6d65 3d22 5661 6c75 6541 7474  e name="ValueAtt
+00000a20: 7269 6275 7465 5f54 7970 6522 3e0a 2020  ribute_Type">.  
+00000a30: 2020 2020 2020 3c61 6e6e 6f74 6174 696f        <annotatio
+00000a40: 6e3e 0a20 2020 2020 2020 2020 2020 203c  n>.            <
+00000a50: 646f 6375 6d65 6e74 6174 696f 6e3e 4120  documentation>A 
+00000a60: 7369 6e67 6c65 2076 616c 7565 2061 7474  single value att
+00000a70: 7269 6275 7465 206f 6620 7468 6520 7479  ribute of the ty
+00000a80: 7065 2064 6f75 626c 6520 2866 6c6f 6174  pe double (float
+00000a90: 3634 292e 3c2f 646f 6375 6d65 6e74 6174  64).</documentat
+00000aa0: 696f 6e3e 0a20 2020 2020 2020 203c 2f61  ion>.        </a
+00000ab0: 6e6e 6f74 6174 696f 6e3e 0a20 2020 2020  nnotation>.     
+00000ac0: 2020 203c 6174 7472 6962 7574 6520 6e61     <attribute na
+00000ad0: 6d65 3d22 7661 6c75 6522 2074 7970 653d  me="value" type=
+00000ae0: 2264 6f75 626c 6522 2075 7365 3d22 7265  "double" use="re
+00000af0: 7175 6972 6564 2220 6964 3d22 7661 6c75  quired" id="valu
+00000b00: 6522 202f 3e0a 2020 2020 3c2f 636f 6d70  e" />.    </comp
+00000b10: 6c65 7854 7970 653e 0a0a 0a20 2020 203c  lexType>...    <
+00000b20: 636f 6d70 6c65 7854 7970 6520 6e61 6d65  complexType name
+00000b30: 3d22 5556 616c 7565 4174 7472 6962 7574  ="UValueAttribut
+00000b40: 655f 5479 7065 223e 0a20 2020 2020 2020  e_Type">.       
+00000b50: 203c 616e 6e6f 7461 7469 6f6e 3e0a 2020   <annotation>.  
+00000b60: 2020 2020 2020 2020 2020 3c64 6f63 756d            <docum
+00000b70: 656e 7461 7469 6f6e 3e41 2073 696e 676c  entation>A singl
+00000b80: 6520 7661 6c75 6520 6174 7472 6962 7574  e value attribut
+00000b90: 6520 6f66 2074 6865 2074 7970 6520 646f  e of the type do
+00000ba0: 7562 6c65 2028 666c 6f61 7436 3429 2074  uble (float64) t
+00000bb0: 6861 7420 6973 203e 3d20 302e 643c 2f64  hat is >= 0.d</d
+00000bc0: 6f63 756d 656e 7461 7469 6f6e 3e0a 2020  ocumentation>.  
+00000bd0: 2020 2020 2020 3c2f 616e 6e6f 7461 7469        </annotati
+00000be0: 6f6e 3e0a 2020 2020 2020 2020 3c63 6f6d  on>.        <com
+00000bf0: 706c 6578 436f 6e74 656e 743e 0a20 2020  plexContent>.   
+00000c00: 2020 2020 2020 2020 203c 7265 7374 7269           <restri
+00000c10: 6374 696f 6e20 6261 7365 3d22 6461 7461  ction base="data
+00000c20: 2d74 7970 653a 5661 6c75 6541 7474 7269  -type:ValueAttri
+00000c30: 6275 7465 5f54 7970 6522 3e0a 2020 2020  bute_Type">.    
+00000c40: 2020 2020 2020 2020 2020 2020 3c61 7474              <att
+00000c50: 7269 6275 7465 206e 616d 653d 2276 616c  ribute name="val
+00000c60: 7565 2220 7479 7065 3d22 6461 7461 2d74  ue" type="data-t
+00000c70: 7970 653a 5546 6c6f 6174 3634 5f54 7970  ype:UFloat64_Typ
+00000c80: 6522 2075 7365 3d22 7265 7175 6972 6564  e" use="required
+00000c90: 2220 2f3e 0a20 2020 2020 2020 2020 2020  " />.           
+00000ca0: 203c 2f72 6573 7472 6963 7469 6f6e 3e0a   </restriction>.
+00000cb0: 2020 2020 2020 2020 3c2f 636f 6d70 6c65          </comple
+00000cc0: 7843 6f6e 7465 6e74 3e0a 2020 2020 3c2f  xContent>.    </
+00000cd0: 636f 6d70 6c65 7854 7970 653e 0a0a 2020  complexType>..  
+00000ce0: 2020 3c67 726f 7570 206e 616d 653d 2244    <group name="D
+00000cf0: 696d 656e 7369 6f6e 735f 4772 6f75 7022  imensions_Group"
+00000d00: 3e0a 2020 2020 2020 2020 3c61 6e6e 6f74  >.        <annot
+00000d10: 6174 696f 6e3e 0a20 2020 2020 2020 2020  ation>.         
+00000d20: 2020 203c 646f 6375 6d65 6e74 6174 696f     <documentatio
+00000d30: 6e20 786d 6c3a 6c61 6e67 3d22 656e 223e  n xml:lang="en">
+00000d40: 4120 6469 6d65 6e73 696f 6e20 6672 6f6d  A dimension from
+00000d50: 2074 6865 2046 4353 2066 696c 653b 2074   the FCS file; t
+00000d60: 6869 7320 7368 616c 6c20 636f 7272 6573  his shall corres
+00000d70: 706f 6e64 2074 6f20 7468 6520 7661 6c75  pond to the valu
+00000d80: 6520 6f66 2074 6865 2024 506e 4e20 6b65  e of the $PnN ke
+00000d90: 7977 6f72 6420 696e 2046 4353 2066 696c  yword in FCS fil
+00000da0: 6573 2c20 6f72 2061 206e 6577 6c79 2063  es, or a newly c
+00000db0: 7265 6174 6564 2064 696d 656e 7369 6f6e  reated dimension
+00000dc0: 2e3c 2f64 6f63 756d 656e 7461 7469 6f6e  .</documentation
+00000dd0: 3e0a 2020 2020 2020 2020 3c2f 616e 6e6f  >.        </anno
+00000de0: 7461 7469 6f6e 3e0a 2020 2020 2020 2020  tation>.        
+00000df0: 3c63 686f 6963 653e 0a20 2020 2020 2020  <choice>.       
+00000e00: 2020 2020 203c 656c 656d 656e 7420 6e61       <element na
+00000e10: 6d65 3d22 6663 732d 6469 6d65 6e73 696f  me="fcs-dimensio
+00000e20: 6e22 2074 7970 653d 2264 6174 612d 7479  n" type="data-ty
+00000e30: 7065 3a4e 6f6e 456d 7074 794e 616d 655f  pe:NonEmptyName_
+00000e40: 5479 7065 2220 2f3e 0a20 2020 2020 2020  Type" />.       
+00000e50: 2020 2020 203c 656c 656d 656e 7420 6e61       <element na
+00000e60: 6d65 3d22 6e65 772d 6469 6d65 6e73 696f  me="new-dimensio
+00000e70: 6e22 2074 7970 653d 2264 6174 612d 7479  n" type="data-ty
+00000e80: 7065 3a54 7261 6e73 666f 726d 6174 696f  pe:Transformatio
+00000e90: 6e52 6566 6572 656e 6365 5f54 7970 6522  nReference_Type"
+00000ea0: 202f 3e0a 2020 2020 2020 2020 3c2f 6368   />.        </ch
+00000eb0: 6f69 6365 3e0a 2020 2020 3c2f 6772 6f75  oice>.    </grou
+00000ec0: 703e 0a0a 2020 2020 3c67 726f 7570 206e  p>..    <group n
+00000ed0: 616d 653d 2246 4353 4469 6d65 6e73 696f  ame="FCSDimensio
+00000ee0: 6e73 5f47 726f 7570 223e 0a20 2020 2020  ns_Group">.     
+00000ef0: 2020 203c 616e 6e6f 7461 7469 6f6e 3e0a     <annotation>.
+00000f00: 2020 2020 2020 2020 2020 2020 3c64 6f63              <doc
+00000f10: 756d 656e 7461 7469 6f6e 2078 6d6c 3a6c  umentation xml:l
+00000f20: 616e 673d 2265 6e22 3e41 2064 696d 656e  ang="en">A dimen
+00000f30: 7369 6f6e 2066 726f 6d20 7468 6520 4643  sion from the FC
+00000f40: 5320 6669 6c65 3b20 7468 6973 2073 6861  S file; this sha
+00000f50: 6c6c 2063 6f72 7265 7370 6f6e 6420 746f  ll correspond to
+00000f60: 2074 6865 2076 616c 7565 206f 6620 7468   the value of th
+00000f70: 6520 2450 6e4e 206b 6579 776f 7264 2069  e $PnN keyword i
+00000f80: 6e20 4643 5320 6669 6c65 732e 3c2f 646f  n FCS files.</do
+00000f90: 6375 6d65 6e74 6174 696f 6e3e 0a20 2020  cumentation>.   
+00000fa0: 2020 2020 203c 2f61 6e6e 6f74 6174 696f       </annotatio
+00000fb0: 6e3e 0a20 2020 2020 2020 203c 7365 7175  n>.        <sequ
+00000fc0: 656e 6365 3e0a 2020 2020 2020 2020 2020  ence>.          
+00000fd0: 2020 3c65 6c65 6d65 6e74 206e 616d 653d    <element name=
+00000fe0: 2266 6373 2d64 696d 656e 7369 6f6e 2220  "fcs-dimension" 
+00000ff0: 7479 7065 3d22 6461 7461 2d74 7970 653a  type="data-type:
+00001000: 4e6f 6e45 6d70 7479 4e61 6d65 5f54 7970  NonEmptyName_Typ
+00001010: 6522 202f 3e0a 2020 2020 2020 2020 3c2f  e" />.        </
+00001020: 7365 7175 656e 6365 3e0a 2020 2020 3c2f  sequence>.    </
+00001030: 6772 6f75 703e 0a20 2020 200a 0a20 2020  group>.    ..   
+00001040: 203c 636f 6d70 6c65 7854 7970 6520 6e61   <complexType na
+00001050: 6d65 3d22 5472 616e 7366 6f72 6d61 7469  me="Transformati
+00001060: 6f6e 5265 6665 7265 6e63 655f 5479 7065  onReference_Type
+00001070: 223e 0a20 2020 2020 2020 203c 616e 6e6f  ">.        <anno
+00001080: 7461 7469 6f6e 3e0a 2020 2020 2020 2020  tation>.        
+00001090: 2020 2020 3c64 6f63 756d 656e 7461 7469      <documentati
+000010a0: 6f6e 2078 6d6c 3a6c 616e 673d 2265 6e22  on xml:lang="en"
+000010b0: 3e41 2063 6f6d 706c 6578 2074 7970 6520  >A complex type 
+000010c0: 7769 7468 2061 206e 6f6e 2065 6d70 7479  with a non empty
+000010d0: 2073 7472 696e 6720 6174 7472 6962 7574   string attribut
+000010e0: 6520 6361 6c65 6420 6e61 6d65 2e20 5468  e caled name. Th
+000010f0: 6973 2074 7970 6520 6973 2075 7365 6420  is type is used 
+00001100: 746f 2072 6566 6572 656e 6365 2046 4353  to reference FCS
+00001110: 2064 696d 656e 7369 6f6e 732e 3c2f 646f   dimensions.</do
+00001120: 6375 6d65 6e74 6174 696f 6e3e 0a20 2020  cumentation>.   
+00001130: 2020 2020 203c 2f61 6e6e 6f74 6174 696f       </annotatio
+00001140: 6e3e 0a20 2020 2020 2020 203c 6174 7472  n>.        <attr
+00001150: 6962 7574 6520 6e61 6d65 3d22 7472 616e  ibute name="tran
+00001160: 7366 6f72 6d61 7469 6f6e 2d72 6566 2220  sformation-ref" 
+00001170: 7573 653d 2272 6571 7569 7265 6422 2074  use="required" t
+00001180: 7970 653d 2249 4452 4546 2220 2f3e 0a20  ype="IDREF" />. 
+00001190: 2020 203c 2f63 6f6d 706c 6578 5479 7065     </complexType
+000011a0: 3e0a 2020 2020 2020 2020 0a20 2020 203c  >.        .    <
+000011b0: 6772 6f75 7020 6e61 6d65 3d22 4375 7374  group name="Cust
+000011c0: 6f6d 5f47 726f 7570 223e 0a20 2020 2020  om_Group">.     
+000011d0: 2020 203c 616e 6e6f 7461 7469 6f6e 3e0a     <annotation>.
+000011e0: 2020 2020 2020 2020 2020 2020 3c64 6f63              <doc
+000011f0: 756d 656e 7461 7469 6f6e 2078 6d6c 3a6c  umentation xml:l
+00001200: 616e 673d 2265 6e22 3e43 7572 7265 6e74  ang="en">Current
+00001210: 6c79 2c20 7468 6520 6368 6f69 6365 2069  ly, the choice i
+00001220: 7320 6c69 6d69 7465 6420 746f 2074 6865  s limited to the
+00001230: 2063 7573 746f 6d5f 696e 666f 2065 6c65   custom_info ele
+00001240: 6d65 6e74 2e3c 2f64 6f63 756d 656e 7461  ment.</documenta
+00001250: 7469 6f6e 3e0a 2020 2020 2020 2020 3c2f  tion>.        </
+00001260: 616e 6e6f 7461 7469 6f6e 3e0a 2020 2020  annotation>.    
+00001270: 2020 2020 3c63 686f 6963 653e 0a20 2020      <choice>.   
+00001280: 2020 2020 2020 2020 203c 656c 656d 656e           <elemen
+00001290: 7420 6e61 6d65 3d22 6375 7374 6f6d 5f69  t name="custom_i
+000012a0: 6e66 6f22 2074 7970 653d 2261 6e79 5479  nfo" type="anyTy
+000012b0: 7065 2220 2f3e 0a20 2020 2020 2020 203c  pe" />.        <
+000012c0: 2f63 686f 6963 653e 0a20 2020 203c 2f67  /choice>.    </g
+000012d0: 726f 7570 3e0a 2020 2020 0a3c 2f73 6368  roup>.    .</sch
+000012e0: 656d 613e 0a                             ema>.
```

### Comparing `FlowKit-1.0.1/flowkit/_resources/Gating-ML.v2.0.xsd` & `FlowKit-1.1.0/src/flowkit/_resources/Gating-ML.v2.0.xsd`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text, with CRLF line terminators*

 * *Files 13% similar despite different names*

```diff
@@ -1,735 +1,718 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
-00000020: 462d 3822 3f3e 0d0a 0d0a 3c73 6368 656d  F-8"?>....<schem
-00000030: 6120 786d 6c6e 733d 2268 7474 703a 2f2f  a xmlns="http://
-00000040: 7777 772e 7733 2e6f 7267 2f32 3030 312f  www.w3.org/2001/
-00000050: 584d 4c53 6368 656d 6122 0d0a 2020 2020  XMLSchema"..    
-00000060: 786d 6c6e 733a 6761 7469 6e67 3d22 6874  xmlns:gating="ht
-00000070: 7470 3a2f 2f77 7777 2e69 7361 632d 6e65  tp://www.isac-ne
-00000080: 742e 6f72 672f 7374 642f 4761 7469 6e67  t.org/std/Gating
-00000090: 2d4d 4c2f 7632 2e30 2f67 6174 696e 6722  -ML/v2.0/gating"
-000000a0: 0d0a 2020 2020 786d 6c6e 733a 7472 616e  ..    xmlns:tran
-000000b0: 7366 6f72 6d73 3d22 6874 7470 3a2f 2f77  sforms="http://w
-000000c0: 7777 2e69 7361 632d 6e65 742e 6f72 672f  ww.isac-net.org/
-000000d0: 7374 642f 4761 7469 6e67 2d4d 4c2f 7632  std/Gating-ML/v2
-000000e0: 2e30 2f74 7261 6e73 666f 726d 6174 696f  .0/transformatio
-000000f0: 6e73 220d 0a20 2020 2078 6d6c 6e73 3a64  ns"..    xmlns:d
-00000100: 6174 612d 7479 7065 3d22 6874 7470 3a2f  ata-type="http:/
-00000110: 2f77 7777 2e69 7361 632d 6e65 742e 6f72  /www.isac-net.or
-00000120: 672f 7374 642f 4761 7469 6e67 2d4d 4c2f  g/std/Gating-ML/
-00000130: 7632 2e30 2f64 6174 6174 7970 6573 220d  v2.0/datatypes".
-00000140: 0a20 2020 2074 6172 6765 744e 616d 6573  .    targetNames
-00000150: 7061 6365 3d22 6874 7470 3a2f 2f77 7777  pace="http://www
-00000160: 2e69 7361 632d 6e65 742e 6f72 672f 7374  .isac-net.org/st
-00000170: 642f 4761 7469 6e67 2d4d 4c2f 7632 2e30  d/Gating-ML/v2.0
-00000180: 2f67 6174 696e 6722 0d0a 2020 2020 656c  /gating"..    el
-00000190: 656d 656e 7446 6f72 6d44 6566 6175 6c74  ementFormDefault
-000001a0: 3d22 7175 616c 6966 6965 6422 2061 7474  ="qualified" att
-000001b0: 7269 6275 7465 466f 726d 4465 6661 756c  ributeFormDefaul
-000001c0: 743d 2271 7561 6c69 6669 6564 2220 7665  t="qualified" ve
-000001d0: 7273 696f 6e3d 2232 2e30 2e31 3231 3230  rsion="2.0.12120
-000001e0: 3722 3e0d 0a0d 0a20 2020 203c 696d 706f  7">....    <impo
-000001f0: 7274 206e 616d 6573 7061 6365 3d22 6874  rt namespace="ht
-00000200: 7470 3a2f 2f77 7777 2e69 7361 632d 6e65  tp://www.isac-ne
-00000210: 742e 6f72 672f 7374 642f 4761 7469 6e67  t.org/std/Gating
-00000220: 2d4d 4c2f 7632 2e30 2f74 7261 6e73 666f  -ML/v2.0/transfo
-00000230: 726d 6174 696f 6e73 2220 7363 6865 6d61  rmations" schema
-00000240: 4c6f 6361 7469 6f6e 3d22 5472 616e 7366  Location="Transf
-00000250: 6f72 6d61 7469 6f6e 732e 7632 2e30 2e78  ormations.v2.0.x
-00000260: 7364 2220 2f3e 0d0a 2020 2020 3c69 6d70  sd" />..    <imp
-00000270: 6f72 7420 6e61 6d65 7370 6163 653d 2268  ort namespace="h
-00000280: 7474 703a 2f2f 7777 772e 6973 6163 2d6e  ttp://www.isac-n
-00000290: 6574 2e6f 7267 2f73 7464 2f47 6174 696e  et.org/std/Gatin
-000002a0: 672d 4d4c 2f76 322e 302f 6461 7461 7479  g-ML/v2.0/dataty
-000002b0: 7065 7322 2073 6368 656d 614c 6f63 6174  pes" schemaLocat
-000002c0: 696f 6e3d 2244 6174 6154 7970 6573 2e76  ion="DataTypes.v
-000002d0: 322e 302e 7873 6422 202f 3e0d 0a0d 0a20  2.0.xsd" />.... 
-000002e0: 2020 203c 616e 6e6f 7461 7469 6f6e 3e0d     <annotation>.
-000002f0: 0a20 2020 2020 2020 203c 6170 7069 6e66  .        <appinf
-00000300: 6f20 736f 7572 6365 3d22 6874 7470 3a2f  o source="http:/
-00000310: 2f66 6c6f 7763 7974 2e73 662e 6e65 742f  /flowcyt.sf.net/
-00000320: 223e 4761 7469 6e67 2d4d 4c3a 2047 6174  ">Gating-ML: Gat
-00000330: 696e 6720 4465 7363 7269 7074 696f 6e20  ing Description 
-00000340: 5370 6563 6966 6963 6174 696f 6e2e 3c2f  Specification.</
-00000350: 6170 7069 6e66 6f3e 0d0a 2020 2020 2020  appinfo>..      
-00000360: 2020 3c64 6f63 756d 656e 7461 7469 6f6e    <documentation
-00000370: 2078 6d6c 3a6c 616e 673d 2265 6e22 2073   xml:lang="en" s
-00000380: 6f75 7263 653d 2268 7474 703a 2f2f 666c  ource="http://fl
-00000390: 6f77 6379 742e 736f 7572 6365 666f 7267  owcyt.sourceforg
-000003a0: 652e 6e65 742f 223e 0d0a 2020 2020 2020  e.net/">..      
-000003b0: 2020 2020 2020 3c61 7574 686f 723e 0d0a        <author>..
-000003c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003d0: 3c6e 616d 653e 4a6f 7365 6620 5370 6964  <name>Josef Spid
-000003e0: 6c65 6e3c 2f6e 616d 653e 0d0a 2020 2020  len</name>..    
-000003f0: 2020 2020 2020 2020 2020 2020 3c65 6d61              <ema
-00000400: 696c 3e6a 7370 6964 6c65 6e40 6263 6372  il>jspidlen@bccr
-00000410: 632e 6361 3c2f 656d 6169 6c3e 0d0a 2020  c.ca</email>..  
-00000420: 2020 2020 2020 2020 2020 3c2f 6175 7468            </auth
-00000430: 6f72 3e0d 0a20 2020 2020 2020 2020 2020  or>..           
-00000440: 203c 636f 7079 7269 6768 743e 0d0a 2020   <copyright>..  
-00000450: 2020 2020 2020 2020 2020 2020 2020 436f                Co
-00000460: 7079 7269 6768 7420 2863 2920 3230 3038  pyright (c) 2008
-00000470: 2d32 3031 3420 4953 4143 2028 496e 7465  -2014 ISAC (Inte
-00000480: 726e 6174 696f 6e61 6c20 536f 6369 6574  rnational Societ
-00000490: 7920 666f 7220 4164 7661 6e63 656d 656e  y for Advancemen
-000004a0: 7420 6f66 0d0a 2020 2020 2020 2020 2020  t of..          
-000004b0: 2020 2020 2020 4379 746f 6d65 7472 7929        Cytometry)
-000004c0: 2e20 4672 6565 206f 6620 6368 6172 6765  . Free of charge
-000004d0: 2064 6973 7472 6962 7574 696f 6e20 616e   distribution an
-000004e0: 6420 7265 6164 2d6f 6e6c 7920 7573 6167  d read-only usag
-000004f0: 6520 7065 726d 6974 6564 2e20 4d6f 6469  e permited. Modi
-00000500: 6669 6361 7469 6f6e 0d0a 2020 2020 2020  fication..      
-00000510: 2020 2020 2020 2020 2020 616e 6420 616c            and al
-00000520: 6c20 6f74 6865 7220 7269 6768 7473 2072  l other rights r
-00000530: 6573 6572 7665 642e 2046 6f72 2061 6c6c  eserved. For all
-00000540: 206f 7468 6572 2075 7365 7320 706c 6561   other uses plea
-00000550: 7365 2063 6f6e 7461 6374 2049 5341 432e  se contact ISAC.
-00000560: 0d0a 2020 2020 2020 2020 2020 2020 3c2f  ..            </
-00000570: 636f 7079 7269 6768 743e 0d0a 2020 2020  copyright>..    
-00000580: 2020 2020 3c2f 646f 6375 6d65 6e74 6174      </documentat
-00000590: 696f 6e3e 0d0a 2020 2020 3c2f 616e 6e6f  ion>..    </anno
-000005a0: 7461 7469 6f6e 3e0d 0a0d 0a20 2020 203c  tation>....    <
-000005b0: 656c 656d 656e 7420 6e61 6d65 3d22 4761  element name="Ga
-000005c0: 7469 6e67 2d4d 4c22 2074 7970 653d 2267  ting-ML" type="g
-000005d0: 6174 696e 673a 4761 7469 6e67 2d4d 4c5f  ating:Gating-ML_
-000005e0: 5479 7065 2220 6964 3d22 4761 7469 6e67  Type" id="Gating
-000005f0: 2d4d 4c22 3e0d 0a20 2020 2020 2020 203c  -ML">..        <
-00000600: 616e 6e6f 7461 7469 6f6e 3e0d 0a20 2020  annotation>..   
-00000610: 2020 2020 2020 2020 203c 646f 6375 6d65           <docume
-00000620: 6e74 6174 696f 6e20 786d 6c3a 6c61 6e67  ntation xml:lang
-00000630: 3d22 656e 223e 4761 7469 6e67 2d4d 4c20  ="en">Gating-ML 
-00000640: 6973 2074 6865 206d 6169 6e20 656c 656d  is the main elem
-00000650: 656e 7420 6f66 2061 6e20 584d 4c20 636f  ent of an XML co
-00000660: 7272 6573 706f 6e64 696e 6720 746f 2074  rresponding to t
-00000670: 6869 7320 7363 6865 6d61 2e3c 2f64 6f63  his schema.</doc
-00000680: 756d 656e 7461 7469 6f6e 3e0d 0a20 2020  umentation>..   
-00000690: 2020 2020 203c 2f61 6e6e 6f74 6174 696f       </annotatio
-000006a0: 6e3e 0d0a 2020 2020 3c2f 656c 656d 656e  n>..    </elemen
-000006b0: 743e 0d0a 0d0a 2020 2020 3c67 726f 7570  t>....    <group
-000006c0: 206e 616d 653d 2247 6174 6573 5f47 726f   name="Gates_Gro
-000006d0: 7570 223e 0d0a 2020 2020 2020 2020 3c61  up">..        <a
-000006e0: 6e6e 6f74 6174 696f 6e3e 0d0a 2020 2020  nnotation>..    
-000006f0: 2020 2020 2020 2020 3c64 6f63 756d 656e          <documen
-00000700: 7461 7469 6f6e 2078 6d6c 3a6c 616e 673d  tation xml:lang=
-00000710: 2265 6e22 3e54 6865 2067 726f 7570 2069  "en">The group i
-00000720: 6e63 6c75 6465 7320 6120 6368 6f69 6365  ncludes a choice
-00000730: 2066 726f 6d20 616c 6c20 7468 6520 7479   from all the ty
-00000740: 7065 7320 6f66 2067 6174 6573 2e3c 2f64  pes of gates.</d
-00000750: 6f63 756d 656e 7461 7469 6f6e 3e0d 0a20  ocumentation>.. 
-00000760: 2020 2020 2020 203c 2f61 6e6e 6f74 6174         </annotat
-00000770: 696f 6e3e 0d0a 2020 2020 2020 2020 3c63  ion>..        <c
-00000780: 686f 6963 653e 0d0a 2020 2020 2020 2020  hoice>..        
-00000790: 2020 2020 3c65 6c65 6d65 6e74 206e 616d      <element nam
-000007a0: 653d 2252 6563 7461 6e67 6c65 4761 7465  e="RectangleGate
-000007b0: 2220 7479 7065 3d22 6761 7469 6e67 3a52  " type="gating:R
-000007c0: 6563 7461 6e67 6c65 4761 7465 5f54 7970  ectangleGate_Typ
-000007d0: 6522 202f 3e0d 0a20 2020 2020 2020 2020  e" />..         
-000007e0: 2020 203c 656c 656d 656e 7420 6e61 6d65     <element name
-000007f0: 3d22 506f 6c79 676f 6e47 6174 6522 2074  ="PolygonGate" t
-00000800: 7970 653d 2267 6174 696e 673a 506f 6c79  ype="gating:Poly
-00000810: 676f 6e47 6174 655f 5479 7065 2220 2f3e  gonGate_Type" />
-00000820: 0d0a 2020 2020 2020 2020 2020 2020 3c65  ..            <e
-00000830: 6c65 6d65 6e74 206e 616d 653d 2245 6c6c  lement name="Ell
-00000840: 6970 736f 6964 4761 7465 2220 7479 7065  ipsoidGate" type
-00000850: 3d22 6761 7469 6e67 3a45 6c6c 6970 736f  ="gating:Ellipso
-00000860: 6964 4761 7465 5f54 7970 6522 202f 3e0d  idGate_Type" />.
-00000870: 0a20 2020 2020 2020 2020 2020 203c 656c  .            <el
-00000880: 656d 656e 7420 6e61 6d65 3d22 426f 6f6c  ement name="Bool
-00000890: 6561 6e47 6174 6522 2074 7970 653d 2267  eanGate" type="g
-000008a0: 6174 696e 673a 426f 6f6c 6561 6e47 6174  ating:BooleanGat
-000008b0: 655f 5479 7065 2220 2f3e 0d0a 2020 2020  e_Type" />..    
-000008c0: 2020 2020 2020 2020 3c65 6c65 6d65 6e74          <element
-000008d0: 206e 616d 653d 2251 7561 6472 616e 7447   name="QuadrantG
-000008e0: 6174 6522 2074 7970 653d 2267 6174 696e  ate" type="gatin
-000008f0: 673a 5175 6164 7261 6e74 4761 7465 5f54  g:QuadrantGate_T
-00000900: 7970 6522 202f 3e0d 0a20 2020 2020 2020  ype" />..       
-00000910: 203c 2f63 686f 6963 653e 0d0a 2020 2020   </choice>..    
-00000920: 3c2f 6772 6f75 703e 0d0a 0d0a 2020 2020  </group>....    
-00000930: 3c63 6f6d 706c 6578 5479 7065 206e 616d  <complexType nam
-00000940: 653d 2247 6174 696e 672d 4d4c 5f54 7970  e="Gating-ML_Typ
-00000950: 6522 3e0d 0a20 2020 2020 2020 203c 7365  e">..        <se
-00000960: 7175 656e 6365 206d 696e 4f63 6375 7273  quence minOccurs
-00000970: 3d22 3122 206d 6178 4f63 6375 7273 3d22  ="1" maxOccurs="
-00000980: 756e 626f 756e 6465 6422 3e0d 0a20 2020  unbounded">..   
-00000990: 2020 2020 2020 2020 203c 6368 6f69 6365           <choice
-000009a0: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
-000009b0: 2020 203c 6772 6f75 7020 7265 663d 2267     <group ref="g
-000009c0: 6174 696e 673a 4761 7465 735f 4772 6f75  ating:Gates_Grou
-000009d0: 7022 202f 3e0d 0a20 2020 2020 2020 2020  p" />..         
-000009e0: 2020 2020 2020 203c 6772 6f75 7020 7265         <group re
-000009f0: 663d 2274 7261 6e73 666f 726d 733a 5472  f="transforms:Tr
-00000a00: 616e 7366 6f72 6d61 7469 6f6e 5f47 726f  ansformation_Gro
-00000a10: 7570 2220 2f3e 0d0a 2020 2020 2020 2020  up" />..        
-00000a20: 2020 2020 2020 2020 3c67 726f 7570 2072          <group r
-00000a30: 6566 3d22 7472 616e 7366 6f72 6d73 3a53  ef="transforms:S
-00000a40: 7065 6374 7275 6d4d 6174 7269 785f 4772  pectrumMatrix_Gr
-00000a50: 6f75 7022 202f 3e0d 0a20 2020 2020 2020  oup" />..       
-00000a60: 2020 2020 2020 2020 203c 6772 6f75 7020           <group 
-00000a70: 7265 663d 2264 6174 612d 7479 7065 3a43  ref="data-type:C
-00000a80: 7573 746f 6d5f 4772 6f75 7022 202f 3e0d  ustom_Group" />.
-00000a90: 0a20 2020 2020 2020 2020 2020 203c 2f63  .            </c
-00000aa0: 686f 6963 653e 0d0a 2020 2020 2020 2020  hoice>..        
-00000ab0: 3c2f 7365 7175 656e 6365 3e0d 0a20 2020  </sequence>..   
-00000ac0: 203c 2f63 6f6d 706c 6578 5479 7065 3e0d   </complexType>.
-00000ad0: 0a0d 0a20 2020 203c 636f 6d70 6c65 7854  ...    <complexT
-00000ae0: 7970 6520 6e61 6d65 3d22 4162 7374 7261  ype name="Abstra
-00000af0: 6374 4761 7465 5f54 7970 6522 2061 6273  ctGate_Type" abs
-00000b00: 7472 6163 743d 2274 7275 6522 3e0d 0a20  tract="true">.. 
-00000b10: 2020 2020 2020 203c 616e 6e6f 7461 7469         <annotati
-00000b20: 6f6e 3e0d 0a20 2020 2020 2020 2020 2020  on>..           
-00000b30: 203c 646f 6375 6d65 6e74 6174 696f 6e20   <documentation 
-00000b40: 786d 6c3a 6c61 6e67 3d22 656e 223e 4162  xml:lang="en">Ab
-00000b50: 7374 7261 6374 2074 7970 6520 746f 2062  stract type to b
-00000b60: 6520 7573 6564 2061 7320 6120 636f 6d6d  e used as a comm
-00000b70: 6f6e 2070 6172 656e 7420 6f66 2061 6c6c  on parent of all
-00000b80: 2074 7970 6573 206f 6620 6761 7465 732e   types of gates.
-00000b90: 3c2f 646f 6375 6d65 6e74 6174 696f 6e3e  </documentation>
-00000ba0: 0d0a 2020 2020 2020 2020 3c2f 616e 6e6f  ..        </anno
-00000bb0: 7461 7469 6f6e 3e0d 0a20 2020 2020 2020  tation>..       
-00000bc0: 203c 6772 6f75 7020 7265 663d 2264 6174   <group ref="dat
-00000bd0: 612d 7479 7065 3a43 7573 746f 6d5f 4772  a-type:Custom_Gr
-00000be0: 6f75 7022 206d 696e 4f63 6375 7273 3d22  oup" minOccurs="
-00000bf0: 3022 202f 3e0d 0a20 2020 2020 2020 203c  0" />..        <
-00000c00: 6174 7472 6962 7574 6520 6e61 6d65 3d22  attribute name="
-00000c10: 6964 2220 7479 7065 3d22 4944 2220 7573  id" type="ID" us
-00000c20: 653d 2272 6571 7569 7265 6422 2069 643d  e="required" id=
-00000c30: 2269 6422 202f 3e0d 0a20 2020 2020 2020  "id" />..       
-00000c40: 203c 6174 7472 6962 7574 6520 6e61 6d65   <attribute name
-00000c50: 3d22 7061 7265 6e74 5f69 6422 2074 7970  ="parent_id" typ
-00000c60: 653d 2249 4452 4546 2220 7573 653d 226f  e="IDREF" use="o
-00000c70: 7074 696f 6e61 6c22 2069 643d 2270 6172  ptional" id="par
-00000c80: 656e 745f 6964 2220 2f3e 0d0a 2020 2020  ent_id" />..    
-00000c90: 2020 2020 3c61 6e79 4174 7472 6962 7574      <anyAttribut
-00000ca0: 6520 7072 6f63 6573 7343 6f6e 7465 6e74  e processContent
-00000cb0: 733d 2273 6b69 7022 2f3e 0d0a 2020 2020  s="skip"/>..    
-00000cc0: 3c2f 636f 6d70 6c65 7854 7970 653e 0d0a  </complexType>..
-00000cd0: 0d0a 2020 2020 3c63 6f6d 706c 6578 5479  ..    <complexTy
-00000ce0: 7065 206e 616d 653d 2251 7561 6472 616e  pe name="Quadran
-00000cf0: 7447 6174 655f 5479 7065 223e 0d0a 2020  tGate_Type">..  
-00000d00: 2020 2020 2020 3c63 6f6d 706c 6578 436f        <complexCo
-00000d10: 6e74 656e 743e 0d0a 2020 2020 2020 2020  ntent>..        
-00000d20: 2020 2020 3c65 7874 656e 7369 6f6e 2062      <extension b
-00000d30: 6173 653d 2267 6174 696e 673a 4162 7374  ase="gating:Abst
-00000d40: 7261 6374 4761 7465 5f54 7970 6522 3e0d  ractGate_Type">.
-00000d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000d60: 203c 7365 7175 656e 6365 3e0d 0a20 2020   <sequence>..   
-00000d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d80: 203c 656c 656d 656e 7420 6e61 6d65 3d22   <element name="
-00000d90: 6469 7669 6465 7222 2074 7970 653d 2267  divider" type="g
-00000da0: 6174 696e 673a 5175 6164 7261 6e74 4761  ating:QuadrantGa
-00000db0: 7465 4469 7669 6465 725f 5479 7065 2220  teDivider_Type" 
-00000dc0: 6d61 784f 6363 7572 733d 2275 6e62 6f75  maxOccurs="unbou
-00000dd0: 6e64 6564 2220 6964 3d22 6469 7669 6465  nded" id="divide
-00000de0: 7222 202f 3e0d 0a20 2020 2020 2020 2020  r" />..         
-00000df0: 2020 2020 2020 2020 2020 203c 656c 656d             <elem
-00000e00: 656e 7420 6e61 6d65 3d22 5175 6164 7261  ent name="Quadra
-00000e10: 6e74 2220 7479 7065 3d22 6761 7469 6e67  nt" type="gating
-00000e20: 3a51 7561 6472 616e 745f 5479 7065 2220  :Quadrant_Type" 
-00000e30: 6d61 784f 6363 7572 733d 2275 6e62 6f75  maxOccurs="unbou
-00000e40: 6e64 6564 2220 6964 3d22 7175 6164 7261  nded" id="quadra
-00000e50: 6e74 2220 2f3e 0d0a 2020 2020 2020 2020  nt" />..        
-00000e60: 2020 2020 2020 2020 3c2f 7365 7175 656e          </sequen
-00000e70: 6365 3e0d 0a20 2020 2020 2020 2020 2020  ce>..           
-00000e80: 203c 2f65 7874 656e 7369 6f6e 3e0d 0a20   </extension>.. 
-00000e90: 2020 2020 2020 203c 2f63 6f6d 706c 6578         </complex
-00000ea0: 436f 6e74 656e 743e 0d0a 2020 2020 3c2f  Content>..    </
-00000eb0: 636f 6d70 6c65 7854 7970 653e 0d0a 0d0a  complexType>....
-00000ec0: 2020 2020 3c63 6f6d 706c 6578 5479 7065      <complexType
-00000ed0: 206e 616d 653d 2251 7561 6472 616e 7447   name="QuadrantG
-00000ee0: 6174 6544 6976 6964 6572 5f54 7970 6522  ateDivider_Type"
-00000ef0: 3e0d 0a20 2020 2020 2020 203c 636f 6d70  >..        <comp
-00000f00: 6c65 7843 6f6e 7465 6e74 3e0d 0a20 2020  lexContent>..   
-00000f10: 2020 2020 2020 2020 203c 6578 7465 6e73           <extens
-00000f20: 696f 6e20 6261 7365 3d22 6761 7469 6e67  ion base="gating
-00000f30: 3a44 696d 656e 7369 6f6e 5f54 7970 6522  :Dimension_Type"
-00000f40: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
-00000f50: 2020 203c 7365 7175 656e 6365 3e0d 0a20     <sequence>.. 
-00000f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f70: 2020 203c 656c 656d 656e 7420 6e61 6d65     <element name
-00000f80: 3d22 7661 6c75 6522 2074 7970 653d 2266  ="value" type="f
-00000f90: 6c6f 6174 2220 6d61 784f 6363 7572 733d  loat" maxOccurs=
-00000fa0: 2275 6e62 6f75 6e64 6564 2220 6964 3d22  "unbounded" id="
-00000fb0: 6469 7669 6465 7276 616c 7565 2220 2f3e  dividervalue" />
-00000fc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000fd0: 2020 3c2f 7365 7175 656e 6365 3e0d 0a20    </sequence>.. 
-00000fe0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000ff0: 6174 7472 6962 7574 6520 6e61 6d65 3d22  attribute name="
-00001000: 6964 2220 7479 7065 3d22 4944 2220 6964  id" type="ID" id
-00001010: 3d22 6469 7669 6465 725f 6964 2220 7573  ="divider_id" us
-00001020: 653d 2272 6571 7569 7265 6422 202f 3e0d  e="required" />.
-00001030: 0a20 2020 2020 2020 2020 2020 203c 2f65  .            </e
-00001040: 7874 656e 7369 6f6e 3e0d 0a20 2020 2020  xtension>..     
-00001050: 2020 203c 2f63 6f6d 706c 6578 436f 6e74     </complexCont
-00001060: 656e 743e 0d0a 2020 2020 3c2f 636f 6d70  ent>..    </comp
-00001070: 6c65 7854 7970 653e 0d0a 0d0a 2020 2020  lexType>....    
-00001080: 3c63 6f6d 706c 6578 5479 7065 206e 616d  <complexType nam
-00001090: 653d 2251 7561 6472 616e 745f 5479 7065  e="Quadrant_Type
-000010a0: 223e 0d0a 2020 2020 2020 2020 3c73 6571  ">..        <seq
-000010b0: 7565 6e63 653e 0d0a 2020 2020 2020 2020  uence>..        
-000010c0: 2020 2020 3c65 6c65 6d65 6e74 206e 616d      <element nam
-000010d0: 653d 2270 6f73 6974 696f 6e22 206d 6178  e="position" max
-000010e0: 4f63 6375 7273 3d22 756e 626f 756e 6465  Occurs="unbounde
-000010f0: 6422 2069 643d 2270 6f73 6974 696f 6e22  d" id="position"
-00001100: 2074 7970 653d 2267 6174 696e 673a 506f   type="gating:Po
-00001110: 7369 7469 6f6e 5f54 7970 6522 202f 3e0d  sition_Type" />.
-00001120: 0a20 2020 2020 2020 203c 2f73 6571 7565  .        </seque
-00001130: 6e63 653e 0d0a 2020 2020 2020 2020 3c61  nce>..        <a
-00001140: 7474 7269 6275 7465 206e 616d 653d 2269  ttribute name="i
-00001150: 6422 2074 7970 653d 2249 4422 2075 7365  d" type="ID" use
-00001160: 3d22 7265 7175 6972 6564 2220 6964 3d22  ="required" id="
-00001170: 7175 6164 7261 6e74 5f69 6422 202f 3e0d  quadrant_id" />.
-00001180: 0a20 2020 203c 2f63 6f6d 706c 6578 5479  .    </complexTy
-00001190: 7065 3e0d 0a0d 0a20 2020 203c 636f 6d70  pe>....    <comp
-000011a0: 6c65 7854 7970 6520 6e61 6d65 3d22 506f  lexType name="Po
-000011b0: 7369 7469 6f6e 5f54 7970 6522 3e0d 0a20  sition_Type">.. 
-000011c0: 2020 2020 2020 203c 6174 7472 6962 7574         <attribut
-000011d0: 6520 6e61 6d65 3d22 6469 7669 6465 725f  e name="divider_
-000011e0: 7265 6622 2075 7365 3d22 7265 7175 6972  ref" use="requir
-000011f0: 6564 2220 7479 7065 3d22 4944 5245 4622  ed" type="IDREF"
-00001200: 2069 643d 2264 6976 6964 6572 5f72 6566   id="divider_ref
-00001210: 2220 2f3e 0d0a 2020 2020 2020 2020 3c61  " />..        <a
-00001220: 7474 7269 6275 7465 206e 616d 653d 226c  ttribute name="l
-00001230: 6f63 6174 696f 6e22 2075 7365 3d22 7265  ocation" use="re
-00001240: 7175 6972 6564 2220 7479 7065 3d22 6461  quired" type="da
-00001250: 7461 2d74 7970 653a 466c 6f61 7436 345f  ta-type:Float64_
-00001260: 5479 7065 2220 6964 3d22 6c6f 6361 7469  Type" id="locati
-00001270: 6f6e 5f76 616c 7565 2220 2f3e 0d0a 2020  on_value" />..  
-00001280: 2020 3c2f 636f 6d70 6c65 7854 7970 653e    </complexType>
-00001290: 0d0a 0d0a 2020 2020 3c63 6f6d 706c 6578  ....    <complex
-000012a0: 5479 7065 206e 616d 653d 2252 6563 7461  Type name="Recta
-000012b0: 6e67 6c65 4761 7465 5f54 7970 6522 3e0d  ngleGate_Type">.
-000012c0: 0a20 2020 2020 2020 203c 636f 6d70 6c65  .        <comple
-000012d0: 7843 6f6e 7465 6e74 3e0d 0a20 2020 2020  xContent>..     
-000012e0: 2020 2020 2020 203c 6578 7465 6e73 696f         <extensio
-000012f0: 6e20 6261 7365 3d22 6761 7469 6e67 3a41  n base="gating:A
-00001300: 6273 7472 6163 7447 6174 655f 5479 7065  bstractGate_Type
-00001310: 223e 0d0a 2020 2020 2020 2020 2020 2020  ">..            
-00001320: 2020 2020 3c73 6571 7565 6e63 653e 0d0a      <sequence>..
-00001330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001340: 2020 2020 3c65 6c65 6d65 6e74 206e 616d      <element nam
-00001350: 653d 2264 696d 656e 7369 6f6e 2220 7479  e="dimension" ty
-00001360: 7065 3d22 6761 7469 6e67 3a52 6563 7461  pe="gating:Recta
-00001370: 6e67 6c65 4761 7465 4469 6d65 6e73 696f  ngleGateDimensio
-00001380: 6e5f 5479 7065 2220 6d61 784f 6363 7572  n_Type" maxOccur
-00001390: 733d 2275 6e62 6f75 6e64 6564 2220 6964  s="unbounded" id
-000013a0: 3d22 6469 6d65 6e73 696f 6e22 202f 3e0d  ="dimension" />.
-000013b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000013c0: 203c 2f73 6571 7565 6e63 653e 0d0a 2020   </sequence>..  
-000013d0: 2020 2020 2020 2020 2020 3c2f 6578 7465            </exte
-000013e0: 6e73 696f 6e3e 0d0a 2020 2020 2020 2020  nsion>..        
-000013f0: 3c2f 636f 6d70 6c65 7843 6f6e 7465 6e74  </complexContent
-00001400: 3e0d 0a20 2020 203c 2f63 6f6d 706c 6578  >..    </complex
-00001410: 5479 7065 3e0d 0a0d 0a20 2020 203c 636f  Type>....    <co
-00001420: 6d70 6c65 7854 7970 6520 6e61 6d65 3d22  mplexType name="
-00001430: 506f 6c79 676f 6e47 6174 655f 5479 7065  PolygonGate_Type
-00001440: 223e 0d0a 2020 2020 2020 2020 3c63 6f6d  ">..        <com
-00001450: 706c 6578 436f 6e74 656e 743e 0d0a 2020  plexContent>..  
-00001460: 2020 2020 2020 2020 2020 3c65 7874 656e            <exten
-00001470: 7369 6f6e 2062 6173 653d 2267 6174 696e  sion base="gatin
-00001480: 673a 4162 7374 7261 6374 4761 7465 5f54  g:AbstractGate_T
-00001490: 7970 6522 3e0d 0a20 2020 2020 2020 2020  ype">..         
-000014a0: 2020 2020 2020 203c 7365 7175 656e 6365         <sequence
-000014b0: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
-000014c0: 2020 2020 2020 203c 656c 656d 656e 7420         <element 
-000014d0: 6e61 6d65 3d22 6469 6d65 6e73 696f 6e22  name="dimension"
-000014e0: 2074 7970 653d 2267 6174 696e 673a 4469   type="gating:Di
-000014f0: 6d65 6e73 696f 6e5f 5479 7065 2220 6d69  mension_Type" mi
-00001500: 6e4f 6363 7572 733d 2232 2220 6d61 784f  nOccurs="2" maxO
-00001510: 6363 7572 733d 2232 2220 2f3e 0d0a 2020  ccurs="2" />..  
-00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001530: 2020 3c65 6c65 6d65 6e74 206e 616d 653d    <element name=
-00001540: 2276 6572 7465 7822 2074 7970 653d 2267  "vertex" type="g
-00001550: 6174 696e 673a 506f 696e 7432 445f 5479  ating:Point2D_Ty
-00001560: 7065 2220 6d69 6e4f 6363 7572 733d 2233  pe" minOccurs="3
-00001570: 2220 6d61 784f 6363 7572 733d 2275 6e62  " maxOccurs="unb
-00001580: 6f75 6e64 6564 2220 2f3e 0d0a 2020 2020  ounded" />..    
-00001590: 2020 2020 2020 2020 2020 2020 3c2f 7365              </se
-000015a0: 7175 656e 6365 3e0d 0a20 2020 2020 2020  quence>..       
-000015b0: 2020 2020 203c 2f65 7874 656e 7369 6f6e       </extension
-000015c0: 3e0d 0a20 2020 2020 2020 203c 2f63 6f6d  >..        </com
-000015d0: 706c 6578 436f 6e74 656e 743e 0d0a 2020  plexContent>..  
-000015e0: 2020 3c2f 636f 6d70 6c65 7854 7970 653e    </complexType>
-000015f0: 0d0a 0d0a 2020 2020 3c63 6f6d 706c 6578  ....    <complex
-00001600: 5479 7065 206e 616d 653d 2245 6c6c 6970  Type name="Ellip
-00001610: 736f 6964 4761 7465 5f54 7970 6522 3e0d  soidGate_Type">.
-00001620: 0a20 2020 2020 2020 203c 636f 6d70 6c65  .        <comple
-00001630: 7843 6f6e 7465 6e74 3e0d 0a20 2020 2020  xContent>..     
-00001640: 2020 2020 2020 203c 6578 7465 6e73 696f         <extensio
-00001650: 6e20 6261 7365 3d22 6761 7469 6e67 3a41  n base="gating:A
-00001660: 6273 7472 6163 7447 6174 655f 5479 7065  bstractGate_Type
-00001670: 223e 0d0a 2020 2020 2020 2020 2020 2020  ">..            
-00001680: 2020 2020 3c73 6571 7565 6e63 653e 0d0a      <sequence>..
-00001690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016a0: 2020 2020 3c65 6c65 6d65 6e74 206e 616d      <element nam
-000016b0: 653d 2264 696d 656e 7369 6f6e 2220 7479  e="dimension" ty
-000016c0: 7065 3d22 6761 7469 6e67 3a44 696d 656e  pe="gating:Dimen
-000016d0: 7369 6f6e 5f54 7970 6522 206d 696e 4f63  sion_Type" minOc
-000016e0: 6375 7273 3d22 3222 206d 6178 4f63 6375  curs="2" maxOccu
-000016f0: 7273 3d22 756e 626f 756e 6465 6422 202f  rs="unbounded" /
-00001700: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
-00001710: 2020 2020 2020 203c 656c 656d 656e 7420         <element 
-00001720: 6e61 6d65 3d22 6d65 616e 2220 7479 7065  name="mean" type
-00001730: 3d22 6761 7469 6e67 3a50 6f69 6e74 5844  ="gating:PointXD
-00001740: 5f54 7970 6522 206d 696e 4f63 6375 7273  _Type" minOccurs
-00001750: 3d22 3122 206d 6178 4f63 6375 7273 3d22  ="1" maxOccurs="
-00001760: 3122 202f 3e0d 0a20 2020 2020 2020 2020  1" />..         
-00001770: 2020 2020 2020 2020 2020 203c 656c 656d             <elem
-00001780: 656e 7420 6e61 6d65 3d22 636f 7661 7269  ent name="covari
-00001790: 616e 6365 4d61 7472 6978 2220 7479 7065  anceMatrix" type
-000017a0: 3d22 6761 7469 6e67 3a4d 6174 7269 785f  ="gating:Matrix_
-000017b0: 5479 7065 2220 6d69 6e4f 6363 7572 733d  Type" minOccurs=
-000017c0: 2231 2220 6d61 784f 6363 7572 733d 2231  "1" maxOccurs="1
-000017d0: 2220 2f3e 0d0a 2020 2020 2020 2020 2020  " />..          
-000017e0: 2020 2020 2020 2020 2020 3c65 6c65 6d65            <eleme
-000017f0: 6e74 206e 616d 653d 2264 6973 7461 6e63  nt name="distanc
-00001800: 6553 7175 6172 6522 2074 7970 653d 2264  eSquare" type="d
-00001810: 6174 612d 7479 7065 3a55 5661 6c75 6541  ata-type:UValueA
-00001820: 7474 7269 6275 7465 5f54 7970 6522 206d  ttribute_Type" m
-00001830: 696e 4f63 6375 7273 3d22 3122 206d 6178  inOccurs="1" max
-00001840: 4f63 6375 7273 3d22 3122 202f 3e0d 0a20  Occurs="1" />.. 
-00001850: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001860: 2f73 6571 7565 6e63 653e 0d0a 2020 2020  /sequence>..    
-00001870: 2020 2020 2020 2020 3c2f 6578 7465 6e73          </extens
-00001880: 696f 6e3e 0d0a 2020 2020 2020 2020 3c2f  ion>..        </
-00001890: 636f 6d70 6c65 7843 6f6e 7465 6e74 3e0d  complexContent>.
-000018a0: 0a20 2020 203c 2f63 6f6d 706c 6578 5479  .    </complexTy
-000018b0: 7065 3e0d 0a0d 0a20 2020 203c 636f 6d70  pe>....    <comp
-000018c0: 6c65 7854 7970 6520 6e61 6d65 3d22 426f  lexType name="Bo
-000018d0: 6f6c 6561 6e47 6174 655f 5479 7065 223e  oleanGate_Type">
-000018e0: 0d0a 2020 2020 2020 2020 3c63 6f6d 706c  ..        <compl
-000018f0: 6578 436f 6e74 656e 743e 0d0a 2020 2020  exContent>..    
-00001900: 2020 2020 2020 2020 3c65 7874 656e 7369          <extensi
-00001910: 6f6e 2062 6173 653d 2267 6174 696e 673a  on base="gating:
-00001920: 4162 7374 7261 6374 4761 7465 5f54 7970  AbstractGate_Typ
-00001930: 6522 3e0d 0a20 2020 2020 2020 2020 2020  e">..           
-00001940: 2020 2020 203c 7365 7175 656e 6365 3e0d       <sequence>.
-00001950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001960: 2020 2020 203c 6368 6f69 6365 3e0d 0a20       <choice>.. 
-00001970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001980: 2020 2020 2020 203c 656c 656d 656e 7420         <element 
-00001990: 6e61 6d65 3d22 616e 6422 2074 7970 653d  name="and" type=
-000019a0: 2267 6174 696e 673a 5477 6f41 6e64 4d6f  "gating:TwoAndMo
-000019b0: 7265 4f70 6572 616e 6473 5f42 6f6f 6c47  reOperands_BoolG
-000019c0: 6174 655f 5479 7065 2220 6964 3d22 616e  ate_Type" id="an
-000019d0: 6422 202f 3e0d 0a20 2020 2020 2020 2020  d" />..         
-000019e0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000019f0: 656c 656d 656e 7420 6e61 6d65 3d22 6f72  element name="or
-00001a00: 2220 7479 7065 3d22 6761 7469 6e67 3a54  " type="gating:T
-00001a10: 776f 416e 644d 6f72 654f 7065 7261 6e64  woAndMoreOperand
-00001a20: 735f 426f 6f6c 4761 7465 5f54 7970 6522  s_BoolGate_Type"
-00001a30: 2069 643d 226f 7222 202f 3e0d 0a20 2020   id="or" />..   
-00001a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a50: 2020 2020 203c 656c 656d 656e 7420 6e61       <element na
-00001a60: 6d65 3d22 6e6f 7422 2074 7970 653d 2267  me="not" type="g
-00001a70: 6174 696e 673a 4f6e 654f 7065 7261 6e64  ating:OneOperand
-00001a80: 5f42 6f6f 6c47 6174 655f 5479 7065 2220  _BoolGate_Type" 
-00001a90: 6964 3d22 6e6f 7422 202f 3e0d 0a20 2020  id="not" />..   
-00001aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ab0: 203c 2f63 686f 6963 653e 0d0a 2020 2020   </choice>..    
-00001ac0: 2020 2020 2020 2020 2020 2020 3c2f 7365              </se
-00001ad0: 7175 656e 6365 3e0d 0a20 2020 2020 2020  quence>..       
-00001ae0: 2020 2020 203c 2f65 7874 656e 7369 6f6e       </extension
-00001af0: 3e0d 0a20 2020 2020 2020 203c 2f63 6f6d  >..        </com
-00001b00: 706c 6578 436f 6e74 656e 743e 0d0a 2020  plexContent>..  
-00001b10: 2020 3c2f 636f 6d70 6c65 7854 7970 653e    </complexType>
-00001b20: 0d0a 0d0a 2020 2020 3c63 6f6d 706c 6578  ....    <complex
-00001b30: 5479 7065 206e 616d 653d 2244 696d 656e  Type name="Dimen
-00001b40: 7369 6f6e 5f54 7970 6522 3e0d 0a20 2020  sion_Type">..   
-00001b50: 2020 2020 203c 616e 6e6f 7461 7469 6f6e       <annotation
-00001b60: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
-00001b70: 646f 6375 6d65 6e74 6174 696f 6e20 786d  documentation xm
-00001b80: 6c3a 6c61 6e67 3d22 656e 223e 4643 5320  l:lang="en">FCS 
-00001b90: 6469 6d65 6e73 696f 6e20 706c 7573 2074  dimension plus t
-00001ba0: 7261 6e73 666f 726d 6174 696f 6e20 286f  ransformation (o
-00001bb0: 7074 696f 6e61 6c29 2061 6e64 2063 6f6d  ptional) and com
-00001bc0: 7065 6e73 6174 696f 6e20 7265 6665 7265  pensation refere
-00001bd0: 6e63 6573 2028 7265 7175 6972 6564 3a20  nces (required: 
-00001be0: 6368 6f69 6365 2027 756e 636f 6d70 656e  choice 'uncompen
-00001bf0: 7361 7465 6427 2c20 2746 4353 2720 6f72  sated', 'FCS' or
-00001c00: 2069 6420 6f66 2061 2073 7069 6c6c 6f76   id of a spillov
-00001c10: 6572 206d 6174 7269 7829 2e3c 2f64 6f63  er matrix).</doc
-00001c20: 756d 656e 7461 7469 6f6e 3e0d 0a20 2020  umentation>..   
-00001c30: 2020 2020 203c 2f61 6e6e 6f74 6174 696f       </annotatio
-00001c40: 6e3e 0d0a 2020 2020 2020 2020 3c67 726f  n>..        <gro
-00001c50: 7570 2072 6566 3d22 6461 7461 2d74 7970  up ref="data-typ
-00001c60: 653a 4469 6d65 6e73 696f 6e73 5f47 726f  e:Dimensions_Gro
-00001c70: 7570 2220 2f3e 0d0a 2020 2020 2020 2020  up" />..        
-00001c80: 3c61 7474 7269 6275 7465 206e 616d 653d  <attribute name=
-00001c90: 2274 7261 6e73 666f 726d 6174 696f 6e2d  "transformation-
-00001ca0: 7265 6622 2074 7970 653d 2249 4452 4546  ref" type="IDREF
-00001cb0: 2220 7573 653d 226f 7074 696f 6e61 6c22  " use="optional"
-00001cc0: 202f 3e0d 0a20 2020 2020 2020 203c 6174   />..        <at
-00001cd0: 7472 6962 7574 6520 6e61 6d65 3d22 636f  tribute name="co
-00001ce0: 6d70 656e 7361 7469 6f6e 2d72 6566 2220  mpensation-ref" 
-00001cf0: 7479 7065 3d22 6461 7461 2d74 7970 653a  type="data-type:
-00001d00: 4e6f 6e45 6d70 7479 5374 7269 6e67 5f54  NonEmptyString_T
-00001d10: 7970 6522 2075 7365 3d22 7265 7175 6972  ype" use="requir
-00001d20: 6564 2220 2f3e 0d0a 2020 2020 3c2f 636f  ed" />..    </co
-00001d30: 6d70 6c65 7854 7970 653e 0d0a 0d0a 2020  mplexType>....  
-00001d40: 2020 3c63 6f6d 706c 6578 5479 7065 206e    <complexType n
-00001d50: 616d 653d 2252 6563 7461 6e67 6c65 4761  ame="RectangleGa
-00001d60: 7465 4469 6d65 6e73 696f 6e5f 5479 7065  teDimension_Type
-00001d70: 223e 0d0a 2020 2020 2020 2020 3c61 6e6e  ">..        <ann
-00001d80: 6f74 6174 696f 6e3e 0d0a 2020 2020 2020  otation>..      
-00001d90: 2020 2020 2020 3c64 6f63 756d 656e 7461        <documenta
-00001da0: 7469 6f6e 3e41 2064 696d 656e 7369 6f6e  tion>A dimension
-00001db0: 2074 7970 6520 666f 7220 6120 7265 6374   type for a rect
-00001dc0: 616e 676c 6520 6761 7465 3b20 7468 6520  angle gate; the 
-00001dd0: 636f 6d6d 6f6e 2064 696d 656e 7369 6f6e  common dimension
-00001de0: 2069 7320 6578 7465 6e64 6564 2062 7920   is extended by 
-00001df0: 7468 6520 6d69 6e20 616e 6420 6d61 7820  the min and max 
-00001e00: 6174 7472 6962 7574 6573 2e20 3c2f 646f  attributes. </do
-00001e10: 6375 6d65 6e74 6174 696f 6e3e 0d0a 2020  cumentation>..  
-00001e20: 2020 2020 2020 3c2f 616e 6e6f 7461 7469        </annotati
-00001e30: 6f6e 3e0d 0a20 2020 2020 2020 203c 636f  on>..        <co
-00001e40: 6d70 6c65 7843 6f6e 7465 6e74 3e0d 0a20  mplexContent>.. 
-00001e50: 2020 2020 2020 2020 2020 203c 6578 7465             <exte
-00001e60: 6e73 696f 6e20 6261 7365 3d22 6761 7469  nsion base="gati
-00001e70: 6e67 3a44 696d 656e 7369 6f6e 5f54 7970  ng:Dimension_Typ
-00001e80: 6522 3e0d 0a20 2020 2020 2020 2020 2020  e">..           
-00001e90: 2020 2020 203c 6174 7472 6962 7574 6520       <attribute 
-00001ea0: 6e61 6d65 3d22 6d69 6e22 2074 7970 653d  name="min" type=
-00001eb0: 2264 6174 612d 7479 7065 3a46 6c6f 6174  "data-type:Float
-00001ec0: 3634 5f54 7970 6522 2075 7365 3d22 6f70  64_Type" use="op
-00001ed0: 7469 6f6e 616c 2220 6964 3d22 6d69 6e22  tional" id="min"
-00001ee0: 202f 3e0d 0a20 2020 2020 2020 2020 2020   />..           
-00001ef0: 2020 2020 203c 6174 7472 6962 7574 6520       <attribute 
-00001f00: 6e61 6d65 3d22 6d61 7822 2074 7970 653d  name="max" type=
-00001f10: 2264 6174 612d 7479 7065 3a46 6c6f 6174  "data-type:Float
-00001f20: 3634 5f54 7970 6522 2075 7365 3d22 6f70  64_Type" use="op
-00001f30: 7469 6f6e 616c 2220 6964 3d22 6d61 7822  tional" id="max"
-00001f40: 202f 3e0d 0a20 2020 2020 2020 2020 2020   />..           
-00001f50: 203c 2f65 7874 656e 7369 6f6e 3e0d 0a20   </extension>.. 
-00001f60: 2020 2020 2020 203c 2f63 6f6d 706c 6578         </complex
-00001f70: 436f 6e74 656e 743e 0d0a 2020 2020 3c2f  Content>..    </
-00001f80: 636f 6d70 6c65 7854 7970 653e 0d0a 0d0a  complexType>....
-00001f90: 2020 2020 3c63 6f6d 706c 6578 5479 7065      <complexType
-00001fa0: 206e 616d 653d 2250 6f69 6e74 5f54 7970   name="Point_Typ
-00001fb0: 6522 3e0d 0a20 2020 2020 2020 203c 616e  e">..        <an
-00001fc0: 6e6f 7461 7469 6f6e 3e0d 0a20 2020 2020  notation>..     
-00001fd0: 2020 2020 2020 203c 646f 6375 6d65 6e74         <document
-00001fe0: 6174 696f 6e3e 4120 706f 696e 7420 6973  ation>A point is
-00001ff0: 2061 2073 6571 7565 6e63 6520 6f66 2063   a sequence of c
-00002000: 6f6f 7264 696e 6174 6573 2e3c 2f64 6f63  oordinates.</doc
-00002010: 756d 656e 7461 7469 6f6e 3e0d 0a20 2020  umentation>..   
-00002020: 2020 2020 203c 2f61 6e6e 6f74 6174 696f       </annotatio
-00002030: 6e3e 0d0a 2020 2020 2020 2020 3c73 6571  n>..        <seq
-00002040: 7565 6e63 653e 0d0a 2020 2020 2020 2020  uence>..        
-00002050: 2020 2020 3c65 6c65 6d65 6e74 206e 616d      <element nam
-00002060: 653d 2263 6f6f 7264 696e 6174 6522 2074  e="coordinate" t
-00002070: 7970 653d 2264 6174 612d 7479 7065 3a56  ype="data-type:V
-00002080: 616c 7565 4174 7472 6962 7574 655f 5479  alueAttribute_Ty
-00002090: 7065 2220 6d61 784f 6363 7572 733d 2275  pe" maxOccurs="u
-000020a0: 6e62 6f75 6e64 6564 2220 6964 3d22 636f  nbounded" id="co
-000020b0: 6f72 6469 6e61 7465 2220 2f3e 0d0a 2020  ordinate" />..  
-000020c0: 2020 2020 2020 3c2f 7365 7175 656e 6365        </sequence
-000020d0: 3e0d 0a20 2020 203c 2f63 6f6d 706c 6578  >..    </complex
-000020e0: 5479 7065 3e0d 0a0d 0a20 2020 203c 636f  Type>....    <co
-000020f0: 6d70 6c65 7854 7970 6520 6e61 6d65 3d22  mplexType name="
-00002100: 506f 696e 7432 445f 5479 7065 223e 0d0a  Point2D_Type">..
-00002110: 2020 2020 2020 2020 3c61 6e6e 6f74 6174          <annotat
-00002120: 696f 6e3e 0d0a 2020 2020 2020 2020 2020  ion>..          
-00002130: 2020 3c64 6f63 756d 656e 7461 7469 6f6e    <documentation
-00002140: 3e41 2032 4420 706f 696e 7420 6973 2061  >A 2D point is a
-00002150: 2073 6571 7565 6e63 6520 6f66 2074 776f   sequence of two
-00002160: 2063 6f6f 7264 696e 6174 6573 2e3c 2f64   coordinates.</d
-00002170: 6f63 756d 656e 7461 7469 6f6e 3e0d 0a20  ocumentation>.. 
-00002180: 2020 2020 2020 203c 2f61 6e6e 6f74 6174         </annotat
-00002190: 696f 6e3e 0d0a 2020 2020 2020 2020 3c63  ion>..        <c
-000021a0: 6f6d 706c 6578 436f 6e74 656e 743e 0d0a  omplexContent>..
-000021b0: 2020 2020 2020 2020 2020 2020 3c72 6573              <res
-000021c0: 7472 6963 7469 6f6e 2062 6173 653d 2267  triction base="g
-000021d0: 6174 696e 673a 506f 696e 745f 5479 7065  ating:Point_Type
-000021e0: 223e 0d0a 2020 2020 2020 2020 2020 2020  ">..            
-000021f0: 2020 2020 3c73 6571 7565 6e63 653e 0d0a      <sequence>..
-00002200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002210: 2020 2020 3c65 6c65 6d65 6e74 206e 616d      <element nam
-00002220: 653d 2263 6f6f 7264 696e 6174 6522 2074  e="coordinate" t
-00002230: 7970 653d 2264 6174 612d 7479 7065 3a56  ype="data-type:V
-00002240: 616c 7565 4174 7472 6962 7574 655f 5479  alueAttribute_Ty
-00002250: 7065 2220 6d69 6e4f 6363 7572 733d 2232  pe" minOccurs="2
-00002260: 2220 6d61 784f 6363 7572 733d 2232 2220  " maxOccurs="2" 
-00002270: 2f3e 0d0a 2020 2020 2020 2020 2020 2020  />..            
-00002280: 2020 2020 3c2f 7365 7175 656e 6365 3e0d      </sequence>.
-00002290: 0a20 2020 2020 2020 2020 2020 203c 2f72  .            </r
-000022a0: 6573 7472 6963 7469 6f6e 3e0d 0a20 2020  estriction>..   
-000022b0: 2020 2020 203c 2f63 6f6d 706c 6578 436f       </complexCo
-000022c0: 6e74 656e 743e 0d0a 2020 2020 3c2f 636f  ntent>..    </co
-000022d0: 6d70 6c65 7854 7970 653e 0d0a 0d0a 2020  mplexType>....  
-000022e0: 2020 3c63 6f6d 706c 6578 5479 7065 206e    <complexType n
-000022f0: 616d 653d 2250 6f69 6e74 5844 5f54 7970  ame="PointXD_Typ
-00002300: 6522 3e0d 0a20 2020 2020 2020 203c 616e  e">..        <an
-00002310: 6e6f 7461 7469 6f6e 3e0d 0a20 2020 2020  notation>..     
-00002320: 2020 2020 2020 203c 646f 6375 6d65 6e74         <document
-00002330: 6174 696f 6e3e 4120 3220 6f72 206d 6f72  ation>A 2 or mor
-00002340: 6520 6469 6d65 6e73 696f 6e61 6c20 706f  e dimensional po
-00002350: 696e 7420 6973 2061 2073 6571 7565 6e63  int is a sequenc
-00002360: 6520 6f66 2074 776f 206f 7220 6d6f 7265  e of two or more
-00002370: 2063 6f6f 7264 696e 6174 6573 2e3c 2f64   coordinates.</d
-00002380: 6f63 756d 656e 7461 7469 6f6e 3e0d 0a20  ocumentation>.. 
-00002390: 2020 2020 2020 203c 2f61 6e6e 6f74 6174         </annotat
-000023a0: 696f 6e3e 0d0a 2020 2020 2020 2020 3c63  ion>..        <c
-000023b0: 6f6d 706c 6578 436f 6e74 656e 743e 0d0a  omplexContent>..
-000023c0: 2020 2020 2020 2020 2020 2020 3c72 6573              <res
-000023d0: 7472 6963 7469 6f6e 2062 6173 653d 2267  triction base="g
-000023e0: 6174 696e 673a 506f 696e 745f 5479 7065  ating:Point_Type
-000023f0: 223e 0d0a 2020 2020 2020 2020 2020 2020  ">..            
-00002400: 2020 2020 3c73 6571 7565 6e63 653e 0d0a      <sequence>..
-00002410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002420: 2020 2020 3c65 6c65 6d65 6e74 206e 616d      <element nam
-00002430: 653d 2263 6f6f 7264 696e 6174 6522 2074  e="coordinate" t
-00002440: 7970 653d 2264 6174 612d 7479 7065 3a56  ype="data-type:V
-00002450: 616c 7565 4174 7472 6962 7574 655f 5479  alueAttribute_Ty
-00002460: 7065 2220 6d69 6e4f 6363 7572 733d 2232  pe" minOccurs="2
-00002470: 2220 6d61 784f 6363 7572 733d 2275 6e62  " maxOccurs="unb
-00002480: 6f75 6e64 6564 2220 2f3e 0d0a 2020 2020  ounded" />..    
-00002490: 2020 2020 2020 2020 2020 2020 3c2f 7365              </se
-000024a0: 7175 656e 6365 3e0d 0a20 2020 2020 2020  quence>..       
-000024b0: 2020 2020 203c 2f72 6573 7472 6963 7469       </restricti
-000024c0: 6f6e 3e0d 0a20 2020 2020 2020 203c 2f63  on>..        </c
-000024d0: 6f6d 706c 6578 436f 6e74 656e 743e 0d0a  omplexContent>..
-000024e0: 2020 2020 3c2f 636f 6d70 6c65 7854 7970      </complexTyp
-000024f0: 653e 0d0a 0d0a 2020 2020 3c63 6f6d 706c  e>....    <compl
-00002500: 6578 5479 7065 206e 616d 653d 224d 6174  exType name="Mat
-00002510: 7269 785f 5479 7065 223e 0d0a 2020 2020  rix_Type">..    
-00002520: 2020 2020 3c61 6e6e 6f74 6174 696f 6e3e      <annotation>
-00002530: 0d0a 2020 2020 2020 2020 2020 2020 3c64  ..            <d
-00002540: 6f63 756d 656e 7461 7469 6f6e 3e44 6573  ocumentation>Des
-00002550: 6372 6970 7469 6f6e 206f 6620 6120 6d61  cription of a ma
-00002560: 7472 6978 2e3c 2f64 6f63 756d 656e 7461  trix.</documenta
-00002570: 7469 6f6e 3e0d 0a20 2020 2020 2020 203c  tion>..        <
-00002580: 2f61 6e6e 6f74 6174 696f 6e3e 0d0a 2020  /annotation>..  
-00002590: 2020 2020 2020 3c73 6571 7565 6e63 653e        <sequence>
-000025a0: 0d0a 2020 2020 2020 2020 2020 2020 3c65  ..            <e
-000025b0: 6c65 6d65 6e74 206e 616d 653d 2272 6f77  lement name="row
-000025c0: 2220 7479 7065 3d22 6761 7469 6e67 3a4d  " type="gating:M
-000025d0: 6174 7269 7852 6f77 5f54 7970 6522 206d  atrixRow_Type" m
-000025e0: 696e 4f63 6375 7273 3d22 3122 206d 6178  inOccurs="1" max
-000025f0: 4f63 6375 7273 3d22 756e 626f 756e 6465  Occurs="unbounde
-00002600: 6422 202f 3e0d 0a20 2020 2020 2020 203c  d" />..        <
-00002610: 2f73 6571 7565 6e63 653e 0d0a 2020 2020  /sequence>..    
-00002620: 3c2f 636f 6d70 6c65 7854 7970 653e 0d0a  </complexType>..
-00002630: 0d0a 2020 2020 3c63 6f6d 706c 6578 5479  ..    <complexTy
-00002640: 7065 206e 616d 653d 224d 6174 7269 7852  pe name="MatrixR
-00002650: 6f77 5f54 7970 6522 3e0d 0a20 2020 2020  ow_Type">..     
-00002660: 2020 203c 616e 6e6f 7461 7469 6f6e 3e0d     <annotation>.
-00002670: 0a20 2020 2020 2020 2020 2020 203c 646f  .            <do
-00002680: 6375 6d65 6e74 6174 696f 6e3e 4465 7363  cumentation>Desc
-00002690: 7269 7074 696f 6e20 6f66 2061 2072 6f77  ription of a row
-000026a0: 206f 6620 6120 6d61 7472 6978 2e3c 2f64   of a matrix.</d
-000026b0: 6f63 756d 656e 7461 7469 6f6e 3e0d 0a20  ocumentation>.. 
-000026c0: 2020 2020 2020 203c 2f61 6e6e 6f74 6174         </annotat
-000026d0: 696f 6e3e 0d0a 2020 2020 2020 2020 3c73  ion>..        <s
-000026e0: 6571 7565 6e63 653e 0d0a 2020 2020 2020  equence>..      
-000026f0: 2020 2020 2020 3c65 6c65 6d65 6e74 206e        <element n
-00002700: 616d 653d 2265 6e74 7279 2220 7479 7065  ame="entry" type
-00002710: 3d22 6461 7461 2d74 7970 653a 5661 6c75  ="data-type:Valu
-00002720: 6541 7474 7269 6275 7465 5f54 7970 6522  eAttribute_Type"
-00002730: 206d 696e 4f63 6375 7273 3d22 3122 0d0a   minOccurs="1"..
-00002740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002750: 6d61 784f 6363 7572 733d 2275 6e62 6f75  maxOccurs="unbou
-00002760: 6e64 6564 2220 2f3e 0d0a 2020 2020 2020  nded" />..      
-00002770: 2020 3c2f 7365 7175 656e 6365 3e0d 0a20    </sequence>.. 
-00002780: 2020 203c 2f63 6f6d 706c 6578 5479 7065     </complexType
-00002790: 3e0d 0a0d 0a20 2020 203c 6772 6f75 7020  >....    <group 
-000027a0: 6e61 6d65 3d22 426f 6f6c 4761 7465 4f70  name="BoolGateOp
-000027b0: 6572 616e 6473 5f47 726f 7570 223e 0d0a  erands_Group">..
-000027c0: 2020 2020 2020 2020 3c61 6e6e 6f74 6174          <annotat
-000027d0: 696f 6e3e 0d0a 2020 2020 2020 2020 2020  ion>..          
-000027e0: 2020 3c64 6f63 756d 656e 7461 7469 6f6e    <documentation
-000027f0: 2078 6d6c 3a6c 616e 673d 2265 6e22 3e41   xml:lang="en">A
-00002800: 6e20 6f70 6572 616e 6420 6f66 2061 2042  n operand of a B
-00002810: 6f6f 6c65 616e 2067 6174 6520 6361 6e20  oolean gate can 
-00002820: 6265 2073 7065 6369 6669 6564 2061 7320  be specified as 
-00002830: 6761 7465 5265 6665 7265 6e63 6520 6f72  gateReference or
-00002840: 2061 7320 616e 2065 6d62 6564 6465 6420   as an embedded 
-00002850: 7370 6563 6966 6963 6174 696f 6e20 6f66  specification of
-00002860: 2061 6e6f 7468 6572 2067 6174 652e 3c2f   another gate.</
-00002870: 646f 6375 6d65 6e74 6174 696f 6e3e 0d0a  documentation>..
-00002880: 2020 2020 2020 2020 3c2f 616e 6e6f 7461          </annota
-00002890: 7469 6f6e 3e0d 0a20 2020 2020 2020 203c  tion>..        <
-000028a0: 6368 6f69 6365 3e0d 0a20 2020 2020 2020  choice>..       
-000028b0: 2020 2020 203c 656c 656d 656e 7420 6e61       <element na
-000028c0: 6d65 3d22 6761 7465 5265 6665 7265 6e63  me="gateReferenc
-000028d0: 6522 2074 7970 653d 2267 6174 696e 673a  e" type="gating:
-000028e0: 4761 7465 5265 6665 7265 6e63 655f 5479  GateReference_Ty
-000028f0: 7065 2220 6964 3d22 6761 7465 5265 6665  pe" id="gateRefe
-00002900: 7265 6e63 6522 202f 3e0d 0a20 2020 2020  rence" />..     
-00002910: 2020 203c 2f63 686f 6963 653e 0d0a 2020     </choice>..  
-00002920: 2020 3c2f 6772 6f75 703e 0d0a 0d0a 2020    </group>....  
-00002930: 2020 3c63 6f6d 706c 6578 5479 7065 206e    <complexType n
-00002940: 616d 653d 2254 776f 416e 644d 6f72 654f  ame="TwoAndMoreO
-00002950: 7065 7261 6e64 735f 426f 6f6c 4761 7465  perands_BoolGate
-00002960: 5f54 7970 6522 3e0d 0a20 2020 2020 2020  _Type">..       
-00002970: 203c 616e 6e6f 7461 7469 6f6e 3e0d 0a20   <annotation>.. 
-00002980: 2020 2020 2020 2020 2020 203c 646f 6375             <docu
-00002990: 6d65 6e74 6174 696f 6e20 786d 6c3a 6c61  mentation xml:la
-000029a0: 6e67 3d22 656e 223e 5468 6520 7479 7065  ng="en">The type
-000029b0: 206f 6620 426f 6f6c 6561 6e20 6761 7465   of Boolean gate
-000029c0: 7320 7769 7468 2074 776f 206f 7220 6d6f  s with two or mo
-000029d0: 7265 206f 7065 7261 6e64 7320 2841 4e44  re operands (AND
-000029e0: 2061 6e64 204f 5220 6761 7465 7329 2e3c   and OR gates).<
-000029f0: 2f64 6f63 756d 656e 7461 7469 6f6e 3e0d  /documentation>.
-00002a00: 0a20 2020 2020 2020 203c 2f61 6e6e 6f74  .        </annot
-00002a10: 6174 696f 6e3e 0d0a 2020 2020 2020 2020  ation>..        
-00002a20: 3c73 6571 7565 6e63 6520 6d69 6e4f 6363  <sequence minOcc
-00002a30: 7572 733d 2232 2220 6d61 784f 6363 7572  urs="2" maxOccur
-00002a40: 733d 2275 6e62 6f75 6e64 6564 223e 0d0a  s="unbounded">..
-00002a50: 2020 2020 2020 2020 2020 2020 3c67 726f              <gro
-00002a60: 7570 2072 6566 3d22 6761 7469 6e67 3a42  up ref="gating:B
-00002a70: 6f6f 6c47 6174 654f 7065 7261 6e64 735f  oolGateOperands_
-00002a80: 4772 6f75 7022 202f 3e0d 0a20 2020 2020  Group" />..     
-00002a90: 2020 203c 2f73 6571 7565 6e63 653e 0d0a     </sequence>..
-00002aa0: 2020 2020 3c2f 636f 6d70 6c65 7854 7970      </complexTyp
-00002ab0: 653e 0d0a 0d0a 2020 2020 3c63 6f6d 706c  e>....    <compl
-00002ac0: 6578 5479 7065 206e 616d 653d 224f 6e65  exType name="One
-00002ad0: 4f70 6572 616e 645f 426f 6f6c 4761 7465  Operand_BoolGate
-00002ae0: 5f54 7970 6522 3e0d 0a20 2020 2020 2020  _Type">..       
-00002af0: 203c 616e 6e6f 7461 7469 6f6e 3e0d 0a20   <annotation>.. 
-00002b00: 2020 2020 2020 2020 2020 203c 646f 6375             <docu
-00002b10: 6d65 6e74 6174 696f 6e20 786d 6c3a 6c61  mentation xml:la
-00002b20: 6e67 3d22 656e 223e 5468 6520 7479 7065  ng="en">The type
-00002b30: 206f 6620 426f 6f6c 6561 6e20 4761 7465   of Boolean Gate
-00002b40: 7320 7769 7468 2065 7861 6374 6c79 206f  s with exactly o
-00002b50: 6e65 206f 7065 7261 6e64 2028 4e4f 5420  ne operand (NOT 
-00002b60: 6761 7465 292e 3c2f 646f 6375 6d65 6e74  gate).</document
-00002b70: 6174 696f 6e3e 0d0a 2020 2020 2020 2020  ation>..        
-00002b80: 3c2f 616e 6e6f 7461 7469 6f6e 3e0d 0a20  </annotation>.. 
-00002b90: 2020 2020 2020 203c 7365 7175 656e 6365         <sequence
-00002ba0: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
-00002bb0: 6772 6f75 7020 7265 663d 2267 6174 696e  group ref="gatin
-00002bc0: 673a 426f 6f6c 4761 7465 4f70 6572 616e  g:BoolGateOperan
-00002bd0: 6473 5f47 726f 7570 2220 2f3e 0d0a 2020  ds_Group" />..  
-00002be0: 2020 2020 2020 3c2f 7365 7175 656e 6365        </sequence
-00002bf0: 3e0d 0a20 2020 203c 2f63 6f6d 706c 6578  >..    </complex
-00002c00: 5479 7065 3e0d 0a0d 0a20 2020 203c 636f  Type>....    <co
-00002c10: 6d70 6c65 7854 7970 6520 6e61 6d65 3d22  mplexType name="
-00002c20: 4761 7465 5265 6665 7265 6e63 655f 5479  GateReference_Ty
-00002c30: 7065 223e 0d0a 2020 2020 2020 2020 3c61  pe">..        <a
-00002c40: 6e6e 6f74 6174 696f 6e3e 0d0a 2020 2020  nnotation>..    
-00002c50: 2020 2020 2020 2020 3c64 6f63 756d 656e          <documen
-00002c60: 7461 7469 6f6e 2078 6d6c 3a6c 616e 673d  tation xml:lang=
-00002c70: 2265 6e22 3e54 7970 6520 6f66 2061 2072  "en">Type of a r
-00002c80: 6566 6572 656e 6365 2074 6f20 616e 6f74  eference to anot
-00002c90: 6865 7220 2861 6c72 6561 6479 2064 6566  her (already def
-00002ca0: 696e 6564 2920 6761 7465 2e20 5468 6520  ined) gate. The 
-00002cb0: 6174 7472 6962 7574 6520 7265 6620 7265  attribute ref re
-00002cc0: 6665 7265 6e63 6573 2061 2067 6174 6520  ferences a gate 
-00002cd0: 6279 2069 7473 2069 642e 203c 2f64 6f63  by its id. </doc
-00002ce0: 756d 656e 7461 7469 6f6e 3e0d 0a20 2020  umentation>..   
-00002cf0: 2020 2020 203c 2f61 6e6e 6f74 6174 696f       </annotatio
-00002d00: 6e3e 0d0a 2020 2020 2020 2020 3c61 7474  n>..        <att
-00002d10: 7269 6275 7465 206e 616d 653d 2272 6566  ribute name="ref
-00002d20: 2220 7479 7065 3d22 4944 5245 4622 2075  " type="IDREF" u
-00002d30: 7365 3d22 7265 7175 6972 6564 2220 6964  se="required" id
-00002d40: 3d22 7265 6622 202f 3e0d 0a20 2020 2020  ="ref" />..     
-00002d50: 2020 203c 6174 7472 6962 7574 6520 6e61     <attribute na
-00002d60: 6d65 3d22 7573 652d 6173 2d63 6f6d 706c  me="use-as-compl
-00002d70: 656d 656e 7422 2074 7970 653d 2262 6f6f  ement" type="boo
-00002d80: 6c65 616e 2220 6465 6661 756c 743d 2266  lean" default="f
-00002d90: 616c 7365 2220 7573 653d 226f 7074 696f  alse" use="optio
-00002da0: 6e61 6c22 2069 643d 2275 7365 2d61 732d  nal" id="use-as-
-00002db0: 636f 6d70 6c65 6d65 6e74 2220 2f3e 0d0a  complement" />..
-00002dc0: 2020 2020 3c2f 636f 6d70 6c65 7854 7970      </complexTyp
-00002dd0: 653e 0d0a 0d0a 3c2f 7363 6865 6d61 3e0d  e>....</schema>.
-00002de0: 0a                                       .
+00000020: 462d 3822 3f3e 0a0a 3c73 6368 656d 6120  F-8"?>..<schema 
+00000030: 786d 6c6e 733d 2268 7474 703a 2f2f 7777  xmlns="http://ww
+00000040: 772e 7733 2e6f 7267 2f32 3030 312f 584d  w.w3.org/2001/XM
+00000050: 4c53 6368 656d 6122 0a20 2020 2078 6d6c  LSchema".    xml
+00000060: 6e73 3a67 6174 696e 673d 2268 7474 703a  ns:gating="http:
+00000070: 2f2f 7777 772e 6973 6163 2d6e 6574 2e6f  //www.isac-net.o
+00000080: 7267 2f73 7464 2f47 6174 696e 672d 4d4c  rg/std/Gating-ML
+00000090: 2f76 322e 302f 6761 7469 6e67 220a 2020  /v2.0/gating".  
+000000a0: 2020 786d 6c6e 733a 7472 616e 7366 6f72    xmlns:transfor
+000000b0: 6d73 3d22 6874 7470 3a2f 2f77 7777 2e69  ms="http://www.i
+000000c0: 7361 632d 6e65 742e 6f72 672f 7374 642f  sac-net.org/std/
+000000d0: 4761 7469 6e67 2d4d 4c2f 7632 2e30 2f74  Gating-ML/v2.0/t
+000000e0: 7261 6e73 666f 726d 6174 696f 6e73 220a  ransformations".
+000000f0: 2020 2020 786d 6c6e 733a 6461 7461 2d74      xmlns:data-t
+00000100: 7970 653d 2268 7474 703a 2f2f 7777 772e  ype="http://www.
+00000110: 6973 6163 2d6e 6574 2e6f 7267 2f73 7464  isac-net.org/std
+00000120: 2f47 6174 696e 672d 4d4c 2f76 322e 302f  /Gating-ML/v2.0/
+00000130: 6461 7461 7479 7065 7322 0a20 2020 2074  datatypes".    t
+00000140: 6172 6765 744e 616d 6573 7061 6365 3d22  argetNamespace="
+00000150: 6874 7470 3a2f 2f77 7777 2e69 7361 632d  http://www.isac-
+00000160: 6e65 742e 6f72 672f 7374 642f 4761 7469  net.org/std/Gati
+00000170: 6e67 2d4d 4c2f 7632 2e30 2f67 6174 696e  ng-ML/v2.0/gatin
+00000180: 6722 0a20 2020 2065 6c65 6d65 6e74 466f  g".    elementFo
+00000190: 726d 4465 6661 756c 743d 2271 7561 6c69  rmDefault="quali
+000001a0: 6669 6564 2220 6174 7472 6962 7574 6546  fied" attributeF
+000001b0: 6f72 6d44 6566 6175 6c74 3d22 7175 616c  ormDefault="qual
+000001c0: 6966 6965 6422 2076 6572 7369 6f6e 3d22  ified" version="
+000001d0: 322e 302e 3132 3132 3037 223e 0a0a 2020  2.0.121207">..  
+000001e0: 2020 3c69 6d70 6f72 7420 6e61 6d65 7370    <import namesp
+000001f0: 6163 653d 2268 7474 703a 2f2f 7777 772e  ace="http://www.
+00000200: 6973 6163 2d6e 6574 2e6f 7267 2f73 7464  isac-net.org/std
+00000210: 2f47 6174 696e 672d 4d4c 2f76 322e 302f  /Gating-ML/v2.0/
+00000220: 7472 616e 7366 6f72 6d61 7469 6f6e 7322  transformations"
+00000230: 2073 6368 656d 614c 6f63 6174 696f 6e3d   schemaLocation=
+00000240: 2254 7261 6e73 666f 726d 6174 696f 6e73  "Transformations
+00000250: 2e76 322e 302e 7873 6422 202f 3e0a 2020  .v2.0.xsd" />.  
+00000260: 2020 3c69 6d70 6f72 7420 6e61 6d65 7370    <import namesp
+00000270: 6163 653d 2268 7474 703a 2f2f 7777 772e  ace="http://www.
+00000280: 6973 6163 2d6e 6574 2e6f 7267 2f73 7464  isac-net.org/std
+00000290: 2f47 6174 696e 672d 4d4c 2f76 322e 302f  /Gating-ML/v2.0/
+000002a0: 6461 7461 7479 7065 7322 2073 6368 656d  datatypes" schem
+000002b0: 614c 6f63 6174 696f 6e3d 2244 6174 6154  aLocation="DataT
+000002c0: 7970 6573 2e76 322e 302e 7873 6422 202f  ypes.v2.0.xsd" /
+000002d0: 3e0a 0a20 2020 203c 616e 6e6f 7461 7469  >..    <annotati
+000002e0: 6f6e 3e0a 2020 2020 2020 2020 3c61 7070  on>.        <app
+000002f0: 696e 666f 2073 6f75 7263 653d 2268 7474  info source="htt
+00000300: 703a 2f2f 666c 6f77 6379 742e 7366 2e6e  p://flowcyt.sf.n
+00000310: 6574 2f22 3e47 6174 696e 672d 4d4c 3a20  et/">Gating-ML: 
+00000320: 4761 7469 6e67 2044 6573 6372 6970 7469  Gating Descripti
+00000330: 6f6e 2053 7065 6369 6669 6361 7469 6f6e  on Specification
+00000340: 2e3c 2f61 7070 696e 666f 3e0a 2020 2020  .</appinfo>.    
+00000350: 2020 2020 3c64 6f63 756d 656e 7461 7469      <documentati
+00000360: 6f6e 2078 6d6c 3a6c 616e 673d 2265 6e22  on xml:lang="en"
+00000370: 2073 6f75 7263 653d 2268 7474 703a 2f2f   source="http://
+00000380: 666c 6f77 6379 742e 736f 7572 6365 666f  flowcyt.sourcefo
+00000390: 7267 652e 6e65 742f 223e 0a20 2020 2020  rge.net/">.     
+000003a0: 2020 2020 2020 203c 6175 7468 6f72 3e0a         <author>.
+000003b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000003c0: 3c6e 616d 653e 4a6f 7365 6620 5370 6964  <name>Josef Spid
+000003d0: 6c65 6e3c 2f6e 616d 653e 0a20 2020 2020  len</name>.     
+000003e0: 2020 2020 2020 2020 2020 203c 656d 6169             <emai
+000003f0: 6c3e 6a73 7069 646c 656e 4062 6363 7263  l>jspidlen@bccrc
+00000400: 2e63 613c 2f65 6d61 696c 3e0a 2020 2020  .ca</email>.    
+00000410: 2020 2020 2020 2020 3c2f 6175 7468 6f72          </author
+00000420: 3e0a 2020 2020 2020 2020 2020 2020 3c63  >.            <c
+00000430: 6f70 7972 6967 6874 3e0a 2020 2020 2020  opyright>.      
+00000440: 2020 2020 2020 2020 2020 436f 7079 7269            Copyri
+00000450: 6768 7420 2863 2920 3230 3038 2d32 3031  ght (c) 2008-201
+00000460: 3420 4953 4143 2028 496e 7465 726e 6174  4 ISAC (Internat
+00000470: 696f 6e61 6c20 536f 6369 6574 7920 666f  ional Society fo
+00000480: 7220 4164 7661 6e63 656d 656e 7420 6f66  r Advancement of
+00000490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000004a0: 2043 7974 6f6d 6574 7279 292e 2046 7265   Cytometry). Fre
+000004b0: 6520 6f66 2063 6861 7267 6520 6469 7374  e of charge dist
+000004c0: 7269 6275 7469 6f6e 2061 6e64 2072 6561  ribution and rea
+000004d0: 642d 6f6e 6c79 2075 7361 6765 2070 6572  d-only usage per
+000004e0: 6d69 7465 642e 204d 6f64 6966 6963 6174  mited. Modificat
+000004f0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+00000500: 2020 2020 616e 6420 616c 6c20 6f74 6865      and all othe
+00000510: 7220 7269 6768 7473 2072 6573 6572 7665  r rights reserve
+00000520: 642e 2046 6f72 2061 6c6c 206f 7468 6572  d. For all other
+00000530: 2075 7365 7320 706c 6561 7365 2063 6f6e   uses please con
+00000540: 7461 6374 2049 5341 432e 0a20 2020 2020  tact ISAC..     
+00000550: 2020 2020 2020 203c 2f63 6f70 7972 6967         </copyrig
+00000560: 6874 3e0a 2020 2020 2020 2020 3c2f 646f  ht>.        </do
+00000570: 6375 6d65 6e74 6174 696f 6e3e 0a20 2020  cumentation>.   
+00000580: 203c 2f61 6e6e 6f74 6174 696f 6e3e 0a0a   </annotation>..
+00000590: 2020 2020 3c65 6c65 6d65 6e74 206e 616d      <element nam
+000005a0: 653d 2247 6174 696e 672d 4d4c 2220 7479  e="Gating-ML" ty
+000005b0: 7065 3d22 6761 7469 6e67 3a47 6174 696e  pe="gating:Gatin
+000005c0: 672d 4d4c 5f54 7970 6522 2069 643d 2247  g-ML_Type" id="G
+000005d0: 6174 696e 672d 4d4c 223e 0a20 2020 2020  ating-ML">.     
+000005e0: 2020 203c 616e 6e6f 7461 7469 6f6e 3e0a     <annotation>.
+000005f0: 2020 2020 2020 2020 2020 2020 3c64 6f63              <doc
+00000600: 756d 656e 7461 7469 6f6e 2078 6d6c 3a6c  umentation xml:l
+00000610: 616e 673d 2265 6e22 3e47 6174 696e 672d  ang="en">Gating-
+00000620: 4d4c 2069 7320 7468 6520 6d61 696e 2065  ML is the main e
+00000630: 6c65 6d65 6e74 206f 6620 616e 2058 4d4c  lement of an XML
+00000640: 2063 6f72 7265 7370 6f6e 6469 6e67 2074   corresponding t
+00000650: 6f20 7468 6973 2073 6368 656d 612e 3c2f  o this schema.</
+00000660: 646f 6375 6d65 6e74 6174 696f 6e3e 0a20  documentation>. 
+00000670: 2020 2020 2020 203c 2f61 6e6e 6f74 6174         </annotat
+00000680: 696f 6e3e 0a20 2020 203c 2f65 6c65 6d65  ion>.    </eleme
+00000690: 6e74 3e0a 0a20 2020 203c 6772 6f75 7020  nt>..    <group 
+000006a0: 6e61 6d65 3d22 4761 7465 735f 4772 6f75  name="Gates_Grou
+000006b0: 7022 3e0a 2020 2020 2020 2020 3c61 6e6e  p">.        <ann
+000006c0: 6f74 6174 696f 6e3e 0a20 2020 2020 2020  otation>.       
+000006d0: 2020 2020 203c 646f 6375 6d65 6e74 6174       <documentat
+000006e0: 696f 6e20 786d 6c3a 6c61 6e67 3d22 656e  ion xml:lang="en
+000006f0: 223e 5468 6520 6772 6f75 7020 696e 636c  ">The group incl
+00000700: 7564 6573 2061 2063 686f 6963 6520 6672  udes a choice fr
+00000710: 6f6d 2061 6c6c 2074 6865 2074 7970 6573  om all the types
+00000720: 206f 6620 6761 7465 732e 3c2f 646f 6375   of gates.</docu
+00000730: 6d65 6e74 6174 696f 6e3e 0a20 2020 2020  mentation>.     
+00000740: 2020 203c 2f61 6e6e 6f74 6174 696f 6e3e     </annotation>
+00000750: 0a20 2020 2020 2020 203c 6368 6f69 6365  .        <choice
+00000760: 3e0a 2020 2020 2020 2020 2020 2020 3c65  >.            <e
+00000770: 6c65 6d65 6e74 206e 616d 653d 2252 6563  lement name="Rec
+00000780: 7461 6e67 6c65 4761 7465 2220 7479 7065  tangleGate" type
+00000790: 3d22 6761 7469 6e67 3a52 6563 7461 6e67  ="gating:Rectang
+000007a0: 6c65 4761 7465 5f54 7970 6522 202f 3e0a  leGate_Type" />.
+000007b0: 2020 2020 2020 2020 2020 2020 3c65 6c65              <ele
+000007c0: 6d65 6e74 206e 616d 653d 2250 6f6c 7967  ment name="Polyg
+000007d0: 6f6e 4761 7465 2220 7479 7065 3d22 6761  onGate" type="ga
+000007e0: 7469 6e67 3a50 6f6c 7967 6f6e 4761 7465  ting:PolygonGate
+000007f0: 5f54 7970 6522 202f 3e0a 2020 2020 2020  _Type" />.      
+00000800: 2020 2020 2020 3c65 6c65 6d65 6e74 206e        <element n
+00000810: 616d 653d 2245 6c6c 6970 736f 6964 4761  ame="EllipsoidGa
+00000820: 7465 2220 7479 7065 3d22 6761 7469 6e67  te" type="gating
+00000830: 3a45 6c6c 6970 736f 6964 4761 7465 5f54  :EllipsoidGate_T
+00000840: 7970 6522 202f 3e0a 2020 2020 2020 2020  ype" />.        
+00000850: 2020 2020 3c65 6c65 6d65 6e74 206e 616d      <element nam
+00000860: 653d 2242 6f6f 6c65 616e 4761 7465 2220  e="BooleanGate" 
+00000870: 7479 7065 3d22 6761 7469 6e67 3a42 6f6f  type="gating:Boo
+00000880: 6c65 616e 4761 7465 5f54 7970 6522 202f  leanGate_Type" /
+00000890: 3e0a 2020 2020 2020 2020 2020 2020 3c65  >.            <e
+000008a0: 6c65 6d65 6e74 206e 616d 653d 2251 7561  lement name="Qua
+000008b0: 6472 616e 7447 6174 6522 2074 7970 653d  drantGate" type=
+000008c0: 2267 6174 696e 673a 5175 6164 7261 6e74  "gating:Quadrant
+000008d0: 4761 7465 5f54 7970 6522 202f 3e0a 2020  Gate_Type" />.  
+000008e0: 2020 2020 2020 3c2f 6368 6f69 6365 3e0a        </choice>.
+000008f0: 2020 2020 3c2f 6772 6f75 703e 0a0a 2020      </group>..  
+00000900: 2020 3c63 6f6d 706c 6578 5479 7065 206e    <complexType n
+00000910: 616d 653d 2247 6174 696e 672d 4d4c 5f54  ame="Gating-ML_T
+00000920: 7970 6522 3e0a 2020 2020 2020 2020 3c73  ype">.        <s
+00000930: 6571 7565 6e63 6520 6d69 6e4f 6363 7572  equence minOccur
+00000940: 733d 2231 2220 6d61 784f 6363 7572 733d  s="1" maxOccurs=
+00000950: 2275 6e62 6f75 6e64 6564 223e 0a20 2020  "unbounded">.   
+00000960: 2020 2020 2020 2020 203c 6368 6f69 6365           <choice
+00000970: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000980: 2020 3c67 726f 7570 2072 6566 3d22 6761    <group ref="ga
+00000990: 7469 6e67 3a47 6174 6573 5f47 726f 7570  ting:Gates_Group
+000009a0: 2220 2f3e 0a20 2020 2020 2020 2020 2020  " />.           
+000009b0: 2020 2020 203c 6772 6f75 7020 7265 663d       <group ref=
+000009c0: 2274 7261 6e73 666f 726d 733a 5472 616e  "transforms:Tran
+000009d0: 7366 6f72 6d61 7469 6f6e 5f47 726f 7570  sformation_Group
+000009e0: 2220 2f3e 0a20 2020 2020 2020 2020 2020  " />.           
+000009f0: 2020 2020 203c 6772 6f75 7020 7265 663d       <group ref=
+00000a00: 2274 7261 6e73 666f 726d 733a 5370 6563  "transforms:Spec
+00000a10: 7472 756d 4d61 7472 6978 5f47 726f 7570  trumMatrix_Group
+00000a20: 2220 2f3e 0a20 2020 2020 2020 2020 2020  " />.           
+00000a30: 2020 2020 203c 6772 6f75 7020 7265 663d       <group ref=
+00000a40: 2264 6174 612d 7479 7065 3a43 7573 746f  "data-type:Custo
+00000a50: 6d5f 4772 6f75 7022 202f 3e0a 2020 2020  m_Group" />.    
+00000a60: 2020 2020 2020 2020 3c2f 6368 6f69 6365          </choice
+00000a70: 3e0a 2020 2020 2020 2020 3c2f 7365 7175  >.        </sequ
+00000a80: 656e 6365 3e0a 2020 2020 3c2f 636f 6d70  ence>.    </comp
+00000a90: 6c65 7854 7970 653e 0a0a 2020 2020 3c63  lexType>..    <c
+00000aa0: 6f6d 706c 6578 5479 7065 206e 616d 653d  omplexType name=
+00000ab0: 2241 6273 7472 6163 7447 6174 655f 5479  "AbstractGate_Ty
+00000ac0: 7065 2220 6162 7374 7261 6374 3d22 7472  pe" abstract="tr
+00000ad0: 7565 223e 0a20 2020 2020 2020 203c 616e  ue">.        <an
+00000ae0: 6e6f 7461 7469 6f6e 3e0a 2020 2020 2020  notation>.      
+00000af0: 2020 2020 2020 3c64 6f63 756d 656e 7461        <documenta
+00000b00: 7469 6f6e 2078 6d6c 3a6c 616e 673d 2265  tion xml:lang="e
+00000b10: 6e22 3e41 6273 7472 6163 7420 7479 7065  n">Abstract type
+00000b20: 2074 6f20 6265 2075 7365 6420 6173 2061   to be used as a
+00000b30: 2063 6f6d 6d6f 6e20 7061 7265 6e74 206f   common parent o
+00000b40: 6620 616c 6c20 7479 7065 7320 6f66 2067  f all types of g
+00000b50: 6174 6573 2e3c 2f64 6f63 756d 656e 7461  ates.</documenta
+00000b60: 7469 6f6e 3e0a 2020 2020 2020 2020 3c2f  tion>.        </
+00000b70: 616e 6e6f 7461 7469 6f6e 3e0a 2020 2020  annotation>.    
+00000b80: 2020 2020 3c67 726f 7570 2072 6566 3d22      <group ref="
+00000b90: 6461 7461 2d74 7970 653a 4375 7374 6f6d  data-type:Custom
+00000ba0: 5f47 726f 7570 2220 6d69 6e4f 6363 7572  _Group" minOccur
+00000bb0: 733d 2230 2220 2f3e 0a20 2020 2020 2020  s="0" />.       
+00000bc0: 203c 6174 7472 6962 7574 6520 6e61 6d65   <attribute name
+00000bd0: 3d22 6964 2220 7479 7065 3d22 4944 2220  ="id" type="ID" 
+00000be0: 7573 653d 2272 6571 7569 7265 6422 2069  use="required" i
+00000bf0: 643d 2269 6422 202f 3e0a 2020 2020 2020  d="id" />.      
+00000c00: 2020 3c61 7474 7269 6275 7465 206e 616d    <attribute nam
+00000c10: 653d 2270 6172 656e 745f 6964 2220 7479  e="parent_id" ty
+00000c20: 7065 3d22 4944 5245 4622 2075 7365 3d22  pe="IDREF" use="
+00000c30: 6f70 7469 6f6e 616c 2220 6964 3d22 7061  optional" id="pa
+00000c40: 7265 6e74 5f69 6422 202f 3e0a 2020 2020  rent_id" />.    
+00000c50: 2020 2020 3c61 6e79 4174 7472 6962 7574      <anyAttribut
+00000c60: 6520 7072 6f63 6573 7343 6f6e 7465 6e74  e processContent
+00000c70: 733d 2273 6b69 7022 2f3e 0a20 2020 203c  s="skip"/>.    <
+00000c80: 2f63 6f6d 706c 6578 5479 7065 3e0a 0a20  /complexType>.. 
+00000c90: 2020 203c 636f 6d70 6c65 7854 7970 6520     <complexType 
+00000ca0: 6e61 6d65 3d22 5175 6164 7261 6e74 4761  name="QuadrantGa
+00000cb0: 7465 5f54 7970 6522 3e0a 2020 2020 2020  te_Type">.      
+00000cc0: 2020 3c63 6f6d 706c 6578 436f 6e74 656e    <complexConten
+00000cd0: 743e 0a20 2020 2020 2020 2020 2020 203c  t>.            <
+00000ce0: 6578 7465 6e73 696f 6e20 6261 7365 3d22  extension base="
+00000cf0: 6761 7469 6e67 3a41 6273 7472 6163 7447  gating:AbstractG
+00000d00: 6174 655f 5479 7065 223e 0a20 2020 2020  ate_Type">.     
+00000d10: 2020 2020 2020 2020 2020 203c 7365 7175             <sequ
+00000d20: 656e 6365 3e0a 2020 2020 2020 2020 2020  ence>.          
+00000d30: 2020 2020 2020 2020 2020 3c65 6c65 6d65            <eleme
+00000d40: 6e74 206e 616d 653d 2264 6976 6964 6572  nt name="divider
+00000d50: 2220 7479 7065 3d22 6761 7469 6e67 3a51  " type="gating:Q
+00000d60: 7561 6472 616e 7447 6174 6544 6976 6964  uadrantGateDivid
+00000d70: 6572 5f54 7970 6522 206d 6178 4f63 6375  er_Type" maxOccu
+00000d80: 7273 3d22 756e 626f 756e 6465 6422 2069  rs="unbounded" i
+00000d90: 643d 2264 6976 6964 6572 2220 2f3e 0a20  d="divider" />. 
+00000da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000db0: 2020 203c 656c 656d 656e 7420 6e61 6d65     <element name
+00000dc0: 3d22 5175 6164 7261 6e74 2220 7479 7065  ="Quadrant" type
+00000dd0: 3d22 6761 7469 6e67 3a51 7561 6472 616e  ="gating:Quadran
+00000de0: 745f 5479 7065 2220 6d61 784f 6363 7572  t_Type" maxOccur
+00000df0: 733d 2275 6e62 6f75 6e64 6564 2220 6964  s="unbounded" id
+00000e00: 3d22 7175 6164 7261 6e74 2220 2f3e 0a20  ="quadrant" />. 
+00000e10: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000e20: 2f73 6571 7565 6e63 653e 0a20 2020 2020  /sequence>.     
+00000e30: 2020 2020 2020 203c 2f65 7874 656e 7369         </extensi
+00000e40: 6f6e 3e0a 2020 2020 2020 2020 3c2f 636f  on>.        </co
+00000e50: 6d70 6c65 7843 6f6e 7465 6e74 3e0a 2020  mplexContent>.  
+00000e60: 2020 3c2f 636f 6d70 6c65 7854 7970 653e    </complexType>
+00000e70: 0a0a 2020 2020 3c63 6f6d 706c 6578 5479  ..    <complexTy
+00000e80: 7065 206e 616d 653d 2251 7561 6472 616e  pe name="Quadran
+00000e90: 7447 6174 6544 6976 6964 6572 5f54 7970  tGateDivider_Typ
+00000ea0: 6522 3e0a 2020 2020 2020 2020 3c63 6f6d  e">.        <com
+00000eb0: 706c 6578 436f 6e74 656e 743e 0a20 2020  plexContent>.   
+00000ec0: 2020 2020 2020 2020 203c 6578 7465 6e73           <extens
+00000ed0: 696f 6e20 6261 7365 3d22 6761 7469 6e67  ion base="gating
+00000ee0: 3a44 696d 656e 7369 6f6e 5f54 7970 6522  :Dimension_Type"
+00000ef0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000f00: 2020 3c73 6571 7565 6e63 653e 0a20 2020    <sequence>.   
+00000f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f20: 203c 656c 656d 656e 7420 6e61 6d65 3d22   <element name="
+00000f30: 7661 6c75 6522 2074 7970 653d 2266 6c6f  value" type="flo
+00000f40: 6174 2220 6d61 784f 6363 7572 733d 2275  at" maxOccurs="u
+00000f50: 6e62 6f75 6e64 6564 2220 6964 3d22 6469  nbounded" id="di
+00000f60: 7669 6465 7276 616c 7565 2220 2f3e 0a20  vidervalue" />. 
+00000f70: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000f80: 2f73 6571 7565 6e63 653e 0a20 2020 2020  /sequence>.     
+00000f90: 2020 2020 2020 2020 2020 203c 6174 7472             <attr
+00000fa0: 6962 7574 6520 6e61 6d65 3d22 6964 2220  ibute name="id" 
+00000fb0: 7479 7065 3d22 4944 2220 6964 3d22 6469  type="ID" id="di
+00000fc0: 7669 6465 725f 6964 2220 7573 653d 2272  vider_id" use="r
+00000fd0: 6571 7569 7265 6422 202f 3e0a 2020 2020  equired" />.    
+00000fe0: 2020 2020 2020 2020 3c2f 6578 7465 6e73          </extens
+00000ff0: 696f 6e3e 0a20 2020 2020 2020 203c 2f63  ion>.        </c
+00001000: 6f6d 706c 6578 436f 6e74 656e 743e 0a20  omplexContent>. 
+00001010: 2020 203c 2f63 6f6d 706c 6578 5479 7065     </complexType
+00001020: 3e0a 0a20 2020 203c 636f 6d70 6c65 7854  >..    <complexT
+00001030: 7970 6520 6e61 6d65 3d22 5175 6164 7261  ype name="Quadra
+00001040: 6e74 5f54 7970 6522 3e0a 2020 2020 2020  nt_Type">.      
+00001050: 2020 3c73 6571 7565 6e63 653e 0a20 2020    <sequence>.   
+00001060: 2020 2020 2020 2020 203c 656c 656d 656e           <elemen
+00001070: 7420 6e61 6d65 3d22 706f 7369 7469 6f6e  t name="position
+00001080: 2220 6d61 784f 6363 7572 733d 2275 6e62  " maxOccurs="unb
+00001090: 6f75 6e64 6564 2220 6964 3d22 706f 7369  ounded" id="posi
+000010a0: 7469 6f6e 2220 7479 7065 3d22 6761 7469  tion" type="gati
+000010b0: 6e67 3a50 6f73 6974 696f 6e5f 5479 7065  ng:Position_Type
+000010c0: 2220 2f3e 0a20 2020 2020 2020 203c 2f73  " />.        </s
+000010d0: 6571 7565 6e63 653e 0a20 2020 2020 2020  equence>.       
+000010e0: 203c 6174 7472 6962 7574 6520 6e61 6d65   <attribute name
+000010f0: 3d22 6964 2220 7479 7065 3d22 4944 2220  ="id" type="ID" 
+00001100: 7573 653d 2272 6571 7569 7265 6422 2069  use="required" i
+00001110: 643d 2271 7561 6472 616e 745f 6964 2220  d="quadrant_id" 
+00001120: 2f3e 0a20 2020 203c 2f63 6f6d 706c 6578  />.    </complex
+00001130: 5479 7065 3e0a 0a20 2020 203c 636f 6d70  Type>..    <comp
+00001140: 6c65 7854 7970 6520 6e61 6d65 3d22 506f  lexType name="Po
+00001150: 7369 7469 6f6e 5f54 7970 6522 3e0a 2020  sition_Type">.  
+00001160: 2020 2020 2020 3c61 7474 7269 6275 7465        <attribute
+00001170: 206e 616d 653d 2264 6976 6964 6572 5f72   name="divider_r
+00001180: 6566 2220 7573 653d 2272 6571 7569 7265  ef" use="require
+00001190: 6422 2074 7970 653d 2249 4452 4546 2220  d" type="IDREF" 
+000011a0: 6964 3d22 6469 7669 6465 725f 7265 6622  id="divider_ref"
+000011b0: 202f 3e0a 2020 2020 2020 2020 3c61 7474   />.        <att
+000011c0: 7269 6275 7465 206e 616d 653d 226c 6f63  ribute name="loc
+000011d0: 6174 696f 6e22 2075 7365 3d22 7265 7175  ation" use="requ
+000011e0: 6972 6564 2220 7479 7065 3d22 6461 7461  ired" type="data
+000011f0: 2d74 7970 653a 466c 6f61 7436 345f 5479  -type:Float64_Ty
+00001200: 7065 2220 6964 3d22 6c6f 6361 7469 6f6e  pe" id="location
+00001210: 5f76 616c 7565 2220 2f3e 0a20 2020 203c  _value" />.    <
+00001220: 2f63 6f6d 706c 6578 5479 7065 3e0a 0a20  /complexType>.. 
+00001230: 2020 203c 636f 6d70 6c65 7854 7970 6520     <complexType 
+00001240: 6e61 6d65 3d22 5265 6374 616e 676c 6547  name="RectangleG
+00001250: 6174 655f 5479 7065 223e 0a20 2020 2020  ate_Type">.     
+00001260: 2020 203c 636f 6d70 6c65 7843 6f6e 7465     <complexConte
+00001270: 6e74 3e0a 2020 2020 2020 2020 2020 2020  nt>.            
+00001280: 3c65 7874 656e 7369 6f6e 2062 6173 653d  <extension base=
+00001290: 2267 6174 696e 673a 4162 7374 7261 6374  "gating:Abstract
+000012a0: 4761 7465 5f54 7970 6522 3e0a 2020 2020  Gate_Type">.    
+000012b0: 2020 2020 2020 2020 2020 2020 3c73 6571              <seq
+000012c0: 7565 6e63 653e 0a20 2020 2020 2020 2020  uence>.         
+000012d0: 2020 2020 2020 2020 2020 203c 656c 656d             <elem
+000012e0: 656e 7420 6e61 6d65 3d22 6469 6d65 6e73  ent name="dimens
+000012f0: 696f 6e22 2074 7970 653d 2267 6174 696e  ion" type="gatin
+00001300: 673a 5265 6374 616e 676c 6547 6174 6544  g:RectangleGateD
+00001310: 696d 656e 7369 6f6e 5f54 7970 6522 206d  imension_Type" m
+00001320: 6178 4f63 6375 7273 3d22 756e 626f 756e  axOccurs="unboun
+00001330: 6465 6422 2069 643d 2264 696d 656e 7369  ded" id="dimensi
+00001340: 6f6e 2220 2f3e 0a20 2020 2020 2020 2020  on" />.         
+00001350: 2020 2020 2020 203c 2f73 6571 7565 6e63         </sequenc
+00001360: 653e 0a20 2020 2020 2020 2020 2020 203c  e>.            <
+00001370: 2f65 7874 656e 7369 6f6e 3e0a 2020 2020  /extension>.    
+00001380: 2020 2020 3c2f 636f 6d70 6c65 7843 6f6e      </complexCon
+00001390: 7465 6e74 3e0a 2020 2020 3c2f 636f 6d70  tent>.    </comp
+000013a0: 6c65 7854 7970 653e 0a0a 2020 2020 3c63  lexType>..    <c
+000013b0: 6f6d 706c 6578 5479 7065 206e 616d 653d  omplexType name=
+000013c0: 2250 6f6c 7967 6f6e 4761 7465 5f54 7970  "PolygonGate_Typ
+000013d0: 6522 3e0a 2020 2020 2020 2020 3c63 6f6d  e">.        <com
+000013e0: 706c 6578 436f 6e74 656e 743e 0a20 2020  plexContent>.   
+000013f0: 2020 2020 2020 2020 203c 6578 7465 6e73           <extens
+00001400: 696f 6e20 6261 7365 3d22 6761 7469 6e67  ion base="gating
+00001410: 3a41 6273 7472 6163 7447 6174 655f 5479  :AbstractGate_Ty
+00001420: 7065 223e 0a20 2020 2020 2020 2020 2020  pe">.           
+00001430: 2020 2020 203c 7365 7175 656e 6365 3e0a       <sequence>.
+00001440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001450: 2020 2020 3c65 6c65 6d65 6e74 206e 616d      <element nam
+00001460: 653d 2264 696d 656e 7369 6f6e 2220 7479  e="dimension" ty
+00001470: 7065 3d22 6761 7469 6e67 3a44 696d 656e  pe="gating:Dimen
+00001480: 7369 6f6e 5f54 7970 6522 206d 696e 4f63  sion_Type" minOc
+00001490: 6375 7273 3d22 3222 206d 6178 4f63 6375  curs="2" maxOccu
+000014a0: 7273 3d22 3222 202f 3e0a 2020 2020 2020  rs="2" />.      
+000014b0: 2020 2020 2020 2020 2020 2020 2020 3c65                <e
+000014c0: 6c65 6d65 6e74 206e 616d 653d 2276 6572  lement name="ver
+000014d0: 7465 7822 2074 7970 653d 2267 6174 696e  tex" type="gatin
+000014e0: 673a 506f 696e 7432 445f 5479 7065 2220  g:Point2D_Type" 
+000014f0: 6d69 6e4f 6363 7572 733d 2233 2220 6d61  minOccurs="3" ma
+00001500: 784f 6363 7572 733d 2275 6e62 6f75 6e64  xOccurs="unbound
+00001510: 6564 2220 2f3e 0a20 2020 2020 2020 2020  ed" />.         
+00001520: 2020 2020 2020 203c 2f73 6571 7565 6e63         </sequenc
+00001530: 653e 0a20 2020 2020 2020 2020 2020 203c  e>.            <
+00001540: 2f65 7874 656e 7369 6f6e 3e0a 2020 2020  /extension>.    
+00001550: 2020 2020 3c2f 636f 6d70 6c65 7843 6f6e      </complexCon
+00001560: 7465 6e74 3e0a 2020 2020 3c2f 636f 6d70  tent>.    </comp
+00001570: 6c65 7854 7970 653e 0a0a 2020 2020 3c63  lexType>..    <c
+00001580: 6f6d 706c 6578 5479 7065 206e 616d 653d  omplexType name=
+00001590: 2245 6c6c 6970 736f 6964 4761 7465 5f54  "EllipsoidGate_T
+000015a0: 7970 6522 3e0a 2020 2020 2020 2020 3c63  ype">.        <c
+000015b0: 6f6d 706c 6578 436f 6e74 656e 743e 0a20  omplexContent>. 
+000015c0: 2020 2020 2020 2020 2020 203c 6578 7465             <exte
+000015d0: 6e73 696f 6e20 6261 7365 3d22 6761 7469  nsion base="gati
+000015e0: 6e67 3a41 6273 7472 6163 7447 6174 655f  ng:AbstractGate_
+000015f0: 5479 7065 223e 0a20 2020 2020 2020 2020  Type">.         
+00001600: 2020 2020 2020 203c 7365 7175 656e 6365         <sequence
+00001610: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00001620: 2020 2020 2020 3c65 6c65 6d65 6e74 206e        <element n
+00001630: 616d 653d 2264 696d 656e 7369 6f6e 2220  ame="dimension" 
+00001640: 7479 7065 3d22 6761 7469 6e67 3a44 696d  type="gating:Dim
+00001650: 656e 7369 6f6e 5f54 7970 6522 206d 696e  ension_Type" min
+00001660: 4f63 6375 7273 3d22 3222 206d 6178 4f63  Occurs="2" maxOc
+00001670: 6375 7273 3d22 756e 626f 756e 6465 6422  curs="unbounded"
+00001680: 202f 3e0a 2020 2020 2020 2020 2020 2020   />.            
+00001690: 2020 2020 2020 2020 3c65 6c65 6d65 6e74          <element
+000016a0: 206e 616d 653d 226d 6561 6e22 2074 7970   name="mean" typ
+000016b0: 653d 2267 6174 696e 673a 506f 696e 7458  e="gating:PointX
+000016c0: 445f 5479 7065 2220 6d69 6e4f 6363 7572  D_Type" minOccur
+000016d0: 733d 2231 2220 6d61 784f 6363 7572 733d  s="1" maxOccurs=
+000016e0: 2231 2220 2f3e 0a20 2020 2020 2020 2020  "1" />.         
+000016f0: 2020 2020 2020 2020 2020 203c 656c 656d             <elem
+00001700: 656e 7420 6e61 6d65 3d22 636f 7661 7269  ent name="covari
+00001710: 616e 6365 4d61 7472 6978 2220 7479 7065  anceMatrix" type
+00001720: 3d22 6761 7469 6e67 3a4d 6174 7269 785f  ="gating:Matrix_
+00001730: 5479 7065 2220 6d69 6e4f 6363 7572 733d  Type" minOccurs=
+00001740: 2231 2220 6d61 784f 6363 7572 733d 2231  "1" maxOccurs="1
+00001750: 2220 2f3e 0a20 2020 2020 2020 2020 2020  " />.           
+00001760: 2020 2020 2020 2020 203c 656c 656d 656e           <elemen
+00001770: 7420 6e61 6d65 3d22 6469 7374 616e 6365  t name="distance
+00001780: 5371 7561 7265 2220 7479 7065 3d22 6461  Square" type="da
+00001790: 7461 2d74 7970 653a 5556 616c 7565 4174  ta-type:UValueAt
+000017a0: 7472 6962 7574 655f 5479 7065 2220 6d69  tribute_Type" mi
+000017b0: 6e4f 6363 7572 733d 2231 2220 6d61 784f  nOccurs="1" maxO
+000017c0: 6363 7572 733d 2231 2220 2f3e 0a20 2020  ccurs="1" />.   
+000017d0: 2020 2020 2020 2020 2020 2020 203c 2f73               </s
+000017e0: 6571 7565 6e63 653e 0a20 2020 2020 2020  equence>.       
+000017f0: 2020 2020 203c 2f65 7874 656e 7369 6f6e       </extension
+00001800: 3e0a 2020 2020 2020 2020 3c2f 636f 6d70  >.        </comp
+00001810: 6c65 7843 6f6e 7465 6e74 3e0a 2020 2020  lexContent>.    
+00001820: 3c2f 636f 6d70 6c65 7854 7970 653e 0a0a  </complexType>..
+00001830: 2020 2020 3c63 6f6d 706c 6578 5479 7065      <complexType
+00001840: 206e 616d 653d 2242 6f6f 6c65 616e 4761   name="BooleanGa
+00001850: 7465 5f54 7970 6522 3e0a 2020 2020 2020  te_Type">.      
+00001860: 2020 3c63 6f6d 706c 6578 436f 6e74 656e    <complexConten
+00001870: 743e 0a20 2020 2020 2020 2020 2020 203c  t>.            <
+00001880: 6578 7465 6e73 696f 6e20 6261 7365 3d22  extension base="
+00001890: 6761 7469 6e67 3a41 6273 7472 6163 7447  gating:AbstractG
+000018a0: 6174 655f 5479 7065 223e 0a20 2020 2020  ate_Type">.     
+000018b0: 2020 2020 2020 2020 2020 203c 7365 7175             <sequ
+000018c0: 656e 6365 3e0a 2020 2020 2020 2020 2020  ence>.          
+000018d0: 2020 2020 2020 2020 2020 3c63 686f 6963            <choic
+000018e0: 653e 0a20 2020 2020 2020 2020 2020 2020  e>.             
+000018f0: 2020 2020 2020 2020 2020 203c 656c 656d             <elem
+00001900: 656e 7420 6e61 6d65 3d22 616e 6422 2074  ent name="and" t
+00001910: 7970 653d 2267 6174 696e 673a 5477 6f41  ype="gating:TwoA
+00001920: 6e64 4d6f 7265 4f70 6572 616e 6473 5f42  ndMoreOperands_B
+00001930: 6f6f 6c47 6174 655f 5479 7065 2220 6964  oolGate_Type" id
+00001940: 3d22 616e 6422 202f 3e0a 2020 2020 2020  ="and" />.      
+00001950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001960: 2020 3c65 6c65 6d65 6e74 206e 616d 653d    <element name=
+00001970: 226f 7222 2074 7970 653d 2267 6174 696e  "or" type="gatin
+00001980: 673a 5477 6f41 6e64 4d6f 7265 4f70 6572  g:TwoAndMoreOper
+00001990: 616e 6473 5f42 6f6f 6c47 6174 655f 5479  ands_BoolGate_Ty
+000019a0: 7065 2220 6964 3d22 6f72 2220 2f3e 0a20  pe" id="or" />. 
+000019b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019c0: 2020 2020 2020 203c 656c 656d 656e 7420         <element 
+000019d0: 6e61 6d65 3d22 6e6f 7422 2074 7970 653d  name="not" type=
+000019e0: 2267 6174 696e 673a 4f6e 654f 7065 7261  "gating:OneOpera
+000019f0: 6e64 5f42 6f6f 6c47 6174 655f 5479 7065  nd_BoolGate_Type
+00001a00: 2220 6964 3d22 6e6f 7422 202f 3e0a 2020  " id="not" />.  
+00001a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a20: 2020 3c2f 6368 6f69 6365 3e0a 2020 2020    </choice>.    
+00001a30: 2020 2020 2020 2020 2020 2020 3c2f 7365              </se
+00001a40: 7175 656e 6365 3e0a 2020 2020 2020 2020  quence>.        
+00001a50: 2020 2020 3c2f 6578 7465 6e73 696f 6e3e      </extension>
+00001a60: 0a20 2020 2020 2020 203c 2f63 6f6d 706c  .        </compl
+00001a70: 6578 436f 6e74 656e 743e 0a20 2020 203c  exContent>.    <
+00001a80: 2f63 6f6d 706c 6578 5479 7065 3e0a 0a20  /complexType>.. 
+00001a90: 2020 203c 636f 6d70 6c65 7854 7970 6520     <complexType 
+00001aa0: 6e61 6d65 3d22 4469 6d65 6e73 696f 6e5f  name="Dimension_
+00001ab0: 5479 7065 223e 0a20 2020 2020 2020 203c  Type">.        <
+00001ac0: 616e 6e6f 7461 7469 6f6e 3e0a 2020 2020  annotation>.    
+00001ad0: 2020 2020 2020 2020 3c64 6f63 756d 656e          <documen
+00001ae0: 7461 7469 6f6e 2078 6d6c 3a6c 616e 673d  tation xml:lang=
+00001af0: 2265 6e22 3e46 4353 2064 696d 656e 7369  "en">FCS dimensi
+00001b00: 6f6e 2070 6c75 7320 7472 616e 7366 6f72  on plus transfor
+00001b10: 6d61 7469 6f6e 2028 6f70 7469 6f6e 616c  mation (optional
+00001b20: 2920 616e 6420 636f 6d70 656e 7361 7469  ) and compensati
+00001b30: 6f6e 2072 6566 6572 656e 6365 7320 2872  on references (r
+00001b40: 6571 7569 7265 643a 2063 686f 6963 6520  equired: choice 
+00001b50: 2775 6e63 6f6d 7065 6e73 6174 6564 272c  'uncompensated',
+00001b60: 2027 4643 5327 206f 7220 6964 206f 6620   'FCS' or id of 
+00001b70: 6120 7370 696c 6c6f 7665 7220 6d61 7472  a spillover matr
+00001b80: 6978 292e 3c2f 646f 6375 6d65 6e74 6174  ix).</documentat
+00001b90: 696f 6e3e 0a20 2020 2020 2020 203c 2f61  ion>.        </a
+00001ba0: 6e6e 6f74 6174 696f 6e3e 0a20 2020 2020  nnotation>.     
+00001bb0: 2020 203c 6772 6f75 7020 7265 663d 2264     <group ref="d
+00001bc0: 6174 612d 7479 7065 3a44 696d 656e 7369  ata-type:Dimensi
+00001bd0: 6f6e 735f 4772 6f75 7022 202f 3e0a 2020  ons_Group" />.  
+00001be0: 2020 2020 2020 3c61 7474 7269 6275 7465        <attribute
+00001bf0: 206e 616d 653d 2274 7261 6e73 666f 726d   name="transform
+00001c00: 6174 696f 6e2d 7265 6622 2074 7970 653d  ation-ref" type=
+00001c10: 2249 4452 4546 2220 7573 653d 226f 7074  "IDREF" use="opt
+00001c20: 696f 6e61 6c22 202f 3e0a 2020 2020 2020  ional" />.      
+00001c30: 2020 3c61 7474 7269 6275 7465 206e 616d    <attribute nam
+00001c40: 653d 2263 6f6d 7065 6e73 6174 696f 6e2d  e="compensation-
+00001c50: 7265 6622 2074 7970 653d 2264 6174 612d  ref" type="data-
+00001c60: 7479 7065 3a4e 6f6e 456d 7074 7953 7472  type:NonEmptyStr
+00001c70: 696e 675f 5479 7065 2220 7573 653d 2272  ing_Type" use="r
+00001c80: 6571 7569 7265 6422 202f 3e0a 2020 2020  equired" />.    
+00001c90: 3c2f 636f 6d70 6c65 7854 7970 653e 0a0a  </complexType>..
+00001ca0: 2020 2020 3c63 6f6d 706c 6578 5479 7065      <complexType
+00001cb0: 206e 616d 653d 2252 6563 7461 6e67 6c65   name="Rectangle
+00001cc0: 4761 7465 4469 6d65 6e73 696f 6e5f 5479  GateDimension_Ty
+00001cd0: 7065 223e 0a20 2020 2020 2020 203c 616e  pe">.        <an
+00001ce0: 6e6f 7461 7469 6f6e 3e0a 2020 2020 2020  notation>.      
+00001cf0: 2020 2020 2020 3c64 6f63 756d 656e 7461        <documenta
+00001d00: 7469 6f6e 3e41 2064 696d 656e 7369 6f6e  tion>A dimension
+00001d10: 2074 7970 6520 666f 7220 6120 7265 6374   type for a rect
+00001d20: 616e 676c 6520 6761 7465 3b20 7468 6520  angle gate; the 
+00001d30: 636f 6d6d 6f6e 2064 696d 656e 7369 6f6e  common dimension
+00001d40: 2069 7320 6578 7465 6e64 6564 2062 7920   is extended by 
+00001d50: 7468 6520 6d69 6e20 616e 6420 6d61 7820  the min and max 
+00001d60: 6174 7472 6962 7574 6573 2e20 3c2f 646f  attributes. </do
+00001d70: 6375 6d65 6e74 6174 696f 6e3e 0a20 2020  cumentation>.   
+00001d80: 2020 2020 203c 2f61 6e6e 6f74 6174 696f       </annotatio
+00001d90: 6e3e 0a20 2020 2020 2020 203c 636f 6d70  n>.        <comp
+00001da0: 6c65 7843 6f6e 7465 6e74 3e0a 2020 2020  lexContent>.    
+00001db0: 2020 2020 2020 2020 3c65 7874 656e 7369          <extensi
+00001dc0: 6f6e 2062 6173 653d 2267 6174 696e 673a  on base="gating:
+00001dd0: 4469 6d65 6e73 696f 6e5f 5479 7065 223e  Dimension_Type">
+00001de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001df0: 203c 6174 7472 6962 7574 6520 6e61 6d65   <attribute name
+00001e00: 3d22 6d69 6e22 2074 7970 653d 2264 6174  ="min" type="dat
+00001e10: 612d 7479 7065 3a46 6c6f 6174 3634 5f54  a-type:Float64_T
+00001e20: 7970 6522 2075 7365 3d22 6f70 7469 6f6e  ype" use="option
+00001e30: 616c 2220 6964 3d22 6d69 6e22 202f 3e0a  al" id="min" />.
+00001e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e50: 3c61 7474 7269 6275 7465 206e 616d 653d  <attribute name=
+00001e60: 226d 6178 2220 7479 7065 3d22 6461 7461  "max" type="data
+00001e70: 2d74 7970 653a 466c 6f61 7436 345f 5479  -type:Float64_Ty
+00001e80: 7065 2220 7573 653d 226f 7074 696f 6e61  pe" use="optiona
+00001e90: 6c22 2069 643d 226d 6178 2220 2f3e 0a20  l" id="max" />. 
+00001ea0: 2020 2020 2020 2020 2020 203c 2f65 7874             </ext
+00001eb0: 656e 7369 6f6e 3e0a 2020 2020 2020 2020  ension>.        
+00001ec0: 3c2f 636f 6d70 6c65 7843 6f6e 7465 6e74  </complexContent
+00001ed0: 3e0a 2020 2020 3c2f 636f 6d70 6c65 7854  >.    </complexT
+00001ee0: 7970 653e 0a0a 2020 2020 3c63 6f6d 706c  ype>..    <compl
+00001ef0: 6578 5479 7065 206e 616d 653d 2250 6f69  exType name="Poi
+00001f00: 6e74 5f54 7970 6522 3e0a 2020 2020 2020  nt_Type">.      
+00001f10: 2020 3c61 6e6e 6f74 6174 696f 6e3e 0a20    <annotation>. 
+00001f20: 2020 2020 2020 2020 2020 203c 646f 6375             <docu
+00001f30: 6d65 6e74 6174 696f 6e3e 4120 706f 696e  mentation>A poin
+00001f40: 7420 6973 2061 2073 6571 7565 6e63 6520  t is a sequence 
+00001f50: 6f66 2063 6f6f 7264 696e 6174 6573 2e3c  of coordinates.<
+00001f60: 2f64 6f63 756d 656e 7461 7469 6f6e 3e0a  /documentation>.
+00001f70: 2020 2020 2020 2020 3c2f 616e 6e6f 7461          </annota
+00001f80: 7469 6f6e 3e0a 2020 2020 2020 2020 3c73  tion>.        <s
+00001f90: 6571 7565 6e63 653e 0a20 2020 2020 2020  equence>.       
+00001fa0: 2020 2020 203c 656c 656d 656e 7420 6e61       <element na
+00001fb0: 6d65 3d22 636f 6f72 6469 6e61 7465 2220  me="coordinate" 
+00001fc0: 7479 7065 3d22 6461 7461 2d74 7970 653a  type="data-type:
+00001fd0: 5661 6c75 6541 7474 7269 6275 7465 5f54  ValueAttribute_T
+00001fe0: 7970 6522 206d 6178 4f63 6375 7273 3d22  ype" maxOccurs="
+00001ff0: 756e 626f 756e 6465 6422 2069 643d 2263  unbounded" id="c
+00002000: 6f6f 7264 696e 6174 6522 202f 3e0a 2020  oordinate" />.  
+00002010: 2020 2020 2020 3c2f 7365 7175 656e 6365        </sequence
+00002020: 3e0a 2020 2020 3c2f 636f 6d70 6c65 7854  >.    </complexT
+00002030: 7970 653e 0a0a 2020 2020 3c63 6f6d 706c  ype>..    <compl
+00002040: 6578 5479 7065 206e 616d 653d 2250 6f69  exType name="Poi
+00002050: 6e74 3244 5f54 7970 6522 3e0a 2020 2020  nt2D_Type">.    
+00002060: 2020 2020 3c61 6e6e 6f74 6174 696f 6e3e      <annotation>
+00002070: 0a20 2020 2020 2020 2020 2020 203c 646f  .            <do
+00002080: 6375 6d65 6e74 6174 696f 6e3e 4120 3244  cumentation>A 2D
+00002090: 2070 6f69 6e74 2069 7320 6120 7365 7175   point is a sequ
+000020a0: 656e 6365 206f 6620 7477 6f20 636f 6f72  ence of two coor
+000020b0: 6469 6e61 7465 732e 3c2f 646f 6375 6d65  dinates.</docume
+000020c0: 6e74 6174 696f 6e3e 0a20 2020 2020 2020  ntation>.       
+000020d0: 203c 2f61 6e6e 6f74 6174 696f 6e3e 0a20   </annotation>. 
+000020e0: 2020 2020 2020 203c 636f 6d70 6c65 7843         <complexC
+000020f0: 6f6e 7465 6e74 3e0a 2020 2020 2020 2020  ontent>.        
+00002100: 2020 2020 3c72 6573 7472 6963 7469 6f6e      <restriction
+00002110: 2062 6173 653d 2267 6174 696e 673a 506f   base="gating:Po
+00002120: 696e 745f 5479 7065 223e 0a20 2020 2020  int_Type">.     
+00002130: 2020 2020 2020 2020 2020 203c 7365 7175             <sequ
+00002140: 656e 6365 3e0a 2020 2020 2020 2020 2020  ence>.          
+00002150: 2020 2020 2020 2020 2020 3c65 6c65 6d65            <eleme
+00002160: 6e74 206e 616d 653d 2263 6f6f 7264 696e  nt name="coordin
+00002170: 6174 6522 2074 7970 653d 2264 6174 612d  ate" type="data-
+00002180: 7479 7065 3a56 616c 7565 4174 7472 6962  type:ValueAttrib
+00002190: 7574 655f 5479 7065 2220 6d69 6e4f 6363  ute_Type" minOcc
+000021a0: 7572 733d 2232 2220 6d61 784f 6363 7572  urs="2" maxOccur
+000021b0: 733d 2232 2220 2f3e 0a20 2020 2020 2020  s="2" />.       
+000021c0: 2020 2020 2020 2020 203c 2f73 6571 7565           </seque
+000021d0: 6e63 653e 0a20 2020 2020 2020 2020 2020  nce>.           
+000021e0: 203c 2f72 6573 7472 6963 7469 6f6e 3e0a   </restriction>.
+000021f0: 2020 2020 2020 2020 3c2f 636f 6d70 6c65          </comple
+00002200: 7843 6f6e 7465 6e74 3e0a 2020 2020 3c2f  xContent>.    </
+00002210: 636f 6d70 6c65 7854 7970 653e 0a0a 2020  complexType>..  
+00002220: 2020 3c63 6f6d 706c 6578 5479 7065 206e    <complexType n
+00002230: 616d 653d 2250 6f69 6e74 5844 5f54 7970  ame="PointXD_Typ
+00002240: 6522 3e0a 2020 2020 2020 2020 3c61 6e6e  e">.        <ann
+00002250: 6f74 6174 696f 6e3e 0a20 2020 2020 2020  otation>.       
+00002260: 2020 2020 203c 646f 6375 6d65 6e74 6174       <documentat
+00002270: 696f 6e3e 4120 3220 6f72 206d 6f72 6520  ion>A 2 or more 
+00002280: 6469 6d65 6e73 696f 6e61 6c20 706f 696e  dimensional poin
+00002290: 7420 6973 2061 2073 6571 7565 6e63 6520  t is a sequence 
+000022a0: 6f66 2074 776f 206f 7220 6d6f 7265 2063  of two or more c
+000022b0: 6f6f 7264 696e 6174 6573 2e3c 2f64 6f63  oordinates.</doc
+000022c0: 756d 656e 7461 7469 6f6e 3e0a 2020 2020  umentation>.    
+000022d0: 2020 2020 3c2f 616e 6e6f 7461 7469 6f6e      </annotation
+000022e0: 3e0a 2020 2020 2020 2020 3c63 6f6d 706c  >.        <compl
+000022f0: 6578 436f 6e74 656e 743e 0a20 2020 2020  exContent>.     
+00002300: 2020 2020 2020 203c 7265 7374 7269 6374         <restrict
+00002310: 696f 6e20 6261 7365 3d22 6761 7469 6e67  ion base="gating
+00002320: 3a50 6f69 6e74 5f54 7970 6522 3e0a 2020  :Point_Type">.  
+00002330: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
+00002340: 6571 7565 6e63 653e 0a20 2020 2020 2020  equence>.       
+00002350: 2020 2020 2020 2020 2020 2020 203c 656c               <el
+00002360: 656d 656e 7420 6e61 6d65 3d22 636f 6f72  ement name="coor
+00002370: 6469 6e61 7465 2220 7479 7065 3d22 6461  dinate" type="da
+00002380: 7461 2d74 7970 653a 5661 6c75 6541 7474  ta-type:ValueAtt
+00002390: 7269 6275 7465 5f54 7970 6522 206d 696e  ribute_Type" min
+000023a0: 4f63 6375 7273 3d22 3222 206d 6178 4f63  Occurs="2" maxOc
+000023b0: 6375 7273 3d22 756e 626f 756e 6465 6422  curs="unbounded"
+000023c0: 202f 3e0a 2020 2020 2020 2020 2020 2020   />.            
+000023d0: 2020 2020 3c2f 7365 7175 656e 6365 3e0a      </sequence>.
+000023e0: 2020 2020 2020 2020 2020 2020 3c2f 7265              </re
+000023f0: 7374 7269 6374 696f 6e3e 0a20 2020 2020  striction>.     
+00002400: 2020 203c 2f63 6f6d 706c 6578 436f 6e74     </complexCont
+00002410: 656e 743e 0a20 2020 203c 2f63 6f6d 706c  ent>.    </compl
+00002420: 6578 5479 7065 3e0a 0a20 2020 203c 636f  exType>..    <co
+00002430: 6d70 6c65 7854 7970 6520 6e61 6d65 3d22  mplexType name="
+00002440: 4d61 7472 6978 5f54 7970 6522 3e0a 2020  Matrix_Type">.  
+00002450: 2020 2020 2020 3c61 6e6e 6f74 6174 696f        <annotatio
+00002460: 6e3e 0a20 2020 2020 2020 2020 2020 203c  n>.            <
+00002470: 646f 6375 6d65 6e74 6174 696f 6e3e 4465  documentation>De
+00002480: 7363 7269 7074 696f 6e20 6f66 2061 206d  scription of a m
+00002490: 6174 7269 782e 3c2f 646f 6375 6d65 6e74  atrix.</document
+000024a0: 6174 696f 6e3e 0a20 2020 2020 2020 203c  ation>.        <
+000024b0: 2f61 6e6e 6f74 6174 696f 6e3e 0a20 2020  /annotation>.   
+000024c0: 2020 2020 203c 7365 7175 656e 6365 3e0a       <sequence>.
+000024d0: 2020 2020 2020 2020 2020 2020 3c65 6c65              <ele
+000024e0: 6d65 6e74 206e 616d 653d 2272 6f77 2220  ment name="row" 
+000024f0: 7479 7065 3d22 6761 7469 6e67 3a4d 6174  type="gating:Mat
+00002500: 7269 7852 6f77 5f54 7970 6522 206d 696e  rixRow_Type" min
+00002510: 4f63 6375 7273 3d22 3122 206d 6178 4f63  Occurs="1" maxOc
+00002520: 6375 7273 3d22 756e 626f 756e 6465 6422  curs="unbounded"
+00002530: 202f 3e0a 2020 2020 2020 2020 3c2f 7365   />.        </se
+00002540: 7175 656e 6365 3e0a 2020 2020 3c2f 636f  quence>.    </co
+00002550: 6d70 6c65 7854 7970 653e 0a0a 2020 2020  mplexType>..    
+00002560: 3c63 6f6d 706c 6578 5479 7065 206e 616d  <complexType nam
+00002570: 653d 224d 6174 7269 7852 6f77 5f54 7970  e="MatrixRow_Typ
+00002580: 6522 3e0a 2020 2020 2020 2020 3c61 6e6e  e">.        <ann
+00002590: 6f74 6174 696f 6e3e 0a20 2020 2020 2020  otation>.       
+000025a0: 2020 2020 203c 646f 6375 6d65 6e74 6174       <documentat
+000025b0: 696f 6e3e 4465 7363 7269 7074 696f 6e20  ion>Description 
+000025c0: 6f66 2061 2072 6f77 206f 6620 6120 6d61  of a row of a ma
+000025d0: 7472 6978 2e3c 2f64 6f63 756d 656e 7461  trix.</documenta
+000025e0: 7469 6f6e 3e0a 2020 2020 2020 2020 3c2f  tion>.        </
+000025f0: 616e 6e6f 7461 7469 6f6e 3e0a 2020 2020  annotation>.    
+00002600: 2020 2020 3c73 6571 7565 6e63 653e 0a20      <sequence>. 
+00002610: 2020 2020 2020 2020 2020 203c 656c 656d             <elem
+00002620: 656e 7420 6e61 6d65 3d22 656e 7472 7922  ent name="entry"
+00002630: 2074 7970 653d 2264 6174 612d 7479 7065   type="data-type
+00002640: 3a56 616c 7565 4174 7472 6962 7574 655f  :ValueAttribute_
+00002650: 5479 7065 2220 6d69 6e4f 6363 7572 733d  Type" minOccurs=
+00002660: 2231 220a 2020 2020 2020 2020 2020 2020  "1".            
+00002670: 2020 2020 6d61 784f 6363 7572 733d 2275      maxOccurs="u
+00002680: 6e62 6f75 6e64 6564 2220 2f3e 0a20 2020  nbounded" />.   
+00002690: 2020 2020 203c 2f73 6571 7565 6e63 653e       </sequence>
+000026a0: 0a20 2020 203c 2f63 6f6d 706c 6578 5479  .    </complexTy
+000026b0: 7065 3e0a 0a20 2020 203c 6772 6f75 7020  pe>..    <group 
+000026c0: 6e61 6d65 3d22 426f 6f6c 4761 7465 4f70  name="BoolGateOp
+000026d0: 6572 616e 6473 5f47 726f 7570 223e 0a20  erands_Group">. 
+000026e0: 2020 2020 2020 203c 616e 6e6f 7461 7469         <annotati
+000026f0: 6f6e 3e0a 2020 2020 2020 2020 2020 2020  on>.            
+00002700: 3c64 6f63 756d 656e 7461 7469 6f6e 2078  <documentation x
+00002710: 6d6c 3a6c 616e 673d 2265 6e22 3e41 6e20  ml:lang="en">An 
+00002720: 6f70 6572 616e 6420 6f66 2061 2042 6f6f  operand of a Boo
+00002730: 6c65 616e 2067 6174 6520 6361 6e20 6265  lean gate can be
+00002740: 2073 7065 6369 6669 6564 2061 7320 6761   specified as ga
+00002750: 7465 5265 6665 7265 6e63 6520 6f72 2061  teReference or a
+00002760: 7320 616e 2065 6d62 6564 6465 6420 7370  s an embedded sp
+00002770: 6563 6966 6963 6174 696f 6e20 6f66 2061  ecification of a
+00002780: 6e6f 7468 6572 2067 6174 652e 3c2f 646f  nother gate.</do
+00002790: 6375 6d65 6e74 6174 696f 6e3e 0a20 2020  cumentation>.   
+000027a0: 2020 2020 203c 2f61 6e6e 6f74 6174 696f       </annotatio
+000027b0: 6e3e 0a20 2020 2020 2020 203c 6368 6f69  n>.        <choi
+000027c0: 6365 3e0a 2020 2020 2020 2020 2020 2020  ce>.            
+000027d0: 3c65 6c65 6d65 6e74 206e 616d 653d 2267  <element name="g
+000027e0: 6174 6552 6566 6572 656e 6365 2220 7479  ateReference" ty
+000027f0: 7065 3d22 6761 7469 6e67 3a47 6174 6552  pe="gating:GateR
+00002800: 6566 6572 656e 6365 5f54 7970 6522 2069  eference_Type" i
+00002810: 643d 2267 6174 6552 6566 6572 656e 6365  d="gateReference
+00002820: 2220 2f3e 0a20 2020 2020 2020 203c 2f63  " />.        </c
+00002830: 686f 6963 653e 0a20 2020 203c 2f67 726f  hoice>.    </gro
+00002840: 7570 3e0a 0a20 2020 203c 636f 6d70 6c65  up>..    <comple
+00002850: 7854 7970 6520 6e61 6d65 3d22 5477 6f41  xType name="TwoA
+00002860: 6e64 4d6f 7265 4f70 6572 616e 6473 5f42  ndMoreOperands_B
+00002870: 6f6f 6c47 6174 655f 5479 7065 223e 0a20  oolGate_Type">. 
+00002880: 2020 2020 2020 203c 616e 6e6f 7461 7469         <annotati
+00002890: 6f6e 3e0a 2020 2020 2020 2020 2020 2020  on>.            
+000028a0: 3c64 6f63 756d 656e 7461 7469 6f6e 2078  <documentation x
+000028b0: 6d6c 3a6c 616e 673d 2265 6e22 3e54 6865  ml:lang="en">The
+000028c0: 2074 7970 6520 6f66 2042 6f6f 6c65 616e   type of Boolean
+000028d0: 2067 6174 6573 2077 6974 6820 7477 6f20   gates with two 
+000028e0: 6f72 206d 6f72 6520 6f70 6572 616e 6473  or more operands
+000028f0: 2028 414e 4420 616e 6420 4f52 2067 6174   (AND and OR gat
+00002900: 6573 292e 3c2f 646f 6375 6d65 6e74 6174  es).</documentat
+00002910: 696f 6e3e 0a20 2020 2020 2020 203c 2f61  ion>.        </a
+00002920: 6e6e 6f74 6174 696f 6e3e 0a20 2020 2020  nnotation>.     
+00002930: 2020 203c 7365 7175 656e 6365 206d 696e     <sequence min
+00002940: 4f63 6375 7273 3d22 3222 206d 6178 4f63  Occurs="2" maxOc
+00002950: 6375 7273 3d22 756e 626f 756e 6465 6422  curs="unbounded"
+00002960: 3e0a 2020 2020 2020 2020 2020 2020 3c67  >.            <g
+00002970: 726f 7570 2072 6566 3d22 6761 7469 6e67  roup ref="gating
+00002980: 3a42 6f6f 6c47 6174 654f 7065 7261 6e64  :BoolGateOperand
+00002990: 735f 4772 6f75 7022 202f 3e0a 2020 2020  s_Group" />.    
+000029a0: 2020 2020 3c2f 7365 7175 656e 6365 3e0a      </sequence>.
+000029b0: 2020 2020 3c2f 636f 6d70 6c65 7854 7970      </complexTyp
+000029c0: 653e 0a0a 2020 2020 3c63 6f6d 706c 6578  e>..    <complex
+000029d0: 5479 7065 206e 616d 653d 224f 6e65 4f70  Type name="OneOp
+000029e0: 6572 616e 645f 426f 6f6c 4761 7465 5f54  erand_BoolGate_T
+000029f0: 7970 6522 3e0a 2020 2020 2020 2020 3c61  ype">.        <a
+00002a00: 6e6e 6f74 6174 696f 6e3e 0a20 2020 2020  nnotation>.     
+00002a10: 2020 2020 2020 203c 646f 6375 6d65 6e74         <document
+00002a20: 6174 696f 6e20 786d 6c3a 6c61 6e67 3d22  ation xml:lang="
+00002a30: 656e 223e 5468 6520 7479 7065 206f 6620  en">The type of 
+00002a40: 426f 6f6c 6561 6e20 4761 7465 7320 7769  Boolean Gates wi
+00002a50: 7468 2065 7861 6374 6c79 206f 6e65 206f  th exactly one o
+00002a60: 7065 7261 6e64 2028 4e4f 5420 6761 7465  perand (NOT gate
+00002a70: 292e 3c2f 646f 6375 6d65 6e74 6174 696f  ).</documentatio
+00002a80: 6e3e 0a20 2020 2020 2020 203c 2f61 6e6e  n>.        </ann
+00002a90: 6f74 6174 696f 6e3e 0a20 2020 2020 2020  otation>.       
+00002aa0: 203c 7365 7175 656e 6365 3e0a 2020 2020   <sequence>.    
+00002ab0: 2020 2020 2020 2020 3c67 726f 7570 2072          <group r
+00002ac0: 6566 3d22 6761 7469 6e67 3a42 6f6f 6c47  ef="gating:BoolG
+00002ad0: 6174 654f 7065 7261 6e64 735f 4772 6f75  ateOperands_Grou
+00002ae0: 7022 202f 3e0a 2020 2020 2020 2020 3c2f  p" />.        </
+00002af0: 7365 7175 656e 6365 3e0a 2020 2020 3c2f  sequence>.    </
+00002b00: 636f 6d70 6c65 7854 7970 653e 0a0a 2020  complexType>..  
+00002b10: 2020 3c63 6f6d 706c 6578 5479 7065 206e    <complexType n
+00002b20: 616d 653d 2247 6174 6552 6566 6572 656e  ame="GateReferen
+00002b30: 6365 5f54 7970 6522 3e0a 2020 2020 2020  ce_Type">.      
+00002b40: 2020 3c61 6e6e 6f74 6174 696f 6e3e 0a20    <annotation>. 
+00002b50: 2020 2020 2020 2020 2020 203c 646f 6375             <docu
+00002b60: 6d65 6e74 6174 696f 6e20 786d 6c3a 6c61  mentation xml:la
+00002b70: 6e67 3d22 656e 223e 5479 7065 206f 6620  ng="en">Type of 
+00002b80: 6120 7265 6665 7265 6e63 6520 746f 2061  a reference to a
+00002b90: 6e6f 7468 6572 2028 616c 7265 6164 7920  nother (already 
+00002ba0: 6465 6669 6e65 6429 2067 6174 652e 2054  defined) gate. T
+00002bb0: 6865 2061 7474 7269 6275 7465 2072 6566  he attribute ref
+00002bc0: 2072 6566 6572 656e 6365 7320 6120 6761   references a ga
+00002bd0: 7465 2062 7920 6974 7320 6964 2e20 3c2f  te by its id. </
+00002be0: 646f 6375 6d65 6e74 6174 696f 6e3e 0a20  documentation>. 
+00002bf0: 2020 2020 2020 203c 2f61 6e6e 6f74 6174         </annotat
+00002c00: 696f 6e3e 0a20 2020 2020 2020 203c 6174  ion>.        <at
+00002c10: 7472 6962 7574 6520 6e61 6d65 3d22 7265  tribute name="re
+00002c20: 6622 2074 7970 653d 2249 4452 4546 2220  f" type="IDREF" 
+00002c30: 7573 653d 2272 6571 7569 7265 6422 2069  use="required" i
+00002c40: 643d 2272 6566 2220 2f3e 0a20 2020 2020  d="ref" />.     
+00002c50: 2020 203c 6174 7472 6962 7574 6520 6e61     <attribute na
+00002c60: 6d65 3d22 7573 652d 6173 2d63 6f6d 706c  me="use-as-compl
+00002c70: 656d 656e 7422 2074 7970 653d 2262 6f6f  ement" type="boo
+00002c80: 6c65 616e 2220 6465 6661 756c 743d 2266  lean" default="f
+00002c90: 616c 7365 2220 7573 653d 226f 7074 696f  alse" use="optio
+00002ca0: 6e61 6c22 2069 643d 2275 7365 2d61 732d  nal" id="use-as-
+00002cb0: 636f 6d70 6c65 6d65 6e74 2220 2f3e 0a20  complement" />. 
+00002cc0: 2020 203c 2f63 6f6d 706c 6578 5479 7065     </complexType
+00002cd0: 3e0a 0a3c 2f73 6368 656d 613e 0a         >..</schema>.
```

### Comparing `FlowKit-1.0.1/flowkit/_resources/Transformations.v2.0.xsd` & `FlowKit-1.1.0/src/flowkit/_resources/Transformations.v2.0.xsd`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text, with CRLF line terminators*

 * *Files 13% similar despite different names*

```diff
@@ -1,588 +1,576 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
-00000020: 462d 3822 3f3e 0d0a 0d0a 3c73 6368 656d  F-8"?>....<schem
-00000030: 6120 786d 6c6e 733d 2268 7474 703a 2f2f  a xmlns="http://
-00000040: 7777 772e 7733 2e6f 7267 2f32 3030 312f  www.w3.org/2001/
-00000050: 584d 4c53 6368 656d 6122 0d0a 2020 786d  XMLSchema"..  xm
-00000060: 6c6e 733a 7472 616e 7366 6f72 6d73 3d22  lns:transforms="
-00000070: 6874 7470 3a2f 2f77 7777 2e69 7361 632d  http://www.isac-
-00000080: 6e65 742e 6f72 672f 7374 642f 4761 7469  net.org/std/Gati
-00000090: 6e67 2d4d 4c2f 7632 2e30 2f74 7261 6e73  ng-ML/v2.0/trans
-000000a0: 666f 726d 6174 696f 6e73 220d 0a20 2078  formations"..  x
-000000b0: 6d6c 6e73 3a64 6174 612d 7479 7065 3d22  mlns:data-type="
-000000c0: 6874 7470 3a2f 2f77 7777 2e69 7361 632d  http://www.isac-
-000000d0: 6e65 742e 6f72 672f 7374 642f 4761 7469  net.org/std/Gati
-000000e0: 6e67 2d4d 4c2f 7632 2e30 2f64 6174 6174  ng-ML/v2.0/datat
-000000f0: 7970 6573 220d 0a20 2078 6d6c 6e73 3a6d  ypes"..  xmlns:m
-00000100: 6d6c 3d22 6874 7470 3a2f 2f77 7777 2e77  ml="http://www.w
-00000110: 332e 6f72 672f 3139 3938 2f4d 6174 682f  3.org/1998/Math/
-00000120: 4d61 7468 4d4c 220d 0a20 2074 6172 6765  MathML"..  targe
-00000130: 744e 616d 6573 7061 6365 3d22 6874 7470  tNamespace="http
-00000140: 3a2f 2f77 7777 2e69 7361 632d 6e65 742e  ://www.isac-net.
-00000150: 6f72 672f 7374 642f 4761 7469 6e67 2d4d  org/std/Gating-M
-00000160: 4c2f 7632 2e30 2f74 7261 6e73 666f 726d  L/v2.0/transform
-00000170: 6174 696f 6e73 220d 0a20 2065 6c65 6d65  ations"..  eleme
-00000180: 6e74 466f 726d 4465 6661 756c 743d 2271  ntFormDefault="q
-00000190: 7561 6c69 6669 6564 2220 6174 7472 6962  ualified" attrib
-000001a0: 7574 6546 6f72 6d44 6566 6175 6c74 3d22  uteFormDefault="
-000001b0: 7175 616c 6966 6965 6422 2076 6572 7369  qualified" versi
-000001c0: 6f6e 3d22 322e 302e 3132 3132 3037 223e  on="2.0.121207">
-000001d0: 0d0a 0d0a 2020 3c69 6d70 6f72 7420 6e61  ....  <import na
-000001e0: 6d65 7370 6163 653d 2268 7474 703a 2f2f  mespace="http://
-000001f0: 7777 772e 6973 6163 2d6e 6574 2e6f 7267  www.isac-net.org
-00000200: 2f73 7464 2f47 6174 696e 672d 4d4c 2f76  /std/Gating-ML/v
-00000210: 322e 302f 6461 7461 7479 7065 7322 0d0a  2.0/datatypes"..
-00000220: 2020 2020 7363 6865 6d61 4c6f 6361 7469      schemaLocati
-00000230: 6f6e 3d22 4461 7461 5479 7065 732e 7632  on="DataTypes.v2
-00000240: 2e30 2e78 7364 2220 2f3e 0d0a 0d0a 2020  .0.xsd" />....  
-00000250: 3c61 6e6e 6f74 6174 696f 6e3e 0d0a 2020  <annotation>..  
-00000260: 2020 3c61 7070 696e 666f 2073 6f75 7263    <appinfo sourc
-00000270: 653d 2268 7474 703a 2f2f 666c 6f77 6379  e="http://flowcy
-00000280: 742e 736f 7572 6365 666f 7267 652e 6e65  t.sourceforge.ne
-00000290: 742f 223e 5472 616e 7366 6f72 6d61 7469  t/">Transformati
-000002a0: 6f6e 2064 6573 6372 6970 7469 6f6e 7320  on descriptions 
-000002b0: 7769 7468 696e 2047 6174 696e 672d 4d4c  within Gating-ML
-000002c0: 2e3c 2f61 7070 696e 666f 3e0d 0a0d 0a20  .</appinfo>.... 
-000002d0: 2020 203c 646f 6375 6d65 6e74 6174 696f     <documentatio
-000002e0: 6e20 786d 6c3a 6c61 6e67 3d22 656e 2220  n xml:lang="en" 
-000002f0: 736f 7572 6365 3d22 6874 7470 3a2f 2f66  source="http://f
-00000300: 6c6f 7763 7974 2e73 6f75 7263 6566 6f72  lowcyt.sourcefor
-00000310: 6765 2e6e 6574 2f22 3e0d 0a20 2020 2020  ge.net/">..     
-00000320: 203c 6175 7468 6f72 3e0d 0a20 2020 2020   <author>..     
-00000330: 2020 203c 6e61 6d65 3e4a 6f73 6566 2053     <name>Josef S
-00000340: 7069 646c 656e 3c2f 6e61 6d65 3e0d 0a20  pidlen</name>.. 
-00000350: 2020 2020 2020 203c 656d 6169 6c3e 6a73         <email>js
-00000360: 7069 646c 656e 4062 6363 7263 2e63 613c  pidlen@bccrc.ca<
-00000370: 2f65 6d61 696c 3e0d 0a20 2020 2020 203c  /email>..      <
-00000380: 2f61 7574 686f 723e 0d0a 2020 2020 2020  /author>..      
-00000390: 3c63 6f70 7972 6967 6874 3e0d 0a20 2020  <copyright>..   
-000003a0: 2020 2020 2043 6f70 7972 6967 6874 2028       Copyright (
-000003b0: 6329 2032 3030 382d 3230 3134 2049 5341  c) 2008-2014 ISA
-000003c0: 4320 2849 6e74 6572 6e61 7469 6f6e 616c  C (International
-000003d0: 2053 6f63 6965 7479 2066 6f72 2041 6476   Society for Adv
-000003e0: 616e 6365 6d65 6e74 206f 6620 4379 746f  ancement of Cyto
-000003f0: 6d65 7472 7929 0d0a 2020 2020 2020 2020  metry)..        
-00000400: 4672 6565 206f 6620 6368 6172 6765 2064  Free of charge d
-00000410: 6973 7472 6962 7574 696f 6e20 616e 6420  istribution and 
-00000420: 7265 6164 2d6f 6e6c 7920 7573 6167 6520  read-only usage 
-00000430: 7065 726d 6974 6564 2e20 4d6f 6469 6669  permited. Modifi
-00000440: 6361 7469 6f6e 2061 6e64 2061 6c6c 206f  cation and all o
-00000450: 7468 6572 2072 6967 6874 730d 0a20 2020  ther rights..   
-00000460: 2020 2020 2072 6573 6572 7665 642e 2046       reserved. F
-00000470: 6f72 2061 6c6c 206f 7468 6572 2075 7365  or all other use
-00000480: 7320 706c 6561 7365 2063 6f6e 7461 6374  s please contact
-00000490: 2049 5341 432e 200d 0a20 2020 2020 203c   ISAC. ..      <
-000004a0: 2f63 6f70 7972 6967 6874 3e0d 0a20 2020  /copyright>..   
-000004b0: 203c 2f64 6f63 756d 656e 7461 7469 6f6e   </documentation
-000004c0: 3e0d 0a20 203c 2f61 6e6e 6f74 6174 696f  >..  </annotatio
-000004d0: 6e3e 0d0a 0d0a 2020 3c67 726f 7570 206e  n>....  <group n
-000004e0: 616d 653d 2254 7261 6e73 666f 726d 6174  ame="Transformat
-000004f0: 696f 6e5f 4772 6f75 7022 3e0d 0a20 2020  ion_Group">..   
-00000500: 203c 6368 6f69 6365 3e0d 0a20 2020 2020   <choice>..     
-00000510: 2020 203c 656c 656d 656e 7420 6e61 6d65     <element name
-00000520: 3d22 7472 616e 7366 6f72 6d61 7469 6f6e  ="transformation
-00000530: 2220 6964 3d22 7472 616e 7366 6f72 6d61  " id="transforma
-00000540: 7469 6f6e 2220 7479 7065 3d22 7472 616e  tion" type="tran
-00000550: 7366 6f72 6d73 3a74 7261 6e73 666f 726d  sforms:transform
-00000560: 6174 696f 6e5f 5479 7065 2220 2f3e 0d0a  ation_Type" />..
-00000570: 2020 2020 3c2f 6368 6f69 6365 3e0d 0a20      </choice>.. 
-00000580: 203c 2f67 726f 7570 3e0d 0a0d 0a20 203c   </group>....  <
-00000590: 6772 6f75 7020 6e61 6d65 3d22 5370 6563  group name="Spec
-000005a0: 7472 756d 4d61 7472 6978 5f47 726f 7570  trumMatrix_Group
-000005b0: 223e 0d0a 2020 2020 3c63 686f 6963 653e  ">..    <choice>
-000005c0: 0d0a 2020 2020 2020 3c65 6c65 6d65 6e74  ..      <element
-000005d0: 206e 616d 653d 2273 7065 6374 7275 6d4d   name="spectrumM
-000005e0: 6174 7269 7822 2074 7970 653d 2274 7261  atrix" type="tra
-000005f0: 6e73 666f 726d 733a 5370 6563 7472 756d  nsforms:Spectrum
-00000600: 4d61 7472 6978 5f54 7970 6522 202f 3e0d  Matrix_Type" />.
-00000610: 0a20 2020 203c 2f63 686f 6963 653e 0d0a  .    </choice>..
-00000620: 2020 3c2f 6772 6f75 703e 0d0a 0d0a 2020    </group>....  
-00000630: 3c63 6f6d 706c 6578 5479 7065 206e 616d  <complexType nam
-00000640: 653d 2274 7261 6e73 666f 726d 6174 696f  e="transformatio
-00000650: 6e5f 5479 7065 223e 0d0a 2020 2020 3c61  n_Type">..    <a
-00000660: 6e6e 6f74 6174 696f 6e3e 0d0a 2020 2020  nnotation>..    
-00000670: 2020 3c64 6f63 756d 656e 7461 7469 6f6e    <documentation
-00000680: 2078 6d6c 3a6c 616e 673d 2265 6e22 3e54   xml:lang="en">T
-00000690: 7261 6e73 666f 726d 6174 696f 6e73 2061  ransformations a
-000006a0: 7265 2066 756e 6374 696f 6e73 2061 7070  re functions app
-000006b0: 6c69 6361 626c 6520 6f6e 206f 6e65 206f  licable on one o
-000006c0: 7220 6d6f 7265 2046 4353 2064 696d 656e  r more FCS dimen
-000006d0: 7369 6f6e 733b 2074 6865 7920 7265 6365  sions; they rece
-000006e0: 6976 6520 616e 2069 6420 6174 7472 6962  ive an id attrib
-000006f0: 7574 6520 746f 2062 6520 7265 6665 7265  ute to be refere
-00000700: 6e63 6162 6c65 2066 726f 6d20 6761 7469  ncable from gati
-00000710: 6e67 2064 6573 6372 6970 7469 6f6e 732e  ng descriptions.
-00000720: 203c 2f64 6f63 756d 656e 7461 7469 6f6e   </documentation
-00000730: 3e0d 0a20 2020 203c 2f61 6e6e 6f74 6174  >..    </annotat
-00000740: 696f 6e3e 0d0a 2020 2020 3c73 6571 7565  ion>..    <seque
-00000750: 6e63 653e 0d0a 2020 2020 2020 3c21 2d2d  nce>..      <!--
-00000760: 3c67 726f 7570 2072 6566 3d22 6461 7461  <group ref="data
-00000770: 2d74 7970 653a 4375 7374 6f6d 5f47 726f  -type:Custom_Gro
-00000780: 7570 2220 6d69 6e4f 6363 7572 733d 2230  up" minOccurs="0
-00000790: 2220 2f3e 2d2d 3e0d 0a20 2020 2020 203c  " />-->..      <
-000007a0: 6368 6f69 6365 3e0d 0a20 2020 2020 2020  choice>..       
-000007b0: 203c 656c 656d 656e 7420 6e61 6d65 3d22   <element name="
-000007c0: 666c 696e 2220 7479 7065 3d22 7472 616e  flin" type="tran
-000007d0: 7366 6f72 6d73 3a46 4c69 6e54 7261 6e73  sforms:FLinTrans
-000007e0: 666f 726d 6174 696f 6e5f 5479 7065 2220  formation_Type" 
-000007f0: 6964 3d22 666c 696e 2220 2f3e 0d0a 2020  id="flin" />..  
-00000800: 2020 2020 2020 3c65 6c65 6d65 6e74 206e        <element n
-00000810: 616d 653d 2266 7261 7469 6f22 2074 7970  ame="fratio" typ
-00000820: 653d 2274 7261 6e73 666f 726d 733a 4652  e="transforms:FR
-00000830: 6174 696f 5472 616e 7366 6f72 6d61 7469  atioTransformati
-00000840: 6f6e 5f54 7970 6522 2069 643d 2266 7261  on_Type" id="fra
-00000850: 7469 6f22 202f 3e0d 0a20 2020 2020 2020  tio" />..       
-00000860: 203c 656c 656d 656e 7420 6e61 6d65 3d22   <element name="
-00000870: 666c 6f67 2220 7479 7065 3d22 7472 616e  flog" type="tran
-00000880: 7366 6f72 6d73 3a46 4c6f 6754 7261 6e73  sforms:FLogTrans
-00000890: 666f 726d 6174 696f 6e5f 5479 7065 2220  formation_Type" 
-000008a0: 6964 3d22 666c 6f67 2220 2f3e 0d0a 2020  id="flog" />..  
-000008b0: 2020 2020 2020 3c65 6c65 6d65 6e74 206e        <element n
-000008c0: 616d 653d 2266 6173 696e 6822 2074 7970  ame="fasinh" typ
-000008d0: 653d 2274 7261 6e73 666f 726d 733a 4641  e="transforms:FA
-000008e0: 5369 6e48 5472 616e 7366 6f72 6d61 7469  SinHTransformati
-000008f0: 6f6e 5f54 7970 6522 2069 643d 2261 7369  on_Type" id="asi
-00000900: 6e68 2220 2f3e 0d0a 2020 2020 2020 2020  nh" />..        
-00000910: 3c65 6c65 6d65 6e74 206e 616d 653d 2268  <element name="h
-00000920: 7970 6572 6c6f 6722 2074 7970 653d 2274  yperlog" type="t
-00000930: 7261 6e73 666f 726d 733a 4879 7065 726c  ransforms:Hyperl
-00000940: 6f67 5472 616e 7366 6f72 6d61 7469 6f6e  ogTransformation
-00000950: 5f54 7970 6522 2069 643d 2268 7970 6572  _Type" id="hyper
-00000960: 6c6f 6722 202f 3e0d 0a20 2020 2020 2020  log" />..       
-00000970: 203c 656c 656d 656e 7420 6e61 6d65 3d22   <element name="
-00000980: 6c6f 6769 636c 6522 2074 7970 653d 2274  logicle" type="t
-00000990: 7261 6e73 666f 726d 733a 4c6f 6769 636c  ransforms:Logicl
-000009a0: 6554 7261 6e73 666f 726d 6174 696f 6e5f  eTransformation_
-000009b0: 5479 7065 2220 6964 3d22 6c6f 6769 636c  Type" id="logicl
-000009c0: 6522 202f 3e0d 0a20 2020 2020 203c 2f63  e" />..      </c
-000009d0: 686f 6963 653e 0d0a 2020 2020 3c2f 7365  hoice>..    </se
-000009e0: 7175 656e 6365 3e0d 0a20 2020 203c 6174  quence>..    <at
-000009f0: 7472 6962 7574 6520 6e61 6d65 3d22 6964  tribute name="id
-00000a00: 2220 7479 7065 3d22 4944 2220 7573 653d  " type="ID" use=
-00000a10: 2272 6571 7569 7265 6422 202f 3e0d 0a20  "required" />.. 
-00000a20: 2020 203c 6174 7472 6962 7574 6520 6e61     <attribute na
-00000a30: 6d65 3d22 626f 756e 644d 696e 2220 7479  me="boundMin" ty
-00000a40: 7065 3d22 6461 7461 2d74 7970 653a 466c  pe="data-type:Fl
-00000a50: 6f61 7436 345f 5479 7065 2220 7573 653d  oat64_Type" use=
-00000a60: 226f 7074 696f 6e61 6c22 202f 3e0d 0a20  "optional" />.. 
-00000a70: 2020 203c 6174 7472 6962 7574 6520 6e61     <attribute na
-00000a80: 6d65 3d22 626f 756e 644d 6178 2220 7479  me="boundMax" ty
-00000a90: 7065 3d22 6461 7461 2d74 7970 653a 466c  pe="data-type:Fl
-00000aa0: 6f61 7436 345f 5479 7065 2220 7573 653d  oat64_Type" use=
-00000ab0: 226f 7074 696f 6e61 6c22 202f 3e0d 0a20  "optional" />.. 
-00000ac0: 2020 203c 616e 7941 7474 7269 6275 7465     <anyAttribute
-00000ad0: 2070 726f 6365 7373 436f 6e74 656e 7473   processContents
-00000ae0: 3d22 736b 6970 222f 3e0d 0a20 203c 2f63  ="skip"/>..  </c
-00000af0: 6f6d 706c 6578 5479 7065 3e0d 0a0d 0a20  omplexType>.... 
-00000b00: 203c 636f 6d70 6c65 7854 7970 6520 6e61   <complexType na
-00000b10: 6d65 3d22 4162 7374 7261 6374 5472 616e  me="AbstractTran
-00000b20: 7366 6f72 6d61 7469 6f6e 5f54 7970 6522  sformation_Type"
-00000b30: 2061 6273 7472 6163 743d 2274 7275 6522   abstract="true"
-00000b40: 3e0d 0a20 2020 203c 616e 6e6f 7461 7469  >..    <annotati
-00000b50: 6f6e 3e0d 0a20 2020 2020 203c 646f 6375  on>..      <docu
-00000b60: 6d65 6e74 6174 696f 6e20 786d 6c3a 6c61  mentation xml:la
-00000b70: 6e67 3d22 656e 223e 4162 7374 7261 6374  ng="en">Abstract
-00000b80: 2074 7970 6520 746f 2062 6520 7573 6564   type to be used
-00000b90: 2061 7320 6120 636f 6d6d 6f6e 2070 6172   as a common par
-00000ba0: 656e 7420 6f66 2061 6c6c 2074 7261 6e73  ent of all trans
-00000bb0: 666f 726d 6174 696f 6e73 2e3c 2f64 6f63  formations.</doc
-00000bc0: 756d 656e 7461 7469 6f6e 3e0d 0a20 2020  umentation>..   
-00000bd0: 203c 2f61 6e6e 6f74 6174 696f 6e3e 0d0a   </annotation>..
-00000be0: 2020 2020 3c67 726f 7570 2072 6566 3d22      <group ref="
-00000bf0: 6461 7461 2d74 7970 653a 4375 7374 6f6d  data-type:Custom
-00000c00: 5f47 726f 7570 2220 6d69 6e4f 6363 7572  _Group" minOccur
-00000c10: 733d 2230 2220 2f3e 0d0a 2020 2020 3c61  s="0" />..    <a
-00000c20: 6e79 4174 7472 6962 7574 6520 7072 6f63  nyAttribute proc
-00000c30: 6573 7343 6f6e 7465 6e74 733d 2273 6b69  essContents="ski
-00000c40: 7022 2f3e 0d0a 2020 3c2f 636f 6d70 6c65  p"/>..  </comple
-00000c50: 7854 7970 653e 0d0a 0d0a 2020 3c63 6f6d  xType>....  <com
-00000c60: 706c 6578 5479 7065 206e 616d 653d 2246  plexType name="F
-00000c70: 4c69 6e54 7261 6e73 666f 726d 6174 696f  LinTransformatio
-00000c80: 6e5f 5479 7065 223e 0d0a 2020 2020 3c63  n_Type">..    <c
-00000c90: 6f6d 706c 6578 436f 6e74 656e 743e 0d0a  omplexContent>..
-00000ca0: 2020 2020 2020 3c65 7874 656e 7369 6f6e        <extension
-00000cb0: 2062 6173 653d 2274 7261 6e73 666f 726d   base="transform
-00000cc0: 733a 4162 7374 7261 6374 5472 616e 7366  s:AbstractTransf
-00000cd0: 6f72 6d61 7469 6f6e 5f54 7970 6522 3e0d  ormation_Type">.
-00000ce0: 0a20 2020 2020 2020 203c 6174 7472 6962  .        <attrib
-00000cf0: 7574 6520 6e61 6d65 3d22 4122 2074 7970  ute name="A" typ
-00000d00: 653d 2264 6174 612d 7479 7065 3a46 6c6f  e="data-type:Flo
-00000d10: 6174 3634 5f54 7970 6522 2075 7365 3d22  at64_Type" use="
-00000d20: 7265 7175 6972 6564 2220 2f3e 0d0a 2020  required" />..  
-00000d30: 2020 2020 2020 3c61 7474 7269 6275 7465        <attribute
-00000d40: 206e 616d 653d 2254 2220 7479 7065 3d22   name="T" type="
-00000d50: 6461 7461 2d74 7970 653a 5046 6c6f 6174  data-type:PFloat
-00000d60: 3634 5f54 7970 6522 2075 7365 3d22 7265  64_Type" use="re
-00000d70: 7175 6972 6564 2220 2f3e 0d0a 2020 2020  quired" />..    
-00000d80: 2020 2020 3c21 2d2d 0d0a 2020 2020 2020      <!--..      
-00000d90: 2020 2020 5853 4431 2e31 2061 6c6c 6f77      XSD1.1 allow
-00000da0: 7320 7573 2074 6f20 706c 6163 6520 7468  s us to place th
-00000db0: 6520 666f 6c6c 6f77 696e 6720 6173 7365  e following asse
-00000dc0: 7274 696f 6e20 7374 6174 696e 6720 7468  rtion stating th
-00000dd0: 6174 2054 3e41 200d 0a20 2020 2020 2020  at T>A ..       
-00000de0: 2020 203c 6173 7365 7274 2074 6573 743d     <assert test=
-00000df0: 2240 5420 6774 6520 4041 2220 2f3e 0d0a  "@T gte @A" />..
-00000e00: 2020 2020 2020 2020 2020 486f 7765 7665            Howeve
-00000e10: 722c 2077 6520 6861 7665 2066 6f75 6e64  r, we have found
-00000e20: 2065 7870 6572 696d 656e 7461 6c6c 7920   experimentally 
-00000e30: 7468 6174 2074 6869 7320 7465 7374 2066  that this test f
-00000e40: 6169 6c73 2061 7420 7468 6520 584d 4c20  ails at the XML 
-00000e50: 696e 7374 616e 6365 206c 6576 656c 2065  instance level e
-00000e60: 7665 6e20 6576 656e 2069 6620 7468 6973  ven even if this
-00000e70: 2063 6f6e 6469 7469 6f6e 2069 7320 6d65   condition is me
-00000e80: 742e 0d0a 2020 2020 2020 2020 2020 4375  t...          Cu
-00000e90: 7265 6e74 6c79 2c20 7468 6520 6361 7573  rently, the caus
-00000ea0: 6520 6f66 2074 6869 7320 7072 6f62 6c65  e of this proble
-00000eb0: 6d20 6973 2075 6e63 6c65 6172 2c20 7768  m is unclear, wh
-00000ec0: 6963 6820 6c65 6164 2075 7320 746f 2063  ich lead us to c
-00000ed0: 6f6d 6d65 6e74 696e 6720 6f75 7420 7468  ommenting out th
-00000ee0: 6520 6173 7365 7469 6f6e 2061 6e64 206c  e assetion and l
-00000ef0: 6561 7669 6e67 2069 7420 7570 2074 6f20  eaving it up to 
-00000f00: 0d0a 2020 2020 2020 2020 2020 7468 6520  ..          the 
-00000f10: 696d 706c 656d 656e 7469 6e67 2073 6f66  implementing sof
-00000f20: 7477 6172 6520 746f 2076 6572 6966 7920  tware to verify 
-00000f30: 7468 6174 2061 7474 7269 6275 7465 2076  that attribute v
-00000f40: 616c 7565 7320 6172 6520 636f 7272 6563  alues are correc
-00000f50: 742e 0d0a 2020 2020 2020 2020 2d2d 3e0d  t...        -->.
-00000f60: 0a20 2020 2020 203c 2f65 7874 656e 7369  .      </extensi
-00000f70: 6f6e 3e0d 0a20 2020 203c 2f63 6f6d 706c  on>..    </compl
-00000f80: 6578 436f 6e74 656e 743e 0d0a 2020 3c2f  exContent>..  </
-00000f90: 636f 6d70 6c65 7854 7970 653e 0d0a 0d0a  complexType>....
-00000fa0: 2020 3c63 6f6d 706c 6578 5479 7065 206e    <complexType n
-00000fb0: 616d 653d 2246 5261 7469 6f54 7261 6e73  ame="FRatioTrans
+00000020: 462d 3822 3f3e 0a0a 3c73 6368 656d 6120  F-8"?>..<schema 
+00000030: 786d 6c6e 733d 2268 7474 703a 2f2f 7777  xmlns="http://ww
+00000040: 772e 7733 2e6f 7267 2f32 3030 312f 584d  w.w3.org/2001/XM
+00000050: 4c53 6368 656d 6122 0a20 2078 6d6c 6e73  LSchema".  xmlns
+00000060: 3a74 7261 6e73 666f 726d 733d 2268 7474  :transforms="htt
+00000070: 703a 2f2f 7777 772e 6973 6163 2d6e 6574  p://www.isac-net
+00000080: 2e6f 7267 2f73 7464 2f47 6174 696e 672d  .org/std/Gating-
+00000090: 4d4c 2f76 322e 302f 7472 616e 7366 6f72  ML/v2.0/transfor
+000000a0: 6d61 7469 6f6e 7322 0a20 2078 6d6c 6e73  mations".  xmlns
+000000b0: 3a64 6174 612d 7479 7065 3d22 6874 7470  :data-type="http
+000000c0: 3a2f 2f77 7777 2e69 7361 632d 6e65 742e  ://www.isac-net.
+000000d0: 6f72 672f 7374 642f 4761 7469 6e67 2d4d  org/std/Gating-M
+000000e0: 4c2f 7632 2e30 2f64 6174 6174 7970 6573  L/v2.0/datatypes
+000000f0: 220a 2020 786d 6c6e 733a 6d6d 6c3d 2268  ".  xmlns:mml="h
+00000100: 7474 703a 2f2f 7777 772e 7733 2e6f 7267  ttp://www.w3.org
+00000110: 2f31 3939 382f 4d61 7468 2f4d 6174 684d  /1998/Math/MathM
+00000120: 4c22 0a20 2074 6172 6765 744e 616d 6573  L".  targetNames
+00000130: 7061 6365 3d22 6874 7470 3a2f 2f77 7777  pace="http://www
+00000140: 2e69 7361 632d 6e65 742e 6f72 672f 7374  .isac-net.org/st
+00000150: 642f 4761 7469 6e67 2d4d 4c2f 7632 2e30  d/Gating-ML/v2.0
+00000160: 2f74 7261 6e73 666f 726d 6174 696f 6e73  /transformations
+00000170: 220a 2020 656c 656d 656e 7446 6f72 6d44  ".  elementFormD
+00000180: 6566 6175 6c74 3d22 7175 616c 6966 6965  efault="qualifie
+00000190: 6422 2061 7474 7269 6275 7465 466f 726d  d" attributeForm
+000001a0: 4465 6661 756c 743d 2271 7561 6c69 6669  Default="qualifi
+000001b0: 6564 2220 7665 7273 696f 6e3d 2232 2e30  ed" version="2.0
+000001c0: 2e31 3231 3230 3722 3e0a 0a20 203c 696d  .121207">..  <im
+000001d0: 706f 7274 206e 616d 6573 7061 6365 3d22  port namespace="
+000001e0: 6874 7470 3a2f 2f77 7777 2e69 7361 632d  http://www.isac-
+000001f0: 6e65 742e 6f72 672f 7374 642f 4761 7469  net.org/std/Gati
+00000200: 6e67 2d4d 4c2f 7632 2e30 2f64 6174 6174  ng-ML/v2.0/datat
+00000210: 7970 6573 220a 2020 2020 7363 6865 6d61  ypes".    schema
+00000220: 4c6f 6361 7469 6f6e 3d22 4461 7461 5479  Location="DataTy
+00000230: 7065 732e 7632 2e30 2e78 7364 2220 2f3e  pes.v2.0.xsd" />
+00000240: 0a0a 2020 3c61 6e6e 6f74 6174 696f 6e3e  ..  <annotation>
+00000250: 0a20 2020 203c 6170 7069 6e66 6f20 736f  .    <appinfo so
+00000260: 7572 6365 3d22 6874 7470 3a2f 2f66 6c6f  urce="http://flo
+00000270: 7763 7974 2e73 6f75 7263 6566 6f72 6765  wcyt.sourceforge
+00000280: 2e6e 6574 2f22 3e54 7261 6e73 666f 726d  .net/">Transform
+00000290: 6174 696f 6e20 6465 7363 7269 7074 696f  ation descriptio
+000002a0: 6e73 2077 6974 6869 6e20 4761 7469 6e67  ns within Gating
+000002b0: 2d4d 4c2e 3c2f 6170 7069 6e66 6f3e 0a0a  -ML.</appinfo>..
+000002c0: 2020 2020 3c64 6f63 756d 656e 7461 7469      <documentati
+000002d0: 6f6e 2078 6d6c 3a6c 616e 673d 2265 6e22  on xml:lang="en"
+000002e0: 2073 6f75 7263 653d 2268 7474 703a 2f2f   source="http://
+000002f0: 666c 6f77 6379 742e 736f 7572 6365 666f  flowcyt.sourcefo
+00000300: 7267 652e 6e65 742f 223e 0a20 2020 2020  rge.net/">.     
+00000310: 203c 6175 7468 6f72 3e0a 2020 2020 2020   <author>.      
+00000320: 2020 3c6e 616d 653e 4a6f 7365 6620 5370    <name>Josef Sp
+00000330: 6964 6c65 6e3c 2f6e 616d 653e 0a20 2020  idlen</name>.   
+00000340: 2020 2020 203c 656d 6169 6c3e 6a73 7069       <email>jspi
+00000350: 646c 656e 4062 6363 7263 2e63 613c 2f65  dlen@bccrc.ca</e
+00000360: 6d61 696c 3e0a 2020 2020 2020 3c2f 6175  mail>.      </au
+00000370: 7468 6f72 3e0a 2020 2020 2020 3c63 6f70  thor>.      <cop
+00000380: 7972 6967 6874 3e0a 2020 2020 2020 2020  yright>.        
+00000390: 436f 7079 7269 6768 7420 2863 2920 3230  Copyright (c) 20
+000003a0: 3038 2d32 3031 3420 4953 4143 2028 496e  08-2014 ISAC (In
+000003b0: 7465 726e 6174 696f 6e61 6c20 536f 6369  ternational Soci
+000003c0: 6574 7920 666f 7220 4164 7661 6e63 656d  ety for Advancem
+000003d0: 656e 7420 6f66 2043 7974 6f6d 6574 7279  ent of Cytometry
+000003e0: 290a 2020 2020 2020 2020 4672 6565 206f  ).        Free o
+000003f0: 6620 6368 6172 6765 2064 6973 7472 6962  f charge distrib
+00000400: 7574 696f 6e20 616e 6420 7265 6164 2d6f  ution and read-o
+00000410: 6e6c 7920 7573 6167 6520 7065 726d 6974  nly usage permit
+00000420: 6564 2e20 4d6f 6469 6669 6361 7469 6f6e  ed. Modification
+00000430: 2061 6e64 2061 6c6c 206f 7468 6572 2072   and all other r
+00000440: 6967 6874 730a 2020 2020 2020 2020 7265  ights.        re
+00000450: 7365 7276 6564 2e20 466f 7220 616c 6c20  served. For all 
+00000460: 6f74 6865 7220 7573 6573 2070 6c65 6173  other uses pleas
+00000470: 6520 636f 6e74 6163 7420 4953 4143 2e20  e contact ISAC. 
+00000480: 0a20 2020 2020 203c 2f63 6f70 7972 6967  .      </copyrig
+00000490: 6874 3e0a 2020 2020 3c2f 646f 6375 6d65  ht>.    </docume
+000004a0: 6e74 6174 696f 6e3e 0a20 203c 2f61 6e6e  ntation>.  </ann
+000004b0: 6f74 6174 696f 6e3e 0a0a 2020 3c67 726f  otation>..  <gro
+000004c0: 7570 206e 616d 653d 2254 7261 6e73 666f  up name="Transfo
+000004d0: 726d 6174 696f 6e5f 4772 6f75 7022 3e0a  rmation_Group">.
+000004e0: 2020 2020 3c63 686f 6963 653e 0a20 2020      <choice>.   
+000004f0: 2020 2020 203c 656c 656d 656e 7420 6e61       <element na
+00000500: 6d65 3d22 7472 616e 7366 6f72 6d61 7469  me="transformati
+00000510: 6f6e 2220 6964 3d22 7472 616e 7366 6f72  on" id="transfor
+00000520: 6d61 7469 6f6e 2220 7479 7065 3d22 7472  mation" type="tr
+00000530: 616e 7366 6f72 6d73 3a74 7261 6e73 666f  ansforms:transfo
+00000540: 726d 6174 696f 6e5f 5479 7065 2220 2f3e  rmation_Type" />
+00000550: 0a20 2020 203c 2f63 686f 6963 653e 0a20  .    </choice>. 
+00000560: 203c 2f67 726f 7570 3e0a 0a20 203c 6772   </group>..  <gr
+00000570: 6f75 7020 6e61 6d65 3d22 5370 6563 7472  oup name="Spectr
+00000580: 756d 4d61 7472 6978 5f47 726f 7570 223e  umMatrix_Group">
+00000590: 0a20 2020 203c 6368 6f69 6365 3e0a 2020  .    <choice>.  
+000005a0: 2020 2020 3c65 6c65 6d65 6e74 206e 616d      <element nam
+000005b0: 653d 2273 7065 6374 7275 6d4d 6174 7269  e="spectrumMatri
+000005c0: 7822 2074 7970 653d 2274 7261 6e73 666f  x" type="transfo
+000005d0: 726d 733a 5370 6563 7472 756d 4d61 7472  rms:SpectrumMatr
+000005e0: 6978 5f54 7970 6522 202f 3e0a 2020 2020  ix_Type" />.    
+000005f0: 3c2f 6368 6f69 6365 3e0a 2020 3c2f 6772  </choice>.  </gr
+00000600: 6f75 703e 0a0a 2020 3c63 6f6d 706c 6578  oup>..  <complex
+00000610: 5479 7065 206e 616d 653d 2274 7261 6e73  Type name="trans
+00000620: 666f 726d 6174 696f 6e5f 5479 7065 223e  formation_Type">
+00000630: 0a20 2020 203c 616e 6e6f 7461 7469 6f6e  .    <annotation
+00000640: 3e0a 2020 2020 2020 3c64 6f63 756d 656e  >.      <documen
+00000650: 7461 7469 6f6e 2078 6d6c 3a6c 616e 673d  tation xml:lang=
+00000660: 2265 6e22 3e54 7261 6e73 666f 726d 6174  "en">Transformat
+00000670: 696f 6e73 2061 7265 2066 756e 6374 696f  ions are functio
+00000680: 6e73 2061 7070 6c69 6361 626c 6520 6f6e  ns applicable on
+00000690: 206f 6e65 206f 7220 6d6f 7265 2046 4353   one or more FCS
+000006a0: 2064 696d 656e 7369 6f6e 733b 2074 6865   dimensions; the
+000006b0: 7920 7265 6365 6976 6520 616e 2069 6420  y receive an id 
+000006c0: 6174 7472 6962 7574 6520 746f 2062 6520  attribute to be 
+000006d0: 7265 6665 7265 6e63 6162 6c65 2066 726f  referencable fro
+000006e0: 6d20 6761 7469 6e67 2064 6573 6372 6970  m gating descrip
+000006f0: 7469 6f6e 732e 203c 2f64 6f63 756d 656e  tions. </documen
+00000700: 7461 7469 6f6e 3e0a 2020 2020 3c2f 616e  tation>.    </an
+00000710: 6e6f 7461 7469 6f6e 3e0a 2020 2020 3c73  notation>.    <s
+00000720: 6571 7565 6e63 653e 0a20 2020 2020 203c  equence>.      <
+00000730: 212d 2d3c 6772 6f75 7020 7265 663d 2264  !--<group ref="d
+00000740: 6174 612d 7479 7065 3a43 7573 746f 6d5f  ata-type:Custom_
+00000750: 4772 6f75 7022 206d 696e 4f63 6375 7273  Group" minOccurs
+00000760: 3d22 3022 202f 3e2d 2d3e 0a20 2020 2020  ="0" />-->.     
+00000770: 203c 6368 6f69 6365 3e0a 2020 2020 2020   <choice>.      
+00000780: 2020 3c65 6c65 6d65 6e74 206e 616d 653d    <element name=
+00000790: 2266 6c69 6e22 2074 7970 653d 2274 7261  "flin" type="tra
+000007a0: 6e73 666f 726d 733a 464c 696e 5472 616e  nsforms:FLinTran
+000007b0: 7366 6f72 6d61 7469 6f6e 5f54 7970 6522  sformation_Type"
+000007c0: 2069 643d 2266 6c69 6e22 202f 3e0a 2020   id="flin" />.  
+000007d0: 2020 2020 2020 3c65 6c65 6d65 6e74 206e        <element n
+000007e0: 616d 653d 2266 7261 7469 6f22 2074 7970  ame="fratio" typ
+000007f0: 653d 2274 7261 6e73 666f 726d 733a 4652  e="transforms:FR
+00000800: 6174 696f 5472 616e 7366 6f72 6d61 7469  atioTransformati
+00000810: 6f6e 5f54 7970 6522 2069 643d 2266 7261  on_Type" id="fra
+00000820: 7469 6f22 202f 3e0a 2020 2020 2020 2020  tio" />.        
+00000830: 3c65 6c65 6d65 6e74 206e 616d 653d 2266  <element name="f
+00000840: 6c6f 6722 2074 7970 653d 2274 7261 6e73  log" type="trans
+00000850: 666f 726d 733a 464c 6f67 5472 616e 7366  forms:FLogTransf
+00000860: 6f72 6d61 7469 6f6e 5f54 7970 6522 2069  ormation_Type" i
+00000870: 643d 2266 6c6f 6722 202f 3e0a 2020 2020  d="flog" />.    
+00000880: 2020 2020 3c65 6c65 6d65 6e74 206e 616d      <element nam
+00000890: 653d 2266 6173 696e 6822 2074 7970 653d  e="fasinh" type=
+000008a0: 2274 7261 6e73 666f 726d 733a 4641 5369  "transforms:FASi
+000008b0: 6e48 5472 616e 7366 6f72 6d61 7469 6f6e  nHTransformation
+000008c0: 5f54 7970 6522 2069 643d 2261 7369 6e68  _Type" id="asinh
+000008d0: 2220 2f3e 0a20 2020 2020 2020 203c 656c  " />.        <el
+000008e0: 656d 656e 7420 6e61 6d65 3d22 6879 7065  ement name="hype
+000008f0: 726c 6f67 2220 7479 7065 3d22 7472 616e  rlog" type="tran
+00000900: 7366 6f72 6d73 3a48 7970 6572 6c6f 6754  sforms:HyperlogT
+00000910: 7261 6e73 666f 726d 6174 696f 6e5f 5479  ransformation_Ty
+00000920: 7065 2220 6964 3d22 6879 7065 726c 6f67  pe" id="hyperlog
+00000930: 2220 2f3e 0a20 2020 2020 2020 203c 656c  " />.        <el
+00000940: 656d 656e 7420 6e61 6d65 3d22 6c6f 6769  ement name="logi
+00000950: 636c 6522 2074 7970 653d 2274 7261 6e73  cle" type="trans
+00000960: 666f 726d 733a 4c6f 6769 636c 6554 7261  forms:LogicleTra
+00000970: 6e73 666f 726d 6174 696f 6e5f 5479 7065  nsformation_Type
+00000980: 2220 6964 3d22 6c6f 6769 636c 6522 202f  " id="logicle" /
+00000990: 3e0a 2020 2020 2020 3c2f 6368 6f69 6365  >.      </choice
+000009a0: 3e0a 2020 2020 3c2f 7365 7175 656e 6365  >.    </sequence
+000009b0: 3e0a 2020 2020 3c61 7474 7269 6275 7465  >.    <attribute
+000009c0: 206e 616d 653d 2269 6422 2074 7970 653d   name="id" type=
+000009d0: 2249 4422 2075 7365 3d22 7265 7175 6972  "ID" use="requir
+000009e0: 6564 2220 2f3e 0a20 2020 203c 6174 7472  ed" />.    <attr
+000009f0: 6962 7574 6520 6e61 6d65 3d22 626f 756e  ibute name="boun
+00000a00: 644d 696e 2220 7479 7065 3d22 6461 7461  dMin" type="data
+00000a10: 2d74 7970 653a 466c 6f61 7436 345f 5479  -type:Float64_Ty
+00000a20: 7065 2220 7573 653d 226f 7074 696f 6e61  pe" use="optiona
+00000a30: 6c22 202f 3e0a 2020 2020 3c61 7474 7269  l" />.    <attri
+00000a40: 6275 7465 206e 616d 653d 2262 6f75 6e64  bute name="bound
+00000a50: 4d61 7822 2074 7970 653d 2264 6174 612d  Max" type="data-
+00000a60: 7479 7065 3a46 6c6f 6174 3634 5f54 7970  type:Float64_Typ
+00000a70: 6522 2075 7365 3d22 6f70 7469 6f6e 616c  e" use="optional
+00000a80: 2220 2f3e 0a20 2020 203c 616e 7941 7474  " />.    <anyAtt
+00000a90: 7269 6275 7465 2070 726f 6365 7373 436f  ribute processCo
+00000aa0: 6e74 656e 7473 3d22 736b 6970 222f 3e0a  ntents="skip"/>.
+00000ab0: 2020 3c2f 636f 6d70 6c65 7854 7970 653e    </complexType>
+00000ac0: 0a0a 2020 3c63 6f6d 706c 6578 5479 7065  ..  <complexType
+00000ad0: 206e 616d 653d 2241 6273 7472 6163 7454   name="AbstractT
+00000ae0: 7261 6e73 666f 726d 6174 696f 6e5f 5479  ransformation_Ty
+00000af0: 7065 2220 6162 7374 7261 6374 3d22 7472  pe" abstract="tr
+00000b00: 7565 223e 0a20 2020 203c 616e 6e6f 7461  ue">.    <annota
+00000b10: 7469 6f6e 3e0a 2020 2020 2020 3c64 6f63  tion>.      <doc
+00000b20: 756d 656e 7461 7469 6f6e 2078 6d6c 3a6c  umentation xml:l
+00000b30: 616e 673d 2265 6e22 3e41 6273 7472 6163  ang="en">Abstrac
+00000b40: 7420 7479 7065 2074 6f20 6265 2075 7365  t type to be use
+00000b50: 6420 6173 2061 2063 6f6d 6d6f 6e20 7061  d as a common pa
+00000b60: 7265 6e74 206f 6620 616c 6c20 7472 616e  rent of all tran
+00000b70: 7366 6f72 6d61 7469 6f6e 732e 3c2f 646f  sformations.</do
+00000b80: 6375 6d65 6e74 6174 696f 6e3e 0a20 2020  cumentation>.   
+00000b90: 203c 2f61 6e6e 6f74 6174 696f 6e3e 0a20   </annotation>. 
+00000ba0: 2020 203c 6772 6f75 7020 7265 663d 2264     <group ref="d
+00000bb0: 6174 612d 7479 7065 3a43 7573 746f 6d5f  ata-type:Custom_
+00000bc0: 4772 6f75 7022 206d 696e 4f63 6375 7273  Group" minOccurs
+00000bd0: 3d22 3022 202f 3e0a 2020 2020 3c61 6e79  ="0" />.    <any
+00000be0: 4174 7472 6962 7574 6520 7072 6f63 6573  Attribute proces
+00000bf0: 7343 6f6e 7465 6e74 733d 2273 6b69 7022  sContents="skip"
+00000c00: 2f3e 0a20 203c 2f63 6f6d 706c 6578 5479  />.  </complexTy
+00000c10: 7065 3e0a 0a20 203c 636f 6d70 6c65 7854  pe>..  <complexT
+00000c20: 7970 6520 6e61 6d65 3d22 464c 696e 5472  ype name="FLinTr
+00000c30: 616e 7366 6f72 6d61 7469 6f6e 5f54 7970  ansformation_Typ
+00000c40: 6522 3e0a 2020 2020 3c63 6f6d 706c 6578  e">.    <complex
+00000c50: 436f 6e74 656e 743e 0a20 2020 2020 203c  Content>.      <
+00000c60: 6578 7465 6e73 696f 6e20 6261 7365 3d22  extension base="
+00000c70: 7472 616e 7366 6f72 6d73 3a41 6273 7472  transforms:Abstr
+00000c80: 6163 7454 7261 6e73 666f 726d 6174 696f  actTransformatio
+00000c90: 6e5f 5479 7065 223e 0a20 2020 2020 2020  n_Type">.       
+00000ca0: 203c 6174 7472 6962 7574 6520 6e61 6d65   <attribute name
+00000cb0: 3d22 4122 2074 7970 653d 2264 6174 612d  ="A" type="data-
+00000cc0: 7479 7065 3a46 6c6f 6174 3634 5f54 7970  type:Float64_Typ
+00000cd0: 6522 2075 7365 3d22 7265 7175 6972 6564  e" use="required
+00000ce0: 2220 2f3e 0a20 2020 2020 2020 203c 6174  " />.        <at
+00000cf0: 7472 6962 7574 6520 6e61 6d65 3d22 5422  tribute name="T"
+00000d00: 2074 7970 653d 2264 6174 612d 7479 7065   type="data-type
+00000d10: 3a50 466c 6f61 7436 345f 5479 7065 2220  :PFloat64_Type" 
+00000d20: 7573 653d 2272 6571 7569 7265 6422 202f  use="required" /
+00000d30: 3e0a 2020 2020 2020 2020 3c21 2d2d 0a20  >.        <!--. 
+00000d40: 2020 2020 2020 2020 2058 5344 312e 3120           XSD1.1 
+00000d50: 616c 6c6f 7773 2075 7320 746f 2070 6c61  allows us to pla
+00000d60: 6365 2074 6865 2066 6f6c 6c6f 7769 6e67  ce the following
+00000d70: 2061 7373 6572 7469 6f6e 2073 7461 7469   assertion stati
+00000d80: 6e67 2074 6861 7420 543e 4120 0a20 2020  ng that T>A .   
+00000d90: 2020 2020 2020 203c 6173 7365 7274 2074         <assert t
+00000da0: 6573 743d 2240 5420 6774 6520 4041 2220  est="@T gte @A" 
+00000db0: 2f3e 0a20 2020 2020 2020 2020 2048 6f77  />.          How
+00000dc0: 6576 6572 2c20 7765 2068 6176 6520 666f  ever, we have fo
+00000dd0: 756e 6420 6578 7065 7269 6d65 6e74 616c  und experimental
+00000de0: 6c79 2074 6861 7420 7468 6973 2074 6573  ly that this tes
+00000df0: 7420 6661 696c 7320 6174 2074 6865 2058  t fails at the X
+00000e00: 4d4c 2069 6e73 7461 6e63 6520 6c65 7665  ML instance leve
+00000e10: 6c20 6576 656e 2065 7665 6e20 6966 2074  l even even if t
+00000e20: 6869 7320 636f 6e64 6974 696f 6e20 6973  his condition is
+00000e30: 206d 6574 2e0a 2020 2020 2020 2020 2020   met..          
+00000e40: 4375 7265 6e74 6c79 2c20 7468 6520 6361  Curently, the ca
+00000e50: 7573 6520 6f66 2074 6869 7320 7072 6f62  use of this prob
+00000e60: 6c65 6d20 6973 2075 6e63 6c65 6172 2c20  lem is unclear, 
+00000e70: 7768 6963 6820 6c65 6164 2075 7320 746f  which lead us to
+00000e80: 2063 6f6d 6d65 6e74 696e 6720 6f75 7420   commenting out 
+00000e90: 7468 6520 6173 7365 7469 6f6e 2061 6e64  the assetion and
+00000ea0: 206c 6561 7669 6e67 2069 7420 7570 2074   leaving it up t
+00000eb0: 6f20 0a20 2020 2020 2020 2020 2074 6865  o .          the
+00000ec0: 2069 6d70 6c65 6d65 6e74 696e 6720 736f   implementing so
+00000ed0: 6674 7761 7265 2074 6f20 7665 7269 6679  ftware to verify
+00000ee0: 2074 6861 7420 6174 7472 6962 7574 6520   that attribute 
+00000ef0: 7661 6c75 6573 2061 7265 2063 6f72 7265  values are corre
+00000f00: 6374 2e0a 2020 2020 2020 2020 2d2d 3e0a  ct..        -->.
+00000f10: 2020 2020 2020 3c2f 6578 7465 6e73 696f        </extensio
+00000f20: 6e3e 0a20 2020 203c 2f63 6f6d 706c 6578  n>.    </complex
+00000f30: 436f 6e74 656e 743e 0a20 203c 2f63 6f6d  Content>.  </com
+00000f40: 706c 6578 5479 7065 3e0a 0a20 203c 636f  plexType>..  <co
+00000f50: 6d70 6c65 7854 7970 6520 6e61 6d65 3d22  mplexType name="
+00000f60: 4652 6174 696f 5472 616e 7366 6f72 6d61  FRatioTransforma
+00000f70: 7469 6f6e 5f54 7970 6522 3e0a 2020 2020  tion_Type">.    
+00000f80: 3c63 6f6d 706c 6578 436f 6e74 656e 743e  <complexContent>
+00000f90: 0a20 2020 2020 203c 6578 7465 6e73 696f  .      <extensio
+00000fa0: 6e20 6261 7365 3d22 7472 616e 7366 6f72  n base="transfor
+00000fb0: 6d73 3a41 6273 7472 6163 7454 7261 6e73  ms:AbstractTrans
 00000fc0: 666f 726d 6174 696f 6e5f 5479 7065 223e  formation_Type">
-00000fd0: 0d0a 2020 2020 3c63 6f6d 706c 6578 436f  ..    <complexCo
-00000fe0: 6e74 656e 743e 0d0a 2020 2020 2020 3c65  ntent>..      <e
-00000ff0: 7874 656e 7369 6f6e 2062 6173 653d 2274  xtension base="t
-00001000: 7261 6e73 666f 726d 733a 4162 7374 7261  ransforms:Abstra
-00001010: 6374 5472 616e 7366 6f72 6d61 7469 6f6e  ctTransformation
-00001020: 5f54 7970 6522 3e0d 0a20 2020 2020 2020  _Type">..       
-00001030: 203c 6772 6f75 7020 7265 663d 2264 6174   <group ref="dat
-00001040: 612d 7479 7065 3a46 4353 4469 6d65 6e73  a-type:FCSDimens
-00001050: 696f 6e73 5f47 726f 7570 2220 6d69 6e4f  ions_Group" minO
-00001060: 6363 7572 733d 2232 2220 6d61 784f 6363  ccurs="2" maxOcc
-00001070: 7572 733d 2232 2220 2f3e 0d0a 2020 2020  urs="2" />..    
-00001080: 2020 2020 3c61 7474 7269 6275 7465 206e      <attribute n
-00001090: 616d 653d 2241 2220 7479 7065 3d22 6461  ame="A" type="da
-000010a0: 7461 2d74 7970 653a 466c 6f61 7436 345f  ta-type:Float64_
-000010b0: 5479 7065 2220 7573 653d 2272 6571 7569  Type" use="requi
-000010c0: 7265 6422 202f 3e0d 0a20 2020 2020 2020  red" />..       
-000010d0: 203c 6174 7472 6962 7574 6520 6e61 6d65   <attribute name
-000010e0: 3d22 4222 2074 7970 653d 2264 6174 612d  ="B" type="data-
-000010f0: 7479 7065 3a46 6c6f 6174 3634 5f54 7970  type:Float64_Typ
-00001100: 6522 2075 7365 3d22 7265 7175 6972 6564  e" use="required
-00001110: 2220 2f3e 0d0a 2020 2020 2020 2020 3c61  " />..        <a
-00001120: 7474 7269 6275 7465 206e 616d 653d 2243  ttribute name="C
-00001130: 2220 7479 7065 3d22 6461 7461 2d74 7970  " type="data-typ
-00001140: 653a 466c 6f61 7436 345f 5479 7065 2220  e:Float64_Type" 
-00001150: 7573 653d 2272 6571 7569 7265 6422 202f  use="required" /
-00001160: 3e0d 0a20 2020 2020 203c 2f65 7874 656e  >..      </exten
-00001170: 7369 6f6e 3e0d 0a20 2020 203c 2f63 6f6d  sion>..    </com
-00001180: 706c 6578 436f 6e74 656e 743e 0d0a 2020  plexContent>..  
-00001190: 3c2f 636f 6d70 6c65 7854 7970 653e 0d0a  </complexType>..
-000011a0: 0d0a 2020 3c63 6f6d 706c 6578 5479 7065  ..  <complexType
-000011b0: 206e 616d 653d 2246 4c6f 6754 7261 6e73   name="FLogTrans
-000011c0: 666f 726d 6174 696f 6e5f 5479 7065 223e  formation_Type">
-000011d0: 0d0a 2020 2020 3c63 6f6d 706c 6578 436f  ..    <complexCo
-000011e0: 6e74 656e 743e 0d0a 2020 2020 2020 3c65  ntent>..      <e
-000011f0: 7874 656e 7369 6f6e 2062 6173 653d 2274  xtension base="t
-00001200: 7261 6e73 666f 726d 733a 4162 7374 7261  ransforms:Abstra
-00001210: 6374 5472 616e 7366 6f72 6d61 7469 6f6e  ctTransformation
-00001220: 5f54 7970 6522 3e0d 0a20 2020 2020 2020  _Type">..       
-00001230: 203c 6174 7472 6962 7574 6520 6e61 6d65   <attribute name
-00001240: 3d22 5422 2074 7970 653d 2264 6174 612d  ="T" type="data-
-00001250: 7479 7065 3a50 466c 6f61 7436 345f 5479  type:PFloat64_Ty
-00001260: 7065 2220 7573 653d 2272 6571 7569 7265  pe" use="require
-00001270: 6422 202f 3e0d 0a20 2020 2020 2020 203c  d" />..        <
-00001280: 6174 7472 6962 7574 6520 6e61 6d65 3d22  attribute name="
-00001290: 4d22 2074 7970 653d 2264 6174 612d 7479  M" type="data-ty
-000012a0: 7065 3a50 466c 6f61 7436 345f 5479 7065  pe:PFloat64_Type
-000012b0: 2220 7573 653d 2272 6571 7569 7265 6422  " use="required"
-000012c0: 202f 3e0d 0a20 2020 2020 203c 2f65 7874   />..      </ext
-000012d0: 656e 7369 6f6e 3e0d 0a20 2020 203c 2f63  ension>..    </c
-000012e0: 6f6d 706c 6578 436f 6e74 656e 743e 0d0a  omplexContent>..
-000012f0: 2020 3c2f 636f 6d70 6c65 7854 7970 653e    </complexType>
-00001300: 0d0a 0d0a 2020 3c63 6f6d 706c 6578 5479  ....  <complexTy
-00001310: 7065 206e 616d 653d 2246 4153 696e 4854  pe name="FASinHT
-00001320: 7261 6e73 666f 726d 6174 696f 6e5f 5479  ransformation_Ty
-00001330: 7065 223e 0d0a 2020 2020 3c63 6f6d 706c  pe">..    <compl
-00001340: 6578 436f 6e74 656e 743e 0d0a 2020 2020  exContent>..    
-00001350: 2020 3c65 7874 656e 7369 6f6e 2062 6173    <extension bas
-00001360: 653d 2274 7261 6e73 666f 726d 733a 4162  e="transforms:Ab
-00001370: 7374 7261 6374 5472 616e 7366 6f72 6d61  stractTransforma
-00001380: 7469 6f6e 5f54 7970 6522 3e0d 0a20 2020  tion_Type">..   
-00001390: 2020 2020 203c 6174 7472 6962 7574 6520       <attribute 
-000013a0: 6e61 6d65 3d22 5422 2074 7970 653d 2264  name="T" type="d
-000013b0: 6174 612d 7479 7065 3a50 466c 6f61 7436  ata-type:PFloat6
-000013c0: 345f 5479 7065 2220 7573 653d 2272 6571  4_Type" use="req
-000013d0: 7569 7265 6422 202f 3e0d 0a20 2020 2020  uired" />..     
-000013e0: 2020 203c 6174 7472 6962 7574 6520 6e61     <attribute na
-000013f0: 6d65 3d22 4d22 2074 7970 653d 2264 6174  me="M" type="dat
-00001400: 612d 7479 7065 3a50 466c 6f61 7436 345f  a-type:PFloat64_
-00001410: 5479 7065 2220 7573 653d 2272 6571 7569  Type" use="requi
-00001420: 7265 6422 202f 3e0d 0a20 2020 2020 2020  red" />..       
-00001430: 203c 6174 7472 6962 7574 6520 6e61 6d65   <attribute name
-00001440: 3d22 4122 2074 7970 653d 2264 6174 612d  ="A" type="data-
-00001450: 7479 7065 3a55 466c 6f61 7436 345f 5479  type:UFloat64_Ty
-00001460: 7065 2220 7573 653d 2272 6571 7569 7265  pe" use="require
-00001470: 6422 202f 3e0d 0a20 2020 2020 203c 2f65  d" />..      </e
-00001480: 7874 656e 7369 6f6e 3e0d 0a20 2020 2020  xtension>..     
-00001490: 203c 212d 2d0d 0a20 2020 2020 2020 2058   <!--..        X
-000014a0: 5344 312e 3120 616c 6c6f 7773 2075 7320  SD1.1 allows us 
-000014b0: 746f 2070 6c61 6365 2074 6865 2066 6f6c  to place the fol
-000014c0: 6c6f 7769 6e67 2061 7373 6572 7469 6f6e  lowing assertion
-000014d0: 2073 7461 7469 6e67 2074 6861 7420 543e   stating that T>
-000014e0: 4120 0d0a 2020 2020 2020 2020 3c61 7373  A ..        <ass
-000014f0: 6572 7420 7465 7374 3d22 404d 2067 7465  ert test="@M gte
-00001500: 2040 4122 202f 3e0d 0a20 2020 2020 2020   @A" />..       
-00001510: 2048 6f77 6576 6572 2c20 7765 2068 6176   However, we hav
-00001520: 6520 666f 756e 6420 6578 7065 7269 6d65  e found experime
-00001530: 6e74 616c 6c79 2074 6861 7420 7468 6973  ntally that this
-00001540: 2074 6573 7420 6661 696c 7320 6174 2074   test fails at t
-00001550: 6865 2058 4d4c 2069 6e73 7461 6e63 6520  he XML instance 
-00001560: 6c65 7665 6c20 6576 656e 2065 7665 6e20  level even even 
-00001570: 6966 2074 6869 7320 636f 6e64 6974 696f  if this conditio
-00001580: 6e20 6973 206d 6574 2e0d 0a20 2020 2020  n is met...     
-00001590: 2020 2043 7572 656e 746c 792c 2074 6865     Curently, the
-000015a0: 2063 6175 7365 206f 6620 7468 6973 2070   cause of this p
-000015b0: 726f 626c 656d 2069 7320 756e 636c 6561  roblem is unclea
-000015c0: 722c 2077 6869 6368 206c 6561 6420 7573  r, which lead us
-000015d0: 2074 6f20 636f 6d6d 656e 7469 6e67 206f   to commenting o
-000015e0: 7574 2074 6865 2061 7373 6574 696f 6e20  ut the assetion 
-000015f0: 616e 6420 6c65 6176 696e 6720 6974 2075  and leaving it u
-00001600: 7020 746f 200d 0a20 2020 2020 2020 2074  p to ..        t
-00001610: 6865 2069 6d70 6c65 6d65 6e74 696e 6720  he implementing 
-00001620: 736f 6674 7761 7265 2074 6f20 7665 7269  software to veri
-00001630: 6679 2074 6861 7420 6174 7472 6962 7574  fy that attribut
-00001640: 6520 7661 6c75 6573 2061 7265 2063 6f72  e values are cor
-00001650: 7265 6374 2e0d 0a20 2020 2020 202d 2d3e  rect...      -->
-00001660: 0d0a 2020 2020 3c2f 636f 6d70 6c65 7843  ..    </complexC
-00001670: 6f6e 7465 6e74 3e0d 0a20 203c 2f63 6f6d  ontent>..  </com
-00001680: 706c 6578 5479 7065 3e0d 0a0d 0a20 203c  plexType>....  <
-00001690: 636f 6d70 6c65 7854 7970 6520 6e61 6d65  complexType name
-000016a0: 3d22 4879 7065 726c 6f67 5472 616e 7366  ="HyperlogTransf
-000016b0: 6f72 6d61 7469 6f6e 5f54 7970 6522 3e0d  ormation_Type">.
-000016c0: 0a20 2020 203c 636f 6d70 6c65 7843 6f6e  .    <complexCon
-000016d0: 7465 6e74 3e0d 0a20 2020 2020 203c 6578  tent>..      <ex
-000016e0: 7465 6e73 696f 6e20 6261 7365 3d22 7472  tension base="tr
-000016f0: 616e 7366 6f72 6d73 3a41 6273 7472 6163  ansforms:Abstrac
-00001700: 7454 7261 6e73 666f 726d 6174 696f 6e5f  tTransformation_
-00001710: 5479 7065 223e 0d0a 2020 2020 2020 2020  Type">..        
-00001720: 3c61 7474 7269 6275 7465 206e 616d 653d  <attribute name=
-00001730: 2254 2220 7479 7065 3d22 6461 7461 2d74  "T" type="data-t
-00001740: 7970 653a 5046 6c6f 6174 3634 5f54 7970  ype:PFloat64_Typ
-00001750: 6522 2075 7365 3d22 7265 7175 6972 6564  e" use="required
-00001760: 2220 2f3e 0d0a 2020 2020 2020 2020 3c61  " />..        <a
-00001770: 7474 7269 6275 7465 206e 616d 653d 224d  ttribute name="M
-00001780: 2220 7479 7065 3d22 6461 7461 2d74 7970  " type="data-typ
-00001790: 653a 5046 6c6f 6174 3634 5f54 7970 6522  e:PFloat64_Type"
-000017a0: 2075 7365 3d22 7265 7175 6972 6564 2220   use="required" 
-000017b0: 2f3e 0d0a 2020 2020 2020 2020 3c61 7474  />..        <att
-000017c0: 7269 6275 7465 206e 616d 653d 2257 2220  ribute name="W" 
-000017d0: 7479 7065 3d22 6461 7461 2d74 7970 653a  type="data-type:
-000017e0: 5046 6c6f 6174 3634 5f54 7970 6522 2075  PFloat64_Type" u
-000017f0: 7365 3d22 7265 7175 6972 6564 2220 2f3e  se="required" />
-00001800: 0d0a 2020 2020 2020 2020 3c61 7474 7269  ..        <attri
-00001810: 6275 7465 206e 616d 653d 2241 2220 7479  bute name="A" ty
-00001820: 7065 3d22 6461 7461 2d74 7970 653a 466c  pe="data-type:Fl
-00001830: 6f61 7436 345f 5479 7065 2220 7573 653d  oat64_Type" use=
-00001840: 2272 6571 7569 7265 6422 202f 3e0d 0a20  "required" />.. 
-00001850: 2020 2020 2020 203c 212d 2d0d 0a20 2020         <!--..   
-00001860: 2020 2020 2020 2058 5344 312e 3120 616c         XSD1.1 al
-00001870: 6c6f 7773 2075 7320 746f 2070 6c61 6365  lows us to place
-00001880: 2074 6865 2066 6f6c 6c6f 7769 6e67 2061   the following a
-00001890: 7373 6572 7469 6f6e 7320 7374 6174 696e  ssertions statin
-000018a0: 6720 7468 6174 2057 203e 3d20 4d2f 322c  g that W >= M/2,
-000018b0: 202d 5720 3c3d 2041 203c 3d20 4d2d 3257   -W <= A <= M-2W
-000018c0: 200d 0a20 2020 2020 2020 2020 203c 6173   ..          <as
-000018d0: 7365 7274 2074 6573 743d 2240 5720 6c65  sert test="@W le
-000018e0: 2028 2840 4d29 2064 6976 2032 2922 202f   ((@M) div 2)" /
-000018f0: 3e0d 0a20 2020 2020 2020 2020 203c 6173  >..          <as
-00001900: 7365 7274 2074 6573 743d 2240 4120 6765  sert test="@A ge
-00001910: 2028 282d 3129 2a28 4057 2929 2220 2f3e   ((-1)*(@W))" />
-00001920: 0d0a 2020 2020 2020 2020 2020 3c61 7373  ..          <ass
-00001930: 6572 7420 7465 7374 3d22 4041 206c 6520  ert test="@A le 
-00001940: 2840 4d29 2d28 322a 4057 2922 2f3e 0d0a  (@M)-(2*@W)"/>..
-00001950: 2020 2020 2020 2020 2020 486f 7765 7665            Howeve
-00001960: 722c 2077 6520 6861 7665 2066 6f75 6e64  r, we have found
-00001970: 2065 7870 6572 696d 656e 7461 6c6c 7920   experimentally 
-00001980: 7468 6174 2074 6865 7365 2074 6573 7473  that these tests
-00001990: 2066 6169 6c73 2061 7420 7468 6520 584d   fails at the XM
-000019a0: 4c20 696e 7374 616e 6365 206c 6576 656c  L instance level
-000019b0: 2065 7665 6e20 6576 656e 2069 6620 7468   even even if th
-000019c0: 6573 6520 636f 6e64 6974 696f 6e73 2061  ese conditions a
-000019d0: 7265 206d 6574 2e0d 0a20 2020 2020 2020  re met...       
-000019e0: 2020 2043 7572 656e 746c 792c 2074 6865     Curently, the
-000019f0: 2063 6175 7365 206f 6620 7468 6973 2070   cause of this p
-00001a00: 726f 626c 656d 2069 7320 756e 636c 6561  roblem is unclea
-00001a10: 722c 2077 6869 6368 206c 6561 6420 7573  r, which lead us
-00001a20: 2074 6f20 636f 6d6d 656e 7469 6e67 206f   to commenting o
-00001a30: 7574 2074 6865 2061 7373 6574 696f 6e20  ut the assetion 
-00001a40: 616e 6420 6c65 6176 696e 6720 6974 2075  and leaving it u
-00001a50: 7020 746f 200d 0a20 2020 2020 2020 2020  p to ..         
-00001a60: 2074 6865 2069 6d70 6c65 6d65 6e74 696e   the implementin
-00001a70: 6720 736f 6674 7761 7265 2074 6f20 7665  g software to ve
-00001a80: 7269 6679 2074 6861 7420 6174 7472 6962  rify that attrib
-00001a90: 7574 6520 7661 6c75 6573 2061 7265 2063  ute values are c
-00001aa0: 6f72 7265 6374 2e0d 0a20 2020 2020 2020  orrect...       
-00001ab0: 202d 2d3e 0d0a 2020 2020 2020 3c2f 6578   -->..      </ex
-00001ac0: 7465 6e73 696f 6e3e 0d0a 2020 2020 3c2f  tension>..    </
-00001ad0: 636f 6d70 6c65 7843 6f6e 7465 6e74 3e0d  complexContent>.
-00001ae0: 0a20 203c 2f63 6f6d 706c 6578 5479 7065  .  </complexType
-00001af0: 3e0d 0a0d 0a20 203c 636f 6d70 6c65 7854  >....  <complexT
-00001b00: 7970 6520 6e61 6d65 3d22 4c6f 6769 636c  ype name="Logicl
-00001b10: 6554 7261 6e73 666f 726d 6174 696f 6e5f  eTransformation_
-00001b20: 5479 7065 223e 0d0a 2020 2020 3c63 6f6d  Type">..    <com
-00001b30: 706c 6578 436f 6e74 656e 743e 0d0a 2020  plexContent>..  
-00001b40: 2020 2020 3c65 7874 656e 7369 6f6e 2062      <extension b
-00001b50: 6173 653d 2274 7261 6e73 666f 726d 733a  ase="transforms:
-00001b60: 4162 7374 7261 6374 5472 616e 7366 6f72  AbstractTransfor
-00001b70: 6d61 7469 6f6e 5f54 7970 6522 3e0d 0a20  mation_Type">.. 
-00001b80: 2020 2020 2020 203c 6174 7472 6962 7574         <attribut
-00001b90: 6520 6e61 6d65 3d22 5422 2074 7970 653d  e name="T" type=
-00001ba0: 2264 6174 612d 7479 7065 3a50 466c 6f61  "data-type:PFloa
-00001bb0: 7436 345f 5479 7065 2220 7573 653d 2272  t64_Type" use="r
-00001bc0: 6571 7569 7265 6422 202f 3e0d 0a20 2020  equired" />..   
-00001bd0: 2020 2020 203c 6174 7472 6962 7574 6520       <attribute 
-00001be0: 6e61 6d65 3d22 4d22 2074 7970 653d 2264  name="M" type="d
-00001bf0: 6174 612d 7479 7065 3a50 466c 6f61 7436  ata-type:PFloat6
-00001c00: 345f 5479 7065 2220 7573 653d 2272 6571  4_Type" use="req
-00001c10: 7569 7265 6422 202f 3e0d 0a20 2020 2020  uired" />..     
-00001c20: 2020 203c 6174 7472 6962 7574 6520 6e61     <attribute na
-00001c30: 6d65 3d22 5722 2074 7970 653d 2264 6174  me="W" type="dat
-00001c40: 612d 7479 7065 3a55 466c 6f61 7436 345f  a-type:UFloat64_
-00001c50: 5479 7065 2220 7573 653d 2272 6571 7569  Type" use="requi
-00001c60: 7265 6422 202f 3e0d 0a20 2020 2020 2020  red" />..       
-00001c70: 203c 6174 7472 6962 7574 6520 6e61 6d65   <attribute name
-00001c80: 3d22 4122 2074 7970 653d 2264 6174 612d  ="A" type="data-
-00001c90: 7479 7065 3a46 6c6f 6174 3634 5f54 7970  type:Float64_Typ
-00001ca0: 6522 2075 7365 3d22 7265 7175 6972 6564  e" use="required
-00001cb0: 2220 2f3e 0d0a 2020 2020 2020 2020 3c21  " />..        <!
-00001cc0: 2d2d 0d0a 2020 2020 2020 2020 2020 5853  --..          XS
-00001cd0: 4431 2e31 2061 6c6c 6f77 7320 7573 2074  D1.1 allows us t
-00001ce0: 6f20 706c 6163 6520 7468 6520 666f 6c6c  o place the foll
-00001cf0: 6f77 696e 6720 6173 7365 7274 696f 6e73  owing assertions
-00001d00: 2073 7461 7469 6e67 2074 6861 7420 5720   stating that W 
-00001d10: 3e3d 204d 2f32 2c20 2d57 203c 3d20 4120  >= M/2, -W <= A 
-00001d20: 3c3d 204d 2d32 5720 0d0a 2020 2020 2020  <= M-2W ..      
-00001d30: 2020 2020 3c61 7373 6572 7420 7465 7374      <assert test
-00001d40: 3d22 4057 206c 6520 2828 404d 2920 6469  ="@W le ((@M) di
-00001d50: 7620 3229 2220 2f3e 0d0a 2020 2020 2020  v 2)" />..      
-00001d60: 2020 2020 3c61 7373 6572 7420 7465 7374      <assert test
-00001d70: 3d22 4041 2067 6520 2828 2d31 292a 2840  ="@A ge ((-1)*(@
-00001d80: 5729 2922 202f 3e0d 0a20 2020 2020 2020  W))" />..       
-00001d90: 2020 203c 6173 7365 7274 2074 6573 743d     <assert test=
-00001da0: 2240 4120 6c65 2028 404d 292d 2832 2a40  "@A le (@M)-(2*@
-00001db0: 5729 222f 3e0d 0a20 2020 2020 2020 2020  W)"/>..         
-00001dc0: 2048 6f77 6576 6572 2c20 7765 2068 6176   However, we hav
-00001dd0: 6520 666f 756e 6420 6578 7065 7269 6d65  e found experime
-00001de0: 6e74 616c 6c79 2074 6861 7420 7468 6573  ntally that thes
-00001df0: 6520 7465 7374 7320 6661 696c 7320 6174  e tests fails at
-00001e00: 2074 6865 2058 4d4c 2069 6e73 7461 6e63   the XML instanc
-00001e10: 6520 6c65 7665 6c20 6576 656e 2065 7665  e level even eve
-00001e20: 6e20 6966 2074 6865 7365 2063 6f6e 6469  n if these condi
-00001e30: 7469 6f6e 7320 6172 6520 6d65 742e 0d0a  tions are met...
-00001e40: 2020 2020 2020 2020 2020 4375 7265 6e74            Curent
-00001e50: 6c79 2c20 7468 6520 6361 7573 6520 6f66  ly, the cause of
-00001e60: 2074 6869 7320 7072 6f62 6c65 6d20 6973   this problem is
-00001e70: 2075 6e63 6c65 6172 2c20 7768 6963 6820   unclear, which 
-00001e80: 6c65 6164 2075 7320 746f 2063 6f6d 6d65  lead us to comme
-00001e90: 6e74 696e 6720 6f75 7420 7468 6520 6173  nting out the as
-00001ea0: 7365 7469 6f6e 2061 6e64 206c 6561 7669  setion and leavi
-00001eb0: 6e67 2069 7420 7570 2074 6f20 0d0a 2020  ng it up to ..  
-00001ec0: 2020 2020 2020 2020 7468 6520 696d 706c          the impl
-00001ed0: 656d 656e 7469 6e67 2073 6f66 7477 6172  ementing softwar
-00001ee0: 6520 746f 2076 6572 6966 7920 7468 6174  e to verify that
-00001ef0: 2061 7474 7269 6275 7465 2076 616c 7565   attribute value
-00001f00: 7320 6172 6520 636f 7272 6563 742e 0d0a  s are correct...
-00001f10: 2020 2020 2020 2020 2d2d 3e0d 0a20 2020          -->..   
-00001f20: 2020 203c 2f65 7874 656e 7369 6f6e 3e0d     </extension>.
-00001f30: 0a20 2020 203c 2f63 6f6d 706c 6578 436f  .    </complexCo
-00001f40: 6e74 656e 743e 0d0a 2020 3c2f 636f 6d70  ntent>..  </comp
-00001f50: 6c65 7854 7970 653e 0d0a 0d0a 2020 3c63  lexType>....  <c
-00001f60: 6f6d 706c 6578 5479 7065 206e 616d 653d  omplexType name=
-00001f70: 2253 7065 6374 7275 6d4d 6174 7269 785f  "SpectrumMatrix_
-00001f80: 5479 7065 223e 0d0a 2020 2020 3c63 6f6d  Type">..    <com
-00001f90: 706c 6578 436f 6e74 656e 743e 0d0a 2020  plexContent>..  
-00001fa0: 2020 2020 3c65 7874 656e 7369 6f6e 2062      <extension b
-00001fb0: 6173 653d 2274 7261 6e73 666f 726d 733a  ase="transforms:
-00001fc0: 4162 7374 7261 6374 5472 616e 7366 6f72  AbstractTransfor
-00001fd0: 6d61 7469 6f6e 5f54 7970 6522 3e0d 0a20  mation_Type">.. 
-00001fe0: 2020 2020 2020 203c 7365 7175 656e 6365         <sequence
-00001ff0: 3e0d 0a20 2020 2020 2020 2020 203c 656c  >..          <el
-00002000: 656d 656e 7420 6e61 6d65 3d22 666c 756f  ement name="fluo
-00002010: 726f 6368 726f 6d65 7322 2074 7970 653d  rochromes" type=
-00002020: 2274 7261 6e73 666f 726d 733a 4643 5344  "transforms:FCSD
-00002030: 696d 656e 7369 6f6e 735f 5479 7065 2220  imensions_Type" 
-00002040: 2f3e 0d0a 2020 2020 2020 2020 2020 3c65  />..          <e
-00002050: 6c65 6d65 6e74 206e 616d 653d 2264 6574  lement name="det
-00002060: 6563 746f 7273 2220 7479 7065 3d22 7472  ectors" type="tr
-00002070: 616e 7366 6f72 6d73 3a46 4353 4469 6d65  ansforms:FCSDime
-00002080: 6e73 696f 6e73 5f54 7970 6522 202f 3e0d  nsions_Type" />.
-00002090: 0a20 2020 2020 2020 2020 203c 656c 656d  .          <elem
-000020a0: 656e 7420 6e61 6d65 3d22 7370 6563 7472  ent name="spectr
-000020b0: 756d 2220 7479 7065 3d22 7472 616e 7366  um" type="transf
-000020c0: 6f72 6d73 3a53 7065 6374 7275 6d5f 5479  orms:Spectrum_Ty
-000020d0: 7065 2220 6d69 6e4f 6363 7572 733d 2231  pe" minOccurs="1
-000020e0: 2220 6d61 784f 6363 7572 733d 2275 6e62  " maxOccurs="unb
-000020f0: 6f75 6e64 6564 2220 2f3e 0d0a 2020 2020  ounded" />..    
-00002100: 2020 2020 3c2f 7365 7175 656e 6365 3e0d      </sequence>.
-00002110: 0a20 2020 2020 2020 203c 6174 7472 6962  .        <attrib
-00002120: 7574 6520 6e61 6d65 3d22 6964 2220 7479  ute name="id" ty
-00002130: 7065 3d22 4944 2220 7573 653d 2272 6571  pe="ID" use="req
-00002140: 7569 7265 6422 202f 3e0d 0a20 2020 2020  uired" />..     
-00002150: 2020 203c 6174 7472 6962 7574 6520 6e61     <attribute na
-00002160: 6d65 3d22 6d61 7472 6978 2d69 6e76 6572  me="matrix-inver
-00002170: 7465 642d 616c 7265 6164 7922 2074 7970  ted-already" typ
-00002180: 653d 2262 6f6f 6c65 616e 2220 6465 6661  e="boolean" defa
-00002190: 756c 743d 2266 616c 7365 2220 7573 653d  ult="false" use=
-000021a0: 226f 7074 696f 6e61 6c22 2069 643d 226d  "optional" id="m
-000021b0: 6174 7269 782d 696e 7665 7274 6564 2d61  atrix-inverted-a
-000021c0: 6c72 6561 6479 2220 2f3e 0d0a 2020 2020  lready" />..    
-000021d0: 2020 2020 3c61 6e79 4174 7472 6962 7574      <anyAttribut
-000021e0: 6520 7072 6f63 6573 7343 6f6e 7465 6e74  e processContent
-000021f0: 733d 2273 6b69 7022 2f3e 0d0a 2020 2020  s="skip"/>..    
-00002200: 2020 3c2f 6578 7465 6e73 696f 6e3e 0d0a    </extension>..
-00002210: 2020 2020 3c2f 636f 6d70 6c65 7843 6f6e      </complexCon
-00002220: 7465 6e74 3e0d 0a20 203c 2f63 6f6d 706c  tent>..  </compl
-00002230: 6578 5479 7065 3e0d 0a0d 0a20 203c 636f  exType>....  <co
-00002240: 6d70 6c65 7854 7970 6520 6e61 6d65 3d22  mplexType name="
-00002250: 4643 5344 696d 656e 7369 6f6e 735f 5479  FCSDimensions_Ty
-00002260: 7065 223e 0d0a 2020 2020 3c67 726f 7570  pe">..    <group
-00002270: 2072 6566 3d22 6461 7461 2d74 7970 653a   ref="data-type:
-00002280: 4643 5344 696d 656e 7369 6f6e 735f 4772  FCSDimensions_Gr
-00002290: 6f75 7022 206d 696e 4f63 6375 7273 3d22  oup" minOccurs="
-000022a0: 3222 206d 6178 4f63 6375 7273 3d22 756e  2" maxOccurs="un
-000022b0: 626f 756e 6465 6422 202f 3e0d 0a20 203c  bounded" />..  <
-000022c0: 2f63 6f6d 706c 6578 5479 7065 3e0d 0a0d  /complexType>...
-000022d0: 0a20 203c 636f 6d70 6c65 7854 7970 6520  .  <complexType 
-000022e0: 6e61 6d65 3d22 5370 6563 7472 756d 5f54  name="Spectrum_T
-000022f0: 7970 6522 3e0d 0a20 2020 203c 616e 6e6f  ype">..    <anno
-00002300: 7461 7469 6f6e 3e0d 0a20 2020 2020 203c  tation>..      <
-00002310: 646f 6375 6d65 6e74 6174 696f 6e20 786d  documentation xm
-00002320: 6c3a 6c61 6e67 3d22 656e 223e 526f 7720  l:lang="en">Row 
-00002330: 6f66 2074 6865 2073 7069 6c6c 6f76 6572  of the spillover
-00002340: 2f73 7065 6374 7275 6d20 6d61 7472 6978  /spectrum matrix
-00002350: 2e3c 2f64 6f63 756d 656e 7461 7469 6f6e  .</documentation
-00002360: 3e0d 0a20 2020 203c 2f61 6e6e 6f74 6174  >..    </annotat
-00002370: 696f 6e3e 0d0a 2020 2020 3c73 6571 7565  ion>..    <seque
-00002380: 6e63 653e 0d0a 2020 2020 2020 3c65 6c65  nce>..      <ele
-00002390: 6d65 6e74 206e 616d 653d 2263 6f65 6666  ment name="coeff
-000023a0: 6963 6965 6e74 2220 7479 7065 3d22 7472  icient" type="tr
-000023b0: 616e 7366 6f72 6d73 3a53 7065 6374 7275  ansforms:Spectru
-000023c0: 6d43 6f65 6666 6963 6965 6e74 5f54 7970  mCoefficient_Typ
-000023d0: 6522 206d 696e 4f63 6375 7273 3d22 3122  e" minOccurs="1"
-000023e0: 206d 6178 4f63 6375 7273 3d22 756e 626f   maxOccurs="unbo
-000023f0: 756e 6465 6422 202f 3e0d 0a20 2020 203c  unded" />..    <
-00002400: 2f73 6571 7565 6e63 653e 0d0a 2020 3c2f  /sequence>..  </
-00002410: 636f 6d70 6c65 7854 7970 653e 0d0a 0d0a  complexType>....
-00002420: 2020 3c63 6f6d 706c 6578 5479 7065 206e    <complexType n
-00002430: 616d 653d 2253 7065 6374 7275 6d43 6f65  ame="SpectrumCoe
-00002440: 6666 6963 6965 6e74 5f54 7970 6522 3e0d  fficient_Type">.
-00002450: 0a20 2020 203c 6174 7472 6962 7574 6520  .    <attribute 
-00002460: 6e61 6d65 3d22 7661 6c75 6522 2074 7970  name="value" typ
-00002470: 653d 2264 6174 612d 7479 7065 3a46 6c6f  e="data-type:Flo
-00002480: 6174 3634 5f54 7970 6522 2075 7365 3d22  at64_Type" use="
-00002490: 7265 7175 6972 6564 2220 2f3e 0d0a 2020  required" />..  
-000024a0: 3c2f 636f 6d70 6c65 7854 7970 653e 0d0a  </complexType>..
-000024b0: 0d0a 3c2f 7363 6865 6d61 3e0d 0a         ..</schema>..
+00000fd0: 0a20 2020 2020 2020 203c 6772 6f75 7020  .        <group 
+00000fe0: 7265 663d 2264 6174 612d 7479 7065 3a46  ref="data-type:F
+00000ff0: 4353 4469 6d65 6e73 696f 6e73 5f47 726f  CSDimensions_Gro
+00001000: 7570 2220 6d69 6e4f 6363 7572 733d 2232  up" minOccurs="2
+00001010: 2220 6d61 784f 6363 7572 733d 2232 2220  " maxOccurs="2" 
+00001020: 2f3e 0a20 2020 2020 2020 203c 6174 7472  />.        <attr
+00001030: 6962 7574 6520 6e61 6d65 3d22 4122 2074  ibute name="A" t
+00001040: 7970 653d 2264 6174 612d 7479 7065 3a46  ype="data-type:F
+00001050: 6c6f 6174 3634 5f54 7970 6522 2075 7365  loat64_Type" use
+00001060: 3d22 7265 7175 6972 6564 2220 2f3e 0a20  ="required" />. 
+00001070: 2020 2020 2020 203c 6174 7472 6962 7574         <attribut
+00001080: 6520 6e61 6d65 3d22 4222 2074 7970 653d  e name="B" type=
+00001090: 2264 6174 612d 7479 7065 3a46 6c6f 6174  "data-type:Float
+000010a0: 3634 5f54 7970 6522 2075 7365 3d22 7265  64_Type" use="re
+000010b0: 7175 6972 6564 2220 2f3e 0a20 2020 2020  quired" />.     
+000010c0: 2020 203c 6174 7472 6962 7574 6520 6e61     <attribute na
+000010d0: 6d65 3d22 4322 2074 7970 653d 2264 6174  me="C" type="dat
+000010e0: 612d 7479 7065 3a46 6c6f 6174 3634 5f54  a-type:Float64_T
+000010f0: 7970 6522 2075 7365 3d22 7265 7175 6972  ype" use="requir
+00001100: 6564 2220 2f3e 0a20 2020 2020 203c 2f65  ed" />.      </e
+00001110: 7874 656e 7369 6f6e 3e0a 2020 2020 3c2f  xtension>.    </
+00001120: 636f 6d70 6c65 7843 6f6e 7465 6e74 3e0a  complexContent>.
+00001130: 2020 3c2f 636f 6d70 6c65 7854 7970 653e    </complexType>
+00001140: 0a0a 2020 3c63 6f6d 706c 6578 5479 7065  ..  <complexType
+00001150: 206e 616d 653d 2246 4c6f 6754 7261 6e73   name="FLogTrans
+00001160: 666f 726d 6174 696f 6e5f 5479 7065 223e  formation_Type">
+00001170: 0a20 2020 203c 636f 6d70 6c65 7843 6f6e  .    <complexCon
+00001180: 7465 6e74 3e0a 2020 2020 2020 3c65 7874  tent>.      <ext
+00001190: 656e 7369 6f6e 2062 6173 653d 2274 7261  ension base="tra
+000011a0: 6e73 666f 726d 733a 4162 7374 7261 6374  nsforms:Abstract
+000011b0: 5472 616e 7366 6f72 6d61 7469 6f6e 5f54  Transformation_T
+000011c0: 7970 6522 3e0a 2020 2020 2020 2020 3c61  ype">.        <a
+000011d0: 7474 7269 6275 7465 206e 616d 653d 2254  ttribute name="T
+000011e0: 2220 7479 7065 3d22 6461 7461 2d74 7970  " type="data-typ
+000011f0: 653a 5046 6c6f 6174 3634 5f54 7970 6522  e:PFloat64_Type"
+00001200: 2075 7365 3d22 7265 7175 6972 6564 2220   use="required" 
+00001210: 2f3e 0a20 2020 2020 2020 203c 6174 7472  />.        <attr
+00001220: 6962 7574 6520 6e61 6d65 3d22 4d22 2074  ibute name="M" t
+00001230: 7970 653d 2264 6174 612d 7479 7065 3a50  ype="data-type:P
+00001240: 466c 6f61 7436 345f 5479 7065 2220 7573  Float64_Type" us
+00001250: 653d 2272 6571 7569 7265 6422 202f 3e0a  e="required" />.
+00001260: 2020 2020 2020 3c2f 6578 7465 6e73 696f        </extensio
+00001270: 6e3e 0a20 2020 203c 2f63 6f6d 706c 6578  n>.    </complex
+00001280: 436f 6e74 656e 743e 0a20 203c 2f63 6f6d  Content>.  </com
+00001290: 706c 6578 5479 7065 3e0a 0a20 203c 636f  plexType>..  <co
+000012a0: 6d70 6c65 7854 7970 6520 6e61 6d65 3d22  mplexType name="
+000012b0: 4641 5369 6e48 5472 616e 7366 6f72 6d61  FASinHTransforma
+000012c0: 7469 6f6e 5f54 7970 6522 3e0a 2020 2020  tion_Type">.    
+000012d0: 3c63 6f6d 706c 6578 436f 6e74 656e 743e  <complexContent>
+000012e0: 0a20 2020 2020 203c 6578 7465 6e73 696f  .      <extensio
+000012f0: 6e20 6261 7365 3d22 7472 616e 7366 6f72  n base="transfor
+00001300: 6d73 3a41 6273 7472 6163 7454 7261 6e73  ms:AbstractTrans
+00001310: 666f 726d 6174 696f 6e5f 5479 7065 223e  formation_Type">
+00001320: 0a20 2020 2020 2020 203c 6174 7472 6962  .        <attrib
+00001330: 7574 6520 6e61 6d65 3d22 5422 2074 7970  ute name="T" typ
+00001340: 653d 2264 6174 612d 7479 7065 3a50 466c  e="data-type:PFl
+00001350: 6f61 7436 345f 5479 7065 2220 7573 653d  oat64_Type" use=
+00001360: 2272 6571 7569 7265 6422 202f 3e0a 2020  "required" />.  
+00001370: 2020 2020 2020 3c61 7474 7269 6275 7465        <attribute
+00001380: 206e 616d 653d 224d 2220 7479 7065 3d22   name="M" type="
+00001390: 6461 7461 2d74 7970 653a 5046 6c6f 6174  data-type:PFloat
+000013a0: 3634 5f54 7970 6522 2075 7365 3d22 7265  64_Type" use="re
+000013b0: 7175 6972 6564 2220 2f3e 0a20 2020 2020  quired" />.     
+000013c0: 2020 203c 6174 7472 6962 7574 6520 6e61     <attribute na
+000013d0: 6d65 3d22 4122 2074 7970 653d 2264 6174  me="A" type="dat
+000013e0: 612d 7479 7065 3a55 466c 6f61 7436 345f  a-type:UFloat64_
+000013f0: 5479 7065 2220 7573 653d 2272 6571 7569  Type" use="requi
+00001400: 7265 6422 202f 3e0a 2020 2020 2020 3c2f  red" />.      </
+00001410: 6578 7465 6e73 696f 6e3e 0a20 2020 2020  extension>.     
+00001420: 203c 212d 2d0a 2020 2020 2020 2020 5853   <!--.        XS
+00001430: 4431 2e31 2061 6c6c 6f77 7320 7573 2074  D1.1 allows us t
+00001440: 6f20 706c 6163 6520 7468 6520 666f 6c6c  o place the foll
+00001450: 6f77 696e 6720 6173 7365 7274 696f 6e20  owing assertion 
+00001460: 7374 6174 696e 6720 7468 6174 2054 3e41  stating that T>A
+00001470: 200a 2020 2020 2020 2020 3c61 7373 6572   .        <asser
+00001480: 7420 7465 7374 3d22 404d 2067 7465 2040  t test="@M gte @
+00001490: 4122 202f 3e0a 2020 2020 2020 2020 486f  A" />.        Ho
+000014a0: 7765 7665 722c 2077 6520 6861 7665 2066  wever, we have f
+000014b0: 6f75 6e64 2065 7870 6572 696d 656e 7461  ound experimenta
+000014c0: 6c6c 7920 7468 6174 2074 6869 7320 7465  lly that this te
+000014d0: 7374 2066 6169 6c73 2061 7420 7468 6520  st fails at the 
+000014e0: 584d 4c20 696e 7374 616e 6365 206c 6576  XML instance lev
+000014f0: 656c 2065 7665 6e20 6576 656e 2069 6620  el even even if 
+00001500: 7468 6973 2063 6f6e 6469 7469 6f6e 2069  this condition i
+00001510: 7320 6d65 742e 0a20 2020 2020 2020 2043  s met..        C
+00001520: 7572 656e 746c 792c 2074 6865 2063 6175  urently, the cau
+00001530: 7365 206f 6620 7468 6973 2070 726f 626c  se of this probl
+00001540: 656d 2069 7320 756e 636c 6561 722c 2077  em is unclear, w
+00001550: 6869 6368 206c 6561 6420 7573 2074 6f20  hich lead us to 
+00001560: 636f 6d6d 656e 7469 6e67 206f 7574 2074  commenting out t
+00001570: 6865 2061 7373 6574 696f 6e20 616e 6420  he assetion and 
+00001580: 6c65 6176 696e 6720 6974 2075 7020 746f  leaving it up to
+00001590: 200a 2020 2020 2020 2020 7468 6520 696d   .        the im
+000015a0: 706c 656d 656e 7469 6e67 2073 6f66 7477  plementing softw
+000015b0: 6172 6520 746f 2076 6572 6966 7920 7468  are to verify th
+000015c0: 6174 2061 7474 7269 6275 7465 2076 616c  at attribute val
+000015d0: 7565 7320 6172 6520 636f 7272 6563 742e  ues are correct.
+000015e0: 0a20 2020 2020 202d 2d3e 0a20 2020 203c  .      -->.    <
+000015f0: 2f63 6f6d 706c 6578 436f 6e74 656e 743e  /complexContent>
+00001600: 0a20 203c 2f63 6f6d 706c 6578 5479 7065  .  </complexType
+00001610: 3e0a 0a20 203c 636f 6d70 6c65 7854 7970  >..  <complexTyp
+00001620: 6520 6e61 6d65 3d22 4879 7065 726c 6f67  e name="Hyperlog
+00001630: 5472 616e 7366 6f72 6d61 7469 6f6e 5f54  Transformation_T
+00001640: 7970 6522 3e0a 2020 2020 3c63 6f6d 706c  ype">.    <compl
+00001650: 6578 436f 6e74 656e 743e 0a20 2020 2020  exContent>.     
+00001660: 203c 6578 7465 6e73 696f 6e20 6261 7365   <extension base
+00001670: 3d22 7472 616e 7366 6f72 6d73 3a41 6273  ="transforms:Abs
+00001680: 7472 6163 7454 7261 6e73 666f 726d 6174  tractTransformat
+00001690: 696f 6e5f 5479 7065 223e 0a20 2020 2020  ion_Type">.     
+000016a0: 2020 203c 6174 7472 6962 7574 6520 6e61     <attribute na
+000016b0: 6d65 3d22 5422 2074 7970 653d 2264 6174  me="T" type="dat
+000016c0: 612d 7479 7065 3a50 466c 6f61 7436 345f  a-type:PFloat64_
+000016d0: 5479 7065 2220 7573 653d 2272 6571 7569  Type" use="requi
+000016e0: 7265 6422 202f 3e0a 2020 2020 2020 2020  red" />.        
+000016f0: 3c61 7474 7269 6275 7465 206e 616d 653d  <attribute name=
+00001700: 224d 2220 7479 7065 3d22 6461 7461 2d74  "M" type="data-t
+00001710: 7970 653a 5046 6c6f 6174 3634 5f54 7970  ype:PFloat64_Typ
+00001720: 6522 2075 7365 3d22 7265 7175 6972 6564  e" use="required
+00001730: 2220 2f3e 0a20 2020 2020 2020 203c 6174  " />.        <at
+00001740: 7472 6962 7574 6520 6e61 6d65 3d22 5722  tribute name="W"
+00001750: 2074 7970 653d 2264 6174 612d 7479 7065   type="data-type
+00001760: 3a50 466c 6f61 7436 345f 5479 7065 2220  :PFloat64_Type" 
+00001770: 7573 653d 2272 6571 7569 7265 6422 202f  use="required" /
+00001780: 3e0a 2020 2020 2020 2020 3c61 7474 7269  >.        <attri
+00001790: 6275 7465 206e 616d 653d 2241 2220 7479  bute name="A" ty
+000017a0: 7065 3d22 6461 7461 2d74 7970 653a 466c  pe="data-type:Fl
+000017b0: 6f61 7436 345f 5479 7065 2220 7573 653d  oat64_Type" use=
+000017c0: 2272 6571 7569 7265 6422 202f 3e0a 2020  "required" />.  
+000017d0: 2020 2020 2020 3c21 2d2d 0a20 2020 2020        <!--.     
+000017e0: 2020 2020 2058 5344 312e 3120 616c 6c6f       XSD1.1 allo
+000017f0: 7773 2075 7320 746f 2070 6c61 6365 2074  ws us to place t
+00001800: 6865 2066 6f6c 6c6f 7769 6e67 2061 7373  he following ass
+00001810: 6572 7469 6f6e 7320 7374 6174 696e 6720  ertions stating 
+00001820: 7468 6174 2057 203e 3d20 4d2f 322c 202d  that W >= M/2, -
+00001830: 5720 3c3d 2041 203c 3d20 4d2d 3257 200a  W <= A <= M-2W .
+00001840: 2020 2020 2020 2020 2020 3c61 7373 6572            <asser
+00001850: 7420 7465 7374 3d22 4057 206c 6520 2828  t test="@W le ((
+00001860: 404d 2920 6469 7620 3229 2220 2f3e 0a20  @M) div 2)" />. 
+00001870: 2020 2020 2020 2020 203c 6173 7365 7274           <assert
+00001880: 2074 6573 743d 2240 4120 6765 2028 282d   test="@A ge ((-
+00001890: 3129 2a28 4057 2929 2220 2f3e 0a20 2020  1)*(@W))" />.   
+000018a0: 2020 2020 2020 203c 6173 7365 7274 2074         <assert t
+000018b0: 6573 743d 2240 4120 6c65 2028 404d 292d  est="@A le (@M)-
+000018c0: 2832 2a40 5729 222f 3e0a 2020 2020 2020  (2*@W)"/>.      
+000018d0: 2020 2020 486f 7765 7665 722c 2077 6520      However, we 
+000018e0: 6861 7665 2066 6f75 6e64 2065 7870 6572  have found exper
+000018f0: 696d 656e 7461 6c6c 7920 7468 6174 2074  imentally that t
+00001900: 6865 7365 2074 6573 7473 2066 6169 6c73  hese tests fails
+00001910: 2061 7420 7468 6520 584d 4c20 696e 7374   at the XML inst
+00001920: 616e 6365 206c 6576 656c 2065 7665 6e20  ance level even 
+00001930: 6576 656e 2069 6620 7468 6573 6520 636f  even if these co
+00001940: 6e64 6974 696f 6e73 2061 7265 206d 6574  nditions are met
+00001950: 2e0a 2020 2020 2020 2020 2020 4375 7265  ..          Cure
+00001960: 6e74 6c79 2c20 7468 6520 6361 7573 6520  ntly, the cause 
+00001970: 6f66 2074 6869 7320 7072 6f62 6c65 6d20  of this problem 
+00001980: 6973 2075 6e63 6c65 6172 2c20 7768 6963  is unclear, whic
+00001990: 6820 6c65 6164 2075 7320 746f 2063 6f6d  h lead us to com
+000019a0: 6d65 6e74 696e 6720 6f75 7420 7468 6520  menting out the 
+000019b0: 6173 7365 7469 6f6e 2061 6e64 206c 6561  assetion and lea
+000019c0: 7669 6e67 2069 7420 7570 2074 6f20 0a20  ving it up to . 
+000019d0: 2020 2020 2020 2020 2074 6865 2069 6d70           the imp
+000019e0: 6c65 6d65 6e74 696e 6720 736f 6674 7761  lementing softwa
+000019f0: 7265 2074 6f20 7665 7269 6679 2074 6861  re to verify tha
+00001a00: 7420 6174 7472 6962 7574 6520 7661 6c75  t attribute valu
+00001a10: 6573 2061 7265 2063 6f72 7265 6374 2e0a  es are correct..
+00001a20: 2020 2020 2020 2020 2d2d 3e0a 2020 2020          -->.    
+00001a30: 2020 3c2f 6578 7465 6e73 696f 6e3e 0a20    </extension>. 
+00001a40: 2020 203c 2f63 6f6d 706c 6578 436f 6e74     </complexCont
+00001a50: 656e 743e 0a20 203c 2f63 6f6d 706c 6578  ent>.  </complex
+00001a60: 5479 7065 3e0a 0a20 203c 636f 6d70 6c65  Type>..  <comple
+00001a70: 7854 7970 6520 6e61 6d65 3d22 4c6f 6769  xType name="Logi
+00001a80: 636c 6554 7261 6e73 666f 726d 6174 696f  cleTransformatio
+00001a90: 6e5f 5479 7065 223e 0a20 2020 203c 636f  n_Type">.    <co
+00001aa0: 6d70 6c65 7843 6f6e 7465 6e74 3e0a 2020  mplexContent>.  
+00001ab0: 2020 2020 3c65 7874 656e 7369 6f6e 2062      <extension b
+00001ac0: 6173 653d 2274 7261 6e73 666f 726d 733a  ase="transforms:
+00001ad0: 4162 7374 7261 6374 5472 616e 7366 6f72  AbstractTransfor
+00001ae0: 6d61 7469 6f6e 5f54 7970 6522 3e0a 2020  mation_Type">.  
+00001af0: 2020 2020 2020 3c61 7474 7269 6275 7465        <attribute
+00001b00: 206e 616d 653d 2254 2220 7479 7065 3d22   name="T" type="
+00001b10: 6461 7461 2d74 7970 653a 5046 6c6f 6174  data-type:PFloat
+00001b20: 3634 5f54 7970 6522 2075 7365 3d22 7265  64_Type" use="re
+00001b30: 7175 6972 6564 2220 2f3e 0a20 2020 2020  quired" />.     
+00001b40: 2020 203c 6174 7472 6962 7574 6520 6e61     <attribute na
+00001b50: 6d65 3d22 4d22 2074 7970 653d 2264 6174  me="M" type="dat
+00001b60: 612d 7479 7065 3a50 466c 6f61 7436 345f  a-type:PFloat64_
+00001b70: 5479 7065 2220 7573 653d 2272 6571 7569  Type" use="requi
+00001b80: 7265 6422 202f 3e0a 2020 2020 2020 2020  red" />.        
+00001b90: 3c61 7474 7269 6275 7465 206e 616d 653d  <attribute name=
+00001ba0: 2257 2220 7479 7065 3d22 6461 7461 2d74  "W" type="data-t
+00001bb0: 7970 653a 5546 6c6f 6174 3634 5f54 7970  ype:UFloat64_Typ
+00001bc0: 6522 2075 7365 3d22 7265 7175 6972 6564  e" use="required
+00001bd0: 2220 2f3e 0a20 2020 2020 2020 203c 6174  " />.        <at
+00001be0: 7472 6962 7574 6520 6e61 6d65 3d22 4122  tribute name="A"
+00001bf0: 2074 7970 653d 2264 6174 612d 7479 7065   type="data-type
+00001c00: 3a46 6c6f 6174 3634 5f54 7970 6522 2075  :Float64_Type" u
+00001c10: 7365 3d22 7265 7175 6972 6564 2220 2f3e  se="required" />
+00001c20: 0a20 2020 2020 2020 203c 212d 2d0a 2020  .        <!--.  
+00001c30: 2020 2020 2020 2020 5853 4431 2e31 2061          XSD1.1 a
+00001c40: 6c6c 6f77 7320 7573 2074 6f20 706c 6163  llows us to plac
+00001c50: 6520 7468 6520 666f 6c6c 6f77 696e 6720  e the following 
+00001c60: 6173 7365 7274 696f 6e73 2073 7461 7469  assertions stati
+00001c70: 6e67 2074 6861 7420 5720 3e3d 204d 2f32  ng that W >= M/2
+00001c80: 2c20 2d57 203c 3d20 4120 3c3d 204d 2d32  , -W <= A <= M-2
+00001c90: 5720 0a20 2020 2020 2020 2020 203c 6173  W .          <as
+00001ca0: 7365 7274 2074 6573 743d 2240 5720 6c65  sert test="@W le
+00001cb0: 2028 2840 4d29 2064 6976 2032 2922 202f   ((@M) div 2)" /
+00001cc0: 3e0a 2020 2020 2020 2020 2020 3c61 7373  >.          <ass
+00001cd0: 6572 7420 7465 7374 3d22 4041 2067 6520  ert test="@A ge 
+00001ce0: 2828 2d31 292a 2840 5729 2922 202f 3e0a  ((-1)*(@W))" />.
+00001cf0: 2020 2020 2020 2020 2020 3c61 7373 6572            <asser
+00001d00: 7420 7465 7374 3d22 4041 206c 6520 2840  t test="@A le (@
+00001d10: 4d29 2d28 322a 4057 2922 2f3e 0a20 2020  M)-(2*@W)"/>.   
+00001d20: 2020 2020 2020 2048 6f77 6576 6572 2c20         However, 
+00001d30: 7765 2068 6176 6520 666f 756e 6420 6578  we have found ex
+00001d40: 7065 7269 6d65 6e74 616c 6c79 2074 6861  perimentally tha
+00001d50: 7420 7468 6573 6520 7465 7374 7320 6661  t these tests fa
+00001d60: 696c 7320 6174 2074 6865 2058 4d4c 2069  ils at the XML i
+00001d70: 6e73 7461 6e63 6520 6c65 7665 6c20 6576  nstance level ev
+00001d80: 656e 2065 7665 6e20 6966 2074 6865 7365  en even if these
+00001d90: 2063 6f6e 6469 7469 6f6e 7320 6172 6520   conditions are 
+00001da0: 6d65 742e 0a20 2020 2020 2020 2020 2043  met..          C
+00001db0: 7572 656e 746c 792c 2074 6865 2063 6175  urently, the cau
+00001dc0: 7365 206f 6620 7468 6973 2070 726f 626c  se of this probl
+00001dd0: 656d 2069 7320 756e 636c 6561 722c 2077  em is unclear, w
+00001de0: 6869 6368 206c 6561 6420 7573 2074 6f20  hich lead us to 
+00001df0: 636f 6d6d 656e 7469 6e67 206f 7574 2074  commenting out t
+00001e00: 6865 2061 7373 6574 696f 6e20 616e 6420  he assetion and 
+00001e10: 6c65 6176 696e 6720 6974 2075 7020 746f  leaving it up to
+00001e20: 200a 2020 2020 2020 2020 2020 7468 6520   .          the 
+00001e30: 696d 706c 656d 656e 7469 6e67 2073 6f66  implementing sof
+00001e40: 7477 6172 6520 746f 2076 6572 6966 7920  tware to verify 
+00001e50: 7468 6174 2061 7474 7269 6275 7465 2076  that attribute v
+00001e60: 616c 7565 7320 6172 6520 636f 7272 6563  alues are correc
+00001e70: 742e 0a20 2020 2020 2020 202d 2d3e 0a20  t..        -->. 
+00001e80: 2020 2020 203c 2f65 7874 656e 7369 6f6e       </extension
+00001e90: 3e0a 2020 2020 3c2f 636f 6d70 6c65 7843  >.    </complexC
+00001ea0: 6f6e 7465 6e74 3e0a 2020 3c2f 636f 6d70  ontent>.  </comp
+00001eb0: 6c65 7854 7970 653e 0a0a 2020 3c63 6f6d  lexType>..  <com
+00001ec0: 706c 6578 5479 7065 206e 616d 653d 2253  plexType name="S
+00001ed0: 7065 6374 7275 6d4d 6174 7269 785f 5479  pectrumMatrix_Ty
+00001ee0: 7065 223e 0a20 2020 203c 636f 6d70 6c65  pe">.    <comple
+00001ef0: 7843 6f6e 7465 6e74 3e0a 2020 2020 2020  xContent>.      
+00001f00: 3c65 7874 656e 7369 6f6e 2062 6173 653d  <extension base=
+00001f10: 2274 7261 6e73 666f 726d 733a 4162 7374  "transforms:Abst
+00001f20: 7261 6374 5472 616e 7366 6f72 6d61 7469  ractTransformati
+00001f30: 6f6e 5f54 7970 6522 3e0a 2020 2020 2020  on_Type">.      
+00001f40: 2020 3c73 6571 7565 6e63 653e 0a20 2020    <sequence>.   
+00001f50: 2020 2020 2020 203c 656c 656d 656e 7420         <element 
+00001f60: 6e61 6d65 3d22 666c 756f 726f 6368 726f  name="fluorochro
+00001f70: 6d65 7322 2074 7970 653d 2274 7261 6e73  mes" type="trans
+00001f80: 666f 726d 733a 4643 5344 696d 656e 7369  forms:FCSDimensi
+00001f90: 6f6e 735f 5479 7065 2220 2f3e 0a20 2020  ons_Type" />.   
+00001fa0: 2020 2020 2020 203c 656c 656d 656e 7420         <element 
+00001fb0: 6e61 6d65 3d22 6465 7465 6374 6f72 7322  name="detectors"
+00001fc0: 2074 7970 653d 2274 7261 6e73 666f 726d   type="transform
+00001fd0: 733a 4643 5344 696d 656e 7369 6f6e 735f  s:FCSDimensions_
+00001fe0: 5479 7065 2220 2f3e 0a20 2020 2020 2020  Type" />.       
+00001ff0: 2020 203c 656c 656d 656e 7420 6e61 6d65     <element name
+00002000: 3d22 7370 6563 7472 756d 2220 7479 7065  ="spectrum" type
+00002010: 3d22 7472 616e 7366 6f72 6d73 3a53 7065  ="transforms:Spe
+00002020: 6374 7275 6d5f 5479 7065 2220 6d69 6e4f  ctrum_Type" minO
+00002030: 6363 7572 733d 2231 2220 6d61 784f 6363  ccurs="1" maxOcc
+00002040: 7572 733d 2275 6e62 6f75 6e64 6564 2220  urs="unbounded" 
+00002050: 2f3e 0a20 2020 2020 2020 203c 2f73 6571  />.        </seq
+00002060: 7565 6e63 653e 0a20 2020 2020 2020 203c  uence>.        <
+00002070: 6174 7472 6962 7574 6520 6e61 6d65 3d22  attribute name="
+00002080: 6964 2220 7479 7065 3d22 4944 2220 7573  id" type="ID" us
+00002090: 653d 2272 6571 7569 7265 6422 202f 3e0a  e="required" />.
+000020a0: 2020 2020 2020 2020 3c61 7474 7269 6275          <attribu
+000020b0: 7465 206e 616d 653d 226d 6174 7269 782d  te name="matrix-
+000020c0: 696e 7665 7274 6564 2d61 6c72 6561 6479  inverted-already
+000020d0: 2220 7479 7065 3d22 626f 6f6c 6561 6e22  " type="boolean"
+000020e0: 2064 6566 6175 6c74 3d22 6661 6c73 6522   default="false"
+000020f0: 2075 7365 3d22 6f70 7469 6f6e 616c 2220   use="optional" 
+00002100: 6964 3d22 6d61 7472 6978 2d69 6e76 6572  id="matrix-inver
+00002110: 7465 642d 616c 7265 6164 7922 202f 3e0a  ted-already" />.
+00002120: 2020 2020 2020 2020 3c61 6e79 4174 7472          <anyAttr
+00002130: 6962 7574 6520 7072 6f63 6573 7343 6f6e  ibute processCon
+00002140: 7465 6e74 733d 2273 6b69 7022 2f3e 0a20  tents="skip"/>. 
+00002150: 2020 2020 203c 2f65 7874 656e 7369 6f6e       </extension
+00002160: 3e0a 2020 2020 3c2f 636f 6d70 6c65 7843  >.    </complexC
+00002170: 6f6e 7465 6e74 3e0a 2020 3c2f 636f 6d70  ontent>.  </comp
+00002180: 6c65 7854 7970 653e 0a0a 2020 3c63 6f6d  lexType>..  <com
+00002190: 706c 6578 5479 7065 206e 616d 653d 2246  plexType name="F
+000021a0: 4353 4469 6d65 6e73 696f 6e73 5f54 7970  CSDimensions_Typ
+000021b0: 6522 3e0a 2020 2020 3c67 726f 7570 2072  e">.    <group r
+000021c0: 6566 3d22 6461 7461 2d74 7970 653a 4643  ef="data-type:FC
+000021d0: 5344 696d 656e 7369 6f6e 735f 4772 6f75  SDimensions_Grou
+000021e0: 7022 206d 696e 4f63 6375 7273 3d22 3222  p" minOccurs="2"
+000021f0: 206d 6178 4f63 6375 7273 3d22 756e 626f   maxOccurs="unbo
+00002200: 756e 6465 6422 202f 3e0a 2020 3c2f 636f  unded" />.  </co
+00002210: 6d70 6c65 7854 7970 653e 0a0a 2020 3c63  mplexType>..  <c
+00002220: 6f6d 706c 6578 5479 7065 206e 616d 653d  omplexType name=
+00002230: 2253 7065 6374 7275 6d5f 5479 7065 223e  "Spectrum_Type">
+00002240: 0a20 2020 203c 616e 6e6f 7461 7469 6f6e  .    <annotation
+00002250: 3e0a 2020 2020 2020 3c64 6f63 756d 656e  >.      <documen
+00002260: 7461 7469 6f6e 2078 6d6c 3a6c 616e 673d  tation xml:lang=
+00002270: 2265 6e22 3e52 6f77 206f 6620 7468 6520  "en">Row of the 
+00002280: 7370 696c 6c6f 7665 722f 7370 6563 7472  spillover/spectr
+00002290: 756d 206d 6174 7269 782e 3c2f 646f 6375  um matrix.</docu
+000022a0: 6d65 6e74 6174 696f 6e3e 0a20 2020 203c  mentation>.    <
+000022b0: 2f61 6e6e 6f74 6174 696f 6e3e 0a20 2020  /annotation>.   
+000022c0: 203c 7365 7175 656e 6365 3e0a 2020 2020   <sequence>.    
+000022d0: 2020 3c65 6c65 6d65 6e74 206e 616d 653d    <element name=
+000022e0: 2263 6f65 6666 6963 6965 6e74 2220 7479  "coefficient" ty
+000022f0: 7065 3d22 7472 616e 7366 6f72 6d73 3a53  pe="transforms:S
+00002300: 7065 6374 7275 6d43 6f65 6666 6963 6965  pectrumCoefficie
+00002310: 6e74 5f54 7970 6522 206d 696e 4f63 6375  nt_Type" minOccu
+00002320: 7273 3d22 3122 206d 6178 4f63 6375 7273  rs="1" maxOccurs
+00002330: 3d22 756e 626f 756e 6465 6422 202f 3e0a  ="unbounded" />.
+00002340: 2020 2020 3c2f 7365 7175 656e 6365 3e0a      </sequence>.
+00002350: 2020 3c2f 636f 6d70 6c65 7854 7970 653e    </complexType>
+00002360: 0a0a 2020 3c63 6f6d 706c 6578 5479 7065  ..  <complexType
+00002370: 206e 616d 653d 2253 7065 6374 7275 6d43   name="SpectrumC
+00002380: 6f65 6666 6963 6965 6e74 5f54 7970 6522  oefficient_Type"
+00002390: 3e0a 2020 2020 3c61 7474 7269 6275 7465  >.    <attribute
+000023a0: 206e 616d 653d 2276 616c 7565 2220 7479   name="value" ty
+000023b0: 7065 3d22 6461 7461 2d74 7970 653a 466c  pe="data-type:Fl
+000023c0: 6f61 7436 345f 5479 7065 2220 7573 653d  oat64_Type" use=
+000023d0: 2272 6571 7569 7265 6422 202f 3e0a 2020  "required" />.  
+000023e0: 3c2f 636f 6d70 6c65 7854 7970 653e 0a0a  </complexType>..
+000023f0: 3c2f 7363 6865 6d61 3e0a                 </schema>.
```

### Comparing `FlowKit-1.0.1/flowkit/_resources/__init__.py` & `FlowKit-1.1.0/src/flowkit/_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.1/flowkit/_utils/gating_utils.py` & `FlowKit-1.1.0/src/flowkit/_utils/gating_utils.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.1/flowkit/_utils/wsp_utils.py` & `FlowKit-1.1.0/src/flowkit/_utils/wsp_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """
 Utility functions related to FlowJo Workspace files (.wsp)
 """
 import copy
 import datetime
+import os
 import re
 import numpy as np
+from urllib.parse import urlparse, unquote
 from lxml import etree
 from flowio.fcs_keywords import FCS_STANDARD_KEYWORDS
-from .xml_utils import find_attribute_value, _get_xml_type
+from .xml_common import find_attribute_value, _get_xml_type
 from .._models.dimension import Dimension
 # noinspection PyProtectedMember
 from .._models.transforms._matrix import Matrix
 # noinspection PyProtectedMember
 from .._models.transforms import _transforms, _wsp_transforms
 # noinspection PyProtectedMember
 from .._models.gates._gates import PolygonGate, RectangleGate
@@ -30,14 +32,32 @@
     'PolygonGate': GMLPolygonGate,
     'EllipsoidGate': WSPEllipsoidGate,
     'QuadrantGate': GMLQuadrantGate,
     'BooleanGate': GMLBooleanGate
 }
 
 
+def _uri_to_path(uri, wsp_file_path):
+    """Convert a URI to a file path, handling both relative and absolute paths."""
+    parsed = urlparse(uri)
+
+    if parsed.scheme not in ('file', ''):
+        raise ValueError("Unsupported URI scheme: {}".format(parsed.scheme))
+
+    parsed_path = unquote(parsed.path)
+
+    # if the path is relative, join it with the wsp file's directory
+    if os.path.isabs(parsed_path):
+        return parsed_path
+    else:
+        # The relative path is relative to the wsp file's directory, so prepend that.
+        base_path = os.path.dirname(os.path.abspath(wsp_file_path))
+        return os.path.join(base_path, parsed_path)
+
+
 def _parse_wsp_compensation(sample_el, transform_ns, data_type_ns):
     # Find spilloverMatrix elements, not sure if there should be just a
     # single matrix or multiple. Going with a single one now since there
     # do not appear to be comp references in the WSP gate elements.
     matrix_els = sample_el.findall(
         '%s:spilloverMatrix' % transform_ns,
         namespaces=sample_el.nsmap
@@ -162,15 +182,14 @@
             # biex transform has 5 parameters, but only 2 are really used
             # these are attributes of the 'biex' element
             param_neg = find_attribute_value(xform_el, transform_ns, 'neg')
             param_width = find_attribute_value(xform_el, transform_ns, 'width')
             param_length = find_attribute_value(xform_el, transform_ns, 'length')
             param_max_range = find_attribute_value(xform_el, transform_ns, 'maxRange')
             param_pos = find_attribute_value(xform_el, transform_ns, 'pos')
-            param_pos = round(float(param_pos), 2)
 
             if param_length != '256':
                 raise ValueError("FlowJo biex 'length' parameter value of %s is not supported." % param_length)
 
             xforms_lut[param_name] = _wsp_transforms.WSPBiexTransform(
                 param_name,
                 negative=float(param_neg),
@@ -215,15 +234,15 @@
         keyword_value = keyword_el.attrib['value']
 
         keywords_lut[keyword_name] = keyword_value
 
     return keywords_lut
 
 
-def _convert_wsp_gate(wsp_gate, comp_matrix, xform_lut, ignore_transforms=False):
+def _convert_wsp_gate(wsp_gate, comp_matrix, xform_lut):
     new_dims = []
     xforms = []
 
     for dim in wsp_gate.dimensions:
         if comp_matrix is not None:
             pre = comp_matrix['prefix']
             suf = comp_matrix['suffix']
@@ -242,23 +261,23 @@
             dim_id = dim.id
             comp_ref = None
 
         xform_id = None
         new_dim_min = None
         new_dim_max = None
 
-        if dim_id in xform_lut and not ignore_transforms:
+        if dim_id in xform_lut:
             xform = xform_lut[dim_id]
             xforms.append(xform)  # need these later for vertices, coordinates, etc.
             xform_id = xform.id
             if dim.min is not None:
-                new_dim_min = xform.apply(np.array([[float(dim.min)]]))
+                new_dim_min = xform.apply(np.array([[float(dim.min)]]))[0][0]
 
             if dim.max is not None:
-                new_dim_max = xform.apply(np.array([[float(dim.max)]]))
+                new_dim_max = xform.apply(np.array([[float(dim.max)]]))[0][0]
         else:
             xforms.append(None)
             if dim.min is not None:
                 new_dim_min = float(dim.min)
 
             if dim.max is not None:
                 new_dim_max = float(dim.max)
@@ -416,15 +435,15 @@
             group_gates = _recurse_wsp_sub_populations(
                 group_root_sub_pop_el,
                 None,  # starting at root, so no gate path
                 gating_ns,
                 data_type_ns
             )
 
-        # skip groups with no gates or samples
+        # skip groups with no gates AND no samples
         if len(group_gates) == 0 and len(group_samples) == 0:
             continue
 
         wsp_groups[group_name] = {
             'gates': group_gates,
             'samples': group_samples
         }
@@ -438,14 +457,20 @@
     for sample_el in sample_els:
         transforms_el = sample_el.find('Transformations', ns_map)
         keywords_el = sample_el.find('Keywords', ns_map)
         sample_node_el = sample_el.find('SampleNode', ns_map)
         sample_name = sample_node_el.attrib['name']
         sample_id = sample_node_el.attrib['sampleID']
 
+        # Get the sample DataSet parameters, and form there get the URI from the FCS file
+        dataset_el = sample_el.find('DataSet', ns_map)
+        sample_uri = None
+        if 'uri' in dataset_el.attrib.keys():
+            sample_uri = dataset_el.attrib['uri']
+
         # It appears there is only a single set of xforms per sample, one for each channel.
         # And, the xforms have no IDs. We'll extract it and give it IDs based on ???
         sample_xform_lut = _parse_wsp_transforms(transforms_el, transform_ns, data_type_ns)
 
         # Parse sample keywords. Some keywords may be present in the WSP file that are not
         # in the FCS metadata. FJ allows adding custom keywords for samples.
         sample_keywords_lut = _parse_wsp_keywords(keywords_el)
@@ -467,14 +492,15 @@
                 data_type_ns
             )
 
         # sample gate LUT will store everything we need to convert sample gates,
         # including any custom gates (ones with empty string owning groups).
         wsp_samples[sample_id] = {
             'sample_name': sample_name,
+            'sample_uri': sample_uri,
             'sample_gates': sample_gates,
             'custom_gate_ids': set(),
             'transforms': sample_xform_lut,
             'keywords': sample_keywords_lut,
             'comp': sample_comp
         }
 
@@ -486,18 +512,20 @@
                 # Since there is only a single custom gate per gate name per sample, then we
                 # can create a LUT of custom gates per sample
                 wsp_samples[sample_id]['custom_gate_ids'].add(gate_id)
 
     return wsp_samples
 
 
-def parse_wsp(workspace_file_or_path, ignore_transforms=False):
+def parse_wsp(workspace_file_or_path):
     """
     Converts a FlowJo 10 workspace file (.wsp) into a nested Python dictionary with the following structure:
 
+    .. code-block:: text
+
         wsp_dict = {
             'groups': {
                 group_name: {
                     'samples': sample list,
                     'group_gates': list of common group gates (may not be the complete tree)
                 },
                 ...
@@ -511,16 +539,14 @@
                     'gating_strategy': {gate_id: gate_instance, ...}
                 },
                 ...
             }
         }
 
     :param workspace_file_or_path: A FlowJo .wsp file or file path
-    :param ignore_transforms: Some FlowJo 10 transforms are incompatible with FlowKit. This boolean argument
-        allows parsing workspace files with unsupported transforms without raising errors. Default is False.
     :return: dict
     """
     doc_type, root_xml, gating_ns, data_type_ns, transform_ns = _get_xml_type(workspace_file_or_path)
 
     # first, find 1st level elements:
     #     - Groups -> GroupNode
     #     - SampleList -> Sample
@@ -549,16 +575,15 @@
     # samples in the group have a custom sample gate for that gate node.
     #
     # A few remaining complications:
     #     - The 'All Samples' group: This is a special group containing all
     #       samples. This is potentially problematic b/c multiple group gate
     #       trees can exist among the samples here. It is also possible that
     #       variations in gate trees can occur with custom sample gates, a
-    #       scenario that is even harder to detect. For these reasons, the
-    #       'All Samples' group is ignored for now.
+    #       scenario that is even harder to detect.
     #     - Multi-group samples: If a sample belongs to more than 1 group,
     #       then it can have group gates from more than 1 group. This shows
     #       up in its sample gate tree.
     #     - Transformation LUTs: FlowJo stores gate boundary info in the
     #       untransformed space. Transforms used by a sample are stored with
     #       the sample node in the SampleList, and variations can occur for
     #       the same dimension across different samples. This means that 2
@@ -594,20 +619,17 @@
     # those to make a GatingStrategy for each sample. However, the
     # gates need to be  converted to the transformed space according
     # to the correct specified transforms. This is because FlowJo
     # gates are stored in the untransformed space.
     processed_samples = {}
 
     for sample_id, sample_dict in wsp_samples.items():
-        # First, check the sample's sample_gates. If empty, then the
-        # sample has no gate hierarchy. We'll skip it.
-        if len(sample_dict['sample_gates']) == 0:
-            continue
-
         sample_name = sample_dict['sample_name']
+        sample_uri = sample_dict['sample_uri']
+
         sample_gating_strategy = GatingStrategy()
 
         # Add sample's comp matrix & transforms to GatingStrategy
         if sample_dict['comp'] is not None:
             sample_gating_strategy.add_comp_matrix(sample_dict['comp']['matrix'])
 
         for transform in sample_dict['transforms'].values():
@@ -620,25 +642,25 @@
             sample_gate = sample_gate_dict['gate']
             sample_gate_path = sample_gate_dict['gate_path']
 
             # Convert sample gate and add to gating strategy
             tmp_gate = _convert_wsp_gate(
                 sample_gate,
                 sample_dict['comp'],
-                sample_dict['transforms'],
-                ignore_transforms=ignore_transforms
+                sample_dict['transforms']
             )
             sample_gating_strategy.add_gate(tmp_gate, sample_gate_path, sample_id=sample_name)
 
         processed_sample_data = {
             'keywords': sample_dict['keywords'],
             'compensation': sample_dict['comp'],
             'transforms': sample_dict['transforms'],
             'custom_gate_ids': sample_dict['custom_gate_ids'],
-            'gating_strategy': sample_gating_strategy
+            'gating_strategy': sample_gating_strategy,
+            'sample_uri': sample_uri
         }
 
         processed_samples[sample_name] = processed_sample_data
 
     wsp_dict = {
         'groups': wsp_groups,
         'samples': processed_samples
@@ -648,14 +670,16 @@
 
 
 def extract_wsp_sample_data(workspace_file_or_path):
     """
     Parses a FlowJo 10 workspace file (.wsp) and extracts Sample metadata (keywords)
     into a Python dictionary with the following structure:
 
+    .. code-block:: text
+
         wsp_sample_dict[sample_name] = {
             'keywords': {gate_id: gate_instance, ...},
             'transforms': transforms_list,
             'compensation': matrix
         }
 
     :param workspace_file_or_path: A FlowJo .wsp file or file path
@@ -726,14 +750,21 @@
     elif isinstance(transform, _transforms.LogicleTransform):
         xform_el = etree.SubElement(parent_el, "{%s}logicle" % ns_map['transforms'])
         xform_el.set('{%s}length' % ns_map['transforms'], "256")
         xform_el.set('{%s}T' % ns_map['transforms'], str(transform.param_t))
         xform_el.set('{%s}A' % ns_map['transforms'], str(transform.param_a))
         xform_el.set('{%s}W' % ns_map['transforms'], str(transform.param_w))
         xform_el.set('{%s}M' % ns_map['transforms'], str(transform.param_m))
+    elif isinstance(transform, _wsp_transforms.WSPBiexTransform):
+        xform_el = etree.SubElement(parent_el, "{%s}biex" % ns_map['transforms'])
+        xform_el.set('{%s}length' % ns_map['transforms'], "256")
+        xform_el.set('{%s}maxRange' % ns_map['transforms'], str(transform.max_value))
+        xform_el.set('{%s}neg' % ns_map['transforms'], str(transform.negative))
+        xform_el.set('{%s}width' % ns_map['transforms'], str(transform.width))
+        xform_el.set('{%s}pos' % ns_map['transforms'], str(transform.positive))
     else:
         raise NotImplementedError("Transform type %s is not yet supported" % type(transform))
 
     param_el = etree.SubElement(xform_el, "{%s}parameter" % ns_map['data-type'])
     param_el.set('{%s}name' % ns_map['data-type'], str(parameter_label))
 
 
@@ -816,25 +847,36 @@
             dim_id = comp_prefix + dim.id
 
         dim_el = etree.SubElement(gate_instance_el, "{%s}dimension" % ns_map['gating'])
         fcs_dim_el = etree.SubElement(dim_el, "{%s}fcs-dimension" % ns_map['data-type'])
         fcs_dim_el.set("{%s}name" % ns_map['data-type'], dim_id)
 
         xform_ref = dim.transformation_ref
-
         if xform_ref is not None:
             xform = gating_strategy.get_transform(xform_ref)
-            dim_min = xform.inverse(np.array([[dim.min]]))[0, 0]
-            dim_max = xform.inverse(np.array([[dim.max]]))[0, 0]
         else:
-            dim_min = dim.min
-            dim_max = dim.max
+            xform = None
+
+        # check both min & max, could be an open-ended range gate
+        # only write to doc if present
+        if dim.min is not None:
+            if xform is not None:
+                dim_min = xform.inverse(np.array([[dim.min]]))[0, 0]
+            else:
+                dim_min = dim.min
+
+            dim_el.set('{%s}min' % ns_map['gating'], str(dim_min))
+
+        if dim.max is not None:
+            if xform is not None:
+                dim_max = xform.inverse(np.array([[dim.max]]))[0, 0]
+            else:
+                dim_max = dim.max
 
-        dim_el.set('{%s}min' % ns_map['gating'], str(dim_min))
-        dim_el.set('{%s}max' % ns_map['gating'], str(dim_max))
+            dim_el.set('{%s}max' % ns_map['gating'], str(dim_max))
 
 
 def _add_group_node_to_wsp(parent_el, group_name, sample_id_list):
     group_node_el = etree.SubElement(parent_el, "GroupNode")
     group_node_el.set('name', group_name)
     group_node_el.set('annotation', "")
     group_node_el.set('owningGroup', group_name)
```

### Comparing `FlowKit-1.0.1/flowkit/_utils/xml_utils.py` & `FlowKit-1.1.0/src/flowkit/_utils/xml_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,27 @@
 """
-Utility functions for parsing & exporting gating related XML documents
+Utility functions for parsing GatingML 2.0 documents
 """
 import numpy as np
-from lxml import etree
 import networkx as nx
-from .._resources import gml_schema
+from .xml_common import _get_xml_type, find_attribute_value
 from .._models.dimension import Dimension, RatioDimension, QuadrantDivider
 from .._models.gating_strategy import GatingStrategy
-# noinspection PyProtectedMember
-from .._models.transforms import _transforms, _gml_transforms
+from .._models import transforms
 # noinspection PyProtectedMember
 from .._models.transforms._matrix import Matrix
 # noinspection PyProtectedMember
 from .._models.gates._gml_gates import \
     GMLBooleanGate, \
     GMLEllipsoidGate, \
     GMLQuadrantGate, \
     GMLPolygonGate, \
     GMLRectangleGate
 # noinspection PyProtectedMember
-from .._models.gates._gates import \
-    BooleanGate, \
-    EllipsoidGate, \
-    QuadrantGate, \
-    PolygonGate, \
-    RectangleGate
-from ..exceptions import QuadrantReferenceError
-
+from .._models.gates._gates import BooleanGate, QuadrantGate
 
 # map GatingML gate keys to our GML gate classes
 gate_constructor_lut = {
     'RectangleGate': GMLRectangleGate,
     'PolygonGate': GMLPolygonGate,
     'EllipsoidGate': GMLEllipsoidGate,
     'QuadrantGate': GMLQuadrantGate,
@@ -125,51 +116,14 @@
 
         # Convert GML gates to their superclass & add to gating strategy
         gating_strategy.add_gate(gate.convert_to_parent_class(), gate_path)
 
     return gating_strategy
 
 
-def _get_xml_type(xml_file_or_path):
-    xml_document = etree.parse(xml_file_or_path)
-
-    val = gml_schema.validate(xml_document)
-    root = xml_document.getroot()
-
-    if val:
-        doc_type = 'gatingml'
-    else:
-        # Try parsing as a FlowJo workspace
-        if 'flowJoVersion' in root.attrib:
-            if int(root.attrib['flowJoVersion'].split('.')[0]) >= 10:
-                doc_type = 'flowjo'
-            else:
-                raise ValueError("FlowKit only supports FlowJo workspaces for version 10 or higher.")
-        else:
-            raise ValueError("File is neither GatingML 2.0 compliant nor a FlowJo workspace.")
-
-    gating_ns = None
-    data_type_ns = None
-    transform_ns = None
-
-    # find GatingML target namespace in the map
-    for ns, url in root.nsmap.items():
-        if url == 'http://www.isac-net.org/std/Gating-ML/v2.0/gating':
-            gating_ns = ns
-        elif url == 'http://www.isac-net.org/std/Gating-ML/v2.0/datatypes':
-            data_type_ns = ns
-        elif url == 'http://www.isac-net.org/std/Gating-ML/v2.0/transformations':
-            transform_ns = ns
-
-    if gating_ns is None:
-        raise ValueError("GatingML namespace reference is missing from GatingML file")
-
-    return doc_type, root, gating_ns, data_type_ns, transform_ns
-
-
 def _construct_gates(root_gml, gating_ns, data_type_ns):
     gates_dict = {}
 
     for gate_str, gate_class in gate_constructor_lut.items():
         gt_gates = root_gml.findall(
             ':'.join([gating_ns, gate_str]),
             root_gml.nsmap
@@ -192,96 +146,22 @@
     return gates_dict
 
 
 def _construct_transforms(root_gml, transform_ns, data_type_ns):
     transformations = {}
 
     if transform_ns is not None:
-        # types of transforms include:
-        #   - ratio
-        #   - log10
-        #   - asinh
-        #   - hyperlog
-        #   - linear
-        #   - logicle
+        # GML uses a 'transformation' wrapper tag before we can tell what kind of xform it is
         xform_els = root_gml.findall(
             '%s:transformation' % transform_ns,
             namespaces=root_gml.nsmap
         )
 
         for xform_el in xform_els:
-            xform = None
-
-            # determine type of transformation
-            fratio_els = xform_el.findall(
-                '%s:fratio' % transform_ns,
-                namespaces=root_gml.nsmap
-            )
-
-            if len(fratio_els) > 0:
-                xform = _gml_transforms.RatioGMLTransform(
-                    xform_el,
-                    transform_ns,
-                    data_type_ns
-                )
-
-            flog_els = xform_el.findall(
-                '%s:flog' % transform_ns,
-                namespaces=root_gml.nsmap
-            )
-
-            if len(flog_els) > 0:
-                xform = _gml_transforms.LogGMLTransform(
-                    xform_el,
-                    transform_ns
-                )
-
-            fasinh_els = xform_el.findall(
-                '%s:fasinh' % transform_ns,
-                namespaces=root_gml.nsmap
-            )
-
-            if len(fasinh_els) > 0:
-                xform = _gml_transforms.AsinhGMLTransform(
-                    xform_el,
-                    transform_ns
-                )
-
-            hyperlog_els = xform_el.findall(
-                '%s:hyperlog' % transform_ns,
-                namespaces=root_gml.nsmap
-            )
-
-            if len(hyperlog_els) > 0:
-                xform = _gml_transforms.HyperlogGMLTransform(
-                    xform_el,
-                    transform_ns
-                )
-
-            flin_els = xform_el.findall(
-                '%s:flin' % transform_ns,
-                namespaces=root_gml.nsmap
-            )
-
-            if len(flin_els) > 0:
-                xform = _gml_transforms.LinearGMLTransform(
-                    xform_el,
-                    transform_ns
-                )
-
-            logicle_els = xform_el.findall(
-                '%s:logicle' % transform_ns,
-                namespaces=root_gml.nsmap
-            )
-
-            if len(logicle_els) > 0:
-                xform = _gml_transforms.LogicleGMLTransform(
-                    xform_el,
-                    transform_ns
-                )
+            xform = _parse_transformation_element(xform_el, transform_ns, data_type_ns)
 
             if xform is not None:
                 transformations[xform.id] = xform
 
     return transformations
 
 
@@ -303,43 +183,14 @@
             )
 
             comp_matrices[matrix.id] = matrix
 
     return comp_matrices
 
 
-def find_attribute_value(xml_el, namespace, attribute_name):
-    """
-    Extract the value from an XML element attribute.
-
-    :param xml_el: lxml etree Element
-    :param namespace: string for the XML element's namespace prefix
-    :param attribute_name: attribute string to retrieve the value from
-    :return: value string for the given attribute_name
-    """
-    attribs = xml_el.xpath(
-        '@%s:%s' % (namespace, attribute_name),
-        namespaces=xml_el.nsmap,
-        smart_strings=False
-    )
-    attribs_cnt = len(attribs)
-
-    if attribs_cnt > 1:
-        raise ValueError(
-            "Multiple %s attributes found (line %d)" % (
-                attribute_name, xml_el.sourceline
-            )
-        )
-    elif attribs_cnt == 0:
-        return None
-
-    # return as pure str to save memory (otherwise it's an _ElementUnicodeResult from lxml)
-    return str(attribs[0])
-
-
 def parse_gate_element(
         gate_element,
         gating_namespace,
         data_type_namespace
 ):
     """
     This class parses a GatingML-2.0 compatible gate XML element and extracts the gate ID,
@@ -592,244 +443,199 @@
         matrix.append(matrix_row)
 
     matrix = np.array(matrix)
 
     return Matrix(matrix_id, matrix, detectors, fluorochomes)
 
 
-def _add_matrix_to_gml(root, matrix, ns_map):
-    xform_ml = etree.SubElement(root, "{%s}spectrumMatrix" % ns_map['transforms'])
-    xform_ml.set('{%s}id' % ns_map['transforms'], matrix.id)
-
-    fluoros_ml = etree.SubElement(xform_ml, "{%s}fluorochromes" % ns_map['transforms'])
-
-    for fluoro in matrix.fluorochomes:
-        fluoro_ml = etree.SubElement(fluoros_ml, '{%s}fcs-dimension' % ns_map['data-type'])
-        fluoro_ml.set('{%s}name' % ns_map['data-type'], fluoro)
-
-    detectors_ml = etree.SubElement(xform_ml, "{%s}detectors" % ns_map['transforms'])
-
-    for detector in matrix.detectors:
-        detector_ml = etree.SubElement(detectors_ml, '{%s}fcs-dimension' % ns_map['data-type'])
-        detector_ml.set('{%s}name' % ns_map['data-type'], detector)
-
-    for row in matrix.matrix:
-        row_ml = etree.SubElement(xform_ml, "{%s}spectrum" % ns_map['transforms'])
-        for val in row:
-            coefficient_ml = etree.SubElement(row_ml, "{%s}coefficient" % ns_map['transforms'])
-            coefficient_ml.set('{%s}value' % ns_map['transforms'], str(val))
-
-
-def _add_transform_to_gml(root, transform, ns_map):
-    xform_ml = etree.SubElement(root, "{%s}transformation" % ns_map['transforms'])
-    xform_ml.set('{%s}id' % ns_map['transforms'], transform.id)
-
-    if isinstance(transform, _transforms.RatioTransform):
-        ratio_ml = etree.SubElement(xform_ml, "{%s}fratio" % ns_map['transforms'])
-        ratio_ml.set('{%s}A' % ns_map['transforms'], str(transform.param_a))
-        ratio_ml.set('{%s}B' % ns_map['transforms'], str(transform.param_b))
-        ratio_ml.set('{%s}C' % ns_map['transforms'], str(transform.param_c))
-
-        for dim in transform.dimensions:
-            fcs_dim_ml = etree.SubElement(ratio_ml, '{%s}fcs-dimension' % ns_map['data-type'])
-            fcs_dim_ml.set('{%s}name' % ns_map['data-type'], dim)
-    elif isinstance(transform, _transforms.LogTransform):
-        log_ml = etree.SubElement(xform_ml, "{%s}flog" % ns_map['transforms'])
-        log_ml.set('{%s}T' % ns_map['transforms'], str(transform.param_t))
-        log_ml.set('{%s}M' % ns_map['transforms'], str(transform.param_m))
-    elif isinstance(transform, _transforms.AsinhTransform):
-        asinh_ml = etree.SubElement(xform_ml, "{%s}fasinh" % ns_map['transforms'])
-        asinh_ml.set('{%s}T' % ns_map['transforms'], str(transform.param_t))
-        asinh_ml.set('{%s}M' % ns_map['transforms'], str(transform.param_m))
-        asinh_ml.set('{%s}A' % ns_map['transforms'], str(transform.param_a))
-    elif isinstance(transform, _transforms.LogicleTransform):
-        logicle_ml = etree.SubElement(xform_ml, "{%s}logicle" % ns_map['transforms'])
-        logicle_ml.set('{%s}T' % ns_map['transforms'], str(transform.param_t))
-        logicle_ml.set('{%s}W' % ns_map['transforms'], str(transform.param_w))
-        logicle_ml.set('{%s}M' % ns_map['transforms'], str(transform.param_m))
-        logicle_ml.set('{%s}A' % ns_map['transforms'], str(transform.param_a))
-    elif isinstance(transform, _transforms.HyperlogTransform):
-        hyperlog_ml = etree.SubElement(xform_ml, "{%s}hyperlog" % ns_map['transforms'])
-        hyperlog_ml.set('{%s}T' % ns_map['transforms'], str(transform.param_t))
-        hyperlog_ml.set('{%s}W' % ns_map['transforms'], str(transform.param_w))
-        hyperlog_ml.set('{%s}M' % ns_map['transforms'], str(transform.param_m))
-        hyperlog_ml.set('{%s}A' % ns_map['transforms'], str(transform.param_a))
-    elif isinstance(transform, _transforms.LinearTransform):
-        lin_ml = etree.SubElement(xform_ml, "{%s}flin" % ns_map['transforms'])
-        lin_ml.set('{%s}T' % ns_map['transforms'], str(transform.param_t))
-        lin_ml.set('{%s}A' % ns_map['transforms'], str(transform.param_a))
-
-
-def _add_gate_to_gml(root, gate, ns_map):
-    if isinstance(gate, RectangleGate):
-        gate_ml = etree.SubElement(root, "{%s}RectangleGate" % ns_map['gating'])
-    elif isinstance(gate, PolygonGate):
-        gate_ml = etree.SubElement(root, "{%s}PolygonGate" % ns_map['gating'])
-
-        for v in gate.vertices:
-            vert_ml = etree.SubElement(gate_ml, '{%s}vertex' % ns_map['gating'])
-            for coord in v:
-                coord_ml = etree.SubElement(vert_ml, '{%s}coordinate' % ns_map['gating'])
-                coord_ml.set('{%s}value' % ns_map['data-type'], str(coord))
-    elif isinstance(gate, BooleanGate):
-        gate_ml = etree.SubElement(root, "{%s}BooleanGate" % ns_map['gating'])
-
-        if gate.type == 'and':
-            bool_type_ml = etree.SubElement(gate_ml, '{%s}and' % ns_map['gating'])
-        elif gate.type == 'or':
-            bool_type_ml = etree.SubElement(gate_ml, '{%s}or' % ns_map['gating'])
-        elif gate.type == 'not':
-            bool_type_ml = etree.SubElement(gate_ml, '{%s}not' % ns_map['gating'])
-        else:
-            raise ValueError("Boolean gate type '%s' is not valid" % gate.type)
+def _parse_fratio_element(transform_id, fratio_element, transform_namespace, data_type_namespace):
+    # f ratio transform has 3 parameters: A, B, and C
+    # these are attributes of the 'fratio' element
+    param_a = find_attribute_value(fratio_element, transform_namespace, 'A')
+    param_b = find_attribute_value(fratio_element, transform_namespace, 'B')
+    param_c = find_attribute_value(fratio_element, transform_namespace, 'C')
 
-        for gate_ref in gate.gate_refs:
-            gate_ref_ml = etree.SubElement(bool_type_ml, '{%s}gateReference' % ns_map['gating'])
-            gate_ref_ml.set('{%s}ref' % ns_map['gating'], gate_ref['ref'])
-            if gate_ref['complement']:
-                gate_ref_ml.set('{%s}use-as-complement' % ns_map['gating'], "true")
-
-    elif isinstance(gate, EllipsoidGate):
-        gate_ml = etree.SubElement(root, "{%s}EllipsoidGate" % ns_map['gating'])
-        mean_ml = etree.SubElement(gate_ml, '{%s}mean' % ns_map['gating'])
-        cov_ml = etree.SubElement(gate_ml, '{%s}covarianceMatrix' % ns_map['gating'])
-        dist_square_ml = etree.SubElement(gate_ml, '{%s}distanceSquare' % ns_map['gating'])
-        dist_square_ml.set('{%s}value' % ns_map['data-type'], str(gate.distance_square))
-
-        for c in gate.coordinates:
-            coord_ml = etree.SubElement(mean_ml, '{%s}coordinate' % ns_map['gating'])
-            coord_ml.set('{%s}value' % ns_map['data-type'], str(c))
-
-        for row in gate.covariance_matrix:
-            row_ml = etree.SubElement(cov_ml, '{%s}row' % ns_map['gating'])
-
-            for val in row:
-                entry_ml = etree.SubElement(row_ml, '{%s}entry' % ns_map['gating'])
-                entry_ml.set('{%s}value' % ns_map['data-type'], str(val))
-    elif isinstance(gate, QuadrantGate):
-        gate_ml = etree.SubElement(root, "{%s}QuadrantGate" % ns_map['gating'])
-
-        for q_id, quadrant in gate.quadrants.items():
-            quad_ml = etree.SubElement(gate_ml, '{%s}Quadrant' % ns_map['gating'])
-            quad_ml.set('{%s}id' % ns_map['gating'], q_id)
-
-            for div_ref in quadrant.divider_refs:
-                pos_ml = etree.SubElement(quad_ml, '{%s}position' % ns_map['gating'])
-                pos_ml.set('{%s}divider_ref' % ns_map['gating'], div_ref)
-
-                div_ranges = quadrant.get_divider_range(div_ref)
-                if div_ranges[0] is None:
-                    loc_coord = div_ranges[1] / 2.0
-                elif div_ranges[1] is None:
-                    loc_coord = div_ranges[0] * 2.0
-                else:
-                    loc_coord = np.mean(div_ranges)
-                
-                pos_ml.set('{%s}location' % ns_map['gating'], str(loc_coord))
-    else:
-        raise ValueError("Gate %s is not a valid GatingML 2.0 element" % gate.gate_name)
+    if None in [param_a, param_b, param_c]:
+        raise ValueError(
+            "Ratio transform must provide an 'A', a 'B', and a 'C' "
+            "attribute (line %d)" % fratio_element.sourceline
+        )
 
-    gate_ml.set('{%s}id' % ns_map['gating'], gate.gate_name)
+    # convert from string to float
+    param_a = float(param_a)
+    param_b = float(param_b)
+    param_c = float(param_c)
 
-    for i, dim in enumerate(gate.dimensions):
-        dim_type = 'dim'
+    fcs_dim_els = fratio_element.findall(
+        '%s:fcs-dimension' % data_type_namespace,
+        namespaces=fratio_element.nsmap
+    )
 
-        if isinstance(dim, QuadrantDivider):
-            dim_ml = etree.Element('{%s}divider' % ns_map['gating'])
-            dim_ml.set('{%s}id' % ns_map['gating'], dim.id)
-            dim_type = 'quad'
-        elif isinstance(dim, RatioDimension):
-            dim_ml = etree.Element('{%s}dimension' % ns_map['gating'])
-            dim_type = 'ratio'
-        else:
-            dim_ml = etree.Element('{%s}dimension' % ns_map['gating'])
+    dim_ids = []
 
-        gate_ml.insert(i, dim_ml)
+    for dim_el in fcs_dim_els:
+        dim_id = find_attribute_value(dim_el, data_type_namespace, 'name')
 
-        if dim.compensation_ref is not None:
-            dim_ml.set('{%s}compensation-ref' % ns_map['gating'], dim.compensation_ref)
-        if dim.transformation_ref is not None:
-            dim_ml.set('{%s}transformation-ref' % ns_map['gating'], dim.transformation_ref)
-
-        if dim_type != 'quad':
-            if dim.min is not None:
-                dim_ml.set('{%s}min' % ns_map['gating'], str(dim.min))
-            if dim.max is not None:
-                dim_ml.set('{%s}max' % ns_map['gating'], str(dim.max))
-
-        if dim_type == 'ratio':
-            new_dim_el = etree.SubElement(dim_ml, '{%s}new-dimension' % ns_map['data-type'])
-            new_dim_el.set('{%s}transformation-ref' % ns_map['data-type'], dim.ratio_ref)
-        else:
-            fcs_dim_ml = etree.SubElement(dim_ml, '{%s}fcs-dimension' % ns_map['data-type'])
-            if dim_type == 'dim':
-                fcs_dim_ml.set('{%s}name' % ns_map['data-type'], dim.id)
-            elif dim_type == 'quad':
-                fcs_dim_ml.set('{%s}name' % ns_map['data-type'], dim.dimension_ref)
-                for val in dim.values:
-                    value_ml = etree.SubElement(dim_ml, '{%s}value' % ns_map['gating'])
-                    value_ml.text = str(val)
+        if dim_id is None:
+            raise ValueError(
+                'Dimension name not found (line %d)' % dim_el.sourceline
+            )
+        dim_ids.append(dim_id)
 
-    return gate_ml
+    xform = transforms.RatioTransform(
+        transform_id, dim_ids, param_a, param_b, param_c
+    )
 
+    return xform
 
-def _add_gates_from_gate_dict(gating_strategy, gate_dict, ns_map, parent_ml, sample_id=None):
-    # the gate_dict will have keys 'name' and 'children'. top-level 'name' value is 'root'
-    for child in gate_dict['children']:
-        gate_id = child['name']
 
-        try:
-            gate = gating_strategy.get_gate(gate_id, sample_id=sample_id)
-        except QuadrantReferenceError:
-            # single quadrants will be handled in the owning quadrant gate
-            gate = None
+def _parse_flog_element(transform_id, flog_element, transform_namespace):
+    # f log transform has 2 parameters: T and M
+    # these are attributes of the 'flog' element
+    param_t = find_attribute_value(flog_element, transform_namespace, 'T')
+    param_m = find_attribute_value(flog_element, transform_namespace, 'M')
 
-        if gate is not None:
-            child_ml = _add_gate_to_gml(parent_ml, gate, ns_map)
+    if None in [param_t, param_m]:
+        raise ValueError(
+            "Log transform must provide an 'T' attribute (line %d)" % flog_element.sourceline
+        )
 
-            if gate_dict['name'] != 'root':
-                # this is a recursion, add the parent reference
-                child_ml.set('{%s}parent_id' % ns_map['gating'], gate_dict['name'])
+    # convert string to float
+    param_t = float(param_t)
+    param_m = float(param_m)
 
-        if 'children' in child:  # and not isinstance(gate, QuadrantGate):
-            _add_gates_from_gate_dict(gating_strategy, child, ns_map, parent_ml, sample_id=sample_id)
+    xform = transforms.LogTransform(transform_id, param_t, param_m)
 
+    return xform
 
-def export_gatingml(gating_strategy, file_handle, sample_id=None):
-    """
-    Exports a valid GatingML 2.0 document from given GatingStrategy instance.
-    Specify the sample ID to use that sample's custom gates in the exported
-    file, otherwise the template gates will be exported.
-
-    :param gating_strategy: A GatingStrategy instance
-    :param file_handle: File handle for exported GatingML 2.0 document
-    :param sample_id: an optional text string representing a Sample instance
-    :return: None
-    """
-    ns_g = "http://www.isac-net.org/std/Gating-ML/v2.0/gating"
-    ns_dt = "http://www.isac-net.org/std/Gating-ML/v2.0/datatypes"
-    ns_xform = "http://www.isac-net.org/std/Gating-ML/v2.0/transformations"
-    ns_map = {
-        'gating': ns_g,
-        'data-type': ns_dt,
-        'transforms': ns_xform
-    }
-
-    root = etree.Element('{%s}Gating-ML' % ns_g, nsmap=ns_map)
-
-    # process gating strategy transformations
-    for xform_id, xform in gating_strategy.transformations.items():
-        _add_transform_to_gml(root, xform, ns_map)
-
-    # process gating strategy compensation matrices
-    for matrix_id, matrix in gating_strategy.comp_matrices.items():
-        _add_matrix_to_gml(root, matrix, ns_map)
-
-    # get gate hierarchy as a dictionary
-    gate_dict = gating_strategy.get_gate_hierarchy('dict')
 
-    # recursively convert all gates to GatingML
-    _add_gates_from_gate_dict(gating_strategy, gate_dict, ns_map, root, sample_id=sample_id)
+def _parse_fasinh_element(transform_id, fasinh_element, transform_namespace):
+    # f asinh transform has 3 parameters: T, M, and A
+    # these are attributes of the 'fasinh' element
+    param_t = find_attribute_value(fasinh_element, transform_namespace, 'T')
+    param_m = find_attribute_value(fasinh_element, transform_namespace, 'M')
+    param_a = find_attribute_value(fasinh_element, transform_namespace, 'A')
+
+    if None in [param_t, param_m, param_a]:
+        raise ValueError(
+            "Asinh transform must provide 'T', 'M', and 'A' attributes (line %d)" % fasinh_element.sourceline
+        )
+
+    # convert string to float
+    param_t = float(param_t)
+    param_m = float(param_m)
+    param_a = float(param_a)
+
+    xform = transforms.AsinhTransform(transform_id, param_t, param_m, param_a)
+
+    return xform
+
+
+def _parse_hyperlog_element(transform_id, hyperlog_element, transform_namespace):
+    # hyperlog transform has 4 parameters: T, W, M, and A
+    # these are attributes of the 'hyperlog' element
+    param_t = find_attribute_value(hyperlog_element, transform_namespace, 'T')
+    param_w = find_attribute_value(hyperlog_element, transform_namespace, 'W')
+    param_m = find_attribute_value(hyperlog_element, transform_namespace, 'M')
+    param_a = find_attribute_value(hyperlog_element, transform_namespace, 'A')
+
+    if None in [param_t, param_w, param_m, param_a]:
+        raise ValueError(
+            "Hyperlog transform must provide 'T', 'W', 'M', and 'A' "
+            "attributes (line %d)" % hyperlog_element.sourceline
+        )
+
+    # convert string to float
+    param_t = float(param_t)
+    param_w = float(param_w)
+    param_m = float(param_m)
+    param_a = float(param_a)
+
+    xform = transforms.HyperlogTransform(
+        transform_id, param_t, param_w, param_m, param_a
+    )
+
+    return xform
+
+
+def _parse_flin_element(transform_id, flin_element, transform_namespace):
+    # f linear transform has 2 parameters: T and A
+    # these are attributes of the 'flin' element
+    param_t = find_attribute_value(flin_element, transform_namespace, 'T')
+    param_a = find_attribute_value(flin_element, transform_namespace, 'A')
+
+    if None in [param_t, param_a]:
+        raise ValueError(
+            "Linear transform must provide 'T' and 'A' attributes (line %d)" % flin_element.sourceline
+        )
+
+    # convert string to float
+    param_t = float(param_t)
+    param_a = float(param_a)
+
+    xform = transforms.LinearTransform(transform_id, param_t, param_a)
+
+    return xform
+
+
+def _parse_logicle_element(transform_id, logicle_element, transform_namespace):
+    # logicle transform has 4 parameters: T, W, M, and A
+    # these are attributes of the 'logicle' element
+    param_t = find_attribute_value(logicle_element, transform_namespace, 'T')
+    param_w = find_attribute_value(logicle_element, transform_namespace, 'W')
+    param_m = find_attribute_value(logicle_element, transform_namespace, 'M')
+    param_a = find_attribute_value(logicle_element, transform_namespace, 'A')
+
+    if None in [param_t, param_w, param_m, param_a]:
+        raise ValueError(
+            "Logicle transform must provide 'T', 'W', 'M', and 'A' "
+            "attributes (line %d)" % logicle_element.sourceline
+        )
+
+    # convert string to float
+    param_t = float(param_t)
+    param_w = float(param_w)
+    param_m = float(param_m)
+    param_a = float(param_a)
+
+    xform = transforms.LogicleTransform(
+        transform_id, param_t, param_w, param_m, param_a
+    )
+
+    return xform
+
+
+def _parse_transformation_element(transformation_element, transform_namespace, data_type_namespace):
+    xform = None
+
+    # 'transformation' wrapper tag has the transform ID, so grab that & then parse
+    # the child tags. There should only be 1 child that will reveal the xform type.
+    xform_id = find_attribute_value(transformation_element, transform_namespace, 'id')
+    xform_child_els = transformation_element.getchildren()
+
+    # there should only ever be 1 child tag, but we'll loop
+    for xform_child_el in xform_child_els:
+        # Transform type tags include:
+        #   - fratio
+        #   - flog
+        #   - fasinh
+        #   - hyperlog
+        #   - flin
+        #   - logicle
+        xform_type = xform_child_el.tag.partition('}')[-1]
 
-    et = etree.ElementTree(root)
+        if xform_type == 'fratio':
+            xform = _parse_fratio_element(
+                xform_id, xform_child_el, transform_namespace, data_type_namespace
+            )
+        elif xform_type == 'flog':
+            xform = _parse_flog_element(xform_id, xform_child_el, transform_namespace)
+        elif xform_type == 'fasinh':
+            xform = _parse_fasinh_element(xform_id, xform_child_el, transform_namespace)
+        elif xform_type == 'hyperlog':
+            xform = _parse_hyperlog_element(xform_id, xform_child_el, transform_namespace)
+        elif xform_type == 'flin':
+            xform = _parse_flin_element(xform_id, xform_child_el, transform_namespace)
+        elif xform_type == 'logicle':
+            xform = _parse_logicle_element(xform_id, xform_child_el, transform_namespace)
 
-    et.write(file_handle, encoding="utf-8", xml_declaration=True, pretty_print=True)
+    return xform
```

### Comparing `FlowKit-1.0.1/flowkit/exceptions.py` & `FlowKit-1.1.0/src/flowkit/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 flowkit.exceptions
 ~~~~~~~~~~~~~~~~~~
 This module contains the set of FlowKit exceptions.
 """
 # import FlowIO exceptions
-from flowio.exceptions import FCSParsingError, DataOffsetDiscrepancyError
+from flowio.exceptions import FCSParsingError, DataOffsetDiscrepancyError  # noqa
 
 
 class FlowKitWarning(Warning):
     """A generic FlowKit warning"""
     pass
```

### Comparing `FlowKit-1.0.1/setup.py` & `FlowKit-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 """
 Setup script for the FlowKit package
 """
 from setuptools import setup, find_packages
 
 # read in version string
-VERSION_FILE = 'flowkit/_version.py'
+VERSION_FILE = 'src/flowkit/_version.py'
 __version__ = None  # to avoid inspection warning and check if __version__ was loaded
 exec(open(VERSION_FILE).read())
 
 if __version__ is None:
     raise RuntimeError("__version__ string not found in file %s" % VERSION_FILE)
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 reqs = [
-    'anytree>=2.6',
-    'bokeh>=2.4,<3',
-    'flowio==1.1.1',
-    'flowutils>=1,<1.1',
-    'lxml>=4.7',
-    'matplotlib>=3.5',
-    'networkx>=2.3',
-    'numpy>=1.20',
-    'pandas>=1.2,<2',
+    'anytree>=2.9',
+    'bokeh>=3.1',
+    'contourpy>=1.1.0',
+    'flowio>=1.3.0,<1.4',
+    'flowutils>=1.1.0,<1.2',
+    'lxml>=4.9',
+    'networkx>=3.1',
+    'numpy>=1.22,<2',
+    'pandas>=2.0',
     'psutil>=5.8',
-    'scipy>=1.6',
-    'seaborn>=0.11,<0.12'
+    'scipy>=1.8'
 ]
 
 setup(
     name='FlowKit',
-    version=__version__,
-    packages=find_packages(exclude=["flowkit/tests/"]),
+    version=__version__,  # noqa PyTypeChecker
+    packages=find_packages(where='src'),
+    package_dir={'': 'src'},
     package_data={'': ['_resources/*.xsd']},
     include_package_data=True,
     description='Flow Cytometry Toolkit',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Scott White",
     license='BSD',
     url="https://github.com/whitews/flowkit",
     ext_modules=[],
     install_requires=reqs,
     classifiers=[
+        'Programming Language :: Python :: 3.12',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.7'
+        'Programming Language :: Python :: 3.8'
     ]
 )
```

