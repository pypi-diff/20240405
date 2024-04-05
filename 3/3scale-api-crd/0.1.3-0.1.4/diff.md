# Comparing `tmp/3scale-api-crd-0.1.3.tar.gz` & `tmp/3scale-api-crd-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3scale-api-crd-0.1.3.tar", last modified: Fri Apr  5 13:00:17 2024, max compression
+gzip compressed data, was "3scale-api-crd-0.1.4.tar", last modified: Fri Apr  5 13:00:33 2024, max compression
```

## Comparing `3scale-api-crd-0.1.3.tar` & `3scale-api-crd-0.1.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:00:17.009842 3scale-api-crd-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:00:17.005841 3scale-api-crd-0.1.3/3scale_api_crd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-05 13:00:16.000000 3scale-api-crd-0.1.3/3scale_api_crd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-05 13:00:17.000000 3scale-api-crd-0.1.3/3scale_api_crd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:00:16.000000 3scale-api-crd-0.1.3/3scale_api_crd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-05 13:00:16.000000 3scale-api-crd-0.1.3/3scale_api_crd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 13:00:16.000000 3scale-api-crd-0.1.3/3scale_api_crd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-05 13:00:17.009842 3scale-api-crd-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:00:17.009842 3scale-api-crd-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:00:17.005841 3scale-api-crd-0.1.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:00:17.009842 3scale-api-crd-0.1.3/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/tests/integration/asserts.py
--rw-r--r--   0 runner    (1001) docker     (127)    18166 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/tests/integration/test_integration_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/tests/integration/test_integration_activedocs.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/tests/integration/test_integration_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/tests/integration/test_integration_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/tests/integration/test_integration_application_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/tests/integration/test_integration_backend_mapping_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/tests/integration/test_integration_backend_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/tests/integration/test_integration_backend_usages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/tests/integration/test_integration_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/tests/integration/test_integration_custom_tenant.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/tests/integration/test_integration_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/tests/integration/test_integration_mapping_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/tests/integration/test_integration_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/tests/integration/test_integration_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/tests/integration/test_integration_openapis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/tests/integration/test_integration_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/tests/integration/test_integration_policy_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/tests/integration/test_integration_pricing_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/tests/integration/test_integration_promotes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/tests/integration/test_integration_services.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:00:17.009842 3scale-api-crd-0.1.3/threescale_api_crd/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/threescale_api_crd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/threescale_api_crd/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/threescale_api_crd/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    22087 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/threescale_api_crd/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)   107696 2024-04-05 13:00:11.000000 3scale-api-crd-0.1.3/threescale_api_crd/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:00:33.385916 3scale-api-crd-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:00:33.381916 3scale-api-crd-0.1.4/3scale_api_crd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-05 13:00:33.000000 3scale-api-crd-0.1.4/3scale_api_crd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-05 13:00:33.000000 3scale-api-crd-0.1.4/3scale_api_crd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:00:33.000000 3scale-api-crd-0.1.4/3scale_api_crd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-05 13:00:33.000000 3scale-api-crd-0.1.4/3scale_api_crd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 13:00:33.000000 3scale-api-crd-0.1.4/3scale_api_crd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-05 13:00:33.385916 3scale-api-crd-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:00:33.385916 3scale-api-crd-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:00:33.381916 3scale-api-crd-0.1.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:00:33.385916 3scale-api-crd-0.1.4/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18166 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_activedocs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_application_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_backend_mapping_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_backend_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_backend_usages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_custom_tenant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_mapping_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_openapis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_policy_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_pricing_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_promotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_services.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:00:33.385916 3scale-api-crd-0.1.4/threescale_api_crd/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/threescale_api_crd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/threescale_api_crd/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/threescale_api_crd/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22087 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/threescale_api_crd/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)   107696 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/threescale_api_crd/resources.py
```

### Comparing `3scale-api-crd-0.1.3/3scale_api_crd.egg-info/PKG-INFO` & `3scale-api-crd-0.1.4/3scale_api_crd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 3scale-api-crd
-Version: 0.1.3
+Version: 0.1.4
 Summary: 3scale CRD Python Client
 Home-page: https://github.com/3scale-qe/3scale-api-python-crd
 Author: Martin Kudlej
 Author-email: kudlej.martin@gmail.com
 Maintainer: Martin Kudlej
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `3scale-api-crd-0.1.3/3scale_api_crd.egg-info/SOURCES.txt` & `3scale-api-crd-0.1.4/3scale_api_crd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/LICENSE` & `3scale-api-crd-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/PKG-INFO` & `3scale-api-crd-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 3scale-api-crd
-Version: 0.1.3
+Version: 0.1.4
 Summary: 3scale CRD Python Client
 Home-page: https://github.com/3scale-qe/3scale-api-python-crd
 Author: Martin Kudlej
 Author-email: kudlej.martin@gmail.com
 Maintainer: Martin Kudlej
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `3scale-api-crd-0.1.3/README.md` & `3scale-api-crd-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/setup.py` & `3scale-api-crd-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/tests/integration/asserts.py` & `3scale-api-crd-0.1.4/tests/integration/asserts.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/tests/integration/conftest.py` & `3scale-api-crd-0.1.4/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/tests/integration/test_integration_accounts.py` & `3scale-api-crd-0.1.4/tests/integration/test_integration_accounts.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/tests/integration/test_integration_activedocs.py` & `3scale-api-crd-0.1.4/tests/integration/test_integration_activedocs.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/tests/integration/test_integration_application.py` & `3scale-api-crd-0.1.4/tests/integration/test_integration_application.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/tests/integration/test_integration_application_plan.py` & `3scale-api-crd-0.1.4/tests/integration/test_integration_application_plan.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/tests/integration/test_integration_backend_mapping_rules.py` & `3scale-api-crd-0.1.4/tests/integration/test_integration_backend_mapping_rules.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/tests/integration/test_integration_backend_metrics.py` & `3scale-api-crd-0.1.4/tests/integration/test_integration_backend_metrics.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/tests/integration/test_integration_backend_usages.py` & `3scale-api-crd-0.1.4/tests/integration/test_integration_backend_usages.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/tests/integration/test_integration_backends.py` & `3scale-api-crd-0.1.4/tests/integration/test_integration_backends.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/tests/integration/test_integration_custom_tenant.py` & `3scale-api-crd-0.1.4/tests/integration/test_integration_custom_tenant.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/tests/integration/test_integration_limit.py` & `3scale-api-crd-0.1.4/tests/integration/test_integration_limit.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/tests/integration/test_integration_mapping_rules.py` & `3scale-api-crd-0.1.4/tests/integration/test_integration_mapping_rules.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/tests/integration/test_integration_methods.py` & `3scale-api-crd-0.1.4/tests/integration/test_integration_methods.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/tests/integration/test_integration_metrics.py` & `3scale-api-crd-0.1.4/tests/integration/test_integration_metrics.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/tests/integration/test_integration_openapis.py` & `3scale-api-crd-0.1.4/tests/integration/test_integration_openapis.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/tests/integration/test_integration_policies.py` & `3scale-api-crd-0.1.4/tests/integration/test_integration_policies.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/tests/integration/test_integration_policy_registry.py` & `3scale-api-crd-0.1.4/tests/integration/test_integration_policy_registry.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/tests/integration/test_integration_pricing_rules.py` & `3scale-api-crd-0.1.4/tests/integration/test_integration_pricing_rules.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/tests/integration/test_integration_promotes.py` & `3scale-api-crd-0.1.4/tests/integration/test_integration_promotes.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/tests/integration/test_integration_services.py` & `3scale-api-crd-0.1.4/tests/integration/test_integration_services.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/threescale_api_crd/client.py` & `3scale-api-crd-0.1.4/threescale_api_crd/client.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/threescale_api_crd/constants.py` & `3scale-api-crd-0.1.4/threescale_api_crd/constants.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/threescale_api_crd/defaults.py` & `3scale-api-crd-0.1.4/threescale_api_crd/defaults.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.3/threescale_api_crd/resources.py` & `3scale-api-crd-0.1.4/threescale_api_crd/resources.py`

 * *Files identical despite different names*

