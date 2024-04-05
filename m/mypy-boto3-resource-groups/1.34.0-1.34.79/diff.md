# Comparing `tmp/mypy-boto3-resource-groups-1.34.0.tar.gz` & `tmp/mypy-boto3-resource-groups-1.34.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-resource-groups-1.34.0.tar", last modified: Wed Dec 13 21:23:39 2023, max compression
+gzip compressed data, was "mypy-boto3-resource-groups-1.34.79.tar", last modified: Fri Apr  5 19:20:35 2024, max compression
```

## Comparing `mypy-boto3-resource-groups-1.34.0.tar` & `mypy-boto3-resource-groups-1.34.79.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:39.411340 mypy-boto3-resource-groups-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:18:14.000000 mypy-boto3-resource-groups-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13402 2023-12-13 21:23:39.411340 mypy-boto3-resource-groups-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11838 2023-12-13 21:18:14.000000 mypy-boto3-resource-groups-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:39.411340 mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups/
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2023-12-13 21:18:14.000000 mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2023-12-13 21:18:14.000000 mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      935 2023-12-13 21:18:14.000000 mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15492 2023-12-13 21:18:15.000000 mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15488 2023-12-13 21:18:14.000000 mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9989 2023-12-13 21:18:15.000000 mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9987 2023-12-13 21:18:15.000000 mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2023-12-13 21:18:15.000000 mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2023-12-13 21:18:15.000000 mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:18:14.000000 mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14290 2023-12-13 21:18:15.000000 mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14289 2023-12-13 21:18:15.000000 mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:18:14.000000 mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:39.411340 mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13402 2023-12-13 21:23:39.000000 mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-13 21:23:39.000000 mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:39.000000 mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:39.000000 mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:23:39.000000 mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 21:23:39.000000 mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:23:39.411340 mypy-boto3-resource-groups-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2023-12-13 21:18:14.000000 mypy-boto3-resource-groups-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:20:35.138697 mypy-boto3-resource-groups-1.34.79/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-05 19:20:19.000000 mypy-boto3-resource-groups-1.34.79/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13425 2024-04-05 19:20:35.138697 mypy-boto3-resource-groups-1.34.79/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11839 2024-04-05 19:20:19.000000 mypy-boto3-resource-groups-1.34.79/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:20:35.134697 mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups/
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-05 19:20:19.000000 mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-05 19:20:19.000000 mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-05 19:20:19.000000 mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15494 2024-04-05 19:20:20.000000 mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15491 2024-04-05 19:20:19.000000 mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10176 2024-04-05 19:20:20.000000 mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10176 2024-04-05 19:20:20.000000 mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-04-05 19:20:20.000000 mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-05 19:20:20.000000 mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:20:19.000000 mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    14302 2024-04-05 19:20:20.000000 mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14302 2024-04-05 19:20:20.000000 mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-05 19:20:19.000000 mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:20:35.138697 mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13425 2024-04-05 19:20:35.000000 mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-05 19:20:35.000000 mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:20:35.000000 mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:20:35.000000 mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-05 19:20:35.000000 mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-05 19:20:35.000000 mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 19:20:35.138697 mypy-boto3-resource-groups-1.34.79/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-05 19:20:19.000000 mypy-boto3-resource-groups-1.34.79/setup.py
```

### Comparing `mypy-boto3-resource-groups-1.34.0/LICENSE` & `mypy-boto3-resource-groups-1.34.79/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-resource-groups-1.34.0/PKG-INFO` & `mypy-boto3-resource-groups-1.34.79/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resource-groups
-Version: 1.34.0
-Summary: Type annotations for boto3.ResourceGroups 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.79
+Summary: Type annotations for boto3.ResourceGroups 1.34.79 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-resource-groups"></a>
 
 # mypy-boto3-resource-groups
 
 [![PyPI - mypy-boto3-resource-groups](https://img.shields.io/pypi/v/mypy-boto3-resource-groups.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-groups)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resource-groups.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-groups)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resource-groups)](https://pepy.tech/project/mypy-boto3-resource-groups)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceGroups 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
+[boto3.ResourceGroups 1.34.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-resource-groups docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-resource-groups-1.34.0/README.md` & `mypy-boto3-resource-groups-1.34.79/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resource-groups.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-groups)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resource-groups)](https://pepy.tech/project/mypy-boto3-resource-groups)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceGroups 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
+[boto3.ResourceGroups 1.34.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-resource-groups docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups/__init__.py` & `mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 """
 
 from .client import ResourceGroupsClient
 from .paginator import ListGroupResourcesPaginator, ListGroupsPaginator, SearchResourcesPaginator
 
 Client = ResourceGroupsClient
 
-
 __all__ = (
     "Client",
     "ListGroupResourcesPaginator",
     "ListGroupsPaginator",
     "ResourceGroupsClient",
     "SearchResourcesPaginator",
 )
```

### Comparing `mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups/__init__.pyi` & `mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups/__main__.py` & `mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ResourceGroups 1.34.0\nVersion:         1.34.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.ResourceGroups 1.34.79\n"
+        "Version:         1.34.79\n"
+        "Builder version: 7.23.2\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.0")
+    print("1.34.79")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups/client.py` & `mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ResourceGroupsClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -109,15 +108,15 @@
     def create_group(
         self,
         *,
         Name: str,
         Description: str = ...,
         ResourceQuery: ResourceQueryTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        Configuration: Sequence[GroupConfigurationItemTypeDef] = ...
+        Configuration: Sequence[GroupConfigurationItemTypeDef] = ...,
     ) -> CreateGroupOutputTypeDef:
         """
         Creates a resource group with the specified name and description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.create_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/client/#create_group)
         """
@@ -202,15 +201,15 @@
     def list_group_resources(
         self,
         *,
         GroupName: str = ...,
         Group: str = ...,
         Filters: Sequence[ResourceFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListGroupResourcesOutputTypeDef:
         """
         Returns a list of ARNs of the resources that are members of a specified
         resource
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.list_group_resources)
@@ -218,15 +217,15 @@
         """
 
     def list_groups(
         self,
         *,
         Filters: Sequence[GroupFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListGroupsOutputTypeDef:
         """
         Returns a list of existing Resource Groups in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.list_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/client/#list_groups)
         """
```

### Comparing `mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups/client.pyi` & `mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     def create_group(
         self,
         *,
         Name: str,
         Description: str = ...,
         ResourceQuery: ResourceQueryTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        Configuration: Sequence[GroupConfigurationItemTypeDef] = ...
+        Configuration: Sequence[GroupConfigurationItemTypeDef] = ...,
     ) -> CreateGroupOutputTypeDef:
         """
         Creates a resource group with the specified name and description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.create_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/client/#create_group)
         """
@@ -198,15 +198,15 @@
     def list_group_resources(
         self,
         *,
         GroupName: str = ...,
         Group: str = ...,
         Filters: Sequence[ResourceFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListGroupResourcesOutputTypeDef:
         """
         Returns a list of ARNs of the resources that are members of a specified
         resource
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.list_group_resources)
@@ -214,15 +214,15 @@
         """
 
     def list_groups(
         self,
         *,
         Filters: Sequence[GroupFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListGroupsOutputTypeDef:
         """
         Returns a list of existing Resource Groups in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.list_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/client/#list_groups)
         """
```

### Comparing `mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups/literals.py` & `mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "GroupConfigurationStatusType",
     "GroupFilterNameType",
     "GroupLifecycleEventsDesiredStatusType",
     "GroupLifecycleEventsStatusType",
     "ListGroupResourcesPaginatorName",
     "ListGroupsPaginatorName",
@@ -35,25 +34,25 @@
     "ResourceGroupsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 GroupConfigurationStatusType = Literal["UPDATE_COMPLETE", "UPDATE_FAILED", "UPDATING"]
 GroupFilterNameType = Literal["configuration-type", "resource-type"]
 GroupLifecycleEventsDesiredStatusType = Literal["ACTIVE", "INACTIVE"]
 GroupLifecycleEventsStatusType = Literal["ACTIVE", "ERROR", "INACTIVE", "IN_PROGRESS"]
 ListGroupResourcesPaginatorName = Literal["list_group_resources"]
 ListGroupsPaginatorName = Literal["list_groups"]
 QueryErrorCodeType = Literal[
     "CLOUDFORMATION_STACK_INACTIVE",
     "CLOUDFORMATION_STACK_NOT_EXISTING",
     "CLOUDFORMATION_STACK_UNASSUMABLE_ROLE",
+    "RESOURCE_TYPE_NOT_SUPPORTED",
 ]
 QueryTypeType = Literal["CLOUDFORMATION_STACK_1_0", "TAG_FILTERS_1_0"]
 ResourceFilterNameType = Literal["resource-type"]
 ResourceStatusValueType = Literal["PENDING"]
 SearchResourcesPaginatorName = Literal["search_resources"]
 ResourceGroupsServiceName = Literal["resource-groups"]
 ServiceName = Literal[
@@ -78,14 +77,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -96,14 +96,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -121,14 +122,15 @@
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
@@ -151,14 +153,15 @@
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
@@ -219,15 +222,14 @@
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
@@ -299,17 +301,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -399,19 +403,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
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
@@ -454,14 +460,15 @@
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ap-southeast-4",
     "ca-central-1",
+    "ca-west-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
```

### Comparing `mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups/literals.pyi` & `mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 GroupLifecycleEventsStatusType = Literal["ACTIVE", "ERROR", "INACTIVE", "IN_PROGRESS"]
 ListGroupResourcesPaginatorName = Literal["list_group_resources"]
 ListGroupsPaginatorName = Literal["list_groups"]
 QueryErrorCodeType = Literal[
     "CLOUDFORMATION_STACK_INACTIVE",
     "CLOUDFORMATION_STACK_NOT_EXISTING",
     "CLOUDFORMATION_STACK_UNASSUMABLE_ROLE",
+    "RESOURCE_TYPE_NOT_SUPPORTED",
 ]
 QueryTypeType = Literal["CLOUDFORMATION_STACK_1_0", "TAG_FILTERS_1_0"]
 ResourceFilterNameType = Literal["resource-type"]
 ResourceStatusValueType = Literal["PENDING"]
 SearchResourcesPaginatorName = Literal["search_resources"]
 ResourceGroupsServiceName = Literal["resource-groups"]
 ServiceName = Literal[
@@ -76,14 +77,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -94,14 +96,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -119,14 +122,15 @@
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
@@ -149,14 +153,15 @@
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
@@ -217,15 +222,14 @@
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
@@ -297,17 +301,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -397,19 +403,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
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
@@ -452,14 +460,15 @@
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ap-southeast-4",
     "ca-central-1",
+    "ca-west-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
```

### Comparing `mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups/paginator.py` & `mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     ResourceFilterTypeDef,
     ResourceQueryTypeDef,
     SearchResourcesOutputTypeDef,
 )
 
 __all__ = ("ListGroupResourcesPaginator", "ListGroupsPaginator", "SearchResourcesPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -59,15 +58,15 @@
 
     def paginate(
         self,
         *,
         GroupName: str = ...,
         Group: str = ...,
         Filters: Sequence[ResourceFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListGroupResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.ListGroupResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/paginators/#listgroupresourcespaginator)
         """
 
 
@@ -77,15 +76,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/paginators/#listgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[GroupFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/paginators/#listgroupspaginator)
         """
```

### Comparing `mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups/paginator.pyi` & `mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
     def paginate(
         self,
         *,
         GroupName: str = ...,
         Group: str = ...,
         Filters: Sequence[ResourceFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListGroupResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.ListGroupResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/paginators/#listgroupresourcespaginator)
         """
 
 class ListGroupsPaginator(Paginator):
@@ -73,15 +73,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/paginators/#listgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[GroupFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/paginators/#listgroupspaginator)
         """
 
 class SearchResourcesPaginator(Paginator):
```

### Comparing `mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups/type_defs.py` & `mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountSettingsTypeDef",
     "ResourceQueryTypeDef",
     "GroupTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteGroupInputRequestTypeDef",
     "FailedResourceTypeDef",
@@ -119,18 +118,18 @@
         "Description": NotRequired[str],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 DeleteGroupInputRequestTypeDef = TypedDict(
     "DeleteGroupInputRequestTypeDef",
     {
         "GroupName": NotRequired[str],
         "Group": NotRequired[str],
```

### Comparing `mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups/type_defs.pyi` & `mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -118,18 +118,18 @@
         "Description": NotRequired[str],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 DeleteGroupInputRequestTypeDef = TypedDict(
     "DeleteGroupInputRequestTypeDef",
     {
         "GroupName": NotRequired[str],
         "Group": NotRequired[str],
```

### Comparing `mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups.egg-info/PKG-INFO` & `mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resource-groups
-Version: 1.34.0
-Summary: Type annotations for boto3.ResourceGroups 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.79
+Summary: Type annotations for boto3.ResourceGroups 1.34.79 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-resource-groups"></a>
 
 # mypy-boto3-resource-groups
 
 [![PyPI - mypy-boto3-resource-groups](https://img.shields.io/pypi/v/mypy-boto3-resource-groups.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-groups)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resource-groups.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-groups)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resource-groups)](https://pepy.tech/project/mypy-boto3-resource-groups)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceGroups 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
+[boto3.ResourceGroups 1.34.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-resource-groups docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-resource-groups-1.34.0/mypy_boto3_resource_groups.egg-info/SOURCES.txt` & `mypy-boto3-resource-groups-1.34.79/mypy_boto3_resource_groups.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.34.0/setup.py` & `mypy-boto3-resource-groups-1.34.79/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-resource-groups",
-    version="1.34.0",
+    version="1.34.79",
     packages=["mypy_boto3_resource_groups"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.ResourceGroups 1.34.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
-    ),
+    description="Type annotations for boto3.ResourceGroups 1.34.79 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Typing :: Typed",
+        "Typing :: Stubs Only",
     ],
     keywords="boto3 resource-groups type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_resource_groups": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

