# Comparing `tmp/tablecache-4.0.0rc0.tar.gz` & `tmp/tablecache-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablecache-4.0.0rc0.tar", last modified: Tue Apr  2 05:13:26 2024, max compression
+gzip compressed data, was "tablecache-4.1.0.tar", last modified: Thu Apr  4 17:26:48 2024, max compression
```

## Comparing `tablecache-4.0.0rc0.tar` & `tablecache-4.1.0.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 05:13:26.653800 tablecache-4.0.0rc0/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-02 05:13:26.653800 tablecache-4.0.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 05:13:26.645800 tablecache-4.0.0rc0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/requirements/local.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/requirements/postgres.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/requirements/redis.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 05:13:26.653800 tablecache-4.0.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 05:13:26.645800 tablecache-4.0.0rc0/tablecache/
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tablecache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24310 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tablecache/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tablecache/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tablecache/index.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 05:13:26.645800 tablecache-4.0.0rc0/tablecache/local/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tablecache/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14058 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tablecache/local/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 05:13:26.645800 tablecache-4.0.0rc0/tablecache/postgres/
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tablecache/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tablecache/postgres/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 05:13:26.645800 tablecache-4.0.0rc0/tablecache/redis/
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tablecache/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tablecache/redis/codec.py
--rw-r--r--   0 runner    (1001) docker     (127)    35091 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tablecache/redis/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tablecache/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tablecache/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 05:13:26.649800 tablecache-4.0.0rc0/tablecache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-02 05:13:26.000000 tablecache-4.0.0rc0/tablecache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-02 05:13:26.000000 tablecache-4.0.0rc0/tablecache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 05:13:26.000000 tablecache-4.0.0rc0/tablecache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-02 05:13:26.000000 tablecache-4.0.0rc0/tablecache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 05:13:26.000000 tablecache-4.0.0rc0/tablecache.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 05:13:26.649800 tablecache-4.0.0rc0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    62150 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    16610 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tests/test_indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tests/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:26:48.674941 tablecache-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-04 17:26:45.000000 tablecache-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-04 17:26:45.000000 tablecache-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-04 17:26:48.674941 tablecache-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-04 17:26:45.000000 tablecache-4.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-04 17:26:45.000000 tablecache-4.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:26:48.666941 tablecache-4.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:26:45.000000 tablecache-4.1.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-04 17:26:45.000000 tablecache-4.1.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-04 17:26:45.000000 tablecache-4.1.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-04 17:26:45.000000 tablecache-4.1.0/requirements/local.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 17:26:45.000000 tablecache-4.1.0/requirements/postgres.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-04 17:26:45.000000 tablecache-4.1.0/requirements/prometheus.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-04 17:26:45.000000 tablecache-4.1.0/requirements/redis.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-04 17:26:45.000000 tablecache-4.1.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 17:26:48.674941 tablecache-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-04 17:26:45.000000 tablecache-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:26:48.670941 tablecache-4.1.0/tablecache/
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-04 17:26:45.000000 tablecache-4.1.0/tablecache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26933 2024-04-04 17:26:45.000000 tablecache-4.1.0/tablecache/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-04 17:26:45.000000 tablecache-4.1.0/tablecache/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-04 17:26:45.000000 tablecache-4.1.0/tablecache/index.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:26:48.670941 tablecache-4.1.0/tablecache/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-04 17:26:45.000000 tablecache-4.1.0/tablecache/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14942 2024-04-04 17:26:45.000000 tablecache-4.1.0/tablecache/local/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-04 17:26:45.000000 tablecache-4.1.0/tablecache/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:26:48.670941 tablecache-4.1.0/tablecache/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-04 17:26:45.000000 tablecache-4.1.0/tablecache/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-04 17:26:45.000000 tablecache-4.1.0/tablecache/postgres/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:26:48.670941 tablecache-4.1.0/tablecache/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-04 17:26:45.000000 tablecache-4.1.0/tablecache/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-04-04 17:26:45.000000 tablecache-4.1.0/tablecache/redis/codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35091 2024-04-04 17:26:45.000000 tablecache-4.1.0/tablecache/redis/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-04-04 17:26:45.000000 tablecache-4.1.0/tablecache/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-04 17:26:45.000000 tablecache-4.1.0/tablecache/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:26:48.670941 tablecache-4.1.0/tablecache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-04 17:26:48.000000 tablecache-4.1.0/tablecache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-04 17:26:48.000000 tablecache-4.1.0/tablecache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 17:26:48.000000 tablecache-4.1.0/tablecache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-04 17:26:48.000000 tablecache-4.1.0/tablecache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 17:26:48.000000 tablecache-4.1.0/tablecache.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:26:48.670941 tablecache-4.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    66060 2024-04-04 17:26:45.000000 tablecache-4.1.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-04 17:26:45.000000 tablecache-4.1.0/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16610 2024-04-04 17:26:45.000000 tablecache-4.1.0/tests/test_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-04 17:26:45.000000 tablecache-4.1.0/tests/test_storage.py
```

### Comparing `tablecache-4.0.0rc0/LICENSE` & `tablecache-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tablecache-4.0.0rc0/PKG-INFO` & `tablecache-4.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tablecache
-Version: 4.0.0rc0
+Version: 4.1.0
 Summary: Simple cache for unwieldily joined relations.
 Author: Marc Lehmann
 Author-email: marc.lehmann@gmx.de
 License: AGPL-3.0-or-later
 Project-URL: Github, https://github.com/dddsnn/tablecache
 Project-URL: Documentation, https://tablecache.readthedocs.io
 Requires-Python: >=3.12
@@ -13,38 +13,42 @@
 Provides-Extra: redis
 Requires-Dist: redis[hiredis]==4.*,>=4.5.5; extra == "redis"
 Requires-Dist: aiorwlock==1.4.0; extra == "redis"
 Provides-Extra: local
 Requires-Dist: sortedcontainers==2.*,>=2.4.0; extra == "local"
 Requires-Dist: aiorwlock==1.4.0; extra == "local"
 Provides-Extra: test
-Requires-Dist: asyncpg>=0.27.0; extra == "test"
 Requires-Dist: redis[hiredis]==4.*,>=4.5.5; extra == "test"
 Requires-Dist: sortedcontainers==2.*,>=2.4.0; extra == "test"
+Requires-Dist: PyHamcrest>=2.0.4; extra == "test"
 Requires-Dist: pytest>=7.4.0; extra == "test"
+Requires-Dist: asyncpg>=0.27.0; extra == "test"
 Requires-Dist: aiorwlock==1.4.0; extra == "test"
-Requires-Dist: PyHamcrest>=2.0.4; extra == "test"
+Requires-Dist: prometheus_client==0.20.0; extra == "test"
 Requires-Dist: pytest-asyncio==0.21.1; extra == "test"
 Provides-Extra: docs
 Requires-Dist: myst-parser==2.*,>=2.0.0; extra == "docs"
-Requires-Dist: sphinx-rtd-theme==2.*,>=2.0.0; extra == "docs"
 Requires-Dist: sphinx==7.*,>=7.2.6; extra == "docs"
+Requires-Dist: sphinx-rtd-theme==2.*,>=2.0.0; extra == "docs"
+Provides-Extra: prometheus
+Requires-Dist: prometheus_client==0.20.0; extra == "prometheus"
 Provides-Extra: dev
-Requires-Dist: asyncpg>=0.27.0; extra == "dev"
+Requires-Dist: sphinx-rtd-theme==2.*,>=2.0.0; extra == "dev"
+Requires-Dist: myst-parser==2.*,>=2.0.0; extra == "dev"
+Requires-Dist: flake8>=6.1.0; extra == "dev"
 Requires-Dist: redis[hiredis]==4.*,>=4.5.5; extra == "dev"
 Requires-Dist: sortedcontainers==2.*,>=2.4.0; extra == "dev"
-Requires-Dist: flake8>=6.1.0; extra == "dev"
-Requires-Dist: pytest>=7.4.0; extra == "dev"
-Requires-Dist: sphinx-rtd-theme==2.*,>=2.0.0; extra == "dev"
 Requires-Dist: autopep8>=2.0.4; extra == "dev"
-Requires-Dist: Flake8-pyproject>=1.2.3; extra == "dev"
-Requires-Dist: myst-parser==2.*,>=2.0.0; extra == "dev"
-Requires-Dist: aiorwlock==1.4.0; extra == "dev"
-Requires-Dist: sphinx==7.*,>=7.2.6; extra == "dev"
 Requires-Dist: PyHamcrest>=2.0.4; extra == "dev"
+Requires-Dist: sphinx==7.*,>=7.2.6; extra == "dev"
+Requires-Dist: pytest>=7.4.0; extra == "dev"
+Requires-Dist: asyncpg>=0.27.0; extra == "dev"
+Requires-Dist: aiorwlock==1.4.0; extra == "dev"
+Requires-Dist: prometheus_client==0.20.0; extra == "dev"
+Requires-Dist: Flake8-pyproject>=1.2.3; extra == "dev"
 Requires-Dist: pytest-asyncio==0.21.1; extra == "dev"
 Provides-Extra: postgres
 Requires-Dist: asyncpg>=0.27.0; extra == "postgres"
 
 # tablecache
 
 Simple cache for unwieldily joined relations.
```

### Comparing `tablecache-4.0.0rc0/README.md` & `tablecache-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tablecache-4.0.0rc0/setup.py` & `tablecache-4.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `tablecache-4.0.0rc0/tablecache/__init__.py` & `tablecache-4.1.0/tablecache/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 more likely, big joins of many tables) in a faster storage. It allows you to
 define ways to index the data and then query ranges of records performantly.
 Not all records have to be loaded into the cache, and ones that aren't are
 transparently fetched from the underlying database instead. Cache entries that
 become invalid must be marked as invalid, but are then refreshed automatically.
 """
 
-__version__ = '4.0.0rc0'
+__version__ = '4.1.0'
 
 from tablecache.cache import CachedTable
 from tablecache.db import DbAccess, DbRecordsSpec, QueryArgsDbRecordsSpec
 from tablecache.index import (
     Adjustment,
     AllIndexes,
     Indexes,
```

### Comparing `tablecache-4.0.0rc0/tablecache/cache.py` & `tablecache-4.1.0/tablecache/cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 import asyncio
 import collections.abc as ca
 import logging
 import typing as t
 
 import tablecache.db as db
 import tablecache.index as index
+import tablecache.metrics as metrics
 import tablecache.storage as storage
 import tablecache.types as tp
 
 
 class CachedTable[Record, PrimaryKey: tp.PrimaryKey]:
     """
     A cached table.
@@ -82,14 +83,34 @@
         self._db_access = db_access
         self._storage_table = storage_table
         self._invalid_record_repo = InvalidRecordRepository(indexes)
         self._loaded_event = asyncio.Event()
         self._scratch_space_lock = asyncio.Lock()
         self._logger = logging.getLogger(
             f'tablecache.CachedTable({storage_table.name})')
+        self._metric_reads = metrics.get_counter(
+            'tablecache_cached_table_reads_total',
+            'Number of read operations on the cached table',
+            ['table_name', 'type'])
+        self._metric_refreshes = metrics.get_counter(
+            'tablecache_cached_table_refreshes_total',
+            'Number of refreshes performed on the cached table',
+            ['table_name']).labels(table_name=storage_table.name)
+        self._metric_adjustments = metrics.get_counter(
+            'tablecache_cached_table_adjustments_total',
+            'Number of adjustments performed on the cached table',
+            ['table_name']).labels(table_name=storage_table.name)
+        self._metric_adjustments_expired = metrics.get_counter(
+            'tablecache_cached_table_adjustment_expired_total',
+            'Number of records expired during adjustments on the cached table',
+            ['table_name']).labels(table_name=storage_table.name)
+        self._metric_adjustments_loaded = metrics.get_counter(
+            'tablecache_cached_table_adjustment_loaded_total',
+            'Number of records loaded during adjustments on the cached table',
+            ['table_name']).labels(table_name=storage_table.name)
 
     async def loaded(self):
         """
         Wait until the table is loaded.
 
         Blocks until the initial load completes. Once this returns, read access
         becomes enabled. This can be used e.g. in a readiness check.
@@ -161,14 +182,17 @@
             delete = self._storage_table.delete_records
         num_deleted, num_loaded = await self._apply_adjustment(
             adjustment, put, delete)
         if use_scratch:
             self._storage_table.scratch_merge()
         self._logger.info(f'Applying {adjustment}.')
         self._indexes.commit_adjustment(adjustment)
+        self._metric_adjustments_expired.inc(num_deleted)
+        self._metric_adjustments_loaded.inc(num_loaded)
+        self._metric_adjustments.inc()
         return num_deleted, num_loaded
 
     async def _apply_adjustment(self, adjustment, put, delete):
         num_deleted = num_loaded = 0
         if adjustment.expire_spec:
             async for record in delete(adjustment.expire_spec):
                 adjustment.observe_expired(record)
@@ -269,55 +293,62 @@
         try:
             get_from_storage = self._indexes.covers(index_spec)
         except index.UnsupportedIndexOperation as e:
             raise ValueError(
                 'Indexes don\'t support coverage check on '
                 f'{index_spec.index_name}.') from e
         if get_from_storage:
-            records = await self._check_and_get_records_from_storage(
-                index_spec)
+            records, read_type = (
+                await self._check_and_get_records_from_storage(index_spec))
         else:
+            read_type = 'cache_miss'
             db_records_spec = self._indexes.db_records_spec(
                 index_spec)
             records = self._db_access.get_records(db_records_spec)
+        self._metric_reads.labels(
+            table_name=self._storage_table.name, type=read_type).inc()
         try:
             async for record in records:
                 yield record
         finally:
             await records.aclose()
 
     async def _check_and_get_records_from_storage(self, index_spec):
+        read_type = 'cache_hit'
         records_spec = self._indexes.storage_records_spec(index_spec)
         if not self._intervals_are_valid(records_spec):
+            read_type = 'cache_hit_with_refresh'
             await self.refresh_invalid()
-        return self._storage_table.get_records(records_spec)
+        return self._storage_table.get_records(records_spec), read_type
 
     def _intervals_are_valid(self, records_spec):
         for interval in records_spec.score_intervals:
             if self._invalid_record_repo.interval_intersects_invalid(
                     records_spec.index_name, interval):
                 return False
         return True
 
     def invalidate_records(
             self,
             old_index_specs: list[index.Indexes[Record, PrimaryKey].IndexSpec],
-            new_index_specs: list[index.Indexes[Record, PrimaryKey].IndexSpec]
+            new_index_specs: list[index.Indexes[Record, PrimaryKey].IndexSpec],
+            *, force_refresh_on_next_read: bool = True
     ) -> None:
         """
         Mark records in storage as invalid.
 
         All records that are currently in storage and match any index spec in
         ``old_index_specs`` or ``new_index_specs`` are marked as invalid. This
-        means that before any future request for any of these records, they are
-        guaranteed to be refreshed (i.e. fetched from the DB) first. This
-        guarantee holds for read operations that start after this method
-        returns. Reads that have already started (in a different task) may
-        respect invalidations that happen here, but probably won't. It is valid
-        to specify records that haven't actually changed (they will be
+        stores the information necessary to do a refresh (i.e. fetch from the
+        DB) of these records. If force_refresh_on_next_read is True, any future
+        request for any of these records is guaranteed to trigger a refresh
+        first. This guarantee holds for read operations that start after this
+        method returns. Reads that have already started (in a different task)
+        may respect invalidations that happen here, but probably won't. It is
+        valid to specify records that haven't actually changed (they will be
         refreshed as well, though).
 
         During a refresh, all records matching the first index spec in
         ``old_index_specs`` are deleted, then records are loaded again using
         the first index spec in ``new_index_specs``. It is valid (and perfectly
         reasonable for many setups) if old_index_specs == new_index_specs.
 
@@ -351,29 +382,36 @@
 
         :param old_index_specs: Specifications of the sets of records that
             should be invalidated, using their old (i.e. now possibly invalid)
             scores. Must not be empty, and may contain a specification for any
             available index.
         :param new_index_specs: Like ``old_index_specs``, but specifying the
             same records by their new (possibly updated) scores.
+        :param force_refresh_on_next_read: Whether to do an automatic refresh
+            before the next read for any of the invalidated records. The
+            refresh is executed lazily when the read arrives, not immediately.
+            If False, the invalid records will continue to be served from
+            storage. A manual refresh must be performed (using
+            :py:meth:`refresh_invalid`).
         :raise ValueError: If the table is not yet loaded, an index is
             specified more than once, or one of the index specs lists is empty.
         """
         if not self._loaded_event.is_set():
             raise ValueError('Table is not yet loaded.')
         old_index_for_refresh, old_specs_by_name = (
             self._parse_index_specs_for_invalidation(old_index_specs))
         new_index_for_refresh, new_specs_by_name = (
             self._parse_index_specs_for_invalidation(new_index_specs))
         if not old_index_for_refresh or not new_index_for_refresh:
             raise ValueError(
                 'At least one old and one new index spec must be given.')
         self._invalid_record_repo.flag_invalid(
             old_specs_by_name, new_specs_by_name, old_index_for_refresh,
-            new_index_for_refresh)
+            new_index_for_refresh,
+            consider_in_intersects_check=force_refresh_on_next_read)
 
     def _parse_index_specs_for_invalidation(self, index_specs):
         first_index_name = None
         specs_by_name = {}
         for index_spec in index_specs:
             if index_spec.index_name in specs_by_name:
                 raise ValueError(
@@ -426,14 +464,15 @@
                 await self._storage_table.scratch_put_record(record)
                 num_loaded += 1
         self._storage_table.scratch_merge()
         self._invalid_record_repo.clear()
         self._logger.info(
             f'Refresh done. Deleted {num_deleted} and loaded {num_loaded} '
             f'records across {len(old_and_new_specs)} index spec pairs.')
+        self._metric_refreshes.inc()
 
 
 class InvalidRecordRepository[Record, PrimaryKey: tp.PrimaryKey]:
     """
     A repository of invalid records.
 
     Keeps track of intervals of records scores which have been marked as
@@ -449,47 +488,52 @@
 
     def flag_invalid(
         self,
         old_index_specs:
             t.Mapping[str, index.Indexes[Record, PrimaryKey].IndexSpec],
         new_index_specs:
             t.Mapping[str, index.Indexes[Record, PrimaryKey].IndexSpec],
-        old_index_for_refresh: str, new_index_for_refresh: str
+        old_index_for_refresh: str, new_index_for_refresh: str,
+        consider_in_intersects_check: bool
     ) -> None:
         """
         Flag records as invalid.
 
         Takes 2 dictionaries of index specs, one specifying the invalid records
         as they exist in storage now, the other specifying the updated records.
         These may be the same. Each dictionary maps index names to
-        corresponding index specs. All score intervals in the corresponding
-        StorageRecordsSpecs will be considered invalid in
-        interval_intersects_invalid(). Any keys in the dictionaries that aren't
-        names of indexes are ignored.
-
-        Not every index has to be present in the specs, but for the ones that
-        aren't the respective index is marked as dirty. This means that future
-        calls to interval_intersects_invalid() for that index will always
-        return True, since there is no longer a way to know what scores are
-        valid.
+        corresponding index specs. Not every index has to be present in the
+        specs, but missing ones may be marked as dirty. Any keys in the
+        dictionaries that aren't names of indexes are ignored.
 
         One old and one new index spec is stored to be part of
         specs_for_refresh(). Which are chosen must be specified via
         {old,new}_index_for_refresh. These must be keys into the respective
         dictionaries.
+
+        If consider_in_intersects_check is True, all score intervals in the
+        corresponding StorageRecordsSpecs will be considered invalid in
+        interval_intersects_invalid(). Additionally, any indexes that are
+        missing are marked as dirty, i.e. future calls to
+        interval_intersects_invalid() for that index will always return True,
+        since there is no longer a way to know what scores are valid.
+
+        :param consider_in_intersects_check: Whether to consider the records
+            invalid in interval_intersects_invalid().
         """
         if not old_index_specs or not new_index_specs:
             raise ValueError(
                 'Must provide at least one old and one new index spec.')
         self._specs_for_refresh.append(
             (old_index_specs[old_index_for_refresh],
              new_index_specs[new_index_for_refresh]))
-        for index_name in self._indexes.index_names:
-            self._record_invalid_intervals(
-                index_name, old_index_specs, new_index_specs)
+        if consider_in_intersects_check:
+            for index_name in self._indexes.index_names:
+                self._record_invalid_intervals(
+                    index_name, old_index_specs, new_index_specs)
 
     def _record_invalid_intervals(
             self, index_name, old_index_specs, new_index_specs):
         try:
             old_index_spec = old_index_specs[index_name]
             new_index_spec = new_index_specs[index_name]
         except KeyError:
```

### Comparing `tablecache-4.0.0rc0/tablecache/db.py` & `tablecache-4.1.0/tablecache/db.py`

 * *Files identical despite different names*

### Comparing `tablecache-4.0.0rc0/tablecache/index.py` & `tablecache-4.1.0/tablecache/index.py`

 * *Files identical despite different names*

### Comparing `tablecache-4.0.0rc0/tablecache/local/__init__.py` & `tablecache-4.1.0/tablecache/local/__init__.py`

 * *Files identical despite different names*

### Comparing `tablecache-4.0.0rc0/tablecache/local/storage.py` & `tablecache-4.1.0/tablecache/local/storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import typing as t
 import uuid
 
 import aiorwlock
 import sortedcontainers
 
 import tablecache.index as index
+import tablecache.metrics as metrics
 import tablecache.storage as storage
 import tablecache.types as tp
 
 
 def _always_true(*args, **kwargs): return True
 
 
@@ -84,25 +85,40 @@
         self._record_scorer = record_scorer
         self._table_name = table_name
         if self._table_name is None:
             self._table_name = str(uuid.uuid4())
         self._scratch_condition = asyncio.Condition()
         self._scratch_merge_task = None
         self._scratch_merge_read_lock = aiorwlock.RWLock()
+        self._metric_records = metrics.get_gauge(
+            'tablecache_local_table_records_total',
+            'Number of records currently in the table',
+            ['table_name', 'type'])
         self._reset_record_storage()
 
     def __repr__(self) -> str:
         return f'Local table {self.name} ({len(self._records)} records)'
 
     def _reset_record_storage(self):
         self._records = {}
         self._scratch_records = {}
         self._indexes = self._make_index_dict()
         self._scratch_indexes = self._make_index_dict()
         self._scratch_records_to_delete = {}
+        self._set_records_metrics()
+
+    def _set_records_metrics(self):
+        self._metric_records.labels(
+            table_name=self.name, type='regular').set(len(self._records))
+        self._metric_records.labels(
+            table_name=self.name, type='scratch').set(
+                len(self._scratch_records))
+        self._metric_records.labels(
+            table_name=self.name, type='scratch_delete').set(
+                len(self._scratch_records_to_delete))
 
     def _make_index_dict(self):
         return {
             index_name: sortedcontainers.SortedKeyList(key=op.itemgetter(0))
             for index_name in self._record_scorer.index_names}
 
     @t.override
@@ -123,14 +139,15 @@
         after the scratch merge finishes.
 
         :param record: The record to add.
         """
         async with self._scratch_condition:
             await self._scratch_condition.wait_for(self._scratch_is_clear)
             self._put_record_to_dicts(record, self._records, self._indexes)
+        self._set_records_metrics()
 
     def _put_record_to_dicts(self, record, records, indexes):
         primary_key = self._record_scorer.primary_key(record)
         try:
             existing_record = records.pop(primary_key)
             self._discard_record_from_dicts(
                 existing_record, records, indexes, primary_key)
@@ -221,14 +238,15 @@
             records_to_delete = [
                 r async for r in self.get_records(records_spec)]
             for record in records_to_delete:
                 self._discard_record_from_dicts(
                     record, self._records, self._indexes)
                 yield record
                 await asyncio.sleep(0)  # Yield to event loop to remain lively.
+        self._set_records_metrics()
 
     @property
     def _include_scratch_records(self):
         return self._scratch_merge_task is not None
 
     def _scratch_is_not_merging(self):
         return self._scratch_merge_task is None
@@ -249,14 +267,15 @@
         """
         async with self._scratch_condition:
             await self._scratch_condition.wait_for(
                 self._scratch_is_not_merging)
             primary_key = self._put_record_to_dicts(
                 record, self._scratch_records, self._scratch_indexes)
             self._scratch_records_to_delete.pop(primary_key, None)
+        self._set_records_metrics()
 
     @t.override
     async def scratch_discard_records(
             self, records_spec: storage.StorageRecordsSpec[Record]
     ) -> ca.AsyncIterable[Record]:
         """
         Mark a set of records to be deleted in scratch space.
@@ -290,14 +309,15 @@
                 score = self._record_scorer.score(index_name, record)
                 self._scratch_indexes[index_name].discard((score, record))
             await asyncio.sleep(0)  # Yield to event loop to remain lively.
         async for record in self.get_records(records_spec):
             primary_key = self._record_scorer.primary_key(record)
             self._scratch_records_to_delete[primary_key] = record
             yield record
+        self._set_records_metrics()
 
     @t.override
     def scratch_merge(self) -> None:
         """
         Merge scratch space.
 
         This immediately causes read operations to reflect the state of the
@@ -324,7 +344,8 @@
                     primary_key)
             await asyncio.sleep(0)  # Yield to event loop to remain lively.
         assert not any(self._scratch_indexes.values())
         assert not self._scratch_records_to_delete
         self._scratch_merge_task = None
         async with self._scratch_condition:
             self._scratch_condition.notify_all()
+        self._set_records_metrics()
```

### Comparing `tablecache-4.0.0rc0/tablecache/postgres/__init__.py` & `tablecache-4.1.0/tablecache/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `tablecache-4.0.0rc0/tablecache/postgres/db.py` & `tablecache-4.1.0/tablecache/postgres/db.py`

 * *Files identical despite different names*

### Comparing `tablecache-4.0.0rc0/tablecache/redis/__init__.py` & `tablecache-4.1.0/tablecache/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `tablecache-4.0.0rc0/tablecache/redis/codec.py` & `tablecache-4.1.0/tablecache/redis/codec.py`

 * *Files identical despite different names*

### Comparing `tablecache-4.0.0rc0/tablecache/redis/storage.py` & `tablecache-4.1.0/tablecache/redis/storage.py`

 * *Files identical despite different names*

### Comparing `tablecache-4.0.0rc0/tablecache/storage.py` & `tablecache-4.1.0/tablecache/storage.py`

 * *Files identical despite different names*

### Comparing `tablecache-4.0.0rc0/tablecache/types.py` & `tablecache-4.1.0/tablecache/types.py`

 * *Files identical despite different names*

### Comparing `tablecache-4.0.0rc0/tablecache.egg-info/PKG-INFO` & `tablecache-4.1.0/tablecache.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tablecache
-Version: 4.0.0rc0
+Version: 4.1.0
 Summary: Simple cache for unwieldily joined relations.
 Author: Marc Lehmann
 Author-email: marc.lehmann@gmx.de
 License: AGPL-3.0-or-later
 Project-URL: Github, https://github.com/dddsnn/tablecache
 Project-URL: Documentation, https://tablecache.readthedocs.io
 Requires-Python: >=3.12
@@ -13,38 +13,42 @@
 Provides-Extra: redis
 Requires-Dist: redis[hiredis]==4.*,>=4.5.5; extra == "redis"
 Requires-Dist: aiorwlock==1.4.0; extra == "redis"
 Provides-Extra: local
 Requires-Dist: sortedcontainers==2.*,>=2.4.0; extra == "local"
 Requires-Dist: aiorwlock==1.4.0; extra == "local"
 Provides-Extra: test
-Requires-Dist: asyncpg>=0.27.0; extra == "test"
 Requires-Dist: redis[hiredis]==4.*,>=4.5.5; extra == "test"
 Requires-Dist: sortedcontainers==2.*,>=2.4.0; extra == "test"
+Requires-Dist: PyHamcrest>=2.0.4; extra == "test"
 Requires-Dist: pytest>=7.4.0; extra == "test"
+Requires-Dist: asyncpg>=0.27.0; extra == "test"
 Requires-Dist: aiorwlock==1.4.0; extra == "test"
-Requires-Dist: PyHamcrest>=2.0.4; extra == "test"
+Requires-Dist: prometheus_client==0.20.0; extra == "test"
 Requires-Dist: pytest-asyncio==0.21.1; extra == "test"
 Provides-Extra: docs
 Requires-Dist: myst-parser==2.*,>=2.0.0; extra == "docs"
-Requires-Dist: sphinx-rtd-theme==2.*,>=2.0.0; extra == "docs"
 Requires-Dist: sphinx==7.*,>=7.2.6; extra == "docs"
+Requires-Dist: sphinx-rtd-theme==2.*,>=2.0.0; extra == "docs"
+Provides-Extra: prometheus
+Requires-Dist: prometheus_client==0.20.0; extra == "prometheus"
 Provides-Extra: dev
-Requires-Dist: asyncpg>=0.27.0; extra == "dev"
+Requires-Dist: sphinx-rtd-theme==2.*,>=2.0.0; extra == "dev"
+Requires-Dist: myst-parser==2.*,>=2.0.0; extra == "dev"
+Requires-Dist: flake8>=6.1.0; extra == "dev"
 Requires-Dist: redis[hiredis]==4.*,>=4.5.5; extra == "dev"
 Requires-Dist: sortedcontainers==2.*,>=2.4.0; extra == "dev"
-Requires-Dist: flake8>=6.1.0; extra == "dev"
-Requires-Dist: pytest>=7.4.0; extra == "dev"
-Requires-Dist: sphinx-rtd-theme==2.*,>=2.0.0; extra == "dev"
 Requires-Dist: autopep8>=2.0.4; extra == "dev"
-Requires-Dist: Flake8-pyproject>=1.2.3; extra == "dev"
-Requires-Dist: myst-parser==2.*,>=2.0.0; extra == "dev"
-Requires-Dist: aiorwlock==1.4.0; extra == "dev"
-Requires-Dist: sphinx==7.*,>=7.2.6; extra == "dev"
 Requires-Dist: PyHamcrest>=2.0.4; extra == "dev"
+Requires-Dist: sphinx==7.*,>=7.2.6; extra == "dev"
+Requires-Dist: pytest>=7.4.0; extra == "dev"
+Requires-Dist: asyncpg>=0.27.0; extra == "dev"
+Requires-Dist: aiorwlock==1.4.0; extra == "dev"
+Requires-Dist: prometheus_client==0.20.0; extra == "dev"
+Requires-Dist: Flake8-pyproject>=1.2.3; extra == "dev"
 Requires-Dist: pytest-asyncio==0.21.1; extra == "dev"
 Provides-Extra: postgres
 Requires-Dist: asyncpg>=0.27.0; extra == "postgres"
 
 # tablecache
 
 Simple cache for unwieldily joined relations.
```

### Comparing `tablecache-4.0.0rc0/tablecache.egg-info/SOURCES.txt` & `tablecache-4.1.0/tablecache.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 pyproject.toml
 setup.py
 requirements/base.txt
 requirements/dev.txt
 requirements/docs.txt
 requirements/local.txt
 requirements/postgres.txt
+requirements/prometheus.txt
 requirements/redis.txt
 requirements/test.txt
 tablecache/__init__.py
 tablecache/cache.py
 tablecache/db.py
 tablecache/index.py
+tablecache/metrics.py
 tablecache/storage.py
 tablecache/types.py
 tablecache.egg-info/PKG-INFO
 tablecache.egg-info/SOURCES.txt
 tablecache.egg-info/dependency_links.txt
 tablecache.egg-info/requires.txt
 tablecache.egg-info/top_level.txt
```

### Comparing `tablecache-4.0.0rc0/tests/test_cache.py` & `tablecache-4.1.0/tests/test_cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -1026,15 +1026,15 @@
         assert not self.table_has_invalid_records(table)
         table.invalidate_records(
             [indexes.IndexSpec('x_range', min=12, max=14)],
             [indexes.IndexSpec('x_range', min=102, max=104)])
         assert self.table_has_invalid_records(table)
         assert_that(
             await collect_async_iter(
-                table.get_records('x_range', min=11, max=13)),
+                table.get_records('x_range', min=11, max=14)),
             contains_inanyorder(
                 has_entries(pk=1, x=11, source='storage')))
         assert not self.table_has_invalid_records(table)
 
     async def test_refreshes_after_invalidate_records_on_affected_new(
             self, make_tables, db_access):
         indexes = MultiIndexes()
@@ -1046,17 +1046,18 @@
         assert not self.table_has_invalid_records(table)
         table.invalidate_records(
             [indexes.IndexSpec('x_range', min=12, max=14)],
             [indexes.IndexSpec('x_range', min=102, max=104)])
         assert self.table_has_invalid_records(table)
         assert_that(
             await collect_async_iter(
-                table.get_records('x_range', min=101, max=103)),
+                table.get_records('x_range', min=101, max=104)),
             contains_inanyorder(
-                has_entries(pk=2, x=102, source='storage')))
+                has_entries(pk=2, x=102, source='storage'),
+                has_entries(pk=3, x=103, source='storage')))
         assert not self.table_has_invalid_records(table)
 
     async def test_doesnt_refresh_after_invalidate_records_on_unaffected_old(
             self, make_tables, db_access):
         indexes = MultiIndexes()
         table, _ = make_tables(indexes)
         db_access.records = [{'pk': i, 'x': i + 10} for i in range(6)]
@@ -1090,14 +1091,66 @@
             [indexes.IndexSpec('x_range', min=102, max=104)])
         assert self.table_has_invalid_records(table)
         assert_that(
             await collect_async_iter(
                 table.get_records('x_range', min=104, max=106)), empty())
         assert self.table_has_invalid_records(table)
 
+    async def test_doesnt_refresh_automatically_after_invalidate_records(
+            self, make_tables, db_access):
+        indexes = MultiIndexes()
+        table, _ = make_tables(indexes)
+        db_access.records = [{'pk': i, 'x': i + 10} for i in range(6)]
+        await table.load('x_range', min=10, max=106)
+        for i in range(2, 4):
+            db_access.records[i]['x'] = i + 100
+        assert not self.table_has_invalid_records(table)
+        table.invalidate_records(
+            [indexes.IndexSpec('x_range', min=12, max=14)],
+            [indexes.IndexSpec('x_range', min=102, max=104)],
+            force_refresh_on_next_read=False)
+        assert_that(
+            await collect_async_iter(
+                table.get_records('x_range', min=11, max=14)),
+            contains_inanyorder(
+                has_entries(pk=1, x=11, source='storage'),
+                has_entries(pk=2, x=12, source='storage'),
+                has_entries(pk=3, x=13, source='storage')))
+        assert_that(
+            await collect_async_iter(
+                table.get_records('x_range', min=101, max=104)), empty())
+        assert self.table_has_invalid_records(table)
+
+    async def test_refreshes_manually_after_non_automatic_invalidate_records(
+            self, make_tables, db_access):
+        indexes = MultiIndexes()
+        table, _ = make_tables(indexes)
+        db_access.records = [{'pk': i, 'x': i + 10} for i in range(6)]
+        await table.load('x_range', min=10, max=106)
+        for i in range(2, 4):
+            db_access.records[i]['x'] = i + 100
+        assert not self.table_has_invalid_records(table)
+        table.invalidate_records(
+            [indexes.IndexSpec('x_range', min=12, max=14)],
+            [indexes.IndexSpec('x_range', min=102, max=104)],
+            force_refresh_on_next_read=False)
+        await table.refresh_invalid()
+        assert_that(
+            await collect_async_iter(
+                table.get_records('x_range', min=11, max=14)),
+            contains_inanyorder(
+                has_entries(pk=1, x=11, source='storage')))
+        assert_that(
+            await collect_async_iter(
+                table.get_records('x_range', min=101, max=104)),
+            contains_inanyorder(
+                has_entries(pk=2, x=102, source='storage'),
+                has_entries(pk=3, x=103, source='storage')))
+        assert not self.table_has_invalid_records(table)
+
     async def test_invalidate_records_tolerates_overspecified_new(
             self, make_tables, db_access):
         indexes = MultiIndexes()
         table, _ = make_tables(indexes)
         db_access.records = [{'pk': i, 'x': i + 10} for i in range(6)]
         await table.load('primary_key', all_primary_keys=True)
         for i in range(2, 4):
@@ -1315,15 +1368,15 @@
         assert not repo.interval_intersects_invalid(
             'x_range', tc.Interval.everything())
         repo.flag_invalid(
             {'primary_key': indexes.IndexSpec('primary_key', 2),
              'x_range': indexes.IndexSpec('x_range', min=10, max=20)},
             {'primary_key': indexes.IndexSpec('primary_key', 2),
              'x_range': indexes.IndexSpec('x_range', min=110, max=120)},
-            'primary_key', 'primary_key')
+            'primary_key', 'primary_key', True)
         assert not repo.interval_intersects_invalid(
             'primary_key', pk_interval(float('-inf'), 2))
         assert not repo.interval_intersects_invalid(
             'x_range', x_range_interval(float('-inf'), 10))
         assert not repo.interval_intersects_invalid(
             'x_range', x_range_interval(20, 110))
         assert not repo.interval_intersects_invalid(
@@ -1344,46 +1397,70 @@
 
     def test_interval_invalid_raises_if_index_for_refresh_not_given(
             self, repo, indexes):
         with pytest.raises(KeyError):
             repo.flag_invalid(
                 {'primary_key': indexes.IndexSpec('primary_key', 2)},
                 {'primary_key': indexes.IndexSpec('primary_key', 2)},
-                'x_range', 'x_range')
+                'x_range', 'x_range', True)
 
     def test_interval_invalid_on_dirty_index(
             self, repo, indexes, x_range_interval):
         assert not repo.interval_intersects_invalid(
             'x_range', tc.Interval.everything())
         repo.flag_invalid(
             {'primary_key': indexes.IndexSpec('primary_key', 2)},
             {'primary_key': indexes.IndexSpec('primary_key', 2)},
-            'primary_key', 'primary_key')
+            'primary_key', 'primary_key', True)
         assert repo.interval_intersects_invalid(
             'x_range', x_range_interval(0, 5))
 
-    def test_specs_for_refresh(self, repo, indexes):
+    def test_interval_invalid_without_consider_not_in_intersects(
+            self, repo, indexes):
+        repo.flag_invalid(
+            {'primary_key': indexes.IndexSpec('primary_key', 2),
+             'x_range': indexes.IndexSpec('x_range', min=10, max=20)},
+            {'primary_key': indexes.IndexSpec('primary_key', 2),
+             'x_range': indexes.IndexSpec('x_range', min=110, max=120)},
+            'primary_key', 'primary_key', False)
+        assert not repo.interval_intersects_invalid(
+            'primary_key', tc.Interval.everything())
+        assert not repo.interval_intersects_invalid(
+            'x_range', tc.Interval.everything())
+
+    def test_interval_invalid_without_consider_doesnt_dirty_index(
+            self, repo, indexes):
+        repo.flag_invalid(
+            {'primary_key': indexes.IndexSpec('primary_key', 2)},
+            {'primary_key': indexes.IndexSpec('primary_key', 2)},
+            'primary_key', 'primary_key', False)
+        assert not repo.interval_intersects_invalid(
+            'x_range', tc.Interval.everything())
+
+    @pytest.mark.parametrize('consider_in_intersects_check', [True, False])
+    def test_specs_for_refresh(
+            self, repo, indexes, consider_in_intersects_check):
         assert_that(repo.specs_for_refresh(), empty())
         repo.flag_invalid(
             {'primary_key': indexes.IndexSpec('primary_key', 2)},
             {'primary_key': indexes.IndexSpec('primary_key', 2)},
-            'primary_key', 'primary_key')
+            'primary_key', 'primary_key', consider_in_intersects_check)
         assert_that(
             repo.specs_for_refresh(),
             contains_inanyorder(
                 contains_exactly(
                     has_properties(index_name='primary_key', primary_keys={2}),
                     has_properties(index_name='primary_key', primary_keys={2})
                 )))
         repo.flag_invalid(
             {'primary_key': indexes.IndexSpec('primary_key', 3),
              'x_range': indexes.IndexSpec('x_range', min=10, max=20)},
             {'primary_key': indexes.IndexSpec('primary_key', 3),
              'x_range': indexes.IndexSpec('x_range', min=110, max=120)},
-            'primary_key', 'x_range')
+            'primary_key', 'x_range', True)
         assert_that(
             repo.specs_for_refresh(),
             contains_inanyorder(
                 contains_exactly(
                     has_properties(index_name='primary_key', primary_keys={2}),
                     has_properties(index_name='primary_key', primary_keys={2})
                 ), contains_exactly(
@@ -1393,45 +1470,47 @@
 
     def test_interval_not_invalid_after_clear(self, repo, indexes):
         repo.flag_invalid(
             {'primary_key': indexes.IndexSpec('primary_key', 2),
              'x_range': indexes.IndexSpec('x_range', min=10, max=20)},
             {'primary_key': indexes.IndexSpec('primary_key', 2),
              'x_range': indexes.IndexSpec('x_range', min=110, max=120)},
-            'primary_key', 'primary_key')
+            'primary_key', 'primary_key', True)
         assert repo.interval_intersects_invalid(
             'primary_key', tc.Interval.everything())
         assert repo.interval_intersects_invalid(
             'x_range', tc.Interval.everything())
         repo.clear()
         assert not repo.interval_intersects_invalid(
             'primary_key', tc.Interval.everything())
         assert not repo.interval_intersects_invalid(
             'x_range', tc.Interval.everything())
 
     def test_index_not_dirty_after_clean(self, repo, indexes):
         repo.flag_invalid(
             {'primary_key': indexes.IndexSpec('primary_key', 2)},
             {'primary_key': indexes.IndexSpec('primary_key', 2)},
-            'primary_key', 'primary_key')
+            'primary_key', 'primary_key', True)
         assert repo.interval_intersects_invalid(
             'x_range', tc.Interval.everything())
         repo.clear()
         assert not repo.interval_intersects_invalid(
             'x_range', tc.Interval.everything())
 
-    def test_len_is_number_of_specs_for_refresh(self, repo, indexes):
+    @pytest.mark.parametrize('consider_in_intersects_check', [True, False])
+    def test_len_is_number_of_specs_for_refresh(
+            self, repo, indexes, consider_in_intersects_check):
         assert len(repo) == 0
         repo.flag_invalid(
             {'primary_key': indexes.IndexSpec('primary_key', 2)},
             {'primary_key': indexes.IndexSpec('primary_key', 2)},
-            'primary_key', 'primary_key')
+            'primary_key', 'primary_key', consider_in_intersects_check)
         assert len(repo) == 1
         repo.flag_invalid(
             {'primary_key': indexes.IndexSpec('primary_key', 3),
              'x_range': indexes.IndexSpec('x_range', min=10, max=20)},
             {'primary_key': indexes.IndexSpec('primary_key', 3),
              'x_range': indexes.IndexSpec('x_range', min=110, max=120)},
-            'primary_key', 'x_range')
+            'primary_key', 'x_range', consider_in_intersects_check)
         assert len(repo) == 2
         repo.clear()
         assert len(repo) == 0
```

### Comparing `tablecache-4.0.0rc0/tests/test_db.py` & `tablecache-4.1.0/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `tablecache-4.0.0rc0/tests/test_indexes.py` & `tablecache-4.1.0/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `tablecache-4.0.0rc0/tests/test_storage.py` & `tablecache-4.1.0/tests/test_storage.py`

 * *Files identical despite different names*

