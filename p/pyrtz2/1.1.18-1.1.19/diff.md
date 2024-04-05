# Comparing `tmp/pyrtz2-1.1.18.tar.gz` & `tmp/pyrtz2-1.1.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrtz2-1.1.18.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyrtz2-1.1.19.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyrtz2-1.1.18.tar` & `pyrtz2-1.1.19.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0       66 2024-04-02 19:47:59.285340 pyrtz2-1.1.18/.gitattributes
--rw-r--r--   0        0        0       37 2024-04-05 12:35:50.341792 pyrtz2-1.1.18/.gitignore
--rw-r--r--   0        0        0    33041 2024-04-02 20:07:11.768711 pyrtz2-1.1.18/LICENSE
--rw-r--r--   0        0        0      455 2024-04-05 17:28:24.205830 pyrtz2-1.1.18/README.md
--rw-r--r--   0        0        0   442996 2024-03-22 20:48:12.000000 pyrtz2-1.1.18/example/con050/jasYcon050cell37m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:48:22.000000 pyrtz2-1.1.18/example/con050/jasYcon050cell37m0001.tif
--rw-r--r--   0        0        0   453575 2024-03-22 20:48:52.000000 pyrtz2-1.1.18/example/con050/jasYcon050cell38m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:49:00.000000 pyrtz2-1.1.18/example/con050/jasYcon050cell38m0001.tif
--rw-r--r--   0        0        0   458723 2024-03-22 20:49:32.000000 pyrtz2-1.1.18/example/con050/jasYcon050cell39m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:49:38.000000 pyrtz2-1.1.18/example/con050/jasYcon050cell39m0001.tif
--rw-r--r--   0        0        0   435180 2024-03-22 20:50:14.000000 pyrtz2-1.1.18/example/con050/jasYcon050cell40m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:50:22.000000 pyrtz2-1.1.18/example/con050/jasYcon050cell40m0001.tif
--rw-r--r--   0        0        0   457660 2024-03-22 20:54:28.000000 pyrtz2-1.1.18/example/con050/jasYcon050cell42m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:54:36.000000 pyrtz2-1.1.18/example/con050/jasYcon050cell42m0001.tif
--rw-r--r--   0        0        0      196 2024-03-27 20:17:56.223149 pyrtz2-1.1.18/example/con050_cp_annotations.json
--rw-r--r--   0        0        0   331740 2024-04-04 23:26:50.939244 pyrtz2-1.1.18/example/con050_curves.pdf
--rw-r--r--   0        0        0     1749 2024-04-04 23:26:34.450692 pyrtz2-1.1.18/example/con050_fits.csv
--rw-r--r--   0        0        0      205 2024-03-26 23:15:37.330282 pyrtz2-1.1.18/example/con050_vd_annotations.json
--rw-r--r--   0        0        0       37 2024-04-05 12:53:39.905466 pyrtz2-1.1.18/example/test.py
--rw-r--r--   0        0        0      794 2024-04-04 21:36:24.676720 pyrtz2-1.1.18/pyproject.toml
--rw-r--r--   0        0        0       62 2024-04-05 18:43:42.871751 pyrtz2-1.1.18/pyrtz2/__init__.py
--rw-r--r--   0        0        0     1874 2024-04-04 20:43:57.261121 pyrtz2-1.1.18/pyrtz2/afm.py
--rw-r--r--   0        0        0      335 2024-04-05 13:06:49.354563 pyrtz2-1.1.18/pyrtz2/app.py
--rw-r--r--   0        0        0     1320 2024-03-29 18:30:21.132859 pyrtz2-1.1.18/pyrtz2/assets/style.css
--rw-r--r--   0        0        0     4718 2024-04-04 20:43:28.570132 pyrtz2-1.1.18/pyrtz2/asylum.py
--rw-r--r--   0        0        0    18040 2024-04-05 18:43:29.214731 pyrtz2-1.1.18/pyrtz2/curves.py
--rw-r--r--   0        0        0     4451 2024-04-02 14:59:14.529838 pyrtz2-1.1.18/pyrtz2/fit.py
--rw-r--r--   0        0        0        0 2024-04-03 01:57:24.101285 pyrtz2-1.1.18/pyrtz2/src/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.18/pyrtz2/src/components/__init__.py
--rw-r--r--   0        0        0     1982 2024-04-04 23:28:38.697339 pyrtz2-1.1.18/pyrtz2/src/components/annotator.py
--rw-r--r--   0        0        0     5060 2024-04-05 12:35:50.358816 pyrtz2-1.1.18/pyrtz2/src/components/contact_controls.py
--rw-r--r--   0        0        0     4139 2024-04-03 02:17:21.251676 pyrtz2-1.1.18/pyrtz2/src/components/curve_dropdown.py
--rw-r--r--   0        0        0     2886 2024-04-05 18:47:58.605617 pyrtz2-1.1.18/pyrtz2/src/components/fig.py
--rw-r--r--   0        0        0     2904 2024-04-05 18:42:39.056993 pyrtz2-1.1.18/pyrtz2/src/components/fig_frame.py
--rw-r--r--   0        0        0     2393 2024-04-04 18:36:08.361121 pyrtz2-1.1.18/pyrtz2/src/components/fitter.py
--rw-r--r--   0        0        0     1194 2024-04-05 12:35:50.370793 pyrtz2-1.1.18/pyrtz2/src/components/ids.py
--rw-r--r--   0        0        0     1221 2024-04-05 12:35:50.375793 pyrtz2-1.1.18/pyrtz2/src/components/image_frame.py
--rw-r--r--   0        0        0     1666 2024-04-02 01:29:34.764572 pyrtz2-1.1.18/pyrtz2/src/components/layout.py
--rw-r--r--   0        0        0     3408 2024-04-05 12:35:50.379817 pyrtz2-1.1.18/pyrtz2/src/components/loader.py
--rw-r--r--   0        0        0     1052 2024-04-04 18:50:12.478289 pyrtz2-1.1.18/pyrtz2/src/components/toolbox.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.18/pyrtz2/src/data/__init__.py
--rw-r--r--   0        0        0     3307 2024-04-05 12:39:49.693713 pyrtz2-1.1.18/pyrtz2/src/data/downloader.py
--rw-r--r--   0        0        0     1560 2024-04-05 12:35:50.388794 pyrtz2-1.1.18/pyrtz2/src/data/experiment_loader.py
--rw-r--r--   0        0        0     1117 2024-04-05 12:35:50.392818 pyrtz2-1.1.18/pyrtz2/src/data/image_loader.py
--rw-r--r--   0        0        0     1218 2024-04-04 21:40:13.246607 pyrtz2-1.1.18/pyrtz2/src/data/processor.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.18/pyrtz2/src/utils/__init__.py
--rw-r--r--   0        0        0     2474 2024-04-05 12:35:50.397796 pyrtz2-1.1.18/pyrtz2/src/utils/utils.py
--rw-r--r--   0        0        0     1191 1970-01-01 00:00:00.000000 pyrtz2-1.1.18/PKG-INFO
+-rw-r--r--   0        0        0       66 2024-04-02 19:47:59.285340 pyrtz2-1.1.19/.gitattributes
+-rw-r--r--   0        0        0       37 2024-04-05 12:35:50.341792 pyrtz2-1.1.19/.gitignore
+-rw-r--r--   0        0        0    33041 2024-04-02 20:07:11.768711 pyrtz2-1.1.19/LICENSE
+-rw-r--r--   0        0        0      455 2024-04-05 17:28:24.205830 pyrtz2-1.1.19/README.md
+-rw-r--r--   0        0        0   442996 2024-03-22 20:48:12.000000 pyrtz2-1.1.19/example/con050/jasYcon050cell37m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:48:22.000000 pyrtz2-1.1.19/example/con050/jasYcon050cell37m0001.tif
+-rw-r--r--   0        0        0   453575 2024-03-22 20:48:52.000000 pyrtz2-1.1.19/example/con050/jasYcon050cell38m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:49:00.000000 pyrtz2-1.1.19/example/con050/jasYcon050cell38m0001.tif
+-rw-r--r--   0        0        0   458723 2024-03-22 20:49:32.000000 pyrtz2-1.1.19/example/con050/jasYcon050cell39m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:49:38.000000 pyrtz2-1.1.19/example/con050/jasYcon050cell39m0001.tif
+-rw-r--r--   0        0        0   435180 2024-03-22 20:50:14.000000 pyrtz2-1.1.19/example/con050/jasYcon050cell40m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:50:22.000000 pyrtz2-1.1.19/example/con050/jasYcon050cell40m0001.tif
+-rw-r--r--   0        0        0   457660 2024-03-22 20:54:28.000000 pyrtz2-1.1.19/example/con050/jasYcon050cell42m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:54:36.000000 pyrtz2-1.1.19/example/con050/jasYcon050cell42m0001.tif
+-rw-r--r--   0        0        0      196 2024-03-27 20:17:56.223149 pyrtz2-1.1.19/example/con050_cp_annotations.json
+-rw-r--r--   0        0        0   331740 2024-04-04 23:26:50.939244 pyrtz2-1.1.19/example/con050_curves.pdf
+-rw-r--r--   0        0        0     1749 2024-04-04 23:26:34.450692 pyrtz2-1.1.19/example/con050_fits.csv
+-rw-r--r--   0        0        0      205 2024-03-26 23:15:37.330282 pyrtz2-1.1.19/example/con050_vd_annotations.json
+-rw-r--r--   0        0        0       37 2024-04-05 12:53:39.905466 pyrtz2-1.1.19/example/test.py
+-rw-r--r--   0        0        0      794 2024-04-04 21:36:24.676720 pyrtz2-1.1.19/pyproject.toml
+-rw-r--r--   0        0        0       62 2024-04-05 19:40:29.943030 pyrtz2-1.1.19/pyrtz2/__init__.py
+-rw-r--r--   0        0        0     1874 2024-04-04 20:43:57.261121 pyrtz2-1.1.19/pyrtz2/afm.py
+-rw-r--r--   0        0        0      335 2024-04-05 13:06:49.354563 pyrtz2-1.1.19/pyrtz2/app.py
+-rw-r--r--   0        0        0     1320 2024-03-29 18:30:21.132859 pyrtz2-1.1.19/pyrtz2/assets/style.css
+-rw-r--r--   0        0        0     4718 2024-04-04 20:43:28.570132 pyrtz2-1.1.19/pyrtz2/asylum.py
+-rw-r--r--   0        0        0    17714 2024-04-05 19:38:14.869532 pyrtz2-1.1.19/pyrtz2/curves.py
+-rw-r--r--   0        0        0     4451 2024-04-02 14:59:14.529838 pyrtz2-1.1.19/pyrtz2/fit.py
+-rw-r--r--   0        0        0        0 2024-04-03 01:57:24.101285 pyrtz2-1.1.19/pyrtz2/src/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.19/pyrtz2/src/components/__init__.py
+-rw-r--r--   0        0        0     1982 2024-04-04 23:28:38.697339 pyrtz2-1.1.19/pyrtz2/src/components/annotator.py
+-rw-r--r--   0        0        0     5060 2024-04-05 12:35:50.358816 pyrtz2-1.1.19/pyrtz2/src/components/contact_controls.py
+-rw-r--r--   0        0        0     4139 2024-04-03 02:17:21.251676 pyrtz2-1.1.19/pyrtz2/src/components/curve_dropdown.py
+-rw-r--r--   0        0        0     2866 2024-04-05 19:13:38.359613 pyrtz2-1.1.19/pyrtz2/src/components/fig.py
+-rw-r--r--   0        0        0     2933 2024-04-05 19:03:28.975317 pyrtz2-1.1.19/pyrtz2/src/components/fig_frame.py
+-rw-r--r--   0        0        0     2393 2024-04-04 18:36:08.361121 pyrtz2-1.1.19/pyrtz2/src/components/fitter.py
+-rw-r--r--   0        0        0     1194 2024-04-05 12:35:50.370793 pyrtz2-1.1.19/pyrtz2/src/components/ids.py
+-rw-r--r--   0        0        0     1221 2024-04-05 19:13:08.301764 pyrtz2-1.1.19/pyrtz2/src/components/image_frame.py
+-rw-r--r--   0        0        0     1666 2024-04-05 19:10:45.242952 pyrtz2-1.1.19/pyrtz2/src/components/layout.py
+-rw-r--r--   0        0        0     3408 2024-04-05 12:35:50.379817 pyrtz2-1.1.19/pyrtz2/src/components/loader.py
+-rw-r--r--   0        0        0     1052 2024-04-04 18:50:12.478289 pyrtz2-1.1.19/pyrtz2/src/components/toolbox.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.19/pyrtz2/src/data/__init__.py
+-rw-r--r--   0        0        0     3307 2024-04-05 19:35:59.106653 pyrtz2-1.1.19/pyrtz2/src/data/downloader.py
+-rw-r--r--   0        0        0     1560 2024-04-05 12:35:50.388794 pyrtz2-1.1.19/pyrtz2/src/data/experiment_loader.py
+-rw-r--r--   0        0        0     1117 2024-04-05 12:35:50.392818 pyrtz2-1.1.19/pyrtz2/src/data/image_loader.py
+-rw-r--r--   0        0        0     1218 2024-04-04 21:40:13.246607 pyrtz2-1.1.19/pyrtz2/src/data/processor.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.19/pyrtz2/src/utils/__init__.py
+-rw-r--r--   0        0        0     2474 2024-04-05 12:35:50.397796 pyrtz2-1.1.19/pyrtz2/src/utils/utils.py
+-rw-r--r--   0        0        0     1191 1970-01-01 00:00:00.000000 pyrtz2-1.1.19/PKG-INFO
```

### Comparing `pyrtz2-1.1.18/LICENSE` & `pyrtz2-1.1.19/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/example/con050/jasYcon050cell37m0000.ibw` & `pyrtz2-1.1.19/example/con050/jasYcon050cell37m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/example/con050/jasYcon050cell37m0001.tif` & `pyrtz2-1.1.19/example/con050/jasYcon050cell37m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/example/con050/jasYcon050cell38m0000.ibw` & `pyrtz2-1.1.19/example/con050/jasYcon050cell38m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/example/con050/jasYcon050cell38m0001.tif` & `pyrtz2-1.1.19/example/con050/jasYcon050cell38m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/example/con050/jasYcon050cell39m0000.ibw` & `pyrtz2-1.1.19/example/con050/jasYcon050cell39m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/example/con050/jasYcon050cell39m0001.tif` & `pyrtz2-1.1.19/example/con050/jasYcon050cell39m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/example/con050/jasYcon050cell40m0000.ibw` & `pyrtz2-1.1.19/example/con050/jasYcon050cell40m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/example/con050/jasYcon050cell40m0001.tif` & `pyrtz2-1.1.19/example/con050/jasYcon050cell40m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/example/con050/jasYcon050cell42m0000.ibw` & `pyrtz2-1.1.19/example/con050/jasYcon050cell42m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/example/con050/jasYcon050cell42m0001.tif` & `pyrtz2-1.1.19/example/con050/jasYcon050cell42m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/example/con050_curves.pdf` & `pyrtz2-1.1.19/example/con050_curves.pdf`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/example/con050_fits.csv` & `pyrtz2-1.1.19/example/con050_fits.csv`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/pyproject.toml` & `pyrtz2-1.1.19/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/pyrtz2/afm.py` & `pyrtz2-1.1.19/pyrtz2/afm.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/pyrtz2/assets/style.css` & `pyrtz2-1.1.19/pyrtz2/assets/style.css`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/pyrtz2/asylum.py` & `pyrtz2-1.1.19/pyrtz2/asylum.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/pyrtz2/curves.py` & `pyrtz2-1.1.19/pyrtz2/curves.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import pandas as pd
 import numpy as np
 import json
 import ast
 import io
 from tqdm import tqdm
 from typing import Any, Iterable
+from time import sleep
 
 from .fit import lin_fit, poly_fit, hertzian_fit, biexponential_fit
 from .src.components.fig import make_fig
 
 
 def read_json_file(file: str) -> dict[tuple, bool | int]:
     with open(file, 'rt') as cf:
@@ -348,48 +349,36 @@
             fig.add_trace(trace)
 
             x, y = self.fits_data['hertzian']
             trace = go.Scatter(x=x, y=y, name='HertzianFit',
                                mode='lines', line={'color': 'green', 'width': 3})
             fig.add_trace(trace)
 
+        fig.update_layout(width=480)
+        sleep(1)
         return fig
 
     def get_dwell_fig_pdf(self) -> go.Figure:
         title = r"$\text{Dwell}$"
         xaxis = r"$Time \text{ (s)}$"
         fig = make_fig(title, xaxis)
 
         x, y = self.figs_data['dwell']
         trace = go.Scatter(x=x, y=y, name='Dwell',
                            marker_color='red')
         fig.add_trace(trace)
 
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
         if hasattr(self, 'fits_data'):
             x, y = self.fits_data['dwell']
             trace = go.Scatter(x=x, y=y, name='DwellFit',
                                mode='lines', line={'color': 'green', 'width': 3})
             fig.add_trace(trace)
 
+        fig.update_layout(width=480)
+        sleep(1)
         return fig
 
     def get_all_fits(self) -> dict:
         fit_results_dict = {
             'max_ind': self.max_ind,
             'max_f': self.max_f,
```

### Comparing `pyrtz2-1.1.18/pyrtz2/fit.py` & `pyrtz2-1.1.19/pyrtz2/fit.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/pyrtz2/src/components/annotator.py` & `pyrtz2-1.1.19/pyrtz2/src/components/annotator.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/pyrtz2/src/components/contact_controls.py` & `pyrtz2-1.1.19/pyrtz2/src/components/contact_controls.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/pyrtz2/src/components/curve_dropdown.py` & `pyrtz2-1.1.19/pyrtz2/src/components/curve_dropdown.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/pyrtz2/src/components/fig.py` & `pyrtz2-1.1.19/pyrtz2/src/components/fig.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,15 @@
             'xanchor': 'center'
         },
         plot_bgcolor='white',
         paper_bgcolor='white',
         margin=dict(t=50, b=50, l=50, r=50),
         showlegend=False,
         transition={'duration': 500},
-        width=800,
-        height=600
+        height=400
     )
 
     fig.update_annotations(yshift=10)
 
     fig.update_xaxes(
         showgrid=False,
         ticks='outside',
```

### Comparing `pyrtz2-1.1.18/pyrtz2/src/components/fig_frame.py` & `pyrtz2-1.1.19/pyrtz2/src/components/fig_frame.py`

 * *Files 9% similar despite different names*

```diff
@@ -60,15 +60,16 @@
         return json.dumps(cp_annotations)
 
     return html.Div(
         className='figure',
         id=ids.FIG_HOLDER,
         style={
             'display': 'flex',
-            'width': '100%',
+            'width': '98%',
+            'height': '90%',
         },
         children=[
             fig.render(id=ids.CONTACT_FIG,
                        title=r"$\text{Selected Contact Point: }$",
                        xaxis=r"$Indentation \text{ (m)}$"),
             fig.render(id=ids.FORCETIME_FIG,
                        title=r"$\text{Dwell and Relaxation}$",
```

### Comparing `pyrtz2-1.1.18/pyrtz2/src/components/fitter.py` & `pyrtz2-1.1.19/pyrtz2/src/components/fitter.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/pyrtz2/src/components/ids.py` & `pyrtz2-1.1.19/pyrtz2/src/components/ids.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/pyrtz2/src/components/image_frame.py` & `pyrtz2-1.1.19/pyrtz2/src/components/image_frame.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/pyrtz2/src/components/layout.py` & `pyrtz2-1.1.19/pyrtz2/src/components/layout.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/pyrtz2/src/components/loader.py` & `pyrtz2-1.1.19/pyrtz2/src/components/loader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/pyrtz2/src/components/toolbox.py` & `pyrtz2-1.1.19/pyrtz2/src/components/toolbox.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/pyrtz2/src/data/downloader.py` & `pyrtz2-1.1.19/pyrtz2/src/data/downloader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/pyrtz2/src/data/experiment_loader.py` & `pyrtz2-1.1.19/pyrtz2/src/data/experiment_loader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/pyrtz2/src/data/image_loader.py` & `pyrtz2-1.1.19/pyrtz2/src/data/image_loader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/pyrtz2/src/data/processor.py` & `pyrtz2-1.1.19/pyrtz2/src/data/processor.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/pyrtz2/src/utils/utils.py` & `pyrtz2-1.1.19/pyrtz2/src/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.18/PKG-INFO` & `pyrtz2-1.1.19/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtz2
-Version: 1.1.18
+Version: 1.1.19
 Summary: Force spectroscopy in Python
 Author-email: "Hoseyn A. Amiri" <aamirihoseyn@gmail.com>
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: dash
 Requires-Dist: dash-bootstrap-components
```

