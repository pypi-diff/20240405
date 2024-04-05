# Comparing `tmp/openparse-0.3.1.tar.gz` & `tmp/openparse-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openparse-0.3.1.tar", last modified: Mon Apr  1 21:30:39 2024, max compression
+gzip compressed data, was "openparse-0.4.0.tar", last modified: Fri Apr  5 04:40:27 2024, max compression
```

## Comparing `openparse-0.3.1.tar` & `openparse-0.4.0.tar`

### file list

```diff
@@ -1,78 +1,92 @@
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.232764 openparse-0.3.1/
--rw-r--r--   0 sergey     (501) staff       (20)     1072 2024-03-26 18:50:21.000000 openparse-0.3.1/LICENSE
--rw-r--r--   0 sergey     (501) staff       (20)     4581 2024-04-01 21:30:39.232469 openparse-0.3.1/PKG-INFO
--rw-r--r--   0 sergey     (501) staff       (20)     3970 2024-04-01 21:24:05.000000 openparse-0.3.1/README.md
--rw-r--r--   0 sergey     (501) staff       (20)       38 2024-04-01 21:30:39.232818 openparse-0.3.1/setup.cfg
--rw-r--r--   0 sergey     (501) staff       (20)      706 2024-04-01 21:28:49.000000 openparse-0.3.1/setup.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.215076 openparse-0.3.1/src/
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.216854 openparse-0.3.1/src/evals/
--rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-25 03:59:07.000000 openparse-0.3.1/src/evals/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)      684 2024-03-31 16:14:48.000000 openparse-0.3.1/src/evals/run_evals.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.217583 openparse-0.3.1/src/notebooks/
--rw-r--r--   0 sergey     (501) staff       (20)       68 2024-03-25 18:09:44.000000 openparse-0.3.1/src/notebooks/config.py
--rw-r--r--   0 sergey     (501) staff       (20)    29161 2024-03-27 07:16:53.000000 openparse-0.3.1/src/notebooks/trash.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.219991 openparse-0.3.1/src/openparse/
--rw-r--r--   0 sergey     (501) staff       (20)      435 2024-03-27 22:22:49.000000 openparse-0.3.1/src/openparse/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)      225 2024-03-31 17:51:39.000000 openparse-0.3.1/src/openparse/consts.py
--rw-r--r--   0 sergey     (501) staff       (20)     3190 2024-03-27 22:42:17.000000 openparse-0.3.1/src/openparse/main.py
--rw-r--r--   0 sergey     (501) staff       (20)     6083 2024-04-01 21:28:09.000000 openparse-0.3.1/src/openparse/pdf.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.221513 openparse-0.3.1/src/openparse/postprocessing/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-22 22:57:26.000000 openparse-0.3.1/src/openparse/postprocessing/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)      478 2024-03-27 17:19:41.000000 openparse-0.3.1/src/openparse/postprocessing/ingest.py
--rw-r--r--   0 sergey     (501) staff       (20)      733 2024-03-27 17:19:41.000000 openparse-0.3.1/src/openparse/postprocessing/steps.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.222315 openparse-0.3.1/src/openparse/processing/
--rw-r--r--   0 sergey     (501) staff       (20)      609 2024-03-31 21:13:57.000000 openparse-0.3.1/src/openparse/processing/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)      531 2024-03-27 22:41:54.000000 openparse-0.3.1/src/openparse/processing/ingest.py
--rw-r--r--   0 sergey     (501) staff       (20)    10136 2024-03-31 21:47:45.000000 openparse-0.3.1/src/openparse/processing/steps.py
--rw-r--r--   0 sergey     (501) staff       (20)    17544 2024-03-31 21:36:06.000000 openparse-0.3.1/src/openparse/schemas.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.223572 openparse-0.3.1/src/openparse/tables/
--rw-r--r--   0 sergey     (501) staff       (20)      124 2024-03-27 17:19:41.000000 openparse-0.3.1/src/openparse/tables/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     4933 2024-03-27 22:10:32.000000 openparse-0.3.1/src/openparse/tables/parse.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.224132 openparse-0.3.1/src/openparse/tables/pymupdf/
--rw-r--r--   0 sergey     (501) staff       (20)      174 2024-03-27 17:19:41.000000 openparse-0.3.1/src/openparse/tables/pymupdf/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     1199 2024-03-27 05:08:58.000000 openparse-0.3.1/src/openparse/tables/pymupdf/parse.py
--rw-r--r--   0 sergey     (501) staff       (20)     7727 2024-03-27 17:19:41.000000 openparse-0.3.1/src/openparse/tables/schemas.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.225728 openparse-0.3.1/src/openparse/tables/table_transformers/
--rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-27 16:25:28.000000 openparse-0.3.1/src/openparse/tables/table_transformers/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     2700 2024-03-29 00:46:39.000000 openparse-0.3.1/src/openparse/tables/table_transformers/geometry.py
--rw-r--r--   0 sergey     (501) staff       (20)    10495 2024-03-29 00:46:39.000000 openparse-0.3.1/src/openparse/tables/table_transformers/ml.py
--rw-r--r--   0 sergey     (501) staff       (20)      950 2024-03-27 17:19:41.000000 openparse-0.3.1/src/openparse/tables/table_transformers/schemas.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.226211 openparse-0.3.1/src/openparse/tables/unitable/
--rw-r--r--   0 sergey     (501) staff       (20)     6849 2024-03-28 19:39:53.000000 openparse-0.3.1/src/openparse/tables/unitable/ml.py
--rw-r--r--   0 sergey     (501) staff       (20)     3424 2024-03-27 22:12:24.000000 openparse-0.3.1/src/openparse/tables/utils.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.226783 openparse-0.3.1/src/openparse/text/
--rw-r--r--   0 sergey     (501) staff       (20)       48 2024-03-27 17:16:27.000000 openparse-0.3.1/src/openparse/text/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)      743 2024-03-27 17:19:41.000000 openparse-0.3.1/src/openparse/text/parse.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.227342 openparse-0.3.1/src/openparse/text/pdfminer/
--rw-r--r--   0 sergey     (501) staff       (20)       47 2024-03-27 17:16:32.000000 openparse-0.3.1/src/openparse/text/pdfminer/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     4484 2024-03-29 18:14:03.000000 openparse-0.3.1/src/openparse/text/pdfminer/core.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.227834 openparse-0.3.1/src/openparse/text/pymupdf/
--rw-r--r--   0 sergey     (501) staff       (20)       47 2024-03-27 17:19:41.000000 openparse-0.3.1/src/openparse/text/pymupdf/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     2815 2024-03-27 17:19:41.000000 openparse-0.3.1/src/openparse/text/pymupdf/core.py
--rw-r--r--   0 sergey     (501) staff       (20)      221 2024-03-27 17:19:41.000000 openparse-0.3.1/src/openparse/utils.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.231632 openparse-0.3.1/src/openparse.egg-info/
--rw-r--r--   0 sergey     (501) staff       (20)     4581 2024-04-01 21:30:39.000000 openparse-0.3.1/src/openparse.egg-info/PKG-INFO
--rw-r--r--   0 sergey     (501) staff       (20)     1767 2024-04-01 21:30:39.000000 openparse-0.3.1/src/openparse.egg-info/SOURCES.txt
--rw-r--r--   0 sergey     (501) staff       (20)        1 2024-04-01 21:30:39.000000 openparse-0.3.1/src/openparse.egg-info/dependency_links.txt
--rw-r--r--   0 sergey     (501) staff       (20)      129 2024-04-01 21:30:39.000000 openparse-0.3.1/src/openparse.egg-info/requires.txt
--rw-r--r--   0 sergey     (501) staff       (20)       32 2024-04-01 21:30:39.000000 openparse-0.3.1/src/openparse.egg-info/top_level.txt
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.228524 openparse-0.3.1/src/tests/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-23 00:56:45.000000 openparse-0.3.1/src/tests/__init__.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.229574 openparse-0.3.1/src/tests/processing/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-25 01:35:13.000000 openparse-0.3.1/src/tests/processing/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     1085 2024-03-31 15:54:18.000000 openparse-0.3.1/src/tests/processing/test_pipeline.py
--rw-r--r--   0 sergey     (501) staff       (20)    16585 2024-03-31 21:47:11.000000 openparse-0.3.1/src/tests/processing/test_steps.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.229941 openparse-0.3.1/src/tests/tables/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-25 03:12:34.000000 openparse-0.3.1/src/tests/tables/__init__.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.230162 openparse-0.3.1/src/tests/tables/pymupdf/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-27 04:18:24.000000 openparse-0.3.1/src/tests/tables/pymupdf/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     2765 2024-03-27 17:19:41.000000 openparse-0.3.1/src/tests/tables/pymupdf/test_parse.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.230945 openparse-0.3.1/src/tests/tables/transformers/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-27 03:41:31.000000 openparse-0.3.1/src/tests/tables/transformers/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     2174 2024-03-29 00:46:39.000000 openparse-0.3.1/src/tests/tables/transformers/test_geometry.py
--rw-r--r--   0 sergey     (501) staff       (20)    10190 2024-03-27 17:17:26.000000 openparse-0.3.1/src/tests/tables/transformers/test_ml.py
--rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-28 23:19:06.000000 openparse-0.3.1/src/tests/test_main.py
--rw-r--r--   0 sergey     (501) staff       (20)    20672 2024-03-31 21:03:58.000000 openparse-0.3.1/src/tests/test_schemas.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.215465 openparse-0.3.1/src/tests/text/
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-01 21:30:39.231297 openparse-0.3.1/src/tests/text/pdf_miner/
--rw-r--r--   0 sergey     (501) staff       (20)     4002 2024-03-27 17:19:41.000000 openparse-0.3.1/src/tests/text/pdf_miner/test_core.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 04:40:27.498169 openparse-0.4.0/
+-rw-r--r--   0 sergey     (501) staff       (20)     1072 2024-03-26 18:50:21.000000 openparse-0.4.0/LICENSE
+-rw-r--r--   0 sergey     (501) staff       (20)     4855 2024-04-05 04:40:27.497924 openparse-0.4.0/PKG-INFO
+-rw-r--r--   0 sergey     (501) staff       (20)     4203 2024-04-02 23:44:34.000000 openparse-0.4.0/README.md
+-rw-r--r--   0 sergey     (501) staff       (20)       38 2024-04-05 04:40:27.498276 openparse-0.4.0/setup.cfg
+-rw-r--r--   0 sergey     (501) staff       (20)      873 2024-04-05 04:03:18.000000 openparse-0.4.0/setup.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 04:40:27.476563 openparse-0.4.0/src/
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 04:40:27.477910 openparse-0.4.0/src/evals/
+-rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-25 03:59:07.000000 openparse-0.4.0/src/evals/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)      684 2024-03-31 16:14:48.000000 openparse-0.4.0/src/evals/run_evals.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 04:40:27.478572 openparse-0.4.0/src/notebooks/
+-rw-r--r--   0 sergey     (501) staff       (20)       68 2024-03-25 18:09:44.000000 openparse-0.4.0/src/notebooks/config.py
+-rw-r--r--   0 sergey     (501) staff       (20)    29161 2024-03-27 07:16:53.000000 openparse-0.4.0/src/notebooks/trash.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 04:40:27.481624 openparse-0.4.0/src/openparse/
+-rw-r--r--   0 sergey     (501) staff       (20)      435 2024-03-27 22:22:49.000000 openparse-0.4.0/src/openparse/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     1814 2024-04-05 04:39:18.000000 openparse-0.4.0/src/openparse/cli.py
+-rw-r--r--   0 sergey     (501) staff       (20)      225 2024-04-05 01:50:40.000000 openparse-0.4.0/src/openparse/consts.py
+-rw-r--r--   0 sergey     (501) staff       (20)     3641 2024-04-05 01:44:20.000000 openparse-0.4.0/src/openparse/main.py
+-rw-r--r--   0 sergey     (501) staff       (20)     6083 2024-04-03 23:45:13.000000 openparse-0.4.0/src/openparse/pdf.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 04:40:27.483441 openparse-0.4.0/src/openparse/postprocessing/
+-rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-22 22:57:26.000000 openparse-0.4.0/src/openparse/postprocessing/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)      478 2024-03-27 17:19:41.000000 openparse-0.4.0/src/openparse/postprocessing/ingest.py
+-rw-r--r--   0 sergey     (501) staff       (20)      733 2024-03-27 17:19:41.000000 openparse-0.4.0/src/openparse/postprocessing/steps.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 04:40:27.484408 openparse-0.4.0/src/openparse/processing/
+-rw-r--r--   0 sergey     (501) staff       (20)      609 2024-03-31 21:13:57.000000 openparse-0.4.0/src/openparse/processing/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)      536 2024-04-05 00:11:18.000000 openparse-0.4.0/src/openparse/processing/ingest.py
+-rw-r--r--   0 sergey     (501) staff       (20)    10133 2024-04-05 02:32:51.000000 openparse-0.4.0/src/openparse/processing/steps.py
+-rw-r--r--   0 sergey     (501) staff       (20)    17235 2024-04-05 02:32:01.000000 openparse-0.4.0/src/openparse/schemas.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 04:40:27.485690 openparse-0.4.0/src/openparse/tables/
+-rw-r--r--   0 sergey     (501) staff       (20)      154 2024-04-04 23:25:17.000000 openparse-0.4.0/src/openparse/tables/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     7686 2024-04-05 00:02:31.000000 openparse-0.4.0/src/openparse/tables/parse.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 04:40:27.486286 openparse-0.4.0/src/openparse/tables/pymupdf/
+-rw-r--r--   0 sergey     (501) staff       (20)      174 2024-03-27 17:19:41.000000 openparse-0.4.0/src/openparse/tables/pymupdf/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     1199 2024-03-27 05:08:58.000000 openparse-0.4.0/src/openparse/tables/pymupdf/parse.py
+-rw-r--r--   0 sergey     (501) staff       (20)     7727 2024-04-04 04:03:34.000000 openparse-0.4.0/src/openparse/tables/schemas.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 04:40:27.487545 openparse-0.4.0/src/openparse/tables/table_transformers/
+-rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-27 16:25:28.000000 openparse-0.4.0/src/openparse/tables/table_transformers/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     1343 2024-04-04 04:05:49.000000 openparse-0.4.0/src/openparse/tables/table_transformers/geometry.py
+-rw-r--r--   0 sergey     (501) staff       (20)    10575 2024-04-04 05:55:33.000000 openparse-0.4.0/src/openparse/tables/table_transformers/ml.py
+-rw-r--r--   0 sergey     (501) staff       (20)     8546 2024-04-04 05:54:53.000000 openparse-0.4.0/src/openparse/tables/table_transformers/schemas.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 04:40:27.490138 openparse-0.4.0/src/openparse/tables/unitable/
+-rw-r--r--   0 sergey     (501) staff       (20)       69 2024-04-05 01:51:43.000000 openparse-0.4.0/src/openparse/tables/unitable/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     1681 2024-04-05 04:40:04.000000 openparse-0.4.0/src/openparse/tables/unitable/config.py
+-rw-r--r--   0 sergey     (501) staff       (20)     6288 2024-04-04 23:28:47.000000 openparse-0.4.0/src/openparse/tables/unitable/core.py
+-rw-r--r--   0 sergey     (501) staff       (20)     2976 2024-04-04 22:49:10.000000 openparse-0.4.0/src/openparse/tables/unitable/schemas.py
+-rw-r--r--   0 sergey     (501) staff       (20)     6164 2024-04-03 16:13:24.000000 openparse-0.4.0/src/openparse/tables/unitable/tabular_transformer.py
+-rw-r--r--   0 sergey     (501) staff       (20)     1629 2024-04-03 16:10:37.000000 openparse-0.4.0/src/openparse/tables/unitable/tokens.py
+-rw-r--r--   0 sergey     (501) staff       (20)     2215 2024-04-04 20:54:38.000000 openparse-0.4.0/src/openparse/tables/unitable/unitable_model.py
+-rw-r--r--   0 sergey     (501) staff       (20)     4212 2024-04-04 23:00:47.000000 openparse-0.4.0/src/openparse/tables/unitable/utils.py
+-rw-r--r--   0 sergey     (501) staff       (20)     6189 2024-04-05 00:01:16.000000 openparse-0.4.0/src/openparse/tables/utils.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 04:40:27.490866 openparse-0.4.0/src/openparse/text/
+-rw-r--r--   0 sergey     (501) staff       (20)       48 2024-03-27 17:16:27.000000 openparse-0.4.0/src/openparse/text/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)      743 2024-03-27 17:19:41.000000 openparse-0.4.0/src/openparse/text/parse.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 04:40:27.491474 openparse-0.4.0/src/openparse/text/pdfminer/
+-rw-r--r--   0 sergey     (501) staff       (20)       47 2024-03-27 17:16:32.000000 openparse-0.4.0/src/openparse/text/pdfminer/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     4484 2024-03-29 18:14:03.000000 openparse-0.4.0/src/openparse/text/pdfminer/core.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 04:40:27.492029 openparse-0.4.0/src/openparse/text/pymupdf/
+-rw-r--r--   0 sergey     (501) staff       (20)       47 2024-03-27 17:19:41.000000 openparse-0.4.0/src/openparse/text/pymupdf/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     2815 2024-03-27 17:19:41.000000 openparse-0.4.0/src/openparse/text/pymupdf/core.py
+-rw-r--r--   0 sergey     (501) staff       (20)      839 2024-04-04 23:36:41.000000 openparse-0.4.0/src/openparse/types.py
+-rw-r--r--   0 sergey     (501) staff       (20)      221 2024-03-27 17:19:41.000000 openparse-0.4.0/src/openparse/utils.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 04:40:27.497313 openparse-0.4.0/src/openparse.egg-info/
+-rw-r--r--   0 sergey     (501) staff       (20)     4855 2024-04-05 04:40:27.000000 openparse-0.4.0/src/openparse.egg-info/PKG-INFO
+-rw-r--r--   0 sergey     (501) staff       (20)     2292 2024-04-05 04:40:27.000000 openparse-0.4.0/src/openparse.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey     (501) staff       (20)        1 2024-04-05 04:40:27.000000 openparse-0.4.0/src/openparse.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey     (501) staff       (20)       79 2024-04-05 04:40:27.000000 openparse-0.4.0/src/openparse.egg-info/entry_points.txt
+-rw-r--r--   0 sergey     (501) staff       (20)      140 2024-04-05 04:40:27.000000 openparse-0.4.0/src/openparse.egg-info/requires.txt
+-rw-r--r--   0 sergey     (501) staff       (20)       42 2024-04-05 04:40:27.000000 openparse-0.4.0/src/openparse.egg-info/top_level.txt
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 04:40:27.492796 openparse-0.4.0/src/tests/
+-rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-23 00:56:45.000000 openparse-0.4.0/src/tests/__init__.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 04:40:27.493627 openparse-0.4.0/src/tests/processing/
+-rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-25 01:35:13.000000 openparse-0.4.0/src/tests/processing/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     1085 2024-03-31 15:54:18.000000 openparse-0.4.0/src/tests/processing/test_pipeline.py
+-rw-r--r--   0 sergey     (501) staff       (20)    16585 2024-03-31 21:47:11.000000 openparse-0.4.0/src/tests/processing/test_steps.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 04:40:27.493986 openparse-0.4.0/src/tests/tables/
+-rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-25 03:12:34.000000 openparse-0.4.0/src/tests/tables/__init__.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 04:40:27.494225 openparse-0.4.0/src/tests/tables/pymupdf/
+-rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-27 04:18:24.000000 openparse-0.4.0/src/tests/tables/pymupdf/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     2765 2024-03-27 17:19:41.000000 openparse-0.4.0/src/tests/tables/pymupdf/test_parse.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 04:40:27.494959 openparse-0.4.0/src/tests/tables/transformers/
+-rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-27 03:41:31.000000 openparse-0.4.0/src/tests/tables/transformers/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)     2174 2024-03-29 00:46:39.000000 openparse-0.4.0/src/tests/tables/transformers/test_geometry.py
+-rw-r--r--   0 sergey     (501) staff       (20)    10190 2024-03-27 17:17:26.000000 openparse-0.4.0/src/tests/tables/transformers/test_ml.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 04:40:27.496769 openparse-0.4.0/src/tests/tables/unitable/
+-rw-r--r--   0 sergey     (501) staff       (20)        0 2024-04-04 21:15:51.000000 openparse-0.4.0/src/tests/tables/unitable/__init__.py
+-rw-r--r--   0 sergey     (501) staff       (20)   190851 2024-04-04 21:28:58.000000 openparse-0.4.0/src/tests/tables/unitable/sample_pred_outputs.py
+-rw-r--r--   0 sergey     (501) staff       (20)     1113 2024-04-05 03:42:13.000000 openparse-0.4.0/src/tests/tables/unitable/test_pred_to_schema.py
+-rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-28 23:19:06.000000 openparse-0.4.0/src/tests/test_main.py
+-rw-r--r--   0 sergey     (501) staff       (20)    20672 2024-03-31 21:03:58.000000 openparse-0.4.0/src/tests/test_schemas.py
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 04:40:27.477024 openparse-0.4.0/src/tests/text/
+drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-05 04:40:27.497012 openparse-0.4.0/src/tests/text/pdf_miner/
+-rw-r--r--   0 sergey     (501) staff       (20)     4002 2024-03-27 17:19:41.000000 openparse-0.4.0/src/tests/text/pdf_miner/test_core.py
```

### Comparing `openparse-0.3.1/LICENSE` & `openparse-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openparse-0.3.1/PKG-INFO` & `openparse-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openparse
-Version: 0.3.1
+Version: 0.4.0
 Summary: Streamlines the process of preparing documents for LLM's.
 Home-page: https://github.com/Filimoa/open-parse/
 Author: Sergey Filimonov
 Author-email: hello@sergey.fyi
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyMuPDF>=1.23.2
@@ -13,21 +13,26 @@
 Requires-Dist: pypdf>=4.0.0
 Requires-Dist: pdfminer.six>=20200401
 Requires-Dist: tiktoken>=0.3
 Provides-Extra: ml
 Requires-Dist: torch; extra == "ml"
 Requires-Dist: torchvision; extra == "ml"
 Requires-Dist: transformers; extra == "ml"
+Requires-Dist: tokenizers; extra == "ml"
 
 <p align="center">
     <img src="https://sergey-filimonov.nyc3.digitaloceanspaces.com/open-parse/open-parse-with-text-tp-logo.webp" width="350" />
 </p>
 <br/>
 
-Open-Parse streamlines the process of preparing complex documents for analysis by LLMs. Our goal is to expose state-of-the-art deep learning models with a few lines of code while also providing flexible heuristic options for faster, basic parsing.
+**Easily chunk complex documents the same way a human would.**  
+
+Chunking documents is a challenging task that underpins any RAG system.  High quality results are critical to a sucessful AI application, yet most open-source libraries are limited in their ability to handle complex documents.  
+
+Open Parse is designed to fill this gap by providing a flexible, easy-to-use library capable of visually discerning document layouts and chunking them effectively.
 
 ### Highlights
 
 - **🔍 Visually-Driven:** Open-Parse visually analyzes documents for superior LLM input, going beyond naive text splitting.
 - **✍️ Markdown Support:** Basic markdown support for parsing headings, bold and italics.
 - **📊 High-Precision Table Support:** Extract tables into clean Markdown formats with accuracy that surpasses traditional tools.
 - **🛠️ Extensible:** Easily implement your own post-processing steps.
@@ -45,15 +50,15 @@
 import openparse
 
 basic_doc_path = "./sample-docs/mobile-home-manual.pdf"
 parser = openparse.DocumentParser()
 parsed_basic_doc = parser.parse(basic_doc_path)
 
 for node in parsed_basic_doc.nodes:
-    display(node)
+    print(node)
 ```
 
 **📓 Try the sample notebook** <a href="https://colab.research.google.com/drive/1Z5B5gsnmhFKEFL-5yYIcoox7-jQao8Ep?usp=sharing" class="external-link" target="_blank">here</a>
 
 ## Requirements
 
 Python 3.8+
@@ -101,13 +106,13 @@
 **Note:** _On Windows systems, this must happen outside Python – before starting your script. Just manipulating os.environ will not work!_
 
 #### 2. ML Table Detection (Optional)
 
 This repository provides an optional feature to parse content from tables using the state-of-the-art Table Transformer (DETR) model. The Table Transformer model, introduced in the paper "PubTables-1M: Towards Comprehensive Table Extraction From Unstructured Documents" by Smock et al., achieves best-in-class results for table extraction.
 
 ```console
-pip install "open-parse[ml]"
+pip install "openparse[ml]"
 ```
 
 ## Documentation
 
-_Coming Soon_
+https://filimoa.github.io/open-parse/
```

#### html2text {}

```diff
@@ -1,36 +1,39 @@
-Metadata-Version: 2.1 Name: openparse Version: 0.3.1 Summary: Streamlines the
+Metadata-Version: 2.1 Name: openparse Version: 0.4.0 Summary: Streamlines the
 process of preparing documents for LLM's. Home-page: https://github.com/
 Filimoa/open-parse/ Author: Sergey Filimonov Author-email: hello@sergey.fyi
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 PyMuPDF>=1.23.2 Requires-Dist: pillow>=8.3 Requires-Dist: pydantic>=2.0
 Requires-Dist: pypdf>=4.0.0 Requires-Dist: pdfminer.six>=20200401 Requires-
 Dist: tiktoken>=0.3 Provides-Extra: ml Requires-Dist: torch; extra == "ml"
 Requires-Dist: torchvision; extra == "ml" Requires-Dist: transformers; extra ==
-"ml"
+"ml" Requires-Dist: tokenizers; extra == "ml"
  [https://sergey-filimonov.nyc3.digitaloceanspaces.com/open-parse/open-parse-
                             with-text-tp-logo.webp]
 
-Open-Parse streamlines the process of preparing complex documents for analysis
-by LLMs. Our goal is to expose state-of-the-art deep learning models with a few
-lines of code while also providing flexible heuristic options for faster, basic
-parsing. ### Highlights - **ð Visually-Driven:** Open-Parse visually
-analyzes documents for superior LLM input, going beyond naive text splitting. -
-**âï¸ Markdown Support:** Basic markdown support for parsing headings, bold
-and italics. - **ð High-Precision Table Support:** Extract tables into clean
+**Easily chunk complex documents the same way a human would.** Chunking
+documents is a challenging task that underpins any RAG system. High quality
+results are critical to a sucessful AI application, yet most open-source
+libraries are limited in their ability to handle complex documents. Open Parse
+is designed to fill this gap by providing a flexible, easy-to-use library
+capable of visually discerning document layouts and chunking them effectively.
+### Highlights - **ð Visually-Driven:** Open-Parse visually analyzes
+documents for superior LLM input, going beyond naive text splitting. - **âï¸
+Markdown Support:** Basic markdown support for parsing headings, bold and
+italics. - **ð High-Precision Table Support:** Extract tables into clean
 Markdown formats with accuracy that surpasses traditional tools. - **ð ï¸
 Extensible:** Easily implement your own post-processing steps. -
 **ð¡Intuitive:** Great editor support. Completion everywhere. Less time
 debugging. - **ð¯ Easy:** Designed to be easy to use and learn. Less time
 reading docs.
 [https://sergey-filimonov.nyc3.digitaloceanspaces.com/open-parse/marked-up-doc-
                                     2.webp]
 ## Example ```python import openparse basic_doc_path = "./sample-docs/mobile-
 home-manual.pdf" parser = openparse.DocumentParser() parsed_basic_doc =
-parser.parse(basic_doc_path) for node in parsed_basic_doc.nodes: display(node)
+parser.parse(basic_doc_path) for node in parsed_basic_doc.nodes: print(node)
 ``` **ð Try the sample notebook** _h_e_r_e ## Requirements Python 3.8+ **Dealing
 with PDF's:** - _p_d_f_m_i_n_e_r_._s_i_x Fully open source. **Extracting Tables:** -
 _P_y_M_u_P_D_F has some table detection functionality. Please see their _l_i_c_e_n_s_e. -
 _T_a_b_l_e_ _T_r_a_n_s_f_o_r_m_e_r is a deep learning approach. - _u_n_i_t_a_b_l_e is a more recent deep
 learning approach that seems promising _(coming soon)_ ## Installation #### 1.
 Core Library ```console pip install openparse ``` **Enabling OCR Support**:
 PyMuPDF will already contain all the logic to support OCR functions. But it
@@ -47,9 +50,9 @@
 tesseract-ocr/5/tessdata` **Note:** _On Windows systems, this must happen
 outside Python â before starting your script. Just manipulating os.environ
 will not work!_ #### 2. ML Table Detection (Optional) This repository provides
 an optional feature to parse content from tables using the state-of-the-art
 Table Transformer (DETR) model. The Table Transformer model, introduced in the
 paper "PubTables-1M: Towards Comprehensive Table Extraction From Unstructured
 Documents" by Smock et al., achieves best-in-class results for table
-extraction. ```console pip install "open-parse[ml]" ``` ## Documentation
-_Coming Soon_
+extraction. ```console pip install "openparse[ml]" ``` ## Documentation https:/
+/filimoa.github.io/open-parse/
```

### Comparing `openparse-0.3.1/README.md` & `openparse-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 <p align="center">
     <img src="https://sergey-filimonov.nyc3.digitaloceanspaces.com/open-parse/open-parse-with-text-tp-logo.webp" width="350" />
 </p>
 <br/>
 
-Open-Parse streamlines the process of preparing complex documents for analysis by LLMs. Our goal is to expose state-of-the-art deep learning models with a few lines of code while also providing flexible heuristic options for faster, basic parsing.
+**Easily chunk complex documents the same way a human would.**  
+
+Chunking documents is a challenging task that underpins any RAG system.  High quality results are critical to a sucessful AI application, yet most open-source libraries are limited in their ability to handle complex documents.  
+
+Open Parse is designed to fill this gap by providing a flexible, easy-to-use library capable of visually discerning document layouts and chunking them effectively.
 
 ### Highlights
 
 - **🔍 Visually-Driven:** Open-Parse visually analyzes documents for superior LLM input, going beyond naive text splitting.
 - **✍️ Markdown Support:** Basic markdown support for parsing headings, bold and italics.
 - **📊 High-Precision Table Support:** Extract tables into clean Markdown formats with accuracy that surpasses traditional tools.
 - **🛠️ Extensible:** Easily implement your own post-processing steps.
@@ -25,15 +29,15 @@
 import openparse
 
 basic_doc_path = "./sample-docs/mobile-home-manual.pdf"
 parser = openparse.DocumentParser()
 parsed_basic_doc = parser.parse(basic_doc_path)
 
 for node in parsed_basic_doc.nodes:
-    display(node)
+    print(node)
 ```
 
 **📓 Try the sample notebook** <a href="https://colab.research.google.com/drive/1Z5B5gsnmhFKEFL-5yYIcoox7-jQao8Ep?usp=sharing" class="external-link" target="_blank">here</a>
 
 ## Requirements
 
 Python 3.8+
@@ -81,13 +85,13 @@
 **Note:** _On Windows systems, this must happen outside Python – before starting your script. Just manipulating os.environ will not work!_
 
 #### 2. ML Table Detection (Optional)
 
 This repository provides an optional feature to parse content from tables using the state-of-the-art Table Transformer (DETR) model. The Table Transformer model, introduced in the paper "PubTables-1M: Towards Comprehensive Table Extraction From Unstructured Documents" by Smock et al., achieves best-in-class results for table extraction.
 
 ```console
-pip install "open-parse[ml]"
+pip install "openparse[ml]"
 ```
 
 ## Documentation
 
-_Coming Soon_
+https://filimoa.github.io/open-parse/
```

#### html2text {}

```diff
@@ -1,27 +1,30 @@
  [https://sergey-filimonov.nyc3.digitaloceanspaces.com/open-parse/open-parse-
                             with-text-tp-logo.webp]
 
-Open-Parse streamlines the process of preparing complex documents for analysis
-by LLMs. Our goal is to expose state-of-the-art deep learning models with a few
-lines of code while also providing flexible heuristic options for faster, basic
-parsing. ### Highlights - **ð Visually-Driven:** Open-Parse visually
-analyzes documents for superior LLM input, going beyond naive text splitting. -
-**âï¸ Markdown Support:** Basic markdown support for parsing headings, bold
-and italics. - **ð High-Precision Table Support:** Extract tables into clean
+**Easily chunk complex documents the same way a human would.** Chunking
+documents is a challenging task that underpins any RAG system. High quality
+results are critical to a sucessful AI application, yet most open-source
+libraries are limited in their ability to handle complex documents. Open Parse
+is designed to fill this gap by providing a flexible, easy-to-use library
+capable of visually discerning document layouts and chunking them effectively.
+### Highlights - **ð Visually-Driven:** Open-Parse visually analyzes
+documents for superior LLM input, going beyond naive text splitting. - **âï¸
+Markdown Support:** Basic markdown support for parsing headings, bold and
+italics. - **ð High-Precision Table Support:** Extract tables into clean
 Markdown formats with accuracy that surpasses traditional tools. - **ð ï¸
 Extensible:** Easily implement your own post-processing steps. -
 **ð¡Intuitive:** Great editor support. Completion everywhere. Less time
 debugging. - **ð¯ Easy:** Designed to be easy to use and learn. Less time
 reading docs.
 [https://sergey-filimonov.nyc3.digitaloceanspaces.com/open-parse/marked-up-doc-
                                     2.webp]
 ## Example ```python import openparse basic_doc_path = "./sample-docs/mobile-
 home-manual.pdf" parser = openparse.DocumentParser() parsed_basic_doc =
-parser.parse(basic_doc_path) for node in parsed_basic_doc.nodes: display(node)
+parser.parse(basic_doc_path) for node in parsed_basic_doc.nodes: print(node)
 ``` **ð Try the sample notebook** _h_e_r_e ## Requirements Python 3.8+ **Dealing
 with PDF's:** - _p_d_f_m_i_n_e_r_._s_i_x Fully open source. **Extracting Tables:** -
 _P_y_M_u_P_D_F has some table detection functionality. Please see their _l_i_c_e_n_s_e. -
 _T_a_b_l_e_ _T_r_a_n_s_f_o_r_m_e_r is a deep learning approach. - _u_n_i_t_a_b_l_e is a more recent deep
 learning approach that seems promising _(coming soon)_ ## Installation #### 1.
 Core Library ```console pip install openparse ``` **Enabling OCR Support**:
 PyMuPDF will already contain all the logic to support OCR functions. But it
@@ -38,9 +41,9 @@
 tesseract-ocr/5/tessdata` **Note:** _On Windows systems, this must happen
 outside Python â before starting your script. Just manipulating os.environ
 will not work!_ #### 2. ML Table Detection (Optional) This repository provides
 an optional feature to parse content from tables using the state-of-the-art
 Table Transformer (DETR) model. The Table Transformer model, introduced in the
 paper "PubTables-1M: Towards Comprehensive Table Extraction From Unstructured
 Documents" by Smock et al., achieves best-in-class results for table
-extraction. ```console pip install "open-parse[ml]" ``` ## Documentation
-_Coming Soon_
+extraction. ```console pip install "openparse[ml]" ``` ## Documentation https:/
+/filimoa.github.io/open-parse/
```

### Comparing `openparse-0.3.1/src/evals/run_evals.py` & `openparse-0.4.0/src/evals/run_evals.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.1/src/notebooks/trash.py` & `openparse-0.4.0/src/notebooks/trash.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.1/src/openparse/main.py` & `openparse-0.4.0/src/openparse/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 from pathlib import Path
 from typing import List, Literal, Optional, TypedDict, Union
 
 from openparse import tables, text, consts
 from openparse.pdf import Pdf
+from openparse.types import NOT_GIVEN, NotGiven
 from openparse.processing import ProcessingStep, default_pipeline, run_pipeline
 from openparse.schemas import Node, TableElement, TextElement, ParsedDocument
 
 
+class UnitableArgsDict(TypedDict, total=False):
+    parsing_algorithm: Literal["unitable"]
+    min_table_confidence: float
+    table_output_format: Literal["html"]
+
+
 class TableTransformersArgsDict(TypedDict, total=False):
     parsing_algorithm: Literal["table-transformers"]
     min_table_confidence: float
     min_cell_confidence: float
-    table_output_format: Literal["str", "markdown", "html"]
+    table_output_format: Literal["markdown", "html"]
 
 
 class PyMuPDFArgsDict(TypedDict, total=False):
     parsing_algorithm: Literal["pymupdf"]
-    table_output_format: Literal["str", "markdown", "html"]
+    table_output_format: Literal["markdown", "html"]
 
 
 def _table_args_dict_to_model(
     args_dict: Union[TableTransformersArgsDict, PyMuPDFArgsDict]
 ) -> Union[tables.TableTransformersArgs, tables.PyMuPDFArgs]:
     if args_dict["parsing_algorithm"] == "table-transformers":
         return tables.TableTransformersArgs(**args_dict)
     elif args_dict["parsing_algorithm"] == "pymupdf":
         return tables.PyMuPDFArgs(**args_dict)
+    elif args_dict["parsing_algorithm"] == "unitable":
+        return tables.UnitableArgs(**args_dict)
     else:
         raise ValueError(
             f"Unsupported parsing_algorithm: {args_dict['parsing_algorithm']}"
         )
 
 
 class DocumentParser:
@@ -42,18 +51,23 @@
     """
 
     _verbose: bool = False
 
     def __init__(
         self,
         *,
-        processing_pipeline: Optional[List[ProcessingStep]] = None,
-        table_args: Union[TableTransformersArgsDict, PyMuPDFArgsDict, None] = None,
+        processing_pipeline: Union[List[ProcessingStep], NotGiven] = NOT_GIVEN,
+        table_args: Union[
+            TableTransformersArgsDict, PyMuPDFArgsDict, NotGiven
+        ] = NOT_GIVEN,
     ):
-        self.processing_pipeline = processing_pipeline or default_pipeline
+        if processing_pipeline is NOT_GIVEN:
+            self.processing_pipeline = default_pipeline
+        else:
+            self.processing_pipeline = processing_pipeline or []
 
         self.table_args = table_args
 
     def parse(
         self,
         file: str | Path,
     ) -> ParsedDocument:
```

### Comparing `openparse-0.3.1/src/openparse/pdf.py` & `openparse-0.4.0/src/openparse/pdf.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.1/src/openparse/postprocessing/steps.py` & `openparse-0.4.0/src/openparse/postprocessing/steps.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.1/src/openparse/processing/__init__.py` & `openparse-0.4.0/src/openparse/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.1/src/openparse/processing/steps.py` & `openparse-0.4.0/src/openparse/processing/steps.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,52 +19,51 @@
     If we're using the table extraction pipeline, we need to remove text that is inside tables to avoid duplication.
     """
 
     def process(self, nodes: List[Node]) -> List[Node]:
         # Group all table bounding boxes by page
         tables_by_page = defaultdict(list)
         for node in nodes:
-            if node.variant == "table":
+            if node.variant == {"table"}:
                 for table_element in node.elements:
                     tables_by_page[table_element.page].append(table_element.bbox)
 
         updated_nodes = []
         for node in nodes:
-            if node.variant == "table":
+            if node.variant == {"table"}:
                 updated_nodes.append(node)
                 continue
 
             new_elements = [
                 element
                 for element in node.elements
                 if not (
                     isinstance(element, TextElement)
-                    and self.is_inside_any_table(
+                    and self.intersects_any_table(
                         element.bbox, tables_by_page[element.page]
                     )
                 )
             ]
-
             if new_elements:
                 updated_nodes.append(Node(elements=tuple(new_elements)))
 
         return updated_nodes
 
-    def is_inside_any_table(self, text_bbox: Bbox, table_bboxes: List[Bbox]) -> bool:
+    def intersects_any_table(self, text_bbox: Bbox, table_bboxes: List[Bbox]) -> bool:
         return any(
-            self.is_contained(text_bbox, table_bbox) for table_bbox in table_bboxes
+            self.intersects(text_bbox, table_bbox) for table_bbox in table_bboxes
         )
 
     @staticmethod
-    def is_contained(text_bbox: Bbox, table_bbox: Bbox) -> bool:
+    def intersects(text_bbox: Bbox, table_bbox: Bbox) -> bool:
         return (
-            text_bbox.x0 >= table_bbox.x0
-            and text_bbox.x1 <= table_bbox.x1
-            and text_bbox.y0 >= table_bbox.y0
-            and text_bbox.y1 <= table_bbox.y1
+            text_bbox.x1 > table_bbox.x0
+            and text_bbox.x0 < table_bbox.x1
+            and text_bbox.y1 > table_bbox.y0
+            and text_bbox.y0 < table_bbox.y1
         )
 
 
 class RemoveFullPageStubs(ProcessingStep):
     """
     Sometimes elements take up entire pages and are not useful for downstream processing.
     """
```

### Comparing `openparse-0.3.1/src/openparse/schemas.py` & `openparse-0.4.0/src/openparse/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,12 @@
 import re
 from collections import defaultdict, namedtuple
 from enum import Enum
 from functools import cached_property
-from typing import (
-    Any,
-    List,
-    Literal,
-    Optional,
-    Tuple,
-    Union,
-)
+from typing import Any, List, Literal, Optional, Tuple, Union, Set
 
 from pydantic import BaseModel, ConfigDict, computed_field, model_validator, Field
 
 from openparse import consts
 from openparse.utils import num_tokens
 
 bullet_regex = re.compile(
@@ -366,24 +359,16 @@
     _tokenization_upper_limit: int = consts.TOKENIZATION_UPPER_LIMIT
     _coordinates: Literal["top-left", "bottom-left"] = (
         consts.COORDINATE_SYSTEM
     )  # controlled globally for now, should be moved into elements
 
     @computed_field  # type: ignore
     @cached_property
-    def variant(self) -> Literal["text", "table", "mixed"]:
-        unique_variants = set(e.variant for e in self.elements)
-        if len(unique_variants) > 1:
-            return "mixed"
-        elif NodeVariant.TEXT in unique_variants:
-            return "text"
-        elif NodeVariant.TABLE in unique_variants:
-            return "table"
-        else:
-            raise ValueError("Unknown variant")
+    def variant(self) -> Set[Literal["text", "table"]]:
+        return set(e.variant.value for e in self.elements)
 
     @computed_field  # type: ignore
     @cached_property
     def tokens(self) -> int:
         return sum([e.tokens for e in self.elements])
 
     @computed_field  # type: ignore
@@ -441,24 +426,24 @@
 
             texts.append(current.embed_text)
 
         return "".join(texts)
 
     @cached_property
     def is_heading(self) -> bool:
-        if self.variant != "text":
+        if self.variant != {"text"}:
             return False
         if not self.is_stub:
             return False
 
         return all(element.is_heading or element.is_bold for element in self.elements)  # type: ignore
 
     @cached_property
     def starts_with_heading(self) -> bool:
-        if not self.variant == "text":
+        if not self.variant == {"text"}:
             return False
         return self.elements[0].is_heading  # type: ignore
 
     @cached_property
     def starts_with_bullet(self) -> bool:
         first_line = self.text.split(consts.ELEMENT_DELIMETER)[0].strip()
         if not first_line:
```

### Comparing `openparse-0.3.1/src/openparse/tables/parse.py` & `openparse-0.4.0/src/openparse/tables/parse.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,45 @@
 from typing import List, Literal, Union
 
 from pydantic import BaseModel, ConfigDict, Field
 
 from openparse.pdf import Pdf
 from openparse.schemas import Bbox, TableElement
+from openparse.tables.utils import crop_img_with_padding, adjust_bbox_with_padding
 
 from . import pymupdf
 
 
 class ParsingArgs(BaseModel):
     parsing_algorithm: str
     table_output_format: Literal["str", "markdown", "html"] = Field(default="html")
 
 
-class TableTransformersArgs(ParsingArgs):
-    min_table_confidence: float = Field(default=0.75, ge=0.0, le=1.0)
-    min_cell_confidence: float = Field(default=0.95, ge=0.0, le=1.0)
+class TableTransformersArgs(BaseModel):
     parsing_algorithm: Literal["table-transformers"] = Field(
         default="table-transformers"
     )
+    min_table_confidence: float = Field(default=0.75, ge=0.0, le=1.0)
+    min_cell_confidence: float = Field(default=0.95, ge=0.0, le=1.0)
+    table_output_format: Literal["str", "markdown", "html"] = Field(default="html")
 
     model_config = ConfigDict(extra="forbid")
 
 
-class PyMuPDFArgs(ParsingArgs):
+class PyMuPDFArgs(BaseModel):
     parsing_algorithm: Literal["pymupdf"] = Field(default="pymupdf")
+    table_output_format: Literal["str", "markdown", "html"] = Field(default="html")
+
+    model_config = ConfigDict(extra="forbid")
+
+
+class UnitableArgs(BaseModel):
+    parsing_algorithm: Literal["unitable"] = Field(default="unitable")
+    min_table_confidence: float = Field(default=0.75, ge=0.0, le=1.0)
+    table_output_format: Literal["html"] = Field(default="html")
 
     model_config = ConfigDict(extra="forbid")
 
 
 def _ingest_with_pymupdf(
     doc: Pdf,
     parsing_args: PyMuPDFArgs,
@@ -78,43 +89,49 @@
     args: TableTransformersArgs,
     verbose: bool = False,
 ) -> List[TableElement]:
     try:
         from openparse.tables.utils import doc_to_imgs
 
         from .table_transformers.ml import find_table_bboxes, get_table_content
-    except ImportError:
+    except ImportError as e:
         raise ImportError(
-            "Table detection and extraction requires the `torch`, `torchvision` and `transformers` libraries to be installed."
+            "Table detection and extraction requires the `torch`, `torchvision` and `transformers` libraries to be installed.",
+            e,
         )
     pdoc = doc.to_pymupdf_doc()  # type: ignore
     pdf_as_imgs = doc_to_imgs(pdoc)
 
     pages_with_tables = {}
     for page_num, img in enumerate(pdf_as_imgs):
         pages_with_tables[page_num] = find_table_bboxes(img, args.min_table_confidence)
 
     tables = []
     for page_num, table_bboxes in pages_with_tables.items():
         page = pdoc[page_num]
         page_dims = (page.rect.width, page.rect.height)
         for table_bbox in table_bboxes:
             table = get_table_content(
-                page_dims, img, table_bbox.bbox, args.min_cell_confidence, verbose
+                page_dims,
+                pdf_as_imgs[page_num],
+                table_bbox.bbox,
+                args.min_cell_confidence,
+                verbose,
             )
             table._run_ocr(page)
 
             if args.table_output_format == "str":
                 table_text = table.to_str()
             elif args.table_output_format == "markdown":
                 table_text = table.to_markdown_str()
             elif args.table_output_format == "html":
                 table_text = table.to_html_str()
 
             # Flip y-coordinates to match the top-left origin system
+            # FIXME: incorporate padding into bbox
             fy0 = page.rect.height - table_bbox.bbox[3]
             fy1 = page.rect.height - table_bbox.bbox[1]
 
             table_elem = TableElement(
                 bbox=Bbox(
                     page=page_num,
                     x0=table_bbox.bbox[0],
@@ -130,18 +147,79 @@
                 print(f"Page {page_num}:\n{table_text}\n")
 
             tables.append(table_elem)
 
     return tables
 
 
+def _ingest_with_unitable(
+    doc: Pdf,
+    args: UnitableArgs,
+    verbose: bool = False,
+) -> List[TableElement]:
+    try:
+        from openparse.tables.utils import doc_to_imgs
+        from .table_transformers.ml import find_table_bboxes
+        from .unitable.core import table_img_to_html
+
+    except ImportError as e:
+        raise ImportError(
+            "Table detection and extraction requires the `torch`, `torchvision` and `transformers` libraries to be installed.",
+            e,
+        )
+    pdoc = doc.to_pymupdf_doc()  # type: ignore
+    pdf_as_imgs = doc_to_imgs(pdoc)
+
+    pages_with_tables = {}
+    for page_num, img in enumerate(pdf_as_imgs):
+        pages_with_tables[page_num] = find_table_bboxes(img, args.min_table_confidence)
+
+    tables = []
+    for page_num, table_bboxes in pages_with_tables.items():
+        page = pdoc[page_num]
+        for table_bbox in table_bboxes:
+            padding_pct = 0.05
+            padded_bbox = adjust_bbox_with_padding(
+                bbox=table_bbox.bbox,
+                page_width=page.rect.width,
+                page_height=page.rect.height,
+                padding_pct=padding_pct,
+            )
+            table_img = crop_img_with_padding(pdf_as_imgs[page_num], padded_bbox)
+
+            table_str = table_img_to_html(table_img)
+
+            # Flip y-coordinates to match the top-left origin system
+            fy0 = page.rect.height - padded_bbox[3]
+            fy1 = page.rect.height - padded_bbox[1]
+
+            table_elem = TableElement(
+                bbox=Bbox(
+                    page=page_num,
+                    x0=padded_bbox[0],
+                    y0=fy0,
+                    x1=padded_bbox[2],
+                    y1=fy1,
+                    page_width=page.rect.width,
+                    page_height=page.rect.height,
+                ),
+                text=table_str,
+            )
+
+            tables.append(table_elem)
+
+    return tables
+
+
 def ingest(
     doc: Pdf,
-    parsing_args: Union[TableTransformersArgs, PyMuPDFArgs, None] = None,
+    parsing_args: Union[TableTransformersArgs, PyMuPDFArgs, UnitableArgs, None] = None,
     verbose: bool = False,
 ) -> List[TableElement]:
     if isinstance(parsing_args, TableTransformersArgs):
         return _ingest_with_table_transformers(doc, parsing_args, verbose)
     elif isinstance(parsing_args, PyMuPDFArgs):
         return _ingest_with_pymupdf(doc, parsing_args, verbose)
+    elif isinstance(parsing_args, UnitableArgs):
+        return _ingest_with_unitable(doc, parsing_args, verbose)
     else:
         raise ValueError("Unsupported parsing_algorithm.")
```

### Comparing `openparse-0.3.1/src/openparse/tables/pymupdf/parse.py` & `openparse-0.4.0/src/openparse/tables/pymupdf/parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.1/src/openparse/tables/schemas.py` & `openparse-0.4.0/src/openparse/tables/schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.1/src/openparse/tables/table_transformers/ml.py` & `openparse-0.4.0/src/openparse/tables/table_transformers/ml.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,32 +4,38 @@
 
 import torch  # type: ignore
 from PIL import Image  # type: ignore
 from torchvision import transforms  # type: ignore
 from transformers import (
     AutoModelForObjectDetection,  # type: ignore
     TableTransformerForObjectDetection,  # type: ignore
-)
+)  # type: ignore
 
 from ..schemas import (
     BBox,
     Size,
+)
+from ..utils import (
+    display_cells_on_img,
+    crop_img_with_padding,
+    convert_croppped_cords_to_full_img_cords,
+    convert_img_cords_to_pdf_cords,
+)
+from .geometry import (
+    calc_bbox_intersection,
+)
+from .schemas import (
+    _TableCellModelOutput,
+    _TableModelOutput,
     _Table,
     _TableDataCell,
     _TableHeader,
     _TableHeaderCell,
     _TableRow,
 )
-from ..utils import display_cells_on_img, crop_img_with_padding
-from .geometry import (
-    calc_bbox_intersection,
-    convert_croppped_cords_to_full_img_cords,
-    convert_img_cords_to_pdf_cords,
-)
-from .schemas import _TableCellModelOutput, _TableModelOutput
 
 t0 = time.time()
 
 cuda_available = torch.cuda.is_available()
 user_preferred_device = "cuda"
 device = torch.device(
     "cuda" if cuda_available and user_preferred_device != "cpu" else "cpu"
@@ -312,21 +318,21 @@
                 if overlap_percentage > overlap_threshold:
                     return True
     return False
 
 
 def get_table_content(
     page_dims: Size,
-    img: Image.Image,
+    page_img: Image.Image,
     table_bbox: BBox,
     min_cell_confidence: float,
     verbose: bool = False,
 ) -> _Table:
     OFFSET = 0.05
-    table_img = crop_img_with_padding(img, table_bbox, padding_pct=OFFSET)
+    table_img = crop_img_with_padding(page_img, table_bbox, padding_pct=OFFSET)
     structure_id2label = {
         **structure_model.config.id2label,
         len(structure_model.config.id2label): "no object",
     }
 
     pixel_values_st = structure_transform(table_img).unsqueeze(0).to("cpu")
     with torch.no_grad():
@@ -334,17 +340,19 @@
 
     cells = _cell_outputs_to_objs(outputs_st, table_img.size, structure_id2label)
 
     for cell in cells:
         cell.bbox = convert_croppped_cords_to_full_img_cords(
             padding_pct=OFFSET,
             cropped_image_size=table_img.size,
-            detection_bbox=cell.bbox,
+            table_bbox=cell.bbox,
             bbox=table_bbox,
         )
 
     if verbose:
-        display_cells_on_img(img, cells, "all", min_cell_confidence=min_cell_confidence)
+        display_cells_on_img(
+            page_img, cells, "all", min_cell_confidence=min_cell_confidence
+        )
 
     return table_from_model_outputs(
-        img, page_dims, table_bbox, cells, min_cell_confidence
+        page_img, page_dims, table_bbox, cells, min_cell_confidence
     )
```

### Comparing `openparse-0.3.1/src/openparse/text/parse.py` & `openparse-0.4.0/src/openparse/text/parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.1/src/openparse/text/pdfminer/core.py` & `openparse-0.4.0/src/openparse/text/pdfminer/core.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.1/src/openparse/text/pymupdf/core.py` & `openparse-0.4.0/src/openparse/text/pymupdf/core.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.1/src/openparse.egg-info/PKG-INFO` & `openparse-0.4.0/src/openparse.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openparse
-Version: 0.3.1
+Version: 0.4.0
 Summary: Streamlines the process of preparing documents for LLM's.
 Home-page: https://github.com/Filimoa/open-parse/
 Author: Sergey Filimonov
 Author-email: hello@sergey.fyi
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyMuPDF>=1.23.2
@@ -13,21 +13,26 @@
 Requires-Dist: pypdf>=4.0.0
 Requires-Dist: pdfminer.six>=20200401
 Requires-Dist: tiktoken>=0.3
 Provides-Extra: ml
 Requires-Dist: torch; extra == "ml"
 Requires-Dist: torchvision; extra == "ml"
 Requires-Dist: transformers; extra == "ml"
+Requires-Dist: tokenizers; extra == "ml"
 
 <p align="center">
     <img src="https://sergey-filimonov.nyc3.digitaloceanspaces.com/open-parse/open-parse-with-text-tp-logo.webp" width="350" />
 </p>
 <br/>
 
-Open-Parse streamlines the process of preparing complex documents for analysis by LLMs. Our goal is to expose state-of-the-art deep learning models with a few lines of code while also providing flexible heuristic options for faster, basic parsing.
+**Easily chunk complex documents the same way a human would.**  
+
+Chunking documents is a challenging task that underpins any RAG system.  High quality results are critical to a sucessful AI application, yet most open-source libraries are limited in their ability to handle complex documents.  
+
+Open Parse is designed to fill this gap by providing a flexible, easy-to-use library capable of visually discerning document layouts and chunking them effectively.
 
 ### Highlights
 
 - **🔍 Visually-Driven:** Open-Parse visually analyzes documents for superior LLM input, going beyond naive text splitting.
 - **✍️ Markdown Support:** Basic markdown support for parsing headings, bold and italics.
 - **📊 High-Precision Table Support:** Extract tables into clean Markdown formats with accuracy that surpasses traditional tools.
 - **🛠️ Extensible:** Easily implement your own post-processing steps.
@@ -45,15 +50,15 @@
 import openparse
 
 basic_doc_path = "./sample-docs/mobile-home-manual.pdf"
 parser = openparse.DocumentParser()
 parsed_basic_doc = parser.parse(basic_doc_path)
 
 for node in parsed_basic_doc.nodes:
-    display(node)
+    print(node)
 ```
 
 **📓 Try the sample notebook** <a href="https://colab.research.google.com/drive/1Z5B5gsnmhFKEFL-5yYIcoox7-jQao8Ep?usp=sharing" class="external-link" target="_blank">here</a>
 
 ## Requirements
 
 Python 3.8+
@@ -101,13 +106,13 @@
 **Note:** _On Windows systems, this must happen outside Python – before starting your script. Just manipulating os.environ will not work!_
 
 #### 2. ML Table Detection (Optional)
 
 This repository provides an optional feature to parse content from tables using the state-of-the-art Table Transformer (DETR) model. The Table Transformer model, introduced in the paper "PubTables-1M: Towards Comprehensive Table Extraction From Unstructured Documents" by Smock et al., achieves best-in-class results for table extraction.
 
 ```console
-pip install "open-parse[ml]"
+pip install "openparse[ml]"
 ```
 
 ## Documentation
 
-_Coming Soon_
+https://filimoa.github.io/open-parse/
```

#### html2text {}

```diff
@@ -1,36 +1,39 @@
-Metadata-Version: 2.1 Name: openparse Version: 0.3.1 Summary: Streamlines the
+Metadata-Version: 2.1 Name: openparse Version: 0.4.0 Summary: Streamlines the
 process of preparing documents for LLM's. Home-page: https://github.com/
 Filimoa/open-parse/ Author: Sergey Filimonov Author-email: hello@sergey.fyi
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 PyMuPDF>=1.23.2 Requires-Dist: pillow>=8.3 Requires-Dist: pydantic>=2.0
 Requires-Dist: pypdf>=4.0.0 Requires-Dist: pdfminer.six>=20200401 Requires-
 Dist: tiktoken>=0.3 Provides-Extra: ml Requires-Dist: torch; extra == "ml"
 Requires-Dist: torchvision; extra == "ml" Requires-Dist: transformers; extra ==
-"ml"
+"ml" Requires-Dist: tokenizers; extra == "ml"
  [https://sergey-filimonov.nyc3.digitaloceanspaces.com/open-parse/open-parse-
                             with-text-tp-logo.webp]
 
-Open-Parse streamlines the process of preparing complex documents for analysis
-by LLMs. Our goal is to expose state-of-the-art deep learning models with a few
-lines of code while also providing flexible heuristic options for faster, basic
-parsing. ### Highlights - **ð Visually-Driven:** Open-Parse visually
-analyzes documents for superior LLM input, going beyond naive text splitting. -
-**âï¸ Markdown Support:** Basic markdown support for parsing headings, bold
-and italics. - **ð High-Precision Table Support:** Extract tables into clean
+**Easily chunk complex documents the same way a human would.** Chunking
+documents is a challenging task that underpins any RAG system. High quality
+results are critical to a sucessful AI application, yet most open-source
+libraries are limited in their ability to handle complex documents. Open Parse
+is designed to fill this gap by providing a flexible, easy-to-use library
+capable of visually discerning document layouts and chunking them effectively.
+### Highlights - **ð Visually-Driven:** Open-Parse visually analyzes
+documents for superior LLM input, going beyond naive text splitting. - **âï¸
+Markdown Support:** Basic markdown support for parsing headings, bold and
+italics. - **ð High-Precision Table Support:** Extract tables into clean
 Markdown formats with accuracy that surpasses traditional tools. - **ð ï¸
 Extensible:** Easily implement your own post-processing steps. -
 **ð¡Intuitive:** Great editor support. Completion everywhere. Less time
 debugging. - **ð¯ Easy:** Designed to be easy to use and learn. Less time
 reading docs.
 [https://sergey-filimonov.nyc3.digitaloceanspaces.com/open-parse/marked-up-doc-
                                     2.webp]
 ## Example ```python import openparse basic_doc_path = "./sample-docs/mobile-
 home-manual.pdf" parser = openparse.DocumentParser() parsed_basic_doc =
-parser.parse(basic_doc_path) for node in parsed_basic_doc.nodes: display(node)
+parser.parse(basic_doc_path) for node in parsed_basic_doc.nodes: print(node)
 ``` **ð Try the sample notebook** _h_e_r_e ## Requirements Python 3.8+ **Dealing
 with PDF's:** - _p_d_f_m_i_n_e_r_._s_i_x Fully open source. **Extracting Tables:** -
 _P_y_M_u_P_D_F has some table detection functionality. Please see their _l_i_c_e_n_s_e. -
 _T_a_b_l_e_ _T_r_a_n_s_f_o_r_m_e_r is a deep learning approach. - _u_n_i_t_a_b_l_e is a more recent deep
 learning approach that seems promising _(coming soon)_ ## Installation #### 1.
 Core Library ```console pip install openparse ``` **Enabling OCR Support**:
 PyMuPDF will already contain all the logic to support OCR functions. But it
@@ -47,9 +50,9 @@
 tesseract-ocr/5/tessdata` **Note:** _On Windows systems, this must happen
 outside Python â before starting your script. Just manipulating os.environ
 will not work!_ #### 2. ML Table Detection (Optional) This repository provides
 an optional feature to parse content from tables using the state-of-the-art
 Table Transformer (DETR) model. The Table Transformer model, introduced in the
 paper "PubTables-1M: Towards Comprehensive Table Extraction From Unstructured
 Documents" by Smock et al., achieves best-in-class results for table
-extraction. ```console pip install "open-parse[ml]" ``` ## Documentation
-_Coming Soon_
+extraction. ```console pip install "openparse[ml]" ``` ## Documentation https:/
+/filimoa.github.io/open-parse/
```

### Comparing `openparse-0.3.1/src/openparse.egg-info/SOURCES.txt` & `openparse-0.4.0/src/openparse.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 README.md
 setup.py
 src/evals/__init__.py
 src/evals/run_evals.py
 src/notebooks/config.py
 src/notebooks/trash.py
 src/openparse/__init__.py
+src/openparse/cli.py
 src/openparse/consts.py
 src/openparse/main.py
 src/openparse/pdf.py
 src/openparse/schemas.py
+src/openparse/types.py
 src/openparse/utils.py
 src/openparse.egg-info/PKG-INFO
 src/openparse.egg-info/SOURCES.txt
 src/openparse.egg-info/dependency_links.txt
+src/openparse.egg-info/entry_points.txt
 src/openparse.egg-info/requires.txt
 src/openparse.egg-info/top_level.txt
 src/openparse/postprocessing/__init__.py
 src/openparse/postprocessing/ingest.py
 src/openparse/postprocessing/steps.py
 src/openparse/processing/__init__.py
 src/openparse/processing/ingest.py
@@ -28,15 +31,22 @@
 src/openparse/tables/utils.py
 src/openparse/tables/pymupdf/__init__.py
 src/openparse/tables/pymupdf/parse.py
 src/openparse/tables/table_transformers/__init__.py
 src/openparse/tables/table_transformers/geometry.py
 src/openparse/tables/table_transformers/ml.py
 src/openparse/tables/table_transformers/schemas.py
-src/openparse/tables/unitable/ml.py
+src/openparse/tables/unitable/__init__.py
+src/openparse/tables/unitable/config.py
+src/openparse/tables/unitable/core.py
+src/openparse/tables/unitable/schemas.py
+src/openparse/tables/unitable/tabular_transformer.py
+src/openparse/tables/unitable/tokens.py
+src/openparse/tables/unitable/unitable_model.py
+src/openparse/tables/unitable/utils.py
 src/openparse/text/__init__.py
 src/openparse/text/parse.py
 src/openparse/text/pdfminer/__init__.py
 src/openparse/text/pdfminer/core.py
 src/openparse/text/pymupdf/__init__.py
 src/openparse/text/pymupdf/core.py
 src/tests/__init__.py
@@ -47,8 +57,11 @@
 src/tests/processing/test_steps.py
 src/tests/tables/__init__.py
 src/tests/tables/pymupdf/__init__.py
 src/tests/tables/pymupdf/test_parse.py
 src/tests/tables/transformers/__init__.py
 src/tests/tables/transformers/test_geometry.py
 src/tests/tables/transformers/test_ml.py
+src/tests/tables/unitable/__init__.py
+src/tests/tables/unitable/sample_pred_outputs.py
+src/tests/tables/unitable/test_pred_to_schema.py
 src/tests/text/pdf_miner/test_core.py
```

### Comparing `openparse-0.3.1/src/tests/processing/test_pipeline.py` & `openparse-0.4.0/src/tests/processing/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.1/src/tests/processing/test_steps.py` & `openparse-0.4.0/src/tests/processing/test_steps.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.1/src/tests/tables/pymupdf/test_parse.py` & `openparse-0.4.0/src/tests/tables/pymupdf/test_parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.1/src/tests/tables/transformers/test_geometry.py` & `openparse-0.4.0/src/tests/tables/transformers/test_geometry.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.1/src/tests/tables/transformers/test_ml.py` & `openparse-0.4.0/src/tests/tables/transformers/test_ml.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.1/src/tests/test_schemas.py` & `openparse-0.4.0/src/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.3.1/src/tests/text/pdf_miner/test_core.py` & `openparse-0.4.0/src/tests/text/pdf_miner/test_core.py`

 * *Files identical despite different names*

