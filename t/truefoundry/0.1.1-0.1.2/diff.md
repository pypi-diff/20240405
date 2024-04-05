# Comparing `tmp/truefoundry-0.1.1.tar.gz` & `tmp/truefoundry-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truefoundry-0.1.1.tar", max compression
+gzip compressed data, was "truefoundry-0.1.2.tar", max compression
```

## Comparing `truefoundry-0.1.1.tar` & `truefoundry-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      871 2024-04-03 07:22:03.172516 truefoundry-0.1.1/README.md
--rw-r--r--   0        0        0      655 2024-04-03 07:22:14.400750 truefoundry-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-03 07:22:03.176516 truefoundry-0.1.1/truefoundry/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 07:22:03.176516 truefoundry-0.1.1/truefoundry/cli/__init__.py
--rw-r--r--   0        0        0      794 2024-04-03 07:22:03.176516 truefoundry-0.1.1/truefoundry/cli/__main__.py
--rw-r--r--   0        0        0       29 2024-04-03 07:22:03.176516 truefoundry-0.1.1/truefoundry/deploy/__init__.py
--rw-r--r--   0        0        0       39 2024-04-03 07:22:03.176516 truefoundry-0.1.1/truefoundry/langchain/__init__.py
--rw-r--r--   0        0        0      151 2024-04-03 07:22:03.176516 truefoundry-0.1.1/truefoundry/ml/__init__.py
--rw-r--r--   0        0        0     1502 1970-01-01 00:00:00.000000 truefoundry-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      871 2024-04-05 17:00:29.485450 truefoundry-0.1.2/README.md
+-rw-r--r--   0        0        0      655 2024-04-05 17:00:40.725604 truefoundry-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-05 17:00:29.485450 truefoundry-0.1.2/truefoundry/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 17:00:29.489450 truefoundry-0.1.2/truefoundry/cli/__init__.py
+-rw-r--r--   0        0        0      794 2024-04-05 17:00:29.489450 truefoundry-0.1.2/truefoundry/cli/__main__.py
+-rw-r--r--   0        0        0       29 2024-04-05 17:00:29.489450 truefoundry-0.1.2/truefoundry/deploy/__init__.py
+-rw-r--r--   0        0        0       39 2024-04-05 17:00:29.489450 truefoundry-0.1.2/truefoundry/langchain/__init__.py
+-rw-r--r--   0        0        0      151 2024-04-05 17:00:29.489450 truefoundry-0.1.2/truefoundry/ml/__init__.py
+-rw-r--r--   0        0        0     1502 1970-01-01 00:00:00.000000 truefoundry-0.1.2/PKG-INFO
```

### Comparing `truefoundry-0.1.1/README.md` & `truefoundry-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `truefoundry-0.1.1/pyproject.toml` & `truefoundry-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "truefoundry"
-version = "0.1.1"
+version = "0.1.2"
 description = "Truefoundry CLI"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.13"
-servicefoundry = "0.10.5"
-mlfoundry = { version = "0.10.8", optional = true }
+servicefoundry = "0.10.6"
+mlfoundry = { version = "0.10.9", optional = true }
 
 [tool.poetry.extras]
 ml = ["mlfoundry"]
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `truefoundry-0.1.1/truefoundry/cli/__main__.py` & `truefoundry-0.1.2/truefoundry/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.1.1/PKG-INFO` & `truefoundry-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: truefoundry
-Version: 0.1.1
+Version: 0.1.2
 Summary: Truefoundry CLI
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: ml
-Requires-Dist: mlfoundry (==0.10.8) ; extra == "ml"
-Requires-Dist: servicefoundry (==0.10.5)
+Requires-Dist: mlfoundry (==0.10.9) ; extra == "ml"
+Requires-Dist: servicefoundry (==0.10.6)
 Description-Content-Type: text/markdown
 
 # Truefoundry
 
 TrueFoundry library to help you interact with the platform programmatically by
 
 - Interacting with the deployments side of TrueFoundry, enabling you to manage workspaces, deployments, applications, and view logs.
```

