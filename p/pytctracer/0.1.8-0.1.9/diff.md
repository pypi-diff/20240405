# Comparing `tmp/pytctracer-0.1.8.tar.gz` & `tmp/pytctracer-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytctracer-0.1.8.tar", last modified: Wed Apr  3 19:00:10 2024, max compression
+gzip compressed data, was "pytctracer-0.1.9.tar", last modified: Fri Apr  5 16:25:03 2024, max compression
```

## Comparing `pytctracer-0.1.8.tar` & `pytctracer-0.1.9.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-03 19:00:10.185096 pytctracer-0.1.8/
--rw-r--r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1381 2024-04-03 19:00:10.185096 pytctracer-0.1.8/PKG-INFO
--rwxr-xr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)      459 2024-04-03 18:55:36.000000 pytctracer-0.1.8/README.md
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-03 19:00:10.177097 pytctracer-0.1.8/data/
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-03 19:00:10.173097 pytctracer-0.1.8/data/ground-truth-data/
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-03 19:00:10.177097 pytctracer-0.1.8/data/ground-truth-data/pyopenssl/
--rwxr-xr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)    14927 2023-12-12 17:26:56.000000 pytctracer-0.1.8/data/ground-truth-data/pyopenssl/pyopenssl_all_functions.py
--rwxr-xr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)     2737 2024-01-17 14:14:19.000000 pytctracer-0.1.8/data/ground-truth-data/pyopenssl/pyopenssl_chosen_tests.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     2240 2024-03-21 02:03:31.000000 pytctracer-0.1.8/data/t.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      464 2024-02-25 02:21:54.000000 pytctracer-0.1.8/data/tes.py
--rwxr-xr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)    83796 2024-03-28 11:46:42.000000 pytctracer-0.1.8/data/trace_parser_dynamic.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1011 2024-04-03 18:59:47.000000 pytctracer-0.1.8/pyproject.toml
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-03 19:00:10.177097 pytctracer-0.1.8/pytctracer/
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      104 2024-03-31 18:38:21.000000 pytctracer-0.1.8/pytctracer/__init__.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)    19287 2024-03-30 14:21:53.000000 pytctracer-0.1.8/pytctracer/analyser.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     9400 2024-04-01 01:30:08.000000 pytctracer-0.1.8/pytctracer/cli.py
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-03 19:00:10.177097 pytctracer-0.1.8/pytctracer/config/
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)       49 2024-03-30 00:46:49.000000 pytctracer-0.1.8/pytctracer/config/__init__.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      821 2024-03-30 14:16:16.000000 pytctracer-0.1.8/pytctracer/config/config.py
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-03 19:00:10.177097 pytctracer-0.1.8/pytctracer/config/constants/
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      942 2024-03-31 18:39:49.000000 pytctracer-0.1.8/pytctracer/config/constants/__init__.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      181 2024-03-30 00:46:54.000000 pytctracer-0.1.8/pytctracer/config/constants/classification_types.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      383 2024-03-31 18:51:10.000000 pytctracer-0.1.8/pytctracer/config/constants/event_types.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      217 2024-03-31 18:30:31.000000 pytctracer-0.1.8/pytctracer/config/constants/function_types.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      130 2024-03-31 18:51:10.000000 pytctracer-0.1.8/pytctracer/config/constants/instruction_opnames.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      100 2024-03-30 00:46:53.000000 pytctracer-0.1.8/pytctracer/config/constants/level_types.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      203 2024-03-30 00:46:53.000000 pytctracer-0.1.8/pytctracer/config/constants/metric_score_types.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      537 2024-03-30 00:46:52.000000 pytctracer-0.1.8/pytctracer/config/constants/technique_parameters.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      299 2024-03-30 00:46:52.000000 pytctracer-0.1.8/pytctracer/config/constants/technique_thresholds.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      150 2024-03-30 00:46:51.000000 pytctracer-0.1.8/pytctracer/config/constants/testing_method_event_types.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      573 2024-03-31 19:07:44.000000 pytctracer-0.1.8/pytctracer/config/constants/trace_data_headers.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      508 2024-03-31 18:51:10.000000 pytctracer-0.1.8/pytctracer/config/constants/trace_data_variables.py
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-03 19:00:10.177097 pytctracer-0.1.8/pytctracer/evaluation/
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      170 2024-03-26 14:14:33.000000 pytctracer-0.1.8/pytctracer/evaluation/__init__.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1329 2024-03-30 00:47:09.000000 pytctracer-0.1.8/pytctracer/evaluation/classify_predictions.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1238 2024-03-30 00:47:10.000000 pytctracer-0.1.8/pytctracer/evaluation/evaluate_predictions.py
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-03 19:00:10.181097 pytctracer-0.1.8/pytctracer/evaluation/metrics/
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      613 2024-03-30 00:46:46.000000 pytctracer-0.1.8/pytctracer/evaluation/metrics/__init__.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1583 2024-03-30 00:46:45.000000 pytctracer-0.1.8/pytctracer/evaluation/metrics/area_under_curve.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     2967 2024-03-30 00:46:45.000000 pytctracer-0.1.8/pytctracer/evaluation/metrics/arg_name_to_metric_mapper.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      916 2024-03-30 00:46:45.000000 pytctracer-0.1.8/pytctracer/evaluation/metrics/f1.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      991 2024-03-30 00:46:44.000000 pytctracer-0.1.8/pytctracer/evaluation/metrics/false_negatives.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      991 2024-03-30 00:46:44.000000 pytctracer-0.1.8/pytctracer/evaluation/metrics/false_positives.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1472 2024-03-30 00:46:43.000000 pytctracer-0.1.8/pytctracer/evaluation/metrics/mean_average_precision.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      746 2024-03-30 00:46:43.000000 pytctracer-0.1.8/pytctracer/evaluation/metrics/metric.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1086 2024-03-30 00:46:42.000000 pytctracer-0.1.8/pytctracer/evaluation/metrics/precision.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1062 2024-03-30 00:46:42.000000 pytctracer-0.1.8/pytctracer/evaluation/metrics/recall.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      997 2024-03-30 00:46:42.000000 pytctracer-0.1.8/pytctracer/evaluation/metrics/true_positives.py
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-03 19:00:10.181097 pytctracer-0.1.8/pytctracer/io/
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-03-30 00:46:30.000000 pytctracer-0.1.8/pytctracer/io/__init__.py
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-03 19:00:10.181097 pytctracer-0.1.8/pytctracer/io/input/
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      110 2024-03-30 00:46:37.000000 pytctracer-0.1.8/pytctracer/io/input/__init__.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      920 2024-03-30 00:46:37.000000 pytctracer-0.1.8/pytctracer/io/input/from_file.py
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-03 19:00:10.181097 pytctracer-0.1.8/pytctracer/io/output/
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      367 2024-03-30 00:46:35.000000 pytctracer-0.1.8/pytctracer/io/output/__init__.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1714 2024-03-30 00:46:34.000000 pytctracer-0.1.8/pytctracer/io/output/to_display.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1097 2024-03-30 14:22:59.000000 pytctracer-0.1.8/pytctracer/io/output/to_file.py
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-03 19:00:10.181097 pytctracer-0.1.8/pytctracer/parsing/
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1382 2024-03-30 00:46:28.000000 pytctracer-0.1.8/pytctracer/parsing/__init__.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     5336 2024-03-30 00:46:27.000000 pytctracer-0.1.8/pytctracer/parsing/find_class_level_calls.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1285 2024-03-30 14:16:16.000000 pytctracer-0.1.8/pytctracer/parsing/find_class_level_names.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     4768 2024-03-30 00:46:26.000000 pytctracer-0.1.8/pytctracer/parsing/find_function_level_calls.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1225 2024-03-30 14:16:16.000000 pytctracer-0.1.8/pytctracer/parsing/find_function_level_names.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     3431 2024-03-30 00:46:24.000000 pytctracer-0.1.8/pytctracer/parsing/functions_called_before_assert.py
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-03 19:00:10.181097 pytctracer-0.1.8/pytctracer/techniques/
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      883 2024-03-27 16:49:38.000000 pytctracer-0.1.8/pytctracer/techniques/__init__.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     3749 2024-03-30 00:46:03.000000 pytctracer-0.1.8/pytctracer/techniques/arg_name_to_technique_mapper.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1555 2024-03-30 14:18:46.000000 pytctracer-0.1.8/pytctracer/techniques/combined.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     4026 2024-03-30 14:18:43.000000 pytctracer-0.1.8/pytctracer/techniques/last_call_before_assert.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     4742 2024-03-30 14:18:38.000000 pytctracer-0.1.8/pytctracer/techniques/levenshtein_distance.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)    10091 2024-03-30 14:18:34.000000 pytctracer-0.1.8/pytctracer/techniques/longest_common_subsequence.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     6039 2024-03-30 14:17:34.000000 pytctracer-0.1.8/pytctracer/techniques/naming_conventions.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     4621 2024-03-30 14:18:24.000000 pytctracer-0.1.8/pytctracer/techniques/tarantula.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     5544 2024-03-30 14:24:31.000000 pytctracer-0.1.8/pytctracer/techniques/technique.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)    10135 2024-03-30 14:18:30.000000 pytctracer-0.1.8/pytctracer/techniques/tfidf.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)    21018 2024-03-31 20:41:26.000000 pytctracer-0.1.8/pytctracer/tracer.py
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-03 19:00:10.181097 pytctracer-0.1.8/pytctracer.egg-info/
--rw-r--r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1381 2024-04-03 19:00:10.000000 pytctracer-0.1.8/pytctracer.egg-info/PKG-INFO
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     2645 2024-04-03 19:00:10.000000 pytctracer-0.1.8/pytctracer.egg-info/SOURCES.txt
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)        1 2024-04-03 19:00:10.000000 pytctracer-0.1.8/pytctracer.egg-info/dependency_links.txt
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)       50 2024-04-03 19:00:10.000000 pytctracer-0.1.8/pytctracer.egg-info/entry_points.txt
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      145 2024-04-03 19:00:10.000000 pytctracer-0.1.8/pytctracer.egg-info/requires.txt
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)       21 2024-04-03 19:00:10.000000 pytctracer-0.1.8/pytctracer.egg-info/top_level.txt
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)       38 2024-04-03 19:00:10.185096 pytctracer-0.1.8/setup.cfg
+drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.171188 pytctracer-0.1.9/
+-rw-r--r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1789 2024-04-05 16:25:03.171188 pytctracer-0.1.9/PKG-INFO
+-rwxr-xr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)      863 2024-04-05 16:22:58.000000 pytctracer-0.1.9/README.md
+drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.163188 pytctracer-0.1.9/data/
+drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.159188 pytctracer-0.1.9/data/ground-truth-data/
+drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.163188 pytctracer-0.1.9/data/ground-truth-data/pyopenssl/
+-rwxr-xr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)    14927 2023-12-12 17:26:56.000000 pytctracer-0.1.9/data/ground-truth-data/pyopenssl/pyopenssl_all_functions.py
+-rwxr-xr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)     2737 2024-01-17 14:14:19.000000 pytctracer-0.1.9/data/ground-truth-data/pyopenssl/pyopenssl_chosen_tests.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     2240 2024-03-21 02:03:31.000000 pytctracer-0.1.9/data/t.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      464 2024-02-25 02:21:54.000000 pytctracer-0.1.9/data/tes.py
+-rwxr-xr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)    83796 2024-03-28 11:46:42.000000 pytctracer-0.1.9/data/trace_parser_dynamic.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1019 2024-04-05 16:24:32.000000 pytctracer-0.1.9/pyproject.toml
+drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.163188 pytctracer-0.1.9/pytctracer/
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      104 2024-03-31 18:38:21.000000 pytctracer-0.1.9/pytctracer/__init__.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)    19254 2024-04-03 23:07:28.000000 pytctracer-0.1.9/pytctracer/analyser.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     9390 2024-04-03 23:07:08.000000 pytctracer-0.1.9/pytctracer/cli.py
+drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.163188 pytctracer-0.1.9/pytctracer/config/
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)       49 2024-03-30 00:46:49.000000 pytctracer-0.1.9/pytctracer/config/__init__.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      821 2024-03-30 14:16:16.000000 pytctracer-0.1.9/pytctracer/config/config.py
+drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.167188 pytctracer-0.1.9/pytctracer/config/constants/
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      904 2024-04-03 23:07:54.000000 pytctracer-0.1.9/pytctracer/config/constants/__init__.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      180 2024-04-03 23:05:28.000000 pytctracer-0.1.9/pytctracer/config/constants/classification_type.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      380 2024-04-03 23:05:47.000000 pytctracer-0.1.9/pytctracer/config/constants/event_type.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      216 2024-04-03 23:05:58.000000 pytctracer-0.1.9/pytctracer/config/constants/function_type.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      129 2024-04-03 23:06:06.000000 pytctracer-0.1.9/pytctracer/config/constants/instruction_opname.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)       99 2024-04-03 23:07:08.000000 pytctracer-0.1.9/pytctracer/config/constants/level_type.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      202 2024-04-03 23:07:13.000000 pytctracer-0.1.9/pytctracer/config/constants/metric_score_type.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      535 2024-04-03 23:07:28.000000 pytctracer-0.1.9/pytctracer/config/constants/technique_parameter.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      298 2024-04-03 23:07:36.000000 pytctracer-0.1.9/pytctracer/config/constants/technique_threshold.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      149 2024-04-03 23:07:44.000000 pytctracer-0.1.9/pytctracer/config/constants/testing_method_event_type.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      572 2024-04-03 23:07:50.000000 pytctracer-0.1.9/pytctracer/config/constants/trace_data_header.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      507 2024-04-03 23:07:54.000000 pytctracer-0.1.9/pytctracer/config/constants/trace_data_variable.py
+drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.167188 pytctracer-0.1.9/pytctracer/evaluation/
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      170 2024-03-26 14:14:33.000000 pytctracer-0.1.9/pytctracer/evaluation/__init__.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1325 2024-04-03 23:05:28.000000 pytctracer-0.1.9/pytctracer/evaluation/classify_predictions.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1234 2024-04-03 23:07:13.000000 pytctracer-0.1.9/pytctracer/evaluation/evaluate_predictions.py
+drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.167188 pytctracer-0.1.9/pytctracer/evaluation/metrics/
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      613 2024-03-30 00:46:46.000000 pytctracer-0.1.9/pytctracer/evaluation/metrics/__init__.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1581 2024-04-03 23:07:13.000000 pytctracer-0.1.9/pytctracer/evaluation/metrics/area_under_curve.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     2967 2024-03-30 00:46:45.000000 pytctracer-0.1.9/pytctracer/evaluation/metrics/arg_name_to_metric_mapper.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      914 2024-04-03 23:07:13.000000 pytctracer-0.1.9/pytctracer/evaluation/metrics/f1.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      989 2024-04-03 23:07:13.000000 pytctracer-0.1.9/pytctracer/evaluation/metrics/false_negatives.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      989 2024-04-03 23:07:13.000000 pytctracer-0.1.9/pytctracer/evaluation/metrics/false_positives.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1470 2024-04-03 23:07:13.000000 pytctracer-0.1.9/pytctracer/evaluation/metrics/mean_average_precision.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      744 2024-04-03 23:07:13.000000 pytctracer-0.1.9/pytctracer/evaluation/metrics/metric.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1084 2024-04-03 23:07:13.000000 pytctracer-0.1.9/pytctracer/evaluation/metrics/precision.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1060 2024-04-03 23:07:13.000000 pytctracer-0.1.9/pytctracer/evaluation/metrics/recall.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      995 2024-04-03 23:07:13.000000 pytctracer-0.1.9/pytctracer/evaluation/metrics/true_positives.py
+drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.167188 pytctracer-0.1.9/pytctracer/io/
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-03-30 00:46:30.000000 pytctracer-0.1.9/pytctracer/io/__init__.py
+drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.167188 pytctracer-0.1.9/pytctracer/io/input/
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      110 2024-03-30 00:46:37.000000 pytctracer-0.1.9/pytctracer/io/input/__init__.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      920 2024-03-30 00:46:37.000000 pytctracer-0.1.9/pytctracer/io/input/from_file.py
+drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.167188 pytctracer-0.1.9/pytctracer/io/output/
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      367 2024-03-30 00:46:35.000000 pytctracer-0.1.9/pytctracer/io/output/__init__.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1714 2024-03-30 00:46:34.000000 pytctracer-0.1.9/pytctracer/io/output/to_display.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1097 2024-03-30 14:22:59.000000 pytctracer-0.1.9/pytctracer/io/output/to_file.py
+drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.167188 pytctracer-0.1.9/pytctracer/parsing/
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1382 2024-03-30 00:46:28.000000 pytctracer-0.1.9/pytctracer/parsing/__init__.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     5292 2024-04-03 23:07:50.000000 pytctracer-0.1.9/pytctracer/parsing/find_class_level_calls.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1274 2024-04-03 23:07:50.000000 pytctracer-0.1.9/pytctracer/parsing/find_class_level_names.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     4728 2024-04-03 23:07:50.000000 pytctracer-0.1.9/pytctracer/parsing/find_function_level_calls.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1214 2024-04-03 23:07:50.000000 pytctracer-0.1.9/pytctracer/parsing/find_function_level_names.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     3403 2024-04-03 23:07:50.000000 pytctracer-0.1.9/pytctracer/parsing/functions_called_before_assert.py
+drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.171188 pytctracer-0.1.9/pytctracer/techniques/
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      883 2024-03-27 16:49:38.000000 pytctracer-0.1.9/pytctracer/techniques/__init__.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     3749 2024-03-30 00:46:03.000000 pytctracer-0.1.9/pytctracer/techniques/arg_name_to_technique_mapper.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1553 2024-04-03 23:07:36.000000 pytctracer-0.1.9/pytctracer/techniques/combined.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     4021 2024-04-03 23:07:28.000000 pytctracer-0.1.9/pytctracer/techniques/last_call_before_assert.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     4735 2024-04-03 23:07:36.000000 pytctracer-0.1.9/pytctracer/techniques/levenshtein_distance.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)    10083 2024-04-03 23:07:36.000000 pytctracer-0.1.9/pytctracer/techniques/longest_common_subsequence.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     6032 2024-04-03 23:07:28.000000 pytctracer-0.1.9/pytctracer/techniques/naming_conventions.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     4613 2024-04-03 23:07:37.000000 pytctracer-0.1.9/pytctracer/techniques/tarantula.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     5544 2024-03-30 14:24:31.000000 pytctracer-0.1.9/pytctracer/techniques/technique.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)    10121 2024-04-03 23:07:37.000000 pytctracer-0.1.9/pytctracer/techniques/tfidf.py
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)    20952 2024-04-03 23:07:54.000000 pytctracer-0.1.9/pytctracer/tracer.py
+drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.171188 pytctracer-0.1.9/pytctracer.egg-info/
+-rw-r--r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1789 2024-04-05 16:25:03.000000 pytctracer-0.1.9/pytctracer.egg-info/PKG-INFO
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     2634 2024-04-05 16:25:03.000000 pytctracer-0.1.9/pytctracer.egg-info/SOURCES.txt
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)        1 2024-04-05 16:25:03.000000 pytctracer-0.1.9/pytctracer.egg-info/dependency_links.txt
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)       50 2024-04-05 16:25:03.000000 pytctracer-0.1.9/pytctracer.egg-info/entry_points.txt
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      145 2024-04-05 16:25:03.000000 pytctracer-0.1.9/pytctracer.egg-info/requires.txt
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)       21 2024-04-05 16:25:03.000000 pytctracer-0.1.9/pytctracer.egg-info/top_level.txt
+-rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)       38 2024-04-05 16:25:03.171188 pytctracer-0.1.9/setup.cfg
```

### Comparing `pytctracer-0.1.8/PKG-INFO` & `pytctracer-0.1.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pytctracer
-Version: 0.1.8
-Summary: CLI tool demonstrating test-to-code traceability techniques on Python codebases that use the Pytest testing framework.
+Version: 0.1.9
+Summary: Research library demonstrating test-to-code traceability techniques on Python codebases that use the Pytest testing framework.
 Author: Jason Ho
 Project-URL: Repository, https://github.com/jasonho2582001/comp0138-pytctracer
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -20,8 +20,12 @@
 Requires-Dist: pylint==3.1.0; extra == "dev"
 Requires-Dist: setuptools==69.2.0; extra == "dev"
 Requires-Dist: bump2version==1.0.1; extra == "dev"
 
 # PyTCTracer
 PyTCTracer is a test-to-code traceability approach and library, which allows for dynamic code tracing of Python repositories using the Pytest testing framework, and automatic generation of test-to-code traceability links from the trace data using a number of established traceability techniques. 
 
+There are two core components in the library:
+- `PytestTracer`: A class that is used to trace the execution of Pytest unit tests and record dynamic tracing information to a CSV log file.
+- `pytctracer` CLI: A CLI tool which can read and parse the dynamic information from the log file, apply traceability techniques to generate link predictions, and evaluate the predictions against a ground truth.
+
 This library forms part of an undergraduate research project for a Masters of Engineering in Computer Science at UCL (University College London).
```

### Comparing `pytctracer-0.1.8/data/ground-truth-data/pyopenssl/pyopenssl_all_functions.py` & `pytctracer-0.1.9/data/ground-truth-data/pyopenssl/pyopenssl_all_functions.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.8/data/ground-truth-data/pyopenssl/pyopenssl_chosen_tests.py` & `pytctracer-0.1.9/data/ground-truth-data/pyopenssl/pyopenssl_chosen_tests.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.8/data/t.py` & `pytctracer-0.1.9/data/t.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.8/data/trace_parser_dynamic.py` & `pytctracer-0.1.9/data/trace_parser_dynamic.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.8/pyproject.toml` & `pytctracer-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 authors = [
   {name = "Jason Ho"}
 ]
-description = """CLI tool demonstrating test-to-code traceability techniques on Python codebases that use the Pytest testing framework."""
+description = """Research library demonstrating test-to-code traceability techniques on Python codebases that use the Pytest testing framework."""
 readme = "README.md"
 name = "pytctracer"
-version = "0.1.8"
+version = "0.1.9"
 classifiers=[
     "Natural Language :: English",
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
```

### Comparing `pytctracer-0.1.8/pytctracer/analyser.py` & `pytctracer-0.1.9/pytctracer/analyser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Optional, Dict, Any, Tuple, Set
 from click import ClickException
-from pytctracer.config.constants import LevelTypes, TechniqueParameters
+from pytctracer.config.constants import LevelType, TechniqueParameter
 from pytctracer.config import Config
 from pytctracer.io.input import read_trace_csv_log, load_link_json
 from pytctracer.io.output import (
     display_predicted_links,
     write_dict_to_json,
     write_evaluation_metrics_to_csv,
     display_evaluation_results,
@@ -103,15 +103,15 @@
                     f"Test '{test}' in ground truth but not in predicted links"
                 )
 
     def evaluate_traceability_links_for_trace(
         self,
         trace_csv_log_path: str,
         ground_truth_path: str,
-        traceability_level: LevelTypes,
+        traceability_level: LevelType,
         add_combined_technique: bool = False,
         chosen_technique_names: Optional[List[str]] = None,
         chosen_metric_names: Optional[List[str]] = None,
         classifications_output_directory_path: Optional[str] = None,
         evaluation_metrics_output_path: Optional[str] = None,
         display_classifications_to_stdout: bool = False,
         metric_as_percentage: bool = False,
@@ -166,15 +166,15 @@
                 combined_evaluation_dict=evaluation_metrics_for_techniques,
                 csv_name=evaluation_metrics_output_path,
             )
 
     def produce_traceability_links_for_trace(
         self,
         trace_csv_log_path: str,
-        traceability_level: LevelTypes,
+        traceability_level: LevelType,
         add_combined_technique: bool = False,
         chosen_technique_names: Optional[List[str]] = None,
         prediction_output_directory_path: Optional[str] = None,
     ) -> int:
         if not chosen_technique_names:
             chosen_technique_names = self.default_technique_names
         _, link_predictions_for_techniques = self._predict_links(
@@ -194,23 +194,23 @@
                 traceability_level,
             )
 
     def _write_classifications_for_techniques(
         self,
         classifications_for_techniques: Dict[str, Dict[str, List[str]]],
         classifications_output_directory_path: str,
-        traceability_level: LevelTypes,
+        traceability_level: LevelType,
     ) -> None:
         for (
             technique_arg_name,
             classifications,
         ) in classifications_for_techniques.items():
             technique_arg_name = technique_arg_name.replace("-", "_")
-            file_path = f"""{classifications_output_directory_path}/
-            {technique_arg_name}_{traceability_level.lower()}_classifications.json"""
+            file_path = f"{classifications_output_directory_path}/
+            {technique_arg_name}_{traceability_level.lower()}_classifications.json"
             write_dict_to_json(classifications, file_path)
 
     def _display_classifications_for_techniques(
         self, classifications_for_techniques: Dict[str, Dict[str, List[str]]]
     ) -> None:
         for (
             technique_arg_name,
@@ -280,19 +280,19 @@
 
         return evaluation_metrics_for_techniques
 
     def _predict_links(
         self,
         trace_csv_log_path: str,
         chosen_technique_names: List[str],
-        traceability_level: LevelTypes,
+        traceability_level: LevelType,
         add_combined_technique: bool,
         test_to_create_links_for: Optional[Set[str]] = None,
     ) -> Tuple[Dict[str, Dict[str, Dict[str, float]]], Dict[str, Dict[str, List[str]]]]:
-        if traceability_level == LevelTypes.FUNCTION:
+        if traceability_level == LevelType.FUNCTION:
             technique_parameter_map = self._parse_function_level_data(
                 trace_csv_log_path
             )
         else:
             technique_parameter_map = self._parse_class_level_data(trace_csv_log_path)
         traceability_scores_for_techniques = self._run_technique_scoring(
             chosen_technique_names=chosen_technique_names,
@@ -321,23 +321,23 @@
 
         return traceability_scores_for_techniques, link_predictions_for_techniques
 
     def _write_predicted_links_for_techniques(
         self,
         link_predictions_for_techniques: Dict[str, Dict[str, List[str]]],
         prediction_output_directory_path: str,
-        traceability_level: LevelTypes,
+        traceability_level: LevelType,
     ) -> None:
         for (
             technique_arg_name,
             link_predictions,
         ) in link_predictions_for_techniques.items():
             technique_arg_name = technique_arg_name.replace("-", "_")
-            file_path = f"""{prediction_output_directory_path}/
-            {technique_arg_name}_{traceability_level.lower()}_predicted_links.json"""
+            file_path = f"{prediction_output_directory_path}/
+            {technique_arg_name}_{traceability_level.lower()}_predicted_links.json"
             write_dict_to_json(link_predictions, file_path)
 
     def _display_predicted_links_for_techniques(
         self, link_predictions_for_techniques: Dict[str, Dict[str, List[str]]]
     ) -> None:
         for (
             technique_arg_name,
@@ -368,15 +368,15 @@
             link_predictions_for_technqiues[technique_arg_name] = link_predictions
 
         return link_predictions_for_technqiues
 
     def _run_technique_scoring(
         self,
         chosen_technique_names: List[str],
-        technique_parameter_map: Dict[TechniqueParameters, Any],
+        technique_parameter_map: Dict[TechniqueParameter, Any],
     ) -> Dict[str, Dict[str, Dict[str, float]]]:
         traceability_scores_for_techniques = {}
         for technique_arg_name in chosen_technique_names:
             technique = self.arg_name_to_technique_map.get_technique(
                 technique_arg_name
             )()
 
@@ -388,39 +388,39 @@
             traceability_scores = technique.run(**technique_parameters)
             traceability_scores_for_techniques[technique_arg_name] = traceability_scores
 
         return traceability_scores_for_techniques
 
     def _parse_function_level_data(
         self, trace_csv_log_path: str
-    ) -> Dict[TechniqueParameters, Any]:
+    ) -> Dict[TechniqueParameter, Any]:
         trace_data = read_trace_csv_log(trace_csv_log_path)
         function_names_tuple = find_function_names_tuple(trace_data)
         test_names_tuple = find_test_names_tuple(trace_data)
         functions_called_by_test = find_functions_called_by_test(trace_data)
         functions_called_by_test_count = find_functions_called_by_test_count(trace_data)
         functions_called_by_test_depth = find_functions_called_by_test_depth(trace_data)
         functions_called_by_test_before_assert = (
             find_functions_called_before_assert_for_each_test(trace_data)
         )
         tests_that_call_function = find_tests_that_call_function(trace_data)
 
         return {
-            TechniqueParameters.FUNCTION_NAMES_TUPLE: function_names_tuple,
-            TechniqueParameters.TEST_NAMES_TUPLE: test_names_tuple,
-            TechniqueParameters.FUNCTIONS_CALLED_BY_TESTS: functions_called_by_test,
-            TechniqueParameters.FUNCTIONS_CALLED_BY_TEST_COUNT: functions_called_by_test_count,
-            TechniqueParameters.FUNCTIONS_CALLED_BY_TEST_DEPTH: functions_called_by_test_depth,
-            TechniqueParameters.FUNCTIONS_CALLED_BY_TEST_BEFORE_ASSERT: functions_called_by_test_before_assert,
-            TechniqueParameters.TESTS_THAT_CALL_FUNCTIONS: tests_that_call_function,
+            TechniqueParameter.FUNCTION_NAMES_TUPLE: function_names_tuple,
+            TechniqueParameter.TEST_NAMES_TUPLE: test_names_tuple,
+            TechniqueParameter.FUNCTIONS_CALLED_BY_TESTS: functions_called_by_test,
+            TechniqueParameter.FUNCTIONS_CALLED_BY_TEST_COUNT: functions_called_by_test_count,
+            TechniqueParameter.FUNCTIONS_CALLED_BY_TEST_DEPTH: functions_called_by_test_depth,
+            TechniqueParameter.FUNCTIONS_CALLED_BY_TEST_BEFORE_ASSERT: functions_called_by_test_before_assert,
+            TechniqueParameter.TESTS_THAT_CALL_FUNCTIONS: tests_that_call_function,
         }
 
     def _parse_class_level_data(
         self, trace_csv_log_path: str
-    ) -> Dict[TechniqueParameters, Any]:
+    ) -> Dict[TechniqueParameter, Any]:
         trace_data = read_trace_csv_log(trace_csv_log_path)
         function_class_names_tuple = find_function_class_names_tuple(trace_data)
         test_class_names_tuple = find_test_class_names_tuple(trace_data)
         functions_called_by_test_class = find_function_classes_called_by_test(
             trace_data
         )
         functions_called_by_test_class_count = (
@@ -433,18 +433,18 @@
             find_classes_called_before_assert_for_each_test(trace_data)
         )
         tests_that_call_function_classes = find_tests_that_call_function_classes(
             trace_data
         )
 
         return {
-            TechniqueParameters.FUNCTION_NAMES_TUPLE: function_class_names_tuple,
-            TechniqueParameters.TEST_NAMES_TUPLE: test_class_names_tuple,
-            TechniqueParameters.FUNCTIONS_CALLED_BY_TESTS: functions_called_by_test_class,
-            TechniqueParameters.FUNCTIONS_CALLED_BY_TEST_COUNT: functions_called_by_test_class_count,
-            TechniqueParameters.FUNCTIONS_CALLED_BY_TEST_DEPTH: functions_called_by_test_class_depth,
-            TechniqueParameters.FUNCTIONS_CALLED_BY_TEST_BEFORE_ASSERT: functions_called_by_test_class_before_assert,
-            TechniqueParameters.TESTS_THAT_CALL_FUNCTIONS: tests_that_call_function_classes,
+            TechniqueParameter.FUNCTION_NAMES_TUPLE: function_class_names_tuple,
+            TechniqueParameter.TEST_NAMES_TUPLE: test_class_names_tuple,
+            TechniqueParameter.FUNCTIONS_CALLED_BY_TESTS: functions_called_by_test_class,
+            TechniqueParameter.FUNCTIONS_CALLED_BY_TEST_COUNT: functions_called_by_test_class_count,
+            TechniqueParameter.FUNCTIONS_CALLED_BY_TEST_DEPTH: functions_called_by_test_class_depth,
+            TechniqueParameter.FUNCTIONS_CALLED_BY_TEST_BEFORE_ASSERT: functions_called_by_test_class_before_assert,
+            TechniqueParameter.TESTS_THAT_CALL_FUNCTIONS: tests_that_call_function_classes,
         }
 
 
 __all__ = ["Analyser"]
```

### Comparing `pytctracer-0.1.8/pytctracer/cli.py` & `pytctracer-0.1.9/pytctracer/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Tuple, Optional
 import click
 from pytctracer import Analyser
 from pytctracer.config import Config
-from pytctracer.config.constants import LevelTypes
+from pytctracer.config.constants import LevelType
 
 
 @click.group(
     "pytctracer",
     help="""CLI for producing, analysing and comparing test-to-code
     traceability links for Python projects using the Pytest framework.""",
 )
@@ -32,16 +32,16 @@
     type=click.Choice(Config.SELECTABLE_TECHNIQUE_NAMES),
     multiple=True,
     help="""Use a specified technique (can be multiple of this flag). 
     If omitted, all selectable techniques are used by default.""",
 )
 @click.option(
     "--level",
-    type=click.Choice([LevelTypes.FUNCTION, LevelTypes.CLASS]),
-    default=LevelTypes.FUNCTION,
+    type=click.Choice([LevelType.FUNCTION, LevelType.CLASS]),
+    default=LevelType.FUNCTION,
     help="""What level of traceability to produce links for (function or class). 
     If omitted, links are produced at the function level by default.""",
 )
 @click.option(
     "--add-combined",
     is_flag=True,
     default=False,
@@ -102,16 +102,16 @@
     type=click.Choice(Config.SELECTABLE_METRIC_NAMES),
     multiple=True,
     help="""Use a specified evaluation metric (can be multiple of this flag). If omitted,
     all selectable metrics are used by default.""",
 )
 @click.option(
     "--level",
-    type=click.Choice([LevelTypes.FUNCTION, LevelTypes.CLASS]),
-    default=LevelTypes.FUNCTION,
+    type=click.Choice([LevelType.FUNCTION, LevelType.CLASS]),
+    default=LevelType.FUNCTION,
     help="""What level of traceability to produce links for (function or class).
     If omitted, links are produced at the function level by default.""",
 )
 @click.option(
     "--add-combined",
     is_flag=True,
     default=False,
@@ -191,16 +191,16 @@
 @click.option(
     "--metric", type=click.Choice(Config.SELECTABLE_METRIC_NAMES), multiple=True,
     help="""Use a specified evaluation metric (can be multiple of this flag). If omitted,
     all selectable metrics are used by default.""",
 )
 @click.option(
     "--level",
-    type=click.Choice([LevelTypes.FUNCTION, LevelTypes.CLASS]),
-    default=LevelTypes.FUNCTION,
+    type=click.Choice([LevelType.FUNCTION, LevelType.CLASS]),
+    default=LevelType.FUNCTION,
     help="""What level of traceability to produce links for (function or class).
     If omitted, links are produced at the function level by default.""",
 )
 @click.option(
     "--as-percentage",
     is_flag=True,
     default=False,
```

### Comparing `pytctracer-0.1.8/pytctracer/config/config.py` & `pytctracer-0.1.9/pytctracer/config/config.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.8/pytctracer/config/constants/__init__.py` & `pytctracer-0.1.9/pytctracer/config/constants/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from .technique_parameters import TechniqueParameters
-from .testing_method_event_types import TestingMethodTypes
-from .trace_data_headers import TraceDataHeaders
-from .event_types import EventTypes, SetTraceEventTypes, SetProfileCEventTypes
-from .function_types import FunctionTypes
-from .metric_score_types import MetricScoreTypes
-from .classification_types import ClassificationTypes
-from .level_types import LevelTypes
-from .technique_thresholds import TechniqueThresholds
-from .trace_data_variables import TraceDataVariables
-from .instruction_opnames import InstructionOpnames
+from .technique_parameter import TechniqueParameter
+from .testing_method_event_type import TestingMethodType
+from .trace_data_header import TraceDataHeader
+from .event_type import EventType, SetTraceEventType, SetProfileCEventType
+from .function_type import FunctionType
+from .metric_score_type import MetricScoreType
+from .classification_type import ClassificationType
+from .level_type import LevelType
+from .technique_threshold import TechniqueThreshold
+from .trace_data_variable import TraceDataVariable
+from .instruction_opname import InstructionOpname
 
 __all__ = [
-    "TechniqueParameters",
-    "TestingMethodTypes",
-    "TraceDataHeaders",
-    "EventTypes",
-    "FunctionTypes",
-    "TechniqueThresholds",
-    "MetricScoreTypes",
-    "ClassificationTypes",
-    "LevelTypes",
-    "TechniqueThresholds",
-    "TraceDataVariables",
-    "SetTraceEventTypes",
-    "SetProfileCEventTypes",
-    "InstructionOpnames",
+    "TechniqueParameter",
+    "TestingMethodType",
+    "TraceDataHeader",
+    "EventType",
+    "FunctionType",
+    "TechniqueThreshold",
+    "MetricScoreType",
+    "ClassificationType",
+    "LevelType",
+    "TechniqueThreshold",
+    "TraceDataVariable",
+    "SetTraceEventType",
+    "SetProfileCEventType",
+    "InstructionOpname",
 ]
```

### Comparing `pytctracer-0.1.8/pytctracer/config/constants/technique_parameters.py` & `pytctracer-0.1.9/pytctracer/config/constants/technique_parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import StrEnum
 
 
-class TechniqueParameters(StrEnum):
+class TechniqueParameter(StrEnum):
     FUNCTION_NAMES_TUPLE = "function_names_tuple"
     TEST_NAMES_TUPLE = "test_names_tuple"
     TESTS_THAT_CALL_FUNCTIONS = "tests_that_call_functions"
     FUNCTIONS_CALLED_BY_TESTS = "functions_called_by_tests"
     FUNCTIONS_CALLED_BY_TEST_COUNT = "functions_called_by_test_count"
     FUNCTIONS_CALLED_BY_TEST_DEPTH = "functions_called_by_test_depth"
     FUNCTIONS_CALLED_BY_TEST_BEFORE_ASSERT = "functions_called_by_test_before_assert"
 
 
-__all__ = ["TechniqueParameters"]
+__all__ = ["TechniqueParameter"]
```

### Comparing `pytctracer-0.1.8/pytctracer/config/constants/trace_data_headers.py` & `pytctracer-0.1.9/pytctracer/config/constants/trace_data_header.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import StrEnum
 
 
-class TraceDataHeaders(StrEnum):
+class TraceDataHeader(StrEnum):
     DEPTH = "Depth"
     FUNCTION_TYPE = "Function Type"
     TESTNG_METHOD = "Testing Method"
     FUNCTION_NAME = "Function Name"
     FULLY_QUALIFIED_FUNCTION_NAME = "Fully Qualified Function Name"
     CLASS_NAME = "Class Name"
     FULLY_QUALIFIED_CLASS_NAME = "Fully Qualified Class Name"
```

### Comparing `pytctracer-0.1.8/pytctracer/evaluation/classify_predictions.py` & `pytctracer-0.1.9/pytctracer/evaluation/classify_predictions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, List
 from collections import defaultdict
-from pytctracer.config.constants import ClassificationTypes
+from pytctracer.config.constants import ClassificationType
 
 
 def classify_predictions(
     predicted_links: Dict[str, List[str]], ground_truth_links: Dict[str, List[str]]
 ) -> Dict[str, Dict[str, List[str]]]:
     classification_dict = defaultdict(dict)
 
@@ -15,20 +15,20 @@
         true_positive_set = predicted_links_for_test.intersection(
             ground_truth_links_for_test
         )
         false_positive_set = predicted_links_for_test - ground_truth_links_for_test
         false_negatives_set = ground_truth_links_for_test - predicted_links_for_test
 
         classification_dict[fully_qualified_test_name][
-            ClassificationTypes.TRUE_POSITIVES
+            ClassificationType.TRUE_POSITIVES
         ] = list(true_positive_set)
         classification_dict[fully_qualified_test_name][
-            ClassificationTypes.FALSE_POSITIVES
+            ClassificationType.FALSE_POSITIVES
         ] = list(false_positive_set)
         classification_dict[fully_qualified_test_name][
-            ClassificationTypes.FALSE_NEGATIVES
+            ClassificationType.FALSE_NEGATIVES
         ] = list(false_negatives_set)
 
     return classification_dict
 
 
 __all__ = ["classify_predictions"]
```

### Comparing `pytctracer-0.1.8/pytctracer/evaluation/evaluate_predictions.py` & `pytctracer-0.1.9/pytctracer/evaluation/evaluate_predictions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from typing import Dict, List, Optional
 from pytctracer.evaluation.metrics import Metric
-from pytctracer.config.constants import MetricScoreTypes
+from pytctracer.config.constants import MetricScoreType
 
 
 def evaluate_predictions(
     predicted_links: Dict[str, List[str]],
     ground_truth_links: Dict[str, List[str]],
     selected_metrics: List[Metric],
     traceability_score_dict: Optional[Dict[str, Dict[str, float]]] = None,
     metric_as_percentage: bool = False,
     uses_threshold: bool = True,
 ) -> Dict[str, float]:
     evaluation_dict = {}
     for metric in selected_metrics:
-        if metric.metric_type == MetricScoreTypes.THRESHOLD_INDEPENDENT and (
+        if metric.metric_type == MetricScoreType.THRESHOLD_INDEPENDENT and (
             not uses_threshold or traceability_score_dict is None
         ):
             metric_result = 0
         else:
             metric_result = metric.calculate(
                 predicted_links, ground_truth_links, traceability_score_dict
             )
             if metric_as_percentage and metric.metric_type in [
-                MetricScoreTypes.CONTINUOUS,
-                MetricScoreTypes.THRESHOLD_INDEPENDENT,
+                MetricScoreType.CONTINUOUS,
+                MetricScoreType.THRESHOLD_INDEPENDENT,
             ]:
                 metric_result = metric.to_percentage(metric_result)
 
         evaluation_dict[metric.arg_name] = metric_result
 
     return evaluation_dict
```

### Comparing `pytctracer-0.1.8/pytctracer/evaluation/metrics/__init__.py` & `pytctracer-0.1.9/pytctracer/evaluation/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.8/pytctracer/evaluation/metrics/area_under_curve.py` & `pytctracer-0.1.9/pytctracer/evaluation/metrics/area_under_curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Dict, List, Optional
 from sklearn.metrics import precision_recall_curve, auc
-from pytctracer.config.constants import MetricScoreTypes
+from pytctracer.config.constants import MetricScoreType
 from pytctracer.evaluation.metrics.metric import Metric
 
 
 class AreaUnderCurve(Metric):
     full_name = "Area Under Curve"
     short_name = "AUC"
     arg_name = "auc"
-    metric_type = MetricScoreTypes.THRESHOLD_INDEPENDENT
+    metric_type = MetricScoreType.THRESHOLD_INDEPENDENT
 
     def calculate(
         self,
         _: Dict[str, List[str]],
         ground_truth_links: Dict[str, List[str]],
         traceability_score_dict: Optional[Dict[str, Dict[str, float]]] = None,
     ) -> float:
```

### Comparing `pytctracer-0.1.8/pytctracer/evaluation/metrics/arg_name_to_metric_mapper.py` & `pytctracer-0.1.9/pytctracer/evaluation/metrics/arg_name_to_metric_mapper.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.8/pytctracer/evaluation/metrics/f1.py` & `pytctracer-0.1.9/pytctracer/evaluation/metrics/f1.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Dict, List, Optional
-from pytctracer.config.constants import MetricScoreTypes
+from pytctracer.config.constants import MetricScoreType
 from pytctracer.evaluation.metrics.metric import Metric
 from pytctracer.evaluation.metrics.precision import Precision
 from pytctracer.evaluation.metrics.recall import Recall
 
 
 class F1(Metric):
     full_name = "F1"
     short_name = "F1"
     arg_name = "f1"
-    metric_type = MetricScoreTypes.CONTINUOUS
+    metric_type = MetricScoreType.CONTINUOUS
 
     def calculate(
         self,
         predicted_links: Dict[str, List[str]],
         ground_truth_links: Dict[str, List[str]],
         _: Optional[Dict[str, Dict[str, float]]] = None,
     ) -> float:
```

### Comparing `pytctracer-0.1.8/pytctracer/evaluation/metrics/false_negatives.py` & `pytctracer-0.1.9/pytctracer/evaluation/metrics/true_positives.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from typing import Dict, List, Optional
-from pytctracer.config.constants import MetricScoreTypes
+from pytctracer.config.constants import MetricScoreType
 from pytctracer.evaluation.metrics.metric import Metric
 
 
-class FalseNegatives(Metric):
-    full_name = "False Negatives"
-    short_name = "FN"
-    arg_name = "fn"
-    metric_type = MetricScoreTypes.INTEGER
+class TruePositives(Metric):
+    full_name = "True Positives"
+    short_name = "TP"
+    arg_name = "tp"
+    metric_type = MetricScoreType.INTEGER
 
     def calculate(
         self,
         predicted_links: Dict[str, List[str]],
         ground_truth_links: Dict[str, List[str]],
         _: Optional[Dict[str, Dict[str, float]]] = None,
     ) -> float:
-        false_negatives = 0
+        true_positives = 0
         for fully_qualified_test_name in ground_truth_links:
             predicted_links_for_test = set(predicted_links[fully_qualified_test_name])
             ground_truth_links_for_test = set(
                 ground_truth_links[fully_qualified_test_name]
             )
-            false_negatives += len(
-                ground_truth_links_for_test - predicted_links_for_test
+            true_positives += len(
+                predicted_links_for_test.intersection(ground_truth_links_for_test)
             )
 
-        return false_negatives
+        return true_positives
 
 
-__all__ = ["FalseNegatives"]
+__all__ = ["TruePositives"]
```

### Comparing `pytctracer-0.1.8/pytctracer/evaluation/metrics/false_positives.py` & `pytctracer-0.1.9/pytctracer/evaluation/metrics/false_positives.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Dict, List, Optional
-from pytctracer.config.constants import MetricScoreTypes
+from pytctracer.config.constants import MetricScoreType
 from pytctracer.evaluation.metrics.metric import Metric
 
 
 class FalsePositives(Metric):
     full_name = "False Positives"
     short_name = "FN"
     arg_name = "fp"
-    metric_type = MetricScoreTypes.INTEGER
+    metric_type = MetricScoreType.INTEGER
 
     def calculate(
         self,
         predicted_links: Dict[str, List[str]],
         ground_truth_links: Dict[str, List[str]],
         _: Optional[Dict[str, Dict[str, float]]] = None,
     ) -> float:
```

### Comparing `pytctracer-0.1.8/pytctracer/evaluation/metrics/mean_average_precision.py` & `pytctracer-0.1.9/pytctracer/evaluation/metrics/mean_average_precision.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Dict, List, Optional
-from pytctracer.config.constants import MetricScoreTypes
+from pytctracer.config.constants import MetricScoreType
 from pytctracer.evaluation.metrics.metric import Metric
 
 
 class MeanAveragePrecision(Metric):
     full_name = "Mean Average Precision"
     short_name = "MAP"
     arg_name = "map"
-    metric_type = MetricScoreTypes.CONTINUOUS
+    metric_type = MetricScoreType.CONTINUOUS
 
     def calculate(
         self,
         predicted_links: Dict[str, List[str]],
         ground_truth_links: Dict[str, List[str]],
         _: Optional[Dict[str, Dict[str, float]]] = None,
     ) -> float:
```

### Comparing `pytctracer-0.1.8/pytctracer/evaluation/metrics/metric.py` & `pytctracer-0.1.9/pytctracer/evaluation/metrics/metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from abc import ABC, abstractmethod
 from typing import Dict, List, Optional
-from pytctracer.config.constants import MetricScoreTypes
+from pytctracer.config.constants import MetricScoreType
 
 
 class Metric(ABC):
     full_name = "Metric"
     short_name = "Metric"
     arg_name = "metric"
-    metric_type = MetricScoreTypes.NA
+    metric_type = MetricScoreType.NA
 
     @abstractmethod
     def calculate(
         self,
         predicted_links: Dict[str, List[str]],
         ground_truth_links: Dict[str, List[str]],
         traceability_score_dict: Optional[Dict[str, Dict[str, float]]],
```

### Comparing `pytctracer-0.1.8/pytctracer/evaluation/metrics/precision.py` & `pytctracer-0.1.9/pytctracer/evaluation/metrics/precision.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Dict, List, Optional
-from pytctracer.config.constants import MetricScoreTypes
+from pytctracer.config.constants import MetricScoreType
 from pytctracer.evaluation.metrics.metric import Metric
 from pytctracer.evaluation.metrics.false_positives import FalsePositives
 from pytctracer.evaluation.metrics.true_positives import TruePositives
 
 
 class Precision(Metric):
     full_name = "Precision"
     short_name = "Precision"
     arg_name = "precision"
-    metric_type = MetricScoreTypes.CONTINUOUS
+    metric_type = MetricScoreType.CONTINUOUS
 
     def calculate(
         self,
         predicted_links: Dict[str, List[str]],
         ground_truth_links: Dict[str, List[str]],
         _: Optional[Dict[str, Dict[str, float]]] = None,
     ) -> float:
```

### Comparing `pytctracer-0.1.8/pytctracer/evaluation/metrics/recall.py` & `pytctracer-0.1.9/pytctracer/evaluation/metrics/recall.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Dict, List, Optional
-from pytctracer.config.constants import MetricScoreTypes
+from pytctracer.config.constants import MetricScoreType
 from pytctracer.evaluation.metrics.metric import Metric
 from pytctracer.evaluation.metrics.false_negatives import FalseNegatives
 from pytctracer.evaluation.metrics.true_positives import TruePositives
 
 
 class Recall(Metric):
     full_name = "Recall"
     short_name = "Recall"
     arg_name = "recall"
-    metric_type = MetricScoreTypes.CONTINUOUS
+    metric_type = MetricScoreType.CONTINUOUS
 
     def calculate(
         self,
         predicted_links: Dict[str, List[str]],
         ground_truth_links: Dict[str, List[str]],
         _: Optional[Dict[str, Dict[str, float]]] = None,
     ) -> float:
```

### Comparing `pytctracer-0.1.8/pytctracer/evaluation/metrics/true_positives.py` & `pytctracer-0.1.9/pytctracer/evaluation/metrics/false_negatives.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from typing import Dict, List, Optional
-from pytctracer.config.constants import MetricScoreTypes
+from pytctracer.config.constants import MetricScoreType
 from pytctracer.evaluation.metrics.metric import Metric
 
 
-class TruePositives(Metric):
-    full_name = "True Positives"
-    short_name = "TP"
-    arg_name = "tp"
-    metric_type = MetricScoreTypes.INTEGER
+class FalseNegatives(Metric):
+    full_name = "False Negatives"
+    short_name = "FN"
+    arg_name = "fn"
+    metric_type = MetricScoreType.INTEGER
 
     def calculate(
         self,
         predicted_links: Dict[str, List[str]],
         ground_truth_links: Dict[str, List[str]],
         _: Optional[Dict[str, Dict[str, float]]] = None,
     ) -> float:
-        true_positives = 0
+        false_negatives = 0
         for fully_qualified_test_name in ground_truth_links:
             predicted_links_for_test = set(predicted_links[fully_qualified_test_name])
             ground_truth_links_for_test = set(
                 ground_truth_links[fully_qualified_test_name]
             )
-            true_positives += len(
-                predicted_links_for_test.intersection(ground_truth_links_for_test)
+            false_negatives += len(
+                ground_truth_links_for_test - predicted_links_for_test
             )
 
-        return true_positives
+        return false_negatives
 
 
-__all__ = ["TruePositives"]
+__all__ = ["FalseNegatives"]
```

### Comparing `pytctracer-0.1.8/pytctracer/io/input/from_file.py` & `pytctracer-0.1.9/pytctracer/io/input/from_file.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.8/pytctracer/io/output/to_display.py` & `pytctracer-0.1.9/pytctracer/io/output/to_display.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.8/pytctracer/io/output/to_file.py` & `pytctracer-0.1.9/pytctracer/io/output/to_file.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.8/pytctracer/parsing/__init__.py` & `pytctracer-0.1.9/pytctracer/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.8/pytctracer/parsing/find_class_level_calls.py` & `pytctracer-0.1.9/pytctracer/parsing/find_class_level_calls.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,100 +1,100 @@
 from typing import Dict, List, Set
 from collections import defaultdict
 from pytctracer.config.constants import (
-    TraceDataHeaders,
-    TestingMethodTypes,
-    EventTypes,
-    FunctionTypes,
+    TraceDataHeader,
+    TestingMethodType,
+    EventType,
+    FunctionType,
 )
 
 
 def find_function_classes_called_by_test(
     data: List[Dict[str, str]]
 ) -> Dict[str, Set[str]]:
     function_classes_called_by_test_dict = defaultdict(set)
     current_test = None
 
     for record in data:
         if (
-            record[TraceDataHeaders.TESTNG_METHOD]
-            == TestingMethodTypes.TEST_METHOD_CALL
+            record[TraceDataHeader.TESTNG_METHOD]
+            == TestingMethodType.TEST_METHOD_CALL
         ):
-            current_test = record[TraceDataHeaders.FULLY_QUALIFIED_CLASS_NAME]
+            current_test = record[TraceDataHeader.FULLY_QUALIFIED_CLASS_NAME]
         elif (
-            record[TraceDataHeaders.TESTNG_METHOD]
-            == TestingMethodTypes.TEST_METHOD_RETURN
+            record[TraceDataHeader.TESTNG_METHOD]
+            == TestingMethodType.TEST_METHOD_RETURN
         ):
             current_test = None
         elif (
             current_test
-            and record[TraceDataHeaders.FUNCTION_TYPE] == FunctionTypes.SOURCE
-            and record[TraceDataHeaders.FULLY_QUALIFIED_CLASS_NAME]
+            and record[TraceDataHeader.FUNCTION_TYPE] == FunctionType.SOURCE
+            and record[TraceDataHeader.FULLY_QUALIFIED_CLASS_NAME]
         ):
             function_classes_called_by_test_dict[current_test].add(
-                record[TraceDataHeaders.FULLY_QUALIFIED_CLASS_NAME]
+                record[TraceDataHeader.FULLY_QUALIFIED_CLASS_NAME]
             )
 
     return function_classes_called_by_test_dict
 
 
 def find_function_classes_called_by_test_count(
     data: List[Dict[str, str]]
 ) -> Dict[str, Dict[str, int]]:
     function_classes_called_by_test_count_dict = defaultdict(lambda: defaultdict(int))
     current_test = None
 
     for record in data:
         if (
-            record[TraceDataHeaders.TESTNG_METHOD]
-            == TestingMethodTypes.TEST_METHOD_CALL
+            record[TraceDataHeader.TESTNG_METHOD]
+            == TestingMethodType.TEST_METHOD_CALL
         ):
-            current_test = record[TraceDataHeaders.FULLY_QUALIFIED_CLASS_NAME]
+            current_test = record[TraceDataHeader.FULLY_QUALIFIED_CLASS_NAME]
         elif (
-            record[TraceDataHeaders.TESTNG_METHOD]
-            == TestingMethodTypes.TEST_METHOD_RETURN
+            record[TraceDataHeader.TESTNG_METHOD]
+            == TestingMethodType.TEST_METHOD_RETURN
         ):
             current_test = None
         elif (
             current_test
-            and record[TraceDataHeaders.FUNCTION_TYPE] == FunctionTypes.SOURCE
-            and record[TraceDataHeaders.FULLY_QUALIFIED_CLASS_NAME]
-            and record[TraceDataHeaders.EVENT_TYPE] == EventTypes.CALL
+            and record[TraceDataHeader.FUNCTION_TYPE] == FunctionType.SOURCE
+            and record[TraceDataHeader.FULLY_QUALIFIED_CLASS_NAME]
+            and record[TraceDataHeader.EVENT_TYPE] == EventType.CALL
         ):
             function_classes_called_by_test_count_dict[current_test][
-                record[TraceDataHeaders.FULLY_QUALIFIED_CLASS_NAME]
+                record[TraceDataHeader.FULLY_QUALIFIED_CLASS_NAME]
             ] += 1
 
     return function_classes_called_by_test_count_dict
 
 
 def find_tests_that_call_function_classes(
     data: List[Dict[str, str]],
 ) -> Dict[str, Set[str]]:
     tests_that_call_function_classes_dict = defaultdict(set)
     current_test = None
 
     for record in data:
         if (
-            record[TraceDataHeaders.TESTNG_METHOD]
-            == TestingMethodTypes.TEST_METHOD_CALL
+            record[TraceDataHeader.TESTNG_METHOD]
+            == TestingMethodType.TEST_METHOD_CALL
         ):
-            current_test = record[TraceDataHeaders.FULLY_QUALIFIED_CLASS_NAME]
+            current_test = record[TraceDataHeader.FULLY_QUALIFIED_CLASS_NAME]
         elif (
-            record[TraceDataHeaders.TESTNG_METHOD]
-            == TestingMethodTypes.TEST_METHOD_RETURN
+            record[TraceDataHeader.TESTNG_METHOD]
+            == TestingMethodType.TEST_METHOD_RETURN
         ):
             current_test = None
         elif (
             current_test
-            and record[TraceDataHeaders.FUNCTION_TYPE] == FunctionTypes.SOURCE
-            and record[TraceDataHeaders.FULLY_QUALIFIED_CLASS_NAME]
+            and record[TraceDataHeader.FUNCTION_TYPE] == FunctionType.SOURCE
+            and record[TraceDataHeader.FULLY_QUALIFIED_CLASS_NAME]
         ):
             tests_that_call_function_classes_dict[
-                record[TraceDataHeaders.FULLY_QUALIFIED_CLASS_NAME]
+                record[TraceDataHeader.FULLY_QUALIFIED_CLASS_NAME]
             ].add(current_test)
 
     return tests_that_call_function_classes_dict
 
 
 def find_function_classes_called_by_test_depth(
     data: List[Dict[str, str]],
@@ -102,31 +102,31 @@
     # Each function appears once for a test, at the highest depth
     function_classes_called_by_test_depth_dict = defaultdict(dict)
     current_test_class = None
     current_test_class_depth = 0
 
     for record in data:
         if (
-            record[TraceDataHeaders.TESTNG_METHOD]
-            == TestingMethodTypes.TEST_METHOD_CALL
+            record[TraceDataHeader.TESTNG_METHOD]
+            == TestingMethodType.TEST_METHOD_CALL
         ):
-            current_test_class = record[TraceDataHeaders.FULLY_QUALIFIED_CLASS_NAME]
-            current_test_class_depth = int(record[TraceDataHeaders.DEPTH])
+            current_test_class = record[TraceDataHeader.FULLY_QUALIFIED_CLASS_NAME]
+            current_test_class_depth = int(record[TraceDataHeader.DEPTH])
         elif (
-            record[TraceDataHeaders.TESTNG_METHOD]
-            == TestingMethodTypes.TEST_METHOD_RETURN
+            record[TraceDataHeader.TESTNG_METHOD]
+            == TestingMethodType.TEST_METHOD_RETURN
         ):
             current_test_class = None
         elif (
             current_test_class is not None
-            and record[TraceDataHeaders.FUNCTION_TYPE] == FunctionTypes.SOURCE
-            and record[TraceDataHeaders.FULLY_QUALIFIED_CLASS_NAME]
+            and record[TraceDataHeader.FUNCTION_TYPE] == FunctionType.SOURCE
+            and record[TraceDataHeader.FULLY_QUALIFIED_CLASS_NAME]
         ):
-            function_class_name = record[TraceDataHeaders.FULLY_QUALIFIED_CLASS_NAME]
-            function_class_depth = int(record[TraceDataHeaders.DEPTH])
+            function_class_name = record[TraceDataHeader.FULLY_QUALIFIED_CLASS_NAME]
+            function_class_depth = int(record[TraceDataHeader.DEPTH])
             if (
                 current_test_class in function_classes_called_by_test_depth_dict
                 and function_class_name
                 in function_classes_called_by_test_depth_dict[current_test_class]
             ):
                 function_class_depth = min(
                     function_class_depth,
```

### Comparing `pytctracer-0.1.8/pytctracer/parsing/find_class_level_names.py` & `pytctracer-0.1.9/pytctracer/parsing/find_class_level_names.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 from typing import List, Dict, Tuple, Set
 from pytctracer.config.constants import (
-    TraceDataHeaders,
-    FunctionTypes,
-    TestingMethodTypes,
+    TraceDataHeader,
+    FunctionType,
+    TestingMethodType,
 )
 
 
 def find_function_class_names_tuple(
     trace_data: List[Dict[str, str]]
 ) -> Set[Tuple[str, str]]:
     function_class_names_tuple = set()
     for record in trace_data:
-        if record[TraceDataHeaders.FUNCTION_TYPE] == FunctionTypes.SOURCE:
+        if record[TraceDataHeader.FUNCTION_TYPE] == FunctionType.SOURCE:
             function_class_names_tuple.add(
                 (
-                    record[TraceDataHeaders.FULLY_QUALIFIED_CLASS_NAME],
-                    record[TraceDataHeaders.CLASS_NAME],
+                    record[TraceDataHeader.FULLY_QUALIFIED_CLASS_NAME],
+                    record[TraceDataHeader.CLASS_NAME],
                 )
             )
 
     return function_class_names_tuple
 
 
 def find_test_class_names_tuple(
     trace_data: List[Dict[str, str]]
 ) -> Set[Tuple[str, str]]:
     test_class_names_tuple = set()
     for record in trace_data:
         if (
-            record[TraceDataHeaders.TESTNG_METHOD]
-            == TestingMethodTypes.TEST_METHOD_CALL
+            record[TraceDataHeader.TESTNG_METHOD]
+            == TestingMethodType.TEST_METHOD_CALL
         ):
             test_class_names_tuple.add(
                 (
-                    record[TraceDataHeaders.FULLY_QUALIFIED_CLASS_NAME],
-                    record[TraceDataHeaders.CLASS_NAME],
+                    record[TraceDataHeader.FULLY_QUALIFIED_CLASS_NAME],
+                    record[TraceDataHeader.CLASS_NAME],
                 )
             )
 
     return test_class_names_tuple
 
 
 __all__ = ["find_function_class_names_tuple", "find_test_class_names_tuple"]
```

### Comparing `pytctracer-0.1.8/pytctracer/parsing/find_function_level_calls.py` & `pytctracer-0.1.9/pytctracer/parsing/find_function_level_calls.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,93 +1,93 @@
 from typing import List, Dict, Set
 from collections import defaultdict
 from pytctracer.config.constants import (
-    TraceDataHeaders,
-    TestingMethodTypes,
-    EventTypes,
-    FunctionTypes,
+    TraceDataHeader,
+    TestingMethodType,
+    EventType,
+    FunctionType,
 )
 
 
 def find_functions_called_by_test(data: List[Dict[str, str]]) -> Dict[str, Set[str]]:
     functions_called_by_test_dict = defaultdict(set)
     current_test = None
 
     for record in data:
         if (
-            record[TraceDataHeaders.TESTNG_METHOD]
-            == TestingMethodTypes.TEST_METHOD_CALL
+            record[TraceDataHeader.TESTNG_METHOD]
+            == TestingMethodType.TEST_METHOD_CALL
         ):
-            current_test = record[TraceDataHeaders.FULLY_QUALIFIED_FUNCTION_NAME]
+            current_test = record[TraceDataHeader.FULLY_QUALIFIED_FUNCTION_NAME]
         elif (
-            record[TraceDataHeaders.TESTNG_METHOD]
-            == TestingMethodTypes.TEST_METHOD_RETURN
+            record[TraceDataHeader.TESTNG_METHOD]
+            == TestingMethodType.TEST_METHOD_RETURN
         ):
             current_test = None
         elif (
             current_test is not None
-            and record[TraceDataHeaders.FUNCTION_TYPE] == FunctionTypes.SOURCE
+            and record[TraceDataHeader.FUNCTION_TYPE] == FunctionType.SOURCE
         ):
             functions_called_by_test_dict[current_test].add(
-                record[TraceDataHeaders.FULLY_QUALIFIED_FUNCTION_NAME]
+                record[TraceDataHeader.FULLY_QUALIFIED_FUNCTION_NAME]
             )
 
     return functions_called_by_test_dict
 
 
 def find_functions_called_by_test_count(
     data: List[Dict[str, str]]
 ) -> Dict[str, Dict[str, int]]:
     functions_called_by_test_count_dict = defaultdict(lambda: defaultdict(int))
     current_test = None
 
     for record in data:
         if (
-            record[TraceDataHeaders.TESTNG_METHOD]
-            == TestingMethodTypes.TEST_METHOD_CALL
+            record[TraceDataHeader.TESTNG_METHOD]
+            == TestingMethodType.TEST_METHOD_CALL
         ):
-            current_test = record[TraceDataHeaders.FULLY_QUALIFIED_FUNCTION_NAME]
+            current_test = record[TraceDataHeader.FULLY_QUALIFIED_FUNCTION_NAME]
         elif (
-            record[TraceDataHeaders.TESTNG_METHOD]
-            == TestingMethodTypes.TEST_METHOD_RETURN
+            record[TraceDataHeader.TESTNG_METHOD]
+            == TestingMethodType.TEST_METHOD_RETURN
         ):
             current_test = None
         elif (
             current_test is not None
-            and record[TraceDataHeaders.FUNCTION_TYPE] == FunctionTypes.SOURCE
-            and record[TraceDataHeaders.EVENT_TYPE] == EventTypes.CALL
+            and record[TraceDataHeader.FUNCTION_TYPE] == FunctionType.SOURCE
+            and record[TraceDataHeader.EVENT_TYPE] == EventType.CALL
         ):
             functions_called_by_test_count_dict[current_test][
-                record[TraceDataHeaders.FULLY_QUALIFIED_FUNCTION_NAME]
+                record[TraceDataHeader.FULLY_QUALIFIED_FUNCTION_NAME]
             ] += 1
 
     return functions_called_by_test_count_dict
 
 
 def find_tests_that_call_function(data: List[Dict[str, str]]) -> Dict[str, Set[str]]:
     tests_that_call_function_dict = defaultdict(set)
     current_test = None
 
     for record in data:
         if (
-            record[TraceDataHeaders.TESTNG_METHOD]
-            == TestingMethodTypes.TEST_METHOD_CALL
+            record[TraceDataHeader.TESTNG_METHOD]
+            == TestingMethodType.TEST_METHOD_CALL
         ):
-            current_test = record[TraceDataHeaders.FULLY_QUALIFIED_FUNCTION_NAME]
+            current_test = record[TraceDataHeader.FULLY_QUALIFIED_FUNCTION_NAME]
         elif (
-            record[TraceDataHeaders.TESTNG_METHOD]
-            == TestingMethodTypes.TEST_METHOD_RETURN
+            record[TraceDataHeader.TESTNG_METHOD]
+            == TestingMethodType.TEST_METHOD_RETURN
         ):
             current_test = None
         elif (
             current_test is not None
-            and record[TraceDataHeaders.FUNCTION_TYPE] == FunctionTypes.SOURCE
+            and record[TraceDataHeader.FUNCTION_TYPE] == FunctionType.SOURCE
         ):
             tests_that_call_function_dict[
-                record[TraceDataHeaders.FULLY_QUALIFIED_FUNCTION_NAME]
+                record[TraceDataHeader.FULLY_QUALIFIED_FUNCTION_NAME]
             ].add(current_test)
 
     return tests_that_call_function_dict
 
 
 def find_functions_called_by_test_depth(
     data: List[Dict[str, str]]
@@ -95,30 +95,30 @@
     # Each function appears once for a test, at the highest depth
     functions_called_by_test_depth_dict = defaultdict(dict)
     current_test = None
     current_test_depth = 0
 
     for record in data:
         if (
-            record[TraceDataHeaders.TESTNG_METHOD]
-            == TestingMethodTypes.TEST_METHOD_CALL
+            record[TraceDataHeader.TESTNG_METHOD]
+            == TestingMethodType.TEST_METHOD_CALL
         ):
-            current_test = record[TraceDataHeaders.FULLY_QUALIFIED_FUNCTION_NAME]
-            current_test_depth = int(record[TraceDataHeaders.DEPTH])
+            current_test = record[TraceDataHeader.FULLY_QUALIFIED_FUNCTION_NAME]
+            current_test_depth = int(record[TraceDataHeader.DEPTH])
         elif (
-            record[TraceDataHeaders.TESTNG_METHOD]
-            == TestingMethodTypes.TEST_METHOD_RETURN
+            record[TraceDataHeader.TESTNG_METHOD]
+            == TestingMethodType.TEST_METHOD_RETURN
         ):
             current_test = None
         elif (
             current_test is not None
-            and record[TraceDataHeaders.FUNCTION_TYPE] == FunctionTypes.SOURCE
+            and record[TraceDataHeader.FUNCTION_TYPE] == FunctionType.SOURCE
         ):
-            function_name = record[TraceDataHeaders.FULLY_QUALIFIED_FUNCTION_NAME]
-            function_depth = int(record[TraceDataHeaders.DEPTH])
+            function_name = record[TraceDataHeader.FULLY_QUALIFIED_FUNCTION_NAME]
+            function_depth = int(record[TraceDataHeader.DEPTH])
             if (
                 current_test in functions_called_by_test_depth_dict
                 and function_name in functions_called_by_test_depth_dict[current_test]
             ):
                 function_depth = min(
                     function_depth,
                     functions_called_by_test_depth_dict[current_test][function_name],
```

### Comparing `pytctracer-0.1.8/pytctracer/parsing/find_function_level_names.py` & `pytctracer-0.1.9/pytctracer/parsing/find_function_level_names.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from typing import Tuple, Set, Dict, List
 from pytctracer.config.constants import (
-    TraceDataHeaders,
-    FunctionTypes,
-    TestingMethodTypes,
+    TraceDataHeader,
+    FunctionType,
+    TestingMethodType,
 )
 
 
 def find_function_names_tuple(trace_data: List[Dict[str, str]]) -> Set[Tuple[str, str]]:
     function_names_tuple = set()
     for record in trace_data:
-        if record[TraceDataHeaders.FUNCTION_TYPE] == FunctionTypes.SOURCE:
+        if record[TraceDataHeader.FUNCTION_TYPE] == FunctionType.SOURCE:
             function_names_tuple.add(
                 (
-                    record[TraceDataHeaders.FULLY_QUALIFIED_FUNCTION_NAME],
-                    record[TraceDataHeaders.FUNCTION_NAME],
+                    record[TraceDataHeader.FULLY_QUALIFIED_FUNCTION_NAME],
+                    record[TraceDataHeader.FUNCTION_NAME],
                 )
             )
 
     return function_names_tuple
 
 
 def find_test_names_tuple(trace_data: List[Dict[str, str]]) -> Set[Tuple[str, str]]:
     test_names_tuple = set()
     for record in trace_data:
         if (
-            record[TraceDataHeaders.TESTNG_METHOD]
-            == TestingMethodTypes.TEST_METHOD_CALL
+            record[TraceDataHeader.TESTNG_METHOD]
+            == TestingMethodType.TEST_METHOD_CALL
         ):
             test_names_tuple.add(
                 (
-                    record[TraceDataHeaders.FULLY_QUALIFIED_FUNCTION_NAME],
-                    record[TraceDataHeaders.FUNCTION_NAME],
+                    record[TraceDataHeader.FULLY_QUALIFIED_FUNCTION_NAME],
+                    record[TraceDataHeader.FUNCTION_NAME],
                 )
             )
 
     return test_names_tuple
 
 
 __all__ = ["find_function_names_tuple", "find_test_names_tuple"]
```

### Comparing `pytctracer-0.1.8/pytctracer/parsing/functions_called_before_assert.py` & `pytctracer-0.1.9/pytctracer/parsing/functions_called_before_assert.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from collections import defaultdict
 from typing import Dict, List, Set
 from pytctracer.config.constants import (
-    TestingMethodTypes,
-    TraceDataHeaders,
-    EventTypes,
-    FunctionTypes,
+    TestingMethodType,
+    TraceDataHeader,
+    EventType,
+    FunctionType,
 )
 
 
 def find_functions_called_before_assert_for_each_test(
     trace_data: List[Dict[str, str]]
 ) -> Dict[str, Set[str]]:
     functions_called_before_assert_for_each_test = defaultdict(set)
     current_test = None
     last_returned_function = None
 
     for record in trace_data:
         if (
-            record[TraceDataHeaders.TESTNG_METHOD]
-            == TestingMethodTypes.TEST_METHOD_CALL
+            record[TraceDataHeader.TESTNG_METHOD]
+            == TestingMethodType.TEST_METHOD_CALL
         ):
-            current_test = record[TraceDataHeaders.FULLY_QUALIFIED_FUNCTION_NAME]
+            current_test = record[TraceDataHeader.FULLY_QUALIFIED_FUNCTION_NAME]
             last_returned_function = None
         elif (
-            record[TraceDataHeaders.TESTNG_METHOD]
-            == TestingMethodTypes.TEST_METHOD_RETURN
+            record[TraceDataHeader.TESTNG_METHOD]
+            == TestingMethodType.TEST_METHOD_RETURN
         ):
             current_test = None
         elif (
             current_test is not None
-            and record[TraceDataHeaders.EVENT_TYPE] == EventTypes.RETURN
-            and record[TraceDataHeaders.FUNCTION_TYPE] == FunctionTypes.SOURCE
+            and record[TraceDataHeader.EVENT_TYPE] == EventType.RETURN
+            and record[TraceDataHeader.FUNCTION_TYPE] == FunctionType.SOURCE
         ):
             last_returned_function = record[
-                TraceDataHeaders.FULLY_QUALIFIED_FUNCTION_NAME
+                TraceDataHeader.FULLY_QUALIFIED_FUNCTION_NAME
             ]
         elif (
             current_test is not None
             and last_returned_function is not None
-            and record[TraceDataHeaders.FUNCTION_TYPE] == FunctionTypes.ASSERT
+            and record[TraceDataHeader.FUNCTION_TYPE] == FunctionType.ASSERT
         ):
             # Won't catch the last returned function if there was no return
             # before an assert in the current test
             functions_called_before_assert_for_each_test[current_test].add(
                 last_returned_function
             )
 
@@ -54,36 +54,36 @@
 ) -> Dict[str, Set[str]]:
     function_classes_called_before_assert_for_each_test = defaultdict(set)
     current_test_class = None
     last_returned_function_class = None
 
     for record in trace_data:
         if (
-            record[TraceDataHeaders.TESTNG_METHOD]
-            == TestingMethodTypes.TEST_METHOD_CALL
+            record[TraceDataHeader.TESTNG_METHOD]
+            == TestingMethodType.TEST_METHOD_CALL
         ):
-            current_test_class = record[TraceDataHeaders.FULLY_QUALIFIED_CLASS_NAME]
+            current_test_class = record[TraceDataHeader.FULLY_QUALIFIED_CLASS_NAME]
             last_returned_function_class = None
         elif (
-            record[TraceDataHeaders.TESTNG_METHOD]
-            == TestingMethodTypes.TEST_METHOD_RETURN
+            record[TraceDataHeader.TESTNG_METHOD]
+            == TestingMethodType.TEST_METHOD_RETURN
         ):
             current_test_class = None
         elif (
             current_test_class
-            and record[TraceDataHeaders.EVENT_TYPE] == EventTypes.RETURN
-            and record[TraceDataHeaders.FUNCTION_TYPE] == FunctionTypes.SOURCE
+            and record[TraceDataHeader.EVENT_TYPE] == EventType.RETURN
+            and record[TraceDataHeader.FUNCTION_TYPE] == FunctionType.SOURCE
         ):
             last_returned_function_class = record[
-                TraceDataHeaders.FULLY_QUALIFIED_CLASS_NAME
+                TraceDataHeader.FULLY_QUALIFIED_CLASS_NAME
             ]
         elif (
             current_test_class
             and last_returned_function_class
-            and record[TraceDataHeaders.FUNCTION_TYPE] == FunctionTypes.ASSERT
+            and record[TraceDataHeader.FUNCTION_TYPE] == FunctionType.ASSERT
         ):
             # Won't catch the last returned function if there was no return
             # before an assert in the current test
             function_classes_called_before_assert_for_each_test[current_test_class].add(
                 last_returned_function_class
             )
```

### Comparing `pytctracer-0.1.8/pytctracer/techniques/__init__.py` & `pytctracer-0.1.9/pytctracer/techniques/__init__.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.8/pytctracer/techniques/arg_name_to_technique_mapper.py` & `pytctracer-0.1.9/pytctracer/techniques/arg_name_to_technique_mapper.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.8/pytctracer/techniques/combined.py` & `pytctracer-0.1.9/pytctracer/techniques/combined.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import Dict
 from collections import defaultdict
 from pytctracer.techniques.technique import Technique
-from pytctracer.config.constants import TechniqueThresholds
+from pytctracer.config.constants import TechniqueThreshold
 
 
 class Combined(Technique):
     """
     Class implementing the Combined
     traceability technique.
     """
 
     full_name = "Combined (Simple Average)"
     short_name = "Combined"
     arg_name = "combined"
     description = "TBC"
     required_parameters = {}
     uses_threshold = True
-    threshold = TechniqueThresholds.THRESHOLD_FOR_COMBINED
+    threshold = TechniqueThreshold.THRESHOLD_FOR_COMBINED
     normalise = True
 
     def run(
         self, traceability_scores_for_techniques: Dict[str, Dict[str, Dict[str, float]]]
     ) -> Dict[str, Dict[str, float]]:
         number_of_techniques_to_combine = len(traceability_scores_for_techniques)
         combined_scores = None
```

### Comparing `pytctracer-0.1.8/pytctracer/techniques/last_call_before_assert.py` & `pytctracer-0.1.9/pytctracer/techniques/last_call_before_assert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Dict, Union, List, Tuple, Set
 from collections import defaultdict
 from pytctracer.techniques.technique import Technique
-from pytctracer.config.constants import TechniqueParameters
+from pytctracer.config.constants import TechniqueParameter
 
 
 class LastCallBeforeAssert(Technique):
     """
     Parent Class implementing the Last Call Before Assert traceability technique.
     """
 
     full_name = "Last Call Before Assert"
     short_name = "LCBA"
     arg_name = "lcba"
     description = "TBC"
     required_parameters = {
-        TechniqueParameters.FUNCTION_NAMES_TUPLE,
-        TechniqueParameters.TEST_NAMES_TUPLE,
-        TechniqueParameters.FUNCTIONS_CALLED_BY_TESTS,
-        TechniqueParameters.FUNCTIONS_CALLED_BY_TEST_BEFORE_ASSERT,
+        TechniqueParameter.FUNCTION_NAMES_TUPLE,
+        TechniqueParameter.TEST_NAMES_TUPLE,
+        TechniqueParameter.FUNCTIONS_CALLED_BY_TESTS,
+        TechniqueParameter.FUNCTIONS_CALLED_BY_TEST_BEFORE_ASSERT,
     }
 
     def run(
         self,
         function_names_tuple: List[Tuple[str, str]],
         test_names_tuple: List[Tuple[str, str]],
         functions_called_by_tests: Dict[str, Set[str]],
```

### Comparing `pytctracer-0.1.8/pytctracer/techniques/levenshtein_distance.py` & `pytctracer-0.1.9/pytctracer/techniques/levenshtein_distance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from typing import Dict, Union, List, Tuple, Set
 from collections import defaultdict
 from pytctracer.techniques.technique import Technique
-from pytctracer.config.constants import TechniqueParameters, TechniqueThresholds
+from pytctracer.config.constants import TechniqueParameter, TechniqueThreshold
 
 
 class LevenshteinDistance(Technique):
     """
     Class implementing the Levenshtein
     traceability technique.
     """
 
     full_name = "Levenshtein Distance"
     short_name = "Leven"
     arg_name = "leven"
     description = "TBC"
     required_parameters = {
-        TechniqueParameters.FUNCTION_NAMES_TUPLE,
-        TechniqueParameters.TEST_NAMES_TUPLE,
-        TechniqueParameters.FUNCTIONS_CALLED_BY_TESTS,
-        TechniqueParameters.FUNCTIONS_CALLED_BY_TEST_DEPTH,
+        TechniqueParameter.FUNCTION_NAMES_TUPLE,
+        TechniqueParameter.TEST_NAMES_TUPLE,
+        TechniqueParameter.FUNCTIONS_CALLED_BY_TESTS,
+        TechniqueParameter.FUNCTIONS_CALLED_BY_TEST_DEPTH,
     }
     uses_threshold = True
-    threshold = TechniqueThresholds.THRESHOLD_FOR_LEVENSHTEIN
+    threshold = TechniqueThreshold.THRESHOLD_FOR_LEVENSHTEIN
     normalise = True
     call_depth_discount = True
 
     def run(
         self,
         function_names_tuple: List[Tuple[str, str]],
         test_names_tuple: List[Tuple[str, str]],
```

### Comparing `pytctracer-0.1.8/pytctracer/techniques/longest_common_subsequence.py` & `pytctracer-0.1.9/pytctracer/techniques/longest_common_subsequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Dict, Union, List, Tuple, Set
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from pytctracer.techniques.technique import Technique
-from pytctracer.config.constants import TechniqueParameters, TechniqueThresholds
+from pytctracer.config.constants import TechniqueParameter, TechniqueThreshold
 
 
 class LongestCommonSubsequence(Technique, ABC):
     """
     Parent Class for the LCS-B and LCS-U traceability techniques.
     """
 
     full_name = "Longest Common Subsequence"
     short_name = "LCS"
     description = "TBC"
     required_parameters = {
-        TechniqueParameters.FUNCTION_NAMES_TUPLE,
-        TechniqueParameters.TEST_NAMES_TUPLE,
-        TechniqueParameters.FUNCTIONS_CALLED_BY_TESTS,
-        TechniqueParameters.FUNCTIONS_CALLED_BY_TEST_DEPTH,
+        TechniqueParameter.FUNCTION_NAMES_TUPLE,
+        TechniqueParameter.TEST_NAMES_TUPLE,
+        TechniqueParameter.FUNCTIONS_CALLED_BY_TESTS,
+        TechniqueParameter.FUNCTIONS_CALLED_BY_TEST_DEPTH,
     }
     uses_threshold = True
     normalise = True
     call_depth_discount = True
 
     def run(
         self,
@@ -120,15 +120,15 @@
     traceability technique.
     """
 
     full_name = "Longest Common Subsequence - Unit"
     short_name = "LCS-U"
     description = "TBC"
     arg_name = "lcsu"
-    threshold = TechniqueThresholds.THRESHOLD_FOR_LCSU
+    threshold = TechniqueThreshold.THRESHOLD_FOR_LCSU
 
     def run(
         self,
         function_names_tuple: List[Tuple[str, str]],
         test_names_tuple: List[Tuple[str, str]],
         functions_called_by_tests: Dict[str, Set[str]],
         functions_called_by_test_depth: Dict[str, Dict[str, int]],
@@ -182,15 +182,15 @@
     traceability technique.
     """
 
     full_name = "Longest Common Subsequence - Both"
     short_name = "LCS-B"
     arg_name = "lcsb"
     description = "TBC"
-    threshold = TechniqueThresholds.THRESHOLD_FOR_LCSB
+    threshold = TechniqueThreshold.THRESHOLD_FOR_LCSB
 
     def run(
         self,
         function_names_tuple: List[Tuple[str, str]],
         test_names_tuple: List[Tuple[str, str]],
         functions_called_by_tests: Dict[str, Set[str]],
         functions_called_by_test_depth: Dict[str, Dict[str, int]],
```

### Comparing `pytctracer-0.1.8/pytctracer/techniques/naming_conventions.py` & `pytctracer-0.1.9/pytctracer/techniques/naming_conventions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import Dict, Union, List, Tuple, Set
 from collections import defaultdict
 from pytctracer.techniques.technique import Technique
-from pytctracer.config.constants import TechniqueParameters
+from pytctracer.config.constants import TechniqueParameter
 
 
 class NamingConventions(Technique):
     """
     Class implementing the Naming Conventions traceability technique.
     """
 
     full_name = "Naming Conventions"
     short_name = "NC"
     description = "TBC"
     arg_name = "nc"
     required_parameters = {
-        TechniqueParameters.FUNCTION_NAMES_TUPLE,
-        TechniqueParameters.TEST_NAMES_TUPLE,
-        TechniqueParameters.FUNCTIONS_CALLED_BY_TESTS,
+        TechniqueParameter.FUNCTION_NAMES_TUPLE,
+        TechniqueParameter.TEST_NAMES_TUPLE,
+        TechniqueParameter.FUNCTIONS_CALLED_BY_TESTS,
     }
 
     def run(
         self,
         function_names_tuple: List[Tuple[str, str]],
         test_names_tuple: List[Tuple[str, str]],
         functions_called_by_tests: Dict[str, Set[str]],
@@ -90,17 +90,17 @@
     """
 
     full_name = "Naming Conventions - Contains"
     short_name = "NCC"
     description = "TBC"
     arg_name = "ncc"
     required_parameters = {
-        TechniqueParameters.FUNCTION_NAMES_TUPLE,
-        TechniqueParameters.TEST_NAMES_TUPLE,
-        TechniqueParameters.FUNCTIONS_CALLED_BY_TESTS,
+        TechniqueParameter.FUNCTION_NAMES_TUPLE,
+        TechniqueParameter.TEST_NAMES_TUPLE,
+        TechniqueParameter.FUNCTIONS_CALLED_BY_TESTS,
     }
 
     def run(
         self,
         function_names_tuple: List[Tuple[str, str]],
         test_names_tuple: List[Tuple[str, str]],
         functions_called_by_tests: Dict[str, Set[str]],
```

### Comparing `pytctracer-0.1.8/pytctracer/techniques/tarantula.py` & `pytctracer-0.1.9/pytctracer/techniques/tarantula.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from typing import Dict, Union, List, Tuple, Set
 from collections import defaultdict
 from pytctracer.techniques.technique import Technique
-from pytctracer.config.constants import TechniqueParameters, TechniqueThresholds
+from pytctracer.config.constants import TechniqueParameter, TechniqueThreshold
 
 
 class Tarantula(Technique):
     """
     Class implementing the Tarantula
     traceability technique.
     """
 
     full_name = "Tarantula"
     short_name = "Tarantula"
     description = "TBC"
     arg_name = "tarantula"
     required_parameters = {
-        TechniqueParameters.FUNCTION_NAMES_TUPLE,
-        TechniqueParameters.TEST_NAMES_TUPLE,
-        TechniqueParameters.FUNCTIONS_CALLED_BY_TESTS,
-        TechniqueParameters.TESTS_THAT_CALL_FUNCTIONS,
-        TechniqueParameters.FUNCTIONS_CALLED_BY_TEST_DEPTH,
+        TechniqueParameter.FUNCTION_NAMES_TUPLE,
+        TechniqueParameter.TEST_NAMES_TUPLE,
+        TechniqueParameter.FUNCTIONS_CALLED_BY_TESTS,
+        TechniqueParameter.TESTS_THAT_CALL_FUNCTIONS,
+        TechniqueParameter.FUNCTIONS_CALLED_BY_TEST_DEPTH,
     }
     uses_threshold = True
-    threshold = TechniqueThresholds.THRESHOLD_FOR_TARANTULA
+    threshold = TechniqueThreshold.THRESHOLD_FOR_TARANTULA
     normalise = True
     call_depth_discount = True
 
     def run(
         self,
         function_names_tuple: List[Tuple[str, str]],
         test_names_tuple: List[Tuple[str, str]],
```

### Comparing `pytctracer-0.1.8/pytctracer/techniques/technique.py` & `pytctracer-0.1.9/pytctracer/techniques/technique.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.8/pytctracer/techniques/tfidf.py` & `pytctracer-0.1.9/pytctracer/techniques/tfidf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from typing import Dict, Union, List, Tuple, Set
 from math import log
 from collections import defaultdict
 from pytctracer.techniques.technique import Technique
-from pytctracer.config.constants import TechniqueParameters, TechniqueThresholds
+from pytctracer.config.constants import TechniqueParameter, TechniqueThreshold
 
 
 class TFIDF(Technique):
     """
     Class implementing the TF-IDF
     traceability technique.
     """
 
     full_name = "TF-IDF"
     short_name = "TF-IDF"
     arg_name = "tfidf"
     description = "TBC"
     required_parameters = {
-        TechniqueParameters.FUNCTION_NAMES_TUPLE,
-        TechniqueParameters.TEST_NAMES_TUPLE,
-        TechniqueParameters.FUNCTIONS_CALLED_BY_TESTS,
-        TechniqueParameters.TESTS_THAT_CALL_FUNCTIONS,
-        TechniqueParameters.FUNCTIONS_CALLED_BY_TEST_DEPTH,
+        TechniqueParameter.FUNCTION_NAMES_TUPLE,
+        TechniqueParameter.TEST_NAMES_TUPLE,
+        TechniqueParameter.FUNCTIONS_CALLED_BY_TESTS,
+        TechniqueParameter.TESTS_THAT_CALL_FUNCTIONS,
+        TechniqueParameter.FUNCTIONS_CALLED_BY_TEST_DEPTH,
     }
     uses_threshold = True
-    threshold = TechniqueThresholds.THRESHOLD_FOR_TFIDF
+    threshold = TechniqueThreshold.THRESHOLD_FOR_TFIDF
     normalise = True
     call_depth_discount = True
 
     def run(
         self,
         function_names_tuple: List[Tuple[str, str]],
         test_names_tuple: List[Tuple[str, str]],
@@ -141,21 +141,21 @@
     """
 
     full_name = "TF-IDF (Multiset)"
     short_name = "TF-IDF*"
     description = "TBC"
     arg_name = "tfidf_multiset"
     required_parameters = {
-        TechniqueParameters.FUNCTION_NAMES_TUPLE,
-        TechniqueParameters.TEST_NAMES_TUPLE,
-        TechniqueParameters.FUNCTIONS_CALLED_BY_TEST_COUNT,
-        TechniqueParameters.TESTS_THAT_CALL_FUNCTIONS,
-        TechniqueParameters.FUNCTIONS_CALLED_BY_TEST_DEPTH,
+        TechniqueParameter.FUNCTION_NAMES_TUPLE,
+        TechniqueParameter.TEST_NAMES_TUPLE,
+        TechniqueParameter.FUNCTIONS_CALLED_BY_TEST_COUNT,
+        TechniqueParameter.TESTS_THAT_CALL_FUNCTIONS,
+        TechniqueParameter.FUNCTIONS_CALLED_BY_TEST_DEPTH,
     }
-    threshold = TechniqueThresholds.THRESHOLD_FOR_TFIDF_MULTISET
+    threshold = TechniqueThreshold.THRESHOLD_FOR_TFIDF_MULTISET
 
     def run(
         self,
         function_names_tuple: List[Tuple[str, str]],
         test_names_tuple: List[Tuple[str, str]],
         functions_called_by_test_count: Dict[str, Dict[str, int]],
         tests_that_call_functions: Dict[str, Set[str]],
```

### Comparing `pytctracer-0.1.8/pytctracer/tracer.py` & `pytctracer-0.1.9/pytctracer/tracer.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 import os
 import inspect
 import pytest
 import csv
 import threading
 import dis
 from pytctracer.config.constants import (
-    TraceDataHeaders,
-    TestingMethodTypes,
-    TraceDataVariables,
-    EventTypes,
-    FunctionTypes,
-    InstructionOpnames,
-    SetProfileCEventTypes,
-    SetTraceEventTypes,
+    TraceDataHeader,
+    TestingMethodType,
+    TraceDataVariable,
+    EventType,
+    FunctionType,
+    InstructionOpname,
+    SetProfileCEventType,
+    SetTraceEventType,
 )
 
 TRACE_QUALIFIED_NAME = "PytestTracer.trace"
 TEST_PREFIX = "test"
 TEST_CLASS_PREFIX = "Test"
 LOCALS = "<locals>"
 MODULE = "<module>"
@@ -40,15 +40,15 @@
         ]
         self._source_folders = [
             os.path.normcase(os.path.join(self._project_root, source_folder))
             for source_folder in source_folders
         ]
         self._pytest_path = os.path.normcase(os.path.dirname(inspect.getfile(pytest)))
         # Retrieves the absolute file path to the directory of the pytest module
-        self._csv_headers = [header for header in TraceDataHeaders]
+        self._csv_headers = [header for header in TraceDataHeader]
         self._csv_name = output_csv_file_name
         self._test_function_stack = []
         self._function_stack = []
         self._current_depth = 0
         self._file_of_last_assert = None
         self._line_of_last_assert = None
         self._csv_data = []
@@ -88,154 +88,154 @@
                 )
                 fully_qualified_class_name = self._get_fully_qualified_name(
                     file_name=file_name,
                     code_qualified_name=qualified_class_name,
                     function_type=function_type,
                 )
                 if (
-                    event == SetTraceEventTypes.LINE
-                    and function_type == FunctionTypes.ASSERT
+                    event == SetTraceEventType.LINE
+                    and function_type == FunctionType.ASSERT
                 ):
                     if self._check_in_line_functions_in_assert():
                         self._save_assert_line_values(
                             depth=self._current_depth,
                             function_type=function_type,
                             function_name=function_name,
                             fully_qualified_function_name=fully_qualified_function_name,
                             class_name=class_name,
                             fully_qualified_class_name=fully_qualified_class_name,
                             line_number=line_number,
-                            event_type=EventTypes.LINE,
+                            event_type=EventType.LINE,
                             return_value=str(arg),
                             return_type=str(type(arg)),
                             testing_method="",
                             thread_id=current_thread_id,
                         )
                     else:
                         self._add_csv_row_data(
                             depth=self._current_depth,
                             function_type=function_type,
                             function_name=function_name,
                             fully_qualified_function_name=fully_qualified_function_name,
                             class_name=class_name,
                             fully_qualified_class_name=fully_qualified_class_name,
                             line_number=line_number,
-                            event_type=EventTypes.LINE,
+                            event_type=EventType.LINE,
                             return_value=str(arg),
                             return_type=str(type(arg)),
                             testing_method="",
                             thread_id=current_thread_id,
                         )
 
-                elif event == SetTraceEventTypes.CALL:
+                elif event == SetTraceEventType.CALL:
                     testing_method = (
-                        TestingMethodTypes.TEST_METHOD_CALL
-                        if function_type == FunctionTypes.TEST_FUNCTION
+                        TestingMethodType.TEST_METHOD_CALL
+                        if function_type == FunctionType.TEST_FUNCTION
                         and len(self._test_function_stack) == 0
                         else ""
                     )  # Testing method is whether the actual function is a unit test or not
                     self._add_csv_row_data(
                         depth=self._current_depth,
                         function_type=function_type,
                         function_name=function_name,
                         fully_qualified_function_name=fully_qualified_function_name,
                         class_name=class_name,
                         fully_qualified_class_name=fully_qualified_class_name,
                         line_number=line_number,
-                        event_type=EventTypes.CALL,
+                        event_type=EventType.CALL,
                         testing_method=testing_method,
                         thread_id=current_thread_id,
                     )
                     self._function_stack.append(
                         (fully_qualified_function_name, self._current_depth)
                     )
                     if function_type.startswith(TEST_PREFIX.upper()):
                         self._test_function_stack.append(fully_qualified_function_name)
 
                     self._current_depth += 1
 
-                elif event == SetTraceEventTypes.RETURN:
+                elif event == SetTraceEventType.RETURN:
                     # Keep track of the last function that was last returned
                     self._current_depth -= 1
                     self._function_stack.pop()
                     # print(f"{'  ' * (self._current_depth)}< {self._current_depth}: Function '{fully_qualified_function_name}()' returned at line {line_number} with value: '{arg}' of type {type(arg)}")
                     if (
                         function_type.startswith(TEST_PREFIX.upper())
-                        or function_type == FunctionTypes.ASSERT
+                        or function_type == FunctionType.ASSERT
                     ):
                         self._test_function_stack.pop()
                         # if len(self._test_function_stack) == 0:
                         #     print(f"=== EXITING TEST FUNCTION '{fully_qualified_function_name}\n")
-                    if function_type == FunctionTypes.ASSERT:
+                    if function_type == FunctionType.ASSERT:
                         # If an assert happens to be on the last line, it may get caught as a return event, so we add a duplicate entry to account for assert line and return
                         self._add_csv_row_data(
                             depth=self._current_depth + 1,
                             function_type=function_type,
                             function_name=function_name,
                             fully_qualified_function_name=fully_qualified_function_name,
                             class_name=class_name,
                             fully_qualified_class_name=fully_qualified_class_name,
                             line_number=line_number,
-                            event_type=EventTypes.RETURN,
+                            event_type=EventType.RETURN,
                             return_value=str(arg),
                             return_type=str(type(arg)),
                             testing_method="",
                             thread_id=current_thread_id,
                         )
-                        function_type = FunctionTypes.TEST_FUNCTION
+                        function_type = FunctionType.TEST_FUNCTION
                     testing_method = (
-                        TestingMethodTypes.TEST_METHOD_RETURN
-                        if function_type == FunctionTypes.TEST_FUNCTION
+                        TestingMethodType.TEST_METHOD_RETURN
+                        if function_type == FunctionType.TEST_FUNCTION
                         and len(self._test_function_stack) == 0
                         else ""
                     )
                     self._add_csv_row_data(
                         depth=self._current_depth,
                         function_type=function_type,
                         function_name=function_name,
                         fully_qualified_function_name=fully_qualified_function_name,
                         class_name=class_name,
                         fully_qualified_class_name=fully_qualified_class_name,
                         line_number=line_number,
-                        event_type=EventTypes.RETURN,
+                        event_type=EventType.RETURN,
                         return_value=str(arg),
                         return_type=str(type(arg)),
                         testing_method=testing_method,
                         thread_id=current_thread_id,
                     )
                     self._check_remaining_in_line_functions(self._current_depth)
 
-                elif event == SetTraceEventTypes.EXCEPTION:
+                elif event == SetTraceEventType.EXCEPTION:
                     exc_type, exc_value, exc_traceback = arg
                     # print(f"{'  ' * (self._current_depth - 1)}- {self._current_depth}: Function '{fully_qualified_function_name}()' at line {line_number} has raised an Exception, with exception type: {exc_type} and message: '{str(exc_value)}'")
                     self._add_csv_row_data(
                         depth=self._current_depth,
                         function_type=function_type,
                         function_name=function_name,
                         fully_qualified_function_name=fully_qualified_function_name,
                         class_name=class_name,
                         fully_qualified_class_name=fully_qualified_class_name,
                         line_number=line_number,
-                        event_type=EventTypes.EXCEPTION,
+                        event_type=EventType.EXCEPTION,
                         exception_type=exc_type,
                         exception_message=str(exc_value),
                     )
 
         return self.trace
 
     def trace_in_built(self, _frame: FrameType, event, _arg=None):
         # Handle in-line function returns that don't get captured by sys.settrace, for assert checking
         # For example, isinstance within an assert statement
         # These built in functions won't be caught by the sys.settrace function, so we need to check
         # for them here.
-        if event == SetProfileCEventTypes.C_CALL:
+        if event == SetProfileCEventType.C_CALL:
             self._current_depth += 1
         if (
-            event == SetProfileCEventTypes.C_RETURN
-            or event == SetProfileCEventTypes.C_EXCEPTION
+            event == SetProfileCEventType.C_RETURN
+            or event == SetProfileCEventType.C_EXCEPTION
         ):
             self._current_depth -= 1
             self._check_remaining_in_line_functions(self._current_depth)
 
     def write_to_csv(self) -> None:
         with open(self._csv_name, "w", newline="") as csv_file:
             csv_writer = csv.DictWriter(csv_file, fieldnames=self._csv_headers)
@@ -261,28 +261,28 @@
         return_type: Optional[str] = "",
         exception_type: Optional[str] = "",
         exception_message: Optional[str] = "",
         testing_method: Optional[str] = "",
         thread_id: Optional[int] = None,
     ):
         data = {
-            TraceDataHeaders.DEPTH: depth,
-            TraceDataHeaders.FUNCTION_TYPE: function_type,
-            TraceDataHeaders.TESTNG_METHOD: testing_method,
-            TraceDataHeaders.FUNCTION_NAME: function_name,
-            TraceDataHeaders.FULLY_QUALIFIED_FUNCTION_NAME: fully_qualified_function_name,
-            TraceDataHeaders.CLASS_NAME: class_name,
-            TraceDataHeaders.FULLY_QUALIFIED_CLASS_NAME: fully_qualified_class_name,
-            TraceDataHeaders.LINE: line_number,
-            TraceDataHeaders.EVENT_TYPE: event_type,
-            TraceDataHeaders.RETURN_VALUE: return_value,
-            TraceDataHeaders.RETURN_TYPE: return_type,
-            TraceDataHeaders.EXCEPTION_TYPE: exception_type,
-            TraceDataHeaders.EXCEPTION_MESSAGE: exception_message,
-            TraceDataHeaders.THREAD_ID: thread_id,
+            TraceDataHeader.DEPTH: depth,
+            TraceDataHeader.FUNCTION_TYPE: function_type,
+            TraceDataHeader.TESTNG_METHOD: testing_method,
+            TraceDataHeader.FUNCTION_NAME: function_name,
+            TraceDataHeader.FULLY_QUALIFIED_FUNCTION_NAME: fully_qualified_function_name,
+            TraceDataHeader.CLASS_NAME: class_name,
+            TraceDataHeader.FULLY_QUALIFIED_CLASS_NAME: fully_qualified_class_name,
+            TraceDataHeader.LINE: line_number,
+            TraceDataHeader.EVENT_TYPE: event_type,
+            TraceDataHeader.RETURN_VALUE: return_value,
+            TraceDataHeader.RETURN_TYPE: return_type,
+            TraceDataHeader.EXCEPTION_TYPE: exception_type,
+            TraceDataHeader.EXCEPTION_MESSAGE: exception_message,
+            TraceDataHeader.THREAD_ID: thread_id,
         }
         self._csv_data.append(data)
 
     def _get_class_names(
         self,
         code_qualified_name: str,
         function_name: str,
@@ -336,19 +336,19 @@
         self, file_name: str, code: CodeType, line_number: int
     ) -> bool:
         byte_code_iterator = dis.Bytecode(code)
         assert_found = False
         call_line_numbers = []
         for instruction in byte_code_iterator:
             byte_code_line_number = instruction.positions.lineno
-            if InstructionOpnames.CALL in instruction.opname:
+            if InstructionOpname.CALL in instruction.opname:
                 call_line_numbers.append(byte_code_line_number)
             if (
                 line_number == byte_code_line_number
-                and instruction.opname == InstructionOpnames.LOAD_ASSERTION_ERROR
+                and instruction.opname == InstructionOpname.LOAD_ASSERTION_ERROR
                 and (
                     line_number != self._line_of_last_assert
                     or file_name != self._file_of_last_assert
                 )
             ):
                 self._line_of_last_assert = line_number
                 self._file_of_last_assert = file_name
@@ -375,20 +375,20 @@
         byte_code_iterator = dis.Bytecode(code)
         is_assert = False
         calls = 0
         for instruction in byte_code_iterator:
             byte_code_line_number = instruction.positions.lineno
             if (
                 line_number == byte_code_line_number
-                and InstructionOpnames.CALL in instruction.opname
+                and InstructionOpname.CALL in instruction.opname
             ):
                 calls += 1
             if (
                 line_number == byte_code_line_number
-                and instruction.opname == InstructionOpnames.LOAD_ASSERTION_ERROR
+                and instruction.opname == InstructionOpname.LOAD_ASSERTION_ERROR
                 and (
                     line_number != self._line_of_last_assert
                     or file_name != self._file_of_last_assert
                 )
             ):
                 self._line_of_last_assert = line_number
                 self._file_of_last_assert = file_name
@@ -416,24 +416,24 @@
 
         for test_folder in self._test_folders:
             if file_name.startswith(test_folder):
                 if (
                     function_name == qualified_function_name
                     and qualified_function_name.startswith(TEST_CLASS_PREFIX)
                 ):
-                    return FunctionTypes.TEST_CLASS
+                    return FunctionType.TEST_CLASS
                 if self._check_is_assert(file_name, line_number, code):
-                    return FunctionTypes.ASSERT
+                    return FunctionType.ASSERT
                 if function_name.startswith(TEST_PREFIX):
-                    return FunctionTypes.TEST_FUNCTION
-                return FunctionTypes.TEST_HELPER
+                    return FunctionType.TEST_FUNCTION
+                return FunctionType.TEST_HELPER
 
         for source_folder in self._source_folders:
             if file_name.startswith(source_folder):
-                return FunctionTypes.SOURCE
+                return FunctionType.SOURCE
 
         return None
 
     def _save_assert_line_values(
         self,
         depth: int,
         function_type: str,
@@ -445,35 +445,35 @@
         event_type: str,
         return_value: str,
         return_type: str,
         testing_method: str,
         thread_id: int,
     ) -> None:
         assert_line_data = {
-            TraceDataVariables.DEPTH: depth,
-            TraceDataVariables.FUNCTION_TYPE: function_type,
-            TraceDataVariables.FUNCTION_NAME: function_name,
-            TraceDataVariables.FULLY_QUALIFIED_FUNCTION_NAME: fully_qualified_function_name,
-            TraceDataVariables.CLASS_NAME: class_name,
-            TraceDataVariables.FULLY_QUALIFIED_CLASS_NAME: fully_qualified_class_name,
-            TraceDataVariables.LINE_NUMBER: line_number,
-            TraceDataVariables.EVENT_TYPE: event_type,
-            TraceDataVariables.RETURN_VALUE: return_value,
-            TraceDataVariables.RETURN_TYPE: return_type,
-            TraceDataVariables.TESTING_METHOD: testing_method,
-            TraceDataVariables.THREAD_ID: thread_id,
+            TraceDataVariable.DEPTH: depth,
+            TraceDataVariable.FUNCTION_TYPE: function_type,
+            TraceDataVariable.FUNCTION_NAME: function_name,
+            TraceDataVariable.FULLY_QUALIFIED_FUNCTION_NAME: fully_qualified_function_name,
+            TraceDataVariable.CLASS_NAME: class_name,
+            TraceDataVariable.FULLY_QUALIFIED_CLASS_NAME: fully_qualified_class_name,
+            TraceDataVariable.LINE_NUMBER: line_number,
+            TraceDataVariable.EVENT_TYPE: event_type,
+            TraceDataVariable.RETURN_VALUE: return_value,
+            TraceDataVariable.RETURN_TYPE: return_type,
+            TraceDataVariable.TESTING_METHOD: testing_method,
+            TraceDataVariable.THREAD_ID: thread_id,
         }
         # Data of the line of trace occuring due to an in-line assert, so that we store
         # to add to the trace later
 
         self._assert_line_values.append(assert_line_data)
 
     def _check_remaining_in_line_functions(self, depth: int) -> bool:
         if self._in_line_functions_left_list:
-            prev_assert_depth = self._assert_line_values[-1][TraceDataVariables.DEPTH]
+            prev_assert_depth = self._assert_line_values[-1][TraceDataVariable.DEPTH]
             if prev_assert_depth == depth:
                 self._in_line_functions_left_list[-1] -= 1
                 if self._in_line_functions_left_list[-1] == 0:
                     self._in_line_functions_left_list.pop()
                     last_assert_values = self._assert_line_values.pop()
                     self._add_csv_row_data(**last_assert_values)
                 return True
```

### Comparing `pytctracer-0.1.8/pytctracer.egg-info/PKG-INFO` & `pytctracer-0.1.9/pytctracer.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pytctracer
-Version: 0.1.8
-Summary: CLI tool demonstrating test-to-code traceability techniques on Python codebases that use the Pytest testing framework.
+Version: 0.1.9
+Summary: Research library demonstrating test-to-code traceability techniques on Python codebases that use the Pytest testing framework.
 Author: Jason Ho
 Project-URL: Repository, https://github.com/jasonho2582001/comp0138-pytctracer
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -20,8 +20,12 @@
 Requires-Dist: pylint==3.1.0; extra == "dev"
 Requires-Dist: setuptools==69.2.0; extra == "dev"
 Requires-Dist: bump2version==1.0.1; extra == "dev"
 
 # PyTCTracer
 PyTCTracer is a test-to-code traceability approach and library, which allows for dynamic code tracing of Python repositories using the Pytest testing framework, and automatic generation of test-to-code traceability links from the trace data using a number of established traceability techniques. 
 
+There are two core components in the library:
+- `PytestTracer`: A class that is used to trace the execution of Pytest unit tests and record dynamic tracing information to a CSV log file.
+- `pytctracer` CLI: A CLI tool which can read and parse the dynamic information from the log file, apply traceability techniques to generate link predictions, and evaluate the predictions against a ground truth.
+
 This library forms part of an undergraduate research project for a Masters of Engineering in Computer Science at UCL (University College London).
```

### Comparing `pytctracer-0.1.8/pytctracer.egg-info/SOURCES.txt` & `pytctracer-0.1.9/pytctracer.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 pytctracer.egg-info/dependency_links.txt
 pytctracer.egg-info/entry_points.txt
 pytctracer.egg-info/requires.txt
 pytctracer.egg-info/top_level.txt
 pytctracer/config/__init__.py
 pytctracer/config/config.py
 pytctracer/config/constants/__init__.py
-pytctracer/config/constants/classification_types.py
-pytctracer/config/constants/event_types.py
-pytctracer/config/constants/function_types.py
-pytctracer/config/constants/instruction_opnames.py
-pytctracer/config/constants/level_types.py
-pytctracer/config/constants/metric_score_types.py
-pytctracer/config/constants/technique_parameters.py
-pytctracer/config/constants/technique_thresholds.py
-pytctracer/config/constants/testing_method_event_types.py
-pytctracer/config/constants/trace_data_headers.py
-pytctracer/config/constants/trace_data_variables.py
+pytctracer/config/constants/classification_type.py
+pytctracer/config/constants/event_type.py
+pytctracer/config/constants/function_type.py
+pytctracer/config/constants/instruction_opname.py
+pytctracer/config/constants/level_type.py
+pytctracer/config/constants/metric_score_type.py
+pytctracer/config/constants/technique_parameter.py
+pytctracer/config/constants/technique_threshold.py
+pytctracer/config/constants/testing_method_event_type.py
+pytctracer/config/constants/trace_data_header.py
+pytctracer/config/constants/trace_data_variable.py
 pytctracer/evaluation/__init__.py
 pytctracer/evaluation/classify_predictions.py
 pytctracer/evaluation/evaluate_predictions.py
 pytctracer/evaluation/metrics/__init__.py
 pytctracer/evaluation/metrics/area_under_curve.py
 pytctracer/evaluation/metrics/arg_name_to_metric_mapper.py
 pytctracer/evaluation/metrics/f1.py
```

