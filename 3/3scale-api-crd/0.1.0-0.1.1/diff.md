# Comparing `tmp/3scale-api-crd-0.1.0.tar.gz` & `tmp/3scale-api-crd-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3scale-api-crd-0.1.0.tar", last modified: Thu Apr  4 15:05:13 2024, max compression
+gzip compressed data, was "3scale-api-crd-0.1.1.tar", last modified: Fri Apr  5 08:30:09 2024, max compression
```

## Comparing `3scale-api-crd-0.1.0.tar` & `3scale-api-crd-0.1.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 mkudlej   (1000) mkudlej   (1000)        0 2024-04-04 15:05:13.683218 3scale-api-crd-0.1.0/
-drwxr-xr-x   0 mkudlej   (1000) mkudlej   (1000)        0 2024-04-04 15:05:13.679218 3scale-api-crd-0.1.0/3scale_api_crd.egg-info/
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     3776 2024-04-04 15:05:13.000000 3scale-api-crd-0.1.0/3scale_api_crd.egg-info/PKG-INFO
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     1489 2024-04-04 15:05:13.000000 3scale-api-crd-0.1.0/3scale_api_crd.egg-info/SOURCES.txt
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)        1 2024-04-04 15:05:13.000000 3scale-api-crd-0.1.0/3scale_api_crd.egg-info/dependency_links.txt
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)       98 2024-04-04 15:05:13.000000 3scale-api-crd-0.1.0/3scale_api_crd.egg-info/requires.txt
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)       25 2024-04-04 15:05:13.000000 3scale-api-crd-0.1.0/3scale_api_crd.egg-info/top_level.txt
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)    11358 2022-02-11 13:36:00.000000 3scale-api-crd-0.1.0/LICENSE
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     3776 2024-04-04 15:05:13.683218 3scale-api-crd-0.1.0/PKG-INFO
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     3148 2024-04-04 14:56:52.000000 3scale-api-crd-0.1.0/README.md
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)       38 2024-04-04 15:05:13.683218 3scale-api-crd-0.1.0/setup.cfg
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     1455 2024-04-04 15:02:42.000000 3scale-api-crd-0.1.0/setup.py
-drwxr-xr-x   0 mkudlej   (1000) mkudlej   (1000)        0 2024-04-04 15:05:13.679218 3scale-api-crd-0.1.0/tests/
-drwxr-xr-x   0 mkudlej   (1000) mkudlej   (1000)        0 2024-04-04 15:05:13.679218 3scale-api-crd-0.1.0/tests/integration/
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)        0 2021-09-01 05:17:29.000000 3scale-api-crd-0.1.0/tests/integration/__init__.py
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)      945 2022-12-07 14:43:15.000000 3scale-api-crd-0.1.0/tests/integration/asserts.py
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)    17864 2024-04-04 10:19:03.000000 3scale-api-crd-0.1.0/tests/integration/conftest.py
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     2880 2022-07-25 17:58:00.000000 3scale-api-crd-0.1.0/tests/integration/test_integration_accounts.py
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     2027 2022-02-14 14:35:10.000000 3scale-api-crd-0.1.0/tests/integration/test_integration_activedocs.py
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)      331 2022-02-09 12:32:30.000000 3scale-api-crd-0.1.0/tests/integration/test_integration_api_client.py
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     2269 2023-11-24 11:41:16.000000 3scale-api-crd-0.1.0/tests/integration/test_integration_application.py
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     1584 2023-05-29 12:01:16.000000 3scale-api-crd-0.1.0/tests/integration/test_integration_application_plan.py
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     2613 2024-02-05 12:15:06.000000 3scale-api-crd-0.1.0/tests/integration/test_integration_backend_mapping_rules.py
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     4686 2023-12-08 13:46:04.000000 3scale-api-crd-0.1.0/tests/integration/test_integration_backend_metrics.py
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     1152 2023-10-11 11:36:10.000000 3scale-api-crd-0.1.0/tests/integration/test_integration_backend_usages.py
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     1579 2023-11-24 17:01:58.000000 3scale-api-crd-0.1.0/tests/integration/test_integration_backends.py
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     1724 2023-10-24 08:13:19.000000 3scale-api-crd-0.1.0/tests/integration/test_integration_custom_tenant.py
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     2364 2023-12-07 10:22:26.000000 3scale-api-crd-0.1.0/tests/integration/test_integration_limit.py
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     2404 2023-06-20 08:11:41.000000 3scale-api-crd-0.1.0/tests/integration/test_integration_mapping_rules.py
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     1252 2023-12-08 12:46:21.000000 3scale-api-crd-0.1.0/tests/integration/test_integration_methods.py
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     3708 2023-06-09 07:18:56.000000 3scale-api-crd-0.1.0/tests/integration/test_integration_metrics.py
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     1027 2023-11-07 09:34:07.000000 3scale-api-crd-0.1.0/tests/integration/test_integration_openapis.py
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     1673 2021-09-01 05:17:29.000000 3scale-api-crd-0.1.0/tests/integration/test_integration_policies.py
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     1734 2021-09-01 05:17:29.000000 3scale-api-crd-0.1.0/tests/integration/test_integration_policy_registry.py
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     2891 2022-06-13 12:40:20.000000 3scale-api-crd-0.1.0/tests/integration/test_integration_pricing_rules.py
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     1710 2024-02-01 10:42:10.000000 3scale-api-crd-0.1.0/tests/integration/test_integration_promotes.py
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     5047 2024-03-26 13:47:32.000000 3scale-api-crd-0.1.0/tests/integration/test_integration_services.py
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     1140 2024-04-04 14:30:44.000000 3scale-api-crd-0.1.0/tests/test_3scale_api_client.py
-drwxr-xr-x   0 mkudlej   (1000) mkudlej   (1000)        0 2024-04-04 15:05:13.679218 3scale-api-crd-0.1.0/threescale_api_crd/
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)      121 2022-03-03 07:08:49.000000 3scale-api-crd-0.1.0/threescale_api_crd/__init__.py
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     4079 2024-04-04 14:30:47.000000 3scale-api-crd-0.1.0/threescale_api_crd/client.py
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)    13860 2024-03-04 17:15:51.000000 3scale-api-crd-0.1.0/threescale_api_crd/constants.py
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)    21039 2024-03-27 16:11:21.000000 3scale-api-crd-0.1.0/threescale_api_crd/defaults.py
--rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)   102324 2024-03-27 16:11:16.000000 3scale-api-crd-0.1.0/threescale_api_crd/resources.py
+drwxr-xr-x   0 mkudlej   (1000) mkudlej   (1000)        0 2024-04-05 08:30:09.283106 3scale-api-crd-0.1.1/
+drwxr-xr-x   0 mkudlej   (1000) mkudlej   (1000)        0 2024-04-05 08:30:09.275106 3scale-api-crd-0.1.1/3scale_api_crd.egg-info/
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     3776 2024-04-05 08:30:09.000000 3scale-api-crd-0.1.1/3scale_api_crd.egg-info/PKG-INFO
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     1489 2024-04-05 08:30:09.000000 3scale-api-crd-0.1.1/3scale_api_crd.egg-info/SOURCES.txt
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)        1 2024-04-05 08:30:09.000000 3scale-api-crd-0.1.1/3scale_api_crd.egg-info/dependency_links.txt
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)       98 2024-04-05 08:30:09.000000 3scale-api-crd-0.1.1/3scale_api_crd.egg-info/requires.txt
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)       25 2024-04-05 08:30:09.000000 3scale-api-crd-0.1.1/3scale_api_crd.egg-info/top_level.txt
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)    11358 2022-02-11 13:36:00.000000 3scale-api-crd-0.1.1/LICENSE
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     3776 2024-04-05 08:30:09.283106 3scale-api-crd-0.1.1/PKG-INFO
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     3148 2024-04-04 14:56:52.000000 3scale-api-crd-0.1.1/README.md
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)       38 2024-04-05 08:30:09.283106 3scale-api-crd-0.1.1/setup.cfg
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     1447 2024-04-05 08:29:58.000000 3scale-api-crd-0.1.1/setup.py
+drwxr-xr-x   0 mkudlej   (1000) mkudlej   (1000)        0 2024-04-05 08:30:09.275106 3scale-api-crd-0.1.1/tests/
+drwxr-xr-x   0 mkudlej   (1000) mkudlej   (1000)        0 2024-04-05 08:30:09.283106 3scale-api-crd-0.1.1/tests/integration/
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)        0 2021-09-01 05:17:29.000000 3scale-api-crd-0.1.1/tests/integration/__init__.py
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)      945 2022-12-07 14:43:15.000000 3scale-api-crd-0.1.1/tests/integration/asserts.py
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)    17864 2024-04-04 10:19:03.000000 3scale-api-crd-0.1.1/tests/integration/conftest.py
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     2880 2022-07-25 17:58:00.000000 3scale-api-crd-0.1.1/tests/integration/test_integration_accounts.py
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     2027 2022-02-14 14:35:10.000000 3scale-api-crd-0.1.1/tests/integration/test_integration_activedocs.py
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)      331 2022-02-09 12:32:30.000000 3scale-api-crd-0.1.1/tests/integration/test_integration_api_client.py
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     2269 2023-11-24 11:41:16.000000 3scale-api-crd-0.1.1/tests/integration/test_integration_application.py
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     1584 2023-05-29 12:01:16.000000 3scale-api-crd-0.1.1/tests/integration/test_integration_application_plan.py
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     2613 2024-02-05 12:15:06.000000 3scale-api-crd-0.1.1/tests/integration/test_integration_backend_mapping_rules.py
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     4686 2023-12-08 13:46:04.000000 3scale-api-crd-0.1.1/tests/integration/test_integration_backend_metrics.py
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     1152 2023-10-11 11:36:10.000000 3scale-api-crd-0.1.1/tests/integration/test_integration_backend_usages.py
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     1579 2023-11-24 17:01:58.000000 3scale-api-crd-0.1.1/tests/integration/test_integration_backends.py
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     1724 2023-10-24 08:13:19.000000 3scale-api-crd-0.1.1/tests/integration/test_integration_custom_tenant.py
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     2364 2023-12-07 10:22:26.000000 3scale-api-crd-0.1.1/tests/integration/test_integration_limit.py
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     2404 2023-06-20 08:11:41.000000 3scale-api-crd-0.1.1/tests/integration/test_integration_mapping_rules.py
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     1252 2023-12-08 12:46:21.000000 3scale-api-crd-0.1.1/tests/integration/test_integration_methods.py
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     3708 2023-06-09 07:18:56.000000 3scale-api-crd-0.1.1/tests/integration/test_integration_metrics.py
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     1027 2023-11-07 09:34:07.000000 3scale-api-crd-0.1.1/tests/integration/test_integration_openapis.py
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     1673 2021-09-01 05:17:29.000000 3scale-api-crd-0.1.1/tests/integration/test_integration_policies.py
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     1734 2021-09-01 05:17:29.000000 3scale-api-crd-0.1.1/tests/integration/test_integration_policy_registry.py
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     2891 2022-06-13 12:40:20.000000 3scale-api-crd-0.1.1/tests/integration/test_integration_pricing_rules.py
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     1710 2024-02-01 10:42:10.000000 3scale-api-crd-0.1.1/tests/integration/test_integration_promotes.py
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     5047 2024-03-26 13:47:32.000000 3scale-api-crd-0.1.1/tests/integration/test_integration_services.py
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     1140 2024-04-04 14:30:44.000000 3scale-api-crd-0.1.1/tests/test_3scale_api_client.py
+drwxr-xr-x   0 mkudlej   (1000) mkudlej   (1000)        0 2024-04-05 08:30:09.283106 3scale-api-crd-0.1.1/threescale_api_crd/
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)      121 2022-03-03 07:08:49.000000 3scale-api-crd-0.1.1/threescale_api_crd/__init__.py
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)     4079 2024-04-04 14:30:47.000000 3scale-api-crd-0.1.1/threescale_api_crd/client.py
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)    13860 2024-03-04 17:15:51.000000 3scale-api-crd-0.1.1/threescale_api_crd/constants.py
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)    21039 2024-03-27 16:11:21.000000 3scale-api-crd-0.1.1/threescale_api_crd/defaults.py
+-rw-r--r--   0 mkudlej   (1000) mkudlej   (1000)   102324 2024-03-27 16:11:16.000000 3scale-api-crd-0.1.1/threescale_api_crd/resources.py
```

### Comparing `3scale-api-crd-0.1.0/3scale_api_crd.egg-info/PKG-INFO` & `3scale-api-crd-0.1.1/3scale_api_crd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 3scale-api-crd
-Version: 0.1.0
+Version: 0.1.1
 Summary: 3scale CRD Python Client
 Home-page: https://github.com/3scale-qe/3scale-api-python-crd
 Author: Martin Kudlej
 Author-email: kudlej.martin@gmail.com
 Maintainer: Martin Kudlej
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `3scale-api-crd-0.1.0/3scale_api_crd.egg-info/SOURCES.txt` & `3scale-api-crd-0.1.1/3scale_api_crd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/LICENSE` & `3scale-api-crd-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/PKG-INFO` & `3scale-api-crd-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 3scale-api-crd
-Version: 0.1.0
+Version: 0.1.1
 Summary: 3scale CRD Python Client
 Home-page: https://github.com/3scale-qe/3scale-api-python-crd
 Author: Martin Kudlej
 Author-email: kudlej.martin@gmail.com
 Maintainer: Martin Kudlej
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `3scale-api-crd-0.1.0/README.md` & `3scale-api-crd-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/setup.py` & `3scale-api-crd-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,24 +8,23 @@
 
 VERSION = "devel"
 if sys.argv[1] == "--release-version":
     sys.argv.pop(1)
     VERSION = sys.argv.pop(1)
     assert re.match(r"[0-9]+\.[0-9]+\.[0-9]+", VERSION), "Version definition required as first arg"
 
-requirements = ['3scale-api', 'openshift-client']
+requirements = ['3scale-api', 'openshift-client', 'backoff']
 
 extra_requirements = {
     'dev': [
         'flake8',
         'mypy',
         'pylint',
         'pytest',
         'python-dotenv',
-        'backoff',
     ],
     'docs': ['sphinx']
 }
 
 setup(name='3scale-api-crd',
       version=VERSION,
       description='3scale CRD Python Client',
```

### Comparing `3scale-api-crd-0.1.0/tests/integration/asserts.py` & `3scale-api-crd-0.1.1/tests/integration/asserts.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/tests/integration/conftest.py` & `3scale-api-crd-0.1.1/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/tests/integration/test_integration_accounts.py` & `3scale-api-crd-0.1.1/tests/integration/test_integration_accounts.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/tests/integration/test_integration_activedocs.py` & `3scale-api-crd-0.1.1/tests/integration/test_integration_activedocs.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/tests/integration/test_integration_application.py` & `3scale-api-crd-0.1.1/tests/integration/test_integration_application.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/tests/integration/test_integration_application_plan.py` & `3scale-api-crd-0.1.1/tests/integration/test_integration_application_plan.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/tests/integration/test_integration_backend_mapping_rules.py` & `3scale-api-crd-0.1.1/tests/integration/test_integration_backend_mapping_rules.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/tests/integration/test_integration_backend_metrics.py` & `3scale-api-crd-0.1.1/tests/integration/test_integration_backend_metrics.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/tests/integration/test_integration_backend_usages.py` & `3scale-api-crd-0.1.1/tests/integration/test_integration_backend_usages.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/tests/integration/test_integration_backends.py` & `3scale-api-crd-0.1.1/tests/integration/test_integration_backends.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/tests/integration/test_integration_custom_tenant.py` & `3scale-api-crd-0.1.1/tests/integration/test_integration_custom_tenant.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/tests/integration/test_integration_limit.py` & `3scale-api-crd-0.1.1/tests/integration/test_integration_limit.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/tests/integration/test_integration_mapping_rules.py` & `3scale-api-crd-0.1.1/tests/integration/test_integration_mapping_rules.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/tests/integration/test_integration_methods.py` & `3scale-api-crd-0.1.1/tests/integration/test_integration_methods.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/tests/integration/test_integration_metrics.py` & `3scale-api-crd-0.1.1/tests/integration/test_integration_metrics.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/tests/integration/test_integration_openapis.py` & `3scale-api-crd-0.1.1/tests/integration/test_integration_openapis.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/tests/integration/test_integration_policies.py` & `3scale-api-crd-0.1.1/tests/integration/test_integration_policies.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/tests/integration/test_integration_policy_registry.py` & `3scale-api-crd-0.1.1/tests/integration/test_integration_policy_registry.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/tests/integration/test_integration_pricing_rules.py` & `3scale-api-crd-0.1.1/tests/integration/test_integration_pricing_rules.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/tests/integration/test_integration_promotes.py` & `3scale-api-crd-0.1.1/tests/integration/test_integration_promotes.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/tests/integration/test_integration_services.py` & `3scale-api-crd-0.1.1/tests/integration/test_integration_services.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/tests/test_3scale_api_client.py` & `3scale-api-crd-0.1.1/tests/test_3scale_api_client.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/threescale_api_crd/client.py` & `3scale-api-crd-0.1.1/threescale_api_crd/client.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/threescale_api_crd/constants.py` & `3scale-api-crd-0.1.1/threescale_api_crd/constants.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/threescale_api_crd/defaults.py` & `3scale-api-crd-0.1.1/threescale_api_crd/defaults.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.0/threescale_api_crd/resources.py` & `3scale-api-crd-0.1.1/threescale_api_crd/resources.py`

 * *Files identical despite different names*

