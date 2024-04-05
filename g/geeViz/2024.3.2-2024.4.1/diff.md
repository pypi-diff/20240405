# Comparing `tmp/geeViz-2024.3.2.tar.gz` & `tmp/geeViz-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geeViz-2024.3.2.tar", last modified: Fri Mar 22 23:06:35 2024, max compression
+gzip compressed data, was "geeViz-2024.4.1.tar", last modified: Fri Apr  5 01:26:47 2024, max compression
```

## Comparing `geeViz-2024.3.2.tar` & `geeViz-2024.4.1.tar`

### file list

```diff
@@ -1,92 +1,93 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 23:06:35.818733 geeViz-2024.3.2/
--rw-rw-rw-   0        0        0      574 2023-07-18 20:24:42.000000 geeViz-2024.3.2/LICENSE
--rw-rw-rw-   0        0        0     4489 2024-03-22 23:06:35.787482 geeViz-2024.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     3549 2024-03-21 18:20:46.000000 geeViz-2024.3.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-22 23:06:29.302583 geeViz-2024.3.2/geeViz/
--rw-rw-rw-   0        0        0      120 2024-03-22 22:59:23.000000 geeViz-2024.3.2/geeViz/__init__.py
--rw-rw-rw-   0        0        0    26721 2024-03-19 16:59:37.000000 geeViz-2024.3.2/geeViz/assetManagerLib.py
--rw-rw-rw-   0        0        0   115771 2024-03-19 16:55:41.000000 geeViz-2024.3.2/geeViz/changeDetectionLib.py
--rw-rw-rw-   0        0        0     3119 2024-03-19 17:01:18.000000 geeViz-2024.3.2/geeViz/cloudStorageManagerLib.py
-drwxrwxrwx   0        0        0        0 2024-03-22 23:06:32.396579 geeViz-2024.3.2/geeViz/examples/
--rw-rw-rw-   0        0        0     5506 2024-01-19 23:22:16.000000 geeViz-2024.3.2/geeViz/examples/CCDCViz.py
--rw-rw-rw-   0        0        0    13528 2024-01-19 23:21:46.000000 geeViz-2024.3.2/geeViz/examples/CCDCVizNotebook.ipynb
--rw-rw-rw-   0        0        0     7865 2024-01-20 01:32:54.000000 geeViz-2024.3.2/geeViz/examples/CCDCWrapper.py
--rw-rw-rw-   0        0        0     4385 2024-01-20 01:32:54.000000 geeViz-2024.3.2/geeViz/examples/GFSTimeLapse.py
--rw-rw-rw-   0        0        0     5259 2024-02-08 18:08:46.000000 geeViz-2024.3.2/geeViz/examples/LANDTRENDRViz.py
--rw-rw-rw-   0        0        0    11466 2024-01-19 23:21:45.000000 geeViz-2024.3.2/geeViz/examples/LANDTRENDRWrapper.py
--rw-rw-rw-   0        0        0    22824 2024-01-19 23:21:46.000000 geeViz-2024.3.2/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb
--rw-rw-rw-   0        0        0    12434 2024-01-19 23:21:45.000000 geeViz-2024.3.2/geeViz/examples/LCMAP_and_LCMS_Viewer.py
--rw-rw-rw-   0        0        0    20606 2024-01-19 23:21:46.000000 geeViz-2024.3.2/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb
--rw-rw-rw-   0        0        0      120 2024-03-22 23:00:13.000000 geeViz-2024.3.2/geeViz/examples/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-22 23:06:28.380635 geeViz-2024.3.2/geeViz/examples/data/
-drwxrwxrwx   0        0        0        0 2024-03-22 23:06:33.302901 geeViz-2024.3.2/geeViz/examples/data/gadm41_CHE_shp/
--rw-rw-rw-   0        0        0        5 2024-01-19 21:39:53.000000 geeViz-2024.3.2/geeViz/examples/data/gadm41_CHE_shp/gadm41_CHE_0.cpg
--rw-rw-rw-   0        0        0      120 2024-01-19 21:39:53.000000 geeViz-2024.3.2/geeViz/examples/data/gadm41_CHE_shp/gadm41_CHE_0.dbf
--rw-rw-rw-   0        0        0  3062140 2024-01-19 21:59:00.000000 geeViz-2024.3.2/geeViz/examples/data/gadm41_CHE_shp/gadm41_CHE_0.geojson
--rw-rw-rw-   0        0        0      145 2024-01-19 21:39:53.000000 geeViz-2024.3.2/geeViz/examples/data/gadm41_CHE_shp/gadm41_CHE_0.prj
--rw-rw-rw-   0        0        0   461372 2024-01-19 21:39:53.000000 geeViz-2024.3.2/geeViz/examples/data/gadm41_CHE_shp/gadm41_CHE_0.shp
--rw-rw-rw-   0        0        0      108 2024-01-19 21:39:53.000000 geeViz-2024.3.2/geeViz/examples/data/gadm41_CHE_shp/gadm41_CHE_0.shx
--rw-rw-rw-   0        0        0     1925 2024-01-19 23:21:45.000000 geeViz-2024.3.2/geeViz/examples/foliumViewerExample.py
--rw-rw-rw-   0        0        0   236037 2024-01-19 23:21:46.000000 geeViz-2024.3.2/geeViz/examples/gee2PandasExample.ipynb
--rw-rw-rw-   0        0        0     5856 2024-01-19 23:21:12.000000 geeViz-2024.3.2/geeViz/examples/geeViewExample.py
--rw-rw-rw-   0        0        0    18940 2024-01-19 23:21:46.000000 geeViz-2024.3.2/geeViz/examples/geeViewExampleNotebook.ipynb
--rw-rw-rw-   0        0        0    43684 2024-02-13 19:37:24.000000 geeViz-2024.3.2/geeViz/examples/geeViewVSFoliumViewerExampleNotebook.ipynb
--rw-rw-rw-   0        0        0     1641 2024-01-20 02:01:38.000000 geeViz-2024.3.2/geeViz/examples/geeViz_and_geemap.py
--rw-rw-rw-   0        0        0     5653 2024-01-20 01:32:55.000000 geeViz-2024.3.2/geeViz/examples/getClimateWrapper.py
--rw-rw-rw-   0        0        0    14964 2024-01-20 01:30:46.000000 geeViz-2024.3.2/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py
--rw-rw-rw-   0        0        0    11660 2024-03-07 20:00:49.000000 geeViz-2024.3.2/geeViz/examples/getLandsatWrapper.py
--rw-rw-rw-   0        0        0    20983 2024-01-19 23:21:46.000000 geeViz-2024.3.2/geeViz/examples/getLandsatWrapperNotebook.ipynb
--rw-rw-rw-   0        0        0    12989 2024-01-20 01:32:54.000000 geeViz-2024.3.2/geeViz/examples/getSentinel2Wrapper.py
--rw-rw-rw-   0        0        0     8991 2024-01-20 01:32:55.000000 geeViz-2024.3.2/geeViz/examples/harmonicRegressionWrapper.py
--rw-rw-rw-   0        0        0    10265 2024-03-19 19:26:08.000000 geeViz-2024.3.2/geeViz/examples/lcmsViewerExample.py
--rw-rw-rw-   0        0        0    23631 2024-01-19 23:21:46.000000 geeViz-2024.3.2/geeViz/examples/lcmsViewerExampleNotebook.ipynb
--rw-rw-rw-   0        0        0     6262 2024-03-21 17:55:40.000000 geeViz-2024.3.2/geeViz/examples/mapBiomasViewerExample.py
--rw-rw-rw-   0        0        0    13051 2024-01-20 01:32:55.000000 geeViz-2024.3.2/geeViz/examples/phEEnoVizWrapper.py
--rw-rw-rw-   0        0        0     1038 2024-01-20 01:32:55.000000 geeViz-2024.3.2/geeViz/examples/taskTrackerExample.py
--rw-rw-rw-   0        0        0     6194 2024-01-20 02:08:49.000000 geeViz-2024.3.2/geeViz/examples/timeLapseExample.py
--rw-rw-rw-   0        0        0     9132 2024-03-19 17:03:58.000000 geeViz-2024.3.2/geeViz/foliumView.py
--rw-rw-rw-   0        0        0     1741 2021-04-01 17:15:14.000000 geeViz-2024.3.2/geeViz/gcpLib.py
--rw-rw-rw-   0        0        0    18888 2024-03-19 17:05:58.000000 geeViz-2024.3.2/geeViz/gee2Pandas.py
-drwxrwxrwx   0        0        0        0 2024-03-22 23:06:33.552957 geeViz-2024.3.2/geeViz/geeView/
--rw-rw-rw-   0        0        0     7260 2024-02-07 20:42:41.000000 geeViz-2024.3.2/geeViz/geeView/foliumView.html
--rw-rw-rw-   0        0        0     3321 2024-02-27 19:55:46.000000 geeViz-2024.3.2/geeViz/geeView/index.html
-drwxrwxrwx   0        0        0        0 2024-03-22 23:06:28.411887 geeViz-2024.3.2/geeViz/geeView/src/
-drwxrwxrwx   0        0        0        0 2024-03-22 23:06:28.396261 geeViz-2024.3.2/geeViz/geeView/src/assets/
-drwxrwxrwx   0        0        0        0 2024-03-22 23:06:34.787399 geeViz-2024.3.2/geeViz/geeView/src/assets/images/
--rw-rw-rw-   0        0        0     7295 2021-04-01 17:15:14.000000 geeViz-2024.3.2/geeViz/geeView/src/assets/images/EE-logo-150.png
--rw-rw-rw-   0        0        0    10301 2021-04-01 17:15:14.000000 geeViz-2024.3.2/geeViz/geeView/src/assets/images/GEE.png
--rw-rw-rw-   0        0        0     5692 2022-08-19 21:41:40.000000 geeViz-2024.3.2/geeViz/geeView/src/assets/images/GEE_logo_transparent.png
--rw-rw-rw-   0        0        0     4551 2021-04-01 17:15:14.000000 geeViz-2024.3.2/geeViz/geeView/src/assets/images/RCR-logo.jpg
--rw-rw-rw-   0        0        0    35328 2022-12-07 01:04:30.000000 geeViz-2024.3.2/geeViz/geeView/src/assets/images/Thumbs.db
--rw-rw-rw-   0        0        0     8352 2021-04-01 17:15:14.000000 geeViz-2024.3.2/geeViz/geeView/src/assets/images/cumulative_icon.png
--rw-rw-rw-   0        0        0     1502 2021-04-01 17:15:15.000000 geeViz-2024.3.2/geeViz/geeView/src/assets/images/layer_icon.png
--rw-rw-rw-   0        0        0   230271 2022-06-28 20:18:38.000000 geeViz-2024.3.2/geeViz/geeView/src/assets/images/logos_usda-fs.svg
--rw-rw-rw-   0        0        0   229463 2022-06-30 19:30:12.000000 geeViz-2024.3.2/geeViz/geeView/src/assets/images/logos_usda-fs_bn-dk-01.svg
--rw-rw-rw-   0        0        0      635 2022-06-29 22:17:42.000000 geeViz-2024.3.2/geeViz/geeView/src/assets/images/menu-hamburger_ffffff.svg
--rw-rw-rw-   0        0        0     1489 2021-04-01 17:15:15.000000 geeViz-2024.3.2/geeViz/geeView/src/assets/images/usdalogo.png
--rw-rw-rw-   0        0        0     8174 2021-04-01 17:15:15.000000 geeViz-2024.3.2/geeViz/geeView/src/assets/images/usfslogo.png
-drwxrwxrwx   0        0        0        0 2024-03-22 23:06:28.411887 geeViz-2024.3.2/geeViz/geeView/src/gee/
-drwxrwxrwx   0        0        0        0 2024-03-22 23:06:35.021793 geeViz-2024.3.2/geeViz/geeView/src/gee/gee-libraries/
--rw-rw-rw-   0        0        0    65322 2024-03-22 22:30:17.000000 geeViz-2024.3.2/geeViz/geeView/src/gee/gee-libraries/changeDetectionLib.js
--rw-rw-rw-   0        0        0   112794 2024-03-22 22:30:17.000000 geeViz-2024.3.2/geeViz/geeView/src/gee/gee-libraries/getImagesLib.js
-drwxrwxrwx   0        0        0        0 2024-03-22 23:06:35.146803 geeViz-2024.3.2/geeViz/geeView/src/gee/gee-run/
--rw-rw-rw-   0        0        0     1044 2024-03-22 22:59:13.000000 geeViz-2024.3.2/geeViz/geeView/src/gee/gee-run/runGeeViz.js
-drwxrwxrwx   0        0        0        0 2024-03-22 23:06:35.631218 geeViz-2024.3.2/geeViz/geeView/src/js/
--rw-rw-rw-   0        0        0    45351 2020-01-16 17:35:18.000000 geeViz-2024.3.2/geeViz/geeView/src/js/gena-gee-palettes.js
--rw-rw-rw-   0        0        0   462779 2024-03-22 22:30:17.000000 geeViz-2024.3.2/geeViz/geeView/src/js/lcms-viewer.min.js
--rw-rw-rw-   0        0        0     1021 2023-03-08 18:47:59.000000 geeViz-2024.3.2/geeViz/geeView/src/js/load.min.js
-drwxrwxrwx   0        0        0        0 2024-03-22 23:06:35.678097 geeViz-2024.3.2/geeViz/geeView/src/styles/
--rw-rw-rw-   0        0        0    32682 2024-03-22 22:30:18.000000 geeViz-2024.3.2/geeViz/geeView/src/styles/style.min.css
--rw-rw-rw-   0        0        0    58167 2024-03-22 22:42:47.000000 geeViz-2024.3.2/geeViz/geeView.py
--rw-rw-rw-   0        0        0   228998 2024-03-19 16:37:42.000000 geeViz-2024.3.2/geeViz/getImagesLib.py
--rw-rw-rw-   0        0        0     7928 2024-03-19 17:06:25.000000 geeViz-2024.3.2/geeViz/migrateGEEAssets.py
--rw-rw-rw-   0        0        0    25768 2024-03-19 17:09:18.000000 geeViz-2024.3.2/geeViz/phEEnoViz.py
--rw-rw-rw-   0        0        0    11182 2024-03-19 17:10:37.000000 geeViz-2024.3.2/geeViz/taskManagerLib.py
-drwxrwxrwx   0        0        0        0 2024-03-22 23:06:35.740602 geeViz-2024.3.2/geeViz.egg-info/
--rw-rw-rw-   0        0        0     4489 2024-03-22 23:06:27.000000 geeViz-2024.3.2/geeViz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2866 2024-03-22 23:06:28.000000 geeViz-2024.3.2/geeViz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 23:06:27.000000 geeViz-2024.3.2/geeViz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2024-03-22 23:06:27.000000 geeViz-2024.3.2/geeViz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-22 23:06:27.000000 geeViz-2024.3.2/geeViz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-22 23:06:35.865612 geeViz-2024.3.2/setup.cfg
--rw-rw-rw-   0        0        0     2587 2024-03-21 18:41:47.000000 geeViz-2024.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 01:26:47.721872 geeViz-2024.4.1/
+-rw-rw-rw-   0        0        0      574 2023-07-18 20:24:42.000000 geeViz-2024.4.1/LICENSE
+-rw-rw-rw-   0        0        0     4442 2024-04-05 01:26:47.690589 geeViz-2024.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3502 2024-03-25 18:03:29.000000 geeViz-2024.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 01:26:41.908860 geeViz-2024.4.1/geeViz/
+-rw-rw-rw-   0        0        0      120 2024-04-05 01:24:26.000000 geeViz-2024.4.1/geeViz/__init__.py
+-rw-rw-rw-   0        0        0    26721 2024-03-19 16:59:37.000000 geeViz-2024.4.1/geeViz/assetManagerLib.py
+-rw-rw-rw-   0        0        0   115771 2024-03-19 16:55:41.000000 geeViz-2024.4.1/geeViz/changeDetectionLib.py
+-rw-rw-rw-   0        0        0     3119 2024-03-19 17:01:18.000000 geeViz-2024.4.1/geeViz/cloudStorageManagerLib.py
+drwxrwxrwx   0        0        0        0 2024-04-05 01:26:43.971530 geeViz-2024.4.1/geeViz/examples/
+-rw-rw-rw-   0        0        0     5506 2024-01-19 23:22:16.000000 geeViz-2024.4.1/geeViz/examples/CCDCViz.py
+-rw-rw-rw-   0        0        0    13528 2024-01-19 23:21:46.000000 geeViz-2024.4.1/geeViz/examples/CCDCVizNotebook.ipynb
+-rw-rw-rw-   0        0        0     7865 2024-01-20 01:32:54.000000 geeViz-2024.4.1/geeViz/examples/CCDCWrapper.py
+-rw-rw-rw-   0        0        0     4385 2024-01-20 01:32:54.000000 geeViz-2024.4.1/geeViz/examples/GFSTimeLapse.py
+-rw-rw-rw-   0        0        0     5259 2024-02-08 18:08:46.000000 geeViz-2024.4.1/geeViz/examples/LANDTRENDRViz.py
+-rw-rw-rw-   0        0        0    11466 2024-01-19 23:21:45.000000 geeViz-2024.4.1/geeViz/examples/LANDTRENDRWrapper.py
+-rw-rw-rw-   0        0        0    22824 2024-01-19 23:21:46.000000 geeViz-2024.4.1/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb
+-rw-rw-rw-   0        0        0    12434 2024-01-19 23:21:45.000000 geeViz-2024.4.1/geeViz/examples/LCMAP_and_LCMS_Viewer.py
+-rw-rw-rw-   0        0        0    20606 2024-01-19 23:21:46.000000 geeViz-2024.4.1/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb
+-rw-rw-rw-   0        0        0      120 2024-04-05 01:24:16.000000 geeViz-2024.4.1/geeViz/examples/__init__.py
+-rw-rw-rw-   0        0        0    59514 2024-04-05 01:24:06.000000 geeViz-2024.4.1/geeViz/examples/areaChart_examples.ipynb
+drwxrwxrwx   0        0        0        0 2024-04-05 01:26:40.986909 geeViz-2024.4.1/geeViz/examples/data/
+drwxrwxrwx   0        0        0        0 2024-04-05 01:26:44.831011 geeViz-2024.4.1/geeViz/examples/data/gadm41_CHE_shp/
+-rw-rw-rw-   0        0        0        5 2024-01-19 21:39:53.000000 geeViz-2024.4.1/geeViz/examples/data/gadm41_CHE_shp/gadm41_CHE_0.cpg
+-rw-rw-rw-   0        0        0      120 2024-01-19 21:39:53.000000 geeViz-2024.4.1/geeViz/examples/data/gadm41_CHE_shp/gadm41_CHE_0.dbf
+-rw-rw-rw-   0        0        0  3062140 2024-01-19 21:59:00.000000 geeViz-2024.4.1/geeViz/examples/data/gadm41_CHE_shp/gadm41_CHE_0.geojson
+-rw-rw-rw-   0        0        0      145 2024-01-19 21:39:53.000000 geeViz-2024.4.1/geeViz/examples/data/gadm41_CHE_shp/gadm41_CHE_0.prj
+-rw-rw-rw-   0        0        0   461372 2024-01-19 21:39:53.000000 geeViz-2024.4.1/geeViz/examples/data/gadm41_CHE_shp/gadm41_CHE_0.shp
+-rw-rw-rw-   0        0        0      108 2024-01-19 21:39:53.000000 geeViz-2024.4.1/geeViz/examples/data/gadm41_CHE_shp/gadm41_CHE_0.shx
+-rw-rw-rw-   0        0        0     1925 2024-01-19 23:21:45.000000 geeViz-2024.4.1/geeViz/examples/foliumViewerExample.py
+-rw-rw-rw-   0        0        0   236037 2024-01-19 23:21:46.000000 geeViz-2024.4.1/geeViz/examples/gee2PandasExample.ipynb
+-rw-rw-rw-   0        0        0     5856 2024-01-19 23:21:12.000000 geeViz-2024.4.1/geeViz/examples/geeViewExample.py
+-rw-rw-rw-   0        0        0    18940 2024-01-19 23:21:46.000000 geeViz-2024.4.1/geeViz/examples/geeViewExampleNotebook.ipynb
+-rw-rw-rw-   0        0        0    43684 2024-02-13 19:37:24.000000 geeViz-2024.4.1/geeViz/examples/geeViewVSFoliumViewerExampleNotebook.ipynb
+-rw-rw-rw-   0        0        0     1641 2024-01-20 02:01:38.000000 geeViz-2024.4.1/geeViz/examples/geeViz_and_geemap.py
+-rw-rw-rw-   0        0        0     5653 2024-01-20 01:32:55.000000 geeViz-2024.4.1/geeViz/examples/getClimateWrapper.py
+-rw-rw-rw-   0        0        0    14964 2024-01-20 01:30:46.000000 geeViz-2024.4.1/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py
+-rw-rw-rw-   0        0        0    11660 2024-03-07 20:00:49.000000 geeViz-2024.4.1/geeViz/examples/getLandsatWrapper.py
+-rw-rw-rw-   0        0        0    20983 2024-01-19 23:21:46.000000 geeViz-2024.4.1/geeViz/examples/getLandsatWrapperNotebook.ipynb
+-rw-rw-rw-   0        0        0    12989 2024-01-20 01:32:54.000000 geeViz-2024.4.1/geeViz/examples/getSentinel2Wrapper.py
+-rw-rw-rw-   0        0        0     8991 2024-01-20 01:32:55.000000 geeViz-2024.4.1/geeViz/examples/harmonicRegressionWrapper.py
+-rw-rw-rw-   0        0        0     9996 2024-04-05 01:00:59.000000 geeViz-2024.4.1/geeViz/examples/lcmsViewerExample.py
+-rw-rw-rw-   0        0        0    23631 2024-01-19 23:21:46.000000 geeViz-2024.4.1/geeViz/examples/lcmsViewerExampleNotebook.ipynb
+-rw-rw-rw-   0        0        0     6262 2024-03-21 17:55:40.000000 geeViz-2024.4.1/geeViz/examples/mapBiomasViewerExample.py
+-rw-rw-rw-   0        0        0    13051 2024-01-20 01:32:55.000000 geeViz-2024.4.1/geeViz/examples/phEEnoVizWrapper.py
+-rw-rw-rw-   0        0        0     1038 2024-01-20 01:32:55.000000 geeViz-2024.4.1/geeViz/examples/taskTrackerExample.py
+-rw-rw-rw-   0        0        0     6194 2024-01-20 02:08:49.000000 geeViz-2024.4.1/geeViz/examples/timeLapseExample.py
+-rw-rw-rw-   0        0        0     9132 2024-03-19 17:03:58.000000 geeViz-2024.4.1/geeViz/foliumView.py
+-rw-rw-rw-   0        0        0     1741 2021-04-01 17:15:14.000000 geeViz-2024.4.1/geeViz/gcpLib.py
+-rw-rw-rw-   0        0        0    18888 2024-03-19 17:05:58.000000 geeViz-2024.4.1/geeViz/gee2Pandas.py
+drwxrwxrwx   0        0        0        0 2024-04-05 01:26:45.159132 geeViz-2024.4.1/geeViz/geeView/
+-rw-rw-rw-   0        0        0     7260 2024-02-07 20:42:41.000000 geeViz-2024.4.1/geeViz/geeView/foliumView.html
+-rw-rw-rw-   0        0        0     3321 2024-02-27 19:55:46.000000 geeViz-2024.4.1/geeViz/geeView/index.html
+drwxrwxrwx   0        0        0        0 2024-04-05 01:26:41.018162 geeViz-2024.4.1/geeViz/geeView/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 01:26:41.002536 geeViz-2024.4.1/geeViz/geeView/src/assets/
+drwxrwxrwx   0        0        0        0 2024-04-05 01:26:46.440484 geeViz-2024.4.1/geeViz/geeView/src/assets/images/
+-rw-rw-rw-   0        0        0     7295 2021-04-01 17:15:14.000000 geeViz-2024.4.1/geeViz/geeView/src/assets/images/EE-logo-150.png
+-rw-rw-rw-   0        0        0    10301 2021-04-01 17:15:14.000000 geeViz-2024.4.1/geeViz/geeView/src/assets/images/GEE.png
+-rw-rw-rw-   0        0        0     5692 2022-08-19 21:41:40.000000 geeViz-2024.4.1/geeViz/geeView/src/assets/images/GEE_logo_transparent.png
+-rw-rw-rw-   0        0        0     4551 2021-04-01 17:15:14.000000 geeViz-2024.4.1/geeViz/geeView/src/assets/images/RCR-logo.jpg
+-rw-rw-rw-   0        0        0    35328 2022-12-07 01:04:30.000000 geeViz-2024.4.1/geeViz/geeView/src/assets/images/Thumbs.db
+-rw-rw-rw-   0        0        0     8352 2021-04-01 17:15:14.000000 geeViz-2024.4.1/geeViz/geeView/src/assets/images/cumulative_icon.png
+-rw-rw-rw-   0        0        0     1502 2021-04-01 17:15:15.000000 geeViz-2024.4.1/geeViz/geeView/src/assets/images/layer_icon.png
+-rw-rw-rw-   0        0        0   230271 2022-06-28 20:18:38.000000 geeViz-2024.4.1/geeViz/geeView/src/assets/images/logos_usda-fs.svg
+-rw-rw-rw-   0        0        0   229463 2022-06-30 19:30:12.000000 geeViz-2024.4.1/geeViz/geeView/src/assets/images/logos_usda-fs_bn-dk-01.svg
+-rw-rw-rw-   0        0        0      635 2022-06-29 22:17:42.000000 geeViz-2024.4.1/geeViz/geeView/src/assets/images/menu-hamburger_ffffff.svg
+-rw-rw-rw-   0        0        0     1489 2021-04-01 17:15:15.000000 geeViz-2024.4.1/geeViz/geeView/src/assets/images/usdalogo.png
+-rw-rw-rw-   0        0        0     8174 2021-04-01 17:15:15.000000 geeViz-2024.4.1/geeViz/geeView/src/assets/images/usfslogo.png
+drwxrwxrwx   0        0        0        0 2024-04-05 01:26:41.018162 geeViz-2024.4.1/geeViz/geeView/src/gee/
+drwxrwxrwx   0        0        0        0 2024-04-05 01:26:46.690504 geeViz-2024.4.1/geeViz/geeView/src/gee/gee-libraries/
+-rw-rw-rw-   0        0        0    65322 2024-04-05 00:50:32.000000 geeViz-2024.4.1/geeViz/geeView/src/gee/gee-libraries/changeDetectionLib.js
+-rw-rw-rw-   0        0        0   112794 2024-04-05 00:50:32.000000 geeViz-2024.4.1/geeViz/geeView/src/gee/gee-libraries/getImagesLib.js
+drwxrwxrwx   0        0        0        0 2024-04-05 01:26:46.909305 geeViz-2024.4.1/geeViz/geeView/src/gee/gee-run/
+-rw-rw-rw-   0        0        0     3211 2024-04-05 01:23:07.000000 geeViz-2024.4.1/geeViz/geeView/src/gee/gee-run/runGeeViz.js
+drwxrwxrwx   0        0        0        0 2024-04-05 01:26:47.534323 geeViz-2024.4.1/geeViz/geeView/src/js/
+-rw-rw-rw-   0        0        0    45351 2020-01-16 17:35:18.000000 geeViz-2024.4.1/geeViz/geeView/src/js/gena-gee-palettes.js
+-rw-rw-rw-   0        0        0   468413 2024-04-05 00:50:32.000000 geeViz-2024.4.1/geeViz/geeView/src/js/lcms-viewer.min.js
+-rw-rw-rw-   0        0        0     1021 2023-03-08 18:47:59.000000 geeViz-2024.4.1/geeViz/geeView/src/js/load.min.js
+drwxrwxrwx   0        0        0        0 2024-04-05 01:26:47.612486 geeViz-2024.4.1/geeViz/geeView/src/styles/
+-rw-rw-rw-   0        0        0    32682 2024-04-05 00:50:32.000000 geeViz-2024.4.1/geeViz/geeView/src/styles/style.min.css
+-rw-rw-rw-   0        0        0    59855 2024-04-05 01:20:31.000000 geeViz-2024.4.1/geeViz/geeView.py
+-rw-rw-rw-   0        0        0   228998 2024-03-19 16:37:42.000000 geeViz-2024.4.1/geeViz/getImagesLib.py
+-rw-rw-rw-   0        0        0     7928 2024-03-19 17:06:25.000000 geeViz-2024.4.1/geeViz/migrateGEEAssets.py
+-rw-rw-rw-   0        0        0    25768 2024-03-19 17:09:18.000000 geeViz-2024.4.1/geeViz/phEEnoViz.py
+-rw-rw-rw-   0        0        0    11182 2024-03-19 17:10:37.000000 geeViz-2024.4.1/geeViz/taskManagerLib.py
+drwxrwxrwx   0        0        0        0 2024-04-05 01:26:47.659334 geeViz-2024.4.1/geeViz.egg-info/
+-rw-rw-rw-   0        0        0     4442 2024-04-05 01:26:40.000000 geeViz-2024.4.1/geeViz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2907 2024-04-05 01:26:40.000000 geeViz-2024.4.1/geeViz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 01:26:40.000000 geeViz-2024.4.1/geeViz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2024-04-05 01:26:40.000000 geeViz-2024.4.1/geeViz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-05 01:26:40.000000 geeViz-2024.4.1/geeViz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 01:26:47.753123 geeViz-2024.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     2587 2024-03-21 18:41:47.000000 geeViz-2024.4.1/setup.py
```

### Comparing `geeViz-2024.3.2/LICENSE` & `geeViz-2024.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/PKG-INFO` & `geeViz-2024.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geeViz
-Version: 2024.3.2
+Version: 2024.4.1
 Summary: A package to help with GEE data processing, analysis, and visualization
 Home-page: https://github.com/gee-community/geeViz
 Author: Ian Housman
 Author-email: ian.housman@gmail.com
 License: Apache
 Keywords: earthengine google remote sensing landsat sentinel modis forestry forest
 Classifier: Programming Language :: Python :: 3
@@ -39,15 +39,15 @@
 
 Ian Housman- ian.housman@usda.gov
 
 Josh Heyer- joshua.heyer@usda.gov
 
 Bonnie Ruefenacht- bonnie.ruefenacht@usda.gov
 
-<iframe src='https://gee-community.github.io/geeViz/build/html/index.html#' width='100%' height='500'  title='geeViz documentation'></iframe>
+## [Documentation (in progress)](https://gee-community.github.io/geeViz/build/html/index.html)
 
 ## Installing
 
 1. Become a trusted Google Earth Engine (GEE) tester (<https://signup.earthengine.google.com/#!/>)
 2. Install package using pip (`pip install geeViz`)
    folder
 3. Authenticate using the GEE cli in a cmd prompt (`earthengine authenticate`)
```

### Comparing `geeViz-2024.3.2/README.md` & `geeViz-2024.4.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 Ian Housman- ian.housman@usda.gov
 
 Josh Heyer- joshua.heyer@usda.gov
 
 Bonnie Ruefenacht- bonnie.ruefenacht@usda.gov
 
-<iframe src='https://gee-community.github.io/geeViz/build/html/index.html#' width='100%' height='500'  title='geeViz documentation'></iframe>
+## [Documentation (in progress)](https://gee-community.github.io/geeViz/build/html/index.html)
 
 ## Installing
 
 1. Become a trusted Google Earth Engine (GEE) tester (<https://signup.earthengine.google.com/#!/>)
 2. Install package using pip (`pip install geeViz`)
    folder
 3. Authenticate using the GEE cli in a cmd prompt (`earthengine authenticate`)
```

### Comparing `geeViz-2024.3.2/geeViz/assetManagerLib.py` & `geeViz-2024.4.1/geeViz/assetManagerLib.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/changeDetectionLib.py` & `geeViz-2024.4.1/geeViz/changeDetectionLib.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/cloudStorageManagerLib.py` & `geeViz-2024.4.1/geeViz/cloudStorageManagerLib.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/CCDCViz.py` & `geeViz-2024.4.1/geeViz/examples/CCDCViz.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/CCDCVizNotebook.ipynb` & `geeViz-2024.4.1/geeViz/examples/CCDCVizNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/CCDCWrapper.py` & `geeViz-2024.4.1/geeViz/examples/CCDCWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/GFSTimeLapse.py` & `geeViz-2024.4.1/geeViz/examples/GFSTimeLapse.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/LANDTRENDRViz.py` & `geeViz-2024.4.1/geeViz/examples/LANDTRENDRViz.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/LANDTRENDRWrapper.py` & `geeViz-2024.4.1/geeViz/examples/LANDTRENDRWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb` & `geeViz-2024.4.1/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/LCMAP_and_LCMS_Viewer.py` & `geeViz-2024.4.1/geeViz/examples/LCMAP_and_LCMS_Viewer.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb` & `geeViz-2024.4.1/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/data/gadm41_CHE_shp/gadm41_CHE_0.geojson` & `geeViz-2024.4.1/geeViz/examples/data/gadm41_CHE_shp/gadm41_CHE_0.geojson`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/data/gadm41_CHE_shp/gadm41_CHE_0.shp` & `geeViz-2024.4.1/geeViz/examples/data/gadm41_CHE_shp/gadm41_CHE_0.shp`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/foliumViewerExample.py` & `geeViz-2024.4.1/geeViz/examples/foliumViewerExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/gee2PandasExample.ipynb` & `geeViz-2024.4.1/geeViz/examples/gee2PandasExample.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/geeViewExample.py` & `geeViz-2024.4.1/geeViz/examples/geeViewExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/geeViewExampleNotebook.ipynb` & `geeViz-2024.4.1/geeViz/examples/geeViewExampleNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/geeViewVSFoliumViewerExampleNotebook.ipynb` & `geeViz-2024.4.1/geeViz/examples/geeViewVSFoliumViewerExampleNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/geeViz_and_geemap.py` & `geeViz-2024.4.1/geeViz/examples/geeViz_and_geemap.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/getClimateWrapper.py` & `geeViz-2024.4.1/geeViz/examples/getClimateWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py` & `geeViz-2024.4.1/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/getLandsatWrapper.py` & `geeViz-2024.4.1/geeViz/examples/getLandsatWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/getLandsatWrapperNotebook.ipynb` & `geeViz-2024.4.1/geeViz/examples/getLandsatWrapperNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/getSentinel2Wrapper.py` & `geeViz-2024.4.1/geeViz/examples/getSentinel2Wrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/harmonicRegressionWrapper.py` & `geeViz-2024.4.1/geeViz/examples/harmonicRegressionWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/lcmsViewerExample.py` & `geeViz-2024.4.1/geeViz/examples/lcmsViewerExample.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,35 +41,28 @@
 #############################################################################
 startYear = 1985
 endYear = 2022
 lossYearPalette = ["ffffe5", "fff7bc", "fee391", "fec44f", "fe9929", "ec7014", "cc4c02"]
 gainYearPalette = ["c5ee93", "00a398"]
 durationPalette = ["BD1600", "E2F400", "0C2780"]
 
-lossYearPalette = geeView.get_poly_gradient_ct(lossYearPalette, startYear, endYear)
-gainYearPalette = geeView.get_poly_gradient_ct(gainYearPalette, startYear, endYear)
+
 lossYearViz = {
     "min": startYear,
     "max": endYear,
     "palette": lossYearPalette,
     "canAreaChart": True,
-    "areaChartParams": {
-        "reducer": ee.Reducer.frequencyHistogram(),
-        "palette": lossYearPalette,
-    },
+    "areaChartParams": {"reducer": ee.Reducer.frequencyHistogram()},
 }
 gainYearViz = {
     "min": startYear,
     "max": endYear,
     "palette": gainYearPalette,
     "canAreaChart": True,
-    "areaChartParams": {
-        "reducer": ee.Reducer.frequencyHistogram(),
-        "palette": gainYearPalette,
-    },
+    "areaChartParams": {"reducer": ee.Reducer.frequencyHistogram()},
 }
 durationViz = {"min": 1, "max": 5, "palette": durationPalette}
 #############################################################################
 ### Define functions ###
 #############################################################################
 
 # Convert given code to year that number was present in the image.
```

### Comparing `geeViz-2024.3.2/geeViz/examples/lcmsViewerExampleNotebook.ipynb` & `geeViz-2024.4.1/geeViz/examples/lcmsViewerExampleNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/mapBiomasViewerExample.py` & `geeViz-2024.4.1/geeViz/examples/mapBiomasViewerExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/phEEnoVizWrapper.py` & `geeViz-2024.4.1/geeViz/examples/phEEnoVizWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/taskTrackerExample.py` & `geeViz-2024.4.1/geeViz/examples/taskTrackerExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/examples/timeLapseExample.py` & `geeViz-2024.4.1/geeViz/examples/timeLapseExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/foliumView.py` & `geeViz-2024.4.1/geeViz/foliumView.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/gcpLib.py` & `geeViz-2024.4.1/geeViz/gcpLib.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/gee2Pandas.py` & `geeViz-2024.4.1/geeViz/gee2Pandas.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/geeView/foliumView.html` & `geeViz-2024.4.1/geeViz/geeView/foliumView.html`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/geeView/index.html` & `geeViz-2024.4.1/geeViz/geeView/index.html`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/geeView/src/assets/images/EE-logo-150.png` & `geeViz-2024.4.1/geeViz/geeView/src/assets/images/EE-logo-150.png`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/geeView/src/assets/images/GEE.png` & `geeViz-2024.4.1/geeViz/geeView/src/assets/images/GEE.png`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/geeView/src/assets/images/GEE_logo_transparent.png` & `geeViz-2024.4.1/geeViz/geeView/src/assets/images/GEE_logo_transparent.png`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/geeView/src/assets/images/RCR-logo.jpg` & `geeViz-2024.4.1/geeViz/geeView/src/assets/images/RCR-logo.jpg`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/geeView/src/assets/images/Thumbs.db` & `geeViz-2024.4.1/geeViz/geeView/src/assets/images/Thumbs.db`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/geeView/src/assets/images/cumulative_icon.png` & `geeViz-2024.4.1/geeViz/geeView/src/assets/images/cumulative_icon.png`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/geeView/src/assets/images/layer_icon.png` & `geeViz-2024.4.1/geeViz/geeView/src/assets/images/layer_icon.png`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/geeView/src/assets/images/logos_usda-fs.svg` & `geeViz-2024.4.1/geeViz/geeView/src/assets/images/logos_usda-fs.svg`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/geeView/src/assets/images/logos_usda-fs_bn-dk-01.svg` & `geeViz-2024.4.1/geeViz/geeView/src/assets/images/logos_usda-fs_bn-dk-01.svg`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/geeView/src/assets/images/menu-hamburger_ffffff.svg` & `geeViz-2024.4.1/geeViz/geeView/src/assets/images/menu-hamburger_ffffff.svg`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/geeView/src/assets/images/usdalogo.png` & `geeViz-2024.4.1/geeViz/geeView/src/assets/images/usdalogo.png`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/geeView/src/assets/images/usfslogo.png` & `geeViz-2024.4.1/geeViz/geeView/src/assets/images/usfslogo.png`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/geeView/src/gee/gee-libraries/changeDetectionLib.js` & `geeViz-2024.4.1/geeViz/geeView/src/gee/gee-libraries/changeDetectionLib.js`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/geeView/src/gee/gee-libraries/getImagesLib.js` & `geeViz-2024.4.1/geeViz/geeView/src/gee/gee-libraries/getImagesLib.js`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/geeView/src/js/gena-gee-palettes.js` & `geeViz-2024.4.1/geeViz/geeView/src/js/gena-gee-palettes.js`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/geeView/src/js/lcms-viewer.min.js` & `geeViz-2024.4.1/geeViz/geeView/src/js/lcms-viewer.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -577,14 +577,20 @@
     geeAPIURL = null;
     ee.data.setAuthToken("", "Bearer", urlParams.accessToken, 3600, [], undefined, false);
 }
 var projectID = null;
 if (urlParams.projectID !== null && urlParams.projectID !== undefined && urlParams.projectID !== "None") {
     projectID = urlParams.projectID;
 }
+if (urlParams.layerProps === undefined || urlParams.layerProps === null) {
+    urlParams.layerProps = {};
+}
+if (urlParams.cumulativeMode === undefined || urlParams.cumulativeMode === null) {
+    urlParams.cumulativeMode = false;
+}
 var plotsOn = false;
 Array.prototype.max = function() {
     return Math.max.apply(null, this);
 };
 Array.prototype.min = function() {
     return Math.min.apply(null, this);
 };
@@ -3025,15 +3031,15 @@
     }
     if (layer.viz.isTimeLapse) {
         timeLapseObj[layer.viz.timeLapseID].loadingLayerIDs.push(id);
         timeLapseObj[layer.viz.timeLapseID].sliders.push(opacityID);
         timeLapseObj[layer.viz.timeLapseID].layerVisibleIDs.push(visibleID);
         isDraggable = "not-draggable-layer";
     }
-    if (layer.layerType === "geeVector" || layer.layerType === "geoJSONVector") {
+    if (layer.layerType === "geeVector" || layer.layerType === "geoJSONVector" || layer.layerType === "dynamicMapService") {
         isDraggable = "not-draggable-layer";
     }
     $("#" + layer.whichLayerList).prepend(`<li id = '${containerID}' aria-label="Map layer controls container for ${layer.name}" class = 'layer-container ${isDraggable}'  title= '${layer.helpBoxMessage}'>
 								           <div id="${opacityID}" aria-labelledby="${containerID}" aria-label="Opacity range slider for ${layer.name}" class = 'simple-layer-opacity-range'></div>
 								           <input  role="option" id="${visibleID}" aria-label="Layer visibility toggle checkbox for ${layer.name}" type="checkbox" ${checked}  />
 								            <label class = 'layer-checkbox' id="${visibleLabelID}" aria-label="Layer visibility toggle checkbox for ${layer.name}" style = 'margin-bottom:0px;display:none;'  for="${visibleID}"></label>
 								            <i id = "${spinnerID}" class="fa fa-spinner fa-spin layer-spinner" title='Waiting for layer service from Google Earth Engine'></i>
@@ -3045,14 +3051,17 @@
     $("#" + opacityID).slider({
         min: 0,
         max: 100,
         step: 1,
         value: layer.opacity * 100,
         slide: function(e, ui) {
             layer.opacity = ui.value / 100;
+            if (layer.viz.isTimeLapse === false) {
+                urlParams.layerProps[layer.id].opacity = layer.opacity;
+            }
             if (layer.layerType !== "geeVector" && layer.layerType !== "geoJSONVector") {
                 layer.layer.setOpacity(layer.opacity);
             } else {
                 var style = layer.layer.getStyle();
                 style.strokeOpacity = layer.opacity;
                 style.fillOpacity = layer.opacity / layer.viz.opacityRatio;
                 layer.layer.setStyle(style);
@@ -3105,14 +3114,17 @@
         console.log(containerID);
         $("#" + containerID).css("background", "red");
         $("#" + containerID).attr("title", 'Layer failed to load. Error message: "' + failure + '"');
     }
 
     function turnOff() {
         ga("send", "event", "layer-off", layer.layerType, layer.name);
+        if (!layer.viz.isTimeLapse) {
+            urlParams.layerProps[id].visible = false;
+        }
         if (layer.layerType === "dynamicMapService") {
             layer.layer.setMap(null);
             layer.visible = false;
             layer.percent = 0;
             layer.rangeOpacity = 0;
             setRangeSliderThumbOpacity();
             updateProgress();
@@ -3151,14 +3163,15 @@
         vizToggleCleanup();
     }
 
     function turnOn() {
         ga("send", "event", "layer-on", layer.layerType, layer.name);
         if (!layer.viz.isTimeLapse) {
             turnOffTimeLapseCheckboxes();
+            urlParams.layerProps[id].visible = true;
         }
         if (layer.layerType === "dynamicMapService") {
             layer.layer.setMap(map);
             layer.visible = true;
             layer.percent = 100;
             layer.rangeOpacity = layer.opacity;
             setRangeSliderThumbOpacity();
@@ -3169,15 +3182,17 @@
             layer.map.overlayMapTypes.setAt(layer.layerId, layer.layer);
             $("#" + layer.legendDivID).show();
             layer.rangeOpacity = layer.opacity;
             if (layer.isTileMapService) {
                 layer.percent = 100;
                 updateProgress();
             }
-            layer.layer.setOpacity(layer.opacity);
+            if (!layer.viz.isTimeLapse) {
+                layer.layer.setOpacity(layer.opacity);
+            }
             if (layer.layerType !== "tileMapService" && layer.layerType !== "dynamicMapService" && layer.canQuery) {
                 queryObj[queryID].visible = layer.visible;
             }
         } else {
             layer.visible = true;
             layer.percent = 100;
             updateProgress();
@@ -3292,14 +3307,17 @@
                     layer.viz.reducer = ee.Deserializer.fromJSON(layer.viz.reducer);
                 } catch (err) {
                     layer.viz.reducer = eval(layer.viz.reducer);
                 }
             }
             var bandNames = ee.Image(layer.item.first()).bandNames();
             layer.item = ee.Image(ee.ImageCollection(layer.item).reduce(layer.viz.reducer).rename(bandNames).copyProperties(layer.imageCollection.first()).set(layer.item.toDictionary()));
+            if (layer.viz.selfMask === true) {
+                layer.item = layer.item.selfMask();
+            }
         } else if (layer.layerType === "geeVectorImage" || layer.layerType === "geeVector") {
             if (layer.viz.isSelectLayer) {
                 selectedFeaturesJSON[layer.name] = {
                     layerName: layer.name,
                     filterList: [],
                     geoJSON: new google.maps.Data(),
                     id: layer.id,
@@ -3391,14 +3409,18 @@
                 timeLapseObj[layer.viz.timeLapseID].loadingLayerIDs = timeLapseObj[layer.viz.timeLapseID].loadingLayerIDs.filter((timeLapseLayerID) => timeLapseLayerID !== id);
                 var prop = parseInt((1 - timeLapseObj[layer.viz.timeLapseID].loadingLayerIDs.length / timeLapseObj[layer.viz.timeLapseID].nFrames) * 100);
                 $("#" + layer.viz.timeLapseID + "-collapse-label").css("background", `-webkit-linear-gradient(left, #FFF, #FFF ${prop}%, transparent ${prop}%, transparent 100%)`);
                 if (timeLapseObj[layer.viz.timeLapseID].loadingLayerIDs.length === 0) {
                     $("#" + layer.viz.timeLapseID + "-loading-spinner").hide();
                     $("#" + layer.viz.timeLapseID + "-year-label").hide();
                     $("#" + layer.viz.timeLapseID + "-collapse-label").css("background", `-webkit-linear-gradient(left, #FFF, #FFF ${0}%, transparent ${0}%, transparent 100%)`);
+                    if (timeLapseObj[layer.viz.timeLapseID].userChosenVisible === true) {
+                        console.log("here");
+                        $("#" + layer.viz.timeLapseID + "-toggle-checkbox-label").click();
+                    }
                     $("#" + layer.viz.timeLapseID + "-toggle-checkbox-label").show();
                     timeLapseObj[layer.viz.timeLapseID].isReady = true;
                 }
             }
             $("#" + visibleLabelID).show();
             if (layer.currentGEERunID === geeRunID) {
                 if (eeLayer === undefined) {
@@ -3502,14 +3524,20 @@
                 $("#" + layer.viz.timeLapseID + "-collapse-label").css("background", `-webkit-linear-gradient(left, #FFF, #FFF ${prop}%, transparent ${prop}%, transparent 100%)`);
                 if (timeLapseObj[layer.viz.timeLapseID].loadingLayerIDs.length === 0) {
                     $("#" + layer.viz.timeLapseID + "-loading-spinner").hide();
                     $("#" + layer.viz.timeLapseID + "-year-label").hide();
                     $("#" + layer.viz.timeLapseID + "-collapse-label").css("background", `-webkit-linear-gradient(left, #FFF, #FFF ${0}%, transparent ${0}%, transparent 100%)`);
                     $("#" + layer.viz.timeLapseID + "-toggle-checkbox-label").show();
                     timeLapseObj[layer.viz.timeLapseID].isReady = true;
+                    if (urlParams.layerProps[layer.viz.timeLapseID].visible === true) {
+                        timeLapseCheckbox(layer.viz.timeLapseID);
+                    }
+                    if (urlParams.cumulativeMode === true) {
+                        turnOnCumulativeMode();
+                    }
                 }
             }
             $("#" + visibleLabelID).show();
             if (layer.currentGEERunID === geeRunID) {
                 if (eeLayer === undefined || failure !== undefined) {
                     loadFailure(failure);
                 } else {
@@ -5652,15 +5680,15 @@
     viz.canQuery = false;
     viz.isSelectLayer = true;
     addToMap(item, viz, name, visible, label, fontColor, helpBox, "area-charting-select-layer-list", queryItem);
 }
 var intervalPeriod = 666.6666666666666;
 var timeLapseID;
 var timeLapseFrame = 0;
-var cumulativeMode = false;
+var cumulativeMode = urlParams.cumulativeMode;
 
 function pauseTimeLapse(id) {
     if (id === null || id === undefined) {
         id = timeLapseID;
     }
     timeLapseID = id;
     if (timeLapseObj[timeLapseID].isReady) {
@@ -5941,14 +5969,15 @@
     return jittered;
 }
 
 function alignTimeLapseCheckboxes() {
     Object.keys(timeLapseObj).map(function(k) {
         if (timeLapseObj[k].isReady) {
             var checked = false;
+            urlParams.layerProps[k].visible = timeLapseObj[k].visible;
             if (timeLapseObj[k].visible) {
                 checked = true;
                 $("#" + k + "-time-lapse-layer-range-container").slideDown();
                 $("#" + k + "-icon-bar").slideDown();
                 $("#" + k + "-collapse-label").addClass("time-lapse-label-container");
             } else {
                 $("#" + k + "-collapse-label").css("background", `-webkit-linear-gradient(left, #FFF, #FFF ${0}%, transparent ${0}%, transparent 100%)`);
@@ -5985,23 +6014,34 @@
                 stopTimeLapse(k);
             }
         }
     });
     alignTimeLapseCheckboxes();
 }
 
+function turnOnCumulativeMode() {
+    $(".cumulativeToggler").addClass("time-lapse-active");
+    cumulativeMode = true;
+    urlParams.cumulativeMode = cumulativeMode;
+    selectFrame();
+}
+
+function turnOffCumulativeMode() {
+    $(".cumulativeToggler").removeClass("time-lapse-active");
+    cumulativeMode = false;
+    urlParams.cumulativeMode = cumulativeMode;
+    selectFrame();
+}
+
 function toggleCumulativeMode() {
     if (cumulativeMode) {
-        $(".cumulativeToggler").removeClass("time-lapse-active");
-        cumulativeMode = false;
+        turnOffCumulativeMode();
     } else {
-        $(".cumulativeToggler").addClass("time-lapse-active");
-        cumulativeMode = true;
+        turnOnCumulativeMode();
     }
-    selectFrame();
 }
 
 function fillEmptyCollections(inCollection, dummyImage) {
     var dummyCollection = ee.ImageCollection([dummyImage.mask(ee.Image(0))]);
     var imageCount = inCollection.toList(1).length();
     return ee.ImageCollection(ee.Algorithms.If(imageCount.gt(0), inCollection, dummyCollection));
 }
@@ -6010,54 +6050,61 @@
     if (viz !== null && viz !== undefined && viz.serialized !== null && viz.serialized !== undefined && viz.serialized === true) {
         item = ee.Deserializer.decode(item);
         if (viz.areaChartParams !== undefined && viz.areaChartParams !== null && viz.areaChartParams.reducer !== undefined && viz.areaChartParams.reducer !== null) {
             viz.areaChartParams.reducer = ee.Deserializer.fromJSON(viz.areaChartParams.reducer);
         }
         viz.serialized = false;
     }
-    if (viz.cumulativeMode === null || viz.cumulativeMode === undefined) {
-        viz.cumulativeMode = false;
-    }
     if (viz.canAreaChart === undefined || viz.canAreaChart === null) {
         viz.canAreaChart = false;
     }
     var visible = false;
     if (viz.opacity === undefined || viz.opacity === null) {
         viz.opacity = 1;
     }
+    if (viz.bands !== undefined && typeof viz.bands === "string") {
+        viz.bands = viz.bands.split(",");
+    }
+    if (viz.palette !== undefined && typeof viz.palette === "string") {
+        viz.palette = viz.palette.split(",");
+    }
     item = ee.ImageCollection(item);
-    let dictServerSide = true;
+    viz.dictServerSide = true;
     if (viz.eeObjInfo === undefined || viz.eeObjInfo === null) {
         viz.eeObjInfo = getImagesLib.eeObjInfo(item, "ImageCollection");
     } else {
         viz.eeObjInfo = ee.Dictionary(viz.eeObjInfo);
     }
     if (viz.autoViz === true && (viz.class_names === undefined || viz.class_names === null)) {
         console.log("start");
         console.log(name);
         viz.eeObjInfo = viz.eeObjInfo.getInfo();
-        dictServerSide = false;
+        viz.dictServerSide = false;
         viz = addClassVizDicts(viz);
         console.log(viz);
     }
     if (name == undefined || name == null) {
         name = "Layer " + NEXT_LAYER_ID;
     }
     var checked = "";
-    if (visible) {
-        checked = "checked";
-    }
     var legendDivID = name.replaceAll(" ", "-") + "-" + NEXT_LAYER_ID.toString();
     legendDivID = legendDivID.replace(/[^A-Za-z0-9]/g, "-");
+    if (urlParams.layerProps[legendDivID] === undefined || urlParams.layerProps[legendDivID] === null) {
+        urlParams.layerProps[legendDivID] = {};
+        urlParams.layerProps[legendDivID].visible = false;
+        urlParams.layerProps[legendDivID].opacity = viz.opacity || 1;
+    } else {
+        viz.opacity = urlParams.layerProps[legendDivID].opacity || 1;
+    }
     if (viz.autoViz) {
-        if (dictServerSide) {
+        if (viz.dictServerSide) {
             console.log("start");
             console.log(name);
             viz.eeObjInfo = viz.eeObjInfo.getInfo();
-            dictServerSide = false;
+            viz.dictServerSide = false;
             console.log(viz);
         }
         if (viz.bands === undefined || viz.bands === null) {
             viz.bands = viz.eeObjInfo.bandNames;
         }
         viz.bands = viz.bands[0];
         dicts = getLookupDicts(viz.bands, viz.class_values, viz.class_names, viz.class_palette);
@@ -6174,15 +6221,15 @@
         viz.years.map(function(yr) {
             if (yr !== viz.years[0]) {
                 viz.addToLegend = false;
                 viz.addToClassLegend = false;
             }
             var vizT = Object.assign({}, viz);
             vizT.year = yr;
-            addToMap(standardTileURLFunction(item + yr.toString() + "/", true, ""), vizT, name + " " + yr.toString(), visible, label, fontColor, helpBox, legendDivID + "-collapse-div", queryItem);
+            addToMap(standardTileURLFunction(item + yr.toString() + "/", true, ""), vizT, name + " " + yr.toString(), false, label, fontColor, helpBox, legendDivID + "-collapse-div", queryItem);
         });
     } else {
         var dummyImage = ee.Image(item.first());
         var cT = [];
         viz.years.map(function(yr) {
             var d = ee.Date.parse(viz.dateFormat.replaceAll("-", ""), yr.toString());
             if (viz.dateField !== "system:time_start") {
@@ -6205,22 +6252,22 @@
             }
             var vizT = Object.assign({}, viz);
             vizT.year = yr;
             vizT.layerType = "geeImage";
             vizT.canAreaChart = false;
             vizT.legendTitle = name;
             vizT.opacity = 0;
-            addToMap(ee.Image(img), vizT, name + " " + yr.toString(), visible, label, fontColor, helpBox, legendDivID + "-collapse-div", queryItem);
+            addToMap(ee.Image(img), vizT, name + " " + yr.toString(), false, label, fontColor, helpBox, legendDivID + "-collapse-div", queryItem);
         });
         if (viz.dateField !== "system:time_start" || viz.canAreaChart) {
             item = ee.ImageCollection(cT);
         }
         if (viz.canAreaChart) {
             let vizTT = copyObj(viz);
-            vizTT = setupAreaChartParams(vizTT, dictServerSide, legendDivID);
+            vizTT = setupAreaChartParams(vizTT, legendDivID);
             if (vizTT.areaChartParams.sankey && vizTT.areaChartParams.line) {
                 let areaChartParamsLine = copyObj(vizTT.areaChartParams);
                 areaChartParamsLine.sankey = false;
                 areaChartParamsLine.line = true;
                 areaChartParamsLine.id = `${vizTT.areaChartParams.id}-----line`;
                 areaChart.addLayer(item, areaChartParamsLine, name, visible);
                 let areaChartParamsSankey = copyObj(vizTT.areaChartParams);
@@ -6253,14 +6300,15 @@
     $("#" + legendDivID + "-opacity-slider").slider({
         min: 0,
         max: 1,
         step: 0.05,
         value: timeLapseObj[legendDivID].opacity / 100,
         slide: function(e, ui) {
             var opacity = ui.value;
+            urlParams.layerProps[legendDivID].opacity = opacity;
             var k = legendDivID;
             var s = $("#" + k + "-opacity-slider").slider();
             s.slider("option", "value", ui.value);
             $("#" + k + "-opacity-slider-handle-label").text(opacity);
             timeLapseObj[k].opacity = opacity * 100;
             selectFrame(null, null, false);
             setTimeLapseRangeSliderThumbOpacity(opacity);
@@ -6363,50 +6411,54 @@
     });
     $("#" + name + "-checkbox-" + exportID.toString()).on("change", function() {
         exportImageDict[exportElement.ID].shouldExport = this.checked;
     });
     exportID++;
 }
 
-function setupAreaChartParams(viz, dictServerSide, legendDivID) {
+function setupAreaChartParams(viz, legendDivID) {
     viz.areaChartParams = viz.areaChartParams || {};
     viz.areaChartParams.sankey = viz.areaChartParams.sankey || false;
     viz.areaChartParams.line = viz.areaChartParams.line || viz.areaChartParams.sankey == false;
     viz.areaChartParams.id = legendDivID;
-    if ((viz.bands === undefined || viz.bands === null) && dictServerSide) {
+    if ((viz.areaChartParams.bandNames === undefined || viz.areaChartParams.bandNames === null) && (viz.bands === undefined || viz.bands === null) && viz.dictServerSide) {
         console.log("start");
         viz.eeObjInfo = viz.eeObjInfo.getInfo();
-        dictServerSide = false;
+        viz.dictServerSide = false;
         console.log(viz);
     }
-    viz.areaChartParams.bandNames = viz.bands || viz.eeObjInfo.bandNames;
-    if ((viz.class_names === undefined || viz.class_names === null) && dictServerSide) {
+    viz.areaChartParams.bandNames = viz.areaChartParams.bandNames || viz.bands || viz.eeObjInfo.bandNames;
+    if (viz.autoViz && (viz.class_names === undefined || viz.class_names === null) && viz.dictServerSide) {
         console.log("start");
         viz.eeObjInfo = viz.eeObjInfo.getInfo();
         console.log(viz);
-        dictServerSide = false;
+        viz.dictServerSide = false;
     }
-    if (viz.class_names === undefined || viz.class_names === null) {
+    if ((viz.autoViz && viz.class_names === undefined) || viz.class_names === null) {
         viz = addClassVizDicts(viz);
         viz.areaChartParams.class_dicts_added = true;
+    } else if ((viz.areaChartParams.palette === undefined || viz.areaChartParams.palette === null) && viz.areaChartParams.reducer !== undefined && viz.areaChartParams.reducer !== null && viz.min !== undefined && viz.min !== null && viz.max !== undefined && viz.max !== null && viz.palette !== undefined && viz.palette !== null) {
+        viz.areaChartParams.palette_lookup = toObj(range(viz.min, viz.max + 1), get_poly_gradient_ct(viz.palette, viz.min, viz.max));
     }
     viz.areaChartParams.class_values = viz.class_values;
     viz.areaChartParams.class_names = viz.class_names;
     viz.areaChartParams.class_palette = viz.class_palette;
     viz.areaChartParams.class_visibility = viz.class_visibility;
     viz.areaChartParams.layerType = viz.areaChartParams.layerType || viz.eeObjectType;
+    viz.areaChartParams.eeObjInfo = viz.eeObjInfo;
+    viz.areaChartParams.dictServerSide = viz.dictServerSide;
     return viz;
 }
 
 function addClassVizDicts(viz) {
     let cls_names_keys = Object.keys(viz.eeObjInfo).filter((k) => k.indexOf("_class_names") > -1);
     if (cls_names_keys.length > 0) {
         let bns = cls_names_keys.map((k) => k.split("_class_names")[0]);
         bns = bns.filter((bn) => viz.eeObjInfo.bandNames.indexOf(bn) > -1);
-        if (bns.length === 1) {
+        if (bns.length >= 1) {
             viz.autoViz = true;
             viz.class_names = {};
             viz.class_values = {};
             viz.class_palette = {};
             viz.class_visibility = {};
             bns.map((bn) => {
                 let cns = viz.eeObjInfo[`${bn}_class_names`];
@@ -6461,36 +6513,35 @@
     if (viz === null || viz === undefined) {
         viz = {};
     }
     if (name === undefined || name === null) {
         name = "Layer " + NEXT_LAYER_ID;
     }
     viz.isTimeLapse = viz.isTimeLapse || false;
-    let dictServerSide = true;
-    if (viz.eeObjInfo === undefined || viz.eeObjInfo === null) {
+    viz.dictServerSide = true;
+    if (viz.layerType !== "geoJSONVector" && viz.layerType !== "tileMapService" && viz.layerType !== "dynamicMapService" && (viz.eeObjInfo === undefined || viz.eeObjInfo === null)) {
         viz.eeObjInfo = getImagesLib.eeObjInfo(item, reverseTypeLookup[viz.layerType]);
     } else {
         viz.eeObjInfo = ee.Dictionary(viz.eeObjInfo);
     }
     if (viz.autoViz === true && (viz.class_names === undefined || viz.class_names === null) && viz.layerType !== "geoJSONVector" && viz.layerType !== "tileMapService" && viz.layerType !== "dynamicMapService") {
         console.log("start");
         console.log(name);
         viz.eeObjInfo = viz.eeObjInfo.getInfo();
-        dictServerSide = false;
+        viz.dictServerSide = false;
         viz = addClassVizDicts(viz);
         console.log(viz);
     }
     if (viz.layerType === null || viz.layerType === undefined) {
-        if (dictServerSide) {
+        if (viz.dictServerSide) {
             console.log("start");
             console.log(name);
             viz.eeObjInfo = viz.eeObjInfo.getInfo();
             console.log(viz);
-            dictServerSide = false;
-            viz = addClassVizDicts(viz);
+            viz.dictServerSide = false;
         }
         var eeType = viz.eeObjInfo.layerType;
         if (eeType === "Feature") {
             item = ee.FeatureCollection([item]);
             viz.eeObjInfo.layerType = "FeatureCollection";
             eeType = "FeatureCollection";
         }
@@ -6549,18 +6600,35 @@
             viz.strokeColor = "#" + viz.strokeColor;
         }
         if (viz.addToClassLegend === undefined || viz.addToClassLegend === null) {
             viz.addToClassLegend = true;
             viz.addToLegend = false;
         }
     }
+    if (viz.bands !== undefined && typeof viz.bands === "string") {
+        viz.bands = viz.bands.split(",");
+    }
+    if (viz.palette !== undefined && typeof viz.palette === "string") {
+        viz.palette = viz.palette.split(",");
+    }
     var legendDivID = name.replaceAll(" ", "-") + "-" + NEXT_LAYER_ID.toString();
     legendDivID = legendDivID.replace(/[^A-Za-z0-9]/g, "-");
+    if (viz.isTimeLapse === false) {
+        if (urlParams.layerProps[legendDivID] === undefined || urlParams.layerProps[legendDivID] === null) {
+            urlParams.layerProps[legendDivID] = {};
+            urlParams.layerProps[legendDivID].visible = visible === undefined ? true : visible;
+            urlParams.layerProps[legendDivID].opacity = viz.opacity || 1;
+        } else {
+            visible = urlParams.layerProps[legendDivID].visible;
+            viz.opacity = urlParams.layerProps[legendDivID].opacity;
+        }
+    }
     if (viz.canAreaChart) {
-        viz = setupAreaChartParams(viz, dictServerSide, legendDivID);
+        viz = setupAreaChartParams(viz, legendDivID);
+        console.log(viz.areaChartParams);
         if (viz.areaChartParams.sankey && viz.areaChartParams.line) {
             let areaChartParamsLine = copyObj(viz.areaChartParams);
             areaChartParamsLine.sankey = false;
             areaChartParamsLine.line = true;
             areaChartParamsLine.id = `${viz.areaChartParams.id}-----line`;
             areaChart.addLayer(item, areaChartParamsLine, name, visible);
             let areaChartParamsSankey = copyObj(viz.areaChartParams);
@@ -6574,17 +6642,14 @@
     }
     if (visible == null) {
         visible = true;
     }
     if (viz.opacity == null) {
         viz.opacity = 1;
     }
-    if (viz.bands !== undefined && typeof viz.bands === "string") {
-        viz.bands = viz.bands.split(",");
-    }
     var layerObjKeys = Object.keys(layerObj);
     var nameIndex = layerObjKeys.indexOf(legendDivID);
     if (nameIndex != -1) {
         visible = layerObj[legendDivID].visible;
         viz.opacity = layerObj[legendDivID].opacity;
         if (viz.layerType === "geeVector" || viz.layerType === "geoJSONVector") {
             viz.strokeOpacity = layerObj[legendDivID].opacity;
@@ -6618,19 +6683,19 @@
     if (viz.canQuery === null || viz.canQuery === undefined) {
         viz.canQuery = true;
     }
     layer.canQuery = viz.canQuery;
     layer.queryItem = queryItem;
     layer.layerType = viz.layerType;
     if (viz.autoViz && viz.isTimeLapse === false) {
-        if (dictServerSide) {
+        if (viz.dictServerSide) {
             console.log("start");
             console.log(name);
             viz.eeObjInfo = viz.eeObjInfo.getInfo();
-            dictServerSide = false;
+            viz.dictServerSide = false;
             viz = addClassVizDicts(viz);
             console.log(viz);
         }
         if (viz.bands === undefined || viz.bands === null) {
             viz.bands = viz.eeObjInfo.bandNames;
         }
         viz.bands = viz.bands[0];
@@ -7169,15 +7234,15 @@
     areaChartCollections = {};
     pixelChartCollections = {};
     timeLapseObj = {};
     dashboardObj = {};
     intervalPeriod = 666.6666666;
     timeLapseID = null;
     timeLapseFrame = 0;
-    cumulativeMode = false;
+    cumulativeMode = urlParams.cumulativeMode;
     NEXT_LAYER_ID = 1;
     clearSelectedAreas();
     selectedFeaturesGeoJSON = {};
     ["layer-list", "reference-layer-list", "area-charting-select-layer-list", "fhp-div", "time-lapse-legend-list"].map(function(l) {
         $("#" + l).empty();
         $("#legend-" + l).empty();
     });
@@ -7247,14 +7312,20 @@
         g = colors[1];
         b = colors[2];
     }
     return "#" + ("00000" + ((r << 16) | (g << 8) | b).toString(16)).slice(-6);
 }
 
 function hexToRgb(hex) {
+    if (hex.indexOf("#") === 0) {
+        hex = hex.slice(1);
+    }
+    if (hex.length === 3) {
+        hex = hex[0] + hex[0] + hex[1] + hex[1] + hex[2] + hex[2];
+    }
     var result = /^#?([a-f\d]{2})([a-f\d]{2})([a-f\d]{2})$/i.exec(hex);
     return result ? {
         r: parseInt(result[1], 16),
         g: parseInt(result[2], 16),
         b: parseInt(result[3], 16),
     } : null;
 }
@@ -7329,14 +7400,62 @@
     var out = [];
     while (n > 0) {
         out.push(randomColor());
         n = n - 1;
     }
     return out;
 }
+
+function linear_gradient(start_hex, finish_hex = "#FFFFFF", n = 10) {
+    s = Object.values(hexToRgb(start_hex));
+    f = Object.values(hexToRgb(finish_hex));
+    RGB_list = [s];
+    range(1, n).map((t) => {
+        curr_vector = range(0, 3).map((j) => {
+            return parseInt(s[j] + (parseFloat(t) / (n - 1)) * (f[j] - s[j]));
+        });
+        RGB_list.push(curr_vector);
+    });
+    let hex_list = RGB_list.map(rgbToHex);
+    return hex_list;
+}
+
+function polylinear_gradient(colors, n) {
+    n_out = parseInt(parseFloat(n) / (colors.length - 1)) + 1;
+    apply_offset = false;
+    if (n % n_out !== 0) {
+        apply_offset = true;
+        n_out = n_out + 1;
+    }
+    gradient_dict = linear_gradient(colors[0], colors[1], n_out);
+    if (colors.length > 2) {
+        range(1, colors.length - 1).map((col) => {
+            next = linear_gradient(colors[col], colors[col + 1], n_out).slice(1);
+            gradient_dict = gradient_dict.concat(next);
+        });
+    }
+    if (apply_offset === true) {
+        offset = gradient_dict.length - n;
+        sliceval = [];
+        range(1, offset + 1).map((i) => sliceval.push(parseInt((gradient_dict.length * i) / parseFloat(offset + 2))));
+        let out = [];
+        for (const [index, element] of gradient_dict.entries()) {
+            if (sliceval.indexOf(index) === -1) {
+                out.push(element);
+            }
+        }
+        gradient_dict = out;
+    }
+    return gradient_dict;
+}
+
+function get_poly_gradient_ct(palette, min, max) {
+    ramp = polylinear_gradient(palette, max - min + 1);
+    return ramp;
+}
 var colorList = ["#e6194b", "#3cb44b", "#ffe119", "#4363d8", "#f58231", "#911eb4", "#46f0f0", "#f032e6", "#bcf60c", "#fabebe", "#008080", "#e6beff", "#9a6324", "#fffac8", "#800000", "#aaffc3", "#808000", "#ffd8b1", "#000075", "#808080", "#ffffff", "#000000", ];
 var colorMod = colorList.length;
 
 function getColor() {
     var currentColor = colorList[colorMod % colorList.length];
     colorMod++;
     return currentColor;
@@ -10505,54 +10624,74 @@
     this.layerSelectContainerID = "area-chart-params-div";
     this.layerSelectID = "area-chart-layer-select";
     this.listeners = [];
     this.plot_bgcolor = "#D6D1CA";
     this.plot_font = "Roboto Condensed, sans-serif";
     this.autoChartingOn = false;
     this.firstRun = true;
-    this.sankeyTransitionPeriodYearBuffer = 2;
+    this.sankeyTransitionPeriodYearBuffer = 0;
     this.clearLayers = function() {
         this.areaChartObj = {};
         this.areaChartID = 1;
         this.clearCharts();
     };
     this.addLayer = function(eeLayer, params = {}, name, shouldChart = true) {
+        if (params !== null && params !== undefined && params.serialized !== null && params.serialized !== undefined && params.serialized === true) {
+            eeLayer = ee.Deserializer.decode(eeLayer);
+            if (params.reducer !== undefined && params.reducer !== null) {
+                params.reducer = ee.Deserializer.fromJSON(params.reducer);
+            }
+            params.serialized = false;
+        }
         $("#map-defined-area-chart-label").show();
         $("#area-collection-dropdown-container").hide();
         let obj = {};
         obj.name = name || `Area-Layer-${this.areaChartID}`;
         obj.id = params.id || obj.name.replaceAll(" ", "-") + "-" + this.areaChartID.toString();
         obj.id = obj.id.replace(/[^A-Za-z0-9]/g, "-");
-        obj.layerType = params.layerType || ee.Algorithms.ObjectType(eeLayer).getInfo();
+        if (params.dictServerSide !== undefined && params.dictServerSide !== null) {
+            obj.dictServerSide = params.dictServerSide;
+        } else {
+            obj.dictServerSide = true;
+        }
+        params.eeObjInfo = params.eeObjInfo || getImagesLib.eeObjInfo(eeLayer, obj.layerType);
+        if (params.layerType === undefined || params.layerType === null) {
+            if (obj.dictServerSide === true) {
+                console.log("start");
+                params.eeObjInfo = params.eeObjInfo.getInfo();
+                obj.dictServerSide = false;
+                console.log(params.eeObjInfo);
+            }
+            obj.layerType = params.eeObjInfo.layerType;
+        } else {
+            obj.layerType = params.layerType;
+        }
         eeLayer = obj.layerType === "ImageCollection" ? ee.ImageCollection(eeLayer) : ee.Image(eeLayer);
         if (obj.layerType !== "ImageCollection" && obj.layerType !== "Image") {
             setTimeout(() => showMessage("Area Chart addLayer Error", `Cannot add ee object type ${obj.layerType} as an area chart layer.<br>Accepted types are ee.ImageCollection and ee.Image`), 500);
         } else if (obj.layerType === "Image" && params.sankey === true) {
             setTimeout(() => showMessage("Area Chart addLayer Error", `Cannot add ee object type "${obj.layerType}" as an area chart layer sankey : true.<br>Accepted sankey GEE object types are "ImageCollection"`), 500);
         } else {
-            let dictServerSide = true;
-            params.eeObjInfo = getImagesLib.eeObjInfo(eeLayer, obj.layerType);
             if (params.bandNames === undefined || params.bandNames === null) {
-                if (dictServerSide) {
+                if (obj.dictServerSide) {
                     console.log("start");
                     params.eeObjInfo = params.eeObjInfo.getInfo();
-                    dictServerSide = false;
+                    obj.dictServerSide = false;
                     console.log(params);
                 }
                 obj.bandNames = params.eeObjInfo.bandNames;
             } else {
                 obj.bandNames = params.bandNames;
             }
             obj.bandNames = typeof obj.bandNames === "string" ? obj.bandNames.split(",") : obj.bandNames;
-            console.log(params);
             if ((params.class_names === undefined || params.class_names === null) && params.class_dicts_added !== true) {
-                if (dictServerSide) {
+                if (obj.dictServerSide) {
                     console.log("start");
                     params.eeObjInfo = params.eeObjInfo.getInfo();
-                    dictServerSide = false;
+                    obj.dictServerSide = false;
                     console.log(params);
                 }
                 params = addClassVizDicts(params);
             }
             obj.rangeSlider = params.rangeSlider === true ? {} : null;
             obj.item = eeLayer.select(obj.bandNames);
             obj.class_names = params.class_names || null;
@@ -10567,19 +10706,21 @@
                 obj.bandNames = Object.keys(obj.class_names);
                 obj.item = obj.item.select(obj.bandNames);
             }
             obj.palette = params.palette;
             if (typeof obj.palette === "string") {
                 obj.palette = obj.palette.split(",");
             }
+            obj.palette_lookup = params.palette_lookup;
             obj.chartType = params.chartType || "line";
             obj.stackedAreaChart = params.stackedAreaChart || false;
             obj.steppedLine = params.steppedLine || false;
             obj.label = obj.name;
             obj.xAxisLabel = params.xAxisLabel || obj.layerType === "ImageCollection" ? "Year" : "";
+            obj.xAxisLabels = params.xAxisLabels;
             obj.xAxisProperty = params.xAxisProperty || obj.layerType === "ImageCollection" ? "year" : "system:index";
             obj.size = obj.layerType === "ImageCollection" ? obj.item.size().getInfo() : 1;
             obj.dateFormat = params.dateFormat || "YYYY";
             obj.chartLabelFontSize = params.chartLabelFontSize || 10;
             obj.chartAxisTitleFontSize = params.chartAxisTitleFontSize || 12;
             obj.chartLabelMaxWidth = params.chartLabelMaxWidth || 15;
             obj.chartLabelMaxLength = params.chartLabelMaxLength || 50;
@@ -10632,44 +10773,49 @@
                         });
                     });
                     obj.sankey_class_names[bn] = bn_sankey_class_names;
                     obj.sankey_class_values[bn] = bn_sankey_class_values;
                     obj.sankey_class_palette[bn] = bn_sankey_class_palette;
                 });
             } else {
-                if (obj.xAxisProperty === "year") {
-                    if (obj.layerType === "ImageCollection") {
-                        let tempItem = obj.item.map(function(img) {
+                if (obj.xAxisLabels === undefined || obj.xAxisLabels === null) {
+                    if (obj.dictServerSide) {
+                        console.log("start");
+                        params.eeObjInfo = params.eeObjInfo.getInfo();
+                        obj.dictServerSide = false;
+                        console.log(params.eeObjInfo);
+                    }
+                    if (obj.layerType === "ImageCollection" && Object.keys(params.eeObjInfo).indexOf(obj.xAxisProperty) === -1) {
+                        console.log("need to add x axis property value");
+                        obj.item = obj.item.map(function(img) {
                             return img.set("year", img.date().format(obj.dateFormat));
                         });
-                        obj.xAxisLabels = tempItem.aggregate_histogram(obj.xAxisProperty).keys().getInfo();
-                    } else {
-                        let tempItem = obj.item.set("year", obj.item.date().format(obj.dateFormat));
-                        obj.xAxisLabels = [tempItem.get(obj.xAxisProperty).getInfo()];
                     }
-                } else {
                     if (obj.layerType === "ImageCollection") {
                         obj.xAxisLabels = obj.item.aggregate_histogram(obj.xAxisProperty).keys().getInfo();
                     } else {
-                        obj.xAxisLabels = [obj.item.get(obj.xAxisProperty).getInfo()];
+                        obj.xAxisLabels = [""];
                     }
                 }
+                obj.xAxisLabels = obj.xAxisLabels.map((l) => (isNaN(parseInt(l)) ? l : parseInt(l)));
                 if (obj.layerType === "ImageCollection") {
                     obj.stackBandNames = [];
                     obj.xAxisLabels.map((xLabel) => {
                         obj.bandNames.map((bn) => {
                             obj.stackBandNames.push(`${xLabel}${obj.splitStr}${bn}`);
                         });
                     });
                     if (obj.size > obj.xAxisLabels.length) {
                         console.log("Mosaicking for single image per x label");
                         let temp = [];
                         obj.xAxisLabels.map((l) => {
-                            l = isNaN(parseInt(l)) ? l : parseInt(l);
-                            temp.push(obj.item.filter(ee.Filter.eq(obj.xAxisProperty, l)).mosaic().set(obj.xAxisProperty, l));
+                            let t = obj.item.filter(ee.Filter.eq(obj.xAxisProperty, l));
+                            let f = t.first();
+                            t = t.mosaic().copyProperties(f).set(obj.xAxisProperty, l);
+                            temp.push(t);
                         });
                         obj.size = temp.length;
                         obj.item = ee.ImageCollection(temp);
                     }
                 } else {
                     obj.stackBandNames = obj.bandNames;
                 }
@@ -10843,25 +10989,27 @@
         if (selectedObj.layerType === "ImageCollection") {
             let xColumn = arrayColumn(table, 0).slice(1);
             let iOffset = selectedObj.layerType === "ImageCollection" ? 1 : 0;
             let header = table[0];
             table = table.slice(1);
             let yColumns = range(1, header.length);
             var data = yColumns.map((i) => {
+                let c = colors !== undefined ? colors[i - iOffset] : null;
                 return {
                     x: xColumn,
                     y: arrayColumn(table, i).map(smartToFixed),
                     visible: visible[i - 1],
                     name: header[i].slice(0, selectedObj.chartLabelMaxLength).chunk(selectedObj.chartLabelMaxWidth).join("<br>"),
                     line: {
-                        color: colors[i - iOffset]
+                        color: c
                     },
                 };
             });
         } else {
+            colors = colors || [randomColor()];
             colors = colors.indexOf(null) > -1 ? colors.map((c) => randomColor()) : colors;
             table[0] = table[0].map((n) => n.slice(0, selectedObj.chartLabelMaxLength).chunk(selectedObj.chartLabelMaxWidth).join("<br>"));
             var data = [{
                 x: table[0],
                 y: table[1],
                 type: "bar",
                 name: selectedObj.name,
@@ -11036,20 +11184,28 @@
                                         source: [],
                                         target: [],
                                         value: [],
                                     };
                                     let labels = [];
                                     let colors = [];
                                     let outCSV = [];
-                                    selectedObj.class_names[bn].map((l) => labels.push(`${sankeyTransitionPeriods[0].join("-")} ${l}`));
+                                    selectedObj.class_names[bn].map((l) => {
+                                        let sankeyTransitionPeriod = sankeyTransitionPeriods[0];
+                                        sankeyTransitionPeriod = sankeyTransitionPeriod[0] === sankeyTransitionPeriod[1] ? sankeyTransitionPeriod[0] : sankeyTransitionPeriod.join("-");
+                                        labels.push(`${sankeyTransitionPeriod} ${l}`);
+                                    });
                                     selectedObj.class_palette[bn].map((c) => colors.push(c));
                                     Object.keys(counts).map((transitionPeriod) => {
                                         let offset1 = (transitionPeriodI - 1) * selectedObj.class_names[bn].length;
                                         let offset2 = transitionPeriodI * selectedObj.class_names[bn].length;
-                                        selectedObj.class_names[bn].map((l) => labels.push(`${sankeyTransitionPeriods[transitionPeriodI].join("-")} ${l}`));
+                                        selectedObj.class_names[bn].map((l) => {
+                                            let sankeyTransitionPeriod = sankeyTransitionPeriods[transitionPeriodI];
+                                            sankeyTransitionPeriod = sankeyTransitionPeriod[0] === sankeyTransitionPeriod[1] ? sankeyTransitionPeriod[0] : sankeyTransitionPeriod.join("-");
+                                            labels.push(`${sankeyTransitionPeriod} ${l}`);
+                                        });
                                         selectedObj.class_palette[bn].map((c) => colors.push(c));
                                         let countsTransitionPeriod = counts[transitionPeriod];
                                         let values = Object.values(countsTransitionPeriod);
                                         let pixelTotal = sum(values);
                                         let mult;
                                         if (areaChartFormat === "Percentage") {
                                             mult = (1 / pixelTotal) * 100;
@@ -11067,17 +11223,25 @@
                                             let color_value2 = selectedObj.class_palette[bn][class_valueI2];
                                             sankey_dict.source.push(class_valueI1 + offset1);
                                             sankey_dict.target.push(class_valueI2 + offset2);
                                             sankey_dict.value.push(values[vi]);
                                             countLookup[`${selectedObj.class_names[bn][class_valueI1]}---${selectedObj.class_names[bn][class_valueI2]}`] = values[vi];
                                             vi++;
                                         });
-                                        outCSV.push([""].concat(selectedObj.class_names[bn].map((nm) => `${nm.replace(/[^A-Za-z0-9]/g, "-")} ${transitionPeriod.split("---")[1]} `)));
+                                        outCSV.push([""].concat(selectedObj.class_names[bn].map((nm) => {
+                                            let tp = transitionPeriod.split("---")[1];
+                                            let tps = tp.split("-");
+                                            tp = tps[0] === tps[1] ? tps[0] : tp;
+                                            return `${nm.replace(/[^A-Za-z0-9]/g, "-")} ${tp} `;
+                                        })));
                                         selectedObj.class_names[bn].map((nm1) => {
-                                            let line = [`${nm1.replace(/[^A-Za-z0-9]/g, "-")} ${transitionPeriod.split("---")[0]}`];
+                                            let tp = transitionPeriod.split("---")[0];
+                                            let tps = tp.split("-");
+                                            tp = tps[0] === tps[1] ? tps[0] : tp;
+                                            let line = [`${nm1.replace(/[^A-Za-z0-9]/g, "-")} ${tp}`];
                                             selectedObj.class_names[bn].map((nm2) => {
                                                 let v = countLookup[`${nm1}---${nm2}`];
                                                 v = v !== undefined ? v : 0;
                                                 line.push(v);
                                             });
                                             outCSV.push(line);
                                         });
@@ -11131,14 +11295,16 @@
                                         selectedObj.class_namesT[bn] = class_namesT;
                                     }
                                     let class_paletteT;
                                     if (selectedObj.class_palette !== null) {
                                         class_paletteT = selectedObj.class_palette[bn];
                                     } else if (selectedObj.palette !== undefined && selectedObj.palette !== null) {
                                         class_paletteT = selectedObj.palette;
+                                    } else if (selectedObj.palette_lookup !== undefined && selectedObj.palette_lookup !== null) {
+                                        class_paletteT = class_namesT.map((cn) => selectedObj.palette_lookup[cn]);
                                     } else {
                                         class_paletteT = class_namesT.map((c) => null);
                                     }
                                     if (selectedObj.bandNames.length == 1) {
                                         nameStart = "";
                                     }
                                     class_namesT.map((cn) => {
```

### Comparing `geeViz-2024.3.2/geeViz/geeView/src/js/load.min.js` & `geeViz-2024.4.1/geeViz/geeView/src/js/load.min.js`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/geeView/src/styles/style.min.css` & `geeViz-2024.4.1/geeViz/geeView/src/styles/style.min.css`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/geeView.py` & `geeViz-2024.4.1/geeViz/geeView.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,20 +264,22 @@
         offset = len(gradient_dict["hex"]) - n
         sliceval = []
         # print(('len(gradient_dict)',len(gradient_dict['hex'])))
         # print(('offset',offset))
 
         for i in range(1, offset + 1):
             sliceval.append(int(len(gradient_dict["hex"]) * i / float(offset + 2)))
-        # print(('sliceval',sliceval))
+        print(gradient_dict["hex"])
+        print(("sliceval", sliceval))
         for k in ("hex", "r", "g", "b"):
             gradient_dict[k] = [
                 i for j, i in enumerate(gradient_dict[k]) if j not in sliceval
             ]
         # print(('new len dict', len(gradient_dict['hex'])))
+    print(gradient_dict["hex"], len(gradient_dict["hex"]))
     return gradient_dict
 
 
 def get_poly_gradient_ct(palette, min, max):
     """
     Take a palette and a set of min and max stretch values to get a 1:1 value to color hex list
 
@@ -291,14 +293,17 @@
     Returns:
         list: A list of linearly interpolated hex codes where there is 1:1 color to value from min-max (inclusive)
     """
     ramp = polylinear_gradient(palette, max - min + 1)
     return ramp["hex"]
 
 
+# print(get_poly_gradient_ct(["#FFFF00", "00F", "0FF", "FF0000"], 1, 2))
+
+
 ##############################################################
 ######################################################################
 # Function to check if being run inside a notebook
 # Taken from: https://stackoverflow.com/questions/15411967/how-can-i-check-if-code-is-executed-in-the-ipython-notebook
 def is_notebook():
     return ee.oauth._in_jupyter_shell()
 
@@ -445,16 +450,17 @@
 
                     "bias" (int, list, or comma-separated numbers): One numeric value or one per band to map onto 00-FF.,
 
                     "gamma" (int, list, or comma-separated numbers): Gamma correction factor. One numeric value or one per band.,
 
                     "palette" (str, list, or comma-separated strings): List of CSS-style color strings (single-band previews only).,
 
-                    "opacity" (float): a number between 0 and 1 for initially set opacity.
+                    "opacity" (float): a number between 0 and 1 for initially set opacity.,
 
+                    "layerType" (str, one of geeImage, geeImageCollection, geeVector, geeVectorImage): Optional parameter, but if specified, can speed up the initial page loading of geeView since it won't have to figure out the layer type. For vector data ("featureCollection", "feature", or "geometry"), you can spcify "geeVector" if you would like to force the vector to be an actual vector object on the client. This can be slow if the ee object is large and/or complex. Otherwise, any "featureCollection", "feature", or "geometry" will default to "geeVectorImage" where the vector is rasterized on-the-fly for map rendering. Any querying of the vector will query the underlying vector data though.,
 
                     "reducer" (Reducer, default 'ee.Reducer.lastNonNull()'): If an ImageCollection is provided, how to reduce it to create the layer that is shown on the map. Defaults to ee.Reducer.lastNonNull(),
 
                     "autoViz" (bool): Whether to take image bandName_class_values, bandName_class_names, bandName_class_palette properties to visualize, create a legend (populates `classLegendDict`), and apply class names to any query functions (populates `queryDict`),
 
                     "canQuery" (bool, default True): Whether a layer can be queried when visible.,
 
@@ -592,16 +598,17 @@
 
                     "bias" (int, list, or comma-separated numbers): One numeric value or one per band to map onto 00-FF.,
 
                     "gamma" (int, list, or comma-separated numbers): Gamma correction factor. One numeric value or one per band.,
 
                     "palette" (str, list, or comma-separated strings): List of CSS-style color strings (single-band previews only).,
 
-                    "opacity" (float): a number between 0 and 1 for initially set opacity.
+                    "opacity" (float): a number between 0 and 1 for initially set opacity.,
 
+                    "layerType" (str, one of geeImage, geeImageCollection, geeVector, geeVectorImage): Optional parameter, but if specified, can speed up the initial page loading of geeView since it won't have to figure out the layer type. For vector data ("featureCollection", "feature", or "geometry"), you can spcify "geeVector" if you would like to force the vector to be an actual vector object on the client. This can be slow if the ee object is large and/or complex. Otherwise, any "featureCollection", "feature", or "geometry" will default to "geeVectorImage" where the vector is rasterized on-the-fly for map rendering. Any querying of the vector will query the underlying vector data though.,
 
                     "autoViz" (bool): Whether to take image bandName_class_values, bandName_class_names, bandName_class_palette properties to visualize, create a legend (populates `classLegendDict`), and apply class names to any query functions (populates `queryDict`),
 
                     "canQuery" (bool, default True): Whether a layer can be queried when visible.,
 
                     "addToLegend" (bool, default True): Whether geeViz should try to create a legend for this layer. Sometimes setting it to `False` is useful for continuous multi-band inputs.,
 
@@ -705,28 +712,28 @@
                     "strokeWeight" (int, default 3): The thickness of the polygon outlines,
 
                     "selectLayerNameProperty" (str, default first feature attribute with "name" in it or "system:index"): The attribute name to show when a user selects a feature.
 
 
 
                 }
-            name (str): Descriptive name for map layer that will be shown on the map UI
+            name (str, default None): Descriptive name for map layer that will be shown on the map UI. Will be auto-populated with `Layer N` if not specified
 
         """
         if name == None:
             name = "Layer " + str(self.layerNumber)
             self.layerNumber += 1
         print("Adding layer: " + name)
 
         # Get the id and populate dictionary
         idDict = {}  # image.getMapId()
         idDict["objectName"] = "Map"
         idDict["item"] = featureCollection.serialize()
         idDict["name"] = name
-        idDict["visible"] = str(True).lower()
+        idDict["visible"] = str(False).lower()
         idDict["viz"] = json.dumps(viz, sort_keys=False)
         idDict["function"] = "addSerializedSelectLayer"
         self.idDictList.append(idDict)
 
     ######################################################################
     # Function for setting the map zoom
     def setZoom(self, zoom):
@@ -1110,15 +1117,15 @@
             try:
                 params["reducer"] = params["reducer"].serialize()
             except Exception as e:
                 try:
                     params["reducer"] = eval(params["reducer"]).serialize()
                 except Exception as e:  # Most likely it's already serialized
                     e = e
-
+        params["serialized"] = True
         # Get the id and populate dictionary
         idDict = {}
         if not isinstance(image, dict):
             image = image.serialize()
 
         idDict["item"] = image
         idDict["function"] = "addLayer"
@@ -1129,15 +1136,16 @@
 
         self.idDictList.append(idDict)
 
     def populateAreaChartLayerSelect(self):
         """
         Once you add all area chart layers to the map, you can turn them on using this method- `Map.populateAreaChartLayerSelect`. This will create a selection menu inside the `Area Tools -> Area Tools Parameters` menu. You can then turn layers to include in any area charts on and off from that menu.
         """
-        query_command = "areaChart.populateAreaChartLayerSelect();"
+        query_command = "areaChart.populateChartLayerSelect();"
+
         if query_command not in self.mapCommandList:
             self.mapCommandList.append(query_command)
 
     # Functions to handle setting query output y labels
     def setYLabelMaxLength(self, maxLength):
         command = f"yLabelMaxLength = {maxLength}"
         if command not in self.mapCommandList:
```

### Comparing `geeViz-2024.3.2/geeViz/getImagesLib.py` & `geeViz-2024.4.1/geeViz/getImagesLib.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/migrateGEEAssets.py` & `geeViz-2024.4.1/geeViz/migrateGEEAssets.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/phEEnoViz.py` & `geeViz-2024.4.1/geeViz/phEEnoViz.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz/taskManagerLib.py` & `geeViz-2024.4.1/geeViz/taskManagerLib.py`

 * *Files identical despite different names*

### Comparing `geeViz-2024.3.2/geeViz.egg-info/PKG-INFO` & `geeViz-2024.4.1/geeViz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geeViz
-Version: 2024.3.2
+Version: 2024.4.1
 Summary: A package to help with GEE data processing, analysis, and visualization
 Home-page: https://github.com/gee-community/geeViz
 Author: Ian Housman
 Author-email: ian.housman@gmail.com
 License: Apache
 Keywords: earthengine google remote sensing landsat sentinel modis forestry forest
 Classifier: Programming Language :: Python :: 3
@@ -39,15 +39,15 @@
 
 Ian Housman- ian.housman@usda.gov
 
 Josh Heyer- joshua.heyer@usda.gov
 
 Bonnie Ruefenacht- bonnie.ruefenacht@usda.gov
 
-<iframe src='https://gee-community.github.io/geeViz/build/html/index.html#' width='100%' height='500'  title='geeViz documentation'></iframe>
+## [Documentation (in progress)](https://gee-community.github.io/geeViz/build/html/index.html)
 
 ## Installing
 
 1. Become a trusted Google Earth Engine (GEE) tester (<https://signup.earthengine.google.com/#!/>)
 2. Install package using pip (`pip install geeViz`)
    folder
 3. Authenticate using the GEE cli in a cmd prompt (`earthengine authenticate`)
```

### Comparing `geeViz-2024.3.2/geeViz.egg-info/SOURCES.txt` & `geeViz-2024.4.1/geeViz.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 geeViz/examples/GFSTimeLapse.py
 geeViz/examples/LANDTRENDRViz.py
 geeViz/examples/LANDTRENDRWrapper.py
 geeViz/examples/LANDTRENDRWrapperNotebook.ipynb
 geeViz/examples/LCMAP_and_LCMS_Viewer.py
 geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb
 geeViz/examples/__init__.py
+geeViz/examples/areaChart_examples.ipynb
 geeViz/examples/foliumViewerExample.py
 geeViz/examples/gee2PandasExample.ipynb
 geeViz/examples/geeViewExample.py
 geeViz/examples/geeViewExampleNotebook.ipynb
 geeViz/examples/geeViewVSFoliumViewerExampleNotebook.ipynb
 geeViz/examples/geeViz_and_geemap.py
 geeViz/examples/getClimateWrapper.py
```

### Comparing `geeViz-2024.3.2/setup.py` & `geeViz-2024.4.1/setup.py`

 * *Files identical despite different names*

