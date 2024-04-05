# Comparing `tmp/insilicova-0.1.0.tar.gz` & `tmp/insilicova-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insilicova-0.1.0.tar", last modified: Tue Apr  2 15:24:46 2024, max compression
+gzip compressed data, was "insilicova-0.1.1.tar", last modified: Fri Apr  5 17:05:30 2024, max compression
```

## Comparing `insilicova-0.1.0.tar` & `insilicova-0.1.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:24:46.670824 insilicova-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-02 15:24:42.000000 insilicova-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-02 15:24:42.000000 insilicova-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-02 15:24:46.670824 insilicova-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-02 15:24:42.000000 insilicova-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-02 15:24:42.000000 insilicova-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 15:24:46.670824 insilicova-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-02 15:24:42.000000 insilicova-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:24:46.658824 insilicova-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:24:46.658824 insilicova-0.1.0/src/insilicova/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:24:42.000000 insilicova-0.1.0/src/insilicova/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:24:46.662824 insilicova-0.1.0/src/insilicova/_sampler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:24:42.000000 insilicova-0.1.0/src/insilicova/_sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47895 2024-04-02 15:24:42.000000 insilicova-0.1.0/src/insilicova/_sampler/sampler.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    76716 2024-04-02 15:24:42.000000 insilicova-0.1.0/src/insilicova/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:24:46.666824 insilicova-0.1.0/src/insilicova/data/
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-02 15:24:42.000000 insilicova-0.1.0/src/insilicova/data/causetext.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-02 15:24:42.000000 insilicova-0.1.0/src/insilicova/data/causetextV5.csv
--rw-r--r--   0 runner    (1001) docker     (127)    61954 2024-04-02 15:24:42.000000 insilicova-0.1.0/src/insilicova/data/condprob.csv
--rw-r--r--   0 runner    (1001) docker     (127)    74841 2024-04-02 15:24:42.000000 insilicova-0.1.0/src/insilicova/data/condprobnum.csv
--rw-r--r--   0 runner    (1001) docker     (127)    96815 2024-04-02 15:24:42.000000 insilicova-0.1.0/src/insilicova/data/probbase.csv
--rw-r--r--   0 runner    (1001) docker     (127)    96856 2024-04-02 15:24:42.000000 insilicova-0.1.0/src/insilicova/data/probbaseV3.csv
--rw-r--r--   0 runner    (1001) docker     (127)   164661 2024-04-02 15:24:42.000000 insilicova-0.1.0/src/insilicova/data/probbaseV5.csv
--rw-r--r--   0 runner    (1001) docker     (127)   944653 2024-04-02 15:24:42.000000 insilicova-0.1.0/src/insilicova/data/random_physician.csv
--rw-r--r--   0 runner    (1001) docker     (127)   912053 2024-04-02 15:24:42.000000 insilicova-0.1.0/src/insilicova/data/randomva1.csv
--rw-r--r--   0 runner    (1001) docker     (127)   925145 2024-04-02 15:24:42.000000 insilicova-0.1.0/src/insilicova/data/randomva2.csv
--rw-r--r--   0 runner    (1001) docker     (127)   286521 2024-04-02 15:24:42.000000 insilicova-0.1.0/src/insilicova/data/randomva5.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-02 15:24:42.000000 insilicova-0.1.0/src/insilicova/data/sample_category.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-04-02 15:24:42.000000 insilicova-0.1.0/src/insilicova/data/sample_physician.csv
--rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-04-02 15:24:42.000000 insilicova-0.1.0/src/insilicova/diag.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-02 15:24:42.000000 insilicova-0.1.0/src/insilicova/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    24139 2024-04-02 15:24:42.000000 insilicova-0.1.0/src/insilicova/indiv.py
--rw-r--r--   0 runner    (1001) docker     (127)    13455 2024-04-02 15:24:42.000000 insilicova-0.1.0/src/insilicova/structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-02 15:24:42.000000 insilicova-0.1.0/src/insilicova/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:24:46.670824 insilicova-0.1.0/src/insilicova.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-02 15:24:46.000000 insilicova-0.1.0/src/insilicova.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-02 15:24:46.000000 insilicova-0.1.0/src/insilicova.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:24:46.000000 insilicova-0.1.0/src/insilicova.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 15:24:46.000000 insilicova-0.1.0/src/insilicova.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 15:24:46.000000 insilicova-0.1.0/src/insilicova.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:24:46.670824 insilicova-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-02 15:24:42.000000 insilicova-0.1.0/tests/test_compare_r.py
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-02 15:24:42.000000 insilicova-0.1.0/tests/test_diag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-02 15:24:42.000000 insilicova-0.1.0/tests/test_indiv.py
--rw-r--r--   0 runner    (1001) docker     (127)    34028 2024-04-02 15:24:42.000000 insilicova-0.1.0/tests/test_insilicova.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:05:30.685387 insilicova-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-05 17:05:26.000000 insilicova-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-05 17:05:26.000000 insilicova-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-05 17:05:30.685387 insilicova-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-05 17:05:26.000000 insilicova-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-05 17:05:26.000000 insilicova-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 17:05:30.685387 insilicova-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-05 17:05:26.000000 insilicova-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:05:30.673387 insilicova-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:05:30.677387 insilicova-0.1.1/src/insilicova/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:05:30.677387 insilicova-0.1.1/src/insilicova/_sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/_sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47895 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/_sampler/sampler.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    76716 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:05:30.685387 insilicova-0.1.1/src/insilicova/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/data/causetext.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/data/causetextV5.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    61954 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/data/condprob.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    74841 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/data/condprobnum.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    96815 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/data/probbase.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    96856 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/data/probbaseV3.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   164661 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/data/probbaseV5.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   944653 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/data/random_physician.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   912053 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/data/randomva1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   925145 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/data/randomva2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   286521 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/data/randomva5.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/data/sample_category.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/data/sample_physician.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/diag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24139 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/indiv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13455 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:05:30.685387 insilicova-0.1.1/src/insilicova.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-05 17:05:30.000000 insilicova-0.1.1/src/insilicova.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-05 17:05:30.000000 insilicova-0.1.1/src/insilicova.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:05:30.000000 insilicova-0.1.1/src/insilicova.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-05 17:05:30.000000 insilicova-0.1.1/src/insilicova.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 17:05:30.000000 insilicova-0.1.1/src/insilicova.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:05:30.685387 insilicova-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-05 17:05:26.000000 insilicova-0.1.1/tests/test_compare_r.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-05 17:05:26.000000 insilicova-0.1.1/tests/test_diag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-05 17:05:26.000000 insilicova-0.1.1/tests/test_indiv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34028 2024-04-05 17:05:26.000000 insilicova-0.1.1/tests/test_insilicova.py
```

### Comparing `insilicova-0.1.0/LICENSE` & `insilicova-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.0/PKG-INFO` & `insilicova-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insilicova
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python implementation of the InSilicoVA Algorithm.
 Author-email: Jason Thomas <jarathomas@gmail.com>, Sherry Zhao <zhao.3248@buckeyemail.osu.edu>
 Maintainer-email: Jason Thomas <jarathomas@gmail.com>
 License: GPLv3
 Project-URL: Homepage, https://github.com/verbal-autopsy-software/pyinsilicova
 Project-URL: Bug Tracker, https://github.com/verbal-autopsy-software/pyinsilicoVA/issues
 Keywords: verbal autopsy
@@ -17,24 +17,29 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: numpy
-Requires-Dist: vacheck>=0.0.2
+Requires-Dist: vacheck>=0.0.3
 Requires-Dist: statsmodels
 Requires-Dist: scipy
 
-# pyinsilicova
+# insilicova (Python version)
 
-[![pytest](https://github.com/verbal-autopsy-software/pyinsilicova/actions/workflows/python-package.yml/badge.svg)](https://github.com/verbal-autopsy-software/pyinsilicova/actions)
+[![image](https://img.shields.io/pypi/pyversions/insilicova)](https://pypi.org/project/insilicova/)
 
 
-Python implementation of the InSilicoVA algorithm for assigning causes of death to verbal autopsy (VA) data collected with the 2016 WHO VA instrument.
+Python implementation of the InSilicoVA algorithm for assigning causes of death
+to verbal autopsy (VA) data collected with the 2016 WHO VA instrument.  This
+package is an attempt to replicate the R version
+[InSilicoVA](https://github.com/verbal-autopsy-software/InSilicoVA), but the R
+version offers more features and functionality via the
+[openva](https://github.com/verbal-autopsy-software/openVA) R package.
 
 Example run:
 
 ```python
 from insilicova.api import InSilicoVA
 from insilicova.utils import get_vadata
 
@@ -46,14 +51,16 @@
 results.get_summary() # prints CSMF
 results.get_csmf()    # returns CSMF
 ```
 
 
 ## Build Dependencies
 
-This package depends on the C++ library boost (v1.82.0) [https://www.boost.org/](https://www.boost.org/) and the Python package
-pyind11 ([pybind11 docs](https://pybind11.readthedocs.io/en/latest/)).
+The insilicova package depends on the C++ library [boost](https://www.boost.org/)
+(v1.82.0), and the Python package [pyind11](https://github.com/pybind/pybind11)
+([pybind11 docs](https://pybind11.readthedocs.io/en/latest/)) is used to help build insilicova.
 
-* On Windows it is assumed that boost is installed at: `C:\Program Files\boost\boost_1_82_0` (as specified in `setup.py`)
+* On Windows it is assumed that boost is installed at:
+  `C:\Program Files\boost\boost_1_82_0` (as specified in `setup.py`)
 
 * Build the package with `python -m build`
```

### Comparing `insilicova-0.1.0/pyproject.toml` & `insilicova-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 build-requires = [
     "virtual:compiler/cpp",
     "pkg:generic/boost",
 ]
 
 [project]
 name = "insilicova"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     {name = "Jason Thomas", email = "jarathomas@gmail.com"},
     {name = "Sherry Zhao", email =" zhao.3248@buckeyemail.osu.edu"},
 ]
 maintainers = [
     {name = "Jason Thomas", email = "jarathomas@gmail.com"},
 ]
@@ -35,15 +35,15 @@
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
 ]
 dependencies = [
         "pandas",
         "numpy",
-        "vacheck >= 0.0.2",
+        "vacheck>=0.0.3",
         "statsmodels",
         "scipy",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/verbal-autopsy-software/pyinsilicova"
 "Bug Tracker" = "https://github.com/verbal-autopsy-software/pyinsilicoVA/issues"
```

### Comparing `insilicova-0.1.0/setup.py` & `insilicova-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.0/src/insilicova/_sampler/sampler.cpp` & `insilicova-0.1.1/src/insilicova/_sampler/sampler.cpp`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.0/src/insilicova/api.py` & `insilicova-0.1.1/src/insilicova/api.py`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.0/src/insilicova/data/causetext.csv` & `insilicova-0.1.1/src/insilicova/data/causetext.csv`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.0/src/insilicova/data/causetextV5.csv` & `insilicova-0.1.1/src/insilicova/data/causetextV5.csv`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.0/src/insilicova/data/condprob.csv` & `insilicova-0.1.1/src/insilicova/data/condprob.csv`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.0/src/insilicova/data/condprobnum.csv` & `insilicova-0.1.1/src/insilicova/data/condprobnum.csv`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.0/src/insilicova/data/probbase.csv` & `insilicova-0.1.1/src/insilicova/data/probbase.csv`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.0/src/insilicova/data/probbaseV3.csv` & `insilicova-0.1.1/src/insilicova/data/probbaseV3.csv`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.0/src/insilicova/data/probbaseV5.csv` & `insilicova-0.1.1/src/insilicova/data/probbaseV5.csv`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.0/src/insilicova/data/random_physician.csv` & `insilicova-0.1.1/src/insilicova/data/random_physician.csv`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.0/src/insilicova/data/randomva1.csv` & `insilicova-0.1.1/src/insilicova/data/randomva1.csv`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.0/src/insilicova/data/randomva2.csv` & `insilicova-0.1.1/src/insilicova/data/randomva2.csv`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.0/src/insilicova/data/randomva5.csv` & `insilicova-0.1.1/src/insilicova/data/randomva5.csv`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.0/src/insilicova/data/sample_category.csv` & `insilicova-0.1.1/src/insilicova/data/sample_category.csv`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.0/src/insilicova/data/sample_physician.csv` & `insilicova-0.1.1/src/insilicova/data/sample_physician.csv`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.0/src/insilicova/diag.py` & `insilicova-0.1.1/src/insilicova/diag.py`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.0/src/insilicova/exceptions.py` & `insilicova-0.1.1/src/insilicova/exceptions.py`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.0/src/insilicova/indiv.py` & `insilicova-0.1.1/src/insilicova/indiv.py`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.0/src/insilicova/structures.py` & `insilicova-0.1.1/src/insilicova/structures.py`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.0/src/insilicova/utils.py` & `insilicova-0.1.1/src/insilicova/utils.py`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.0/src/insilicova.egg-info/PKG-INFO` & `insilicova-0.1.1/src/insilicova.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insilicova
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python implementation of the InSilicoVA Algorithm.
 Author-email: Jason Thomas <jarathomas@gmail.com>, Sherry Zhao <zhao.3248@buckeyemail.osu.edu>
 Maintainer-email: Jason Thomas <jarathomas@gmail.com>
 License: GPLv3
 Project-URL: Homepage, https://github.com/verbal-autopsy-software/pyinsilicova
 Project-URL: Bug Tracker, https://github.com/verbal-autopsy-software/pyinsilicoVA/issues
 Keywords: verbal autopsy
@@ -17,24 +17,29 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: numpy
-Requires-Dist: vacheck>=0.0.2
+Requires-Dist: vacheck>=0.0.3
 Requires-Dist: statsmodels
 Requires-Dist: scipy
 
-# pyinsilicova
+# insilicova (Python version)
 
-[![pytest](https://github.com/verbal-autopsy-software/pyinsilicova/actions/workflows/python-package.yml/badge.svg)](https://github.com/verbal-autopsy-software/pyinsilicova/actions)
+[![image](https://img.shields.io/pypi/pyversions/insilicova)](https://pypi.org/project/insilicova/)
 
 
-Python implementation of the InSilicoVA algorithm for assigning causes of death to verbal autopsy (VA) data collected with the 2016 WHO VA instrument.
+Python implementation of the InSilicoVA algorithm for assigning causes of death
+to verbal autopsy (VA) data collected with the 2016 WHO VA instrument.  This
+package is an attempt to replicate the R version
+[InSilicoVA](https://github.com/verbal-autopsy-software/InSilicoVA), but the R
+version offers more features and functionality via the
+[openva](https://github.com/verbal-autopsy-software/openVA) R package.
 
 Example run:
 
 ```python
 from insilicova.api import InSilicoVA
 from insilicova.utils import get_vadata
 
@@ -46,14 +51,16 @@
 results.get_summary() # prints CSMF
 results.get_csmf()    # returns CSMF
 ```
 
 
 ## Build Dependencies
 
-This package depends on the C++ library boost (v1.82.0) [https://www.boost.org/](https://www.boost.org/) and the Python package
-pyind11 ([pybind11 docs](https://pybind11.readthedocs.io/en/latest/)).
+The insilicova package depends on the C++ library [boost](https://www.boost.org/)
+(v1.82.0), and the Python package [pyind11](https://github.com/pybind/pybind11)
+([pybind11 docs](https://pybind11.readthedocs.io/en/latest/)) is used to help build insilicova.
 
-* On Windows it is assumed that boost is installed at: `C:\Program Files\boost\boost_1_82_0` (as specified in `setup.py`)
+* On Windows it is assumed that boost is installed at:
+  `C:\Program Files\boost\boost_1_82_0` (as specified in `setup.py`)
 
 * Build the package with `python -m build`
```

### Comparing `insilicova-0.1.0/src/insilicova.egg-info/SOURCES.txt` & `insilicova-0.1.1/src/insilicova.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.0/tests/test_compare_r.py` & `insilicova-0.1.1/tests/test_compare_r.py`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.0/tests/test_diag.py` & `insilicova-0.1.1/tests/test_diag.py`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.0/tests/test_indiv.py` & `insilicova-0.1.1/tests/test_indiv.py`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.0/tests/test_insilicova.py` & `insilicova-0.1.1/tests/test_insilicova.py`

 * *Files identical despite different names*

