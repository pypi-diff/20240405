# Comparing `tmp/mathutils_vinit-0.0.3.tar.gz` & `tmp/mathutils_vinit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathutils_vinit-0.0.3.tar", last modified: Sun Mar 24 14:41:43 2024, max compression
+gzip compressed data, was "mathutils_vinit-0.0.4.tar", last modified: Fri Apr  5 12:38:33 2024, max compression
```

## Comparing `mathutils_vinit-0.0.3.tar` & `mathutils_vinit-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-03-24 14:41:43.447893 mathutils_vinit-0.0.3/
--rw-rw-r--   0 oem      (29999) oem      (29999)     1073 2024-03-24 13:56:05.000000 mathutils_vinit-0.0.3/LICENSE
--rw-r--r--   0 oem      (29999) oem      (29999)      538 2024-03-24 14:41:43.447893 mathutils_vinit-0.0.3/PKG-INFO
--rw-rw-r--   0 oem      (29999) oem      (29999)       34 2024-03-24 13:55:43.000000 mathutils_vinit-0.0.3/README.md
--rw-rw-r--   0 oem      (29999) oem      (29999)      485 2024-03-24 14:41:27.000000 mathutils_vinit-0.0.3/pyproject.toml
--rw-rw-r--   0 oem      (29999) oem      (29999)       38 2024-03-24 14:41:43.447893 mathutils_vinit-0.0.3/setup.cfg
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-03-24 14:41:43.443894 mathutils_vinit-0.0.3/src/
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-03-24 14:41:43.443894 mathutils_vinit-0.0.3/src/mathutils_vinit/
--rw-rw-r--   0 oem      (29999) oem      (29999)       24 2024-03-24 14:41:17.000000 mathutils_vinit-0.0.3/src/mathutils_vinit/__init__.py
--rw-rw-r--   0 oem      (29999) oem      (29999)      143 2024-03-24 13:30:14.000000 mathutils_vinit-0.0.3/src/mathutils_vinit/operations.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-03-24 14:41:43.447893 mathutils_vinit-0.0.3/src/mathutils_vinit.egg-info/
--rw-r--r--   0 oem      (29999) oem      (29999)      538 2024-03-24 14:41:43.000000 mathutils_vinit-0.0.3/src/mathutils_vinit.egg-info/PKG-INFO
--rw-rw-r--   0 oem      (29999) oem      (29999)      270 2024-03-24 14:41:43.000000 mathutils_vinit-0.0.3/src/mathutils_vinit.egg-info/SOURCES.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)        1 2024-03-24 14:41:43.000000 mathutils_vinit-0.0.3/src/mathutils_vinit.egg-info/dependency_links.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)       16 2024-03-24 14:41:43.000000 mathutils_vinit-0.0.3/src/mathutils_vinit.egg-info/top_level.txt
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 12:38:33.129616 mathutils_vinit-0.0.4/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     1073 2024-03-24 13:56:05.000000 mathutils_vinit-0.0.4/LICENSE
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      538 2024-04-05 12:38:33.129355 mathutils_vinit-0.0.4/PKG-INFO
+-rw-r--r--   0 vinitsarode   (501) staff       (20)       34 2024-03-24 13:55:43.000000 mathutils_vinit-0.0.4/README.md
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      485 2024-04-05 12:38:21.000000 mathutils_vinit-0.0.4/pyproject.toml
+-rw-r--r--   0 vinitsarode   (501) staff       (20)       38 2024-04-05 12:38:33.129667 mathutils_vinit-0.0.4/setup.cfg
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 12:38:33.126779 mathutils_vinit-0.0.4/src/
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 12:38:33.128159 mathutils_vinit-0.0.4/src/mathutils_vinit/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)       44 2024-04-05 12:32:10.000000 mathutils_vinit-0.0.4/src/mathutils_vinit/__init__.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      143 2024-03-24 13:30:14.000000 mathutils_vinit-0.0.4/src/mathutils_vinit/operations.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      133 2024-04-05 12:31:59.000000 mathutils_vinit-0.0.4/src/mathutils_vinit/roots.py
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 12:38:33.129111 mathutils_vinit-0.0.4/src/mathutils_vinit.egg-info/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      538 2024-04-05 12:38:33.000000 mathutils_vinit-0.0.4/src/mathutils_vinit.egg-info/PKG-INFO
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      299 2024-04-05 12:38:33.000000 mathutils_vinit-0.0.4/src/mathutils_vinit.egg-info/SOURCES.txt
+-rw-r--r--   0 vinitsarode   (501) staff       (20)        1 2024-04-05 12:38:33.000000 mathutils_vinit-0.0.4/src/mathutils_vinit.egg-info/dependency_links.txt
+-rw-r--r--   0 vinitsarode   (501) staff       (20)       16 2024-04-05 12:38:33.000000 mathutils_vinit-0.0.4/src/mathutils_vinit.egg-info/top_level.txt
```

### Comparing `mathutils_vinit-0.0.3/LICENSE` & `mathutils_vinit-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mathutils_vinit-0.0.3/PKG-INFO` & `mathutils_vinit-0.0.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathutils_vinit
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small example package
 Author-email: vinit sarode <vinitsarode5@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mathutils_vinit-0.0.3/src/mathutils_vinit.egg-info/PKG-INFO` & `mathutils_vinit-0.0.4/src/mathutils_vinit.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathutils_vinit
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small example package
 Author-email: vinit sarode <vinitsarode5@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

