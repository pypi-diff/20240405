# Comparing `tmp/valjean-0.11.0a0.tar.gz` & `tmp/valjean-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valjean-0.11.0a0.tar", max compression
+gzip compressed data, was "valjean-0.9.0.tar", max compression
```

## Comparing `valjean-0.11.0a0.tar` & `valjean-0.9.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0    21864 2021-05-03 13:30:18.768275 valjean-0.11.0a0/LICENSE
--rw-r--r--   0        0        0    22756 2021-05-03 13:30:18.768275 valjean-0.11.0a0/LICENSE_fr
--rw-r--r--   0        0        0     1395 2022-02-02 11:56:45.908392 valjean-0.11.0a0/README.md
--rw-r--r--   0        0        0     7743 2024-03-27 09:36:50.100132 valjean-0.11.0a0/pyproject.toml
--rw-r--r--   0        0        0     4636 2024-03-19 08:55:02.209099 valjean-0.11.0a0/valjean/__init__.py
--rw-r--r--   0        0        0        0 2018-01-22 10:31:18.799174 valjean-0.11.0a0/valjean/cambronne/__init__.py
--rw-r--r--   0        0        0        0 2018-01-22 10:31:18.799174 valjean-0.11.0a0/valjean/cambronne/commands/__init__.py
--rw-r--r--   0        0        0     2958 2024-03-19 08:55:02.209099 valjean-0.11.0a0/valjean/cambronne/commands/env.py
--rw-r--r--   0        0        0     5861 2024-03-19 08:55:02.209099 valjean-0.11.0a0/valjean/cambronne/commands/graph.py
--rw-r--r--   0        0        0     7038 2024-03-19 08:55:02.209099 valjean-0.11.0a0/valjean/cambronne/commands/run.py
--rw-r--r--   0        0        0    10211 2024-03-19 08:55:02.209099 valjean-0.11.0a0/valjean/cambronne/common.py
--rw-r--r--   0        0        0     5215 2024-03-19 08:55:02.209099 valjean-0.11.0a0/valjean/cambronne/main.py
--rw-r--r--   0        0        0     3145 2022-09-16 09:08:15.976983 valjean-0.11.0a0/valjean/chrono.py
--rw-r--r--   0        0        0     4800 2022-09-16 09:08:15.976983 valjean-0.11.0a0/valjean/config.py
--rw-r--r--   0        0        0        0 2017-11-09 17:57:29.083235 valjean-0.11.0a0/valjean/cosette/__init__.py
--rw-r--r--   0        0        0        0 2017-11-17 14:54:32.866418 valjean-0.11.0a0/valjean/cosette/backends/__init__.py
--rw-r--r--   0        0        0    12404 2024-03-19 08:55:02.209099 valjean-0.11.0a0/valjean/cosette/backends/queue.py
--rw-r--r--   0        0        0    17071 2024-03-19 08:55:02.209099 valjean-0.11.0a0/valjean/cosette/code.py
--rw-r--r--   0        0        0    27746 2024-03-19 08:55:02.209099 valjean-0.11.0a0/valjean/cosette/depgraph.py
--rw-r--r--   0        0        0    12946 2024-03-19 08:55:02.209099 valjean-0.11.0a0/valjean/cosette/env.py
--rw-r--r--   0        0        0      976 2021-01-12 13:21:41.899274 valjean-0.11.0a0/valjean/cosette/loop.py
--rw-r--r--   0        0        0    13959 2024-03-19 08:55:02.209099 valjean-0.11.0a0/valjean/cosette/pythontask.py
--rw-r--r--   0        0        0    10545 2022-09-16 09:08:15.976983 valjean-0.11.0a0/valjean/cosette/rlist.py
--rw-r--r--   0        0        0    25079 2024-03-19 08:55:02.209099 valjean-0.11.0a0/valjean/cosette/run.py
--rw-r--r--   0        0        0     6652 2024-03-19 08:55:02.209099 valjean-0.11.0a0/valjean/cosette/scheduler.py
--rw-r--r--   0        0        0     8442 2024-03-19 08:55:02.209099 valjean-0.11.0a0/valjean/cosette/task.py
--rw-r--r--   0        0        0    32682 2024-03-19 08:55:02.209099 valjean-0.11.0a0/valjean/cosette/use.py
--rw-r--r--   0        0        0     3254 2024-03-19 08:55:02.209099 valjean-0.11.0a0/valjean/dyn_import.py
--rw-r--r--   0        0        0        0 2018-01-22 10:31:18.799174 valjean-0.11.0a0/valjean/eponine/__init__.py
--rw-r--r--   0        0        0        0 2021-03-12 16:05:51.079289 valjean-0.11.0a0/valjean/eponine/apollo3/__init__.py
--rw-r--r--   0        0        0    17061 2024-03-19 08:55:02.209099 valjean-0.11.0a0/valjean/eponine/apollo3/hdf5_picker.py
--rw-r--r--   0        0        0    25819 2024-03-19 08:55:02.209099 valjean-0.11.0a0/valjean/eponine/apollo3/hdf5_reader.py
--rw-r--r--   0        0        0    23433 2024-03-19 08:55:02.209099 valjean-0.11.0a0/valjean/eponine/browser.py
--rw-r--r--   0        0        0    38451 2024-03-19 08:55:02.209099 valjean-0.11.0a0/valjean/eponine/dataset.py
--rw-r--r--   0        0        0        0 2018-11-19 17:37:11.315922 valjean-0.11.0a0/valjean/eponine/tripoli4/__init__.py
--rw-r--r--   0        0        0   101019 2024-03-19 08:55:02.209099 valjean-0.11.0a0/valjean/eponine/tripoli4/common.py
--rw-r--r--   0        0        0    13641 2024-03-19 08:55:02.209099 valjean-0.11.0a0/valjean/eponine/tripoli4/data_convertor.py
--rw-r--r--   0        0        0    17556 2024-03-19 08:55:02.209099 valjean-0.11.0a0/valjean/eponine/tripoli4/depletion.py
--rw-r--r--   0        0        0     8529 2024-03-19 08:55:02.209099 valjean-0.11.0a0/valjean/eponine/tripoli4/dump.py
--rw-r--r--   0        0        0    65268 2024-03-19 08:55:02.209099 valjean-0.11.0a0/valjean/eponine/tripoli4/grammar.py
--rw-r--r--   0        0        0    18009 2024-03-19 08:55:02.213099 valjean-0.11.0a0/valjean/eponine/tripoli4/parse.py
--rw-r--r--   0        0        0     5310 2024-03-19 08:55:02.213099 valjean-0.11.0a0/valjean/eponine/tripoli4/parse_debug.py
--rw-r--r--   0        0        0        0 2021-04-13 12:03:50.186457 valjean-0.11.0a0/valjean/eponine/tripoli4/resources/__init__.py
--rw-r--r--   0        0        0    26847 2021-04-13 12:03:50.186457 valjean-0.11.0a0/valjean/eponine/tripoli4/resources/depletion/BurnupResults.C
--rw-r--r--   0        0        0     4963 2021-04-13 12:03:50.186457 valjean-0.11.0a0/valjean/eponine/tripoli4/resources/depletion/BurnupResults.h
--rw-r--r--   0        0        0    12026 2021-04-13 12:03:50.186457 valjean-0.11.0a0/valjean/eponine/tripoli4/resources/depletion/DepletedComposition.C
--rw-r--r--   0        0        0     3718 2021-04-13 12:03:50.186457 valjean-0.11.0a0/valjean/eponine/tripoli4/resources/depletion/DepletedComposition.h
--rw-r--r--   0        0        0    56688 2021-04-13 12:03:50.186457 valjean-0.11.0a0/valjean/eponine/tripoli4/resources/depletion/MeanBurnupResults.C
--rw-r--r--   0        0        0     6655 2021-04-13 12:03:50.186457 valjean-0.11.0a0/valjean/eponine/tripoli4/resources/depletion/MeanBurnupResults.h
--rw-r--r--   0        0        0        0 2021-04-13 12:03:50.186457 valjean-0.11.0a0/valjean/eponine/tripoli4/resources/depletion/__init__.py
--rw-r--r--   0        0        0    25708 2024-03-19 08:55:02.213099 valjean-0.11.0a0/valjean/eponine/tripoli4/scan.py
--rw-r--r--   0        0        0    28242 2024-03-19 08:55:02.213099 valjean-0.11.0a0/valjean/eponine/tripoli4/transform.py
--rw-r--r--   0        0        0    12914 2022-09-16 09:08:15.980983 valjean-0.11.0a0/valjean/eponine/tripoli4/use.py
--rw-r--r--   0        0        0     2767 2022-09-16 09:08:15.980983 valjean-0.11.0a0/valjean/fingerprint.py
--rw-r--r--   0        0        0        0 2018-10-12 08:04:59.368120 valjean-0.11.0a0/valjean/gavroche/__init__.py
--rw-r--r--   0        0        0        0 2019-05-15 15:56:25.795331 valjean-0.11.0a0/valjean/gavroche/diagnostics/__init__.py
--rw-r--r--   0        0        0     5572 2024-03-19 08:55:02.213099 valjean-0.11.0a0/valjean/gavroche/diagnostics/metadata.py
--rw-r--r--   0        0        0    30688 2024-03-19 08:55:02.213099 valjean-0.11.0a0/valjean/gavroche/diagnostics/stats.py
--rw-r--r--   0        0        0     5643 2024-03-19 08:55:02.213099 valjean-0.11.0a0/valjean/gavroche/eval_test_task.py
--rw-r--r--   0        0        0        0 2019-02-11 17:57:22.023822 valjean-0.11.0a0/valjean/gavroche/stat_tests/__init__.py
--rw-r--r--   0        0        0    22603 2024-03-19 08:55:02.213099 valjean-0.11.0a0/valjean/gavroche/stat_tests/bonferroni.py
--rw-r--r--   0        0        0    16176 2022-09-16 09:08:15.980983 valjean-0.11.0a0/valjean/gavroche/stat_tests/chi2.py
--rw-r--r--   0        0        0    21253 2024-03-19 08:55:02.213099 valjean-0.11.0a0/valjean/gavroche/stat_tests/student.py
--rw-r--r--   0        0        0    13147 2022-09-16 09:08:15.980983 valjean-0.11.0a0/valjean/gavroche/test.py
--rw-r--r--   0        0        0        0 2020-05-11 16:57:48.997156 valjean-0.11.0a0/valjean/javert/__init__.py
--rw-r--r--   0        0        0     2511 2022-09-16 09:08:15.980983 valjean-0.11.0a0/valjean/javert/formatter.py
--rw-r--r--   0        0        0    44306 2024-03-19 08:55:02.213099 valjean-0.11.0a0/valjean/javert/mpl.py
--rw-r--r--   0        0        0    25909 2024-03-19 08:55:02.213099 valjean-0.11.0a0/valjean/javert/plot_repr.py
--rw-r--r--   0        0        0    16393 2024-03-19 08:55:02.213099 valjean-0.11.0a0/valjean/javert/representation.py
--rw-r--r--   0        0        0        0 2019-04-26 13:40:17.312157 valjean-0.11.0a0/valjean/javert/resources/__init__.py
--rw-r--r--   0        0        0        0 2019-04-26 13:40:17.312157 valjean-0.11.0a0/valjean/javert/resources/rst/__init__.py
--rw-r--r--   0        0        0      846 2021-03-12 16:05:51.095289 valjean-0.11.0a0/valjean/javert/resources/rst/conf.py.template
--rw-r--r--   0        0        0       38 2019-04-26 13:40:17.316157 valjean-0.11.0a0/valjean/javert/resources/rst/valjean.css
--rw-r--r--   0        0        0    33173 2024-03-19 08:55:02.213099 valjean-0.11.0a0/valjean/javert/rst.py
--rw-r--r--   0        0        0    32957 2024-03-19 08:55:02.213099 valjean-0.11.0a0/valjean/javert/table_repr.py
--rw-r--r--   0        0        0    41442 2024-03-19 08:55:02.213099 valjean-0.11.0a0/valjean/javert/templates.py
--rw-r--r--   0        0        0     4439 2022-09-16 09:08:15.980983 valjean-0.11.0a0/valjean/javert/test_external.py
--rw-r--r--   0        0        0     5453 2022-09-16 09:08:15.980983 valjean-0.11.0a0/valjean/javert/test_report.py
--rw-r--r--   0        0        0     2102 2022-09-16 09:08:15.980983 valjean-0.11.0a0/valjean/javert/verbosity.py
--rw-r--r--   0        0        0     2909 2022-09-16 09:08:15.980983 valjean-0.11.0a0/valjean/path.py
--rw-r--r--   0        0        0     4297 1970-01-01 00:00:00.000000 valjean-0.11.0a0/PKG-INFO
+-rw-r--r--   0        0        0    21864 2022-09-16 11:19:34.366966 valjean-0.9.0/LICENSE
+-rw-r--r--   0        0        0    22756 2022-09-16 11:19:34.366966 valjean-0.9.0/LICENSE_fr
+-rw-r--r--   0        0        0     1395 2022-09-16 11:19:34.366966 valjean-0.9.0/README.md
+-rw-r--r--   0        0        0     8479 2022-09-16 11:19:34.458966 valjean-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3461 2022-09-16 11:19:34.510966 valjean-0.9.0/valjean/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-16 11:19:34.510966 valjean-0.9.0/valjean/cambronne/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-16 11:19:34.510966 valjean-0.9.0/valjean/cambronne/commands/__init__.py
+-rw-r--r--   0        0        0     2928 2022-09-16 11:19:34.510966 valjean-0.9.0/valjean/cambronne/commands/env.py
+-rw-r--r--   0        0        0     5830 2022-09-16 11:19:34.510966 valjean-0.9.0/valjean/cambronne/commands/graph.py
+-rw-r--r--   0        0        0     7007 2022-09-16 11:19:34.510966 valjean-0.9.0/valjean/cambronne/commands/run.py
+-rw-r--r--   0        0        0    10191 2022-09-16 11:19:34.510966 valjean-0.9.0/valjean/cambronne/common.py
+-rw-r--r--   0        0        0     5184 2022-09-16 11:19:34.510966 valjean-0.9.0/valjean/cambronne/main.py
+-rw-r--r--   0        0        0     3145 2022-09-16 11:19:34.510966 valjean-0.9.0/valjean/chrono.py
+-rw-r--r--   0        0        0     4800 2022-09-16 11:19:34.510966 valjean-0.9.0/valjean/config.py
+-rw-r--r--   0        0        0        0 2022-09-16 11:19:34.510966 valjean-0.9.0/valjean/cosette/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-16 11:19:34.510966 valjean-0.9.0/valjean/cosette/backends/__init__.py
+-rw-r--r--   0        0        0    12388 2022-09-16 11:19:34.510966 valjean-0.9.0/valjean/cosette/backends/queue.py
+-rw-r--r--   0        0        0    17046 2022-09-16 11:19:34.510966 valjean-0.9.0/valjean/cosette/code.py
+-rw-r--r--   0        0        0    27714 2022-09-16 11:19:34.510966 valjean-0.9.0/valjean/cosette/depgraph.py
+-rw-r--r--   0        0        0    12914 2022-09-16 11:19:34.510966 valjean-0.9.0/valjean/cosette/env.py
+-rw-r--r--   0        0        0    13883 2022-09-16 11:19:34.510966 valjean-0.9.0/valjean/cosette/pythontask.py
+-rw-r--r--   0        0        0    10545 2022-09-16 11:19:34.510966 valjean-0.9.0/valjean/cosette/rlist.py
+-rw-r--r--   0        0        0    24994 2022-09-16 11:19:34.510966 valjean-0.9.0/valjean/cosette/run.py
+-rw-r--r--   0        0        0     6623 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/cosette/scheduler.py
+-rw-r--r--   0        0        0     8411 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/cosette/task.py
+-rw-r--r--   0        0        0    32605 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/cosette/use.py
+-rw-r--r--   0        0        0     3222 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/dyn_import.py
+-rw-r--r--   0        0        0        0 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/eponine/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/eponine/apollo3/__init__.py
+-rw-r--r--   0        0        0    17018 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/eponine/apollo3/hdf5_picker.py
+-rw-r--r--   0        0        0    25619 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/eponine/apollo3/hdf5_reader.py
+-rw-r--r--   0        0        0    23401 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/eponine/browser.py
+-rw-r--r--   0        0        0    38420 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/eponine/dataset.py
+-rw-r--r--   0        0        0        0 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/eponine/tripoli4/__init__.py
+-rw-r--r--   0        0        0   100679 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/eponine/tripoli4/common.py
+-rw-r--r--   0        0        0    13856 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/eponine/tripoli4/data_convertor.py
+-rw-r--r--   0        0        0    17001 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/eponine/tripoli4/depletion.py
+-rw-r--r--   0        0        0     8515 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/eponine/tripoli4/dump.py
+-rw-r--r--   0        0        0    63142 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/eponine/tripoli4/grammar.py
+-rw-r--r--   0        0        0    17774 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/eponine/tripoli4/parse.py
+-rw-r--r--   0        0        0     5339 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/eponine/tripoli4/parse_debug.py
+-rw-r--r--   0        0        0        0 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/eponine/tripoli4/resources/__init__.py
+-rw-r--r--   0        0        0    26847 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/eponine/tripoli4/resources/depletion/BurnupResults.C
+-rw-r--r--   0        0        0     4963 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/eponine/tripoli4/resources/depletion/BurnupResults.h
+-rw-r--r--   0        0        0    12026 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/eponine/tripoli4/resources/depletion/DepletedComposition.C
+-rw-r--r--   0        0        0     3718 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/eponine/tripoli4/resources/depletion/DepletedComposition.h
+-rw-r--r--   0        0        0    56688 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/eponine/tripoli4/resources/depletion/MeanBurnupResults.C
+-rw-r--r--   0        0        0     6655 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/eponine/tripoli4/resources/depletion/MeanBurnupResults.h
+-rw-r--r--   0        0        0        0 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/eponine/tripoli4/resources/depletion/__init__.py
+-rw-r--r--   0        0        0    25681 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/eponine/tripoli4/scan.py
+-rw-r--r--   0        0        0    27326 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/eponine/tripoli4/transform.py
+-rw-r--r--   0        0        0    12914 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/eponine/tripoli4/use.py
+-rw-r--r--   0        0        0     2767 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/fingerprint.py
+-rw-r--r--   0        0        0        0 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/gavroche/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/gavroche/diagnostics/__init__.py
+-rw-r--r--   0        0        0     5613 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/gavroche/diagnostics/metadata.py
+-rw-r--r--   0        0        0    30704 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/gavroche/diagnostics/stats.py
+-rw-r--r--   0        0        0     5611 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/gavroche/eval_test_task.py
+-rw-r--r--   0        0        0        0 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/gavroche/stat_tests/__init__.py
+-rw-r--r--   0        0        0    22648 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/gavroche/stat_tests/bonferroni.py
+-rw-r--r--   0        0        0    16176 2022-09-16 11:19:34.514966 valjean-0.9.0/valjean/gavroche/stat_tests/chi2.py
+-rw-r--r--   0        0        0    21222 2022-09-16 11:19:34.518966 valjean-0.9.0/valjean/gavroche/stat_tests/student.py
+-rw-r--r--   0        0        0    13147 2022-09-16 11:19:34.518966 valjean-0.9.0/valjean/gavroche/test.py
+-rw-r--r--   0        0        0        0 2022-09-16 11:19:34.518966 valjean-0.9.0/valjean/javert/__init__.py
+-rw-r--r--   0        0        0     2511 2022-09-16 11:19:34.518966 valjean-0.9.0/valjean/javert/formatter.py
+-rw-r--r--   0        0        0    44369 2022-09-16 11:19:34.518966 valjean-0.9.0/valjean/javert/mpl.py
+-rw-r--r--   0        0        0    25886 2022-09-16 11:19:34.518966 valjean-0.9.0/valjean/javert/plot_repr.py
+-rw-r--r--   0        0        0    16361 2022-09-16 11:19:34.518966 valjean-0.9.0/valjean/javert/representation.py
+-rw-r--r--   0        0        0        0 2022-09-16 11:19:34.518966 valjean-0.9.0/valjean/javert/resources/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-16 11:19:34.518966 valjean-0.9.0/valjean/javert/resources/rst/__init__.py
+-rw-r--r--   0        0        0      846 2022-09-16 11:19:34.518966 valjean-0.9.0/valjean/javert/resources/rst/conf.py.template
+-rw-r--r--   0        0        0       38 2022-09-16 11:19:34.518966 valjean-0.9.0/valjean/javert/resources/rst/valjean.css
+-rw-r--r--   0        0        0    32936 2022-09-16 11:19:34.518966 valjean-0.9.0/valjean/javert/rst.py
+-rw-r--r--   0        0        0    32925 2022-09-16 11:19:34.518966 valjean-0.9.0/valjean/javert/table_repr.py
+-rw-r--r--   0        0        0    41439 2022-09-16 11:19:34.518966 valjean-0.9.0/valjean/javert/templates.py
+-rw-r--r--   0        0        0     4439 2022-09-16 11:19:34.518966 valjean-0.9.0/valjean/javert/test_external.py
+-rw-r--r--   0        0        0     5453 2022-09-16 11:19:34.518966 valjean-0.9.0/valjean/javert/test_report.py
+-rw-r--r--   0        0        0     2102 2022-09-16 11:19:34.518966 valjean-0.9.0/valjean/javert/verbosity.py
+-rw-r--r--   0        0        0     2909 2022-09-16 11:19:34.518966 valjean-0.9.0/valjean/path.py
+-rw-r--r--   0        0        0     3496 1970-01-01 00:00:00.000000 valjean-0.9.0/setup.py
+-rw-r--r--   0        0        0     3564 1970-01-01 00:00:00.000000 valjean-0.9.0/PKG-INFO
```

### Comparing `valjean-0.11.0a0/LICENSE` & `valjean-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `valjean-0.11.0a0/LICENSE_fr` & `valjean-0.9.0/LICENSE_fr`

 * *Files identical despite different names*

### Comparing `valjean-0.11.0a0/README.md` & `valjean-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `valjean-0.11.0a0/pyproject.toml` & `valjean-0.9.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -26,20 +26,20 @@
 # the security of their systems and/or data to be ensured and, more generally,
 # to use and operate it in the same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 [build-system]
-requires = ["poetry-core >= 1.0"]
+requires = ["poetry-core >= 1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "valjean"
-version = "0.11.0-alpha.0"
+version = "0.9.0"
 description = "VALidation, Journal d'Évolution et ANalyse"
 authors = ["valjean developers"]
 maintainers = ["valjean developers <valjean-support@cea.fr>"]
 license = "CeCILL-C Free Software License Agreement (CECILL-C)"
 readme = "README.md"
 homepage = "https://github.com/valjean-framework/valjean"
 repository = "https://github.com/valjean-framework/valjean.git"
@@ -57,44 +57,39 @@
 [tool.poetry.urls]
 "Bug tracker" = "https://github.com/valjean-framework/valjean/issues"
 
 [tool.poetry.scripts]
 valjean = "valjean.cambronne.main:main"
 
 [tool.poetry.dependencies]
-python = "^3.6.2"
+python = "^3.6.1"
 pyparsing = "^3.0"
 toml = "^0.10"
-numpy = [{version = "^1.19", python = ">=3.6,<3.7"},
-         {version = "^1.20", python = ">=3.7"}]
+numpy = "^1.19"
 matplotlib = "^3.3"
-scipy = [{version = "^1.5", python = ">=3.6,<3.7"},
-         {version = "^1.6", python = ">=3.7"}]
-h5py = [{version = "~3.1", python = ">=3.6,<3.7"},
-        {version = "^3.2", python = ">=3.7"}]
+scipy = "^1.5"
+h5py = "~3.1"
+
 # dependencies for the [graphviz] extra
 pydot = {version = "^1.4.2", optional = true}
 
 # dependencies for the [dev] extra
-pytest = "^7.0"
-pytest-cov = "^4.0"
-pytest-mpl = "^0.16"
+pytest = "^6.2"
+pytest-cov = "^3.0"
+pytest-mpl = "^0.13"
 pytest-timeout = "^2.0"
-rstcheck = [{version = "^3.3", python = ">=3.6,<3.7"},
-            {version = "^6.0", python = ">=3.7"}]
-Sphinx = "~5.0"
+rstcheck = "^3.3"
+Sphinx = "^4.3"
 sphinx-rtd-theme = "^1.0"
-pylint = [{version = "^2.13", python = ">=3.6,<3.8"},
-          {version = "^3.0", python = ">=3.8"}]
-flake8 = "<6"
-hypothesis = "^6.31"
+pylint = "^2.12"
+flake8 = "^4.0"
+hypothesis = {version = "^6.31", extras = ["numpy"]}
 nbsphinx = "^0.8"
 jupyter-client = "^7.1"
 ipykernel = "^5.5"
-ipython = "!=8.7.0"
 
 [tool.poetry.extras]
 graphviz = ["pydot"]
 dev = [
   "pytest",
   "pytest-cov",
   "pytest-mpl",
@@ -104,15 +99,14 @@
   "sphinx-rtd-theme",
   "pylint",
   "flake8",
   "hypothesis",
   "nbsphinx",
   "jupyter-client",
   "ipykernel",
-  "ipython"
 ]
 
 [tool.pytest.ini_options]
 addopts = "-v -s -ra --doctest-modules"
 norecursedirs = ["data", ".eggs", "doc", ".git", "build", "dist", "*.egg"]
 markers = [
   "slow: marks tests as slow (using runslow argument)",
@@ -121,102 +115,114 @@
 junit_family = "xunit2"
 
 [tool.pylint.basic]
 good-names=["i", "j", "k", "ex", "Run", "x", "y", "z", "on", "do"]
 
 [tool.pylint.message_control]
 disable = [
-  "bad-inline-option", "deprecated-pragma", "import-outside-toplevel",
-  "locally-disabled", "raw-checker-failed", "redefined-outer-name",
-  "suppressed-message", "useless-suppression",
+  "apply-builtin", "backtick", "bad-inline-option", "bad-python3-import",
+  "basestring-builtin", "buffer-builtin", "cmp-builtin", "cmp-method",
+  "coerce-builtin", "coerce-method", "delslice-method", "deprecated-pragma",
+  "deprecated-str-translate-call", "deprecated-string-function",
+  "dict-iter-method", "dict-view-method", "div-method", "eq-without-hash",
+  "exception-message-attribute", "execfile-builtin", "file-builtin",
+  "file-ignored", "filter-builtin-not-iterating", "getslice-method",
+  "hex-method", "idiv-method", "import-outside-toplevel",
+  "import-star-module-level", "indexing-exception", "input-builtin",
+  "intern-builtin", "invalid-str-codec", "locally-disabled", "locally-enabled",
+  "long-builtin", "long-suffix", "map-builtin-not-iterating",
+  "metaclass-assignment", "next-method-called", "no-absolute-import",
+  "nonzero-method", "oct-method", "old-division", "old-ne-operator",
+  "old-octal-literal", "old-raise-syntax", "parameter-unpacking",
+  "print-statement", "raising-string", "range-builtin-not-iterating",
+  "raw-checker-failed", "raw_input-builtin", "rdiv-method",
+  "redefined-outer-name", "reduce-builtin", "reload-builtin", "round-builtin",
+  "setslice-method", "standarderror-builtin", "suppressed-message",
+  "sys-max-int", "unichr-builtin", "unicode-builtin", "unpacking-in-except",
+  "useless-suppression", "using-cmp-argument", "xrange-builtin",
+  "zip-builtin-not-iterating",
   ]
 
 [tool.pylint.typecheck]
 ignored-modules = "py"
 
 [tool.pylint.format]
 max-line-length = 79
 
 [tool.pylint.design]
 max-parents = 8
 max-public-methods = 25
 min-public-methods = 0
-max-args=6
 
 
 [tool.tox]
 legacy_tox_ini = """
 # See doc/src/devs/tox.rst if you have questions about the tox configuration
 [tox]
 minversion = 3.17.0
-requires = virtualenv<20.22.0
-           setuptools<59.0
 # isolated_build is required by poetry
 isolated_build = true
-envlist = py{36,37,38,39,310}
+envlist = py{36,37,38,39}
 
 [tox:jenkins]
 skip_missing_interpreters = true
 
 [testenv]
+whitelist_externals = poetry
 setenv =
         COVERAGE_FILE=.coverage.{envname}
-        PIP_CACHE_DIR={toxworkdir}/{envname}/pip-cache
 description = invoke pytest with coverage, XML output and mpl
-commands = pip install .[dev,graphviz]
-           pytest --basetemp="{toxworkdir}/tmp-{envname}" \
+extras = graphviz
+commands = poetry install -v -E graphviz -E dev --no-root
+           poetry run pytest --basetemp="{toxworkdir}/tmp-{envname}" \
                 --durations=20 --cov-report term-missing \
                 --cov-config "{toxinidir}/.coveragerc" \
                 --cov-report=xml:"{toxworkdir}/coverage-{envname}.xml" \
                 --cov=valjean --junit-xml="{toxworkdir}/pytest-{envname}.xml" \
                 --junit-prefix="{envname}" --mpl \
                 --mpl-results-path="{toxworkdir}/{envname}/mpl_image_compare" \
                 --timeout=30 {posargs}
 
-[testenv:py310]
+[testenv:py39]
 passenv = PYTHONPATH
 
-[testenv:docs-py310]
+[testenv:docs-py39]
 description = invoke sphinx-build to build the HTML docs
 # be nitpicky on the HTML documentation
-passenv = HOME
-commands = pip install .[dev]
-           sphinx-build -d "{toxworkdir}/docs_doctree" -n -E \
+commands = poetry install -v --no-root -E dev
+           poetry run sphinx-build -d "{toxworkdir}/docs_doctree" -n -E \
                 --keep-going -b html -w "{toxworkdir}/sphinx-html-notags.out" \
                 -t no_notebooks "{toxinidir}/doc/src" \
                 "{toxworkdir}/doc/html-notags"
-           sphinx-build -d "{toxworkdir}/docs_doctree" -n -E -W \
+           poetry run sphinx-build -d "{toxworkdir}/docs_doctree" -n -E -W \
                 --keep-going -b html -w "{toxworkdir}/sphinx-html.out" \
                 -t tests "{toxinidir}/doc/src" \
                 "{toxworkdir}/doc/html"
-           sphinx-build -d "{toxworkdir}/docs_doctree" -W \
+           poetry run sphinx-build -d "{toxworkdir}/docs_doctree" -W \
                 --keep-going -b linkcheck -t tests \
                 "{toxinidir}/doc/src" "{toxworkdir}/doc/linkcheck"
 
-[testenv:linting-py310]
+[testenv:linting-py39]
 description = invoke pylint and flake8 on the source package
-commands = pip install .[dev]
-           pylint -f parseable --exit-zero \
+commands = poetry install -v --no-root -E dev
+           poetry run pylint -f parseable --exit-zero \
                 --rcfile "{toxinidir}/pyproject.toml" {posargs}
-           flake8 --config "{toxinidir}/.flake8" \
+           poetry run flake8 --config "{toxinidir}/.flake8" \
                 --exit-zero {posargs}
 
-[testenv:parsing-py310]
+[testenv:parsing-py39]
 description = invoke pytest on the nightly parsing tests
 passenv =
-        PYTHONPATH
         VALJEAN_NIGHTLY_JET4_MONO_PATH
         VALJEAN_NIGHTLY_JET4_PARA_PATH
-        VALJEAN_NIGHTLY_JET4_EVOL_PATH
         VALJEAN_NIGHTLY_V10_2_PATH
         VALJEAN_NIGHTLY_V11_0_PATH
         VALJEAN_NIGHTLY_V11_1_PATH
-        VALJEAN_NIGHTLY_V12_0_PATH
-        VALJEAN_NIGHTLY_V12_1_PATH
         VALJEAN_NIGHTLY_AP3_RATES_PATH
-commands = pip install .[dev,graphviz]
-           pytest --runslow --cov-report term-missing \
+extras = graphviz
+commands = poetry install -v --no-root -E dev
+           poetry run pytest --runslow --cov-report term-missing \
                 --durations=20 --cov-config "{toxinidir}/.coveragerc" \
                 --cov=valjean --mpl \
                 --mpl-results-path="{toxworkdir}/{envname}/mpl_image_compare" \
                 {posargs}
 """
```

### Comparing `valjean-0.11.0a0/valjean/cambronne/commands/env.py` & `valjean-0.9.0/valjean/cambronne/commands/env.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,24 +26,22 @@
 # to use and operate it in the same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 '''Module for the ``env`` subcommand.'''
 
-import logging
+
 from pprint import pprint
 
+from ... import LOGGER
 from ..common import Command
 from ...cosette.env import Env
 
 
-LOGGER = logging.getLogger(__name__)
-
-
 class EnvCommand(Command):
     '''Command class for the ``env`` subcommand.'''
 
     NAME = 'env'
 
     HELP = 'Inspect the content of one or more serialized environment files.'
```

### Comparing `valjean-0.11.0a0/valjean/cambronne/commands/graph.py` & `valjean-0.9.0/valjean/cambronne/commands/graph.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,20 +27,17 @@
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 '''Module for the ``graph`` subcommand.'''
 
 import os
-import logging
 
 from ..common import JobCommand, build_graphs
-
-
-LOGGER = logging.getLogger(__name__)
+from ... import LOGGER
 
 
 class GraphCommand(JobCommand):
     '''Command class for the ``build`` subcommand.'''
 
     NAME = 'graph'
```

### Comparing `valjean-0.11.0a0/valjean/cambronne/commands/run.py` & `valjean-0.9.0/valjean/cambronne/commands/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,28 +26,25 @@
 # to use and operate it in the same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 '''Module for the ``run`` subcommand.'''
 
-import logging
 from pathlib import Path
 
+from ... import LOGGER
 from ..common import JobCommand, read_env, write_env, build_graphs
 from ...cosette.backends.queue import QueueScheduling
 from ...chrono import Chrono
 from ...cosette.scheduler import Scheduler
 from ...cosette.task import TaskStatus
 from ...path import ensure
 
 
-LOGGER = logging.getLogger(__name__)
-
-
 class RunCommand(JobCommand):
     '''Command class for the ``run`` subcommand.'''
 
     NAME = 'run'
 
     HELP = 'Run the tasks defined in a job file.'
```

### Comparing `valjean-0.11.0a0/valjean/cambronne/common.py` & `valjean-0.9.0/valjean/cambronne/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,22 +30,19 @@
 
 '''Common utilities for :program:`valjean` commands.'''
 
 from pathlib import Path
 import argparse
 import sys
 import inspect
-import logging
 
 from ..cosette.env import Env
 from ..cosette.depgraph import DepGraph
 from ..cosette.task import close_dependency_graph
-
-
-LOGGER = logging.getLogger(__name__)
+from .. import LOGGER
 
 
 class Command:
     '''Base class for all :program:`valjean` subcommands.'''
 
     ALIASES = ()
 
@@ -66,15 +63,16 @@
         kwargs[key] = value
 
 
 class JobCommand(Command):
     '''Base class for all :program:`valjean` subcommands that take a job file
     and job arguments.'''
 
-    def register(self, parser):
+    @staticmethod
+    def register(parser):
         '''Add the `job_file` and `job_args` positional arguments to the
         parser.'''
         parser.add_argument('job_file', action='store', metavar='JOB_FILE',
                             help='path to the job file')
         parser.add_argument('job_args', metavar='JOB_ARG', nargs='*',
                             help='positional arguments that will be passed to '
                             'the job() function; multiple arguments may be '
```

### Comparing `valjean-0.11.0a0/valjean/cambronne/main.py` & `valjean-0.9.0/valjean/cambronne/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,22 +33,19 @@
 import sys
 import argparse
 import pkgutil
 import importlib
 import logging
 
 from . import commands
-from .. import LOG_FILE_FORMAT, __version__
+from .. import LOGGER, LOG_FILE_FORMAT, __version__
 from ..config import Config
 from ..path import ensure
 
 
-LOGGER = logging.getLogger(__name__)
-
-
 def main(argv=None):
     '''Main entry point for the :program:`valjean` executable.'''
     if argv is None:
         argv = sys.argv[1:]
     LOGGER.debug('arguments: %s', argv)
 
     parser = make_parser()
```

### Comparing `valjean-0.11.0a0/valjean/chrono.py` & `valjean-0.9.0/valjean/chrono.py`

 * *Files identical despite different names*

### Comparing `valjean-0.11.0a0/valjean/config.py` & `valjean-0.9.0/valjean/config.py`

 * *Files identical despite different names*

### Comparing `valjean-0.11.0a0/valjean/cosette/backends/queue.py` & `valjean-0.9.0/valjean/cosette/backends/queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,17 +39,15 @@
 import logging
 import time
 from queue import Queue
 from functools import partial
 
 from ..task import TaskStatus
 from ...chrono import Chrono
-
-
-LOGGER = logging.getLogger(__name__)
+from ... import LOGGER
 
 
 class QueueScheduling:
     '''The default scheduling backend.
 
     Uses :mod:`threading` and :mod:`queue` to handle concurrent execution of
     tasks.
@@ -254,15 +252,15 @@
             LOGGER.debug('worker %s: starting', self.name)
             while True:
                 task = self.queue.get()
                 if task is None:
                     LOGGER.debug('worker %s: exiting', self.name)
                     break
                 LOGGER.debug('worker %s: got task %s', self.name, task)
-                LOGGER.note('task %s starts', task)
+                LOGGER.info('task %s starts', task)
 
                 start = time.time()
                 try:
                     task_result = task.do(self.env, self.config)
                 except Exception as ex:  # pylint: disable=broad-except
                     LOGGER.exception('task %s on worker %s failed with the '
                                      'following exception:\n%s',
@@ -275,15 +273,15 @@
                         LOGGER.error('expected an (env_update, status) pair '
                                      'from task %s, got None', task.name)
                         self.env.set_failed(task)
                     else:
                         env_update, status = task_result
                         LOGGER.debug('worker %s: task %s completed '
                                      'with status %s', self.name, task, status)
-                        LOGGER.note('task %s completed with status %s',
+                        LOGGER.info('task %s completed with status %s',
                                     task, status)
                         LOGGER.debug('worker %s: proposed environment update: '
                                      '%s', self.name, env_update)
                         self.env.set_status(task, status)
                         self.env.apply(env_update)
                 end = time.time()
                 self.env.set_start_end_clock(task, start=start, end=end)
```

### Comparing `valjean-0.11.0a0/valjean/cosette/code.py` & `valjean-0.9.0/valjean/cosette/code.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,27 +139,25 @@
 import logging
 
 from ..path import ensure
 from ..chrono import Chrono
 from .run import run
 from .task import TaskStatus
 from .pythontask import PythonTask
-
-
-LOGGER = logging.getLogger(__name__)
+from .. import LOGGER
 
 
 class CheckoutTask(PythonTask):
     '''Task to check out code from a version-control system.  The actual code
     checkout is performed when the task is executed.
     '''
 
+    # pylint: disable=too-many-arguments
     def __init__(self, name, *, repository, checkout_root=None, log_root=None,
                  flags=None, ref=None, vcs='git', deps=None, soft_deps=None):
-        # pylint: disable=too-many-arguments
         '''Construct a :class:`CheckoutTask`.
 
         :param str name: The name of this task.
         :param str checkout_root: The directory where the code will be checked
                                   out, or `None` for the configuration default.
         :param str repository: The repository for checkout.
         :param str log_root: The path to the log directory, or `None` for the
@@ -252,18 +250,18 @@
 
 
 class BuildTask(PythonTask):
     '''Task to build an existing source tree. The build is actually performed
     when the task is executed.
     '''
 
+    # pylint: disable=too-many-arguments
     def __init__(self, name, source, *, build_root=None, log_root=None,
                  targets=None, build_system='cmake', configure_flags=None,
                  build_flags=None, deps=None, soft_deps=None):
-        # pylint: disable=too-many-arguments
         '''Construct a :class:`BuildTask`.
 
         :param str name: The name of this task.
         :param str source: The path to the directory containing the sources, or
                            a :class:`CheckoutTask` object (in which case the
                            checkout directory will be assumed to contain the
                            sources).
```

### Comparing `valjean-0.11.0a0/valjean/cosette/depgraph.py` & `valjean-0.9.0/valjean/cosette/depgraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,25 +275,22 @@
     TypeError: 'int' object is not iterable
 
   Here ``1`` is not iterable, and the test crashed. However, if your graph
   nodes happen to be iterable, the :class:`DepGraph` constructor will not
   crash, but you will not get what you expect.
 '''
 
-import logging
 import itertools
 import copy
 import enum
 from .rlist import RList
+from .. import LOGGER
 from ..chrono import Chrono
 
 
-LOGGER = logging.getLogger(__name__)
-
-
 class DepGraphError(Exception):
     '''An exception raised by :class:`DepGraph`.'''
 
 
 class DepGraph:
     '''A dependency graph.
```

### Comparing `valjean-0.11.0a0/valjean/cosette/env.py` & `valjean-0.9.0/valjean/cosette/env.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,25 +99,22 @@
     ...     if env.is_done(quest):
     ...         env.set_skipped(quest)
     >>> env.atomically(modify_task1)
     >>> env.is_skipped(quest)
     True
 """
 
-import logging
 import threading
 import pickle
 from collections.abc import MutableMapping
 
+from .. import LOGGER
 from .task import TaskStatus
 
 
-LOGGER = logging.getLogger(__name__)
-
-
 class EnvError(Exception):
     '''An error that may be raised by the :class:`~Env` class.'''
 
 
 def _add_enum_accessors(enum):
     '''Dynamically instantiate is_* and set_* methods for the :class:`Env`
     class, based on the values of the :class:`~.TaskStatus` enum.
```

### Comparing `valjean-0.11.0a0/valjean/cosette/pythontask.py` & `valjean-0.9.0/valjean/cosette/pythontask.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,20 +261,17 @@
     /.../output
 
 
 Module API
 ----------
 '''
 
-import logging
 import copy
 from .task import Task, TaskStatus
-
-
-LOGGER = logging.getLogger(__name__)
+from .. import LOGGER
 
 
 class TaskException(Exception):
     '''An exception that can be raised by any functions wrapped in
     :class:`PythonTask`. It causes the task to fail. A reason can be specified
     in the constructor.'''
 
@@ -284,17 +281,17 @@
         :param str reason: why this exception was raised.'''
         super().__init__()
         self.because = reason
 
 
 class PythonTask(Task):
     '''Task that executes specified Python code.'''
+
     def __init__(self, name, func, *, args=None, kwargs=None,
                  env_kwarg=None, config_kwarg=None, deps=None, soft_deps=None):
-        # pylint: disable=too-many-arguments
         '''Initialize the task with a function, a tuple of arguments and a
         dictionary of kwargs.
 
         :param str name: The name of the task.
         :param func: A function to be executed.
         :param tuple args: A tuple of positional arguments to `func`, or `None`
                            if none are required.
```

### Comparing `valjean-0.11.0a0/valjean/cosette/rlist.py` & `valjean-0.9.0/valjean/cosette/rlist.py`

 * *Files identical despite different names*

### Comparing `valjean-0.11.0a0/valjean/cosette/run.py` & `valjean-0.9.0/valjean/cosette/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,27 +209,24 @@
 
 Module API
 ==========
 '''
 
 import os
 import shlex
-import logging
 from functools import partial
 from subprocess import call
 
+from .. import LOGGER
 from ..chrono import Chrono
 from ..path import ensure, sanitize_filename
 from .task import TaskStatus, det_hash
 from .pythontask import PythonTask
 
 
-LOGGER = logging.getLogger(__name__)
-
-
 # The following functions are helpers for RunTask, but they may be used
 # elsewhere, too
 def run(clis, stdout, stderr, **subprocess_args):
     '''Run the given command lines and capture their stdout/stderr.
 
     Execution stops at the first failure (result value != 0).
 
@@ -340,16 +337,16 @@
                          deps=deps, soft_deps=soft_deps,
                          env_kwarg='env', config_kwarg='config')
         LOGGER.debug('Created %s task %r', self.__class__.__name__, self.name)
         LOGGER.debug('  - deps = %s', deps)
         LOGGER.debug('  - soft_deps = %s', soft_deps)
         LOGGER.debug('  - subprocess_args = %s', subprocess_args)
 
+    # pylint: disable=unused-argument
     def run_task(self, clis_closure, name, **subprocess_args):
-        # pylint: disable=unused-argument
         '''Execute the specified command and wait for its completion.
 
         On completion, this method proposes the following updates to the
         environment::
 
             env[task.name]['clis'] = clis
             env[task.name]['return_codes'] = return_codes
@@ -364,16 +361,16 @@
         respectively the captured standard output and standard error streams.
 
         :param Env env: The task environment.
         :param config: The configuration object.
         :type config: Config or None
         :returns: The proposed environment update.
         '''
+        # pylint: disable=too-many-locals
         def runner(*, env, config, name, clis_closure, subprocess_args):
-            # pylint: disable=too-many-locals
             '''Actually run the command lines.'''
             from pathlib import Path
 
             clis = clis_closure(env, config)
             output_dir = Path(config.query('path', 'output-root'),
                               sanitize_filename(name))
             stdout_path, stderr_path = make_cap_paths(output_dir)
@@ -404,15 +401,14 @@
 class RunTaskFactory:
     '''Create multiple tasks from the same executable without even breaking a
     sweat.'''
 
     @classmethod
     def _generic_clis_closure(cls, executable, *, env, config, default_args,
                               extra_args, **kwargs):
-        # pylint: disable=too-many-arguments
         cli = [executable]
         cli.extend(arg.format(env=env, config=config, **kwargs)
                    for arg in default_args)
         cli.extend(extra_args)
         return [cli]
 
     @classmethod
```

### Comparing `valjean-0.11.0a0/valjean/cosette/scheduler.py` & `valjean-0.9.0/valjean/cosette/scheduler.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,25 +47,23 @@
    ...     })
 
    >>> from valjean.cosette.scheduler import Scheduler
    >>> s = Scheduler(hard_graph=g)
    >>> env = s.schedule()  # executes the tasks in the correct order
 '''
 
-import logging
+
 from .depgraph import DepGraph
 from .backends.queue import QueueScheduling
 from .env import Env
 from ..chrono import Chrono
+from .. import LOGGER
 from ..config import Config
 
 
-LOGGER = logging.getLogger(__name__)
-
-
 class SchedulerError(Exception):
     '''An error that may be raised by the :class:`Scheduler` class.'''
 
 
 class Scheduler:
     '''Schedule a number of tasks.
 
@@ -105,15 +103,15 @@
         with Chrono() as chrono:
             self.hard_graph = hard_graph.copy()
         LOGGER.info('hard graph copied in %s seconds', chrono)
         with chrono:
             self.hard_graph.flatten()
         LOGGER.info('hard graph flattened in %s seconds', chrono)
         with chrono:
-            self.full_graph = hard_graph + soft_graph
+            self.full_graph = (hard_graph + soft_graph)
         LOGGER.info('full graph computed in %s seconds', chrono)
         with chrono:
             self.full_graph.flatten()
         LOGGER.info('full graph flattened in %s seconds', chrono)
 
         # make sure that all nodes appear in the hard graph
         for node in self.full_graph.nodes():
```

### Comparing `valjean-0.11.0a0/valjean/cosette/task.py` & `valjean-0.9.0/valjean/cosette/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,18 +55,16 @@
 on task `B`, it means that `A` will not start before `B`'s termination, but it
 makes sense to run `A` even if `B` fails.
 '''
 
 import enum
 import json
 from abc import ABC, abstractmethod
-import logging
 
-
-LOGGER = logging.getLogger(__name__)
+from .. import LOGGER
 
 
 #: Enumeration for the task status. The possible values are:
 #:
 #: * ``WAITING`` (the task is waiting to be scheduled)
 #: * ``PENDING`` (the task is under execution)
 #: * ``DONE`` (the task was executed and it succeeded)
```

### Comparing `valjean-0.11.0a0/valjean/cosette/use.py` & `valjean-0.9.0/valjean/cosette/use.py`

 * *Files 1% similar despite different names*

```diff
@@ -571,24 +571,21 @@
     { rank=same slurp_task check_stripped_task run_task strip_task }
 
 
 Module API
 ==========
 '''
 
-import logging
 from pathlib import Path
 from functools import update_wrapper
 
 from .task import TaskStatus
 from ..path import ensure, sanitize_filename
 from .pythontask import PythonTask
-
-
-LOGGER = logging.getLogger(__name__)
+from .. import LOGGER
 
 
 def from_env(*, env, task_name, key):
     '''Helper function to extract a value from the environment for argument
     injection.
 
     :param env: the environment.
@@ -625,15 +622,14 @@
 
     _CACHE = {}
     _USE_CACHING = True
 
     @classmethod
     def from_func(cls, *, func, task, key='result', kwarg=None,
                   deps_type='hard', serialize=False):
-        # pylint: disable=too-many-arguments
         '''Create a :class:`Use` from a function.
 
         :param func: a function or a callable object.
         :param task: the task whose result should be injected as an argument to
             `func`.
         :type task: :class:`~.Task`
         :param str key: the name of the key that contains the task result in
```

### Comparing `valjean-0.11.0a0/valjean/dyn_import.py` & `valjean-0.9.0/valjean/dyn_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,19 +28,17 @@
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 '''This module contains somme common utility functions for dynamically
 importing Python source files as modules.'''
 
 import sys
-import logging
 from pathlib import Path
 
-
-LOGGER = logging.getLogger(__name__)
+from . import LOGGER
 
 
 def split_module_path(file_name):
     '''Split a path to a Python module into a path and a module name.
 
     :param path: A path to a Python file.
     :type path: str or :term:`path-like object`
```

### Comparing `valjean-0.11.0a0/valjean/eponine/apollo3/hdf5_picker.py` & `valjean-0.9.0/valjean/eponine/apollo3/hdf5_picker.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,28 +119,25 @@
   output folder, isotope can be precised if needed
 * :meth:`Picker.nb_anisotropies`: number of anisotropies available for a given
   result for the considered isotope in its zone and output
 * :meth:`Picker.local_names`: list of names of the local values stored in a
   given zone from a given output folder
 '''
 
-import logging
 from functools import lru_cache
 from collections import OrderedDict
 import h5py
 import numpy as np
 
+from ... import LOGGER
 from ...chrono import Chrono
 from ..dataset import Dataset
 from ...cosette.rlist import RList
 
 
-LOGGER = logging.getLogger(__name__)
-
-
 class Picker:
     '''Pick selected values from an Apollo3 HDF5 file.'''
 
     CACHE_SIZE = 512
 
     def __init__(self, fname, error_value=np.nan):
         '''Initialize the :class:`Picker` object and read the HDF5 file.
@@ -280,18 +277,18 @@
         '''
         error = np.full_like(
             data, self.error_value,
             dtype=(float if np.isnan(self.error_value) else data.dtype))
         if not bins:
             return Dataset(value=data, error=error, what=name.lower())
         if 'anisotropies' in bins:
-            nb_groups = len(bins['groups'])
-            nb_aniso = len(bins['anisotropies'])
-            return Dataset(value=data.reshape(nb_aniso, nb_groups),
-                           error=error.reshape(nb_aniso, nb_groups),
+            ngroups = len(bins['groups'])
+            naniso = len(bins['anisotropies'])
+            return Dataset(value=data.reshape(naniso, ngroups),
+                           error=error.reshape(naniso, ngroups),
                            what=name.lower(), bins=bins)
         if 'incident neutron groups' in bins:
             nb_groups = len(bins['groups'])
             nb_incg = len(bins['incident neutron groups'])
             return Dataset(value=data.reshape(nb_incg, nb_groups),
                            error=error.reshape(nb_incg, nb_groups),
                            what=name.lower(), bins=bins)
```

### Comparing `valjean-0.11.0a0/valjean/eponine/apollo3/hdf5_reader.py` & `valjean-0.9.0/valjean/eponine/apollo3/hdf5_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,19 +66,16 @@
     │            │               └─ ZONENAME[NZONE]
     │            ├─ geometry_id2 ┄
     │            ┆
     │            ┆
     │            └─ geometry_idNGEO ┄
     │
     ├─ output_id1 ─┬─ totaloutput ─┬─ KEFF (float)
-    │              │               ├─ (KINF (float))
     │              │               ├─ (ABSORPTION[NG])
-    │              │               ├─ (CURRENT[NG])
     │              │               ├─ (FLUX[NG])
-    │              │               ├─ (MIGRATIONAREA (float))
     │              │               ├─ (PRODUCTION[NG])
     │              │               ├─ (NVAL)
     │              │               ├─ (LOCALVALUE[NVAL])
     │              │               ├─ (LOCALNAME[NVAL])
     │              │               └─ (localvalue) ─┬─ LOCALNAME[NVAL]
     │              │                                ├─ value_id1
     │              │                                ├─ value_id2
@@ -117,15 +114,15 @@
 ``zone_id`` folder names appear as values in the ZONENAME dataset in the
 geometry group, and they are arbitrary strings (chosen by the user in the
 Apollo3 case). ``VOLUME`` stores the volumes (in cm³) of the zones, if needed
 later for normalisation for example. Most physics quantities are given on
 ``NG`` energy groups but the group bounds are not stored in the file. Some
 quantities are given as a function of energy groups and anisotropy. The order
 of the anisotropy development is available in the ``'info'`` group, possibly in
-the ``'isotope_id`` one. Current and surfacic flux (under ``'totaloutput'``)
+the ``'isotope_id`` one. Current and surfacic flux (under ``'totaloutput'``
 have a ``surface id`` component in addition to energy groups.
 
 Some files can also contain custom values or user values, especially in some
 cases the standard structure does not appear at all (no ``zone_id`` or
 ``totaloutput`` folder) but directly local values:
 
 .. code-block::
@@ -201,22 +198,20 @@
 '''
 
 from collections import OrderedDict
 import logging
 import h5py
 import numpy as np
 
+from ... import LOGGER
 from ...chrono import Chrono
 from ..browser import Browser
 from ..dataset import Dataset
 
 
-LOGGER = logging.getLogger(__name__)
-
-
 def hdf_to_browser(*args, **kwargs):
     '''Build a :class:`~valjean.eponine.browser.Browser` from an Apollo3 HDF5
     output.
 
     :param args: other arguments to be passed to :class:`Reader` constructor
     :param kargs: keyword arguments to be passed to :class:`Reader` constructor
     :returns: Browser
@@ -369,14 +364,15 @@
     '''
     if 'LOCALNAME' in val:
         return extract_localvalues(val['LOCALNAME'], val['LOCALVALUE'], error)
     rlist = []
     locval = 'localvalue'
     lkeys = [e.decode('UTF-8').strip()
              for e in val[locval]['LOCALNAME'][...]]
+    print('local value')
     rlist = [{'result_name': k,
               'results': hdfdataset_to_dataset(val[locval][k], k, error)}
              for k in lkeys]
     return rlist
 
 
 def extract_localvalues(lnames, lvals, error):
@@ -487,15 +483,15 @@
     * number of anisotropies (for isotopes reaction rates)
     * number of surfaces (for current and surface flux)
 
     :param h5py.Group data: `info` block from `output_*`
     :rtype: dict
     :returns: dictionary of all possible number of bins
     '''
-    if nres in ('KEFF', 'KINF', 'MIGRATIONAREA'):
+    if nres in ('KEFF', 'KINF'):
         return None
     data = vres[...]
     if ngroups == data.size:
         return OrderedDict([('groups', np.arange(ngroups))])
     if nres == 'SURFFLUX':
         return OrderedDict([('groups', np.arange(ngroups)),
                             ('surfaces', np.arange(nsurfaces))])
```

### Comparing `valjean-0.11.0a0/valjean/eponine/browser.py` & `valjean-0.9.0/valjean/eponine/browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,20 +196,17 @@
     valjean.eponine.browser.NoItemBrowserError: No item corresponding to the \
 selection.
 
 Module API
 ----------
 '''
 
-import logging
 from collections import defaultdict
 from collections.abc import Mapping, Container
-
-
-LOGGER = logging.getLogger(__name__)
+from .. import LOGGER
 
 
 def _make_defaultdict_set():
     '''The sole purpose of this function is to give a name to the defaultdict
     factory in :meth:`Index.index`. Without a name, the :class:`Index` class
     cannot be serialized by :mod:`pickle`.
     '''
```

### Comparing `valjean-0.11.0a0/valjean/eponine/dataset.py` & `valjean-0.9.0/valjean/eponine/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -708,20 +708,17 @@
 True
 >>> np.ma.is_masked(sds.error)
 True
 >>> np.sum(sds.value) == 42
 True
 '''
 # pylint: enable=trailing-whitespace
-import logging
 from collections import OrderedDict
 import numpy as np
-
-
-LOGGER = logging.getLogger(__name__)
+from .. import LOGGER
 
 
 class Dataset:
     '''Common class for data from all codes.
 
     For the moment, units are not treated (removed).
 
@@ -729,14 +726,15 @@
 
         Think about units. Possibility: using a units package from scipy.
 
     .. todo::
 
         How to deal with bins of N values (= center of bins)
     '''
+
     def __init__(self, value, error, *, bins=None, name='', what=''):
         '''Dataset class initialization.
 
         :param value: array of N dimensions representing the values
         :type value: int or float or numpy.ndarray or numpy.generic
         :param error: array of N dimensions representing the **absolute**
           errors
```

### Comparing `valjean-0.11.0a0/valjean/eponine/tripoli4/common.py` & `valjean-0.9.0/valjean/eponine/tripoli4/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -600,19 +600,18 @@
 '''
 
 import logging
 from abc import ABC, abstractmethod
 from collections import OrderedDict
 from io import StringIO
 import numpy as np
+from ... import LOGGER
 from .data_convertor import bins_reduction
 
 
-LOGGER = logging.getLogger(__name__)
-
 # get profile from globals (cleaner)
 if 'profile' not in globals()['__builtins__']:
     def profile(func):
         '''No memory profiling if "mem" not in arguments of the command line.
         '''
         return func
 
@@ -1763,24 +1762,24 @@
     Selections are done like in the default score cases.
     '''
     keys = ('score', 'sigma')
     tlist = []
     loctype = list(res['adj_res'].keys())[0]
     index = loctype.split('_')[2:]
     adjres = res.pop('adj_res')
-    if len(adjres.as_dict()) != 1:
+    if len(adjres.asDict()) != 1:
         LOGGER.warning("Issue: more than one key for adjoint result")
     ubatch = res.get('used_batches', None)
     # deal with units (stored in all results)
     units = {}
     # check names of units
     if 'uscore' in res:
         units['uscore'] = res.pop('uscore')
         units['usigma'] = res.pop('usigma')
-    assert len(res.as_dict()) == 1, \
+    assert len(res.asDict()) == 1, \
         "used_batches should be the only remaining key in the dict"
     assert ubatch is not None, "used batches should not the None"
     for ires in adjres[loctype]:
         mydict = {'used_batches_res': ubatch}
         mydict[index[0]] = ires[0]
         if len(ires) == 1:
             mydict['generic_res'] = {
@@ -2209,21 +2208,14 @@
     Bins are filled in an :class:`collections.OrderedDict` always containing
     the 3 keys ``'einc', 'e', 'mu'`` in the order of the bins in the
     :obj:`numpy.ndarray`.
     '''
     lres = res['sensit_res']
     thelist = []
     for ires in lres:
-        if 'reaction_rate' in ires:
-            resdict = {'used_batches_res': res['used_batches']}
-            resdict['reaction_rate_ratio_res'] = (
-                ires['reaction_rate'].as_dict())
-            resdict['sensitivity_ref'] = 'reaction_rate_ratio'
-            thelist.append(resdict)
-            continue
         itype = ''.join(ires['sensitivity_type'])
         for iindex in ires['res']:
             sensidb = SensitivityDictBuilder(
                 ['score', 'sigma'],
                 _get_sensitivity_bins(iindex['vals']))
             if 'energy_integrated' in iindex:
                 sensidb.add_array('integrated_res', ['score', 'sigma'],
@@ -2233,15 +2225,15 @@
             sensidb.convert_bins_to_increasing_arrays()
             if 'units' in res:
                 sensidb.units['score'] = res['units'][0]['uscore']
             datadict = {
                 'array': sensidb.arrays['default'],
                 'bins': sensidb.bins,
                 'units': sensidb.units}
-            resdict = iindex['charac'].as_dict()
+            resdict = iindex['charac'].asDict()
             resdict['sensitivity_type'] = itype
             resdict['sensitivity_spectrum_res'] = datadict
             resdict['integrated_res'] = sensidb.arrays['integrated_res']
             resdict['used_batches_res'] = res['used_batches']
             thelist.append(resdict)
     return thelist
 
@@ -2278,15 +2270,15 @@
     def fill_arrays_and_bins(self, data):
         '''Fill arrays and bins for spherical harmonics results.
 
         :param data: parsed result from *pyparsing*
         '''
         for res in data:
             score = self.rev_correspondence_table[res['score_name'][0]]
-            spaceb = res['score'][0]['space'].as_list()
+            spaceb = res['score'][0]['space'].asList()
             for iie, spres in enumerate(res['score'][0]['vpspace']):
                 if ((len(self.bins['ie']) < self.arrays[score].shape[3]
                      and 'incident_energy' in spres)):
                     self.bins['ie'].append(spres['incident_energy'][0])
                 for ioe, ieres in enumerate(spres['vpie']):
                     if len(self.bins['e']) < self.arrays['default'].shape[4]:
                         self.bins['e'].append(ieres['energy'][0])
@@ -2396,15 +2388,15 @@
         elif score in ('scattering_matrix',):
             shdb.add_array(score, colnames, tbins)
         else:
             shdb.add_array(score, colnames, tbins[:3] + [1] + tbins[4:])
     shdb.fill_space_bins()
     shdb.fill_moments_bins()
     shdb.fill_arrays_and_bins(res['res'])
-    shdb.add_last_bins(res['res'][-1].as_dict())
+    shdb.add_last_bins(res['res'][-1].asDict())
     shdb.convert_bins_to_increasing_arrays()
     shlist = []
     for narr, arr in shdb.arrays.items():
         if narr == 'default':
             continue
         shlist.append({
             'spherical_harmonics_res': {
```

### Comparing `valjean-0.11.0a0/valjean/eponine/tripoli4/data_convertor.py` & `valjean-0.9.0/valjean/eponine/tripoli4/data_convertor.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,21 +28,18 @@
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 '''This module converts Tripoli-4 data from parsing in
 :class:`~valjean.eponine.dataset.Dataset`.
 '''
 
-import logging
 from collections import OrderedDict
 import numpy as np
 from ..dataset import Dataset
-
-
-LOGGER = logging.getLogger(__name__)
+from ... import LOGGER
 
 
 def bins_reduction(def_bins, reduced_dims):
     '''Reduce number of bins for integrated results (on one or more dimension).
 
     For the reduced dimensions, all the bounds are suppressed except the first
     and the last one. This is also the case if they represent center of bins.
@@ -75,14 +72,15 @@
         else:
             LOGGER.debug("Keep bins from 'array'.")
             bins[_bin] = def_bins[_bin]
     return bins
 
 
 def special_array(array, score, bins, array_key='array', name='', what=''):
+    # pylint: disable=too-many-arguments
     '''Convert special arrays in :class:`~.dataset.Dataset`.
 
     These special cases are typically vov results or uncertainty spectrum
     associated to a perturbation result. No error is associated to the score in
     that case. Bins are given by the spectrum.
 
     :param dict array: result
@@ -98,14 +96,15 @@
     return Dataset(
         the_array.copy(), np.full_like(the_array, np.nan), bins=bins,
         name=name, what=what)
 
 
 def array_result(farray_res, res_type, name='', what='', array_key='array',
                  score='score'):
+    # pylint: disable=too-many-arguments
     '''Conversion of arrays in :class:`~.dataset.Dataset`.
 
     :param dict farray_res: results dictionary containing ``res_type`` key
     :param str res_type: result type, like ``'spectrum'``, ``'mesh'``
     :param str array_key: default=``'array'`` but it can be an integrated
         array for example, should be a key inside ``farray_res``
     :param str name: name of dataset
@@ -129,23 +128,25 @@
         array_res[array_key][score].copy(),
         array_res[array_key]['sigma'] * array_res[array_key][score] * 0.01,
         bins=bins, name=name, what=what)
 
 
 def masked_array_result(farray_res, res_type, name='', what='',
                         array_key='array', score='score'):
+    # pylint: disable=too-many-arguments
     '''Mask invalid (``np.nan`` and ``np.inf``) values.'''
     ards = array_result(farray_res, res_type, name=name, what=what,
                         array_key=array_key, score=score)
     mask = np.ma.masked_invalid(ards.value).mask  # pylint: disable=no-member
     return ards.mask(mask)
 
 
 def integrated_result(result, res_type='integrated', name='', what='',
                       score='score', sigma='sigma'):
+    # pylint: disable=too-many-arguments
     '''Conversion of generic score (or energy integrated result) in
     :class:`~valjean.eponine.dataset.Dataset`.
 
     Bins are squeezed according to the integrated dimension obtained from
     another array stored in the same result. Default full arrays are
     `'spectrum'` and `'mesh'`. A case is also foreseen for uncertainty
     results (in perturbation cases).
@@ -213,14 +214,15 @@
     res = result[res_type]
     error = 0 if np.issubdtype(res.dtype, np.integer) else np.nan
     return Dataset(res, np.full(res.shape, error), name=name, what=what)
 
 
 def result_with_error(result, res_type, name='', what='',
                       score='score', sigma='sigma'):
+    # pylint: disable=too-many-arguments
     '''Conversion of generic score (or energy integrated result) in
     :class:`~valjean.eponine.dataset.Dataset`.
 
     :param dict result: results dictionary containing ``res_type`` key
     :param str res_type: should be 'generic'
     :param str name: name of dataset
     :param str what: what attribute of dataset
@@ -240,14 +242,15 @@
     return Dataset(intres[score].copy(),
                    intres[sigma] * intres[score] * 0.01,
                    name=name, what=what)
 
 
 def unbinned_result(result, res_type, name='', what='', score=None,
                     sigma=None):
+    # pylint: disable=too-many-arguments
     '''Conversion of all unbinned results in
     :class:`~valjean.eponine.dataset.Dataset`.
 
     :dict result: results dictionary containing ``res_type`` key
     :param str res_type: key in result allowing access to the desired quantity
     :param str name: name of dataset
     :param str what: what attribute of dataset
```

### Comparing `valjean-0.11.0a0/valjean/eponine/tripoli4/depletion.py` & `valjean-0.9.0/valjean/eponine/tripoli4/depletion.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,24 +89,21 @@
 Some helper methods provide the list of compositions, the list of isotopes in a
 given composition or the reaction rates associated to a given isotope in a
 given composition.
 '''
 
 # pylint: disable=no-member
 
-import logging
 import re
 from collections import OrderedDict
 from pathlib import Path
 import pkg_resources as pkg
 import numpy as np
 from ..dataset import Dataset
-
-
-LOGGER = logging.getLogger(__name__)
+from ... import LOGGER
 
 
 def title_to_snake_case(word):
     '''Convert `word` from title case to snake case.
 
     >>> title_to_snake_case('ThisIsATitle')
     'this_is_a_title'
@@ -264,21 +261,14 @@
         in the `__t4depletion__` folder to used afterwards.
         '''
         try:
             import ROOT
         except ImportError as ierr:
             LOGGER.error('ROOT needs to be added to PYTHONPATH')
             raise ImportError('ROOT missing') from ierr
-        if all(hasattr(ROOT, cls) for cls in ['DepletedComposition',
-                                              'BurnupResults',
-                                              'MeanBurnupResults']):
-            LOGGER.info('skipping compilation of the ROOT depletion scripts '
-                        'because they are already available')
-            return ROOT
-        LOGGER.info('attempting compilation of the ROOT depletion scripts...')
         ps_fold = 'valjean.eponine.tripoli4.resources.depletion'
         assert pkg.resource_exists(ps_fold, 'DepletedComposition.C')
         assert pkg.resource_exists(ps_fold, 'BurnupResults.C')
         assert pkg.resource_exists(ps_fold, 'MeanBurnupResults.C')
         fname = pkg.resource_filename(ps_fold, 'DepletedComposition.C')
         path_fname = Path(fname)
         ROOT.gROOT.SetMacroPath(str(path_fname.parent))
@@ -288,15 +278,14 @@
                            'be granted.')
             root_build = path_fname.parent / "__t4depletion__"
         ROOT.gSystem.MakeDirectory(str(root_build))
         ROOT.gSystem.SetBuildDir(str(root_build), True)
         ROOT.gROOT.LoadMacro('DepletedComposition.C+')
         ROOT.gROOT.LoadMacro('BurnupResults.C+')
         ROOT.gROOT.LoadMacro('MeanBurnupResults.C+')
-        LOGGER.info('... ROOT depletion scripts have been compiled and loaded')
         return ROOT
 
     @classmethod
     def from_evolution_steps(cls, *fnames, root_build=""):
         '''Initialisation from `evolution.root` files (one per simulation).
 
         :param str fnames: ROOT files
```

### Comparing `valjean-0.11.0a0/valjean/eponine/tripoli4/dump.py` & `valjean-0.9.0/valjean/eponine/tripoli4/dump.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,17 @@
 ``pyparsing.ParseResults``. This main function is called in a
 ``pyparsing.ParseElement.setParseAction`` in :mod:`~grammar`.
 '''
 
 import logging
 from collections import OrderedDict
 import numpy as np
+from ... import LOGGER
 
 
-LOGGER = logging.getLogger(__name__)
 MAX_DEPTH = 0
 MAX_DEPTH_STR = f"MAX_DEPTH = {MAX_DEPTH} reached\n"
 
 
 def array_to_str(array):
     '''Transform :obj:`numpy.ndarray` in condensed string.
```

### Comparing `valjean-0.11.0a0/valjean/eponine/tripoli4/grammar.py` & `valjean-0.9.0/valjean/eponine/tripoli4/grammar.py`

 * *Files 8% similar despite different names*

```diff
@@ -216,29 +216,26 @@
     for the moment to specify the method, it can be obtained from the response
     function itself. Adjoint criticality editions are only done for IFP, this
     may change when the same will be available for Wielandt. Some renaming can
     also be needed.
 
 '''
 
-import logging
-from pyparsing import (Word, Keyword, White, alphas, alphanums, LineEnd,
-                       Suppress, Optional, CaselessKeyword, original_text_for,
-                       Group, OneOrMore, ZeroOrMore, Forward,
-                       token_map, delimited_list, printables, replace_with)
+from pyparsing import (Word, Keyword, White, alphas, alphanums,
+                       Suppress, Optional, LineEnd, CaselessKeyword,
+                       Group, OneOrMore, ZeroOrMore, Forward, originalTextFor,
+                       tokenMap, delimitedList, printables, replaceWith)
 from pyparsing import pyparsing_common as pyparscom
 from . import transform as trans
 from .transform import compose2
 from .dump import dump_in_logger
+from ... import LOGGER
 
-
-LOGGER = logging.getLogger(__name__)
-
-_fnums = pyparscom.fnumber.set_parse_action(token_map(trans.common.FTYPE))
-_inums = pyparscom.number.set_parse_action(token_map(trans.common.ITYPE))
+_fnums = pyparscom.fnumber.setParseAction(tokenMap(trans.common.FTYPE))
+_inums = pyparscom.number.setParseAction(tokenMap(trans.common.ITYPE))
 
 ###################################
 #            KEYWORDS             #
 ###################################
 
 # General keywords
 _integratedres_kw = Keyword("INTEGRATED RESULTS")
@@ -295,32 +292,33 @@
 _spectrumresp_kw = Keyword("SPECTRUM")
 _filters_kw = Keyword("Score filtered by volume")
 
 # Scoring description
 _scoremode_kw = Keyword("scoring mode")
 _scorezone_kw = Keyword("scoring zone")
 _scoremesh_kw = (Keyword("Results on a mesh")
-                 .set_parse_action(replace_with('Mesh')))
+                 .setParseAction(replaceWith('Mesh')))
 _scoremeshinfobins_kw = Keyword("(x,y,z)")
 _scoreallgeom_kw = (Keyword("Results cumulated on all geometry")
-                    .set_parse_action(replace_with('All geometry')))
+                    .setParseAction(replaceWith('All geometry')))
 _scoreallsources_kw = (Keyword("Results cumulated on all sources")
-                       .set_parse_action(replace_with('All sources')))
+                       .setParseAction(replaceWith('All sources')))
 _scorevol_kw = Keyword("Volume")
 _scorevolvol_kw = Keyword("num of volume")
-_scorevolumeunit_kw = Keyword("Volume in")
+_scorevolume_kw = (Keyword("Volume in cm3")
+                   | Keyword('Volume in 1.000000e+00 cm3'))
 _scorevolumeint_kw = (Keyword("The result is integrated over the volume")
                       | Keyword("The result is integrated in volume")
-                      ).set_parse_action(replace_with('volume integrated'))
+                      ).setParseAction(replaceWith('volume integrated'))
 _scorevolumenotint_kw = (
     Keyword("The volume has been provided by the user "
             "(the user requested a score per unit volume)")
     | Keyword("The volume has been calculated by Tripoli-4 "
-              "or provided by the user")).set_parse_action(
-                  replace_with('per unit volume'))
+              "or provided by the user")).setParseAction(
+                  replaceWith('per unit volume'))
 _scorevolsum_kw = Keyword("Volume Sum")
 _scorevolsumvol_kw = Keyword("num of volumes")
 _scorevolumesum_kw = Keyword("Total volume in cm3")
 _scorevolumecell_kw = Keyword("Cell volume in cm3")
 _scoresurf_kw = Keyword("Frontier")
 _scoresurfvol_kw = Keyword("volumes")
 _scoresurface_kw = Keyword("Surface in cm2")
@@ -340,15 +338,14 @@
 
 # Correspondence table (volumes and their names)
 _corresptable_kw = Keyword("Correspondence table between volumes "
                            "ids and names :")
 _vol_kw = CaselessKeyword("Volume")
 
 # KEFF keywords
-_notcvg_exp_kw = Keyword("(invalid keff domain)")
 _fullcomb_kw = Keyword("full combined estimator")
 _bestresdiscbatchs_kw = Keyword("best results are obtained with discarding")
 _correlations_kw = Group(Keyword("estimators")
                          + Keyword("correlations")
                          + Keyword("combined values")
                          + Keyword("combined sigma%"))
 _estimator_kw = Keyword("ESTIMATOR")
@@ -356,17 +353,14 @@
 _warn_combkeff_kw = (
     Keyword("One of the Keffectives is null and should not be")
     + Keyword("Combined Keffectives will not be edited"))
 _warn_fixsourcekeff_kw = (
     Keyword("In FIXED_SOURCES_CRITICITY mode, the keff result")
     + Keyword("is actually an overall multiplication factor "
               "(cf User's Guide)"))
-_parna_likelihood_kw = Keyword("parna likelihood confidence interval (on the "
-                               "mean of M = M' + 1)")
-_parna_inv_cdf_kw = Keyword("inversion of the CDF converged after")
 
 # Time steps
 _timestepnum_kw = Keyword("TIME STEP NUMBER")
 _timestepmin_kw = Keyword("time min. =")
 _timestepmax_kw = Keyword("time max. =")
 
 # Angular zones
@@ -411,15 +405,14 @@
 _nucleus_kw = Keyword("Nucleus :")
 # Perturbation order
 _perturborder_kw = Keyword("Scores are ordered by perturbation index:")
 # Sensitivities
 _sensitivitytypeorder_kw = Keyword("Scores are ordered by type")
 _sensitivityindexorder_kw = Keyword("and index:")
 _sensitivity_kw = Keyword("SENSITIVITY :")
-_sensitivityreactionrate_kw = Keyword("REACTION_RATE_RATIO :")
 _sensitivity_energyint_kw = Keyword("Energy integrated S")
 _sensitivity_incenergy_kw = Keyword("Incident energy interval in MeV:")
 _sensitivity_dircos_kw = Keyword("Direction cosine interval:")
 
 # Variance of variance
 _vovstar_kw = Keyword("variance of variance* :")
 _sensibtomaxval_kw = Keyword("sensibility to maximum value:")
@@ -542,29 +535,25 @@
 _meanweightrestartpart = (Suppress(_meanweightrestartpart_kw)
                           + _fnums('mean_weight_restart_particle'))
 _introelts = (_meanweightleak | _meanweightleakin | _edbatchnum
               | _meanweightrestartpart)
 intro = Group(_sourceintensity + _star_line + OneOrMore(_introelts))('intro')
 
 # Conclusion parser
-_packet_length_warning = Suppress(
-    "* packet length is" + _inums
-    + "(check documentation for conventions about discard and batches)")
 _simutime = Suppress(_simulationtime_kw + ':') + _fnums('simulation_time')
 _exploitime = (Suppress(_exploitationtime_kw + ':')
                + _fnums('exploitation_time'))
 _elapsedtime = Suppress(_elapsedtime_kw + ':') + _fnums('elapsed_time')
-runtime = (Optional(_packet_length_warning)
-           + Group(_simutime | _elapsedtime | _exploitime)('conclu'))
+runtime = Group(_simutime | _elapsedtime | _exploitime)('conclu')
 
 # Response parser
 # Description of the response
 _respfunc = (Suppress(_respfunction_kw + ':')
              + OneOrMore(Word(printables), stopOn=LineEnd())
-             .set_parse_action(' '.join)('response_function'))
+             .setParseAction(' '.join)('response_function'))
 # warning: order matters hier, LineEnd has to be before Optional(Word)
 _respname = (Suppress(_respname_kw + ':')
              + (Suppress(LineEnd())
                 | Optional(Word(printables)('response_name'))))
 _scorename = (Suppress(_scorename_kw + ":")
               + Optional(Word(printables)('score_name')))
 _energysplit = (Suppress(_energysplitname_kw + ':')
@@ -573,38 +562,38 @@
             + Word(printables)('nu_split_name'))
 respdesc = (_respfunc + Optional(_respname) + Optional(_scorename)
             + Optional(_energysplit | _nusplit))
 
 _respfilter = (Suppress(_respfiltered_kw) + _inums('nb_filtered_compos')
                + Suppress(_respfiltcompos_kw + ':')
                + Group(OneOrMore(Word(printables), stopOn=LineEnd()))
-               .set_parse_action(trans.convert_list_to_tuple)
+               .setParseAction(trans.convert_list_to_tuple)
                ('filtered_compositions'))
 
 _particle = (Suppress(_particule_kw + ':')
              + OneOrMore(Word(alphas+','), stopOn=LineEnd())
-             .set_parse_action(' '.join)('particle'))
+             .setParseAction(' '.join)('particle'))
 _incparticle = (Suppress(_incparticle_kw + ':')
                 + Word(alphas)('incident_particle'))
 _noise_equation = (Suppress(_noise_equation_kw + ':')
                    + OneOrMore(Word(alphas), stopOn=LineEnd())
-                   .set_parse_action(' '.join)('noise_equation'))
+                   .setParseAction(' '.join)('noise_equation'))
 # response characteristics written in lower case
 _reactiononnucl = (Suppress(_reactiononnucl_kw + ':')
                    + Word(printables)('reaction_on_nucleus'))
 _temperature = Suppress(_temperature_kw + ':') + _fnums('temperature')
 _composition = (Suppress(_composition_kw + ':')
                 + Word(printables)('composition'))
 _concentration = Suppress(_concentration_kw + ':') + _fnums('concentration')
 _reaction = (Suppress(_reaction_kw)
              + ((Suppress(Word(alphas) + ':')
-                 + Group(delimited_list(_inums, delim='+')))
+                 + Group(delimitedList(_inums, delim='+')))
                 | OneOrMore(Word(alphas), stopOn=LineEnd())
-                .set_parse_action(' '.join))
-             .set_parse_action(trans.convert_list_to_tuple)('reaction'))
+                .setParseAction(' '.join))
+             .setParseAction(trans.convert_list_to_tuple)('reaction'))
 
 
 # Goal: when more than one reaction are required, keep characteristics grouped
 # by particle, reaction, etc.
 def _next_compos(toks):
     if toks.getName() == 'reaction_on_nucleus':
         detail = _temperature | _composition | _concentration | _reaction
@@ -625,44 +614,44 @@
 
 _compodetails = Forward()
 _otherdetails = Forward()
 _compoptions = (_reactiononnucl
                 | _temperature
                 | _composition
                 | _concentration
-                | _reaction).set_parse_action(_next_compos)
+                | _reaction).setParseAction(_next_compos)
 _compodetails << Group(_compoptions + _otherdetails)  # pylint: disable=W0106
-_nuclflags = (OneOrMore(_compodetails).set_parse_action(trans.lod_to_dot)
+_nuclflags = (OneOrMore(_compodetails).setParseAction(trans.lod_to_dot)
               ('compos_details'))
 
 
 # other response characteristics
 _dpatype = (Suppress(_dpatype_kw)
             + OneOrMore(Word(alphas+'-,'), stopOn=LineEnd())
-            .set_parse_action(' '.join)('dpa_type'))
+            .setParseAction(' '.join)('dpa_type'))
 _required = (Suppress(_required_kw)
              + OneOrMore(Word(alphanums+'():'), stopOn=LineEnd())
-             .set_parse_action(' '.join)('required'))
+             .setParseAction(' '.join)('required'))
 _mode = Suppress(_mode_kw) + Word(alphas)('mode')
 _inducedbyint = (Suppress(_inducedbyint_kw)
                  + Group(OneOrMore(_inums))
-                 .set_parse_action(trans.convert_list_to_tuple)
+                 .setParseAction(trans.convert_list_to_tuple)
                  ('induced_by_interation'))
 _notinducedbyint = (Suppress("NOT" + _inducedbyint_kw)
                     + Group(OneOrMore(_inums))
-                    .set_parse_action(trans.convert_list_to_tuple)
+                    .setParseAction(trans.convert_list_to_tuple)
                     ('NOT_induced_by_interation'))
 _fxptcontrib = (OneOrMore(Word(alphas+'()'),
-                          stopOn=_fxptcontrib_kw).set_parse_action(' '.join)
+                          stopOn=_fxptcontrib_kw).setParseAction(' '.join)
                 ('fxpt_contribution')
                 + Suppress(_fxptcontrib_kw))
 _spectrumresp = Suppress(_spectrumresp_kw + ':') + Word(alphas)('spectrum')
 _filters = (Suppress(_filters_kw + ':')
             + Group(OneOrMore(_inums))
-            .set_parse_action(trans.convert_list_to_tuple)
+            .setParseAction(trans.convert_list_to_tuple)
             ('filtered_volumes')
             + Optional(Suppress('With') + Word(alphas+'_')('filter_type')))
 
 
 respcarac = (_respfilter
              | _particle
              | _incparticle
@@ -696,57 +685,51 @@
                            + Optional(_scoremeshinfobins_kw)
                            + Word(alphas)
                            + Word(alphas+'() '))
 _score_meshinfounit_cols = (Suppress(Word(alphas))
                             + _score_meshinfo_cell_unit
                             + _score_meshinfo_volume
                             + Suppress(Word(alphas) + Word(alphas+'() ')))
-_score_mesh = (Optional(Suppress(_scorevolumeunit_kw)
-                        + Word(alphanums+' .^-+')('scoring_zone_volsurf_unit')
-                        + Suppress(':')
+_score_mesh = (Optional(Suppress(_scorevolume_kw + ':')
                         + _fnums('scoring_zone_volsurf'))
                + Optional(Suppress(_scorevolumecell_kw + ':')
                           + _fnums('scoring_zone_cellvol'))
                + _scoremesh_kw('scoring_zone_type') + Suppress(':')
                + (_score_meshinfounit_cols | _score_meshcols)
                + Optional(_score_mesh_unit))
 _score_allgeom = _scoreallgeom_kw('scoring_zone_type')
 _score_allsources = _scoreallsources_kw('scoring_zone_type')
 _score_vol = (_scorevol_kw('scoring_zone_type')
               + Suppress(_scorevolvol_kw + ':')
               + (_inums | Word(printables))('scoring_zone_id')
-              + Suppress(_scorevolumeunit_kw)
-              + Word(alphanums+' .^-+')('scoring_zone_volsurf_unit')
-              + Suppress(':')
+              + Suppress(_scorevolume_kw + ':')
               + _fnums('scoring_zone_volsurf')
               + Optional(_scorevolumeint_kw | _scorevolumenotint_kw)
               ('scoring_zone_details'))
-_score_vol_sum = (
-    (_scorevolsum_kw('scoring_zone_type')
-     + Suppress(_scorevolsumvol_kw + ':')
-     + Group(delimited_list(_inums, delim='+'))('scoring_zone_id')
-     + Suppress(_scorevolumesum_kw + ':')
-     + _fnums('scoring_zone_volsurf')))
+_score_vol_sum = ((_scorevolsum_kw('scoring_zone_type')
+                   + Suppress(_scorevolsumvol_kw + ':')
+                   + Group(delimitedList(_inums, delim='+'))('scoring_zone_id')
+                   + Suppress(_scorevolumesum_kw + ':')
+                   + _fnums('scoring_zone_volsurf')))
 _score_surf = (_scoresurf_kw('scoring_zone_type')
                + Suppress(_scoresurfvol_kw + ':')
-               + Group(delimited_list(_inums
-                                      | Word(printables, excludeChars=',')))
+               + Group(delimitedList(_inums
+                                     | Word(printables, excludeChars=',')))
                ('scoring_zone_id')
                + Optional(Suppress(_scoresurface_kw + ':')
                           + _fnums('scoring_zone_volsurf'))
                + Optional(Suppress(_scoresurfaceint_kw
                                    | _scoresurfacenotint_kw)))
 _score_surf_sum = (
     _scoresurfsum_kw('scoring_zone_type')
     + Suppress(_scoresurfsumfront_kw + ':')
-    + delimited_list(
-        Group(Suppress('(')
-              + delimited_list(Word(printables, excludeChars=',()') | _inums)
-              + Suppress(')')),
-        delim='+')('scoring_zone_id')
+    + delimitedList(Group(Suppress('(')
+                          + delimitedList(Word(printables, excludeChars=',()')
+                                          | _inums)
+                          + Suppress(')')), delim='+')('scoring_zone_id')
     + Suppress(_scoresurfacesum_kw + ':')
     + _fnums('scoring_zone_volsurf'))
 _score_point = (_scorepoint_kw('scoring_zone_type')
                 + Suppress(':')
                 + Group(_fnums + Suppress(',')
                         + _fnums + Suppress(',')
                         + _fnums)('scoring_zone_id'))
@@ -814,33 +797,32 @@
 
 # Default integrated result
 _numdiscbatch = (Suppress(_numbatchs1stdiscarded_kw + ':')
                  + _inums('discarded_batches'))
 _numusedbatch = Suppress(_numbatchsused_kw + ':') + _inums('used_batches')
 _integratedres_name = _integratedres_kw | Word(alphas) + _integratedres_kw
 _integratedres = _fnums('score') + _fnums('sigma')
-_unitsres = (
-    Suppress(_units_kw)
-    + (Word('%').set_parse_action(_set_no_unit_case)
-       | (Word(alphanums+'.^-+ ').set_parse_action(_rm_blanks)('uscore')
-          + Word('%')('usigma'))))
+_unitsres = (Suppress(_units_kw)
+             + (Word('%').setParseAction(_set_no_unit_case)
+                | (Word(alphanums+'.^-+ ').setParseAction(_rm_blanks)('uscore')
+                   + Word('%')('usigma'))))
 # rejection in vov and sensibility cases
 _rejection = (Suppress('[')
-              + OneOrMore(Word(alphanums+'<>.+-')).set_parse_action(' '.join)
+              + OneOrMore(Word(alphanums+'<>.+-')).setParseAction(' '.join)
               ('rejection')
               + Suppress(']'))
 _vovnostar = Suppress(_vov_kw) + Group(_fnums('score'))('vov_res')
 _vovstar = Group(
     Suppress(_vovstar_kw) + _fnums('score')
     + Suppress('[') + _fnums('sigma') + Suppress(']')
     + Optional(_rejection))('vovstar_res')
 _sensibtomaxval = Group(
     Suppress(_sensibtomaxval_kw) + _fnums('max_val')
     + Optional(_rejection))('sensibility_res')
-_vov = _vovnostar | _vovstar + _sensibtomaxval
+_vov = (_vovnostar | _vovstar + _sensibtomaxval)
 # best result
 bestres = (Group(Suppress(_bestresdiscbatchs_kw) + _inums('discarded_batches')
                  + Suppress("batches")
                  + _minus_line
                  + _numusedbatch + _fnums('score') + _fnums('sigma'))
            ('best_result_res'))
 
@@ -853,15 +835,15 @@
                  + Optional(_vov))
 
 genericscoreblock = (Group(Optional(Suppress(_integratedres_name))
                            + ((_numusedbatch
                                + _integratedres
                                + Optional(_unitsres))
                               | _notconverged_kw('not_converged')))
-                     ('generic_res').set_parse_action(trans.group_to_dict))
+                     ('generic_res').setParseAction(trans.group_to_dict))
 
 
 # Time steps
 _timestep = Group(Suppress(_timestepnum_kw + ':') + _inums
                   + _minus_line
                   + Suppress(_timestepmin_kw) + _fnums
                   + Suppress(_timestepmax_kw) + _fnums)('time_step')
@@ -883,15 +865,15 @@
                        + Word(alphanums+'.^-+%') * 4)('units')
 _spectrumbin = _fnums + Suppress('-') + _fnums
 _spectrumcols = Suppress((_spgroupwunit_kw | _spgroup_kw)
                          + _spscore_kw
                          + _spsigma_kw
                          + _spscovlethargy_kw)
 _spectrumvals = (Group(_spectrumbin + _fnums + _fnums + _fnums)
-                 .set_fail_action(trans.fail_spectrum))
+                 .setFailAction(trans.fail_spectrum))
 _spectrum = (Suppress(_spectrum_kw)
              + _numdiscbatch
              + _spectrumcols
              + Optional(_spectrumunits)
              + OneOrMore(_spectrumvals, stopOn=_endtable)('spectrum_vals'))
 spectrumblock = (Group(OneOrMore
                        (Group(OneOrMore(_timestep | _muangzone | _phiangzone)
@@ -917,15 +899,15 @@
 
 
 # Nu spectrum
 _nuspectrumunits = Group(Suppress(_units_kw)
                          + Word(alphanums+'.^-+%') * 3)('units')
 _nuspectrumcols = Suppress(_nusprange_kw + _spscore_kw + _spsigma_kw)
 _nuspectrumvals = (Group(_spectrumbin + _fnums + _fnums)
-                   .set_fail_action(trans.fail_spectrum))
+                   .setFailAction(trans.fail_spectrum))
 _nuspectrum = (Suppress(_nuspectrum_kw)
                + _numdiscbatch
                + _nuspectrumcols
                + Optional(_nuspectrumunits)
                + OneOrMore(_nuspectrumvals, stopOn=_endtable)('spectrum_vals'))
 nuspectrumblock = Group(Group(_nuspectrum + integratedres))('nu_spectrum_res')
 
@@ -933,15 +915,15 @@
 # ZA spectrum
 _zaspectrumunits = Group(Suppress(_units_kw)
                          + Word(alphanums+'.^-+%') * 2)('units')
 _zaspectrumcols = Suppress(_zaspid_kw + _spscore_kw + _spsigma_kw)
 _zaspectrumbin = (Suppress('(') + _inums + Suppress(',')
                   + _inums + Suppress(')'))
 _zaspectrumvals = (Group(_zaspectrumbin + _fnums + _fnums)
-                   .set_fail_action(trans.fail_spectrum))
+                   .setFailAction(trans.fail_spectrum))
 _zaspectrum = (Suppress(_zaspectrum_kw)
                + _numdiscbatch
                + _zaspectrumcols
                + Optional(_zaspectrumunits)
                + OneOrMore(_zaspectrumvals, stopOn=_endtable)('spectrum_vals'))
 zaspectrumblock = Group(Group(_zaspectrum + integratedres))('za_spectrum_res')
 
@@ -962,15 +944,15 @@
                            + Suppress('):') + _fnums + Suppress('-') + _fnums)
                      ('mesh_energyrange'))
 _mesh_energyintegrated = ((Suppress(_integratedres_name) + Suppress(':'))
                           ('mesh_energyintegrated'))
 _mesh_energyline = _mesh_energyrange | _mesh_energyintegrated
 _meshres = Group(
     _mesh_energyline
-    + Group(original_text_for(
+    + Group(originalTextFor(
         OneOrMore(Word(printables), stopOn=_endtable)))('mesh_vals')
     + Optional(Group(entropy)('entropy')))
 meshblock = Group(OneOrMore(Group(_timestep
                                   + Optional(_score_mesh_unit)
                                   + Group(OneOrMore(_meshres))('meshes')
                                   + Optional(integratedres)))
                   | Group(Group(OneOrMore(_meshres))('meshes')))('mesh_res')
@@ -991,40 +973,40 @@
 _kijsum = Group(Optional(Suppress(_kijlefteigenval_kw))
                 + Suppress(_kijmkeff_kw) + _fnums
                 + Suppress(_kijdomratio_kw) + _fnums)('kijmkeff_res')
 _kijeigenval = Group(_fnums + _fnums)
 _kijeigenvec = Forward()
 _kijmatrix = Forward()
 _kijeigenvaltab = (Suppress(_kijeigenval_kw)
-                   + (OneOrMore(_kijeigenval).set_parse_action(_set_kijdim))
+                   + (OneOrMore(_kijeigenval).setParseAction(_set_kijdim))
                    ('kij_eigenval'))
 _kijeigenvectab = ((Suppress(_kijeigenvec_kw) + (OneOrMore(_kijeigenvec)))
                    | _kijeigenvecnotprint_kw)('kij_eigenvec')
 _kijmatrixtab = (Suppress(_kijmatrix_kw)
                  + ((OneOrMore(_kijmatrix)) | _kijmatrixnotprint_kw)
                  ('kij_matrix'))
 kijres = (Group(Suppress(_integratedres_name)
                 + _numusedbatch
                 + _kijsum
                 + _kijeigenvaltab
                 + _kijeigenvectab
-                + _kijmatrixtab).set_parse_action(trans.convert_kij_result)
+                + _kijmatrixtab).setParseAction(trans.convert_kij_result)
           ('kij_res'))
 
 
 # KIJ SOURCES
 _kijsourcesorder = (Suppress(_kijsourcesorder_kw)
                     + Word(alphas)('kij_sources_order') + Suppress(':'))
 _kijsourcesval = Group(OneOrMore(_fnums))('kij_sources_vals')
 kijsources = (Group(Suppress(_integratedres_name)
                     + _numusedbatch
                     + Suppress(_kijsources_kw)
                     + Optional(_kijsourcesorder)
                     + _kijsourcesval)
-              .set_parse_action(trans.convert_kij_sources)('kij_sources'))
+              .setParseAction(trans.convert_kij_sources)('kij_sources'))
 
 
 # KIJ estimator for keff
 
 def _define_kij_dim(toks):
     LOGGER.debug("KIJ dimension: %d", len(toks))
     _kijdim = len(toks)
@@ -1043,25 +1025,24 @@
     _nbvols = int(toks[0])
     _kijlistvol << Group(_inums * _nbvols)  # pylint: disable=W0106
 
 
 _kijkeffbeg = Word(alphas)('estimator') + Suppress(_estimator_kw) + _minus_line
 _kijlistvol = Forward()
 _kijfissilevol = ((Suppress(_kijfissilevol_kw) + _inums('nb_fissile_vols'))
-                  .set_parse_action(_set_kij_vols)
+                  .setParseAction(_set_kij_vols)
                   + Suppress(_kijlistfissilevol_kw)
                   + _kijlistvol('list_fissile_vols'))
 _kijkeffintro = (Optional(_kijfissilevol)
                  + Suppress(_kijbatchs_kw) + _inums('batchs_kept')
                  + Suppress(_kijmkeff_kw) + _fnums('kij_mkeff'))
 
 _idline = Forward()
 _matline = Forward()
-_kijkeffev = (OneOrMore(Group(_inums + _fnums))
-              .set_parse_action(_define_kij_dim))
+_kijkeffev = OneOrMore(Group(_inums + _fnums)).setParseAction(_define_kij_dim)
 _kijkeffevtab = Group(Suppress(_kijkeffevid_kw) + _kijkeffev)('kij_leigenvec')
 _defmatrix = _idline + _minus_line + OneOrMore(_matline + _minus_line)
 _kijkeffmatrix = (Group(Suppress(_kijkeffmat_kw) + _defmatrix)
                   ('kij_matrix'))
 _kijkeffstdmatrix = (Group(Suppress(_kijkeffstddevmat_kw) + _defmatrix)
                      ('kij_stddev_matrix'))
 _kijkeffsensibmatrix = (Group(Suppress(_kijkeffsensibilitymat_kw) + _defmatrix)
@@ -1069,84 +1050,65 @@
 
 _kijkeffblock = (Group(_kijkeffbeg
                        + _kijkeffintro
                        + _kijkeffevtab
                        + _kijkeffmatrix
                        + _kijkeffstdmatrix
                        + _kijkeffsensibmatrix)
-                 .set_parse_action(trans.convert_kij_keff))
+                 .setParseAction(trans.convert_kij_keff))
 
 
 # Keff as generic response
 _keffres = Group(Word(alphas) + _fnums + _fnums)
 _keffresblock = Group(OneOrMore(_keffres))('res_per_estimator')
 _correlationdesc = Suppress(_correlations_kw)
 _correlationestim = Group(Word(alphas) + Suppress('<->') + Word(alphas))
 _correlationvals = OneOrMore(_fnums
                              | _notconverged_kw)
 _correlation = Group(_correlationestim + _correlationvals)
 _correlationblock = (Group(_correlationdesc + OneOrMore(_correlation))
                      ('correlation_mat'))
 _fullcombestimation = (Group(Suppress(_fullcomb_kw)
-                             + ((_fnums + _fnums)
-                                | (_notconverged_kw
-                                   + Suppress(Optional(_notcvg_exp_kw)))))
+                             + ((_fnums + _fnums) | _notconverged_kw))
                        ('full_comb_estimation'))
 _autokeffres = ((_keffresblock + _correlationblock + _fullcombestimation)
                 | _notconverged_kw('not_converged'))
 _warnkeff = (Suppress(_warning_kw)
-             + _warn_combkeff_kw.set_parse_action(' '.join)('warning'))
+             + _warn_combkeff_kw.setParseAction(' '.join)('warning'))
 keffblock = Group(Suppress(_integratedres_name)
                   + _numusedbatch
                   + (_autokeffres | _warnkeff)
-                  ).set_parse_action(trans.convert_keff)('keff_res')
+                  ).setParseAction(trans.convert_keff)('keff_res')
 
 
 # Keff as historical response
 _bestresestim = (OneOrMore(Word(alphas), stopOn=_estimator_kw)
-                 .set_parse_action(' '.join)('keff_estimator')
+                 .setParseAction(' '.join)('keff_estimator')
                  + Suppress(_estimator_kw))
 _bestresdiscbatch = (Suppress(_bestresdiscbatchs_kw)
                      + _inums('best_disc_batchs')
                      + Suppress("batches"))
 _bestkeff = (Suppress(Keyword("keff") + '=') + _fnums('keff')
              + Suppress(Keyword("sigma") + '=') + _fnums('sigma')
              + Suppress(Keyword("sigma%") + '=') + _fnums('sigma%'))
 _equivkeff = Suppress(_equivkeff_kw) + _fnums('equivalent_keff')
-_parna_lh = (Suppress(Keyword("mean") + '=') + _fnums('mean')
-             + Suppress(Keyword("lambda") + '=') + _fnums('lambda')
-             + Suppress(Keyword("sigma") + '=') + _fnums('sigma')
-             + Suppress(Keyword("sigma%") + '=') + _fnums('sigma%'))
-_parna_proba = (Suppress(Keyword("proba") + ':') + _fnums('proba')
-                + Suppress(Keyword("lower") + '=') + _fnums('lower')
-                + Suppress(Keyword("upper") + '=') + _fnums('upper')
-                + Suppress(Keyword("length") + '=') + _fnums('length'))
-_parna_inv_cdf = Suppress(_parna_inv_cdf_kw + ":"
-                          + _inums('iterations')
-                          + Keyword('iterations'))
-_parna_likelihood = (Suppress(_parna_likelihood_kw) + _parna_lh
-                     + Group(_parna_proba + _parna_inv_cdf)('3sigma')
-                     + Group(_parna_proba + _parna_inv_cdf)('2.57sigma'))
-_parna_block = (Group(_parna_likelihood)('parna'))
 _bestkeffpestim = (Group(_notconverged_kw('not_converged')
                          | Group(Optional(_bestresdiscbatch)
                                  + _numusedbatch
                                  + _bestkeff
-                                 + Optional(_equivkeff)
-                                 + Optional(_parna_block)
-                                 )('keff_auto'))
+                                 + Optional(_equivkeff))('keff_auto'))
                    ('results'))
 _bestreskeff = Group(_bestresestim + _minus_line + _bestkeffpestim)
 _warnfixedsources = Group(Suppress(_warning_kw) + _minus_line
                           + _warn_fixsourcekeff_kw('warning'))
 _bestresblock = OneOrMore(_bestreskeff, stopOn="KIJ")
 autokeffblock = Group(Group(Optional(_warnfixedsources)
                             + _bestresblock
                             + Optional(_kijkeffblock))
-                      .set_parse_action(trans.convert_keff_auto))('keff_auto')
+                      .setParseAction(trans.convert_keff_auto))('keff_auto')
 
 
 # MED files
 medfile = (Suppress((_creationmedfile_kw | _creationfile_kw) + ':')
            + Word(alphanums+'/_.')('med_file')
            + Suppress(_medmeshid_kw + Word(alphanums+'_.')))
 
@@ -1197,38 +1159,36 @@
                           + _numusedbatch
                           + Group(_nuclfamorder
                                   | _nucleiorder
                                   | _familyorder
                                   | _perturborder
                                   | _cvgstat)('adj_res')
                           + Optional(_unitsres)
-                          ).set_parse_action(trans.convert_generic_adjoint))
+                          ).setParseAction(trans.convert_generic_adjoint))
               )('adjoint')
 # Convergence statistics
 _kingcritline = Group(Suppress("CRITICALITY SOURCE") + _fnums + _fnums)
 _kingtimestepline = Group(Suppress("END OF TIME STEP ") + Suppress(_inums)
                           + _fnums + _fnums)
 _kingstat = Group(_kingcritline
                   + ZeroOrMore(_kingtimestepline))('kin_generic_res')
 kingres = (Group(Suppress(_integratedres_name)
                  + _numusedbatch
                  + _kingstat
                  + Optional(_unitsres)('units')
-                 ).set_parse_action(trans.convert_generic_kinetic)
+                 ).setParseAction(trans.convert_generic_kinetic)
            )('kinetic_generic')
 # sensitivities
 _sensitivityorder = (Suppress(_sensitivitytypeorder_kw)
                      + OneOrMore(Word(alphas + '_,()'),
                                  stopOn=_sensitivityindexorder_kw)
-                     .set_parse_action(' '.join)
+                     .setParseAction(' '.join)
                      + Suppress(_sensitivityindexorder_kw))
-_sensitivityreactionrate_ratio = Group(Suppress(_sensitivityreactionrate_kw)
-                                       + _fnums('score') + _fnums('sigma'))
 _sensitivity_type = (OneOrMore(Word(alphas.upper()), stopOn=_sensitivity_kw)
-                     .set_parse_action(' '.join)
+                     .setParseAction(' '.join)
                      + Suppress(_sensitivity_kw))('typeI')
 _sensitivity_index = Group(
     Suppress("i =") + _inums('sensitivity_index') + Suppress(';')
     + Suppress("NUCLEUS :") + Word(alphanums + '_')('sensitivity_nucleus')
     + Suppress(',') + Suppress("TYPE :")
     + Word(alphanums.upper() + '_() ')('sensitivity_reaction'))
 _sensitivity_dircos = Group(Suppress(_sensitivity_dircos_kw)
@@ -1245,23 +1205,21 @@
                              ZeroOrMore(_sensitivity_dircos
                                         | _sensitivity_energyinc)
                              + Suppress(_sensitivity_cols)
                              + OneOrMore(_sensitivity_vals)('values'))))
                          ('vals')
                          + _sensitivity_energyint('energy_integrated'))
 _sensitivity = (Suppress(_sensitivityorder)
-                + ZeroOrMore(Group(_sensitivityreactionrate_ratio
-                                   ('reaction_rate')))
                 + (OneOrMore(Group(_sensitivity_type('sensitivity_type')
                                    + OneOrMore(_sensitivity_res)('res')))))
 sensitivityres = Group(Group(Optional(Suppress(_integratedres_name))
                              + _numusedbatch
                              + Group(_sensitivity)('sensit_res')
                              + Optional(_unitsres)('units'))
-                       .set_parse_action(trans.convert_sensitivities)
+                       .setParseAction(trans.convert_sensitivities)
                        )('sensitivity')
 
 
 def _rename_norm_kw():
     '''Transform RESULTS ARE NORMALIZED keyword in int (lighter)'''
     return 1
 
@@ -1281,64 +1239,63 @@
 # IFP adjoint criticality edition
 _adjcrit_ed_intro = _star_line + Suppress(_ifpadjcriticality_kw) + _star_line
 _ifpadjcrit_intro = Group(Word(alphas+'_')('ifp_response')
                           + _scorename
                           + Suppress(_ifpadjcyclelength_kw)
                           + _inums('ifp_cycle_length')
                           + (Optional(_ifpadjnormalizedres_kw
-                                      .set_parse_action(_rename_norm_kw))
+                                      .setParseAction(_rename_norm_kw))
                              ('normalized'))
                           + _star_line)
 _ifpadjbinval = Forward()
 _ifpadjcoordinate = Word(alphas) + Suppress(_ifpadjminmax_kw)
 _ifpadjcoordinates = ((Optional(_ifpadjvol_kw) + OneOrMore(_ifpadjcoordinate))
-                      .set_parse_action(_define_ifp_adj_table_dim))
+                      .setParseAction(_define_ifp_adj_table_dim))
 _ifpadjcolumns = _ifpadjcoordinates + _ifpadjscore_kw + _spsigma_kw
 _ifpadjline = Group(_ifpadjbinval + _fnums + _fnums)
 _ifpadjvalues = OneOrMore(_ifpadjline)
 _adjcritblock = Group(_ifpadjcrit_intro('ifp_adjoint_criticality_intro')
                       + _ifpadjcolumns('columns')
                       + _ifpadjvalues('values')
                       + _star_line)
-ifpadjointcriticality = (
-    Group((_adjcrit_ed_intro + OneOrMore(_adjcritblock))
-          .set_parse_action(trans.convert_ifp_adj_crit_ed))
-    ('ifp_adjoint_crit_edition'))
+ifpadjointcriticality = (Group((_adjcrit_ed_intro + OneOrMore(_adjcritblock))
+                               .setParseAction(trans.convert_ifp_adj_crit_ed))
+                         ('ifp_adjoint_crit_edition'))
 
 # Spherical harmonics results
 _shr_bins = Group(Suppress(_shr_nb_space_bins_kw) + _inums('nb_sbins')
                   + Suppress(_shr_nb_u_space_bins_kw) + _inums('nb_ubins')
                   + Suppress(_shr_nb_v_space_bins_kw) + _inums('nb_vbins')
                   + Suppress(_shr_nb_w_space_bins_kw) + _inums('nb_wbins')
                   + Suppress(_shr_nb_energy_bins_kw) + _inums('nb_ebins')
                   + Suppress(_shr_nb_inc_energy_bins_kw) + _inums('nb_iebins')
                   + Suppress(_shr_lmax_kw) + _inums('lmax'))('nb_bins')
 _shrscore = (Suppress(_shr_score_name_kw)
              + Group(OneOrMore(Word(printables), stopOn=LineEnd())
-             .set_parse_action(' '.join))('score_name'))
+             .setParseAction(' '.join))('score_name'))
 _shrspace = Suppress(_shr_space_kw) + Group(_inums + _inums + _inums)('space')
 _shrenergy = Suppress(_shr_energy_kw) + Group(_fnums + _fnums)('energy')
 _shrincenergy = (Suppress(_shr_incident_energy_kw)
                  + Group(_fnums + _fnums)('incident_energy'))
 _shrcols = Suppress(_shr_l_kw + _shr_m_kw + _shr_score_kw + _shr_sigma_kw)
 _shrvals = Group(_inums + _inums + _fnums + _fnums)
 _shrtable = _shrenergy + _shrcols + OneOrMore(_shrvals)('values')
 _shr_ietable = Optional(_shrincenergy) + OneOrMore(Group(_shrtable))('vpie')
 _shr_spacetable = _shrspace + OneOrMore(Group(_shr_ietable))('vpspace')
 _shr_scoretable = _shrscore + OneOrMore(Group(_shr_spacetable))('score')
 shrblock = Group(_shr_bins
                  + Group(OneOrMore(Group(_shr_scoretable)))('res')
                  + Suppress(_star_line)
-                 ).set_parse_action(trans.convert_shr)('spherical_harmonics')
+                 ).setParseAction(trans.convert_shr)('spherical_harmonics')
 
 # Perturbations
 _perturank = Suppress(_perturank_kw) + _inums('perturbation_rank')
 _pertumethod = (Suppress(_pertumethod_kw)
                 + OneOrMore(Word(alphas), stopOn=LineEnd())
-                .set_parse_action(' '.join)('perturbation_method'))
+                .setParseAction(' '.join)('perturbation_method'))
 _pertuorder = Suppress(_pertuorder_kw) + _inums('perturbation_order')
 _pertutype = Suppress(_pertutype_kw) + Word(alphas)('perturbation_type')
 _pertucompo = (Suppress(_pertucompo_kw)
                + Word(alphanums+'_')('perturbation_composition'))
 pertu_desc = (Group(Suppress(_perturbation_kw)
                     + _perturank
                     + _pertumethod
@@ -1392,18 +1349,18 @@
                                            | medfile
                                            | integratedres
                                            | bestres
                                            | uncertblock
                                            | uncertintegblock
                                            | gbblock
                                            | corresptable)))
-              .set_parse_action(trans.convert_score))
+              .setParseAction(trans.convert_score))
 
 listscoreblock = (Group(OneOrMore(scoreblock)
-                        .set_parse_action(trans.index_elements('score_index')))
+                        .setParseAction(trans.index_elements('score_index')))
                   ('score_res'))
 
 # Response block
 responseblock = Group(keffblock
                       | kijres
                       | kijsources
                       | adjointres
@@ -1413,47 +1370,46 @@
                       | shrblock
                       | listscoreblock)('results')
 
 response = (Group(_star_line
                   + respintro
                   + _star_line
                   + responseblock)
-            .set_parse_action(trans.finalize_response_dict))
+            .setParseAction(trans.finalize_response_dict))
 
-listresponses = Group(OneOrMore(response).set_parse_action(
+listresponses = Group(OneOrMore(response).setParseAction(
     compose2(trans.extract_all_metadata,
              trans.index_elements('response_index'))))('list_responses')
 
 perturbation = (OneOrMore(Group(pertu_desc + listresponses)
-                          .set_parse_action(trans.propagate_all_metadata))
-                .set_parse_action(trans.index_elements('perturbation_index'))
+                          .setParseAction(trans.propagate_all_metadata))
+                .setParseAction(trans.index_elements('perturbation_index'))
                 ('perturbation'))
 
 
 ################################
 #         DEBUG PARSER         #
 ################################
 
 # debug grammar, to be used with parse_debug (only for parsing development)
 t4debug_gram = (OneOrMore((intro
                            + OneOrMore(listresponses | ifpadjointcriticality
                                        | autokeffblock | perturbation
                                        | Suppress(contribpartblock)
                                        | OneOrMore(runtime)))
-                          .set_parse_action(trans.to_final_dict))
-                .set_parse_action(dump_in_logger)
-                | intro + OneOrMore(runtime)
-                ).set_fail_action(trans.fail_parsing)
+                          .setParseAction(trans.to_final_dict))
+                .setParseAction(dump_in_logger)
+                | intro + OneOrMore(runtime)).setFailAction(trans.fail_parsing)
 
 
 ################################
 #        GENERAL PARSER        #
 ################################
 
 t4gram = (OneOrMore((intro
                      + ZeroOrMore(listresponses | ifpadjointcriticality
                                   | autokeffblock | perturbation
                                   | Suppress(contribpartblock))
                      + runtime)
-                    .set_parse_action(trans.to_final_dict))
-          .set_parse_action(dump_in_logger)
-          ).set_fail_action(trans.fail_parsing)
+                    .setParseAction(trans.to_final_dict))
+          .setParseAction(dump_in_logger)
+          ).setFailAction(trans.fail_parsing)
```

### Comparing `valjean-0.11.0a0/valjean/eponine/tripoli4/parse.py` & `valjean-0.9.0/valjean/eponine/tripoli4/parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,27 +38,27 @@
 Some options for debugging are available (end flag).
 
 .. todo::
 
    Change absolute imports in relative ones when main will be moved to
    :ref:`cambronne <cambronne-main>`.
 '''
-import logging
+
 import threading
 from pyparsing import ParseException, ParserElement
 
 from . import scan
 from .grammar import t4gram
 from .common import SpectrumDictBuilderException, MeshDictBuilderException
 from ...chrono import Chrono
 from ..browser import Browser
 from .data_convertor import convert_data
+from ... import LOGGER
 
 
-LOGGER = logging.getLogger(__name__)
 PYPARSING_LOCK = threading.RLock()
 
 # in Eponine, profile is a key of globals
 if 'profile' not in globals()['__builtins__']:
     def profile(fprof):
         '''To profile memory usage.'''
         return fprof
@@ -101,15 +101,16 @@
                 self.scan_res = self._scan()
         except scan.ScannerException as t4se:
             LOGGER.error(t4se)
             raise ParserException("Scan failed.") from None
         except ParserException as t4pe:
             LOGGER.error(t4pe)
             raise ParserException("Scan failed.") from None
-        LOGGER.info("Successful scan in %f s", chrono)
+        else:
+            LOGGER.info("Successful scan in %f s", chrono)
 
     def _scan(self):
         '''Scan the parse the given jdd.'''
         scan_res = self._scan_listing()
         self._check_scan(scan_res)
         return scan_res
 
@@ -337,21 +338,14 @@
             sigma = None
         elif 'vovstar' in score:
             sigma = 'vovstar_sigma'
             what = 'vovstar'
         elif 'uncert' in resn:
             rname = rname.replace('uncert_', '')
             what = score
-        elif resn == 'parna_likelihood':
-            if score == 'mean':
-                rname = resn
-                what = resn
-            else:
-                rname = '_'.join((resn, score))
-                what = score
         else:
             what = resp['response_function'].lower()
         return rname, sigma, what
 
     def _dset_from_dict(self, resn, res, resp):
         tdict = {}
         for arr in res:
```

### Comparing `valjean-0.11.0a0/valjean/eponine/tripoli4/parse_debug.py` & `valjean-0.9.0/valjean/eponine/tripoli4/parse_debug.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,24 +35,23 @@
 '''
 
 import logging
 
 from .parse import Parser, ParseResult, ParserException
 from . import scan
 from .grammar import t4debug_gram
+from ... import LOGGER
 from ...chrono import Chrono
 
 
-LOGGER = logging.getLogger(__name__)
-
-
 class ParserDebug(Parser):
     '''Scan up to the end flag then parse. For parsing debugging.'''
 
     def __init__(self, jddname, *, end_flag="", ofile=""):
+        # pylint: disable=too-many-arguments
         '''Initialize the :class:`ParserDebug` object.
 
         :param str jddname: path to the Tripoli-4 output
         :param int batch: batch to read (-1 = last, 0 = all, then X)
         :param str end_flag: optional end flag to stop scanning and parsing
                              (empty string per default)
```

### Comparing `valjean-0.11.0a0/valjean/eponine/tripoli4/resources/depletion/BurnupResults.C` & `valjean-0.9.0/valjean/eponine/tripoli4/resources/depletion/BurnupResults.C`

 * *Files identical despite different names*

### Comparing `valjean-0.11.0a0/valjean/eponine/tripoli4/resources/depletion/BurnupResults.h` & `valjean-0.9.0/valjean/eponine/tripoli4/resources/depletion/BurnupResults.h`

 * *Files identical despite different names*

### Comparing `valjean-0.11.0a0/valjean/eponine/tripoli4/resources/depletion/DepletedComposition.C` & `valjean-0.9.0/valjean/eponine/tripoli4/resources/depletion/DepletedComposition.C`

 * *Files identical despite different names*

### Comparing `valjean-0.11.0a0/valjean/eponine/tripoli4/resources/depletion/DepletedComposition.h` & `valjean-0.9.0/valjean/eponine/tripoli4/resources/depletion/DepletedComposition.h`

 * *Files identical despite different names*

### Comparing `valjean-0.11.0a0/valjean/eponine/tripoli4/resources/depletion/MeanBurnupResults.C` & `valjean-0.9.0/valjean/eponine/tripoli4/resources/depletion/MeanBurnupResults.C`

 * *Files identical despite different names*

### Comparing `valjean-0.11.0a0/valjean/eponine/tripoli4/resources/depletion/MeanBurnupResults.h` & `valjean-0.9.0/valjean/eponine/tripoli4/resources/depletion/MeanBurnupResults.h`

 * *Files identical despite different names*

### Comparing `valjean-0.11.0a0/valjean/eponine/tripoli4/scan.py` & `valjean-0.9.0/valjean/eponine/tripoli4/scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,20 +108,21 @@
   * For exploitation jobs use ``"exploitation time"`` (example: Green bands);
   * for jobs running in parallel, ``"elapsed time"`` will also appear, after
     ``"simulation time"`` normal.
 
 Module API
 ----------
 '''
-import logging
+
 from collections.abc import Mapping
 from collections import OrderedDict
 
 
-LOGGER = logging.getLogger(__name__)
+from ... import LOGGER
+
 
 # get profile from globals (cleaner)
 if 'profile' not in globals()['__builtins__']:
     def profile(fmem):
         '''Deactivate profiling if not required in command line.'''
         return fmem
```

### Comparing `valjean-0.11.0a0/valjean/eponine/tripoli4/transform.py` & `valjean-0.9.0/valjean/eponine/tripoli4/transform.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,22 +40,19 @@
 .. |parseres| replace:: pyparsing.ParseResults
 
 .. note::
 
     This module is not standalone, needs a `pyparsing` result in input.
 '''
 
-import logging
 from collections.abc import Iterable
 import numpy as np
 from pyparsing import ParseException
 from . import common
-
-
-LOGGER = logging.getLogger(__name__)
+from ... import LOGGER
 
 
 def compose2(f, g):  # pylint: disable=invalid-name
     '''Functions composition (2 functions), like fog in mathematics.
 
     :params func f: last function to compose, takes result from g as arguments
     :params func g: first function to apply
@@ -156,35 +153,35 @@
 
 
 def convert_correspondence_table(toks):
     '''Convert correspondence table to dict (volume id, volume name).
 
     :returns: tuple(tuple)
     '''
-    return tuple(set(common.convert_list_to_tuple(toks.as_list())))
+    return tuple(set(common.convert_list_to_tuple(toks.asList())))
 
 
 def convert_scoring_zone_id(toks):
     '''Convert scoring zone id (volume numbers, cells, points, etc) into native
     python objects (str, tuple, numpy object).
     '''
     if isinstance(toks, (np.generic, str)):
         return toks
-    cv_toks = common.convert_list_to_tuple(toks.as_list())
+    cv_toks = common.convert_list_to_tuple(toks.asList())
     return cv_toks
 
 
 def convert_list_to_tuple(toks):
     '''Convert list from pyparsing to tuple.
 
     This function is only used to transform the parseResult in standard python
     list and send it to convert_list_to_tuple in
     :mod:`~valjean.eponine.tripoli4.common`.
     '''
-    ltoks = toks.as_list()
+    ltoks = toks.asList()
     # in reaction case, e.g. [[104]] while [[21, 104]] is fine
     if isinstance(ltoks[0], list) and len(ltoks) == 1 and len(ltoks[0]) == 1:
         ltoks = ltoks[0]
     cv_toks = common.convert_list_to_tuple(ltoks)
     return cv_toks
 
 
@@ -210,15 +207,15 @@
     res = {}
     is_uncert = any('uncert' in k for k in list(score.keys()))
     for key in score.keys():
         # green bands: too complicated structure
         if (('_res' in key and isinstance(score[key], Iterable)
              and key != 'green_bands_res')):
             usc = (score[key]
-                   if isinstance(score[key], dict) or score[key].as_dict()
+                   if isinstance(score[key], dict) or score[key].asDict()
                    else score[key][0])
             _extract_batch_numbers(usc, res)
             if ('used_batches_res' in res and 'discarded_batches_res' in res
                     and not is_uncert):
                 break
             if 'integrated_res' in usc:
                 _extract_batch_numbers(usc['integrated_res'], res)
@@ -250,15 +247,15 @@
             elif 'spectrum_res' in key:
                 # uncert_spectrum_res singularized as spectrum_res also exists
                 # in same response
                 keystr = 'spectrum_res' if 'uncert' not in key else key
                 res[keystr] = convert_spectrum(score[key], key)
             elif key in ('integrated_res', 'uncert_integrated_res', 'vov_res',
                          'vovstar_res', 'sensibility_res', 'best_result_res'):
-                res[key] = score[key].as_dict()
+                res[key] = score[key].asDict()
             elif key == 'green_bands_res':
                 res[key] = convert_green_bands(score[key])
                 res['discarded_batches_res'] = res[key].pop(
                     'discarded_batches')
             elif key == 'scoring_zone_id':
                 res['scoring_zone_id'] = convert_scoring_zone_id(score[key])
             elif key == 'correspondence_table':
@@ -269,16 +266,16 @@
                 res[key] = score[key]
     return res
 
 
 def _debug_print(toks):
     print("FOUND THE POINT")
     # print(toks)
-    print("List:", toks.as_list())
-    print("Dict:", toks.as_dict())
+    print("List:", toks.asList())
+    print("Dict:", toks.asDict())
 
 
 def convert_generic_adjoint(toks):
     '''Convert adjoint output in :obj:`numpy` object using
     :mod:`~valjean.eponine.tripoli4.common`.
 
     This method does not take into account sensitivities calculated via the IFP
@@ -338,15 +335,15 @@
        <valjean.eponine.tripoli4.common.convert_keff>` instead.
 
     .. seealso::
        :func:`common.convert_keff
        <valjean.eponine.tripoli4.common.convert_keff>` and more generally
        :mod:`~valjean.eponine.tripoli4.common`
     '''
-    keffmat = common.convert_keff(toks['keff_res'].as_dict())
+    keffmat = common.convert_keff(toks['keff_res'].asDict())
     return keffmat
 
 
 def convert_kij_sources(toks):
     r'''Convert k\ :sub:`ij` sources to python dictionary containing
     :obj:`numpy` objects and using :mod:`~valjean.eponine.tripoli4.common`.
 
@@ -356,15 +353,15 @@
       :obj:`numpy.ndarray`
 
     .. seealso::
        :func:`common.convert_kij_sources
        <valjean.eponine.tripoli4.common.convert_kij_sources>`
        and more generally :mod:`~valjean.eponine.tripoli4.common`
     '''
-    kijs = common.convert_kij_sources(toks['kij_sources'].as_dict())
+    kijs = common.convert_kij_sources(toks['kij_sources'].asDict())
     return kijs
 
 
 def convert_kij_result(toks):
     r'''Convert k\ :sub:`ij` result to dictionary of :obj:`numpy` objects using
     :mod:`~valjean.eponine.tripoli4.common`.
 
@@ -373,15 +370,15 @@
     :returns: dictionary of :obj:`numpy.ndarray` and :obj:`numpy.matrix`
 
     .. seealso::
        :func:`common.convert_kij_result
        <valjean.eponine.tripoli4.common.convert_kij_result>`
        and more generally :mod:`~valjean.eponine.tripoli4.common`
     '''
-    kijm = common.convert_kij_result(toks['kij_res'].as_dict())
+    kijm = common.convert_kij_result(toks['kij_res'].asDict())
     return kijm
 
 
 def convert_kij_keff(toks):
     r'''Convert k\ :sub:`eff` estimated from k\ :sub:`ij` to dictionary of
     :obj:`numpy` objects using :mod:`~valjean.eponine.tripoli4.common`.
 
@@ -393,71 +390,44 @@
     .. note:: It is possible to add a check on estimator if issue.
 
     .. seealso::
        :func:`common.convert_kij_keff
        <valjean.eponine.tripoli4.common.convert_kij_keff>`
        and more generally :mod:`~valjean.eponine.tripoli4.common`
     '''
-    kijkeff = common.convert_kij_keff(toks[-1].as_dict())
+    kijkeff = common.convert_kij_keff(toks[-1].asDict())
     return kijkeff
 
 
-def convert_parna_keff(pdict):
-    '''Convert Parna likelihood results to python dictionary.
-
-    This result is part of the ``keff_auto`` results.
-
-    :param pdict: parna results block to be converted in dictionary (with
-      filter).
-    :returns: dictionary
-    '''
-    plhd = {}
-    for key, val in pdict.items():
-        if isinstance(val, dict):
-            for keyd, vald in val.items():
-                if keyd != 'length':
-                    plhd[f'{key}_{keyd}'] = vald
-        else:
-            plhd[key] = val
-    return plhd
-
-
 def convert_keff_auto(toks):
     '''Convert auto keff estimation (old or default output, not printed as a
     usual response) in standard python objects.
 
     Add the ``'response_type'`` key to the dictionary with ``'keff_auto_res'``
     as associated value (to match browser and data_convertor requirements).
-
-    :param toks: `pyparsing` element
-    :type toks: |parseres|
-    :returns: python list corresponding to input `pyparsing` list
     '''
     assert len(toks) == 1, "Not correct number of elements in keff_auto toks"
     akeff_res = toks[0]
     akeff_key = 'keff_auto'
     res = []
     for akeff in akeff_res:
         # if kij result always a dict at that step, not for auto keff
         is_kij = isinstance(akeff, dict)
         akeffd = {}
         akeffd['response_type'] = akeff_key if not is_kij else 'kijkeff'
         if 'results' not in akeff:  # some warning cases
             continue
         akeffd['keff_estimator'] = akeff['keff_estimator']
-        akeffr = akeff['results'].as_dict() if not is_kij else akeff['results']
+        akeffr = akeff['results'].asDict() if not is_kij else akeff['results']
         # may not be there for not converged results
         if akeff_key in akeffr:
             akeffra = akeffr[akeff_key]
             akeffr['used_batches'] = akeffra.pop('used_batches')
             if 'best_disc_batchs' in akeffra:
                 akeffr['discarded_batches'] = akeffra.pop('best_disc_batchs')
-        if 'keff_auto' in akeffr and 'parna' in akeffr['keff_auto']:
-            parna = akeffr['keff_auto'].pop('parna')
-            akeffr['parna_likelihood'] = convert_parna_keff(parna)
         akeffd['results'] = akeffr
         res.append(akeffd)
     return res
 
 
 def convert_sensitivities(toks):
     '''Convert sensitivity results to dictionary of :obj:`numpy` objects using
@@ -484,15 +454,15 @@
 
 
 def convert_ifp_adj_crit_ed(toks):
     '''Convert IFP adjoint criticality edition in kinematic array.'''
     lced = []
     for ind, crit_ed in enumerate(toks):
         LOGGER.debug("IFP adjoint crit edition result %d", ind)
-        score_res = {'results': common.convert_crit_edition(crit_ed.as_dict()),
+        score_res = {'results': common.convert_crit_edition(crit_ed.asDict()),
                      'response_type': 'ifp_adj_crit_edition'}
         score_res.update(crit_ed['ifp_adjoint_criticality_intro'])
         lced.append(score_res)
         LOGGER.debug(list(score_res.keys()))
     LOGGER.debug("Nombre de score dans l'edition: %d", len(lced))
     return lced
 
@@ -500,15 +470,15 @@
 def to_final_dict(toks):
     '''Convert to dictionary result of `pyparsing`.
 
     :param toks: `pyparsing` element
     :type toks: |parseres|
     :returns: python dictionary corresponding to input `pyparsing` dictionary
     '''
-    res = toks.as_dict()
+    res = toks.asDict()
     res['batch_data'] = res.pop('intro')
     res['batch_data'].update(res.pop('conclu', {}))
     return res
 
 
 def lod_to_dot(toks):
     '''List of dictionaries to dictionary of tuples.
@@ -544,15 +514,15 @@
     element.
     '''
     LOGGER.debug("In lod_of_dot")
     ldict = {}
     for elt in toks:
         # to be able to test the method (= allow toks is already a dict and not
         # necessarly a pyparsing.ParseResults)
-        edict = elt if isinstance(elt, dict) else elt.as_dict()
+        edict = elt if isinstance(elt, dict) else elt.asDict()
         for key, val in edict.items():
             ldict.setdefault(key, []).append(val)
     ldict = {k: tuple(v) for k, v in ldict.items()}
     return ldict
 
 
 def finalize_response_dict(s, loc, toks):
@@ -571,24 +541,24 @@
     dictionary. As a consequence, the `compos_details` key  disappears.
 
     :param toks: `pyparsing` element
     :type toks: |parseres|
     :returns: python dict corresponding to input `pyparsing` response result
     '''
     LOGGER.debug("In finalize_response_dict")
-    assert len(toks[0]['results'].as_dict()) == 1, \
-        f"More than one entry in dict: {len(toks[0]['results'].as_dict())!r}"
+    assert len(toks[0]['results'].asDict()) == 1, \
+        f"More than one entry in dict: {len(toks[0]['results'].asDict())!r}"
     res = toks[0]['results']
     key, val = next(res.items())
     # in keff case, results are stored in a list
     if len(res) > 1:
         val = res
-    assert isinstance(val, dict) or val.as_list()
-    mydict = toks[0].as_dict()
-    mydict['results'] = val if isinstance(val, dict) else val.as_list()
+    assert isinstance(val, dict) or val.asList()
+    mydict = toks[0].asDict()
+    mydict['results'] = val if isinstance(val, dict) else val.asList()
     mydict['response_type'] = key[:-4] if '_res' in key else key
     mydict.update(mydict.pop('compos_details', {}))
     LOGGER.debug("Final response metadata: %s",
                  {k: v for k, v in mydict.items() if k != 'results'})
     return mydict
 
 
@@ -712,15 +682,15 @@
     been extracted. This case typically apply to perturbations (not IFP ones).
 
     :param dict ldict: dictionary corresponding to a response
     :rtype: list(dict)
     '''
     LOGGER.debug("In propagate_top_metadata")
     if not isinstance(ldict, dict):
-        ldict = ldict.as_dict()
+        ldict = ldict.asDict()
     assert 'list_responses' in ldict
     lresps = ldict.pop('list_responses')
     for resp in lresps:
         for k, val in ldict.items():
             if isinstance(val, dict):
                 resp.update(val)
             else:
@@ -738,15 +708,15 @@
 
     :param toks: `pyparsing` element
     :type toks: |parseres|
     :returns: python dict corresponding to input `pyparsing` named group
     '''
     assert len(toks) == 1
     key = next(toks.keys())
-    tmpdict = toks.as_dict()
+    tmpdict = toks.asDict()
     tmpdict.update(convert_batch_numbers(tmpdict))
     for elt in toks[0]:
         if isinstance(elt, dict):
             tmpdict[key].update(elt)
     return tmpdict
```

### Comparing `valjean-0.11.0a0/valjean/eponine/tripoli4/use.py` & `valjean-0.9.0/valjean/eponine/tripoli4/use.py`

 * *Files identical despite different names*

### Comparing `valjean-0.11.0a0/valjean/fingerprint.py` & `valjean-0.9.0/valjean/fingerprint.py`

 * *Files identical despite different names*

### Comparing `valjean-0.11.0a0/valjean/gavroche/diagnostics/metadata.py` & `valjean-0.9.0/valjean/gavroche/diagnostics/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     '''A test that compares metadata.
 
     .. todo::
 
         Document the parameters...
     '''
 
+    # pylint: disable=too-many-arguments
     def __init__(self, dict_md, name, description='', labels=None,
                  exclude=('results', 'index', 'score_index', 'response_index',
                           'response_type')):
         '''Initialisation of :class:`TestMetadata`.
 
         :param str name: local name of the test
         :param str description: specific description of the test
```

### Comparing `valjean-0.11.0a0/valjean/gavroche/diagnostics/stats.py` & `valjean-0.9.0/valjean/gavroche/diagnostics/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,28 +39,25 @@
   initialization with :func:`test_stats_by_labels`
 
 The two tests over the test results are performed using the
 :class:`~.TestResult`, so the statistics only includes the tests that were
 actually run.
 '''
 
-import logging
 from collections import defaultdict
 from functools import partial, update_wrapper, total_ordering
 from enum import IntEnum
 
 from ...fingerprint import fingerprint
 from ...cosette.task import TaskStatus, close_dependency_graph
 from ...cosette.use import Use
 from ..test import Test, TestResult
 from ..eval_test_task import EvalTestTask
 from ...eponine.browser import Index
-
-
-LOGGER = logging.getLogger(__name__)
+from ... import LOGGER
 
 
 def stats_worker(test_fn, name, description, tasks, **kwargs):
     '''Function creating the test for all the required tasks (summary tests of
     test tasks or summary tests on all tasks for example).
 
     :param test_fn: function generating the test to apply to tasks
@@ -624,14 +621,15 @@
         :param Index index: index used to calculate the statistics
         :param tuple(str) labels: ordered labels to sort the test results
         :param set rok: successful test results
         :param set rko: failed test results
         :param tuple plab: previous labels
         :rtype: list(dict)
         '''
+        # pylint: disable=too-many-arguments
         label = labels[0]
         if label not in index:
             LOGGER.warning('%s not found in some test labels', label)
             return []
         if len(labels) > 1:
             lres = []
             for lab, labset in index.get(label, {}).items():
@@ -715,15 +713,15 @@
 
     def nb_missing_labels(self):
         '''Return the number of tests where at least one of the labels required
         were missing.
 
         :rtype: int
         '''
-        return self.n_labels - sum(s['total'] for s in self.classify)
+        return self.n_labels - sum([s['total'] for s in self.classify])
 
 
 def classification_counts(classify, status_first):
     '''Count the occurrences of different statuses in the `classify`
     dictionary.
 
     :param dict classify: a dictionary associating *things* to statuses. The
```

### Comparing `valjean-0.11.0a0/valjean/gavroche/eval_test_task.py` & `valjean-0.9.0/valjean/gavroche/eval_test_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,25 +30,22 @@
 
 '''The purpose of this module is to define the :class:`EvalTestTask` class, a
 task that evaluates a collection of :class:`~.gavroche.test.Test` objects and
 transforms them into :class:`~.gavroche.test.TestResult` objects, which can be
 subsequently processed for inclusion in a test report.
 '''
 
-import logging
 from pathlib import Path
 
 from ..path import ensure, sanitize_filename
 from ..cosette.task import TaskStatus
 from ..cosette.use import from_env
 from ..cosette.pythontask import PythonTask
 from ..gavroche.test import Test, TestResultFailed
-
-
-LOGGER = logging.getLogger(__name__)
+from .. import LOGGER
 
 
 def actually_eval_test(test):
     '''Actually perform test evaluation.
 
     :returns: the result of test evaluation.
     :rtype: TestResult
```

### Comparing `valjean-0.11.0a0/valjean/gavroche/stat_tests/bonferroni.py` & `valjean-0.9.0/valjean/gavroche/stat_tests/bonferroni.py`

 * *Files 2% similar despite different names*

```diff
@@ -437,14 +437,15 @@
         yield float(self.alpha).hex().encode('utf-8')
 
 
 class TestResultHolmBonferroni(TestResult):
     '''Result from the Holm-Bonferroni method.'''
 
     def __init__(self, test, first_test_res, alphas_i, rejected_null_hyp):
+        # pylint: disable=too-many-arguments
         '''Initialisation of :class:`~.TestResultHolmBonferroni`
 
         :param test: the used Holm-Bonferroni test
         :type test: :class:`~TestHolmBonferroni`
         :param first_test_res: the test result used to obtain the p-values
         :type first_test_res: :class:`~valjean.gavroche.test.TestResult`
                               child class
```

### Comparing `valjean-0.11.0a0/valjean/gavroche/stat_tests/chi2.py` & `valjean-0.9.0/valjean/gavroche/stat_tests/chi2.py`

 * *Files identical despite different names*

### Comparing `valjean-0.11.0a0/valjean/gavroche/stat_tests/student.py` & `valjean-0.9.0/valjean/gavroche/stat_tests/student.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,21 +319,18 @@
     >>> bool(tstudent_res)
     False
     >>> print(np.array2string(tstudent_res.tstud[0]))
     [  0.   0. -inf]
     >>> print(np.array2string(tstudent_res.oracles()))
     [[ True  True False]]
 '''
-import logging
 import numpy as np
 from scipy.stats import t, norm
 from ..test import check_bins, TestDataset, TestResult
-
-
-LOGGER = logging.getLogger(__name__)
+from ... import LOGGER
 
 
 class TestResultStudent(TestResult):
     '''Result from Student's t-test.'''
 
     def __init__(self, test, tstud, pvalue=None):
         '''Initialisation of :class:`~.TestResultStudent`
```

### Comparing `valjean-0.11.0a0/valjean/gavroche/test.py` & `valjean-0.9.0/valjean/gavroche/test.py`

 * *Files identical despite different names*

### Comparing `valjean-0.11.0a0/valjean/javert/formatter.py` & `valjean-0.9.0/valjean/javert/formatter.py`

 * *Files identical despite different names*

### Comparing `valjean-0.11.0a0/valjean/javert/mpl.py` & `valjean-0.9.0/valjean/javert/mpl.py`

 * *Files 0% similar despite different names*

```diff
@@ -541,29 +541,27 @@
     >>> from valjean.javert import mpl
     >>> mplplt = mpl.MplPlot(pltbar)
     >>> fig, _ = mplplt.draw()
 
 Module API
 ----------
 '''
-import logging
 from itertools import cycle, chain
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.colors as mplcol
-
-
-LOGGER = logging.getLogger(__name__)
+from .. import LOGGER
 
 
 class MplStyle:
     '''Class to store style characteristics.'''
 
     def __init__(self, style=None, colors=None, mshape=None, mfill=None,
                  legends=None):
+        # pylint: disable=too-many-arguments
         '''Initialisation of the style.
 
         :param style: style from `matplotlib styles`_ or from user one, if
             ``None`` ``'default'`` is used
         :type style: str or None
         :param colors: colors from `matplotlib colors`_, if ``None`` CN are
             used
@@ -732,15 +730,15 @@
 
     def save(self, name='fig.png'):
         '''Save the plot under the given name.
 
         :param str name: name of the output file. Expected extensions: png,
             pdf, svg, eps.
         '''
-        LOGGER.debug('drawing figure %s', name)
+        LOGGER.info('drawing figure %s', name)
         fig, _ = self.draw()
         if fig is not None:
             fig.savefig(name)
             plt.close(fig)
 
 
 class _MplLegend:
@@ -839,15 +837,15 @@
                     ncol=ncol, **self.mpl_style.legends)
 
     def customize_plots(self, splt):
         '''Customize plots (scale, limits and lines).'''
         splt.set_xlabel(self.data.axnames[0])
         splt.set_ylabel(self.data.axnames[1])
         if self.data.curves[0].bins[0].dtype.kind == 'U':
-            bmax = max(len(b) for b in self.data.curves[0].bins[0])
+            bmax = max([len(b) for b in self.data.curves[0].bins[0]])
             if bmax * self.data.curves[0].bins[0].size > 60:
                 splt.tick_params(axis='x', rotation=90)
         if self.data.attributes.limits is not None:
             splt.set_xlim(*self.data.attributes.limits[0])
         if self.data.attributes.logx:
             splt.set_xscale('log')
         if self.data.attributes.logy:
@@ -920,14 +918,15 @@
                 cbins.append((tbin[1:] + tbin[:-1]) * 0.5)
                 bins.append(tbin)
             rsbins.append(np.array(cbins[-1]).reshape(shape))
         gbins = np.broadcast_arrays(*rsbins)
         return gbins, bins, cbins
 
     def itwod_plot(self, fig, splt, curve, axnames, norm):
+        # pylint: disable=too-many-arguments
         '''Draw the 2D distribution on the ith subplot.
 
         :param matplotlib.figure.Figure fig: the current figure
         :param matplotlib.axes.Axes splt: the current subplot
         :param CurveElements curve: data to plot
         :param int iplot: number of the subplot
         :param norm: function corresponding to the chosen
@@ -940,15 +939,15 @@
             bins=bins, norm=norm, weights=curve.values.flatten())
         cbar = fig.colorbar(h2d[3], ax=splt)
         splt.set_xlabel(axnames[0])
         if curve.bins[0].size == curve.values.shape[0]:
             splt.set_xticks(cbins[0])
             splt.set_xticklabels(list(curve.bins[0]))
             if curve.bins[0].dtype.kind == 'U':
-                bmax = max(len(b) for b in self.data.curves[0].bins[0])
+                bmax = max([len(b) for b in self.data.curves[0].bins[0]])
                 if bmax * self.data.curves[0].bins[0].size > 60:
                     splt.tick_params(axis='x', rotation=90)
         splt.set_ylabel(axnames[1])
         if curve.bins[1].size == curve.values.shape[1]:
             splt.set_yticks(cbins[1])
             splt.set_yticklabels(list(curve.bins[1]))
         cbar.set_label(axnames[2])
@@ -977,15 +976,15 @@
             splt.set_xlim(*self.data.attributes.limits[0])
             splt.set_ylim(*self.data.attributes.limits[1])
         if self.data.attributes.logx:
             splt.set_xscale('log')
         if self.data.attributes.logy:
             splt.set_yscale('log')
         if self.data.curves[0].bins[0].dtype.kind == 'U':
-            bmax = max(len(b) for b in self.data.curves[0].bins[0])
+            bmax = max([len(b) for b in self.data.curves[0].bins[0]])
             if bmax * self.data.curves[0].bins[0].size > 60:
                 splt.tick_params(axis='x', rotation=90)
 
 
 class _MplPie:
     '''Convert a :class:`~.templates.PlotTemplate` into a matplotlib pie chart.
     '''
```

### Comparing `valjean-0.11.0a0/valjean/javert/plot_repr.py` & `valjean-0.9.0/valjean/javert/plot_repr.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,33 +27,30 @@
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 '''Module containing all available methods to convert a test result in a table
 to be converted in rst.
 '''
-import logging
 from collections import OrderedDict
 import numpy as np
+from .. import LOGGER
 from ..cosette.task import TaskStatus
 from ..gavroche.diagnostics.stats import TestOutcome, classification_counts
 from .templates import PlotTemplate, CurveElements, SubPlotElements, join
 from .verbosity import Verbosity
 
 
 # turn off pylint warnings about invalid names in this file; there are just too
 # many long function names and they cannot be renamed because
 # javert.representation looks for them by programmatically constructing their
 # name based on the name of the test result class, the verbosity, etc.
 # pylint: disable=invalid-name
 
 
-LOGGER = logging.getLogger(__name__)
-
-
 def dimensions_from_array(array_shape):
     '''Check if array is consistent with 1D plot.
 
     Checks are done on presence of non-trivial and trivial dimensions, trivial
     being a dimension with size equal to one, non-trivial being for a dimension
     with at least two values.
 
@@ -129,20 +126,20 @@
         nbins = lbins
         has_changed = [False, False]
         limits = [nbins[0], nbins[-1]]
         if lbins.dtype.kind == 'U':
             blimits.append(tuple(limits + [False]))
             continue
         if nbins.size < 3:
-            LOGGER.note('Not enough bins to adapt range.')
+            LOGGER.warning('Not enough bins to adapt range.')
             blimits.append(tuple(limits + [False]))
             continue
         if nbins.size < 4:
-            LOGGER.note('Will adapt range for %d bins, '
-                        'binning might be not suitable', nbins.size)
+            LOGGER.warning('Will adapt range for %d bins, '
+                           'binning might be not suitable', nbins.size)
         binw = np.ediff1d(lbins)
         if binw[0]/binw[1] > max_ratio:
             limits[0] = nbins[1]
             has_changed[0] = True
         if binw[-1]/binw[-2] > max_ratio:
             limits[1] = nbins[-2]
             has_changed[1] = True
@@ -635,15 +632,15 @@
 
 def repr_testresultstatstestsbylabels(result, _verbosity=Verbosity.DEFAULT):
     '''Plot statistics on the tests classified by labels if 1 or labels.
 
     :rtype: list(PlotTemplate)
     '''
     if len(result.test.by_labels) > 2:
-        LOGGER.note('No plot for more than 2 labels.')
+        LOGGER.info('No plot for more than 2 labels.')
         return []
     if len(result.test.by_labels) == 2:
         return repr_statstestsby2labels(result)
     lok, lko, legs = ([] for i in range(3))
     for res in result.classify:
         lok.append(res['OK'])
         lko.append(res['KO'])
```

### Comparing `valjean-0.11.0a0/valjean/javert/representation.py` & `valjean-0.9.0/valjean/javert/representation.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,23 +82,20 @@
 * if customisation is needed, you can easily call the additional method
   available in :mod:`.table_repr` and :mod:`.plot_repr`;
 * you can also write your own representation method provided they follow the
   naming convention ``'repr_' + class.name``;
 * :mod:`valjean` calls the ``Representer`` classes through the
   :class:`Representation` class.
 '''
-import logging
+from .. import LOGGER
 from . import table_repr
 from . import plot_repr
 from .verbosity import Verbosity
 
 
-LOGGER = logging.getLogger(__name__)
-
-
 class Representation:
     '''Class for representing test results as templates calling the available
     representers (tables or plots).
 
     This class corresponds to the `Context` role in the `Strategy` design
     pattern.
     '''
```

### Comparing `valjean-0.11.0a0/valjean/javert/resources/rst/conf.py.template` & `valjean-0.9.0/valjean/javert/resources/rst/conf.py.template`

 * *Files identical despite different names*

### Comparing `valjean-0.11.0a0/valjean/javert/rst.py` & `valjean-0.9.0/valjean/javert/rst.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,39 +32,36 @@
 format. reStructuredText_ is a text markup language meant for easy human
 consumption. The `reStructuredText primer`_ provides a good introduction to its
 syntax.
 
 .. _reStructuredText: https://docutils.sourceforge.io/rst.html
 .. _reStructuredText primer: https://
     docutils.sourceforge.io/docs/user/rst/quickstart.html
-.. _pkg_resources: https://setuptools.pypa.io/en/latest/pkg_resources.html
 '''
 
-import logging
+
 from datetime import datetime
 from collections import defaultdict
 from pathlib import Path
 import multiprocessing as mp
 import pkg_resources as pkg
 import numpy as np
 
+from .. import LOGGER
 from ..fingerprint import fingerprint
 from ..path import ensure, sanitize_filename
 from ..cosette.task import TaskStatus
 from ..cosette.pythontask import PythonTask
 from ..gavroche.test import TestResult
 from .formatter import Formatter
 from .mpl import MplPlot
 from .test_report import TestReport, TestReportTask
 from .verbosity import Verbosity
 
 
-LOGGER = logging.getLogger(__name__)
-
-
 class Rst:
     '''Class to convert :class:`~.TestResult` objects into `reStructuredText`_
     format.'''
 
     def __init__(self, representation, *, n_workers=None):
         '''Initialize a class instance with the given representation.
 
@@ -587,15 +584,14 @@
 
 class FormattedRst:
     '''This class represents a formatted rst document tree, which typically
     consists of an index file and of several sections.
     '''
     def __init__(self, *, author, title, version,
                  tree_dict, text_dict, plots, n_workers=None):
-        # pylint: disable=too-many-arguments
         '''Create a :class:`FormattedRst` object. The `author`, `title` and
         `version` arguments are expected to be strings and are
         self-explanatory.
 
         The `tree_dict` and `text_dict` arguments must be dictionaries.  The
         `tree_dict` dictionary represents the tree structure of the
         `reStructuredText`_ document, and the `text_dict` represent the
@@ -672,15 +668,15 @@
     def _write_rec(self, *, tree, path):
 
         if tree:
             tree_path = self.tree_to_path(base=path, tree=tree)
         else:
             tree_path = path / 'index'
 
-        LOGGER.note('writing tree_path: %s', tree_path)
+        LOGGER.info('writing tree_path: %s', tree_path)
         ensure(tree_path.parent, is_dir=True)
 
         subtrees = self.tree_dict[tree]
         write_path = tree_path.with_name(tree_path.name + '.rst')
         with write_path.open('w') as tree_file:
             text = '\n'.join(self.text_dict[tree])
             tree_file.write(text)
@@ -740,15 +736,15 @@
                        formatting=False)
 
     @staticmethod
     def configure(resource, dest, formatting=True, **kwargs):
         '''Copy a package resource to the specified destination, optionally
         formatting the resource content using :meth:`str.format`.
 
-        For more information about resources, see `pkg_resources`_.
+        For more information about resources, see :doc:`pkg_resources`.
 
         :param str resource: the name of the resource.
         :param pathlib.Path dest: the destination path.
         :param bool formatting: whether formatting should be applied.
         :param dict kwargs: any additional keyword arguments will be passed to
                             the formatting.
         '''
@@ -763,29 +759,27 @@
 class RstTestReportTask(PythonTask):
     '''Task class that transforms a list of tests into a test report.
     :class:`~.TestResult` objects in the environment.'''
 
     @classmethod
     def from_tasks(cls, name, *, make_report, eval_tasks, representation,
                    author, version, kwargs=None, deps=None, soft_deps=None):
-        # pylint: disable=too-many-arguments
         '''Construct an :class:`RstTestReportTask` from a list of test
         evaluation tasks and a function to classify test results and put them
         in test reports.
         '''
         report_name = 'report-' + name
         report_task = TestReportTask(report_name, make_report=make_report,
                                      eval_tasks=eval_tasks, kwargs=kwargs)
         return cls(name, report_task=report_task,
                    representation=representation, author=author,
                    version=version, deps=deps, soft_deps=soft_deps)
 
     def __init__(self, name, *, report_task, representation, author, version,
                  deps=None, soft_deps=None):
-        # pylint: disable=too-many-arguments
 
         def write_rst(*, env, config):
             report = env[report_task.name]['result']
             if 'args' in config and 'workers' in config['args']:
                 n_workers = config['args']['workers']
                 LOGGER.debug('will use %d subprocesses to write the report',
                              n_workers)
```

### Comparing `valjean-0.11.0a0/valjean/javert/table_repr.py` & `valjean-0.9.0/valjean/javert/table_repr.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,32 +27,29 @@
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 '''Module containing all available methods to convert a test result in a table
 to be converted in rst.
 '''
-import logging
 from itertools import chain
 import numpy as np
+from .. import LOGGER
 from ..cosette.task import TaskStatus
 from ..gavroche.diagnostics.stats import TestOutcome, classification_counts
 from .templates import TableTemplate, TextTemplate
 from .verbosity import Verbosity
 
 # turn off pylint warnings about invalid names in this file; there are just too
 # many long function names and they cannot be renamed because
 # javert.representation looks for them by programmatically constructing their
 # name based on the name of the test result class, the verbosity, etc.
 # pylint: disable=invalid-name
 
 
-LOGGER = logging.getLogger(__name__)
-
-
 def repr_bins(dsref):
     '''Representation of bins in tables.
 
     When bins are given by edges, representation is ``min - max``, when they
     are given at center, representation is ``center``.
 
     Trivial dimensions are not represented, i.e. dimensions where there is only
```

### Comparing `valjean-0.11.0a0/valjean/javert/templates.py` & `valjean-0.9.0/valjean/javert/templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,19 +34,16 @@
 instance, in the case of tables this includes the column contents, the headers,
 etc.  It does **not** include any formatting information, such as column
 widths, floating-point precision, colours, etc.  Decisions about the formatting
 are handled by suitable formatting classes, such as :class:`~.Rst`.
 
 .. _numpy indexing: https://numpy.org/doc/stable/user/basics.indexing.html
 '''
-import logging
 import numpy as np
-
-
-LOGGER = logging.getLogger(__name__)
+from .. import LOGGER
 
 
 class TableTemplate:
     '''A container class that encapsulates all the necessary information to
     represent a table.
 
     Examples of use of mainly show in context of concatentation of
@@ -606,15 +603,16 @@
     def data(self):
         '''Generator yielding objects supporting the buffer protocol that (as a
         whole) represent a serialized version of `self`.'''
         for aname in self.axnames:
             yield aname.encode('utf-8')
         yield self.ptype.encode('utf-8')
         for curve in self.curves:
-            yield from curve.data()
+            for data in curve.data():
+                yield data
 
     def __eq__(self, other):
         '''Test of equality of `self` and another :class:`SubPlotElements`.'''
         return (all(s == o for s, o in zip(self.curves, other.curves))
                 and self.axnames == other.axnames
                 and self.ptype == other.ptype)
```

### Comparing `valjean-0.11.0a0/valjean/javert/test_external.py` & `valjean-0.9.0/valjean/javert/test_external.py`

 * *Files identical despite different names*

### Comparing `valjean-0.11.0a0/valjean/javert/test_report.py` & `valjean-0.9.0/valjean/javert/test_report.py`

 * *Files identical despite different names*

### Comparing `valjean-0.11.0a0/valjean/javert/verbosity.py` & `valjean-0.9.0/valjean/javert/verbosity.py`

 * *Files identical despite different names*

### Comparing `valjean-0.11.0a0/valjean/path.py` & `valjean-0.9.0/valjean/path.py`

 * *Files identical despite different names*

### Comparing `valjean-0.11.0a0/PKG-INFO` & `valjean-0.9.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,49 @@
 Metadata-Version: 2.1
 Name: valjean
-Version: 0.11.0a0
+Version: 0.9.0
 Summary: VALidation, Journal d'Évolution et ANalyse
 Home-page: https://github.com/valjean-framework/valjean
 License: CeCILL-C Free Software License Agreement (CECILL-C)
 Author: valjean developers
 Maintainer: valjean developers
 Maintainer-email: valjean-support@cea.fr
-Requires-Python: >=3.6.2,<4.0.0
+Requires-Python: >=3.6.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides-Extra: dev
 Provides-Extra: graphviz
-Requires-Dist: Sphinx (>=5.0,<5.1) ; extra == "dev"
-Requires-Dist: flake8 (<6) ; extra == "dev"
-Requires-Dist: h5py (>=3.1,<3.2) ; python_version >= "3.6" and python_version < "3.7"
-Requires-Dist: h5py (>=3.2,<4.0) ; python_version >= "3.7"
-Requires-Dist: hypothesis (>=6.31,<7.0) ; extra == "dev"
-Requires-Dist: ipykernel (>=5.5,<6.0) ; extra == "dev"
-Requires-Dist: ipython (!=8.7.0) ; extra == "dev"
-Requires-Dist: jupyter-client (>=7.1,<8.0) ; extra == "dev"
+Requires-Dist: Sphinx (>=4.3,<5.0); extra == "dev"
+Requires-Dist: flake8 (>=4.0,<5.0); extra == "dev"
+Requires-Dist: h5py (>=3.1,<3.2)
+Requires-Dist: hypothesis[numpy] (>=6.31,<7.0); extra == "dev"
+Requires-Dist: ipykernel (>=5.5,<6.0); extra == "dev"
+Requires-Dist: jupyter-client (>=7.1,<8.0); extra == "dev"
 Requires-Dist: matplotlib (>=3.3,<4.0)
-Requires-Dist: nbsphinx (>=0.8,<0.9) ; extra == "dev"
-Requires-Dist: numpy (>=1.19,<2.0) ; python_version >= "3.6" and python_version < "3.7"
-Requires-Dist: numpy (>=1.20,<2.0) ; python_version >= "3.7"
-Requires-Dist: pydot (>=1.4.2,<2.0.0) ; extra == "graphviz"
-Requires-Dist: pylint (>=2.13,<3.0) ; (python_version >= "3.6" and python_version < "3.8") and (extra == "dev")
-Requires-Dist: pylint (>=3.0,<4.0) ; (python_version >= "3.8") and (extra == "dev")
+Requires-Dist: nbsphinx (>=0.8,<0.9); extra == "dev"
+Requires-Dist: numpy (>=1.19,<2.0)
+Requires-Dist: pydot (>=1.4.2,<2.0.0); extra == "graphviz"
+Requires-Dist: pylint (>=2.12,<3.0); extra == "dev"
 Requires-Dist: pyparsing (>=3.0,<4.0)
-Requires-Dist: pytest (>=7.0,<8.0) ; extra == "dev"
-Requires-Dist: pytest-cov (>=4.0,<5.0) ; extra == "dev"
-Requires-Dist: pytest-mpl (>=0.16,<0.17) ; extra == "dev"
-Requires-Dist: pytest-timeout (>=2.0,<3.0) ; extra == "dev"
-Requires-Dist: rstcheck (>=3.3,<4.0) ; (python_version >= "3.6" and python_version < "3.7") and (extra == "dev")
-Requires-Dist: rstcheck (>=6.0,<7.0) ; (python_version >= "3.7") and (extra == "dev")
-Requires-Dist: scipy (>=1.5,<2.0) ; python_version >= "3.6" and python_version < "3.7"
-Requires-Dist: scipy (>=1.6,<2.0) ; python_version >= "3.7"
-Requires-Dist: sphinx-rtd-theme (>=1.0,<2.0) ; extra == "dev"
+Requires-Dist: pytest (>=6.2,<7.0); extra == "dev"
+Requires-Dist: pytest-cov (>=3.0,<4.0); extra == "dev"
+Requires-Dist: pytest-mpl (>=0.13,<0.14); extra == "dev"
+Requires-Dist: pytest-timeout (>=2.0,<3.0); extra == "dev"
+Requires-Dist: rstcheck (>=3.3,<4.0); extra == "dev"
+Requires-Dist: scipy (>=1.5,<2.0)
+Requires-Dist: sphinx-rtd-theme (>=1.0,<2.0); extra == "dev"
 Requires-Dist: toml (>=0.10,<0.11)
 Project-URL: Bug tracker, https://github.com/valjean-framework/valjean/issues
 Project-URL: Documentation, https://valjean.readthedocs.io/
 Project-URL: Repository, https://github.com/valjean-framework/valjean.git
 Description-Content-Type: text/markdown
 
 # Valjean #
```

