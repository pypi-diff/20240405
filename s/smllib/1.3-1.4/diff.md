# Comparing `tmp/smllib-1.3.tar.gz` & `tmp/smllib-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smllib-1.3.tar", last modified: Wed Oct 18 05:34:33 2023, max compression
+gzip compressed data, was "smllib-1.4.tar", last modified: Fri Apr  5 05:42:53 2024, max compression
```

## Comparing `smllib-1.3.tar` & `smllib-1.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 05:34:33.948305 smllib-1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-10-18 05:34:23.000000 smllib-1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-10-18 05:34:23.000000 smllib-1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6312 2023-10-18 05:34:33.948305 smllib-1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-18 05:34:33.948305 smllib-1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2023-10-18 05:34:23.000000 smllib-1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 05:34:33.940305 smllib-1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 05:34:33.944305 smllib-1.3/src/smllib/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2023-10-18 05:34:23.000000 smllib-1.3/src/smllib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-18 05:34:23.000000 smllib-1.3/src/smllib/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 05:34:33.944305 smllib-1.3/src/smllib/builder/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2023-10-18 05:34:23.000000 smllib-1.3/src/smllib/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2023-10-18 05:34:23.000000 smllib-1.3/src/smllib/builder/_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2023-10-18 05:34:23.000000 smllib-1.3/src/smllib/builder/default_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2023-10-18 05:34:23.000000 smllib-1.3/src/smllib/builder/list_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2023-10-18 05:34:23.000000 smllib-1.3/src/smllib/builder/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2023-10-18 05:34:23.000000 smllib-1.3/src/smllib/builder/response_get_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2023-10-18 05:34:23.000000 smllib-1.3/src/smllib/builder/response_open_close.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2023-10-18 05:34:23.000000 smllib-1.3/src/smllib/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2023-10-18 05:34:23.000000 smllib-1.3/src/smllib/crc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2023-10-18 05:34:23.000000 smllib-1.3/src/smllib/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-18 05:34:23.000000 smllib-1.3/src/smllib/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2023-10-18 05:34:23.000000 smllib-1.3/src/smllib/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 05:34:33.948305 smllib-1.3/src/smllib/sml/
--rw-r--r--   0 runner    (1001) docker     (127)      539 2023-10-18 05:34:23.000000 smllib-1.3/src/smllib/sml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2023-10-18 05:34:23.000000 smllib-1.3/src/smllib/sml/_base_obj.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2023-10-18 05:34:23.000000 smllib-1.3/src/smllib/sml/_field_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2023-10-18 05:34:23.000000 smllib-1.3/src/smllib/sml/list_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2023-10-18 05:34:23.000000 smllib-1.3/src/smllib/sml/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2023-10-18 05:34:23.000000 smllib-1.3/src/smllib/sml/response_get_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2023-10-18 05:34:23.000000 smllib-1.3/src/smllib/sml/response_open_close.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2023-10-18 05:34:23.000000 smllib-1.3/src/smllib/sml/sml_choice.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-10-18 05:34:23.000000 smllib-1.3/src/smllib/sml/sml_eom.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2023-10-18 05:34:23.000000 smllib-1.3/src/smllib/sml/sml_obis.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2023-10-18 05:34:23.000000 smllib-1.3/src/smllib/sml/sml_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2023-10-18 05:34:23.000000 smllib-1.3/src/smllib/sml_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-10-18 05:34:23.000000 smllib-1.3/src/smllib/sml_frame_snippet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 05:34:33.944305 smllib-1.3/src/smllib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6312 2023-10-18 05:34:33.000000 smllib-1.3/src/smllib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2023-10-18 05:34:33.000000 smllib-1.3/src/smllib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-18 05:34:33.000000 smllib-1.3/src/smllib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-18 05:34:33.000000 smllib-1.3/src/smllib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 05:34:33.948305 smllib-1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2023-10-18 05:34:23.000000 smllib-1.3/tests/test_crc.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-10-18 05:34:23.000000 smllib-1.3/tests/test_frame_snipped.py
--rw-r--r--   0 runner    (1001) docker     (127)     9445 2023-10-18 05:34:23.000000 smllib-1.3/tests/test_frames.py
--rw-r--r--   0 runner    (1001) docker     (127)     6257 2023-10-18 05:34:23.000000 smllib-1.3/tests/test_sml_data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2023-10-18 05:34:23.000000 smllib-1.3/tests/test_sml_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2023-10-18 05:34:23.000000 smllib-1.3/tests/test_sml_stream_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:42:53.026432 smllib-1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-05 05:42:43.000000 smllib-1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-05 05:42:43.000000 smllib-1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-04-05 05:42:53.026432 smllib-1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 05:42:53.026432 smllib-1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-05 05:42:43.000000 smllib-1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:42:53.018432 smllib-1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:42:53.022432 smllib-1.4/src/smllib/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-05 05:42:43.000000 smllib-1.4/src/smllib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-05 05:42:43.000000 smllib-1.4/src/smllib/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:42:53.022432 smllib-1.4/src/smllib/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-05 05:42:43.000000 smllib-1.4/src/smllib/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-05 05:42:43.000000 smllib-1.4/src/smllib/builder/_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-05 05:42:43.000000 smllib-1.4/src/smllib/builder/default_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-05 05:42:43.000000 smllib-1.4/src/smllib/builder/list_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-05 05:42:43.000000 smllib-1.4/src/smllib/builder/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-05 05:42:43.000000 smllib-1.4/src/smllib/builder/response_get_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-05 05:42:43.000000 smllib-1.4/src/smllib/builder/response_open_close.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-05 05:42:43.000000 smllib-1.4/src/smllib/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-05 05:42:43.000000 smllib-1.4/src/smllib/crc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-05 05:42:43.000000 smllib-1.4/src/smllib/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 05:42:43.000000 smllib-1.4/src/smllib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-05 05:42:43.000000 smllib-1.4/src/smllib/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:42:53.022432 smllib-1.4/src/smllib/sml/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-05 05:42:43.000000 smllib-1.4/src/smllib/sml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-05 05:42:43.000000 smllib-1.4/src/smllib/sml/_base_obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-05 05:42:43.000000 smllib-1.4/src/smllib/sml/_field_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-05 05:42:43.000000 smllib-1.4/src/smllib/sml/list_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-05 05:42:43.000000 smllib-1.4/src/smllib/sml/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-05 05:42:43.000000 smllib-1.4/src/smllib/sml/response_get_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-05 05:42:43.000000 smllib-1.4/src/smllib/sml/response_open_close.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-05 05:42:43.000000 smllib-1.4/src/smllib/sml/sml_choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-05 05:42:43.000000 smllib-1.4/src/smllib/sml/sml_eom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-05 05:42:43.000000 smllib-1.4/src/smllib/sml/sml_obis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-05 05:42:43.000000 smllib-1.4/src/smllib/sml/sml_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-04-05 05:42:43.000000 smllib-1.4/src/smllib/sml_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-05 05:42:43.000000 smllib-1.4/src/smllib/sml_frame_snippet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:42:53.026432 smllib-1.4/src/smllib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-04-05 05:42:52.000000 smllib-1.4/src/smllib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-05 05:42:52.000000 smllib-1.4/src/smllib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 05:42:52.000000 smllib-1.4/src/smllib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 05:42:52.000000 smllib-1.4/src/smllib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:42:53.026432 smllib-1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-05 05:42:43.000000 smllib-1.4/tests/test_crc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-05 05:42:43.000000 smllib-1.4/tests/test_frame_snipped.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-04-05 05:42:43.000000 smllib-1.4/tests/test_frames.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-04-05 05:42:43.000000 smllib-1.4/tests/test_sml_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-05 05:42:43.000000 smllib-1.4/tests/test_sml_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-05 05:42:43.000000 smllib-1.4/tests/test_sml_stream_reader.py
```

### Comparing `smllib-1.3/LICENSE` & `smllib-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `smllib-1.3/PKG-INFO` & `smllib-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smllib
-Version: 1.3
+Version: 1.4
 Summary: A library for the SML (Smart Message Language) protocol
 Home-page: https://github.com/spacemanspiff2007/SmlLib
 Author: spaceman_spiff
 Project-URL: GitHub, https://github.com/spacemanspiff2007/SmlLib
 Keywords: sml,obis,smart message language,energy meter
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `smllib-1.3/setup.py` & `smllib-1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import typing
 from pathlib import Path
 
-import setuptools  # type: ignore
+import setuptools
 
 
 def load_version() -> str:
     version: typing.Dict[str, str] = {}
-    with open("src/smllib/__version__.py") as fp:
+    with (Path(__file__).parent / "src/smllib/__version__.py").open() as fp:
         exec(fp.read(), version)
     assert version['__version__'], version
     return version['__version__']
 
 
 __version__ = load_version()
 
@@ -40,14 +40,15 @@
     long_description_content_type="text/markdown",
     url="https://github.com/spacemanspiff2007/SmlLib",
     project_urls={
         'GitHub': "https://github.com/spacemanspiff2007/SmlLib",
     },
     packages=setuptools.find_packages(where='src', exclude=['tests*']),
     package_dir={'': 'src'},
+    package_data={'smllib': ['py.typed']},
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

### Comparing `smllib-1.3/src/smllib/builder/_builder.py` & `smllib-1.4/src/smllib/builder/_builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, Generic, Type, TypeVar
 
 from smllib.errors import WrongArgCount, WrongValueType
-from smllib.sml import inspect_obj, SmlBaseObj, SmlObjFieldInfo, T_SML_OBJ
+from smllib.sml import T_SML_OBJ, SmlBaseObj, SmlObjFieldInfo, inspect_obj
 from smllib.sml_frame_snippet import SmlFrameSnippet
 
 
 class SmlObjBuilder(Generic[T_SML_OBJ]):
     BUILDS: Type[T_SML_OBJ]
 
     def __init__(self):
@@ -33,14 +33,15 @@
                 value = func(value)
 
             if field.is_container:
                 cls_builder = classes[field.type]
                 value = tuple([cls_builder.build(v, classes) for v in value])
             else:
                 if not isinstance(value, field.type):
-                    raise WrongValueType(f'{value} ({type(value)}) != {field.type}')
+                    msg = f'{value} ({type(value)}) != {field.type}'
+                    raise WrongValueType(msg)
 
             setattr(out, name, value)
         return out
 
 
 T_SML_BUILDER = TypeVar('T_SML_BUILDER', bound=SmlObjBuilder, covariant=True)
```

### Comparing `smllib-1.3/src/smllib/builder/default_context.py` & `smllib-1.4/src/smllib/builder/default_context.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 from typing import Dict, Type
 
 from smllib.sml import SmlBaseObj, SmlCloseResponse, SmlGetListResponse, SmlListEntry, SmlMessage, SmlOpenResponse
 
-from . import SmlCloseResponseBuilder, SmlGetListResponseBuilder, \
-    SmlListEntryBuilder, SmlMessageBuilder, SmlOpenResponseBuilder, T_SML_BUILDER
+from . import (
+    T_SML_BUILDER,
+    SmlCloseResponseBuilder,
+    SmlGetListResponseBuilder,
+    SmlListEntryBuilder,
+    SmlMessageBuilder,
+    SmlOpenResponseBuilder,
+)
+
 
 CTX_HINT = Dict[Type[SmlBaseObj], T_SML_BUILDER]
 
 
 def create_context() -> CTX_HINT:
     return {
         SmlListEntry: SmlListEntryBuilder(),
```

### Comparing `smllib-1.3/src/smllib/builder/list_entry.py` & `smllib-1.4/src/smllib/builder/list_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
     BUILDS = SmlListEntry
 
     def build(self, obj: SmlFrameSnippet, classes: Dict[Type[SmlBaseObj], 'SmlObjBuilder']) -> SmlListEntry:
         ret = super().build(obj, classes)    # type: SmlListEntry
 
         value = ret.value
         if value is None:
-            raise ValueError('value is required!')
+            msg = 'value is required!'
+            raise ValueError(msg)
 
         # Maybe it's ascii so we try to decode it
         if isinstance(value, str):
             v = a2b_hex(value).decode(errors='ignore')
             if v.isalnum():
                 ret.value = v
```

### Comparing `smllib-1.3/src/smllib/builder/message.py` & `smllib-1.4/src/smllib/builder/message.py`

 * *Files identical despite different names*

### Comparing `smllib-1.3/src/smllib/const.py` & `smllib-1.4/src/smllib/const.py`

 * *Files identical despite different names*

### Comparing `smllib-1.3/src/smllib/crc.py` & `smllib-1.4/src/smllib/crc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Union
 
+
 CRC16_X25_TABLE = (
     0x0000, 0x1189, 0x2312, 0x329B, 0x4624, 0x57AD, 0x6536, 0x74BF,
     0x8C48, 0x9DC1, 0xAF5A, 0xBED3, 0xCA6C, 0xDBE5, 0xE97E, 0xF8F7,
     0x1081, 0x0108, 0x3393, 0x221A, 0x56A5, 0x472C, 0x75B7, 0x643E,
     0x9CC9, 0x8D40, 0xBFDB, 0xAE52, 0xDAED, 0xCB64, 0xF9FF, 0xE876,
     0x2102, 0x308B, 0x0210, 0x1399, 0x6726, 0x76AF, 0x4434, 0x55BD,
     0xAD4A, 0xBCC3, 0x8E58, 0x9FD1, 0xEB6E, 0xFAE7, 0xC87C, 0xD9F5,
```

### Comparing `smllib-1.3/src/smllib/errors.py` & `smllib-1.4/src/smllib/errors.py`

 * *Files identical despite different names*

### Comparing `smllib-1.3/src/smllib/reader.py` & `smllib-1.4/src/smllib/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from smllib.builder import create_context, CTX_HINT
+from smllib.builder import CTX_HINT, create_context
 from smllib.crc import get_crc
 from smllib.errors import CrcError
 from smllib.sml_frame import SmlFrame
 
 
 class SmlStreamReader:
     MAX_SIZE = 50 * 1024
```

### Comparing `smllib-1.3/src/smllib/sml/__init__.py` & `smllib-1.4/src/smllib/sml/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,29 @@
-from smllib.sml._base_obj import SmlBaseObj, T_SML_OBJ
+from smllib.sml._base_obj import T_SML_OBJ, SmlBaseObj
 from smllib.sml.sml_eom import EndOfSmlMsg
 
+
 # isort: split
 
+
 from smllib.sml.sml_choice import SmlChoice
 
+
 # isort: split
-from smllib.sml._field_info import inspect_obj, SmlObjFieldInfo
+
+
+from smllib.sml._field_info import SmlObjFieldInfo, inspect_obj
+
 
 # isort: split
 
+
 from smllib.sml.list_entry import SmlListEntry
 from smllib.sml.response_get_list import SmlGetListResponse
 from smllib.sml.response_open_close import SmlCloseResponse, SmlOpenResponse
 from smllib.sml.sml_obis import ObisCode
 
+
 # isort: split
+
+
 from smllib.sml.message import SmlMessage
```

### Comparing `smllib-1.3/src/smllib/sml/_base_obj.py` & `smllib-1.4/src/smllib/sml/_base_obj.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,27 @@
+import typing
 from typing import Final, TypeVar
 
+
 INDENT: Final = '  '
 
 
 class SmlBaseObj:
-    __sml__: dict
+    __sml__: typing.ClassVar[dict]
 
     def format_msg(self, indent: int = 0):
         indent += 1
         r = f'<{self.__class__.__name__}>\n'
         w = max(map(len, self.__dict__), default=0)
         for k, v in self.__dict__.items():
             if isinstance(v, SmlBaseObj):
-                r += f'{INDENT * indent}{str(k):s} {v.format_msg(indent)}'
+                r += f'{INDENT * indent}{k!s:s} {v.format_msg(indent)}'
             elif isinstance(v, (tuple, list)):
-                r += f'{INDENT * indent}{str(k):s}:\n'
+                r += f'{INDENT * indent}{k!s:s}:\n'
                 for e in v:
                     r += f'{INDENT * (indent + 1)}{e.format_msg(indent + 1)}'
             else:
-                r += f'{INDENT * indent}{str(k):{w}s}: {v}\n'
+                r += f'{INDENT * indent}{k!s:{w}s}: {v}\n'
         return r
 
 
 T_SML_OBJ = TypeVar('T_SML_OBJ', bound=SmlBaseObj, covariant=True)
```

### Comparing `smllib-1.3/src/smllib/sml/_field_info.py` & `smllib-1.4/src/smllib/sml/_field_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable, Dict, Final, get_args, get_origin, get_type_hints, Optional, Type, Union
+from typing import Any, Callable, Dict, Final, Optional, Type, Union, get_args, get_origin, get_type_hints
 
 from smllib.sml import SmlBaseObj, SmlChoice
 
 
 class SmlObjFieldInfo:
     def __init__(self, func: Optional[Callable[[Any], Any]] = None, type=None,
                  choice: Optional[SmlChoice] = None, is_container=False):
@@ -60,10 +60,11 @@
         if origin is tuple:
             info.is_container = True
             args = get_args(hint)
             assert args[1] is ...
             info.type = args[0]
             continue
 
-        raise ValueError(f'Unknown hint: {origin} for {name}')
+        msg = f'Unknown hint: {origin} for {name}'
+        raise ValueError(msg)
 
     return fields
```

### Comparing `smllib-1.3/src/smllib/sml/list_entry.py` & `smllib-1.4/src/smllib/sml/list_entry.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Dict, Optional, Union
+from typing import ClassVar, Dict, Optional, Union
 
 from smllib.const import OBIS_NAMES, UNITS
 from smllib.sml import SmlObjFieldInfo
 from smllib.sml._base_obj import INDENT, SmlBaseObj
 
-from .sml_obis import build_obis, ObisCode
-from .sml_time import build_time, TIME_HINT
+from .sml_obis import ObisCode, build_obis
+from .sml_time import TIME_HINT, build_time
 
 
 class SmlListEntry(SmlBaseObj):
-    __sml__: Dict[str, SmlObjFieldInfo] = {
+    __sml__: ClassVar[Dict[str, SmlObjFieldInfo]] = {
         'val_time': SmlObjFieldInfo(func=build_time),
         'obis': SmlObjFieldInfo(func=build_obis)
     }
 
     obis: ObisCode
     status: Optional[int]
     val_time: TIME_HINT
@@ -31,15 +31,15 @@
 
     def format_msg(self, indent: int = 0):
         indent += 1
         r = f'<{self.__class__.__name__}>\n'
         w = max(map(len, self.__dict__), default=0)
 
         for k, v in self.__dict__.items():
-            r += f'{INDENT*indent}{str(k):{w}s}: {v}{f" ({self.obis.obis_code})" if k == "obis" else ""}\n'
+            r += f'{INDENT*indent}{k!s:{w}s}: {v}{f" ({self.obis.obis_code})" if k == "obis" else ""}\n'
 
         summary = ''
         if self.unit:
             val = self.get_value()
             u = UNITS.get(self.unit)
             if u is None:
                 u = f" ?:{self.unit}"
```

### Comparing `smllib-1.3/src/smllib/sml/message.py` & `smllib-1.4/src/smllib/sml/message.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from typing import Dict, Type, Union
+from typing import ClassVar, Dict, Type, Union
 
 from smllib.sml import SmlBaseObj, SmlChoice, SmlCloseResponse, SmlGetListResponse, SmlObjFieldInfo, SmlOpenResponse
 
+
 MSG_TYPES: Dict[int, Type[SmlBaseObj]] = {
     # 0x0100: 'SmlOpenRequest',
     0x0101: SmlOpenResponse,
     # 0x0200: 'SmlCloseRequest',
     0x0201: SmlCloseResponse,
     # 0x0300: 'SmlGetProfilePackRequest',
     # 0x0301: 'SmlGetProfilePackResponse',
@@ -18,15 +19,15 @@
     # 0x0700: 'SmlGetListRequest',
     0x0701: SmlGetListResponse,
     # 0xff01: 'SmlAttentionResponse',
 }
 
 
 class SmlMessage(SmlBaseObj):
-    __sml__: Dict[str, SmlObjFieldInfo] = {
+    __sml__: ClassVar[Dict[str, SmlObjFieldInfo]] = {
         'message_body': SmlObjFieldInfo(choice=SmlChoice(MSG_TYPES))
     }
 
     transaction_id: str
     group_no: int
     abort_on_error: int
     message_body: Union[SmlOpenResponse, SmlCloseResponse, SmlGetListResponse]
```

### Comparing `smllib-1.3/src/smllib/sml/response_get_list.py` & `smllib-1.4/src/smllib/sml/response_get_list.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import Dict, Optional, Tuple
+from typing import ClassVar, Dict, Optional, Tuple
 
 from smllib.sml import SmlBaseObj, SmlListEntry, SmlObjFieldInfo
 
-from .sml_time import build_time, TIME_HINT
+from .sml_time import TIME_HINT, build_time
 
 
 class SmlGetListResponse(SmlBaseObj):
-    __sml__: Dict[str, SmlObjFieldInfo] = {
+    __sml__: ClassVar[Dict[str, SmlObjFieldInfo]] = {
         'act_sensor_time': SmlObjFieldInfo(func=build_time),
         'act_gateway_time': SmlObjFieldInfo(func=build_time),
     }
 
     client_id: Optional[str]
     server_id: str
     list_name: Optional[str]
```

### Comparing `smllib-1.3/src/smllib/sml/response_open_close.py` & `smllib-1.4/src/smllib/sml/response_open_close.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from typing import Dict, Optional
+from typing import ClassVar, Dict, Optional
 
 from smllib.sml import SmlBaseObj, SmlObjFieldInfo
 
-from .sml_time import build_time, TIME_HINT
+from .sml_time import TIME_HINT, build_time
 
 
 class SmlOpenResponse(SmlBaseObj):
-    __sml__: Dict[str, SmlObjFieldInfo] = {
+    __sml__: ClassVar[Dict[str, SmlObjFieldInfo]] = {
         'ref_time': SmlObjFieldInfo(func=build_time)
     }
 
     codepage: Optional[str]
     client_id: Optional[str]
     req_file_id: str
     server_id: str
     ref_time: TIME_HINT
     sml_version: Optional[int]
 
 
 class SmlCloseResponse(SmlBaseObj):
-    __sml__: Dict[str, SmlObjFieldInfo] = {}
+    __sml__: ClassVar[Dict[str, SmlObjFieldInfo]] = {}
 
     global_signature: Optional[str]
```

### Comparing `smllib-1.3/src/smllib/sml/sml_choice.py` & `smllib-1.4/src/smllib/sml/sml_choice.py`

 * *Files identical despite different names*

### Comparing `smllib-1.3/src/smllib/sml/sml_obis.py` & `smllib-1.4/src/smllib/sml/sml_obis.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 class ObisCode(str):
+    __slots__ = ('obis_code', 'obis_short')
+
     def __init__(self, obis_hex: str):
         _a = int(obis_hex[0:2], 16)
         _b = int(obis_hex[2:4], 16)
         _c = int(obis_hex[4:6], 16)
         _d = int(obis_hex[6:8], 16)
         _e = int(obis_hex[8:10], 16)
         _f = int(obis_hex[10:12], 16)
         self.obis_code = f'{_a}-{_b}:{_c}.{_d}.{_e}*{_f}'
         self.obis_short = f'{_c}.{_d}.{_e}'
 
     def __new__(cls, obis_hex: str):
-        obj = str.__new__(cls, obis_hex)
-        return obj
+        return str.__new__(cls, obis_hex)
 
 
 def build_obis(_in) -> ObisCode:
     if not isinstance(_in, str) or len(_in) != 12:
-        raise ValueError(f'Obis code must be a 12 char hex str (is "{_in}" {type(_in)})!')
+        msg = f'Obis code must be a 12 char hex str (is "{_in}" {type(_in)})!'
+        raise ValueError(msg)
 
     return ObisCode(_in)
```

### Comparing `smllib-1.3/src/smllib/sml/sml_time.py` & `smllib-1.4/src/smllib/sml/sml_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from datetime import datetime, timedelta
 from typing import Union
 
 from smllib.errors import UnsupportedChoiceValue
 
+
 TIME_HINT = Union[None, int, datetime]
 
 
 def build_time(_in):
     if _in is None:
         return _in
```

### Comparing `smllib-1.3/src/smllib/sml_frame.py` & `smllib-1.4/src/smllib/sml_frame.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Optional
 
-from smllib.builder import create_context, CTX_HINT
+from smllib.builder import CTX_HINT, create_context
 from smllib.errors import InvalidBufferPos
 from smllib.sml import EndOfSmlMsg, SmlListEntry, SmlMessage
 from smllib.sml_frame_snippet import SmlFrameSnippet
 
 
 class SmlFrame:
     def __init__(self, buffer: bytes, build_ctx: Optional[CTX_HINT] = None, msg_ctx: Optional[bytes] = None):
@@ -20,15 +20,16 @@
     def get_value(self, pos: Optional[int] = None) -> SmlFrameSnippet:
         if pos is None:
             pos = self.next_pos
         snip_start = pos
 
         # check start pos
         if pos >= self.buf_len:
-            raise InvalidBufferPos(f'Start pos bigger than buffer: {pos} > {self.buf_len}')
+            msg = f'Start pos bigger than buffer: {pos} > {self.buf_len}'
+            raise InvalidBufferPos(msg)
 
         # advance
         v = self.buffer[pos]
         start = pos + 1
 
         # ----------------------------------------
         # types with fixed size
@@ -65,40 +66,43 @@
         if _type == 0x70:
             self.next_pos = start   # Must be s_pos because we can have lists with a long length
             return SmlFrameSnippet([None for _ in range(_size)], snip_start)
 
         # End position
         end = pos + _size
         if end > self.buf_len:
-            raise InvalidBufferPos(f'Pos bigger than buffer: {end} > {self.buf_len}')
+            msg = f'Pos bigger than buffer: {end} > {self.buf_len}'
+            raise InvalidBufferPos(msg)
         self.next_pos = end
 
         # 0x50: signed integer, 0x60 unsigned integer
         if _type == 0x50 or _type == 0x60:
             return SmlFrameSnippet(
                 int.from_bytes(self.buffer[start:end], byteorder='big', signed=_type == 0x50),
                 snip_start, end, self.buffer
             )
 
         # 0x00: octet str
         if _type == 0x00:
             return SmlFrameSnippet(self.buffer[start:end].hex(), snip_start, end, self.buffer)
 
-        raise ValueError(f'Unknown data type: {_type:02x}!')
+        msg = f'Unknown data type: {_type:02x}!'
+        raise ValueError(msg)
 
     def parse_frame(self) -> List[SmlMessage]:
         ret = []
         self.next_pos = 0
         while self.next_pos < self.buf_len:
 
-            if not self.buffer[self.next_pos] == 0x76:
-                raise ValueError(
+            if self.buffer[self.next_pos] != 0x76:
+                msg = (
                     f'No start of SML Message found at {self.next_pos}: 0x{self.buffer[self.next_pos]:x}\n'
                     f'{self.buffer.hex()}'
                 )
+                raise ValueError(msg)
 
             # This will always return a list
             val = self._parse_msg(self.get_value())
             ret.append(self.build_ctx[SmlMessage].build(val, self.build_ctx))
         return ret
 
     def _parse_msg(self, parent_obj: SmlFrameSnippet) -> SmlFrameSnippet:
```

### Comparing `smllib-1.3/src/smllib/sml_frame_snippet.py` & `smllib-1.4/src/smllib/sml_frame_snippet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 from typing import Optional, Type, TypeVar, Union
 
 from smllib.errors import WrongValueType
 from smllib.sml.sml_eom import CEndOfSmlMsg
 
+
 SNIP_TYPE = TypeVar('SNIP_TYPE', bound=object)
 
 
 class SmlFrameSnippet:
     __slots__ = ('pos', 'value', 'msg')
 
     def __init__(self, value: Union[None, bool, int, str, float, list, CEndOfSmlMsg], start: int,
                  stop: Optional[int] = None, buf: Optional[memoryview] = None):
 
         msg = None
         if stop is not None:
             if buf is None:
-                raise ValueError('Arg stop und buf must be used together')
+                err_msg = 'Arg stop und buf must be used together'
+                raise ValueError(err_msg)
             msg = buf[start: stop]
 
         self.value = value
         self.pos = start
         self.msg: Optional[memoryview] = msg
 
     def stop_pos(self, pos: int, buf: memoryview) -> 'SmlFrameSnippet':
         assert self.msg is None
         self.msg = buf[self.pos: pos]
         return self
 
     def get_value(self, val_type: Type[SNIP_TYPE]) -> SNIP_TYPE:
         value = self.value
         if not isinstance(value, val_type):
-            raise WrongValueType(f'Expected type {val_type.__name__} but got type {type(value).__name__}')
+            msg = f'Expected type {val_type.__name__} but got type {type(value).__name__}'
+            raise WrongValueType(msg)
         return value
```

### Comparing `smllib-1.3/src/smllib.egg-info/PKG-INFO` & `smllib-1.4/src/smllib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smllib
-Version: 1.3
+Version: 1.4
 Summary: A library for the SML (Smart Message Language) protocol
 Home-page: https://github.com/spacemanspiff2007/SmlLib
 Author: spaceman_spiff
 Project-URL: GitHub, https://github.com/spacemanspiff2007/SmlLib
 Keywords: sml,obis,smart message language,energy meter
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `smllib-1.3/src/smllib.egg-info/SOURCES.txt` & `smllib-1.4/src/smllib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smllib-1.3/tests/test_crc.py` & `smllib-1.4/tests/test_crc.py`

 * *Files identical despite different names*

### Comparing `smllib-1.3/tests/test_frame_snipped.py` & `smllib-1.4/tests/test_frame_snipped.py`

 * *Files identical despite different names*

### Comparing `smllib-1.3/tests/test_frames.py` & `smllib-1.4/tests/test_frames.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,23 +73,23 @@
     )
 )
 def test_frames(frame):
 
     reader = SmlStreamReader()
     reader.add(a2b_hex(frame))
 
-    frame = reader.get_frame()
-    assert frame is not None
+    parsed_frame = reader.get_frame()
+    assert parsed_frame is not None
 
     # ensure that parsing always works
     for _ in range(3):
-        sml_messages = frame.parse_frame()
+        sml_messages = parsed_frame.parse_frame()
         assert len(sml_messages) >= 3, sml_messages
 
-        obis_values = frame.get_obis()
+        obis_values = parsed_frame.get_obis()
         assert len(obis_values) >= 4, obis_values
 
         for obis in obis_values:
             obis.get_value()
 
 
 @pytest.mark.parametrize(
```

### Comparing `smllib-1.3/tests/test_sml_data_types.py` & `smllib-1.4/tests/test_sml_data_types.py`

 * *Files identical despite different names*

### Comparing `smllib-1.3/tests/test_sml_fields.py` & `smllib-1.4/tests/test_sml_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from binascii import a2b_hex
 
-from smllib.builder import create_context, SmlListEntryBuilder
+from smllib.builder import SmlListEntryBuilder, create_context
 from smllib.sml_frame import SmlFrame
 
 
 def test_sml_fields():
     f = SmlFrame(a2b_hex('77078181c78203ff010101010449534b0177070100000009ff010101010b'))
     val_list = f._parse_msg(f.get_value(0))
     o = SmlListEntryBuilder().build(val_list, create_context())
```

### Comparing `smllib-1.3/tests/test_sml_stream_reader.py` & `smllib-1.4/tests/test_sml_stream_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 
 def test_msg_long_list():
     msg2 = binascii.a2b_hex(
         '1b1b1b1b01010101'
         '76040000016200620072650000010176010107000002dba23c0b0a01484c5902000424a0010163945b00'
         # This frame contains a long list (f104)
-        '76040000026200620072650000070177010b0a01484c5902000424a00101f10477070100603201010101010104484c590177070100600100ff010101010b0a01484c5902000424a00177070100010800ff65001c81046502dba23d621e52ff6502aea1320177070100020800ff65001c81046502dba23d621e52ff62000177070100100700ff0101621b52005300890177070100200700ff0101622352ff6309280177070100340700ff0101622352ff6309290177070100480700ff0101622352ff63092201770701001f0700ff0101622152fe62290177070100330700ff0101622152fe624e0177070100470700ff0101622152fe622e0177070100510701ff01016208520062f00177070100510702ff01016208520062780177070100510704ff010162085200630110017707010051070fff010162085200630138017707010051071aff01016208520063011101770701000e0700ff0101622c52ff6301f40177070100000200000101010109312e30322e3030370177070100605a02010101010105413031410177070100600500ff0101010165001c810401010163fc1e00'  # noqa: E501
+        '76040000026200620072650000070177010b0a01484c5902000424a00101f10477070100603201010101010104484c590177070100600100ff010101010b0a01484c5902000424a00177070100010800ff65001c81046502dba23d621e52ff6502aea1320177070100020800ff65001c81046502dba23d621e52ff62000177070100100700ff0101621b52005300890177070100200700ff0101622352ff6309280177070100340700ff0101622352ff6309290177070100480700ff0101622352ff63092201770701001f0700ff0101622152fe62290177070100330700ff0101622152fe624e0177070100470700ff0101622152fe622e0177070100510701ff01016208520062f00177070100510702ff01016208520062780177070100510704ff010162085200630110017707010051070fff010162085200630138017707010051071aff01016208520063011101770701000e0700ff0101622c52ff6301f40177070100000200000101010109312e30322e3030370177070100605a02010101010105413031410177070100600500ff0101010165001c810401010163fc1e00'
         '760400000362006200726500000201710163e82300'
         '00001b1b1b1b1a0222ed'
     )
 
     r = SmlStreamReader()
     r.add(msg2)
     frame = r.get_frame()
```

