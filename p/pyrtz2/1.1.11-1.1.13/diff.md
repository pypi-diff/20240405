# Comparing `tmp/pyrtz2-1.1.11.tar.gz` & `tmp/pyrtz2-1.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrtz2-1.1.11.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyrtz2-1.1.13.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyrtz2-1.1.11.tar` & `pyrtz2-1.1.13.tar`

### file list

```diff
@@ -1,40 +1,51 @@
--rw-r--r--   0        0        0       66 2024-04-02 19:47:59.285340 pyrtz2-1.1.11/.gitattributes
--rw-r--r--   0        0        0       20 2024-04-04 22:35:31.627883 pyrtz2-1.1.11/.gitignore
--rw-r--r--   0        0        0    33041 2024-04-02 20:07:11.768711 pyrtz2-1.1.11/LICENSE
--rw-r--r--   0        0        0      228 2024-04-02 19:51:47.632334 pyrtz2-1.1.11/README.md
--rw-r--r--   0        0        0      794 2024-04-04 21:36:24.676720 pyrtz2-1.1.11/pyproject.toml
--rw-r--r--   0        0        0       62 2024-04-05 02:11:21.366282 pyrtz2-1.1.11/pyrtz2/__init__.py
--rw-r--r--   0        0        0     1874 2024-04-04 20:43:57.261121 pyrtz2-1.1.11/pyrtz2/afm.py
--rw-r--r--   0        0        0      359 2024-04-05 02:11:14.258329 pyrtz2-1.1.11/pyrtz2/app.py
--rw-r--r--   0        0        0     1320 2024-03-29 18:30:21.132859 pyrtz2-1.1.11/pyrtz2/assets/style.css
--rw-r--r--   0        0        0     4718 2024-04-04 20:43:28.570132 pyrtz2-1.1.11/pyrtz2/asylum.py
--rw-r--r--   0        0        0    20124 2024-04-04 20:43:38.173145 pyrtz2-1.1.11/pyrtz2/curves.py
--rw-r--r--   0        0        0     4451 2024-04-02 14:59:14.529838 pyrtz2-1.1.11/pyrtz2/fit.py
--rw-r--r--   0        0        0        0 2024-04-03 01:57:24.101285 pyrtz2-1.1.11/pyrtz2/src/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.11/pyrtz2/src/components/__init__.py
--rw-r--r--   0        0        0     1982 2024-04-04 23:28:38.697339 pyrtz2-1.1.11/pyrtz2/src/components/annotator.py
--rw-r--r--   0        0        0     5604 2024-04-04 18:49:51.040442 pyrtz2-1.1.11/pyrtz2/src/components/contact_controls.py
--rw-r--r--   0        0        0     4139 2024-04-03 02:17:21.251676 pyrtz2-1.1.11/pyrtz2/src/components/curve_dropdown.py
--rw-r--r--   0        0        0     3409 2024-04-04 18:23:41.184544 pyrtz2-1.1.11/pyrtz2/src/components/fig.py
--rw-r--r--   0        0        0     4525 2024-04-05 00:22:08.628868 pyrtz2-1.1.11/pyrtz2/src/components/fig_frame.py
--rw-r--r--   0        0        0     2393 2024-04-04 18:36:08.361121 pyrtz2-1.1.11/pyrtz2/src/components/fitter.py
--rw-r--r--   0        0        0     1241 2024-04-04 18:49:04.376522 pyrtz2-1.1.11/pyrtz2/src/components/ids.py
--rw-r--r--   0        0        0     1195 2024-04-03 02:18:43.224430 pyrtz2-1.1.11/pyrtz2/src/components/image_frame.py
--rw-r--r--   0        0        0     1666 2024-04-02 01:29:34.764572 pyrtz2-1.1.11/pyrtz2/src/components/layout.py
--rw-r--r--   0        0        0     3461 2024-04-04 20:44:27.712291 pyrtz2-1.1.11/pyrtz2/src/components/loader.py
--rw-r--r--   0        0        0     1052 2024-04-04 18:50:12.478289 pyrtz2-1.1.11/pyrtz2/src/components/toolbox.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.11/pyrtz2/src/data/__init__.py
--rw-r--r--   0        0        0     3346 2024-04-04 20:08:19.361627 pyrtz2-1.1.11/pyrtz2/src/data/downloader.py
--rw-r--r--   0        0        0     1824 2024-04-05 02:11:14.359347 pyrtz2-1.1.11/pyrtz2/src/data/experiment_loader.py
--rw-r--r--   0        0        0     1131 2024-04-05 02:11:14.364347 pyrtz2-1.1.11/pyrtz2/src/data/image_loader.py
--rw-r--r--   0        0        0     1218 2024-04-04 21:40:13.246607 pyrtz2-1.1.11/pyrtz2/src/data/processor.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.11/pyrtz2/src/utils/__init__.py
--rw-r--r--   0        0        0     1020 2024-03-29 20:53:21.746168 pyrtz2-1.1.11/pyrtz2/src/utils/_backup/igor/__init__.py
--rw-r--r--   0        0        0    30699 2024-03-29 20:52:56.279210 pyrtz2-1.1.11/pyrtz2/src/utils/_backup/igor/binarywave.py
--rw-r--r--   0        0        0    29217 2024-03-29 21:12:48.091560 pyrtz2-1.1.11/pyrtz2/src/utils/_backup/igor/structure.py
--rw-r--r--   0        0        0     3911 2024-02-02 05:34:10.456245 pyrtz2-1.1.11/pyrtz2/src/utils/_backup/igor/util.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.11/pyrtz2/src/utils/_backup/pyrtz/__init__.py
--rw-r--r--   0        0        0     4623 2024-03-29 23:09:57.877567 pyrtz2-1.1.11/pyrtz2/src/utils/_backup/pyrtz/asylum.py
--rw-r--r--   0        0        0    35543 2024-03-30 00:31:39.650484 pyrtz2-1.1.11/pyrtz2/src/utils/_backup/pyrtz/curves.py
--rw-r--r--   0        0        0     2403 2024-04-05 00:44:05.466747 pyrtz2-1.1.11/pyrtz2/src/utils/utils.py
--rw-r--r--   0        0        0      976 1970-01-01 00:00:00.000000 pyrtz2-1.1.11/PKG-INFO
+-rw-r--r--   0        0        0       66 2024-04-02 19:47:59.285340 pyrtz2-1.1.13/.gitattributes
+-rw-r--r--   0        0        0       37 2024-04-05 12:35:50.341792 pyrtz2-1.1.13/.gitignore
+-rw-r--r--   0        0        0    33041 2024-04-02 20:07:11.768711 pyrtz2-1.1.13/LICENSE
+-rw-r--r--   0        0        0      228 2024-04-02 19:51:47.632334 pyrtz2-1.1.13/README.md
+-rw-r--r--   0        0        0   442996 2024-03-22 20:48:12.000000 pyrtz2-1.1.13/example/con050/jasYcon050cell37m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:48:22.000000 pyrtz2-1.1.13/example/con050/jasYcon050cell37m0001.tif
+-rw-r--r--   0        0        0   453575 2024-03-22 20:48:52.000000 pyrtz2-1.1.13/example/con050/jasYcon050cell38m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:49:00.000000 pyrtz2-1.1.13/example/con050/jasYcon050cell38m0001.tif
+-rw-r--r--   0        0        0   458723 2024-03-22 20:49:32.000000 pyrtz2-1.1.13/example/con050/jasYcon050cell39m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:49:38.000000 pyrtz2-1.1.13/example/con050/jasYcon050cell39m0001.tif
+-rw-r--r--   0        0        0   435180 2024-03-22 20:50:14.000000 pyrtz2-1.1.13/example/con050/jasYcon050cell40m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:50:22.000000 pyrtz2-1.1.13/example/con050/jasYcon050cell40m0001.tif
+-rw-r--r--   0        0        0   922624 2024-03-22 20:51:28.000000 pyrtz2-1.1.13/example/con050/jasYcon050cell41m0000.tif
+-rw-r--r--   0        0        0   922624 2024-03-22 20:51:56.000000 pyrtz2-1.1.13/example/con050/jasYcon050cell41m0001.tif
+-rw-r--r--   0        0        0   457660 2024-03-22 20:54:28.000000 pyrtz2-1.1.13/example/con050/jasYcon050cell42m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:54:36.000000 pyrtz2-1.1.13/example/con050/jasYcon050cell42m0001.tif
+-rw-r--r--   0        0        0      196 2024-03-27 20:17:56.223149 pyrtz2-1.1.13/example/con050_cp_annotations.json
+-rw-r--r--   0        0        0      205 2024-03-26 23:15:37.330282 pyrtz2-1.1.13/example/con050_vd_annotations.json
+-rw-r--r--   0        0        0      196 2024-03-27 20:17:56.223149 pyrtz2-1.1.13/example/con111_cp_annotations.json
+-rw-r--r--   0        0        0   331740 2024-04-04 23:26:50.939244 pyrtz2-1.1.13/example/con111_curves.pdf
+-rw-r--r--   0        0        0     1749 2024-04-04 23:26:34.450692 pyrtz2-1.1.13/example/con111_fits.csv
+-rw-r--r--   0        0        0      205 2024-03-26 23:15:37.330282 pyrtz2-1.1.13/example/con111_vd_annotations.json
+-rw-r--r--   0        0        0      794 2024-04-04 21:36:24.676720 pyrtz2-1.1.13/pyproject.toml
+-rw-r--r--   0        0        0       62 2024-04-05 12:42:00.629914 pyrtz2-1.1.13/pyrtz2/__init__.py
+-rw-r--r--   0        0        0     1874 2024-04-04 20:43:57.261121 pyrtz2-1.1.13/pyrtz2/afm.py
+-rw-r--r--   0        0        0      358 2024-04-05 12:35:50.349791 pyrtz2-1.1.13/pyrtz2/app.py
+-rw-r--r--   0        0        0     1320 2024-03-29 18:30:21.132859 pyrtz2-1.1.13/pyrtz2/assets/style.css
+-rw-r--r--   0        0        0     4718 2024-04-04 20:43:28.570132 pyrtz2-1.1.13/pyrtz2/asylum.py
+-rw-r--r--   0        0        0    20707 2024-04-05 12:35:50.353795 pyrtz2-1.1.13/pyrtz2/curves.py
+-rw-r--r--   0        0        0     4451 2024-04-02 14:59:14.529838 pyrtz2-1.1.13/pyrtz2/fit.py
+-rw-r--r--   0        0        0        0 2024-04-03 01:57:24.101285 pyrtz2-1.1.13/pyrtz2/src/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.13/pyrtz2/src/components/__init__.py
+-rw-r--r--   0        0        0     1982 2024-04-04 23:28:38.697339 pyrtz2-1.1.13/pyrtz2/src/components/annotator.py
+-rw-r--r--   0        0        0     5060 2024-04-05 12:35:50.358816 pyrtz2-1.1.13/pyrtz2/src/components/contact_controls.py
+-rw-r--r--   0        0        0     4139 2024-04-03 02:17:21.251676 pyrtz2-1.1.13/pyrtz2/src/components/curve_dropdown.py
+-rw-r--r--   0        0        0     3046 2024-04-05 12:35:50.362793 pyrtz2-1.1.13/pyrtz2/src/components/fig.py
+-rw-r--r--   0        0        0     3295 2024-04-05 12:35:50.366794 pyrtz2-1.1.13/pyrtz2/src/components/fig_frame.py
+-rw-r--r--   0        0        0     2393 2024-04-04 18:36:08.361121 pyrtz2-1.1.13/pyrtz2/src/components/fitter.py
+-rw-r--r--   0        0        0     1194 2024-04-05 12:35:50.370793 pyrtz2-1.1.13/pyrtz2/src/components/ids.py
+-rw-r--r--   0        0        0     1221 2024-04-05 12:35:50.375793 pyrtz2-1.1.13/pyrtz2/src/components/image_frame.py
+-rw-r--r--   0        0        0     1666 2024-04-02 01:29:34.764572 pyrtz2-1.1.13/pyrtz2/src/components/layout.py
+-rw-r--r--   0        0        0     3408 2024-04-05 12:35:50.379817 pyrtz2-1.1.13/pyrtz2/src/components/loader.py
+-rw-r--r--   0        0        0     1052 2024-04-04 18:50:12.478289 pyrtz2-1.1.13/pyrtz2/src/components/toolbox.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.13/pyrtz2/src/data/__init__.py
+-rw-r--r--   0        0        0     3307 2024-04-05 12:39:49.693713 pyrtz2-1.1.13/pyrtz2/src/data/downloader.py
+-rw-r--r--   0        0        0     1560 2024-04-05 12:35:50.388794 pyrtz2-1.1.13/pyrtz2/src/data/experiment_loader.py
+-rw-r--r--   0        0        0     1117 2024-04-05 12:35:50.392818 pyrtz2-1.1.13/pyrtz2/src/data/image_loader.py
+-rw-r--r--   0        0        0     1218 2024-04-04 21:40:13.246607 pyrtz2-1.1.13/pyrtz2/src/data/processor.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.13/pyrtz2/src/utils/__init__.py
+-rw-r--r--   0        0        0     2474 2024-04-05 12:35:50.397796 pyrtz2-1.1.13/pyrtz2/src/utils/utils.py
+-rw-r--r--   0        0        0      976 1970-01-01 00:00:00.000000 pyrtz2-1.1.13/PKG-INFO
```

### Comparing `pyrtz2-1.1.11/LICENSE` & `pyrtz2-1.1.13/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.11/pyproject.toml` & `pyrtz2-1.1.13/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.11/pyrtz2/afm.py` & `pyrtz2-1.1.13/pyrtz2/afm.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.11/pyrtz2/assets/style.css` & `pyrtz2-1.1.13/pyrtz2/assets/style.css`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.11/pyrtz2/asylum.py` & `pyrtz2-1.1.13/pyrtz2/asylum.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.11/pyrtz2/curves.py` & `pyrtz2-1.1.13/pyrtz2/curves.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,613 +1,612 @@
-from plotly import graph_objs as go
-import plotly.express as px
-
-import PyPDF2 as pdf
-import pickle
-import pandas as pd
-import numpy as np
-import json
-import ast
-import io
-from tqdm import tqdm
-from typing import Any, Iterable
-
-from .fit import lin_fit, poly_fit, hertzian_fit, biexponential_fit
-from .src.components.fig import make_fig
-
-
-def read_json_file(file: str) -> dict[tuple, bool | int]:
-    with open(file, 'rt') as cf:
-        anno_str_dict = json.load(cf)
-
-    anno_tuple_dict = {}
-    for key, value in anno_str_dict.items():
-        tuple_key = ast.literal_eval(key)
-        anno_tuple_dict[tuple_key] = value
-
-    return anno_tuple_dict
-
-
-class Curve:
-
-    _data: pd.DataFrame
-    corrected: bool = False
-    contact_index: int = 0
-    contact_values: pd.Series | None = None
-    max_ind: float
-    max_f: float
-    vel_ind: float
-    vel_z: float
-    figs_data: dict[str, tuple[np.ndarray, np.ndarray]]
-    fits_data: dict[str, tuple[np.ndarray, np.ndarray]]
-    indent_param: list[float]
-    indent_R2: float
-    hertzian_param: list[float]
-    hertzian_R2: float
-    dwell_param: list[float]
-    dwell_R2: float
-    relaxation_param: list[float]
-    relaxation_R2: float
-    contact_fig: go.Figure
-    dwell_relax_fig: go.Figure
-
-    def __init__(
-            self,
-            filename: str,
-            data: pd.DataFrame,
-            notes: dict,
-            invOLS: float,
-            k: float,
-            dwell_range: list[int],
-    ) -> None:
-
-        self.filename = filename
-        self.data = data
-        self.notes = notes
-        self.invOLS = invOLS
-        self.k = k
-        self.dwell_range = dwell_range
-
-        self.backup_data()
-
-    def backup_data(self) -> None:
-        self._data = self.data.copy()
-
-    def restore_data(self) -> None:
-        self.data = self._data.copy()
-
-    def reduce_data(self) -> None:
-        self.data.drop(['rawz', 'defl'], axis=1, inplace=True)
-
-    def set_contact_index(self, cp: int) -> None:
-        self.contact_index = cp
-
-    def check_contact(self) -> None:
-        if self.contact_index == 0:
-            raise Exception('Contact index has not been set.')
-
-    def get_contact_values(self) -> pd.Series:
-        self.check_contact()
-        if self.contact_values is None:
-            self.contact_values = self.data.iloc[self.contact_index].copy()
-        return self.contact_values
-
-    def adjust_to_contact(self) -> None:
-        self.data -= self.get_contact_values()
-
-    def get_data_between(self, start: int, last: int) -> pd.DataFrame:
-        return self.data.iloc[start:last].reset_index(drop=True)
-
-    def get_approach(self) -> pd.DataFrame:
-        return self.get_data_between(0, self.dwell_range[0])
-
-    def get_preapproach(self) -> pd.DataFrame:
-        return self.get_data_between(0, self.contact_index)
-
-    def get_indent(self) -> pd.DataFrame:
-        return self.get_data_between(self.contact_index, self.dwell_range[0])
-
-    def get_indent_until(self, ind: float) -> pd.DataFrame:
-        indent = self.get_indent()
-        ind_index = (np.abs(indent['ind'].to_numpy() - ind)).argmin()
-        return indent.iloc[:ind_index].reset_index(drop=True)
-
-    def get_indent_between(self, start: float, last: float) -> pd.DataFrame:
-        indent = self.get_indent()
-        start_index = int(start * len(indent))
-        last_index = int(last * len(indent))
-        return indent.iloc[start_index:last_index].reset_index(drop=True)
-
-    def get_dwell(self) -> pd.DataFrame:
-        return self.get_data_between(self.dwell_range[0], self.dwell_range[1])
-
-    def get_relaxation(self) -> pd.DataFrame:
-        dwell = self.get_dwell()
-        max_ind = dwell['ind'].argmax()
-        return dwell.iloc[:max_ind].reset_index(drop=True)
-
-    def get_repulsion(self) -> pd.DataFrame:
-        dwell = self.get_dwell()
-        max_ind = dwell['ind'].argmax()
-        return dwell.iloc[max_ind:].reset_index(drop=True)
-
-    def get_retract(self) -> pd.DataFrame:
-        return self.get_data_between(self.dwell_range[1], -1)
-
-    def get_trigger_data(self) -> pd.Series:
-        indent = self.get_indent()
-        return indent.iloc[-1].reset_index(drop=True)
-
-    def get_approach_rates(self) -> None:
-        indent = self.get_indent()
-        t, ind, z = indent['t'], indent['ind'], indent['z']
-        self.vel_ind = lin_fit(t, ind)[0][0]
-        self.vel_z = lin_fit(t, z)[0][0]
-
-    def correct_virtual_defl(self) -> None:
-        self.check_contact()
-        if self.corrected:
-            self.restore_data()
-
-        preapproach = self.get_preapproach()
-        x = preapproach['z'].to_numpy()
-        y = preapproach['f'].to_numpy()
-        popt, _, _ = lin_fit(x, y)
-        f_line = np.poly1d(popt)(self.data['z'])
-        self.data['f'] = self.data['f'] - f_line
-
-    def detect_contact(self) -> int:
-        current_contact_index = self.contact_index
-        approach = self.get_approach()
-        max_index = len(approach) - 1
-        index = max_index
-        while True:
-            self.set_contact_index(index)
-            self.correct_virtual_defl()
-            approach_new = self.get_approach()
-            force = approach_new['f'].to_numpy()
-            mean = np.mean(force[:index+1])
-
-            ratio = force[index] / force[-1]
-            step_size = max(1, int((0.01 * max_index) ** ratio))
-            index = index - step_size
-            if force[index] < mean:
-                contact_index = index + 1
-                break
-
-        self.set_contact_index(current_contact_index)
-        self.restore_data()
-        return contact_index
-
-    def fit_indent(self) -> tuple:
-        self.check_contact()
-        indent = self.get_indent()
-        return poly_fit(indent['ind'], indent['f'])
-
-    def fit_indent_until(self, probe_diameter: float, ind: float) -> tuple:
-        self.check_contact()
-        indent_until = self.get_indent_until(ind)
-        return hertzian_fit(indent_until['ind'], indent_until['f'], probe_diameter)
-
-    def fit_indent_between(self, probe_diameter: float, interval: list[float] = [0.0, 1.0]) -> tuple:
-        self.check_contact()
-        indent_between = self.get_indent_between(interval[0], interval[1])
-        return hertzian_fit(indent_between['ind'], indent_between['f'], probe_diameter)
-
-    def fit_dwell(self) -> tuple:
-        dwell = self.get_dwell()
-        return biexponential_fit(dwell['t'], dwell['f'])
-
-    def fit_relaxation(self) -> tuple:
-        relaxation = self.get_relaxation()
-        return biexponential_fit(relaxation['t'], relaxation['ind'])
-
-    def get_figs_data(self, vd: bool = False, adjust: bool = False) -> None:
-        if vd or adjust:
-            self.restore_data()
-        if vd:
-            self.correct_virtual_defl()
-        if adjust:
-            self.adjust_to_contact()
-
-        approach = self.get_approach()
-
-        dwell = self.get_dwell()
-        relaxation = self.get_relaxation()
-
-        self.figs_data = {
-            'approach': (approach['ind'].to_numpy(), approach['f'].to_numpy()),
-            'dwell': (dwell['t'].to_numpy(), dwell['f'].to_numpy()),
-            'relaxation': (relaxation['t'].to_numpy(), relaxation['ind'].to_numpy()),
-        }
-
-    def get_contact_fig_plot(self) -> go.Figure:
-        fig = make_fig(
-            title=fr"$\text{{Selected Contact Point: {self.contact_index}}}$",
-            xaxis=r"$Indentation \text{ (m)}$"
-        )
-
-        x, y = self.figs_data['approach']
-        hover_texts = [f'Index: {i}' for i in range(len(x))]
-        trace = go.Scattergl(
-            x=x,
-            y=y,
-            name='Approach',
-            mode='markers',
-            text=hover_texts,
-            hoverinfo='text',
-            hoverlabel={'bgcolor': 'red'},
-            marker={'color': 'blue'},
-        )
-
-        fig.add_trace(trace)
-
-        x_line = x[self.contact_index]
-        y_line = y[self.contact_index]
-        fig.add_vline(x=x_line, line=dict(color='red', width=1.2))
-        fig.add_hline(y=y_line, line=dict(color='red', width=1.2))
-        self.contact_fig = fig
-        return fig
-
-    def get_dwell_relax_fig_plot(self) -> go.Figure:
-        fig = make_fig(
-            title=r"$\text{Dwell and Relaxation}$",
-            xaxis=r"$Time \text{ (s)}$"
-        )
-
-        fig.update_layout(
-            yaxis2=dict(
-                title=r"$Indentation \text{ (m)}$",
-                overlaying='y',
-                side='right'
-            )
-        )
-
-        x, y = self.figs_data['dwell']
-        trace = go.Scattergl(
-            x=x,
-            y=y,
-            name='Dwell',
-            mode='markers',
-            marker={'color': 'red'},
-        )
-
-        fig.add_trace(trace)
-
-        x, y = self.figs_data['relaxation']
-        trace = go.Scattergl(
-            x=x,
-            y=y,
-            yaxis='y2',
-            name='Relaxation',
-            mode='markers',
-            marker={'color': 'blue'},
-        )
-
-        fig.add_trace(trace)
-
-        self.dwell_relax_fig = fig
-        return fig
-
-    def get_fits_data(self, probe_diameter: float, ind: float | list[float]) -> None:
-        indent = self.get_indent()
-        indent_x_pred = indent['ind'].to_numpy()
-        self.indent_param, self.indent_R2, indent_y_pred = self.fit_indent()
-
-        self.max_ind = max(indent['ind'])
-        self.max_f = max(indent['f'])
-
-        if isinstance(ind, float):
-            self.hertzian_param, self.hertzian_R2, hertzian_y_pred = self.fit_indent_until(
-                probe_diameter, ind)
-            hertzian_x_pred = self.get_indent_until(ind)['ind'].to_numpy()
-        elif isinstance(ind, list) and len(ind) == 2:
-            self.hertzian_param, self.hertzian_R2, hertzian_y_pred = self.fit_indent_between(
-                probe_diameter, interval=ind)
-            hertzian_x_pred = self.get_indent_between(ind[0], ind[1])[
-                'ind'].to_numpy()
-
-        dwell = self.get_dwell()
-        dwell_x_pred = dwell['t'].to_numpy()
-        self.dwell_param, self.dwell_R2, dwell_y_pred = self.fit_dwell()
-
-        relaxation = self.get_relaxation()
-        relaxation_x_pred = relaxation['t'].to_numpy()
-        self.relaxation_param, self.relaxation_R2, relaxation_y_pred = self.fit_relaxation()
-
-        self.fits_data = {
-            'indent': (indent_x_pred, indent_y_pred),
-            'hertzian': (hertzian_x_pred, hertzian_y_pred),
-            'dwell': (dwell_x_pred, dwell_y_pred),
-            'relaxation': (relaxation_x_pred, relaxation_y_pred),
-        }
-
-    def add_contact_fit(self) -> go.Figure:
-        x, y = self.fits_data['indent']
-        trace = go.Scattergl(
-            x=x,
-            y=y,
-            name='PolyFit',
-            mode='lines',
-            line={'color': 'red'},
-        )
-        self.contact_fig.add_trace(trace)
-
-        x, y = self.fits_data['hertzian']
-        trace = go.Scattergl(
-            x=x,
-            y=y,
-            name='HertzianFit',
-            mode='lines',
-            line={
-                'color': 'green',
-                'width': 3,
-            },
-        )
-        self.contact_fig.add_trace(trace)
-
-        return self.contact_fig
-
-    def add_dwell_relax_fit(self) -> go.Figure:
-        x, y = self.fits_data['dwell']
-
-        trace = go.Scattergl(
-            x=x,
-            y=y,
-            name='DwellFit',
-            mode='lines',
-            line={
-                'color': 'green',
-                'width': 3,
-            },
-        )
-        self.dwell_relax_fig.add_trace(trace)
-
-        x, y = self.fits_data['relaxation']
-        trace = go.Scattergl(
-            x=x,
-            y=y,
-            yaxis='y2',
-            name='RelaxationFit',
-            mode='lines',
-            line={
-                'color': 'green',
-                'width': 3,
-            },
-        )
-        self.dwell_relax_fig.add_trace(trace)
-
-        return self.dwell_relax_fig
-
-    def get_contact_fig_pdf(self) -> go.Figure:
-        title = fr"$\text{{Selected Contact Point: {self.contact_index}}}$"
-        xaxis = r"$Indentation \text{ (m)}$"
-        fig = make_fig(title, xaxis)
-
-        x, y = self.figs_data['approach']
-        trace = go.Scatter(x=x, y=y, name='Approach', marker={'color': 'blue'})
-        fig.add_trace(trace)
-
-        x_line = x[self.contact_index]
-        y_line = y[self.contact_index]
-        fig.add_shape(type='line', x0=x_line, x1=x_line, y0=min(y),
-                      y1=max(y), line=dict(color='red', width=1.2))
-        fig.add_shape(type='line', y0=y_line, y1=y_line, x0=min(x),
-                      x1=max(x), line=dict(color='red', width=1.2))
-
-        if hasattr(self, 'fits_data'):
-            x, y = self.fits_data['indent']
-            trace = go.Scatter(x=x, y=y, name='PolyFit',
-                               mode='lines', line={'color': 'red'})
-            fig.add_trace(trace)
-
-            x, y = self.fits_data['hertzian']
-            trace = go.Scatter(x=x, y=y, name='HertzianFit',
-                               mode='lines', line={'color': 'green', 'width': 3})
-            fig.add_trace(trace)
-
-        return fig
-
-    def get_dwell_relax_fig_pdf(self) -> go.Figure:
-        title = r"$\text{Dwell and Relaxation}$"
-        xaxis = r"$Time \text{ (s)}$"
-        fig = make_fig(title, xaxis)
-
-        x, y = self.figs_data['dwell']
-        trace = go.Scatter(x=x, y=y, name='Dwell',
-                           marker_color='red')
-        fig.add_trace(trace)
-
-        fig.update_layout(
-            yaxis2=dict(
-                title=r"$Indentation \text{ (m)}$",
-                overlaying='y',
-                side='right',
-                showgrid=False,
-                ticks='outside',
-                tickwidth=2,
-                showline=True,
-                linewidth=2,
-                linecolor='black',
-                tickprefix=r"$",
-                ticksuffix=r"$",
-            )
-        )
-
-        x, y = self.figs_data['relaxation']
-        trace = go.Scatter(x=x, y=y, name='Relaxation',
-                           marker_color='blue', yaxis='y2')
-        fig.add_trace(trace)
-
-        if hasattr(self, 'fits_data'):
-            x, y = self.fits_data['dwell']
-            trace = go.Scatter(x=x, y=y, name='DwellFit',
-                               mode='lines', line={'color': 'green', 'width': 3})
-            fig.add_trace(trace)
-
-            x, y = self.fits_data['relaxation']
-            trace = go.Scatter(x=x, y=y, yaxis='y2', name='RelaxationFit',
-                               mode='lines', line={'color': 'green', 'width': 3})
-            fig.add_trace(trace)
-
-        return fig
-
-    def get_all_fits(self) -> dict:
-        fit_results_dict = {
-            'max_ind': self.max_ind,
-            'max_f': self.max_f,
-
-            'vel_ind': self.vel_ind,
-            'vel_z': self.vel_z,
-
-            'indent_a': self.indent_param[0],
-            'indent_b': self.indent_param[1],
-            'indent_c': self.indent_param[2],
-            'indent_R2': self.indent_R2,
-
-            'Hertzian_E': self.hertzian_param[0],
-            'Hertzian_R2': self.hertzian_R2,
-
-            'dwell_c': self.dwell_param[0],
-            'dwell_tau1': self.dwell_param[1],
-            'dwell_tau2': self.dwell_param[2],
-            'dwell_tauMax': max(self.dwell_param[1], self.dwell_param[2]),
-            'dwell_tauMin': min(self.dwell_param[1], self.dwell_param[2]),
-            'dwell_yf': self.dwell_param[3],
-            'dwell_R2': self.dwell_R2,
-
-            'relaxation_c': self.relaxation_param[0],
-            'relaxation_tau1': self.relaxation_param[1],
-            'relaxation_tau2': self.relaxation_param[2],
-            'relaxation_tauMax': max(self.relaxation_param[1], self.relaxation_param[2]),
-            'relaxation_tauMin': min(self.relaxation_param[1], self.relaxation_param[2]),
-            'relaxation_yf': self.relaxation_param[3],
-            'relaxation_R2': self.relaxation_R2
-        }
-
-        return fit_results_dict
-
-
-class CurveSet:
-    vd_dict: dict[tuple[str], bool] = {}
-    cp_dict: dict[tuple[str], int] = {}
-
-    def __init__(self, ident_labels: list[str], curve_dict: dict[tuple[str], Curve]) -> None:
-
-        self.ident_labels = ident_labels
-        self.curve_dict = curve_dict
-        self._index = 0
-
-    def __iter__(self):
-        self._index = 0
-        return self
-
-    def __next__(self) -> Curve:
-        if self._index < len(self.curve_dict):
-            key = list(self.curve_dict.keys())[self._index]
-            self._index += 1
-            return self.curve_dict[key]
-        else:
-            raise StopIteration
-
-    def __getitem__(self, key: tuple[str]) -> Curve:
-        return self.curve_dict[key]
-
-    def items(self) -> Iterable[tuple[tuple[str], Curve]]:
-        return self.curve_dict.items()
-
-    def pickle(self, filename: str) -> None:
-        with open(filename, 'wb') as f:
-            pickle.dump(self, f)
-
-    def keys(self) -> list[tuple[str]]:
-        return list(self.curve_dict.keys())
-
-    def reduce_data(self) -> None:
-        for curve in self:
-            curve.reduce_data()
-
-    def remove_curve(self, key: tuple[str]) -> None:
-        del self.curve_dict[key]
-
-    def remove_unannotated(self) -> None:
-        keys_to_remove = []
-        for key, curve in self.items():
-            if curve.contact_index == 0:
-                keys_to_remove.append(key)
-
-        for key in keys_to_remove:
-            self.remove_curve(key)
-
-    def correct_all_virtual_defl(self) -> None:
-        for curve in self:
-            curve.correct_virtual_defl()
-
-    def set_vd_by_annotations(self) -> None:
-        for key, value in self.vd_dict.items():
-            if value:
-                self[key].correct_virtual_defl()
-
-    def set_cp_by_annotations(self) -> None:
-        for key, value in self.cp_dict.items():
-            self[key].set_contact_index(value)
-
-    def update_annotations(self, annotations_dict: dict[tuple[str], Any]) -> None:
-        value = next(iter(annotations_dict.values()))
-        if isinstance(value, bool):
-            self.vd_dict = annotations_dict
-        elif isinstance(value, int):
-            self.cp_dict = annotations_dict
-
-    def update_annotations_from_file(self, file: str) -> None:
-        anno_tuple_dict = read_json_file(file)
-        self.update_annotations(anno_tuple_dict)
-
-    def adjust_to_contact(self) -> None:
-        for curve in self:
-            curve.adjust_to_contact()
-
-    def prepare_fit_all(self) -> None:
-        self.set_cp_by_annotations()
-        self.remove_unannotated()
-        self.set_vd_by_annotations()
-        self.adjust_to_contact()
-
-    def get_fit_all(self, probe_diameter: float, ind: float | list[float]) -> pd.DataFrame:
-        self.prepare_fit_all()
-        all_fit = []
-
-        for key, curve in tqdm(self.items()):
-            fit_results_dict = {label: key_value for label,
-                                key_value in zip(self.ident_labels, key)}
-            curve.get_fits_data(probe_diameter, ind)
-            curve.get_approach_rates()
-            fit_results_dict.update(curve.get_all_fits())
-            fit_results = pd.DataFrame([fit_results_dict])
-            all_fit.append(fit_results)
-
-        combined_results = pd.concat(all_fit, ignore_index=True)
-
-        return combined_results
-
-    def export_figures(self) -> pdf.PdfMerger:
-        merger = pdf.PdfMerger()
-        for key, curve in tqdm(self.items()):
-            curve.get_figs_data()
-            title = ""
-            for label, ident in zip(self.ident_labels, key):
-                title += label + ident
-
-            title = fr"$\text{{{title}}}$"
-            contact_fit_fig = curve.get_contact_fig_pdf()
-            contact_fit_fig.update_layout(title={'text': title})
-            contact_fit_fig_pdf = io.BytesIO(
-                contact_fit_fig.to_image(format='pdf'))
-            merger.append(contact_fit_fig_pdf)
-
-            dwell_relaxation_fit_fig = curve.get_dwell_relax_fig_pdf()
-            dwell_relaxation_fit_fig.update_layout(title={'text': title})
-            dwell_relaxation_fit_fig_pdf = io.BytesIO(
-                dwell_relaxation_fit_fig.to_image(format='pdf'))
-            merger.append(dwell_relaxation_fit_fig_pdf)
-
-        return merger
+from plotly import graph_objs as go
+import plotly.express as px
+
+import PyPDF2 as pdf
+import pickle
+import pandas as pd
+import numpy as np
+import json
+import ast
+import io
+from tqdm import tqdm
+from typing import Any, Iterable
+
+from .fit import lin_fit, poly_fit, hertzian_fit, biexponential_fit
+from .src.components.fig import make_fig
+
+
+def read_json_file(file: str) -> dict[tuple, bool | int]:
+    with open(file, 'rt') as cf:
+        anno_str_dict = json.load(cf)
+
+    anno_tuple_dict = {}
+    for key, value in anno_str_dict.items():
+        tuple_key = ast.literal_eval(key)
+        anno_tuple_dict[tuple_key] = value
+
+    return anno_tuple_dict
+
+
+class Curve:
+
+    _data: pd.DataFrame
+    corrected: bool = False
+    contact_index: int = 0
+    contact_values: pd.Series | None = None
+    max_ind: float
+    max_f: float
+    vel_ind: float
+    vel_z: float
+    figs_data: dict[str, tuple[np.ndarray, np.ndarray]]
+    fits_data: dict[str, tuple[np.ndarray, np.ndarray]]
+    indent_param: list[float]
+    indent_R2: float
+    hertzian_param: list[float]
+    hertzian_R2: float
+    dwell_param: list[float]
+    dwell_R2: float
+    relaxation_param: list[float]
+    relaxation_R2: float
+    contact_fig: go.Figure
+    dwell_relax_fig: go.Figure
+
+    def __init__(
+            self,
+            filename: str,
+            data: pd.DataFrame,
+            notes: dict,
+            invOLS: float,
+            k: float,
+            dwell_range: list[int],
+    ) -> None:
+
+        self.filename = filename
+        self.data = data
+        self.notes = notes
+        self.invOLS = invOLS
+        self.k = k
+        self.dwell_range = dwell_range
+
+        self.backup_data()
+
+    def backup_data(self) -> None:
+        self._data = self.data.copy()
+
+    def restore_data(self) -> None:
+        self.data = self._data.copy()
+
+    def reduce_data(self) -> None:
+        self.data.drop(['rawz', 'defl'], axis=1, inplace=True)
+
+    def set_contact_index(self, cp: int) -> None:
+        self.contact_index = cp
+
+    def check_contact(self) -> None:
+        if self.contact_index == 0:
+            raise Exception('Contact index has not been set.')
+
+    def get_contact_values(self) -> pd.Series:
+        if self.contact_values is None:
+            self.contact_values = self.data.iloc[self.contact_index].copy()
+        return self.contact_values
+
+    def adjust_to_contact(self) -> None:
+        self.data -= self.get_contact_values()
+
+    def get_data_between(self, start: int, last: int) -> pd.DataFrame:
+        return self.data.iloc[start:last].reset_index(drop=True)
+
+    def get_approach(self) -> pd.DataFrame:
+        return self.get_data_between(0, self.dwell_range[0])
+
+    def get_preapproach(self) -> pd.DataFrame:
+        return self.get_data_between(0, self.contact_index)
+
+    def get_indent(self) -> pd.DataFrame:
+        return self.get_data_between(self.contact_index, self.dwell_range[0])
+
+    def get_indent_until(self, ind: float) -> pd.DataFrame:
+        indent = self.get_indent()
+        ind_index = (np.abs(indent['ind'].to_numpy() - ind)).argmin()
+        return indent.iloc[:ind_index].reset_index(drop=True)
+
+    def get_indent_between(self, start: float, last: float) -> pd.DataFrame:
+        indent = self.get_indent()
+        start_index = int(start * len(indent))
+        last_index = int(last * len(indent))
+        return indent.iloc[start_index:last_index].reset_index(drop=True)
+
+    def get_dwell(self) -> pd.DataFrame:
+        return self.get_data_between(self.dwell_range[0], self.dwell_range[1])
+
+    def get_relaxation(self) -> pd.DataFrame:
+        dwell = self.get_dwell()
+        max_ind = dwell['ind'].argmax()
+        return dwell.iloc[:max_ind].reset_index(drop=True)
+
+    def get_repulsion(self) -> pd.DataFrame:
+        dwell = self.get_dwell()
+        max_ind = dwell['ind'].argmax()
+        return dwell.iloc[max_ind:].reset_index(drop=True)
+
+    def get_retract(self) -> pd.DataFrame:
+        return self.get_data_between(self.dwell_range[1], -1)
+
+    def get_trigger_data(self) -> pd.Series:
+        indent = self.get_indent()
+        return indent.iloc[-1].reset_index(drop=True)
+
+    def get_approach_rates(self) -> None:
+        indent = self.get_indent()
+        t, ind, z = indent['t'], indent['ind'], indent['z']
+        self.vel_ind = lin_fit(t, ind)[0][0]
+        self.vel_z = lin_fit(t, z)[0][0]
+
+    def correct_virtual_defl(self) -> None:
+        self.check_contact()
+        if self.corrected:
+            self.restore_data()
+
+        preapproach = self.get_preapproach()
+        x = preapproach['z'].to_numpy()
+        y = preapproach['f'].to_numpy()
+        popt, _, _ = lin_fit(x, y)
+        f_line = np.poly1d(popt)(self.data['z'])
+        self.data['f'] = self.data['f'] - f_line
+
+    def detect_contact(self) -> int:
+        current_contact_index = self.contact_index
+        approach = self.get_approach()
+        max_index = len(approach) - 1
+        index = max_index
+        while True:
+            self.set_contact_index(index)
+            self.correct_virtual_defl()
+            approach_new = self.get_approach()
+            force = approach_new['f'].to_numpy()
+            mean = np.mean(force[:index+1])
+
+            ratio = force[index] / force[-1]
+            step_size = max(1, int((0.01 * max_index) ** ratio))
+            index = index - step_size
+            if force[index] < mean:
+                contact_index = index + 1
+                break
+
+        self.set_contact_index(current_contact_index)
+        self.restore_data()
+        return contact_index
+
+    def fit_indent(self) -> tuple:
+        self.check_contact()
+        indent = self.get_indent()
+        return poly_fit(indent['ind'], indent['f'])
+
+    def fit_indent_until(self, probe_diameter: float, ind: float) -> tuple:
+        self.check_contact()
+        indent_until = self.get_indent_until(ind)
+        return hertzian_fit(indent_until['ind'], indent_until['f'], probe_diameter)
+
+    def fit_indent_between(self, probe_diameter: float, interval: list[float] = [0.0, 1.0]) -> tuple:
+        self.check_contact()
+        indent_between = self.get_indent_between(interval[0], interval[1])
+        return hertzian_fit(indent_between['ind'], indent_between['f'], probe_diameter)
+
+    def fit_dwell(self) -> tuple:
+        dwell = self.get_dwell()
+        return biexponential_fit(dwell['t'], dwell['f'])
+
+    def fit_relaxation(self) -> tuple:
+        relaxation = self.get_relaxation()
+        return biexponential_fit(relaxation['t'], relaxation['ind'])
+
+    def get_figs_data(self, vd: bool = False, adjust: bool = False) -> None:
+        if vd or adjust:
+            self.restore_data()
+        if vd:
+            self.correct_virtual_defl()
+        if adjust:
+            self.adjust_to_contact()
+
+        approach = self.get_approach()
+
+        dwell = self.get_dwell()
+        relaxation = self.get_relaxation()
+
+        self.figs_data = {
+            'approach': (approach['ind'].to_numpy(), approach['f'].to_numpy()),
+            'dwell': (dwell['t'].to_numpy(), dwell['f'].to_numpy()),
+            'relaxation': (relaxation['t'].to_numpy(), relaxation['ind'].to_numpy()),
+        }
+
+    def get_contact_fig_plot(self) -> go.Figure:
+        fig = make_fig(
+            title=fr"$\text{{Selected Contact Point: {self.contact_index}}}$",
+            xaxis=r"$Indentation \text{ (m)}$"
+        )
+
+        x, y = self.figs_data['approach']
+        hover_texts = [f'Index: {i}' for i in range(len(x))]
+        trace = go.Scattergl(
+            x=x,
+            y=y,
+            name='Approach',
+            mode='markers',
+            text=hover_texts,
+            hoverinfo='text',
+            hoverlabel={'bgcolor': 'red'},
+            marker={'color': 'blue'},
+        )
+
+        fig.add_trace(trace)
+
+        x_line = x[self.contact_index]
+        y_line = y[self.contact_index]
+        fig.add_vline(x=x_line, line=dict(color='red', width=1.2))
+        fig.add_hline(y=y_line, line=dict(color='red', width=1.2))
+        self.contact_fig = fig
+        return fig
+
+    def get_dwell_relax_fig_plot(self) -> go.Figure:
+        fig = make_fig(
+            title=r"$\text{Dwell and Relaxation}$",
+            xaxis=r"$Time \text{ (s)}$"
+        )
+
+        fig.update_layout(
+            yaxis2=dict(
+                title=r"$Indentation \text{ (m)}$",
+                overlaying='y',
+                side='right'
+            )
+        )
+
+        x, y = self.figs_data['dwell']
+        trace = go.Scattergl(
+            x=x,
+            y=y,
+            name='Dwell',
+            mode='markers',
+            marker={'color': 'red'},
+        )
+
+        fig.add_trace(trace)
+
+        x, y = self.figs_data['relaxation']
+        trace = go.Scattergl(
+            x=x,
+            y=y,
+            yaxis='y2',
+            name='Relaxation',
+            mode='markers',
+            marker={'color': 'blue'},
+        )
+
+        fig.add_trace(trace)
+
+        self.dwell_relax_fig = fig
+        return fig
+
+    def get_fits_data(self, probe_diameter: float, ind: float | list[float]) -> None:
+        indent = self.get_indent()
+        indent_x_pred = indent['ind'].to_numpy()
+        self.indent_param, self.indent_R2, indent_y_pred = self.fit_indent()
+
+        self.max_ind = max(indent['ind'])
+        self.max_f = max(indent['f'])
+
+        if isinstance(ind, float):
+            self.hertzian_param, self.hertzian_R2, hertzian_y_pred = self.fit_indent_until(
+                probe_diameter, ind)
+            hertzian_x_pred = self.get_indent_until(ind)['ind'].to_numpy()
+        elif isinstance(ind, list) and len(ind) == 2:
+            self.hertzian_param, self.hertzian_R2, hertzian_y_pred = self.fit_indent_between(
+                probe_diameter, interval=ind)
+            hertzian_x_pred = self.get_indent_between(ind[0], ind[1])[
+                'ind'].to_numpy()
+
+        dwell = self.get_dwell()
+        dwell_x_pred = dwell['t'].to_numpy()
+        self.dwell_param, self.dwell_R2, dwell_y_pred = self.fit_dwell()
+
+        relaxation = self.get_relaxation()
+        relaxation_x_pred = relaxation['t'].to_numpy()
+        self.relaxation_param, self.relaxation_R2, relaxation_y_pred = self.fit_relaxation()
+
+        self.fits_data = {
+            'indent': (indent_x_pred, indent_y_pred),
+            'hertzian': (hertzian_x_pred, hertzian_y_pred),
+            'dwell': (dwell_x_pred, dwell_y_pred),
+            'relaxation': (relaxation_x_pred, relaxation_y_pred),
+        }
+
+    def add_contact_fit(self) -> go.Figure:
+        x, y = self.fits_data['indent']
+        trace = go.Scattergl(
+            x=x,
+            y=y,
+            name='PolyFit',
+            mode='lines',
+            line={'color': 'red'},
+        )
+        self.contact_fig.add_trace(trace)
+
+        x, y = self.fits_data['hertzian']
+        trace = go.Scattergl(
+            x=x,
+            y=y,
+            name='HertzianFit',
+            mode='lines',
+            line={
+                'color': 'green',
+                'width': 3,
+            },
+        )
+        self.contact_fig.add_trace(trace)
+
+        return self.contact_fig
+
+    def add_dwell_relax_fit(self) -> go.Figure:
+        x, y = self.fits_data['dwell']
+
+        trace = go.Scattergl(
+            x=x,
+            y=y,
+            name='DwellFit',
+            mode='lines',
+            line={
+                'color': 'green',
+                'width': 3,
+            },
+        )
+        self.dwell_relax_fig.add_trace(trace)
+
+        x, y = self.fits_data['relaxation']
+        trace = go.Scattergl(
+            x=x,
+            y=y,
+            yaxis='y2',
+            name='RelaxationFit',
+            mode='lines',
+            line={
+                'color': 'green',
+                'width': 3,
+            },
+        )
+        self.dwell_relax_fig.add_trace(trace)
+
+        return self.dwell_relax_fig
+
+    def get_contact_fig_pdf(self) -> go.Figure:
+        title = fr"$\text{{Selected Contact Point: {self.contact_index}}}$"
+        xaxis = r"$Indentation \text{ (m)}$"
+        fig = make_fig(title, xaxis)
+
+        x, y = self.figs_data['approach']
+        trace = go.Scatter(x=x, y=y, name='Approach', marker={'color': 'blue'})
+        fig.add_trace(trace)
+
+        x_line = x[self.contact_index]
+        y_line = y[self.contact_index]
+        fig.add_shape(type='line', x0=x_line, x1=x_line, y0=min(y),
+                      y1=max(y), line=dict(color='red', width=1.2))
+        fig.add_shape(type='line', y0=y_line, y1=y_line, x0=min(x),
+                      x1=max(x), line=dict(color='red', width=1.2))
+
+        if hasattr(self, 'fits_data'):
+            x, y = self.fits_data['indent']
+            trace = go.Scatter(x=x, y=y, name='PolyFit',
+                               mode='lines', line={'color': 'red'})
+            fig.add_trace(trace)
+
+            x, y = self.fits_data['hertzian']
+            trace = go.Scatter(x=x, y=y, name='HertzianFit',
+                               mode='lines', line={'color': 'green', 'width': 3})
+            fig.add_trace(trace)
+
+        return fig
+
+    def get_dwell_relax_fig_pdf(self) -> go.Figure:
+        title = r"$\text{Dwell and Relaxation}$"
+        xaxis = r"$Time \text{ (s)}$"
+        fig = make_fig(title, xaxis)
+
+        x, y = self.figs_data['dwell']
+        trace = go.Scatter(x=x, y=y, name='Dwell',
+                           marker_color='red')
+        fig.add_trace(trace)
+
+        fig.update_layout(
+            yaxis2=dict(
+                title=r"$Indentation \text{ (m)}$",
+                overlaying='y',
+                side='right',
+                showgrid=False,
+                ticks='outside',
+                tickwidth=2,
+                showline=True,
+                linewidth=2,
+                linecolor='black',
+                tickprefix=r"$",
+                ticksuffix=r"$",
+            )
+        )
+
+        x, y = self.figs_data['relaxation']
+        trace = go.Scatter(x=x, y=y, name='Relaxation',
+                           marker_color='blue', yaxis='y2')
+        fig.add_trace(trace)
+
+        if hasattr(self, 'fits_data'):
+            x, y = self.fits_data['dwell']
+            trace = go.Scatter(x=x, y=y, name='DwellFit',
+                               mode='lines', line={'color': 'green', 'width': 3})
+            fig.add_trace(trace)
+
+            x, y = self.fits_data['relaxation']
+            trace = go.Scatter(x=x, y=y, yaxis='y2', name='RelaxationFit',
+                               mode='lines', line={'color': 'green', 'width': 3})
+            fig.add_trace(trace)
+
+        return fig
+
+    def get_all_fits(self) -> dict:
+        fit_results_dict = {
+            'max_ind': self.max_ind,
+            'max_f': self.max_f,
+
+            'vel_ind': self.vel_ind,
+            'vel_z': self.vel_z,
+
+            'indent_a': self.indent_param[0],
+            'indent_b': self.indent_param[1],
+            'indent_c': self.indent_param[2],
+            'indent_R2': self.indent_R2,
+
+            'Hertzian_E': self.hertzian_param[0],
+            'Hertzian_R2': self.hertzian_R2,
+
+            'dwell_c': self.dwell_param[0],
+            'dwell_tau1': self.dwell_param[1],
+            'dwell_tau2': self.dwell_param[2],
+            'dwell_tauMax': max(self.dwell_param[1], self.dwell_param[2]),
+            'dwell_tauMin': min(self.dwell_param[1], self.dwell_param[2]),
+            'dwell_yf': self.dwell_param[3],
+            'dwell_R2': self.dwell_R2,
+
+            'relaxation_c': self.relaxation_param[0],
+            'relaxation_tau1': self.relaxation_param[1],
+            'relaxation_tau2': self.relaxation_param[2],
+            'relaxation_tauMax': max(self.relaxation_param[1], self.relaxation_param[2]),
+            'relaxation_tauMin': min(self.relaxation_param[1], self.relaxation_param[2]),
+            'relaxation_yf': self.relaxation_param[3],
+            'relaxation_R2': self.relaxation_R2
+        }
+
+        return fit_results_dict
+
+
+class CurveSet:
+    vd_dict: dict[tuple[str], bool] = {}
+    cp_dict: dict[tuple[str], int] = {}
+
+    def __init__(self, ident_labels: list[str], curve_dict: dict[tuple[str], Curve]) -> None:
+
+        self.ident_labels = ident_labels
+        self.curve_dict = curve_dict
+        self._index = 0
+
+    def __iter__(self):
+        self._index = 0
+        return self
+
+    def __next__(self) -> Curve:
+        if self._index < len(self.curve_dict):
+            key = list(self.curve_dict.keys())[self._index]
+            self._index += 1
+            return self.curve_dict[key]
+        else:
+            raise StopIteration
+
+    def __getitem__(self, key: tuple[str]) -> Curve:
+        return self.curve_dict[key]
+
+    def items(self) -> Iterable[tuple[tuple[str], Curve]]:
+        return self.curve_dict.items()
+
+    def pickle(self, filename: str) -> None:
+        with open(filename, 'wb') as f:
+            pickle.dump(self, f)
+
+    def keys(self) -> list[tuple[str]]:
+        return list(self.curve_dict.keys())
+
+    def reduce_data(self) -> None:
+        for curve in self:
+            curve.reduce_data()
+
+    def remove_curve(self, key: tuple[str]) -> None:
+        del self.curve_dict[key]
+
+    def remove_unannotated(self) -> None:
+        keys_to_remove = []
+        for key, curve in self.items():
+            if curve.contact_index == 0:
+                keys_to_remove.append(key)
+
+        for key in keys_to_remove:
+            self.remove_curve(key)
+
+    def correct_all_virtual_defl(self) -> None:
+        for curve in self:
+            curve.correct_virtual_defl()
+
+    def set_vd_by_annotations(self) -> None:
+        for key, value in self.vd_dict.items():
+            if value:
+                self[key].correct_virtual_defl()
+
+    def set_cp_by_annotations(self) -> None:
+        for key, value in self.cp_dict.items():
+            self[key].set_contact_index(value)
+
+    def update_annotations(self, annotations_dict: dict[tuple[str], Any]) -> None:
+        value = next(iter(annotations_dict.values()))
+        if isinstance(value, bool):
+            self.vd_dict = annotations_dict
+        elif isinstance(value, int):
+            self.cp_dict = annotations_dict
+
+    def update_annotations_from_file(self, file: str) -> None:
+        anno_tuple_dict = read_json_file(file)
+        self.update_annotations(anno_tuple_dict)
+
+    def adjust_to_contact(self) -> None:
+        for curve in self:
+            curve.adjust_to_contact()
+
+    def prepare_fit_all(self) -> None:
+        self.set_cp_by_annotations()
+        self.remove_unannotated()
+        self.set_vd_by_annotations()
+        self.adjust_to_contact()
+
+    def get_fit_all(self, probe_diameter: float, ind: float | list[float]) -> pd.DataFrame:
+        self.prepare_fit_all()
+        all_fit = []
+
+        for key, curve in tqdm(self.items()):
+            fit_results_dict = {label: key_value for label,
+                                key_value in zip(self.ident_labels, key)}
+            curve.get_fits_data(probe_diameter, ind)
+            curve.get_approach_rates()
+            fit_results_dict.update(curve.get_all_fits())
+            fit_results = pd.DataFrame([fit_results_dict])
+            all_fit.append(fit_results)
+
+        combined_results = pd.concat(all_fit, ignore_index=True)
+
+        return combined_results
+
+    def export_figures(self) -> pdf.PdfMerger:
+        merger = pdf.PdfMerger()
+        for key, curve in tqdm(self.items()):
+            curve.get_figs_data()
+            title = ""
+            for label, ident in zip(self.ident_labels, key):
+                title += label + ident
+
+            title = fr"$\text{{{title}}}$"
+            contact_fit_fig = curve.get_contact_fig_pdf()
+            contact_fit_fig.update_layout(title={'text': title})
+            contact_fit_fig_pdf = io.BytesIO(
+                contact_fit_fig.to_image(format='pdf'))
+            merger.append(contact_fit_fig_pdf)
+
+            dwell_relaxation_fit_fig = curve.get_dwell_relax_fig_pdf()
+            dwell_relaxation_fit_fig.update_layout(title={'text': title})
+            dwell_relaxation_fit_fig_pdf = io.BytesIO(
+                dwell_relaxation_fit_fig.to_image(format='pdf'))
+            merger.append(dwell_relaxation_fit_fig_pdf)
+
+        return merger
```

### Comparing `pyrtz2-1.1.11/pyrtz2/fit.py` & `pyrtz2-1.1.13/pyrtz2/fit.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.11/pyrtz2/src/components/annotator.py` & `pyrtz2-1.1.13/pyrtz2/src/components/annotator.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.11/pyrtz2/src/components/contact_controls.py` & `pyrtz2-1.1.13/pyrtz2/src/components/contact_controls.py`

 * *Files 13% similar despite different names*

```diff
@@ -51,40 +51,29 @@
             if vd_checklist:
                 vd_annotations[repr(key)] = True
             else:
                 vd_annotations[repr(key)] = False
             return no_update, json.dumps(vd_annotations)
 
     @app.callback(
-        [Output(ids.CONTACT_FIG, 'figure', allow_duplicate=True),
-         Output(ids.FORCETIME_FIG, 'figure', allow_duplicate=True),],
-        [Input(ids.ADJUST_CHECKLIST, 'value'),
-         Input(ids.CP_ANNOTATIONS, 'data')],
-        [State(ids.CURVE_DROPDOWN, 'value'),
+        Output(ids.CONTACT_FIG, 'figure', allow_duplicate=True),
+        [Input(ids.CP_ANNOTATIONS, 'data')],
+        [State(ids.ADJUST_CHECKLIST, 'value'),
+         State(ids.CURVE_DROPDOWN, 'value'),
          State(ids.CONTACT_FIG, 'figure'),
-         State(ids.FORCETIME_FIG, 'figure'),
          State(ids.VD_CHECKLIST, 'value')],
         prevent_initial_call=True
     )
-    def set_contact(adjust, cp_data, curve_value, contact_fig_dict, forcetime_fig_dict, vd):
-        if not curve_value or vd:
+    def set_contact(cp_data, adjust, curve_value, contact_fig_dict, vd):
+        if not curve_value or vd or adjust:
             raise PreventUpdate
 
         cp = get_current_annotation(curve_value, cp_data)
-
-        contact_fig = fig.get_fig(contact_fig_dict)
-        if adjust:
-            forcetime_fig = fig.get_fig(forcetime_fig_dict)
-            contact_fig = fig.adjust_to_contact(cp, contact_fig)
-            forcetime_fig = fig.adjust_to_contact(cp, forcetime_fig)
-            contact_fig = fig.update_contact_line(cp, contact_fig)
-            return contact_fig, forcetime_fig
-        else:
-            contact_fig = fig.update_contact_line(cp, contact_fig)
-            return contact_fig, no_update
+        contact_fig = fig.update_contact_line(cp, contact_fig_dict)
+        return contact_fig
 
     @app.callback(
         [Output(ids.CP_ANNOTATIONS, 'data', allow_duplicate=True),
          Output(ids.DETECT_CONTACT, 'children')],
         [Input(ids.RESET_CONTACT, 'n_clicks'),
          Input(ids.DETECT_CONTACT, 'n_clicks')],
         [State(ids.CURVE_DROPDOWN, 'value'),
```

### Comparing `pyrtz2-1.1.11/pyrtz2/src/components/curve_dropdown.py` & `pyrtz2-1.1.13/pyrtz2/src/components/curve_dropdown.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.11/pyrtz2/src/components/fig.py` & `pyrtz2-1.1.13/pyrtz2/src/components/fig.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,22 +6,14 @@
 
 def render(id: str, title: str, xaxis: str) -> dcc.Graph:
     fig = make_fig(title, xaxis)
 
     if 'contact' in id:
         fig.add_vline(x=0, line=dict(color='red', width=1.2))
         fig.add_hline(y=0, line=dict(color='red', width=1.2))
-    else:
-        fig.update_layout(
-            yaxis2=dict(
-                title=r"$Indentation \text{ (m)}$",
-                overlaying='y',
-                side='right'
-            )
-        )
 
     return dcc.Graph(
         figure=fig,
         id=id,
         mathjax=True,
         style={
             'width': '50%',
@@ -38,15 +30,22 @@
             'x': 0.5,
             'xanchor': 'center'
         },
         plot_bgcolor='white',
         paper_bgcolor='white',
         margin=dict(t=50, b=50, l=50, r=50),
         showlegend=False,
-        transition={'duration': 500}
+        transition={'duration': 500},
+        yaxis2=dict(
+            title=r"$Indentation \text{ (m)}$",
+            overlaying='y',
+            side='right',
+            tickprefix=r"$",
+            ticksuffix=r"$",
+        )
     )
 
     fig.update_annotations(yshift=10)
 
     fig.update_xaxes(
         showgrid=False,
         ticks='outside',
@@ -104,38 +103,20 @@
         fig.data[0].x = x
         fig.data[0].y = y
         fig.data[0]['text'] = hover_texts
 
     return fig
 
 
-def get_fig(fig: dict) -> go.Figure:
-    return go.Figure(fig)
-
-
-def update_contact_line(cp: int, fig: go.Figure) -> go.Figure:
+def update_contact_line(cp: int, fig: dict | go.Figure) -> go.Figure:
+    if isinstance(fig, dict):
+        fig = go.Figure(fig)
     data_x = fig.data[0].x
     data_y = fig.data[0].y
-    fig.layout.shapes[0]['x0'] = data_x[cp]
-    fig.layout.shapes[0]['x1'] = data_x[cp]
-    fig.layout.shapes[1]['y0'] = data_y[cp]
-    fig.layout.shapes[1]['y1'] = data_y[cp]
+    fig.layout['shapes'][0]['x0'] = data_x[cp]
+    fig.layout['shapes'][0]['x1'] = data_x[cp]
+    fig.layout['shapes'][1]['y0'] = data_y[cp]
+    fig.layout['shapes'][1]['y1'] = data_y[cp]
     fig.layout['title']['text'] = fr"$\text{{Selected Contact Point: {cp}}}$"
 
     return fig
 
-
-def adjust_to_contact(cp: int, fig: go.Figure) -> go.Figure:
-    data_x = fig.data[0].x
-    data_y = fig.data[0].y
-    x_data = np.array(data_x)
-    y_data = np.array(data_y)
-    fig.update(
-        data=[
-            {
-                'x': x_data - x_data[cp],
-                'y': y_data - y_data[cp]
-            }
-        ]
-    )
-
-    return fig
```

### Comparing `pyrtz2-1.1.11/pyrtz2/src/components/fitter.py` & `pyrtz2-1.1.13/pyrtz2/src/components/fitter.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.11/pyrtz2/src/components/ids.py` & `pyrtz2-1.1.13/pyrtz2/src/components/ids.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 EXPERIMENT_PATH = "experiment-path"
 EXPERIMENT_LABELS = "experiment-labels"
 PROBE_DIAMETER = "probe-diameter"
 LOAD_EXPERIMENT = "load-experiment"
 LOAD_OUTPUT = "load-output"
 EXPERIMENT = "experiment"
-EXPERIMENT_PROCESSED = "experiment-processed"
 IMAGES = "images"
 
 CURVE_DROPDOWN = "curve-dropdown"
 CURVE_DATA = "curve-data"
 LOAD_ANIMATION = "load-animation"
 BUTTON_BACK = "button-back"
 BUTTON_FORWARD = "button-forward"
```

### Comparing `pyrtz2-1.1.11/pyrtz2/src/components/image_frame.py` & `pyrtz2-1.1.13/pyrtz2/src/components/image_frame.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from dash import Dash, html
 from dash.dependencies import Input, Output
 
 from . import ids
-from ..utils.utils import load
+from ..utils.utils import load, load_image
 
 
 def render(app: Dash) -> html.Div:
 
     @app.callback(
         Output(ids.IMAGE_FRAME, 'src'),
         [Input(ids.CURVE_DROPDOWN, 'value'),
          Input(ids.IMAGES, 'data')],
         prevent_initial_call=True
     )
     def update_image_frame(curve_value, encoded_images):
-        if not encoded_images:
+        if not encoded_images or not curve_value:
             return ''
 
         images: dict = load(encoded_images)
 
         key = eval(curve_value)['key']
         new_key = key[:-1] if len(key) > 1 else key
 
         # THIS ONLY SHOWS THE FIRST IMAGE IF THERE IS ONE
         if images.get(new_key):
-            image = images[new_key][0]
-            image_src = f'data:image/png;base64,{image}'
+            image_path = images[new_key][0]
+            image_src = load_image(image_path)
             return image_src
         else:
             return ''
 
     return html.Div(
         className='image',
         children=[
```

### Comparing `pyrtz2-1.1.11/pyrtz2/src/components/layout.py` & `pyrtz2-1.1.13/pyrtz2/src/components/layout.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.11/pyrtz2/src/components/loader.py` & `pyrtz2-1.1.13/pyrtz2/src/components/loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,15 +83,14 @@
                 ],
                 style={
                     'display': 'flex',
                     'width': '100%',
                 }
             ),
             experiment_loader.render(app),
-            dcc.Store(id=ids.EXPERIMENT_PROCESSED),
             image_loader.render(app),
             html.Div(
                 children="Enter experiment info and then click load.",
                 id=ids.LOAD_OUTPUT
             )
         ],
         className='experiment-loader',
```

### Comparing `pyrtz2-1.1.11/pyrtz2/src/components/toolbox.py` & `pyrtz2-1.1.13/pyrtz2/src/components/toolbox.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.11/pyrtz2/src/data/downloader.py` & `pyrtz2-1.1.13/pyrtz2/src/data/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         data_dict = json.loads(vd_data)
 
         json_string = json.dumps(data_dict, indent=4)
         return {'content': json_string, 'filename': f'{exp_name}_vd_annotations.json', 'type': 'text/json'}
 
     @app.callback(
         [Output(ids.DOWNLOAD, 'data', allow_duplicate=True),
-         Output(ids.EXPERIMENT_PROCESSED, 'data', allow_duplicate=True),
+         Output(ids.EXPERIMENT, 'data', allow_duplicate=True),
          Output(ids.DOWNLOAD_FITS, 'children', allow_duplicate=True),
          Output(ids.INDENTATION, 'value')],
         [Input(ids.DOWNLOAD_FITS, "n_clicks")],
         [State(ids.EXPERIMENT, 'data'),
          State(ids.CP_ANNOTATIONS, 'data'),
          State(ids.VD_ANNOTATIONS, 'data'),
          State(ids.INDENTATION, 'value'),
@@ -52,27 +52,27 @@
     def download_fits_csv(_, encoded_experiment, cp_data, vd_data, indentation, exp_output):
         if indentation:
             experiment = load(encoded_experiment)
             indentation = process_indentation(indentation)
             experiment_processed, df = process_experiment(
                 experiment, cp_data, vd_data, indentation)
             exp_name = exp_output.split('\'')[1]
-            return dcc.send_data_frame(df.to_csv, filename=f"{exp_name}_its.csv"), dump(experiment_processed), no_update, no_update
+            return dcc.send_data_frame(df.to_csv, filename=f"{exp_name}_fits.csv"), dump(experiment_processed), no_update, no_update
 
         return no_update, no_update, no_update, "Unable to proceed without indentation!"
 
     @app.callback(
         [Output(ids.DOWNLOAD, 'data', allow_duplicate=True),
          Output(ids.DOWNLOAD_CURVES, 'children')],
         [Input(ids.DOWNLOAD_CURVES, "n_clicks")],
-        [State(ids.EXPERIMENT_PROCESSED, 'data'),
+        [State(ids.EXPERIMENT, 'data'),
          State(ids.LOAD_OUTPUT, 'children')],
         prevent_initial_call=True
     )
-    def download_curves_pdf(_, encoded_experiment_processed, exp_output):
-        experiment_processed = load(encoded_experiment_processed)
+    def download_curves_pdf(_, encoded_experiment, exp_output):
+        experiment_processed = load(encoded_experiment)
         exp_name = exp_output.split('\'')[1]
         pdf_src = get_pdf(experiment_processed)
 
         return dcc.send_bytes(src=pdf_src.getvalue(), filename=f"{exp_name}_curves.pdf", base64=True), no_update
 
     return dcc.Download(id=ids.DOWNLOAD)
```

### Comparing `pyrtz2-1.1.11/pyrtz2/src/data/experiment_loader.py` & `pyrtz2-1.1.13/pyrtz2/src/data/experiment_loader.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,17 +29,9 @@
         path = os.path.dirname(os.path.normpath(experiment_path))
         label_list = [label.strip() for label in labels.split(';')]
         experiment = AFM(path, exp_name, label_list, float(probe_diameter))
         experiment.experiment.reduce_data()
         cp_data = make_json(experiment.curve_keys, 0)
         vd_data = make_json(experiment.curve_keys, False)
         return dump(experiment), cp_data, vd_data
-    
-    @app.callback(
-        Output(ids.EXPERIMENT_PROCESSED, 'data', allow_duplicate=True),
-        Input(ids.EXPERIMENT, 'data'),
-        prevent_initial_call=True
-    )
-    def copy_to_processed(encoded_experiment):
-        return encoded_experiment
 
     return dcc.Store(id=ids.EXPERIMENT)
```

### Comparing `pyrtz2-1.1.11/pyrtz2/src/data/processor.py` & `pyrtz2-1.1.13/pyrtz2/src/data/processor.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.11/pyrtz2/src/utils/utils.py` & `pyrtz2-1.1.13/pyrtz2/src/utils/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,13 +78,13 @@
         new_key = key[:-1]
         if new_key not in new_dict:
             new_dict[new_key] = [value]
         else:
             new_dict[new_key].append(value)
     return new_dict
 
-
-def tif_to_base64(tif_path):
-    img = Image.open(tif_path)
+def load_image(image_path:str) -> str:
+    img = Image.open(image_path)
     buffer = io.BytesIO()
-    img.save(buffer, format="PNG")  # can be changeg to "JPEG"
-    return base64.b64encode(buffer.getvalue()).decode()
+    img.save(buffer, format="JPEG")  # can be changed to "PNG"
+    encoded_image = base64.b64encode(buffer.getvalue()).decode()
+    return f"data:image/jpeg;base64,{encoded_image}"
```

### Comparing `pyrtz2-1.1.11/PKG-INFO` & `pyrtz2-1.1.13/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtz2
-Version: 1.1.11
+Version: 1.1.13
 Summary: Force spectroscopy in Python
 Author-email: "Hoseyn A. Amiri" <aamirihoseyn@gmail.com>
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: dash
 Requires-Dist: dash-bootstrap-components
```

