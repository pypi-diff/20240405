# Comparing `tmp/vollseg-napari-trackmate-2.5.1.tar.gz` & `tmp/vollseg-napari-trackmate-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vollseg-napari-trackmate-2.5.1.tar", last modified: Mon Feb 26 03:39:44 2024, max compression
+gzip compressed data, was "vollseg-napari-trackmate-2.5.4.tar", last modified: Fri Apr  5 21:40:00 2024, max compression
```

## Comparing `vollseg-napari-trackmate-2.5.1.tar` & `vollseg-napari-trackmate-2.5.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:39:44.447537 vollseg-napari-trackmate-2.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:39:44.439537 vollseg-napari-trackmate-2.5.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:39:44.443537 vollseg-napari-trackmate-2.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-02-26 03:39:26.000000 vollseg-napari-trackmate-2.5.1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-02-26 03:39:26.000000 vollseg-napari-trackmate-2.5.1/.github/workflows/napari-hub-preview.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-02-26 03:39:26.000000 vollseg-napari-trackmate-2.5.1/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-02-26 03:39:26.000000 vollseg-napari-trackmate-2.5.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:39:44.443537 vollseg-napari-trackmate-2.5.1/.napari-hub/
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-02-26 03:39:26.000000 vollseg-napari-trackmate-2.5.1/.napari-hub/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-26 03:39:26.000000 vollseg-napari-trackmate-2.5.1/.napari-hub/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-02-26 03:39:26.000000 vollseg-napari-trackmate-2.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-02-26 03:39:26.000000 vollseg-napari-trackmate-2.5.1/ALGORITHM.md
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-02-26 03:39:26.000000 vollseg-napari-trackmate-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-26 03:39:26.000000 vollseg-napari-trackmate-2.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-02-26 03:39:26.000000 vollseg-napari-trackmate-2.5.1/MITOSIS.md
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-02-26 03:39:44.447537 vollseg-napari-trackmate-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-02-26 03:39:26.000000 vollseg-napari-trackmate-2.5.1/RADIAL_ANGLE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-02-26 03:39:26.000000 vollseg-napari-trackmate-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-02-26 03:39:26.000000 vollseg-napari-trackmate-2.5.1/_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-26 03:39:26.000000 vollseg-napari-trackmate-2.5.1/_toc.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:39:44.443537 vollseg-napari-trackmate-2.5.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-02-26 03:39:26.000000 vollseg-napari-trackmate-2.5.1/examples/annotate_oneat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-02-26 03:39:26.000000 vollseg-napari-trackmate-2.5.1/examples/apply_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-02-26 03:39:26.000000 vollseg-napari-trackmate-2.5.1/examples/create_oneat_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-02-26 03:39:26.000000 vollseg-napari-trackmate-2.5.1/examples/train_oneat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-02-26 03:39:26.000000 vollseg-napari-trackmate-2.5.1/examples/visualize_point_clouds.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-26 03:39:27.000000 vollseg-napari-trackmate-2.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-02-26 03:39:44.447537 vollseg-napari-trackmate-2.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:39:44.439537 vollseg-napari-trackmate-2.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:39:44.443537 vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-02-26 03:39:27.000000 vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-02-26 03:39:27.000000 vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate/_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-26 03:39:27.000000 vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate/_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-02-26 03:39:27.000000 vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate/_temporal_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:39:44.447537 vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate/_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 03:39:27.000000 vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-26 03:39:27.000000 vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate/_tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-26 03:39:27.000000 vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-02-26 03:39:27.000000 vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-26 03:39:27.000000 vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate/_tests/test_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-26 03:39:27.000000 vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    82850 2024-02-26 03:39:27.000000 vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate/_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-02-26 03:39:27.000000 vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate/launch.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-02-26 03:39:27.000000 vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:39:44.447537 vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-02-26 03:39:27.000000 vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate/resources/kapoorlogo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:39:44.447537 vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-02-26 03:39:43.000000 vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-02-26 03:39:44.000000 vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 03:39:43.000000 vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-26 03:39:43.000000 vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-26 03:39:43.000000 vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-26 03:39:43.000000 vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-02-26 03:39:27.000000 vollseg-napari-trackmate-2.5.1/tox.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-02-26 03:39:27.000000 vollseg-napari-trackmate-2.5.1/update_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:40:00.744773 vollseg-napari-trackmate-2.5.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:40:00.736773 vollseg-napari-trackmate-2.5.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:40:00.740773 vollseg-napari-trackmate-2.5.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/.github/workflows/napari-hub-preview.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:40:00.740773 vollseg-napari-trackmate-2.5.4/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/ALGORITHM.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/MITOSIS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-05 21:40:00.744773 vollseg-napari-trackmate-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/RADIAL_ANGLE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/_toc.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:40:00.740773 vollseg-napari-trackmate-2.5.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/examples/annotate_oneat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/examples/apply_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/examples/create_oneat_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/examples/train_oneat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/examples/visualize_point_clouds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-05 21:40:00.748772 vollseg-napari-trackmate-2.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:40:00.736773 vollseg-napari-trackmate-2.5.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:40:00.744773 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_temporal_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:40:00.744773 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_tests/test_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91994 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/launch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:40:00.744773 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/resources/kapoorlogo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:40:00.744773 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-05 21:40:00.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-05 21:40:00.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 21:40:00.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-05 21:40:00.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-05 21:40:00.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 21:40:00.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/update_version.py
```

### Comparing `vollseg-napari-trackmate-2.5.1/.github/workflows/deploy.yml` & `vollseg-napari-trackmate-2.5.4/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.1/.github/workflows/napari-hub-preview.yml` & `vollseg-napari-trackmate-2.5.4/.github/workflows/napari-hub-preview.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.1/.github/workflows/test_and_deploy.yml` & `vollseg-napari-trackmate-2.5.4/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.1/.gitignore` & `vollseg-napari-trackmate-2.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.1/.napari-hub/DESCRIPTION.md` & `vollseg-napari-trackmate-2.5.4/.napari-hub/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.1/.napari-hub/config.yml` & `vollseg-napari-trackmate-2.5.4/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.1/.pre-commit-config.yaml` & `vollseg-napari-trackmate-2.5.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.1/ALGORITHM.md` & `vollseg-napari-trackmate-2.5.4/ALGORITHM.md`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.1/LICENSE` & `vollseg-napari-trackmate-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.1/MITOSIS.md` & `vollseg-napari-trackmate-2.5.4/MITOSIS.md`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.1/PKG-INFO` & `vollseg-napari-trackmate-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-trackmate
-Version: 2.5.1
+Version: 2.5.4
 Summary: Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate#README.md
```

### Comparing `vollseg-napari-trackmate-2.5.1/README.md` & `vollseg-napari-trackmate-2.5.4/README.md`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.1/_config.yml` & `vollseg-napari-trackmate-2.5.4/_config.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.1/examples/apply_autoencoder.py` & `vollseg-napari-trackmate-2.5.4/examples/apply_autoencoder.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.1/examples/create_oneat_patches.py` & `vollseg-napari-trackmate-2.5.4/examples/create_oneat_patches.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.1/examples/train_oneat.py` & `vollseg-napari-trackmate-2.5.4/examples/train_oneat.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.1/examples/visualize_point_clouds.py` & `vollseg-napari-trackmate-2.5.4/examples/visualize_point_clouds.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.1/setup.cfg` & `vollseg-napari-trackmate-2.5.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate/_data_model.py` & `vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_data_model.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate/_temporal_plots.py` & `vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_temporal_plots.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate/_tests/test_widget.py` & `vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate/_widget.py` & `vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_widget.py`

 * *Files 5% similar despite different names*

```diff
@@ -852,15 +852,15 @@
                         )
                         (
                             cluster_time,
                             cluster_z,
                             cluster_y,
                             cluster_x,
                             cluster_radius,
-                            cluster_volume,
+                            cluster_radius_pixel,
                             cluster_eccentricity_comp_first,
                             cluster_eccentricity_comp_second,
                             cluster_eccentricity_comp_third,
                             cluster_surface_area,
                             _,
                         ) = unique_shape_properties_tracklet
 
@@ -868,44 +868,56 @@
                             _trackmate_objects.unique_dynamic_properties[
                                 unique_track_id
                             ][k]
                         )
                         (
                             cluster_time,
                             cluster_speed,
-                            cluster_motion_angle,
+                            cluster_motion_angle_z,
+                            cluster_motion_angle_y,
+                            cluster_motion_angle_x,
                             cluster_acceleration,
                             cluster_distance_cell_mask,
-                            cluster_radial_angle,
-                            cluster_cell_axis_mask,
+                            cluster_radial_angle_z,
+                            cluster_radial_angle_y,
+                            cluster_radial_angle_x,
+                            cluster_cell_axis_z,
+                            cluster_cell_axis_y,
+                            cluster_cell_axis_x,
                             _,
                             _,
                             _,
                             _,
                         ) = unique_dynamic_properties_tracklet
                         unique_dynamic_properties.append(
                             [
                                 cluster_time,
                                 cluster_speed,
-                                cluster_motion_angle,
+                                cluster_motion_angle_z,
+                                cluster_motion_angle_y,
+                                cluster_motion_angle_x,
                                 cluster_acceleration,
                                 cluster_distance_cell_mask,
-                                cluster_radial_angle,
-                                cluster_cell_axis_mask,
+                                cluster_radial_angle_z,
+                                cluster_radial_angle_y,
+                                cluster_radial_angle_x,
+                                cluster_cell_axis_z,
+                                cluster_cell_axis_y,
+                                cluster_cell_axis_x,
                                 countk + 1,
                             ]
                         )
                         unique_shape_properties.append(
                             [
                                 cluster_time,
                                 cluster_z,
                                 cluster_y,
                                 cluster_x,
                                 cluster_radius,
-                                cluster_volume,
+                                cluster_radius_pixel,
                                 cluster_eccentricity_comp_first,
                                 cluster_eccentricity_comp_second,
                                 cluster_eccentricity_comp_third,
                                 cluster_surface_area,
                                 countk + 1,
                             ]
                         )
@@ -919,35 +931,59 @@
                         ):
 
                             current_unique_dynamic_properties = (
                                 unique_dynamic_properties[i]
                             )
                             cluster_time = current_unique_dynamic_properties[0]
                             cluster_speed = current_unique_dynamic_properties[1]
-                            cluster_motion_angle = current_unique_dynamic_properties[2]
-                            cluster_acceleration = current_unique_dynamic_properties[3]
+                            cluster_motion_angle_z = current_unique_dynamic_properties[
+                                2
+                            ]
+                            cluster_motion_angle_y = current_unique_dynamic_properties[
+                                3
+                            ]
+                            cluster_motion_angle_x = current_unique_dynamic_properties[
+                                4
+                            ]
+
+                            cluster_acceleration = current_unique_dynamic_properties[5]
                             cluster_distance_cell_mask = (
-                                current_unique_dynamic_properties[4]
+                                current_unique_dynamic_properties[6]
                             )
-                            cluster_radial_angle = current_unique_dynamic_properties[5]
-                            cluster_cell_axis_mask = current_unique_dynamic_properties[
-                                6
+                            cluster_radial_angle_z = current_unique_dynamic_properties[
+                                7
+                            ]
+                            cluster_radial_angle_y = current_unique_dynamic_properties[
+                                8
+                            ]
+                            cluster_radial_angle_x = current_unique_dynamic_properties[
+                                9
                             ]
 
+                            cluster_cell_axis_z = current_unique_dynamic_properties[10]
+                            cluster_cell_axis_y = current_unique_dynamic_properties[11]
+                            cluster_cell_axis_x = current_unique_dynamic_properties[12]
+
                             cluster_id = current_unique_dynamic_properties[-1]
 
                             data_dynamic_cluster_plot = pd.DataFrame(
                                 {
                                     "Time": cluster_time,
                                     "Speed": cluster_speed,
-                                    "Motion Angle": cluster_motion_angle,
+                                    "Motion_Angle_Z": cluster_motion_angle_z,
+                                    "Motion_Angle_Y": cluster_motion_angle_y,
+                                    "Motion_Angle_X": cluster_motion_angle_x,
                                     "Acceleration": cluster_acceleration,
-                                    "Distance cell to tissue": cluster_distance_cell_mask,
-                                    "Radial Angle": cluster_radial_angle,
-                                    "Cell Axis Mask": cluster_cell_axis_mask,
+                                    "Distance_cell_to_tissue": cluster_distance_cell_mask,
+                                    "Radial_Angle_Z": cluster_radial_angle_z,
+                                    "Radial_Angle_Y": cluster_radial_angle_y,
+                                    "Radial_Angle_X": cluster_radial_angle_x,
+                                    "Cell_Axis_Z": cluster_cell_axis_z,
+                                    "Cell_Axis_Y": cluster_cell_axis_y,
+                                    "Cell_Axis_X": cluster_cell_axis_x,
                                     "id": cluster_id,
                                 }
                             )
 
                             if len(global_data_dynamic_cluster_plot) == 0:
                                 global_data_dynamic_cluster_plot = (
                                     data_dynamic_cluster_plot
@@ -962,15 +998,15 @@
                                 )
 
                         for count, i in enumerate(range(len(unique_shape_properties))):
 
                             current_unique_shape_properties = unique_shape_properties[i]
                             cluster_time = current_unique_shape_properties[0]
                             cluster_radius = current_unique_shape_properties[1]
-                            cluster_volume = current_unique_shape_properties[2]
+                            cluster_radius_pixel = current_unique_shape_properties[2]
                             cluster_eccentricity_comp_first = (
                                 current_unique_shape_properties[3]
                             )
                             cluster_eccentricity_comp_second = (
                                 current_unique_shape_properties[4]
                             )
                             cluster_eccentricity_comp_third = (
@@ -980,15 +1016,15 @@
 
                             cluster_id = current_unique_shape_properties[-1]
 
                             data_cluster_plot = pd.DataFrame(
                                 {
                                     "Time": cluster_time,
                                     "Radius": cluster_radius,
-                                    "Volume": cluster_volume,
+                                    "Radius_Pixel": cluster_radius_pixel,
                                     "Eccentricity_Comp_First": cluster_eccentricity_comp_first,
                                     "Eccentricity_Comp_Second": cluster_eccentricity_comp_second,
                                     "Eccentricity_Comp_Third": cluster_eccentricity_comp_third,
                                     "Surface_Area": cluster_surface_area,
                                     "id": cluster_id,
                                 }
                             )
@@ -1021,36 +1057,96 @@
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
                 sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_dynamic_cluster_plot,
                     x="Time",
-                    y="Motion Angle",
+                    y="Motion_Angle_Z",
+                    hue="id",
+                    ax=plot_ax,
+                    legend=False,
+                )
+
+                plot_ax.set_title("Motion Angle Z")
+                plot_ax.set_xlabel("Time (min)")
+
+                phenotype_plot_class._repeat_after_plot()
+                plot_ax = phenotype_plot_class.plot_ax
+                sns.set_palette(flatui)
+                sns.lineplot(
+                    global_data_dynamic_cluster_plot,
+                    x="Time",
+                    y="Radial_Angle_Z",
+                    hue="id",
+                    ax=plot_ax,
+                    legend=False,
+                )
+
+                plot_ax.set_title("Radial Angle Z")
+                plot_ax.set_xlabel("Time (min)")
+
+                phenotype_plot_class._repeat_after_plot()
+                plot_ax = phenotype_plot_class.plot_ax
+                sns.set_palette(flatui)
+                sns.lineplot(
+                    global_data_dynamic_cluster_plot,
+                    x="Time",
+                    y="Motion_Angle_Y",
+                    hue="id",
+                    ax=plot_ax,
+                    legend=False,
+                )
+
+                plot_ax.set_title("Motion Angle Y")
+                plot_ax.set_xlabel("Time (min)")
+
+                phenotype_plot_class._repeat_after_plot()
+                plot_ax = phenotype_plot_class.plot_ax
+                sns.set_palette(flatui)
+                sns.lineplot(
+                    global_data_dynamic_cluster_plot,
+                    x="Time",
+                    y="Radial_Angle_Y",
                     hue="id",
                     ax=plot_ax,
                     legend=False,
                 )
 
-                plot_ax.set_title("Motion Angle")
+                plot_ax.set_title("Radial Angle Y")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
                 sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_dynamic_cluster_plot,
                     x="Time",
-                    y="Radial Angle",
+                    y="Motion_Angle_X",
                     hue="id",
                     ax=plot_ax,
                     legend=False,
                 )
 
-                plot_ax.set_title("Radial Angle")
+                plot_ax.set_title("Motion Angle X")
+                plot_ax.set_xlabel("Time (min)")
+
+                phenotype_plot_class._repeat_after_plot()
+                plot_ax = phenotype_plot_class.plot_ax
+                sns.set_palette(flatui)
+                sns.lineplot(
+                    global_data_dynamic_cluster_plot,
+                    x="Time",
+                    y="Radial_Angle_X",
+                    hue="id",
+                    ax=plot_ax,
+                    legend=False,
+                )
+
+                plot_ax.set_title("Radial Angle X")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
                 sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_dynamic_cluster_plot,
@@ -1066,36 +1162,66 @@
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
                 sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_dynamic_cluster_plot,
                     x="Time",
-                    y="Distance cell to tissue",
+                    y="Distance_cell_to_tissue",
                     hue="id",
                     ax=plot_ax,
                     legend=False,
                 )
 
                 plot_ax.set_title("Distance cell to tissue")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
                 sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_dynamic_cluster_plot,
                     x="Time",
-                    y="Cell Axis Mask",
+                    y="Cell_Axis_Z",
                     hue="id",
                     ax=plot_ax,
                     legend=False,
                 )
 
-                plot_ax.set_title("Cell Axis Mask")
+                plot_ax.set_title("Cell Axis Z")
+                plot_ax.set_xlabel("Time (min)")
+
+                phenotype_plot_class._repeat_after_plot()
+                plot_ax = phenotype_plot_class.plot_ax
+                sns.set_palette(flatui)
+                sns.lineplot(
+                    global_data_dynamic_cluster_plot,
+                    x="Time",
+                    y="Aell_Axis_Y",
+                    hue="id",
+                    ax=plot_ax,
+                    legend=False,
+                )
+
+                plot_ax.set_title("Cell Axis Y")
+                plot_ax.set_xlabel("Time (min)")
+
+                phenotype_plot_class._repeat_after_plot()
+                plot_ax = phenotype_plot_class.plot_ax
+                sns.set_palette(flatui)
+                sns.lineplot(
+                    global_data_dynamic_cluster_plot,
+                    x="Time",
+                    y="Cell_Axis_X",
+                    hue="id",
+                    ax=plot_ax,
+                    legend=False,
+                )
+
+                plot_ax.set_title("Cell Axis X")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
                 sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_cluster_plot,
@@ -1111,21 +1237,21 @@
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
                 sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_cluster_plot,
                     x="Time",
-                    y="Volume",
+                    y="Radius_pixel",
                     hue="id",
                     ax=plot_ax,
                     legend=False,
                 )
 
-                plot_ax.set_title("Volume")
+                plot_ax.set_title("Radius_pixel")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
                 sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_cluster_plot,
@@ -1407,22 +1533,54 @@
                 plot_ax.set_ylabel("um")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
-                    _trackmate_objects.mitotic_mean_directional_change,
-                    _trackmate_objects.mitotic_var_directional_change,
+                    _trackmate_objects.mitotic_mean_directional_change_z,
+                    _trackmate_objects.mitotic_var_directional_change_z,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
-                plot_ax.set_title("Instantaneous Directional change")
+                plot_ax.set_title("Instantaneous Directional change in Z")
+                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_ylabel("angle (degrees)")
+
+                stat_plot_class._repeat_after_plot()
+                plot_ax = stat_plot_class.plot_ax
+
+                plot_ax.errorbar(
+                    _trackmate_objects.time,
+                    _trackmate_objects.mitotic_mean_directional_change_y,
+                    _trackmate_objects.mitotic_var_directional_change_y,
+                    linestyle="None",
+                    marker=".",
+                    mfc="green",
+                    ecolor="green",
+                )
+                plot_ax.set_title("Instantaneous Directional change in Y")
+                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_ylabel("angle (degrees)")
+
+                stat_plot_class._repeat_after_plot()
+                plot_ax = stat_plot_class.plot_ax
+
+                plot_ax.errorbar(
+                    _trackmate_objects.time,
+                    _trackmate_objects.mitotic_mean_directional_change_x,
+                    _trackmate_objects.mitotic_var_directional_change_x,
+                    linestyle="None",
+                    marker=".",
+                    mfc="green",
+                    ecolor="green",
+                )
+                plot_ax.set_title("Instantaneous Directional change in X")
                 plot_ax.set_xlabel("Time (min)")
                 plot_ax.set_ylabel("angle (degrees)")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
@@ -1541,22 +1699,54 @@
                 plot_ax.set_ylabel("um")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
-                    _trackmate_objects.non_mitotic_mean_directional_change,
-                    _trackmate_objects.non_mitotic_var_directional_change,
+                    _trackmate_objects.non_mitotic_mean_directional_change_z,
+                    _trackmate_objects.non_mitotic_var_directional_change_z,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
-                plot_ax.set_title("Instantaneous Directional change")
+                plot_ax.set_title("Instantaneous Directional change in Z")
+                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_ylabel("angle (degrees)")
+
+                stat_plot_class._repeat_after_plot()
+                plot_ax = stat_plot_class.plot_ax
+
+                plot_ax.errorbar(
+                    _trackmate_objects.time,
+                    _trackmate_objects.non_mitotic_mean_directional_change_y,
+                    _trackmate_objects.non_mitotic_var_directional_change_y,
+                    linestyle="None",
+                    marker=".",
+                    mfc="green",
+                    ecolor="green",
+                )
+                plot_ax.set_title("Instantaneous Directional change in Y")
+                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_ylabel("angle (degrees)")
+
+                stat_plot_class._repeat_after_plot()
+                plot_ax = stat_plot_class.plot_ax
+
+                plot_ax.errorbar(
+                    _trackmate_objects.time,
+                    _trackmate_objects.non_mitotic_mean_directional_change_x,
+                    _trackmate_objects.non_mitotic_var_directional_change_x,
+                    linestyle="None",
+                    marker=".",
+                    mfc="green",
+                    ecolor="green",
+                )
+                plot_ax.set_title("Instantaneous Directional change in X")
                 plot_ax.set_xlabel("Time (min)")
                 plot_ax.set_ylabel("angle (degrees)")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
@@ -1675,22 +1865,54 @@
                 plot_ax.set_ylabel("um")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
-                    _trackmate_objects.all_mean_directional_change,
-                    _trackmate_objects.all_var_directional_change,
+                    _trackmate_objects.all_mean_directional_change_z,
+                    _trackmate_objects.all_var_directional_change_z,
+                    linestyle="None",
+                    marker=".",
+                    mfc="green",
+                    ecolor="green",
+                )
+                plot_ax.set_title("Instantaneous Directional change in Z")
+                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_ylabel("angle (degrees)")
+
+                stat_plot_class._repeat_after_plot()
+                plot_ax = stat_plot_class.plot_ax
+
+                plot_ax.errorbar(
+                    _trackmate_objects.time,
+                    _trackmate_objects.all_mean_directional_change_y,
+                    _trackmate_objects.all_var_directional_change_y,
+                    linestyle="None",
+                    marker=".",
+                    mfc="green",
+                    ecolor="green",
+                )
+                plot_ax.set_title("Instantaneous Directional change in Y")
+                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_ylabel("angle (degrees)")
+
+                stat_plot_class._repeat_after_plot()
+                plot_ax = stat_plot_class.plot_ax
+
+                plot_ax.errorbar(
+                    _trackmate_objects.time,
+                    _trackmate_objects.all_mean_directional_change_x,
+                    _trackmate_objects.all_var_directional_change_x,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
-                plot_ax.set_title("Instantaneous Directional change")
+                plot_ax.set_title("Instantaneous Directional change in X")
                 plot_ax.set_xlabel("Time (min)")
                 plot_ax.set_ylabel("angle (degrees)")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
@@ -2122,15 +2344,15 @@
             num_points=num_points,
             progress_bar=plugin.progress_bar,
             batch_size=plugin_data.batch_size.value,
             accelerator=accelerator,
             devices=1,
             scale_z=scale_z,
             scale_xy=scale_xy,
-            compute_with_autoencoder = False
+            compute_with_autoencoder=False,
         )
         nonlocal track_centroid_tree, track_centroid_list
         track_centroid_list = [
             k for k in _trackmate_objects.unique_track_centroid.keys()
         ]
         track_centroid_tree = spatial.cKDTree(track_centroid_list)
         _refreshStatPlotData()
```

### Comparing `vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate/napari.yaml` & `vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/napari.yaml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate/resources/kapoorlogo.png` & `vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/resources/kapoorlogo.png`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate.egg-info/PKG-INFO` & `vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-trackmate
-Version: 2.5.1
+Version: 2.5.4
 Summary: Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate#README.md
```

### Comparing `vollseg-napari-trackmate-2.5.1/src/vollseg_napari_trackmate.egg-info/SOURCES.txt` & `vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.1/tox.ini` & `vollseg-napari-trackmate-2.5.4/tox.ini`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.1/update_version.py` & `vollseg-napari-trackmate-2.5.4/update_version.py`

 * *Files identical despite different names*

