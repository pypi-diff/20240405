# Comparing `tmp/streamlit-nested-layout-0.1.2.tar.gz` & `tmp/streamlit-nested-layout-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-nested-layout-0.1.2.tar", last modified: Fri Mar 15 03:36:00 2024, max compression
+gzip compressed data, was "streamlit-nested-layout-0.1.3.tar", last modified: Fri Apr  5 09:27:55 2024, max compression
```

## Comparing `streamlit-nested-layout-0.1.2.tar` & `streamlit-nested-layout-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 joy        (501) staff       (20)        0 2024-03-15 03:36:00.263794 streamlit-nested-layout-0.1.2/
--rw-r--r--   0 joy        (501) staff       (20)    11357 2022-09-15 07:05:04.000000 streamlit-nested-layout-0.1.2/LICENSE
--rw-r--r--   0 joy        (501) staff       (20)       25 2022-09-15 07:03:39.000000 streamlit-nested-layout-0.1.2/MANIFEST.in
--rw-r--r--   0 joy        (501) staff       (20)     1465 2024-03-15 03:36:00.263562 streamlit-nested-layout-0.1.2/PKG-INFO
--rw-r--r--   0 joy        (501) staff       (20)      757 2024-03-15 03:28:40.000000 streamlit-nested-layout-0.1.2/README.md
--rw-r--r--   0 joy        (501) staff       (20)       38 2024-03-15 03:36:00.263861 streamlit-nested-layout-0.1.2/setup.cfg
--rw-r--r--   0 joy        (501) staff       (20)     4125 2024-03-15 03:35:41.000000 streamlit-nested-layout-0.1.2/setup.py
-drwxr-xr-x   0 joy        (501) staff       (20)        0 2024-03-15 03:36:00.262298 streamlit-nested-layout-0.1.2/streamlit_nested_layout/
--rw-r--r--   0 joy        (501) staff       (20)       18 2022-09-15 07:53:19.000000 streamlit-nested-layout-0.1.2/streamlit_nested_layout/__init__.py
--rw-r--r--   0 joy        (501) staff       (20)     3593 2024-03-15 03:21:13.000000 streamlit-nested-layout-0.1.2/streamlit_nested_layout/nest.py
-drwxr-xr-x   0 joy        (501) staff       (20)        0 2024-03-15 03:36:00.263294 streamlit-nested-layout-0.1.2/streamlit_nested_layout.egg-info/
--rw-r--r--   0 joy        (501) staff       (20)     1465 2024-03-15 03:36:00.000000 streamlit-nested-layout-0.1.2/streamlit_nested_layout.egg-info/PKG-INFO
--rw-r--r--   0 joy        (501) staff       (20)      340 2024-03-15 03:36:00.000000 streamlit-nested-layout-0.1.2/streamlit_nested_layout.egg-info/SOURCES.txt
--rw-r--r--   0 joy        (501) staff       (20)        1 2024-03-15 03:36:00.000000 streamlit-nested-layout-0.1.2/streamlit_nested_layout.egg-info/dependency_links.txt
--rw-r--r--   0 joy        (501) staff       (20)       18 2024-03-15 03:36:00.000000 streamlit-nested-layout-0.1.2/streamlit_nested_layout.egg-info/requires.txt
--rw-r--r--   0 joy        (501) staff       (20)       24 2024-03-15 03:36:00.000000 streamlit-nested-layout-0.1.2/streamlit_nested_layout.egg-info/top_level.txt
+drwxr-xr-x   0 joy        (501) staff       (20)        0 2024-04-05 09:27:55.409889 streamlit-nested-layout-0.1.3/
+-rw-r--r--   0 joy        (501) staff       (20)    11357 2022-09-15 07:05:04.000000 streamlit-nested-layout-0.1.3/LICENSE
+-rw-r--r--   0 joy        (501) staff       (20)       25 2022-09-15 07:03:39.000000 streamlit-nested-layout-0.1.3/MANIFEST.in
+-rw-r--r--   0 joy        (501) staff       (20)     1465 2024-04-05 09:27:55.409614 streamlit-nested-layout-0.1.3/PKG-INFO
+-rw-r--r--   0 joy        (501) staff       (20)      757 2024-04-05 09:27:40.000000 streamlit-nested-layout-0.1.3/README.md
+-rw-r--r--   0 joy        (501) staff       (20)       38 2024-04-05 09:27:55.409947 streamlit-nested-layout-0.1.3/setup.cfg
+-rw-r--r--   0 joy        (501) staff       (20)     4125 2024-04-05 09:20:22.000000 streamlit-nested-layout-0.1.3/setup.py
+drwxr-xr-x   0 joy        (501) staff       (20)        0 2024-04-05 09:27:55.408424 streamlit-nested-layout-0.1.3/streamlit_nested_layout/
+-rw-r--r--   0 joy        (501) staff       (20)       18 2022-09-15 07:53:19.000000 streamlit-nested-layout-0.1.3/streamlit_nested_layout/__init__.py
+-rw-r--r--   0 joy        (501) staff       (20)     3630 2024-04-05 09:19:54.000000 streamlit-nested-layout-0.1.3/streamlit_nested_layout/nest.py
+drwxr-xr-x   0 joy        (501) staff       (20)        0 2024-04-05 09:27:55.409335 streamlit-nested-layout-0.1.3/streamlit_nested_layout.egg-info/
+-rw-r--r--   0 joy        (501) staff       (20)     1465 2024-04-05 09:27:55.000000 streamlit-nested-layout-0.1.3/streamlit_nested_layout.egg-info/PKG-INFO
+-rw-r--r--   0 joy        (501) staff       (20)      340 2024-04-05 09:27:55.000000 streamlit-nested-layout-0.1.3/streamlit_nested_layout.egg-info/SOURCES.txt
+-rw-r--r--   0 joy        (501) staff       (20)        1 2024-04-05 09:27:55.000000 streamlit-nested-layout-0.1.3/streamlit_nested_layout.egg-info/dependency_links.txt
+-rw-r--r--   0 joy        (501) staff       (20)       18 2024-04-05 09:27:55.000000 streamlit-nested-layout-0.1.3/streamlit_nested_layout.egg-info/requires.txt
+-rw-r--r--   0 joy        (501) staff       (20)       24 2024-04-05 09:27:55.000000 streamlit-nested-layout-0.1.3/streamlit_nested_layout.egg-info/top_level.txt
```

### Comparing `streamlit-nested-layout-0.1.2/LICENSE` & `streamlit-nested-layout-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-nested-layout-0.1.2/PKG-INFO` & `streamlit-nested-layout-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-nested-layout
-Version: 0.1.2
+Version: 0.1.3
 Summary: Enables nested layout in streamlit.
 Home-page: https://github.com/joy13975/streamlit-nested-layout
 Author: Joy Yeh
 Author-email: joyyeh.tw@gmail.com
 License: Apache 2.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -21,15 +21,15 @@
 # streamlit-nested-layout
 An unofficial monkey patch that enables [streamlit](https://github.com/streamlit/streamlit) columns and expanders to be nested.
 
 ```diff
 - ⚠️Streamlit developers disallow this behavior by design, so you are on your own if you encounter issues using this package!⚠️
 ```
 
-Last tested for `streamlit==1.32.2` on `Python 3.9.18`.
+Last tested for `streamlit==1.33.0` on `Python 3.9.18`.
 
 Credits to [streamlit PR #5266](https://github.com/streamlit/streamlit/pull/5266) by [@ZeroCool940711](https://github.com/ZeroCool940711).
 
 ### Install
 ```
 pip install streamlit-nested-layout
 ```
```

### Comparing `streamlit-nested-layout-0.1.2/README.md` & `streamlit-nested-layout-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # streamlit-nested-layout
 An unofficial monkey patch that enables [streamlit](https://github.com/streamlit/streamlit) columns and expanders to be nested.
 
 ```diff
 - ⚠️Streamlit developers disallow this behavior by design, so you are on your own if you encounter issues using this package!⚠️
 ```
 
-Last tested for `streamlit==1.32.2` on `Python 3.9.18`.
+Last tested for `streamlit==1.33.0` on `Python 3.9.18`.
 
 Credits to [streamlit PR #5266](https://github.com/streamlit/streamlit/pull/5266) by [@ZeroCool940711](https://github.com/ZeroCool940711).
 
 ### Install
 ```
 pip install streamlit-nested-layout
 ```
```

### Comparing `streamlit-nested-layout-0.1.2/setup.py` & `streamlit-nested-layout-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 # REQUIRES_PYTHON = '>=3.6.0'
 # << According to streamlit's setup.py >>
 # We exclude Python 3.9.7 from our compatible versions due to a bug in that version
 # with typing.Protocol. See https://github.com/streamlit/streamlit/issues/5140 and
 # https://bugs.python.org/issue45121
 REQUIRES_PYTHON=">=3.7, !=3.9.7"
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
     'streamlit>=1.10.0'
 ]
```

### Comparing `streamlit-nested-layout-0.1.2/streamlit_nested_layout/nest.py` & `streamlit-nested-layout-0.1.3/streamlit_nested_layout/nest.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,52 +2,53 @@
 
 from streamlit import cursor
 from streamlit.delta_generator import DeltaGenerator
 from streamlit.delta_generator import _enqueue_message
 from streamlit.elements.form import FormData, current_form_id
 from streamlit.proto import Block_pb2, ForwardMsg_pb2
 from streamlit.runtime import caching
+from streamlit.proto.RootContainer_pb2 import RootContainer
 
 def _nestable_block(
     self,
     block_proto: Block_pb2.Block = Block_pb2.Block(),
     dg_type: Union[type, None] = None,
-) -> "DeltaGenerator":
+) -> DeltaGenerator:
     # Operate on the active DeltaGenerator, in case we're in a `with` block.
     dg = self._active_dg
 
     # Prevent nested columns & expanders by checking all parents.
     block_type = block_proto.WhichOneof("type")
     # Convert the generator to a list, so we can use it multiple times.
-    parent_block_types = list(dg._parent_block_types)
+    ancestor_block_types = list(dg._ancestor_block_types)
 
     # if block_type == "column":
     #     num_of_parent_columns = self._count_num_of_parent_columns(
-    #         parent_block_types
+    #         ancestor_block_types
     #     )
     #     if (
     #         self._root_container == RootContainer.SIDEBAR
     #         and num_of_parent_columns > 0
     #     ):
     #         raise StreamlitAPIException(
     #             "Columns cannot be placed inside other columns in the sidebar. This is only possible in the main area of the app."
     #         )
     #     if num_of_parent_columns > 1:
     #         raise StreamlitAPIException(
     #             "Columns can only be placed inside other columns up to one level of nesting."
     #         )
-    # if block_type == "chat_message" and block_type in frozenset(parent_block_types):
+    # if block_type == "chat_message" and block_type in ancestor_block_types:
     #     raise StreamlitAPIException(
     #         "Chat messages cannot nested inside other chat messages."
     #     )
-    # if block_type == "expandable" and block_type in frozenset(parent_block_types):
+    # if block_type == "expandable" and block_type in ancestor_block_types:
     #     raise StreamlitAPIException(
     #         "Expanders may not be nested inside other expanders."
     #     )
-    # if block_type == "popover" and block_type in frozenset(parent_block_types):
+    # if block_type == "popover" and block_type in ancestor_block_types:
     #     raise StreamlitAPIException(
     #         "Popovers may not be nested inside other popovers."
     #     )
 
     if dg._root_container is None or dg._cursor is None:
         return dg
```

### Comparing `streamlit-nested-layout-0.1.2/streamlit_nested_layout.egg-info/PKG-INFO` & `streamlit-nested-layout-0.1.3/streamlit_nested_layout.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-nested-layout
-Version: 0.1.2
+Version: 0.1.3
 Summary: Enables nested layout in streamlit.
 Home-page: https://github.com/joy13975/streamlit-nested-layout
 Author: Joy Yeh
 Author-email: joyyeh.tw@gmail.com
 License: Apache 2.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -21,15 +21,15 @@
 # streamlit-nested-layout
 An unofficial monkey patch that enables [streamlit](https://github.com/streamlit/streamlit) columns and expanders to be nested.
 
 ```diff
 - ⚠️Streamlit developers disallow this behavior by design, so you are on your own if you encounter issues using this package!⚠️
 ```
 
-Last tested for `streamlit==1.32.2` on `Python 3.9.18`.
+Last tested for `streamlit==1.33.0` on `Python 3.9.18`.
 
 Credits to [streamlit PR #5266](https://github.com/streamlit/streamlit/pull/5266) by [@ZeroCool940711](https://github.com/ZeroCool940711).
 
 ### Install
 ```
 pip install streamlit-nested-layout
 ```
```

