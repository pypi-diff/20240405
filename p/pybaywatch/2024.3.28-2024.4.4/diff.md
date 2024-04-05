# Comparing `tmp/pybaywatch-2024.3.28.tar.gz` & `tmp/pybaywatch-2024.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybaywatch-2024.3.28.tar", last modified: Fri Mar 29 01:22:44 2024, max compression
+gzip compressed data, was "pybaywatch-2024.4.4.tar", last modified: Fri Apr  5 00:41:37 2024, max compression
```

## Comparing `pybaywatch-2024.3.28.tar` & `pybaywatch-2024.4.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-03-29 01:22:44.770475 pybaywatch-2024.3.28/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1065 2024-03-17 02:29:06.000000 pybaywatch-2024.3.28/LICENSE
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       33 2024-03-17 18:02:15.000000 pybaywatch-2024.3.28/MANIFEST.in
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      482 2024-03-29 01:22:44.769445 pybaywatch-2024.3.28/PKG-INFO
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       32 2024-03-17 02:29:06.000000 pybaywatch-2024.3.28/README.md
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-03-29 01:22:44.026342 pybaywatch-2024.3.28/pybaywatch/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     3119 2024-03-27 06:04:37.000000 pybaywatch-2024.3.28/pybaywatch/TEX_forward.m
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1717 2024-03-28 04:18:11.000000 pybaywatch-2024.3.28/pybaywatch/UK_forward.m
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      276 2024-03-28 04:36:12.000000 pybaywatch-2024.3.28/pybaywatch/__init__.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2131 2024-03-28 04:25:40.000000 pybaywatch-2024.3.28/pybaywatch/bayfox_forward.m
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     7017 2024-03-29 01:14:10.000000 pybaywatch-2024.3.28/pybaywatch/baymag_forward_ln.m
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2824 2024-03-28 03:57:42.000000 pybaywatch-2024.3.28/pybaywatch/baymbt_forward.m
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    12818 2024-03-29 01:19:40.000000 pybaywatch-2024.3.28/pybaywatch/core.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      461 2024-03-24 20:42:45.000000 pybaywatch-2024.3.28/pybaywatch/fnval.m
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1256 2024-03-17 16:27:16.000000 pybaywatch-2024.3.28/pybaywatch/normrnd.m
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     4622 2024-03-24 20:43:51.000000 pybaywatch-2024.3.28/pybaywatch/randsample.m
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     7777 2024-03-17 16:38:54.000000 pybaywatch-2024.3.28/pybaywatch/rndcheck.m
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2960 2024-03-24 20:59:29.000000 pybaywatch-2024.3.28/pybaywatch/utils.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     3900 2024-03-29 01:12:36.000000 pybaywatch-2024.3.28/pybaywatch/wrapper.py
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-03-29 01:22:44.768681 pybaywatch-2024.3.28/pybaywatch.egg-info/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      482 2024-03-29 01:22:41.000000 pybaywatch-2024.3.28/pybaywatch.egg-info/PKG-INFO
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      546 2024-03-29 01:22:42.000000 pybaywatch-2024.3.28/pybaywatch.egg-info/SOURCES.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2024-03-29 01:22:41.000000 pybaywatch-2024.3.28/pybaywatch.egg-info/dependency_links.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2024-03-17 02:47:06.000000 pybaywatch-2024.3.28/pybaywatch.egg-info/not-zip-safe
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       16 2024-03-29 01:22:41.000000 pybaywatch-2024.3.28/pybaywatch.egg-info/requires.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       11 2024-03-29 01:22:41.000000 pybaywatch-2024.3.28/pybaywatch.egg-info/top_level.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       38 2024-03-29 01:22:44.770600 pybaywatch-2024.3.28/setup.cfg
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      763 2024-03-29 01:22:07.000000 pybaywatch-2024.3.28/setup.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-05 00:41:37.238664 pybaywatch-2024.4.4/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1065 2024-03-17 02:29:06.000000 pybaywatch-2024.4.4/LICENSE
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       33 2024-03-17 18:02:15.000000 pybaywatch-2024.4.4/MANIFEST.in
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      481 2024-04-05 00:41:37.236826 pybaywatch-2024.4.4/PKG-INFO
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       32 2024-03-17 02:29:06.000000 pybaywatch-2024.4.4/README.md
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-05 00:41:37.228649 pybaywatch-2024.4.4/pybaywatch/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     3119 2024-03-27 06:04:37.000000 pybaywatch-2024.4.4/pybaywatch/TEX_forward.m
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1717 2024-03-28 04:18:11.000000 pybaywatch-2024.4.4/pybaywatch/UK_forward.m
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      276 2024-03-28 04:36:12.000000 pybaywatch-2024.4.4/pybaywatch/__init__.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2131 2024-03-28 04:25:40.000000 pybaywatch-2024.4.4/pybaywatch/bayfox_forward.m
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     7017 2024-03-29 01:14:10.000000 pybaywatch-2024.4.4/pybaywatch/baymag_forward_ln.m
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2824 2024-03-28 03:57:42.000000 pybaywatch-2024.4.4/pybaywatch/baymbt_forward.m
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    12833 2024-04-04 23:45:06.000000 pybaywatch-2024.4.4/pybaywatch/core.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      461 2024-03-24 20:42:45.000000 pybaywatch-2024.4.4/pybaywatch/fnval.m
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1256 2024-03-17 16:27:16.000000 pybaywatch-2024.4.4/pybaywatch/normrnd.m
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     4622 2024-03-24 20:43:51.000000 pybaywatch-2024.4.4/pybaywatch/randsample.m
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     7777 2024-03-17 16:38:54.000000 pybaywatch-2024.4.4/pybaywatch/rndcheck.m
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2960 2024-03-24 20:59:29.000000 pybaywatch-2024.4.4/pybaywatch/utils.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     3900 2024-03-29 01:12:36.000000 pybaywatch-2024.4.4/pybaywatch/wrapper.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-05 00:41:37.235517 pybaywatch-2024.4.4/pybaywatch.egg-info/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      481 2024-04-05 00:41:37.229673 pybaywatch-2024.4.4/pybaywatch.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      546 2024-04-05 00:41:37.230452 pybaywatch-2024.4.4/pybaywatch.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2024-04-05 00:41:37.232131 pybaywatch-2024.4.4/pybaywatch.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2024-03-17 02:47:06.000000 pybaywatch-2024.4.4/pybaywatch.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       16 2024-04-05 00:41:37.234371 pybaywatch-2024.4.4/pybaywatch.egg-info/requires.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       11 2024-04-05 00:41:37.235621 pybaywatch-2024.4.4/pybaywatch.egg-info/top_level.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       38 2024-04-05 00:41:37.238788 pybaywatch-2024.4.4/setup.cfg
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      762 2024-04-05 00:41:15.000000 pybaywatch-2024.4.4/setup.py
```

### Comparing `pybaywatch-2024.3.28/LICENSE` & `pybaywatch-2024.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pybaywatch-2024.3.28/pybaywatch/TEX_forward.m` & `pybaywatch-2024.4.4/pybaywatch/TEX_forward.m`

 * *Files identical despite different names*

### Comparing `pybaywatch-2024.3.28/pybaywatch/UK_forward.m` & `pybaywatch-2024.4.4/pybaywatch/UK_forward.m`

 * *Files identical despite different names*

### Comparing `pybaywatch-2024.3.28/pybaywatch/bayfox_forward.m` & `pybaywatch-2024.4.4/pybaywatch/bayfox_forward.m`

 * *Files identical despite different names*

### Comparing `pybaywatch-2024.3.28/pybaywatch/baymag_forward_ln.m` & `pybaywatch-2024.4.4/pybaywatch/baymag_forward_ln.m`

 * *Files identical despite different names*

### Comparing `pybaywatch-2024.3.28/pybaywatch/baymbt_forward.m` & `pybaywatch-2024.4.4/pybaywatch/baymbt_forward.m`

 * *Files identical despite different names*

### Comparing `pybaywatch-2024.3.28/pybaywatch/core.py` & `pybaywatch-2024.4.4/pybaywatch/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,15 +286,15 @@
 
         # Calculate the ratio to the modern value and convert to log units
         # H: Optional exponent (if provided)
         mgsw = np.log((mgsw_interp / mg_mod) ** H)
     else:
         mgsw = 0
 
-    lmg_mean = alpha.T + sst[:, np.newaxis] * betaT.T + omega * betaO.T + salinity * betaS.T + (1 - clean * betaC.T) + mgsw.T
+    lmg_mean = alpha.T + sst[:, np.newaxis] * betaT.T + omega * betaO.T + salinity[:, np.newaxis] * betaS.T + (1 - clean * betaC.T) + mgsw.T
     if idx < 2:  # If you selected ruber, bulloides, or the "all" models, assume pH sensitivity
         lmg_mean += pH * betaP.T
 
     lmg_sig = sigma.T
     lmg = lmg_mean + np.random.randn(nobs, nparams) * lmg_sig
 
     return lmg
```

### Comparing `pybaywatch-2024.3.28/pybaywatch/normrnd.m` & `pybaywatch-2024.4.4/pybaywatch/normrnd.m`

 * *Files identical despite different names*

### Comparing `pybaywatch-2024.3.28/pybaywatch/randsample.m` & `pybaywatch-2024.4.4/pybaywatch/randsample.m`

 * *Files identical despite different names*

### Comparing `pybaywatch-2024.3.28/pybaywatch/rndcheck.m` & `pybaywatch-2024.4.4/pybaywatch/rndcheck.m`

 * *Files identical despite different names*

### Comparing `pybaywatch-2024.3.28/pybaywatch/utils.py` & `pybaywatch-2024.4.4/pybaywatch/utils.py`

 * *Files identical despite different names*

### Comparing `pybaywatch-2024.3.28/pybaywatch/wrapper.py` & `pybaywatch-2024.4.4/pybaywatch/wrapper.py`

 * *Files identical despite different names*

### Comparing `pybaywatch-2024.3.28/pybaywatch.egg-info/SOURCES.txt` & `pybaywatch-2024.4.4/pybaywatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybaywatch-2024.3.28/setup.py` & `pybaywatch-2024.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='pybaywatch',  # required
-    version='2024.3.28',
+    version='2024.4.4',
     description='PyBAYWATCH: BAYWATCH in Python',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Jessica Tierney',
     author_email='fengzhu@ucar.edu, jesst@arizona.edu',
     url='https://github.com/fzhu2e/pybaywatch',
     packages=find_packages(),
```

