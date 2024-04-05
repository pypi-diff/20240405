# Comparing `tmp/cellfinder-1.1.1.tar.gz` & `tmp/cellfinder-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellfinder-1.1.1.tar", last modified: Tue Feb 27 10:31:49 2024, max compression
+gzip compressed data, was "cellfinder-1.1.2.tar", last modified: Fri Apr  5 10:44:13 2024, max compression
```

## Comparing `cellfinder-1.1.1.tar` & `cellfinder-1.1.2.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:49.760670 cellfinder-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:49.744670 cellfinder-1.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:49.748670 cellfinder-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-02-27 10:31:38.000000 cellfinder-1.1.1/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-02-27 10:31:38.000000 cellfinder-1.1.1/.github/workflows/test_include_guard.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-02-27 10:31:38.000000 cellfinder-1.1.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:49.748670 cellfinder-1.1.1/.napari/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-02-27 10:31:38.000000 cellfinder-1.1.1/.napari/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-02-27 10:31:38.000000 cellfinder-1.1.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-02-27 10:31:38.000000 cellfinder-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-27 10:31:38.000000 cellfinder-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6613 2024-02-27 10:31:49.760670 cellfinder-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-02-27 10:31:38.000000 cellfinder-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:49.748670 cellfinder-1.1.1/cellfinder/
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/cli_migration_warning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:49.748670 cellfinder-1.1.1/cellfinder/core/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:49.748670 cellfinder-1.1.1/cellfinder/core/classify/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/classify/augment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/classify/classify.py
--rw-r--r--   0 runner    (1001) docker     (127)    16586 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/classify/cube_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10057 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/classify/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/classify/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:49.748670 cellfinder-1.1.1/cellfinder/core/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/config/cellfinder.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:49.748670 cellfinder-1.1.1/cellfinder/core/detect/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/detect/detect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:49.752670 cellfinder-1.1.1/cellfinder/core/detect/filters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/detect/filters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:49.752670 cellfinder-1.1.1/cellfinder/core/detect/filters/plane/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/detect/filters/plane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/detect/filters/plane/classical_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/detect/filters/plane/plane_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/detect/filters/plane/tile_walker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/detect/filters/setup_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:49.752670 cellfinder-1.1.1/cellfinder/core/detect/filters/volume/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/detect/filters/volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11175 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/detect/filters/volume/ball_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/detect/filters/volume/structure_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/detect/filters/volume/structure_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/detect/filters/volume/volume_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:49.752670 cellfinder-1.1.1/cellfinder/core/download/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/download/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/download/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/download/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:49.756670 cellfinder-1.1.1/cellfinder/core/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/tools/IO.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/tools/array_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/tools/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/tools/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/tools/prep.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/tools/source_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/tools/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/tools/tf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/tools/tiff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/tools/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:49.756670 cellfinder-1.1.1/cellfinder/core/train/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13214 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/train/train_yml.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:49.756670 cellfinder-1.1.1/cellfinder/napari/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/napari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21447 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/napari/curation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:49.756670 cellfinder-1.1.1/cellfinder/napari/detect/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/napari/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7443 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/napari/detect/detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/napari/detect/detect_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/napari/detect/thread_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:49.756670 cellfinder-1.1.1/cellfinder/napari/images/
--rw-r--r--   0 runner    (1001) docker     (127)    21216 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/napari/images/brainglobe.png
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/napari/input_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/napari/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/napari/sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:49.756670 cellfinder-1.1.1/cellfinder/napari/train/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/napari/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/napari/train/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/napari/train/train_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-02-27 10:31:38.000000 cellfinder-1.1.1/cellfinder/napari/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:31:49.756670 cellfinder-1.1.1/cellfinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6613 2024-02-27 10:31:48.000000 cellfinder-1.1.1/cellfinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-02-27 10:31:49.000000 cellfinder-1.1.1/cellfinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 10:31:48.000000 cellfinder-1.1.1/cellfinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-27 10:31:48.000000 cellfinder-1.1.1/cellfinder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-02-27 10:31:48.000000 cellfinder-1.1.1/cellfinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-27 10:31:48.000000 cellfinder-1.1.1/cellfinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-02-27 10:31:38.000000 cellfinder-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 10:31:49.760670 cellfinder-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.167877 cellfinder-1.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.151877 cellfinder-1.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.155876 cellfinder-1.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-05 10:44:05.000000 cellfinder-1.1.2/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-05 10:44:05.000000 cellfinder-1.1.2/.github/workflows/test_include_guard.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-05 10:44:05.000000 cellfinder-1.1.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.155876 cellfinder-1.1.2/.napari/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-05 10:44:05.000000 cellfinder-1.1.2/.napari/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-05 10:44:05.000000 cellfinder-1.1.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-05 10:44:05.000000 cellfinder-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-05 10:44:05.000000 cellfinder-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-04-05 10:44:13.167877 cellfinder-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-05 10:44:05.000000 cellfinder-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.155876 cellfinder-1.1.2/cellfinder/
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/cli_migration_warning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.159876 cellfinder-1.1.2/cellfinder/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.159876 cellfinder-1.1.2/cellfinder/core/classify/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/classify/augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/classify/classify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16586 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/classify/cube_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10057 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/classify/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/classify/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.159876 cellfinder-1.1.2/cellfinder/core/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/config/cellfinder.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.159876 cellfinder-1.1.2/cellfinder/core/detect/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/detect/detect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.159876 cellfinder-1.1.2/cellfinder/core/detect/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/detect/filters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.159876 cellfinder-1.1.2/cellfinder/core/detect/filters/plane/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/detect/filters/plane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/detect/filters/plane/classical_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/detect/filters/plane/plane_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/detect/filters/plane/tile_walker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/detect/filters/setup_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.159876 cellfinder-1.1.2/cellfinder/core/detect/filters/volume/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/detect/filters/volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11175 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/detect/filters/volume/ball_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/detect/filters/volume/structure_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/detect/filters/volume/structure_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/detect/filters/volume/volume_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.159876 cellfinder-1.1.2/cellfinder/core/download/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/download/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/download/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/download/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.163877 cellfinder-1.1.2/cellfinder/core/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/tools/IO.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/tools/array_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/tools/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/tools/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/tools/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/tools/source_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/tools/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/tools/tf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/tools/tiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/tools/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.163877 cellfinder-1.1.2/cellfinder/core/train/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13214 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/train/train_yml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.163877 cellfinder-1.1.2/cellfinder/napari/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21447 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/curation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.163877 cellfinder-1.1.2/cellfinder/napari/detect/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7443 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/detect/detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/detect/detect_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/detect/thread_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.163877 cellfinder-1.1.2/cellfinder/napari/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    21216 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/images/brainglobe.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/input_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.163877 cellfinder-1.1.2/cellfinder/napari/train/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/train/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/train/train_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.167877 cellfinder-1.1.2/cellfinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-04-05 10:44:12.000000 cellfinder-1.1.2/cellfinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-05 10:44:13.000000 cellfinder-1.1.2/cellfinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 10:44:12.000000 cellfinder-1.1.2/cellfinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-05 10:44:12.000000 cellfinder-1.1.2/cellfinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-05 10:44:12.000000 cellfinder-1.1.2/cellfinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 10:44:12.000000 cellfinder-1.1.2/cellfinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-05 10:44:05.000000 cellfinder-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 10:44:13.167877 cellfinder-1.1.2/setup.cfg
```

### Comparing `cellfinder-1.1.1/.github/workflows/test_and_deploy.yml` & `cellfinder-1.1.2/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/.github/workflows/test_include_guard.yaml` & `cellfinder-1.1.2/.github/workflows/test_include_guard.yaml`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/.gitignore` & `cellfinder-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/CITATION.cff` & `cellfinder-1.1.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/LICENSE` & `cellfinder-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/PKG-INFO` & `cellfinder-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellfinder
-Version: 1.1.1
+Version: 1.1.2
 Summary: Automated 3D cell detection in large microscopy images
 Author-email: "Adam Tyson, Christian Niedworok, Charly Rousseau" <code@adamltyson.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://brainglobe.info/documentation/cellfinder/index.html
 Project-URL: Source Code, https://github.com/brainglobe/cellfinder
 Project-URL: Bug Tracker, https://github.com/brainglobe/cellfinder/issues
 Project-URL: Documentation, https://brainglobe.info/documentation/cellfinder/index.html
@@ -18,16 +18,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: brainglobe-utils
-Requires-Dist: brainglobe-napari-io
+Requires-Dist: brainglobe-utils>=0.4.2
+Requires-Dist: brainglobe-napari-io>=0.3.4
 Requires-Dist: dask[array]
 Requires-Dist: fancylog>=0.0.7
 Requires-Dist: natsort
 Requires-Dist: numba
 Requires-Dist: numpy
 Requires-Dist: scikit-image
 Requires-Dist: scikit-learn
```

### Comparing `cellfinder-1.1.1/README.md` & `cellfinder-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/__init__.py` & `cellfinder-1.1.2/cellfinder/__init__.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/cli_migration_warning.py` & `cellfinder-1.1.2/cellfinder/cli_migration_warning.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/core/classify/augment.py` & `cellfinder-1.1.2/cellfinder/core/classify/augment.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/core/classify/classify.py` & `cellfinder-1.1.2/cellfinder/core/classify/classify.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/core/classify/cube_generator.py` & `cellfinder-1.1.2/cellfinder/core/classify/cube_generator.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/core/classify/resnet.py` & `cellfinder-1.1.2/cellfinder/core/classify/resnet.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/core/classify/tools.py` & `cellfinder-1.1.2/cellfinder/core/classify/tools.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/core/detect/detect.py` & `cellfinder-1.1.2/cellfinder/core/detect/detect.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/core/detect/filters/plane/classical_filter.py` & `cellfinder-1.1.2/cellfinder/core/detect/filters/plane/classical_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/core/detect/filters/plane/plane_filter.py` & `cellfinder-1.1.2/cellfinder/core/detect/filters/plane/plane_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/core/detect/filters/plane/tile_walker.py` & `cellfinder-1.1.2/cellfinder/core/detect/filters/plane/tile_walker.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/core/detect/filters/setup_filters.py` & `cellfinder-1.1.2/cellfinder/core/detect/filters/setup_filters.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/core/detect/filters/volume/ball_filter.py` & `cellfinder-1.1.2/cellfinder/core/detect/filters/volume/ball_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/core/detect/filters/volume/structure_detection.py` & `cellfinder-1.1.2/cellfinder/core/detect/filters/volume/structure_detection.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/core/detect/filters/volume/structure_splitting.py` & `cellfinder-1.1.2/cellfinder/core/detect/filters/volume/structure_splitting.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/core/detect/filters/volume/volume_filter.py` & `cellfinder-1.1.2/cellfinder/core/detect/filters/volume/volume_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/core/download/cli.py` & `cellfinder-1.1.2/cellfinder/core/download/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import tempfile
 from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser
 from pathlib import Path
 
 from cellfinder.core.download import models
-from cellfinder.core.download.download import amend_cfg
+from cellfinder.core.download.download import amend_user_configuration
 
 home = Path.home()
 DEFAULT_DOWNLOAD_DIRECTORY = home / ".cellfinder"
 temp_dir = tempfile.TemporaryDirectory()
 temp_dir_path = Path(temp_dir.name)
 
 
@@ -61,12 +61,12 @@
 
 def main():
     args = download_parser().parse_args()
     if not args.no_models:
         model_path = models.main(args.model, args.install_path)
 
     if not args.no_amend_config:
-        amend_cfg(new_model_path=model_path)
+        amend_user_configuration(new_model_path=model_path)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `cellfinder-1.1.1/cellfinder/core/download/download.py` & `cellfinder-1.1.2/cellfinder/core/download/download.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import tarfile
 import urllib.request
 
 from brainglobe_utils.general.config import get_config_obj
 from brainglobe_utils.general.system import disk_free_gb
 
 from cellfinder.core.tools.source_files import (
-    source_config_cellfinder,
-    source_custom_config_cellfinder,
+    default_configuration_path,
+    user_specific_configuration_path,
 )
 
 
 class DownloadError(Exception):
     pass
 
 
@@ -71,24 +71,53 @@
 
     download_file(download_path, url, file_name)
     if install_path is not None:
         extract_file(download_path, install_path)
         os.remove(download_path)
 
 
-def amend_cfg(new_model_path=None):
-    print("Ensuring custom config file is correct")
+def amend_user_configuration(new_model_path=None) -> None:
+    """
+    Amends the user configuration to contain the configuration
+    in new_model_path, if specified.
+
+    Parameters
+    ----------
+    new_model_path : str, optional
+        The path to the new model configuration.
+    """
+    print("(Over-)writing custom user configuration")
 
-    original_config = source_config_cellfinder()
-    new_config = source_custom_config_cellfinder()
+    original_config = default_configuration_path()
+    new_config = user_specific_configuration_path()
     if new_model_path is not None:
-        write_model_to_cfg(new_model_path, original_config, new_config)
+        write_model_to_config(new_model_path, original_config, new_config)
 
 
-def write_model_to_cfg(new_model_path, orig_config, custom_config):
+def write_model_to_config(new_model_path, orig_config, custom_config):
+    """
+    Update the model path in the custom configuration file, by
+    reading the lines in the original configuration file, replacing
+    the line starting with "model_path =" and writing these
+    lines to the custom file.
+
+    Parameters
+    ----------
+    new_model_path : str
+        The new path to the model.
+    orig_config : str
+        The path to the original configuration file.
+    custom_config : str
+        The path to the custom configuration file to be created.
+
+    Returns
+    -------
+    None
+
+    """
     config_obj = get_config_obj(orig_config)
     model_conf = config_obj["model"]
     orig_path = model_conf["model_path"]
 
     with open(orig_config, "r") as in_conf:
         data = in_conf.readlines()
     for i, line in enumerate(data):
```

### Comparing `cellfinder-1.1.1/cellfinder/core/download/models.py` & `cellfinder-1.1.2/cellfinder/core/download/models.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/core/main.py` & `cellfinder-1.1.2/cellfinder/core/main.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/core/tools/IO.py` & `cellfinder-1.1.2/cellfinder/core/tools/IO.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/core/tools/array_operations.py` & `cellfinder-1.1.2/cellfinder/core/tools/array_operations.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/core/tools/geometry.py` & `cellfinder-1.1.2/cellfinder/core/tools/geometry.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/core/tools/image_processing.py` & `cellfinder-1.1.2/cellfinder/core/tools/image_processing.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/core/tools/prep.py` & `cellfinder-1.1.2/cellfinder/core/tools/prep.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 from brainglobe_utils.general.config import get_config_obj
 from brainglobe_utils.general.system import get_num_processes
 
 import cellfinder.core.tools.tf as tf_tools
 from cellfinder.core import logger
 from cellfinder.core.download import models as model_download
-from cellfinder.core.download.download import amend_cfg
-from cellfinder.core.tools.source_files import source_custom_config_cellfinder
+from cellfinder.core.download.download import amend_user_configuration
+from cellfinder.core.tools.source_files import user_specific_configuration_path
 
 home = Path.home()
 DEFAULT_INSTALL_PATH = home / ".cellfinder"
 
 
 def prep_model_weights(
     model_weights: Optional[os.PathLike],
@@ -45,26 +45,26 @@
     model_name: model_download.model_type,
 ) -> Path:
     install_path = install_path or DEFAULT_INSTALL_PATH
     # if no model or weights, set default weights
     if model_weights_path is None:
         logger.debug("No model supplied, so using the default")
 
-        config_file = source_custom_config_cellfinder()
+        config_file = user_specific_configuration_path()
 
         if not Path(config_file).exists():
             logger.debug("Custom config does not exist, downloading models")
             model_path = model_download.main(model_name, install_path)
-            amend_cfg(new_model_path=model_path)
+            amend_user_configuration(new_model_path=model_path)
 
         model_weights = get_model_weights(config_file)
         if not model_weights.exists():
             logger.debug("Model weights do not exist, downloading")
             model_path = model_download.main(model_name, install_path)
-            amend_cfg(new_model_path=model_path)
+            amend_user_configuration(new_model_path=model_path)
             model_weights = get_model_weights(config_file)
     else:
         model_weights = Path(model_weights_path)
     return model_weights
 
 
 def get_model_weights(config_file: os.PathLike) -> Path:
```

### Comparing `cellfinder-1.1.1/cellfinder/core/tools/system.py` & `cellfinder-1.1.2/cellfinder/core/tools/system.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/core/tools/tf.py` & `cellfinder-1.1.2/cellfinder/core/tools/tf.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/core/tools/tiff.py` & `cellfinder-1.1.2/cellfinder/core/tools/tiff.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/core/tools/tools.py` & `cellfinder-1.1.2/cellfinder/core/tools/tools.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/core/train/train_yml.py` & `cellfinder-1.1.2/cellfinder/core/train/train_yml.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/napari/curation.py` & `cellfinder-1.1.2/cellfinder/napari/curation.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/napari/detect/detect.py` & `cellfinder-1.1.2/cellfinder/napari/detect/detect.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/napari/detect/detect_containers.py` & `cellfinder-1.1.2/cellfinder/napari/detect/detect_containers.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/napari/detect/thread_worker.py` & `cellfinder-1.1.2/cellfinder/napari/detect/thread_worker.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/napari/images/brainglobe.png` & `cellfinder-1.1.2/cellfinder/napari/images/brainglobe.png`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/napari/input_container.py` & `cellfinder-1.1.2/cellfinder/napari/input_container.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/napari/napari.yaml` & `cellfinder-1.1.2/cellfinder/napari/napari.yaml`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/napari/sample_data.py` & `cellfinder-1.1.2/cellfinder/napari/sample_data.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/napari/train/train.py` & `cellfinder-1.1.2/cellfinder/napari/train/train.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/napari/train/train_containers.py` & `cellfinder-1.1.2/cellfinder/napari/train/train_containers.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder/napari/utils.py` & `cellfinder-1.1.2/cellfinder/napari/utils.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder.egg-info/PKG-INFO` & `cellfinder-1.1.2/cellfinder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellfinder
-Version: 1.1.1
+Version: 1.1.2
 Summary: Automated 3D cell detection in large microscopy images
 Author-email: "Adam Tyson, Christian Niedworok, Charly Rousseau" <code@adamltyson.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://brainglobe.info/documentation/cellfinder/index.html
 Project-URL: Source Code, https://github.com/brainglobe/cellfinder
 Project-URL: Bug Tracker, https://github.com/brainglobe/cellfinder/issues
 Project-URL: Documentation, https://brainglobe.info/documentation/cellfinder/index.html
@@ -18,16 +18,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: brainglobe-utils
-Requires-Dist: brainglobe-napari-io
+Requires-Dist: brainglobe-utils>=0.4.2
+Requires-Dist: brainglobe-napari-io>=0.3.4
 Requires-Dist: dask[array]
 Requires-Dist: fancylog>=0.0.7
 Requires-Dist: natsort
 Requires-Dist: numba
 Requires-Dist: numpy
 Requires-Dist: scikit-image
 Requires-Dist: scikit-learn
```

### Comparing `cellfinder-1.1.1/cellfinder.egg-info/SOURCES.txt` & `cellfinder-1.1.2/cellfinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.1/cellfinder.egg-info/requires.txt` & `cellfinder-1.1.2/cellfinder.egg-info/requires.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-brainglobe-utils
-brainglobe-napari-io
+brainglobe-utils>=0.4.2
+brainglobe-napari-io>=0.3.4
 dask[array]
 fancylog>=0.0.7
 natsort
 numba
 numpy
 scikit-image
 scikit-learn
```

### Comparing `cellfinder-1.1.1/pyproject.toml` & `cellfinder-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering :: Image Recognition",
 ]
 requires-python = ">=3.9"
 dependencies = [
-    "brainglobe-utils",
-    "brainglobe-napari-io",
+    "brainglobe-utils>=0.4.2",
+    "brainglobe-napari-io>=0.3.4",
     "dask[array]",
     "fancylog>=0.0.7",
     "natsort",
     "numba",
     "numpy",
     "scikit-image",
     "scikit-learn",
```

