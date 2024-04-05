# Comparing `tmp/stsmfa_cli-1.1.8.tar.gz` & `tmp/stsmfa_cli-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stsmfa_cli-1.1.8.tar", max compression
+gzip compressed data, was "stsmfa_cli-1.1.9.tar", max compression
```

## Comparing `stsmfa_cli-1.1.8.tar` & `stsmfa_cli-1.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2024-03-30 05:26:42.756442 stsmfa_cli-1.1.8/LICENSE
--rw-r--r--   0        0        0     5114 2024-03-30 05:26:42.756442 stsmfa_cli-1.1.8/README.md
--rw-r--r--   0        0        0     3250 2024-03-30 05:26:45.376448 stsmfa_cli-1.1.8/pyproject.toml
--rw-r--r--   0        0        0       22 2024-03-30 05:26:45.376448 stsmfa_cli-1.1.8/src/stsmfa/__init__.py
--rw-r--r--   0        0        0       59 2024-03-30 05:26:42.756442 stsmfa_cli-1.1.8/src/stsmfa/__maIn__.py
--rw-r--r--   0        0        0     2049 2024-03-30 05:26:42.756442 stsmfa_cli-1.1.8/src/stsmfa/cli.py
--rw-r--r--   0        0        0        0 2024-03-30 05:26:42.756442 stsmfa_cli-1.1.8/src/stsmfa/py.typed
--rw-r--r--   0        0        0     6366 1970-01-01 00:00:00.000000 stsmfa_cli-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-05 05:27:58.118639 stsmfa_cli-1.1.9/LICENSE
+-rw-r--r--   0        0        0     5114 2024-04-05 05:27:58.118639 stsmfa_cli-1.1.9/README.md
+-rw-r--r--   0        0        0     3250 2024-04-05 05:28:00.970690 stsmfa_cli-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-05 05:28:00.970690 stsmfa_cli-1.1.9/src/stsmfa/__init__.py
+-rw-r--r--   0        0        0       59 2024-04-05 05:27:58.118639 stsmfa_cli-1.1.9/src/stsmfa/__maIn__.py
+-rw-r--r--   0        0        0     2049 2024-04-05 05:27:58.118639 stsmfa_cli-1.1.9/src/stsmfa/cli.py
+-rw-r--r--   0        0        0        0 2024-04-05 05:27:58.118639 stsmfa_cli-1.1.9/src/stsmfa/py.typed
+-rw-r--r--   0        0        0     6366 1970-01-01 00:00:00.000000 stsmfa_cli-1.1.9/PKG-INFO
```

### Comparing `stsmfa_cli-1.1.8/LICENSE` & `stsmfa_cli-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stsmfa_cli-1.1.8/README.md` & `stsmfa_cli-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `stsmfa_cli-1.1.8/pyproject.toml` & `stsmfa_cli-1.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stsmfa-cli"
-version = "1.1.8"
+version = "1.1.9"
 description = "A small CLI to help with creating AWS profile for MFA protected sessions"
 authors = ["Bruno Alla <alla.brunoo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/browniebroke/stsmfa-cli"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

### Comparing `stsmfa_cli-1.1.8/src/stsmfa/cli.py` & `stsmfa_cli-1.1.9/src/stsmfa/cli.py`

 * *Files identical despite different names*

### Comparing `stsmfa_cli-1.1.8/PKG-INFO` & `stsmfa_cli-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stsmfa-cli
-Version: 1.1.8
+Version: 1.1.9
 Summary: A small CLI to help with creating AWS profile for MFA protected sessions
 Home-page: https://github.com/browniebroke/stsmfa-cli
 License: MIT
 Author: Bruno Alla
 Author-email: alla.brunoo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: stsmfa-cli Version: 1.1.8 Summary: A small CLI to
+Metadata-Version: 2.1 Name: stsmfa-cli Version: 1.1.9 Summary: A small CLI to
 help with creating AWS profile for MFA protected sessions Home-page: https://
 github.com/browniebroke/stsmfa-cli License: MIT Author: Bruno Alla Author-
 email: alla.brunoo@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

