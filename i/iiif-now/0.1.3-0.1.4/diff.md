# Comparing `tmp/iiif_now-0.1.3.tar.gz` & `tmp/iiif_now-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iiif_now-0.1.3.tar", max compression
+gzip compressed data, was "iiif_now-0.1.4.tar", max compression
```

## Comparing `iiif_now-0.1.3.tar` & `iiif_now-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      280 2024-04-03 22:39:47.822765 iiif_now-0.1.3/CHANGELOG.md
--rw-r--r--   0        0        0     1096 2024-04-03 23:26:07.781593 iiif_now-0.1.3/README.md
--rw-r--r--   0        0        0      165 2024-04-03 22:15:54.969000 iiif_now-0.1.3/iiif_now/__init__.py
--rw-r--r--   0        0        0       33 2024-03-31 14:34:26.835751 iiif_now-0.1.3/iiif_now/csvreader/__init__.py
--rw-r--r--   0        0        0     4520 2024-04-03 14:47:09.996938 iiif_now-0.1.3/iiif_now/csvreader/csvreader.py
--rw-r--r--   0        0        0       34 2024-03-31 14:35:09.074716 iiif_now-0.1.3/iiif_now/datacanvas/__init__.py
--rw-r--r--   0        0        0     2033 2024-04-03 15:22:16.528962 iiif_now-0.1.3/iiif_now/datacanvas/datacanvas.py
--rw-r--r--   0        0        0      975 2024-04-02 23:02:06.414380 iiif_now-0.1.3/iiif_now/iiifnow.py
--rw-r--r--   0        0        0       32 2024-03-31 23:06:07.096746 iiif_now-0.1.3/iiif_now/manifest/__init__.py
--rw-r--r--   0        0        0     6038 2024-04-03 22:57:04.940434 iiif_now-0.1.3/iiif_now/manifest/manifest.py
--rw-r--r--   0        0        0       30 2024-04-02 22:30:01.682517 iiif_now-0.1.3/iiif_now/navplace/__init__.py
--rw-r--r--   0        0        0     2173 2024-04-02 22:33:08.662831 iiif_now-0.1.3/iiif_now/navplace/navplace.py
--rw-r--r--   0        0        0       32 2024-04-03 22:15:54.948804 iiif_now-0.1.3/iiif_now/thumbnail/__init__.py
--rw-r--r--   0        0        0     1041 2024-04-03 22:38:50.485206 iiif_now-0.1.3/iiif_now/thumbnail/thumbnail.py
--rw-r--r--   0        0        0      593 2024-04-03 23:28:07.016844 iiif_now-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2298 1970-01-01 00:00:00.000000 iiif_now-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      545 2024-04-05 18:46:31.521092 iiif_now-0.1.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1157 2024-04-05 18:50:34.024138 iiif_now-0.1.4/README.md
+-rw-r--r--   0        0        0      165 2024-04-03 22:15:54.969000 iiif_now-0.1.4/iiif_now/__init__.py
+-rw-r--r--   0        0        0       33 2024-03-31 14:34:26.835751 iiif_now-0.1.4/iiif_now/csvreader/__init__.py
+-rw-r--r--   0        0        0     4520 2024-04-03 14:47:09.996938 iiif_now-0.1.4/iiif_now/csvreader/csvreader.py
+-rw-r--r--   0        0        0       34 2024-03-31 14:35:09.074716 iiif_now-0.1.4/iiif_now/datacanvas/__init__.py
+-rw-r--r--   0        0        0     2033 2024-04-03 15:22:16.528962 iiif_now-0.1.4/iiif_now/datacanvas/datacanvas.py
+-rw-r--r--   0        0        0      975 2024-04-02 23:02:06.414380 iiif_now-0.1.4/iiif_now/iiifnow.py
+-rw-r--r--   0        0        0       32 2024-03-31 23:06:07.096746 iiif_now-0.1.4/iiif_now/manifest/__init__.py
+-rw-r--r--   0        0        0     6065 2024-04-05 18:45:21.332298 iiif_now-0.1.4/iiif_now/manifest/manifest.py
+-rw-r--r--   0        0        0       30 2024-04-02 22:30:01.682517 iiif_now-0.1.4/iiif_now/navplace/__init__.py
+-rw-r--r--   0        0        0     2418 2024-04-05 13:28:21.220416 iiif_now-0.1.4/iiif_now/navplace/navplace.py
+-rw-r--r--   0        0        0       32 2024-04-03 22:15:54.948804 iiif_now-0.1.4/iiif_now/thumbnail/__init__.py
+-rw-r--r--   0        0        0     1041 2024-04-03 22:38:50.485206 iiif_now-0.1.4/iiif_now/thumbnail/thumbnail.py
+-rw-r--r--   0        0        0      593 2024-04-04 12:22:12.705733 iiif_now-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2624 1970-01-01 00:00:00.000000 iiif_now-0.1.4/PKG-INFO
```

### Comparing `iiif_now-0.1.3/README.md` & `iiif_now-0.1.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # IIIF Now
 
 ## About
 
 IIIF Manifest generation tools for the Abolition Now project.
 
-![Example Manifest](manifest_example.png "Example Manifest")
+![Example Manifest](https://github.com/abolition-now/iiif_now/blob/main/manifest_example.png?raw=true "Example Manifest")
 
 ## Installation
 
 ```bash
 pip install iiif-now
 ```
```

### Comparing `iiif_now-0.1.3/iiif_now/csvreader/csvreader.py` & `iiif_now-0.1.4/iiif_now/csvreader/csvreader.py`

 * *Files identical despite different names*

### Comparing `iiif_now-0.1.3/iiif_now/datacanvas/datacanvas.py` & `iiif_now-0.1.4/iiif_now/datacanvas/datacanvas.py`

 * *Files identical despite different names*

### Comparing `iiif_now-0.1.3/iiif_now/iiifnow.py` & `iiif_now-0.1.4/iiif_now/iiifnow.py`

 * *Files identical despite different names*

### Comparing `iiif_now-0.1.3/iiif_now/manifest/manifest.py` & `iiif_now-0.1.4/iiif_now/manifest/manifest.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,75 +2,77 @@
 import requests
 import json
 from iiif_now.navplace import NavPlace
 from iiif_now.thumbnail import Thumbnail
 
 
 class ANManifest:
-    # @Todo: Reduce requests by adding thumbnails to manifest.
     def __init__(
             self,
             manifest_data,
             image_server_path="https://strob6zro3bzklrulaqu2545sy0odbvz.lambda-url.us-east-2.on.aws/iiif/3/",
             video_location="https://digital.lib.utk.edu/static/",
-            manifest_bucket="https://aboltion-now-manifests.s3.us-east-2.amazonaws.com/",
+            manifest_bucket="https://raw.githubusercontent.com/markpbaggett/static_iiif/main/manifests/abolition_now/",
             extensions=[]
     ):
         self.config = config.configs['helpers.auto_fields.AutoLang'].auto_lang = "en"
         self.image_server_path = image_server_path
         self.manifest_bucket = manifest_bucket
         self.video_location = video_location
         self.manifest_data = manifest_data
-        self.metadata = self.__build_metadata()
+        self.metadata = self.__build_metadata(manifest_data['metadata'])
         self.features = self.__find_features()
         self.manifest = self.__build_manifest()
         self.extensions = load_bundled_extensions(
             extensions=extensions
         )
 
     def __build_manifest(self):
+        # @Todo: Clean up this method.  It's a mess and doing too much.
         if self.features:
             navplace_data = NavPlace(
                 self.features,
                 self.manifest_bucket,
                 self.manifest_data['manifest_title'] if self.manifest_data['manifest_title'] != "" else "Untitled"
             ).features
             manifest = Manifest(
-                id=f"https://raw.githubusercontent.com/markpbaggett/static_iiif/main/manifests/abolition_now/{self.manifest_data['id']}.json",
+                id=f"{self.manifest_bucket}{self.manifest_data['id']}.json",
                 label=self.manifest_data['manifest_title'] if self.manifest_data['manifest_title'] != "" else "Untitled",
                 metadata=self.metadata,
                 navPlace={"features": navplace_data}
             )
         else:
             manifest = Manifest(
-                id=f"https://raw.githubusercontent.com/markpbaggett/static_iiif/main/manifests/abolition_now/{self.manifest_data['id']}.json",
+                id=f"{self.manifest_bucket}{self.manifest_data['id']}.json",
                 label=self.manifest_data['manifest_title'] if self.manifest_data[
                                                                   'manifest_title'] != "" else "Untitled",
                 metadata=self.metadata
             )
         for canvas in self.manifest_data['canvases']:
-            # @Todo: Add canvas metadata to canvas.
+            thumbnail = Thumbnail(f"{self.image_server_path}{canvas['thumbnail']}").get()
             if canvas['type'] == 'Image':
                 try:
                     # @Todo: Protect anno page and annotation
-                    thumbnail = Thumbnail(f"{self.image_server_path}{canvas['key']}").get()
                     manifest.make_canvas_from_iiif(
                         url=f"{self.image_server_path}{canvas['key']}",
                         label=canvas['label'] if canvas['label'] != "" else "Untitled",
                         id=f"{self.manifest_bucket}{canvas['key']}/canvas/{canvas['sequence']}",
                         anno_id=f"{self.manifest_bucket}{canvas['key']}/canvas/{canvas['sequence']}/annotation/1",
                         anno_page_id=f"{self.manifest_bucket}{canvas['key']}/canvas/{canvas['sequence']}/annotation/1/page/1",
-                        thumbnail=thumbnail
+                        thumbnail=thumbnail,
+                        metadata=self.__build_metadata(canvas.get('metadata'))
                     )
                 except requests.HTTPError as e:
                     print(f'{e}. Missing file in bucket or other image server problem.')
             elif canvas['type'] == 'Video':
                 vid_canvas = manifest.make_canvas(
                     id=f"{self.manifest_bucket}{canvas['key']}/canvas/{canvas['sequence']}",
                     label=canvas['label'] if canvas['label'] != "" else "Untitled",
+                    thumbnail=thumbnail,
+                    metadata=self.__build_metadata(canvas.get('metadata'))
                 )
                 details = self.__create_video_canvas(
                     canvas=vid_canvas,
                     canvas_data= canvas
                 )
                 vid_canvas.set_hwd(**details[1])
                 vid_canvas.add_item(details[0])
@@ -83,17 +85,18 @@
         all_features = []
         for k, v in self.manifest_data['metadata'].items():
             if k == 'Geography':
                 for feature in v:
                     all_features.append(feature)
         return all_features
 
-    def __build_metadata(self):
+    @staticmethod
+    def __build_metadata(metadata_values):
         metadata = []
-        for k, v in self.manifest_data['metadata'].items():
+        for k, v in metadata_values.items():
             metadata.append(
                 KeyValueString(
                     label=k,
                     value={"en": v}
                 )
             )
         if not metadata:
@@ -109,15 +112,14 @@
         with open(f'{path}/{self.manifest_data["id"]}.json', 'w') as outfile:
             outfile.write(
                 json.dumps(
                     self.manifest, indent=2)
             )
 
     def __create_video_canvas(self, canvas, canvas_data):
-        # @Todo: Check for video file like we do for images.
         anno_body = ResourceItem(
             id=f"{self.video_location}{canvas_data['key']}",
             type="Video",
             format="video/mp4"
         )
         anno_page = AnnotationPage(
             id=f"{self.manifest_bucket}{canvas_data['key']}/canvas/{canvas_data['sequence']}/annotation/1/page/1"
```

### Comparing `iiif_now-0.1.3/iiif_now/navplace/navplace.py` & `iiif_now-0.1.4/iiif_now/navplace/navplace.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,35 +27,39 @@
             "Minneapolis": [44.9778, -93.2650],
             "Standing Rock": [45.8038, -101.8642],
             "New York City, NY": [40.7128, -74.0060],
             "Philadelphia": [39.9526, -75.1652],
             "Boston": [42.3601, -71.0589],
             "Durham": [35.9940, -78.8986],
             "Turtle Island": [36.7783, -119.4179],
+            "Colombia": [4.7110, -74.0721]
         }
 
     def __add_navplace_features(self):
         features = []
         i = 0
         for feature in self.features:
-            features.append(
-                {
-                    "id": f"{self.parent_uri}/notdereferenceable/feature/{i}",
-                    "type": "Feature",
-                    "properties": {
-                        "label": {
-                            "en": [
-                                f"{self.title} -- {feature}"
+            try:
+                features.append(
+                    {
+                        "id": f"{self.parent_uri}notdereferenceable/feature/{i}",
+                        "type": "Feature",
+                        "properties": {
+                            "label": {
+                                "en": [
+                                    f"{self.title} -- {feature}"
+                                ]
+                            }
+                        },
+                        "geometry": {
+                            "type": "Point",
+                            "coordinates": [
+                                self.all_locations[feature][1],
+                                self.all_locations[feature][0]
                             ]
                         }
-                    },
-                    "geometry": {
-                        "type": "Point",
-                        "coordinates": [
-                            self.all_locations[feature][1],
-                            self.all_locations[feature][0]
-                        ]
                     }
-                }
-            )
-            i += 1
+                )
+                i += 1
+            except KeyError:
+                print(f"Feature {feature} not found in locations. Add.")
         return features
```

### Comparing `iiif_now-0.1.3/iiif_now/thumbnail/thumbnail.py` & `iiif_now-0.1.4/iiif_now/thumbnail/thumbnail.py`

 * *Files identical despite different names*

### Comparing `iiif_now-0.1.3/pyproject.toml` & `iiif_now-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iiif-now"
-version = "0.1.3"
+version = "0.1.4"
 description = "IIIF Manifest Generator for Abolition Now project"
 authors = ["Mark Baggett <mbagget1@utk.edu>"]
 license = "WTFPL"
 readme = ["README.md", "CHANGELOG.md"]
 repository = "https://github.com/abolition-now/iiif_now/"
 
 [tool.poetry.dependencies]
```

### Comparing `iiif_now-0.1.3/PKG-INFO` & `iiif_now-0.1.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iiif-now
-Version: 0.1.3
+Version: 0.1.4
 Summary: IIIF Manifest Generator for Abolition Now project
 Home-page: https://github.com/abolition-now/iiif_now/
 License: WTFPL
 Author: Mark Baggett
 Author-email: mbagget1@utk.edu
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -24,15 +24,15 @@
 
 # IIIF Now
 
 ## About
 
 IIIF Manifest generation tools for the Abolition Now project.
 
-![Example Manifest](manifest_example.png "Example Manifest")
+![Example Manifest](https://github.com/abolition-now/iiif_now/blob/main/manifest_example.png?raw=true "Example Manifest")
 
 ## Installation
 
 ```bash
 pip install iiif-now
 ```
 
@@ -54,14 +54,29 @@
 ## Usage
 
 ```bash
 iiifnow use config.yml
 ```
 # Changes
 
+## [0.1.4] - 2024-04-05
+
+### Features
+
+* Canvases now have metadata.
+
+### Bug Fixes
+
+* Thumbnails: Both video an image canvases get thumbnails.
+* navPlace: If location unknown, print error and pass.
+
+### Minor Changes
+
+* Manifests: Got rid of all hard-coded URIs.
+
 ## [0.1.3] - 2024-04-03
 
 ### Features
 
 * Added artists to metadata.
 * Added thumbnails to image canvases.
```

