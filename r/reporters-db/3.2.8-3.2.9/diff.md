# Comparing `tmp/reporters-db-3.2.8.tar.gz` & `tmp/reporters-db-3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reporters-db-3.2.8.tar", last modified: Thu Jan  6 01:07:52 2022, max compression
+gzip compressed data, was "reporters-db-3.2.9.tar", last modified: Thu Jan  6 17:51:20 2022, max compression
```

## Comparing `reporters-db-3.2.8.tar` & `reporters-db-3.2.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 01:07:52.312643 reporters-db-3.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1300 2022-01-06 01:07:47.000000 reporters-db-3.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-01-06 01:07:47.000000 reporters-db-3.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    13657 2022-01-06 01:07:52.312643 reporters-db-3.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10460 2022-01-06 01:07:47.000000 reporters-db-3.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-01-06 01:07:47.000000 reporters-db-3.2.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 01:07:52.308643 reporters-db-3.2.8/reporters_db/
--rw-r--r--   0 runner    (1001) docker     (121)     1420 2022-01-06 01:07:47.000000 reporters-db-3.2.8/reporters_db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 01:07:52.312643 reporters-db-3.2.8/reporters_db/data/
--rw-r--r--   0 runner    (1001) docker     (121)     5942 2022-01-06 01:07:47.000000 reporters-db-3.2.8/reporters_db/data/case_name_abbreviations.json
--rw-r--r--   0 runner    (1001) docker     (121)   265208 2022-01-06 01:07:47.000000 reporters-db-3.2.8/reporters_db/data/journals.json
--rw-r--r--   0 runner    (1001) docker     (121)   209204 2022-01-06 01:07:47.000000 reporters-db-3.2.8/reporters_db/data/laws.json
--rw-r--r--   0 runner    (1001) docker     (121)     4189 2022-01-06 01:07:47.000000 reporters-db-3.2.8/reporters_db/data/regexes.json
--rw-r--r--   0 runner    (1001) docker     (121)    93881 2022-01-06 01:07:47.000000 reporters-db-3.2.8/reporters_db/data/reporters.csv
--rw-r--r--   0 runner    (1001) docker     (121)   623024 2022-01-06 01:07:47.000000 reporters-db-3.2.8/reporters_db/data/reporters.json
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-01-06 01:07:47.000000 reporters-db-3.2.8/reporters_db/data/state_abbreviations.json
--rw-r--r--   0 runner    (1001) docker     (121)     2041 2022-01-06 01:07:47.000000 reporters-db-3.2.8/reporters_db/make_csv.py
--rw-r--r--   0 runner    (1001) docker     (121)     6087 2022-01-06 01:07:47.000000 reporters-db-3.2.8/reporters_db/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 01:07:52.308643 reporters-db-3.2.8/reporters_db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13657 2022-01-06 01:07:52.000000 reporters-db-3.2.8/reporters_db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-01-06 01:07:52.000000 reporters-db-3.2.8/reporters_db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-06 01:07:52.000000 reporters-db-3.2.8/reporters_db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-01-06 01:07:52.000000 reporters-db-3.2.8/reporters_db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-01-06 01:07:52.000000 reporters-db-3.2.8/reporters_db.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-01-06 01:07:47.000000 reporters-db-3.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-01-06 01:07:52.312643 reporters-db-3.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1874 2022-01-06 01:07:47.000000 reporters-db-3.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 17:51:20.979341 reporters-db-3.2.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1300 2022-01-06 17:51:14.000000 reporters-db-3.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2022-01-06 17:51:14.000000 reporters-db-3.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    13657 2022-01-06 17:51:20.979341 reporters-db-3.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10460 2022-01-06 17:51:14.000000 reporters-db-3.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2022-01-06 17:51:14.000000 reporters-db-3.2.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 17:51:20.975341 reporters-db-3.2.9/reporters_db/
+-rw-r--r--   0 runner    (1001) docker     (121)     1420 2022-01-06 17:51:14.000000 reporters-db-3.2.9/reporters_db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 17:51:20.979341 reporters-db-3.2.9/reporters_db/data/
+-rw-r--r--   0 runner    (1001) docker     (121)     5942 2022-01-06 17:51:14.000000 reporters-db-3.2.9/reporters_db/data/case_name_abbreviations.json
+-rw-r--r--   0 runner    (1001) docker     (121)   265208 2022-01-06 17:51:14.000000 reporters-db-3.2.9/reporters_db/data/journals.json
+-rw-r--r--   0 runner    (1001) docker     (121)   209204 2022-01-06 17:51:14.000000 reporters-db-3.2.9/reporters_db/data/laws.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4189 2022-01-06 17:51:14.000000 reporters-db-3.2.9/reporters_db/data/regexes.json
+-rw-r--r--   0 runner    (1001) docker     (121)    93881 2022-01-06 17:51:14.000000 reporters-db-3.2.9/reporters_db/data/reporters.csv
+-rw-r--r--   0 runner    (1001) docker     (121)   623499 2022-01-06 17:51:14.000000 reporters-db-3.2.9/reporters_db/data/reporters.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-01-06 17:51:14.000000 reporters-db-3.2.9/reporters_db/data/state_abbreviations.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2041 2022-01-06 17:51:14.000000 reporters-db-3.2.9/reporters_db/make_csv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6087 2022-01-06 17:51:14.000000 reporters-db-3.2.9/reporters_db/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 17:51:20.975341 reporters-db-3.2.9/reporters_db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    13657 2022-01-06 17:51:20.000000 reporters-db-3.2.9/reporters_db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      578 2022-01-06 17:51:20.000000 reporters-db-3.2.9/reporters_db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-06 17:51:20.000000 reporters-db-3.2.9/reporters_db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2022-01-06 17:51:20.000000 reporters-db-3.2.9/reporters_db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-01-06 17:51:20.000000 reporters-db-3.2.9/reporters_db.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2022-01-06 17:51:14.000000 reporters-db-3.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2022-01-06 17:51:20.979341 reporters-db-3.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1874 2022-01-06 17:51:14.000000 reporters-db-3.2.9/setup.py
```

### Comparing `reporters-db-3.2.8/LICENSE` & `reporters-db-3.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `reporters-db-3.2.8/PKG-INFO` & `reporters-db-3.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: reporters-db
-Version: 3.2.8
+Version: 3.2.9
 Summary: Database of Court Reporters
 Home-page: https://github.com/freelawproject/reporters-db
 Author: Mike Lissner
 Author-email: mike@free.law
 Maintainer: Mike Lissner
 Maintainer-email: mike@free.law
 License: BSD
```

### Comparing `reporters-db-3.2.8/README.rst` & `reporters-db-3.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `reporters-db-3.2.8/reporters_db/__init__.py` & `reporters-db-3.2.9/reporters_db/__init__.py`

 * *Files identical despite different names*

### Comparing `reporters-db-3.2.8/reporters_db/data/case_name_abbreviations.json` & `reporters-db-3.2.9/reporters_db/data/case_name_abbreviations.json`

 * *Files identical despite different names*

### Comparing `reporters-db-3.2.8/reporters_db/data/journals.json` & `reporters-db-3.2.9/reporters_db/data/journals.json`

 * *Files identical despite different names*

### Comparing `reporters-db-3.2.8/reporters_db/data/laws.json` & `reporters-db-3.2.9/reporters_db/data/laws.json`

 * *Files identical despite different names*

### Comparing `reporters-db-3.2.8/reporters_db/data/regexes.json` & `reporters-db-3.2.9/reporters_db/data/regexes.json`

 * *Files identical despite different names*

### Comparing `reporters-db-3.2.8/reporters_db/data/reporters.csv` & `reporters-db-3.2.9/reporters_db/data/reporters.csv`

 * *Files identical despite different names*

### Comparing `reporters-db-3.2.8/reporters_db/data/reporters.json` & `reporters-db-3.2.9/reporters_db/data/reporters.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999111374407583%*

 * *Differences: {"'Ark. App.'": "{0: {'editions': {'Ark. App.': {'regexes': ['(?P<volume>\\\\d{1,3}) $reporter "*

 * *                "$page']}}, 'examples': ['84 Ark. App. 412']}, 1: {'editions': {'Ark. App.': "*

 * *                "{'regexes': ['$volume_year $reporter $page']}}, 'examples': ['2013 Ark. App. "*

 * *                "5']}}",*

 * * "'Ark.'": "{1: {'editions': {'Ark.': {'regexes': ['$full_cite']}}}}"}*

```diff
@@ -1176,14 +1176,17 @@
             }
         },
         {
             "cite_type": "state",
             "editions": {
                 "Ark.": {
                     "end": "2008-12-31T00:00:00",
+                    "regexes": [
+                        "$full_cite"
+                    ],
                     "start": "1837-01-01T00:00:00"
                 }
             },
             "examples": [
                 "298 Ark. 1"
             ],
             "mlz_jurisdiction": [
@@ -1234,34 +1237,46 @@
     ],
     "Ark. App.": [
         {
             "cite_type": "state",
             "editions": {
                 "Ark. App.": {
                     "end": "2008-12-31T00:00:00",
+                    "regexes": [
+                        "(?P<volume>\\d{1,3}) $reporter $page"
+                    ],
                     "start": "1981-01-01T00:00:00"
                 }
             },
+            "examples": [
+                "84 Ark. App. 412"
+            ],
             "mlz_jurisdiction": [
                 "us:ar;appeals.court"
             ],
             "name": "Arkansas Appellate Reports",
             "variations": {
                 "Ak. App.": "Ark. App.",
                 "Ark.App.": "Ark. App."
             }
         },
         {
             "cite_type": "neutral",
             "editions": {
                 "Ark. App.": {
                     "end": null,
+                    "regexes": [
+                        "$volume_year $reporter $page"
+                    ],
                     "start": "2009-01-01T00:00:00"
                 }
             },
+            "examples": [
+                "2013 Ark. App. 5"
+            ],
             "mlz_jurisdiction": [
                 "us:ar;appeals.court"
             ],
             "name": "Arkansas Appellate Reports",
             "variations": {
                 "Ak. App.": "Ark. App.",
                 "Ark.App.": "Ark. App."
```

### Comparing `reporters-db-3.2.8/reporters_db/data/state_abbreviations.json` & `reporters-db-3.2.9/reporters_db/data/state_abbreviations.json`

 * *Files identical despite different names*

### Comparing `reporters-db-3.2.8/reporters_db/make_csv.py` & `reporters-db-3.2.9/reporters_db/make_csv.py`

 * *Files identical despite different names*

### Comparing `reporters-db-3.2.8/reporters_db/utils.py` & `reporters-db-3.2.9/reporters_db/utils.py`

 * *Files identical despite different names*

### Comparing `reporters-db-3.2.8/reporters_db.egg-info/PKG-INFO` & `reporters-db-3.2.9/reporters_db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: reporters-db
-Version: 3.2.8
+Version: 3.2.9
 Summary: Database of Court Reporters
 Home-page: https://github.com/freelawproject/reporters-db
 Author: Mike Lissner
 Author-email: mike@free.law
 Maintainer: Mike Lissner
 Maintainer-email: mike@free.law
 License: BSD
```

### Comparing `reporters-db-3.2.8/reporters_db.egg-info/SOURCES.txt` & `reporters-db-3.2.9/reporters_db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reporters-db-3.2.8/setup.py` & `reporters-db-3.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import codecs
 import os
 
 from setuptools import find_packages, setup
 
-VERSION = "3.2.8"
+VERSION = "3.2.9"
 AUTHOR = "Mike Lissner"
 EMAIL = "mike@free.law"
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 reqs_path = f"{HERE}/requirements.txt"
 with open(reqs_path) as reqs_file:
     reqs = reqs_file.read().splitlines()
```

