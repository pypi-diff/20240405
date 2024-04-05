# Comparing `tmp/ennemi-1.3.0.tar.gz` & `tmp/ennemi-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ennemi-1.3.0.tar", last modified: Thu Jan 12 07:34:55 2023, max compression
+gzip compressed data, was "ennemi-1.4.0.tar", last modified: Fri Apr  5 07:23:09 2024, max compression
```

## Comparing `ennemi-1.3.0.tar` & `ennemi-1.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 07:34:55.561976 ennemi-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-01-12 07:34:53.000000 ennemi-1.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-01-12 07:34:55.561976 ennemi-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-01-12 07:34:53.000000 ennemi-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 07:34:55.561976 ennemi-1.3.0/ennemi/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-01-12 07:34:53.000000 ennemi-1.3.0/ennemi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38543 2023-01-12 07:34:53.000000 ennemi-1.3.0/ennemi/_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-01-12 07:34:53.000000 ennemi-1.3.0/ennemi/_entropy_estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 07:34:53.000000 ennemi-1.3.0/ennemi/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 07:34:55.561976 ennemi-1.3.0/ennemi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-01-12 07:34:55.000000 ennemi-1.3.0/ennemi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-01-12 07:34:55.000000 ennemi-1.3.0/ennemi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 07:34:55.000000 ennemi-1.3.0/ennemi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-12 07:34:55.000000 ennemi-1.3.0/ennemi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-12 07:34:55.000000 ennemi-1.3.0/ennemi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 07:34:55.561976 ennemi-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-01-12 07:34:53.000000 ennemi-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:23:09.018292 ennemi-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-05 07:23:07.000000 ennemi-1.4.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-05 07:23:09.018292 ennemi-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-05 07:23:07.000000 ennemi-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:23:09.014292 ennemi-1.4.0/ennemi/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-05 07:23:07.000000 ennemi-1.4.0/ennemi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39372 2024-04-05 07:23:07.000000 ennemi-1.4.0/ennemi/_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13471 2024-04-05 07:23:07.000000 ennemi-1.4.0/ennemi/_entropy_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 07:23:07.000000 ennemi-1.4.0/ennemi/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:23:09.014292 ennemi-1.4.0/ennemi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-05 07:23:08.000000 ennemi-1.4.0/ennemi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-05 07:23:08.000000 ennemi-1.4.0/ennemi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 07:23:08.000000 ennemi-1.4.0/ennemi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-05 07:23:08.000000 ennemi-1.4.0/ennemi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 07:23:08.000000 ennemi-1.4.0/ennemi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 07:23:09.018292 ennemi-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-05 07:23:07.000000 ennemi-1.4.0/setup.py
```

### Comparing `ennemi-1.3.0/LICENSE.md` & `ennemi-1.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ennemi-1.3.0/PKG-INFO` & `ennemi-1.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ennemi
-Version: 1.3.0
+Version: 1.4.0
 Summary: Non-linear correlation detection with mutual information
 Home-page: https://polsys.github.io/ennemi/
 Author: Petri Laarne
 Author-email: petri.laarne@helsinki.fi
 License: MIT
 Project-URL: Documentation, https://polsys.github.io/ennemi/
 Project-URL: Source, https://github.com/polsys/ennemi/
@@ -12,24 +12,23 @@
 Project-URL: Zenodo, https://doi.org/10.5281/zenodo.3834018
 Keywords: information-theory entropy mutual-information data-analysis scientific
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Typing :: Typed
-Requires-Python: ~=3.8
+Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
 
 This package performs non-linear correlation analysis with mutual information (MI).
 MI is an information-theoretical measure of dependency between two variables.
 The package is designed for practical data analysis
@@ -44,16 +43,18 @@
   - Interfaces for evaluating multiple variable pairs and time lags with one call
   - Integrated with `pandas` data frames (optional)
   - Optimized and automatically parallelized estimation
   - Algorithms verified to work, so that you can focus on your data
 
 This package depends only on NumPy and SciPy;
 Pandas is suggested for more enjoyable data analysis.
-Python 3.8+ on the latest macOS, Ubuntu and Windows versions
+Recent versions of NumPy 1.x and 2.x are supported.
+Python 3.10+ on the latest macOS, Ubuntu and Windows versions
 is officially supported.
+Older `ennemi` versions have generally identical behavior if you need to run on older Python.
 
 For more information on theoretical background and usage, please see the
 [documentation](https://polsys.github.io/ennemi).
 If you encounter any problems or have suggestions, please file an issue!
 
 ---
```

### Comparing `ennemi-1.3.0/README.md` & `ennemi-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ennemi-1.3.0/ennemi/_driver.py` & `ennemi-1.4.0/ennemi/_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,20 @@
     "You have set normalize=True while at least one variable is discrete. " +\
     "The correlation coefficient formula assumes both variables to be continuous, " +\
     "and the results are not comparable across different discrete variables. " +\
     "Compare the raw MI against entropy of the discrete variable instead. " +\
     "If you really want to calculate correlation coefficients, you can suppress " +\
     "this warning by setting normalize=False and calling normalize_mi() on the results."
 
+PREPROCESS_CONSTANT_DATA_WARNING = \
+    "A variable not marked as discrete takes only a single value, " +\
+    "or values in a very small numerical range. " +\
+    "If this is intentional, you can suppress this warning by passing preprocess=False. " +\
+    "Note that this disables rescaling on all other variables as well."
+
 def normalize_mi(mi: Union[float, GenArrayLike]) -> GenArrayLike:
     """Normalize mutual information values to the unit interval.
 
     Equivalent to passing `normalize=True` to the estimation methods.
 
     The return value matches the correlation coefficient between two Gaussian
     random variables with unit variance. This coefficient is preserved by all
@@ -57,18 +63,24 @@
     mi : array_like or float
         One or more mutual information values (in nats).
         If this is a Pandas `DataFrame` or `Series`, the columns and indices
         are preserved.
     """
 
     # If the parameter is a pandas type, preserve the columns and indices
+    # In pandas 2.1 applymap was renamed to map,
+    # so use that if possible, and fall back to older function if that fails
+    # (since our support goes all the way to pandas 1.0).
     if "pandas" in sys.modules:
         import pandas
         if isinstance(mi, (pandas.DataFrame, pandas.Series)):
-            return mi.applymap(_normalize)
+            if "map" in pandas.DataFrame.__dict__:
+                return mi.map(_normalize)
+            else:
+                return mi.applymap(_normalize)
     
     return np.vectorize(_normalize, otypes=[float])(mi)
 
 def _normalize(mi: float) -> float:
     if mi <= 0.0:
         return mi
     else:
@@ -203,15 +215,15 @@
     # The joint entropy depends on multidim and number of dimensions:
     # In the latter case, the joint entropy is calculated for each x variable
     if multidim or x.ndim == 1:
         xs = _mask_and_validate_entropy(np.column_stack((x, cond)), mask, drop_nan, discrete, k)
         return np.asarray(_call_entropy_func(xs, k, discrete) - marginal)
     else:
         nvar = x.shape[1]
-        joint = np.empty(nvar) # type: npt.NDArray[np.float64]
+        joint = np.empty(nvar)
         for i in range(nvar):
             xs = _mask_and_validate_entropy(np.column_stack((x[:,i], cond)), mask, drop_nan, discrete, k)
             joint[i] = _call_entropy_func(xs, k, discrete)
         return joint - marginal
 
 def _call_entropy_func(xs: FloatArray, k: int, discrete: bool) -> float:
     if discrete:
@@ -324,15 +336,15 @@
     if cond is not None:
         # Make cond 2D
         cond_arr = np.column_stack((np.asarray(cond),))
         ncond = cond_arr.shape[1]
     else:
         cond_arr = None
         ncond = 1
-    mask_arr = None # type: Optional[npt.NDArray[np.float64]]
+    mask_arr = None
     if mask is not None: mask_arr = np.asarray(mask)
 
     # Broadcast cond_lag to be (#lags, #cond vars) in shape
     lag_arr = np.atleast_1d(lag)
     cond_lag_arr = np.broadcast_to(np.column_stack((cond_lag,)), (lag_arr.shape[0], ncond))
 
     # Check the parameters and run the estimation
@@ -586,16 +598,16 @@
         must take two integer parameters, representing the variable indices.
         This method should be very short. Because Python code is not executed
         concurrently, the callback may slow down other estimation tasks.
     """
 
     # Convert arrays to consistent type; _lagged_mi assumes cond to be 2D
     data_arr = np.asarray(data)
-    cond_arr = None # type: Optional[npt.NDArray[np.float64]]
-    mask_arr = None # type: Optional[npt.NDArray[np.float64]]
+    cond_arr = None
+    mask_arr = None
     if cond is not None: cond_arr = np.column_stack((np.asarray(cond),))
     if mask is not None: mask_arr = np.asarray(mask)
 
     # If there is just one variable, return the trivial result
     if data_arr.ndim == 1 or data_arr.shape[1] == 1:
         return np.full((1,1), np.nan)
 
@@ -864,21 +876,33 @@
 
 def _rescale_data(xs: FloatArray, ys: FloatArray, zs: Optional[FloatArray],
         discrete_x: bool, discrete_y: bool) -> Tuple[FloatArray, FloatArray, Optional[FloatArray]]:
     # Digits of e for reproducibility
     rng = np.random.default_rng(2_718281828)
 
     if not discrete_x:
-        # This warns if the standard deviation is zero
-        xs = (xs - xs.mean()) / xs.std()
-        xs += rng.normal(0.0, 1e-10, xs.shape)
+        # Do not try to divide by zero
+        std = xs.std()
+        if np.abs(std) < 1e-20:
+            warn(PREPROCESS_CONSTANT_DATA_WARNING)
+        else:
+            xs = (xs - xs.mean()) / std
+            xs += rng.normal(0.0, 1e-10, xs.shape)
 
     if not discrete_y:
-        ys = (ys - ys.mean()) / ys.std()
-        ys += rng.normal(0.0, 1e-10, ys.shape)
+        std = ys.std()
+        if np.abs(std) < 1e-20:
+            warn(PREPROCESS_CONSTANT_DATA_WARNING)
+        else:
+            ys = (ys - ys.mean()) / std
+            ys += rng.normal(0.0, 1e-10, ys.shape)
     
     # If both X and Y are discrete, we assume the condition to be discrete too
     if zs is not None and not (discrete_x and discrete_y):
-        zs = (zs - zs.mean(axis=0)) / zs.std(axis=0)
-        zs += rng.normal(0.0, 1e-10, zs.shape) # type: ignore # mypy does not realize this is ndarray
+        std = zs.std(axis=0)
+        if np.any(np.abs(std) < 1e-20):
+            warn(PREPROCESS_CONSTANT_DATA_WARNING)
+        else:
+            zs = (zs - zs.mean(axis=0)) / std
+            zs += rng.normal(0.0, 1e-10, zs.shape) # type: ignore # mypy does not realize this is ndarray
 
     return xs, ys, zs
```

### Comparing `ennemi-1.3.0/ennemi/_entropy_estimators.py` & `ennemi-1.4.0/ennemi/_entropy_estimators.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,14 +299,18 @@
 
     N = len(x)
     _assert_not_object(cond)
 
     # Determine probabilities of the conditioning variable
     cond_vals, cond_inverses, cond_counts = np.unique(cond,
         axis=0, return_inverse=True, return_counts=True)
+    
+    # Starting from NumPy 2.0, cond_inverses is multidimensional, so we need to flatten it
+    # This is a no-op for NumPy 1.x
+    cond_inverses = np.ravel(cond_inverses)
 
     # For each condition, compute the conditional probability (given by basic MI on subset of data)
     cond_probs = np.zeros(len(cond_vals))
     for i in range(len(cond_vals)):
         x_subset = x[cond_inverses == i]
         y_subset = y[cond_inverses == i]
         cond_probs[i] = cond_counts[i] * _estimate_discrete_mi(x_subset, y_subset)
```

### Comparing `ennemi-1.3.0/ennemi.egg-info/PKG-INFO` & `ennemi-1.4.0/ennemi.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ennemi
-Version: 1.3.0
+Version: 1.4.0
 Summary: Non-linear correlation detection with mutual information
 Home-page: https://polsys.github.io/ennemi/
 Author: Petri Laarne
 Author-email: petri.laarne@helsinki.fi
 License: MIT
 Project-URL: Documentation, https://polsys.github.io/ennemi/
 Project-URL: Source, https://github.com/polsys/ennemi/
@@ -12,24 +12,23 @@
 Project-URL: Zenodo, https://doi.org/10.5281/zenodo.3834018
 Keywords: information-theory entropy mutual-information data-analysis scientific
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Typing :: Typed
-Requires-Python: ~=3.8
+Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
 
 This package performs non-linear correlation analysis with mutual information (MI).
 MI is an information-theoretical measure of dependency between two variables.
 The package is designed for practical data analysis
@@ -44,16 +43,18 @@
   - Interfaces for evaluating multiple variable pairs and time lags with one call
   - Integrated with `pandas` data frames (optional)
   - Optimized and automatically parallelized estimation
   - Algorithms verified to work, so that you can focus on your data
 
 This package depends only on NumPy and SciPy;
 Pandas is suggested for more enjoyable data analysis.
-Python 3.8+ on the latest macOS, Ubuntu and Windows versions
+Recent versions of NumPy 1.x and 2.x are supported.
+Python 3.10+ on the latest macOS, Ubuntu and Windows versions
 is officially supported.
+Older `ennemi` versions have generally identical behavior if you need to run on older Python.
 
 For more information on theoretical background and usage, please see the
 [documentation](https://polsys.github.io/ennemi).
 If you encounter any problems or have suggestions, please file an issue!
 
 ---
```

### Comparing `ennemi-1.3.0/setup.py` & `ennemi-1.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,33 +6,32 @@
 
 description_file = path.join(path.abspath(path.dirname(__file__)), "DESCRIPTION.md")
 with open(description_file, encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name = "ennemi",
-    version = "1.3.0",
+    version = "1.4.0",
     description = "Non-linear correlation detection with mutual information",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://polsys.github.io/ennemi/",
     author = "Petri Laarne",
     author_email = "petri.laarne@helsinki.fi",
     license = "MIT",
 
     classifiers = [
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Information Analysis",
         "Topic :: Scientific/Engineering :: Mathematics",
         "Topic :: Scientific/Engineering :: Physics",
         "Typing :: Typed"
     ],
     keywords = "information-theory entropy mutual-information data-analysis scientific",
@@ -42,13 +41,13 @@
         "Source": "https://github.com/polsys/ennemi/",
         "Issues": "https://github.com/polsys/ennemi/issues",
         "Zenodo": "https://doi.org/10.5281/zenodo.3834018"
     },
 
     packages = [ "ennemi" ],
     package_data = { "ennemi": ["py.typed"] },
-    python_requires = "~=3.8",
-    install_requires = [ "numpy~=1.21", "scipy~=1.7" ],
+    python_requires = "~=3.10",
+    install_requires = [ "numpy>=1.23", "scipy~=1.9" ],
     extras_require = {
-        "dev": [ "pandas~=1.0", "pytest~=6.2", "mypy~=0.991" ]
+        "dev": [ "pandas>=1.5", "pytest~=8.0", "mypy~=1.9" ]
     }
 )
```

