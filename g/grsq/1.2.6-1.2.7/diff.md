# Comparing `tmp/grsq-1.2.6.tar.gz` & `tmp/grsq-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grsq-1.2.6.tar", last modified: Wed Mar 20 14:23:17 2024, max compression
+gzip compressed data, was "grsq-1.2.7.tar", last modified: Fri Apr  5 11:32:02 2024, max compression
```

## Comparing `grsq-1.2.6.tar` & `grsq-1.2.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 asod       (501) staff       (20)        0 2024-03-20 14:23:17.177961 grsq-1.2.6/
--rw-r--r--   0 asod       (501) staff       (20)     1075 2024-02-23 13:20:10.000000 grsq-1.2.6/LICENSE
--rw-r--r--   0 asod       (501) staff       (20)     8608 2024-03-20 14:23:17.177734 grsq-1.2.6/PKG-INFO
--rw-rw-r--   0 asod       (501) staff       (20)     6527 2023-10-21 13:06:09.000000 grsq-1.2.6/README.md
--rw-r--r--   0 asod       (501) staff       (20)      827 2024-03-20 14:22:36.000000 grsq-1.2.6/pyproject.toml
--rw-rw-r--   0 asod       (501) staff       (20)      675 2024-03-20 14:23:17.178362 grsq-1.2.6/setup.cfg
-drwxr-xr-x   0 asod       (501) staff       (20)        0 2024-03-20 14:23:17.171986 grsq-1.2.6/src/
-drwxr-xr-x   0 asod       (501) staff       (20)        0 2024-03-20 14:23:17.174090 grsq-1.2.6/src/grsq/
--rw-rw-r--   0 asod       (501) staff       (20)      163 2022-12-14 13:41:51.000000 grsq-1.2.6/src/grsq/__init__.py
--rw-r--r--   0 asod       (501) staff       (20)      938 2024-03-02 14:23:45.000000 grsq-1.2.6/src/grsq/accel.py
--rw-rw-r--   0 asod       (501) staff       (20)     3083 2024-03-20 14:21:40.000000 grsq-1.2.6/src/grsq/damping.py
--rw-r--r--   0 asod       (501) staff       (20)    11277 2024-03-15 12:40:26.000000 grsq-1.2.6/src/grsq/debye.py
--rw-r--r--   0 asod       (501) staff       (20)    23882 2024-03-15 12:41:50.000000 grsq-1.2.6/src/grsq/grsq.py
--rw-r--r--   0 asod       (501) staff       (20)     1263 2024-03-02 14:23:45.000000 grsq-1.2.6/src/grsq/histogramming.py
--rw-rw-r--   0 asod       (501) staff       (20)       61 2022-12-14 13:27:28.000000 grsq-1.2.6/src/grsq/py.typed
-drwxr-xr-x   0 asod       (501) staff       (20)        0 2024-03-20 14:23:17.177178 grsq-1.2.6/src/grsq.egg-info/
--rw-r--r--   0 asod       (501) staff       (20)     8608 2024-03-20 14:23:17.000000 grsq-1.2.6/src/grsq.egg-info/PKG-INFO
--rw-rw-r--   0 asod       (501) staff       (20)      409 2024-03-20 14:23:17.000000 grsq-1.2.6/src/grsq.egg-info/SOURCES.txt
--rw-rw-r--   0 asod       (501) staff       (20)        1 2024-03-20 14:23:17.000000 grsq-1.2.6/src/grsq.egg-info/dependency_links.txt
--rw-rw-r--   0 asod       (501) staff       (20)        1 2023-01-04 12:55:54.000000 grsq-1.2.6/src/grsq.egg-info/not-zip-safe
--rw-rw-r--   0 asod       (501) staff       (20)       84 2024-03-20 14:23:17.000000 grsq-1.2.6/src/grsq.egg-info/requires.txt
--rw-rw-r--   0 asod       (501) staff       (20)        5 2024-03-20 14:23:17.000000 grsq-1.2.6/src/grsq.egg-info/top_level.txt
-drwxr-xr-x   0 asod       (501) staff       (20)        0 2024-03-20 14:23:17.176924 grsq-1.2.6/tests/
--rw-r--r--   0 asod       (501) staff       (20)     3829 2024-03-13 10:19:28.000000 grsq-1.2.6/tests/test_debye.py
--rw-rw-r--   0 asod       (501) staff       (20)    10558 2024-03-15 12:53:07.000000 grsq-1.2.6/tests/test_grsq.py
+drwxrwxr-x   0 asod      (1000) asod      (1000)        0 2024-04-05 11:32:02.947856 grsq-1.2.7/
+-rw-rw-r--   0 asod      (1000) asod      (1000)     1075 2023-12-07 12:38:23.000000 grsq-1.2.7/LICENSE
+-rw-r--r--   0 asod      (1000) asod      (1000)     8608 2024-04-05 11:32:02.947856 grsq-1.2.7/PKG-INFO
+-rw-rw-r--   0 asod      (1000) asod      (1000)     6527 2023-10-21 13:06:09.000000 grsq-1.2.7/README.md
+-rw-rw-r--   0 asod      (1000) asod      (1000)      827 2024-04-05 11:30:41.000000 grsq-1.2.7/pyproject.toml
+-rw-rw-r--   0 asod      (1000) asod      (1000)      675 2024-04-05 11:32:02.947856 grsq-1.2.7/setup.cfg
+drwxrwxr-x   0 asod      (1000) asod      (1000)        0 2024-04-05 11:32:02.943856 grsq-1.2.7/src/
+drwxrwxr-x   0 asod      (1000) asod      (1000)        0 2024-04-05 11:32:02.947856 grsq-1.2.7/src/grsq/
+-rw-rw-r--   0 asod      (1000) asod      (1000)      163 2022-12-14 13:41:51.000000 grsq-1.2.7/src/grsq/__init__.py
+-rw-rw-r--   0 asod      (1000) asod      (1000)      938 2024-03-02 14:27:33.000000 grsq-1.2.7/src/grsq/accel.py
+-rw-rw-r--   0 asod      (1000) asod      (1000)     3083 2024-04-05 11:15:15.000000 grsq-1.2.7/src/grsq/damping.py
+-rw-rw-r--   0 asod      (1000) asod      (1000)    11277 2024-04-05 11:15:15.000000 grsq-1.2.7/src/grsq/debye.py
+-rw-rw-r--   0 asod      (1000) asod      (1000)    23856 2024-04-05 11:30:26.000000 grsq-1.2.7/src/grsq/grsq.py
+-rw-rw-r--   0 asod      (1000) asod      (1000)     1263 2024-03-02 14:27:33.000000 grsq-1.2.7/src/grsq/histogramming.py
+-rw-rw-r--   0 asod      (1000) asod      (1000)       61 2022-12-14 13:27:28.000000 grsq-1.2.7/src/grsq/py.typed
+drwxrwxr-x   0 asod      (1000) asod      (1000)        0 2024-04-05 11:32:02.947856 grsq-1.2.7/src/grsq.egg-info/
+-rw-r--r--   0 asod      (1000) asod      (1000)     8608 2024-04-05 11:32:02.000000 grsq-1.2.7/src/grsq.egg-info/PKG-INFO
+-rw-rw-r--   0 asod      (1000) asod      (1000)      409 2024-04-05 11:32:02.000000 grsq-1.2.7/src/grsq.egg-info/SOURCES.txt
+-rw-rw-r--   0 asod      (1000) asod      (1000)        1 2024-04-05 11:32:02.000000 grsq-1.2.7/src/grsq.egg-info/dependency_links.txt
+-rw-rw-r--   0 asod      (1000) asod      (1000)        1 2023-01-04 12:55:54.000000 grsq-1.2.7/src/grsq.egg-info/not-zip-safe
+-rw-rw-r--   0 asod      (1000) asod      (1000)       84 2024-04-05 11:32:02.000000 grsq-1.2.7/src/grsq.egg-info/requires.txt
+-rw-rw-r--   0 asod      (1000) asod      (1000)        5 2024-04-05 11:32:02.000000 grsq-1.2.7/src/grsq.egg-info/top_level.txt
+drwxrwxr-x   0 asod      (1000) asod      (1000)        0 2024-04-05 11:32:02.947856 grsq-1.2.7/tests/
+-rw-rw-r--   0 asod      (1000) asod      (1000)     3829 2024-04-05 11:15:15.000000 grsq-1.2.7/tests/test_debye.py
+-rw-rw-r--   0 asod      (1000) asod      (1000)    10558 2024-04-05 11:15:15.000000 grsq-1.2.7/tests/test_grsq.py
```

### Comparing `grsq-1.2.6/LICENSE` & `grsq-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `grsq-1.2.6/PKG-INFO` & `grsq-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grsq
-Version: 1.2.6
+Version: 1.2.7
 Summary: Structure factor and X-ray scattering from radial distribution functions
 Home-page: https://gitlab.com/asod/grsq
 Author: Asmus Ougaard Dohn
 Author-email: Asmus Ougaard Dohn <asmus.od@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Asmus Ougaard Dohn
```

### Comparing `grsq-1.2.6/README.md` & `grsq-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `grsq-1.2.6/pyproject.toml` & `grsq-1.2.7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "grsq"
-version = "1.2.6"
+version = "1.2.7"
 authors = [
   { name="Asmus Ougaard Dohn", email="asmus.od@gmail.com" },
 ]
 description = "Structure factor and X-ray scattering from radial distribution functions"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `grsq-1.2.6/setup.cfg` & `grsq-1.2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `grsq-1.2.6/src/grsq/accel.py` & `grsq-1.2.7/src/grsq/accel.py`

 * *Files identical despite different names*

### Comparing `grsq-1.2.6/src/grsq/damping.py` & `grsq-1.2.7/src/grsq/damping.py`

 * *Files identical despite different names*

### Comparing `grsq-1.2.6/src/grsq/debye.py` & `grsq-1.2.7/src/grsq/debye.py`

 * *Files identical despite different names*

### Comparing `grsq-1.2.6/src/grsq/grsq.py` & `grsq-1.2.7/src/grsq/grsq.py`

 * *Files 1% similar despite different names*

```diff
@@ -571,16 +571,16 @@
 ''' Helper Functions'''
 def rdfset_from_dir(dirname, prmtop=None, volume=None, stoich=None):
     ''' Read in a directory of rdf files with the naming convention:
             gEl1_w1-El2_w2.dat
         where:
             | El1: Element name 1 (also used for the IAM)
             | El2: Element name 2 (also used for the IAM)
-            | w1:  Region of element 1 (u, c, v) (i.e. solute, cross, solvent)
-            | w2:  Region of element 2 (u, c, v)
+            | w1:  Region of element 1 (u, v) (i.e. solUte, solVent)
+            | w2:  Region of element 2 (u, v)
 
             So e.g. water would have the RDFs: gO_v-O_v.dat, gO_v-H_v.dat, etc..
 
         prmtop (str): path to structure file for a single frame:
             | The method can read the stoichometry from either a prmtop or an xyzfile.
             | If an xyz file is used, you need to specify the volume in which the RDFs
             | where sampled manually.
@@ -594,15 +594,15 @@
         '''
     import MDAnalysis as mda
     import glob
 
     rdf_files = sorted(glob.glob(dirname + os.sep + '*dat'))
     assert len(rdf_files) > 0, f'Found no .dat files in {dirname + os.sep} '
 
-    whered = {'u':'solute', 'v':'solvent', 'c':'cross'}
+    whered = {'u':'solute', 'v':'solvent'}
     if prmtop is not None:
         # Load universe to get stoichometry.
         u = mda.Universe(prmtop)
 
     if volume is None:
         # Unfortunately mda cannot get the box size from the prmtop, even though it is there
         with open(prmtop, 'r') as f:
```

### Comparing `grsq-1.2.6/src/grsq/histogramming.py` & `grsq-1.2.7/src/grsq/histogramming.py`

 * *Files identical despite different names*

### Comparing `grsq-1.2.6/src/grsq.egg-info/PKG-INFO` & `grsq-1.2.7/src/grsq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grsq
-Version: 1.2.6
+Version: 1.2.7
 Summary: Structure factor and X-ray scattering from radial distribution functions
 Home-page: https://gitlab.com/asod/grsq
 Author: Asmus Ougaard Dohn
 Author-email: Asmus Ougaard Dohn <asmus.od@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Asmus Ougaard Dohn
```

### Comparing `grsq-1.2.6/tests/test_debye.py` & `grsq-1.2.7/tests/test_debye.py`

 * *Files identical despite different names*

### Comparing `grsq-1.2.6/tests/test_grsq.py` & `grsq-1.2.7/tests/test_grsq.py`

 * *Files identical despite different names*

