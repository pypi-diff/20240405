# Comparing `tmp/jao-py-0.4.4.tar.gz` & `tmp/jao-py-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jao-py-0.4.4.tar", last modified: Thu Feb 22 14:51:00 2024, max compression
+gzip compressed data, was "jao-py-0.4.5.tar", last modified: Fri Apr  5 07:33:17 2024, max compression
```

## Comparing `jao-py-0.4.4.tar` & `jao-py-0.4.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 14:51:00.187648 jao-py-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-22 14:50:52.000000 jao-py-0.4.4/LICENSE.MD
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-02-22 14:51:00.187648 jao-py-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-02-22 14:50:52.000000 jao-py-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 14:51:00.183648 jao-py-0.4.4/jao/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 14:51:00.183648 jao-py-0.4.4/jao/CWE/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-22 14:50:52.000000 jao-py-0.4.4/jao/CWE/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-22 14:50:52.000000 jao-py-0.4.4/jao/CWE/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-22 14:50:52.000000 jao-py-0.4.4/jao/CWE/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14485 2024-02-22 14:50:52.000000 jao-py-0.4.4/jao/CWE/jao.py
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-02-22 14:50:52.000000 jao-py-0.4.4/jao/CWE/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-02-22 14:50:52.000000 jao-py-0.4.4/jao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-22 14:50:52.000000 jao-py-0.4.4/jao/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-02-22 14:50:52.000000 jao-py-0.4.4/jao/jao.py
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-02-22 14:50:52.000000 jao-py-0.4.4/jao/jao_par_run.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 14:50:52.000000 jao-py-0.4.4/jao/mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-02-22 14:50:52.000000 jao-py-0.4.4/jao/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-22 14:50:52.000000 jao-py-0.4.4/jao/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-02-22 14:50:52.000000 jao-py-0.4.4/jao/webservice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 14:51:00.187648 jao-py-0.4.4/jao_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-02-22 14:51:00.000000 jao-py-0.4.4/jao_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-02-22 14:51:00.000000 jao-py-0.4.4/jao_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 14:51:00.000000 jao-py-0.4.4/jao_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-22 14:51:00.000000 jao-py-0.4.4/jao_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-22 14:51:00.000000 jao-py-0.4.4/jao_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-22 14:51:00.187648 jao-py-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-02-22 14:50:52.000000 jao-py-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:33:17.776136 jao-py-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-05 07:33:14.000000 jao-py-0.4.5/LICENSE.MD
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-05 07:33:17.776136 jao-py-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-05 07:33:14.000000 jao-py-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:33:17.772136 jao-py-0.4.5/jao/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:33:17.776136 jao-py-0.4.5/jao/CWE/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-05 07:33:14.000000 jao-py-0.4.5/jao/CWE/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-05 07:33:14.000000 jao-py-0.4.5/jao/CWE/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-05 07:33:14.000000 jao-py-0.4.5/jao/CWE/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14485 2024-04-05 07:33:14.000000 jao-py-0.4.5/jao/CWE/jao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-05 07:33:14.000000 jao-py-0.4.5/jao/CWE/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-05 07:33:14.000000 jao-py-0.4.5/jao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-05 07:33:14.000000 jao-py-0.4.5/jao/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-04-05 07:33:14.000000 jao-py-0.4.5/jao/jao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-05 07:33:14.000000 jao-py-0.4.5/jao/jao_par_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 07:33:14.000000 jao-py-0.4.5/jao/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-05 07:33:14.000000 jao-py-0.4.5/jao/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-05 07:33:14.000000 jao-py-0.4.5/jao/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-04-05 07:33:14.000000 jao-py-0.4.5/jao/webservice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:33:17.776136 jao-py-0.4.5/jao_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-05 07:33:17.000000 jao-py-0.4.5/jao_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-05 07:33:17.000000 jao-py-0.4.5/jao_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 07:33:17.000000 jao-py-0.4.5/jao_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-05 07:33:17.000000 jao-py-0.4.5/jao_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-05 07:33:17.000000 jao-py-0.4.5/jao_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-05 07:33:17.776136 jao-py-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-05 07:33:14.000000 jao-py-0.4.5/setup.py
```

### Comparing `jao-py-0.4.4/LICENSE.MD` & `jao-py-0.4.5/LICENSE.MD`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Frank Boerman
+Copyright (c) 2024 Frank Boerman
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `jao-py-0.4.4/PKG-INFO` & `jao-py-0.4.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: jao-py
-Version: 0.4.4
+Version: 0.4.5
 Summary: A python API wrapper for JAO.eu
 Home-page: https://github.com/fboerman/jao-py
 Author: Frank Boerman
 Author-email: frank@fboerman.nl
 License: MIT
 Keywords: JAO data api energy
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.MD
 Requires-Dist: requests
 Requires-Dist: pandas
 Requires-Dist: python-dateutil
 Requires-Dist: beautifulsoup4
```

### Comparing `jao-py-0.4.4/README.md` & `jao-py-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `jao-py-0.4.4/jao/CWE/jao.py` & `jao-py-0.4.5/jao/CWE/jao.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.4.4/jao/CWE/parsers.py` & `jao-py-0.4.5/jao/CWE/parsers.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.4.4/jao/jao.py` & `jao-py-0.4.5/jao/jao.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import itertools
 from .exceptions import NoMatchingDataError
 from .parsers import parse_final_domain, parse_base_output
 from typing import List, Dict
 from .util import to_snake_case
 
 __title__ = "jao-py"
-__version__ = "0.4.4"
+__version__ = "0.4.5"
 __author__ = "Frank Boerman"
 __license__ = "MIT"
 
 
 class JaoPublicationToolClient:
     BASEURL = "https://publicationtool.jao.eu/core/api/data/"
 
@@ -96,17 +96,24 @@
         r.raise_for_status()
         data = r.json()['data']
         if len(data) == 0:
             raise NoMatchingDataError
         return data
 
     def _query_base_day(self, day: pd.Timestamp, type: str) -> List[Dict]:
+        d_from = day.replace(hour=0, minute=0)
+        d_to = day.replace(hour=0, minute=0) + pd.Timedelta(days=1)
+        # the api does some funny stuff on dst days, so adjust the to for this edge case
+        if d_from.dst() > d_to.dst():
+            d_to += pd.Timedelta(hours=1)
+        elif d_from.dst() < d_to.dst():
+            d_to -= pd.Timedelta(hours=1)
         return self._query_base_fromto(
-            d_from=day.replace(hour=0, minute=0),
-            d_to=day.replace(hour=0, minute=0) + pd.Timedelta(days=1),
+            d_from=d_from,
+            d_to=d_to,
             type=type
         )
 
     def query_net_position(self, day: pd.Timestamp) -> List[Dict]:
         return self._query_base_day(
             day=day,
             type='netPos'
```

### Comparing `jao-py-0.4.4/jao/jao_par_run.py` & `jao-py-0.4.5/jao/jao_par_run.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.4.4/jao/parsers.py` & `jao-py-0.4.5/jao/parsers.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.4.4/jao/webservice.py` & `jao-py-0.4.5/jao/webservice.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.4.4/jao_py.egg-info/PKG-INFO` & `jao-py-0.4.5/jao_py.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: jao-py
-Version: 0.4.4
+Version: 0.4.5
 Summary: A python API wrapper for JAO.eu
 Home-page: https://github.com/fboerman/jao-py
 Author: Frank Boerman
 Author-email: frank@fboerman.nl
 License: MIT
 Keywords: JAO data api energy
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.MD
 Requires-Dist: requests
 Requires-Dist: pandas
 Requires-Dist: python-dateutil
 Requires-Dist: beautifulsoup4
```

### Comparing `jao-py-0.4.4/setup.py` & `jao-py-0.4.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,74 +4,58 @@
 A setuptools based setup module for jao-py
 
 Adapted from
 https://packaging.python.org/en/latest/distributing.html
 https://github.com/pypa/sampleproject
 """
 
-# Always prefer setuptools over distutils
 from setuptools import setup, find_packages
-# To use a consistent encoding
 from codecs import open
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 
-# Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # Get the version from the source code
 with open(path.join(here, 'jao', 'jao.py'), encoding='utf-8') as f:
     lines = f.readlines()
     for l in lines:
         if l.startswith('__version__'):
-            __version__ = l.split('"')[1] # take the part after the first "
+            __version__ = l.split('"')[1]
 
 setup(
     name='jao-py',
     version=__version__,
     description='A python API wrapper for JAO.eu',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/fboerman/jao-py',
     author='Frank Boerman',
     author_email='frank@fboerman.nl',
     license='MIT',
 
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
 
-        # Indicate who your project is intended for
         'Intended Audience :: Developers',
         'Topic :: Scientific/Engineering',
 
-        # Pick your license as you wish (should match "license" above)
         'License :: OSI Approved :: MIT License',
 
-        # Specify the Python versions you support here. In particular, ensure
-        # that you indicate whether you support Python 2, Python 3 or both.
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 
     keywords='JAO data api energy',
 
-    # You can just specify the packages manually here if your project is
-    # simple. Or you can use find_packages().
     packages=find_packages(),
 
-
-    # List run-time dependencies here.  These will be installed by pip when
-    # your project is installed.
     install_requires=['requests', 'pandas', 'python-dateutil', 'beautifulsoup4'],
 
-    # If there are data files included in your packages that need to be
-    # installed, specify them here.  If using Python 2.6 or less, then these
-    # have to be included in MANIFEST.in as well.
-    # Note: for creating the source distribution, they had to be included in the
-    # MANIFEST.in as well.
     package_data={
         'jao-py': ['LICENSE.md', 'README.md'],
     },
 )
```

