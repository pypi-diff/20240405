# Comparing `tmp/rm_pycache-1.0.0.tar.gz` & `tmp/rm_pycache-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rm_pycache-1.0.0.tar", max compression
+gzip compressed data, was "rm_pycache-1.0.1.tar", max compression
```

## Comparing `rm_pycache-1.0.0.tar` & `rm_pycache-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1073 2024-04-05 06:56:43.728415 rm_pycache-1.0.0/LICENSE
--rw-r--r--   0        0        0      222 2024-04-05 08:00:32.735695 rm_pycache-1.0.0/README.md
--rw-r--r--   0        0        0      577 2024-04-05 07:37:47.774349 rm_pycache-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      942 2024-04-05 07:40:44.428482 rm_pycache-1.0.0/src/rm_pycache.py
--rw-r--r--   0        0        0      895 1970-01-01 00:00:00.000000 rm_pycache-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-05 06:56:43.728415 rm_pycache-1.0.1/LICENSE
+-rw-r--r--   0        0        0      222 2024-04-05 08:00:32.735695 rm_pycache-1.0.1/README.md
+-rw-r--r--   0        0        0      581 2024-04-05 15:51:46.826844 rm_pycache-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      941 2024-04-05 15:48:52.968755 rm_pycache-1.0.1/src/rm_pycache.py
+-rw-r--r--   0        0        0      899 1970-01-01 00:00:00.000000 rm_pycache-1.0.1/PKG-INFO
```

### Comparing `rm_pycache-1.0.0/LICENSE` & `rm_pycache-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rm_pycache-1.0.0/pyproject.toml` & `rm_pycache-1.0.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["poetry-core~=1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rm_pycache"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   "rapid537 <rapid537@zoho.com>",
 ]
 description = "Remove all __pycache__ in specified directory"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-homepage = "https://github.com/rapid537/op.git"
+homepage = "https://github.com/rapid537/rm_pycache"
 packages = [
     { include = "rm_pycache.py", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `rm_pycache-1.0.0/src/rm_pycache.py` & `rm_pycache-1.0.1/src/rm_pycache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import shutil
 
 
-def rm_pycache(path: str=None, stdout: bool=False) -> None or Exception:
+def rm_pycache(path: str=None, stdout: bool=False) -> None | Exception:
     """
     Delete all __pycache__ directories in the specified path.
 
     :param path: path to directory to search for __pycache__
     :type path: str
     :default path: current working directory
```

### Comparing `rm_pycache-1.0.0/PKG-INFO` & `rm_pycache-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: rm_pycache
-Version: 1.0.0
+Version: 1.0.1
 Summary: Remove all __pycache__ in specified directory
-Home-page: https://github.com/rapid537/op.git
+Home-page: https://github.com/rapid537/rm_pycache
 Author: rapid537
 Author-email: rapid537@zoho.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

