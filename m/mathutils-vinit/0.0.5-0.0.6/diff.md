# Comparing `tmp/mathutils_vinit-0.0.5.tar.gz` & `tmp/mathutils_vinit-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathutils_vinit-0.0.5.tar", last modified: Fri Apr  5 12:46:05 2024, max compression
+gzip compressed data, was "mathutils_vinit-0.0.6.tar", last modified: Fri Apr  5 13:15:17 2024, max compression
```

## Comparing `mathutils_vinit-0.0.5.tar` & `mathutils_vinit-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 12:46:05.634426 mathutils_vinit-0.0.5/
--rw-r--r--   0 vinitsarode   (501) staff       (20)     1073 2024-03-24 13:56:05.000000 mathutils_vinit-0.0.5/LICENSE
--rw-r--r--   0 vinitsarode   (501) staff       (20)      567 2024-04-05 12:46:05.634171 mathutils_vinit-0.0.5/PKG-INFO
--rw-r--r--   0 vinitsarode   (501) staff       (20)       34 2024-03-24 13:55:43.000000 mathutils_vinit-0.0.5/README.md
--rw-r--r--   0 vinitsarode   (501) staff       (20)      584 2024-04-05 12:45:52.000000 mathutils_vinit-0.0.5/pyproject.toml
--rw-r--r--   0 vinitsarode   (501) staff       (20)       13 2024-04-05 12:45:49.000000 mathutils_vinit-0.0.5/requirements.txt
--rw-r--r--   0 vinitsarode   (501) staff       (20)       38 2024-04-05 12:46:05.634469 mathutils_vinit-0.0.5/setup.cfg
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 12:46:05.631501 mathutils_vinit-0.0.5/src/
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 12:46:05.632903 mathutils_vinit-0.0.5/src/mathutils_vinit/
--rw-r--r--   0 vinitsarode   (501) staff       (20)       44 2024-04-05 12:32:10.000000 mathutils_vinit-0.0.5/src/mathutils_vinit/__init__.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)      143 2024-03-24 13:30:14.000000 mathutils_vinit-0.0.5/src/mathutils_vinit/operations.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)      133 2024-04-05 12:31:59.000000 mathutils_vinit-0.0.5/src/mathutils_vinit/roots.py
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 12:46:05.633899 mathutils_vinit-0.0.5/src/mathutils_vinit.egg-info/
--rw-r--r--   0 vinitsarode   (501) staff       (20)      567 2024-04-05 12:46:05.000000 mathutils_vinit-0.0.5/src/mathutils_vinit.egg-info/PKG-INFO
--rw-r--r--   0 vinitsarode   (501) staff       (20)      358 2024-04-05 12:46:05.000000 mathutils_vinit-0.0.5/src/mathutils_vinit.egg-info/SOURCES.txt
--rw-r--r--   0 vinitsarode   (501) staff       (20)        1 2024-04-05 12:46:05.000000 mathutils_vinit-0.0.5/src/mathutils_vinit.egg-info/dependency_links.txt
--rw-r--r--   0 vinitsarode   (501) staff       (20)       14 2024-04-05 12:46:05.000000 mathutils_vinit-0.0.5/src/mathutils_vinit.egg-info/requires.txt
--rw-r--r--   0 vinitsarode   (501) staff       (20)       16 2024-04-05 12:46:05.000000 mathutils_vinit-0.0.5/src/mathutils_vinit.egg-info/top_level.txt
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 13:15:17.153825 mathutils_vinit-0.0.6/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     1073 2024-03-24 13:56:05.000000 mathutils_vinit-0.0.6/LICENSE
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      567 2024-04-05 13:15:17.153536 mathutils_vinit-0.0.6/PKG-INFO
+-rw-r--r--   0 vinitsarode   (501) staff       (20)       34 2024-03-24 13:55:43.000000 mathutils_vinit-0.0.6/README.md
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      722 2024-04-05 13:14:45.000000 mathutils_vinit-0.0.6/pyproject.toml
+-rw-r--r--   0 vinitsarode   (501) staff       (20)       13 2024-04-05 12:45:49.000000 mathutils_vinit-0.0.6/requirements.txt
+-rw-r--r--   0 vinitsarode   (501) staff       (20)       38 2024-04-05 13:15:17.153871 mathutils_vinit-0.0.6/setup.cfg
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 13:15:17.150529 mathutils_vinit-0.0.6/src/
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 13:15:17.150667 mathutils_vinit-0.0.6/src/source/
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 13:15:17.152234 mathutils_vinit-0.0.6/src/source/mathutils_vinit/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)       44 2024-04-05 12:32:10.000000 mathutils_vinit-0.0.6/src/source/mathutils_vinit/__init__.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      143 2024-03-24 13:30:14.000000 mathutils_vinit-0.0.6/src/source/mathutils_vinit/operations.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      133 2024-04-05 12:31:59.000000 mathutils_vinit-0.0.6/src/source/mathutils_vinit/roots.py
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 13:15:17.153285 mathutils_vinit-0.0.6/src/source/mathutils_vinit.egg-info/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      567 2024-04-05 13:15:17.000000 mathutils_vinit-0.0.6/src/source/mathutils_vinit.egg-info/PKG-INFO
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      414 2024-04-05 13:15:17.000000 mathutils_vinit-0.0.6/src/source/mathutils_vinit.egg-info/SOURCES.txt
+-rw-r--r--   0 vinitsarode   (501) staff       (20)        1 2024-04-05 13:15:17.000000 mathutils_vinit-0.0.6/src/source/mathutils_vinit.egg-info/dependency_links.txt
+-rw-r--r--   0 vinitsarode   (501) staff       (20)       14 2024-04-05 13:15:17.000000 mathutils_vinit-0.0.6/src/source/mathutils_vinit.egg-info/requires.txt
+-rw-r--r--   0 vinitsarode   (501) staff       (20)       16 2024-04-05 13:15:17.000000 mathutils_vinit-0.0.6/src/source/mathutils_vinit.egg-info/top_level.txt
```

### Comparing `mathutils_vinit-0.0.5/LICENSE` & `mathutils_vinit-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mathutils_vinit-0.0.5/PKG-INFO` & `mathutils_vinit-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathutils_vinit
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small example package
 Author-email: vinit sarode <vinitsarode5@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mathutils_vinit-0.0.5/pyproject.toml` & `mathutils_vinit-0.0.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,29 @@
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
+
 [project]
 name = "mathutils_vinit"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     { name="vinit sarode", email="vinitsarode5@gmail.com"},
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dynamic = ["dependencies"]
 
+[tool.setuptools.packages.find]
+where = ["src/source"]
+
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
 [project.urls]
 Homepage = "https://github.com/pypa/sampleproject"
 Issues = "https://github.com/pypa/sampleproject/issues"
```

### Comparing `mathutils_vinit-0.0.5/src/mathutils_vinit.egg-info/PKG-INFO` & `mathutils_vinit-0.0.6/src/source/mathutils_vinit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathutils_vinit
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small example package
 Author-email: vinit sarode <vinitsarode5@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

