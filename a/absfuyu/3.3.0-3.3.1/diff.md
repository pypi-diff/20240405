# Comparing `tmp/absfuyu-3.3.0.tar.gz` & `tmp/absfuyu-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absfuyu-3.3.0.tar", last modified: Wed Mar 20 08:03:28 2024, max compression
+gzip compressed data, was "absfuyu-3.3.1.tar", last modified: Fri Apr  5 15:56:03 2024, max compression
```

## Comparing `absfuyu-3.3.0.tar` & `absfuyu-3.3.1.tar`

### file list

```diff
@@ -1,103 +1,102 @@
-drwxrwxrwx   0        0        0        0 2024-03-20 08:03:28.490414 absfuyu-3.3.0/
--rw-rw-rw-   0        0        0     1076 2024-03-15 16:47:51.000000 absfuyu-3.3.0/LICENSE
--rw-rw-rw-   0        0        0      205 2022-06-19 18:27:30.000000 absfuyu-3.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     8136 2024-03-20 08:03:28.490414 absfuyu-3.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2511 2024-03-06 12:24:24.000000 absfuyu-3.3.0/README.md
--rw-rw-rw-   0        0        0     2035 2023-11-30 15:44:02.000000 absfuyu-3.3.0/extra_requirements.txt
-drwxrwxrwx   0        0        0        0 2024-03-20 08:03:28.290347 absfuyu-3.3.0/images/
--rw-rw-rw-   0        0        0    34015 2022-01-20 09:25:05.000000 absfuyu-3.3.0/images/repository-image-crop.png
--rw-rw-rw-   0        0        0     2332 2023-11-30 04:27:48.000000 absfuyu-3.3.0/pyproject.toml
--rw-rw-rw-   0        0        0      191 2024-03-14 03:10:43.000000 absfuyu-3.3.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-03-20 08:03:28.490414 absfuyu-3.3.0/setup.cfg
--rw-rw-rw-   0        0        0      867 2023-12-01 06:21:18.000000 absfuyu-3.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-20 08:03:28.272970 absfuyu-3.3.0/src/
-drwxrwxrwx   0        0        0        0 2024-03-20 08:03:28.307015 absfuyu-3.3.0/src/absfuyu/
--rw-rw-rw-   0        0        0      838 2023-11-30 09:16:39.000000 absfuyu-3.3.0/src/absfuyu/__init__.py
--rw-rw-rw-   0        0        0     6514 2023-11-24 18:11:40.000000 absfuyu-3.3.0/src/absfuyu/__main__.py
-drwxrwxrwx   0        0        0        0 2024-03-20 08:03:28.356235 absfuyu-3.3.0/src/absfuyu/config/
--rw-rw-rw-   0        0        0     9270 2024-03-20 07:07:45.000000 absfuyu-3.3.0/src/absfuyu/config/__init__.py
--rw-rw-rw-   0        0        0      791 2024-03-20 08:03:14.000000 absfuyu-3.3.0/src/absfuyu/config/config.json
--rw-rw-rw-   0        0        0     2713 2024-03-20 07:07:44.000000 absfuyu-3.3.0/src/absfuyu/core.py
--rw-rw-rw-   0        0        0      778 2023-11-26 06:43:22.000000 absfuyu-3.3.0/src/absfuyu/everything.py
-drwxrwxrwx   0        0        0        0 2024-03-20 08:03:28.356991 absfuyu-3.3.0/src/absfuyu/extensions/
--rw-rw-rw-   0        0        0      146 2023-11-24 18:02:41.000000 absfuyu-3.3.0/src/absfuyu/extensions/__init__.py
--rw-rw-rw-   0        0        0     5303 2024-03-20 07:07:44.000000 absfuyu-3.3.0/src/absfuyu/extensions/beautiful.py
-drwxrwxrwx   0        0        0        0 2024-03-20 08:03:28.373549 absfuyu-3.3.0/src/absfuyu/extensions/dev/
--rw-rw-rw-   0        0        0     6422 2024-03-20 07:07:45.000000 absfuyu-3.3.0/src/absfuyu/extensions/dev/__init__.py
--rw-rw-rw-   0        0        0     1794 2023-12-01 10:48:27.000000 absfuyu-3.3.0/src/absfuyu/extensions/dev/password_hash.py
--rw-rw-rw-   0        0        0     6796 2023-11-30 08:56:15.000000 absfuyu-3.3.0/src/absfuyu/extensions/dev/passwordlib.py
--rw-rw-rw-   0        0        0     2215 2023-12-01 10:48:27.000000 absfuyu-3.3.0/src/absfuyu/extensions/dev/pkglib.py
--rw-rw-rw-   0        0        0     1561 2023-12-01 10:48:27.000000 absfuyu-3.3.0/src/absfuyu/extensions/dev/project_starter.py
--rw-rw-rw-   0        0        0      132 2023-12-01 10:48:27.000000 absfuyu-3.3.0/src/absfuyu/extensions/dev/shutdownizer.py
-drwxrwxrwx   0        0        0        0 2024-03-20 08:03:28.373549 absfuyu-3.3.0/src/absfuyu/extensions/extra/
--rw-rw-rw-   0        0        0      554 2024-03-20 07:07:44.000000 absfuyu-3.3.0/src/absfuyu/extensions/extra/__init__.py
--rw-rw-rw-   0        0        0    31268 2024-03-20 07:46:38.000000 absfuyu-3.3.0/src/absfuyu/extensions/extra/data_analysis.py
-drwxrwxrwx   0        0        0        0 2024-03-20 08:03:28.385311 absfuyu-3.3.0/src/absfuyu/fun/
--rw-rw-rw-   0        0        0     9447 2024-03-20 07:07:45.000000 absfuyu-3.3.0/src/absfuyu/fun/WGS.py
--rw-rw-rw-   0        0        0     6249 2023-11-27 09:55:54.000000 absfuyu-3.3.0/src/absfuyu/fun/__init__.py
--rw-rw-rw-   0        0        0     2554 2024-01-01 10:57:12.000000 absfuyu-3.3.0/src/absfuyu/fun/tarot.py
-drwxrwxrwx   0        0        0        0 2024-03-20 08:03:28.396591 absfuyu-3.3.0/src/absfuyu/game/
--rw-rw-rw-   0        0        0     4536 2024-03-20 07:07:44.000000 absfuyu-3.3.0/src/absfuyu/game/__init__.py
--rw-rw-rw-   0        0        0    10450 2024-03-20 07:25:26.000000 absfuyu-3.3.0/src/absfuyu/game/sudoku.py
--rw-rw-rw-   0        0        0    15278 2024-03-20 07:25:33.000000 absfuyu-3.3.0/src/absfuyu/game/tictactoe.py
--rw-rw-rw-   0        0        0     9645 2024-03-20 07:07:45.000000 absfuyu-3.3.0/src/absfuyu/game/tictactoe2.py
--rw-rw-rw-   0        0        0   101133 2024-03-20 07:25:33.000000 absfuyu-3.3.0/src/absfuyu/game/wordle.py
-drwxrwxrwx   0        0        0        0 2024-03-20 08:03:28.407247 absfuyu-3.3.0/src/absfuyu/general/
--rw-rw-rw-   0        0        0     2412 2024-03-20 07:07:44.000000 absfuyu-3.3.0/src/absfuyu/general/__init__.py
--rw-rw-rw-   0        0        0    17375 2023-11-27 08:21:56.000000 absfuyu-3.3.0/src/absfuyu/general/content.py
--rw-rw-rw-   0        0        0    48494 2024-03-20 08:01:40.000000 absfuyu-3.3.0/src/absfuyu/general/data_extension.py
--rw-rw-rw-   0        0        0     9547 2024-03-20 07:07:45.000000 absfuyu-3.3.0/src/absfuyu/general/generator.py
--rw-rw-rw-   0        0        0     9486 2024-03-20 07:07:45.000000 absfuyu-3.3.0/src/absfuyu/general/human.py
--rw-rw-rw-   0        0        0    12883 2024-03-20 07:25:33.000000 absfuyu-3.3.0/src/absfuyu/logger.py
-drwxrwxrwx   0        0        0        0 2024-03-20 08:03:28.407247 absfuyu-3.3.0/src/absfuyu/pkg_data/
--rw-rw-rw-   0        0        0     4929 2024-03-20 07:25:33.000000 absfuyu-3.3.0/src/absfuyu/pkg_data/__init__.py
--rw-rw-rw-   0        0        0     4655 2023-11-27 09:32:17.000000 absfuyu-3.3.0/src/absfuyu/pkg_data/chemistry.pkl
--rw-rw-rw-   0        0        0    56195 2023-11-27 09:45:45.000000 absfuyu-3.3.0/src/absfuyu/pkg_data/tarot.pkl
--rw-rw-rw-   0        0        0     6821 2024-03-20 07:01:48.000000 absfuyu-3.3.0/src/absfuyu/sort.py
-drwxrwxrwx   0        0        0        0 2024-03-20 08:03:28.423669 absfuyu-3.3.0/src/absfuyu/tools/
--rw-rw-rw-   0        0        0      143 2023-11-24 16:16:41.000000 absfuyu-3.3.0/src/absfuyu/tools/__init__.py
--rw-rw-rw-   0        0        0     9737 2024-03-20 07:25:33.000000 absfuyu-3.3.0/src/absfuyu/tools/converter.py
--rw-rw-rw-   0        0        0     7413 2024-03-20 07:25:33.000000 absfuyu-3.3.0/src/absfuyu/tools/keygen.py
--rw-rw-rw-   0        0        0     8582 2024-03-20 07:07:45.000000 absfuyu-3.3.0/src/absfuyu/tools/obfuscator.py
--rw-rw-rw-   0        0        0     5187 2024-03-20 07:25:33.000000 absfuyu-3.3.0/src/absfuyu/tools/stats.py
--rw-rw-rw-   0        0        0     1356 2023-11-24 18:02:41.000000 absfuyu-3.3.0/src/absfuyu/tools/web.py
-drwxrwxrwx   0        0        0        0 2024-03-20 08:03:28.440531 absfuyu-3.3.0/src/absfuyu/util/
--rw-rw-rw-   0        0        0     3980 2024-03-20 07:25:33.000000 absfuyu-3.3.0/src/absfuyu/util/__init__.py
--rw-rw-rw-   0        0        0     4075 2024-03-20 07:07:45.000000 absfuyu-3.3.0/src/absfuyu/util/api.py
--rw-rw-rw-   0        0        0     2676 2024-03-20 07:22:29.000000 absfuyu-3.3.0/src/absfuyu/util/json_method.py
--rw-rw-rw-   0        0        0    13839 2023-11-24 18:02:41.000000 absfuyu-3.3.0/src/absfuyu/util/lunar.py
--rw-rw-rw-   0        0        0    21224 2024-03-20 07:47:18.000000 absfuyu-3.3.0/src/absfuyu/util/path.py
--rw-rw-rw-   0        0        0    10830 2024-03-20 07:07:45.000000 absfuyu-3.3.0/src/absfuyu/util/performance.py
--rw-rw-rw-   0        0        0     1561 2024-03-20 07:07:45.000000 absfuyu-3.3.0/src/absfuyu/util/pkl.py
--rw-rw-rw-   0        0        0     2529 2024-03-20 07:25:33.000000 absfuyu-3.3.0/src/absfuyu/util/zipped.py
--rw-rw-rw-   0        0        0    14647 2024-03-20 07:07:45.000000 absfuyu-3.3.0/src/absfuyu/version.py
-drwxrwxrwx   0        0        0        0 2024-03-20 08:03:28.486568 absfuyu-3.3.0/src/absfuyu.egg-info/
--rw-rw-rw-   0        0        0     8136 2024-03-20 08:03:28.000000 absfuyu-3.3.0/src/absfuyu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2361 2024-03-20 08:03:28.000000 absfuyu-3.3.0/src/absfuyu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-20 08:03:28.000000 absfuyu-3.3.0/src/absfuyu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-03-20 08:03:28.000000 absfuyu-3.3.0/src/absfuyu.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      888 2024-03-20 08:03:28.000000 absfuyu-3.3.0/src/absfuyu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-20 08:03:28.000000 absfuyu-3.3.0/src/absfuyu.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-20 08:03:28.484569 absfuyu-3.3.0/tests/
--rw-rw-rw-   0        0        0     1356 2024-03-20 07:58:46.000000 absfuyu-3.3.0/tests/test_DictExt.py
--rw-rw-rw-   0        0        0     3823 2024-03-14 18:28:46.000000 absfuyu-3.3.0/tests/test_IntNumber.py
--rw-rw-rw-   0        0        0     2706 2023-12-25 08:17:30.000000 absfuyu-3.3.0/tests/test_ListExt.py
--rw-rw-rw-   0        0        0     4364 2024-03-20 07:42:12.000000 absfuyu-3.3.0/tests/test_Text.py
--rw-rw-rw-   0        0        0      634 2023-12-01 06:21:18.000000 absfuyu-3.3.0/tests/test_api.py
--rw-rw-rw-   0        0        0      115 2023-12-01 06:21:18.000000 absfuyu-3.3.0/tests/test_beautiful.py
--rw-rw-rw-   0        0        0     1559 2024-03-14 07:26:48.000000 absfuyu-3.3.0/tests/test_config.py
--rw-rw-rw-   0        0        0     1401 2023-12-01 06:21:18.000000 absfuyu-3.3.0/tests/test_converter.py
--rw-rw-rw-   0        0        0     4650 2024-03-14 04:06:46.000000 absfuyu-3.3.0/tests/test_data_analysis.py
--rw-rw-rw-   0        0        0     3306 2024-03-14 07:14:27.000000 absfuyu-3.3.0/tests/test_everything.py
--rw-rw-rw-   0        0        0      293 2023-12-01 06:21:18.000000 absfuyu-3.3.0/tests/test_extensions.py
--rw-rw-rw-   0        0        0      590 2023-12-01 06:21:18.000000 absfuyu-3.3.0/tests/test_fun.py
--rw-rw-rw-   0        0        0     3745 2024-03-05 18:25:35.000000 absfuyu-3.3.0/tests/test_generator.py
--rw-rw-rw-   0        0        0      501 2023-12-01 06:21:18.000000 absfuyu-3.3.0/tests/test_json_method.py
--rw-rw-rw-   0        0        0      906 2023-12-01 06:21:18.000000 absfuyu-3.3.0/tests/test_logger.py
--rw-rw-rw-   0        0        0      692 2023-12-01 06:21:18.000000 absfuyu-3.3.0/tests/test_obfuscator.py
--rw-rw-rw-   0        0        0     1536 2023-12-01 06:21:18.000000 absfuyu-3.3.0/tests/test_passwordlib.py
--rw-rw-rw-   0        0        0      524 2023-12-01 06:21:18.000000 absfuyu-3.3.0/tests/test_path.py
--rw-rw-rw-   0        0        0      374 2023-12-01 06:21:18.000000 absfuyu-3.3.0/tests/test_pkg_data.py
--rw-rw-rw-   0        0        0      398 2023-12-01 06:21:18.000000 absfuyu-3.3.0/tests/test_tarot.py
--rw-rw-rw-   0        0        0     1143 2023-12-01 06:21:18.000000 absfuyu-3.3.0/tests/test_util.py
--rw-rw-rw-   0        0        0     8327 2023-11-24 16:26:18.000000 absfuyu-3.3.0/tests/test_version.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:56:03.719410 absfuyu-3.3.1/
+-rw-rw-rw-   0        0        0     1076 2024-03-15 16:47:51.000000 absfuyu-3.3.1/LICENSE
+-rw-rw-rw-   0        0        0      205 2022-06-19 18:27:30.000000 absfuyu-3.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6585 2024-04-05 15:56:03.716410 absfuyu-3.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2645 2024-04-05 15:51:45.000000 absfuyu-3.3.1/README.md
+-rw-rw-rw-   0        0        0     2068 2024-04-05 15:13:57.000000 absfuyu-3.3.1/extra_requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 15:56:03.524373 absfuyu-3.3.1/images/
+-rw-rw-rw-   0        0        0    34015 2022-01-20 09:25:05.000000 absfuyu-3.3.1/images/repository-image-crop.png
+-rw-rw-rw-   0        0        0     2895 2024-04-05 15:35:36.000000 absfuyu-3.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0      215 2024-04-05 15:13:57.000000 absfuyu-3.3.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 15:56:03.719410 absfuyu-3.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      867 2023-12-01 06:21:18.000000 absfuyu-3.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:56:03.495375 absfuyu-3.3.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 15:56:03.538373 absfuyu-3.3.1/src/absfuyu/
+-rw-rw-rw-   0        0        0      687 2024-04-05 15:30:08.000000 absfuyu-3.3.1/src/absfuyu/__init__.py
+-rw-rw-rw-   0        0        0     5953 2024-04-05 15:27:32.000000 absfuyu-3.3.1/src/absfuyu/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:56:03.576888 absfuyu-3.3.1/src/absfuyu/config/
+-rw-rw-rw-   0        0        0     9649 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/config/__init__.py
+-rw-rw-rw-   0        0        0      791 2024-04-05 15:55:46.000000 absfuyu-3.3.1/src/absfuyu/config/config.json
+-rw-rw-rw-   0        0        0     2367 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/core.py
+-rw-rw-rw-   0        0        0      778 2023-11-26 06:43:22.000000 absfuyu-3.3.1/src/absfuyu/everything.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:56:03.580887 absfuyu-3.3.1/src/absfuyu/extensions/
+-rw-rw-rw-   0        0        0      146 2023-11-24 18:02:41.000000 absfuyu-3.3.1/src/absfuyu/extensions/__init__.py
+-rw-rw-rw-   0        0        0     5319 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/extensions/beautiful.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:56:03.591896 absfuyu-3.3.1/src/absfuyu/extensions/dev/
+-rw-rw-rw-   0        0        0     6516 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/extensions/dev/__init__.py
+-rw-rw-rw-   0        0        0     1808 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/extensions/dev/password_hash.py
+-rw-rw-rw-   0        0        0     6812 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/extensions/dev/passwordlib.py
+-rw-rw-rw-   0        0        0     1577 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/extensions/dev/project_starter.py
+-rw-rw-rw-   0        0        0     4011 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/extensions/dev/shutdownizer.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:56:03.595889 absfuyu-3.3.1/src/absfuyu/extensions/extra/
+-rw-rw-rw-   0        0        0      554 2024-03-20 07:07:44.000000 absfuyu-3.3.1/src/absfuyu/extensions/extra/__init__.py
+-rw-rw-rw-   0        0        0    31699 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/extensions/extra/data_analysis.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:56:03.601889 absfuyu-3.3.1/src/absfuyu/fun/
+-rw-rw-rw-   0        0        0     9447 2024-04-05 14:43:40.000000 absfuyu-3.3.1/src/absfuyu/fun/WGS.py
+-rw-rw-rw-   0        0        0     6263 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/fun/__init__.py
+-rw-rw-rw-   0        0        0     2570 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/fun/tarot.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:56:03.612889 absfuyu-3.3.1/src/absfuyu/game/
+-rw-rw-rw-   0        0        0     4552 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/game/__init__.py
+-rw-rw-rw-   0        0        0    10409 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/game/sudoku.py
+-rw-rw-rw-   0        0        0    15311 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/game/tictactoe.py
+-rw-rw-rw-   0        0        0    10084 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/game/tictactoe2.py
+-rw-rw-rw-   0        0        0   101143 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/game/wordle.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:56:03.624412 absfuyu-3.3.1/src/absfuyu/general/
+-rw-rw-rw-   0        0        0     2471 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/general/__init__.py
+-rw-rw-rw-   0        0        0    17431 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/general/content.py
+-rw-rw-rw-   0        0        0    48862 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/general/data_extension.py
+-rw-rw-rw-   0        0        0     9681 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/general/generator.py
+-rw-rw-rw-   0        0        0     9680 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/general/human.py
+-rw-rw-rw-   0        0        0    12906 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:56:03.631411 absfuyu-3.3.1/src/absfuyu/pkg_data/
+-rw-rw-rw-   0        0        0     4929 2024-03-20 07:25:33.000000 absfuyu-3.3.1/src/absfuyu/pkg_data/__init__.py
+-rw-rw-rw-   0        0        0     4655 2023-11-27 09:32:17.000000 absfuyu-3.3.1/src/absfuyu/pkg_data/chemistry.pkl
+-rw-rw-rw-   0        0        0    56195 2023-11-27 09:45:45.000000 absfuyu-3.3.1/src/absfuyu/pkg_data/tarot.pkl
+-rw-rw-rw-   0        0        0     6827 2024-04-05 15:17:46.000000 absfuyu-3.3.1/src/absfuyu/sort.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:56:03.646410 absfuyu-3.3.1/src/absfuyu/tools/
+-rw-rw-rw-   0        0        0      143 2023-11-24 16:16:41.000000 absfuyu-3.3.1/src/absfuyu/tools/__init__.py
+-rw-rw-rw-   0        0        0     9925 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/tools/converter.py
+-rw-rw-rw-   0        0        0     7437 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/tools/keygen.py
+-rw-rw-rw-   0        0        0     8666 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/tools/obfuscator.py
+-rw-rw-rw-   0        0        0     5197 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/tools/stats.py
+-rw-rw-rw-   0        0        0     1382 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/tools/web.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:56:03.664408 absfuyu-3.3.1/src/absfuyu/util/
+-rw-rw-rw-   0        0        0     3901 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/util/__init__.py
+-rw-rw-rw-   0        0        0     4427 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/util/api.py
+-rw-rw-rw-   0        0        0     2721 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/util/json_method.py
+-rw-rw-rw-   0        0        0    13797 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/util/lunar.py
+-rw-rw-rw-   0        0        0    15565 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/util/path.py
+-rw-rw-rw-   0        0        0     9157 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/util/performance.py
+-rw-rw-rw-   0        0        0     1561 2024-03-20 07:07:45.000000 absfuyu-3.3.1/src/absfuyu/util/pkl.py
+-rw-rw-rw-   0        0        0     2531 2024-04-05 15:13:57.000000 absfuyu-3.3.1/src/absfuyu/util/zipped.py
+-rw-rw-rw-   0        0        0    14733 2024-04-05 15:26:53.000000 absfuyu-3.3.1/src/absfuyu/version.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:56:03.711410 absfuyu-3.3.1/src/absfuyu.egg-info/
+-rw-rw-rw-   0        0        0     6585 2024-04-05 15:56:03.000000 absfuyu-3.3.1/src/absfuyu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2324 2024-04-05 15:56:03.000000 absfuyu-3.3.1/src/absfuyu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 15:56:03.000000 absfuyu-3.3.1/src/absfuyu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-04-05 15:56:03.000000 absfuyu-3.3.1/src/absfuyu.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      751 2024-04-05 15:56:03.000000 absfuyu-3.3.1/src/absfuyu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 15:56:03.000000 absfuyu-3.3.1/src/absfuyu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 15:56:03.707411 absfuyu-3.3.1/tests/
+-rw-rw-rw-   0        0        0     1435 2024-03-22 11:16:55.000000 absfuyu-3.3.1/tests/test_DictExt.py
+-rw-rw-rw-   0        0        0     4518 2024-03-22 13:06:56.000000 absfuyu-3.3.1/tests/test_IntNumber.py
+-rw-rw-rw-   0        0        0     3362 2024-03-22 11:24:39.000000 absfuyu-3.3.1/tests/test_ListExt.py
+-rw-rw-rw-   0        0        0     5534 2024-03-22 13:37:44.000000 absfuyu-3.3.1/tests/test_Text.py
+-rw-rw-rw-   0        0        0      941 2024-04-05 15:38:59.000000 absfuyu-3.3.1/tests/test_api.py
+-rw-rw-rw-   0        0        0      115 2023-12-01 06:21:18.000000 absfuyu-3.3.1/tests/test_beautiful.py
+-rw-rw-rw-   0        0        0     1533 2024-03-22 10:56:25.000000 absfuyu-3.3.1/tests/test_config.py
+-rw-rw-rw-   0        0        0     1484 2024-03-22 11:09:09.000000 absfuyu-3.3.1/tests/test_converter.py
+-rw-rw-rw-   0        0        0     4650 2024-04-04 18:52:14.000000 absfuyu-3.3.1/tests/test_data_analysis.py
+-rw-rw-rw-   0        0        0     3401 2024-04-05 15:13:57.000000 absfuyu-3.3.1/tests/test_everything.py
+-rw-rw-rw-   0        0        0      293 2023-12-01 06:21:18.000000 absfuyu-3.3.1/tests/test_extensions.py
+-rw-rw-rw-   0        0        0      590 2023-12-01 06:21:18.000000 absfuyu-3.3.1/tests/test_fun.py
+-rw-rw-rw-   0        0        0     3554 2024-03-22 13:49:37.000000 absfuyu-3.3.1/tests/test_generator.py
+-rw-rw-rw-   0        0        0      501 2023-12-01 06:21:18.000000 absfuyu-3.3.1/tests/test_json_method.py
+-rw-rw-rw-   0        0        0      906 2023-12-01 06:21:18.000000 absfuyu-3.3.1/tests/test_logger.py
+-rw-rw-rw-   0        0        0      692 2023-12-01 06:21:18.000000 absfuyu-3.3.1/tests/test_obfuscator.py
+-rw-rw-rw-   0        0        0     1536 2023-12-01 06:21:18.000000 absfuyu-3.3.1/tests/test_passwordlib.py
+-rw-rw-rw-   0        0        0      524 2023-12-01 06:21:18.000000 absfuyu-3.3.1/tests/test_path.py
+-rw-rw-rw-   0        0        0      374 2023-12-01 06:21:18.000000 absfuyu-3.3.1/tests/test_pkg_data.py
+-rw-rw-rw-   0        0        0      398 2023-12-01 06:21:18.000000 absfuyu-3.3.1/tests/test_tarot.py
+-rw-rw-rw-   0        0        0     1143 2023-12-01 06:21:18.000000 absfuyu-3.3.1/tests/test_util.py
+-rw-rw-rw-   0        0        0     3271 2024-03-22 10:50:19.000000 absfuyu-3.3.1/tests/test_version.py
```

### Comparing `absfuyu-3.3.0/LICENSE` & `absfuyu-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `absfuyu-3.3.0/PKG-INFO` & `absfuyu-3.3.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,13 @@
 Metadata-Version: 2.1
 Name: absfuyu
-Version: 3.3.0
+Version: 3.3.1
 Summary: A small collection of code
 Author: somewhatcold (AbsoluteWinter)
 License: MIT License
-        
-        Copyright (c) 2022-2024 AbsoluteWinter
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
 Project-URL: Homepage, https://github.com/AbsoluteWinter/absfuyu-public
 Project-URL: Documentation, https://absolutewinter.github.io/absfuyu
 Project-URL: Repository, https://github.com/AbsoluteWinter/absfuyu-public
 Project-URL: Issues, https://github.com/AbsoluteWinter/absfuyu-public/issues
 Keywords: utilities
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -46,101 +25,93 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bs4
+Requires-Dist: click>=8.0.0
+Requires-Dist: colorama
 Requires-Dist: Deprecated
+Requires-Dist: importlib_resources; python_version < "3.10"
 Requires-Dist: python-dateutil
 Requires-Dist: requests
-Requires-Dist: unidecode
 Requires-Dist: tomli>=1.1.0; python_version < "3.11"
 Requires-Dist: typing_extensions>=4.0.1; python_version < "3.11"
-Requires-Dist: importlib_resources; python_version < "3.10"
-Provides-Extra: full
-Requires-Dist: pandas; extra == "full"
-Requires-Dist: rich; extra == "full"
-Requires-Dist: click>=8.0.0; extra == "full"
-Requires-Dist: numpy; extra == "full"
-Requires-Dist: absfuyu-res; extra == "full"
-Requires-Dist: colorama>=0.4; extra == "full"
+Requires-Dist: unidecode
 Provides-Extra: res
 Requires-Dist: absfuyu-res; extra == "res"
 Provides-Extra: absfuyu-res
 Requires-Dist: absfuyu-res; extra == "absfuyu-res"
-Provides-Extra: rich
-Requires-Dist: rich; extra == "rich"
+Provides-Extra: full
+Requires-Dist: absfuyu-res; extra == "full"
+Requires-Dist: numpy; extra == "full"
+Requires-Dist: rich; extra == "full"
+Requires-Dist: pandas; extra == "full"
 Provides-Extra: beautiful
 Requires-Dist: rich; extra == "beautiful"
 Provides-Extra: dev
+Requires-Dist: sphinx>=7.0.0; extra == "dev"
+Requires-Dist: twine>=3.7.1; extra == "dev"
 Requires-Dist: rich; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
 Requires-Dist: sphinx_rtd_theme; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: black; extra == "dev"
-Requires-Dist: click>=8.0.0; extra == "dev"
-Requires-Dist: coverage; extra == "dev"
-Requires-Dist: twine>=3.7.1; extra == "dev"
-Requires-Dist: sphinx>=7.0.0; extra == "dev"
-Requires-Dist: colorama>=0.4; extra == "dev"
-Requires-Dist: build; extra == "dev"
-Requires-Dist: pytest>=6.2.5; extra == "dev"
+Requires-Dist: pytest>=7.0.0; extra == "dev"
+Provides-Extra: rich
+Requires-Dist: rich; extra == "rich"
+Provides-Extra: numpy
+Requires-Dist: numpy; extra == "numpy"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
-Requires-Dist: colorama>=0.4; extra == "extra"
-Requires-Dist: click>=8.0.0; extra == "extra"
 Requires-Dist: numpy; extra == "extra"
-Provides-Extra: click
-Requires-Dist: click>=8.0.0; extra == "click"
-Provides-Extra: cli
-Requires-Dist: colorama>=0.4; extra == "cli"
-Requires-Dist: click>=8.0.0; extra == "cli"
-Provides-Extra: colorama
-Requires-Dist: colorama>=0.4; extra == "colorama"
-Provides-Extra: numpy
-Requires-Dist: numpy; extra == "numpy"
 Provides-Extra: pandas
 Requires-Dist: pandas; extra == "pandas"
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Provides-Extra: black
 Requires-Dist: black; extra == "black"
-Provides-Extra: coverage
-Requires-Dist: coverage; extra == "coverage"
 Provides-Extra: twine
 Requires-Dist: twine>=3.7.1; extra == "twine"
 Provides-Extra: pytest
-Requires-Dist: pytest>=6.2.5; extra == "pytest"
+Requires-Dist: pytest>=7.0.0; extra == "pytest"
+Provides-Extra: pytest-cov
+Requires-Dist: pytest-cov; extra == "pytest-cov"
 Provides-Extra: sphinx
 Requires-Dist: sphinx>=7.0.0; extra == "sphinx"
 Provides-Extra: sphinx-rtd-theme
 Requires-Dist: sphinx_rtd_theme; extra == "sphinx-rtd-theme"
+Provides-Extra: mypy
+Requires-Dist: mypy; extra == "mypy"
 Provides-Extra: all
-Requires-Dist: pandas; extra == "all"
-Requires-Dist: colorama>=0.4; extra == "all"
+Requires-Dist: numpy; extra == "all"
+Requires-Dist: sphinx>=7.0.0; extra == "all"
+Requires-Dist: absfuyu-res; extra == "all"
+Requires-Dist: twine>=3.7.1; extra == "all"
 Requires-Dist: rich; extra == "all"
+Requires-Dist: build; extra == "all"
+Requires-Dist: mypy; extra == "all"
+Requires-Dist: pytest>=7.0.0; extra == "all"
+Requires-Dist: pandas; extra == "all"
 Requires-Dist: sphinx_rtd_theme; extra == "all"
 Requires-Dist: black; extra == "all"
-Requires-Dist: click>=8.0.0; extra == "all"
-Requires-Dist: coverage; extra == "all"
-Requires-Dist: twine>=3.7.1; extra == "all"
-Requires-Dist: absfuyu-res; extra == "all"
-Requires-Dist: sphinx>=7.0.0; extra == "all"
-Requires-Dist: numpy; extra == "all"
-Requires-Dist: build; extra == "all"
-Requires-Dist: pytest>=6.2.5; extra == "all"
+Requires-Dist: pytest-cov; extra == "all"
 
 <div align="center">
 	<h1 align="center">
 		<img src="https://github.com/AbsoluteWinter/AbsoluteWinter.github.io/blob/main/absfuyu/images/repository-image-crop.png?raw=true" alt="absfuyu"/>
 	</h1>
 	<p align="center">
-		<a href="https://pypi.org/project/absfuyu/"><img src="https://img.shields.io/pypi/pyversions/absfuyu?style=flat-square" alt="PyPI Supported Versions"/></a>
-		<a href="https://pypi.org/project/absfuyu/"><img src="https://img.shields.io/pypi/dm/absfuyu?style=flat-square" alt="pypi"/></a>
-		<a href="https://pypi.org/project/absfuyu/"><img src="https://img.shields.io/pypi/v/absfuyu?style=flat-square" /></a>
-		<a><img src="https://img.shields.io/badge/license-MIT-blue?style=flat-square" /></a>
+		<a href="https://pypi.org/project/absfuyu/"><img src="https://img.shields.io/pypi/pyversions/absfuyu?style=flat-square&logo=python" alt="PyPI Supported Versions"/></a>
+		<a href="https://pypi.org/project/absfuyu/"><img src="https://img.shields.io/pypi/dm/absfuyu?style=flat-square&color=blue" alt="pypi"/></a>
+		<a href="https://pypi.org/project/absfuyu/"><img src="https://img.shields.io/pypi/v/absfuyu?style=flat-square&logo=pypi" /></a>
+		<a><img src="https://img.shields.io/badge/style-black-blue?style=flat-square"/></a>
+		<a><img src="https://img.shields.io/pypi/l/absfuyu?style=flat-square&logo=github&color=blue"/></a>
 	</p>
 </div>
 
 
 ---
 
 ## **SUMMARY:**
```

### Comparing `absfuyu-3.3.0/README.md` & `absfuyu-3.3.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 <div align="center">
 	<h1 align="center">
 		<img src="https://github.com/AbsoluteWinter/AbsoluteWinter.github.io/blob/main/absfuyu/images/repository-image-crop.png?raw=true" alt="absfuyu"/>
 	</h1>
 	<p align="center">
-		<a href="https://pypi.org/project/absfuyu/"><img src="https://img.shields.io/pypi/pyversions/absfuyu?style=flat-square" alt="PyPI Supported Versions"/></a>
-		<a href="https://pypi.org/project/absfuyu/"><img src="https://img.shields.io/pypi/dm/absfuyu?style=flat-square" alt="pypi"/></a>
-		<a href="https://pypi.org/project/absfuyu/"><img src="https://img.shields.io/pypi/v/absfuyu?style=flat-square" /></a>
-		<a><img src="https://img.shields.io/badge/license-MIT-blue?style=flat-square" /></a>
+		<a href="https://pypi.org/project/absfuyu/"><img src="https://img.shields.io/pypi/pyversions/absfuyu?style=flat-square&logo=python" alt="PyPI Supported Versions"/></a>
+		<a href="https://pypi.org/project/absfuyu/"><img src="https://img.shields.io/pypi/dm/absfuyu?style=flat-square&color=blue" alt="pypi"/></a>
+		<a href="https://pypi.org/project/absfuyu/"><img src="https://img.shields.io/pypi/v/absfuyu?style=flat-square&logo=pypi" /></a>
+		<a><img src="https://img.shields.io/badge/style-black-blue?style=flat-square"/></a>
+		<a><img src="https://img.shields.io/pypi/l/absfuyu?style=flat-square&logo=github&color=blue"/></a>
 	</p>
 </div>
 
 
 ---
 
 ## **SUMMARY:**
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
                             ************ [[aabbssffuuyyuu]] ************
         _[_P_y_P_I_ _S_u_p_p_o_r_t_e_d_ _V_e_r_s_i_o_n_s_]_[_p_y_p_i_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/
-     _a_b_s_f_u_y_u_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_][https://img.shields.io/badge/license-MIT-
-                            blue?style=flat-square]
+_a_b_s_f_u_y_u_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_&_l_o_g_o_=_p_y_p_i_][https://img.shields.io/badge/style-black-
+   blue?style=flat-square][https://img.shields.io/pypi/l/absfuyu?style=flat-
+                        square&logo=github&color=blue]
 --- ## **SUMMARY:** *TL;DR: A collection of code* ## **INSTALLATION:** ```bash
 $ pip install -U absfuyu ``` ## **USAGE:** ```python import absfuyu help
 (absfuyu) ``` ## **DOCUMENTATION:** > [here](https://absolutewinter.github.io/
 absfuyu/) ## **DEV SETUP** 1. Create virtual environment ```bash python -m venv
 env ``` Note: Might need to run this in powershell (windows) ```powershell Set-
 ExecutionPolicy -ExecutionPolicy Unrestricted -Scope CurrentUser ``` 2. Install
 all required packages ```bash python -m pip install -e .[all] ``` or ```bash
```

### Comparing `absfuyu-3.3.0/extra_requirements.txt` & `absfuyu-3.3.1/extra_requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -22,36 +22,37 @@
 # autoimport:                 fixers, dev
 # tox>=4.0.0:                 dev
 # matplotlib:                 extra
 
 # Already in requirements.txt
 # ---------------------------------------------------------------
 # bs4:                        tools, dev
+# click>=8.0.0:               cli, dev, extra, full
+# colorama>=0.4:              cli, dev, extra, full
 # requests:                   extra, tools, dev
 # python-dateutil:            extra
 # unidecode:                  extra, dev
 
 # ---------------------------------------------------------------
 absfuyu-res:                res, full
 rich:                       beautiful, dev, full
-click>=8.0.0:               cli, dev, extra, full
-colorama>=0.4:              cli, dev, extra, full
 numpy:                      extra, full
 pandas:                     extra, full
 # scipy:                      extra, full
 build:                      dev
 black:                      dev
-coverage:                   dev
+# coverage:                   dev
 twine>=3.7.1:               dev
-pytest>=6.2.5:              dev
+pytest>=7.0.0:              dev
+pytest-cov:                 dev
 sphinx>=7.0.0:              dev
 sphinx_rtd_theme:           dev
+mypy:                       dev
 
 # ---------------------------------------------------------------
-# Current tags: all, beautiful, cli, dev, extra, full, res
+# Current tags: all, beautiful, dev, extra, full, res
 # all: Everything
 # beautiful: Beautiful output module
-# cli: Using command in terminal
 # dev: Everything needed to build, dev, check, test the package
 # extra: Extra module
 # full: Full features without dev requirements
 # res: absfuyu resources
```

### Comparing `absfuyu-3.3.0/images/repository-image-crop.png` & `absfuyu-3.3.1/images/repository-image-crop.png`

 * *Files identical despite different names*

### Comparing `absfuyu-3.3.0/pyproject.toml` & `absfuyu-3.3.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # ========== BUILD ==========
 [build-system]
 requires = [
     "setuptools >= 61.0",
-    # "wheel",
-    # "click",
-    # "colorama",
+    "wheel",
+    "click",
+    "colorama",
     # "pytest",
 ]
 build-backend = "setuptools.build_meta"
+# requires = ["hatchling"]
+# build-backend = "hatchling.build"
 
 # ========== PROJECT ==========
 [project]
 name = "absfuyu"
 description = "A small collection of code"
 readme = "README.md"
 requires-python = ">=3.8, <4"
-license = {file = "LICENSE"}
+license = { text = "MIT License" }
 keywords = ["utilities"]
-authors = [
-    {name = "somewhatcold (AbsoluteWinter)"}
-]
+authors = [{ name = "somewhatcold (AbsoluteWinter)" }]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
@@ -34,37 +34,30 @@
     "Natural Language :: English",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
 ]
-dynamic = [
-    "version",
-    "dependencies",
-    "optional-dependencies",
-]
+dynamic = ["version", "dependencies", "optional-dependencies"]
 
 [project.urls]
 Homepage = "https://github.com/AbsoluteWinter/absfuyu-public"
 Documentation = "https://absolutewinter.github.io/absfuyu"
 Repository = "https://github.com/AbsoluteWinter/absfuyu-public"
 Issues = "https://github.com/AbsoluteWinter/absfuyu-public/issues"
 
 # [project.optional-dependencies]
-# cli = ["click>=8.0.0", "colorama>=0.4"]
 # dev = [
 #     "sphinx>=7.0.0",
 #     "sphinx_rtd_theme",
 #     "pytest>=6.2.5",
 #     "twine",
 #     "build",
 #     "tox",
-#     "click>=8.0.0",
-#     "colorama>=0.4"
 # ]
 
 [project.scripts]
 fuyu = "absfuyu.__main__:main"
 
 # ========== TOOL ==========
 [tool.setuptools]
@@ -77,9 +70,35 @@
 "absfuyu.config" = ["*"]
 "absfuyu.pkg_data" = ["*"]
 
 [tool.setuptools.exclude-package-data]
 absfuyu = [".gitattributes", ".gitignore"]
 
 [tool.setuptools.dynamic]
-dependencies = {file = "requirements.txt"}
-version = {attr = "absfuyu.__version__"}
+dependencies = { file = "requirements.txt" }
+version = { attr = "absfuyu.__version__" }
+
+[tool.pytest.ini_options]
+addopts = [
+    "--strict-markers",
+    "--maxfail=1",
+    # "--cov=absfuyu"
+]
+markers = [
+    "test_this: Select desire test to test",
+    "data_extension: Test all data extension classes",
+]
+
+[tool.mypy]
+mypy_path = "src"
+check_untyped_defs = true
+# disallow_any_generics = true
+ignore_missing_imports = true
+no_implicit_optional = true
+show_error_codes = true
+strict_equality = true
+warn_redundant_casts = true
+warn_return_any = true
+warn_unreachable = true
+warn_unused_configs = true
+no_implicit_reexport = true
+# install_types = true  # type: ignore
```

### Comparing `absfuyu-3.3.0/setup.py` & `absfuyu-3.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `absfuyu-3.3.0/src/absfuyu/__init__.py` & `absfuyu-3.3.1/src/absfuyu/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,19 +16,18 @@
 >>> help(absfuyu)
 
 Using in cmd (`absfuyu[cli]` required): 
 ``$ fuyu --help``
 """
 
 
-# Module level
-###########################################################################
 __title__ = "absfuyu"
 __author__ = "AbsoluteWinter"
 __license__ = "MIT License"
+# __version__ = "3.4.0.dev0"
 __all__ = [
     "core",
     "config",
     "everything",
     "extensions",
     "logger",
     "fun",
@@ -38,10 +37,8 @@
     "sort",
     "tools",
     "util",
     "version",
 ]
 
 
-# Library
-###########################################################################
 from .version import __version__
```

### Comparing `absfuyu-3.3.0/src/absfuyu/__main__.py` & `absfuyu-3.3.1/src/absfuyu/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,51 +1,34 @@
 """
 ABSFUYU
 ---
 COMMAND LINE INTERFACE
 
-Version: 2.0.1
-Date updated: 25/11/2023 (dd/mm/yyyy)
+Version: 2.0.2
+Date updated: 05/04/2024 (dd/mm/yyyy)
 """
 
-
 # Library
 ###########################################################################
-from random import choice as __randc
 import subprocess
+from random import choice as __randc
 
-CLI_MODE = False
-try:
-    import click
-    import colorama
-except ImportError:
-    # Auto install absfuyu[cli]
-    from absfuyu.config import ABSFUYU_CONFIG
-
-    if ABSFUYU_CONFIG._get_setting("auto-install-extra").value:
-        __cmd: str = "python -m pip install -U absfuyu[cli]".split()
-        subprocess.run(__cmd)
-    else:
-        raise SystemExit("This feature is in absfuyu[cli] package")
-else:
-    CLI_MODE = True
+import click
+import colorama
 
-from absfuyu.config import ABSFUYU_CONFIG
 from absfuyu import core as __core
 from absfuyu import version as __v
-
+from absfuyu.config import ABSFUYU_CONFIG
+from absfuyu.game import game_escapeLoop, game_RockPaperScissors  # type: ignore
+from absfuyu.game.tictactoe import game_tictactoe  # type: ignore
 
 # Color stuff
 ###########################################################################
-if CLI_MODE:
-    if colorama is not None:
-        colorama.init(autoreset=True)
-        __COLOR = __core.Color
-    else:
-        __COLOR = {"green": "", "blue": "", "red": "", "yellow": "", "reset": ""}
+colorama.init(autoreset=True)
+__COLOR = __core.Color
 
 
 # Main group
 ###########################################################################
 @click.command()
 def welcome():
     """Welcome message"""
@@ -88,15 +71,15 @@
     # Dictionary
     trans = {
         "luckgod": "luckgod-mode",
         "install-extra": "auto-install-extra",
     }  # trans[setting]
 
     if setting is None:
-        click.echo(f"{__COLOR['red']}Invalid setting")
+        click.echo(f"{__COLOR['red']}Invalid setting")  # type: ignore
     else:
         ABSFUYU_CONFIG.toggle_setting(trans[setting])
         out = ABSFUYU_CONFIG._get_setting(trans[setting])
         click.echo(f"{__COLOR['red']}{out}")
     pass
 
 
@@ -164,29 +147,25 @@
     Play game
 
     Game list:
     - esc: Escape loop
     - rps: Rock Paper Scissors
     - ttt: Tic Tac Toe
     """
-    from absfuyu.game import game_escapeLoop, game_RockPaperScissors
-
     if game_name.startswith("random"):
         if __randc([0, 1]) == 0:
             game_escapeLoop()
         else:
             game_RockPaperScissors()
     else:
         if game_name.startswith("esc"):
             game_escapeLoop()
         elif game_name.startswith("rps"):
             game_RockPaperScissors(hard_mode=mode)
         elif game_name.startswith("ttt"):
-            from absfuyu.game.tictactoe import game_tictactoe
-
             if board_style == "None":
                 board_style = None
             elif board_style == "1":
                 board_style = True
             else:
                 board_style = False
             game_tictactoe(size=size, mode=mode, board_game=board_style)
@@ -252,9 +231,8 @@
 main.add_command(version)
 main.add_command(do_group)
 
 
 # Run
 ###########################################################################
 if __name__ == "__main__":
-    if CLI_MODE:
-        main()
+    main()
```

### Comparing `absfuyu-3.3.0/src/absfuyu/config/__init__.py` & `absfuyu-3.3.1/src/absfuyu/config/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """
 Absfuyu: Configuration
 ----------------------
 Package configuration module
 
-Version: 2.0.2
-Date updated: 14/03/2024 (dd/mm/yyyy)
+Version: 2.0.3
+Date updated: 05/04/2024 (dd/mm/yyyy)
 """
 
-
 # Module level
 ###########################################################################
 __all__ = [
     "ABSFUYU_CONFIG",
     "Config",
     # "Setting"
 ]
@@ -21,15 +20,14 @@
 ###########################################################################
 from pathlib import Path
 from typing import Any, Dict, List, Optional, TypedDict, Union
 
 from absfuyu.core import CONFIG_PATH
 from absfuyu.util.json_method import JsonFile
 
-
 # Setting
 ###########################################################################
 _SPACE_REPLACE = "-"  # Replace " " character in setting name
 
 
 # Type hint
 ###########################################################################
@@ -104,21 +102,18 @@
 
     @classmethod
     def from_dict(cls, dict_data: Dict[str, SettingDictFormat]):
         """
         Convert ``dict`` into ``Setting`` (``len==1`` only)
         """
         name: str = list(dict_data.keys())[0]
-        _val: dict = list(dict_data.values())[0]
-        value: Any = _val.get("value")
-        default: Any = _val.get("default")
-        help_: str = _val.get("help")
-        # value: Any = _val["value"]
-        # default: Any = _val["default"]
-        # help_: str = _val["help"]
+        _val: SettingDictFormat = list(dict_data.values())[0]
+        value: Any = _val["value"]
+        default: Any = _val["default"]
+        help_: str = _val["help"]
         return cls(name, value, default, help_)
 
     def reset(self) -> None:
         """
         Reset setting to default value
         (``Setting.value = Setting.default``)
         """
@@ -152,46 +147,44 @@
 
         if name:
             self.name = name
         else:
             self.name = self.config_path.name
 
         # Data
-        self.settings: List[Setting] = None
-        self.version: dict = None
+        self.settings: List[Setting] = None  # type: ignore
+        self.version: VersionDictFormat = None  # type: ignore
         self._fetch_data()  # Load data
 
     def __str__(self) -> str:
         return f"{self.__class__.__name__}({self.config_path.name})"
 
     def __repr__(self) -> str:
         return self.__str__()
 
     # Data prepare and export
     def _fetch_data(self) -> None:
         """Load data from ``self.config_file`` file"""
         data: dict = self.json_engine.load_json()
-        settings: Dict[str, SettingDictFormat] = data.get("setting")
-        self.settings: List[Setting] = [
-            Setting.from_dict({k: v}) for k, v in settings.items()
-        ]
-        self.version: VersionDictFormat = data.get("version")
+        settings: Dict[str, SettingDictFormat] = data.get("setting")  # type: ignore
+        self.settings = [Setting.from_dict({k: v}) for k, v in settings.items()]
+        self.version: VersionDictFormat = data.get("version")  # type: ignore
 
     def _prepare_data(self) -> ConfigFormat:
         """Prepare data to save config"""
         settings = dict()
         for setting in self.settings:
             settings.update(setting.to_dict())
 
         out: ConfigFormat = {"setting": settings, "version": self.version}
         return out
 
     def save(self) -> None:
         """Save config to ``.json`` file"""
-        self.json_engine.update_data(self._prepare_data())
+        self.json_engine.update_data(self._prepare_data())  # type: ignore
         self.json_engine.save_json()
 
     # Setting method
     @property
     def setting_list(self) -> List[str]:
         """List of name of available settings"""
         return [setting.name for setting in self.settings]
@@ -204,15 +197,15 @@
                 if setting.name.startswith(name):
                     return setting
         else:
             raise ValueError(f"Setting list: {self.setting_list}")
 
     def reset_config(self) -> None:
         """Reset all settings to default value"""
-        [setting.reset() for setting in self.settings]
+        [setting.reset() for setting in self.settings]  # type: ignore
         self.save()
 
     def show_settings(self) -> List[Setting]:
         """
         Returns a list of available settings
         (wrapper for ``Config.settings``)
         """
@@ -315,12 +308,26 @@
         self.save()
 
 
 # Init
 ###########################################################################
 ABSFUYU_CONFIG = Config(CONFIG_PATH)
 
+# TODO: Version 3.4: Create a config file [W.I.P]
+# _settings = [
+#     Setting(
+#         "auto-install-extra", False, False, "Automatically install required packages"
+#     ),
+#     Setting("first-run", True, True, "Check if this package has ever been run"),
+#     Setting(
+#         "luckgod-mode",
+#         False,
+#         False,
+#         "A chance that the machine will be randomly shutdown",
+#     ),
+# ]
+
 
 # Run
 ###########################################################################
 if __name__ == "__main__":
     pass
```

### Comparing `absfuyu-3.3.0/src/absfuyu/config/config.json` & `absfuyu-3.3.1/src/absfuyu/config/config.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "{'patch': 1}"}*

```diff
@@ -20,12 +20,12 @@
             "help": "Test",
             "value": false
         }
     },
     "version": {
         "major": 3,
         "minor": 3,
-        "patch": 0,
+        "patch": 1,
         "release_level": "final",
         "serial": 0
     }
 }
```

### Comparing `absfuyu-3.3.0/src/absfuyu/core.py` & `absfuyu-3.3.1/src/absfuyu/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """
 Absfuyu: Core
 -------------
 Contain type hints and other stuffs
 
-Version: 2.1.9
-Date updated: 27/11/2023 (dd/mm/yyyy)
+Version: 2.1.10
+Date updated: 05/04/2024 (dd/mm/yyyy)
 """
 
-
 # Module Package
 ###########################################################################
 __all__ = [
     # module
     "ModulePackage",
     "ModuleList",
     # color
@@ -19,15 +18,15 @@
     "CLITextColor",
     # path
     "CORE_PATH",
     "CONFIG_PATH",
     "DATA_PATH",
 ]
 
-ModulePackage = ["all", "cli", "beautiful", "extra", "res", "full", "dev"]
+ModulePackage = ["all", "beautiful", "extra", "res", "full", "dev"]
 ModuleList = [
     "config",
     "extensions",
     "fun",
     "game",
     "general",
     "pkg_data",
@@ -38,58 +37,42 @@
 ]
 
 
 # Library
 ###########################################################################
 from pathlib import Path
 
+import colorama
+
 # import sys
+# from sys import version_info as _python_version
 
 # if sys.version_info.minor >= 10:
 #     from importlib.resources import files
 # else:
 #     try:
 #         from importlib_resources import files
 #     except:
 #         raise ImportError("Please install importlib-resources")
 
 
-try:
-    import colorama as __colorama
-except ImportError:
-    __colorama = None
-
-
 # Color - colorama
 ###########################################################################
-if __colorama is not None:
-    # __colorama.init(autoreset=True)
-    Color = {
-        "green": __colorama.Fore.LIGHTGREEN_EX,
-        "GREEN": __colorama.Fore.GREEN,
-        "blue": __colorama.Fore.LIGHTCYAN_EX,
-        "BLUE": __colorama.Fore.CYAN,
-        "red": __colorama.Fore.LIGHTRED_EX,
-        "RED": __colorama.Fore.RED,
-        "yellow": __colorama.Fore.LIGHTYELLOW_EX,
-        "YELLOW": __colorama.Fore.YELLOW,
-        "reset": __colorama.Fore.RESET,
-    }
-else:
-    Color = {
-        "green": "",
-        "GREEN": "",
-        "blue": "",
-        "BLUE": "",
-        "red": "",
-        "RED": "",
-        "yellow": "",
-        "YELLOW": "",
-        "reset": "",
-    }
+# colorama.init(autoreset=True)
+Color = {
+    "green": colorama.Fore.LIGHTGREEN_EX,
+    "GREEN": colorama.Fore.GREEN,
+    "blue": colorama.Fore.LIGHTCYAN_EX,
+    "BLUE": colorama.Fore.CYAN,
+    "red": colorama.Fore.LIGHTRED_EX,
+    "RED": colorama.Fore.RED,
+    "yellow": colorama.Fore.LIGHTYELLOW_EX,
+    "YELLOW": colorama.Fore.YELLOW,
+    "reset": colorama.Fore.RESET,
+}
 
 
 class CLITextColor:
     """Color code for text in terminal"""
 
     WHITE = "\x1b[37m"
     BLACK = "\x1b[30m"
```

### Comparing `absfuyu-3.3.0/src/absfuyu/everything.py` & `absfuyu-3.3.1/src/absfuyu/everything.py`

 * *Files identical despite different names*

### Comparing `absfuyu-3.3.0/src/absfuyu/extensions/beautiful.py` & `absfuyu-3.3.1/src/absfuyu/extensions/beautiful.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# type: ignore
 """
 Absfuyu: Beautiful
 ------------------
 A decorator that makes output more beautiful
 
 Version: 1.0.2
 Date updated: 24/11/2023 (dd/mm/yyyy)
```

### Comparing `absfuyu-3.3.0/src/absfuyu/extensions/dev/__init__.py` & `absfuyu-3.3.1/src/absfuyu/extensions/dev/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
+# type: ignore
 """
 Absfuyu: Development
----
-Some stuffs that are not ready to use yet
+--------------------
+Some stuffs that are not ready to use yet.
+Use at your own risk, everything is subject to change
 
 Version: 2.0.0
 Date updated: 23/11/2023 (dd/mm/yyyy)
 """
 
-
 # Module level
 ###########################################################################
 __all__ = [
     "password_check",
     "fib",
 ]
 
 
 # Library
 ###########################################################################
 import base64
+import re
 from collections import deque
 from functools import lru_cache
-import re
-from typing import Dict, TypedDict, Final, List, NamedTuple
+from typing import Dict, Final, List, NamedTuple
 
 
 # PASSWORD CHECKER
 def password_check(password: str) -> bool:
     """
     Verify the strength of 'password'.
     Returns a dict indicating the wrong criteria.
@@ -109,29 +110,30 @@
 
     :param toml_file: Path to ``.toml`` file
     """
     from sys import version_info as _python_version
 
     if _python_version.minor < 11:
         try:
-            import tomli as tomllib
+            import tomli as tomllib  # type: ignore
         except ImportError:
             raise ImportError("Please install tomli python package")
         except:
             raise SystemExit
     else:
         import tomllib
 
     with open(toml_file, "rb") as file:
         toml_data = tomllib.load(file)
         return toml_data
 
 
 def get_sitemap(url: str):
     import re
+
     import requests
 
     class Url(NamedTuple):
         base: str
         extra: str
 
         def __str__(self) -> str:
```

### Comparing `absfuyu-3.3.0/src/absfuyu/extensions/dev/password_hash.py` & `absfuyu-3.3.1/src/absfuyu/extensions/dev/password_hash.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
+# type: ignore
 # Library
 ##############################################################
 import hashlib as __hash
 import os as __os
 from typing import Dict as __Dict
+from typing import NewType as __NewType
 from typing import TypeVar as __TypeVar
 from typing import Union as __Union
-from typing import NewType as __NewType
-
 
 # Define type
 ##############################################################
 Password = __NewType("Password", str)
 Salt = __NewType("Salt", str)
 Key = __NewType("Key", str)
 Salt_V = __NewType("Salt_V", bytes)
```

### Comparing `absfuyu-3.3.0/src/absfuyu/extensions/dev/passwordlib.py` & `absfuyu-3.3.1/src/absfuyu/extensions/dev/passwordlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# type: ignore
 """
 Absfuyu: Passwordlib
 --------------------
 Password library
 
 Version: 1.0.0dev1
 Date updated: 30/11/2023 (dd/mm/yyyy)
@@ -11,21 +12,21 @@
 # Library
 ###########################################################################
 # from collections import namedtuple
 import hashlib
 import os
 import random
 import re
-from typing import List, Dict, Optional, Union
+from typing import Dict, List, Optional, Union
 
 from absfuyu_res import DATA
 
-from absfuyu.logger import logger
 from absfuyu.general.data_extension import DictExt, Text
-from absfuyu.general.generator import Generator, Charset
+from absfuyu.general.generator import Charset, Generator
+from absfuyu.logger import logger
 from absfuyu.util import set_min
 from absfuyu.util.pkl import Pickler
 
 
 # Function
 ###########################################################################
 def password_check(password: str) -> bool:
```

### Comparing `absfuyu-3.3.0/src/absfuyu/extensions/dev/project_starter.py` & `absfuyu-3.3.1/src/absfuyu/extensions/dev/project_starter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# type: ignore
 """
 Absfuyu: Project starter
 ------------------------
 
 Version: 1.0.0dev1
 Date updated: 01/12/2023 (dd/mm/yyyy)
 """
@@ -10,15 +11,15 @@
 # Module level
 ###########################################################################
 __all__ = ["get_parser"]
 
 
 # Library
 ###########################################################################
-from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
+from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser
 from typing import Optional
 
 
 # Function
 ###########################################################################
 def get_parser(
     name: Optional[str] = None,
```

### Comparing `absfuyu-3.3.0/src/absfuyu/extensions/extra/__init__.py` & `absfuyu-3.3.1/src/absfuyu/extensions/extra/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-3.3.0/src/absfuyu/extensions/extra/data_analysis.py` & `absfuyu-3.3.1/src/absfuyu/extensions/extra/data_analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,22 +35,19 @@
 
 # import matplotlib.pyplot as plt
 # from scipy import stats
 # from dateutil.relativedelta import relativedelta
 import numpy as np
 import pandas as pd
 from deprecated import deprecated
-from deprecated.sphinx import (
-    versionadded,
-    versionchanged,
-    deprecated as sphinx_deprecated,
-)
+from deprecated.sphinx import deprecated as sphinx_deprecated
+from deprecated.sphinx import versionadded, versionchanged
 
-from absfuyu.logger import logger
-from absfuyu.util import set_min_max, set_min
+from absfuyu.logger import logger  # type: ignore
+from absfuyu.util import set_min, set_min_max
 
 
 # Function
 ###########################################################################
 @deprecated(reason="Not needed", version="3.1.0")
 @sphinx_deprecated(reason="Not needed", version="3.1.0")
 def summary(data: Union[list, np.ndarray]):  # del this
@@ -97,15 +94,15 @@
                 v.append(fillna)
     return data
 
 
 ## Update 05/10
 
 
-def compare_2_list(*arr: list) -> pd.DataFrame:
+def compare_2_list(*arr) -> pd.DataFrame:
     """
     Compare 2 lists then create DataFrame
     to see which items are missing
 
     Parameters
     ----------
     arr : list
@@ -114,15 +111,15 @@
     Returns
     -------
     DataFrame
         Compare result
     """
     # Setup
     col_name = "list"
-    arr = [sorted(x) for x in arr]  # map(sorted, arr)
+    arr = [sorted(x) for x in arr]  # type: ignore # map(sorted, arr)
 
     # Total array
     tarr = sorted(list(set(chain.from_iterable(arr))))
     # max_len = len(tarr)
 
     # Temp dataset
     temp_dict = {"base": tarr}
@@ -182,39 +179,39 @@
     """
 
     city: str
     region: str
     area: str
 
     @staticmethod
-    def _sample_city_data(size: int = 100):
+    def _sample_city_data(size: int = 100) -> List["CityData"]:
         """
         Generate sample city data (testing purpose)
         """
         sample_range = 10 ** len(str(size))
 
         # Serial list
-        serials = []
+        serials: List[str] = []
         while len(serials) != size:  # Unique serial
             serial = random.randint(0, sample_range - 1)
-            serial = str(serial).rjust(len(str(size)), "0")
-            if serial not in serials:
-                serials.append(serial)
+            serial = str(serial).rjust(len(str(size)), "0")  # type: ignore
+            if serial not in serials:  # type: ignore
+                serials.append(serial)  # type: ignore
 
         ss2 = deque(serials[: int(len(serials) / 2)])  # Cut half for region
         ss2.rotate(random.randrange(1, 5))
-        [ss2.extend(ss2) for _ in range(2)]  # Extend back
+        [ss2.extend(ss2) for _ in range(2)]  # type: ignore # Extend back
 
         ss3 = deque(serials[: int(len(serials) / 4)])  # Cut forth for area
         ss3.rotate(random.randrange(1, 5))
-        [ss3.extend(ss3) for _ in range(4)]  # Extend back
+        [ss3.extend(ss3) for _ in range(4)]  # type: ignore # Extend back
 
         serials = ["city_" + x for x in serials]
-        ss2 = ["region_" + x for x in ss2]
-        ss3 = ["area_" + x for x in ss3]
+        ss2 = ["region_" + x for x in ss2]  # type: ignore
+        ss3 = ["area_" + x for x in ss3]  # type: ignore
 
         ss = list(zip(serials, ss2, ss3))  # Zip back
         out = list(map(CityData._make, ss))
 
         return out
 
 
@@ -269,15 +266,15 @@
             (Default: ``"inner"``)
 
         Returns
         -------
         DataFrame
             Joined DataFrame
         """
-        return self.concat_df(self, join=join)
+        return self.concat_df(self, join=join)  # type: ignore
 
     @staticmethod
     def divide_dataframe(df: pd.DataFrame, by_column: str) -> List[pd.DataFrame]:
         """
         Divide DataFrame into a list of DataFrame
 
         Parameters
@@ -322,32 +319,32 @@
         remove_char: Characters that excluded from attribute name
         """
         self._data = dict_data
 
         if key_as_atrribute:
             # temp = list(map(self._remove_space, self._data.keys()))
             temp = [self._remove_space(x, remove_char) for x in self._data.keys()]
-            [self.__setattr__(k, v) for k, v in zip(temp, self._data.values())]
+            [self.__setattr__(k, v) for k, v in zip(temp, self._data.values())]  # type: ignore
         else:
             temp = [self._remove_space(x, remove_char) for x in self._data.values()]
-            [self.__setattr__(k, v) for k, v in zip(temp, self._data.keys())]
+            [self.__setattr__(k, v) for k, v in zip(temp, self._data.keys())]  # type: ignore
         self._keys = temp
 
     def __str__(self) -> str:
         return f"{self.__class__.__name__}({self._keys})"
 
     def __repr__(self) -> str:
         return self.__str__()
 
     @staticmethod
     def _remove_space(value: str, remove_char: str) -> str:
         """
         Remove special characters and replace space with underscore
         """
-        remove_char = remove_char.split(" ")
+        remove_char = remove_char.split(" ")  # type: ignore
         logger.debug(remove_char)
         for x in remove_char:
             value = value.replace(x, "")
         value = value.replace(" ", "_")
         return value
 
 
@@ -402,23 +399,23 @@
     Marker = _DictToAtrr(MARKER_LIST, key_as_atrribute=False)
     LineStyle = _DictToAtrr(LINE_STYLE_LIST, key_as_atrribute=False)
     Color = _DictToAtrr(COLOR_LIST, key_as_atrribute=False)
 
     @staticmethod
     def all_format_string() -> List[PLTFormatString]:
         fmt_str = [
-            __class__.MARKER_LIST,
-            __class__.LINE_STYLE_LIST,
-            __class__.COLOR_LIST,
+            __class__.MARKER_LIST,  # type: ignore
+            __class__.LINE_STYLE_LIST,  # type: ignore
+            __class__.COLOR_LIST,  # type: ignore
         ]
         return [PLTFormatString._make(x) for x in list(product(*fmt_str))]
 
     @staticmethod
     def get_random(alt: bool = False) -> str:
-        temp = random.choice(__class__.all_format_string())
+        temp = random.choice(__class__.all_format_string())  # type: ignore
         if alt:
             return f"{temp.marker}{temp.line_style}{temp.color}"
         else:
             return f"{temp.color}{temp.marker}{temp.line_style}"
 
 
 # Class - DA
@@ -445,22 +442,22 @@
 
         Returns
         -------
         DataAnalystDataFrame
             Modified DataFrame
         """
         cols = self.columns.to_list()  # List of columns
-        num_of_cols = set_min_max(num_of_cols, min_value=1, max_value=len(cols))
+        num_of_cols = int(set_min_max(num_of_cols, min_value=1, max_value=len(cols)))
         col_index = cols.index(insert_to_col)
         cols = (
             cols[: col_index + 1]
             + cols[-num_of_cols:]
             + cols[col_index + 1 : len(cols) - num_of_cols]
         )
-        self = __class__(self[cols])
+        self = self.__class__(self[cols])
         return self
 
     # Drop a list of column
     def drop_columns(self, columns: List[str]):
         """
         Drop columns in DataFrame
 
@@ -498,15 +495,17 @@
             Modified DataFrame
         """
         # Restrain
         # if num_of_cols < 1:
         #     num_of_cols = 1
         # if num_of_cols > self.shape[1]:
         #     num_of_cols = self.shape[1]
-        num_of_cols = set_min_max(num_of_cols, min_value=1, max_value=self.shape[1])
+        num_of_cols = int(
+            set_min_max(num_of_cols, min_value=1, max_value=self.shape[1])
+        )
 
         # Logic
         for _ in range(num_of_cols):
             self.drop(self.columns[len(self.columns) - 1], axis=1, inplace=True)
         return self
 
     # Add blank column
@@ -530,15 +529,19 @@
         self[column_name] = [fill] * self.shape[0]
         return self
 
     # Modify
     # ================================================================
     # Convert city
     def convert_city(
-        self, city_column: str, city_list: List[CityData] = None, *, mode: str = "ra"
+        self,
+        city_column: str,
+        city_list: List[CityData],
+        *,
+        mode: str = "ra",
     ):
         """
         Get ``region`` and ``area`` of a city
 
         Parameters
         ----------
         city_column : str
@@ -557,19 +560,19 @@
         Returns
         -------
         DataAnalystDataFrame
             Modified DataFrame
         """
 
         # Support function
-        def _convert_city_support(value: str):
+        def _convert_city_support(value: str) -> CityData:
             for x in city_list:
                 if x.city.lower().startswith(value.lower()):
                     return x
-            return CityData(city=value, region=np.nan, area=np.nan)
+            return CityData(city=value, region=np.nan, area=np.nan)  # type: ignore
 
         # Convert
         col_counter = 0
         if mode.find("r") != -1:
             logger.debug("Mode: 'region'")
             self["region"] = self[city_column].apply(
                 lambda x: _convert_city_support(x).region
@@ -817,32 +820,32 @@
             list_of_keep: list = (
                 col_df[destination_column]
                 .head(set_min_max(top - 1, min_value=1, max_value=col_df.shape[0]))
                 .to_list()
             )
             # logger.debug(list_of_keep)
         else:
-            list_of_keep: list = col_df[col_df["percentage"] >= threshold][
+            list_of_keep = col_df[col_df["percentage"] >= threshold][
                 destination_column
             ].to_list()  # values that will not be renamed
         self[f"{destination_column}_filtered"] = self[destination_column].apply(
             lambda x: replace_with if x not in list_of_keep else x
         )
 
         # Return
         return self
 
     # Info
     # ================================================================
     # Total observation
-    @versionadded(version="3.2.0")
     @property
+    @versionadded(version="3.2.0")
     def total_observation(self) -> int:
         """Returns total observation of the DataFrame"""
-        return self.shape[0] * self.shape[1]
+        return self.shape[0] * self.shape[1]  # type: ignore
 
     # Quick info
     @versionadded(version="3.2.0")
     def qinfo(self) -> str:
         """
         Show quick infomation about DataFrame
         """
@@ -970,15 +973,15 @@
 
     # Help
     @staticmethod
     def dadf_help() -> List[str]:
         """
         Show all available method of DataAnalystDataFrame
         """
-        list_of_method = list(set(dir(__class__)) - set(dir(pd.DataFrame)))
+        list_of_method = list(set(dir(__class__)) - set(dir(pd.DataFrame)))  # type: ignore
         return sorted(list_of_method)
 
     # Sample DataFrame
     @classmethod
     def sample_df(cls, size: int = 100):
         """
         Create sample DataFrame
@@ -1010,15 +1013,15 @@
         96  1.296795         255          200            NaN  lwvytego 2014-05-10
         97  1.440746         297          200            5.0  lqsoykun 2010-04-03
         98  0.327702         845          800            NaN  leadkvsy 2005-08-05
         99  0.556720         981          900           36.0  bozmxixy 2004-02-22
         [100 rows x 6 columns]
         """
         # Restrain
-        size = set_min(size, min_value=1)
+        size = int(set_min(size, min_value=1))
 
         # Number col
         df = pd.DataFrame(np.random.randn(size, 1), columns=["number"])
         df["number_big"] = [
             random.choice(range(100, 999)) for _ in range(size)
         ]  # Big number in range 100-999
         df["number_range"] = df["number_big"].apply(lambda x: str(x)[0] + "00")
```

### Comparing `absfuyu-3.3.0/src/absfuyu/fun/WGS.py` & `absfuyu-3.3.1/src/absfuyu/fun/WGS.py`

 * *Files identical despite different names*

### Comparing `absfuyu-3.3.0/src/absfuyu/fun/__init__.py` & `absfuyu-3.3.1/src/absfuyu/fun/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """
 Absfuyu: Fun
 ------------
 Some fun or weird stuff
 
-Version: 1.0.5
-Date updated: 27/11/2023 (dd/mm/yyyy)
+Version: 1.0.6
+Date updated: 05/04/2023 (dd/mm/yyyy)
 """
 
-
 # Library
 ###########################################################################
-from datetime import date
 import subprocess
 import sys
+from datetime import date
 
 from absfuyu.logger import logger
 from absfuyu.util.api import APIRequest
 from absfuyu.util.lunar import LunarCalendar
 
 
 # Function
@@ -51,15 +50,15 @@
 
     # Condition check
     conditions = [
         0 < day < 32,
         0 < month < 13,
     ]
     if not all(conditions):
-        raise SystemExit("Value out of range")
+        raise ValueError("Value out of range")
 
     zodiac = {
         "Aquarius": any(
             [month == 1 and day >= 20, month == 2 and day <= 18]
         ),  # 20/1-18/2
         "Pisces": any(
             [month == 2 and day >= 19, month == 3 and day <= 20]
@@ -144,15 +143,15 @@
     """
     Get random activity from ``boredapi`` website
 
     :rtype: str
     """
     try:
         api = APIRequest("https://www.boredapi.com/api/activity")
-        return api.fetch_data_only().json()["activity"]
+        return api.fetch_data_only().json()["activity"]  # type: ignore
     except:
         return "FAILED"
 
 
 def force_shutdown():
     """Force the computer to shutdown"""
     # Get operating system
```

### Comparing `absfuyu-3.3.0/src/absfuyu/fun/tarot.py` & `absfuyu-3.3.1/src/absfuyu/fun/tarot.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     @property
     def tarot_deck(self) -> List[TarotCard]:
         """
         Load pickled tarot data
 
         :rtype: list[TarotCard]
         """
-        tarot_data: list = Pickler.load(self.data_location)
+        tarot_data: list = Pickler.load(self.data_location)  # type: ignore
         logger.debug(f"{len(tarot_data)} tarot cards loaded")
         return [
             TarotCard(
                 name=x["name"],
                 rank=x["rank"],
                 suit=x["suit"],
                 meanings=x["meanings"],
```

### Comparing `absfuyu-3.3.0/src/absfuyu/game/__init__.py` & `absfuyu-3.3.1/src/absfuyu/game/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# type: ignore
 """
 Absfuyu: Game
 -------------
 Contain some game that can be played on terminal
 
 Version: 1.0.2
 Date updated: 24/11/2023 (mm/dd/yyyy)
```

### Comparing `absfuyu-3.3.0/src/absfuyu/game/sudoku.py` & `absfuyu-3.3.1/src/absfuyu/game/sudoku.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 __all__ = [
     "Sudoku"
 ]
 
 
 # Library
 ###########################################################################
-from typing import List
+from typing import List, Tuple
 
 
 # Class
 ###########################################################################
 class Sudoku:
     def __init__(self, sudoku_data: List[List[int]]) -> None:
         self.data = sudoku_data
@@ -34,15 +34,15 @@
         self._row_len = len(self.data)
         self._col_len = len(self.data[0])
         # self.solved = None
     def __str__(self) -> str:
         return f"{self.__class__.__name__}({self.export_to_string()})"
     def __repr__(self) -> str:
         return self.__str__()
-    
+
     def export_to_string(self, *, style: str = "dot") -> str:
         """
         Export Sudoku data to string form
 
         Parameters
         ----------
         style : str
@@ -53,20 +53,20 @@
         -------
         str
             Sudoku string
         """
         style_option = ["zero", "dot"]
         if style.lower() not in style_option:
             style = "dot"
-        
+
         out = "".join(str(self.data))
         remove = ["[", "]", " ", ","]
         for x in remove:
             out = out.replace(x, "")
-        
+
         if style.startswith("zero"):
             return out
         elif style.startswith("dot"):
             out = out.replace("0",".")
             return out
         else:
             return out
@@ -99,46 +99,45 @@
          [0, 0, 1, 0, 0, 0, 0, 6, 8],
          [0, 0, 8, 5, 0, 0, 0, 1, 0],
          [0, 9, 0, 0, 0, 0, 4, 0, 0]]
         """
         if len(string_data) == 81:
             # Convert
             sdk = str(string_data).replace(".","0")
-            
+
             # Divide into 9 equal parts
             temp = []
             while len(sdk) != 0:
                 temp.append(sdk[:9])
                 sdk = sdk[9:]
-            
+
             # Turn into list[list[int]]
             out = []
             for value in temp:
                 temp_list = [int(x) for x in value]
                 out.append(temp_list)
-        
+
         else:
             # Invalid length
             raise ValueError("Invalid length")
         return cls(out)
-    
+
     @classmethod
     def hardest_sudoku(cls):
         """
         Create Hardest Sudoku instance 
         ([Source](https://www.telegraph.co.uk/news/science/science-news/9359579/Worlds-hardest-sudoku-can-you-crack-it.html))
         
         Returns
         -------
         Sudoku
             ``Sudoku`` instance
         """
         return cls.from_string("8..........36......7..9.2...5...7.......457.....1...3...1....68..85...1..9....4..")
 
-
     def to_board_form(self) -> str:
         """
         Prepare sudoku board ready to print
 
         Returns
         -------
         str
@@ -178,15 +177,14 @@
                 if col == 8:
                     out_string = out_string + str(self.data[row][col]) + u"  \u2503\n"
                 else:
                     out_string = out_string + str(self.data[row][col]) + " "
 
         out_string = out_string + u" \u2516" + u"\u2500"*29 + u"\u251A"
         return out_string
-    
 
     # Solve
     def _find_empty(self):
         """
         Find the empty cell (value = 0)
 
         Return postion(row, col)
@@ -196,16 +194,16 @@
         for row in range(self._row_len):
             for col in range(self._col_len):
                 if self.data[row][col] == 0:
                     # Return position when empty
                     return (row, col)
         # Return None when there is no empty cell
         return None
-    
-    def _is_valid(self, number: int, position: tuple) -> bool:
+
+    def _is_valid(self, number: int, position: Tuple[int, int]) -> bool:
         """
         Check valid number value in row, column, box
         """
         row, col = position # unpack tuple
 
         # Check row
         for i in range(self._col_len): # each item in row i; row i has `col_len` items
@@ -249,15 +247,15 @@
                 if self._solve():
                     return True
 
                 self.data[row][col] = 0
 
         # End recursive
         return False
-    
+
     def solve(self):
         """
         Solve the Sudoku
         
         Returns
         -------
         Sudoku
@@ -282,15 +280,15 @@
          \u2503  4 3 8  \u2503  5 2 6  \u2503  9 1 7  \u2503
          \u2503  7 9 6  \u2503  3 1 8  \u2503  4 5 2  \u2503
          \u2516\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u251A
         """
         self._solve()
         # self.solved = self.data
         # self.data = self._original
-        return __class__(self.data)
-    
+        return __class__(self.data)  # type: ignore
+
 
 # Run
 ###########################################################################
 if __name__ == "__main__":
     test = Sudoku.hardest_sudoku()
-    print(test.solve().to_board_form())
+    print(test.solve().to_board_form())
```

### Comparing `absfuyu-3.3.0/src/absfuyu/game/tictactoe.py` & `absfuyu-3.3.1/src/absfuyu/game/tictactoe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
+# type: ignore
 """
 Game: Tic Tac Toe
 -----------------
 
 Version: 1.0.3
 Date update: 24/11/2023 (mm/dd/yyyy)
 """
 
 
 # Library
 ##############################################################
 import random as __random
 import time as __time
-from typing import Optional as __Optional, List as __List
+from typing import List as __List
+from typing import Optional as __Optional
 
 from absfuyu import core as __core
 from absfuyu.game.tictactoe2 import GameMode
 
-
 # Tic Tac Toe
 ##############################################################
 
 # GAME SETTING
 X = "X"
 O = "O"
 BLANK = " "
@@ -65,15 +66,14 @@
         pass
     
     if num < 1:
         return case
     return case[num]
 
 
-
 def __gen_board(row_size: int, col_size: int, content: str = BLANK):
     """
     Generate board game (with or without `numpy`)
 
     Parameter:
     ---
     row_size : int
@@ -554,8 +554,8 @@
         "Total move": filled,
         "Win by": None if state==BLANK else state,
     }
     if show_stats:
         print(f"{__C['BLUE']}GAME STATS:{__C['reset']}")
         for k, v in game_stats.items():
             print(f"{__C['YELLOW']}{k}: {v}{__C['reset']}")
-    return game_stats
+    return game_stats
```

### Comparing `absfuyu-3.3.0/src/absfuyu/game/tictactoe2.py` & `absfuyu-3.3.1/src/absfuyu/game/tictactoe2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 """
 Game: Tic Tac Toe
 -----------------
 
-Version: 2.0.2
-Date updated: 04/12/2023 (mm/dd/yyyy)
+Version: 2.0.3
+Date updated: 05/04/2024 (mm/dd/yyyy)
 """
 
-
 # Module level
 ###########################################################################
 __all__ = ["TicTacToe", "GameMode"]
 
 
 # Library
 ###########################################################################
 # from collections import namedtuple
 import random
 import time
-from typing import Dict, List, NamedTuple, Union
+from typing import Dict, List, Literal, NamedTuple, Union
 
 from absfuyu.core import CLITextColor
 
-
 # Class
 ###########################################################################
 BoardGame = List[List[str]]
 
 
 # Pos = namedtuple("Pos", ["row", "col"])  # Position
 class Pos(NamedTuple):
@@ -37,14 +35,20 @@
 
 class GameMode:
     ONE_V_ONE = "1v1"
     ONE_V_BOT = "1v0"
     BOT_V_BOT = "0v0"
 
 
+class GameStateResult(NamedTuple):
+    key: str
+    location: Literal["col", "row", "diag", "blank"]
+    pos: int
+
+
 class TicTacToe:
     """Tic Tac Toe game"""
 
     def __init__(
         self,
         game_size: int = 3,
         *,
@@ -92,50 +96,55 @@
         Generate board game
         """
         board = [
             [self.BLANK for _ in range(self.row_size)] for _ in range(self.col_size)
         ]
         return board
 
-    def _check_state(self) -> Dict[str, Union[str, int]]:
+    def _check_state(self) -> GameStateResult:
         """
         Check game winning state
 
         Returns
         -------
         dict[str, str | int]
             ``X`` | ``O`` | ``BLANK``
         """
 
         # Check rows
         for row in range(self.row_size):
             if len(set(self.board[row])) == 1:
                 key = list(set(self.board[row]))[0]
-                return {"key": key, "location": "row", "pos": row}  # modified
+                return GameStateResult(key, "row", row)
+                # return {"key": key, "location": "row", "pos": row}  # modified
 
         # Check cols
         for col in range(self.col_size):
             temp = [self.board[row][col] for row in range(self.row_size)]
             if len(set(temp)) == 1:
                 key = list(set(temp))[0]
-                return {"key": key, "location": "col", "pos": col}  # modified
+                return GameStateResult(key, "col", col)
+                # return {"key": key, "location": "col", "pos": col}  # modified
 
         # Check diagonal
         diag1 = [self.board[i][i] for i in range(len(self.board))]
         if len(set(diag1)) == 1:
             key = list(set(diag1))[0]
-            return {"key": key, "location": "diag", "pos": 1}  # modified
+            return GameStateResult(key, "diag", 1)
+            # return {"key": key, "location": "diag", "pos": 1}  # modified
 
         diag2 = [self.board[i][len(self.board) - i - 1] for i in range(len(self.board))]
         if len(set(diag2)) == 1:
             key = list(set(diag2))[0]
-            return {"key": key, "location": "diag", "pos": 2}  # modified
+            return GameStateResult(key, "diag", 2)
+            # return {"key": key, "location": "diag", "pos": 2}  # modified
 
         # Else
-        return {"key": self.BLANK}
+        return GameStateResult(self.BLANK, "blank", 0)
+        # return {"key": self.BLANK}
 
     @staticmethod
     def _print_board(board: BoardGame) -> None:
         """
         Print Tic Tac Toe board
         """
         nrow, ncol = len(board), len(board[0])
@@ -149,34 +158,34 @@
     def _win_hightlight(self) -> BoardGame:
         """
         Hight light the win by removing other placed key
         """
 
         # Get detailed information
         detail = self._check_state()
-        loc = detail["location"]
-        loc_line = detail["pos"]
+        loc = detail.location
+        loc_line = detail.pos
 
         # Make new board
         board = self._gen_board()
 
         # Fill in the hightlighted content
         if loc.startswith("col"):
             for i in range(len(board)):
-                board[i][loc_line] = detail["key"]
+                board[i][loc_line] = detail.key
         elif loc.startswith("row"):
             for i in range(len(board)):
-                board[loc_line][i] = detail["key"]
+                board[loc_line][i] = detail.key
         else:
             if loc_line == 1:
                 for i in range(len(board)):
-                    board[i][i] = detail["key"]
+                    board[i][i] = detail.key
             else:
                 for i in range(len(board)):
-                    board[i][len(board) - i - 1] = detail["key"]
+                    board[i][len(board) - i - 1] = detail.key
 
         # Output
         return board
 
     def _is_blank(self, pos: Pos) -> bool:
         """Check if current pos is filled"""
         return self.board[pos.row][pos.col] == self.BLANK
@@ -220,15 +229,15 @@
 
         bot_time : float
             Time sleep between each bot move (Default: ``0``)
         """
         # Init game
         filled = 0
         current_player = self.X
-        state = self._check_state()["key"]
+        state = self._check_state().key
         BOT = False
         BOT2 = False
 
         # Welcome message
         if self.welcome_message:
             print(
                 f"""\
@@ -260,25 +269,25 @@
         while state == self.BLANK and filled < self.row_size**2:
             print(f"{CLITextColor.BLUE}{current_player}'s turn:{CLITextColor.RESET}")
 
             try:  # Error handling
                 if (BOT and current_player == self.O) or BOT2:
                     move = self._generate_random_move()
                     str_move = f"{move.row}{self.POS_SPLIT}{move.col}"
-                    move = str_move
+                    move = str_move  # type: ignore
                 else:
-                    move = input(
+                    move = input(  # type: ignore
                         f"Place {CLITextColor.BLUE}{current_player}{CLITextColor.RESET} at {CLITextColor.BLUE}<row{self.POS_SPLIT}col>:{CLITextColor.RESET} "
                     )
 
-                if move.upper() == self.END_BREAK:  # Failsafe
+                if move.upper() == self.END_BREAK:  # type: ignore # Failsafe
                     print(f"{CLITextColor.RED}Game ended{CLITextColor.RESET}")
                     break
 
-                move = move.split(self.POS_SPLIT)
+                move = move.split(self.POS_SPLIT)  # type: ignore
                 row = int(move[0])
                 col = int(move[1])
                 place_pos = Pos(row - 1, col - 1)
 
                 if self._is_blank(place_pos):
                     self.board[place_pos.row][place_pos.col] = current_player
                     filled += 1
@@ -291,15 +300,15 @@
 
             except:  # User error
                 print(
                     f"{CLITextColor.RED}Invalid move, please try again{CLITextColor.RESET}"
                 )
                 continue
 
-            state = self._check_state()["key"]
+            state = self._check_state().key
             self._print_board(self.board)
 
             if state != self.BLANK:
                 print(f"{CLITextColor.GREEN}{state} WON!{CLITextColor.RESET}")
                 self._print_board(self._win_hightlight())
 
             # Change turn
```

### Comparing `absfuyu-3.3.0/src/absfuyu/game/wordle.py` & `absfuyu-3.3.1/src/absfuyu/game/wordle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 """
 Game: Wordle Solver
 -------------------
 
-Version: 1.1.2
-Date updated: 24/11/2023 (dd/mm/yyyy)
+Version: 1.1.3
+Date updated: 05/04/2024 (dd/mm/yyyy)
 
 Usage:
 ------
 >>> Wordle.solve()
 
 Credit:
 -------
 - [Code](https://www.inspiredpython.com/article/solving-wordle-puzzles-with-basic-python)
 - [Words](https://raw.githubusercontent.com/dwyl/english-words/master/words_dictionary.json)
 """
 
-
 # Library
 ###########################################################################
-from collections import Counter
-from itertools import chain
 import operator
 import string
+from collections import Counter
+from itertools import chain
 
 import requests
 
 from absfuyu.logger import logger
 
-
 # Settings
 ###########################################################################
 OFFLINE_WORDS = """\
 aahed,aalii,aargh,aaron,abaca,abaci,aback,abada,abaff,abaft,abaka,abama,abamp,aband,abase,abash,abask,abate,abaue,abave,abaze,abbas,abbes,abbey,abbie,abbot,abdal,abdat,abdom,abeam,abear,abede,abele,abend,aberr,abets,abhor,abide,abidi,abies,abilo,abime,abkar,abler,ables,ablet,ablow,abmho,abner,abnet,abode,abody,abohm,aboil,aboma,aboon,abord,abort,abote,about,above,abram,abray,abret,abrim,abrin,abris,abrus,absee,absey,absis,absit,abstr,abuna,abune,abura,abuse,abush,abuta,abuts,abuzz,abwab,abyes,abysm,abyss,acale,acana,acapu,acara,acari,acast,acate,accel,accoy,accra,accts,accum,accur,accus,acedy,acerb,aceta,achar,ached,achen,acher,aches,achoo,achor,acids,acidy,acier,acies,acing,acini,ackee,acker,ackey,aclys,acmes,acmic,acned,acnes,acock,acoin,acold,acoma,acone,acool,acorn,acost,acoup,acrab,acred,acres,acrid,acroa,acron,acrux,acryl,acted,actin,acton,actor,actos,actus,acuan,acute,acyls,adage,adagy,adams,adapa,adapt,adati,adaty,adawe,adawn,adays,adcon,addax,addda,added,adder,addie,addio,addis,addle,addnl,adead,adeem,adeep,adela,adeps,adept,adfix,adiel,adieu,adion,adios,adits,adjag,adlai,adlay,adlet,adman,admen,admin,admit,admix,admov,admrx,adnex,adobe,adobo,adolf,adopt,adore,adorn,adown,adoxa,adoxy,adoze,adpao,adrad,adret,adrip,adrop,adrue,adsum,adult,adunc,adure,adusk,adust,adyta,adzer,adzes,aecia,aedes,aeger,aegir,aegis,aegle,aeons,aequi,aeric,aerie,aeron,aesir,aesop,aetat,aevia,aevum,aface,afara,afars,afear,affix,afgod,afifi,afire,aflat,afley,aflow,afoam,afoot,afore,afoul,afray,afret,afric,afrit,afros,after,agada,agade,again,agama,agami,agamy,agape,agars,agasp,agast,agata,agate,agaty,agave,agaze,agena,agend,agene,agent,agers,agete,agger,aggie,aggro,aggry,aggur,aghan,aghas,agiel,agile,aging,agios,agism,agist,aglee,aglet,agley,aglow,agmas,agnat,agnel,agnes,agnus,agoge,agoho,agone,agons,agony,agora,agrah,agral,agree,agria,agric,agrin,agrom,agron,agsam,agues,aguey,agura,agush,agust,ahead,aheap,ahems,ahind,ahint,ahmed,ahmet,ahold,aholt,ahong,ahsan,ahull,ahunt,ahura,ahush,ahwal,aided,aider,aides,aiery,aiger,aigre,ailed,ailie,aillt,aimak,aimed,aimee,aimer,ainee,ainoi,ainus,aioli,airan,aired,airer,airns,airth,airts,aisle,aitch,aitis,aiver,aiwan,aizle,ajaja,ajari,ajava,ajhar,ajiva,ajuga,akala,akali,akasa,akebi,akees,akeki,akela,akene,aking,akkad,aknee,aknow,akpek,akron,akule,akund,alack,alada,alain,alaki,alala,alamo,aland,alane,alang,alani,alans,alant,alapa,alarm,alary,alate,alawi,alban,albas,albee,albin,album,albus,albyn,alcae,alces,alcid,alcor,alday,aldea,alden,alder,aldim,aldol,aldus,aleak,
 aleck,alecs,alefs,aleft,alenu,aleph,alert,aleut,alfas,alfet,alfin,alfur,algae,algal,algas,algic,algid,algin,algol,algor,algum,alhet,alias,alibi,alice,alick,alida,alids,alien,aliet,alife,alifs,align,alike,alima,aline,alish,aliso,alisp,alist,alite,ality,alive,aliya,alkes,alkin,alkyd,alkyl,allah,allan,allay,allen,aller,alley,allez,allie,allis,allod,alloo,allot,allow,alloy,allyl,almah,alman,almas,almeh,almes,almon,almud,almug,alnus,alody,aloed,aloes,aloft,alogy,aloha,aloid,aloin,alois,aloma,alone,along,aloof,alosa,alose,aloud,alout,alowe,alpax,alpen,alpha,alpid,altar,alter,altho,altin,altos,altun,altus,aluco,alula,alums,alure,aluta,alvah,alvan,alvar,alvia,alvin,alvus,alway,amaas,amadi,amaga,amahs,amain,amala,amalg,amang,amani,amant,amapa,amara,amass,amate,amati,amaut,amaze,amban,ambar,ambas,ambay,amber,ambit,amble,ambon,ambos,ambry,ameba,ameed,ameen,ameer,amelu,amend,amene,amens,ament,amess,amhar,amias,amice,amici,amide,amido,amids,amies,amiga,amigo,amine,amini,amino,amins,amire,amirs,amish,amiss,amita,amity,amlet,amman,ammer,ammos,amnia,amnic,amoke,amoks,amole,among,amora,amort,amour,amove,amowt,amper,amphi,ample,amply,ampul,ampyx,amrit,amsel,amuck,amula,amuse,amuze,amvis,amylo,amyls,amzel,anabo,anack,anama,anana,anasa,ancha,ancle,ancon,ancor,ancre,andes,andia,andor,andre,anear,anele,anend,anent,angas,angel,anger,angia,angie,angka,angle,anglo,angor,angry,angst,angus,anhyd,aniba,anice,anigh,anile,anils,anima,anime,animi,animo,anion,anise,anita,anjan,anjou,ankee,anker,ankhs,ankle,ankou,ankus,anlas,anlet,anlia,anmia,annal,annam,annas,annat,annet,annex,annie,anniv,annot,annoy,annul,annum,annus,anoas,anode,anoia,anoil,anole,anoli,anomy,anorn,anour,anous,anova,ansae,ansar,ansel,anser,antae,antal,antar,antas,anted,antes,antic,antiq,antis,anton,antra,antre,antsy,antum,anura,anury,anvil,anzac,aoife,aorta,aotea,aotes,aotus,aouad,apace,apaid,apair,apama,apart,apass,apast,apeak,apeek,apers,apert,aperu,apery,aphid,aphis,aphra,apian,apiin,apili,apina,aping,apiol,apios,apish,apism,apium,apnea,apoda,apods,apoop,aport,apout,appal,appar,appay,appel,appet,apple,apply,appmt,appro,apptd,appui,apres,april,apron,apses,apsid,apsis,aptal,apter,aptly,aquae,aquas,araba,arabs,araby,araca,arace,arach,arado,arage,arain,arake,araks,aramu,arank,arara,araru,arase,arati,araua,arawa,arber,arbor,arcae,arced,arces,archd,arche,archt,archy,arcos,arcus,ardea,ardeb,arder,ardor,ardri,aread,areae,areal,arean,arear,areas,areca,areek,areel,arefy,areic,arena,arend,areng,arent,arere,arest,arete,argal,argan,argas,argel,argid,argil,
 argin,argle,argol,argon,argos,argot,argue,argus,arhar,arhat,arian,arias,ariel,aries,ariki,arils,arioi,arion,ariot,arise,arish,arist,arite,arith,arius,arjun,arkab,arkie,arles,armed,armer,armet,armil,armit,armor,arneb,arnee,arnut,aroar,arock,aroid,aroma,aroon,aroph,arose,arpen,arrah,arras,arrau,array,arret,arrgt,arrha,arrie,arris,arrow,arroz,arses,arsis,arsle,arson,arsyl,artal,artar,artel,arter,artha,artic,artie,artly,artou,artsy,artus,aruac,aruke,arulo,arums,arupa,arusa,arval,arvel,arvos,aryan,aryls,arzan,arzun,asale,asana,asaph,asarh,ascan,ascii,ascon,ascot,ascry,ascus,asdic,asgmt,ashed,ashen,asher,ashes,ashet,ashir,ashot,ashur,asian,aside,askar,asked,asker,askew,askip,askoi,askos,aslop,asoak,asoka,aspca,aspen,asper,aspic,aspis,assai,assam,assay,asses,asset,assis,assoc,assot,astay,astel,aster,astir,astor,astre,astur,asuri,asway,aswim,asyla,asyle,async,atake,atame,atavi,ataxy,ateba,atees,atelo,ately,athar,athel,atilt,atimy,ating,atlas,atlee,atman,atmas,atmid,atmos,atnah,atoke,atole,atoll,atoms,atomy,atone,atony,atopy,atour,atren,atria,atrip,attal,attar,atter,attic,attid,attle,attry,atule,atune,atwin,atypy,aubin,aucan,aucht,audad,audio,audit,aueto,augen,auger,auget,aught,augur,aulae,aulas,aulic,auloi,aulos,aumil,aunts,aunty,aurae,aural,aurar,auras,aurei,aures,auric,aurin,aurir,auris,aurum,auryl,autem,autor,autos,autre,auxil,auxin,avahi,avail,avale,avant,avars,avast,avell,avena,avens,aveny,avera,avern,avers,avert,avery,avgas,avian,avick,aview,avile,avine,avion,aviso,avoid,avoir,avoke,avoue,avour,avowe,avows,awabi,awacs,awaft,await,awake,awald,awalt,awane,award,aware,awarn,awash,awave,aways,awber,aweek,aweel,awest,aweto,awful,awhet,awhir,awide,awing,awink,awiwi,awkly,awned,awner,awoke,awols,awork,axels,axers,axial,axile,axils,axine,axing,axiom,axion,axite,axled,axles,axman,axmen,axoid,axone,axons,ayahs,ayelp,ayens,ayins,aylet,ayllu,ayond,ayont,ayous,ayuyu,azans,azide,azido,azine,azlon,azoch,azofy,azoic,azole,azons,azote,azoth,azoxy,aztec,azure,azury,azyme,
 baaed,baals,babai,babas,babby,babel,babes,babis,babka,bable,baboo,babua,babul,babus,bacao,bacca,baccy,bache,bacin,bacis,backs,backy,bacon,badan,baddy,badge,badju,badly,badon,baffs,baffy,bafta,bagdi,bagel,bagge,baggy,bagie,bagio,bagle,bagne,bagre,bahai,baham,bahan,bahar,bahay,bahoe,bahoo,bahts,bahur,bahut,baign,baile,bailo,bails,baioc,bairn,baith,baits,baiza,baize,bajan,bajau,bajra,bajri,bakal,baked,baken,baker,bakes,bakie,bakli,bakra,balai,balak,balan,balao,balas,balat,balau,balds,baldy,baled,balei,baler,bales,balks,balky,balli,ballo,balls,bally,balms,balmy,balon,baloo,balor,balow,balsa,balti,balun,balut,balza,bamah,banak,banal,banat,banba,banca,banco,banda,bande,bandh,bandi,bando,bands,bandy,baned,banes,banff,banga,bange,bangs,bangy,bania,banig,banjo,banks,banky,banns,bantu,banty,banus,banya,barad,barat,barba,barbe,barbs,barbu,barde,bardo,bards,bardy,bared,barer,bares,baret,barff,barfs,barfy,barge,bargh,baria,baric,barid,barie,barih,baris,barit,barks,barky,barly,barms,barmy,barns,barny,baroi,baron,barra,barre,barry,barse,barth,barye,basad,basal,basan,basat,based,baser,bases,basic,basil,basin,basis,baske,basks,bason,basos,bassa,bassi,basso,bassy,basta,baste,basti,basto,basts,basyl,batad,batak,batan,batch,batea,bated,batel,bater,bates,bathe,baths,batik,batis,baton,batta,batts,battu,batty,batwa,baubo,bauch,bauds,bauge,bauld,baulk,baume,bauno,baure,bauta,bavin,bawds,bawdy,bawke,bawls,bawly,bawra,bawty,bayal,bayed,bayok,bayou,bazar,bazoo,beach,beads,beady,beaks,beaky,beala,beams,beamy,beano,beans,beant,beany,beard,bearm,bears,beast,beata,beath,beati,beats,beaus,beaut,beaux,bebar,bebat,bebay,bebed,bebog,bebop,becap,becco,beche,becks,becky,becry,becut,bedad,beday,bedel,beden,bedew,bedim,bedin,bedip,bedog,bedot,bedub,bedur,bedye,beech,beedi,beefs,beefy,beele,beent,beeps,beers,beery,beest,beeth,beets,beety,beeve,befan,befit,befog,befop,befur,begad,began,begar,begat,begay,begem,beget,begin,begob,begod,begot,begum,begun,begut,behap,behav,behen,behew,beice,beige,beigy,beild,being,beira,beisa,bejan,bejel,bejig,bekah,bekko,belah,belam,belap,belar,belat,belay,belch,belee,belga,belie,belis,bella,belle,belli,bello,bells,belly,below,belts,belue,belve,bemad,beman,bemar,bemas,bemat,bemba,bemix,bemol,bemud,benab,bench,benda,bends,bendy,benes,benet,benic,benim,benin,benjy,benne,benni,benny,bensh,bents,benty,benzo,beode,bepat,bepaw,bepen,bepun,berat,beray,beret,bergh,bergs,bergy,berme,berms,berne,berob,beroe,berri,berry,berth,berun,beryl,beryx,besan,besee,beset,besew,besin,besit,besom,besot,bespy,besra,
@@ -113,19 +111,21 @@
             for character, value in self._LETTER_COUNTER.items()
         }
 
         # Notation
         self._GREEN = green
         self._YELLOW = yellow
         self._GRAY = gray
+
     def __str__(self) -> str:
-        pass
+        return self.__class__.__name__
+
     def __repr__(self) -> str:
         return self.__str__()
-    
+
     def update_words(self) -> None:
         """
         Try to fetch words list from online source
         """
         try:
             dict_link = "https://raw.githubusercontent.com/dwyl/english-words/master/words_dictionary.json"
             res = requests.get(dict_link)
@@ -149,26 +149,26 @@
     def _sort_by_word_commonality(self):
         sort_by = operator.itemgetter(1)
         return sorted(
             [(word, self._calculate_word_commonality(word)) for word in self._WORDS],
             key=sort_by,
             reverse=True,
         )
-    
+
     def _display_word_table(self, word_commonalities):
         for (word, freq) in word_commonalities:
             print(f"{word:<10} | {freq:<5.2}")
 
     def _input_word(self):
         while True:
             word = input("Input the word you entered> ")
             if len(word) == self._WORD_LENGTH and word.lower() in self._WORDS:
                 break
         return word.lower()
-    
+
     def _input_response(self):
         print("Type the color-coded reply from Wordle:")
         print(f"  {self._GREEN} for Green")
         print(f"  {self._YELLOW} for Yellow")
         print(f"  {self._GRAY} for Gray")
         while True:
             response = input("Response from Wordle> ")
@@ -183,15 +183,15 @@
         for letter, v_letter in zip(word, word_vector):
             if letter not in v_letter:
                 return False
         return True
 
     def _match(self, word_vector, possible_words):
         return [word for word in possible_words if self._match_word_vector(word, word_vector)]
-    
+
     # Main
     def solve(self) -> None:
         """Solve Wordle"""
         word_vector = [set(string.ascii_lowercase) for _ in range(self._WORD_LENGTH)]
         for attempt in range(1, self._ALLOWED_ATTEMPTS + 1):
             print(f"Attempt {attempt} with {len(self._WORDS)} possible words")
             self._display_word_table(self._sort_by_word_commonality()[:15])
```

### Comparing `absfuyu-3.3.0/src/absfuyu/general/__init__.py` & `absfuyu-3.3.1/src/absfuyu/general/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,46 +12,46 @@
 - data_extension
 - generator
 - human
 """
 
 # Libary
 ###########################################################################
-# from typing import List
+from typing import Any, Dict, Optional
 
 from absfuyu.general import content, data_extension, generator, human
 
 
 # Class
 ###########################################################################
 class Dummy:
     """
     Dummy class that has nothing
 
     Update attribute through dict
     """
 
-    def __init__(self, data: dict = None) -> None:
+    def __init__(self, data: Optional[Dict[Any, Any]] = None) -> None:
         try:
-            self.__dict__.update(data)
+            self.__dict__.update(data)  # type: ignore
         except:
             pass
 
     def __str__(self) -> str:
         class_name = self.__class__.__name__
         return f"{class_name}({self.__dict__})"
 
     def __repr__(self) -> str:
         return self.__str__()
 
     def dir_(self):
         """List ``property``"""
         return [x for x in self.__dir__() if not x.startswith("_")]
 
-    def update(self, data: dict) -> None:
+    def update(self, data: Dict[Any, Any]) -> None:
         """
         Update with dict data
 
         :param data: Dict data
         :type data: dict
         """
         self.__dict__.update(data)
```

### Comparing `absfuyu-3.3.0/src/absfuyu/general/content.py` & `absfuyu-3.3.1/src/absfuyu/general/content.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 """
 Absfuyu: Content
 ----------------
 Handle .txt file
 
-Version: 1.2.5
-Date updated: 27/11/2023 (dd/mm/yyyy)
+Version: 1.2.6
+Date updated: 05/04/2024 (dd/mm/yyyy)
 
 Usage:
 ------
 >>> from absfuyu.general.content import ContentLoader
 """
 
-
 # Module level
 ###########################################################################
 __all__ = ["ContentLoader", "Content", "LoadedContent"]
 
 
 # Library
 ###########################################################################
-from collections import Counter
-from itertools import chain
 import json
-from pathlib import Path
 import random
 import re
+from collections import Counter
+from itertools import chain
+from pathlib import Path
 from typing import List, Optional
 
 from unidecode import unidecode
 
 from absfuyu.logger import logger
 
 
@@ -59,15 +58,15 @@
         Convert data through ``unidecode`` package
 
         Returns
         -------
         Content
             ``unidecoded`` Content
         """
-        return __class__([unidecode(self.data), list(map(unidecode, self.tag))])
+        return self.__class__([unidecode(self.data), list(map(unidecode, self.tag))])
 
     def to_text(self) -> str:
         """
         Convert back into text
 
         Returns
         -------
@@ -136,15 +135,15 @@
 
         new_tag = [x.strip().lower() for x in temp]
         logger.debug(f"Current tags: {self.tag}")
         logger.debug(f"New tags: {new_tag}")
         self.tag = list(set(self.tag + new_tag))
         logger.debug(f"Final tags: {self.tag} Len: {len(self.tag)}")
 
-        return __class__([self.data, self.tag])
+        return self.__class__([self.data, self.tag])
 
 
 class LoadedContent(List[Content]):
     """
     Contain list of ``Content``
     """
 
@@ -159,15 +158,15 @@
         """
         Apply function to each entry
 
         :param func: Callable function
         :type func: Callable
         :rtype: LoadedContent
         """
-        return __class__(func(x.data) for x in self)
+        return self.__class__(func(x.data) for x in self)
 
     @classmethod
     def load_from_json(cls, file: Path) -> "LoadedContent":
         """
         Use this method to load data from ``.json`` file from ``to_json()`` method
 
         Parameters
@@ -218,25 +217,27 @@
             # logger.debug(f"Tag not exist, changing to a random tag... {tag}")
             logger.warning(f'"{tag}" tag does not exist')
             _avail_tag = ", ".join(list(dict(self.tag_count().most_common(5)).keys()))
             raise ValueError(
                 f"Available tags: {_avail_tag},..."
                 f"\nMore tag at: `{self.__class__.__name__}.tags`"
             )
-        return __class__([x for x in self if tag in x.tag])
+        return self.__class__([x for x in self if tag in x.tag])
 
     def find(self, keyword: str) -> "LoadedContent":
         """
         Return all entries that include ``keyword``
 
         :param keyword: Keyword to find
         :type keyword: str
         :rtype: LoadedContent
         """
-        temp = __class__([x for x in self if x.data.lower().find(keyword.lower()) >= 0])
+        temp = self.__class__(
+            [x for x in self if x.data.lower().find(keyword.lower()) >= 0]
+        )
         if temp:
             logger.debug(f"Found {len(temp)} {'entries' if len(temp) > 1 else 'entry'}")
         else:
             logger.debug("No result")
         return temp
 
     def short_form(self, separator: str = ",") -> List[str]:
@@ -302,15 +303,15 @@
         >>> test = "Shop A, 22 ABC Street, DEF District, GHI City"
         >>> # After handle_address()
         ["Shop A", "22 ABC Street", "DEF District", "GHI City"]
 
         >>> # After handle_address(first_item_not_address = False)
         ["22 ABC Street", "DEF District", "GHI City"]
         """
-        return __class__(
+        return self.__class__(
             [
                 x.handle_address(
                     address_separator=address_separator,
                     first_item_not_address=first_item_not_address,
                 )
                 for x in self
             ]
@@ -369,15 +370,15 @@
     ``<content><split_symbol><tags separated by <tag_separate_symbol>>``
     """
 
     def __init__(
         self,
         file_path: Path,
         characteristic_detect: bool = True,
-        tag_dictionary: dict = None,
+        tag_dictionary: Optional[dict] = None,
         *,
         comment_symbol: str = "#",
         split_symbol: str = "|",
         tag_separate_symbol: str = ",",
     ) -> None:
         """
         Parameters
@@ -419,15 +420,15 @@
         else:
             logger.debug(
                 f"Tag pattern available: "
                 f"{len(tag_dictionary)} {'entries' if len(tag_dictionary) > 1 else 'entry'} "
                 f"({len(set(tag_dictionary.values()))} unique "
                 f"{'tags' if len(set(tag_dictionary.values())) > 1 else 'tag'})"
             )
-            self.tag_dictionary: dict = tag_dictionary
+            self.tag_dictionary = tag_dictionary
 
         # symbol stuff
         assert (
             comment_symbol != split_symbol
         ), "comment_symbol and split_symbol should have different values"
         assert (
             tag_separate_symbol != split_symbol
```

### Comparing `absfuyu-3.3.0/src/absfuyu/general/data_extension.py` & `absfuyu-3.3.1/src/absfuyu/general/data_extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """
 Absfuyu: Data extension
 -----------------------
 Extension for data type such as ``list``, ``str``, ``dict``, ...
 
-Version: 1.14.2
-Date updated: 20/03/2024 (dd/mm/yyyy)
+Version: 1.14.3
+Date updated: 05/04/2024 (dd/mm/yyyy)
 
 Features:
 ---------
 - DictExt
 - IntNumber
 - ListExt
 - Text
 
 Usage:
 ------
 >>> from absfuyu.general.data_extension import DictExt, IntNumber, ListExt, Text
 """
 
-
 # Module level
 ###########################################################################
 __all__ = [
     # Main
     "Text",
     "IntNumber",
     "ListExt",
@@ -44,36 +43,36 @@
 # Library
 ###########################################################################
 import math
 import operator
 import random
 from collections import Counter
 from itertools import accumulate, chain, groupby
+from sys import version_info as _python_version
 from typing import (
     Any,
     Callable,
     Dict,
     List,
     NamedTuple,
     Optional,
     Tuple,
     TypedDict,
     Union,
 )
-from sys import version_info as python_version
 
-if python_version.minor >= 11:
+if _python_version.minor >= 11:
     from typing import NotRequired
 else:
-    from typing_extensions import NotRequired
+    from typing_extensions import NotRequired  # type: ignore
 
 from deprecated.sphinx import versionadded, versionchanged
 
-from absfuyu.general.generator import Generator, Charset
-from absfuyu.logger import logger, _compress_list_for_print
+from absfuyu.general.generator import Charset, Generator
+from absfuyu.logger import _compress_list_for_print, logger
 from absfuyu.util import set_min, set_min_max
 
 
 # Function
 ###########################################################################
 def _dict_bool(dict_object: dict, option: bool) -> Optional[dict]:
     """
@@ -110,15 +109,15 @@
 
     def to_list(self) -> List[Union[int, float]]:
         """
         Convert into list
 
         :rtype: list[int | float]
         """
-        return [self.number] * self.power_by
+        return [self.number] * int(self.power_by)
 
     def calculate(self) -> float:
         """
         Calculate the ``self.number`` to the power of ``self.power_by``
 
         :rtype: float
         """
@@ -216,39 +215,39 @@
 # Class
 ###########################################################################
 class Text(str):
     """
     ``str`` extension
     """
 
-    def divide(self, string_split_size: int = 60) -> list:
+    def divide(self, string_split_size: int = 60) -> List[str]:
         """
         Divide long string into smaller size
 
         Parameters
         ----------
         string_split_size : int
             Divide string every ``x`` character
             (Default: ``60``)
 
         Returns
         -------
-        list
+        list[str]
             A list in which each item is a smaller
             string with the size of ``string_split_size``
             (need to be concaternate later)
 
 
         Example:
         --------
         >>> test = Text("This is an extremely long line of text!")
         >>> test.divide(string_split_size=20)
         ['This is an extremely', ' long line of text!']
         """
-        temp = self
+        temp = str(self)
         output = []
         while len(temp) != 0:
             output.append(temp[:string_split_size])
             temp = temp[string_split_size:]
         return output
 
     def divide_with_variable(
@@ -410,15 +409,15 @@
 
         Example:
         --------
         >>> test = Text("Hello, World!")
         >>> test.reverse()
         '!dlroW ,olleH'
         """
-        return __class__(self[::-1])
+        return self.__class__(self[::-1])
 
     def is_pangram(self) -> bool:
         """
         Check if string is a pangram
 
             A pangram is a unique sentence in which
             every letter of the alphabet is used at least once
@@ -507,24 +506,24 @@
 
         Example:
         --------
         >>> test = Text("This is an extremely long line of text!")
         >>> test.random_capslock()
         'tHis iS An ExtREmELY loNg liNE oF tExT!'
         """
-        probability = set_min_max(probability)
+        probability = int(set_min_max(probability))
         text = self.lower()
 
         temp = []
         for x in text:
             if random.randint(1, 100) <= probability:
                 x = x.upper()
             temp.append(x)
         logger.debug(temp)
-        return __class__("".join(temp))
+        return self.__class__("".join(temp))
 
     def reverse_capslock(self) -> "Text":
         """
         Reverse capslock in string
 
         Returns
         -------
@@ -540,15 +539,15 @@
         """
         temp = list(self)
         for i, x in enumerate(temp):
             if x.isupper():
                 temp[i] = x.lower()
             else:
                 temp[i] = x.upper()
-        return __class__("".join(temp))
+        return self.__class__("".join(temp))
 
     def to_list(self) -> List[str]:
         """
         Convert into list
 
         Returns
         -------
@@ -606,17 +605,17 @@
 
         Example:
         --------
         >>> Text("test").count_pattern("t")
         2
         """
         if len(pattern) > len(self):
-            raise ValueError(f"len(pattern) must not larger than len({self})")
+            raise ValueError(f"len(pattern) must not larger than {len(self)}")
 
-        temp = self
+        temp = str(self)
         if ignore_capslock:
             pattern = pattern.lower()
             temp = temp.lower()
 
         out = [
             1
             for i in range(0, len(temp) - len(pattern) + 1)
@@ -655,15 +654,15 @@
 
         >>> test.hapax(strict=True)
         ['b']
         """
         word_list: List[str] = self.lower().split()
         if strict:
             remove_characters: List[str] = list("\"'.,:;|()[]{}\/!@#$%^&*-_=+?<>`~")
-            temp = self
+            temp = str(self)
             for x in remove_characters:
                 temp = temp.replace(x, "")
             word_list = temp.lower().split()
 
         hapaxes = filter(lambda x: word_list.count(x) == 1, word_list)
         return list(hapaxes)
 
@@ -819,36 +818,36 @@
             ## 74_207_281, 77_232_917, 82_589_933
         ]
         perfect_number = []
         for x in perfect_number_index:
             # a perfect number have a form of (2**(n-1))*((2**n)-1)
             perfect_number.append((2**(x-1))*((2**x)-1))
         """
-        number = self
+        number = int(self)
 
         perfect_number = [
             6,
             28,
             496,
             8128,
             33_550_336,
             8_589_869_056,
             137_438_691_328,
             2_305_843_008_139_952_128,
         ]
 
-        if int(number) in perfect_number:
+        if number in perfect_number:
             return True
 
-        elif int(number) < perfect_number[-1]:
+        elif number < perfect_number[-1]:
             return False
 
         else:
             # Faster way to check
-            perfect_number_index = [
+            perfect_number_index: List[int] = [
                 61,
                 89,
                 107,
                 127,
                 521,
                 607,
                 1279,
@@ -888,27 +887,27 @@
                 ## 74_207_281,
                 ## 77_232_917,
                 ## 82_589_933
             ]
             for x in perfect_number_index:
                 # a perfect number have a form of (2**(n-1))*((2**n)-1)
                 perfect_number = (2 ** (x - 1)) * ((2**x) - 1)
-                if number < perfect_number:
+                if number < perfect_number:  # type: ignore
                     return False
-                elif number == perfect_number:
+                elif number == perfect_number:  # type: ignore
                     return True
 
             # Manual way when above method not working
             # sum
             s = 1
             # add all divisors
             i = 2
             while i * i <= number:
                 if number % i == 0:
-                    s += +i + number / i
+                    s += +i + number / i  # type: ignore
                 i += 1
             # s == number -> perfect
             return True if s == number and number != 1 else False
 
     def is_narcissistic(self) -> bool:
         """
         Check if a narcissistic number
@@ -924,15 +923,16 @@
         -------
         bool
             | ``True`` if a narcissistic number
             | ``False`` if not a narcissistic number
         """
         try:
             check = sum([int(x) ** len(str(self)) for x in str(self)])
-            return self == check
+            res = int(self) == check
+            return res  # type: ignore
         except:
             return False
 
     def reverse(self) -> "IntNumber":
         """
         Reverse a number. Reverse ``abs(number)`` if ``number < 0``
 
@@ -944,18 +944,18 @@
 
         Example:
         --------
         >>> test = IntNumber(102)
         >>> test.reverse()
         201
         """
-        number = self
+        number = int(self)
         if number <= 1:
             number *= -1
-        return __class__(str(number)[::-1])
+        return self.__class__(str(number)[::-1])
 
     def is_palindromic(self) -> bool:
         """
         A palindromic number (also known as a numeral palindrome
         or a numeric palindrome) is a number (such as ``16461``)
         that remains the same when its digits are reversed.
 
@@ -999,17 +999,17 @@
         Example:
         --------
         >>> test = IntNumber(102)
         >>> test.lcm(5)
         510
         """
         try:
-            return __class__(math.lcm(self, with_number))
+            return self.__class__(math.lcm(self, with_number))
         except:
-            return __class__((self * with_number) // math.gcd(self, with_number))
+            return self.__class__((self * with_number) // math.gcd(self, with_number))
 
     @versionchanged(version="3.3.0", reason="Fix bug")
     def gcd(self, with_number: int) -> "IntNumber":
         """
         Greatest common divisor of ``self`` and ``with_number``
 
         Parameters
@@ -1025,15 +1025,15 @@
 
         Example:
         --------
         >>> test = IntNumber(1024)
         >>> test.gcd(8)
         8
         """
-        return __class__(math.gcd(self, with_number))
+        return self.__class__(math.gcd(self, with_number))
 
     def add_to_one_digit(self, master_number: bool = False) -> "IntNumber":
         """
         Convert ``self`` into 1-digit number
         by adding all of the digits together
 
         Parameters
@@ -1054,25 +1054,25 @@
         >>> test.add_to_one_digit()
         2
 
         >>> test = IntNumber(119)
         >>> test.add_to_one_digit(master_number=True)
         11
         """
-        number = self
+        number = int(self)
         if number < 0:
             number *= -1
         logger.debug(f"Current number: {number}")
         while len(str(number)) != 1:
             number = sum(map(int, str(number)))
             if master_number:
                 if number == 22 or number == 11:
                     break  # Master number
             logger.debug(f"Sum after loop: {number}")
-        return __class__(number)
+        return self.__class__(number)
 
     def divisible_list(self, short_form: bool = True) -> List[int]:
         """
         A list of divisible number
 
         Parameters
         ----------
@@ -1205,15 +1205,15 @@
             "palindromic": self.is_palindromic(),
             "palindromic prime": self.is_palindromic_prime(),
         }
         if short_form:
             characteristic = DictBoolTrue(characteristic)
 
         output["characteristic"] = characteristic
-        return output
+        return output  # type: ignore
 
 
 class ListExt(list):
     """
     ``list`` extension
     """
 
@@ -1246,15 +1246,17 @@
             | (Default: ``5``)
 
         Returns
         -------
         list
             Filtered list
         """
-        number_of_items = set_min_max(number_of_items, min_value=0, max_value=len(self))
+        number_of_items = int(
+            set_min_max(number_of_items, min_value=0, max_value=len(self))
+        )
         return self[:number_of_items]
 
     def tail(self, number_of_items: int = 5) -> list:
         """
         Show last ``number_of_items`` items in ``ListExt``
 
         Parameters
@@ -1264,15 +1266,17 @@
             | (Default: ``5``)
 
         Returns
         -------
         list
             Filtered list
         """
-        number_of_items = set_min_max(number_of_items, min_value=0, max_value=len(self))
+        number_of_items = int(
+            set_min_max(number_of_items, min_value=0, max_value=len(self))
+        )
         return self[::-1][:number_of_items][::-1]
 
     def sorts(self, reverse: bool = False) -> "ListExt":
         """
         Sort all items (with different type) in ``list``
 
         Parameters
@@ -1291,26 +1295,26 @@
         Example:
         --------
         >>> test = ListExt([9, "abc", 3.5, "aaa", 1, 1.4])
         >>> test.sorts()
         [1, 9, 'aaa', 'abc', 1.4, 3.5]
         """
         lst = self.copy()
-        type_weights = {}
+        type_weights: dict = {}
         for x in lst:
             if type(x) not in type_weights:
                 type_weights[type(x)] = len(type_weights)
         logger.debug(f"Type weight: {type_weights}")
 
         output = sorted(
             lst, key=lambda x: (type_weights[type(x)], str(x)), reverse=reverse
         )
 
         logger.debug(output)
-        return __class__(output)
+        return self.__class__(output)
 
     def freq(
         self,
         sort: bool = False,
         num_of_first_char: Optional[int] = None,
         appear_increment: bool = False,
     ) -> Union[dict, List[int]]:
@@ -1349,15 +1353,15 @@
 
         >>> test = ListExt([1, 1, 2, 3, 3, 4, 5, 6])
         >>> test.freq(appear_increment=True)
         [2, 3, 5, 6, 7, 8]
         """
 
         if sort:
-            data = self.sorts()
+            data = self.sorts().copy()
         else:
             data = self.copy()
 
         if num_of_first_char is None:
             temp = Counter(data)
         else:
             max_char: int = min([len(str(x)) for x in data])
@@ -1368,15 +1372,15 @@
             else:
                 logger.debug(f"Freq of first {num_of_first_char} char")
                 temp = Counter([str(x)[:num_of_first_char] for x in data])
 
         try:
             times_appear = dict(sorted(temp.items()))
         except:
-            times_appear = dict(__class__(temp.items()).sorts())
+            times_appear = dict(self.__class__(temp.items()).sorts())
         logger.debug(times_appear)
 
         if appear_increment:
             times_appear_increment: List[int] = list(
                 accumulate(times_appear.values(), operator.add)
             )
             logger.debug(times_appear_increment)
@@ -1510,15 +1514,15 @@
         Example:
         --------
         >>> test = ListExt([1, 2, 3])
         >>> test.apply(str)
         ['1', '2', '3']
         """
         # return __class__(func(x) for x in self)
-        return __class__(map(func, self))
+        return self.__class__(map(func, self))
 
     def unique(self) -> "ListExt":
         """
         Remove duplicates
 
         Returns
         -------
@@ -1528,15 +1532,15 @@
 
         Example:
         --------
         >>> test = ListExt([1, 1, 1, 2, 2, 3])
         >>> test.unique()
         [1, 2, 3]
         """
-        return __class__(set(self))
+        return self.__class__(set(self))
 
     def group_by_unique(self) -> "ListExt":
         """
         Group duplicated elements into list
 
         Returns
         -------
@@ -1552,15 +1556,15 @@
         """
         # Old
         # out = self.sorts().slice_points(self.freq(appear_increment=True))
         # return __class__(out[:-1])
 
         # New
         temp = groupby(self.sorts())
-        return __class__([list(g) for _, g in temp])
+        return self.__class__([list(g) for _, g in temp])
 
     @staticmethod
     def _group_by_unique(iterable: list) -> List[list]:
         """
         Static method for ``group_by_unique``
         """
         return list([list(g) for _, g in groupby(iterable)])
@@ -1595,15 +1599,15 @@
         >>> test.group_by_pair_value()
         [['a', 4, 'b'], ['c', 5]]
         """
 
         iter = self.copy()
 
         # Init loop
-        for _ in range(set_min(max_loop, min_value=3)):
+        for _ in range(int(set_min(max_loop, min_value=3))):
             temp: Dict[Any, list] = {}
             # Make dict{key: all `item` that contains `key`}
             for item in iter:
                 for x in item:
                     if temp.get(x, None) is None:
                         temp[x] = [item]
                     else:
@@ -1658,23 +1662,23 @@
 
         Example:
         --------
         >>> test = ListExt([9, 9, 9])
         >>> test.numbering()
         [(0, 9), (1, 9), (2, 9)]
         """
-        start = set_min(start, min_value=0)
+        start = int(set_min(start, min_value=0))
         return ListExt(enumerate(self, start=start))
 
     @staticmethod
     def _numbering(iterable: list, start: int = 0) -> List[Tuple[int, Any]]:
         """
         Static method for ``numbering``
         """
-        start = set_min(start, min_value=0)
+        start = int(set_min(start, min_value=0))
         return list(enumerate(iterable, start=start))
 
 
 class DictExt(dict):
     """
     ``dict`` extension
     """
@@ -1748,15 +1752,15 @@
 
         Example:
         --------
         >>> test = DictExt({"abc": 9})
         >>> test.swap_items()
         {9: 'abc'}
         """
-        return __class__(zip(self.values(), self.keys()))
+        return self.__class__(zip(self.values(), self.keys()))
 
     def apply(self, func: Callable, apply_to_value: bool = True) -> "DictExt":
         """
         Apply function to ``DictExt.keys()`` or ``DictExt.values()``
 
         Parameters
         ----------
@@ -1779,16 +1783,16 @@
         >>> test.apply(str)
         {'abc': '9'}
         """
         if apply_to_value:
             k = self.keys()
             v = map(func, self.values())
         else:
-            k = map(func, self.keys())
-            v = self.values()
-        return __class__(zip(k, v))
+            k = map(func, self.keys())  # type: ignore
+            v = self.values()  # type: ignore
+        return self.__class__(zip(k, v))
 
 
 # Run
 ###########################################################################
 if __name__ == "__main__":
     logger.setLevel(10)
```

### Comparing `absfuyu-3.3.0/src/absfuyu/general/generator.py` & `absfuyu-3.3.1/src/absfuyu/general/generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 """
 Absfuyu: Generator
 ------------------
 This generate stuff (Not python's ``generator``)
 
-Version: 1.1.0
-Date updated: 06/03/2024 (dd/mm/yyyy)
+Version: 1.1.1
+Date updated: 05/04/2024 (dd/mm/yyyy)
 
 Features:
 ---------
 - Generate random string
 - Generate key
 - Generate check digit
 - Generate combinations of list in range
 """
 
-
 # Module level
 ###########################################################################
 __all__ = ["Charset", "Generator"]
 
 
 # Library
 ###########################################################################
+import string
 from itertools import chain, combinations
 from random import choice
-import string
 
 # from string import (
 #     ascii_letters as _ascii_letters,
 #     ascii_uppercase as _ascii_uppercase,
 #     ascii_lowercase as _ascii_lowercase,
 #     digits as _digits,
 #     printable as _printable,
@@ -62,15 +61,15 @@
     # UPPERCASE = _ascii_uppercase
     # LOWERCASE = _ascii_lowercase
     # DIGIT = _digits
     # SPECIAL = _punctuation
     # ALL = _printable
 
     def __str__(self) -> str:
-        charset = [x for x in __class__.__dict__.keys() if not x.startswith("__")]
+        charset = [x for x in self.__class__.__dict__.keys() if not x.startswith("__")]
         return f"List of Character set: {charset}"
 
     def __repr__(self) -> str:
         return self.__str__()
 
 
 class Generator:
@@ -144,15 +143,15 @@
         >>> Generator.generate_string(times=3)
         ['67Xfh1fv', 'iChcGz9P', 'u82fNzlm']
         """
 
         try:
             char_lst = list(charset)
         except:
-            char_lst = charset
+            char_lst = charset  # type: ignore # ! review this sometime
         # logger.debug(char_lst)
 
         unique_string = []
         count = 0
         logger.debug(f"Unique generated text: {unique}")
 
         while count < times:
@@ -208,15 +207,15 @@
 
         Example:
         --------
         >>> Generator.generate_key(letter_per_block=10, number_of_block=2)
         'VKKPJVYD2H-M7R687QCV2'
         """
         out = sep.join(
-            __class__.generate_string(
+            __class__.generate_string(  # type: ignore
                 charset,
                 size=letter_per_block,
                 times=number_of_block,
                 unique=False,
                 string_type_if_1=False,
             )
         )
@@ -263,22 +262,22 @@
         logger.debug(f"Base: {number}")
         # turn into list then reverse the order
         num = list(str(number))[::-1]
         sum = 0
         logger.debug(f"Reversed: {''.join(num)}")
         for i in range(len(num)):
             # convert back into integer
-            num[i] = int(num[i])
+            num[i] = int(num[i])  # type: ignore
             if i % 2 == 0:
                 # double value of the even-th digit
                 num[i] *= 2
                 # sum the character of digit if it's >= 10
-                if num[i] >= 10:
-                    num[i] -= 9
-            sum += num[i]
+                if num[i] >= 10:  # type: ignore
+                    num[i] -= 9  # type: ignore
+            sum += num[i]  # type: ignore
             logger.debug(f"Loop {i+1}: {num[i]}, {sum}")
 
         out = (10 - (sum % 10)) % 10
         logger.debug(f"Output: {out}")
         return out
 
     @staticmethod
@@ -305,16 +304,16 @@
         -------
         list[tuple]
             A list of all combinations from range(``min_len``, ``max_len``) of ``sequence``
         """
         # Restrain
         if max_len < 1:
             max_len = len(sequence)
-        max_len = set_max(max_len, max_value=len(sequence))
-        min_len = set_min_max(min_len, min_value=1, max_value=max_len)
+        max_len = int(set_max(max_len, max_value=len(sequence)))
+        min_len = int(set_min_max(min_len, min_value=1, max_value=max_len))
         logger.debug(f"Combination range: [{min_len}, {max_len}]")
 
         # Return
         return list(
             chain.from_iterable(
                 [list(combinations(sequence, i)) for i in range(min_len, max_len + 1)]
             )
```

### Comparing `absfuyu-3.3.0/src/absfuyu/general/human.py` & `absfuyu-3.3.1/src/absfuyu/general/human.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 """
 Absfuyu: Human
 --------------
 Human related stuff
 
-Version: 1.3.0
-Date updated: 08/12/2023 (dd/mm/yyyy)
+Version: 1.3.1
+Date updated: 05/04/2024 (dd/mm/yyyy)
 """
 
-
 # Module level
 ###########################################################################
 __all__ = ["Human", "Person"]
 
 
 # Library
 ###########################################################################
 from datetime import datetime, time
 from typing import Optional, Union
 
 from dateutil.relativedelta import relativedelta
 
-from absfuyu.general.data_extension import IntNumber
 from absfuyu.fun import zodiac_sign
-
-# from absfuyu.util import set_min_max
-from absfuyu.version import Version
+from absfuyu.general.data_extension import IntNumber
+from absfuyu.version import Version  # type: ignore
 
 
 # Sub-Class
 ###########################################################################
 class _FloatBase:
     """To show some unit"""
 
@@ -103,45 +100,47 @@
             else self.first_name
         )
 
         # Birthday
         now = datetime.now()
         if birthday is None:
             modified_birthday = now.date()
-        else:
+        elif isinstance(birthday, str):
             for x in ["/", "-"]:
                 birthday = birthday.replace(x, "/")
             modified_birthday = datetime.strptime(birthday, "%Y/%m/%d")
+        else:
+            modified_birthday = birthday
             # birthday = list(map(int, birthday.split("/")))
             # modified_birthday = date(*birthday)
             # modified_birthday = date(birthday[0], birthday[1], birthday[2])
 
         if birth_time is None:
             modified_birthtime = now.time()
         else:
-            birth_time = list(map(int, birth_time.split(":")))
+            birth_time = list(map(int, birth_time.split(":")))  # type: ignore
             modified_birthtime = time(*birth_time)
             # modified_birthtime = time(birth_time[0], birth_time[1])
 
-        self.birthday = modified_birthday.date()
+        self.birthday = modified_birthday.date()  # type: ignore
         self.birth_time = modified_birthtime
 
         self.birth = datetime(
             modified_birthday.year,
             modified_birthday.month,
             modified_birthday.day,
             modified_birthtime.hour,
             modified_birthtime.minute,
         )
 
         # Others
-        self.gender: bool = gender  # True: Male; False: Female
-        self.height: float = None  # centimeter
-        self.weight: float = None  # kilogram
-        self.blood_type: Union[str, BloodType] = BloodType.OTHER
+        self.gender: bool = gender  # type: ignore # True: Male; False: Female
+        self.height: float = None  # type: ignore # centimeter
+        self.weight: float = None  # type: ignore # kilogram
+        self.blood_type: Union[str, BloodType] = BloodType.OTHER  # type: ignore
 
     def __str__(self) -> str:
         class_name = self.__class__.__name__
         return f"{class_name}({str(self.name)})"
 
     def __repr__(self) -> str:
         class_name = self.__class__.__name__
@@ -284,25 +283,25 @@
         first_name: str,
         last_name: Optional[str] = None,
         birthday: Union[str, datetime, None] = None,
         birth_time: Optional[str] = None,
         gender: Union[bool, None] = None,
     ) -> None:
         super().__init__(first_name, last_name, birthday, birth_time, gender)
-        self.address: str = None
-        self.hometown: str = None
-        self.email: str = None
-        self.phone_number: str = None
-        self.nationality = None
-        self.likes: list = None
-        self.hates: list = None
-        self.education = None
-        self.occupation: str = None
-        self.personality = None
-        self.note: str = None
+        self.address: str = None  # type: ignore
+        self.hometown: str = None  # type: ignore
+        self.email: str = None  # type: ignore
+        self.phone_number: str = None  # type: ignore
+        self.nationality = None  # type: ignore
+        self.likes: list = None  # type: ignore
+        self.hates: list = None  # type: ignore
+        self.education = None  # type: ignore
+        self.occupation: str = None  # type: ignore
+        self.personality = None  # type: ignore
+        self.note: str = None  # type: ignore
 
     @property
     def zodiac_sign(self):
         """
         Zodiac sign of ``Person``
 
         Returns
@@ -341,22 +340,16 @@
         """
         Numerology number of ``Person``
 
         Returns
         -------
         int
             Numerology number
-
-        None
-            When unable to get ``self.birthday``
         """
-        try:
-            temp = f"{self.birthday.year}{self.birthday.month}{self.birthday.day}"
-            return IntNumber(temp).add_to_one_digit(master_number=True)
-        except:
-            return None
+        temp = f"{self.birthday.year}{self.birthday.month}{self.birthday.day}"
+        return IntNumber(temp).add_to_one_digit(master_number=True)
 
 
 # Run
 ###########################################################################
 if __name__ == "__main__":
     print(Person.JohnDoe().__dict__)
```

### Comparing `absfuyu-3.3.0/src/absfuyu/logger.py` & `absfuyu-3.3.1/src/absfuyu/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 """
 Absfuyu: Logger
 ---------------
 Custom Logger Module
 
-Version: 1.3.1
-Date updated: 23/11/2023 (mm/dd/yyyy)
+Version: 1.3.2
+Date updated: 05/04/2024 (mm/dd/yyyy)
 
 Usage:
 ------
 >>> from absfuyu.logger import logger, LogLevel
 >>> logger.setLevel(LogLevel.DEBUG)
 >>> logger.debug("This logs!")
 """
 
-
 # Module level
 ###########################################################################
 __all__ = [
     # logger
     "logger", "compress_for_log",
     # log level
     "LogLevel"
 ]
 
 
 # Library
 ###########################################################################
-# from itertools import chain
 import logging
-from logging.handlers import (
-    TimedRotatingFileHandler as _TRFH,
-    RotatingFileHandler as _RFH
-)
 import math
+from logging.handlers import RotatingFileHandler as _RFH
+from logging.handlers import TimedRotatingFileHandler as _TRFH
 from pathlib import Path
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
 
 # Setup
 ###########################################################################
 class LogLevel:
     """
     ``logging``'s log level wrapper + custom log level
@@ -104,56 +100,57 @@
 def _compress_string_for_print(text: str, max_visible: Optional[int] = 120) -> str:
     """
     Compress the string to be more log-readable
 
     text: str
     max_visible: Maximum text can be printed on screen (Minimum: 5)
     """
-    
+
     if max_visible is None or max_visible <= 5:
         max_visible = 120
-    
+
     text = text.replace("\n", " ") # Remove new line
     # logger.debug(text)
-    
+
     if len(text) <= max_visible:
         return str(text)
     else:
         cut_idx = math.floor((max_visible - 3) / 2)
         temp = f"{text[:cut_idx]}...{text[len(text)-cut_idx:]}"
         return f"{temp} [Len: {len(text)}]"
 
-def compress_for_log(object_, max_visible: Optional[int] = None) -> str:
+
+def compress_for_log(object_: Any, max_visible: Optional[int] = None) -> str:
     """
     Compress the object to be more log-readable
 
     :param object_: Object
     :param max_visible: Maximum objects can be printed on screen
     :returns: Compressed log output
     :rtype: str
     """
-    
+
     if isinstance(object_, list):
         return _compress_list_for_print(object_, max_visible)
-    
+
     elif isinstance(object_, set) or isinstance(object_, tuple):
         return _compress_list_for_print(list(object_), max_visible)
-    
+
     elif isinstance(object_, dict):
         temp = [{k: v} for k, v in object_.items()]
         return _compress_list_for_print(temp, max_visible)
-    
+
     elif isinstance(object_, str):
         return _compress_string_for_print(object_, max_visible)
-    
+
     else:
         try:
             return _compress_string_for_print(str(object_), max_visible)
         except:
-            return object_
+            return object_  # type: ignore
 
 
 # Class
 ###########################################################################
 class _CustomLogger:
     """
     Custom logger [W.I.P]
@@ -228,15 +225,15 @@
             file_handler = logging.FileHandler(self.log_file, mode="a", encoding="utf-8")
             file_handler.setLevel(logging.DEBUG)
             _file_log_format = _log_format
             _file_formatter = logging.Formatter(_file_log_format, datefmt=_date_format)
             file_handler.setFormatter(_file_formatter)
             self._file_handler = file_handler
             self.logger.addHandler(self._file_handler)
-            
+
             if timed_log:
                 ## Time handler (split log every day)
                 time_handler = _TRFH(self.log_folder.joinpath(f"{self.name}_timed.log"),
                                      when="midnight", interval=1, encoding="utf-8")
                 time_handler.setLevel(logging.DEBUG)
                 time_handler.setFormatter(_file_formatter)
                 self._time_handler = time_handler
@@ -256,25 +253,27 @@
                 # Time|LogType|FileName|Function|LineNumber|Message
                 _log_format = "%(asctime)s [%(levelname)5s] %(filename)s:%(funcName)s:%(lineno)3d: %(message)s"
             else:
                 _log_format = log_format
             error_handler = _RFH(self.log_folder.joinpath(f"{self.name}_error.log"),
                                  maxBytes=error_log_size, backupCount=1, encoding="utf-8")
             error_handler.setLevel(logging.ERROR)
-            error_handler.setFormatter(_log_format)
+            error_handler.setFormatter(_log_format)  # type: ignore
             self._error_handler = error_handler
             self.logger.addHandler(self._error_handler)
 
     def __str__(self) -> str:
         return f"{self.__class__.__name__}({self.name})"
     def __repr__(self) -> str:
         return self.__str__()
 
     @staticmethod
-    def _add_logging_level(level_name: str, level_num: int, method_name: str = None):
+    def _add_logging_level(
+        level_name: str, level_num: int, method_name: Optional[str] = None
+    ):
         """
         Comprehensively adds a new logging level to the `logging` module and the
         currently configured logging class.
 
         `level_name` becomes an attribute of the `logging` module with the value
         `level_num`. `method_name` becomes a convenience method for both `logging`
         itself and the class returned by `logging.getLoggerClass()` (usually just
@@ -307,15 +306,15 @@
 
         logging.addLevelName(level_num, level_name)
         setattr(logging, level_name, level_num)
         setattr(logging.getLoggerClass(), method_name, logForLevel)
         setattr(logging, method_name, logToRoot)
 
     def add_log_level(self, level_name: str, level_num: int):
-        __class__._add_logging_level(level_name, level_num)
+        __class__._add_logging_level(level_name, level_num)  # type: ignore
         if level_num < logging.DEBUG:
             self._console_handler.setLevel(level_num)
             self.logger.setLevel(level_num)
 
 
 # Run
 ###########################################################################
```

### Comparing `absfuyu-3.3.0/src/absfuyu/pkg_data/__init__.py` & `absfuyu-3.3.1/src/absfuyu/pkg_data/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-3.3.0/src/absfuyu/pkg_data/chemistry.pkl` & `absfuyu-3.3.1/src/absfuyu/pkg_data/chemistry.pkl`

 * *Files identical despite different names*

### Comparing `absfuyu-3.3.0/src/absfuyu/pkg_data/tarot.pkl` & `absfuyu-3.3.1/src/absfuyu/pkg_data/tarot.pkl`

 * *Files identical despite different names*

### Comparing `absfuyu-3.3.0/src/absfuyu/sort.py` & `absfuyu-3.3.1/src/absfuyu/sort.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# type: ignore
 """
 Absfuyu: Sort
 -------------
 Sort Module
 
 Version: 1.2.4
 Date updated: 20/03/2024 (mm/dd/yyyy)
@@ -20,24 +21,22 @@
     "linear_search",
     "binary_search",
 ]
 
 
 # Library
 ###########################################################################
+import operator
 from collections import Counter
 from itertools import accumulate
-import operator
-from typing import Any, Dict, List, Union, NamedTuple
+from typing import Any, Dict, List, NamedTuple, Union
 
 from deprecated import deprecated
 from deprecated.sphinx import (
-    # versionadded,
-    # versionchanged,
-    deprecated as sphinx_deprecated,
+    deprecated as sphinx_deprecated,  # versionadded,; versionchanged,
 )
 
 from absfuyu.logger import logger
 
 
 # Functions
 ###########################################################################
```

### Comparing `absfuyu-3.3.0/src/absfuyu/tools/converter.py` & `absfuyu-3.3.1/src/absfuyu/tools/converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 """
 Absufyu: Converter
 ------------------
 Convert stuff
 
-Version: 1.2.1
-Date updated: 30/11/2023 (dd/mm/yyyy)
+Version: 1.2.2
+Date updated: 05/04/2024 (dd/mm/yyyy)
 
 Feature:
 --------
 - Text2Chemistry
 - Str2Pixel
 - Base64EncodeDecode
 """
 
-
 # Module level
 ###########################################################################
-__all__ = [
-    "Text2Chemistry", "Str2Pixel", "Base64EncodeDecode"
-]
+__all__ = ["Text2Chemistry", "Str2Pixel", "Base64EncodeDecode"]
 
 
 # Library
 ###########################################################################
 import base64
-from itertools import combinations, chain
 import math
 import re
 import string
+from itertools import chain, combinations
 from typing import Dict, List, Union
 
 from absfuyu.core import CLITextColor
 from absfuyu.logger import logger
 from absfuyu.pkg_data import DataList
 from absfuyu.util import set_min
 from absfuyu.util.pkl import Pickler
@@ -39,106 +36,110 @@
 
 # Class
 ###########################################################################
 class Base64EncodeDecode:
     """
     Encode and decode base64
     """
+
     @staticmethod
     def encode(data: str) -> str:
         return base64.b64encode(data.encode()).decode()
 
     @staticmethod
     def decode(data: str) -> str:
         return base64.b64decode(data).decode()
 
 
 class ChemistryElement:
     """Chemistry Element"""
+
     _VERSION = (1, 1, 0)
-    def __init__(
-            self,
-            name: str,
-            number: int,
-            symbol: str,
-            atomic_mass: float
-        ) -> None:
+
+    def __init__(self, name: str, number: int, symbol: str, atomic_mass: float) -> None:
         """
         name: element name
         number: order in periodic table
         symbol: short symbol of element
         atomic_mass: atomic mass of element
         """
         self.name = name
         self.number = number
         self.symbol = symbol
         self.atomic_mass = atomic_mass
+
     def __str__(self) -> str:
         return self.symbol
+
     def __repr__(self) -> str:
         # return self.symbol
         return f"{self.__class__.__name__}({self.symbol})"
-    
+
     def to_dict(self) -> Dict[str, Union[str, int, float]]:
         """
         Output content to dict
-        
+
         :rtype: dict[str, str | int | float]
         """
         return {
             "name": self.name,
             "number": self.number,
             "symbol": self.symbol,
-            "atomic_mass": self.atomic_mass
+            "atomic_mass": self.atomic_mass,
         }
-    
+
     @classmethod
     def from_dict(cls, data: Dict[str, Union[str, int, float]]) -> "ChemistryElement":
         """
         Convert from ``dict`` data
-        
+
         :param data: Dict data
         :type data: dict[str, str | int | float]
         :rtype: ChemistryElement
         """
         return cls(
-                name=data["name"],
-                number=int(data["number"]),
-                symbol=data["symbol"],
-                atomic_mass=float(data["atomic_mass"])
+            name=data["name"],  # type: ignore
+            number=int(data["number"]),
+            symbol=data["symbol"],  # type: ignore
+            atomic_mass=float(data["atomic_mass"]),
         )
 
+
 class Text2Chemistry:
     def __init__(self) -> None:
         self.data_location = DataList.CHEMISTRY
+
     def __str__(self) -> str:
         return f"{self.__class__.__name__}()"
+
     def __repr__(self) -> str:
         return self.__str__()
-    
+
     def _load_chemistry_data(self) -> List[ChemistryElement]:
         """
         Load chemistry pickle data
         """
-        data: List[dict] = Pickler.load(self.data_location)
+        data: List[dict] = Pickler.load(self.data_location)  # type: ignore
         return [ChemistryElement.from_dict(x) for x in data]
-        
+
     @property
     def unvailable_characters(self):
         """
         Characters that can not be converted (unvailable chemistry symbol)
-        
+
         :rtype: set[str]
         """
         base = set(string.ascii_lowercase)
-        available = set("".join(map(lambda x: x.symbol.lower(), self._load_chemistry_data())))
+        available = set(
+            "".join(map(lambda x: x.symbol.lower(), self._load_chemistry_data()))
+        )
         # logger.debug(base)
         # logger.debug(available)
         return base.difference(available)
-    
+
     def convert(self, text: str) -> List[List[ChemistryElement]]:
         """
         Convert text to chemistry symbol
 
         :param text: desired text
         :type text: str
         :returns: Converted text (empty list when failed to convert)
@@ -147,119 +148,136 @@
         # Check if `text` is a word (without digits)
         is_word_pattern = r"^[a-zA-Z]+$"
         if re.search(is_word_pattern, text) is None:
             logger.error("Convert Failed. Word Only!")
             raise ValueError("Convert Failed. Word Only!")
         for x in self.unvailable_characters:
             if text.find(x) != -1:
-                logger.debug(f"{text} contains unvailable characters: {self.unvailable_characters}")
+                logger.debug(
+                    f"{text} contains unvailable characters: {self.unvailable_characters}"
+                )
                 # raise ValueError(f"Text contains {self.unvailable_character}")
                 return []
-        
+
         # Setup
         text_lower = text.lower()
         data = self._load_chemistry_data()
-        
+
         # List possible elements
         possible_elements: List[ChemistryElement] = []
         for i, letter in enumerate(text_lower):
             for element in data:
-                if element.symbol.lower().startswith(letter): # Check for `element.symbol` starts with `letter`
+                if element.symbol.lower().startswith(
+                    letter
+                ):  # Check for `element.symbol` starts with `letter`
                     # logger.debug(f"{letter} {element}")
-                    if element.symbol.lower().startswith(text_lower[i:i+len(element.symbol)]): # Check for `element.symbol` with len > 1 starts with `letter` of len(element.symbol)
+                    if element.symbol.lower().startswith(
+                        text_lower[i : i + len(element.symbol)]
+                    ):  # Check for `element.symbol` with len > 1 starts with `letter` of len(element.symbol)
                         possible_elements.append(element)
                     # Break when reach last letter in text
                     if letter == text_lower[-1]:
                         break
         logger.debug(possible_elements)
-        if len(possible_elements) < 1: # No possible elements
+        if len(possible_elements) < 1:  # No possible elements
             return []
 
         # temp = []
         # for i in range(min_combination_range, len(text_lower)+1):
         #     comb = combinations(possible_elements, i)
         #     temp.append(comb)
         # possible_combinations = chain(*temp)
-        max_symbol_len = max(map(lambda x: len(x.symbol), possible_elements)) # Max len of `element.symbol`
+        max_symbol_len = max(
+            map(lambda x: len(x.symbol), possible_elements)
+        )  # Max len of `element.symbol`
         min_combination_range = math.ceil(len(text_lower) / max_symbol_len)
         logger.debug(f"Combination range: [{min_combination_range}, {len(text_lower)}]")
-        possible_combinations = chain(*(combinations(possible_elements, i) for i in range(min_combination_range, len(text_lower)+1)))
+        possible_combinations = chain(
+            *(
+                combinations(possible_elements, i)
+                for i in range(min_combination_range, len(text_lower) + 1)
+            )
+        )
         # logger.debug(list(possible_combinations))
-        
+
         output = []
         for comb in possible_combinations:
             merged = "".join(map(lambda x: x.symbol, comb))
             if text_lower == merged.lower():
                 output.append(list(comb))
                 logger.debug(f"Found: {merged}")
 
         return output
 
 
 class Str2Pixel:
     """Convert str into pixel"""
-    PIXEL = u"\u2588"
+
+    PIXEL = "\u2588"
+
     def __init__(
-            self,
-            str_data: str,
-            *,
-            pixel_size: int = 2,
-            pixel_symbol_overwrite: Union[str, None] = None
-        ) -> None:
+        self,
+        str_data: str,
+        *,
+        pixel_size: int = 2,
+        pixel_symbol_overwrite: Union[str, None] = None,
+    ) -> None:
         """
         str_data: Pixel string data (Format: <number_of_pixel><color_code>)
         pixel_size: Pixel size (Default: 2)
         pixel_symbol_overwrite: Overwrite pixel symbol (Default: None)
 
         Example: 50w20b = 50 white pixels and 20 black pixels
         """
         self.data = str_data
         if pixel_symbol_overwrite is None:
-            self.pixel = self.PIXEL * set_min(pixel_size, min_value=1)
+            self.pixel = self.PIXEL * int(set_min(pixel_size, min_value=1))
         else:
             self.pixel = pixel_symbol_overwrite
+
     def __str__(self) -> str:
         return f"{self.__class__.__name__}(pixel={self.pixel})"
+
     def __repr__(self) -> str:
         return self.__str__()
-    
+
     def _extract_pixel(self):
         """Split str_data into corresponding int and str"""
-        num = re.split("[a-zA-Z]", self.data)
-        num = filter(lambda x: x != "", num) # Clean "" in list
-        num = list(map(int, num))
+        num = re.split("[a-zA-Z]", self.data)  # type: ignore
+        num = filter(lambda x: x != "", num)  # type: ignore # Clean "" in list
+        num = list(map(int, num))  # type: ignore
         char = re.split("[0-9]", self.data)
-        char = filter(lambda x: x != "", char)
+        char = filter(lambda x: x != "", char)  # type: ignore
         return [x for y in zip(num, char) for x in y]
 
     def convert(self, line_break: bool = True) -> str:
         """
         Convert data into pixel
-        
+
         :param line_break: add ``\\n`` at the end of line (Default: ``False``)
         :type line_break: bool
         :returns: Converted colored pixels
         :rtype: str
         """
         # Extract pixel
         pixel_map = self._extract_pixel()
 
         # Translation to color
         translate = {
             "w": CLITextColor.WHITE,
-            "b": CLITextColor.BLACK, 
-            "B": CLITextColor.BLUE, 
-            "g": CLITextColor.GRAY, 
-            "G": CLITextColor.GREEN, 
-            "r": CLITextColor.RED, 
-            "R": CLITextColor.DARK_RED, 
-            "m": CLITextColor.MAGENTA, 
-            "y": CLITextColor.YELLOW, 
+            "b": CLITextColor.BLACK,
+            "B": CLITextColor.BLUE,
+            "g": CLITextColor.GRAY,
+            "G": CLITextColor.GREEN,
+            "r": CLITextColor.RED,
+            "R": CLITextColor.DARK_RED,
+            "m": CLITextColor.MAGENTA,
+            "y": CLITextColor.YELLOW,
             "E": CLITextColor.RESET,
-            "N": "\n" # New line
+            "N": "\n",  # New line
         }
 
         # import colorama
         # translate = {
         #     "w": colorama.Fore.WHITE,
         #     "b": colorama.Fore.BLACK,
         #     "B": colorama.Fore.BLUE,
@@ -273,15 +291,15 @@
         #     "N": "\n", # New line
         # }
 
         # Output
         out = ""
         for i, x in enumerate(pixel_map):
             if isinstance(x, str):
-                temp = self.pixel * pixel_map[i-1]
+                temp = self.pixel * pixel_map[i - 1]
                 out += f"{translate[x]}{temp}{translate['E']}"
         if line_break:
             return out + "\n"
         else:
             return out
```

### Comparing `absfuyu-3.3.0/src/absfuyu/tools/keygen.py` & `absfuyu-3.3.1/src/absfuyu/tools/keygen.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """
 Absfuyu: Keygen
 ---------------
 Mod7 product key generator (90's)
 
 This is for educational and informative purposes only.
 
-Version: 2.0.1
-Date updated: 24/11/2023 (dd/mm/yyyy)
+Version: 2.0.2
+Date updated: 05/04/2024 (dd/mm/yyyy)
 """
 
-
 # Module level
 ###########################################################################
 __all__ = [
     "Keygen"
 ]
 
 
@@ -36,15 +35,15 @@
         text = str(text) # Safety convert
         try:
             res = sum(map(int, text)) % 7
             # logger.debug(f"Sum value: {res}")
             return res == 0
         except:
             raise ValueError("Invalid string")
-    
+
     @staticmethod
     def _mod7_gen(
             num_of_digits: int,
             *,
             fillchar: str = "0"
         ) -> str:
         """
@@ -59,40 +58,39 @@
             filled character when `len(generated number)` < `num_of_digits`
         
         Return:
         ---
         str:
             Mod7 number
         """
-        
+
         # Init
         mod7_num: int = 0
-        
+
         # Conditions
         max_value = 10**num_of_digits-1
         mod7_valid = False
         invalid_digits = [0,8,9] # Invalid last digit
-        
+
         # Loop
         while not mod7_valid:
             # Gen num
             mod7_num = random.randint(0, max_value)
-            
+
             # Check last digit
             if int(str(mod7_num)[-1]) in invalid_digits:
                 continue
-            
+
             # Check divide by 7
-            if __class__._is_mod7(mod7_num):
+            if __class__._is_mod7(mod7_num):  # type: ignore
                 mod7_valid = True
-        
+
         # Output
         return str(mod7_num).rjust(num_of_digits, fillchar)
 
-
     @staticmethod
     def mod7_cd_key(fast: bool = False) -> str:
         """
         CD Key generator
 
         Format: ``XXX-XXXXXXX``                              
         
@@ -126,15 +124,15 @@
             part1_num = random.randint(0, 998) # Gen random int from 0 to 998
             # part1_num = random.randint(100,300) # or just use this
             if part1_num not in part1_not_valid_digits:
                 part1 = str(part1_num).rjust(3, "0") # Convert into string
                 part1_valid = True # Break loop
 
         # PART 02
-        part2 = __class__._mod7_gen(num_of_digits=7)
+        part2 = __class__._mod7_gen(num_of_digits=7)  # type: ignore
 
         # OUTPUT
         return f"{part1}-{part2}"
 
     @staticmethod
     def mod7_11_digit_key(fast: bool = False) -> str:
         """
@@ -152,35 +150,35 @@
             (Default: ``False``)
         
         Returns
         -------
         str:
             Mod7 Key
         """
-        
+
         # Fast mode: pre-generated key
         if fast:
             return "0001-0000007"
-        
+
         # PART 01
         part1_valid = False
         part1: str = ""
         while not part1_valid:
             part1_1_num = random.randint(0, 999) # Random 3-digit number
             last_digit_choice = [1, 2] # Choice for last digit
             part1_2_num = int(str(part1_1_num)[-1]) + random.choice(last_digit_choice) # Make last digit
             if part1_2_num > 9: # Check condition then overflow
-                part1_2_num = str(part1_2_num)[-1]
+                part1_2_num = int(str(part1_2_num)[-1])
             part1_str = f"{part1_1_num}{part1_2_num}" # Concat string
             if int(part1_str) < 9991: # Check if < 9991
                 part1 = part1_str.rjust(4, "0")
                 part1_valid = True
 
         # PART 02
-        part2 = __class__._mod7_gen(num_of_digits=7)
+        part2 = __class__._mod7_gen(num_of_digits=7)  # type: ignore
 
         # OUTPUT
         return f"{part1}-{part2}"
 
     @staticmethod
     def mod7_oem_key(fast: bool = False) -> str:
         """
@@ -200,30 +198,30 @@
             (Default: ``False``)
         
         Returns
         -------
         str:
             Mod7 Key
         """
-        
+
         # Fast mode: pre-generated key
         if fast:
             return "00100-OEM-0000007-00000"
-        
+
         # PART ABC
         abc_part = str(random.randint(1, 365)).rjust(3, "0")
 
         # PART YY
         year_choice = ["95", "96", "97", "98", "99", "00", "01", "02"]
         # isleap = [False, True, False, False, False, True, False, False]
         # year_choice = ["95", "96", "97", "98", "99", "00", "01", "02", "03"] # "03" not wotk on win95
         y_part = random.choice(year_choice)
 
         # NUM PART
-        num_part = __class__._mod7_gen(num_of_digits=6)
+        num_part = __class__._mod7_gen(num_of_digits=6)  # type: ignore
 
         # NUM PART 02
         num_part_2 = str(random.randint(0, 99999)).rjust(5, "0")
 
         # OUTPUT
         return f"{abc_part}{y_part}-OEM-0{num_part}-{num_part_2}"
 
@@ -240,19 +238,19 @@
         
         Returns
         -------
         dict:
             Mod7 Key combo
         """
         out = {
-            "CD Key": __class__.mod7_cd_key(fast=fast),
-            "OEM Key": __class__.mod7_oem_key(fast=fast),
-            "11-digit Key": __class__.mod7_11_digit_key(fast=fast)
+            "CD Key": __class__.mod7_cd_key(fast=fast),  # type: ignore
+            "OEM Key": __class__.mod7_oem_key(fast=fast),  # type: ignore
+            "11-digit Key": __class__.mod7_11_digit_key(fast=fast),  # type: ignore
         }
         return out
 
 
 # Run
 ###########################################################################
 if __name__ == "__main__":
     test = Keygen()
-    print(test.mod7_combo())
+    print(test.mod7_combo())
```

### Comparing `absfuyu-3.3.0/src/absfuyu/tools/obfuscator.py` & `absfuyu-3.3.1/src/absfuyu/tools/obfuscator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """
 Absfuyu: Obfuscator
 -------------------
 Obfuscate code
 
-Version: 2.0.1
-Date updated: 26/11/2023 (dd/mm/yyyy)
+Version: 2.0.2
+Date updated: 05/04/2024 (dd/mm/yyyy)
 """
 
-
 # Module level
 ###########################################################################
 __all__ = ["Obfuscator"]
 
 
 # Library
 ###########################################################################
 import base64
 import codecs
 import random
 import zlib
 
-from absfuyu.logger import logger
-from absfuyu.general.generator import Generator as gen, Charset
 from absfuyu.general.data_extension import Text
+from absfuyu.general.generator import Charset
+from absfuyu.general.generator import Generator as gen
+from absfuyu.logger import logger
 
 
 # Class
 ###########################################################################
 class ObfuscatorLibraryList:
     BASE64_ONLY = ["base64"]
     FULL = ["base64", "codecs", "zlib"]
@@ -99,18 +99,18 @@
 
         b64_encode = base64.b64encode(code.encode())
         if self.base64_only:
             output = b64_encode.decode()
         else:
             compressed_data = zlib.compress(b64_encode)
             # log_debug(compressed_data)
-            logger.debug(f"Compressed data: {compressed_data}")
+            logger.debug(f"Compressed data: {compressed_data}")  # type: ignore
             b64_encode_2 = base64.b64encode(compressed_data)
             # log_debug(b64_encode_2)
-            logger.debug(f"Base64 encode 2: {b64_encode_2}")
+            logger.debug(f"Base64 encode 2: {b64_encode_2}")  # type: ignore
             caesar_data = codecs.encode(b64_encode_2.decode(), "rot_13")
             output = caesar_data
 
         logger.debug(f"Output: {output}")
         logger.debug("Code encoded.")
         return output
 
@@ -127,15 +127,15 @@
         b64_decode_codec = f"base64.b64decode('{b64_encode_codec}'.encode())"
         hex = Text(b64_decode_codec).to_hex()
         out = f"eval('{hex}').decode()"
         if raw:
             return hex
         return out
 
-    def _obfuscate_out(self) -> list:
+    def _obfuscate_out(self) -> list:  # type: ignore
         """
         Convert multiple lines of code through multiple transformation
         (base64 -> compress -> base64 -> caesar (13))
 
         Then return a list (obfuscated code) that can
         be print or export into .txt file
         """
```

### Comparing `absfuyu-3.3.0/src/absfuyu/tools/stats.py` & `absfuyu-3.3.1/src/absfuyu/tools/stats.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,22 +89,22 @@
         --------
         >>> test = ListStats([1, 1, 2, 3, 4, 5, 6])
         >>> test.mode()
         [1]
         """
         lst = self
         frequency = ListExt(lst).freq()
-        
-        max_val = max(frequency.values())
+
+        max_val = max(frequency.values())  # type: ignore
         keys = []
-        
-        for k, v in frequency.items():
+
+        for k, v in frequency.items():  # type: ignore
             if v == max_val:
                 keys.append(k)
-        
+
         return keys
 
     def var(self) -> float:
         """
         Variance
         
         Returns
@@ -219,8 +219,8 @@
 
 # Run
 ###########################################################################
 if __name__ == "__main__":
     logger.setLevel(10)
     from rich import print
     test = ListStats([1,8,9,2,3,4,4])
-    print(test.summary())
+    print(test.summary())
```

### Comparing `absfuyu-3.3.0/src/absfuyu/tools/web.py` & `absfuyu-3.3.1/src/absfuyu/tools/web.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """
 Absfuyu: Web
 ------------
 Web, ``request``, ``BeautifulSoup`` stuff
 
-Version: 1.0.1
-Date updated: 24/11/2023 (dd/mm/yyyy)
+Version: 1.0.2
+Date updated: 05/04/2024 (dd/mm/yyyy)
 """
 
-
 # Library
 ###########################################################################
-from bs4 import BeautifulSoup
 import requests
+from bs4 import BeautifulSoup
 
 from absfuyu.logger import logger
 
 
 # Function
 ###########################################################################
 def soup_link(link: str) -> BeautifulSoup:
@@ -42,20 +41,22 @@
         raise SystemExit("Something wrong")
 
 
 def gen_random_commit_msg() -> str:
     """
     Generate random commit message
 
-    :returns: Random commit message
-    :rtype: str
+    Returns
+    -------
+    str
+        Random commit message
     """
     out = soup_link("https://whatthecommit.com/").get_text()[34:-20]
     logger.debug(out)
-    return out
+    return out  # type: ignore
 
 
 # Run
 ###########################################################################
 if __name__ == "__main__":
     logger.setLevel(10)
     gen_random_commit_msg()
```

### Comparing `absfuyu-3.3.0/src/absfuyu/util/__init__.py` & `absfuyu-3.3.1/src/absfuyu/util/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """
 Absufyu: Utilities
 ------------------
 Some random utilities
 
-Version: 1.5.0
-Date updated: 12/03/2024 (dd/mm/yyyy)
+Version: 1.5.1
+Date updated: 05/04/2024 (dd/mm/yyyy)
 """
 
-
 # Library
 ###########################################################################
-from datetime import datetime
 import pkgutil
-# import sys
-from typing import Union
+from datetime import datetime
+from typing import Optional, Union
 
 from absfuyu.logger import logger
 
 
 # Function
 ###########################################################################
 def get_installed_package():
@@ -25,17 +23,17 @@
     Return a list of installed packages
 
     Returns
     -------
     list[str]
         List of installed packages
     """
-    iter_modules = list({module.name for module in pkgutil.iter_modules() if module.ispkg})
-    # builtin = sys.builtin_module_names
-    # return set.union(iter_modules, builtin)
+    iter_modules = list(
+        {module.name for module in pkgutil.iter_modules() if module.ispkg}
+    )
     return sorted(iter_modules)
 
 
 def set_min(
         current_value: Union[int, float],
         *,
         min_value: Union[int, float] = 0,
@@ -135,18 +133,16 @@
     """
     current_value = set_min(current_value, min_value=min_value)
     current_value = set_max(current_value, max_value=max_value)
     return current_value
 
 
 def stop_after_day(
-        year: int = None, 
-        month: int = None, 
-        day: int = None
-    ) -> None:
+    year: Optional[int] = None, month: Optional[int] = None, day: Optional[int] = None
+) -> None:
     """
     Stop working after specified day. 
     Put the function at the begining of the code is recommended.
 
     Parameters
     ----------
     year : int
@@ -165,19 +161,19 @@
     now = datetime.now()
     if year is None:
         year = now.year
     if month is None:
         month = now.month
     if day is None:
         day = now.day + 1
-    
+
     # Logic
     end_date = datetime(year, month, day)
     result = end_date - now
     if result.days < 0:
         raise SystemExit("End of time")
 
 
 # Run
 ###########################################################################
 if __name__ == "__main__":
-    logger.setLevel(10)
+    logger.setLevel(10)
```

### Comparing `absfuyu-3.3.0/src/absfuyu/util/api.py` & `absfuyu-3.3.1/src/absfuyu/util/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,52 @@
-# -*- coding: utf-8 -*-
 """
 Absufyu: API
 ------------
 Fetch data stuff
 
-Version: 1.1.2
-Date updated: 24/11/2023 (dd/mm/yyyy)
+Version: 1.2.0
+Date updated: 05/04/2024 (dd/mm/yyyy)
 """
 
-
 # Module level
 ###########################################################################
 __all__ = [
     "APIRequest",
     "ping_windows",
 ]
 
 
 # Library
 ###########################################################################
 import json
-from pathlib import Path
 import re
 import subprocess
-from typing import List, Optional, Union
+from pathlib import Path
+from typing import List, NamedTuple, Optional, Union
 
 import requests
+from deprecated.sphinx import versionchanged
 
 from absfuyu.logger import logger
 
 
 # Function
 ###########################################################################
-def ping_windows(host: List[str], ping_count: int = 3) -> list:
+class PingResult(NamedTuple):
+    """
+    :param host: Host name/IP
+    :param result: Ping result in ms
+    """
+
+    host: str
+    result: str
+
+
+@versionchanged(version="3.4.0", reason="Change function's return")
+def ping_windows(host: List[str], ping_count: int = 3) -> List[PingResult]:
     """
     Ping web
 
     Parameters
     ----------
     host : list[str]
         List of host to ping
@@ -52,29 +62,31 @@
 
 
     Example:
     --------
     >>> ping_windows(["1.1.1.1", "google.com"])
     ['1.1.1.1 : xxms', 'google.com : xxms']
     """
-    out = []
+    out: List[PingResult] = []
 
     for ip in host:
-        output = subprocess.Popen(
+        output = subprocess.run(
             f"ping {ip.strip()} -n {ping_count}",
-            stdout=subprocess.PIPE,
             encoding="utf-8",
+            capture_output=True,
+            text=True,
         )
+        logger.debug(output)
 
-        data = "".join(output.stdout)
+        data: str = "".join(output.stdout)
         res = re.findall(r"Average = (.*)", data)
         if res:
-            out.append(f"{ip} : {res[0]}")
+            out.append(PingResult(ip, res[0]))
         else:
-            out.append(f"{ip} : FAILED")
+            out.append(PingResult(ip, "FAILED"))
 
     return out
 
 
 # Class
 ###########################################################################
 class APIRequest:
```

### Comparing `absfuyu-3.3.0/src/absfuyu/util/json_method.py` & `absfuyu-3.3.1/src/absfuyu/util/json_method.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """
 Absfuyu: Json Method
 --------------------
 ``.json`` file handling
 
-Version: 1.1.2
-Date updated: 20/03/2024 (dd/mm/yyyy)
+Version: 1.1.3
+Date updated: 05/04/2024 (dd/mm/yyyy)
 """
 
-
 # Module level
 ###########################################################################
 __all__ = ["JsonFile"]
 
 
 # Library
 ###########################################################################
 import json
 from pathlib import Path
-from typing import Optional, Union
+from typing import Any, Dict, Optional, Union
 
 
 # Function
 ###########################################################################
 def load_json(json_file_location: Path):  # Deprecated
     """Load JSON file"""
     print("This function is deprecated as of version 3.0.0")
@@ -51,23 +50,23 @@
         indent: indentation when export to json file
         sort_keys: sort the keys before export to json file
         """
         self.json_file_location = Path(json_file_location)
         self.encoding = encoding
         self.indent = indent
         self.sort_keys = sort_keys
-        self.data = {}
+        self.data: Dict[Any, Any] = {}
 
     def __str__(self) -> str:
         return f"{self.__class__.__name__}({self.json_file_location.name})"
 
     def __repr__(self) -> str:
         return self.__str__()
 
-    def load_json(self) -> dict:
+    def load_json(self) -> Dict[Any, Any]:
         """
         Load ``.json`` file
 
         :returns: ``.json`` data
         :rtype: dict
         """
         with open(self.json_file_location, "r", encoding=self.encoding) as file:
@@ -76,15 +75,15 @@
 
     def save_json(self) -> None:
         """Save ``.json`` file"""
         json_data = json.dumps(self.data, indent=self.indent, sort_keys=self.sort_keys)
         with open(self.json_file_location, "w", encoding=self.encoding) as file:
             file.writelines(json_data)
 
-    def update_data(self, data: dict) -> None:
+    def update_data(self, data: Dict[Any, Any]) -> None:
         """
         Update ``.json`` data without save
 
         :param data: ``.json`` data
         :type data: dict
         """
         self.data = data
```

### Comparing `absfuyu-3.3.0/src/absfuyu/util/lunar.py` & `absfuyu-3.3.1/src/absfuyu/util/lunar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 """
 Absfuyu: Lunar calendar
 -----------------------
 Convert to lunar calendar
 
-Version: 1.0.1
-Date updated: 24/11/2023 (dd/mm/yyyy)
+Version: 1.0.2
+Date updated: 05/04/2024 (dd/mm/yyyy)
 
 Source:
 -------
 Astronomical algorithms from the book "Astronomical Algorithms" by Jean Meeus, 1998
 https://www.informatik.uni-leipzig.de/~duc/amlich/AL.py
 """
 
 # Module level
 ###########################################################################
 __all__ = ["LunarCalendar"]
 
 
 # Library
 ###########################################################################
-from datetime import date, datetime
 import math
-from typing import Union
-
-# from absfuyu.logger import logger
+from datetime import date, datetime
+from typing import Optional, Union
 
 
 # Class
 ###########################################################################
 class LunarCalendar:
     """Lunar Calendar"""
 
@@ -53,17 +51,17 @@
 
     def __repr__(self) -> str:
         return self.__str__()
 
     def _julian_day_from_date(
         self,
         *,
-        overwrite_year: int = None,
-        overwrite_month: int = None,
-        overwrite_day: int = None,
+        overwrite_year: Optional[int] = None,
+        overwrite_month: Optional[int] = None,
+        overwrite_day: Optional[int] = None,
     ) -> int:
         """
         Compute the (integral) Julian day number of `self.date`
 
         i.e., the number of days between 1/1/4713 BC (Julian calendar) and `self.date`.
         """
         day = self.date.day if overwrite_day is None else overwrite_day
@@ -197,28 +195,26 @@
         The time zone if the time difference between local time and UTC: 7.0 for UTC+7:00.
 
         The function returns a number between `0` and `11`.
 
         From the day after March equinox and the 1st major term after March equinox, 0 is returned. After that, return 1, 2, 3 ...
         """
         return int(
-            __class__._sun_longitude(day_number - 0.5 - self.time_zone / 24.0)
-            / math.pi
-            * 6
+            self._sun_longitude(day_number - 0.5 - self.time_zone / 24.0) / math.pi * 6
         )
 
     def _get_new_moon_day(self, k: int) -> int:
         """
         Compute the day of the k-th new moon in the given time zone.
 
         The time zone if the time difference between local time and UTC: 7.0 for UTC+7:00.
         """
-        return int(__class__._new_moon(k) + 0.5 + self.time_zone / 24.0)
+        return int(self._new_moon(k) + 0.5 + self.time_zone / 24.0)
 
-    def _get_lunar_month_11(self, *, overwrite_year: int = None) -> int:
+    def _get_lunar_month_11(self, *, overwrite_year: Optional[int] = None) -> int:
         """
         Find the day that starts the luner month 11
         of the given year for the given time zone.
         """
         # off = self._julian_day_from_date(overwrite_month=12, overwrite_day=31) - 2415021.076998695
         year = self.date.year if overwrite_year is None else overwrite_year
         off = (
@@ -291,15 +287,15 @@
                 lunar_month = diff + 10
                 if diff == leap_month_diff:
                     self._lunar_leap = True
         if lunar_month > 12:
             lunar_month = lunar_month - 12
         if lunar_month >= 11 and diff < 4:
             lunar_year -= 1
-        return __class__(
+        return self.__class__(
             lunar_year, lunar_month, lunar_day, lunar_leap=self._lunar_leap
         )
 
     def to_solar(self):
         """
         Convert a lunar date to the corresponding solar date.
 
@@ -333,15 +329,15 @@
                 # logger.warning("lunar_leap is True")
                 # raise ValueError()
                 return date(1, 1, 1)
             elif self._lunar_leap is True or off >= leapOff:
                 off += 1
         monthStart = self._get_new_moon_day(k + off)
         out = self._julian_day_to_date(monthStart + lunarD - 1)
-        return __class__(out.year, out.month, out.day, lunar_leap=self._lunar_leap)
+        return self.__class__(out.year, out.month, out.day, lunar_leap=self._lunar_leap)
 
     def convert_all(self) -> dict:
         """
         Convert to both lunar and solar
 
         This method has no practical use
 
@@ -405,9 +401,8 @@
         today = datetime.now().date()
         return cls(today.year, today.month, today.day).to_lunar()
 
 
 # Run
 ###########################################################################
 if __name__ == "__main__":
-    # logger.setLevel(10)
     pass
```

### Comparing `absfuyu-3.3.0/src/absfuyu/util/performance.py` & `absfuyu-3.3.1/src/absfuyu/util/performance.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """
 Absfuyu: Performance
 --------------------
 Performance Check
 
-Version: 1.2.2
-Date updated: 20/03/2024 (dd/mm/yyyy)
+Version: 1.2.3
+Date updated: 05/04/2024 (dd/mm/yyyy)
 
 Feature:
 --------
 - measure_performance
 - function_debug
 - retry
 - var_check
 - Checker
 """
 
-
 # Module level
 ###########################################################################
 __all__ = [
     # Wrapper
     "function_debug",
     "measure_performance",
     "retry",
@@ -28,36 +27,31 @@
     # Class
     "Checker",
 ]
 
 
 # Library
 ###########################################################################
+import time
+import tracemalloc
 from functools import wraps
 from inspect import getsource
-from time import perf_counter, sleep
-import tracemalloc
 from typing import Any, Callable, Dict, List, Union
 
-from deprecated import deprecated
-from deprecated.sphinx import (
-    versionadded,
-    versionchanged,
-    deprecated as sphinx_deprecated,
-)
+from deprecated.sphinx import versionadded, versionchanged
 
 from absfuyu.general.data_extension import ListNoDunder
 
 # from absfuyu.logger import logger, LogLevel
 
 
 # Function
 ###########################################################################
 @versionchanged(version="3.2.0", reason="Clean up code")
-def measure_performance(func: Callable) -> Callable:
+def measure_performance(func: Callable) -> Callable:  # type: ignore
     r"""
     Measure performance of a function
 
     Parameters
     ----------
     func : Callable
         A callable function
@@ -86,18 +80,18 @@
         --------------------------------------
     """
 
     @wraps(func)
     def wrapper(*args, **kwargs) -> Any:
         # Performance check
         tracemalloc.start()  # Start memory measure
-        start_time = perf_counter()  # Start time measure
+        start_time = time.perf_counter()  # Start time measure
         output = func(*args, **kwargs)  # Run function and save result into a variable
         current, peak = tracemalloc.get_traced_memory()  # Get memory stats
-        finish_time = perf_counter()  # Get finished time
+        finish_time = time.perf_counter()  # Get finished time
         tracemalloc.stop()  # End memory measure
 
         # Print output
         print(
             f"{'-' * 38}\n"
             f"Function: {func.__name__}\n"
             f"Memory usage:\t\t {current / 10**6:,.6f} MB\n"
@@ -109,15 +103,15 @@
         # Return
         return output
 
     return wrapper
 
 
 @versionadded(version="3.2.0")
-def function_debug(func: Callable) -> Callable:
+def function_debug(func: Callable) -> Callable:  # type: ignore
     """
     Print the function signature and return value
 
     Parameters
     ----------
     func : Callable
         A callable function
@@ -157,15 +151,15 @@
         # logger.debug(f"{func.__name__}() returned {repr(value)}")
         return value
 
     return wrapper
 
 
 @versionadded(version="3.2.0")
-def retry(retries: int = 3, delay: float = 1) -> Callable:
+def retry(retries: int = 3, delay: float = 1) -> Callable:  # type: ignore
     """
     Attempt to call a function, if it fails, try again with a specified delay.
 
     Parameters
     ----------
     retries : int
         The max amount of retries you want for the function call
@@ -199,37 +193,39 @@
     "test()" failed after 3 retries.
     """
 
     # Condition
     if retries < 1 or delay <= 0:
         raise ValueError("retries must be >= 1, delay must be >= 0")
 
-    def decorator(func: Callable) -> Callable:
+    def decorator(func: Callable) -> Callable:  # type: ignore
         @wraps(func)
         def wrapper(*args, **kwargs) -> Any:
             for i in range(1, retries + 1):
                 try:
                     print(f"Running ({i}): {func.__name__}()")
                     return func(*args, **kwargs)
                 except Exception as e:
                     # Break out of the loop if the max amount of retries is exceeded
                     if i == retries:
                         print(f"Error: {repr(e)}.")
                         print(f'"{func.__name__}()" failed after {retries} retries.')
                         break
                     else:
                         print(f"Error: {repr(e)} -> Retrying...")
-                        sleep(delay)  # Add a delay before running the next iteration
+                        time.sleep(
+                            delay
+                        )  # Add a delay before running the next iteration
 
         return wrapper
 
     return decorator
 
 
-def _deprecated_warning(func: Callable):
+def _deprecated_warning(func: Callable):  # type: ignore
     """
     Notice that the function is deprecated and should not be used
 
     Parameters
     ----------
     func : Callable
         A callable function
@@ -244,96 +240,14 @@
         print(f"[WARNING] {func.__name__}() is deprecated")
         value = func(*args, **kwargs)
         return value
 
     return wrapper
 
 
-@deprecated(
-    reason="Implemented into absfuyu.util.performance.Checker()", version="3.2.0"
-)
-@sphinx_deprecated(
-    reason="Implemented into ``absfuyu.util.performance.Checker()``", version="3.2.0"
-)
-def var_check(variable: Any, full: bool = False):  # del soon
-    """
-    Check a variable [Deprecated]
-
-    Parameters
-    ----------
-    variable : Any
-        Variable that needed to check
-
-    full : bool
-        | ``True``: Shows full detail
-        | ``False``: Hides ``dir`` and ``docstring``
-
-
-    Example:
-    --------
-    >>> test = "test"
-    >>> var_check(test)
-    {'value': 'test', 'class': str, 'id': ...}
-    """
-
-    # Check class
-    try:
-        clss = [variable.__name__, type(variable)]
-    except:
-        clss = type(variable)
-
-    output = dict()
-    try:
-        output = {
-            "value": variable,
-            "class": clss,
-            "id": id(variable),
-        }
-    except:
-        return None
-
-    # Docstring
-    try:
-        lc = [  # list of Python data types
-            str,
-            int,
-            float,
-            complex,
-            list,
-            tuple,
-            range,
-            dict,
-            set,
-            frozenset,
-            bool,
-            bytes,
-            bytearray,
-            memoryview,
-            type(None),
-        ]
-        if type(variable) in lc:
-            pass
-        else:
-            docs = variable.__doc__
-            if full:
-                output["docstring"] = docs
-    except:
-        pass
-
-    # Dir
-    try:
-        if full:
-            output["dir"] = ListNoDunder(variable.__dir__())
-    except:
-        pass
-
-    # Output
-    return output
-
-
 # Class
 ###########################################################################
 class Checker:
     """
     Check a variable
 
     Parameters
@@ -349,15 +263,15 @@
     {'name': None, 'value': 'test', 'class': <class 'str'>, 'id': ...}
     """
 
     def __init__(self, variable: Any) -> None:
         self.item_to_check = variable
 
     def __str__(self) -> str:
-        return self.item_to_check.__str__()
+        return self.item_to_check.__str__()  # type: ignore
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.item_to_check})"
 
     @property
     def name(self) -> Union[Any, None]:
         """``__name__`` of variable (if any)"""
@@ -370,15 +284,15 @@
     def value(self) -> Any:
         """Value of the variable"""
         return self.item_to_check
 
     @property
     def docstring(self) -> Union[str, None]:
         """``__doc__`` of variable (if any)"""
-        return self.item_to_check.__doc__
+        return self.item_to_check.__doc__  # type: ignore
 
     @property
     def class_(self) -> Any:
         """``class()`` of variable"""
         return type(self.item_to_check)
 
     @property
```

### Comparing `absfuyu-3.3.0/src/absfuyu/util/pkl.py` & `absfuyu-3.3.1/src/absfuyu/util/pkl.py`

 * *Files identical despite different names*

### Comparing `absfuyu-3.3.0/src/absfuyu/util/zipped.py` & `absfuyu-3.3.1/src/absfuyu/util/zipped.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 __all__ = [
     "Zipper"
 ]
 
 
 # Library
 ###########################################################################
-from pathlib import Path
 import shutil
-from typing import Union
 import zipfile
+from pathlib import Path
+from typing import Union
 
 from absfuyu.logger import logger
 
 
 ###########################################################################
 class Zipper:
     """Zip file or folder"""
@@ -79,8 +79,8 @@
             except OSError as e:
                 logger.error(f"Error: {e.filename} - {e.strerror}.")
 
 
 # Run
 ###########################################################################
 if __name__ == "__main__":
-    logger.setLevel(10)
+    logger.setLevel(10)
```

### Comparing `absfuyu-3.3.0/src/absfuyu/version.py` & `absfuyu-3.3.1/src/absfuyu/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """
 Absfuyu: Version
 ----------------
 Package versioning module
 
-Version: 2.0.5
-Date updated: 14/03/2024 (dd/mm/yyyy)
+Version: 2.0.6
+Date updated: 05/04/2024 (dd/mm/yyyy)
 """
 
-
 # Module level
 ###########################################################################
 __all__ = [
     # Version
     "__version__",
     # Options
     "ReleaseOption",
@@ -27,15 +26,15 @@
 import json
 import subprocess
 from typing import List
 from urllib.error import URLError
 from urllib.request import Request, urlopen
 
 from absfuyu import __title__
-from absfuyu.config import ABSFUYU_CONFIG, Config
+from absfuyu.config import ABSFUYU_CONFIG, Config, VersionDictFormat
 from absfuyu.logger import logger
 
 
 # Class
 ###########################################################################
 class ReleaseOption:
     """
@@ -43,32 +42,32 @@
     """
 
     MAJOR: str = "major"
     MINOR: str = "minor"
     PATCH: str = "patch"
 
     # @staticmethod
-    def all_option() -> List[str]:
+    def all_option() -> List[str]:  # type: ignore
         """Return a list of release options"""
-        return [__class__.MAJOR, __class__.MINOR, __class__.PATCH]
+        return [__class__.MAJOR, __class__.MINOR, __class__.PATCH]  # type: ignore
 
 
 class ReleaseLevel:
     """
     ``FINAL``, ``DEV``, ``RC``
     """
 
     FINAL: str = "final"
     DEV: str = "dev"
     RC: str = "rc"  # Release candidate
 
     # @staticmethod
-    def all_level() -> List[str]:
+    def all_level() -> List[str]:  # type: ignore
         """Return a list of release levels"""
-        return [__class__.FINAL, __class__.DEV, __class__.RC]
+        return [__class__.FINAL, __class__.DEV, __class__.RC]  # type: ignore
 
 
 class Version:
     """Version"""
 
     def __init__(
         self,
@@ -307,25 +306,25 @@
         package_name: Name of the package
         config_file_handler: Config file handler
         """
 
         # Get config
         try:
             self.config_file = config_file_handler
-            version: dict = self.config_file.version
+            version = self.config_file.version
         except Exception as e:
             logger.error("Can't load config file")
             raise ValueError(e)
 
         # Set version
-        self.major: int = version.get("major")
-        self.minor: int = version.get("minor")
-        self.patch: int = version.get("patch")
-        self.release_level: str = version.get("release_level")
-        self.serial: int = version.get("serial")
+        self.major: int = version["major"]
+        self.minor: int = version["minor"]
+        self.patch: int = version["patch"]
+        self.release_level: str = version["release_level"]
+        self.serial: int = version["serial"]
 
         # Set package name
         self.package_name = package_name
 
     # Check for update
     @staticmethod
     def _fetch_data_from_server(link: str):
@@ -357,15 +356,15 @@
         return version
 
     def _load_data_from_json(self, json_link: str) -> dict:
         """
         Load data from api then convert to json
         """
         json_file: str = self._fetch_data_from_server(json_link)
-        return json.loads(json_file)
+        return json.loads(json_file)  # type: ignore
 
     def _get_latest_version(self) -> str:
         """
         Get latest version from PyPI's API
         """
         link = f"https://pypi.org/pypi/{self.package_name}/json"
         ver: str = self._load_data_from_json(link)["info"]["version"]
@@ -437,15 +436,15 @@
 
         Returns
         -------
         str
             Bumped version string
         """
         self.bump(option=option, channel=channel)  # Bump
-        self.config_file.update_version(self.to_dict())  # Save to config
+        self.config_file.update_version(self.to_dict())  # type: ignore # Save to config
         return self.version
 
     # Release package
     def _release_to_pypi(
         self,
         option: str = ReleaseOption.PATCH,
         channel: str = ReleaseLevel.FINAL,
```

### Comparing `absfuyu-3.3.0/src/absfuyu.egg-info/PKG-INFO` & `absfuyu-3.3.1/src/absfuyu.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,13 @@
 Metadata-Version: 2.1
 Name: absfuyu
-Version: 3.3.0
+Version: 3.3.1
 Summary: A small collection of code
 Author: somewhatcold (AbsoluteWinter)
 License: MIT License
-        
-        Copyright (c) 2022-2024 AbsoluteWinter
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
 Project-URL: Homepage, https://github.com/AbsoluteWinter/absfuyu-public
 Project-URL: Documentation, https://absolutewinter.github.io/absfuyu
 Project-URL: Repository, https://github.com/AbsoluteWinter/absfuyu-public
 Project-URL: Issues, https://github.com/AbsoluteWinter/absfuyu-public/issues
 Keywords: utilities
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -46,101 +25,93 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bs4
+Requires-Dist: click>=8.0.0
+Requires-Dist: colorama
 Requires-Dist: Deprecated
+Requires-Dist: importlib_resources; python_version < "3.10"
 Requires-Dist: python-dateutil
 Requires-Dist: requests
-Requires-Dist: unidecode
 Requires-Dist: tomli>=1.1.0; python_version < "3.11"
 Requires-Dist: typing_extensions>=4.0.1; python_version < "3.11"
-Requires-Dist: importlib_resources; python_version < "3.10"
-Provides-Extra: full
-Requires-Dist: pandas; extra == "full"
-Requires-Dist: rich; extra == "full"
-Requires-Dist: click>=8.0.0; extra == "full"
-Requires-Dist: numpy; extra == "full"
-Requires-Dist: absfuyu-res; extra == "full"
-Requires-Dist: colorama>=0.4; extra == "full"
+Requires-Dist: unidecode
 Provides-Extra: res
 Requires-Dist: absfuyu-res; extra == "res"
 Provides-Extra: absfuyu-res
 Requires-Dist: absfuyu-res; extra == "absfuyu-res"
-Provides-Extra: rich
-Requires-Dist: rich; extra == "rich"
+Provides-Extra: full
+Requires-Dist: absfuyu-res; extra == "full"
+Requires-Dist: numpy; extra == "full"
+Requires-Dist: rich; extra == "full"
+Requires-Dist: pandas; extra == "full"
 Provides-Extra: beautiful
 Requires-Dist: rich; extra == "beautiful"
 Provides-Extra: dev
+Requires-Dist: sphinx>=7.0.0; extra == "dev"
+Requires-Dist: twine>=3.7.1; extra == "dev"
 Requires-Dist: rich; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
 Requires-Dist: sphinx_rtd_theme; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: black; extra == "dev"
-Requires-Dist: click>=8.0.0; extra == "dev"
-Requires-Dist: coverage; extra == "dev"
-Requires-Dist: twine>=3.7.1; extra == "dev"
-Requires-Dist: sphinx>=7.0.0; extra == "dev"
-Requires-Dist: colorama>=0.4; extra == "dev"
-Requires-Dist: build; extra == "dev"
-Requires-Dist: pytest>=6.2.5; extra == "dev"
+Requires-Dist: pytest>=7.0.0; extra == "dev"
+Provides-Extra: rich
+Requires-Dist: rich; extra == "rich"
+Provides-Extra: numpy
+Requires-Dist: numpy; extra == "numpy"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
-Requires-Dist: colorama>=0.4; extra == "extra"
-Requires-Dist: click>=8.0.0; extra == "extra"
 Requires-Dist: numpy; extra == "extra"
-Provides-Extra: click
-Requires-Dist: click>=8.0.0; extra == "click"
-Provides-Extra: cli
-Requires-Dist: colorama>=0.4; extra == "cli"
-Requires-Dist: click>=8.0.0; extra == "cli"
-Provides-Extra: colorama
-Requires-Dist: colorama>=0.4; extra == "colorama"
-Provides-Extra: numpy
-Requires-Dist: numpy; extra == "numpy"
 Provides-Extra: pandas
 Requires-Dist: pandas; extra == "pandas"
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Provides-Extra: black
 Requires-Dist: black; extra == "black"
-Provides-Extra: coverage
-Requires-Dist: coverage; extra == "coverage"
 Provides-Extra: twine
 Requires-Dist: twine>=3.7.1; extra == "twine"
 Provides-Extra: pytest
-Requires-Dist: pytest>=6.2.5; extra == "pytest"
+Requires-Dist: pytest>=7.0.0; extra == "pytest"
+Provides-Extra: pytest-cov
+Requires-Dist: pytest-cov; extra == "pytest-cov"
 Provides-Extra: sphinx
 Requires-Dist: sphinx>=7.0.0; extra == "sphinx"
 Provides-Extra: sphinx-rtd-theme
 Requires-Dist: sphinx_rtd_theme; extra == "sphinx-rtd-theme"
+Provides-Extra: mypy
+Requires-Dist: mypy; extra == "mypy"
 Provides-Extra: all
-Requires-Dist: pandas; extra == "all"
-Requires-Dist: colorama>=0.4; extra == "all"
+Requires-Dist: numpy; extra == "all"
+Requires-Dist: sphinx>=7.0.0; extra == "all"
+Requires-Dist: absfuyu-res; extra == "all"
+Requires-Dist: twine>=3.7.1; extra == "all"
 Requires-Dist: rich; extra == "all"
+Requires-Dist: build; extra == "all"
+Requires-Dist: mypy; extra == "all"
+Requires-Dist: pytest>=7.0.0; extra == "all"
+Requires-Dist: pandas; extra == "all"
 Requires-Dist: sphinx_rtd_theme; extra == "all"
 Requires-Dist: black; extra == "all"
-Requires-Dist: click>=8.0.0; extra == "all"
-Requires-Dist: coverage; extra == "all"
-Requires-Dist: twine>=3.7.1; extra == "all"
-Requires-Dist: absfuyu-res; extra == "all"
-Requires-Dist: sphinx>=7.0.0; extra == "all"
-Requires-Dist: numpy; extra == "all"
-Requires-Dist: build; extra == "all"
-Requires-Dist: pytest>=6.2.5; extra == "all"
+Requires-Dist: pytest-cov; extra == "all"
 
 <div align="center">
 	<h1 align="center">
 		<img src="https://github.com/AbsoluteWinter/AbsoluteWinter.github.io/blob/main/absfuyu/images/repository-image-crop.png?raw=true" alt="absfuyu"/>
 	</h1>
 	<p align="center">
-		<a href="https://pypi.org/project/absfuyu/"><img src="https://img.shields.io/pypi/pyversions/absfuyu?style=flat-square" alt="PyPI Supported Versions"/></a>
-		<a href="https://pypi.org/project/absfuyu/"><img src="https://img.shields.io/pypi/dm/absfuyu?style=flat-square" alt="pypi"/></a>
-		<a href="https://pypi.org/project/absfuyu/"><img src="https://img.shields.io/pypi/v/absfuyu?style=flat-square" /></a>
-		<a><img src="https://img.shields.io/badge/license-MIT-blue?style=flat-square" /></a>
+		<a href="https://pypi.org/project/absfuyu/"><img src="https://img.shields.io/pypi/pyversions/absfuyu?style=flat-square&logo=python" alt="PyPI Supported Versions"/></a>
+		<a href="https://pypi.org/project/absfuyu/"><img src="https://img.shields.io/pypi/dm/absfuyu?style=flat-square&color=blue" alt="pypi"/></a>
+		<a href="https://pypi.org/project/absfuyu/"><img src="https://img.shields.io/pypi/v/absfuyu?style=flat-square&logo=pypi" /></a>
+		<a><img src="https://img.shields.io/badge/style-black-blue?style=flat-square"/></a>
+		<a><img src="https://img.shields.io/pypi/l/absfuyu?style=flat-square&logo=github&color=blue"/></a>
 	</p>
 </div>
 
 
 ---
 
 ## **SUMMARY:**
```

### Comparing `absfuyu-3.3.0/src/absfuyu.egg-info/SOURCES.txt` & `absfuyu-3.3.1/src/absfuyu.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 src/absfuyu/config/__init__.py
 src/absfuyu/config/config.json
 src/absfuyu/extensions/__init__.py
 src/absfuyu/extensions/beautiful.py
 src/absfuyu/extensions/dev/__init__.py
 src/absfuyu/extensions/dev/password_hash.py
 src/absfuyu/extensions/dev/passwordlib.py
-src/absfuyu/extensions/dev/pkglib.py
 src/absfuyu/extensions/dev/project_starter.py
 src/absfuyu/extensions/dev/shutdownizer.py
 src/absfuyu/extensions/extra/__init__.py
 src/absfuyu/extensions/extra/data_analysis.py
 src/absfuyu/fun/WGS.py
 src/absfuyu/fun/__init__.py
 src/absfuyu/fun/tarot.py
```

### Comparing `absfuyu-3.3.0/src/absfuyu.egg-info/requires.txt` & `absfuyu-3.3.1/src/absfuyu.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 bs4
+click>=8.0.0
+colorama
 Deprecated
 python-dateutil
 requests
 unidecode
 
 [:python_version < "3.10"]
 importlib_resources
@@ -11,84 +13,71 @@
 tomli>=1.1.0
 typing_extensions>=4.0.1
 
 [absfuyu-res]
 absfuyu-res
 
 [all]
-pandas
-colorama>=0.4
+numpy
+sphinx>=7.0.0
+absfuyu-res
+twine>=3.7.1
 rich
+build
+mypy
+pytest>=7.0.0
+pandas
 sphinx_rtd_theme
 black
-click>=8.0.0
-coverage
-twine>=3.7.1
-absfuyu-res
-sphinx>=7.0.0
-numpy
-build
-pytest>=6.2.5
+pytest-cov
 
 [beautiful]
 rich
 
 [black]
 black
 
 [build]
 build
 
-[cli]
-colorama>=0.4
-click>=8.0.0
-
-[click]
-click>=8.0.0
-
-[colorama]
-colorama>=0.4
-
-[coverage]
-coverage
-
 [dev]
+sphinx>=7.0.0
+twine>=3.7.1
 rich
+build
+mypy
 sphinx_rtd_theme
+pytest-cov
 black
-click>=8.0.0
-coverage
-twine>=3.7.1
-sphinx>=7.0.0
-colorama>=0.4
-build
-pytest>=6.2.5
+pytest>=7.0.0
 
 [extra]
 pandas
-colorama>=0.4
-click>=8.0.0
 numpy
 
 [full]
-pandas
-rich
-click>=8.0.0
-numpy
 absfuyu-res
-colorama>=0.4
+numpy
+rich
+pandas
+
+[mypy]
+mypy
 
 [numpy]
 numpy
 
 [pandas]
 pandas
 
 [pytest]
-pytest>=6.2.5
+pytest>=7.0.0
+
+[pytest-cov]
+pytest-cov
 
 [res]
 absfuyu-res
 
 [rich]
 rich
```

### Comparing `absfuyu-3.3.0/tests/test_DictExt.py` & `absfuyu-3.3.1/tests/test_DictExt.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 """
 Test: DictExt
 
-Version: 1.3.0
-Date updated: 20/03/2024 (dd/mm/yyyy)
+Version: 1.3.1
+Date updated: 22/03/2024 (dd/mm/yyyy)
 """
 
-
-# Library
-###########################################################################
 import pytest
 
-from absfuyu.general.data_extension import DictExt, DictAnalyzeResult
+from absfuyu.general.data_extension import DictAnalyzeResult, DictExt
 
 
-# Test
-###########################################################################
 @pytest.fixture
 def example():
     return DictExt({
         "Line 1": 99,
         "Line 2": 50
     })
 
@@ -26,33 +21,34 @@
 def example_2():
     return DictExt({
         "Line 1": 99,
         "Line 2": "test"
     })
 
 
-# analyze
-def test_analyze(example: DictExt):
-    # assert example.analyze() == {'max_value': 99, 'min_value': 50, 'max': [('Line 1', 99)], 'min': [('Line 2', 50)]}
-    assert example.analyze() == DictAnalyzeResult(99, 50, [('Line 1', 99)], [('Line 2', 50)])
-
-def test_analyze_2(example_2: DictExt):
-    """When values are not int or float"""
-    try:
-        example_2.analyze()
-    except:
-        assert True
-
-
-# swap
-def test_swap(example: DictExt):
-    assert example.swap_items() == {99: 'Line 1', 50: 'Line 2'}
-
-
-# apply
-def test_apply(example: DictExt):
-    """Values"""
-    assert example.apply(str) == {'Line 1': '99', 'Line 2': '50'}
-
-def test_apply_2():
-    """Keys"""
-    assert DictExt({1: 1}).apply(str, apply_to_value=False) == {'1': 1}
+@pytest.mark.data_extension
+class TestDictExt:
+    # analyze
+    def test_analyze(self, example: DictExt) -> None:
+        # assert example.analyze() == {'max_value': 99, 'min_value': 50, 'max': [('Line 1', 99)], 'min': [('Line 2', 50)]}
+        assert example.analyze() == DictAnalyzeResult(
+            99, 50, [("Line 1", 99)], [("Line 2", 50)]
+        )
+
+    def test_analyze_error(self, example_2: DictExt) -> None:
+        """When values are not int or float"""
+        with pytest.raises(ValueError) as excinfo:
+            example_2.analyze()
+        assert str(excinfo.value)
+
+    # swap
+    def test_swap(self, example: DictExt) -> None:
+        assert example.swap_items() == {99: "Line 1", 50: "Line 2"}
+
+    # apply
+    def test_apply(self, example: DictExt) -> None:
+        """Values"""
+        assert example.apply(str) == {"Line 1": "99", "Line 2": "50"}
+
+    def test_apply_2(self) -> None:
+        """Keys"""
+        assert DictExt({1: 1}).apply(str, apply_to_value=False) == {"1": 1}
```

### Comparing `absfuyu-3.3.0/tests/test_config.py` & `absfuyu-3.3.1/tests/test_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,65 +1,58 @@
 """
 Test: Config
 
-Version: 2.0.2
-Date updated: 14/03/2024 (dd/mm/yyyy)
+Version: 2.0.3
+Date updated: 22/03/2024 (dd/mm/yyyy)
 """
 
-
-# Library
-###########################################################################
 import random
 
 import pytest
 
 from absfuyu.config import ABSFUYU_CONFIG, Setting
 
 
-# Test
-###########################################################################
-
 # Setting
 def test_from_dict():
     test = Setting.from_dict({
         "test": {
             "default": False,
             "help": "HELP",
             "value": True
         }
     })
     assert True
 
 
 # Config
-def test_add_and_del_setting():
-    # Make random name
-    name = f"test_add_setting_{random.randint(100_000, 999_999)}"
-
-    # Test add
-    old = len(ABSFUYU_CONFIG.settings)
-    ABSFUYU_CONFIG.add_setting(name, True, True)
-    new = len(ABSFUYU_CONFIG.settings)
-    add_result = old < new
-
-    # Test del
-    ABSFUYU_CONFIG.del_setting(name)
-    new2 = len(ABSFUYU_CONFIG.settings)
-    del_result = old == new2
-
-    # Output
-    assert all([add_result, del_result])
-
-
-def test_toggle_setting():
-    setting = "test"
-    test_before = ABSFUYU_CONFIG._get_setting(setting).value
-    ABSFUYU_CONFIG.toggle_setting(setting)
-    test_after = ABSFUYU_CONFIG._get_setting(setting).value
-    ABSFUYU_CONFIG.toggle_setting(setting)  # Back to original value
-    assert test_before != test_after
-
-
-def test_reset_config():
-    ABSFUYU_CONFIG.reset_config()
-    test = [setting.value == setting.default for setting in ABSFUYU_CONFIG.settings]
-    assert all(test)
+class TestConfig:
+    def test_add_and_del_setting(self) -> None:
+        # Make random name
+        name = f"test_add_setting_{random.randint(100_000, 999_999)}"
+
+        # Test add
+        old = len(ABSFUYU_CONFIG.settings)
+        ABSFUYU_CONFIG.add_setting(name, True, True)
+        new = len(ABSFUYU_CONFIG.settings)
+        add_result = old < new
+
+        # Test del
+        ABSFUYU_CONFIG.del_setting(name)
+        new2 = len(ABSFUYU_CONFIG.settings)
+        del_result = old == new2
+
+        # Output
+        assert all([add_result, del_result])
+
+    def test_toggle_setting(self) -> None:
+        setting = "test"
+        test_before = ABSFUYU_CONFIG._get_setting(setting).value
+        ABSFUYU_CONFIG.toggle_setting(setting)
+        test_after = ABSFUYU_CONFIG._get_setting(setting).value
+        ABSFUYU_CONFIG.toggle_setting(setting)  # Back to original value
+        assert test_before != test_after
+
+    def test_reset_config(self) -> None:
+        ABSFUYU_CONFIG.reset_config()
+        test = [setting.value == setting.default for setting in ABSFUYU_CONFIG.settings]
+        assert all(test)
```

### Comparing `absfuyu-3.3.0/tests/test_data_analysis.py` & `absfuyu-3.3.1/tests/test_data_analysis.py`

 * *Files identical despite different names*

### Comparing `absfuyu-3.3.0/tests/test_everything.py` & `absfuyu-3.3.1/tests/test_everything.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,105 +1,119 @@
 """
 Test: Everything
 
-Version: 1.1.19
-Date updated: 14/03/2024 (dd/mm/yyyy)
+Version: 1.1.20
+Date updated: 05/04/2024 (dd/mm/yyyy)
 """
 
-
 # Library
 ###########################################################################
 import pytest
 
 from absfuyu import everything as ab
+from absfuyu.config import (
+    _SPACE_REPLACE,
+    ABSFUYU_CONFIG,
+    Config,
+    ConfigFormat,
+    Setting,
+    SettingDictFormat,
+    VersionDictFormat,
+)
 
 # --- Loading test --------------------------------------------------------
 # from absfuyu.core import *
 from absfuyu.core import (
-    ModulePackage, ModuleList,
-    Color, CLITextColor,
-    CORE_PATH, CONFIG_PATH, DATA_PATH
+    CONFIG_PATH,
+    CORE_PATH,
+    DATA_PATH,
+    CLITextColor,
+    Color,
+    ModuleList,
+    ModulePackage,
 )
-# from absfuyu.logger import *
-from absfuyu.logger import logger, LogLevel, compress_for_log
-from absfuyu.sort import (
-    selection_sort, insertion_sort,
-    alphabetAppear,
-    linear_search, binary_search
-)
-from absfuyu.version import (
-    __version__,
-    Version, PkgVersion, Bumper,
-    ReleaseLevel, ReleaseOption,
-    _AbsfuyuPackage
-)
-
-# --- Sub-package ---
-from absfuyu.general import Dummy, ClassBase
-from absfuyu.general.content import ContentLoader, Content, LoadedContent # Has unidecode
-from absfuyu.general.data_extension import Text, IntNumber, ListExt, DictExt
-from absfuyu.general.generator import Charset, Generator
-from absfuyu.general.human import BloodType, Human, Person # Has python-dateutil
-
-from absfuyu.config import (
-    ABSFUYU_CONFIG, Config, Setting, _SPACE_REPLACE,
-    SettingDictFormat, VersionDictFormat, ConfigFormat
-)
-
 from absfuyu.extensions import *
-from absfuyu.extensions.beautiful import beautiful_output, demo # Has rich
+from absfuyu.extensions.beautiful import beautiful_output, demo  # Has rich
 from absfuyu.extensions.extra import *
-from absfuyu.extensions.extra.data_analysis import ( # Has pandas, numpy
-    summary, equalize_df, compare_2_list, rename_with_dict,
+from absfuyu.extensions.extra.data_analysis import (  # Has pandas, numpy
+    CityData,
+    DataAnalystDataFrame,
+    MatplotlibFormatString,
     PLTFormatString,
+    SplittedDF,
     _DictToAtrr,
-    MatplotlibFormatString,
-    DataAnalystDataFrame, CityData, SplittedDF
+    compare_2_list,
+    equalize_df,
+    rename_with_dict,
+    summary,
 )
-
-from absfuyu.fun import zodiac_sign, im_bored, force_shutdown, happy_new_year
+from absfuyu.fun import force_shutdown, happy_new_year, im_bored, zodiac_sign
 from absfuyu.fun.tarot import Tarot, TarotCard
 from absfuyu.fun.WGS import WGS
-
 from absfuyu.game import game_escapeLoop, game_RockPaperScissors
 from absfuyu.game.sudoku import Sudoku
 from absfuyu.game.tictactoe import *
-from absfuyu.game.wordle import Wordle # Has requests
+from absfuyu.game.wordle import Wordle  # Has requests
 
-from absfuyu.pkg_data import PkgData, PACKAGE_DATA, DataList
+# --- Sub-package ---
+from absfuyu.general import ClassBase, Dummy
+from absfuyu.general.content import (  # Has unidecode
+    Content,
+    ContentLoader,
+    LoadedContent,
+)
+from absfuyu.general.data_extension import DictExt, IntNumber, ListExt, Text
+from absfuyu.general.generator import Charset, Generator
+from absfuyu.general.human import BloodType, Human, Person  # Has python-dateutil
 
+# from absfuyu.logger import *
+from absfuyu.logger import LogLevel, compress_for_log, logger
+from absfuyu.pkg_data import PACKAGE_DATA, DataList, PkgData
+from absfuyu.sort import (
+    alphabetAppear,
+    binary_search,
+    insertion_sort,
+    linear_search,
+    selection_sort,
+)
 from absfuyu.tools import *
 from absfuyu.tools.converter import (
-    ChemistryElement, Text2Chemistry, 
-    Str2Pixel, 
-    Base64EncodeDecode
+    Base64EncodeDecode,
+    ChemistryElement,
+    Str2Pixel,
+    Text2Chemistry,
 )
 from absfuyu.tools.keygen import Keygen
 from absfuyu.tools.obfuscator import Obfuscator, ObfuscatorLibraryList
 from absfuyu.tools.stats import ListStats
-from absfuyu.tools.web import soup_link, gen_random_commit_msg # Has bs4, requests
-
+from absfuyu.tools.web import gen_random_commit_msg, soup_link  # Has bs4, requests
 from absfuyu.util import (
-    get_installed_package, 
-    set_max, set_min, set_min_max, 
-    stop_after_day
+    get_installed_package,
+    set_max,
+    set_min,
+    set_min_max,
+    stop_after_day,
 )
-from absfuyu.util.api import APIRequest, ping_windows # Has requests
+from absfuyu.util.api import APIRequest, ping_windows  # Has requests
 from absfuyu.util.json_method import JsonFile
 from absfuyu.util.lunar import LunarCalendar
 from absfuyu.util.path import Directory, SaveFileAs
-from absfuyu.util.performance import (
-    measure_performance, retry, function_debug,
-    Checker,
-    var_check,
-)
+from absfuyu.util.performance import Checker, function_debug, measure_performance, retry
 from absfuyu.util.pkl import Pickler
 from absfuyu.util.zipped import Zipper
-
+from absfuyu.version import (
+    Bumper,
+    PkgVersion,
+    ReleaseLevel,
+    ReleaseOption,
+    Version,
+    __version__,
+    _AbsfuyuPackage,
+)
 
 # Test
 ###########################################################################
 # def test_ev():
 #     assert ab.__IS_EVERYTHING is True
 
 def test_everything():
-    assert True
+    assert True
```

### Comparing `absfuyu-3.3.0/tests/test_fun.py` & `absfuyu-3.3.1/tests/test_fun.py`

 * *Files identical despite different names*

### Comparing `absfuyu-3.3.0/tests/test_logger.py` & `absfuyu-3.3.1/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `absfuyu-3.3.0/tests/test_obfuscator.py` & `absfuyu-3.3.1/tests/test_obfuscator.py`

 * *Files identical despite different names*

### Comparing `absfuyu-3.3.0/tests/test_passwordlib.py` & `absfuyu-3.3.1/tests/test_passwordlib.py`

 * *Files identical despite different names*

### Comparing `absfuyu-3.3.0/tests/test_path.py` & `absfuyu-3.3.1/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `absfuyu-3.3.0/tests/test_util.py` & `absfuyu-3.3.1/tests/test_util.py`

 * *Files identical despite different names*

