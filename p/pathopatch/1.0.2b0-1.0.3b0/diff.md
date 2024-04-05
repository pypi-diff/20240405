# Comparing `tmp/pathopatch-1.0.2b0.tar.gz` & `tmp/pathopatch-1.0.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathopatch-1.0.2b0.tar", last modified: Wed Apr  3 14:44:29 2024, max compression
+gzip compressed data, was "pathopatch-1.0.3b0.tar", last modified: Fri Apr  5 14:09:40 2024, max compression
```

## Comparing `pathopatch-1.0.2b0.tar` & `pathopatch-1.0.3b0.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-03 14:44:29.693850 pathopatch-1.0.2b0/
--rw-r--r--   0 fhoerst    (501) staff       (20)     1184 2024-03-26 16:01:10.000000 pathopatch-1.0.2b0/LICENSE.md
--rw-r--r--   0 fhoerst    (501) staff       (20)    18127 2024-04-03 14:44:29.693473 pathopatch-1.0.2b0/PKG-INFO
--rw-r--r--   0 fhoerst    (501) staff       (20)    23383 2024-04-02 13:00:08.000000 pathopatch-1.0.2b0/README.md
-drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-03 14:44:29.678562 pathopatch-1.0.2b0/pathopatch/
--rw-r--r--   0 fhoerst    (501) staff       (20)       96 2024-01-12 12:43:51.000000 pathopatch-1.0.2b0/pathopatch/__init__.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     5013 2024-01-12 12:43:51.000000 pathopatch-1.0.2b0/pathopatch/annotation_conversion.py
-drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-03 14:44:29.679790 pathopatch-1.0.2b0/pathopatch/base_ml/
--rw-r--r--   0 fhoerst    (501) staff       (20)        0 2024-01-12 12:43:51.000000 pathopatch-1.0.2b0/pathopatch/base_ml/__init__.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     4541 2024-01-12 12:43:51.000000 pathopatch-1.0.2b0/pathopatch/base_ml/base_cli.py
--rw-r--r--   0 fhoerst    (501) staff       (20)    39568 2024-04-02 12:25:57.000000 pathopatch-1.0.2b0/pathopatch/cli.py
-drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-03 14:44:29.680458 pathopatch-1.0.2b0/pathopatch/config/
--rw-r--r--   0 fhoerst    (501) staff       (20)       96 2024-01-12 12:43:51.000000 pathopatch-1.0.2b0/pathopatch/config/__init__.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     1428 2024-04-02 12:25:57.000000 pathopatch-1.0.2b0/pathopatch/config/config.py
-drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-03 14:44:29.684603 pathopatch-1.0.2b0/pathopatch/data/
--rw-r--r--   0 fhoerst    (501) staff       (20)       96 2024-01-12 12:43:51.000000 pathopatch-1.0.2b0/pathopatch/data/__init__.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     1165 2024-01-12 12:43:52.000000 pathopatch-1.0.2b0/pathopatch/macenko_vector_generation.py
-drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-03 14:44:29.686143 pathopatch-1.0.2b0/pathopatch/patch_extraction/
--rw-r--r--   0 fhoerst    (501) staff       (20)       96 2024-01-12 12:43:52.000000 pathopatch-1.0.2b0/pathopatch/patch_extraction/__init__.py
--rw-r--r--   0 fhoerst    (501) staff       (20)    32674 2024-04-02 06:34:36.000000 pathopatch-1.0.2b0/pathopatch/patch_extraction/dataset.py
--rw-r--r--   0 fhoerst    (501) staff       (20)    63509 2024-04-02 12:25:59.000000 pathopatch-1.0.2b0/pathopatch/patch_extraction/patch_extraction.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     9676 2024-04-02 12:25:58.000000 pathopatch-1.0.2b0/pathopatch/patch_extraction/process_batch.py
--rw-r--r--   0 fhoerst    (501) staff       (20)    12265 2024-01-12 12:43:52.000000 pathopatch-1.0.2b0/pathopatch/patch_extraction/storage.py
-drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-03 14:44:29.689655 pathopatch-1.0.2b0/pathopatch/utils/
--rw-r--r--   0 fhoerst    (501) staff       (20)        0 2024-01-12 12:43:52.000000 pathopatch-1.0.2b0/pathopatch/utils/__init__.py
--rw-r--r--   0 fhoerst    (501) staff       (20)      608 2024-01-12 12:43:52.000000 pathopatch-1.0.2b0/pathopatch/utils/exceptions.py
--rw-r--r--   0 fhoerst    (501) staff       (20)      626 2024-01-12 12:43:52.000000 pathopatch-1.0.2b0/pathopatch/utils/file_handling.py
--rw-r--r--   0 fhoerst    (501) staff       (20)    13833 2024-03-26 16:01:13.000000 pathopatch-1.0.2b0/pathopatch/utils/filters.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     6334 2024-03-27 14:05:13.000000 pathopatch-1.0.2b0/pathopatch/utils/logger.py
--rw-r--r--   0 fhoerst    (501) staff       (20)    10801 2024-01-19 13:20:20.000000 pathopatch-1.0.2b0/pathopatch/utils/masking.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     3216 2024-01-12 12:43:52.000000 pathopatch-1.0.2b0/pathopatch/utils/patch_dataset.py
--rw-r--r--   0 fhoerst    (501) staff       (20)    46150 2024-04-02 12:25:58.000000 pathopatch-1.0.2b0/pathopatch/utils/patch_util.py
--rw-r--r--   0 fhoerst    (501) staff       (20)    10592 2024-01-12 12:43:52.000000 pathopatch-1.0.2b0/pathopatch/utils/plotting.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     7204 2024-01-12 12:43:52.000000 pathopatch-1.0.2b0/pathopatch/utils/tools.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     1066 2024-04-02 13:09:13.000000 pathopatch-1.0.2b0/pathopatch/wsi_extraction.py
-drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-03 14:44:29.690839 pathopatch-1.0.2b0/pathopatch/wsi_interfaces/
--rw-r--r--   0 fhoerst    (501) staff       (20)      387 2024-03-29 14:01:43.000000 pathopatch-1.0.2b0/pathopatch/wsi_interfaces/__init__.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     3115 2024-04-02 06:35:01.000000 pathopatch-1.0.2b0/pathopatch/wsi_interfaces/cucim_deepzoom.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     1318 2024-04-02 12:25:58.000000 pathopatch-1.0.2b0/pathopatch/wsi_interfaces/openslide_deepzoom.py
--rw-r--r--   0 fhoerst    (501) staff       (20)    10424 2024-04-03 14:41:27.000000 pathopatch-1.0.2b0/pathopatch/wsi_interfaces/wsidicomizer_openslide.py
-drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-03 14:44:29.693090 pathopatch-1.0.2b0/pathopatch.egg-info/
--rw-r--r--   0 fhoerst    (501) staff       (20)    18127 2024-04-03 14:44:29.000000 pathopatch-1.0.2b0/pathopatch.egg-info/PKG-INFO
--rw-r--r--   0 fhoerst    (501) staff       (20)     1817 2024-04-03 14:44:29.000000 pathopatch-1.0.2b0/pathopatch.egg-info/SOURCES.txt
--rw-r--r--   0 fhoerst    (501) staff       (20)        1 2024-04-03 14:44:29.000000 pathopatch-1.0.2b0/pathopatch.egg-info/dependency_links.txt
--rw-r--r--   0 fhoerst    (501) staff       (20)      198 2024-04-03 14:44:29.000000 pathopatch-1.0.2b0/pathopatch.egg-info/entry_points.txt
--rw-r--r--   0 fhoerst    (501) staff       (20)      297 2024-04-03 14:44:29.000000 pathopatch-1.0.2b0/pathopatch.egg-info/requires.txt
--rw-r--r--   0 fhoerst    (501) staff       (20)       11 2024-04-03 14:44:29.000000 pathopatch-1.0.2b0/pathopatch.egg-info/top_level.txt
--rw-r--r--   0 fhoerst    (501) staff       (20)       38 2024-04-03 14:44:29.693893 pathopatch-1.0.2b0/setup.cfg
--rw-r--r--   0 fhoerst    (501) staff       (20)     2167 2024-04-03 14:44:23.000000 pathopatch-1.0.2b0/setup.py
-drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-03 14:44:29.691229 pathopatch-1.0.2b0/tests/
--rw-r--r--   0 fhoerst    (501) staff       (20)        0 2024-01-12 10:03:42.000000 pathopatch-1.0.2b0/tests/__init__.py
-drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-03 14:44:29.692465 pathopatch-1.0.2b0/tests/test_core_modules/
--rw-r--r--   0 fhoerst    (501) staff       (20)        0 2024-01-12 10:03:42.000000 pathopatch-1.0.2b0/tests/test_core_modules/__init__.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     5478 2024-03-25 15:46:06.000000 pathopatch-1.0.2b0/tests/test_core_modules/test_annotations_filtering.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     5956 2024-03-26 07:05:02.000000 pathopatch-1.0.2b0/tests/test_core_modules/test_baseline.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     5198 2024-03-25 15:46:15.000000 pathopatch-1.0.2b0/tests/test_core_modules/test_complex_setup.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     4700 2024-03-25 15:46:19.000000 pathopatch-1.0.2b0/tests/test_core_modules/test_downsample.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     5457 2024-03-25 15:46:28.000000 pathopatch-1.0.2b0/tests/test_core_modules/test_roi.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     5759 2024-03-25 15:46:24.000000 pathopatch-1.0.2b0/tests/test_core_modules/test_roi_context.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     3064 2024-03-25 15:46:32.000000 pathopatch-1.0.2b0/tests/test_core_modules/test_target_magnification.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     3021 2024-03-25 15:46:42.000000 pathopatch-1.0.2b0/tests/test_core_modules/test_target_mpp.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     3705 2024-03-26 15:00:25.000000 pathopatch-1.0.2b0/tests/test_core_modules/test_target_mpp_macenko.py
-drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-03 14:44:29.692938 pathopatch-1.0.2b0/tests/test_utils/
--rw-r--r--   0 fhoerst    (501) staff       (20)        0 2024-01-12 10:03:42.000000 pathopatch-1.0.2b0/tests/test_utils/__init__.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     1657 2024-01-12 12:43:52.000000 pathopatch-1.0.2b0/tests/test_utils/test_csv_loading.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     5002 2024-03-26 16:01:13.000000 pathopatch-1.0.2b0/tests/test_utils/test_filters.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     1254 2024-01-12 12:43:52.000000 pathopatch-1.0.2b0/tests/test_utils/test_mask_rgb.py
+drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-05 14:09:40.140384 pathopatch-1.0.3b0/
+-rw-r--r--   0 fhoerst    (501) staff       (20)     1184 2024-03-26 16:01:10.000000 pathopatch-1.0.3b0/LICENSE.md
+-rw-r--r--   0 fhoerst    (501) staff       (20)    17500 2024-04-05 14:09:40.140173 pathopatch-1.0.3b0/PKG-INFO
+-rw-r--r--   0 fhoerst    (501) staff       (20)    23383 2024-04-02 13:00:08.000000 pathopatch-1.0.3b0/README.md
+drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-05 14:09:40.128198 pathopatch-1.0.3b0/pathopatch/
+-rw-r--r--   0 fhoerst    (501) staff       (20)       96 2024-01-12 12:43:51.000000 pathopatch-1.0.3b0/pathopatch/__init__.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     5013 2024-01-12 12:43:51.000000 pathopatch-1.0.3b0/pathopatch/annotation_conversion.py
+drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-05 14:09:40.129126 pathopatch-1.0.3b0/pathopatch/base_ml/
+-rw-r--r--   0 fhoerst    (501) staff       (20)        0 2024-01-12 12:43:51.000000 pathopatch-1.0.3b0/pathopatch/base_ml/__init__.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     4541 2024-01-12 12:43:51.000000 pathopatch-1.0.3b0/pathopatch/base_ml/base_cli.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)    39568 2024-04-02 12:25:57.000000 pathopatch-1.0.3b0/pathopatch/cli.py
+drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-05 14:09:40.129382 pathopatch-1.0.3b0/pathopatch/config/
+-rw-r--r--   0 fhoerst    (501) staff       (20)       96 2024-01-12 12:43:51.000000 pathopatch-1.0.3b0/pathopatch/config/__init__.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     1428 2024-04-02 12:25:57.000000 pathopatch-1.0.3b0/pathopatch/config/config.py
+drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-05 14:09:40.129625 pathopatch-1.0.3b0/pathopatch/data/
+-rw-r--r--   0 fhoerst    (501) staff       (20)       96 2024-01-12 12:43:51.000000 pathopatch-1.0.3b0/pathopatch/data/__init__.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)  6219914 2024-01-12 12:43:52.000000 pathopatch-1.0.3b0/pathopatch/data/tissue_detector.pt
+-rw-r--r--   0 fhoerst    (501) staff       (20)     1165 2024-01-12 12:43:52.000000 pathopatch-1.0.3b0/pathopatch/macenko_vector_generation.py
+drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-05 14:09:40.135281 pathopatch-1.0.3b0/pathopatch/patch_extraction/
+-rw-r--r--   0 fhoerst    (501) staff       (20)       96 2024-01-12 12:43:52.000000 pathopatch-1.0.3b0/pathopatch/patch_extraction/__init__.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)    32673 2024-04-05 13:47:50.000000 pathopatch-1.0.3b0/pathopatch/patch_extraction/dataset.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)    63509 2024-04-02 12:25:59.000000 pathopatch-1.0.3b0/pathopatch/patch_extraction/patch_extraction.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     9676 2024-04-02 12:25:58.000000 pathopatch-1.0.3b0/pathopatch/patch_extraction/process_batch.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)    12265 2024-01-12 12:43:52.000000 pathopatch-1.0.3b0/pathopatch/patch_extraction/storage.py
+drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-05 14:09:40.137168 pathopatch-1.0.3b0/pathopatch/utils/
+-rw-r--r--   0 fhoerst    (501) staff       (20)        0 2024-01-12 12:43:52.000000 pathopatch-1.0.3b0/pathopatch/utils/__init__.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)      608 2024-01-12 12:43:52.000000 pathopatch-1.0.3b0/pathopatch/utils/exceptions.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)      626 2024-01-12 12:43:52.000000 pathopatch-1.0.3b0/pathopatch/utils/file_handling.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)    13833 2024-03-26 16:01:13.000000 pathopatch-1.0.3b0/pathopatch/utils/filters.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     6334 2024-03-27 14:05:13.000000 pathopatch-1.0.3b0/pathopatch/utils/logger.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)    10801 2024-01-19 13:20:20.000000 pathopatch-1.0.3b0/pathopatch/utils/masking.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     3216 2024-01-12 12:43:52.000000 pathopatch-1.0.3b0/pathopatch/utils/patch_dataset.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)    46150 2024-04-02 12:25:58.000000 pathopatch-1.0.3b0/pathopatch/utils/patch_util.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)    10592 2024-01-12 12:43:52.000000 pathopatch-1.0.3b0/pathopatch/utils/plotting.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     7204 2024-01-12 12:43:52.000000 pathopatch-1.0.3b0/pathopatch/utils/tools.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     1066 2024-04-02 13:09:13.000000 pathopatch-1.0.3b0/pathopatch/wsi_extraction.py
+drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-05 14:09:40.137781 pathopatch-1.0.3b0/pathopatch/wsi_interfaces/
+-rw-r--r--   0 fhoerst    (501) staff       (20)      387 2024-03-29 14:01:43.000000 pathopatch-1.0.3b0/pathopatch/wsi_interfaces/__init__.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     3115 2024-04-02 06:35:01.000000 pathopatch-1.0.3b0/pathopatch/wsi_interfaces/cucim_deepzoom.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     1318 2024-04-02 12:25:58.000000 pathopatch-1.0.3b0/pathopatch/wsi_interfaces/openslide_deepzoom.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)    10424 2024-04-03 14:41:27.000000 pathopatch-1.0.3b0/pathopatch/wsi_interfaces/wsidicomizer_openslide.py
+drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-05 14:09:40.128923 pathopatch-1.0.3b0/pathopatch.egg-info/
+-rw-r--r--   0 fhoerst    (501) staff       (20)    17500 2024-04-05 14:09:40.000000 pathopatch-1.0.3b0/pathopatch.egg-info/PKG-INFO
+-rw-r--r--   0 fhoerst    (501) staff       (20)     1852 2024-04-05 14:09:40.000000 pathopatch-1.0.3b0/pathopatch.egg-info/SOURCES.txt
+-rw-r--r--   0 fhoerst    (501) staff       (20)        1 2024-04-05 14:09:40.000000 pathopatch-1.0.3b0/pathopatch.egg-info/dependency_links.txt
+-rw-r--r--   0 fhoerst    (501) staff       (20)      198 2024-04-05 14:09:40.000000 pathopatch-1.0.3b0/pathopatch.egg-info/entry_points.txt
+-rw-r--r--   0 fhoerst    (501) staff       (20)      297 2024-04-05 14:09:40.000000 pathopatch-1.0.3b0/pathopatch.egg-info/requires.txt
+-rw-r--r--   0 fhoerst    (501) staff       (20)       11 2024-04-05 14:09:40.000000 pathopatch-1.0.3b0/pathopatch.egg-info/top_level.txt
+-rw-r--r--   0 fhoerst    (501) staff       (20)       38 2024-04-05 14:09:40.140426 pathopatch-1.0.3b0/setup.cfg
+-rw-r--r--   0 fhoerst    (501) staff       (20)     2243 2024-04-05 13:03:55.000000 pathopatch-1.0.3b0/setup.py
+drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-05 14:09:40.138007 pathopatch-1.0.3b0/tests/
+-rw-r--r--   0 fhoerst    (501) staff       (20)        0 2024-01-12 10:03:42.000000 pathopatch-1.0.3b0/tests/__init__.py
+drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-05 14:09:40.139459 pathopatch-1.0.3b0/tests/test_core_modules/
+-rw-r--r--   0 fhoerst    (501) staff       (20)        0 2024-01-12 10:03:42.000000 pathopatch-1.0.3b0/tests/test_core_modules/__init__.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     5478 2024-03-25 15:46:06.000000 pathopatch-1.0.3b0/tests/test_core_modules/test_annotations_filtering.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     5956 2024-03-26 07:05:02.000000 pathopatch-1.0.3b0/tests/test_core_modules/test_baseline.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     5198 2024-03-25 15:46:15.000000 pathopatch-1.0.3b0/tests/test_core_modules/test_complex_setup.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     4700 2024-03-25 15:46:19.000000 pathopatch-1.0.3b0/tests/test_core_modules/test_downsample.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     5457 2024-03-25 15:46:28.000000 pathopatch-1.0.3b0/tests/test_core_modules/test_roi.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     5759 2024-03-25 15:46:24.000000 pathopatch-1.0.3b0/tests/test_core_modules/test_roi_context.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     3064 2024-03-25 15:46:32.000000 pathopatch-1.0.3b0/tests/test_core_modules/test_target_magnification.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     3021 2024-03-25 15:46:42.000000 pathopatch-1.0.3b0/tests/test_core_modules/test_target_mpp.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     3705 2024-03-26 15:00:25.000000 pathopatch-1.0.3b0/tests/test_core_modules/test_target_mpp_macenko.py
+drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-05 14:09:40.139970 pathopatch-1.0.3b0/tests/test_utils/
+-rw-r--r--   0 fhoerst    (501) staff       (20)        0 2024-01-12 10:03:42.000000 pathopatch-1.0.3b0/tests/test_utils/__init__.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     1657 2024-01-12 12:43:52.000000 pathopatch-1.0.3b0/tests/test_utils/test_csv_loading.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     5002 2024-03-26 16:01:13.000000 pathopatch-1.0.3b0/tests/test_utils/test_filters.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     1254 2024-01-12 12:43:52.000000 pathopatch-1.0.3b0/tests/test_utils/test_mask_rgb.py
```

### Comparing `pathopatch-1.0.2b0/LICENSE.md` & `pathopatch-1.0.3b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/PKG-INFO` & `pathopatch-1.0.3b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathopatch
-Version: 1.0.2b0
+Version: 1.0.3b0
 Summary: PathoPatch - Accelerating Artificial Intelligence Based Whole Slide Image Analysis with an Optimized Preprocessing Pipeline
 Home-page: https://github.com/TIO-IKIM/PathoPatcher
 Author: Fabian Hörst
 Author-email: fabian.hoerst@uk-essen.de
 Keywords: python,pathopatch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
@@ -12,36 +12,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Other
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: Pillow>=9.5.0
-Requires-Dist: PyYAML
-Requires-Dist: Shapely==1.8.5.post1
-Requires-Dist: colorama
-Requires-Dist: future
-Requires-Dist: geojson>=3.0.0
-Requires-Dist: matplotlib
-Requires-Dist: natsort
-Requires-Dist: numpy<1.24,>1.22
-Requires-Dist: opencv_python_headless
-Requires-Dist: openslide_python
-Requires-Dist: pandas
-Requires-Dist: pydantic==1.10.4
-Requires-Dist: rasterio==1.3.5.post1
-Requires-Dist: requests
-Requires-Dist: scikit-image
-Requires-Dist: setuptools<=65.6.3
-Requires-Dist: tqdm
-Requires-Dist: torchvision
-Requires-Dist: torch
-Requires-Dist: wsidicom==0.20.4
-Requires-Dist: wsidicomizer==0.13.2
 
 [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-360/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![Test-Results](https://github.com/TIO-IKIM/PathoPatcher/actions/workflows/test_build.yml/badge.svg)
 <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=Pytorch&logoColor=white"/></a>
 
 ___
```

### Comparing `pathopatch-1.0.2b0/README.md` & `pathopatch-1.0.3b0/README.md`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/pathopatch/annotation_conversion.py` & `pathopatch-1.0.3b0/pathopatch/annotation_conversion.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/pathopatch/base_ml/base_cli.py` & `pathopatch-1.0.3b0/pathopatch/base_ml/base_cli.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/pathopatch/cli.py` & `pathopatch-1.0.3b0/pathopatch/cli.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/pathopatch/config/config.py` & `pathopatch-1.0.3b0/pathopatch/config/config.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/pathopatch/macenko_vector_generation.py` & `pathopatch-1.0.3b0/pathopatch/macenko_vector_generation.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/pathopatch/patch_extraction/dataset.py` & `pathopatch-1.0.3b0/pathopatch/patch_extraction/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,15 +321,15 @@
         if self.detector_device == "cpu":
             self.logger.warning(
                 "No CUDA device detected - Speed may be very slow. Please consider performing extraction on CUDA device or disable tissue detector!"
             )
         model = mobilenet_v3_small().to(device=self.detector_device)
         model.classifier[-1] = nn.Linear(1024, 4)
         checkpoint = torch.load(
-            "./pathopatch/data/tissue_detector.pt",  # this causes errors
+            "/pathopatch/data/tissue_detector.pt",  # this causes errors
             map_location=self.detector_device,
         )
         model.load_state_dict(checkpoint["model_state_dict"])
         model.eval()
 
         self.detector_model = model
         self.detector_transforms = Compose(
```

### Comparing `pathopatch-1.0.2b0/pathopatch/patch_extraction/patch_extraction.py` & `pathopatch-1.0.3b0/pathopatch/patch_extraction/patch_extraction.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/pathopatch/patch_extraction/process_batch.py` & `pathopatch-1.0.3b0/pathopatch/patch_extraction/process_batch.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/pathopatch/patch_extraction/storage.py` & `pathopatch-1.0.3b0/pathopatch/patch_extraction/storage.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/pathopatch/utils/exceptions.py` & `pathopatch-1.0.3b0/pathopatch/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/pathopatch/utils/file_handling.py` & `pathopatch-1.0.3b0/pathopatch/utils/file_handling.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/pathopatch/utils/filters.py` & `pathopatch-1.0.3b0/pathopatch/utils/filters.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/pathopatch/utils/logger.py` & `pathopatch-1.0.3b0/pathopatch/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/pathopatch/utils/masking.py` & `pathopatch-1.0.3b0/pathopatch/utils/masking.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/pathopatch/utils/patch_dataset.py` & `pathopatch-1.0.3b0/pathopatch/utils/patch_dataset.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/pathopatch/utils/patch_util.py` & `pathopatch-1.0.3b0/pathopatch/utils/patch_util.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/pathopatch/utils/plotting.py` & `pathopatch-1.0.3b0/pathopatch/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/pathopatch/utils/tools.py` & `pathopatch-1.0.3b0/pathopatch/utils/tools.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/pathopatch/wsi_extraction.py` & `pathopatch-1.0.3b0/pathopatch/wsi_extraction.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/pathopatch/wsi_interfaces/cucim_deepzoom.py` & `pathopatch-1.0.3b0/pathopatch/wsi_interfaces/cucim_deepzoom.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/pathopatch/wsi_interfaces/openslide_deepzoom.py` & `pathopatch-1.0.3b0/pathopatch/wsi_interfaces/openslide_deepzoom.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/pathopatch/wsi_interfaces/wsidicomizer_openslide.py` & `pathopatch-1.0.3b0/pathopatch/wsi_interfaces/wsidicomizer_openslide.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/pathopatch.egg-info/PKG-INFO` & `pathopatch-1.0.3b0/pathopatch.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathopatch
-Version: 1.0.2b0
+Version: 1.0.3b0
 Summary: PathoPatch - Accelerating Artificial Intelligence Based Whole Slide Image Analysis with an Optimized Preprocessing Pipeline
 Home-page: https://github.com/TIO-IKIM/PathoPatcher
 Author: Fabian Hörst
 Author-email: fabian.hoerst@uk-essen.de
 Keywords: python,pathopatch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
@@ -12,36 +12,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Other
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: Pillow>=9.5.0
-Requires-Dist: PyYAML
-Requires-Dist: Shapely==1.8.5.post1
-Requires-Dist: colorama
-Requires-Dist: future
-Requires-Dist: geojson>=3.0.0
-Requires-Dist: matplotlib
-Requires-Dist: natsort
-Requires-Dist: numpy<1.24,>1.22
-Requires-Dist: opencv_python_headless
-Requires-Dist: openslide_python
-Requires-Dist: pandas
-Requires-Dist: pydantic==1.10.4
-Requires-Dist: rasterio==1.3.5.post1
-Requires-Dist: requests
-Requires-Dist: scikit-image
-Requires-Dist: setuptools<=65.6.3
-Requires-Dist: tqdm
-Requires-Dist: torchvision
-Requires-Dist: torch
-Requires-Dist: wsidicom==0.20.4
-Requires-Dist: wsidicomizer==0.13.2
 
 [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-360/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![Test-Results](https://github.com/TIO-IKIM/PathoPatcher/actions/workflows/test_build.yml/badge.svg)
 <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=Pytorch&logoColor=white"/></a>
 
 ___
```

### Comparing `pathopatch-1.0.2b0/pathopatch.egg-info/SOURCES.txt` & `pathopatch-1.0.3b0/pathopatch.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 pathopatch.egg-info/requires.txt
 pathopatch.egg-info/top_level.txt
 pathopatch/base_ml/__init__.py
 pathopatch/base_ml/base_cli.py
 pathopatch/config/__init__.py
 pathopatch/config/config.py
 pathopatch/data/__init__.py
+pathopatch/data/tissue_detector.pt
 pathopatch/patch_extraction/__init__.py
 pathopatch/patch_extraction/dataset.py
 pathopatch/patch_extraction/patch_extraction.py
 pathopatch/patch_extraction/process_batch.py
 pathopatch/patch_extraction/storage.py
 pathopatch/utils/__init__.py
 pathopatch/utils/exceptions.py
```

### Comparing `pathopatch-1.0.2b0/setup.py` & `pathopatch-1.0.3b0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "1.0.2b"
+VERSION = "1.0.3b"
 DESCRIPTION = "PathoPatch - Accelerating Artificial Intelligence Based Whole Slide Image Analysis with an Optimized Preprocessing Pipeline"
 with open("docs/README_pypi.md", "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
@@ -60,8 +60,10 @@
         "Intended Audience :: Education",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Programming Language :: Python :: 3",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX :: Other",
     ],
+    include_package_data=True,
+    package_data={"pathopatch": ["data/*"]},
 )
```

### Comparing `pathopatch-1.0.2b0/tests/test_core_modules/test_annotations_filtering.py` & `pathopatch-1.0.3b0/tests/test_core_modules/test_annotations_filtering.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/tests/test_core_modules/test_baseline.py` & `pathopatch-1.0.3b0/tests/test_core_modules/test_baseline.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/tests/test_core_modules/test_complex_setup.py` & `pathopatch-1.0.3b0/tests/test_core_modules/test_complex_setup.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/tests/test_core_modules/test_downsample.py` & `pathopatch-1.0.3b0/tests/test_core_modules/test_downsample.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/tests/test_core_modules/test_roi.py` & `pathopatch-1.0.3b0/tests/test_core_modules/test_roi.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/tests/test_core_modules/test_roi_context.py` & `pathopatch-1.0.3b0/tests/test_core_modules/test_roi_context.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/tests/test_core_modules/test_target_magnification.py` & `pathopatch-1.0.3b0/tests/test_core_modules/test_target_magnification.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/tests/test_core_modules/test_target_mpp.py` & `pathopatch-1.0.3b0/tests/test_core_modules/test_target_mpp.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/tests/test_core_modules/test_target_mpp_macenko.py` & `pathopatch-1.0.3b0/tests/test_core_modules/test_target_mpp_macenko.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/tests/test_utils/test_csv_loading.py` & `pathopatch-1.0.3b0/tests/test_utils/test_csv_loading.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/tests/test_utils/test_filters.py` & `pathopatch-1.0.3b0/tests/test_utils/test_filters.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.2b0/tests/test_utils/test_mask_rgb.py` & `pathopatch-1.0.3b0/tests/test_utils/test_mask_rgb.py`

 * *Files identical despite different names*

