# Comparing `tmp/schwab-py-0.0.0a4.tar.gz` & `tmp/schwab-py-0.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schwab-py-0.0.0a4.tar", last modified: Wed Apr  3 01:48:26 2024, max compression
+gzip compressed data, was "schwab-py-0.0.0a5.tar", last modified: Fri Apr  5 20:01:45 2024, max compression
```

## Comparing `schwab-py-0.0.0a4.tar` & `schwab-py-0.0.0a5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-03 01:48:26.612751 schwab-py-0.0.0a4/
--rw-r--r--   0 alexgolec   (501) staff       (20)     1067 2024-03-26 01:18:54.000000 schwab-py-0.0.0a4/LICENSE
--rw-r--r--   0 alexgolec   (501) staff       (20)     3401 2024-04-03 01:48:26.612682 schwab-py-0.0.0a4/PKG-INFO
--rw-r--r--   0 alexgolec   (501) staff       (20)     2075 2024-03-26 01:18:54.000000 schwab-py-0.0.0a4/README.rst
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-03 01:48:26.610928 schwab-py-0.0.0a4/schwab/
--rw-r--r--   0 alexgolec   (501) staff       (20)      211 2024-04-03 01:16:43.000000 schwab-py-0.0.0a4/schwab/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    24222 2024-04-02 16:02:24.000000 schwab-py-0.0.0a4/schwab/auth.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-03 01:48:26.611428 schwab-py-0.0.0a4/schwab/client/
--rw-r--r--   0 alexgolec   (501) staff       (20)       70 2024-04-01 12:04:09.000000 schwab-py-0.0.0a4/schwab/client/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     2603 2024-04-03 01:45:43.000000 schwab-py-0.0.0a4/schwab/client/asynchronous.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     6566 2024-04-03 01:29:10.000000 schwab-py-0.0.0a4/schwab/client/base.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     2458 2024-04-03 01:45:45.000000 schwab-py-0.0.0a4/schwab/client/synchronous.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     5482 2024-04-03 01:18:33.000000 schwab-py-0.0.0a4/schwab/debug.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     5097 2024-04-01 12:04:09.000000 schwab-py-0.0.0a4/schwab/utils.py
--rw-r--r--   0 alexgolec   (501) staff       (20)       20 2024-04-03 01:48:23.000000 schwab-py-0.0.0a4/schwab/version.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-03 01:48:26.612270 schwab-py-0.0.0a4/schwab_py.egg-info/
--rw-r--r--   0 alexgolec   (501) staff       (20)     3401 2024-04-03 01:48:26.000000 schwab-py-0.0.0a4/schwab_py.egg-info/PKG-INFO
--rw-r--r--   0 alexgolec   (501) staff       (20)      406 2024-04-03 01:48:26.000000 schwab-py-0.0.0a4/schwab_py.egg-info/SOURCES.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)        1 2024-04-03 01:48:26.000000 schwab-py-0.0.0a4/schwab_py.egg-info/dependency_links.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)      105 2024-04-03 01:48:26.000000 schwab-py-0.0.0a4/schwab_py.egg-info/requires.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)        7 2024-04-03 01:48:26.000000 schwab-py-0.0.0a4/schwab_py.egg-info/top_level.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)      568 2024-04-03 01:48:26.613102 schwab-py-0.0.0a4/setup.cfg
--rw-r--r--   0 alexgolec   (501) staff       (20)     1745 2024-04-02 12:03:48.000000 schwab-py-0.0.0a4/setup.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-03 01:48:26.612120 schwab-py-0.0.0a4/tests/
--rw-r--r--   0 alexgolec   (501) staff       (20)      159 2024-04-02 12:25:54.000000 schwab-py-0.0.0a4/tests/test.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-05 20:01:45.446681 schwab-py-0.0.0a5/
+-rw-r--r--   0 alexgolec   (501) staff       (20)     1067 2024-03-26 01:18:54.000000 schwab-py-0.0.0a5/LICENSE
+-rw-r--r--   0 alexgolec   (501) staff       (20)     3518 2024-04-05 20:01:45.446612 schwab-py-0.0.0a5/PKG-INFO
+-rw-r--r--   0 alexgolec   (501) staff       (20)     2075 2024-03-26 01:18:54.000000 schwab-py-0.0.0a5/README.rst
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-05 20:01:45.444779 schwab-py-0.0.0a5/schwab/
+-rw-r--r--   0 alexgolec   (501) staff       (20)      211 2024-04-03 01:16:43.000000 schwab-py-0.0.0a5/schwab/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    24222 2024-04-02 16:02:24.000000 schwab-py-0.0.0a5/schwab/auth.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-05 20:01:45.445280 schwab-py-0.0.0a5/schwab/client/
+-rw-r--r--   0 alexgolec   (501) staff       (20)       70 2024-04-01 12:04:09.000000 schwab-py-0.0.0a5/schwab/client/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     2603 2024-04-03 01:45:43.000000 schwab-py-0.0.0a5/schwab/client/asynchronous.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    18577 2024-04-05 03:46:49.000000 schwab-py-0.0.0a5/schwab/client/base.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     2458 2024-04-03 01:45:45.000000 schwab-py-0.0.0a5/schwab/client/synchronous.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     5482 2024-04-03 01:18:33.000000 schwab-py-0.0.0a5/schwab/debug.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     5097 2024-04-01 12:04:09.000000 schwab-py-0.0.0a5/schwab/utils.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)       20 2024-04-05 20:01:38.000000 schwab-py-0.0.0a5/schwab/version.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-05 20:01:45.446137 schwab-py-0.0.0a5/schwab_py.egg-info/
+-rw-r--r--   0 alexgolec   (501) staff       (20)     3518 2024-04-05 20:01:45.000000 schwab-py-0.0.0a5/schwab_py.egg-info/PKG-INFO
+-rw-r--r--   0 alexgolec   (501) staff       (20)      406 2024-04-05 20:01:45.000000 schwab-py-0.0.0a5/schwab_py.egg-info/SOURCES.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)        1 2024-04-05 20:01:45.000000 schwab-py-0.0.0a5/schwab_py.egg-info/dependency_links.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)      129 2024-04-05 20:01:45.000000 schwab-py-0.0.0a5/schwab_py.egg-info/requires.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)        7 2024-04-05 20:01:45.000000 schwab-py-0.0.0a5/schwab_py.egg-info/top_level.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)      568 2024-04-05 20:01:45.447003 schwab-py-0.0.0a5/setup.cfg
+-rw-r--r--   0 alexgolec   (501) staff       (20)     1814 2024-04-04 00:52:00.000000 schwab-py-0.0.0a5/setup.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-05 20:01:45.445978 schwab-py-0.0.0a5/tests/
+-rw-r--r--   0 alexgolec   (501) staff       (20)      159 2024-04-02 12:25:54.000000 schwab-py-0.0.0a5/tests/test.py
```

### Comparing `schwab-py-0.0.0a4/LICENSE` & `schwab-py-0.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a4/PKG-INFO` & `schwab-py-0.0.0a5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab-py
-Version: 0.0.0a4
+Version: 0.0.0a5
 Summary: Unofficial API wrapper for the upcoming Schwab HTTP API
 Home-page: https://github.com/alexgolec/schwab
 Author: Alex Golec
 Author-email: bottomless.septic.tank@gmail.com
 License: MIT
 Project-URL: Documentation, https://schwab-api.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/alexgolec/schwab-api
@@ -23,17 +23,20 @@
 License-File: LICENSE
 Requires-Dist: authlib
 Requires-Dist: httpx
 Requires-Dist: prompt_toolkit
 Requires-Dist: python-dateutil
 Requires-Dist: selenium
 Provides-Extra: dev
+Requires-Dist: asynctest; extra == "dev"
+Requires-Dist: colorama; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: nose; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytz; extra == "dev"
 Requires-Dist: sphinx_rtd_theme; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 ``schwab-py``: A Schwab API Wrapper
 ========================================
 
 .. image:: https://img.shields.io/discord/720378361880248621.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2
```

### Comparing `schwab-py-0.0.0a4/README.rst` & `schwab-py-0.0.0a5/README.rst`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a4/schwab/auth.py` & `schwab-py-0.0.0a5/schwab/auth.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a4/schwab/client/asynchronous.py` & `schwab-py-0.0.0a5/schwab/client/asynchronous.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a4/schwab/client/synchronous.py` & `schwab-py-0.0.0a5/schwab/client/synchronous.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a4/schwab/debug.py` & `schwab-py-0.0.0a5/schwab/debug.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a4/schwab/utils.py` & `schwab-py-0.0.0a5/schwab/utils.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a4/schwab_py.egg-info/PKG-INFO` & `schwab-py-0.0.0a5/schwab_py.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab-py
-Version: 0.0.0a4
+Version: 0.0.0a5
 Summary: Unofficial API wrapper for the upcoming Schwab HTTP API
 Home-page: https://github.com/alexgolec/schwab
 Author: Alex Golec
 Author-email: bottomless.septic.tank@gmail.com
 License: MIT
 Project-URL: Documentation, https://schwab-api.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/alexgolec/schwab-api
@@ -23,17 +23,20 @@
 License-File: LICENSE
 Requires-Dist: authlib
 Requires-Dist: httpx
 Requires-Dist: prompt_toolkit
 Requires-Dist: python-dateutil
 Requires-Dist: selenium
 Provides-Extra: dev
+Requires-Dist: asynctest; extra == "dev"
+Requires-Dist: colorama; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: nose; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytz; extra == "dev"
 Requires-Dist: sphinx_rtd_theme; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 ``schwab-py``: A Schwab API Wrapper
 ========================================
 
 .. image:: https://img.shields.io/discord/720378361880248621.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2
```

### Comparing `schwab-py-0.0.0a4/setup.cfg` & `schwab-py-0.0.0a5/setup.cfg`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a4/setup.py` & `schwab-py-0.0.0a5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,17 +34,20 @@
         'httpx',
         'prompt_toolkit',
         'python-dateutil',
         'selenium',
     ],
     extras_require={
         'dev': [
+            'asynctest',
+            'colorama',
             'coverage',
             'nose',
             'pytest',
+            'pytz',
             'sphinx_rtd_theme',
             'twine',
         ]
     },
     keywords='finance trading equities bonds options research',
     project_urls={
         'Documentation': 'https://schwab-api.readthedocs.io/en/latest/',
```

