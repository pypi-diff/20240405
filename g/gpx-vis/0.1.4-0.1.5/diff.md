# Comparing `tmp/gpx_vis-0.1.4.tar.gz` & `tmp/gpx_vis-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpx_vis-0.1.4.tar", last modified: Fri Apr  5 13:41:48 2024, max compression
+gzip compressed data, was "gpx_vis-0.1.5.tar", last modified: Fri Apr  5 13:51:13 2024, max compression
```

## Comparing `gpx_vis-0.1.4.tar` & `gpx_vis-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-05 13:41:48.736803 gpx_vis-0.1.4/
--rw-r--r--   0 jwt        (501) staff       (20)     1514 2024-04-05 12:16:08.000000 gpx_vis-0.1.4/LICENSE
--rw-r--r--   0 jwt        (501) staff       (20)      513 2024-04-05 13:41:48.736551 gpx_vis-0.1.4/PKG-INFO
--rw-r--r--   0 jwt        (501) staff       (20)      142 2024-04-05 12:13:11.000000 gpx_vis-0.1.4/README.md
--rw-r--r--   0 jwt        (501) staff       (20)      454 2024-04-05 13:41:40.000000 gpx_vis-0.1.4/pyproject.toml
--rw-r--r--   0 jwt        (501) staff       (20)       38 2024-04-05 13:41:48.736903 gpx_vis-0.1.4/setup.cfg
-drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-05 13:41:48.735138 gpx_vis-0.1.4/src/
--rw-r--r--   0 jwt        (501) staff       (20)      174 2024-04-05 12:36:48.000000 gpx_vis-0.1.4/src/__init__.py
-drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-05 13:41:48.736260 gpx_vis-0.1.4/src/gpx_vis.egg-info/
--rw-r--r--   0 jwt        (501) staff       (20)      513 2024-04-05 13:41:48.000000 gpx_vis-0.1.4/src/gpx_vis.egg-info/PKG-INFO
--rw-r--r--   0 jwt        (501) staff       (20)      203 2024-04-05 13:41:48.000000 gpx_vis-0.1.4/src/gpx_vis.egg-info/SOURCES.txt
--rw-r--r--   0 jwt        (501) staff       (20)        1 2024-04-05 13:41:48.000000 gpx_vis-0.1.4/src/gpx_vis.egg-info/dependency_links.txt
--rw-r--r--   0 jwt        (501) staff       (20)       17 2024-04-05 13:41:48.000000 gpx_vis-0.1.4/src/gpx_vis.egg-info/top_level.txt
--rw-r--r--   0 jwt        (501) staff       (20)    16847 2024-04-05 13:39:39.000000 gpx_vis-0.1.4/src/gpx_vis.py
+drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-05 13:51:13.872618 gpx_vis-0.1.5/
+-rw-r--r--   0 jwt        (501) staff       (20)     1514 2024-04-05 12:16:08.000000 gpx_vis-0.1.5/LICENSE
+-rw-r--r--   0 jwt        (501) staff       (20)      513 2024-04-05 13:51:13.872385 gpx_vis-0.1.5/PKG-INFO
+-rw-r--r--   0 jwt        (501) staff       (20)      142 2024-04-05 12:13:11.000000 gpx_vis-0.1.5/README.md
+-rw-r--r--   0 jwt        (501) staff       (20)      454 2024-04-05 13:51:08.000000 gpx_vis-0.1.5/pyproject.toml
+-rw-r--r--   0 jwt        (501) staff       (20)       38 2024-04-05 13:51:13.872686 gpx_vis-0.1.5/setup.cfg
+drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-05 13:51:13.871075 gpx_vis-0.1.5/src/
+-rw-r--r--   0 jwt        (501) staff       (20)      174 2024-04-05 12:36:48.000000 gpx_vis-0.1.5/src/__init__.py
+drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-05 13:51:13.872150 gpx_vis-0.1.5/src/gpx_vis.egg-info/
+-rw-r--r--   0 jwt        (501) staff       (20)      513 2024-04-05 13:51:13.000000 gpx_vis-0.1.5/src/gpx_vis.egg-info/PKG-INFO
+-rw-r--r--   0 jwt        (501) staff       (20)      203 2024-04-05 13:51:13.000000 gpx_vis-0.1.5/src/gpx_vis.egg-info/SOURCES.txt
+-rw-r--r--   0 jwt        (501) staff       (20)        1 2024-04-05 13:51:13.000000 gpx_vis-0.1.5/src/gpx_vis.egg-info/dependency_links.txt
+-rw-r--r--   0 jwt        (501) staff       (20)       17 2024-04-05 13:51:13.000000 gpx_vis-0.1.5/src/gpx_vis.egg-info/top_level.txt
+-rw-r--r--   0 jwt        (501) staff       (20)    16922 2024-04-05 13:49:16.000000 gpx_vis-0.1.5/src/gpx_vis.py
```

### Comparing `gpx_vis-0.1.4/LICENSE` & `gpx_vis-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gpx_vis-0.1.4/PKG-INFO` & `gpx_vis-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpx_vis
-Version: 0.1.4
+Version: 0.1.5
 Summary: A small example package
 Author-email: Jia Wei Teh <jiaweiteh.astro@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `gpx_vis-0.1.4/src/gpx_vis.egg-info/PKG-INFO` & `gpx_vis-0.1.5/src/gpx_vis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpx_vis
-Version: 0.1.4
+Version: 0.1.5
 Summary: A small example package
 Author-email: Jia Wei Teh <jiaweiteh.astro@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `gpx_vis-0.1.4/src/gpx_vis.py` & `gpx_vis-0.1.5/src/gpx_vis.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,14 +314,16 @@
         _tilesList = ['openstreetmap', 'CartoDB Voyager', 'Cartodb dark_matter', 'cartodbpositron']
         for tiles in _tilesList:
             folium.TileLayer(tiles).add_to(main_map)
         # add layer control
         folium.LayerControl(position='bottomright').add_to(main_map)
         
         # save
+        if not filename.endswith(".html"):
+            filename += '.html'
         main_map.save(filename)
         
         return print(f"File saved as {filename}.")
     
     @staticmethod
     def _addTracksOnMap(self, group, selected_idx):
         """
```

