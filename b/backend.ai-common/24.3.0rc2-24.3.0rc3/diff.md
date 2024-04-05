# Comparing `tmp/backend.ai-common-24.3.0rc2.tar.gz` & `tmp/backend.ai-common-24.3.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-common-24.3.0rc2.tar", last modified: Sun Mar 31 14:09:10 2024, max compression
+gzip compressed data, was "backend.ai-common-24.3.0rc3.tar", last modified: Fri Apr  5 02:25:36 2024, max compression
```

## Comparing `backend.ai-common-24.3.0rc2.tar` & `backend.ai-common-24.3.0rc3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.391435 backend.ai-common-24.3.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-03-31 14:09:10.391435 backend.ai-common-24.3.0rc2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.383435 backend.ai-common-24.3.0rc2/ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.383435 backend.ai-common-24.3.0rc2/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.391435 backend.ai-common-24.3.0rc2/ai/backend/common/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/arch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/asyncio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.391435 backend.ai-common-24.3.0rc2/ai/backend/common/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11083 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/bgtask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/cgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)    21189 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/enum_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/enum_extension.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19833 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/etcd.py
--rw-r--r--   0 runner    (1001) docker     (127)    33020 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     7968 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)    22559 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/logging_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.383435 backend.ai-common-24.3.0rc2/ai/backend/common/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.391435 backend.ai-common-24.3.0rc2/ai/backend/common/models/minilang/
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/models/minilang/mount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/msgpack.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/netns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/networking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.391435 backend.ai-common-24.3.0rc2/ai/backend/common/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5646 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/plugin/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/plugin/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/plugin/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    18454 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/redis_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/sd_notify.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/service_ports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/testutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/typed_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)    37619 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25246 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.383435 backend.ai-common-24.3.0rc2/ai/backend/common/web/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.391435 backend.ai-common-24.3.0rc2/ai/backend/common/web/session/
--rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/web/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/ai/backend/common/web/session/redis_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.391435 backend.ai-common-24.3.0rc2/backend.ai_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-03-31 14:09:10.000000 backend.ai-common-24.3.0rc2/backend.ai_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-03-31 14:09:10.000000 backend.ai-common-24.3.0rc2/backend.ai_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:09:10.000000 backend.ai-common-24.3.0rc2/backend.ai_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:09:10.000000 backend.ai-common-24.3.0rc2/backend.ai_common.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:09:10.000000 backend.ai-common-24.3.0rc2/backend.ai_common.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-31 14:09:10.000000 backend.ai-common-24.3.0rc2/backend.ai_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-03-31 14:09:10.000000 backend.ai-common-24.3.0rc2/backend.ai_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 14:09:10.391435 backend.ai-common-24.3.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-03-31 14:09:09.000000 backend.ai-common-24.3.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.734037 backend.ai-common-24.3.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-05 02:25:36.730037 backend.ai-common-24.3.0rc3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.718037 backend.ai-common-24.3.0rc3/ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.718037 backend.ai-common-24.3.0rc3/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.730037 backend.ai-common-24.3.0rc3/ai/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/arch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/asyncio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.730037 backend.ai-common-24.3.0rc3/ai/backend/common/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/bgtask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/cgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21291 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/enum_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/enum_extension.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19833 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33020 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7968 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22559 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/logging_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.718037 backend.ai-common-24.3.0rc3/ai/backend/common/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.730037 backend.ai-common-24.3.0rc3/ai/backend/common/models/minilang/
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/models/minilang/mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/netns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/networking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.730037 backend.ai-common-24.3.0rc3/ai/backend/common/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5646 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/plugin/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/plugin/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/plugin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18454 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/redis_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/sd_notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/service_ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/typed_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37619 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25246 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.722037 backend.ai-common-24.3.0rc3/ai/backend/common/web/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.730037 backend.ai-common-24.3.0rc3/ai/backend/common/web/session/
+-rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/web/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/ai/backend/common/web/session/redis_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.730037 backend.ai-common-24.3.0rc3/backend.ai_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/backend.ai_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/backend.ai_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/backend.ai_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/backend.ai_common.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/backend.ai_common.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/backend.ai_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/backend.ai_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 02:25:36.734037 backend.ai-common-24.3.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-05 02:25:36.000000 backend.ai-common-24.3.0rc3/setup.py
```

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/argparse.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/argparse.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/asyncio.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/asyncio.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/auth/__init__.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/bgtask.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/bgtask.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import json
 import logging
 import time
 import uuid
 import weakref
 from collections import defaultdict
 from typing import (
+    Any,
+    AsyncIterator,
     Awaitable,
     Callable,
     DefaultDict,
     Final,
     Literal,
     Set,
     Type,
@@ -140,76 +142,90 @@
         request: web.Request,
         task_id: uuid.UUID,
     ) -> web.StreamResponse:
         """
         A aiohttp-based server-sent events (SSE) responder that pushes the bgtask updates
         to the clients.
         """
+        async with sse_response(request) as resp:
+            try:
+                async for event, extra_data in self.poll_bgtask_event(task_id):
+                    body: dict[str, Any] = {
+                        "task_id": str(event.task_id),
+                        "message": event.message,
+                    }
+                    match event:
+                        case BgtaskUpdatedEvent():
+                            body["current_progress"] = event.current_progress
+                            body["total_progress"] = event.total_progress
+                            await resp.send(json.dumps(body), event=event.name, retry=5)
+                        case BgtaskDoneEvent():
+                            if extra_data:
+                                body.update(extra_data)
+                                await resp.send(
+                                    json.dumps(body), event="bgtask_" + extra_data["status"]
+                                )
+                            else:
+                                await resp.send("{}", event="bgtask_done")
+                            await resp.send("{}", event="server_close")
+                        case BgtaskCancelledEvent() | BgtaskFailedEvent():
+                            await resp.send("{}", event="server_close")
+            except:
+                log.exception("")
+                raise
+            finally:
+                return resp
+
+    async def poll_bgtask_event(
+        self,
+        task_id: uuid.UUID,
+    ) -> AsyncIterator[tuple[BgtaskEvents, dict]]:
+        """
+        RHS of return tuple will be filled with extra informations when needed
+        (e.g. progress information of task when callee is trying to poll information of already completed one)
+        """
         tracker_key = f"bgtask.{task_id}"
         redis_producer = self.event_producer.redis_client
         task_info = await redis_helper.execute(
             redis_producer,
             lambda r: r.hgetall(tracker_key),
             encoding="utf-8",
         )
 
-        log.debug("task info: {}", task_info)
         if task_info is None:
             # The task ID is invalid or represents a task completed more than 24 hours ago.
             raise ValueError("No such background task.")
 
         if task_info["status"] != "started":
             # It is an already finished task!
-            async with sse_response(request) as resp:
-                try:
-                    body = {
-                        "task_id": str(task_id),
-                        "status": task_info["status"],
-                        "current_progress": task_info["current"],
-                        "total_progress": task_info["total"],
-                        "message": task_info["msg"],
-                    }
-                    await resp.send(json.dumps(body), event="bgtask_" + task_info["status"])
-                finally:
-                    await resp.send("{}", event="server_close")
-            return resp
+            yield (
+                BgtaskDoneEvent(task_id, message=task_info["msg"]),
+                {
+                    "status": task_info["status"],
+                    "current_progress": task_info["current"],
+                    "total_progress": task_info["total"],
+                },
+            )
+            return
 
         # It is an ongoing task.
         my_queue: asyncio.Queue[BgtaskEvents | Sentinel] = asyncio.Queue()
         async with self.dict_lock:
             self.task_update_queues[task_id].add(my_queue)
         try:
-            async with sse_response(request) as resp:
+            while True:
+                event = await my_queue.get()
                 try:
-                    while True:
-                        event = await my_queue.get()
-                        try:
-                            if event is sentinel:
-                                break
-                            if task_id != event.task_id:
-                                continue
-                            body = {
-                                "task_id": str(task_id),
-                                "message": event.message,
-                            }
-                            if isinstance(event, BgtaskUpdatedEvent):
-                                body["current_progress"] = event.current_progress
-                                body["total_progress"] = event.total_progress
-                            await resp.send(json.dumps(body), event=event.name, retry=5)
-                            if (
-                                isinstance(event, BgtaskDoneEvent)
-                                or isinstance(event, BgtaskFailedEvent)
-                                or isinstance(event, BgtaskCancelledEvent)
-                            ):
-                                await resp.send("{}", event="server_close")
-                                break
-                        finally:
-                            my_queue.task_done()
+                    if event is sentinel:
+                        break
+                    if task_id != event.task_id:
+                        continue
+                    yield event, {}
                 finally:
-                    return resp
+                    my_queue.task_done()
         finally:
             self.task_update_queues[task_id].remove(my_queue)
             async with self.dict_lock:
                 if len(self.task_update_queues[task_id]) == 0:
                     del self.task_update_queues[task_id]
 
     async def start(
```

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/cgroup.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/cgroup.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/cli.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/cli.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/config.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/distributed.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/distributed.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/docker.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -354,15 +354,15 @@
             pass
     return common_labels
 
 
 class PlatformTagSet(Mapping):
     __slots__ = ("_data",)
     _data: dict[str, str]
-    _rx_ver = re.compile(r"^(?P<tag>[a-zA-Z]+)(?P<version>\d+(?:\.\d+)*[a-z0-9]*)?$")
+    _rx_ver = re.compile(r"^(?P<tag>[a-zA-Z_]+)(?P<version>\d+(?:\.\d+)*[a-z0-9]*)?$")
 
     def __init__(self, tags: Iterable[str], value: str = None) -> None:
         self._data = dict()
         rx = type(self)._rx_ver
         for tag in tags:
             match = rx.search(tag)
             if match is None:
@@ -399,14 +399,22 @@
 class ImageRef:
     """
     Class to represent image reference.
     passing ['*'] to `known_registries` when creating object
     will allow any repository on canonical string.
     """
 
+    _value: str
+    _is_local: bool
+    _arch: str
+    _registry: str
+
+    _name: str
+    _tag: str
+
     __slots__ = ("_registry", "_name", "_tag", "_arch", "_tag_set", "_sha", "_is_local", "_value")
 
     _rx_slug = re.compile(r"^[A-Za-z0-9](?:[A-Za-z0-9-._]*[A-Za-z0-9])?$")
 
     def __init__(
         self,
         value: str,
```

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/enum_extension.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/enum_extension.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/enum_extension.pyi` & `backend.ai-common-24.3.0rc3/ai/backend/common/enum_extension.pyi`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/etcd.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/events.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/events.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/exception.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/exception.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/files.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/files.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/identity.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/identity.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/lock.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/lock.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/logging.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/logging.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/logging_utils.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/logging_utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/models/minilang/mount.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/models/minilang/mount.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/msgpack.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/msgpack.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/netns.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/netns.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/networking.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/networking.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/plugin/__init__.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/plugin/hook.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/plugin/hook.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/plugin/monitor.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/plugin/monitor.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/redis_helper.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/redis_helper.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/sd_notify.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/sd_notify.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/service_ports.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/service_ports.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/testutils.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/testutils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/typed_validators.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/typed_validators.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/types.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/utils.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/validators.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/validators.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/web/session/__init__.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/web/session/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/ai/backend/common/web/session/redis_storage.py` & `backend.ai-common-24.3.0rc3/ai/backend/common/web/session/redis_storage.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/backend.ai_common.egg-info/SOURCES.txt` & `backend.ai-common-24.3.0rc3/backend.ai_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/backend.ai_common.egg-info/requires.txt` & `backend.ai-common-24.3.0rc3/backend.ai_common.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 aiohttp~=3.9.1
 aiomonitor~=0.7.0
 aiotools~=1.7.0
 async_timeout~=4.0
 asynctest>=0.13.0
 asyncudp>=0.4
 attrs>=20.3
-backend.ai-plugin==24.03.0rc2
+backend.ai-plugin==24.03.0rc3
 callosum~=1.0.3
 click~=8.1.7
 coloredlogs~=15.0
 etcd-client-py==0.2.4
 graypy==2.1.0
 ifaddr~=0.2
 janus~=1.0.0
```

### Comparing `backend.ai-common-24.3.0rc2/backend_shim.py` & `backend.ai-common-24.3.0rc3/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc2/setup.py` & `backend.ai-common-24.3.0rc3/setup.py`

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
     'description': 'Backend.AI commons library',
     'install_requires': (
         'PyJWT~=2.0',
         'aiodns>=3.0',
         'aiofiles~=0.8.0',
@@ -28,15 +28,15 @@
         'aiohttp~=3.9.1',
         'aiomonitor~=0.7.0',
         'aiotools~=1.7.0',
         'async_timeout~=4.0',
         'asynctest>=0.13.0',
         'asyncudp>=0.4',
         'attrs>=20.3',
-        """backend.ai-plugin==24.03.0rc2
+        """backend.ai-plugin==24.03.0rc3
 """,
         'callosum~=1.0.3',
         'click~=8.1.7',
         'coloredlogs~=15.0',
         'etcd-client-py==0.2.4',
         'graypy==2.1.0',
         'ifaddr~=0.2',
@@ -125,13 +125,13 @@
         'ai.backend.common.plugin',
         'ai.backend.common.web.session',
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

