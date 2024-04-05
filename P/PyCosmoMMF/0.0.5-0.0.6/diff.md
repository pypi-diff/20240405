# Comparing `tmp/PyCosmoMMF-0.0.5.tar.gz` & `tmp/PyCosmoMMF-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCosmoMMF-0.0.5.tar", last modified: Sat Mar 23 18:29:26 2024, max compression
+gzip compressed data, was "PyCosmoMMF-0.0.6.tar", last modified: Fri Apr  5 21:12:50 2024, max compression
```

## Comparing `PyCosmoMMF-0.0.5.tar` & `PyCosmoMMF-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jamessunseri   (501) staff       (20)        0 2024-03-23 18:29:26.552271 PyCosmoMMF-0.0.5/
--rw-r--r--   0 jamessunseri   (501) staff       (20)     1070 2024-03-12 07:03:50.000000 PyCosmoMMF-0.0.5/LICENSE
--rw-r--r--   0 jamessunseri   (501) staff       (20)      109 2024-03-12 22:35:52.000000 PyCosmoMMF-0.0.5/MANIFEST.in
--rw-r--r--   0 jamessunseri   (501) staff       (20)     7708 2024-03-23 18:29:26.552345 PyCosmoMMF-0.0.5/PKG-INFO
-drwxr-xr-x   0 jamessunseri   (501) staff       (20)        0 2024-03-23 18:29:26.551651 PyCosmoMMF-0.0.5/PyCosmoMMF/
--rw-r--r--   0 jamessunseri   (501) staff       (20)      346 2024-03-23 18:29:11.000000 PyCosmoMMF-0.0.5/PyCosmoMMF/__init__.py
--rw-r--r--   0 jamessunseri   (501) staff       (20)     4245 2024-03-23 18:28:22.000000 PyCosmoMMF-0.0.5/PyCosmoMMF/filter.py
--rw-r--r--   0 jamessunseri   (501) staff       (20)     1973 2024-03-23 18:27:34.000000 PyCosmoMMF-0.0.5/PyCosmoMMF/hessian.py
--rw-r--r--   0 jamessunseri   (501) staff       (20)     3660 2024-03-23 18:27:51.000000 PyCosmoMMF-0.0.5/PyCosmoMMF/signatures.py
--rw-r--r--   0 jamessunseri   (501) staff       (20)    13385 2024-03-23 18:28:06.000000 PyCosmoMMF-0.0.5/PyCosmoMMF/tagging.py
--rw-r--r--   0 jamessunseri   (501) staff       (20)   131200 2024-03-12 20:43:00.000000 PyCosmoMMF-0.0.5/PyCosmoMMF/test_density_cube.npy
--rw-r--r--   0 jamessunseri   (501) staff       (20)      661 2024-03-23 18:28:11.000000 PyCosmoMMF-0.0.5/PyCosmoMMF/utils.py
-drwxr-xr-x   0 jamessunseri   (501) staff       (20)        0 2024-03-23 18:29:26.552165 PyCosmoMMF-0.0.5/PyCosmoMMF.egg-info/
--rw-r--r--   0 jamessunseri   (501) staff       (20)     7708 2024-03-23 18:29:26.000000 PyCosmoMMF-0.0.5/PyCosmoMMF.egg-info/PKG-INFO
--rw-r--r--   0 jamessunseri   (501) staff       (20)      382 2024-03-23 18:29:26.000000 PyCosmoMMF-0.0.5/PyCosmoMMF.egg-info/SOURCES.txt
--rw-r--r--   0 jamessunseri   (501) staff       (20)        1 2024-03-23 18:29:26.000000 PyCosmoMMF-0.0.5/PyCosmoMMF.egg-info/dependency_links.txt
--rw-r--r--   0 jamessunseri   (501) staff       (20)       11 2024-03-23 18:29:26.000000 PyCosmoMMF-0.0.5/PyCosmoMMF.egg-info/top_level.txt
--rw-r--r--   0 jamessunseri   (501) staff       (20)     6546 2024-03-12 21:49:32.000000 PyCosmoMMF-0.0.5/README.md
--rw-r--r--   0 jamessunseri   (501) staff       (20)      167 2024-03-12 20:11:18.000000 PyCosmoMMF-0.0.5/pyproject.toml
--rw-r--r--   0 jamessunseri   (501) staff       (20)       42 2024-03-12 21:43:49.000000 PyCosmoMMF-0.0.5/requirements.txt
--rw-r--r--   0 jamessunseri   (501) staff       (20)       98 2024-03-23 18:29:26.552543 PyCosmoMMF-0.0.5/setup.cfg
--rw-r--r--   0 jamessunseri   (501) staff       (20)     2188 2024-03-23 18:28:53.000000 PyCosmoMMF-0.0.5/setup.py
+drwxr-xr-x   0 jamessunseri   (501) staff       (20)        0 2024-04-05 21:12:50.768143 PyCosmoMMF-0.0.6/
+-rw-r--r--   0 jamessunseri   (501) staff       (20)     1070 2024-03-12 07:03:50.000000 PyCosmoMMF-0.0.6/LICENSE
+-rw-r--r--   0 jamessunseri   (501) staff       (20)      109 2024-03-12 22:35:52.000000 PyCosmoMMF-0.0.6/MANIFEST.in
+-rw-r--r--   0 jamessunseri   (501) staff       (20)     7708 2024-04-05 21:12:50.768232 PyCosmoMMF-0.0.6/PKG-INFO
+drwxr-xr-x   0 jamessunseri   (501) staff       (20)        0 2024-04-05 21:12:50.767323 PyCosmoMMF-0.0.6/PyCosmoMMF/
+-rw-r--r--   0 jamessunseri   (501) staff       (20)      346 2024-03-23 18:29:11.000000 PyCosmoMMF-0.0.6/PyCosmoMMF/__init__.py
+-rw-r--r--   0 jamessunseri   (501) staff       (20)     4245 2024-03-23 18:28:22.000000 PyCosmoMMF-0.0.6/PyCosmoMMF/filter.py
+-rw-r--r--   0 jamessunseri   (501) staff       (20)     1973 2024-03-23 18:27:34.000000 PyCosmoMMF-0.0.6/PyCosmoMMF/hessian.py
+-rw-r--r--   0 jamessunseri   (501) staff       (20)     3660 2024-03-23 18:27:51.000000 PyCosmoMMF-0.0.6/PyCosmoMMF/signatures.py
+-rw-r--r--   0 jamessunseri   (501) staff       (20)    13385 2024-04-05 21:09:54.000000 PyCosmoMMF-0.0.6/PyCosmoMMF/tagging.py
+-rw-r--r--   0 jamessunseri   (501) staff       (20)   131200 2024-03-12 20:43:00.000000 PyCosmoMMF-0.0.6/PyCosmoMMF/test_density_cube.npy
+-rw-r--r--   0 jamessunseri   (501) staff       (20)      661 2024-03-23 18:28:11.000000 PyCosmoMMF-0.0.6/PyCosmoMMF/utils.py
+drwxr-xr-x   0 jamessunseri   (501) staff       (20)        0 2024-04-05 21:12:50.768022 PyCosmoMMF-0.0.6/PyCosmoMMF.egg-info/
+-rw-r--r--   0 jamessunseri   (501) staff       (20)     7708 2024-04-05 21:12:50.000000 PyCosmoMMF-0.0.6/PyCosmoMMF.egg-info/PKG-INFO
+-rw-r--r--   0 jamessunseri   (501) staff       (20)      382 2024-04-05 21:12:50.000000 PyCosmoMMF-0.0.6/PyCosmoMMF.egg-info/SOURCES.txt
+-rw-r--r--   0 jamessunseri   (501) staff       (20)        1 2024-04-05 21:12:50.000000 PyCosmoMMF-0.0.6/PyCosmoMMF.egg-info/dependency_links.txt
+-rw-r--r--   0 jamessunseri   (501) staff       (20)       11 2024-04-05 21:12:50.000000 PyCosmoMMF-0.0.6/PyCosmoMMF.egg-info/top_level.txt
+-rw-r--r--   0 jamessunseri   (501) staff       (20)     6546 2024-03-12 21:49:32.000000 PyCosmoMMF-0.0.6/README.md
+-rw-r--r--   0 jamessunseri   (501) staff       (20)      167 2024-03-12 20:11:18.000000 PyCosmoMMF-0.0.6/pyproject.toml
+-rw-r--r--   0 jamessunseri   (501) staff       (20)       42 2024-03-12 21:43:49.000000 PyCosmoMMF-0.0.6/requirements.txt
+-rw-r--r--   0 jamessunseri   (501) staff       (20)       98 2024-04-05 21:12:50.768435 PyCosmoMMF-0.0.6/setup.cfg
+-rw-r--r--   0 jamessunseri   (501) staff       (20)     2188 2024-04-05 21:10:16.000000 PyCosmoMMF-0.0.6/setup.py
```

### Comparing `PyCosmoMMF-0.0.5/LICENSE` & `PyCosmoMMF-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCosmoMMF-0.0.5/PKG-INFO` & `PyCosmoMMF-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCosmoMMF
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package for detecting structures in the Cosmic Web.
 Home-page: https://github.com/James11222/PyCosmoMMF/
 Author: James Sunseri
 Author-email: js7501@princeton.edu
 License: MIT
 Project-URL: Bug Reports, https://github.com/James11222/PyCosmoMMF/issues
 Project-URL: Funding, https://donate.pypi.org
```

### Comparing `PyCosmoMMF-0.0.5/PyCosmoMMF/filter.py` & `PyCosmoMMF-0.0.6/PyCosmoMMF/filter.py`

 * *Files identical despite different names*

### Comparing `PyCosmoMMF-0.0.5/PyCosmoMMF/hessian.py` & `PyCosmoMMF-0.0.6/PyCosmoMMF/hessian.py`

 * *Files identical despite different names*

### Comparing `PyCosmoMMF-0.0.5/PyCosmoMMF/signatures.py` & `PyCosmoMMF-0.0.6/PyCosmoMMF/signatures.py`

 * *Files identical despite different names*

### Comparing `PyCosmoMMF-0.0.5/PyCosmoMMF/tagging.py` & `PyCosmoMMF-0.0.6/PyCosmoMMF/tagging.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
     filament_valid = filament_signature[ not_clus_flat ] 
     flat_data_valid = np.reshape(data, N_cells)[ not_clus_flat ]
 
     #Compute Mass Change Curves and Find Filament Threshold
     S_fil, dM2_fil = calc_mass_change(filament_valid, flat_data_valid, Smin, Smax)
     ind = np.argmax(dM2_fil) 
     filament_thresh = S_fil[ind]
-    filbool = (max_sigs[:,:,:,2] > filament_thresh) & (~clusbool)
+    filbool = (max_sigs[:,:,:,1] > filament_thresh) & (~clusbool)
     
     # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 
     #                   Step 3. Create Wall Boolean Filter
     # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 
 
     #Isolate Valid Walls (not clusters or filaments)
     wall_valid_filt = (not_clus_flat) & (filament_signature < filament_thresh)
```

### Comparing `PyCosmoMMF-0.0.5/PyCosmoMMF/test_density_cube.npy` & `PyCosmoMMF-0.0.6/PyCosmoMMF/test_density_cube.npy`

 * *Files identical despite different names*

### Comparing `PyCosmoMMF-0.0.5/PyCosmoMMF/utils.py` & `PyCosmoMMF-0.0.6/PyCosmoMMF/utils.py`

 * *Files identical despite different names*

### Comparing `PyCosmoMMF-0.0.5/PyCosmoMMF.egg-info/PKG-INFO` & `PyCosmoMMF-0.0.6/PyCosmoMMF.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCosmoMMF
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package for detecting structures in the Cosmic Web.
 Home-page: https://github.com/James11222/PyCosmoMMF/
 Author: James Sunseri
 Author-email: js7501@princeton.edu
 License: MIT
 Project-URL: Bug Reports, https://github.com/James11222/PyCosmoMMF/issues
 Project-URL: Funding, https://donate.pypi.org
```

### Comparing `PyCosmoMMF-0.0.5/README.md` & `PyCosmoMMF-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `PyCosmoMMF-0.0.5/setup.py` & `PyCosmoMMF-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from setuptools import setup
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 setup(
     name='PyCosmoMMF',  # Required
-    version='0.0.5',  # Required
+    version='0.0.6',  # Required
     description='A package for detecting structures in the Cosmic Web.',  # Optional
     long_description=(here / 'README.md').read_text(encoding='utf-8'),  # Optional
     long_description_content_type='text/markdown',  # Optional (see note above)
     url='https://github.com/James11222/PyCosmoMMF/',  # Optional
 
     author='James Sunseri',  # Optional
```

