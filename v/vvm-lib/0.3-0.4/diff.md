# Comparing `tmp/vvm_lib-0.3.tar.gz` & `tmp/vvm_lib-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vvm_lib-0.3.tar", last modified: Thu Apr  4 12:46:21 2024, max compression
+gzip compressed data, was "vvm_lib-0.4.tar", last modified: Fri Apr  5 12:47:38 2024, max compression
```

## Comparing `vvm_lib-0.3.tar` & `vvm_lib-0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 12:46:21.251080 vvm_lib-0.3/
--rw-rw-rw-   0        0        0      428 2024-04-04 12:46:21.251080 vvm_lib-0.3/PKG-INFO
--rw-rw-rw-   0        0        0       10 2024-04-04 10:32:19.000000 vvm_lib-0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-04 12:46:21.256142 vvm_lib-0.3/setup.cfg
--rw-rw-rw-   0        0        0      575 2024-04-04 12:44:42.000000 vvm_lib-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 12:46:21.225824 vvm_lib-0.3/vvm_lib/
--rw-rw-rw-   0        0        0      229 2024-04-04 10:13:09.000000 vvm_lib-0.3/vvm_lib/__init__.py
--rw-rw-rw-   0        0        0     1120 2024-04-03 11:26:36.000000 vvm_lib-0.3/vvm_lib/google_book.py
--rw-rw-rw-   0        0        0     1780 2024-04-03 11:27:48.000000 vvm_lib-0.3/vvm_lib/greenplum.py
--rw-rw-rw-   0        0        0      299 2024-04-03 11:24:43.000000 vvm_lib-0.3/vvm_lib/mssql.py
--rw-rw-rw-   0        0        0      397 2024-04-03 11:25:52.000000 vvm_lib-0.3/vvm_lib/vault.py
-drwxrwxrwx   0        0        0        0 2024-04-04 12:46:21.251080 vvm_lib-0.3/vvm_lib.egg-info/
--rw-rw-rw-   0        0        0      428 2024-04-04 12:46:21.000000 vvm_lib-0.3/vvm_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2024-04-04 12:46:21.000000 vvm_lib-0.3/vvm_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 12:46:21.000000 vvm_lib-0.3/vvm_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-04 09:46:15.000000 vvm_lib-0.3/vvm_lib.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       86 2024-04-04 12:46:21.000000 vvm_lib-0.3/vvm_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-04 12:46:21.000000 vvm_lib-0.3/vvm_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:38.690784 vvm_lib-0.4/
+-rw-rw-rw-   0        0        0      428 2024-04-05 12:47:38.689779 vvm_lib-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-04-05 12:46:01.000000 vvm_lib-0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-05 12:47:38.699807 vvm_lib-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      574 2024-04-05 12:43:44.000000 vvm_lib-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:38.666685 vvm_lib-0.4/vvm_lib/
+-rw-rw-rw-   0        0        0      229 2024-04-04 10:13:09.000000 vvm_lib-0.4/vvm_lib/__init__.py
+-rw-rw-rw-   0        0        0     2747 2024-04-05 12:41:47.000000 vvm_lib-0.4/vvm_lib/google_book.py
+-rw-rw-rw-   0        0        0     3545 2024-04-05 12:43:44.000000 vvm_lib-0.4/vvm_lib/greenplum.py
+-rw-rw-rw-   0        0        0      654 2024-04-05 12:43:44.000000 vvm_lib-0.4/vvm_lib/mssql.py
+-rw-rw-rw-   0        0        0      807 2024-04-05 12:29:39.000000 vvm_lib-0.4/vvm_lib/vault.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:38.689779 vvm_lib-0.4/vvm_lib.egg-info/
+-rw-rw-rw-   0        0        0      428 2024-04-05 12:47:38.000000 vvm_lib-0.4/vvm_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2024-04-05 12:47:38.000000 vvm_lib-0.4/vvm_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 12:47:38.000000 vvm_lib-0.4/vvm_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-04 09:46:15.000000 vvm_lib-0.4/vvm_lib.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       86 2024-04-05 12:47:38.000000 vvm_lib-0.4/vvm_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 12:47:38.000000 vvm_lib-0.4/vvm_lib.egg-info/top_level.txt
```

### Comparing `vvm_lib-0.3/setup.py` & `vvm_lib-0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='vvm_lib',
-      version='0.03',
+      version='0.4',
       description='my frequently used functions',
       packages=[
           'vvm_lib'
           ],
       author_email='v.vazhinskiy@yandex.ru',
       author="vvazhinskiy",
       url="https://github.com/VazhikVM/vvm_lib",
```

