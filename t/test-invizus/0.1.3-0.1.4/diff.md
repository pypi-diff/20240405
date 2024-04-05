# Comparing `tmp/test_invizus-0.1.3.tar.gz` & `tmp/test_invizus-0.1.4.tar.gz`

## Comparing `test_invizus-0.1.3.tar` & `test_invizus-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,14 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 test_invizus-0.1.3/src/test_invizus/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 test_invizus-0.1.3/src/test_invizus/invizus-test.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 test_invizus-0.1.3/LICENCE
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 test_invizus-0.1.3/README.md
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 test_invizus-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 test_invizus-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 test_invizus-0.1.4/dist2/test_invizus-0.1.0-py3-none-any.whl
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 test_invizus-0.1.4/dist2/test_invizus-0.1.0.tar.gz
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 test_invizus-0.1.4/dist2/test_invizus-0.1.1-py3-none-any.whl
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 test_invizus-0.1.4/dist2/test_invizus-0.1.1.tar.gz
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 test_invizus-0.1.4/dist2/test_invizus-0.1.2-py3-none-any.whl
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 test_invizus-0.1.4/dist2/test_invizus-0.1.2.tar.gz
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 test_invizus-0.1.4/dist2/test_invizus-0.1.3-py3-none-any.whl
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 test_invizus-0.1.4/dist2/test_invizus-0.1.3.tar.gz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 test_invizus-0.1.4/src/test_invizus/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 test_invizus-0.1.4/src/test_invizus/invizus-test.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 test_invizus-0.1.4/LICENCE
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 test_invizus-0.1.4/README.md
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 test_invizus-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 test_invizus-0.1.4/PKG-INFO
```

### Comparing `test_invizus-0.1.3/pyproject.toml` & `test_invizus-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "test_invizus"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="invizus", email="invizus@gmail.com" },
 ]
 description = "Testing docker build"
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
```

### Comparing `test_invizus-0.1.3/PKG-INFO` & `test_invizus-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: test_invizus
-Version: 0.1.3
+Version: 0.1.4
 Summary: Testing docker build
 Project-URL: Homepage, https://github.com/invizus/sampleproject
 Project-URL: Issues, https://github.com/invizus/sampleproject/issues
 Author-email: invizus <invizus@gmail.com>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

