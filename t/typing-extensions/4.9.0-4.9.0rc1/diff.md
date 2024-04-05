# Comparing `tmp/typing_extensions-4.9.0.tar.gz` & `tmp/typing_extensions-4.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typing_extensions-4.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "typing_extensions-4.9.0rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `typing_extensions-4.9.0.tar` & `typing_extensions-4.9.0rc1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    17794 2023-12-10 01:10:08.541661 typing_extensions-4.9.0/CHANGELOG.md
--rw-r--r--   0        0        0    13936 2023-06-01 23:37:58.110406 typing_extensions-4.9.0/LICENSE
--rw-r--r--   0        0        0     1469 2023-08-30 00:40:02.754719 typing_extensions-4.9.0/README.md
--rw-r--r--   0        0        0     1917 2023-12-10 01:10:17.241821 typing_extensions-4.9.0/pyproject.toml
--rw-r--r--   0        0        0      563 2023-06-15 04:06:19.836805 typing_extensions-4.9.0/src/_typed_dict_test_helper.py
--rw-r--r--   0        0        0   214746 2023-11-29 17:46:32.803016 typing_extensions-4.9.0/src/test_typing_extensions.py
--rw-r--r--   0        0        0   110125 2023-11-29 17:46:32.803519 typing_extensions-4.9.0/src/typing_extensions.py
--rw-r--r--   0        0        0      143 2023-11-29 02:00:24.530703 typing_extensions-4.9.0/tox.ini
--rw-r--r--   0        0        0     2966 1970-01-01 00:00:00.000000 typing_extensions-4.9.0/PKG-INFO
+-rw-r--r--   0        0        0    17551 2023-11-29 18:14:36.089886 typing_extensions-4.9.0rc1/CHANGELOG.md
+-rw-r--r--   0        0        0    13936 2023-06-01 23:37:58.110406 typing_extensions-4.9.0rc1/LICENSE
+-rw-r--r--   0        0        0     1469 2023-08-30 00:40:02.754719 typing_extensions-4.9.0rc1/README.md
+-rw-r--r--   0        0        0     1920 2023-11-29 18:14:36.090198 typing_extensions-4.9.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      563 2023-06-15 04:06:19.836805 typing_extensions-4.9.0rc1/src/_typed_dict_test_helper.py
+-rw-r--r--   0        0        0   214746 2023-11-29 17:46:32.803016 typing_extensions-4.9.0rc1/src/test_typing_extensions.py
+-rw-r--r--   0        0        0   110125 2023-11-29 17:46:32.803519 typing_extensions-4.9.0rc1/src/typing_extensions.py
+-rw-r--r--   0        0        0      143 2023-11-29 02:00:24.530703 typing_extensions-4.9.0rc1/tox.ini
+-rw-r--r--   0        0        0     2969 1970-01-01 00:00:00.000000 typing_extensions-4.9.0rc1/PKG-INFO
```

### Comparing `typing_extensions-4.9.0/CHANGELOG.md` & `typing_extensions-4.9.0rc1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-# Release 4.9.0 (December 9, 2023)
-
-This feature release adds `typing_extensions.ReadOnly`, as specified
-by PEP 705, and makes various other improvements, especially to
-`@typing_extensions.deprecated()`.
-
-There are no changes since 4.9.0rc1.
-
 # Release 4.9.0rc1 (November 29, 2023)
 
 - Add support for PEP 705, adding `typing_extensions.ReadOnly`. Patch
   by Jelle Zijlstra.
 - All parameters on `NewType.__call__` are now positional-only. This means that
   the signature of `typing_extensions.NewType.__call__` now exactly matches the
   signature of `typing.NewType.__call__`. Patch by Alex Waygood.
```

### Comparing `typing_extensions-4.9.0/LICENSE` & `typing_extensions-4.9.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `typing_extensions-4.9.0/README.md` & `typing_extensions-4.9.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `typing_extensions-4.9.0/pyproject.toml` & `typing_extensions-4.9.0rc1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["flit_core >=3.4,<4"]
 build-backend = "flit_core.buildapi"
 
 # Project metadata
 [project]
 name = "typing_extensions"
-version = "4.9.0"
+version = "4.9.0rc1"
 description = "Backported and Experimental Type Hints for Python 3.8+"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = [
     "annotations",
     "backport",
```

### Comparing `typing_extensions-4.9.0/src/_typed_dict_test_helper.py` & `typing_extensions-4.9.0rc1/src/_typed_dict_test_helper.py`

 * *Files identical despite different names*

### Comparing `typing_extensions-4.9.0/src/test_typing_extensions.py` & `typing_extensions-4.9.0rc1/src/test_typing_extensions.py`

 * *Files identical despite different names*

### Comparing `typing_extensions-4.9.0/src/typing_extensions.py` & `typing_extensions-4.9.0rc1/src/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `typing_extensions-4.9.0/PKG-INFO` & `typing_extensions-4.9.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typing_extensions
-Version: 4.9.0
+Version: 4.9.0rc1
 Summary: Backported and Experimental Type Hints for Python 3.8+
 Keywords: annotations,backport,checker,checking,function,hinting,hints,type,typechecking,typehinting,typehints,typing
 Author-email: "Guido van Rossum, Jukka Lehtosalo, Łukasz Langa, Michael Lee" <levkivskyi@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

