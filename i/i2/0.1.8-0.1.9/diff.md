# Comparing `tmp/i2-0.1.8.tar.gz` & `tmp/i2-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i2-0.1.8.tar", last modified: Sun Dec 31 09:38:01 2023, max compression
+gzip compressed data, was "i2-0.1.9.tar", last modified: Thu Mar 14 12:22:50 2024, max compression
```

## Comparing `i2-0.1.8.tar` & `i2-0.1.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 09:38:01.054321 i2-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-12-31 09:37:35.000000 i2-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2023-12-31 09:38:01.054321 i2-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2023-12-31 09:37:35.000000 i2-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 09:38:01.050321 i2-0.1.8/i2/
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2023-12-31 09:37:35.000000 i2-0.1.8/i2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2023-12-31 09:37:35.000000 i2-0.1.8/i2/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    15393 2023-12-31 09:37:35.000000 i2-0.1.8/i2/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2023-12-31 09:37:35.000000 i2-0.1.8/i2/chain_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    54497 2023-12-31 09:37:35.000000 i2-0.1.8/i2/deco.py
--rw-r--r--   0 runner    (1001) docker     (127)    11887 2023-12-31 09:37:35.000000 i2-0.1.8/i2/doc_mint.py
--rw-r--r--   0 runner    (1001) docker     (127)     6786 2023-12-31 09:37:35.000000 i2-0.1.8/i2/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 09:38:01.050321 i2-0.1.8/i2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-31 09:37:35.000000 i2-0.1.8/i2/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2023-12-31 09:37:35.000000 i2-0.1.8/i2/examples/signature_calculus.py
--rw-r--r--   0 runner    (1001) docker     (127)    22321 2023-12-31 09:37:35.000000 i2-0.1.8/i2/footprints.py
--rw-r--r--   0 runner    (1001) docker     (127)     9546 2023-12-31 09:37:35.000000 i2-0.1.8/i2/io_trans.py
--rw-r--r--   0 runner    (1001) docker     (127)     9073 2023-12-31 09:37:35.000000 i2-0.1.8/i2/itypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    23008 2023-12-31 09:37:35.000000 i2-0.1.8/i2/key_path.py
--rw-r--r--   0 runner    (1001) docker     (127)    31885 2023-12-31 09:37:35.000000 i2-0.1.8/i2/multi_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    25805 2023-12-31 09:37:35.000000 i2-0.1.8/i2/routing_forest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 09:38:01.050321 i2-0.1.8/i2/scrap/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-31 09:37:35.000000 i2-0.1.8/i2/scrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8279 2023-12-31 09:37:35.000000 i2-0.1.8/i2/scrap/scrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2023-12-31 09:37:35.000000 i2-0.1.8/i2/scrap/scrap_ch_variadics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2023-12-31 09:37:35.000000 i2-0.1.8/i2/scrap/scrap_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4183 2023-12-31 09:37:35.000000 i2-0.1.8/i2/scrap/signature_bops.py
--rw-r--r--   0 runner    (1001) docker     (127)     7379 2023-12-31 09:37:35.000000 i2-0.1.8/i2/scrap/simple_pymint.py
--rw-r--r--   0 runner    (1001) docker     (127)     8950 2023-12-31 09:37:35.000000 i2-0.1.8/i2/scrap/switch_case_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)   175415 2023-12-31 09:37:35.000000 i2-0.1.8/i2/signatures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 09:38:01.054321 i2-0.1.8/i2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-31 09:37:35.000000 i2-0.1.8/i2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2023-12-31 09:37:35.000000 i2-0.1.8/i2/tests/footprints_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5417 2023-12-31 09:37:35.000000 i2-0.1.8/i2/tests/objects_for_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)    80573 2023-12-31 09:37:35.000000 i2-0.1.8/i2/tests/signatures_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2023-12-31 09:37:35.000000 i2-0.1.8/i2/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9220 2023-12-31 09:37:35.000000 i2-0.1.8/i2/tests/test_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    24874 2023-12-31 09:37:35.000000 i2-0.1.8/i2/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    40553 2023-12-31 09:37:35.000000 i2-0.1.8/i2/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    81514 2023-12-31 09:37:35.000000 i2-0.1.8/i2/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 09:38:01.050321 i2-0.1.8/i2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2023-12-31 09:38:01.000000 i2-0.1.8/i2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      814 2023-12-31 09:38:01.000000 i2-0.1.8/i2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-31 09:38:01.000000 i2-0.1.8/i2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-31 09:38:01.000000 i2-0.1.8/i2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        3 2023-12-31 09:38:01.000000 i2-0.1.8/i2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      549 2023-12-31 09:38:01.054321 i2-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-12-31 09:37:35.000000 i2-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 12:22:50.646646 i2-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-14 12:22:21.000000 i2-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-03-14 12:22:50.646646 i2-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-03-14 12:22:21.000000 i2-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 12:22:50.642646 i2-0.1.9/i2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-03-14 12:22:21.000000 i2-0.1.9/i2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-03-14 12:22:21.000000 i2-0.1.9/i2/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15393 2024-03-14 12:22:21.000000 i2-0.1.9/i2/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-03-14 12:22:21.000000 i2-0.1.9/i2/chain_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54497 2024-03-14 12:22:21.000000 i2-0.1.9/i2/deco.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11887 2024-03-14 12:22:21.000000 i2-0.1.9/i2/doc_mint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6786 2024-03-14 12:22:21.000000 i2-0.1.9/i2/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 12:22:50.646646 i2-0.1.9/i2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-14 12:22:21.000000 i2-0.1.9/i2/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-03-14 12:22:21.000000 i2-0.1.9/i2/examples/signature_calculus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22321 2024-03-14 12:22:21.000000 i2-0.1.9/i2/footprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-03-14 12:22:21.000000 i2-0.1.9/i2/io_trans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-03-14 12:22:21.000000 i2-0.1.9/i2/itypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23008 2024-03-14 12:22:21.000000 i2-0.1.9/i2/key_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31885 2024-03-14 12:22:21.000000 i2-0.1.9/i2/multi_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25805 2024-03-14 12:22:21.000000 i2-0.1.9/i2/routing_forest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 12:22:50.646646 i2-0.1.9/i2/scrap/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-14 12:22:21.000000 i2-0.1.9/i2/scrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-03-14 12:22:21.000000 i2-0.1.9/i2/scrap/scrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-03-14 12:22:21.000000 i2-0.1.9/i2/scrap/scrap_ch_variadics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-03-14 12:22:21.000000 i2-0.1.9/i2/scrap/scrap_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-03-14 12:22:21.000000 i2-0.1.9/i2/scrap/signature_bops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-03-14 12:22:21.000000 i2-0.1.9/i2/scrap/simple_pymint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-03-14 12:22:21.000000 i2-0.1.9/i2/scrap/switch_case_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)   175415 2024-03-14 12:22:21.000000 i2-0.1.9/i2/signatures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 12:22:50.646646 i2-0.1.9/i2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-14 12:22:21.000000 i2-0.1.9/i2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-03-14 12:22:21.000000 i2-0.1.9/i2/tests/footprints_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-03-14 12:22:21.000000 i2-0.1.9/i2/tests/objects_for_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80573 2024-03-14 12:22:21.000000 i2-0.1.9/i2/tests/signatures_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-03-14 12:22:21.000000 i2-0.1.9/i2/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9220 2024-03-14 12:22:21.000000 i2-0.1.9/i2/tests/test_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24874 2024-03-14 12:22:21.000000 i2-0.1.9/i2/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41417 2024-03-14 12:22:30.000000 i2-0.1.9/i2/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81514 2024-03-14 12:22:21.000000 i2-0.1.9/i2/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 12:22:50.646646 i2-0.1.9/i2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-03-14 12:22:50.000000 i2-0.1.9/i2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-03-14 12:22:50.000000 i2-0.1.9/i2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 12:22:50.000000 i2-0.1.9/i2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 12:22:50.000000 i2-0.1.9/i2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-03-14 12:22:50.000000 i2-0.1.9/i2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-14 12:22:50.646646 i2-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-14 12:22:21.000000 i2-0.1.9/setup.py
```

### Comparing `i2-0.1.8/LICENSE` & `i2-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/PKG-INFO` & `i2-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2
-Version: 0.1.8
+Version: 0.1.9
 Summary: Creating
 Home-page: https://github.com/i2mint/i2
 Author: Otosense
 License: Apache Software License
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `i2-0.1.8/README.md` & `i2-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2/__init__.py` & `i2-0.1.9/i2/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Meta-programming tools to build declarative frameworks"""
+
 from i2.deco import (
     FuncFactory,
     preprocess,
     postprocess,
     preprocess_arguments,
     input_output_decorator,
     wrap_class_methods_input_and_output,
@@ -45,14 +46,15 @@
     ch_names,
     func_to_method_func,
     bind_funcs_object_attrs,
     kwargs_trans,
 )
 
 from i2.util import (
+    Namespace,
     copy_func,
     get_app_data_folder,
     LiteralVal,
     path_extractor,
     get_function_body,
     lazyprop,
     frozendict,
```

### Comparing `i2-0.1.8/i2/_deprecated.py` & `i2-0.1.9/i2/_deprecated.py`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2/base.py` & `i2-0.1.9/i2/base.py`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2/chain_map.py` & `i2-0.1.9/i2/chain_map.py`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2/deco.py` & `i2-0.1.9/i2/deco.py`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2/doc_mint.py` & `i2-0.1.9/i2/doc_mint.py`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2/errors.py` & `i2-0.1.9/i2/errors.py`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2/examples/signature_calculus.py` & `i2-0.1.9/i2/examples/signature_calculus.py`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2/footprints.py` & `i2-0.1.9/i2/footprints.py`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2/io_trans.py` & `i2-0.1.9/i2/io_trans.py`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2/itypes.py` & `i2-0.1.9/i2/itypes.py`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2/key_path.py` & `i2-0.1.9/i2/key_path.py`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2/multi_object.py` & `i2-0.1.9/i2/multi_object.py`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2/routing_forest.py` & `i2-0.1.9/i2/routing_forest.py`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2/scrap/scrap.py` & `i2-0.1.9/i2/scrap/scrap.py`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2/scrap/scrap_ch_variadics.py` & `i2-0.1.9/i2/scrap/scrap_ch_variadics.py`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2/scrap/scrap_kwargs.py` & `i2-0.1.9/i2/scrap/scrap_kwargs.py`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2/scrap/signature_bops.py` & `i2-0.1.9/i2/scrap/signature_bops.py`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2/scrap/simple_pymint.py` & `i2-0.1.9/i2/scrap/simple_pymint.py`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2/scrap/switch_case_tree.py` & `i2-0.1.9/i2/scrap/switch_case_tree.py`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2/signatures.py` & `i2-0.1.9/i2/signatures.py`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2/tests/footprints_test.py` & `i2-0.1.9/i2/tests/footprints_test.py`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2/tests/objects_for_testing.py` & `i2-0.1.9/i2/tests/objects_for_testing.py`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2/tests/signatures_test.py` & `i2-0.1.9/i2/tests/signatures_test.py`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2/tests/test_util.py` & `i2-0.1.9/i2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2/tests/test_wrapper.py` & `i2-0.1.9/i2/tests/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2/tests/util.py` & `i2-0.1.9/i2/tests/util.py`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2/util.py` & `i2-0.1.9/i2/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Misc util objects"""
+
 from operator import attrgetter, itemgetter
 import inspect
 import re
 import os
 import itertools
 import sys
 from functools import partial, wraps
 import types
+from types import SimpleNamespace
 from typing import (
     Mapping,
     Callable,
     Any,
     MutableMapping,
     Union,
     Optional,
@@ -19,19 +21,70 @@
 )
 import contextlib
 import io
 
 T = TypeVar('T')
 
 
+class Namespace(SimpleNamespace, MutableMapping):
+    """
+    A namespace that is also a mutable mapping.
+
+    Example:
+
+    >>> s = Namespace(apple=1, apps=2)
+
+    Get your values via attributes:
+
+    >>> s.apple
+    1
+
+    Get your values via keys:
+
+    >>> s['apple']
+    1
+
+    Do the stuff Mappings do:
+
+    >>> list(s)
+    ['apple', 'apps']
+    >>> 'apps' in s
+    True
+
+    Or even MutableMappings do:
+
+    >>> s['appartment'] = 3
+    >>> s
+    Namespace(apple=1, apps=2, appartment=3)
+    >>> s.appartment
+    3
+
+    """
+
+    def __getitem__(self, k):
+        return getattr(self, k)
+
+    def __setitem__(self, k, v):
+        setattr(self, k, v)
+
+    def __delitem__(self, k):
+        delattr(self, k)
+
+    def __iter__(self):
+        return iter(self.__dict__)
+
+    def __len__(self):
+        return len(self.__dict__)
+
+
 @contextlib.contextmanager
 def FileLikeObject(file, *, io_cls=io.BytesIO, open_mode='rb'):
     """Context manager for file-like objects.
 
-    The purpose of this context manager is to be able to ensure we have a file-like 
+    The purpose of this context manager is to be able to ensure we have a file-like
     object interface to work with, regardless of whether we are given a file path,
     bytes of a file, or an open file pointer.
 
     Args:
         file (str, bytes, io.IOBase): The file path, bytes of a file, or an open file pointer.
 
     Yields:
```

### Comparing `i2-0.1.8/i2/wrapper.py` & `i2-0.1.9/i2/wrapper.py`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/i2.egg-info/PKG-INFO` & `i2-0.1.9/i2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2
-Version: 0.1.8
+Version: 0.1.9
 Summary: Creating
 Home-page: https://github.com/i2mint/i2
 Author: Otosense
 License: Apache Software License
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `i2-0.1.8/i2.egg-info/SOURCES.txt` & `i2-0.1.9/i2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `i2-0.1.8/setup.cfg` & `i2-0.1.9/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = i2
-version = 0.1.8
+version = 0.1.9
 url = https://github.com/i2mint/i2
 platforms = any
 description_file = README.md
 root_url = https://github.com/i2mint
 description = 
 	Creating
 	manipulating
```

