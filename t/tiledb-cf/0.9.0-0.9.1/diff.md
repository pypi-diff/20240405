# Comparing `tmp/tiledb-cf-0.9.0.tar.gz` & `tmp/tiledb-cf-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiledb-cf-0.9.0.tar", last modified: Tue Sep 12 14:27:56 2023, max compression
+gzip compressed data, was "tiledb-cf-0.9.1.tar", last modified: Fri Apr  5 19:56:01 2024, max compression
```

## Comparing `tiledb-cf-0.9.0.tar` & `tiledb-cf-0.9.1.tar`

### file list

```diff
@@ -1,44 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 14:27:56.977977 tiledb-cf-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2023-09-12 14:27:56.977977 tiledb-cf-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      511 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2023-09-12 14:27:56.977977 tiledb-cf-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 14:27:56.969976 tiledb-cf-0.9.0/tiledb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 14:27:56.969976 tiledb-cf-0.9.0/tiledb/cf/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/tiledb/cf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/tiledb/cf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/tiledb/cf/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/tiledb/cf/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 14:27:56.969976 tiledb-cf-0.9.0/tiledb/cf/core/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/tiledb/cf/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42573 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/tiledb/cf/core/_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/tiledb/cf/core/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/tiledb/cf/core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 14:27:56.973976 tiledb-cf-0.9.0/tiledb/cf/netcdf_engine/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/tiledb/cf/netcdf_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13308 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/tiledb/cf/netcdf_engine/_array_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/tiledb/cf/netcdf_engine/_attr_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)    18969 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/tiledb/cf/netcdf_engine/_dim_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6634 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/tiledb/cf/netcdf_engine/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/tiledb/cf/netcdf_engine/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    40606 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/tiledb/cf/netcdf_engine/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 14:27:56.973976 tiledb-cf-0.9.0/tiledb/cf/xarray_engine/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/tiledb/cf/xarray_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8006 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/tiledb/cf/xarray_engine/_array_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8758 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/tiledb/cf/xarray_engine/_backend_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/tiledb/cf/xarray_engine/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    17950 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/tiledb/cf/xarray_engine/_deprecated_backend_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     7816 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/tiledb/cf/xarray_engine/_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)    14789 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/tiledb/cf/xarray_engine/_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8498 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/tiledb/cf/xarray_engine/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7195 2023-09-12 14:27:50.000000 tiledb-cf-0.9.0/tiledb/cf/xarray_engine/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 14:27:56.973976 tiledb-cf-0.9.0/tiledb_cf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2023-09-12 14:27:56.000000 tiledb-cf-0.9.0/tiledb_cf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-09-12 14:27:56.000000 tiledb-cf-0.9.0/tiledb_cf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-12 14:27:56.000000 tiledb-cf-0.9.0/tiledb_cf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-09-12 14:27:56.000000 tiledb-cf-0.9.0/tiledb_cf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-12 14:27:56.000000 tiledb-cf-0.9.0/tiledb_cf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      255 2023-09-12 14:27:56.000000 tiledb-cf-0.9.0/tiledb_cf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-09-12 14:27:56.000000 tiledb-cf-0.9.0/tiledb_cf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:56:01.421621 tiledb-cf-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-05 19:56:01.421621 tiledb-cf-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-05 19:56:01.421621 tiledb-cf-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:56:01.409621 tiledb-cf-0.9.1/tiledb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:56:01.413621 tiledb-cf-0.9.1/tiledb/cf/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:56:01.413621 tiledb-cf-0.9.1/tiledb/cf/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34437 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/core/_array_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/core/_attr_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21103 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/core/_dataspace_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/core/_dim_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11073 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/core/_fragment_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/core/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/core/_shared_dim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/core/source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:56:01.417621 tiledb-cf-0.9.1/tiledb/cf/netcdf_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/netcdf_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14972 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/netcdf_engine/_array_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7889 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/netcdf_engine/_attr_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22824 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/netcdf_engine/_dim_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/netcdf_engine/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/netcdf_engine/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40901 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/netcdf_engine/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:56:01.417621 tiledb-cf-0.9.1/tiledb/cf/xarray_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/xarray_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/xarray_engine/_array_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/xarray_engine/_backend_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/xarray_engine/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18218 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/xarray_engine/_deprecated_backend_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/xarray_engine/_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15141 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/xarray_engine/_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8560 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/xarray_engine/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7347 2024-04-05 19:55:58.000000 tiledb-cf-0.9.1/tiledb/cf/xarray_engine/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:56:01.417621 tiledb-cf-0.9.1/tiledb_cf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-05 19:56:01.000000 tiledb-cf-0.9.1/tiledb_cf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-05 19:56:01.000000 tiledb-cf-0.9.1/tiledb_cf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:56:01.000000 tiledb-cf-0.9.1/tiledb_cf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-05 19:56:01.000000 tiledb-cf-0.9.1/tiledb_cf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:56:01.000000 tiledb-cf-0.9.1/tiledb_cf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-05 19:56:01.000000 tiledb-cf-0.9.1/tiledb_cf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 19:56:01.000000 tiledb-cf-0.9.1/tiledb_cf.egg-info/top_level.txt
```

### Comparing `tiledb-cf-0.9.0/LICENSE` & `tiledb-cf-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tiledb-cf-0.9.0/README.md` & `tiledb-cf-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `tiledb-cf-0.9.0/setup.cfg` & `tiledb-cf-0.9.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tiledb-cf
-version = 0.9.0
+version = 0.9.1
 description = TileDB Python library for supporting Climate and Forecast datasets.
 author = TileDB, Inc.
 author_email = help@tiledb.io
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 keywords = tiledb, climate, forecast, netcdf
@@ -34,14 +34,15 @@
 	tiledb.cf.xarray_engine
 python_requires = >=3.7
 install_requires = 
 	numpy >= 1.16.5
 	setuptools >= 40.4
 	tiledb >= 0.21.2
 	click >= 0.7.0
+	typing-extensions >= 4.0.0
 
 [options.extras_require]
 netCDF4 = netCDF4
 xarray = xarray >= 0.18.0
 parallel = dask[complete]
 complete = 
 	%(netCDF4)s
```

### Comparing `tiledb-cf-0.9.0/tiledb/cf/__init__.py` & `tiledb-cf-0.9.1/tiledb/cf/__init__.py`

 * *Files identical despite different names*

### Comparing `tiledb-cf-0.9.0/tiledb/cf/_utils.py` & `tiledb-cf-0.9.1/tiledb/cf/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,39 +22,49 @@
 
 
 def get_array_key(
     key: Optional[Union[Dict[str, str], str]], array_name
 ) -> Optional[str]:
     """Returns a key for the array with name ``array_name``.
 
-    Parameters:
-        key: If not ``None``, encryption key, or dictionary of encryption keys, to
-            decrypt arrays.
-        array_name: Name of the array to decrypt.
-
-    Returns:
+    Parameters
+    ----------
+    key
+        If not ``None``, encryption key, or dictionary of encryption keys, to decrypt
+        arrays.
+    array_name
+        Name of the array to decrypt.
+
+    Returns
+    -------
+    Optional[str]
        Key for the array with name ``array_name``.
     """
     return key.get(array_name) if isinstance(key, dict) else key
 
 
 def get_array_uri(group_uri: str, array_name: str) -> str:
     """Returns a URI for an array with name ``array_name`` inside a group at URI
      ``group_uri``.
 
      This method is only needed for creating relative arrays before adding them
      to a group.
 
-    Parameters:
-        group_uri: URI of the group containing the array
-        array_name: name of the array
-
-    Returns:
+    Parameters
+    ----------
+    group_uri
+        URI of the group containing the array
+    array_name
+        name of the array
+
+    Returns
+    -------
+    str:
         Array URI of an array with name ``array_name`` inside a group at URI
-            ``group_uri``.
+        ``group_uri``.
     """
     return os.path.join(group_uri, array_name)
 
 
 def safe_set_metadata(meta, key, value):
     """Copy a metadata item to a TileDB array catching any errors as warnings."""
     if isinstance(value, np.ndarray):
```

### Comparing `tiledb-cf-0.9.0/tiledb/cf/cli.py` & `tiledb-cf-0.9.1/tiledb/cf/cli.py`

 * *Files identical despite different names*

### Comparing `tiledb-cf-0.9.0/tiledb/cf/core/_creator.py` & `tiledb-cf-0.9.1/tiledb/cf/core/_array_creator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,489 +1,167 @@
-"""Classes for creating a dataspace."""
-
 from __future__ import annotations
 
-from abc import ABCMeta
 from collections import OrderedDict
+from collections.abc import Sequence
 from io import StringIO
-from typing import Any, Dict, Optional, Sequence, Tuple, Union
+from typing import Dict, Iterable, List, Optional, Tuple, Union
 
 import numpy as np
+from typing_extensions import Self
 
 import tiledb
 
-from .._utils import DType
-from .api import create_group
-
+from ._attr_creator import AttrCreator
+from ._dim_creator import DimCreator
+from ._fragment_writer import FragmentWriter
+from ._shared_dim import SharedDim
+from .registry import RegisteredByNameMixin, Registry
+from .source import FieldData
 
-class DataspaceCreator:
-    """Creator for a group of arrays that satify the CF Dataspace Convention.
+DenseRange = Union[Tuple[int, int], Tuple[np.datetime64, np.datetime64]]
 
 
-    This class can be used directly to create a TileDB group that follows the
-    TileDB CF Dataspace convention. It is also useful as a super class for
-    converters/ingesters of data from sources that follow a NetCDF or NetCDF-like
-    data model to TileDB.
-    """
-
+class ArrayDimRegistry:
     def __init__(self):
-        self._registry = DataspaceRegistry()
-
-    def __repr__(self):
-        output = StringIO()
-        output.write("DataspaceCreator(")
-        if self._registry.ndim > 0:
-            output.write("\n Shared Dimensions:\n")
-            for dim in self._registry.shared_dims():
-                output.write(f"  '{dim.name}':  {repr(dim)},\n")
-        if self._registry.narray > 0:
-            output.write("\n Array Creators:\n")
-            for array_creator in self._registry.array_creators():
-                output.write(f"  '{array_creator.name}':{repr(array_creator)}\n")
-        output.write(")")
-        return output.getvalue()
-
-    def _repr_html_(self):
-        output = StringIO()
-        output.write(f"<h4>{self.__class__.__name__}</h4>\n")
-        output.write("<ul>\n")
-        output.write("<li>\n")
-        output.write("Shared Dimensions\n")
-        if self._registry.ndim > 0:
-            output.write("<table>\n")
-            for dim in self._registry.shared_dims():
-                output.write(
-                    f'<tr><td style="text-align: left;">{dim.html_input_summary()} '
-                    f"&rarr; SharedDim({dim.html_output_summary()})</td>\n</tr>\n"
-                )
-            output.write("</table>\n")
-        output.write("</li>\n")
-        output.write("<li>\n")
-        output.write("Array Creators\n")
-        for array_creator in self._registry.array_creators():
-            output.write("<details>\n")
-            output.write("<summary>\n")
-            output.write(
-                f"{array_creator.__class__.__name__} <em>{array_creator.name}</em>("
-                f"{', '.join(map(lambda x: str(x.name), array_creator.domain_creator))}"
-                f")\n"
-            )
-            output.write("</summary>\n")
-            output.write(f"{array_creator.html_summary()}\n")
-            output.write("</details>\n")
-        output.write("</li>\n")
-        output.write("</ul>\n")
-        return output.getvalue()
-
-    def add_array_creator(
-        self,
-        array_name: str,
-        dims: Sequence[str],
-        cell_order: str = "row-major",
-        tile_order: str = "row-major",
-        capacity: int = 0,
-        tiles: Optional[Sequence[int]] = None,
-        dim_filters: Optional[Dict[str, tiledb.FilterList]] = None,
-        offsets_filters: Optional[tiledb.FilterList] = None,
-        attrs_filters: Optional[tiledb.FilterList] = None,
-        allows_duplicates: bool = False,
-        sparse: bool = False,
-    ):
-        """Adds a new array to the CF dataspace.
-
-        The name of each array must be unique. All other properties should satisfy
-        the same requirements as a ``tiledb.ArraySchema``.
-
-        Parameters:
-            array_name: Name of the new array to be created.
-            dims: An ordered list of the names of the shared dimensions for the domain
-                of this array.
-            cell_order: The order in which TileDB stores the cells on disk inside a
-                tile. Valid values are: ``row-major`` (default) or ``C`` for row major;
-                ``col-major`` or ``F`` for column major; or ``Hilbert`` for a Hilbert
-                curve.
-            tile_order: The order in which TileDB stores the tiles on disk. Valid values
-                are: ``row-major`` or ``C`` (default) for row major; or ``col-major`` or
-                ``F`` for column major.
-            capacity: The number of cells in a data tile of a sparse fragment.
-            tiles: An optional ordered list of tile sizes for the dimensions of the
-                array. The length must match the number of dimensions in the array.
-            dim_filters: A dict from dimension name to a :class:`tiledb.FilterList`
-                for dimensions in the array.
-            offsets_filters: Filters for the offsets for variable length attributes or
-                dimensions.
-            attrs_filters: Default filters to use when adding an attribute to the
-                array.
-            allows_duplicates: Specifies if multiple values can be stored at the same
-                 coordinate. Only allowed for sparse arrays.
-            sparse: Specifies if the array is a sparse TileDB array (true) or dense
-                TileDB array (false).
-        """
-        ArrayCreator(
-            dataspace_registry=self._registry,
-            name=array_name,
-            dims=dims,
-            cell_order=cell_order,
-            tile_order=tile_order,
-            capacity=capacity,
-            tiles=tiles,
-            dim_filters=dim_filters,
-            offsets_filters=offsets_filters,
-            attrs_filters=attrs_filters,
-            allows_duplicates=allows_duplicates,
-            sparse=sparse,
-        )
-
-    def add_attr_creator(
-        self,
-        attr_name: str,
-        array_name: str,
-        dtype: np.dtype,
-        fill: Optional[Union[int, float, str]] = None,
-        var: bool = False,
-        nullable: bool = False,
-        filters: Optional[tiledb.FilterList] = None,
-    ):
-        """Adds a new attribute to an array in the CF dataspace.
-
-        The 'dataspace name' (name after dropping the suffix ``.data`` or ``.index``)
-        must be unique.
+        self._shared_dims: Dict[str, SharedDim] = dict()
 
-        Parameters:
-            attr_name: Name of the new attribute that will be added.
-            array_name: Name of the array the attribute will be added to.
-            dtype: Numpy dtype of the new attribute.
-            fill: Fill value for unset cells.
-            var: Specifies if the attribute is variable length (automatic for
-                byte/strings).
-            nullable: Specifies if the attribute is nullable using validity tiles.
-            filters: Specifies compression filters for the attribute.
-        """
-        array_creator = self._registry.get_array_creator(array_name)
-        array_creator.add_attr_creator(attr_name, dtype, fill, var, nullable, filters)
-
-    def add_shared_dim(self, dim_name: str, domain: Tuple[Any, Any], dtype: np.dtype):
-        """Adds a new dimension to the CF dataspace.
-
-        Each dimension name must be unique. Adding a dimension where the name, domain,
-        and dtype matches a current dimension does nothing.
-
-        Parameters:
-            dim_name: Name of the new dimension to be created.
-            domain: The (inclusive) interval on which the dimension is valid.
-            dtype: The numpy dtype of the values and domain of the dimension.
-        """
-        SharedDim(self._registry, dim_name, domain, dtype)
-
-    def array_creators(self):
-        """Iterates over array creators in the CF dataspace."""
-        return self._registry.array_creators()
+    def __delitem__(self, name: str):
+        del self._shared_dims[name]
 
-    def create_array(
-        self,
-        uri: str,
-        key: Optional[str] = None,
-        ctx: Optional[tiledb.Ctx] = None,
-    ):
-        """Creates a TileDB array for a CF dataspace with only one array.
+    def __getitem__(self, name: str) -> SharedDim:
+        return self._shared_dims[name]
 
-        Parameters:
-            uri: Uniform resource identifier for the TileDB array to be created.
-            key: If not ``None``, encryption key to decrypt the array.
-            ctx: If not ``None``, TileDB context wrapper for a TileDB storage manager.
-        """
-        if self._registry.narray != 1:
+    def __setitem__(self, name: str, value: SharedDim):
+        if value.is_registered:
+            raise ValueError(f"Shared dimension '{value.name}' is already registered.")
+        old_name = value.name
+        if name != value.name:
+            value.name = name
+        if value.name in self._shared_dims and value != self._shared_dims[value.name]:
+            if value.name != old_name:
+                value.name = old_name
             raise ValueError(
-                f"Can only use `create_array` for a {self.__class__.__name__} with "
-                f"exactly 1 array creator."
+                f"Cannot add shared dimension '{value.name}'. A different shared "
+                f"dimension with that name already exists."
             )
-        array_creator = next(self._registry.array_creators())
-        array_creator.create(uri, key=key, ctx=ctx)
-
-    def create_group(
-        self,
-        uri: str,
-        key: Optional[Union[Dict[str, str], str]] = None,
-        ctx: Optional[tiledb.Ctx] = None,
-        append: bool = False,
-    ):
-        """Creates a TileDB group and arrays for the CF dataspace.
-
-        Parameters:
-            uri: Uniform resource identifier for the TileDB group to be created.
-            key: If not ``None``, encryption key, or dictionary of encryption keys, to
-                decrypt arrays.
-            ctx: If not ``None``, TileDB context wrapper for a TileDB storage manager.
-            append: If ``True``, add arrays in the dataspace to an already existing
-                group. The arrays in the dataspace cannot be in the group that is being
-                append to.
-        """
-        schema = self.to_schema(ctx)
-        create_group(uri, schema, key=key, ctx=ctx, append=append)
-
-    def get_array_creator(self, array_name: str):
-        """Returns the array creator with the requested name.
-
-        Parameters:
-            array_name: Name of the array to return.
-        """
-        return self._registry.get_array_creator(array_name)
-
-    def get_array_creator_by_attr(self, attr_name: str):
-        """Returns the array creator with the requested attribute in it.
-
-        Parameters:
-            attr_name: Name of the attribute to return the array creator with.
-        """
-        return self._registry.get_array_creator_by_attr(attr_name)
-
-    def get_shared_dim(self, dim_name: str):
-        """Returns the shared dimension with the requested name.
-
-        Parameters:
-            array_name: Name of the array to return.
-        """
-        return self._registry.get_shared_dim(dim_name)
-
-    def remove_array_creator(self, array_name: str):
-        """Removes the specified array and all its attributes from the CF dataspace.
-
-        Parameters:
-            array_name: Name of the array that will be removed.
-        """
-        self._registry.deregister_array_creator(array_name)
-
-    def remove_attr_creator(self, attr_name: str):
-        """Removes the specified attribute from the CF dataspace.
+        self._shared_dims[name] = value
 
-        Parameters:
-            attr_name: Name of the attribute that will be removed.
-        """
-        array_creator = self._registry.get_array_creator_by_attr(attr_name=attr_name)
-        array_creator.remove_attr_creator(attr_name)
-
-    def remove_shared_dim(self, dim_name: str):
-        """Removes the specified dimension from the CF dataspace.
-
-        This can only be used to remove dimensions that are not currently being used in
-        an array.
-
-        Parameters:
-            dim_name: Name of the dimension to be removed.
-        """
-        self._registry.deregister_shared_dim(dim_name)
-
-    def shared_dims(self):
-        """Iterators over shared dimensions in the CF dataspace."""
-        return self._registry.shared_dims()
-
-    def to_schema(
-        self, ctx: Optional[tiledb.Ctx] = None
-    ) -> Dict[str, tiledb.ArraySchema]:
-        """Returns a dictionary of array schemas for the CF dataspace.
-
-        Parameters:
-           ctx: If not ``None``, TileDB context wrapper for a TileDB storage manager.
-        """
-        array_schemas = {}
-        for array_creator in self._registry.array_creators():
-            try:
-                array_schemas[array_creator.name] = array_creator.to_schema(ctx)
-            except tiledb.libtiledb.TileDBError as err:
-                raise RuntimeError(
-                    f"Failed to create an ArraySchema for array '{array_creator.name}'."
-                    f" {str(err)}"
-                ) from err
-        return array_schemas
-
-
-class DataspaceRegistry:
-    def __init__(self):
-        self._shared_dims: Dict[str, SharedDim] = {}
-        self._array_creators: Dict[str, ArrayCreator] = {}
-
-    def array_creators(self):
-        """Iterator over array creators in the CF dataspace."""
-        return iter(self._array_creators.values())
-
-    def check_new_array_name(self, array_name: str):
-        if array_name in self._array_creators:
-            raise ValueError(f"An array with name '{array_name}' already exists.")
-
-    def check_new_dim(self, shared_dim: SharedDim):
-        if (
-            shared_dim.name in self._shared_dims
-            and shared_dim != self._shared_dims[shared_dim.name]
-        ):
-            raise ValueError(
-                f"A different dimension with name '{shared_dim.name}' already exists."
-            )
-
-    def check_rename_shared_dim(self, original_name: str, new_name: str):
+    def rename(self, old_name: str, new_name: str):
         if new_name in self._shared_dims:
             raise NotImplementedError(
-                f"Cannot rename dimension '{original_name}' to '{new_name}'. A "
+                f"Cannot rename dimension '{old_name}' to '{new_name}'. A "
                 f"dimension with the same name already exists, and merging dimensions "
                 f"has not yet been implemented."
             )
-        for array_creator in self.array_creators():
-            if array_creator.has_attr_creator(new_name) and original_name in set(
-                dim_creator.name for dim_creator in array_creator.domain_creator
-            ):
-                raise ValueError(
-                    f"Cannot rename dimension '{original_name}' to '{new_name}'. An"
-                    f" attribute with the same name already exists in the array "
-                    f"'{array_creator.name}' that uses this dimension."
-                )
-
-    def deregister_array_creator(self, array_name: str):
-        """Removes the specified array and all its attributes from the CF dataspace.
-
-        Parameters:
-            array_name: Name of the array that will be removed.
-        """
-        del self._array_creators[array_name]
-
-    def deregister_shared_dim(self, dim_name: str):
-        array_list = [
-            array_creator.name
-            for array_creator in self.array_creators()
-            if dim_name
-            in (dim_creator.name for dim_creator in array_creator.domain_creator)
-        ]
-        if array_list:
-            raise ValueError(
-                f"Cannot remove dimension '{dim_name}'. Dimension is being used in "
-                f"arrays: {array_list}."
-            )
-        del self._shared_dims[dim_name]
-
-    def get_array_creator(self, array_name: str) -> ArrayCreator:
-        """Returns the array creator with the requested name."""
-        return self._array_creators[array_name]
-
-    def get_array_creator_by_attr(self, attr_name: str) -> ArrayCreator:
-        """Returns an array creator that contains the requested attribute."""
-        requested = None
-        for array_creator in self.array_creators():
-            if array_creator.has_attr_creator(attr_name):
-                if requested is not None:
-                    raise ValueError(
-                        f"Multiple array creators have an attribute named "
-                        f"'{attr_name}'."
-                    )
-                requested = array_creator
-        if requested is None:
-            raise KeyError(f"No attribute with the name '{attr_name}'.")
-        return requested
-
-    def get_attr_creator(self, attr_name: str) -> AttrCreator:
-        """Returns the attribute creator with the requested name."""
-        array_creator = self.get_array_creator_by_attr(attr_name=attr_name)
-        return array_creator.attr_creator(attr_name)
-
-    def get_shared_dim(self, dim_name: str) -> SharedDim:
-        """Returns the dim creator with the requested name."""
-        return self._shared_dims[dim_name]
-
-    @property
-    def narray(self) -> int:
-        return len(self._array_creators)
-
-    @property
-    def ndim(self) -> int:
-        return len(self._shared_dims)
-
-    def register_array_creator(self, array_creator: ArrayCreator):
-        """Registers a new array creator with the CF dataspace."""
-        self.check_new_array_name(array_creator.name)
-        self._array_creators[array_creator.name] = array_creator
-
-    def register_shared_dim(self, shared_dim: SharedDim):
-        """Registers a new shared dimension to the CF dataspace.
-
-        Parameters:
-            shared_dim: The new shared dimension to register.
-        """
-        self.check_new_dim(shared_dim)
-        self._shared_dims[shared_dim.name] = shared_dim
+        self._shared_dims[new_name] = self._shared_dims.pop(old_name)
 
-    def shared_dims(self):
-        """Iterates over shared dimensions in the CF dataspace."""
-        return iter(self._shared_dims.values())
 
-    def update_array_creator_name(self, original_name: str, new_name: str):
-        self._array_creators[new_name] = self._array_creators.pop(original_name)
-
-    def update_shared_dim_name(self, original_name: str, new_name: str):
-        self._shared_dims[new_name] = self._shared_dims.pop(original_name)
-
-
-class ArrayCreator:
+class ArrayCreator(RegisteredByNameMixin):
     """Creator for a TileDB array using shared dimension definitions.
 
-    Attributes:
-        cell_order: The order in which TileDB stores the cells on disk inside a
-            tile. Valid values are: ``row-major`` (default) or ``C`` for row major;
-            ``col-major`` or ``F`` for column major; or ``Hilbert`` for a Hilbert curve.
-        tile_order: The order in which TileDB stores the tiles on disk. Valid values
-            are: ``row-major`` or ``C`` (default) for row major; or ``col-major`` or
-            ``F`` for column major.
-        capacity: The number of cells in a data tile of a sparse fragment.
-        offsets_filters: Filters for the offsets for variable length attributes or
-            dimensions.
-        attrs_filters: Default filters to use when adding an attribute to the array.
-        allows_duplicates: Specifies if multiple values can be stored at the same
-             coordinate. Only allowed for sparse arrays.
-        sparse: If ``True``, creates a sparse array. Otherwise, create
+    Attributes
+    ----------
+    cell_order
+        The order in which TileDB stores the cells on disk inside a
+        tile. Valid values are: ``row-major`` (default) or ``C`` for row major;
+        ``col-major`` or ``F`` for column major; or ``Hilbert`` for a Hilbert curve.
+    tile_order
+        The order in which TileDB stores the tiles on disk. Valid values are:
+        ``row-major`` or ``C`` (default) for row major; or ``col-major`` or
+        ``F`` for column major.
+    capacity
+        The number of cells in a data tile of a sparse fragment.
+    tiles
+        The tile extents to set on each dimension. The length must match the number
+        of dimensions.
+    dim_filters
+        A dictionary from dimension name to TileDB filters to apply to the dimension.
+    offsets_filters
+        Filters for the offsets for variable length attributes or dimensions.
+    attrs_filters
+        Default filters to use when adding an attribute to the array.
+    allows_duplicates
+        Specifies if multiple values can be stored at the same
+        coordinate. Only allowed for sparse arrays.
+    sparse
+        If ``True``, creates a sparse array. Otherwise, creates a dense array.
+    registry
+        Registry this array will belong to.
+    dim_registry
+        Registry for the shared dimensions this array will use. If none is provided,
+        a registry will be created.
+    shared_dims
+        An ordered list of shared dimensions to use as the dimensions this array.
     """
 
     def __init__(
         self,
-        dataspace_registry: DataspaceRegistry,
-        name: str,
-        dims: Sequence[str],
+        *,
+        name: str = "array",
+        dim_order: Optional[Sequence[str]] = None,
         cell_order: str = "row-major",
         tile_order: str = "row-major",
         capacity: int = 0,
         tiles: Optional[Sequence[int]] = None,
         dim_filters: Optional[Dict[str, tiledb.FilterList]] = None,
         offsets_filters: Optional[tiledb.FilterList] = None,
         attrs_filters: Optional[tiledb.FilterList] = None,
         allows_duplicates: bool = False,
         sparse: bool = False,
-    ):
-        if isinstance(dims, str):
-            dims = (dims,)
-        if len(set(dims)) != len(dims):
+        registry: Optional[Registry[Self]] = None,
+        dim_registry: Optional[Registry[SharedDim]] = None,
+        shared_dims: Optional[Iterable[SharedDim]] = None,
+    ):
+        # Check all dimension names are unique.
+        if dim_order is None:
+            dim_order = tuple()
+        elif isinstance(dim_order, str):
+            dim_order = (dim_order,)
+        if len(set(dim_order)) != len(dim_order):
             raise ValueError(
                 "Cannot create array; the array has repeating dimensions. All "
                 "dimensions must have a unique name."
             )
-        self._registry, self._domain_creator = self._register(
-            dataspace_registry, name, dims
-        )
+
+        # Get dimension registry and add any new dimensions.
+        if dim_registry is None:
+            dim_registry = ArrayDimRegistry()
+        if shared_dims is not None:
+            for dim in shared_dims:
+                dim_registry[dim.name] = dim
+
+        # Initialize the core implementation, the domain creator, and the
+        # attribute registry.
+        self._core = self._new_core(sparse, dim_registry, dim_order)
+        self._domain_creator = self._new_domain_creator()
+        self._attr_registry = ArrayAttrRegistry(self._core)
+
+        # Set array properties.
         self.cell_order = cell_order
         self.tile_order = tile_order
         self.capacity = capacity
         if tiles is not None:
             self._domain_creator.tiles = tiles
         if dim_filters is not None:
             for dim_name, filters in dim_filters.items():
                 self._domain_creator.dim_creator(dim_name).filters = filters
         self.offsets_filters = offsets_filters
         self.attrs_filters = attrs_filters
         self.allows_duplicates = allows_duplicates
         self.sparse = sparse
-        self._name = name
-        dataspace_registry.register_array_creator(self)
+
+        # Set name and registry for the array creator.
+        super().__init__(name, registry)
+
+    def __getitem__(self, key: Union[int, str]) -> AttrCreator:
+        return self._core.get_attr_creator(key)
 
     def __iter__(self):
         """Returns iterator over attribute creators."""
-        return self._registry.attr_creators()
+        return self._core.attr_creators()
 
     def __repr__(self) -> str:
         output = StringIO()
         output.write("  ArrayCreator(\n")
         output.write("     domain=Domain(*[\n")
         for dim_creator in self._domain_creator:
             output.write(f"       {repr(dim_creator)},\n")
@@ -499,35 +177,35 @@
         output.write(f"     capacity={self.capacity},\n")
         output.write(f"     sparse={self.sparse},\n")
         if self.sparse:
             output.write(f"     allows_duplicates={self.allows_duplicates},\n")
         output.write("  )")
         return output.getvalue()
 
-    def _register(
-        self, dataspace_registry: DataspaceRegistry, name: str, dim_names: Sequence[str]
+    def _new_core(
+        self, sparse: bool, dim_registry: Registry[SharedDim], dim_names: Sequence[str]
     ):
-        dim_creators = tuple(
-            DimCreator(dataspace_registry.get_shared_dim(dim_name))
-            for dim_name in dim_names
-        )
+        return ArrayCreatorCore(sparse, dim_registry, dim_names)
 
-        array_registry = ArrayRegistry(dataspace_registry, name, dim_creators)
-        return array_registry, DomainCreator(array_registry, dataspace_registry)
+    def _new_domain_creator(self):
+        return DomainCreator(self._core)
 
     def attr_creator(self, key: Union[int, str]) -> AttrCreator:
         """Returns the requested attribute creator
 
-        Parameters:
-            key: The attribute creator index (int) or name (str).
-
-        Returns:
-            The attribute creator at the given index of name.
+        Parameters
+        ----------
+        key
+            The attribute creator index (int) or name (str).
+
+        Returns
+        -------
+        The attribute creator at the given index of name.
         """
-        return self._registry.get_attr_creator(key)
+        return self._core.get_attr_creator(key)
 
     def add_attr_creator(
         self,
         name: str,
         dtype: np.dtype,
         fill: Optional[Union[int, float, str]] = None,
         var: bool = False,
@@ -535,72 +213,204 @@
         filters: Optional[tiledb.FilterList] = None,
     ):
         """Adds a new attribute to an array in the CF dataspace.
 
         The attribute's 'dataspace name' (name after dropping the suffix ``.data`` or
         ``.index``) must be unique.
 
-        Parameters:
-            name: Name of the new attribute that will be added.
-            dtype: Numpy dtype of the new attribute.
-            fill: Fill value for unset cells.
-            var: Specifies if the attribute is variable length (automatic for
-                byte/strings).
-            nullable: Specifies if the attribute is nullable using validity tiles.
-            filters: Specifies compression filters for the attribute. If ``None``, use
-                the array's ``attrs_filters`` property.
+        Parameters
+        ----------
+        name
+            Name of the new attribute that will be added.
+        dtype
+            Numpy dtype of the new attribute.
+        fill
+            Fill value for unset cells.
+        var
+            Specifies if the attribute is variable length (automatic for
+            byte/strings).
+        nullable
+            Specifies if the attribute is nullable using validity tiles.
+        filters
+            Specifies compression filters for the attribute. If ``None``, use
+            the array's ``attrs_filters`` property.
         """
         if filters is None:
             filters = self.attrs_filters
-        AttrCreator(self._registry, name, dtype, fill, var, nullable, filters)
+        AttrCreator(
+            registry=self._attr_registry,
+            name=name,
+            dtype=dtype,
+            fill=fill,
+            var=var,
+            nullable=nullable,
+            filters=filters,
+        )
+
+    def add_dense_fragment_writer(
+        self,
+        target_region: Optional[Tuple[DenseRange, ...]] = None,
+    ):
+        """Add a writer for dense fragments.
+
+        Parameters
+        ----------
+        target_region
+            Region the fragments are written on. If ``None``, the region is
+            set to the entire domain of the array.
+        """
+        self._core.add_dense_fragment_writer(target_region)
+
+    def add_sparse_fragment_writer(
+        self,
+        *,
+        size: Optional[int] = None,
+        shape: Optional[Tuple[int, ...]] = None,
+        form: str = "coo",
+    ):
+        """Add a writer for sparse fragments.
+
+        There are two valid forms for the sparse writer: "coo" and "row-major".
+
+        For "coo" form, the size is used to define the footprint of the data. This
+        supports a general sparse writes. The full expanded data for each dimension
+        must be provided.
+
+        Example input data for "coo" form on a 2D array:
+           dim1 = [1, 2, 1, 2]
+           dim2 = [3, 3, 4, 4]
+           attr = [1, 2, 3, 4]
+
+        For "row-major" form, a grid of data is provided. The data on each dimension
+        is just the dimension for that part of the grid:
+
+        Example input data for "row-major" form on a 2D array:
+            dim1 = [1, 2]
+            dim2 = [3, 4]
+            attr = [1, 2, 3, 4]
+
+        Parameters
+        ----------
+        size
+            The number of elements the fragment stores.
+        shape
+            The shape of the fragment. Required for "row-major" form.
+        form
+            The form for the dimension data. Can either be "coo" (coordinate form) or
+            "row-major".
+        """
+        if size is not None and shape is not None and np.prod(shape) != size:
+            raise ValueError("Mismatch between shape={shape} and size={size}.")
+
+        if form == "coo":
+            if size is None:
+                if shape is None:
+                    raise TypeError(
+                        "Must provided shape or size for writing in 'coo' form."
+                    )
+                size = np.prod(shape)
+            self._core.add_sparse_coo_fragment_writer(size)
+        elif form == "row-major":
+            if shape is None:
+                raise ValueError("Must set shape when using form 'row-major'.")
+            self._core.add_sparse_row_major_fragment_writer(shape)
+        else:
+            raise ValueError(
+                f"'{form}' is not a valid value for 'form'. Valid options include: "
+                f"'coo', 'row-major'."
+            )
 
     def create(
         self, uri: str, key: Optional[str] = None, ctx: Optional[tiledb.Ctx] = None
     ):
         """Creates a TileDB array at the provided URI.
 
-        Parameters:
-            uri: Uniform resource identifier for the array to be created.
-            key: If not ``None``, encryption key to decrypt arrays.
-            ctx: If not ``None``, TileDB context wrapper for a TileDB storage manager.
+        Parameters
+        ----------
+        uri
+            Uniform resource identifier for the array to be created.
+        key
+            If not ``None``, encryption key to decrypt arrays.
+        ctx
+            If not ``None``, TileDB context wrapper for a TileDB storage manager.
         """
         tiledb.Array.create(uri=uri, schema=self.to_schema(ctx), key=key, ctx=ctx)
 
+    def write(
+        self,
+        uri: str,
+        *,
+        key: Optional[str] = None,
+        ctx: Optional[tiledb.Ctx] = None,
+        timestamp: Optional[int] = None,
+        append: bool = False,
+        skip_metadata: bool = False,
+        writer_indices: Optional[Iterable[int]] = None,
+    ):
+        """Writes data to a TileDB array at the provided URI.
+
+        If ``apend=True``, a new TileDB array will be created at the URI. Otherwise,
+        the data will be written to an existing array.
+
+        Parameters
+        ----------
+        uri
+            Uniform resource identifier for the array.
+        key
+            If not ``None``, encryption key to decrypt arrays.
+        timestamp
+            If not ``None``, the timestamp to write new data at.
+        append
+            If ``True``, write data to an existing array. Otherwise, create a new array.
+        skip_metadata
+            If ``True``, do not write metadata.
+        writer_indices
+            If not ``None``, an iterable list of fragment writers to write from.
+        """
+        if not append:
+            self.create(uri, key=key, ctx=ctx)
+        with tiledb.open(uri, key=key, ctx=ctx, timestamp=timestamp, mode="w") as array:
+            if writer_indices is None:
+                for frag_writer in self._core.fragment_writers():
+                    frag_writer.write(array, skip_metadata=skip_metadata)
+            else:
+                for index in writer_indices:
+                    frag_writer = self._core.get_fragment_writer(index)
+                    frag_writer.write(array, skip_metadata=skip_metadata)
+
     @property
     def domain_creator(self) -> DomainCreator:
         """Domain creator that creates the domain for the TileDB array."""
         return self._domain_creator
 
     def has_attr_creator(self, name: str) -> bool:
         """Returns if an attribute creator with the requested name is in the array
         creator
 
-        Parameters:
-            name: The name of the attribute creator to check for.
+        Parameters
+        ----------
+        name
+            The name of the attribute creator to check for.
+
+        Returns
+        -------
+        bool
+            If an attribute creator with the requested name is in the array creator.
         """
-        return self._registry.has_attr_creator(name)
-
-    @property
-    def name(self) -> str:
-        """Name of the array."""
-        return self._registry.name
-
-    @name.setter
-    def name(self, name: str):
-        self._registry.name = name
+        return self._core.has_attr_creator(name)
 
     @property
     def nattr(self) -> int:
         """Number of attributes in the array."""
-        return self._registry.nattr
+        return self._core.nattr
 
     @property
     def ndim(self) -> int:
         """Number of dimensions in the array."""
-        return self._registry.ndim
+        return self._core.ndim
 
     def html_summary(self) -> str:
         """Returns a string HTML summary of the :class:`ArrayCreator`."""
         cell_style = 'style="text-align: left;"'
         output = StringIO()
         output.write("<ul>\n")
         output.write("<li>\n")
@@ -639,26 +449,45 @@
         output.write("</li>\n")
         output.write("</ul>\n")
         return output.getvalue()
 
     def remove_attr_creator(self, attr_name):
         """Removes the requested attribute from the array.
 
-        Parameters:
-            attr_name: Name of the attribute to remove.
+        Parameters
+        ----------
+        attr_name
+            Name of the attribute to remove.
         """
-        return self._registry.deregister_attr_creator(attr_name)
+        return self._core.deregister_attr_creator(attr_name)
+
+    @property
+    def sparse(self) -> bool:
+        """If the array creator is sparse."""
+        return self._core.sparse
+
+    @sparse.setter
+    def sparse(self, is_sparse: bool):
+        self._core.sparse = is_sparse
 
     def to_schema(self, ctx: Optional[tiledb.Ctx] = None) -> tiledb.ArraySchema:
         """Returns an array schema for the array.
 
-        Parameters:
-            ctx: If not ``None``, TileDB context wrapper for a TileDB storage manager.
+        Parameters
+        ----------
+        ctx
+            If not ``None``, TileDB context wrapper for a TileDB storage manager.
+
+
+        Returns
+        -------
+        tiledb.ArraySchema
+            An array schema for the array from the array creator properties.
         """
-        if self._registry.nattr == 0:
+        if self._core.nattr == 0:
             raise ValueError("Cannot create schema for array with no attributes.")
         domain = self._domain_creator.to_tiledb(ctx)
         attrs = tuple(attr_creator.to_tiledb(ctx) for attr_creator in self)
         return tiledb.ArraySchema(
             domain=domain,
             attrs=attrs,
             cell_order=self.cell_order,
@@ -667,106 +496,241 @@
             offsets_filters=self.offsets_filters,
             allows_duplicates=self.allows_duplicates,
             sparse=self.sparse,
             ctx=ctx,
         )
 
 
-class ArrayRegistry:
+class ArrayCreatorCore:
     def __init__(
-        self,
-        dataspace_registry: DataspaceRegistry,
-        name: str,
-        dim_creators: Tuple[DimCreator, ...],
+        self, sparse: bool, dim_registry: Registry[SharedDim], array_dims: Sequence[str]
     ):
-        self._dataspace_registry = dataspace_registry
-        self._name = name
-        self._dim_creators = dim_creators
+        self._sparse = sparse
+        self._dim_registry = dim_registry
+        self._dim_creators = tuple(
+            self._new_dim_creator(dim_name) for dim_name in array_dims
+        )
         self._attr_creators: Dict[str, AttrCreator] = OrderedDict()
+        self._fragment_writers: List[FragmentWriter] = list()
+
+    def _new_dim_creator(self, dim_name: str, **kwargs):
+        return DimCreator(
+            self._dim_registry[dim_name], registry=DomainDimRegistry(self), **kwargs
+        )
+
+    def add_dense_fragment_writer(
+        self,
+        target_region: Optional[Tuple[Tuple[int, int], ...]],
+    ):
+        """Add a writer for dense fragments.
+
+        Parameters
+        ----------
+        target_region
+            Region the fragments are written on. If ``None``, the region is
+            set to the entire domain of the array.
+        """
+        self._fragment_writers.append(
+            FragmentWriter.create_dense(
+                dims=tuple(dim.base for dim in self._dim_creators),
+                attr_names=self._attr_creators.keys(),
+                target_region=target_region,
+            )
+        )
+
+    def add_sparse_coo_fragment_writer(self, size: int):
+        """Adds a spare writer for a COO fragment.
+
+        For "coo" form, the size is used to define the footprint of the data. This
+        supports a general sparse writes. The full expanded data for each dimension
+        must be provided.
+
+        Example input data for "coo" form on a 2D array:
+           dim1 = [1, 2, 1, 2]
+           dim2 = [3, 3, 4, 4]
+           attr = [1, 2, 3, 4]
+
+        Parameters
+        ----------
+        size
+            The number of elements the fragment stores.
+        """
+        self._fragment_writers.append(
+            FragmentWriter.create_sparse_coo(
+                dims=tuple(dim.base for dim in self._dim_creators),
+                attr_names=self._attr_creators.keys(),
+                size=size,
+            )
+        )
+
+    def add_sparse_row_major_fragment_writer(self, shape: Tuple[int, ...]):
+        """Adds a sparse writer for a row-major grament.
+
+        For "row-major" form, a grid of data is provided. The data on each dimension
+        is just the dimension for that part of the grid:
+
+        Example input data for "row-major" form on a 2D array:
+            dim1 = [1, 2]
+            dim2 = [3, 4]
+            attr = [1, 2, 3, 4]
+
+        Parameters
+        ----------
+        shape
+            The shape of the fragment.
+        """
+        self._fragment_writers.append(
+            FragmentWriter.create_sparse_row_major(
+                dims=tuple(dim.base for dim in self._dim_creators),
+                attr_names=self._attr_creators.keys(),
+                shape=shape,
+            )
+        )
 
     def attr_creators(self):
         """Iterates over attribute creators in the array creator."""
         return iter(self._attr_creators.values())
 
     def check_new_attr_name(self, attr_name):
+        """Raises an error if the provided name is not a valid new attribute name.
+
+        Parameters
+        ----------
+        attr_name
+            The attribute name to check.
+        """
         if attr_name in self._attr_creators:
             raise ValueError(
                 f"An attribute with the name '{attr_name}' already exists in this "
                 f"array."
             )
         for dim_creator in self.dim_creators():
             if attr_name == dim_creator.name:
                 raise ValueError(
                     f"A dimension with the name '{attr_name}' already exists in this "
                     f"array."
                 )
 
     def deregister_attr_creator(self, attr_name: str):
-        """Removes an attribute from the group."""
+        """Removes an attribute from the group.
+
+        Parameters
+        ----------
+        attr_name
+            The name of the attribute creator to remove.
+        """
         del self._attr_creators[attr_name]
+        for frag_writer in self._fragment_writers:
+            frag_writer.remove_attr(attr_name)
 
     def dim_creators(self):
         """Iterates over dimension creators in the array creator."""
         return iter(self._dim_creators)
 
+    def fragment_writers(self):
+        """Iterates over fragmetn writers in the array creator."""
+        return iter(self._fragment_writers)
+
     def get_attr_creator(self, key: Union[str, int]) -> AttrCreator:
         """Returns the requested attribute creator.
 
-        Parameters:
-            attr_name: Name of the attribute to return.
+        Parameters
+        ----------
+        attr_name
+            Name of the attribute creator to return.
         """
         if isinstance(key, int):
             return tuple(self._attr_creators.values())[key]
         return self._attr_creators[key]
 
     def get_dim_creator(self, key: Union[int, str]) -> DimCreator:
         """Returns the requested dimension creator.
 
-        Parameters:
-            key: Name (string) or index (integer) of the dimension to return.
-
-        Returns:
+        Parameters
+        ----------
+        key
+            Name (string) or index (integer) of the dimension to return.
+
+        Returns
+        -------
+        DimCreator
             The requested dimension creator.
         """
         if isinstance(key, int):
             return self._dim_creators[key]
         index = self.get_dim_position_by_name(key)
         return self._dim_creators[index]
 
     def get_dim_position_by_name(self, dim_name: str) -> int:
         """Returns the dimension position of the requested dimension name.
 
-        Parameters:
-            dim_name: Name of the dimension to get the position of.
-
-        Returns:
+        Parameters
+        ----------
+        dim_name
+            Name of the dimension to get the position of.
+
+        Returns
+        -------
+        int
             The position of the requested dimension in the array domain.
         """
         for index, dim_creator in enumerate(self._dim_creators):
             if dim_creator.name == dim_name:
                 return index
         raise KeyError(f"Dimension creator with name '{dim_name}' not found.")
 
-    def has_attr_creator(self, name: str) -> AttrCreator:
+    def get_fragment_writer(self, index: int) -> FragmentWriter:
+        """Returns the fragment writer at the requested index.
+
+        Parameters
+        ----------
+        index
+            The index of the fragment writer to return.
+
+        Returns
+        -------
+        FragmentWriter
+            The requested fragment writer.
+        """
+        return self._fragment_writers[index]
+
+    def has_attr_creator(self, name: str) -> bool:
         """Returns if an attribute creator with the requested name is in the array
-        creator
+        creator.
 
-        Parameters:
-            name: The name of the attribute creator to check for.
+        Parameters
+        ----------
+        name
+            The name of the attribute creator to check for.
+
+        Returns
+        -------
+        bool
+            If an attribute creator with the requested name is in the array creator.
         """
         return name in self._attr_creators
 
-    def inject_dim_creator(self, dim_creator: DimCreator, position: int):
+    def inject_dim_creator(self, dim_name: str, position: int, **dim_kwargs):
         """Add an additional dimension into the domain of the array.
 
-        Parameters:
-            dim_creator: The dimension creator to add.
-            position: Position of the shared dimension. Negative values count backwards
-                from the end of the new number of dimensions.
+        Parameters
+        ----------
+        dim_name
+            Name of the dimension creator that will be added.
+        position
+            Index the dimension creator will be added at.
+        **dim_kwargs: dict, optional
+            Keyword arguments to pass to the dimension creator.
         """
+        if len(self._fragment_writers) > 0:
+            raise NotImplementedError(
+                "Injecting a dimension on an array that already has fragment writers "
+                "is not implemented."
+            )
+        dim_creator = self._new_dim_creator(dim_name, **dim_kwargs)
         if dim_creator.name in {dim_creator.name for dim_creator in self._dim_creators}:
             raise ValueError(
                 f"Cannot add dimension creator `{dim_creator.name}` to this array. "
                 f"That dimension is already in use."
             )
         if dim_creator.name in self._attr_creators:
             raise ValueError(
@@ -780,196 +744,236 @@
                 f"{self.ndim} dimensions."
             )
         self._dim_creators = (
             self._dim_creators[:index] + (dim_creator,) + self._dim_creators[index:]
         )
 
     @property
-    def name(self) -> str:
-        """Name of the array."""
-        return self._name
-
-    @name.setter
-    def name(self, name: str):
-        self._dataspace_registry.check_new_array_name(name)
-        self._dataspace_registry.update_array_creator_name(self._name, name)
-        self._name = name
-
-    @property
     def nattr(self) -> int:
+        """Number of attribute creators."""
         return len(self._attr_creators)
 
     @property
     def ndim(self) -> int:
+        """Number of dimension creators."""
         return len(self._dim_creators)
 
+    @property
+    def nwriter(self) -> int:
+        """Number of writers."""
+        return len(self._fragment_writers)
+
     def register_attr_creator(self, attr_creator):
+        """Register an attribute creator to this array creator."""
         self.check_new_attr_name(attr_creator.name)
         attr_name = attr_creator.name
         self._attr_creators[attr_name] = attr_creator
+        for frag_writer in self._fragment_writers:
+            frag_writer.add_attr(attr_name)
 
     def remove_dim_creator(self, dim_index: int):
         """Remove a dim creator from the array.
 
-        Parameters:
-            dim_creator: The dimension creator to add.
-            position: Position of the shared dimension. Negative values count backwards
-                from the end of the new number of dimensions.
+        Parameters
+        ----------
+        dim_creator
+            The location of the dimension creator to remove.
         """
+        if len(self._fragment_writers) > 0:
+            raise NotImplementedError(
+                "Removing a dimension on an array that already has fragment writers "
+                "is not implemented."
+            )
         index = dim_index + self.ndim if dim_index < 0 else dim_index
         if index < 0 or index >= self.ndim:
             raise IndexError(
                 f"Dimension index {dim_index} is outside the bounds of the domain."
             )
         self._dim_creators = (
             self._dim_creators[:dim_index] + self._dim_creators[dim_index + 1 :]
         )
 
+    def set_writer_attr_data(
+        self, writer_index: Optional[int], attr_name: str, data: FieldData
+    ):
+        """Sets attribute data on a fragment writer.
+
+        Parameters
+        ----------
+        writer_index
+            Index of the fragment writer to add attribute data to.
+        attr_name
+            The name of the attribute creator to add data for.
+        data
+            The data that is being added.
+        """
+        if writer_index is None:
+            if self.nwriter > 1:
+                raise ValueError(
+                    "Must specify `writer_index` for array with multiple writers."
+                )
+            writer_index = 0
+        self._fragment_writers[writer_index].set_attr_data(attr_name, data)
+
+    def set_writer_dim_data(
+        self, writer_index: Optional[int], dim_name: str, data: FieldData
+    ):
+        """Sets dimension data on a fragment writer.
+
+        Parameters
+        ----------
+        writer_index
+            The index of the fragment writer to add dimension data to.
+        dim_name
+            The name of the dimension creator to add data for.
+        data
+            The data that is being added.
+        """
+        if writer_index is None:
+            if self.nwriter > 1:
+                raise ValueError(
+                    "Must specify `writer_index` for array with multiple writers."
+                )
+            writer_index = 0
+        self._fragment_writers[writer_index].set_dim_data(dim_name, data)
+
+    @property
+    def sparse(self) -> bool:
+        """If the array creator is sparse."""
+        return self._sparse
+
+    @sparse.setter
+    def sparse(self, is_sparse: bool):
+        if is_sparse is self._sparse:
+            # No-op
+            return
+        if is_sparse is False and any(
+            not writer.is_dense_region for writer in self._fragment_writers
+        ):
+            raise ValueError(
+                "Cannot convert an array with a sparse fragment writer to a dense "
+                "array."
+            )
+        self._sparse = is_sparse
+
     def update_attr_creator_name(self, original_name: str, new_name: str):
         """Renames an attribute in the array.
 
-        Parameters:
-            original_name: Current name of the attribute to be renamed.
-            new_name: New name the attribute will be renamed to.
+        Parameters
+        ----------
+        original_name
+            Current name of the attribute to be renamed.
+        new_name
+            New name the attribute will be renamed to.
         """
         self._attr_creators[new_name] = self._attr_creators.pop(original_name)
 
 
-class AttrCreator(metaclass=ABCMeta):
-    """Creator for a TileDB attribute.
+class ArrayAttrRegistry:
+    def __init__(self, array_core: ArrayCreatorCore):
+        self._core = array_core
 
-    Attributes:
-        dtype: Numpy dtype of the attribute.
-        fill: Fill value for unset cells.
-        var: Specifies if the attribute is variable length (automatic for
-            byte/strings).
-        nullable: Specifies if the attribute is nullable using validity tiles.
-        filters: Specifies compression filters for the attribute.
-    """
+    def __delitem__(self, name: str):
+        self._core.deregister_attr_creator(name)
 
-    def __init__(
-        self,
-        array_registry: ArrayRegistry,
-        name: str,
-        dtype: np.dtype,
-        fill: Optional[DType] = None,
-        var: bool = False,
-        nullable: bool = False,
-        filters: Optional[tiledb.FilterList] = None,
+    def __getitem__(self, name: str) -> AttrCreator:
+        return self._core.get_attr_creator(name)
+
+    def __setitem__(self, name: str, value: AttrCreator):
+        if value.is_registered:
+            raise ValueError("AttrCreator '{value.name}' is already registered.")
+        if name != value.name:
+            value.name = name
+        self._core.register_attr_creator(value)
+
+    def set_writer_data(
+        self, writer_index: Optional[int], attr_name: str, data: FieldData
     ):
-        self._array_registry = array_registry
-        self._name = name
-        self.dtype = np.dtype(dtype)
-        self.fill = fill
-        self.var = var
-        self.nullable = nullable
-        self.filters = filters
-        self._array_registry.register_attr_creator(self)
-
-    def __repr__(self):
-        filters_str = f", filters=FilterList({self.filters})" if self.filters else ""
-        return (
-            f"AttrCreator(name={self.name}, dtype='{self.dtype!s}', var={self.var}, "
-            f"nullable={self.nullable}{filters_str})"
-        )
+        self._core.set_writer_attr_data(writer_index, attr_name, data)
 
-    def html_summary(self) -> str:
-        """Returns a string HTML summary of the :class:`AttrCreator`."""
-        filters_str = f", filters=FilterList({self.filters})" if self.filters else ""
-        return (
-            f" &rarr; tiledb.Attr(name={self.name}, dtype='{self.dtype!s}', "
-            f"var={self.var}, nullable={self.nullable}{filters_str})"
-        )
+    def rename(self, old_name: str, new_name: str):
+        self._core.check_new_attr_name(new_name)
+        self._core.update_attr_creator_name(old_name, new_name)
 
-    @property
-    def name(self) -> str:
-        """Name of the attribute."""
-        return self._name
-
-    @name.setter
-    def name(self, name: str):
-        self._array_registry.check_new_attr_name(name)
-        self._array_registry.update_attr_creator_name(self._name, name)
-        self._name = name
-
-    def to_tiledb(self, ctx: Optional[tiledb.Ctx] = None) -> tiledb.Attr:
-        """Returns a :class:`tiledb.Attr` using the current properties.
-
-        Parameters:
-            ctx: If not ``None``, TileDB context wrapper for a TileDB storage manager.
-
-        Returns:
-            Returns an attribute with the set properties.
-        """
-        return tiledb.Attr(
-            name=self.name,
-            dtype=self.dtype,
-            fill=self.fill,
-            var=self.var,
-            nullable=self.nullable,
-            filters=self.filters,
-            ctx=ctx,
-        )
+
+class DomainDimRegistry:
+    def __init__(self, array_core: ArrayCreatorCore):
+        self._core = array_core
+
+    def set_writer_data(
+        self, writer_index: Optional[int], dim_name: str, data: FieldData
+    ):
+        self._core.set_writer_dim_data(writer_index, dim_name, data)
 
 
 class DomainCreator:
     """Creator for a TileDB domain."""
 
-    def __init__(self, array_registry, dataspace_registry):
-        self._array_registry = array_registry
-        self._dataspace_registry = dataspace_registry
+    def __init__(self, array_core: ArrayCreatorCore):
+        self._core = array_core
+        self._dim_registry = DomainDimRegistry(self._core)
+
+    def __getitem__(self, key: Union[int, str]):
+        return self._core.get_dim_creator(key)
 
     def __iter__(self):
-        return self._array_registry.dim_creators()
+        return self._core.dim_creators()
 
     def __len__(self):
         return self.ndim
 
     def inject_dim_creator(self, dim_name: str, position: int, **dim_kwargs):
         """Adds a new dimension creator at a specified location.
 
-        Parameters:
-            dim_name: Name of the shared dimension to add to the array's domain.
-            position: Position of the shared dimension. Negative values count backwards
-                from the end of the new number of dimensions.
-            dim_kwargs: Keyword arguments to pass to :class:`DimCreator`.
-        """
-        self._array_registry.inject_dim_creator(
-            DimCreator(self._dataspace_registry.get_shared_dim(dim_name), **dim_kwargs),
-            position,
-        )
+        Parameters
+        ----------
+        dim_name
+            Name of the shared dimension to add to the array's domain.
+        position
+            Position of the shared dimension. Negative values count backwards
+            from the end of the new number of dimensions.
+        dim_kwargs: dict, optional
+            Keyword arguments to pass to ``DimCreator``.
+        """
+        self._core.inject_dim_creator(dim_name, position, **dim_kwargs)
 
     @property
     def ndim(self):
         """Number of dimensions in the domain."""
-        return self._array_registry.ndim
+        return self._core.ndim
 
-    def dim_creator(self, dim_id):
+    def dim_creator(self, dim_id) -> DimCreator:
         """Returns a dimension creator from the domain creator given the dimension's
         index or name.
 
-        Parameter:
-            dim_id: dimension index (int) or name (str)
-
-        Returns:
+        Parameters
+        ----------
+        dim_id
+            dimension index (int) or name (str)
+
+        Returns
+        -------
+        DimCreator
             The dimension creator with the requested key.
         """
-        return self._array_registry.get_dim_creator(dim_id)
+        return self._core.get_dim_creator(dim_id)
 
     def remove_dim_creator(self, dim_id: Union[str, int]):
         """Removes a dimension creator from the array creator.
 
-        Parameters:
-            dim_id: dimension index (int) or name (str)
+        Parameters
+        ----------
+        dim_id
+            dimension index (int) or name (str)
         """
         if isinstance(dim_id, int):
-            self._array_registry.remove_dim_creator(dim_id)
+            self._core.remove_dim_creator(dim_id)
         else:
-            index = self._array_registry.get_dim_position_by_name(dim_id)
-            self._array_registry.remove_dim_creator(index)
+            index = self._core.get_dim_position_by_name(dim_id)
+            self._core.remove_dim_creator(index)
 
     @property
     def tiles(self):
         """Tiles for the dimension creators in the domain."""
         return tuple(dim_creator.tile for dim_creator in self)
 
     @tiles.setter
@@ -979,159 +983,18 @@
                 f"Cannot set tiles. Got {len(tiles)} tile(s) for an array with "
                 f"{self.ndim} dimension(s)."
             )
         for dim_creator, tile in zip(self, tiles):
             dim_creator.tile = tile
 
     def to_tiledb(self, ctx: Optional[tiledb.Ctx] = None) -> tiledb.Domain:
-        """Returns a TileDB domain from the contained dimension creators."""
+        """Returns a TileDB domain from the contained dimension creators.
+
+        Parameters
+        ----------
+        ctx
+            If not ``None``, the context to use when creating the domain.
+        """
         if self.ndim == 0:
             raise ValueError("Cannot create schema for array with no dimensions.")
         tiledb_dims = [dim_creator.to_tiledb() for dim_creator in self]
         return tiledb.Domain(tiledb_dims, ctx=ctx)
-
-
-class DimCreator:
-    """Creator for a TileDB dimension using a SharedDim.
-
-    Attributes:
-        tile: The tile size for the dimension.
-        filters: Specifies compression filters for the dimension.
-    """
-
-    def __init__(
-        self,
-        base: SharedDim,
-        tile: Optional[Union[int, float]] = None,
-        filters: Optional[Union[tiledb.FilterList]] = None,
-    ):
-        self._base = base
-        self.tile = tile
-        self.filters = filters
-
-    def __repr__(self):
-        filters_str = ""
-        if self.filters:
-            filters_str = ", filters=FilterList(["
-            for dim_filter in self.filters:
-                filters_str += repr(dim_filter) + ", "
-            filters_str += "])"
-        return f"DimCreator({repr(self._base)}, tile={self.tile}{filters_str})"
-
-    @property
-    def base(self) -> SharedDim:
-        """Shared definition for the dimensions name, domain, and dtype."""
-        return self._base
-
-    @property
-    def dtype(self) -> np.dtype:
-        """The numpy dtype of the values and domain of the dimension."""
-        return self._base.dtype
-
-    @property
-    def domain(self) -> Optional[Tuple[Optional[DType], Optional[DType]]]:
-        """The (inclusive) interval on which the dimension is valid."""
-        return self._base.domain
-
-    def html_summary(self) -> str:
-        """Returns a string HTML summary of the :class:`DimCreator`."""
-        filters_str = ""
-        if self.filters:
-            filters_str = ", filters=FilterList(["
-            for dim_filter in self.filters:
-                filters_str += repr(dim_filter) + ", "
-            filters_str += "])"
-        return (
-            f"{self._base.html_input_summary()} &rarr; tiledb.Dim("
-            f"{self._base.html_output_summary()}, tile={self.tile}{filters_str})"
-        )
-
-    @property
-    def name(self) -> str:
-        """Name of the dimension."""
-        return self._base.name
-
-    def to_tiledb(self, ctx: Optional[tiledb.Ctx] = None) -> tiledb.Domain:
-        """Returns a :class:`tiledb.Dim` using the current properties.
-
-        Parameters:
-            ctx: If not ``None``, TileDB context wrapper for a TileDB storage manager.
-
-        Returns:
-            A tiledb dimension with the set properties.
-        """
-        if self.domain is None:
-            raise ValueError(
-                f"Cannot create a TileDB dimension for dimension '{self.name}'. No "
-                f"domain is set."
-            )
-        return tiledb.Dim(
-            name=self.name,
-            domain=self.domain,
-            tile=self.tile,
-            filters=self.filters,
-            dtype=self.dtype,
-            ctx=ctx,
-        )
-
-
-class SharedDim(metaclass=ABCMeta):
-    """Definition for the name, domain and data type of a collection of dimensions."""
-
-    def __init__(
-        self,
-        dataspace_registry: DataspaceRegistry,
-        name: str,
-        domain: Optional[Tuple[Optional[DType], Optional[DType]]],
-        dtype: np.dtype,
-    ):
-        self._name = name
-        self.domain = domain
-        self.dtype = np.dtype(dtype)
-        self._dataspace_registry = dataspace_registry
-        self._dataspace_registry.register_shared_dim(self)
-
-    def __eq__(self, other):
-        if not isinstance(other, self.__class__):
-            return False
-        if not isinstance(self, other.__class__):
-            return False
-        return (
-            self.name == other.name
-            and self.domain == other.domain
-            and self.dtype == other.dtype
-        )
-
-    def __repr__(self) -> str:
-        return (
-            f"SharedDim(name={self.name}, domain={self.domain}, dtype='{self.dtype!s}')"
-        )
-
-    def html_input_summary(self) -> str:
-        """Returns a HTML string summarizing the input for the dimension."""
-        return ""
-
-    def html_output_summary(self) -> str:
-        """Returns a string HTML summary of the :class:`SharedDim`."""
-        return f"name={self.name}, domain={self.domain}, dtype='{self.dtype!s}'"
-
-    @property
-    def is_index_dim(self) -> bool:
-        """Returns ``True`` if this is an `index dimension` and ``False`` otherwise.
-
-        An index dimension is a dimension with an integer data type and whose domain
-        starts at 0.
-        """
-        if self.domain:
-            return np.issubdtype(self.dtype, np.integer) and self.domain[0] == 0
-        return False
-
-    @property
-    def name(self) -> str:
-        """Name of the shared dimension."""
-        return self._name
-
-    @name.setter
-    def name(self, name: str):
-        self._dataspace_registry.check_rename_shared_dim(self._name, name)
-        self._dataspace_registry.update_shared_dim_name(self._name, name)
-        self._name = name
```

### Comparing `tiledb-cf-0.9.0/tiledb/cf/core/_metadata.py` & `tiledb-cf-0.9.1/tiledb/cf/core/_metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 ATTR_METADATA_FLAG = "__tiledb_attr."
 DIM_METADATA_FLAG = "__tiledb_dim."
 
 
 class Metadata(MutableMapping):
     """Class for accessing Metadata using the standard MutableMapping API.
 
-    Parameters:
-        metadata (tiledb.Metadata): TileDB array metadata object.
+    Parameters
+    ----------
+    metadata
+        TileDB array metadata object.
     """
 
     def __init__(self, metadata: tiledb.Metadata):
         self._metadata = metadata
 
     def __iter__(self) -> Iterator[str]:
         """Iterates over all metadata keys."""
@@ -33,61 +35,74 @@
     def __len__(self) -> int:
         """Returns the number of metadata items."""
         return sum(1 for _ in self)
 
     def __getitem__(self, key: str) -> Any:
         """Implementation of [key] -> val (dict item retrieval).
 
-        Parameters:
-            key: Key to find value from.
-
-        Returns:
+        Parameters
+        ----------
+        key
+            Key to find value from.
+
+        Returns
+        -------
+        Any
             Value stored with provided key.
         """
         return self._metadata[self._to_tiledb_key(key)]
 
-    def __setitem__(self, key: str, value: Any) -> None:
+    def __setitem__(self, key: str, value: Any):
         """Implementation of [key] <- val (dict item assignment).
 
-        Paremeters:
-            key: key to set
-            value: corresponding value
+        Paremeters
+        ----------
+        key
+            Key to set
+        value
+            Corresponding value
         """
         self._metadata[self._to_tiledb_key(key)] = value
 
     def __delitem__(self, key):
         """Implementation of del [key] (dict item deletion).
 
-        Parameters:
-            key: Key to remove.
+        Parameters
+        ----------
+        key
+            Key to remove.
         """
         del self._metadata[self._to_tiledb_key(key)]
 
     def _to_tiledb_key(self, key: str) -> str:
         """Map an external user metadata key to an internal tiledb key."""
         return key  # pragma: no cover
 
     def _from_tiledb_key(self, tiledb_key: str) -> Optional[str]:
         """Map an internal tiledb key to an external user metadata key.
 
-        Returns:
+        Parameters
+        ----------
+        tiledb_key
+            Internal key to use for metadata.
+
+        Returns
+        -------
+        Optional[str]
             The external user metadata key corresponding to `tiledb_key`,
             or None if there is no such corresponding key.
         """
         return tiledb_key  # pragma: no cover
 
 
 class ArrayMetadata(Metadata):
     """Class for accessing array-related metadata from a TileDB metadata object.
 
     This class provides a way for accessing the TileDB array metadata that excludes
     attribute and dimension specific metadata.
-
-    Parameters:
-        metadata (tiledb.Metadata): TileDB array metadata object for the desired array.
     """
 
     def _to_tiledb_key(self, key: str) -> str:
         if key.startswith(ATTR_METADATA_FLAG):
             raise KeyError("Key is reserved for attribute metadata.")
         if key.startswith(DIM_METADATA_FLAG):
             raise KeyError("Key is reserved for dimension metadata.")
@@ -104,18 +119,20 @@
 
 class AttrMetadata(Metadata):
     """Metadata wrapper for accessing attribute metadata.
 
     This class allows access to the metadata for an attribute stored in the metadata
     for a TileDB array.
 
-    Parameters:
-        metadata (tiledb.Metadata): TileDB array metadata for the array containing the
-            desired attribute.
-        attr (str): Name or index of the arrary attribute being requested.
+    Parameters
+    ----------
+    metadata
+        TileDB array metadata for the array containing the desired attribute.
+    attr
+        Name or index of the arrary attribute being requested.
     """
 
     def __init__(self, metadata: tiledb.Metadata, attr: Union[str, int]):
         super().__init__(metadata)
         try:
             attr_name = metadata.array.attr(attr).name
         except tiledb.TileDBError as err:
@@ -133,18 +150,20 @@
 
 class DimMetadata(Metadata):
     """Metadata wrapper for accessing dimension metadata.
 
     This class allows access to the metadata for a dimension stored in the metadata
     for a TileDB array.
 
-    Parameters:
-        metadata (tiledb.Metadata): TileDB array metadata for the array containing the
-            desired attribute.
-        dim (str): Name or index of the arrary attribute being requested.
+    Parameters
+    ----------
+    metadata
+        TileDB array metadata for the array containing the desired attribute.
+    dim
+        Name or index of the arrary attribute being requested.
     """
 
     def __init__(self, metadata: tiledb.Metadata, dim: Union[str, int]):
         super().__init__(metadata)
         try:
             dim_name = metadata.array.dim(dim).name
         except tiledb.TileDBError as err:
```

### Comparing `tiledb-cf-0.9.0/tiledb/cf/core/api.py` & `tiledb-cf-0.9.1/tiledb/cf/core/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,21 +17,28 @@
     config: Optional[tiledb.Config] = None,
     append: bool = False,
 ):
     """Creates a TileDB group with arrays at relative locations inside the group.
 
     All arrays in the group will be added at a relative URI that matches the array name.
 
-    Parameters:
-        uri: Uniform resource identifier for TileDB group or array.
-        group_schema: A mapping from array names to array schemas to add to the group.
-        ctx: If not ``None``, TileDB context wrapper for a TileDB storage manager.
-        append: If ``True``, add arrays from the provided group schema to an
-            already existing group. The names for the arrays in the group schema
-            cannot already exist in the group being append to.
+    Parameters
+    ----------
+    uri
+        Uniform resource identifier for TileDB group or array.
+    group_schema
+        A mapping from array names to array schemas to add to the group.
+    key
+        A encryption key or dict from array names to encryption keys.
+    ctx
+        If not ``None``, TileDB context wrapper for a TileDB storage manager.
+    append
+        If ``True``, add arrays from the provided group schema to an already existing
+        group. The names for the arrays in the group schema cannot already exist in the
+        group being append to.
     """
     if append:
         check_valid_group(uri, ctx=ctx)
         with tiledb.Group(uri, ctx=ctx) as group:
             for array_name in group_schema:
                 if array_name in group:
                     raise ValueError(
@@ -59,23 +66,31 @@
 ) -> tiledb.Array:
     """Opens an array in a group either by specifying the name of the array or the name
     of an attribute in the array.
 
     If only providing the attribute, there must be exactly one array in the group with
     an attribute with the requested name.
 
-    Parameters:
-        array: If not ``None``, the name of the array to open. Overrides attr if
-            both are provided.
-        attr: If not ``None``, open the array that contains this attr. Attr must be in
-            only one of the group arrays.
-        **kwargs: Keyword arguments to pass to the ``tiledb.open`` method.
-
-    Returns:
-        tiledb.Array opened in the specified mode
+    Parameters
+    ----------
+    group
+        The tiledb group to open the array in.
+    array
+        If not ``None``, the name of the array to open. Overrides attr if both are
+        provided.
+    attr
+        If not ``None``, open the array that contains this attr. Attr must be in only
+        one of the group arrays.
+    **kwargs: dict, optional
+        Keyword arguments to pass to the ``tiledb.open`` method.
+
+    Returns
+    -------
+    tiledb.Array:
+        An array opened in the specified mode
     """
     # Get the item in the group that either has the requested array name or
     # requested attribute.
     if array is not None:
         item = group[array]
     elif attr is not None:
         arrays = tuple(
@@ -86,15 +101,15 @@
         )
         if not arrays:
             raise KeyError(f"No attribute with name '{attr}' found.")
         if len(arrays) > 1:
             raise ValueError(
                 f"The array must be specified when opening an attribute that "
                 f"exists in multiple arrays in a group. Arrays with attribute "
-                f"'{attr}' include: {item.name for item in group}."
+                f"'{attr}' include: {list(item.name for item in group)}."
             )
         item = arrays[0]
     else:
         raise ValueError(
             "Cannot open array. Either an array or attribute must be specified."
         )
     return tiledb.open(item.uri, attr=attr, **kwargs)
```

### Comparing `tiledb-cf-0.9.0/tiledb/cf/netcdf_engine/__init__.py` & `tiledb-cf-0.9.1/tiledb/cf/netcdf_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `tiledb-cf-0.9.0/tiledb/cf/netcdf_engine/_array_converters.py` & `tiledb-cf-0.9.1/tiledb/cf/netcdf_engine/_array_converters.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,61 +3,70 @@
 import itertools
 from typing import Any, Dict, Optional, Sequence, Tuple, Union
 
 import netCDF4
 import numpy as np
 
 import tiledb
-from tiledb.cf.core._creator import (
-    ArrayCreator,
-    ArrayRegistry,
-    DataspaceRegistry,
-    DomainCreator,
-)
 
+from ..core._array_creator import ArrayCreator, ArrayCreatorCore, DomainCreator
+from ..core._shared_dim import SharedDim
+from ..core.registry import Registry
 from ._attr_converters import NetCDF4ToAttrConverter, NetCDF4VarToAttrConverter
 from ._dim_converters import NetCDF4ToDimBase, NetCDF4ToDimConverter
 
 
 class NetCDF4ArrayConverter(ArrayCreator):
     """Converter for a TileDB array from a collection of NetCDF variables.
 
-    Attributes:
-        cell_order: The order in which TileDB stores the cells on disk inside a
-            tile. Valid values are: ``row-major`` (default) or ``C`` for row major;
-            ``col-major`` or ``F`` for column major; or ``Hilbert`` for a Hilbert curve.
-        tile_order: The order in which TileDB stores the tiles on disk. Valid values
-            are: ``row-major`` or ``C`` (default) for row major; or ``col-major`` or
-            ``F`` for column major.
-        capacity: The number of cells in a data tile of a sparse fragment.
-        offsets_filters: Filters for the offsets for variable length attributes or
-            dimensions.
-        attrs_filters: Default filters to use when adding an attribute to the array.
-        allows_duplicates: Specifies if multiple values can be stored at the same
-             coordinate. Only allowed for sparse arrays.
+    Attributes
+    ----------
+    cell_order
+        The order in which TileDB stores the cells on disk inside a tile. Valid values
+        are: ``row-major`` (default) or ``C`` for row major; ``col-major`` or ``F`` for
+        column major; or ``Hilbert`` for a Hilbert curve.
+    tile_order
+        The order in which TileDB stores the tiles on disk. Valid values are:
+        ``row-major`` or ``C`` (default) for row major; or ``col-major`` or  ``F`` for
+        column major.
+    capacity
+        The number of cells in a data tile of a sparse fragment.
+    offsets_filters
+        Filters for the offsets for variable length attributes or dimensions.
+    attrs_filters
+        Default filters to use when adding an attribute to the array.
+    allows_duplicates
+        Specifies if multiple values can be stored at the same coordinate. Only allowed
+        for sparse arrays.
     """
 
     def _copy_to_array(
         self,
         netcdf_group: netCDF4.Group,
         tiledb_array: tiledb.Array,
         indexer: Tuple[slice, ...],
         assigned_dim_values: Optional[Dict[str, Any]],
         assigned_attr_values: Optional[Dict[str, np.ndarray]],
     ):
         """Copies data from a NetCDF group to a TileDB CF array.
 
-        Parameters:
-            netcdf_group: The NetCDF group to copy data from.
-            tiledb_array: The TileDB array to  copy data to.
-            indexer: Slices defining what values to copy for each dimension.
-            assigned_dim_values: Mapping from dimension name to value for dimensions
-                that are not copied from the NetCDF group.
-            assigned_attr_values: Mapping from attribute name to numpy array of values
-                for attributes that are not copied from the NetCDF group.
+        Parameters
+        ----------
+        netcdf_group
+            The NetCDF group to copy data from.
+        tiledb_array
+            The TileDB array to  copy data to.
+        indexer
+            Slices defining what values to copy for each dimension.
+        assigned_dim_values
+            Mapping from dimension name to value for dimensions that are not copied from
+            the NetCDF group.
+        assigned_attr_values
+            Mapping from attribute name to numpy array of values for attributes that are
+            not copied from the NetCDF group.
         """
         assert len(indexer) == self.ndim, "indexer has incorrect number of values"
         netcdf_indexer = tuple(
             index_slice
             for index_slice, dim_creator in zip(indexer, self.domain_creator)
             if dim_creator.is_from_netcdf
         )
@@ -77,24 +86,21 @@
 
                 data[attr_name] = assigned_attr_values[attr_name][indexer]
         coord_values = self._domain_creator.get_query_coordinates(
             netcdf_group, self.sparse, indexer, assigned_dim_values
         )
         tiledb_array[coord_values] = data
 
-    def _register(
-        self, dataspace_registry: DataspaceRegistry, name: str, dim_names: Sequence[str]
+    def _new_core(
+        self, sparse: bool, dim_registry: Registry[SharedDim], dim_names: Sequence[str]
     ):
-        shared_dims = map(dataspace_registry.get_shared_dim, dim_names)
-        dim_creators = tuple(map(NetCDF4ToDimConverter, shared_dims))
-        array_registry = ArrayRegistry(dataspace_registry, name, dim_creators)
-        return (
-            array_registry,
-            NetCDF4DomainConverter(array_registry, dataspace_registry),
-        )
+        return NetCDF4ArrayConverterCore(sparse, dim_registry, dim_names)
+
+    def _new_domain_creator(self):
+        return NetCDF4DomainConverter(self._core)
 
     def add_var_to_attr_converter(
         self,
         ncvar: netCDF4.Variable,
         name: Optional[str] = None,
         dtype: Optional[np.dtype] = None,
         fill: Optional[Union[int, float, str]] = None,
@@ -104,42 +110,49 @@
         unpack: bool = False,
     ):
         """Adds a new variable to attribute converter to the array creator.
 
         The attribute's 'dataspace name' (name after dropping the suffix ``.data`` or
         ``.index``) be unique.
 
-        Parameters:
-            ncvar: NetCDF variable to convert to a TileDB attribute.
-            name: Name of the new attribute that will be added. If ``None``, the name
-                will be copied from the NetCDF variable.
-            dtype: Numpy dtype of the new attribute. If ``None``, the data type will be
-                copied from the variable.
-            fill: Fill value for unset cells. If ``None``, the fill value will be
-                copied from the NetCDF variable if it has a fill value.
-            var: Specifies if the attribute is variable length (automatic for
-                byte/strings).
-            nullable: Specifies if the attribute is nullable using validity tiles.
-            filters: Specifies compression filters for the attribute. If ``None``, use
-                array's ``attrs_filters`` property.
-            unpack: Unpack NetCDF data that has NetCDF attributes ``scale_factor`` or
-                ``add_offset`` using the transformation ``scale_factor * value +
-                unpack``.
+        Parameters
+        ----------
+        ncvar
+            NetCDF variable to convert to a TileDB attribute.
+        name
+            Name of the new attribute that will be added. If ``None``, the name will be
+            copied from the NetCDF variable.
+        dtype
+            Numpy dtype of the new attribute. If ``None``, the data type will be copied
+            from the variable.
+        fill
+            Fill value for unset cells. If ``None``, the fill value will be copied from
+            the NetCDF variable if it has a fill value.
+        var
+            Specifies if the attribute is variable length (automatic for byte/strings).
+        nullable
+            Specifies if the attribute is nullable using validity tiles.
+        filters
+            Specifies compression filters for the attribute. If ``None``, use array's
+            ``attrs_filters`` property.
+        unpack
+            Unpack NetCDF data that has NetCDF attributes ``scale_factor`` or
+            ``add_offset`` using the transformation ``scale_factor * value + unpack``.
         """
         if ncvar.dimensions != self.domain_creator.netcdf_dims:
             raise ValueError(
                 f"Cannot add NetCDF variable converter with NetCDF dimensions "
                 f"that do not match the array NetCDF dimension converters. Variable "
                 f"dimensions={ncvar.dimensions}, array NetCDF dimensions="
                 f"{self.domain_creator.netcdf_dims}."
             )
         if filters is None:
             filters = self.attrs_filters
         NetCDF4VarToAttrConverter.from_netcdf(
-            array_registry=self._registry,
+            registry=self._attr_registry,
             ncvar=ncvar,
             name=name,
             dtype=dtype,
             fill=fill,
             var=var,
             nullable=nullable,
             filters=filters,
@@ -155,26 +168,35 @@
         tiledb_timestamp: Optional[int] = None,
         assigned_dim_values: Optional[Dict[str, Any]] = None,
         assigned_attr_values: Optional[Dict[str, np.ndarray]] = None,
         copy_metadata: bool = True,
     ):
         """Copies data from a NetCDF group to a TileDB CF array.
 
-        Parameters:
-            netcdf_group: The NetCDF group to copy data from.
-            tiledb_uri: The TileDB array uri to copy data into.
-            tiledb_key: If not ``None``, the encryption key for the TileDB array.
-            tiledb_ctx: If not ``None``, the TileDB context wrapper for a TileDB
-                storage manager to use when opening the TileDB array.
-            tiledb_timestamp: If not ``None``, the timestamp to write the TileDB data
-                at.
-            assigned_dim_values: Mapping from dimension name to value for dimensions
-                that are not copied from the NetCDF group.
-            assigned_attr_values: Mapping from attribute name to numpy array of values
-                for attributes that are not copied from the NetCDF group.
+        Parameters
+        ----------
+        netcdf_group
+            The NetCDF group to copy data from.
+        tiledb_uri
+            The TileDB array uri to copy data into.
+        tiledb_key
+            If not ``None``, the encryption key for the TileDB array.
+        tiledb_ctx
+            If not ``None``, the TileDB context wrapper for a TileDB storage manager to
+            use when opening the TileDB array.
+        tiledb_timestamp
+            If not ``None``, the timestamp to write the TileDB data at.
+        assigned_dim_values
+            Mapping from dimension name to value for dimensions that are not copied
+            from the NetCDF group.
+        assigned_attr_values
+            Mapping from attribute name to numpy array of values for attributes that
+            are not copied from the NetCDF group.
+        copy_metadata
+            If ``False``, do not copy the metadata from netCDF.
         """
         dim_slices = tuple(
             dim_creator.get_fragment_indices(netcdf_group)
             for dim_creator in self.domain_creator
         )
         with tiledb.open(
             tiledb_uri,
@@ -197,31 +219,83 @@
                     tiledb_array,
                     indexer,
                     assigned_dim_values,
                     assigned_attr_values,
                 )
 
 
+class NetCDF4ArrayConverterCore(ArrayCreatorCore):
+    def _new_dim_creator(self, dim_name: str, **kwargs):
+        return NetCDF4ToDimConverter(self._dim_registry[dim_name], **kwargs)
+
+    def inject_dim_creator(self, dim_name: str, position: int, **dim_kwargs):
+        """Add an additional dimension into the domain of the array.
+
+        Parameters
+        ----------
+        dim_name
+            Name of the shared dimension to add to the array's domain.
+        position
+            Position of the shared dimension. Negative values count backwards from the
+            end of the new number of dimensions.
+        dim_kwargs
+            Keyword arguments to pass to ``NetCDF4ToDimConverter``.
+        """
+        dim_creator = self._new_dim_creator(dim_name, **dim_kwargs)
+        if dim_creator.is_from_netcdf:
+            if any(
+                isinstance(attr_creator, NetCDF4VarToAttrConverter)
+                for attr_creator in self.attr_creators()
+            ):
+                raise ValueError(
+                    "Cannot add a new NetCDF dimension converter to an array that "
+                    "already contains NetCDF variable to attribute converters."
+                )
+        if dim_creator.name in {dim_creator.name for dim_creator in self._dim_creators}:
+            raise ValueError(
+                f"Cannot add dimension creator `{dim_creator.name}` to this array. "
+                f"That dimension is already in use."
+            )
+        if dim_creator.name in self._attr_creators:
+            raise ValueError(
+                f"Cannot add dimension creator `{dim_creator.name}` to this array. An "
+                f"attribute creator with that name already exists."
+            )
+        index = self.ndim + 1 + position if position < 0 else position
+        if index < 0 or index > self.ndim:
+            raise IndexError(
+                f"Cannot add dimension to position {position} for an array with "
+                f"{self.ndim} dimensions."
+            )
+        self._dim_creators = (
+            self._dim_creators[:index] + (dim_creator,) + self._dim_creators[index:]
+        )
+
+
 class NetCDF4DomainConverter(DomainCreator):
     """Converter for NetCDF dimensions to a TileDB domain."""
 
     def get_query_coordinates(
         self,
         netcdf_group: netCDF4.Group,
         sparse: bool,
         indexer: Sequence[slice],
         assigned_dim_values: Optional[Dict[str, Any]] = None,
     ):
         """Returns the coordinates used to copy data from a NetCDF group.
 
-        Parameters:
-            netcdf_group: Group to query the data from.
-            sparse: If ``True``, return coordinates for a sparse write. If ``False``,
-                return coordinates for a dense write.
-            assigned_dim_values: Values for any non-NetCDF dimensions.
+        Parameters
+        ----------
+        netcdf_group
+            Group to query the data from.
+        sparse
+            If ``True``, return coordinates for a sparse write. If ``False``, return
+            coordinates for a dense write.
+        assigned_dim_values
+            Values for any non-NetCDF dimensions.
         """
         if len(indexer) != self.ndim:
             raise ValueError(
                 f"Indexer must be the same length as the domain of the array. Indexer "
                 f"of length {len(indexer)} provide for an array with {self.ndim} "
                 f"dimensions."
             )
@@ -237,33 +311,25 @@
                 for dim_data in np.meshgrid(*query_coords, indexing="ij")
             )
         return query_coords
 
     def inject_dim_creator(self, dim_name: str, position: int, **dim_kwargs):
         """Add an additional dimension into the domain of the array.
 
-        Parameters:
-            dim_name: Name of the shared dimension to add to the array's domain.
-            position: Position of the shared dimension. Negative values count backwards
-                from the end of the new number of dimensions.
-            dim_kwargs: Keyword arguments to pass to :class:`NetCDF4ToDimConverter`.
+        Parameters
+        ----------
+        dim_name
+            Name of the shared dimension to add to the array's domain.
+        position
+            Position of the shared dimension. Negative values count backwards from the
+            end of the new number of dimensions.
+        dim_kwargs
+            Keyword arguments to pass to :class:`NetCDF4ToDimConverter`.
         """
-        dim_creator = NetCDF4ToDimConverter(
-            self._dataspace_registry.get_shared_dim(dim_name), **dim_kwargs
-        )
-        if dim_creator.is_from_netcdf:
-            if any(
-                isinstance(attr_creator, NetCDF4VarToAttrConverter)
-                for attr_creator in self._array_registry.attr_creators()
-            ):
-                raise ValueError(
-                    "Cannot add a new NetCDF dimension converter to an array that "
-                    "already contains NetCDF variable to attribute converters."
-                )
-        self._array_registry.inject_dim_creator(dim_creator, position)
+        self._core.inject_dim_creator(dim_name, position, **dim_kwargs)
 
     @property
     def max_fragment_shape(self):
         """Maximum shape of a fragment when copying from NetCDF to TileDB.
 
         For a dense array, this is the shape of dense fragment. For a sparse array,
         it is the maximum number of coordinates copied for each dimension.
@@ -289,26 +355,28 @@
             for dim_creator in self
             if hasattr(dim_creator.base, "input_dim_name")
         )
 
     def remove_dim_creator(self, dim_id: Union[str, int]):
         """Removes a dimension creator from the array creator.
 
-        Parameters:
-            dim_id: dimension index (int) or name (str)
+        Parameters
+        ----------
+        dim_id
+            dimension index (int) or name (str)
         """
         index = (
             dim_id
             if isinstance(dim_id, int)
-            else self._array_registry.get_dim_position_by_name(dim_id)
+            else self._core.get_dim_position_by_name(dim_id)
         )
-        dim_creator = self._array_registry.get_dim_creator(index)
+        dim_creator = self._core.get_dim_creator(index)
         if isinstance(dim_creator.base, NetCDF4ToDimBase):
             if any(
                 isinstance(attr_creator, NetCDF4VarToAttrConverter)
-                for attr_creator in self._array_registry.attr_creators()
+                for attr_creator in self._core.attr_creators()
             ):
                 raise ValueError(
                     "Cannot remove NetCDF dimension converter from an array that "
                     "contains NetCDF variable to attribute converters."
                 )
-        self._array_registry.remove_dim_creator(index)
+        self._core.remove_dim_creator(index)
```

### Comparing `tiledb-cf-0.9.0/tiledb/cf/netcdf_engine/_attr_converters.py` & `tiledb-cf-0.9.1/tiledb/cf/netcdf_engine/_attr_converters.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Classes for converting NetCDF4 objects to TileDB attributes."""
 
 from abc import abstractmethod
 from typing import Optional, Sequence, Union
 
 import netCDF4
 import numpy as np
+from typing_extensions import Self
 
 import tiledb
 from tiledb.cf.core import AttrMetadata
-from tiledb.cf.core._creator import ArrayRegistry, AttrCreator
 
+from ..core._attr_creator import AttrCreator
+from ..core.registry import Registry
 from ._utils import (
     COORDINATE_SUFFIX,
     get_netcdf_metadata,
     get_unpacked_dtype,
     get_variable_values,
     safe_set_metadata,
 )
@@ -23,70 +25,91 @@
     """Abstract base class for classes that copy data from objects in a NetCDF group to
     a TileDB attribute.
     """
 
     def copy_metadata(self, netcdf_group: netCDF4.Dataset, tiledb_array: tiledb.Array):
         """Copy the metadata data from NetCDF to TileDB.
 
-        Parameters:
-            netcdf_group: NetCDF group to get the metadata items from.
-            tiledb_array: TileDB array to copy the metadata items to.
+        Parameters
+        ----------
+        netcdf_group
+            NetCDF group to get the metadata items from.
+        tiledb_array
+            TileDB array to copy the metadata items to.
         """
 
     @abstractmethod
     def get_values(
         self,
         netcdf_group: netCDF4.Dataset,
         indexer: Sequence[slice],
     ) -> np.ndarray:
         """Returns TileDB attribute values from a NetCDF group.
 
-        Parameters:
-            netcdf_group: NetCDF group to get the dimension values from.
-            sparse: ``True`` if copying into a sparse array and ``False`` if copying
-                into a dense array.
-            shape: If not ``None``, the shape to return the numpy array as.
-
-        Returns:
-            The values needed to set an attribute in a TileDB array. If the array
-        is sparse the values will be returned as an 1D array; otherwise, they will
-        be returned as an ND array.
+        Parameters
+        ----------
+        netcdf_group
+            NetCDF group to get the dimension values from.
+        indexer
+            Region to get data for.
+
+        Returns
+        -------
+        np.ndarray
+            The values needed to set an attribute in a TileDB array. If the array is
+            sparse the values will be returned as an 1D array; otherwise, they will be
+            returned as an ND array.
         """
 
 
 class NetCDF4VarToAttrConverter(NetCDF4ToAttrConverter):
     """Converter for a NetCDF variable to a TileDB attribute.
 
-    Attributes:
-        name: Name of the new attribute.
-        dtype: Numpy dtype of the attribute.
-        fill: Fill value for unset cells.
-        var: Specifies if the attribute is variable length (automatic for
-            byte/strings).
-        nullable: Specifies if the attribute is nullable using validity tiles.
-        filters: Specifies compression filters for the attribute.
-        input_var_name: Name of the input NetCDF variable that will be converted.
-        input_var_dtype: Numpy dtype of the input NetCDF variable.
+    Parameters
+    ----------
+    name
+        The name of the attribute.
+    dtype
+        The datatype of the attribute that will be created.
+    fill
+        Optional fill value for the attribute that will be created.
+    var
+        Specifies if the attribute that will be created will be variable length
+        (automatic for byte/strings).
+    nullable
+        Specifies if the attribute that will be created will be nullable using
+        validity tiles.
+    filters
+        Filter pipeline to apply to the attribute.
+    input_var_name
+        Name of the input netCDF variable to convert.
+    input_var_dtype
+        Datatype of the netCDF variable to convert.
+    unpack
+        If ``True``, unpack the data before converting.
+    registry
+        Registry for this attribute creator.
     """
 
     def __init__(
         self,
-        array_registry: ArrayRegistry,
         name: str,
         dtype: np.dtype,
         fill: Optional[Union[int, float, str]],
         var: bool,
         nullable: bool,
         filters: Optional[tiledb.FilterList],
         input_var_name: str,
         input_var_dtype: np.dtype,
         unpack: bool,
+        *,
+        registry: Optional[Registry[Self]] = None,
     ):
         super().__init__(
-            array_registry=array_registry,
+            registry=registry,
             name=name,
             dtype=dtype,
             fill=fill,
             var=var,
             nullable=nullable,
             filters=filters,
         )
@@ -106,17 +129,20 @@
             f"NetCDFVariable(name={self.input_var_name}, dtype={self.input_var_dtype})"
             f"{super().html_summary()}"
         )
 
     def copy_metadata(self, netcdf_group: netCDF4.Dataset, tiledb_array: tiledb.Array):
         """Copy the metadata data from NetCDF to TileDB.
 
-        Parameters:
-            netcdf_group: NetCDF group to get the metadata items from.
-            tiledb_array: TileDB array to copy the metadata items to.
+        Parameters
+        ----------
+        netcdf_group
+            NetCDF group to get the metadata items from.
+        tiledb_array
+            TileDB array to copy the metadata items to.
         """
         try:
             variable = netcdf_group.variables[self.input_var_name]
         except KeyError as err:
             raise KeyError(
                 f"The variable '{self.input_var_name}' was not found in the provided "
                 f"NetCDF group."
@@ -128,37 +154,64 @@
             if self.unpack and key in {"scale_factor", "add_offset"}:
                 continue
             safe_set_metadata(attr_meta, key, variable.getncattr(key))
 
     @classmethod
     def from_netcdf(
         cls,
-        array_registry: ArrayRegistry,
         ncvar: netCDF4.Variable,
+        *,
         name: Optional[str] = None,
         dtype: Optional[np.dtype] = None,
         fill: Optional[Union[int, float, str]] = None,
         var: bool = False,
         nullable: bool = False,
         filters: Optional[tiledb.FilterList] = None,
         unpack: bool = False,
+        registry: Optional[Registry[Self]] = None,
     ):
+        """Create from a NetCDF variable.
+
+        Parameters
+        ----------
+        ncvar
+            Input netCDF variable.
+        name
+            Name to use for the attribute. If ``None``, use the NetCDF variable name.
+        dtype
+            The datatype of the attribute. If ``None``, use the NetCDF variable dtype.
+        fill
+            Optional fill value for the attribute. If ``None, use the NetCDF variable
+            fill.
+        var
+            Specifies if the attribute that will be created will be variable length
+            (automatic for byte/strings).
+        nullable
+            Specifies if the attribute that will be created will be nullable using
+            validity tiles.
+        filters
+            Filter pipeline to apply to the attribute.
+        unpack
+            If ``True``, unpack the NetCDF variable before converting.
+        registry
+            The registry for the attribute creator.
+        """
         if fill is None:
             fill = get_netcdf_metadata(ncvar, "_FillValue")
         if name is None:
             name = (
                 ncvar.name
                 if ncvar.name not in ncvar.dimensions
                 else ncvar.name + COORDINATE_SUFFIX
             )
         if dtype is None:
             dtype = get_unpacked_dtype(ncvar) if unpack else ncvar.dtype
         dtype = np.dtype(dtype)
         return cls(
-            array_registry=array_registry,
+            registry=registry,
             name=name,
             dtype=dtype,
             fill=fill,
             var=var,
             nullable=nullable,
             filters=filters,
             input_var_name=ncvar.name,
@@ -169,22 +222,27 @@
     def get_values(
         self,
         netcdf_group: netCDF4.Dataset,
         indexer: Sequence[slice],
     ) -> np.ndarray:
         """Returns TileDB attribute values from a NetCDF group.
 
-        Parameters:
-            netcdf_group: NetCDF group to get the dimension values from.
-            indexer: Slice to query the NetCDF variable on.
-
-        Returns:
-            The values needed to set an attribute in a TileDB array. If the array
-        is sparse the values will be returned as an 1D array; otherwise, they will
-        be returned as an ND array.
+        Parameters
+        ----------
+        netcdf_group
+            NetCDF group to get the dimension values from.
+        indexer
+            Slice to query the NetCDF variable on.
+
+        Returns
+        -------
+        np.ndarray
+            The values needed to set an attribute in a TileDB array. If the array is
+            sparse the values will be returned as an 1D array; otherwise, they will be
+            returned as an ND array.
         """
         try:
             variable = netcdf_group.variables[self.input_var_name]
         except KeyError as err:  # pragma: no cover
             raise KeyError(
                 f"The variable '{self.input_var_name}' was not found in the provided "
                 f"NetCDF group."
```

### Comparing `tiledb-cf-0.9.0/tiledb/cf/netcdf_engine/_dim_converters.py` & `tiledb-cf-0.9.1/tiledb/cf/netcdf_engine/_dim_converters.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,35 +2,53 @@
 
 import itertools
 from abc import abstractmethod
 from typing import Any, Dict, Iterable, Optional, Tuple, Union
 
 import netCDF4
 import numpy as np
+from typing_extensions import Self
 
 import tiledb
 from tiledb.cf.core import DimMetadata
-from tiledb.cf.core._creator import DataspaceRegistry, DimCreator, SharedDim
 
 from .._utils import DType
+from ..core._dim_creator import DimCreator
+from ..core._shared_dim import SharedDim
+from ..core.registry import Registry
 from ._utils import get_unpacked_dtype, get_variable_values, safe_set_metadata
 
 
 class NetCDF4ToDimConverter(DimCreator):
-    """Converter from NetCDF to a TileDB dimension in a :class:`NetCDF4ArrayConverter`
-    using a :class:`SharedDim` for the base dimension.
+    """Converter from NetCDF to a TileDB dimension in a ``NetCDF4ArrayConverter``
+    using a ``SharedDim`` for the base dimension.
 
-    Attributes:
-        tile: The tile size for the dimension.
-        filters: Specifies compression filters for the dimension.
+    Parameters
+    ----------
+    base
+        The core shared dimension describing the dimension.
+    tile
+        The tile size for the dimension.
+    filters
+        Specifies compression filters for the dimension.
+    max_fragment_length
+        The size of the maximum length.
+
+    Attributes
+    ----------
+    tile
+        The tile size for the dimension.
+    filters
+        Specifies compression filters for the dimension.
     """
 
     def __init__(
         self,
         base: SharedDim,
+        *,
         tile: Optional[Union[int, float]] = None,
         filters: Optional[tiledb.FilterList] = None,
         max_fragment_length: Optional[int] = None,
     ):
         self._base = base
         self.tile = tile
         self.filters = filters
@@ -48,18 +66,22 @@
             f"max_fragment_length={self.max_fragment_length}{filters_str})"
         )
 
     def get_fragment_indices(self, netcdf_group: netCDF4.Dataset) -> Iterable[slice]:
         """Returns a sequence of slices for copying chunks of the dimension data for
         each TileDB fragment.
 
-        Parameters:
-            netcdf_group: NetCDF group to copy the data from.
-
-        Returns:
+        Parameters
+        ----------
+        netcdf_group
+            NetCDF group to copy the data from.
+
+        Returns
+        -------
+        Iterable[slice]
             A sequence of slices for copying chunks of the dimension data for each
             TileDB fragment.
         """
         if not isinstance(self._base, NetCDF4ToDimBase):
             return (slice(None),)
         size = self.base.get_query_size(netcdf_group)
         if self.max_fragment_length is None:
@@ -73,14 +95,27 @@
     def get_query_coordinates(
         self,
         netcdf_group: netCDF4.Group,
         sparse: bool,
         indexer: slice,
         assigned_dim_values: Optional[Dict[str, Any]],
     ):
+        """Returns the coordinates for querying the array.
+
+        Parameters
+        ----------
+        netcdf_group
+            The netcdf group to get the data from.
+        sparse
+            The sparsity of the array.
+        indexer
+            The slice to indices on.
+        assigned_dim_values
+            Input dimension values for non-NetCDF dimensions.
+        """
         if assigned_dim_values is not None and self.name in assigned_dim_values:
             if self.is_from_netcdf:
                 raise NotImplementedError(
                     "Support for over-writing dimension coordinate values copied from "
                     "NetCDF is not yet implemented."
                 )
             return assigned_dim_values[self.name]
@@ -126,68 +161,103 @@
     """Abstract base class for classes that copy data from objects in a NetCDF group to
     a TileDB dimension.
     """
 
     def copy_metadata(self, netcdf_group: netCDF4.Dataset, tiledb_array: tiledb.Array):
         """Copy the metadata data from NetCDF to TileDB.
 
-        Parameters:
-            netcdf_group: NetCDF group to get the metadata items from.
-            tiledb_array: TileDB array to copy the metadata items to.
+        Parameters
+        ----------
+        netcdf_group
+            NetCDF group to get the metadata items from.
+        tiledb_array
+            TileDB array to copy the metadata items to.
         """
 
     @abstractmethod
     def get_query_size(self, netcdf_group: netCDF4.Dataset):
         """Returns the number of coordinates to copy from NetCDF to TileDB.
 
-        Parameters:
-            netcdf_group: NetCDF group to copy the data from.
+        Parameters
+        ----------
+        netcdf_group
+            NetCDF group to copy the data from.
         """
 
     @abstractmethod
     def get_values(
         self, netcdf_group: netCDF4.Dataset, sparse: bool, indexer: slice
     ) -> Union[np.ndarray, slice]:
         """Returns values from a NetCDF group that will be copied to TileDB.
 
-        Parameters:
-            netcdf_group: NetCDF group to get the values from.
-            sparse: ``True`` if copying into a sparse array and ``False`` if copying
-                into a dense array.
-
-        Returns:
+        Parameters
+        ----------
+        netcdf_group
+            NetCDF group to get the values from.
+        sparse
+            ``True`` if copying into a sparse array and ``False`` if copying into a
+            dense array.
+        indexer
+            The slice to indices on.
+
+        Returns
+        -------
+        np.ndarray or slice
             The coordinates needed for querying the create TileDB dimension in the form
-                of a numpy array if sparse is ``True`` and a slice otherwise.
+            of a numpy array if sparse is ``True`` and a slice otherwise.
         """
 
 
 class NetCDF4CoordToDimConverter(NetCDF4ToDimBase):
     """Converter for a NetCDF variable/dimension pair to a TileDB dimension.
 
-    Attributes:
-        name: Name of the TileDB dimension.
-        domain: The (inclusive) interval on which the dimension is valid.
-        dtype: The numpy dtype of the values and domain of the dimension.
-        input_dim_name: The name of input NetCDF dimension.
-        input_var_name: The name of input NetCDF variable.
-        input_var_dtype: The numpy dtype of the input NetCDF variable.
+    Parameters
+    ----------
+    name
+        Name of the TileDB dimension.
+    domain
+        The (inclusive) interval on which the dimension is valid.
+    dtype
+        The numpy dtype of the values and domain of the dimension.
+    input_dim_name
+        The name of input NetCDF dimension.
+    input_var_name
+        The name of input NetCDF variable.
+    input_var_dtype
+        The numpy dtype of the input NetCDF variable.
+
+    Attributes
+    ----------
+    name
+        Name of the TileDB dimension.
+    domain
+        The (inclusive) interval on which the dimension is valid.
+    dtype
+        The numpy dtype of the values and domain of the dimension.
+    input_dim_name
+        The name of input NetCDF dimension.
+    input_var_name
+        The name of input NetCDF variable.
+    input_var_dtype
+        The numpy dtype of the input NetCDF variable.
     """
 
     def __init__(
         self,
-        dataspace_registry: DataspaceRegistry,
         name: str,
         domain: Optional[Tuple[Optional[DType], Optional[DType]]],
         dtype: np.dtype,
         input_dim_name: str,
         input_var_name: str,
         input_var_dtype: np.dtype,
         unpack: bool,
+        *,
+        registry: Optional[Registry[Self]] = None,
     ):
-        super().__init__(dataspace_registry, name, domain, dtype)
+        super().__init__(name, domain, dtype, registry=registry)
         self.input_dim_name = input_dim_name
         self.input_var_name = input_var_name
         self.input_var_dtype = input_var_dtype
         self.unpack = unpack
 
     def __eq__(self, other):
         return (
@@ -218,75 +288,105 @@
                 f"dimension."
             )
         return variable
 
     def copy_metadata(self, netcdf_group: netCDF4.Dataset, tiledb_array: tiledb.Array):
         """Copy the metadata data from NetCDF to TileDB.
 
-        Parameters:
-            netcdf_group: NetCDF group to get the metadata items from.
-            tiledb_array: TileDB array to copy the metadata items to.
+        Parameters
+        ----------
+        netcdf_group
+            NetCDF group to get the metadata items from.
+        tiledb_array
+            TileDB array to copy the metadata items to.
         """
         variable = self._get_ncvar(netcdf_group)
         dim_meta = DimMetadata(tiledb_array.meta, self.name)
         for key in variable.ncattrs():
             if self.unpack and key in {"scale_factor", "add_offset"}:
                 continue
             safe_set_metadata(dim_meta, key, variable.getncattr(key))
 
     @classmethod
     def from_netcdf(
         cls,
-        dataspace_registry: DataspaceRegistry,
         ncvar: netCDF4.Variable,
+        *,
         name: Optional[str] = None,
         domain: Optional[Tuple[DType, DType]] = None,
         dtype: Optional[np.dtype] = None,
         unpack: bool = False,
+        registry: Optional[Registry[Self]] = None,
     ):
+        """Create the dimension from a NetCDF variable.
+
+        Parameters
+        ----------
+        ncvar
+            Input netCDF variable.
+        name
+            Name to use for the attribute. If ``None``, use the NetCDF variable name.
+        domain
+            Domain to use for the dimension.
+        dtype
+            The datatype of the attribute. If ``None``, use the NetCDF variable dtype.
+        unpack
+            If ``True``, unpack the NetCDF variable before converting.
+        registry
+            The registry for the attribute creator.
+        """
         if len(ncvar.dimensions) != 1:
             raise ValueError(
                 f"Cannot create dimension from variable '{ncvar.name}' with shape "
                 f"{ncvar.shape}. Coordinate variables must have only one dimension."
             )
         if dtype is None:
             dtype = get_unpacked_dtype(ncvar) if unpack else ncvar.dtype
         dtype = np.dtype(dtype)
         return cls(
-            dataspace_registry=dataspace_registry,
+            registry=registry,
             name=name if name is not None else ncvar.name,
             domain=domain,
             dtype=dtype,
             input_dim_name=ncvar.dimensions[0],
             input_var_name=ncvar.name,
             input_var_dtype=dtype,
             unpack=unpack,
         )
 
     def get_query_size(self, netcdf_group: netCDF4.Dataset):
         """Returns the number of coordinates to copy from NetCDF to TileDB.
 
-        Parameters:
-            netcdf_group: NetCDF group to copy the data from.
+        Parameters
+        ----------
+        netcdf_group
+            NetCDF group to copy the data from.
         """
         variable = self._get_ncvar(netcdf_group)
         return variable.get_dims()[0].size
 
     def get_values(self, netcdf_group: netCDF4.Dataset, sparse: bool, indexer: slice):
         """Returns the values of the NetCDF coordinate that is being copied, or
         None if the coordinate is of size 0.
 
-        Parameters:
-            netcdf_group: NetCDF group to get the coordinate values from.
-            sparse: ``True`` if copying into a sparse array and ``False`` if copying
-                into a dense array.
-
-        Returns:
+        Parameters
+        ----------
+        netcdf_group
+            NetCDF group to get the coordinate values from.
+        sparse
+            ``True`` if copying into a sparse array and ``False`` if copying into a
+            dense array.
+        indexer
+            The slice to indices on.
+
+        Returns
+        -------
+        np.ndarray or None
             The coordinate values needed for querying the TileDB dimension in the
-                form a numpy array.
+            form a numpy array.
         """
         if indexer.step not in {1, None}:
             raise ValueError("Dimension indexer must have step size of 1.")
         if not sparse:
             raise NotImplementedError(
                 "Support for copying NetCDF coordinates to dense arrays has not "
                 "been implemented."
@@ -310,34 +410,57 @@
     def is_index_dim(self) -> bool:
         return False
 
 
 class NetCDF4DimToDimConverter(NetCDF4ToDimBase):
     """Converter for a NetCDF dimension to a TileDB dimension.
 
-    Attributes:
-        name: Name of the TileDB dimension.
-        domain: The (inclusive) interval on which the dimension is valid.
-        dtype: The numpy dtype of the values and domain of the dimension.
-        input_dim_name: Name of the input NetCDF variable.
-        input_dim_size: Size of the input NetCDF variable.
-        is_unlimited: If True, the input NetCDF variable is unlimited.
+    Parameters
+    ----------
+    name
+        Name of the TileDB dimension.
+    domain
+        The (inclusive) interval on which the dimension is valid.
+    dtype
+        The numpy dtype of the values and domain of the dimension.
+    input_dim_name
+        Name of the input NetCDF variable.
+    input_dim_size
+        Size of the input NetCDF variable.
+    is_unlimited
+        If True, the input NetCDF variable is unlimited.
+
+    Attributes
+    ----------
+    name
+        Name of the TileDB dimension.
+    domain
+        The (inclusive) interval on which the dimension is valid.
+    dtype
+        The numpy dtype of the values and domain of the dimension.
+    input_dim_name
+        Name of the input NetCDF dimension
+    input_dim_size
+        Size of the input NetCDF dimension.
+    is_unlimited
+        If True, the input NetCDF dimension is unlimited.
     """
 
     def __init__(
         self,
-        dataspace_registry: DataspaceRegistry,
         name: str,
         domain: Optional[Tuple[Optional[DType], Optional[DType]]],
         dtype: np.dtype,
         input_dim_name: str,
         input_dim_size: int,
         is_unlimited: bool,
+        *,
+        registry: Optional[Registry[Self]],
     ):
-        super().__init__(dataspace_registry, name, domain, dtype)
+        super().__init__(name, domain, dtype, registry=registry)
         self.input_dim_name = input_dim_name
         self.input_dim_size = input_dim_size
         self.is_unlimited = is_unlimited
 
     def __eq__(self, other):
         return (
             super.__eq__(self, other)
@@ -364,55 +487,81 @@
             f"dimension '{self.name}'. No NetCDF dimension with that name exists in "
             f"the NetCDF group '{netcdf_group.path}' or its parent groups."
         )
 
     @classmethod
     def from_netcdf(
         cls,
-        dataspace_registry: DataspaceRegistry,
         dim: netCDF4.Dimension,
         unlimited_dim_size: Optional[int],
         dtype: np.dtype,
+        *,
         name: Optional[str] = None,
+        registry: Optional[Registry[Self]] = None,
     ):
+        """Create the dimension creator from a NetCDF dimension
+
+        Parameters
+        ----------
+        dim
+            Input NetCDF dimension.
+        unlimited_dim_size
+            Size to create the domain for an unlimited dimension.
+        dtype
+            Datatype to use for the dimension.
+        name
+            The name to use for the dimension. If not provided, use the name from the
+            NetCDF dimension.
+        registry
+            The registry for the dimension creator.
+        """
         size = (
             unlimited_dim_size
             if dim.isunlimited() and unlimited_dim_size is not None
             else dim.size
         )
         return cls(
-            dataspace_registry=dataspace_registry,
+            registry=registry,
             name=name if name is not None else dim.name,
             domain=(0, size - 1),
             dtype=dtype,
             input_dim_name=dim.name,
             input_dim_size=dim.size,
             is_unlimited=dim.isunlimited(),
         )
 
     def get_query_size(self, netcdf_group: netCDF4.Dataset):
         """Returns the number of coordinates to copy from NetCDF to TileDB.
 
-        Parameters:
-            netcdf_group: NetCDF group to copy the data from.
+        Parameters
+        ----------
+        netcdf_group
+            NetCDF group to copy the data from.
         """
         dim = self._get_ncdim(netcdf_group)
         return dim.size
 
     def get_values(
         self, netcdf_group: netCDF4.Dataset, sparse: bool, indexer: slice
     ) -> Union[np.ndarray, slice]:
         """Returns the values of the NetCDF dimension that is being copied.
 
-        Parameters:
-            netcdf_group: NetCDF group to get the dimension values from.
-            sparse: ``True`` if copying into a sparse array and ``False`` if copying
-                into a dense array.
-
-        Returns:
+        Parameters
+        ----------
+        netcdf_group
+            NetCDF group to get the dimension values from.
+        sparse
+            ``True`` if copying into a sparse array and ``False`` if copying into a
+            dense array.
+        indexer
+            Range to get values on.
+
+        Returns
+        -------
+        np.ndarray or slice
             The coordinates needed for querying the created TileDB dimension in the form
                 of a numpy array if sparse is ``True`` and a slice otherwise.
         """
         if indexer.step not in {1, None}:
             raise ValueError("Dimension indexer must have step size of 1.")
         start = 0 if indexer.start is None else indexer.start
         stop = indexer.stop
@@ -441,50 +590,78 @@
         size_str = "unlimited" if self.is_unlimited else str(self.input_dim_size)
         return f"NetCDFDimension(name={self.input_dim_name}, size={size_str})"
 
 
 class NetCDF4ScalarToDimConverter(NetCDF4ToDimBase):
     """Converter for NetCDF scalar (empty) dimensions to a TileDB Dimension.
 
-    Attributes:
-        name: Name of the TileDB dimension.
-        domain: The (inclusive) interval on which the dimension is valid.
-        dtype: The numpy dtype of the values and domain of the dimension.
+    Attributes
+    ----------
+    name
+        Name of the TileDB dimension.
+    domain
+        The (inclusive) interval on which the dimension is valid.
+    dtype
+        The numpy dtype of the values and domain of the dimension.
     """
 
     def __repr__(self):
         return f" Scalar dimensions -> {super().__repr__()}"
 
     @classmethod
     def create(
-        cls, dataspace_registry: DataspaceRegistry, dim_name: str, dtype: np.dtype
+        cls,
+        dim_name: str,
+        dtype: np.dtype,
+        *,
+        registry: Optional[Registry[Self]] = None,
     ):
-        return cls(dataspace_registry, dim_name, (0, 0), dtype)
+        """Create a NetCDF scalar to dim converter.
+
+        Parameters
+        ----------
+        dim_name
+            The name of the dimension.
+        dtype
+            The dimension for the datatype.
+        registry
+            The registry for the shared dimension core.
+        """
+        return cls(dim_name, (0, 0), dtype, registry=registry)
 
     def get_query_size(self, netcdf_group: netCDF4.Dataset):
         """Returns the number of coordinates to copy from NetCDF to TileDB.
 
-        Parameters:
-            netcdf_group: NetCDF group to copy the data from.
+        Parameters
+        ----------
+        netcdf_group
+            NetCDF group to copy the data from.
         """
         return 1
 
     def get_values(
         self, netcdf_group: netCDF4.Dataset, sparse: bool, indexer: slice
     ) -> Union[np.ndarray, slice]:
         """Get dimension values from a NetCDF group.
 
-        Parameters:
-            netcdf_group: NetCDF group to get the dimension values from.
-            sparse: ``True`` if copying into a sparse array and ``False`` if copying
-                into a dense array.
-
-        Returns:
+        Parameters
+        ----------
+        netcdf_group
+            NetCDF group to get the dimension values from.
+        sparse
+            ``True`` if copying into a sparse array and ``False`` if copying into a
+            dense array.
+        indexer
+            The slice to get the values on.
+
+        Returns
+        -------
+        np.ndarray or slice
             The coordinates needed for querying the create TileDB dimension in the form
-                of a numpy array if sparse is ``True`` and a slice otherwise.
+            of a numpy array if sparse is ``True`` and a slice otherwise.
         """
         if indexer.step not in {1, None}:
             raise ValueError("Dimension indexer must have step size of 1.")
         if indexer.start not in {None, 0}:
             raise IndexError(
                 f"Cannot copy scalar data to TileDB dimension '{self.name}'. The NetCDF"
                 f" chunk starting at {indexer.start} is out of bounds."
```

### Comparing `tiledb-cf-0.9.0/tiledb/cf/netcdf_engine/_utils.py` & `tiledb-cf-0.9.1/tiledb/cf/netcdf_engine/_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,19 +32,26 @@
     """Returns a NetCDF attribute value from a key if it exists and the default value
     otherwise.
 
     If ``is_number=True``, the result is only returned if it is a numpy number. If the
     key exists but is not a numpy number, then a warning is raised. If the key exists
     and is an array of length 1, the scalar value is returned.
 
-    Parameters:
-        key: NetCDF attribute name to return.
-        default: Default value to return if the attribute is not found.
-
-    Returns:
+    Parameters
+    ----------
+    key
+        NetCDF attribute name to return.
+    default
+        Default value to return if the attribute is not found.
+    is_number
+        If ``True``, the result is only returned if it is a numpy number.
+
+    Returns
+    -------
+    Any
         The NetCDF attribute value, if found. Otherwise, return the default value.
     """
     if key in netcdf_item.ncattrs():
         value = netcdf_item.getncattr(key)
         if is_number:
             if (
                 isinstance(value, str)
@@ -64,16 +71,23 @@
     return default
 
 
 def get_unpacked_dtype(variable: netCDF4.Variable) -> np.dtype:
     """Returns the Numpy data type of a variable after it has been unpacked by applying
     any scale_factor or add_offset.
 
-    Parameters:
-        variable: The NetCDF variable to get the unpacked data type of.
+    Parameters
+    ----------
+    variable
+        The NetCDF variable to get the unpacked data type of.
+
+    Returns
+    -------
+    np.dtype
+        The unpacked data from the NetCDF variable.
     """
     input_dtype = np.dtype(variable.dtype)
     if not np.issubdtype(input_dtype, np.number):
         raise ValueError(
             f"Unpacking only support NetCDF variables with integer or floating-point "
             f"data. Input variable has datatype {input_dtype}."
         )
@@ -91,20 +105,30 @@
     variable: netCDF4.Variable,
     indexer: Union[slice, Sequence[slice]],
     fill: Optional[Union[int, float, str]],
     unpack: bool,
 ) -> np.ndarray:
     """Returns the values for a NetCDF variable at the requested indices.
 
-    Parameters:
-        variable: NetCDF variable to get values from.
-        indexer: Sequence of slices used to index the NetCDF variable.
-        fill: If not ``None``, the fill value to use for the output data.
-        unpack: If ``True``, unpack the variable if it contains a ``scale_factor``
-            or ``add_offset``.
+    Parameters
+    ----------
+    variable
+        NetCDF variable to get values from.
+    indexer
+        Sequence of slices used to index the NetCDF variable.
+    fill
+        If not ``None``, the fill value to use for the output data.
+    unpack
+        If ``True``, unpack the variable if it contains a ``scale_factor`` or
+        ``add_offset``.
+
+    Returns
+    -------
+    np.ndarray
+        The data from the NetCDF variable.
     """
     values = variable.getValue() if variable.ndim == 0 else variable[indexer]
     netcdf_fill = get_netcdf_metadata(variable, "_FillValue")
     if fill is not None and netcdf_fill is not None and fill != netcdf_fill:
         np.putmask(values, values == netcdf_fill, fill)
     if unpack:
         scale_factor = get_netcdf_metadata(variable, "scale_factor", is_number=True)
@@ -118,17 +142,28 @@
 
 def get_variable_chunks(
     variable: netCDF4.Variable, unlimited_dim_size
 ) -> Optional[Tuple[int, ...]]:
     """
     Returns the chunks from a NetCDF variable if chunked and ``None`` otherwise.
 
-
     If one of the dimensions has a unlimited dimension, the chunk size will be
     reduced to the unlimited_dim_size.
+
+    Parameters
+    ----------
+    variable
+        The variable to get chunks from.
+    unlimited_dim_size
+        The size to use for unlimited dimensions.
+
+    Returns
+    -------
+    Tuple[int, ...], optional
+        Chunks from the NetCDF variable if it is chunked and ``None`` otherwise.
     """
     chunks = variable.chunking()
     if chunks is None or chunks == "contiguous":
         return None
     return tuple(
         min(ck, dim.size if unlimited_dim_size is None else unlimited_dim_size)
         if dim.isunlimited()
@@ -144,19 +179,23 @@
     group_path: Optional[str] = None,
 ):
     """Context manager for opening a NetCDF group.
 
     If both an input file and group are provided, this function will prioritize
     opening from the group.
 
-    Parameters:
-        group: A NetCDF group to read from.
-        input_file: A NetCDF file to read from.
-        group_path: The path to the NetCDF group to read from in a NetCDF file. Use
-            ``'/'`` to specify the root group.
+    Parameters
+    ----------
+    group
+        A NetCDF group to read from.
+    input_file
+        A NetCDF file to read from.
+    group_path
+        The path to the NetCDF group to read from in a NetCDF file. Use ``'/'`` to
+        specify the root group.
     """
     if group is not None:
         if not isinstance(group, (netCDF4.Dataset, netCDF4.Group)):
             raise TypeError(
                 f"Invalid input: group={group} of type {type(group)} is not a netCDF "
                 f"Group or or Dataset."
             )
```

### Comparing `tiledb-cf-0.9.0/tiledb/cf/netcdf_engine/api.py` & `tiledb-cf-0.9.1/tiledb/cf/netcdf_engine/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -28,50 +28,60 @@
     unpack_vars: bool = False,
     offsets_filters: Optional[tiledb.FilterList] = None,
     attrs_filters: Optional[tiledb.FilterList] = None,
     copy_metadata: bool = True,
 ):
     """Converts a NetCDF input file to nested TileDB CF dataspaces.
 
-    See :class:`~tiledb.cf.NetCDF4ConverterEngine` for more
-    information on the backend converter engine used for the conversion.
+    See ``tiledb.cf.NetCDF4ConverterEngine`` for more information on the backend
+    converter engine used for the conversion.
 
-    Parameters:
-        input_file: The input NetCDF file to generate the converter engine from.
-        output_uri: The uniform resource identifier for the TileDB group to be created.
-        input_group_path: The path to the NetCDF group to copy data from. Use ``'/'``
-            for the root group.
-        recursive: If ``True``, recursively convert groups in a NetCDF file. Otherwise,
-            only convert group provided.
-        output_key: If not ``None``, encryption key to decrypt arrays.
-        output_ctx: If not ``None``, TileDB context wrapper for a TileDB storage
-            manager.
-        dim_dtype: The numpy dtype for the TileDB dimensions created from NetCDF
-            dimensions.
-        unlimited_dim_size: The size of the domain for TileDB dimensions created
-            from unlimited NetCDF dimensions.
-        dim_dtype: The numpy dtype for TileDB dimensions.
-        tiles_by_var: A map from the name of a NetCDF variable to the tiles of the
-            dimensions of the variable in the generated TileDB array.
-        tiles_by_dims: A map from the name of NetCDF dimensions defining a variable
-            to the tiles of those dimensions in the generated TileDB array.
-        coords_to_dims: If ``True``, convert the NetCDF coordinate variable into a
-            TileDB dimension for sparse arrays. Otherwise, convert the coordinate
-            dimension into a TileDB dimension and the coordinate variable into a
-            TileDB attribute.
-        collect_attrs: If ``True``, store all attributes with the same dimensions in
-            the same array. Otherwise, store each attribute in a scalar array.
-        unpack_vars: Unpack NetCDF variables with NetCDF attributes ``scale_factor``
-            or ``add_offset`` using the transformation ``scale_factor * value +
-            unpack``.
-        offsets_filters: Default filters for all offsets for variable attributes
-            and dimensions.
-        attrs_filters: Default filters for all attributes.
-        copy_metadata: If  ``True`` copy NetCDF group and variable attributes to
-            TileDB metadata. If ``False`` do not copy metadata.
+    Parameters
+    ----------
+    input_file
+        The input NetCDF file to generate the converter engine from.
+    output_uri
+        The uniform resource identifier for the TileDB group to be created.
+    input_group_path:
+        The path to the NetCDF group to copy data from. Use ``'/'`` for the root group.
+    recursive
+        If ``True``, recursively convert groups in a NetCDF file. Otherwise, only
+        convert group provided.
+    output_key
+        If not ``None``, encryption key to decrypt arrays.
+    output_ctx
+        If not ``None``, TileDB context wrapper for a TileDB storage manager.
+    unlimited_dim_size:
+        The size of the domain for TileDB dimensions created from unlimited NetCDF
+        dimensions.
+    dim_dtype
+        The numpy dtype for TileDB dimensions.
+    tiles_by_var
+        A map from the name of a NetCDF variable to the tiles of the dimensions of the
+        variable in the generated TileDB array.
+    tiles_by_dims
+        A map from the name of NetCDF dimensions defining a variable to the tiles of
+        those dimensions in the generated TileDB array.
+    coords_to_dims
+        If ``True``, convert the NetCDF coordinate variable into a TileDB dimension for
+        sparse arrays. Otherwise, convert the coordinate dimension into a TileDB
+        dimension and the coordinate variable into a TileDB attribute.
+    collect_attrs
+        If ``True``, store all attributes with the same dimensions in the same array.
+        Otherwise, store each attribute in a scalar array.
+    unpack_vars
+        Unpack NetCDF variables with NetCDF attributes ``scale_factor`` or
+        ``add_offset`` using the transformation ``scale_factor * value + unpack``.
+    offsets_filters
+        Default filters for all offsets for variable attributes and dimensions.
+    attrs_filters
+        Default filters for all attributes.
+    copy_metadata
+        If  ``True`` copy NetCDF group and variable attributes to TileDB metadata. If
+        ``False`` do not copy metadata.
     """
     from .converter import NetCDF4ConverterEngine, open_netcdf_group
 
     output_uri = output_uri if not output_uri.endswith("/") else output_uri[:-1]
 
     if tiles_by_var is None:
         tiles_by_var = {}
```

### Comparing `tiledb-cf-0.9.0/tiledb/cf/netcdf_engine/converter.py` & `tiledb-cf-0.9.1/tiledb/cf/netcdf_engine/converter.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 class NetCDF4ConverterEngine(DataspaceCreator):
     """Converter for NetCDF to TileDB using netCDF4.
 
     This class is used to generate and copy data to a TileDB group or array from a
     NetCDF file. The converter can be auto-generated from a NetCDF group, or it can
     be manually defined.
 
-    This is a subclass of :class:`tiledb.cf.DataspaceCreator`. See
-    :class:`tiledb.cf.DataspaceCreator` for documentation of additional properties and
+    This is a subclass of ``tiledb.cf.DataspaceCreator``. See
+    ``tiledb.cf.DataspaceCreator`` for documentation of additional properties and
     methods.
     """
 
     @classmethod
     def from_file(
         cls,
         input_file: Union[str, Path],
@@ -50,40 +50,50 @@
         tiles_by_dims: Optional[Dict[Sequence[str], Optional[Sequence[int]]]] = None,
         coords_to_dims: bool = False,
         collect_attrs: bool = True,
         unpack_vars: bool = False,
         offsets_filters: Optional[tiledb.FilterList] = None,
         attrs_filters: Optional[tiledb.FilterList] = None,
     ):
-        """Returns a :class:`NetCDF4ConverterEngine` from a group in a NetCDF file.
+        """Returns a ``NetCDF4ConverterEngine`` from a group in a NetCDF file.
 
-        Parameters:
-            input_file: The input NetCDF file to generate the converter engine from.
-            group_path: The path to the NetCDF group to copy data from. Use ``'/'`` for
-                the root group.
-            unlimited_dim_size: The size of the domain for TileDB dimensions created
-                from unlimited NetCDF dimensions. If ``None``, the current size of the
-                NetCDF dimension will be used.
-            dim_dtype: The numpy dtype for TileDB dimensions.
-            tiles_by_var: A map from the name of a NetCDF variable to the tiles of the
-                dimensions of the variable in the generated TileDB array.
-            tiles_by_dims: A map from the name of NetCDF dimensions defining a variable
-                to the tiles of those dimensions in the generated TileDB array.
-            coords_to_dims: If ``True``, convert the NetCDF coordinate variable into a
-                TileDB dimension for sparse arrays. Otherwise, convert the coordinate
-                dimension into a TileDB dimension and the coordinate variable into a
-                TileDB attribute.
-            collect_attrs: If True, store all attributes with the same dimensions
-                in the same array. Otherwise, store each attribute in a scalar array.
-            unpack_vars: Unpack NetCDF variables with NetCDF attributes ``scale_factor``
-                or ``add_offset`` using the transformation ``scale_factor * value +
-                unpack``.
-            offsets_filters: Default filters for all offsets for variable attributes
-                and dimensions.
-            attrs_filters: Default filters for all attributes.
+        Parameters
+        ----------
+        input_file
+            The input NetCDF file to generate the converter engine from.
+        group_path
+            The path to the NetCDF group to copy data from. Use ``'/'`` for the root
+            group.
+        unlimited_dim_size
+            The size of the domain for TileDB dimensions created from unlimited NetCDF
+            dimensions. If ``None``, the current size of the NetCDF dimension will be
+            used.
+        dim_dtype
+            The numpy dtype for TileDB dimensions.
+        tiles_by_var
+            A map from the name of a NetCDF variable to the tiles of the
+            dimensions of the variable in the generated TileDB array.
+        tiles_by_dims
+            A map from the name of NetCDF dimensions defining a variable
+            to the tiles of those dimensions in the generated TileDB array.
+        coords_to_dims
+            If ``True``, convert the NetCDF coordinate variable into a
+            TileDB dimension for sparse arrays. Otherwise, convert the coordinate
+            dimension into a TileDB dimension and the coordinate variable into a
+            TileDB attribute.
+        collect_attrs
+            If True, store all attributes with the same dimensions
+            in the same array. Otherwise, store each attribute in a scalar array.
+        unpack_vars
+            Unpack NetCDF variables with NetCDF attributes ``scale_factor`` or
+            ``add_offset`` using the transformation ``scale_factor * value + unpack``.
+        offsets_filters
+            Default filters for all offsets for variable attributes and dimensions.
+        attrs_filters
+            Default filters for all attributes.
         """
         with open_netcdf_group(input_file=input_file, group_path=group_path) as group:
             return cls.from_group(
                 group,
                 unlimited_dim_size,
                 dim_dtype,
                 tiles_by_var,
@@ -109,42 +119,51 @@
         collect_attrs: bool = True,
         unpack_vars: bool = False,
         offsets_filters: Optional[tiledb.FilterList] = None,
         attrs_filters: Optional[tiledb.FilterList] = None,
         default_input_file: Optional[Union[str, Path]] = None,
         default_group_path: Optional[str] = None,
     ):
-        """Returns a :class:`NetCDF4ConverterEngine` from a :class:`netCDF4.Group`.
+        """Returns a ``NetCDF4ConverterEngine`` from a ``netCDF4.Group``.
 
-        Parameters:
-            group: The NetCDF group to convert.
-            unlimited_dim_size: The size of the domain for TileDB dimensions created
-                from unlimited NetCDF dimensions. If ``None``, the current size of the
-                NetCDF variable will be used.
-            dim_dtype: The numpy dtype for TileDB dimensions.
-            tiles_by_var: A map from the name of a NetCDF variable to the tiles of the
-                dimensions of the variable in the generated TileDB array.
-            tiles_by_dims: A map from the name of NetCDF dimensions defining a variable
-                to the tiles of those dimensions in the generated TileDB array.
-            coords_to_dims: If ``True``, convert the NetCDF coordinate variable into a
-                TileDB dimension for sparse arrays. Otherwise, convert the coordinate
-                dimension into a TileDB dimension and the coordinate variable into a
-                TileDB attribute.
-            collect_attrs: If ``True``, store all attributes with the same dimensions
-                in the same array. Otherwise, store each attribute in a scalar array.
-            unpack_vars: Unpack NetCDF variables with NetCDF attributes ``scale_factor``
-                or ``add_offset`` using the transformation ``scale_factor * value +
-                unpack``.
-            offsets_filters: Default filters for all offsets for variable attributes
-                and dimensions.
-            attrs_filters: Default filters for all attributes.
-            default_input_file: If not ``None``, the default NetCDF input file to copy
-                data from.
-            default_group_path: If not ``None``, the default NetCDF group to copy data
-                from. Use ``'/'`` to specify the root group.
+        Parameters
+        ----------
+        netcdf_group
+            The NetCDF group to convert.
+        unlimited_dim_size
+            The size of the domain for TileDB dimensions created
+            from unlimited NetCDF dimensions. If ``None``, the current size of the
+            NetCDF variable will be used.
+        dim_dtype
+            The numpy dtype for TileDB dimensions.
+        tiles_by_var
+            A map from the name of a NetCDF variable to the tiles of the
+            dimensions of the variable in the generated TileDB array.
+        tiles_by_dims
+            A map from the name of NetCDF dimensions defining a variable
+            to the tiles of those dimensions in the generated TileDB array.
+        coords_to_dims
+            If ``True``, convert the NetCDF coordinate variable into a TileDB
+            dimension for sparse arrays. Otherwise, convert the coordinate dimension
+            into a TileDB dimension and the coordinate variable into a TileDB attribute.
+        collect_attrs
+            If ``True``, store all attributes with the same dimensions in the same
+            array. Otherwise, store each attribute in a scalar array.
+        unpack_vars
+            Unpack NetCDF variables with NetCDF attributes ``scale_factor`` or
+            ``add_offset`` using the transformation ``scale_factor * value + unpack``.
+        offsets_filters
+            Default filters for all offsets for variable attributes and dimensions.
+        attrs_filters
+            Default filters for all attributes.
+        default_input_file
+            If not ``None``, the default NetCDF input file to copy data from.
+        default_group_path
+            If not ``None``, the default NetCDF group to copy data from. Use ``'/'`` to
+            specify the root group.
         """
         if collect_attrs:
             return cls._from_group_to_collected_attrs(
                 netcdf_group=netcdf_group,
                 unlimited_dim_size=unlimited_dim_size,
                 dim_dtype=dim_dtype,
                 tiles_by_var=tiles_by_var,
@@ -183,46 +202,55 @@
         scalar_array_name: str,
         unpack_vars: bool,
         offsets_filters: Optional[tiledb.FilterList],
         attrs_filters: Optional[tiledb.FilterList],
         default_input_file: Optional[Union[str, Path]],
         default_group_path: Optional[str],
     ):
-        """Returns a :class:`NetCDF4ConverterEngine` from a :class:`netCDF4.Group`.
+        """Returns a ``NetCDF4ConverterEngine`` from a ``netCDF4.Group``.
 
-        Parameters:
-            group: The NetCDF group to convert.
-            unlimited_dim_size: The size of the domain for TileDB dimensions created
-                from unlimited NetCDF dimensions.
-            dim_dtype: The numpy dtype for TileDB dimensions.
-            tiles_by_var: A map from the name of a NetCDF variable to the tiles of the
-                dimensions of the variable in the generated TileDB array. The tile
-                sizes defined by this dict take priority over the ``tiles_by_dims``
-                parameter and the NetCDF variable chunksize.
-            tiles_by_dims: A map from the name of NetCDF dimensions defining a variable
-                to the tiles of those dimensions in the generated TileDB array. The
-                tile size defined by this dict are used if they are not defined by the
-                parameter ``tiles_by_var``.
-            coords_to_dims: If ``True``, convert the NetCDF coordinate variable into a
-                TileDB dimension for sparse arrays. Otherwise, convert the coordinate
-                dimension into a TileDB dimension and the coordinate variable into a
-                TileDB attribute.
-            scalar_array_name: Name for the array the stores all NetCDF scalar
-                variables. Cannot be the same name as any of the NetCDF variables in
-                the provided NetCDF group.
-            unpack_vars: Unpack NetCDF variables with NetCDF attributes ``scale_factor``
-                or ``add_offset`` using the transformation ``scale_factor * value +
-                unpack``.
-            offsets_filters: Default filters for all offsets for variable attributes
-                and dimensions.
-            attrs_filters: Default filters for all attributes.
-            default_input_file: If not ``None``, the default NetCDF input file to copy
-                data from.
-            default_group_path: If not ``None``, the default NetCDF group to copy data
-                from. Use ``'/'`` to specify the root group.
+        Parameters
+        ---------
+        group
+            The NetCDF group to convert.
+        unlimited_dim_size
+            The size of the domain for TileDB dimensions created from unlimited NetCDF
+            dimensions.
+        dim_dtype
+            The numpy dtype for TileDB dimensions.
+        tiles_by_var
+            A map from the name of a NetCDF variable to the tiles of the dimensions of
+            the variable in the generated TileDB array. The tile sizes defined by this
+            dict take priority over the ``tiles_by_dims`` parameter and the NetCDF
+            variable chunksize.
+        tiles_by_dims
+            A map from the name of NetCDF dimensions defining a variable to the tiles of
+            those dimensions in the generated TileDB array. The tile size defined by
+            this dict are used if they are not defined by the parameter
+            ``tiles_by_var``.
+        coords_to_dims
+            If ``True``, convert the NetCDF coordinate variable into a
+            TileDB dimension for sparse arrays. Otherwise, convert the coordinate
+            dimension into a TileDB dimension and the coordinate variable into a
+            TileDB attribute.
+        scalar_array_name
+            Name for the array the stores all NetCDF scalar variables. Cannot be the
+            same name as any of the NetCDF variables in the provided NetCDF group.
+        unpack_vars
+            Unpack NetCDF variables with NetCDF attributes ``scale_factor`` or
+            ``add_offset`` using the transformation ``scale_factor * value + unpack``.
+        offsets_filters
+            Default filters for all offsets for variable attributes and dimensions.
+        attrs_filters
+            Default filters for all attributes.
+        default_input_file
+            If not ``None``, the default NetCDF input file to copy data from.
+        default_group_path
+            If not ``None``, the default NetCDF group to copy data from. Use ``'/'`` to
+            specify the root group.
         """
         converter = cls(default_input_file, default_group_path)
         coord_names = set()
         tiles_by_var = {} if tiles_by_var is None else tiles_by_var
         tiles_by_dims = {} if tiles_by_dims is None else tiles_by_dims
         if coords_to_dims:
             for ncvar in netcdf_group.variables.values():
@@ -296,43 +324,51 @@
         coords_to_dims: bool,
         unpack_vars: bool,
         offsets_filters: Optional[tiledb.FilterList],
         attrs_filters: Optional[tiledb.FilterList],
         default_input_file: Optional[Union[str, Path]],
         default_group_path: Optional[str],
     ):
-        """Returns a :class:`NetCDF4ConverterEngine` from a :class:`netCDF4.Group`.
+        """Returns a ``NetCDF4ConverterEngine`` from a ``netCDF4.Group``.
 
-        Parameters:
-            group: The NetCDF group to convert.
-            unlimited_dim_size: The size of the domain for TileDB dimensions created
-                from unlimited NetCDF dimensions. If ``None``, the current size of the
-                NetCDf dimension will be used.
-            dim_dtype: The numpy dtype for TileDB dimensions.
-            tiles_by_var: A map from the name of a NetCDF variable to the tiles of the
-                dimensions of the variable in the generated TileDB array. This will
-                take priority over NetCDF variable chunksize.
-            tiles_by_dims: A map from the name of NetCDF dimensions defining a variable
-                to the tiles of those dimensions in the generated TileDB array. This
-                will take priority over tile sizes defined by the ``tiles_by_var``
-                parameter and the NetCDF variable chunksize.
-            coords_to_dims: If ``True``, convert the NetCDF coordinate variable into a
-                TileDB dimension for sparse arrays. Otherwise, convert the coordinate
-                dimension into a TileDB dimension and the coordinate variable into a
-                TileDB attribute.
-            unpack_vars: Unpack NetCDF variables with NetCDF attributes ``scale_factor``
-                or ``add_offset`` using the transformation ``scale_factor * value +
-                unpack``.
-            offsets_filters: Default filters for all offsets for variable attributes
-                and dimensions.
-            attrs_filters: Default filters for all attributes.
-            default_input_file: If not ``None``, the default NetCDF input file to copy
-                data from.
-            default_group_path: If not ``None``, the default NetCDF group to copy data
-                from. Use ``'/'`` to specify the root group.
+        Parameters
+        ----------
+        group
+            The NetCDF group to convert.
+        unlimited_dim_size
+            The size of the domain for TileDB dimensions created from unlimited NetCDF
+            dimensions. If ``None``, the current size of the  NetCDf dimension will be
+            used.
+        dim_dtype
+            The numpy dtype for TileDB dimensions.
+        tiles_by_var
+            A map from the name of a NetCDF variable to the tiles of the dimensions of
+            the variable in the generated TileDB array. This will take priority over
+            NetCDF variable chunksize.
+        tiles_by_dims
+            A map from the name of NetCDF dimensions defining a variable to the tiles
+            of those dimensions in the generated TileDB array. This will take priority
+            over tile sizes defined by the ``tiles_by_var`` parameter and the NetCDF
+            variable chunksize.
+        coords_to_dims
+            If ``True``, convert the NetCDF coordinate variable into a TileDB dimension
+            for sparse arrays. Otherwise, convert the coordinate dimension into a
+            TileDB dimension and the coordinate variable into a TileDB attribute.
+        unpack_vars
+            Unpack NetCDF variables with NetCDF attributes ``scale_factor`` or
+            ``add_offset`` using the transformation ``scale_factor * value + unpack``.
+        offsets_filters
+            Default filters for all offsets for variable attributes and dimensions.
+        attrs_filters
+            Default filters for all attributes.
+        default_input_file
+            If not ``None``, the default NetCDF input file to copy data from.
+        default_group_path
+            If not ``None``, the default NetCDF group to copy data from. Use ``'/'``
+            to specify the root group.
         """
         converter = cls(default_input_file, default_group_path)
         coord_names = set()
         dims_to_vars: Dict[Tuple[str, ...], List[str]] = defaultdict(list)
         autotiles: Dict[Sequence[str], Optional[Sequence[int]]] = {}
         tiles_by_dims = {} if tiles_by_dims is None else tiles_by_dims
         tiles_by_var = {} if tiles_by_var is None else tiles_by_var
@@ -437,42 +473,52 @@
         sparse: bool = False,
     ):
         """Adds a new NetCDF to TileDB array converter to the CF dataspace.
 
         The name of each array must be unique. All properties must match the normal
         requirements for a ``TileDB.ArraySchema``.
 
-        Parameters:
-            array_name: Name of the new array to be created.
-            dims: An ordered list of the names of the shared dimensions for the domain
-                of this array.
-            cell_order: The order in which TileDB stores the cells on disk inside a
-                tile. Valid values are: ``row-major`` (default) or ``C`` for row major;
-                ``col-major`` or ``F`` for column major; or ``Hilbert`` for a Hilbert
-                curve.
-            tile_order: The order in which TileDB stores the tiles on disk. Valid values
-                are: ``row-major`` or ``C`` (default) for row major; or ``col-major`` or
-                ``F`` for column major.
-            capacity: The number of cells in a data tile of a sparse fragment.
-            tiles: An optional ordered list of tile sizes for the dimensions of the
-                array. The length must match the number of dimensions in the array.
-            dim_filters: A dict from dimension name to a ``FilterList`` for dimensions
-                in the array.
-            offsets_filters: Filters for the offsets for variable length attributes or
-                dimensions.
-            attrs_filters: Default filters to use when adding an attribute to the array.
-            allows_duplicates: Specifies if multiple values can be stored at the same
-                 coordinate. Only allowed for sparse arrays.
-            sparse: Specifies if the array is a sparse TileDB array (true) or dense
-                TileDB array (false).
+        Parameters
+        ----------
+        array_name
+            Name of the new array to be created.
+        dims
+            An ordered list of the names of the shared dimensions for the domain
+            of this array.
+        cell_order
+            The order in which TileDB stores the cells on disk inside a tile. Valid
+            values are: ``row-major`` (default) or ``C`` for row major; ``col-major``
+            or ``F`` for column major; or ``Hilbert`` for a Hilbert curve.
+        tile_order
+            The order in which TileDB stores the tiles on disk. Valid values are:
+            ``row-major`` or ``C`` (default) for row major; or ``col-major`` or ``F``
+            for column major.
+        capacity
+            The number of cells in a data tile of a sparse fragment.
+        tiles
+            An optional ordered list of tile sizes for the dimensions of the
+            array. The length must match the number of dimensions in the array.
+        dim_filters
+            A dict from dimension name to a ``FilterList`` for dimensions in the array.
+        offsets_filters
+            Filters for the offsets for variable length attributes or dimensions.
+        attrs_filters
+            Default filters to use when adding an attribute to the array.
+        allows_duplicates
+            Specifies if multiple values can be stored at the same coordinate. Only
+            allowed for sparse arrays.
+        sparse
+            Specifies if the array is a sparse TileDB array (true) or dense TileDB
+            array (false).
         """
         NetCDF4ArrayConverter(
-            dataspace_registry=self._registry,
+            registry=self._array_registry,
+            dim_registry=self._domain,
             name=array_name,
-            dims=dims,
+            dim_order=dims,
             cell_order=cell_order,
             tile_order=tile_order,
             capacity=capacity,
             tiles=tiles,
             dim_filters=dim_filters,
             offsets_filters=offsets_filters,
             attrs_filters=attrs_filters,
@@ -486,26 +532,30 @@
         dim_name: Optional[str] = None,
         domain: Optional[Tuple[DType, DType]] = None,
         dtype: Optional[np.dtype] = None,
         unpack: bool = False,
     ):
         """Adds a new NetCDF coordinate to TileDB dimension converter.
 
-        Parameters:
-            var: NetCDF coordinate variable to be converted.
-            dim_name: If not ``None``, name to use for the TileDB dimension.
-            domain: If not ``None``, the domain the TileDB dimension is valid on.
-            dtype: If not ``None``, the data type the TileDB dimension will be set to.
-            unpack: Unpack NetCDF data that has NetCDF attributes ``scale_factor`` or
-                ``add_offset`` using the transformation ``scale_factor * value +
-                unpack``.
-
+        Parameters
+        ----------
+        ncvar
+            NetCDF coordinate variable to be converted.
+        dim_name
+            If not ``None``, name to use for the TileDB dimension.
+        domain
+            If not ``None``, the domain the TileDB dimension is valid on.
+        dtype
+            If not ``None``, the data type the TileDB dimension will be set to.
+        unpack
+            Unpack NetCDF data that has NetCDF attributes ``scale_factor`` or
+            ``add_offset`` using the transformation ``scale_factor * value + unpack``.
         """
         NetCDF4CoordToDimConverter.from_netcdf(
-            dataspace_registry=self._registry,
+            registry=self._domain,
             ncvar=ncvar,
             name=dim_name,
             domain=domain,
             dtype=dtype,
             unpack=unpack,
         )
 
@@ -514,42 +564,50 @@
         ncdim: netCDF4.Dimension,
         unlimited_dim_size: Optional[int] = None,
         dtype: np.dtype = _DEFAULT_INDEX_DTYPE,
         dim_name: Optional[str] = None,
     ):
         """Adds a new NetCDF dimension to TileDB dimension converter.
 
-        Parameters:
-            ncdim: NetCDF dimension to be converted.
-            unlimited_dim_size: The size to use if the dimension is unlimited. If
-                ``None``, the current size of the NetCDF dimension will be used.
-            dtype: Numpy type to use for the NetCDF dimension.
-            dim_name: If not ``None``, output name of the TileDB dimension.
+        Parameters
+        ----------
+        ncdim
+            NetCDF dimension to be converted.
+        unlimited_dim_size
+            The size to use if the dimension is unlimited. If ``None``, the current
+            size of the NetCDF dimension will be used.
+        dtype
+            Numpy type to use for the NetCDF dimension.
+        dim_name
+            If not ``None``, output name of the TileDB dimension.
         """
         NetCDF4DimToDimConverter.from_netcdf(
-            dataspace_registry=self._registry,
+            registry=self._domain,
             dim=ncdim,
             unlimited_dim_size=unlimited_dim_size,
             dtype=dtype,
             name=dim_name,
         )
 
     def add_scalar_to_dim_converter(
         self,
         dim_name: str = "__scalars",
         dtype: np.dtype = _DEFAULT_INDEX_DTYPE,
     ):
         """Adds a new TileDB dimension for NetCDF scalar variables.
 
-        Parameters:
-            dim_name: Output name of the dimension.
-            dtype: Numpy type to use for the scalar dimension
+        Parameters
+        ----------
+        dim_name
+            Output name of the dimension.
+        dtype
+            Numpy type to use for the scalar dimension
         """
         NetCDF4ScalarToDimConverter.create(
-            dataspace_registry=self._registry, dim_name=dim_name, dtype=dtype
+            registry=self._domain, dim_name=dim_name, dtype=dtype
         )
 
     def add_var_to_attr_converter(
         self,
         ncvar: netCDF4.Variable,
         array_name: str,
         attr_name: Optional[str] = None,
@@ -561,32 +619,42 @@
         unpack: bool = False,
     ):
         """Adds a new variable to attribute converter to an array in the CF dataspace.
 
         The attribute's 'dataspace name' (name after dropping the suffix ``.data`` or
         ``.index``) must be unique.
 
-        Parameters:
-            ncvar: NetCDF variable to convert to a TileDB attribute.
-            name: Name of the new attribute that will be added. If ``None``, the name
-                will be copied from the NetCDF variable.
-            dtype: Numpy dtype of the new attribute. If ``None``, the data type will be
-                copied from the variable.
-            fill: Fill value for unset cells. If ``None``, the fill value will be
-                copied from the NetCDF variable if it has a fill value.
-            var: Specifies if the attribute is variable length (automatic for
-                byte/strings).
-            nullable: Specifies if the attribute is nullable using validity tiles.
-            filters: Specifies compression filters for the attribute.
-            unpack: Unpack NetCDF data that has NetCDF attributes ``scale_factor`` or
-                ``add_offset`` using the transformation ``scale_factor * value +
-                unpack``.
+        Parameters
+        ----------
+        ncvar
+            NetCDF variable to convert to a TileDB attribute.
+        array_name
+            Name of the array the attribute is stored in.
+        attr_name
+            Name of the new attribute that will be added. If ``None``, the name
+            will be copied from the NetCDF variable.
+        dtype
+            Numpy dtype of the new attribute. If ``None``, the data type will be
+            copied from the variable.
+        fill
+            Fill value for unset cells. If ``None``, the fill value will be
+            copied from the NetCDF variable if it has a fill value.
+        var
+            Specifies if the attribute is variable length (automatic for
+            byte/strings).
+        nullable
+            Specifies if the attribute is nullable using validity tiles.
+        filters
+            Specifies compression filters for the attribute.
+        unpack
+            Unpack NetCDF data that has NetCDF attributes ``scale_factor`` or
+            ``add_offset`` using the transformation ``scale_factor * value + unpack``.
         """
         try:
-            array_creator = self._registry.get_array_creator(array_name)
+            array_creator = self._core.get_array_creator(array_name)
         except KeyError as err:  # pragma: no cover
             raise KeyError(
                 f"Cannot add attribute to array '{array_name}'. No array named "
                 f"'{array_name}' exists."
             ) from err
         array_creator.add_var_to_attr_converter(
             ncvar=ncvar,
@@ -611,32 +679,42 @@
         assigned_dim_values: Optional[Dict[str, Any]] = None,
         assigned_attr_values: Optional[Dict[str, np.ndarray]] = None,
         copy_metadata: bool = True,
     ):
         """Creates a TileDB arrays for a CF dataspace with only one array and copies
         data into it using the NetCDF converter engine.
 
-        Parameters:
-            output_uri: Uniform resource identifier for the TileDB array to be created.
-            key: If not ``None``, encryption key to encrypt and decrypt output arrays.
-            ctx: If not ``None``, TileDB context wrapper for a TileDB storage manager.
-            timestamp: If not ``None``, the TileDB timestamp to write the NetCDF data to
-                TileDB at.
-            input_netcdf_group: If not ``None``, the NetCDF group to copy data from.
-                This will be prioritized over ``input_file`` if both are provided.
-            input_file: If not ``None``, the NetCDF file to copy data from. This will
-                not be used if ``netcdf_group`` is not ``None``.
-            input_group_path: If not ``None``, the path to the NetCDF group to copy data
-                from.
-            assigned_dim_values: Mapping from dimension name to value for dimensions
-                that are not converter from the NetCDF group.
-            assigned_attr_values: Mapping from attribute name to numpy array of values
-                for attributes that are not converted from the NetCDF group.
-            copy_metadata: If  ``True`` copy NetCDF group and variable attributes to
-                TileDB metadata. If ``False`` do not copy metadata.
+        Parameters
+        ----------
+        output_uri
+            Uniform resource identifier for the TileDB array to be created.
+        key
+            If not ``None``, encryption key to encrypt and decrypt output arrays.
+        ctx
+            If not ``None``, TileDB context wrapper for a TileDB storage manager.
+        timestamp
+            If not ``None``, the TileDB timestamp to write the NetCDF data to
+            TileDB at.
+        input_netcdf_group
+            If not ``None``, the NetCDF group to copy data from. This will be
+            prioritized over ``input_file`` if both are provided.
+        input_file
+            If not ``None``, the NetCDF file to copy data from. This will not be used
+            if ``netcdf_group`` is not ``None``.
+        input_group_path
+            If not ``None``, the path to the NetCDF group to copy data from.
+        assigned_dim_values
+            Mapping from dimension name to value for dimensions that are not converter
+            from the NetCDF group.
+        assigned_attr_values
+            Mapping from attribute name to numpy array of values for attributes that
+            are not converted from the NetCDF group.
+        copy_metadata
+            If  ``True`` copy NetCDF group and variable attributes to TileDB metadata.
+            If ``False`` do not copy metadata.
         """
         self.create_array(output_uri, key, ctx)
         self.copy_to_array(
             output_uri=output_uri,
             key=key,
             ctx=ctx,
             timestamp=timestamp,
@@ -661,35 +739,45 @@
         assigned_attr_values: Optional[Dict[str, np.ndarray]] = None,
         copy_metadata: bool = True,
         append: bool = False,
     ):
         """Creates a TileDB group and its arrays from the defined CF dataspace and
         copies data into them using the converter engine.
 
-        Parameters:
-            output_uri: Uniform resource identifier for the TileDB group to be created.
-            key: If not ``None``, encryption key to encrypt and decrypt output arrays.
-            ctx: If not ``None``, TileDB context wrapper for a TileDB storage manager.
-            timestamp: If not ``None``, the TileDB timestamp to write the NetCDF data to
-                TileDB at.
-            input_netcdf_group: If not ``None``, the NetCDF group to copy data from.
-                This will be prioritized over ``input_file`` if both are provided.
-            input_file: If not ``None``, the NetCDF file to copy data from. This will
-                not be used if ``netcdf_group`` is not ``None``.
-            input_group_path: If not ``None``, the path to the NetCDF group to copy data
-                from.
-            assigned_dim_values: Mapping from dimension name to value for dimensions
-                that are not converted from the NetCDF group.
-            assigned_attr_values: Mapping from attribute name to numpy array of values
-                for attributes that are not converted from the NetCDF group.
-            copy_metadata: If  ``True`` copy NetCDF group and variable attributes to
-                TileDB metadata. If ``False`` do not copy metadata.
-            append: If ``True``, add arrays in the dataspace to an already existing
-                group. The arrays in the dataspace cannot be in the group that is being
-                append to.
+        Parameters
+        ----------
+        output_uri
+            Uniform resource identifier for the TileDB group to be created.
+        key
+            If not ``None``, encryption key to encrypt and decrypt output arrays.
+        ctx
+            If not ``None``, TileDB context wrapper for a TileDB storage manager.
+        timestamp
+            If not ``None``, the TileDB timestamp to write the NetCDF data to
+            TileDB at.
+        input_netcdf_group
+            If not ``None``, the NetCDF group to copy data from. This will be
+            prioritized over ``input_file`` if both are provided.
+        input_file
+            If not ``None``, the NetCDF file to copy data from. This will not be used
+            if ``netcdf_group`` is not ``None``.
+        input_group_path
+            If not ``None``, the path to the NetCDF group to copy data from.
+        assigned_dim_values
+            Mapping from dimension name to value for dimensions that are not converted
+            from the NetCDF group.
+        assigned_attr_values
+            Mapping from attribute name to numpy array of values for attributes that
+            are not converted from the NetCDF group.
+        copy_metadata
+            If  ``True`` copy NetCDF group and variable attributes to TileDB metadata.
+            If ``False`` do not copy metadata.
+        append
+            If ``True``, add arrays in the dataspace to an already existing group. The
+            arrays in the dataspace cannot be in the group that is being append to.
         """
         self.create_group(output_uri, key, ctx, append=append)
         self.copy_to_group(
             output_uri=output_uri,
             key=key,
             ctx=ctx,
             input_netcdf_group=input_netcdf_group,
@@ -712,47 +800,55 @@
         assigned_dim_values: Optional[Dict[str, Any]] = None,
         assigned_attr_values: Optional[Dict[str, np.ndarray]] = None,
         copy_metadata: bool = True,
     ):
         """Copies data from a NetCDF group to a TileDB array.
 
         This will copy data from a NetCDF group that is defined either by a
-        :class:`netCDF4.Group` or by an input_file and group path. If neither the
+        ``netCDF4.Group`` or by an input_file and group path. If neither the
         ``netcdf_group`` or ``input_file`` is specified, this will copy data from the
         input file ``self.default_input_file``.  If both ``netcdf_group`` and
         ``input_file`` are set, this method will prioritize using the NetCDF group set
         by ``netcdf_group``.
 
-        Parameters:
-            output_uri: Uniform resource identifier for the TileDB array data is being
-                copied to.
-            key: If not ``None``, encryption key to decrypt arrays.
-            ctx: If not ``None``, TileDB context wrapper for a TileDB storage manager.
-            timestamp: If not ``None``, the TileDB timestamp to write the NetCDF data to
-                TileDB at.
-            input_netcdf_group: If not ``None``, the NetCDF group to copy data from.
-                This will be prioritized over ``input_file`` if both are provided.
-            input_file: If not ``None``, the NetCDF file to copy data from. This will
-                not be used if ``netcdf_group`` is not ``None``.
-            input_group_path: If not ``None``, the path to the NetCDF group to copy data
-                from.
-            assigned_dim_values: Mapping from dimension name to value for dimensions
-                that are not copied from the NetCDF group.
-            assigned_attr_values: Mapping from attribute name to numpy array of values
-                for attributes that are not copied from the NetCDF group.
-            copy_metadata: If  ``True`` copy NetCDF group and variable attributes to
-                TileDB metadata. If ``False`` do not copy metadata.
+        Parameters
+        ----------
+        output_uri
+            Uniform resource identifier for the TileDB array data is being copied to.
+        key
+            If not ``None``, encryption key to decrypt arrays.
+        ctx
+            If not ``None``, TileDB context wrapper for a TileDB storage manager.
+        timestamp
+            If not ``None``, the TileDB timestamp to write the NetCDF data to TileDB at.
+        input_netcdf_group
+            If not ``None``, the NetCDF group to copy data from. This will be
+            prioritized over ``input_file`` if both are provided.
+        input_file
+            If not ``None``, the NetCDF file to copy data from. This will not be used
+            if ``netcdf_group`` is not ``None``.
+        input_group_path
+            If not ``None``, the path to the NetCDF group to copy data from.
+        assigned_dim_values
+            Mapping from dimension name to value for dimensions that are not copied
+            from the NetCDF group.
+        assigned_attr_values
+            Mapping from attribute name to numpy array of values for attributes that
+            are not copied from the NetCDF group.
+        copy_metadata
+            If  ``True`` copy NetCDF group and variable attributes to TileDB metadata.
+            If ``False`` do not copy metadata.
         """
-        if self._registry.narray != 1:  # pragma: no cover
+        if self._core.narray != 1:  # pragma: no cover
             raise ValueError(
                 f"Can only use `copy_to_array` for a {self.__class__.__name__} with "
                 f"exactly 1 array creator. This {self.__class__.__name__} contains "
-                f"{self._registry.narray} array creators."
+                f"{self._core.narray} array creators."
             )
-        array_creator = next(self._registry.array_creators())
+        array_creator = next(self._core.array_creators())
         if input_netcdf_group is None:
             input_file = (
                 input_file if input_file is not None else self.default_input_file
             )
             input_group_path = (
                 input_group_path
                 if input_group_path is not None
@@ -790,47 +886,55 @@
         assigned_dim_values: Optional[Dict[str, Any]] = None,
         assigned_attr_values: Optional[Dict[str, np.ndarray]] = None,
         copy_metadata: bool = True,
     ):
         """Copies data from a NetCDF group to a TileDB CF dataspace.
 
         This will copy data from a NetCDF group that is defined either by a
-        :class:`netCDF4.Group` or by an input_file and group path. If neither the
+        ``netCDF4.Group`` or by an input_file and group path. If neither the
         ``netcdf_group`` or ``input_file`` is specified, this will copy data from the
         input file ``self.default_input_file``.  If both ``netcdf_group`` and
         ``input_file`` are set, this method will prioritize using the NetCDF group set
         by ``netcdf_group``.
 
-        Parameters:
-            output_uri: Uniform resource identifier for the TileDB group data is being
-                copied to.
-            key: If not ``None``, encryption key to decrypt arrays.
-            ctx: If not ``None``, TileDB context wrapper for a TileDB storage manager.
-            timestamp: If not ``None``, the TileDB timestamp to write the NetCDF data to
-                TileDB at.
-            input_netcdf_group: If not ``None``, the NetCDF group to copy data from.
-                This will be prioritized over ``input_file`` if both are provided.
-            input_file: If not ``None``, the NetCDF file to copy data from. This will
-                not be used if ``netcdf_group`` is not ``None``.
-            input_group_path: If not ``None``, the path to the NetCDF group to copy data
-                from.
-            assigned_dim_values: Mapping from dimension name to value for dimensions
-                that are not copied from the NetCDF group.
-            assigned_attr_values: Mapping from attribute name to numpy array of values
-                for the attributes that are not copied from the NetCDF group.
-            copy_metadata: If  ``True`` copy NetCDF group and variable attributes to
-                TileDB metadata. If ``False`` do not copy metadata.
+        Parameters
+        ----------
+        output_uri
+            Uniform resource identifier for the TileDB group data is being copied to.
+        key
+            If not ``None``, encryption key to decrypt arrays.
+        ctx
+            If not ``None``, TileDB context wrapper for a TileDB storage manager.
+        timestamp
+            If not ``None``, the TileDB timestamp to write the NetCDF data to TileDB at.
+        input_netcdf_group
+            If not ``None``, the NetCDF group to copy data from. This will be
+            prioritized over ``input_file`` if both are provided.
+        input_file
+            If not ``None``, the NetCDF file to copy data from. This will not be used
+            if ``netcdf_group`` is not ``None``.
+        input_group_path
+            If not ``None``, the path to the NetCDF group to copy data from.
+        assigned_dim_values
+            Mapping from dimension name to value for dimensions that are not copied
+            from the NetCDF group.
+        assigned_attr_values
+            Mapping from attribute name to numpy array of values for the attributes
+            that are not copied from the NetCDF group.
+        copy_metadata
+            If  ``True`` copy NetCDF group and variable attributes to TileDB metadata.
+            If ``False`` do not copy metadata.
         """
         if copy_metadata and timestamp is not None:
             raise NotImplementedError(
                 "Writing group metadata at a timestamp is not yet supported."
             )
         array_uris = {
             array_creator.name: os.path.join(output_uri, array_creator.name)
-            for array_creator in self._registry.array_creators()
+            for array_creator in self._core.array_creators()
         }
         if input_netcdf_group is None:
             input_file = (
                 input_file if input_file is not None else self.default_input_file
             )
             input_group_path = (
                 input_group_path
@@ -839,15 +943,15 @@
             )
         with open_netcdf_group(
             input_netcdf_group, input_file, input_group_path
         ) as netcdf_group:
             if copy_metadata:
                 with tiledb.Group(output_uri, mode="w", ctx=ctx) as group:
                     copy_group_metadata(netcdf_group, group.meta)
-            for array_creator in self._registry.array_creators():
+            for array_creator in self._core.array_creators():
                 if isinstance(array_creator, NetCDF4ArrayConverter):
                     array_creator.copy(
                         netcdf_group=netcdf_group,
                         tiledb_uri=array_uris[array_creator.name],
                         tiledb_key=key,
                         tiledb_ctx=ctx,
                         tiledb_timestamp=timestamp,
```

### Comparing `tiledb-cf-0.9.0/tiledb/cf/xarray_engine/_array_wrapper.py` & `tiledb-cf-0.9.1/tiledb/cf/xarray_engine/_array_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,26 +17,26 @@
        * An integer index or component of an array is such that -size <= value < size.
          * Non-negative values are a standard zero-based index.
          * Negative values count backwards from the end of the array with the last value
            of the array starting at -1.
 
     Parameters
     ----------
-    dim_name: int
+    dim_name
         Name of the dimension. Used for errors.
-    dim_size: int
+    dim_size
         Size of the dimension as interpreted by xarray. May be smaller than the
         full domain of the TileDB dimension.
-    index : Union[int, np.array, slice]
+    index
         An integer index, array of integer indices, or a slice for indexing an
         xarray dimension.
 
     Returns
     -------
-    new_index : Union[int, List[int], slice]
+    Union[int, List[int], slice]
         An integer, a list of integer values, or a slice for indexing a
         TileDB dimension using mulit_index.
     """
     if np.isscalar(index):
         # Convert xarray index to TileDB dimension coordinate
         if not -dim_size <= index < dim_size:
             raise IndexError(
```

### Comparing `tiledb-cf-0.9.0/tiledb/cf/xarray_engine/_backend_store.py` & `tiledb-cf-0.9.1/tiledb/cf/xarray_engine/_backend_store.py`

 * *Files identical despite different names*

### Comparing `tiledb-cf-0.9.0/tiledb/cf/xarray_engine/_deprecated_backend_store.py` & `tiledb-cf-0.9.1/tiledb/cf/xarray_engine/_deprecated_backend_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,19 +15,26 @@
 
 from collections import defaultdict
 from typing import Tuple
 
 import numpy as np
 from xarray.backends.common import AbstractDataStore, BackendArray
 from xarray.core.indexing import ExplicitIndexer, LazilyIndexedArray
-from xarray.core.pycompat import integer_types
+
 from xarray.core.utils import FrozenDict
 from xarray.core.variable import Variable
 
 try:
+    # handle https://github.com/TileDB-Inc/TileDB-CF-Py/issues/152#issuecomment-2035080835
+    # - https://github.com/pydata/xarray/commit/d64460795e406bc4a998e2ddae0054a1029d52a9
+    from xarray.core.pycompat import integer_types
+except ImportError:
+    from xarray.namedarray.pycompat import integer_types
+
+try:
     import tiledb
 
     has_tiledb = True
 except ModuleNotFoundError:
     has_tiledb = False
 
 _ATTR_PREFIX = "__tiledb_attr."
```

### Comparing `tiledb-cf-0.9.0/tiledb/cf/xarray_engine/_encoding.py` & `tiledb-cf-0.9.1/tiledb/cf/xarray_engine/_encoding.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,34 +11,39 @@
 _ATTR_FILTERS_ENCODING = "filters"
 _TILE_SIZES_ENCODING = "tiles"
 _MAX_SHAPE_ENCODING = "max_shape"
 _DIM_DTYPE_ENCODING = "dim_dtype"
 
 
 class TileDBVariableEncoder:
+    """Class for encoding array variables.
+
+    Parameters
+    ----------
+    name
+        Name of the variable.
+    variable
+        Xarray variable to encode.
+    encoding
+        Dictionary of TileDB encoding keywords.
+    unlimited_dims
+        Unlimited dimensions. Only used if max_shape is not provided in the encoding.
+    ctx
+        Context object for TileDB operations.
+    """
+
     valid_encoding_keys = {
         _ATTR_FILTERS_ENCODING,
         _ATTR_NAME_ENCODING,
         _DIM_DTYPE_ENCODING,
         _MAX_SHAPE_ENCODING,
         _TILE_SIZES_ENCODING,
     }
 
     def __init__(self, name, variable, encoding, unlimited_dims, ctx):
-        """Creates a class for encoding xarray variables.
-
-        Parameters:
-        -----------
-        name: Name of the variable.
-        variable: Xarray variable to encode.
-        encoding: Dictionary of TileDB encoding keywords.
-        unlimited_dims: Unlimited dimensions. Only used if max_shape is not provided
-            in the encoding.
-        ctx: Context object for TileDB operations.
-        """
         # Set initial class properties.
         self._ctx = ctx
         self._name = name
         self._variable = variable
         self._encoding = dict()
 
         # Check the input encoding data is valid.
```

### Comparing `tiledb-cf-0.9.0/tiledb/cf/xarray_engine/_writer.py` & `tiledb-cf-0.9.1/tiledb/cf/xarray_engine/_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,28 +25,38 @@
     copy_variable_metadata: bool,
     copy_variable_data: bool,
 ):
     """Copies data and metadata from an xarray dataset to a TileDB group corresponding
     to the dataset.
 
 
-    Parameters:
-    -----------
-    group_uri: The URI to the TileDB group to create or append to.
-    dataset: The xarray Dataset to write.
-    variables: A mapping of encoded xarray variables.
-    group_metadata: A mapping of key-value pairs correspoding to dataset metadata.
-    config: A TileDB config object to use for TileDB objects.
-    ctx: A TileDB context object to use for TileDB operations.
-    region: A mapping from dimension names to integer slices along the
-        dataset dimensions to indicate the region to write this dataset's data in.
-    copy_group_metadata: If true, copy xarray dataset metadata to the TileDB group.
-    copy_variable_metadata: If true, copy xarray variable metadata to the TileDB
-        arrays as TileDB attribute metadata.
-    copy_variable_data: If true, copy variable data to the TileDB arrays.
+    Parameters
+    ----------
+    group_uri
+        The URI to the TileDB group to create or append to.
+    dataset
+        The xarray Dataset to write.
+    variables
+        A mapping of encoded xarray variables.
+    group_metadata
+        A mapping of key-value pairs correspoding to dataset metadata.
+    config
+        A TileDB config object to use for TileDB objects.
+    ctx
+        A TileDB context object to use for TileDB operations.
+    region
+        A mapping from dimension names to integer slices along thevdataset dimensions
+        to indicate the region to write this dataset's data in.
+    copy_group_metadata
+        If true, copy xarray dataset metadata to the TileDB group.
+    copy_variable_metadata
+        If true, copy xarray variable metadata to the TileDBvarrays as TileDB attribute
+        metadata.
+    copy_variable_data
+        If true, copy variable data to the TileDB arrays.
     """
 
     # Check that there is a group at the location.
     check_valid_group(group_uri, ctx)
 
     # Check the region input is valid.
     region = dict() if region is None else region
@@ -138,17 +148,22 @@
     # Get the target region to write the data into.
     def get_dimension_slice(dim_name, var_dim_size, array_dim_size):
         """Returns target dimension slice for xarray write.
 
         Raises a value error if the size of the target slice does not match the
         size of the source dimension.
 
-        dim_name: Name of the dimension to return the slice for.
-        var_dim_size: Size of the dimension in the source xarray variable.
-        array_dim_size: Size of the domain of the dimension in the target TileDB array.
+        Parameters
+        ----------
+        dim_name
+            Name of the dimension to return the slice for.
+        var_dim_size
+            Size of the dimension in the source xarray variable.
+        array_dim_size
+            Size of the domain of the dimension in the target TileDB array.
         """
         if var_dim_size > array_dim_size:
             raise ValueError(
                 f"Cannot write variable '{name}' with shape {variable.shape} on a "
                 f"TileDB array with maximum shape {array_wrapper.shape}."
             )
         if dim_name not in region:
@@ -211,27 +226,36 @@
     append: bool,
     encoding: Optional[Mapping[str, Any]],
     unlimited_dims: Optional[Iterable[str]],
 ):
     """Creates a TileDB group and arrays from a xarray dataset and optionally copies
     metadata over.
 
-    Parameters:
+    Parameters
     ----------
-    dataset: The xarray Dataset to write.
-    group_uri: The URI to the TileDB group to create or append to.
-    variables: A mapping of encoded xarray variables.
-    config: A TileDB config object to use for TileDB objects.
-    ctx: A TileDB context object to use for TileDB operations.
-    encoding: A nested dictionary with variable names as keys and dictionaries
-        of TileDB specific encoding.
-    unlimited_dims: Set of dimensions to use the maximum dimension size for. Only used
-        for variables in the dataset that do not have `max_size` encoding provided.
-    config: TileDB configuration to use for writing metadata to groups and arrays.
-    ctx: Context object to use for TileDB operations.
+    dataset
+        The xarray Dataset to write.
+    group_uri
+        The URI to the TileDB group to create or append to.
+    variables
+        A mapping of encoded xarray variables.
+    config
+        A TileDB config object to use for TileDB objects.
+    ctx
+        A TileDB context object to use for TileDB operations.
+    encoding
+        A nested dictionary with variable names as keys and dictionaries of TileDB
+        specific encoding.
+    unlimited_dims
+        Set of dimensions to use the maximum dimension size for. Only used for variables
+        in the dataset that do not have `max_size` encoding provided.
+    config
+        TileDB configuration to use for writing metadata to groups and arrays.
+    ctx
+        Context object to use for TileDB operations.
     """
 
     # Check the TileDB encoding is for valid variables.
     encoding = dict() if encoding is None else encoding
     for var_name in encoding:
         if var_name not in variables:
             raise KeyError(
@@ -282,16 +306,20 @@
                 group.meta[key] = value
 
 
 def extract_encoded_data(dataset, skip_vars=None):
     """Returns encoded xarray variables and attribtues (metadata) from an
     input xarray dataset.
 
-    dataset: Xarray dataset to encode.
-    skip_vars: Variables to exclude if they exist in the dataset
+    Parameters
+    ----------
+    dataset
+        Xarray dataset to encode.
+    skip_vars
+        Variables to exclude if they exist in the dataset
     """
 
     if skip_vars is None:
         skip_vars = set()
 
     # Get variables and apply xarray encoders.
     variables, group_metadata = encode_dataset_coordinates(dataset)
@@ -317,24 +345,30 @@
     target_region: Tuple[slice, ...],
     source_shape: Tuple[int, ...],
     chunks: Optional[Tuple[Tuple[int, ...], ...]],
 ) -> Generator[Tuple[Tuple[slice, ...], Tuple[slice, ...]], None, None]:
     """Returns a generator of (target_region, source_region) for writing the
     input source by chunks.
 
-    Parameters:
+    Parameters
     ----------
-    target_region: Slices that correspond to the target region to query using
+    target_region
+        Slices that correspond to the target region to query using
         numpy-style indexing.
-    source_shape: Shape of the input data.
-    chunks: A tuple or tuples containing the fully explicit size of chunks along each
+    source_shape
+        Shape of the input data.
+    chunks
+        A tuple or tuples containing the fully explicit size of chunks along each
         dimension.
 
-    Yields tuples of (target_chunk, source_chunk) pairs that cover the entire target
-    and source regions.
+    Yields
+    ------
+    Tuple[Tuple[slice, ...], Tuple[slice, ....]] or None
+        Yields tuples of (target_chunk, source_chunk) pairs that cover the entire target
+        and source regions.
     """
 
     # Return a single (target region, source region ) pair for a non-chunked array.
     if chunks is None:
         source_region = tuple(len(source_shape) * [slice(None)])
         yield (target_region, source_region)
```

### Comparing `tiledb-cf-0.9.0/tiledb/cf/xarray_engine/api.py` & `tiledb-cf-0.9.1/tiledb/cf/xarray_engine/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,31 +17,40 @@
     copy_group_metadata: bool = True,
     copy_variable_metadata: bool = True,
 ):
     """Creates a TileDB group and arrays from an xarray dataset.
 
     Optionally copies metadata as well.
 
-    Parameters:
-        dataset: The xarray Dataset to write.
-        group_uri: The URI to the TileDB group to create or append to.
-        config: A TileDB config object to use for TileDB objects.
-        ctx: A TileDB context object to use for TileDB operations.
-        append: If true, add arrays to an existing TileDB Group. Otherwise,
-            create a new TileDB group to add arrays to.
-        encoding: A nested dictionary with variable names as keys and dictionaries
-            of TileDB specific encodings as values.
-        unlimited_dims: Set of dimensions to use the maximum dimension size for. Only
-            used for variables in the dataset that do not have ``max_size`` encoding
-            provided.
-        skip_vars: A set of names of variables not to add to the TileDB group.
-        copy_group_metadata: If true, copy xarray dataset metadata to the TileDB group.
-        copy_variable_metadata: If true, copy xarray variable metadata to the TileDB
-            arrays as TileDB attribute metadata.
-
+    Parameters
+    ----------
+    dataset
+        The xarray Dataset to write.
+    group_uri
+        The URI to the TileDB group to create or append to.
+    config
+        A TileDB config object to use for TileDB objects.
+    ctx
+        A TileDB context object to use for TileDB operations.
+    append
+        If true, add arrays to an existing TileDB Group. Otherwise, create a new TileDB
+        group to add arrays to.
+    encoding
+        A nested dictionary with variable names as keys and dictionaries of TileDB
+        specific encodings as values.
+    unlimited_dims
+        Set of dimensions to use the maximum dimension size for. Only used for
+        variables in the dataset that do not have ``max_size`` encoding provided.
+    skip_vars
+        A set of names of variables not to add to the TileDB group.
+    copy_group_metadata
+        If true, copy xarray dataset metadata to the TileDB group.
+    copy_variable_metadata
+        If true, copy xarray variable metadata to the TileDB arrays as TileDB attribute
+        metadata.
     """
 
     from ._writer import copy_from_xarray, create_from_xarray, extract_encoded_data
 
     # Splits dataset into variables and group-level metadata using the CF Convention
     # where possible.
     variables, group_metadata = extract_encoded_data(dataset, skip_vars=skip_vars)
@@ -85,27 +94,35 @@
     copy_group_metadata=False,
     copy_variable_metadata=False,
 ):
     """Copies data from an xarray dataset to a TileDB group.
 
     Optionally copies metadata as well as variable data.
 
-    Parameters:
-        dataset: The xarray Dataset to write.
-        group_uri: The URI to the TileDB group to create or append to.
-        config: A TileDB config object to use for TileDB objects.
-        ctx: A TileDB context object to use for TileDB operations.
-        region: A mapping from dimension names to integer slices that specify what
-            regions in the TileDB arrays to write the data. Regions include the first
-            value of the slice and exclude the final value.
-        skip_vars: A set of names of variables not to copy to the TileDB group.
-        copy_group_metadata: If true, copy xarray dataset metadata to the TileDB group.
-        copy_variable_metadata: If true, copy xarray variable metadata to the TileDB
-            arrays as TileDB attribute metadata.
-
+    Parameters
+    ----------
+    dataset
+        The xarray Dataset to write.
+    group_uri
+        The URI to the TileDB group to create or append to.
+    config
+        A TileDB config object to use for TileDB objects.
+    ctx
+        A TileDB context object to use for TileDB operations.
+    region
+        A mapping from dimension names to integer slices that specify what regions in
+        the TileDB arrays to write the data. Regions include the first value of the
+        slice and exclude the final value.
+    skip_vars
+        A set of names of variables not to copy to the TileDB group.
+    copy_group_metadata
+        If true, copy xarray dataset metadata to the TileDB group.
+    copy_variable_metadata
+        If true, copy xarray variable metadata to the TileDB arrays as TileDB
+        attribute metadata.
     """
 
     from ._writer import copy_from_xarray, extract_encoded_data
 
     # Splits dataset into variables and group-level metadata using the CF Convention
     # where possible.
     variables, group_metadata = extract_encoded_data(dataset, skip_vars)
@@ -133,25 +150,31 @@
     ctx: Optional[tiledb.Ctx] = None,
     skip_vars: Optional[Set[str]] = None,
     copy_group_metadata: bool = True,
     copy_variable_metadata: bool = True,
 ):
     """Copies metadata from an xarray dataset to a TileDB group.
 
-    Parameters:
-        dataset: The xarray Dataset to write.
-        group_uri: The URI to the TileDB group to create or append to.
-        config: A TileDB config object to use for TileDB objects.
-        ctx: A TileDB context object to use for TileDB operations.
-        skip_vars: A set of names of variables not to copy to the group.
-        copy_group_metadata: If true, copy xarray dataset metadata to the TileDB
-            group.
-        copy_variable_metadata: If true, copy xarray variable metadata to the TileDB
-            arrays as TileDB attribute metadata.
-
+    Parameters
+    ----------
+    dataset
+        The xarray Dataset to write.
+    group_uri
+        The URI to the TileDB group to create or append to.
+    config
+        A TileDB config object to use for TileDB objects.
+    ctx
+        A TileDB context object to use for TileDB operations.
+    skip_vars
+        A set of names of variables not to copy to the group.
+    copy_group_metadata
+        If true, copy xarray dataset metadata to the TileDB group.
+    copy_variable_metadata
+        If true, copy xarray variable metadata to the TileDB arrays as TileDB
+        attribute metadata.
     """
 
     from ._writer import copy_from_xarray, extract_encoded_data
 
     # Splits dataset into variables and group-level metadata using the CF Convention
     # where possible.
     variables, group_metadata = extract_encoded_data(dataset, skip_vars)
@@ -180,31 +203,39 @@
     encoding: Optional[Mapping[str, Any]] = None,
     region: Optional[Mapping[str, slice]] = None,
     unlimited_dims: Optional[Iterable[str]] = None,
     skip_vars: Optional[Set[str]] = None,
 ):
     """Creates a TileDB group and copies all data from an xarray dataset.
 
-    Parameters:
-        dataset: The xarray Dataset to write.
-        group_uri: The URI to the TileDB group to create or append to.
-        config: A TileDB config object to use for TileDB objects.
-        ctx: A TileDB context object to use for TileDB operations.
-            encoding: A nested dictionary with variable names as keys and dictionaries
-            of TileDB specific encoding.
-        encoding: A nested dictionary with variable names as keys and dictionaries
-            of TileDB specific encodings as values.
-        region: A mapping from dimension names to integer slices that specify what
-            regions in the TileDB arrays to write the data. Regions include the first
-            value of the slice and exclude the final value.
-        unlimited_dims: Set of dimensions to use the maximum dimension size for. Only
-            used for variables in the dataset that do not have `max_size` encoding
-            provided.
-        skip_vars: A set of names of variables not to add to the TileDB group.
-
+    Parameters
+    ----------
+    dataset
+        The xarray Dataset to write.
+    group_uri
+        The URI to the TileDB group to create or append to.
+    config
+        A TileDB config object to use for TileDB objects.
+    ctx
+        A TileDB context object to use for TileDB operations.
+    encoding
+        A nested dictionary with variable names as keys and dictionaries of TileDB
+        specific encoding.
+    encoding
+        A nested dictionary with variable names as keys and dictionaries of TileDB
+        specific encodings as values.
+    region
+        A mapping from dimension names to integer slices that specify what regions in
+        the TileDB arrays to write the data. Regions include the first value of the
+        slice and exclude the final value.
+    unlimited_dims
+        Set of dimensions to use the maximum dimension size for. Only used for variables
+        in the dataset that do not have `max_size` encoding provided.
+    skip_vars
+        A set of names of variables not to add to the TileDB group.
     """
     from ._writer import copy_from_xarray, create_from_xarray, extract_encoded_data
 
     # Splits dataset into variables and group-level metadata using the CF Convention
     # where possible.
     variables, group_metadata = extract_encoded_data(dataset, skip_vars)
```

### Comparing `tiledb-cf-0.9.0/tiledb/cf/xarray_engine/engine.py` & `tiledb-cf-0.9.1/tiledb/cf/xarray_engine/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,36 +64,49 @@
         decode_timedelta=None,
     ) -> Dataset:
         """
         Open a TileDB group or array as an xarray dataset.
 
         Parameters
         ----------
-        filename_or_obj: TileDB URI for the group or array to open in xarray.
-        config: TileDB config object to pass to TileDB objects.
-        ctx: TileDB context to use for TileDB operations.
-        timestamp: Timestamp to open the TileDB array at. Not valid for groups.
-        key: [Deprecated] Encryption key to use for the backend array.
-        encode_fill: [Deprecated] Encode the TileDB fill value.
-        coord_dims: [Deprecated] List of dimensions to convert to coordinates.
-        open_full_domain: [Deprecated] Open the full TileDB domain instead of the
-            non-empty domain.
-        mask_and_scale: xarray decoder that masks fill value and applies float-scale
-            filter using variable metadata.
-        decode_times: xarray decoder that converts variables with NetCDF CF-Convention
-            time metadata to a numpy.datetime64 datatype.
-        concat_characters: xarray decoder not supported by TileDB.
-        decode_coords: xarray decoder that controls which variables are set as
-            coordinate variables.
-        drop_variables: A variable or list of variables to exclude from being
-            parase from the dataset.
-        use_cftime: xarray decoder option. Uses cftime for datetime decoding.
-        decode_timedelta: xarray decoder that converts variables with time units
-            to a numpy.timedelta64 datatype.
-
+        filename_or_obj
+            TileDB URI for the group or array to open in xarray.
+        config
+            TileDB config object to pass to TileDB objects.
+        ctx
+            TileDB context to use for TileDB operations.
+        timestamp
+            Timestamp to open the TileDB array at. Not valid for groups.
+        key
+            [Deprecated] Encryption key to use for the backend array.
+        encode_fill
+            [Deprecated] Encode the TileDB fill value.
+        coord_dims
+            [Deprecated] List of dimensions to convert to coordinates.
+        open_full_domain
+            [Deprecated] Open the full TileDB domain instead of the non-empty domain.
+        mask_and_scale
+            xarray decoder that masks fill value and applies float-scale filter using
+            variable metadata.
+        decode_times
+            xarray decoder that converts variables with NetCDF CF-Convention time
+            metadata to a numpy.datetime64 datatype.
+        concat_characters
+            xarray decoder not supported by TileDB.
+        decode_coords
+            xarray decoder that controls which variables are set as coordinate
+            variables.
+        drop_variables
+            A variable or list of variables to exclude from being opened from the
+            dataset.
+        use_cftime
+            xarray decoder option. Uses cftime for datetime decoding.
+        decode_timedelta
+            xarray decoder that converts variables with time units to a
+            numpy.timedelta64 datatype.
         """
 
         deprecated_kwargs = {
             "key": key,
             "encode_fill": encode_fill,
             "open_full_domain": open_full_domain,
         }
```

### Comparing `tiledb-cf-0.9.0/tiledb_cf.egg-info/SOURCES.txt` & `tiledb-cf-0.9.1/tiledb_cf.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -3,18 +3,26 @@
 pyproject.toml
 setup.cfg
 setup.py
 tiledb/cf/__init__.py
 tiledb/cf/__main__.py
 tiledb/cf/_utils.py
 tiledb/cf/cli.py
+tiledb/cf/testing.py
 tiledb/cf/core/__init__.py
-tiledb/cf/core/_creator.py
+tiledb/cf/core/_array_creator.py
+tiledb/cf/core/_attr_creator.py
+tiledb/cf/core/_dataspace_creator.py
+tiledb/cf/core/_dim_creator.py
+tiledb/cf/core/_fragment_writer.py
 tiledb/cf/core/_metadata.py
+tiledb/cf/core/_shared_dim.py
 tiledb/cf/core/api.py
+tiledb/cf/core/registry.py
+tiledb/cf/core/source.py
 tiledb/cf/netcdf_engine/__init__.py
 tiledb/cf/netcdf_engine/_array_converters.py
 tiledb/cf/netcdf_engine/_attr_converters.py
 tiledb/cf/netcdf_engine/_dim_converters.py
 tiledb/cf/netcdf_engine/_utils.py
 tiledb/cf/netcdf_engine/api.py
 tiledb/cf/netcdf_engine/converter.py
```

