# Comparing `tmp/mypy-boto3-quicksight-1.34.73.tar.gz` & `tmp/mypy-boto3-quicksight-1.34.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-quicksight-1.34.73.tar", last modified: Thu Mar 28 19:34:43 2024, max compression
+gzip compressed data, was "mypy-boto3-quicksight-1.34.79.tar", last modified: Fri Apr  5 19:20:34 2024, max compression
```

## Comparing `mypy-boto3-quicksight-1.34.73.tar` & `mypy-boto3-quicksight-1.34.79.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:34:43.036079 mypy-boto3-quicksight-1.34.73/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-28 19:34:16.000000 mypy-boto3-quicksight-1.34.73/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17061 2024-03-28 19:34:43.036079 mypy-boto3-quicksight-1.34.73/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15494 2024-03-28 19:34:16.000000 mypy-boto3-quicksight-1.34.73/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:34:43.036079 mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight/
--rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-03-28 19:34:16.000000 mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-03-28 19:34:16.000000 mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-28 19:34:16.000000 mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   135042 2024-03-28 19:34:17.000000 mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   135039 2024-03-28 19:34:16.000000 mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    39634 2024-03-28 19:34:17.000000 mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    39634 2024-03-28 19:34:17.000000 mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    36169 2024-03-28 19:34:17.000000 mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    36137 2024-03-28 19:34:17.000000 mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 19:34:16.000000 mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   381606 2024-03-28 19:34:28.000000 mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   381606 2024-03-28 19:34:24.000000 mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-28 19:34:16.000000 mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:34:43.036079 mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17061 2024-03-28 19:34:43.000000 mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-28 19:34:43.000000 mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:34:43.000000 mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:34:43.000000 mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-28 19:34:43.000000 mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-28 19:34:43.000000 mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 19:34:43.036079 mypy-boto3-quicksight-1.34.73/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-03-28 19:34:15.000000 mypy-boto3-quicksight-1.34.73/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:20:34.734695 mypy-boto3-quicksight-1.34.79/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-05 19:20:07.000000 mypy-boto3-quicksight-1.34.79/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17061 2024-04-05 19:20:34.734695 mypy-boto3-quicksight-1.34.79/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15494 2024-04-05 19:20:07.000000 mypy-boto3-quicksight-1.34.79/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:20:34.730695 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/
+-rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-05 19:20:07.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-05 19:20:07.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-05 19:20:07.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   135091 2024-04-05 19:20:11.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   135088 2024-04-05 19:20:08.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    39673 2024-04-05 19:20:12.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39673 2024-04-05 19:20:12.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    36169 2024-04-05 19:20:12.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36137 2024-04-05 19:20:11.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:20:07.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   381664 2024-04-05 19:20:19.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   381664 2024-04-05 19:20:17.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-05 19:20:07.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:20:34.734695 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17061 2024-04-05 19:20:34.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-05 19:20:34.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:20:34.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:20:34.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-05 19:20:34.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-05 19:20:34.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 19:20:34.734695 mypy-boto3-quicksight-1.34.79/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-05 19:20:07.000000 mypy-boto3-quicksight-1.34.79/setup.py
```

### Comparing `mypy-boto3-quicksight-1.34.73/LICENSE` & `mypy-boto3-quicksight-1.34.79/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.34.73/PKG-INFO` & `mypy-boto3-quicksight-1.34.79/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-quicksight
-Version: 1.34.73
-Summary: Type annotations for boto3.QuickSight 1.34.73 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.79
+Summary: Type annotations for boto3.QuickSight 1.34.79 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-quicksight.svg?color=blue)](https://pypi.org/project/mypy-boto3-quicksight)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-quicksight)](https://pepy.tech/project/mypy-boto3-quicksight)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QuickSight 1.34.73](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
+[boto3.QuickSight 1.34.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-quicksight-1.34.73/README.md` & `mypy-boto3-quicksight-1.34.79/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-quicksight.svg?color=blue)](https://pypi.org/project/mypy-boto3-quicksight)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-quicksight)](https://pepy.tech/project/mypy-boto3-quicksight)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QuickSight 1.34.73](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
+[boto3.QuickSight 1.34.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight/__init__.py` & `mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight/__init__.pyi` & `mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight/__main__.py` & `mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.QuickSight 1.34.73\n"
-        "Version:         1.34.73\n"
+        "Type annotations for boto3.QuickSight 1.34.79\n"
+        "Version:         1.34.79\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.73")
+    print("1.34.79")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight/client.py` & `mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,14 +405,15 @@
         AdminGroup: Sequence[str] = ...,
         AuthorGroup: Sequence[str] = ...,
         ReaderGroup: Sequence[str] = ...,
         FirstName: str = ...,
         LastName: str = ...,
         EmailAddress: str = ...,
         ContactNumber: str = ...,
+        IAMIdentityCenterInstanceArn: str = ...,
     ) -> CreateAccountSubscriptionResponseTypeDef:
         """
         Creates an Amazon QuickSight account, or subscribes to Amazon QuickSight Q.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_account_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_account_subscription)
         """
```

### Comparing `mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight/client.pyi` & `mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -402,14 +402,15 @@
         AdminGroup: Sequence[str] = ...,
         AuthorGroup: Sequence[str] = ...,
         ReaderGroup: Sequence[str] = ...,
         FirstName: str = ...,
         LastName: str = ...,
         EmailAddress: str = ...,
         ContactNumber: str = ...,
+        IAMIdentityCenterInstanceArn: str = ...,
     ) -> CreateAccountSubscriptionResponseTypeDef:
         """
         Creates an Amazon QuickSight account, or subscribes to Amazon QuickSight Q.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_account_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_account_subscription)
         """
```

### Comparing `mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight/literals.py` & `mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -933,14 +933,15 @@
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
@@ -963,14 +964,15 @@
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
```

### Comparing `mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight/literals.pyi` & `mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -933,14 +933,15 @@
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
@@ -963,14 +964,15 @@
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
```

### Comparing `mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight/paginator.py` & `mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight/paginator.pyi` & `mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight/type_defs.py` & `mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2058,14 +2058,15 @@
         "AdminGroup": NotRequired[Sequence[str]],
         "AuthorGroup": NotRequired[Sequence[str]],
         "ReaderGroup": NotRequired[Sequence[str]],
         "FirstName": NotRequired[str],
         "LastName": NotRequired[str],
         "EmailAddress": NotRequired[str],
         "ContactNumber": NotRequired[str],
+        "IAMIdentityCenterInstanceArn": NotRequired[str],
     },
 )
 SignupResponseTypeDef = TypedDict(
     "SignupResponseTypeDef",
     {
         "IAMUser": NotRequired[bool],
         "userLoginName": NotRequired[str],
```

### Comparing `mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight/type_defs.pyi` & `mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2058,14 +2058,15 @@
         "AdminGroup": NotRequired[Sequence[str]],
         "AuthorGroup": NotRequired[Sequence[str]],
         "ReaderGroup": NotRequired[Sequence[str]],
         "FirstName": NotRequired[str],
         "LastName": NotRequired[str],
         "EmailAddress": NotRequired[str],
         "ContactNumber": NotRequired[str],
+        "IAMIdentityCenterInstanceArn": NotRequired[str],
     },
 )
 SignupResponseTypeDef = TypedDict(
     "SignupResponseTypeDef",
     {
         "IAMUser": NotRequired[bool],
         "userLoginName": NotRequired[str],
```

### Comparing `mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight.egg-info/PKG-INFO` & `mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-quicksight
-Version: 1.34.73
-Summary: Type annotations for boto3.QuickSight 1.34.73 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.79
+Summary: Type annotations for boto3.QuickSight 1.34.79 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-quicksight.svg?color=blue)](https://pypi.org/project/mypy-boto3-quicksight)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-quicksight)](https://pepy.tech/project/mypy-boto3-quicksight)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QuickSight 1.34.73](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
+[boto3.QuickSight 1.34.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-quicksight-1.34.73/mypy_boto3_quicksight.egg-info/SOURCES.txt` & `mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.34.73/setup.py` & `mypy-boto3-quicksight-1.34.79/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-quicksight",
-    version="1.34.73",
+    version="1.34.79",
     packages=["mypy_boto3_quicksight"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.QuickSight 1.34.73 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.QuickSight 1.34.79 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

