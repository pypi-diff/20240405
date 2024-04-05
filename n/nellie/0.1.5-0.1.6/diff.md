# Comparing `tmp/nellie-0.1.5.tar.gz` & `tmp/nellie-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nellie-0.1.5.tar", last modified: Mon Apr  1 22:22:07 2024, max compression
+gzip compressed data, was "nellie-0.1.6.tar", last modified: Fri Apr  5 16:01:00 2024, max compression
```

## Comparing `nellie-0.1.5.tar` & `nellie-0.1.6.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-01 22:22:07.366368 nellie-0.1.5/
--rw-r--r--   0 austin     (501) staff       (20)    18826 2024-03-19 19:14:37.000000 nellie-0.1.5/LICENSE
--rw-r--r--   0 austin     (501) staff       (20)    11211 2024-04-01 22:22:07.366221 nellie-0.1.5/PKG-INFO
--rw-r--r--   0 austin     (501) staff       (20)    10555 2024-03-23 00:41:03.000000 nellie-0.1.5/README.md
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-01 22:22:07.355267 nellie-0.1.5/nellie/
--rw-r--r--   0 austin     (501) staff       (20)     1421 2024-03-15 22:18:53.000000 nellie-0.1.5/nellie/__init__.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-01 22:22:07.356464 nellie-0.1.5/nellie/feature_extraction/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.5/nellie/feature_extraction/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)    54414 2024-04-01 21:48:11.000000 nellie-0.1.5/nellie/feature_extraction/hierarchical.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-01 22:22:07.356809 nellie-0.1.5/nellie/im_info/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.5/nellie/im_info/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)    16203 2024-04-01 22:05:10.000000 nellie-0.1.5/nellie/im_info/im_info.py
--rw-r--r--   0 austin     (501) staff       (20)     1774 2024-04-01 22:21:40.000000 nellie-0.1.5/nellie/run.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-01 22:22:07.358078 nellie-0.1.5/nellie/segmentation/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.5/nellie/segmentation/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)    11578 2024-03-15 22:18:53.000000 nellie-0.1.5/nellie/segmentation/filtering.py
--rw-r--r--   0 austin     (501) staff       (20)     6487 2024-03-15 22:18:53.000000 nellie-0.1.5/nellie/segmentation/labelling.py
--rw-r--r--   0 austin     (501) staff       (20)     9769 2024-04-01 17:29:51.000000 nellie-0.1.5/nellie/segmentation/mocap_marking.py
--rw-r--r--   0 austin     (501) staff       (20)    16823 2024-03-15 22:18:53.000000 nellie-0.1.5/nellie/segmentation/networking.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-01 22:22:07.359621 nellie-0.1.5/nellie/tracking/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.5/nellie/tracking/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)     4743 2024-03-23 00:41:03.000000 nellie-0.1.5/nellie/tracking/all_tracks_for_label.py
--rw-r--r--   0 austin     (501) staff       (20)    11441 2024-04-01 16:16:45.000000 nellie-0.1.5/nellie/tracking/flow_interpolation.py
--rw-r--r--   0 austin     (501) staff       (20)    17974 2024-04-01 16:16:45.000000 nellie-0.1.5/nellie/tracking/hu_tracking.py
--rw-r--r--   0 austin     (501) staff       (20)    19639 2024-04-01 16:16:45.000000 nellie-0.1.5/nellie/tracking/voxel_reassignment.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-01 22:22:07.360859 nellie-0.1.5/nellie/utils/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.5/nellie/utils/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)      275 2024-03-15 22:13:16.000000 nellie-0.1.5/nellie/utils/base_logger.py
--rw-r--r--   0 austin     (501) staff       (20)     1572 2024-04-01 21:26:56.000000 nellie-0.1.5/nellie/utils/general.py
--rw-r--r--   0 austin     (501) staff       (20)     2594 2024-03-15 22:18:53.000000 nellie-0.1.5/nellie/utils/gpu_functions.py
--rw-r--r--   0 austin     (501) staff       (20)     5892 2024-03-15 22:13:16.000000 nellie-0.1.5/nellie/utils/torch_xp.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-01 22:22:07.365859 nellie-0.1.5/nellie.egg-info/
--rw-r--r--   0 austin     (501) staff       (20)    11211 2024-04-01 22:22:07.000000 nellie-0.1.5/nellie.egg-info/PKG-INFO
--rw-r--r--   0 austin     (501) staff       (20)     1253 2024-04-01 22:22:07.000000 nellie-0.1.5/nellie.egg-info/SOURCES.txt
--rw-r--r--   0 austin     (501) staff       (20)        1 2024-04-01 22:22:07.000000 nellie-0.1.5/nellie.egg-info/dependency_links.txt
--rw-r--r--   0 austin     (501) staff       (20)       53 2024-04-01 22:22:07.000000 nellie-0.1.5/nellie.egg-info/entry_points.txt
--rw-r--r--   0 austin     (501) staff       (20)      121 2024-04-01 22:22:07.000000 nellie-0.1.5/nellie.egg-info/requires.txt
--rw-r--r--   0 austin     (501) staff       (20)       27 2024-04-01 22:22:07.000000 nellie-0.1.5/nellie.egg-info/top_level.txt
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-01 22:22:07.364274 nellie-0.1.5/nellie_napari/
--rw-r--r--   0 austin     (501) staff       (20)      112 2024-03-18 21:13:24.000000 nellie-0.1.5/nellie_napari/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)     8386 2024-03-19 15:37:36.000000 nellie-0.1.5/nellie_napari/batch_mode.py
--rw-r--r--   0 austin     (501) staff       (20)     3595 2024-03-23 00:44:38.000000 nellie-0.1.5/nellie_napari/home.py
--rw-r--r--   0 austin     (501) staff       (20)    89016 2024-03-19 16:27:20.000000 nellie-0.1.5/nellie_napari/logo.png
--rw-r--r--   0 austin     (501) staff       (20)      218 2024-03-15 22:32:30.000000 nellie-0.1.5/nellie_napari/napari.yaml
--rw-r--r--   0 austin     (501) staff       (20)    20913 2024-03-19 21:11:06.000000 nellie-0.1.5/nellie_napari/nellie_analysis.py
--rw-r--r--   0 austin     (501) staff       (20)    16190 2024-03-19 18:53:00.000000 nellie-0.1.5/nellie_napari/nellie_fileselect.py
--rw-r--r--   0 austin     (501) staff       (20)     2719 2024-03-19 01:57:46.000000 nellie-0.1.5/nellie_napari/nellie_loader.py
--rw-r--r--   0 austin     (501) staff       (20)    15621 2024-04-01 16:16:45.000000 nellie-0.1.5/nellie_napari/nellie_processor.py
--rw-r--r--   0 austin     (501) staff       (20)    12833 2024-03-19 16:50:50.000000 nellie-0.1.5/nellie_napari/visualizer.py
--rw-r--r--   0 austin     (501) staff       (20)       90 2024-01-23 18:46:05.000000 nellie-0.1.5/pyproject.toml
--rw-r--r--   0 austin     (501) staff       (20)      816 2024-04-01 22:22:07.366691 nellie-0.1.5/setup.cfg
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-01 22:22:07.364757 nellie-0.1.5/tests/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.5/tests/__init__.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-01 22:22:07.365406 nellie-0.1.5/tests/unit/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.5/tests/unit/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)        6 2024-03-15 22:13:16.000000 nellie-0.1.5/tests/unit/test_frangi_filter.py
--rw-r--r--   0 austin     (501) staff       (20)     3310 2024-03-15 22:18:53.000000 nellie-0.1.5/tests/unit/test_im_info.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-05 16:01:00.616237 nellie-0.1.6/
+-rw-r--r--   0 austin     (501) staff       (20)    18826 2024-03-19 19:14:37.000000 nellie-0.1.6/LICENSE
+-rw-r--r--   0 austin     (501) staff       (20)    11217 2024-04-05 16:01:00.616082 nellie-0.1.6/PKG-INFO
+-rw-r--r--   0 austin     (501) staff       (20)    10555 2024-03-23 00:41:03.000000 nellie-0.1.6/README.md
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-05 16:01:00.603968 nellie-0.1.6/nellie/
+-rw-r--r--   0 austin     (501) staff       (20)     1421 2024-03-15 22:18:53.000000 nellie-0.1.6/nellie/__init__.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-05 16:01:00.605241 nellie-0.1.6/nellie/feature_extraction/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.6/nellie/feature_extraction/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)    54414 2024-04-01 21:48:11.000000 nellie-0.1.6/nellie/feature_extraction/hierarchical.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-05 16:01:00.606000 nellie-0.1.6/nellie/im_info/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.6/nellie/im_info/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)    16203 2024-04-01 22:05:10.000000 nellie-0.1.6/nellie/im_info/im_info.py
+-rw-r--r--   0 austin     (501) staff       (20)     1774 2024-04-01 22:21:40.000000 nellie-0.1.6/nellie/run.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-05 16:01:00.607393 nellie-0.1.6/nellie/segmentation/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.6/nellie/segmentation/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)    11578 2024-03-15 22:18:53.000000 nellie-0.1.6/nellie/segmentation/filtering.py
+-rw-r--r--   0 austin     (501) staff       (20)     6487 2024-03-15 22:18:53.000000 nellie-0.1.6/nellie/segmentation/labelling.py
+-rw-r--r--   0 austin     (501) staff       (20)     9769 2024-04-01 17:29:51.000000 nellie-0.1.6/nellie/segmentation/mocap_marking.py
+-rw-r--r--   0 austin     (501) staff       (20)    16823 2024-03-15 22:18:53.000000 nellie-0.1.6/nellie/segmentation/networking.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-05 16:01:00.609019 nellie-0.1.6/nellie/tracking/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.6/nellie/tracking/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)     4743 2024-03-23 00:41:03.000000 nellie-0.1.6/nellie/tracking/all_tracks_for_label.py
+-rw-r--r--   0 austin     (501) staff       (20)    11441 2024-04-01 16:16:45.000000 nellie-0.1.6/nellie/tracking/flow_interpolation.py
+-rw-r--r--   0 austin     (501) staff       (20)    17974 2024-04-01 16:16:45.000000 nellie-0.1.6/nellie/tracking/hu_tracking.py
+-rw-r--r--   0 austin     (501) staff       (20)    19639 2024-04-01 16:16:45.000000 nellie-0.1.6/nellie/tracking/voxel_reassignment.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-05 16:01:00.610269 nellie-0.1.6/nellie/utils/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.6/nellie/utils/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)      275 2024-03-15 22:13:16.000000 nellie-0.1.6/nellie/utils/base_logger.py
+-rw-r--r--   0 austin     (501) staff       (20)     1572 2024-04-01 21:26:56.000000 nellie-0.1.6/nellie/utils/general.py
+-rw-r--r--   0 austin     (501) staff       (20)     2594 2024-03-15 22:18:53.000000 nellie-0.1.6/nellie/utils/gpu_functions.py
+-rw-r--r--   0 austin     (501) staff       (20)     5892 2024-03-15 22:13:16.000000 nellie-0.1.6/nellie/utils/torch_xp.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-05 16:01:00.615721 nellie-0.1.6/nellie.egg-info/
+-rw-r--r--   0 austin     (501) staff       (20)    11217 2024-04-05 16:01:00.000000 nellie-0.1.6/nellie.egg-info/PKG-INFO
+-rw-r--r--   0 austin     (501) staff       (20)     1253 2024-04-05 16:01:00.000000 nellie-0.1.6/nellie.egg-info/SOURCES.txt
+-rw-r--r--   0 austin     (501) staff       (20)        1 2024-04-05 16:01:00.000000 nellie-0.1.6/nellie.egg-info/dependency_links.txt
+-rw-r--r--   0 austin     (501) staff       (20)       53 2024-04-05 16:01:00.000000 nellie-0.1.6/nellie.egg-info/entry_points.txt
+-rw-r--r--   0 austin     (501) staff       (20)      127 2024-04-05 16:01:00.000000 nellie-0.1.6/nellie.egg-info/requires.txt
+-rw-r--r--   0 austin     (501) staff       (20)       27 2024-04-05 16:01:00.000000 nellie-0.1.6/nellie.egg-info/top_level.txt
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-05 16:01:00.614243 nellie-0.1.6/nellie_napari/
+-rw-r--r--   0 austin     (501) staff       (20)      112 2024-03-18 21:13:24.000000 nellie-0.1.6/nellie_napari/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)     8386 2024-03-19 15:37:36.000000 nellie-0.1.6/nellie_napari/batch_mode.py
+-rw-r--r--   0 austin     (501) staff       (20)     3595 2024-03-23 00:44:38.000000 nellie-0.1.6/nellie_napari/home.py
+-rw-r--r--   0 austin     (501) staff       (20)    89016 2024-03-19 16:27:20.000000 nellie-0.1.6/nellie_napari/logo.png
+-rw-r--r--   0 austin     (501) staff       (20)      218 2024-03-15 22:32:30.000000 nellie-0.1.6/nellie_napari/napari.yaml
+-rw-r--r--   0 austin     (501) staff       (20)    20913 2024-03-19 21:11:06.000000 nellie-0.1.6/nellie_napari/nellie_analysis.py
+-rw-r--r--   0 austin     (501) staff       (20)    16190 2024-03-19 18:53:00.000000 nellie-0.1.6/nellie_napari/nellie_fileselect.py
+-rw-r--r--   0 austin     (501) staff       (20)     2719 2024-03-19 01:57:46.000000 nellie-0.1.6/nellie_napari/nellie_loader.py
+-rw-r--r--   0 austin     (501) staff       (20)    15621 2024-04-01 16:16:45.000000 nellie-0.1.6/nellie_napari/nellie_processor.py
+-rw-r--r--   0 austin     (501) staff       (20)    12833 2024-03-19 16:50:50.000000 nellie-0.1.6/nellie_napari/visualizer.py
+-rw-r--r--   0 austin     (501) staff       (20)       90 2024-01-23 18:46:05.000000 nellie-0.1.6/pyproject.toml
+-rw-r--r--   0 austin     (501) staff       (20)      822 2024-04-05 16:01:00.616549 nellie-0.1.6/setup.cfg
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-05 16:01:00.614682 nellie-0.1.6/tests/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.6/tests/__init__.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-05 16:01:00.615264 nellie-0.1.6/tests/unit/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.6/tests/unit/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)        6 2024-03-15 22:13:16.000000 nellie-0.1.6/tests/unit/test_frangi_filter.py
+-rw-r--r--   0 austin     (501) staff       (20)     3310 2024-03-15 22:18:53.000000 nellie-0.1.6/tests/unit/test_im_info.py
```

### Comparing `nellie-0.1.5/LICENSE` & `nellie-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nellie-0.1.5/PKG-INFO` & `nellie-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: nellie
-Version: 0.1.5
+Version: 0.1.6
 Summary: Automated organelle segmentation, tracking, and hierarchical feature extraction in 2D/3D live-cell microscopy
 Home-page: https://github.com/aelefebv/nellie
 Author: Austin E. Y. T. Lefebvre
 Author-email: austin.e.lefebvre+nellie@gmail.com
 Classifier: Framework :: napari
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.26.4
 Requires-Dist: scipy==1.12.0
 Requires-Dist: scikit-image==0.22.0
 Requires-Dist: nd2==0.9.0
-Requires-Dist: ome-types==0.5.0
+Requires-Dist: ome-types==0.5.1.post1
 Requires-Dist: pandas==2.2.1
 Requires-Dist: matplotlib==3.8.3
 Requires-Dist: napari[all]
 
 # Nellie
 ## Automated organelle segmentation, tracking, and hierarchical feature extraction in 2D/3D live-cell microscopy
```

### Comparing `nellie-0.1.5/README.md` & `nellie-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `nellie-0.1.5/nellie/__init__.py` & `nellie-0.1.6/nellie/__init__.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.5/nellie/feature_extraction/hierarchical.py` & `nellie-0.1.6/nellie/feature_extraction/hierarchical.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.5/nellie/im_info/im_info.py` & `nellie-0.1.6/nellie/im_info/im_info.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.5/nellie/run.py` & `nellie-0.1.6/nellie/run.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.5/nellie/segmentation/filtering.py` & `nellie-0.1.6/nellie/segmentation/filtering.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.5/nellie/segmentation/labelling.py` & `nellie-0.1.6/nellie/segmentation/labelling.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.5/nellie/segmentation/mocap_marking.py` & `nellie-0.1.6/nellie/segmentation/mocap_marking.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.5/nellie/segmentation/networking.py` & `nellie-0.1.6/nellie/segmentation/networking.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.5/nellie/tracking/all_tracks_for_label.py` & `nellie-0.1.6/nellie/tracking/all_tracks_for_label.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.5/nellie/tracking/flow_interpolation.py` & `nellie-0.1.6/nellie/tracking/flow_interpolation.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.5/nellie/tracking/hu_tracking.py` & `nellie-0.1.6/nellie/tracking/hu_tracking.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.5/nellie/tracking/voxel_reassignment.py` & `nellie-0.1.6/nellie/tracking/voxel_reassignment.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.5/nellie/utils/general.py` & `nellie-0.1.6/nellie/utils/general.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.5/nellie/utils/gpu_functions.py` & `nellie-0.1.6/nellie/utils/gpu_functions.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.5/nellie/utils/torch_xp.py` & `nellie-0.1.6/nellie/utils/torch_xp.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.5/nellie.egg-info/PKG-INFO` & `nellie-0.1.6/nellie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: nellie
-Version: 0.1.5
+Version: 0.1.6
 Summary: Automated organelle segmentation, tracking, and hierarchical feature extraction in 2D/3D live-cell microscopy
 Home-page: https://github.com/aelefebv/nellie
 Author: Austin E. Y. T. Lefebvre
 Author-email: austin.e.lefebvre+nellie@gmail.com
 Classifier: Framework :: napari
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.26.4
 Requires-Dist: scipy==1.12.0
 Requires-Dist: scikit-image==0.22.0
 Requires-Dist: nd2==0.9.0
-Requires-Dist: ome-types==0.5.0
+Requires-Dist: ome-types==0.5.1.post1
 Requires-Dist: pandas==2.2.1
 Requires-Dist: matplotlib==3.8.3
 Requires-Dist: napari[all]
 
 # Nellie
 ## Automated organelle segmentation, tracking, and hierarchical feature extraction in 2D/3D live-cell microscopy
```

### Comparing `nellie-0.1.5/nellie.egg-info/SOURCES.txt` & `nellie-0.1.6/nellie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nellie-0.1.5/nellie_napari/batch_mode.py` & `nellie-0.1.6/nellie_napari/batch_mode.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.5/nellie_napari/home.py` & `nellie-0.1.6/nellie_napari/home.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.5/nellie_napari/logo.png` & `nellie-0.1.6/nellie_napari/logo.png`

 * *Files identical despite different names*

### Comparing `nellie-0.1.5/nellie_napari/nellie_analysis.py` & `nellie-0.1.6/nellie_napari/nellie_analysis.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.5/nellie_napari/nellie_fileselect.py` & `nellie-0.1.6/nellie_napari/nellie_fileselect.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.5/nellie_napari/nellie_loader.py` & `nellie-0.1.6/nellie_napari/nellie_loader.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.5/nellie_napari/nellie_processor.py` & `nellie-0.1.6/nellie_napari/nellie_processor.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.5/nellie_napari/visualizer.py` & `nellie-0.1.6/nellie_napari/visualizer.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.5/setup.cfg` & `nellie-0.1.6/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nellie
-version = 0.1.5
+version = 0.1.6
 description = Automated organelle segmentation, tracking, and hierarchical feature extraction in 2D/3D live-cell microscopy
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Austin E. Y. T. Lefebvre
 author_email = austin.e.lefebvre+nellie@gmail.com
 url = https://github.com/aelefebv/nellie
 classifiers = 
@@ -14,15 +14,15 @@
 packages = find:
 python_requires = >=3.9
 install_requires = 
 	numpy==1.26.4
 	scipy==1.12.0
 	scikit-image==0.22.0
 	nd2==0.9.0
-	ome-types==0.5.0
+	ome-types==0.5.1.post1
 	pandas==2.2.1
 	matplotlib==3.8.3
 	napari[all]
 include_package_data = True
 
 [options.package_data]
 nellie_napari = napari.yaml, logo.png
```

### Comparing `nellie-0.1.5/tests/unit/test_im_info.py` & `nellie-0.1.6/tests/unit/test_im_info.py`

 * *Files identical despite different names*

