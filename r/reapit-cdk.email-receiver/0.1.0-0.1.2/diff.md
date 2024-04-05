# Comparing `tmp/reapit-cdk.email-receiver-0.1.0.tar.gz` & `tmp/reapit-cdk.email-receiver-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reapit-cdk.email-receiver-0.1.0.tar", last modified: Tue Apr  2 13:26:28 2024, max compression
+gzip compressed data, was "reapit-cdk.email-receiver-0.1.2.tar", last modified: Fri Apr  5 10:27:39 2024, max compression
```

## Comparing `reapit-cdk.email-receiver-0.1.0.tar` & `reapit-cdk.email-receiver-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:26:28.351308 reapit-cdk.email-receiver-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-02 13:26:22.000000 reapit-cdk.email-receiver-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 13:26:22.000000 reapit-cdk.email-receiver-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-02 13:26:28.351308 reapit-cdk.email-receiver-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-02 13:26:22.000000 reapit-cdk.email-receiver-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-02 13:26:22.000000 reapit-cdk.email-receiver-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 13:26:28.351308 reapit-cdk.email-receiver-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-02 13:26:22.000000 reapit-cdk.email-receiver-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:26:28.347308 reapit-cdk.email-receiver-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:26:28.347308 reapit-cdk.email-receiver-0.1.0/src/reapit_cdk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:26:28.351308 reapit-cdk.email-receiver-0.1.0/src/reapit_cdk/email_receiver/
--rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-04-02 13:26:22.000000 reapit-cdk.email-receiver-0.1.0/src/reapit_cdk/email_receiver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:26:28.351308 reapit-cdk.email-receiver-0.1.0/src/reapit_cdk/email_receiver/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-02 13:26:22.000000 reapit-cdk.email-receiver-0.1.0/src/reapit_cdk/email_receiver/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   588033 2024-04-02 13:26:22.000000 reapit-cdk.email-receiver-0.1.0/src/reapit_cdk/email_receiver/_jsii/email-receiver@0.1.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:26:22.000000 reapit-cdk.email-receiver-0.1.0/src/reapit_cdk/email_receiver/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:26:28.351308 reapit-cdk.email-receiver-0.1.0/src/reapit_cdk.email_receiver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-02 13:26:28.000000 reapit-cdk.email-receiver-0.1.0/src/reapit_cdk.email_receiver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-02 13:26:28.000000 reapit-cdk.email-receiver-0.1.0/src/reapit_cdk.email_receiver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:26:28.000000 reapit-cdk.email-receiver-0.1.0/src/reapit_cdk.email_receiver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-02 13:26:28.000000 reapit-cdk.email-receiver-0.1.0/src/reapit_cdk.email_receiver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 13:26:28.000000 reapit-cdk.email-receiver-0.1.0/src/reapit_cdk.email_receiver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:27:39.869251 reapit-cdk.email-receiver-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-05 10:27:34.000000 reapit-cdk.email-receiver-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-05 10:27:34.000000 reapit-cdk.email-receiver-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-05 10:27:39.869251 reapit-cdk.email-receiver-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-05 10:27:34.000000 reapit-cdk.email-receiver-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-05 10:27:34.000000 reapit-cdk.email-receiver-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 10:27:39.869251 reapit-cdk.email-receiver-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-05 10:27:34.000000 reapit-cdk.email-receiver-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:27:39.865251 reapit-cdk.email-receiver-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:27:39.865251 reapit-cdk.email-receiver-0.1.2/src/reapit_cdk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:27:39.869251 reapit-cdk.email-receiver-0.1.2/src/reapit_cdk/email_receiver/
+-rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-04-05 10:27:34.000000 reapit-cdk.email-receiver-0.1.2/src/reapit_cdk/email_receiver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:27:39.869251 reapit-cdk.email-receiver-0.1.2/src/reapit_cdk/email_receiver/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-05 10:27:34.000000 reapit-cdk.email-receiver-0.1.2/src/reapit_cdk/email_receiver/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   586334 2024-04-05 10:27:34.000000 reapit-cdk.email-receiver-0.1.2/src/reapit_cdk/email_receiver/_jsii/email-receiver@0.1.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 10:27:34.000000 reapit-cdk.email-receiver-0.1.2/src/reapit_cdk/email_receiver/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:27:39.865251 reapit-cdk.email-receiver-0.1.2/src/reapit_cdk.email_receiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-05 10:27:39.000000 reapit-cdk.email-receiver-0.1.2/src/reapit_cdk.email_receiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-05 10:27:39.000000 reapit-cdk.email-receiver-0.1.2/src/reapit_cdk.email_receiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 10:27:39.000000 reapit-cdk.email-receiver-0.1.2/src/reapit_cdk.email_receiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-05 10:27:39.000000 reapit-cdk.email-receiver-0.1.2/src/reapit_cdk.email_receiver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 10:27:39.000000 reapit-cdk.email-receiver-0.1.2/src/reapit_cdk.email_receiver.egg-info/top_level.txt
```

### Comparing `reapit-cdk.email-receiver-0.1.0/LICENSE` & `reapit-cdk.email-receiver-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reapit-cdk.email-receiver-0.1.0/PKG-INFO` & `reapit-cdk.email-receiver-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reapit-cdk.email-receiver
-Version: 0.1.0
+Version: 0.1.2
 Summary: This construct sets up everything necessary to receive email. The emails get stored in a dynamodb table, queryable by recipient. This is designed to be used in end-to-end tests, with the [@reapit-cdk/email-receiver-client](../../libs/email-receiver-client) helper library.
 Home-page: https://github.com/reapit/ts-cdk-constructs/blob/main/packages/constructs/email-receiver
 Author: Josh Balfour<jbalfour@reapit.com>
 License: MIT
 Project-URL: Source, https://github.com/reapit/ts-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `reapit-cdk.email-receiver-0.1.0/README.md` & `reapit-cdk.email-receiver-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `reapit-cdk.email-receiver-0.1.0/setup.py` & `reapit-cdk.email-receiver-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "reapit-cdk.email-receiver",
-    "version": "0.1.0",
+    "version": "0.1.2",
     "description": "This construct sets up everything necessary to receive email. The emails get stored in a dynamodb table, queryable by recipient. This is designed to be used in end-to-end tests, with the [@reapit-cdk/email-receiver-client](../../libs/email-receiver-client) helper library.",
     "license": "MIT",
     "url": "https://github.com/reapit/ts-cdk-constructs/blob/main/packages/constructs/email-receiver",
     "long_description_content_type": "text/markdown",
     "author": "Josh Balfour<jbalfour@reapit.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,27 +22,27 @@
     },
     "packages": [
         "reapit_cdk.email_receiver",
         "reapit_cdk.email_receiver._jsii"
     ],
     "package_data": {
         "reapit_cdk.email_receiver._jsii": [
-            "email-receiver@0.1.0.jsii.tgz"
+            "email-receiver@0.1.2.jsii.tgz"
         ],
         "reapit_cdk.email_receiver": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.96.2, <3.0.0",
         "constructs>=10.2.70, <11.0.0",
         "jsii>=1.94.0, <2.0.0",
         "publication>=0.0.3",
-        "reapit-cdk.active-ruleset>=0.1.0, <0.2.0",
+        "reapit-cdk.active-ruleset>=0.1.2, <0.2.0",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
```

### Comparing `reapit-cdk.email-receiver-0.1.0/src/reapit_cdk/email_receiver/__init__.py` & `reapit-cdk.email-receiver-0.1.2/src/reapit_cdk/email_receiver/__init__.py`

 * *Files identical despite different names*

### Comparing `reapit-cdk.email-receiver-0.1.0/src/reapit_cdk.email_receiver.egg-info/PKG-INFO` & `reapit-cdk.email-receiver-0.1.2/src/reapit_cdk.email_receiver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reapit-cdk.email-receiver
-Version: 0.1.0
+Version: 0.1.2
 Summary: This construct sets up everything necessary to receive email. The emails get stored in a dynamodb table, queryable by recipient. This is designed to be used in end-to-end tests, with the [@reapit-cdk/email-receiver-client](../../libs/email-receiver-client) helper library.
 Home-page: https://github.com/reapit/ts-cdk-constructs/blob/main/packages/constructs/email-receiver
 Author: Josh Balfour<jbalfour@reapit.com>
 License: MIT
 Project-URL: Source, https://github.com/reapit/ts-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `reapit-cdk.email-receiver-0.1.0/src/reapit_cdk.email_receiver.egg-info/SOURCES.txt` & `reapit-cdk.email-receiver-0.1.2/src/reapit_cdk.email_receiver.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/reapit_cdk.email_receiver.egg-info/SOURCES.txt
 src/reapit_cdk.email_receiver.egg-info/dependency_links.txt
 src/reapit_cdk.email_receiver.egg-info/requires.txt
 src/reapit_cdk.email_receiver.egg-info/top_level.txt
 src/reapit_cdk/email_receiver/__init__.py
 src/reapit_cdk/email_receiver/py.typed
 src/reapit_cdk/email_receiver/_jsii/__init__.py
-src/reapit_cdk/email_receiver/_jsii/email-receiver@0.1.0.jsii.tgz
+src/reapit_cdk/email_receiver/_jsii/email-receiver@0.1.2.jsii.tgz
```

