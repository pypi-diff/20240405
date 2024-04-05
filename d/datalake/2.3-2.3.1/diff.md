# Comparing `tmp/datalake-2.3.tar.gz` & `tmp/datalake-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalake-2.3.tar", last modified: Mon Mar  4 23:29:05 2024, max compression
+gzip compressed data, was "datalake-2.3.1.tar", last modified: Fri Apr  5 19:20:58 2024, max compression
```

## Comparing `datalake-2.3.tar` & `datalake-2.3.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 23:29:05.468809 datalake-2.3/
--rw-rw-rw-   0 root         (0) root         (0)    11313 2024-02-29 17:11:31.000000 datalake-2.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       51 2024-02-29 17:11:31.000000 datalake-2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1230 2024-03-04 23:29:05.468809 datalake-2.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11986 2024-02-29 17:11:31.000000 datalake-2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 23:29:05.468809 datalake-2.3/datalake/
--rw-rw-rw-   0 root         (0) root         (0)     1424 2024-02-29 17:11:31.000000 datalake-2.3/datalake/__init__.py
--rw-r--r--   0 root         (0) root         (0)      495 2024-03-04 23:29:05.468809 datalake-2.3/datalake/_version.py
--rw-rw-rw-   0 root         (0) root         (0)    16311 2024-02-29 17:11:31.000000 datalake-2.3/datalake/archive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 23:29:05.468809 datalake-2.3/datalake/common/
--rw-rw-rw-   0 root         (0) root         (0)      852 2024-02-29 17:11:31.000000 datalake-2.3/datalake/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2968 2024-02-29 17:11:31.000000 datalake-2.3/datalake/common/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      783 2024-02-29 17:11:31.000000 datalake-2.3/datalake/common/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     7098 2024-02-29 17:11:31.000000 datalake-2.3/datalake/common/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     7231 2024-02-29 17:11:31.000000 datalake-2.3/datalake/common/record.py
--rw-rw-rw-   0 root         (0) root         (0)     1166 2024-02-29 17:11:31.000000 datalake-2.3/datalake/config_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     1936 2024-02-29 17:11:31.000000 datalake-2.3/datalake/crtime.py
--rw-rw-rw-   0 root         (0) root         (0)    11143 2024-02-29 17:11:31.000000 datalake-2.3/datalake/dlfile.py
--rw-rw-rw-   0 root         (0) root         (0)     1794 2024-02-29 17:11:31.000000 datalake-2.3/datalake/logging_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     8664 2024-02-29 17:11:31.000000 datalake-2.3/datalake/queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 23:29:05.468809 datalake-2.3/datalake/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-04 23:29:04.000000 datalake-2.3/datalake/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9424 2024-02-29 17:11:31.000000 datalake-2.3/datalake/scripts/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 23:29:05.468809 datalake-2.3/datalake/tests/
--rw-rw-rw-   0 root         (0) root         (0)      615 2024-02-29 17:11:31.000000 datalake-2.3/datalake/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4130 2024-02-29 17:11:31.000000 datalake-2.3/datalake/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     2116 2024-02-29 17:11:31.000000 datalake-2.3/datalake/tests/test_conf.py
--rw-rw-rw-   0 root         (0) root         (0)     5942 2024-02-29 17:11:31.000000 datalake-2.3/datalake/tests/test_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     4494 2024-02-29 17:11:31.000000 datalake-2.3/datalake/tests/test_record.py
--rw-rw-rw-   0 root         (0) root         (0)     3329 2024-02-29 17:11:31.000000 datalake-2.3/datalake/translator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 23:29:05.468809 datalake-2.3/datalake.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1230 2024-03-04 23:29:05.000000 datalake-2.3/datalake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      998 2024-03-04 23:29:05.000000 datalake-2.3/datalake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-04 23:29:05.000000 datalake-2.3/datalake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2024-03-04 23:29:05.000000 datalake-2.3/datalake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      344 2024-03-04 23:29:05.000000 datalake-2.3/datalake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-03-04 23:29:05.000000 datalake-2.3/datalake.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      176 2024-03-04 23:29:05.468809 datalake-2.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1837 2024-02-29 17:11:31.000000 datalake-2.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 23:29:05.468809 datalake-2.3/test/
--rw-rw-rw-   0 root         (0) root         (0)     2244 2024-02-29 17:11:31.000000 datalake-2.3/test/test_archive.py
--rw-rw-rw-   0 root         (0) root         (0)     3479 2024-02-29 17:11:31.000000 datalake-2.3/test/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)      922 2024-02-29 17:11:31.000000 datalake-2.3/test/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)     1220 2024-02-29 17:11:31.000000 datalake-2.3/test/test_crtime.py
--rw-rw-rw-   0 root         (0) root         (0)     9426 2024-02-29 17:11:31.000000 datalake-2.3/test/test_fetch.py
--rw-rw-rw-   0 root         (0) root         (0)     5578 2024-02-29 17:11:31.000000 datalake-2.3/test/test_file.py
--rw-rw-rw-   0 root         (0) root         (0)     2080 2024-02-29 17:11:31.000000 datalake-2.3/test/test_latest.py
--rw-rw-rw-   0 root         (0) root         (0)    11863 2024-02-29 17:11:31.000000 datalake-2.3/test/test_list.py
--rw-rw-rw-   0 root         (0) root         (0)      703 2024-02-29 17:11:31.000000 datalake-2.3/test/test_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     8381 2024-02-29 17:11:31.000000 datalake-2.3/test/test_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     2664 2024-02-29 17:11:31.000000 datalake-2.3/test/test_translator.py
--rw-rw-rw-   0 root         (0) root         (0)    68611 2024-02-29 17:11:31.000000 datalake-2.3/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 19:20:57.988261 datalake-2.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11313 2024-04-02 17:12:14.000000 datalake-2.3.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       51 2024-04-02 17:12:14.000000 datalake-2.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1232 2024-04-05 19:20:57.988261 datalake-2.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11986 2024-04-02 17:12:14.000000 datalake-2.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 19:20:57.992261 datalake-2.3.1/datalake/
+-rw-rw-rw-   0 root         (0) root         (0)     1424 2024-04-02 17:12:14.000000 datalake-2.3.1/datalake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2024-04-05 19:20:57.992261 datalake-2.3.1/datalake/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    16311 2024-04-02 17:12:14.000000 datalake-2.3.1/datalake/archive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 19:20:57.988261 datalake-2.3.1/datalake/common/
+-rw-rw-rw-   0 root         (0) root         (0)      852 2024-04-02 17:12:14.000000 datalake-2.3.1/datalake/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2968 2024-04-02 17:12:14.000000 datalake-2.3.1/datalake/common/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      783 2024-04-02 17:12:14.000000 datalake-2.3.1/datalake/common/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     7098 2024-04-02 17:12:14.000000 datalake-2.3.1/datalake/common/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     7231 2024-04-02 17:12:14.000000 datalake-2.3.1/datalake/common/record.py
+-rw-rw-rw-   0 root         (0) root         (0)     1166 2024-04-02 17:12:14.000000 datalake-2.3.1/datalake/config_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1936 2024-04-02 17:12:14.000000 datalake-2.3.1/datalake/crtime.py
+-rw-rw-rw-   0 root         (0) root         (0)    11143 2024-04-02 17:12:14.000000 datalake-2.3.1/datalake/dlfile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1794 2024-04-02 17:12:14.000000 datalake-2.3.1/datalake/logging_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     8664 2024-04-02 17:12:14.000000 datalake-2.3.1/datalake/queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 19:20:57.988261 datalake-2.3.1/datalake/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 19:20:56.000000 datalake-2.3.1/datalake/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9424 2024-04-02 17:12:14.000000 datalake-2.3.1/datalake/scripts/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 19:20:57.988261 datalake-2.3.1/datalake/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      615 2024-04-02 17:12:14.000000 datalake-2.3.1/datalake/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4130 2024-04-02 17:12:14.000000 datalake-2.3.1/datalake/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2116 2024-04-02 17:12:14.000000 datalake-2.3.1/datalake/tests/test_conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     5942 2024-04-02 17:12:14.000000 datalake-2.3.1/datalake/tests/test_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     4494 2024-04-02 17:12:14.000000 datalake-2.3.1/datalake/tests/test_record.py
+-rw-rw-rw-   0 root         (0) root         (0)     3329 2024-04-02 17:12:14.000000 datalake-2.3.1/datalake/translator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 19:20:57.988261 datalake-2.3.1/datalake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1232 2024-04-05 19:20:57.000000 datalake-2.3.1/datalake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      998 2024-04-05 19:20:57.000000 datalake-2.3.1/datalake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 19:20:57.000000 datalake-2.3.1/datalake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2024-04-05 19:20:57.000000 datalake-2.3.1/datalake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      344 2024-04-05 19:20:57.000000 datalake-2.3.1/datalake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-05 19:20:57.000000 datalake-2.3.1/datalake.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      176 2024-04-05 19:20:57.992261 datalake-2.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1837 2024-04-02 17:12:14.000000 datalake-2.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 19:20:57.988261 datalake-2.3.1/test/
+-rw-rw-rw-   0 root         (0) root         (0)     2244 2024-04-02 17:12:14.000000 datalake-2.3.1/test/test_archive.py
+-rw-rw-rw-   0 root         (0) root         (0)     3479 2024-04-02 17:12:14.000000 datalake-2.3.1/test/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-02 17:12:14.000000 datalake-2.3.1/test/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1220 2024-04-02 17:12:14.000000 datalake-2.3.1/test/test_crtime.py
+-rw-rw-rw-   0 root         (0) root         (0)     9426 2024-04-02 17:12:14.000000 datalake-2.3.1/test/test_fetch.py
+-rw-rw-rw-   0 root         (0) root         (0)     5578 2024-04-02 17:12:14.000000 datalake-2.3.1/test/test_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     2080 2024-04-02 17:12:14.000000 datalake-2.3.1/test/test_latest.py
+-rw-rw-rw-   0 root         (0) root         (0)    11863 2024-04-02 17:12:14.000000 datalake-2.3.1/test/test_list.py
+-rw-rw-rw-   0 root         (0) root         (0)      703 2024-04-02 17:12:14.000000 datalake-2.3.1/test/test_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     8381 2024-04-02 17:12:14.000000 datalake-2.3.1/test/test_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     2664 2024-04-02 17:12:14.000000 datalake-2.3.1/test/test_translator.py
+-rw-rw-rw-   0 root         (0) root         (0)    68611 2024-04-02 17:12:14.000000 datalake-2.3.1/versioneer.py
```

### Comparing `datalake-2.3/LICENSE` & `datalake-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datalake-2.3/PKG-INFO` & `datalake-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalake
-Version: 2.3
+Version: 2.3.1
 Summary: datalake: a metadata-aware archive
 Home-page: https://github.com/planetlabs/datalake
 Author: Brian Cavagnolo
 Author-email: brian@planet.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `datalake-2.3/README.md` & `datalake-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `datalake-2.3/datalake/__init__.py` & `datalake-2.3.1/datalake/__init__.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/datalake/archive.py` & `datalake-2.3.1/datalake/archive.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/datalake/common/__init__.py` & `datalake-2.3.1/datalake/common/__init__.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/datalake/common/conf.py` & `datalake-2.3.1/datalake/common/conf.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/datalake/common/errors.py` & `datalake-2.3.1/datalake/common/errors.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/datalake/common/metadata.py` & `datalake-2.3.1/datalake/common/metadata.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/datalake/common/record.py` & `datalake-2.3.1/datalake/common/record.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/datalake/config_helpers.py` & `datalake-2.3.1/datalake/config_helpers.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/datalake/crtime.py` & `datalake-2.3.1/datalake/crtime.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/datalake/dlfile.py` & `datalake-2.3.1/datalake/dlfile.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/datalake/logging_helpers.py` & `datalake-2.3.1/datalake/logging_helpers.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/datalake/queue.py` & `datalake-2.3.1/datalake/queue.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/datalake/scripts/cli.py` & `datalake-2.3.1/datalake/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/datalake/tests/__init__.py` & `datalake-2.3.1/datalake/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/datalake/tests/conftest.py` & `datalake-2.3.1/datalake/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/datalake/tests/test_conf.py` & `datalake-2.3.1/datalake/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/datalake/tests/test_metadata.py` & `datalake-2.3.1/datalake/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/datalake/tests/test_record.py` & `datalake-2.3.1/datalake/tests/test_record.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/datalake/translator.py` & `datalake-2.3.1/datalake/translator.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/datalake.egg-info/PKG-INFO` & `datalake-2.3.1/datalake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalake
-Version: 2.3
+Version: 2.3.1
 Summary: datalake: a metadata-aware archive
 Home-page: https://github.com/planetlabs/datalake
 Author: Brian Cavagnolo
 Author-email: brian@planet.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `datalake-2.3/datalake.egg-info/SOURCES.txt` & `datalake-2.3.1/datalake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datalake-2.3/setup.py` & `datalake-2.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/test/test_archive.py` & `datalake-2.3.1/test/test_archive.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/test/test_cli.py` & `datalake-2.3.1/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/test/test_config.py` & `datalake-2.3.1/test/test_config.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/test/test_crtime.py` & `datalake-2.3.1/test/test_crtime.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/test/test_fetch.py` & `datalake-2.3.1/test/test_fetch.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/test/test_file.py` & `datalake-2.3.1/test/test_file.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/test/test_latest.py` & `datalake-2.3.1/test/test_latest.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/test/test_list.py` & `datalake-2.3.1/test/test_list.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/test/test_logging.py` & `datalake-2.3.1/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/test/test_queue.py` & `datalake-2.3.1/test/test_queue.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/test/test_translator.py` & `datalake-2.3.1/test/test_translator.py`

 * *Files identical despite different names*

### Comparing `datalake-2.3/versioneer.py` & `datalake-2.3.1/versioneer.py`

 * *Files identical despite different names*

