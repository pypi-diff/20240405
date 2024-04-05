# Comparing `tmp/arkindex-base-worker-0.3.7rc7.tar.gz` & `tmp/arkindex-base-worker-0.3.7rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkindex-base-worker-0.3.7rc7.tar", last modified: Thu Apr  4 13:32:10 2024, max compression
+gzip compressed data, was "arkindex-base-worker-0.3.7rc8.tar", last modified: Fri Apr  5 10:26:55 2024, max compression
```

## Comparing `arkindex-base-worker-0.3.7rc7.tar` & `arkindex-base-worker-0.3.7rc8.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:32:10.146465 arkindex-base-worker-0.3.7rc7/
--rw-rw-rw-   0 root         (0) root         (0)     1063 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3359 2024-04-04 13:32:10.142465 arkindex-base-worker-0.3.7rc7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      569 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:32:10.142465 arkindex-base-worker-0.3.7rc7/arkindex_base_worker.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3359 2024-04-04 13:32:10.000000 arkindex-base-worker-0.3.7rc7/arkindex_base_worker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1633 2024-04-04 13:32:10.000000 arkindex-base-worker-0.3.7rc7/arkindex_base_worker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 13:32:10.000000 arkindex-base-worker-0.3.7rc7/arkindex_base_worker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      273 2024-04-04 13:32:10.000000 arkindex-base-worker-0.3.7rc7/arkindex_base_worker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       50 2024-04-04 13:32:10.000000 arkindex-base-worker-0.3.7rc7/arkindex_base_worker.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:32:10.134466 arkindex-base-worker-0.3.7rc7/arkindex_worker/
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11248 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/cache.py
--rw-rw-rw-   0 root         (0) root         (0)    14267 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/image.py
--rw-rw-rw-   0 root         (0) root         (0)     9844 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/models.py
--rw-rw-rw-   0 root         (0) root         (0)     6900 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:32:10.138466 arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/
--rw-rw-rw-   0 root         (0) root         (0)    18575 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19585 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/base.py
--rw-rw-rw-   0 root         (0) root         (0)    10328 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/classification.py
--rw-rw-rw-   0 root         (0) root         (0)     2923 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)    33848 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/element.py
--rw-rw-rw-   0 root         (0) root         (0)    14714 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/entity.py
--rw-rw-rw-   0 root         (0) root         (0)     6702 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     1475 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/task.py
--rw-rw-rw-   0 root         (0) root         (0)    10235 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/training.py
--rw-rw-rw-   0 root         (0) root         (0)    20464 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/transcription.py
--rw-rw-rw-   0 root         (0) root         (0)     1927 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/version.py
--rw-rw-rw-   0 root         (0) root         (0)      132 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/docs-requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:32:10.138466 arkindex-base-worker-0.3.7rc7/hooks/
--rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/hooks/pre_gen_project.py
--rw-rw-rw-   0 root         (0) root         (0)     2405 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      133 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 13:32:10.146465 arkindex-base-worker-0.3.7rc7/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:32:10.138466 arkindex-base-worker-0.3.7rc7/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 13:31:52.000000 arkindex-base-worker-0.3.7rc7/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22134 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    24512 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_base_worker.py
--rw-rw-rw-   0 root         (0) root         (0)    10640 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_cache.py
--rw-rw-rw-   0 root         (0) root         (0)    23728 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_dataset_worker.py
--rw-rw-rw-   0 root         (0) root         (0)    13181 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_element.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:32:10.142465 arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/
--rw-rw-rw-   0 root         (0) root         (0)      179 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26417 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_classifications.py
--rw-rw-rw-   0 root         (0) root         (0)     2878 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    11777 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)    84971 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_elements.py
--rw-rw-rw-   0 root         (0) root         (0)    34557 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_entities.py
--rw-rw-rw-   0 root         (0) root         (0)    18756 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     6312 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_task.py
--rw-rw-rw-   0 root         (0) root         (0)     8414 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_training.py
--rw-rw-rw-   0 root         (0) root         (0)    73468 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_transcriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    17163 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_worker.py
--rw-rw-rw-   0 root         (0) root         (0)    16262 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_image.py
--rw-rw-rw-   0 root         (0) root         (0)     8331 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_merge.py
--rw-rw-rw-   0 root         (0) root         (0)     1236 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:32:10.134466 arkindex-base-worker-0.3.7rc7/worker-demo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:32:10.142465 arkindex-base-worker-0.3.7rc7/worker-demo/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1002 2024-04-04 13:29:16.000000 arkindex-base-worker-0.3.7rc7/worker-demo/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      304 2024-04-04 13:29:16.000000 arkindex-base-worker-0.3.7rc7/worker-demo/tests/test_worker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:32:10.142465 arkindex-base-worker-0.3.7rc7/worker-demo/worker_demo/
--rw-rw-rw-   0 root         (0) root         (0)      125 2024-04-04 13:29:16.000000 arkindex-base-worker-0.3.7rc7/worker-demo/worker_demo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-04 13:29:16.000000 arkindex-base-worker-0.3.7rc7/worker-demo/worker_demo/worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:26:55.425494 arkindex-base-worker-0.3.7rc8/
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3359 2024-04-05 10:26:55.425494 arkindex-base-worker-0.3.7rc8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      569 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:26:55.421494 arkindex-base-worker-0.3.7rc8/arkindex_base_worker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3359 2024-04-05 10:26:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_base_worker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1633 2024-04-05 10:26:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_base_worker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 10:26:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_base_worker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      273 2024-04-05 10:26:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_base_worker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2024-04-05 10:26:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_base_worker.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:26:55.417494 arkindex-base-worker-0.3.7rc8/arkindex_worker/
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11248 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    14267 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/image.py
+-rw-rw-rw-   0 root         (0) root         (0)     9844 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     6900 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:26:55.417494 arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/
+-rw-rw-rw-   0 root         (0) root         (0)    18806 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19585 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    10328 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)     2923 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)    33848 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/element.py
+-rw-rw-rw-   0 root         (0) root         (0)    14714 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/entity.py
+-rw-rw-rw-   0 root         (0) root         (0)     6702 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     1475 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/task.py
+-rw-rw-rw-   0 root         (0) root         (0)    10235 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/training.py
+-rw-rw-rw-   0 root         (0) root         (0)    20464 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/transcription.py
+-rw-rw-rw-   0 root         (0) root         (0)     1927 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      132 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/docs-requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:26:55.417494 arkindex-base-worker-0.3.7rc8/hooks/
+-rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/hooks/pre_gen_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     2405 2024-04-05 10:25:44.000000 arkindex-base-worker-0.3.7rc8/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      133 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 10:26:55.425494 arkindex-base-worker-0.3.7rc8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:26:55.421494 arkindex-base-worker-0.3.7rc8/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 10:26:37.000000 arkindex-base-worker-0.3.7rc8/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22134 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    24512 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_base_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)    10640 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    23848 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_dataset_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)    13181 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_element.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:26:55.421494 arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/
+-rw-rw-rw-   0 root         (0) root         (0)      179 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26417 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_classifications.py
+-rw-rw-rw-   0 root         (0) root         (0)     2878 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    11777 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)    84971 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_elements.py
+-rw-rw-rw-   0 root         (0) root         (0)    34557 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)    18756 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     6312 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     8414 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_training.py
+-rw-rw-rw-   0 root         (0) root         (0)    73468 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_transcriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    17163 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)    16262 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_image.py
+-rw-rw-rw-   0 root         (0) root         (0)     8331 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_merge.py
+-rw-rw-rw-   0 root         (0) root         (0)     1236 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:26:55.413494 arkindex-base-worker-0.3.7rc8/worker-demo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:26:55.421494 arkindex-base-worker-0.3.7rc8/worker-demo/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2024-04-05 10:23:38.000000 arkindex-base-worker-0.3.7rc8/worker-demo/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      304 2024-04-05 10:23:38.000000 arkindex-base-worker-0.3.7rc8/worker-demo/tests/test_worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:26:55.421494 arkindex-base-worker-0.3.7rc8/worker-demo/worker_demo/
+-rw-rw-rw-   0 root         (0) root         (0)      125 2024-04-05 10:23:38.000000 arkindex-base-worker-0.3.7rc8/worker-demo/worker_demo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-05 10:23:38.000000 arkindex-base-worker-0.3.7rc8/worker-demo/worker_demo/worker.py
```

### Comparing `arkindex-base-worker-0.3.7rc7/LICENSE` & `arkindex-base-worker-0.3.7rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/PKG-INFO` & `arkindex-base-worker-0.3.7rc8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkindex-base-worker
-Version: 0.3.7rc7
+Version: 0.3.7rc8
 Summary: Base Worker to easily build Arkindex ML workflows
 Author-email: Teklia <contact@teklia.com>
 Maintainer-email: Teklia <contact@teklia.com>
 License: MIT License
         
         Copyright (c) 2023 Teklia
```

### Comparing `arkindex-base-worker-0.3.7rc7/README.md` & `arkindex-base-worker-0.3.7rc8/README.md`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/arkindex_base_worker.egg-info/PKG-INFO` & `arkindex-base-worker-0.3.7rc8/arkindex_base_worker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkindex-base-worker
-Version: 0.3.7rc7
+Version: 0.3.7rc8
 Summary: Base Worker to easily build Arkindex ML workflows
 Author-email: Teklia <contact@teklia.com>
 Maintainer-email: Teklia <contact@teklia.com>
 License: MIT License
         
         Copyright (c) 2023 Teklia
```

### Comparing `arkindex-base-worker-0.3.7rc7/arkindex_base_worker.egg-info/SOURCES.txt` & `arkindex-base-worker-0.3.7rc8/arkindex_base_worker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/arkindex_worker/cache.py` & `arkindex-base-worker-0.3.7rc8/arkindex_worker/cache.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/arkindex_worker/image.py` & `arkindex-base-worker-0.3.7rc8/arkindex_worker/image.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/arkindex_worker/models.py` & `arkindex-base-worker-0.3.7rc8/arkindex_worker/models.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/arkindex_worker/utils.py` & `arkindex-base-worker-0.3.7rc8/arkindex_worker/utils.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/__init__.py` & `arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -347,15 +347,17 @@
     ):
         """
         :param description: The worker's description.
         :param support_cache: Whether the worker supports cache.
         """
         super().__init__(description, support_cache)
 
-        self.downloaded_artifact: Path | None = None
+        # Path to the dataset compressed archive (containing images and a SQLite database)
+        # Set as an instance variable as dataset workers might use it to easily extract its content
+        self.downloaded_dataset_artifact: Path | None = None
 
         self.parser.add_argument(
             "--set",
             type=check_dataset_set,
             nargs="+",
             help="""
                 One or more Arkindex dataset sets, format is <dataset_uuid>:<set_name>
@@ -385,20 +387,20 @@
         # Retrieve the user configuration
         if self.user_configuration:
             self.config.update(self.user_configuration)
             logger.info("User configuration retrieved")
 
     def cleanup_downloaded_artifact(self) -> None:
         """
-        Cleanup the downloaded artifact if any
+        Cleanup the downloaded dataset artifact if any
         """
-        if not self.downloaded_artifact:
+        if not self.downloaded_dataset_artifact:
             return
 
-        self.downloaded_artifact.unlink(missing_ok=True)
+        self.downloaded_dataset_artifact.unlink(missing_ok=True)
 
     def download_dataset_artifact(self, dataset: Dataset) -> None:
         """
         Find and download the compressed archive artifact describing a dataset using
         the [list_artifacts][arkindex_worker.worker.task.TaskMixin.list_artifacts] and
         [download_artifact][arkindex_worker.worker.task.TaskMixin.download_artifact] methods.
 
@@ -416,15 +418,15 @@
         logger.info(f"Downloading artifact for {dataset}")
         task_id = uuid.UUID(dataset.task_id)
         for artifact in self.list_artifacts(task_id):
             if artifact.path != dataset.filepath:
                 continue
 
             archive.write_bytes(self.download_artifact(task_id, artifact).read())
-            self.downloaded_artifact = archive
+            self.downloaded_dataset_artifact = archive
             return
 
         raise MissingDatasetArchive(
             "The dataset compressed archive artifact was not found."
         )
 
     def process_set(self, set: Set):
```

### Comparing `arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/base.py` & `arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/base.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/classification.py` & `arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/classification.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/dataset.py` & `arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/dataset.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/element.py` & `arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/element.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/entity.py` & `arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/entity.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/metadata.py` & `arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/metadata.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/task.py` & `arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/task.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/training.py` & `arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/training.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/transcription.py` & `arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/transcription.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/version.py` & `arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/version.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/pyproject.toml` & `arkindex-base-worker-0.3.7rc8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "arkindex-base-worker"
-version = "0.3.7rc7"
+version = "0.3.7rc8"
 description = "Base Worker to easily build Arkindex ML workflows"
 license = { file = "LICENSE" }
 dynamic = ["dependencies", "optional-dependencies"]
 authors = [
     { name = "Teklia", email = "contact@teklia.com" },
 ]
 maintainers = [
```

### Comparing `arkindex-base-worker-0.3.7rc7/tests/conftest.py` & `arkindex-base-worker-0.3.7rc8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/tests/test_base_worker.py` & `arkindex-base-worker-0.3.7rc8/tests/test_base_worker.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/tests/test_cache.py` & `arkindex-base-worker-0.3.7rc8/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/tests/test_dataset_worker.py` & `arkindex-base-worker-0.3.7rc8/tests/test_dataset_worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,26 +34,26 @@
 
 
 def test_check_dataset_set():
     assert check_dataset_set(f"{RANDOM_UUID}:train") == (RANDOM_UUID, "train")
 
 
 def test_cleanup_downloaded_artifact_no_download(mock_dataset_worker):
-    assert not mock_dataset_worker.downloaded_artifact
+    assert not mock_dataset_worker.downloaded_dataset_artifact
     # Do nothing
     mock_dataset_worker.cleanup_downloaded_artifact()
 
 
 def test_cleanup_downloaded_artifact(mock_dataset_worker, tmp_archive):
-    mock_dataset_worker.downloaded_artifact = tmp_archive
+    mock_dataset_worker.downloaded_dataset_artifact = tmp_archive
 
-    assert mock_dataset_worker.downloaded_artifact.exists()
+    assert mock_dataset_worker.downloaded_dataset_artifact.exists()
     # Unlink the downloaded archive
     mock_dataset_worker.cleanup_downloaded_artifact()
-    assert not mock_dataset_worker.downloaded_artifact.exists()
+    assert not mock_dataset_worker.downloaded_dataset_artifact.exists()
 
     # Unlinking again does not raise an error even if the archive no longer exists
     mock_dataset_worker.cleanup_downloaded_artifact()
 
 
 def test_download_dataset_artifact_list_api_error(
     responses, mock_dataset_worker, default_dataset
@@ -226,29 +226,32 @@
         f"http://testserver/api/v1/task/{task_id}/artifact/dataset_id.tar.zst",
         status=200,
         body=archive_path.read_bytes(),
         content_type="application/zstd",
     )
 
     if downloaded_cache:
-        mock_dataset_worker.downloaded_artifact = tmp_archive
-    previous_artifact = mock_dataset_worker.downloaded_artifact
+        mock_dataset_worker.downloaded_dataset_artifact = tmp_archive
+    previous_artifact = mock_dataset_worker.downloaded_dataset_artifact
 
     mock_dataset_worker.download_dataset_artifact(default_dataset)
 
     # We removed the artifact that was downloaded previously
     if previous_artifact:
         assert not previous_artifact.exists()
 
-    assert mock_dataset_worker.downloaded_artifact == tmp_path / "dataset_id.tar.zst"
     assert (
-        mock_dataset_worker.downloaded_artifact.read_bytes()
+        mock_dataset_worker.downloaded_dataset_artifact
+        == tmp_path / "dataset_id.tar.zst"
+    )
+    assert (
+        mock_dataset_worker.downloaded_dataset_artifact.read_bytes()
         == archive_path.read_bytes()
     )
-    mock_dataset_worker.downloaded_artifact.unlink()
+    mock_dataset_worker.downloaded_dataset_artifact.unlink()
 
     assert len(responses.calls) == len(BASE_API_CALLS) + 2
     assert [
         (call.request.method, call.request.url) for call in responses.calls
     ] == BASE_API_CALLS + [
         ("GET", f"http://testserver/api/v1/task/{task_id}/artifacts/"),
         ("GET", f"http://testserver/api/v1/task/{task_id}/artifact/dataset_id.tar.zst"),
@@ -260,19 +263,19 @@
 ):
     mocker.patch(
         "arkindex_worker.worker.base.BaseWorker.find_extras_directory",
         return_value=tmp_path,
     )
     already_downloaded = tmp_path / "dataset_id.tar.zst"
     already_downloaded.write_bytes(b"Some content")
-    mock_dataset_worker.downloaded_artifact = already_downloaded
+    mock_dataset_worker.downloaded_dataset_artifact = already_downloaded
 
     mock_dataset_worker.download_dataset_artifact(default_dataset)
 
-    assert mock_dataset_worker.downloaded_artifact == already_downloaded
+    assert mock_dataset_worker.downloaded_dataset_artifact == already_downloaded
     already_downloaded.unlink()
 
     assert len(responses.calls) == len(BASE_API_CALLS)
     assert [
         (call.request.method, call.request.url) for call in responses.calls
     ] == BASE_API_CALLS
 
@@ -530,15 +533,15 @@
         (
             logging.ERROR,
             "Ran on 1 set: 0 completed, 1 failed",
         ),
     ]
 
 
-def test_run_no_downloaded_artifact_error(
+def test_run_no_downloaded_dataset_artifact_error(
     mocker,
     tmp_path,
     responses,
     caplog,
     mock_dataset_worker,
     default_dataset,
 ):
```

### Comparing `arkindex-base-worker-0.3.7rc7/tests/test_element.py` & `arkindex-base-worker-0.3.7rc8/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_classifications.py` & `arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_classifications.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_cli.py` & `arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_cli.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_dataset.py` & `arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_dataset.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_elements.py` & `arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_elements.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_entities.py` & `arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_entities.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_metadata.py` & `arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_metadata.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_task.py` & `arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_task.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_training.py` & `arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_training.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_transcriptions.py` & `arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_transcriptions.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_worker.py` & `arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_worker.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/tests/test_image.py` & `arkindex-base-worker-0.3.7rc8/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/tests/test_merge.py` & `arkindex-base-worker-0.3.7rc8/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/tests/test_utils.py` & `arkindex-base-worker-0.3.7rc8/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc7/worker-demo/tests/conftest.py` & `arkindex-base-worker-0.3.7rc8/worker-demo/tests/conftest.py`

 * *Files identical despite different names*

