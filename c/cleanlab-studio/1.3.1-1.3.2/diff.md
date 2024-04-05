# Comparing `tmp/cleanlab-studio-1.3.1.tar.gz` & `tmp/cleanlab-studio-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanlab-studio-1.3.1.tar", last modified: Tue Mar 19 22:19:52 2024, max compression
+gzip compressed data, was "cleanlab-studio-1.3.2.tar", last modified: Fri Apr  5 17:09:34 2024, max compression
```

## Comparing `cleanlab-studio-1.3.1.tar` & `cleanlab-studio-1.3.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:19:52.160060 cleanlab-studio-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-03-19 22:19:52.160060 cleanlab-studio-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:19:52.152059 cleanlab-studio-1.3.1/cleanlab_studio/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:19:52.152059 cleanlab-studio-1.3.1/cleanlab_studio/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/cli/api_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:19:52.156059 cleanlab-studio-1.3.1/cleanlab_studio/cli/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/cli/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/cli/classes/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/cli/classes/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/cli/classes/excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/cli/classes/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:19:52.156059 cleanlab-studio-1.3.1/cleanlab_studio/cli/cleanset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/cli/cleanset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/cli/cleanset/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/cli/cleanset/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/cli/cleanset/download_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/cli/click_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:19:52.156059 cleanlab-studio-1.3.1/cleanlab_studio/cli/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/cli/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/cli/dataset/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/cli/dataset/schema_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/cli/dataset/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:19:52.156059 cleanlab-studio-1.3.1/cleanlab_studio/cli/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/cli/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/cli/decorators/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/cli/decorators/previous_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:19:52.156059 cleanlab-studio-1.3.1/cleanlab_studio/cli/login/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/cli/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/cli/login/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:19:52.156059 cleanlab-studio-1.3.1/cleanlab_studio/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:19:52.160060 cleanlab-studio-1.3.1/cleanlab_studio/internal/api/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/internal/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21042 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/internal/api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/internal/api/api_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/internal/clean_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/internal/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:19:52.160060 cleanlab-studio-1.3.1/cleanlab_studio/internal/dataset_source/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/internal/dataset_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/internal/dataset_source/dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/internal/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/internal/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/internal/upload_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11520 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/internal/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:19:52.160060 cleanlab-studio-1.3.1/cleanlab_studio/studio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/studio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/studio/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)    21808 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/studio/studio.py
--rw-r--r--   0 runner    (1001) docker     (127)    17685 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/studio/trustworthy_language_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:19:52.160060 cleanlab-studio-1.3.1/cleanlab_studio/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/utils/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/cleanlab_studio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:19:52.160060 cleanlab-studio-1.3.1/cleanlab_studio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-03-19 22:19:52.000000 cleanlab-studio-1.3.1/cleanlab_studio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-03-19 22:19:52.000000 cleanlab-studio-1.3.1/cleanlab_studio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 22:19:52.000000 cleanlab-studio-1.3.1/cleanlab_studio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-19 22:19:52.000000 cleanlab-studio-1.3.1/cleanlab_studio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-19 22:19:52.000000 cleanlab-studio-1.3.1/cleanlab_studio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-19 22:19:52.000000 cleanlab-studio-1.3.1/cleanlab_studio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 22:19:52.160060 cleanlab-studio-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-03-19 22:19:42.000000 cleanlab-studio-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.136367 cleanlab-studio-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-04-05 17:09:34.136367 cleanlab-studio-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.128367 cleanlab-studio-1.3.2/cleanlab_studio/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.128367 cleanlab-studio-1.3.2/cleanlab_studio/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/api_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.128367 cleanlab-studio-1.3.2/cleanlab_studio/cli/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/classes/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/classes/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/classes/excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/classes/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.128367 cleanlab-studio-1.3.2/cleanlab_studio/cli/cleanset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/cleanset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/cleanset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/cleanset/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/cleanset/download_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/click_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.132367 cleanlab-studio-1.3.2/cleanlab_studio/cli/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/dataset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/dataset/schema_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/dataset/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.132367 cleanlab-studio-1.3.2/cleanlab_studio/cli/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/decorators/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/decorators/previous_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.132367 cleanlab-studio-1.3.2/cleanlab_studio/cli/login/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/login/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.132367 cleanlab-studio-1.3.2/cleanlab_studio/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.132367 cleanlab-studio-1.3.2/cleanlab_studio/internal/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22356 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/api/api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/clean_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.132367 cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.136367 cleanlab-studio-1.3.2/cleanlab_studio/studio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/studio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/studio/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22008 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/studio/studio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17685 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/studio/trustworthy_language_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.136367 cleanlab-studio-1.3.2/cleanlab_studio/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/utils/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.136367 cleanlab-studio-1.3.2/cleanlab_studio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-04-05 17:09:34.000000 cleanlab-studio-1.3.2/cleanlab_studio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-05 17:09:34.000000 cleanlab-studio-1.3.2/cleanlab_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:09:34.000000 cleanlab-studio-1.3.2/cleanlab_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-05 17:09:34.000000 cleanlab-studio-1.3.2/cleanlab_studio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-05 17:09:34.000000 cleanlab-studio-1.3.2/cleanlab_studio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 17:09:34.000000 cleanlab-studio-1.3.2/cleanlab_studio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 17:09:34.136367 cleanlab-studio-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/setup.py
```

### Comparing `cleanlab-studio-1.3.1/LICENSE` & `cleanlab-studio-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/PKG-INFO` & `cleanlab-studio-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 1.3.1
+Version: 1.3.2
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Project-URL: Documentation, https://help.cleanlab.ai
```

### Comparing `cleanlab-studio-1.3.1/README.md` & `cleanlab-studio-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/cli/api_service.py` & `cleanlab-studio-1.3.2/cleanlab_studio/cli/api_service.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/cli/classes/csv_dataset.py` & `cleanlab-studio-1.3.2/cleanlab_studio/cli/classes/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/cli/classes/dataset.py` & `cleanlab-studio-1.3.2/cleanlab_studio/cli/classes/dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/cli/classes/excel_dataset.py` & `cleanlab-studio-1.3.2/cleanlab_studio/cli/classes/excel_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/cli/classes/json_dataset.py` & `cleanlab-studio-1.3.2/cleanlab_studio/cli/classes/json_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/cli/cleanset/download.py` & `cleanlab-studio-1.3.2/cleanlab_studio/cli/cleanset/download.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/cli/cleanset/download_helpers.py` & `cleanlab-studio-1.3.2/cleanlab_studio/cli/cleanset/download_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/cli/click_helpers.py` & `cleanlab-studio-1.3.2/cleanlab_studio/cli/click_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/cli/dataset/schema_helpers.py` & `cleanlab-studio-1.3.2/cleanlab_studio/cli/dataset/schema_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/cli/dataset/upload.py` & `cleanlab-studio-1.3.2/cleanlab_studio/cli/dataset/upload.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/cli/decorators/auth_config.py` & `cleanlab-studio-1.3.2/cleanlab_studio/cli/decorators/auth_config.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/cli/decorators/previous_state.py` & `cleanlab-studio-1.3.2/cleanlab_studio/cli/decorators/previous_state.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/cli/login/login.py` & `cleanlab-studio-1.3.2/cleanlab_studio/cli/login/login.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/cli/main.py` & `cleanlab-studio-1.3.2/cleanlab_studio/cli/main.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/cli/types.py` & `cleanlab-studio-1.3.2/cleanlab_studio/cli/types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/cli/util.py` & `cleanlab-studio-1.3.2/cleanlab_studio/cli/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/internal/api/api.py` & `cleanlab-studio-1.3.2/cleanlab_studio/internal/api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 import asyncio
 import io
 from math import e
 import os
 import time
 from typing import Callable, cast, List, Optional, Tuple, Dict, Union, Any
-from cleanlab_studio.errors import APIError, IngestionError, RateLimitError, TlmBadRequest
+from cleanlab_studio.errors import (
+    APIError,
+    IngestionError,
+    InvalidProjectConfiguration,
+    RateLimitError,
+    TlmBadRequest,
+)
+from cleanlab_studio.internal.util import get_basic_info, obfuscate_stack_trace
 
 import aiohttp
 import requests
 from tqdm import tqdm
 import pandas as pd
 import numpy as np
 import numpy.typing as npt
@@ -52,24 +59,28 @@
     if content_type:
         retval["Content-Type"] = content_type
     retval["Client-Type"] = "python-api"
     return retval
 
 
 def handle_api_error(res: requests.Response) -> None:
-    handle_api_error_from_json(res.json())
+    handle_api_error_from_json(res.json(), res.status_code)
 
 
-def handle_api_error_from_json(res_json: JSONDict) -> None:
+def handle_api_error_from_json(res_json: JSONDict, status_code: Optional[int] = None) -> None:
     if "code" in res_json and "description" in res_json:  # AuthError or UserQuotaError format
         if res_json["code"] == "user_soft_quota_exceeded":
             pass  # soft quota limit is going away soon, so ignore it
         else:
             raise APIError(res_json["description"])
+
     if res_json.get("error", None) is not None:
+        error = res_json["error"]
+        if status_code == 422 and error.get("code", None) == "UNSUPPORTED_PROJECT_CONFIGURATION":
+            raise InvalidProjectConfiguration(error["description"])
         raise APIError(res_json["error"])
 
 
 def handle_rate_limit_error_from_resp(resp: aiohttp.ClientResponse) -> None:
     """Catches 429 (rate limit) errors."""
     if resp.status == 429:
         raise RateLimitError(
@@ -319,14 +330,36 @@
         headers=_construct_headers(api_key),
     )
     handle_api_error(res)
     dataset_details: JSONDict = res.json()
     return dataset_details
 
 
+def check_column_diversity(api_key: str, dataset_id: str, column_name: str) -> JSONDict:
+    check_uuid_well_formed(dataset_id, "dataset ID")
+    res = requests.get(
+        dataset_base_url + f"/diversity/{dataset_id}/{column_name}",
+        headers=_construct_headers(api_key),
+    )
+    handle_api_error(res)
+    column_diversity: JSONDict = res.json()
+    return column_diversity
+
+
+def is_valid_multilabel_column(api_key: str, dataset_id: str, column_name: str) -> bool:
+    check_uuid_well_formed(dataset_id, "dataset ID")
+    res = requests.get(
+        dataset_base_url + f"/check_valid_multilabel/{dataset_id}/{column_name}",
+        headers=_construct_headers(api_key),
+    )
+    handle_api_error(res)
+    multilabel_column: JSONDict = res.json()
+    return bool(multilabel_column["is_valid_multilabel_column"])
+
+
 def clean_dataset(
     api_key: str,
     dataset_id: str,
     project_name: str,
     task_type: Optional[str],
     modality: str,
     model_type: str,
@@ -630,7 +663,11 @@
         handle_api_error_from_json(res_json)
 
     finally:
         if local_scoped_client:
             await client_session.close()
 
     return cast(JSONDict, res_json)
+
+
+def send_telemetry(info: JSONDict) -> None:
+    requests.post(f"{cli_base_url}/telemetry", json=info)
```

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/internal/dataset_source/__init__.py` & `cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/__init__.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py` & `cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/internal/dataset_source/dataset_source.py` & `cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py` & `cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py` & `cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py` & `cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/internal/settings.py` & `cleanlab-studio-1.3.2/cleanlab_studio/internal/settings.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/internal/upload_helpers.py` & `cleanlab-studio-1.3.2/cleanlab_studio/internal/upload_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/internal/util.py` & `cleanlab-studio-1.3.2/cleanlab_studio/internal/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import requests
 import re
 
 
 import numpy as np
 import pandas as pd
 
-from cleanlab_studio.internal.api.api import cli_base_url
+from cleanlab_studio.internal.api import api
 from cleanlab_studio.internal.settings import CleanlabSettings
 from cleanlab_studio.errors import InvalidDatasetError, HandledError
 
 try:
     import snowflake.snowpark as snowpark
 
     snowpark_exists = True
@@ -251,44 +251,51 @@
                     # first arg is self, get _api_key from self
                     user_info["api_key"] = api_key if load_api_key else args[0]._api_key
                     trace_str = traceback.format_exc()
                     # only send stack trace for cleanlab functions
                     if track_all_frames:
                         cleanlab_traceback = trace_str
                     else:
-                        # remove stack frames for user code
-                        cleanlab_match = re.search("File.*cleanlab", trace_str)
-                        cleanlab_traceback = (
-                            trace_str[cleanlab_match.start() :] if cleanlab_match else ""
-                        )
-
-                        # clean up paths that don't contain "cleanlab-studio" which may contain local paths
-                        pattern1 = re.compile(r"File \"((?!cleanlab-studio).)*\n")
-                        cleanlab_traceback = pattern1.sub("File \n", cleanlab_traceback)
-
-                        # remove portios of paths preceding cleanlab-studio that may contain local paths
-                        pattern2 = re.compile(r"File([^\n]*?)cleanlab-studio")
-                        cleanlab_traceback = pattern2.sub(
-                            'File "cleanlab-studio', cleanlab_traceback
-                        )
+                        # remove user code/local paths from trace
+                        cleanlab_traceback = obfuscate_stack_trace(trace_str)
 
                     user_info["stack_trace"] = cleanlab_traceback
                     user_info["error_type"] = type(err).__name__
                     user_info["is_handled_error"] = isinstance(err, HandledError)
-                    _ = requests.post(
-                        f"{cli_base_url}/telemetry",
-                        json=user_info,
-                    )
+                    api.send_telemetry(user_info)
                 raise err
 
         return tracked_func
 
     return track
 
 
+def log_internal_error(error_message: str, stack_trace: str, api_key: Optional[str] = None) -> None:
+    user_info = get_basic_info()
+    user_info["api_key"] = api_key
+    user_info["error_message"] = error_message
+    user_info["stack_trace"] = obfuscate_stack_trace(stack_trace)
+    api.send_telemetry(user_info)
+
+
+def obfuscate_stack_trace(stack_trace: str) -> str:
+    # remove stack frames for user code
+    cleanlab_match = re.search("File.*cleanlab", stack_trace)
+    cleanlab_traceback = stack_trace[cleanlab_match.start() :] if cleanlab_match else ""
+
+    # clean up paths that don't contain "cleanlab-studio" which may contain local paths
+    pattern1 = re.compile(r"File \"((?!cleanlab-studio).)*\n")
+    cleanlab_traceback = pattern1.sub("File \n", cleanlab_traceback)
+
+    # remove portions of paths preceding cleanlab-studio that may contain local paths
+    pattern2 = re.compile(r"File([^\n]*?)cleanlab-studio")
+    cleanlab_traceback = pattern2.sub('File "cleanlab-studio', cleanlab_traceback)
+    return cleanlab_traceback
+
+
 def get_basic_info() -> Dict[str, Any]:
     user_info: Dict[str, Any] = {}
     # get OS
     user_info["os"] = platform.system()
     user_info["os_release"] = platform.release()
     # get python version
     user_info["python_version"] = sys.version
```

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/studio/inference.py` & `cleanlab-studio-1.3.2/cleanlab_studio/studio/inference.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 """
-Methods for interfacing with deployed ML models (to produce predictions)
+Methods for interfacing with deployed ML models (to produce predictions).
+
+**This module is not meant to be imported and used directly.** Instead, use [`Studio.get_model()`](../studio/#method-get_model) to instantiate a [Model](#class-model) object.
+
+The [Model Deployment tutorial](/tutorials/inference_api/) explains the end-to-end workflow for using Cleanlab Studio's model deployment functionality.
 """
 
 import abc
 import csv
 import io
 import time
 from typing import List, Optional, Tuple, Union, Any
@@ -22,18 +26,23 @@
 Batch = Union[TextBatch, TabularBatch]
 
 Predictions = Union[npt.NDArray[np.int_], npt.NDArray[np.str_], npt.NDArray[Any]]
 ClassProbablities: TypeAlias = pd.DataFrame
 
 
 class Model(abc.ABC):
-    """Base class for deployed model inference."""
+    """Represents a machine learning model instance in a Cleanlab Studio account.
+
+    Models should be instantiated using the [`Studio.get_model()`](../studio/#method-get_model) method. Then, using a Model object, you can [`predict()`](#method-predict) labels for new data.
+    """
 
     def __init__(self, api_key: str, model_id: str):
-        """Initializes model class w/ API key and model ID."""
+        """Initializes a model.
+
+        **Objects of this class are not meant to be constructed directly.** Instead, use [`Studio.get_model()`](../studio/#method-get_model)."""
         self._api_key = api_key
         self._model_id = model_id
 
         model_info = api.get_deployed_model_info(self._api_key, self._model_id)
         self._tasktype = model_info["tasktype"]
 
     def predict(
@@ -111,15 +120,15 @@
             resp = api.get_prediction_status(self._api_key, query_id)
 
             if result_url := resp.get("results"):
                 results: pd.DataFrame = pd.read_csv(result_url)
                 if self._tasktype == "multi-label":
                     # convert multi-label suggested labels to list of list of strings
                     suggested_labels = (
-                        results.pop("Suggested Label").apply(csv_string_to_list).to_numpy()
+                        results.pop("Suggested Label").apply(_csv_string_to_list).to_numpy()
                     )
                 else:
                     suggested_labels = results.pop("Suggested Label").to_numpy()
 
                 return suggested_labels, results
 
             time.sleep(1)
@@ -150,15 +159,15 @@
         else:
             raise TypeError(f"Invalid type of batch: {type(batch)}")
 
         sio.seek(0)
         return sio
 
 
-def csv_string_to_list(csv_string: Optional[str]) -> List[str]:
+def _csv_string_to_list(csv_string: Optional[str]) -> List[str]:
     """Convert a csv string with one row that represents a list into a list
 
     Return empty list if string is empty
     """
     if pd.isna(csv_string):
         return []
     input_stream = io.StringIO(csv_string)
```

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/studio/studio.py` & `cleanlab-studio-1.3.2/cleanlab_studio/studio/studio.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,21 @@
     import pyspark.sql
 
 
 class Studio:
     _api_key: str
 
     def __init__(self, api_key: Optional[str]):
+        """
+        Creates a Cleanlab Studio client.
+
+        Args:
+            api_key: You can find your API key on your [account page](https://app.cleanlab.ai/account) in Cleanlab Studio. Instead of specifying the API key here, you can also log in with `cleanlab login` on the command-line.
+
+        """
         if not api.is_valid_client_version():
             raise VersionError(
                 "CLI is out of date and must be updated. Run 'pip install --upgrade cleanlab-studio'."
             )
         if api_key is None:
             try:
                 api_key = CleanlabSettings.load().api_key
@@ -208,43 +215,35 @@
             text_column: Name of column containing the text to train text modality project on (if not supplied and modality is "text" we'll make our best guess).
 
         Returns:
             ID of created project.
         """
         dataset_details = api.get_dataset_details(self._api_key, dataset_id, task_type)
 
-        if label_column is not None:
-            if label_column not in dataset_details["label_columns"]:
-                raise InvalidDatasetError(
-                    f"Invalid label column: {label_column}. Label column must have categorical feature type"
-                )
-        elif task_type is not None and task_type != "unsupervised":
+        if label_column is None and task_type is not None and task_type != "unsupervised":
             label_column = str(dataset_details["label_column_guess"])
             print(f"Label column not supplied. Using best guess {label_column}")
 
         if feature_columns is not None and modality != "tabular":
             if label_column in feature_columns:
                 raise InvalidDatasetError("Label column cannot be included in feature columns")
             raise InvalidDatasetError(
                 "Feature columns supplied, but project modality is not tabular"
             )
         if feature_columns is None:
             if modality == "tabular":
                 feature_columns = dataset_details["distinct_columns"]
-                if label_column is not None:
+                if label_column is not None and label_column in feature_columns:
                     feature_columns.remove(label_column)
                 print(f"Feature columns not supplied. Using all valid feature columns")
 
         if text_column is not None:
             if modality != "text":
                 raise InvalidDatasetError("Text column supplied, but project modality is not text")
-            elif text_column not in dataset_details["text_columns"]:
-                raise InvalidDatasetError(
-                    f"Invalid text column: {text_column}. Column must have text feature type"
-                )
+
         if text_column is None and modality == "text":
             text_column = dataset_details["text_column_guess"]
             print(f"Text column not supplied. Using best guess {text_column}")
 
         return api.clean_dataset(
             api_key=self._api_key,
             dataset_id=dataset_id,
@@ -309,21 +308,23 @@
             project_id: ID of project to delete.
         """
         api.delete_project(self._api_key, project_id)
         print(f"Successfully deleted project: {project_id}")
 
     def get_model(self, model_id: str) -> inference.Model:
         """
-        Gets a model deployed by Cleanlab Studio.
+        Gets a model that is deployed in a Cleanlab Studio account.
+
+        The returned model can then be used to predict labels for new data. See the documentation for the [Model](../inference#class-model) class for more on what you can do with a Model object.
 
         Args:
-            model_id: ID of model to get. This ID should be fetched in the deployments page of the app UI.
+            model_id: ID of model to get. The model ID can be found in the "Model Details" tab of a model page.
 
         Returns:
-            [Model](../inference#class-model) object with methods to run predictions on new input data.
+            [Model](../inference#class-model) instance, which exposes methods to predict labels for new data.
         """
         return inference.Model(self._api_key, model_id)
 
     def download_pred_probs(
         self,
         cleanset_id: str,
         keep_id: bool = False,
@@ -427,10 +428,13 @@
             return True
 
         except (TimeoutError, CleansetError):
             return False
 
 
 # decorate all functions of self
-for name, method in Studio.__dict__.items():
-    if isinstance(method, FunctionType):
-        setattr(Studio, name, (telemetry(track_all_frames=False))(method))
+#
+# using variable names prepended with "_" to not create global variables that
+# show up in the docs
+for _name, _method in Studio.__dict__.items():
+    if isinstance(_method, FunctionType):
+        setattr(Studio, _name, (telemetry(track_all_frames=False))(_method))
```

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/studio/trustworthy_language_model.py` & `cleanlab-studio-1.3.2/cleanlab_studio/studio/trustworthy_language_model.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio/utils/synthetic.py` & `cleanlab-studio-1.3.2/cleanlab_studio/utils/synthetic.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio.egg-info/PKG-INFO` & `cleanlab-studio-1.3.2/cleanlab_studio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 1.3.1
+Version: 1.3.2
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Project-URL: Documentation, https://help.cleanlab.ai
```

### Comparing `cleanlab-studio-1.3.1/cleanlab_studio.egg-info/SOURCES.txt` & `cleanlab-studio-1.3.2/cleanlab_studio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.1/setup.py` & `cleanlab-studio-1.3.2/setup.py`

 * *Files identical despite different names*

