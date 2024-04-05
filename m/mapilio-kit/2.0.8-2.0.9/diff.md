# Comparing `tmp/mapilio-kit-2.0.8.tar.gz` & `tmp/mapilio-kit-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapilio-kit-2.0.8.tar", last modified: Thu Dec  7 13:56:51 2023, max compression
+gzip compressed data, was "mapilio-kit-2.0.9.tar", last modified: Wed Dec 20 11:20:41 2023, max compression
```

## Comparing `mapilio-kit-2.0.8.tar` & `mapilio-kit-2.0.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 13:56:51.221493 mapilio-kit-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15696 2023-12-07 13:56:51.221493 mapilio-kit-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14571 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 13:56:51.213493 mapilio-kit-2.0.8/mapilio_kit/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 13:56:51.213493 mapilio-kit-2.0.8/mapilio_kit/base/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/base/authenticate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8630 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/base/decompose.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/base/gopro_360max.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/base/image_and_csv_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/base/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/base/process_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)    10272 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/base/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/base/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/base/video_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/base/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 13:56:51.221493 mapilio-kit-2.0.8/mapilio_kit/components/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5225 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/edit_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/error.py
--rw-r--r--   0 runner    (1001) docker     (127)    13017 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/exif_metadata_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/exif_metadata_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/geotag_property_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/gpmf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8801 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/gps_from_gopro360.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/gps_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/gpx_from_exif.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/gpx_from_gopro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/image_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4772 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/insert_MAPJson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/interprocess_communication.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/metadata_property_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/process_csv_to_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     8955 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7962 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/sequence_property_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6057 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/types_fmt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     6713 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/upload_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    15247 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8266 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5627 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/mapilio_kit/components/video_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 13:56:51.221493 mapilio-kit-2.0.8/mapilio_kit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15696 2023-12-07 13:56:51.000000 mapilio-kit-2.0.8/mapilio_kit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2023-12-07 13:56:51.000000 mapilio-kit-2.0.8/mapilio_kit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 13:56:51.000000 mapilio-kit-2.0.8/mapilio_kit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-12-07 13:56:51.000000 mapilio-kit-2.0.8/mapilio_kit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      448 2023-12-07 13:56:51.000000 mapilio-kit-2.0.8/mapilio_kit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-07 13:56:51.000000 mapilio-kit-2.0.8/mapilio_kit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-07 13:56:51.221493 mapilio-kit-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2023-12-07 13:56:35.000000 mapilio-kit-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 11:20:41.233999 mapilio-kit-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15690 2023-12-20 11:20:41.229999 mapilio-kit-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14565 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 11:20:41.221999 mapilio-kit-2.0.9/mapilio_kit/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 11:20:41.225999 mapilio-kit-2.0.9/mapilio_kit/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/base/authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8630 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/base/decompose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/base/gopro_360max.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/base/image_and_csv_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/base/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/base/process_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10272 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/base/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/base/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/base/video_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/base/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 11:20:41.229999 mapilio-kit-2.0.9/mapilio_kit/components/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5225 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/edit_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13017 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/exif_metadata_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/exif_metadata_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/geotag_property_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/gpmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8753 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/gps_from_gopro360.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/gps_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/gpx_from_exif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/gpx_from_gopro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/image_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4772 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/insert_MAPJson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/interprocess_communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/metadata_property_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/process_csv_to_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8955 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7962 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/sequence_property_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/types_fmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6713 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/upload_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15247 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5627 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/mapilio_kit/components/video_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 11:20:41.229999 mapilio-kit-2.0.9/mapilio_kit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15690 2023-12-20 11:20:41.000000 mapilio-kit-2.0.9/mapilio_kit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2023-12-20 11:20:41.000000 mapilio-kit-2.0.9/mapilio_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 11:20:41.000000 mapilio-kit-2.0.9/mapilio_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2023-12-20 11:20:41.000000 mapilio-kit-2.0.9/mapilio_kit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2023-12-20 11:20:41.000000 mapilio-kit-2.0.9/mapilio_kit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-20 11:20:41.000000 mapilio-kit-2.0.9/mapilio_kit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-20 11:20:41.233999 mapilio-kit-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2023-12-20 11:20:25.000000 mapilio-kit-2.0.9/setup.py
```

### Comparing `mapilio-kit-2.0.8/LICENSE` & `mapilio-kit-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/PKG-INFO` & `mapilio-kit-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapilio-kit
-Version: 2.0.8
+Version: 2.0.9
 Summary: MAPILIO Image/Video Upload and Pipeline
 Home-page: https://github.com/mapilio/mapilio-kit-v2
 Author: Mapilio
 License: MIT License
 Requires-Python: >=3.6, !=3.12.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -248,15 +248,15 @@
 python script config
 
 - --video-file {video file path}
 - --output-folder {output frames path}
 - --bin-dir {equirectanguler bin path}
 
 ```shell
-mapilio_kit gopro360max_process --video-file ~/Desktop/GS017111.360 --output-folder ~/Desktop/OutputData/ --bin-dir ../../bin
+mapilio_kit gopro360max_process --video-file ~/Desktop/GS017111.360 --output-folder ~/Desktop/OutputData/ --bin-dir bin
 ```
 
 2. Now we can upload frames
 
 ```shell
 mapilio_kit upload ~/Desktop/OutputData/frames --user_name="username@mapilio.com" \
                     --geotag_source "gpx" \
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mapilio-kit Version: 2.0.8 Summary: MAPILIO Image/
+Metadata-Version: 2.1 Name: mapilio-kit Version: 2.0.9 Summary: MAPILIO Image/
 Video Upload and Pipeline Home-page: https://github.com/mapilio/mapilio-kit-v2
 Author: Mapilio License: MIT License Requires-Python: >=3.6, !=3.12.*
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 attrs==21.2.0 Requires-Dist: certifi==2021.10.8 Requires-Dist: chardet==3.0.4
 Requires-Dist: charset-normalizer==2.0.7 Requires-Dist: construct==2.8.8
 Requires-Dist: ExifRead==2.3.2 Requires-Dist: gpxpy==0.9.8 Requires-Dist:
 pip>22.3.0 Requires-Dist: idna==2.7 Requires-Dist: jsonschema==4.1.1 Requires-
@@ -168,16 +168,16 @@
 mapilio_kit video_upload "path/to/sample_images/" --desc_path
 "mapilio_image_description.json" --processed
 ### **GoPro Max .360 videos** #### Must be installed with this method `./
 max_extractor_install.sh` 1. First, create equirectangular convert script such
 as below python script config - --video-file {video file path} - --output-
 folder {output frames path} - --bin-dir {equirectanguler bin path} ```shell
 mapilio_kit gopro360max_process --video-file ~/Desktop/GS017111.360 --output-
-folder ~/Desktop/OutputData/ --bin-dir ../../bin ``` 2. Now we can upload
-frames ```shell mapilio_kit upload ~/Desktop/OutputData/frames --
+folder ~/Desktop/OutputData/ --bin-dir bin ``` 2. Now we can upload frames
+```shell mapilio_kit upload ~/Desktop/OutputData/frames --
 user_name="username@mapilio.com" \ --geotag_source "gpx" \ --geotag_source_path
 "~Desktop/gps_track.gpx" ```
 ******** DDeeccoommppoossee IImmaaggeess ********
 The decompose command geotags images in the given directory. It extracts the
 required and optional metadata from image EXIF (or the other supported geotag
 sources), and writes all the metadata (or process errors) in an image
 description file, which will be read during upload.
```

### Comparing `mapilio-kit-2.0.8/README.md` & `mapilio-kit-2.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
 python script config
 
 - --video-file {video file path}
 - --output-folder {output frames path}
 - --bin-dir {equirectanguler bin path}
 
 ```shell
-mapilio_kit gopro360max_process --video-file ~/Desktop/GS017111.360 --output-folder ~/Desktop/OutputData/ --bin-dir ../../bin
+mapilio_kit gopro360max_process --video-file ~/Desktop/GS017111.360 --output-folder ~/Desktop/OutputData/ --bin-dir bin
 ```
 
 2. Now we can upload frames
 
 ```shell
 mapilio_kit upload ~/Desktop/OutputData/frames --user_name="username@mapilio.com" \
                     --geotag_source "gpx" \
```

#### html2text {}

```diff
@@ -153,16 +153,16 @@
 mapilio_kit video_upload "path/to/sample_images/" --desc_path
 "mapilio_image_description.json" --processed
 ### **GoPro Max .360 videos** #### Must be installed with this method `./
 max_extractor_install.sh` 1. First, create equirectangular convert script such
 as below python script config - --video-file {video file path} - --output-
 folder {output frames path} - --bin-dir {equirectanguler bin path} ```shell
 mapilio_kit gopro360max_process --video-file ~/Desktop/GS017111.360 --output-
-folder ~/Desktop/OutputData/ --bin-dir ../../bin ``` 2. Now we can upload
-frames ```shell mapilio_kit upload ~/Desktop/OutputData/frames --
+folder ~/Desktop/OutputData/ --bin-dir bin ``` 2. Now we can upload frames
+```shell mapilio_kit upload ~/Desktop/OutputData/frames --
 user_name="username@mapilio.com" \ --geotag_source "gpx" \ --geotag_source_path
 "~Desktop/gps_track.gpx" ```
 ******** DDeeccoommppoossee IImmaaggeess ********
 The decompose command geotags images in the given directory. It extracts the
 required and optional metadata from image EXIF (or the other supported geotag
 sources), and writes all the metadata (or process errors) in an image
 description file, which will be read during upload.
```

### Comparing `mapilio-kit-2.0.8/mapilio_kit/__main__.py` & `mapilio-kit-2.0.9/mapilio_kit/__main__.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/base/__init__.py` & `mapilio-kit-2.0.9/mapilio_kit/base/__init__.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/base/authenticate.py` & `mapilio-kit-2.0.9/mapilio_kit/base/authenticate.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/base/decompose.py` & `mapilio-kit-2.0.9/mapilio_kit/base/decompose.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/base/gopro_360max.py` & `mapilio-kit-2.0.9/mapilio_kit/base/gopro_360max.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/base/image_and_csv_upload.py` & `mapilio-kit-2.0.9/mapilio_kit/base/image_and_csv_upload.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/base/loader.py` & `mapilio-kit-2.0.9/mapilio_kit/base/loader.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/base/process_csv.py` & `mapilio-kit-2.0.9/mapilio_kit/base/process_csv.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/base/run.py` & `mapilio-kit-2.0.9/mapilio_kit/base/run.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/base/sampler.py` & `mapilio-kit-2.0.9/mapilio_kit/base/sampler.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/base/video_upload.py` & `mapilio-kit-2.0.9/mapilio_kit/base/video_upload.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/base/zip.py` & `mapilio-kit-2.0.9/mapilio_kit/base/zip.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/components/arguments.py` & `mapilio-kit-2.0.9/mapilio_kit/components/arguments.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/components/auth_config.py` & `mapilio-kit-2.0.9/mapilio_kit/components/auth_config.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/components/config.py` & `mapilio-kit-2.0.9/mapilio_kit/components/config.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/components/edit_config.py` & `mapilio-kit-2.0.9/mapilio_kit/components/edit_config.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/components/exif_metadata_reader.py` & `mapilio-kit-2.0.9/mapilio_kit/components/exif_metadata_reader.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/components/exif_metadata_writer.py` & `mapilio-kit-2.0.9/mapilio_kit/components/exif_metadata_writer.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/components/ffmpeg.py` & `mapilio-kit-2.0.9/mapilio_kit/components/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/components/geotag_property_handler.py` & `mapilio-kit-2.0.9/mapilio_kit/components/geotag_property_handler.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/components/gpmf.py` & `mapilio-kit-2.0.9/mapilio_kit/components/gpmf.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/components/gps_from_gopro360.py` & `mapilio-kit-2.0.9/mapilio_kit/components/gps_from_gopro360.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,14 @@
                        bin_dir: str):
     script_dir = os.path.dirname(os.path.realpath(__file__))
     frame_delta = 1.0 / frame_rate
     print(f"frame_delta: {frame_delta}")
 
     assert_file_exists(video_file, "video file")
 
-    bin_dir = os.path.join(script_dir, bin_dir)
     assert_folder_exists(bin_dir)
 
     eac_stitcher_exe = os.path.join(bin_dir, 'MAX2spherebatch')
     assert_file_exists(eac_stitcher_exe)
 
     make_directory(output_folder, remove_if_present=True)
```

### Comparing `mapilio-kit-2.0.8/mapilio_kit/components/gps_parser.py` & `mapilio-kit-2.0.9/mapilio_kit/components/gps_parser.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/components/gpx_from_exif.py` & `mapilio-kit-2.0.9/mapilio_kit/components/gpx_from_exif.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/components/gpx_from_gopro.py` & `mapilio-kit-2.0.9/mapilio_kit/components/gpx_from_gopro.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/components/image_log.py` & `mapilio-kit-2.0.9/mapilio_kit/components/image_log.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/components/insert_MAPJson.py` & `mapilio-kit-2.0.9/mapilio_kit/components/insert_MAPJson.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/components/interprocess_communication.py` & `mapilio-kit-2.0.9/mapilio_kit/components/interprocess_communication.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/components/login.py` & `mapilio-kit-2.0.9/mapilio_kit/components/login.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/components/metadata_property_handler.py` & `mapilio-kit-2.0.9/mapilio_kit/components/metadata_property_handler.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/components/process_csv_to_description.py` & `mapilio-kit-2.0.9/mapilio_kit/components/process_csv_to_description.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/components/processing.py` & `mapilio-kit-2.0.9/mapilio_kit/components/processing.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/components/sequence_property_handler.py` & `mapilio-kit-2.0.9/mapilio_kit/components/sequence_property_handler.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/components/types_fmt.py` & `mapilio-kit-2.0.9/mapilio_kit/components/types_fmt.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/components/upload.py` & `mapilio-kit-2.0.9/mapilio_kit/components/upload.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/components/upload_manager.py` & `mapilio-kit-2.0.9/mapilio_kit/components/upload_manager.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/components/uploader.py` & `mapilio-kit-2.0.9/mapilio_kit/components/uploader.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/components/utilities.py` & `mapilio-kit-2.0.9/mapilio_kit/components/utilities.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit/components/video_processor.py` & `mapilio-kit-2.0.9/mapilio_kit/components/video_processor.py`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/mapilio_kit.egg-info/PKG-INFO` & `mapilio-kit-2.0.9/mapilio_kit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapilio-kit
-Version: 2.0.8
+Version: 2.0.9
 Summary: MAPILIO Image/Video Upload and Pipeline
 Home-page: https://github.com/mapilio/mapilio-kit-v2
 Author: Mapilio
 License: MIT License
 Requires-Python: >=3.6, !=3.12.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -248,15 +248,15 @@
 python script config
 
 - --video-file {video file path}
 - --output-folder {output frames path}
 - --bin-dir {equirectanguler bin path}
 
 ```shell
-mapilio_kit gopro360max_process --video-file ~/Desktop/GS017111.360 --output-folder ~/Desktop/OutputData/ --bin-dir ../../bin
+mapilio_kit gopro360max_process --video-file ~/Desktop/GS017111.360 --output-folder ~/Desktop/OutputData/ --bin-dir bin
 ```
 
 2. Now we can upload frames
 
 ```shell
 mapilio_kit upload ~/Desktop/OutputData/frames --user_name="username@mapilio.com" \
                     --geotag_source "gpx" \
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mapilio-kit Version: 2.0.8 Summary: MAPILIO Image/
+Metadata-Version: 2.1 Name: mapilio-kit Version: 2.0.9 Summary: MAPILIO Image/
 Video Upload and Pipeline Home-page: https://github.com/mapilio/mapilio-kit-v2
 Author: Mapilio License: MIT License Requires-Python: >=3.6, !=3.12.*
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 attrs==21.2.0 Requires-Dist: certifi==2021.10.8 Requires-Dist: chardet==3.0.4
 Requires-Dist: charset-normalizer==2.0.7 Requires-Dist: construct==2.8.8
 Requires-Dist: ExifRead==2.3.2 Requires-Dist: gpxpy==0.9.8 Requires-Dist:
 pip>22.3.0 Requires-Dist: idna==2.7 Requires-Dist: jsonschema==4.1.1 Requires-
@@ -168,16 +168,16 @@
 mapilio_kit video_upload "path/to/sample_images/" --desc_path
 "mapilio_image_description.json" --processed
 ### **GoPro Max .360 videos** #### Must be installed with this method `./
 max_extractor_install.sh` 1. First, create equirectangular convert script such
 as below python script config - --video-file {video file path} - --output-
 folder {output frames path} - --bin-dir {equirectanguler bin path} ```shell
 mapilio_kit gopro360max_process --video-file ~/Desktop/GS017111.360 --output-
-folder ~/Desktop/OutputData/ --bin-dir ../../bin ``` 2. Now we can upload
-frames ```shell mapilio_kit upload ~/Desktop/OutputData/frames --
+folder ~/Desktop/OutputData/ --bin-dir bin ``` 2. Now we can upload frames
+```shell mapilio_kit upload ~/Desktop/OutputData/frames --
 user_name="username@mapilio.com" \ --geotag_source "gpx" \ --geotag_source_path
 "~Desktop/gps_track.gpx" ```
 ******** DDeeccoommppoossee IImmaaggeess ********
 The decompose command geotags images in the given directory. It extracts the
 required and optional metadata from image EXIF (or the other supported geotag
 sources), and writes all the metadata (or process errors) in an image
 description file, which will be read during upload.
```

### Comparing `mapilio-kit-2.0.8/mapilio_kit.egg-info/SOURCES.txt` & `mapilio-kit-2.0.9/mapilio_kit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mapilio-kit-2.0.8/setup.py` & `mapilio-kit-2.0.9/setup.py`

 * *Files identical despite different names*

