# Comparing `tmp/optima-ml-0.3.2a3.tar.gz` & `tmp/optima-ml-0.3.2a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optima-ml-0.3.2a3.tar", last modified: Sat Mar 30 12:35:03 2024, max compression
+gzip compressed data, was "optima-ml-0.3.2a4.tar", last modified: Fri Apr  5 11:57:50 2024, max compression
```

## Comparing `optima-ml-0.3.2a3.tar` & `optima-ml-0.3.2a4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-03-30 12:35:03.649588 optima-ml-0.3.2a3/
--rw-rw-r--   0 erik     (30000) erik     (30003)    35150 2023-08-12 13:57:40.000000 optima-ml-0.3.2a3/LICENSE
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-03-30 12:35:03.637588 optima-ml-0.3.2a3/OPTIMA/
--rw-rw-r--   0 erik     (30000) erik     (30003)      382 2024-01-30 16:21:26.000000 optima-ml-0.3.2a3/OPTIMA/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)      132 2023-08-12 13:57:39.000000 optima-ml-0.3.2a3/OPTIMA/__main__.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-03-30 12:35:03.641588 optima-ml-0.3.2a3/OPTIMA/builtin/
--rw-rw-r--   0 erik     (30000) erik     (30003)      137 2024-02-07 21:12:40.000000 optima-ml-0.3.2a3/OPTIMA/builtin/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    35186 2024-02-07 21:12:40.000000 optima-ml-0.3.2a3/OPTIMA/builtin/evaluation.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    32098 2024-02-07 21:12:40.000000 optima-ml-0.3.2a3/OPTIMA/builtin/figures_of_merit.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    66743 2024-03-23 18:21:18.000000 optima-ml-0.3.2a3/OPTIMA/builtin/inputs.py
--rw-rw-r--   0 erik     (30000) erik     (30003)      423 2024-03-30 12:27:00.000000 optima-ml-0.3.2a3/OPTIMA/builtin/model.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    15439 2024-02-15 12:31:11.000000 optima-ml-0.3.2a3/OPTIMA/builtin/search_space.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-03-30 12:35:03.641588 optima-ml-0.3.2a3/OPTIMA/core/
--rw-rw-r--   0 erik     (30000) erik     (30003)      114 2024-01-30 16:21:26.000000 optima-ml-0.3.2a3/OPTIMA/core/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    91727 2024-03-30 12:27:00.000000 optima-ml-0.3.2a3/OPTIMA/core/evaluation.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    19104 2024-03-23 18:05:57.000000 optima-ml-0.3.2a3/OPTIMA/core/inputs.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    10090 2024-03-30 12:27:00.000000 optima-ml-0.3.2a3/OPTIMA/core/model.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     8297 2024-03-23 18:21:18.000000 optima-ml-0.3.2a3/OPTIMA/core/search_space.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     3469 2024-03-23 18:53:01.000000 optima-ml-0.3.2a3/OPTIMA/core/tools.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    79736 2024-03-30 12:27:00.000000 optima-ml-0.3.2a3/OPTIMA/core/training.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    80215 2024-03-30 12:27:00.000000 optima-ml-0.3.2a3/OPTIMA/core/variable_optimization.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    15893 2024-03-30 12:27:00.000000 optima-ml-0.3.2a3/OPTIMA/defaults.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-03-30 12:35:03.641588 optima-ml-0.3.2a3/OPTIMA/hardware_configs/
--rw-rw-r--   0 erik     (30000) erik     (30003)     2823 2024-02-19 17:16:10.000000 optima-ml-0.3.2a3/OPTIMA/hardware_configs/Dresden_Taurus.py
--rw-rw-r--   0 erik     (30000) erik     (30003)      111 2024-01-30 16:21:26.000000 optima-ml-0.3.2a3/OPTIMA/hardware_configs/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    16772 2024-03-30 12:31:40.000000 optima-ml-0.3.2a3/OPTIMA/hardware_configs/common.py
--rw-rw-r--   0 erik     (30000) erik     (30003)      505 2024-02-19 18:33:13.000000 optima-ml-0.3.2a3/OPTIMA/hardware_configs/helpers.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-03-30 12:35:03.645588 optima-ml-0.3.2a3/OPTIMA/helpers/
--rw-rw-r--   0 erik     (30000) erik     (30003)       35 2024-01-30 16:21:26.000000 optima-ml-0.3.2a3/OPTIMA/helpers/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     4853 2024-01-30 16:21:26.000000 optima-ml-0.3.2a3/OPTIMA/helpers/extract_data_from_NTuples.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     8670 2024-03-30 12:33:29.000000 optima-ml-0.3.2a3/OPTIMA/helpers/manage_ray_nodes.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-03-30 12:35:03.645588 optima-ml-0.3.2a3/OPTIMA/keras/
--rw-rw-r--   0 erik     (30000) erik     (30003)      102 2024-01-30 16:21:26.000000 optima-ml-0.3.2a3/OPTIMA/keras/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    28626 2024-03-30 12:27:00.000000 optima-ml-0.3.2a3/OPTIMA/keras/model.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    53862 2024-03-30 12:27:00.000000 optima-ml-0.3.2a3/OPTIMA/keras/tools.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     3912 2024-03-30 12:27:00.000000 optima-ml-0.3.2a3/OPTIMA/keras/training.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-03-30 12:35:03.645588 optima-ml-0.3.2a3/OPTIMA/lightning/
--rw-rw-r--   0 erik     (30000) erik     (30003)      106 2024-01-30 16:23:00.000000 optima-ml-0.3.2a3/OPTIMA/lightning/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    10100 2024-03-24 16:56:32.000000 optima-ml-0.3.2a3/OPTIMA/lightning/inputs.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     6301 2024-01-30 16:21:26.000000 optima-ml-0.3.2a3/OPTIMA/lightning/training.py
--rwxrwxr-x   0 erik     (30000) erik     (30003)    98348 2024-03-30 12:32:13.000000 optima-ml-0.3.2a3/OPTIMA/optima.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-03-30 12:35:03.645588 optima-ml-0.3.2a3/OPTIMA/resources/
--rw-rw-r--   0 erik     (30000) erik     (30003)        0 2023-08-12 13:57:39.000000 optima-ml-0.3.2a3/OPTIMA/resources/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     4772 2024-03-20 17:10:29.000000 optima-ml-0.3.2a3/OPTIMA/resources/config_verification.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    48922 2024-03-23 18:53:01.000000 optima-ml-0.3.2a3/OPTIMA/resources/pbt_with_seed.py
--rw-r--r--   0 erik     (30000) erik     (30003)    88068 2024-03-30 12:35:03.649588 optima-ml-0.3.2a3/PKG-INFO
--rw-rw-r--   0 erik     (30000) erik     (30003)    86687 2024-03-24 18:08:57.000000 optima-ml-0.3.2a3/README.md
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-03-30 12:35:03.649588 optima-ml-0.3.2a3/optima_ml.egg-info/
--rw-r--r--   0 erik     (30000) erik     (30003)    88068 2024-03-30 12:35:03.000000 optima-ml-0.3.2a3/optima_ml.egg-info/PKG-INFO
--rw-rw-r--   0 erik     (30000) erik     (30003)     1342 2024-03-30 12:35:03.000000 optima-ml-0.3.2a3/optima_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)        1 2024-03-30 12:35:03.000000 optima-ml-0.3.2a3/optima_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)      102 2024-03-30 12:35:03.000000 optima-ml-0.3.2a3/optima_ml.egg-info/entry_points.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)      173 2024-03-30 12:35:03.000000 optima-ml-0.3.2a3/optima_ml.egg-info/requires.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)        7 2024-03-30 12:35:03.000000 optima-ml-0.3.2a3/optima_ml.egg-info/top_level.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)       38 2024-03-30 12:35:03.649588 optima-ml-0.3.2a3/setup.cfg
--rw-rw-r--   0 erik     (30000) erik     (30003)     4223 2024-03-23 18:53:01.000000 optima-ml-0.3.2a3/setup.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-03-30 12:35:03.649588 optima-ml-0.3.2a3/tests/
--rw-rw-r--   0 erik     (30000) erik     (30003)    37821 2024-03-30 12:27:00.000000 optima-ml-0.3.2a3/tests/test_builtin.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     8594 2024-02-07 21:12:40.000000 optima-ml-0.3.2a3/tests/test_core.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     6398 2024-01-30 16:21:26.000000 optima-ml-0.3.2a3/tests/test_integration.py
--rw-rw-rw-   0 erik     (30000) erik     (30003)     6399 2023-11-02 02:48:49.000000 optima-ml-0.3.2a3/tests/test_integration_sameMachine.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    56852 2024-03-24 16:53:28.000000 optima-ml-0.3.2a3/tests/test_preprocessing.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-05 11:57:50.744589 optima-ml-0.3.2a4/
+-rw-rw-r--   0 erik     (30000) erik     (30003)    35150 2023-08-12 13:57:40.000000 optima-ml-0.3.2a4/LICENSE
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-05 11:57:50.736590 optima-ml-0.3.2a4/OPTIMA/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      382 2024-01-30 16:21:26.000000 optima-ml-0.3.2a4/OPTIMA/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)      132 2023-08-12 13:57:39.000000 optima-ml-0.3.2a4/OPTIMA/__main__.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-05 11:57:50.740589 optima-ml-0.3.2a4/OPTIMA/builtin/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      137 2024-02-07 21:12:40.000000 optima-ml-0.3.2a4/OPTIMA/builtin/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    35186 2024-02-07 21:12:40.000000 optima-ml-0.3.2a4/OPTIMA/builtin/evaluation.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    32098 2024-02-07 21:12:40.000000 optima-ml-0.3.2a4/OPTIMA/builtin/figures_of_merit.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    66743 2024-03-23 18:21:18.000000 optima-ml-0.3.2a4/OPTIMA/builtin/inputs.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)      423 2024-04-04 10:43:33.000000 optima-ml-0.3.2a4/OPTIMA/builtin/model.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    15439 2024-02-15 12:31:11.000000 optima-ml-0.3.2a4/OPTIMA/builtin/search_space.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-05 11:57:50.740589 optima-ml-0.3.2a4/OPTIMA/core/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      114 2024-01-30 16:21:26.000000 optima-ml-0.3.2a4/OPTIMA/core/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    91727 2024-04-04 10:43:33.000000 optima-ml-0.3.2a4/OPTIMA/core/evaluation.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    19104 2024-03-23 18:05:57.000000 optima-ml-0.3.2a4/OPTIMA/core/inputs.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    10090 2024-04-04 10:43:33.000000 optima-ml-0.3.2a4/OPTIMA/core/model.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     8297 2024-03-23 18:21:18.000000 optima-ml-0.3.2a4/OPTIMA/core/search_space.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     3469 2024-03-23 18:53:01.000000 optima-ml-0.3.2a4/OPTIMA/core/tools.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    79736 2024-04-04 10:43:33.000000 optima-ml-0.3.2a4/OPTIMA/core/training.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    80215 2024-04-04 10:43:33.000000 optima-ml-0.3.2a4/OPTIMA/core/variable_optimization.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    16272 2024-04-05 11:41:05.000000 optima-ml-0.3.2a4/OPTIMA/defaults.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-05 11:57:50.740589 optima-ml-0.3.2a4/OPTIMA/hardware_configs/
+-rw-rw-r--   0 erik     (30000) erik     (30003)     2823 2024-02-19 17:16:10.000000 optima-ml-0.3.2a4/OPTIMA/hardware_configs/Dresden_Taurus.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)      111 2024-01-30 16:21:26.000000 optima-ml-0.3.2a4/OPTIMA/hardware_configs/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    16772 2024-03-30 12:31:40.000000 optima-ml-0.3.2a4/OPTIMA/hardware_configs/common.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)      505 2024-02-19 18:33:13.000000 optima-ml-0.3.2a4/OPTIMA/hardware_configs/helpers.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-05 11:57:50.740589 optima-ml-0.3.2a4/OPTIMA/helpers/
+-rw-rw-r--   0 erik     (30000) erik     (30003)       35 2024-01-30 16:21:26.000000 optima-ml-0.3.2a4/OPTIMA/helpers/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     4853 2024-01-30 16:21:26.000000 optima-ml-0.3.2a4/OPTIMA/helpers/extract_data_from_NTuples.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     8670 2024-04-04 10:43:33.000000 optima-ml-0.3.2a4/OPTIMA/helpers/manage_ray_nodes.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-05 11:57:50.740589 optima-ml-0.3.2a4/OPTIMA/keras/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      102 2024-01-30 16:21:26.000000 optima-ml-0.3.2a4/OPTIMA/keras/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    28626 2024-04-04 10:43:33.000000 optima-ml-0.3.2a4/OPTIMA/keras/model.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    53862 2024-04-04 10:43:33.000000 optima-ml-0.3.2a4/OPTIMA/keras/tools.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     3912 2024-04-04 10:43:33.000000 optima-ml-0.3.2a4/OPTIMA/keras/training.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-05 11:57:50.744589 optima-ml-0.3.2a4/OPTIMA/lightning/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      106 2024-01-30 16:23:00.000000 optima-ml-0.3.2a4/OPTIMA/lightning/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    10100 2024-03-24 16:56:32.000000 optima-ml-0.3.2a4/OPTIMA/lightning/inputs.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     6301 2024-01-30 16:21:26.000000 optima-ml-0.3.2a4/OPTIMA/lightning/training.py
+-rwxrwxr-x   0 erik     (30000) erik     (30003)    98442 2024-04-05 11:55:00.000000 optima-ml-0.3.2a4/OPTIMA/optima.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-05 11:57:50.744589 optima-ml-0.3.2a4/OPTIMA/resources/
+-rw-rw-r--   0 erik     (30000) erik     (30003)        0 2023-08-12 13:57:39.000000 optima-ml-0.3.2a4/OPTIMA/resources/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     4772 2024-03-20 17:10:29.000000 optima-ml-0.3.2a4/OPTIMA/resources/config_verification.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    48922 2024-03-23 18:53:01.000000 optima-ml-0.3.2a4/OPTIMA/resources/pbt_with_seed.py
+-rw-r--r--   0 erik     (30000) erik     (30003)    88892 2024-04-05 11:57:50.744589 optima-ml-0.3.2a4/PKG-INFO
+-rw-rw-r--   0 erik     (30000) erik     (30003)    87511 2024-04-05 11:54:01.000000 optima-ml-0.3.2a4/README.md
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-05 11:57:50.744589 optima-ml-0.3.2a4/optima_ml.egg-info/
+-rw-r--r--   0 erik     (30000) erik     (30003)    88892 2024-04-05 11:57:50.000000 optima-ml-0.3.2a4/optima_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 erik     (30000) erik     (30003)     1342 2024-04-05 11:57:50.000000 optima-ml-0.3.2a4/optima_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)        1 2024-04-05 11:57:50.000000 optima-ml-0.3.2a4/optima_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)      102 2024-04-05 11:57:50.000000 optima-ml-0.3.2a4/optima_ml.egg-info/entry_points.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)      173 2024-04-05 11:57:50.000000 optima-ml-0.3.2a4/optima_ml.egg-info/requires.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)        7 2024-04-05 11:57:50.000000 optima-ml-0.3.2a4/optima_ml.egg-info/top_level.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)       38 2024-04-05 11:57:50.744589 optima-ml-0.3.2a4/setup.cfg
+-rw-rw-r--   0 erik     (30000) erik     (30003)     4223 2024-03-23 18:53:01.000000 optima-ml-0.3.2a4/setup.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-05 11:57:50.744589 optima-ml-0.3.2a4/tests/
+-rw-rw-r--   0 erik     (30000) erik     (30003)    37821 2024-04-04 10:43:33.000000 optima-ml-0.3.2a4/tests/test_builtin.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     8594 2024-02-07 21:12:40.000000 optima-ml-0.3.2a4/tests/test_core.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     6398 2024-01-30 16:21:26.000000 optima-ml-0.3.2a4/tests/test_integration.py
+-rw-rw-rw-   0 erik     (30000) erik     (30003)     6399 2023-11-02 02:48:49.000000 optima-ml-0.3.2a4/tests/test_integration_sameMachine.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    56852 2024-03-24 16:53:28.000000 optima-ml-0.3.2a4/tests/test_preprocessing.py
```

### Comparing `optima-ml-0.3.2a3/LICENSE` & `optima-ml-0.3.2a4/LICENSE`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/OPTIMA/builtin/evaluation.py` & `optima-ml-0.3.2a4/OPTIMA/builtin/evaluation.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/OPTIMA/builtin/figures_of_merit.py` & `optima-ml-0.3.2a4/OPTIMA/builtin/figures_of_merit.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/OPTIMA/builtin/inputs.py` & `optima-ml-0.3.2a4/OPTIMA/builtin/inputs.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/OPTIMA/builtin/search_space.py` & `optima-ml-0.3.2a4/OPTIMA/builtin/search_space.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/OPTIMA/core/evaluation.py` & `optima-ml-0.3.2a4/OPTIMA/core/evaluation.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/OPTIMA/core/inputs.py` & `optima-ml-0.3.2a4/OPTIMA/core/inputs.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/OPTIMA/core/model.py` & `optima-ml-0.3.2a4/OPTIMA/core/model.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/OPTIMA/core/search_space.py` & `optima-ml-0.3.2a4/OPTIMA/core/search_space.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/OPTIMA/core/tools.py` & `optima-ml-0.3.2a4/OPTIMA/core/tools.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/OPTIMA/core/training.py` & `optima-ml-0.3.2a4/OPTIMA/core/training.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/OPTIMA/core/variable_optimization.py` & `optima-ml-0.3.2a4/OPTIMA/core/variable_optimization.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/OPTIMA/defaults.py` & `optima-ml-0.3.2a4/OPTIMA/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,19 @@
 num_repeats_hybrid_retrain = 1  # how often should each variable set be evaluated per iteration in the second phase of hybrid mode (retrain); not used if variable_optimization_mode != 'hybrid'
 reevaluate_candidate_to_drop = True  # if True: instead of using the metric value after variable drop directly, an additional evaluation set is performed for the best variable set in each iteration to get an unbiased performance estimate
 retrain_for_reevaluation = True  # if True: instead of using the original evaluation method used for each variable set, the re-evaluation for the baseline uses the retrain method
 num_repeats_for_reevaluation = 2  # the number of times the re-evaluation of the best variable set should be done
 use_median_for_averages = False  # if True: use the median and MAD to calculate averages and uncertainties across the k folds, otherwise use mean and standard deviation
 use_fit_results_for_varOpt = True  # whether to use the hyperparameters from the best fit or highest metric value of the initial hyperoptimization step
 
+# a list of references to a callback class (specific for the used ML framework, i.e. a subclass of keras.callbacks.Callback for Keras or lightning.pytorch.callbacks.Callback for Lightning) in the form (ClassName, {"kwarg1": kwarg1, ...}. They are only used during the model training.
+callbacks = [
+    # (tf.keras.callbacks.ReduceLROnPlateau, {"patience": 10, "factor": 0.2})
+]
+
 # list of references to a metric class (native to the used ML framework) in the form (name, (ClassName, {"kwarg1": kwarg1, ...})). Their values are calculated without applying event weights.
 native_metrics = [
     # ('binary_accuracy', (tf.keras.metrics.BinaryAccuracy, {"threshold": 0.75}))
     # ('lightning_accuracy', (torchmetrics.classification.BinaryAccuracy, {"threshold": 0.5})),,
 ]
 
 # list of references to a metric class (native to the used ML framework) in the form (name, (ClassName, {"kwarg1": kwarg1, ...})). Their values are calculated using the event weights.
```

### Comparing `optima-ml-0.3.2a3/OPTIMA/hardware_configs/Dresden_Taurus.py` & `optima-ml-0.3.2a4/OPTIMA/hardware_configs/Dresden_Taurus.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/OPTIMA/hardware_configs/common.py` & `optima-ml-0.3.2a4/OPTIMA/hardware_configs/common.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/OPTIMA/helpers/extract_data_from_NTuples.py` & `optima-ml-0.3.2a4/OPTIMA/helpers/extract_data_from_NTuples.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/OPTIMA/helpers/manage_ray_nodes.py` & `optima-ml-0.3.2a4/OPTIMA/helpers/manage_ray_nodes.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/OPTIMA/keras/model.py` & `optima-ml-0.3.2a4/OPTIMA/keras/model.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/OPTIMA/keras/tools.py` & `optima-ml-0.3.2a4/OPTIMA/keras/tools.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/OPTIMA/keras/training.py` & `optima-ml-0.3.2a4/OPTIMA/keras/training.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/OPTIMA/lightning/inputs.py` & `optima-ml-0.3.2a4/OPTIMA/lightning/inputs.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/OPTIMA/lightning/training.py` & `optima-ml-0.3.2a4/OPTIMA/lightning/training.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/OPTIMA/optima.py` & `optima-ml-0.3.2a4/OPTIMA/optima.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Main steering script of OPTIMA."""
 
 __author__ = "E. Bachmann"
 __licence__ = "GPL3"
-__version__ = "0.3.2alpha3"
+__version__ = "0.3.2alpha4"
 __maintainer__ = "E. Bachmann"
 
 import os
 import sys
 import shutil
 import logging
 import argparse
@@ -329,29 +329,29 @@
             logging.warning(f"Starting the subprocess and prepare training took {time.time()-start_time}s which may be a performance bottleneck.")
 
         if run_config.model_type == "Keras":
             model.fit(
                 train_data,
                 validation_data=val_data,
                 epochs=model_config["max_epochs"],
-                callbacks=[early_stopper],
+                callbacks=[early_stopper, *[c[0](**c[1]) for c in run_config.callbacks]],
                 verbose=verbose
             )
         elif run_config.model_type == "Lightning":
             # set correct number of cpu cores; TODO: this for some reason currently only works with pytorch-gpu and is ignored by pytorch??
             from torch import get_num_threads, get_num_interop_threads, set_num_threads, set_num_interop_threads
             if get_num_threads() != num_threads:
                 set_num_threads(num_threads)
             if get_num_interop_threads() != min(num_threads, 2):
                 set_num_interop_threads(min(num_threads, 2))
 
             # currently, the device summary cannot be disabled. TODO: check if this has changed
             trainer = pl.Trainer(
                 max_epochs=model_config["max_epochs"],
-                callbacks=[early_stopper],
+                callbacks=[early_stopper, *[c[0](**c[1]) for c in run_config.callbacks]],
                 devices='auto',
                 accelerator='auto',
                 num_sanity_val_steps=0,  # this messes with the reporting to Tune since it calls the Callbacks
                 enable_progress_bar=False,
                 enable_model_summary=False,
                 logger=False,  # logging is done via Tune
                 enable_checkpointing=False,  # checkpointing is done in the early stopper
```

### Comparing `optima-ml-0.3.2a3/OPTIMA/resources/config_verification.py` & `optima-ml-0.3.2a4/OPTIMA/resources/config_verification.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/OPTIMA/resources/pbt_with_seed.py` & `optima-ml-0.3.2a4/OPTIMA/resources/pbt_with_seed.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/PKG-INFO` & `optima-ml-0.3.2a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optima-ml
-Version: 0.3.2a3
+Version: 0.3.2a4
 Summary: Distributed hyperparameter optimization and input variable selection for artificial neural networks.
 Home-page: https://gitlab.cern.ch/atlas-germany-dresden-vbs-group/optima
 Author: E. Bachmann
 Author-email: erik.bachmann@tu-dresden.de
 License: GPL
 Platform: linux
 Platform: darwin
@@ -384,27 +384,28 @@
 
 #### Evaluation
 
 | Parameter                          | Default value | Explanation                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
 |------------------------------------|---------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `monitor_name` *(str)*             | `'val_loss'`  | Controls which metric is used as the target of the optimization and for early stopping during training. Allowed are native, weighted native, custom and composite metrics as well as all metrics reported by the ML backend during training (e.g. `"val_loss"`). Make sure to add the `"val_"`-prefix when using native, weighted native or custom metrics.                                                                                                                                                                                                                                                                                                                                                                |
 | `monitor_op` *(str)*               | `'min'`       | Is the target metric to be minimized (`'min'`) or maximized (`'max'`)?                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
-| `native_metrics` *(list)*          | `[]`          | A list of references to a metric class native to the used ML backend. Each entry must be a tuple of the form `("name", (ClassName, {"kwarg1": kwarg1, ...}))`. Their values are calculated separately on the training and validation datasets and reported as `"train_name" and "val_name". Event weights are not applied.                                                                                                                                                                                                                                                                                                                                                                                                 |
-| `weighted_native_metrics` *(list)* | `[]`          | A list of references to a metric class native to the used ML backend. Each entry must be a tuple of the form `("name", (ClassName, {"kwarg1": kwarg1, ...}))`. Their values are calculated separately on the training and validation datasets and reported as `"train_name" and "val_name". Event weights are applied. Currently, weighted metrics are not supported for Lightning (see https://github.com/Lightning-AI/torchmetrics/issues/784).                                                                                                                                                                                                                                                                          |
+| `native_metrics` *(list)*          | `[]`          | A list of references to a metric class native to the used ML backend. Each entry must be a tuple of the form `("name", (ClassReference, {"kwarg1": kwarg1, ...}))`. Their values are calculated separately on the training and validation datasets and reported as `"train_name" and "val_name". Event weights are not applied.                                                                                                                                                                                                                                                                                                                                                                                            |
+| `weighted_native_metrics` *(list)* | `[]`          | A list of references to a metric class native to the used ML backend. Each entry must be a tuple of the form `("name", (ClassReference, {"kwarg1": kwarg1, ...}))`. Their values are calculated separately on the training and validation datasets and reported as `"train_name" and "val_name". Event weights are applied. Currently, weighted metrics are not supported for Lightning (see https://github.com/Lightning-AI/torchmetrics/issues/784).                                                                                                                                                                                                                                                                     |
 | `custom_metrics` *(list)*          | `[]`          | A list of custom metrics. Each entry must be a tuple of the form `("name", callable)`. `callable` needs to accept target values, model prediction and sample weights and return a number or a boolean. Their values are calculated at the end of each epoch separately on the training and validation datasets and reported as `"train_name" and "val_name".                                                                                                                                                                                                                                                                                                                                                               |
 | `composite_metrics` *(list)*       | `[]`          | A list of composite metrics. These are metrics that combine the values of already existing metrics. Each entry must be a tuple of the form `("name", (metric_name1, metric_name2, ...), callable)` where `callable` accepts the same number of positional arguments as the number of provided metric names and returns a number or a boolean. They are calculated at the end of each epoch and allow all native, weighted native and custom metrics as well as metrics directly reported by the ML backend (e.g. validation loss) as inputs. It is possible to mix training and validation metrics, allowing e.g. to assess the generalization gap. The value of composite metrics is reported as "name" without a prefix. |
 | `overtraining_conditions` *(list)* | `[]`          | A list of overtraining conditions. Thse are special composite metrics that should return `True` when overtraining is detected and `False` otherwise. Each entry must be a tuple of the form `("name", (metric_name1, metric_name2, ...), callable)` where `callable` accepts the same number of positional arguments as the number of provided metric names and returns a boolean. They are calculated at the end of each epoch and allow all native, weighted native, custom and composite metrics as well as metrics directly reported by the ML backend (e.g. validation loss) as inputs. Naturally, it is possible to mix training and validation metrics. The value of overtraining conditions is not reported.       |
 
 #### Training
 
-| Parameter                         | Default value | Explanation                                                                                                                                                                                                                         |
-|-----------------------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `max_epochs` *(int)*              | `200`         | The maximal number of epochs until the training is terminated. Early stopping may terminate the training earlier.                                                                                                                   |
-| `early_stopping_patience` *(int)* | `6`           | The maximal number of consecutive epochs without an improvement of the target metric before early-stopping the training.                                                                                                            |
-| `overtraining_patience` *(int)*   | `6`           | The maximal number of consecutive epochs with overtraining detected (i.e. at least one overtraining condition detected overtraining) before early-stopping the training. This is ignored if no overtraining conditions are defined. |
+| Parameter                         | Default value | Explanation                                                                                                                                                                                                                                                                                                                   |
+|-----------------------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `max_epochs` *(int)*              | `200`         | The maximal number of epochs until the training is terminated. Early stopping may terminate the training earlier.                                                                                                                                                                                                             |
+| `early_stopping_patience` *(int)* | `6`           | The maximal number of consecutive epochs without an improvement of the target metric before early-stopping the training.                                                                                                                                                                                                      |
+| `overtraining_patience` *(int)*   | `6`           | The maximal number of consecutive epochs with overtraining detected (i.e. at least one overtraining condition detected overtraining) before early-stopping the training. This is ignored if no overtraining conditions are defined.                                                                                           |
+| `callbacks` *(list)*              | `[]`          | A list of references to a callback class native to the used ML backend (i.e. a subclass of `keras.callbacks.Callback` for Keras or `lightning.pytorch.callbacks.Callback` for Lightning. Each entry must be a tuple of the form `(ClassReference, {"kwarg1": kwarg1, ...})`. The callbacks are only used during the training. |
 
 #### Hyperparameter optimization
 
 ##### General
 
 | Parameter                             | Default value                                                                                                                 | Explanation                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
 |---------------------------------------|-------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
```

### Comparing `optima-ml-0.3.2a3/README.md` & `optima-ml-0.3.2a4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -346,27 +346,28 @@
 
 #### Evaluation
 
 | Parameter                          | Default value | Explanation                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
 |------------------------------------|---------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `monitor_name` *(str)*             | `'val_loss'`  | Controls which metric is used as the target of the optimization and for early stopping during training. Allowed are native, weighted native, custom and composite metrics as well as all metrics reported by the ML backend during training (e.g. `"val_loss"`). Make sure to add the `"val_"`-prefix when using native, weighted native or custom metrics.                                                                                                                                                                                                                                                                                                                                                                |
 | `monitor_op` *(str)*               | `'min'`       | Is the target metric to be minimized (`'min'`) or maximized (`'max'`)?                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
-| `native_metrics` *(list)*          | `[]`          | A list of references to a metric class native to the used ML backend. Each entry must be a tuple of the form `("name", (ClassName, {"kwarg1": kwarg1, ...}))`. Their values are calculated separately on the training and validation datasets and reported as `"train_name" and "val_name". Event weights are not applied.                                                                                                                                                                                                                                                                                                                                                                                                 |
-| `weighted_native_metrics` *(list)* | `[]`          | A list of references to a metric class native to the used ML backend. Each entry must be a tuple of the form `("name", (ClassName, {"kwarg1": kwarg1, ...}))`. Their values are calculated separately on the training and validation datasets and reported as `"train_name" and "val_name". Event weights are applied. Currently, weighted metrics are not supported for Lightning (see https://github.com/Lightning-AI/torchmetrics/issues/784).                                                                                                                                                                                                                                                                          |
+| `native_metrics` *(list)*          | `[]`          | A list of references to a metric class native to the used ML backend. Each entry must be a tuple of the form `("name", (ClassReference, {"kwarg1": kwarg1, ...}))`. Their values are calculated separately on the training and validation datasets and reported as `"train_name" and "val_name". Event weights are not applied.                                                                                                                                                                                                                                                                                                                                                                                            |
+| `weighted_native_metrics` *(list)* | `[]`          | A list of references to a metric class native to the used ML backend. Each entry must be a tuple of the form `("name", (ClassReference, {"kwarg1": kwarg1, ...}))`. Their values are calculated separately on the training and validation datasets and reported as `"train_name" and "val_name". Event weights are applied. Currently, weighted metrics are not supported for Lightning (see https://github.com/Lightning-AI/torchmetrics/issues/784).                                                                                                                                                                                                                                                                     |
 | `custom_metrics` *(list)*          | `[]`          | A list of custom metrics. Each entry must be a tuple of the form `("name", callable)`. `callable` needs to accept target values, model prediction and sample weights and return a number or a boolean. Their values are calculated at the end of each epoch separately on the training and validation datasets and reported as `"train_name" and "val_name".                                                                                                                                                                                                                                                                                                                                                               |
 | `composite_metrics` *(list)*       | `[]`          | A list of composite metrics. These are metrics that combine the values of already existing metrics. Each entry must be a tuple of the form `("name", (metric_name1, metric_name2, ...), callable)` where `callable` accepts the same number of positional arguments as the number of provided metric names and returns a number or a boolean. They are calculated at the end of each epoch and allow all native, weighted native and custom metrics as well as metrics directly reported by the ML backend (e.g. validation loss) as inputs. It is possible to mix training and validation metrics, allowing e.g. to assess the generalization gap. The value of composite metrics is reported as "name" without a prefix. |
 | `overtraining_conditions` *(list)* | `[]`          | A list of overtraining conditions. Thse are special composite metrics that should return `True` when overtraining is detected and `False` otherwise. Each entry must be a tuple of the form `("name", (metric_name1, metric_name2, ...), callable)` where `callable` accepts the same number of positional arguments as the number of provided metric names and returns a boolean. They are calculated at the end of each epoch and allow all native, weighted native, custom and composite metrics as well as metrics directly reported by the ML backend (e.g. validation loss) as inputs. Naturally, it is possible to mix training and validation metrics. The value of overtraining conditions is not reported.       |
 
 #### Training
 
-| Parameter                         | Default value | Explanation                                                                                                                                                                                                                         |
-|-----------------------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `max_epochs` *(int)*              | `200`         | The maximal number of epochs until the training is terminated. Early stopping may terminate the training earlier.                                                                                                                   |
-| `early_stopping_patience` *(int)* | `6`           | The maximal number of consecutive epochs without an improvement of the target metric before early-stopping the training.                                                                                                            |
-| `overtraining_patience` *(int)*   | `6`           | The maximal number of consecutive epochs with overtraining detected (i.e. at least one overtraining condition detected overtraining) before early-stopping the training. This is ignored if no overtraining conditions are defined. |
+| Parameter                         | Default value | Explanation                                                                                                                                                                                                                                                                                                                   |
+|-----------------------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `max_epochs` *(int)*              | `200`         | The maximal number of epochs until the training is terminated. Early stopping may terminate the training earlier.                                                                                                                                                                                                             |
+| `early_stopping_patience` *(int)* | `6`           | The maximal number of consecutive epochs without an improvement of the target metric before early-stopping the training.                                                                                                                                                                                                      |
+| `overtraining_patience` *(int)*   | `6`           | The maximal number of consecutive epochs with overtraining detected (i.e. at least one overtraining condition detected overtraining) before early-stopping the training. This is ignored if no overtraining conditions are defined.                                                                                           |
+| `callbacks` *(list)*              | `[]`          | A list of references to a callback class native to the used ML backend (i.e. a subclass of `keras.callbacks.Callback` for Keras or `lightning.pytorch.callbacks.Callback` for Lightning. Each entry must be a tuple of the form `(ClassReference, {"kwarg1": kwarg1, ...})`. The callbacks are only used during the training. |
 
 #### Hyperparameter optimization
 
 ##### General
 
 | Parameter                             | Default value                                                                                                                 | Explanation                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
 |---------------------------------------|-------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
```

### Comparing `optima-ml-0.3.2a3/optima_ml.egg-info/PKG-INFO` & `optima-ml-0.3.2a4/optima_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optima-ml
-Version: 0.3.2a3
+Version: 0.3.2a4
 Summary: Distributed hyperparameter optimization and input variable selection for artificial neural networks.
 Home-page: https://gitlab.cern.ch/atlas-germany-dresden-vbs-group/optima
 Author: E. Bachmann
 Author-email: erik.bachmann@tu-dresden.de
 License: GPL
 Platform: linux
 Platform: darwin
@@ -384,27 +384,28 @@
 
 #### Evaluation
 
 | Parameter                          | Default value | Explanation                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
 |------------------------------------|---------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `monitor_name` *(str)*             | `'val_loss'`  | Controls which metric is used as the target of the optimization and for early stopping during training. Allowed are native, weighted native, custom and composite metrics as well as all metrics reported by the ML backend during training (e.g. `"val_loss"`). Make sure to add the `"val_"`-prefix when using native, weighted native or custom metrics.                                                                                                                                                                                                                                                                                                                                                                |
 | `monitor_op` *(str)*               | `'min'`       | Is the target metric to be minimized (`'min'`) or maximized (`'max'`)?                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
-| `native_metrics` *(list)*          | `[]`          | A list of references to a metric class native to the used ML backend. Each entry must be a tuple of the form `("name", (ClassName, {"kwarg1": kwarg1, ...}))`. Their values are calculated separately on the training and validation datasets and reported as `"train_name" and "val_name". Event weights are not applied.                                                                                                                                                                                                                                                                                                                                                                                                 |
-| `weighted_native_metrics` *(list)* | `[]`          | A list of references to a metric class native to the used ML backend. Each entry must be a tuple of the form `("name", (ClassName, {"kwarg1": kwarg1, ...}))`. Their values are calculated separately on the training and validation datasets and reported as `"train_name" and "val_name". Event weights are applied. Currently, weighted metrics are not supported for Lightning (see https://github.com/Lightning-AI/torchmetrics/issues/784).                                                                                                                                                                                                                                                                          |
+| `native_metrics` *(list)*          | `[]`          | A list of references to a metric class native to the used ML backend. Each entry must be a tuple of the form `("name", (ClassReference, {"kwarg1": kwarg1, ...}))`. Their values are calculated separately on the training and validation datasets and reported as `"train_name" and "val_name". Event weights are not applied.                                                                                                                                                                                                                                                                                                                                                                                            |
+| `weighted_native_metrics` *(list)* | `[]`          | A list of references to a metric class native to the used ML backend. Each entry must be a tuple of the form `("name", (ClassReference, {"kwarg1": kwarg1, ...}))`. Their values are calculated separately on the training and validation datasets and reported as `"train_name" and "val_name". Event weights are applied. Currently, weighted metrics are not supported for Lightning (see https://github.com/Lightning-AI/torchmetrics/issues/784).                                                                                                                                                                                                                                                                     |
 | `custom_metrics` *(list)*          | `[]`          | A list of custom metrics. Each entry must be a tuple of the form `("name", callable)`. `callable` needs to accept target values, model prediction and sample weights and return a number or a boolean. Their values are calculated at the end of each epoch separately on the training and validation datasets and reported as `"train_name" and "val_name".                                                                                                                                                                                                                                                                                                                                                               |
 | `composite_metrics` *(list)*       | `[]`          | A list of composite metrics. These are metrics that combine the values of already existing metrics. Each entry must be a tuple of the form `("name", (metric_name1, metric_name2, ...), callable)` where `callable` accepts the same number of positional arguments as the number of provided metric names and returns a number or a boolean. They are calculated at the end of each epoch and allow all native, weighted native and custom metrics as well as metrics directly reported by the ML backend (e.g. validation loss) as inputs. It is possible to mix training and validation metrics, allowing e.g. to assess the generalization gap. The value of composite metrics is reported as "name" without a prefix. |
 | `overtraining_conditions` *(list)* | `[]`          | A list of overtraining conditions. Thse are special composite metrics that should return `True` when overtraining is detected and `False` otherwise. Each entry must be a tuple of the form `("name", (metric_name1, metric_name2, ...), callable)` where `callable` accepts the same number of positional arguments as the number of provided metric names and returns a boolean. They are calculated at the end of each epoch and allow all native, weighted native, custom and composite metrics as well as metrics directly reported by the ML backend (e.g. validation loss) as inputs. Naturally, it is possible to mix training and validation metrics. The value of overtraining conditions is not reported.       |
 
 #### Training
 
-| Parameter                         | Default value | Explanation                                                                                                                                                                                                                         |
-|-----------------------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `max_epochs` *(int)*              | `200`         | The maximal number of epochs until the training is terminated. Early stopping may terminate the training earlier.                                                                                                                   |
-| `early_stopping_patience` *(int)* | `6`           | The maximal number of consecutive epochs without an improvement of the target metric before early-stopping the training.                                                                                                            |
-| `overtraining_patience` *(int)*   | `6`           | The maximal number of consecutive epochs with overtraining detected (i.e. at least one overtraining condition detected overtraining) before early-stopping the training. This is ignored if no overtraining conditions are defined. |
+| Parameter                         | Default value | Explanation                                                                                                                                                                                                                                                                                                                   |
+|-----------------------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `max_epochs` *(int)*              | `200`         | The maximal number of epochs until the training is terminated. Early stopping may terminate the training earlier.                                                                                                                                                                                                             |
+| `early_stopping_patience` *(int)* | `6`           | The maximal number of consecutive epochs without an improvement of the target metric before early-stopping the training.                                                                                                                                                                                                      |
+| `overtraining_patience` *(int)*   | `6`           | The maximal number of consecutive epochs with overtraining detected (i.e. at least one overtraining condition detected overtraining) before early-stopping the training. This is ignored if no overtraining conditions are defined.                                                                                           |
+| `callbacks` *(list)*              | `[]`          | A list of references to a callback class native to the used ML backend (i.e. a subclass of `keras.callbacks.Callback` for Keras or `lightning.pytorch.callbacks.Callback` for Lightning. Each entry must be a tuple of the form `(ClassReference, {"kwarg1": kwarg1, ...})`. The callbacks are only used during the training. |
 
 #### Hyperparameter optimization
 
 ##### General
 
 | Parameter                             | Default value                                                                                                                 | Explanation                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
 |---------------------------------------|-------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
```

### Comparing `optima-ml-0.3.2a3/optima_ml.egg-info/SOURCES.txt` & `optima-ml-0.3.2a4/optima_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/setup.py` & `optima-ml-0.3.2a4/setup.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/tests/test_builtin.py` & `optima-ml-0.3.2a4/tests/test_builtin.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/tests/test_core.py` & `optima-ml-0.3.2a4/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/tests/test_integration.py` & `optima-ml-0.3.2a4/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/tests/test_integration_sameMachine.py` & `optima-ml-0.3.2a4/tests/test_integration_sameMachine.py`

 * *Files identical despite different names*

### Comparing `optima-ml-0.3.2a3/tests/test_preprocessing.py` & `optima-ml-0.3.2a4/tests/test_preprocessing.py`

 * *Files identical despite different names*

