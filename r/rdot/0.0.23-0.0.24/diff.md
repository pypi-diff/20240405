# Comparing `tmp/rdot-0.0.23.tar.gz` & `tmp/rdot-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdot-0.0.23.tar", last modified: Wed Mar 20 17:26:03 2024, max compression
+gzip compressed data, was "rdot-0.0.24.tar", last modified: Fri Apr  5 04:03:11 2024, max compression
```

## Comparing `rdot-0.0.23.tar` & `rdot-0.0.24.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-03-20 17:26:03.026806 rdot-0.0.23/
--rw-r--r--   0 nathanielimel   (501) staff       (20)    35149 2023-12-11 19:41:32.000000 rdot-0.0.23/LICENSE
--rw-r--r--   0 nathanielimel   (501) staff       (20)     4237 2024-03-20 17:26:03.026454 rdot-0.0.23/PKG-INFO
--rw-r--r--   0 nathanielimel   (501) staff       (20)     3707 2024-03-20 17:23:16.000000 rdot-0.0.23/README.md
--rw-r--r--   0 nathanielimel   (501) staff       (20)       38 2024-03-20 17:26:03.026870 rdot-0.0.23/setup.cfg
--rw-r--r--   0 nathanielimel   (501) staff       (20)      981 2024-03-20 17:25:36.000000 rdot-0.0.23/setup.py
-drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-03-20 17:26:03.019438 rdot-0.0.23/src/
-drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-03-20 17:26:03.023468 rdot-0.0.23/src/rdot/
--rw-r--r--   0 nathanielimel   (501) staff       (20)       63 2024-01-13 19:48:27.000000 rdot-0.0.23/src/rdot/__init__.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)    18197 2024-02-24 09:03:45.000000 rdot-0.0.23/src/rdot/ba.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     2147 2024-01-18 03:41:25.000000 rdot-0.0.23/src/rdot/distortions.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     2274 2024-02-24 08:52:31.000000 rdot-0.0.23/src/rdot/information.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     1440 2024-01-20 07:01:11.000000 rdot-0.0.23/src/rdot/postprocessing.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     1987 2023-12-24 05:50:27.000000 rdot-0.0.23/src/rdot/probability.py
-drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-03-20 17:26:03.025933 rdot-0.0.23/src/rdot.egg-info/
--rw-r--r--   0 nathanielimel   (501) staff       (20)     4237 2024-03-20 17:26:02.000000 rdot-0.0.23/src/rdot.egg-info/PKG-INFO
--rw-r--r--   0 nathanielimel   (501) staff       (20)      363 2024-03-20 17:26:02.000000 rdot-0.0.23/src/rdot.egg-info/SOURCES.txt
--rw-r--r--   0 nathanielimel   (501) staff       (20)        1 2024-03-20 17:26:02.000000 rdot-0.0.23/src/rdot.egg-info/dependency_links.txt
--rw-r--r--   0 nathanielimel   (501) staff       (20)       17 2024-03-20 17:26:02.000000 rdot-0.0.23/src/rdot.egg-info/requires.txt
--rw-r--r--   0 nathanielimel   (501) staff       (20)       11 2024-03-20 17:26:02.000000 rdot-0.0.23/src/rdot.egg-info/top_level.txt
-drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-03-20 17:26:03.025246 rdot-0.0.23/src/tests/
--rw-r--r--   0 nathanielimel   (501) staff       (20)        0 2023-12-01 22:53:39.000000 rdot-0.0.23/src/tests/__init__.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)    17435 2023-12-25 06:35:20.000000 rdot-0.0.23/src/tests/test_rd.py
+drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-04-05 04:03:11.602059 rdot-0.0.24/
+-rw-r--r--   0 nathanielimel   (501) staff       (20)    35149 2023-12-11 19:41:32.000000 rdot-0.0.24/LICENSE
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     4237 2024-04-05 04:03:11.601812 rdot-0.0.24/PKG-INFO
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     3707 2024-03-20 17:23:16.000000 rdot-0.0.24/README.md
+-rw-r--r--   0 nathanielimel   (501) staff       (20)       38 2024-04-05 04:03:11.602097 rdot-0.0.24/setup.cfg
+-rw-r--r--   0 nathanielimel   (501) staff       (20)      981 2024-04-05 04:00:22.000000 rdot-0.0.24/setup.py
+drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-04-05 04:03:11.596578 rdot-0.0.24/src/
+drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-04-05 04:03:11.599919 rdot-0.0.24/src/rdot/
+-rw-r--r--   0 nathanielimel   (501) staff       (20)       97 2024-04-04 19:20:51.000000 rdot-0.0.24/src/rdot/__init__.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)    18197 2024-02-24 09:03:45.000000 rdot-0.0.24/src/rdot/ba.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     2460 2024-04-05 03:55:19.000000 rdot-0.0.24/src/rdot/distortions.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     2274 2024-02-24 08:52:31.000000 rdot-0.0.24/src/rdot/information.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     1440 2024-01-20 07:01:11.000000 rdot-0.0.24/src/rdot/postprocessing.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     1987 2023-12-24 05:50:27.000000 rdot-0.0.24/src/rdot/probability.py
+drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-04-05 04:03:11.601427 rdot-0.0.24/src/rdot.egg-info/
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     4237 2024-04-05 04:03:11.000000 rdot-0.0.24/src/rdot.egg-info/PKG-INFO
+-rw-r--r--   0 nathanielimel   (501) staff       (20)      363 2024-04-05 04:03:11.000000 rdot-0.0.24/src/rdot.egg-info/SOURCES.txt
+-rw-r--r--   0 nathanielimel   (501) staff       (20)        1 2024-04-05 04:03:11.000000 rdot-0.0.24/src/rdot.egg-info/dependency_links.txt
+-rw-r--r--   0 nathanielimel   (501) staff       (20)       17 2024-04-05 04:03:11.000000 rdot-0.0.24/src/rdot.egg-info/requires.txt
+-rw-r--r--   0 nathanielimel   (501) staff       (20)       11 2024-04-05 04:03:11.000000 rdot-0.0.24/src/rdot.egg-info/top_level.txt
+drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-04-05 04:03:11.600915 rdot-0.0.24/src/tests/
+-rw-r--r--   0 nathanielimel   (501) staff       (20)        0 2023-12-01 22:53:39.000000 rdot-0.0.24/src/tests/__init__.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)    16927 2024-04-05 03:49:12.000000 rdot-0.0.24/src/tests/test_rd.py
```

### Comparing `rdot-0.0.23/LICENSE` & `rdot-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `rdot-0.0.23/PKG-INFO` & `rdot-0.0.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdot
-Version: 0.0.23
+Version: 0.0.24
 Summary: Rate distortion optimization tools
 Home-page: https://github.com/nathimel/rdot
 Author: Nathaniel Imel
 Author-email: nimel@uci.edu
 Project-URL: Bug Tracker, https://github.com/nathimel/rdot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `rdot-0.0.23/README.md` & `rdot-0.0.24/README.md`

 * *Files identical despite different names*

### Comparing `rdot-0.0.23/setup.py` & `rdot-0.0.24/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 test_requirements = [
     "pytest",
     "pdoc",
 ]
 
 setuptools.setup(
     name="rdot",
-    version="0.0.23",
+    version="0.0.24",
     author="Nathaniel Imel",
     author_email="nimel@uci.edu",
     description="Rate distortion optimization tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nathimel/rdot",
     project_urls={"Bug Tracker": "https://github.com/nathimel/rdot/issues"},
```

### Comparing `rdot-0.0.23/src/rdot/ba.py` & `rdot-0.0.24/src/rdot/ba.py`

 * *Files identical despite different names*

### Comparing `rdot-0.0.23/src/rdot/distortions.py` & `rdot-0.0.24/src/rdot/distortions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+from scipy.spatial.distance import cdist
 from .information import DKL
 
 def expected_distortion(
     px: np.ndarray, qxhat_x: np.ndarray, dist_mat: np.ndarray
 ) -> float:
     """Compute the expected distortion $E[D[X, \\hat{X}]]$ of a joint distribution defind by $P(X)$ and $P(\\hat{X}|X)$, where
     
@@ -16,18 +17,21 @@
         dist_mat: array of shape `(|X|, |X_hat|)` representing the distoriton matrix between the input alphabet and the reconstruction alphabet.    
     """
     return np.sum(np.diag(px) @ (qxhat_x * dist_mat))
 
 # Pairwise distortion measures
 
 def hamming(x: np.ndarray, y: np.ndarray) -> np.ndarray:
+    """Get a hamming distortion matrix for source and target alphabets of same length as x and y."""
+    # TODO: actually compute hamming between values, instead of assuming x and y are appropriately aligned
     return 1 - np.eye(len(x),len(y))
 
 def quadratic(x: np.ndarray, y: np.ndarray) -> np.ndarray:
-    return np.subtract.outer(x,y)**2
+    """Compute the L2 distance between two arrays of n-dimensional points."""
+    return cdist(x, y)
 
 def ib_kl(py_x: np.ndarray, qy_xhat: np.ndarray) -> np.ndarray:
     # D[p(y|x) || q(y|xhat)]
     return DKL(py_x[:,None,:], qy_xhat[None,:,:], axis=2)
 
 def ib_bin_se(py_x: np.ndarray, qy_xhat: np.ndarray) -> np.ndarray:
     # [ p(y=1|x) - q(y=1|xhat) ]^2
```

### Comparing `rdot-0.0.23/src/rdot/information.py` & `rdot-0.0.24/src/rdot/information.py`

 * *Files identical despite different names*

### Comparing `rdot-0.0.23/src/rdot/postprocessing.py` & `rdot-0.0.24/src/rdot/postprocessing.py`

 * *Files identical despite different names*

### Comparing `rdot-0.0.23/src/rdot/probability.py` & `rdot-0.0.24/src/rdot/probability.py`

 * *Files identical despite different names*

### Comparing `rdot-0.0.23/src/rdot.egg-info/PKG-INFO` & `rdot-0.0.24/src/rdot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdot
-Version: 0.0.23
+Version: 0.0.24
 Summary: Rate distortion optimization tools
 Home-page: https://github.com/nathimel/rdot
 Author: Nathaniel Imel
 Author-email: nimel@uci.edu
 Project-URL: Bug Tracker, https://github.com/nathimel/rdot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `rdot-0.0.23/src/tests/test_rd.py` & `rdot-0.0.24/src/tests/test_rd.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,28 +129,34 @@
         # The more general version of this test would check that all points on the curve satisfy the definition of convexity for a function
 
 
 class TestRDGaussianQuadratic:
 
     """Gaussian random variable with quadratic distortion"""
 
+    # (truncated) Gaussian input with quadratic distortion
+    x = np.linspace(-5,5,1000) # source alphabet
+    xhat = np.linspace(-5,5,1000) # reconstruction alphabet
+    px = 1/(2*np.pi) * np.exp(-x ** 2 / 2) # source pdf
+    px /= px.sum() # guess we actually need this
+
+    # source and target need to be n-dim points, so add dummy dims
+    x = x[:, None]
+    xhat = xhat[:, None]
+
+    dist_mat = distortions.quadratic(x, xhat)
+
     def test_ba_beta_0(self):
-        # (truncated) Gaussian input with quadratic distortion
-        x = np.linspace(-5,5,1000) # source alphabet
-        xhat = np.linspace(-5,5,1000) # reconstruction alphabet
-        px = 1/(2*np.pi) * np.exp(-x ** 2 / 2) # source pdf
-        px /= px.sum() # guess we actually need this
 
-        dist_mat = distortions.quadratic(x, xhat)
         beta = 0.
-        
-        # distortion matrix
-        dist_mat = distortions.hamming(x, xhat)
+
         optimizer = ba.RateDistortionOptimizer(
-            px, dist_mat, np.array([beta]),
+            TestRDGaussianQuadratic.px, 
+            TestRDGaussianQuadratic.dist_mat, 
+            np.array([beta]),
         )
         result, = optimizer.get_results()
         rate = result.rate
         dist = result.distortion
         encoder = result.qxhat_x
 
         true = 2 ** (-2 * rate) # D(R) = σ^2 2^{−2R} in theory, but we truncated
@@ -158,52 +164,45 @@
         assert np.isclose(rate, 0., atol=1e-5)
 
         # Is this too strong a requirement in 'Gaussian' case?
         # expected = np.full_like(encoder, 1/len(xhat))
         # assert np.allclose(expected, encoder, atol=1e-5)
 
     def test_ba_beta_1e10(self):
-        # (truncated) Gaussian input with quadratic distortion
-        x = np.linspace(-5,5,1000) # source alphabet
-        xhat = np.linspace(-5,5,1000) # reconstruction alphabet
-        px = 1/(2*np.pi) * np.exp(-x ** 2 / 2) # source pdf
-        px /= px.sum() # guess we actually need this
 
-        dist_mat = distortions.quadratic(x, xhat)
         beta = 1e10
-        
-        # distortion matrix
-        dist_mat = distortions.hamming(x, xhat)
+
         optimizer = ba.RateDistortionOptimizer(
-            px, dist_mat, np.array([beta]),
-        )
+            TestRDGaussianQuadratic.px, 
+            TestRDGaussianQuadratic.dist_mat, 
+            np.array([beta]),
+        )        
+
         result, = optimizer.get_results()
         rate = result.rate
         dist = result.distortion
         encoder = result.qxhat_x
 
         # deterministic
         assert np.isclose(dist, 0.)
 
-        assert len(np.argwhere(encoder)) == len(xhat)
+        assert len(np.argwhere(encoder)) == len(encoder)
 
     def test_curve(self):
 
-        # (truncated) Gaussian input with quadratic distortion
-        x = np.linspace(-5,5,1000) # source alphabet
-        xhat = np.linspace(-5,5,1000) # reconstruction alphabet
-        px = 1/(2*np.pi) * np.exp(-x ** 2 / 2) # source pdf
-        px /= px.sum() # guess we actually need this
-
-        dist_mat = distortions.quadratic(x, xhat)
 
         # Test many values of beta to sweep out a curve. 
         betas = np.logspace(-5, 5, num=100)
 
-        optimizer = ba.RateDistortionOptimizer(px, dist_mat, betas)
+        optimizer = ba.RateDistortionOptimizer(
+            TestRDGaussianQuadratic.px, 
+            TestRDGaussianQuadratic.dist_mat,
+            betas,
+        )
+
         results = optimizer.get_results()
 
         # rd_values = ba_basic.ba_iterate(px, dist_mat, betas)
 
         # Check for convexity
         ind1 = 20
         ind2 = 30
```

