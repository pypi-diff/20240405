# Comparing `tmp/pyrtz2-1.1.0.tar.gz` & `tmp/pyrtz2-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrtz2-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyrtz2-1.1.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyrtz2-1.1.0.tar` & `pyrtz2-1.1.9.tar`

### file list

```diff
@@ -1,41 +1,40 @@
--rw-r--r--   0        0        0       66 2024-04-02 19:47:59.285340 pyrtz2-1.1.0/.gitattributes
--rw-r--r--   0        0        0      105 2024-04-04 14:02:39.390822 pyrtz2-1.1.0/.vscode/settings.json
--rw-r--r--   0        0        0    33041 2024-04-02 20:07:11.768711 pyrtz2-1.1.0/LICENSE
--rw-r--r--   0        0        0      228 2024-04-02 19:51:47.632334 pyrtz2-1.1.0/README.md
--rw-r--r--   0        0        0     1644 2024-04-04 20:26:20.279513 pyrtz2-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       98 2024-04-04 20:30:49.197222 pyrtz2-1.1.0/pyrtz2/__init__.py
--rw-r--r--   0        0        0     1867 2024-04-04 19:07:59.221420 pyrtz2-1.1.0/pyrtz2/afm.py
--rw-r--r--   0        0        0      372 2024-04-03 01:57:39.926418 pyrtz2-1.1.0/pyrtz2/app.py
--rw-r--r--   0        0        0     1320 2024-03-29 18:30:21.132859 pyrtz2-1.1.0/pyrtz2/assets/style.css
--rw-r--r--   0        0        0     4711 2024-04-04 18:06:07.236982 pyrtz2-1.1.0/pyrtz2/asylum.py
--rw-r--r--   0        0        0    20122 2024-04-04 19:44:01.385877 pyrtz2-1.1.0/pyrtz2/curves.py
--rw-r--r--   0        0        0     4451 2024-04-02 14:59:14.529838 pyrtz2-1.1.0/pyrtz2/fit.py
--rw-r--r--   0        0        0        0 2024-04-03 01:57:24.101285 pyrtz2-1.1.0/pyrtz2/src/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.0/pyrtz2/src/components/__init__.py
--rw-r--r--   0        0        0     1970 2024-04-03 03:12:28.001519 pyrtz2-1.1.0/pyrtz2/src/components/annotator.py
--rw-r--r--   0        0        0     5604 2024-04-04 18:49:51.040442 pyrtz2-1.1.0/pyrtz2/src/components/contact_controls.py
--rw-r--r--   0        0        0     4139 2024-04-03 02:17:21.251676 pyrtz2-1.1.0/pyrtz2/src/components/curve_dropdown.py
--rw-r--r--   0        0        0     3409 2024-04-04 18:23:41.184544 pyrtz2-1.1.0/pyrtz2/src/components/fig.py
--rw-r--r--   0        0        0     4475 2024-04-04 18:07:38.738998 pyrtz2-1.1.0/pyrtz2/src/components/fig_frame.py
--rw-r--r--   0        0        0     2393 2024-04-04 18:36:08.361121 pyrtz2-1.1.0/pyrtz2/src/components/fitter.py
--rw-r--r--   0        0        0     1241 2024-04-04 18:49:04.376522 pyrtz2-1.1.0/pyrtz2/src/components/ids.py
--rw-r--r--   0        0        0     1195 2024-04-03 02:18:43.224430 pyrtz2-1.1.0/pyrtz2/src/components/image_frame.py
--rw-r--r--   0        0        0     1666 2024-04-02 01:29:34.764572 pyrtz2-1.1.0/pyrtz2/src/components/layout.py
--rw-r--r--   0        0        0     3461 2024-04-03 02:29:10.462290 pyrtz2-1.1.0/pyrtz2/src/components/loader.py
--rw-r--r--   0        0        0     1052 2024-04-04 18:50:12.478289 pyrtz2-1.1.0/pyrtz2/src/components/toolbox.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.0/pyrtz2/src/data/__init__.py
--rw-r--r--   0        0        0     3346 2024-04-04 20:08:19.361627 pyrtz2-1.1.0/pyrtz2/src/data/downloader.py
--rw-r--r--   0        0        0     1617 2024-04-04 20:06:58.075042 pyrtz2-1.1.0/pyrtz2/src/data/experiment_loader.py
--rw-r--r--   0        0        0     1128 2024-04-03 02:24:32.297813 pyrtz2-1.1.0/pyrtz2/src/data/image_loader.py
--rw-r--r--   0        0        0     1230 2024-04-04 20:00:47.653098 pyrtz2-1.1.0/pyrtz2/src/data/processor.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.0/pyrtz2/src/utils/__init__.py
--rw-r--r--   0        0        0     1020 2024-03-29 20:53:21.746168 pyrtz2-1.1.0/pyrtz2/src/utils/_backup/igor/__init__.py
--rw-r--r--   0        0        0    30699 2024-03-29 20:52:56.279210 pyrtz2-1.1.0/pyrtz2/src/utils/_backup/igor/binarywave.py
--rw-r--r--   0        0        0    29217 2024-03-29 21:12:48.091560 pyrtz2-1.1.0/pyrtz2/src/utils/_backup/igor/structure.py
--rw-r--r--   0        0        0     3911 2024-02-02 05:34:10.456245 pyrtz2-1.1.0/pyrtz2/src/utils/_backup/igor/util.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.0/pyrtz2/src/utils/_backup/pyrtz/__init__.py
--rw-r--r--   0        0        0     4623 2024-03-29 23:09:57.877567 pyrtz2-1.1.0/pyrtz2/src/utils/_backup/pyrtz/asylum.py
--rw-r--r--   0        0        0    35543 2024-03-30 00:31:39.650484 pyrtz2-1.1.0/pyrtz2/src/utils/_backup/pyrtz/curves.py
--rw-r--r--   0        0        0     2403 2024-04-04 18:28:36.838363 pyrtz2-1.1.0/pyrtz2/src/utils/utils.py
--rw-r--r--   0        0        0     1852 2024-04-04 17:22:15.402815 pyrtz2-1.1.0/test.py
--rw-r--r--   0        0        0     2028 1970-01-01 00:00:00.000000 pyrtz2-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2024-04-02 19:47:59.285340 pyrtz2-1.1.9/.gitattributes
+-rw-r--r--   0        0        0       20 2024-04-04 22:35:31.627883 pyrtz2-1.1.9/.gitignore
+-rw-r--r--   0        0        0    33041 2024-04-02 20:07:11.768711 pyrtz2-1.1.9/LICENSE
+-rw-r--r--   0        0        0      228 2024-04-02 19:51:47.632334 pyrtz2-1.1.9/README.md
+-rw-r--r--   0        0        0      794 2024-04-04 21:36:24.676720 pyrtz2-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0       61 2024-04-04 22:38:22.148901 pyrtz2-1.1.9/pyrtz2/__init__.py
+-rw-r--r--   0        0        0     1874 2024-04-04 20:43:57.261121 pyrtz2-1.1.9/pyrtz2/afm.py
+-rw-r--r--   0        0        0      404 2024-04-04 22:20:09.403050 pyrtz2-1.1.9/pyrtz2/app.py
+-rw-r--r--   0        0        0     1320 2024-03-29 18:30:21.132859 pyrtz2-1.1.9/pyrtz2/assets/style.css
+-rw-r--r--   0        0        0     4718 2024-04-04 20:43:28.570132 pyrtz2-1.1.9/pyrtz2/asylum.py
+-rw-r--r--   0        0        0    20124 2024-04-04 20:43:38.173145 pyrtz2-1.1.9/pyrtz2/curves.py
+-rw-r--r--   0        0        0     4451 2024-04-02 14:59:14.529838 pyrtz2-1.1.9/pyrtz2/fit.py
+-rw-r--r--   0        0        0        0 2024-04-03 01:57:24.101285 pyrtz2-1.1.9/pyrtz2/src/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.9/pyrtz2/src/components/__init__.py
+-rw-r--r--   0        0        0     1982 2024-04-04 22:36:35.966687 pyrtz2-1.1.9/pyrtz2/src/components/annotator.py
+-rw-r--r--   0        0        0     5604 2024-04-04 18:49:51.040442 pyrtz2-1.1.9/pyrtz2/src/components/contact_controls.py
+-rw-r--r--   0        0        0     4139 2024-04-03 02:17:21.251676 pyrtz2-1.1.9/pyrtz2/src/components/curve_dropdown.py
+-rw-r--r--   0        0        0     3409 2024-04-04 18:23:41.184544 pyrtz2-1.1.9/pyrtz2/src/components/fig.py
+-rw-r--r--   0        0        0     4475 2024-04-04 18:07:38.738998 pyrtz2-1.1.9/pyrtz2/src/components/fig_frame.py
+-rw-r--r--   0        0        0     2393 2024-04-04 18:36:08.361121 pyrtz2-1.1.9/pyrtz2/src/components/fitter.py
+-rw-r--r--   0        0        0     1241 2024-04-04 18:49:04.376522 pyrtz2-1.1.9/pyrtz2/src/components/ids.py
+-rw-r--r--   0        0        0     1195 2024-04-03 02:18:43.224430 pyrtz2-1.1.9/pyrtz2/src/components/image_frame.py
+-rw-r--r--   0        0        0     1666 2024-04-02 01:29:34.764572 pyrtz2-1.1.9/pyrtz2/src/components/layout.py
+-rw-r--r--   0        0        0     3461 2024-04-04 20:44:27.712291 pyrtz2-1.1.9/pyrtz2/src/components/loader.py
+-rw-r--r--   0        0        0     1052 2024-04-04 18:50:12.478289 pyrtz2-1.1.9/pyrtz2/src/components/toolbox.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.9/pyrtz2/src/data/__init__.py
+-rw-r--r--   0        0        0     3346 2024-04-04 20:08:19.361627 pyrtz2-1.1.9/pyrtz2/src/data/downloader.py
+-rw-r--r--   0        0        0     1620 2024-04-04 20:44:13.562141 pyrtz2-1.1.9/pyrtz2/src/data/experiment_loader.py
+-rw-r--r--   0        0        0     1128 2024-04-03 02:24:32.297813 pyrtz2-1.1.9/pyrtz2/src/data/image_loader.py
+-rw-r--r--   0        0        0     1218 2024-04-04 21:40:13.246607 pyrtz2-1.1.9/pyrtz2/src/data/processor.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.9/pyrtz2/src/utils/__init__.py
+-rw-r--r--   0        0        0     1020 2024-03-29 20:53:21.746168 pyrtz2-1.1.9/pyrtz2/src/utils/_backup/igor/__init__.py
+-rw-r--r--   0        0        0    30699 2024-03-29 20:52:56.279210 pyrtz2-1.1.9/pyrtz2/src/utils/_backup/igor/binarywave.py
+-rw-r--r--   0        0        0    29217 2024-03-29 21:12:48.091560 pyrtz2-1.1.9/pyrtz2/src/utils/_backup/igor/structure.py
+-rw-r--r--   0        0        0     3911 2024-02-02 05:34:10.456245 pyrtz2-1.1.9/pyrtz2/src/utils/_backup/igor/util.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.9/pyrtz2/src/utils/_backup/pyrtz/__init__.py
+-rw-r--r--   0        0        0     4623 2024-03-29 23:09:57.877567 pyrtz2-1.1.9/pyrtz2/src/utils/_backup/pyrtz/asylum.py
+-rw-r--r--   0        0        0    35543 2024-03-30 00:31:39.650484 pyrtz2-1.1.9/pyrtz2/src/utils/_backup/pyrtz/curves.py
+-rw-r--r--   0        0        0     2403 2024-04-04 18:28:36.838363 pyrtz2-1.1.9/pyrtz2/src/utils/utils.py
+-rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 pyrtz2-1.1.9/PKG-INFO
```

### Comparing `pyrtz2-1.1.0/LICENSE` & `pyrtz2-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.0/pyrtz2/afm.py` & `pyrtz2-1.1.9/pyrtz2/afm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import copy
 import os
-import asylum
+from . import asylum
 
 
 class AFM():
     def __init__(
         self,
             path: str,
             exp_name: str,
```

### Comparing `pyrtz2-1.1.0/pyrtz2/assets/style.css` & `pyrtz2-1.1.9/pyrtz2/assets/style.css`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.0/pyrtz2/asylum.py` & `pyrtz2-1.1.9/pyrtz2/asylum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from igor2 import binarywave as bw
 import numpy as np
 import pandas as pd
 import re
 import os
 
-import curves
+from . import curves
 
 
 def _get_notes(wave: dict) -> dict:
     '''Utility function for processing the 'notes' section of a .ibw file,
     the end user should not call this function'''
 
     note_raw = wave['wave']['note']
```

### Comparing `pyrtz2-1.1.0/pyrtz2/curves.py` & `pyrtz2-1.1.9/pyrtz2/curves.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import numpy as np
 import json
 import ast
 import io
 from tqdm import tqdm
 from typing import Any, Iterable
 
-from fit import lin_fit, poly_fit, hertzian_fit, biexponential_fit
-from src.components.fig import make_fig
+from .fit import lin_fit, poly_fit, hertzian_fit, biexponential_fit
+from .src.components.fig import make_fig
 
 
 def read_json_file(file: str) -> dict[tuple, bool | int]:
     with open(file, 'rt') as cf:
         anno_str_dict = json.load(cf)
 
     anno_tuple_dict = {}
```

### Comparing `pyrtz2-1.1.0/pyrtz2/fit.py` & `pyrtz2-1.1.9/pyrtz2/fit.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.0/pyrtz2/src/components/annotator.py` & `pyrtz2-1.1.9/pyrtz2/src/components/annotator.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,13 +39,13 @@
     return html.Div(
         children=[
             dcc.Store(id=ids.CP_ANNOTATIONS),
             dcc.Store(id=ids.VD_ANNOTATIONS),
             dcc.Upload(
                 className='drag-drop',
                 children=html.Div(
-                    ['Drag and Drop or ', html.A('Select Annotation File')]),
+                    ['Drag and Drop or ', html.A('Select Annotation File'), ' to Load']),
                 id=ids.UPLOAD_ANNOTATIONS,
                 multiple=False
             ),
         ],
     )
```

### Comparing `pyrtz2-1.1.0/pyrtz2/src/components/contact_controls.py` & `pyrtz2-1.1.9/pyrtz2/src/components/contact_controls.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.0/pyrtz2/src/components/curve_dropdown.py` & `pyrtz2-1.1.9/pyrtz2/src/components/curve_dropdown.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.0/pyrtz2/src/components/fig.py` & `pyrtz2-1.1.9/pyrtz2/src/components/fig.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.0/pyrtz2/src/components/fig_frame.py` & `pyrtz2-1.1.9/pyrtz2/src/components/fig_frame.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.0/pyrtz2/src/components/fitter.py` & `pyrtz2-1.1.9/pyrtz2/src/components/fitter.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.0/pyrtz2/src/components/ids.py` & `pyrtz2-1.1.9/pyrtz2/src/components/ids.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.0/pyrtz2/src/components/image_frame.py` & `pyrtz2-1.1.9/pyrtz2/src/components/image_frame.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.0/pyrtz2/src/components/layout.py` & `pyrtz2-1.1.9/pyrtz2/src/components/layout.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.0/pyrtz2/src/components/loader.py` & `pyrtz2-1.1.9/pyrtz2/src/components/loader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.0/pyrtz2/src/components/toolbox.py` & `pyrtz2-1.1.9/pyrtz2/src/components/toolbox.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.0/pyrtz2/src/data/downloader.py` & `pyrtz2-1.1.9/pyrtz2/src/data/downloader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.0/pyrtz2/src/data/experiment_loader.py` & `pyrtz2-1.1.9/pyrtz2/src/data/experiment_loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dash import Dash, dcc
 from dash.dependencies import Input, Output, State
 from dash.exceptions import PreventUpdate
 import os
 
-from afm import AFM
+from ...afm import AFM
 from ..components import ids
 from ..utils.utils import dump, make_json
 
 
 def render(app: Dash) -> dcc.Store:
     @app.callback(
         [Output(ids.EXPERIMENT, 'data', allow_duplicate=True),
```

### Comparing `pyrtz2-1.1.0/pyrtz2/src/data/image_loader.py` & `pyrtz2-1.1.9/pyrtz2/src/data/image_loader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.0/pyrtz2/src/data/processor.py` & `pyrtz2-1.1.9/pyrtz2/src/data/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import ast
 import json
 import pandas as pd
-import base64
 from io import BytesIO
 
-from afm import AFM
+from ...afm import AFM
 
 
 def process_experiment(experiment: AFM, cp_data: str, vd_data: str, indentation: float | list[float]) -> tuple[AFM, pd.DataFrame]:
     cp_annotations = json.loads(cp_data)
     cp_annotations = {ast.literal_eval(
         key): value for key, value in cp_annotations.items()}
```

### Comparing `pyrtz2-1.1.0/pyrtz2/src/utils/_backup/igor/__init__.py` & `pyrtz2-1.1.9/pyrtz2/src/utils/_backup/igor/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.0/pyrtz2/src/utils/_backup/igor/binarywave.py` & `pyrtz2-1.1.9/pyrtz2/src/utils/_backup/igor/binarywave.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.0/pyrtz2/src/utils/_backup/igor/structure.py` & `pyrtz2-1.1.9/pyrtz2/src/utils/_backup/igor/structure.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.0/pyrtz2/src/utils/_backup/igor/util.py` & `pyrtz2-1.1.9/pyrtz2/src/utils/_backup/igor/util.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.0/pyrtz2/src/utils/_backup/pyrtz/asylum.py` & `pyrtz2-1.1.9/pyrtz2/src/utils/_backup/pyrtz/asylum.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.0/pyrtz2/src/utils/_backup/pyrtz/curves.py` & `pyrtz2-1.1.9/pyrtz2/src/utils/_backup/pyrtz/curves.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.0/pyrtz2/src/utils/utils.py` & `pyrtz2-1.1.9/pyrtz2/src/utils/utils.py`

 * *Files identical despite different names*

