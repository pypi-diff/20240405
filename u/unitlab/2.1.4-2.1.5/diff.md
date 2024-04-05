# Comparing `tmp/unitlab-2.1.4.tar.gz` & `tmp/unitlab-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitlab-2.1.4.tar", last modified: Thu Mar 28 12:17:13 2024, max compression
+gzip compressed data, was "unitlab-2.1.5.tar", last modified: Fri Apr  5 12:20:50 2024, max compression
```

## Comparing `unitlab-2.1.4.tar` & `unitlab-2.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-03-28 12:17:13.184551 unitlab-2.1.4/
--rw-rw-r--   0 me        (1000) me        (1000)     1069 2024-02-13 07:39:37.000000 unitlab-2.1.4/LICENSE.md
--rw-r--r--   0 me        (1000) me        (1000)      843 2024-03-28 12:17:13.184551 unitlab-2.1.4/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)     1434 2023-09-24 12:59:00.000000 unitlab-2.1.4/README.md
--rw-rw-r--   0 me        (1000) me        (1000)      106 2024-03-28 12:17:13.184551 unitlab-2.1.4/setup.cfg
--rw-rw-r--   0 me        (1000) me        (1000)     1141 2024-03-27 11:46:56.000000 unitlab-2.1.4/setup.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-03-28 12:17:13.184551 unitlab-2.1.4/src/
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-03-28 12:17:13.184551 unitlab-2.1.4/src/unitlab/
--rw-rw-r--   0 me        (1000) me        (1000)      214 2024-03-06 15:43:31.000000 unitlab-2.1.4/src/unitlab/__init__.py
--rw-rw-r--   0 me        (1000) me        (1000)       29 2024-03-06 15:43:31.000000 unitlab-2.1.4/src/unitlab/__main__.py
--rw-rw-r--   0 me        (1000) me        (1000)    12057 2024-03-27 11:46:26.000000 unitlab-2.1.4/src/unitlab/client.py
--rw-rw-r--   0 me        (1000) me        (1000)    12479 2024-03-27 11:37:04.000000 unitlab-2.1.4/src/unitlab/dataset.py
--rw-rw-r--   0 me        (1000) me        (1000)      951 2024-03-06 15:43:31.000000 unitlab-2.1.4/src/unitlab/exceptions.py
--rw-rw-r--   0 me        (1000) me        (1000)     4547 2024-03-27 11:46:48.000000 unitlab-2.1.4/src/unitlab/main.py
--rw-rw-r--   0 me        (1000) me        (1000)     1852 2024-03-06 15:43:31.000000 unitlab-2.1.4/src/unitlab/utils.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-03-28 12:17:13.184551 unitlab-2.1.4/src/unitlab.egg-info/
--rw-r--r--   0 me        (1000) me        (1000)      843 2024-03-28 12:17:13.000000 unitlab-2.1.4/src/unitlab.egg-info/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)      411 2024-03-28 12:17:13.000000 unitlab-2.1.4/src/unitlab.egg-info/SOURCES.txt
--rw-rw-r--   0 me        (1000) me        (1000)        1 2024-03-28 12:17:13.000000 unitlab-2.1.4/src/unitlab.egg-info/dependency_links.txt
--rw-rw-r--   0 me        (1000) me        (1000)       45 2024-03-28 12:17:13.000000 unitlab-2.1.4/src/unitlab.egg-info/entry_points.txt
--rw-rw-r--   0 me        (1000) me        (1000)       48 2024-03-28 12:17:13.000000 unitlab-2.1.4/src/unitlab.egg-info/requires.txt
--rw-rw-r--   0 me        (1000) me        (1000)        8 2024-03-28 12:17:13.000000 unitlab-2.1.4/src/unitlab.egg-info/top_level.txt
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-05 12:20:50.913275 unitlab-2.1.5/
+-rw-rw-r--   0 me        (1000) me        (1000)     1069 2024-02-13 07:39:37.000000 unitlab-2.1.5/LICENSE.md
+-rw-r--r--   0 me        (1000) me        (1000)      793 2024-04-05 12:20:50.913275 unitlab-2.1.5/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)     1434 2023-09-24 12:59:00.000000 unitlab-2.1.5/README.md
+-rw-rw-r--   0 me        (1000) me        (1000)      106 2024-04-05 12:20:50.913275 unitlab-2.1.5/setup.cfg
+-rw-rw-r--   0 me        (1000) me        (1000)     1092 2024-04-05 12:19:12.000000 unitlab-2.1.5/setup.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-05 12:20:50.913275 unitlab-2.1.5/src/
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-05 12:20:50.913275 unitlab-2.1.5/src/unitlab/
+-rw-rw-r--   0 me        (1000) me        (1000)      214 2024-04-05 11:53:23.000000 unitlab-2.1.5/src/unitlab/__init__.py
+-rw-rw-r--   0 me        (1000) me        (1000)       29 2024-03-06 15:43:31.000000 unitlab-2.1.5/src/unitlab/__main__.py
+-rw-rw-r--   0 me        (1000) me        (1000)    12057 2024-04-05 09:59:24.000000 unitlab-2.1.5/src/unitlab/client.py
+-rw-rw-r--   0 me        (1000) me        (1000)    12386 2024-04-05 09:59:30.000000 unitlab-2.1.5/src/unitlab/dataset.py
+-rw-rw-r--   0 me        (1000) me        (1000)      950 2024-04-05 12:19:27.000000 unitlab-2.1.5/src/unitlab/exceptions.py
+-rw-rw-r--   0 me        (1000) me        (1000)     4513 2024-04-05 12:20:03.000000 unitlab-2.1.5/src/unitlab/main.py
+-rw-rw-r--   0 me        (1000) me        (1000)     1852 2024-04-05 12:20:07.000000 unitlab-2.1.5/src/unitlab/utils.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-05 12:20:50.913275 unitlab-2.1.5/src/unitlab.egg-info/
+-rw-r--r--   0 me        (1000) me        (1000)      793 2024-04-05 12:20:50.000000 unitlab-2.1.5/src/unitlab.egg-info/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)      411 2024-04-05 12:20:50.000000 unitlab-2.1.5/src/unitlab.egg-info/SOURCES.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        1 2024-04-05 12:20:50.000000 unitlab-2.1.5/src/unitlab.egg-info/dependency_links.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       45 2024-04-05 12:20:50.000000 unitlab-2.1.5/src/unitlab.egg-info/entry_points.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       48 2024-04-05 12:20:50.000000 unitlab-2.1.5/src/unitlab.egg-info/requires.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        8 2024-04-05 12:20:50.000000 unitlab-2.1.5/src/unitlab.egg-info/top_level.txt
```

### Comparing `unitlab-2.1.4/LICENSE.md` & `unitlab-2.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unitlab-2.1.4/PKG-INFO` & `unitlab-2.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: unitlab
-Version: 2.1.4
+Version: 2.1.5
 Home-page: https://github.com/teamunitlab/unitlab-sdk
 Author: Unitlab Inc.
 Author-email: team@unitlab.ai
 License: MIT
 Keywords: unitlab-sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE.md
 Requires-Dist: aiohttp
```

### Comparing `unitlab-2.1.4/README.md` & `unitlab-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `unitlab-2.1.4/setup.py` & `unitlab-2.1.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from setuptools import find_packages, setup
 
 setup(
     name="unitlab",
-    version="2.1.4",
+    version="2.1.5",
     license="MIT",
     author="Unitlab Inc.",
     author_email="team@unitlab.ai",
     packages=find_packages("src"),
     include_package_data=True,
     package_data={"static": ["*"], "Potato": ["*.so"]},
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
     package_dir={"": "src"},
```

### Comparing `unitlab-2.1.4/src/unitlab/client.py` & `unitlab-2.1.5/src/unitlab/client.py`

 * *Files identical despite different names*

### Comparing `unitlab-2.1.4/src/unitlab/dataset.py` & `unitlab-2.1.5/src/unitlab/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,17 +282,14 @@
 
     def get_img_line_payload(self, anns):
         return self.get_img_semantic_segmentation_payload(anns)
 
     def get_img_point_payload(self, anns):
         return self.get_img_semantic_segmentation_payload(anns)
 
-    def get_img_skeleton_payload(self, anns):
-        logger.warning("Not implemented yet")
-
     def get_payload(self, img_id):
         image = self.imgs[img_id]
         ann_ids = self.getAnnIds(imgIds=img_id)
         anns = self.loadAnns(ann_ids)
         if not os.path.isfile(os.path.join(self.data_path, image["file_name"])):
             logger.warning(
                 "Image file not found: {}".format(
```

### Comparing `unitlab-2.1.4/src/unitlab/exceptions.py` & `unitlab-2.1.5/src/unitlab/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
     def __init__(self, message: str, detail: Optional[Exception] = None):
         """
         Args:
             message: An informative message about the exception.
             detail: The detail of the exception raised by Python or another library. Defaults to :obj:`None`.
         """
-
         super().__init__(message, detail)
         self.message = message
         self.detail = detail
 
     def __str__(self) -> str:
         return self.message
```

### Comparing `unitlab-2.1.4/src/unitlab/main.py` & `unitlab-2.1.5/src/unitlab/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 class AnnotationType(str, Enum):
     IMG_BBOX = "img_bbox"
     IMG_SEMANTIC_SEGMENTATION = "img_semantic_segmentation"
     IMG_INSTANCE_SEGMENTATION = "img_instance_segmentation"
     IMG_POLYGON = "img_polygon"
     IMG_LINE = "img_line"
     IMG_POINT = "img_point"
-    IMG_SKELETON = "img_skeleton"
 
 
 @app.command()
 def configure(
     api_key: Annotated[str, typer.Option(help="The api-key obtained from unitlab.ai")],
     api_url: Annotated[str, typer.Option()] = "https://api.unitlab.ai",
 ):
```

### Comparing `unitlab-2.1.4/src/unitlab/utils.py` & `unitlab-2.1.5/src/unitlab/utils.py`

 * *Files identical despite different names*

### Comparing `unitlab-2.1.4/src/unitlab.egg-info/PKG-INFO` & `unitlab-2.1.5/src/unitlab.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: unitlab
-Version: 2.1.4
+Version: 2.1.5
 Home-page: https://github.com/teamunitlab/unitlab-sdk
 Author: Unitlab Inc.
 Author-email: team@unitlab.ai
 License: MIT
 Keywords: unitlab-sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE.md
 Requires-Dist: aiohttp
```

