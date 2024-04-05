# Comparing `tmp/STpipe-sc-0.0.1.tar.gz` & `tmp/STpipe-sc-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "STpipe-sc-0.0.1.tar", last modified: Wed Apr  3 20:45:37 2024, max compression
+gzip compressed data, was "STpipe-sc-0.0.2.tar", last modified: Fri Apr  5 15:10:31 2024, max compression
```

## Comparing `STpipe-sc-0.0.1.tar` & `STpipe-sc-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 20:45:36.981561 STpipe-sc-0.0.1/
--rw-rw-rw-   0        0        0      945 2024-04-03 20:45:36.981561 STpipe-sc-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-03 20:45:36.931587 STpipe-sc-0.0.1/STpipe_sc.egg-info/
--rw-rw-rw-   0        0        0      945 2024-04-03 20:45:36.000000 STpipe-sc-0.0.1/STpipe_sc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2024-04-03 20:45:36.000000 STpipe-sc-0.0.1/STpipe_sc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 20:45:36.000000 STpipe-sc-0.0.1/STpipe_sc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      352 2024-04-03 20:45:36.000000 STpipe-sc-0.0.1/STpipe_sc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-03 20:45:36.000000 STpipe-sc-0.0.1/STpipe_sc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 20:45:36.981561 STpipe-sc-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1081 2024-04-03 20:45:31.000000 STpipe-sc-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:45:36.971565 STpipe-sc-0.0.1/stpipe/
--rw-rw-rw-   0        0        0     3748 2024-03-26 18:54:55.000000 STpipe-sc-0.0.1/stpipe/Findmarkers.py
--rw-rw-rw-   0        0        0    18514 2024-03-31 00:45:27.000000 STpipe-sc-0.0.1/stpipe/QC.py
--rw-rw-rw-   0        0        0      195 2024-03-24 13:36:13.000000 STpipe-sc-0.0.1/stpipe/__init__.py
--rw-rw-rw-   0        0        0     1674 2024-04-01 16:57:25.000000 STpipe-sc-0.0.1/stpipe/cluster.py
--rw-rw-rw-   0        0        0     9970 2024-03-25 17:33:55.000000 STpipe-sc-0.0.1/stpipe/format.py
--rw-rw-rw-   0        0        0    21984 2024-04-03 00:48:54.000000 STpipe-sc-0.0.1/stpipe/function.py
--rw-rw-rw-   0        0        0     2507 2024-03-25 17:08:16.000000 STpipe-sc-0.0.1/stpipe/labeltransfer.py
--rw-rw-rw-   0        0        0    37008 2024-04-02 17:59:02.000000 STpipe-sc-0.0.1/stpipe/plot.py
--rw-rw-rw-   0        0        0     5567 2024-04-03 16:18:46.000000 STpipe-sc-0.0.1/stpipe/spatial_metacell.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:10:31.039553 STpipe-sc-0.0.2/
+-rw-rw-rw-   0        0        0      945 2024-04-05 15:10:31.038596 STpipe-sc-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-05 15:10:30.984085 STpipe-sc-0.0.2/STpipe_sc.egg-info/
+-rw-rw-rw-   0        0        0      945 2024-04-05 15:10:30.000000 STpipe-sc-0.0.2/STpipe_sc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2024-04-05 15:10:30.000000 STpipe-sc-0.0.2/STpipe_sc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 15:10:30.000000 STpipe-sc-0.0.2/STpipe_sc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      352 2024-04-05 15:10:30.000000 STpipe-sc-0.0.2/STpipe_sc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-05 15:10:30.000000 STpipe-sc-0.0.2/STpipe_sc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 15:10:31.039553 STpipe-sc-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1101 2024-04-05 15:10:12.000000 STpipe-sc-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:10:31.028570 STpipe-sc-0.0.2/stpipe/
+-rw-rw-rw-   0        0        0     3748 2024-03-26 18:54:55.000000 STpipe-sc-0.0.2/stpipe/Findmarkers.py
+-rw-rw-rw-   0        0        0    18514 2024-03-31 00:45:27.000000 STpipe-sc-0.0.2/stpipe/QC.py
+-rw-rw-rw-   0        0        0      195 2024-03-24 13:36:13.000000 STpipe-sc-0.0.2/stpipe/__init__.py
+-rw-rw-rw-   0        0        0     1674 2024-04-01 16:57:25.000000 STpipe-sc-0.0.2/stpipe/cluster.py
+-rw-rw-rw-   0        0        0     9970 2024-03-25 17:33:55.000000 STpipe-sc-0.0.2/stpipe/format.py
+-rw-rw-rw-   0        0        0    21984 2024-04-03 00:48:54.000000 STpipe-sc-0.0.2/stpipe/function.py
+-rw-rw-rw-   0        0        0     2507 2024-03-25 17:08:16.000000 STpipe-sc-0.0.2/stpipe/labeltransfer.py
+-rw-rw-rw-   0        0        0    37008 2024-04-02 17:59:02.000000 STpipe-sc-0.0.2/stpipe/plot.py
+-rw-rw-rw-   0        0        0     5567 2024-04-03 16:18:46.000000 STpipe-sc-0.0.2/stpipe/spatial_metacell.py
```

### Comparing `STpipe-sc-0.0.1/PKG-INFO` & `STpipe-sc-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: STpipe-sc
-Version: 0.0.1
+Version: 0.0.2
 Summary: STpipe is designed to analyze spatial transcriptomic data.
 Home-page: https://github.com/mgy520/STpipe
 Author: Mao Guangyao
 License: MIT License
 Requires-Python: ==3.8.18
 Requires-Dist: rpy2==3.5.15
 Requires-Dist: anndata2ri==1.3.1
```

### Comparing `STpipe-sc-0.0.1/STpipe_sc.egg-info/PKG-INFO` & `STpipe-sc-0.0.2/STpipe_sc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: STpipe-sc
-Version: 0.0.1
+Version: 0.0.2
 Summary: STpipe is designed to analyze spatial transcriptomic data.
 Home-page: https://github.com/mgy520/STpipe
 Author: Mao Guangyao
 License: MIT License
 Requires-Python: ==3.8.18
 Requires-Dist: rpy2==3.5.15
 Requires-Dist: anndata2ri==1.3.1
```

### Comparing `STpipe-sc-0.0.1/setup.py` & `STpipe-sc-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from setuptools import setup, find_packages
+from setuptools import setup, find_namespace_packages
 
 setup(
     name='STpipe-sc',
-    version='0.0.1',
+    version='0.0.2',
     description=('STpipe is designed to analyze spatial transcriptomic data.'),
     author='Mao Guangyao',
     license='MIT License',
     url='https://github.com/mgy520/STpipe',
-    packages=find_packages(),
+    packages=find_namespace_packages(),
     python_requires='==3.8.18',
     install_requires=[
             'rpy2==3.5.15',
             'anndata2ri==1.3.1',
             'numpy==1.24.4',
             'diffxpy==0.7.4',
             'scipy==1.10.1',
```

### Comparing `STpipe-sc-0.0.1/stpipe/Findmarkers.py` & `STpipe-sc-0.0.2/stpipe/Findmarkers.py`

 * *Files identical despite different names*

### Comparing `STpipe-sc-0.0.1/stpipe/QC.py` & `STpipe-sc-0.0.2/stpipe/QC.py`

 * *Files identical despite different names*

### Comparing `STpipe-sc-0.0.1/stpipe/cluster.py` & `STpipe-sc-0.0.2/stpipe/cluster.py`

 * *Files identical despite different names*

### Comparing `STpipe-sc-0.0.1/stpipe/format.py` & `STpipe-sc-0.0.2/stpipe/format.py`

 * *Files identical despite different names*

### Comparing `STpipe-sc-0.0.1/stpipe/function.py` & `STpipe-sc-0.0.2/stpipe/function.py`

 * *Files identical despite different names*

### Comparing `STpipe-sc-0.0.1/stpipe/labeltransfer.py` & `STpipe-sc-0.0.2/stpipe/labeltransfer.py`

 * *Files identical despite different names*

### Comparing `STpipe-sc-0.0.1/stpipe/plot.py` & `STpipe-sc-0.0.2/stpipe/plot.py`

 * *Files identical despite different names*

### Comparing `STpipe-sc-0.0.1/stpipe/spatial_metacell.py` & `STpipe-sc-0.0.2/stpipe/spatial_metacell.py`

 * *Files identical despite different names*

