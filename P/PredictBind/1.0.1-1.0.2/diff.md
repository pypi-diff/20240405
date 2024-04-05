# Comparing `tmp/PredictBind-1.0.1.tar.gz` & `tmp/PredictBind-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PredictBind-1.0.1.tar", last modified: Wed Apr  3 21:47:51 2024, max compression
+gzip compressed data, was "PredictBind-1.0.2.tar", last modified: Fri Apr  5 18:47:46 2024, max compression
```

## Comparing `PredictBind-1.0.1.tar` & `PredictBind-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 tamaraveres   (501) staff       (20)        0 2024-04-03 21:47:51.637896 PredictBind-1.0.1/
--rw-r--r--   0 tamaraveres   (501) staff       (20)     1115 2024-04-03 21:38:46.000000 PredictBind-1.0.1/LICENSE
--rw-r--r--   0 tamaraveres   (501) staff       (20)     8136 2024-04-03 21:47:51.637552 PredictBind-1.0.1/PKG-INFO
-drwxr-xr-x   0 tamaraveres   (501) staff       (20)        0 2024-04-03 21:47:51.637172 PredictBind-1.0.1/PredictBind.egg-info/
--rw-r--r--   0 tamaraveres   (501) staff       (20)     8136 2024-04-03 21:47:51.000000 PredictBind-1.0.1/PredictBind.egg-info/PKG-INFO
--rw-r--r--   0 tamaraveres   (501) staff       (20)      200 2024-04-03 21:47:51.000000 PredictBind-1.0.1/PredictBind.egg-info/SOURCES.txt
--rw-r--r--   0 tamaraveres   (501) staff       (20)        1 2024-04-03 21:47:51.000000 PredictBind-1.0.1/PredictBind.egg-info/dependency_links.txt
--rw-r--r--   0 tamaraveres   (501) staff       (20)        9 2024-04-03 21:47:51.000000 PredictBind-1.0.1/PredictBind.egg-info/requires.txt
--rw-r--r--   0 tamaraveres   (501) staff       (20)        1 2024-04-03 21:47:51.000000 PredictBind-1.0.1/PredictBind.egg-info/top_level.txt
--rw-r--r--   0 tamaraveres   (501) staff       (20)     7627 2024-04-03 21:45:21.000000 PredictBind-1.0.1/README.md
--rw-r--r--   0 tamaraveres   (501) staff       (20)       38 2024-04-03 21:47:51.637962 PredictBind-1.0.1/setup.cfg
--rw-r--r--   0 tamaraveres   (501) staff       (20)      794 2024-04-03 21:46:41.000000 PredictBind-1.0.1/setup.py
+drwxr-xr-x   0 tamaraveres   (501) staff       (20)        0 2024-04-05 18:47:46.150082 PredictBind-1.0.2/
+-rw-r--r--   0 tamaraveres   (501) staff       (20)     1115 2024-04-03 21:38:46.000000 PredictBind-1.0.2/LICENSE
+-rw-r--r--   0 tamaraveres   (501) staff       (20)     8136 2024-04-05 18:47:46.149842 PredictBind-1.0.2/PKG-INFO
+drwxr-xr-x   0 tamaraveres   (501) staff       (20)        0 2024-04-05 18:47:46.149613 PredictBind-1.0.2/PredictBind.egg-info/
+-rw-r--r--   0 tamaraveres   (501) staff       (20)     8136 2024-04-05 18:47:46.000000 PredictBind-1.0.2/PredictBind.egg-info/PKG-INFO
+-rw-r--r--   0 tamaraveres   (501) staff       (20)      238 2024-04-05 18:47:46.000000 PredictBind-1.0.2/PredictBind.egg-info/SOURCES.txt
+-rw-r--r--   0 tamaraveres   (501) staff       (20)        1 2024-04-05 18:47:46.000000 PredictBind-1.0.2/PredictBind.egg-info/dependency_links.txt
+-rw-r--r--   0 tamaraveres   (501) staff       (20)       53 2024-04-05 18:47:46.000000 PredictBind-1.0.2/PredictBind.egg-info/entry_points.txt
+-rw-r--r--   0 tamaraveres   (501) staff       (20)        9 2024-04-05 18:47:46.000000 PredictBind-1.0.2/PredictBind.egg-info/requires.txt
+-rw-r--r--   0 tamaraveres   (501) staff       (20)        1 2024-04-05 18:47:46.000000 PredictBind-1.0.2/PredictBind.egg-info/top_level.txt
+-rw-r--r--   0 tamaraveres   (501) staff       (20)     7627 2024-04-03 21:45:21.000000 PredictBind-1.0.2/README.md
+-rw-r--r--   0 tamaraveres   (501) staff       (20)       38 2024-04-05 18:47:46.150133 PredictBind-1.0.2/setup.cfg
+-rw-r--r--   0 tamaraveres   (501) staff       (20)      908 2024-04-05 18:47:31.000000 PredictBind-1.0.2/setup.py
```

### Comparing `PredictBind-1.0.1/LICENSE` & `PredictBind-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PredictBind-1.0.1/PKG-INFO` & `PredictBind-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PredictBind
-Version: 1.0.1
+Version: 1.0.2
 Summary: PredictBind is a wrapped inspired and built around P2Rank as ligand binding site predictor for proteins
 Home-page: https://github.com/TamaraVeres/binder
 Author: Tamara Veres
 Author-email: tamaraveres19@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PredictBind-1.0.1/PredictBind.egg-info/PKG-INFO` & `PredictBind-1.0.2/PredictBind.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PredictBind
-Version: 1.0.1
+Version: 1.0.2
 Summary: PredictBind is a wrapped inspired and built around P2Rank as ligand binding site predictor for proteins
 Home-page: https://github.com/TamaraVeres/binder
 Author: Tamara Veres
 Author-email: tamaraveres19@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PredictBind-1.0.1/README.md` & `PredictBind-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `PredictBind-1.0.1/setup.py` & `PredictBind-1.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh: 
     long_description = fh.read() 
 
 setuptools.setup(
     name='PredictBind',
-    version='1.0.1',
+    version='1.0.2',
     packages=setuptools.find_packages(),
     package_data={'PredictBind': ['p2rank.jar']},
     install_requires=['requests'],
     author='Tamara Veres',
     author_email='tamaraveres19@gmail.com',
     description='PredictBind is a wrapped inspired and built around P2Rank as ligand binding site predictor for proteins',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/TamaraVeres/binder',
     classifiers=[ 
         "Programming Language :: Python :: 3", 
         "License :: OSI Approved :: MIT License", 
         "Operating System :: OS Independent", 
     ], 
+    entry_points={
+        'console_scripts': [
+            'PredictBind=PredictBind.Main:cli',
+        ],
+    },
 )
```

