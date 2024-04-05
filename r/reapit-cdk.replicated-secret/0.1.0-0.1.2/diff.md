# Comparing `tmp/reapit-cdk.replicated-secret-0.1.0.tar.gz` & `tmp/reapit-cdk.replicated-secret-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reapit-cdk.replicated-secret-0.1.0.tar", last modified: Tue Apr  2 12:56:39 2024, max compression
+gzip compressed data, was "reapit-cdk.replicated-secret-0.1.2.tar", last modified: Fri Apr  5 10:33:58 2024, max compression
```

## Comparing `reapit-cdk.replicated-secret-0.1.0.tar` & `reapit-cdk.replicated-secret-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:56:39.026105 reapit-cdk.replicated-secret-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-02 12:56:33.000000 reapit-cdk.replicated-secret-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 12:56:33.000000 reapit-cdk.replicated-secret-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-02 12:56:39.026105 reapit-cdk.replicated-secret-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-02 12:56:33.000000 reapit-cdk.replicated-secret-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-02 12:56:33.000000 reapit-cdk.replicated-secret-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 12:56:39.026105 reapit-cdk.replicated-secret-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-02 12:56:33.000000 reapit-cdk.replicated-secret-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:56:39.022105 reapit-cdk.replicated-secret-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:56:39.022105 reapit-cdk.replicated-secret-0.1.0/src/reapit_cdk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:56:39.026105 reapit-cdk.replicated-secret-0.1.0/src/reapit_cdk/replicated_secret/
--rw-r--r--   0 runner    (1001) docker     (127)    12581 2024-04-02 12:56:33.000000 reapit-cdk.replicated-secret-0.1.0/src/reapit_cdk/replicated_secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:56:39.026105 reapit-cdk.replicated-secret-0.1.0/src/reapit_cdk/replicated_secret/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-02 12:56:33.000000 reapit-cdk.replicated-secret-0.1.0/src/reapit_cdk/replicated_secret/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   112211 2024-04-02 12:56:33.000000 reapit-cdk.replicated-secret-0.1.0/src/reapit_cdk/replicated_secret/_jsii/replicated-secret@0.1.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:56:33.000000 reapit-cdk.replicated-secret-0.1.0/src/reapit_cdk/replicated_secret/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:56:39.026105 reapit-cdk.replicated-secret-0.1.0/src/reapit_cdk.replicated_secret.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-02 12:56:38.000000 reapit-cdk.replicated-secret-0.1.0/src/reapit_cdk.replicated_secret.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-02 12:56:39.000000 reapit-cdk.replicated-secret-0.1.0/src/reapit_cdk.replicated_secret.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:56:38.000000 reapit-cdk.replicated-secret-0.1.0/src/reapit_cdk.replicated_secret.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-02 12:56:38.000000 reapit-cdk.replicated-secret-0.1.0/src/reapit_cdk.replicated_secret.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 12:56:38.000000 reapit-cdk.replicated-secret-0.1.0/src/reapit_cdk.replicated_secret.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:33:58.795875 reapit-cdk.replicated-secret-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-05 10:33:53.000000 reapit-cdk.replicated-secret-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-05 10:33:53.000000 reapit-cdk.replicated-secret-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-05 10:33:58.795875 reapit-cdk.replicated-secret-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-05 10:33:53.000000 reapit-cdk.replicated-secret-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-05 10:33:53.000000 reapit-cdk.replicated-secret-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 10:33:58.795875 reapit-cdk.replicated-secret-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-05 10:33:53.000000 reapit-cdk.replicated-secret-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:33:58.791875 reapit-cdk.replicated-secret-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:33:58.791875 reapit-cdk.replicated-secret-0.1.2/src/reapit_cdk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:33:58.791875 reapit-cdk.replicated-secret-0.1.2/src/reapit_cdk/replicated_secret/
+-rw-r--r--   0 runner    (1001) docker     (127)    12581 2024-04-05 10:33:53.000000 reapit-cdk.replicated-secret-0.1.2/src/reapit_cdk/replicated_secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:33:58.795875 reapit-cdk.replicated-secret-0.1.2/src/reapit_cdk/replicated_secret/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-05 10:33:53.000000 reapit-cdk.replicated-secret-0.1.2/src/reapit_cdk/replicated_secret/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   110852 2024-04-05 10:33:53.000000 reapit-cdk.replicated-secret-0.1.2/src/reapit_cdk/replicated_secret/_jsii/replicated-secret@0.1.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 10:33:53.000000 reapit-cdk.replicated-secret-0.1.2/src/reapit_cdk/replicated_secret/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:33:58.791875 reapit-cdk.replicated-secret-0.1.2/src/reapit_cdk.replicated_secret.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-05 10:33:58.000000 reapit-cdk.replicated-secret-0.1.2/src/reapit_cdk.replicated_secret.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-05 10:33:58.000000 reapit-cdk.replicated-secret-0.1.2/src/reapit_cdk.replicated_secret.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 10:33:58.000000 reapit-cdk.replicated-secret-0.1.2/src/reapit_cdk.replicated_secret.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-05 10:33:58.000000 reapit-cdk.replicated-secret-0.1.2/src/reapit_cdk.replicated_secret.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 10:33:58.000000 reapit-cdk.replicated-secret-0.1.2/src/reapit_cdk.replicated_secret.egg-info/top_level.txt
```

### Comparing `reapit-cdk.replicated-secret-0.1.0/LICENSE` & `reapit-cdk.replicated-secret-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reapit-cdk.replicated-secret-0.1.0/PKG-INFO` & `reapit-cdk.replicated-secret-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reapit-cdk.replicated-secret
-Version: 0.1.0
+Version: 0.1.2
 Summary: Creates a Secret and replicates it across the given regions. Requires a [ReplicatedKey](../replicated-key/readme.md) be passed in.
 Home-page: https://github.com/reapit/ts-cdk-constructs/blob/main/packages/constructs/replicated-secret
 Author: Josh Balfour<jbalfour@reapit.com>
 License: MIT
 Project-URL: Source, https://github.com/reapit/ts-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `reapit-cdk.replicated-secret-0.1.0/README.md` & `reapit-cdk.replicated-secret-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `reapit-cdk.replicated-secret-0.1.0/setup.py` & `reapit-cdk.replicated-secret-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "reapit-cdk.replicated-secret",
-    "version": "0.1.0",
+    "version": "0.1.2",
     "description": "Creates a Secret and replicates it across the given regions. Requires a [ReplicatedKey](../replicated-key/readme.md) be passed in.",
     "license": "MIT",
     "url": "https://github.com/reapit/ts-cdk-constructs/blob/main/packages/constructs/replicated-secret",
     "long_description_content_type": "text/markdown",
     "author": "Josh Balfour<jbalfour@reapit.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,27 +22,27 @@
     },
     "packages": [
         "reapit_cdk.replicated_secret",
         "reapit_cdk.replicated_secret._jsii"
     ],
     "package_data": {
         "reapit_cdk.replicated_secret._jsii": [
-            "replicated-secret@0.1.0.jsii.tgz"
+            "replicated-secret@0.1.2.jsii.tgz"
         ],
         "reapit_cdk.replicated_secret": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.96.2, <3.0.0",
         "constructs>=10.2.70, <11.0.0",
         "jsii>=1.94.0, <2.0.0",
         "publication>=0.0.3",
-        "reapit-cdk.replicated-key>=0.1.0, <0.2.0",
+        "reapit-cdk.replicated-key>=0.1.2, <0.2.0",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
```

### Comparing `reapit-cdk.replicated-secret-0.1.0/src/reapit_cdk/replicated_secret/__init__.py` & `reapit-cdk.replicated-secret-0.1.2/src/reapit_cdk/replicated_secret/__init__.py`

 * *Files identical despite different names*

### Comparing `reapit-cdk.replicated-secret-0.1.0/src/reapit_cdk.replicated_secret.egg-info/PKG-INFO` & `reapit-cdk.replicated-secret-0.1.2/src/reapit_cdk.replicated_secret.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reapit-cdk.replicated-secret
-Version: 0.1.0
+Version: 0.1.2
 Summary: Creates a Secret and replicates it across the given regions. Requires a [ReplicatedKey](../replicated-key/readme.md) be passed in.
 Home-page: https://github.com/reapit/ts-cdk-constructs/blob/main/packages/constructs/replicated-secret
 Author: Josh Balfour<jbalfour@reapit.com>
 License: MIT
 Project-URL: Source, https://github.com/reapit/ts-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `reapit-cdk.replicated-secret-0.1.0/src/reapit_cdk.replicated_secret.egg-info/SOURCES.txt` & `reapit-cdk.replicated-secret-0.1.2/src/reapit_cdk.replicated_secret.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/reapit_cdk.replicated_secret.egg-info/SOURCES.txt
 src/reapit_cdk.replicated_secret.egg-info/dependency_links.txt
 src/reapit_cdk.replicated_secret.egg-info/requires.txt
 src/reapit_cdk.replicated_secret.egg-info/top_level.txt
 src/reapit_cdk/replicated_secret/__init__.py
 src/reapit_cdk/replicated_secret/py.typed
 src/reapit_cdk/replicated_secret/_jsii/__init__.py
-src/reapit_cdk/replicated_secret/_jsii/replicated-secret@0.1.0.jsii.tgz
+src/reapit_cdk/replicated_secret/_jsii/replicated-secret@0.1.2.jsii.tgz
```

