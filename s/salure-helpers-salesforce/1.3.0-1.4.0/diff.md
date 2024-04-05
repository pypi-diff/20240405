# Comparing `tmp/salure_helpers_salesforce-1.3.0.tar.gz` & `tmp/salure_helpers_salesforce-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_salesforce-1.3.0.tar", last modified: Wed Nov  1 10:53:07 2023, max compression
+gzip compressed data, was "dist/salure_helpers_salesforce-1.4.0.tar", last modified: Fri Apr  5 07:07:13 2024, max compression
```

## Comparing `salure_helpers_salesforce-1.3.0.tar` & `salure_helpers_salesforce-1.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-01 10:53:07.000000 salure_helpers_salesforce-1.3.0/
--rw-r--r--   0 root         (0) root         (0)      274 2023-11-01 10:53:07.000000 salure_helpers_salesforce-1.3.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-01 10:53:07.000000 salure_helpers_salesforce-1.3.0/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-01 10:53:07.000000 salure_helpers_salesforce-1.3.0/salure_helpers/salesforce/
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-11-01 10:52:54.000000 salure_helpers_salesforce-1.3.0/salure_helpers/salesforce/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15006 2023-11-01 10:52:54.000000 salure_helpers_salesforce-1.3.0/salure_helpers/salesforce/salesforce.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-01 10:53:07.000000 salure_helpers_salesforce-1.3.0/salure_helpers_salesforce.egg-info/
--rw-r--r--   0 root         (0) root         (0)      274 2023-11-01 10:53:07.000000 salure_helpers_salesforce-1.3.0/salure_helpers_salesforce.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      378 2023-11-01 10:53:07.000000 salure_helpers_salesforce-1.3.0/salure_helpers_salesforce.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-01 10:53:07.000000 salure_helpers_salesforce-1.3.0/salure_helpers_salesforce.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-01 10:53:07.000000 salure_helpers_salesforce-1.3.0/salure_helpers_salesforce.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       78 2023-11-01 10:53:07.000000 salure_helpers_salesforce-1.3.0/salure_helpers_salesforce.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-11-01 10:53:07.000000 salure_helpers_salesforce-1.3.0/salure_helpers_salesforce.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-11-01 10:53:07.000000 salure_helpers_salesforce-1.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      520 2023-11-01 10:52:54.000000 salure_helpers_salesforce-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 07:07:13.000000 salure_helpers_salesforce-1.4.0/
+-rw-r--r--   0 root         (0) root         (0)      274 2024-04-05 07:07:13.000000 salure_helpers_salesforce-1.4.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 07:07:13.000000 salure_helpers_salesforce-1.4.0/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 07:07:13.000000 salure_helpers_salesforce-1.4.0/salure_helpers/salesforce/
+-rw-rw-rw-   0 root         (0) root         (0)       59 2024-04-05 07:06:55.000000 salure_helpers_salesforce-1.4.0/salure_helpers/salesforce/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15147 2024-04-05 07:06:55.000000 salure_helpers_salesforce-1.4.0/salure_helpers/salesforce/salesforce.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 07:07:13.000000 salure_helpers_salesforce-1.4.0/salure_helpers_salesforce.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      274 2024-04-05 07:07:13.000000 salure_helpers_salesforce-1.4.0/salure_helpers_salesforce.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      378 2024-04-05 07:07:13.000000 salure_helpers_salesforce-1.4.0/salure_helpers_salesforce.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 07:07:13.000000 salure_helpers_salesforce-1.4.0/salure_helpers_salesforce.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 07:07:13.000000 salure_helpers_salesforce-1.4.0/salure_helpers_salesforce.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       78 2024-04-05 07:07:13.000000 salure_helpers_salesforce-1.4.0/salure_helpers_salesforce.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-05 07:07:13.000000 salure_helpers_salesforce-1.4.0/salure_helpers_salesforce.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 07:07:13.000000 salure_helpers_salesforce-1.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      520 2024-04-05 07:06:55.000000 salure_helpers_salesforce-1.4.0/setup.py
```

### Comparing `salure_helpers_salesforce-1.3.0/salure_helpers/salesforce/salesforce.py` & `salure_helpers_salesforce-1.4.0/salure_helpers/salesforce/salesforce.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,28 @@
 
 
 class Salesforce(SalureConnect):
     """
     This class is meant to be a simple wrapper around the Salesforce API. In order to start using it, authorize your application is Salureconnect.
     You will receive a code which you can use to obtain a refresh token using the get_refresh_token method. Use this refresh token to refresh your access token always before you make a data call.
     """
-    def __init__(self, label: Union[str, List], debug: bool = False):
+    def __init__(self, label: Union[str, List], debug: bool = False, sandbox: bool = False):
         super().__init__()
-        self.credentials = self.get_system_credential(system='salesforce', label=label)
+        if sandbox:
+            self.system = 'salesforce-sandbox'
+        else:
+            self.system = 'salesforce'
+        self.credentials = self.get_system_credential(system=self.system, label=label)
         self.credential_id = self.credentials['id']
         self.customer_url = self.credentials['auth']['instance_url']
         self.debug = debug
         self.api_version = 56.0
 
     def __get_headers(self) -> dict:
-        credentials = self.refresh_system_credential(system='salesforce', system_id=self.credential_id)
+        credentials = self.refresh_system_credential(system=self.system, system_id=self.credential_id)
         headers = {"Authorization": f"Bearer {credentials['access_token']}",
                    "Content-Type": "application/json"}
         if self.debug:
             print(f"Headers: {headers}")
 
         return headers
```

### Comparing `salure_helpers_salesforce-1.3.0/setup.py` & `salure_helpers_salesforce-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='salure_helpers_salesforce',
-    version='1.3.0',
+    version='1.4.0',
     description='Salesforce wrapper from Salure',
     long_description='Salesforce wrapper from Salure',
     author='D&A Salure',
     author_email='support@salureconnnect.com',
     packages=["salure_helpers.salesforce"],
     license='Salure License',
     install_requires=[
```

