# Comparing `tmp/kBmc-2.3.7.tar.gz` & `tmp/kBmc-2.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kBmc-2.3.7.tar", last modified: Thu Apr  4 05:47:18 2024, max compression
+gzip compressed data, was "kBmc-2.3.8.tar", last modified: Fri Apr  5 13:55:11 2024, max compression
```

## Comparing `kBmc-2.3.7.tar` & `kBmc-2.3.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kage      (1000) kage      (1000)        0 2024-04-04 05:47:18.223357 kBmc-2.3.7/
--rw-rw-r--   0 kage      (1000) kage      (1000)     1066 2021-12-17 05:54:12.000000 kBmc-2.3.7/LICENSE
--rw-r--r--   0 kage      (1000) kage      (1000)     2875 2024-04-04 05:47:18.223357 kBmc-2.3.7/PKG-INFO
--rw-rw-r--   0 kage      (1000) kage      (1000)     2457 2021-12-19 02:10:48.000000 kBmc-2.3.7/README.md
-drwxr-xr-x   0 kage      (1000) kage      (1000)        0 2024-04-04 05:47:18.222357 kBmc-2.3.7/kBmc/
--rw-r--r--   0 kage      (1000) kage      (1000)   208397 2024-04-04 05:46:06.000000 kBmc-2.3.7/kBmc/__init__.py
-drwxr-xr-x   0 kage      (1000) kage      (1000)        0 2024-04-04 05:47:18.222357 kBmc-2.3.7/kBmc.egg-info/
--rw-rw-r--   0 kage      (1000) kage      (1000)     2875 2024-04-04 05:47:18.000000 kBmc-2.3.7/kBmc.egg-info/PKG-INFO
--rw-rw-r--   0 kage      (1000) kage      (1000)      155 2024-04-04 05:47:18.000000 kBmc-2.3.7/kBmc.egg-info/SOURCES.txt
--rw-rw-r--   0 kage      (1000) kage      (1000)        1 2024-04-04 05:47:18.000000 kBmc-2.3.7/kBmc.egg-info/dependency_links.txt
--rw-rw-r--   0 kage      (1000) kage      (1000)        5 2024-04-04 05:47:18.000000 kBmc-2.3.7/kBmc.egg-info/top_level.txt
--rw-r--r--   0 kage      (1000) kage      (1000)       38 2024-04-04 05:47:18.223357 kBmc-2.3.7/setup.cfg
--rw-rw-r--   0 kage      (1000) kage      (1000)     1975 2021-12-17 05:56:02.000000 kBmc-2.3.7/setup.py
+drwxr-xr-x   0 kage      (1000) kage      (1000)        0 2024-04-05 13:55:11.666340 kBmc-2.3.8/
+-rw-rw-r--   0 kage      (1000) kage      (1000)     1066 2021-12-17 05:54:12.000000 kBmc-2.3.8/LICENSE
+-rw-r--r--   0 kage      (1000) kage      (1000)     2875 2024-04-05 13:55:11.666340 kBmc-2.3.8/PKG-INFO
+-rw-rw-r--   0 kage      (1000) kage      (1000)     2457 2021-12-19 02:10:48.000000 kBmc-2.3.8/README.md
+drwxr-xr-x   0 kage      (1000) kage      (1000)        0 2024-04-05 13:55:11.664339 kBmc-2.3.8/kBmc/
+-rw-r--r--   0 kage      (1000) kage      (1000)   208397 2024-04-04 05:46:06.000000 kBmc-2.3.8/kBmc/__init__.py
+drwxr-xr-x   0 kage      (1000) kage      (1000)        0 2024-04-05 13:55:11.665340 kBmc-2.3.8/kBmc.egg-info/
+-rw-rw-r--   0 kage      (1000) kage      (1000)     2875 2024-04-05 13:55:11.000000 kBmc-2.3.8/kBmc.egg-info/PKG-INFO
+-rw-rw-r--   0 kage      (1000) kage      (1000)      155 2024-04-05 13:55:11.000000 kBmc-2.3.8/kBmc.egg-info/SOURCES.txt
+-rw-rw-r--   0 kage      (1000) kage      (1000)        1 2024-04-05 13:55:11.000000 kBmc-2.3.8/kBmc.egg-info/dependency_links.txt
+-rw-rw-r--   0 kage      (1000) kage      (1000)        5 2024-04-05 13:55:11.000000 kBmc-2.3.8/kBmc.egg-info/top_level.txt
+-rw-r--r--   0 kage      (1000) kage      (1000)       38 2024-04-05 13:55:11.666340 kBmc-2.3.8/setup.cfg
+-rw-rw-r--   0 kage      (1000) kage      (1000)     1975 2021-12-17 05:56:02.000000 kBmc-2.3.8/setup.py
```

### Comparing `kBmc-2.3.7/LICENSE` & `kBmc-2.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kBmc-2.3.7/PKG-INFO` & `kBmc-2.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kBmc
-Version: 2.3.7
+Version: 2.3.8
 Summary: Kage's Intelgent BMC handler
 Home-page: https://github.com/kagepark/kBmc
 Author: Kage Park
 License: MIT
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kBmc-2.3.7/README.md` & `kBmc-2.3.8/README.md`

 * *Files identical despite different names*

### Comparing `kBmc-2.3.7/kBmc/__init__.py` & `kBmc-2.3.8/kBmc/__init__.py`

 * *Files identical despite different names*

### Comparing `kBmc-2.3.7/kBmc.egg-info/PKG-INFO` & `kBmc-2.3.8/kBmc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kBmc
-Version: 2.3.7
+Version: 2.3.8
 Summary: Kage's Intelgent BMC handler
 Home-page: https://github.com/kagepark/kBmc
 Author: Kage Park
 License: MIT
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kBmc-2.3.7/setup.py` & `kBmc-2.3.8/setup.py`

 * *Files identical despite different names*

