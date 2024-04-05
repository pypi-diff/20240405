# Comparing `tmp/valor-client-0.20.0.tar.gz` & `tmp/valor-client-0.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valor-client-0.20.0.tar", last modified: Tue Apr  2 01:02:01 2024, max compression
+gzip compressed data, was "valor-client-0.20.1.tar", last modified: Fri Apr  5 21:44:28 2024, max compression
```

## Comparing `valor-client-0.20.0.tar` & `valor-client-0.20.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:02:01.599599 valor-client-0.20.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-02 01:01:56.000000 valor-client-0.20.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-02 01:02:01.599599 valor-client-0.20.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-02 01:01:56.000000 valor-client-0.20.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 01:02:01.599599 valor-client-0.20.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-02 01:01:56.000000 valor-client-0.20.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:02:01.595599 valor-client-0.20.0/unit-tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:02:01.595599 valor-client-0.20.0/unit-tests/coretypes/
--rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/coretypes/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/coretypes/test_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/coretypes/test_filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:02:01.595599 valor-client-0.20.0/unit-tests/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/schemas/test_evaluation_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/schemas/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/schemas/test_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/schemas/test_label.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:02:01.595599 valor-client-0.20.0/unit-tests/symbolic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:02:01.595599 valor-client-0.20.0/unit-tests/symbolic/collections/
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/symbolic/collections/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/symbolic/collections/test_static_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/symbolic/collections/test_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/symbolic/test_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:02:01.595599 valor-client-0.20.0/unit-tests/symbolic/types/
--rw-r--r--   0 runner    (1001) docker     (127)    14686 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/symbolic/types/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    28256 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/symbolic/types/test_symbolic_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/test_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:02:01.599599 valor-client-0.20.0/valor/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29003 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    53715 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/coretypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/metatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:02:01.599599 valor-client-0.20.0/valor/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/schemas/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/schemas/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14596 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/schemas/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:02:01.599599 valor-client-0.20.0/valor/schemas/symbolic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/schemas/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25442 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/schemas/symbolic/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/schemas/symbolic/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    46702 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/schemas/symbolic/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/type_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10632 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:02:01.599599 valor-client-0.20.0/valor_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-02 01:02:01.000000 valor-client-0.20.0/valor_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-02 01:02:01.000000 valor-client-0.20.0/valor_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 01:02:01.000000 valor-client-0.20.0/valor_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-02 01:02:01.000000 valor-client-0.20.0/valor_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 01:02:01.000000 valor-client-0.20.0/valor_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:44:28.513570 valor-client-0.20.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-05 21:44:23.000000 valor-client-0.20.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-05 21:44:28.513570 valor-client-0.20.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-05 21:44:23.000000 valor-client-0.20.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 21:44:28.513570 valor-client-0.20.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-05 21:44:23.000000 valor-client-0.20.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:44:28.505570 valor-client-0.20.1/unit-tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:44:28.505570 valor-client-0.20.1/unit-tests/coretypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/coretypes/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/coretypes/test_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/coretypes/test_filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:44:28.505570 valor-client-0.20.1/unit-tests/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/schemas/test_evaluation_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/schemas/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/schemas/test_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/schemas/test_label.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:44:28.505570 valor-client-0.20.1/unit-tests/symbolic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:44:28.505570 valor-client-0.20.1/unit-tests/symbolic/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/symbolic/collections/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/symbolic/collections/test_static_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/symbolic/collections/test_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/symbolic/test_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:44:28.509570 valor-client-0.20.1/unit-tests/symbolic/types/
+-rw-r--r--   0 runner    (1001) docker     (127)    14686 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/symbolic/types/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28256 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/symbolic/types/test_symbolic_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:44:28.509570 valor-client-0.20.1/valor/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29003 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53715 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/coretypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/metatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:44:28.509570 valor-client-0.20.1/valor/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/schemas/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/schemas/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14596 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/schemas/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:44:28.509570 valor-client-0.20.1/valor/schemas/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/schemas/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25442 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/schemas/symbolic/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/schemas/symbolic/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46702 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/schemas/symbolic/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/type_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10632 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:44:28.513570 valor-client-0.20.1/valor_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-05 21:44:28.000000 valor-client-0.20.1/valor_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-05 21:44:28.000000 valor-client-0.20.1/valor_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 21:44:28.000000 valor-client-0.20.1/valor_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-05 21:44:28.000000 valor-client-0.20.1/valor_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 21:44:28.000000 valor-client-0.20.1/valor_client.egg-info/top_level.txt
```

### Comparing `valor-client-0.20.0/LICENSE` & `valor-client-0.20.1/LICENSE`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/PKG-INFO` & `valor-client-0.20.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valor-client
-Version: 0.20.0
+Version: 0.20.1
 Summary: Python client for the Valor evaluation store
 License: MIT License
         
         Copyright (c) 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `valor-client-0.20.0/pyproject.toml` & `valor-client-0.20.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/unit-tests/conftest.py` & `valor-client-0.20.1/unit-tests/conftest.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/unit-tests/coretypes/test_core.py` & `valor-client-0.20.1/unit-tests/coretypes/test_core.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/unit-tests/coretypes/test_evaluation.py` & `valor-client-0.20.1/unit-tests/coretypes/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/unit-tests/coretypes/test_filtering.py` & `valor-client-0.20.1/unit-tests/coretypes/test_filtering.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/unit-tests/schemas/test_filters.py` & `valor-client-0.20.1/unit-tests/schemas/test_filters.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/unit-tests/schemas/test_geojson.py` & `valor-client-0.20.1/unit-tests/schemas/test_geojson.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/unit-tests/schemas/test_label.py` & `valor-client-0.20.1/unit-tests/schemas/test_label.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/unit-tests/symbolic/collections/test_dictionary.py` & `valor-client-0.20.1/unit-tests/symbolic/collections/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/unit-tests/symbolic/collections/test_static_collection.py` & `valor-client-0.20.1/unit-tests/symbolic/collections/test_static_collection.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/unit-tests/symbolic/collections/test_structures.py` & `valor-client-0.20.1/unit-tests/symbolic/collections/test_structures.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/unit-tests/symbolic/test_operators.py` & `valor-client-0.20.1/unit-tests/symbolic/test_operators.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/unit-tests/symbolic/types/test_schemas.py` & `valor-client-0.20.1/unit-tests/symbolic/types/test_schemas.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/unit-tests/symbolic/types/test_symbolic_types.py` & `valor-client-0.20.1/unit-tests/symbolic/types/test_symbolic_types.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/unit-tests/test_client.py` & `valor-client-0.20.1/unit-tests/test_client.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/unit-tests/test_viz.py` & `valor-client-0.20.1/unit-tests/test_viz.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/valor/__init__.py` & `valor-client-0.20.1/valor/__init__.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/valor/client.py` & `valor-client-0.20.1/valor/client.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/valor/coretypes.py` & `valor-client-0.20.1/valor/coretypes.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/valor/enums.py` & `valor-client-0.20.1/valor/enums.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/valor/exceptions.py` & `valor-client-0.20.1/valor/exceptions.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/valor/metatypes.py` & `valor-client-0.20.1/valor/metatypes.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/valor/schemas/__init__.py` & `valor-client-0.20.1/valor/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/valor/schemas/compatibility.py` & `valor-client-0.20.1/valor/schemas/compatibility.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/valor/schemas/evaluation.py` & `valor-client-0.20.1/valor/schemas/evaluation.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/valor/schemas/filters.py` & `valor-client-0.20.1/valor/schemas/filters.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/valor/schemas/symbolic/collections.py` & `valor-client-0.20.1/valor/schemas/symbolic/collections.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/valor/schemas/symbolic/operators.py` & `valor-client-0.20.1/valor/schemas/symbolic/operators.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/valor/schemas/symbolic/types.py` & `valor-client-0.20.1/valor/schemas/symbolic/types.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/valor/type_checks.py` & `valor-client-0.20.1/valor/type_checks.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/valor/viz.py` & `valor-client-0.20.1/valor/viz.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.0/valor_client.egg-info/PKG-INFO` & `valor-client-0.20.1/valor_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valor-client
-Version: 0.20.0
+Version: 0.20.1
 Summary: Python client for the Valor evaluation store
 License: MIT License
         
         Copyright (c) 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `valor-client-0.20.0/valor_client.egg-info/SOURCES.txt` & `valor-client-0.20.1/valor_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

