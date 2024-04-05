# Comparing `tmp/luxonis-ml-0.0.1.tar.gz` & `tmp/luxonis-ml-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luxonis-ml-0.0.1.tar", last modified: Wed Jan 10 14:31:32 2024, max compression
+gzip compressed data, was "luxonis-ml-0.1.0.tar", last modified: Fri Apr  5 14:38:12 2024, max compression
```

## Comparing `luxonis-ml-0.0.1.tar` & `luxonis-ml-0.1.0.tar`

### file list

```diff
@@ -1,80 +1,134 @@
-drwxrwxr-x   0 matija    (1000) matija    (1000)        0 2024-01-10 14:31:32.293228 luxonis-ml-0.0.1/
--rw-rw-r--   0 matija    (1000) matija    (1000)    11357 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/LICENSE
--rw-r--r--   0 matija    (1000) matija    (1000)    21788 2024-01-10 14:31:32.293228 luxonis-ml-0.0.1/PKG-INFO
--rw-rw-r--   0 matija    (1000) matija    (1000)     2134 2024-01-10 14:29:21.000000 luxonis-ml-0.0.1/README.md
-drwxrwxr-x   0 matija    (1000) matija    (1000)        0 2024-01-10 14:31:32.213228 luxonis-ml-0.0.1/examples/
-drwxrwxr-x   0 matija    (1000) matija    (1000)        0 2024-01-10 14:31:32.225228 luxonis-ml-0.0.1/examples/utils/
--rw-rw-r--   0 matija    (1000) matija    (1000)     3207 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/examples/utils/data_utils.py
-drwxrwxr-x   0 matija    (1000) matija    (1000)        0 2024-01-10 14:31:32.225228 luxonis-ml-0.0.1/luxonis_ml/
--rw-rw-r--   0 matija    (1000) matija    (1000)        0 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/__init__.py
-drwxrwxr-x   0 matija    (1000) matija    (1000)        0 2024-01-10 14:31:32.233228 luxonis-ml-0.0.1/luxonis_ml/data/
--rw-rw-r--   0 matija    (1000) matija    (1000)      956 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/data/__init__.py
-drwxrwxr-x   0 matija    (1000) matija    (1000)        0 2024-01-10 14:31:32.237228 luxonis-ml-0.0.1/luxonis_ml/data/augmentations/
--rw-rw-r--   0 matija    (1000) matija    (1000)      260 2024-01-10 14:29:21.000000 luxonis-ml-0.0.1/luxonis_ml/data/augmentations/__init__.py
--rw-rw-r--   0 matija    (1000) matija    (1000)    15489 2024-01-10 14:29:21.000000 luxonis-ml-0.0.1/luxonis_ml/data/augmentations/batch_compose.py
--rw-rw-r--   0 matija    (1000) matija    (1000)     5922 2024-01-10 14:29:21.000000 luxonis-ml-0.0.1/luxonis_ml/data/augmentations/batch_processors.py
--rw-rw-r--   0 matija    (1000) matija    (1000)     2143 2024-01-10 14:29:21.000000 luxonis-ml-0.0.1/luxonis_ml/data/augmentations/batch_transform.py
--rw-rw-r--   0 matija    (1000) matija    (1000)     2498 2024-01-10 14:29:21.000000 luxonis-ml-0.0.1/luxonis_ml/data/augmentations/batch_utils.py
-drwxrwxr-x   0 matija    (1000) matija    (1000)        0 2024-01-10 14:31:32.237228 luxonis-ml-0.0.1/luxonis_ml/data/augmentations/custom/
--rw-rw-r--   0 matija    (1000) matija    (1000)      150 2024-01-10 14:29:21.000000 luxonis-ml-0.0.1/luxonis_ml/data/augmentations/custom/__init__.py
--rw-rw-r--   0 matija    (1000) matija    (1000)     9837 2024-01-10 14:29:21.000000 luxonis-ml-0.0.1/luxonis_ml/data/augmentations/custom/letterbox_resize.py
--rw-rw-r--   0 matija    (1000) matija    (1000)     6454 2024-01-10 14:29:21.000000 luxonis-ml-0.0.1/luxonis_ml/data/augmentations/custom/mixup.py
--rw-rw-r--   0 matija    (1000) matija    (1000)    17275 2024-01-10 14:29:21.000000 luxonis-ml-0.0.1/luxonis_ml/data/augmentations/custom/mosaic.py
--rw-rw-r--   0 matija    (1000) matija    (1000)    21026 2024-01-10 14:29:21.000000 luxonis-ml-0.0.1/luxonis_ml/data/augmentations/utils.py
--rw-rw-r--   0 matija    (1000) matija    (1000)    31226 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/data/dataset.py
--rw-rw-r--   0 matija    (1000) matija    (1000)    10537 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/data/loader.py
--rw-rw-r--   0 matija    (1000) matija    (1000)    44505 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/data/parsers.py
--rw-rw-r--   0 matija    (1000) matija    (1000)      255 2024-01-10 14:29:21.000000 luxonis-ml-0.0.1/luxonis_ml/data/requirements.txt
-drwxrwxr-x   0 matija    (1000) matija    (1000)        0 2024-01-10 14:31:32.237228 luxonis-ml-0.0.1/luxonis_ml/data/utils/
--rw-rw-r--   0 matija    (1000) matija    (1000)        0 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/data/utils/__init__.py
--rw-rw-r--   0 matija    (1000) matija    (1000)      563 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/data/utils/constants.py
--rw-rw-r--   0 matija    (1000) matija    (1000)     4732 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/data/utils/data_utils.py
--rw-rw-r--   0 matija    (1000) matija    (1000)     1358 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/data/utils/enums.py
--rw-rw-r--   0 matija    (1000) matija    (1000)     2707 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/data/utils/labelstudio.py
--rw-rw-r--   0 matija    (1000) matija    (1000)     3605 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/data/utils/parquet.py
-drwxrwxr-x   0 matija    (1000) matija    (1000)        0 2024-01-10 14:31:32.237228 luxonis-ml-0.0.1/luxonis_ml/embeddings/
--rw-rw-r--   0 matija    (1000) matija    (1000)     1361 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/embeddings/__init__.py
-drwxrwxr-x   0 matija    (1000) matija    (1000)        0 2024-01-10 14:31:32.241228 luxonis-ml-0.0.1/luxonis_ml/embeddings/methods/
--rw-rw-r--   0 matija    (1000) matija    (1000)     3482 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/embeddings/methods/OOD.py
--rw-rw-r--   0 matija    (1000) matija    (1000)      550 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/embeddings/methods/__init__.py
--rw-rw-r--   0 matija    (1000) matija    (1000)     9167 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/embeddings/methods/duplicate.py
--rw-rw-r--   0 matija    (1000) matija    (1000)     4680 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/embeddings/methods/mistakes.py
--rw-rw-r--   0 matija    (1000) matija    (1000)     6371 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/embeddings/methods/representative.py
--rw-rw-r--   0 matija    (1000) matija    (1000)      312 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/embeddings/requirements.txt
-drwxrwxr-x   0 matija    (1000) matija    (1000)        0 2024-01-10 14:31:32.261228 luxonis-ml-0.0.1/luxonis_ml/embeddings/utils/
--rw-rw-r--   0 matija    (1000) matija    (1000)      738 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/embeddings/utils/__init__.py
--rw-rw-r--   0 matija    (1000) matija    (1000)     3538 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/embeddings/utils/embedding.py
--rw-rw-r--   0 matija    (1000) matija    (1000)    12121 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/embeddings/utils/ldf.py
--rw-rw-r--   0 matija    (1000) matija    (1000)     4709 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/embeddings/utils/model.py
--rw-rw-r--   0 matija    (1000) matija    (1000)    19362 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/embeddings/utils/qdrant.py
-drwxrwxr-x   0 matija    (1000) matija    (1000)        0 2024-01-10 14:31:32.265228 luxonis-ml-0.0.1/luxonis_ml/enums/
--rw-rw-r--   0 matija    (1000) matija    (1000)       82 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/enums/__init__.py
--rw-rw-r--   0 matija    (1000) matija    (1000)      405 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/enums/enums.py
--rw-rw-r--   0 matija    (1000) matija    (1000)      508 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/guard_extras.py
-drwxrwxr-x   0 matija    (1000) matija    (1000)        0 2024-01-10 14:31:32.265228 luxonis-ml-0.0.1/luxonis_ml/tracker/
--rw-rw-r--   0 matija    (1000) matija    (1000)      248 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/tracker/__init__.py
--rw-rw-r--   0 matija    (1000) matija    (1000)      631 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/tracker/mlflow_plugins.py
--rw-rw-r--   0 matija    (1000) matija    (1000)      135 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/tracker/requirements.txt
--rw-rw-r--   0 matija    (1000) matija    (1000)    11667 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/tracker/tracker.py
-drwxrwxr-x   0 matija    (1000) matija    (1000)        0 2024-01-10 14:31:32.269228 luxonis-ml-0.0.1/luxonis_ml/utils/
--rw-rw-r--   0 matija    (1000) matija    (1000)      448 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/utils/__init__.py
--rw-rw-r--   0 matija    (1000) matija    (1000)     8824 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/utils/config.py
--rw-rw-r--   0 matija    (1000) matija    (1000)     1437 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/utils/environ.py
--rw-rw-r--   0 matija    (1000) matija    (1000)    17712 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/utils/filesystem.py
--rw-rw-r--   0 matija    (1000) matija    (1000)     2897 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/utils/logging.py
--rw-rw-r--   0 matija    (1000) matija    (1000)     5779 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/utils/registry.py
--rw-rw-r--   0 matija    (1000) matija    (1000)      176 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/luxonis_ml/utils/requirements.txt
-drwxrwxr-x   0 matija    (1000) matija    (1000)        0 2024-01-10 14:31:32.273228 luxonis-ml-0.0.1/luxonis_ml.egg-info/
--rw-r--r--   0 matija    (1000) matija    (1000)    21788 2024-01-10 14:31:32.000000 luxonis-ml-0.0.1/luxonis_ml.egg-info/PKG-INFO
--rw-rw-r--   0 matija    (1000) matija    (1000)     2092 2024-01-10 14:31:32.000000 luxonis-ml-0.0.1/luxonis_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 matija    (1000) matija    (1000)        1 2024-01-10 14:31:32.000000 luxonis-ml-0.0.1/luxonis_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 matija    (1000) matija    (1000)     2167 2024-01-10 14:31:32.000000 luxonis-ml-0.0.1/luxonis_ml.egg-info/requires.txt
--rw-rw-r--   0 matija    (1000) matija    (1000)       46 2024-01-10 14:31:32.000000 luxonis-ml-0.0.1/luxonis_ml.egg-info/top_level.txt
--rw-rw-r--   0 matija    (1000) matija    (1000)     2331 2024-01-06 16:44:19.000000 luxonis-ml-0.0.1/pyproject.toml
--rw-rw-r--   0 matija    (1000) matija    (1000)       88 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/requirements-dev.txt
--rw-rw-r--   0 matija    (1000) matija    (1000)       38 2024-01-10 14:31:32.293228 luxonis-ml-0.0.1/setup.cfg
-drwxrwxr-x   0 matija    (1000) matija    (1000)        0 2024-01-10 14:31:32.221228 luxonis-ml-0.0.1/tests/
-drwxrwxr-x   0 matija    (1000) matija    (1000)        0 2024-01-10 14:31:32.273228 luxonis-ml-0.0.1/tests/test_utils/
--rw-rw-r--   0 matija    (1000) matija    (1000)     8746 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/tests/test_utils/test_config.py
--rw-rw-r--   0 matija    (1000) matija    (1000)      454 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/tests/test_utils/test_filesystem.py
--rw-rw-r--   0 matija    (1000) matija    (1000)     2335 2024-01-05 15:51:52.000000 luxonis-ml-0.0.1/tests/test_utils/test_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:12.646727 luxonis-ml-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22228 2024-04-05 14:38:12.646727 luxonis-ml-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:12.610727 luxonis-ml-0.1.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:12.614727 luxonis-ml-0.1.0/examples/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/examples/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/examples/utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:12.614727 luxonis-ml-0.1.0/luxonis_ml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:12.618727 luxonis-ml-0.1.0/luxonis_ml/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:12.618727 luxonis-ml-0.1.0/luxonis_ml/data/augmentations/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/augmentations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15489 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/augmentations/batch_compose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/augmentations/batch_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/augmentations/batch_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/augmentations/batch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:12.618727 luxonis-ml-0.1.0/luxonis_ml/data/augmentations/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/augmentations/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/augmentations/custom/letterbox_resize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/augmentations/custom/mixup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17279 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/augmentations/custom/mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21026 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/augmentations/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:12.618727 luxonis-ml-0.1.0/luxonis_ml/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/datasets/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28298 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/datasets/luxonis_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/datasets/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10767 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:12.622727 luxonis-ml-0.1.0/luxonis_ml/data/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/parsers/base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/parsers/classification_directory_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/parsers/coco_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/parsers/create_ml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/parsers/darknet_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/parsers/luxonis_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/parsers/segmentation_mask_directory_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/parsers/solo_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/parsers/tensorflow_csv_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/parsers/voc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/parsers/yolov4_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/parsers/yolov6_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:12.622727 luxonis-ml-0.1.0/luxonis_ml/data/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/utils/labelstudio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/data/utils/parquet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:12.622727 luxonis-ml-0.1.0/luxonis_ml/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/embeddings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:12.626727 luxonis-ml-0.1.0/luxonis_ml/embeddings/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/embeddings/methods/OOD.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/embeddings/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/embeddings/methods/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/embeddings/methods/mistakes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/embeddings/methods/representative.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/embeddings/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:12.626727 luxonis-ml-0.1.0/luxonis_ml/embeddings/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/embeddings/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/embeddings/utils/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/embeddings/utils/ldf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/embeddings/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17476 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/embeddings/utils/qdrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/embeddings/utils/vectordb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10926 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/embeddings/utils/weaviate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:12.626727 luxonis-ml-0.1.0/luxonis_ml/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/enums/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/guard_extras.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:12.626727 luxonis-ml-0.1.0/luxonis_ml/nn_archive/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/nn_archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/nn_archive/archive_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/nn_archive/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:12.626727 luxonis-ml-0.1.0/luxonis_ml/nn_archive/config_building_blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/nn_archive/config_building_blocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:12.630727 luxonis-ml-0.1.0/luxonis_ml/nn_archive/config_building_blocks/base_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/nn_archive/config_building_blocks/base_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/nn_archive/config_building_blocks/base_models/custom_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9376 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/nn_archive/config_building_blocks/base_models/head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/nn_archive/config_building_blocks/base_models/head_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/nn_archive/config_building_blocks/base_models/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/nn_archive/config_building_blocks/base_models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/nn_archive/config_building_blocks/base_models/output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:12.630727 luxonis-ml-0.1.0/luxonis_ml/nn_archive/config_building_blocks/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/nn_archive/config_building_blocks/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/nn_archive/config_building_blocks/enums/data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/nn_archive/config_building_blocks/enums/decoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/nn_archive/config_building_blocks/enums/input_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/nn_archive/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/nn_archive/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/nn_archive/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:12.630727 luxonis-ml-0.1.0/luxonis_ml/tracker/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/tracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/tracker/mlflow_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/tracker/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/tracker/tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:12.630727 luxonis-ml-0.1.0/luxonis_ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/utils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8824 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/utils/environ.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23001 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/luxonis_ml/utils/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:12.634727 luxonis-ml-0.1.0/luxonis_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22228 2024-04-05 14:38:12.000000 luxonis-ml-0.1.0/luxonis_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-05 14:38:12.000000 luxonis-ml-0.1.0/luxonis_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:38:12.000000 luxonis-ml-0.1.0/luxonis_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 14:38:12.000000 luxonis-ml-0.1.0/luxonis_ml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-05 14:38:12.000000 luxonis-ml-0.1.0/luxonis_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-05 14:38:12.000000 luxonis-ml-0.1.0/luxonis_ml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:38:12.646727 luxonis-ml-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:12.614727 luxonis-ml-0.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:12.630727 luxonis-ml-0.1.0/tests/test_augmentations/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/tests/test_augmentations/test_letterbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/tests/test_augmentations/test_mixup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/tests/test_augmentations/test_mosaic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:12.630727 luxonis-ml-0.1.0/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/tests/test_data/test_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:12.634727 luxonis-ml-0.1.0/tests/test_nn_archive/
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/tests/test_nn_archive/test_nn_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:12.634727 luxonis-ml-0.1.0/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     8746 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/tests/test_utils/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/tests/test_utils/test_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-05 14:37:58.000000 luxonis-ml-0.1.0/tests/test_utils/test_registry.py
```

### Comparing `luxonis-ml-0.0.1/LICENSE` & `luxonis-ml-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `luxonis-ml-0.0.1/PKG-INFO` & `luxonis-ml-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxonis-ml
-Version: 0.0.1
+Version: 0.1.0
 Summary: MLOps tools for training models for Luxonis devices
 Author-email: Luxonis <support@luxonis.com>
 Maintainer-email: Luxonis <support@luxonis.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -242,31 +242,31 @@
 Requires-Dist: pydantic-settings>=2.1.0; extra == "utils"
 Requires-Dist: PyYAML>=6.0; extra == "utils"
 Requires-Dist: fsspec>=2023.1.0; extra == "utils"
 Requires-Dist: rich>=13.6.0; extra == "utils"
 Provides-Extra: tracker
 Requires-Dist: unique-names-generator>=1.0.2; extra == "tracker"
 Requires-Dist: numpy>=1.22; extra == "tracker"
-Requires-Dist: mlflow>=2.0.1; extra == "tracker"
 Provides-Extra: embedd
 Requires-Dist: docker>=6.1.3; extra == "embedd"
 Requires-Dist: KDEpy>=1.1.5; extra == "embedd"
 Requires-Dist: kmedoids>=0.4.3; extra == "embedd"
 Requires-Dist: matplotlib>=3.7.2; extra == "embedd"
 Requires-Dist: numpy>=1.22; extra == "embedd"
 Requires-Dist: onnx>=1.14.0; extra == "embedd"
 Requires-Dist: onnxruntime-gpu>=1.15.1; sys_platform == "linux" and extra == "embedd"
 Requires-Dist: onnxruntime>=1.15.1; sys_platform != "linux" and extra == "embedd"
 Requires-Dist: opencv-python>=4.7.0.68; extra == "embedd"
 Requires-Dist: qdrant-client>=1.4.0; extra == "embedd"
+Requires-Dist: weaviate-client>=4.4b2; extra == "embedd"
 Requires-Dist: scikit-learn>=1.3.0; extra == "embedd"
 Requires-Dist: scipy>=1.10.1; extra == "embedd"
-Requires-Dist: torch>=1.13.1; extra == "embedd"
-Requires-Dist: torchaudio>=0.13.1; extra == "embedd"
-Requires-Dist: torchvision>=0.14.1; extra == "embedd"
+Provides-Extra: nn-archive
+Requires-Dist: pydantic>=2.4.0; extra == "nn-archive"
+Requires-Dist: pydantic-settings>=2.1.0; extra == "nn-archive"
 Provides-Extra: all
 Requires-Dist: numpy>=1.22; extra == "all"
 Requires-Dist: tqdm>=4.64.1; extra == "all"
 Requires-Dist: opencv-python==4.7.0.68; extra == "all"
 Requires-Dist: opencv-python-headless==4.7.0.68; extra == "all"
 Requires-Dist: PyYAML>=6.0; extra == "all"
 Requires-Dist: label-studio-sdk>=0.0.28; extra == "all"
@@ -278,30 +278,29 @@
 Requires-Dist: pydantic>=2.4.0; extra == "all"
 Requires-Dist: pydantic-settings>=2.1.0; extra == "all"
 Requires-Dist: PyYAML>=6.0; extra == "all"
 Requires-Dist: fsspec>=2023.1.0; extra == "all"
 Requires-Dist: rich>=13.6.0; extra == "all"
 Requires-Dist: unique-names-generator>=1.0.2; extra == "all"
 Requires-Dist: numpy>=1.22; extra == "all"
-Requires-Dist: mlflow>=2.0.1; extra == "all"
 Requires-Dist: docker>=6.1.3; extra == "all"
 Requires-Dist: KDEpy>=1.1.5; extra == "all"
 Requires-Dist: kmedoids>=0.4.3; extra == "all"
 Requires-Dist: matplotlib>=3.7.2; extra == "all"
 Requires-Dist: numpy>=1.22; extra == "all"
 Requires-Dist: onnx>=1.14.0; extra == "all"
 Requires-Dist: onnxruntime-gpu>=1.15.1; sys_platform == "linux" and extra == "all"
 Requires-Dist: onnxruntime>=1.15.1; sys_platform != "linux" and extra == "all"
 Requires-Dist: opencv-python>=4.7.0.68; extra == "all"
 Requires-Dist: qdrant-client>=1.4.0; extra == "all"
+Requires-Dist: weaviate-client>=4.4b2; extra == "all"
 Requires-Dist: scikit-learn>=1.3.0; extra == "all"
 Requires-Dist: scipy>=1.10.1; extra == "all"
-Requires-Dist: torch>=1.13.1; extra == "all"
-Requires-Dist: torchaudio>=0.13.1; extra == "all"
-Requires-Dist: torchvision>=0.14.1; extra == "all"
+Requires-Dist: pydantic>=2.4.0; extra == "all"
+Requires-Dist: pydantic-settings>=2.1.0; extra == "all"
 Provides-Extra: dev
 Requires-Dist: numpy>=1.22; extra == "dev"
 Requires-Dist: tqdm>=4.64.1; extra == "dev"
 Requires-Dist: opencv-python==4.7.0.68; extra == "dev"
 Requires-Dist: opencv-python-headless==4.7.0.68; extra == "dev"
 Requires-Dist: PyYAML>=6.0; extra == "dev"
 Requires-Dist: label-studio-sdk>=0.0.28; extra == "dev"
@@ -313,44 +312,49 @@
 Requires-Dist: pydantic>=2.4.0; extra == "dev"
 Requires-Dist: pydantic-settings>=2.1.0; extra == "dev"
 Requires-Dist: PyYAML>=6.0; extra == "dev"
 Requires-Dist: fsspec>=2023.1.0; extra == "dev"
 Requires-Dist: rich>=13.6.0; extra == "dev"
 Requires-Dist: unique-names-generator>=1.0.2; extra == "dev"
 Requires-Dist: numpy>=1.22; extra == "dev"
-Requires-Dist: mlflow>=2.0.1; extra == "dev"
 Requires-Dist: docker>=6.1.3; extra == "dev"
 Requires-Dist: KDEpy>=1.1.5; extra == "dev"
 Requires-Dist: kmedoids>=0.4.3; extra == "dev"
 Requires-Dist: matplotlib>=3.7.2; extra == "dev"
 Requires-Dist: numpy>=1.22; extra == "dev"
 Requires-Dist: onnx>=1.14.0; extra == "dev"
 Requires-Dist: onnxruntime-gpu>=1.15.1; sys_platform == "linux" and extra == "dev"
 Requires-Dist: onnxruntime>=1.15.1; sys_platform != "linux" and extra == "dev"
 Requires-Dist: opencv-python>=4.7.0.68; extra == "dev"
 Requires-Dist: qdrant-client>=1.4.0; extra == "dev"
+Requires-Dist: weaviate-client>=4.4b2; extra == "dev"
 Requires-Dist: scikit-learn>=1.3.0; extra == "dev"
 Requires-Dist: scipy>=1.10.1; extra == "dev"
-Requires-Dist: torch>=1.13.1; extra == "dev"
-Requires-Dist: torchaudio>=0.13.1; extra == "dev"
-Requires-Dist: torchvision>=0.14.1; extra == "dev"
+Requires-Dist: pydantic>=2.4.0; extra == "dev"
+Requires-Dist: pydantic-settings>=2.1.0; extra == "dev"
 Requires-Dist: pre-commit>=3.2.1; extra == "dev"
 Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
+Requires-Dist: pytest-dependency>=0.6.0; extra == "dev"
 Requires-Dist: pytest-md>=0.2.0; extra == "dev"
 Requires-Dist: gdown>=4.7.1; extra == "dev"
 Requires-Dist: coverage-badge>=1.1.0; extra == "dev"
 
 # LuxonisML
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-![PyBadge](media/pybadge.svg)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+![PyBadge](https://github.com/luxonis/luxonis-ml/blob/116262ee55c36433861689077a522faeb32b3967/media/pybadge.svg)
+![PyPI](https://img.shields.io/pypi/v/luxonis-ml?label=pypi%20package)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/luxonis-ml)
+
 ![CI](https://github.com/luxonis/luxonis-ml/actions/workflows/ci.yaml/badge.svg)
-![Docs](https://github.com/luxonis/luxonis-ml/actions/workflows/docs.yaml/badge.svg)
-![Coverage](media/coverage_badge.svg)
+![Coverage](https://github.com/luxonis/luxonis-ml/blob/dev/media/coverage_badge.svg)
+
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Docformatter](https://img.shields.io/badge/%20formatter-docformatter-fedcba.svg)](https://github.com/PyCQA/docformatter)
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 This library includes a collection of helper functions and utilities for the Luxonis MLOps stack. This includes the following submodules:
 
 - **Dataset Management**: Creating computer vision datasets focused around Luxonis hardware and loading data into our training library.
 - **Embeddings**: Methods to compute image embeddings.
 - **Tracking**: Our implementation of a logger for use with PyTorch Lightning or in our training library.
 - **Utils**: Miscellaneous utils for developers. See this README for details on the different utils.
@@ -380,8 +384,8 @@
 
 ```bash
 pip install luxonis-ml[all]
 ```
 
 ## Contributing
 
-If you want to contribute to this project, read the instructions in [CONTRIBUTING.md](CONTRIBUTING.md)
+If you want to contribute to this project, read the instructions in [CONTRIBUTING.md](https://github.com/luxonis/luxonis-ml/blob/main/CONTRIBUTING.md)
```

### Comparing `luxonis-ml-0.0.1/README.md` & `luxonis-ml-0.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 # LuxonisML
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-![PyBadge](media/pybadge.svg)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+![PyBadge](https://github.com/luxonis/luxonis-ml/blob/116262ee55c36433861689077a522faeb32b3967/media/pybadge.svg)
+![PyPI](https://img.shields.io/pypi/v/luxonis-ml?label=pypi%20package)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/luxonis-ml)
+
 ![CI](https://github.com/luxonis/luxonis-ml/actions/workflows/ci.yaml/badge.svg)
-![Docs](https://github.com/luxonis/luxonis-ml/actions/workflows/docs.yaml/badge.svg)
-![Coverage](media/coverage_badge.svg)
+![Coverage](https://github.com/luxonis/luxonis-ml/blob/dev/media/coverage_badge.svg)
+
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Docformatter](https://img.shields.io/badge/%20formatter-docformatter-fedcba.svg)](https://github.com/PyCQA/docformatter)
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 This library includes a collection of helper functions and utilities for the Luxonis MLOps stack. This includes the following submodules:
 
 - **Dataset Management**: Creating computer vision datasets focused around Luxonis hardware and loading data into our training library.
 - **Embeddings**: Methods to compute image embeddings.
 - **Tracking**: Our implementation of a logger for use with PyTorch Lightning or in our training library.
 - **Utils**: Miscellaneous utils for developers. See this README for details on the different utils.
@@ -39,8 +44,8 @@
 
 ```bash
 pip install luxonis-ml[all]
 ```
 
 ## Contributing
 
-If you want to contribute to this project, read the instructions in [CONTRIBUTING.md](CONTRIBUTING.md)
+If you want to contribute to this project, read the instructions in [CONTRIBUTING.md](https://github.com/luxonis/luxonis-ml/blob/main/CONTRIBUTING.md)
```

### Comparing `luxonis-ml-0.0.1/examples/utils/data_utils.py` & `luxonis-ml-0.1.0/examples/utils/data_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,22 +23,20 @@
         images, labels = batch
         ...  # Your processing here
     ```
 
 Note: This loader is particularly useful when you want to use MNIST data with models that were
 pre-trained on datasets like ImageNet and expect 3-channel RGB input.
 """
-
-
 import torch
 import torchvision
 import torchvision.transforms as transforms
 
 
-def mnist_transformations():
+def mnist_transformations() -> transforms.Compose:
     """Returns composed transformations for the MNIST dataset.
 
     Transforms the images from 1 channel grayscale to 3 channels RGB and resizes them.
     """
     return transforms.Compose(
         [
             transforms.Grayscale(num_output_channels=3),
@@ -46,15 +44,17 @@
             transforms.Resize((224, 224)),
             transforms.ToTensor(),
             transforms.Normalize(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225]),
         ]
     )
 
 
-def load_mnist_data(save_path="./mnist", num_samples=640, batch_size=64):
+def load_mnist_data(
+    save_path: str = "./mnist", num_samples: int = 640, batch_size: int = 64
+) -> torch.utils.data.DataLoader:
     """Loads the MNIST dataset with the specified preprocessing.
 
     Parameters:
     - save_path (str): Directory to save/load the MNIST data.
     - num_samples (int): Number of samples to load from the dataset.
                          Set as -1 to load the entire dataset.
     - batch_size (int): Batch size for the DataLoader.
```

### Comparing `luxonis-ml-0.0.1/luxonis_ml/data/augmentations/batch_compose.py` & `luxonis-ml-0.1.0/luxonis_ml/data/augmentations/batch_compose.py`

 * *Files identical despite different names*

### Comparing `luxonis-ml-0.0.1/luxonis_ml/data/augmentations/batch_processors.py` & `luxonis-ml-0.1.0/luxonis_ml/data/augmentations/batch_processors.py`

 * *Files identical despite different names*

### Comparing `luxonis-ml-0.0.1/luxonis_ml/data/augmentations/batch_transform.py` & `luxonis-ml-0.1.0/luxonis_ml/data/augmentations/batch_transform.py`

 * *Files identical despite different names*

### Comparing `luxonis-ml-0.0.1/luxonis_ml/data/augmentations/batch_utils.py` & `luxonis-ml-0.1.0/luxonis_ml/data/augmentations/batch_utils.py`

 * *Files identical despite different names*

### Comparing `luxonis-ml-0.0.1/luxonis_ml/data/augmentations/custom/letterbox_resize.py` & `luxonis-ml-0.1.0/luxonis_ml/data/augmentations/custom/letterbox_resize.py`

 * *Files identical despite different names*

### Comparing `luxonis-ml-0.0.1/luxonis_ml/data/augmentations/custom/mixup.py` & `luxonis-ml-0.1.0/luxonis_ml/data/augmentations/custom/mixup.py`

 * *Files identical despite different names*

### Comparing `luxonis-ml-0.0.1/luxonis_ml/data/augmentations/custom/mosaic.py` & `luxonis-ml-0.1.0/luxonis_ml/data/augmentations/custom/mosaic.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,15 +417,15 @@
     keypoint: KeypointInternalType,
     rows: int,
     cols: int,
     position_index: int,
     height: int,
     width: int,
 ) -> KeypointInternalType:
-    """Put the given bbox in one of the cells of the 2x2 grid.
+    """Put the given keypoint in one of the cells of the 2x2 grid.
 
     @param keypoint: A keypoint `(x, y, angle, scale)`.
     @type bbox: KeypointInternalType
     @param rows: Height of input image that corresponds to one of the mosaic cells
     @type rows: int
     @param cols: Width of input image that corresponds to one of the mosaic cells
     @type cols: int
```

### Comparing `luxonis-ml-0.0.1/luxonis_ml/data/augmentations/utils.py` & `luxonis-ml-0.1.0/luxonis_ml/data/augmentations/utils.py`

 * *Files identical despite different names*

### Comparing `luxonis-ml-0.0.1/luxonis_ml/data/dataset.py` & `luxonis-ml-0.1.0/luxonis_ml/data/datasets/luxonis_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,105 +1,34 @@
 import json
 import logging
 import os
 import os.path as osp
 import shutil
 import time
 from datetime import datetime
-from typing import Any, Callable, Dict, Generator, List, Optional, Tuple
+from pathlib import Path
+from typing import Dict, List, Optional, Tuple
 
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
-from tqdm import tqdm
+import rich.progress
 
 import luxonis_ml.data.utils.data_utils as data_utils
-from luxonis_ml.data.utils.parquet import ParquetFileManager
 from luxonis_ml.utils import LuxonisFileSystem, environ
 
-from .utils.constants import LABEL_TYPES, LDF_VERSION
-from .utils.enums import BucketStorage, BucketType, ImageType, MediaType
+from ..utils.constants import LABEL_TYPES, LDF_VERSION
+from ..utils.enums import BucketStorage, BucketType, ImageType, MediaType
+from ..utils.parquet import ParquetFileManager
+from .base_dataset import BaseDataset, DatasetGeneratorFunction
+from .source import LuxonisComponent, LuxonisSource
 
-DatasetGenerator = Generator[Dict[str, Any], None, None]
-DatasetGeneratorFunction = Callable[[], DatasetGenerator]
 
-
-class LuxonisComponent:
-    def __init__(
-        self,
-        name: str,
-        media_type: MediaType = MediaType.IMAGE,
-        image_type: Optional[ImageType] = ImageType.COLOR,
-    ) -> None:
-        """Abstraction for a piece of media within a source. Most commonly, this
-        abstracts an image sensor.
-
-        @type name: str
-        @param name: A recognizable name for the component.
-        @type media_type: MediaType
-        @param media_type: Enum for the type of media for the component.
-        @type image_type: Optional[ImageType]
-        @param image_type: Enum for the image type if C{media_type==MediaType.IMAGE}.
-            Else this param can be None or default.
-        """
-
-        if media_type not in MediaType:
-            raise Exception(f"{media_type.value} is not a valid MediaType")
-        if image_type not in ImageType:
-            raise Exception(f"{image_type.value} is not a valid ImageType")
-
-        self.name = name
-        self.media_type = media_type
-        self.image_type = image_type
-
-        if media_type == MediaType.IMAGE:
-            self.image_type = image_type
-        else:
-            self.image_type = None
-
-
-class LuxonisSource:
-    """Abstracts the structure of a dataset and which components/media are included."""
-
-    def __init__(
-        self,
-        name: str,
-        components: Optional[List[LuxonisComponent]] = None,
-        main_component: Optional[str] = None,
-    ) -> None:
-        """Abstracts the structure of a dataset by grouping together components.
-
-        For example, with an U{OAK-D<https://docs.luxonis.com/projects/hardware
-        /en/latest/pages/BW1098OAK/>}, you can have a source with 4 image
-        components: rgb (color), left (mono), right (mono), and depth.
-
-        @type name: str
-        @param name: A recognizable name for the source.
-
-        @type components: Optional[List[LuxonisComponent]]
-        @param components: If not using the default configuration, a list of
-        L{LuxonisComponent} to group together in the source.
-
-        @type main_component: Optional[str]
-        @param main_component: The name of the component that should be
-            primarily visualized.
-        """
-
-        self.name = name
-        if components is None:
-            components = [
-                LuxonisComponent(name)
-            ]  # basic source includes a single color image
-
-        self.components = {component.name: component for component in components}
-        self.main_component = main_component or next(iter(self.components))
-
-
-class LuxonisDataset:
+class LuxonisDataset(BaseDataset):
     def __init__(
         self,
         dataset_name: Optional[str] = None,
         dataset_id: Optional[str] = None,
         team_id: Optional[str] = None,
         team_name: Optional[str] = None,
         bucket_type: BucketType = BucketType.INTERNAL,
@@ -129,14 +58,16 @@
 
         if dataset_name is None and dataset_id is None:
             raise ValueError(
                 "Must provide either dataset_name or dataset_id when initializing LuxonisDataset"
             )
 
         self.base_path = environ.LUXONISML_BASE_PATH
+        os.makedirs(self.base_path, exist_ok=True)
+
         credentials_cache_file = osp.join(self.base_path, "credentials.json")
         if osp.exists(credentials_cache_file):
             with open(credentials_cache_file) as file:
                 self.config = json.load(file)
         else:
             self.config = {}
 
@@ -157,64 +88,63 @@
             raise Exception("Must use a valid BucketType!")
         if not isinstance(self.bucket_storage, BucketStorage):
             raise Exception("Must use a valid BucketStorage!")
 
         if self.bucket_storage != BucketStorage.LOCAL and self.bucket is None:
             raise Exception("Must set LUXONISML_BUCKET environment variable!")
 
-        self.online = self.team_id != "offline"
-
         self.datasets_cache_file = osp.join(self.base_path, "datasets.json")
         if osp.exists(self.datasets_cache_file):
             with open(self.datasets_cache_file) as file:
                 self.datasets = json.load(file)
         else:
             self.datasets = {}
 
-        if self.online:
-            raise NotImplementedError()
-        else:
-            if self.dataset_name is None:
-                raise Exception("Must provide a dataset_name for offline mode")
-            if self.dataset_name in self.datasets:
-                self.dataset_doc = self.datasets[self.dataset_name]
+        if self.dataset_name is None:
+            raise Exception("Must provide a dataset_name for offline mode")
+        if self.dataset_name in self.datasets:
+            self.dataset_doc = self.datasets[self.dataset_name]
 
-            else:
-                self.source = LuxonisSource("default")
-                self.datasets[self.dataset_name] = {
-                    "source": self._source_to_document(self.source),
-                    "ldf_version": LDF_VERSION,
-                    "classes": {},
-                    "skeletons": {},
-                }
-                self._write_datasets()
+        else:
+            self.source = LuxonisSource("default")
+            self.datasets[self.dataset_name] = {
+                "source": self._source_to_document(self.source),
+                "ldf_version": LDF_VERSION,
+                "classes": {},
+                "skeletons": {},
+            }
+            self._write_datasets()
 
         self._init_path()
 
         if self.bucket_storage == BucketStorage.LOCAL:
             self.fs = LuxonisFileSystem(f"file://{self.path}")
         elif self.bucket_storage == BucketStorage.AZURE_BLOB:
             raise NotImplementedError
         else:
             self.tmp_dir = ".luxonis_tmp"
             self.fs = LuxonisFileSystem(self.path)
 
         self.logger = logging.getLogger(__name__)
 
+    @property
+    def identifier(self) -> str:
+        if self.dataset_name is not None:
+            return self.dataset_name
+        assert self.dataset_id is not None
+        return self.dataset_id
+
     def __len__(self) -> int:
         """Returns the number of instances in the dataset."""
 
-        if self.online:
-            raise NotImplementedError
+        df = self._load_df_offline()
+        if df is not None:
+            return len(set(df["instance_id"]))
         else:
-            df = self._load_df_offline()
-            if df is not None:
-                return len(set(df["instance_id"]))
-            else:
-                return 0
+            return 0
 
     def _write_datasets(self) -> None:
         with open(self.datasets_cache_file, "w") as file:
             json.dump(self.datasets, file, indent=4)
 
     def _component_to_document(self, component: LuxonisComponent) -> Dict:
         return {
@@ -364,53 +294,45 @@
     def update_source(self, source: LuxonisSource) -> None:
         """Updates underlying source of the dataset with a new LuxonisSource.
 
         @type source: L{LuxonisSource}
         @param source: The new L{LuxonisSource} to replace the old one.
         """
 
-        if self.online:
-            raise NotImplementedError()
-        else:
-            self.datasets[self.dataset_name]["source"] = self._source_to_document(
-                source
-            )
-            self._write_datasets()
-            self.source = source
+        self.datasets[self.dataset_name]["source"] = self._source_to_document(source)
+        self._write_datasets()
+        self.source = source
 
     def set_classes(self, classes: List[str], task: Optional[str] = None) -> None:
         """Sets the names of classes for the dataset. This can be across all CV tasks or
         certain tasks.
 
         @type classes: List[str]
         @param classes: List of class names to set.
         @type task: Optional[str]
         @param task: Optionally specify the LabelType where these classes apply.
         """
 
-        if self.online:
-            raise NotImplementedError()
+        if task is not None:
+            if task not in LABEL_TYPES:
+                raise Exception(f"Task {task} is not a supported task")
+            self.datasets[self.dataset_name]["classes"][task] = classes
         else:
-            if task is not None:
-                if task not in LABEL_TYPES:
-                    raise Exception(f"Task {task} is not a supported task")
+            for task in LABEL_TYPES:
                 self.datasets[self.dataset_name]["classes"][task] = classes
-            else:
-                for task in LABEL_TYPES:
-                    self.datasets[self.dataset_name]["classes"][task] = classes
-            self._write_datasets()
+        self._write_datasets()
 
-            if self.bucket_storage != BucketStorage.LOCAL:
-                classes_json = self.datasets[self.dataset_name]["classes"]
-                self._make_temp_dir()
-                local_file = osp.join(self.tmp_dir, "classes.json")
-                with open(local_file, "w") as file:
-                    json.dump(classes_json, file, indent=4)
-                self.fs.put_file(local_file, "metadata/classes.json")
-                self._remove_temp_dir()
+        if self.bucket_storage != BucketStorage.LOCAL:
+            classes_json = self.datasets[self.dataset_name]["classes"]
+            self._make_temp_dir()
+            local_file = osp.join(self.tmp_dir, "classes.json")
+            with open(local_file, "w") as file:
+                json.dump(classes_json, file, indent=4)
+            self.fs.put_file(local_file, "metadata/classes.json")
+            self._remove_temp_dir()
 
     # TODO: method to auto-set classes per-task using pandas
 
     def set_skeletons(self, skeletons: Dict[str, Dict]) -> None:
         """Sets the semantic structure of keypoint skeletons for the classes that use
         keypoints.
 
@@ -426,95 +348,83 @@
                     "person": {
                         "labels": ["right hand", "right shoulder", ...]
                         "edges" [[0, 1], [4, 5], ...]
                     }
                 }
         """
 
-        if self.online:
-            raise NotImplementedError()
-        else:
-            self.datasets[self.dataset_name]["skeletons"] = skeletons
-            self._write_datasets()
+        self.datasets[self.dataset_name]["skeletons"] = skeletons
+        self._write_datasets()
 
     def sync_from_cloud(self) -> None:
         """Downloads data from a remote cloud bucket."""
 
         if self.bucket_storage == BucketStorage.LOCAL:
             self.logger.warning("This is a local dataset! Cannot sync")
         else:
             if not hasattr(self, "is_synced") or not self.is_synced:
-                local_dir = osp.join(
-                    self.base_path, "data", self.team_id, "datasets", self.dataset_name
-                )
+                local_dir = osp.join(self.base_path, "data", self.team_id, "datasets")
                 if not osp.exists(local_dir):
                     os.makedirs(local_dir, exist_ok=True)
 
-                protocol = self.bucket_storage.value
-                bucket = self.bucket
-                fs_path = f"{protocol}://{bucket}"
-                remote_dir = fs_path.split(fs_path)[1]
-                self.fs.get_dir(remote_dir=remote_dir, local_dir=local_dir)
+                self.fs.get_dir(remote_paths="", local_dir=local_dir)
 
                 self.is_synced = True
 
-    def get_classes(self, sync_mode: bool = False) -> Tuple[List[str], Dict]:
+    def get_classes(
+        self, sync_mode: bool = False
+    ) -> Tuple[List[str], Dict[str, List[str]]]:
         """Gets overall classes in the dataset and classes according to computer vision
         task.
 
         @type sync_mode: bool
         @param sync_mode: If C{True}, reads classes from remote storage. If C{False},
             classes are read locally.
-        @rtype: Tuple[List[str], Dict]
+        @rtype: Tuple[List[str], Dict[str, List[str]]
         @return: A combined list of classes for all tasks and a dictionary mapping tasks
             to the classes used in each task.
         """
 
-        if self.online:
-            raise NotImplementedError()
-        else:
-            classes = set()
-            classes_by_task = {}
-            if sync_mode:
-                local_file = osp.join(self.metadata_path, "classes.json")
-                self.fs.get_file("metadata/classes.json", local_file)
-                with open(local_file) as file:
-                    classes_json = json.load(file)
-            else:
-                classes_json = self.datasets[self.dataset_name]["classes"]
-            for task in classes_json:
-                task_classes = classes_json[task]
-                if len(task_classes):
-                    classes_by_task[task] = task_classes
-                    for cls in task_classes:
-                        classes.add(cls)
-            classes = list(classes)
-            classes.sort()
+        classes = set()
+        classes_by_task = {}
+        if sync_mode:
+            local_file = osp.join(self.metadata_path, "classes.json")
+            self.fs.get_file("metadata/classes.json", local_file)
+            with open(local_file) as file:
+                classes_json = json.load(file)
+        else:
+            classes_json = self.datasets[self.dataset_name]["classes"]
+        for task in classes_json:
+            task_classes = classes_json[task]
+            if len(task_classes):
+                classes_by_task[task] = task_classes
+                for cls in task_classes:
+                    classes.add(cls)
+        classes = list(classes)
+        classes.sort()
 
-            return classes, classes_by_task
+        return classes, classes_by_task
 
     def get_skeletons(self) -> Dict[str, Dict]:
         """Returns the dictionary defining the semantic skeleton for each class using
-        keypoints."""
+        keypoints.
 
-        if self.online:
-            raise NotImplementedError()
-        else:
-            return self.datasets[self.dataset_name]["skeletons"]
+        @rtype: Dict[str, Dict]
+        @return: A dictionary mapping classes to their skeleton definitions.
+        """
+
+        return self.datasets[self.dataset_name]["skeletons"]
 
     def delete_dataset(self) -> None:
         """Deletes all local files belonging to the dataset."""
 
-        if self.online:
-            raise NotImplementedError()
-        else:
-            del self.datasets[self.dataset_name]
-            self._write_datasets()
-            if self.bucket_storage == BucketStorage.LOCAL:
-                shutil.rmtree(self.path)
+        del self.datasets[self.dataset_name]
+        self._write_datasets()
+        if self.bucket_storage == BucketStorage.LOCAL:
+            shutil.rmtree(self.path)
 
     def add(
         self,
         generator: DatasetGeneratorFunction,
         batch_size: int = 1000000,
     ) -> None:
         """Write annotations to parquet files.
@@ -560,14 +470,24 @@
                     local_paths=paths, remote_dir="media", uuid_dict=uuid_dict
                 )
                 self._end_time()
 
             array_paths = list(
                 set([data["value"] for data in batch_data if data["type"] == "array"])
             )
+            progress = rich.progress.Progress(
+                rich.progress.TextColumn("[progress.description]{task.description}"),
+                rich.progress.BarColumn(),
+                rich.progress.TaskProgressColumn(),
+                rich.progress.MofNCompleteColumn(),
+                rich.progress.TimeRemainingColumn(),
+            )
+            task = progress.add_task(
+                "[magenta]Processing data...", total=len(batch_data)
+            )
             if len(array_paths):
                 self.logger.info("Checking arrays...")
                 self._start_time()
                 data_utils.check_arrays(array_paths)
                 self._end_time()
                 self.logger.info("Generating array UUIDs...")
                 self._start_time()
@@ -582,26 +502,31 @@
                     mask_upload_dict = self.fs.put_dir(
                         local_paths=array_paths,
                         remote_dir="arrays",
                         uuid_dict=array_uuid_dict,
                     )
                     self._end_time()
                 self.logger.info("Finalizing paths...")
-                for data in tqdm(batch_data):
+                progress.start()
+                for data in batch_data:
                     if data["type"] == "array":
                         if self.bucket_storage != BucketStorage.LOCAL:
                             remote_path = mask_upload_dict[data["value"]]
                             remote_path = f"{self.fs.protocol}://{osp.join(self.fs.path, remote_path)}"
                             data["value"] = remote_path
                         else:
                             data["value"] = osp.abspath(data["value"])
+                        progress.update(task, advance=1)
+                progress.stop()
 
             self.logger.info("Saving annotations...")
             self._start_time()
-            for data in tqdm(batch_data):
+            progress.reset(task)
+            progress.start()
+            for data in batch_data:
                 filepath = data["file"]
                 file = osp.basename(filepath)
                 instance_id = uuid_dict[filepath]
                 matched_id = self._try_instance_id(file, index)
                 if matched_id is not None:
                     if matched_id != instance_id:
                         # TODO: not sure if this should be an exception or how we should really handle it
@@ -625,50 +550,49 @@
                 if isinstance(data["value"], (list, tuple)):
                     data["value"] = json.dumps(data["value"])  # convert lists to string
                 else:
                     data["value"] = str(data["value"])
                 data["created_at"] = datetime.utcnow()
 
                 self.pfm.write(data)
+                progress.update(task, advance=1)
+            progress.stop()
             self._end_time()
 
-        if self.online:
-            raise NotImplementedError()
+        if self.bucket_storage == BucketStorage.LOCAL:
+            self.pfm = ParquetFileManager(self.annotations_path)
         else:
-            if self.bucket_storage == BucketStorage.LOCAL:
-                self.pfm = ParquetFileManager(self.annotations_path)
-            else:
-                self._make_temp_dir()
-                annotations_dir = osp.join(self.tmp_dir, "annotations")
-                os.makedirs(annotations_dir, exist_ok=True)
-                self.pfm = ParquetFileManager(annotations_dir)
+            self._make_temp_dir()
+            annotations_dir = osp.join(self.tmp_dir, "annotations")
+            os.makedirs(annotations_dir, exist_ok=True)
+            self.pfm = ParquetFileManager(annotations_dir)
 
-            index = self._get_file_index()
-            new_index = {"instance_id": [], "file": [], "original_filepath": []}
+        index = self._get_file_index()
+        new_index = {"instance_id": [], "file": [], "original_filepath": []}
 
-            batch_data = []
+        batch_data = []
 
-            for i, data in enumerate(generator()):
-                batch_data.append(data)
-                if (i + 1) % batch_size == 0:
-                    _add_process_batch(batch_data)
-                    batch_data = []
+        for i, data in enumerate(generator()):
+            batch_data.append(data)
+            if (i + 1) % batch_size == 0:
+                _add_process_batch(batch_data)
+                batch_data = []
 
-            _add_process_batch(batch_data)
+        _add_process_batch(batch_data)
 
-            self.pfm.close()
+        self.pfm.close()
 
-            if self.bucket_storage == BucketStorage.LOCAL:
-                self._write_index(index, new_index)
-            else:
-                file_index_path = osp.join(".luxonis_tmp", "file_index.parquet")
-                self._write_index(index, new_index, override_path=file_index_path)
-                self.fs.put_dir(annotations_dir, "annotations")
-                self.fs.put_file(file_index_path, "metadata/file_index.parquet")
-                self._remove_temp_dir()
+        if self.bucket_storage == BucketStorage.LOCAL:
+            self._write_index(index, new_index)
+        else:
+            file_index_path = osp.join(".luxonis_tmp", "file_index.parquet")
+            self._write_index(index, new_index, override_path=file_index_path)
+            self.fs.put_dir(Path(annotations_dir), "annotations")
+            self.fs.put_file(file_index_path, "metadata/file_index.parquet")
+            self._remove_temp_dir()
 
     def make_splits(
         self,
         ratios: Tuple[float, float, float] = (0.8, 0.1, 0.1),
         definitions: Optional[Dict] = None,
     ) -> None:
         """Saves a splits json file that specified the train/val/test split. For use in
@@ -687,94 +611,96 @@
                     "train": ["/path/to/cat.jpg", "/path/to/dog.jpg"],
                     "val": [...],
                     "test": [...]
                 }
 
             Only overrides splits that are present in the dictionary.
         """
-        if self.online:
-            raise NotImplementedError()
-        else:
-            new_splits = {"train": {}, "val": {}, "test": {}}
-            splits_to_update = []
 
-            if definitions is None:  # random split
-                if self.bucket_storage != BucketStorage.LOCAL:
-                    self._make_temp_dir()
-                    self.fs.get_dir(
-                        "annotations", osp.join(self.tmp_dir, "annotations")
-                    )
+        new_splits = {"train": {}, "val": {}, "test": {}}
+        splits_to_update = []
 
-                df = self._load_df_offline()
-                ids = list(set(df["instance_id"]))
-                np.random.shuffle(ids)
-                N = len(ids)
-                b1 = round(N * ratios[0])
-                b2 = round(N * ratios[0]) + round(N * ratios[1])
-                new_splits["train"] = ids[:b1]
-                new_splits["val"] = ids[b1:b2]
-                new_splits["test"] = ids[b2:]
-                splits_to_update = ["train", "val", "test"]
-            else:  # provided split
-                index = self._get_file_index()
-                if index is None:
-                    raise Exception("File index not found")
-                for split in "train", "val", "test":
-                    if split not in definitions:
-                        continue
-                    splits_to_update.append(split)
-                    files = definitions[split]
-                    if not isinstance(files, list):
-                        raise Exception("Must provide splits as a list of str")
-                    files = [osp.basename(file) for file in files]
-                    ids = [self._try_instance_id(file, index) for file in files]
-                    new_splits[split] = ids
-
-            if self.bucket_storage == BucketStorage.LOCAL:
-                splits_path = os.path.join(self.metadata_path, "splits.json")
-                if os.path.exists(splits_path):
-                    with open(splits_path, "r") as file:
-                        splits = json.load(file)
-                    for split in splits_to_update:
-                        splits[split] = new_splits[split]
-                else:
-                    splits = new_splits
-                with open(os.path.join(self.metadata_path, "splits.json"), "w") as file:
-                    json.dump(splits, file, indent=4)
+        if definitions is None:  # random split
+            if self.bucket_storage != BucketStorage.LOCAL:
+                self._make_temp_dir()
+                self.fs.get_dir("annotations", osp.join(self.tmp_dir, "annotations"))
+
+            df = self._load_df_offline()
+            ids = list(set(df["instance_id"]))
+            np.random.shuffle(ids)
+            N = len(ids)
+            b1 = round(N * ratios[0])
+            b2 = round(N * ratios[0]) + round(N * ratios[1])
+            new_splits["train"] = ids[:b1]
+            new_splits["val"] = ids[b1:b2]
+            new_splits["test"] = ids[b2:]
+            splits_to_update = ["train", "val", "test"]
+        else:  # provided split
+            index = self._get_file_index()
+            if index is None:
+                raise Exception("File index not found")
+            for split in "train", "val", "test":
+                if split not in definitions:
+                    continue
+                splits_to_update.append(split)
+                files = definitions[split]
+                if not isinstance(files, list):
+                    raise Exception("Must provide splits as a list of str")
+                files = [osp.basename(file) for file in files]
+                ids = [self._try_instance_id(file, index) for file in files]
+                new_splits[split] = ids
+
+        if self.bucket_storage == BucketStorage.LOCAL:
+            splits_path = os.path.join(self.metadata_path, "splits.json")
+            if os.path.exists(splits_path):
+                with open(splits_path, "r") as file:
+                    splits = json.load(file)
+                for split in splits_to_update:
+                    splits[split] = new_splits[split]
             else:
-                remote_path = "metadata/splits.json"
-                local_path = os.path.join(self.tmp_dir, "splits.json")
-                if self.fs.file_exists(remote_path):
-                    self.fs.get_file(remote_path, local_path)
-                    with open(splits_path, "r") as file:
-                        splits = json.load(file)
-                    for split in splits_to_update:
-                        splits[split] = new_splits[split]
-                else:
-                    splits = new_splits
-                with open(local_path, "w") as file:
-                    json.dump(splits, file, indent=4)
-                self.fs.put_file(local_path, "metadata/splits.json")
-                self._remove_temp_dir()
+                splits = new_splits
+            with open(os.path.join(self.metadata_path, "splits.json"), "w") as file:
+                json.dump(splits, file, indent=4)
+        else:
+            remote_splits_path = "metadata/splits.json"
+            local_splits_path = os.path.join(self.tmp_dir, "splits.json")
+            if self.fs.exists(remote_splits_path):
+                self.fs.get_file(remote_splits_path, local_splits_path)
+                with open(local_splits_path, "r") as file:
+                    splits = json.load(file)
+                for split in splits_to_update:
+                    splits[split] = new_splits[split]
+            else:
+                splits = new_splits
+            with open(local_splits_path, "w") as file:
+                json.dump(splits, file, indent=4)
+            self.fs.put_file(local_splits_path, "metadata/splits.json")
+            self._remove_temp_dir()
 
     @staticmethod
     def exists(dataset_name: str) -> bool:
         """Checks whether a dataset exists.
 
         @warning: For offline mode only.
         @type dataset_name: str
         @param dataset_name: Name of the dataset
         @rtype: bool
         @return: Whether the dataset exists
         """
+        return dataset_name in LuxonisDataset.list_datasets()
+
+    @staticmethod
+    def list_datasets() -> Dict:
+        """Returns a dictionary of all datasets.
+
+        @rtype: Dict
+        @return: Dictionary of all datasets
+        """
         base_path = environ.LUXONISML_BASE_PATH
         datasets_cache_file = osp.join(base_path, "datasets.json")
         if osp.exists(datasets_cache_file):
             with open(datasets_cache_file) as file:
                 datasets = json.load(file)
         else:
             datasets = {}
 
-        if dataset_name in datasets:
-            return True
-        else:
-            return False
+        return datasets
```

### Comparing `luxonis-ml-0.0.1/luxonis_ml/data/loader.py` & `luxonis-ml-0.1.0/luxonis_ml/data/loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import pandas as pd
 import pycocotools.mask as mask_util
 from PIL import Image, ImageDraw
 
 from luxonis_ml.enums import LabelType
 
 from .augmentations import Augmentations
-from .dataset import LuxonisDataset
+from .datasets import LuxonisDataset
 from .utils.enums import BucketStorage
 
 Labels = Dict[LabelType, np.ndarray]
 """C{Labels} is a dictionary of a label type and its annotations as L{numpy
 arrays<np.ndarray>}."""
 
 LuxonisLoaderOutput = Tuple[np.ndarray, Labels]
@@ -82,14 +82,19 @@
         self.sync_mode = (
             self.dataset.bucket_storage != BucketStorage.LOCAL and not self.stream
         )
 
         if self.sync_mode:
             self.logger.info("Syncing from cloud...")
             self.dataset.sync_from_cloud()
+            classes_file = os.path.join(self.dataset.metadata_path, "classes.json")
+            with open(classes_file) as file:
+                synced_classes = json.load(file)
+            for task in synced_classes:
+                self.dataset.set_classes(classes=synced_classes[task], task=task)
 
         if self.dataset.bucket_storage == BucketStorage.LOCAL or not self.stream:
             self.file_index = self.dataset._get_file_index()
             if self.file_index is None:
                 raise Exception("Cannot find file index")
         else:
             raise NotImplementedError(
@@ -109,17 +114,14 @@
         }
         if len(list(self.nk.values())):
             self.max_nk = max(list(self.nk.values()))
         else:
             self.max_nk = 0
         self.augmentations = augmentations
 
-        if self.dataset.online:
-            raise NotImplementedError
-
         if self.view in ["train", "val", "test"]:
             splits_path = os.path.join(dataset.metadata_path, "splits.json")
             if not os.path.exists(splits_path):
                 raise Exception(
                     "Cannot find splits! Ensure you call dataset.make_splits()"
                 )
             with open(splits_path, "r") as file:
```

### Comparing `luxonis-ml-0.0.1/luxonis_ml/data/utils/constants.py` & `luxonis-ml-0.1.0/luxonis_ml/data/utils/constants.py`

 * *Files identical despite different names*

### Comparing `luxonis-ml-0.0.1/luxonis_ml/data/utils/data_utils.py` & `luxonis-ml-0.1.0/luxonis_ml/data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `luxonis-ml-0.0.1/luxonis_ml/data/utils/enums.py` & `luxonis-ml-0.1.0/luxonis_ml/data/utils/enums.py`

 * *Files identical despite different names*

### Comparing `luxonis-ml-0.0.1/luxonis_ml/data/utils/labelstudio.py` & `luxonis-ml-0.1.0/luxonis_ml/data/utils/labelstudio.py`

 * *Files identical despite different names*

### Comparing `luxonis-ml-0.0.1/luxonis_ml/data/utils/parquet.py` & `luxonis-ml-0.1.0/luxonis_ml/data/utils/parquet.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import io
 import os
 from typing import Dict, Tuple
 
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
 
@@ -22,48 +21,31 @@
             another file is created.
         """
 
         self.dir = directory
         self.files = os.listdir(self.dir)
         self.num_rows = num_rows
 
-        if len(self.files):
-            self.num = self._find_num()
-            self.current_file = self._get_current_parquet_file()
-        else:
-            self.num = 0
-            new_filename, self.current_file = self._generate_filename(self.num)
-            self.files = [new_filename]
+        self.num = self._find_num() if len(self.files) else 0
+        self.current_file = self._generate_filename(self.num)
 
         self._read()
 
-    def _get_current_parquet_file(self) -> str:
-        """Finds the best parquet file to edit based on the file size and most last
-        write time."""
-
-        path = self._generate_filename(self.num)[1]
-        current_size = os.path.getsize(path) / (1024 * 1024)
-        if current_size < self.file_size:
-            return path
-        else:
-            self.num += 1
-            return self._generate_filename(self.num)[1]
-
     def _find_num(self) -> int:
         nums = [
             int(os.path.splitext(file)[0])
             for file in self.files
             if os.path.splitext(file)[1] == ".parquet"
         ]
         return max(nums)
 
     def _generate_filename(self, num: int) -> Tuple[str, str]:
         filename = f"{str(num).zfill(10)}.parquet"
         path = os.path.join(self.dir, filename)
-        return filename, path
+        return path
 
     def _read(self) -> Dict:
         if os.path.exists(self.current_file):
             df = pd.read_parquet(self.current_file)
             self.data = df.to_dict()
             self.data = {k: list(v.values()) for k, v in self.data.items()}
             self.row_count = len(df)
@@ -71,43 +53,35 @@
             self.row_count = 0
             self.data = {}
 
     def _initialize_data(self, data: Dict) -> None:
         for key in data:
             self.data[key] = []
 
-    def _estimate_file_size(self, df: pd.DataFrame) -> float:
-        with io.BytesIO() as buffer:
-            df.to_parquet(buffer)
-            return buffer.tell() / (1024 * 1024)
-
     def write(self, add_data: Dict) -> None:
         """Writes a row to the current working parquet file.
 
         @type add_data: Dict
         @param add_data: A dictionary representing annotations, mapping annotation types
             to values.
         """
 
         if len(self.data) == 0:
             self._initialize_data(add_data)
         for key in add_data:
             if key not in self.data:
                 raise Exception(f"Key {key} Not Found")
             self.data[key].append(add_data[key])
-            self.row_count += 1
 
+        self.row_count += 1
         if self.row_count % self.num_rows == 0:
-            df = pd.DataFrame(self.data)
-            estimated_size = self._estimate_file_size(df)
-            if estimated_size > self.file_size:
-                self.close()
-                self.num += 1
-                self.current_file = self._generate_filename(self.num)[1]
-                self._read()
+            self.close()
+            self.num += 1
+            self.current_file = self._generate_filename(self.num)
+            self._read()
 
     def close(self) -> None:
         """Ensures all data is written to parquet."""
 
         df = pd.DataFrame(self.data)
         table = pa.Table.from_pandas(df)
         pq.write_table(table, self.current_file)
```

### Comparing `luxonis-ml-0.0.1/luxonis_ml/embeddings/__init__.py` & `luxonis-ml-0.1.0/luxonis_ml/embeddings/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,50 +3,42 @@
 with guard_missing_extra("embedd"):
     from .methods import (
         calculate_similarity_matrix,
         find_mismatches_centroids,
         find_mismatches_knn,
         find_representative_greedy,
         find_representative_kmedoids,
-        find_similar_qdrant,
+        find_similar,
         isolation_forest_OOD,
         leverage_OOD,
     )
     from .utils import (
         QdrantAPI,
         QdrantManager,
-        export_model_onnx,
+        VectorDBAPI,
+        WeaviateAPI,
         extend_output_onnx,
-        extend_output_onnx_overwrite,
         extract_embeddings,
-        extract_embeddings_onnx,
         generate_embeddings,
-        load_embeddings,
-        load_model,
         load_model_onnx,
-        load_model_resnet50_minuslastlayer,
-        save_embeddings,
+        save_model_onnx,
     )
 
 __all__ = [
-    "find_similar_qdrant",
+    "find_similar",
     "find_mismatches_centroids",
     "find_mismatches_knn",
     "isolation_forest_OOD",
     "leverage_OOD",
     "calculate_similarity_matrix",
     "find_representative_greedy",
     "find_representative_kmedoids",
-    "load_model_resnet50_minuslastlayer",
-    "load_model",
-    "export_model_onnx",
     "load_model_onnx",
+    "save_model_onnx",
     "extend_output_onnx",
-    "extend_output_onnx_overwrite",
     "QdrantManager",
     "QdrantAPI",
+    "WeaviateAPI",
+    "VectorDBAPI",
     "extract_embeddings",
-    "extract_embeddings_onnx",
-    "save_embeddings",
-    "load_embeddings",
     "generate_embeddings",
 ]
```

### Comparing `luxonis-ml-0.0.1/luxonis_ml/embeddings/methods/OOD.py` & `luxonis-ml-0.1.0/luxonis_ml/embeddings/methods/OOD.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,35 +19,40 @@
     - Expanding Datasets: Recognizing valuable data points that are distinct from the current distribution can be helpful
       when we're looking to diversify the dataset, especially in iterative learning scenarios.
 
 Dependencies:
     - numpy
     - scikit-learn
 """
+from typing import Optional, Union
 
 import numpy as np
 from sklearn.ensemble import IsolationForest
 
 
 def isolation_forest_OOD(
-    X, contamination="auto", n_jobs=-1, verbose=1, random_state=None
-):
+    X: np.array,
+    contamination: Union[float, str] = "auto",
+    n_jobs: int = -1,
+    verbose: int = 1,
+    random_state: Optional[int] = None,
+) -> np.array:
     """Out-of-distribution detection using Isolation Forests.
 
     @type X: np.array
     @param X: The embeddings to use.
-    @type contamination: float
+    @type contamination: Union[float, str]
     @param contamination: The contamination parameter for Isolation Forests. Default is
         'auto'.
     @type n_jobs: int
     @param n_jobs: The number of jobs to use. Default is -1, which means all available
         CPUs.
     @type verbose: int
     @param verbose: The verbosity level. Default is 1.
-    @type random_state: int
+    @type random_state: Optional[int]
     @param random_state: The random state to use. Default is None.
     @rtype: np.array
     @return: The indices of the embeddings that are in-distribution.
     """
     # Initialize the Isolation Forest model
     isolation_forest = IsolationForest(
         contamination=contamination,
@@ -64,15 +69,15 @@
 
     # Get the indices of the outliers (where the predicted label is -1)
     outlier_indices_forest = np.where(predicted_labels == -1)[0]
 
     return outlier_indices_forest
 
 
-def leverage_OOD(X, std_threshold=3):
+def leverage_OOD(X: np.array, std_threshold: int = 3) -> np.array:
     """Out-of-distribution detection using leverage and linear regression.
 
     @type X: np.array
     @param X: The embeddings to use.
     @type std_threshold: int
     @param std_threshold: The number of standard deviations to use for the leverage
         threshold. Default is 3.
```

### Comparing `luxonis-ml-0.0.1/luxonis_ml/embeddings/methods/__init__.py` & `luxonis-ml-0.1.0/luxonis_ml/embeddings/methods/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from .duplicate import find_similar_qdrant
+from .duplicate import find_similar
 from .mistakes import find_mismatches_centroids, find_mismatches_knn
 from .OOD import isolation_forest_OOD, leverage_OOD
 from .representative import (
     calculate_similarity_matrix,
     find_representative_greedy,
     find_representative_kmedoids,
 )
 
 __all__ = [
-    "find_similar_qdrant",
+    "find_similar",
     "find_mismatches_centroids",
     "find_mismatches_knn",
     "isolation_forest_OOD",
     "leverage_OOD",
     "calculate_similarity_matrix",
     "find_representative_greedy",
     "find_representative_kmedoids",
```

### Comparing `luxonis-ml-0.0.1/luxonis_ml/embeddings/methods/duplicate.py` & `luxonis-ml-0.1.0/luxonis_ml/embeddings/methods/duplicate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,94 +1,110 @@
-"""Near-duplicate Search with Qdrant.
+"""Near-duplicate Search with Qdrant and Weaviate.
 
-This module provides utilities to detect and remove near-duplicate data points
-within a given set of embeddings. The removal process uses Kernel Density
-Estimation (KDE) on embeddings cosine similarity for optimal split, making
-this approach particularly suited for embeddings in high dimensional spaces.
-
-Functionality Includes:
-    - Using Qdrant for efficient search and retrieval of embeddings.
-    - Applying Kernel Density Estimation (KDE) to detect similarity peaks.
-    - Visualizing KDE results with matplotlib.
-    - Dynamic selection of best candidates for removal based on KDE peaks.
+Overview:
+This module provides utilities to detect and remove near-duplicate data points within a given set of embeddings.
+It leverages vector databases (Qdrant or Weaviate) for efficient search and retrieval,
+and employs Kernel Density Estimation (KDE) for optimal split based on embeddings' cosine similarity.
+This approach is particularly well-suited for handling high-dimensional embeddings.
+
+Key Features:
+    - Vector Database Integration: Supports both Qdrant and Weaviate for flexible deployment options.
+    - KDE-Based Near-Duplicate Detection: Uses KDE to identify clusters of near-duplicates, ensuring accuracy in high-dimensional spaces.
+    - Visualization: Allows plotting KDE results using matplotlib for intuitive understanding.
+    - Dynamic KDE Peak Selection: Automatically determines the best candidates for removal based on KDE peaks, minimizing manual thresholding.
 
 Dependencies:
-    - Requires the KDEpy library for KDE.
-    - Utilizes Qdrant (an open-source vector database) for embedding storage and search.
+    - KDEpy
+    - Qdrant (optional, for Qdrant-specific features)
+    - Weaviate (optional, for Weaviate-specific features)
 
 Functions:
-    - search_qdrant: Search embeddings within Qdrant based on query vectors.
-    - _plot_kde: Utility function to plot a KDE distribution.
-    - kde_peaks: Determine peaks in a KDE distribution.
-    - find_similar_qdrant: Find the most similar embeddings to the given reference embeddings.
-
-Examples:
-    1. Initialize a Qdrant client and retrieve all embeddings from a specific collection:
+    - search_vectordb(vectordb_api, query_vector, property_name, top_k): Searches for similar embeddings within the specified vector database.
+    - _plot_kde(xs, s, density, maxima, minima): Plots a KDE distribution.
+    - kde_peaks(data, bandwidth="scott", plot=False): Identifies peaks in a KDE distribution.
+    - find_similar(reference_embeddings, vectordb_api, k=100, n=1000, method="first", k_method=None, kde_bw="scott", plot=False): Finds the most similar embeddings to the given reference embeddings.
 
+Examples (using Qdrant):
+    1. Initialize a Qdrant client and retrieve embeddings:
         from luxonis_ml.embeddings.utils.qdrant import QdrantAPI
-        qdrant_api = QdrantAPI(host="localhost", port=6333, collection_name="webscraped_real_all")
+        qdrant_api = QdrantAPI(host="localhost", port=6333)
+        qdrant_api.create_collection("images", ["image_path", "embedding"])
         id_X, X = qdrant_api.get_all_embeddings()
-        i = 111
-
-    2. Search for similar embeddings in Qdrant for a specific embedding:
-
-        ids, similarites, image_paths = search_qdrant(qdrant_api, X[i], "real", 1000)
-        vals = np.array(similarites)
-        k = len(np.where(vals > 0.961)[0])  # manually selected threshold
-        imgk = image_paths[:k]
-
-    3. Find similar embeddings by providing an instance ID:
-
-        ix, paths = find_similar_qdrant(id_X[i], qdrant_api, "real", 5, 100, "first")
 
-    4. Find similar embeddings using the KDE Peaks method:
+    2. Find similar embeddings using various methods:
+        # By instance ID:
+        ix, paths = find_similar_qdrant(id_X[i], qdrant_api, "image_path", 5, 100, "first")
 
-        ix, paths = find_similar_qdrant(X[i], qdrant_api, "real", 5, 100, "first", "kde_peaks", "silverman", plot=False)
+        # Using KDE Peaks method:
+        ix, paths = find_similar_qdrant(X[i], qdrant_api, "image_path", 5, 100, "first", "kde_peaks", "silverman", plot=False)
 
-    5. Calculate the average of multiple embeddings and then find similar embeddings:
-
-        dark_ix = np.array([10,123,333,405])
+        # Based on average of multiple embeddings:
+        dark_ix = np.array([10, 123, 333, 405])
         emb_dark = X[dark_ix]
-        remove_dark_ix, paths = find_similar_qdrant(emb_dark, qdrant_api, "real", 25, 5000, "average", "kde_basic", "scott", plot=True)
+        remove_dark_ix, paths = find_similar_qdrant(emb_dark, qdrant_api, "image_path", 25, 5000, "average", "kde_basic", "scott", plot=True)
+
+Additional Notes:
+    - For Weaviate-specific examples, refer to the provided code examples.
+    - The search_vectordb function can be used with either Qdrant or Weaviate, depending on the provided vectordb_api object.
+    - Adjust parameters like k, n, and kde_bw based on your dataset and requirements.
 """
 
+from typing import List, Tuple, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 from KDEpy import FFTKDE
-
-# Near-duplicate search
 from scipy.signal import argrelextrema
 
-# Qdrant
-
+from luxonis_ml.embeddings.utils.vectordb import VectorDBAPI
 
-def search_qdrant(qdrant_api, query_vector, data_name, limit=5000):
-    """Search embeddings in Qdrant."""
-    hits = qdrant_api.search_embeddings_by_imagepath(query_vector, data_name, top=limit)
 
-    ix = [h.id for h in hits]
-    vals = [h.score for h in hits]
-    res = [h.payload["image_path"] for h in hits]
-
-    return ix, vals, res
-
-
-def _plot_kde(xs, s, density, maxima, minima):
-    """Plot a KDE distribution."""
+def _plot_kde(
+    xs: np.ndarray,
+    s: np.ndarray,
+    density: np.ndarray,
+    maxima: np.ndarray,
+    minima: np.ndarray,
+) -> None:
+    """Plot a KDE distribution.
+
+    @type xs: np.ndarray
+    @param xs: The x-axis values.
+    @type s: np.ndarray
+    @param s: The y-axis values.
+    @type density: np.ndarray
+    @param density: The density values.
+    @type maxima: np.ndarray
+    @param maxima: The indices of the local maxima.
+    @type minima: np.ndarray
+    @param minima: The indices of the local minima.
+    """
     plt.plot(xs, density, label="KDE")
     plt.plot(xs[maxima], s[maxima], "ro", label="local maxima")
     plt.plot(xs[minima], s[minima], "bo", label="local minima")
     plt.plot(xs[np.argmax(s)], np.max(s), "go", label="global maxima")
     plt.legend()
     plt.show()
 
 
-def kde_peaks(data, bandwidth="scott", plot=False):
-    """Find peaks in a KDE distribution using scipy's argrelextrema function."""
+def kde_peaks(
+    data: np.ndarray, bandwidth: Union[str, float] = "scott", plot: bool = False
+) -> Tuple[np.ndarray, np.ndarray, int, float]:
+    """Find peaks in a KDE distribution using scipy's argrelextrema function.
+
+    @type data: np.ndarray
+    @param data: The data to fit the KDE.
+    @type bandwidth: Union[str, float]
+    @param bandwidth: The bandwidth to use for the KDE. Default is 'scott'.
+    @type plot: bool
+    @param plot: Whether to plot the KDE.
+    @rtype: Tuple[np.ndarray, np.ndarray, int, float]
+    @return: The indices of the KDE maxima, the indices of the KDE minima, the index of
+        the global maxima, and the standard deviation of the data.
+    """
     # fit density
     kde = FFTKDE(kernel="gaussian", bw=bandwidth)
     xs = np.linspace(np.min(data) - 0.01, np.max(data) + 0.01, 1000)
     density = kde.fit(data).evaluate(xs)
 
     # find local maxima
     s = np.array(density)
@@ -104,44 +120,39 @@
     # plot
     if plot:
         _plot_kde(xs, s, density, maxima, minima)
 
     return xs[maxima], xs[minima], global_max_ix, std
 
 
-def find_similar_qdrant(
-    reference_embeddings,
-    qdrant_api,
-    dataset,
-    k=100,
-    n=1000,
-    method="first",
-    k_method=None,
-    kde_bw="scott",
-    plot=False,
-):
+def find_similar(
+    reference_embeddings: Union[str, List[str], List[List[float]], np.ndarray],
+    vectordb_api: VectorDBAPI,
+    k: int = 100,
+    n: int = 1000,
+    method: str = "first",
+    k_method: Union[str, None] = None,
+    kde_bw: Union[str, float] = "scott",
+    plot: bool = False,
+) -> np.ndarray:
     """Find the most similar embeddings to the reference embeddings.
 
-    @type reference_embeddings: Union[np.array, list]
+    @type reference_embeddings: Union[str, List[str], List[List[float]], np.ndarray]
     @param reference_embeddings: The embeddings to compare against. Or a list of of
-        embedding instance_ids that reside in Qdrant.
-    @type qdrant_api: QdrantAPI
-    @param qdrant_api: The Qdrant client API instance to use for searches.
-    @type dataset: str
-    @param dataset: The dataset to use. (It actually filters on the image_path field, so
-        it can be any string. It can be helpful if you have different datasets in
-        subfolders for the same collection, like 'real/img1.jpg' and 'synth/img1.jpg'.)
+        embedding instance_ids that reside in VectorDB.
+    @type vectordb_api: VectorDBAPI
+    @param vectordb_api: The VectorDBAPI instance to use.
     @type k: int
     @param k: The number of embeddings to return. Default is 100.
     @type n: int
     @param n: The number of embeddings to compare against. Default is 1000. (This is the
-        number of embeddings that are returned by the Qdrant search. It matters for the
-        KDE, as it can be slow for large n. Your choice of n depends on the amount of
-        duplicates in your dataset, the more duplicates, the larger n should be. If you
-        have 2-10 duplicates per image, n=100 should be ok. If you have 50-300
+        number of embeddings that are returned by the VectorDB search. It matters for
+        the KDE, as it can be slow for large n. Your choice of n depends on the amount
+        of duplicates in your dataset, the more duplicates, the larger n should be. If
+        you have 2-10 duplicates per image, n=100 should be ok. If you have 50-300
         duplicates per image, n=1000 should work good enough.
     @type method: str
     @param method: The method to use to find the most similar embeddings. If 'first' use
         the first of the reference embeddings. If 'average', use the average of the
         reference embeddings.
     @type k_method: str
     @param k_method: The method to select the best k. If None, use k as is. If
@@ -150,39 +161,46 @@
     @type kde_bw: Union[str, float]
     @param kde_bw: The bandwidth to use for the KDE. Default is 'scott'.
     @type plot: bool
     @param plot: Whether to plot the KDE.
     @rtype: np.array
     @return: The instance_ids of the most similar embeddings.
     """
+
     # Get the reference embeddings
-    # check if reference_embeddings is a list of instance_ids
-    if isinstance(reference_embeddings, str):
+    if isinstance(
+        reference_embeddings, str
+    ):  # if it is a single instance_id: string uuid
         reference_embeddings = [reference_embeddings]
-    if isinstance(reference_embeddings[0], str):
-        reference_embeddings = qdrant_api.get_embeddings_from_ids(reference_embeddings)
+    if isinstance(
+        reference_embeddings[0], str
+    ):  # if it is a list of instance_ids: list of strings
+        reference_embeddings = vectordb_api.retrieve_embeddings_by_ids(
+            reference_embeddings
+        )
 
     # Select the reference embedding
     if method == "first":
-        if isinstance(reference_embeddings, list):
+        if isinstance(
+            reference_embeddings, list
+        ):  # if it is a list of embeddings: list of lists of floats
             reference_embeddings = np.array(reference_embeddings)
         if len(reference_embeddings.shape) > 1:
             reference_embeddings = reference_embeddings[0]
     elif method == "average":
         # Calculate the average of the reference embeddings
         avg_embedding = np.mean(reference_embeddings, axis=0)
         reference_embeddings = avg_embedding
     else:
         raise ValueError(f"Unknown method: {method}")
 
-    # Search for similar embeddings in Qdrant
-    ix, vals, res = search_qdrant(
-        qdrant_api, reference_embeddings, data_name=dataset, limit=n
+    ix, similarities = vectordb_api.search_similar_embeddings(
+        reference_embeddings, top_k=n
     )
-    ix, similarities, res = np.array(ix), np.array(vals), np.array(res)
+    ix, similarities = np.array(ix), np.array(similarities)
 
     # Select the best k embeddings
     if k_method is None:
         best_embeddings_ix = np.argsort(similarities)[-k:]
 
     elif k_method == "kde_basic":
         _, new_min, _, _ = kde_peaks(similarities, bandwidth=kde_bw, plot=plot)
@@ -230,8 +248,8 @@
 
         # select the best k embeddings
         best_embeddings_ix = np.argsort(similarities)[-k:]
 
     else:
         raise ValueError(f"Unknown k_method: {k_method}")
 
-    return ix[best_embeddings_ix], res[best_embeddings_ix]
+    return ix[best_embeddings_ix]
```

### Comparing `luxonis-ml-0.0.1/luxonis_ml/embeddings/methods/mistakes.py` & `luxonis-ml-0.1.0/luxonis_ml/embeddings/methods/mistakes.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,29 +21,31 @@
         >>> from mismatch_detection import find_mismatches_centroids, find_mismatches_knn
         >>> # Detect mismatches using centroids
         >>> mismatches, new_labels = find_mismatches_centroids(X_train, y_train)
         >>> # Detect mismatches using KNN
         >>> mismatches, new_labels = find_mismatches_knn(X_train, y_train)
 """
 
+from typing import Tuple
+
 import numpy as np
 import scipy.spatial.distance as distance
 from sklearn.neighbors import KNeighborsClassifier
 
 
-def find_mismatches_centroids(X, y):
+def find_mismatches_centroids(X: np.array, y: np.array) -> Tuple[np.array, np.array]:
     """Find mismatches in the dataset. A mismatch is defined as a sample that is closer
     to another centroid than to its own centroid.
 
     @type X: np.array
     @param X: The embeddings to use.
     @type y: np.array
     @param y: The targets to use.
-    @rtype: np.array
-    @return: The indices of the mismatches.
+    @rtype: Tuple[np.array, np.array]
+    @return: The indices of the mismatches and the new labels.
     """
     unique_labels = np.unique(y)
     # Create a mapping from string labels to integer indices
     label_to_index = {label: index for index, label in enumerate(unique_labels)}
 
     # calculate centroids of each class
     centroids = []
@@ -85,31 +87,33 @@
     mismatches = np.array(mismatches)
     predicted_labels = np.array(predicted_labels)
     new_labels = predicted_labels
 
     return mismatches, new_labels
 
 
-def find_mismatches_knn(X, y, n_neighbors=5):
+def find_mismatches_knn(
+    X: np.array, y: np.array, n_neighbors: int = 5
+) -> Tuple[np.array, np.array]:
     """
     Find mismatches in the dataset.
     Single Algorithm Filter (see Figure 1 in Brodley, Carla E., and Mark A. Friedl. "Identifying mislabeled training data.").
     Idea: if the vast majority of the data is correctly labeled and you do knn prediction, the minority of mislabeled data will be engulfed (corrected) by the correct neighbors.
 
     @type X: np.array
     @param X: The embeddings to use.
 
     @type y: np.array
     @param y: The targets to use.
 
     @type n_neighbors: int
     @param n_neighbors: The number of neighbors to use for KNN. Default is 5.
 
-    @rtype: np.array
-    @return: The indices of the mismatches.
+    @rtype: Tuple[np.array, np.array]
+    @return: The indices of the mismatches and the new labels.
     """
 
     # Step 1: Fit KNN on the train set with corrupted labels
     knn = KNeighborsClassifier(n_neighbors=n_neighbors)
     knn.fit(X, y)
 
     # Step 2: Predict labels on the train set using the trained KNN model
```

### Comparing `luxonis-ml-0.0.1/luxonis_ml/embeddings/methods/representative.py` & `luxonis-ml-0.1.0/luxonis_ml/embeddings/methods/representative.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,43 +30,49 @@
         # Assuming you have 'embeddings' as a numpy array of shape (num_images, embedding_dim)
         similarity_matrix = calculate_similarity_matrix(embeddings)
         desired_size = int(len(embeddings) * 0.1)
         selected_image_indices = find_representative_greedy(1-similarity_matrix, desired_size)
 
     2. K-Medoids:
 
-            # to get all embeddings from qdrant:
-            ids, embeddings = get_all_embeddings(qdrant_client, collection_name="mnist")
-            # Assuming you have 'embeddings' as a numpy array of shape (num_images, embedding_dim)
-            similarity_matrix = calculate_similarity_matrix(embeddings)
-            desired_size = int(len(embeddings) * 0.1)
-            selected_image_indices = find_representative_kmedoids(similarity_matrix, desired_size)
+        # to get all embeddings from qdrant:
+        ids, embeddings = get_all_embeddings(qdrant_client, collection_name="mnist")
+        # Assuming you have 'embeddings' as a numpy array of shape (num_images, embedding_dim)
+        similarity_matrix = calculate_similarity_matrix(embeddings)
+        desired_size = int(len(embeddings) * 0.1)
+        selected_image_indices = find_representative_kmedoids(similarity_matrix, desired_size)
 """
 
+from typing import List
+
 import numpy as np
 from kmedoids import KMedoids
 from sklearn.metrics.pairwise import cosine_similarity
 
+from luxonis_ml.embeddings.utils.vectordb import VectorDBAPI
 
-def calculate_similarity_matrix(embeddings):
+
+def calculate_similarity_matrix(embeddings: np.ndarray) -> np.ndarray:
     return cosine_similarity(embeddings)
 
 
-def find_representative_greedy(distance_matrix, desired_size=1000, seed=0):
+def find_representative_greedy(
+    distance_matrix: np.ndarray, desired_size: int = 1000, seed: int = 0
+) -> List[int]:
     """Find the most representative images using a greedy algorithm. Gready search of
     maximally unique embeddings.
 
     @type distance_matrix: np.array
     @param distance_matrix: The distance matrix to use.
     @type desired_size: int
     @param desired_size: The desired size of the representative set. Default is 1000.
     @type seed: int
     @param seed: The index of the seed image. Default is 0. Must be in the range [0,
         num_images-1].
-    @rtype: np.array
+    @rtype: List[int]
     @return: The indices of the representative images.
     """
     num_images = distance_matrix.shape[0]
     selected_images = set()
     selected_images.add(seed)  # If seed==0: start with the first image as a seed.
 
     while len(selected_images) < desired_size:
@@ -83,30 +89,32 @@
 
         if best_image is not None:
             selected_images.add(best_image)
 
     return list(selected_images)
 
 
-def find_representative_greedy_qdrant(qdrant_api, desired_size=1000, seed=None):
-    """Find the most representative embeddings using a greedy algorithm with Qdrant.
-
-    @note: Due to many Qdrant requests, this function is very slow. Use
-        get_all_embeddings() and find_representative_greedy() instead.
-    @type qdrant_api: QdrantAPI
-    @param qdrant_api: The Qdrant client instance to use for searches.
+def find_representative_greedy_vectordb(
+    vectordb_api: VectorDBAPI, desired_size: int = 1000, seed: int = None
+) -> List[int]:
+    """Find the most representative embeddings using a greedy algorithm with VectorDB.
+
+    @note: Due to many requests, this function is very slow. Use
+        vectordb_api.retrieve_all_embeddings() and find_representative_greedy() instead.
+    @type vectordb_api: VectorDBAPI
+    @param vectordb_api: The Vector database client instance to use for searches.
     @type desired_size: int
     @param desired_size: The desired size of the representative set. Default is 1000.
     @type seed: int
     @param seed: The ID of the seed embedding. Default is None, which means a random
         seed is chosen.
-    @rtype: list
+    @rtype: List[int]
     @return: The IDs of the representative embeddings.
     """
-    all_ids = qdrant_api.get_all_ids()
+    all_ids = vectordb_api.retrieve_all_ids()
 
     if seed is None:
         seed = np.random.choice(all_ids)
     elif seed > len(all_ids):
         raise ValueError(f"Seed must be in the range [0, {len(all_ids)-1}].")
 
     selected_embeddings = set()
@@ -115,15 +123,15 @@
     while len(selected_embeddings) < desired_size:
         max_similarity = -1
         best_embedding = None
 
         for embedding_id in all_ids:
             if embedding_id not in selected_embeddings:
                 # Get similarities of the current embedding with the already selected embeddings
-                _, scores = qdrant_api.get_similarities(
+                _, scores = vectordb_api.get_similarity_scores(
                     embedding_id, list(selected_embeddings)
                 )
 
                 # Calculate the minimum similarity to all previously selected embeddings
                 min_similarity = max(scores) if scores else -1
 
                 if 1 - min_similarity > max_similarity:
@@ -133,28 +141,31 @@
         if best_embedding is not None:
             selected_embeddings.add(best_embedding)
 
     return list(selected_embeddings)
 
 
 def find_representative_kmedoids(
-    similarity_matrix, desired_size=1000, max_iter=100, seed=None
-):
+    similarity_matrix: np.ndarray,
+    desired_size: int = 1000,
+    max_iter: int = 100,
+    seed: int = None,
+) -> List[int]:
     """Find the most representative images using k-medoids. K-medoids clustering of
     embeddings.
 
     @type similarity_matrix: np.array
     @param similarity_matrix: The similarity matrix to use.
     @type desired_size: int
     @param desired_size: The desired size of the representative set. Default is 1000.
     @type max_iter: int
     @param max_iter: The maximum number of iterations to use. Default is 100.
     @type seed: int
     @param seed: The random seed to use. Default is None.
-    @rtype: np.array
+    @rtype: list
     @return: The indices of the representative images.
     """
     num_images = similarity_matrix.shape[0]
     k = min(
         desired_size, num_images
     )  # Choose 'k' as the desired size or the number of images, whichever is smaller.
```

### Comparing `luxonis-ml-0.0.1/luxonis_ml/tracker/mlflow_plugins.py` & `luxonis-ml-0.1.0/luxonis_ml/tracker/mlflow_plugins.py`

 * *Files identical despite different names*

### Comparing `luxonis-ml-0.0.1/luxonis_ml/tracker/tracker.py` & `luxonis-ml-0.1.0/luxonis_ml/tracker/tracker.py`

 * *Files identical despite different names*

### Comparing `luxonis-ml-0.0.1/luxonis_ml/utils/config.py` & `luxonis-ml-0.1.0/luxonis_ml/utils/config.py`

 * *Files identical despite different names*

### Comparing `luxonis-ml-0.0.1/luxonis_ml/utils/environ.py` & `luxonis-ml-0.1.0/luxonis_ml/utils/environ.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,16 @@
     POSTGRES_DB: Optional[str] = None
 
     LUXONISML_BUCKET: Optional[str] = None
     LUXONISML_BASE_PATH: str = str(Path.home() / "luxonis_ml")
     LUXONISML_TEAM_ID: str = "offline"
     LUXONISML_TEAM_NAME: str = "offline"
 
+    GOOGLE_APPLICATION_CREDENTIALS: Optional[str] = None
+
     LOG_LEVEL: Literal["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"] = "INFO"
 
     @model_serializer(when_used="always", mode="plain", return_type=str)
     def _serialize_environ(self) -> str:
         return "[Content hidden ...]"
```

### Comparing `luxonis-ml-0.0.1/luxonis_ml/utils/filesystem.py` & `luxonis-ml-0.1.0/luxonis_ml/utils/filesystem.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,46 @@
 import os
+import os.path as osp
+import subprocess
+import sys
 import uuid
 from concurrent.futures import ThreadPoolExecutor
+from enum import Enum
+from importlib.util import find_spec
 from io import BytesIO
 from logging import getLogger
+from pathlib import Path, PurePosixPath
 from types import ModuleType
-from typing import Dict, Iterator, List, Optional, Tuple, Union
+from typing import Dict, Iterator, List, Optional, Sequence, Tuple, Union, cast
 
 import fsspec
 
 from .environ import environ
+from .registry import Registry
 
 logger = getLogger(__name__)
 
+PathType = Union[str, Path]
+
+PUT_FILE_REGISTRY = Registry(name="put_file")
+
+
+class FSType(Enum):
+    MLFLOW = "mlflow"
+    FSSPEC = "fsspec"
+
 
 class LuxonisFileSystem:
     def __init__(
         self,
         path: str,
         allow_active_mlflow_run: Optional[bool] = False,
         allow_local: Optional[bool] = True,
         cache_storage: Optional[str] = None,
+        put_file_plugin: Optional[str] = None,
     ):
         """Abstraction over remote and local sources.
 
         Helper class which abstracts uploading and downloading files from remote and
         local sources. Supports S3, MLflow, GCS, and local file systems.
 
         @type path: str
@@ -34,60 +51,83 @@
             run. Defaults to False.
         @type allow_local: Optional[bool]
         @param allow_local: Flag if operations are allowed on local file system.
             Defaults to True.
         @type cache_storage: Optional[str]
         @param cache_storage: Path to cache storage. No cache is used if set to None.
             Defaults to None.
+        @type put_file_plugin: Optional[str]
+        @param put_file_plugin: The name of a registered function under the
+            PUT_FILE_REGISTRY to override C{self.put_file}.
         """
         if path is None:
             raise ValueError("No path provided to LuxonisFileSystem.")
 
         self.cache_storage = cache_storage
 
-        self.protocol, self.path = _get_protocol_and_path(path)
+        self.protocol, _path = _get_protocol_and_path(path)
         supported_protocols = ["s3", "gcs", "file", "mlflow"]
         if self.protocol not in supported_protocols:
             raise ValueError(
                 f"Protocol `{self.protocol}` not supported. Choose from {supported_protocols}."
             )
 
+        _check_package_installed(self.protocol)
+
         self.allow_local = allow_local
         if self.protocol == "file" and not self.allow_local:
             raise ValueError("Local filesystem is not allowed.")
 
-        self.is_mlflow = False
-        self.is_fsspec = False
-
         if self.protocol == "mlflow":
-            self.is_mlflow = True
+            self.fs_type = FSType.MLFLOW
 
             self.allow_active_mlflow_run = allow_active_mlflow_run
             self.is_mlflow_active_run = False
-            if len(self.path):
+            if _path is not None:
                 (
                     self.experiment_id,
                     self.run_id,
                     self.artifact_path,
-                ) = self._split_mlflow_path(self.path)
-            elif len(self.path) == 0 and self.allow_active_mlflow_run:
+                ) = self._split_mlflow_path(_path)
+            elif _path is None and self.allow_active_mlflow_run:
                 self.is_mlflow_active_run = True
+                _path = ""
             else:
                 raise ValueError(
                     "Using active MLFlow run is not allowed. Specify full MLFlow path."
                 )
             self.tracking_uri = environ.MLFLOW_TRACKING_URI
 
             if self.tracking_uri is None:
                 raise KeyError(
                     "There is no 'MLFLOW_TRACKING_URI' in environment variables"
                 )
         else:
-            self.is_fsspec = True
+            self.fs_type = FSType.FSSPEC
             self.fs = self.init_fsspec_filesystem()
+        self.path = PurePosixPath(cast(str, _path))
+
+        if put_file_plugin:
+            self.put_file = PUT_FILE_REGISTRY.get(put_file_plugin)
+
+    @property
+    def is_mlflow(self) -> bool:
+        """Returns True if the filesystem is MLFlow.
+
+        @type: bool
+        """
+        return self.fs_type == FSType.MLFLOW
+
+    @property
+    def is_fsspec(self) -> bool:
+        """Returns True if the filesystem is fsspec.
+
+        @type: bool
+        """
+        return self.fs_type == FSType.FSSPEC
 
     @property
     def full_path(self) -> str:
         """Returns full remote path.
 
         @type: str
         """
@@ -121,223 +161,250 @@
             logger.warning("Ignoring cache storage for local filesystem.")
             return fs
 
         return fsspec.filesystem("filecache", fs=fs, cache_storage=self.cache_storage)
 
     def put_file(
         self,
-        local_path: str,
-        remote_path: str,
+        local_path: PathType,
+        remote_path: PathType,
         mlflow_instance: Optional[ModuleType] = None,
-    ) -> None:
+    ) -> str:
         """Copy a single file to remote storage.
 
-        @type local_path: str
+        @type local_path: PathType
         @param local_path: Path to local file
-        @type remote_path: str
+        @type remote_path: PathType
         @param remote_path: Relative path to remote file
         @type mlflow_instance: Optional[L{ModuleType}]
         @param mlflow_instance: MLFlow instance if uploading to active run. Defaults to
-            None.
+            C{None}.
+        @rtype: str
+        @return: The full remote path of the uploded file.
         """
+        local_path = str(local_path)
         if self.is_mlflow:
             # NOTE: remote_path not used in mlflow since it creates new folder each time
             if self.is_mlflow_active_run:
                 if mlflow_instance is not None:
                     mlflow_instance.log_artifact(local_path)
                 else:
                     raise KeyError("No active mlflow_instance provided.")
             else:
                 import mlflow
 
                 client = mlflow.MlflowClient(tracking_uri=self.tracking_uri)
                 client.log_artifact(run_id=self.run_id, local_path=local_path)
 
         elif self.is_fsspec:
-            self.fs.put_file(local_path, os.path.join(self.path, remote_path))
+            self.fs.put_file(local_path, str(self.path / remote_path))
+        return self.protocol + "://" + str(self.path / remote_path)
 
     def put_dir(
         self,
-        local_paths: Union[str, List[str]],
-        remote_dir: str,
+        local_paths: Union[PathType, Sequence[PathType]],
+        remote_dir: PathType,
         uuid_dict: Optional[Dict[str, str]] = None,
         mlflow_instance: Optional[ModuleType] = None,
     ) -> Optional[Dict[str, str]]:
         """Uploads files to remote storage.
 
-        @type local_paths: Union[str, List[str]]
+        @type local_paths: Union[PathType, Sequence[PathType]]
         @param local_paths: Either a string specifying a directory to walk the files or
-            a list of files which can be in different directories
-        @type remote_dir: str
+            a list of files which can be in different directories.
+        @type remote_dir: PathType
         @param remote_dir: Relative path to remote directory
         @type uuid_dict: Optional[Dict[str, str]]
         @param uuid_dict: Stores paths as keys and corresponding UUIDs as values to
             replace the file basename.
         @type mlflow_instance: Optional[L{ModuleType}]
         @param mlflow_instance: MLFlow instance if uploading to active run. Defaults to
             None.
         @rtype: Optional[Dict[str, str]]
         @return: When local_paths is a list, this maps local_paths to remote_paths
         """
         if self.is_mlflow:
             raise NotImplementedError
         elif self.is_fsspec:
-            if isinstance(local_paths, str) and os.path.isdir(local_paths):
+            if isinstance(local_paths, Path) and Path(local_paths).is_dir():
                 self.fs.put(
-                    local_paths, os.path.join(self.path, remote_dir), recursive=True
+                    str(local_paths),
+                    str(self.path / remote_dir),
+                    recursive=True,
                 )
-            else:
+            elif isinstance(local_paths, list):
                 upload_dict = {}
                 with ThreadPoolExecutor() as executor:
                     for local_path in local_paths:
-                        if uuid_dict:
+                        local_path = str(local_path)
+                        if uuid_dict is not None:
                             file_uuid = uuid_dict[local_path]
-                            ext = os.path.splitext(local_path)[1]
+                            ext = osp.splitext(local_path)[1]
                             basename = file_uuid + ext
                         else:
-                            basename = os.path.basename(local_path)
-                        remote_path = os.path.join(remote_dir, basename)
+                            basename = Path(local_path).name
+                        remote_path = str(PurePosixPath(remote_dir) / basename)
                         upload_dict[local_path] = remote_path
                         executor.submit(self.put_file, local_path, remote_path)
                 return upload_dict
 
     def put_bytes(
         self,
         file_bytes: bytes,
-        remote_path: str,
+        remote_path: PathType,
         mlflow_instance: Optional[ModuleType] = None,
     ) -> None:
         """Uploads a file to remote storage directly from file bytes.
 
         @type file_bytes: bytes
         @param file_bytes: the bytes for the file contents
-        @type remote_path: str
+        @type remote_path: PathType
         @param remote_path: Relative path to remote file
         @type mlflow_instance: Optional[L{ModuleType}]
         @param mlflow_instance: MLFlow instance if uploading to active run. Defaults to
             None.
         """
         if self.is_mlflow:
             raise NotImplementedError
         elif self.is_fsspec:
-            full_path = os.path.join(self.path, remote_path)
+            full_path = str(self.path / remote_path)
             with self.fs.open(full_path, "wb") as file:
-                file.write(file_bytes)
+                file.write(file_bytes)  # type: ignore
 
     def get_file(
         self,
-        remote_path: str,
-        local_path: str,
+        remote_path: PathType,
+        local_path: PathType,
         mlflow_instance: Optional[ModuleType] = None,
-    ) -> None:
+    ) -> Path:
         """Copy a single file from remote storage.
 
-        @type remote_path: str
+        @type remote_path: PathType
         @param remote_path: Relative path to remote file
-        @type local_path: str
+        @type local_path: PathType
         @param local_path: Path to local file
         @type mlflow_instance: Optional[L{ModuleType}]
         @param mlflow_instance: MLFlow instance if uploading to active run. Defaults to
-            None.
+            C{None}.
+        @rtype: Path
+        @return: Path to the downloaded file.
         """
 
         if self.is_mlflow:
             raise NotImplementedError
         elif self.is_fsspec:
             self.fs.download(
-                os.path.join(self.path, remote_path), local_path, recursive=False
+                str(self.path / remote_path),
+                str(local_path),
+                recursive=False,
             )
+        return Path(local_path) / Path(remote_path).name
 
-    def delete_file(self, remote_path: str) -> None:
+    def delete_file(self, remote_path: PathType) -> None:
         """Deletes a single file from remote storage.
 
-        @type remote_path: str
+        @type remote_path: PathType
         @param remote_path: Relative path to remote file
         """
         if self.is_fsspec:
-            full_remote_path = os.path.join(self.path, remote_path)
+            full_remote_path = str(self.path / remote_path)
             self.fs.rm(full_remote_path)
         else:
             raise NotImplementedError
 
-    def delete_files(self, remote_paths: List[str]) -> None:
+    def delete_files(self, remote_paths: List[PathType]) -> None:
         """Deletes multiple files from remote storage.
 
-        @type remote_paths: List[str]
+        @type remote_paths: List[PathType]
         @param remote_paths: Relative paths to remote files
         """
         if self.is_fsspec:
             full_remote_paths = [
-                os.path.join(self.path, remote_path) for remote_path in remote_paths
+                str(self.path / remote_path) for remote_path in remote_paths
             ]
             self.fs.rm(full_remote_paths)
         else:
             raise NotImplementedError
 
     def get_dir(
         self,
-        remote_dir: str,
-        local_dir: str,
+        remote_paths: Union[PathType, Sequence[PathType]],
+        local_dir: PathType,
         mlflow_instance: Optional[ModuleType] = None,
-    ) -> None:
+    ) -> Path:
         """Copies many files from remote storage to local storage.
 
-        @type remote_dir: str
-        @param remote_dir: Relative path to remote directory
-        @type local_dir: str
+        @type remote_paths: Union[PathType, Sequence[PathType]]
+        @param remote_paths: Either a string specifying a directory to walk the files or
+            a list of files which can be in different directories.
+        @type local_dir: PathType
         @param local_dir: Path to local directory
         @type mlflow_instance: Optional[L{ModuleType}]
         @param mlflow_instance: MLFlow instance if uploading to active run. Defaults to
-            None.
+            C{None}.
+        @rtype: Path
+        @return: Path to the downloaded directory.
         """
         if self.is_mlflow:
             raise NotImplementedError
         elif self.is_fsspec:
-            self.fs.download(
-                os.path.join(self.path, remote_dir), local_dir, recursive=True
-            )
+            if isinstance(remote_paths, Path) or isinstance(remote_paths, str):
+                self.fs.download(
+                    str(self.path / remote_paths),
+                    str(local_dir),
+                    recursive=True,
+                )
+                return Path(local_dir) / Path(remote_paths).name
+
+            elif isinstance(remote_paths, list):
+                with ThreadPoolExecutor() as executor:
+                    for remote_path in remote_paths:
+                        local_path = str(local_dir / Path(Path(remote_path).name))
+                        executor.submit(self.get_file, remote_path, local_path)
+
+        return Path(local_dir)
 
-    def delete_dir(self, remote_dir: str) -> None:
+    def delete_dir(self, remote_dir: PathType) -> None:
         """Deletes a directory and all its contents from remote storage.
 
-        @type remote_dir: str
+        @type remote_dir: PathType
         @param remote_dir: Relative path to remote directory
         """
         if self.is_fsspec:
-            full_remote_dir = os.path.join(self.path, remote_dir)
+            full_remote_dir = str(self.path / remote_dir)
             self.fs.rm(full_remote_dir, recursive=True)
         else:
             raise NotImplementedError
 
-    def walk_dir(self, remote_dir: str) -> Iterator[str]:
-        """Recursively walks through the individual files in a remote directory.
+    def walk_dir(self, remote_dir: PathType, recursive: bool = True) -> Iterator[str]:
+        """Walks through the individual files in a remote directory.
 
-        @type remote_dir: str
+        @type remote_dir: PathType
         @param remote_dir: Relative path to remote directory
+        @type recursive: bool
+        @param recursive: If True, walks through the directory recursively.
         @rtype: Iterator[str]
         @return: Iterator over the paths.
         """
 
         if self.is_mlflow:
             raise NotImplementedError
         elif self.is_fsspec:
-            full_path = os.path.join(self.path, remote_dir)
-            for file in self.fs.glob(full_path + "/**", detail=True):
+            full_path = str(self.path / remote_dir)
+            for file in self.fs.glob(
+                full_path + f"/{'**' if recursive else '*'}", detail=True
+            ):
                 if self.fs.info(file)["type"] == "file":
-                    assert isinstance(file, str)
+                    file = str(file)
+                    yield str(PurePosixPath(file).relative_to(self.path))
 
-                    file_without_path = file.replace(self.path, "")
-                    if file_without_path.startswith("/"):
-                        file_without_path = file_without_path[1:]
-                    yield os.path.relpath(file, self.path)
-
-    def read_to_byte_buffer(self, remote_path: Optional[str] = None) -> BytesIO:
+    def read_to_byte_buffer(self, remote_path: Optional[PathType] = None) -> BytesIO:
         """Reads a file into a byte buffer.
 
-        @type remote_path: Optional[str]
+        @type remote_path: Optional[PathType]
         @param remote_path: Relative path to remote file.
         @rtype: BytesIO
         @return: The byte buffer containing the file contents.
         """
 
         if self.is_mlflow:
             if self.is_mlflow_active_run:
@@ -346,147 +413,222 @@
                 )
             else:
                 if self.artifact_path is None:
                     raise ValueError("No relative artifact path specified.")
                 import mlflow
 
                 client = mlflow.MlflowClient(tracking_uri=self.tracking_uri)
+                if self.run_id is None:
+                    raise RuntimeError("`run_id` cannot be `None` when using `mlflow`")
                 download_path = client.download_artifacts(
                     run_id=self.run_id, path=self.artifact_path, dst_path="."
                 )
             with open(download_path, "rb") as f:
                 buffer = BytesIO(f.read())
             os.remove(download_path)  # remove local file
 
-        elif self.is_fsspec:
-            if remote_path:
-                download_path = os.path.join(self.path, remote_path)
+        else:
+            if remote_path is not None:
+                download_path = str(self.path / remote_path)
             else:
-                download_path = self.path
+                download_path = str(self.path)
             with self.fs.open(download_path, "rb") as f:
-                buffer = BytesIO(f.read())
+                buffer = BytesIO(cast(bytes, f.read()))
 
         return buffer
 
-    def get_file_uuid(self, path: str, local: bool = False) -> str:
+    def get_file_uuid(self, path: PathType, local: bool = False) -> str:
         """Reads a file and returns the (unique) UUID generated from file bytes.
 
-        @type path: str
+        @type path: PathType
         @param path: Relative path to remote file.
         @type local: bool
         @param local: Specifies a local path as opposed to a remote path.
         @rtype: str
         @return: The generated UUID.
         """
 
         if local:
             with open(path, "rb") as f:
-                file_contents = f.read()
+                file_contents = cast(bytes, f.read())
         else:
             if self.is_mlflow:
                 raise NotImplementedError
 
-            elif self.is_fsspec:
-                download_path = os.path.join(self.path, path)
+            else:
+                download_path = str(self.path / path)
                 with self.fs.open(download_path, "rb") as f:
-                    file_contents = f.read()
+                    file_contents = cast(bytes, f.read())
 
         file_hash_uuid = str(uuid.uuid5(uuid.NAMESPACE_URL, file_contents.hex()))
 
         return file_hash_uuid
 
-    def get_file_uuids(self, paths: List[str], local: bool = False) -> Dict[str, str]:
+    def get_file_uuids(
+        self, paths: List[PathType], local: bool = False
+    ) -> Dict[str, str]:
         """Computes the UUIDs for all files stored in the filesystem.
 
-        @type paths: List[str]
+        @type paths: List[PathType]
         @param paths: A list of relative remote paths if remote else local paths.
         @type local: bool
         @param local: Specifies local paths as opposed to remote paths.
         @rtype: Dict[str, str]
         @return: A dictionary mapping the paths to their UUIDs
         """
 
         result = {}
 
         if self.is_fsspec:
             with ThreadPoolExecutor() as executor:
                 for path in paths:
+                    path = str(path)
                     future = executor.submit(self.get_file_uuid, path, local)
                     result[path] = future.result()
 
         return result
 
-    def _split_mlflow_path(self, path: str) -> List[Optional[str]]:
+    def _split_mlflow_path(self, path: PathType) -> List[Optional[str]]:
         """Splits mlflow path into 3 parts."""
-        parts = path.split("/")
+        path = Path(path)
+        parts: List[Optional[str]] = list(path.parts)
         if len(parts) < 3:
             while len(parts) < 3:
                 parts.append(None)
         elif len(parts) > 3:
-            parts[2] = "/".join(parts[2:])
+            parts[2] = "/".join(cast(List[str], parts[2:]))
             parts = parts[:3]
         return parts
 
-    def is_directory(self, remote_path: str) -> bool:
+    def is_directory(self, remote_path: PathType) -> bool:
         """Checks whether the given remote path is a directory.
 
-        @type remote_path: str
+        @type remote_path: PathType
         @param remote_path: Relative path to remote file.
         @rtype: bool
         @return: True if the path is a directory.
         """
 
-        full_path = os.path.join(self.path, remote_path)
+        full_path = str(self.path / remote_path)
         file_info = self.fs.info(full_path)
-        if file_info["type"] == "directory":
-            return True
-        else:
-            return False
+        return file_info["type"] == "directory"
 
-    def file_exists(self, remote_path: str) -> bool:
+    def exists(self, remote_path: PathType) -> bool:
         """Checks whether the given remote path exists.
 
-        @type remote_path: str
+        @type remote_path: PathType
         @param remote_path: Relative path to remote file.
         @rtype: bool
         @return: True if the path exists.
         """
-        full_path = os.path.join(self.path, remote_path)
+        full_path = str(self.path / remote_path)
         return self.fs.exists(full_path)
 
     @staticmethod
-    def split_full_path(path: str) -> Tuple[str, str]:
+    def split_full_path(path: PathType) -> Tuple[str, str]:
         """Splits the full path into protocol and absolute path.
 
-        @type path: str
+        @type path: PathType
         @param path: Full path
         @rtype: Tuple[str, str]
         @return: Tuple of protocol and absolute path.
         """
-        path = path.rstrip("/\\")
-        return os.path.split(path)
+        path = str(path).rstrip("/\\")
+        return osp.split(path)
 
     @staticmethod
     def get_protocol(path: str) -> str:
         """Extracts the detected protocol from a path.
 
         @type path: str
         @param path: Full path
         @rtype: str
         @return: Protocol of the path.
         """
         return _get_protocol_and_path(path)[0]
 
+    @staticmethod
+    def download(url: str, dest: Optional[PathType]) -> Path:
+        """Downloads file or directory from remote storage.
+
+        Intended for downloading a single remote object, elevating the need to create an
+        instance of L{LuxonisFileSystem}.
+
+        @type url: str
+        @param url: URL to the file or directory
+        @type dest: Optional[PathType]
+        @param dest: Destination directory. If unspecified, the current directory is
+            used.
+        @rtype: Path
+        @return: Path to the downloaded file or directory.
+        """
+
+        if LuxonisFileSystem.get_protocol(url) == "file":
+            return Path(url)
+
+        dest = Path(dest or ".")
+        absolute_path, remote_path = LuxonisFileSystem.split_full_path(url)
+        if dest.suffix:
+            local_path = dest
+        else:
+            local_path = dest / remote_path
+        fs = LuxonisFileSystem(absolute_path)
+
+        if fs.is_directory(remote_path):
+            fs.get_dir(remote_path, local_path)
+        else:
+            fs.get_file(remote_path, str(local_path))
+
+        return local_path
+
+    @staticmethod
+    def upload(local_path: PathType, url: str) -> None:
+        """Uploads file or directory to remote storage.
+
+        Intended for uploading a single local object, elevating the need to create an
+        instance of L{LuxonisFileSystem}.
+
+        @type local_path: PathType
+        @param local_path: Path to the local file or directory
+        @type url: str
+        @param url: URL to the remote file or directory
+        @rtype: str
+        @return: URL to the uploaded file or directory.
+        """
+
+        absolute_path, remote_path = LuxonisFileSystem.split_full_path(url)
+        fs = LuxonisFileSystem(absolute_path)
+        if Path(local_path).is_dir():
+            fs.put_dir(local_path, remote_path)
+        else:
+            fs.put_file(str(local_path), remote_path)
+
+
+def _check_package_installed(protocol: str) -> None:
+    def _pip_install(package: str, version: str) -> None:
+        logger.error(f"{package} is necessary for {protocol} protocol.")
+        logger.info(f"Installing {package}...")
+        subprocess.run(
+            [sys.executable, "-m", "pip", "install", f"{package}>={version}"]
+        )
+
+    if protocol in ["gs", "gcs"] and find_spec("gcsfs") is None:
+        _pip_install("gcsfs", "2023.1.0")
+    elif protocol == "s3" and find_spec("s3fs") is None:
+        _pip_install("s3fs", "2023.1.0")
+    elif protocol == "mlflow" and find_spec("mlflow") is None:
+        _pip_install("mlflow", "2.10.0")
+
 
-def _get_protocol_and_path(path: str) -> Tuple[str, str]:
+def _get_protocol_and_path(path: str) -> Tuple[str, Optional[str]]:
     """Gets the protocol and absolute path of a full path."""
 
     if "://" in path:
         protocol, path = path.split("://")
         if protocol == "gs":
             # ensure gs:// URLs are accepted as the gcs protocol
             protocol = "gcs"
     else:
         # assume that it is local path
         protocol = "file"
 
-    return protocol, path
+    return protocol, path if path else None
```

### Comparing `luxonis-ml-0.0.1/luxonis_ml/utils/logging.py` & `luxonis-ml-0.1.0/luxonis_ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `luxonis-ml-0.0.1/luxonis_ml/utils/registry.py` & `luxonis-ml-0.1.0/luxonis_ml/utils/registry.py`

 * *Files identical despite different names*

### Comparing `luxonis-ml-0.0.1/luxonis_ml.egg-info/PKG-INFO` & `luxonis-ml-0.1.0/luxonis_ml.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxonis-ml
-Version: 0.0.1
+Version: 0.1.0
 Summary: MLOps tools for training models for Luxonis devices
 Author-email: Luxonis <support@luxonis.com>
 Maintainer-email: Luxonis <support@luxonis.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -242,31 +242,31 @@
 Requires-Dist: pydantic-settings>=2.1.0; extra == "utils"
 Requires-Dist: PyYAML>=6.0; extra == "utils"
 Requires-Dist: fsspec>=2023.1.0; extra == "utils"
 Requires-Dist: rich>=13.6.0; extra == "utils"
 Provides-Extra: tracker
 Requires-Dist: unique-names-generator>=1.0.2; extra == "tracker"
 Requires-Dist: numpy>=1.22; extra == "tracker"
-Requires-Dist: mlflow>=2.0.1; extra == "tracker"
 Provides-Extra: embedd
 Requires-Dist: docker>=6.1.3; extra == "embedd"
 Requires-Dist: KDEpy>=1.1.5; extra == "embedd"
 Requires-Dist: kmedoids>=0.4.3; extra == "embedd"
 Requires-Dist: matplotlib>=3.7.2; extra == "embedd"
 Requires-Dist: numpy>=1.22; extra == "embedd"
 Requires-Dist: onnx>=1.14.0; extra == "embedd"
 Requires-Dist: onnxruntime-gpu>=1.15.1; sys_platform == "linux" and extra == "embedd"
 Requires-Dist: onnxruntime>=1.15.1; sys_platform != "linux" and extra == "embedd"
 Requires-Dist: opencv-python>=4.7.0.68; extra == "embedd"
 Requires-Dist: qdrant-client>=1.4.0; extra == "embedd"
+Requires-Dist: weaviate-client>=4.4b2; extra == "embedd"
 Requires-Dist: scikit-learn>=1.3.0; extra == "embedd"
 Requires-Dist: scipy>=1.10.1; extra == "embedd"
-Requires-Dist: torch>=1.13.1; extra == "embedd"
-Requires-Dist: torchaudio>=0.13.1; extra == "embedd"
-Requires-Dist: torchvision>=0.14.1; extra == "embedd"
+Provides-Extra: nn-archive
+Requires-Dist: pydantic>=2.4.0; extra == "nn-archive"
+Requires-Dist: pydantic-settings>=2.1.0; extra == "nn-archive"
 Provides-Extra: all
 Requires-Dist: numpy>=1.22; extra == "all"
 Requires-Dist: tqdm>=4.64.1; extra == "all"
 Requires-Dist: opencv-python==4.7.0.68; extra == "all"
 Requires-Dist: opencv-python-headless==4.7.0.68; extra == "all"
 Requires-Dist: PyYAML>=6.0; extra == "all"
 Requires-Dist: label-studio-sdk>=0.0.28; extra == "all"
@@ -278,30 +278,29 @@
 Requires-Dist: pydantic>=2.4.0; extra == "all"
 Requires-Dist: pydantic-settings>=2.1.0; extra == "all"
 Requires-Dist: PyYAML>=6.0; extra == "all"
 Requires-Dist: fsspec>=2023.1.0; extra == "all"
 Requires-Dist: rich>=13.6.0; extra == "all"
 Requires-Dist: unique-names-generator>=1.0.2; extra == "all"
 Requires-Dist: numpy>=1.22; extra == "all"
-Requires-Dist: mlflow>=2.0.1; extra == "all"
 Requires-Dist: docker>=6.1.3; extra == "all"
 Requires-Dist: KDEpy>=1.1.5; extra == "all"
 Requires-Dist: kmedoids>=0.4.3; extra == "all"
 Requires-Dist: matplotlib>=3.7.2; extra == "all"
 Requires-Dist: numpy>=1.22; extra == "all"
 Requires-Dist: onnx>=1.14.0; extra == "all"
 Requires-Dist: onnxruntime-gpu>=1.15.1; sys_platform == "linux" and extra == "all"
 Requires-Dist: onnxruntime>=1.15.1; sys_platform != "linux" and extra == "all"
 Requires-Dist: opencv-python>=4.7.0.68; extra == "all"
 Requires-Dist: qdrant-client>=1.4.0; extra == "all"
+Requires-Dist: weaviate-client>=4.4b2; extra == "all"
 Requires-Dist: scikit-learn>=1.3.0; extra == "all"
 Requires-Dist: scipy>=1.10.1; extra == "all"
-Requires-Dist: torch>=1.13.1; extra == "all"
-Requires-Dist: torchaudio>=0.13.1; extra == "all"
-Requires-Dist: torchvision>=0.14.1; extra == "all"
+Requires-Dist: pydantic>=2.4.0; extra == "all"
+Requires-Dist: pydantic-settings>=2.1.0; extra == "all"
 Provides-Extra: dev
 Requires-Dist: numpy>=1.22; extra == "dev"
 Requires-Dist: tqdm>=4.64.1; extra == "dev"
 Requires-Dist: opencv-python==4.7.0.68; extra == "dev"
 Requires-Dist: opencv-python-headless==4.7.0.68; extra == "dev"
 Requires-Dist: PyYAML>=6.0; extra == "dev"
 Requires-Dist: label-studio-sdk>=0.0.28; extra == "dev"
@@ -313,44 +312,49 @@
 Requires-Dist: pydantic>=2.4.0; extra == "dev"
 Requires-Dist: pydantic-settings>=2.1.0; extra == "dev"
 Requires-Dist: PyYAML>=6.0; extra == "dev"
 Requires-Dist: fsspec>=2023.1.0; extra == "dev"
 Requires-Dist: rich>=13.6.0; extra == "dev"
 Requires-Dist: unique-names-generator>=1.0.2; extra == "dev"
 Requires-Dist: numpy>=1.22; extra == "dev"
-Requires-Dist: mlflow>=2.0.1; extra == "dev"
 Requires-Dist: docker>=6.1.3; extra == "dev"
 Requires-Dist: KDEpy>=1.1.5; extra == "dev"
 Requires-Dist: kmedoids>=0.4.3; extra == "dev"
 Requires-Dist: matplotlib>=3.7.2; extra == "dev"
 Requires-Dist: numpy>=1.22; extra == "dev"
 Requires-Dist: onnx>=1.14.0; extra == "dev"
 Requires-Dist: onnxruntime-gpu>=1.15.1; sys_platform == "linux" and extra == "dev"
 Requires-Dist: onnxruntime>=1.15.1; sys_platform != "linux" and extra == "dev"
 Requires-Dist: opencv-python>=4.7.0.68; extra == "dev"
 Requires-Dist: qdrant-client>=1.4.0; extra == "dev"
+Requires-Dist: weaviate-client>=4.4b2; extra == "dev"
 Requires-Dist: scikit-learn>=1.3.0; extra == "dev"
 Requires-Dist: scipy>=1.10.1; extra == "dev"
-Requires-Dist: torch>=1.13.1; extra == "dev"
-Requires-Dist: torchaudio>=0.13.1; extra == "dev"
-Requires-Dist: torchvision>=0.14.1; extra == "dev"
+Requires-Dist: pydantic>=2.4.0; extra == "dev"
+Requires-Dist: pydantic-settings>=2.1.0; extra == "dev"
 Requires-Dist: pre-commit>=3.2.1; extra == "dev"
 Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
+Requires-Dist: pytest-dependency>=0.6.0; extra == "dev"
 Requires-Dist: pytest-md>=0.2.0; extra == "dev"
 Requires-Dist: gdown>=4.7.1; extra == "dev"
 Requires-Dist: coverage-badge>=1.1.0; extra == "dev"
 
 # LuxonisML
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-![PyBadge](media/pybadge.svg)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+![PyBadge](https://github.com/luxonis/luxonis-ml/blob/116262ee55c36433861689077a522faeb32b3967/media/pybadge.svg)
+![PyPI](https://img.shields.io/pypi/v/luxonis-ml?label=pypi%20package)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/luxonis-ml)
+
 ![CI](https://github.com/luxonis/luxonis-ml/actions/workflows/ci.yaml/badge.svg)
-![Docs](https://github.com/luxonis/luxonis-ml/actions/workflows/docs.yaml/badge.svg)
-![Coverage](media/coverage_badge.svg)
+![Coverage](https://github.com/luxonis/luxonis-ml/blob/dev/media/coverage_badge.svg)
+
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Docformatter](https://img.shields.io/badge/%20formatter-docformatter-fedcba.svg)](https://github.com/PyCQA/docformatter)
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 This library includes a collection of helper functions and utilities for the Luxonis MLOps stack. This includes the following submodules:
 
 - **Dataset Management**: Creating computer vision datasets focused around Luxonis hardware and loading data into our training library.
 - **Embeddings**: Methods to compute image embeddings.
 - **Tracking**: Our implementation of a logger for use with PyTorch Lightning or in our training library.
 - **Utils**: Miscellaneous utils for developers. See this README for details on the different utils.
@@ -380,8 +384,8 @@
 
 ```bash
 pip install luxonis-ml[all]
 ```
 
 ## Contributing
 
-If you want to contribute to this project, read the instructions in [CONTRIBUTING.md](CONTRIBUTING.md)
+If you want to contribute to this project, read the instructions in [CONTRIBUTING.md](https://github.com/luxonis/luxonis-ml/blob/main/CONTRIBUTING.md)
```

### Comparing `luxonis-ml-0.0.1/luxonis_ml.egg-info/requires.txt` & `luxonis-ml-0.1.0/luxonis_ml.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -17,27 +17,24 @@
 pycocotools>=2.0.7
 typeguard>=4.1.0
 pydantic>=2.4.0
 pydantic-settings>=2.1.0
 fsspec>=2023.1.0
 rich>=13.6.0
 unique-names-generator>=1.0.2
-mlflow>=2.0.1
 docker>=6.1.3
 KDEpy>=1.1.5
 kmedoids>=0.4.3
 matplotlib>=3.7.2
 onnx>=1.14.0
 opencv-python>=4.7.0.68
 qdrant-client>=1.4.0
+weaviate-client>=4.4b2
 scikit-learn>=1.3.0
 scipy>=1.10.1
-torch>=1.13.1
-torchaudio>=0.13.1
-torchvision>=0.14.1
 
 [all:sys_platform != "linux"]
 onnxruntime>=1.15.1
 
 [all:sys_platform == "linux"]
 onnxruntime-gpu>=1.15.1
 
@@ -67,29 +64,27 @@
 pycocotools>=2.0.7
 typeguard>=4.1.0
 pydantic>=2.4.0
 pydantic-settings>=2.1.0
 fsspec>=2023.1.0
 rich>=13.6.0
 unique-names-generator>=1.0.2
-mlflow>=2.0.1
 docker>=6.1.3
 KDEpy>=1.1.5
 kmedoids>=0.4.3
 matplotlib>=3.7.2
 onnx>=1.14.0
 opencv-python>=4.7.0.68
 qdrant-client>=1.4.0
+weaviate-client>=4.4b2
 scikit-learn>=1.3.0
 scipy>=1.10.1
-torch>=1.13.1
-torchaudio>=0.13.1
-torchvision>=0.14.1
 pre-commit>=3.2.1
 pytest-cov>=4.1.0
+pytest-dependency>=0.6.0
 pytest-md>=0.2.0
 gdown>=4.7.1
 coverage-badge>=1.1.0
 
 [dev:sys_platform != "linux"]
 onnxruntime>=1.15.1
 
@@ -101,30 +96,31 @@
 KDEpy>=1.1.5
 kmedoids>=0.4.3
 matplotlib>=3.7.2
 numpy>=1.22
 onnx>=1.14.0
 opencv-python>=4.7.0.68
 qdrant-client>=1.4.0
+weaviate-client>=4.4b2
 scikit-learn>=1.3.0
 scipy>=1.10.1
-torch>=1.13.1
-torchaudio>=0.13.1
-torchvision>=0.14.1
 
 [embedd:sys_platform != "linux"]
 onnxruntime>=1.15.1
 
 [embedd:sys_platform == "linux"]
 onnxruntime-gpu>=1.15.1
 
+[nn_archive]
+pydantic>=2.4.0
+pydantic-settings>=2.1.0
+
 [tracker]
 unique-names-generator>=1.0.2
 numpy>=1.22
-mlflow>=2.0.1
 
 [utils]
 pydantic>=2.4.0
 pydantic-settings>=2.1.0
 PyYAML>=6.0
 fsspec>=2023.1.0
 rich>=13.6.0
```

### Comparing `luxonis-ml-0.0.1/pyproject.toml` & `luxonis-ml-0.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "luxonis-ml"
-version = "0.0.1"
+version = "0.1.0"
 description = "MLOps tools for training models for Luxonis devices"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [{ name = "Luxonis", email = "support@luxonis.com" }]
 maintainers = [{ name = "Luxonis", email = "support@luxonis.com" }]
 keywords = ["ml", "ops", "camera", "luxonis", "oak"]
@@ -16,14 +16,17 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
   "Topic :: Scientific/Engineering :: Image Processing",
   "Topic :: Scientific/Engineering :: Image Recognition",
 ]
 
+[project.scripts]
+luxonis_ml = "luxonis_ml.__main__:app"
+
 [project.urls]
 repository = "https://github.com/luxonis/luxonis-ml"
 issues = "https://github.com/luxonis/luxonis-ml/issues"
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
@@ -35,29 +38,32 @@
 dependencies = { file = ["luxonis_ml/utils/requirements.txt"] }
 
 [tool.setuptools.dynamic.optional-dependencies]
 data = { file = ["luxonis_ml/data/requirements.txt"] }
 utils = { file = ["luxonis_ml/utils/requirements.txt"] }
 tracker = { file = ["luxonis_ml/tracker/requirements.txt"] }
 embedd = { file = ["luxonis_ml/embeddings/requirements.txt"] }
+nn_archive = { file = ["luxonis_ml/nn_archive/requirements.txt"] }
 
 [tool.setuptools.dynamic.optional-dependencies.all]
 file = [
     "luxonis_ml/data/requirements.txt",
     "luxonis_ml/utils/requirements.txt",
     "luxonis_ml/tracker/requirements.txt",
     "luxonis_ml/embeddings/requirements.txt",
+    "luxonis_ml/nn_archive/requirements.txt"
 ]
 
 [tool.setuptools.dynamic.optional-dependencies.dev]
 file = [
     "luxonis_ml/data/requirements.txt",
     "luxonis_ml/utils/requirements.txt",
     "luxonis_ml/tracker/requirements.txt",
     "luxonis_ml/embeddings/requirements.txt",
+    "luxonis_ml/nn_archive/requirements.txt",
     "requirements-dev.txt"
 ]
 
 [tool.ruff]
 target-version = "py38"
 line-length = 88
 indent-width = 4
@@ -72,7 +78,13 @@
 
 [tool.mypy]
 python_version = "3.8"
 ignore_missing_imports = true
 
 [tool.pyright]
 typeCheckingMode = "basic"
+
+[tool.coverage.run]
+omit = [
+    "luxonis_ml/embeddings/*",
+    "**/__main__.py"
+]
```

### Comparing `luxonis-ml-0.0.1/tests/test_utils/test_config.py` & `luxonis-ml-0.1.0/tests/test_utils/test_config.py`

 * *Files identical despite different names*

### Comparing `luxonis-ml-0.0.1/tests/test_utils/test_registry.py` & `luxonis-ml-0.1.0/tests/test_utils/test_registry.py`

 * *Files identical despite different names*

