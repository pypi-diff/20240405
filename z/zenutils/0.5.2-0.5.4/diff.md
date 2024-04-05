# Comparing `tmp/zenutils-0.5.2.tar.gz` & `tmp/zenutils-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenutils-0.5.2.tar", last modified: Thu Nov 16 14:54:01 2023, max compression
+gzip compressed data, was "zenutils-0.5.4.tar", last modified: Fri Apr  5 01:02:58 2024, max compression
```

## Comparing `zenutils-0.5.2.tar` & `zenutils-0.5.4.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-11-16 14:54:01.599070 zenutils-0.5.2/
--rw-r--r--   0 test       (501) staff       (20)     1067 2023-03-09 12:54:10.000000 zenutils-0.5.2/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      198 2022-06-17 11:16:41.000000 zenutils-0.5.2/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)    21541 2023-11-16 14:54:01.598936 zenutils-0.5.2/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)    20913 2023-11-16 14:50:25.000000 zenutils-0.5.2/README.md
--rw-r--r--   0 test       (501) staff       (20)       16 2022-06-17 10:49:49.000000 zenutils-0.5.2/requirements.py32.txt
--rw-r--r--   0 test       (501) staff       (20)        0 2023-11-16 14:54:00.000000 zenutils-0.5.2/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2023-11-16 14:54:01.599103 zenutils-0.5.2/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1742 2023-11-16 14:50:40.000000 zenutils-0.5.2/setup.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-11-16 14:54:01.594743 zenutils-0.5.2/tests/
--rw-r--r--   0 test       (501) staff       (20)      171 2022-06-17 06:56:58.000000 zenutils-0.5.2/tests/__init__.py
--rw-r--r--   0 test       (501) staff       (20)      143 2022-09-23 14:14:23.000000 zenutils-0.5.2/tests/t08_01.py
--rw-r--r--   0 test       (501) staff       (20)      536 2023-04-29 08:10:49.000000 zenutils-0.5.2/tests/test_baseutils.py
--rw-r--r--   0 test       (501) staff       (20)     6021 2023-09-07 02:52:03.000000 zenutils-0.5.2/tests/test_cacheutils.py
--rw-r--r--   0 test       (501) staff       (20)    15419 2022-06-21 03:54:40.000000 zenutils-0.5.2/tests/test_cipherutils.py
--rw-r--r--   0 test       (501) staff       (20)     1246 2022-11-29 02:04:49.000000 zenutils-0.5.2/tests/test_dateutils.py
--rw-r--r--   0 test       (501) staff       (20)    12895 2023-09-07 01:38:03.000000 zenutils-0.5.2/tests/test_dictutils.py
--rw-r--r--   0 test       (501) staff       (20)     4573 2022-11-23 12:36:21.000000 zenutils-0.5.2/tests/test_errorutils.py
--rw-r--r--   0 test       (501) staff       (20)     7281 2022-09-20 04:29:06.000000 zenutils-0.5.2/tests/test_fsutils.py
--rw-r--r--   0 test       (501) staff       (20)     8677 2023-04-28 16:03:25.000000 zenutils-0.5.2/tests/test_funcutils.py
--rw-r--r--   0 test       (501) staff       (20)     6676 2023-11-16 13:37:01.000000 zenutils-0.5.2/tests/test_hashutils.py
--rw-r--r--   0 test       (501) staff       (20)     2818 2022-08-28 08:48:38.000000 zenutils-0.5.2/tests/test_httputils.py
--rw-r--r--   0 test       (501) staff       (20)     1020 2022-11-23 06:59:43.000000 zenutils-0.5.2/tests/test_import_all.py
--rw-r--r--   0 test       (501) staff       (20)     2502 2022-11-23 08:06:56.000000 zenutils-0.5.2/tests/test_importutils.py
--rw-r--r--   0 test       (501) staff       (20)     1821 2022-06-21 06:30:06.000000 zenutils-0.5.2/tests/test_jsonutils.py
--rw-r--r--   0 test       (501) staff       (20)    10098 2023-11-16 13:28:54.000000 zenutils-0.5.2/tests/test_listutils.py
--rw-r--r--   0 test       (501) staff       (20)     1051 2023-11-16 13:28:47.000000 zenutils-0.5.2/tests/test_logutils.py
--rw-r--r--   0 test       (501) staff       (20)      980 2022-06-19 14:09:25.000000 zenutils-0.5.2/tests/test_nameutils.py
--rw-r--r--   0 test       (501) staff       (20)    13971 2022-11-20 03:51:51.000000 zenutils-0.5.2/tests/test_numericutils.py
--rw-r--r--   0 test       (501) staff       (20)     1187 2022-11-20 04:12:31.000000 zenutils-0.5.2/tests/test_packutils.py
--rw-r--r--   0 test       (501) staff       (20)    54463 2022-09-28 07:22:41.000000 zenutils-0.5.2/tests/test_randomutils.py
--rw-r--r--   0 test       (501) staff       (20)     1746 2022-11-20 03:15:03.000000 zenutils-0.5.2/tests/test_serviceutils.py
--rw-r--r--   0 test       (501) staff       (20)     4304 2022-10-18 04:33:14.000000 zenutils-0.5.2/tests/test_sixutils.py
--rw-r--r--   0 test       (501) staff       (20)    27083 2022-06-21 07:36:31.000000 zenutils-0.5.2/tests/test_strutils.py
--rw-r--r--   0 test       (501) staff       (20)     2056 2022-08-16 15:10:43.000000 zenutils-0.5.2/tests/test_sysutils.py
--rw-r--r--   0 test       (501) staff       (20)     6750 2023-08-16 06:13:12.000000 zenutils-0.5.2/tests/test_threadutils.py
--rw-r--r--   0 test       (501) staff       (20)     3151 2022-08-05 14:11:47.000000 zenutils-0.5.2/tests/test_treeutils.py
--rw-r--r--   0 test       (501) staff       (20)     5116 2022-06-19 14:09:58.000000 zenutils-0.5.2/tests/test_typingutils.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-11-16 14:54:01.598213 zenutils-0.5.2/zenutils/
--rw-r--r--   0 test       (501) staff       (20)      218 2023-04-19 02:53:36.000000 zenutils-0.5.2/zenutils/__init__.py
--rw-r--r--   0 test       (501) staff       (20)      715 2023-09-13 06:08:51.000000 zenutils-0.5.2/zenutils/base64utils.py
--rw-r--r--   0 test       (501) staff       (20)      328 2023-08-17 15:10:25.000000 zenutils-0.5.2/zenutils/baseutils.py
--rw-r--r--   0 test       (501) staff       (20)     6467 2023-09-13 06:15:58.000000 zenutils-0.5.2/zenutils/cacheutils.py
--rw-r--r--   0 test       (501) staff       (20)    16731 2023-08-18 14:08:08.000000 zenutils-0.5.2/zenutils/cipherutils.py
--rw-r--r--   0 test       (501) staff       (20)     1100 2023-08-17 15:12:14.000000 zenutils-0.5.2/zenutils/dateutils.py
--rw-r--r--   0 test       (501) staff       (20)    17617 2023-09-07 01:38:06.000000 zenutils-0.5.2/zenutils/dictutils.py
--rw-r--r--   0 test       (501) staff       (20)    27016 2023-04-29 02:27:06.000000 zenutils-0.5.2/zenutils/errorutils.py
--rw-r--r--   0 test       (501) staff       (20)    23276 2023-04-20 02:53:46.000000 zenutils-0.5.2/zenutils/fsutils.py
--rw-r--r--   0 test       (501) staff       (20)    18179 2023-08-18 13:16:10.000000 zenutils-0.5.2/zenutils/funcutils.py
--rw-r--r--   0 test       (501) staff       (20)    27068 2023-11-16 13:49:52.000000 zenutils-0.5.2/zenutils/hashutils.py
--rw-r--r--   0 test       (501) staff       (20)     3574 2023-08-18 14:37:10.000000 zenutils-0.5.2/zenutils/httputils.py
--rw-r--r--   0 test       (501) staff       (20)     2650 2023-04-20 02:54:51.000000 zenutils-0.5.2/zenutils/importutils.py
--rw-r--r--   0 test       (501) staff       (20)    11145 2023-08-17 15:51:53.000000 zenutils-0.5.2/zenutils/jsonutils.py
--rw-r--r--   0 test       (501) staff       (20)     9101 2023-08-18 13:27:27.000000 zenutils-0.5.2/zenutils/listutils.py
--rw-r--r--   0 test       (501) staff       (20)     7899 2023-11-16 13:25:02.000000 zenutils-0.5.2/zenutils/logutils.py
--rw-r--r--   0 test       (501) staff       (20)    23117 2023-08-18 14:39:37.000000 zenutils-0.5.2/zenutils/nameutils.py
--rw-r--r--   0 test       (501) staff       (20)     5553 2023-04-20 02:57:09.000000 zenutils-0.5.2/zenutils/numericutils.py
--rw-r--r--   0 test       (501) staff       (20)     2285 2023-04-20 02:57:21.000000 zenutils-0.5.2/zenutils/packutils.py
--rw-r--r--   0 test       (501) staff       (20)     1594 2023-04-20 02:57:30.000000 zenutils-0.5.2/zenutils/perfutils.py
--rw-r--r--   0 test       (501) staff       (20)    11099 2023-04-20 02:57:38.000000 zenutils-0.5.2/zenutils/randomutils.py
--rw-r--r--   0 test       (501) staff       (20)     6507 2023-08-14 13:20:09.000000 zenutils-0.5.2/zenutils/serviceutils.py
--rw-r--r--   0 test       (501) staff       (20)     5843 2023-09-07 01:32:52.000000 zenutils-0.5.2/zenutils/sixutils.py
--rw-r--r--   0 test       (501) staff       (20)     6448 2023-04-20 02:58:25.000000 zenutils-0.5.2/zenutils/socketserverutils.py
--rw-r--r--   0 test       (501) staff       (20)    32036 2023-09-13 06:25:47.000000 zenutils-0.5.2/zenutils/strutils.py
--rw-r--r--   0 test       (501) staff       (20)     7857 2023-04-20 02:58:48.000000 zenutils-0.5.2/zenutils/sysutils.py
--rw-r--r--   0 test       (501) staff       (20)    30268 2023-08-18 13:18:59.000000 zenutils-0.5.2/zenutils/threadutils.py
--rw-r--r--   0 test       (501) staff       (20)     5242 2023-11-16 13:02:56.000000 zenutils-0.5.2/zenutils/treeutils.py
--rw-r--r--   0 test       (501) staff       (20)     8202 2023-04-20 03:01:17.000000 zenutils-0.5.2/zenutils/typingutils.py
--rw-r--r--   0 test       (501) staff       (20)     3054 2023-04-20 03:17:04.000000 zenutils-0.5.2/zenutils/xmlrpcutils.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-11-16 14:54:01.598753 zenutils-0.5.2/zenutils.egg-info/
--rw-r--r--   0 test       (501) staff       (20)    21541 2023-11-16 14:54:01.000000 zenutils-0.5.2/zenutils.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     1590 2023-11-16 14:54:01.000000 zenutils-0.5.2/zenutils.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2023-11-16 14:54:01.000000 zenutils-0.5.2/zenutils.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2023-11-16 14:54:01.000000 zenutils-0.5.2/zenutils.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)       15 2023-11-16 14:54:01.000000 zenutils-0.5.2/zenutils.egg-info/top_level.txt
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-05 01:02:58.114982 zenutils-0.5.4/
+-rw-r--r--   0 test       (501) staff       (20)     1036 2024-04-05 00:47:01.000000 zenutils-0.5.4/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      198 2022-06-17 11:16:41.000000 zenutils-0.5.4/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)    21592 2024-04-05 01:02:58.114835 zenutils-0.5.4/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)    21038 2024-04-05 00:56:51.000000 zenutils-0.5.4/README.md
+-rw-r--r--   0 test       (501) staff       (20)       16 2022-06-17 10:49:49.000000 zenutils-0.5.4/requirements.py32.txt
+-rw-r--r--   0 test       (501) staff       (20)        0 2024-04-05 01:02:56.000000 zenutils-0.5.4/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2024-04-05 01:02:58.115023 zenutils-0.5.4/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1656 2024-04-05 00:50:40.000000 zenutils-0.5.4/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-05 01:02:58.109035 zenutils-0.5.4/tests/
+-rw-r--r--   0 test       (501) staff       (20)      204 2024-04-05 01:01:11.000000 zenutils-0.5.4/tests/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)      144 2024-04-05 01:00:19.000000 zenutils-0.5.4/tests/t08_01.py
+-rw-r--r--   0 test       (501) staff       (20)      536 2024-04-05 01:01:08.000000 zenutils-0.5.4/tests/test_baseutils.py
+-rw-r--r--   0 test       (501) staff       (20)     6021 2024-04-05 01:01:06.000000 zenutils-0.5.4/tests/test_cacheutils.py
+-rw-r--r--   0 test       (501) staff       (20)    15969 2024-04-05 01:00:15.000000 zenutils-0.5.4/tests/test_cipherutils.py
+-rw-r--r--   0 test       (501) staff       (20)     1594 2024-04-05 01:00:14.000000 zenutils-0.5.4/tests/test_dateutils.py
+-rw-r--r--   0 test       (501) staff       (20)    12895 2024-04-05 01:00:13.000000 zenutils-0.5.4/tests/test_dictutils.py
+-rw-r--r--   0 test       (501) staff       (20)     4663 2024-04-05 01:00:12.000000 zenutils-0.5.4/tests/test_errorutils.py
+-rw-r--r--   0 test       (501) staff       (20)     7415 2024-04-05 01:00:11.000000 zenutils-0.5.4/tests/test_fsutils.py
+-rw-r--r--   0 test       (501) staff       (20)     8677 2024-04-05 01:01:03.000000 zenutils-0.5.4/tests/test_funcutils.py
+-rw-r--r--   0 test       (501) staff       (20)     6676 2024-04-05 01:01:00.000000 zenutils-0.5.4/tests/test_hashutils.py
+-rw-r--r--   0 test       (501) staff       (20)     2852 2024-04-05 01:00:07.000000 zenutils-0.5.4/tests/test_httputils.py
+-rw-r--r--   0 test       (501) staff       (20)     1015 2024-04-05 01:00:04.000000 zenutils-0.5.4/tests/test_import_all.py
+-rw-r--r--   0 test       (501) staff       (20)     2507 2024-04-05 00:59:46.000000 zenutils-0.5.4/tests/test_importutils.py
+-rw-r--r--   0 test       (501) staff       (20)     2153 2024-04-05 01:00:20.000000 zenutils-0.5.4/tests/test_jsonutils.py
+-rw-r--r--   0 test       (501) staff       (20)    10098 2024-04-05 01:00:54.000000 zenutils-0.5.4/tests/test_listutils.py
+-rw-r--r--   0 test       (501) staff       (20)     1051 2024-04-05 01:00:56.000000 zenutils-0.5.4/tests/test_logutils.py
+-rw-r--r--   0 test       (501) staff       (20)     1014 2024-04-05 01:00:23.000000 zenutils-0.5.4/tests/test_nameutils.py
+-rw-r--r--   0 test       (501) staff       (20)    14262 2024-04-05 01:00:24.000000 zenutils-0.5.4/tests/test_numericutils.py
+-rw-r--r--   0 test       (501) staff       (20)     1221 2024-04-05 01:00:25.000000 zenutils-0.5.4/tests/test_packutils.py
+-rw-r--r--   0 test       (501) staff       (20)    78618 2024-04-05 01:00:46.000000 zenutils-0.5.4/tests/test_randomutils.py
+-rw-r--r--   0 test       (501) staff       (20)     1763 2024-04-05 01:00:27.000000 zenutils-0.5.4/tests/test_serviceutils.py
+-rw-r--r--   0 test       (501) staff       (20)     4447 2024-04-05 01:00:28.000000 zenutils-0.5.4/tests/test_sixutils.py
+-rw-r--r--   0 test       (501) staff       (20)    28099 2024-04-05 01:00:30.000000 zenutils-0.5.4/tests/test_strutils.py
+-rw-r--r--   0 test       (501) staff       (20)     2087 2024-04-05 01:00:31.000000 zenutils-0.5.4/tests/test_sysutils.py
+-rw-r--r--   0 test       (501) staff       (20)     6789 2024-04-05 01:00:41.000000 zenutils-0.5.4/tests/test_threadutils.py
+-rw-r--r--   0 test       (501) staff       (20)     3225 2024-04-05 01:00:33.000000 zenutils-0.5.4/tests/test_treeutils.py
+-rw-r--r--   0 test       (501) staff       (20)     5215 2024-04-05 01:00:35.000000 zenutils-0.5.4/tests/test_typingutils.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-05 01:02:58.114071 zenutils-0.5.4/zenutils/
+-rw-r--r--   0 test       (501) staff       (20)      218 2023-04-19 02:53:36.000000 zenutils-0.5.4/zenutils/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)      715 2024-04-05 01:01:19.000000 zenutils-0.5.4/zenutils/base64utils.py
+-rw-r--r--   0 test       (501) staff       (20)      328 2024-04-05 01:01:21.000000 zenutils-0.5.4/zenutils/baseutils.py
+-rw-r--r--   0 test       (501) staff       (20)     6467 2024-04-05 01:01:23.000000 zenutils-0.5.4/zenutils/cacheutils.py
+-rw-r--r--   0 test       (501) staff       (20)    16731 2024-04-05 01:01:26.000000 zenutils-0.5.4/zenutils/cipherutils.py
+-rw-r--r--   0 test       (501) staff       (20)     1100 2024-04-05 01:01:28.000000 zenutils-0.5.4/zenutils/dateutils.py
+-rw-r--r--   0 test       (501) staff       (20)    17617 2024-04-05 01:01:30.000000 zenutils-0.5.4/zenutils/dictutils.py
+-rw-r--r--   0 test       (501) staff       (20)    27287 2024-04-05 01:01:34.000000 zenutils-0.5.4/zenutils/errorutils.py
+-rw-r--r--   0 test       (501) staff       (20)    23357 2024-04-05 01:01:38.000000 zenutils-0.5.4/zenutils/fsutils.py
+-rw-r--r--   0 test       (501) staff       (20)    18179 2024-04-05 01:01:41.000000 zenutils-0.5.4/zenutils/funcutils.py
+-rw-r--r--   0 test       (501) staff       (20)    27068 2024-04-05 01:01:44.000000 zenutils-0.5.4/zenutils/hashutils.py
+-rw-r--r--   0 test       (501) staff       (20)     3574 2023-08-18 14:37:10.000000 zenutils-0.5.4/zenutils/httputils.py
+-rw-r--r--   0 test       (501) staff       (20)     2607 2024-02-03 04:57:26.000000 zenutils-0.5.4/zenutils/importutils.py
+-rw-r--r--   0 test       (501) staff       (20)    11262 2024-01-09 15:31:23.000000 zenutils-0.5.4/zenutils/jsonutils.py
+-rw-r--r--   0 test       (501) staff       (20)     9101 2023-08-18 13:27:27.000000 zenutils-0.5.4/zenutils/listutils.py
+-rw-r--r--   0 test       (501) staff       (20)     7899 2023-11-16 13:25:02.000000 zenutils-0.5.4/zenutils/logutils.py
+-rw-r--r--   0 test       (501) staff       (20)    23117 2023-08-18 14:39:37.000000 zenutils-0.5.4/zenutils/nameutils.py
+-rw-r--r--   0 test       (501) staff       (20)     5553 2023-04-20 02:57:09.000000 zenutils-0.5.4/zenutils/numericutils.py
+-rw-r--r--   0 test       (501) staff       (20)     2285 2023-04-20 02:57:21.000000 zenutils-0.5.4/zenutils/packutils.py
+-rw-r--r--   0 test       (501) staff       (20)     1594 2023-04-20 02:57:30.000000 zenutils-0.5.4/zenutils/perfutils.py
+-rw-r--r--   0 test       (501) staff       (20)    11547 2024-02-03 04:51:57.000000 zenutils-0.5.4/zenutils/randomutils.py
+-rw-r--r--   0 test       (501) staff       (20)     6507 2023-08-14 13:20:09.000000 zenutils-0.5.4/zenutils/serviceutils.py
+-rw-r--r--   0 test       (501) staff       (20)     5843 2023-09-07 01:32:52.000000 zenutils-0.5.4/zenutils/sixutils.py
+-rw-r--r--   0 test       (501) staff       (20)     6448 2023-04-20 02:58:25.000000 zenutils-0.5.4/zenutils/socketserverutils.py
+-rw-r--r--   0 test       (501) staff       (20)    32036 2023-09-13 06:25:47.000000 zenutils-0.5.4/zenutils/strutils.py
+-rw-r--r--   0 test       (501) staff       (20)     7857 2023-04-20 02:58:48.000000 zenutils-0.5.4/zenutils/sysutils.py
+-rw-r--r--   0 test       (501) staff       (20)    30268 2023-08-18 13:18:59.000000 zenutils-0.5.4/zenutils/threadutils.py
+-rw-r--r--   0 test       (501) staff       (20)     5242 2023-11-16 13:02:56.000000 zenutils-0.5.4/zenutils/treeutils.py
+-rw-r--r--   0 test       (501) staff       (20)     8202 2023-04-20 03:01:17.000000 zenutils-0.5.4/zenutils/typingutils.py
+-rw-r--r--   0 test       (501) staff       (20)     3054 2023-04-20 03:17:04.000000 zenutils-0.5.4/zenutils/xmlrpcutils.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-05 01:02:58.114638 zenutils-0.5.4/zenutils.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)    21592 2024-04-05 01:02:58.000000 zenutils-0.5.4/zenutils.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     1590 2024-04-05 01:02:58.000000 zenutils-0.5.4/zenutils.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-04-05 01:02:58.000000 zenutils-0.5.4/zenutils.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-04-05 01:02:57.000000 zenutils-0.5.4/zenutils.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)       15 2024-04-05 01:02:58.000000 zenutils-0.5.4/zenutils.egg-info/top_level.txt
```

### Comparing `zenutils-0.5.2/LICENSE` & `zenutils-0.5.4/LICENSE`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 MIT License
 
-Copyright (c) 2022 zencore.cn
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `zenutils-0.5.2/PKG-INFO` & `zenutils-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: zenutils
-Version: 0.5.2
+Version: 0.5.4
 Summary: Collection of simple utils.
 Author: Xin HaoJia
-Author-email: xinhaojia@zencore.cn
 Maintainer: Xin HaoJia
-Maintainer-email: xinhaojia@zencore.cn
 License: MIT
 Keywords: zenutils
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -871,7 +869,16 @@
 
 - Fix logutils default format missing space between thread and module fields.
 
 ### v0.5.2
 
 - Add hashutils.get_hash_digest.
 - Add log_to_console and log_to_file option in logutils.get_simple_config.
+
+### v0.5.3
+
+- Fix jsonutils.simple_json_dumps for set value problem.
+
+### v0.5.4
+
+- fsutils.safe_write add timestr suffix.
+
```

### Comparing `zenutils-0.5.2/README.md` & `zenutils-0.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -852,7 +852,16 @@
 
 - Fix logutils default format missing space between thread and module fields.
 
 ### v0.5.2
 
 - Add hashutils.get_hash_digest.
 - Add log_to_console and log_to_file option in logutils.get_simple_config.
+
+### v0.5.3
+
+- Fix jsonutils.simple_json_dumps for set value problem.
+
+### v0.5.4
+
+- fsutils.safe_write add timestr suffix.
+
```

### Comparing `zenutils-0.5.2/setup.py` & `zenutils-0.5.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,22 +27,20 @@
     with open(
         os.path.join(here, "requirements.py32.txt"), "r", encoding="utf-8"
     ) as fobj:
         requires += [x.strip() for x in fobj.readlines() if x.strip()]
 
 setup(
     name="zenutils",
-    version="0.5.2",
+    version="0.5.4",
     description="Collection of simple utils.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Xin HaoJia",
-    author_email="xinhaojia@zencore.cn",
     maintainer="Xin HaoJia",
-    maintainer_email="xinhaojia@zencore.cn",
     license="MIT",
     license_files=("LICENSE",),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: MIT License",
```

### Comparing `zenutils-0.5.2/tests/test_baseutils.py` & `zenutils-0.5.4/tests/test_baseutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/tests/test_cacheutils.py` & `zenutils-0.5.4/tests/test_cacheutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/tests/test_cipherutils.py` & `zenutils-0.5.4/tests/test_cipherutils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,71 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 
 import unittest
 import random
 import string
 import os
 
 from zenutils import randomutils
 from zenutils import cipherutils
 from zenutils import listutils
 
+
 class TestCipherUtils(unittest.TestCase):
-   
+
     def test01(self):
-        password = "".join(randomutils.choices(string.ascii_letters, k=random.randint(4, 16)))
+        password = "".join(
+            randomutils.choices(string.ascii_letters, k=random.randint(4, 16))
+        )
         cipher = cipherutils.S12Cipher(password=password)
-        text1 = ("".join(randomutils.choices(string.ascii_letters, k=random.randint(0, 1024)))).encode()
+        text1 = (
+            "".join(
+                randomutils.choices(string.ascii_letters, k=random.randint(0, 1024))
+            )
+        ).encode()
         data = cipher.encrypt(text1)
         text2 = cipher.decrypt(data)
         assert text1 == text2
-    
+
     def test02(self):
-        password = "".join(randomutils.choices(string.ascii_letters, k=random.randint(4, 16)))
+        password = "".join(
+            randomutils.choices(string.ascii_letters, k=random.randint(4, 16))
+        )
         cipher = cipherutils.S12Cipher(password=password)
         text1 = "hello"
         text2 = "hello world"
         data1 = cipher.encrypt(text1)
         data2 = cipher.encrypt(text2)
         assert data2.startswith(data1)
 
     def test03(self):
-        password = "".join(randomutils.choices(string.ascii_letters, k=random.randint(4, 16)))
+        password = "".join(
+            randomutils.choices(string.ascii_letters, k=random.randint(4, 16))
+        )
         cipher = cipherutils.S12Cipher(password=password)
         es = set()
         ps = set()
         for c in string.ascii_letters:
             d = cipher.encrypt(c)
             ps.add(c)
             es.add(d)
         assert len(ps) == len(es)
 
-
     def test04(self):
         gen = cipherutils.RawDataEncoder()
         data1 = os.urandom(1024)
         data2 = gen.encode(data1)
         data3 = gen.decode(data2)
         assert data1 == data3
 
@@ -78,92 +96,111 @@
         data3 = gen.decode(data2)
         assert data1 == data3
 
         assert gen.encode(None) is None
         assert gen.decode(None) is None
 
     def test08(self):
-        cipher = cipherutils.S12Cipher(password="testpwd", result_encoder=cipherutils.HexlifyEncoder(), force_text=True)
+        cipher = cipherutils.S12Cipher(
+            password="testpwd",
+            result_encoder=cipherutils.HexlifyEncoder(),
+            force_text=True,
+        )
         text1 = "".join(randomutils.choices(string.ascii_letters, k=1024))
         text2 = cipher.encrypt(text1)
         text3 = cipher.decrypt(text2)
         assert text1 == text3
 
-
     def test11(self):
-        password = "".join(randomutils.choices(string.ascii_letters, k=random.randint(4, 16)))
+        password = "".join(
+            randomutils.choices(string.ascii_letters, k=random.randint(4, 16))
+        )
         cipher = cipherutils.IvCipher(password=password)
         last_n2 = None
         for n1 in range(-10000, 10000, 100):
             n2 = cipher.encrypt(n1)
             n3 = cipher.decrypt(n2)
             if last_n2 is None:
                 last_n2 = n2
             else:
                 assert n2 > last_n2
             assert n1 == n3
             last_n2 = n2
 
     def test12(self):
-        password = "".join(randomutils.choices(string.ascii_letters, k=random.randint(4, 16)))
+        password = "".join(
+            randomutils.choices(string.ascii_letters, k=random.randint(4, 16))
+        )
         cipher = cipherutils.IvCipher(password=password)
         last_n2 = None
         for n1 in range(-10000, 10000, 100):
             n2 = cipher.encrypt(n1)
             n3 = cipher.decrypt(n2)
             if last_n2 is None:
                 last_n2 = n2
             else:
                 assert n2 > last_n2
             assert n1 == n3
             last_n2 = n2
 
     def test13(self):
-        password = "".join(randomutils.choices(string.ascii_letters, k=random.randint(4, 16)))
+        password = "".join(
+            randomutils.choices(string.ascii_letters, k=random.randint(4, 16))
+        )
         cipher = cipherutils.IvfCipher(password=password)
         n1 = 19231.1313
         n2 = cipher.encrypt(n1)
         n3 = cipher.decrypt(n2)
         assert n1 == n3
 
     def test14(self):
         for int_digits in range(1, 11):
             for float_digits in range(1, 6):
                 for _ in range(5):
-                    password = "".join(randomutils.choices(string.ascii_letters, k=random.randint(4, 16)))
+                    password = "".join(
+                        randomutils.choices(
+                            string.ascii_letters, k=random.randint(4, 16)
+                        )
+                    )
                     cipher_params = {
                         "int_digits": int_digits,
                         "float_digits": float_digits,
                     }
                     cipher = cipherutils.IvfCipher(password=password, **cipher_params)
-                    max_value = 10 ** int_digits + (1 - 0.1 ** float_digits)
-                    range_start = -1 * max_value * (10 ** float_digits)
-                    range_end = max_value * (10 ** float_digits)
+                    max_value = 10**int_digits + (1 - 0.1**float_digits)
+                    range_start = -1 * max_value * (10**float_digits)
+                    range_end = max_value * (10**float_digits)
                     ns = []
-                    for n1 in range(int(range_start), int(range_end), int(range_end / 13)):
-                        n1 /= (10 ** float_digits)
+                    for n1 in range(
+                        int(range_start), int(range_end), int(range_end / 13)
+                    ):
+                        n1 /= 10**float_digits
                         n2 = cipher.encrypt(n1)
                         n3 = cipher.decrypt(n2)
                         assert n1 == n3
                         ns.append(n2)
                     assert listutils.is_ordered(ns)
 
     def test15(self):
         for int_digits in range(1, 11):
             for _ in range(50):
                 float_digits = 0
-                password = "".join(randomutils.choices(string.ascii_letters, k=random.randint(4, 16)))
+                password = "".join(
+                    randomutils.choices(string.ascii_letters, k=random.randint(4, 16))
+                )
                 cipher_params = {
                     "int_digits": int_digits,
                     "float_digits": float_digits,
                 }
                 cipher = cipherutils.IvfCipher(password=password, kwargs=cipher_params)
-                max_value = 10 ** int_digits - random.randint(1, 1000)
+                max_value = 10**int_digits - random.randint(1, 1000)
                 last_n2 = None
-                for n1 in range(int(-1 * max_value), int(max_value), max(int(max_value / 13), 1)):
+                for n1 in range(
+                    int(-1 * max_value), int(max_value), max(int(max_value / 13), 1)
+                ):
                     n2 = cipher.encrypt(n1)
                     n3 = cipher.decrypt(n2)
                     if last_n2 is None:
                         last_n2 = n2
                     else:
                         assert n2 > last_n2
                     assert n1 == n3
@@ -193,29 +230,29 @@
             for loop2 in range(100):
                 data1 = os.urandom(random.randint(1, 100))
                 data2 = os.urandom(random.randint(1, 100))
                 flag1 = data1 > data2
                 data3 = cipher.encrypt(data1)
                 data4 = cipher.encrypt(data2)
                 flag2 = data3 > data4
-                #assert flag1 == flag2
+                # assert flag1 == flag2
 
     def test19(self):
         # Used for sorting test for S2Cipher
         # failed
         for loop1 in range(1):
             cipher = cipherutils.S2Cipher(password=os.urandom(16))
             for loop2 in range(100):
                 data1 = os.urandom(random.randint(1, 100))
                 data2 = os.urandom(random.randint(1, 100))
                 flag1 = data1 > data2
                 data3 = cipher.encrypt(data1)
                 data4 = cipher.encrypt(data2)
                 flag2 = data3 > data4
-                #assert flag1 == flag2
+                # assert flag1 == flag2
 
     def test20(self):
         # Used for sorting test for S12Cipher
         # pass
         for loop1 in range(1):
             cipher = cipherutils.S12Cipher(password=os.urandom(16))
             for loop2 in range(100):
@@ -243,88 +280,93 @@
                     assert not xt in data
 
     def test22(self):
         # Used for partly searching test for S1Cipher with result_encoder=HexlifyEncoder
         # failed
         for loop1 in range(1):
             password = os.urandom(16)
-            cipher = cipherutils.S1Cipher(password=password, result_encoder=cipherutils.HexlifyEncoder())
+            cipher = cipherutils.S1Cipher(
+                password=password, result_encoder=cipherutils.HexlifyEncoder()
+            )
             for loop2 in range(10):
                 for x in range(256):
                     all_seeds = list(range(256))
                     all_seeds.remove(x)
                     random.shuffle(all_seeds)
                     data = cipher.encrypt(bytes(all_seeds))
                     xt = cipher.encrypt(bytes([x]))
-                    #assert not xt in data
+                    # assert not xt in data
 
     def test23(self):
         # Used for partly searching test for S2Cipher with result_encoder=Utf8Encoder
         # failed
         for loop1 in range(1):
             password = os.urandom(16)
             cipher = cipherutils.S2Cipher(password=password)
             for loop2 in range(10):
                 for x in range(256):
                     all_seeds = list(range(256))
                     all_seeds.remove(x)
                     random.shuffle(all_seeds)
                     data = cipher.encrypt(bytes(all_seeds))
                     xt = cipher.encrypt(bytes([x]))
-                    #assert not xt in data
+                    # assert not xt in data
 
     def test24(self):
         # Used for partly searching test for S2Cipher with result_encoder=HexlifyEncoder
         # failed
         for loop1 in range(1):
             password = os.urandom(16)
-            cipher = cipherutils.S2Cipher(password=password, result_encoder=cipherutils.HexlifyEncoder())
+            cipher = cipherutils.S2Cipher(
+                password=password, result_encoder=cipherutils.HexlifyEncoder()
+            )
             for loop2 in range(10):
                 for x in range(256):
                     all_seeds = list(range(256))
                     all_seeds.remove(x)
                     random.shuffle(all_seeds)
                     data = cipher.encrypt(bytes(all_seeds))
                     xt = cipher.encrypt(bytes([x]))
-                    #assert not xt in data
+                    # assert not xt in data
 
     def test25(self):
         # Used for partly searching test for S12Cipher with result_encoder=RawDataEncoder
         # failed
         for loop1 in range(1):
             password = os.urandom(16)
             cipher = cipherutils.S12Cipher(password=password)
             for loop2 in range(10):
                 for x in range(256):
                     all_seeds = list(range(256))
                     all_seeds.remove(x)
                     random.shuffle(all_seeds)
                     data = cipher.encrypt(bytes(all_seeds))
                     xt = cipher.encrypt(bytes([x]))
-                    #assert not xt in data
+                    # assert not xt in data
 
     def test26(self):
         # Used for partly searching test for S12Cipher with result_encoder=HexlifyEncoder
         # failed
         for loop1 in range(1):
             password = os.urandom(16)
-            cipher = cipherutils.S12Cipher(password=password, result_encoder=cipherutils.HexlifyEncoder())
+            cipher = cipherutils.S12Cipher(
+                password=password, result_encoder=cipherutils.HexlifyEncoder()
+            )
             for loop2 in range(10):
                 for x in range(256):
                     all_seeds = list(range(256))
                     all_seeds.remove(x)
                     random.shuffle(all_seeds)
                     data = cipher.encrypt(bytes(all_seeds))
                     xt = cipher.encrypt(bytes([x]))
-                    #assert not xt in data
-
+                    # assert not xt in data
 
     def test29(self):
         thelist = []
-        for i in range(1000000000000000, 1000000000000000+10):
+        for i in range(1000000000000000, 1000000000000000 + 10):
             cipher = cipherutils.IvfCipher(password="testpwd")
             value = cipher.encrypt(i)
             thelist.append(value)
         assert listutils.is_ordered(thelist)
 
     def test30(self):
         c1 = cipherutils.S1Cipher(password="hello")
@@ -346,33 +388,33 @@
         d1 = c1.encrypt("hello")
         d2 = c2.encrypt("hello")
         assert d1 == d2
 
     def test33(self):
         c1 = cipherutils.S1Cipher(password="hello")
         d1 = c1.encrypt("hello")
-    
+
         password = c1.dumps()
         c2 = cipherutils.S1Cipher(password=password)
         d2 = c2.encrypt("hello")
         assert d1 == d2
 
     def test34(self):
         c1 = cipherutils.S2Cipher(password="hello")
         d1 = c1.encrypt("hello")
-    
+
         password = c1.dumps()
         c2 = cipherutils.S2Cipher(password=password)
         d2 = c2.encrypt("hello")
         assert d1 == d2
 
     def test35(self):
         c1 = cipherutils.S12Cipher(password="hello")
         d1 = c1.encrypt("hello")
-    
+
         password = c1.dumps()
         c2 = cipherutils.S12Cipher(password=password)
         d2 = c2.encrypt("hello")
         assert d1 == d2
 
     def test36(self):
         gen = cipherutils.Utf8Encoder()
```

### Comparing `zenutils-0.5.2/tests/test_dateutils.py` & `zenutils-0.5.4/tests/test_dateutils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,68 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 import datetime
 import unittest
 
 from zenutils import dateutils
 
+
 class TestDateUtils(unittest.TestCase):
-   
-   def test01(self):
-        days = list(dateutils.get_days(datetime.datetime(2022, 1, 1), datetime.datetime(2022, 2, 1)))
+
+    def test01(self):
+        days = list(
+            dateutils.get_days(
+                datetime.datetime(2022, 1, 1), datetime.datetime(2022, 2, 1)
+            )
+        )
         assert len(days) == 32
 
-   def test02(self):
-        days = list(dateutils.get_days(datetime.datetime(2022, 2, 1), datetime.datetime(2022, 3, 1)))
+    def test02(self):
+        days = list(
+            dateutils.get_days(
+                datetime.datetime(2022, 2, 1), datetime.datetime(2022, 3, 1)
+            )
+        )
         assert len(days) == 29
 
-   def test03(self):
-        days = list(dateutils.get_months(datetime.datetime(2022, 2, 1), datetime.datetime(2022, 3, 1)))
+    def test03(self):
+        days = list(
+            dateutils.get_months(
+                datetime.datetime(2022, 2, 1), datetime.datetime(2022, 3, 1)
+            )
+        )
         assert len(days) == 2
 
-   def test04(self):
-        days = list(dateutils.get_years(datetime.datetime(2022, 2, 1), datetime.datetime(2022, 3, 1)))
+    def test04(self):
+        days = list(
+            dateutils.get_years(
+                datetime.datetime(2022, 2, 1), datetime.datetime(2022, 3, 1)
+            )
+        )
         assert len(days) == 1
 
-   def test04(self):
-        days = list(dateutils.get_years(datetime.datetime(2021, 2, 1), datetime.datetime(2022, 3, 1)))
+    def test04(self):
+        days = list(
+            dateutils.get_years(
+                datetime.datetime(2021, 2, 1), datetime.datetime(2022, 3, 1)
+            )
+        )
         assert len(days) == 2
 
-   def test05(self):
-        days = list(dateutils.get_months(datetime.datetime(2021, 2, 1), datetime.datetime(2022, 3, 1)))
+    def test05(self):
+        days = list(
+            dateutils.get_months(
+                datetime.datetime(2021, 2, 1), datetime.datetime(2022, 3, 1)
+            )
+        )
         assert len(days) == 14
-
```

### Comparing `zenutils-0.5.2/tests/test_dictutils.py` & `zenutils-0.5.4/tests/test_dictutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/tests/test_errorutils.py` & `zenutils-0.5.4/tests/test_errorutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 import os
 import sys
 import json
 import unittest
 
 from zenutils import errorutils
 
+
 class TestBizError(unittest.TestCase):
 
     def test01(self):
         e = errorutils.BizError()
         assert e.code
         assert e.message
         assert e.json
@@ -57,28 +66,29 @@
         assert errorutils.OK().message == "正常。"
 
     def test09(self):
         error = errorutils.BizError(RuntimeError("hi"))
         assert error.message == "hi"
 
     def test10(self):
-        error = errorutils.BizError(RuntimeError({
-            "a": "a",
-            "b": [1,2,3],
-            "c": b"hello",
-            "d": os.urandom(1024),
-        }))
+        error = errorutils.BizError(
+            RuntimeError(
+                {
+                    "a": "a",
+                    "b": [1, 2, 3],
+                    "c": b"hello",
+                    "d": os.urandom(1024),
+                }
+            )
+        )
         print(error)
         assert "hello" in error.message
 
     def test11(self):
-        error = errorutils.BizError({
-            "code": 1234,
-            "message": "hello world"
-        })
+        error = errorutils.BizError({"code": 1234, "message": "hello world"})
         assert error.code == 1234
         assert error.message == "hello world"
 
     def test12(self):
         lang = errorutils.get_language()
 
         errorutils.OK().message == "正常。"
@@ -88,32 +98,32 @@
 
         errorutils.set_language(lang)
 
     def test13(self):
         error = errorutils.BizError(ValueError("hello"))
         assert error.code == 226
         assert error.message == "hello"
-    
+
     def test14(self):
         error = errorutils.BizError(ValueError(508, "hello"))
         assert error.code == 508
         assert error.message == "hello"
 
     def test15(self):
         error = errorutils.BizError(ValueError(508, "hello", "world"))
         assert error.code == 508
         assert error.message == """hello world"""
 
     def test18(self):
-        e1 = RuntimeError('hello', 'world')
+        e1 = RuntimeError("hello", "world")
         e2 = errorutils.BizError(e1)
         assert e2.message == "hello world"
 
     def test19(self):
-        e1 = RuntimeError('hello world')
+        e1 = RuntimeError("hello world")
         e2 = errorutils.BizError(e1)
         assert e2.message == "hello world"
 
     def test20(self):
         error_message = "错误原因"
         e1 = RuntimeError(error_message.encode("utf-8"))
         e2 = errorutils.BizError(e1)
@@ -149,10 +159,9 @@
         if PY2:
             d = unicode(a)
             assert d
 
     def test25(self):
         # 具体的异常不能是能用异常
         error = errorutils.BizError(ZeroDivisionError())
-        assert error.code!= 1
+        assert error.code != 1
         assert not error.message in ["Error", "异常！"]
-
```

### Comparing `zenutils-0.5.2/tests/test_fsutils.py` & `zenutils-0.5.4/tests/test_fsutils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 import time
 import uuid
 import os
 import getpass
 
 import unittest
 from zenutils import fsutils
 
+
 class TestFsUtils(unittest.TestCase):
 
     def test01(self):
         folder_name = str(uuid.uuid4())
         assert fsutils.mkdir(folder_name)
         assert fsutils.mkdir(folder_name)
         assert fsutils.rm(folder_name)
@@ -28,15 +37,17 @@
         assert fsutils.rm(filename)
 
     def test03(self):
         filename1 = str(uuid.uuid4())
         content1 = str(uuid.uuid4())
         content2 = str(uuid.uuid4())
         fsutils.write(filename1, content1)
-        file_replaced, file_failed = fsutils.file_content_replace(filename1, content1, content2)
+        file_replaced, file_failed = fsutils.file_content_replace(
+            filename1, content1, content2
+        )
         assert os.path.abspath(file_replaced[0]) == os.path.abspath(filename1)
         assert fsutils.readfile(filename1) == content2
         assert fsutils.rm(filename1)
 
     def test04(self):
         filename = str(uuid.uuid4())
         info1 = fsutils.touch(filename)
@@ -85,15 +96,15 @@
 
     def test09(self):
         src = fsutils.TemporaryFile(content="hello world")
         dst = fsutils.TemporaryFile()
         fsutils.filecopy(src.filepath, dst.filepath)
         dst.open("r", encoding="utf-8")
         assert dst.read() == "hello world"
-    
+
     def test10(self):
         src = fsutils.TemporaryFile(content="hello world")
         dst = str(uuid.uuid4())
         fsutils.mkdir(dst)
         try:
             fsutils.filecopy(src.filepath, dst)
             dst_content = fsutils.readfile(os.path.join(dst, src.filename))
@@ -111,17 +122,17 @@
 
     def test12(self):
         src = fsutils.TemporaryFile(content="hello world")
         assert fsutils.readfile(src.filepath, binary=True) == b"hello world"
 
     def test13(self):
         src = fsutils.TemporaryFile(content="hello world")
-        fsutils.rename(src.filepath, src.filepath+".tmp")
-        assert fsutils.readfile(src.filepath+".tmp") == "hello world"
-        fsutils.rm(src.filepath+".tmp")
+        fsutils.rename(src.filepath, src.filepath + ".tmp")
+        assert fsutils.readfile(src.filepath + ".tmp") == "hello world"
+        fsutils.rm(src.filepath + ".tmp")
 
     def test14(self):
         uid = str(uuid.uuid4())
         os.environ.setdefault("VAR", uid)
         filename = fsutils.expand("~/$VAR/a.txt")
         assert filename
         assert uid in filename
@@ -136,16 +147,16 @@
     def test16(self):
         assert fsutils.get_size_display(0) == "0B"
         assert fsutils.get_size_display(1) == "1B"
         assert fsutils.get_size_display(1023) == "1023B"
         assert fsutils.get_size_display(1024) == "1KB"
         assert fsutils.get_size_display(1025) == "1.00KB"
         assert fsutils.get_size_display(1030) == "1.01KB"
-        assert fsutils.get_size_display(1024*1024) == "1MB"
-        assert fsutils.get_size_display(1024*1024+1) == "1.00MB"
+        assert fsutils.get_size_display(1024 * 1024) == "1MB"
+        assert fsutils.get_size_display(1024 * 1024 + 1) == "1.00MB"
 
     def test17(self):
         filename = str(uuid.uuid4()) + ".txt"
         filename1 = fsutils.get_swap_filename(filename)
         filename2 = fsutils.get_swap_filename(filename)
         assert filename1.startswith("." + filename + ".swap.")
         assert filename1 != filename2
@@ -163,33 +174,38 @@
         filename1 = fsutils.get_swap_filename(filename, prefix=".hello.")
         filename2 = fsutils.get_swap_filename(filename, prefix=".hello.")
         assert filename1.startswith(".hello." + filename + ".swap.")
         assert filename1 != filename2
 
     def test20(self):
         filename = str(uuid.uuid4()) + ".txt"
-        filename1 = fsutils.get_swap_filename(filename, prefix=".hello.", add_random_suffix=False)
-        filename2 = fsutils.get_swap_filename(filename, prefix=".hello.", add_random_suffix=False)
+        filename1 = fsutils.get_swap_filename(
+            filename, prefix=".hello.", add_random_suffix=False
+        )
+        filename2 = fsutils.get_swap_filename(
+            filename, prefix=".hello.", add_random_suffix=False
+        )
         assert filename1.startswith(".hello." + filename + ".swap")
         assert filename1 == filename2
 
     def test21(self):
         assert fsutils.get_safe_filename("a.txt") == "a.txt"
         assert fsutils.get_safe_filename("a.exe") == "a.exe"
         assert fsutils.get_safe_filename("CON") == "_CON"
         assert fsutils.get_safe_filename("a/b.txt") == "a_b.txt"
         assert fsutils.get_safe_filename("a\\b.txt") == "a_b.txt"
         assert fsutils.get_safe_filename("a<b.txt") == "a_b.txt"
         assert fsutils.get_safe_filename("a>b.txt") == "a_b.txt"
         assert fsutils.get_safe_filename("a:b.txt") == "a_b.txt"
-        assert fsutils.get_safe_filename("a\"b.txt") == "a_b.txt"
-        assert fsutils.get_safe_filename("a\'b.txt") == "a_b.txt"
+        assert fsutils.get_safe_filename('a"b.txt') == "a_b.txt"
+        assert fsutils.get_safe_filename("a'b.txt") == "a_b.txt"
         assert fsutils.get_safe_filename("a.") == "a_"
 
     def test22(self):
         if os.name == "posix":
             filename = str(uuid.uuid4())
             filename += "a<b.txt"
-            assert fsutils.get_safe_filename(filename, for_all_platform=False) == filename
+            assert (
+                fsutils.get_safe_filename(filename, for_all_platform=False) == filename
+            )
             fsutils.write(filename, filename)
             fsutils.rm(filename)
-
```

### Comparing `zenutils-0.5.2/tests/test_funcutils.py` & `zenutils-0.5.4/tests/test_funcutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/tests/test_hashutils.py` & `zenutils-0.5.4/tests/test_hashutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/tests/test_httputils.py` & `zenutils-0.5.4/tests/test_httputils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 
 import os
 import uuid
 import unittest
 from zenutils import httputils
 
+
 class TestHttpUtils(unittest.TestCase):
 
     def test01(self):
         info = httputils.get_urlinfo("https://127.0.0.1:8080/tmp/?ts=1234")
         assert info.netloc == "127.0.0.1:8080"
         assert info.scheme == "https"
         assert info.path == "/tmp/"
```

### Comparing `zenutils-0.5.2/tests/test_import_all.py` & `zenutils-0.5.4/tests/test_import_all.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import unittest
 
 from zenutils.base64utils import *
 from zenutils.baseutils import *
 from zenutils.cacheutils import *
 from zenutils.cipherutils import *
 from zenutils.errorutils import *
@@ -27,10 +26,10 @@
 from zenutils.sysutils import *
 from zenutils.threadutils import *
 from zenutils.treeutils import *
 from zenutils.typingutils import *
 
 
 class TestImportAll(unittest.TestCase):
-    
+
     def test01(self):
         assert True
```

### Comparing `zenutils-0.5.2/tests/test_importutils.py` & `zenutils-0.5.4/tests/test_importutils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 import os
 import unittest
 from zenutils.importutils import get_caller_globals
 from zenutils.importutils import get_caller_locals
 from zenutils.importutils import import_module
 from zenutils.importutils import import_from_string
 
 g01 = "hello"
 
+
 class TestImportUtils(unittest.TestCase):
-    
+
     def test01(self):
         def hello():
             return get_caller_locals()
+
         a01 = 12341
         ls = hello()
         print(ls)
         print(ls.keys())
         b01 = ls["a01"]
         assert a01 == b01
 
     def test02(self):
         def hello():
             return get_caller_globals()
+
         gs = hello()
         print(gs)
         print(gs.keys)
         b01 = gs["g01"]
         assert b01 == g01
 
     def test03(self):
@@ -48,51 +59,48 @@
     def test06(self):
         listdir = import_from_string("os.listdir")
         assert callable(listdir)
 
     def test07(self):
         class C(object):
             value = 3
+
         c = C()
-        data = {
-            "a": {
-                "b": {
-                    "c": c
-                }
-            }
-        }
-        v = import_from_string("data.a.b.c.value")
+        data12391981 = {"a": {"b": {"c": c}}}
+        v = import_from_string("data12391981.a.b.c.value")
         assert v == 3
 
     def test08(self):
         none = import_from_string("not-exist-module")
         assert none is None
 
     def test09(self):
         t09 = "hello"
         v09 = import_from_string("t09")
         assert v09 == t09
 
     def test10(self):
         class C(object):
             value = 10
+
         c = C()
         assert import_from_string("c.value") == 10
 
     def test11(self):
         if os.sys.version.startswith("2.6"):
-            self.assertRaises(ImportError, lambda:import_from_string("not-exist-module", slient=False))
+            self.assertRaises(
+                ImportError,
+                lambda: import_from_string("not-exist-module", slient=False),
+            )
         else:
             with self.assertRaises(ImportError):
                 import_from_string("not-exist-module", slient=False)
 
     def test12(self):
-        t12 = [1,2]
+        t12 = [1, 2]
         none = import_from_string("t12.2")
         assert none is None
 
     def test13(self):
         Random = import_from_string("random.Random")
         gen = Random()
-        assert gen.choice([1,2,3])
-    
-
+        assert gen.choice([1, 2, 3])
```

### Comparing `zenutils-0.5.2/tests/test_jsonutils.py` & `zenutils-0.5.4/tests/test_jsonutils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 import unittest
 import os
 import time
 import datetime
 import uuid
 import decimal
 from zenutils import jsonutils
 
 
 class TestJsonUtils(unittest.TestCase):
     def test01(self):
+        """常用类型的序列化。"""
         data = {
             "t1": datetime.datetime.now(),
             "t2": datetime.date(2019, 12, 7),
             "t3": datetime.time(21, 35, 1),
             "uid": uuid.uuid4(),
             "p1": 3.45,
             "p2": decimal.Decimal(1) / decimal.Decimal(7),
@@ -30,28 +39,38 @@
             "d1": decimal.Decimal(1.3),
             "d2": decimal.Decimal(1.1234567),
         }
         result = jsonutils.simple_json_dumps(data, indent=4, ensure_ascii=False)
         assert result
 
     def test02(self):
+        """测试bytes的序列化。"""
         data = {
             "r1": os.urandom(1024),
         }
         result = jsonutils.simple_json_dumps(data, indent=4, ensure_ascii=False)
         assert result
 
+    def test3(self):
+        """测试set的序列化。"""
+        data = {"a": set(["a", "b", "a"])}
+        result = jsonutils.simple_json_dumps(data)
+        assert result
+
     def test99(self):
         try:
             from PIL import Image
         except:
             Image = None
         if Image:
+
             def get_example_image():
-                example_image_path = os.path.abspath(os.path.join(os.path.dirname(__file__), "./assets/p1.jpeg"))
+                example_image_path = os.path.abspath(
+                    os.path.join(os.path.dirname(__file__), "./assets/p1.jpeg")
+                )
                 return Image.open(example_image_path)
 
             im = get_example_image()
             data = {
                 "ts": time.time(),
                 "image": im,
             }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zenutils-0.5.2/tests/test_listutils.py` & `zenutils-0.5.4/tests/test_listutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/tests/test_logutils.py` & `zenutils-0.5.4/tests/test_logutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/tests/test_nameutils.py` & `zenutils-0.5.4/tests/test_nameutils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 import unittest
 from zenutils import nameutils
 
+
 class TestNameUtils(unittest.TestCase):
 
     def test01(self):
         name = nameutils.get_random_name()
         assert 2 <= len(name) <= 4
 
     def test02(self):
```

### Comparing `zenutils-0.5.2/tests/test_numericutils.py` & `zenutils-0.5.4/tests/test_numericutils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,52 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 import os
 import random
 import unittest
 from zenutils import numericutils
 
+
 class TestNumericUtils(unittest.TestCase):
     def test01(self):
         assert numericutils.binary_decompose(0) == set([])
         assert numericutils.binary_decompose(1) == set([1])
         assert numericutils.binary_decompose(2) == set([2])
         assert numericutils.binary_decompose(3) == set([1, 2])
         assert numericutils.binary_decompose(4) == set([4])
         assert numericutils.binary_decompose(5) == set([1, 4])
         assert numericutils.binary_decompose(6) == set([2, 4])
         assert numericutils.binary_decompose(7) == set([1, 2, 4])
         assert numericutils.binary_decompose(8) == set([8])
-    
+
     def test02(self):
         assert numericutils.decimal_change_base(0, 10) == "0"
         assert numericutils.decimal_change_base(1, 10) == "1"
         assert numericutils.decimal_change_base(2, 10) == "2"
         assert numericutils.decimal_change_base(3, 10) == "3"
         assert numericutils.decimal_change_base(4, 10) == "4"
         assert numericutils.decimal_change_base(5, 10) == "5"
         assert numericutils.decimal_change_base(6, 10) == "6"
         assert numericutils.decimal_change_base(7, 10) == "7"
         assert numericutils.decimal_change_base(8, 10) == "8"
         assert numericutils.decimal_change_base(9, 10) == "9"
         assert numericutils.decimal_change_base(10, 10) == "10"
         assert numericutils.decimal_change_base(11, 10) == "11"
 
-
     def test03(self):
         assert numericutils.decimal_change_base(0, 2) == "0"
         assert numericutils.decimal_change_base(1, 2) == "1"
         assert numericutils.decimal_change_base(2, 2) == "10"
         assert numericutils.decimal_change_base(3, 2) == "11"
         assert numericutils.decimal_change_base(4, 2) == "100"
         assert numericutils.decimal_change_base(5, 2) == "101"
@@ -93,15 +101,14 @@
         assert numericutils.get_float_part(-0.001) == 10000
         assert numericutils.get_float_part(-0.0001) == 1000
         assert numericutils.get_float_part(-0.00001) == 100
         assert numericutils.get_float_part(-0.000001) == 10
         assert numericutils.get_float_part(-0.0000001) == 1
         assert numericutils.get_float_part(-0.00000001, 9) == 10
 
-
     def test06(self):
         assert numericutils.float_split(0) == (1, 0, 0)
         assert numericutils.float_split(1) == (1, 1, 0)
         assert numericutils.float_split(-0) == (1, 0, 0)
         assert numericutils.float_split(-1) == (-1, 1, 0)
         assert numericutils.float_split(1.0) == (1, 1, 0)
         assert numericutils.float_split(1.1) == (1, 1, 1000000)
@@ -125,125 +132,138 @@
     def test07(self):
         assert numericutils.is_infinity(float("inf")) is True
         assert numericutils.is_infinity(float("-inf")) is True
         assert numericutils.is_infinity(0.0) is False
         assert numericutils.is_infinity(0.1) is False
 
     def test08(self):
-        assert numericutils._from_bytes(b'hello', 'big') == 448378203247
-        assert numericutils._from_bytes(b'hello', 'big', signed=True) == 448378203247
-        assert numericutils._from_bytes(b'hello', 'little') == 478560413032
-        assert numericutils._from_bytes(b'hello', 'little', signed=True) == 478560413032
-
-        assert numericutils._from_bytes(b'abc', 'big') == 6382179
-        assert numericutils._from_bytes(b'abc', 'big', signed=True) == 6382179
-        assert numericutils._from_bytes(b'abc', 'little') == 6513249
-        assert numericutils._from_bytes(b'abc', 'little', signed=True) == 6513249
-
-        assert numericutils._from_bytes(b'', 'big') == 0
-        assert numericutils._from_bytes(b'', 'big', signed=True) == 0
-        assert numericutils._from_bytes(b'', 'little') == 0
-        assert numericutils._from_bytes(b'', 'little', signed=True) == 0
-
-        assert numericutils._from_bytes(b'\xff', 'big') == 255
-        assert numericutils._from_bytes(b'\xff', 'big', signed=True) == -1
-        assert numericutils._from_bytes(b'\xff', 'little') == 255
-        assert numericutils._from_bytes(b'\xff', 'little', signed=True) == -1
-
-        assert numericutils._from_bytes(b'\xff\xaa', 'big') == 65450
-        assert numericutils._from_bytes(b'\xff\xaa', 'big', signed=True) == -86
-        assert numericutils._from_bytes(b'\xff\xaa', 'little') == 43775
-        assert numericutils._from_bytes(b'\xff\xaa', 'little', signed=True) == -21761
+        assert numericutils._from_bytes(b"hello", "big") == 448378203247
+        assert numericutils._from_bytes(b"hello", "big", signed=True) == 448378203247
+        assert numericutils._from_bytes(b"hello", "little") == 478560413032
+        assert numericutils._from_bytes(b"hello", "little", signed=True) == 478560413032
+
+        assert numericutils._from_bytes(b"abc", "big") == 6382179
+        assert numericutils._from_bytes(b"abc", "big", signed=True) == 6382179
+        assert numericutils._from_bytes(b"abc", "little") == 6513249
+        assert numericutils._from_bytes(b"abc", "little", signed=True) == 6513249
+
+        assert numericutils._from_bytes(b"", "big") == 0
+        assert numericutils._from_bytes(b"", "big", signed=True) == 0
+        assert numericutils._from_bytes(b"", "little") == 0
+        assert numericutils._from_bytes(b"", "little", signed=True) == 0
+
+        assert numericutils._from_bytes(b"\xff", "big") == 255
+        assert numericutils._from_bytes(b"\xff", "big", signed=True) == -1
+        assert numericutils._from_bytes(b"\xff", "little") == 255
+        assert numericutils._from_bytes(b"\xff", "little", signed=True) == -1
+
+        assert numericutils._from_bytes(b"\xff\xaa", "big") == 65450
+        assert numericutils._from_bytes(b"\xff\xaa", "big", signed=True) == -86
+        assert numericutils._from_bytes(b"\xff\xaa", "little") == 43775
+        assert numericutils._from_bytes(b"\xff\xaa", "little", signed=True) == -21761
 
     def test09(self):
         data = b"\xfbv\x9dq6\x94\xa1\xe2\xa0P\xa8\x96\xac\xe3O\x8b\x0bi\x9a\xe9\xea\x92@\x08)\xee\x8a\x15\t%\xe6\x90\xa8\xcfJ\nX\xe6\x12\x96\x97G\xa5'm\x8b\x13\xc5m\xaf\xb9\x9f"
         value = 166231341758227121687846500029642935057146082350369973176474181511812540102287508707676189261858076641625610704832490992810399
-        assert numericutils._from_bytes(data, 'big', signed=False) == value
+        assert numericutils._from_bytes(data, "big", signed=False) == value
 
     def test10(self):
         if hasattr(int, "from_bytes"):
             for i in range(1024):
                 length = random.randint(0, 1024)
                 data = os.urandom(length)
-                assert int.from_bytes(data, "big", signed=False) == numericutils._from_bytes(data, "big", signed=False)
-                assert int.from_bytes(data, "big", signed=True) == numericutils._from_bytes(data, "big", signed=True)
-                assert int.from_bytes(data, "little", signed=False) == numericutils._from_bytes(data, "little", signed=False)
-                assert int.from_bytes(data, "little", signed=True) == numericutils._from_bytes(data, "little", signed=True)
+                assert int.from_bytes(
+                    data, "big", signed=False
+                ) == numericutils._from_bytes(data, "big", signed=False)
+                assert int.from_bytes(
+                    data, "big", signed=True
+                ) == numericutils._from_bytes(data, "big", signed=True)
+                assert int.from_bytes(
+                    data, "little", signed=False
+                ) == numericutils._from_bytes(data, "little", signed=False)
+                assert int.from_bytes(
+                    data, "little", signed=True
+                ) == numericutils._from_bytes(data, "little", signed=True)
 
     def test11(self):
         for i in range(1024):
             length = random.randint(0, 1024)
             data1 = os.urandom(length)
             data2 = numericutils.from_bytes(data1)
             data3 = numericutils.int2bytes(data2)
             assert data1.strip(b"\x00") == data3.strip(b"\x00")
 
     def test12(self):
-        assert numericutils.int2bytes(0) ==  b'\x00'
-        assert numericutils.int2bytes(1) ==  b'\x01'
-        assert numericutils.int2bytes(127) ==  b'\x7f'
-        assert numericutils.int2bytes(128) ==  b'\x80'
-        assert numericutils.int2bytes(255) ==  b'\xff'
-        assert numericutils.int2bytes(256) ==  b'\x01\x00'
-        assert numericutils.int2bytes(512) ==  b'\x02\x00'
-        assert numericutils.int2bytes(513) ==  b'\x02\x01'
-        assert numericutils.int2bytes(1023) ==  b'\x03\xff'
-        assert numericutils.int2bytes(1024) ==  b'\x04\x00'
-        assert numericutils.int2bytes(1025) ==  b'\x04\x01'
+        assert numericutils.int2bytes(0) == b"\x00"
+        assert numericutils.int2bytes(1) == b"\x01"
+        assert numericutils.int2bytes(127) == b"\x7f"
+        assert numericutils.int2bytes(128) == b"\x80"
+        assert numericutils.int2bytes(255) == b"\xff"
+        assert numericutils.int2bytes(256) == b"\x01\x00"
+        assert numericutils.int2bytes(512) == b"\x02\x00"
+        assert numericutils.int2bytes(513) == b"\x02\x01"
+        assert numericutils.int2bytes(1023) == b"\x03\xff"
+        assert numericutils.int2bytes(1024) == b"\x04\x00"
+        assert numericutils.int2bytes(1025) == b"\x04\x01"
 
     def test13(self):
-        assert numericutils._int2bytes(0) ==  b'\x00'
-        assert numericutils._int2bytes(1) ==  b'\x01'
-        assert numericutils._int2bytes(127) ==  b'\x7f'
-        assert numericutils._int2bytes(128) ==  b'\x80'
-        assert numericutils._int2bytes(255) ==  b'\xff'
-        assert numericutils._int2bytes(256) ==  b'\x01\x00'
-        assert numericutils._int2bytes(512) ==  b'\x02\x00'
-        assert numericutils._int2bytes(513) ==  b'\x02\x01'
-        assert numericutils._int2bytes(1023) ==  b'\x03\xff'
-        assert numericutils._int2bytes(1024) ==  b'\x04\x00'
-        assert numericutils._int2bytes(1025) ==  b'\x04\x01'
+        assert numericutils._int2bytes(0) == b"\x00"
+        assert numericutils._int2bytes(1) == b"\x01"
+        assert numericutils._int2bytes(127) == b"\x7f"
+        assert numericutils._int2bytes(128) == b"\x80"
+        assert numericutils._int2bytes(255) == b"\xff"
+        assert numericutils._int2bytes(256) == b"\x01\x00"
+        assert numericutils._int2bytes(512) == b"\x02\x00"
+        assert numericutils._int2bytes(513) == b"\x02\x01"
+        assert numericutils._int2bytes(1023) == b"\x03\xff"
+        assert numericutils._int2bytes(1024) == b"\x04\x00"
+        assert numericutils._int2bytes(1025) == b"\x04\x01"
 
     def test14(self):
         if hasattr(int, "to_bytes"):
             for i in range(2048):
                 length = random.randint(8, 16)
-                assert numericutils.int2bytes(i, length) == i.to_bytes(length, 'big')
-                assert numericutils.int2bytes(i, length, 'little') == i.to_bytes(length, 'little')
+                assert numericutils.int2bytes(i, length) == i.to_bytes(length, "big")
+                assert numericutils.int2bytes(i, length, "little") == i.to_bytes(
+                    length, "little"
+                )
             for i in range(2048):
                 i *= -1
                 length = random.randint(8, 16)
-                assert numericutils.int2bytes(i, length, signed=True) == i.to_bytes(length, 'big', signed=True)
-                assert numericutils.int2bytes(i, length, 'little', signed=True) == i.to_bytes(length, 'little', signed=True)
+                assert numericutils.int2bytes(i, length, signed=True) == i.to_bytes(
+                    length, "big", signed=True
+                )
+                assert numericutils.int2bytes(
+                    i, length, "little", signed=True
+                ) == i.to_bytes(length, "little", signed=True)
 
     def test15(self):
-        assert numericutils._int2bytes(-1, signed=True) == b'\xff'
-        assert numericutils._int2bytes(-2, signed=True) == b'\xfe'
-        assert numericutils._int2bytes(-127, signed=True) == b'\x81'
-        assert numericutils._int2bytes(-128, signed=True) == b'\x80'
-        assert numericutils._int2bytes(-129, signed=True) == b'\xff\x7f'
-        assert numericutils._int2bytes(-255, signed=True) == b'\xff\x01'
-        assert numericutils._int2bytes(-256, signed=True) == b'\xff\x00'
-        assert numericutils._int2bytes(-257, signed=True) == b'\xfe\xff'
-        assert numericutils._int2bytes(-511, signed=True) == b'\xfe\x01'
-        assert numericutils._int2bytes(-512, signed=True) == b'\xfe\x00'
-        assert numericutils._int2bytes(-513, signed=True) == b'\xfd\xff'
-        assert numericutils._int2bytes(-1023, signed=True) == b'\xfc\x01'
-        assert numericutils._int2bytes(-1024, signed=True) == b'\xfc\x00'
-        assert numericutils._int2bytes(-1025, signed=True) == b'\xfb\xff'
+        assert numericutils._int2bytes(-1, signed=True) == b"\xff"
+        assert numericutils._int2bytes(-2, signed=True) == b"\xfe"
+        assert numericutils._int2bytes(-127, signed=True) == b"\x81"
+        assert numericutils._int2bytes(-128, signed=True) == b"\x80"
+        assert numericutils._int2bytes(-129, signed=True) == b"\xff\x7f"
+        assert numericutils._int2bytes(-255, signed=True) == b"\xff\x01"
+        assert numericutils._int2bytes(-256, signed=True) == b"\xff\x00"
+        assert numericutils._int2bytes(-257, signed=True) == b"\xfe\xff"
+        assert numericutils._int2bytes(-511, signed=True) == b"\xfe\x01"
+        assert numericutils._int2bytes(-512, signed=True) == b"\xfe\x00"
+        assert numericutils._int2bytes(-513, signed=True) == b"\xfd\xff"
+        assert numericutils._int2bytes(-1023, signed=True) == b"\xfc\x01"
+        assert numericutils._int2bytes(-1024, signed=True) == b"\xfc\x00"
+        assert numericutils._int2bytes(-1025, signed=True) == b"\xfb\xff"
 
     def test16(self):
-        assert numericutils.int2bytes(-1, signed=True) == b'\xff'
-        assert numericutils.int2bytes(-2, signed=True) == b'\xfe'
-        assert numericutils.int2bytes(-127, signed=True) == b'\x81'
-        assert numericutils.int2bytes(-128, signed=True) == b'\x80'
-        assert numericutils.int2bytes(-129, signed=True) == b'\xff\x7f'
-        assert numericutils.int2bytes(-255, signed=True) == b'\xff\x01'
-        assert numericutils.int2bytes(-256, signed=True) == b'\xff\x00'
-        assert numericutils.int2bytes(-257, signed=True) == b'\xfe\xff'
-        assert numericutils.int2bytes(-511, signed=True) == b'\xfe\x01'
-        assert numericutils.int2bytes(-512, signed=True) == b'\xfe\x00'
-        assert numericutils.int2bytes(-513, signed=True) == b'\xfd\xff'
-        assert numericutils.int2bytes(-1023, signed=True) == b'\xfc\x01'
-        assert numericutils.int2bytes(-1024, signed=True) == b'\xfc\x00'
-        assert numericutils.int2bytes(-1025, signed=True) == b'\xfb\xff'
-
+        assert numericutils.int2bytes(-1, signed=True) == b"\xff"
+        assert numericutils.int2bytes(-2, signed=True) == b"\xfe"
+        assert numericutils.int2bytes(-127, signed=True) == b"\x81"
+        assert numericutils.int2bytes(-128, signed=True) == b"\x80"
+        assert numericutils.int2bytes(-129, signed=True) == b"\xff\x7f"
+        assert numericutils.int2bytes(-255, signed=True) == b"\xff\x01"
+        assert numericutils.int2bytes(-256, signed=True) == b"\xff\x00"
+        assert numericutils.int2bytes(-257, signed=True) == b"\xfe\xff"
+        assert numericutils.int2bytes(-511, signed=True) == b"\xfe\x01"
+        assert numericutils.int2bytes(-512, signed=True) == b"\xfe\x00"
+        assert numericutils.int2bytes(-513, signed=True) == b"\xfd\xff"
+        assert numericutils.int2bytes(-1023, signed=True) == b"\xfc\x01"
+        assert numericutils.int2bytes(-1024, signed=True) == b"\xfc\x00"
+        assert numericutils.int2bytes(-1025, signed=True) == b"\xfb\xff"
```

### Comparing `zenutils-0.5.2/tests/test_packutils.py` & `zenutils-0.5.4/tests/test_packutils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 import unittest
 from zenutils import packutils
 from zenutils import errorutils
 
+
 class TestPackUtils(unittest.TestCase):
 
     def test01(self):
         pack = packutils.RcmPacker()
         package = pack.pack_result("hello")
         assert package["result"] == "hello"
         assert package["code"] == 0
```

### Comparing `zenutils-0.5.2/tests/test_serviceutils.py` & `zenutils-0.5.4/tests/test_serviceutils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 import unittest
 from zenutils import serviceutils
 
+
 class TestServiceUtils(unittest.TestCase):
 
     def test01(self):
         service = serviceutils.DebugService()
         assert service.ping() == "pong"
-    
+
     def test02(self):
         config = {}
         service = serviceutils.DebugService(config)
         assert service.echo("hello world") == "hello world"
 
     def test03(self):
         service = serviceutils.DebugService()
@@ -37,21 +46,19 @@
         assert methods
         assert isinstance(methods, list)
         assert "ping" in dict(methods)
 
     def test06(self):
         service = serviceutils.DebugService()
         assert service.get_ignore_methods()
-    
+
     def test07(self):
         service = serviceutils.DebugService()
         assert service.get_namespace() == "debug"
-    
+
     def test08(self):
         service = serviceutils.DebugService(namespace="test")
         assert service.get_namespace() == "test"
 
     def test09(self):
         service = serviceutils.DebugService(namespace="")
         assert service.get_namespace() == ""
-
-
```

### Comparing `zenutils-0.5.2/tests/test_sixutils.py` & `zenutils-0.5.4/tests/test_sixutils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 import os
 import unittest
 from zenutils import sixutils
 from zenutils import strutils
 
 
 class TestSixUtils(unittest.TestCase):
 
     def test01(self):
         assert sixutils.bytes_to_array(b"hello") == [b"h", b"e", b"l", b"l", b"o"]
-    
+
     def test02(self):
         assert sixutils.bstr_to_array(b"hello") == [b"h", b"e", b"l", b"l", b"o"]
         assert sixutils.bstr_to_array("hello") == ["h", "e", "l", "l", "o"]
         data = sixutils.bstr_to_array(os.urandom(16))
         for c in data:
             assert isinstance(c, sixutils.BYTES_TYPE)
         data = sixutils.bstr_to_array(strutils.random_string(16))
@@ -42,67 +50,75 @@
         assert sixutils.bchar(255) == b"\xff"
 
     def test04(self):
         assert sixutils.force_bytes("hello") == b"hello"
         assert sixutils.force_bytes(b"hello") == b"hello"
         assert sixutils.force_text("hello") == "hello"
         assert sixutils.force_text(b"hello") == "hello"
-    
+
     def test05(self):
         assert sixutils.force_bytes(None) is None
         assert sixutils.force_text(None) is None
-    
+
     def test06(self):
-        assert sixutils.force_bytes(lambda:"hello") == b"hello"
-        assert sixutils.force_bytes(lambda:b"hello") == b"hello"
-        assert sixutils.force_text(lambda:"hello") == "hello"
-        assert sixutils.force_text(lambda:b"hello") == "hello"
-
-        assert sixutils.BYTES(lambda:"hello") == b"hello"
-        assert sixutils.BYTES(lambda:b"hello") == b"hello"
-        assert sixutils.TEXT(lambda:"hello") == "hello"
-        assert sixutils.TEXT(lambda:b"hello") == "hello"
+        assert sixutils.force_bytes(lambda: "hello") == b"hello"
+        assert sixutils.force_bytes(lambda: b"hello") == b"hello"
+        assert sixutils.force_text(lambda: "hello") == "hello"
+        assert sixutils.force_text(lambda: b"hello") == "hello"
+
+        assert sixutils.BYTES(lambda: "hello") == b"hello"
+        assert sixutils.BYTES(lambda: b"hello") == b"hello"
+        assert sixutils.TEXT(lambda: "hello") == "hello"
+        assert sixutils.TEXT(lambda: b"hello") == "hello"
 
     def test07(self):
         class Hello(object):
             def __init__(self, name):
                 self.name = name
-            
+
             def __repr__(self):
                 return "hi, {name}.".format(name=self.name)
 
-        assert sixutils.force_bytes(lambda:Hello("tom")) == b"hi, tom."
-        assert sixutils.force_text(lambda:Hello("tom")) == "hi, tom."
+        assert sixutils.force_bytes(lambda: Hello("tom")) == b"hi, tom."
+        assert sixutils.force_text(lambda: Hello("tom")) == "hi, tom."
         assert sixutils.force_bytes(Hello("tom")) == b"hi, tom."
         assert sixutils.force_text(Hello("tom")) == "hi, tom."
-    
+
     def test08(self):
         with self.assertRaises(UnicodeDecodeError):
             sixutils.TEXT(os.urandom(1024))
 
     def test09(self):
-        assert sixutils.force_bytes(b'hello') == b'hello'
-        assert sixutils.force_bytes('测试') == '测试'.encode('utf-8')
-        assert sixutils.force_bytes('hello') == b'hello'
-        assert sixutils.force_bytes(1234) == b'1234'
-        assert sixutils.force_bytes([1,2,3]) == b"[1, 2, 3]"
-    
+        assert sixutils.force_bytes(b"hello") == b"hello"
+        assert sixutils.force_bytes("测试") == "测试".encode("utf-8")
+        assert sixutils.force_bytes("hello") == b"hello"
+        assert sixutils.force_bytes(1234) == b"1234"
+        assert sixutils.force_bytes([1, 2, 3]) == b"[1, 2, 3]"
+
     def test10(self):
-        assert sixutils.force_text(b'hello') == 'hello'
-        assert sixutils.force_text('测试'.encode('utf-8')) == '测试'
-        assert sixutils.force_text('hello') == 'hello'
-        assert sixutils.force_text(1234) == '1234'
-        assert sixutils.force_text([1,2,3]) == "[1, 2, 3]"
+        assert sixutils.force_text(b"hello") == "hello"
+        assert sixutils.force_text("测试".encode("utf-8")) == "测试"
+        assert sixutils.force_text("hello") == "hello"
+        assert sixutils.force_text(1234) == "1234"
+        assert sixutils.force_text([1, 2, 3]) == "[1, 2, 3]"
 
     def test11(self):
         data = {"测试": "测试"}
         if sixutils.PY2:
-            assert sixutils.force_text(data) == """{u'\\u6d4b\\u8bd5': u'\\u6d4b\\u8bd5'}"""
+            assert (
+                sixutils.force_text(data)
+                == """{u'\\u6d4b\\u8bd5': u'\\u6d4b\\u8bd5'}"""
+            )
         else:
             assert sixutils.force_text(data) == """{'测试': '测试'}"""
 
     def test12(self):
         data = {"测试": "测试"}
         if sixutils.PY2:
-            assert sixutils.force_bytes(data) == b"{u'\\u6d4b\\u8bd5': u'\\u6d4b\\u8bd5'}"
+            assert (
+                sixutils.force_bytes(data) == b"{u'\\u6d4b\\u8bd5': u'\\u6d4b\\u8bd5'}"
+            )
         else:
-            assert sixutils.force_bytes(data) == b"{'\xe6\xb5\x8b\xe8\xaf\x95': '\xe6\xb5\x8b\xe8\xaf\x95'}"
+            assert (
+                sixutils.force_bytes(data)
+                == b"{'\xe6\xb5\x8b\xe8\xaf\x95': '\xe6\xb5\x8b\xe8\xaf\x95'}"
+            )
```

### Comparing `zenutils-0.5.2/tests/test_strutils.py` & `zenutils-0.5.4/tests/test_strutils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 """
 String operate functions.
 
 """
 import os
@@ -15,18 +23,25 @@
 import uuid
 from decimal import Decimal
 
 from zenutils import strutils
 from zenutils import base64utils
 from zenutils import nameutils
 
+
 def get_test_assets(filename):
-    return os.path.abspath(os.path.join(os.path.dirname(__file__), "./assets/{filename}".format(
-        filename=filename,
-    )))
+    return os.path.abspath(
+        os.path.join(
+            os.path.dirname(__file__),
+            "./assets/{filename}".format(
+                filename=filename,
+            ),
+        )
+    )
+
 
 class TestStrUtils(unittest.TestCase):
 
     def test01(self):
         text = "1,2.3,4.5"
         values = strutils.split(text, [",", "."])
         assert values == ["1", "2", "3", "4", "5"]
@@ -137,27 +152,45 @@
     def test11(self):
         assert strutils.text_display_shorten("", 5) == strutils.force_text("")
         assert strutils.text_display_shorten("a", 5) == strutils.force_text("a")
         assert strutils.text_display_shorten("ab", 5) == strutils.force_text("ab")
         assert strutils.text_display_shorten("abc", 5) == strutils.force_text("abc")
         assert strutils.text_display_shorten("abcd", 5) == strutils.force_text("abcd")
         assert strutils.text_display_shorten("abcde", 5) == strutils.force_text("abcde")
-        assert strutils.text_display_shorten("abcdef", 5) == strutils.force_text("ab...")
-        assert strutils.text_display_shorten("abcdefg", 5) == strutils.force_text("ab...")
-        assert strutils.text_display_shorten("abcdefgh", 5) == strutils.force_text("ab...")
+        assert strutils.text_display_shorten("abcdef", 5) == strutils.force_text(
+            "ab..."
+        )
+        assert strutils.text_display_shorten("abcdefg", 5) == strutils.force_text(
+            "ab..."
+        )
+        assert strutils.text_display_shorten("abcdefgh", 5) == strutils.force_text(
+            "ab..."
+        )
         assert strutils.text_display_shorten("测", 5) == strutils.force_text("测")
         assert strutils.text_display_shorten("测测", 5) == strutils.force_text("测测")
-        assert strutils.text_display_shorten("测测测", 5) == strutils.force_text("测...")
-        assert strutils.text_display_shorten("测测测测", 5) == strutils.force_text("测...")
-        assert strutils.text_display_shorten("测测测测测", 5) == strutils.force_text("测...")
+        assert strutils.text_display_shorten("测测测", 5) == strutils.force_text(
+            "测..."
+        )
+        assert strutils.text_display_shorten("测测测测", 5) == strutils.force_text(
+            "测..."
+        )
+        assert strutils.text_display_shorten("测测测测测", 5) == strutils.force_text(
+            "测..."
+        )
         assert strutils.text_display_shorten("a测", 5) == strutils.force_text("a测")
         assert strutils.text_display_shorten("a测测", 5) == strutils.force_text("a测测")
-        assert strutils.text_display_shorten("a测测测", 5) == strutils.force_text("a...")
-        assert strutils.text_display_shorten("a测测测测", 5) == strutils.force_text("a...")
-        assert strutils.text_display_shorten("a测测测测测", 5) == strutils.force_text("a...")
+        assert strutils.text_display_shorten("a测测测", 5) == strutils.force_text(
+            "a..."
+        )
+        assert strutils.text_display_shorten("a测测测测", 5) == strutils.force_text(
+            "a..."
+        )
+        assert strutils.text_display_shorten("a测测测测测", 5) == strutils.force_text(
+            "a..."
+        )
 
     def test12(self):
         assert strutils.wholestrip("a b") == "ab"
         assert strutils.wholestrip(" a b ") == "ab"
 
     def test13(self):
         s1 = os.urandom(random.randint(0, 1024))
@@ -179,18 +212,21 @@
         for length in range(1024):
             a = os.urandom(length)
             b = strutils.binarify(a)
             c = strutils.unbinarify(b)
             assert a == c
 
     def test16(self):
-        assert strutils.ints2bytes([]) == b''
-        assert strutils.ints2bytes([ord('a'), ord('b'), ord('c')]) == b'abc'
-        assert strutils.ints2bytes([0, 1, 2, 255]) == b'\x00\x01\x02\xff'
-        assert strutils.ints2bytes([256, 257, 65534, 65535, 65536]) == b'\x01\x00\x01\x01\xff\xfe\xff\xff\x01\x00\x00'
+        assert strutils.ints2bytes([]) == b""
+        assert strutils.ints2bytes([ord("a"), ord("b"), ord("c")]) == b"abc"
+        assert strutils.ints2bytes([0, 1, 2, 255]) == b"\x00\x01\x02\xff"
+        assert (
+            strutils.ints2bytes([256, 257, 65534, 65535, 65536])
+            == b"\x01\x00\x01\x01\xff\xfe\xff\xff\x01\x00\x00"
+        )
 
     def test17(self):
         assert strutils.force_numberic(1) == 1
         assert strutils.force_numberic(1.2) == 1.2
         assert strutils.force_numberic("1") == 1
         assert strutils.force_numberic("1.2") == 1.2
 
@@ -211,31 +247,35 @@
         assert strutils.force_text(t1.encode("gbk"), ["utf-8", "gb18030"]) == t1
 
     def test21(self):
         assert len(strutils.substrings("")) == 0
         assert len(strutils.substrings("a")) == 1
         assert len(strutils.substrings("ab")) == 3
         assert len(strutils.substrings("aa")) == 2
-        assert len(strutils.substrings("abc")) == len(["a", "b", "c", "ab", "bc", "abc"])
+        assert len(strutils.substrings("abc")) == len(
+            ["a", "b", "c", "ab", "bc", "abc"]
+        )
         assert len(strutils.substrings("abc", 2)) == len(["ab", "bc"])
         assert len(strutils.substrings("abc", 3)) == 1
         assert len(strutils.substrings("abc", 1)) == 3
         assert len(strutils.substrings("abc", [1, 2])) == 5
         assert len(strutils.substrings(b"abc", [1, 2])) == 5
-        assert len(strutils.substrings(b"abc")) == len([b"a", b"b", b"c", b"ab", b"bc", b"abc"])
+        assert len(strutils.substrings(b"abc")) == len(
+            [b"a", b"b", b"c", b"ab", b"bc", b"abc"]
+        )
 
     def test22(self):
-        assert len(strutils.combinations("a", 2)) == 1 ** 2
-        assert len(strutils.combinations("ab", 2)) == 2 ** 2
-        assert len(strutils.combinations("abc", 2)) == 3 ** 2
-        assert len(strutils.combinations("a", 3)) == 1 ** 3
-        assert len(strutils.combinations("ab", 3)) == 2 ** 3
-        assert len(strutils.combinations(string.digits, 2)) == 10 ** 2
-        assert len(strutils.combinations(string.digits, 3)) == 10 ** 3
-        assert len(strutils.combinations(string.ascii_lowercase, 3)) == 26 ** 3
+        assert len(strutils.combinations("a", 2)) == 1**2
+        assert len(strutils.combinations("ab", 2)) == 2**2
+        assert len(strutils.combinations("abc", 2)) == 3**2
+        assert len(strutils.combinations("a", 3)) == 1**3
+        assert len(strutils.combinations("ab", 3)) == 2**3
+        assert len(strutils.combinations(string.digits, 2)) == 10**2
+        assert len(strutils.combinations(string.digits, 3)) == 10**3
+        assert len(strutils.combinations(string.ascii_lowercase, 3)) == 26**3
         assert len(strutils.combinations(["a", "cd"], 3)) == 8
         assert len(strutils.combinations(["ab", "cd"], 3)) == 8
         assert len(strutils.combinations([b"ab", b"cd"], 3)) == 8
         assert len(strutils.combinations(["aa", "bb"], 3)) == 6
         assert len(strutils.combinations(["abc"], 1)) == 3
         assert len(strutils.combinations(["abc"], 2)) == 3
         assert len(strutils.combinations(["abc"], 3)) == 3
@@ -267,15 +307,18 @@
         assert strutils.captital_number(112005) == "壹拾壹万贰仟零伍圆"
         assert strutils.captital_number(10112005) == "壹仟零壹拾壹万贰仟零伍圆"
         assert strutils.captital_number(100000000) == "壹亿圆"
         assert strutils.captital_number(100000002) == "壹亿零贰圆"
         assert strutils.captital_number(100030000) == "壹亿零叁万圆"
         assert strutils.captital_number(100003000) == "壹亿零叁仟圆"
         assert strutils.captital_number(123100003000) == "壹仟贰佰叁拾壹亿零叁仟圆"
-        assert strutils.captital_number(1234567890123) == "壹万贰仟叁佰肆拾伍亿陆仟柒佰捌拾玖万零壹佰贰拾叁圆"
+        assert (
+            strutils.captital_number(1234567890123)
+            == "壹万贰仟叁佰肆拾伍亿陆仟柒佰捌拾玖万零壹佰贰拾叁圆"
+        )
         assert strutils.captital_number(1234567) == "壹佰贰拾叁万肆仟伍佰陆拾柒圆"
 
     def test24(self):
         assert strutils.captital_number(0.1) == "零圆壹角"
         assert strutils.captital_number(0.01) == "零圆壹分"
         assert strutils.captital_number(0.001) == "零圆壹厘"
         assert strutils.captital_number(0.0001) == "零圆壹毫"
@@ -285,15 +328,17 @@
         assert strutils.captital_number(0.00000001) == "零圆"
         assert strutils.captital_number(0.12) == "零圆壹角贰分"
         assert strutils.captital_number(0.123) == "零圆壹角贰分叁厘"
         assert strutils.captital_number(0.1234) == "零圆壹角贰分叁厘肆毫"
         assert strutils.captital_number(0.12345) == "零圆壹角贰分叁厘肆毫伍丝"
         assert strutils.captital_number(0.123456) == "零圆壹角贰分叁厘肆毫伍丝陆忽"
         assert strutils.captital_number(0.1234567) == "零圆壹角贰分叁厘肆毫伍丝陆忽柒微"
-        assert strutils.captital_number(0.12345678) == "零圆壹角贰分叁厘肆毫伍丝陆忽柒微"
+        assert (
+            strutils.captital_number(0.12345678) == "零圆壹角贰分叁厘肆毫伍丝陆忽柒微"
+        )
 
     def test25(self):
         assert strutils.camel("hello") == "Hello"
         assert strutils.camel("hello world") == "Hello World"
         assert strutils.camel(" hello ") == " Hello "
         assert strutils.camel("hello  world") == "Hello  World"
         assert strutils.camel("hello-world") == "Hello-World"
@@ -303,43 +348,63 @@
         assert strutils.camel("hello world", clean=True) == "HelloWorld"
         assert strutils.camel(" hello ", clean=True) == "Hello"
         assert strutils.camel("hello  world", clean=True) == "HelloWorld"
         assert strutils.camel("hello-world", clean=True) == "HelloWorld"
         assert strutils.camel("hello_world", clean=True) == "HelloWorld"
 
     def test26(self):
-        assert strutils.format_with_mapping("{}{}", strutils.none_to_empty_string, 1, None) == "1"
-        assert strutils.format_with_mapping("{a}{b}", strutils.none_to_empty_string, a=1, b=None) == "1"
-        assert strutils.format_with_mapping("{}{a}{}{b}", strutils.none_to_empty_string, 1, None, a=3, b=None) == "13"
-        assert strutils.format_with_mapping("{:d}:{:}", strutils.no_mapping, 1, None) == "1:None"
+        assert (
+            strutils.format_with_mapping("{}{}", strutils.none_to_empty_string, 1, None)
+            == "1"
+        )
+        assert (
+            strutils.format_with_mapping(
+                "{a}{b}", strutils.none_to_empty_string, a=1, b=None
+            )
+            == "1"
+        )
+        assert (
+            strutils.format_with_mapping(
+                "{}{a}{}{b}", strutils.none_to_empty_string, 1, None, a=3, b=None
+            )
+            == "13"
+        )
+        assert (
+            strutils.format_with_mapping("{:d}:{:}", strutils.no_mapping, 1, None)
+            == "1:None"
+        )
 
     def test27(self):
         assert strutils.unquote('''"hello"''') == "hello"
         assert strutils.unquote('"""hello"""') == "hello"
-        assert strutils.unquote('“hello”') == "hello"
-        assert strutils.unquote('‘hello’') == "hello"
+        assert strutils.unquote("“hello”") == "hello"
+        assert strutils.unquote("‘hello’") == "hello"
 
     def test28(self):
         assert strutils.is_uuid(uuid.uuid4())
         assert strutils.is_uuid(uuid.uuid4().bytes)
         assert strutils.is_uuid("abc") == False
         assert strutils.is_uuid("abcdefghijklmnopqrstuvwxyz") == False
         assert strutils.is_uuid("{12345678-1234-5678-1234-567812345678}")
         assert strutils.is_uuid("12345678123456781234567812345678")
         assert strutils.is_uuid("12345678-1234-5678-1234-567812345678")
         assert strutils.is_uuid(strutils.force_text(uuid.uuid4().hex))
         assert strutils.is_uuid(uuid.uuid4().hex)
 
     def test29(self):
-        assert strutils.camel("hello world", clean=True, lower_first=True) == "helloWorld"
+        assert (
+            strutils.camel("hello world", clean=True, lower_first=True) == "helloWorld"
+        )
 
     def test30(self):
         assert strutils.stringlist_append("a b c", "a", separator=" ") == "a b c a"
         assert strutils.stringlist_append("a,b,c", "a") == "a,b,c,a"
-        assert strutils.stringlist_append("a,b,c", "a", allow_duplicate=False) == "a,b,c"
+        assert (
+            strutils.stringlist_append("a,b,c", "a", allow_duplicate=False) == "a,b,c"
+        )
 
     def test31(self):
         assert strutils.is_urlsafeb64_decodable("abcd") is True
 
     def test32(self):
         assert strutils.html_element_css_append("a b c", "a") == "a b c"
         assert strutils.html_element_css_append("a b c", "d") == "a b c d"
@@ -357,17 +422,30 @@
     def test35(self):
         assert strutils.split2("hello world") == ["hello", "world"]
         assert strutils.split2("hello world !") == ["hello", "world !"]
         assert strutils.split2("1,2,3", ",") == ["1", "2,3"]
 
     def test36(self):
         assert strutils.is_uuid("90a0332d-7f06-gace-a1e2-3c27e634c17f") == False
-        assert strutils.is_uuid("90a0332d-7f06-gace-a1e2-3c27e634c17f", allow_bad_characters=True) == True
-        assert strutils.is_uuid("90a0332d-7f06-gace-a1e2-3c27e634c17f-x", allow_bad_characters=True) == False
-        assert strutils.is_uuid("123412341234123412341234", allow_bad_characters=True) == False
+        assert (
+            strutils.is_uuid(
+                "90a0332d-7f06-gace-a1e2-3c27e634c17f", allow_bad_characters=True
+            )
+            == True
+        )
+        assert (
+            strutils.is_uuid(
+                "90a0332d-7f06-gace-a1e2-3c27e634c17f-x", allow_bad_characters=True
+            )
+            == False
+        )
+        assert (
+            strutils.is_uuid("123412341234123412341234", allow_bad_characters=True)
+            == False
+        )
 
     def test37(self):
         assert strutils.chunk("", 2) == []
         assert strutils.chunk("1", 2) == ["1"]
         assert strutils.chunk("12", 2) == ["12"]
         assert strutils.chunk("123", 2) == ["12", "3"]
         assert strutils.chunk("1234", 2) == ["12", "34"]
@@ -375,32 +453,48 @@
         assert strutils.chunk("1", 1) == ["1"]
         assert strutils.chunk("12", 1) == ["1", "2"]
         assert strutils.chunk("123", 1) == ["1", "2", "3"]
 
     def test38(self):
         assert strutils.get_all_substrings("a") == set(["a"])
         assert strutils.get_all_substrings("ab") == set(["a", "b", "ab"])
-        assert strutils.get_all_substrings("abc") == set(["a", "b", "c", "ab", "bc", "abc"])
-        assert strutils.get_all_substrings("abcd") == set(["a", "b", "c", "d", "ab", "bc", "cd", "abc", "bcd", "abcd"])
+        assert strutils.get_all_substrings("abc") == set(
+            ["a", "b", "c", "ab", "bc", "abc"]
+        )
+        assert strutils.get_all_substrings("abcd") == set(
+            ["a", "b", "c", "d", "ab", "bc", "cd", "abc", "bcd", "abcd"]
+        )
 
         assert strutils.get_all_substrings("aa") == set(["a", "aa"])
         assert strutils.get_all_substrings("aab") == set(["a", "b", "aa", "ab", "aab"])
         assert strutils.get_all_substrings("aba") == set(["a", "b", "ab", "ba", "aba"])
-        assert strutils.get_all_substrings("abab") == set(["a", "b", "ab", "ba", "aba", "bab", "abab"])
+        assert strutils.get_all_substrings("abab") == set(
+            ["a", "b", "ab", "ba", "aba", "bab", "abab"]
+        )
 
     def test39(self):
         assert strutils.get_all_substrings(b"a") == set([b"a"])
         assert strutils.get_all_substrings(b"ab") == set([b"a", b"b", b"ab"])
-        assert strutils.get_all_substrings(b"abc") == set([b"a", b"b", b"c", b"ab", b"bc", b"abc"])
-        assert strutils.get_all_substrings(b"abcd") == set([b"a", b"b", b"c", b"d", b"ab", b"bc", b"cd", b"abc", b"bcd", b"abcd"])
+        assert strutils.get_all_substrings(b"abc") == set(
+            [b"a", b"b", b"c", b"ab", b"bc", b"abc"]
+        )
+        assert strutils.get_all_substrings(b"abcd") == set(
+            [b"a", b"b", b"c", b"d", b"ab", b"bc", b"cd", b"abc", b"bcd", b"abcd"]
+        )
 
         assert strutils.get_all_substrings(b"aa") == set([b"a", b"aa"])
-        assert strutils.get_all_substrings(b"aab") == set([b"a", b"b", b"aa", b"ab", b"aab"])
-        assert strutils.get_all_substrings(b"aba") == set([b"a", b"b", b"ab", b"ba", b"aba"])
-        assert strutils.get_all_substrings(b"abab") == set([b"a", b"b", b"ab", b"ba", b"aba", b"bab", b"abab"])
+        assert strutils.get_all_substrings(b"aab") == set(
+            [b"a", b"b", b"aa", b"ab", b"aab"]
+        )
+        assert strutils.get_all_substrings(b"aba") == set(
+            [b"a", b"b", b"ab", b"ba", b"aba"]
+        )
+        assert strutils.get_all_substrings(b"abab") == set(
+            [b"a", b"b", b"ab", b"ba", b"aba", b"bab", b"abab"]
+        )
 
     def test40(self):
         assert strutils.force_type_to("src", "dst") == "src"
         assert strutils.force_type_to("src", b"dst") == b"src"
         assert strutils.force_type_to(b"src", "dst") == "src"
         assert strutils.force_type_to(b"src", b"dst") == b"src"
 
@@ -420,15 +514,15 @@
         assert strutils.random_string(8, choices=choices)
 
         choices = strutils.force_bytes(string.ascii_letters)
         assert strutils.random_string(8, choices=choices)
 
     def test43(self):
         assert strutils.force_float(None) is None
-        assert strutils.force_float(lambda:1.101) == 1.101
+        assert strutils.force_float(lambda: 1.101) == 1.101
         assert strutils.force_float(1.101) == 1.101
         assert strutils.force_float("1.101") == 1.101
         assert strutils.force_float(b"1.101") == 1.101
         assert strutils.force_float(Decimal(1.101)) == 1.101
 
     def test44(self):
         assert strutils.clean("abc", "ab") == "ab"
@@ -488,15 +582,15 @@
     def test53(self):
         data = uuid.uuid4()
         assert strutils.is_uuid(data)
         assert strutils.is_uuid(data.fields)
         assert strutils.is_uuid(data.bytes)
         assert strutils.is_uuid(str(data))
         assert strutils.is_uuid(data.hex)
-    
+
     def test54(self):
         assert strutils.encodable("hello")
         assert strutils.encodable("测试")
         assert strutils.encodable("测试", encoding="big5") is False
 
     def test55(self):
         assert strutils.reverse(None) is None
@@ -519,38 +613,40 @@
     def test58(self):
         filename1 = get_test_assets("p1.jpeg")
         format1 = "jpeg"
         data1 = strutils.get_base64image(filename1, format=format1)
         format2, data2 = strutils.parse_base64image(data1)
         assert format1 == format2
         assert data2 == strutils.get_image_bytes(filename1, format=format1)
- 
+
     def test59(self):
         filename1 = get_test_assets("p1.jpeg")
         format1 = "jpeg"
         content = b""
         with open(filename1, "rb") as fobj:
             content = fobj.read()
         data1 = strutils.get_base64image(content, format=format1)
         format2, data2 = strutils.parse_base64image(data1)
         assert format1 == format2
         assert data2 == strutils.get_image_bytes(filename1, format=format1)
 
     def test60(self):
         from PIL import Image
+
         image = Image.new("RGB", (1, 1))
         format1 = "webp"
         content = strutils.get_image_bytes(image, format1)
         data1 = strutils.get_base64image(content, format=format1)
         format2, data2 = strutils.parse_base64image(data1)
         assert format1 == format2
         assert data2 == strutils.get_image_bytes(image, format=format1)
 
     def test61(self):
         from PIL import Image
+
         image = Image.new("RGB", (1, 1))
         format1 = "webp"
         content1 = strutils.get_image_bytes(image, format1)
         content2 = strutils.get_image_bytes(content1, format1)
         data1 = strutils.get_base64image(content2, format=format1)
         format2, data2 = strutils.parse_base64image(data1)
         assert format1 == format2
```

### Comparing `zenutils-0.5.2/tests/test_sysutils.py` & `zenutils-0.5.4/tests/test_sysutils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,48 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 import time
 import threading
 import unittest
 
 from zenutils import sysutils
 
 
 def fakeproc():
     print("i am in fake process...")
 
+
 class TestSysUtils(unittest.TestCase):
 
     def test01(self):
         w1 = sysutils.get_worker_id()
         w2 = sysutils.get_worker_id()
         assert w1 == w2
-    
+
     def test02(self):
         # thread id may reused after a thread terminated
         info = {}
         set_lock = threading.Lock()
+
         def get_info(info, name):
             with set_lock:
                 info[name] = sysutils.get_worker_id()
             time.sleep(5)
+
         get_info(info, "w0")
         t1 = threading.Thread(target=get_info, args=[info, "w1"])
         t2 = threading.Thread(target=get_info, args=[info, "w2"])
         t1.start()
         t2.start()
         t1.join()
         t2.join()
@@ -40,15 +51,14 @@
         assert info["w2"] != info["w0"]
 
     def test03(self):
         w1 = sysutils.get_worker_id("redis")
         w2 = sysutils.get_worker_id("mysql")
         assert w1 != w2
 
-
     def test04(self):
         code, stdout, stderr = sysutils.execute_script("hostname")
         assert code == 0
         assert stdout != ""
         assert stderr == ""
         assert isinstance(stdout, STR_TYPE)
         assert isinstance(stderr, STR_TYPE)
```

### Comparing `zenutils-0.5.2/tests/test_threadutils.py` & `zenutils-0.5.4/tests/test_threadutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,18 +59,19 @@
         time.sleep(5)
         len12 = len(numbers)
         assert len11 == len12
         service.start()
         time.sleep(5)
         len2 = len(numbers)
         assert len2 > len1
-        service.terminate()
-        assert service.is_running == False
+        assert service.terminate()
+        print(service.__dict__)
+        assert service.is_running is False
         assert service.terminated_time
-        assert service.service_thread.is_alive() == False
+        assert service.service_thread.is_alive() is False
         len3 = len(numbers)
         time.sleep(5)
         len4 = len(numbers)
         assert len4 == len3
         s1 = sum(numbers)
         s2 = (len(numbers) + 1) * len(numbers) / 2
         assert s1 == s2
```

### Comparing `zenutils-0.5.2/tests/test_treeutils.py` & `zenutils-0.5.4/tests/test_treeutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 
 import unittest
 from zenutils import treeutils
 
+
 class TestTreeUtils(unittest.TestCase):
     def test01(self):
         thelist = [
             {"id": 1, "title": "a"},
             {"id": 2, "title": "b"},
             {"id": 3, "title": "a.a", "parent_id": 1},
             {"id": 4, "title": "b.a", "parent_id": 2},
@@ -21,15 +30,15 @@
             {"id": 9, "title": "a.a.b.a", "parent_id": 6},
             {"id": 10, "title": "b.a.a", "parent_id": 4},
             {"id": 11, "title": "d"},
         ]
         tree = treeutils.build_tree(thelist)
         treeutils.print_tree(tree)
         title = tree[0]["children"][0]["children"][1]["children"][0]["title"]
-        assert title  == "a.a.b.a"
+        assert title == "a.a.b.a"
 
     def test02(self):
         ## if the node's parent_id is not in current list, then the node is treated as root node.
         thelist = [
             {"id": 1, "title": "a", "parent_id": 4},
             {"id": 2, "title": "b", "parent_id": 4},
             {"id": 3, "title": "c", "parent_id": 5},
@@ -42,24 +51,26 @@
     def test03(self):
         srt = treeutils.SimpleRouterTree()
         srt.index("/api/v1/uc/", 1)
         srt.index("/api/v1/uc/token/new", 2)
         srt.index("/api/v1/biz/", 3)
         srt.index("/api/v1/biz/jump", 4)
 
-        p1, r1 = srt.get_best_match("/api/v1/uc/ping") # 前缀匹配
-        p2, r2 = srt.get_best_match("/api/v1/uc/token/new") # 精确匹配
-        p3, r3 = srt.get_best_match("/api/v1/biz/go") # 前缀匹配
-        p4, r4 = srt.get_best_match("/api/v1/biz/jump") # 精确匹配
-        p5, r5 = srt.get_best_match("/api/v1/foo") # 前缀匹配，无
-        r6 = srt.get("/api/v1/uc/ping") # 精确匹配，没有
+        p1, r1 = srt.get_best_match("/api/v1/uc/ping")  # 前缀匹配
+        p2, r2 = srt.get_best_match("/api/v1/uc/token/new")  # 精确匹配
+        p3, r3 = srt.get_best_match("/api/v1/biz/go")  # 前缀匹配
+        p4, r4 = srt.get_best_match("/api/v1/biz/jump")  # 精确匹配
+        p5, r5 = srt.get_best_match("/api/v1/foo")  # 前缀匹配，无
+        r6 = srt.get("/api/v1/uc/ping")  # 精确匹配，没有
         ps1 = srt.get_all_paths()
 
-        srt.delete("/api/v1/uc/token/new") # 删除索引
-        p7, r7 = srt.get_best_match("/api/v1/uc/token/new") # 无法精确匹配，降级为前缀匹配
+        srt.delete("/api/v1/uc/token/new")  # 删除索引
+        p7, r7 = srt.get_best_match(
+            "/api/v1/uc/token/new"
+        )  # 无法精确匹配，降级为前缀匹配
         ps2 = srt.get_all_paths()
 
         assert r1 == 1
         assert p1 == "/api/v1/uc/"
         assert r2 == 2
         assert p2 == "/api/v1/uc/token/new"
         assert r3 == 3
```

### Comparing `zenutils-0.5.2/tests/test_typingutils.py` & `zenutils-0.5.4/tests/test_typingutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 
 import unittest
 import os
 import binascii
 import uuid
 from zenutils import typingutils
 from zenutils import base64utils
 
+
 class TestTypingUtils(unittest.TestCase):
 
     def test01(self):
         assert typingutils.smart_cast(int, "12") == 12
         assert typingutils.smart_cast(float, "12.34") == 12.34
         assert typingutils.smart_cast(bool, "true") == True
         assert typingutils.smart_cast(list, "1,2,3") == ["1", "2", "3"]
-        assert typingutils.smart_cast(dict, """{"a": "a", "b": "b"}""") == {"a": "a", "b": "b"}
+        assert typingutils.smart_cast(dict, """{"a": "a", "b": "b"}""") == {
+            "a": "a",
+            "b": "b",
+        }
         assert typingutils.smart_cast(STR_TYPE, b"hello") == "hello"
         assert isinstance("6869", STR_TYPE)
         result = typingutils.smart_cast(BYTES_TYPE, "6869")
         assert isinstance(result, BYTES_TYPE)
         assert result == b"hi"
 
     def test02(self):
@@ -107,8 +119,10 @@
         # test only if typing is available
         try:
             import typing
         except:
             typing = None
         if typing:
             assert typingutils.smart_cast(typing.List, "[1, 2, 3]") == [1, 2, 3]
-            assert typingutils.smart_cast(typing.Mapping, """{"a": "a", "b": "b"}""") == {"a": "a", "b": "b"}
+            assert typingutils.smart_cast(
+                typing.Mapping, """{"a": "a", "b": "b"}"""
+            ) == {"a": "a", "b": "b"}
```

### Comparing `zenutils-0.5.2/zenutils/base64utils.py` & `zenutils-0.5.4/zenutils/base64utils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/zenutils/cacheutils.py` & `zenutils-0.5.4/zenutils/cacheutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/zenutils/cipherutils.py` & `zenutils-0.5.4/zenutils/cipherutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/zenutils/dateutils.py` & `zenutils-0.5.4/zenutils/dateutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/zenutils/dictutils.py` & `zenutils-0.5.4/zenutils/dictutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/zenutils/errorutils.py` & `zenutils-0.5.4/zenutils/errorutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,15 +151,17 @@
             message = message.get("message", message)
         elif isinstance(
             message, Exception
         ):  # 从python内置异常类构造新的BizError，根据系统内置code映射表设置code
             error = message
             code = 0
             message = None
-            if len(error.args) >= 2:  # 如果内置异常遵循(code, message)参数形式构建，则尝试提取其code和message
+            if (
+                len(error.args) >= 2
+            ):  # 如果内置异常遵循(code, message)参数形式构建，则尝试提取其code和message
                 try:
                     code = int(error.args[0])
                     message = error.args[1:]
                     if len(message) == 1:
                         message = message[0]
                     else:
                         message = " ".join([strutils.force_text(x) for x in message])
@@ -414,15 +416,18 @@
 set_error_info(
     "en",
     "BadResponseContent",
     1001010003,
     "Bad response content. Content returned: {content}.",
 )
 set_error_info(
-    "zh-hans", "BadResponseContent", 1001010003, "HTTP接口响应内容格式非法，响应报文内容为{content}。"
+    "zh-hans",
+    "BadResponseContent",
+    1001010003,
+    "HTTP接口响应内容格式非法，响应报文内容为{content}。",
 )
 
 
 class NoMatchingRouteFound(HttpError):
     pass
 
 
@@ -441,15 +446,17 @@
 class NoUpstreamServerAvailabe(HttpError):
     pass
 
 
 set_error_info(
     "en", "NoUpstreamServerAvailabe", 1001010006, "No upstream server availabe."
 )
-set_error_info("zh-hans", "NoUpstreamServerAvailabe", 1001010006, "没有找到有效的后端服务节点！")
+set_error_info(
+    "zh-hans", "NoUpstreamServerAvailabe", 1001010006, "没有找到有效的后端服务节点！"
+)
 
 
 class ConfigError(BizErrorBase):
     pass
 
 
 set_error_info("en", "ConfigError", 1001020000, "Config error.")
@@ -489,26 +496,31 @@
 
 
 class AccountLockedError(AuthError):
     pass
 
 
 set_error_info("en", "AccountLockedError", 1001040001, "Account locked.")
-set_error_info("zh-hans", "AccountLockedError", 1001040001, "帐号被锁定，请联系管理员！")
+set_error_info(
+    "zh-hans", "AccountLockedError", 1001040001, "帐号被锁定，请联系管理员！"
+)
 
 
 class AccountTemporaryLockedError(AuthError):
     pass
 
 
 set_error_info(
     "en", "AccountTemporaryLockedError", 1001040002, "Account temporary locked."
 )
 set_error_info(
-    "zh-hans", "AccountTemporaryLockedError", 1001040002, "登录失败次数超过上限，帐号被临时锁定！"
+    "zh-hans",
+    "AccountTemporaryLockedError",
+    1001040002,
+    "登录失败次数超过上限，帐号被临时锁定！",
 )
 
 
 class UserPasswordError(AuthError):
     pass
 
 
@@ -535,23 +547,27 @@
 
 
 class AccountDisabledError(AuthError):
     pass
 
 
 set_error_info("en", "AccountDisabledError", 1001040006, "Account disabled.")
-set_error_info("zh-hans", "AccountDisabledError", 1001040006, "帐号已禁用，请联系管理员！")
+set_error_info(
+    "zh-hans", "AccountDisabledError", 1001040006, "帐号已禁用，请联系管理员！"
+)
 
 
 class AccountStatusError(AuthError):
     pass
 
 
 set_error_info("en", "AccountStatusError", 1001040007, "Bad account status.")
-set_error_info("zh-hans", "AccountStatusError", 1001040007, "帐号状态异常，请联系管理员处理！")
+set_error_info(
+    "zh-hans", "AccountStatusError", 1001040007, "帐号状态异常，请联系管理员处理！"
+)
 
 
 class AccountRemovedError(AuthError):
     pass
 
 
 set_error_info("en", "AccountRemovedError", 1001040008, "Account removed.")
@@ -599,15 +615,17 @@
 
 
 class AuthenticationRequired(AuthError):
     pass
 
 
 set_error_info("en", "AuthenticationRequired", 1001040014, "Authentication required.")
-set_error_info("zh-hans", "AuthenticationRequired", 1001040014, "请先完成身份认证才能使用本服务！")
+set_error_info(
+    "zh-hans", "AuthenticationRequired", 1001040014, "请先完成身份认证才能使用本服务！"
+)
 
 
 class TypeError(BizErrorBase):
     pass
 
 
 set_error_info("en", "TypeError", 1001050000, "Type error.")
@@ -616,36 +634,43 @@
 
 class ParseJsonError(TypeError):
     pass
 
 
 set_error_info("en", "ParseJsonError", 1001050006, "Parse json error. Raw text {text}.")
 set_error_info(
-    "zh-hans", "ParseJsonError", 1001050006, "字段{field}值为{value}{text}进行Json反序列化异常！"
+    "zh-hans",
+    "ParseJsonError",
+    1001050006,
+    "字段{field}值为{value}{text}进行Json反序列化异常！",
 )
 
 
 class InformalResultPackage(TypeError):
     pass
 
 
 set_error_info(
     "en", "InformalResultPackage", 1001050007, "Informal result package: {message}."
 )
-set_error_info("zh-hans", "InformalResultPackage", 1001050007, "错误的数据封装包：{message}。")
+set_error_info(
+    "zh-hans", "InformalResultPackage", 1001050007, "错误的数据封装包：{message}。"
+)
 
 
 class InformalRequestError(TypeError):
     pass
 
 
 set_error_info(
     "en", "InformalRequestError", 1001050008, "Informal request error: {message}."
 )
-set_error_info("zh-hans", "InformalRequestError", 1001050008, "请求体格式错误：{message}。")
+set_error_info(
+    "zh-hans", "InformalRequestError", 1001050008, "请求体格式错误：{message}。"
+)
 
 
 class TooLargeRequestError(TypeError):
     pass
 
 
 set_error_info(
@@ -692,23 +717,30 @@
 
 
 class StringTooShort(ParamError):
     pass
 
 
 set_error_info("en", "StringTooShort", 1001060004, "String shorter than {min_length}.")
-set_error_info("zh-hans", "StringTooShort", 1001060004, "参数字符数不足，最低要求为：{min_length}。")
+set_error_info(
+    "zh-hans",
+    "StringTooShort",
+    1001060004,
+    "参数字符数不足，最低要求为：{min_length}。",
+)
 
 
 class StringTooLong(ParamError):
     pass
 
 
 set_error_info("en", "StringTooLong", 1001060005, "String longer than {max_length}.")
-set_error_info("zh-hans", "StringTooLong", 1001060005, "参数字符数过多，最高限定为：{max_length}。")
+set_error_info(
+    "zh-hans", "StringTooLong", 1001060005, "参数字符数过多，最高限定为：{max_length}。"
+)
 
 
 class MissingField(ParamError):
     pass
 
 
 set_error_info("en", "MissingField", 1001060006, "Missing field: {field}.")
@@ -734,28 +766,32 @@
 class ValueExceedsMaxLimit(ParamError):
     pass
 
 
 set_error_info(
     "en", "ValueExceedsMaxLimit", 1001060009, "The value exceeds the upper limit."
 )
-set_error_info("zh-hans", "ValueExceedsMaxLimit", 1001060009, "数值{value}超过最大限制{max}！")
+set_error_info(
+    "zh-hans", "ValueExceedsMaxLimit", 1001060009, "数值{value}超过最大限制{max}！"
+)
 
 
 class ValueLessThanMinLimit(ParamError):
     pass
 
 
 set_error_info(
     "en",
     "ValueLessThanMinLimit",
     1001060010,
     "The value is less than the minimum limit.",
 )
-set_error_info("zh-hans", "ValueLessThanMinLimit", 1001060010, "数值{value}小于最小限制{min}！")
+set_error_info(
+    "zh-hans", "ValueLessThanMinLimit", 1001060010, "数值{value}小于最小限制{min}！"
+)
 
 
 class FormError(BizErrorBase):
     pass
 
 
 set_error_info("en", "FormError", 1001070000, "Form error.")
@@ -765,23 +801,30 @@
 class CaptchaOnlyAllowedOnce(FormError):
     pass
 
 
 set_error_info(
     "en", "CaptchaOnlyAllowedOnce", 1001070001, "Captcha only allowed one time use."
 )
-set_error_info("zh-hans", "CaptchaOnlyAllowedOnce", 1001070001, "验证码不允许重复使用！")
+set_error_info(
+    "zh-hans", "CaptchaOnlyAllowedOnce", 1001070001, "验证码不允许重复使用！"
+)
 
 
 class CaptchaValidateFailed(FormError):
     pass
 
 
 set_error_info("en", "CaptchaValidateFailed", 1001070002, "Captcha validate failed.")
-set_error_info("zh-hans", "CaptchaValidateFailed", 1001070002, "图形验证码校验失败，请输入正确的图形验证码！")
+set_error_info(
+    "zh-hans",
+    "CaptchaValidateFailed",
+    1001070002,
+    "图形验证码校验失败，请输入正确的图形验证码！",
+)
 
 
 class RepeatedlySubmitForm(FormError):
     pass
 
 
 set_error_info(
@@ -791,15 +834,17 @@
 
 
 class CaptchaRequired(FormError):
     pass
 
 
 set_error_info("en", "CaptchaRequired", 1001070004, "Captcha Required.")
-set_error_info("zh-hans", "CaptchaRequired", 1001070004, "启用图形验证码校验，请输入正确的验证码。")
+set_error_info(
+    "zh-hans", "CaptchaRequired", 1001070004, "启用图形验证码校验，请输入正确的验证码。"
+)
 
 
 class LogicError(BizErrorBase):
     pass
 
 
 set_error_info("en", "LogicError", 1001080000, "Logic error.")
@@ -821,90 +866,108 @@
 set_error_info(
     "en",
     "CastToIntegerFailed",
     1001090001,
     "Cast to integer value failed on field {field} value={value}.",
 )
 set_error_info(
-    "zh-hans", "CastToIntegerFailed", 1001090001, "字段{field}值为{value}转化整数型数据失败！"
+    "zh-hans",
+    "CastToIntegerFailed",
+    1001090001,
+    "字段{field}值为{value}转化整数型数据失败！",
 )
 
 
 class CastToFloatFailed(CastFailedError):
     pass
 
 
 set_error_info(
     "en",
     "CastToFloatFailed",
     1001090002,
     "Cast to float value failed on field {field} value={value}.",
 )
 set_error_info(
-    "zh-hans", "CastToFloatFailed", 1001090002, "字段{field}值为{value}转化浮点数型数据失败！"
+    "zh-hans",
+    "CastToFloatFailed",
+    1001090002,
+    "字段{field}值为{value}转化浮点数型数据失败！",
 )
 
 
 class CastToNumbericFailed(CastFailedError):
     pass
 
 
 set_error_info(
     "en",
     "CastToNumbericFailed",
     1001090003,
     "Cast to numberic value failed on field {field} value={value}.",
 )
 set_error_info(
-    "zh-hans", "CastToNumbericFailed", 1001090003, "字段{field}值为{value}转化数值型数据失败！"
+    "zh-hans",
+    "CastToNumbericFailed",
+    1001090003,
+    "字段{field}值为{value}转化数值型数据失败！",
 )
 
 
 class CastToBooleanFailed(CastFailedError):
     pass
 
 
 set_error_info(
     "en",
     "CastToBooleanFailed",
     1001090004,
     "Cast to boolean value failed on field {field} value={value}.",
 )
 set_error_info(
-    "zh-hans", "CastToBooleanFailed", 1001090004, "字段{field}值为{value}转化布尔型数据失败！"
+    "zh-hans",
+    "CastToBooleanFailed",
+    1001090004,
+    "字段{field}值为{value}转化布尔型数据失败！",
 )
 
 
 class CastToStringFailed(CastFailedError):
     pass
 
 
 set_error_info(
     "en",
     "CastToStringFailed",
     1001090005,
     "Cast to string value failed on field {field} value={value}.",
 )
 set_error_info(
-    "zh-hans", "CastToStringFailed", 1001090005, "字段{field}值为{value}转化字符串型数据失败！"
+    "zh-hans",
+    "CastToStringFailed",
+    1001090005,
+    "字段{field}值为{value}转化字符串型数据失败！",
 )
 
 
 class NotSupportedTypeToCast(CastFailedError):
     pass
 
 
 set_error_info(
     "en",
     "NotSupportedTypeToCast",
     1001090006,
     "Not supported type to cast on field {field} value={value} type={type}.",
 )
 set_error_info(
-    "zh-hans", "NotSupportedTypeToCast", 1001090006, "字段{field}值为{value}不支持转化为{type}类型！"
+    "zh-hans",
+    "NotSupportedTypeToCast",
+    1001090006,
+    "字段{field}值为{value}不支持转化为{type}类型！",
 )
 
 
 class PermissionError(BizErrorBase):
     pass
 
 
@@ -962,15 +1025,17 @@
 
 set_error_info(
     "en",
     "NoPermissionToCleanCacheError",
     1001100006,
     "No permission to clean cache error.",
 )
-set_error_info("zh-hans", "NoPermissionToCleanCacheError", 1001100006, "没有权限清除缓存！")
+set_error_info(
+    "zh-hans", "NoPermissionToCleanCacheError", 1001100006, "没有权限清除缓存！"
+)
 
 
 class NetworkError(BizErrorBase):
     pass
 
 
 set_error_info("en", "NetworkError", 1001110000, "Network error.")
@@ -988,15 +1053,17 @@
 class SendRequestToServerError(NetworkError):
     pass
 
 
 set_error_info(
     "en", "SendRequestToServerError", 1001110002, "Send request to server error."
 )
-set_error_info("zh-hans", "SendRequestToServerError", 1001110002, "向服务器发送请求失败！")
+set_error_info(
+    "zh-hans", "SendRequestToServerError", 1001110002, "向服务器发送请求失败！"
+)
 
 
 class RecvServerResponseError(NetworkError):
     pass
 
 
 set_error_info(
```

### Comparing `zenutils-0.5.2/zenutils/fsutils.py` & `zenutils-0.5.4/zenutils/fsutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,18 +191,19 @@
     data,
     encoding="utf-8",
     swap_prefix=".",
     swap_suffix=".swap",
     swap_add_random_suffix=True,
 ):
     """Write content to a swap file and then rename it to the target filename."""
+    timestr = datetime.datetime.now().strftime("%Y%m%d%H%M%S%f")
     swap_filename = get_swap_filename(
         filename,
         prefix=swap_prefix,
-        suffix=swap_suffix,
+        suffix=swap_suffix + "." + timestr,
         add_random_suffix=swap_add_random_suffix,
     )
     write(swap_filename, data, encoding)
     rename(swap_filename, filename)
 
 
 def get_temp_workspace(prefix="", makedir=True):
```

### Comparing `zenutils-0.5.2/zenutils/funcutils.py` & `zenutils-0.5.4/zenutils/funcutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -525,15 +525,15 @@
 
     @Example:
         @retry(sleep=5, limit=3)
         def download(url, filename):
             response = requests.get(url)
             with open(filename, "wb") as fobj:
                 fobj.write(response.content)
-        download("http://zencore.cn/example.zip", "example.zip")
+        download("http://example.cn/example.zip", "example.zip")
     """
     if isinstance(raise_exceptions, (list, set)):
         raise_exceptions = tuple(list(raise_exceptions))
     if isinstance(exceptions, (list, set)):
         exceptions = tuple(list(exceptions))
 
     def outter_wrapper(func):
```

### Comparing `zenutils-0.5.2/zenutils/hashutils.py` & `zenutils-0.5.4/zenutils/hashutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/zenutils/httputils.py` & `zenutils-0.5.4/zenutils/httputils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/zenutils/importutils.py` & `zenutils-0.5.4/zenutils/importutils.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     division,
     generators,
     nested_scopes,
     print_function,
     unicode_literals,
     with_statement,
 )
-from zenutils.sixutils import *
 
 __all__ = [
     "get_caller_globals",
     "get_caller_locals",
     "import_module",
     "import_from_string",
 ]
@@ -22,14 +21,16 @@
 import importlib
 
 try:
     import inspect
 except ImportError:
     import inspect2 as inspect
 
+from .dictutils import select
+
 
 def get_caller_globals():
     """
     获取当前函数调用者的globals。
     例如：
         def a():
             x = 2
@@ -85,15 +86,14 @@
         return None
 
 
 def import_from_string(path, slient=True):
     """
     根据给定的对象路径，动态加载对象。
     """
-    from zenutils.dictutils import select
 
     names = path.split(".")
     for i in range(len(names), 0, -1):
         p1 = ".".join(names[0:i])
         module = import_module(p1)
         if module:
             p2 = ".".join(names[i:])
```

### Comparing `zenutils-0.5.2/zenutils/jsonutils.py` & `zenutils-0.5.4/zenutils/jsonutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,14 +174,19 @@
 
 
 def encode_uuid(value):
     """UUID类型编码。"""
     return str(value)
 
 
+def encode_set(value):
+    """set类型编码。"""
+    return list(value)
+
+
 def encode_image(image):
     """PIL Image类型编码。"""
     buffer = BytesIO()
     image.save(buffer, format="png")
     # pylint: disable=consider-using-f-string
     return """data:image/{format};base64,{data}""".format(
         format=format,
@@ -323,15 +328,15 @@
 register_global_encoder(
     (datetime.datetime, datetime.date, datetime.time), encode_datetime
 )
 register_global_encoder(decimal.Decimal, encode_decimal)
 register_global_encoder(complex, encode_complex)
 register_global_encoder(uuid.UUID, encode_uuid)
 register_global_encoder(BASESTRING_TYPES, encode_basestring)
-
+register_global_encoder(set, encode_set)
 
 try:
     from zenutils import dictutils
 
     register_global_encoder(dictutils.HttpHeadersDict, lambda x: x.data)
 except Exception:  # pylint: disable=broad-exception-caught
     pass
```

### Comparing `zenutils-0.5.2/zenutils/listutils.py` & `zenutils-0.5.4/zenutils/listutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/zenutils/logutils.py` & `zenutils-0.5.4/zenutils/logutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/zenutils/nameutils.py` & `zenutils-0.5.4/zenutils/nameutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/zenutils/numericutils.py` & `zenutils-0.5.4/zenutils/numericutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/zenutils/packutils.py` & `zenutils-0.5.4/zenutils/packutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/zenutils/perfutils.py` & `zenutils-0.5.4/zenutils/perfutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/zenutils/randomutils.py` & `zenutils-0.5.4/zenutils/randomutils.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,38 +6,43 @@
     division,
     generators,
     nested_scopes,
     print_function,
     unicode_literals,
     with_statement,
 )
-from zenutils.sixutils import *
 
 __all__ = [
     "choices",
     "get_password_seed32",
     "Random",
     "Lcg31Random",
     "UuidGenerator",
     "uuid1",
     "uuid3",
     "uuid4",
     "uuid5",
 ]
 
+from zlib import crc32
 import random
 import time
 import uuid
 import socket
 import getpass
 import os
 import threading
 import hashlib
 import struct
 import functools
+from .sixutils import STR_TYPE
+from .sixutils import BYTES_TYPE
+from .sixutils import NUMERIC_TYPES
+from .sixutils import force_bytes
+from .numericutils import from_bytes
 
 if not hasattr(time, "perf_counter"):  # fix for py2.7
     time.perf_counter = time.clock
 
 DEFAULT_MODULUS = (2**30 - 123) * 0.91  # always NOT change this
 DEFAULT_MULTIPLIER = (2**29 - 456) * 0.93  # always NOT change this
 DEFAULT_INCREMENT = (2**28 - 789) * 0.95  # always NOT change this
@@ -58,16 +63,14 @@
     if isinstance(passowrd, NUMERIC_TYPES):
         return int(passowrd) % modulus
     if isinstance(passowrd, float):
         return int(passowrd) % modulus
     if isinstance(passowrd, STR_TYPE):
         passowrd = passowrd.encode("utf-8")
     if isinstance(passowrd, BYTES_TYPE):
-        from zlib import crc32
-
         return crc32(passowrd) % modulus
     else:
         msg = "Random seed type must be in (str, bytes, int, long, float), but {} got.".format(
             type(passowrd)
         )
         raise ValueError(msg)
 
@@ -205,23 +208,21 @@
     ):
         self.seed = self.get_seed(seed)
         self.a = a
         self.c = c
         self.m = m
 
     @classmethod
-    def get_seed(cls, seed):
-        from zenutils import numericutils
-
+    def get_seed(cls, seed, **kwargs):
         if seed is None:
             return time.time()
         if isinstance(seed, STR_TYPE):
             seed = seed.encode("utf-8")
         if isinstance(seed, BYTES_TYPE):
-            seed = numericutils.from_bytes(hashlib.sha512(seed).digest(), "big")
+            seed = from_bytes(hashlib.sha512(seed).digest(), "big")
         if isinstance(seed, NUMERIC_TYPES):
             return seed
         else:
             msg = "Random seed type must be in (str, bytes, int, long, float), but {} got.".format(
                 type(seed)
             )
             raise ValueError(msg)
@@ -246,39 +247,42 @@
         a=LCG31_RANDOM_DEFAULT_MULTIPLIER,
         c=LCG31_RANDOM_DEFAULT_INCREMENT,
         m=LCG31_RANDOM_DEFAULT_MODULUS,
     ):
         self.a = a
         self.c = c
         self.m = m
-        self.seed = self.get_seed(seed)
+        super(Lcg31Random, self).__init__(seed=seed)
 
     @classmethod
-    def get_seed(cls, seed):
+    def get_seed(cls, seed, **kwargs):
         return get_password_seed32(seed)
 
     def random(self):
         r = (self.a * self.seed + self.c) % self.m
         p = r / self.m
         self.seed = r
         return p
 
 
 class HashPrng(RandomBase):
+    """基于HASH的伪随机数生成器。"""
+
     BASE_BYTES = 4
     BASE = 256**BASE_BYTES
 
     def __init__(self, seed=None, method=hashlib.sha512):
+        """如果seed为空，则取当前时间为随机数种子。"""
         self.seed = self.get_seed(seed, method)
         self.generator = method(self.seed)
         self.digests = []
         self.round = 1
 
     @classmethod
-    def get_seed(cls, seed, method):
+    def get_seed(cls, seed, method, **kwargs):
         if seed is None:
             seed = time.time()
         seed = force_bytes(seed)
         return method(seed).digest()
 
     def random(self):
         if not self.digests:
@@ -290,14 +294,15 @@
             self.digests = list(struct.unpack(">" + ("I" * digest_count), digest_data))
         digest = self.digests.pop()
         result = 1.0 * digest / self.BASE
         return result
 
 
 def get_random_space_size(generator, length):
+    """统计随机数生成器连续生成不重复随机字节串的长度。可用于检验随机数生成器的随机性。"""
     data = set()
     while True:
         seed = generator.get_bytes(length)
         if seed in data:
             return len(data)
         data.add(seed)
 
@@ -362,14 +367,15 @@
             return uuids
 
 
 uuidgen = UuidGenerator()
 
 
 def uuid1():
+    """使用randomutils取代系统默认的uuid1, uuid3, uuid4, uuid5。"""
     return uuidgen.next()
 
 
 uuid3 = uuid4 = uuid5 = uuid1
 
 
 def choices(thelist, k):
```

### Comparing `zenutils-0.5.2/zenutils/serviceutils.py` & `zenutils-0.5.4/zenutils/serviceutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/zenutils/sixutils.py` & `zenutils-0.5.4/zenutils/sixutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/zenutils/socketserverutils.py` & `zenutils-0.5.4/zenutils/socketserverutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/zenutils/strutils.py` & `zenutils-0.5.4/zenutils/strutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/zenutils/sysutils.py` & `zenutils-0.5.4/zenutils/sysutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/zenutils/threadutils.py` & `zenutils-0.5.4/zenutils/threadutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/zenutils/treeutils.py` & `zenutils-0.5.4/zenutils/treeutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/zenutils/typingutils.py` & `zenutils-0.5.4/zenutils/typingutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/zenutils/xmlrpcutils.py` & `zenutils-0.5.4/zenutils/xmlrpcutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.5.2/zenutils.egg-info/PKG-INFO` & `zenutils-0.5.4/zenutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: zenutils
-Version: 0.5.2
+Version: 0.5.4
 Summary: Collection of simple utils.
 Author: Xin HaoJia
-Author-email: xinhaojia@zencore.cn
 Maintainer: Xin HaoJia
-Maintainer-email: xinhaojia@zencore.cn
 License: MIT
 Keywords: zenutils
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -871,7 +869,16 @@
 
 - Fix logutils default format missing space between thread and module fields.
 
 ### v0.5.2
 
 - Add hashutils.get_hash_digest.
 - Add log_to_console and log_to_file option in logutils.get_simple_config.
+
+### v0.5.3
+
+- Fix jsonutils.simple_json_dumps for set value problem.
+
+### v0.5.4
+
+- fsutils.safe_write add timestr suffix.
+
```

### Comparing `zenutils-0.5.2/zenutils.egg-info/SOURCES.txt` & `zenutils-0.5.4/zenutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

