# Comparing `tmp/easyoutput-0.0.7.1.tar.gz` & `tmp/easyoutput-0.0.8.tar.gz`

## Comparing `easyoutput-0.0.7.1.tar` & `easyoutput-0.0.8.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 easyoutput-0.0.7.1/.github/ISSUE_TEMPLATE/🐞-bug-report.md
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 easyoutput-0.0.7.1/.github/ISSUE_TEMPLATE/🚀feature-request.md
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 easyoutput-0.0.7.1/src/EasyOutput/EasyOutput.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyoutput-0.0.7.1/src/EasyOutput/__init__.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 easyoutput-0.0.7.1/tests/test.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 easyoutput-0.0.7.1/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 easyoutput-0.0.7.1/LICENSE
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 easyoutput-0.0.7.1/README.md
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 easyoutput-0.0.7.1/pyproject.toml
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 easyoutput-0.0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 easyoutput-0.0.8/README.MD
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 easyoutput-0.0.8/.github/ISSUE_TEMPLATE/🐞-bug-report.md
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 easyoutput-0.0.8/.github/ISSUE_TEMPLATE/🚀feature-request.md
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 easyoutput-0.0.8/src/EasyOutput/EasyOutput.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 easyoutput-0.0.8/src/EasyOutput/__init__.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 easyoutput-0.0.8/tests/test.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 easyoutput-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 easyoutput-0.0.8/LICENSE
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 easyoutput-0.0.8/README.md
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 easyoutput-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3871 2020-02-02 00:00:00.000000 easyoutput-0.0.8/PKG-INFO
```

### Comparing `easyoutput-0.0.7.1/.github/ISSUE_TEMPLATE/🚀feature-request.md` & `easyoutput-0.0.8/.github/ISSUE_TEMPLATE/🚀feature-request.md`

 * *Files identical despite different names*

### Comparing `easyoutput-0.0.7.1/LICENSE` & `easyoutput-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `easyoutput-0.0.7.1/pyproject.toml` & `easyoutput-0.0.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EasyOutput"
-version = "0.0.7.1"
+version = "0.0.8"
 authors = [
   { name="FrankAustin", email="frankaustindev808@gmail.com" },
 ]
 description = "Colored messages in the palm of your hand"
 readme = "README.md"
 requires-python = ">=3.12"
 install_requires=['colorama']
 classifiers=[
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "Operating System :: Unix",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
 ]
```

