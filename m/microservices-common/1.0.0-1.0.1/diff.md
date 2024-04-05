# Comparing `tmp/microservices_common-1.0.0.tar.gz` & `tmp/microservices_common-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microservices_common-1.0.0.tar", last modified: Mon Feb 12 07:47:42 2024, max compression
+gzip compressed data, was "microservices_common-1.0.1.tar", last modified: Fri Apr  5 12:43:06 2024, max compression
```

## Comparing `microservices_common-1.0.0.tar` & `microservices_common-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-02-12 07:47:42.987795 microservices_common-1.0.0/
--rw-r--r--   0 AliZaidi   (502) staff       (20)      560 2024-02-12 07:47:42.987550 microservices_common-1.0.0/PKG-INFO
--rw-r--r--   0 AliZaidi   (502) staff       (20)       38 2024-02-12 07:47:42.987855 microservices_common-1.0.0/setup.cfg
--rw-r--r--   0 AliZaidi   (502) staff       (20)      752 2024-02-12 07:36:34.000000 microservices_common-1.0.0/setup.py
-drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-02-12 07:47:42.981455 microservices_common-1.0.0/src/
-drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-02-12 07:47:42.982014 microservices_common-1.0.0/src/microservices_common/
--rw-r--r--   0 AliZaidi   (502) staff       (20)      134 2023-08-18 11:57:19.000000 microservices_common-1.0.0/src/microservices_common/__init__.py
-drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-02-12 07:47:42.985376 microservices_common-1.0.0/src/microservices_common/exceptions/
--rw-r--r--   0 AliZaidi   (502) staff       (20)      498 2023-08-18 11:57:19.000000 microservices_common-1.0.0/src/microservices_common/exceptions/__init__.py
--rw-r--r--   0 AliZaidi   (502) staff       (20)      354 2023-08-18 11:57:19.000000 microservices_common-1.0.0/src/microservices_common/exceptions/authentication_exception.py
--rw-r--r--   0 AliZaidi   (502) staff       (20)      361 2023-08-18 11:57:19.000000 microservices_common-1.0.0/src/microservices_common/exceptions/custom_exception.py
--rw-r--r--   0 AliZaidi   (502) staff       (20)      387 2023-08-18 11:57:19.000000 microservices_common-1.0.0/src/microservices_common/exceptions/incorrect_parameter_format_exception.py
--rw-r--r--   0 AliZaidi   (502) staff       (20)      469 2023-08-18 11:57:19.000000 microservices_common-1.0.0/src/microservices_common/exceptions/invalid_input_exception.py
--rw-r--r--   0 AliZaidi   (502) staff       (20)      379 2023-08-18 11:57:19.000000 microservices_common-1.0.0/src/microservices_common/exceptions/not_found_exception.py
--rw-r--r--   0 AliZaidi   (502) staff       (20)      354 2023-08-18 11:57:19.000000 microservices_common-1.0.0/src/microservices_common/exceptions/owner_not_found_exception.py
--rw-r--r--   0 AliZaidi   (502) staff       (20)      352 2023-08-18 11:57:19.000000 microservices_common-1.0.0/src/microservices_common/exceptions/userid_not_found_exception.py
-drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-02-12 07:47:42.986327 microservices_common-1.0.0/src/microservices_common/middlewares/
--rw-r--r--   0 AliZaidi   (502) staff       (20)      176 2023-08-18 11:57:19.000000 microservices_common-1.0.0/src/microservices_common/middlewares/__init__.py
--rw-r--r--   0 AliZaidi   (502) staff       (20)      349 2023-08-18 11:57:19.000000 microservices_common-1.0.0/src/microservices_common/middlewares/admin.py
--rw-r--r--   0 AliZaidi   (502) staff       (20)     3402 2023-08-18 11:57:19.000000 microservices_common-1.0.0/src/microservices_common/middlewares/authorized.py
--rw-r--r--   0 AliZaidi   (502) staff       (20)     1116 2023-08-18 11:57:19.000000 microservices_common-1.0.0/src/microservices_common/middlewares/exception_handler.py
-drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-02-12 07:47:42.987108 microservices_common-1.0.0/src/microservices_common/utils/
--rw-r--r--   0 AliZaidi   (502) staff       (20)      149 2023-08-18 11:57:19.000000 microservices_common-1.0.0/src/microservices_common/utils/__init__.py
--rw-r--r--   0 AliZaidi   (502) staff       (20)     2779 2023-08-18 11:57:19.000000 microservices_common-1.0.0/src/microservices_common/utils/datetime_util.py
--rw-r--r--   0 AliZaidi   (502) staff       (20)     1061 2024-02-12 07:32:18.000000 microservices_common-1.0.0/src/microservices_common/utils/logger.py
--rw-r--r--   0 AliZaidi   (502) staff       (20)    15355 2023-08-18 11:57:19.000000 microservices_common-1.0.0/src/microservices_common/utils/util.py
-drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-02-12 07:47:42.983276 microservices_common-1.0.0/src/microservices_common.egg-info/
--rw-r--r--   0 AliZaidi   (502) staff       (20)      560 2024-02-12 07:47:42.000000 microservices_common-1.0.0/src/microservices_common.egg-info/PKG-INFO
--rw-r--r--   0 AliZaidi   (502) staff       (20)     1156 2024-02-12 07:47:42.000000 microservices_common-1.0.0/src/microservices_common.egg-info/SOURCES.txt
--rw-r--r--   0 AliZaidi   (502) staff       (20)        1 2024-02-12 07:47:42.000000 microservices_common-1.0.0/src/microservices_common.egg-info/dependency_links.txt
--rw-r--r--   0 AliZaidi   (502) staff       (20)      140 2024-02-12 07:47:42.000000 microservices_common-1.0.0/src/microservices_common.egg-info/requires.txt
--rw-r--r--   0 AliZaidi   (502) staff       (20)       21 2024-02-12 07:47:42.000000 microservices_common-1.0.0/src/microservices_common.egg-info/top_level.txt
+drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-04-05 12:43:06.159484 microservices_common-1.0.1/
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      560 2024-04-05 12:43:06.159224 microservices_common-1.0.1/PKG-INFO
+-rw-r--r--   0 AliZaidi   (502) staff       (20)       38 2024-04-05 12:43:06.159533 microservices_common-1.0.1/setup.cfg
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      752 2024-04-05 12:42:59.000000 microservices_common-1.0.1/setup.py
+drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-04-05 12:43:06.154443 microservices_common-1.0.1/src/
+drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-04-05 12:43:06.154938 microservices_common-1.0.1/src/microservices_common/
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      134 2023-08-18 11:57:19.000000 microservices_common-1.0.1/src/microservices_common/__init__.py
+drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-04-05 12:43:06.157127 microservices_common-1.0.1/src/microservices_common/exceptions/
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      498 2023-08-18 11:57:19.000000 microservices_common-1.0.1/src/microservices_common/exceptions/__init__.py
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      354 2023-08-18 11:57:19.000000 microservices_common-1.0.1/src/microservices_common/exceptions/authentication_exception.py
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      361 2023-08-18 11:57:19.000000 microservices_common-1.0.1/src/microservices_common/exceptions/custom_exception.py
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      387 2023-08-18 11:57:19.000000 microservices_common-1.0.1/src/microservices_common/exceptions/incorrect_parameter_format_exception.py
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      469 2023-08-18 11:57:19.000000 microservices_common-1.0.1/src/microservices_common/exceptions/invalid_input_exception.py
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      379 2023-08-18 11:57:19.000000 microservices_common-1.0.1/src/microservices_common/exceptions/not_found_exception.py
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      354 2023-08-18 11:57:19.000000 microservices_common-1.0.1/src/microservices_common/exceptions/owner_not_found_exception.py
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      352 2023-08-18 11:57:19.000000 microservices_common-1.0.1/src/microservices_common/exceptions/userid_not_found_exception.py
+drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-04-05 12:43:06.157666 microservices_common-1.0.1/src/microservices_common/middlewares/
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      176 2023-08-18 11:57:19.000000 microservices_common-1.0.1/src/microservices_common/middlewares/__init__.py
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      349 2023-08-18 11:57:19.000000 microservices_common-1.0.1/src/microservices_common/middlewares/admin.py
+-rw-r--r--   0 AliZaidi   (502) staff       (20)     3402 2023-08-18 11:57:19.000000 microservices_common-1.0.1/src/microservices_common/middlewares/authorized.py
+-rw-r--r--   0 AliZaidi   (502) staff       (20)     1116 2024-04-05 12:38:51.000000 microservices_common-1.0.1/src/microservices_common/middlewares/exception_handler.py
+drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-04-05 12:43:06.158761 microservices_common-1.0.1/src/microservices_common/utils/
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      149 2023-08-18 11:57:19.000000 microservices_common-1.0.1/src/microservices_common/utils/__init__.py
+-rw-r--r--   0 AliZaidi   (502) staff       (20)     2779 2023-08-18 11:57:19.000000 microservices_common-1.0.1/src/microservices_common/utils/datetime_util.py
+-rw-r--r--   0 AliZaidi   (502) staff       (20)     1293 2024-03-05 07:23:11.000000 microservices_common-1.0.1/src/microservices_common/utils/logger.py
+-rw-r--r--   0 AliZaidi   (502) staff       (20)    15465 2024-04-05 12:43:01.000000 microservices_common-1.0.1/src/microservices_common/utils/util.py
+drwxr-xr-x   0 AliZaidi   (502) staff       (20)        0 2024-04-05 12:43:06.155588 microservices_common-1.0.1/src/microservices_common.egg-info/
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      560 2024-04-05 12:43:06.000000 microservices_common-1.0.1/src/microservices_common.egg-info/PKG-INFO
+-rw-r--r--   0 AliZaidi   (502) staff       (20)     1156 2024-04-05 12:43:06.000000 microservices_common-1.0.1/src/microservices_common.egg-info/SOURCES.txt
+-rw-r--r--   0 AliZaidi   (502) staff       (20)        1 2024-04-05 12:43:06.000000 microservices_common-1.0.1/src/microservices_common.egg-info/dependency_links.txt
+-rw-r--r--   0 AliZaidi   (502) staff       (20)      140 2024-04-05 12:43:06.000000 microservices_common-1.0.1/src/microservices_common.egg-info/requires.txt
+-rw-r--r--   0 AliZaidi   (502) staff       (20)       21 2024-04-05 12:43:06.000000 microservices_common-1.0.1/src/microservices_common.egg-info/top_level.txt
```

### Comparing `microservices_common-1.0.0/PKG-INFO` & `microservices_common-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microservices_common
-Version: 1.0.0
+Version: 1.0.1
 Home-page: https://github.com/arrivy-dev/microservices-python-common
 Author: Ali Zaidi
 Author-email: support@arrivy.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: google-cloud-error-reporting==1.5.2
```

### Comparing `microservices_common-1.0.0/setup.py` & `microservices_common-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="microservices_common",
-    version="1.0.0",
+    version="1.0.1",
     author="Ali Zaidi",
     author_email="support@arrivy.com",
     description="",
     long_description="",
     url="https://github.com/arrivy-dev/microservices-python-common",
     packages=find_packages('src'),
     package_dir={'': 'src'},
```

### Comparing `microservices_common-1.0.0/src/microservices_common/middlewares/authorized.py` & `microservices_common-1.0.1/src/microservices_common/middlewares/authorized.py`

 * *Files identical despite different names*

### Comparing `microservices_common-1.0.0/src/microservices_common/middlewares/exception_handler.py` & `microservices_common-1.0.1/src/microservices_common/middlewares/exception_handler.py`

 * *Files identical despite different names*

### Comparing `microservices_common-1.0.0/src/microservices_common/utils/datetime_util.py` & `microservices_common-1.0.1/src/microservices_common/utils/datetime_util.py`

 * *Files identical despite different names*

### Comparing `microservices_common-1.0.0/src/microservices_common/utils/util.py` & `microservices_common-1.0.1/src/microservices_common/utils/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,15 +247,16 @@
         if _json and Util.check_attribute_type('_json', _json) != 'dict':
             return json.loads(_json)
         return _json
 
     @classmethod
     def is_admin(cls, request):
         import os
-        return request.headers.get('Admin-Key') and request.headers.get('Admin-Key') == os.getenv('ADMIN_KEY')
+        return (request.headers.get('Admin-Key') and request.headers.get('Admin-Key') == os.getenv('ADMIN_KEY')) or (
+            request.args.get('admin_key') and request.args.get('admin_key') == os.getenv('ADMIN_KEY'))
 
     @classmethod
     def print_traceback(cls):
         import traceback
         Logger.info(traceback.format_exc())
 
 
@@ -369,15 +370,15 @@
             "http_request": {  # Specify the type of request.
                 "http_method": tasks_v2.HttpMethod.POST,
 
                 "url": url,  # The full url path that the task will be sent to.
             }
         }
         request_headers = dict()
-        if headers is not None and isinstance(payload, dict):
+        if headers is not None and isinstance(headers, dict):
             request_headers = json.dumps(headers)
 
         if payload is not None:
             if isinstance(payload, dict):
                 # Convert dict to JSON string
                 payload = json.dumps(payload)
                 # specify http content-type to application/json
```

### Comparing `microservices_common-1.0.0/src/microservices_common.egg-info/PKG-INFO` & `microservices_common-1.0.1/src/microservices_common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microservices-common
-Version: 1.0.0
+Version: 1.0.1
 Home-page: https://github.com/arrivy-dev/microservices-python-common
 Author: Ali Zaidi
 Author-email: support@arrivy.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: google-cloud-error-reporting==1.5.2
```

### Comparing `microservices_common-1.0.0/src/microservices_common.egg-info/SOURCES.txt` & `microservices_common-1.0.1/src/microservices_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

