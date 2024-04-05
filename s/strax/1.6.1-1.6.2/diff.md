# Comparing `tmp/strax-1.6.1.tar.gz` & `tmp/strax-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strax-1.6.1.tar", last modified: Wed Feb 21 13:19:29 2024, max compression
+gzip compressed data, was "strax-1.6.2.tar", last modified: Fri Apr  5 01:14:17 2024, max compression
```

## Comparing `strax-1.6.1.tar` & `strax-1.6.2.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:19:29.958481 strax-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-02-21 13:19:27.000000 strax-1.6.1/CODE-OF-CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-02-21 13:19:27.000000 strax-1.6.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    24098 2024-02-21 13:19:27.000000 strax-1.6.1/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-02-21 13:19:27.000000 strax-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-21 13:19:27.000000 strax-1.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    26901 2024-02-21 13:19:29.958481 strax-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-02-21 13:19:27.000000 strax-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:19:29.946481 strax-1.6.1/bin/
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-02-21 13:19:27.000000 strax-1.6.1/bin/rechunker
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:19:29.946481 strax-1.6.1/extra_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-21 13:19:27.000000 strax-1.6.1/extra_requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-21 13:19:27.000000 strax-1.6.1/extra_requirements/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-02-21 13:19:27.000000 strax-1.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-02-21 13:19:29.958481 strax-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-02-21 13:19:27.000000 strax-1.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:19:29.950481 strax-1.6.1/strax/
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-02-21 13:19:27.000000 strax-1.6.1/strax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-21 13:19:27.000000 strax-1.6.1/strax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13508 2024-02-21 13:19:27.000000 strax-1.6.1/strax/chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)    10976 2024-02-21 13:19:27.000000 strax-1.6.1/strax/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    97822 2024-02-21 13:19:27.000000 strax-1.6.1/strax/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    12954 2024-02-21 13:19:27.000000 strax-1.6.1/strax/corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-02-21 13:19:27.000000 strax-1.6.1/strax/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-02-21 13:19:27.000000 strax-1.6.1/strax/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    19813 2024-02-21 13:19:27.000000 strax-1.6.1/strax/mailbox.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-21 13:19:27.000000 strax-1.6.1/strax/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:19:29.950481 strax-1.6.1/strax/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-21 13:19:27.000000 strax-1.6.1/strax/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-02-21 13:19:27.000000 strax-1.6.1/strax/plugins/cut_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-02-21 13:19:27.000000 strax-1.6.1/strax/plugins/down_chunking_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-02-21 13:19:27.000000 strax-1.6.1/strax/plugins/loop_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-02-21 13:19:27.000000 strax-1.6.1/strax/plugins/merge_only_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-02-21 13:19:27.000000 strax-1.6.1/strax/plugins/overlap_window_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-02-21 13:19:27.000000 strax-1.6.1/strax/plugins/parrallel_source_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    27126 2024-02-21 13:19:27.000000 strax-1.6.1/strax/plugins/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:19:29.954481 strax-1.6.1/strax/processing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 13:19:27.000000 strax-1.6.1/strax/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-02-21 13:19:27.000000 strax-1.6.1/strax/processing/data_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)    18567 2024-02-21 13:19:27.000000 strax-1.6.1/strax/processing/general.py
--rw-r--r--   0 runner    (1001) docker     (127)    22690 2024-02-21 13:19:27.000000 strax-1.6.1/strax/processing/hitlets.py
--rw-r--r--   0 runner    (1001) docker     (127)    18761 2024-02-21 13:19:27.000000 strax-1.6.1/strax/processing/peak_building.py
--rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-02-21 13:19:27.000000 strax-1.6.1/strax/processing/peak_merging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-02-21 13:19:27.000000 strax-1.6.1/strax/processing/peak_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    13738 2024-02-21 13:19:27.000000 strax-1.6.1/strax/processing/peak_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-02-21 13:19:27.000000 strax-1.6.1/strax/processing/pulse_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-02-21 13:19:27.000000 strax-1.6.1/strax/processing/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12799 2024-02-21 13:19:27.000000 strax-1.6.1/strax/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    20209 2024-02-21 13:19:27.000000 strax-1.6.1/strax/run_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:19:29.954481 strax-1.6.1/strax/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 13:19:27.000000 strax-1.6.1/strax/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27409 2024-02-21 13:19:27.000000 strax-1.6.1/strax/storage/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-02-21 13:19:27.000000 strax-1.6.1/strax/storage/file_rechunker.py
--rw-r--r--   0 runner    (1001) docker     (127)    14348 2024-02-21 13:19:27.000000 strax-1.6.1/strax/storage/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    13716 2024-02-21 13:19:27.000000 strax-1.6.1/strax/storage/mongo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-02-21 13:19:27.000000 strax-1.6.1/strax/storage/zipfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    13619 2024-02-21 13:19:27.000000 strax-1.6.1/strax/testutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    27108 2024-02-21 13:19:27.000000 strax-1.6.1/strax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:19:29.950481 strax-1.6.1/strax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    26901 2024-02-21 13:19:29.000000 strax-1.6.1/strax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-02-21 13:19:29.000000 strax-1.6.1/strax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 13:19:29.000000 strax-1.6.1/strax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 13:19:29.000000 strax-1.6.1/strax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-21 13:19:29.000000 strax-1.6.1/strax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-21 13:19:29.000000 strax-1.6.1/strax.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:19:29.958481 strax-1.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 13:19:27.000000 strax-1.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10983 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_child_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    18019 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    16134 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_cut_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_data_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_down_chunk_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_fixed_plugin_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    15800 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_general_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_get_zarr.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20402 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_hitlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_inline_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_lone_hit_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_loop_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_mailbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    11124 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_mongo_frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_multi_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_overlap_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_peak_merging.py
--rw-r--r--   0 runner    (1001) docker     (127)    10617 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_peak_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_peak_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_peak_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_pulse_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_saving.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12270 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    15816 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_superruns.py
--rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-02-21 13:19:27.000000 strax-1.6.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:14:17.137385 strax-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-05 01:14:12.000000 strax-1.6.2/CODE-OF-CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-05 01:14:12.000000 strax-1.6.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    25061 2024-04-05 01:14:12.000000 strax-1.6.2/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-05 01:14:12.000000 strax-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-05 01:14:12.000000 strax-1.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    27864 2024-04-05 01:14:17.137385 strax-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-05 01:14:12.000000 strax-1.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:14:17.129385 strax-1.6.2/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-05 01:14:12.000000 strax-1.6.2/bin/rechunker
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:14:17.129385 strax-1.6.2/extra_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-05 01:14:12.000000 strax-1.6.2/extra_requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-05 01:14:12.000000 strax-1.6.2/extra_requirements/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-05 01:14:12.000000 strax-1.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-05 01:14:17.137385 strax-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-05 01:14:12.000000 strax-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:14:17.129385 strax-1.6.2/strax/
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-05 01:14:12.000000 strax-1.6.2/strax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-05 01:14:12.000000 strax-1.6.2/strax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13508 2024-04-05 01:14:12.000000 strax-1.6.2/strax/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10976 2024-04-05 01:14:12.000000 strax-1.6.2/strax/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99037 2024-04-05 01:14:12.000000 strax-1.6.2/strax/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12954 2024-04-05 01:14:12.000000 strax-1.6.2/strax/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-04-05 01:14:12.000000 strax-1.6.2/strax/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-05 01:14:12.000000 strax-1.6.2/strax/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19813 2024-04-05 01:14:12.000000 strax-1.6.2/strax/mailbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-05 01:14:12.000000 strax-1.6.2/strax/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:14:17.133385 strax-1.6.2/strax/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-05 01:14:12.000000 strax-1.6.2/strax/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-05 01:14:12.000000 strax-1.6.2/strax/plugins/cut_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-05 01:14:12.000000 strax-1.6.2/strax/plugins/down_chunking_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-04-05 01:14:12.000000 strax-1.6.2/strax/plugins/loop_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-05 01:14:12.000000 strax-1.6.2/strax/plugins/merge_only_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-05 01:14:12.000000 strax-1.6.2/strax/plugins/overlap_window_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-04-05 01:14:12.000000 strax-1.6.2/strax/plugins/parrallel_source_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27126 2024-04-05 01:14:12.000000 strax-1.6.2/strax/plugins/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:14:17.133385 strax-1.6.2/strax/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 01:14:12.000000 strax-1.6.2/strax/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-05 01:14:12.000000 strax-1.6.2/strax/processing/data_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18567 2024-04-05 01:14:12.000000 strax-1.6.2/strax/processing/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22690 2024-04-05 01:14:12.000000 strax-1.6.2/strax/processing/hitlets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18761 2024-04-05 01:14:12.000000 strax-1.6.2/strax/processing/peak_building.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-04-05 01:14:12.000000 strax-1.6.2/strax/processing/peak_merging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-05 01:14:12.000000 strax-1.6.2/strax/processing/peak_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13738 2024-04-05 01:14:12.000000 strax-1.6.2/strax/processing/peak_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-04-05 01:14:12.000000 strax-1.6.2/strax/processing/pulse_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-04-05 01:14:12.000000 strax-1.6.2/strax/processing/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12799 2024-04-05 01:14:12.000000 strax-1.6.2/strax/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20209 2024-04-05 01:14:12.000000 strax-1.6.2/strax/run_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:14:17.133385 strax-1.6.2/strax/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 01:14:12.000000 strax-1.6.2/strax/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27542 2024-04-05 01:14:12.000000 strax-1.6.2/strax/storage/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-04-05 01:14:12.000000 strax-1.6.2/strax/storage/file_rechunker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14348 2024-04-05 01:14:12.000000 strax-1.6.2/strax/storage/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13716 2024-04-05 01:14:12.000000 strax-1.6.2/strax/storage/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-05 01:14:12.000000 strax-1.6.2/strax/storage/zipfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13619 2024-04-05 01:14:12.000000 strax-1.6.2/strax/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27108 2024-04-05 01:14:12.000000 strax-1.6.2/strax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:14:17.129385 strax-1.6.2/strax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27864 2024-04-05 01:14:17.000000 strax-1.6.2/strax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-05 01:14:17.000000 strax-1.6.2/strax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 01:14:17.000000 strax-1.6.2/strax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 01:14:17.000000 strax-1.6.2/strax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-05 01:14:17.000000 strax-1.6.2/strax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 01:14:17.000000 strax-1.6.2/strax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:14:17.137385 strax-1.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 01:14:12.000000 strax-1.6.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10983 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_child_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18309 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16134 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_cut_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_data_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_down_chunk_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_fixed_plugin_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15800 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_general_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_get_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20402 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_hitlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_inline_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_lone_hit_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_loop_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_mailbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11124 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_mongo_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_multi_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_overlap_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_peak_merging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10617 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_peak_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_peak_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_peak_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_pulse_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_saving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12270 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15816 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_superruns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_utils.py
```

### Comparing `strax-1.6.1/CODE-OF-CONDUCT.md` & `strax-1.6.2/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/CONTRIBUTING.md` & `strax-1.6.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/HISTORY.md` & `strax-1.6.2/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+1.6.2 / 2024-04-04
+---------------------
+* Use parentheses to separate the class name and attributes in the representation of StorageFrontend by @dachengx in https://github.com/AxFoundation/strax/pull/809
+* Specifically install `lxml_html_clean` by @dachengx in https://github.com/AxFoundation/strax/pull/812
+* Add a function to purge unused configs by @dachengx in https://github.com/AxFoundation/strax/pull/800
+* Warn if user checks is_stored for plugin not always saved by @cfuselli in https://github.com/AxFoundation/strax/pull/796
+* Bump urllib3 from 2.2.0 to 2.2.1 in /extra_requirements by @dependabot in https://github.com/AxFoundation/strax/pull/808
+* Do not call `get_components` in `is_stored` by @dachengx in https://github.com/AxFoundation/strax/pull/813
+
+New Contributors
+* @cfuselli made their first contribution in https://github.com/AxFoundation/strax/pull/796
+
+**Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.6.1...v1.6.2
+
+
 1.6.1 / 2024-02-17
 ---------------------
 * Remove a redundant function and fix some style by @dachengx in https://github.com/AxFoundation/strax/pull/795
 * Find the frontends which stored the targets by @dachengx in https://github.com/AxFoundation/strax/pull/802
 * Simpler chunk length check, avoid recursion limit crash by @JelleAalbers in https://github.com/AxFoundation/strax/pull/803
 * Deprecate the usage of `XENONnT/ax_env` by @dachengx in https://github.com/AxFoundation/strax/pull/804
 * Add a function to directly load file from strax folder by @dachengx in https://github.com/AxFoundation/strax/pull/801
```

### Comparing `strax-1.6.1/LICENSE` & `strax-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/PKG-INFO` & `strax-1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strax
-Version: 1.6.1
+Version: 1.6.2
 Summary: Streaming analysis for xenon TPCs
 Home-page: https://github.com/AxFoundation/strax
 Author: strax developers
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
@@ -36,14 +36,29 @@
 
 
 Strax is an analysis framework for pulse-only digitization data, specialized for live data reduction at speeds of 50-100 MB(raw) / core / sec. For more information, please see the [strax documentation](https://strax.readthedocs.io).
 
 Strax' primary aim is to support noble liquid TPC dark matter searches, such as XENONnT. The XENON-specific algorithms live in the separate package [straxen](https://github.com/XENONnT/straxen). If you want to try out strax, you probably want to start there. This package only contains the core framework and basic algorithms any TPCs would want to use.
 
 
+1.6.2 / 2024-04-04
+---------------------
+* Use parentheses to separate the class name and attributes in the representation of StorageFrontend by @dachengx in https://github.com/AxFoundation/strax/pull/809
+* Specifically install `lxml_html_clean` by @dachengx in https://github.com/AxFoundation/strax/pull/812
+* Add a function to purge unused configs by @dachengx in https://github.com/AxFoundation/strax/pull/800
+* Warn if user checks is_stored for plugin not always saved by @cfuselli in https://github.com/AxFoundation/strax/pull/796
+* Bump urllib3 from 2.2.0 to 2.2.1 in /extra_requirements by @dependabot in https://github.com/AxFoundation/strax/pull/808
+* Do not call `get_components` in `is_stored` by @dachengx in https://github.com/AxFoundation/strax/pull/813
+
+New Contributors
+* @cfuselli made their first contribution in https://github.com/AxFoundation/strax/pull/796
+
+**Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.6.1...v1.6.2
+
+
 1.6.1 / 2024-02-17
 ---------------------
 * Remove a redundant function and fix some style by @dachengx in https://github.com/AxFoundation/strax/pull/795
 * Find the frontends which stored the targets by @dachengx in https://github.com/AxFoundation/strax/pull/802
 * Simpler chunk length check, avoid recursion limit crash by @JelleAalbers in https://github.com/AxFoundation/strax/pull/803
 * Deprecate the usage of `XENONnT/ax_env` by @dachengx in https://github.com/AxFoundation/strax/pull/804
 * Add a function to directly load file from strax folder by @dachengx in https://github.com/AxFoundation/strax/pull/801
```

### Comparing `strax-1.6.1/README.md` & `strax-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/bin/rechunker` & `strax-1.6.2/bin/rechunker`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/setup.cfg` & `strax-1.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/setup.py` & `strax-1.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     readme = file.read()
 
 with open("HISTORY.md") as file:
     history = file.read()
 
 setuptools.setup(
     name="strax",
-    version="1.6.1",
+    version="1.6.2",
     description="Streaming analysis for xenon TPCs",
     author="strax developers",
     url="https://github.com/AxFoundation/strax",
     setup_requires=["pytest-runner"],
     install_requires=requires,
     tests_require=requires + tests_requires,
     long_description=readme + "\n\n" + history,
```

### Comparing `strax-1.6.1/strax/__init__.py` & `strax-1.6.2/strax/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # flake8: noqa
-__version__ = "1.6.1"
+__version__ = "1.6.2"
 
 # Glue the package together
 # See https://www.youtube.com/watch?v=0oTh1CXRaQ0 if this confuses you
 # The order of subpackes is not invariant, since we use strax.xxx inside strax
 from .utils import *
 from .chunk import *
 from .dtypes import *
```

### Comparing `strax-1.6.1/strax/chunk.py` & `strax-1.6.2/strax/chunk.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/config.py` & `strax-1.6.2/strax/config.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/context.py` & `strax-1.6.2/strax/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -384,14 +384,27 @@
 
                 except strax.InvalidConfiguration:
                     # These are option which are inherited from context options.
                     pass
 
         return plugin_class
 
+    def purge_unused_configs(self):
+        """Purge unused configs from the context."""
+        all_opts = set().union(
+            *[pc.takes_config.keys() for pc in self._plugin_class_registry.values()]
+        )
+        waiting_for = []
+        for k in self.config:
+            if not (k in all_opts or k in self.context_config["free_options"]):
+                self.log.warning(f"Option {k} purged from context config as it is not used.")
+                waiting_for.append(k)
+        for k in waiting_for:
+            del self.config[k]
+
     def deregister_plugins_with_missing_dependencies(self):
         """Deregister plugins in case a data_type the plugin depends on is not provided by any other
         plugin."""
         registry_changed = True
         while registry_changed:
             all_provides = set()
             plugins_to_deregister = []
@@ -1964,15 +1977,15 @@
                 RUN_DEFAULTS_KEY, dict()
             )
         except strax.RunMetadataNotAvailable:
             defs = dict()
         self._run_defaults_cache[run_id] = defs
         return defs
 
-    def is_stored(self, run_id, target, **kwargs):
+    def is_stored(self, run_id, target, detailed=False, **kwargs):
         """Return whether data type target has been saved for run_id through any of the registered
         storage frontends.
 
         Note that even if False is returned, the data type may still be made with a trivial
         computation.
 
         """
@@ -1986,14 +1999,30 @@
             # noinspection PyMethodFirstArgAssignment
             self = self.new_context(**kwargs)
 
         for sf in self._sorted_storage:
             if self._is_stored_in_sf(run_id, target, sf):
                 return True
         # None of the frontends has the data
+
+        # Before returning False, check if the data can be made trivially
+        plugin = self._plugin_class_registry[target]
+        save_when = plugin.save_when
+
+        # Mutli-target plugins provide a save_when per target
+        if isinstance(save_when, immutabledict):
+            save_when = save_when[target]
+
+        if save_when < strax.SaveWhen.ALWAYS and detailed:
+            warnings.warn(
+                f"{target} is not set to always be saved. "
+                "This is probably because it can be trivially made from other data. "
+                f"{target} depends on {plugin.depends_on}. Check if these are stored."
+            )
+
         return False
 
     def _check_forbidden(self):
         """Check that the forbid_creation_of config is of tuple type.
 
         Otherwise, try to make it a tuple
```

### Comparing `strax-1.6.1/strax/corrections.py` & `strax-1.6.2/strax/corrections.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/dtypes.py` & `strax-1.6.2/strax/dtypes.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/io.py` & `strax-1.6.2/strax/io.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/mailbox.py` & `strax-1.6.2/strax/mailbox.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/plugins/cut_plugin.py` & `strax-1.6.2/strax/plugins/cut_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/plugins/down_chunking_plugin.py` & `strax-1.6.2/strax/plugins/down_chunking_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/plugins/loop_plugin.py` & `strax-1.6.2/strax/plugins/loop_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/plugins/merge_only_plugin.py` & `strax-1.6.2/strax/plugins/merge_only_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/plugins/overlap_window_plugin.py` & `strax-1.6.2/strax/plugins/overlap_window_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/plugins/parrallel_source_plugin.py` & `strax-1.6.2/strax/plugins/parrallel_source_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/plugins/plugin.py` & `strax-1.6.2/strax/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/processing/data_reduction.py` & `strax-1.6.2/strax/processing/data_reduction.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/processing/general.py` & `strax-1.6.2/strax/processing/general.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/processing/hitlets.py` & `strax-1.6.2/strax/processing/hitlets.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/processing/peak_building.py` & `strax-1.6.2/strax/processing/peak_building.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/processing/peak_merging.py` & `strax-1.6.2/strax/processing/peak_merging.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/processing/peak_properties.py` & `strax-1.6.2/strax/processing/peak_properties.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/processing/peak_splitting.py` & `strax-1.6.2/strax/processing/peak_splitting.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/processing/pulse_processing.py` & `strax-1.6.2/strax/processing/pulse_processing.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/processing/statistics.py` & `strax-1.6.2/strax/processing/statistics.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/processor.py` & `strax-1.6.2/strax/processor.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/run_selection.py` & `strax-1.6.2/strax/run_selection.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/storage/common.py` & `strax-1.6.2/strax/storage/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,18 +162,21 @@
     def __str__(self):
         return self.__repr__()
 
     def __repr__(self):
         # List the relevant attributes ('path' is actually for the
         # strax.DataDirectory but it makes more sense to put it here).
         attributes = ("readonly", "path", "exclude", "take_only")
-        representation = f"{self.__class__.__module__}.{self.__class__.__name__}"
+        representation = ""
         for attr in attributes:
             if hasattr(self, attr) and getattr(self, attr):
                 representation += f", {attr}: {getattr(self, attr)}"
+        if representation:
+            representation = " (" + representation[2:] + ")"
+        representation = f"{self.__class__.__module__}.{self.__class__.__name__}" + representation
         return representation
 
     def loader(
         self,
         key: DataKey,
         time_range=None,
         allow_incomplete=False,
```

### Comparing `strax-1.6.1/strax/storage/file_rechunker.py` & `strax-1.6.2/strax/storage/file_rechunker.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/storage/files.py` & `strax-1.6.2/strax/storage/files.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/storage/mongo.py` & `strax-1.6.2/strax/storage/mongo.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/storage/zipfiles.py` & `strax-1.6.2/strax/storage/zipfiles.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/testutils.py` & `strax-1.6.2/strax/testutils.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax/utils.py` & `strax-1.6.2/strax/utils.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/strax.egg-info/PKG-INFO` & `strax-1.6.2/strax.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strax
-Version: 1.6.1
+Version: 1.6.2
 Summary: Streaming analysis for xenon TPCs
 Home-page: https://github.com/AxFoundation/strax
 Author: strax developers
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
@@ -36,14 +36,29 @@
 
 
 Strax is an analysis framework for pulse-only digitization data, specialized for live data reduction at speeds of 50-100 MB(raw) / core / sec. For more information, please see the [strax documentation](https://strax.readthedocs.io).
 
 Strax' primary aim is to support noble liquid TPC dark matter searches, such as XENONnT. The XENON-specific algorithms live in the separate package [straxen](https://github.com/XENONnT/straxen). If you want to try out strax, you probably want to start there. This package only contains the core framework and basic algorithms any TPCs would want to use.
 
 
+1.6.2 / 2024-04-04
+---------------------
+* Use parentheses to separate the class name and attributes in the representation of StorageFrontend by @dachengx in https://github.com/AxFoundation/strax/pull/809
+* Specifically install `lxml_html_clean` by @dachengx in https://github.com/AxFoundation/strax/pull/812
+* Add a function to purge unused configs by @dachengx in https://github.com/AxFoundation/strax/pull/800
+* Warn if user checks is_stored for plugin not always saved by @cfuselli in https://github.com/AxFoundation/strax/pull/796
+* Bump urllib3 from 2.2.0 to 2.2.1 in /extra_requirements by @dependabot in https://github.com/AxFoundation/strax/pull/808
+* Do not call `get_components` in `is_stored` by @dachengx in https://github.com/AxFoundation/strax/pull/813
+
+New Contributors
+* @cfuselli made their first contribution in https://github.com/AxFoundation/strax/pull/796
+
+**Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.6.1...v1.6.2
+
+
 1.6.1 / 2024-02-17
 ---------------------
 * Remove a redundant function and fix some style by @dachengx in https://github.com/AxFoundation/strax/pull/795
 * Find the frontends which stored the targets by @dachengx in https://github.com/AxFoundation/strax/pull/802
 * Simpler chunk length check, avoid recursion limit crash by @JelleAalbers in https://github.com/AxFoundation/strax/pull/803
 * Deprecate the usage of `XENONnT/ax_env` by @dachengx in https://github.com/AxFoundation/strax/pull/804
 * Add a function to directly load file from strax folder by @dachengx in https://github.com/AxFoundation/strax/pull/801
```

### Comparing `strax-1.6.1/strax.egg-info/SOURCES.txt` & `strax-1.6.2/strax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_child_plugins.py` & `strax-1.6.2/tests/test_child_plugins.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_config.py` & `strax-1.6.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_context.py` & `strax-1.6.2/tests/test_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -305,14 +305,21 @@
         st.register(Peaks)
         st.deregister_plugins_with_missing_dependencies()
         assert all([p in st._plugin_class_registry for p in "peaks records".split()])
         st._plugin_class_registry.pop("records", None)
         st.deregister_plugins_with_missing_dependencies()
         assert st._plugin_class_registry.pop("peaks", None) is None
 
+    def test_purge_configs(self):
+        """Tests if config purging is working:"""
+        st = self.get_context(True)
+        st.set_config({"you_will_not_use_this_config": 42})
+        st.purge_unused_configs()
+        assert st.config.get("you_will_not_use_this_config", None) is None
+
     def get_context(self, use_defaults, **kwargs):
         """Get simple context where we have one mock run in the only storage frontend."""
         assert isinstance(use_defaults, bool)
         st = strax.Context(storage=self.get_mock_sf(), check_available=("records",), **kwargs)
         st.set_context_config({"use_per_run_defaults": use_defaults})
         return st
```

### Comparing `strax-1.6.1/tests/test_core.py` & `strax-1.6.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_corrections.py` & `strax-1.6.2/tests/test_corrections.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_cut_plugin.py` & `strax-1.6.2/tests/test_cut_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_data_reduction.py` & `strax-1.6.2/tests/test_data_reduction.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_down_chunk_plugin.py` & `strax-1.6.2/tests/test_down_chunk_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_fixed_plugin_cache.py` & `strax-1.6.2/tests/test_fixed_plugin_cache.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_general_processing.py` & `strax-1.6.2/tests/test_general_processing.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_get_zarr.py` & `strax-1.6.2/tests/test_get_zarr.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_helpers.py` & `strax-1.6.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_hitlet.py` & `strax-1.6.2/tests/test_hitlet.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_inline_plugin.py` & `strax-1.6.2/tests/test_inline_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_lone_hit_integration.py` & `strax-1.6.2/tests/test_lone_hit_integration.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_loop_plugins.py` & `strax-1.6.2/tests/test_loop_plugins.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_mailbox.py` & `strax-1.6.2/tests/test_mailbox.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_mongo_frontend.py` & `strax-1.6.2/tests/test_mongo_frontend.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_multi_output.py` & `strax-1.6.2/tests/test_multi_output.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_overlap_plugin.py` & `strax-1.6.2/tests/test_overlap_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_peak_merging.py` & `strax-1.6.2/tests/test_peak_merging.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_peak_processing.py` & `strax-1.6.2/tests/test_peak_processing.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_peak_properties.py` & `strax-1.6.2/tests/test_peak_properties.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_peak_splitting.py` & `strax-1.6.2/tests/test_peak_splitting.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_pulse_processing.py` & `strax-1.6.2/tests/test_pulse_processing.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_saving.py` & `strax-1.6.2/tests/test_saving.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_statistics.py` & `strax-1.6.2/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_storage.py` & `strax-1.6.2/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_superruns.py` & `strax-1.6.2/tests/test_superruns.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.1/tests/test_utils.py` & `strax-1.6.2/tests/test_utils.py`

 * *Files identical despite different names*

