# Comparing `tmp/fastapi-requests-limit-0.1.5.tar.gz` & `tmp/fastapi-requests-limit-0.1.5b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-requests-limit-0.1.5.tar", last modified: Fri Apr  5 20:20:04 2024, max compression
+gzip compressed data, was "fastapi-requests-limit-0.1.5b1.tar", last modified: Wed Apr  3 22:30:10 2024, max compression
```

## Comparing `fastapi-requests-limit-0.1.5.tar` & `fastapi-requests-limit-0.1.5b1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 20:20:04.556407 fastapi-requests-limit-0.1.5/
--rw-rw-rw-   0        0        0     1106 2024-03-21 23:13:37.000000 fastapi-requests-limit-0.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0     4120 2024-04-05 20:20:04.556407 fastapi-requests-limit-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     3126 2024-04-02 21:58:23.000000 fastapi-requests-limit-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 20:20:04.485395 fastapi-requests-limit-0.1.5/fastapi_requests_limit/
--rw-rw-rw-   0        0        0        0 2023-10-17 00:43:53.000000 fastapi-requests-limit-0.1.5/fastapi_requests_limit/__init__.py
--rw-rw-rw-   0        0        0      866 2024-04-02 21:33:31.000000 fastapi-requests-limit-0.1.5/fastapi_requests_limit/configuration.py
--rw-rw-rw-   0        0        0      538 2024-04-02 20:00:53.000000 fastapi-requests-limit-0.1.5/fastapi_requests_limit/handle_errors.py
--rw-rw-rw-   0        0        0     2162 2024-04-02 20:00:54.000000 fastapi-requests-limit-0.1.5/fastapi_requests_limit/limiter_rest.py
--rw-rw-rw-   0        0        0      390 2024-04-02 21:33:31.000000 fastapi-requests-limit-0.1.5/fastapi_requests_limit/storage_engines.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:20:04.525995 fastapi-requests-limit-0.1.5/fastapi_requests_limit/storages/
--rw-rw-rw-   0        0        0        0 2023-10-19 02:31:00.000000 fastapi-requests-limit-0.1.5/fastapi_requests_limit/storages/__init__.py
--rw-rw-rw-   0        0        0      771 2024-04-02 20:00:54.000000 fastapi-requests-limit-0.1.5/fastapi_requests_limit/storages/memory.py
--rw-rw-rw-   0        0        0        0 2023-10-19 02:31:30.000000 fastapi-requests-limit-0.1.5/fastapi_requests_limit/storages/mondodb.py
--rw-rw-rw-   0        0        0      897 2024-04-02 20:00:53.000000 fastapi-requests-limit-0.1.5/fastapi_requests_limit/storages/redis.py
--rw-rw-rw-   0        0        0      589 2024-04-02 20:03:20.000000 fastapi-requests-limit-0.1.5/fastapi_requests_limit/storages/storage.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:20:04.555374 fastapi-requests-limit-0.1.5/fastapi_requests_limit/test/
--rw-rw-rw-   0        0        0        0 2023-11-09 21:24:25.000000 fastapi-requests-limit-0.1.5/fastapi_requests_limit/test/__init__.py
--rw-rw-rw-   0        0        0      282 2023-11-17 23:12:25.000000 fastapi-requests-limit-0.1.5/fastapi_requests_limit/test/mock.py
--rw-rw-rw-   0        0        0      420 2024-04-02 20:03:32.000000 fastapi-requests-limit-0.1.5/fastapi_requests_limit/test/test.py
--rw-rw-rw-   0        0        0       33 2023-11-17 16:42:06.000000 fastapi-requests-limit-0.1.5/fastapi_requests_limit/test/test_constans.py
--rw-rw-rw-   0        0        0     1517 2024-04-02 21:06:26.000000 fastapi-requests-limit-0.1.5/fastapi_requests_limit/test/test_limiter_memory.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:20:04.504775 fastapi-requests-limit-0.1.5/fastapi_requests_limit.egg-info/
--rw-rw-rw-   0        0        0     4120 2024-04-05 20:20:04.000000 fastapi-requests-limit-0.1.5/fastapi_requests_limit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      876 2024-04-05 20:20:04.000000 fastapi-requests-limit-0.1.5/fastapi_requests_limit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 20:20:04.000000 fastapi-requests-limit-0.1.5/fastapi_requests_limit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-05 20:20:04.000000 fastapi-requests-limit-0.1.5/fastapi_requests_limit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-04-05 20:20:04.000000 fastapi-requests-limit-0.1.5/fastapi_requests_limit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 20:20:04.556407 fastapi-requests-limit-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1302 2024-04-05 20:19:57.000000 fastapi-requests-limit-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:30:10.993750 fastapi-requests-limit-0.1.5b1/
+-rw-rw-rw-   0        0        0     1106 2024-03-21 23:13:37.000000 fastapi-requests-limit-0.1.5b1/LICENSE.txt
+-rw-rw-rw-   0        0        0     4122 2024-04-03 22:30:10.992745 fastapi-requests-limit-0.1.5b1/PKG-INFO
+-rw-rw-rw-   0        0        0     3126 2024-04-02 21:58:23.000000 fastapi-requests-limit-0.1.5b1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 22:30:10.933145 fastapi-requests-limit-0.1.5b1/fastapi_requests_limit/
+-rw-rw-rw-   0        0        0        0 2023-10-17 00:43:53.000000 fastapi-requests-limit-0.1.5b1/fastapi_requests_limit/__init__.py
+-rw-rw-rw-   0        0        0      866 2024-04-02 21:33:31.000000 fastapi-requests-limit-0.1.5b1/fastapi_requests_limit/configuration.py
+-rw-rw-rw-   0        0        0      538 2024-04-02 20:00:53.000000 fastapi-requests-limit-0.1.5b1/fastapi_requests_limit/handle_errors.py
+-rw-rw-rw-   0        0        0     2162 2024-04-02 20:00:54.000000 fastapi-requests-limit-0.1.5b1/fastapi_requests_limit/limiter_rest.py
+-rw-rw-rw-   0        0        0      390 2024-04-02 21:33:31.000000 fastapi-requests-limit-0.1.5b1/fastapi_requests_limit/storage_engines.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:30:10.966282 fastapi-requests-limit-0.1.5b1/fastapi_requests_limit/storages/
+-rw-rw-rw-   0        0        0        0 2023-10-19 02:31:00.000000 fastapi-requests-limit-0.1.5b1/fastapi_requests_limit/storages/__init__.py
+-rw-rw-rw-   0        0        0      771 2024-04-02 20:00:54.000000 fastapi-requests-limit-0.1.5b1/fastapi_requests_limit/storages/memory.py
+-rw-rw-rw-   0        0        0        0 2023-10-19 02:31:30.000000 fastapi-requests-limit-0.1.5b1/fastapi_requests_limit/storages/mondodb.py
+-rw-rw-rw-   0        0        0      897 2024-04-02 20:00:53.000000 fastapi-requests-limit-0.1.5b1/fastapi_requests_limit/storages/redis.py
+-rw-rw-rw-   0        0        0      589 2024-04-02 20:03:20.000000 fastapi-requests-limit-0.1.5b1/fastapi_requests_limit/storages/storage.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:30:10.990779 fastapi-requests-limit-0.1.5b1/fastapi_requests_limit/test/
+-rw-rw-rw-   0        0        0        0 2023-11-09 21:24:25.000000 fastapi-requests-limit-0.1.5b1/fastapi_requests_limit/test/__init__.py
+-rw-rw-rw-   0        0        0      282 2023-11-17 23:12:25.000000 fastapi-requests-limit-0.1.5b1/fastapi_requests_limit/test/mock.py
+-rw-rw-rw-   0        0        0      420 2024-04-02 20:03:32.000000 fastapi-requests-limit-0.1.5b1/fastapi_requests_limit/test/test.py
+-rw-rw-rw-   0        0        0       33 2023-11-17 16:42:06.000000 fastapi-requests-limit-0.1.5b1/fastapi_requests_limit/test/test_constans.py
+-rw-rw-rw-   0        0        0     1517 2024-04-02 21:06:26.000000 fastapi-requests-limit-0.1.5b1/fastapi_requests_limit/test/test_limiter_memory.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:30:10.948024 fastapi-requests-limit-0.1.5b1/fastapi_requests_limit.egg-info/
+-rw-rw-rw-   0        0        0     4122 2024-04-03 22:30:10.000000 fastapi-requests-limit-0.1.5b1/fastapi_requests_limit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      876 2024-04-03 22:30:10.000000 fastapi-requests-limit-0.1.5b1/fastapi_requests_limit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 22:30:10.000000 fastapi-requests-limit-0.1.5b1/fastapi_requests_limit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-03 22:30:10.000000 fastapi-requests-limit-0.1.5b1/fastapi_requests_limit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-04-03 22:30:10.000000 fastapi-requests-limit-0.1.5b1/fastapi_requests_limit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 22:30:10.993750 fastapi-requests-limit-0.1.5b1/setup.cfg
+-rw-rw-rw-   0        0        0     1309 2024-04-03 22:30:04.000000 fastapi-requests-limit-0.1.5b1/setup.py
```

### Comparing `fastapi-requests-limit-0.1.5/LICENSE.txt` & `fastapi-requests-limit-0.1.5b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastapi-requests-limit-0.1.5/PKG-INFO` & `fastapi-requests-limit-0.1.5b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-requests-limit
-Version: 0.1.5
+Version: 0.1.5b1
 Summary: Control and limit request rates to FastAPI applications with Redis and local memory support.
 Home-page: https://github.com/oscarPyth/fastapi-requests-limit
 Author: Oscar Arias
 Author-email: ariasp26@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/oscarPyth/fastapi-requests-limit/issues
 Project-URL: Source, https://github.com/oscarPyth/fastapi-requests-limit
```

### Comparing `fastapi-requests-limit-0.1.5/README.md` & `fastapi-requests-limit-0.1.5b1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi-requests-limit-0.1.5/fastapi_requests_limit/configuration.py` & `fastapi-requests-limit-0.1.5b1/fastapi_requests_limit/configuration.py`

 * *Files identical despite different names*

### Comparing `fastapi-requests-limit-0.1.5/fastapi_requests_limit/handle_errors.py` & `fastapi-requests-limit-0.1.5b1/fastapi_requests_limit/handle_errors.py`

 * *Files identical despite different names*

### Comparing `fastapi-requests-limit-0.1.5/fastapi_requests_limit/limiter_rest.py` & `fastapi-requests-limit-0.1.5b1/fastapi_requests_limit/limiter_rest.py`

 * *Files identical despite different names*

### Comparing `fastapi-requests-limit-0.1.5/fastapi_requests_limit/storages/memory.py` & `fastapi-requests-limit-0.1.5b1/fastapi_requests_limit/storages/memory.py`

 * *Files identical despite different names*

### Comparing `fastapi-requests-limit-0.1.5/fastapi_requests_limit/storages/redis.py` & `fastapi-requests-limit-0.1.5b1/fastapi_requests_limit/storages/redis.py`

 * *Files identical despite different names*

### Comparing `fastapi-requests-limit-0.1.5/fastapi_requests_limit/storages/storage.py` & `fastapi-requests-limit-0.1.5b1/fastapi_requests_limit/storages/storage.py`

 * *Files identical despite different names*

### Comparing `fastapi-requests-limit-0.1.5/fastapi_requests_limit/test/test_limiter_memory.py` & `fastapi-requests-limit-0.1.5b1/fastapi_requests_limit/test/test_limiter_memory.py`

 * *Files identical despite different names*

### Comparing `fastapi-requests-limit-0.1.5/fastapi_requests_limit.egg-info/PKG-INFO` & `fastapi-requests-limit-0.1.5b1/fastapi_requests_limit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-requests-limit
-Version: 0.1.5
+Version: 0.1.5b1
 Summary: Control and limit request rates to FastAPI applications with Redis and local memory support.
 Home-page: https://github.com/oscarPyth/fastapi-requests-limit
 Author: Oscar Arias
 Author-email: ariasp26@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/oscarPyth/fastapi-requests-limit/issues
 Project-URL: Source, https://github.com/oscarPyth/fastapi-requests-limit
```

### Comparing `fastapi-requests-limit-0.1.5/fastapi_requests_limit.egg-info/SOURCES.txt` & `fastapi-requests-limit-0.1.5b1/fastapi_requests_limit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi-requests-limit-0.1.5/setup.py` & `fastapi-requests-limit-0.1.5b1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="fastapi-requests-limit",
-    version="0.1.5",
+    version="0.1.5-beta.1",
     author="Oscar Arias",
     author_email="ariasp26@gmail.com",
     description="Control and limit request rates to FastAPI applications with Redis and local memory support.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/oscarPyth/fastapi-requests-limit",
     packages=find_packages(),
```

