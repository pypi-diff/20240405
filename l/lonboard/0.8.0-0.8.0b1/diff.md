# Comparing `tmp/lonboard-0.8.0.tar.gz` & `tmp/lonboard-0.8.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lonboard-0.8.0.tar", max compression
+gzip compressed data, was "lonboard-0.8.0b1.tar", max compression
```

## Comparing `lonboard-0.8.0.tar` & `lonboard-0.8.0b1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1073 2024-04-05 15:26:43.372268 lonboard-0.8.0/LICENSE
--rw-r--r--   0        0        0       36 2024-04-05 15:26:43.372268 lonboard-0.8.0/MANIFEST.in
--rw-r--r--   0        0        0     3074 2024-04-05 15:26:43.372268 lonboard-0.8.0/README.md
--rw-r--r--   0        0        0      445 2024-04-05 15:26:43.560267 lonboard-0.8.0/lonboard/__init__.py
--rw-r--r--   0        0        0       39 2024-04-05 15:26:43.560267 lonboard-0.8.0/lonboard/__main__.py
--rw-r--r--   0        0        0     1418 2024-04-05 15:26:43.560267 lonboard-0.8.0/lonboard/_base.py
--rw-r--r--   0        0        0     4560 2024-04-05 15:26:43.560267 lonboard-0.8.0/lonboard/_cli.py
--rw-r--r--   0        0        0      862 2024-04-05 15:26:43.560267 lonboard-0.8.0/lonboard/_constants.py
--rw-r--r--   0        0        0     1421 2024-04-05 15:26:43.560267 lonboard-0.8.0/lonboard/_environment.py
--rw-r--r--   0        0        0       95 2024-04-05 15:26:43.560267 lonboard-0.8.0/lonboard/_geoarrow/__init__.py
--rw-r--r--   0        0        0      509 2024-04-05 15:26:43.560267 lonboard-0.8.0/lonboard/_geoarrow/crs.py
--rw-r--r--   0        0        0    13399 2024-04-05 15:26:43.560267 lonboard-0.8.0/lonboard/_geoarrow/extension_types.py
--rw-r--r--   0        0        0      716 2024-04-05 15:26:43.560267 lonboard-0.8.0/lonboard/_geoarrow/geopandas_interop.py
--rw-r--r--   0        0        0      174 2024-04-05 15:26:43.560267 lonboard-0.8.0/lonboard/_geoarrow/ops/__init__.py
--rw-r--r--   0        0        0     2619 2024-04-05 15:26:43.560267 lonboard-0.8.0/lonboard/_geoarrow/ops/bbox.py
--rw-r--r--   0        0        0     4584 2024-04-05 15:26:43.560267 lonboard-0.8.0/lonboard/_geoarrow/ops/centroid.py
--rw-r--r--   0        0        0     8208 2024-04-05 15:26:43.560267 lonboard-0.8.0/lonboard/_geoarrow/ops/reproject.py
--rw-r--r--   0        0        0     3416 2024-04-05 15:26:43.560267 lonboard-0.8.0/lonboard/_geoarrow/parse_wkb.py
--rw-r--r--   0        0        0     1801 2024-04-05 15:26:43.560267 lonboard-0.8.0/lonboard/_geoarrow/sanitize.py
--rw-r--r--   0        0        0    55962 2024-04-05 15:26:43.560267 lonboard-0.8.0/lonboard/_layer.py
--rw-r--r--   0        0        0    12187 2024-04-05 15:26:43.560267 lonboard-0.8.0/lonboard/_map.py
--rw-r--r--   0        0        0     3578 2024-04-05 15:26:43.560267 lonboard-0.8.0/lonboard/_serialization.py
--rw-r--r--   0        0        0      285 2024-04-05 15:26:43.560267 lonboard-0.8.0/lonboard/_testing.py
--rw-r--r--   0        0        0     3344 2024-04-05 15:26:43.560267 lonboard-0.8.0/lonboard/_utils.py
--rw-r--r--   0        0        0      166 2024-04-05 15:26:43.560267 lonboard-0.8.0/lonboard/_version.py
--rw-r--r--   0        0        0     2380 2024-04-05 15:26:43.560267 lonboard-0.8.0/lonboard/_viewport.py
--rw-r--r--   0        0        0    15775 2024-04-05 15:26:43.560267 lonboard-0.8.0/lonboard/_viz.py
--rw-r--r--   0        0        0     1367 2024-04-05 15:26:43.560267 lonboard-0.8.0/lonboard/basemap.py
--rw-r--r--   0        0        0     6914 2024-04-05 15:26:43.560267 lonboard-0.8.0/lonboard/colormap.py
--rw-r--r--   0        0        0     2758 2024-04-05 15:26:43.564267 lonboard-0.8.0/lonboard/controls.py
--rw-r--r--   0        0        0      207 2024-04-05 15:26:43.564267 lonboard-0.8.0/lonboard/experimental/__init__.py
--rw-r--r--   0        0        0     9728 2024-04-05 15:26:43.564267 lonboard-0.8.0/lonboard/experimental/_layer.py
--rw-r--r--   0        0        0     9870 2024-04-05 15:26:43.564267 lonboard-0.8.0/lonboard/layer_extension.py
--rw-r--r--   0        0        0      357 2024-04-05 15:26:43.564267 lonboard-0.8.0/lonboard/models.py
--rw-r--r--   0        0        0        0 2024-04-05 15:26:43.564267 lonboard-0.8.0/lonboard/py.typed
--rw-r--r--   0        0        0      385 2024-04-05 15:26:54.336236 lonboard-0.8.0/lonboard/static/index.css
--rw-r--r--   0        0        0  2142403 2024-04-05 15:26:54.336236 lonboard-0.8.0/lonboard/static/index.js
--rw-r--r--   0        0        0    32473 2024-04-05 15:26:43.564267 lonboard-0.8.0/lonboard/traits.py
--rw-r--r--   0        0        0        0 2024-04-05 15:26:43.564267 lonboard-0.8.0/lonboard/types/__init__.py
--rw-r--r--   0        0        0     4535 2024-04-05 15:26:43.564267 lonboard-0.8.0/lonboard/types/layer.py
--rw-r--r--   0        0        0      475 2024-04-05 15:26:43.564267 lonboard-0.8.0/lonboard/types/map.py
--rw-r--r--   0        0        0     2192 2024-04-05 15:26:43.564267 lonboard-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     4179 1970-01-01 00:00:00.000000 lonboard-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-02 13:55:38.236771 lonboard-0.8.0b1/LICENSE
+-rw-r--r--   0        0        0       36 2024-04-02 13:55:38.236771 lonboard-0.8.0b1/MANIFEST.in
+-rw-r--r--   0        0        0     3074 2024-04-02 13:55:38.236771 lonboard-0.8.0b1/README.md
+-rw-r--r--   0        0        0      445 2024-04-02 13:55:38.420771 lonboard-0.8.0b1/lonboard/__init__.py
+-rw-r--r--   0        0        0       39 2024-04-02 13:55:38.420771 lonboard-0.8.0b1/lonboard/__main__.py
+-rw-r--r--   0        0        0     1418 2024-04-02 13:55:38.420771 lonboard-0.8.0b1/lonboard/_base.py
+-rw-r--r--   0        0        0     4411 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/_cli.py
+-rw-r--r--   0        0        0      862 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/_constants.py
+-rw-r--r--   0        0        0     1421 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/_environment.py
+-rw-r--r--   0        0        0       95 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/_geoarrow/__init__.py
+-rw-r--r--   0        0        0      509 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/_geoarrow/crs.py
+-rw-r--r--   0        0        0    13399 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/_geoarrow/extension_types.py
+-rw-r--r--   0        0        0      716 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/_geoarrow/geopandas_interop.py
+-rw-r--r--   0        0        0      174 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/_geoarrow/ops/__init__.py
+-rw-r--r--   0        0        0     2619 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/_geoarrow/ops/bbox.py
+-rw-r--r--   0        0        0     4584 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/_geoarrow/ops/centroid.py
+-rw-r--r--   0        0        0     8208 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/_geoarrow/ops/reproject.py
+-rw-r--r--   0        0        0     3416 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/_geoarrow/parse_wkb.py
+-rw-r--r--   0        0        0     1801 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/_geoarrow/sanitize.py
+-rw-r--r--   0        0        0    55962 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/_layer.py
+-rw-r--r--   0        0        0    12187 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/_map.py
+-rw-r--r--   0        0        0     3578 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/_serialization.py
+-rw-r--r--   0        0        0      285 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/_testing.py
+-rw-r--r--   0        0        0     3344 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/_utils.py
+-rw-r--r--   0        0        0      166 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/_version.py
+-rw-r--r--   0        0        0     2380 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/_viewport.py
+-rw-r--r--   0        0        0    15775 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/_viz.py
+-rw-r--r--   0        0        0     1367 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/basemap.py
+-rw-r--r--   0        0        0     6914 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/colormap.py
+-rw-r--r--   0        0        0     2758 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/controls.py
+-rw-r--r--   0        0        0      207 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/experimental/__init__.py
+-rw-r--r--   0        0        0     9728 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/experimental/_layer.py
+-rw-r--r--   0        0        0     9870 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/layer_extension.py
+-rw-r--r--   0        0        0      357 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/models.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/py.typed
+-rw-r--r--   0        0        0      385 2024-04-02 13:55:48.936756 lonboard-0.8.0b1/lonboard/static/index.css
+-rw-r--r--   0        0        0  2142403 2024-04-02 13:55:48.936756 lonboard-0.8.0b1/lonboard/static/index.js
+-rw-r--r--   0        0        0    32473 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/traits.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/types/__init__.py
+-rw-r--r--   0        0        0     4535 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/types/layer.py
+-rw-r--r--   0        0        0      475 2024-04-02 13:55:38.424771 lonboard-0.8.0b1/lonboard/types/map.py
+-rw-r--r--   0        0        0     2199 2024-04-02 13:55:38.428771 lonboard-0.8.0b1/pyproject.toml
+-rw-r--r--   0        0        0     4181 1970-01-01 00:00:00.000000 lonboard-0.8.0b1/PKG-INFO
```

### Comparing `lonboard-0.8.0/LICENSE` & `lonboard-0.8.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `lonboard-0.8.0/README.md` & `lonboard-0.8.0b1/README.md`

 * *Files identical despite different names*

### Comparing `lonboard-0.8.0/lonboard/_base.py` & `lonboard-0.8.0b1/lonboard/_base.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.8.0/lonboard/_cli.py` & `lonboard-0.8.0b1/lonboard/_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,17 +23,15 @@
     except ImportError as e:
         raise ImportError(
             "pyogrio is a required dependency for the CLI. "
             "Install with `pip install pyogrio`."
         ) from e
 
     meta, table = read_arrow(path)
-    # The `geometry_name` key always exists but can be an empty string. In the case of
-    # an empty string, we want to default to `wkb_geometry`
-    geometry_column_name = meta.get("geometry_name") or "wkb_geometry"
+    geometry_column_name = meta.get("geometry_name", "wkb_geometry")
     # TODO: assert there are not two column names of wkb_geometry, nor an existing
     # column named "geometry"
 
     # Rename wkb_geometry to geometry
     geometry_column_index = [
         i for (i, name) in enumerate(table.column_names) if name == geometry_column_name
     ][0]
```

### Comparing `lonboard-0.8.0/lonboard/_constants.py` & `lonboard-0.8.0b1/lonboard/_constants.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.8.0/lonboard/_environment.py` & `lonboard-0.8.0b1/lonboard/_environment.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.8.0/lonboard/_geoarrow/extension_types.py` & `lonboard-0.8.0b1/lonboard/_geoarrow/extension_types.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.8.0/lonboard/_geoarrow/geopandas_interop.py` & `lonboard-0.8.0b1/lonboard/_geoarrow/geopandas_interop.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.8.0/lonboard/_geoarrow/ops/bbox.py` & `lonboard-0.8.0b1/lonboard/_geoarrow/ops/bbox.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.8.0/lonboard/_geoarrow/ops/centroid.py` & `lonboard-0.8.0b1/lonboard/_geoarrow/ops/centroid.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.8.0/lonboard/_geoarrow/ops/reproject.py` & `lonboard-0.8.0b1/lonboard/_geoarrow/ops/reproject.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.8.0/lonboard/_geoarrow/parse_wkb.py` & `lonboard-0.8.0b1/lonboard/_geoarrow/parse_wkb.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.8.0/lonboard/_geoarrow/sanitize.py` & `lonboard-0.8.0b1/lonboard/_geoarrow/sanitize.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.8.0/lonboard/_layer.py` & `lonboard-0.8.0b1/lonboard/_layer.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.8.0/lonboard/_map.py` & `lonboard-0.8.0b1/lonboard/_map.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.8.0/lonboard/_serialization.py` & `lonboard-0.8.0b1/lonboard/_serialization.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.8.0/lonboard/_utils.py` & `lonboard-0.8.0b1/lonboard/_utils.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.8.0/lonboard/_viewport.py` & `lonboard-0.8.0b1/lonboard/_viewport.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.8.0/lonboard/_viz.py` & `lonboard-0.8.0b1/lonboard/_viz.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.8.0/lonboard/basemap.py` & `lonboard-0.8.0b1/lonboard/basemap.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.8.0/lonboard/colormap.py` & `lonboard-0.8.0b1/lonboard/colormap.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.8.0/lonboard/controls.py` & `lonboard-0.8.0b1/lonboard/controls.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.8.0/lonboard/experimental/_layer.py` & `lonboard-0.8.0b1/lonboard/experimental/_layer.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.8.0/lonboard/layer_extension.py` & `lonboard-0.8.0b1/lonboard/layer_extension.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.8.0/lonboard/static/index.js` & `lonboard-0.8.0b1/lonboard/static/index.js`

 * *Files identical despite different names*

### Comparing `lonboard-0.8.0/lonboard/traits.py` & `lonboard-0.8.0b1/lonboard/traits.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.8.0/lonboard/types/layer.py` & `lonboard-0.8.0b1/lonboard/types/layer.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.8.0/pyproject.toml` & `lonboard-0.8.0b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lonboard"
-version = "0.8.0"
+version = "0.8.0-beta.1"
 description = "Python library for fast, interactive geospatial vector data visualization in Jupyter."
 authors = ["Kyle Barron <kyle@developmentseed.org>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "lonboard" }]
 include = ["lonboard/static/*.js", "lonboard/static/*.css", "MANIFEST.in"]
```

### Comparing `lonboard-0.8.0/PKG-INFO` & `lonboard-0.8.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lonboard
-Version: 0.8.0
+Version: 0.8.0b1
 Summary: Python library for fast, interactive geospatial vector data visualization in Jupyter.
 License: MIT
 Author: Kyle Barron
 Author-email: kyle@developmentseed.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: lonboard Version: 0.8.0 Summary: Python library for
-fast, interactive geospatial vector data visualization in Jupyter. License: MIT
-Author: Kyle Barron Author-email: kyle@developmentseed.org Requires-Python:
+Metadata-Version: 2.1 Name: lonboard Version: 0.8.0b1 Summary: Python library
+for fast, interactive geospatial vector data visualization in Jupyter. License:
+MIT Author: Kyle Barron Author-email: kyle@developmentseed.org Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Provides-
 Extra: cli Requires-Dist: anywidget (>=0.9.0,<0.10.0) Requires-Dist: click
 (>=8.1.7,<9.0.0) ; extra == "cli" Requires-Dist: geopandas (>=0.13) Requires-
```

