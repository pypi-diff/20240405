# Comparing `tmp/encommon-0.7.3.tar.gz` & `tmp/encommon-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encommon-0.7.3.tar", last modified: Thu Apr  4 05:11:00 2024, max compression
+gzip compressed data, was "encommon-0.7.4.tar", last modified: Fri Apr  5 00:13:03 2024, max compression
```

## Comparing `encommon-0.7.3.tar` & `encommon-0.7.4.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-04 05:11:00.050277 encommon-0.7.3/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1071 2024-03-20 05:52:00.000000 encommon-0.7.3/LICENSE
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       32 2023-12-31 23:18:53.000000 encommon-0.7.3/MANIFEST.in
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2671 2024-04-04 05:11:00.050277 encommon-0.7.3/PKG-INFO
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2177 2024-03-31 14:52:08.000000 encommon-0.7.3/README.md
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-04 05:11:00.047277 encommon-0.7.3/encommon/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2024-04-02 23:01:55.000000 encommon-0.7.3/encommon/__init__.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-04 05:11:00.047277 encommon-0.7.3/encommon/config/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      710 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/config/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2041 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/config/common.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4743 2024-04-04 05:08:51.000000 encommon-0.7.3/encommon/config/config.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2313 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/config/files.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)    13973 2024-04-04 05:08:51.000000 encommon-0.7.3/encommon/config/logger.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1816 2024-04-04 05:08:51.000000 encommon-0.7.3/encommon/config/params.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2433 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/config/paths.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-04 05:11:00.048277 encommon-0.7.3/encommon/config/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-02 23:01:55.000000 encommon-0.7.3/encommon/config/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      731 2024-04-02 23:01:55.000000 encommon-0.7.3/encommon/config/test/test_common.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3327 2024-04-04 05:08:51.000000 encommon-0.7.3/encommon/config/test/test_config.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2292 2024-04-04 05:08:51.000000 encommon-0.7.3/encommon/config/test/test_files.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4740 2024-04-02 23:01:55.000000 encommon-0.7.3/encommon/config/test/test_logger.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2101 2024-04-04 05:08:51.000000 encommon-0.7.3/encommon/config/test/test_paths.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      880 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/conftest.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-04 05:11:00.048277 encommon-0.7.3/encommon/crypts/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      318 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/crypts/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3500 2024-04-04 05:08:51.000000 encommon-0.7.3/encommon/crypts/crypts.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3103 2024-04-04 05:08:51.000000 encommon-0.7.3/encommon/crypts/hashes.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      590 2024-04-04 05:02:38.000000 encommon-0.7.3/encommon/crypts/params.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-04 05:11:00.048277 encommon-0.7.3/encommon/crypts/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/crypts/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2433 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/crypts/test/test_crypts.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1206 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/crypts/test/test_hashes.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2023-12-31 23:18:53.000000 encommon-0.7.3/encommon/py.typed
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-04 05:11:00.048277 encommon-0.7.3/encommon/times/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      597 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/times/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2506 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/times/common.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     9854 2024-04-04 05:08:51.000000 encommon-0.7.3/encommon/times/duration.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6411 2024-04-04 05:08:51.000000 encommon-0.7.3/encommon/times/parse.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-04 05:11:00.049276 encommon-0.7.3/encommon/times/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/times/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1477 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/times/test/test_common.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3901 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/times/test/test_duration.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4308 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/times/test/test_parse.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2314 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/times/test/test_timers.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2023 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/times/test/test_times.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4735 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/times/test/test_window.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6287 2024-04-04 05:08:51.000000 encommon-0.7.3/encommon/times/timers.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     9688 2024-04-04 05:08:51.000000 encommon-0.7.3/encommon/times/times.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7975 2024-04-04 05:08:51.000000 encommon-0.7.3/encommon/times/window.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-04 05:11:00.049276 encommon-0.7.3/encommon/types/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      420 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/types/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2208 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/types/dicts.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2675 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/types/empty.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      560 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/types/strings.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-04 05:11:00.049276 encommon-0.7.3/encommon/types/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/types/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2673 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/types/test/test_dicts.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      981 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/types/test/test_empty.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      407 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/types/test/test_strings.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-04 05:11:00.049276 encommon-0.7.3/encommon/utils/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      833 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/utils/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      466 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/utils/common.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2462 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/utils/match.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3236 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/utils/paths.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3169 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/utils/sample.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7360 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/utils/stdout.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-04 05:11:00.049276 encommon-0.7.3/encommon/utils/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/utils/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1124 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/utils/test/test_match.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1892 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/utils/test/test_paths.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1464 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/utils/test/test_sample.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4878 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/utils/test/test_stdout.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        6 2024-04-04 05:09:53.000000 encommon-0.7.3/encommon/version.txt
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-04 05:11:00.050277 encommon-0.7.3/encommon.egg-info/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2671 2024-04-04 05:11:00.000000 encommon-0.7.3/encommon.egg-info/PKG-INFO
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1891 2024-04-04 05:11:00.000000 encommon-0.7.3/encommon.egg-info/SOURCES.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        1 2024-04-04 05:11:00.000000 encommon-0.7.3/encommon.egg-info/dependency_links.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       63 2024-04-04 05:11:00.000000 encommon-0.7.3/encommon.egg-info/requires.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        9 2024-04-04 05:11:00.000000 encommon-0.7.3/encommon.egg-info/top_level.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2023-12-31 23:18:53.000000 encommon-0.7.3/pyproject.toml
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       63 2024-01-01 10:25:04.000000 encommon-0.7.3/reqs-install.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      422 2024-04-04 05:11:00.050277 encommon-0.7.3/setup.cfg
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-05 00:13:03.598882 encommon-0.7.4/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1071 2024-03-20 05:52:00.000000 encommon-0.7.4/LICENSE
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       32 2023-12-31 23:18:53.000000 encommon-0.7.4/MANIFEST.in
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2671 2024-04-05 00:13:03.598882 encommon-0.7.4/PKG-INFO
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2177 2024-03-31 14:52:08.000000 encommon-0.7.4/README.md
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-05 00:13:03.595882 encommon-0.7.4/encommon/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2024-04-02 23:01:55.000000 encommon-0.7.4/encommon/__init__.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-05 00:13:03.596881 encommon-0.7.4/encommon/config/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      710 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/config/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2041 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/config/common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4743 2024-04-04 05:08:51.000000 encommon-0.7.4/encommon/config/config.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2313 2024-04-05 00:11:42.000000 encommon-0.7.4/encommon/config/files.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)    13973 2024-04-05 00:11:42.000000 encommon-0.7.4/encommon/config/logger.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1816 2024-04-04 05:08:51.000000 encommon-0.7.4/encommon/config/params.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2433 2024-04-05 00:11:42.000000 encommon-0.7.4/encommon/config/paths.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-05 00:13:03.596881 encommon-0.7.4/encommon/config/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-02 23:01:55.000000 encommon-0.7.4/encommon/config/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      731 2024-04-02 23:01:55.000000 encommon-0.7.4/encommon/config/test/test_common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3327 2024-04-04 05:08:51.000000 encommon-0.7.4/encommon/config/test/test_config.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2292 2024-04-04 05:08:51.000000 encommon-0.7.4/encommon/config/test/test_files.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4740 2024-04-02 23:01:55.000000 encommon-0.7.4/encommon/config/test/test_logger.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2101 2024-04-04 05:08:51.000000 encommon-0.7.4/encommon/config/test/test_paths.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      880 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/conftest.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-05 00:13:03.596881 encommon-0.7.4/encommon/crypts/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      318 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/crypts/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3500 2024-04-04 05:08:51.000000 encommon-0.7.4/encommon/crypts/crypts.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3103 2024-04-04 05:08:51.000000 encommon-0.7.4/encommon/crypts/hashes.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      590 2024-04-04 05:02:38.000000 encommon-0.7.4/encommon/crypts/params.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-05 00:13:03.596881 encommon-0.7.4/encommon/crypts/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/crypts/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2433 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/crypts/test/test_crypts.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1206 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/crypts/test/test_hashes.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2023-12-31 23:18:53.000000 encommon-0.7.4/encommon/py.typed
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-05 00:13:03.597881 encommon-0.7.4/encommon/times/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      597 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/times/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2506 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/times/common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     9854 2024-04-05 00:11:42.000000 encommon-0.7.4/encommon/times/duration.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6411 2024-04-04 05:08:51.000000 encommon-0.7.4/encommon/times/parse.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-05 00:13:03.597881 encommon-0.7.4/encommon/times/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/times/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1477 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/times/test/test_common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3901 2024-04-05 00:11:42.000000 encommon-0.7.4/encommon/times/test/test_duration.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4308 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/times/test/test_parse.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2314 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/times/test/test_timers.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2023 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/times/test/test_times.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4735 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/times/test/test_window.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6287 2024-04-04 05:08:51.000000 encommon-0.7.4/encommon/times/timers.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     9688 2024-04-04 05:08:51.000000 encommon-0.7.4/encommon/times/times.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7975 2024-04-04 05:08:51.000000 encommon-0.7.4/encommon/times/window.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-05 00:13:03.597881 encommon-0.7.4/encommon/types/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      420 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/types/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2208 2024-04-04 21:54:07.000000 encommon-0.7.4/encommon/types/dicts.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2675 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/types/empty.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      560 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/types/strings.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-05 00:13:03.597881 encommon-0.7.4/encommon/types/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/types/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2673 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/types/test/test_dicts.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      981 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/types/test/test_empty.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      407 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/types/test/test_strings.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-05 00:13:03.597881 encommon-0.7.4/encommon/utils/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      833 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/utils/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      466 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/utils/common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2462 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/utils/match.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3236 2024-04-04 21:54:29.000000 encommon-0.7.4/encommon/utils/paths.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3136 2024-04-05 00:09:08.000000 encommon-0.7.4/encommon/utils/sample.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7360 2024-04-04 21:55:08.000000 encommon-0.7.4/encommon/utils/stdout.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-05 00:13:03.598882 encommon-0.7.4/encommon/utils/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/utils/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1124 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/utils/test/test_match.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1892 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/utils/test/test_paths.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1464 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/utils/test/test_sample.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4878 2024-04-02 23:01:56.000000 encommon-0.7.4/encommon/utils/test/test_stdout.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        6 2024-04-05 00:12:01.000000 encommon-0.7.4/encommon/version.txt
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-05 00:13:03.598882 encommon-0.7.4/encommon.egg-info/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2671 2024-04-05 00:13:03.000000 encommon-0.7.4/encommon.egg-info/PKG-INFO
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1891 2024-04-05 00:13:03.000000 encommon-0.7.4/encommon.egg-info/SOURCES.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        1 2024-04-05 00:13:03.000000 encommon-0.7.4/encommon.egg-info/dependency_links.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       63 2024-04-05 00:13:03.000000 encommon-0.7.4/encommon.egg-info/requires.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        9 2024-04-05 00:13:03.000000 encommon-0.7.4/encommon.egg-info/top_level.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2023-12-31 23:18:53.000000 encommon-0.7.4/pyproject.toml
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       63 2024-01-01 10:25:04.000000 encommon-0.7.4/reqs-install.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      452 2024-04-05 00:13:03.598882 encommon-0.7.4/setup.cfg
```

### Comparing `encommon-0.7.3/LICENSE` & `encommon-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/PKG-INFO` & `encommon-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encommon
-Version: 0.7.3
+Version: 0.7.4
 Summary: Enasis Network Common Library
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `encommon-0.7.3/README.md` & `encommon-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/__init__.py` & `encommon-0.7.4/encommon/__init__.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/config/__init__.py` & `encommon-0.7.4/encommon/config/__init__.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/config/common.py` & `encommon-0.7.4/encommon/config/common.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/config/config.py` & `encommon-0.7.4/encommon/config/config.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/config/files.py` & `encommon-0.7.4/encommon/config/files.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/config/logger.py` & `encommon-0.7.4/encommon/config/logger.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/config/params.py` & `encommon-0.7.4/encommon/config/params.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/config/paths.py` & `encommon-0.7.4/encommon/config/paths.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/config/test/test_common.py` & `encommon-0.7.4/encommon/config/test/test_common.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/config/test/test_config.py` & `encommon-0.7.4/encommon/config/test/test_config.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/config/test/test_files.py` & `encommon-0.7.4/encommon/config/test/test_files.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/config/test/test_logger.py` & `encommon-0.7.4/encommon/config/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/config/test/test_paths.py` & `encommon-0.7.4/encommon/config/test/test_paths.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/conftest.py` & `encommon-0.7.4/encommon/conftest.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/crypts/crypts.py` & `encommon-0.7.4/encommon/crypts/crypts.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/crypts/hashes.py` & `encommon-0.7.4/encommon/crypts/hashes.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/crypts/params.py` & `encommon-0.7.4/encommon/crypts/params.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/crypts/test/test_crypts.py` & `encommon-0.7.4/encommon/crypts/test/test_crypts.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/crypts/test/test_hashes.py` & `encommon-0.7.4/encommon/crypts/test/test_hashes.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/times/__init__.py` & `encommon-0.7.4/encommon/times/__init__.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/times/common.py` & `encommon-0.7.4/encommon/times/common.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/times/duration.py` & `encommon-0.7.4/encommon/times/duration.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/times/parse.py` & `encommon-0.7.4/encommon/times/parse.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/times/test/test_common.py` & `encommon-0.7.4/encommon/times/test/test_common.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/times/test/test_duration.py` & `encommon-0.7.4/encommon/times/test/test_duration.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/times/test/test_parse.py` & `encommon-0.7.4/encommon/times/test/test_parse.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/times/test/test_timers.py` & `encommon-0.7.4/encommon/times/test/test_timers.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/times/test/test_times.py` & `encommon-0.7.4/encommon/times/test/test_times.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/times/test/test_window.py` & `encommon-0.7.4/encommon/times/test/test_window.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/times/timers.py` & `encommon-0.7.4/encommon/times/timers.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/times/times.py` & `encommon-0.7.4/encommon/times/times.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/times/window.py` & `encommon-0.7.4/encommon/times/window.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/types/dicts.py` & `encommon-0.7.4/encommon/types/dicts.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/types/empty.py` & `encommon-0.7.4/encommon/types/empty.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/types/strings.py` & `encommon-0.7.4/encommon/types/strings.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/types/test/test_dicts.py` & `encommon-0.7.4/encommon/types/test/test_dicts.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/types/test/test_empty.py` & `encommon-0.7.4/encommon/types/test/test_empty.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/utils/__init__.py` & `encommon-0.7.4/encommon/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/utils/match.py` & `encommon-0.7.4/encommon/utils/match.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/utils/paths.py` & `encommon-0.7.4/encommon/utils/paths.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/utils/sample.py` & `encommon-0.7.4/encommon/utils/sample.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 
 from .. import PROJECT
 from .. import WORKSPACE
 
 
 
 def prep_sample(
-    content: Any,  # noqa: ANN401
+    content: Any,
     *,
     default: Callable[[Any], str] = str,
-    replace: Optional[dict[str, str]] = None,
-) -> Any:  # noqa: ANN401
+    replace: Optional[dict[str, str | Path]] = None,
+) -> Any:
     """
     Return the content after processing using JSON functions.
 
     .. testsetup::
        >>> from ..types import Empty
 
     Example
@@ -51,33 +51,37 @@
         content, default=default)
 
     prefix = 'encommon_sample'
 
     replace = replace or {}
 
     replace |= {
-        'PROJECT': str(PROJECT.resolve()),
-        'WORKSPACE': str(WORKSPACE.resolve())}
+        'PROJECT': PROJECT,
+        'WORKSPACE': WORKSPACE}
 
     for old, new in replace.items():
+
+        if isinstance(new, Path):
+            new = str(new)
+
         content = content.replace(
             new, f'_/{prefix}/{old}/_')
 
     return loads(content)
 
 
 
 def load_sample(
     path: Path,
     content: Optional[Any] = None,
     update: bool = False,
     *,
     default: Callable[[Any], str] = str,
-    replace: Optional[dict[str, str]] = None,
-) -> Any:  # noqa: ANN401
+    replace: Optional[dict[str, str | Path]] = None,
+) -> Any:
     """
     Load the sample file and compare using provided content.
 
     .. testsetup::
        >>> from json import dumps
        >>> from json import loads
        >>> path = Path(getfixture('tmpdir'))
@@ -111,24 +115,24 @@
 
 
     def _save_sample() -> None:
         path.write_text(
             dumps(content, indent=2))
 
 
-    def _load_sample() -> Any:  # noqa: ANN401
+    def _load_sample() -> Any:
         return loads(
             path.read_text(
                 encoding='utf-8'))
 
 
     if path.exists():
         loaded = _load_sample()
 
-    if not path.exists():  # noqa: SIM114
+    if not path.exists():
         _save_sample()
 
     elif (update is True
             and content is not None
             and content != loaded):
         _save_sample()
```

### Comparing `encommon-0.7.3/encommon/utils/stdout.py` & `encommon-0.7.4/encommon/utils/stdout.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/utils/test/test_match.py` & `encommon-0.7.4/encommon/utils/test/test_match.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/utils/test/test_paths.py` & `encommon-0.7.4/encommon/utils/test/test_paths.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/utils/test/test_sample.py` & `encommon-0.7.4/encommon/utils/test/test_sample.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon/utils/test/test_stdout.py` & `encommon-0.7.4/encommon/utils/test/test_stdout.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/encommon.egg-info/PKG-INFO` & `encommon-0.7.4/encommon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encommon
-Version: 0.7.3
+Version: 0.7.4
 Summary: Enasis Network Common Library
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `encommon-0.7.3/encommon.egg-info/SOURCES.txt` & `encommon-0.7.4/encommon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `encommon-0.7.3/pyproject.toml` & `encommon-0.7.4/pyproject.toml`

 * *Files identical despite different names*

