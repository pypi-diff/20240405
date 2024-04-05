# Comparing `tmp/reapit-cdk.service-quotas-0.1.0.tar.gz` & `tmp/reapit-cdk.service-quotas-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reapit-cdk.service-quotas-0.1.0.tar", last modified: Tue Apr  2 13:00:30 2024, max compression
+gzip compressed data, was "reapit-cdk.service-quotas-0.1.2.tar", last modified: Fri Apr  5 10:29:19 2024, max compression
```

## Comparing `reapit-cdk.service-quotas-0.1.0.tar` & `reapit-cdk.service-quotas-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:00:30.094190 reapit-cdk.service-quotas-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-02 13:00:22.000000 reapit-cdk.service-quotas-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 13:00:22.000000 reapit-cdk.service-quotas-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-02 13:00:30.094190 reapit-cdk.service-quotas-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-02 13:00:22.000000 reapit-cdk.service-quotas-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-02 13:00:22.000000 reapit-cdk.service-quotas-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 13:00:30.094190 reapit-cdk.service-quotas-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-02 13:00:22.000000 reapit-cdk.service-quotas-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:00:30.090190 reapit-cdk.service-quotas-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:00:30.090190 reapit-cdk.service-quotas-0.1.0/src/reapit_cdk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:00:30.094190 reapit-cdk.service-quotas-0.1.0/src/reapit_cdk/service_quotas/
--rw-r--r--   0 runner    (1001) docker     (127)   708742 2024-04-02 13:00:22.000000 reapit-cdk.service-quotas-0.1.0/src/reapit_cdk/service_quotas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:00:30.094190 reapit-cdk.service-quotas-0.1.0/src/reapit_cdk/service_quotas/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-02 13:00:22.000000 reapit-cdk.service-quotas-0.1.0/src/reapit_cdk/service_quotas/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   732317 2024-04-02 13:00:22.000000 reapit-cdk.service-quotas-0.1.0/src/reapit_cdk/service_quotas/_jsii/service-quotas@0.1.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:00:22.000000 reapit-cdk.service-quotas-0.1.0/src/reapit_cdk/service_quotas/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:00:30.090190 reapit-cdk.service-quotas-0.1.0/src/reapit_cdk.service_quotas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-02 13:00:30.000000 reapit-cdk.service-quotas-0.1.0/src/reapit_cdk.service_quotas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-02 13:00:30.000000 reapit-cdk.service-quotas-0.1.0/src/reapit_cdk.service_quotas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:00:30.000000 reapit-cdk.service-quotas-0.1.0/src/reapit_cdk.service_quotas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 13:00:30.000000 reapit-cdk.service-quotas-0.1.0/src/reapit_cdk.service_quotas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 13:00:30.000000 reapit-cdk.service-quotas-0.1.0/src/reapit_cdk.service_quotas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:29:19.889750 reapit-cdk.service-quotas-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-05 10:29:12.000000 reapit-cdk.service-quotas-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-05 10:29:12.000000 reapit-cdk.service-quotas-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-05 10:29:19.889750 reapit-cdk.service-quotas-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-05 10:29:12.000000 reapit-cdk.service-quotas-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-05 10:29:12.000000 reapit-cdk.service-quotas-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 10:29:19.889750 reapit-cdk.service-quotas-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-05 10:29:12.000000 reapit-cdk.service-quotas-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:29:19.885750 reapit-cdk.service-quotas-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:29:19.885750 reapit-cdk.service-quotas-0.1.2/src/reapit_cdk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:29:19.889750 reapit-cdk.service-quotas-0.1.2/src/reapit_cdk/service_quotas/
+-rw-r--r--   0 runner    (1001) docker     (127)   708742 2024-04-05 10:29:12.000000 reapit-cdk.service-quotas-0.1.2/src/reapit_cdk/service_quotas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:29:19.889750 reapit-cdk.service-quotas-0.1.2/src/reapit_cdk/service_quotas/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-05 10:29:12.000000 reapit-cdk.service-quotas-0.1.2/src/reapit_cdk/service_quotas/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   622159 2024-04-05 10:29:12.000000 reapit-cdk.service-quotas-0.1.2/src/reapit_cdk/service_quotas/_jsii/service-quotas@0.1.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 10:29:12.000000 reapit-cdk.service-quotas-0.1.2/src/reapit_cdk/service_quotas/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:29:19.889750 reapit-cdk.service-quotas-0.1.2/src/reapit_cdk.service_quotas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-05 10:29:19.000000 reapit-cdk.service-quotas-0.1.2/src/reapit_cdk.service_quotas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-05 10:29:19.000000 reapit-cdk.service-quotas-0.1.2/src/reapit_cdk.service_quotas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 10:29:19.000000 reapit-cdk.service-quotas-0.1.2/src/reapit_cdk.service_quotas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-05 10:29:19.000000 reapit-cdk.service-quotas-0.1.2/src/reapit_cdk.service_quotas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 10:29:19.000000 reapit-cdk.service-quotas-0.1.2/src/reapit_cdk.service_quotas.egg-info/top_level.txt
```

### Comparing `reapit-cdk.service-quotas-0.1.0/LICENSE` & `reapit-cdk.service-quotas-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reapit-cdk.service-quotas-0.1.0/PKG-INFO` & `reapit-cdk.service-quotas-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reapit-cdk.service-quotas
-Version: 0.1.0
+Version: 0.1.2
 Summary: This construct allows you to IaC your service quotas
 Home-page: https://github.com/reapit/ts-cdk-constructs/blob/main/packages/modules/service-quotas
 Author: Josh Balfour<jbalfour@reapit.com>
 License: MIT
 Project-URL: Source, https://github.com/reapit/ts-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `reapit-cdk.service-quotas-0.1.0/README.md` & `reapit-cdk.service-quotas-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `reapit-cdk.service-quotas-0.1.0/setup.py` & `reapit-cdk.service-quotas-0.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "reapit-cdk.service-quotas",
-    "version": "0.1.0",
+    "version": "0.1.2",
     "description": "This construct allows you to IaC your service quotas",
     "license": "MIT",
     "url": "https://github.com/reapit/ts-cdk-constructs/blob/main/packages/modules/service-quotas",
     "long_description_content_type": "text/markdown",
     "author": "Josh Balfour<jbalfour@reapit.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "reapit_cdk.service_quotas",
         "reapit_cdk.service_quotas._jsii"
     ],
     "package_data": {
         "reapit_cdk.service_quotas._jsii": [
-            "service-quotas@0.1.0.jsii.tgz"
+            "service-quotas@0.1.2.jsii.tgz"
         ],
         "reapit_cdk.service_quotas": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `reapit-cdk.service-quotas-0.1.0/src/reapit_cdk/service_quotas/__init__.py` & `reapit-cdk.service-quotas-0.1.2/src/reapit_cdk/service_quotas/__init__.py`

 * *Files identical despite different names*

### Comparing `reapit-cdk.service-quotas-0.1.0/src/reapit_cdk.service_quotas.egg-info/PKG-INFO` & `reapit-cdk.service-quotas-0.1.2/src/reapit_cdk.service_quotas.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reapit-cdk.service-quotas
-Version: 0.1.0
+Version: 0.1.2
 Summary: This construct allows you to IaC your service quotas
 Home-page: https://github.com/reapit/ts-cdk-constructs/blob/main/packages/modules/service-quotas
 Author: Josh Balfour<jbalfour@reapit.com>
 License: MIT
 Project-URL: Source, https://github.com/reapit/ts-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `reapit-cdk.service-quotas-0.1.0/src/reapit_cdk.service_quotas.egg-info/SOURCES.txt` & `reapit-cdk.service-quotas-0.1.2/src/reapit_cdk.service_quotas.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/reapit_cdk.service_quotas.egg-info/SOURCES.txt
 src/reapit_cdk.service_quotas.egg-info/dependency_links.txt
 src/reapit_cdk.service_quotas.egg-info/requires.txt
 src/reapit_cdk.service_quotas.egg-info/top_level.txt
 src/reapit_cdk/service_quotas/__init__.py
 src/reapit_cdk/service_quotas/py.typed
 src/reapit_cdk/service_quotas/_jsii/__init__.py
-src/reapit_cdk/service_quotas/_jsii/service-quotas@0.1.0.jsii.tgz
+src/reapit_cdk/service_quotas/_jsii/service-quotas@0.1.2.jsii.tgz
```

