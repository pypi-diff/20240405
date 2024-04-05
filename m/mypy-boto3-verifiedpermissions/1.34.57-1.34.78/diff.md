# Comparing `tmp/mypy-boto3-verifiedpermissions-1.34.57.tar.gz` & `tmp/mypy-boto3-verifiedpermissions-1.34.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-verifiedpermissions-1.34.57.tar", last modified: Wed Mar  6 21:33:28 2024, max compression
+gzip compressed data, was "mypy-boto3-verifiedpermissions-1.34.78.tar", last modified: Thu Apr  4 19:33:18 2024, max compression
```

## Comparing `mypy-boto3-verifiedpermissions-1.34.57.tar` & `mypy-boto3-verifiedpermissions-1.34.78.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:33:28.664245 mypy-boto3-verifiedpermissions-1.34.57/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-06 21:33:16.000000 mypy-boto3-verifiedpermissions-1.34.57/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13815 2024-03-06 21:33:28.664245 mypy-boto3-verifiedpermissions-1.34.57/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12212 2024-03-06 21:33:16.000000 mypy-boto3-verifiedpermissions-1.34.57/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:33:28.664245 mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions/
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-06 21:33:16.000000 mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-06 21:33:16.000000 mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-03-06 21:33:16.000000 mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22033 2024-03-06 21:33:16.000000 mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    22030 2024-03-06 21:33:16.000000 mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-03-06 21:33:16.000000 mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-03-06 21:33:16.000000 mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-03-06 21:33:16.000000 mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-03-06 21:33:16.000000 mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 21:33:16.000000 mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    26571 2024-03-06 21:33:17.000000 mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    26571 2024-03-06 21:33:16.000000 mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-06 21:33:16.000000 mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:33:28.664245 mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13815 2024-03-06 21:33:28.000000 mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-06 21:33:28.000000 mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 21:33:28.000000 mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 21:33:28.000000 mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-06 21:33:28.000000 mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-06 21:33:28.000000 mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 21:33:28.664245 mypy-boto3-verifiedpermissions-1.34.57/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-03-06 21:33:16.000000 mypy-boto3-verifiedpermissions-1.34.57/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:18.128019 mypy-boto3-verifiedpermissions-1.34.78/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-04 19:33:03.000000 mypy-boto3-verifiedpermissions-1.34.78/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13815 2024-04-04 19:33:18.128019 mypy-boto3-verifiedpermissions-1.34.78/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12212 2024-04-04 19:33:03.000000 mypy-boto3-verifiedpermissions-1.34.78/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:18.124019 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-04 19:33:03.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-04 19:33:03.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-04 19:33:03.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22033 2024-04-04 19:33:04.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22030 2024-04-04 19:33:04.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-04-04 19:33:04.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-04-04 19:33:04.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-04 19:33:04.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-04 19:33:04.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:03.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    27707 2024-04-04 19:33:05.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27707 2024-04-04 19:33:05.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-04 19:33:03.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:18.128019 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13815 2024-04-04 19:33:18.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-04 19:33:18.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:33:18.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:33:18.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-04 19:33:18.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-04 19:33:18.000000 mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 19:33:18.128019 mypy-boto3-verifiedpermissions-1.34.78/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-04 19:33:03.000000 mypy-boto3-verifiedpermissions-1.34.78/setup.py
```

### Comparing `mypy-boto3-verifiedpermissions-1.34.57/LICENSE` & `mypy-boto3-verifiedpermissions-1.34.78/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.34.57/PKG-INFO` & `mypy-boto3-verifiedpermissions-1.34.78/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-verifiedpermissions
-Version: 1.34.57
-Summary: Type annotations for boto3.VerifiedPermissions 1.34.57 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.78
+Summary: Type annotations for boto3.VerifiedPermissions 1.34.78 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-verifiedpermissions.svg?color=blue)](https://pypi.org/project/mypy-boto3-verifiedpermissions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-verifiedpermissions)](https://pepy.tech/project/mypy-boto3-verifiedpermissions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VerifiedPermissions 1.34.57](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
+[boto3.VerifiedPermissions 1.34.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-verifiedpermissions-1.34.57/README.md` & `mypy-boto3-verifiedpermissions-1.34.78/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-verifiedpermissions.svg?color=blue)](https://pypi.org/project/mypy-boto3-verifiedpermissions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-verifiedpermissions)](https://pepy.tech/project/mypy-boto3-verifiedpermissions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VerifiedPermissions 1.34.57](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
+[boto3.VerifiedPermissions 1.34.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions/__init__.py` & `mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions/__init__.pyi` & `mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions/__main__.py` & `mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.VerifiedPermissions 1.34.57\n"
-        "Version:         1.34.57\n"
+        "Type annotations for boto3.VerifiedPermissions 1.34.78\n"
+        "Version:         1.34.78\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.57")
+    print("1.34.78")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions/client.py` & `mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions/client.pyi` & `mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions/literals.py` & `mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -141,14 +142,15 @@
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -209,15 +211,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -397,14 +398,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions/literals.pyi` & `mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -141,14 +142,15 @@
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -209,15 +211,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -397,14 +398,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions/paginator.py` & `mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions/paginator.pyi` & `mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions/type_defs.py` & `mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,17 +34,17 @@
 __all__ = (
     "ActionIdentifierTypeDef",
     "EntityIdentifierTypeDef",
     "ContextDefinitionTypeDef",
     "DeterminingPolicyItemTypeDef",
     "EvaluationErrorItemTypeDef",
     "ResponseMetadataTypeDef",
-    "CognitoUserPoolConfigurationDetailTypeDef",
-    "CognitoUserPoolConfigurationItemTypeDef",
-    "CognitoUserPoolConfigurationTypeDef",
+    "CognitoGroupConfigurationDetailTypeDef",
+    "CognitoGroupConfigurationItemTypeDef",
+    "CognitoGroupConfigurationTypeDef",
     "ValidationSettingsTypeDef",
     "CreatePolicyTemplateInputRequestTypeDef",
     "DeleteIdentitySourceInputRequestTypeDef",
     "DeletePolicyInputRequestTypeDef",
     "DeletePolicyStoreInputRequestTypeDef",
     "DeletePolicyTemplateInputRequestTypeDef",
     "GetIdentitySourceInputRequestTypeDef",
@@ -60,15 +60,15 @@
     "PolicyStoreItemTypeDef",
     "ListPolicyTemplatesInputRequestTypeDef",
     "PolicyTemplateItemTypeDef",
     "StaticPolicyDefinitionDetailTypeDef",
     "StaticPolicyDefinitionItemTypeDef",
     "StaticPolicyDefinitionTypeDef",
     "SchemaDefinitionTypeDef",
-    "UpdateCognitoUserPoolConfigurationTypeDef",
+    "UpdateCognitoGroupConfigurationTypeDef",
     "UpdateStaticPolicyDefinitionTypeDef",
     "UpdatePolicyTemplateInputRequestTypeDef",
     "AttributeValueTypeDef",
     "EntityItemTypeDef",
     "EntityReferenceTypeDef",
     "TemplateLinkedPolicyDefinitionDetailTypeDef",
     "TemplateLinkedPolicyDefinitionItemTypeDef",
@@ -83,51 +83,55 @@
     "IsAuthorizedOutputTypeDef",
     "IsAuthorizedWithTokenOutputTypeDef",
     "PutSchemaOutputTypeDef",
     "UpdateIdentitySourceOutputTypeDef",
     "UpdatePolicyOutputTypeDef",
     "UpdatePolicyStoreOutputTypeDef",
     "UpdatePolicyTemplateOutputTypeDef",
-    "ConfigurationDetailTypeDef",
-    "ConfigurationItemTypeDef",
-    "ConfigurationTypeDef",
+    "CognitoUserPoolConfigurationDetailTypeDef",
+    "CognitoUserPoolConfigurationItemTypeDef",
+    "CognitoUserPoolConfigurationTypeDef",
     "CreatePolicyStoreInputRequestTypeDef",
     "GetPolicyStoreOutputTypeDef",
     "UpdatePolicyStoreInputRequestTypeDef",
     "ListIdentitySourcesInputRequestTypeDef",
     "ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
     "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
     "ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
     "ListPolicyStoresOutputTypeDef",
     "ListPolicyTemplatesOutputTypeDef",
     "PutSchemaInputRequestTypeDef",
-    "UpdateConfigurationTypeDef",
+    "UpdateCognitoUserPoolConfigurationTypeDef",
     "UpdatePolicyDefinitionTypeDef",
     "EntitiesDefinitionTypeDef",
     "PolicyFilterTypeDef",
     "PolicyDefinitionDetailTypeDef",
     "PolicyDefinitionItemTypeDef",
     "PolicyDefinitionTypeDef",
     "BatchIsAuthorizedOutputItemTypeDef",
-    "GetIdentitySourceOutputTypeDef",
-    "IdentitySourceItemTypeDef",
-    "CreateIdentitySourceInputRequestTypeDef",
-    "UpdateIdentitySourceInputRequestTypeDef",
+    "ConfigurationDetailTypeDef",
+    "ConfigurationItemTypeDef",
+    "ConfigurationTypeDef",
+    "UpdateConfigurationTypeDef",
     "UpdatePolicyInputRequestTypeDef",
     "BatchIsAuthorizedInputRequestTypeDef",
     "IsAuthorizedInputRequestTypeDef",
     "IsAuthorizedWithTokenInputRequestTypeDef",
     "ListPoliciesInputListPoliciesPaginateTypeDef",
     "ListPoliciesInputRequestTypeDef",
     "GetPolicyOutputTypeDef",
     "PolicyItemTypeDef",
     "CreatePolicyInputRequestTypeDef",
     "BatchIsAuthorizedOutputTypeDef",
-    "ListIdentitySourcesOutputTypeDef",
+    "GetIdentitySourceOutputTypeDef",
+    "IdentitySourceItemTypeDef",
+    "CreateIdentitySourceInputRequestTypeDef",
+    "UpdateIdentitySourceInputRequestTypeDef",
     "ListPoliciesOutputTypeDef",
+    "ListIdentitySourcesOutputTypeDef",
 )
 
 ActionIdentifierTypeDef = TypedDict(
     "ActionIdentifierTypeDef",
     {
         "actionType": str,
         "actionId": str,
@@ -164,35 +168,30 @@
         "RequestId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
         "HostId": NotRequired[str],
     },
 )
-CognitoUserPoolConfigurationDetailTypeDef = TypedDict(
-    "CognitoUserPoolConfigurationDetailTypeDef",
+CognitoGroupConfigurationDetailTypeDef = TypedDict(
+    "CognitoGroupConfigurationDetailTypeDef",
     {
-        "userPoolArn": str,
-        "clientIds": List[str],
-        "issuer": str,
+        "groupEntityType": NotRequired[str],
     },
 )
-CognitoUserPoolConfigurationItemTypeDef = TypedDict(
-    "CognitoUserPoolConfigurationItemTypeDef",
+CognitoGroupConfigurationItemTypeDef = TypedDict(
+    "CognitoGroupConfigurationItemTypeDef",
     {
-        "userPoolArn": str,
-        "clientIds": List[str],
-        "issuer": str,
+        "groupEntityType": NotRequired[str],
     },
 )
-CognitoUserPoolConfigurationTypeDef = TypedDict(
-    "CognitoUserPoolConfigurationTypeDef",
+CognitoGroupConfigurationTypeDef = TypedDict(
+    "CognitoGroupConfigurationTypeDef",
     {
-        "userPoolArn": str,
-        "clientIds": NotRequired[Sequence[str]],
+        "groupEntityType": str,
     },
 )
 ValidationSettingsTypeDef = TypedDict(
     "ValidationSettingsTypeDef",
     {
         "mode": ValidationModeType,
     },
@@ -355,19 +354,18 @@
 )
 SchemaDefinitionTypeDef = TypedDict(
     "SchemaDefinitionTypeDef",
     {
         "cedarJson": NotRequired[str],
     },
 )
-UpdateCognitoUserPoolConfigurationTypeDef = TypedDict(
-    "UpdateCognitoUserPoolConfigurationTypeDef",
+UpdateCognitoGroupConfigurationTypeDef = TypedDict(
+    "UpdateCognitoGroupConfigurationTypeDef",
     {
-        "userPoolArn": str,
-        "clientIds": NotRequired[Sequence[str]],
+        "groupEntityType": str,
     },
 )
 UpdateStaticPolicyDefinitionTypeDef = TypedDict(
     "UpdateStaticPolicyDefinitionTypeDef",
     {
         "statement": str,
         "description": NotRequired[str],
@@ -518,14 +516,15 @@
 )
 IsAuthorizedWithTokenOutputTypeDef = TypedDict(
     "IsAuthorizedWithTokenOutputTypeDef",
     {
         "decision": DecisionType,
         "determiningPolicies": List[DeterminingPolicyItemTypeDef],
         "errors": List[EvaluationErrorItemTypeDef],
+        "principal": EntityIdentifierTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 PutSchemaOutputTypeDef = TypedDict(
     "PutSchemaOutputTypeDef",
     {
         "policyStoreId": str,
@@ -574,30 +573,38 @@
         "policyStoreId": str,
         "policyTemplateId": str,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ConfigurationDetailTypeDef = TypedDict(
-    "ConfigurationDetailTypeDef",
+CognitoUserPoolConfigurationDetailTypeDef = TypedDict(
+    "CognitoUserPoolConfigurationDetailTypeDef",
     {
-        "cognitoUserPoolConfiguration": NotRequired[CognitoUserPoolConfigurationDetailTypeDef],
+        "userPoolArn": str,
+        "clientIds": List[str],
+        "issuer": str,
+        "groupConfiguration": NotRequired[CognitoGroupConfigurationDetailTypeDef],
     },
 )
-ConfigurationItemTypeDef = TypedDict(
-    "ConfigurationItemTypeDef",
+CognitoUserPoolConfigurationItemTypeDef = TypedDict(
+    "CognitoUserPoolConfigurationItemTypeDef",
     {
-        "cognitoUserPoolConfiguration": NotRequired[CognitoUserPoolConfigurationItemTypeDef],
+        "userPoolArn": str,
+        "clientIds": List[str],
+        "issuer": str,
+        "groupConfiguration": NotRequired[CognitoGroupConfigurationItemTypeDef],
     },
 )
-ConfigurationTypeDef = TypedDict(
-    "ConfigurationTypeDef",
+CognitoUserPoolConfigurationTypeDef = TypedDict(
+    "CognitoUserPoolConfigurationTypeDef",
     {
-        "cognitoUserPoolConfiguration": NotRequired[CognitoUserPoolConfigurationTypeDef],
+        "userPoolArn": str,
+        "clientIds": NotRequired[Sequence[str]],
+        "groupConfiguration": NotRequired[CognitoGroupConfigurationTypeDef],
     },
 )
 CreatePolicyStoreInputRequestTypeDef = TypedDict(
     "CreatePolicyStoreInputRequestTypeDef",
     {
         "validationSettings": ValidationSettingsTypeDef,
         "clientToken": NotRequired[str],
@@ -673,18 +680,20 @@
 PutSchemaInputRequestTypeDef = TypedDict(
     "PutSchemaInputRequestTypeDef",
     {
         "policyStoreId": str,
         "definition": SchemaDefinitionTypeDef,
     },
 )
-UpdateConfigurationTypeDef = TypedDict(
-    "UpdateConfigurationTypeDef",
+UpdateCognitoUserPoolConfigurationTypeDef = TypedDict(
+    "UpdateCognitoUserPoolConfigurationTypeDef",
     {
-        "cognitoUserPoolConfiguration": NotRequired[UpdateCognitoUserPoolConfigurationTypeDef],
+        "userPoolArn": str,
+        "clientIds": NotRequired[Sequence[str]],
+        "groupConfiguration": NotRequired[UpdateCognitoGroupConfigurationTypeDef],
     },
 )
 UpdatePolicyDefinitionTypeDef = TypedDict(
     "UpdatePolicyDefinitionTypeDef",
     {
         "static": NotRequired[UpdateStaticPolicyDefinitionTypeDef],
     },
@@ -730,55 +739,36 @@
     {
         "request": BatchIsAuthorizedInputItemTypeDef,
         "decision": DecisionType,
         "determiningPolicies": List[DeterminingPolicyItemTypeDef],
         "errors": List[EvaluationErrorItemTypeDef],
     },
 )
-GetIdentitySourceOutputTypeDef = TypedDict(
-    "GetIdentitySourceOutputTypeDef",
+ConfigurationDetailTypeDef = TypedDict(
+    "ConfigurationDetailTypeDef",
     {
-        "createdDate": datetime,
-        "details": IdentitySourceDetailsTypeDef,
-        "identitySourceId": str,
-        "lastUpdatedDate": datetime,
-        "policyStoreId": str,
-        "principalEntityType": str,
-        "configuration": ConfigurationDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "cognitoUserPoolConfiguration": NotRequired[CognitoUserPoolConfigurationDetailTypeDef],
     },
 )
-IdentitySourceItemTypeDef = TypedDict(
-    "IdentitySourceItemTypeDef",
+ConfigurationItemTypeDef = TypedDict(
+    "ConfigurationItemTypeDef",
     {
-        "createdDate": datetime,
-        "identitySourceId": str,
-        "lastUpdatedDate": datetime,
-        "policyStoreId": str,
-        "principalEntityType": str,
-        "details": NotRequired[IdentitySourceItemDetailsTypeDef],
-        "configuration": NotRequired[ConfigurationItemTypeDef],
+        "cognitoUserPoolConfiguration": NotRequired[CognitoUserPoolConfigurationItemTypeDef],
     },
 )
-CreateIdentitySourceInputRequestTypeDef = TypedDict(
-    "CreateIdentitySourceInputRequestTypeDef",
+ConfigurationTypeDef = TypedDict(
+    "ConfigurationTypeDef",
     {
-        "policyStoreId": str,
-        "configuration": ConfigurationTypeDef,
-        "clientToken": NotRequired[str],
-        "principalEntityType": NotRequired[str],
+        "cognitoUserPoolConfiguration": NotRequired[CognitoUserPoolConfigurationTypeDef],
     },
 )
-UpdateIdentitySourceInputRequestTypeDef = TypedDict(
-    "UpdateIdentitySourceInputRequestTypeDef",
+UpdateConfigurationTypeDef = TypedDict(
+    "UpdateConfigurationTypeDef",
     {
-        "policyStoreId": str,
-        "identitySourceId": str,
-        "updateConfiguration": UpdateConfigurationTypeDef,
-        "principalEntityType": NotRequired[str],
+        "cognitoUserPoolConfiguration": NotRequired[UpdateCognitoUserPoolConfigurationTypeDef],
     },
 )
 UpdatePolicyInputRequestTypeDef = TypedDict(
     "UpdatePolicyInputRequestTypeDef",
     {
         "policyStoreId": str,
         "policyId": str,
@@ -871,23 +861,66 @@
 BatchIsAuthorizedOutputTypeDef = TypedDict(
     "BatchIsAuthorizedOutputTypeDef",
     {
         "results": List[BatchIsAuthorizedOutputItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ListIdentitySourcesOutputTypeDef = TypedDict(
-    "ListIdentitySourcesOutputTypeDef",
+GetIdentitySourceOutputTypeDef = TypedDict(
+    "GetIdentitySourceOutputTypeDef",
     {
-        "nextToken": str,
-        "identitySources": List[IdentitySourceItemTypeDef],
+        "createdDate": datetime,
+        "details": IdentitySourceDetailsTypeDef,
+        "identitySourceId": str,
+        "lastUpdatedDate": datetime,
+        "policyStoreId": str,
+        "principalEntityType": str,
+        "configuration": ConfigurationDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+IdentitySourceItemTypeDef = TypedDict(
+    "IdentitySourceItemTypeDef",
+    {
+        "createdDate": datetime,
+        "identitySourceId": str,
+        "lastUpdatedDate": datetime,
+        "policyStoreId": str,
+        "principalEntityType": str,
+        "details": NotRequired[IdentitySourceItemDetailsTypeDef],
+        "configuration": NotRequired[ConfigurationItemTypeDef],
+    },
+)
+CreateIdentitySourceInputRequestTypeDef = TypedDict(
+    "CreateIdentitySourceInputRequestTypeDef",
+    {
+        "policyStoreId": str,
+        "configuration": ConfigurationTypeDef,
+        "clientToken": NotRequired[str],
+        "principalEntityType": NotRequired[str],
+    },
+)
+UpdateIdentitySourceInputRequestTypeDef = TypedDict(
+    "UpdateIdentitySourceInputRequestTypeDef",
+    {
+        "policyStoreId": str,
+        "identitySourceId": str,
+        "updateConfiguration": UpdateConfigurationTypeDef,
+        "principalEntityType": NotRequired[str],
+    },
+)
 ListPoliciesOutputTypeDef = TypedDict(
     "ListPoliciesOutputTypeDef",
     {
         "nextToken": str,
         "policies": List[PolicyItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ListIdentitySourcesOutputTypeDef = TypedDict(
+    "ListIdentitySourcesOutputTypeDef",
+    {
+        "nextToken": str,
+        "identitySources": List[IdentitySourceItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions/type_defs.pyi` & `mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -34,17 +34,17 @@
 __all__ = (
     "ActionIdentifierTypeDef",
     "EntityIdentifierTypeDef",
     "ContextDefinitionTypeDef",
     "DeterminingPolicyItemTypeDef",
     "EvaluationErrorItemTypeDef",
     "ResponseMetadataTypeDef",
-    "CognitoUserPoolConfigurationDetailTypeDef",
-    "CognitoUserPoolConfigurationItemTypeDef",
-    "CognitoUserPoolConfigurationTypeDef",
+    "CognitoGroupConfigurationDetailTypeDef",
+    "CognitoGroupConfigurationItemTypeDef",
+    "CognitoGroupConfigurationTypeDef",
     "ValidationSettingsTypeDef",
     "CreatePolicyTemplateInputRequestTypeDef",
     "DeleteIdentitySourceInputRequestTypeDef",
     "DeletePolicyInputRequestTypeDef",
     "DeletePolicyStoreInputRequestTypeDef",
     "DeletePolicyTemplateInputRequestTypeDef",
     "GetIdentitySourceInputRequestTypeDef",
@@ -60,15 +60,15 @@
     "PolicyStoreItemTypeDef",
     "ListPolicyTemplatesInputRequestTypeDef",
     "PolicyTemplateItemTypeDef",
     "StaticPolicyDefinitionDetailTypeDef",
     "StaticPolicyDefinitionItemTypeDef",
     "StaticPolicyDefinitionTypeDef",
     "SchemaDefinitionTypeDef",
-    "UpdateCognitoUserPoolConfigurationTypeDef",
+    "UpdateCognitoGroupConfigurationTypeDef",
     "UpdateStaticPolicyDefinitionTypeDef",
     "UpdatePolicyTemplateInputRequestTypeDef",
     "AttributeValueTypeDef",
     "EntityItemTypeDef",
     "EntityReferenceTypeDef",
     "TemplateLinkedPolicyDefinitionDetailTypeDef",
     "TemplateLinkedPolicyDefinitionItemTypeDef",
@@ -83,51 +83,55 @@
     "IsAuthorizedOutputTypeDef",
     "IsAuthorizedWithTokenOutputTypeDef",
     "PutSchemaOutputTypeDef",
     "UpdateIdentitySourceOutputTypeDef",
     "UpdatePolicyOutputTypeDef",
     "UpdatePolicyStoreOutputTypeDef",
     "UpdatePolicyTemplateOutputTypeDef",
-    "ConfigurationDetailTypeDef",
-    "ConfigurationItemTypeDef",
-    "ConfigurationTypeDef",
+    "CognitoUserPoolConfigurationDetailTypeDef",
+    "CognitoUserPoolConfigurationItemTypeDef",
+    "CognitoUserPoolConfigurationTypeDef",
     "CreatePolicyStoreInputRequestTypeDef",
     "GetPolicyStoreOutputTypeDef",
     "UpdatePolicyStoreInputRequestTypeDef",
     "ListIdentitySourcesInputRequestTypeDef",
     "ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
     "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
     "ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
     "ListPolicyStoresOutputTypeDef",
     "ListPolicyTemplatesOutputTypeDef",
     "PutSchemaInputRequestTypeDef",
-    "UpdateConfigurationTypeDef",
+    "UpdateCognitoUserPoolConfigurationTypeDef",
     "UpdatePolicyDefinitionTypeDef",
     "EntitiesDefinitionTypeDef",
     "PolicyFilterTypeDef",
     "PolicyDefinitionDetailTypeDef",
     "PolicyDefinitionItemTypeDef",
     "PolicyDefinitionTypeDef",
     "BatchIsAuthorizedOutputItemTypeDef",
-    "GetIdentitySourceOutputTypeDef",
-    "IdentitySourceItemTypeDef",
-    "CreateIdentitySourceInputRequestTypeDef",
-    "UpdateIdentitySourceInputRequestTypeDef",
+    "ConfigurationDetailTypeDef",
+    "ConfigurationItemTypeDef",
+    "ConfigurationTypeDef",
+    "UpdateConfigurationTypeDef",
     "UpdatePolicyInputRequestTypeDef",
     "BatchIsAuthorizedInputRequestTypeDef",
     "IsAuthorizedInputRequestTypeDef",
     "IsAuthorizedWithTokenInputRequestTypeDef",
     "ListPoliciesInputListPoliciesPaginateTypeDef",
     "ListPoliciesInputRequestTypeDef",
     "GetPolicyOutputTypeDef",
     "PolicyItemTypeDef",
     "CreatePolicyInputRequestTypeDef",
     "BatchIsAuthorizedOutputTypeDef",
-    "ListIdentitySourcesOutputTypeDef",
+    "GetIdentitySourceOutputTypeDef",
+    "IdentitySourceItemTypeDef",
+    "CreateIdentitySourceInputRequestTypeDef",
+    "UpdateIdentitySourceInputRequestTypeDef",
     "ListPoliciesOutputTypeDef",
+    "ListIdentitySourcesOutputTypeDef",
 )
 
 ActionIdentifierTypeDef = TypedDict(
     "ActionIdentifierTypeDef",
     {
         "actionType": str,
         "actionId": str,
@@ -164,35 +168,30 @@
         "RequestId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
         "HostId": NotRequired[str],
     },
 )
-CognitoUserPoolConfigurationDetailTypeDef = TypedDict(
-    "CognitoUserPoolConfigurationDetailTypeDef",
+CognitoGroupConfigurationDetailTypeDef = TypedDict(
+    "CognitoGroupConfigurationDetailTypeDef",
     {
-        "userPoolArn": str,
-        "clientIds": List[str],
-        "issuer": str,
+        "groupEntityType": NotRequired[str],
     },
 )
-CognitoUserPoolConfigurationItemTypeDef = TypedDict(
-    "CognitoUserPoolConfigurationItemTypeDef",
+CognitoGroupConfigurationItemTypeDef = TypedDict(
+    "CognitoGroupConfigurationItemTypeDef",
     {
-        "userPoolArn": str,
-        "clientIds": List[str],
-        "issuer": str,
+        "groupEntityType": NotRequired[str],
     },
 )
-CognitoUserPoolConfigurationTypeDef = TypedDict(
-    "CognitoUserPoolConfigurationTypeDef",
+CognitoGroupConfigurationTypeDef = TypedDict(
+    "CognitoGroupConfigurationTypeDef",
     {
-        "userPoolArn": str,
-        "clientIds": NotRequired[Sequence[str]],
+        "groupEntityType": str,
     },
 )
 ValidationSettingsTypeDef = TypedDict(
     "ValidationSettingsTypeDef",
     {
         "mode": ValidationModeType,
     },
@@ -355,19 +354,18 @@
 )
 SchemaDefinitionTypeDef = TypedDict(
     "SchemaDefinitionTypeDef",
     {
         "cedarJson": NotRequired[str],
     },
 )
-UpdateCognitoUserPoolConfigurationTypeDef = TypedDict(
-    "UpdateCognitoUserPoolConfigurationTypeDef",
+UpdateCognitoGroupConfigurationTypeDef = TypedDict(
+    "UpdateCognitoGroupConfigurationTypeDef",
     {
-        "userPoolArn": str,
-        "clientIds": NotRequired[Sequence[str]],
+        "groupEntityType": str,
     },
 )
 UpdateStaticPolicyDefinitionTypeDef = TypedDict(
     "UpdateStaticPolicyDefinitionTypeDef",
     {
         "statement": str,
         "description": NotRequired[str],
@@ -518,14 +516,15 @@
 )
 IsAuthorizedWithTokenOutputTypeDef = TypedDict(
     "IsAuthorizedWithTokenOutputTypeDef",
     {
         "decision": DecisionType,
         "determiningPolicies": List[DeterminingPolicyItemTypeDef],
         "errors": List[EvaluationErrorItemTypeDef],
+        "principal": EntityIdentifierTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 PutSchemaOutputTypeDef = TypedDict(
     "PutSchemaOutputTypeDef",
     {
         "policyStoreId": str,
@@ -574,30 +573,38 @@
         "policyStoreId": str,
         "policyTemplateId": str,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ConfigurationDetailTypeDef = TypedDict(
-    "ConfigurationDetailTypeDef",
+CognitoUserPoolConfigurationDetailTypeDef = TypedDict(
+    "CognitoUserPoolConfigurationDetailTypeDef",
     {
-        "cognitoUserPoolConfiguration": NotRequired[CognitoUserPoolConfigurationDetailTypeDef],
+        "userPoolArn": str,
+        "clientIds": List[str],
+        "issuer": str,
+        "groupConfiguration": NotRequired[CognitoGroupConfigurationDetailTypeDef],
     },
 )
-ConfigurationItemTypeDef = TypedDict(
-    "ConfigurationItemTypeDef",
+CognitoUserPoolConfigurationItemTypeDef = TypedDict(
+    "CognitoUserPoolConfigurationItemTypeDef",
     {
-        "cognitoUserPoolConfiguration": NotRequired[CognitoUserPoolConfigurationItemTypeDef],
+        "userPoolArn": str,
+        "clientIds": List[str],
+        "issuer": str,
+        "groupConfiguration": NotRequired[CognitoGroupConfigurationItemTypeDef],
     },
 )
-ConfigurationTypeDef = TypedDict(
-    "ConfigurationTypeDef",
+CognitoUserPoolConfigurationTypeDef = TypedDict(
+    "CognitoUserPoolConfigurationTypeDef",
     {
-        "cognitoUserPoolConfiguration": NotRequired[CognitoUserPoolConfigurationTypeDef],
+        "userPoolArn": str,
+        "clientIds": NotRequired[Sequence[str]],
+        "groupConfiguration": NotRequired[CognitoGroupConfigurationTypeDef],
     },
 )
 CreatePolicyStoreInputRequestTypeDef = TypedDict(
     "CreatePolicyStoreInputRequestTypeDef",
     {
         "validationSettings": ValidationSettingsTypeDef,
         "clientToken": NotRequired[str],
@@ -673,18 +680,20 @@
 PutSchemaInputRequestTypeDef = TypedDict(
     "PutSchemaInputRequestTypeDef",
     {
         "policyStoreId": str,
         "definition": SchemaDefinitionTypeDef,
     },
 )
-UpdateConfigurationTypeDef = TypedDict(
-    "UpdateConfigurationTypeDef",
+UpdateCognitoUserPoolConfigurationTypeDef = TypedDict(
+    "UpdateCognitoUserPoolConfigurationTypeDef",
     {
-        "cognitoUserPoolConfiguration": NotRequired[UpdateCognitoUserPoolConfigurationTypeDef],
+        "userPoolArn": str,
+        "clientIds": NotRequired[Sequence[str]],
+        "groupConfiguration": NotRequired[UpdateCognitoGroupConfigurationTypeDef],
     },
 )
 UpdatePolicyDefinitionTypeDef = TypedDict(
     "UpdatePolicyDefinitionTypeDef",
     {
         "static": NotRequired[UpdateStaticPolicyDefinitionTypeDef],
     },
@@ -730,55 +739,36 @@
     {
         "request": BatchIsAuthorizedInputItemTypeDef,
         "decision": DecisionType,
         "determiningPolicies": List[DeterminingPolicyItemTypeDef],
         "errors": List[EvaluationErrorItemTypeDef],
     },
 )
-GetIdentitySourceOutputTypeDef = TypedDict(
-    "GetIdentitySourceOutputTypeDef",
+ConfigurationDetailTypeDef = TypedDict(
+    "ConfigurationDetailTypeDef",
     {
-        "createdDate": datetime,
-        "details": IdentitySourceDetailsTypeDef,
-        "identitySourceId": str,
-        "lastUpdatedDate": datetime,
-        "policyStoreId": str,
-        "principalEntityType": str,
-        "configuration": ConfigurationDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "cognitoUserPoolConfiguration": NotRequired[CognitoUserPoolConfigurationDetailTypeDef],
     },
 )
-IdentitySourceItemTypeDef = TypedDict(
-    "IdentitySourceItemTypeDef",
+ConfigurationItemTypeDef = TypedDict(
+    "ConfigurationItemTypeDef",
     {
-        "createdDate": datetime,
-        "identitySourceId": str,
-        "lastUpdatedDate": datetime,
-        "policyStoreId": str,
-        "principalEntityType": str,
-        "details": NotRequired[IdentitySourceItemDetailsTypeDef],
-        "configuration": NotRequired[ConfigurationItemTypeDef],
+        "cognitoUserPoolConfiguration": NotRequired[CognitoUserPoolConfigurationItemTypeDef],
     },
 )
-CreateIdentitySourceInputRequestTypeDef = TypedDict(
-    "CreateIdentitySourceInputRequestTypeDef",
+ConfigurationTypeDef = TypedDict(
+    "ConfigurationTypeDef",
     {
-        "policyStoreId": str,
-        "configuration": ConfigurationTypeDef,
-        "clientToken": NotRequired[str],
-        "principalEntityType": NotRequired[str],
+        "cognitoUserPoolConfiguration": NotRequired[CognitoUserPoolConfigurationTypeDef],
     },
 )
-UpdateIdentitySourceInputRequestTypeDef = TypedDict(
-    "UpdateIdentitySourceInputRequestTypeDef",
+UpdateConfigurationTypeDef = TypedDict(
+    "UpdateConfigurationTypeDef",
     {
-        "policyStoreId": str,
-        "identitySourceId": str,
-        "updateConfiguration": UpdateConfigurationTypeDef,
-        "principalEntityType": NotRequired[str],
+        "cognitoUserPoolConfiguration": NotRequired[UpdateCognitoUserPoolConfigurationTypeDef],
     },
 )
 UpdatePolicyInputRequestTypeDef = TypedDict(
     "UpdatePolicyInputRequestTypeDef",
     {
         "policyStoreId": str,
         "policyId": str,
@@ -871,23 +861,66 @@
 BatchIsAuthorizedOutputTypeDef = TypedDict(
     "BatchIsAuthorizedOutputTypeDef",
     {
         "results": List[BatchIsAuthorizedOutputItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ListIdentitySourcesOutputTypeDef = TypedDict(
-    "ListIdentitySourcesOutputTypeDef",
+GetIdentitySourceOutputTypeDef = TypedDict(
+    "GetIdentitySourceOutputTypeDef",
     {
-        "nextToken": str,
-        "identitySources": List[IdentitySourceItemTypeDef],
+        "createdDate": datetime,
+        "details": IdentitySourceDetailsTypeDef,
+        "identitySourceId": str,
+        "lastUpdatedDate": datetime,
+        "policyStoreId": str,
+        "principalEntityType": str,
+        "configuration": ConfigurationDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+IdentitySourceItemTypeDef = TypedDict(
+    "IdentitySourceItemTypeDef",
+    {
+        "createdDate": datetime,
+        "identitySourceId": str,
+        "lastUpdatedDate": datetime,
+        "policyStoreId": str,
+        "principalEntityType": str,
+        "details": NotRequired[IdentitySourceItemDetailsTypeDef],
+        "configuration": NotRequired[ConfigurationItemTypeDef],
+    },
+)
+CreateIdentitySourceInputRequestTypeDef = TypedDict(
+    "CreateIdentitySourceInputRequestTypeDef",
+    {
+        "policyStoreId": str,
+        "configuration": ConfigurationTypeDef,
+        "clientToken": NotRequired[str],
+        "principalEntityType": NotRequired[str],
+    },
+)
+UpdateIdentitySourceInputRequestTypeDef = TypedDict(
+    "UpdateIdentitySourceInputRequestTypeDef",
+    {
+        "policyStoreId": str,
+        "identitySourceId": str,
+        "updateConfiguration": UpdateConfigurationTypeDef,
+        "principalEntityType": NotRequired[str],
+    },
+)
 ListPoliciesOutputTypeDef = TypedDict(
     "ListPoliciesOutputTypeDef",
     {
         "nextToken": str,
         "policies": List[PolicyItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ListIdentitySourcesOutputTypeDef = TypedDict(
+    "ListIdentitySourcesOutputTypeDef",
+    {
+        "nextToken": str,
+        "identitySources": List[IdentitySourceItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions.egg-info/PKG-INFO` & `mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-verifiedpermissions
-Version: 1.34.57
-Summary: Type annotations for boto3.VerifiedPermissions 1.34.57 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.78
+Summary: Type annotations for boto3.VerifiedPermissions 1.34.78 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-verifiedpermissions.svg?color=blue)](https://pypi.org/project/mypy-boto3-verifiedpermissions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-verifiedpermissions)](https://pepy.tech/project/mypy-boto3-verifiedpermissions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VerifiedPermissions 1.34.57](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
+[boto3.VerifiedPermissions 1.34.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-verifiedpermissions-1.34.57/mypy_boto3_verifiedpermissions.egg-info/SOURCES.txt` & `mypy-boto3-verifiedpermissions-1.34.78/mypy_boto3_verifiedpermissions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.34.57/setup.py` & `mypy-boto3-verifiedpermissions-1.34.78/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-verifiedpermissions",
-    version="1.34.57",
+    version="1.34.78",
     packages=["mypy_boto3_verifiedpermissions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.VerifiedPermissions 1.34.57 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.VerifiedPermissions 1.34.78 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

