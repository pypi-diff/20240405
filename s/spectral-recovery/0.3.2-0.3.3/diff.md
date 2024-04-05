# Comparing `tmp/spectral_recovery-0.3.2.tar.gz` & `tmp/spectral_recovery-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectral_recovery-0.3.2.tar", last modified: Fri Apr  5 00:08:10 2024, max compression
+gzip compressed data, was "spectral_recovery-0.3.3.tar", last modified: Fri Apr  5 18:45:23 2024, max compression
```

## Comparing `spectral_recovery-0.3.2.tar` & `spectral_recovery-0.3.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 00:08:11.097531 spectral_recovery-0.3.2/
--rw-rw-rw-   0        0        0    10349 2023-10-11 06:09:47.000000 spectral_recovery-0.3.2/LICENSE
--rw-rw-rw-   0        0        0    16166 2024-04-05 00:08:11.073834 spectral_recovery-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     3325 2024-01-02 16:59:25.000000 spectral_recovery-0.3.2/README.md
--rw-rw-rw-   0        0        0     1192 2024-04-05 00:00:41.000000 spectral_recovery-0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 00:08:11.100858 spectral_recovery-0.3.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-05 00:08:10.359881 spectral_recovery-0.3.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 00:08:10.342608 spectral_recovery-0.3.2/src/scripts/
--rw-rw-rw-   0        0        0        0 2023-10-11 06:09:52.000000 spectral_recovery-0.3.2/src/scripts/__init__.py
--rw-rw-rw-   0        0        0     5268 2024-03-12 20:57:23.000000 spectral_recovery-0.3.2/src/scripts/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-05 00:08:10.769207 spectral_recovery-0.3.2/src/spectral_recovery/
--rw-rw-rw-   0        0        0      432 2024-04-04 23:49:27.000000 spectral_recovery-0.3.2/src/spectral_recovery/__init__.py
--rw-rw-rw-   0        0        0      566 2024-04-02 21:36:55.000000 spectral_recovery-0.3.2/src/spectral_recovery/_config.py
--rw-rw-rw-   0        0        0     4597 2024-03-19 20:21:39.000000 spectral_recovery-0.3.2/src/spectral_recovery/_utils.py
--rw-rw-rw-   0        0        0      517 2024-03-12 20:57:23.000000 spectral_recovery-0.3.2/src/spectral_recovery/enums.py
--rw-rw-rw-   0        0        0     3709 2024-04-02 21:36:55.000000 spectral_recovery-0.3.2/src/spectral_recovery/indices.py
-drwxrwxrwx   0        0        0        0 2024-04-05 00:08:11.012933 spectral_recovery-0.3.2/src/spectral_recovery/io/
--rw-rw-rw-   0        0        0        0 2024-02-13 22:18:33.000000 spectral_recovery-0.3.2/src/spectral_recovery/io/__init__.py
--rw-rw-rw-   0        0        0     4797 2024-03-28 17:22:15.000000 spectral_recovery-0.3.2/src/spectral_recovery/io/polygon.py
--rw-rw-rw-   0        0        0     8536 2024-04-02 21:36:55.000000 spectral_recovery-0.3.2/src/spectral_recovery/io/raster.py
--rw-rw-rw-   0        0        0    11419 2024-04-04 23:49:27.000000 spectral_recovery-0.3.2/src/spectral_recovery/metrics.py
--rw-rw-rw-   0        0        0     9674 2024-04-04 23:58:44.000000 spectral_recovery-0.3.2/src/spectral_recovery/plotting.py
--rw-rw-rw-   0        0        0    20944 2024-03-19 20:21:39.000000 spectral_recovery-0.3.2/src/spectral_recovery/restoration.py
--rw-rw-rw-   0        0        0    11375 2024-03-19 20:21:39.000000 spectral_recovery-0.3.2/src/spectral_recovery/targets.py
--rw-rw-rw-   0        0        0     5766 2024-03-19 20:21:39.000000 spectral_recovery-0.3.2/src/spectral_recovery/timeseries.py
-drwxrwxrwx   0        0        0        0 2024-04-05 00:08:11.053486 spectral_recovery-0.3.2/src/spectral_recovery.egg-info/
--rw-rw-rw-   0        0        0    16166 2024-04-05 00:08:09.000000 spectral_recovery-0.3.2/src/spectral_recovery.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      791 2024-04-05 00:08:10.000000 spectral_recovery-0.3.2/src/spectral_recovery.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 00:08:09.000000 spectral_recovery-0.3.2/src/spectral_recovery.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-04-05 00:08:09.000000 spectral_recovery-0.3.2/src/spectral_recovery.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      308 2024-04-05 00:08:10.000000 spectral_recovery-0.3.2/src/spectral_recovery.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-05 00:08:10.000000 spectral_recovery-0.3.2/src/spectral_recovery.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 18:45:24.765288 spectral_recovery-0.3.3/
+-rw-rw-rw-   0        0        0    10349 2023-10-11 06:09:47.000000 spectral_recovery-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0    16166 2024-04-05 18:45:24.741288 spectral_recovery-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3325 2024-01-02 16:59:25.000000 spectral_recovery-0.3.3/README.md
+-rw-rw-rw-   0        0        0     1192 2024-04-05 18:44:34.000000 spectral_recovery-0.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 18:45:24.768343 spectral_recovery-0.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 18:45:23.990643 spectral_recovery-0.3.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 18:45:24.116820 spectral_recovery-0.3.3/src/scripts/
+-rw-rw-rw-   0        0        0        0 2023-10-11 06:09:52.000000 spectral_recovery-0.3.3/src/scripts/__init__.py
+-rw-rw-rw-   0        0        0     5268 2024-03-12 20:57:23.000000 spectral_recovery-0.3.3/src/scripts/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:45:24.401751 spectral_recovery-0.3.3/src/spectral_recovery/
+-rw-rw-rw-   0        0        0      485 2024-04-05 18:35:52.000000 spectral_recovery-0.3.3/src/spectral_recovery/__init__.py
+-rw-rw-rw-   0        0        0      566 2024-04-02 21:36:55.000000 spectral_recovery-0.3.3/src/spectral_recovery/_config.py
+-rw-rw-rw-   0        0        0     4597 2024-03-19 20:21:39.000000 spectral_recovery-0.3.3/src/spectral_recovery/_utils.py
+-rw-rw-rw-   0        0        0      517 2024-03-12 20:57:23.000000 spectral_recovery-0.3.3/src/spectral_recovery/enums.py
+-rw-rw-rw-   0        0        0     3709 2024-04-02 21:36:55.000000 spectral_recovery-0.3.3/src/spectral_recovery/indices.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:45:24.672863 spectral_recovery-0.3.3/src/spectral_recovery/io/
+-rw-rw-rw-   0        0        0        0 2024-02-13 22:18:33.000000 spectral_recovery-0.3.3/src/spectral_recovery/io/__init__.py
+-rw-rw-rw-   0        0        0     4797 2024-03-28 17:22:15.000000 spectral_recovery-0.3.3/src/spectral_recovery/io/polygon.py
+-rw-rw-rw-   0        0        0     8536 2024-04-02 21:36:55.000000 spectral_recovery-0.3.3/src/spectral_recovery/io/raster.py
+-rw-rw-rw-   0        0        0    11227 2024-04-05 18:35:52.000000 spectral_recovery-0.3.3/src/spectral_recovery/metrics.py
+-rw-rw-rw-   0        0        0     9548 2024-04-05 18:35:52.000000 spectral_recovery-0.3.3/src/spectral_recovery/plotting.py
+-rw-rw-rw-   0        0        0    20944 2024-03-19 20:21:39.000000 spectral_recovery-0.3.3/src/spectral_recovery/restoration.py
+-rw-rw-rw-   0        0        0    11375 2024-03-19 20:21:39.000000 spectral_recovery-0.3.3/src/spectral_recovery/targets.py
+-rw-rw-rw-   0        0        0     5766 2024-03-19 20:21:39.000000 spectral_recovery-0.3.3/src/spectral_recovery/timeseries.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:45:24.720682 spectral_recovery-0.3.3/src/spectral_recovery.egg-info/
+-rw-rw-rw-   0        0        0    16166 2024-04-05 18:45:23.000000 spectral_recovery-0.3.3/src/spectral_recovery.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      791 2024-04-05 18:45:23.000000 spectral_recovery-0.3.3/src/spectral_recovery.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 18:45:23.000000 spectral_recovery-0.3.3/src/spectral_recovery.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-04-05 18:45:23.000000 spectral_recovery-0.3.3/src/spectral_recovery.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      308 2024-04-05 18:45:23.000000 spectral_recovery-0.3.3/src/spectral_recovery.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-05 18:45:23.000000 spectral_recovery-0.3.3/src/spectral_recovery.egg-info/top_level.txt
```

### Comparing `spectral_recovery-0.3.2/LICENSE` & `spectral_recovery-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spectral_recovery-0.3.2/PKG-INFO` & `spectral_recovery-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectral_recovery
-Version: 0.3.2
+Version: 0.3.3
 Author-email: Sarah Zwiep <sarahvz@mail.ubc.ca>
 Maintainer-email: Sarah Zwiep <sarahvz@mail.ubc.ca>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `spectral_recovery-0.3.2/README.md` & `spectral_recovery-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `spectral_recovery-0.3.2/pyproject.toml` & `spectral_recovery-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python"
 ]
-version = "0.3.2"
+version = "0.3.3"
 dependencies = [
     "geopandas >= 0.13.2",
     "rioxarray >= 0.14.1",
     "rasterio >= 1.3.7",
     "xarray >= 2023.5.0",
     "spyndex == 0.5.0",
     "numpy >= 1.24.3",
```

### Comparing `spectral_recovery-0.3.2/src/scripts/cli.py` & `spectral_recovery-0.3.3/src/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `spectral_recovery-0.3.2/src/spectral_recovery/_config.py` & `spectral_recovery-0.3.3/src/spectral_recovery/_config.py`

 * *Files identical despite different names*

### Comparing `spectral_recovery-0.3.2/src/spectral_recovery/_utils.py` & `spectral_recovery-0.3.3/src/spectral_recovery/_utils.py`

 * *Files identical despite different names*

### Comparing `spectral_recovery-0.3.2/src/spectral_recovery/enums.py` & `spectral_recovery-0.3.3/src/spectral_recovery/enums.py`

 * *Files identical despite different names*

### Comparing `spectral_recovery-0.3.2/src/spectral_recovery/indices.py` & `spectral_recovery-0.3.3/src/spectral_recovery/indices.py`

 * *Files identical despite different names*

### Comparing `spectral_recovery-0.3.2/src/spectral_recovery/io/polygon.py` & `spectral_recovery-0.3.3/src/spectral_recovery/io/polygon.py`

 * *Files identical despite different names*

### Comparing `spectral_recovery-0.3.2/src/spectral_recovery/io/raster.py` & `spectral_recovery-0.3.3/src/spectral_recovery/io/raster.py`

 * *Files identical despite different names*

### Comparing `spectral_recovery-0.3.2/src/spectral_recovery/metrics.py` & `spectral_recovery-0.3.3/src/spectral_recovery/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,28 +25,23 @@
 
 
 @maintain_rio_attrs
 def compute_metrics(
     timeseries_data: xr.DataArray,
     restoration_polygons: gpd.GeoDataFrame,
     metrics: List[str],
-    indices: List[str],
     reference_polygons: gpd.GeoDataFrame = None,
-    index_constants: Dict[str, int] = {},
     timestep: int = 5,
     percent_of_target: int = 80,
     recovery_target_method=MedianTarget(scale="polygon"),
 ):
-    indices_stack = compute_indices(
-        image_stack=timeseries_data, indices=indices, constants=index_constants
-    )
     restoration_area = RestorationArea(
         restoration_polygon=restoration_polygons,
         reference_polygons=reference_polygons,
-        composite_stack=indices_stack,
+        composite_stack=timeseries_data,
         recovery_target_method=recovery_target_method,
     )
     m_results = []
     for m in metrics:
         try:
             m_func = METRIC_FUNCS[m.lower()]
         except KeyError:
```

### Comparing `spectral_recovery-0.3.2/src/spectral_recovery/plotting.py` & `spectral_recovery-0.3.3/src/spectral_recovery/plotting.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,20 +10,19 @@
 from matplotlib.legend_handler import HandlerPatch
 
 from spectral_recovery.restoration import RestorationArea
 from spectral_recovery.targets import MedianTarget
 from spectral_recovery.indices import compute_indices
 
 
+# TODO: Refactor. Bring plot_spectral_trajectory into this module.
 def plot_spectral_trajectory(
     timeseries_data: xr.DataArray,
     restoration_polygons: gpd.GeoDataFrame,
-    indices: List[str],
     reference_polygons: gpd.GeoDataFrame = None,
-    index_constants: Dict[str, int] = {},
     recovery_target_method=MedianTarget(scale="polygon"),
     path: str = None,
 ):
     """Plot the spectral trajectory of the restoration polygon
 
     Parameters
     ----------
@@ -37,22 +36,18 @@
         The refernce polygons to compute recovery target with
     indices_constants : dict
         Constant values for indices
     recovery_target_method : callable
         Recovery target method to derive recovery target values
 
     """
-
-    indices_stack = compute_indices(
-        image_stack=timeseries_data, indices=indices, constants=index_constants
-    )
     restoration_area = RestorationArea(
         restoration_polygon=restoration_polygons,
         reference_polygons=reference_polygons,
-        composite_stack=indices_stack,
+        composite_stack=timeseries_data,
         recovery_target_method=recovery_target_method,
     )
     if path:
         plot_ra(ra=restoration_area, path=path)
     else:
         plot_ra(ra=restoration_area)
```

### Comparing `spectral_recovery-0.3.2/src/spectral_recovery/restoration.py` & `spectral_recovery-0.3.3/src/spectral_recovery/restoration.py`

 * *Files identical despite different names*

### Comparing `spectral_recovery-0.3.2/src/spectral_recovery/targets.py` & `spectral_recovery-0.3.3/src/spectral_recovery/targets.py`

 * *Files identical despite different names*

### Comparing `spectral_recovery-0.3.2/src/spectral_recovery/timeseries.py` & `spectral_recovery-0.3.3/src/spectral_recovery/timeseries.py`

 * *Files identical despite different names*

### Comparing `spectral_recovery-0.3.2/src/spectral_recovery.egg-info/PKG-INFO` & `spectral_recovery-0.3.3/src/spectral_recovery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectral_recovery
-Version: 0.3.2
+Version: 0.3.3
 Author-email: Sarah Zwiep <sarahvz@mail.ubc.ca>
 Maintainer-email: Sarah Zwiep <sarahvz@mail.ubc.ca>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `spectral_recovery-0.3.2/src/spectral_recovery.egg-info/SOURCES.txt` & `spectral_recovery-0.3.3/src/spectral_recovery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

