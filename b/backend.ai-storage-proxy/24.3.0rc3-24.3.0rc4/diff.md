# Comparing `tmp/backend.ai-storage-proxy-24.3.0rc3.tar.gz` & `tmp/backend.ai-storage-proxy-24.3.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-storage-proxy-24.3.0rc3.tar", last modified: Fri Apr  5 02:25:36 2024, max compression
+gzip compressed data, was "backend.ai-storage-proxy-24.3.0rc4.tar", last modified: Fri Apr  5 03:40:02 2024, max compression
```

## Comparing `backend.ai-storage-proxy-24.3.0rc3.tar` & `backend.ai-storage-proxy-24.3.0rc4.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.258033 backend.ai-storage-proxy-24.3.0rc3/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-04-05 02:25:36.258033 backend.ai-storage-proxy-24.3.0rc3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.242032 backend.ai-storage-proxy-24.3.0rc3/ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.242032 backend.ai-storage-proxy-24.3.0rc3/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.250033 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10934 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.250033 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15195 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    39754 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/api/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/api/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.250033 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/cephfs/
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/cephfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.250033 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/ddn/
--rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/ddn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.250033 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/dellemc/
--rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/dellemc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/dellemc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7450 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/dellemc/onefs_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.254032 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/gpfs/
--rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/gpfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/gpfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13569 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/gpfs/gpfs_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/gpfs/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/migration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.254032 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/netapp/
--rw-r--r--   0 runner    (1001) docker     (127)    21159 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/netapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21068 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/netapp/netappclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.254032 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/purestorage/
--rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/purestorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/purestorage/purity.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13285 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/subproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.254032 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/vast/
--rw-r--r--   0 runner    (1001) docker     (127)     9539 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/vast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/vast/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/vast/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14745 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/vast/vastdata_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.254032 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/vfs/
--rw-r--r--   0 runner    (1001) docker     (127)    22740 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/vfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13782 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.254032 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/weka/
--rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/weka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/weka/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12723 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/weka/weka_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.254032 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/xfs/
--rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/xfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.258033 backend.ai-storage-proxy-24.3.0rc3/backend.ai_storage_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-04-05 02:25:36.000000 backend.ai-storage-proxy-24.3.0rc3/backend.ai_storage_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-05 02:25:36.000000 backend.ai-storage-proxy-24.3.0rc3/backend.ai_storage_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:36.000000 backend.ai-storage-proxy-24.3.0rc3/backend.ai_storage_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-05 02:25:36.000000 backend.ai-storage-proxy-24.3.0rc3/backend.ai_storage_proxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:36.000000 backend.ai-storage-proxy-24.3.0rc3/backend.ai_storage_proxy.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:36.000000 backend.ai-storage-proxy-24.3.0rc3/backend.ai_storage_proxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-05 02:25:36.000000 backend.ai-storage-proxy-24.3.0rc3/backend.ai_storage_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-05 02:25:36.000000 backend.ai-storage-proxy-24.3.0rc3/backend.ai_storage_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 02:25:36.258033 backend.ai-storage-proxy-24.3.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8560 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.521382 backend.ai-storage-proxy-24.3.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-04-05 03:40:02.521382 backend.ai-storage-proxy-24.3.0rc4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.509382 backend.ai-storage-proxy-24.3.0rc4/ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.509382 backend.ai-storage-proxy-24.3.0rc4/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.513382 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10934 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.513382 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15195 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39754 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/api/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/api/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.513382 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/cephfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/cephfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.513382 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/ddn/
+-rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/ddn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.513382 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/dellemc/
+-rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/dellemc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/dellemc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7450 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/dellemc/onefs_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.513382 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/gpfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/gpfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/gpfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13569 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/gpfs/gpfs_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/gpfs/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/migration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.517382 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/netapp/
+-rw-r--r--   0 runner    (1001) docker     (127)    21159 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/netapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21068 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/netapp/netappclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.517382 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/purestorage/
+-rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/purestorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/purestorage/purity.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13285 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/subproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.517382 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/vast/
+-rw-r--r--   0 runner    (1001) docker     (127)     9539 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/vast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/vast/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/vast/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14745 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/vast/vastdata_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.517382 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/vfs/
+-rw-r--r--   0 runner    (1001) docker     (127)    22740 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/vfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13782 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.517382 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/weka/
+-rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/weka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/weka/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12723 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/weka/weka_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.517382 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/xfs/
+-rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/xfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.521382 backend.ai-storage-proxy-24.3.0rc4/backend.ai_storage_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/backend.ai_storage_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/backend.ai_storage_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/backend.ai_storage_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/backend.ai_storage_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/backend.ai_storage_proxy.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/backend.ai_storage_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/backend.ai_storage_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/backend.ai_storage_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 03:40:02.521382 backend.ai-storage-proxy-24.3.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8560 2024-04-05 03:40:02.000000 backend.ai-storage-proxy-24.3.0rc4/setup.py
```

### Comparing `backend.ai-storage-proxy-24.3.0rc3/PKG-INFO` & `backend.ai-storage-proxy-24.3.0rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-storage-proxy
-Version: 24.3.0rc3
+Version: 24.3.0rc4
 Summary: Backend.AI Storage Proxy
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -24,16 +24,16 @@
 Requires-Dist: aiofiles~=0.8.0
 Requires-Dist: aiohttp_cors~=0.7
 Requires-Dist: aiohttp~=3.9.1
 Requires-Dist: aiomonitor~=0.7.0
 Requires-Dist: aiotools~=1.7.0
 Requires-Dist: asyncpg>=0.27.0
 Requires-Dist: attrs>=20.3
-Requires-Dist: backend.ai-common==24.03.0rc3
-Requires-Dist: backend.ai-plugin==24.03.0rc3
+Requires-Dist: backend.ai-common==24.03.0rc4
+Requires-Dist: backend.ai-plugin==24.03.0rc4
 Requires-Dist: click~=8.1.7
 Requires-Dist: dataclasses-json~=0.5.7
 Requires-Dist: janus~=1.0.0
 Requires-Dist: more-itertools~=8.13.0
 Requires-Dist: pyzmq~=25.1.2
 Requires-Dist: setproctitle~=1.3.2
 Requires-Dist: tenacity>=8.0
```

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/abc.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/abc.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/api/client.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/api/client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/api/manager.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/api/manager.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/cephfs/__init__.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/cephfs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/config.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/context.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/context.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/ddn/__init__.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/ddn/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/dellemc/__init__.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/dellemc/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/dellemc/exceptions.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/dellemc/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/dellemc/onefs_client.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/dellemc/onefs_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/exception.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/exception.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/gpfs/__init__.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/gpfs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/gpfs/exceptions.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/gpfs/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/gpfs/gpfs_client.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/gpfs/gpfs_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/gpfs/types.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/gpfs/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/migration.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/migration.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/netapp/__init__.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/netapp/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/netapp/netappclient.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/netapp/netappclient.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/plugin.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/plugin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/purestorage/__init__.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/purestorage/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/purestorage/purity.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/purestorage/purity.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/server.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/server.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/subproc.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/subproc.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/types.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/utils.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/vast/__init__.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/vast/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/vast/config.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/vast/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/vast/exceptions.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/vast/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/vast/vastdata_client.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/vast/vastdata_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/vfs/__init__.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/vfs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/watcher.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/watcher.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/weka/__init__.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/weka/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/weka/exceptions.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/weka/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/weka/weka_client.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/weka/weka_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/xfs/__init__.py` & `backend.ai-storage-proxy-24.3.0rc4/ai/backend/storage/xfs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/backend.ai_storage_proxy.egg-info/PKG-INFO` & `backend.ai-storage-proxy-24.3.0rc4/backend.ai_storage_proxy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-storage-proxy
-Version: 24.3.0rc3
+Version: 24.3.0rc4
 Summary: Backend.AI Storage Proxy
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -24,16 +24,16 @@
 Requires-Dist: aiofiles~=0.8.0
 Requires-Dist: aiohttp_cors~=0.7
 Requires-Dist: aiohttp~=3.9.1
 Requires-Dist: aiomonitor~=0.7.0
 Requires-Dist: aiotools~=1.7.0
 Requires-Dist: asyncpg>=0.27.0
 Requires-Dist: attrs>=20.3
-Requires-Dist: backend.ai-common==24.03.0rc3
-Requires-Dist: backend.ai-plugin==24.03.0rc3
+Requires-Dist: backend.ai-common==24.03.0rc4
+Requires-Dist: backend.ai-plugin==24.03.0rc4
 Requires-Dist: click~=8.1.7
 Requires-Dist: dataclasses-json~=0.5.7
 Requires-Dist: janus~=1.0.0
 Requires-Dist: more-itertools~=8.13.0
 Requires-Dist: pyzmq~=25.1.2
 Requires-Dist: setproctitle~=1.3.2
 Requires-Dist: tenacity>=8.0
```

### Comparing `backend.ai-storage-proxy-24.3.0rc3/backend.ai_storage_proxy.egg-info/SOURCES.txt` & `backend.ai-storage-proxy-24.3.0rc4/backend.ai_storage_proxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/backend_shim.py` & `backend.ai-storage-proxy-24.3.0rc4/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc3/setup.py` & `backend.ai-storage-proxy-24.3.0rc4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,17 +31,17 @@
         'aiofiles~=0.8.0',
         'aiohttp_cors~=0.7',
         'aiohttp~=3.9.1',
         'aiomonitor~=0.7.0',
         'aiotools~=1.7.0',
         'asyncpg>=0.27.0',
         'attrs>=20.3',
-        """backend.ai-common==24.03.0rc3
+        """backend.ai-common==24.03.0rc4
 """,
-        """backend.ai-plugin==24.03.0rc3
+        """backend.ai-plugin==24.03.0rc4
 """,
         'click~=8.1.7',
         'dataclasses-json~=0.5.7',
         'janus~=1.0.0',
         'more-itertools~=8.13.0',
         'pyzmq~=25.1.2',
         'setproctitle~=1.3.2',
@@ -260,11 +260,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.12,<3.13',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """24.03.0rc3
+    'version': """24.03.0rc4
 """,
     'zip_safe': False,
 })
```

