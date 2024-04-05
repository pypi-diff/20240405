# Comparing `tmp/prusek_spheroid-3.8.tar.gz` & `tmp/prusek_spheroid-3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prusek_spheroid-3.8.tar", last modified: Thu Apr  4 18:50:00 2024, max compression
+gzip compressed data, was "prusek_spheroid-3.9.tar", last modified: Thu Apr  4 18:51:08 2024, max compression
```

## Comparing `prusek_spheroid-3.8.tar` & `prusek_spheroid-3.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-04 18:50:00.502385 prusek_spheroid-3.8/
--rw-r--r--   0 michalprusek   (501) staff       (20)     9069 2024-04-04 18:50:00.502148 prusek_spheroid-3.8/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)     8544 2024-03-27 11:29:11.000000 prusek_spheroid-3.8/README.md
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-04 18:50:00.500697 prusek_spheroid-3.8/prusek_spheroid/
--rw-r--r--   0 michalprusek   (501) staff       (20)    17332 2024-04-04 17:31:23.000000 prusek_spheroid-3.8/prusek_spheroid/ContoursClassGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    50417 2024-04-04 18:36:20.000000 prusek_spheroid-3.8/prusek_spheroid/GUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    12427 2024-03-22 06:33:48.000000 prusek_spheroid-3.8/prusek_spheroid/GradientDescentGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-3.8/prusek_spheroid/characteristic_functions.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-3.8/prusek_spheroid/conversion.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     7199 2024-04-04 16:33:02.000000 prusek_spheroid-3.8/prusek_spheroid/file_management.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     6737 2024-04-04 14:40:14.000000 prusek_spheroid-3.8/prusek_spheroid/image_processing.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     2555 2024-04-04 18:44:25.000000 prusek_spheroid-3.8/prusek_spheroid/merge_directories.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     3641 2024-04-03 14:52:18.000000 prusek_spheroid-3.8/prusek_spheroid/methods.py
--rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-3.8/prusek_spheroid/metrics.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-3.8/prusek_spheroid/selection_dialog.py
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-04 18:50:00.501802 prusek_spheroid-3.8/prusek_spheroid.egg-info/
--rw-r--r--   0 michalprusek   (501) staff       (20)     9069 2024-04-04 18:50:00.000000 prusek_spheroid-3.8/prusek_spheroid.egg-info/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-04 18:50:00.000000 prusek_spheroid-3.8/prusek_spheroid.egg-info/SOURCES.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-04 18:50:00.000000 prusek_spheroid-3.8/prusek_spheroid.egg-info/dependency_links.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)      110 2024-04-04 18:50:00.000000 prusek_spheroid-3.8/prusek_spheroid.egg-info/requires.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-04 18:50:00.000000 prusek_spheroid-3.8/prusek_spheroid.egg-info/top_level.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-04 18:50:00.502501 prusek_spheroid-3.8/setup.cfg
--rw-r--r--   0 michalprusek   (501) staff       (20)      729 2024-04-04 18:49:57.000000 prusek_spheroid-3.8/setup.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-04 18:51:08.652334 prusek_spheroid-3.9/
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9094 2024-04-04 18:51:08.652067 prusek_spheroid-3.9/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)     8544 2024-03-27 11:29:11.000000 prusek_spheroid-3.9/README.md
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-04 18:51:08.650580 prusek_spheroid-3.9/prusek_spheroid/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    17332 2024-04-04 17:31:23.000000 prusek_spheroid-3.9/prusek_spheroid/ContoursClassGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    50417 2024-04-04 18:36:20.000000 prusek_spheroid-3.9/prusek_spheroid/GUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    12427 2024-03-22 06:33:48.000000 prusek_spheroid-3.9/prusek_spheroid/GradientDescentGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-3.9/prusek_spheroid/characteristic_functions.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-3.9/prusek_spheroid/conversion.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     7199 2024-04-04 16:33:02.000000 prusek_spheroid-3.9/prusek_spheroid/file_management.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     6737 2024-04-04 14:40:14.000000 prusek_spheroid-3.9/prusek_spheroid/image_processing.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     2555 2024-04-04 18:44:25.000000 prusek_spheroid-3.9/prusek_spheroid/merge_directories.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     3641 2024-04-03 14:52:18.000000 prusek_spheroid-3.9/prusek_spheroid/methods.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-3.9/prusek_spheroid/metrics.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-3.9/prusek_spheroid/selection_dialog.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-04 18:51:08.651699 prusek_spheroid-3.9/prusek_spheroid.egg-info/
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9094 2024-04-04 18:51:08.000000 prusek_spheroid-3.9/prusek_spheroid.egg-info/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-04 18:51:08.000000 prusek_spheroid-3.9/prusek_spheroid.egg-info/SOURCES.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-04 18:51:08.000000 prusek_spheroid-3.9/prusek_spheroid.egg-info/dependency_links.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)      120 2024-04-04 18:51:08.000000 prusek_spheroid-3.9/prusek_spheroid.egg-info/requires.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-04 18:51:08.000000 prusek_spheroid-3.9/prusek_spheroid.egg-info/top_level.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-04 18:51:08.652456 prusek_spheroid-3.9/setup.cfg
+-rw-r--r--   0 michalprusek   (501) staff       (20)      750 2024-04-04 18:50:55.000000 prusek_spheroid-3.9/setup.py
```

### Comparing `prusek_spheroid-3.8/PKG-INFO` & `prusek_spheroid-3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 3.8
+Version: 3.9
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
@@ -13,14 +13,15 @@
 Requires-Dist: shapely
 Requires-Dist: threadpoolctl
 Requires-Dist: matplotlib
 Requires-Dist: rasterio
 Requires-Dist: pandas
 Requires-Dist: openpyxl
 Requires-Dist: torch
+Requires-Dist: imagehash
 
 # Prusek-Spheroid
 
 Prusek-Spheroid is a Python package designed for spheroid segmentation based on provided microscope images. This package provides an easy-to-use interface and functionalities that are essential for determination of properties and characteristics of the spheroids.
 
 ## Installation
```

### Comparing `prusek_spheroid-3.8/README.md` & `prusek_spheroid-3.9/README.md`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.8/prusek_spheroid/ContoursClassGUI.py` & `prusek_spheroid-3.9/prusek_spheroid/ContoursClassGUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.8/prusek_spheroid/GUI.py` & `prusek_spheroid-3.9/prusek_spheroid/GUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.8/prusek_spheroid/GradientDescentGUI.py` & `prusek_spheroid-3.9/prusek_spheroid/GradientDescentGUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.8/prusek_spheroid/characteristic_functions.py` & `prusek_spheroid-3.9/prusek_spheroid/characteristic_functions.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.8/prusek_spheroid/conversion.py` & `prusek_spheroid-3.9/prusek_spheroid/conversion.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.8/prusek_spheroid/file_management.py` & `prusek_spheroid-3.9/prusek_spheroid/file_management.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.8/prusek_spheroid/image_processing.py` & `prusek_spheroid-3.9/prusek_spheroid/image_processing.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.8/prusek_spheroid/merge_directories.py` & `prusek_spheroid-3.9/prusek_spheroid/merge_directories.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.8/prusek_spheroid/methods.py` & `prusek_spheroid-3.9/prusek_spheroid/methods.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.8/prusek_spheroid/metrics.py` & `prusek_spheroid-3.9/prusek_spheroid/metrics.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.8/prusek_spheroid/selection_dialog.py` & `prusek_spheroid-3.9/prusek_spheroid/selection_dialog.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.8/prusek_spheroid.egg-info/PKG-INFO` & `prusek_spheroid-3.9/prusek_spheroid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 3.8
+Version: 3.9
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
@@ -13,14 +13,15 @@
 Requires-Dist: shapely
 Requires-Dist: threadpoolctl
 Requires-Dist: matplotlib
 Requires-Dist: rasterio
 Requires-Dist: pandas
 Requires-Dist: openpyxl
 Requires-Dist: torch
+Requires-Dist: imagehash
 
 # Prusek-Spheroid
 
 Prusek-Spheroid is a Python package designed for spheroid segmentation based on provided microscope images. This package provides an easy-to-use interface and functionalities that are essential for determination of properties and characteristics of the spheroids.
 
 ## Installation
```

### Comparing `prusek_spheroid-3.8/prusek_spheroid.egg-info/SOURCES.txt` & `prusek_spheroid-3.9/prusek_spheroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.8/setup.py` & `prusek_spheroid-3.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="prusek_spheroid",
-    version="3.8",
+    version="3.9",
     description="Spheroid segmentation package",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Michal Prusek",
     author_email="prusemic@cvut.cz",
     url="https://github.com/michalprusek/prusek-spheroid",
     packages=["prusek_spheroid"],
@@ -20,10 +20,11 @@
         'scikit-learn',
         'shapely',
         'threadpoolctl',
         'matplotlib',
         'rasterio',
         'pandas',
         'openpyxl',
-        'torch'
+        'torch',
+        'imagehash'
     ],
 )
```

