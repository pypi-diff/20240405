# Comparing `tmp/reapit-cdk.active-ruleset-0.1.0.tar.gz` & `tmp/reapit-cdk.active-ruleset-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reapit-cdk.active-ruleset-0.1.0.tar", last modified: Tue Apr  2 11:21:26 2024, max compression
+gzip compressed data, was "reapit-cdk.active-ruleset-0.1.1.tar", last modified: Thu Apr  4 14:59:26 2024, max compression
```

## Comparing `reapit-cdk.active-ruleset-0.1.0.tar` & `reapit-cdk.active-ruleset-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:21:26.414391 reapit-cdk.active-ruleset-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-02 11:21:19.000000 reapit-cdk.active-ruleset-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 11:21:19.000000 reapit-cdk.active-ruleset-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-02 11:21:26.414391 reapit-cdk.active-ruleset-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-02 11:21:19.000000 reapit-cdk.active-ruleset-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-02 11:21:19.000000 reapit-cdk.active-ruleset-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 11:21:26.414391 reapit-cdk.active-ruleset-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-02 11:21:19.000000 reapit-cdk.active-ruleset-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:21:26.410391 reapit-cdk.active-ruleset-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:21:26.410391 reapit-cdk.active-ruleset-0.1.0/src/reapit_cdk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:21:26.414391 reapit-cdk.active-ruleset-0.1.0/src/reapit_cdk/active_ruleset/
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-02 11:21:19.000000 reapit-cdk.active-ruleset-0.1.0/src/reapit_cdk/active_ruleset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:21:26.414391 reapit-cdk.active-ruleset-0.1.0/src/reapit_cdk/active_ruleset/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-02 11:21:19.000000 reapit-cdk.active-ruleset-0.1.0/src/reapit_cdk/active_ruleset/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   105712 2024-04-02 11:21:19.000000 reapit-cdk.active-ruleset-0.1.0/src/reapit_cdk/active_ruleset/_jsii/active-ruleset@0.1.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 11:21:19.000000 reapit-cdk.active-ruleset-0.1.0/src/reapit_cdk/active_ruleset/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:21:26.414391 reapit-cdk.active-ruleset-0.1.0/src/reapit_cdk.active_ruleset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-02 11:21:26.000000 reapit-cdk.active-ruleset-0.1.0/src/reapit_cdk.active_ruleset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-02 11:21:26.000000 reapit-cdk.active-ruleset-0.1.0/src/reapit_cdk.active_ruleset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 11:21:26.000000 reapit-cdk.active-ruleset-0.1.0/src/reapit_cdk.active_ruleset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 11:21:26.000000 reapit-cdk.active-ruleset-0.1.0/src/reapit_cdk.active_ruleset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 11:21:26.000000 reapit-cdk.active-ruleset-0.1.0/src/reapit_cdk.active_ruleset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:59:26.822181 reapit-cdk.active-ruleset-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-04 14:59:19.000000 reapit-cdk.active-ruleset-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-04 14:59:19.000000 reapit-cdk.active-ruleset-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-04 14:59:26.822181 reapit-cdk.active-ruleset-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-04 14:59:19.000000 reapit-cdk.active-ruleset-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-04 14:59:19.000000 reapit-cdk.active-ruleset-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:59:26.822181 reapit-cdk.active-ruleset-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-04 14:59:19.000000 reapit-cdk.active-ruleset-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:59:26.818181 reapit-cdk.active-ruleset-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:59:26.818181 reapit-cdk.active-ruleset-0.1.1/src/reapit_cdk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:59:26.818181 reapit-cdk.active-ruleset-0.1.1/src/reapit_cdk/active_ruleset/
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-04 14:59:19.000000 reapit-cdk.active-ruleset-0.1.1/src/reapit_cdk/active_ruleset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:59:26.822181 reapit-cdk.active-ruleset-0.1.1/src/reapit_cdk/active_ruleset/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-04 14:59:19.000000 reapit-cdk.active-ruleset-0.1.1/src/reapit_cdk/active_ruleset/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104989 2024-04-04 14:59:19.000000 reapit-cdk.active-ruleset-0.1.1/src/reapit_cdk/active_ruleset/_jsii/active-ruleset@0.1.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:59:19.000000 reapit-cdk.active-ruleset-0.1.1/src/reapit_cdk/active_ruleset/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:59:26.818181 reapit-cdk.active-ruleset-0.1.1/src/reapit_cdk.active_ruleset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-04 14:59:26.000000 reapit-cdk.active-ruleset-0.1.1/src/reapit_cdk.active_ruleset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-04 14:59:26.000000 reapit-cdk.active-ruleset-0.1.1/src/reapit_cdk.active_ruleset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:59:26.000000 reapit-cdk.active-ruleset-0.1.1/src/reapit_cdk.active_ruleset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-04 14:59:26.000000 reapit-cdk.active-ruleset-0.1.1/src/reapit_cdk.active_ruleset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 14:59:26.000000 reapit-cdk.active-ruleset-0.1.1/src/reapit_cdk.active_ruleset.egg-info/top_level.txt
```

### Comparing `reapit-cdk.active-ruleset-0.1.0/LICENSE` & `reapit-cdk.active-ruleset-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reapit-cdk.active-ruleset-0.1.0/PKG-INFO` & `reapit-cdk.active-ruleset-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reapit-cdk.active-ruleset
-Version: 0.1.0
+Version: 0.1.1
 Summary: This construct returns the currently active SES receipt RuleSet, or creates one. This enables you to add rules to it.
 Home-page: https://github.com/reapit/ts-cdk-constructs/blob/main/packages/constructs/active-ruleset
 Author: Josh Balfour<jbalfour@reapit.com>
 License: MIT
 Project-URL: Source, https://github.com/reapit/ts-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `reapit-cdk.active-ruleset-0.1.0/README.md` & `reapit-cdk.active-ruleset-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `reapit-cdk.active-ruleset-0.1.0/setup.py` & `reapit-cdk.active-ruleset-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "reapit-cdk.active-ruleset",
-    "version": "0.1.0",
+    "version": "0.1.1",
     "description": "This construct returns the currently active SES receipt RuleSet, or creates one. This enables you to add rules to it.",
     "license": "MIT",
     "url": "https://github.com/reapit/ts-cdk-constructs/blob/main/packages/constructs/active-ruleset",
     "long_description_content_type": "text/markdown",
     "author": "Josh Balfour<jbalfour@reapit.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "reapit_cdk.active_ruleset",
         "reapit_cdk.active_ruleset._jsii"
     ],
     "package_data": {
         "reapit_cdk.active_ruleset._jsii": [
-            "active-ruleset@0.1.0.jsii.tgz"
+            "active-ruleset@0.1.1.jsii.tgz"
         ],
         "reapit_cdk.active_ruleset": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `reapit-cdk.active-ruleset-0.1.0/src/reapit_cdk/active_ruleset/__init__.py` & `reapit-cdk.active-ruleset-0.1.1/src/reapit_cdk/active_ruleset/__init__.py`

 * *Files identical despite different names*

### Comparing `reapit-cdk.active-ruleset-0.1.0/src/reapit_cdk.active_ruleset.egg-info/PKG-INFO` & `reapit-cdk.active-ruleset-0.1.1/src/reapit_cdk.active_ruleset.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reapit-cdk.active-ruleset
-Version: 0.1.0
+Version: 0.1.1
 Summary: This construct returns the currently active SES receipt RuleSet, or creates one. This enables you to add rules to it.
 Home-page: https://github.com/reapit/ts-cdk-constructs/blob/main/packages/constructs/active-ruleset
 Author: Josh Balfour<jbalfour@reapit.com>
 License: MIT
 Project-URL: Source, https://github.com/reapit/ts-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `reapit-cdk.active-ruleset-0.1.0/src/reapit_cdk.active_ruleset.egg-info/SOURCES.txt` & `reapit-cdk.active-ruleset-0.1.1/src/reapit_cdk.active_ruleset.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/reapit_cdk.active_ruleset.egg-info/SOURCES.txt
 src/reapit_cdk.active_ruleset.egg-info/dependency_links.txt
 src/reapit_cdk.active_ruleset.egg-info/requires.txt
 src/reapit_cdk.active_ruleset.egg-info/top_level.txt
 src/reapit_cdk/active_ruleset/__init__.py
 src/reapit_cdk/active_ruleset/py.typed
 src/reapit_cdk/active_ruleset/_jsii/__init__.py
-src/reapit_cdk/active_ruleset/_jsii/active-ruleset@0.1.0.jsii.tgz
+src/reapit_cdk/active_ruleset/_jsii/active-ruleset@0.1.1.jsii.tgz
```

