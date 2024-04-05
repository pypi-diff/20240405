# Comparing `tmp/quackosm-0.5.2.tar.gz` & `tmp/quackosm-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quackosm-0.5.2.tar", last modified: Wed Apr  3 13:01:15 2024, max compression
+gzip compressed data, was "quackosm-0.5.3.tar", last modified: Fri Apr  5 17:36:04 2024, max compression
```

## Comparing `quackosm-0.5.2.tar` & `quackosm-0.5.3.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0    11339 2024-04-03 13:00:45.769424 quackosm-0.5.2/LICENSE
--rw-r--r--   0        0        0    25727 2024-04-03 13:00:45.769424 quackosm-0.5.2/README.md
--rw-r--r--   0        0        0     4326 2024-04-03 13:01:15.233232 quackosm-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      560 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/__init__.py
--rw-r--r--   0        0        0      464 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/__main__.py
--rw-r--r--   0        0        0      127 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/_constants.py
--rw-r--r--   0        0        0      135 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/_exceptions.py
--rw-r--r--   0        0        0     4406 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/_osm_tags_filters.py
--rw-r--r--   0        0        0     1188 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/_osm_way_polygon_features.py
--rw-r--r--   0        0        0     6013 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/_rich_progress.py
--rw-r--r--   0        0        0      717 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/_typing.py
--rw-r--r--   0        0        0    23859 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/cli.py
--rw-r--r--   0        0        0     1875 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/conftest.py
--rw-r--r--   0        0        0    51009 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/functions.py
--rw-r--r--   0        0        0    19065 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/osm_extracts/__init__.py
--rw-r--r--   0        0        0     2320 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/osm_extracts/_poly_parser.py
--rw-r--r--   0        0        0     3141 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/osm_extracts/bbbike.py
--rw-r--r--   0        0        0      251 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/osm_extracts/extract.py
--rw-r--r--   0        0        0     1687 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/osm_extracts/geofabrik.py
--rw-r--r--   0        0        0     4098 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/osm_extracts/osm_fr.py
--rw-r--r--   0        0        0     3362 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/osm_way_polygon_features.json
--rw-r--r--   0        0        0   106840 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/pbf_file_reader.py
--rw-r--r--   0        0        0       33 2024-04-03 13:00:45.777424 quackosm-0.5.2/tests/__init__.py
--rw-r--r--   0        0        0       38 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/base/__init__.py
--rw-r--r--   0        0        0    24681 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/base/test_cli.py
--rw-r--r--   0        0        0     5422 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/base/test_osm_extracts.py
--rw-r--r--   0        0        0    39391 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/base/test_pbf_file_reader.py
--rw-r--r--   0        0        0       43 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/benchmark/__init__.py
--rw-r--r--   0        0        0      919 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/benchmark/test_big_file.py
--rw-r--r--   0        0        0     1472 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/optional_imports/test_optional_cli_dependency.py
--rw-r--r--   0        0        0      342 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
--rw-r--r--   0        0        0      100 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
--rw-r--r--   0        0        0      770 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
--rw-r--r--   0        0        0    73746 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
--rw-r--r--   0        0        0     1013 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
--rw-r--r--   0        0        0   537903 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/test_files/monaco.osm.pbf
--rw-r--r--   0        0        0    91717 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/test_files/monaco_boundary.geojson
--rw-r--r--   0        0        0      112 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/test_files/osm_tags_filter.json
--rw-r--r--   0        0        0     5405 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/test_files/osmconf.ini
--rw-r--r--   0        0        0    27504 1970-01-01 00:00:00.000000 quackosm-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    11339 2024-04-05 17:35:36.291367 quackosm-0.5.3/LICENSE
+-rw-r--r--   0        0        0    25727 2024-04-05 17:35:36.291367 quackosm-0.5.3/README.md
+-rw-r--r--   0        0        0     4326 2024-04-05 17:36:04.067172 quackosm-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      560 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/__init__.py
+-rw-r--r--   0        0        0      464 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/__main__.py
+-rw-r--r--   0        0        0      127 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/_constants.py
+-rw-r--r--   0        0        0      135 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/_exceptions.py
+-rw-r--r--   0        0        0     4406 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/_osm_tags_filters.py
+-rw-r--r--   0        0        0     1188 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/_osm_way_polygon_features.py
+-rw-r--r--   0        0        0     6013 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/_rich_progress.py
+-rw-r--r--   0        0        0      717 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/_typing.py
+-rw-r--r--   0        0        0    23859 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/cli.py
+-rw-r--r--   0        0        0     1875 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/conftest.py
+-rw-r--r--   0        0        0    51009 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/functions.py
+-rw-r--r--   0        0        0    19065 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/osm_extracts/__init__.py
+-rw-r--r--   0        0        0     2320 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/osm_extracts/_poly_parser.py
+-rw-r--r--   0        0        0     3141 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/osm_extracts/bbbike.py
+-rw-r--r--   0        0        0      251 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/osm_extracts/extract.py
+-rw-r--r--   0        0        0     1687 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/osm_extracts/geofabrik.py
+-rw-r--r--   0        0        0     4098 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/osm_extracts/osm_fr.py
+-rw-r--r--   0        0        0     3362 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/osm_way_polygon_features.json
+-rw-r--r--   0        0        0   107058 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/pbf_file_reader.py
+-rw-r--r--   0        0        0       33 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/base/__init__.py
+-rw-r--r--   0        0        0      746 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/base/conftest.py
+-rw-r--r--   0        0        0    24088 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/base/test_cli.py
+-rw-r--r--   0        0        0     5422 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/base/test_osm_extracts.py
+-rw-r--r--   0        0        0    40294 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/base/test_pbf_file_reader.py
+-rw-r--r--   0        0        0       43 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/benchmark/__init__.py
+-rw-r--r--   0        0        0      919 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/benchmark/test_big_file.py
+-rw-r--r--   0        0        0     1472 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/optional_imports/test_optional_cli_dependency.py
+-rw-r--r--   0        0        0      342 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
+-rw-r--r--   0        0        0      100 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
+-rw-r--r--   0        0        0      770 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
+-rw-r--r--   0        0        0    73746 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
+-rw-r--r--   0        0        0     1013 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
+-rw-r--r--   0        0        0   537903 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/test_files/monaco.osm.pbf
+-rw-r--r--   0        0        0    91717 2024-04-05 17:35:36.307367 quackosm-0.5.3/tests/test_files/monaco_boundary.geojson
+-rw-r--r--   0        0        0      112 2024-04-05 17:35:36.307367 quackosm-0.5.3/tests/test_files/osm_tags_filter.json
+-rw-r--r--   0        0        0     5405 2024-04-05 17:35:36.307367 quackosm-0.5.3/tests/test_files/osmconf.ini
+-rw-r--r--   0        0        0    27504 1970-01-01 00:00:00.000000 quackosm-0.5.3/PKG-INFO
```

### Comparing `quackosm-0.5.2/LICENSE` & `quackosm-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.2/README.md` & `quackosm-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.2/pyproject.toml` & `quackosm-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "QuackOSM"
-version = "0.5.2"
+version = "0.5.3"
 description = "An open-source tool for reading OpenStreetMap PBF files using DuckDB"
 authors = [
     { name = "Kamil Raczycki", email = "kraczycki@kraina.ai" },
 ]
 dependencies = [
     "geopandas",
     "shapely>=2",
@@ -184,15 +184,15 @@
 tab-width = 4
 blank = false
 pre-summary-newline = true
 close-quotes-on-newline = true
 wrap-one-line = true
 
 [tool.bumpver]
-current_version = "0.5.2"
+current_version = "0.5.3"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "chore(CI/CD): bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `quackosm-0.5.2/quackosm/__init__.py` & `quackosm-0.5.3/quackosm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     convert_pbf_to_gpq,
     get_features_gdf,
     get_features_gdf_from_geometry,
 )
 from quackosm.pbf_file_reader import PbfFileReader
 
 __app_name__ = "QuackOSM"
-__version__ = "0.5.2"
+__version__ = "0.5.3"
 
 __all__ = [
     "PbfFileReader",
     "convert_pbf_to_gpq",
     "convert_geometry_to_gpq",
     "get_features_gdf",
     "get_features_gdf_from_geometry",
```

### Comparing `quackosm-0.5.2/quackosm/_osm_tags_filters.py` & `quackosm-0.5.3/quackosm/_osm_tags_filters.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.2/quackosm/_osm_way_polygon_features.py` & `quackosm-0.5.3/quackosm/_osm_way_polygon_features.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.2/quackosm/_rich_progress.py` & `quackosm-0.5.3/quackosm/_rich_progress.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.2/quackosm/_typing.py` & `quackosm-0.5.3/quackosm/_typing.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.2/quackosm/cli.py` & `quackosm-0.5.3/quackosm/cli.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.2/quackosm/conftest.py` & `quackosm-0.5.3/quackosm/conftest.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.2/quackosm/functions.py` & `quackosm-0.5.3/quackosm/functions.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.2/quackosm/osm_extracts/__init__.py` & `quackosm-0.5.3/quackosm/osm_extracts/__init__.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.2/quackosm/osm_extracts/_poly_parser.py` & `quackosm-0.5.3/quackosm/osm_extracts/_poly_parser.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.2/quackosm/osm_extracts/bbbike.py` & `quackosm-0.5.3/quackosm/osm_extracts/bbbike.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.2/quackosm/osm_extracts/geofabrik.py` & `quackosm-0.5.3/quackosm/osm_extracts/geofabrik.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.2/quackosm/osm_extracts/osm_fr.py` & `quackosm-0.5.3/quackosm/osm_extracts/osm_fr.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.2/quackosm/osm_way_polygon_features.json` & `quackosm-0.5.3/quackosm/osm_way_polygon_features.json`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.2/quackosm/pbf_file_reader.py` & `quackosm-0.5.3/quackosm/pbf_file_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -507,14 +507,17 @@
         ).set_index(FEATURES_INDEX)
 
         return gdf_parquet
 
     def _drop_duplicated_features_in_pyarrow_table(
         self, parsed_geoparquet_files: list[Path]
     ) -> pa.Table:
+        if len(parsed_geoparquet_files) == 1:
+            return pq.read_table(parsed_geoparquet_files[0])
+
         with TaskProgressSpinner("Combining results", "", self.silent_mode, skip_step_number=True):
             parquet_tables = [
                 pq.read_table(parsed_parquet_file)
                 for parsed_parquet_file in parsed_geoparquet_files
             ]
             joined_parquet_table: pa.Table = pa.concat_tables(
                 parquet_tables, promote_options="default"
@@ -792,15 +795,18 @@
 
         if geometry is None:
             geometry = self.geometry_filter
 
         if isinstance(geometry, LinearRing):
             # https://stackoverflow.com/a/73073112/7766101
             new_coords = []
-            perimeter = list(geometry.coords)
+            if geometry.is_ccw:
+                perimeter = list(geometry.coords)
+            else:
+                perimeter = list(geometry.coords)[::-1]
             smallest_point = sorted(perimeter)[0]
             double_iteration = itertools.chain(perimeter[:-1], perimeter)
             for point in double_iteration:
                 if point == smallest_point:
                     new_coords.append((round(point[0], 7), round(point[1], 7)))
                     while len(new_coords) < len(perimeter):
                         next_point = next(double_iteration)
```

### Comparing `quackosm-0.5.2/tests/base/test_cli.py` & `quackosm-0.5.3/tests/base/test_cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,28 @@
 """Tests for CLI."""
 
 import uuid
 from pathlib import Path
 
 import pytest
 from parametrization import Parametrization as P
-from shapely import to_geojson, to_wkt
-from shapely.geometry import Polygon, box
 from typer.testing import CliRunner
 
 from quackosm import __app_name__, __version__, cli
+from tests.base.conftest import geometry_boundary_file_path, geometry_geojson, geometry_wkt
 
 runner = CliRunner()
 
 
 @pytest.fixture()  # type: ignore
 def monaco_pbf_file_path() -> str:
     """Monaco PBF file path fixture."""
     return str(Path(__file__).parent.parent / "test_files" / "monaco.osm.pbf")
 
 
-def geometry_box() -> Polygon:
-    """Geometry box."""
-    return box(
-        minx=7.416486207767861,
-        miny=43.7310867041912,
-        maxx=7.421931388477276,
-        maxy=43.73370705597216,
-    )
-
-
-def geometry_wkt() -> str:
-    """Geometry box in WKT form."""
-    return str(to_wkt(geometry_box()))
-
-
-def geometry_geojson() -> str:
-    """Geometry box in GeoJSON form."""
-    return str(to_geojson(geometry_box()))
-
-
-def geometry_boundary_file_path() -> str:
-    """Geometry Monaco boundary file path."""
-    return str(Path(__file__).parent.parent / "test_files" / "monaco_boundary.geojson")
-
-
 def osm_tags_filter_file_path() -> str:
     """OSM tags filter file path."""
     return str(Path(__file__).parent.parent / "test_files" / "osm_tags_filter.json")
 
 
 def osm_way_config_file_path() -> str:
     """OSM way features config file path."""
@@ -178,50 +152,50 @@
     "Geometry GeoJSON filter",
     ["--geom-filter-geojson", geometry_geojson()],
     "files/monaco_nofilter_82c0fdfa2d5654818a03540644834d70c353e3f82f9d8f201c37420aeb35118e_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "Geometry file filter",
     ["--geom-filter-file", geometry_boundary_file_path()],
-    "files/monaco_nofilter_6e3ec5872bf41c2c44698fcf71266971c552d13feea19c3714e171bcd7a2b2c8_compact.geoparquet",
+    "files/monaco_nofilter_6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "Geometry geocode filter",
     ["--geom-filter-geocode", "Monaco-Ville, Monaco"],
     "files/monaco_nofilter_e7f0b78a0fdc16c4db31c9767fa4e639eadaa8e83a9b90e07b521f4925cdf4b3_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "Geometry Geohash filter",
     ["--geom-filter-index-geohash", "spv2bc"],
     "files/monaco_nofilter_c08889e81575260e7ea2bc9764ddaa7c5e1141270a890b022799689d39dfe4d5_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "Geometry Geohash filter multiple",
     ["--geom-filter-index-geohash", "spv2bc,spv2bfr"],
-    "files/monaco_nofilter_72883922e5d6e81ab15e5bc2104bd7318d28ffe897a1858f64ba77bafdf62d66_compact.geoparquet",
+    "files/monaco_nofilter_1bd33e0afc3cd0efcb4740185b8a05ecaf1bac916d571403768939b82844b43e_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "Geometry H3 filter",
     ["--geom-filter-index-h3", "8a3969a40ac7fff"],
     "files/monaco_nofilter_a2f8d5114760394646aa999a1204adaa48ad686b3fcadb0b25fd02322c16dff4_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "Geometry H3 filter multiple",
     ["--geom-filter-index-h3", "8a3969a40ac7fff,893969a4037ffff"],
-    "files/monaco_nofilter_9671a25e17150e6171275ed3dc3a96099386644dbbb93d6f4222360e840b7799_compact.geoparquet",
+    "files/monaco_nofilter_e50e6489d4faba664a3c7f9729b7a3bedafb7a396ae826521f32b556d0b554f1_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "Geometry S2 filter",
     ["--geom-filter-index-s2", "12cdc28bc"],
     "files/monaco_nofilter_5c3d61eb108819e543a1a59fe6c67658f817c0453d728b5aa007f227453d5bf6_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "Geometry S2 filter multiple",
     ["--geom-filter-index-s2", "12cdc28bc,12cdc28f"],
-    "files/monaco_nofilter_35e189b968b4f8d8c27c25b0dab484a6623745d1c85dcb77d19599ed0f7ba802_compact.geoparquet",
+    "files/monaco_nofilter_cda5d65e169e3ff04970e66e80b021937a5ae141ed72428cc0d9a3764bf076db_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "Filter OSM features IDs",
     ["--filter-osm-ids", "way/94399646,node/3617982224,relation/36990"],
     "files/monaco_nofilter_noclip_compact_c740a1597e53ae8c5e98c5119eaa1893ddc177161afe8642addcbe54a6dc089d.geoparquet",
 )  # type: ignore
 @P.case(
@@ -298,75 +272,75 @@
     "Geometry Geohash filter",
     ["--geom-filter-index-geohash", "spv2bc"],
     "files/c08889e81575260e7ea2bc9764ddaa7c5e1141270a890b022799689d39dfe4d5_nofilter_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "Geometry Geohash filter multiple",
     ["--geom-filter-index-geohash", "spv2bc,spv2bfr"],
-    "files/72883922e5d6e81ab15e5bc2104bd7318d28ffe897a1858f64ba77bafdf62d66_nofilter_compact.geoparquet",
+    "files/1bd33e0afc3cd0efcb4740185b8a05ecaf1bac916d571403768939b82844b43e_nofilter_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "Geometry H3 filter",
     ["--geom-filter-index-h3", "8a3969a40ac7fff"],
     "files/a2f8d5114760394646aa999a1204adaa48ad686b3fcadb0b25fd02322c16dff4_nofilter_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "Geometry H3 filter multiple",
     ["--geom-filter-index-h3", "8a3969a40ac7fff,893969a4037ffff"],
-    "files/9671a25e17150e6171275ed3dc3a96099386644dbbb93d6f4222360e840b7799_nofilter_compact.geoparquet",
+    "files/e50e6489d4faba664a3c7f9729b7a3bedafb7a396ae826521f32b556d0b554f1_nofilter_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "Geometry S2 filter",
     ["--geom-filter-index-s2", "12cdc28bc"],
     "files/5c3d61eb108819e543a1a59fe6c67658f817c0453d728b5aa007f227453d5bf6_nofilter_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "Geometry S2 filter multiple",
     ["--geom-filter-index-s2", "12cdc28bc,12cdc28f"],
-    "files/35e189b968b4f8d8c27c25b0dab484a6623745d1c85dcb77d19599ed0f7ba802_nofilter_compact.geoparquet",
+    "files/cda5d65e169e3ff04970e66e80b021937a5ae141ed72428cc0d9a3764bf076db_nofilter_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "Geometry file filter with different OSM source",
     ["--geom-filter-file", geometry_boundary_file_path(), "--osm-extract-source", "OSMfr"],
-    "files/6e3ec5872bf41c2c44698fcf71266971c552d13feea19c3714e171bcd7a2b2c8_nofilter_compact.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "Explode",
     ["--geom-filter-file", geometry_boundary_file_path(), "--explode-tags"],
-    "files/6e3ec5872bf41c2c44698fcf71266971c552d13feea19c3714e171bcd7a2b2c8_nofilter_exploded.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_exploded.geoparquet",
 )  # type: ignore
 @P.case(
     "Explode short",
     ["--geom-filter-file", geometry_boundary_file_path(), "--explode"],
-    "files/6e3ec5872bf41c2c44698fcf71266971c552d13feea19c3714e171bcd7a2b2c8_nofilter_exploded.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_exploded.geoparquet",
 )  # type: ignore
 @P.case(
     "Compact",
     ["--geom-filter-file", geometry_boundary_file_path(), "--compact-tags"],
-    "files/6e3ec5872bf41c2c44698fcf71266971c552d13feea19c3714e171bcd7a2b2c8_nofilter_compact.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "Compact short",
     ["--geom-filter-file", geometry_boundary_file_path(), "--compact"],
-    "files/6e3ec5872bf41c2c44698fcf71266971c552d13feea19c3714e171bcd7a2b2c8_nofilter_compact.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "Working directory",
     ["--geom-filter-file", geometry_boundary_file_path(), "--working-directory", "files/workdir"],
-    "files/workdir/6e3ec5872bf41c2c44698fcf71266971c552d13feea19c3714e171bcd7a2b2c8_nofilter_compact.geoparquet",
+    "files/workdir/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "Ignore cache",
     ["--geom-filter-file", geometry_boundary_file_path(), "--ignore-cache"],
-    "files/6e3ec5872bf41c2c44698fcf71266971c552d13feea19c3714e171bcd7a2b2c8_nofilter_compact.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "Ignore cache short",
     ["--geom-filter-file", geometry_boundary_file_path(), "--no-cache"],
-    "files/6e3ec5872bf41c2c44698fcf71266971c552d13feea19c3714e171bcd7a2b2c8_nofilter_compact.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "Output",
     [
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--output",
@@ -395,132 +369,132 @@
     "OSM tags filter",
     [
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--osm-tags-filter",
         '{"building": true, "highway": ["primary", "secondary"], "amenity": "bench"}',
     ],
-    "files/6e3ec5872bf41c2c44698fcf71266971c552d13feea19c3714e171bcd7a2b2c8_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_exploded.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_exploded.geoparquet",
 )  # type: ignore
 @P.case(
     "OSM tags filter compact",
     [
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--osm-tags-filter",
         '{"building": true, "highway": ["primary", "secondary"], "amenity": "bench"}',
         "--compact",
     ],
-    "files/6e3ec5872bf41c2c44698fcf71266971c552d13feea19c3714e171bcd7a2b2c8_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_compact.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "OSM tags filter file",
     [
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--osm-tags-filter-file",
         osm_tags_filter_file_path(),
     ],
-    "files/6e3ec5872bf41c2c44698fcf71266971c552d13feea19c3714e171bcd7a2b2c8_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_exploded.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_exploded.geoparquet",
 )  # type: ignore
 @P.case(
     "OSM tags filter file compact",
     [
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--osm-tags-filter-file",
         osm_tags_filter_file_path(),
         "--compact",
     ],
-    "files/6e3ec5872bf41c2c44698fcf71266971c552d13feea19c3714e171bcd7a2b2c8_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_compact.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "OSM tags filter grouped",
     [
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--osm-tags-filter",
         '{"group": {"building": true, "highway": ["primary", "secondary"], "amenity": "bench"} }',
     ],
-    "files/6e3ec5872bf41c2c44698fcf71266971c552d13feea19c3714e171bcd7a2b2c8_654daac5550b95c8c0e3c57a75a1e16dfa638946461e0977af8f9ca98039db06_exploded.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_654daac5550b95c8c0e3c57a75a1e16dfa638946461e0977af8f9ca98039db06_exploded.geoparquet",
 )  # type: ignore
 @P.case(
     "OSM tags filter grouped compact",
     [
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--osm-tags-filter",
         '{"group": {"building": true, "highway": ["primary", "secondary"], "amenity": "bench"} }',
         "--compact",
     ],
-    "files/6e3ec5872bf41c2c44698fcf71266971c552d13feea19c3714e171bcd7a2b2c8_654daac5550b95c8c0e3c57a75a1e16dfa638946461e0977af8f9ca98039db06_compact.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_654daac5550b95c8c0e3c57a75a1e16dfa638946461e0977af8f9ca98039db06_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "Filter OSM features IDs",
     [
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--filter-osm-ids",
         "way/94399646,node/3617982224,relation/36990",
     ],
-    "files/6e3ec5872bf41c2c44698fcf71266971c552d13feea19c3714e171bcd7a2b2c8_nofilter_compact_c740a1597e53ae8c5e98c5119eaa1893ddc177161afe8642addcbe54a6dc089d.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_compact_c740a1597e53ae8c5e98c5119eaa1893ddc177161afe8642addcbe54a6dc089d.geoparquet",
 )  # type: ignore
 @P.case(
     "Keep all tags",
     [
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--keep-all-tags",
     ],
-    "files/6e3ec5872bf41c2c44698fcf71266971c552d13feea19c3714e171bcd7a2b2c8_nofilter_compact.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "OSM tags filter with keep all tags",
     [
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--keep-all-tags",
         "--osm-tags-filter",
         '{"building": true, "highway": ["primary", "secondary"], "amenity": "bench"}',
     ],
-    "files/6e3ec5872bf41c2c44698fcf71266971c552d13feea19c3714e171bcd7a2b2c8_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_alltags_compact.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_alltags_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "OSM tags filter with keep all tags compact",
     [
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--keep-all-tags",
         "--osm-tags-filter",
         '{"building": true, "highway": ["primary", "secondary"], "amenity": "bench"}',
         "--compact",
     ],
-    "files/6e3ec5872bf41c2c44698fcf71266971c552d13feea19c3714e171bcd7a2b2c8_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_alltags_compact.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_alltags_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "OSM tags filter with keep all tags exploded",
     [
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--keep-all-tags",
         "--osm-tags-filter",
         '{"building": true, "highway": ["primary", "secondary"], "amenity": "bench"}',
         "--explode",
     ],
-    "files/6e3ec5872bf41c2c44698fcf71266971c552d13feea19c3714e171bcd7a2b2c8_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_alltags_exploded.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_alltags_exploded.geoparquet",
 )  # type: ignore
 @P.case(
     "OSM way polygon config",
     [
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--osm-way-polygon-config",
         osm_way_config_file_path(),
     ],
-    "files/6e3ec5872bf41c2c44698fcf71266971c552d13feea19c3714e171bcd7a2b2c8_nofilter_compact.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_compact.geoparquet",
 )  # type: ignore
 @P.case(
     "Allow not covered geometry",
     [
         "--geom-filter-wkt",
         (
             "POLYGON ((-43.064 29.673, -43.064 29.644, -43.017 29.644,"
```

### Comparing `quackosm-0.5.2/tests/base/test_osm_extracts.py` & `quackosm-0.5.3/tests/base/test_osm_extracts.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.2/tests/base/test_pbf_file_reader.py` & `quackosm-0.5.3/tests/base/test_pbf_file_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import geopandas as gpd
 import pandas as pd
 import pyogrio
 import pytest
 import six
 from parametrization import Parametrization as P
 from shapely import from_wkt, hausdorff_distance
-from shapely.geometry import MultiPolygon, Polygon, box
+from shapely.geometry import LinearRing, MultiPolygon, Polygon, box, polygon
 from shapely.geometry.base import BaseGeometry
 from shapely.ops import unary_union
 from srai.geometry import remove_interiors
 from srai.loaders.download import download_file
 from srai.loaders.osm_loaders.filters import GEOFABRIK_LAYERS, HEX2VEC_FILTER
 
 from quackosm._constants import FEATURES_INDEX
@@ -31,14 +31,15 @@
     GeocodeGeometryParser,
     GeohashGeometryParser,
     H3GeometryParser,
     S2GeometryParser,
 )
 from quackosm.osm_extracts import OsmExtractSource
 from quackosm.pbf_file_reader import PbfFileReader
+from tests.base.conftest import geometry_box
 
 ut = TestCase()
 LFS_DIRECTORY_URL = "https://github.com/kraina-ai/srai-test-files/raw/main/files/"
 
 
 @pytest.mark.parametrize(  # type: ignore
     "test_file_name,query,expected_result_length,expected_features_columns_length",
@@ -133,14 +134,39 @@
         file_paths=[Path(__file__).parent.parent / "test_files" / file_name],
         explode_tags=True,
         ignore_cache=True,
     )
     assert len(features_gdf) == 0
 
 
+@pytest.mark.parametrize(
+    "geometry",
+    [
+        geometry_box(),
+        from_wkt(
+            "POLYGON ((-43.064 29.673, -43.064 29.644, -43.017 29.644,"
+            " -43.017 29.673, -43.064 29.673))"
+        ),
+    ],
+)  # type: ignore
+def test_geometry_hash_calculation(geometry: BaseGeometry):
+    """Test if geometry hash is orientation-agnostic."""
+    if isinstance(geometry, Polygon):
+        oriented_a = polygon.orient(geometry, sign=1.0)
+        oriented_b = polygon.orient(geometry, sign=-1.0)
+    elif isinstance(geometry, LinearRing):
+        oriented_a = geometry
+        oriented_b = LinearRing(list(geometry.coords)[::-1])
+
+    assert (
+        PbfFileReader(geometry_filter=oriented_a)._get_oriented_geometry_filter()
+        == PbfFileReader(geometry_filter=oriented_b)._get_oriented_geometry_filter()
+    )
+
+
 def test_unique_osm_ids_duplicated_file():  # type: ignore
     """Test if function returns results without duplicated features."""
     monaco_file_path = Path(__file__).parent.parent / "test_files" / "monaco.osm.pbf"
     result_gdf = PbfFileReader().get_features_gdf(
         file_paths=[monaco_file_path, monaco_file_path], ignore_cache=True
     )
```

### Comparing `quackosm-0.5.2/tests/benchmark/test_big_file.py` & `quackosm-0.5.3/tests/benchmark/test_big_file.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.2/tests/optional_imports/test_optional_cli_dependency.py` & `quackosm-0.5.3/tests/optional_imports/test_optional_cli_dependency.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.2/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf` & `quackosm-0.5.3/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.2/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf` & `quackosm-0.5.3/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.2/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf` & `quackosm-0.5.3/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.2/tests/test_files/monaco.osm.pbf` & `quackosm-0.5.3/tests/test_files/monaco.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.2/tests/test_files/monaco_boundary.geojson` & `quackosm-0.5.3/tests/test_files/monaco_boundary.geojson`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.2/tests/test_files/osmconf.ini` & `quackosm-0.5.3/tests/test_files/osmconf.ini`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.2/PKG-INFO` & `quackosm-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuackOSM
-Version: 0.5.2
+Version: 0.5.3
 Summary: An open-source tool for reading OpenStreetMap PBF files using DuckDB
 Author-Email: Kamil Raczycki <kraczycki@kraina.ai>
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: GIS
```

