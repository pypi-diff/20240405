# Comparing `tmp/kv-sqlite-sync-0.1.0.tar.gz` & `tmp/kv-sqlite-sync-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kv-sqlite-sync-0.1.0.tar", last modified: Thu Apr  4 15:36:32 2024, max compression
+gzip compressed data, was "kv-sqlite-sync-0.1.1.tar", last modified: Fri Apr  5 13:16:18 2024, max compression
```

## Comparing `kv-sqlite-sync-0.1.0.tar` & `kv-sqlite-sync-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 15:36:32.686316 kv-sqlite-sync-0.1.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1433 2024-04-04 15:36:32.686316 kv-sqlite-sync-0.1.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1098 2024-04-01 16:51:31.000000 kv-sqlite-sync-0.1.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      585 2024-04-04 15:35:52.000000 kv-sqlite-sync-0.1.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-04 15:36:32.686316 kv-sqlite-sync-0.1.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 15:36:32.676315 kv-sqlite-sync-0.1.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 15:36:32.676315 kv-sqlite-sync-0.1.0/src/kv/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 15:36:32.686316 kv-sqlite-sync-0.1.0/src/kv/sqlite/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      146 2024-04-02 08:50:49.000000 kv-sqlite-sync-0.1.0/src/kv/sqlite/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 15:36:32.686316 kv-sqlite-sync-0.1.0/src/kv/sqlite/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       25 2024-04-01 16:33:56.000000 kv-sqlite-sync-0.1.0/src/kv/sqlite/api/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3297 2024-04-04 07:26:32.000000 kv-sqlite-sync-0.1.0/src/kv/sqlite/api/api.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 15:36:32.686316 kv-sqlite-sync-0.1.0/src/kv/sqlite/queries/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       92 2024-04-04 07:21:00.000000 kv-sqlite-sync-0.1.0/src/kv/sqlite/queries/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1546 2024-04-04 15:32:12.000000 kv-sqlite-sync-0.1.0/src/kv/sqlite/queries/queries.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 15:36:32.686316 kv-sqlite-sync-0.1.0/src/kv_sqlite_sync.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1433 2024-04-04 15:36:32.000000 kv-sqlite-sync-0.1.0/src/kv_sqlite_sync.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      381 2024-04-04 15:36:32.000000 kv-sqlite-sync-0.1.0/src/kv_sqlite_sync.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-04 15:36:32.000000 kv-sqlite-sync-0.1.0/src/kv_sqlite_sync.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       24 2024-04-04 15:36:32.000000 kv-sqlite-sync-0.1.0/src/kv_sqlite_sync.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-04 15:36:32.000000 kv-sqlite-sync-0.1.0/src/kv_sqlite_sync.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:16:18.950853 kv-sqlite-sync-0.1.1/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      736 2024-04-05 13:16:18.950853 kv-sqlite-sync-0.1.1/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      401 2024-04-05 13:15:45.000000 kv-sqlite-sync-0.1.1/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      585 2024-04-05 13:16:17.000000 kv-sqlite-sync-0.1.1/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-05 13:16:18.950853 kv-sqlite-sync-0.1.1/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:16:18.950853 kv-sqlite-sync-0.1.1/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:16:18.950853 kv-sqlite-sync-0.1.1/src/kv/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:16:18.950853 kv-sqlite-sync-0.1.1/src/kv/sqlite/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      146 2024-04-05 13:12:45.000000 kv-sqlite-sync-0.1.1/src/kv/sqlite/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:16:18.950853 kv-sqlite-sync-0.1.1/src/kv/sqlite/api/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       25 2024-04-05 13:12:45.000000 kv-sqlite-sync-0.1.1/src/kv/sqlite/api/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3297 2024-04-05 13:12:45.000000 kv-sqlite-sync-0.1.1/src/kv/sqlite/api/api.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:16:18.950853 kv-sqlite-sync-0.1.1/src/kv/sqlite/queries/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       92 2024-04-05 13:12:45.000000 kv-sqlite-sync-0.1.1/src/kv/sqlite/queries/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1546 2024-04-05 13:12:45.000000 kv-sqlite-sync-0.1.1/src/kv/sqlite/queries/queries.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:16:18.950853 kv-sqlite-sync-0.1.1/src/kv_sqlite_sync.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      736 2024-04-05 13:16:18.000000 kv-sqlite-sync-0.1.1/src/kv_sqlite_sync.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      381 2024-04-05 13:16:18.000000 kv-sqlite-sync-0.1.1/src/kv_sqlite_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-05 13:16:18.000000 kv-sqlite-sync-0.1.1/src/kv_sqlite_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       24 2024-04-05 13:16:18.000000 kv-sqlite-sync-0.1.1/src/kv_sqlite_sync.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-05 13:16:18.000000 kv-sqlite-sync-0.1.1/src/kv_sqlite_sync.egg-info/top_level.txt
```

### Comparing `kv-sqlite-sync-0.1.0/pyproject.toml` & `kv-sqlite-sync-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kv-sqlite-sync"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Key-Value interface over SQLite. Supports any datatype, including JSON and BLOB"
 dependencies = [
   "kv-api", "haskellian", "ramda"
 ]
```

### Comparing `kv-sqlite-sync-0.1.0/src/kv/sqlite/api/api.py` & `kv-sqlite-sync-0.1.1/src/kv/sqlite/api/api.py`

 * *Files identical despite different names*

### Comparing `kv-sqlite-sync-0.1.0/src/kv/sqlite/queries/queries.py` & `kv-sqlite-sync-0.1.1/src/kv/sqlite/queries/queries.py`

 * *Files identical despite different names*

