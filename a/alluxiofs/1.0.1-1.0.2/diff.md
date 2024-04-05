# Comparing `tmp/alluxiofs-1.0.1.tar.gz` & `tmp/alluxiofs-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alluxiofs-1.0.1.tar", last modified: Wed Mar 27 20:03:38 2024, max compression
+gzip compressed data, was "alluxiofs-1.0.2.tar", last modified: Fri Apr  5 21:33:28 2024, max compression
```

## Comparing `alluxiofs-1.0.1.tar` & `alluxiofs-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 siyuansheng   (501) staff       (20)        0 2024-03-27 20:03:38.082570 alluxiofs-1.0.1/
--rw-r--r--   0 siyuansheng   (501) staff       (20)    27039 2024-03-09 00:16:21.000000 alluxiofs-1.0.1/LICENSE
--rw-r--r--   0 siyuansheng   (501) staff       (20)      657 2024-03-27 20:03:38.082264 alluxiofs-1.0.1/PKG-INFO
--rw-r--r--   0 siyuansheng   (501) staff       (20)     5368 2024-03-13 21:08:16.000000 alluxiofs-1.0.1/README.md
-drwxr-xr-x   0 siyuansheng   (501) staff       (20)        0 2024-03-27 20:03:38.073277 alluxiofs-1.0.1/alluxiofs/
--rw-r--r--   0 siyuansheng   (501) staff       (20)      138 2024-03-09 00:16:21.000000 alluxiofs-1.0.1/alluxiofs/__init__.py
-drwxr-xr-x   0 siyuansheng   (501) staff       (20)        0 2024-03-27 20:03:38.079982 alluxiofs-1.0.1/alluxiofs/client/
--rw-r--r--   0 siyuansheng   (501) staff       (20)      248 2024-03-09 00:16:21.000000 alluxiofs-1.0.1/alluxiofs/client/__init__.py
--rw-r--r--   0 siyuansheng   (501) staff       (20)     1610 2024-03-09 00:16:21.000000 alluxiofs-1.0.1/alluxiofs/client/const.py
--rw-r--r--   0 siyuansheng   (501) staff       (20)    45024 2024-03-14 23:07:14.000000 alluxiofs-1.0.1/alluxiofs/client/core.py
--rw-r--r--   0 siyuansheng   (501) staff       (20)    14570 2024-03-09 00:16:21.000000 alluxiofs-1.0.1/alluxiofs/client/worker_ring.py
--rw-r--r--   0 siyuansheng   (501) staff       (20)    12682 2024-03-27 20:01:28.000000 alluxiofs-1.0.1/alluxiofs/core.py
-drwxr-xr-x   0 siyuansheng   (501) staff       (20)        0 2024-03-27 20:03:38.080872 alluxiofs-1.0.1/alluxiofs.egg-info/
--rw-r--r--   0 siyuansheng   (501) staff       (20)      657 2024-03-27 20:03:38.000000 alluxiofs-1.0.1/alluxiofs.egg-info/PKG-INFO
--rw-r--r--   0 siyuansheng   (501) staff       (20)      420 2024-03-27 20:03:38.000000 alluxiofs-1.0.1/alluxiofs.egg-info/SOURCES.txt
--rw-r--r--   0 siyuansheng   (501) staff       (20)        1 2024-03-27 20:03:38.000000 alluxiofs-1.0.1/alluxiofs.egg-info/dependency_links.txt
--rw-r--r--   0 siyuansheng   (501) staff       (20)       53 2024-03-27 20:03:38.000000 alluxiofs-1.0.1/alluxiofs.egg-info/entry_points.txt
--rw-r--r--   0 siyuansheng   (501) staff       (20)        1 2024-02-27 23:45:11.000000 alluxiofs-1.0.1/alluxiofs.egg-info/not-zip-safe
--rw-r--r--   0 siyuansheng   (501) staff       (20)      136 2024-03-27 20:03:38.000000 alluxiofs-1.0.1/alluxiofs.egg-info/requires.txt
--rw-r--r--   0 siyuansheng   (501) staff       (20)       10 2024-03-27 20:03:38.000000 alluxiofs-1.0.1/alluxiofs.egg-info/top_level.txt
--rw-r--r--   0 siyuansheng   (501) staff       (20)      164 2024-03-27 20:03:38.083609 alluxiofs-1.0.1/setup.cfg
--rw-r--r--   0 siyuansheng   (501) staff       (20)      999 2024-03-27 20:03:12.000000 alluxiofs-1.0.1/setup.py
+drwxr-xr-x   0 siyuansheng   (501) staff       (20)        0 2024-04-05 21:33:28.558352 alluxiofs-1.0.2/
+-rw-r--r--   0 siyuansheng   (501) staff       (20)    27039 2024-03-09 00:16:21.000000 alluxiofs-1.0.2/LICENSE
+-rw-r--r--   0 siyuansheng   (501) staff       (20)      657 2024-04-05 21:33:28.558119 alluxiofs-1.0.2/PKG-INFO
+-rw-r--r--   0 siyuansheng   (501) staff       (20)     5368 2024-03-13 21:08:16.000000 alluxiofs-1.0.2/README.md
+drwxr-xr-x   0 siyuansheng   (501) staff       (20)        0 2024-04-05 21:33:28.548776 alluxiofs-1.0.2/alluxiofs/
+-rw-r--r--   0 siyuansheng   (501) staff       (20)      138 2024-03-09 00:16:21.000000 alluxiofs-1.0.2/alluxiofs/__init__.py
+drwxr-xr-x   0 siyuansheng   (501) staff       (20)        0 2024-04-05 21:33:28.555713 alluxiofs-1.0.2/alluxiofs/client/
+-rw-r--r--   0 siyuansheng   (501) staff       (20)      248 2024-03-09 00:16:21.000000 alluxiofs-1.0.2/alluxiofs/client/__init__.py
+-rw-r--r--   0 siyuansheng   (501) staff       (20)     1732 2024-04-05 21:32:18.000000 alluxiofs-1.0.2/alluxiofs/client/const.py
+-rw-r--r--   0 siyuansheng   (501) staff       (20)    45396 2024-04-05 21:32:18.000000 alluxiofs-1.0.2/alluxiofs/client/core.py
+-rw-r--r--   0 siyuansheng   (501) staff       (20)    14570 2024-03-09 00:16:21.000000 alluxiofs-1.0.2/alluxiofs/client/worker_ring.py
+-rw-r--r--   0 siyuansheng   (501) staff       (20)    12587 2024-04-05 21:18:26.000000 alluxiofs-1.0.2/alluxiofs/core.py
+drwxr-xr-x   0 siyuansheng   (501) staff       (20)        0 2024-04-05 21:33:28.556935 alluxiofs-1.0.2/alluxiofs.egg-info/
+-rw-r--r--   0 siyuansheng   (501) staff       (20)      657 2024-04-05 21:33:28.000000 alluxiofs-1.0.2/alluxiofs.egg-info/PKG-INFO
+-rw-r--r--   0 siyuansheng   (501) staff       (20)      420 2024-04-05 21:33:28.000000 alluxiofs-1.0.2/alluxiofs.egg-info/SOURCES.txt
+-rw-r--r--   0 siyuansheng   (501) staff       (20)        1 2024-04-05 21:33:28.000000 alluxiofs-1.0.2/alluxiofs.egg-info/dependency_links.txt
+-rw-r--r--   0 siyuansheng   (501) staff       (20)       53 2024-04-05 21:33:28.000000 alluxiofs-1.0.2/alluxiofs.egg-info/entry_points.txt
+-rw-r--r--   0 siyuansheng   (501) staff       (20)        1 2024-02-27 23:45:11.000000 alluxiofs-1.0.2/alluxiofs.egg-info/not-zip-safe
+-rw-r--r--   0 siyuansheng   (501) staff       (20)      136 2024-04-05 21:33:28.000000 alluxiofs-1.0.2/alluxiofs.egg-info/requires.txt
+-rw-r--r--   0 siyuansheng   (501) staff       (20)       10 2024-04-05 21:33:28.000000 alluxiofs-1.0.2/alluxiofs.egg-info/top_level.txt
+-rw-r--r--   0 siyuansheng   (501) staff       (20)      164 2024-04-05 21:33:28.559398 alluxiofs-1.0.2/setup.cfg
+-rw-r--r--   0 siyuansheng   (501) staff       (20)      999 2024-04-05 21:33:08.000000 alluxiofs-1.0.2/setup.py
```

### Comparing `alluxiofs-1.0.1/LICENSE` & `alluxiofs-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alluxiofs-1.0.1/PKG-INFO` & `alluxiofs-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alluxiofs
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alluxio Fsspec provides Alluxio filesystem spec implementation.
 Home-page: https://github.com/fsspec/alluxiofs
 Maintainer: Lu Qiu
 Maintainer-email: luqiujob@gmail.com
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: fsspec
```

### Comparing `alluxiofs-1.0.1/README.md` & `alluxiofs-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alluxiofs-1.0.1/alluxiofs/client/const.py` & `alluxiofs-1.0.2/alluxiofs/client/const.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 ALLUXIO_CLUSTER_NAME_KEY = "alluxio.cluster.name"
 ALLUXIO_CLUSTER_NAME_DEFAULT_VALUE = "DefaultAlluxioCluster"
 ALLUXIO_ETCD_USERNAME_KEY = "alluxio.etcd.username"
 ALLUXIO_ETCD_PASSWORD_KEY = "alluxio.etcd.password"
 ALLUXIO_PAGE_SIZE_KEY = "alluxio.worker.page.store.page.size"
 ALLUXIO_PAGE_SIZE_DEFAULT_VALUE = "1MB"
-ALLUXIO_HASH_NODE_PER_WORKER_KEY = (
+ALLUXIO_HASH_NODE_PER_WORKER_KEY1 = (
     "alluxio.user.consistent.hash.virtual.node.count.per.worker"
 )
+ALLUXIO_HASH_NODE_PER_WORKER_KEY2 = "alluxio.user.worker.selection.policy.consistent.hash.virtual.node.count.per.worker"
 ALLUXIO_WORKER_HTTP_SERVER_PORT_KEY = "alluxio.worker.http.server.port"
 ALLUXIO_WORKER_HTTP_SERVER_PORT_DEFAULT_VALUE = 28080
 ALLUXIO_HASH_NODE_PER_WORKER_DEFAULT_VALUE = 5
 ALLUXIO_SUCCESS_IDENTIFIER = "success"
 LIST_URL_FORMAT = "http://{worker_host}:{http_port}/v1/files"
 FULL_PAGE_URL_FORMAT = (
     "http://{worker_host}:{http_port}/v1/file/{path_id}/page/{page_index}"
```

### Comparing `alluxiofs-1.0.1/alluxiofs/client/core.py` & `alluxiofs-1.0.2/alluxiofs/client/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 
 import aiohttp
 import humanfriendly
 import requests
 from requests.adapters import HTTPAdapter
 
 from .const import ALLUXIO_HASH_NODE_PER_WORKER_DEFAULT_VALUE
-from .const import ALLUXIO_HASH_NODE_PER_WORKER_KEY
+from .const import ALLUXIO_HASH_NODE_PER_WORKER_KEY1
+from .const import ALLUXIO_HASH_NODE_PER_WORKER_KEY2
 from .const import ALLUXIO_PAGE_SIZE_DEFAULT_VALUE
 from .const import ALLUXIO_PAGE_SIZE_KEY
 from .const import ALLUXIO_SUCCESS_IDENTIFIER
 from .const import ALLUXIO_WORKER_HTTP_SERVER_PORT_DEFAULT_VALUE
 from .const import FULL_PAGE_URL_FORMAT
 from .const import GET_FILE_STATUS_URL_FORMAT
 from .const import LIST_URL_FORMAT
@@ -176,17 +177,24 @@
         # parse options
         page_size = ALLUXIO_PAGE_SIZE_DEFAULT_VALUE
         hash_node_per_worker = ALLUXIO_HASH_NODE_PER_WORKER_DEFAULT_VALUE
         if options:
             if ALLUXIO_PAGE_SIZE_KEY in options:
                 page_size = options[ALLUXIO_PAGE_SIZE_KEY]
                 self.logger.debug(f"Page size is set to {page_size}")
-            if ALLUXIO_HASH_NODE_PER_WORKER_KEY in options:
+            if ALLUXIO_HASH_NODE_PER_WORKER_KEY1 in options:
                 hash_node_per_worker = int(
-                    options[ALLUXIO_HASH_NODE_PER_WORKER_KEY]
+                    options[ALLUXIO_HASH_NODE_PER_WORKER_KEY1]
+                )
+                self.logger.debug(
+                    f"Hash node per worker is set to {hash_node_per_worker}"
+                )
+            if ALLUXIO_HASH_NODE_PER_WORKER_KEY2 in options:
+                hash_node_per_worker = int(
+                    options[ALLUXIO_HASH_NODE_PER_WORKER_KEY2]
                 )
                 self.logger.debug(
                     f"Hash node per worker is set to {hash_node_per_worker}"
                 )
         if (
             not isinstance(hash_node_per_worker, int)
             or hash_node_per_worker <= 0
```

### Comparing `alluxiofs-1.0.1/alluxiofs/client/worker_ring.py` & `alluxiofs-1.0.2/alluxiofs/client/worker_ring.py`

 * *Files identical despite different names*

### Comparing `alluxiofs-1.0.1/alluxiofs.egg-info/PKG-INFO` & `alluxiofs-1.0.2/alluxiofs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alluxiofs
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alluxio Fsspec provides Alluxio filesystem spec implementation.
 Home-page: https://github.com/fsspec/alluxiofs
 Maintainer: Lu Qiu
 Maintainer-email: luqiujob@gmail.com
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: fsspec
```

### Comparing `alluxiofs-1.0.1/setup.py` & `alluxiofs-1.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="alluxiofs",
-    version="1.0.1",
+    version="1.0.2",
     description="Alluxio Fsspec provides Alluxio filesystem spec implementation.",
     url="https://github.com/fsspec/alluxiofs",
     packages=find_packages(exclude=["tests", "tests.*"]),
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         # Alluxio fs dependencies
```

