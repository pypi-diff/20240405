# Comparing `tmp/logger-36-2024.6.tar.gz` & `tmp/logger-36-2024.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logger-36-2024.6.tar", last modified: Wed Apr  3 16:11:17 2024, max compression
+gzip compressed data, was "logger-36-2024.7.tar", last modified: Fri Apr  5 10:11:30 2024, max compression
```

## Comparing `logger-36-2024.6.tar` & `logger-36-2024.7.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.851893 logger-36-2024.6/
--rwx------   0 eric      (1000) users      (984)      114 2022-10-14 06:42:17.000000 logger-36-2024.6/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     4246 2024-04-03 16:11:17.851893 logger-36-2024.6/PKG-INFO
--rwx------   0 eric      (1000) users      (984)      636 2023-02-17 08:45:51.000000 logger-36-2024.6/README-COPYRIGHT-utf8.txt
--rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 logger-36-2024.6/README-LICENCE-utf8.txt
--rwx------   0 eric      (1000) users      (984)     3458 2023-02-17 09:17:51.000000 logger-36-2024.6/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.838559 logger-36-2024.6/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.841893 logger-36-2024.6/documentation/wiki/
--rwx------   0 eric      (1000) users      (984)     1867 2024-03-29 10:17:44.000000 logger-36-2024.6/documentation/wiki/description.asciidoc
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.841893 logger-36-2024.6/logger_36/
--rwx------   0 eric      (1000) users      (984)     1756 2024-03-15 21:24:09.000000 logger-36-2024.6/logger_36/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.838559 logger-36-2024.6/logger_36/catalog/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.841893 logger-36-2024.6/logger_36/catalog/config/
--rw-r--r--   0 eric      (1000) users      (984)     2030 2024-03-28 08:18:21.000000 logger-36-2024.6/logger_36/catalog/config/console_rich.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.845226 logger-36-2024.6/logger_36/catalog/handler/
--rw-r--r--   0 eric      (1000) users      (984)     3092 2024-03-27 17:11:48.000000 logger-36-2024.6/logger_36/catalog/handler/console.py
--rwx------   0 eric      (1000) users      (984)     6512 2024-04-03 16:05:44.000000 logger-36-2024.6/logger_36/catalog/handler/console_rich.py
--rwx------   0 eric      (1000) users      (984)     3507 2024-03-27 17:11:54.000000 logger-36-2024.6/logger_36/catalog/handler/file.py
--rwx------   0 eric      (1000) users      (984)     5931 2024-03-27 17:12:07.000000 logger-36-2024.6/logger_36/catalog/handler/generic.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.845226 logger-36-2024.6/logger_36/catalog/logging/
--rw-r--r--   0 eric      (1000) users      (984)     1814 2024-03-27 17:05:43.000000 logger-36-2024.6/logger_36/catalog/logging/chronos.py
--rw-r--r--   0 eric      (1000) users      (984)     2465 2024-03-27 17:05:43.000000 logger-36-2024.6/logger_36/catalog/logging/gpu.py
--rw-r--r--   0 eric      (1000) users      (984)     4038 2024-03-28 09:46:44.000000 logger-36-2024.6/logger_36/catalog/logging/memory.py
--rw-r--r--   0 eric      (1000) users      (984)     2447 2024-03-27 17:20:41.000000 logger-36-2024.6/logger_36/catalog/logging/system.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.845226 logger-36-2024.6/logger_36/config/
--rw-r--r--   0 eric      (1000) users      (984)     1637 2024-03-29 09:47:00.000000 logger-36-2024.6/logger_36/config/issue.py
--rw-r--r--   0 eric      (1000) users      (984)     1587 2024-03-28 09:30:00.000000 logger-36-2024.6/logger_36/config/memory.py
--rwx------   0 eric      (1000) users      (984)     2056 2024-03-28 08:16:13.000000 logger-36-2024.6/logger_36/config/message.py
--rw-r--r--   0 eric      (1000) users      (984)     1847 2024-03-27 17:18:16.000000 logger-36-2024.6/logger_36/config/system.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.848559 logger-36-2024.6/logger_36/constant/
--rw-r--r--   0 eric      (1000) users      (984)     1614 2024-03-27 18:55:10.000000 logger-36-2024.6/logger_36/constant/generic.py
--rwx------   0 eric      (1000) users      (984)     1681 2024-03-27 18:54:51.000000 logger-36-2024.6/logger_36/constant/handler.py
--rw-r--r--   0 eric      (1000) users      (984)     1656 2024-03-28 09:36:45.000000 logger-36-2024.6/logger_36/constant/issue.py
--rw-r--r--   0 eric      (1000) users      (984)     2150 2024-03-28 09:06:53.000000 logger-36-2024.6/logger_36/constant/logger.py
--rw-r--r--   0 eric      (1000) users      (984)     1795 2024-03-28 09:36:54.000000 logger-36-2024.6/logger_36/constant/memory.py
--rw-r--r--   0 eric      (1000) users      (984)     2084 2024-03-27 18:54:51.000000 logger-36-2024.6/logger_36/constant/message.py
--rw-r--r--   0 eric      (1000) users      (984)     1681 2024-03-27 17:02:29.000000 logger-36-2024.6/logger_36/constant/record.py
--rw-r--r--   0 eric      (1000) users      (984)     1800 2024-03-27 18:54:51.000000 logger-36-2024.6/logger_36/constant/system.py
--rw-r--r--   0 eric      (1000) users      (984)     1616 2024-03-06 14:38:47.000000 logger-36-2024.6/logger_36/instance.py
--rwx------   0 eric      (1000) users      (984)     6690 2024-04-03 15:42:32.000000 logger-36-2024.6/logger_36/main.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.848559 logger-36-2024.6/logger_36/task/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.848559 logger-36-2024.6/logger_36/task/format/
--rw-r--r--   0 eric      (1000) users      (984)     3610 2024-03-28 09:36:54.000000 logger-36-2024.6/logger_36/task/format/memory.py
--rw-r--r--   0 eric      (1000) users      (984)     3511 2024-03-27 18:54:51.000000 logger-36-2024.6/logger_36/task/format/message.py
--rw-r--r--   0 eric      (1000) users      (984)     1968 2024-03-12 15:08:33.000000 logger-36-2024.6/logger_36/task/format/rule.py
--rwx------   0 eric      (1000) users      (984)     4397 2024-03-07 16:54:56.000000 logger-36-2024.6/logger_36/task/inspection.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.848559 logger-36-2024.6/logger_36/task/measure/
--rwx------   0 eric      (1000) users      (984)     2253 2024-03-27 17:27:28.000000 logger-36-2024.6/logger_36/task/measure/chronos.py
--rwx------   0 eric      (1000) users      (984)     1874 2024-03-27 18:39:46.000000 logger-36-2024.6/logger_36/task/measure/memory.py
--rw-r--r--   0 eric      (1000) users      (984)     5026 2024-03-29 09:49:15.000000 logger-36-2024.6/logger_36/task/storage.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.851893 logger-36-2024.6/logger_36/type/
--rwx------   0 eric      (1000) users      (984)     5198 2024-03-27 18:54:51.000000 logger-36-2024.6/logger_36/type/extension.py
--rw-r--r--   0 eric      (1000) users      (984)     2151 2024-03-29 09:46:52.000000 logger-36-2024.6/logger_36/type/issue.py
--rw-r--r--   0 eric      (1000) users      (984)    12729 2024-04-03 06:51:24.000000 logger-36-2024.6/logger_36/type/logger.py
--rwx------   0 eric      (1000) users      (984)     1575 2024-04-03 16:10:56.000000 logger-36-2024.6/logger_36/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-03 16:11:17.851893 logger-36-2024.6/logger_36.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     4246 2024-04-03 16:11:17.000000 logger-36-2024.6/logger_36.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)     1320 2024-04-03 16:11:17.000000 logger-36-2024.6/logger_36.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2024-04-03 16:11:17.000000 logger-36-2024.6/logger_36.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)       10 2024-04-03 16:11:17.000000 logger-36-2024.6/logger_36.egg-info/top_level.txt
--rwx------   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 logger-36-2024.6/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2024-04-03 16:11:17.851893 logger-36-2024.6/setup.cfg
--rwx------   0 eric      (1000) users      (984)     5533 2024-04-03 07:02:21.000000 logger-36-2024.6/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.736580 logger-36-2024.7/
+-rwx------   0 eric      (1000) users      (984)      114 2022-10-14 06:42:17.000000 logger-36-2024.7/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     4246 2024-04-05 10:11:30.736580 logger-36-2024.7/PKG-INFO
+-rwx------   0 eric      (1000) users      (984)      636 2023-02-17 08:45:51.000000 logger-36-2024.7/README-COPYRIGHT-utf8.txt
+-rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 logger-36-2024.7/README-LICENCE-utf8.txt
+-rwx------   0 eric      (1000) users      (984)     3458 2023-02-17 09:17:51.000000 logger-36-2024.7/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.729913 logger-36-2024.7/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.729913 logger-36-2024.7/documentation/wiki/
+-rwx------   0 eric      (1000) users      (984)     1867 2024-03-29 10:17:44.000000 logger-36-2024.7/documentation/wiki/description.asciidoc
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.733246 logger-36-2024.7/logger_36/
+-rwx------   0 eric      (1000) users      (984)     1756 2024-03-15 21:24:09.000000 logger-36-2024.7/logger_36/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.729913 logger-36-2024.7/logger_36/catalog/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.733246 logger-36-2024.7/logger_36/catalog/config/
+-rw-r--r--   0 eric      (1000) users      (984)     2030 2024-03-28 08:18:21.000000 logger-36-2024.7/logger_36/catalog/config/console_rich.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.733246 logger-36-2024.7/logger_36/catalog/handler/
+-rw-r--r--   0 eric      (1000) users      (984)     3092 2024-03-27 17:11:48.000000 logger-36-2024.7/logger_36/catalog/handler/console.py
+-rwx------   0 eric      (1000) users      (984)     6512 2024-04-03 16:05:44.000000 logger-36-2024.7/logger_36/catalog/handler/console_rich.py
+-rwx------   0 eric      (1000) users      (984)     3507 2024-03-27 17:11:54.000000 logger-36-2024.7/logger_36/catalog/handler/file.py
+-rwx------   0 eric      (1000) users      (984)     6048 2024-04-05 10:08:58.000000 logger-36-2024.7/logger_36/catalog/handler/generic.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.733246 logger-36-2024.7/logger_36/catalog/logging/
+-rw-r--r--   0 eric      (1000) users      (984)     1814 2024-03-27 17:05:43.000000 logger-36-2024.7/logger_36/catalog/logging/chronos.py
+-rw-r--r--   0 eric      (1000) users      (984)     2465 2024-03-27 17:05:43.000000 logger-36-2024.7/logger_36/catalog/logging/gpu.py
+-rw-r--r--   0 eric      (1000) users      (984)     4038 2024-03-28 09:46:44.000000 logger-36-2024.7/logger_36/catalog/logging/memory.py
+-rw-r--r--   0 eric      (1000) users      (984)     2447 2024-03-27 17:20:41.000000 logger-36-2024.7/logger_36/catalog/logging/system.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.733246 logger-36-2024.7/logger_36/config/
+-rw-r--r--   0 eric      (1000) users      (984)     1637 2024-03-29 09:47:00.000000 logger-36-2024.7/logger_36/config/issue.py
+-rw-r--r--   0 eric      (1000) users      (984)     1587 2024-03-28 09:30:00.000000 logger-36-2024.7/logger_36/config/memory.py
+-rwx------   0 eric      (1000) users      (984)     2056 2024-03-28 08:16:13.000000 logger-36-2024.7/logger_36/config/message.py
+-rw-r--r--   0 eric      (1000) users      (984)     1847 2024-03-27 17:18:16.000000 logger-36-2024.7/logger_36/config/system.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.736580 logger-36-2024.7/logger_36/constant/
+-rw-r--r--   0 eric      (1000) users      (984)     1614 2024-03-27 18:55:10.000000 logger-36-2024.7/logger_36/constant/generic.py
+-rwx------   0 eric      (1000) users      (984)     1681 2024-03-27 18:54:51.000000 logger-36-2024.7/logger_36/constant/handler.py
+-rw-r--r--   0 eric      (1000) users      (984)     1656 2024-03-28 09:36:45.000000 logger-36-2024.7/logger_36/constant/issue.py
+-rw-r--r--   0 eric      (1000) users      (984)     2150 2024-03-28 09:06:53.000000 logger-36-2024.7/logger_36/constant/logger.py
+-rw-r--r--   0 eric      (1000) users      (984)     1795 2024-03-28 09:36:54.000000 logger-36-2024.7/logger_36/constant/memory.py
+-rw-r--r--   0 eric      (1000) users      (984)     2084 2024-03-27 18:54:51.000000 logger-36-2024.7/logger_36/constant/message.py
+-rw-r--r--   0 eric      (1000) users      (984)     1681 2024-03-27 17:02:29.000000 logger-36-2024.7/logger_36/constant/record.py
+-rw-r--r--   0 eric      (1000) users      (984)     1800 2024-03-27 18:54:51.000000 logger-36-2024.7/logger_36/constant/system.py
+-rw-r--r--   0 eric      (1000) users      (984)     1616 2024-03-06 14:38:47.000000 logger-36-2024.7/logger_36/instance.py
+-rwx------   0 eric      (1000) users      (984)     6690 2024-04-03 15:42:32.000000 logger-36-2024.7/logger_36/main.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.736580 logger-36-2024.7/logger_36/task/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.736580 logger-36-2024.7/logger_36/task/format/
+-rw-r--r--   0 eric      (1000) users      (984)     3610 2024-03-28 09:36:54.000000 logger-36-2024.7/logger_36/task/format/memory.py
+-rw-r--r--   0 eric      (1000) users      (984)     3511 2024-03-27 18:54:51.000000 logger-36-2024.7/logger_36/task/format/message.py
+-rw-r--r--   0 eric      (1000) users      (984)     1968 2024-03-12 15:08:33.000000 logger-36-2024.7/logger_36/task/format/rule.py
+-rwx------   0 eric      (1000) users      (984)     4397 2024-03-07 16:54:56.000000 logger-36-2024.7/logger_36/task/inspection.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.736580 logger-36-2024.7/logger_36/task/measure/
+-rwx------   0 eric      (1000) users      (984)     2253 2024-03-27 17:27:28.000000 logger-36-2024.7/logger_36/task/measure/chronos.py
+-rwx------   0 eric      (1000) users      (984)     1874 2024-03-27 18:39:46.000000 logger-36-2024.7/logger_36/task/measure/memory.py
+-rw-r--r--   0 eric      (1000) users      (984)     5026 2024-03-29 09:49:15.000000 logger-36-2024.7/logger_36/task/storage.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.736580 logger-36-2024.7/logger_36/type/
+-rwx------   0 eric      (1000) users      (984)     5198 2024-03-27 18:54:51.000000 logger-36-2024.7/logger_36/type/extension.py
+-rw-r--r--   0 eric      (1000) users      (984)     2151 2024-03-29 09:46:52.000000 logger-36-2024.7/logger_36/type/issue.py
+-rw-r--r--   0 eric      (1000) users      (984)    12766 2024-04-05 09:08:38.000000 logger-36-2024.7/logger_36/type/logger.py
+-rwx------   0 eric      (1000) users      (984)     1575 2024-04-05 10:10:59.000000 logger-36-2024.7/logger_36/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-05 10:11:30.736580 logger-36-2024.7/logger_36.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     4246 2024-04-05 10:11:30.000000 logger-36-2024.7/logger_36.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)     1320 2024-04-05 10:11:30.000000 logger-36-2024.7/logger_36.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2024-04-05 10:11:30.000000 logger-36-2024.7/logger_36.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)       10 2024-04-05 10:11:30.000000 logger-36-2024.7/logger_36.egg-info/top_level.txt
+-rwx------   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 logger-36-2024.7/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2024-04-05 10:11:30.736580 logger-36-2024.7/setup.cfg
+-rwx------   0 eric      (1000) users      (984)     5533 2024-04-03 07:02:21.000000 logger-36-2024.7/setup.py
```

### Comparing `logger-36-2024.6/PKG-INFO` & `logger-36-2024.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-36
-Version: 2024.6
+Version: 2024.7
 Summary: Simple logger with a catalog of handlers
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/logger-36/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/logger-36//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/logger-36/
```

### Comparing `logger-36-2024.6/README-COPYRIGHT-utf8.txt` & `logger-36-2024.7/README-COPYRIGHT-utf8.txt`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/README-LICENCE-utf8.txt` & `logger-36-2024.7/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/README.rst` & `logger-36-2024.7/README.rst`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/documentation/wiki/description.asciidoc` & `logger-36-2024.7/documentation/wiki/description.asciidoc`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/__init__.py` & `logger-36-2024.7/logger_36/__init__.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/catalog/config/console_rich.py` & `logger-36-2024.7/logger_36/catalog/config/console_rich.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/catalog/handler/console.py` & `logger-36-2024.7/logger_36/catalog/handler/console.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/catalog/handler/console_rich.py` & `logger-36-2024.7/logger_36/catalog/handler/console_rich.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/catalog/handler/file.py` & `logger-36-2024.7/logger_36/catalog/handler/file.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/catalog/handler/generic.py` & `logger-36-2024.7/logger_36/catalog/handler/generic.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,24 +29,26 @@
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
 import logging as lggg
 import typing as h
 
+from logger_36.catalog.config.console_rich import DATE_TIME_COLOR
+
 try:
     from rich.console import Console as console_t
     from rich.markup import escape as EscapedForRich
     from rich.terminal_theme import DEFAULT_TERMINAL_THEME
 except ModuleNotFoundError:
     console_t = EscapedForRich = DEFAULT_TERMINAL_THEME = None
 
 from logger_36.catalog.handler.console_rich import console_rich_handler_t
 from logger_36.constant.record import SHOW_W_RULE_ATTR
-from logger_36.task.format.rule import Rule
+from logger_36.task.format.rule import Rule, RuleAsText
 from logger_36.type.extension import handler_extension_t
 
 
 class can_show_message_p(h.Protocol):
     def ShowMessage(self, message: str, /) -> None: ...
 
 
@@ -65,15 +67,15 @@
     level: dtcl.InitVar[int] = lggg.NOTSET
     show_where: dtcl.InitVar[bool] = True
     show_memory_usage: dtcl.InitVar[bool] = False
     formatter: dtcl.InitVar[lggg.Formatter | None] = None
 
     supports_html: dtcl.InitVar[bool] = False
     rich_kwargs: dtcl.InitVar[dict[str, h.Any] | None] = None
-    interface: dtcl.InitVar[interface_h | None] = None
+    interface: dtcl.InitVar[interface_h | None] = None  # Cannot be None actually.
 
     def __post_init__(
         self,
         name: str | None,
         level: int,
         show_where: bool,
         show_memory_usage: bool,
@@ -101,27 +103,28 @@
                 highlight=False,
                 force_terminal=True,
                 **rich_kwargs,
             )
 
         self.FormattedLines = self.extension.FormattedLines
 
-        if interface is None:
-            raise ValueError("Interface cannot be None.")
         self.ShowMessage = getattr(
             interface, can_show_message_p.ShowMessage.__name__, interface
         )
 
     def emit(self, record: lggg.LogRecord, /) -> None:
         """"""
         if self.console is None:
-            message, _ = self.FormattedLines(record, should_join_lines=True)
+            if hasattr(record, SHOW_W_RULE_ATTR):
+                message = RuleAsText(record.msg)
+            else:
+                message, _ = self.FormattedLines(record, should_join_lines=True)
         else:
             if hasattr(record, SHOW_W_RULE_ATTR):
-                richer = Rule(record.msg, console_rich_handler_t.DATE_TIME_COLOR)
+                richer = Rule(record.msg, DATE_TIME_COLOR)
             else:
                 first, next_s = self.FormattedLines(record, PreProcessed=EscapedForRich)
                 richer = console_rich_handler_t.HighlightedVersion(
                     first, next_s, record.levelno
                 )
             segments = self.console.render(richer)
```

### Comparing `logger-36-2024.6/logger_36/catalog/logging/chronos.py` & `logger-36-2024.7/logger_36/catalog/logging/chronos.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/catalog/logging/gpu.py` & `logger-36-2024.7/logger_36/catalog/logging/gpu.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/catalog/logging/memory.py` & `logger-36-2024.7/logger_36/catalog/logging/memory.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/catalog/logging/system.py` & `logger-36-2024.7/logger_36/catalog/logging/system.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/config/issue.py` & `logger-36-2024.7/logger_36/config/issue.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/config/memory.py` & `logger-36-2024.7/logger_36/config/memory.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/config/message.py` & `logger-36-2024.7/logger_36/config/message.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/config/system.py` & `logger-36-2024.7/logger_36/config/system.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/constant/generic.py` & `logger-36-2024.7/logger_36/constant/generic.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/constant/handler.py` & `logger-36-2024.7/logger_36/constant/handler.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/constant/issue.py` & `logger-36-2024.7/logger_36/constant/issue.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/constant/logger.py` & `logger-36-2024.7/logger_36/constant/logger.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/constant/memory.py` & `logger-36-2024.7/logger_36/constant/memory.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/constant/message.py` & `logger-36-2024.7/logger_36/constant/message.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/constant/record.py` & `logger-36-2024.7/logger_36/constant/record.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/constant/system.py` & `logger-36-2024.7/logger_36/constant/system.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/instance.py` & `logger-36-2024.7/logger_36/instance.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/main.py` & `logger-36-2024.7/logger_36/main.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/task/format/memory.py` & `logger-36-2024.7/logger_36/task/format/memory.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/task/format/message.py` & `logger-36-2024.7/logger_36/task/format/message.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/task/format/rule.py` & `logger-36-2024.7/logger_36/task/format/rule.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/task/inspection.py` & `logger-36-2024.7/logger_36/task/inspection.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/task/measure/chronos.py` & `logger-36-2024.7/logger_36/task/measure/chronos.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/task/measure/memory.py` & `logger-36-2024.7/logger_36/task/measure/memory.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/task/storage.py` & `logger-36-2024.7/logger_36/task/storage.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/type/extension.py` & `logger-36-2024.7/logger_36/type/extension.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/type/issue.py` & `logger-36-2024.7/logger_36/type/issue.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/logger_36/type/logger.py` & `logger-36-2024.7/logger_36/type/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,17 +212,18 @@
 
             value, unit = FormattedMemoryUsage(usage, 1)
             record.memory_usage = f"{value}{unit}"
 
         date = dttm.now().strftime(DATE_FORMAT)
         if date != self.last_message_date:
             self.last_message_date = date
-            # levelno is added for management by lggg.Logger.handle.
+            # levelno: Added for management by lggg.Logger.handle.
             date_record = lggg.makeLogRecord(
                 {
+                    "name": self.name,
                     "levelno": lggg.INFO,
                     "msg": f"DATE: {date}",
                     SHOW_W_RULE_ATTR: True,
                 }
             )
             if self.should_hold_messages:
                 self.on_hold.append(date_record)
```

### Comparing `logger-36-2024.6/logger_36/version.py` & `logger-36-2024.7/logger_36/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2024.6"
+__version__ = "2024.7"
```

### Comparing `logger-36-2024.6/logger_36.egg-info/PKG-INFO` & `logger-36-2024.7/logger_36.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-36
-Version: 2024.6
+Version: 2024.7
 Summary: Simple logger with a catalog of handlers
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/logger-36/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/logger-36//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/logger-36/
```

### Comparing `logger-36-2024.6/logger_36.egg-info/SOURCES.txt` & `logger-36-2024.7/logger_36.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logger-36-2024.6/setup.py` & `logger-36-2024.7/setup.py`

 * *Files identical despite different names*

