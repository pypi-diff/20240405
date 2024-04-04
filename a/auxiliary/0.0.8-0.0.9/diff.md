# Comparing `tmp/auxiliary-0.0.8.tar.gz` & `tmp/auxiliary-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auxiliary-0.0.8.tar", last modified: Tue Aug 29 13:20:55 2023, max compression
+gzip compressed data, was "auxiliary-0.0.9.tar", last modified: Tue Aug 29 13:30:17 2023, max compression
```

## Comparing `auxiliary-0.0.8.tar` & `auxiliary-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 florian   (1001) florian   (1001)        0 2023-08-29 13:20:55.402691 auxiliary-0.0.8/
--rw-rw-r--   0 florian   (1001) florian   (1001)    34523 2023-08-29 12:48:17.000000 auxiliary-0.0.8/LICENSE
--rw-rw-r--   0 florian   (1001) florian   (1001)      693 2023-08-29 13:20:55.398691 auxiliary-0.0.8/PKG-INFO
--rw-rw-r--   0 florian   (1001) florian   (1001)      112 2023-08-29 12:48:17.000000 auxiliary-0.0.8/README.md
-drwxrwxr-x   0 florian   (1001) florian   (1001)        0 2023-08-29 13:20:55.398691 auxiliary-0.0.8/auxiliary/
--rw-rw-r--   0 florian   (1001) florian   (1001)      125 2023-08-29 12:48:17.000000 auxiliary-0.0.8/auxiliary/__init__.py
--rw-rw-r--   0 florian   (1001) florian   (1001)      379 2023-08-29 12:48:17.000000 auxiliary-0.0.8/auxiliary/nifti.py
--rw-rw-r--   0 florian   (1001) florian   (1001)      810 2023-08-29 12:48:17.000000 auxiliary-0.0.8/auxiliary/path.py
--rw-rw-r--   0 florian   (1001) florian   (1001)     4614 2023-08-29 12:48:17.000000 auxiliary-0.0.8/auxiliary/runscript.py
-drwxrwxr-x   0 florian   (1001) florian   (1001)        0 2023-08-29 13:20:55.398691 auxiliary-0.0.8/auxiliary.egg-info/
--rw-rw-r--   0 florian   (1001) florian   (1001)      693 2023-08-29 13:20:55.000000 auxiliary-0.0.8/auxiliary.egg-info/PKG-INFO
--rw-rw-r--   0 florian   (1001) florian   (1001)      278 2023-08-29 13:20:55.000000 auxiliary-0.0.8/auxiliary.egg-info/SOURCES.txt
--rw-rw-r--   0 florian   (1001) florian   (1001)        1 2023-08-29 13:20:55.000000 auxiliary-0.0.8/auxiliary.egg-info/dependency_links.txt
--rw-rw-r--   0 florian   (1001) florian   (1001)       56 2023-08-29 13:20:55.000000 auxiliary-0.0.8/auxiliary.egg-info/requires.txt
--rw-rw-r--   0 florian   (1001) florian   (1001)       10 2023-08-29 13:20:55.000000 auxiliary-0.0.8/auxiliary.egg-info/top_level.txt
--rw-rw-r--   0 florian   (1001) florian   (1001)     1033 2023-08-29 13:20:50.000000 auxiliary-0.0.8/pyproject.toml
--rw-rw-r--   0 florian   (1001) florian   (1001)       38 2023-08-29 13:20:55.402691 auxiliary-0.0.8/setup.cfg
+drwxrwxr-x   0 florian   (1001) florian   (1001)        0 2023-08-29 13:30:17.988105 auxiliary-0.0.9/
+-rw-rw-r--   0 florian   (1001) florian   (1001)    34523 2023-08-29 12:48:17.000000 auxiliary-0.0.9/LICENSE
+-rw-rw-r--   0 florian   (1001) florian   (1001)      693 2023-08-29 13:30:17.988105 auxiliary-0.0.9/PKG-INFO
+-rw-rw-r--   0 florian   (1001) florian   (1001)      112 2023-08-29 12:48:17.000000 auxiliary-0.0.9/README.md
+drwxrwxr-x   0 florian   (1001) florian   (1001)        0 2023-08-29 13:30:17.988105 auxiliary-0.0.9/auxiliary/
+-rw-rw-r--   0 florian   (1001) florian   (1001)      304 2023-08-29 13:28:59.000000 auxiliary-0.0.9/auxiliary/__init__.py
+-rw-rw-r--   0 florian   (1001) florian   (1001)      379 2023-08-29 12:48:17.000000 auxiliary-0.0.9/auxiliary/nifti.py
+-rw-rw-r--   0 florian   (1001) florian   (1001)      810 2023-08-29 12:48:17.000000 auxiliary-0.0.9/auxiliary/path.py
+-rw-rw-r--   0 florian   (1001) florian   (1001)     4614 2023-08-29 12:48:17.000000 auxiliary-0.0.9/auxiliary/runscript.py
+drwxrwxr-x   0 florian   (1001) florian   (1001)        0 2023-08-29 13:30:17.988105 auxiliary-0.0.9/auxiliary.egg-info/
+-rw-rw-r--   0 florian   (1001) florian   (1001)      693 2023-08-29 13:30:17.000000 auxiliary-0.0.9/auxiliary.egg-info/PKG-INFO
+-rw-rw-r--   0 florian   (1001) florian   (1001)      278 2023-08-29 13:30:17.000000 auxiliary-0.0.9/auxiliary.egg-info/SOURCES.txt
+-rw-rw-r--   0 florian   (1001) florian   (1001)        1 2023-08-29 13:30:17.000000 auxiliary-0.0.9/auxiliary.egg-info/dependency_links.txt
+-rw-rw-r--   0 florian   (1001) florian   (1001)       56 2023-08-29 13:30:17.000000 auxiliary-0.0.9/auxiliary.egg-info/requires.txt
+-rw-rw-r--   0 florian   (1001) florian   (1001)       10 2023-08-29 13:30:17.000000 auxiliary-0.0.9/auxiliary.egg-info/top_level.txt
+-rw-rw-r--   0 florian   (1001) florian   (1001)     1033 2023-08-29 13:29:47.000000 auxiliary-0.0.9/pyproject.toml
+-rw-rw-r--   0 florian   (1001) florian   (1001)       38 2023-08-29 13:30:17.988105 auxiliary-0.0.9/setup.cfg
```

### Comparing `auxiliary-0.0.8/LICENSE` & `auxiliary-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `auxiliary-0.0.8/PKG-INFO` & `auxiliary-0.0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auxiliary
-Version: 0.0.8
+Version: 0.0.9
 Summary: TODO.
 Author-email: Florian Kofler <florian.kofler@tum.de>
 Maintainer-email: Florian Kofler <florian.kofler@tum.de>
 Project-URL: repository, https://github.com/BrainLesion/auxiliary
 Keywords: biomedical image analysis,utils,helpers,auxiliary
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `auxiliary-0.0.8/auxiliary/path.py` & `auxiliary-0.0.9/auxiliary/path.py`

 * *Files identical despite different names*

### Comparing `auxiliary-0.0.8/auxiliary/runscript.py` & `auxiliary-0.0.9/auxiliary/runscript.py`

 * *Files identical despite different names*

### Comparing `auxiliary-0.0.8/auxiliary.egg-info/PKG-INFO` & `auxiliary-0.0.9/auxiliary.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auxiliary
-Version: 0.0.8
+Version: 0.0.9
 Summary: TODO.
 Author-email: Florian Kofler <florian.kofler@tum.de>
 Maintainer-email: Florian Kofler <florian.kofler@tum.de>
 Project-URL: repository, https://github.com/BrainLesion/auxiliary
 Keywords: biomedical image analysis,utils,helpers,auxiliary
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `auxiliary-0.0.8/pyproject.toml` & `auxiliary-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [tool.setuptools_scm]
 write_to = "version.py"
 
 [project]
 name = "auxiliary"
 requires-python = ">=3.5"
 # dynamic = ["version"]
-version = "0.0.8"
+version = "0.0.9"
 authors = [{ name = "Florian Kofler", email = "florian.kofler@tum.de" }]
 maintainers = [{ name = "Florian Kofler", email = "florian.kofler@tum.de" }]
 description = "TODO."
 keywords = ["biomedical image analysis", "utils", "helpers", "auxiliary"]
 readme = "README.md"
 # requires-python = "==3.10"
 classifiers = [
```

