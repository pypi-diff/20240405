# Comparing `tmp/PredictBind-1.0.0a0.tar.gz` & `tmp/PredictBind-1.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PredictBind-1.0.0a0.tar", last modified: Fri Apr  5 19:23:07 2024, max compression
+gzip compressed data, was "PredictBind-1.0.0b0.tar", last modified: Fri Apr  5 19:31:36 2024, max compression
```

## Comparing `PredictBind-1.0.0a0.tar` & `PredictBind-1.0.0b0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 tamaraveres   (501) staff       (20)        0 2024-04-05 19:23:07.529814 PredictBind-1.0.0a0/
--rw-r--r--   0 tamaraveres   (501) staff       (20)     1115 2024-04-03 21:38:46.000000 PredictBind-1.0.0a0/LICENSE
--rw-r--r--   0 tamaraveres   (501) staff       (20)     8138 2024-04-05 19:23:07.529585 PredictBind-1.0.0a0/PKG-INFO
-drwxr-xr-x   0 tamaraveres   (501) staff       (20)        0 2024-04-05 19:23:07.528039 PredictBind-1.0.0a0/PredictBind/
--rw-r--r--   0 tamaraveres   (501) staff       (20)     3335 2024-04-05 19:16:47.000000 PredictBind-1.0.0a0/PredictBind/Cli.py
--rw-r--r--   0 tamaraveres   (501) staff       (20)     1886 2024-04-03 20:14:28.000000 PredictBind-1.0.0a0/PredictBind/Files.py
--rwxr-xr-x   0 tamaraveres   (501) staff       (20)     2281 2024-04-05 19:16:45.000000 PredictBind-1.0.0a0/PredictBind/Main.py
--rw-r--r--   0 tamaraveres   (501) staff       (20)     4575 2024-04-03 20:20:35.000000 PredictBind-1.0.0a0/PredictBind/P2Pocket.py
--rw-r--r--   0 tamaraveres   (501) staff       (20)     2574 2024-04-03 20:58:58.000000 PredictBind-1.0.0a0/PredictBind/P2Rank.py
--rw-r--r--   0 tamaraveres   (501) staff       (20)     1331 2024-04-03 20:47:40.000000 PredictBind-1.0.0a0/PredictBind/TSV.py
--rw-r--r--   0 tamaraveres   (501) staff       (20)     2856 2024-04-05 19:16:41.000000 PredictBind-1.0.0a0/PredictBind/Utils.py
-drwxr-xr-x   0 tamaraveres   (501) staff       (20)        0 2024-04-05 19:23:07.529292 PredictBind-1.0.0a0/PredictBind.egg-info/
--rw-r--r--   0 tamaraveres   (501) staff       (20)     8138 2024-04-05 19:23:07.000000 PredictBind-1.0.0a0/PredictBind.egg-info/PKG-INFO
--rw-r--r--   0 tamaraveres   (501) staff       (20)      384 2024-04-05 19:23:07.000000 PredictBind-1.0.0a0/PredictBind.egg-info/SOURCES.txt
--rw-r--r--   0 tamaraveres   (501) staff       (20)        1 2024-04-05 19:23:07.000000 PredictBind-1.0.0a0/PredictBind.egg-info/dependency_links.txt
--rw-r--r--   0 tamaraveres   (501) staff       (20)       53 2024-04-05 19:23:07.000000 PredictBind-1.0.0a0/PredictBind.egg-info/entry_points.txt
--rw-r--r--   0 tamaraveres   (501) staff       (20)        9 2024-04-05 19:23:07.000000 PredictBind-1.0.0a0/PredictBind.egg-info/requires.txt
--rw-r--r--   0 tamaraveres   (501) staff       (20)       12 2024-04-05 19:23:07.000000 PredictBind-1.0.0a0/PredictBind.egg-info/top_level.txt
--rw-r--r--   0 tamaraveres   (501) staff       (20)     7627 2024-04-03 21:45:21.000000 PredictBind-1.0.0a0/README.md
--rw-r--r--   0 tamaraveres   (501) staff       (20)       38 2024-04-05 19:23:07.529862 PredictBind-1.0.0a0/setup.cfg
--rw-r--r--   0 tamaraveres   (501) staff       (20)      903 2024-04-05 19:22:37.000000 PredictBind-1.0.0a0/setup.py
+drwxr-xr-x   0 tamaraveres   (501) staff       (20)        0 2024-04-05 19:31:36.969476 PredictBind-1.0.0b0/
+-rw-r--r--   0 tamaraveres   (501) staff       (20)     1115 2024-04-03 21:38:46.000000 PredictBind-1.0.0b0/LICENSE
+-rw-r--r--   0 tamaraveres   (501) staff       (20)     8138 2024-04-05 19:31:36.969214 PredictBind-1.0.0b0/PKG-INFO
+drwxr-xr-x   0 tamaraveres   (501) staff       (20)        0 2024-04-05 19:31:36.967370 PredictBind-1.0.0b0/PredictBind/
+-rw-r--r--   0 tamaraveres   (501) staff       (20)     3335 2024-04-05 19:16:47.000000 PredictBind-1.0.0b0/PredictBind/Cli.py
+-rw-r--r--   0 tamaraveres   (501) staff       (20)     1886 2024-04-03 20:14:28.000000 PredictBind-1.0.0b0/PredictBind/Files.py
+-rwxr-xr-x   0 tamaraveres   (501) staff       (20)     2281 2024-04-05 19:16:45.000000 PredictBind-1.0.0b0/PredictBind/Main.py
+-rw-r--r--   0 tamaraveres   (501) staff       (20)     4575 2024-04-03 20:20:35.000000 PredictBind-1.0.0b0/PredictBind/P2Pocket.py
+-rw-r--r--   0 tamaraveres   (501) staff       (20)     2574 2024-04-03 20:58:58.000000 PredictBind-1.0.0b0/PredictBind/P2Rank.py
+-rw-r--r--   0 tamaraveres   (501) staff       (20)     1331 2024-04-03 20:47:40.000000 PredictBind-1.0.0b0/PredictBind/TSV.py
+-rw-r--r--   0 tamaraveres   (501) staff       (20)     2856 2024-04-05 19:16:41.000000 PredictBind-1.0.0b0/PredictBind/Utils.py
+drwxr-xr-x   0 tamaraveres   (501) staff       (20)        0 2024-04-05 19:31:36.968701 PredictBind-1.0.0b0/PredictBind/training_data/
+-rwxr-xr-x   0 tamaraveres   (501) staff       (20)     5037 2024-04-03 18:03:52.000000 PredictBind-1.0.0b0/PredictBind/training_data/prank
+-rw-r--r--   0 tamaraveres   (501) staff       (20)      534 2024-04-03 18:03:52.000000 PredictBind-1.0.0b0/PredictBind/training_data/prank.bat
+drwxr-xr-x   0 tamaraveres   (501) staff       (20)        0 2024-04-05 19:31:36.968905 PredictBind-1.0.0b0/PredictBind.egg-info/
+-rw-r--r--   0 tamaraveres   (501) staff       (20)     8138 2024-04-05 19:31:36.000000 PredictBind-1.0.0b0/PredictBind.egg-info/PKG-INFO
+-rw-r--r--   0 tamaraveres   (501) staff       (20)      452 2024-04-05 19:31:36.000000 PredictBind-1.0.0b0/PredictBind.egg-info/SOURCES.txt
+-rw-r--r--   0 tamaraveres   (501) staff       (20)        1 2024-04-05 19:31:36.000000 PredictBind-1.0.0b0/PredictBind.egg-info/dependency_links.txt
+-rw-r--r--   0 tamaraveres   (501) staff       (20)       53 2024-04-05 19:31:36.000000 PredictBind-1.0.0b0/PredictBind.egg-info/entry_points.txt
+-rw-r--r--   0 tamaraveres   (501) staff       (20)        9 2024-04-05 19:31:36.000000 PredictBind-1.0.0b0/PredictBind.egg-info/requires.txt
+-rw-r--r--   0 tamaraveres   (501) staff       (20)       12 2024-04-05 19:31:36.000000 PredictBind-1.0.0b0/PredictBind.egg-info/top_level.txt
+-rw-r--r--   0 tamaraveres   (501) staff       (20)     7627 2024-04-03 21:45:21.000000 PredictBind-1.0.0b0/README.md
+-rw-r--r--   0 tamaraveres   (501) staff       (20)       38 2024-04-05 19:31:36.969531 PredictBind-1.0.0b0/setup.cfg
+-rw-r--r--   0 tamaraveres   (501) staff       (20)      907 2024-04-05 19:31:26.000000 PredictBind-1.0.0b0/setup.py
```

### Comparing `PredictBind-1.0.0a0/LICENSE` & `PredictBind-1.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `PredictBind-1.0.0a0/PKG-INFO` & `PredictBind-1.0.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PredictBind
-Version: 1.0.0a0
+Version: 1.0.0b0
 Summary: PredictBind is a wrapped inspired and built around P2Rank as ligand binding site predictor for proteins
 Home-page: https://github.com/TamaraVeres/binder
 Author: Tamara Veres
 Author-email: tamaraveres19@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PredictBind-1.0.0a0/PredictBind/Cli.py` & `PredictBind-1.0.0b0/PredictBind/Cli.py`

 * *Files identical despite different names*

### Comparing `PredictBind-1.0.0a0/PredictBind/Files.py` & `PredictBind-1.0.0b0/PredictBind/Files.py`

 * *Files identical despite different names*

### Comparing `PredictBind-1.0.0a0/PredictBind/Main.py` & `PredictBind-1.0.0b0/PredictBind/Main.py`

 * *Files identical despite different names*

### Comparing `PredictBind-1.0.0a0/PredictBind/P2Pocket.py` & `PredictBind-1.0.0b0/PredictBind/P2Pocket.py`

 * *Files identical despite different names*

### Comparing `PredictBind-1.0.0a0/PredictBind/P2Rank.py` & `PredictBind-1.0.0b0/PredictBind/P2Rank.py`

 * *Files identical despite different names*

### Comparing `PredictBind-1.0.0a0/PredictBind/TSV.py` & `PredictBind-1.0.0b0/PredictBind/TSV.py`

 * *Files identical despite different names*

### Comparing `PredictBind-1.0.0a0/PredictBind/Utils.py` & `PredictBind-1.0.0b0/PredictBind/Utils.py`

 * *Files identical despite different names*

### Comparing `PredictBind-1.0.0a0/PredictBind.egg-info/PKG-INFO` & `PredictBind-1.0.0b0/PredictBind.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PredictBind
-Version: 1.0.0a0
+Version: 1.0.0b0
 Summary: PredictBind is a wrapped inspired and built around P2Rank as ligand binding site predictor for proteins
 Home-page: https://github.com/TamaraVeres/binder
 Author: Tamara Veres
 Author-email: tamaraveres19@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PredictBind-1.0.0a0/README.md` & `PredictBind-1.0.0b0/README.md`

 * *Files identical despite different names*

### Comparing `PredictBind-1.0.0a0/setup.py` & `PredictBind-1.0.0b0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 with open("README.md", "r") as fh: 
     long_description = fh.read() 
 
 setuptools.setup(
     name='PredictBind',
-    version='1.0.0-alpha',
+    version='1.0.0-beta',
     packages=['PredictBind'],
-    package_data={'PredictBind': ['p2rank.jar']},
+    package_data={'PredictBind': ['training_data/*']},
     install_requires=['requests'],
     author='Tamara Veres',
     author_email='tamaraveres19@gmail.com',
     description='PredictBind is a wrapped inspired and built around P2Rank as ligand binding site predictor for proteins',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/TamaraVeres/binder',
```

