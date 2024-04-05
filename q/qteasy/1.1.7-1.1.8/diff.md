# Comparing `tmp/qteasy-1.1.7.tar.gz` & `tmp/qteasy-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jackie/Projects/qteasy/dist/.tmp-4rbxi8sd/qteasy-1.1.7.tar", last modified: Wed Apr  3 01:40:56 2024, max compression
+gzip compressed data, was "/Users/jackie/Projects/qteasy/dist/.tmp-gdqa728x/qteasy-1.1.8.tar", last modified: Fri Apr  5 14:24:31 2024, max compression
```

## Comparing `qteasy-1.1.7.tar` & `qteasy-1.1.8.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-03 01:40:56.000000 qteasy-1.1.7/
--rwxr-xr-x   0 jackie     (501) staff       (20)     1463 2024-03-07 04:23:42.000000 qteasy-1.1.7/LICENSE
--rw-r--r--   0 jackie     (501) staff       (20)    27759 2024-04-03 01:40:56.000000 qteasy-1.1.7/PKG-INFO
--rwxr-xr-x   0 jackie     (501) staff       (20)    24521 2024-04-03 01:04:36.000000 qteasy-1.1.7/README.md
--rw-r--r--   0 jackie     (501) staff       (20)     2181 2024-04-03 01:25:45.000000 qteasy-1.1.7/pyproject.toml
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-03 01:40:56.000000 qteasy-1.1.7/qteasy/
--rwxr-xr-x   0 jackie     (501) staff       (20)     8505 2024-04-03 01:04:36.000000 qteasy-1.1.7/qteasy/__init__.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    66919 2024-04-02 02:35:24.000000 qteasy-1.1.7/qteasy/_arg_validators.py
--rw-r--r--   0 jackie     (501) staff       (20)    52573 2024-04-02 02:35:24.000000 qteasy-1.1.7/qteasy/backtest.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    35193 2024-04-02 14:31:55.000000 qteasy-1.1.7/qteasy/blender.py
--rw-r--r--   0 jackie     (501) staff       (20)    30242 2024-04-02 14:50:54.000000 qteasy-1.1.7/qteasy/broker.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   142287 2024-04-02 14:31:45.000000 qteasy-1.1.7/qteasy/built_in.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   109769 2024-04-03 01:38:59.000000 qteasy-1.1.7/qteasy/core.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   380638 2024-04-02 14:33:07.000000 qteasy-1.1.7/qteasy/database.py
--rw-r--r--   0 jackie     (501) staff       (20)     9341 2024-04-02 14:50:54.000000 qteasy-1.1.7/qteasy/emfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    33669 2024-04-02 14:32:34.000000 qteasy-1.1.7/qteasy/evaluate.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    37779 2024-04-03 01:12:45.000000 qteasy-1.1.7/qteasy/finance.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   101000 2024-04-02 14:28:54.000000 qteasy-1.1.7/qteasy/history.py
--rw-r--r--   0 jackie     (501) staff       (20)    39218 2024-04-02 14:32:16.000000 qteasy-1.1.7/qteasy/optimization.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   107901 2024-04-02 14:31:31.000000 qteasy-1.1.7/qteasy/qt_operator.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    33875 2024-04-02 02:35:24.000000 qteasy-1.1.7/qteasy/space.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    88152 2024-04-02 02:35:24.000000 qteasy-1.1.7/qteasy/strategy.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   151551 2024-04-02 02:35:24.000000 qteasy-1.1.7/qteasy/tafuncs.py
--rw-r--r--   0 jackie     (501) staff       (20)    47486 2024-04-02 02:35:24.000000 qteasy-1.1.7/qteasy/trade_recording.py
--rw-r--r--   0 jackie     (501) staff       (20)   180412 2024-04-02 02:35:24.000000 qteasy-1.1.7/qteasy/trader.py
--rw-r--r--   0 jackie     (501) staff       (20)    67732 2024-04-02 02:35:24.000000 qteasy-1.1.7/qteasy/trading_util.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   140763 2024-04-02 02:35:24.000000 qteasy-1.1.7/qteasy/tsfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    74256 2024-04-03 01:38:59.000000 qteasy-1.1.7/qteasy/utilfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    79732 2024-04-02 02:35:24.000000 qteasy-1.1.7/qteasy/visual.py
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-03 01:40:56.000000 qteasy-1.1.7/qteasy.egg-info/
--rw-r--r--   0 jackie     (501) staff       (20)    27759 2024-04-03 01:40:56.000000 qteasy-1.1.7/qteasy.egg-info/PKG-INFO
--rw-r--r--   0 jackie     (501) staff       (20)     1192 2024-04-03 01:40:56.000000 qteasy-1.1.7/qteasy.egg-info/SOURCES.txt
--rw-r--r--   0 jackie     (501) staff       (20)        1 2024-04-03 01:40:56.000000 qteasy-1.1.7/qteasy.egg-info/dependency_links.txt
--rw-r--r--   0 jackie     (501) staff       (20)        1 2023-01-29 16:03:37.000000 qteasy-1.1.7/qteasy.egg-info/not-zip-safe
--rw-r--r--   0 jackie     (501) staff       (20)      154 2024-04-03 01:40:56.000000 qteasy-1.1.7/qteasy.egg-info/requires.txt
--rw-r--r--   0 jackie     (501) staff       (20)        7 2024-04-03 01:40:56.000000 qteasy-1.1.7/qteasy.egg-info/top_level.txt
--rw-r--r--   0 jackie     (501) staff       (20)     1515 2024-04-03 01:40:56.000000 qteasy-1.1.7/setup.cfg
--rw-r--r--   0 jackie     (501) staff       (20)      257 2024-04-01 14:38:19.000000 qteasy-1.1.7/setup.py
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-03 01:40:56.000000 qteasy-1.1.7/tests/
--rw-r--r--   0 jackie     (501) staff       (20)     6524 2024-03-29 13:24:03.000000 qteasy-1.1.7/tests/test_broker.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     8091 2023-02-23 16:04:07.000000 qteasy-1.1.7/tests/test_cashplan.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     3613 2023-11-25 05:35:56.000000 qteasy-1.1.7/tests/test_config.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    17487 2024-04-02 23:40:52.000000 qteasy-1.1.7/tests/test_core_sub_funcs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    17540 2024-03-16 06:43:01.000000 qteasy-1.1.7/tests/test_cost.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   105972 2024-04-02 23:45:06.000000 qteasy-1.1.7/tests/test_datasource.py
--rw-r--r--   0 jackie     (501) staff       (20)     6143 2024-02-03 15:46:14.000000 qteasy-1.1.7/tests/test_eastmoney.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    73675 2023-01-29 16:18:32.000000 qteasy-1.1.7/tests/test_evaluations.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    13901 2024-02-03 15:46:14.000000 qteasy-1.1.7/tests/test_fast_experiments.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    57759 2024-03-29 10:03:15.000000 qteasy-1.1.7/tests/test_historypanel.py
--rwxr-xr-x   0 jackie     (501) staff       (20)      413 2023-01-29 16:18:32.000000 qteasy-1.1.7/tests/test_log.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   326237 2024-03-16 06:43:01.000000 qteasy-1.1.7/tests/test_loop.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   169128 2024-03-02 15:43:47.000000 qteasy-1.1.7/tests/test_operator_and_strategy.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    44354 2024-03-30 13:43:29.000000 qteasy-1.1.7/tests/test_qt.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    18581 2023-01-29 16:18:32.000000 qteasy-1.1.7/tests/test_space.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    39724 2024-03-08 14:36:48.000000 qteasy-1.1.7/tests/test_ta_funcs.py
--rw-r--r--   0 jackie     (501) staff       (20)    43391 2024-04-02 03:20:22.000000 qteasy-1.1.7/tests/test_trader.py
--rw-r--r--   0 jackie     (501) staff       (20)    42445 2024-04-02 03:20:22.000000 qteasy-1.1.7/tests/test_trader_shell.py
--rw-r--r--   0 jackie     (501) staff       (20)   159405 2024-04-02 03:20:22.000000 qteasy-1.1.7/tests/test_trading.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    21881 2024-03-30 12:31:29.000000 qteasy-1.1.7/tests/test_tushare.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    43297 2023-12-06 18:45:12.000000 qteasy-1.1.7/tests/test_utilityfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     3090 2023-01-29 16:18:32.000000 qteasy-1.1.7/tests/test_visual.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-05 14:24:31.000000 qteasy-1.1.8/
+-rwxr-xr-x   0 jackie     (501) staff       (20)     1463 2024-03-07 04:23:42.000000 qteasy-1.1.8/LICENSE
+-rw-r--r--   0 jackie     (501) staff       (20)    27759 2024-04-05 14:24:31.000000 qteasy-1.1.8/PKG-INFO
+-rwxr-xr-x   0 jackie     (501) staff       (20)    24521 2024-04-05 07:48:40.000000 qteasy-1.1.8/README.md
+-rw-r--r--   0 jackie     (501) staff       (20)     2181 2024-04-05 07:48:40.000000 qteasy-1.1.8/pyproject.toml
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-05 14:24:31.000000 qteasy-1.1.8/qteasy/
+-rwxr-xr-x   0 jackie     (501) staff       (20)     8505 2024-04-05 07:38:28.000000 qteasy-1.1.8/qteasy/__init__.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    66919 2024-04-02 02:35:24.000000 qteasy-1.1.8/qteasy/_arg_validators.py
+-rw-r--r--   0 jackie     (501) staff       (20)    52929 2024-04-05 07:43:18.000000 qteasy-1.1.8/qteasy/backtest.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    35193 2024-04-02 14:31:55.000000 qteasy-1.1.8/qteasy/blender.py
+-rw-r--r--   0 jackie     (501) staff       (20)    30242 2024-04-02 14:50:54.000000 qteasy-1.1.8/qteasy/broker.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   142287 2024-04-02 14:31:45.000000 qteasy-1.1.8/qteasy/built_in.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   109762 2024-04-03 15:52:24.000000 qteasy-1.1.8/qteasy/core.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   386464 2024-04-04 15:35:21.000000 qteasy-1.1.8/qteasy/database.py
+-rw-r--r--   0 jackie     (501) staff       (20)     9341 2024-04-02 14:50:54.000000 qteasy-1.1.8/qteasy/emfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    34873 2024-04-05 14:06:04.000000 qteasy-1.1.8/qteasy/evaluate.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    38585 2024-04-05 07:19:15.000000 qteasy-1.1.8/qteasy/finance.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   100797 2024-04-05 12:38:58.000000 qteasy-1.1.8/qteasy/history.py
+-rw-r--r--   0 jackie     (501) staff       (20)    39218 2024-04-02 14:32:16.000000 qteasy-1.1.8/qteasy/optimization.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   107901 2024-04-02 14:31:31.000000 qteasy-1.1.8/qteasy/qt_operator.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    34029 2024-04-05 14:10:37.000000 qteasy-1.1.8/qteasy/space.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    88152 2024-04-02 02:35:24.000000 qteasy-1.1.8/qteasy/strategy.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   151551 2024-04-02 02:35:24.000000 qteasy-1.1.8/qteasy/tafuncs.py
+-rw-r--r--   0 jackie     (501) staff       (20)    47486 2024-04-02 02:35:24.000000 qteasy-1.1.8/qteasy/trade_recording.py
+-rw-r--r--   0 jackie     (501) staff       (20)   180412 2024-04-03 15:51:09.000000 qteasy-1.1.8/qteasy/trader.py
+-rw-r--r--   0 jackie     (501) staff       (20)    68078 2024-04-05 13:49:08.000000 qteasy-1.1.8/qteasy/trading_util.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   140763 2024-04-02 02:35:24.000000 qteasy-1.1.8/qteasy/tsfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    75004 2024-04-03 15:52:24.000000 qteasy-1.1.8/qteasy/utilfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    79732 2024-04-03 15:51:09.000000 qteasy-1.1.8/qteasy/visual.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-05 14:24:31.000000 qteasy-1.1.8/qteasy.egg-info/
+-rw-r--r--   0 jackie     (501) staff       (20)    27759 2024-04-05 14:24:31.000000 qteasy-1.1.8/qteasy.egg-info/PKG-INFO
+-rw-r--r--   0 jackie     (501) staff       (20)     1192 2024-04-05 14:24:31.000000 qteasy-1.1.8/qteasy.egg-info/SOURCES.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        1 2024-04-05 14:24:31.000000 qteasy-1.1.8/qteasy.egg-info/dependency_links.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        1 2023-01-29 16:03:37.000000 qteasy-1.1.8/qteasy.egg-info/not-zip-safe
+-rw-r--r--   0 jackie     (501) staff       (20)      154 2024-04-05 14:24:31.000000 qteasy-1.1.8/qteasy.egg-info/requires.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        7 2024-04-05 14:24:31.000000 qteasy-1.1.8/qteasy.egg-info/top_level.txt
+-rw-r--r--   0 jackie     (501) staff       (20)     1515 2024-04-05 14:24:31.000000 qteasy-1.1.8/setup.cfg
+-rw-r--r--   0 jackie     (501) staff       (20)      257 2024-04-01 14:38:19.000000 qteasy-1.1.8/setup.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-05 14:24:31.000000 qteasy-1.1.8/tests/
+-rw-r--r--   0 jackie     (501) staff       (20)     6524 2024-03-29 13:24:03.000000 qteasy-1.1.8/tests/test_broker.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     8078 2024-04-04 02:50:52.000000 qteasy-1.1.8/tests/test_cashplan.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     3613 2023-11-25 05:35:56.000000 qteasy-1.1.8/tests/test_config.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    17487 2024-04-03 01:57:25.000000 qteasy-1.1.8/tests/test_core_sub_funcs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    19818 2024-04-05 07:21:23.000000 qteasy-1.1.8/tests/test_cost.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   117726 2024-04-04 13:00:13.000000 qteasy-1.1.8/tests/test_datasource.py
+-rw-r--r--   0 jackie     (501) staff       (20)     6143 2024-02-03 15:46:14.000000 qteasy-1.1.8/tests/test_eastmoney.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    73624 2024-04-05 13:44:14.000000 qteasy-1.1.8/tests/test_evaluations.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    13901 2024-02-03 15:46:14.000000 qteasy-1.1.8/tests/test_fast_experiments.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    57759 2024-03-29 10:03:15.000000 qteasy-1.1.8/tests/test_historypanel.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)      413 2023-01-29 16:18:32.000000 qteasy-1.1.8/tests/test_log.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   304019 2024-04-05 12:01:27.000000 qteasy-1.1.8/tests/test_loop.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   169228 2024-04-05 13:35:39.000000 qteasy-1.1.8/tests/test_operator_and_strategy.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    44520 2024-04-03 15:52:24.000000 qteasy-1.1.8/tests/test_qt.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    18581 2023-01-29 16:18:32.000000 qteasy-1.1.8/tests/test_space.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    39724 2024-03-08 14:36:48.000000 qteasy-1.1.8/tests/test_ta_funcs.py
+-rw-r--r--   0 jackie     (501) staff       (20)    43391 2024-04-03 15:51:09.000000 qteasy-1.1.8/tests/test_trader.py
+-rw-r--r--   0 jackie     (501) staff       (20)    44385 2024-04-04 13:00:13.000000 qteasy-1.1.8/tests/test_trader_shell.py
+-rw-r--r--   0 jackie     (501) staff       (20)   159405 2024-04-03 15:51:09.000000 qteasy-1.1.8/tests/test_trading.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    21881 2024-03-30 12:31:29.000000 qteasy-1.1.8/tests/test_tushare.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    43279 2024-04-04 03:20:12.000000 qteasy-1.1.8/tests/test_utilityfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     3090 2023-01-29 16:18:32.000000 qteasy-1.1.8/tests/test_visual.py
```

### Comparing `qteasy-1.1.7/LICENSE` & `qteasy-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.7/PKG-INFO` & `qteasy-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qteasy
-Version: 1.1.7
+Version: 1.1.8
 Summary: A fast quantitative investment tool kit
 Home-page: https://github.com/shepherdpp/qteasy
 Author: Jackie PENG
 Author-email: jackie PENG <jackie.pengzhao@gmail.com>
 Maintainer: Jackie PENG
 Maintainer-email: jackie PENG <jackie.pengzhao@gmail.com>
 License: Copyright <2019> <JACKIE PENG>
@@ -92,15 +92,15 @@
 > 我会尽快修复问题并回复大家的问题。
 
 ## 关于`qteasy`
 
 - 作者: **Jackie PENG**
 - email: *jackie_pengzhao@163.com*
 - Created: 2019, July, 16
-- Latest Version: `1.1.7`
+- Latest Version: `1.1.8`
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
```

### Comparing `qteasy-1.1.7/README.md` & `qteasy-1.1.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 > 我会尽快修复问题并回复大家的问题。
 
 ## 关于`qteasy`
 
 - 作者: **Jackie PENG**
 - email: *jackie_pengzhao@163.com*
 - Created: 2019, July, 16
-- Latest Version: `1.1.7`
+- Latest Version: `1.1.8`
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
```

### Comparing `qteasy-1.1.7/pyproject.toml` & `qteasy-1.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 build-backend = "setuptools.build_meta"
 
 #[tool.setuptools.package.find]
 #where = "qteasy/"
 
 [project]
 name = "qteasy"
-version = "1.1.7"
+version = "1.1.8"
 authors = [
   {name="jackie PENG", email="jackie.pengzhao@gmail.com" },
 ]
 maintainers = [
   {name="jackie PENG", email="jackie.pengzhao@gmail.com" },
 ]
 description = "A fast quantitative investment tool kit"
```

### Comparing `qteasy-1.1.7/qteasy/__init__.py` & `qteasy-1.1.8/qteasy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import tushare as ts
 import numpy as np
 import logging
 from logging.handlers import TimedRotatingFileHandler
 from argparse import Namespace
 
-from .utilfuncs import is_integer_like, is_float_like
+from .utilfuncs import is_float_like, is_integer_like
 from .core import run, set_config, get_configurations, get_config
 from .core import info, is_ready, configure, configuration, save_config, load_config, reset_config
 from .core import get_basic_info, get_stock_info, get_data_overview, refill_data_source
 from .core import get_history_data, filter_stock_codes, filter_stocks
 from .core import reconnect_ds, get_table_info, get_table_overview
 from .history import HistoryPanel
 from .history import dataframe_to_hp, stack_dataframes
@@ -33,23 +33,23 @@
 from .built_in import built_ins, built_in_list, built_in_strategies, get_built_in_strategy
 from .visual import candle
 from .finance import CashPlan, set_cost, update_cost
 from .database import DataSource, find_history_data
 from ._arg_validators import QT_CONFIG, ConfigDict
 
 
-__version__ = '1.1.7'
+__version__ = '1.1.8'
 version_info = Namespace(
         major=1,
         minor=1,
         patch=4,
         short=(1, 1),
-        full=(1, 1, 7),
-        string='1.1.7',
-        tuple=('1', '1', '7'),
+        full=(1, 1, 8),
+        string='1.1.8',
+        tuple=('1', '1', '8'),
         releaselevel='beta',
 )
 
 # 解析qteasy的本地安装路径
 QT_ROOT_PATH = os.path.normpath(os.path.join(os.path.dirname(__file__), os.pardir))
 QT_ROOT_PATH = os.path.join(QT_ROOT_PATH, 'qteasy/')
```

### Comparing `qteasy-1.1.7/qteasy/_arg_validators.py` & `qteasy-1.1.8/qteasy/_arg_validators.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.7/qteasy/backtest.py` & `qteasy-1.1.8/qteasy/backtest.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,33 +12,27 @@
 import os
 import pandas as pd
 import numpy as np
 from numba import njit
 
 import qteasy
 from .history import HistoryPanel
-from .finance import CashPlan, get_selling_result, get_purchase_result
+from .finance import CashPlan, get_selling_result, get_purchase_result, get_cost_pamams
 from .qt_operator import Operator
 
 
 @njit(nogil=False, cache=True)
 def _loop_step(signal_type: int,
                own_cash: float,
                own_amounts: np.ndarray,
                available_cash: float,
                available_amounts: np.ndarray,
                op: np.ndarray,
                prices: np.ndarray,
-               buy_fix: float,
-               sell_fix: float,
-               buy_rate: float,
-               sell_rate: float,
-               buy_min: float,
-               sell_min: float,
-               slipage: float,
+               cost_params: np.ndarray,
                pt_buy_threshold: float,
                pt_sell_threshold: float,
                maximize_cash_usage: bool,
                long_pos_limit: float,
                short_pos_limit: float,
                allow_sell_short: bool,
                moq_buy: float,
@@ -62,26 +56,23 @@
         本次交易开始前账户可用现金余额（交割中的现金不计入余额）
     available_amounts: np.ndarray:
         交易开始前各个股票的可用数量余额（交割中的股票不计入余额）
     op: np.ndarray
         本次交易的个股交易信号清单
     prices: np.ndarray，
         本次交易发生时各个股票的交易价格
-    buy_fix: float
-        交易成本：固定买入费用
-    sell_fix: float
-        交易成本：固定卖出费用
-    buy_rate: float
-        交易成本：固定买入费率
-    sell_rate: float
-        交易成本：固定卖出费率
-    buy_min: float
-        交易成本：最低买入费用
-    sell_min: float
-        交易成本：最低卖出费用
+    cost_params: np.ndarray
+        交易成本参数，包括固定买入费用、固定卖出费用、买入费率、卖出费率、最低买入费用、最低卖出费用
+        buy_fix: float, 交易成本：固定买入费用
+        sell_fix: float, 交易成本：固定卖出费用
+        buy_rate: float, 交易成本：固定买入费率
+        sell_rate: float, 交易成本：固定卖出费率
+        buy_min: float, 交易成本：最低买入费用
+        sell_min: float, 交易成本：最低卖出费用
+        slipage: float, 交易成本：滑点
     pt_buy_threshold: object Cost
         当交易信号类型为PT时，用于计算买入/卖出信号的强度阈值
     pt_sell_threshold: object Cost
         当交易信号类型为PT时，用于计算买入/卖出信号的强度阈值
     maximize_cash_usage: object Cost
         True:   先卖后买模式
         False:  先买后卖模式
@@ -188,21 +179,15 @@
     # 如果不允许卖空交易，则需要更新股票卖出计划数量
     if not allow_sell_short:
         amounts_to_sell = - np.fmin(-amounts_to_sell, available_amounts)
     amount_sold, cash_gained, fee_selling = get_selling_result(
             prices=prices,
             a_to_sell=amounts_to_sell,
             moq=moq_sell,
-            buy_fix=buy_fix,
-            sell_fix=sell_fix,
-            buy_rate=buy_rate,
-            sell_rate=sell_rate,
-            buy_min=buy_min,
-            sell_min=sell_min,
-            slipage=slipage
+            cost_params=cost_params,
     )
 
     if maximize_cash_usage:
         # 仅当现金交割期为0，且希望最大化利用同批交易产生的现金时，才调整现金余额
         # 现金余额 = 期初现金余额 + 本次出售资产获得现金总额
         available_cash += cash_gained.sum()
 
@@ -245,21 +230,15 @@
 
     # 批量提交股份买入计划，计算实际买入的股票份额和交易费用
     # 由于已经提前确认过现金总额，因此不存在买入总金额超过持有现金的情况
     amount_purchased, cash_spent, fee_buying = get_purchase_result(
             prices=prices,
             cash_to_spend=cash_to_spend,
             moq=moq_buy,
-            buy_fix=buy_fix,
-            sell_fix=sell_fix,
-            buy_rate=buy_rate,
-            sell_rate=sell_rate,
-            buy_min=buy_min,
-            sell_min=sell_min,
-            slipage=slipage
+            cost_params=cost_params,
     )
 
     # 4, 计算购入资产产生的交易成本，买入资产和卖出资产的交易成本率可以不同，且每次交易动态计算
     fee = fee_buying + fee_selling
 
     return cash_gained, cash_spent, amount_purchased, amount_sold, fee
 
@@ -460,21 +439,15 @@
         end_idx = op_count
     # 为防止回测价格数据中存在Nan值，需要首先将Nan值替换成0，否则将造成错误值并一直传递到回测历史最后一天
     price = trade_price_list.ffill(0).values
     # 获取每一个资金投入日在历史时间序列中的位置
     investment_date_pos = np.searchsorted(looped_dates, cash_plan.dates)
     invest_dict = cash_plan.to_dict(investment_date_pos)
     # 解析交易费率参数：
-    buy_fix = cost_rate['buy_fix']
-    sell_fix = cost_rate['sell_fix']
-    buy_rate = cost_rate['buy_rate']
-    sell_rate = cost_rate['sell_rate']
-    buy_min = cost_rate['buy_min']
-    sell_min = cost_rate['sell_min']
-    slipage = cost_rate['slipage']
+    cost_params = get_cost_pamams(cost_rate)
     # 确定是否属于PT+lazy的情形
     pt_and_lazy = (signal_type == 0) and (pt_signal_timing == 'lazy')
 
     # 检查信号清单，生成清单回测序号，生成需要跳过的交易信号的列表。这个列表有2维，分别代表每日/每回测价格信号是否可以跳过
     if operator.op_type == 'stepwise':
         # 在stepwise模式下，每一天都需要回，回测所有交易信号行
         skip_op_signal = np.zeros(shape=(op_count, price_type_count), dtype='bool')
@@ -527,21 +500,15 @@
                                                                investment_date_pos,
                                                                invest_amounts,
                                                                price,
                                                                op_list,
                                                                signal_type,
                                                                op_list_bt_indices,
                                                                skip_op_signal,
-                                                               buy_fix,
-                                                               sell_fix,
-                                                               buy_rate,
-                                                               sell_rate,
-                                                               buy_min,
-                                                               sell_min,
-                                                               slipage,
+                                                               cost_params,
                                                                moq_buy,
                                                                moq_sell,
                                                                inflation_rate,
                                                                pt_buy_threshold,
                                                                pt_sell_threshold,
                                                                cash_delivery_period,
                                                                stock_delivery_period,
@@ -636,21 +603,15 @@
                             signal_type=signal_type,
                             own_cash=own_cash,
                             own_amounts=own_amounts,
                             available_cash=available_cash,
                             available_amounts=available_amounts,
                             op=current_op,
                             prices=current_prices,
-                            buy_fix=buy_fix,
-                            sell_fix=sell_fix,
-                            buy_rate=buy_rate,
-                            sell_rate=sell_rate,
-                            buy_min=buy_min,
-                            sell_min=sell_min,
-                            slipage=slipage,
+                            cost_params=cost_params,
                             pt_buy_threshold=pt_buy_threshold,
                             pt_sell_threshold=pt_sell_threshold,
                             maximize_cash_usage=maximize_cash_usage,
                             allow_sell_short=allow_sell_short,
                             long_pos_limit=long_pos_limit,
                             short_pos_limit=short_pos_limit,
                             moq_buy=moq_buy,
@@ -706,31 +667,25 @@
 
     loop_results = (amounts_matrix, cashes, fees, values)
     op_summary_matrix = (op_log_add_invest, op_log_cash, op_log_available_cash, op_log_value)
     return loop_results, op_log_matrix, op_summary_matrix, op_list_bt_indices
 
 
 @njit(nogil=True, cache=True)
-def apply_loop_core(share_count,
-                    looped_dates,
-                    inflation_factors,
-                    investment_date_pos,
-                    invest_amounts,
-                    price,
-                    op_list,
-                    signal_type,
-                    op_list_bt_indices,
-                    skip_op_signal,
-                    buy_fix: float,
-                    sell_fix: float,
-                    buy_rate: float,
-                    sell_rate: float,
-                    buy_min: float,
-                    sell_min: float,
-                    slipage: float,
+def apply_loop_core(share_count: int,
+                    looped_dates: np.ndarray,
+                    inflation_factors: np.ndarray,
+                    investment_date_pos: np.ndarray,
+                    invest_amounts: np.ndarray,
+                    price: np.ndarray,
+                    op_list: np.ndarray,
+                    signal_type: int,
+                    op_list_bt_indices: np.ndarray,
+                    skip_op_signal: np.ndarray,
+                    cost_params: np.ndarray,
                     moq_buy: float,
                     moq_sell: float,
                     inflation_rate: float,
                     pt_buy_threshold: float,
                     pt_sell_threshold: float,
                     cash_delivery_period: int,
                     stock_delivery_period: int,
@@ -739,14 +694,71 @@
                     short_pos_limit: float,
                     max_cash_usage: bool,
                     price_priority_list: list):
     """ apply_loop的核心function,不含任何numba不支持的元素，仅包含batch模式下，
         不需要生成trade_log的情形下运行核心循环的核心代码。
         在符合要求的情况下，这部分代码以njit方式加速运行，实现提速
 
+    TODO: v1.1: 优化代码，去除代码中使用list来进行交割日期计算的部分，使用numpy数组来代替，提高代码效率
+     避免产生numba warnings：
+     NumbaPendingDeprecationWarning:
+     Encountered the use of a type that is scheduled for deprecation: type 'reflected list'
+     found for argument 'looped_dates' of function 'apply_loop_core'.
+     For more information visit
+     https://numba.readthedocs.io/en/stable/reference/deprecation.html#deprecation-of-reflection-for-list-and-set-types
+
+    Parameters
+    ----------
+    share_count: int
+        股票数量
+    looped_dates: np.ndarray
+        回测日期序列
+    inflation_factors: np.ndarray
+        通货膨胀因子序列
+    investment_date_pos: np.ndarray
+        投资日期在回测日期序列中的位置
+    invest_amounts: np.ndarray
+        投资金额序列
+    price: np.ndarray
+        价格序列
+    op_list: np.ndarray
+        交易信号序列
+    signal_type: int
+        交易信号类型
+    op_list_bt_indices: np.ndarray
+        交易信号序列的回测序列
+    skip_op_signal: np.ndarray
+        交易信号跳过序列
+    cost_params: np.ndarray
+        交易费率参数
+    moq_buy: float
+        最小买入量
+    moq_sell: float
+        最小卖出量
+    inflation_rate: float
+        通货膨胀率，用于计算无风险利率
+    pt_buy_threshold: float
+        PT买入阈值
+    pt_sell_threshold: float
+        PT卖出阈值
+    cash_delivery_period: int
+        现金交割周期
+    stock_delivery_period: int
+        股票交割周期
+    allow_sell_short: bool
+        是否允许卖空
+    long_pos_limit: float
+        最大多头仓位
+    short_pos_limit: float
+        最大空头仓位
+    max_cash_usage: bool
+        是否最大化利用现金
+    price_priority_list: list
+        价格优先级列表
+
     Returns
     -------
     """
 
     # 初始化计算结果列表
     own_cash = 0.  # 持有现金总额，期初现金总额总是0，在回测过程中到现金投入日时再加入现金
     available_cash = 0.  # 每期可用现金总额
@@ -799,32 +811,27 @@
             if skip_op_signal[i, j]:
                 cash_gained = np.zeros_like(current_op)
                 cash_spent = np.zeros_like(current_op)
                 amount_purchased = np.zeros_like(current_op)
                 amount_sold = np.zeros_like(current_op)
                 fee = np.zeros_like(current_op)
             else:
+                maximize_cash_usage = max_cash_usage and cash_delivery_period == 0
                 cash_gained, cash_spent, amount_purchased, amount_sold, fee = _loop_step(
                         signal_type=signal_type,
                         own_cash=own_cash,
                         own_amounts=own_amounts,
                         available_cash=available_cash,
                         available_amounts=available_amounts,
                         op=current_op,
                         prices=current_prices,
-                        buy_fix=buy_fix,
-                        sell_fix=sell_fix,
-                        buy_rate=buy_rate,
-                        sell_rate=sell_rate,
-                        buy_min=buy_min,
-                        sell_min=sell_min,
-                        slipage=slipage,
+                        cost_params=cost_params,
                         pt_buy_threshold=pt_buy_threshold,
                         pt_sell_threshold=pt_sell_threshold,
-                        maximize_cash_usage=max_cash_usage and cash_delivery_period == 0,
+                        maximize_cash_usage=maximize_cash_usage,
                         allow_sell_short=allow_sell_short,
                         long_pos_limit=long_pos_limit,
                         short_pos_limit=short_pos_limit,
                         moq_buy=moq_buy,
                         moq_sell=moq_sell
                 )
             # 获得的现金进入交割队列，根据日期的变化确定是新增现金交割还是累加现金交割
```

### Comparing `qteasy-1.1.7/qteasy/blender.py` & `qteasy-1.1.8/qteasy/blender.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.7/qteasy/broker.py` & `qteasy-1.1.8/qteasy/broker.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.7/qteasy/built_in.py` & `qteasy-1.1.8/qteasy/built_in.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.7/qteasy/core.py` & `qteasy-1.1.8/qteasy/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1129,15 +1129,15 @@
         kwargs = QT_CONFIG
     else:
         if isinstance(config_key, str):
             config_key = str_to_list(config_key)
         if not isinstance(config_key, list):
             raise TypeError(f'config_key should be a string or list of strings, got {type(config_key)}')
         assert all(isinstance(item, str) for item in config_key)
-        kwargs = {key: QT_CONFIG[config_key] for key in config_key}
+        kwargs = {key: QT_CONFIG[key] for key in config_key}
         level = [0, 1, 2, 3, 4, 5]
     print(_vkwargs_to_text(kwargs=kwargs, level=level, info=default, verbose=verbose))
 
 
 def get_configurations(config_key=None, level=0, up_to=0, default=True, verbose=False):
     """ 显示qt当前的配置变量，与get_config / configuration 相同
```

### Comparing `qteasy-1.1.7/qteasy/database.py` & `qteasy-1.1.8/qteasy/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -2463,16 +2463,17 @@
         self._table_list = set()
 
         if source_type.lower() in ['db', 'database']:
             # optional packages to be imported
             try:
                 import pymysql
             except ImportError:
-                raise ImportError(f'Missing dependency \'pymysql\' for datasource type '
-                                  f'\'database\'. Use pip or conda to install pymysql: $ pip install pymysql')
+                msg = 'Missing dependency \'pymysql\' for datasource type \'database\'. ' \
+                        'Use pip or conda to install pymysql: $ pip install pymysql'
+                raise ImportError(msg)
             # set up connection to the data base
             if not isinstance(port, int):
                 raise TypeError(f'port should be of type int')
             if user is None:
                 raise ValueError(f'Missing user name for database connection')
             if password is None:
                 raise ValueError(f'Missing password for database connection')
@@ -2498,49 +2499,57 @@
                 self.db_name = db_name
                 self.file_type = None
                 self.file_path = None
                 self.__user__ = user
                 self.__password__ = password
 
             except Exception as e:
-                warnings.warn(f'{str(e)}, Can not set data source type to "db",'
-                              f' will fall back to default type', RuntimeWarning)
+                msg = f'Failed creating database connection, {str(e)}' \
+                      f'Can not set data source type to "db", ' \
+                      f'will fall back to default type'
+
+                warnings.warn(msg, RuntimeWarning)
                 source_type = 'file'
                 file_type = 'csv'
             finally:
                 con.close()
 
         if source_type.lower() == 'file':
             # set up file type and file location
             if not isinstance(file_type, str):
-                raise TypeError(f'file type should be a string, got {type(file_type)} instead!')
+                msg = f'file type should be a string, got {type(file_type)} instead!'
+                raise TypeError(msg)
             file_type = file_type.lower()
             if file_type not in AVAILABLE_DATA_FILE_TYPES:
-                raise KeyError(f'file type not recognized, supported file types are csv / hdf / feather')
+                msg = f'file type not recognized, supported file types are {AVAILABLE_DATA_FILE_TYPES}'
+                raise KeyError(msg)
             if file_type in ['hdf']:
                 try:
                     import tables
                 except ImportError:
-                    raise ImportError(f'Missing optional dependency \'pytables\' for datasource file type '
-                                      f'\'hdf5\'. Use pip or conda to install pytables: $ pip install tables')
+                    msg = f'Missing optional dependency \'pytables\' for datasource file type ' \
+                          f'\'hdf\'. Please install pytables: $ conda install pytables'
+                    raise ImportError(msg)
                 file_type = 'hdf'
             if file_type in ['feather', 'fth']:
                 try:
                     import pyarrow
                 except ImportError:
-                    raise ImportError(f'Missing optional dependency \'pyarrow\' for datasource file type '
-                                      f'\'feather\'. Use pip or conda to install pyarrow: $ pip install pyarrow')
+                    msg = f'Missing optional dependency \'pyarrow\' for datasource file type ' \
+                          f'\'feather\'. Use pip or conda to install pyarrow: $ pip install pyarrow'
+                    raise ImportError(msg)
                 file_type = 'fth'
             from qteasy import QT_ROOT_PATH
             self.file_path = path.join(QT_ROOT_PATH, file_loc)
             try:
                 os.makedirs(self.file_path, exist_ok=True)  # 确保数据dir不存在时创建一个
             except Exception:
-                raise SystemError(f'Failed creating data directory \'{file_loc}\' in qt root path, '
-                                  f'please check your input.')
+                msg = f'Failed creating data directory \'{file_loc}\' in qt root path, ' \
+                        f'please check your input.'
+                raise SystemError(msg)
             self.source_type = 'file'
             self.file_type = file_type
             self.file_loc = file_loc
             self.connection_type = f'file://{file_type}@qt_root/{file_loc}'
             self.host = None
             self.port = None
             self.db_name = None
@@ -2653,19 +2662,20 @@
         -------
         Boolean: 文件存在时返回真，否则返回假
         """
         file_path_name = self.get_file_path_name(file_name)
         return path.exists(file_path_name)
 
     def write_file(self, df, file_name):
-        """ 将df写入本地文件
+        """ 将df写入本地文件，在把文件写入文件之前，需要将primary key写入index，使用
+        set_primary_key_index()函数
 
         Parameters
         ----------
-        df: 待写入文件的DataFrame
+        df: 待写入文件的DataFrame,primary key 为index
         file_name: 本地文件名(不含扩展名)
         Returns
         -------
         str: file_name 如果数据保存成功，返回完整文件路径名称
         """
         file_path_name = self.get_file_path_name(file_name)
         if self.file_type == 'csv':
@@ -2717,15 +2727,18 @@
             return pd.DataFrame()
         if date_like_pk is not None:
             start = pd.to_datetime(start).strftime('%Y-%m-%d')
             end = pd.to_datetime(end).strftime('%Y-%m-%d')
 
         if self.file_type == 'csv':
             # 这里针对csv文件进行了优化，通过分块读取文件，避免当文件过大时导致读取异常
-            df_reader = pd.read_csv(file_path_name, chunksize=chunk_size)  # TODO: add try to escape file reading errors
+            try:
+                df_reader = pd.read_csv(file_path_name, chunksize=chunk_size)
+            except Exception as e:
+                raise RuntimeError(f'{e}, file reading error encountered.')
             df_picker = (chunk for chunk in df_reader)
             if (share_like_pk is not None) and (date_like_pk is not None):
                 df_picker = (chunk.loc[(chunk[share_like_pk].isin(shares)) &
                                        (chunk[date_like_pk] >= start) &
                                        (chunk[date_like_pk] <= end)] for chunk in df_reader)
             elif (share_like_pk is None) and (date_like_pk is not None):
                 df_picker = (chunk.loc[(chunk[date_like_pk] >= start) &
@@ -2735,19 +2748,33 @@
             df = pd.concat(df_picker)
             set_primary_key_index(df, primary_key=primary_key, pk_dtypes=pk_dtypes)
 
             return df
 
         if self.file_type == 'hdf':
             # TODO: hdf5/feather的大文件读取尚未优化
-            df = pd.read_hdf(file_path_name, 'df')  # TODO: add try to escape file reading errors
+            try:
+                df = pd.read_hdf(file_path_name, 'df')
+            except ValueError as e:
+                if 'pickle protocol: 5' in e.__str__():  # check when the file is written in a higher pickle protocol
+                    msg = f'File {file_name} is written in a higher version of python which uses pickle protocol 5, ' \
+                            f'to avoid this error, install pickle5 package and re-save the file.'
+                    raise EnvironmentError(msg)
+                else:
+                    raise RuntimeError(f'{e}, file reading error encountered.')
+            except Exception as e:
+                raise RuntimeError(f'{e}, file reading error encountered.')
+
             df = set_primary_key_frame(df, primary_key=primary_key, pk_dtypes=pk_dtypes)
         elif self.file_type == 'fth':
             # TODO: feather大文件读取尚未优化
-            df = pd.read_feather(file_path_name)  # TODO: add try to escape file reading errors
+            try:
+                df = pd.read_feather(file_path_name)
+            except Exception as e:
+                raise RuntimeError(f'{e}, file reading error encountered.')
         else:  # for some unexpected cases
             raise TypeError(f'Invalid file type: {self.file_type}')
 
         try:
             # 如果self.file_type 为 hdf/fth，那么需要筛选数据
             if (share_like_pk is not None) and (date_like_pk is not None):
                 df = df.loc[(df[share_like_pk].isin(shares)) &
@@ -2762,14 +2789,52 @@
             import traceback
             traceback.print_exc()
             raise RuntimeError(f'{e}')
 
         set_primary_key_index(df, primary_key=primary_key, pk_dtypes=pk_dtypes)
         return df
 
+    def delete_file_records(self, file_name, primary_key, record_ids) -> int:
+        """ 从文件中删除指定的记录
+
+        Parameters
+        ----------
+        file_name: str
+            文件名
+        primary_key: list of str
+            主键
+        record_ids: list of int or tuple of int
+            待删除的记录的主键值
+
+        Returns
+        -------
+        rows_deleted: int
+            删除的记录数
+        """
+        # check that all record_ids are integers
+        if not all(isinstance(record_id, int) for record_id in record_ids):
+            msg = f'All record_ids must be integers, got {record_ids} instead!'
+            raise TypeError(msg)
+        # read all data from file into a dataframe
+        primary_key = [primary_key] if isinstance(primary_key, str) else primary_key
+        df = self.read_file(file_name, primary_key, pk_dtypes=['int'])
+        # check if the record_ids are in the dataframe, remove them if they are
+        rows_deleted = 0
+        for record_id in record_ids:
+            if record_id in df.index:
+                df.drop(record_id, inplace=True)
+                rows_deleted += 1
+
+        # write the updated dataframe back to the file, make sure primary keys are in index
+        df = set_primary_key_frame(df, primary_key=primary_key, pk_dtypes=['int'])
+        set_primary_key_index(df, primary_key=primary_key, pk_dtypes=['int'])
+        self.write_file(df, file_name)
+
+        return rows_deleted
+
     def get_file_table_coverage(self, table, column, primary_key, pk_dtypes, min_max_only):
         """ 检查数据表文件关键列的内容，去重后返回该列的内容清单
 
         Parameters
         ----------
         table: str
             数据表名
@@ -3068,35 +3133,80 @@
         for val in tbl_columns[:-1]:
             sql += "%s, "
         sql += "%s)\n" \
                "ON DUPLICATE KEY UPDATE\n"
         for col in update_cols[:-1]:
             sql += f"`{col}`=VALUES(`{col}`),\n"
         sql += f"`{update_cols[-1]}`=VALUES(`{update_cols[-1]}`)"
+
+        import pymysql
+        con = pymysql.connect(
+                host=self.host,
+                port=self.port,
+                user=self.__user__,
+                password=self.__password__,
+                db=self.db_name,
+        )
         try:
-            import pymysql
-            con = pymysql.connect(
-                    host=self.host,
-                    port=self.port,
-                    user=self.__user__,
-                    password=self.__password__,
-                    db=self.db_name,
-            )
             cursor = con.cursor()
             rows_affected = cursor.executemany(sql, df_tuple)
             con.commit()
             return rows_affected
         except Exception as e:
             con.rollback()
-            raise RuntimeError(f'Error during inserting data to table {db_table} with following sql:\n'
-                               f'Exception:\n{e}\n'
-                               f'SQL:\n{sql} \nwith parameters (first 10 shown):\n{df_tuple[:10]}')
+            msg = f'Error during updating data to table {db_table} with following sql:\n' \
+                    f'Exception:\n{e}\n' \
+                    f'SQL:\n{sql} \nwith parameters (first 10 shown):\n{df_tuple[:10]}'
+            raise RuntimeError(msg)
         finally:
             con.close()
 
+    def delete_database_records(self, db_table, primary_key, record_ids):
+        """ 从数据库表中删除数据
+
+        必须给出数据表的主键名，以及需要删除的记录的主键值
+
+        Parameters
+        ----------
+        db_table: str
+            数据表名
+        primary_key: str
+            数据表的主键名称列表
+        record_ids: list of str or tuple of str
+            需要删除的记录的主键值
+
+        Returns
+        -------
+        int: rows affected
+        """
+
+        # 生成删除记录的SQL语句
+        sql = f"DELETE FROM `{db_table}` WHERE "
+        # 设置删除的条件
+        sql += f"`{primary_key}` IN {tuple(record_ids)}"
+        import pymysql
+        con = pymysql.connect(
+                host=self.host,
+                port=self.port,
+                user=self.__user__,
+                password=self.__password__,
+                db=self.db_name,
+        )
+        try:
+            cursor = con.cursor()
+            rows_affected = cursor.execute(sql)
+            con.commit()
+            return rows_affected
+        except Exception as e:
+            con.rollback()
+            msg = f'Error during deleting data from table {db_table} with following sql:\n' \
+                    f'Exception:\n{e}\n' \
+                    f'SQL:\n{sql}'
+            raise RuntimeError(msg)
+
     def get_db_table_coverage(self, db_table, column):
         """ 检查数据库表关键列的内容，去重后返回该列的内容清单
 
         Parameters
         ----------
         db_table: str
             数据表名
@@ -4234,15 +4344,15 @@
             res_df = res_df.loc[res_df[k] == v]
 
         if record_id is not None:
             return res_df.loc[record_id].to_dict()
         else:
             return res_df if not res_df.empty else None
 
-    def update_sys_table_data(self, table, record_id, **data):
+    def update_sys_table_data(self, table:str, record_id:int, **data) -> int:
         """ 更新系统操作表的数据，根据指定的id更新数据，更新的内容由kwargs给出。
 
         每次只能更新一条数据，数据以dict形式给出
         可以更新一个或多个字段，如果给出的字段不存在，则抛出异，id不可更新。
         id必须存在，否则抛出异常
 
         Parameters
@@ -4298,15 +4408,15 @@
         table_data.update(data)
 
         df_data = pd.DataFrame(table_data, index=[record_id])
         df_data.index.name = p_keys[0]
         self.update_table_data(table, df_data, merge_type='update')
         return record_id
 
-    def insert_sys_table_data(self, table, **data):
+    def insert_sys_table_data(self, table:str, **data) -> int:
         """ 插入系统操作表的数据
 
         一次插入一条记录，数据以dict形式给出
         不需要给出数据的ID，因为ID会自动生成
         如果给出的数据字段不完整，则抛出异常
         如果给出的数据中有不可用的字段，则抛出异常
 
@@ -4390,14 +4500,61 @@
 
         # 插入数据
         self.update_table_data(table, df, merge_type='update')
         # TODO: 这里为什么要用'ignore'而不是'update'? 现在改为'update'，
         #  test_database和test_trading测试都能通过，后续完整测试
         return record_id
 
+    def delete_sys_table_data(self, table, record_ids) -> int:
+        """ 删除系统数据表中的某些记录，被删除的记录的ID使用列表或tuple传入
+
+        parameters
+        ----------
+        table: str
+            需要删除数据的表名
+        record_ids: list of int or tuple of int
+            需要删除的记录的ID列表
+
+        Returns
+        -------
+        int
+            删除的记录数量
+        """
+
+        # 如果不是system table，直接返回0
+        try:
+            ensure_sys_table(table)
+        except KeyError:
+            f'{table} is not valid table, can not delete records from it.'
+            return 0
+        except TypeError:
+            f'{table} is not a system table, can not delete records from it.'
+            return 0
+        except Exception as e:
+            f'An error occurred when checking table {table}: {e}'
+            return 0
+
+        # 检查record_ids是否合法
+        if not isinstance(record_ids, (list, tuple)):
+            raise TypeError(f'record_ids should be a list or tuple, got {type(record_ids)} instead')
+        if not all(isinstance(rid, int) for rid in record_ids):
+            raise TypeError(f'all record_ids should be int, got {[type(rid) for rid in record_ids]} instead')
+
+        columns, dtypes, primary_keys, pk_dtypes = get_built_in_table_schema(table, with_primary_keys=True)
+        primary_key = primary_keys[0]
+
+        if self.source_type == 'db':
+            res = self.delete_database_records(table, primary_key=primary_key, record_ids=record_ids)
+        elif self.source_type == 'file':
+            res = self.delete_file_records(table, primary_key=primary_key, record_ids=record_ids)
+        else:
+            raise RuntimeError(f'invalid source type: {self.source_type}')
+
+        return res
+
     # ==============
     # 顶层函数，包括用于组合HistoryPanel的数据获取接口函数，以及自动或手动下载本地数据的操作函数
     # ==============
     def get_history_data(self, shares=None, symbols=None, htypes=None, freq='d', start=None, end=None, row_count=100,
                          asset_type='any', adj='none'):
         """ 根据给出的参数从不同的本地数据表中获取数据，并打包成一系列的DataFrame，以便组装成
             HistoryPanel对象。
@@ -5082,23 +5239,25 @@
         需要设置为行标签的列的数据类型，日期数据需要小心处理
 
     Returns
     -------
     None
     """
     if not isinstance(df, pd.DataFrame):
-        raise TypeError(f'df should be a pandas DataFrame, got {type(df)} instead')
+        msg = f'df should be a pandas DataFrame, got {type(df)} instead'
+        raise TypeError(msg)
     if df.empty:
         return df
     if not isinstance(primary_key, list):
-        raise TypeError(f'primary key should be a list, got {type(primary_key)} instead')
+        msg = f'primary key should be a list, got {type(primary_key)} instead'
+        raise TypeError(msg)
     all_columns = df.columns
     if not all(item in all_columns for item in primary_key):
-        raise KeyError(f'primary key contains invalid value: '
-                       f'{[item for item in primary_key if item not in all_columns]}')
+        msg = f'primary key contains invalid value: {[item for item in primary_key if item not in all_columns]}'
+        raise KeyError(msg)
 
     # 设置正确的时间日期格式(找到pk_dtype中是否有"date"或"TimeStamp"类型，将相应的列设置为TimeStamp
     set_datetime_format_frame(df, primary_key, pk_dtypes)
 
     # 设置正确的Index或MultiIndex
     pk_count = len(primary_key)
     if pk_count == 1:
@@ -5741,15 +5900,15 @@
     dtype_map = pd.DataFrame(DATA_TABLE_MAP).T
     dtype_map.columns = DATA_TABLE_MAP_COLUMNS
     dtype_map.index.names = DATA_TABLE_MAP_INDEX_NAMES
     return dtype_map
 
 
 @lru_cache(maxsize=1)
-def get_table_map():
+def get_table_map():  # deprecated
     """ 获取所有内置数据表的清单，to be deprecated
 
     Returns
     -------
     pd.DataFrame
     数据表清单
     """
```

### Comparing `qteasy-1.1.7/qteasy/emfuncs.py` & `qteasy-1.1.8/qteasy/emfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.7/qteasy/evaluate.py` & `qteasy-1.1.8/qteasy/evaluate.py`

 * *Files 4% similar despite different names*

```diff
@@ -331,15 +331,20 @@
         final_value = eval_fv(looped_value)
         strategy_return = (final_value / total_invest) ** (1 / total_year) - 1
         reference_return, reference_yearly_return = eval_benchmark(looped_value, reference_value, reference_data)
         b = eval_beta(looped_value, reference_value, reference_data)
         alpha = (strategy_return - risk_free_ror) - b * (reference_yearly_return - risk_free_ror)
         # 当回测期间小于1年时，填充空白alpha值
         looped_value['alpha'] = np.nan
-        looped_value['alpha'].iloc[-1] = alpha
+        # looped_value['alpha'].iloc[-1] = alpha  # Chained assignment is not allowed soon
+        looped_value.at[looped_value.index[-1], 'alpha'] = alpha # use .at to avoid chained assignment
+        # following usage also works
+        # looped_value.loc[looped_value.index[-1], 'alpha'] = alpha
+        # or
+        # looped_value.iat[-1, looped_value.columns.get_loc('alpha')] = alpha
     else:  # loop_len > 250
         # 计算年化收益，如果回测期间大于一年，直接计算滚动年收益率（250天）
         year_ret = looped_value.value / looped_value['value'].shift(250) - 1
         bench = reference_value[reference_data]
         bench_ret = (bench / bench.shift(250)) - 1
         looped_value['alpha'] = (year_ret - risk_free_ror) - looped_value['beta'] * (bench_ret - risk_free_ror)
         alpha = looped_value['alpha'].mean()
@@ -384,15 +389,16 @@
         ret_dev = looped_value['pct_change'].rolling(250).var()
         looped_value['beta'] = looped_value['pct_change'].rolling(250).cov(ref_ret) / ret_dev
         return looped_value['beta'].mean()
     else:
         ret_dev = looped_value['pct_change'].var()
         beta = looped_value['pct_change'].cov(ref_ret) / ret_dev
         looped_value['beta'] = np.nan
-        looped_value['beta'].iloc[-1] = beta
+        # looped_value['beta'].iloc[-1] = beta  # Chained assignment is not allowed soon
+        looped_value.at[looped_value.index[-1], 'beta'] = beta  # use .at to avoid chained assignment
         return beta
 
 
 def eval_sharp(looped_value, riskfree_interest_rate: float = 0.0035):
     """ 夏普比率。表示每承受一单位总风险，会产生多少的超额报酬。
 
     具体计算方法为 (策略年化收益率 - 回测起始交易日的无风险利率) / 策略收益波动率 。
@@ -409,15 +415,16 @@
     # 计算年化收益，如果回测期间大于一年，直接计算滚动年收益率（250天）
     ret = looped_value['value'] / looped_value['value'].shift(1) - 1
     volatility = eval_volatility(looped_value, logarithm=False)
     if loop_len <= 250:
         yearly_return = ret.mean() * 250
         sharp = (yearly_return - riskfree_interest_rate) / volatility
         looped_value['sharp'] = np.nan
-        looped_value['sharp'].iloc[-1] = sharp
+        # looped_value['sharp'].iloc[-1] = sharp  # Chained assignment is not allowed soon
+        looped_value.at[looped_value.index[-1], 'sharp'] = sharp  # use .at to avoid chained assignment
         return sharp
     else:  # loop_len > 250
         roll_yearly_return = ret.rolling(250).mean() * 250
         looped_value['sharp'] = (roll_yearly_return - riskfree_interest_rate) / looped_value['volatility']
         return looped_value['sharp'].mean()
 
 
@@ -446,15 +453,16 @@
     if len(ret) > 250:
         volatility = ret.rolling(250).std() * np.sqrt(250)
         looped_value['volatility'] = volatility
         return volatility.mean()
     else:
         volatility = ret.std() * np.sqrt(250)
         looped_value['volatility'] = np.nan
-        looped_value['volatility'].iloc[-1] = volatility
+        # looped_value['volatility'].iloc[-1] = volatility  # Chained assignment is not allowed soon
+        looped_value.at[looped_value.index[-1], 'volatility'] = volatility  # use .at to avoid chained assignment
         return volatility
 
 
 def eval_info_ratio(looped_value, reference_value, reference_data):
     """ 信息比率。衡量超额风险带来的超额收益。具体计算方法为 (策略每日收益 - 参考标准每日收益)的年化均值 / 年化标准差 。
         information ratio = (portfolio return - reference return) / tracking error
 
@@ -494,15 +502,16 @@
         ret = value / value.shift(250) - 1
         looped_value['calmar'] = ret / drawdown.rolling(250).max()
         return looped_value['calmar'].mean()
     else:  # len(looped_value <= 250
         ret = value[-1] / value[0] - 1
         calmar = ret / drawdown.max()
         looped_value['calmar'] = np.nan
-        looped_value['calmar'].iloc[-1] = calmar
+        # looped_value['calmar'].iloc[-1] = calmar  # Chained assignment is not allowed soon
+        looped_value.at[looped_value.index[-1], 'calmar'] = calmar  # use .at to avoid chained assignment
         return calmar
 
 
 def eval_max_drawdown(looped_value):
     """ 最大回撤。描述策略可能出现的最糟糕的情况。具体计算方法为 max(1 - 策略当日价值 / 当日之前虚拟账户最高价值)
         除了计算最大回撤以外，同时还找到最大的五个回撤区间，分别找到他们的峰值日期、谷值日期、回撤率、回复日期
         并将上述信息放入一个DataFrame中与最大回撤相关数据一起返回
@@ -579,15 +588,15 @@
     if not isinstance(looped_val, pd.DataFrame):
         raise TypeError(f'looped value should be pandas DataFrame, got {type(looped_val)} instead')
     if looped_val.empty:
         return -np.inf
     if 'value' not in looped_val:
         raise KeyError(f'the key \'value\' can not be found in given looped value!')
 
-    perf = looped_val['value'].iloc[-1]
+    perf = looped_val.at[looped_val.index[-1], 'value']
     return perf
 
 
 def eval_return(looped_val, cash_plan):
     """ 评价函数 Return Rate 收益率评价，在looped_value中补充完整的收益率和年化收益率数据
         在looped_val中添加以下数据：
         - invest:       每个交易日累计投入资金总额
@@ -630,20 +639,21 @@
     looped_val['annual_rtn'] = (looped_val.rtn + 1) ** (1 / ys) - 1
     looped_val['pct_change'] = looped_val.value / looped_val.value.shift(1) - 1
     skewness = looped_val['pct_change'].skew()
     kurtosis = looped_val['pct_change'].kurtosis()
 
     first_year = looped_val.index[0].year
     last_year = looped_val.index[-1].year
+    month_freq_code = 'ME' if pd.__version__ > '2.0' else 'M'  # freq='ME' if pandas_version > 2.0
     starts = pd.date_range(start=str(first_year - 1) + '1231',
                            end=str(last_year) + '1130',
-                           freq='M') + pd.Timedelta(1, 'd')
+                           freq=month_freq_code) + pd.Timedelta(1, 'd')
     ends = pd.date_range(start=str(first_year) + '0101',
                          end=str(last_year) + '1231',
-                         freq='M')
+                         freq=month_freq_code)
     # 计算每个月的收益率
     monthly_returns = list()
     for start, end in zip(starts, ends):
         val = looped_val['value'].loc[start:end]
         if len(val) > 0:
             monthly_returns.append(val.iloc[-1] / val.iloc[0] - 1)
         else:
@@ -652,20 +662,21 @@
     monthly_returns = np.array(monthly_returns).reshape(year_count, 12)
     monthly_return_df = pd.DataFrame(monthly_returns,
                                      columns=['Jan', 'Feb', 'Mar', 'Apr',
                                               'May', 'Jun', 'Jul', 'Aug',
                                               'Sep', 'Oct', 'Nov', 'Dec'],
                                      index=range(first_year, last_year + 1))
     # 计算每年的收益率
+    year_freq_code = 'YE' if pd.__version__ > '2.0' else 'Y'  # freq='YE' if pandas_version > 2.0
     starts = pd.date_range(start=str(first_year - 1) + '1231',
                            end=str(last_year) + '1130',
-                           freq='Y') + pd.Timedelta(1, 'd')
+                           freq=year_freq_code) + pd.Timedelta(1, 'd')
     ends = pd.date_range(start=str(first_year) + '0101',
                          end=str(last_year) + '1231',
-                         freq='Y')
+                         freq=year_freq_code)
     # 组装出月度、年度收益率矩阵
     yearly_returns = list()
     for start, end in zip(starts, ends):
         val = looped_val['value'].loc[start:end]
         if len(val) > 0:
             yearly_returns.append(val.iloc[-1] / val.iloc[0] - 1)
         else:
```

### Comparing `qteasy-1.1.7/qteasy/finance.py` & `qteasy-1.1.8/qteasy/finance.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,42 @@
 import numpy as np
 import pandas as pd
 from numba import njit
 
 from .utilfuncs import ALL_COST_PARAMETERS
 
 
+def validate_cost_dict(cost: dict) -> None:
+    """ 检查成本参数是否合法
+
+    Parameters
+    ----------
+    cost: dict
+        一个包含成本参数的字典
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    TypeError
+        如果cost不是一个字典
+    KeyError
+        如果cost中包含非法的成本参数
+    """
+    if not isinstance(cost, dict):
+        msg = f'Cost should be a dict, got {type(cost)} instead'
+        raise TypeError(msg)
+    if any(k not in ALL_COST_PARAMETERS for k in cost.keys()):
+        invalid_keys = [k for k in cost.keys() if k not in ALL_COST_PARAMETERS]
+        raise KeyError(f'Invalid cost parameters: {invalid_keys}')
+    return None
+
+
 def set_cost(**kwargs):
     """ 新建一个cost字典
 
     交易成本的估算依赖四种类型的成本：
     1,  fixed_fee：固定费用，在交易过程中产生的固定现金费用，与交易金额和交易量无关，买入与卖出固定费用可以不同
         固定费用类型与固定费率或最低费用不能同时存在，当固定费用不为0时，直接使用固定费用作为交易费用，忽略其他参数
         交易费用 = 固定费用
@@ -58,235 +86,240 @@
                 sell_min=0.0,
                 slipage=0.0)
 
     update_cost(cost, **kwargs)
     return cost
 
 
-def update_cost(c, **kwargs):
+def update_cost(c: dict, **kwargs):
     """ 更新cost字典中各个值
 
     Parameters
     ----------
+    c: dict
+        一个包含成本参数的字典
     kwargs: dict
         可用的成本参数包括：
         - buy_fix: float, 固定买入费用，如果设置了固定费用，则费率和最低费用会被忽略
         - sell_fix: float, 固定卖出费用，如果设置了固定费用，则费率和最低费用会被忽略
         - buy_rate: float, 买入费率，实际买入费用等于买入金额乘以费率
         - sell_rate: float, 卖出费率，实际卖出费用等于卖出金额乘以费率
         - buy_min: float, 最低买入费用，当按费率计算的费用小于该费用时，按最低费用计算
         - sell_min: float, 最低卖出费用，当按费率计算的费用小于该费用时，按最低费用计算
         - slipage: float, 滑点，用于估算交易价格损失，金额为滑点乘以交易金额
 
     Returns
     -------
     c: dict, 更新后的成本参数
     """
-    if not isinstance(c, dict):
-        raise TypeError(f'cost should be a dict, got {type(c)} instead')
-    if any(k not in ALL_COST_PARAMETERS for k in c.keys()):
-        invalid_keys = [k for k in c.keys() if k not in ALL_COST_PARAMETERS]
-        raise KeyError(f'invalid keys ({invalid_keys}) found in cost dict!')
+    validate_cost_dict(c)
     for k, v in kwargs.items():
         if k not in ALL_COST_PARAMETERS:
             continue
         # TODO: 此处应该validate输入值
         c[k] = v
 
     return c
 
 
+def get_cost_pamams(c: dict) -> np.ndarray:
+    """ 返回成本参数
+
+    Parameters
+    ----------
+    c: dict
+        一个包含成本参数的字典
+
+    Returns
+    -------
+    np.ndarray
+        一个包含成本参数的ndarray，包括以下参数：
+        fee_params[0]: buy_fix: float:
+            买入固定费用
+        fee_params[1]: sell_fix: float:
+            卖出固定费用
+        fee_params[2]: buy_rate: float:
+            买入费率
+        fee_params[3]: sell_rate: float:
+            卖出费率
+        fee_params[4]: buy_min: float:
+            买入最低费用
+        fee_params[5]: sell_min: float:
+            卖出最低费用
+        fee_params[6]: slipage: float:
+            滑点
+    """
+    validate_cost_dict(c)
+    return np.array([c['buy_fix'],
+                     c['sell_fix'],
+                     c['buy_rate'],
+                     c['sell_rate'],
+                     c['buy_min'],
+                     c['sell_min'],
+                     c['slipage']])
+
+
 @njit
-def calculate_fees(trade_values: np.ndarray,
-                   is_buying,
-                   fixed_fees,
-                   buy_fix,
-                   sell_fix,
-                   buy_rate,
-                   sell_rate,
-                   buy_min,
-                   sell_min,
-                   slipage) -> float:
+def calculate_fees(trade_values: np.ndarray, cost_params: np.ndarray, is_buying: bool = True,
+                   fixed_fees: bool = False) -> np.ndarray:
     """直接调用对象，计算交易费率或交易费用
 
     采用两种模式计算：
         当fixed_fees为True时，采用固定费用模式计算，返回值为包含滑点的交易成本列表，
         当fixed_fees为False时，采用固定费率模式计算，返回值为包含滑点的交易成本率列表
 
     Parameters
     ----------
     trade_values: ndarray:
-        总交易金额清单
-    is_buying: bool:
+        总交易金额清单，每一种股票的交易金额
+    cost_params: np.ndarray:
+        交易费用参数，一个ndarray，包括以下参数：
+        fee_params[0]: buy_fix: float:
+            买入固定费用
+        fee_params[1]: sell_fix: float:
+            卖出固定费用
+        fee_params[2]: buy_rate: float:
+            买入费率
+        fee_params[3]: sell_rate: float:
+            卖出费率
+        fee_params[4]: buy_min: float:
+            买入最低费用
+        fee_params[5]: sell_min: float:
+            卖出最低费用
+        fee_params[6]: slipage: float:
+            滑点
+    is_buying: bool, optional, default: True:
         当前是否计算买入费用或费率, 默认True
-    fixed_fees: bool:
+    fixed_fees: bool, optional, default: False:
         当前是否采用固定费用模式计算, 默认False
-    buy_fix: float:
-        买入固定费用
-    sell_fix: float:
-        卖出固定费用
-    buy_rate: float:
-        买入费率
-    sell_rate: float:
-        卖出费率
-    buy_min: float:
-        买入最低费用
-    sell_min: float:
-        卖出最低费用
-    slipage: float:
-        滑点
 
     Returns
     -------
     np.ndarray:
+        一个ndarray，每种股票的交易费用
     """
     if is_buying is None:
         is_buying = True
     if fixed_fees is None:
         fixed_fees = False
 
     # TODO: 重写slipage的计算公式，使得slipage是一个交易费用的乘数，该乘数 = slipage * (qty / 100) ** 2
     if fixed_fees:  # 采用固定费用模式计算, 返回固定费用及滑点成本，返回的是费用而不是费率
         if is_buying:
-            return buy_fix + slipage * trade_values ** 2
+            # buy_fix + slipage * trade_values ** 2
+            return cost_params[0] + cost_params[6] * trade_values ** 2
         else:
-            return sell_fix + slipage * trade_values ** 2
-    else:  # 采用固定费率模式计算
+            # sell_fix + slipage * trade_values ** 2
+            return cost_params[1] + cost_params[6] * trade_values ** 2
+    else:  # 采用固定费率模式计算, 返回费率而不是费用
         if is_buying:
-            if buy_min == 0.:
-                return buy_rate + slipage * trade_values
+            if cost_params[4] == 0.:  # if buy_min == 0
+                # return buy_rate + slipage * trade_values
+                return cost_params[2] + cost_params[6] * trade_values
             else:
-                min_rate = buy_min / (trade_values - buy_min)
-                return np.fmax(buy_rate, min_rate) + slipage * trade_values
+                # min_rate = buy_min / (trade_values - buy_min)
+                min_rate = cost_params[4] / (trade_values - cost_params[4])
+                # return max(buy_rate, min_rate) + slipage * trade_values
+                return np.fmax(cost_params[2], min_rate) + cost_params[6] * trade_values
         else:
-            if sell_min == 0.:
-                return sell_rate - slipage * trade_values
+            if cost_params[5] == 0.:  # if sell_min == 0
+                # return sell_rate - slipage * trade_values
+                return cost_params[3] - cost_params[6] * trade_values
             else:
-                min_rate = -sell_min / trade_values
+                # min_rate = - sell_min / trade_values
+                min_rate = - cost_params[5] / trade_values
                 # 当trade_values中有0值时，将产生inf，且传递到caller后会导致问题，因此需要清零
                 min_rate[np.isinf(min_rate)] = 0
-                return np.fmax(sell_rate, min_rate) + slipage * trade_values
+                # return max(sell_rate, min_rate) - slipage * trade_values
+                return np.fmax(cost_params[3], min_rate) + cost_params[6] * trade_values
 
 
 @njit
 def get_selling_result(prices: np.ndarray,
                        a_to_sell: np.ndarray,
                        moq,
-                       buy_fix,
-                       sell_fix,
-                       buy_rate,
-                       sell_rate,
-                       buy_min,
-                       sell_min,
-                       slipage):
+                       cost_params: np.ndarray,
+                       ) -> (np.ndarray, np.ndarray, np.ndarray):
     """计算出售投资产品的要素
 
     Parameters
     ----------
     prices: ndarray, 投资产品的价格
     a_to_sell: ndarray, 计划卖出数量，其形式为计划卖出的股票的数量，通常为负，且其绝对值通常小于等于可出售的数量
     moq: float, 卖出股票的最小交易单位
-    buy_fix: float, 买入固定费用
-    sell_fix: float, 卖出固定费用
-    buy_rate: float, 买入费率
-    sell_rate: float, 卖出费率
-    buy_min: float, 买入最低费用
-    sell_min: float, 卖出最低费用
-    slipage: float, 滑点
+    cost_params: np.ndarray, 交易费用参数，包括以下参数：
+        - buy_fix: float, 买入固定费用
+        - sell_fix: float, 卖出固定费用
+        - buy_rate: float, 买入费率
+        - sell_rate: float, 卖出费率
+        - buy_min: float, 买入最低费用
+        - sell_min: float, 卖出最低费用
+        - slipage: float, 滑点
 
     Returns
     -------
     tuple: (a_sold, cash_gained, fee)
      - a_sold: ndarray          实际出售的资产份额
      - cash_gained: ndarray     扣除手续费后获得的现金
      - fee: ndarray             扣除的手续费
     """
     if moq == 0:
         a_sold = a_to_sell
     else:
         a_sold = np.trunc(a_to_sell / moq) * moq
     sold_values = a_sold * prices
+    sell_fix = cost_params[1]
     if sell_fix == 0:  # 固定交易费用为0，按照交易费率模式计算
-        rates = calculate_fees(trade_values=sold_values,
-                               is_buying=False,
-                               fixed_fees=False,
-                               buy_fix=buy_fix,
-                               sell_fix=sell_fix,
-                               buy_rate=buy_rate,
-                               sell_rate=sell_rate,
-                               buy_min=buy_min,
-                               sell_min=sell_min,
-                               slipage=slipage)
+        rates = calculate_fees(trade_values=sold_values, cost_params=cost_params, is_buying=False, fixed_fees=False)
         cash_gained = (-1 * sold_values * (1 - rates))
         fees = -(sold_values * rates)
     else:  # 固定交易费用不为0时，按照固定费率收取费用——直接从交易获得的现金中扣除
-        fixed_fees = calculate_fees(trade_values=sold_values,
-                                    is_buying=False,
-                                    fixed_fees=True,
-                                    buy_fix=buy_fix,
-                                    sell_fix=sell_fix,
-                                    buy_rate=buy_rate,
-                                    sell_rate=sell_rate,
-                                    buy_min=buy_min,
-                                    sell_min=sell_min,
-                                    slipage=slipage)
+        fixed_fees = calculate_fees(trade_values=sold_values, cost_params=cost_params, is_buying=False, fixed_fees=True)
         fees = np.where(a_sold, fixed_fees, 0)
         cash_gained = - sold_values - fees
     return a_sold, cash_gained, fees
 
 
 @njit
 def get_purchase_result(prices: np.ndarray,
                         cash_to_spend: np.ndarray,
                         moq,
-                        buy_fix,
-                        sell_fix,
-                        buy_rate,
-                        sell_rate,
-                        buy_min,
-                        sell_min,
-                        slipage):
+                        cost_params: np.ndarray,
+                        ) -> (np.ndarray, np.ndarray, np.ndarray):
     """获得购买资产时的要素
 
     Parameters
     ----------
     prices: ndarray, 投资组合中每只股票的当前单价
     cash_to_spend: ndarray, 买入金额，可用于买入股票或资产的计划金额
     moq: float, 最小交易单位
-    buy_fix: float, 买入固定费用
-    sell_fix: float, 卖出固定费用
-    buy_rate: float, 买入费率
-    sell_rate: float, 卖出费率
-    buy_min: float, 买入最低费用
-    sell_min: float, 卖出最低费用
-    slipage: float, 滑点
+    cost_params: np.ndarray, 交易费用参数，包括以下参数：
+        - buy_fix: float, 买入固定费用
+        - sell_fix: float, 卖出固定费用
+        - buy_rate: float, 买入费率
+        - sell_rate: float, 卖出费率
+        - buy_min: float, 买入最低费用
+        - sell_min: float, 卖出最低费用
+        - slipage: float, 滑点
 
     Returns
     -------
     tuple: (a_to_purchase, cash_spent, fee)
     a_to_purchase: ndarray,  代表所有股票分别买入的份额或数量
     cash_spent: ndarray,     花费的总金额，包括购买成本在内
     fee: ndarray,            花费的费用，购买成本，包括佣金和滑点等投资成本
     """
-    # buy_min = buy_min
-    # buy_fix = buy_fix
+
+    buy_fix = cost_params[0]
+    buy_min = cost_params[4]
     if buy_fix == 0.:
         # 固定费用为0，估算购买一定金额股票的交易费率，考虑最小费用，将绝对值小于buy_min的金额置0
         # （因为在"allow_sell_short"模式下，cash_to_spend可能会小于零，代表买入负持仓）
         cash_to_spend = np.where(np.abs(cash_to_spend) < buy_min, 0, cash_to_spend)
-        rates = calculate_fees(trade_values=cash_to_spend,
-                               is_buying=True,
-                               fixed_fees=False,
-                               buy_fix=buy_fix,
-                               sell_fix=sell_fix,
-                               buy_rate=buy_rate,
-                               sell_rate=sell_rate,
-                               buy_min=buy_min,
-                               sell_min=sell_min,
-                               slipage=slipage)
+        rates = calculate_fees(trade_values=cash_to_spend, cost_params=cost_params, is_buying=True, fixed_fees=False)
         # 根据moq计算实际购买份额，当价格为0的时候买入份额为0
         if moq == 0:  # moq为0，实际买入份额与期望买入份额相同
             a_purchased = np.where(prices,
                                    cash_to_spend / (prices * (1 + rates)),
                                    0.)
         else:  # moq不为零，实际买入份额必须是moq的倍数，因此实际买入份额通常小于期望买入份额
             a_purchased = np.where(prices,
@@ -296,24 +329,15 @@
         fees = np.where(a_purchased, np.fmax(a_purchased * prices * rates, buy_min), 0.)
         purchased_values = a_purchased * prices + fees
         cash_spent = np.where(a_purchased, -1 * purchased_values, 0.)
     else:  # self.buy_fix
         # 固定费用不为0，按照固定费用模式计算费用，忽略费率并且忽略最小费用，将绝对值小于buy_fix的金额置0
         # （因为在"allow_sell_short"模式下，cash_to_spend可能会小于零，代表买入负持仓）
         cash_to_spend = np.where(np.abs(cash_to_spend) < buy_fix, 0, cash_to_spend)
-        fixed_fees = calculate_fees(trade_values=cash_to_spend,
-                                    is_buying=True,
-                                    fixed_fees=True,
-                                    buy_fix=buy_fix,
-                                    sell_fix=sell_fix,
-                                    buy_rate=buy_rate,
-                                    sell_rate=sell_rate,
-                                    buy_min=buy_min,
-                                    sell_min=sell_min,
-                                    slipage=slipage)
+        fixed_fees = calculate_fees(trade_values=cash_to_spend, cost_params=cost_params, is_buying=True, fixed_fees=True)
         if moq == 0.:
             a_purchased = np.fmax(np.where(prices,
                                            (cash_to_spend - fixed_fees) / prices,
                                            0.),
                                   0.)
         else:
             a_purchased = np.fmax(np.where(prices,
@@ -421,14 +445,15 @@
 
         if isinstance(amounts, (int, float)):
             amounts = [amounts]
         if not isinstance(amounts, (list, np.ndarray)):
             msg = f'Amounts should be a list of numbers, got {type(amounts)} instead'
             raise TypeError(msg)
         if isinstance(amounts, list):
+
             if not all([isinstance(amount, (int, float, np.int64, np.float64)) for amount in amounts]):
                 msg = f'Amount should be number format, got unresolved format in amounts!'
                 raise TypeError(msg)
             if not all([amount > 0 for amount in amounts]):
                 msg = f'Investment amount should be larger than 0'
                 raise ValueError(msg)
```

### Comparing `qteasy-1.1.7/qteasy/history.py` & `qteasy-1.1.8/qteasy/history.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,21 +97,21 @@
         可能导致报错。
 
         Parameters
         ----------
         values: ndarray
             一个ndarray，该数组的维度不能超过三维，如果给出的数组维度不够三维，将根据给出的标签推断并补齐维度
             如果不给出values，则会返回一个空HistoryPanel，其empty属性为True
-        levels: Iterables
+        levels: list or tuple
             HistoryPanel的股票标签，层的数量为values第一个维度的数据量，每一层代表一种股票或资产
-        rows: Iterables
+        rows: list or tuple
             HistoryPanel的时间日期标签。
             datetime range或者timestamp index或者str类型，通常是时间类型或可以转化为时间类型，
             行标签代表每一条数据对应的历史时间戳
-        columns: Iterables
+        columns: list or tuple
             HistoryPanel的列标签，代表历史数据的类型，既可以是历史数据的
         """
 
         # TODO: 在生成HistoryPanel时如果只给出data或者只给出data+columns，生成HistoryPanel打印时会报错，问题出在to_dataFrame()上
         #  在生成HistoryPanel时传入的ndarray会被直接用于HistoryPanel，如果事后修改这个ndarray，HistoryPanel也会改变
         #  应该考虑是否在创建HistoryPanel时生成ndarray的一个copy而不是使用其自身 。
         if (not isinstance(values, np.ndarray)) and (values is not None):
@@ -1680,24 +1680,29 @@
                     open
     2020-01-01  0.259304
     2020-01-02  0.600886
     2020-01-03  0.953640
     """
 
     available_column_types = ['shares', 'htypes', None]
-    from collections import Iterable
-    assert isinstance(df, pd.DataFrame), f'Input df should be pandas DataFrame! got {type(df)} instead.'
+    if not isinstance(df, pd.DataFrame):
+        msg = f'Input df should be pandas DataFrame! got {type(df)} instead.'
+        raise TypeError(msg)
     if hdates is None:
         hdates = df.rename(index=pd.to_datetime).index
-    assert isinstance(hdates, Iterable), f'TypeError, hdates should be iterable, got {type(hdates)} instead.'
+    # if not isinstance(hdates, (list, tuple)):
+    #     msg = f'TypeError, hdates should be list or tuple, got {type(hdates)} instead.'
+    #     raise TypeError(msg)
     index_count = len(hdates)
-    assert index_count == len(df.index), \
-        f'InputError, can not match {index_count} indices with {len(df.hdates)} rows of DataFrame'
-    assert column_type in available_column_types, f'column_type should be either "shares" or "htypes", ' \
-                                                  f'got {type(column_type)} instead!'
+    if not index_count == len(df.index):
+        msg = f'InputError, can not match {index_count} indices with {len(df.hdates)} rows of DataFrame'
+        raise ValueError(msg)
+    if not column_type in available_column_types:
+        msg = f'column_type should be either "shares" or "htypes", got {type(column_type)} instead!'
+        raise ValueError(msg)
     # TODO: Temp codes, implement this method when column_type is not given -- the column type should be infered
     #  by the input combination of shares and htypes
     if column_type is None:  # try to infer a proper column type
         if shares is None:
             htype_list = []
             if htypes is None:
                 raise KeyError(f'shares and htypes can not both be None if column_type is not given!')
@@ -1719,26 +1724,23 @@
             try:
                 if len(share_list) == 1:
                     column_type = 'htypes'
                 else:
                     column_type = 'shares'
             except:
                 raise ValueError(f'shares should be a list or a string, got {type(shares)} instead')
-        # print(f'got None in function for column_type, column type is set to {column_type}')
+
     if column_type == 'shares':
         if shares is None:
             shares = df.columns
-        elif isinstance(shares, str):
+        if isinstance(shares, str):
             shares = str_to_list(shares, sep_char=',')
-            assert len(shares) == len(df.columns), \
-                f'InputError, can not match {len(shares)} shares with {len(df.columns)} columns of DataFrame'
-        else:
-            assert isinstance(shares, Iterable), f'TypeError: levels should be iterable, got {type(shares)} instead.'
-            assert len(shares) == len(df.columns), \
-                f'InputError, can not match {len(shares)} shares with {len(df.columns)} columns of DataFrame'
+        if not len(shares) == len(df.columns):
+            msg = f'Can not match {len(shares)} shares with {len(df.columns)} columns of DataFrame'
+            raise ValueError(msg)
         if htypes is None:
             raise KeyError(f', Please provide a valid name for the htype of the History Panel')
         assert isinstance(htypes, str), \
             f'TypeError, data type of dtype should be a string, got {type(htypes)} instead.'
         share_count = len(shares)
         history_panel_value = np.zeros(shape=(share_count, len(hdates), 1))
         for i in range(share_count):
@@ -1747,15 +1749,16 @@
         if htypes is None:
             htypes = df.columns
         elif isinstance(htypes, str):
             htypes = htypes.split(',')
             assert len(htypes) == len(df.columns), \
                 f'InputError, can not match {len(htypes)} shares with {len(df.columns)} columns of DataFrame'
         else:
-            assert isinstance(htypes, Iterable), f'TypeError: levels should be iterable, got {type(htypes)} instead.'
+            assert isinstance(htypes, (list, tuple)), f'TypeError: levels should be list or tuple, ' \
+                                                      f'got {type(htypes)} instead.'
             assert len(htypes) == len(df.columns), \
                 f'InputError, can not match {len(htypes)} shares with {len(df.columns)} columns of DataFrame'
         assert shares is not None, f'InputError, shares should be given when they can not inferred'
         assert isinstance(shares, str), \
             f'TypeError, data type of share should be a string, got {type(shares)} instead.'
         history_panel_value = df.values.reshape(1, len(hdates), len(htypes))
     return HistoryPanel(values=history_panel_value, levels=shares, rows=hdates, columns=htypes)
```

### Comparing `qteasy-1.1.7/qteasy/optimization.py` & `qteasy-1.1.8/qteasy/optimization.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.7/qteasy/qt_operator.py` & `qteasy-1.1.8/qteasy/qt_operator.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.7/qteasy/space.py` & `qteasy-1.1.8/qteasy/space.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,20 +186,22 @@
         s = [ax.size for ax in self._axis]
         return tuple(s)
 
     @property
     def volume(self):
         """输出空间的尺度，输出每个维度的跨度之乘积"""
         s = [ax.size for ax in self._axis]
-        return np.product(s)
+        # return np.product(s)  # np.product() will be deprecated in the future
+        return np.prod(s)
 
     @property
     def count(self):
         s = [ax.count for ax in self._axis]
-        return np.product(s)
+        # return np.product(s)  # np.product() will be deprecated in the future
+        return np.prod(s)
 
     def __repr__(self):
         output = []
         for item in self.boes:
             if len(item) <= 3:
                 output.append(str(item))
             else:
```

### Comparing `qteasy-1.1.7/qteasy/strategy.py` & `qteasy-1.1.8/qteasy/strategy.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.7/qteasy/tafuncs.py` & `qteasy-1.1.8/qteasy/tafuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.7/qteasy/trade_recording.py` & `qteasy-1.1.8/qteasy/trade_recording.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.7/qteasy/trader.py` & `qteasy-1.1.8/qteasy/trader.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.7/qteasy/trading_util.py` & `qteasy-1.1.8/qteasy/trading_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1353,15 +1353,19 @@
             raise RuntimeError(f'Wrong market type is given, {e}')
         trade_cal = calendar.reindex(index=time_index)
         # 如果time_index不是从某天的00:00:00开始，则trade_cal中的第一个值会为nan
         # 此时需要用检查trade_cal的日期，填充正确的交易日标记
         if pd.isna(trade_cal.iloc[0]):
             date = pd.to_datetime(time_index[0].date())
             trade_cal.iloc[0] = calendar.loc[date]
-        trade_cal = trade_cal.fillna(method='ffill')
+
+        # Series.fillna with 'method' is deprecated and will raise in a future version. Use obj.ffill() or
+        # obj.bfill() instead.
+        # trade_cal = trade_cal.fillna(method='ffill')
+        trade_cal = trade_cal.ffill()
         time_index = trade_cal.loc[trade_cal == 1].index
 
     # 判断time_index的freq，当freq小于一天时，需要按交易时段取出部分index
     if time_index.freqstr is not None:
         freq_str = time_index.freqstr.lower().split('-')[0]
     else:
         freq_str = time_index.inferred_freq
@@ -1379,15 +1383,16 @@
         day:        D
         week:       W-SUN/...
         month:      M
         quarter:    Q-DEC/...
         year:       A-DEC/...
         由于周、季、年三种情况存在复合字符串，因此需要split
     '''
-    if freq_str[-1:].lower() in ['t', 'h']:
+    if (freq_str[-1:].lower() in ['t', 'h']) or (freq_str[-3:] in ['min']):
+        # freq_str for min in pandas 2.0 is 'T', in pandas 2.2 is 'MIN'
         idx_am = time_index.indexer_between_time(
                 start_time=start_am,
                 end_time=end_am,
                 include_start=include_start_am,
                 include_end=include_end_am,
         )
         idx_pm = time_index.indexer_between_time(
@@ -1470,14 +1475,16 @@
         'option': df_o[['name']] if not df_o.empty else pd.DataFrame(),
     }
     all_basics = pd.concat(
             (
                 all_data_types[asset_type.lower()] for asset_type in asset_types
             ),
     )
+    if all_basics.empty:
+        return ['N/A'] * len(symbols)
     try:
         names_found = all_basics.reindex(index=symbols)["name"].tolist()
     except Exception as e:
         raise RuntimeError(f'Error in get_symbol_names(): {e}')
     # replace all nan with 'N/A'
     names_found = ['N/A' if pd.isna(name) else name for name in names_found]
```

### Comparing `qteasy-1.1.7/qteasy/tsfuncs.py` & `qteasy-1.1.8/qteasy/tsfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.7/qteasy/utilfuncs.py` & `qteasy-1.1.8/qteasy/utilfuncs.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,15 +292,15 @@
             while mtries > 1:
                 try:
                     return f(*args, **kwargs)
                 except exception_to_check as e:
                     # TODO: define the error to escape retry: no permission, no such file, etc.
                     exception_to_escape = [ValueError, TypeError, AttributeError, FileNotFoundError, PermissionError,]
                     error_str = str(e)
-                    if ('没有访问该接口的权限' in error_str) or ('找不到' in error_str):
+                    if ('没有访问该接口的权限' in error_str) or ('token凭证码' in error_str):
                         raise e
                     if e.__class__ in exception_to_escape:
                         raise e
                     msg = f'Error in {f.__name__}: {e.__class__}:{str(e)}, Retrying in {mdelay} seconds...'
                     if mute:
                         if logger:
                             logger.debug(msg)
@@ -823,15 +823,16 @@
     """
     # public_holidays 是一个含两个list的tuple，存储了闭市的公共假期，第一个list是代表月份的数字，第二个list是代表日期的数字
     public_holidays = ([1, 1, 1, 4, 4, 4, 5, 5, 5, 10, 10, 10, 10, 10, 10, 10],
                        [1, 2, 3, 3, 4, 5, 1, 2, 3, 1, 2, 3, 4, 5, 6, 7])
     try:
         date = pd.to_datetime(date).floor(freq='d')
     except Exception:
-        raise ValueError('date is not a valid date time format, cannot be converted to timestamp')
+        msg = f'{date} is not a valid date time format, cannot be converted to timestamp'
+        raise ValueError(msg)
     if date.weekday() > 4:
         return False
     for m, d in zip(public_holidays[0], public_holidays[1]):
         if date.month == m and date.day == d:
             return False
     return True
 
@@ -921,32 +922,40 @@
     >>> is_market_trade_day('2019-01-01')
     False
     """
     try:
         _date = pd.to_datetime(date).floor(freq='d')
     except Exception as ex:
         ex.extra_info = f'{date} is not a valid date time format, cannot be converted to timestamp'
-        raise
+        raise ex
     if _date is None:
-        raise TypeError(f'{date} is not a valid date')
+        msg = f'{date} is not a valid date'
+        raise TypeError(msg)
     if not isinstance(exchange, str) and exchange in ['SSE', 'SZSE', 'CFFEX', 'SHFE', 'CZCE',
                                                       'DCE', 'INE', 'IB', 'XHKG']:
-        raise TypeError(f'exchange \'{exchange}\' is not a valid input')
+        msg = f'exchange \'{exchange}\' is not a valid input'
+        raise TypeError(msg)
     if qteasy.QT_TRADE_CALENDAR is not None:
         try:
             exchange_trade_cal = qteasy.QT_TRADE_CALENDAR.loc[exchange]
         except KeyError as e:
-            raise KeyError(f'Trade Calender for exchange: {e} was not properly downloaded, please refill data')
+            e.extra_info = f'Trade Calender for exchange: {exchange} is not downloaded, please refill data'
+            raise e
         try:
             is_open = exchange_trade_cal.loc[_date].is_open
-        except KeyError:
-            raise ValueError(f'The date {_date} is out of trade calendar range, please refill data')
+        except KeyError as e:
+            e.extra_info = f'Trade Calendar for exchange: {exchange} is not available, please refill data'
+            raise e
         return is_open == 1
     else:
-        warnings.warn('Trade Calendar is not available, will use maybe_trade_day instead to check trade day')
+        msg = 'Trade Calendar is not available,  will use maybe_trade_day instead to check trade day\n' \
+                'Trade Calendar can be downloaded to DataSource, Use:\n' \
+                'qteasy.refill_data_source(tables="basics")\n' \
+                'see more details in qteasy docs: https://qteasy.readthedocs.io/zh/latest/'
+        warnings.warn(msg, RuntimeWarning)
         return maybe_trade_day(_date)
 
 
 @lru_cache(maxsize=4)
 def last_known_market_trade_day(exchange: str = 'SSE'):
     """ 返回交易日列表中的最后一个已知交易日
 
@@ -963,25 +972,28 @@
     Returns
     -------
     datetime-like
         最后一个已知交易日的日期
     """
     if not isinstance(exchange, str) and exchange in ['SSE', 'SZSE', 'CFFEX', 'SHFE', 'CZCE',
                                                       'DCE', 'INE', 'IB', 'XHKG']:
-        raise TypeError(f'exchange \'{exchange}\' is not a valid input')
+        msg = f'exchange \'{exchange}\' is not a valid input'
+        raise TypeError(msg)
     if qteasy.QT_TRADE_CALENDAR is not None:
         try:
             exchange_trade_cal = qteasy.QT_TRADE_CALENDAR.loc[exchange]
         except KeyError as e:
-            raise KeyError(f'Trade Calender for exchange: {e} was not properly downloaded, please refill data')
+            msg = f'Trade Calender for exchange: {e} was not properly downloaded, please refill data'
+            raise KeyError(msg)
         return exchange_trade_cal[exchange_trade_cal.is_open == 1].index.max()
     else:
-        raise RuntimeError('Trade Calendar is not available, please download basic data into DataSource, Use:\n'
-                           'qteasy.refill_data_source(tables="basics")\n'
-                           'see more details in qteasy docs')
+        msg = 'Trade Calendar is not available, please download basic data into DataSource, Use:\n' \
+               'qteasy.refill_data_source(tables="basics")\n' \
+               'see more details in qteasy docs: https://qteasy.readthedocs.io/zh/latest/'
+        raise RuntimeError(msg)
 
 
 @lru_cache(maxsize=16)
 def prev_market_trade_day(date, exchange='SSE'):
     """ 根据交易所发布的交易日历找到某一日的上一交易日，需要提前准备QT_TRADE_CALENDAR数据
 
     - 如果date是交易日，则返回上一个交易日，如2020-12-24是交易日，它的前一天也是交易日，返回上一日2020-12-23
@@ -1020,17 +1032,18 @@
         e.extra_info = f'{date} is not a valid date time format, cannot be converted to timestamp'
         raise e
     if qteasy.QT_TRADE_CALENDAR is not None:
         exchange_trade_cal = qteasy.QT_TRADE_CALENDAR.loc[exchange]
         pretrade_date = exchange_trade_cal.loc[_date].pretrade_date
         return pd.to_datetime(pretrade_date)
     else:
-        raise RuntimeError('Trade Calendar is not available, please download basic data into DataSource, Use:\n'
-                           'qteasy.refill_data_source(tables="basics")\n'
-                           'see more details in qteasy docs')
+        msg = 'Trade Calendar is not available, please download basic data into DataSource, Use:\n' \
+                'qteasy.refill_data_source(tables="basics")\n' \
+                'see more details in qteasy docs: https://qteasy.readthedocs.io/zh/latest/'
+        raise RuntimeError(msg)
 
 
 @lru_cache(maxsize=16)
 def nearest_market_trade_day(date, exchange='SSE'):
     """ 根据交易所发布的交易日历找到某一日的最近交易日，需要提前准备QT_TRADE_CALENDAR数据
 
     - 如果date是交易日，返回date当日，如2020-12-24日是交易日，返回2020-12-24
@@ -1167,17 +1180,23 @@
 
     Examples
     --------
     >>> list_truncate([1,2,3,4,5,6,7,8,9,0], 4)
     >>> [[1,2,3,4], [5,6,7,8], [9,0]]
     """
 
-    assert isinstance(lst, list), f'first parameter should be a list, got {type(lst)}'
-    assert isinstance(trunc_size, int), f'second parameter should be an integer larger than 0'
-    assert trunc_size > 0, f'second parameter should be an integer larger than 0, got {trunc_size}'
+    if not isinstance(lst, list):
+        msg = f'first parameter should be a list, got {type(lst)}'
+        raise TypeError(msg)
+    if not isinstance(trunc_size, int):
+        msg = f'second parameter should be an integer larger than 0'
+        raise TypeError(msg)
+    if not trunc_size > 0:
+        msg = f'second parameter should be an integer larger than 0, got {trunc_size}'
+        raise ValueError(msg)
     total = len(lst)
     if total <= trunc_size:
         return [lst]
     else:
         sub_lists = []
         begin = 0
         end = trunc_size
@@ -1961,25 +1980,31 @@
     else:
         format_tags = []
         format_tags_positions = []
 
     cut_off_proportion = 0.7
 
     if not isinstance(s, str):
-        raise TypeError(f'the first argument should be a string, got {type(s)} instead')
+        msg = f'the first argument should be a string, got {type(s)} instead'
+        raise TypeError(msg)
     if not isinstance(n, int):
-        raise TypeError(f'the second argument should be an integer, got {type(n)} instead')
+        msg = f'the second argument should be an integer, got {type(n)} instead'
+        raise TypeError(msg)
     if not isinstance(ellipsis, str):
-        raise TypeError(f'the padder should be a character, got {type(ellipsis)} instead')
+        msg = f'the padder should be a character, got {type(ellipsis)} instead'
+        raise TypeError(msg)
     if not len(ellipsis) == 1:
-        raise ValueError(f'the padder should be a single character, got {len(ellipsis)} characters')
+        msg = f'the padder should be a single character, got {len(ellipsis)} characters'
+        raise ValueError(msg)
     if not isinstance(padder, str):
-        raise TypeError(f'the padder should be a character, got {type(padder)} instead')
+        msg = f'the padder should be a character, got {type(padder)} instead'
+        raise TypeError(msg)
     if n < 1:
-        raise ValueError(f'the expected length should be larger than 0, got {n}')
+        msg = f'the expected length should be larger than 0, got {n}'
+        raise ValueError(msg)
 
     length = len(s)
     if hans_aware:
         length += _count_hans(s)
 
     if (length <= n) and (padding == 'right'):
         res_str = s + padder * (n - length)
@@ -2146,14 +2171,15 @@
     >>> _count_hans('hello world')
     0
     >>> _count_hans('你好，世界')
     4
     """
     # for loop is faster than list comprehension and regex
     if not isinstance(s, str):
-        raise TypeError(f'the argument should be a string, got {type(s)} instead')
+        msg = f'should be a string, got {type(s)} instead'
+        raise TypeError(msg)
     hans_total = 0
     for char in s:
         if '\u4e00' <= char <= '\u9fff':
             hans_total += 1
     return hans_total
```

### Comparing `qteasy-1.1.7/qteasy/visual.py` & `qteasy-1.1.8/qteasy/visual.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.7/qteasy.egg-info/PKG-INFO` & `qteasy-1.1.8/qteasy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qteasy
-Version: 1.1.7
+Version: 1.1.8
 Summary: A fast quantitative investment tool kit
 Home-page: https://github.com/shepherdpp/qteasy
 Author: Jackie PENG
 Author-email: jackie PENG <jackie.pengzhao@gmail.com>
 Maintainer: Jackie PENG
 Maintainer-email: jackie PENG <jackie.pengzhao@gmail.com>
 License: Copyright <2019> <JACKIE PENG>
@@ -92,15 +92,15 @@
 > 我会尽快修复问题并回复大家的问题。
 
 ## 关于`qteasy`
 
 - 作者: **Jackie PENG**
 - email: *jackie_pengzhao@163.com*
 - Created: 2019, July, 16
-- Latest Version: `1.1.7`
+- Latest Version: `1.1.8`
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
```

### Comparing `qteasy-1.1.7/qteasy.egg-info/SOURCES.txt` & `qteasy-1.1.8/qteasy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.7/setup.cfg` & `qteasy-1.1.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qteasy
-version = 1.1.7
+version = 1.1.8
 author = Jackie PENG
 author_email = jackie.pengzhao@gmail.com
 maintainer = Jackie PENG
 description = A fast quantitative investment tool kit
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/shepherdpp/qteasy
```

### Comparing `qteasy-1.1.7/tests/test_broker.py` & `qteasy-1.1.8/tests/test_broker.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.7/tests/test_cashplan.py` & `qteasy-1.1.8/tests/test_cashplan.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,17 @@
         print(self.cp2)
         print(self.cp3)
         # test __str__()
         self.cp1.info()
         self.cp2.info()
         self.cp3.info()
         # test assersion errors
-        self.assertRaises(AssertionError, qt.CashPlan, '2016-01-01', [10000, 10000])
-        self.assertRaises(AssertionError, qt.CashPlan, '', '')
-        self.assertRaises(AssertionError, qt.CashPlan, '', [])
+        self.assertRaises(ValueError, qt.CashPlan, '2016-01-01', [10000, 10000])
+        self.assertRaises(TypeError, qt.CashPlan, '', '')
+        self.assertRaises(ValueError, qt.CashPlan, '', [])
         self.assertRaises(KeyError, qt.CashPlan, '2020-20-20', 10000)
         # test empty cash plan
         empty = CashPlan([], [])
         print(empty)
 
     def test_properties(self):
         self.assertEqual(self.cp1.amounts, [20000, 10000], 'property wrong')
```

### Comparing `qteasy-1.1.7/tests/test_config.py` & `qteasy-1.1.8/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.7/tests/test_core_sub_funcs.py` & `qteasy-1.1.8/tests/test_core_sub_funcs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.7/tests/test_cost.py` & `qteasy-1.1.8/tests/test_cost.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #   cost related functions.
 # ======================================
 import unittest
 
 import qteasy as qt
 import numpy as np
 
-from qteasy.finance import get_selling_result, get_purchase_result, calculate_fees
+from qteasy.finance import get_selling_result, get_purchase_result, calculate_fees, get_cost_pamams, update_cost
 
 
 class TestCost(unittest.TestCase):
     """ 测试所有跟交易成本计算相关的函数"""
     def setUp(self):
         self.amounts = np.array([10000., 20000., 10000.])
         self.op = np.array([0., 1., -0.33333333])
@@ -35,248 +35,308 @@
 
     def test_rate_operations(self):
         """测试交易费率对象"""
         self.assertEqual(self.r['buy_fix'], 0.0, 'Item got is incorrect')
         self.assertEqual(self.r['sell_fix'], 0.0, 'Item got is wrong')
         self.assertEqual(self.r['buy_rate'], 0.003, 'Item got is incorrect')
         self.assertEqual(self.r['sell_rate'], 0.001, 'Item got is incorrect')
-        self.assertEqual(self.r['buy_min'], 5., 'Item got is incorrect')
+        self.assertEqual(self.r['buy_min'], 5.0, 'Item got is incorrect')
         self.assertEqual(self.r['sell_min'], 0.0, 'Item got is incorrect')
         self.assertEqual(self.r['slipage'], 0.0, 'Item got is incorrect')
-        self.assertEqual(np.allclose(calculate_fees(self.amounts, None, None, **self.r),
-                                     [0.003, 0.003, 0.003]),
-                         True,
-                         'fee calculation wrong')
+
+        update_cost(self.r,
+                    buy_fix=5.,
+                    sell_fix=10.,
+                    )
+        self.assertEqual(self.r['buy_fix'], 5.0, 'Item got is incorrect')
+        self.assertEqual(self.r['sell_fix'], 10.0, 'Item got is incorrect')
+
+        fee_params = get_cost_pamams(self.r)
+        # basic buy/sell rate calculation
+        self.assertTrue(
+                np.allclose(
+                        calculate_fees(self.amounts, cost_params=fee_params),
+                        [0.003, 0.003, 0.003],
+                )
+        )
+        self.assertTrue(
+                np.allclose(
+                        calculate_fees(-self.amounts, cost_params=fee_params, is_buying=False),
+                        [0.001, 0.001, 0.001],
+                )
+        )
+        # buy/sell rate calculation with fixed fees
+        self.assertTrue(
+                np.allclose(
+                        calculate_fees(self.amounts, cost_params=fee_params, is_buying=True, fixed_fees=True),
+                        [5., 5., 5.],
+                )
+        )
+        self.assertTrue(
+                np.allclose(
+                        calculate_fees(-self.amounts, cost_params=fee_params, is_buying=False, fixed_fees=True),
+                        [10., 10., 10.],
+                )
+        )
+        # set buy and sell min feea
+        update_cost(self.r,
+                    buy_min=50.,
+                    sell_min=15.,
+                    )
+        self.assertEqual(self.r['buy_min'], 50., 'Item got is incorrect')
+        self.assertEqual(self.r['sell_min'], 15., 'Item got is incorrect')
+        fee_params = get_cost_pamams(self.r)
+        # buy/sell rate calculation with min fees
+        fees = calculate_fees(self.amounts, cost_params=fee_params, is_buying=True)
+        print(fees)
+        print(self.amounts)
+        print(self.amounts * fees)
+        self.assertTrue(
+                np.allclose(
+                        calculate_fees(self.amounts, cost_params=fee_params, is_buying=True),
+                        [.00502513, .003, .00502513],
+                )
+        )
+        fees = calculate_fees(-self.amounts, cost_params=fee_params, is_buying=False)
+        print(fees)
+        print(self.amounts)
+        print(self.amounts * fees)
+        self.assertTrue(
+                np.allclose(
+                        calculate_fees(-self.amounts, cost_params=fee_params, is_buying=False),
+                        [.0015, .001, .0015],
+                )
+        )
 
     def test_rate_fee(self):
         """测试买卖交易费率"""
         self.r['buy_rate'] = 0.003
         self.r['sell_rate'] = 0.001
         self.r['buy_fix'] = 0.
         self.r['sell_fix'] = 0.
         self.r['buy_min'] = 0.
         self.r['sell_min'] = 0.
         self.r['slipage'] = 0.
-        r = self.r
+        r = get_cost_pamams(self.r)
         print('\nSell result with fixed rate = 0.001 and moq = 0:')
-        print(get_selling_result(self.prices, self.amounts_to_sell, 0, **r))
-        test_rate_fee_result = get_selling_result(self.prices, self.amounts_to_sell, 0, **r)
+        print(get_selling_result(self.prices, self.amounts_to_sell, 0, r))
+        test_rate_fee_result = get_selling_result(self.prices, self.amounts_to_sell, 0, r)
         self.assertIs(np.allclose(test_rate_fee_result[0], [0., 0., -3333.3333]), True, 'result incorrect')
         self.assertAlmostEqual(test_rate_fee_result[1].sum(), 33299.999667, msg='result incorrect')
         self.assertAlmostEqual(test_rate_fee_result[2].sum(), 33.333333, msg='result incorrect')
 
         print('\nSell result with fixed rate = 0.001 and moq = 1:')
-        print(get_selling_result(self.prices, self.amounts_to_sell, 1., **r))
-        test_rate_fee_result = get_selling_result(self.prices, self.amounts_to_sell, 1, **r)
+        print(get_selling_result(self.prices, self.amounts_to_sell, 1., r))
+        test_rate_fee_result = get_selling_result(self.prices, self.amounts_to_sell, 1, r)
         self.assertIs(np.allclose(test_rate_fee_result[0], [0., 0., -3333]), True, 'result incorrect')
         self.assertAlmostEqual(test_rate_fee_result[1].sum(), 33296.67, msg='result incorrect')
         self.assertAlmostEqual(test_rate_fee_result[2].sum(), 33.33, msg='result incorrect')
 
         print('\nSell result with fixed rate = 0.001 and moq = 100:')
-        print(get_selling_result(self.prices, self.amounts_to_sell, 100, **r))
-        test_rate_fee_result = get_selling_result(self.prices, self.amounts_to_sell, 100, **r)
+        print(get_selling_result(self.prices, self.amounts_to_sell, 100, r))
+        test_rate_fee_result = get_selling_result(self.prices, self.amounts_to_sell, 100, r)
         self.assertIs(np.allclose(test_rate_fee_result[0], [0., 0., -3300]), True, 'result incorrect')
         self.assertAlmostEqual(test_rate_fee_result[1].sum(), 32967.0, msg='result incorrect')
         self.assertAlmostEqual(test_rate_fee_result[2].sum(), 33, msg='result incorrect')
 
         print('\nPurchase result with fixed rate = 0.003 and moq = 0:')
-        print(get_purchase_result(self.prices, self.cash_to_spend, 0, **r))
-        test_rate_fee_result = get_purchase_result(self.prices, self.cash_to_spend, 0, **r)
+        print(get_purchase_result(self.prices, self.cash_to_spend, 0, r))
+        test_rate_fee_result = get_purchase_result(self.prices, self.cash_to_spend, 0, r)
         self.assertIs(np.allclose(test_rate_fee_result[0], [0., 997.00897308, 0.]), True, 'result incorrect')
         self.assertAlmostEqual(test_rate_fee_result[1].sum(), -20000.0, msg='result incorrect')
         self.assertAlmostEqual(test_rate_fee_result[2].sum(), 59.82053838484547, msg='result incorrect')
 
         print('\nPurchase result with fixed rate = 0.003 and moq = 1:')
-        print(get_purchase_result(self.prices, self.cash_to_spend, 1, **r))
-        test_rate_fee_result = get_purchase_result(self.prices, self.cash_to_spend, 1, **r)
+        print(get_purchase_result(self.prices, self.cash_to_spend, 1, r))
+        test_rate_fee_result = get_purchase_result(self.prices, self.cash_to_spend, 1, r)
         self.assertIs(np.allclose(test_rate_fee_result[0], [0., 997., 0.]), True, 'result incorrect')
         self.assertAlmostEqual(test_rate_fee_result[1].sum(), -19999.82, msg='result incorrect')
         self.assertAlmostEqual(test_rate_fee_result[2].sum(), 59.82, msg='result incorrect')
 
         print('\nPurchase result with fixed rate = 0.003 and moq = 100:')
-        print(get_purchase_result(self.prices, self.cash_to_spend, 100, **r))
-        test_rate_fee_result = get_purchase_result(self.prices, self.cash_to_spend, 100, **r)
+        print(get_purchase_result(self.prices, self.cash_to_spend, 100, r))
+        test_rate_fee_result = get_purchase_result(self.prices, self.cash_to_spend, 100, r)
         self.assertIs(np.allclose(test_rate_fee_result[0], [0., 900., 0.]), True, 'result incorrect')
         self.assertAlmostEqual(test_rate_fee_result[1].sum(), -18054., msg='result incorrect')
         self.assertAlmostEqual(test_rate_fee_result[2].sum(), 54.0, msg='result incorrect')
 
     def test_min_fee(self):
         """测试最低交易费用"""
         self.r['buy_rate'] = 0.
         self.r['sell_rate'] = 0.
         self.r['buy_fix'] = 0.
         self.r['sell_fix'] = 0.
         self.r['buy_min'] = 300
         self.r['sell_min'] = 300
         self.r['slipage'] = 0.
-        r = self.r
+        r = get_cost_pamams(self.r)
         print('\npurchase result with fixed cost rate with min fee = 300 and moq = 0:')
-        print(get_purchase_result(self.prices, self.cash_to_spend, 0, **r))
-        test_min_fee_result = get_purchase_result(self.prices, self.cash_to_spend, 0, **r)
+        print(get_purchase_result(self.prices, self.cash_to_spend, 0, r))
+        test_min_fee_result = get_purchase_result(self.prices, self.cash_to_spend, 0, r)
         self.assertIs(np.allclose(test_min_fee_result[0], [0., 985, 0.]), True, 'result incorrect')
         self.assertAlmostEqual(test_min_fee_result[1].sum(), -20000.0, msg='result incorrect')
         self.assertAlmostEqual(test_min_fee_result[2].sum(), 300.0, msg='result incorrect')
 
         print('\npurchase result with fixed cost rate with min fee = 300 and moq = 10:')
-        print(get_purchase_result(self.prices, self.cash_to_spend, 10, **r))
-        test_min_fee_result = get_purchase_result(self.prices, self.cash_to_spend, 10, **r)
+        print(get_purchase_result(self.prices, self.cash_to_spend, 10, r))
+        test_min_fee_result = get_purchase_result(self.prices, self.cash_to_spend, 10, r)
         self.assertIs(np.allclose(test_min_fee_result[0], [0., 980, 0.]), True, 'result incorrect')
         self.assertAlmostEqual(test_min_fee_result[1].sum(), -19900.0, msg='result incorrect')
         self.assertAlmostEqual(test_min_fee_result[2].sum(), 300.0, msg='result incorrect')
 
         print('\npurchase result with fixed cost rate with min fee = 300 and moq = 100:')
-        print(get_purchase_result(self.prices, self.cash_to_spend, 100, **r))
-        test_min_fee_result = get_purchase_result(self.prices, self.cash_to_spend, 100, **r)
+        print(get_purchase_result(self.prices, self.cash_to_spend, 100, r))
+        test_min_fee_result = get_purchase_result(self.prices, self.cash_to_spend, 100, r)
         self.assertIs(np.allclose(test_min_fee_result[0], [0., 900, 0.]), True, 'result incorrect')
         self.assertAlmostEqual(test_min_fee_result[1].sum(), -18300.0, msg='result incorrect')
         self.assertAlmostEqual(test_min_fee_result[2].sum(), 300.0, msg='result incorrect')
 
         print('\nselling result with fixed cost rate with min fee = 300 and moq = 0:')
-        print(get_selling_result(self.prices, self.amounts_to_sell, 0, **r))
-        test_min_fee_result = get_selling_result(self.prices, self.amounts_to_sell, 0, **r)
+        print(get_selling_result(self.prices, self.amounts_to_sell, 0, r))
+        test_min_fee_result = get_selling_result(self.prices, self.amounts_to_sell, 0, r)
         self.assertIs(np.allclose(test_min_fee_result[0], [0, 0, -3333.3333]), True, 'result incorrect')
         self.assertAlmostEqual(test_min_fee_result[1].sum(), 33033.333)
         self.assertAlmostEqual(test_min_fee_result[2].sum(), 300.0)
 
         print('\nselling result with fixed cost rate with min fee = 300 and moq = 1:')
-        print(get_selling_result(self.prices, self.amounts_to_sell, 1, **r))
-        test_min_fee_result = get_selling_result(self.prices, self.amounts_to_sell, 1, **r)
+        print(get_selling_result(self.prices, self.amounts_to_sell, 1, r))
+        test_min_fee_result = get_selling_result(self.prices, self.amounts_to_sell, 1, r)
         self.assertIs(np.allclose(test_min_fee_result[0], [0, 0, -3333]), True, 'result incorrect')
         self.assertAlmostEqual(test_min_fee_result[1].sum(), 33030)
         self.assertAlmostEqual(test_min_fee_result[2].sum(), 300.0)
 
         print('\nselling result with fixed cost rate with min fee = 300 and moq = 100:')
-        print(get_selling_result(self.prices, self.amounts_to_sell, 100, **r))
-        test_min_fee_result = get_selling_result(self.prices, self.amounts_to_sell, 100, **r)
+        print(get_selling_result(self.prices, self.amounts_to_sell, 100, r))
+        test_min_fee_result = get_selling_result(self.prices, self.amounts_to_sell, 100, r)
         self.assertIs(np.allclose(test_min_fee_result[0], [0, 0, -3300]), True, 'result incorrect')
         self.assertAlmostEqual(test_min_fee_result[1].sum(), 32700)
         self.assertAlmostEqual(test_min_fee_result[2].sum(), 300.0)
 
     def test_rate_with_min(self):
         """测试最低交易费用对其他交易费率参数的影响"""
         self.r['buy_rate'] = 0.0153
         self.r['sell_rate'] = 0.01
         self.r['buy_fix'] = 0.
         self.r['sell_fix'] = 0.
         self.r['buy_min'] = 300
         self.r['sell_min'] = 333
         self.r['slipage'] = 0.
-        r = self.r
+        r = get_cost_pamams(self.r)
         print('\npurchase result with fixed cost rate with buy_rate = 0.0153, min fee = 300 and moq = 0:')
-        print(get_purchase_result(self.prices, self.cash_to_spend, 0, **r))
-        test_rate_with_min_result = get_purchase_result(self.prices, self.cash_to_spend, 0, **r)
+        print(get_purchase_result(self.prices, self.cash_to_spend, 0, r))
+        test_rate_with_min_result = get_purchase_result(self.prices, self.cash_to_spend, 0, r)
         self.assertIs(np.allclose(test_rate_with_min_result[0], [0., 984.9305624, 0.]), True, 'result incorrect')
         self.assertAlmostEqual(test_rate_with_min_result[1].sum(), -20000.0, msg='result incorrect')
         self.assertAlmostEqual(test_rate_with_min_result[2].sum(), 301.3887520929774, msg='result incorrect')
 
         print('\npurchase result with fixed cost rate with buy_rate = 0.0153, min fee = 300 and moq = 10:')
-        print(get_purchase_result(self.prices, self.cash_to_spend, 10, **r))
-        test_rate_with_min_result = get_purchase_result(self.prices, self.cash_to_spend, 10, **r)
+        print(get_purchase_result(self.prices, self.cash_to_spend, 10, r))
+        test_rate_with_min_result = get_purchase_result(self.prices, self.cash_to_spend, 10, r)
         self.assertIs(np.allclose(test_rate_with_min_result[0], [0., 980, 0.]), True, 'result incorrect')
         self.assertAlmostEqual(test_rate_with_min_result[1].sum(), -19900.0, msg='result incorrect')
         self.assertAlmostEqual(test_rate_with_min_result[2].sum(), 300.0, msg='result incorrect')
 
         print('\npurchase result with fixed cost rate with buy_rate = 0.0153, min fee = 300 and moq = 100:')
-        print(get_purchase_result(self.prices, self.cash_to_spend, 100, **r))
-        test_rate_with_min_result = get_purchase_result(self.prices, self.cash_to_spend, 100, **r)
+        print(get_purchase_result(self.prices, self.cash_to_spend, 100, r))
+        test_rate_with_min_result = get_purchase_result(self.prices, self.cash_to_spend, 100, r)
         self.assertIs(np.allclose(test_rate_with_min_result[0], [0., 900, 0.]), True, 'result incorrect')
         self.assertAlmostEqual(test_rate_with_min_result[1].sum(), -18300.0, msg='result incorrect')
         self.assertAlmostEqual(test_rate_with_min_result[2].sum(), 300.0, msg='result incorrect')
 
         print('\nselling result with fixed cost rate with sell_rate = 0.01, min fee = 333 and moq = 0:')
-        print(get_selling_result(self.prices, self.amounts_to_sell, 0, **r))
-        test_rate_with_min_result = get_selling_result(self.prices, self.amounts_to_sell, 0, **r)
+        print(get_selling_result(self.prices, self.amounts_to_sell, 0, r))
+        test_rate_with_min_result = get_selling_result(self.prices, self.amounts_to_sell, 0, r)
         self.assertIs(np.allclose(test_rate_with_min_result[0], [0, 0, -3333.3333]), True, 'result incorrect')
         self.assertAlmostEqual(test_rate_with_min_result[1].sum(), 32999.99967)
         self.assertAlmostEqual(test_rate_with_min_result[2].sum(), 333.33333)
 
         print('\nselling result with fixed cost rate with sell_rate = 0.01, min fee = 333 and moq = 1:')
-        print(get_selling_result(self.prices, self.amounts_to_sell, 1, **r))
-        test_rate_with_min_result = get_selling_result(self.prices, self.amounts_to_sell, 1, **r)
+        print(get_selling_result(self.prices, self.amounts_to_sell, 1, r))
+        test_rate_with_min_result = get_selling_result(self.prices, self.amounts_to_sell, 1, r)
         self.assertIs(np.allclose(test_rate_with_min_result[0], [0, 0, -3333]), True, 'result incorrect')
         self.assertAlmostEqual(test_rate_with_min_result[1].sum(), 32996.7)
         self.assertAlmostEqual(test_rate_with_min_result[2].sum(), 333.3)
 
         print('\nselling result with fixed cost rate with sell_rate = 0.01, min fee = 333 and moq = 100:')
-        print(get_selling_result(self.prices, self.amounts_to_sell, 100, **r))
-        test_rate_with_min_result = get_selling_result(self.prices, self.amounts_to_sell, 100, **r)
+        print(get_selling_result(self.prices, self.amounts_to_sell, 100, r))
+        test_rate_with_min_result = get_selling_result(self.prices, self.amounts_to_sell, 100, r)
         self.assertIs(np.allclose(test_rate_with_min_result[0], [0, 0, -3300]), True, 'result incorrect')
         self.assertAlmostEqual(test_rate_with_min_result[1].sum(), 32667.0)
         self.assertAlmostEqual(test_rate_with_min_result[2].sum(), 333.0)
 
     def test_fixed_fee(self):
         """测试固定交易费用"""
         self.r['buy_rate'] = 0.
         self.r['sell_rate'] = 0.
         self.r['buy_fix'] = 200
         self.r['sell_fix'] = 150
         self.r['buy_min'] = 0
         self.r['sell_min'] = 0
         self.r['slipage'] = 0
-        r = self.r
+        r = get_cost_pamams(self.r)
         print('\nselling result of fixed cost with fixed fee = 150 and moq=0:')
-        print(get_selling_result(self.prices, self.amounts_to_sell, 0, **r))
-        test_fixed_fee_result = get_selling_result(self.prices, self.amounts_to_sell, 0, **r)
+        print(get_selling_result(self.prices, self.amounts_to_sell, 0, r))
+        test_fixed_fee_result = get_selling_result(self.prices, self.amounts_to_sell, 0, r)
         self.assertIs(np.allclose(test_fixed_fee_result[0], [0, 0, -3333.3333]), True, 'result incorrect')
         self.assertAlmostEqual(test_fixed_fee_result[1].sum(), 33183.333, msg='result incorrect')
         self.assertAlmostEqual(test_fixed_fee_result[2].sum(), 150.0, msg='result incorrect')
 
         print('\nselling result of fixed cost with fixed fee = 150 and moq=100:')
-        print(get_selling_result(self.prices, self.amounts_to_sell, 100, **r))
-        test_fixed_fee_result = get_selling_result(self.prices, self.amounts_to_sell, 100, **r)
+        print(get_selling_result(self.prices, self.amounts_to_sell, 100, r))
+        test_fixed_fee_result = get_selling_result(self.prices, self.amounts_to_sell, 100, r)
         self.assertIs(np.allclose(test_fixed_fee_result[0], [0, 0, -3300.]), True,
                       f'result incorrect, {test_fixed_fee_result[0]} does not equal to [0,0,-3400]')
         self.assertAlmostEqual(test_fixed_fee_result[1].sum(), 32850., msg='result incorrect')
         self.assertAlmostEqual(test_fixed_fee_result[2].sum(), 150., msg='result incorrect')
 
         print('\npurchase result of fixed cost with fixed fee = 200:')
-        print(get_purchase_result(self.prices, self.cash_to_spend, 0, **r))
-        test_fixed_fee_result = get_purchase_result(self.prices, self.cash_to_spend, 0, **r)
+        print(get_purchase_result(self.prices, self.cash_to_spend, 0, r))
+        test_fixed_fee_result = get_purchase_result(self.prices, self.cash_to_spend, 0, r)
         self.assertIs(np.allclose(test_fixed_fee_result[0], [0., 990., 0.]), True, 'result incorrect')
         self.assertAlmostEqual(test_fixed_fee_result[1].sum(), -20000.0, msg='result incorrect')
         self.assertAlmostEqual(test_fixed_fee_result[2].sum(), 200.0, msg='result incorrect')
 
         print('\npurchase result of fixed cost with fixed fee = 200:')
-        print(get_purchase_result(self.prices, self.cash_to_spend, 100, **r))
-        test_fixed_fee_result = get_purchase_result(self.prices, self.cash_to_spend, 100, **r)
+        print(get_purchase_result(self.prices, self.cash_to_spend, 100, r))
+        test_fixed_fee_result = get_purchase_result(self.prices, self.cash_to_spend, 100, r)
         self.assertIs(np.allclose(test_fixed_fee_result[0], [0., 900., 0.]), True, 'result incorrect')
         self.assertAlmostEqual(test_fixed_fee_result[1].sum(), -18200.0, msg='result incorrect')
         self.assertAlmostEqual(test_fixed_fee_result[2].sum(), 200.0, msg='result incorrect')
 
     def test_slipage(self):
         """测试交易滑点"""
         self.r['buy_fix'] = 0
         self.r['sell_fix'] = 0
         self.r['buy_min'] = 0
         self.r['sell_min'] = 0
         self.r['buy_rate'] = 0.003
         self.r['sell_rate'] = 0.001
         self.r['slipage'] = 1E-9
-        r = self.r
+        r = get_cost_pamams(self.r)
         print('\npurchase result of fixed rate = 0.003 and slipage = 1E-10 and moq = 0:')
-        print(get_purchase_result(self.prices, self.cash_to_spend, 0, **r))
+        print(get_purchase_result(self.prices, self.cash_to_spend, 0, r))
         print('\npurchase result of fixed rate = 0.003 and slipage = 1E-10 and moq = 100:')
-        print(get_purchase_result(self.prices, self.cash_to_spend, 100, **r))
+        print(get_purchase_result(self.prices, self.cash_to_spend, 100, r))
         print('\nselling result with fixed rate = 0.001 and slipage = 1E-10:')
-        print(get_selling_result(self.prices, self.amounts_to_sell, 0, **r))
+        print(get_selling_result(self.prices, self.amounts_to_sell, 0, r))
 
-        test_fixed_fee_result = get_selling_result(self.prices, self.amounts_to_sell, 0, **r)
+        test_fixed_fee_result = get_selling_result(self.prices, self.amounts_to_sell, 0, r)
         self.assertIs(np.allclose(test_fixed_fee_result[0], [0, 0, -3333.3333]), True,
                       f'{test_fixed_fee_result[0]} does not equal to [0, 0, -10000]')
         self.assertAlmostEqual(test_fixed_fee_result[1].sum(), 33298.88855591,
                                 msg=f'{test_fixed_fee_result[1]} does not equal to 33298.')
         self.assertAlmostEqual(test_fixed_fee_result[2].sum(), 34.44444409,
                                 msg=f'{test_fixed_fee_result[2]} does not equal to -36.666663.')
 
-        test_fixed_fee_result = get_purchase_result(self.prices, self.cash_to_spend, 0, **r)
+        test_fixed_fee_result = get_purchase_result(self.prices, self.cash_to_spend, 0, r)
         self.assertIs(np.allclose(test_fixed_fee_result[0], [0., 996.98909294, 0.]), True, 'result incorrect')
         self.assertAlmostEqual(test_fixed_fee_result[1].sum(), -20000.0, msg='result incorrect')
         self.assertAlmostEqual(test_fixed_fee_result[2].sum(), 60.21814121353513, msg='result incorrect')
 
-        test_fixed_fee_result = get_purchase_result(self.prices, self.cash_to_spend, 100, **r)
+        test_fixed_fee_result = get_purchase_result(self.prices, self.cash_to_spend, 100, r)
         self.assertIs(np.allclose(test_fixed_fee_result[0], [0., 900., 0.]), True, 'result incorrect')
         self.assertAlmostEqual(test_fixed_fee_result[1].sum(), -18054.36, msg='result incorrect')
         self.assertAlmostEqual(test_fixed_fee_result[2].sum(), 54.36, msg='result incorrect')
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `qteasy-1.1.7/tests/test_datasource.py` & `qteasy-1.1.8/tests/test_datasource.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     def setUp(self):
         """ execute before each test"""
         from qteasy import QT_ROOT_PATH
         self.qt_root_path = QT_ROOT_PATH
         self.data_test_dir = 'data_test/'
         # 测试数据不会放在默认的data路径下，以免与已有的文件混淆
         # 使用测试数据库进行除"test_get_history_panel()"以外的其他全部测试
-        # TODO: do not explicitly leave password and user in the code
         from qteasy import QT_CONFIG
 
         print('preparing test data sources with configurations...')
         self.ds_db = DataSource(
                 'db',
                 host=QT_CONFIG['test_db_host'],
                 port=QT_CONFIG['test_db_port'],
@@ -136,14 +135,19 @@
             'pre_close':  [10., 10., 10., 10., 10., 10., 10., 10., 10., 10., 10., 10., 10., 10., 10.],
             'change':     [10., 10., 10., 10., 10., 10., 10., 10., 10., 10., 10., 10., 10., 10., 10.],
             'pct_chg':    [10., 10., 10., 10., 10., 10., 10., 10., 10., 10., 10., 10., 10., 10., 10.],
             'vol':        [10., 10., 10., 10., 10., 10., 10., 10., 10., 10., 10., 10., 10., 10., 10.],
             'amount':     [10., 10., 10., 10., 10., 10., 10., 10., 10., 10., 10., 10., 10., 10., 10.]
         })
 
+        # 删除datasource目录下可能存在的所有文件
+        for ds in [self.ds_csv, self.ds_hdf, self.ds_fth]:
+            for f in os.listdir(ds.file_path):
+                os.remove(os.path.join(ds.file_path, f))
+
     def test_properties(self):
         """test properties"""
         self.assertEqual(self.ds_csv.__str__(), 'file://csv@qt_root/data_test/')
         self.assertEqual(self.ds_hdf.__str__(), 'file://hdf@qt_root/data_test/')
         self.assertEqual(self.ds_fth.__str__(), 'file://fth@qt_root/data_test/')
         self.assertEqual(self.ds_db.__str__(), 'db:mysql://localhost@3306/test_db')
 
@@ -653,14 +657,75 @@
                 self.assertEqual(target_index[i], loaded_index[i])
             rows, cols = target_values.shape
             for i in range(rows):
                 for j in range(cols):
                     self.assertEqual(target_values[i, j], loaded_values[i, j])
             self.assertEqual(list(df_res.columns), list(loaded_df.columns))
 
+    def test_delete_file_records(self):
+        """ test deleting a few records from a file"""
+
+        for ds in [self.ds_csv, self.ds_fth, self.ds_hdf]:
+            # create a test dataframe
+            test_sys_df = pd.DataFrame(
+                    {
+                        'account_id':     [1, 2, 3, 4, 5],
+                        'user_name':      ['account1', 'account2', 'account3', 'account4', 'account5'],
+                        'created_time':   ['2024-11-12', '2024-11-12', '2024-11-12', '2024-11-12', '2024-11-12'],
+                        'cash_amount':    [1000, 2000, 3000, 4000, 5000],
+                        'available_cash': [1000, 2000, 3000, 4000, 5000],
+                        'total_invest':   [1000, 2000, 3000, 4000, 5000],
+                    }
+            )
+            table_name = 'sys_op_live_account'
+            test_sys_df = set_primary_key_frame(test_sys_df, primary_key=['account_id'], pk_dtypes=['int'])
+            set_primary_key_index(test_sys_df, primary_key=['account_id'], pk_dtypes=['int'])
+
+            # 删除测试路径中已经存在的数据文件
+            ds.drop_file(table_name)
+
+            self.assertFalse(ds.file_exists(table_name))
+            # 写入数据到csv, fth, hdf文件
+            ds.write_file(test_sys_df, table_name)
+
+            self.assertTrue(ds.file_exists(table_name))
+
+            # 删除csv, fth, hdf文件中的部分数据
+            res = ds.delete_file_records(table_name, 'account_id', [2, 4])
+
+            loaded_df = ds.read_file(table_name, primary_key=['account_id'], pk_dtypes=['int'])
+            # set_primary_key_index(loaded_df, primary_key=['account_id'], pk_dtypes=['int'])
+
+            self.assertEqual(res, 2)
+            self.assertEqual(loaded_df.shape[0], 3)
+            self.assertEqual(loaded_df.index[0], 1)
+            self.assertEqual(loaded_df.index[1], 3)
+            self.assertEqual(loaded_df.index[2], 5)
+            # check if all values are correct
+            self.assertEqual(loaded_df.loc[1, 'user_name'], 'account1')
+            self.assertEqual(loaded_df.loc[1, 'cash_amount'], 1000)
+            self.assertEqual(loaded_df.loc[1, 'available_cash'], 1000)
+            self.assertEqual(loaded_df.loc[1, 'total_invest'], 1000)
+            self.assertEqual(loaded_df.loc[3, 'user_name'], 'account3')
+            self.assertEqual(loaded_df.loc[3, 'cash_amount'], 3000)
+            self.assertEqual(loaded_df.loc[3, 'available_cash'], 3000)
+            self.assertEqual(loaded_df.loc[3, 'total_invest'], 3000)
+            self.assertEqual(loaded_df.loc[5, 'user_name'], 'account5')
+            self.assertEqual(loaded_df.loc[5, 'cash_amount'], 5000)
+            self.assertEqual(loaded_df.loc[5, 'available_cash'], 5000)
+            self.assertEqual(loaded_df.loc[5, 'total_invest'], 5000)
+
+        print('deleting records that are not in the file and with wrong primary key')
+        for ds in [self.ds_csv, self.ds_fth, self.ds_hdf]:
+            res = ds.delete_file_records(table_name, primary_key='account_id', record_ids=[2, 4])
+            self.assertEqual(res, 0)
+
+            with self.assertRaises(TypeError):
+                ds.delete_file_records(table_name, primary_key='account_id', record_ids='1,2,3')
+
     def test_write_and_read_database(self):
         """ test DataSource method read_database and write_database"""
         print(f'write and read a MultiIndex dataframe to database')
         df = set_primary_key_frame(self.df, primary_key=['ts_code', 'trade_date'], pk_dtypes=['str', 'TimeStamp'])
         print(f'following dataframe with multiple index will be written to local database:\n'
               f'{df}')
 
@@ -780,14 +845,93 @@
 
         cov = self.ds_db.get_db_table_coverage('test_db_table', 'trade_date')
         print(cov)
         self.assertIsInstance(cov, list)
         self.assertEqual(cov,
                          ['20211112', '20211113'])
 
+    def test_delete_database_records(self):
+        """ test delete database records"""
+        print(f'delete records from database')
+        con = connect(
+                host=self.ds_db.host,
+                port=self.ds_db.port,
+                user=self.ds_db.__user__,
+                password=self.ds_db.__password__,
+                db=self.ds_db.db_name,
+        )
+        cursor = con.cursor()
+        table_name = 'sys_op_live_accounts'
+        # 删除数据库中的临时表
+        sql = f"DROP TABLE IF EXISTS {table_name}"
+        cursor.execute(sql)
+        con.commit()
+        con.close()
+
+        test_sys_df = pd.DataFrame(
+                {
+                    'account_id': [1, 2, 3, 4, 5],
+                    'user_name': ['account1', 'account2', 'account3', 'account4', 'account5'],
+                    'created_time': ['2024-11-12', '2024-11-12', '2024-11-12', '2024-11-12', '2024-11-12'],
+                    'cash_amount': [1000, 2000, 3000, 4000, 5000],
+                    'available_cash': [1000, 2000, 3000, 4000, 5000],
+                    'total_invest': [1000, 2000, 3000, 4000, 5000],
+                }
+        )
+
+        self.ds_db.write_database(test_sys_df, table_name)
+        loaded_df = self.ds_db.read_database(table_name)
+        set_primary_key_index(loaded_df, primary_key=['account_id'], pk_dtypes=['int'])
+        print(f'df retrieved from database is\n'
+              f'{loaded_df}\n')
+
+        print(f'delete records from database table')
+        res = self.ds_db.delete_database_records(table_name, 'account_id', [2, 4])
+        loaded_df = self.ds_db.read_database(table_name)
+        set_primary_key_index(loaded_df, primary_key=['account_id'], pk_dtypes=['int'])
+        print(f'df retrieved from database after deleting records is\n'
+              f'{loaded_df}\n')
+
+        self.assertEqual(res, 2)
+        self.assertEqual(loaded_df.shape[0], 3)
+        self.assertEqual(loaded_df.index[0], 1)
+        self.assertEqual(loaded_df.index[1], 3)
+        self.assertEqual(loaded_df.index[2], 5)
+        # check if all values are correct
+        self.assertEqual(loaded_df.loc[1, 'user_name'], 'account1')
+        self.assertEqual(loaded_df.loc[1, 'cash_amount'], 1000)
+        self.assertEqual(loaded_df.loc[1, 'available_cash'], 1000)
+        self.assertEqual(loaded_df.loc[1, 'total_invest'], 1000)
+        self.assertEqual(loaded_df.loc[3, 'user_name'], 'account3')
+        self.assertEqual(loaded_df.loc[3, 'cash_amount'], 3000)
+        self.assertEqual(loaded_df.loc[3, 'available_cash'], 3000)
+        self.assertEqual(loaded_df.loc[3, 'total_invest'], 3000)
+        self.assertEqual(loaded_df.loc[5, 'user_name'], 'account5')
+        self.assertEqual(loaded_df.loc[5, 'cash_amount'], 5000)
+        self.assertEqual(loaded_df.loc[5, 'available_cash'], 5000)
+        self.assertEqual(loaded_df.loc[5, 'total_invest'], 5000)
+
+        print('delete records that are not found in the database table')
+        res = self.ds_db.delete_database_records(table_name, 'account_id', [2, 4])
+        loaded_df = self.ds_db.read_database(table_name)
+        set_primary_key_index(loaded_df, primary_key=['account_id'], pk_dtypes=['int'])
+        print(f'df retrieved from database after deleting records is\n'
+              f'{loaded_df}\n')
+
+        self.assertEqual(res, 0)
+        self.assertEqual(loaded_df.shape[0], 3)
+        self.assertEqual(loaded_df.index[0], 1)
+        self.assertEqual(loaded_df.index[1], 3)
+        self.assertEqual(loaded_df.index[2], 5)
+
+        print('wrong parameters are given')
+        self.assertRaises(RuntimeError, self.ds_db.delete_database_records, table_name, 'wrong_key', [1])
+        self.assertRaises(TypeError, self.ds_db.delete_database_records, table_name, 'account_id', 1)
+        self.assertRaises(RuntimeError, self.ds_db.delete_database_records, table_name, 'account_id', '1, 2')
+
     def test_update_database(self):
         """ test the function update_database()"""
         print(f'update a database table with new arr on same primary key')
         df = set_primary_key_frame(self.df, primary_key=['ts_code', 'trade_date'], pk_dtypes=['str', 'TimeStamp'])
         df_add = set_primary_key_frame(self.df_add, primary_key=['ts_code', 'trade_date'],
                                        pk_dtypes=['str', 'TimeStamp'])
         df_res = set_primary_key_frame(self.df_res, primary_key=['ts_code', 'trade_date'],
@@ -817,14 +961,16 @@
         for i in range(len(saved_index)):
             self.assertEqual(saved_index[i], loaded_index[i])
         rows, cols = saved_values.shape
         for i in range(rows):
             for j in range(cols):
                 if pd.isna(saved_values[i, j]):
                     self.assertTrue(pd.isna(loaded_values[i, j]))
+                elif isinstance(saved_values[i, j], pd.Timestamp):
+                    self.assertEqual(saved_values[i, j].date(), loaded_values[i, j])
                 else:
                     self.assertEqual(saved_values[i, j], loaded_values[i, j])
         self.assertEqual(list(self.df.columns), list(loaded_df.columns))
 
     # noinspection PyPep8Naming
     def test_read_write_update_table_data(self):
         """ test DataSource method read_table_data() and write_table_data()
@@ -989,14 +1135,102 @@
 
             # 删除所有的表
             for ds in all_data_sources:
                 ds.drop_table_data(table)
                 print('all table data are cleared')
                 ds.overview()
 
+    def test_delete_table_data(self):
+        """ test function delete_table_data()"""
+
+        # all system tables and all datasources should be tested
+        tables_to_test = ['sys_op_live_accounts', 'sys_op_positions', 'sys_op_trade_orders', 'sys_op_trade_results']
+        all_data_sources = [self.ds_csv, self.ds_hdf, self.ds_fth, self.ds_db]
+
+        # test data
+        test_account_df = pd.DataFrame(
+                {
+                    'account_id': [1, 2, 3, 4, 5],
+                    'user_name': ['account1', 'account2', 'account3', 'account4', 'account5'],
+                    'created_time': ['2023-11-12', '2023-11-12', '2023-11-12', '2023-11-12', '2023-11-12'],
+                    'cash_amount': [1000, 2000, 3000, 4000, 5000],
+                    'available_cash': [1000, 2000, 3000, 4000, 5000],
+                    'total_invest': [1000, 2000, 3000, 4000, 5000],
+                }
+        )
+        test_positions_df = pd.DataFrame(
+                {
+                    'pos_id': [1, 2, 3, 4, 5],
+                    'account_id': [1, 1, 2, 3, 5],
+                    'symbol': ['000001.SZ', '000002.SZ', '000003.SZ', '000004.SZ', '000005.SZ'],
+                    'position': ['long', 'short', 'long', 'short', 'long'],
+                    'qty': [100, 200, 300, 400, 500],
+                    'available_qty': [100, 200, 300, 400, 500],
+                    'cost': [10, 20, 30, 40, 50],
+                }
+        )
+        test_orders_df = pd.DataFrame(
+                {
+                    'order_id': [1, 2, 3, 4, 5],
+                    'pos_id': [1, 2, 3, 4, 5],
+                    'direction': ['buy', 'sell', 'buy', 'sell', 'buy'],
+                    'order_type': ['market', 'limit', 'market', 'limit', 'market'],
+                    'qty': [100, 200, 300, 400, 500],
+                    'price': [10, 20, 30, 40, 50],
+                    'submitted_time': ['2023-11-12', '2023-11-12', '2023-11-12', '2023-11-12', '2023-11-12'],
+                    'status': ['partial-filled', 'filled', 'canceled', 'filled', 'canceled'],
+                }
+        )
+        test_results_df = pd.DataFrame(
+                {
+                    'result_id': [1, 2, 3, 4, 5],
+                    'order_id': [1, 2, 3, 4, 5],
+                    'filled_qty': [50, 100, 0, 400, 0],
+                    'price': [10, 20, 0, 40, 0],
+                    'transaction_fee': [1, 2, 0, 4, 0],
+                    'execution_time': ['2023-11-12', '2023-11-12', '2023-11-12', '2023-11-12', '2023-11-12'],
+                    'canceled_qty': [0, 0, 300, 0, 500],
+                    'delivery_amount': [500, 1000, 0, 2000, 0],
+                    'delivery_status': ['delivered', 'delivered', 'delivered', 'delivered', 'delivered'],
+                }
+        )
+
+        test_data_for_tables = {
+            'sys_op_live_accounts': test_account_df,
+            'sys_op_positions': test_positions_df,
+            'sys_op_trade_orders': test_orders_df,
+            'sys_op_trade_results': test_results_df
+        }
+
+        # test on all data sources and tables
+        for ds in all_data_sources:
+            for table in tables_to_test:
+                print(f'dropping table {table} from datasource: {ds.source_type}-{ds.connection_type}')
+                ds.drop_table_data(table)
+                print(f'-- Done! --')
+                self.assertFalse(ds.table_data_exists(table))
+                print(f'table {table} is deleted from datasource: {ds.source_type}-{ds.connection_type}')
+
+                # write test data to the table
+                test_data = test_data_for_tables[table]
+                ds.write_table_data(test_data, table)
+
+                # check if the table is written
+                self.assertTrue(ds.table_data_exists(table))
+
+                # delete records from the table
+                ds.delete_sys_table_data(table, record_ids=[2, 4])
+
+                df = ds.read_table_data(table)
+                print(f'df read from arr source: \n{ds.source_type}-{ds.connection_type} \nis:\n{df}')
+                self.assertEqual(df.shape[0], 3)
+                self.assertEqual(df.index[0], 1)
+                self.assertEqual(df.index[1], 3)
+                self.assertEqual(df.index[2], 5)
+
     def test_get_history_panel_data(self):
         """ test getting arr, from real database """
         ds = qt.QT_DATA_SOURCE
         shares = ['000001.SZ', '000002.SZ', '600067.SH', '000300.SH', '518860.SH']
         htypes = 'pe, close, open, swing, strength'
         htypes = str_to_list(htypes)
         start = '20210101'
@@ -1939,41 +2173,41 @@
                 self.assertEqual(test_shuffled_signal_data['pos_id'], res['pos_id'])
                 self.assertEqual(test_shuffled_signal_data['order_type'], res['order_type'])
                 self.assertEqual(test_shuffled_signal_data['status'], res['status'])
                 self.assertEqual(test_shuffled_signal_data['direction'], res['direction'])
                 self.assertEqual(test_shuffled_signal_data['price'], res['price'])
                 self.assertEqual(test_shuffled_signal_data['qty'], res['qty'])
 
-            # 测试传入无效的id时是否引发KeyError异常
-            print(f'test passing invalid id to read_sys_table_data')
-            res = ds.read_sys_table_data(table, record_id=-1)
-            self.assertIsNone(res)
-            res = ds.read_sys_table_data(table, record_id=0)
-            self.assertIsNone(res)
-            res = ds.read_sys_table_data(table, record_id=999)
-            self.assertIsNone(res)
-
-            # 测试传入无效的表名时是否引发KeyError异常
-            with self.assertRaises(KeyError):
-                ds.read_sys_table_data('invalid_table')
-
-            # 测试传入无效的kwargs时是否引发KeyError异常
-            with self.assertRaises(KeyError):
-                ds.read_sys_table_data('test_table', invalid_column='test')
-
-            # 测试写入不正确的dict时是否返回错误
-            print(f'test writing wrong data fields into table')
-            with self.assertRaises(Exception):
-                ds.insert_sys_table_data(
-                    table,
-                    **{
-                        'wrong_key1': 'wrong_value',
-                        'wrong_key2': 321,
-                    }
-                )
+                # 测试传入无效的id时是否引发KeyError异常
+                print(f'test passing invalid id to read_sys_table_data')
+                res = ds.read_sys_table_data(table, record_id=-1)
+                self.assertIsNone(res)
+                res = ds.read_sys_table_data(table, record_id=0)
+                self.assertIsNone(res)
+                res = ds.read_sys_table_data(table, record_id=999)
+                self.assertIsNone(res)
+
+                # 测试传入无效的表名时是否引发KeyError异常
+                with self.assertRaises(KeyError):
+                    ds.read_sys_table_data('invalid_table')
+
+                # 测试传入无效的kwargs时是否引发KeyError异常
+                with self.assertRaises(KeyError):
+                    ds.read_sys_table_data('test_table', invalid_column='test')
+
+                # 测试写入不正确的dict时是否返回错误
+                print(f'test writing wrong data fields into table')
+                with self.assertRaises(Exception):
+                    ds.insert_sys_table_data(
+                        table,
+                        **{
+                            'wrong_key1': 'wrong_value',
+                            'wrong_key2': 321,
+                        }
+                    )
 
         # 测试读取指定id的记录
         # 循环使用所有的示例数据在所有的sys表上进行测试，测试覆盖所有的source_type
         # 首先在数据表中写入五条数据，每条数据稍有变化
         # 1，测试随机读取一条已经存在的数据，验证是否读取正确
         # 2，测试传入无效的id时是否返回None
         # 3，测试传入kwargs筛选数据，验证是否读取正确
```

### Comparing `qteasy-1.1.7/tests/test_eastmoney.py` & `qteasy-1.1.8/tests/test_eastmoney.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.7/tests/test_evaluations.py` & `qteasy-1.1.8/tests/test_evaluations.py`

 * *Files 4% similar despite different names*

```diff
@@ -314,80 +314,80 @@
         """
         # TODO: implement this test
         pass
 
     # noinspection PyTypeChecker
     def test_fv(self):
         print(f'test with test arr and empty DataFrame')
-        self.assertAlmostEquals(eval_fv(self.test_data1), 6.39245474)
-        self.assertAlmostEquals(eval_fv(self.test_data2), 10.05126375)
-        self.assertAlmostEquals(eval_fv(self.test_data3), 6.95068113)
-        self.assertAlmostEquals(eval_fv(self.test_data4), 8.86508591)
-        self.assertAlmostEquals(eval_fv(self.test_data5), 4.58627048)
-        self.assertAlmostEquals(eval_fv(self.test_data6), 4.10346795)
-        self.assertAlmostEquals(eval_fv(self.test_data7), 2.92532313)
-        self.assertAlmostEquals(eval_fv(pd.DataFrame()), -np.inf)
+        self.assertAlmostEqual(eval_fv(self.test_data1), 6.39245474)
+        self.assertAlmostEqual(eval_fv(self.test_data2), 10.05126375)
+        self.assertAlmostEqual(eval_fv(self.test_data3), 6.95068113)
+        self.assertAlmostEqual(eval_fv(self.test_data4), 8.86508591)
+        self.assertAlmostEqual(eval_fv(self.test_data5), 4.58627048)
+        self.assertAlmostEqual(eval_fv(self.test_data6), 4.10346795)
+        self.assertAlmostEqual(eval_fv(self.test_data7), 2.92532313)
+        self.assertAlmostEqual(eval_fv(pd.DataFrame()), -np.inf)
         print(f'Error testing')
         self.assertRaises(TypeError, eval_fv, 15)
         self.assertRaises(KeyError,
                           eval_fv,
                           pd.DataFrame([1, 2, 3], columns=['non_value']))
 
     # noinspection PyTypeChecker
     def test_max_drawdown(self):
         print(f'test with test arr and empty DataFrame')
-        self.assertAlmostEquals(eval_max_drawdown(self.test_data1)[0], 0.264274308)
+        self.assertAlmostEqual(eval_max_drawdown(self.test_data1)[0], 0.264274308)
         self.assertEqual(eval_max_drawdown(self.test_data1)[1], 53)
         self.assertEqual(eval_max_drawdown(self.test_data1)[2], 86)
         self.assertTrue(np.isnan(eval_max_drawdown(self.test_data1)[3]))
-        self.assertAlmostEquals(eval_max_drawdown(self.test_data2)[0], 0.334690849)
+        self.assertAlmostEqual(eval_max_drawdown(self.test_data2)[0], 0.334690849)
         self.assertEqual(eval_max_drawdown(self.test_data2)[1], 0)
         self.assertEqual(eval_max_drawdown(self.test_data2)[2], 10)
         self.assertEqual(eval_max_drawdown(self.test_data2)[3], 19)
-        self.assertAlmostEquals(eval_max_drawdown(self.test_data3)[0], 0.244452899)
+        self.assertAlmostEqual(eval_max_drawdown(self.test_data3)[0], 0.244452899)
         self.assertEqual(eval_max_drawdown(self.test_data3)[1], 90)
         self.assertEqual(eval_max_drawdown(self.test_data3)[2], 99)
         self.assertTrue(np.isnan(eval_max_drawdown(self.test_data3)[3]))
-        self.assertAlmostEquals(eval_max_drawdown(self.test_data4)[0], 0.201849684)
+        self.assertAlmostEqual(eval_max_drawdown(self.test_data4)[0], 0.201849684)
         self.assertEqual(eval_max_drawdown(self.test_data4)[1], 14)
         self.assertEqual(eval_max_drawdown(self.test_data4)[2], 50)
         self.assertEqual(eval_max_drawdown(self.test_data4)[3], 54)
-        self.assertAlmostEquals(eval_max_drawdown(self.test_data5)[0], 0.534206456)
+        self.assertAlmostEqual(eval_max_drawdown(self.test_data5)[0], 0.534206456)
         self.assertEqual(eval_max_drawdown(self.test_data5)[1], 21)
         self.assertEqual(eval_max_drawdown(self.test_data5)[2], 60)
         self.assertTrue(np.isnan(eval_max_drawdown(self.test_data5)[3]))
-        self.assertAlmostEquals(eval_max_drawdown(self.test_data6)[0], 0.670062689)
+        self.assertAlmostEqual(eval_max_drawdown(self.test_data6)[0], 0.670062689)
         self.assertEqual(eval_max_drawdown(self.test_data6)[1], 0)
         self.assertEqual(eval_max_drawdown(self.test_data6)[2], 70)
         self.assertTrue(np.isnan(eval_max_drawdown(self.test_data6)[3]))
-        self.assertAlmostEquals(eval_max_drawdown(self.test_data7)[0], 0.783577449)
+        self.assertAlmostEqual(eval_max_drawdown(self.test_data7)[0], 0.783577449)
         self.assertEqual(eval_max_drawdown(self.test_data7)[1], 17)
         self.assertEqual(eval_max_drawdown(self.test_data7)[2], 51)
         self.assertTrue(np.isnan(eval_max_drawdown(self.test_data7)[3]))
         self.assertEqual(eval_max_drawdown(pd.DataFrame()), -np.inf)
         print(f'Error testing')
         self.assertRaises(TypeError, eval_fv, 15)
         self.assertRaises(KeyError,
                           eval_fv,
                           pd.DataFrame([1, 2, 3], columns=['non_value']))
         # test max drawdown == 0:
         # TODO: investigate: how does divide by zero change?
-        self.assertAlmostEquals(eval_max_drawdown(self.test_data4 - 5)[0], 1.0770474121951792)
+        self.assertAlmostEqual(eval_max_drawdown(self.test_data4 - 5)[0], 1.0770474121951792)
         self.assertEqual(eval_max_drawdown(self.test_data4 - 5)[1], 14)
         self.assertEqual(eval_max_drawdown(self.test_data4 - 5)[2], 50)
 
     # noinspection PyTypeChecker
     def test_info_ratio(self):
         reference = self.test_data1
-        self.assertAlmostEquals(eval_info_ratio(self.test_data2, reference, 'value'), 0.075553316)
-        self.assertAlmostEquals(eval_info_ratio(self.test_data3, reference, 'value'), 0.018949457)
-        self.assertAlmostEquals(eval_info_ratio(self.test_data4, reference, 'value'), 0.056328143)
-        self.assertAlmostEquals(eval_info_ratio(self.test_data5, reference, 'value'), -0.004270068)
-        self.assertAlmostEquals(eval_info_ratio(self.test_data6, reference, 'value'), 0.009198027)
-        self.assertAlmostEquals(eval_info_ratio(self.test_data7, reference, 'value'), -0.000890283)
+        self.assertAlmostEqual(eval_info_ratio(self.test_data2, reference, 'value'), 0.075553316)
+        self.assertAlmostEqual(eval_info_ratio(self.test_data3, reference, 'value'), 0.018949457)
+        self.assertAlmostEqual(eval_info_ratio(self.test_data4, reference, 'value'), 0.056328143)
+        self.assertAlmostEqual(eval_info_ratio(self.test_data5, reference, 'value'), -0.004270068)
+        self.assertAlmostEqual(eval_info_ratio(self.test_data6, reference, 'value'), 0.009198027)
+        self.assertAlmostEqual(eval_info_ratio(self.test_data7, reference, 'value'), -0.000890283)
 
     def test_volatility(self):
         self.assertAlmostEqual(eval_volatility(self.test_data1), 0.748646166)
         self.assertAlmostEqual(eval_volatility(self.test_data2), 0.75527442)
         self.assertAlmostEqual(eval_volatility(self.test_data3), 0.654188853)
         self.assertAlmostEqual(eval_volatility(self.test_data4), 0.688375814)
         self.assertAlmostEqual(eval_volatility(self.test_data5), 1.089989522)
@@ -503,15 +503,15 @@
                                         0.36166601, 0.36142665, 0.35954942, 0.35846915, 0.35886759,
                                         0.35813867, 0.35642888, 0.35375231, 0.35061783, 0.35078463,
                                         0.34995508, 0.34688918, 0.34548257, 0.34633158, 0.34622833,
                                         0.34652111, 0.34622774, 0.34540951, 0.34418809, 0.34276593,
                                         0.34160916, 0.33811193, 0.33822709, 0.3391685, 0.33883381])
         test_volatility = eval_volatility(self.long_data)
         test_volatility_roll = self.long_data['volatility'].values
-        self.assertAlmostEqual = (test_volatility, np.nanmean(expected_volatility))
+        self.assertAlmostEqual(test_volatility, np.nanmean(expected_volatility))
         self.assertTrue(np.allclose(expected_volatility, test_volatility_roll, equal_nan=True))
 
     # noinspection PyCallingNonCallable
     def test_sharp(self):
         self.assertAlmostEqual(eval_sharp(self.test_data1, 0), 0.970116743)
         self.assertAlmostEqual(eval_sharp(self.test_data2, 0), 2.654078559)
         self.assertAlmostEqual(eval_sharp(self.test_data3, 0), 1.573319618)
@@ -624,20 +624,20 @@
         test_sharp = eval_sharp(self.long_data, 0.015)
         expected = float(np.nanmean(expected_sharp))
         self.assertAlmostEqual(expected, test_sharp)
         self.assertTrue(np.allclose(self.long_data['sharp'].values, expected_sharp, equal_nan=True))
 
     def test_beta(self):
         reference = self.test_data1
-        self.assertAlmostEquals(eval_beta(self.test_data2, reference, 'value'), -0.017148939)
-        self.assertAlmostEquals(eval_beta(self.test_data3, reference, 'value'), -0.042204233)
-        self.assertAlmostEquals(eval_beta(self.test_data4, reference, 'value'), -0.15652986)
-        self.assertAlmostEquals(eval_beta(self.test_data5, reference, 'value'), -0.049195532)
-        self.assertAlmostEquals(eval_beta(self.test_data6, reference, 'value'), -0.026995082)
-        self.assertAlmostEquals(eval_beta(self.test_data7, reference, 'value'), -0.01147809)
+        self.assertAlmostEqual(eval_beta(self.test_data2, reference, 'value'), -0.017148939)
+        self.assertAlmostEqual(eval_beta(self.test_data3, reference, 'value'), -0.042204233)
+        self.assertAlmostEqual(eval_beta(self.test_data4, reference, 'value'), -0.15652986)
+        self.assertAlmostEqual(eval_beta(self.test_data5, reference, 'value'), -0.049195532)
+        self.assertAlmostEqual(eval_beta(self.test_data6, reference, 'value'), -0.026995082)
+        self.assertAlmostEqual(eval_beta(self.test_data7, reference, 'value'), -0.01147809)
 
         self.assertRaises(TypeError, eval_beta, [1, 2, 3], reference, 'value')
         self.assertRaises(TypeError, eval_beta, self.test_data3, [1, 2, 3], 'value')
         self.assertRaises(KeyError, eval_beta, self.test_data3, reference, 'not_found_value')
 
         # 测试长数据的beta计算
         expected_beta = np.array([np.nan, np.nan, np.nan, np.nan, np.nan,
@@ -739,25 +739,25 @@
                                   -0.10004159, -0.10857084, -0.12209301, -0.11605758, -0.11105113,
                                   -0.1155195, -0.11569505, -0.10513348, -0.09611072, -0.10719791,
                                   -0.10843965, -0.11025856, -0.10247839, -0.10554044, -0.10927647,
                                   -0.10645088, -0.09982498, -0.10542734, -0.09631372, -0.08229695])
         test_beta_mean = eval_beta(self.long_data, self.long_bench, 'value')
         test_beta_roll = self.long_data['beta'].values
         expected = float(np.nanmean(expected_beta))
-        self.assertAlmostEquals(test_beta_mean, expected)
+        self.assertAlmostEqual(test_beta_mean, expected)
         self.assertTrue(np.allclose(test_beta_roll, expected_beta, equal_nan=True))
 
     def test_alpha(self):
         reference = self.test_data1
-        self.assertAlmostEquals(eval_alpha(self.test_data2, 5, reference, 'value', 0.5), 11.63072977)
-        self.assertAlmostEquals(eval_alpha(self.test_data3, 5, reference, 'value', 0.5), 1.886590071)
-        self.assertAlmostEquals(eval_alpha(self.test_data4, 5, reference, 'value', 0.5), 6.827021872)
-        self.assertAlmostEquals(eval_alpha(self.test_data5, 5, reference, 'value', 0.92), -1.192265168)
-        self.assertAlmostEquals(eval_alpha(self.test_data6, 5, reference, 'value', 0.92), -1.437142359)
-        self.assertAlmostEquals(eval_alpha(self.test_data7, 5, reference, 'value', 0.92), -1.781311545)
+        self.assertAlmostEqual(eval_alpha(self.test_data2, 5, reference, 'value', 0.5), 11.63072977)
+        self.assertAlmostEqual(eval_alpha(self.test_data3, 5, reference, 'value', 0.5), 1.886590071)
+        self.assertAlmostEqual(eval_alpha(self.test_data4, 5, reference, 'value', 0.5), 6.827021872)
+        self.assertAlmostEqual(eval_alpha(self.test_data5, 5, reference, 'value', 0.92), -1.192265168)
+        self.assertAlmostEqual(eval_alpha(self.test_data6, 5, reference, 'value', 0.92), -1.437142359)
+        self.assertAlmostEqual(eval_alpha(self.test_data7, 5, reference, 'value', 0.92), -1.781311545)
 
         # 测试长数据的alpha计算
         expected_alpha = np.array([np.nan, np.nan, np.nan, np.nan, np.nan,
                                    np.nan, np.nan, np.nan, np.nan, np.nan,
                                    np.nan, np.nan, np.nan, np.nan, np.nan,
                                    np.nan, np.nan, np.nan, np.nan, np.nan,
                                    np.nan, np.nan, np.nan, np.nan, np.nan,
@@ -855,42 +855,42 @@
                                    0.48594916, 0.4456216, 0.52008189, 0.60548684, 0.62792473,
                                    0.56645031, 0.62766439, 0.71829315, 0.69481356, 0.59550329,
                                    0.58133754, 0.59014148, 0.58026655, 0.61719273, 0.67373203,
                                    0.75573056, 0.89501633, 0.8347253, 0.87964685, 0.89015835])
         test_alpha_mean = eval_alpha(self.long_data, 100, self.long_bench, 'value')
         test_alpha_roll = self.long_data['alpha'].values
         expected = float(np.nanmean(expected_alpha))
-        self.assertAlmostEquals(test_alpha_mean, expected)
+        self.assertAlmostEqual(test_alpha_mean, expected)
         self.assertTrue(np.allclose(test_alpha_roll, expected_alpha, equal_nan=True))
 
     def test_calmar(self):
         """test evaluate function eval_calmar()"""
         # TODO: implement this test
         pass
 
     def test_benchmark(self):
         reference = self.test_data1
         tr, yr = eval_benchmark(self.test_data2, reference, 'value')
-        self.assertAlmostEquals(tr, 0.19509091)
-        self.assertAlmostEquals(yr, 0.929154957)
+        self.assertAlmostEqual(tr, 0.19509091)
+        self.assertAlmostEqual(yr, 0.929154957)
         tr, yr = eval_benchmark(self.test_data3, reference, 'value')
-        self.assertAlmostEquals(tr, 0.19509091)
-        self.assertAlmostEquals(yr, 0.929154957)
+        self.assertAlmostEqual(tr, 0.19509091)
+        self.assertAlmostEqual(yr, 0.929154957)
         tr, yr = eval_benchmark(self.test_data4, reference, 'value')
-        self.assertAlmostEquals(tr, 0.19509091)
-        self.assertAlmostEquals(yr, 0.929154957)
+        self.assertAlmostEqual(tr, 0.19509091)
+        self.assertAlmostEqual(yr, 0.929154957)
         tr, yr = eval_benchmark(self.test_data5, reference, 'value')
-        self.assertAlmostEquals(tr, 0.19509091)
-        self.assertAlmostEquals(yr, 0.929154957)
+        self.assertAlmostEqual(tr, 0.19509091)
+        self.assertAlmostEqual(yr, 0.929154957)
         tr, yr = eval_benchmark(self.test_data6, reference, 'value')
-        self.assertAlmostEquals(tr, 0.19509091)
-        self.assertAlmostEquals(yr, 0.929154957)
+        self.assertAlmostEqual(tr, 0.19509091)
+        self.assertAlmostEqual(yr, 0.929154957)
         tr, yr = eval_benchmark(self.test_data7, reference, 'value')
-        self.assertAlmostEquals(tr, 0.19509091)
-        self.assertAlmostEquals(yr, 0.929154957)
+        self.assertAlmostEqual(tr, 0.19509091)
+        self.assertAlmostEqual(yr, 0.929154957)
 
     def test_evaluate(self):
         """ 测试回测结果评价函数"""
         # TODO: implement this test
         pass
```

### Comparing `qteasy-1.1.7/tests/test_fast_experiments.py` & `qteasy-1.1.8/tests/test_fast_experiments.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.7/tests/test_historypanel.py` & `qteasy-1.1.8/tests/test_historypanel.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.7/tests/test_loop.py` & `qteasy-1.1.8/tests/test_loop.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import unittest
 
 import qteasy as qt
 import pandas as pd
 import numpy as np
 
 from qteasy.backtest import apply_loop, process_loop_results
-
+from qteasy.finance import get_cost_pamams
 from qteasy.history import stack_dataframes, dataframe_to_hp
 
 
 class TestLoop(unittest.TestCase):
     """通过一个假设但精心设计的例子来测试loop_step以及loop方法的正确性"""
 
     def setUp(self):
@@ -2184,28 +2184,23 @@
                  [259.4270, 559.9112, 0.0000, 15820.6915, 0.0000, 24483.5953],
                  [0.0000, 559.9112, 0.0000, 18321.5674, 0.0000, 24486.1895],
                  [0.0000, 0.0000, 0.0000, 24805.3389, 0.0000, 24805.3389],
                  [0.0000, 0.0000, 0.0000, 24805.3389, 0.0000, 24805.3389]])
 
     def test_loop_step_pt_sb00(self):
         """ test loop step PT-signal, sell first"""
+        cost_params = get_cost_pamams(self.rate)
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=0,
                                                          own_cash=10000,
                                                          own_amounts=np.zeros(7, dtype='float'),
                                                          available_cash=10000,
                                                          available_amounts=np.zeros(7, dtype='float'),
                                                          op=self.pt_signals[0],
                                                          prices=self.prices[0],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=True,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -2222,21 +2217,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=0,
                                                          own_cash=self.pt_res_sb00[2][7],
                                                          own_amounts=self.pt_res_sb00[2][0:7],
                                                          available_cash=self.pt_res_sb00[2][7],
                                                          available_amounts=self.pt_res_sb00[2][0:7],
                                                          op=self.pt_signals[3],
                                                          prices=self.prices[3],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=True,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -2253,21 +2242,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=0,
                                                          own_cash=self.pt_res_sb00[30][7],
                                                          own_amounts=self.pt_res_sb00[30][0:7],
                                                          available_cash=self.pt_res_sb00[30][7],
                                                          available_amounts=self.pt_res_sb00[30][0:7],
                                                          op=self.pt_signals[31],
                                                          prices=self.prices[31],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=True,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -2284,21 +2267,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=0,
                                                          own_cash=self.pt_res_sb00[59][7] + 10000,
                                                          own_amounts=self.pt_res_sb00[59][0:7],
                                                          available_cash=self.pt_res_sb00[59][7] + 10000,
                                                          available_amounts=self.pt_res_sb00[59][0:7],
                                                          op=self.pt_signals[60],
                                                          prices=self.prices[60],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=True,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -2315,21 +2292,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=0,
                                                          own_cash=cash,
                                                          own_amounts=amounts,
                                                          available_cash=cash,
                                                          available_amounts=amounts,
                                                          op=self.pt_signals[61],
                                                          prices=self.prices[61],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=True,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -2346,21 +2317,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=0,
                                                          own_cash=self.pt_res_sb00[95][7],
                                                          own_amounts=self.pt_res_sb00[95][0:7],
                                                          available_cash=self.pt_res_sb00[95][7],
                                                          available_amounts=self.pt_res_sb00[95][0:7],
                                                          op=self.pt_signals[96],
                                                          prices=self.prices[96],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=True,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -2377,21 +2342,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=0,
                                                          own_cash=cash,
                                                          own_amounts=amounts,
                                                          available_cash=cash,
                                                          available_amounts=amounts,
                                                          op=self.pt_signals[97],
                                                          prices=self.prices[97],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=True,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -2403,28 +2362,23 @@
         cash = cash + c_g.sum() + c_s.sum()
         amounts = amounts + a_p + a_s
         self.assertAlmostEqual(cash, self.pt_res_sb00[97][7], 2)
         self.assertTrue(np.allclose(amounts, self.pt_res_sb00[97][0:7]))
 
     def test_loop_step_pt_bs00(self):
         """ test loop step PT-signal, buy first"""
+        cost_params = get_cost_pamams(self.rate)
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=0,
                                                          own_cash=10000.,
                                                          own_amounts=np.zeros(7, dtype='float'),
                                                          available_cash=10000.,
                                                          available_amounts=np.zeros(7, dtype='float'),
                                                          op=self.pt_signals[0],
                                                          prices=self.prices[0],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=False,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -2441,21 +2395,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=0,
                                                          own_cash=self.pt_res_bs00[2][7],
                                                          own_amounts=self.pt_res_bs00[2][0:7],
                                                          available_cash=self.pt_res_bs00[2][7],
                                                          available_amounts=self.pt_res_bs00[2][0:7],
                                                          op=self.pt_signals[3],
                                                          prices=self.prices[3],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=False,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -2472,21 +2420,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=0,
                                                          own_cash=self.pt_res_bs00[30][7],
                                                          own_amounts=self.pt_res_bs00[30][0:7],
                                                          available_cash=self.pt_res_bs00[30][7],
                                                          available_amounts=self.pt_res_bs00[30][0:7],
                                                          op=self.pt_signals[31],
                                                          prices=self.prices[31],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=False,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -2503,21 +2445,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=0,
                                                          own_cash=self.pt_res_bs00[59][7] + 10000,
                                                          own_amounts=self.pt_res_bs00[59][0:7],
                                                          available_cash=self.pt_res_bs00[59][7] + 10000,
                                                          available_amounts=self.pt_res_bs00[59][0:7],
                                                          op=self.pt_signals[60],
                                                          prices=self.prices[60],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=False,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -2534,21 +2470,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=0,
                                                          own_cash=cash,
                                                          own_amounts=amounts,
                                                          available_cash=cash,
                                                          available_amounts=amounts,
                                                          op=self.pt_signals[61],
                                                          prices=self.prices[61],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=False,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -2565,21 +2495,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=0,
                                                          own_cash=self.pt_res_bs00[95][7],
                                                          own_amounts=self.pt_res_bs00[95][0:7],
                                                          available_cash=self.pt_res_bs00[95][7],
                                                          available_amounts=self.pt_res_bs00[95][0:7],
                                                          op=self.pt_signals[96],
                                                          prices=self.prices[96],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=False,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -2596,21 +2520,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=0,
                                                          own_cash=cash,
                                                          own_amounts=amounts,
                                                          available_cash=cash,
                                                          available_amounts=amounts,
                                                          op=self.pt_signals[97],
                                                          prices=self.prices[97],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=False,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -2622,28 +2540,23 @@
         cash = cash + c_g.sum() + c_s.sum()
         amounts = amounts + a_p + a_s
         self.assertAlmostEqual(cash, self.pt_res_bs00[97][7], 2)
         self.assertTrue(np.allclose(amounts, self.pt_res_bs00[97][0:7]))
 
     def test_loop_step_ps_sb00(self):
         """ test loop step PS-signal, sell first"""
+        cost_params = get_cost_pamams(self.rate)
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=1,
                                                          own_cash=10000.,
                                                          own_amounts=np.zeros(7, dtype='float'),
                                                          available_cash=10000.,
                                                          available_amounts=np.zeros(7, dtype='float'),
                                                          op=self.ps_signals[0],
                                                          prices=self.prices[0],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=True,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -2660,21 +2573,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=1,
                                                          own_cash=self.ps_res_sb00[2][7],
                                                          own_amounts=self.ps_res_sb00[2][0:7],
                                                          available_cash=self.ps_res_sb00[2][7],
                                                          available_amounts=self.ps_res_sb00[2][0:7],
                                                          op=self.ps_signals[3],
                                                          prices=self.prices[3],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=True,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -2691,21 +2598,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=1,
                                                          own_cash=self.ps_res_sb00[30][7],
                                                          own_amounts=self.ps_res_sb00[30][0:7],
                                                          available_cash=self.ps_res_sb00[30][7],
                                                          available_amounts=self.ps_res_sb00[30][0:7],
                                                          op=self.ps_signals[31],
                                                          prices=self.prices[31],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=True,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -2722,21 +2623,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=1,
                                                          own_cash=self.ps_res_sb00[59][7] + 10000.,
                                                          own_amounts=self.ps_res_sb00[59][0:7],
                                                          available_cash=self.ps_res_sb00[59][7] + 10000.,
                                                          available_amounts=self.ps_res_sb00[59][0:7],
                                                          op=self.ps_signals[60],
                                                          prices=self.prices[60],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=True,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -2753,21 +2648,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=1,
                                                          own_cash=cash,
                                                          own_amounts=amounts,
                                                          available_cash=cash,
                                                          available_amounts=amounts,
                                                          op=self.ps_signals[61],
                                                          prices=self.prices[61],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=True,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -2784,21 +2673,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=1,
                                                          own_cash=self.ps_res_sb00[95][7],
                                                          own_amounts=self.ps_res_sb00[95][0:7],
                                                          available_cash=self.ps_res_sb00[95][7],
                                                          available_amounts=self.ps_res_sb00[95][0:7],
                                                          op=self.ps_signals[96],
                                                          prices=self.prices[96],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=True,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -2815,21 +2698,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=1,
                                                          own_cash=cash,
                                                          own_amounts=amounts,
                                                          available_cash=cash,
                                                          available_amounts=amounts,
                                                          op=self.ps_signals[97],
                                                          prices=self.prices[97],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=True,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -2841,28 +2718,23 @@
         cash = cash + c_g.sum() + c_s.sum()
         amounts = amounts + a_p + a_s
         self.assertAlmostEqual(cash, self.ps_res_sb00[97][7], 2)
         self.assertTrue(np.allclose(amounts, self.ps_res_sb00[97][0:7]))
 
     def test_loop_step_ps_bs00(self):
         """ test loop step PS-signal, buy first"""
+        cost_params = get_cost_pamams(self.rate)
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=1,
                                                          own_cash=10000.,
                                                          own_amounts=np.zeros(7, dtype='float'),
                                                          available_cash=10000.,
                                                          available_amounts=np.zeros(7, dtype='float'),
                                                          op=self.ps_signals[0],
                                                          prices=self.prices[0],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=False,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -2879,21 +2751,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=1,
                                                          own_cash=self.ps_res_bs00[2][7],
                                                          own_amounts=self.ps_res_sb00[2][0:7],
                                                          available_cash=self.ps_res_bs00[2][7],
                                                          available_amounts=self.ps_res_bs00[2][0:7],
                                                          op=self.ps_signals[3],
                                                          prices=self.prices[3],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=False,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -2910,21 +2776,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=1,
                                                          own_cash=self.ps_res_bs00[30][7],
                                                          own_amounts=self.ps_res_sb00[30][0:7],
                                                          available_cash=self.ps_res_bs00[30][7],
                                                          available_amounts=self.ps_res_bs00[30][0:7],
                                                          op=self.ps_signals[31],
                                                          prices=self.prices[31],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=False,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -2941,21 +2801,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=1,
                                                          own_cash=self.ps_res_bs00[59][7] + 10000,
                                                          own_amounts=self.ps_res_bs00[59][0:7],
                                                          available_cash=self.ps_res_bs00[59][7] + 10000,
                                                          available_amounts=self.ps_res_bs00[59][0:7],
                                                          op=self.ps_signals[60],
                                                          prices=self.prices[60],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=False,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -2972,21 +2826,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=1,
                                                          own_cash=cash,
                                                          own_amounts=amounts,
                                                          available_cash=cash,
                                                          available_amounts=amounts,
                                                          op=self.ps_signals[61],
                                                          prices=self.prices[61],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=False,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -3003,21 +2851,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=1,
                                                          own_cash=self.ps_res_bs00[95][7],
                                                          own_amounts=self.ps_res_bs00[95][0:7],
                                                          available_cash=self.ps_res_bs00[95][7],
                                                          available_amounts=self.ps_res_bs00[95][0:7],
                                                          op=self.ps_signals[96],
                                                          prices=self.prices[96],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=False,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -3034,21 +2876,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=1,
                                                          own_cash=cash,
                                                          own_amounts=amounts,
                                                          available_cash=cash,
                                                          available_amounts=amounts,
                                                          op=self.ps_signals[97],
                                                          prices=self.prices[97],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=False,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -3060,28 +2896,23 @@
         cash = cash + c_g.sum() + c_s.sum()
         amounts = amounts + a_p + a_s
         self.assertAlmostEqual(cash, self.ps_res_bs00[97][7], 2)
         self.assertTrue(np.allclose(amounts, self.ps_res_bs00[97][0:7]))
 
     def test_loop_step_vs_sb00(self):
         """test loop step of Volume Signal type of signals"""
+        cost_params = get_cost_pamams(self.rate)
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=2,
                                                          own_cash=10000.,
                                                          own_amounts=np.zeros(7, dtype='float'),
                                                          available_cash=10000.,
                                                          available_amounts=np.zeros(7, dtype='float'),
                                                          op=self.vs_signals[0],
                                                          prices=self.prices[0],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=True,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -3098,21 +2929,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=2,
                                                          own_cash=self.vs_res_sb00[2][7],
                                                          own_amounts=self.vs_res_sb00[2][0:7],
                                                          available_cash=self.vs_res_sb00[2][7],
                                                          available_amounts=self.vs_res_sb00[2][0:7],
                                                          op=self.vs_signals[3],
                                                          prices=self.prices[3],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=True,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -3129,21 +2954,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=2,
                                                          own_cash=self.vs_res_sb00[30][7],
                                                          own_amounts=self.vs_res_sb00[30][0:7],
                                                          available_cash=self.vs_res_sb00[30][7],
                                                          available_amounts=self.vs_res_sb00[30][0:7],
                                                          op=self.vs_signals[31],
                                                          prices=self.prices[31],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=True,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -3160,21 +2979,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=2,
                                                          own_cash=self.vs_res_sb00[59][7] + 10000,
                                                          own_amounts=self.vs_res_sb00[59][0:7],
                                                          available_cash=self.vs_res_sb00[59][7] + 10000,
                                                          available_amounts=self.vs_res_sb00[59][0:7],
                                                          op=self.vs_signals[60],
                                                          prices=self.prices[60],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=True,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -3191,21 +3004,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=2,
                                                          own_cash=cash,
                                                          own_amounts=amounts,
                                                          available_cash=cash,
                                                          available_amounts=amounts,
                                                          op=self.vs_signals[61],
                                                          prices=self.prices[61],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=True,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -3222,21 +3029,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=2,
                                                          own_cash=self.vs_res_sb00[95][7],
                                                          own_amounts=self.vs_res_sb00[95][0:7],
                                                          available_cash=self.vs_res_sb00[95][7],
                                                          available_amounts=self.vs_res_sb00[95][0:7],
                                                          op=self.vs_signals[96],
                                                          prices=self.prices[96],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=True,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -3253,21 +3054,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=2,
                                                          own_cash=cash,
                                                          own_amounts=amounts,
                                                          available_cash=cash,
                                                          available_amounts=amounts,
                                                          op=self.vs_signals[97],
                                                          prices=self.prices[97],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=True,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -3279,28 +3074,23 @@
         cash = cash + c_g.sum() + c_s.sum()
         amounts = amounts + a_p + a_s
         self.assertAlmostEqual(cash, self.vs_res_sb00[97][7], 2)
         self.assertTrue(np.allclose(amounts, self.vs_res_sb00[97][0:7]))
 
     def test_loop_step_vs_bs00(self):
         """test loop step of Volume Signal type of signals"""
+        cost_params = get_cost_pamams(self.rate)
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=2,
                                                          own_cash=10000.,
                                                          own_amounts=np.zeros(7, dtype='float'),
                                                          available_cash=10000.,
                                                          available_amounts=np.zeros(7, dtype='float'),
                                                          op=self.vs_signals[0],
                                                          prices=self.prices[0],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=False,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -3317,21 +3107,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=2,
                                                          own_cash=self.vs_res_bs00[2][7],
                                                          own_amounts=self.vs_res_bs00[2][0:7],
                                                          available_cash=self.vs_res_bs00[2][7],
                                                          available_amounts=self.vs_res_bs00[2][0:7],
                                                          op=self.vs_signals[3],
                                                          prices=self.prices[3],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=False,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -3348,21 +3132,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=2,
                                                          own_cash=self.vs_res_bs00[30][7],
                                                          own_amounts=self.vs_res_bs00[30][0:7],
                                                          available_cash=self.vs_res_bs00[30][7],
                                                          available_amounts=self.vs_res_bs00[30][0:7],
                                                          op=self.vs_signals[31],
                                                          prices=self.prices[31],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=False,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -3379,21 +3157,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=2,
                                                          own_cash=self.vs_res_bs00[59][7] + 10000,
                                                          own_amounts=self.vs_res_bs00[59][0:7],
                                                          available_cash=self.vs_res_bs00[59][7] + 10000,
                                                          available_amounts=self.vs_res_bs00[59][0:7],
                                                          op=self.vs_signals[60],
                                                          prices=self.prices[60],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=False,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -3410,21 +3182,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=2,
                                                          own_cash=cash,
                                                          own_amounts=amounts,
                                                          available_cash=cash,
                                                          available_amounts=amounts,
                                                          op=self.vs_signals[61],
                                                          prices=self.prices[61],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=False,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -3441,21 +3207,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=2,
                                                          own_cash=self.vs_res_bs00[95][7],
                                                          own_amounts=self.vs_res_bs00[95][0:7],
                                                          available_cash=self.vs_res_bs00[95][7],
                                                          available_amounts=self.vs_res_bs00[95][0:7],
                                                          op=self.vs_signals[96],
                                                          prices=self.prices[96],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=False,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
@@ -3472,21 +3232,15 @@
         c_g, c_s, a_p, a_s, fee = qt.backtest._loop_step(signal_type=2,
                                                          own_cash=cash,
                                                          own_amounts=amounts,
                                                          available_cash=cash,
                                                          available_amounts=amounts,
                                                          op=self.vs_signals[97],
                                                          prices=self.prices[97],
-                                                         buy_fix=self.rate['buy_fix'],
-                                                         sell_fix=self.rate['sell_fix'],
-                                                         buy_rate=self.rate['buy_rate'],
-                                                         sell_rate=self.rate['sell_rate'],
-                                                         buy_min=self.rate['buy_min'],
-                                                         sell_min=self.rate['sell_min'],
-                                                         slipage=self.rate['slipage'],
+                                                         cost_params=cost_params,
                                                          pt_buy_threshold=0.1,
                                                          pt_sell_threshold=0.1,
                                                          maximize_cash_usage=False,
                                                          long_pos_limit=1.,
                                                          short_pos_limit=-1.,
                                                          allow_sell_short=False,
                                                          moq_buy=0,
```

### Comparing `qteasy-1.1.7/tests/test_operator_and_strategy.py` & `qteasy-1.1.8/tests/test_operator_and_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -2900,18 +2900,19 @@
                               [0.0, 0.0, 0.0],
                               [0.0, 0.0, 0.0],
                               [0.0, 1.0, 0.0],
                               [0.0, 0.0, -1.0],
                               [0.0, 0.0, 0.0],
                               [0.0, 1.0, 0.0]])
 
-        side_by_side_array = np.array([[i, out_line, sig_line]
+        side_by_side_array = [[i, out_line, sig_line]
                                        for
                                        i, out_line, sig_line
-                                       in zip(range(len(output)), output, sigmatrix)])
+                                       in zip(range(len(output)), output, sigmatrix)]
+        # side_by_side_array = np.array(side_by_side_array)
         print(f'output and signal matrix lined up side by side is \n'
               f'{side_by_side_array}')
         self.assertEqual(sigmatrix.shape, output.shape)
         self.assertTrue(np.allclose(np.array(output), sigmatrix))
 
         # test strategy with also reference data
         print(f'\ntest strategy generate with reference_data')
@@ -2989,18 +2990,19 @@
                               [0.0, 0.0, 1.0],
                               [0.0, 0.0, 0.0],
                               [0.0, 1.0, 0.0],
                               [0.0, 0.0, -1.0],
                               [0.0, 1.0, 0.0],
                               [0.0, 1.0, 0.0]])
 
-        side_by_side_array = np.array([[i, out_line == sig_line, out_line, sig_line]
+        side_by_side_array = [[i, out_line == sig_line, out_line, sig_line]
                                        for
                                        i, out_line, sig_line
-                                       in zip(range(len(output)), output, sigmatrix)])
+                                       in zip(range(len(output)), output, sigmatrix)]
+        # side_by_side_array = np.array(side_by_side_array)
         print(f'output and signal matrix lined up side by side is \n'
               f'{side_by_side_array}')
         self.assertEqual(sigmatrix.shape, output.shape)
         self.assertTrue(np.allclose(np.array(output), sigmatrix, equal_nan=True))
 
     def test_factor_sorter(self):
         """Test Factor Sorter 策略, test all built-in strategy parameters"""
```

### Comparing `qteasy-1.1.7/tests/test_qt.py` & `qteasy-1.1.8/tests/test_qt.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,14 +356,17 @@
         qt.configuration(level=4)
         print(f'configuration with level=1, up_to=3\n')
         qt.configuration(level=1, up_to=3)
         print(f'configuration with info=True\n')
         qt.configuration(default=True)
         print(f'configuration with info=True, verbose=True\n')
         qt.configuration(default=True, verbose=True)
+        print(f'configuration with config_key')
+        qt.configuration('mode, time_zone, asset_pool')
+        qt.configuration(['mode', 'time_zone', 'asset_pool'])
 
     def test_run_mode_0(self):
         """测试策略的实时信号生成模式"""
         op = qt.Operator(strategies=['stema'], op_type='stepwise')
         op.set_parameter('stema', pars=(6,))
         qt.QT_CONFIG.mode = 0
         # qt.run(op)
```

### Comparing `qteasy-1.1.7/tests/test_space.py` & `qteasy-1.1.8/tests/test_space.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.7/tests/test_ta_funcs.py` & `qteasy-1.1.8/tests/test_ta_funcs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.7/tests/test_trader.py` & `qteasy-1.1.8/tests/test_trader.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.7/tests/test_trader_shell.py` & `qteasy-1.1.8/tests/test_trader_shell.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # Desc:
 #   Unittest for trader shell properties
 # and commands.
 # ======================================
 
 import unittest
 import time
+import pandas as pd
 
 from qteasy import DataSource, Operator
 from qteasy.trader import Trader, TraderShell
 from qteasy.trading_util import process_account_delivery, process_trade_result, submit_order, update_position
 from qteasy.trade_recording import new_account, read_trade_order_detail, save_parsed_trade_orders
 from qteasy.trade_recording import get_or_create_position, get_position_by_id, get_account
 from qteasy.broker import SimulatorBroker
@@ -51,14 +52,41 @@
 
         # 创建一个操作员
         operator = Operator(strategies=['macd', 'dma'], op_type='step')
         # 创建一个经纪商
         broker = SimulatorBroker()
 
         test_ds.reconnect()
+
+        # 创建测试datasource需要的股票基础数据等数据
+        stock_basic = {
+            'ts_code': ['000001.SZ', '000002.SZ', '000004.SZ', '000005.SZ', '000006.SZ', '000007.SZ'],
+            'symbol': ['000001', '000002', '000004', '000005', '000006', '000007'],
+            'name': ['平安银行', '万科A', '国农科技', '世纪星源', '深振业A', '全新好'],
+            'area': ['深圳', '深圳', '深圳', '深圳', '深圳', '深圳'],
+            'industry': ['银行', '全国地产', '生物制药', '环境保护', '区域地产', '食品'],
+            'full_name': ['平安银行股份有限公司', '万科企业股份有限公司', '国农科技股份有限公司', '世纪星源股份有限公司',
+                          '深圳市振业(集团)股份有限公司', '深圳市全新好股份有限公司'],
+            'enname': ['Ping An Bank Co., Ltd.', 'China Vanke Co., Ltd.',
+                       'China National Agricultural Technology Co., Ltd.', 'Shijixingyuan Co., Ltd.',
+                       'Shenzhen Zhenye(Group) Co., Ltd.', 'Shenzhen Quanxin Hao Co., Ltd.'],
+            'cnspell': ['PAYH', 'WK', 'GNKJ', 'SJXY', 'SZYA', 'SXH'],
+            'market': ['主板', '主板', '主板', '主板', '主板', '主板'],
+            'exchange': ['SZSE', 'SZSE', 'SZSE', 'SZSE', 'SZSE', 'SZSE'],
+            'curr_type': ['CNY', 'CNY', 'CNY', 'CNY', 'CNY', 'CNY'],
+            'list_status': ['L', 'L', 'L', 'L', 'L', 'L'],
+            'list_date': ['19910403', '19910129', '19951027', '19990602', '19921202', '19910809'],
+            'delist_date': ['', '', '', '', '', ''],
+            'is_hs': ['', '', '', '', '', ''],
+        }
+        stock_basic_df = pd.DataFrame(stock_basic)
+        # 创建测试数据源的股票基础数据
+        if not test_ds.table_data_exists('stock_basic'):
+            test_ds.write_table_data(stock_basic_df, 'stock_basic')
+
         # 清空测试数据源中的所有相关表格数据
         for table in ['sys_op_live_accounts', 'sys_op_positions', 'sys_op_trade_orders', 'sys_op_trade_results']:
             if test_ds.table_data_exists(table):
                 test_ds.drop_table_data(table)
 
         # 创建一个ID=1的账户
         new_account('test_user1', 100000, test_ds)
```

### Comparing `qteasy-1.1.7/tests/test_trading.py` & `qteasy-1.1.8/tests/test_trading.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.7/tests/test_tushare.py` & `qteasy-1.1.8/tests/test_tushare.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.7/tests/test_utilityfuncs.py` & `qteasy-1.1.8/tests/test_utilityfuncs.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,16 +165,16 @@
         self.assertFalse(is_market_trade_day(date_holiday))
         self.assertFalse(is_market_trade_day(date_weekend))
         self.assertFalse(is_market_trade_day(date_seems_trade_day))
         self.assertTrue(is_market_trade_day(date_christmas))
         self.assertFalse(is_market_trade_day(date_christmas, exchange='XHKG'))
 
         # raises when date out of range
-        self.assertRaises(ValueError, is_market_trade_day, date_too_early)
-        self.assertRaises(ValueError, is_market_trade_day, date_too_late)
+        self.assertRaises(KeyError, is_market_trade_day, date_too_early)
+        self.assertRaises(KeyError, is_market_trade_day, date_too_late)
 
         date_trade = pd.to_datetime('20210401')
         date_holiday = pd.to_datetime('20210102')
         date_weekend = pd.to_datetime('20210424')
 
         self.assertTrue(maybe_trade_day(date_trade))
         self.assertFalse(maybe_trade_day(date_holiday))
@@ -194,17 +194,17 @@
         """ test util func list_truncate()"""
         the_list = [1, 2, 3, 4, 5]
         ls = list_truncate(the_list, 2)
         self.assertEqual(ls[0], [1, 2])
         self.assertEqual(ls[1], [3, 4])
         self.assertEqual(ls[2], [5])
 
-        self.assertRaises(AssertionError, list_truncate, the_list, 0)
-        self.assertRaises(AssertionError, list_truncate, 12, 0)
-        self.assertRaises(AssertionError, list_truncate, 0, the_list)
+        self.assertRaises(ValueError, list_truncate, the_list, 0)
+        self.assertRaises(TypeError, list_truncate, 12, 0)
+        self.assertRaises(TypeError, list_truncate, 0, the_list)
 
     def test_maybe_trade_day(self):
         """ test util function maybe_trade_day()"""
         self.assertTrue(maybe_trade_day('20220104'))
         self.assertTrue(maybe_trade_day('2021-12-31'))
         self.assertTrue(maybe_trade_day(pd.to_datetime('2020/03/06')))
```

### Comparing `qteasy-1.1.7/tests/test_visual.py` & `qteasy-1.1.8/tests/test_visual.py`

 * *Files identical despite different names*

