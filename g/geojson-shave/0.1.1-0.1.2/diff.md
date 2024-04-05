# Comparing `tmp/geojson-shave-0.1.1.tar.gz` & `tmp/geojson-shave-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geojson-shave-0.1.1.tar", last modified: Thu Apr  4 01:18:42 2024, max compression
+gzip compressed data, was "geojson-shave-0.1.2.tar", last modified: Fri Apr  5 06:13:31 2024, max compression
```

## Comparing `geojson-shave-0.1.1.tar` & `geojson-shave-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 01:18:41.423693 geojson-shave-0.1.1/
--rw-rw-rw-   0        0        0     1089 2024-04-04 00:47:11.000000 geojson-shave-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     3325 2024-04-04 01:18:42.184688 geojson-shave-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2457 2024-04-04 00:47:11.000000 geojson-shave-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 01:18:41.438691 geojson-shave-0.1.1/geojson_shave/
--rw-rw-rw-   0        0        0      132 2024-04-04 01:02:05.000000 geojson-shave-0.1.1/geojson_shave/__init__.py
--rw-rw-rw-   0        0        0     7746 2024-04-04 00:53:01.000000 geojson-shave-0.1.1/geojson_shave/geojson_shave.py
-drwxrwxrwx   0        0        0        0 2024-04-04 01:18:41.449692 geojson-shave-0.1.1/geojson_shave.egg-info/
--rw-rw-rw-   0        0        0     3325 2024-04-04 01:18:40.000000 geojson-shave-0.1.1/geojson_shave.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-04-04 01:18:41.000000 geojson-shave-0.1.1/geojson_shave.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 01:18:40.000000 geojson-shave-0.1.1/geojson_shave.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-04-04 01:18:40.000000 geojson-shave-0.1.1/geojson_shave.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       24 2024-04-04 01:18:40.000000 geojson-shave-0.1.1/geojson_shave.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-04 01:18:40.000000 geojson-shave-0.1.1/geojson_shave.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      932 2024-04-04 01:18:42.241687 geojson-shave-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0       73 2024-04-04 00:47:12.000000 geojson-shave-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 01:18:41.456692 geojson-shave-0.1.1/tests/
--rw-rw-rw-   0        0        0    20609 2024-04-04 00:47:12.000000 geojson-shave-0.1.1/tests/test_logic.py
+drwxr-xr-x   0 benjaminnour   (501) staff       (20)        0 2024-04-05 06:13:31.041443 geojson-shave-0.1.2/
+-rw-rw-r--   0 benjaminnour   (501) staff       (20)     1067 2024-03-29 06:27:46.000000 geojson-shave-0.1.2/LICENSE
+-rw-r--r--   0 benjaminnour   (501) staff       (20)     3232 2024-04-05 06:13:31.041370 geojson-shave-0.1.2/PKG-INFO
+-rw-r--r--   0 benjaminnour   (501) staff       (20)     2387 2024-04-04 11:18:14.000000 geojson-shave-0.1.2/README.md
+drwxr-xr-x   0 benjaminnour   (501) staff       (20)        0 2024-04-05 06:13:31.039349 geojson-shave-0.1.2/geojson_shave/
+-rw-r--r--   0 benjaminnour   (501) staff       (20)      127 2024-04-05 06:12:24.000000 geojson-shave-0.1.2/geojson_shave/__init__.py
+-rw-r--r--   0 benjaminnour   (501) staff       (20)     7521 2024-04-05 06:04:21.000000 geojson-shave-0.1.2/geojson_shave/geojson_shave.py
+drwxr-xr-x   0 benjaminnour   (501) staff       (20)        0 2024-04-05 06:13:31.041103 geojson-shave-0.1.2/geojson_shave.egg-info/
+-rw-r--r--   0 benjaminnour   (501) staff       (20)     3232 2024-04-05 06:13:30.000000 geojson-shave-0.1.2/geojson_shave.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminnour   (501) staff       (20)      337 2024-04-05 06:13:31.000000 geojson-shave-0.1.2/geojson_shave.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminnour   (501) staff       (20)        1 2024-04-05 06:13:30.000000 geojson-shave-0.1.2/geojson_shave.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminnour   (501) staff       (20)       67 2024-04-05 06:13:30.000000 geojson-shave-0.1.2/geojson_shave.egg-info/entry_points.txt
+-rw-r--r--   0 benjaminnour   (501) staff       (20)       24 2024-04-05 06:13:30.000000 geojson-shave-0.1.2/geojson_shave.egg-info/requires.txt
+-rw-r--r--   0 benjaminnour   (501) staff       (20)       14 2024-04-05 06:13:30.000000 geojson-shave-0.1.2/geojson_shave.egg-info/top_level.txt
+-rw-r--r--   0 benjaminnour   (501) staff       (20)      897 2024-04-05 06:13:31.041884 geojson-shave-0.1.2/setup.cfg
+-rw-r--r--   0 benjaminnour   (501) staff       (20)       69 2024-03-29 07:40:47.000000 geojson-shave-0.1.2/setup.py
+drwxr-xr-x   0 benjaminnour   (501) staff       (20)        0 2024-04-05 06:13:31.040616 geojson-shave-0.1.2/tests/
+-rw-rw-r--   0 benjaminnour   (501) staff       (20)    20054 2024-04-05 05:51:22.000000 geojson-shave-0.1.2/tests/test_logic.py
```

### Comparing `geojson-shave-0.1.1/PKG-INFO` & `geojson-shave-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-Metadata-Version: 2.1
-Name: geojson-shave
-Version: 0.1.1
-Summary: A command-line tool for reducing the size of GeoJSON files.
-Home-page: https://github.com/ben-n93/geojson-shave
-Author: Ben Nour
-Author-email: hello@ben-nour.com
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: alive-progress
-Requires-Dist: humanize
-
-
-<p align="center">
-    <a href="https://pypi.python.org">
-        <img src="https://ben-nour.com/images/geojson-shave.png" alt="GeoJSON-shave" style="width: 60%; height: auto;"/>
-    </a>
-</p>
-
-<p align="center">
-     <a href="https://github.com/ben-n93/geojson-shave/actions/workflows/tests.yml"><img src="https://github.com/ben-n93/geojson-shave/actions/workflows/tests.yml/badge.svg"                 alt="Testing"></a>
-     <a href="https://github.com/ben-n93/geojson-shave/blob/main/LICENSE"><img src="https://img.shields.io/pypi/l/geojson-shave" alt="License"></a>
-    <a href="https://codecov.io/gh/ben-n93/geojson-shave" ><img src="https://codecov.io/gh/ben-n93/geojson-shave/graph/badge.svg?token=XUMK0D4J9X"/></a>
-    <a href="https://pypi.org/project/geojson-shave/"><img src="https://img.shields.io/pypi/pyversions/geojson-shave" alt="versions"></a>
-</p>
-
----
-
-geojson-shave reduces the size of GeoJSON files by:
-
-- Truncating latitude/longitude coordinates to the specified decimal places.
-- Eliminating unnecessary whitespace.
-- (Optionally) replacing the properties key's value with null/empty dictionary.
-
-This tool assumes that your GeoJSON file confirms to the [RFC 7946](https://datatracker.ietf.org/doc/html/rfc7946).
-
-## Installation
-```
-$ pip install geojson-shave
-```
-
-## Usage
-
-<p align="center">
-    <a href="https://pypi.python.org">
-        <img src="https://ben-nour.com/images/demo.gif" alt="GeoJSON-shave-demo">
-    </a>
-</p>
-
-Simply pass the file path of your GeoJSON file and it will truncuate the coordinates to 5 decimal places, outputing to the current working directory:
-
-```
-$ geojson-shave roads.geoson
-```
-
-Alterntatively you can specify the number of decimal points you want the coordiantes truncuated to:
-
-```
-$ geojson-shave roads.geojson -d 3
-```
-
-You can also specify if you only want certain Geometry object types in the file to be processed:
-```
-$ geojson-shave roads.geojson -g LineString Polygon
-```
-
-Note that the -g option doesn't apply to objects nested within Geometry Collection.
-
-And to reduce the file size even further you can nullify the property value of Feature objects:
-
-```
-$ geojson-shave roads.geojson -p
-```
-
-Output to a directory other than the current working directory:
-```
-$ geojson-shave roads.geojson -o ../data/output.geojson
-```
-
-## TODO
-
-- [ ] Add support for passing the URL of a hosted GeoJSON file to the tool.
+Metadata-Version: 2.1
+Name: geojson-shave
+Version: 0.1.2
+Summary: A command-line tool for reducing the size of GeoJSON files.
+Home-page: https://github.com/ben-n93/geojson-shave
+Author: Ben Nour
+Author-email: hello@ben-nour.com
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Environment :: Console
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: alive-progress
+Requires-Dist: humanize
+
+
+<p align="center">
+    <a href="https://pypi.python.org">
+        <img src="https://ben-nour.com/images/geojson-shave.png" alt="GeoJSON-shave" style="width: 60%; height: auto;"/>
+    </a>
+</p>
+
+<p align="center">
+     <a href="https://github.com/ben-n93/geojson-shave/actions/workflows/tests.yml"><img src="https://github.com/ben-n93/geojson-shave/actions/workflows/tests.yml/badge.svg"                 alt="Testing"></a>
+     <a href="https://github.com/ben-n93/geojson-shave/blob/main/LICENSE"><img src="https://img.shields.io/pypi/l/geojson-shave" alt="License"></a>
+    <a href="https://codecov.io/gh/ben-n93/geojson-shave" ><img src="https://codecov.io/gh/ben-n93/geojson-shave/graph/badge.svg?token=XUMK0D4J9X"/></a>
+    <a href="https://pypi.org/project/geojson-shave/"><img src="https://img.shields.io/pypi/pyversions/geojson-shave" alt="versions"></a>
+</p>
+
+---
+
+geojson-shave reduces the size of GeoJSON files by:
+
+- Truncating latitude/longitude coordinates to the specified decimal places.
+- Eliminating unnecessary whitespace.
+- (Optionally) replacing the properties key's value with null/empty dictionary.
+
+This tool assumes that your GeoJSON file confirms to the [RFC 7946](https://datatracker.ietf.org/doc/html/rfc7946).
+
+## Installation
+```
+$ pip install geojson-shave
+```
+
+## Usage
+
+<p align="center">
+    <a href="https://pypi.python.org">
+        <img src="https://ben-nour.com/images/demo.gif" alt="GeoJSON-shave-demo">
+    </a>
+</p>
+
+Simply pass the file path of your GeoJSON file and it will truncuate the coordinates to 5 decimal places, outputing to the current working directory:
+
+```
+$ geojson-shave roads.geoson
+```
+
+Alterntatively you can specify the number of decimal points you want the coordiantes truncuated to:
+
+```
+$ geojson-shave roads.geojson -d 3
+```
+
+You can also specify if you only want certain Geometry object types in the file to be processed:
+```
+$ geojson-shave roads.geojson -g LineString Polygon
+```
+
+Note that the -g option doesn't apply to objects nested within Geometry Collection.
+
+And to reduce the file size even further you can nullify the property value of Feature objects:
+
+```
+$ geojson-shave roads.geojson -p
+```
+
+Output to a directory other than the current working directory:
+```
+$ geojson-shave roads.geojson -o ../data/output.geojson
+```
+
+## TODO
+
+- [ ] Add support for passing the URL of a hosted GeoJSON file to the tool.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: geojson-shave Version: 0.1.1 Summary: A command-
+Metadata-Version: 2.1 Name: geojson-shave Version: 0.1.2 Summary: A command-
 line tool for reducing the size of GeoJSON files. Home-page: https://
 github.com/ben-n93/geojson-shave Author: Ben Nour Author-email: hello@ben-
 nour.com License: MIT Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Environment :: Console Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

### Comparing `geojson-shave-0.1.1/geojson_shave/geojson_shave.py` & `geojson-shave-0.1.2/geojson_shave/geojson_shave.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,219 +1,219 @@
-"""A command-line tool that reduces the size of GeoJSON files.
-"""
-
-import argparse
-import json
-import pathlib
-
-from alive_progress import alive_bar
-import humanize
-
-GEOMETRY_OBJECTS = {
-    "Point",
-    "MultiPoint",
-    "LineString",
-    "MultiLineString",
-    "Polygon",
-    "MultiPolygon",
-    "GeometryCollection",
-}
-
-
-def get_parser():
-    """Create the command-line interface."""
-    parser = argparse.ArgumentParser(
-        description="""Reduces the size of a GeoJSON file by lowering the
-        decimal point precision of the file's latitude/language 
-        coordinates.""",
-        epilog="""
-        EXAMPLES
-        --------
-        Truncuate a GeoJSON's file to 3 decimal points:
-            geojson_shave roads.geojson -d 3
-
-        Only truncuate the coordinates of LineString and Polygon objects:
-            geojson_shave roads.geojson -g LineString Polygon
-
-        Replace the properties value with a null value:
-            geojson_shave roads.geojson -p
-        """,
-        formatter_class=argparse.RawTextHelpFormatter,
-    )
-
-    parser.add_argument(
-        "input",
-        type=argparse.FileType("r"),
-        help="Input GeoJSON file to pass to the tool.",
-    )
-
-    parser.add_argument(
-        "-o",
-        "--output",
-        type=argparse.FileType("w"),
-        help="""Name and path of the output GeoJSON file. Default path is the
-        current working directory.""",
-        default=pathlib.Path.cwd() / "output.geojson",
-        required=False,
-    )
-
-    parser.add_argument(
-        "-d",
-        "--decimal_points",
-        type=int,
-        help="Number of decimal points to keep when \
-                            truncating coordinates. Default is 5.",
-        required=False,
-        default=5,
-    )
-
-    parser.add_argument(
-        "-p",
-        "--properties",
-        help="Overwrite the properties with a null value.",
-        required=False,
-        action="store_true",
-    )
-
-    parser.add_argument(
-        "-g",
-        "--geometry_object",
-        type=str,
-        help="""The types of Geometry Object to be processed.
-        Default is all objects.""",
-        required=False,
-        default=GEOMETRY_OBJECTS,
-        choices=GEOMETRY_OBJECTS,
-        metavar="GEOMETRY_OBJECT",
-        nargs="+",
-    )
-
-    return parser
-
-
-def _create_coordinates(coordinates, precision):
-    """Create truncuated coordinates."""
-    new_coordinates = []
-    for item in coordinates:
-        if isinstance(item, list):
-            new_coordinates.append(_create_coordinates(item, precision))
-        else:
-            item = round(item, precision)
-            new_coordinates.append(float(item))
-    return new_coordinates
-
-
-def _process_geometry_collection(geometry_collection, precision):
-    """Parse and truncuate the coordinates of each geometry
-    object nested within a geometry collection."""
-    new_geometry_collection = {"type": "GeometryCollection"}
-    processed_geometry_objects = []
-    for geometry_object in geometry_collection["geometries"]:
-        object_type = geometry_object["type"]
-        new_coordinates = _create_coordinates(geometry_object["coordinates"], precision)
-        processed_geometry_objects.append(
-            {"type": object_type, "coordinates": new_coordinates}
-        )
-
-    new_geometry_collection["geometries"] = processed_geometry_objects
-    return new_geometry_collection
-
-
-def _process_features(geojson, precision, geometry_to_include, nullify_property):
-    """Process Feature objects, truncuating coordinates and/or replacing
-    the properties member with a blank value."""
-    # Create new GeoJSON object.
-    if (total_features := geojson.get("features")) is None:
-        if geojson.get("type") == "Feature":
-            output_geojson = {"type": "Feature"}
-            length = 1
-        else:
-            raise SystemError("Error: there are no Feature objects in this file.")
-    else:
-        output_geojson = {"type": "FeatureCollection", "features": []}
-        length = len(total_features)
-
-    # Process Feature objects.
-    with alive_bar(length) as progress_bar:
-        progress_bar.title("Processing the input file:")
-        if geojson["type"] == "FeatureCollection":
-            for index, feature in enumerate(geojson["features"]):
-                output_geojson["features"].append(feature)
-                if nullify_property:
-                    output_geojson["features"][index]["properties"] = {}
-                try:
-                    if (geo_type := feature["geometry"]["type"]) in geometry_to_include:
-                        if geo_type == "GeometryCollection":
-                            output_geojson["features"][index]["geometry"] = (
-                                _process_geometry_collection(
-                                    feature["geometry"], precision
-                                )
-                            )
-                        else:
-                            new_coordinates = _create_coordinates(
-                                feature["geometry"]["coordinates"], precision
-                            )
-                            output_geojson["features"][index]["geometry"][
-                                "coordinates"
-                            ] = new_coordinates
-                except TypeError:  # Feature's "geometry" member has a null value.
-                    progress_bar()
-                    continue
-                progress_bar()
-
-        else:  # Only one Feature.
-            if geojson["geometry"]["type"] in geometry_to_include:
-                new_coordinates = _create_coordinates(
-                    geojson["geometry"]["coordinates"], precision
-                )
-                output_geojson["geometry"] = {
-                    "type": geojson["geometry"]["type"],
-                    "coordinates": new_coordinates,
-                }
-                if nullify_property:
-                    output_geojson["properties"] = {}
-                progress_bar()
-
-    # Including any non-standard (RFC) top-level keys in the output file.
-    for key in geojson.keys():
-        if key not in ("type", "features", "geometry"):
-            output_geojson[key] = geojson[key]
-    return output_geojson
-
-
-def main():
-    """Launch the command-line tool."""
-    parser = get_parser()
-    args = parser.parse_args()
-
-    if args.decimal_points < 0:
-        raise ValueError(
-            """Please only pass a positive number to the
-        decimal argument."""
-        )
-
-    # Process input file.
-    with open(args.input.name, "r") as input_file:
-        try:
-            input_geojson = json.load(input_file)
-        except json.decoder.JSONDecodeError as e:
-            raise SystemError("Error: please provide a valid GeoJSON file.") from e
-    output_geojson = _process_features(
-        input_geojson, args.decimal_points, args.geometry_object, args.properties
-    )
-
-    # Write to output file.
-    with open(args.output.name, "w", encoding="utf-8") as output_file:
-        print("Writing to output file...")
-        json.dump(output_geojson, output_file, separators=(",", ":"))
-
-    # Exit message to user.
-    size_before = pathlib.Path(args.input.name).stat().st_size
-    size_after = pathlib.Path(args.output.name).stat().st_size
-    difference = round(((size_before - size_after) / size_before) * 100)
-    print(f"Input file size: {humanize.naturalsize(size_before)}.")
-    print(f"Output file size: {humanize.naturalsize(size_after)}.")
-    print(f"File size reduction: {difference}%")
-
-
-if __name__ == "__main__":
-    main()
+"""A command-line tool that reduces the size of GeoJSON files.
+"""
+
+import argparse
+from contextlib import suppress
+import json
+import pathlib
+
+from alive_progress import alive_bar
+import humanize
+
+GEOMETRY_OBJECTS = {
+    "Point",
+    "MultiPoint",
+    "LineString",
+    "MultiLineString",
+    "Polygon",
+    "MultiPolygon",
+    "GeometryCollection",
+}
+
+
+def get_parser():
+    """Create the command-line interface."""
+    parser = argparse.ArgumentParser(
+        description="""Reduces the size of a GeoJSON file by lowering the
+        decimal point precision of the file's latitude/language 
+        coordinates.""",
+        epilog="""
+        EXAMPLES
+        --------
+        Truncuate a GeoJSON's file to 3 decimal points:
+            geojson_shave roads.geojson -d 3
+
+        Only truncuate the coordinates of LineString and Polygon objects:
+            geojson_shave roads.geojson -g LineString Polygon
+
+        Replace the properties value with a null value:
+            geojson_shave roads.geojson -p
+        """,
+        formatter_class=argparse.RawTextHelpFormatter,
+    )
+
+    parser.add_argument(
+        "input",
+        type=argparse.FileType("r"),
+        help="Input GeoJSON file to pass to the tool.",
+    )
+
+    parser.add_argument(
+        "-o",
+        "--output",
+        type=argparse.FileType("w"),
+        help="""Name and path of the output GeoJSON file. Default path is the
+        current working directory.""",
+        default=pathlib.Path.cwd() / "output.geojson",
+        required=False,
+    )
+
+    parser.add_argument(
+        "-d",
+        "--decimal_points",
+        type=int,
+        help="Number of decimal points to keep when \
+                            truncating coordinates. Default is 5.",
+        required=False,
+        default=5,
+    )
+
+    parser.add_argument(
+        "-p",
+        "--properties",
+        help="Overwrite the properties with a null value.",
+        required=False,
+        action="store_true",
+    )
+
+    parser.add_argument(
+        "-g",
+        "--geometry_object",
+        type=str,
+        help="""The types of Geometry Object to be processed.
+        Default is all objects.""",
+        required=False,
+        default=GEOMETRY_OBJECTS,
+        choices=GEOMETRY_OBJECTS,
+        metavar="GEOMETRY_OBJECT",
+        nargs="+",
+    )
+
+    return parser
+
+
+def _create_coordinates(coordinates, precision):
+    """Create truncuated coordinates."""
+    new_coordinates = []
+    for item in coordinates:
+        if isinstance(item, list):
+            new_coordinates.append(_create_coordinates(item, precision))
+        else:
+            item = round(item, precision)
+            new_coordinates.append(float(item))
+    return new_coordinates
+
+
+def _process_geometry_collection(geometry_collection, precision):
+    """Parse and truncuate the coordinates of each geometry
+    object nested within a geometry collection."""
+    new_geometry_collection = {"type": "GeometryCollection"}
+    processed_geometry_objects = []
+    for geometry_object in geometry_collection["geometries"]:
+        object_type = geometry_object["type"]
+        new_coordinates = _create_coordinates(geometry_object["coordinates"], precision)
+        processed_geometry_objects.append(
+            {"type": object_type, "coordinates": new_coordinates}
+        )
+
+    new_geometry_collection["geometries"] = processed_geometry_objects
+    return new_geometry_collection
+
+
+def _process_features(geojson, precision, geometry_to_include, nullify_property):
+    """Process Feature objects, truncuating coordinates and/or replacing
+    the properties member with a blank value."""
+    # Create new GeoJSON object.
+    if (total_features := geojson.get("features")) is None:
+        if geojson.get("type") == "Feature":
+            output_geojson = {"type": "Feature"}
+            length = 1
+        else:
+            raise RuntimeError("Error: there are no Feature objects in this file.")
+    else:
+        output_geojson = {"type": "FeatureCollection", "features": []}
+        length = len(total_features)
+
+    # Process Feature objects.
+    with alive_bar(length) as progress_bar:
+        progress_bar.title("Processing the input file:")
+        if geojson["type"] == "FeatureCollection":
+            for index, feature in enumerate(geojson["features"]):
+                output_geojson["features"].append(feature)
+                if nullify_property:
+                    output_geojson["features"][index]["properties"] = {}
+                with suppress(
+                    TypeError
+                ):  # Feature's "geometry" member has a null value.
+                    if (geo_type := feature["geometry"]["type"]) in geometry_to_include:
+                        if geo_type == "GeometryCollection":
+                            output_geojson["features"][index]["geometry"] = (
+                                _process_geometry_collection(
+                                    feature["geometry"], precision
+                                )
+                            )
+                        else:
+                            new_coordinates = _create_coordinates(
+                                feature["geometry"]["coordinates"], precision
+                            )
+                            output_geojson["features"][index]["geometry"][
+                                "coordinates"
+                            ] = new_coordinates
+                progress_bar()
+
+        else:  # Only one Feature.
+            if geojson["geometry"]["type"] in geometry_to_include:
+                new_coordinates = _create_coordinates(
+                    geojson["geometry"]["coordinates"], precision
+                )
+                output_geojson["geometry"] = {
+                    "type": geojson["geometry"]["type"],
+                    "coordinates": new_coordinates,
+                }
+                if nullify_property:
+                    output_geojson["properties"] = {}
+                progress_bar()
+
+    # Including any non-standard (RFC) top-level keys in the output file.
+    for key in geojson.keys():
+        if key not in ("type", "features", "geometry"):
+            output_geojson[key] = geojson[key]
+    return output_geojson
+
+
+def main():
+    """Launch the command-line tool."""
+    parser = get_parser()
+    args = parser.parse_args()
+
+    if args.decimal_points < 0:
+        raise ValueError(
+            """Please only pass a positive number to the
+        decimal argument."""
+        )
+
+    # Process input file.
+    with open(args.input.name, "r") as input_file:
+        try:
+            input_geojson = json.load(input_file)
+        except json.decoder.JSONDecodeError as e:
+            raise SystemError("Error: please provide a valid GeoJSON file.") from e
+    output_geojson = _process_features(
+        input_geojson, args.decimal_points, args.geometry_object, args.properties
+    )
+
+    # Write to output file.
+    with open(args.output.name, "w", encoding="utf-8") as output_file:
+        print("Writing to output file...")
+        json.dump(output_geojson, output_file, separators=(",", ":"))
+
+    # Exit message to user.
+    size_before = pathlib.Path(args.input.name).stat().st_size
+    size_after = pathlib.Path(args.output.name).stat().st_size
+    difference = round(((size_before - size_after) / size_before) * 100)
+    print(f"Input file size: {humanize.naturalsize(size_before)}.")
+    print(f"Output file size: {humanize.naturalsize(size_after)}.")
+    print(f"File size reduction: {difference}%")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `geojson-shave-0.1.1/geojson_shave.egg-info/PKG-INFO` & `geojson-shave-0.1.2/geojson_shave.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-Metadata-Version: 2.1
-Name: geojson-shave
-Version: 0.1.1
-Summary: A command-line tool for reducing the size of GeoJSON files.
-Home-page: https://github.com/ben-n93/geojson-shave
-Author: Ben Nour
-Author-email: hello@ben-nour.com
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: alive-progress
-Requires-Dist: humanize
-
-
-<p align="center">
-    <a href="https://pypi.python.org">
-        <img src="https://ben-nour.com/images/geojson-shave.png" alt="GeoJSON-shave" style="width: 60%; height: auto;"/>
-    </a>
-</p>
-
-<p align="center">
-     <a href="https://github.com/ben-n93/geojson-shave/actions/workflows/tests.yml"><img src="https://github.com/ben-n93/geojson-shave/actions/workflows/tests.yml/badge.svg"                 alt="Testing"></a>
-     <a href="https://github.com/ben-n93/geojson-shave/blob/main/LICENSE"><img src="https://img.shields.io/pypi/l/geojson-shave" alt="License"></a>
-    <a href="https://codecov.io/gh/ben-n93/geojson-shave" ><img src="https://codecov.io/gh/ben-n93/geojson-shave/graph/badge.svg?token=XUMK0D4J9X"/></a>
-    <a href="https://pypi.org/project/geojson-shave/"><img src="https://img.shields.io/pypi/pyversions/geojson-shave" alt="versions"></a>
-</p>
-
----
-
-geojson-shave reduces the size of GeoJSON files by:
-
-- Truncating latitude/longitude coordinates to the specified decimal places.
-- Eliminating unnecessary whitespace.
-- (Optionally) replacing the properties key's value with null/empty dictionary.
-
-This tool assumes that your GeoJSON file confirms to the [RFC 7946](https://datatracker.ietf.org/doc/html/rfc7946).
-
-## Installation
-```
-$ pip install geojson-shave
-```
-
-## Usage
-
-<p align="center">
-    <a href="https://pypi.python.org">
-        <img src="https://ben-nour.com/images/demo.gif" alt="GeoJSON-shave-demo">
-    </a>
-</p>
-
-Simply pass the file path of your GeoJSON file and it will truncuate the coordinates to 5 decimal places, outputing to the current working directory:
-
-```
-$ geojson-shave roads.geoson
-```
-
-Alterntatively you can specify the number of decimal points you want the coordiantes truncuated to:
-
-```
-$ geojson-shave roads.geojson -d 3
-```
-
-You can also specify if you only want certain Geometry object types in the file to be processed:
-```
-$ geojson-shave roads.geojson -g LineString Polygon
-```
-
-Note that the -g option doesn't apply to objects nested within Geometry Collection.
-
-And to reduce the file size even further you can nullify the property value of Feature objects:
-
-```
-$ geojson-shave roads.geojson -p
-```
-
-Output to a directory other than the current working directory:
-```
-$ geojson-shave roads.geojson -o ../data/output.geojson
-```
-
-## TODO
-
-- [ ] Add support for passing the URL of a hosted GeoJSON file to the tool.
+Metadata-Version: 2.1
+Name: geojson-shave
+Version: 0.1.2
+Summary: A command-line tool for reducing the size of GeoJSON files.
+Home-page: https://github.com/ben-n93/geojson-shave
+Author: Ben Nour
+Author-email: hello@ben-nour.com
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Environment :: Console
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: alive-progress
+Requires-Dist: humanize
+
+
+<p align="center">
+    <a href="https://pypi.python.org">
+        <img src="https://ben-nour.com/images/geojson-shave.png" alt="GeoJSON-shave" style="width: 60%; height: auto;"/>
+    </a>
+</p>
+
+<p align="center">
+     <a href="https://github.com/ben-n93/geojson-shave/actions/workflows/tests.yml"><img src="https://github.com/ben-n93/geojson-shave/actions/workflows/tests.yml/badge.svg"                 alt="Testing"></a>
+     <a href="https://github.com/ben-n93/geojson-shave/blob/main/LICENSE"><img src="https://img.shields.io/pypi/l/geojson-shave" alt="License"></a>
+    <a href="https://codecov.io/gh/ben-n93/geojson-shave" ><img src="https://codecov.io/gh/ben-n93/geojson-shave/graph/badge.svg?token=XUMK0D4J9X"/></a>
+    <a href="https://pypi.org/project/geojson-shave/"><img src="https://img.shields.io/pypi/pyversions/geojson-shave" alt="versions"></a>
+</p>
+
+---
+
+geojson-shave reduces the size of GeoJSON files by:
+
+- Truncating latitude/longitude coordinates to the specified decimal places.
+- Eliminating unnecessary whitespace.
+- (Optionally) replacing the properties key's value with null/empty dictionary.
+
+This tool assumes that your GeoJSON file confirms to the [RFC 7946](https://datatracker.ietf.org/doc/html/rfc7946).
+
+## Installation
+```
+$ pip install geojson-shave
+```
+
+## Usage
+
+<p align="center">
+    <a href="https://pypi.python.org">
+        <img src="https://ben-nour.com/images/demo.gif" alt="GeoJSON-shave-demo">
+    </a>
+</p>
+
+Simply pass the file path of your GeoJSON file and it will truncuate the coordinates to 5 decimal places, outputing to the current working directory:
+
+```
+$ geojson-shave roads.geoson
+```
+
+Alterntatively you can specify the number of decimal points you want the coordiantes truncuated to:
+
+```
+$ geojson-shave roads.geojson -d 3
+```
+
+You can also specify if you only want certain Geometry object types in the file to be processed:
+```
+$ geojson-shave roads.geojson -g LineString Polygon
+```
+
+Note that the -g option doesn't apply to objects nested within Geometry Collection.
+
+And to reduce the file size even further you can nullify the property value of Feature objects:
+
+```
+$ geojson-shave roads.geojson -p
+```
+
+Output to a directory other than the current working directory:
+```
+$ geojson-shave roads.geojson -o ../data/output.geojson
+```
+
+## TODO
+
+- [ ] Add support for passing the URL of a hosted GeoJSON file to the tool.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: geojson-shave Version: 0.1.1 Summary: A command-
+Metadata-Version: 2.1 Name: geojson-shave Version: 0.1.2 Summary: A command-
 line tool for reducing the size of GeoJSON files. Home-page: https://
 github.com/ben-n93/geojson-shave Author: Ben Nour Author-email: hello@ben-
 nour.com License: MIT Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Environment :: Console Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

### Comparing `geojson-shave-0.1.1/tests/test_logic.py` & `geojson-shave-0.1.2/tests/test_logic.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,573 +1,575 @@
-"""Unit tests for geojson_shave.py"""
-
-import os
-import unittest
-import sys
-
-from geojson_shave.geojson_shave import (_create_coordinates,
- _process_geometry_collection,
-_process_features, 
-GEOMETRY_OBJECTS)
-
-
-class TestCreateCoordinates(unittest.TestCase):
-    """Tests for the _create_coordinates function.
-
-    Note that both LineStrings' and MultiPoints' coordinates both consist
-    of an array of Points, hence only the LineString being tested.
-    """
-
-    def setUp(self):
-        self.point = {
-            "type": "Point",
-            "coordinates": [-100.123456, 200.123456],
-            "properties": {"name": "Test Point"},
-        }
-
-        self.linestring = {
-            "type": "LineString",
-            "coordinates": [
-                [100.123456, 0.123456],
-                [101.123456, 1.123456],
-                [102.123456, 2.123456],
-            ],
-        }
-
-        self.multilinestring = {
-            "type": "MultiLineString",
-            "coordinates": [
-                [[-100.123456, 0.123456], [-101.123456, 1.123456]],
-                [[102.123456, 2.123456], [103.123456, 3.123456]],
-            ],
-        }
-
-        self.polygon = {
-            "type": "Polygon",
-            "coordinates": [
-                [
-                    [100.123456, 0.123456],
-                    [101.123456, 0.123456],
-                    [101.123456, 1.123456],
-                    [100.123456, 1.123456],
-                    [100.123456, 0.123456],
-                ]
-            ],
-        }
-
-        self.multipolygon = {
-            "type": "MultiPolygon",
-            "coordinates": [
-                [
-                    [
-                        [102.123456, 2.123456],
-                        [103.123456, 2.123456],
-                        [103.123456, 3.123456],
-                        [102.123456, 3.123456],
-                        [102.123456, 2.123456],
-                    ]
-                ],
-                [
-                    [
-                        [100.123456, 0.123456],
-                        [101.123456, 0.123456],
-                        [101.123456, 1.123456],
-                        [100.123456, 1.123456],
-                        [100.123456, 0.123456],
-                    ],
-                    [
-                        [100.123456, 0.123456],
-                        [100.123456, 0.123456],
-                        [100.123456, 0.123456],
-                        [100.123456, 0.123456],
-                        [100.123456, 0.123456],
-                    ],
-                ],
-            ],
-        }
-
-    # Point.
-    def test_truncuating_point_coordinates(self):
-        """Test that Point coordinates are truncuated succesfully."""
-        expected_return_value = [-100.123, 200.123]
-        precision = 3
-        geometry_coordinates = self.point["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    def test_point_same_precision(self):
-        """Test that Point coordinates are not truncuated when
-        the coordinate decimal points matches what's passed
-        to the precision parameter.
-        """
-        expected_return_value = self.point["coordinates"]
-        precision = 6
-        geometry_coordinates = self.point["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    def test_point_precision_larger_than_places(self):
-        """Test that when the precision argument is a value larger
-        than the number of coordinate decimnal points, the same coordinate values
-        are returned.
-        """
-        expected_return_value = self.point["coordinates"]
-        precision = 50
-        geometry_coordinates = self.point["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    # LineString.
-    def test_truncuating_linestring_coordinates(self):
-        """Test that LineString coordinates are truncuated succesfully."""
-        expected_return_value = [
-            [100.123, 0.123],
-            [101.123, 1.123],
-            [102.123, 2.123],
-        ]
-        precision = 3
-        geometry_coordinates = self.linestring["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    def test_linestring_same_precision(self):
-        """Test that LineString coordinates are not truncuated when
-        the coordinate decimal points matches what's passed
-        to the precision parameter.
-        """
-        expected_return_value = self.linestring["coordinates"]
-        precision = 6
-        geometry_coordinates = self.linestring["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    def test_linestring_precision_larger_than_places(self):
-        """Test that when the precision argument is a value larger
-        than the number of coordinate decimnal points, the same coordinate values
-        are returned.
-        """
-        expected_return_value = self.linestring["coordinates"]
-        precision = 50
-        geometry_coordinates = self.linestring["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    # MultiLine strings.
-    def test_truncuating_multilinestring_coordinates(self):
-        """Test that MultiLineString coordinates are truncuated succesfully."""
-        expected_return_value = [
-            [[-100.123, 0.123], [-101.123, 1.123]],
-            [[102.123, 2.123], [103.123, 3.123]],
-        ]
-        precision = 3
-        geometry_coordinates = self.multilinestring["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    def test_multilinestring_precision_larger_than_places(self):
-        """Test that when the precision argument is a value larger
-        than the number of coordinate decimnal points, the same coordinate values
-        are returned.
-        """
-        expected_return_value = self.multilinestring["coordinates"]
-        precision = 50
-        geometry_coordinates = self.multilinestring["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    def test_multilinestring_same_precision(self):
-        """Test that LineString coordinates are not truncuated when
-        the coordinate decimal points matches what's passed
-        to the precision parameter.
-        """
-        expected_return_value = self.multipolygon["coordinates"]
-        precision = 6
-        geometry_coordinates = self.multipolygon["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    # Polygon.
-    def test_truncuating_polygon_coordinates(self):
-        """Test that Polygon coordinates are truncuated succesfully."""
-        expected_return_value = [
-            [
-                [100.123, 0.123],
-                [101.123, 0.123],
-                [101.123, 1.123],
-                [100.123, 1.123],
-                [100.123, 0.123],
-            ]
-        ]
-        precision = 3
-        geometry_coordinates = self.polygon["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    def test_polygon_precision_larger_than_places(self):
-        """Test that when the precision argument is a value larger
-        than the number of coordinate decimnal points, the same coordinate values
-        are returned.
-        """
-        expected_return_value = [
-            [
-                [100.123456, 0.123456],
-                [101.123456, 0.123456],
-                [101.123456, 1.123456],
-                [100.123456, 1.123456],
-                [100.123456, 0.123456],
-            ]
-        ]
-        precision = 50
-        geometry_coordinates = self.polygon["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    def test_polygon_same_precision(self):
-        """Test that LineString coordinates are not truncuated when
-        the coordinate decimal points matches what's passed
-        to the precision parameter.
-        """
-        expected_return_value = [
-            [
-                [100.123456, 0.123456],
-                [101.123456, 0.123456],
-                [101.123456, 1.123456],
-                [100.123456, 1.123456],
-                [100.123456, 0.123456],
-            ]
-        ]
-        precision = 6
-        geometry_coordinates = self.polygon["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    # MultiPolygon.
-    def test_truncuating_multipolygon_coordinates(self):
-        """Test that MultiPolygon coordinates are truncuated succesfully."""
-        expected_return_value = [
-            [
-                [
-                    [102.123, 2.123],
-                    [103.123, 2.123],
-                    [103.123, 3.123],
-                    [102.123, 3.123],
-                    [102.123, 2.123],
-                ]
-            ],
-            [
-                [
-                    [100.123, 0.123],
-                    [101.123, 0.123],
-                    [101.123, 1.123],
-                    [100.123, 1.123],
-                    [100.123, 0.123],
-                ],
-                [
-                    [100.123, 0.123],
-                    [100.123, 0.123],
-                    [100.123, 0.123],
-                    [100.123, 0.123],
-                    [100.123, 0.123],
-                ],
-            ],
-        ]
-        precision = 3
-        geometry_coordinates = self.multipolygon["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    def test_multipolygon_precision_larger_than_places(self):
-        """Test that when the precision argument is a value larger
-        than the number of coordinate decimnal points, the same coordinate values
-        are returned.
-        """
-        expected_return_value = self.multipolygon["coordinates"]
-        precision = 50
-        geometry_coordinates = self.multipolygon["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    def test_multipolygon_same_precision(self):
-        """Test that LineString coordinates are not truncuated when
-        the coordinate decimal points matches what's passed
-        to the precision parameter.
-        """
-        expected_return_value = self.multipolygon["coordinates"]
-        precision = 6
-        geometry_coordinates = self.multipolygon["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-
-class TestProcessGeometryCollection(unittest.TestCase):
-    """Tests for the _process_geometry_collection function."""
-
-    def setUp(self):
-        self.geometry_collection = {
-            "type": "GeometryCollection",
-            "geometries": [
-                {"type": "Point", "coordinates": [0.123456, 0.123456]},
-                {
-                    "type": "LineString",
-                    "coordinates": [
-                        [1.123456, 1.123456],
-                        [2.123456, 3.123456],
-                        [4.123456, 5.123456],
-                    ],
-                },
-                {
-                    "type": "Polygon",
-                    "coordinates": [
-                        [
-                            [6.123456, 6.123456],
-                            [8.123456, 8.123456],
-                            [10.123456, 10.123456],
-                            [6.123456, 6.123456],
-                        ]
-                    ],
-                },
-                {
-                    "type": "MultiPoint",
-                    "coordinates": [
-                        [12.123456, 12.123456],
-                        [14.123456, 14.123456],
-                        [16.123456, 16.123456],
-                    ],
-                },
-            ],
-        }
-
-    def test_truncuating_coordinates(self):
-        """Tests that the coordinates of each nested Geometry object
-        is truncuated correctly."""
-
-        expected_return_value = {
-            "type": "GeometryCollection",
-            "geometries": [
-                {"type": "Point", "coordinates": [0.123, 0.123]},
-                {
-                    "type": "LineString",
-                    "coordinates": [[1.123, 1.123], [2.123, 3.123], [4.123, 5.123]],
-                },
-                {
-                    "type": "Polygon",
-                    "coordinates": [
-                        [
-                            [6.123, 6.123],
-                            [8.123, 8.123],
-                            [10.123, 10.123],
-                            [6.123, 6.123],
-                        ]
-                    ],
-                },
-                {
-                    "type": "MultiPoint",
-                    "coordinates": [
-                        [12.123, 12.123],
-                        [14.123, 14.123],
-                        [16.123, 16.123],
-                    ],
-                },
-            ],
-        }
-
-        geo_collection = self.geometry_collection
-        precision = 3
-        self.assertEqual(
-            _process_geometry_collection(geo_collection, precision),
-            expected_return_value,
-        )
-
-
-class TestProcessFeatures(unittest.TestCase):
-    """Tests for the _process_features function."""
-
-    def setUp(self):
-        self.feature_collection = {
-            "type": "FeatureCollection",
-            "features": [
-                {
-                    "type": "Feature",
-                    "geometry": {"type": "Point", "coordinates": [0.123456, 0.123456]},
-                    "properties": {"name": "Feature 1"},
-                },
-                {
-                    "type": "Feature",
-                    "geometry": {
-                        "type": "Polygon",
-                        "coordinates": [
-                            [
-                                [5.123456, 5.123456],
-                                [15.123456, 5.123456],
-                                [15.123456, 15.123456],
-                                [5.123456, 15.123456],
-                                [5.123456, 5.123456],
-                            ]
-                        ],
-                    },
-                    "properties": {"name": "Feature 2"},
-                },
-            ],
-        }
-        self.blank_feature_collection = {}
-
-        self.feature = {
-            "type": "Feature",
-            "geometry": {"type": "Point", "coordinates": [100.123456, -0.123456]},
-            "properties": {"name": "Example Point"},
-        }
-
-    def test_feature_collection_truncuation(self):
-        """Test that the coordinates of each nested Geometry object is
-        truncuated."""
-        geometry_to_include = GEOMETRY_OBJECTS
-        precision = 3
-        expected_return_value = {
-            "type": "FeatureCollection",
-            "features": [
-                {
-                    "type": "Feature",
-                    "geometry": {"type": "Point", "coordinates": [0.123, 0.123]},
-                    "properties": {"name": "Feature 1"},
-                },
-                {
-                    "type": "Feature",
-                    "geometry": {
-                        "type": "Polygon",
-                        "coordinates": [
-                            [
-                                [5.123, 5.123],
-                                [15.123, 5.123],
-                                [15.123, 15.123],
-                                [5.123, 15.123],
-                                [5.123, 5.123],
-                            ]
-                        ],
-                    },
-                    "properties": {"name": "Feature 2"},
-                },
-            ],
-        }
-
-        self.assertEqual(
-            _process_features(
-                self.feature_collection, precision, geometry_to_include, False
-            ),
-            expected_return_value,
-        )
-
-    def test_feature_truncuation(self):
-        """Test that the Feature is processed (coordinates truncuated).
-        Note the distinction between Feature and FeatureCollection.
-        """
-        geometry_to_include = GEOMETRY_OBJECTS
-        precision = 3
-        expected_return_value = {
-            "type": "Feature",
-            "geometry": {"type": "Point", "coordinates": [100.123, -0.123]},
-            "properties": {"name": "Example Point"},
-        }
-
-        self.assertEqual(
-            _process_features(self.feature, precision, geometry_to_include, False),
-            expected_return_value,
-        )
-
-    def test_empty_gson_file(self):
-        """Test that an exception is raised when an empty
-        GeoJSON file is passed."""
-        with self.assertRaises(SystemError):
-            _process_features(self.blank_feature_collection, 3, ["Point"], False)
-
-    def test_properties_nullified(self):
-        """Test that the properties key returns a null/empty dictionary."""
-        precision = 3
-        expected_return_value = {
-            "type": "FeatureCollection",
-            "features": [
-                {
-                    "type": "Feature",
-                    "geometry": {"type": "Point", "coordinates": [0.123, 0.123]},
-                    "properties": {},
-                },
-                {
-                    "type": "Feature",
-                    "geometry": {
-                        "type": "Polygon",
-                        "coordinates": [
-                            [
-                                [5.123, 5.123],
-                                [15.123, 5.123],
-                                [15.123, 15.123],
-                                [5.123, 15.123],
-                                [5.123, 5.123],
-                            ]
-                        ],
-                    },
-                    "properties": {},
-                },
-            ],
-        }
-
-        self.assertEqual(
-            _process_features(
-                self.feature_collection, precision, GEOMETRY_OBJECTS, True
-            ),
-            expected_return_value,
-        )
-
-    def test_geometry_to_include_parameter(self):
-        """Test that only the passed geometry objects are truncuated."""
-        geometry_to_include = ["Polygon"]
-        precision = 3
-        expected_return_value = {
-            "type": "FeatureCollection",
-            "features": [
-                {
-                    "type": "Feature",
-                    "geometry": {"type": "Point", "coordinates": [0.123456, 0.123456]},
-                    "properties": {"name": "Feature 1"},
-                },
-                {
-                    "type": "Feature",
-                    "geometry": {
-                        "type": "Polygon",
-                        "coordinates": [
-                            [
-                                [5.123, 5.123],
-                                [15.123, 5.123],
-                                [15.123, 15.123],
-                                [5.123, 15.123],
-                                [5.123, 5.123],
-                            ]
-                        ],
-                    },
-                    "properties": {"name": "Feature 2"},
-                },
-            ],
-        }
-
-        self.assertEqual(
-            _process_features(
-                self.feature_collection, precision, geometry_to_include, False
-            ),
-            expected_return_value,
-        )
-
-
-if __name__ == "__main__":
-    unittest.main(buffer=True)
+"""Unit tests for geojson_shave.py"""
+
+import os
+import unittest
+import sys
+
+from geojson_shave.geojson_shave import (
+    _create_coordinates,
+    _process_geometry_collection,
+    _process_features,
+    GEOMETRY_OBJECTS,
+)
+
+
+class TestCreateCoordinates(unittest.TestCase):
+    """Tests for the _create_coordinates function.
+
+    Note that both LineStrings' and MultiPoints' coordinates both consist
+    of an array of Points, hence only the LineString being tested.
+    """
+
+    def setUp(self):
+        self.point = {
+            "type": "Point",
+            "coordinates": [-100.123456, 200.123456],
+            "properties": {"name": "Test Point"},
+        }
+
+        self.linestring = {
+            "type": "LineString",
+            "coordinates": [
+                [100.123456, 0.123456],
+                [101.123456, 1.123456],
+                [102.123456, 2.123456],
+            ],
+        }
+
+        self.multilinestring = {
+            "type": "MultiLineString",
+            "coordinates": [
+                [[-100.123456, 0.123456], [-101.123456, 1.123456]],
+                [[102.123456, 2.123456], [103.123456, 3.123456]],
+            ],
+        }
+
+        self.polygon = {
+            "type": "Polygon",
+            "coordinates": [
+                [
+                    [100.123456, 0.123456],
+                    [101.123456, 0.123456],
+                    [101.123456, 1.123456],
+                    [100.123456, 1.123456],
+                    [100.123456, 0.123456],
+                ]
+            ],
+        }
+
+        self.multipolygon = {
+            "type": "MultiPolygon",
+            "coordinates": [
+                [
+                    [
+                        [102.123456, 2.123456],
+                        [103.123456, 2.123456],
+                        [103.123456, 3.123456],
+                        [102.123456, 3.123456],
+                        [102.123456, 2.123456],
+                    ]
+                ],
+                [
+                    [
+                        [100.123456, 0.123456],
+                        [101.123456, 0.123456],
+                        [101.123456, 1.123456],
+                        [100.123456, 1.123456],
+                        [100.123456, 0.123456],
+                    ],
+                    [
+                        [100.123456, 0.123456],
+                        [100.123456, 0.123456],
+                        [100.123456, 0.123456],
+                        [100.123456, 0.123456],
+                        [100.123456, 0.123456],
+                    ],
+                ],
+            ],
+        }
+
+    # Point.
+    def test_truncuating_point_coordinates(self):
+        """Test that Point coordinates are truncuated succesfully."""
+        expected_return_value = [-100.123, 200.123]
+        precision = 3
+        geometry_coordinates = self.point["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    def test_point_same_precision(self):
+        """Test that Point coordinates are not truncuated when
+        the coordinate decimal points matches what's passed
+        to the precision parameter.
+        """
+        expected_return_value = self.point["coordinates"]
+        precision = 6
+        geometry_coordinates = self.point["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    def test_point_precision_larger_than_places(self):
+        """Test that when the precision argument is a value larger
+        than the number of coordinate decimnal points, the same coordinate values
+        are returned.
+        """
+        expected_return_value = self.point["coordinates"]
+        precision = 50
+        geometry_coordinates = self.point["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    # LineString.
+    def test_truncuating_linestring_coordinates(self):
+        """Test that LineString coordinates are truncuated succesfully."""
+        expected_return_value = [
+            [100.123, 0.123],
+            [101.123, 1.123],
+            [102.123, 2.123],
+        ]
+        precision = 3
+        geometry_coordinates = self.linestring["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    def test_linestring_same_precision(self):
+        """Test that LineString coordinates are not truncuated when
+        the coordinate decimal points matches what's passed
+        to the precision parameter.
+        """
+        expected_return_value = self.linestring["coordinates"]
+        precision = 6
+        geometry_coordinates = self.linestring["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    def test_linestring_precision_larger_than_places(self):
+        """Test that when the precision argument is a value larger
+        than the number of coordinate decimnal points, the same coordinate values
+        are returned.
+        """
+        expected_return_value = self.linestring["coordinates"]
+        precision = 50
+        geometry_coordinates = self.linestring["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    # MultiLine strings.
+    def test_truncuating_multilinestring_coordinates(self):
+        """Test that MultiLineString coordinates are truncuated succesfully."""
+        expected_return_value = [
+            [[-100.123, 0.123], [-101.123, 1.123]],
+            [[102.123, 2.123], [103.123, 3.123]],
+        ]
+        precision = 3
+        geometry_coordinates = self.multilinestring["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    def test_multilinestring_precision_larger_than_places(self):
+        """Test that when the precision argument is a value larger
+        than the number of coordinate decimnal points, the same coordinate values
+        are returned.
+        """
+        expected_return_value = self.multilinestring["coordinates"]
+        precision = 50
+        geometry_coordinates = self.multilinestring["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    def test_multilinestring_same_precision(self):
+        """Test that LineString coordinates are not truncuated when
+        the coordinate decimal points matches what's passed
+        to the precision parameter.
+        """
+        expected_return_value = self.multipolygon["coordinates"]
+        precision = 6
+        geometry_coordinates = self.multipolygon["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    # Polygon.
+    def test_truncuating_polygon_coordinates(self):
+        """Test that Polygon coordinates are truncuated succesfully."""
+        expected_return_value = [
+            [
+                [100.123, 0.123],
+                [101.123, 0.123],
+                [101.123, 1.123],
+                [100.123, 1.123],
+                [100.123, 0.123],
+            ]
+        ]
+        precision = 3
+        geometry_coordinates = self.polygon["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    def test_polygon_precision_larger_than_places(self):
+        """Test that when the precision argument is a value larger
+        than the number of coordinate decimnal points, the same coordinate values
+        are returned.
+        """
+        expected_return_value = [
+            [
+                [100.123456, 0.123456],
+                [101.123456, 0.123456],
+                [101.123456, 1.123456],
+                [100.123456, 1.123456],
+                [100.123456, 0.123456],
+            ]
+        ]
+        precision = 50
+        geometry_coordinates = self.polygon["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    def test_polygon_same_precision(self):
+        """Test that LineString coordinates are not truncuated when
+        the coordinate decimal points matches what's passed
+        to the precision parameter.
+        """
+        expected_return_value = [
+            [
+                [100.123456, 0.123456],
+                [101.123456, 0.123456],
+                [101.123456, 1.123456],
+                [100.123456, 1.123456],
+                [100.123456, 0.123456],
+            ]
+        ]
+        precision = 6
+        geometry_coordinates = self.polygon["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    # MultiPolygon.
+    def test_truncuating_multipolygon_coordinates(self):
+        """Test that MultiPolygon coordinates are truncuated succesfully."""
+        expected_return_value = [
+            [
+                [
+                    [102.123, 2.123],
+                    [103.123, 2.123],
+                    [103.123, 3.123],
+                    [102.123, 3.123],
+                    [102.123, 2.123],
+                ]
+            ],
+            [
+                [
+                    [100.123, 0.123],
+                    [101.123, 0.123],
+                    [101.123, 1.123],
+                    [100.123, 1.123],
+                    [100.123, 0.123],
+                ],
+                [
+                    [100.123, 0.123],
+                    [100.123, 0.123],
+                    [100.123, 0.123],
+                    [100.123, 0.123],
+                    [100.123, 0.123],
+                ],
+            ],
+        ]
+        precision = 3
+        geometry_coordinates = self.multipolygon["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    def test_multipolygon_precision_larger_than_places(self):
+        """Test that when the precision argument is a value larger
+        than the number of coordinate decimnal points, the same coordinate values
+        are returned.
+        """
+        expected_return_value = self.multipolygon["coordinates"]
+        precision = 50
+        geometry_coordinates = self.multipolygon["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    def test_multipolygon_same_precision(self):
+        """Test that LineString coordinates are not truncuated when
+        the coordinate decimal points matches what's passed
+        to the precision parameter.
+        """
+        expected_return_value = self.multipolygon["coordinates"]
+        precision = 6
+        geometry_coordinates = self.multipolygon["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+
+class TestProcessGeometryCollection(unittest.TestCase):
+    """Tests for the _process_geometry_collection function."""
+
+    def setUp(self):
+        self.geometry_collection = {
+            "type": "GeometryCollection",
+            "geometries": [
+                {"type": "Point", "coordinates": [0.123456, 0.123456]},
+                {
+                    "type": "LineString",
+                    "coordinates": [
+                        [1.123456, 1.123456],
+                        [2.123456, 3.123456],
+                        [4.123456, 5.123456],
+                    ],
+                },
+                {
+                    "type": "Polygon",
+                    "coordinates": [
+                        [
+                            [6.123456, 6.123456],
+                            [8.123456, 8.123456],
+                            [10.123456, 10.123456],
+                            [6.123456, 6.123456],
+                        ]
+                    ],
+                },
+                {
+                    "type": "MultiPoint",
+                    "coordinates": [
+                        [12.123456, 12.123456],
+                        [14.123456, 14.123456],
+                        [16.123456, 16.123456],
+                    ],
+                },
+            ],
+        }
+
+    def test_truncuating_coordinates(self):
+        """Tests that the coordinates of each nested Geometry object
+        is truncuated correctly."""
+
+        expected_return_value = {
+            "type": "GeometryCollection",
+            "geometries": [
+                {"type": "Point", "coordinates": [0.123, 0.123]},
+                {
+                    "type": "LineString",
+                    "coordinates": [[1.123, 1.123], [2.123, 3.123], [4.123, 5.123]],
+                },
+                {
+                    "type": "Polygon",
+                    "coordinates": [
+                        [
+                            [6.123, 6.123],
+                            [8.123, 8.123],
+                            [10.123, 10.123],
+                            [6.123, 6.123],
+                        ]
+                    ],
+                },
+                {
+                    "type": "MultiPoint",
+                    "coordinates": [
+                        [12.123, 12.123],
+                        [14.123, 14.123],
+                        [16.123, 16.123],
+                    ],
+                },
+            ],
+        }
+
+        geo_collection = self.geometry_collection
+        precision = 3
+        self.assertEqual(
+            _process_geometry_collection(geo_collection, precision),
+            expected_return_value,
+        )
+
+
+class TestProcessFeatures(unittest.TestCase):
+    """Tests for the _process_features function."""
+
+    def setUp(self):
+        self.feature_collection = {
+            "type": "FeatureCollection",
+            "features": [
+                {
+                    "type": "Feature",
+                    "geometry": {"type": "Point", "coordinates": [0.123456, 0.123456]},
+                    "properties": {"name": "Feature 1"},
+                },
+                {
+                    "type": "Feature",
+                    "geometry": {
+                        "type": "Polygon",
+                        "coordinates": [
+                            [
+                                [5.123456, 5.123456],
+                                [15.123456, 5.123456],
+                                [15.123456, 15.123456],
+                                [5.123456, 15.123456],
+                                [5.123456, 5.123456],
+                            ]
+                        ],
+                    },
+                    "properties": {"name": "Feature 2"},
+                },
+            ],
+        }
+        self.blank_feature_collection = {}
+
+        self.feature = {
+            "type": "Feature",
+            "geometry": {"type": "Point", "coordinates": [100.123456, -0.123456]},
+            "properties": {"name": "Example Point"},
+        }
+
+    def test_feature_collection_truncuation(self):
+        """Test that the coordinates of each nested Geometry object is
+        truncuated."""
+        geometry_to_include = GEOMETRY_OBJECTS
+        precision = 3
+        expected_return_value = {
+            "type": "FeatureCollection",
+            "features": [
+                {
+                    "type": "Feature",
+                    "geometry": {"type": "Point", "coordinates": [0.123, 0.123]},
+                    "properties": {"name": "Feature 1"},
+                },
+                {
+                    "type": "Feature",
+                    "geometry": {
+                        "type": "Polygon",
+                        "coordinates": [
+                            [
+                                [5.123, 5.123],
+                                [15.123, 5.123],
+                                [15.123, 15.123],
+                                [5.123, 15.123],
+                                [5.123, 5.123],
+                            ]
+                        ],
+                    },
+                    "properties": {"name": "Feature 2"},
+                },
+            ],
+        }
+
+        self.assertEqual(
+            _process_features(
+                self.feature_collection, precision, geometry_to_include, False
+            ),
+            expected_return_value,
+        )
+
+    def test_feature_truncuation(self):
+        """Test that the Feature is processed (coordinates truncuated).
+        Note the distinction between Feature and FeatureCollection.
+        """
+        geometry_to_include = GEOMETRY_OBJECTS
+        precision = 3
+        expected_return_value = {
+            "type": "Feature",
+            "geometry": {"type": "Point", "coordinates": [100.123, -0.123]},
+            "properties": {"name": "Example Point"},
+        }
+
+        self.assertEqual(
+            _process_features(self.feature, precision, geometry_to_include, False),
+            expected_return_value,
+        )
+
+    def test_empty_gson_file(self):
+        """Test that an exception is raised when an empty
+        GeoJSON file is passed."""
+        with self.assertRaises(RuntimeError):
+            _process_features(self.blank_feature_collection, 3, ["Point"], False)
+
+    def test_properties_nullified(self):
+        """Test that the properties key returns a null/empty dictionary."""
+        precision = 3
+        expected_return_value = {
+            "type": "FeatureCollection",
+            "features": [
+                {
+                    "type": "Feature",
+                    "geometry": {"type": "Point", "coordinates": [0.123, 0.123]},
+                    "properties": {},
+                },
+                {
+                    "type": "Feature",
+                    "geometry": {
+                        "type": "Polygon",
+                        "coordinates": [
+                            [
+                                [5.123, 5.123],
+                                [15.123, 5.123],
+                                [15.123, 15.123],
+                                [5.123, 15.123],
+                                [5.123, 5.123],
+                            ]
+                        ],
+                    },
+                    "properties": {},
+                },
+            ],
+        }
+
+        self.assertEqual(
+            _process_features(
+                self.feature_collection, precision, GEOMETRY_OBJECTS, True
+            ),
+            expected_return_value,
+        )
+
+    def test_geometry_to_include_parameter(self):
+        """Test that only the passed geometry objects are truncuated."""
+        geometry_to_include = ["Polygon"]
+        precision = 3
+        expected_return_value = {
+            "type": "FeatureCollection",
+            "features": [
+                {
+                    "type": "Feature",
+                    "geometry": {"type": "Point", "coordinates": [0.123456, 0.123456]},
+                    "properties": {"name": "Feature 1"},
+                },
+                {
+                    "type": "Feature",
+                    "geometry": {
+                        "type": "Polygon",
+                        "coordinates": [
+                            [
+                                [5.123, 5.123],
+                                [15.123, 5.123],
+                                [15.123, 15.123],
+                                [5.123, 15.123],
+                                [5.123, 5.123],
+                            ]
+                        ],
+                    },
+                    "properties": {"name": "Feature 2"},
+                },
+            ],
+        }
+
+        self.assertEqual(
+            _process_features(
+                self.feature_collection, precision, geometry_to_include, False
+            ),
+            expected_return_value,
+        )
+
+
+if __name__ == "__main__":
+    unittest.main(buffer=True)
```

