# Comparing `tmp/ecallisto_ng-0.7.11.tar.gz` & `tmp/ecallisto_ng-0.7.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecallisto_ng-0.7.11.tar", last modified: Wed Feb 28 16:22:18 2024, max compression
+gzip compressed data, was "ecallisto_ng-0.7.12.tar", last modified: Fri Apr  5 13:06:13 2024, max compression
```

## Comparing `ecallisto_ng-0.7.11.tar` & `ecallisto_ng-0.7.12.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2024-02-28 16:22:18.517049 ecallisto_ng-0.7.11/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-09-04 12:44:04.000000 ecallisto_ng-0.7.11/LICENSE
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       57 2023-12-04 16:26:22.000000 ecallisto_ng-0.7.11/MANIFEST.in
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     8973 2024-02-28 16:22:18.507049 ecallisto_ng-0.7.11/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     7432 2024-02-08 11:52:29.000000 ecallisto_ng-0.7.11/README.md
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1125 2024-02-28 16:22:02.000000 ecallisto_ng-0.7.11/pyproject.toml
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2024-02-28 16:22:18.517049 ecallisto_ng-0.7.11/setup.cfg
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2024-02-28 16:22:18.507049 ecallisto_ng-0.7.11/src/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-09-04 12:44:04.000000 ecallisto_ng-0.7.11/src/__init__.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2024-02-28 16:22:18.507049 ecallisto_ng-0.7.11/src/ecallisto_ng/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-09-04 12:44:04.000000 ecallisto_ng-0.7.11/src/ecallisto_ng/__init__.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2024-02-28 16:22:18.507049 ecallisto_ng-0.7.11/src/ecallisto_ng/burst_list/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-11-30 16:27:05.000000 ecallisto_ng-0.7.11/src/ecallisto_ng/burst_list/__init__.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2024-02-28 16:22:18.507049 ecallisto_ng-0.7.11/src/ecallisto_ng/burst_list/data/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)  1415009 2023-11-30 16:20:50.000000 ecallisto_ng-0.7.11/src/ecallisto_ng/burst_list/data/burst_list.xlsx
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1387 2023-11-30 16:30:41.000000 ecallisto_ng-0.7.11/src/ecallisto_ng/burst_list/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2024-02-28 16:22:18.507049 ecallisto_ng-0.7.11/src/ecallisto_ng/combine_antennas/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-10-03 15:11:40.000000 ecallisto_ng-0.7.11/src/ecallisto_ng/combine_antennas/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5459 2024-02-08 17:04:26.000000 ecallisto_ng-0.7.11/src/ecallisto_ng/combine_antennas/combine.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     8867 2024-02-08 16:30:10.000000 ecallisto_ng-0.7.11/src/ecallisto_ng/combine_antennas/utils.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2809 2024-02-08 17:14:24.000000 ecallisto_ng-0.7.11/src/ecallisto_ng/combine_antennas/virtualantenna.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2024-02-28 16:22:18.507049 ecallisto_ng-0.7.11/src/ecallisto_ng/data_download/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-11-06 17:18:04.000000 ecallisto_ng-0.7.11/src/ecallisto_ng/data_download/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)    13874 2024-02-28 16:21:25.000000 ecallisto_ng-0.7.11/src/ecallisto_ng/data_download/downloader.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)    11095 2023-11-23 22:45:30.000000 ecallisto_ng-0.7.11/src/ecallisto_ng/data_download/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2024-02-28 16:22:18.507049 ecallisto_ng-0.7.11/src/ecallisto_ng/data_fetching/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-09-04 12:44:04.000000 ecallisto_ng-0.7.11/src/ecallisto_ng/data_fetching/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)    10427 2023-11-13 13:42:26.000000 ecallisto_ng-0.7.11/src/ecallisto_ng/data_fetching/get_data.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     4680 2023-09-04 12:44:04.000000 ecallisto_ng-0.7.11/src/ecallisto_ng/data_fetching/get_information.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2024-02-28 16:22:18.507049 ecallisto_ng-0.7.11/src/ecallisto_ng/data_processing/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-09-04 12:44:04.000000 ecallisto_ng-0.7.11/src/ecallisto_ng/data_processing/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     9986 2024-02-08 17:04:31.000000 ecallisto_ng-0.7.11/src/ecallisto_ng/data_processing/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2024-02-28 16:22:18.507049 ecallisto_ng-0.7.11/src/ecallisto_ng/detection/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2024-02-08 11:52:29.000000 ecallisto_ng-0.7.11/src/ecallisto_ng/detection/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     8552 2024-02-08 11:52:29.000000 ecallisto_ng-0.7.11/src/ecallisto_ng/detection/flare_detection.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2024-02-28 16:22:18.507049 ecallisto_ng-0.7.11/src/ecallisto_ng/plotting/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-09-04 12:44:04.000000 ecallisto_ng-0.7.11/src/ecallisto_ng/plotting/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     9168 2024-02-28 15:52:50.000000 ecallisto_ng-0.7.11/src/ecallisto_ng/plotting/plotting.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3835 2023-11-24 11:03:08.000000 ecallisto_ng-0.7.11/src/ecallisto_ng/plotting/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2024-02-28 16:22:18.507049 ecallisto_ng-0.7.11/src/ecallisto_ng.egg-info/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     8973 2024-02-28 16:22:18.000000 ecallisto_ng-0.7.11/src/ecallisto_ng.egg-info/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1520 2024-02-28 16:22:18.000000 ecallisto_ng-0.7.11/src/ecallisto_ng.egg-info/SOURCES.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2024-02-28 16:22:18.000000 ecallisto_ng-0.7.11/src/ecallisto_ng.egg-info/dependency_links.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      268 2024-02-28 16:22:18.000000 ecallisto_ng-0.7.11/src/ecallisto_ng.egg-info/requires.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       29 2024-02-28 16:22:18.000000 ecallisto_ng-0.7.11/src/ecallisto_ng.egg-info/top_level.txt
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2024-02-28 16:22:18.507049 ecallisto_ng-0.7.11/src/models/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3084 2024-02-08 11:52:29.000000 ecallisto_ng-0.7.11/src/models/CustomCNN.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     4290 2024-02-08 11:52:29.000000 ecallisto_ng-0.7.11/src/models/DefaultModel.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1729 2024-02-08 11:52:29.000000 ecallisto_ng-0.7.11/src/models/EfficientNetV2SBinaryClassifier.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1129 2024-02-08 11:52:29.000000 ecallisto_ng-0.7.11/src/models/ResNet18BinaryClassifier.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1129 2024-02-08 11:52:29.000000 ecallisto_ng-0.7.11/src/models/ResNet50BinaryClassifier.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      997 2024-02-08 11:52:29.000000 ecallisto_ng-0.7.11/src/models/SqueezeNetBinaryClassifier.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1209 2024-02-08 11:52:29.000000 ecallisto_ng-0.7.11/src/models/ViTB16BinaryClassifier.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2024-02-08 11:52:29.000000 ecallisto_ng-0.7.11/src/models/__init__.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2024-02-28 16:22:18.507049 ecallisto_ng-0.7.11/tests/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      730 2023-12-20 11:46:31.000000 ecallisto_ng-0.7.11/tests/test_bg_subs.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      150 2023-12-20 12:06:28.000000 ecallisto_ng-0.7.11/tests/test_burstlist.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1855 2023-12-20 11:26:41.000000 ecallisto_ng-0.7.11/tests/test_data_download.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1386 2023-12-20 12:02:31.000000 ecallisto_ng-0.7.11/tests/test_plotting.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:06:13.762991 ecallisto_ng-0.7.12/
+-rw-rw-rw-   0        0        0     1104 2024-03-08 10:46:22.000000 ecallisto_ng-0.7.12/LICENSE
+-rw-rw-rw-   0        0        0       58 2024-03-08 10:46:22.000000 ecallisto_ng-0.7.12/MANIFEST.in
+-rw-rw-rw-   0        0        0     9715 2024-04-05 13:06:13.761009 ecallisto_ng-0.7.12/PKG-INFO
+-rw-rw-rw-   0        0        0     7577 2024-03-08 10:46:22.000000 ecallisto_ng-0.7.12/README.md
+-rw-rw-rw-   0        0        0     1328 2024-04-05 13:06:04.000000 ecallisto_ng-0.7.12/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 13:06:13.762991 ecallisto_ng-0.7.12/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 13:06:13.702261 ecallisto_ng-0.7.12/src/
+-rw-rw-rw-   0        0        0        0 2024-03-08 10:46:22.000000 ecallisto_ng-0.7.12/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:06:13.702261 ecallisto_ng-0.7.12/src/ecallisto_ng/
+-rw-rw-rw-   0        0        0        0 2024-03-08 10:46:22.000000 ecallisto_ng-0.7.12/src/ecallisto_ng/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:06:13.725476 ecallisto_ng-0.7.12/src/ecallisto_ng/burst_list/
+-rw-rw-rw-   0        0        0        0 2024-03-08 10:46:22.000000 ecallisto_ng-0.7.12/src/ecallisto_ng/burst_list/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:06:13.726475 ecallisto_ng-0.7.12/src/ecallisto_ng/burst_list/data/
+-rw-rw-rw-   0        0        0  1415009 2024-03-08 10:46:22.000000 ecallisto_ng-0.7.12/src/ecallisto_ng/burst_list/data/burst_list.xlsx
+-rw-rw-rw-   0        0        0     1432 2024-03-08 10:46:22.000000 ecallisto_ng-0.7.12/src/ecallisto_ng/burst_list/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:06:13.732476 ecallisto_ng-0.7.12/src/ecallisto_ng/combine_antennas/
+-rw-rw-rw-   0        0        0        0 2024-03-08 10:46:22.000000 ecallisto_ng-0.7.12/src/ecallisto_ng/combine_antennas/__init__.py
+-rw-rw-rw-   0        0        0     5555 2024-03-12 12:49:00.000000 ecallisto_ng-0.7.12/src/ecallisto_ng/combine_antennas/combine.py
+-rw-rw-rw-   0        0        0     9170 2024-03-08 10:46:22.000000 ecallisto_ng-0.7.12/src/ecallisto_ng/combine_antennas/utils.py
+-rw-rw-rw-   0        0        0     8849 2024-03-12 12:46:35.000000 ecallisto_ng-0.7.12/src/ecallisto_ng/combine_antennas/virtualantenna.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:06:13.735477 ecallisto_ng-0.7.12/src/ecallisto_ng/data_download/
+-rw-rw-rw-   0        0        0        0 2024-03-08 10:46:22.000000 ecallisto_ng-0.7.12/src/ecallisto_ng/data_download/__init__.py
+-rw-rw-rw-   0        0        0    14258 2024-03-08 18:12:21.000000 ecallisto_ng-0.7.12/src/ecallisto_ng/data_download/downloader.py
+-rw-rw-rw-   0        0        0    11450 2024-03-08 10:46:22.000000 ecallisto_ng-0.7.12/src/ecallisto_ng/data_download/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:06:13.739990 ecallisto_ng-0.7.12/src/ecallisto_ng/data_fetching/
+-rw-rw-rw-   0        0        0        0 2024-03-08 10:46:22.000000 ecallisto_ng-0.7.12/src/ecallisto_ng/data_fetching/__init__.py
+-rw-rw-rw-   0        0        0    10703 2024-03-08 18:12:21.000000 ecallisto_ng-0.7.12/src/ecallisto_ng/data_fetching/get_data.py
+-rw-rw-rw-   0        0        0     4833 2024-03-08 10:46:22.000000 ecallisto_ng-0.7.12/src/ecallisto_ng/data_fetching/get_information.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:06:13.742989 ecallisto_ng-0.7.12/src/ecallisto_ng/data_processing/
+-rw-rw-rw-   0        0        0        0 2024-03-08 10:46:22.000000 ecallisto_ng-0.7.12/src/ecallisto_ng/data_processing/__init__.py
+-rw-rw-rw-   0        0        0    10909 2024-03-08 18:12:02.000000 ecallisto_ng-0.7.12/src/ecallisto_ng/data_processing/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:06:13.744989 ecallisto_ng-0.7.12/src/ecallisto_ng/detection/
+-rw-rw-rw-   0        0        0        0 2024-03-08 10:46:22.000000 ecallisto_ng-0.7.12/src/ecallisto_ng/detection/__init__.py
+-rw-rw-rw-   0        0        0     8799 2024-03-08 18:12:21.000000 ecallisto_ng-0.7.12/src/ecallisto_ng/detection/flare_detection.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:06:13.746988 ecallisto_ng-0.7.12/src/ecallisto_ng/plotting/
+-rw-rw-rw-   0        0        0        0 2024-03-08 10:46:22.000000 ecallisto_ng-0.7.12/src/ecallisto_ng/plotting/__init__.py
+-rw-rw-rw-   0        0        0    10240 2024-03-19 10:57:40.000000 ecallisto_ng-0.7.12/src/ecallisto_ng/plotting/plotting.py
+-rw-rw-rw-   0        0        0     4720 2024-03-12 12:47:55.000000 ecallisto_ng-0.7.12/src/ecallisto_ng/plotting/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:06:13.758988 ecallisto_ng-0.7.12/src/ecallisto_ng.egg-info/
+-rw-rw-rw-   0        0        0     9715 2024-04-05 13:06:13.000000 ecallisto_ng-0.7.12/src/ecallisto_ng.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1520 2024-04-05 13:06:13.000000 ecallisto_ng-0.7.12/src/ecallisto_ng.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 13:06:13.000000 ecallisto_ng-0.7.12/src/ecallisto_ng.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      389 2024-04-05 13:06:13.000000 ecallisto_ng-0.7.12/src/ecallisto_ng.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-04-05 13:06:13.000000 ecallisto_ng-0.7.12/src/ecallisto_ng.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 13:06:13.753989 ecallisto_ng-0.7.12/src/models/
+-rw-rw-rw-   0        0        0     3179 2024-03-08 18:12:21.000000 ecallisto_ng-0.7.12/src/models/CustomCNN.py
+-rw-rw-rw-   0        0        0     4549 2024-03-08 18:12:21.000000 ecallisto_ng-0.7.12/src/models/DefaultModel.py
+-rw-rw-rw-   0        0        0     1820 2024-03-08 18:12:21.000000 ecallisto_ng-0.7.12/src/models/EfficientNetV2SBinaryClassifier.py
+-rw-rw-rw-   0        0        0     1163 2024-03-08 18:12:21.000000 ecallisto_ng-0.7.12/src/models/ResNet18BinaryClassifier.py
+-rw-rw-rw-   0        0        0     1163 2024-03-08 18:12:21.000000 ecallisto_ng-0.7.12/src/models/ResNet50BinaryClassifier.py
+-rw-rw-rw-   0        0        0     1038 2024-03-08 18:12:21.000000 ecallisto_ng-0.7.12/src/models/SqueezeNetBinaryClassifier.py
+-rw-rw-rw-   0        0        0     1284 2024-03-08 18:12:21.000000 ecallisto_ng-0.7.12/src/models/ViTB16BinaryClassifier.py
+-rw-rw-rw-   0        0        0        0 2024-03-08 10:46:22.000000 ecallisto_ng-0.7.12/src/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:06:13.756988 ecallisto_ng-0.7.12/tests/
+-rw-rw-rw-   0        0        0      748 2024-03-08 18:12:21.000000 ecallisto_ng-0.7.12/tests/test_bg_subs.py
+-rw-rw-rw-   0        0        0      156 2024-03-08 10:46:22.000000 ecallisto_ng-0.7.12/tests/test_burstlist.py
+-rw-rw-rw-   0        0        0     1907 2024-03-08 18:12:21.000000 ecallisto_ng-0.7.12/tests/test_data_download.py
+-rw-rw-rw-   0        0        0     1468 2024-03-08 18:12:21.000000 ecallisto_ng-0.7.12/tests/test_plotting.py
```

### Comparing `ecallisto_ng-0.7.11/LICENSE` & `ecallisto_ng-0.7.12/LICENSE`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Institute for Data Science
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Institute for Data Science
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `ecallisto_ng-0.7.11/PKG-INFO` & `ecallisto_ng-0.7.12/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,191 +1,205 @@
-Metadata-Version: 2.1
-Name: ecallisto_ng
-Version: 0.7.11
-Summary: A Python package for the fetching (and some processing and plotting) of eCallisto data based on request and pandas.
-Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
-Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
-Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy>=1.21.6
-Requires-Dist: pandas>=2.0.0
-Requires-Dist: openpyxl
-Requires-Dist: plotly
-Requires-Dist: kaleido
-Requires-Dist: matplotlib
-Requires-Dist: requests
-Requires-Dist: scikit-image>=0.20.0
-Requires-Dist: pyarrow
-Requires-Dist: bs4
-Requires-Dist: lxml
-Requires-Dist: astropy
-Requires-Dist: tqdm
-Provides-Extra: nb
-Requires-Dist: nbformat; extra == "nb"
-Requires-Dist: ipython; extra == "nb"
-Requires-Dist: ipykernel; extra == "nb"
-Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-Requires-Dist: build; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Provides-Extra: ml
-Requires-Dist: mlflow; extra == "ml"
-Requires-Dist: torch; extra == "ml"
-Requires-Dist: torchvision; extra == "ml"
-Requires-Dist: torchmetrics; extra == "ml"
-Requires-Dist: pytorch-lightning; extra == "ml"
-Provides-Extra: va
-Requires-Dist: torch; extra == "va"
-
-# Ecallisto NG 
-Ecallisto NG is a comprehensive Python package tailored for interacting with Ecallisto data. It focuses on facilitating efficient data manipulation, processing, and visualization, leveraging the power of Pandas for data handling and PyTorch for advanced computations. The package is particularly optimized for dealing with large datasets, providing tools for slicing, filtering, and resampling data to make spectogram plotting more manageable.
-
-## Table of Contents
-- [Background](#background)
-- [Installation](#installation)
-  - [PyPI](#pypi)
-  - [Dev Installation](#dev-installation)
-  - [Virtual Antenna Creation](#creation-of-the-virtual-antenna)
-- [Using Pandas with Ecallisto NG](#pandas)
-- [Examples and Usage](#examples-and-usage)
-  - [Data Fetching](#data-fetching-deprecated)
-  - [Data Processing and Visualization](#data-processing-and-visualization)
-  - [Plotting](#plotting)
-  - [Spectogram Editing](#spectogram-editing)
-- [Additional Information](#additional-information)
-  - [Note on .attrs and FITS Header](#note-on-attrs-and-fits-header)
-  - [Contributing](#contributing)
-
-## Background
-he package is built with Python 3.9 and primarily uses the Pandas library for data manipulation. While it initially offered a direct interaction with the Ecallisto Rest API (now deprecated), its current functionality is centered around efficient data processing and visualization. The data provided by e-Callisto is stored in a pandas Dataframe, where the index is the time and the column names are the observed frequencies.
-
-### Note: The REST API is now deprecated. However, you can still access it via https://v000792.fhnw.ch/api/redoc for a while. This was done because with help of pandas and multiprocessing, the download of the data is much faster and more efficient when directly accessing the files.
-
-## PyPI
-Available on PyPI: https://pypi.org/project/ecallisto-ng/
-
-## Installation
-To install this package, use pip for installation. Execute the following command in your terminal with basic functionality, such as plotting and data fetching:
-```pip install ecallisto-ng```
-If you want to use the virtual antenna:
-```pip install ecallisto-ng[va]```
-If you want to use the detection of flares, powered by ML:
-```pip install ecallisto-ng[ml]```
-
-To use the notebook, please install the notebook dependencies.
-
-## Dev Installation
-Of course, you can also install the package from source. To do so, clone the repository and install the package in editable mode:
-```pip install -e .```
-```pip install -e .[va]```
-```pip install -e .[ml]```
-
-## Pandas
-Pandas is an open-source data analysis and manipulation tool, pivotal to Ecallisto NG. Learning Pandas is essential for effectively using Ecallisto NG, as it allows for sophisticated data slicing, filtering, and aggregation. More on Pandas: https://pandas.pydata.org/docs/
-
-## Examples and Usage
-Please have a look at the jupyter notebook under `example`.
-
-# Getting data
-## `get_ecallisto_data` Function
-
-This function fetches e-Callisto data within a specified date range and optional instrument regex pattern. It's suitable for smaller datasets. For larger datasets, consider using the `get_ecallisto_data_generator` function.
-
-## Parameters
-- `start_datetime` (datetime-like): The start date for the file search.
-- `end_datetime` (datetime-like): The end date for the file search.
-- `instrument_string` (str, List[str] or None): Instrument name(s) for file URL matching. If `None`, all files are considered.
-- `freq_start` (float or None): The start frequency for filtering.
-- `freq_end` (float or None): The end frequency for filtering.
-- `base_url` (str): Base URL of the remote file directory.
-
-## Returns
-- (dict of str: pandas.DataFrame) or pandas.DataFrame: A dictionary of instrument names and their corresponding dataframes. If only one instrument is found, it returns a single dataframe.
-
-## Example
-```python
-from ecallisto_ng.data_fetching import get_ecallisto_data
-from datetime import datetime
-
-start = datetime(2021, 3, 1, 6, 30, 0)
-end = datetime(2021, 3, 7, 23, 30, 0)
-instrument_name = "austria_unigraz_01"
-
-df = get_ecallisto_data(start, end, instrument_name)
-```
-# Getting data via a generator
-## `get_ecallisto_data_generator` Function
-
-A generator function that yields e-Callisto data one file at a time within a date range. It's ideal for handling large datasets or when working with limited memory.
-
-## Parameters
-- `start_datetime` (datetime-like): The start date for the file search.
-- `end_datetime` (datetime-like): The end date for the file search.
-- `instrument_name` (List[str], str, or None): Instrument name(s) for file URL matching. If `None`, all files are considered.
-- `freq_start` (float or None): The start frequency for filtering.
-- `freq_end` (float or None): The end frequency for filtering.
-- `base_url` (str): Base URL of the remote file directory.
-
-## Yields
-- (str, pandas.DataFrame): A tuple containing the instrument name and its corresponding DataFrame.
-
-## Example
-```python
-from ecallisto_ng.data_fetching import get_ecallisto_data_generator
-from datetime import datetime
-
-start = datetime(2021, 3, 1, 6, 30, 0)
-end = datetime(2021, 3, 7, 23, 30, 0)
-instrument_name = ["austria_unigraz_01", "another_instrument"]
-
-data_generator = get_ecallisto_data_generator(start, end, instrument_name)
-for instrument_name, data_frame in data_generator:
-    process_data(instrument_name, data_frame)  # Replace with your processing function
-
-```
-## Plotting 
-Ecallisto NG provides basic plotting capabilities. Here's an example of how to generate a spectogram:
-```python
-from ecallisto_ng.plotting.utils import plot_spectogram
-
-plot_spectogram(df)
-```
-Make use of .resample to reduce the size of the data. Alternatively, you can pass a `resolution` parameter to the plot_spectogram. Here's an example:
-```python
-plot_spectogram(df.resample("1min").max())
-plot_spectogram(df, resolution="1min")
-```
-For more documentation on resample, please refer to the [Pandas documentation](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.resample.html).
-## Spectogram editing
-We also provide some basic functionalities to edit the spectogram. Here's how you can do it:
-```python
-from ecallisto_ng.data_processing.utils import elimwrongchannels, subtract_constant_background, subtract_rolling_background
-
-df = elimwrongchannels(df)
-df = fill_missing_timesteps_with_nan(df)
-df = subtract_constant_background(df)
-df = subtract_rolling_background(df)
-
-# Filter keep frequencies only between 40 and 70 MHz
-df = df.loc[:, 40:70]
-
-plot_spectogram(df)
-```
-## Additional Information
-### Note on .attrs and FITS Header
-The function utilizes DataFrames with the .attrs attribute to store FITS header information. This attribute is a dictionary-like object and contains metadata about the FITS file, including header details. Accessing .attrs is essential for understanding the context of the data:
-
-```python
-print(df.attrs)
-```
-
-These simple commands allow you to easily manipulate spectogram data, enabling effective use of the Ecallisto API for your needs.
-
-### Contributing
-Contributions to Ecallisto NG are very welcome! If you have an idea for an improvement or have found a bug, please feel free to contribute. The preferred way to contribute is by submitting a Pull Request (PR) or creating an issue on our GitHub repository. This way, we can discuss potential changes or fixes and maintain the quality of the project.
+Metadata-Version: 2.1
+Name: ecallisto_ng
+Version: 0.7.12
+Summary: A Python package for the fetching (and some processing and plotting) of eCallisto data based on request and pandas.
+Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
+Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
+Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy>=1.21.6
+Requires-Dist: pandas>=2.0.0
+Requires-Dist: openpyxl
+Requires-Dist: plotly
+Requires-Dist: kaleido
+Requires-Dist: matplotlib
+Requires-Dist: requests
+Requires-Dist: scikit-image>=0.20.0
+Requires-Dist: pyarrow
+Requires-Dist: bs4
+Requires-Dist: lxml
+Requires-Dist: astropy
+Requires-Dist: tqdm
+Provides-Extra: nb
+Requires-Dist: nbformat; extra == "nb"
+Requires-Dist: ipython; extra == "nb"
+Requires-Dist: ipykernel; extra == "nb"
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Provides-Extra: ml
+Requires-Dist: mlflow; extra == "ml"
+Requires-Dist: torch; extra == "ml"
+Requires-Dist: torchvision; extra == "ml"
+Requires-Dist: torchmetrics; extra == "ml"
+Requires-Dist: pytorch-lightning; extra == "ml"
+Provides-Extra: va
+Requires-Dist: torch; extra == "va"
+Provides-Extra: all
+Requires-Dist: nbformat; extra == "all"
+Requires-Dist: ipython; extra == "all"
+Requires-Dist: ipykernel; extra == "all"
+Requires-Dist: black; extra == "all"
+Requires-Dist: isort; extra == "all"
+Requires-Dist: twine; extra == "all"
+Requires-Dist: build; extra == "all"
+Requires-Dist: pytest; extra == "all"
+Requires-Dist: mlflow; extra == "all"
+Requires-Dist: torch; extra == "all"
+Requires-Dist: torchvision; extra == "all"
+Requires-Dist: torchmetrics; extra == "all"
+Requires-Dist: pytorch-lightning; extra == "all"
+
+# Ecallisto NG 
+Ecallisto NG is a comprehensive Python package tailored for interacting with Ecallisto data. It focuses on facilitating efficient data manipulation, processing, and visualization, leveraging the power of Pandas for data handling and PyTorch for advanced computations. The package is particularly optimized for dealing with large datasets, providing tools for slicing, filtering, and resampling data to make spectogram plotting more manageable.
+
+## Table of Contents
+- [Background](#background)
+- [Installation](#installation)
+  - [PyPI](#pypi)
+  - [Dev Installation](#dev-installation)
+  - [Virtual Antenna Creation](#creation-of-the-virtual-antenna)
+- [Using Pandas with Ecallisto NG](#pandas)
+- [Examples and Usage](#examples-and-usage)
+  - [Data Fetching](#data-fetching-deprecated)
+  - [Data Processing and Visualization](#data-processing-and-visualization)
+  - [Plotting](#plotting)
+  - [Spectogram Editing](#spectogram-editing)
+- [Additional Information](#additional-information)
+  - [Note on .attrs and FITS Header](#note-on-attrs-and-fits-header)
+  - [Contributing](#contributing)
+
+## Background
+he package is built with Python 3.9 and primarily uses the Pandas library for data manipulation. While it initially offered a direct interaction with the Ecallisto Rest API (now deprecated), its current functionality is centered around efficient data processing and visualization. The data provided by e-Callisto is stored in a pandas Dataframe, where the index is the time and the column names are the observed frequencies.
+
+### Note: The REST API is now deprecated. However, you can still access it via https://v000792.fhnw.ch/api/redoc for a while. This was done because with help of pandas and multiprocessing, the download of the data is much faster and more efficient when directly accessing the files.
+
+## PyPI
+Available on PyPI: https://pypi.org/project/ecallisto-ng/
+
+## Installation
+To install this package, use pip for installation. Execute the following command in your terminal with basic functionality, such as plotting and data fetching:
+```pip install ecallisto-ng```
+If you want to use the virtual antenna:
+```pip install ecallisto-ng[va]```
+If you want to use the detection of flares, powered by ML:
+```pip install ecallisto-ng[ml]```
+
+To use the notebook, please install the notebook dependencies.
+
+## Dev Installation
+Of course, you can also install the package from source. To do so, clone the repository and install the package in editable mode:
+```pip install -e .```
+```pip install -e .[va]```
+```pip install -e .[ml]```
+
+## Pandas
+Pandas is an open-source data analysis and manipulation tool, pivotal to Ecallisto NG. Learning Pandas is essential for effectively using Ecallisto NG, as it allows for sophisticated data slicing, filtering, and aggregation. More on Pandas: https://pandas.pydata.org/docs/
+
+## Examples and Usage
+Please have a look at the jupyter notebook under `example`.
+
+# Getting data
+## `get_ecallisto_data` Function
+
+This function fetches e-Callisto data within a specified date range and optional instrument regex pattern. It's suitable for smaller datasets. For larger datasets, consider using the `get_ecallisto_data_generator` function.
+
+## Parameters
+- `start_datetime` (datetime-like): The start date for the file search.
+- `end_datetime` (datetime-like): The end date for the file search.
+- `instrument_string` (str, List[str] or None): Instrument name(s) for file URL matching. If `None`, all files are considered.
+- `freq_start` (float or None): The start frequency for filtering.
+- `freq_end` (float or None): The end frequency for filtering.
+- `base_url` (str): Base URL of the remote file directory.
+
+## Returns
+- (dict of str: pandas.DataFrame) or pandas.DataFrame: A dictionary of instrument names and their corresponding dataframes. If only one instrument is found, it returns a single dataframe.
+
+## Example
+```python
+from ecallisto_ng.data_fetching import get_ecallisto_data
+from datetime import datetime
+
+start = datetime(2021, 3, 1, 6, 30, 0)
+end = datetime(2021, 3, 7, 23, 30, 0)
+instrument_name = "austria_unigraz_01"
+
+df = get_ecallisto_data(start, end, instrument_name)
+```
+# Getting data via a generator
+## `get_ecallisto_data_generator` Function
+
+A generator function that yields e-Callisto data one file at a time within a date range. It's ideal for handling large datasets or when working with limited memory.
+
+## Parameters
+- `start_datetime` (datetime-like): The start date for the file search.
+- `end_datetime` (datetime-like): The end date for the file search.
+- `instrument_name` (List[str], str, or None): Instrument name(s) for file URL matching. If `None`, all files are considered.
+- `freq_start` (float or None): The start frequency for filtering.
+- `freq_end` (float or None): The end frequency for filtering.
+- `base_url` (str): Base URL of the remote file directory.
+
+## Yields
+- (str, pandas.DataFrame): A tuple containing the instrument name and its corresponding DataFrame.
+
+## Example
+```python
+from ecallisto_ng.data_fetching import get_ecallisto_data_generator
+from datetime import datetime
+
+start = datetime(2021, 3, 1, 6, 30, 0)
+end = datetime(2021, 3, 7, 23, 30, 0)
+instrument_name = ["austria_unigraz_01", "another_instrument"]
+
+data_generator = get_ecallisto_data_generator(start, end, instrument_name)
+for instrument_name, data_frame in data_generator:
+    process_data(instrument_name, data_frame)  # Replace with your processing function
+
+```
+## Plotting 
+Ecallisto NG provides basic plotting capabilities. Here's an example of how to generate a spectogram:
+```python
+from ecallisto_ng.plotting.utils import plot_spectogram
+
+plot_spectogram(df)
+```
+Make use of .resample to reduce the size of the data. Alternatively, you can pass a `resolution` parameter to the plot_spectogram. Here's an example:
+```python
+plot_spectogram(df.resample("1min").max())
+plot_spectogram(df, resolution="1min")
+```
+For more documentation on resample, please refer to the [Pandas documentation](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.resample.html).
+## Spectogram editing
+We also provide some basic functionalities to edit the spectogram. Here's how you can do it:
+```python
+from ecallisto_ng.data_processing.utils import elimwrongchannels, subtract_constant_background, subtract_rolling_background
+
+df = elimwrongchannels(df)
+df = fill_missing_timesteps_with_nan(df)
+df = subtract_constant_background(df)
+df = subtract_rolling_background(df)
+
+# Filter keep frequencies only between 40 and 70 MHz
+df = df.loc[:, 40:70]
+
+plot_spectogram(df)
+```
+## Additional Information
+### Note on .attrs and FITS Header
+The function utilizes DataFrames with the .attrs attribute to store FITS header information. This attribute is a dictionary-like object and contains metadata about the FITS file, including header details. Accessing .attrs is essential for understanding the context of the data:
+
+```python
+print(df.attrs)
+```
+
+These simple commands allow you to easily manipulate spectogram data, enabling effective use of the Ecallisto API for your needs.
+
+### Contributing
+Contributions to Ecallisto NG are very welcome! If you have an idea for an improvement or have found a bug, please feel free to contribute. The preferred way to contribute is by submitting a Pull Request (PR) or creating an issue on our GitHub repository. This way, we can discuss potential changes or fixes and maintain the quality of the project.
```

### Comparing `ecallisto_ng-0.7.11/README.md` & `ecallisto_ng-0.7.12/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-# Ecallisto NG 
-Ecallisto NG is a comprehensive Python package tailored for interacting with Ecallisto data. It focuses on facilitating efficient data manipulation, processing, and visualization, leveraging the power of Pandas for data handling and PyTorch for advanced computations. The package is particularly optimized for dealing with large datasets, providing tools for slicing, filtering, and resampling data to make spectogram plotting more manageable.
-
-## Table of Contents
-- [Background](#background)
-- [Installation](#installation)
-  - [PyPI](#pypi)
-  - [Dev Installation](#dev-installation)
-  - [Virtual Antenna Creation](#creation-of-the-virtual-antenna)
-- [Using Pandas with Ecallisto NG](#pandas)
-- [Examples and Usage](#examples-and-usage)
-  - [Data Fetching](#data-fetching-deprecated)
-  - [Data Processing and Visualization](#data-processing-and-visualization)
-  - [Plotting](#plotting)
-  - [Spectogram Editing](#spectogram-editing)
-- [Additional Information](#additional-information)
-  - [Note on .attrs and FITS Header](#note-on-attrs-and-fits-header)
-  - [Contributing](#contributing)
-
-## Background
-he package is built with Python 3.9 and primarily uses the Pandas library for data manipulation. While it initially offered a direct interaction with the Ecallisto Rest API (now deprecated), its current functionality is centered around efficient data processing and visualization. The data provided by e-Callisto is stored in a pandas Dataframe, where the index is the time and the column names are the observed frequencies.
-
-### Note: The REST API is now deprecated. However, you can still access it via https://v000792.fhnw.ch/api/redoc for a while. This was done because with help of pandas and multiprocessing, the download of the data is much faster and more efficient when directly accessing the files.
-
-## PyPI
-Available on PyPI: https://pypi.org/project/ecallisto-ng/
-
-## Installation
-To install this package, use pip for installation. Execute the following command in your terminal with basic functionality, such as plotting and data fetching:
-```pip install ecallisto-ng```
-If you want to use the virtual antenna:
-```pip install ecallisto-ng[va]```
-If you want to use the detection of flares, powered by ML:
-```pip install ecallisto-ng[ml]```
-
-To use the notebook, please install the notebook dependencies.
-
-## Dev Installation
-Of course, you can also install the package from source. To do so, clone the repository and install the package in editable mode:
-```pip install -e .```
-```pip install -e .[va]```
-```pip install -e .[ml]```
-
-## Pandas
-Pandas is an open-source data analysis and manipulation tool, pivotal to Ecallisto NG. Learning Pandas is essential for effectively using Ecallisto NG, as it allows for sophisticated data slicing, filtering, and aggregation. More on Pandas: https://pandas.pydata.org/docs/
-
-## Examples and Usage
-Please have a look at the jupyter notebook under `example`.
-
-# Getting data
-## `get_ecallisto_data` Function
-
-This function fetches e-Callisto data within a specified date range and optional instrument regex pattern. It's suitable for smaller datasets. For larger datasets, consider using the `get_ecallisto_data_generator` function.
-
-## Parameters
-- `start_datetime` (datetime-like): The start date for the file search.
-- `end_datetime` (datetime-like): The end date for the file search.
-- `instrument_string` (str, List[str] or None): Instrument name(s) for file URL matching. If `None`, all files are considered.
-- `freq_start` (float or None): The start frequency for filtering.
-- `freq_end` (float or None): The end frequency for filtering.
-- `base_url` (str): Base URL of the remote file directory.
-
-## Returns
-- (dict of str: pandas.DataFrame) or pandas.DataFrame: A dictionary of instrument names and their corresponding dataframes. If only one instrument is found, it returns a single dataframe.
-
-## Example
-```python
-from ecallisto_ng.data_fetching import get_ecallisto_data
-from datetime import datetime
-
-start = datetime(2021, 3, 1, 6, 30, 0)
-end = datetime(2021, 3, 7, 23, 30, 0)
-instrument_name = "austria_unigraz_01"
-
-df = get_ecallisto_data(start, end, instrument_name)
-```
-# Getting data via a generator
-## `get_ecallisto_data_generator` Function
-
-A generator function that yields e-Callisto data one file at a time within a date range. It's ideal for handling large datasets or when working with limited memory.
-
-## Parameters
-- `start_datetime` (datetime-like): The start date for the file search.
-- `end_datetime` (datetime-like): The end date for the file search.
-- `instrument_name` (List[str], str, or None): Instrument name(s) for file URL matching. If `None`, all files are considered.
-- `freq_start` (float or None): The start frequency for filtering.
-- `freq_end` (float or None): The end frequency for filtering.
-- `base_url` (str): Base URL of the remote file directory.
-
-## Yields
-- (str, pandas.DataFrame): A tuple containing the instrument name and its corresponding DataFrame.
-
-## Example
-```python
-from ecallisto_ng.data_fetching import get_ecallisto_data_generator
-from datetime import datetime
-
-start = datetime(2021, 3, 1, 6, 30, 0)
-end = datetime(2021, 3, 7, 23, 30, 0)
-instrument_name = ["austria_unigraz_01", "another_instrument"]
-
-data_generator = get_ecallisto_data_generator(start, end, instrument_name)
-for instrument_name, data_frame in data_generator:
-    process_data(instrument_name, data_frame)  # Replace with your processing function
-
-```
-## Plotting 
-Ecallisto NG provides basic plotting capabilities. Here's an example of how to generate a spectogram:
-```python
-from ecallisto_ng.plotting.utils import plot_spectogram
-
-plot_spectogram(df)
-```
-Make use of .resample to reduce the size of the data. Alternatively, you can pass a `resolution` parameter to the plot_spectogram. Here's an example:
-```python
-plot_spectogram(df.resample("1min").max())
-plot_spectogram(df, resolution="1min")
-```
-For more documentation on resample, please refer to the [Pandas documentation](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.resample.html).
-## Spectogram editing
-We also provide some basic functionalities to edit the spectogram. Here's how you can do it:
-```python
-from ecallisto_ng.data_processing.utils import elimwrongchannels, subtract_constant_background, subtract_rolling_background
-
-df = elimwrongchannels(df)
-df = fill_missing_timesteps_with_nan(df)
-df = subtract_constant_background(df)
-df = subtract_rolling_background(df)
-
-# Filter keep frequencies only between 40 and 70 MHz
-df = df.loc[:, 40:70]
-
-plot_spectogram(df)
-```
-## Additional Information
-### Note on .attrs and FITS Header
-The function utilizes DataFrames with the .attrs attribute to store FITS header information. This attribute is a dictionary-like object and contains metadata about the FITS file, including header details. Accessing .attrs is essential for understanding the context of the data:
-
-```python
-print(df.attrs)
-```
-
-These simple commands allow you to easily manipulate spectogram data, enabling effective use of the Ecallisto API for your needs.
-
-### Contributing
+# Ecallisto NG 
+Ecallisto NG is a comprehensive Python package tailored for interacting with Ecallisto data. It focuses on facilitating efficient data manipulation, processing, and visualization, leveraging the power of Pandas for data handling and PyTorch for advanced computations. The package is particularly optimized for dealing with large datasets, providing tools for slicing, filtering, and resampling data to make spectogram plotting more manageable.
+
+## Table of Contents
+- [Background](#background)
+- [Installation](#installation)
+  - [PyPI](#pypi)
+  - [Dev Installation](#dev-installation)
+  - [Virtual Antenna Creation](#creation-of-the-virtual-antenna)
+- [Using Pandas with Ecallisto NG](#pandas)
+- [Examples and Usage](#examples-and-usage)
+  - [Data Fetching](#data-fetching-deprecated)
+  - [Data Processing and Visualization](#data-processing-and-visualization)
+  - [Plotting](#plotting)
+  - [Spectogram Editing](#spectogram-editing)
+- [Additional Information](#additional-information)
+  - [Note on .attrs and FITS Header](#note-on-attrs-and-fits-header)
+  - [Contributing](#contributing)
+
+## Background
+he package is built with Python 3.9 and primarily uses the Pandas library for data manipulation. While it initially offered a direct interaction with the Ecallisto Rest API (now deprecated), its current functionality is centered around efficient data processing and visualization. The data provided by e-Callisto is stored in a pandas Dataframe, where the index is the time and the column names are the observed frequencies.
+
+### Note: The REST API is now deprecated. However, you can still access it via https://v000792.fhnw.ch/api/redoc for a while. This was done because with help of pandas and multiprocessing, the download of the data is much faster and more efficient when directly accessing the files.
+
+## PyPI
+Available on PyPI: https://pypi.org/project/ecallisto-ng/
+
+## Installation
+To install this package, use pip for installation. Execute the following command in your terminal with basic functionality, such as plotting and data fetching:
+```pip install ecallisto-ng```
+If you want to use the virtual antenna:
+```pip install ecallisto-ng[va]```
+If you want to use the detection of flares, powered by ML:
+```pip install ecallisto-ng[ml]```
+
+To use the notebook, please install the notebook dependencies.
+
+## Dev Installation
+Of course, you can also install the package from source. To do so, clone the repository and install the package in editable mode:
+```pip install -e .```
+```pip install -e .[va]```
+```pip install -e .[ml]```
+
+## Pandas
+Pandas is an open-source data analysis and manipulation tool, pivotal to Ecallisto NG. Learning Pandas is essential for effectively using Ecallisto NG, as it allows for sophisticated data slicing, filtering, and aggregation. More on Pandas: https://pandas.pydata.org/docs/
+
+## Examples and Usage
+Please have a look at the jupyter notebook under `example`.
+
+# Getting data
+## `get_ecallisto_data` Function
+
+This function fetches e-Callisto data within a specified date range and optional instrument regex pattern. It's suitable for smaller datasets. For larger datasets, consider using the `get_ecallisto_data_generator` function.
+
+## Parameters
+- `start_datetime` (datetime-like): The start date for the file search.
+- `end_datetime` (datetime-like): The end date for the file search.
+- `instrument_string` (str, List[str] or None): Instrument name(s) for file URL matching. If `None`, all files are considered.
+- `freq_start` (float or None): The start frequency for filtering.
+- `freq_end` (float or None): The end frequency for filtering.
+- `base_url` (str): Base URL of the remote file directory.
+
+## Returns
+- (dict of str: pandas.DataFrame) or pandas.DataFrame: A dictionary of instrument names and their corresponding dataframes. If only one instrument is found, it returns a single dataframe.
+
+## Example
+```python
+from ecallisto_ng.data_fetching import get_ecallisto_data
+from datetime import datetime
+
+start = datetime(2021, 3, 1, 6, 30, 0)
+end = datetime(2021, 3, 7, 23, 30, 0)
+instrument_name = "austria_unigraz_01"
+
+df = get_ecallisto_data(start, end, instrument_name)
+```
+# Getting data via a generator
+## `get_ecallisto_data_generator` Function
+
+A generator function that yields e-Callisto data one file at a time within a date range. It's ideal for handling large datasets or when working with limited memory.
+
+## Parameters
+- `start_datetime` (datetime-like): The start date for the file search.
+- `end_datetime` (datetime-like): The end date for the file search.
+- `instrument_name` (List[str], str, or None): Instrument name(s) for file URL matching. If `None`, all files are considered.
+- `freq_start` (float or None): The start frequency for filtering.
+- `freq_end` (float or None): The end frequency for filtering.
+- `base_url` (str): Base URL of the remote file directory.
+
+## Yields
+- (str, pandas.DataFrame): A tuple containing the instrument name and its corresponding DataFrame.
+
+## Example
+```python
+from ecallisto_ng.data_fetching import get_ecallisto_data_generator
+from datetime import datetime
+
+start = datetime(2021, 3, 1, 6, 30, 0)
+end = datetime(2021, 3, 7, 23, 30, 0)
+instrument_name = ["austria_unigraz_01", "another_instrument"]
+
+data_generator = get_ecallisto_data_generator(start, end, instrument_name)
+for instrument_name, data_frame in data_generator:
+    process_data(instrument_name, data_frame)  # Replace with your processing function
+
+```
+## Plotting 
+Ecallisto NG provides basic plotting capabilities. Here's an example of how to generate a spectogram:
+```python
+from ecallisto_ng.plotting.utils import plot_spectogram
+
+plot_spectogram(df)
+```
+Make use of .resample to reduce the size of the data. Alternatively, you can pass a `resolution` parameter to the plot_spectogram. Here's an example:
+```python
+plot_spectogram(df.resample("1min").max())
+plot_spectogram(df, resolution="1min")
+```
+For more documentation on resample, please refer to the [Pandas documentation](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.resample.html).
+## Spectogram editing
+We also provide some basic functionalities to edit the spectogram. Here's how you can do it:
+```python
+from ecallisto_ng.data_processing.utils import elimwrongchannels, subtract_constant_background, subtract_rolling_background
+
+df = elimwrongchannels(df)
+df = fill_missing_timesteps_with_nan(df)
+df = subtract_constant_background(df)
+df = subtract_rolling_background(df)
+
+# Filter keep frequencies only between 40 and 70 MHz
+df = df.loc[:, 40:70]
+
+plot_spectogram(df)
+```
+## Additional Information
+### Note on .attrs and FITS Header
+The function utilizes DataFrames with the .attrs attribute to store FITS header information. This attribute is a dictionary-like object and contains metadata about the FITS file, including header details. Accessing .attrs is essential for understanding the context of the data:
+
+```python
+print(df.attrs)
+```
+
+These simple commands allow you to easily manipulate spectogram data, enabling effective use of the Ecallisto API for your needs.
+
+### Contributing
 Contributions to Ecallisto NG are very welcome! If you have an idea for an improvement or have found a bug, please feel free to contribute. The preferred way to contribute is by submitting a Pull Request (PR) or creating an issue on our GitHub repository. This way, we can discuss potential changes or fixes and maintain the quality of the project.
```

### Comparing `ecallisto_ng-0.7.11/pyproject.toml` & `ecallisto_ng-0.7.12/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,43 @@
-[project]
-name = "ecallisto_ng"
-version = "0.7.11"
-authors = [{name = "Vincenzo Timmel", email = "vincenzo.timmel@fhnw.ch"}]
-description = "A Python package for the fetching (and some processing and plotting) of eCallisto data based on request and pandas."
-readme = "README.md"
-
-requires-python = ">=3.9"
-
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-dependencies = [
-    'numpy>=1.21.6',
-    'pandas>=2.0.0',
-    'openpyxl',
-    'plotly',
-    'kaleido',
-    'matplotlib',
-    'requests',
-    'scikit-image>=0.20.0',
-    'pyarrow',
-    'bs4',
-    'lxml',
-    'astropy',
-    'tqdm'
-]
-[project.optional-dependencies]
-nb = ['nbformat', 'ipython', 'ipykernel']
-dev = ['black', 'isort', 'twine', 'build', 'pytest']
-ml = ['mlflow', 'torch', 'torchvision', 'torchmetrics', 'pytorch-lightning']
-va = ['torch']
-
-[build-system]
-requires = ["setuptools", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[project.urls]
-Homepage = "https://github.com/i4Ds/ecallisto_ng"
-"Bug Tracker" = "https://github.com/i4Ds/ecallisto_ng/issues"
+[project]
+name = "ecallisto_ng"
+version = "0.7.12"
+authors = [{name = "Vincenzo Timmel", email = "vincenzo.timmel@fhnw.ch"}]
+description = "A Python package for the fetching (and some processing and plotting) of eCallisto data based on request and pandas."
+readme = "README.md"
+
+requires-python = ">=3.9"
+
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+dependencies = [
+    'numpy>=1.21.6',
+    'pandas>=2.0.0',
+    'openpyxl',
+    'plotly',
+    'kaleido',
+    'matplotlib',
+    'requests',
+    'scikit-image>=0.20.0',
+    'pyarrow',
+    'bs4',
+    'lxml',
+    'astropy',
+    'tqdm'
+]
+[project.optional-dependencies]
+nb = ['nbformat', 'ipython', 'ipykernel']
+dev = ['black', 'isort', 'twine', 'build', 'pytest']
+ml = ['mlflow', 'torch', 'torchvision', 'torchmetrics', 'pytorch-lightning']
+va = ['torch']
+all = ['nbformat', 'ipython', 'ipykernel', 'black', 'isort', 'twine', 'build', 'pytest', 'mlflow', 'torch', 'torchvision', 'torchmetrics', 'pytorch-lightning']
+
+[build-system]
+requires = ["setuptools", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[project.urls]
+Homepage = "https://github.com/i4Ds/ecallisto_ng"
+"Bug Tracker" = "https://github.com/i4Ds/ecallisto_ng/issues"
```

### Comparing `ecallisto_ng-0.7.11/src/ecallisto_ng/burst_list/data/burst_list.xlsx` & `ecallisto_ng-0.7.12/src/ecallisto_ng/burst_list/data/burst_list.xlsx`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.7.11/src/ecallisto_ng/burst_list/utils.py` & `ecallisto_ng-0.7.12/src/ecallisto_ng/burst_list/utils.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-import os
-
-import pandas as pd
-
-
-def load_burst_list(burst_list_file=None):
-    """
-    Load a burst list from a specified Excel file into a pandas DataFrame.
-
-    This function reads an Excel file containing information about bursts and
-    loads it into a pandas DataFrame. If no file path is provided, it defaults to
-    'burst_list.xlsx' located in a 'data' folder in the same directory as this script.
-
-    Parameters
-    ----------
-    burst_list_file : str, optional
-        Path to the Excel file containing the burst list. If not provided, defaults to
-        'burst_list.xlsx' in the 'data' subdirectory of the script's directory.
-
-    Returns
-    -------
-    pandas.DataFrame
-        A DataFrame containing the burst list data.
-
-    Examples
-    --------
-    Load a burst list from the default location:
-
-    >>> burst_list = load_burst_list()
-
-    Load a burst list from a specific file:
-
-    >>> burst_list = load_burst_list("path/to/burst_list.xlsx")
-    """
-    if burst_list_file is None:
-        burst_list_file = os.path.join(
-            os.path.dirname(__file__), "data", "burst_list.xlsx"
-        )
-    if burst_list_file.endswith(".csv"):
-        burst_list = pd.read_csv(burst_list_file)
-    elif burst_list_file.endswith(".xlsx"):
-        burst_list = pd.read_excel(burst_list_file)
-    else:
-        raise ValueError("Unknown file format")
-    return burst_list
+import os
+
+import pandas as pd
+
+
+def load_burst_list(burst_list_file=None):
+    """
+    Load a burst list from a specified Excel file into a pandas DataFrame.
+
+    This function reads an Excel file containing information about bursts and
+    loads it into a pandas DataFrame. If no file path is provided, it defaults to
+    'burst_list.xlsx' located in a 'data' folder in the same directory as this script.
+
+    Parameters
+    ----------
+    burst_list_file : str, optional
+        Path to the Excel file containing the burst list. If not provided, defaults to
+        'burst_list.xlsx' in the 'data' subdirectory of the script's directory.
+
+    Returns
+    -------
+    pandas.DataFrame
+        A DataFrame containing the burst list data.
+
+    Examples
+    --------
+    Load a burst list from the default location:
+
+    >>> burst_list = load_burst_list()
+
+    Load a burst list from a specific file:
+
+    >>> burst_list = load_burst_list("path/to/burst_list.xlsx")
+    """
+    if burst_list_file is None:
+        burst_list_file = os.path.join(
+            os.path.dirname(__file__), "data", "burst_list.xlsx"
+        )
+    if burst_list_file.endswith(".csv"):
+        burst_list = pd.read_csv(burst_list_file)
+    elif burst_list_file.endswith(".xlsx"):
+        burst_list = pd.read_excel(burst_list_file)
+    else:
+        raise ValueError("Unknown file format")
+    return burst_list
```

### Comparing `ecallisto_ng-0.7.11/src/ecallisto_ng/combine_antennas/combine.py` & `ecallisto_ng-0.7.12/src/ecallisto_ng/combine_antennas/combine.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,165 +1,163 @@
-import numpy as np
-import torch
-
-from ecallisto_ng.combine_antennas.utils import (
-    align_to_reference,
-    get_cross_corr_matrix,
-    make_frequencies_match_spectograms,
-    make_times_match_spectograms,
-    shift_spectrograms,
-)
-from ecallisto_ng.data_processing.utils import (
-    apply_median_filter,
-    intensity_to_linear,
-    linear_to_intensity,
-    mean_filter,
-    subtract_constant_background,
-    subtract_low_signal_noise_background,
-)
-
-
-def match_spectrograms(datas):
-    """
-    Match the time and frequency dimensions across a list of spectrogram DataFrames.
-    Basically, takes the max and min time and frequency values and makes all the
-    DataFrames have the same time and frequency dimensions and fills them with nans.
-    Incase a NaN is between numbers, it is linearly interpolated.
-
-    Parameters
-    ----------
-    datas : list of pd.DataFrame
-        List of spectrogram DataFrames to be matched.
-
-    Returns
-    -------
-    list of pd.DataFrame
-        List of matched spectrogram DataFrames.
-    """
-    data_processed = make_times_match_spectograms(datas)
-    data_processed = make_frequencies_match_spectograms(data_processed)
-    return data_processed
-
-
-def sync_spectrograms(dfs, shifts=None, method="maximize_cross_correlation"):
-    """
-    Synchronize a list of spectrograms based on pairwise cross-correlation.
-    If the nans are not removed, this method does not work because it can
-    lead to pointless shifts.
-
-    Parameters
-    ----------
-    dfs : list of pd.DataFrame
-        List of spectrogram DataFrames to be synchronized.
-    shifts : np.ndarray, optional
-        List of shifts to apply to each DataFrame, incase you want to
-        calculate the shift outside of this function.
-    method : str, optional
-        The method used for synchronization. Currently only supports 'maximize_cross_correlation'.
-        Default is 'maximize_cross_correlation'.
-
-    Returns
-    -------
-    list of pd.DataFrame
-        List of synchronized spectrogram DataFrames.
-    int or None
-        Index of the DataFrame used as a reference for synchronization.
-    """
-    if method != "maximize_cross_correlation":
-        raise ValueError("Unsupported method")
-    if shifts is not None:
-        shifted_specs = shift_spectrograms(dfs, shifts)
-        ref_idx = None
-
-    elif method == "maximize_cross_correlation":
-        # Check if all dataframes have no missing values.
-        # if they do, this method does not work
-        for df in dfs:
-            if df.isnull().all(axis=1).any():
-                ValueError(
-                    "Time axis of a df is all nan. This method does not work with nan values."
-                )
-        cross_corr_matrix = get_cross_corr_matrix(dfs)
-        # Find the best reference and align all to it
-        ref_idx, shifts_to_ref = align_to_reference(cross_corr_matrix)
-        shifted_specs = shift_spectrograms(dfs, shifts_to_ref)
-    else:
-        raise ValueError(
-            "Unsupported method. Only 'maximize_cross_correlation' supported"
-            "or provide the shifts manually."
-        )
-
-    return shifted_specs, ref_idx
-
-
-def preprocess_data(
-    datas,
-    db_space,
-    min_n_frequencies,
-    freq_range,
-    filter_type,
-    subtract_background,
-    resample_func="MEAN",
-):
-    """
-    Process a list of DataFrames based on a series of filtering and transformation steps.
-
-    Parameters
-    ----------
-    datas : list of pd.DataFrame
-        List of DataFrames to be processed.
-    min_n_frequencies : int, optional
-        Minimum number of frequencies required for processing. Default is 100.
-    freq_range : list of float, optional
-        Frequency range to keep. Default is [20, 80].
-    filter_type : str, optional
-        Type of filter to apply ('median' or 'mean'). Default is None.
-    resample_func : str, optional
-        Resampling function to use. Default is 'MEAN'.
-
-    Returns
-    -------
-    list of pd.DataFrame
-        List of processed DataFrames.
-    """
-    data_processed = []
-    for data in datas:
-        # Cut away columns based on frequency limits
-        columns = np.array([float(col) for col in data.columns])
-        data = data.loc[:, (columns > freq_range[0]) & (columns < freq_range[1])]
-
-        # Resample data
-        if resample_func == "MAX":
-            data = data.resample("250ms").max()
-        elif resample_func == "MIN":
-            data = data.resample("250ms").min()
-        elif resample_func == "MEAN":
-            data = data.resample("250ms").mean()
-        else:
-            raise ValueError("Unsupported resampling function")
-
-        # Check column conditions
-        if len(data.columns) < min_n_frequencies:
-            print(
-                f"Skipping {data.attrs['FULLNAME']} it has only {len(data.columns)} / {min_n_frequencies} frequencies"
-            )
-            continue
-
-        if db_space:
-            data = intensity_to_linear(data)
-
-        if subtract_background:
-            data = subtract_constant_background(data)
-            data = subtract_low_signal_noise_background(data)
-
-        # Apply filter if specified
-        if filter_type == "median":
-            data = apply_median_filter(data)
-        if filter_type == "mean":
-            data = mean_filter(data)
-
-        # Min max scale data per frequency
-        data = (data - data.min()) / (data.max() - data.min())
-
-        # Append processed data
-        data_processed.append(data)
-    return data_processed
+import numpy as np
+import torch
+
+from ecallisto_ng.combine_antennas.utils import (
+    align_to_reference,
+    get_cross_corr_matrix,
+    make_frequencies_match_spectograms,
+    make_times_match_spectograms,
+    shift_spectrograms,
+)
+from ecallisto_ng.data_processing.utils import (
+    apply_median_filter,
+    intensity_to_linear,
+    mean_filter,
+    min_max_scale_per_column,
+    subtract_constant_background,
+    subtract_low_signal_noise_background,
+)
+from ecallisto_ng.plotting.utils import downcast_timedelta
+
+
+def match_spectrograms(datas):
+    """
+    Match the time and frequency dimensions across a list of spectrogram DataFrames.
+    Basically, takes the max and min time and frequency values and makes all the
+    DataFrames have the same time and frequency dimensions and fills them with nans.
+    Incase a NaN is between numbers, it is linearly interpolated.
+
+    Parameters
+    ----------
+    datas : list of pd.DataFrame
+        List of spectrogram DataFrames to be matched.
+
+    Returns
+    -------
+    list of pd.DataFrame
+        List of matched spectrogram DataFrames.
+    """
+    data_processed = make_times_match_spectograms(datas)
+    data_processed = make_frequencies_match_spectograms(data_processed)
+    return data_processed
+
+
+def sync_spectrograms(dfs, shifts=None, method="maximize_cross_correlation"):
+    """
+    Synchronize a list of spectrograms based on pairwise cross-correlation.
+    If the nans are not removed, this method does not work because it can
+    lead to pointless shifts.
+
+    Parameters
+    ----------
+    dfs : list of pd.DataFrame
+        List of spectrogram DataFrames to be synchronized.
+    shifts : np.ndarray, optional
+        List of shifts to apply to each DataFrame, incase you want to
+        calculate the shift outside of this function.
+    method : str, optional
+        The method used for synchronization. Currently only supports 'maximize_cross_correlation'.
+        Default is 'maximize_cross_correlation'.
+
+    Returns
+    -------
+    list of pd.DataFrame
+        List of synchronized spectrogram DataFrames.
+    int or None
+        Index of the DataFrame used as a reference for synchronization.
+    """
+    if method != "maximize_cross_correlation":
+        raise ValueError("Unsupported method")
+    if shifts is not None:
+        shifted_specs = shift_spectrograms(dfs, shifts)
+        ref_idx = None
+
+    elif method == "maximize_cross_correlation":
+        # Check if all dataframes have no missing values.
+        # if they do, this method does not work
+        for df in dfs:
+            if df.isnull().all(axis=1).any():
+                ValueError(
+                    "Time axis of a df is all nan. This method does not work with nan values."
+                )
+        cross_corr_matrix = get_cross_corr_matrix(dfs)
+        # Find the best reference and align all to it
+        ref_idx, shifts_to_ref = align_to_reference(cross_corr_matrix)
+        shifted_specs = shift_spectrograms(dfs, shifts_to_ref)
+    else:
+        raise ValueError(
+            "Unsupported method. Only 'maximize_cross_correlation' supported"
+            "or provide the shifts manually."
+        )
+
+    return shifted_specs, ref_idx
+
+
+def preprocess_data(
+    datas,
+    db_space,
+    resample_time_delta,
+    min_n_frequencies,
+    freq_range,
+    filter_type,
+    filter_size,
+    subtract_background,
+    resample_func="MEAN",
+):
+    """
+    Process a list of DataFrames based on a series of filtering and transformation steps.
+
+    Parameters
+    ----------
+    datas : list of pd.DataFrame
+        List of DataFrames to be processed.
+    min_n_frequencies : int, optional
+        Minimum number of frequencies required for processing. Default is 100.
+    freq_range : list of float, optional
+        Frequency range to keep. Default is [20, 80].
+    filter_type : str, optional
+        Type of filter to apply ('median' or 'mean'). Default is None.
+    filter_size: tuple(int, int)
+        Size of filter in pixel.
+    resample_func : str, optional
+        Resampling function to use. Default is 'MEAN'.
+
+    Returns
+    -------
+    list of pd.DataFrame
+        List of processed DataFrames.
+    """
+    data_processed = []
+    for data in datas:
+        # Cut away columns based on frequency limits
+        columns = np.array([float(col) for col in data.columns])
+        data = data.loc[:, (columns > freq_range[0]) & (columns < freq_range[1])]
+
+        # Resample data
+        data = downcast_timedelta(data, resample_time_delta, resample_func)
+
+        # Check column conditions
+        if len(data.columns) < min_n_frequencies:
+            print(
+                f"Skipping {data.attrs['FULLNAME']} it has only has {len(data.columns)} out of {min_n_frequencies} frequencies"
+            )
+            continue
+
+        if db_space:
+            data = intensity_to_linear(data)
+
+        if subtract_background:
+            data = subtract_constant_background(data)
+            data = subtract_low_signal_noise_background(data)
+
+        # Apply filter if specified
+        if filter_type == "median":
+            data = apply_median_filter(data, filter_size)
+        if filter_type == "mean":
+            data = mean_filter(data, filter_size)
+
+        # Min max scale data per frequency
+        data = min_max_scale_per_column(data)
+
+        # Append processed data
+        data_processed.append(data)
+    return data_processed
```

### Comparing `ecallisto_ng-0.7.11/src/ecallisto_ng/combine_antennas/utils.py` & `ecallisto_ng-0.7.12/src/ecallisto_ng/combine_antennas/utils.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,303 +1,303 @@
-from typing import List
-
-import numpy as np
-import pandas as pd
-import torch
-import torch.nn.functional as F
-
-from ecallisto_ng.plotting.utils import fill_missing_timesteps_with_nan
-
-
-def make_times_match_spectograms(dfs: List[pd.DataFrame]) -> List[pd.DataFrame]:
-    """
-    Adjusts the time index of the given list of DataFrames to have the same start and end times.
-
-    Parameters
-    ----------
-    dfs : List[pd.DataFrame]
-        List of DataFrames with datetime index.
-
-    Returns
-    -------
-    List[pd.DataFrame]
-        List of DataFrames with the adjusted datetime index.
-    """
-    min_datetime = min([df.index.min() for df in dfs])
-    max_datetime = max([df.index.max() for df in dfs])
-    new_dfs = []
-    for df in dfs:
-        df = fill_missing_timesteps_with_nan(
-            df, start_datetime=min_datetime, end_datetime=max_datetime
-        )
-        df = df.interpolate(method="linear", axis=0, limit_area="inside")
-        new_dfs.append(df)
-
-    return new_dfs
-
-
-def interpolate_columns(df: pd.DataFrame, all_columns: List[float]) -> pd.DataFrame:
-    """
-    Interpolates missing columns in a DataFrame.
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        DataFrame to interpolate.
-    all_columns : List[float]
-        List of all columns to include in the DataFrame.
-
-    Returns
-    -------
-    pd.DataFrame
-        DataFrame with interpolated values.
-    """
-    df = df.reindex(columns=all_columns)
-    df.interpolate(method="linear", axis=1, inplace=True, limit_area="inside")
-    return df
-
-
-def make_frequencies_match_spectograms(dfs: List[pd.DataFrame]) -> List[pd.DataFrame]:
-    """
-    Makes frequency columns across multiple spectrogram DataFrames consistent.
-
-    Parameters
-    ----------
-    dfs : List[pd.DataFrame]
-        List of spectrogram DataFrames.
-
-    Returns
-    -------
-    List[pd.DataFrame]
-        List of DataFrames with matching frequency columns.
-    """
-    all_columns = sorted(list(set(float(col) for df in dfs for col in df.columns)))
-    all_columns = [str(col) for col in all_columns]
-    new_dfs = [interpolate_columns(df, all_columns) for df in dfs]
-    return new_dfs
-
-
-def get_max_cross_corr_shift(spec1, spec2):
-    """
-    Get the shift amount that maximizes the cross-correlation between two spectrograms.
-
-    Parameters
-    ----------
-    spec1 : np.array
-        First spectrogram.
-    spec2 : np.array
-        Second spectrogram.
-
-    Returns
-    -------
-    int
-        Shift amount for the second spectrogram that maximizes the cross-correlation.
-    """
-    cross_corr = np.correlate(
-        spec1.sum(axis=1).values, spec2.sum(axis=1).values, mode="full"
-    )
-    return cross_corr.argmax() - (len(spec1) - 1)
-
-
-def get_cross_corr_matrix(specs: List[pd.DataFrame]) -> np.ndarray:
-    """
-    Get the cross-correlation matrix between a list of spectrograms.
-
-    Parameters
-    ----------
-    specs : List[pd.DataFrame]
-        List of spectrograms.
-
-    Returns
-    -------
-    torch.Tensor
-        Cross-correlation matrix.
-    """
-    n_specs = len(specs)
-    cross_corr_matrix = np.zeros((n_specs, n_specs))
-    for i in range(n_specs):
-        for j in range(i + 1, n_specs):
-            shift = get_max_cross_corr_shift(specs[i], specs[j])
-            cross_corr_matrix[i, j] = shift
-            cross_corr_matrix[j, i] = -shift
-    return cross_corr_matrix
-
-
-def find_best_reference(cross_corr_matrix):
-    """
-    Find the best reference spectrogram based on the minimum sum of shifts.
-
-    Parameters
-    ----------
-    cross_corr_matrix : np.ndarray
-        Cross-correlation matrix.
-
-    Returns
-    -------
-    int
-        Index of the best reference spectrogram.
-    """
-    abs_sum_shifts = np.sum(np.abs(cross_corr_matrix), axis=1)
-    return abs_sum_shifts.argmin()
-
-
-def align_to_reference(cross_corr_matrix):
-    """
-    Align all spectrograms to the best reference based on the cross-correlation matrix.
-
-    Parameters
-    ----------
-    cross_corr_matrix : torch.Tensor
-        Cross-correlation matrix.
-
-    Returns
-    -------
-    int, torch.Tensor
-        Index of reference and shifts needed to align to the reference.
-    """
-    ref_idx = find_best_reference(cross_corr_matrix)
-    shifts_to_ref = cross_corr_matrix[ref_idx]
-    return ref_idx, shifts_to_ref
-
-
-def shift_spectrograms(spec_list, shifts):
-    """
-    Shift spectrograms based on the given shifts.
-
-    Parameters
-    ----------
-    spec_list : list of pd.DataFrame
-        List of spectrograms.
-    shifts : np.ndarray
-        Shift amounts for each spectrogram.
-
-    Returns
-    -------
-    list of torch.Tensor
-        List of shifted spectrograms.
-    """
-    shifted_spectrograms = []
-    for shift_, spec in zip(shifts, spec_list):
-        shifted_spec = spec.shift(int(shift_))
-        shifted_spectrograms.append(shifted_spec)
-    return shifted_spectrograms
-
-
-def round_frequencies_to_nearest_bin(dfs, bin_size, method="rebin"):
-    """
-    Rounds each frequency column in multiple DataFrames to the nearest bin edge and groups them.
-    This is so that the frequencies are consistent across multiple DataFrames and we don't
-    have to deal with a huge number of columns.
-
-    Parameters
-    ----------
-    dfs : list of pandas.DataFrame
-        List of DataFrames containing the spectrograms. Columns in each DataFrame are frequencies.
-    bin_size : float
-        The size of the frequency bins.
-    method : str, optional
-        The method used for rounding. Either by rebinning or by rounding to the nearest bin edge.
-
-    Returns
-    -------
-    list of pandas.DataFrame
-        New list of DataFrames with binned frequencies.
-    """
-    rounded_dfs = []
-    for df in dfs:
-        if method == "round":
-            rounded_df = round_col_to_nearest_bin(df.copy(), bin_size)
-        elif method == "rebin":
-            rounded_df = rebin_dataframe(df.copy(), bin_size)
-        rounded_dfs.append(rounded_df)
-
-    return rounded_dfs
-
-
-def round_col_to_nearest_bin(df, bin_size):
-    """
-    Rounds each frequency column to the nearest bin edge and groups them.
-
-    Parameters
-    ----------
-    df : pandas.DataFrame
-        The DataFrame containing the spectrogram. Columns are frequencies.
-    bin_size : float
-        The size of the frequency bins.
-
-    Returns
-    -------
-    pandas.DataFrame
-        New DataFrame with binned frequencies.
-    """
-
-    # Cast column labels to float, round them, then cast back to str
-    rounded_columns = np.round(df.columns.astype(float) / bin_size) * bin_size
-    rounded_columns = np.round(rounded_columns, 1)
-    df.columns = rounded_columns.astype(str)
-
-    # Group by rounded frequencies and average the values
-    return df.T.groupby(df.columns).mean().T
-
-
-def compute_weights(old_freqs, new_freqs, new_res):
-    """
-    Vectorized computation of weights for each old frequency based on their overlap with the new frequency bins.
-
-    Parameters:
-    old_freqs (np.array): Array of old frequency values.
-    new_freqs (np.array): Array of new frequency bin values.
-    new_res (float): New resolution.
-
-    Returns:
-    np.array: 2D array of weights for each old frequency against each new frequency.
-    """
-    # Calculate the boundaries of each old frequency bin
-    left_bounds = np.zeros_like(old_freqs)
-    right_bounds = np.zeros_like(old_freqs)
-
-    left_bounds[1:] = (old_freqs[1:] + old_freqs[:-1]) / 2
-    left_bounds[0] = old_freqs[0] - (old_freqs[1] - old_freqs[0]) / 2
-
-    right_bounds[:-1] = left_bounds[1:]
-    right_bounds[-1] = old_freqs[-1] + (old_freqs[-1] - old_freqs[-2]) / 2
-
-    # Calculate overlaps for each old frequency against each new frequency
-    new_freqs_expanded = new_freqs.reshape(1, -1)
-    overlaps = np.maximum(
-        np.minimum(right_bounds.reshape(-1, 1), new_freqs_expanded + new_res / 2)
-        - np.maximum(left_bounds.reshape(-1, 1), new_freqs_expanded - new_res / 2),
-        0,
-    )
-
-    return overlaps
-
-
-def round_to_nearest(x, base):
-    return base * round(x / base)
-
-
-def rebin_dataframe(df, new_res):
-    """
-    Optimized rebinning of DataFrame using vectorized operations.
-
-    Parameters:
-    df (pd.DataFrame): DataFrame with datetime index and frequency columns.
-    new_res (float): New resolution.
-
-    Returns:
-    pd.DataFrame: Rebinned DataFrame.
-    """
-    old_freqs = np.round(np.array(df.columns, dtype=np.float64), 5)
-
-    start_freq = new_res * round_to_nearest(old_freqs.min(), new_res)
-    end_freq = new_res * round_to_nearest(old_freqs.max(), new_res)
-    new_freqs = np.arange(start_freq, end_freq, new_res)
-    weights = compute_weights(old_freqs, new_freqs, new_res)
-
-    # Normalize weights and compute rebinned values
-    normalized_weights = weights / weights.sum(axis=0)
-    rebinned_values = df.values @ normalized_weights
-
-    rebinned_df = pd.DataFrame(rebinned_values, index=df.index, columns=new_freqs)
-
-    return rebinned_df
+from typing import List
+
+import numpy as np
+import pandas as pd
+import torch
+import torch.nn.functional as F
+
+from ecallisto_ng.plotting.utils import fill_missing_timesteps_with_nan
+
+
+def make_times_match_spectograms(dfs: List[pd.DataFrame]) -> List[pd.DataFrame]:
+    """
+    Adjusts the time index of the given list of DataFrames to have the same start and end times.
+
+    Parameters
+    ----------
+    dfs : List[pd.DataFrame]
+        List of DataFrames with datetime index.
+
+    Returns
+    -------
+    List[pd.DataFrame]
+        List of DataFrames with the adjusted datetime index.
+    """
+    min_datetime = min([df.index.min() for df in dfs])
+    max_datetime = max([df.index.max() for df in dfs])
+    new_dfs = []
+    for df in dfs:
+        df = fill_missing_timesteps_with_nan(
+            df, start_datetime=min_datetime, end_datetime=max_datetime
+        )
+        df = df.interpolate(method="linear", axis=0, limit_area="inside")
+        new_dfs.append(df)
+
+    return new_dfs
+
+
+def interpolate_columns(df: pd.DataFrame, all_columns: List[float]) -> pd.DataFrame:
+    """
+    Interpolates missing columns in a DataFrame.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        DataFrame to interpolate.
+    all_columns : List[float]
+        List of all columns to include in the DataFrame.
+
+    Returns
+    -------
+    pd.DataFrame
+        DataFrame with interpolated values.
+    """
+    df = df.reindex(columns=all_columns)
+    df.interpolate(method="linear", axis=1, inplace=True, limit_area="inside")
+    return df
+
+
+def make_frequencies_match_spectograms(dfs: List[pd.DataFrame]) -> List[pd.DataFrame]:
+    """
+    Makes frequency columns across multiple spectrogram DataFrames consistent.
+
+    Parameters
+    ----------
+    dfs : List[pd.DataFrame]
+        List of spectrogram DataFrames.
+
+    Returns
+    -------
+    List[pd.DataFrame]
+        List of DataFrames with matching frequency columns.
+    """
+    all_columns = sorted(list(set(float(col) for df in dfs for col in df.columns)))
+    all_columns = [str(col) for col in all_columns]
+    new_dfs = [interpolate_columns(df, all_columns) for df in dfs]
+    return new_dfs
+
+
+def get_max_cross_corr_shift(spec1, spec2):
+    """
+    Get the shift amount that maximizes the cross-correlation between two spectrograms.
+
+    Parameters
+    ----------
+    spec1 : np.array
+        First spectrogram.
+    spec2 : np.array
+        Second spectrogram.
+
+    Returns
+    -------
+    int
+        Shift amount for the second spectrogram that maximizes the cross-correlation.
+    """
+    cross_corr = np.correlate(
+        spec1.sum(axis=1).values, spec2.sum(axis=1).values, mode="full"
+    )
+    return cross_corr.argmax() - (len(spec1) - 1)
+
+
+def get_cross_corr_matrix(specs: List[pd.DataFrame]) -> np.ndarray:
+    """
+    Get the cross-correlation matrix between a list of spectrograms.
+
+    Parameters
+    ----------
+    specs : List[pd.DataFrame]
+        List of spectrograms.
+
+    Returns
+    -------
+    torch.Tensor
+        Cross-correlation matrix.
+    """
+    n_specs = len(specs)
+    cross_corr_matrix = np.zeros((n_specs, n_specs))
+    for i in range(n_specs):
+        for j in range(i + 1, n_specs):
+            shift = get_max_cross_corr_shift(specs[i], specs[j])
+            cross_corr_matrix[i, j] = shift
+            cross_corr_matrix[j, i] = -shift
+    return cross_corr_matrix
+
+
+def find_best_reference(cross_corr_matrix):
+    """
+    Find the best reference spectrogram based on the minimum sum of shifts.
+
+    Parameters
+    ----------
+    cross_corr_matrix : np.ndarray
+        Cross-correlation matrix.
+
+    Returns
+    -------
+    int
+        Index of the best reference spectrogram.
+    """
+    abs_sum_shifts = np.sum(np.abs(cross_corr_matrix), axis=1)
+    return abs_sum_shifts.argmin()
+
+
+def align_to_reference(cross_corr_matrix):
+    """
+    Align all spectrograms to the best reference based on the cross-correlation matrix.
+
+    Parameters
+    ----------
+    cross_corr_matrix : torch.Tensor
+        Cross-correlation matrix.
+
+    Returns
+    -------
+    int, torch.Tensor
+        Index of reference and shifts needed to align to the reference.
+    """
+    ref_idx = find_best_reference(cross_corr_matrix)
+    shifts_to_ref = cross_corr_matrix[ref_idx]
+    return ref_idx, shifts_to_ref
+
+
+def shift_spectrograms(spec_list, shifts):
+    """
+    Shift spectrograms based on the given shifts.
+
+    Parameters
+    ----------
+    spec_list : list of pd.DataFrame
+        List of spectrograms.
+    shifts : np.ndarray
+        Shift amounts for each spectrogram.
+
+    Returns
+    -------
+    list of torch.Tensor
+        List of shifted spectrograms.
+    """
+    shifted_spectrograms = []
+    for shift_, spec in zip(shifts, spec_list):
+        shifted_spec = spec.shift(int(shift_))
+        shifted_spectrograms.append(shifted_spec)
+    return shifted_spectrograms
+
+
+def round_frequencies_to_nearest_bin(dfs, bin_size, method="rebin"):
+    """
+    Rounds each frequency column in multiple DataFrames to the nearest bin edge and groups them.
+    This is so that the frequencies are consistent across multiple DataFrames and we don't
+    have to deal with a huge number of columns.
+
+    Parameters
+    ----------
+    dfs : list of pandas.DataFrame
+        List of DataFrames containing the spectrograms. Columns in each DataFrame are frequencies.
+    bin_size : float
+        The size of the frequency bins.
+    method : str, optional
+        The method used for rounding. Either by rebinning or by rounding to the nearest bin edge.
+
+    Returns
+    -------
+    list of pandas.DataFrame
+        New list of DataFrames with binned frequencies.
+    """
+    rounded_dfs = []
+    for df in dfs:
+        if method == "round":
+            rounded_df = round_col_to_nearest_bin(df.copy(), bin_size)
+        elif method == "rebin":
+            rounded_df = rebin_dataframe(df.copy(), bin_size)
+        rounded_dfs.append(rounded_df)
+
+    return rounded_dfs
+
+
+def round_col_to_nearest_bin(df, bin_size):
+    """
+    Rounds each frequency column to the nearest bin edge and groups them.
+
+    Parameters
+    ----------
+    df : pandas.DataFrame
+        The DataFrame containing the spectrogram. Columns are frequencies.
+    bin_size : float
+        The size of the frequency bins.
+
+    Returns
+    -------
+    pandas.DataFrame
+        New DataFrame with binned frequencies.
+    """
+
+    # Cast column labels to float, round them, then cast back to str
+    rounded_columns = np.round(df.columns.astype(float) / bin_size) * bin_size
+    rounded_columns = np.round(rounded_columns, 1)
+    df.columns = rounded_columns.astype(str)
+
+    # Group by rounded frequencies and average the values
+    return df.T.groupby(df.columns).mean().T
+
+
+def compute_weights(old_freqs, new_freqs, new_res):
+    """
+    Vectorized computation of weights for each old frequency based on their overlap with the new frequency bins.
+
+    Parameters:
+    old_freqs (np.array): Array of old frequency values.
+    new_freqs (np.array): Array of new frequency bin values.
+    new_res (float): New resolution.
+
+    Returns:
+    np.array: 2D array of weights for each old frequency against each new frequency.
+    """
+    # Calculate the boundaries of each old frequency bin
+    left_bounds = np.zeros_like(old_freqs)
+    right_bounds = np.zeros_like(old_freqs)
+
+    left_bounds[1:] = (old_freqs[1:] + old_freqs[:-1]) / 2
+    left_bounds[0] = old_freqs[0] - (old_freqs[1] - old_freqs[0]) / 2
+
+    right_bounds[:-1] = left_bounds[1:]
+    right_bounds[-1] = old_freqs[-1] + (old_freqs[-1] - old_freqs[-2]) / 2
+
+    # Calculate overlaps for each old frequency against each new frequency
+    new_freqs_expanded = new_freqs.reshape(1, -1)
+    overlaps = np.maximum(
+        np.minimum(right_bounds.reshape(-1, 1), new_freqs_expanded + new_res / 2)
+        - np.maximum(left_bounds.reshape(-1, 1), new_freqs_expanded - new_res / 2),
+        0,
+    )
+
+    return overlaps
+
+
+def round_to_nearest(x, base):
+    return base * round(x / base)
+
+
+def rebin_dataframe(df, new_res):
+    """
+    Optimized rebinning of DataFrame using vectorized operations.
+
+    Parameters:
+    df (pd.DataFrame): DataFrame with datetime index and frequency columns.
+    new_res (float): New resolution.
+
+    Returns:
+    pd.DataFrame: Rebinned DataFrame.
+    """
+    old_freqs = np.round(np.array(df.columns, dtype=np.float64), 5)
+
+    start_freq = new_res * round_to_nearest(old_freqs.min(), new_res)
+    end_freq = new_res * round_to_nearest(old_freqs.max(), new_res)
+    new_freqs = np.arange(start_freq, end_freq, new_res)
+    weights = compute_weights(old_freqs, new_freqs, new_res)
+
+    # Normalize weights and compute rebinned values
+    normalized_weights = weights / weights.sum(axis=0)
+    rebinned_values = df.values @ normalized_weights
+
+    rebinned_df = pd.DataFrame(rebinned_values, index=df.index, columns=new_freqs)
+
+    return rebinned_df
```

### Comparing `ecallisto_ng-0.7.11/src/ecallisto_ng/data_download/downloader.py` & `ecallisto_ng-0.7.12/src/ecallisto_ng/data_download/downloader.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,402 +1,398 @@
-import fnmatch
-import glob
-import os
-import traceback
-from concurrent.futures import ProcessPoolExecutor
-from datetime import datetime, timedelta
-from functools import partial
-
-import pandas as pd
-import requests
-from astropy.io import fits
-from bs4 import BeautifulSoup
-from tqdm import tqdm
-
-from ecallisto_ng.data_download.utils import (
-    concat_dfs_by_instrument,
-    ecallisto_fits_to_pandas,
-    extract_datetime_from_filename,
-    extract_instrument_name,
-    filter_dataframes,
-    instrument_name_to_globbing_pattern,
-)
-
-BASE_URL = "http://soleil80.cs.technik.fhnw.ch/solarradio/data/2002-20yy_Callisto"
-LOCAL_PATH = "/mnt/nas05/data01/radio/2002-20yy_Callisto"
-
-
-def get_ecallisto_data(
-    start_datetime,
-    end_datetime,
-    instrument_name=None,
-    verbose=False,
-    freq_start=None,
-    freq_end=None,
-    download_from_local=False,
-):
-    """
-    Get the e-Callisto data within a date range and optional instrument regex pattern.
-    For big requests, it is recommended to use the generator function `get_ecallisto_data_generator`,
-    which allows for processing each file individually without loading everything into memory at once.
-
-    Parameters
-    ----------
-    start_datetime : datetime-like
-        The start date for the file search.
-    end_datetime : datetime-like
-        The end date for the file search.
-    instrument_string : str or None
-        The instrument name you want to match in file URLs. If None, all files are considered.
-        Substrings also work, such as 'ALASKA'.
-    verbose : bool
-        Whether to print progress information.
-    freq_start : float or None
-        The start frequency for the filter.
-    freq_end : float or None
-        The end frequency for the filter.
-    download_from_local : bool
-        Whether to download the files from the local directory instead of the remote directory.
-        Useful if you are working with a local copy of the data.
-
-    Returns
-    -------
-    dict of str: `~pandas.DataFrame` or `~pandas.DataFrame`
-        Dictionary of instrument names and their corresponding dataframes.
-    """
-    if download_from_local:
-        file_urls = get_local_file_paths(start_datetime, end_datetime, instrument_name)
-    else:
-        file_urls = get_remote_files_url(start_datetime, end_datetime, instrument_name)
-    if not file_urls and verbose:
-        print(
-            f"No files found for {instrument_name} between {start_datetime} and {end_datetime}."
-        )
-        return {}
-    dfs = download_fits_process_to_pandas(file_urls, verbose)
-    dfs = concat_dfs_by_instrument(dfs, verbose)
-    dfs = filter_dataframes(
-        dfs,
-        start_datetime,
-        end_datetime,
-        verbose,
-        freq_start=freq_start,
-        freq_end=freq_end,
-    )
-    return dfs
-
-
-def get_ecallisto_data_generator(
-    start_datetime,
-    end_datetime,
-    instrument_name=None,
-    freq_start=None,
-    freq_end=None,
-    verbose=False,
-    base_url=BASE_URL,
-):
-    """
-    Generator function to yield e-Callisto data one file at a time within a date range.
-    It returns a tuple with (instrument_name, dataframe)
-
-    This function is a generator, using `yield` to return dataframes one by one. This is beneficial
-    for handling large datasets or when working with limited memory, as it allows for processing
-    each file individually without loading everything into memory at once.
-
-    Parameters
-    ----------
-    start_datetime : datetime-like
-        The start date for the file search.
-    end_datetime : datetime-like
-        The end date for the file search.
-    instrument_names : List[str] or str or None
-        The instrument name you want to match in file URLs. If None, all files are considered.
-    freq_start : float or None
-        The start frequency for the filter.
-    freq_end : float or None
-        The end frequency for the filter.
-    base_url : str
-        The base URL of the remote file directory.
-
-    Yields
-    ------
-    pandas.DataFrame
-        A tuple with (instrument_name, dataframe)
-
-    Example
-    -------
-    >>> start = <start_datetime>
-    >>> end = <end_datetime>
-    >>> instrument = <instrument_name>
-    >>> data_generator = get_ecallisto_data_generator(start, end, instrument)
-    >>> for instrument_name, data_frame in data_generator:
-    ...     process_data(data_frame)  # Replace with your processing function or whatever you want to do with the data
-    """
-    if isinstance(instrument_name, str):
-        instrument_name = [instrument_name]
-    if instrument_name is None:
-        # Get all instrument names with available data. This makes the generator more efficient
-        # because it doesn't have to check for each instrument name individually.
-        instrument_name = get_instrument_with_available_data(
-            start_datetime, end_datetime
-        )
-
-    for instrument_name_ in instrument_name:
-        file_urls = get_remote_files_url(
-            start_datetime, end_datetime, instrument_name_, base_url
-        )
-        if not file_urls and verbose:
-            print(
-                f"No files found for {instrument_name} between {start_datetime} and {end_datetime}."
-            )
-            return {}
-        try:
-            dfs = download_fits_process_to_pandas(file_urls)
-            dfs = concat_dfs_by_instrument(dfs)
-            dfs = filter_dataframes(
-                dfs,
-                start_datetime,
-                end_datetime,
-                freq_start=freq_start,
-                freq_end=freq_end,
-            )
-            for key, value in dfs.items():
-                yield key, value
-        except Exception as e:
-            print(f"Error for {instrument_name_}: {e}")
-            print(f"Skipping {instrument_name_}.")
-            continue
-
-
-def get_instrument_with_available_data(
-    start_date=None, end_date=None, instrument_name=None
-):
-    """
-    Retrieve sorted list of unique instrument names with available data in a specified date range.
-
-    Parameters
-    ----------
-    start_date : pd.Timestamp or None
-        The start date for querying data. If None, the current timestamp is used.
-    end_date : pd.Timestamp or None
-        The end date for querying data. If None, it is set to three days prior to the current timestamp.
-    instrument_name : str, optional
-        Name of the specific instrument to query. If None, all available instruments are considered.
-
-    Returns
-    -------
-    list of str
-        A sorted list of unique instrument names for which data is available in the specified date range.
-        Returns an empty list if no data is found.
-
-    Notes
-    -----
-    - The function depends on `get_remote_files_url` to fetch URLs of available data files.
-    - `extract_instrument_name` is used to parse instrument names from the file URLs.
-    - If both `start_date` and `end_date` are None, the function defaults to a date range from the current date to three days prior.
-
-    Examples
-    --------
-    >>> get_instrument_with_available_data(pd.Timestamp('2023-01-01'), pd.Timestamp('2023-01-10'), 'Instrument')
-    ['InstrumentA', 'InstrumentB', 'InstrumentX']
-    """
-    if start_date is None or end_date is None:
-        # Set start_date to now
-        end_date = pd.Timestamp.now()
-        # Set end_date to 1 day ago
-        start_date = end_date - pd.Timedelta(days=1)
-    file_urls = get_remote_files_url(start_date, end_date, instrument_name)
-    if not file_urls:
-        print(
-            f"No files found for {instrument_name} between {start_date} and {end_date}."
-        )
-        return {}
-    instrument_names = [extract_instrument_name(file_url) for file_url in file_urls]
-    return sorted(list(set(instrument_names)))
-
-
-def download_fits_process_to_pandas(file_urls, verbose=False):
-    with ProcessPoolExecutor(max_workers=os.cpu_count()) as executor:
-        # Use tqdm for progress tracking, passing the total number of tasks
-        partial_f = partial(fetch_fits_to_pandas, verbose=verbose)
-        if verbose:
-            # Show progress bar if verbose is True
-            results = list(
-                tqdm(
-                    executor.map(partial_f, file_urls),
-                    total=len(file_urls),
-                    desc="Downloading and processing files",
-                )
-            )
-        else:
-            # Execute without progress bar if verbose is False
-            results = list(executor.map(partial_f, file_urls))
-    # Check if any of the results are None
-    if verbose and any(result is None for result in results):
-        print("Some files could not be downloaded (See traceback above).")
-    # Remove None values
-    results = [result for result in results if result is not None]
-    return results
-
-
-def fetch_fits_to_pandas(file_url, verbose=False):
-    try:
-        fits_file = fits.open(file_url, cache=False)
-        df = ecallisto_fits_to_pandas(fits_file)
-        # Add the instrument name to it
-        df.attrs["ANTENNAID"] = extract_instrument_name(file_url)[-2:]
-        return df
-    except Exception as e:
-        if verbose:
-            print(f"Error for {file_url}: {e}")
-            traceback.print_exc()
-        return None
-
-
-def fetch_date_files(date_url):
-    """
-    Fetch and parse file URLs from a given date URL.
-
-    Parameters
-    ----------
-    date_url : str
-        The URL for a specific date to fetch files from.
-    session : requests.Session
-        The requests session object for HTTP requests.
-
-    Returns
-    -------
-    list of str
-        List of file URLs ending with '.gz'.
-    """
-    session = requests.Session()
-    response = session.get(date_url)
-    try:
-        soup = BeautifulSoup(
-            response.content, "lxml"
-        )  # using lxml parser because it's faster
-        file_names = [
-            link.get("href")
-            for link in soup.find_all("a")
-            if link.get("href").endswith(".gz")
-        ]
-        to_return = [date_url + file_name for file_name in file_names]
-    except Exception as e:
-        print(f"Error fetching {date_url}.")
-        print(e)
-        to_return = []
-    finally:
-        session.close()
-        return to_return
-
-
-def get_remote_files_url(
-    start_date,
-    end_date,
-    instrument_name=None,
-    base_url="http://soleil80.cs.technik.fhnw.ch/solarradio/data/2002-20yy_Callisto",
-):
-    """
-    Get the remote file URLs within a date range and optional instrument regex pattern.
-
-    Parameters
-    ----------
-    start_date : datetime-like
-        The start date for the file search.
-    end_date : datetime-like
-        The end date for the file search.
-    instrument_string : str or None
-        The instrument name you want to match in file URLs. If None, all files are considered.
-        Substrings also work, such as 'ALASKA'.
-    base_url : str
-        The base URL of the remote file directory.
-
-    Returns
-    -------
-    list of str
-        List of file URLs that match the criteria.
-    """
-    file_urls = []
-    date_urls = [
-        f"{base_url}/{date.year}/{str(date.month).zfill(2)}/{str(date.day).zfill(2)}/"
-        for date in pd.date_range(start_date, end_date, inclusive="both")
-    ]
-
-    with ProcessPoolExecutor(max_workers=os.cpu_count()) as executor:
-        # Map each URL to a fetch function with a session
-        results = executor.map(fetch_date_files, date_urls)
-
-    # Flatten the results
-    results = [item for sublist in results for item in sublist]
-
-    glob_pattern = instrument_name_to_globbing_pattern(instrument_name)
-    file_urls = fnmatch.filter(results, glob_pattern)
-
-    # Extact datetime from filename
-    file_datetimes = [
-        extract_datetime_from_filename(file_name) for file_name in file_urls
-    ]
-
-    # Filter out files that are not in the date range
-    file_urls = [
-        file_url
-        for file_url, file_datetime in zip(file_urls, file_datetimes)
-        if start_date - timedelta(minutes=15)
-        <= file_datetime
-        <= end_date + timedelta(minutes=15)
-    ]  # Timedelta because a file contains up to 15 minutes of data
-
-    return file_urls
-
-
-def get_local_file_paths(
-    start_date,
-    end_date,
-    instrument_name=None,
-    base_path=LOCAL_PATH,
-):
-    """
-    Get the local file paths within a date range and optional instrument regex pattern.
-
-    Parameters
-    ----------
-    start_date : datetime-like
-        The start date for the file search.
-    end_date : datetime-like
-        The end date for the file search.
-    instrument_name : str or None
-        The instrument name to match in file paths. If None, all files are considered.
-        Substrings also work, such as 'ALASKA'.
-    base_path : str
-        The base path of the local file directory.
-
-    Returns
-    -------
-    list of str
-        List of file paths that match the criteria.
-    """
-    file_paths = []
-    for date in pd.date_range(start_date, end_date, inclusive="both"):
-        # Define the path for the year, month, and day
-        date_path = os.path.join(
-            base_path, str(date.year), str(date.month).zfill(2), str(date.day).zfill(2)
-        )
-
-        if instrument_name:
-            glob_pattern = instrument_name_to_globbing_pattern(instrument_name)
-            search_pattern = os.path.join(date_path, f"{glob_pattern}")
-        else:
-            search_pattern = os.path.join(date_path, "*")
-
-        # Use glob to find files that match the search pattern
-        for file_path in glob.glob(search_pattern):
-            # Assuming extract_datetime_from_filename extracts the datetime from the filename
-            file_datetime = extract_datetime_from_filename(file_path)
-            # Check if the file's datetime is within the range
-            if (
-                start_date - timedelta(minutes=15)
-                <= file_datetime
-                <= end_date + timedelta(minutes=15)
-            ):
-                file_paths.append(file_path)
-
-    return file_paths
+import fnmatch
+import glob
+import os
+import traceback
+from concurrent.futures import ProcessPoolExecutor
+from datetime import datetime, timedelta
+from functools import partial
+
+import pandas as pd
+import requests
+from astropy.io import fits
+from bs4 import BeautifulSoup
+from tqdm import tqdm
+
+from ecallisto_ng.data_download.utils import (
+    concat_dfs_by_instrument, ecallisto_fits_to_pandas,
+    extract_datetime_from_filename, extract_instrument_name, filter_dataframes,
+    instrument_name_to_globbing_pattern)
+
+BASE_URL = "http://soleil80.cs.technik.fhnw.ch/solarradio/data/2002-20yy_Callisto"
+LOCAL_PATH = "/mnt/nas05/data01/radio/2002-20yy_Callisto"
+
+
+def get_ecallisto_data(
+    start_datetime,
+    end_datetime,
+    instrument_name=None,
+    verbose=False,
+    freq_start=None,
+    freq_end=None,
+    download_from_local=False,
+):
+    """
+    Get the e-Callisto data within a date range and optional instrument regex pattern.
+    For big requests, it is recommended to use the generator function `get_ecallisto_data_generator`,
+    which allows for processing each file individually without loading everything into memory at once.
+
+    Parameters
+    ----------
+    start_datetime : datetime-like
+        The start date for the file search.
+    end_datetime : datetime-like
+        The end date for the file search.
+    instrument_string : str or None
+        The instrument name you want to match in file URLs. If None, all files are considered.
+        Substrings also work, such as 'ALASKA'.
+    verbose : bool
+        Whether to print progress information.
+    freq_start : float or None
+        The start frequency for the filter.
+    freq_end : float or None
+        The end frequency for the filter.
+    download_from_local : bool
+        Whether to download the files from the local directory instead of the remote directory.
+        Useful if you are working with a local copy of the data.
+
+    Returns
+    -------
+    dict of str: `~pandas.DataFrame` or `~pandas.DataFrame`
+        Dictionary of instrument names and their corresponding dataframes.
+    """
+    if download_from_local:
+        file_urls = get_local_file_paths(start_datetime, end_datetime, instrument_name)
+    else:
+        file_urls = get_remote_files_url(start_datetime, end_datetime, instrument_name)
+    if not file_urls and verbose:
+        print(
+            f"No files found for {instrument_name} between {start_datetime} and {end_datetime}."
+        )
+        return {}
+    dfs = download_fits_process_to_pandas(file_urls, verbose)
+    dfs = concat_dfs_by_instrument(dfs, verbose)
+    dfs = filter_dataframes(
+        dfs,
+        start_datetime,
+        end_datetime,
+        verbose,
+        freq_start=freq_start,
+        freq_end=freq_end,
+    )
+    return dfs
+
+
+def get_ecallisto_data_generator(
+    start_datetime,
+    end_datetime,
+    instrument_name=None,
+    freq_start=None,
+    freq_end=None,
+    verbose=False,
+    base_url=BASE_URL,
+):
+    """
+    Generator function to yield e-Callisto data one file at a time within a date range.
+    It returns a tuple with (instrument_name, dataframe)
+
+    This function is a generator, using `yield` to return dataframes one by one. This is beneficial
+    for handling large datasets or when working with limited memory, as it allows for processing
+    each file individually without loading everything into memory at once.
+
+    Parameters
+    ----------
+    start_datetime : datetime-like
+        The start date for the file search.
+    end_datetime : datetime-like
+        The end date for the file search.
+    instrument_names : List[str] or str or None
+        The instrument name you want to match in file URLs. If None, all files are considered.
+    freq_start : float or None
+        The start frequency for the filter.
+    freq_end : float or None
+        The end frequency for the filter.
+    base_url : str
+        The base URL of the remote file directory.
+
+    Yields
+    ------
+    pandas.DataFrame
+        A tuple with (instrument_name, dataframe)
+
+    Example
+    -------
+    >>> start = <start_datetime>
+    >>> end = <end_datetime>
+    >>> instrument = <instrument_name>
+    >>> data_generator = get_ecallisto_data_generator(start, end, instrument)
+    >>> for instrument_name, data_frame in data_generator:
+    ...     process_data(data_frame)  # Replace with your processing function or whatever you want to do with the data
+    """
+    if isinstance(instrument_name, str):
+        instrument_name = [instrument_name]
+    if instrument_name is None:
+        # Get all instrument names with available data. This makes the generator more efficient
+        # because it doesn't have to check for each instrument name individually.
+        instrument_name = get_instrument_with_available_data(
+            start_datetime, end_datetime
+        )
+
+    for instrument_name_ in instrument_name:
+        file_urls = get_remote_files_url(
+            start_datetime, end_datetime, instrument_name_, base_url
+        )
+        if not file_urls and verbose:
+            print(
+                f"No files found for {instrument_name} between {start_datetime} and {end_datetime}."
+            )
+            return {}
+        try:
+            dfs = download_fits_process_to_pandas(file_urls)
+            dfs = concat_dfs_by_instrument(dfs)
+            dfs = filter_dataframes(
+                dfs,
+                start_datetime,
+                end_datetime,
+                freq_start=freq_start,
+                freq_end=freq_end,
+            )
+            for key, value in dfs.items():
+                yield key, value
+        except Exception as e:
+            print(f"Error for {instrument_name_}: {e}")
+            print(f"Skipping {instrument_name_}.")
+            continue
+
+
+def get_instrument_with_available_data(
+    start_date=None, end_date=None, instrument_name=None
+):
+    """
+    Retrieve sorted list of unique instrument names with available data in a specified date range.
+
+    Parameters
+    ----------
+    start_date : pd.Timestamp or None
+        The start date for querying data. If None, the current timestamp is used.
+    end_date : pd.Timestamp or None
+        The end date for querying data. If None, it is set to three days prior to the current timestamp.
+    instrument_name : str, optional
+        Name of the specific instrument to query. If None, all available instruments are considered.
+
+    Returns
+    -------
+    list of str
+        A sorted list of unique instrument names for which data is available in the specified date range.
+        Returns an empty list if no data is found.
+
+    Notes
+    -----
+    - The function depends on `get_remote_files_url` to fetch URLs of available data files.
+    - `extract_instrument_name` is used to parse instrument names from the file URLs.
+    - If both `start_date` and `end_date` are None, the function defaults to a date range from the current date to three days prior.
+
+    Examples
+    --------
+    >>> get_instrument_with_available_data(pd.Timestamp('2023-01-01'), pd.Timestamp('2023-01-10'), 'Instrument')
+    ['InstrumentA', 'InstrumentB', 'InstrumentX']
+    """
+    if start_date is None or end_date is None:
+        # Set start_date to now
+        end_date = pd.Timestamp.now()
+        # Set end_date to 1 day ago
+        start_date = end_date - pd.Timedelta(days=1)
+    file_urls = get_remote_files_url(start_date, end_date, instrument_name)
+    if not file_urls:
+        print(
+            f"No files found for {instrument_name} between {start_date} and {end_date}."
+        )
+        return {}
+    instrument_names = [extract_instrument_name(file_url) for file_url in file_urls]
+    return sorted(list(set(instrument_names)))
+
+
+def download_fits_process_to_pandas(file_urls, verbose=False):
+    with ProcessPoolExecutor(max_workers=os.cpu_count()) as executor:
+        # Use tqdm for progress tracking, passing the total number of tasks
+        partial_f = partial(fetch_fits_to_pandas, verbose=verbose)
+        if verbose:
+            # Show progress bar if verbose is True
+            results = list(
+                tqdm(
+                    executor.map(partial_f, file_urls),
+                    total=len(file_urls),
+                    desc="Downloading and processing files",
+                )
+            )
+        else:
+            # Execute without progress bar if verbose is False
+            results = list(executor.map(partial_f, file_urls))
+    # Check if any of the results are None
+    if verbose and any(result is None for result in results):
+        print("Some files could not be downloaded (See traceback above).")
+    # Remove None values
+    results = [result for result in results if result is not None]
+    return results
+
+
+def fetch_fits_to_pandas(file_url, verbose=False):
+    try:
+        fits_file = fits.open(file_url, cache=False)
+        df = ecallisto_fits_to_pandas(fits_file)
+        # Add the instrument name to it
+        df.attrs["ANTENNAID"] = extract_instrument_name(file_url)[-2:]
+        return df
+    except Exception as e:
+        if verbose:
+            print(f"Error for {file_url}: {e}")
+            traceback.print_exc()
+        return None
+
+
+def fetch_date_files(date_url):
+    """
+    Fetch and parse file URLs from a given date URL.
+
+    Parameters
+    ----------
+    date_url : str
+        The URL for a specific date to fetch files from.
+    session : requests.Session
+        The requests session object for HTTP requests.
+
+    Returns
+    -------
+    list of str
+        List of file URLs ending with '.gz'.
+    """
+    session = requests.Session()
+    response = session.get(date_url)
+    try:
+        soup = BeautifulSoup(
+            response.content, "lxml"
+        )  # using lxml parser because it's faster
+        file_names = [
+            link.get("href")
+            for link in soup.find_all("a")
+            if link.get("href").endswith(".gz")
+        ]
+        to_return = [date_url + file_name for file_name in file_names]
+    except Exception as e:
+        print(f"Error fetching {date_url}.")
+        print(e)
+        to_return = []
+    finally:
+        session.close()
+        return to_return
+
+
+def get_remote_files_url(
+    start_date,
+    end_date,
+    instrument_name=None,
+    base_url="http://soleil80.cs.technik.fhnw.ch/solarradio/data/2002-20yy_Callisto",
+):
+    """
+    Get the remote file URLs within a date range and optional instrument regex pattern.
+
+    Parameters
+    ----------
+    start_date : datetime-like
+        The start date for the file search.
+    end_date : datetime-like
+        The end date for the file search.
+    instrument_string : str or None
+        The instrument name you want to match in file URLs. If None, all files are considered.
+        Substrings also work, such as 'ALASKA'.
+    base_url : str
+        The base URL of the remote file directory.
+
+    Returns
+    -------
+    list of str
+        List of file URLs that match the criteria.
+    """
+    file_urls = []
+    date_urls = [
+        f"{base_url}/{date.year}/{str(date.month).zfill(2)}/{str(date.day).zfill(2)}/"
+        for date in pd.date_range(start_date, end_date, inclusive="both")
+    ]
+
+    with ProcessPoolExecutor(max_workers=os.cpu_count()) as executor:
+        # Map each URL to a fetch function with a session
+        results = executor.map(fetch_date_files, date_urls)
+
+    # Flatten the results
+    results = [item for sublist in results for item in sublist]
+
+    glob_pattern = instrument_name_to_globbing_pattern(instrument_name)
+    file_urls = fnmatch.filter(results, glob_pattern)
+
+    # Extact datetime from filename
+    file_datetimes = [
+        extract_datetime_from_filename(file_name) for file_name in file_urls
+    ]
+
+    # Filter out files that are not in the date range
+    file_urls = [
+        file_url
+        for file_url, file_datetime in zip(file_urls, file_datetimes)
+        if start_date - timedelta(minutes=15)
+        <= file_datetime
+        <= end_date + timedelta(minutes=15)
+    ]  # Timedelta because a file contains up to 15 minutes of data
+
+    return file_urls
+
+
+def get_local_file_paths(
+    start_date,
+    end_date,
+    instrument_name=None,
+    base_path=LOCAL_PATH,
+):
+    """
+    Get the local file paths within a date range and optional instrument regex pattern.
+
+    Parameters
+    ----------
+    start_date : datetime-like
+        The start date for the file search.
+    end_date : datetime-like
+        The end date for the file search.
+    instrument_name : str or None
+        The instrument name to match in file paths. If None, all files are considered.
+        Substrings also work, such as 'ALASKA'.
+    base_path : str
+        The base path of the local file directory.
+
+    Returns
+    -------
+    list of str
+        List of file paths that match the criteria.
+    """
+    file_paths = []
+    for date in pd.date_range(start_date, end_date, inclusive="both"):
+        # Define the path for the year, month, and day
+        date_path = os.path.join(
+            base_path, str(date.year), str(date.month).zfill(2), str(date.day).zfill(2)
+        )
+
+        if instrument_name:
+            glob_pattern = instrument_name_to_globbing_pattern(instrument_name)
+            search_pattern = os.path.join(date_path, f"{glob_pattern}")
+        else:
+            search_pattern = os.path.join(date_path, "*")
+
+        # Use glob to find files that match the search pattern
+        for file_path in glob.glob(search_pattern):
+            # Assuming extract_datetime_from_filename extracts the datetime from the filename
+            file_datetime = extract_datetime_from_filename(file_path)
+            # Check if the file's datetime is within the range
+            if (
+                start_date - timedelta(minutes=15)
+                <= file_datetime
+                <= end_date + timedelta(minutes=15)
+            ):
+                file_paths.append(file_path)
+
+    return file_paths
```

### Comparing `ecallisto_ng-0.7.11/src/ecallisto_ng/data_download/utils.py` & `ecallisto_ng-0.7.12/src/ecallisto_ng/data_download/utils.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,355 +1,355 @@
-import re
-import warnings
-from datetime import datetime
-
-import numpy as np
-import pandas as pd
-
-
-def filter_dataframes(
-    dfs, start_date, end_date, verbose=False, freq_start=None, freq_end=None
-):
-    """
-    Filter the dataframes in a dictionary by a date range.
-
-    Parameters
-    ----------
-    dfs : dict of str: `~pandas.DataFrame`
-        Dictionary of instrument names and their corresponding dataframes.
-    start_date : datetime-like
-        The start date for the filter.
-    end_date : datetime-like
-        The end date for the filter.
-    verbose : bool
-        Whether to print progress information.
-    freq_start : float or None
-        The start frequency for the filter.
-    freq_end : float or None
-        The end frequency for the filter.
-
-    Returns
-    -------
-    dict of str: `~pandas.DataFrame`
-        Dictionary of instrument names and their corresponding dataframes.
-    """
-    if verbose:
-        print("Filtering dataframes.")
-    for instrument, df in dfs.items():
-        dfs[instrument] = df.loc[start_date:end_date]
-
-    if verbose:
-        print("Filtering frequencies.")
-    if freq_start:
-        for instrument, df in dfs.items():
-            dfs[instrument] = df.loc[:, freq_start:freq_end]
-    if freq_end:
-        for instrument, df in dfs.items():
-            dfs[instrument] = df.loc[:, freq_start:freq_end]
-
-    # Check if any dfs are empty
-    empty_instruments = []
-    for instrument, df in dfs.items():
-        if df.empty:
-            empty_instruments.append(instrument)
-    for instrument in empty_instruments:
-        del dfs[instrument]
-
-    # Update the header
-    if verbose:
-        print("Updating headers after filtering.")
-    for instrument, df in dfs.items():
-        df = readd_edit_header(df, dfs[instrument].attrs)
-    return dfs
-
-
-def extract_datetime_from_filename(file_name):
-    """
-    Extract datetime from the filename.
-
-    Parameters
-    ----------
-    file_name : str
-        The filename from which to extract the datetime.
-
-    Returns
-    -------
-    datetime
-        The extracted datetime object, or None if parsing fails.
-    """
-    # Filename format: 'LOCATION_YYYYMMDD_HHMMSS_X.fit.gz'
-    match = re.search(r"_(\d{8})_(\d{6})", file_name)
-    if match:
-        return datetime.strptime(match.group(1) + match.group(2), "%Y%m%d%H%M%S")
-    return None
-
-
-def instrument_name_to_globbing_pattern(instrument_name=None):
-    """
-    Convert an instrument name (and optional antenna number) to a globbing pattern suitable for matching in file URLs.
-
-    Parameters
-    ----------
-    instrument_name : str
-        The instrument name to be matched in the file URLs.
-
-    Returns
-    -------
-    str
-        A matching pattern string.
-    """
-    if instrument_name is None:
-        return "*.fit.gz"
-    antenna_number = None
-    if instrument_name[-2:].isdigit():
-        antenna_number = instrument_name[-2:]
-        instrument_name = instrument_name[:-3]
-    glob_pattern = "*" + instrument_name + "*"
-    if antenna_number:
-        glob_pattern += antenna_number
-    glob_pattern += ".fit.gz"
-    return glob_pattern
-
-
-def combine_non_unique_frequency_axis(freq_axis, data, agg_function=np.max):
-    """Combine non-unique frequency axis data.
-
-    Parameters
-    ----------
-    spec : `~astropy.io.fits.hdu.hdulist.HDUList`
-        The spectrogram to combine the frequency axis data of.
-    method : callable
-        The method to use to combine the frequency axis data. Defaults to "mean".
-
-    Returns
-    -------
-    unique_freq_axis : `~numpy.ndarray`
-        The unique frequency axis data.
-    data : `~numpy.ndarray`
-        The combined data.
-
-
-    Notes
-    -----
-    The function first finds the unique frequency axis data and the indices of the non-unique frequency axis data.
-    It then combines the non-unique frequency axis data using the method specified by the `method` parameter.
-    """
-    unique_freq, indices = np.unique(freq_axis, return_inverse=True)
-    data = np.array(
-        [agg_function(data[indices == i], axis=0) for i in range(len(unique_freq))]
-    )
-    return unique_freq, data
-
-
-def spec_time_to_pd_datetime(start_datetime, time_axis):
-    """
-    Convert a time axis array to pandas datetime objects, offset by a starting datetime.
-
-    Parameters
-    ----------
-    start_datetime : datetime or Timestamp
-        The starting datetime to which the time axis offsets will be applied.
-    time_axis : array_like
-        An array of time offsets in seconds.
-
-    Returns
-    -------
-    pandas.Series
-        A pandas Series of datetime objects corresponding to each time offset.
-
-    Notes
-    -----
-    This function adds the given time offsets in seconds to the start datetime
-    and converts the result to pandas datetime objects.
-    """
-    return start_datetime + pd.to_timedelta(time_axis, unit="s")
-
-
-def extract_instrument_name(file_path):
-    """Extract the instrument name from a file path.
-
-    Parameters
-    ----------
-    file_path : str
-        The file path to extract the instrument name from.
-
-    Returns
-    -------
-    str
-        The extracted instrument name, converted to lowercase with underscores in place of hyphens.
-
-
-    Example
-    -------
-    >>> extract_instrument_name('/var/lib/ecallisto/2023/01/27/ALASKA-COHOE_20230127_001500_612.fit.gz')
-    'ALASKA_COHOE_612'
-
-    Notes
-    -----
-    The function first selects the last part of the file path and removes the extension.
-    Then, it replaces hyphens with underscores and splits on underscores to get the parts of the file name.
-    The function concatenates these parts, adding a numeric part of the file name if it is less than 6 digits.
-    """
-    # select last part of file path and remove extension
-    file_name = file_path.split("/")[-1].split(".")[0]
-
-    # Remove datetime
-    instrument_name = file_name.split("_")[0]
-    antenna_number = file_name.split("_")[-1]
-    return instrument_name + "_" + antenna_number
-
-
-def extract_identical_dicts(dicts):
-    """
-    Extract identical keys and values from a list of dictionaries.
-
-    Parameters
-    ----------
-    dicts : list of dict
-        The list of dictionaries to extract identical keys and values from.
-
-    Returns
-    -------
-    dict
-        A dictionary of identical keys and values.
-    """
-    identical_keys = set.intersection(*[set(d.keys()) for d in dicts])
-    identical_values = {}
-    for key in identical_keys:
-        values = [d[key] for d in dicts]
-        if len(set(values)) == 1:
-            identical_values[key] = values[0]
-    return identical_values
-
-
-def readd_edit_header(df, dict_):
-    """
-    Re-add and edit header information to a DataFrame.
-
-    This function updates the header of a DataFrame with new values and adds additional
-    time-related and instrument information. It preserves the order of the original header keys.
-
-    Parameters
-    ----------
-    df : pandas.DataFrame
-        DataFrame to which header information will be added or updated.
-    dict_ : dict
-        Dictionary containing header information to be updated or added to `df`.
-
-    Returns
-    -------
-    pandas.DataFrame
-        The DataFrame with updated header information.
-
-    Notes
-    -----
-    The function assumes that the DataFrame `df` has an attribute `header`, which is a dictionary
-    used to store header information. The DataFrame's index is used to derive `DATE-OBS`, `TIME-OBS`,
-    `DATE-END`, and `TIME-END` values.
-    """
-    for key, value in dict_.items():
-        df.attrs[key] = value
-    # Add DATE-OBS and TIME-OBS
-    df.attrs["DATE-OBS"] = df.index[0].strftime("%Y-%m-%d")
-    df.attrs["TIME-OBS"] = df.index[0].strftime("%H:%M:%S")
-    df.attrs["DATE-END"] = df.index[-1].strftime("%Y-%m-%d")
-    df.attrs["TIME-END"] = df.index[-1].strftime("%H:%M:%S")
-    df.attrs["NAXIS1"] = len(df)
-    df.attrs["FULLNAME"] = df.attrs["INSTRUME"] + "_" + df.attrs["ANTENNAID"]
-    return df
-
-
-def concat_dfs_by_instrument(dfs, verbose=False):
-    instruments = {}
-    # Extract attrs from each df
-    headers = [df.attrs for df in dfs]
-    if verbose:
-        print("Combining headers.")
-    for df in dfs:
-        instrument = df.attrs["INSTRUME"] + "_" + df.attrs["ANTENNAID"]
-        if instrument not in instruments:
-            instruments[instrument] = []
-        instruments[instrument].append(df)
-
-    if verbose:
-        print("Concatenating dataframes.")
-    for instrument, dfs in instruments.items():
-        headers = [df.attrs for df in dfs]
-        identical_headers = extract_identical_dicts(headers)
-        instruments[instrument] = pd.concat(dfs).sort_index()
-        instruments[instrument] = readd_edit_header(
-            instruments[instrument], identical_headers
-        )
-
-    return instruments
-
-
-def masked_spectogram_to_array(data, freq_axis):
-    """
-    Converts a masked spectogram to an array by removing all masked values.
-    """
-    # Get row with no masked values
-    idxs = np.where(~np.any(np.ma.getmaskarray(data), axis=1))[0]
-    # Keep only frequencies with no masked values
-    freq_axis = freq_axis[idxs]
-    # keep only rows in idxs
-    data = np.ma.getdata(data)
-    data = data[idxs, :]
-
-    return data, freq_axis
-
-
-def ecallisto_fits_to_pandas(fits_file):
-    """
-    Convert eCallisto FITS data to a pandas DataFrame.
-
-    Parameters
-    ----------
-    fits_file : astropy.io.fits.HDUList
-        An HDUList object representing the FITS file.
-
-    Returns
-    -------
-    pandas.DataFrame
-        A DataFrame containing the FITS data with time as index and frequencies as columns.
-
-    Notes
-    -----
-    This function processes eCallisto FITS files, extracting the time axis, frequency axis,
-    and data values. It handles non-unique frequencies by combining them and converts the
-    time axis to pandas datetime objects. FITS header information is added as attributes
-    to the DataFrame.
-
-    Non-unique frequency axes are combined using the `combine_non_unique_frequency_axis` function,
-    which is not defined in this snippet and should be provided separately.
-    """
-    time_axis = fits_file[1].data[0][0]
-    freq_axis = fits_file[1].data[0][1]
-    data = np.array(fits_file[0].data, dtype=np.uint8)
-
-    # Remove masked values
-    data, freq_axis = masked_spectogram_to_array(data, freq_axis)
-
-    if not len(np.unique(freq_axis)) == len(freq_axis):
-        freq_axis, data = combine_non_unique_frequency_axis(freq_axis, data)
-
-    start_datetime = pd.to_datetime(
-        fits_file[0].header["DATE-OBS"] + " " + fits_file[0].header["TIME-OBS"]
-    )
-    # Cast freq_axis to float to avoid issues with pandas
-    freq_axis = freq_axis.astype(float)
-
-    pd_time_axis = spec_time_to_pd_datetime(start_datetime, time_axis)
-    df = pd.DataFrame(data=data.T, index=pd_time_axis, columns=freq_axis)
-
-    # Sort columns, so that they are in ascending order
-    df = df.sort_index(axis=1)
-
-    # Add the header
-    for key, value in fits_file[0].header.items():
-        df.attrs[key] = value
-
-    # Make columns to floats and sort them
-    df.columns = df.columns.astype(float)
-    df = df.sort_index(axis=1)
-
-    return df
+import re
+import warnings
+from datetime import datetime
+
+import numpy as np
+import pandas as pd
+
+
+def filter_dataframes(
+    dfs, start_date, end_date, verbose=False, freq_start=None, freq_end=None
+):
+    """
+    Filter the dataframes in a dictionary by a date range.
+
+    Parameters
+    ----------
+    dfs : dict of str: `~pandas.DataFrame`
+        Dictionary of instrument names and their corresponding dataframes.
+    start_date : datetime-like
+        The start date for the filter.
+    end_date : datetime-like
+        The end date for the filter.
+    verbose : bool
+        Whether to print progress information.
+    freq_start : float or None
+        The start frequency for the filter.
+    freq_end : float or None
+        The end frequency for the filter.
+
+    Returns
+    -------
+    dict of str: `~pandas.DataFrame`
+        Dictionary of instrument names and their corresponding dataframes.
+    """
+    if verbose:
+        print("Filtering dataframes.")
+    for instrument, df in dfs.items():
+        dfs[instrument] = df.loc[start_date:end_date]
+
+    if verbose:
+        print("Filtering frequencies.")
+    if freq_start:
+        for instrument, df in dfs.items():
+            dfs[instrument] = df.loc[:, freq_start:freq_end]
+    if freq_end:
+        for instrument, df in dfs.items():
+            dfs[instrument] = df.loc[:, freq_start:freq_end]
+
+    # Check if any dfs are empty
+    empty_instruments = []
+    for instrument, df in dfs.items():
+        if df.empty:
+            empty_instruments.append(instrument)
+    for instrument in empty_instruments:
+        del dfs[instrument]
+
+    # Update the header
+    if verbose:
+        print("Updating headers after filtering.")
+    for instrument, df in dfs.items():
+        df = readd_edit_header(df, dfs[instrument].attrs)
+    return dfs
+
+
+def extract_datetime_from_filename(file_name):
+    """
+    Extract datetime from the filename.
+
+    Parameters
+    ----------
+    file_name : str
+        The filename from which to extract the datetime.
+
+    Returns
+    -------
+    datetime
+        The extracted datetime object, or None if parsing fails.
+    """
+    # Filename format: 'LOCATION_YYYYMMDD_HHMMSS_X.fit.gz'
+    match = re.search(r"_(\d{8})_(\d{6})", file_name)
+    if match:
+        return datetime.strptime(match.group(1) + match.group(2), "%Y%m%d%H%M%S")
+    return None
+
+
+def instrument_name_to_globbing_pattern(instrument_name=None):
+    """
+    Convert an instrument name (and optional antenna number) to a globbing pattern suitable for matching in file URLs.
+
+    Parameters
+    ----------
+    instrument_name : str
+        The instrument name to be matched in the file URLs.
+
+    Returns
+    -------
+    str
+        A matching pattern string.
+    """
+    if instrument_name is None:
+        return "*.fit.gz"
+    antenna_number = None
+    if instrument_name[-2:].isdigit():
+        antenna_number = instrument_name[-2:]
+        instrument_name = instrument_name[:-3]
+    glob_pattern = "*" + instrument_name + "*"
+    if antenna_number:
+        glob_pattern += antenna_number
+    glob_pattern += ".fit.gz"
+    return glob_pattern
+
+
+def combine_non_unique_frequency_axis(freq_axis, data, agg_function=np.max):
+    """Combine non-unique frequency axis data.
+
+    Parameters
+    ----------
+    spec : `~astropy.io.fits.hdu.hdulist.HDUList`
+        The spectrogram to combine the frequency axis data of.
+    method : callable
+        The method to use to combine the frequency axis data. Defaults to "mean".
+
+    Returns
+    -------
+    unique_freq_axis : `~numpy.ndarray`
+        The unique frequency axis data.
+    data : `~numpy.ndarray`
+        The combined data.
+
+
+    Notes
+    -----
+    The function first finds the unique frequency axis data and the indices of the non-unique frequency axis data.
+    It then combines the non-unique frequency axis data using the method specified by the `method` parameter.
+    """
+    unique_freq, indices = np.unique(freq_axis, return_inverse=True)
+    data = np.array(
+        [agg_function(data[indices == i], axis=0) for i in range(len(unique_freq))]
+    )
+    return unique_freq, data
+
+
+def spec_time_to_pd_datetime(start_datetime, time_axis):
+    """
+    Convert a time axis array to pandas datetime objects, offset by a starting datetime.
+
+    Parameters
+    ----------
+    start_datetime : datetime or Timestamp
+        The starting datetime to which the time axis offsets will be applied.
+    time_axis : array_like
+        An array of time offsets in seconds.
+
+    Returns
+    -------
+    pandas.Series
+        A pandas Series of datetime objects corresponding to each time offset.
+
+    Notes
+    -----
+    This function adds the given time offsets in seconds to the start datetime
+    and converts the result to pandas datetime objects.
+    """
+    return start_datetime + pd.to_timedelta(time_axis, unit="s")
+
+
+def extract_instrument_name(file_path):
+    """Extract the instrument name from a file path.
+
+    Parameters
+    ----------
+    file_path : str
+        The file path to extract the instrument name from.
+
+    Returns
+    -------
+    str
+        The extracted instrument name, converted to lowercase with underscores in place of hyphens.
+
+
+    Example
+    -------
+    >>> extract_instrument_name('/var/lib/ecallisto/2023/01/27/ALASKA-COHOE_20230127_001500_612.fit.gz')
+    'ALASKA_COHOE_612'
+
+    Notes
+    -----
+    The function first selects the last part of the file path and removes the extension.
+    Then, it replaces hyphens with underscores and splits on underscores to get the parts of the file name.
+    The function concatenates these parts, adding a numeric part of the file name if it is less than 6 digits.
+    """
+    # select last part of file path and remove extension
+    file_name = file_path.split("/")[-1].split(".")[0]
+
+    # Remove datetime
+    instrument_name = file_name.split("_")[0]
+    antenna_number = file_name.split("_")[-1]
+    return instrument_name + "_" + antenna_number
+
+
+def extract_identical_dicts(dicts):
+    """
+    Extract identical keys and values from a list of dictionaries.
+
+    Parameters
+    ----------
+    dicts : list of dict
+        The list of dictionaries to extract identical keys and values from.
+
+    Returns
+    -------
+    dict
+        A dictionary of identical keys and values.
+    """
+    identical_keys = set.intersection(*[set(d.keys()) for d in dicts])
+    identical_values = {}
+    for key in identical_keys:
+        values = [d[key] for d in dicts]
+        if len(set(values)) == 1:
+            identical_values[key] = values[0]
+    return identical_values
+
+
+def readd_edit_header(df, dict_):
+    """
+    Re-add and edit header information to a DataFrame.
+
+    This function updates the header of a DataFrame with new values and adds additional
+    time-related and instrument information. It preserves the order of the original header keys.
+
+    Parameters
+    ----------
+    df : pandas.DataFrame
+        DataFrame to which header information will be added or updated.
+    dict_ : dict
+        Dictionary containing header information to be updated or added to `df`.
+
+    Returns
+    -------
+    pandas.DataFrame
+        The DataFrame with updated header information.
+
+    Notes
+    -----
+    The function assumes that the DataFrame `df` has an attribute `header`, which is a dictionary
+    used to store header information. The DataFrame's index is used to derive `DATE-OBS`, `TIME-OBS`,
+    `DATE-END`, and `TIME-END` values.
+    """
+    for key, value in dict_.items():
+        df.attrs[key] = value
+    # Add DATE-OBS and TIME-OBS
+    df.attrs["DATE-OBS"] = df.index[0].strftime("%Y-%m-%d")
+    df.attrs["TIME-OBS"] = df.index[0].strftime("%H:%M:%S")
+    df.attrs["DATE-END"] = df.index[-1].strftime("%Y-%m-%d")
+    df.attrs["TIME-END"] = df.index[-1].strftime("%H:%M:%S")
+    df.attrs["NAXIS1"] = len(df)
+    df.attrs["FULLNAME"] = df.attrs["INSTRUME"] + "_" + df.attrs["ANTENNAID"]
+    return df
+
+
+def concat_dfs_by_instrument(dfs, verbose=False):
+    instruments = {}
+    # Extract attrs from each df
+    headers = [df.attrs for df in dfs]
+    if verbose:
+        print("Combining headers.")
+    for df in dfs:
+        instrument = df.attrs["INSTRUME"] + "_" + df.attrs["ANTENNAID"]
+        if instrument not in instruments:
+            instruments[instrument] = []
+        instruments[instrument].append(df)
+
+    if verbose:
+        print("Concatenating dataframes.")
+    for instrument, dfs in instruments.items():
+        headers = [df.attrs for df in dfs]
+        identical_headers = extract_identical_dicts(headers)
+        instruments[instrument] = pd.concat(dfs).sort_index()
+        instruments[instrument] = readd_edit_header(
+            instruments[instrument], identical_headers
+        )
+
+    return instruments
+
+
+def masked_spectogram_to_array(data, freq_axis):
+    """
+    Converts a masked spectogram to an array by removing all masked values.
+    """
+    # Get row with no masked values
+    idxs = np.where(~np.any(np.ma.getmaskarray(data), axis=1))[0]
+    # Keep only frequencies with no masked values
+    freq_axis = freq_axis[idxs]
+    # keep only rows in idxs
+    data = np.ma.getdata(data)
+    data = data[idxs, :]
+
+    return data, freq_axis
+
+
+def ecallisto_fits_to_pandas(fits_file):
+    """
+    Convert eCallisto FITS data to a pandas DataFrame.
+
+    Parameters
+    ----------
+    fits_file : astropy.io.fits.HDUList
+        An HDUList object representing the FITS file.
+
+    Returns
+    -------
+    pandas.DataFrame
+        A DataFrame containing the FITS data with time as index and frequencies as columns.
+
+    Notes
+    -----
+    This function processes eCallisto FITS files, extracting the time axis, frequency axis,
+    and data values. It handles non-unique frequencies by combining them and converts the
+    time axis to pandas datetime objects. FITS header information is added as attributes
+    to the DataFrame.
+
+    Non-unique frequency axes are combined using the `combine_non_unique_frequency_axis` function,
+    which is not defined in this snippet and should be provided separately.
+    """
+    time_axis = fits_file[1].data[0][0]
+    freq_axis = fits_file[1].data[0][1]
+    data = np.array(fits_file[0].data, dtype=np.uint8)
+
+    # Remove masked values
+    data, freq_axis = masked_spectogram_to_array(data, freq_axis)
+
+    if not len(np.unique(freq_axis)) == len(freq_axis):
+        freq_axis, data = combine_non_unique_frequency_axis(freq_axis, data)
+
+    start_datetime = pd.to_datetime(
+        fits_file[0].header["DATE-OBS"] + " " + fits_file[0].header["TIME-OBS"]
+    )
+    # Cast freq_axis to float to avoid issues with pandas
+    freq_axis = freq_axis.astype(float)
+
+    pd_time_axis = spec_time_to_pd_datetime(start_datetime, time_axis)
+    df = pd.DataFrame(data=data.T, index=pd_time_axis, columns=freq_axis)
+
+    # Sort columns, so that they are in ascending order
+    df = df.sort_index(axis=1)
+
+    # Add the header
+    for key, value in fits_file[0].header.items():
+        df.attrs[key] = value
+
+    # Make columns to floats and sort them
+    df.columns = df.columns.astype(float)
+    df = df.sort_index(axis=1)
+
+    return df
```

### Comparing `ecallisto_ng-0.7.11/src/ecallisto_ng/data_fetching/get_data.py` & `ecallisto_ng-0.7.12/src/ecallisto_ng/data_fetching/get_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,269 +1,270 @@
-import json
-import os
-import time
-import warnings
-
-import pandas as pd
-import requests
-
-from ecallisto_ng.data_fetching.get_information import check_table_data_availability
-
-# Import exceptions
-
-
-BASE_URL = "https://v000792.fhnw.ch"
-DATA_FOLDER = "ecallisto_ng_cache"
-
-
-class NoDataAvailable(Exception):
-    def __init__(self, data):
-        super().__init__(f"No data available for {data}")
-
-
-def get_data(
-    instrument_name,
-    start_datetime,
-    end_datetime,
-    timebucket=None,
-    agg_function=None,
-    data_folder=DATA_FOLDER,
-    verbose=False,
-    max_retries=3,
-):
-    """
-    Get data from the eCallisto API. See: https://v000792.fhnw.ch/api/redoc
-    Of course, this is just a wrapper around the requests.post function.
-    Depending on the size, the request can take a while. For example, two
-    weeks of data, aggregated in a specific way, can take around 20 seconds.
-
-    Parameters
-    ----------
-    instrument_name : str
-        The name of the instrument to get data from.
-    start_datetime : str
-        The start datetime of the data to get.
-    end_datetime : str
-        The end datetime of the data to get.
-    timebucket : str
-        In what time frame the data should be grouped (see timescaledb
-        "timebucket" function)
-    agg_function : str
-        The aggregation function to use (see timescaledb "timebucket" function)
-    data_folder : str
-        Where to save the cached data.
-    verbose : bool
-        Whether to print the progress or not.
-    max_retries : int
-        The maximum number of retries to download the data.
-    Returns
-    -------
-    pandas.DataFrame
-        A DataFrame containing the data from the eCallisto API.
-    """
-    warnings.warn(
-        DeprecationWarning(
-            "get_data is deprecated and will be removed in the future. See Readme for more information."
-        )
-    )
-    data = {
-        "instrument_name": instrument_name,
-        "start_datetime": start_datetime,
-        "end_datetime": end_datetime,
-        "timebucket": timebucket,
-        "agg_function": agg_function,
-    }
-
-    assert pd.to_datetime(start_datetime) <= pd.to_datetime(
-        end_datetime
-    ), f"start_datetime ({start_datetime}) must be before end_datetime ({end_datetime})"
-
-    # Clean up dates to make it compatible with windows
-    start_datetime = start_datetime.replace(":", "-")
-    end_datetime = end_datetime.replace(":", "-")
-
-    # Create file path
-    file_path = os.path.join(
-        data_folder,
-        f"{instrument_name}_{start_datetime}_{end_datetime}_{timebucket}_{agg_function}.parquet",
-    )
-    os.makedirs(data_folder, exist_ok=True)
-    if os.path.exists(file_path):
-        print(f"Reading data from {file_path}")
-        return read_parquet_and_meta_data(file_path)
-
-    if not check_table_data_availability(**data):
-        raise NoDataAvailable(data)
-
-    # Send the request to the API
-    response = requests.post(BASE_URL + "/api/data", json=data, timeout=180)
-    # Check if the request was successful
-    if response.status_code == 200:
-        if verbose:
-            print(
-                "Data retrieval started successfully. Waiting for file to be ready..."
-            )
-        # Get the URL for the parquet file
-        parquet_url = response.json()["data_parquet_url"]
-        json_url = response.json()["info_json_url"]
-        file_id = response.json()["file_id"]
-        meta_data_url = response.json()["meta_data_url"]
-
-        # Now we can start polling the URL until the parquet file is ready for download
-        n_tries = 1
-        while True:
-            try:
-                if verbose:
-                    print(f"Trying to download file {file_id}")
-                # Try to download the parquet file
-                file_response = requests.get(BASE_URL + parquet_url)
-                # If the file is available, save it to disk
-                if file_response.status_code == 200:
-                    print("File downloaded successfully")
-                    with open(file_path, "wb") as f:
-                        f.write(file_response.content)
-                    # Download the meta data
-                    meta_data_response = requests.get(BASE_URL + meta_data_url)
-                    with open(file_path.replace(".parquet", ".json"), "w") as f:
-                        f.write(meta_data_response.text)
-                    # Check that the file is bigger than 8 bytes (sometimes, the API returns an empty file)
-                    if os.path.getsize(file_path) > 8:
-                        return read_parquet_and_meta_data(file_path)
-                    else:
-                        # Remove file and try again
-                        os.remove(file_path)
-                        raise ValueError(
-                            f"Error downloading file: {file_response.status_code}. File is empty."
-                        )
-                elif file_response.status_code == 204:
-                    # Check if the file creation causes any errors
-                    json_response = requests.get(
-                        BASE_URL + json_url
-                    )  # This json contains information about your data request (e.g. status)
-                    # Check the status of the json
-                    if "status" in json_response.json():
-                        if json_response.json()["status"] == "processing":
-                            # If the file is not found, sleep for a short period and try again
-                            if verbose:
-                                print(f"File {file_id} not ready yet, waiting...")
-                            time.sleep(3)
-                        elif json_response.json()["status"] == "ok":
-                            if verbose:
-                                print(
-                                    f"File {file_id} succesfully written! Will return file."
-                                )
-                        else:
-                            raise ValueError(
-                                f"Error downloading file: {json_response.json()['status']}"
-                            )
-                    elif "error" in json_response.json():
-                        raise ValueError(
-                            f"Error downloading file: {json_response.json()['error']}"
-                        )
-                else:
-                    print(f"Error downloading file: {file_response.status_code}")
-                    json_response = requests.get(BASE_URL + json_url)
-                    print(json_response.json())
-                    break
-            except Exception as e:
-                print(
-                    f"""Error downloading file: {e}. Try {n_tries} of {max_retries}. Retrying in 3 seconds...
-                    """
-                )
-                n_tries += 1
-                if n_tries > max_retries:
-                    raise ValueError(
-                        f"Error downloading file: {file_response.status_code}. Max retries reached."
-                    )
-                time.sleep(3)
-    else:
-        print(f"Error starting data retrieval: {response.status_code}")
-
-
-def read_parquet_and_meta_data(file_path):
-    meta_data_path = file_path.replace(".parquet", ".json")
-    df = pd.read_parquet(file_path)
-    with open(meta_data_path, "r") as f:
-        meta_data = json.load(f)
-    for key, value in meta_data.items():
-        df.attrs[key] = value
-    return df
-
-
-# Because of SQL limitation, the names of the tables do not perfectly match the instrument names.
-# This function converts the instrument name to the table name.
-def extract_instrument_name(file_path):
-    """
-    Because of SQL limitation, the names of the tables do not perfectly match the instrument names.
-    This function converts the instrument name to the table name.
-
-    Parameters
-    ----------
-    file_path : str
-        The file path to extract the instrument name from.
-
-    Returns
-    -------
-    str
-        The extracted instrument name, converted to lowercase with underscores in place of hyphens.
-
-    Example
-    -------
-    >>> extract_instrument_name('/var/lib/ecallisto/2023/01/27/ALASKA-COHOE_20230127_001500_612.fit.gz')
-    'alaska_cohoe_612'
-
-    Notes
-    -----
-    The function first selects the last part of the file path and removes the extension.
-    Then, it replaces hyphens with underscores and splits on underscores to get the parts of the file name.
-    The function concatenates these parts, adding a numeric part of the file name if it is less than 6 digits.
-    """
-    # select last part of path and remove extension
-    file_name_parts = os.path.basename(file_path).split(".")[0]
-    # replace '-' with '_' and split on '_' to get the parts of the file name
-    file_name_parts = file_name_parts.replace("-", "_").lower().split("_")
-    file_name = ""
-    for part in file_name_parts:
-        if not part.isnumeric():
-            file_name += "_" + part
-    if (
-        len(file_name_parts[-1]) < 6 and file_name_parts[-1].isnumeric()
-    ):  # Sometimes, the last part is an ID number for when the station has multiple instruments.
-        # We want to add this to the file name if it's not a time (6 digits).
-        file_name = file_name + "_" + file_name_parts[-1]
-
-    return file_name[1:]  # Remove the first '-'
-
-
-def reverse_extract_instrument_name(instrument_name, include_number=False):
-    """
-    Because of SQL limitation, the names of the tables do not perfectly match the instrument names.
-    Convert a lower-case instrument name with underscores to its original hyphenated form.
-
-    Parameters
-    ----------
-    instrument_name : str
-        The instrument name in lower-case with underscores.
-    include_number : bool, optional
-        Whether to include the last number in the output or not. Default is False.
-
-    Returns
-    -------
-    str
-        The original instrument name with hyphens.
-
-    Example
-    -------
-    >>> reverse_extract_instrument_name('alaska_cohoe_612')
-    'ALASKA-COHOE'
-    >>> reverse_extract_instrument_name('alaska_cohoe_612', include_number=True)
-    'ALASKA-COHOE_612'
-
-    """
-    # Replace underscores with hyphens and upper all the letters
-    parts = [part.upper() for part in instrument_name.split("_")]
-    if not include_number:
-        # Remove the last part if it's a number
-        if parts[-1].isnumeric():
-            parts.pop()
-    # Join the parts with hyphens and return the result
-    return "-".join(parts)
+import json
+import os
+import time
+import warnings
+
+import pandas as pd
+import requests
+
+from ecallisto_ng.data_fetching.get_information import \
+    check_table_data_availability
+
+# Import exceptions
+
+
+BASE_URL = "https://v000792.fhnw.ch"
+DATA_FOLDER = "ecallisto_ng_cache"
+
+
+class NoDataAvailable(Exception):
+    def __init__(self, data):
+        super().__init__(f"No data available for {data}")
+
+
+def get_data(
+    instrument_name,
+    start_datetime,
+    end_datetime,
+    timebucket=None,
+    agg_function=None,
+    data_folder=DATA_FOLDER,
+    verbose=False,
+    max_retries=3,
+):
+    """
+    Get data from the eCallisto API. See: https://v000792.fhnw.ch/api/redoc
+    Of course, this is just a wrapper around the requests.post function.
+    Depending on the size, the request can take a while. For example, two
+    weeks of data, aggregated in a specific way, can take around 20 seconds.
+
+    Parameters
+    ----------
+    instrument_name : str
+        The name of the instrument to get data from.
+    start_datetime : str
+        The start datetime of the data to get.
+    end_datetime : str
+        The end datetime of the data to get.
+    timebucket : str
+        In what time frame the data should be grouped (see timescaledb
+        "timebucket" function)
+    agg_function : str
+        The aggregation function to use (see timescaledb "timebucket" function)
+    data_folder : str
+        Where to save the cached data.
+    verbose : bool
+        Whether to print the progress or not.
+    max_retries : int
+        The maximum number of retries to download the data.
+    Returns
+    -------
+    pandas.DataFrame
+        A DataFrame containing the data from the eCallisto API.
+    """
+    warnings.warn(
+        DeprecationWarning(
+            "get_data is deprecated and will be removed in the future. See Readme for more information."
+        )
+    )
+    data = {
+        "instrument_name": instrument_name,
+        "start_datetime": start_datetime,
+        "end_datetime": end_datetime,
+        "timebucket": timebucket,
+        "agg_function": agg_function,
+    }
+
+    assert pd.to_datetime(start_datetime) <= pd.to_datetime(
+        end_datetime
+    ), f"start_datetime ({start_datetime}) must be before end_datetime ({end_datetime})"
+
+    # Clean up dates to make it compatible with windows
+    start_datetime = start_datetime.replace(":", "-")
+    end_datetime = end_datetime.replace(":", "-")
+
+    # Create file path
+    file_path = os.path.join(
+        data_folder,
+        f"{instrument_name}_{start_datetime}_{end_datetime}_{timebucket}_{agg_function}.parquet",
+    )
+    os.makedirs(data_folder, exist_ok=True)
+    if os.path.exists(file_path):
+        print(f"Reading data from {file_path}")
+        return read_parquet_and_meta_data(file_path)
+
+    if not check_table_data_availability(**data):
+        raise NoDataAvailable(data)
+
+    # Send the request to the API
+    response = requests.post(BASE_URL + "/api/data", json=data, timeout=180)
+    # Check if the request was successful
+    if response.status_code == 200:
+        if verbose:
+            print(
+                "Data retrieval started successfully. Waiting for file to be ready..."
+            )
+        # Get the URL for the parquet file
+        parquet_url = response.json()["data_parquet_url"]
+        json_url = response.json()["info_json_url"]
+        file_id = response.json()["file_id"]
+        meta_data_url = response.json()["meta_data_url"]
+
+        # Now we can start polling the URL until the parquet file is ready for download
+        n_tries = 1
+        while True:
+            try:
+                if verbose:
+                    print(f"Trying to download file {file_id}")
+                # Try to download the parquet file
+                file_response = requests.get(BASE_URL + parquet_url)
+                # If the file is available, save it to disk
+                if file_response.status_code == 200:
+                    print("File downloaded successfully")
+                    with open(file_path, "wb") as f:
+                        f.write(file_response.content)
+                    # Download the meta data
+                    meta_data_response = requests.get(BASE_URL + meta_data_url)
+                    with open(file_path.replace(".parquet", ".json"), "w") as f:
+                        f.write(meta_data_response.text)
+                    # Check that the file is bigger than 8 bytes (sometimes, the API returns an empty file)
+                    if os.path.getsize(file_path) > 8:
+                        return read_parquet_and_meta_data(file_path)
+                    else:
+                        # Remove file and try again
+                        os.remove(file_path)
+                        raise ValueError(
+                            f"Error downloading file: {file_response.status_code}. File is empty."
+                        )
+                elif file_response.status_code == 204:
+                    # Check if the file creation causes any errors
+                    json_response = requests.get(
+                        BASE_URL + json_url
+                    )  # This json contains information about your data request (e.g. status)
+                    # Check the status of the json
+                    if "status" in json_response.json():
+                        if json_response.json()["status"] == "processing":
+                            # If the file is not found, sleep for a short period and try again
+                            if verbose:
+                                print(f"File {file_id} not ready yet, waiting...")
+                            time.sleep(3)
+                        elif json_response.json()["status"] == "ok":
+                            if verbose:
+                                print(
+                                    f"File {file_id} succesfully written! Will return file."
+                                )
+                        else:
+                            raise ValueError(
+                                f"Error downloading file: {json_response.json()['status']}"
+                            )
+                    elif "error" in json_response.json():
+                        raise ValueError(
+                            f"Error downloading file: {json_response.json()['error']}"
+                        )
+                else:
+                    print(f"Error downloading file: {file_response.status_code}")
+                    json_response = requests.get(BASE_URL + json_url)
+                    print(json_response.json())
+                    break
+            except Exception as e:
+                print(
+                    f"""Error downloading file: {e}. Try {n_tries} of {max_retries}. Retrying in 3 seconds...
+                    """
+                )
+                n_tries += 1
+                if n_tries > max_retries:
+                    raise ValueError(
+                        f"Error downloading file: {file_response.status_code}. Max retries reached."
+                    )
+                time.sleep(3)
+    else:
+        print(f"Error starting data retrieval: {response.status_code}")
+
+
+def read_parquet_and_meta_data(file_path):
+    meta_data_path = file_path.replace(".parquet", ".json")
+    df = pd.read_parquet(file_path)
+    with open(meta_data_path, "r") as f:
+        meta_data = json.load(f)
+    for key, value in meta_data.items():
+        df.attrs[key] = value
+    return df
+
+
+# Because of SQL limitation, the names of the tables do not perfectly match the instrument names.
+# This function converts the instrument name to the table name.
+def extract_instrument_name(file_path):
+    """
+    Because of SQL limitation, the names of the tables do not perfectly match the instrument names.
+    This function converts the instrument name to the table name.
+
+    Parameters
+    ----------
+    file_path : str
+        The file path to extract the instrument name from.
+
+    Returns
+    -------
+    str
+        The extracted instrument name, converted to lowercase with underscores in place of hyphens.
+
+    Example
+    -------
+    >>> extract_instrument_name('/var/lib/ecallisto/2023/01/27/ALASKA-COHOE_20230127_001500_612.fit.gz')
+    'alaska_cohoe_612'
+
+    Notes
+    -----
+    The function first selects the last part of the file path and removes the extension.
+    Then, it replaces hyphens with underscores and splits on underscores to get the parts of the file name.
+    The function concatenates these parts, adding a numeric part of the file name if it is less than 6 digits.
+    """
+    # select last part of path and remove extension
+    file_name_parts = os.path.basename(file_path).split(".")[0]
+    # replace '-' with '_' and split on '_' to get the parts of the file name
+    file_name_parts = file_name_parts.replace("-", "_").lower().split("_")
+    file_name = ""
+    for part in file_name_parts:
+        if not part.isnumeric():
+            file_name += "_" + part
+    if (
+        len(file_name_parts[-1]) < 6 and file_name_parts[-1].isnumeric()
+    ):  # Sometimes, the last part is an ID number for when the station has multiple instruments.
+        # We want to add this to the file name if it's not a time (6 digits).
+        file_name = file_name + "_" + file_name_parts[-1]
+
+    return file_name[1:]  # Remove the first '-'
+
+
+def reverse_extract_instrument_name(instrument_name, include_number=False):
+    """
+    Because of SQL limitation, the names of the tables do not perfectly match the instrument names.
+    Convert a lower-case instrument name with underscores to its original hyphenated form.
+
+    Parameters
+    ----------
+    instrument_name : str
+        The instrument name in lower-case with underscores.
+    include_number : bool, optional
+        Whether to include the last number in the output or not. Default is False.
+
+    Returns
+    -------
+    str
+        The original instrument name with hyphens.
+
+    Example
+    -------
+    >>> reverse_extract_instrument_name('alaska_cohoe_612')
+    'ALASKA-COHOE'
+    >>> reverse_extract_instrument_name('alaska_cohoe_612', include_number=True)
+    'ALASKA-COHOE_612'
+
+    """
+    # Replace underscores with hyphens and upper all the letters
+    parts = [part.upper() for part in instrument_name.split("_")]
+    if not include_number:
+        # Remove the last part if it's a number
+        if parts[-1].isnumeric():
+            parts.pop()
+    # Join the parts with hyphens and return the result
+    return "-".join(parts)
```

### Comparing `ecallisto_ng-0.7.11/src/ecallisto_ng/data_fetching/get_information.py` & `ecallisto_ng-0.7.12/src/ecallisto_ng/data_fetching/get_information.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,153 +1,153 @@
-import pandas as pd
-import requests
-
-BASE_URL = "https://v000792.fhnw.ch"
-
-
-def get_tables(verbose=False):
-    """
-    Fetch all the available table names from the eCallisto API.
-
-    Parameters
-    ----------
-    verbose : bool
-        Whether to print out the response from the API.
-
-    Returns
-    -------
-    list of str
-        A list containing the names of the available tables.
-    """
-    response = requests.get(BASE_URL + "/api/tables")
-
-    if response.status_code == 200:
-        table_names = response.json()["tables"]
-        if verbose:
-            print(f"Received table names: {table_names}")
-        return table_names
-    else:
-        raise ValueError(f"Error getting table names from API: {response.text}")
-
-
-def get_table_names_with_data_between_dates(
-    start_datetime, end_datetime, verbose=False
-):
-    """
-    Fetch all the available table names that contain data between the specified dates from the eCallisto API.
-
-    Parameters
-    ----------
-    start_datetime : str
-        The start datetime of the data availability check.
-    end_datetime : str
-        The end datetime of the data availability check.
-    verbose : bool
-        Whether to print out the response from the API.
-
-    Returns
-    -------
-    list of str
-        A list containing the names of the available tables that contain data between the specified dates.
-    """
-    data = {
-        "start_datetime": start_datetime,
-        "end_datetime": end_datetime,
-    }
-
-    assert pd.to_datetime(start_datetime) <= pd.to_datetime(
-        end_datetime
-    ), f"start_datetime ({start_datetime}) must be before end_datetime ({end_datetime})"
-
-    response = requests.post(BASE_URL + "/api/data_availability", json=data)
-
-    if response.status_code == 200:
-        table_names = response.json()["table_names"]
-        if verbose:
-            print(f"Received table names: {table_names}")
-        return table_names
-    else:
-        raise ValueError(f"Error getting table names from API: {response.text}")
-
-
-def check_min_max_datetime_in_table(instrument_name, verbose=False, **kwargs):
-    """
-    Check the minimum and maximum datetimes in a table using the eCallisto API.
-
-    Parameters
-    ----------
-    instrument_name : str
-        The name of the table to check.
-    verbose : bool
-        Whether to print out the response from the API.
-
-    Returns
-    -------
-    dict
-        A dictionary containing 'min_datetime' and 'max_datetime' if successful,
-        raises ValueError otherwise.
-    """
-    data = {"instrument_name": instrument_name}
-
-    response = requests.post(BASE_URL + "/api/min_max_datetime", json=data)
-
-    if response.status_code == 200:
-        min_max_datetime = response.json()
-        # To pd.Datetime
-        min_datetime, max_datetime = (
-            pd.to_datetime(min_max_datetime["min_datetime"]),
-            pd.to_datetime(min_max_datetime["max_datetime"]),
-        )
-        if verbose:
-            print(
-                f"Table '{instrument_name}' has minimum datetime at {min_datetime} and maximum datetime at {max_datetime}"
-            )
-        return min_datetime, max_datetime
-    else:
-        raise ValueError(f"Error checking min/max datetime from API: {response.text}")
-
-
-def check_table_data_availability(
-    instrument_name, start_datetime, end_datetime, verbose=False, **kwargs
-):
-    """
-    Check if a table has data between the specified dates using the eCallisto API.
-
-    Parameters
-    ----------
-    instrument_name : str
-        The name of the table to check.
-    start_datetime : str
-        The start datetime of the data availability check.
-    end_datetime : str
-        The end datetime of the data availability check.
-    verbose : bool
-        Whether to print out the response from the API.
-
-    Returns
-    -------
-    bool
-        True if the table has data between the specified dates, False otherwise.
-    """
-    data = {
-        "instrument_name": instrument_name,
-        "start_datetime": start_datetime,
-        "end_datetime": end_datetime,
-    }
-
-    assert pd.to_datetime(start_datetime) <= pd.to_datetime(
-        end_datetime
-    ), f"start_datetime ({start_datetime}) must be before end_datetime ({end_datetime})"
-
-    response = requests.post(BASE_URL + "/api/table_data_check", json=data)
-
-    if response.status_code == 200:
-        has_data = response.json()["has_data"]
-        if verbose:
-            print(
-                f"Table '{instrument_name}' has data between {start_datetime} and {end_datetime}: {has_data}"
-            )
-        return has_data
-    else:
-        raise ValueError(
-            f"Error checking table data availability from API: {response.text}"
-        )
+import pandas as pd
+import requests
+
+BASE_URL = "https://v000792.fhnw.ch"
+
+
+def get_tables(verbose=False):
+    """
+    Fetch all the available table names from the eCallisto API.
+
+    Parameters
+    ----------
+    verbose : bool
+        Whether to print out the response from the API.
+
+    Returns
+    -------
+    list of str
+        A list containing the names of the available tables.
+    """
+    response = requests.get(BASE_URL + "/api/tables")
+
+    if response.status_code == 200:
+        table_names = response.json()["tables"]
+        if verbose:
+            print(f"Received table names: {table_names}")
+        return table_names
+    else:
+        raise ValueError(f"Error getting table names from API: {response.text}")
+
+
+def get_table_names_with_data_between_dates(
+    start_datetime, end_datetime, verbose=False
+):
+    """
+    Fetch all the available table names that contain data between the specified dates from the eCallisto API.
+
+    Parameters
+    ----------
+    start_datetime : str
+        The start datetime of the data availability check.
+    end_datetime : str
+        The end datetime of the data availability check.
+    verbose : bool
+        Whether to print out the response from the API.
+
+    Returns
+    -------
+    list of str
+        A list containing the names of the available tables that contain data between the specified dates.
+    """
+    data = {
+        "start_datetime": start_datetime,
+        "end_datetime": end_datetime,
+    }
+
+    assert pd.to_datetime(start_datetime) <= pd.to_datetime(
+        end_datetime
+    ), f"start_datetime ({start_datetime}) must be before end_datetime ({end_datetime})"
+
+    response = requests.post(BASE_URL + "/api/data_availability", json=data)
+
+    if response.status_code == 200:
+        table_names = response.json()["table_names"]
+        if verbose:
+            print(f"Received table names: {table_names}")
+        return table_names
+    else:
+        raise ValueError(f"Error getting table names from API: {response.text}")
+
+
+def check_min_max_datetime_in_table(instrument_name, verbose=False, **kwargs):
+    """
+    Check the minimum and maximum datetimes in a table using the eCallisto API.
+
+    Parameters
+    ----------
+    instrument_name : str
+        The name of the table to check.
+    verbose : bool
+        Whether to print out the response from the API.
+
+    Returns
+    -------
+    dict
+        A dictionary containing 'min_datetime' and 'max_datetime' if successful,
+        raises ValueError otherwise.
+    """
+    data = {"instrument_name": instrument_name}
+
+    response = requests.post(BASE_URL + "/api/min_max_datetime", json=data)
+
+    if response.status_code == 200:
+        min_max_datetime = response.json()
+        # To pd.Datetime
+        min_datetime, max_datetime = (
+            pd.to_datetime(min_max_datetime["min_datetime"]),
+            pd.to_datetime(min_max_datetime["max_datetime"]),
+        )
+        if verbose:
+            print(
+                f"Table '{instrument_name}' has minimum datetime at {min_datetime} and maximum datetime at {max_datetime}"
+            )
+        return min_datetime, max_datetime
+    else:
+        raise ValueError(f"Error checking min/max datetime from API: {response.text}")
+
+
+def check_table_data_availability(
+    instrument_name, start_datetime, end_datetime, verbose=False, **kwargs
+):
+    """
+    Check if a table has data between the specified dates using the eCallisto API.
+
+    Parameters
+    ----------
+    instrument_name : str
+        The name of the table to check.
+    start_datetime : str
+        The start datetime of the data availability check.
+    end_datetime : str
+        The end datetime of the data availability check.
+    verbose : bool
+        Whether to print out the response from the API.
+
+    Returns
+    -------
+    bool
+        True if the table has data between the specified dates, False otherwise.
+    """
+    data = {
+        "instrument_name": instrument_name,
+        "start_datetime": start_datetime,
+        "end_datetime": end_datetime,
+    }
+
+    assert pd.to_datetime(start_datetime) <= pd.to_datetime(
+        end_datetime
+    ), f"start_datetime ({start_datetime}) must be before end_datetime ({end_datetime})"
+
+    response = requests.post(BASE_URL + "/api/table_data_check", json=data)
+
+    if response.status_code == 200:
+        has_data = response.json()["has_data"]
+        if verbose:
+            print(
+                f"Table '{instrument_name}' has data between {start_datetime} and {end_datetime}: {has_data}"
+            )
+        return has_data
+    else:
+        raise ValueError(
+            f"Error checking table data availability from API: {response.text}"
+        )
```

### Comparing `ecallisto_ng-0.7.11/src/ecallisto_ng/data_processing/utils.py` & `ecallisto_ng-0.7.12/src/ecallisto_ng/data_processing/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,292 +1,312 @@
-import numpy as np
-import pandas as pd
-import scipy.signal
-from scipy.ndimage import median_filter
-from skimage import filters
-
-
-def mean_filter(df, kernel_size=(5, 5)):
-    """
-    Apply mean filter to a DataFrame using a 2D convolution.
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        Input DataFrame to filter.
-    kernel_size : tuple of int, optional
-        Dimensions of the filter kernel. Default is (5, 5).
-
-    Returns
-    -------
-    pd.DataFrame
-        Filtered DataFrame.
-    """
-    kernel = np.ones(kernel_size) / (kernel_size[0] * kernel_size[1])
-    data = scipy.signal.convolve2d(df.to_numpy(), kernel, "same")
-    df.values[:] = data
-    return df
-
-
-def apply_median_filter(df, size=(3, 3)):
-    """
-    Apply median filter to a DataFrame.
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        Input DataFrame to filter.
-    size : tuple of int, optional
-        Dimensions of the filter kernel. Default is (3, 3).
-
-    Returns
-    -------
-    pd.DataFrame
-        Filtered DataFrame.
-    """
-    data = median_filter(df.values, size)
-    df.values[:] = data
-    return df
-
-
-def return_strftime_based_on_range(time_range):
-    # Decide on the date-time format based on the time range
-    if time_range < pd.Timedelta(days=1):
-        date_format = "%H:%M:%S"
-    elif time_range < pd.Timedelta(weeks=4):
-        date_format = "%Y-%m-%d %H:%M"
-    else:
-        date_format = "%Y-%m-%d"
-
-    return date_format
-
-
-def elimwrongchannels(
-    df,
-    channel_std_mult=5,
-    jump_std_mult=2,
-    nan_interpolation_method="pchip",
-    interpolate_created_nans=True,
-    verbose=False,
-):
-    """
-    Remove Radio Frequency Interference (RFI) from a spectrogram represented by a pandas DataFrame.
-    This function works even when there is missing data thanks to interpolation of missing values.
-    However, it could lead to some false or different results.
-    Parameters
-    ----------
-    df : pandas.DataFrame
-        Input DataFrame where the index represents time and the columns represent frequency channels.
-    channel_std_mult : float, optional
-        Multiplicative factor for the standard deviation threshold used in the first RFI elimination step.
-        Channels with standard deviation less than this threshold times the mean standard deviation across all channels are retained.
-        Default is 5.
-    jump_std_mult : float, optional
-        Multiplicative factor for the standard deviation threshold used in the second RFI elimination step which deals with sharp jumps between channels.
-        Channels with the absolute difference from the mean value less than this threshold times the standard deviation of differences are retained.
-        Default is 2.
-    nan_interpolation_method : str, optional
-        Interpolation method to use for missing values. See pandas.DataFrame.interpolate for more details.
-        Default is "pchip".
-    interpolate_created_nans : bool, optional
-        Whether to interpolate NaNs created by the first RFI elimination step.
-        Default is True.
-    verbose : bool, optional
-        Whether to print out the number of eliminated channels.
-
-    Returns
-    -------
-    pandas.DataFrame
-        DataFrame with RFI removed. The DataFrame is oriented in the same way as the input DataFrame (time on index and frequency on columns).
-
-    """
-    df = df.copy()
-
-    # Store original NaN positions
-    nan_positions = df.isna()
-
-    # Fill missing data with interpolation
-    df.interpolate(method=nan_interpolation_method, inplace=True)
-    df.bfill(inplace=True)  # for cases where NaNs are at the start of a series
-
-    # Transpose df so that rows represent channels and columns represent time
-    df = df.T
-
-    # Calculate standard deviation for each channel and scale it to 0-255
-    std = df.std(axis=1).fillna(0)
-    std = ((std - std.min()) * 255) / (std.max() - std.min())
-    std = std.clip(upper=255).astype(int)
-
-    mean_sigma = std.mean()
-    positions = std < channel_std_mult * mean_sigma
-    eliminated_channels = (~positions).sum()
-    if verbose:
-        print(f"{eliminated_channels} channels eliminated")
-
-    if np.sum(positions) > 0:
-        # Replace the line with nans
-        df.iloc[~positions, :] = np.nan
-
-    if interpolate_created_nans:
-        # Interpolate the nans
-        df = df.interpolate(axis=0, limit_direction="both")
-
-    if verbose:
-        print("Eliminating sharp jumps between channels ...")
-    y_profile = np.average(filters.roberts(df.values.astype(float)), axis=1)
-    y_profile = pd.Series(y_profile - y_profile.mean(), index=df.index)
-    mean_sigma = y_profile.std()
-
-    positions = np.abs(y_profile) < jump_std_mult * mean_sigma
-    eliminated_channels = (~positions).sum()
-    if verbose:
-        print(f"{eliminated_channels} channels eliminated")
-
-    if np.sum(positions) > 0:
-        # Replace the line with nans
-        df.iloc[~positions, :] = np.nan
-    else:
-        if verbose:
-            print("Sorry, all channels are bad ...")
-        df = pd.DataFrame()
-    if interpolate_created_nans:
-        # Interpolate the nans
-        df = df.interpolate(axis=0, limit_direction="both")
-    # Transpose df back to original orientation
-    df = df.T
-
-    # Drop nans
-    df.dropna(inplace=True)
-
-    # Bring back original NaN values
-    df[nan_positions] = np.nan
-
-    return df
-
-
-def subtract_constant_background(df, n=300):
-    """
-    Subtract a constant background from a spectrogram represented by a pandas DataFrame.
-
-    The constant background is defined as the median value of the first n rows (timepoints) of the DataFrame.
-
-    Parameters
-    ----------
-    df : pandas.DataFrame
-        Input DataFrame where the index represents time and the columns represent frequency channels.
-    n : int
-        Number of first rows from which the median value is calculated to define the constant background.
-
-    Returns
-    -------
-    pandas.DataFrame
-        DataFrame with the constant background subtracted. The DataFrame is oriented in the same way as the input DataFrame (time on index and frequency on columns).
-
-    """
-    df = df.copy()
-    return df - df.iloc[0:n].median()
-
-
-def subtract_rolling_background(
-    df, window=30, center=False, how="quantile", quantile_value=0.05, **kwargs
-):
-    """
-    Subtract a rolling background from a spectrogram represented by a pandas DataFrame.
-
-    The rolling background is calculated either as the median or a specific quantile value of each rolling window of size `window`.
-
-    Parameters
-    ----------
-    df : pandas.DataFrame
-        Input DataFrame where the index represents time and the columns represent frequency channels.
-    window : int, default 30
-        Size of the rolling window from which the background value is calculated.
-    center : bool, default False
-        If True, the rolling window is centered on the current timepoint. If False, the rolling window starts at the current timepoint.
-        See pandas.DataFrame.rolling for more details.
-    how : str, default "median"
-        Method to calculate the rolling background. If "median", the median value of the window is used.
-        If "quantile", the quantile defined by `quantile_value` is used.
-    quantile_value : float, default 0.5
-        The quantile value to use when `how` is "quantile". Ignored if `how` is not "quantile".
-    **kwargs : dict
-        Additional keyword arguments passed to pandas.DataFrame.rolling.
-
-    Returns
-    -------
-    pandas.DataFrame
-        DataFrame with the rolling background subtracted. The DataFrame is oriented in the same way as the input DataFrame (time on index and frequency on columns).
-
-    """
-    df = df.copy()
-    if how == "median":
-        df_rolling = df.rolling(window=window, center=center, **kwargs).median()
-    elif how == "quantile":
-        df_rolling = df.rolling(window=window, center=center, **kwargs).quantile(
-            quantile_value
-        )
-    else:
-        raise ValueError("`how` must be 'median' or 'quantile'")
-    return df - df_rolling
-
-
-def subtract_low_signal_noise_background(df, percentile=0.05):
-    """
-    Background subtraction method adapted for DataFrame.
-    The average and the standard deviation of each row will be calculated and subtracted from the DataFrame.
-
-    Parameters
-    ----------
-    df : DataFrame
-        DataFrame representing the spectrogram with time as index and frequencies as columns.
-    percentile : float, default 0.05
-        Percentile of the lowest standard deviations to use as background.
-    """
-    df_ = df.copy()
-
-    # Subtract the average of each row (time point) from that row
-    row_averages = df_.mean(axis=1)
-    df_ = df_.sub(row_averages, axis=0)
-
-    # Calculate standard deviation for each column (frequency bin)
-    column_sdevs = df_.std(axis=1)
-
-    # Select columns (frequency bins) with the lowest standard deviations (assumed background)
-    n_columns = len(column_sdevs)
-    n_background = int(n_columns * percentile)
-    background_cols = column_sdevs.nsmallest(n_background).index
-    background = df_.loc[background_cols].mean()
-
-    # Subtract this background from each column of the DataFrame
-    return df - background
-
-
-def intensity_to_linear(df, factor=0.0386):
-    """
-    Convert Callisto values (W) and make them linear.
-    Based on the following forumla:
-    db = 10 ** (I * factor)
-
-    Parameters:
-    df (pd.DataFrame): DataFrame with Callisto values.
-    factor (float): Conversion factor in the formula.
-
-    Returns:
-    pd.DataFrame: DataFrame with converted intensity values.
-    """
-    return 10 ** (df * factor)
-
-
-def linear_to_intensity(df, factor=0.0386):
-    """
-    Convert db (I) back to Callisto values (W).
-    Based on the following forumla:
-    db = 10 ** (I * factor)
-
-    Parameters:
-    df (pd.DataFrame): DataFrame with intensity values.
-    factor (float): Conversion factor in the formula.
-
-    Returns:
-    pd.DataFrame: DataFrame with converted Callisto values.
-    """
-    return np.log10(df) / factor
+import numpy as np
+import pandas as pd
+import scipy.signal
+from scipy.ndimage import median_filter
+from skimage import filters
+
+
+def min_max_scale_per_column(data: pd.DataFrame) -> pd.DataFrame:
+    """
+    Apply min-max scaling to each column of a DataFrame.
+
+    Parameters:
+    data (pd.DataFrame): The input data with columns representing different frequencies.
+
+    Returns:
+    pd.DataFrame: The scaled data where each column is scaled independently.
+    """
+    # Ensuring the data is a DataFrame
+    if not isinstance(data, pd.DataFrame):
+        raise ValueError("Input must be a pandas DataFrame")
+
+    # Apply min-max scaling per column
+    scaled_data = (data - data.min()) / (data.max() - data.min())
+
+    return scaled_data
+
+
+def mean_filter(df, kernel_size=(5, 5)):
+    """
+    Apply mean filter to a DataFrame using a 2D convolution.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Input DataFrame to filter.
+    kernel_size : tuple of int, optional
+        Dimensions of the filter kernel. Default is (5, 5).
+
+    Returns
+    -------
+    pd.DataFrame
+        Filtered DataFrame.
+    """
+    kernel = np.ones(kernel_size) / (kernel_size[0] * kernel_size[1])
+    data = scipy.signal.convolve2d(df.to_numpy(), kernel, "same")
+    df.values[:] = data
+    return df
+
+
+def apply_median_filter(df, size=(3, 3)):
+    """
+    Apply median filter to a DataFrame.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Input DataFrame to filter.
+    size : tuple of int, optional
+        Dimensions of the filter kernel. Default is (3, 3).
+
+    Returns
+    -------
+    pd.DataFrame
+        Filtered DataFrame.
+    """
+    data = median_filter(df.values, size)
+    df.values[:] = data
+    return df
+
+
+def return_strftime_based_on_range(time_range):
+    # Decide on the date-time format based on the time range
+    if time_range < pd.Timedelta(days=1):
+        date_format = "%H:%M:%S"
+    elif time_range < pd.Timedelta(weeks=4):
+        date_format = "%Y-%m-%d %H:%M"
+    else:
+        date_format = "%Y-%m-%d"
+
+    return date_format
+
+
+def elimwrongchannels(
+    df,
+    channel_std_mult=5,
+    jump_std_mult=2,
+    nan_interpolation_method="pchip",
+    interpolate_created_nans=True,
+    verbose=False,
+):
+    """
+    Remove Radio Frequency Interference (RFI) from a spectrogram represented by a pandas DataFrame.
+    This function works even when there is missing data thanks to interpolation of missing values.
+    However, it could lead to some false or different results.
+    Parameters
+    ----------
+    df : pandas.DataFrame
+        Input DataFrame where the index represents time and the columns represent frequency channels.
+    channel_std_mult : float, optional
+        Multiplicative factor for the standard deviation threshold used in the first RFI elimination step.
+        Channels with standard deviation less than this threshold times the mean standard deviation across all channels are retained.
+        Default is 5.
+    jump_std_mult : float, optional
+        Multiplicative factor for the standard deviation threshold used in the second RFI elimination step which deals with sharp jumps between channels.
+        Channels with the absolute difference from the mean value less than this threshold times the standard deviation of differences are retained.
+        Default is 2.
+    nan_interpolation_method : str, optional
+        Interpolation method to use for missing values. See pandas.DataFrame.interpolate for more details.
+        Default is "pchip".
+    interpolate_created_nans : bool, optional
+        Whether to interpolate NaNs created by the first RFI elimination step.
+        Default is True.
+    verbose : bool, optional
+        Whether to print out the number of eliminated channels.
+
+    Returns
+    -------
+    pandas.DataFrame
+        DataFrame with RFI removed. The DataFrame is oriented in the same way as the input DataFrame (time on index and frequency on columns).
+
+    """
+    df = df.copy()
+
+    # Store original NaN positions
+    nan_positions = df.isna()
+
+    # Fill missing data with interpolation
+    df.interpolate(method=nan_interpolation_method, inplace=True)
+    df.bfill(inplace=True)  # for cases where NaNs are at the start of a series
+
+    # Transpose df so that rows represent channels and columns represent time
+    df = df.T
+
+    # Calculate standard deviation for each channel and scale it to 0-255
+    std = df.std(axis=1).fillna(0)
+    std = ((std - std.min()) * 255) / (std.max() - std.min())
+    std = std.clip(upper=255).astype(int)
+
+    mean_sigma = std.mean()
+    positions = std < channel_std_mult * mean_sigma
+    eliminated_channels = (~positions).sum()
+    if verbose:
+        print(f"{eliminated_channels} channels eliminated")
+
+    if np.sum(positions) > 0:
+        # Replace the line with nans
+        df.iloc[~positions, :] = np.nan
+
+    if interpolate_created_nans:
+        # Interpolate the nans
+        df = df.interpolate(axis=0, limit_direction="both")
+
+    if verbose:
+        print("Eliminating sharp jumps between channels ...")
+    y_profile = np.average(filters.roberts(df.values.astype(float)), axis=1)
+    y_profile = pd.Series(y_profile - y_profile.mean(), index=df.index)
+    mean_sigma = y_profile.std()
+
+    positions = np.abs(y_profile) < jump_std_mult * mean_sigma
+    eliminated_channels = (~positions).sum()
+    if verbose:
+        print(f"{eliminated_channels} channels eliminated")
+
+    if np.sum(positions) > 0:
+        # Replace the line with nans
+        df.iloc[~positions, :] = np.nan
+    else:
+        if verbose:
+            print("Sorry, all channels are bad ...")
+        df = pd.DataFrame()
+    if interpolate_created_nans:
+        # Interpolate the nans
+        df = df.interpolate(axis=0, limit_direction="both")
+    # Transpose df back to original orientation
+    df = df.T
+
+    # Drop nans
+    df.dropna(inplace=True)
+
+    # Bring back original NaN values
+    df[nan_positions] = np.nan
+
+    return df
+
+
+def subtract_constant_background(df, n=300):
+    """
+    Subtract a constant background from a spectrogram represented by a pandas DataFrame.
+
+    The constant background is defined as the median value of the first n rows (timepoints) of the DataFrame.
+
+    Parameters
+    ----------
+    df : pandas.DataFrame
+        Input DataFrame where the index represents time and the columns represent frequency channels.
+    n : int
+        Number of first rows from which the median value is calculated to define the constant background.
+
+    Returns
+    -------
+    pandas.DataFrame
+        DataFrame with the constant background subtracted. The DataFrame is oriented in the same way as the input DataFrame (time on index and frequency on columns).
+
+    """
+    df = df.copy()
+    return df - df.iloc[0:n].median()
+
+
+def subtract_rolling_background(
+    df, window=30, center=False, how="quantile", quantile_value=0.05, **kwargs
+):
+    """
+    Subtract a rolling background from a spectrogram represented by a pandas DataFrame.
+
+    The rolling background is calculated either as the median or a specific quantile value of each rolling window of size `window`.
+
+    Parameters
+    ----------
+    df : pandas.DataFrame
+        Input DataFrame where the index represents time and the columns represent frequency channels.
+    window : int, default 30
+        Size of the rolling window from which the background value is calculated.
+    center : bool, default False
+        If True, the rolling window is centered on the current timepoint. If False, the rolling window starts at the current timepoint.
+        See pandas.DataFrame.rolling for more details.
+    how : str, default "median"
+        Method to calculate the rolling background. If "median", the median value of the window is used.
+        If "quantile", the quantile defined by `quantile_value` is used.
+    quantile_value : float, default 0.5
+        The quantile value to use when `how` is "quantile". Ignored if `how` is not "quantile".
+    **kwargs : dict
+        Additional keyword arguments passed to pandas.DataFrame.rolling.
+
+    Returns
+    -------
+    pandas.DataFrame
+        DataFrame with the rolling background subtracted. The DataFrame is oriented in the same way as the input DataFrame (time on index and frequency on columns).
+
+    """
+    df = df.copy()
+    if how == "median":
+        df_rolling = df.rolling(window=window, center=center, **kwargs).median()
+    elif how == "quantile":
+        df_rolling = df.rolling(window=window, center=center, **kwargs).quantile(
+            quantile_value
+        )
+    else:
+        raise ValueError("`how` must be 'median' or 'quantile'")
+    return df - df_rolling
+
+
+def subtract_low_signal_noise_background(df, percentile=0.05):
+    """
+    Background subtraction method adapted for DataFrame.
+    The average and the standard deviation of each row will be calculated and subtracted from the DataFrame.
+
+    Parameters
+    ----------
+    df : DataFrame
+        DataFrame representing the spectrogram with time as index and frequencies as columns.
+    percentile : float, default 0.05
+        Percentile of the lowest standard deviations to use as background.
+    """
+    df_ = df.copy()
+
+    # Subtract the average of each row (time point) from that row
+    row_averages = df_.mean(axis=1)
+    df_ = df_.sub(row_averages, axis=0)
+
+    # Calculate standard deviation for each column (frequency bin)
+    column_sdevs = df_.std(axis=1)
+
+    # Select columns (frequency bins) with the lowest standard deviations (assumed background)
+    n_columns = len(column_sdevs)
+    n_background = int(n_columns * percentile)
+    background_cols = column_sdevs.nsmallest(n_background).index
+    background = df_.loc[background_cols].mean()
+
+    # Subtract this background from each column of the DataFrame
+    return df - background
+
+
+def intensity_to_linear(df, factor=0.0386):
+    """
+    Convert Callisto values (W) and make them linear.
+    Based on the following forumla:
+    db = 10 ** (I * factor)
+
+    Parameters:
+    df (pd.DataFrame): DataFrame with Callisto values.
+    factor (float): Conversion factor in the formula.
+
+    Returns:
+    pd.DataFrame: DataFrame with converted intensity values.
+    """
+    return 10 ** (df * factor)
+
+
+def linear_to_intensity(df, factor=0.0386):
+    """
+    Convert db (I) back to Callisto values (W).
+    Based on the following forumla:
+    db = 10 ** (I * factor)
+
+    Parameters:
+    df (pd.DataFrame): DataFrame with intensity values.
+    factor (float): Conversion factor in the formula.
+
+    Returns:
+    pd.DataFrame: DataFrame with converted Callisto values.
+    """
+    return np.log10(df) / factor
```

### Comparing `ecallisto_ng-0.7.11/src/ecallisto_ng/detection/flare_detection.py` & `ecallisto_ng-0.7.12/src/ecallisto_ng/detection/flare_detection.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,216 +1,221 @@
-import os
-import sys
-from collections import defaultdict
-
-import matplotlib.pyplot as plt
-import mlflow
-import numpy as np
-import pandas as pd
-import torch
-import torchvision
-from datetime import timedelta
-import ecallisto_ng
-from ecallisto_ng.data_download.downloader import get_ecallisto_data
-from ecallisto_ng.plotting.plotting import plot_spectogram_mpl
-
-
-class FlareDetection:
-    """
-    Class for detecting flares in solar radio data using a pre-trained deep learning model.
-    This is the result of the FlareSense project, a P5 project at I4ds/FHNW. For more information, see:
-    https://github.com/i4Ds/FlareSense
-
-    Authors: https://github.com/patschue, https://github.com/gabrieltorresgamez
-    Supervisor: https://www.fhnw.ch/de/personen/andre-csillaghy
-    Advisor: https://github.com/kenfus
-
-    Currently, only Australia-ASSA-62 is supported as an instrument.
-
-
-    Args:
-        model_id (str): The unique identifier of the pre-trained model to use.
-        standard_cnn (bool, optional): Turn true, if loaded model is not a custom model. Default is True.
-        device (str, optional): The device to run the model on, one of ["cuda", "mps", "cpu"]. Default is auto-detected.
-
-    Attributes:
-        device (str): The device the model is running on.
-        standard_cnn (bool): True if using a standard CNN model, False if using a custom model.
-        model (torch.nn.Module): The loaded pre-trained PyTorch model for flare detection.
-
-    """
-
-    def __init__(
-        self,
-        model_id="a853ec9b54244b4ab37dce5498597fd3",
-        image_size=[224, 224],
-        device=None,
-        standard_cnn=True,
-        tracking_uri="https://dagshub.com/FlareSense/Flaresense.mlflow",
-    ):
-        """
-        Prepares and initializes an instance of the class.
-
-        Args:
-            model_id (str): The ID of the model to be loaded. Defaults to "33ad4d2d26fe416db7dd9eda2e4fd2fb".
-            standard_cnn (bool): Whether to use the standard CNN architecture. Defaults to True.
-            device: The device to be used for model execution. If not specified, "cuda" is used if available, "mps" if supported, else "cpu".
-        """
-        if device is None:
-            # If no device is specified, use "cuda" if available, else "mps" if supported, else "cpu"
-            device = (
-                "cuda"
-                if torch.cuda.is_available()
-                else "mps"
-                if torch.backends.mps.is_available()
-                else "cpu"
-            )
-        self.device = device
-        self.standard_cnn = standard_cnn
-        self.image_size = image_size
-
-        # Add ecallisto_ng to the path, because of relative imports in the .pth files
-        package_dir = os.path.dirname(ecallisto_ng.__file__)
-        desired_dir = os.path.dirname(package_dir)  # src/ecallisto_ng
-        desired_dir = os.path.dirname(desired_dir)  # src
-        sys.path.append(desired_dir)
-
-        # Load the PyTorch model using MLflow and move it to the specified device
-        mlflow.set_tracking_uri(tracking_uri)
-        self.model = mlflow.pytorch.load_model(f"runs:/{model_id}/model/").to(
-            self.device
-        )
-        self.model.eval()
-
-    def preprocess(self, image, length=None):
-        """
-        Preprocess input solar radio data for prediction.
-
-        Args:
-            image (pd.DataFrame): Solar radio data as a pandas DataFrame.
-            length (list, optional): Desired length for the preprocessed data. Default is [224, 224].
-
-        Returns:
-            torch.Tensor: Preprocessed image data as a torch.Tensor.
-
-        """
-        if length is None:
-            length = self.image_size
-        length_s = torch.tensor((image.index.max() - image.index.min()).total_seconds())
-        resampling_s = torch.round((length_s / length[0])).int().item()
-        image = image.resample(f"{resampling_s}s").max()
-        image = image.interpolate(method="linear", limit_direction="both")
-        image = image.values.T
-        image = torch.tensor(image).float()
-        return image
-
-    def detect(self, datetime, instrument="Australia-ASSA_62", window_length=timedelta(minutes=60)):
-        """
-        Detect flares in solar radio data for a given datetime, instrument, and window length.
-
-        Args:
-            datetime (str or pd.Timestamp): Date and time to start flare detection.
-            instrument (str, optional): Name of the radio instrument. Default is "Australia-ASSA_62".
-            window_length (datetime, optional): Length of the time window for detection. Default is 60 minutes.
-
-        Returns:
-            tuple: A tuple containing:
-                - pd.DataFrame: Solar radio data for the specified time range and instrument.
-                - dict: Flare probability predictions for each minute.
-                - matplotlib.figure.Figure: Matplotlib figure showing the data and flare probability.
-
-        Raises:
-            ValueError: If the window_length is less than 15 minutes.
-            ValueError: If the end_time is in another day.
-
-        """
-        datetime = pd.to_datetime(datetime)
-        window_length = pd.to_timedelta(window_length)
-
-        # Check if the window length is at least 15 minutes, models are trained on 15 minute windows
-        if window_length < pd.to_timedelta("30min"):
-            raise ValueError("window_length must be at least 30min")
-
-        start_time = datetime
-        end_time = datetime + window_length
-        print(f"Detecting flares from {start_time} to {end_time} on {instrument}")
-
-
-        # Get data for the specified time range and instrument
-        data = get_ecallisto_data(start_time, end_time, instrument)
-        if data == {}:
-            print(f"No data found for {start_time} - {end_time} on {instrument}")
-            return None
-        
-        data = data[instrument]
-        # Update start_time and end_time to the actual data range
-        start_time = data.index.min()
-        end_time = data.index.max()
-        window_length = end_time - start_time
-
-        # Generate 15min windows of data
-        img_tensor = []
-        n_predictions = 0
-        while start_time + pd.to_timedelta("15min") <= end_time:
-            data_temp = data.copy()
-            data_temp = data_temp.loc[start_time: start_time + pd.to_timedelta("15min")]
-            if data_temp.shape[0] == 0:
-                continue
-
-            # Preprocess the data for prediction
-            data_temp = self.preprocess(data_temp)
-            data_temp = data_temp.unsqueeze(0)
-            data_temp = torchvision.transforms.functional.resize(
-                data_temp, [224, 224], antialias=True
-                )
-            img_tensor.append(data_temp)
-            start_time = start_time + pd.to_timedelta("1min")
-            n_predictions += 1
-
-        # Stack the 15min windows into a single tensor
-        img_tensor = torch.stack(img_tensor).to(self.device)
-
-        # If the model is not a custom model, expand the tensor to 3 color channels
-        if self.standard_cnn:
-            img_tensor = img_tensor.expand(-1, 3, -1, -1)
-
-        # Make predictions on the data
-        with torch.no_grad():
-            predictions = self.model(img_tensor)
-        predictions = predictions.flatten().cpu().numpy()
-
-        # Average the predictions for each minute
-        minute_by_minute = defaultdict(list)
-        for i in range(n_predictions):
-            for j in range(15):
-                minute_by_minute[i + j].append(predictions[i])
-        minute_by_minute = {k: sum(v) / len(v) for k, v in minute_by_minute.items()}
-
-        # Plot the data
-        fig = plot_spectogram_mpl(data, fig_size=(12, 6))
-
-        # Get the current axis
-        ax1 = fig.gca()
-
-        # Plot the flare probability on top of the data
-        x = np.linspace(0, data.shape[0], len(minute_by_minute))
-        y = np.array(list(minute_by_minute.values())) * data.shape[1]
-        ax1.plot(x, y, color="red", linewidth=2, label="Flare Certainty")
-        ax1.legend(loc="upper right")
-
-        # Create a secondary y-axis
-        ax2 = ax1.twinx()
-
-        # Set the limits for the secondary y-axis (0-100%)
-        ax2.set_ylim(0, 100)
-        ticks = np.linspace(0, 100, 11)
-        ax2.set_yticks(ticks)
-        ax2.set_yticklabels([f"{int(t)}%" for t in ticks])
-        ax2.tick_params(axis="y", labelsize=8, colors="red")
-
-        # Show the plot with a tight layout
-        plt.tight_layout()
-
-        # Get the figure
-        fig = plt.gca().get_figure()
-
-        return data, minute_by_minute, predictions, fig
+import os
+import sys
+from collections import defaultdict
+from datetime import timedelta
+
+import matplotlib.pyplot as plt
+import mlflow
+import numpy as np
+import pandas as pd
+import torch
+import torchvision
+
+import ecallisto_ng
+from ecallisto_ng.data_download.downloader import get_ecallisto_data
+from ecallisto_ng.plotting.plotting import plot_spectogram_mpl
+
+
+class FlareDetection:
+    """
+    Class for detecting flares in solar radio data using a pre-trained deep learning model.
+    This is the result of the FlareSense project, a P5 project at I4ds/FHNW. For more information, see:
+    https://github.com/i4Ds/FlareSense
+
+    Authors: https://github.com/patschue, https://github.com/gabrieltorresgamez
+    Supervisor: https://www.fhnw.ch/de/personen/andre-csillaghy
+    Advisor: https://github.com/kenfus
+
+    Currently, only Australia-ASSA-62 is supported as an instrument.
+
+
+    Args:
+        model_id (str): The unique identifier of the pre-trained model to use.
+        standard_cnn (bool, optional): Turn true, if loaded model is not a custom model. Default is True.
+        device (str, optional): The device to run the model on, one of ["cuda", "mps", "cpu"]. Default is auto-detected.
+
+    Attributes:
+        device (str): The device the model is running on.
+        standard_cnn (bool): True if using a standard CNN model, False if using a custom model.
+        model (torch.nn.Module): The loaded pre-trained PyTorch model for flare detection.
+
+    """
+
+    def __init__(
+        self,
+        model_id="a853ec9b54244b4ab37dce5498597fd3",
+        image_size=[224, 224],
+        device=None,
+        standard_cnn=True,
+        tracking_uri="https://dagshub.com/FlareSense/Flaresense.mlflow",
+    ):
+        """
+        Prepares and initializes an instance of the class.
+
+        Args:
+            model_id (str): The ID of the model to be loaded. Defaults to "33ad4d2d26fe416db7dd9eda2e4fd2fb".
+            standard_cnn (bool): Whether to use the standard CNN architecture. Defaults to True.
+            device: The device to be used for model execution. If not specified, "cuda" is used if available, "mps" if supported, else "cpu".
+        """
+        if device is None:
+            # If no device is specified, use "cuda" if available, else "mps" if supported, else "cpu"
+            device = (
+                "cuda"
+                if torch.cuda.is_available()
+                else "mps" if torch.backends.mps.is_available() else "cpu"
+            )
+        self.device = device
+        self.standard_cnn = standard_cnn
+        self.image_size = image_size
+
+        # Add ecallisto_ng to the path, because of relative imports in the .pth files
+        package_dir = os.path.dirname(ecallisto_ng.__file__)
+        desired_dir = os.path.dirname(package_dir)  # src/ecallisto_ng
+        desired_dir = os.path.dirname(desired_dir)  # src
+        sys.path.append(desired_dir)
+
+        # Load the PyTorch model using MLflow and move it to the specified device
+        mlflow.set_tracking_uri(tracking_uri)
+        self.model = mlflow.pytorch.load_model(f"runs:/{model_id}/model/").to(
+            self.device
+        )
+        self.model.eval()
+
+    def preprocess(self, image, length=None):
+        """
+        Preprocess input solar radio data for prediction.
+
+        Args:
+            image (pd.DataFrame): Solar radio data as a pandas DataFrame.
+            length (list, optional): Desired length for the preprocessed data. Default is [224, 224].
+
+        Returns:
+            torch.Tensor: Preprocessed image data as a torch.Tensor.
+
+        """
+        if length is None:
+            length = self.image_size
+        length_s = torch.tensor((image.index.max() - image.index.min()).total_seconds())
+        resampling_s = torch.round((length_s / length[0])).int().item()
+        image = image.resample(f"{resampling_s}s").max()
+        image = image.interpolate(method="linear", limit_direction="both")
+        image = image.values.T
+        image = torch.tensor(image).float()
+        return image
+
+    def detect(
+        self,
+        datetime,
+        instrument="Australia-ASSA_62",
+        window_length=timedelta(minutes=60),
+    ):
+        """
+        Detect flares in solar radio data for a given datetime, instrument, and window length.
+
+        Args:
+            datetime (str or pd.Timestamp): Date and time to start flare detection.
+            instrument (str, optional): Name of the radio instrument. Default is "Australia-ASSA_62".
+            window_length (datetime, optional): Length of the time window for detection. Default is 60 minutes.
+
+        Returns:
+            tuple: A tuple containing:
+                - pd.DataFrame: Solar radio data for the specified time range and instrument.
+                - dict: Flare probability predictions for each minute.
+                - matplotlib.figure.Figure: Matplotlib figure showing the data and flare probability.
+
+        Raises:
+            ValueError: If the window_length is less than 15 minutes.
+            ValueError: If the end_time is in another day.
+
+        """
+        datetime = pd.to_datetime(datetime)
+        window_length = pd.to_timedelta(window_length)
+
+        # Check if the window length is at least 15 minutes, models are trained on 15 minute windows
+        if window_length < pd.to_timedelta("30min"):
+            raise ValueError("window_length must be at least 30min")
+
+        start_time = datetime
+        end_time = datetime + window_length
+        print(f"Detecting flares from {start_time} to {end_time} on {instrument}")
+
+        # Get data for the specified time range and instrument
+        data = get_ecallisto_data(start_time, end_time, instrument)
+        if data == {}:
+            print(f"No data found for {start_time} - {end_time} on {instrument}")
+            return None
+
+        data = data[instrument]
+        # Update start_time and end_time to the actual data range
+        start_time = data.index.min()
+        end_time = data.index.max()
+        window_length = end_time - start_time
+
+        # Generate 15min windows of data
+        img_tensor = []
+        n_predictions = 0
+        while start_time + pd.to_timedelta("15min") <= end_time:
+            data_temp = data.copy()
+            data_temp = data_temp.loc[
+                start_time : start_time + pd.to_timedelta("15min")
+            ]
+            if data_temp.shape[0] == 0:
+                continue
+
+            # Preprocess the data for prediction
+            data_temp = self.preprocess(data_temp)
+            data_temp = data_temp.unsqueeze(0)
+            data_temp = torchvision.transforms.functional.resize(
+                data_temp, [224, 224], antialias=True
+            )
+            img_tensor.append(data_temp)
+            start_time = start_time + pd.to_timedelta("1min")
+            n_predictions += 1
+
+        # Stack the 15min windows into a single tensor
+        img_tensor = torch.stack(img_tensor).to(self.device)
+
+        # If the model is not a custom model, expand the tensor to 3 color channels
+        if self.standard_cnn:
+            img_tensor = img_tensor.expand(-1, 3, -1, -1)
+
+        # Make predictions on the data
+        with torch.no_grad():
+            predictions = self.model(img_tensor)
+        predictions = predictions.flatten().cpu().numpy()
+
+        # Average the predictions for each minute
+        minute_by_minute = defaultdict(list)
+        for i in range(n_predictions):
+            for j in range(15):
+                minute_by_minute[i + j].append(predictions[i])
+        minute_by_minute = {k: sum(v) / len(v) for k, v in minute_by_minute.items()}
+
+        # Plot the data
+        fig = plot_spectogram_mpl(data, fig_size=(12, 6))
+
+        # Get the current axis
+        ax1 = fig.gca()
+
+        # Plot the flare probability on top of the data
+        x = np.linspace(0, data.shape[0], len(minute_by_minute))
+        y = np.array(list(minute_by_minute.values())) * data.shape[1]
+        ax1.plot(x, y, color="red", linewidth=2, label="Flare Certainty")
+        ax1.legend(loc="upper right")
+
+        # Create a secondary y-axis
+        ax2 = ax1.twinx()
+
+        # Set the limits for the secondary y-axis (0-100%)
+        ax2.set_ylim(0, 100)
+        ticks = np.linspace(0, 100, 11)
+        ax2.set_yticks(ticks)
+        ax2.set_yticklabels([f"{int(t)}%" for t in ticks])
+        ax2.tick_params(axis="y", labelsize=8, colors="red")
+
+        # Show the plot with a tight layout
+        plt.tight_layout()
+
+        # Get the figure
+        fig = plt.gca().get_figure()
+
+        return data, minute_by_minute, predictions, fig
```

### Comparing `ecallisto_ng-0.7.11/src/ecallisto_ng/plotting/plotting.py` & `ecallisto_ng-0.7.12/src/ecallisto_ng/plotting/plotting.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,276 +1,296 @@
-import matplotlib.pyplot as plt
-import numpy as np
-import pandas as pd
-import plotly.express as px
-import plotly.io as pio
-
-from ecallisto_ng.data_download.downloader import get_ecallisto_data
-from ecallisto_ng.data_fetching.get_data import NoDataAvailable
-from ecallisto_ng.plotting.utils import (
-    calculate_resample_freq,
-    return_strftime_based_on_range,
-    return_strftime_for_ticks_based_on_range,
-)
-
-
-def plot_spectogram_mpl(
-    df,
-    instrument_name=None,
-    start_datetime=None,
-    end_datetime=None,
-    title="Flux",
-    fig_size=(9, 6),
-    cmap="plasma",
-):
-    # Create a new dataframe with rounded column names
-    df = df.copy()
-    # Check if it's a dictionary. If it is, take the first key
-    if isinstance(df, dict):
-        if len(df) > 1:
-            Warning(
-                "The dataframe has more than one instrument. Only the first instrument will be used."
-            )
-        df = df[list(df.keys())[0]]
-
-    # Drop any rows where the datetime col is NaN
-    df = df[df.index.notnull()]
-
-    # Reverse the columns
-    df = df.iloc[:, ::-1]
-
-    # If instrument name is not provided, try to get it from the dataframe
-    if instrument_name is None:
-        instrument_name = df.attrs.get("FULLNAME", "Unknown")
-
-    # If start_datetime is not provided, try to get it from the dataframe
-    if start_datetime is None:
-        start_datetime = df.index.min()
-    if end_datetime is None:
-        end_datetime = df.index.max()
-
-    # Make datetime prettier
-    if isinstance(start_datetime, str):
-        start_datetime = pd.to_datetime(start_datetime)
-    if isinstance(end_datetime, str):
-        end_datetime = pd.to_datetime(end_datetime)
-
-    strf_format = return_strftime_based_on_range(end_datetime - start_datetime)
-    strf_format_ticks = return_strftime_for_ticks_based_on_range(
-        end_datetime - start_datetime
-    )
-    sd_str = start_datetime.strftime(strf_format)
-    ed_str = end_datetime.strftime(strf_format)
-
-    fig, ax = plt.subplots(figsize=fig_size)
-
-    # Set NaN color to black
-    current_cmap = plt.get_cmap(cmap).copy()
-    current_cmap.set_bad(color="black")
-
-    # The imshow function in matplotlib displays data top-down, so we need to reverse the rows
-    cax = ax.imshow(
-        df.T.iloc[::-1],
-        aspect="auto",
-        extent=[0, df.shape[0], 0, df.shape[1]],
-        cmap=current_cmap,
-        interpolation="none",
-    )
-
-    def find_nearest_idx(array, value):
-        array = np.asarray(array)
-        idx = (np.abs(array - value)).argmin()
-        return idx
-
-    # Calculate the rough spacing for around 15 labels
-    spacing = max(1, int(df.shape[1] / 15))
-
-    # Create target ticks
-    target_ticks = np.unique((df.columns.astype(float) / 10).astype(int) * 10)
-
-    # Finding the closest indices in the DataFrame to the target_ticks
-    major_ticks = [
-        find_nearest_idx(df.columns.astype(float), tick) for tick in target_ticks
-    ]
-
-    # Set major ticks and their appearance
-    ax.set_yticks(major_ticks, minor=False)  # This line was missing
-    ax.tick_params(axis="y", which="major", length=10, labelsize="medium")
-
-    # Create labels based on the position
-    major_labels = [str(int(round(float(df.columns[i]), 0))) for i in major_ticks]
-    ax.set_yticklabels(major_labels, minor=False)
-
-    # Assuming df index is datetime, this will format the x-ticks
-    # Compute the spacing required to get close to 30 x-labels
-    spacing = max(1, df.shape[0] // 15)
-
-    x_ticks = np.arange(0, df.shape[0], spacing)
-    ax.set_xticks(x_ticks)
-    # Get format
-    strf_format_ticks = return_strftime_for_ticks_based_on_range(
-        end_datetime - start_datetime
-    )
-    ax.set_xticklabels(
-        df.index[x_ticks].strftime(strf_format_ticks), rotation=60, ha="center"
-    )
-    # Title
-    title = f"{instrument_name} {title} | {sd_str} to {ed_str}"
-    ax.set_title(title, fontsize=16)
-    ax.set_xlabel("Time [UT]")
-    ax.set_ylabel("Frequency [MHz]")
-    ax.grid(False)
-
-    # Adding colorbar
-    cbar = fig.colorbar(cax)
-    cbar.set_label("Amplitude")
-
-    fig.tight_layout()
-    return fig
-
-
-def plot_spectogram(
-    df,
-    instrument_name=None,
-    start_datetime=None,
-    end_datetime=None,
-    title="Radio Flux Density",
-    save_path=None,
-    resolution=1440,
-    samplig_method="max",
-    font_size=18,
-    fig_size=(600, 1000),
-    color_scale=px.colors.sequential.Plasma,
-):
-    # Check if it's a dictionary. If it is, take the first key
-    if isinstance(df, dict):
-        if len(df) > 1:
-            Warning(
-                "The dataframe has more than one instrument. Only the first instrument will be used."
-            )
-        df = df[list(df.keys())[0]]
-    # Create a new dataframe with rounded column names
-    df = df.copy()
-    df.columns = df.columns.astype(float)
-
-    # If instrument name is not provided, try to get it from the dataframe
-    if instrument_name is None:
-        instrument_name = df.attrs.get("FULLNAME", "Unknown")
-
-    # If start_datetime is not provided, try to get it from the dataframe
-    if start_datetime is None:
-        start_datetime = df.index.min()
-    if end_datetime is None:
-        end_datetime = df.index.max()
-
-    # Make datetime prettier
-    if isinstance(start_datetime, str):
-        start_datetime = pd.to_datetime(start_datetime)
-    if isinstance(end_datetime, str):
-        end_datetime = pd.to_datetime(end_datetime)
-
-    # If resolution is provided, resample the dataframe
-    if resolution is not None:
-        resample_freq = calculate_resample_freq(
-            start_datetime, end_datetime, resolution
-        )
-        resample_freq = max(resample_freq, pd.Timedelta(milliseconds=250))
-
-        # Resample data
-        if samplig_method == "mean":
-            df = df.resample(resample_freq).mean()
-        elif samplig_method == "max":
-            df = df.resample(resample_freq).max()
-        elif samplig_method == "min":
-            df = df.resample(resample_freq).min()
-
-    fig = px.imshow(
-        df.T,
-        color_continuous_scale=color_scale,
-        zmin=df.min().min(),
-        zmax=df.max().max(),
-        height=fig_size[0],
-        width=fig_size[1],
-    )
-    fig.update_layout(
-        title=f"{instrument_name} {title}",
-        xaxis_title="Datetime [UT]",
-        yaxis_title="Frequency [MHz]",
-        font=dict(family="Computer Modern, monospace", size=font_size, color="#4D4D4D"),
-        plot_bgcolor="black",
-        xaxis_showgrid=True,
-        yaxis_showgrid=False,
-    )
-    if save_path is not None:
-        pio.write_image(fig, save_path)  # Save the figure
-    return fig
-
-
-def plot_with_fixed_resolution_mpl(
-    instrument,
-    start_datetime_str,
-    end_datetime_str,
-    sampling_method="max",
-    download_from_local=False,
-    resolution=1440,
-    fig_size=(9, 6),
-    verbose=False,
-):
-    """
-    Plots the spectrogram for the given instrument between specified start and end datetime strings
-    with a fixed resolution using Matplotlib.
-
-    Parameters:
-    - instrument (str): The name of the instrument for which the spectrogram needs to be plotted.
-    - start_datetime_str (str or pd.Timestamp): The starting datetime for the data range.
-        Can be a string in the format 'YYYY-MM-DD HH:MM:SS' or a Pandas Timestamp.
-    - end_datetime_str (str or pd.Timestamp): The ending datetime for the data range.
-        Can be a string in the format 'YYYY-MM-DD HH:MM:SS' or a Pandas Timestamp.
-    - resolution (int, optional): The desired resolution for plotting. Default is 1440.
-        Determines the time bucketing for the data aggregation.
-    - fig_size (tuple, optional): The desired figure size. Default is (9, 6).
-        The figure size is passed to Matplotlib's `figsize` parameter.
-
-    Returns:
-    None. A spectrogram is plotted using Matplotlib.
-    """
-    start_datetime = pd.to_datetime(start_datetime_str)
-    end_datetime = pd.to_datetime(end_datetime_str)
-
-    # Fetch data
-    df = get_ecallisto_data(
-        start_datetime,
-        end_datetime,
-        instrument,
-        download_from_local=download_from_local,
-        verbose=verbose,
-    )
-    # Check if it's a dictionary. If it is, take the first key
-    if isinstance(df, dict):
-        if len(df) > 1:
-            Warning(
-                "The dataframe has more than one instrument. Only the first instrument will be used."
-            )
-        df = df[list(df.keys())[0]]
-
-    if len(df) == 0:
-        print(NoDataAvailable)
-        return None
-
-    if resolution is not None:
-        # Calculate resampling frequency
-        resample_freq = calculate_resample_freq(
-            start_datetime, end_datetime, resolution
-        )
-        resample_freq = max(resample_freq, pd.Timedelta(milliseconds=250))
-        # Resample data
-        if sampling_method.lower() == "mean":
-            df = df.resample(resample_freq).mean()
-        elif sampling_method.lower() == "max":
-            df = df.resample(resample_freq).max()
-        elif sampling_method.lower() == "min":
-            df = df.resample(resample_freq).min()
-
-    # Plot
-    return plot_spectogram_mpl(
-        df, instrument, start_datetime, end_datetime, fig_size=fig_size
-    )
+import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
+import plotly.express as px
+import plotly.io as pio
+
+from ecallisto_ng.data_download.downloader import get_ecallisto_data
+from ecallisto_ng.data_fetching.get_data import NoDataAvailable
+from ecallisto_ng.plotting.utils import (
+    downcast_resolution,
+    return_strftime_based_on_range,
+    return_strftime_for_ticks_based_on_range,
+    calculate_resample_freq,
+)
+
+
+def plot_spectogram_mpl(
+    df,
+    instrument_name=None,
+    start_datetime=None,
+    end_datetime=None,
+    title="Flux",
+    fig_size=(9, 6),
+    cmap="plasma",
+    cross_to_plot=None,
+    dot_to_plot=None,
+    cbar_label="Radio Flux",
+    vmin=None,
+    vmax=None,
+):
+    # Create a new dataframe with rounded column names
+    df = df.copy()
+    # Check if it's a dictionary. If it is, take the first key
+    if isinstance(df, dict):
+        if len(df) > 1:
+            Warning(
+                "The dataframe has more than one instrument. Only the first instrument will be used."
+            )
+        df = df[list(df.keys())[0]]
+
+    # Drop any rows where the datetime col is NaN
+    df = df[df.index.notnull()]
+
+    # Reverse the columns
+    df = df.iloc[:, ::-1]
+
+    # If instrument name is not provided, try to get it from the dataframe
+    if instrument_name is None:
+        instrument_name = df.attrs.get("FULLNAME", "Unknown")
+
+    # If start_datetime is not provided, try to get it from the dataframe
+    if start_datetime is None:
+        start_datetime = df.index.min()
+    if end_datetime is None:
+        end_datetime = df.index.max()
+
+    # Make datetime prettier
+    if isinstance(start_datetime, str):
+        start_datetime = pd.to_datetime(start_datetime)
+    if isinstance(end_datetime, str):
+        end_datetime = pd.to_datetime(end_datetime)
+
+    strf_format = return_strftime_based_on_range(end_datetime - start_datetime)
+    strf_format_ticks = return_strftime_for_ticks_based_on_range(
+        end_datetime - start_datetime
+    )
+    sd_str = start_datetime.strftime(strf_format)
+    ed_str = end_datetime.strftime(strf_format)
+
+    fig, ax = plt.subplots(figsize=fig_size)
+
+    # Set NaN color to black
+    current_cmap = plt.get_cmap(cmap).copy()
+    current_cmap.set_bad(color="black")
+
+    # The imshow function in matplotlib displays data top-down, so we need to reverse the rows
+    cax = ax.imshow(
+        df.T.iloc[::-1],
+        aspect="auto",
+        extent=[0, df.shape[0], 0, df.shape[1]],
+        cmap=current_cmap,
+        interpolation="none",
+        vmin=vmin,
+        vmax=vmax,
+    )
+
+    def find_nearest_idx(array, value):
+        array = np.asarray(array)
+        idx = (np.abs(array - value)).argmin()
+        return idx
+
+    # Calculate the rough spacing for around 15 labels
+    spacing = max(1, int(df.shape[1] / 15))
+
+    # Create target ticks
+    target_ticks = np.unique((df.columns.astype(float) / 10).astype(int) * 10)
+
+    # Finding the closest indices in the DataFrame to the target_ticks
+    major_ticks = [
+        find_nearest_idx(df.columns.astype(float), tick) for tick in target_ticks
+    ]
+
+    # Set major ticks and their appearance
+    ax.set_yticks(major_ticks, minor=False)  # This line was missing
+    ax.tick_params(axis="y", which="major", length=10, labelsize="medium")
+
+    # Create labels based on the position
+    major_labels = [str(int(round(float(df.columns[i]), 0))) for i in major_ticks]
+    ax.set_yticklabels(major_labels, minor=False)
+
+    # Assuming df index is datetime, this will format the x-ticks
+    # Compute the spacing required to get close to 30 x-labels
+    spacing = max(1, df.shape[0] // 8)
+
+    x_ticks = np.arange(0, df.shape[0], spacing)
+    ax.set_xticks(x_ticks)
+    # Get format
+    strf_format_ticks = return_strftime_for_ticks_based_on_range(
+        end_datetime - start_datetime
+    )
+    ax.set_xticklabels(
+        df.index[x_ticks].strftime(strf_format_ticks), rotation=0, ha="center"
+    )
+    # Title
+    title = (
+        f"{instrument_name} {title} | {sd_str} to {ed_str}" if title is not None else ""
+    )
+    ax.set_title(title, fontsize=16)
+    ax.set_xlabel("Time [UT]")
+    ax.set_ylabel("Frequency [MHz]")
+    ax.grid(False)
+
+    if cross_to_plot is not None:
+        for time, y in zip(cross_to_plot[0], cross_to_plot[1]):
+            # Convert time to the corresponding x-coordinate in the plot
+            x_pos = np.argmin(np.abs(df.index - time))
+
+            # Assuming y is a frequency and needs to be mapped to the reversed y-axis
+            y_transformed = find_nearest_idx(df.columns.astype(float), y)
+
+            ax.plot(x_pos, y_transformed, "x", color="gray")  # Adding crosses
+
+    if dot_to_plot is not None:
+        for time, y in zip(dot_to_plot[0], dot_to_plot[1]):
+            # Convert time to the corresponding x-coordinate in the plot
+            x_pos = np.argmin(np.abs(df.index - time))
+
+            # Assuming y is a frequency and needs to be mapped to the reversed y-axis
+            y_transformed = find_nearest_idx(df.columns.astype(float), y)
+
+            ax.plot(x_pos, y_transformed, "+", color="blue")  # Adding crosses
+    # Adding colorbar
+    cbar = fig.colorbar(cax)
+    cbar.set_label(cbar_label)
+
+    fig.tight_layout()
+    return fig
+
+
+def plot_spectogram(
+    df,
+    instrument_name=None,
+    start_datetime=None,
+    end_datetime=None,
+    title="Radio Flux Density",
+    save_path=None,
+    resolution=1440,
+    samplig_method="max",
+    font_size=18,
+    fig_size=(600, 1000),
+    color_scale=px.colors.sequential.Plasma,
+):
+    # Check if it's a dictionary. If it is, take the first key
+    if isinstance(df, dict):
+        if len(df) > 1:
+            Warning(
+                "The dataframe has more than one instrument. Only the first instrument will be used."
+            )
+        df = df[list(df.keys())[0]]
+    # Create a new dataframe with rounded column names
+    df = df.copy()
+    df.columns = df.columns.astype(float)
+
+    # If instrument name is not provided, try to get it from the dataframe
+    if instrument_name is None:
+        instrument_name = df.attrs.get("FULLNAME", "Unknown")
+
+    # If start_datetime is not provided, try to get it from the dataframe
+    if start_datetime is None:
+        start_datetime = df.index.min()
+    if end_datetime is None:
+        end_datetime = df.index.max()
+
+    # Make datetime prettier
+    if isinstance(start_datetime, str):
+        start_datetime = pd.to_datetime(start_datetime)
+    if isinstance(end_datetime, str):
+        end_datetime = pd.to_datetime(end_datetime)
+
+    # If resolution is provided, resample the dataframe
+    if resolution is not None:
+        df = downcast_resolution(
+            df, start_datetime, end_datetime, resolution, samplig_method
+        )
+
+    fig = px.imshow(
+        df.T,
+        color_continuous_scale=color_scale,
+        zmin=df.min().min(),
+        zmax=df.max().max(),
+        height=fig_size[0],
+        width=fig_size[1],
+    )
+    fig.update_layout(
+        title=f"{instrument_name} {title}",
+        xaxis_title="Time [UT]",
+        yaxis_title="Frequency [MHz]",
+        font=dict(family="Computer Modern, monospace", size=font_size, color="#4D4D4D"),
+        plot_bgcolor="black",
+        xaxis_showgrid=True,
+        yaxis_showgrid=False,
+    )
+    if save_path is not None:
+        pio.write_image(fig, save_path)  # Save the figure
+    return fig
+
+
+def plot_with_fixed_resolution_mpl(
+    instrument,
+    start_datetime_str,
+    end_datetime_str,
+    sampling_method="max",
+    download_from_local=False,
+    resolution=1440,
+    fig_size=(9, 6),
+    verbose=False,
+):
+    """
+    Plots the spectrogram for the given instrument between specified start and end datetime strings
+    with a fixed resolution using Matplotlib.
+
+    Parameters:
+    - instrument (str): The name of the instrument for which the spectrogram needs to be plotted.
+    - start_datetime_str (str or pd.Timestamp): The starting datetime for the data range.
+        Can be a string in the format 'YYYY-MM-DD HH:MM:SS' or a Pandas Timestamp.
+    - end_datetime_str (str or pd.Timestamp): The ending datetime for the data range.
+        Can be a string in the format 'YYYY-MM-DD HH:MM:SS' or a Pandas Timestamp.
+    - resolution (int, optional): The desired resolution for plotting. Default is 1440.
+        Determines the time bucketing for the data aggregation.
+    - fig_size (tuple, optional): The desired figure size. Default is (9, 6).
+        The figure size is passed to Matplotlib's `figsize` parameter.
+
+    Returns:
+    None. A spectrogram is plotted using Matplotlib.
+    """
+    start_datetime = pd.to_datetime(start_datetime_str)
+    end_datetime = pd.to_datetime(end_datetime_str)
+
+    # Fetch data
+    df = get_ecallisto_data(
+        start_datetime,
+        end_datetime,
+        instrument,
+        download_from_local=download_from_local,
+        verbose=verbose,
+    )
+    # Check if it's a dictionary. If it is, take the first key
+    if isinstance(df, dict):
+        if len(df) > 1:
+            Warning(
+                "The dataframe has more than one instrument. Only the first instrument will be used."
+            )
+        df = df[list(df.keys())[0]]
+
+    if len(df) == 0:
+        print(NoDataAvailable)
+        return None
+
+    if resolution is not None:
+        # Calculate resampling frequency
+        resample_freq = calculate_resample_freq(
+            start_datetime, end_datetime, resolution
+        )
+        resample_freq = max(resample_freq, pd.Timedelta(milliseconds=250))
+        # Resample data
+        if sampling_method.lower() == "mean":
+            df = df.resample(resample_freq).mean()
+        elif sampling_method.lower() == "max":
+            df = df.resample(resample_freq).max()
+        elif sampling_method.lower() == "min":
+            df = df.resample(resample_freq).min()
+
+    # Plot
+    return plot_spectogram_mpl(
+        df, instrument, start_datetime, end_datetime, fig_size=fig_size
+    )
```

### Comparing `ecallisto_ng-0.7.11/src/ecallisto_ng/plotting/utils.py` & `ecallisto_ng-0.7.12/src/ecallisto_ng/plotting/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,96 +1,118 @@
-import numpy as np
-import pandas as pd
-
-
-def calculate_resample_freq(start_datetime, end_datetime, resolution):
-    tota_time_delta = end_datetime - start_datetime
-    return tota_time_delta / (resolution - 1)
-
-
-def return_strftime_based_on_range(time_range):
-    # Decide on the date-time format based on the time range
-    if time_range > pd.Timedelta(days=1):
-        date_format = "%Y-%m-%d"
-    elif time_range > pd.Timedelta(hours=1):
-        date_format = "%Y-%m-%d %H:%M"
-    else:
-        date_format = "%Y-%m-%d %H:%M:%S"
-
-    return date_format
-
-
-def return_strftime_for_ticks_based_on_range(time_range):
-    # Decide on the date-time format based on the time range
-    if time_range < pd.Timedelta(days=1):
-        date_format = "%H:%M:%S"
-    elif time_range < pd.Timedelta(days=30):
-        date_format = "%m-%d %H:%M"
-    else:
-        date_format = "%m-%d %H:%M:%S"
-
-    return date_format
-
-
-def fill_missing_timesteps_with_nan(df, start_datetime=None, end_datetime=None):
-    """
-    Fill missing timesteps in a pandas DataFrame with NaN values. Only needed for plotting.
-
-    Parameters
-    ----------
-    df : pandas.DataFrame
-        The DataFrame to fill missing timesteps in.
-    start_datetime : str or pandas.Timestamp, optional
-        If you want to make sure that the returned DataFrame starts at a specific datetime,
-        you can specify it here. If not specified, the returned DataFrame will start at the
-        first datetime in the input DataFrame.
-    end_datetime : str or pandas.Timestamp, optional
-        If you want to make sure that the returned DataFrame ends at a specific datetime,
-        you can specify it here. If not specified, the returned DataFrame will end at the
-        last datetime in the input DataFrame.
-
-    Returns
-    -------
-    pandas.DataFrame
-        A new DataFrame with missing timesteps filled with NaN values.
-
-    Notes
-    -----
-    This function is useful when working with time-series data that has missing timesteps.
-    By filling the missing timesteps with NaN values, the DataFrame can be easily visualized
-    or analyzed without introducing errors due to missing data.
-
-    The function calculates the median time delta of the input DataFrame, and then creates
-    a new index with evenly spaced values based on that delta. It then uses the pandas
-    `reindex` function to fill in missing timesteps with NaN values.
-
-    Examples
-    --------
-    >>> dates = pd.date_range('2023-02-19 01:00', '2023-02-19 05:00', freq='2H')
-    >>> freqs = ['10M', '20M', '30M']
-    >>> data = np.random.randn(len(dates), len(freqs))
-    >>> df = pd.DataFrame(data, index=dates, columns=freqs)
-    >>> df = df.drop(df.index[1])
-    >>> df = fill_missing_timesteps_with_nan(df)
-    >>> print(df)
-                            10M       20M       30M
-    2023-02-19 01:00:00 -0.349636  0.004947  0.546848
-    2023-02-19 03:00:00       NaN       NaN       NaN
-    2023-02-19 05:00:00 -0.576182  1.222293 -0.416526
-    """
-    # Change index to datetime, if it's not already
-    df.index = pd.to_datetime(df.index)
-    # Add start and end datetimes to the index
-    # Fill missing timesteps with NaN values
-    time_delta = np.median(np.diff(df.index.values))
-    time_delta = pd.Timedelta(time_delta)
-    start_datetime = df.index[0] if start_datetime is None else start_datetime
-    new_index = pd.date_range(df.index[0], df.index[-1], freq=time_delta)
-    # Add missing timesteps incase they are not present in the original index
-    if start_datetime:
-        while new_index.min() > start_datetime:
-            new_index = new_index.insert(0, new_index.min() - time_delta)
-    if end_datetime:
-        while new_index.max() < end_datetime:
-            new_index = new_index.insert(len(new_index), new_index.max() + time_delta)
-    df = df.reindex(new_index)
-    return df
+import numpy as np
+import pandas as pd
+
+
+def downcast_resolution(df, start_datetime, end_datetime, resolution, sampling_method):
+    # Calculate resampling frequency
+    resample_freq = calculate_resample_freq(start_datetime, end_datetime, resolution)
+    resample_freq = max(resample_freq, pd.Timedelta(milliseconds=250))
+    # Resample data
+    df = downcast_timedelta(df, resample_freq, sampling_method)
+
+    return df
+
+
+def downcast_timedelta(df, resample_timedelta, sampling_method):
+    # Resample data
+    if sampling_method.lower() == "mean":
+        df = df.resample(resample_timedelta).mean()
+    elif sampling_method.lower() == "max":
+        df = df.resample(resample_timedelta).max()
+    elif sampling_method.lower() == "min":
+        df = df.resample(resample_timedelta).min()
+
+    return df
+
+
+def calculate_resample_freq(start_datetime, end_datetime, resolution):
+    tota_time_delta = end_datetime - start_datetime
+    return tota_time_delta / (resolution - 1)
+
+
+def return_strftime_based_on_range(time_range):
+    # Decide on the date-time format based on the time range
+    if time_range > pd.Timedelta(days=1):
+        date_format = "%Y-%m-%d"
+    elif time_range > pd.Timedelta(hours=1):
+        date_format = "%Y-%m-%d %H:%M"
+    else:
+        date_format = "%Y-%m-%d %H:%M:%S"
+
+    return date_format
+
+
+def return_strftime_for_ticks_based_on_range(time_range):
+    # Decide on the date-time format based on the time range
+    if time_range < pd.Timedelta(days=1):
+        date_format = "%H:%M:%S"
+    elif time_range < pd.Timedelta(days=30):
+        date_format = "%m-%d %H:%M"
+    else:
+        date_format = "%m-%d %H:%M:%S"
+
+    return date_format
+
+
+def fill_missing_timesteps_with_nan(df, start_datetime=None, end_datetime=None):
+    """
+    Fill missing timesteps in a pandas DataFrame with NaN values. Only needed for plotting.
+
+    Parameters
+    ----------
+    df : pandas.DataFrame
+        The DataFrame to fill missing timesteps in.
+    start_datetime : str or pandas.Timestamp, optional
+        If you want to make sure that the returned DataFrame starts at a specific datetime,
+        you can specify it here. If not specified, the returned DataFrame will start at the
+        first datetime in the input DataFrame.
+    end_datetime : str or pandas.Timestamp, optional
+        If you want to make sure that the returned DataFrame ends at a specific datetime,
+        you can specify it here. If not specified, the returned DataFrame will end at the
+        last datetime in the input DataFrame.
+
+    Returns
+    -------
+    pandas.DataFrame
+        A new DataFrame with missing timesteps filled with NaN values.
+
+    Notes
+    -----
+    This function is useful when working with time-series data that has missing timesteps.
+    By filling the missing timesteps with NaN values, the DataFrame can be easily visualized
+    or analyzed without introducing errors due to missing data.
+
+    The function calculates the median time delta of the input DataFrame, and then creates
+    a new index with evenly spaced values based on that delta. It then uses the pandas
+    `reindex` function to fill in missing timesteps with NaN values.
+
+    Examples
+    --------
+    >>> dates = pd.date_range('2023-02-19 01:00', '2023-02-19 05:00', freq='2H')
+    >>> freqs = ['10M', '20M', '30M']
+    >>> data = np.random.randn(len(dates), len(freqs))
+    >>> df = pd.DataFrame(data, index=dates, columns=freqs)
+    >>> df = df.drop(df.index[1])
+    >>> df = fill_missing_timesteps_with_nan(df)
+    >>> print(df)
+                            10M       20M       30M
+    2023-02-19 01:00:00 -0.349636  0.004947  0.546848
+    2023-02-19 03:00:00       NaN       NaN       NaN
+    2023-02-19 05:00:00 -0.576182  1.222293 -0.416526
+    """
+    # Change index to datetime, if it's not already
+    df.index = pd.to_datetime(df.index)
+    # Add start and end datetimes to the index
+    # Fill missing timesteps with NaN values
+    time_delta = np.median(np.diff(df.index.values))
+    time_delta = pd.Timedelta(time_delta)
+    start_datetime = df.index[0] if start_datetime is None else start_datetime
+    new_index = pd.date_range(df.index[0], df.index[-1], freq=time_delta)
+    # Add missing timesteps incase they are not present in the original index
+    if start_datetime:
+        while new_index.min() > start_datetime:
+            new_index = new_index.insert(0, new_index.min() - time_delta)
+    if end_datetime:
+        while new_index.max() < end_datetime:
+            new_index = new_index.insert(len(new_index), new_index.max() + time_delta)
+    df = df.reindex(new_index)
+    return df
```

### Comparing `ecallisto_ng-0.7.11/src/ecallisto_ng.egg-info/PKG-INFO` & `ecallisto_ng-0.7.12/src/ecallisto_ng.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,191 +1,205 @@
-Metadata-Version: 2.1
-Name: ecallisto_ng
-Version: 0.7.11
-Summary: A Python package for the fetching (and some processing and plotting) of eCallisto data based on request and pandas.
-Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
-Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
-Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy>=1.21.6
-Requires-Dist: pandas>=2.0.0
-Requires-Dist: openpyxl
-Requires-Dist: plotly
-Requires-Dist: kaleido
-Requires-Dist: matplotlib
-Requires-Dist: requests
-Requires-Dist: scikit-image>=0.20.0
-Requires-Dist: pyarrow
-Requires-Dist: bs4
-Requires-Dist: lxml
-Requires-Dist: astropy
-Requires-Dist: tqdm
-Provides-Extra: nb
-Requires-Dist: nbformat; extra == "nb"
-Requires-Dist: ipython; extra == "nb"
-Requires-Dist: ipykernel; extra == "nb"
-Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-Requires-Dist: build; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Provides-Extra: ml
-Requires-Dist: mlflow; extra == "ml"
-Requires-Dist: torch; extra == "ml"
-Requires-Dist: torchvision; extra == "ml"
-Requires-Dist: torchmetrics; extra == "ml"
-Requires-Dist: pytorch-lightning; extra == "ml"
-Provides-Extra: va
-Requires-Dist: torch; extra == "va"
-
-# Ecallisto NG 
-Ecallisto NG is a comprehensive Python package tailored for interacting with Ecallisto data. It focuses on facilitating efficient data manipulation, processing, and visualization, leveraging the power of Pandas for data handling and PyTorch for advanced computations. The package is particularly optimized for dealing with large datasets, providing tools for slicing, filtering, and resampling data to make spectogram plotting more manageable.
-
-## Table of Contents
-- [Background](#background)
-- [Installation](#installation)
-  - [PyPI](#pypi)
-  - [Dev Installation](#dev-installation)
-  - [Virtual Antenna Creation](#creation-of-the-virtual-antenna)
-- [Using Pandas with Ecallisto NG](#pandas)
-- [Examples and Usage](#examples-and-usage)
-  - [Data Fetching](#data-fetching-deprecated)
-  - [Data Processing and Visualization](#data-processing-and-visualization)
-  - [Plotting](#plotting)
-  - [Spectogram Editing](#spectogram-editing)
-- [Additional Information](#additional-information)
-  - [Note on .attrs and FITS Header](#note-on-attrs-and-fits-header)
-  - [Contributing](#contributing)
-
-## Background
-he package is built with Python 3.9 and primarily uses the Pandas library for data manipulation. While it initially offered a direct interaction with the Ecallisto Rest API (now deprecated), its current functionality is centered around efficient data processing and visualization. The data provided by e-Callisto is stored in a pandas Dataframe, where the index is the time and the column names are the observed frequencies.
-
-### Note: The REST API is now deprecated. However, you can still access it via https://v000792.fhnw.ch/api/redoc for a while. This was done because with help of pandas and multiprocessing, the download of the data is much faster and more efficient when directly accessing the files.
-
-## PyPI
-Available on PyPI: https://pypi.org/project/ecallisto-ng/
-
-## Installation
-To install this package, use pip for installation. Execute the following command in your terminal with basic functionality, such as plotting and data fetching:
-```pip install ecallisto-ng```
-If you want to use the virtual antenna:
-```pip install ecallisto-ng[va]```
-If you want to use the detection of flares, powered by ML:
-```pip install ecallisto-ng[ml]```
-
-To use the notebook, please install the notebook dependencies.
-
-## Dev Installation
-Of course, you can also install the package from source. To do so, clone the repository and install the package in editable mode:
-```pip install -e .```
-```pip install -e .[va]```
-```pip install -e .[ml]```
-
-## Pandas
-Pandas is an open-source data analysis and manipulation tool, pivotal to Ecallisto NG. Learning Pandas is essential for effectively using Ecallisto NG, as it allows for sophisticated data slicing, filtering, and aggregation. More on Pandas: https://pandas.pydata.org/docs/
-
-## Examples and Usage
-Please have a look at the jupyter notebook under `example`.
-
-# Getting data
-## `get_ecallisto_data` Function
-
-This function fetches e-Callisto data within a specified date range and optional instrument regex pattern. It's suitable for smaller datasets. For larger datasets, consider using the `get_ecallisto_data_generator` function.
-
-## Parameters
-- `start_datetime` (datetime-like): The start date for the file search.
-- `end_datetime` (datetime-like): The end date for the file search.
-- `instrument_string` (str, List[str] or None): Instrument name(s) for file URL matching. If `None`, all files are considered.
-- `freq_start` (float or None): The start frequency for filtering.
-- `freq_end` (float or None): The end frequency for filtering.
-- `base_url` (str): Base URL of the remote file directory.
-
-## Returns
-- (dict of str: pandas.DataFrame) or pandas.DataFrame: A dictionary of instrument names and their corresponding dataframes. If only one instrument is found, it returns a single dataframe.
-
-## Example
-```python
-from ecallisto_ng.data_fetching import get_ecallisto_data
-from datetime import datetime
-
-start = datetime(2021, 3, 1, 6, 30, 0)
-end = datetime(2021, 3, 7, 23, 30, 0)
-instrument_name = "austria_unigraz_01"
-
-df = get_ecallisto_data(start, end, instrument_name)
-```
-# Getting data via a generator
-## `get_ecallisto_data_generator` Function
-
-A generator function that yields e-Callisto data one file at a time within a date range. It's ideal for handling large datasets or when working with limited memory.
-
-## Parameters
-- `start_datetime` (datetime-like): The start date for the file search.
-- `end_datetime` (datetime-like): The end date for the file search.
-- `instrument_name` (List[str], str, or None): Instrument name(s) for file URL matching. If `None`, all files are considered.
-- `freq_start` (float or None): The start frequency for filtering.
-- `freq_end` (float or None): The end frequency for filtering.
-- `base_url` (str): Base URL of the remote file directory.
-
-## Yields
-- (str, pandas.DataFrame): A tuple containing the instrument name and its corresponding DataFrame.
-
-## Example
-```python
-from ecallisto_ng.data_fetching import get_ecallisto_data_generator
-from datetime import datetime
-
-start = datetime(2021, 3, 1, 6, 30, 0)
-end = datetime(2021, 3, 7, 23, 30, 0)
-instrument_name = ["austria_unigraz_01", "another_instrument"]
-
-data_generator = get_ecallisto_data_generator(start, end, instrument_name)
-for instrument_name, data_frame in data_generator:
-    process_data(instrument_name, data_frame)  # Replace with your processing function
-
-```
-## Plotting 
-Ecallisto NG provides basic plotting capabilities. Here's an example of how to generate a spectogram:
-```python
-from ecallisto_ng.plotting.utils import plot_spectogram
-
-plot_spectogram(df)
-```
-Make use of .resample to reduce the size of the data. Alternatively, you can pass a `resolution` parameter to the plot_spectogram. Here's an example:
-```python
-plot_spectogram(df.resample("1min").max())
-plot_spectogram(df, resolution="1min")
-```
-For more documentation on resample, please refer to the [Pandas documentation](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.resample.html).
-## Spectogram editing
-We also provide some basic functionalities to edit the spectogram. Here's how you can do it:
-```python
-from ecallisto_ng.data_processing.utils import elimwrongchannels, subtract_constant_background, subtract_rolling_background
-
-df = elimwrongchannels(df)
-df = fill_missing_timesteps_with_nan(df)
-df = subtract_constant_background(df)
-df = subtract_rolling_background(df)
-
-# Filter keep frequencies only between 40 and 70 MHz
-df = df.loc[:, 40:70]
-
-plot_spectogram(df)
-```
-## Additional Information
-### Note on .attrs and FITS Header
-The function utilizes DataFrames with the .attrs attribute to store FITS header information. This attribute is a dictionary-like object and contains metadata about the FITS file, including header details. Accessing .attrs is essential for understanding the context of the data:
-
-```python
-print(df.attrs)
-```
-
-These simple commands allow you to easily manipulate spectogram data, enabling effective use of the Ecallisto API for your needs.
-
-### Contributing
-Contributions to Ecallisto NG are very welcome! If you have an idea for an improvement or have found a bug, please feel free to contribute. The preferred way to contribute is by submitting a Pull Request (PR) or creating an issue on our GitHub repository. This way, we can discuss potential changes or fixes and maintain the quality of the project.
+Metadata-Version: 2.1
+Name: ecallisto_ng
+Version: 0.7.12
+Summary: A Python package for the fetching (and some processing and plotting) of eCallisto data based on request and pandas.
+Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
+Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
+Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy>=1.21.6
+Requires-Dist: pandas>=2.0.0
+Requires-Dist: openpyxl
+Requires-Dist: plotly
+Requires-Dist: kaleido
+Requires-Dist: matplotlib
+Requires-Dist: requests
+Requires-Dist: scikit-image>=0.20.0
+Requires-Dist: pyarrow
+Requires-Dist: bs4
+Requires-Dist: lxml
+Requires-Dist: astropy
+Requires-Dist: tqdm
+Provides-Extra: nb
+Requires-Dist: nbformat; extra == "nb"
+Requires-Dist: ipython; extra == "nb"
+Requires-Dist: ipykernel; extra == "nb"
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Provides-Extra: ml
+Requires-Dist: mlflow; extra == "ml"
+Requires-Dist: torch; extra == "ml"
+Requires-Dist: torchvision; extra == "ml"
+Requires-Dist: torchmetrics; extra == "ml"
+Requires-Dist: pytorch-lightning; extra == "ml"
+Provides-Extra: va
+Requires-Dist: torch; extra == "va"
+Provides-Extra: all
+Requires-Dist: nbformat; extra == "all"
+Requires-Dist: ipython; extra == "all"
+Requires-Dist: ipykernel; extra == "all"
+Requires-Dist: black; extra == "all"
+Requires-Dist: isort; extra == "all"
+Requires-Dist: twine; extra == "all"
+Requires-Dist: build; extra == "all"
+Requires-Dist: pytest; extra == "all"
+Requires-Dist: mlflow; extra == "all"
+Requires-Dist: torch; extra == "all"
+Requires-Dist: torchvision; extra == "all"
+Requires-Dist: torchmetrics; extra == "all"
+Requires-Dist: pytorch-lightning; extra == "all"
+
+# Ecallisto NG 
+Ecallisto NG is a comprehensive Python package tailored for interacting with Ecallisto data. It focuses on facilitating efficient data manipulation, processing, and visualization, leveraging the power of Pandas for data handling and PyTorch for advanced computations. The package is particularly optimized for dealing with large datasets, providing tools for slicing, filtering, and resampling data to make spectogram plotting more manageable.
+
+## Table of Contents
+- [Background](#background)
+- [Installation](#installation)
+  - [PyPI](#pypi)
+  - [Dev Installation](#dev-installation)
+  - [Virtual Antenna Creation](#creation-of-the-virtual-antenna)
+- [Using Pandas with Ecallisto NG](#pandas)
+- [Examples and Usage](#examples-and-usage)
+  - [Data Fetching](#data-fetching-deprecated)
+  - [Data Processing and Visualization](#data-processing-and-visualization)
+  - [Plotting](#plotting)
+  - [Spectogram Editing](#spectogram-editing)
+- [Additional Information](#additional-information)
+  - [Note on .attrs and FITS Header](#note-on-attrs-and-fits-header)
+  - [Contributing](#contributing)
+
+## Background
+he package is built with Python 3.9 and primarily uses the Pandas library for data manipulation. While it initially offered a direct interaction with the Ecallisto Rest API (now deprecated), its current functionality is centered around efficient data processing and visualization. The data provided by e-Callisto is stored in a pandas Dataframe, where the index is the time and the column names are the observed frequencies.
+
+### Note: The REST API is now deprecated. However, you can still access it via https://v000792.fhnw.ch/api/redoc for a while. This was done because with help of pandas and multiprocessing, the download of the data is much faster and more efficient when directly accessing the files.
+
+## PyPI
+Available on PyPI: https://pypi.org/project/ecallisto-ng/
+
+## Installation
+To install this package, use pip for installation. Execute the following command in your terminal with basic functionality, such as plotting and data fetching:
+```pip install ecallisto-ng```
+If you want to use the virtual antenna:
+```pip install ecallisto-ng[va]```
+If you want to use the detection of flares, powered by ML:
+```pip install ecallisto-ng[ml]```
+
+To use the notebook, please install the notebook dependencies.
+
+## Dev Installation
+Of course, you can also install the package from source. To do so, clone the repository and install the package in editable mode:
+```pip install -e .```
+```pip install -e .[va]```
+```pip install -e .[ml]```
+
+## Pandas
+Pandas is an open-source data analysis and manipulation tool, pivotal to Ecallisto NG. Learning Pandas is essential for effectively using Ecallisto NG, as it allows for sophisticated data slicing, filtering, and aggregation. More on Pandas: https://pandas.pydata.org/docs/
+
+## Examples and Usage
+Please have a look at the jupyter notebook under `example`.
+
+# Getting data
+## `get_ecallisto_data` Function
+
+This function fetches e-Callisto data within a specified date range and optional instrument regex pattern. It's suitable for smaller datasets. For larger datasets, consider using the `get_ecallisto_data_generator` function.
+
+## Parameters
+- `start_datetime` (datetime-like): The start date for the file search.
+- `end_datetime` (datetime-like): The end date for the file search.
+- `instrument_string` (str, List[str] or None): Instrument name(s) for file URL matching. If `None`, all files are considered.
+- `freq_start` (float or None): The start frequency for filtering.
+- `freq_end` (float or None): The end frequency for filtering.
+- `base_url` (str): Base URL of the remote file directory.
+
+## Returns
+- (dict of str: pandas.DataFrame) or pandas.DataFrame: A dictionary of instrument names and their corresponding dataframes. If only one instrument is found, it returns a single dataframe.
+
+## Example
+```python
+from ecallisto_ng.data_fetching import get_ecallisto_data
+from datetime import datetime
+
+start = datetime(2021, 3, 1, 6, 30, 0)
+end = datetime(2021, 3, 7, 23, 30, 0)
+instrument_name = "austria_unigraz_01"
+
+df = get_ecallisto_data(start, end, instrument_name)
+```
+# Getting data via a generator
+## `get_ecallisto_data_generator` Function
+
+A generator function that yields e-Callisto data one file at a time within a date range. It's ideal for handling large datasets or when working with limited memory.
+
+## Parameters
+- `start_datetime` (datetime-like): The start date for the file search.
+- `end_datetime` (datetime-like): The end date for the file search.
+- `instrument_name` (List[str], str, or None): Instrument name(s) for file URL matching. If `None`, all files are considered.
+- `freq_start` (float or None): The start frequency for filtering.
+- `freq_end` (float or None): The end frequency for filtering.
+- `base_url` (str): Base URL of the remote file directory.
+
+## Yields
+- (str, pandas.DataFrame): A tuple containing the instrument name and its corresponding DataFrame.
+
+## Example
+```python
+from ecallisto_ng.data_fetching import get_ecallisto_data_generator
+from datetime import datetime
+
+start = datetime(2021, 3, 1, 6, 30, 0)
+end = datetime(2021, 3, 7, 23, 30, 0)
+instrument_name = ["austria_unigraz_01", "another_instrument"]
+
+data_generator = get_ecallisto_data_generator(start, end, instrument_name)
+for instrument_name, data_frame in data_generator:
+    process_data(instrument_name, data_frame)  # Replace with your processing function
+
+```
+## Plotting 
+Ecallisto NG provides basic plotting capabilities. Here's an example of how to generate a spectogram:
+```python
+from ecallisto_ng.plotting.utils import plot_spectogram
+
+plot_spectogram(df)
+```
+Make use of .resample to reduce the size of the data. Alternatively, you can pass a `resolution` parameter to the plot_spectogram. Here's an example:
+```python
+plot_spectogram(df.resample("1min").max())
+plot_spectogram(df, resolution="1min")
+```
+For more documentation on resample, please refer to the [Pandas documentation](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.resample.html).
+## Spectogram editing
+We also provide some basic functionalities to edit the spectogram. Here's how you can do it:
+```python
+from ecallisto_ng.data_processing.utils import elimwrongchannels, subtract_constant_background, subtract_rolling_background
+
+df = elimwrongchannels(df)
+df = fill_missing_timesteps_with_nan(df)
+df = subtract_constant_background(df)
+df = subtract_rolling_background(df)
+
+# Filter keep frequencies only between 40 and 70 MHz
+df = df.loc[:, 40:70]
+
+plot_spectogram(df)
+```
+## Additional Information
+### Note on .attrs and FITS Header
+The function utilizes DataFrames with the .attrs attribute to store FITS header information. This attribute is a dictionary-like object and contains metadata about the FITS file, including header details. Accessing .attrs is essential for understanding the context of the data:
+
+```python
+print(df.attrs)
+```
+
+These simple commands allow you to easily manipulate spectogram data, enabling effective use of the Ecallisto API for your needs.
+
+### Contributing
+Contributions to Ecallisto NG are very welcome! If you have an idea for an improvement or have found a bug, please feel free to contribute. The preferred way to contribute is by submitting a Pull Request (PR) or creating an issue on our GitHub repository. This way, we can discuss potential changes or fixes and maintain the quality of the project.
```

### Comparing `ecallisto_ng-0.7.11/src/ecallisto_ng.egg-info/SOURCES.txt` & `ecallisto_ng-0.7.12/src/ecallisto_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.7.11/src/models/CustomCNN.py` & `ecallisto_ng-0.7.12/src/models/CustomCNN.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,74 +1,80 @@
-import torch
-import torch.nn as nn
-from src.models.DefaultModel import DefaultBinaryModel
-
-class CustomCNN(DefaultBinaryModel):
-    def __init__(self, lr=1e-3, weight_decay=1e-4, dropout_p=0.0):
-        super().__init__(lr=lr, weight_decay=weight_decay)
-        self.dropout_p = dropout_p
-        
-        # Increased convolutional layers with more filters
-        self.conv1 = nn.Conv2d(1, 64, 3, stride=1, padding=1) 
-        self.conv2 = nn.Conv2d(64, 128, 3, stride=1, padding=1)
-        self.conv3 = nn.Conv2d(128, 256, 3, stride=1, padding=1)
-        self.conv4 = nn.Conv2d(256, 512, 3, stride=1, padding=1)
-
-        # Smaller linear layers
-        self.fc1 = nn.Linear(512 * 12 * 14, 64)
-        self.fc2 = nn.Linear(64, 1)
-        
-        self.pool = nn.MaxPool2d(2, 2)
-        self.dropout = nn.Dropout(self.dropout_p)
-
-    def forward(self, x):
-        x = x[:, 0].unsqueeze(1)
-        x = self.pool(nn.functional.relu(self.conv1(x)))
-        x = self.pool(nn.functional.relu(self.conv2(x)))
-        x = self.pool(nn.functional.relu(self.conv3(x)))
-        x = self.pool(nn.functional.relu(self.conv4(x)))
-        x = x.flatten(start_dim=1)
-        x = nn.functional.relu(self.fc1(x))
-        x = self.dropout(x)
-        x = torch.sigmoid(self.fc2(x))
-        return x
-
-    def configure_optimizers(self):
-        return torch.optim.Adam(self.parameters(), lr=self.lr, weight_decay=self.weight_decay)
-
-class CustomCNN2(DefaultBinaryModel):
-    def __init__(self, lr=1e-3, weight_decay=1e-4, dropout_p=0.0):
-        super().__init__(lr=lr, weight_decay=weight_decay)
-        self.dropout_p = dropout_p
-        
-        # Reduced convolutional layers filters for complexity reduction
-        self.conv1 = nn.Conv2d(1, 32, 3, stride=1, padding=1)
-        self.bn1 = nn.BatchNorm2d(32)  # Batch Normalization after Conv1
-        self.conv2 = nn.Conv2d(32, 64, 3, stride=1, padding=1)
-        self.bn2 = nn.BatchNorm2d(64)  # Batch Normalization after Conv2
-        self.conv3 = nn.Conv2d(64, 128, 3, stride=1, padding=1)
-        self.bn3 = nn.BatchNorm2d(128) # Batch Normalization after Conv3
-        self.conv4 = nn.Conv2d(128, 256, 3, stride=1, padding=1)
-        self.bn4 = nn.BatchNorm2d(256) # Batch Normalization after Conv4
-
-        # Adjusted linear layer sizes
-        self.fc1 = nn.Linear(256 * 12 * 14, 64)
-        self.fc2 = nn.Linear(64, 1)
-        
-        self.pool = nn.MaxPool2d(2, 2)
-        self.dropout = nn.Dropout(self.dropout_p)
-
-    def forward(self, x):
-        x = x[:, 0].unsqueeze(1)
-        x = self.pool(nn.functional.relu(self.bn1(self.conv1(x))))
-        x = self.pool(nn.functional.relu(self.bn2(self.conv2(x))))
-        x = self.pool(nn.functional.relu(self.bn3(self.conv3(x))))
-        x = self.pool(nn.functional.relu(self.bn4(self.conv4(x))))
-        x = x.flatten(start_dim=1)
-        x = nn.functional.relu(self.fc1(x))
-        x = self.dropout(x)
-        x = torch.sigmoid(self.fc2(x))
-        return x
-
-    def configure_optimizers(self):
-        return torch.optim.Adam(self.parameters(), lr=self.lr, weight_decay=self.weight_decay)
-
+import torch
+import torch.nn as nn
+
+from src.models.DefaultModel import DefaultBinaryModel
+
+
+class CustomCNN(DefaultBinaryModel):
+    def __init__(self, lr=1e-3, weight_decay=1e-4, dropout_p=0.0):
+        super().__init__(lr=lr, weight_decay=weight_decay)
+        self.dropout_p = dropout_p
+
+        # Increased convolutional layers with more filters
+        self.conv1 = nn.Conv2d(1, 64, 3, stride=1, padding=1)
+        self.conv2 = nn.Conv2d(64, 128, 3, stride=1, padding=1)
+        self.conv3 = nn.Conv2d(128, 256, 3, stride=1, padding=1)
+        self.conv4 = nn.Conv2d(256, 512, 3, stride=1, padding=1)
+
+        # Smaller linear layers
+        self.fc1 = nn.Linear(512 * 12 * 14, 64)
+        self.fc2 = nn.Linear(64, 1)
+
+        self.pool = nn.MaxPool2d(2, 2)
+        self.dropout = nn.Dropout(self.dropout_p)
+
+    def forward(self, x):
+        x = x[:, 0].unsqueeze(1)
+        x = self.pool(nn.functional.relu(self.conv1(x)))
+        x = self.pool(nn.functional.relu(self.conv2(x)))
+        x = self.pool(nn.functional.relu(self.conv3(x)))
+        x = self.pool(nn.functional.relu(self.conv4(x)))
+        x = x.flatten(start_dim=1)
+        x = nn.functional.relu(self.fc1(x))
+        x = self.dropout(x)
+        x = torch.sigmoid(self.fc2(x))
+        return x
+
+    def configure_optimizers(self):
+        return torch.optim.Adam(
+            self.parameters(), lr=self.lr, weight_decay=self.weight_decay
+        )
+
+
+class CustomCNN2(DefaultBinaryModel):
+    def __init__(self, lr=1e-3, weight_decay=1e-4, dropout_p=0.0):
+        super().__init__(lr=lr, weight_decay=weight_decay)
+        self.dropout_p = dropout_p
+
+        # Reduced convolutional layers filters for complexity reduction
+        self.conv1 = nn.Conv2d(1, 32, 3, stride=1, padding=1)
+        self.bn1 = nn.BatchNorm2d(32)  # Batch Normalization after Conv1
+        self.conv2 = nn.Conv2d(32, 64, 3, stride=1, padding=1)
+        self.bn2 = nn.BatchNorm2d(64)  # Batch Normalization after Conv2
+        self.conv3 = nn.Conv2d(64, 128, 3, stride=1, padding=1)
+        self.bn3 = nn.BatchNorm2d(128)  # Batch Normalization after Conv3
+        self.conv4 = nn.Conv2d(128, 256, 3, stride=1, padding=1)
+        self.bn4 = nn.BatchNorm2d(256)  # Batch Normalization after Conv4
+
+        # Adjusted linear layer sizes
+        self.fc1 = nn.Linear(256 * 12 * 14, 64)
+        self.fc2 = nn.Linear(64, 1)
+
+        self.pool = nn.MaxPool2d(2, 2)
+        self.dropout = nn.Dropout(self.dropout_p)
+
+    def forward(self, x):
+        x = x[:, 0].unsqueeze(1)
+        x = self.pool(nn.functional.relu(self.bn1(self.conv1(x))))
+        x = self.pool(nn.functional.relu(self.bn2(self.conv2(x))))
+        x = self.pool(nn.functional.relu(self.bn3(self.conv3(x))))
+        x = self.pool(nn.functional.relu(self.bn4(self.conv4(x))))
+        x = x.flatten(start_dim=1)
+        x = nn.functional.relu(self.fc1(x))
+        x = self.dropout(x)
+        x = torch.sigmoid(self.fc2(x))
+        return x
+
+    def configure_optimizers(self):
+        return torch.optim.Adam(
+            self.parameters(), lr=self.lr, weight_decay=self.weight_decay
+        )
```

### Comparing `ecallisto_ng-0.7.11/src/models/DefaultModel.py` & `ecallisto_ng-0.7.12/src/models/DefaultModel.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,123 +1,134 @@
-import torch
-import torch.nn as nn
-import torch.optim as optim
-import pytorch_lightning as pl
-from torchmetrics.classification import BinaryPrecision, BinaryRecall
-
-
-class DefaultBinaryModel(pl.LightningModule):
-    """
-    Default binary classifier model.
-    Other models should inherit from this class.
-    """
-
-    def __init__(self, lr=1e-4, weight_decay=1e-4):
-        super().__init__()
-
-        self.lr = lr
-        self.weight_decay = weight_decay
-
-        # Metriken
-        self.precision = BinaryPrecision(threshold=0.5)
-        self.recall = BinaryRecall(threshold=0.5)
-
-        # Label- und Vorhersagelisten
-        self.train_loss = []
-        self.train_labels = []
-        self.train_preds = []
-        self.val_loss = []
-        self.val_labels = []
-        self.val_preds = []
-        self.test_loss = []
-        self.test_labels = []
-        self.test_preds = []
-
-    def forward(self, x):
-        raise NotImplementedError("Modell __init__ und forward Methode muss implementiert werden")
-
-    def __step(self, batch):
-        images, info = batch
-
-        binary_labels = [0 if label == "no_burst" else 1 for label in info["label"]]
-        binary_labels = torch.tensor(binary_labels).float().view(-1, 1)
-        binary_labels = binary_labels.to(images.device)
-
-        images = images.expand(-1, 3, -1, -1)
-        outputs = self(images)
-        return outputs, binary_labels
-
-    def training_step(self, batch, batch_idx):
-        outputs, binary_labels = self.__step(batch)
-        loss = nn.BCELoss()(outputs, binary_labels)
-
-        self.train_labels.append(binary_labels)
-        self.train_preds.append(outputs)
-        self.train_loss.append(loss)
-        return loss
-
-    def validation_step(self, batch, batch_idx):
-        outputs, binary_labels = self.__step(batch)
-        loss = nn.BCELoss()(outputs, binary_labels)
-
-        predictions = (outputs >= 0.5).int()
-        self.val_labels.append(binary_labels.int())
-        self.val_preds.append(predictions)
-        self.val_loss.append(loss)
-        return loss
-
-    def test_step(self, batch, batch_idx):
-        outputs, binary_labels = self.__step(batch)
-        loss = nn.BCELoss()(outputs, binary_labels)
-
-        self.test_labels.append(binary_labels)
-        self.test_preds.append(outputs)
-        self.test_loss.append(loss)
-        return loss
-
-    def on_train_epoch_end(self):
-        train_labels = torch.cat(self.train_labels, dim=0)
-        train_preds = torch.cat(self.train_preds, dim=0)
-
-        train_precision = self.precision(train_preds, train_labels)
-        train_recall = self.recall(train_preds, train_labels)
-
-        self.log("train_loss", torch.stack(self.train_loss).mean(), prog_bar=True, logger=True)
-        self.log("train_precision", train_precision, prog_bar=True, logger=True)
-        self.log("train_recall", train_recall, prog_bar=True, logger=True)
-
-        self.train_labels = []
-        self.train_preds = []
-        self.train_loss = []
-
-    def on_validation_epoch_end(self):
-        val_labels = torch.cat(self.val_labels, dim=0)
-        val_preds = torch.cat(self.val_preds, dim=0)
-
-        val_precision = self.precision(val_preds, val_labels)
-        val_recall = self.recall(val_preds, val_labels)
-
-        self.log("val_loss", torch.stack(self.val_loss).mean(), prog_bar=True, logger=True)
-        self.log("val_precision", val_precision, prog_bar=True, logger=True)
-        self.log("val_recall", val_recall, prog_bar=True, logger=True)
-
-        self.val_labels = []
-        self.val_preds = []
-        self.val_loss = []
-
-    def on_test_epoch_end(self):
-        test_labels = torch.cat(self.test_labels, dim=0)
-        test_preds = torch.cat(self.test_preds, dim=0)
-
-        test_precision = self.precision(test_preds, test_labels)
-        test_recall = self.recall(test_preds, test_labels)
-
-        self.log("test_loss", torch.stack(self.test_loss).mean(), prog_bar=True, logger=True)
-        self.log("test_precision", test_precision, prog_bar=True, logger=True)
-        self.log("test_recall", test_recall, prog_bar=True, logger=True)
-
-        self.test_labels = []
-        self.test_preds = []
-        self.test_loss = []
-
-    def configure_optimizers(self):
-        return optim.Adam(self.parameters(), lr=self.lr, weight_decay=self.weight_decay)
+import pytorch_lightning as pl
+import torch
+import torch.nn as nn
+import torch.optim as optim
+from torchmetrics.classification import BinaryPrecision, BinaryRecall
+
+
+class DefaultBinaryModel(pl.LightningModule):
+    """
+    Default binary classifier model.
+    Other models should inherit from this class.
+    """
+
+    def __init__(self, lr=1e-4, weight_decay=1e-4):
+        super().__init__()
+
+        self.lr = lr
+        self.weight_decay = weight_decay
+
+        # Metriken
+        self.precision = BinaryPrecision(threshold=0.5)
+        self.recall = BinaryRecall(threshold=0.5)
+
+        # Label- und Vorhersagelisten
+        self.train_loss = []
+        self.train_labels = []
+        self.train_preds = []
+        self.val_loss = []
+        self.val_labels = []
+        self.val_preds = []
+        self.test_loss = []
+        self.test_labels = []
+        self.test_preds = []
+
+    def forward(self, x):
+        raise NotImplementedError(
+            "Modell __init__ und forward Methode muss implementiert werden"
+        )
+
+    def __step(self, batch):
+        images, info = batch
+
+        binary_labels = [0 if label == "no_burst" else 1 for label in info["label"]]
+        binary_labels = torch.tensor(binary_labels).float().view(-1, 1)
+        binary_labels = binary_labels.to(images.device)
+
+        images = images.expand(-1, 3, -1, -1)
+        outputs = self(images)
+        return outputs, binary_labels
+
+    def training_step(self, batch, batch_idx):
+        outputs, binary_labels = self.__step(batch)
+        loss = nn.BCELoss()(outputs, binary_labels)
+
+        self.train_labels.append(binary_labels)
+        self.train_preds.append(outputs)
+        self.train_loss.append(loss)
+        return loss
+
+    def validation_step(self, batch, batch_idx):
+        outputs, binary_labels = self.__step(batch)
+        loss = nn.BCELoss()(outputs, binary_labels)
+
+        predictions = (outputs >= 0.5).int()
+        self.val_labels.append(binary_labels.int())
+        self.val_preds.append(predictions)
+        self.val_loss.append(loss)
+        return loss
+
+    def test_step(self, batch, batch_idx):
+        outputs, binary_labels = self.__step(batch)
+        loss = nn.BCELoss()(outputs, binary_labels)
+
+        self.test_labels.append(binary_labels)
+        self.test_preds.append(outputs)
+        self.test_loss.append(loss)
+        return loss
+
+    def on_train_epoch_end(self):
+        train_labels = torch.cat(self.train_labels, dim=0)
+        train_preds = torch.cat(self.train_preds, dim=0)
+
+        train_precision = self.precision(train_preds, train_labels)
+        train_recall = self.recall(train_preds, train_labels)
+
+        self.log(
+            "train_loss",
+            torch.stack(self.train_loss).mean(),
+            prog_bar=True,
+            logger=True,
+        )
+        self.log("train_precision", train_precision, prog_bar=True, logger=True)
+        self.log("train_recall", train_recall, prog_bar=True, logger=True)
+
+        self.train_labels = []
+        self.train_preds = []
+        self.train_loss = []
+
+    def on_validation_epoch_end(self):
+        val_labels = torch.cat(self.val_labels, dim=0)
+        val_preds = torch.cat(self.val_preds, dim=0)
+
+        val_precision = self.precision(val_preds, val_labels)
+        val_recall = self.recall(val_preds, val_labels)
+
+        self.log(
+            "val_loss", torch.stack(self.val_loss).mean(), prog_bar=True, logger=True
+        )
+        self.log("val_precision", val_precision, prog_bar=True, logger=True)
+        self.log("val_recall", val_recall, prog_bar=True, logger=True)
+
+        self.val_labels = []
+        self.val_preds = []
+        self.val_loss = []
+
+    def on_test_epoch_end(self):
+        test_labels = torch.cat(self.test_labels, dim=0)
+        test_preds = torch.cat(self.test_preds, dim=0)
+
+        test_precision = self.precision(test_preds, test_labels)
+        test_recall = self.recall(test_preds, test_labels)
+
+        self.log(
+            "test_loss", torch.stack(self.test_loss).mean(), prog_bar=True, logger=True
+        )
+        self.log("test_precision", test_precision, prog_bar=True, logger=True)
+        self.log("test_recall", test_recall, prog_bar=True, logger=True)
+
+        self.test_labels = []
+        self.test_preds = []
+        self.test_loss = []
+
+    def configure_optimizers(self):
+        return optim.Adam(self.parameters(), lr=self.lr, weight_decay=self.weight_decay)
```

### Comparing `ecallisto_ng-0.7.11/src/models/EfficientNetV2SBinaryClassifier.py` & `ecallisto_ng-0.7.12/src/models/EfficientNetV2SBinaryClassifier.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,46 @@
-import torch.nn as nn
-import torch.optim as optim
-import torchvision.models as models
-from src.models.DefaultModel import DefaultBinaryModel
-from torchvision.models.efficientnet import efficientnet_v2_s
-
-
-class EfficientNetV2SBinaryClassifier(DefaultBinaryModel):
-    """
-    Binary classifier based on EfficientNetV2S architecture.
-    """
-
-    def __init__(self, lr=1e-3, weight_decay=1e-4):
-        super().__init__(lr=lr, weight_decay=weight_decay)
-
-        # EfficientNet V2 S Modell laden
-        self.efficientnet_v2_s = efficientnet_v2_s(weights=models.EfficientNet_V2_S_Weights.DEFAULT)
-        num_features = self.efficientnet_v2_s.classifier[1].in_features
-        self.efficientnet_v2_s.classifier = nn.Sequential(nn.Linear(num_features, 1), nn.Sigmoid())
-
-        # Layer einfrieren
-        for param in self.efficientnet_v2_s.parameters():
-            param.requires_grad = False
-
-        # Submodule zum Trainieren bestimmen (Beispiel: die letzten drei Submodule von 'features')
-        submodules_to_train = ["5", "6", "7"]
-        for name, module in self.efficientnet_v2_s.named_children():
-            if name == "features":
-                for sub_name, sub_module in module.named_children():
-                    if sub_name in submodules_to_train:
-                        for param in sub_module.parameters():
-                            param.requires_grad = True
-            elif name in ["avgpool", "classifier"]:
-                for param in module.parameters():
-                    param.requires_grad = True
-
-    def forward(self, x):
-        return self.efficientnet_v2_s(x)
-
-    def configure_optimizers(self):
-        return optim.Adam(self.parameters(), lr=self.lr, weight_decay=self.weight_decay)
+import torch.nn as nn
+import torch.optim as optim
+import torchvision.models as models
+from torchvision.models.efficientnet import efficientnet_v2_s
+
+from src.models.DefaultModel import DefaultBinaryModel
+
+
+class EfficientNetV2SBinaryClassifier(DefaultBinaryModel):
+    """
+    Binary classifier based on EfficientNetV2S architecture.
+    """
+
+    def __init__(self, lr=1e-3, weight_decay=1e-4):
+        super().__init__(lr=lr, weight_decay=weight_decay)
+
+        # EfficientNet V2 S Modell laden
+        self.efficientnet_v2_s = efficientnet_v2_s(
+            weights=models.EfficientNet_V2_S_Weights.DEFAULT
+        )
+        num_features = self.efficientnet_v2_s.classifier[1].in_features
+        self.efficientnet_v2_s.classifier = nn.Sequential(
+            nn.Linear(num_features, 1), nn.Sigmoid()
+        )
+
+        # Layer einfrieren
+        for param in self.efficientnet_v2_s.parameters():
+            param.requires_grad = False
+
+        # Submodule zum Trainieren bestimmen (Beispiel: die letzten drei Submodule von 'features')
+        submodules_to_train = ["5", "6", "7"]
+        for name, module in self.efficientnet_v2_s.named_children():
+            if name == "features":
+                for sub_name, sub_module in module.named_children():
+                    if sub_name in submodules_to_train:
+                        for param in sub_module.parameters():
+                            param.requires_grad = True
+            elif name in ["avgpool", "classifier"]:
+                for param in module.parameters():
+                    param.requires_grad = True
+
+    def forward(self, x):
+        return self.efficientnet_v2_s(x)
+
+    def configure_optimizers(self):
+        return optim.Adam(self.parameters(), lr=self.lr, weight_decay=self.weight_decay)
```

### Comparing `ecallisto_ng-0.7.11/src/models/ResNet50BinaryClassifier.py` & `ecallisto_ng-0.7.12/src/models/ResNet18BinaryClassifier.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-import torch.nn as nn
-import torch.optim as optim
-import torchvision.models as models
-from src.models.DefaultModel import DefaultBinaryModel
-
-
-class ResNet50BinaryClassifier(DefaultBinaryModel):
-    """
-    Binary classifier based on ResNet50 architecture.
-    """
-
-    def __init__(self, lr=1e-3, weight_decay=1e-4):
-        super().__init__(lr=lr, weight_decay=weight_decay)
-
-        self.resnet50 = models.resnet50(weights=models.ResNet50_Weights.DEFAULT)
-        num_features = self.resnet50.fc.in_features
-        self.resnet50.fc = nn.Sequential(nn.Linear(num_features, 1), nn.Sigmoid())
-
-        for param in self.resnet50.parameters():
-            param.requires_grad = False
-
-        layers_to_train = ["layer3", "layer4", "avgpool", "fc"]
-        for name, child in self.resnet50.named_children():
-            if name in layers_to_train:
-                for param in child.parameters():
-                    param.requires_grad = True
-
-    def forward(self, x):
-        return self.resnet50(x)
-
-    def configure_optimizers(self):
-        return optim.Adam(self.parameters(), lr=self.lr, weight_decay=self.weight_decay)
+import torch.nn as nn
+import torch.optim as optim
+import torchvision.models as models
+
+from src.models.DefaultModel import DefaultBinaryModel
+
+
+class ResNet18BinaryClassifier(DefaultBinaryModel):
+    """
+    Binary classifier based on ResNet18 architecture.
+    """
+
+    def __init__(self, lr=1e-3, weight_decay=1e-4):
+        super().__init__(lr=lr, weight_decay=weight_decay)
+
+        self.resnet18 = models.resnet18(weights=models.ResNet18_Weights.DEFAULT)
+        num_features = self.resnet18.fc.in_features
+        self.resnet18.fc = nn.Sequential(nn.Linear(num_features, 1), nn.Sigmoid())
+
+        for param in self.resnet18.parameters():
+            param.requires_grad = False
+
+        layers_to_train = ["layer3", "layer4", "avgpool", "fc"]
+        for name, child in self.resnet18.named_children():
+            if name in layers_to_train:
+                for param in child.parameters():
+                    param.requires_grad = True
+
+    def forward(self, x):
+        return self.resnet18(x)
+
+    def configure_optimizers(self):
+        return optim.Adam(self.parameters(), lr=self.lr, weight_decay=self.weight_decay)
```

### Comparing `ecallisto_ng-0.7.11/tests/test_bg_subs.py` & `ecallisto_ng-0.7.12/tests/test_bg_subs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-import pytest
-
-from ecallisto_ng.data_processing.utils import (
-    elimwrongchannels,
-    subtract_constant_background,
-    subtract_low_signal_noise_background,
-)
-
-
-@pytest.mark.parametrize(
-    "function",
-    [
-        elimwrongchannels,
-        subtract_constant_background,
-        subtract_low_signal_noise_background,
-    ],
-)
-def test_bg_subs(small_assa01_dataframe, function):
-    df = small_assa01_dataframe["Australia-ASSA_01"]
-    df_processed = function(df)
-
-    assert df_processed.shape == df.shape
-    assert df_processed.columns.to_list() == df.columns.to_list()
-    assert df_processed.index.to_list() == df.index.to_list()
-    assert df_processed.isna().sum().sum() == 0
-    assert not df_processed.equals(df)
+import pytest
+
+from ecallisto_ng.data_processing.utils import (
+    elimwrongchannels, subtract_constant_background,
+    subtract_low_signal_noise_background)
+
+
+@pytest.mark.parametrize(
+    "function",
+    [
+        elimwrongchannels,
+        subtract_constant_background,
+        subtract_low_signal_noise_background,
+    ],
+)
+def test_bg_subs(small_assa01_dataframe, function):
+    df = small_assa01_dataframe["Australia-ASSA_01"]
+    df_processed = function(df)
+
+    assert df_processed.shape == df.shape
+    assert df_processed.columns.to_list() == df.columns.to_list()
+    assert df_processed.index.to_list() == df.index.to_list()
+    assert df_processed.isna().sum().sum() == 0
+    assert not df_processed.equals(df)
```

### Comparing `ecallisto_ng-0.7.11/tests/test_data_download.py` & `ecallisto_ng-0.7.12/tests/test_data_download.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,60 +1,58 @@
-from datetime import datetime
-
-from ecallisto_ng.data_download.downloader import (
-    get_ecallisto_data_generator,
-    get_instrument_with_available_data,
-)
-
-
-def test_get_avail_instruments():
-    start_datetime = datetime(2021, 5, 7, 0, 00, 0)
-    end_datetime = datetime(2021, 5, 7, 23, 59, 0)
-
-    avail = get_instrument_with_available_data(start_datetime, end_datetime)
-    assert len(avail) > 0
-    # Check some instruments
-    [
-        "AUSTRIA-Krumbach_10",
-        "AUSTRIA-MICHELBACH_60",
-        "AUSTRIA-OE3FLB_55",
-        "AUSTRIA-OE3FLB_57",
-        "AUSTRIA-UNIGRAZ_01",
-        "AUSTRIA-UNIGRAZ_02",
-        "Australia-ASSA_56",
-        "Australia-ASSA_57",
-        "Australia-ASSA_60",
-        "Australia-ASSA_62",
-        "Australia-ASSA_63",
-        "Australia-LMRO_59",
-        "INDIA-GAURI_01",
-        "INDIA-OOTY_01",
-        "INDIA-OOTY_02",
-        "JAPAN-IBARAKI_59",
-    ]
-    for instrument in avail:
-        assert instrument in avail
-
-
-def test_get_data_multiple(assa_dataframes):
-    assert len(assa_dataframes) == 3
-    assert all(
-        [
-            x in ["Australia-ASSA_01", "Australia-ASSA_02", "Australia-ASSA_60"]
-            for x in assa_dataframes.keys()
-        ]
-    )
-    assert assa_dataframes["Australia-ASSA_01"].shape == (172490, 193)
-
-
-def test_get_data_single(assa01_dataframe):
-    assert len(assa01_dataframe) == 1
-    assert all([x in ["Australia-ASSA_01"] for x in assa01_dataframe.keys()])
-    assert assa01_dataframe["Australia-ASSA_01"].shape == (172490, 193)
-
-
-def test_data_generator():
-    start_datetime = datetime(2021, 5, 7, 0, 00, 0)
-    end_datetime = datetime(2021, 5, 7, 23, 59, 0)
-    generator = get_ecallisto_data_generator(start_datetime, end_datetime, ["ASSA"])
-    for key, _ in generator:
-        assert key in ["Australia-ASSA_01", "Australia-ASSA_02", "Australia-ASSA_60"]
+from datetime import datetime
+
+from ecallisto_ng.data_download.downloader import (
+    get_ecallisto_data_generator, get_instrument_with_available_data)
+
+
+def test_get_avail_instruments():
+    start_datetime = datetime(2021, 5, 7, 0, 00, 0)
+    end_datetime = datetime(2021, 5, 7, 23, 59, 0)
+
+    avail = get_instrument_with_available_data(start_datetime, end_datetime)
+    assert len(avail) > 0
+    # Check some instruments
+    [
+        "AUSTRIA-Krumbach_10",
+        "AUSTRIA-MICHELBACH_60",
+        "AUSTRIA-OE3FLB_55",
+        "AUSTRIA-OE3FLB_57",
+        "AUSTRIA-UNIGRAZ_01",
+        "AUSTRIA-UNIGRAZ_02",
+        "Australia-ASSA_56",
+        "Australia-ASSA_57",
+        "Australia-ASSA_60",
+        "Australia-ASSA_62",
+        "Australia-ASSA_63",
+        "Australia-LMRO_59",
+        "INDIA-GAURI_01",
+        "INDIA-OOTY_01",
+        "INDIA-OOTY_02",
+        "JAPAN-IBARAKI_59",
+    ]
+    for instrument in avail:
+        assert instrument in avail
+
+
+def test_get_data_multiple(assa_dataframes):
+    assert len(assa_dataframes) == 3
+    assert all(
+        [
+            x in ["Australia-ASSA_01", "Australia-ASSA_02", "Australia-ASSA_60"]
+            for x in assa_dataframes.keys()
+        ]
+    )
+    assert assa_dataframes["Australia-ASSA_01"].shape == (172490, 193)
+
+
+def test_get_data_single(assa01_dataframe):
+    assert len(assa01_dataframe) == 1
+    assert all([x in ["Australia-ASSA_01"] for x in assa01_dataframe.keys()])
+    assert assa01_dataframe["Australia-ASSA_01"].shape == (172490, 193)
+
+
+def test_data_generator():
+    start_datetime = datetime(2021, 5, 7, 0, 00, 0)
+    end_datetime = datetime(2021, 5, 7, 23, 59, 0)
+    generator = get_ecallisto_data_generator(start_datetime, end_datetime, ["ASSA"])
+    for key, _ in generator:
+        assert key in ["Australia-ASSA_01", "Australia-ASSA_02", "Australia-ASSA_60"]
```

