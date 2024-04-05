# Comparing `tmp/reapit-cdk.reapit-product-0.1.0.tar.gz` & `tmp/reapit-cdk.reapit-product-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reapit-cdk.reapit-product-0.1.0.tar", last modified: Tue Apr  2 13:01:10 2024, max compression
+gzip compressed data, was "reapit-cdk.reapit-product-0.1.2.tar", last modified: Fri Apr  5 10:28:58 2024, max compression
```

## Comparing `reapit-cdk.reapit-product-0.1.0.tar` & `reapit-cdk.reapit-product-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:01:10.325507 reapit-cdk.reapit-product-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-02 13:01:04.000000 reapit-cdk.reapit-product-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 13:01:04.000000 reapit-cdk.reapit-product-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-02 13:01:10.325507 reapit-cdk.reapit-product-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-02 13:01:04.000000 reapit-cdk.reapit-product-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-02 13:01:04.000000 reapit-cdk.reapit-product-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 13:01:10.325507 reapit-cdk.reapit-product-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-02 13:01:04.000000 reapit-cdk.reapit-product-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:01:10.321507 reapit-cdk.reapit-product-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:01:10.321507 reapit-cdk.reapit-product-0.1.0/src/reapit_cdk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:01:10.325507 reapit-cdk.reapit-product-0.1.0/src/reapit_cdk/reapit_product/
--rw-r--r--   0 runner    (1001) docker     (127)    20683 2024-04-02 13:01:04.000000 reapit-cdk.reapit-product-0.1.0/src/reapit_cdk/reapit_product/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:01:10.325507 reapit-cdk.reapit-product-0.1.0/src/reapit_cdk/reapit_product/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-02 13:01:04.000000 reapit-cdk.reapit-product-0.1.0/src/reapit_cdk/reapit_product/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   120069 2024-04-02 13:01:04.000000 reapit-cdk.reapit-product-0.1.0/src/reapit_cdk/reapit_product/_jsii/reapit-product@0.1.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:01:04.000000 reapit-cdk.reapit-product-0.1.0/src/reapit_cdk/reapit_product/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:01:10.325507 reapit-cdk.reapit-product-0.1.0/src/reapit_cdk.reapit_product.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-02 13:01:10.000000 reapit-cdk.reapit-product-0.1.0/src/reapit_cdk.reapit_product.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-02 13:01:10.000000 reapit-cdk.reapit-product-0.1.0/src/reapit_cdk.reapit_product.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:01:10.000000 reapit-cdk.reapit-product-0.1.0/src/reapit_cdk.reapit_product.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 13:01:10.000000 reapit-cdk.reapit-product-0.1.0/src/reapit_cdk.reapit_product.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 13:01:10.000000 reapit-cdk.reapit-product-0.1.0/src/reapit_cdk.reapit_product.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:28:58.221567 reapit-cdk.reapit-product-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-05 10:28:51.000000 reapit-cdk.reapit-product-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-05 10:28:51.000000 reapit-cdk.reapit-product-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-05 10:28:58.221567 reapit-cdk.reapit-product-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-05 10:28:51.000000 reapit-cdk.reapit-product-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-05 10:28:51.000000 reapit-cdk.reapit-product-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 10:28:58.221567 reapit-cdk.reapit-product-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-05 10:28:51.000000 reapit-cdk.reapit-product-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:28:58.217567 reapit-cdk.reapit-product-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:28:58.217567 reapit-cdk.reapit-product-0.1.2/src/reapit_cdk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:28:58.217567 reapit-cdk.reapit-product-0.1.2/src/reapit_cdk/reapit_product/
+-rw-r--r--   0 runner    (1001) docker     (127)    20683 2024-04-05 10:28:51.000000 reapit-cdk.reapit-product-0.1.2/src/reapit_cdk/reapit_product/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:28:58.221567 reapit-cdk.reapit-product-0.1.2/src/reapit_cdk/reapit_product/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-05 10:28:51.000000 reapit-cdk.reapit-product-0.1.2/src/reapit_cdk/reapit_product/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119021 2024-04-05 10:28:51.000000 reapit-cdk.reapit-product-0.1.2/src/reapit_cdk/reapit_product/_jsii/reapit-product@0.1.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 10:28:51.000000 reapit-cdk.reapit-product-0.1.2/src/reapit_cdk/reapit_product/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:28:58.217567 reapit-cdk.reapit-product-0.1.2/src/reapit_cdk.reapit_product.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-05 10:28:58.000000 reapit-cdk.reapit-product-0.1.2/src/reapit_cdk.reapit_product.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-05 10:28:58.000000 reapit-cdk.reapit-product-0.1.2/src/reapit_cdk.reapit_product.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 10:28:58.000000 reapit-cdk.reapit-product-0.1.2/src/reapit_cdk.reapit_product.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-05 10:28:58.000000 reapit-cdk.reapit-product-0.1.2/src/reapit_cdk.reapit_product.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 10:28:58.000000 reapit-cdk.reapit-product-0.1.2/src/reapit_cdk.reapit_product.egg-info/top_level.txt
```

### Comparing `reapit-cdk.reapit-product-0.1.0/LICENSE` & `reapit-cdk.reapit-product-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reapit-cdk.reapit-product-0.1.0/PKG-INFO` & `reapit-cdk.reapit-product-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reapit-cdk.reapit-product
-Version: 0.1.0
+Version: 0.1.2
 Summary: Creates a product in the organisations service
 Home-page: https://github.com/reapit/ts-cdk-constructs/blob/main/packages/constructs/reapit-product
 Author: Josh Balfour<jbalfour@reapit.com>
 License: MIT
 Project-URL: Source, https://github.com/reapit/ts-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `reapit-cdk.reapit-product-0.1.0/README.md` & `reapit-cdk.reapit-product-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `reapit-cdk.reapit-product-0.1.0/setup.py` & `reapit-cdk.reapit-product-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "reapit-cdk.reapit-product",
-    "version": "0.1.0",
+    "version": "0.1.2",
     "description": "Creates a product in the organisations service",
     "license": "MIT",
     "url": "https://github.com/reapit/ts-cdk-constructs/blob/main/packages/constructs/reapit-product",
     "long_description_content_type": "text/markdown",
     "author": "Josh Balfour<jbalfour@reapit.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "reapit_cdk.reapit_product",
         "reapit_cdk.reapit_product._jsii"
     ],
     "package_data": {
         "reapit_cdk.reapit_product._jsii": [
-            "reapit-product@0.1.0.jsii.tgz"
+            "reapit-product@0.1.2.jsii.tgz"
         ],
         "reapit_cdk.reapit_product": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `reapit-cdk.reapit-product-0.1.0/src/reapit_cdk/reapit_product/__init__.py` & `reapit-cdk.reapit-product-0.1.2/src/reapit_cdk/reapit_product/__init__.py`

 * *Files identical despite different names*

### Comparing `reapit-cdk.reapit-product-0.1.0/src/reapit_cdk.reapit_product.egg-info/PKG-INFO` & `reapit-cdk.reapit-product-0.1.2/src/reapit_cdk.reapit_product.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reapit-cdk.reapit-product
-Version: 0.1.0
+Version: 0.1.2
 Summary: Creates a product in the organisations service
 Home-page: https://github.com/reapit/ts-cdk-constructs/blob/main/packages/constructs/reapit-product
 Author: Josh Balfour<jbalfour@reapit.com>
 License: MIT
 Project-URL: Source, https://github.com/reapit/ts-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `reapit-cdk.reapit-product-0.1.0/src/reapit_cdk.reapit_product.egg-info/SOURCES.txt` & `reapit-cdk.reapit-product-0.1.2/src/reapit_cdk.reapit_product.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/reapit_cdk.reapit_product.egg-info/SOURCES.txt
 src/reapit_cdk.reapit_product.egg-info/dependency_links.txt
 src/reapit_cdk.reapit_product.egg-info/requires.txt
 src/reapit_cdk.reapit_product.egg-info/top_level.txt
 src/reapit_cdk/reapit_product/__init__.py
 src/reapit_cdk/reapit_product/py.typed
 src/reapit_cdk/reapit_product/_jsii/__init__.py
-src/reapit_cdk/reapit_product/_jsii/reapit-product@0.1.0.jsii.tgz
+src/reapit_cdk/reapit_product/_jsii/reapit-product@0.1.2.jsii.tgz
```

