# Comparing `tmp/cdk-circleci-oidc-0.0.2.tar.gz` & `tmp/cdk-circleci-oidc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-circleci-oidc-0.0.2.tar", last modified: Thu Oct  5 20:39:00 2023, max compression
+gzip compressed data, was "cdk-circleci-oidc-0.0.3.tar", last modified: Fri Apr  5 14:27:37 2024, max compression
```

## Comparing `cdk-circleci-oidc-0.0.2.tar` & `cdk-circleci-oidc-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 20:39:00.029747 cdk-circleci-oidc-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2023-10-05 20:38:45.000000 cdk-circleci-oidc-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-05 20:38:45.000000 cdk-circleci-oidc-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2023-10-05 20:39:00.029747 cdk-circleci-oidc-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2023-10-05 20:38:45.000000 cdk-circleci-oidc-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      236 2023-10-05 20:38:45.000000 cdk-circleci-oidc-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-05 20:39:00.029747 cdk-circleci-oidc-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2023-10-05 20:38:45.000000 cdk-circleci-oidc-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 20:39:00.029747 cdk-circleci-oidc-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 20:39:00.029747 cdk-circleci-oidc-0.0.2/src/cdk_circleci_oidc/
--rw-r--r--   0 runner    (1001) docker     (127)    26229 2023-10-05 20:38:45.000000 cdk-circleci-oidc-0.0.2/src/cdk_circleci_oidc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 20:39:00.029747 cdk-circleci-oidc-0.0.2/src/cdk_circleci_oidc/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2023-10-05 20:38:45.000000 cdk-circleci-oidc-0.0.2/src/cdk_circleci_oidc/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24420 2023-10-05 20:38:45.000000 cdk-circleci-oidc-0.0.2/src/cdk_circleci_oidc/_jsii/cdk-circleci-oidc@0.0.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-05 20:38:45.000000 cdk-circleci-oidc-0.0.2/src/cdk_circleci_oidc/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 20:39:00.029747 cdk-circleci-oidc-0.0.2/src/cdk_circleci_oidc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2023-10-05 20:38:59.000000 cdk-circleci-oidc-0.0.2/src/cdk_circleci_oidc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2023-10-05 20:38:59.000000 cdk-circleci-oidc-0.0.2/src/cdk_circleci_oidc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-05 20:38:59.000000 cdk-circleci-oidc-0.0.2/src/cdk_circleci_oidc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-10-05 20:38:59.000000 cdk-circleci-oidc-0.0.2/src/cdk_circleci_oidc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-10-05 20:38:59.000000 cdk-circleci-oidc-0.0.2/src/cdk_circleci_oidc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:27:37.277005 cdk-circleci-oidc-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-05 14:27:21.000000 cdk-circleci-oidc-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-05 14:27:21.000000 cdk-circleci-oidc-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-04-05 14:27:37.273005 cdk-circleci-oidc-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-05 14:27:21.000000 cdk-circleci-oidc-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-05 14:27:21.000000 cdk-circleci-oidc-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:27:37.277005 cdk-circleci-oidc-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-05 14:27:21.000000 cdk-circleci-oidc-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:27:37.273005 cdk-circleci-oidc-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:27:37.273005 cdk-circleci-oidc-0.0.3/src/cdk_circleci_oidc/
+-rw-r--r--   0 runner    (1001) docker     (127)    26305 2024-04-05 14:27:21.000000 cdk-circleci-oidc-0.0.3/src/cdk_circleci_oidc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:27:37.273005 cdk-circleci-oidc-0.0.3/src/cdk_circleci_oidc/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-05 14:27:21.000000 cdk-circleci-oidc-0.0.3/src/cdk_circleci_oidc/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24507 2024-04-05 14:27:21.000000 cdk-circleci-oidc-0.0.3/src/cdk_circleci_oidc/_jsii/cdk-circleci-oidc@0.0.3.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:27:21.000000 cdk-circleci-oidc-0.0.3/src/cdk_circleci_oidc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:27:37.273005 cdk-circleci-oidc-0.0.3/src/cdk_circleci_oidc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-04-05 14:27:37.000000 cdk-circleci-oidc-0.0.3/src/cdk_circleci_oidc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-05 14:27:37.000000 cdk-circleci-oidc-0.0.3/src/cdk_circleci_oidc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:27:37.000000 cdk-circleci-oidc-0.0.3/src/cdk_circleci_oidc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-05 14:27:37.000000 cdk-circleci-oidc-0.0.3/src/cdk_circleci_oidc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 14:27:37.000000 cdk-circleci-oidc-0.0.3/src/cdk_circleci_oidc.egg-info/top_level.txt
```

### Comparing `cdk-circleci-oidc-0.0.2/LICENSE` & `cdk-circleci-oidc-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-circleci-oidc-0.0.2/PKG-INFO` & `cdk-circleci-oidc-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: cdk-circleci-oidc
-Version: 0.0.2
+Version: 0.0.3
 Summary: @blimmer/cdk-circleci-oidc
 Home-page: https://github.com/blimmer/cdk-circleci-oidc.git
 Author: Ben Limmer<hello@benlimmer.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/blimmer/cdk-circleci-oidc.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CircleCI OIDC
 
 This repository contains constructs to communicate between CircleCI and AWS via an Open ID Connect (OIDC) provider.
 The process is described in [this CircleCI blog post](https://circleci.com/blog/openid-connect-identity-tokens/).
```

### Comparing `cdk-circleci-oidc-0.0.2/README.md` & `cdk-circleci-oidc-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cdk-circleci-oidc-0.0.2/setup.py` & `cdk-circleci-oidc-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-circleci-oidc",
-    "version": "0.0.2",
+    "version": "0.0.3",
     "description": "@blimmer/cdk-circleci-oidc",
     "license": "Apache-2.0",
     "url": "https://github.com/blimmer/cdk-circleci-oidc.git",
     "long_description_content_type": "text/markdown",
     "author": "Ben Limmer<hello@benlimmer.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,37 +22,37 @@
     },
     "packages": [
         "cdk_circleci_oidc",
         "cdk_circleci_oidc._jsii"
     ],
     "package_data": {
         "cdk_circleci_oidc._jsii": [
-            "cdk-circleci-oidc@0.0.2.jsii.tgz"
+            "cdk-circleci-oidc@0.0.3.jsii.tgz"
         ],
         "cdk_circleci_oidc": [
             "py.typed"
         ]
     },
-    "python_requires": "~=3.7",
+    "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.1.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.89.0, <2.0.0",
+        "jsii>=1.96.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
```

### Comparing `cdk-circleci-oidc-0.0.2/src/cdk_circleci_oidc/__init__.py` & `cdk-circleci-oidc-0.0.3/src/cdk_circleci_oidc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,17 @@
 pip install cdk-circleci-oidc
 ```
 
 ## Contributing
 
 Contributions, issues, and feedback are welcome!
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -320,15 +323,15 @@
     '''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
-        circle_ci_oidc_provider: typing.Union[CircleCiOidcProvider, typing.Union["ManualCircleCiOidcProviderProps", typing.Dict[builtins.str, typing.Any]]],
+        circle_ci_oidc_provider: typing.Union[typing.Union["ManualCircleCiOidcProviderProps", typing.Dict[builtins.str, typing.Any]], CircleCiOidcProvider],
         circle_ci_project_ids: typing.Optional[typing.Sequence[builtins.str]] = None,
         description: typing.Optional[builtins.str] = None,
         inline_policies: typing.Optional[typing.Mapping[builtins.str, _aws_cdk_aws_iam_ceddda9d.PolicyDocument]] = None,
         managed_policies: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.IManagedPolicy]] = None,
         role_name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
@@ -374,15 +377,15 @@
         "role_name": "roleName",
     },
 )
 class CircleCiOidcRoleProps:
     def __init__(
         self,
         *,
-        circle_ci_oidc_provider: typing.Union[CircleCiOidcProvider, typing.Union["ManualCircleCiOidcProviderProps", typing.Dict[builtins.str, typing.Any]]],
+        circle_ci_oidc_provider: typing.Union[typing.Union["ManualCircleCiOidcProviderProps", typing.Dict[builtins.str, typing.Any]], CircleCiOidcProvider],
         circle_ci_project_ids: typing.Optional[typing.Sequence[builtins.str]] = None,
         description: typing.Optional[builtins.str] = None,
         inline_policies: typing.Optional[typing.Mapping[builtins.str, _aws_cdk_aws_iam_ceddda9d.PolicyDocument]] = None,
         managed_policies: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.IManagedPolicy]] = None,
         role_name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
@@ -414,18 +417,18 @@
             self._values["managed_policies"] = managed_policies
         if role_name is not None:
             self._values["role_name"] = role_name
 
     @builtins.property
     def circle_ci_oidc_provider(
         self,
-    ) -> typing.Union[CircleCiOidcProvider, "ManualCircleCiOidcProviderProps"]:
+    ) -> typing.Union["ManualCircleCiOidcProviderProps", CircleCiOidcProvider]:
         result = self._values.get("circle_ci_oidc_provider")
         assert result is not None, "Required property 'circle_ci_oidc_provider' is missing"
-        return typing.cast(typing.Union[CircleCiOidcProvider, "ManualCircleCiOidcProviderProps"], result)
+        return typing.cast(typing.Union["ManualCircleCiOidcProviderProps", CircleCiOidcProvider], result)
 
     @builtins.property
     def circle_ci_project_ids(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Provide the UUID(s) of the CircleCI project(s) you want to be allowed to use this role.
 
         If you don't provide this
         value, the role will be allowed to be assumed by any CircleCI project in your organization. You can find a
@@ -570,27 +573,27 @@
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__9a1d9304663f45d61bd197cf48bd3145a25be4318f85ebeec9bb3b566e0f0ba9(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
-    circle_ci_oidc_provider: typing.Union[CircleCiOidcProvider, typing.Union[ManualCircleCiOidcProviderProps, typing.Dict[builtins.str, typing.Any]]],
+    circle_ci_oidc_provider: typing.Union[typing.Union[ManualCircleCiOidcProviderProps, typing.Dict[builtins.str, typing.Any]], CircleCiOidcProvider],
     circle_ci_project_ids: typing.Optional[typing.Sequence[builtins.str]] = None,
     description: typing.Optional[builtins.str] = None,
     inline_policies: typing.Optional[typing.Mapping[builtins.str, _aws_cdk_aws_iam_ceddda9d.PolicyDocument]] = None,
     managed_policies: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.IManagedPolicy]] = None,
     role_name: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__d28caf46e7e0d75fcdc4c1a3dec9aa2e5dff8efcf72c3adb43eab258081ffcf9(
     *,
-    circle_ci_oidc_provider: typing.Union[CircleCiOidcProvider, typing.Union[ManualCircleCiOidcProviderProps, typing.Dict[builtins.str, typing.Any]]],
+    circle_ci_oidc_provider: typing.Union[typing.Union[ManualCircleCiOidcProviderProps, typing.Dict[builtins.str, typing.Any]], CircleCiOidcProvider],
     circle_ci_project_ids: typing.Optional[typing.Sequence[builtins.str]] = None,
     description: typing.Optional[builtins.str] = None,
     inline_policies: typing.Optional[typing.Mapping[builtins.str, _aws_cdk_aws_iam_ceddda9d.PolicyDocument]] = None,
     managed_policies: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.IManagedPolicy]] = None,
     role_name: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
```

### Comparing `cdk-circleci-oidc-0.0.2/src/cdk_circleci_oidc.egg-info/PKG-INFO` & `cdk-circleci-oidc-0.0.3/src/cdk_circleci_oidc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: cdk-circleci-oidc
-Version: 0.0.2
+Version: 0.0.3
 Summary: @blimmer/cdk-circleci-oidc
 Home-page: https://github.com/blimmer/cdk-circleci-oidc.git
 Author: Ben Limmer<hello@benlimmer.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/blimmer/cdk-circleci-oidc.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CircleCI OIDC
 
 This repository contains constructs to communicate between CircleCI and AWS via an Open ID Connect (OIDC) provider.
 The process is described in [this CircleCI blog post](https://circleci.com/blog/openid-connect-identity-tokens/).
```

