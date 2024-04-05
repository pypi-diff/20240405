# Comparing `tmp/CellPatchExtraction-1.8.tar.gz` & `tmp/CellPatchExtraction-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CellPatchExtraction-1.8.tar", last modified: Wed Jan 10 15:53:20 2024, max compression
+gzip compressed data, was "CellPatchExtraction-1.9.tar", last modified: Wed Jan 10 15:54:49 2024, max compression
```

## Comparing `CellPatchExtraction-1.8.tar` & `CellPatchExtraction-1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:53:20.297229 CellPatchExtraction-1.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:53:20.293229 CellPatchExtraction-1.8/CellPatchExtraction/
--rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-01-10 15:53:16.000000 CellPatchExtraction-1.8/CellPatchExtraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:53:20.297229 CellPatchExtraction-1.8/CellPatchExtraction/src/
--rwxr-xr-x   0 runner    (1001) docker     (127)      209 2024-01-10 15:53:16.000000 CellPatchExtraction-1.8/CellPatchExtraction/src/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10454 2024-01-10 15:53:16.000000 CellPatchExtraction-1.8/CellPatchExtraction/src/extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-01-10 15:53:16.000000 CellPatchExtraction-1.8/CellPatchExtraction/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:53:20.293229 CellPatchExtraction-1.8/CellPatchExtraction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-01-10 15:53:20.000000 CellPatchExtraction-1.8/CellPatchExtraction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-01-10 15:53:20.000000 CellPatchExtraction-1.8/CellPatchExtraction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 15:53:20.000000 CellPatchExtraction-1.8/CellPatchExtraction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-01-10 15:53:20.000000 CellPatchExtraction-1.8/CellPatchExtraction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-10 15:53:20.000000 CellPatchExtraction-1.8/CellPatchExtraction.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-01-10 15:53:20.297229 CellPatchExtraction-1.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2037 2024-01-10 15:53:16.000000 CellPatchExtraction-1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-10 15:53:20.297229 CellPatchExtraction-1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-01-10 15:53:19.000000 CellPatchExtraction-1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:54:49.587681 CellPatchExtraction-1.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:54:49.587681 CellPatchExtraction-1.9/CellPatchExtraction/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-01-10 15:54:46.000000 CellPatchExtraction-1.9/CellPatchExtraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:54:49.587681 CellPatchExtraction-1.9/CellPatchExtraction/src/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      209 2024-01-10 15:54:46.000000 CellPatchExtraction-1.9/CellPatchExtraction/src/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10454 2024-01-10 15:54:46.000000 CellPatchExtraction-1.9/CellPatchExtraction/src/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-01-10 15:54:46.000000 CellPatchExtraction-1.9/CellPatchExtraction/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:54:49.587681 CellPatchExtraction-1.9/CellPatchExtraction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-01-10 15:54:49.000000 CellPatchExtraction-1.9/CellPatchExtraction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-01-10 15:54:49.000000 CellPatchExtraction-1.9/CellPatchExtraction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 15:54:49.000000 CellPatchExtraction-1.9/CellPatchExtraction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-01-10 15:54:49.000000 CellPatchExtraction-1.9/CellPatchExtraction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-10 15:54:49.000000 CellPatchExtraction-1.9/CellPatchExtraction.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-01-10 15:54:49.587681 CellPatchExtraction-1.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2037 2024-01-10 15:54:46.000000 CellPatchExtraction-1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-10 15:54:49.587681 CellPatchExtraction-1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-01-10 15:54:48.000000 CellPatchExtraction-1.9/setup.py
```

### Comparing `CellPatchExtraction-1.8/CellPatchExtraction/src/extraction.py` & `CellPatchExtraction-1.9/CellPatchExtraction/src/extraction.py`

 * *Files identical despite different names*

### Comparing `CellPatchExtraction-1.8/CellPatchExtraction/src/utils.py` & `CellPatchExtraction-1.9/CellPatchExtraction/src/utils.py`

 * *Files identical despite different names*

### Comparing `CellPatchExtraction-1.8/CellPatchExtraction.egg-info/PKG-INFO` & `CellPatchExtraction-1.9/CellPatchExtraction.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CellPatchExtraction
-Version: 1.8
+Version: 1.9
 Home-page: https://github.com/SimonBon/CellPatchExtraction
 Author: Simon Gutwein
 Author-email: simon.gutwein@ccri.at
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CellPatchExtraction-1.8/PKG-INFO` & `CellPatchExtraction-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CellPatchExtraction
-Version: 1.8
+Version: 1.9
 Home-page: https://github.com/SimonBon/CellPatchExtraction
 Author: Simon Gutwein
 Author-email: simon.gutwein@ccri.at
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CellPatchExtraction-1.8/README.md` & `CellPatchExtraction-1.9/README.md`

 * *Files identical despite different names*

### Comparing `CellPatchExtraction-1.8/setup.py` & `CellPatchExtraction-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def read_requirements():
     with open('requirements.txt', 'r') as file:
         return [line.strip() for line in file.readlines()]
 
 setup(
     name=package_name,
-    version='1.8',
+    version='1.9',
     packages=find_packages(),
     install_requires=read_requirements(),
     author="Simon Gutwein",
     include_package_data=True,
     author_email="simon.gutwein@ccri.at",
     description="",
     long_description=open('README.md').read(),
```

