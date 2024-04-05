# Comparing `tmp/mathutils_vinit-0.0.4.tar.gz` & `tmp/mathutils_vinit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathutils_vinit-0.0.4.tar", last modified: Fri Apr  5 12:38:33 2024, max compression
+gzip compressed data, was "mathutils_vinit-0.0.5.tar", last modified: Fri Apr  5 12:46:05 2024, max compression
```

## Comparing `mathutils_vinit-0.0.4.tar` & `mathutils_vinit-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 12:38:33.129616 mathutils_vinit-0.0.4/
--rw-r--r--   0 vinitsarode   (501) staff       (20)     1073 2024-03-24 13:56:05.000000 mathutils_vinit-0.0.4/LICENSE
--rw-r--r--   0 vinitsarode   (501) staff       (20)      538 2024-04-05 12:38:33.129355 mathutils_vinit-0.0.4/PKG-INFO
--rw-r--r--   0 vinitsarode   (501) staff       (20)       34 2024-03-24 13:55:43.000000 mathutils_vinit-0.0.4/README.md
--rw-r--r--   0 vinitsarode   (501) staff       (20)      485 2024-04-05 12:38:21.000000 mathutils_vinit-0.0.4/pyproject.toml
--rw-r--r--   0 vinitsarode   (501) staff       (20)       38 2024-04-05 12:38:33.129667 mathutils_vinit-0.0.4/setup.cfg
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 12:38:33.126779 mathutils_vinit-0.0.4/src/
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 12:38:33.128159 mathutils_vinit-0.0.4/src/mathutils_vinit/
--rw-r--r--   0 vinitsarode   (501) staff       (20)       44 2024-04-05 12:32:10.000000 mathutils_vinit-0.0.4/src/mathutils_vinit/__init__.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)      143 2024-03-24 13:30:14.000000 mathutils_vinit-0.0.4/src/mathutils_vinit/operations.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)      133 2024-04-05 12:31:59.000000 mathutils_vinit-0.0.4/src/mathutils_vinit/roots.py
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 12:38:33.129111 mathutils_vinit-0.0.4/src/mathutils_vinit.egg-info/
--rw-r--r--   0 vinitsarode   (501) staff       (20)      538 2024-04-05 12:38:33.000000 mathutils_vinit-0.0.4/src/mathutils_vinit.egg-info/PKG-INFO
--rw-r--r--   0 vinitsarode   (501) staff       (20)      299 2024-04-05 12:38:33.000000 mathutils_vinit-0.0.4/src/mathutils_vinit.egg-info/SOURCES.txt
--rw-r--r--   0 vinitsarode   (501) staff       (20)        1 2024-04-05 12:38:33.000000 mathutils_vinit-0.0.4/src/mathutils_vinit.egg-info/dependency_links.txt
--rw-r--r--   0 vinitsarode   (501) staff       (20)       16 2024-04-05 12:38:33.000000 mathutils_vinit-0.0.4/src/mathutils_vinit.egg-info/top_level.txt
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 12:46:05.634426 mathutils_vinit-0.0.5/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     1073 2024-03-24 13:56:05.000000 mathutils_vinit-0.0.5/LICENSE
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      567 2024-04-05 12:46:05.634171 mathutils_vinit-0.0.5/PKG-INFO
+-rw-r--r--   0 vinitsarode   (501) staff       (20)       34 2024-03-24 13:55:43.000000 mathutils_vinit-0.0.5/README.md
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      584 2024-04-05 12:45:52.000000 mathutils_vinit-0.0.5/pyproject.toml
+-rw-r--r--   0 vinitsarode   (501) staff       (20)       13 2024-04-05 12:45:49.000000 mathutils_vinit-0.0.5/requirements.txt
+-rw-r--r--   0 vinitsarode   (501) staff       (20)       38 2024-04-05 12:46:05.634469 mathutils_vinit-0.0.5/setup.cfg
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 12:46:05.631501 mathutils_vinit-0.0.5/src/
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 12:46:05.632903 mathutils_vinit-0.0.5/src/mathutils_vinit/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)       44 2024-04-05 12:32:10.000000 mathutils_vinit-0.0.5/src/mathutils_vinit/__init__.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      143 2024-03-24 13:30:14.000000 mathutils_vinit-0.0.5/src/mathutils_vinit/operations.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      133 2024-04-05 12:31:59.000000 mathutils_vinit-0.0.5/src/mathutils_vinit/roots.py
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 12:46:05.633899 mathutils_vinit-0.0.5/src/mathutils_vinit.egg-info/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      567 2024-04-05 12:46:05.000000 mathutils_vinit-0.0.5/src/mathutils_vinit.egg-info/PKG-INFO
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      358 2024-04-05 12:46:05.000000 mathutils_vinit-0.0.5/src/mathutils_vinit.egg-info/SOURCES.txt
+-rw-r--r--   0 vinitsarode   (501) staff       (20)        1 2024-04-05 12:46:05.000000 mathutils_vinit-0.0.5/src/mathutils_vinit.egg-info/dependency_links.txt
+-rw-r--r--   0 vinitsarode   (501) staff       (20)       14 2024-04-05 12:46:05.000000 mathutils_vinit-0.0.5/src/mathutils_vinit.egg-info/requires.txt
+-rw-r--r--   0 vinitsarode   (501) staff       (20)       16 2024-04-05 12:46:05.000000 mathutils_vinit-0.0.5/src/mathutils_vinit.egg-info/top_level.txt
```

### Comparing `mathutils_vinit-0.0.4/LICENSE` & `mathutils_vinit-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mathutils_vinit-0.0.4/PKG-INFO` & `mathutils_vinit-0.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: mathutils_vinit
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small example package
 Author-email: vinit sarode <vinitsarode5@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pytest==8.1.1
 
 ### mathutils_vinit
 
 operations.py
```

### Comparing `mathutils_vinit-0.0.4/src/mathutils_vinit.egg-info/PKG-INFO` & `mathutils_vinit-0.0.5/src/mathutils_vinit.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: mathutils_vinit
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small example package
 Author-email: vinit sarode <vinitsarode5@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pytest==8.1.1
 
 ### mathutils_vinit
 
 operations.py
```

