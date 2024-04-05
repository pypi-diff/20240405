# Comparing `tmp/backend.ai-storage-proxy-24.3.0rc2.tar.gz` & `tmp/backend.ai-storage-proxy-24.3.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-storage-proxy-24.3.0rc2.tar", last modified: Sun Mar 31 14:09:12 2024, max compression
+gzip compressed data, was "backend.ai-storage-proxy-24.3.0rc3.tar", last modified: Fri Apr  5 02:25:36 2024, max compression
```

## Comparing `backend.ai-storage-proxy-24.3.0rc2.tar` & `backend.ai-storage-proxy-24.3.0rc3.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:12.059458 backend.ai-storage-proxy-24.3.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-03-31 14:09:12.059458 backend.ai-storage-proxy-24.3.0rc2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:12.051458 backend.ai-storage-proxy-24.3.0rc2/ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:12.051458 backend.ai-storage-proxy-24.3.0rc2/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:12.055458 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10934 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:12.055458 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15195 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    39754 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/api/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/api/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:12.055458 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/cephfs/
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/cephfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:12.055458 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/ddn/
--rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/ddn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:12.055458 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/dellemc/
--rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/dellemc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/dellemc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7450 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/dellemc/onefs_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:12.055458 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/gpfs/
--rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/gpfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/gpfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13569 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/gpfs/gpfs_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/gpfs/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/migration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:12.055458 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/netapp/
--rw-r--r--   0 runner    (1001) docker     (127)    20851 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/netapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19999 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/netapp/netappclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:12.059458 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/purestorage/
--rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/purestorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/purestorage/purity.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13285 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/subproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:12.059458 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/vast/
--rw-r--r--   0 runner    (1001) docker     (127)     9539 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/vast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/vast/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/vast/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14745 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/vast/vastdata_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:12.059458 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/vfs/
--rw-r--r--   0 runner    (1001) docker     (127)    22740 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/vfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13782 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:12.059458 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/weka/
--rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/weka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/weka/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12723 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/weka/weka_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:12.059458 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/xfs/
--rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/xfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:12.059458 backend.ai-storage-proxy-24.3.0rc2/backend.ai_storage_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-03-31 14:09:12.000000 backend.ai-storage-proxy-24.3.0rc2/backend.ai_storage_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-03-31 14:09:12.000000 backend.ai-storage-proxy-24.3.0rc2/backend.ai_storage_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:09:12.000000 backend.ai-storage-proxy-24.3.0rc2/backend.ai_storage_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-31 14:09:12.000000 backend.ai-storage-proxy-24.3.0rc2/backend.ai_storage_proxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:09:12.000000 backend.ai-storage-proxy-24.3.0rc2/backend.ai_storage_proxy.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/backend.ai_storage_proxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-31 14:09:12.000000 backend.ai-storage-proxy-24.3.0rc2/backend.ai_storage_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-03-31 14:09:12.000000 backend.ai-storage-proxy-24.3.0rc2/backend.ai_storage_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 14:09:12.059458 backend.ai-storage-proxy-24.3.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8560 2024-03-31 14:09:11.000000 backend.ai-storage-proxy-24.3.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.258033 backend.ai-storage-proxy-24.3.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-04-05 02:25:36.258033 backend.ai-storage-proxy-24.3.0rc3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.242032 backend.ai-storage-proxy-24.3.0rc3/ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.242032 backend.ai-storage-proxy-24.3.0rc3/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.250033 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10934 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.250033 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15195 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39754 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/api/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/api/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.250033 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/cephfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/cephfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.250033 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/ddn/
+-rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/ddn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.250033 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/dellemc/
+-rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/dellemc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/dellemc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7450 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/dellemc/onefs_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.254032 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/gpfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/gpfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/gpfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13569 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/gpfs/gpfs_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/gpfs/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/migration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.254032 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/netapp/
+-rw-r--r--   0 runner    (1001) docker     (127)    21159 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/netapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21068 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/netapp/netappclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.254032 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/purestorage/
+-rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/purestorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/purestorage/purity.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13285 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/subproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.254032 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/vast/
+-rw-r--r--   0 runner    (1001) docker     (127)     9539 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/vast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/vast/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/vast/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14745 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/vast/vastdata_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.254032 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/vfs/
+-rw-r--r--   0 runner    (1001) docker     (127)    22740 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/vfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13782 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.254032 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/weka/
+-rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/weka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/weka/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12723 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/weka/weka_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.254032 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/xfs/
+-rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/xfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.258033 backend.ai-storage-proxy-24.3.0rc3/backend.ai_storage_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-04-05 02:25:36.000000 backend.ai-storage-proxy-24.3.0rc3/backend.ai_storage_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-05 02:25:36.000000 backend.ai-storage-proxy-24.3.0rc3/backend.ai_storage_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:36.000000 backend.ai-storage-proxy-24.3.0rc3/backend.ai_storage_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-05 02:25:36.000000 backend.ai-storage-proxy-24.3.0rc3/backend.ai_storage_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:36.000000 backend.ai-storage-proxy-24.3.0rc3/backend.ai_storage_proxy.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:36.000000 backend.ai-storage-proxy-24.3.0rc3/backend.ai_storage_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-05 02:25:36.000000 backend.ai-storage-proxy-24.3.0rc3/backend.ai_storage_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-05 02:25:36.000000 backend.ai-storage-proxy-24.3.0rc3/backend.ai_storage_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 02:25:36.258033 backend.ai-storage-proxy-24.3.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8560 2024-04-05 02:25:35.000000 backend.ai-storage-proxy-24.3.0rc3/setup.py
```

### Comparing `backend.ai-storage-proxy-24.3.0rc2/PKG-INFO` & `backend.ai-storage-proxy-24.3.0rc3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-storage-proxy
-Version: 24.3.0rc2
+Version: 24.3.0rc3
 Summary: Backend.AI Storage Proxy
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -12,18 +12,41 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Requires-Python: >=3.11,<3.12
+Requires-Python: >=3.12,<3.13
 Description-Content-Type: text/markdown
+Requires-Dist: PyJWT~=2.0
+Requires-Dist: aiofiles~=0.8.0
+Requires-Dist: aiohttp_cors~=0.7
+Requires-Dist: aiohttp~=3.9.1
+Requires-Dist: aiomonitor~=0.7.0
+Requires-Dist: aiotools~=1.7.0
+Requires-Dist: asyncpg>=0.27.0
+Requires-Dist: attrs>=20.3
+Requires-Dist: backend.ai-common==24.03.0rc3
+Requires-Dist: backend.ai-plugin==24.03.0rc3
+Requires-Dist: click~=8.1.7
+Requires-Dist: dataclasses-json~=0.5.7
+Requires-Dist: janus~=1.0.0
+Requires-Dist: more-itertools~=8.13.0
+Requires-Dist: pyzmq~=25.1.2
+Requires-Dist: setproctitle~=1.3.2
+Requires-Dist: tenacity>=8.0
+Requires-Dist: tqdm>=4.61
+Requires-Dist: trafaret~=2.1
+Requires-Dist: types-aiofiles
+Requires-Dist: uvloop~=0.19.0; sys_platform != "Windows"
+Requires-Dist: yarl!=1.9.0,!=1.9.1,!=1.9.2,<2.0,>=1.8.2
+Requires-Dist: zipstream-new~=1.1.8
 
 # Backend.AI Storage Proxy
 
 Backend.AI Storage Proxy is an RPC daemon to manage vfolders used in Backend.AI agent, with quota and
 storage-specific optimization support.
 
 ## Package Structure
```

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/abc.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/abc.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/api/client.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/api/client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/api/manager.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/api/manager.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/cephfs/__init__.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/cephfs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/config.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/context.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/context.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/ddn/__init__.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/ddn/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/dellemc/__init__.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/dellemc/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/dellemc/exceptions.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/dellemc/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/dellemc/onefs_client.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/dellemc/onefs_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/exception.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/exception.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/gpfs/__init__.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/gpfs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/gpfs/exceptions.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/gpfs/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/gpfs/gpfs_client.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/gpfs/gpfs_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/gpfs/types.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/gpfs/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/migration.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/migration.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/netapp/__init__.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/netapp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,23 @@
         options: Optional[QuotaConfig] = None,
         extra_args: Optional[dict[str, Any]] = None,
     ) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
         result = await self.netapp_client.create_qtree(self.svm_id, self.volume_id, qspath.name)
         self.netapp_client.check_job_result(result, [])
         if options is not None:
-            await self.update_quota_scope(quota_scope_id, options)
+            result = await self.netapp_client.set_quota_rule(
+                self.svm_id,
+                self.volume_id,
+                qspath.name,
+                options,
+            )
+            self.netapp_client.check_job_result(result, [])
+            result = await self.netapp_client.enable_quota(self.volume_id)
+            self.netapp_client.check_job_result(result, ["5308507"])  # pass if "already on"
 
     async def describe_quota_scope(
         self,
         quota_scope_id: QuotaScopeID,
     ) -> Optional[QuotaUsage]:
         qspath = self.mangle_qspath(quota_scope_id)
         if not qspath.exists():
@@ -93,23 +101,21 @@
 
     async def update_quota_scope(
         self,
         quota_scope_id: QuotaScopeID,
         config: QuotaConfig,
     ) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
-        result = await self.netapp_client.set_quota_rule(
+        result = await self.netapp_client.update_quota_rule(
             self.svm_id,
             self.volume_id,
             qspath.name,
             config,
         )
         self.netapp_client.check_job_result(result, [])
-        result = await self.netapp_client.enable_quota(self.volume_id)
-        self.netapp_client.check_job_result(result, ["5308507"])  # pass if "already on"
 
     # FIXME: How do we implement unset_quota() for NetApp?
     async def unset_quota(self, quota_scope_id: QuotaScopeID) -> None:
         raise InvalidQuotaScopeError(
             "Unsetting folder limit without removing quota scope is not possible for this backend"
         )
 
@@ -415,14 +421,16 @@
 
     async def init(self) -> None:
         self.ontap_endpoint = self.config["netapp_ontap_endpoint"]
         self.netapp_client = NetAppClient(
             self.ontap_endpoint,
             self.config["netapp_ontap_user"],
             self.config["netapp_ontap_password"],
+            self.local_config["storage-proxy"]["user"],
+            self.local_config["storage-proxy"]["group"],
         )
         self.netapp_nfs_host = self.config["netapp_nfs_host"]
         self.netapp_xcp_cmd = self.config["netapp_xcp_cmd"]
         self.volume_name = self.config["netapp_volume_name"]
         volume_info = await self.netapp_client.get_volume_by_name(self.volume_name, ["svm"])
         assert "svm" in volume_info
         self.volume_id = volume_info["uuid"]
```

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/netapp/netappclient.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/netapp/netappclient.py`

 * *Files 5% similar despite different names*

```diff
@@ -120,25 +120,31 @@
     pass
 
 
 class NetAppClient:
     endpoint: str
     user: str
     password: str
+    user_id: int
+    group_id: int
     _session: aiohttp.ClientSession
 
     def __init__(
         self,
         endpoint: str,
         user: str,
         password: str,
+        user_id: int,
+        group_id: int,
     ) -> None:
         self.endpoint = endpoint
         self.user = user
         self.password = password
+        self.user_id = user_id
+        self.group_id = group_id
         _connector = aiohttp.TCPConnector(ssl=False)
         _auth = aiohttp.BasicAuth(self.user, self.password)
         self._session = aiohttp.ClientSession(
             self.endpoint,
             connector=_connector,
             auth=_auth,
             # raise_for_status=True,
@@ -410,14 +416,16 @@
         async with self.send_request(
             "post",
             "/api/storage/qtrees",
             data={
                 "svm.uuid": str(svm_id),
                 "volume.uuid": str(volume_id),
                 "name": qtree_name,
+                "user.id": self.user_id,
+                "group.id": self.group_id,
             },
         ) as resp:
             data = await resp.json()
         return await self.wait_job(data["job"]["uuid"])
 
     async def set_quota_rule(
         self,
@@ -468,14 +476,39 @@
             records = data["records"]
             if data["num_records"] == 0:
                 raise NetAppClientError(
                     f"Quota rule not found for the volume {volume_id} and the qtree {qtree_name}"
                 )
             return records[0]
 
+    async def update_quota_rule(
+        self,
+        svm_id: StorageID,
+        volume_id: VolumeID,
+        qtree_name: str,
+        config: QuotaConfig,
+    ) -> AsyncJobResult:
+        record = await self._find_quota_rule(svm_id, volume_id, qtree_name)
+        async with self.send_request(
+            "patch",
+            f"/api/storage/quota/rules/{record['uuid']}",
+            data={
+                "space": {
+                    "hard_limit": config.limit_bytes,
+                    "soft_limit": config.limit_bytes,
+                },
+                # 'files': {  # not supported yet from Backend.AI
+                #     'hard_limit': 0,
+                #     'soft_limit': 0,
+                # },
+            },
+        ) as resp:
+            data = await resp.json()
+        return await self.wait_job(data["job"]["uuid"])
+
     async def get_quota_rule(
         self,
         svm_id: StorageID,
         volume_id: VolumeID,
         qtree_name: str,
     ) -> QuotaConfig:
         record = await self._find_quota_rule(svm_id, volume_id, qtree_name)
```

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/plugin.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/plugin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/purestorage/__init__.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/purestorage/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/purestorage/purity.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/purestorage/purity.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/server.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/server.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/subproc.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/subproc.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/types.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/utils.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/vast/__init__.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/vast/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/vast/config.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/vast/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/vast/exceptions.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/vast/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/vast/vastdata_client.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/vast/vastdata_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/vfs/__init__.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/vfs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/watcher.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/watcher.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/weka/__init__.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/weka/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/weka/exceptions.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/weka/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/weka/weka_client.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/weka/weka_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/ai/backend/storage/xfs/__init__.py` & `backend.ai-storage-proxy-24.3.0rc3/ai/backend/storage/xfs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/backend.ai_storage_proxy.egg-info/PKG-INFO` & `backend.ai-storage-proxy-24.3.0rc3/backend.ai_storage_proxy.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-storage-proxy
-Version: 24.3.0rc2
+Version: 24.3.0rc3
 Summary: Backend.AI Storage Proxy
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -12,18 +12,41 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Requires-Python: >=3.11,<3.12
+Requires-Python: >=3.12,<3.13
 Description-Content-Type: text/markdown
+Requires-Dist: PyJWT~=2.0
+Requires-Dist: aiofiles~=0.8.0
+Requires-Dist: aiohttp_cors~=0.7
+Requires-Dist: aiohttp~=3.9.1
+Requires-Dist: aiomonitor~=0.7.0
+Requires-Dist: aiotools~=1.7.0
+Requires-Dist: asyncpg>=0.27.0
+Requires-Dist: attrs>=20.3
+Requires-Dist: backend.ai-common==24.03.0rc3
+Requires-Dist: backend.ai-plugin==24.03.0rc3
+Requires-Dist: click~=8.1.7
+Requires-Dist: dataclasses-json~=0.5.7
+Requires-Dist: janus~=1.0.0
+Requires-Dist: more-itertools~=8.13.0
+Requires-Dist: pyzmq~=25.1.2
+Requires-Dist: setproctitle~=1.3.2
+Requires-Dist: tenacity>=8.0
+Requires-Dist: tqdm>=4.61
+Requires-Dist: trafaret~=2.1
+Requires-Dist: types-aiofiles
+Requires-Dist: uvloop~=0.19.0; sys_platform != "Windows"
+Requires-Dist: yarl!=1.9.0,!=1.9.1,!=1.9.2,<2.0,>=1.8.2
+Requires-Dist: zipstream-new~=1.1.8
 
 # Backend.AI Storage Proxy
 
 Backend.AI Storage Proxy is an RPC daemon to manage vfolders used in Backend.AI agent, with quota and
 storage-specific optimization support.
 
 ## Package Structure
```

### Comparing `backend.ai-storage-proxy-24.3.0rc2/backend.ai_storage_proxy.egg-info/SOURCES.txt` & `backend.ai-storage-proxy-24.3.0rc3/backend.ai_storage_proxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/backend_shim.py` & `backend.ai-storage-proxy-24.3.0rc3/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-24.3.0rc2/setup.py` & `backend.ai-storage-proxy-24.3.0rc3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Environment :: No Input/Output (Daemon)',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development',
         'Development Status :: 4 - Beta',
-        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)',
     ],
     'description': 'Backend.AI Storage Proxy',
     'entry_points': {
         'backendai_cli_v10': [
             'storage = ai.backend.storage.cli:main',
             'storage.start-server = ai.backend.storage.server:main',
@@ -31,29 +31,29 @@
         'aiofiles~=0.8.0',
         'aiohttp_cors~=0.7',
         'aiohttp~=3.9.1',
         'aiomonitor~=0.7.0',
         'aiotools~=1.7.0',
         'asyncpg>=0.27.0',
         'attrs>=20.3',
-        """backend.ai-common==24.03.0rc2
+        """backend.ai-common==24.03.0rc3
 """,
-        """backend.ai-plugin==24.03.0rc2
+        """backend.ai-plugin==24.03.0rc3
 """,
         'click~=8.1.7',
         'dataclasses-json~=0.5.7',
         'janus~=1.0.0',
         'more-itertools~=8.13.0',
         'pyzmq~=25.1.2',
         'setproctitle~=1.3.2',
         'tenacity>=8.0',
         'tqdm>=4.61',
         'trafaret~=2.1',
         'types-aiofiles',
-        'uvloop~=0.17.0; sys_platform != "Windows"',
+        'uvloop~=0.19.0; sys_platform != "Windows"',
         'yarl!=1.9.0,!=1.9.1,!=1.9.2,<2.0,>=1.8.2',
         'zipstream-new~=1.1.8',
     ),
     'license': 'LGPLv3',
     'long_description': """# Backend.AI Storage Proxy
 
 Backend.AI Storage Proxy is an RPC daemon to manage vfolders used in Backend.AI agent, with quota and
@@ -258,13 +258,13 @@
         'ai.backend.storage.weka',
         'ai.backend.storage.xfs',
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
-    'python_requires': '>=3.11,<3.12',
+    'python_requires': '>=3.12,<3.13',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """24.03.0rc2
+    'version': """24.03.0rc3
 """,
     'zip_safe': False,
 })
```

