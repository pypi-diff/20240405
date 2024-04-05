# Comparing `tmp/zerohertzLib-1.0.3.tar.gz` & `tmp/zerohertzLib-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerohertzLib-1.0.3.tar", last modified: Thu Apr  4 12:29:28 2024, max compression
+gzip compressed data, was "zerohertzLib-1.0.4.tar", last modified: Fri Apr  5 09:07:00 2024, max compression
```

## Comparing `zerohertzLib-1.0.3.tar` & `zerohertzLib-1.0.4.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.465173 zerohertzLib-1.0.3/
--rw-r--r--   0 root         (0) root         (0)     1067 2024-04-04 12:29:22.000000 zerohertzLib-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-04 12:29:22.000000 zerohertzLib-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3338 2024-04-04 12:29:28.465173 zerohertzLib-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2316 2024-04-04 12:29:22.000000 zerohertzLib-1.0.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 12:29:28.465173 zerohertzLib-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2704 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.457173 zerohertzLib-1.0.3/test/
--rw-r--r--   0 root         (0) root         (0)     4501 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/test/test_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     1820 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/test/test_api.py
--rw-r--r--   0 root         (0) root         (0)     1230 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/test/test_logging.py
--rw-r--r--   0 root         (0) root         (0)      220 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/test/test_monitoring.py
--rw-r--r--   0 root         (0) root         (0)     8641 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/test/test_plot.py
--rw-r--r--   0 root         (0) root         (0)     2150 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/test/test_quant.py
--rw-r--r--   0 root         (0) root         (0)     1961 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/test/test_util.py
--rw-r--r--   0 root         (0) root         (0)    14679 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/test/test_vision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.457173 zerohertzLib-1.0.3/zerohertzLib/
--rw-r--r--   0 root         (0) root         (0)     1794 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.457173 zerohertzLib-1.0.3/zerohertzLib/algorithm/
--rw-r--r--   0 root         (0) root         (0)     1040 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/algorithm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2626 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/algorithm/bisect.py
--rw-r--r--   0 root         (0) root         (0)     6708 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/algorithm/collections.py
--rw-r--r--   0 root         (0) root         (0)     2420 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/algorithm/fft.py
--rw-r--r--   0 root         (0) root         (0)     7065 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/algorithm/graph.py
--rw-r--r--   0 root         (0) root         (0)     1676 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/algorithm/prime.py
--rw-r--r--   0 root         (0) root         (0)     8048 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/algorithm/sort.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.457173 zerohertzLib-1.0.3/zerohertzLib/api/
--rw-r--r--   0 root         (0) root         (0)      446 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3865 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/api/discord.py
--rw-r--r--   0 root         (0) root         (0)    11096 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/api/github.py
--rw-r--r--   0 root         (0) root         (0)    30846 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/api/koreainvestment.py
--rw-r--r--   0 root         (0) root         (0)     4652 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/api/open_ai.py
--rw-r--r--   0 root         (0) root         (0)     8841 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/api/slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.457173 zerohertzLib-1.0.3/zerohertzLib/logging/
--rw-r--r--   0 root         (0) root         (0)      359 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/logging/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4738 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/logging/handler.py
--rw-r--r--   0 root         (0) root         (0)     5264 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/logging/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.457173 zerohertzLib-1.0.3/zerohertzLib/mlops/
--rw-r--r--   0 root         (0) root         (0)      273 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/mlops/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18002 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/mlops/triton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.457173 zerohertzLib-1.0.3/zerohertzLib/monitoring/
--rw-r--r--   0 root         (0) root         (0)      333 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2829 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/monitoring/cpu.py
--rw-r--r--   0 root         (0) root         (0)     5184 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/monitoring/gpu.py
--rw-r--r--   0 root         (0) root         (0)     2678 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/monitoring/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.457173 zerohertzLib-1.0.3/zerohertzLib/plot/
--rw-r--r--   0 root         (0) root         (0)     1552 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/plot/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15381 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/plot/bar_chart.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.461173 zerohertzLib-1.0.3/zerohertzLib/plot/fonts/
--rw-r--r--   0 root         (0) root         (0)  7549348 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf
--rw-r--r--   0 root         (0) root         (0)   347988 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/plot/fonts/times.ttf
--rw-r--r--   0 root         (0) root         (0)     3435 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/plot/pie.py
--rw-r--r--   0 root         (0) root         (0)    11476 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/plot/plot.py
--rw-r--r--   0 root         (0) root         (0)     4046 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/plot/scatter.py
--rw-r--r--   0 root         (0) root         (0)     3292 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/plot/table.py
--rw-r--r--   0 root         (0) root         (0)     4838 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/plot/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.465173 zerohertzLib-1.0.3/zerohertzLib/quant/
--rw-r--r--   0 root         (0) root         (0)      885 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/quant/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14935 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/quant/backtest.py
--rw-r--r--   0 root         (0) root         (0)    13182 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/quant/methods.py
--rw-r--r--   0 root         (0) root         (0)    41316 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/quant/quant.py
--rw-r--r--   0 root         (0) root         (0)     3755 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/quant/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.465173 zerohertzLib-1.0.3/zerohertzLib/util/
--rw-r--r--   0 root         (0) root         (0)      458 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4527 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/util/csv.py
--rw-r--r--   0 root         (0) root         (0)    11173 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/util/data.py
--rw-r--r--   0 root         (0) root         (0)    11650 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/util/json.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.465173 zerohertzLib-1.0.3/zerohertzLib/vision/
--rw-r--r--   0 root         (0) root         (0)     1623 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/vision/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6964 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/vision/compare.py
--rw-r--r--   0 root         (0) root         (0)    12885 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/vision/convert.py
--rw-r--r--   0 root         (0) root         (0)    22648 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/vision/data.py
--rw-r--r--   0 root         (0) root         (0)    14878 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/vision/eval.py
--rw-r--r--   0 root         (0) root         (0)     4188 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/vision/gif.py
--rw-r--r--   0 root         (0) root         (0)    22281 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/vision/loader.py
--rw-r--r--   0 root         (0) root         (0)     7170 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/vision/transform.py
--rw-r--r--   0 root         (0) root         (0)     4219 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/vision/util.py
--rw-r--r--   0 root         (0) root         (0)    17510 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/vision/visual.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.457173 zerohertzLib-1.0.3/zerohertzLib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3338 2024-04-04 12:29:28.000000 zerohertzLib-1.0.3/zerohertzLib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1923 2024-04-04 12:29:28.000000 zerohertzLib-1.0.3/zerohertzLib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 12:29:28.000000 zerohertzLib-1.0.3/zerohertzLib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      430 2024-04-04 12:29:28.000000 zerohertzLib-1.0.3/zerohertzLib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-04 12:29:28.000000 zerohertzLib-1.0.3/zerohertzLib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.428856 zerohertzLib-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-04-05 09:06:54.000000 zerohertzLib-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-05 09:06:54.000000 zerohertzLib-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3338 2024-04-05 09:07:00.428856 zerohertzLib-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2316 2024-04-05 09:06:54.000000 zerohertzLib-1.0.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 09:07:00.428856 zerohertzLib-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2704 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.416856 zerohertzLib-1.0.4/test/
+-rw-r--r--   0 root         (0) root         (0)     4501 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/test/test_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/test/test_api.py
+-rw-r--r--   0 root         (0) root         (0)     1230 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/test/test_logging.py
+-rw-r--r--   0 root         (0) root         (0)      220 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/test/test_monitoring.py
+-rw-r--r--   0 root         (0) root         (0)     8641 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/test/test_plot.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/test/test_quant.py
+-rw-r--r--   0 root         (0) root         (0)     1961 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/test/test_util.py
+-rw-r--r--   0 root         (0) root         (0)    14679 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/test/test_vision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.420856 zerohertzLib-1.0.4/zerohertzLib/
+-rw-r--r--   0 root         (0) root         (0)     1794 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.420856 zerohertzLib-1.0.4/zerohertzLib/algorithm/
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/algorithm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/algorithm/bisect.py
+-rw-r--r--   0 root         (0) root         (0)     6708 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/algorithm/collections.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/algorithm/fft.py
+-rw-r--r--   0 root         (0) root         (0)     7065 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/algorithm/graph.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/algorithm/prime.py
+-rw-r--r--   0 root         (0) root         (0)     8048 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/algorithm/sort.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.420856 zerohertzLib-1.0.4/zerohertzLib/api/
+-rw-r--r--   0 root         (0) root         (0)      446 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3865 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/api/discord.py
+-rw-r--r--   0 root         (0) root         (0)    11096 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/api/github.py
+-rw-r--r--   0 root         (0) root         (0)    30846 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/api/koreainvestment.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/api/open_ai.py
+-rw-r--r--   0 root         (0) root         (0)     8841 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/api/slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.420856 zerohertzLib-1.0.4/zerohertzLib/logging/
+-rw-r--r--   0 root         (0) root         (0)      359 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/logging/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4738 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/logging/handler.py
+-rw-r--r--   0 root         (0) root         (0)     5264 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/logging/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.420856 zerohertzLib-1.0.4/zerohertzLib/mlops/
+-rw-r--r--   0 root         (0) root         (0)      273 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/mlops/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18002 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/mlops/triton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.420856 zerohertzLib-1.0.4/zerohertzLib/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      333 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2829 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/monitoring/cpu.py
+-rw-r--r--   0 root         (0) root         (0)     5184 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/monitoring/gpu.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/monitoring/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.420856 zerohertzLib-1.0.4/zerohertzLib/plot/
+-rw-r--r--   0 root         (0) root         (0)     1552 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/plot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15381 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/plot/bar_chart.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.424856 zerohertzLib-1.0.4/zerohertzLib/plot/fonts/
+-rw-r--r--   0 root         (0) root         (0)  7549348 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf
+-rw-r--r--   0 root         (0) root         (0)   347988 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/plot/fonts/times.ttf
+-rw-r--r--   0 root         (0) root         (0)     3435 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/plot/pie.py
+-rw-r--r--   0 root         (0) root         (0)    11476 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/plot/plot.py
+-rw-r--r--   0 root         (0) root         (0)     4046 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/plot/scatter.py
+-rw-r--r--   0 root         (0) root         (0)     3292 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/plot/table.py
+-rw-r--r--   0 root         (0) root         (0)     4838 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/plot/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.424856 zerohertzLib-1.0.4/zerohertzLib/quant/
+-rw-r--r--   0 root         (0) root         (0)      885 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/quant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14935 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/quant/backtest.py
+-rw-r--r--   0 root         (0) root         (0)    13182 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/quant/methods.py
+-rw-r--r--   0 root         (0) root         (0)    45370 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/quant/quant.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/quant/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.424856 zerohertzLib-1.0.4/zerohertzLib/util/
+-rw-r--r--   0 root         (0) root         (0)      458 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4527 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/util/csv.py
+-rw-r--r--   0 root         (0) root         (0)    11173 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/util/data.py
+-rw-r--r--   0 root         (0) root         (0)    11650 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/util/json.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.428856 zerohertzLib-1.0.4/zerohertzLib/vision/
+-rw-r--r--   0 root         (0) root         (0)     1623 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/vision/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6967 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/vision/compare.py
+-rw-r--r--   0 root         (0) root         (0)    12885 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/vision/convert.py
+-rw-r--r--   0 root         (0) root         (0)    22648 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/vision/data.py
+-rw-r--r--   0 root         (0) root         (0)    14878 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/vision/eval.py
+-rw-r--r--   0 root         (0) root         (0)     4188 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/vision/gif.py
+-rw-r--r--   0 root         (0) root         (0)    22281 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/vision/loader.py
+-rw-r--r--   0 root         (0) root         (0)     7826 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/vision/transform.py
+-rw-r--r--   0 root         (0) root         (0)     4219 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/vision/util.py
+-rw-r--r--   0 root         (0) root         (0)    17516 2024-04-05 09:06:55.000000 zerohertzLib-1.0.4/zerohertzLib/vision/visual.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:07:00.420856 zerohertzLib-1.0.4/zerohertzLib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3338 2024-04-05 09:07:00.000000 zerohertzLib-1.0.4/zerohertzLib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1923 2024-04-05 09:07:00.000000 zerohertzLib-1.0.4/zerohertzLib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 09:07:00.000000 zerohertzLib-1.0.4/zerohertzLib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      430 2024-04-05 09:07:00.000000 zerohertzLib-1.0.4/zerohertzLib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-05 09:07:00.000000 zerohertzLib-1.0.4/zerohertzLib.egg-info/top_level.txt
```

### Comparing `zerohertzLib-1.0.3/LICENSE` & `zerohertzLib-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/PKG-INFO` & `zerohertzLib-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerohertzLib
-Version: 1.0.3
+Version: 1.0.4
 Summary: Zerohertz's Library
 Home-page: https://github.com/Zerohertz/zerohertzLib
 Author: Zerohertz
 Author-email: ohg3417@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.3 Summary: Zerohertz's
+Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.4 Summary: Zerohertz's
 Library Home-page: https://github.com/Zerohertz/zerohertzLib Author: Zerohertz
 Author-email: ohg3417@gmail.com License: MIT Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
```

### Comparing `zerohertzLib-1.0.3/README.md` & `zerohertzLib-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/setup.py` & `zerohertzLib-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/test/test_algorithm.py` & `zerohertzLib-1.0.4/test/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/test/test_api.py` & `zerohertzLib-1.0.4/test/test_api.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/test/test_logging.py` & `zerohertzLib-1.0.4/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/test/test_plot.py` & `zerohertzLib-1.0.4/test/test_plot.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/test/test_quant.py` & `zerohertzLib-1.0.4/test/test_quant.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/test/test_util.py` & `zerohertzLib-1.0.4/test/test_util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/test/test_vision.py` & `zerohertzLib-1.0.4/test/test_vision.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/__init__.py` & `zerohertzLib-1.0.4/zerohertzLib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,8 +52,8 @@
     print("=" * 100)
     print(f"[Warning] {error}")
     print("Please Install OpenCV Dependency")
     print("--->\t$ sudo apt install python3-opencv -y\t<---")
     print("(but you can use other submodules except zerohertzLib.vision)")
     print("=" * 100)
 
-__version__ = "v1.0.3"
+__version__ = "v1.0.4"
```

### Comparing `zerohertzLib-1.0.3/zerohertzLib/algorithm/__init__.py` & `zerohertzLib-1.0.4/zerohertzLib/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/algorithm/bisect.py` & `zerohertzLib-1.0.4/zerohertzLib/algorithm/bisect.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/algorithm/collections.py` & `zerohertzLib-1.0.4/zerohertzLib/algorithm/collections.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/algorithm/fft.py` & `zerohertzLib-1.0.4/zerohertzLib/algorithm/fft.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/algorithm/graph.py` & `zerohertzLib-1.0.4/zerohertzLib/algorithm/graph.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/algorithm/prime.py` & `zerohertzLib-1.0.4/zerohertzLib/algorithm/prime.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/algorithm/sort.py` & `zerohertzLib-1.0.4/zerohertzLib/algorithm/sort.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/api/discord.py` & `zerohertzLib-1.0.4/zerohertzLib/api/discord.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/api/github.py` & `zerohertzLib-1.0.4/zerohertzLib/api/github.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/api/koreainvestment.py` & `zerohertzLib-1.0.4/zerohertzLib/api/koreainvestment.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/api/open_ai.py` & `zerohertzLib-1.0.4/zerohertzLib/api/open_ai.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/api/slack.py` & `zerohertzLib-1.0.4/zerohertzLib/api/slack.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/logging/handler.py` & `zerohertzLib-1.0.4/zerohertzLib/logging/handler.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/logging/logger.py` & `zerohertzLib-1.0.4/zerohertzLib/logging/logger.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/mlops/triton.py` & `zerohertzLib-1.0.4/zerohertzLib/mlops/triton.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/monitoring/cpu.py` & `zerohertzLib-1.0.4/zerohertzLib/monitoring/cpu.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/monitoring/gpu.py` & `zerohertzLib-1.0.4/zerohertzLib/monitoring/gpu.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/monitoring/storage.py` & `zerohertzLib-1.0.4/zerohertzLib/monitoring/storage.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/plot/__init__.py` & `zerohertzLib-1.0.4/zerohertzLib/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/plot/bar_chart.py` & `zerohertzLib-1.0.4/zerohertzLib/plot/bar_chart.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf` & `zerohertzLib-1.0.4/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/plot/fonts/times.ttf` & `zerohertzLib-1.0.4/zerohertzLib/plot/fonts/times.ttf`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/plot/pie.py` & `zerohertzLib-1.0.4/zerohertzLib/plot/pie.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/plot/plot.py` & `zerohertzLib-1.0.4/zerohertzLib/plot/plot.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/plot/scatter.py` & `zerohertzLib-1.0.4/zerohertzLib/plot/scatter.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/plot/table.py` & `zerohertzLib-1.0.4/zerohertzLib/plot/table.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/plot/util.py` & `zerohertzLib-1.0.4/zerohertzLib/plot/util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/quant/__init__.py` & `zerohertzLib-1.0.4/zerohertzLib/quant/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/quant/backtest.py` & `zerohertzLib-1.0.4/zerohertzLib/quant/backtest.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/quant/methods.py` & `zerohertzLib-1.0.4/zerohertzLib/quant/methods.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/quant/quant.py` & `zerohertzLib-1.0.4/zerohertzLib/quant/quant.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,27 +26,30 @@
 import multiprocessing as mp
 import time
 import traceback
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from datetime import datetime, timedelta
 from itertools import combinations
-from typing import Any, Dict, ItemsView, List, Optional, Tuple, Union
+from typing import Any, Dict, ItemsView, List, Optional, Tuple, TypeVar, Union
 
 import FinanceDataReader as fdr
 import pandas as pd
 import requests
 from matplotlib import pyplot as plt
+from matplotlib import ticker
 
 from zerohertzLib.api import KoreaInvestment, SlackBot
 from zerohertzLib.plot import barh, barv, candle, figure, hist, pie, savefig, table
 
 from .backtest import Experiments, backtest
 from .util import _cash2str, _method2str, _seconds_to_hms
 
+T = TypeVar("T", bound="Balance")
+
 
 class Quant(Experiments):
     """한 가지 종목에 대해 full factorial design 기반의 backtest를 수행하고 최적의 전략을 융합하는 class
 
     Args:
         title (``str``): 종목 이름
         data (``pd.DataFrame``): OHLCV (Open, High, Low, Close, Volume) data
@@ -283,28 +286,28 @@
             >>> "삼성전자" in balance
             False
             >>> len(balance)
             1
             >>> balance[0]
             ['066570', 102200.0, 100200, 1, -1.95, -2000]
             >>> balance()
-            1997997
+            000
 
         ``kor=False``:
             >>> balance = zz.quant.Balance("00000000-00", kor=False)
             >>> "아마존닷컴" in balance
             True
             >>> "삼성전자" in balance
             False
             >>> len(balance)
             1
             >>> balance[0]
-            ['AMZN', 145.98, 146.5, 1, 0.36, 146.5]
+            ['META', 488.74, 510.92, 1, 4.53, 22.18]
             >>> balance()
-            146.5
+            000.000
     """
 
     def __init__(
         self, account_no: str, path: Optional[str] = "./", kor: Optional[bool] = True
     ) -> None:
         super().__init__(account_no, path)
         self.balance = {"stock": defaultdict(list)}
@@ -380,14 +383,93 @@
         Returns:
             ``float``: USD/KRW의 현재 시세
         """
         now = datetime.now()
         data = fdr.DataReader("USD/KRW", now - timedelta(days=10))
         return data.Close[-1]
 
+    def merge(self, balance: T) -> None:
+        """현재 계좌와 입력 계좌의 정보를 병합하는 함수
+
+        Args:
+            balance (``zerohertzLib.quant.Balance``): 병합될 계좌 정보
+
+        Returns:
+            ``None``: 현재 계좌에 정보 update
+
+        Examples:
+            >>> balance_1.merge(balance_2)
+        """
+        merged_balance = balance.balance.copy()
+        if self.kor != balance.kor:
+            exchange = self._exchange()
+            if self.kor:
+                for key, value in balance.items():
+                    merged_balance["stock"][key][1] = value[1] * exchange
+                    merged_balance["stock"][key][2] = value[2] * exchange
+                    merged_balance["stock"][key][-1] = value[-1] * exchange
+                merged_balance["cash"] = balance.balance["cash"] * exchange
+            else:
+                for key, value in balance.items():
+                    merged_balance["stock"][key][1] = value[1] / exchange
+                    merged_balance["stock"][key][2] = value[2] / exchange
+                    merged_balance["stock"][key][-1] = value[-1] / exchange
+                merged_balance["cash"] = balance.balance["cash"] / exchange
+        for key, value in merged_balance["stock"].items():
+            if key in self:
+                (
+                    _merged_code,
+                    _merged_buy_price,
+                    _merged_present_price,
+                    _merged_cnt,
+                    _merged_pandl_per,
+                    _merged_pandl_abs,
+                ) = self.balance["stock"][key]
+                (
+                    _tmp_code,
+                    _tmp_buy_price,
+                    _tmp_present_price,
+                    _tmp_cnt,
+                    _tmp_pandl_per,
+                    _tmp_pandl_abs,
+                ) = value
+                assert _merged_code == _tmp_code
+                _merged_buy_price = (
+                    _merged_buy_price * _merged_cnt + _tmp_buy_price * _tmp_cnt
+                ) / (_merged_cnt + _tmp_cnt)
+                _merged_present_price = (_merged_present_price + _tmp_present_price) / 2
+                _merged_cnt += _tmp_cnt
+                _merged_pandl_abs = (
+                    _merged_present_price - _merged_buy_price
+                ) * _merged_cnt
+                _merged_pandl_per = (
+                    (_merged_present_price - _merged_buy_price)
+                    / _merged_buy_price
+                    * 100
+                )
+                self.balance["stock"][key] = [
+                    _merged_code,
+                    _merged_buy_price,
+                    _merged_present_price,
+                    _merged_cnt,
+                    _merged_pandl_per,
+                    _merged_pandl_abs,
+                ]
+            else:
+                self.symbols.append(key)
+                self.balance["stock"][key] = value
+        self.balance["cash"] += merged_balance["cash"]
+        self.balance["stock"] = dict(
+            sorted(
+                self.balance["stock"].items(),
+                key=lambda item: item[1][1] * item[1][3],
+                reverse=True,
+            )
+        )
+
     def items(self) -> ItemsView[str, List[Union[int, float, str]]]:
         """보유 주식의 반복문 사용을 위한 method
 
         Returns:
             ``ItemsView[str, List[Union[int, float, str]]]``: 보유 종목 code와 그에 따른 정보들
 
         Examples:
@@ -491,19 +573,50 @@
             dim = "₩"
         else:
             dim = "$"
         data = defaultdict(float)
         data["Cash"] = 0
         for name, value in self.items():
             _, purchase, _, quantity, _, _ = value
-            data[f"{name}"] = purchase * quantity
+            data[name] = purchase * quantity
         cash = self() - sum(data.values())
         data["Cash"] = max(data["Cash"], cash)
         return pie(data, dim, title="Portfolio", dpi=100, int_label=self.kor)
 
+    def barv(self) -> str:
+        """현재 보유 종목의 이익과 손실을 bar chart로 시각화
+
+        Returns:
+            ``str``: 저장된 graph의 절대 경로
+
+        Examples:
+            >>> balance.barv()
+        """
+        if self.kor:
+            dim = "₩"
+        else:
+            dim = "$"
+        data = {}
+        for value in self:
+            data[value[0]] = value[5]
+        figure((30, 10))
+        barv(
+            data,
+            xlab="",
+            ylab=f"Profit and Loss (P&L) [{dim}]",
+            title="",
+            dim="",
+            dimsize=16,
+            save=False,
+        )
+        plt.gca().yaxis.set_major_formatter(
+            ticker.FuncFormatter(lambda x, p: format(int(x), ","))
+        )
+        return savefig("ProfitLoss", 100)
+
 
 class QuantSlackBot(ABC, SlackBot):
     """입력된 여러 종목에 대해 매수, 매도 signal을 판단하고 Slack으로 message와 graph를 전송하는 class
 
     Note:
         Abstract Base Class: 종목 code에 따른 종목명과 data를 불러오는 abstract method ``_get_data`` 정의 후 사용
```

### Comparing `zerohertzLib-1.0.3/zerohertzLib/quant/util.py` & `zerohertzLib-1.0.4/zerohertzLib/quant/util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/util/csv.py` & `zerohertzLib-1.0.4/zerohertzLib/util/csv.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/util/data.py` & `zerohertzLib-1.0.4/zerohertzLib/util/data.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/util/json.py` & `zerohertzLib-1.0.4/zerohertzLib/util/json.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/vision/__init__.py` & `zerohertzLib-1.0.4/zerohertzLib/vision/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/vision/compare.py` & `zerohertzLib-1.0.4/zerohertzLib/vision/compare.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         x_0, y_0, x_1, y_1 = (
             d_x * length,
             d_y * length,
             (d_x + 1) * length,
             (d_y + 1) * length,
         )
         img = _cvt_bgra(img)
-        palette[y_0:y_1, x_0:x_1, :] = pad(img, (length, length), color)
+        palette[y_0:y_1, x_0:x_1, :], _ = pad(img, (length, length), color)
     cv2.imwrite(f"{file_name}.png", palette)
 
 
 def vert(
     imgs: List[NDArray[np.uint8]],
     height: Optional[int] = 1000,
     file_name: Optional[str] = "tmp",
```

### Comparing `zerohertzLib-1.0.3/zerohertzLib/vision/convert.py` & `zerohertzLib-1.0.4/zerohertzLib/vision/convert.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/vision/data.py` & `zerohertzLib-1.0.4/zerohertzLib/vision/data.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/vision/eval.py` & `zerohertzLib-1.0.4/zerohertzLib/vision/eval.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/vision/gif.py` & `zerohertzLib-1.0.4/zerohertzLib/vision/gif.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/vision/loader.py` & `zerohertzLib-1.0.4/zerohertzLib/vision/loader.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/vision/transform.py` & `zerohertzLib-1.0.4/zerohertzLib/vision/transform.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,51 +34,62 @@
 
 
 def pad(
     img: NDArray[np.uint8],
     shape: Tuple[int],
     color: Optional[Tuple[int]] = (255, 255, 255),
     poly: Optional[NDArray[DTypeLike]] = None,
-) -> Union[NDArray[np.uint8], Tuple[NDArray[np.uint8], NDArray[DTypeLike]]]:
+) -> Tuple[NDArray[np.uint8], Union[Tuple[float, int, int], NDArray[DTypeLike]]]:
     """입력 image를 원하는 shape로 resize 및 pad
 
     Args:
         img (``NDArray[np.uint8]``): 입력 image (``[H, W, C]``)
         shape (``Tuple[int]``): 출력의 shape ``(H, W)``
         color (``Optional[Tuple[int]]``): Padding의 색
         poly (``Optional[NDArray[DTypeLike]]``): Padding에 따라 변형될 좌표 (``[N, 2]``)
 
     Returns:
-        ``Union[NDArray[np.uint8], Tuple[NDArray[np.uint8], NDArray[DTypeLike]]]``: 출력 image (``[H, W, C]``) 및 ``poly`` 입력 시 padding에 따른 변형된 좌표값
+        ``Tuple[NDArray[np.uint8], Union[Tuple[float, int, int], NDArray[DTypeLike]]]``: 출력 image (``[H, W, C]``) 및 padding에 따른 정보 또는 변형된 좌표값
+
+    Note:
+        ``poly`` 를 입력하지 않을 시 ``(ratio, left, top)`` 가 출력되며 ``poly * ratio + (left, top)`` 와 같이 차후에 변환 가능
 
     Examples:
         GRAY:
             >>> img = cv2.cvtColor(img, cv2.COLOR_BGRA2GRAY)
             >>> res1 = cv2.resize(img, (500, 1000))
-            >>> res1 = zz.vision.pad(res1, (1000, 1000), color=(0, 255, 0))
+            >>> res1, _ = zz.vision.pad(res1, (1000, 1000), color=(0, 255, 0))
 
         BGR:
             >>> res2 = cv2.resize(img, (1000, 500))
-            >>> res2 = zz.vision.pad(res2, (1000, 1000))
+            >>> res2, _ = zz.vision.pad(res2, (1000, 1000))
 
         BGRA:
             >>> img = cv2.cvtColor(img, cv2.COLOR_BGR2BGRA)
             >>> res3 = cv2.resize(img, (500, 1000))
-            >>> res3 = zz.vision.pad(res3, (1000, 1000), color=(0, 0, 255, 128))
+            >>> res3, _ = zz.vision.pad(res3, (1000, 1000), color=(0, 0, 255, 128))
 
         Poly:
             >>> poly = np.array([[100, 400], [400, 400], [800, 900], [400, 1100], [100, 800]])
             >>> res4 = cv2.resize(img, (2000, 1000))
             >>> res4 = zz.vision.bbox(res4, poly, color=(255, 0, 0), thickness=20)
             >>> res4, poly = zz.vision.pad(res4, (1000, 1000), poly=poly)
-            >>> res4 = zz.vision.bbox(img, poly, color=(0, 0, 255))
+            >>> res4 = zz.vision.bbox(res4, poly, color=(0, 0, 255))
+
+        Transformation:
+            >>> poly = np.array([[100, 400], [400, 400], [800, 900], [400, 1100], [100, 800]])
+            >>> res5 = cv2.resize(img, (2000, 1000))
+            >>> res5 = zz.vision.bbox(res5, poly, color=(255, 0, 0), thickness=20)
+            >>> res5, info = zz.vision.pad(res5, (1000, 1000), color=(128, 128, 128))
+            >>> poly = poly * info[0] + info[1:]
+            >>> res5 = zz.vision.bbox(res5, poly, color=(0, 0, 255))
 
         .. image:: _static/examples/dynamic/vision.pad.png
             :align: center
-            :width: 600px
+            :width: 700px
     """
     if len(img.shape) == 2:
         img = cv2.cvtColor(img, cv2.COLOR_GRAY2BGR)
     if img.shape[2] == 4 and len(color) == 3:
         color = [*color, 255]
     img_height, img_width = img.shape[:2]
     tar_height, tar_width = shape
@@ -106,15 +117,15 @@
         (tar_width - resize_width) // 2,
         (tar_width - resize_width) // 2 + (tar_width - resize_width) % 2,
     )
     img = cv2.copyMakeBorder(
         img, top, bottom, left, right, cv2.BORDER_CONSTANT, value=color
     )
     if poly is None:
-        return img
+        return img, (ratio, left, top)
     return img, poly * ratio + (left, top)
 
 
 def cutout(
     img: NDArray[np.uint8],
     poly: Union[List[Union[int, float]], NDArray[DTypeLike]],
     alpha: Optional[int] = 255,
```

### Comparing `zerohertzLib-1.0.3/zerohertzLib/vision/util.py` & `zerohertzLib-1.0.4/zerohertzLib/vision/util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.3/zerohertzLib/vision/visual.py` & `zerohertzLib-1.0.4/zerohertzLib/vision/visual.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,15 @@
     d_x, d_y = (size[0] - text_width) // 2, (size[1] - text_height) // 2
     if d_x < 0 or d_y < 0:
         raise ValueError("Input text 'txt' is too long")
     x_0, x_1 = d_x, d_x + text_width
     y_0, y_1 = d_y, d_y + text_height
     draw.text((d_x, d_y), txt, font=font, fill=(*color, 255))
     palette = np.array(palette)[y_0:y_1, x_0:x_1, :]
-    return pad(palette, shape, (0, 0, 0, 0))
+    return pad(palette, shape, (0, 0, 0, 0))[0]
 
 
 def _text(
     img: NDArray[np.uint8],
     box_cwh: NDArray[DTypeLike],
     txt: str,
     color: Tuple[int],
@@ -445,15 +445,15 @@
         target = cv2.resize(
             target, (box_width, box_height), interpolation=cv2.INTER_LINEAR
         )
         if poly is not None:
             poly = poly * (box_width / tar_width, box_height / tar_height) + (x_0, y_0)
     else:
         if poly is None:
-            target = pad(target, (box_height, box_width), (0, 0, 0, 0))
+            target, _ = pad(target, (box_height, box_width), (0, 0, 0, 0))
         else:
             target, poly = pad(target, (box_height, box_width), (0, 0, 0, 0), poly)
             poly += (x_0, y_0)
     img[y_0:y_1, x_0:x_1, :] = _paste(img[y_0:y_1, x_0:x_1, :], target)
     if vis:
         box = np.array([[x_0, y_0], [x_0, y_1], [x_1, y_1], [x_1, y_0]])
         img = _bbox(img, box, (0, 0, 255, 255), 2)
```

### Comparing `zerohertzLib-1.0.3/zerohertzLib.egg-info/PKG-INFO` & `zerohertzLib-1.0.4/zerohertzLib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerohertzLib
-Version: 1.0.3
+Version: 1.0.4
 Summary: Zerohertz's Library
 Home-page: https://github.com/Zerohertz/zerohertzLib
 Author: Zerohertz
 Author-email: ohg3417@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.3 Summary: Zerohertz's
+Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.4 Summary: Zerohertz's
 Library Home-page: https://github.com/Zerohertz/zerohertzLib Author: Zerohertz
 Author-email: ohg3417@gmail.com License: MIT Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
```

### Comparing `zerohertzLib-1.0.3/zerohertzLib.egg-info/SOURCES.txt` & `zerohertzLib-1.0.4/zerohertzLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

