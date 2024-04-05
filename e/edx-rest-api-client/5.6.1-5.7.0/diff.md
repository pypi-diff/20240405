# Comparing `tmp/edx-rest-api-client-5.6.1.tar.gz` & `tmp/edx-rest-api-client-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-rest-api-client-5.6.1.tar", last modified: Thu Oct 12 14:06:43 2023, max compression
+gzip compressed data, was "edx-rest-api-client-5.7.0.tar", last modified: Fri Apr  5 16:49:11 2024, max compression
```

## Comparing `edx-rest-api-client-5.6.1.tar` & `edx-rest-api-client-5.7.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 14:06:43.388532 edx-rest-api-client-5.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2023-10-12 14:06:37.000000 edx-rest-api-client-5.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-10-12 14:06:37.000000 edx-rest-api-client-5.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2023-10-12 14:06:43.384532 edx-rest-api-client-5.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2023-10-12 14:06:37.000000 edx-rest-api-client-5.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 14:06:43.380532 edx-rest-api-client-5.6.1/edx_rest_api_client/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-10-12 14:06:37.000000 edx-rest-api-client-5.6.1/edx_rest_api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-12 14:06:37.000000 edx-rest-api-client-5.6.1/edx_rest_api_client/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2023-10-12 14:06:37.000000 edx-rest-api-client-5.6.1/edx_rest_api_client/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    13918 2023-10-12 14:06:37.000000 edx-rest-api-client-5.6.1/edx_rest_api_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-10-12 14:06:37.000000 edx-rest-api-client-5.6.1/edx_rest_api_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 14:06:43.384532 edx-rest-api-client-5.6.1/edx_rest_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2023-10-12 14:06:43.000000 edx-rest-api-client-5.6.1/edx_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      462 2023-10-12 14:06:43.000000 edx-rest-api-client-5.6.1/edx_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-12 14:06:43.000000 edx-rest-api-client-5.6.1/edx_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-10-12 14:06:43.000000 edx-rest-api-client-5.6.1/edx_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-12 14:06:43.000000 edx-rest-api-client-5.6.1/edx_rest_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 14:06:43.384532 edx-rest-api-client-5.6.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-10-12 14:06:37.000000 edx-rest-api-client-5.6.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      562 2023-10-12 14:06:37.000000 edx-rest-api-client-5.6.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-12 14:06:43.388532 edx-rest-api-client-5.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2023-10-12 14:06:37.000000 edx-rest-api-client-5.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:49:11.310763 edx-rest-api-client-5.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-05 16:49:08.000000 edx-rest-api-client-5.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-05 16:49:08.000000 edx-rest-api-client-5.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-04-05 16:49:11.310763 edx-rest-api-client-5.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-05 16:49:08.000000 edx-rest-api-client-5.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:49:11.306763 edx-rest-api-client-5.7.0/edx_rest_api_client/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-05 16:49:08.000000 edx-rest-api-client-5.7.0/edx_rest_api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-05 16:49:08.000000 edx-rest-api-client-5.7.0/edx_rest_api_client/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-05 16:49:08.000000 edx-rest-api-client-5.7.0/edx_rest_api_client/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13918 2024-04-05 16:49:08.000000 edx-rest-api-client-5.7.0/edx_rest_api_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-05 16:49:08.000000 edx-rest-api-client-5.7.0/edx_rest_api_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:49:11.310763 edx-rest-api-client-5.7.0/edx_rest_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-04-05 16:49:11.000000 edx-rest-api-client-5.7.0/edx_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-05 16:49:11.000000 edx-rest-api-client-5.7.0/edx_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:49:11.000000 edx-rest-api-client-5.7.0/edx_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 16:49:11.000000 edx-rest-api-client-5.7.0/edx_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-05 16:49:11.000000 edx-rest-api-client-5.7.0/edx_rest_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:49:11.310763 edx-rest-api-client-5.7.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-05 16:49:08.000000 edx-rest-api-client-5.7.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-05 16:49:08.000000 edx-rest-api-client-5.7.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:49:11.310763 edx-rest-api-client-5.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-05 16:49:08.000000 edx-rest-api-client-5.7.0/setup.py
```

### Comparing `edx-rest-api-client-5.6.1/LICENSE` & `edx-rest-api-client-5.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-rest-api-client-5.6.1/PKG-INFO` & `edx-rest-api-client-5.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: edx-rest-api-client
-Version: 5.6.1
+Version: 5.7.0
 Summary: Client utilities to access various Open edX Platform REST APIs.
 Home-page: https://github.com/openedx/edx-rest-api-client
 Author: edX
 Author-email: oscm@edx.org
 License: Apache
 Keywords: edx rest api client
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Framework :: Django :: 3.2
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Internet
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: PyJWT
 Requires-Dist: edx-django-utils
-Requires-Dist: requests
-Requires-Dist: slumber
+Requires-Dist: requests==2.31.0
+Requires-Dist: slumber==0.7.1
 
 edX REST API Client
 ###################
 
 | |status-badge| |license-badge| |CI| |Codecov| |pypi-badge|
 
 The edX REST API Client simplifies communicating with other Open edX services by providing OAuth2 and JWT utilities.
```

### Comparing `edx-rest-api-client-5.6.1/README.rst` & `edx-rest-api-client-5.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `edx-rest-api-client-5.6.1/edx_rest_api_client/auth.py` & `edx-rest-api-client-5.7.0/edx_rest_api_client/auth.py`

 * *Files identical despite different names*

### Comparing `edx-rest-api-client-5.6.1/edx_rest_api_client/client.py` & `edx-rest-api-client-5.7.0/edx_rest_api_client/client.py`

 * *Files identical despite different names*

### Comparing `edx-rest-api-client-5.6.1/edx_rest_api_client.egg-info/PKG-INFO` & `edx-rest-api-client-5.7.0/edx_rest_api_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: edx-rest-api-client
-Version: 5.6.1
+Version: 5.7.0
 Summary: Client utilities to access various Open edX Platform REST APIs.
 Home-page: https://github.com/openedx/edx-rest-api-client
 Author: edX
 Author-email: oscm@edx.org
 License: Apache
 Keywords: edx rest api client
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Framework :: Django :: 3.2
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Internet
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: PyJWT
 Requires-Dist: edx-django-utils
-Requires-Dist: requests
-Requires-Dist: slumber
+Requires-Dist: requests==2.31.0
+Requires-Dist: slumber==0.7.1
 
 edX REST API Client
 ###################
 
 | |status-badge| |license-badge| |CI| |Codecov| |pypi-badge|
 
 The edX REST API Client simplifies communicating with other Open edX services by providing OAuth2 and JWT utilities.
```

### Comparing `edx-rest-api-client-5.6.1/setup.py` & `edx-rest-api-client-5.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,16 @@
     long_description=long_description,
     long_description_content_type="text/x-rst",
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.8',
-        'Framework :: Django :: 3.2',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Framework :: Django :: 4.2',
         'Topic :: Internet',
         'Intended Audience :: Developers',
         'Environment :: Web Environment',
     ],
     keywords='edx rest api client',
     url='https://github.com/openedx/edx-rest-api-client',
```

