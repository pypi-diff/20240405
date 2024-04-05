# Comparing `tmp/test_invizus-0.1.0.tar.gz` & `tmp/test_invizus-0.1.1.tar.gz`

## Comparing `test_invizus-0.1.0.tar` & `test_invizus-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 test_invizus-0.1.0/src/test_invizus/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 test_invizus-0.1.0/src/test_invizus/invizus-test.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 test_invizus-0.1.0/LICENCE
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 test_invizus-0.1.0/README.md
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 test_invizus-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 test_invizus-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 test_invizus-0.1.1/src/test_invizus/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 test_invizus-0.1.1/src/test_invizus/invizus-test.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 test_invizus-0.1.1/LICENCE
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 test_invizus-0.1.1/README.md
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 test_invizus-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 test_invizus-0.1.1/PKG-INFO
```

### Comparing `test_invizus-0.1.0/pyproject.toml` & `test_invizus-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "test_invizus"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="invizus", email="invizus@gmail.com" },
 ]
 description = "Testing docker build"
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
```

### Comparing `test_invizus-0.1.0/PKG-INFO` & `test_invizus-0.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: test_invizus
-Version: 0.1.0
+Version: 0.1.1
 Summary: Testing docker build
 Project-URL: Homepage, https://github.com/invizus/sampleproject
 Project-URL: Issues, https://github.com/invizus/sampleproject/issues
 Author-email: invizus <invizus@gmail.com>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

