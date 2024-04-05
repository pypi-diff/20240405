# Comparing `tmp/linien-common-2.0.0rc1.tar.gz` & `tmp/linien-common-2.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien-common-2.0.0rc1.tar", last modified: Fri Apr  5 13:10:23 2024, max compression
+gzip compressed data, was "linien-common-2.0.0rc2.tar", last modified: Fri Apr  5 13:46:34 2024, max compression
```

## Comparing `linien-common-2.0.0rc1.tar` & `linien-common-2.0.0rc2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:10:23.052651 linien-common-2.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-05 13:10:23.052651 linien-common-2.0.0rc1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:10:23.052651 linien-common-2.0.0rc1/linien_common/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-05 13:10:16.000000 linien-common-2.0.0rc1/linien_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9767 2024-04-05 13:10:16.000000 linien-common-2.0.0rc1/linien_common/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-05 13:10:16.000000 linien-common-2.0.0rc1/linien_common/communication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-05 13:10:16.000000 linien-common-2.0.0rc1/linien_common/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-05 13:10:16.000000 linien-common-2.0.0rc1/linien_common/influxdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:10:23.052651 linien-common-2.0.0rc1/linien_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-05 13:10:23.000000 linien-common-2.0.0rc1/linien_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-05 13:10:23.000000 linien-common-2.0.0rc1/linien_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:10:23.000000 linien-common-2.0.0rc1/linien_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-05 13:10:23.000000 linien-common-2.0.0rc1/linien_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 13:10:23.000000 linien-common-2.0.0rc1/linien_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-05 13:10:16.000000 linien-common-2.0.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:10:23.052651 linien-common-2.0.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:34.871191 linien-common-2.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-05 13:46:34.871191 linien-common-2.0.0rc2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:34.867191 linien-common-2.0.0rc2/linien_common/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-05 13:46:25.000000 linien-common-2.0.0rc2/linien_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9767 2024-04-05 13:46:25.000000 linien-common-2.0.0rc2/linien_common/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-05 13:46:25.000000 linien-common-2.0.0rc2/linien_common/communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-05 13:46:25.000000 linien-common-2.0.0rc2/linien_common/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-05 13:46:25.000000 linien-common-2.0.0rc2/linien_common/influxdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:34.867191 linien-common-2.0.0rc2/linien_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-05 13:46:34.000000 linien-common-2.0.0rc2/linien_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-05 13:46:34.000000 linien-common-2.0.0rc2/linien_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:46:34.000000 linien-common-2.0.0rc2/linien_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-05 13:46:34.000000 linien-common-2.0.0rc2/linien_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 13:46:34.000000 linien-common-2.0.0rc2/linien_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-05 13:46:25.000000 linien-common-2.0.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:46:34.871191 linien-common-2.0.0rc2/setup.cfg
```

### Comparing `linien-common-2.0.0rc1/PKG-INFO` & `linien-common-2.0.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: linien-common
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: Shared components of the Linien spectroscopy lock application.
 Author-email: Benjamin Wiegand <benjamin.wiegand@physik.hu-berlin.de>, Bastian Leykauf <leykauf@physik.hu-berlin.de>, Robert Jördens <rj@quartiq.de>, Christian Freier <christian.freier@gmail.com>, Doron Behar <doron.behar@gmail.com>
 Maintainer-email: Bastian Leykauf <leykauf@physik.hu-berlin.de>
 Project-URL: Homepage, https://github.com/linien-org/linien
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: appdirs<2.0,>=1.4.4
-Requires-Dist: fire>=0.5.0
 Requires-Dist: importlib_metadata<5.0,>=2.1.3
 Requires-Dist: numpy<2.0,>=1.21.5
 Requires-Dist: rpyc<7.0,>=6.0
 Requires-Dist: scipy<2.0,>=1.8.0
 Provides-Extra: dev
 Requires-Dist: black>=22.8.0; extra == "dev"
 Requires-Dist: pre-commit>=2.20.0; extra == "dev"
```

### Comparing `linien-common-2.0.0rc1/linien_common/__init__.py` & `linien-common-2.0.0rc2/linien_common/__init__.py`

 * *Files identical despite different names*

### Comparing `linien-common-2.0.0rc1/linien_common/common.py` & `linien-common-2.0.0rc2/linien_common/common.py`

 * *Files identical despite different names*

### Comparing `linien-common-2.0.0rc1/linien_common/communication.py` & `linien-common-2.0.0rc2/linien_common/communication.py`

 * *Files identical despite different names*

### Comparing `linien-common-2.0.0rc1/linien_common/config.py` & `linien-common-2.0.0rc2/linien_common/config.py`

 * *Files identical despite different names*

### Comparing `linien-common-2.0.0rc1/linien_common/influxdb.py` & `linien-common-2.0.0rc2/linien_common/influxdb.py`

 * *Files identical despite different names*

### Comparing `linien-common-2.0.0rc1/linien_common.egg-info/PKG-INFO` & `linien-common-2.0.0rc2/linien_common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: linien-common
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: Shared components of the Linien spectroscopy lock application.
 Author-email: Benjamin Wiegand <benjamin.wiegand@physik.hu-berlin.de>, Bastian Leykauf <leykauf@physik.hu-berlin.de>, Robert Jördens <rj@quartiq.de>, Christian Freier <christian.freier@gmail.com>, Doron Behar <doron.behar@gmail.com>
 Maintainer-email: Bastian Leykauf <leykauf@physik.hu-berlin.de>
 Project-URL: Homepage, https://github.com/linien-org/linien
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: appdirs<2.0,>=1.4.4
-Requires-Dist: fire>=0.5.0
 Requires-Dist: importlib_metadata<5.0,>=2.1.3
 Requires-Dist: numpy<2.0,>=1.21.5
 Requires-Dist: rpyc<7.0,>=6.0
 Requires-Dist: scipy<2.0,>=1.8.0
 Provides-Extra: dev
 Requires-Dist: black>=22.8.0; extra == "dev"
 Requires-Dist: pre-commit>=2.20.0; extra == "dev"
```

### Comparing `linien-common-2.0.0rc1/pyproject.toml` & `linien-common-2.0.0rc2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "linien-common"
-version = "2.0.0rc1"
+version = "2.0.0rc2"
 authors = [
     { name = "Benjamin Wiegand", email = "benjamin.wiegand@physik.hu-berlin.de" },
     { name = "Bastian Leykauf", email = "leykauf@physik.hu-berlin.de" },
     { name = "Robert Jördens", email = "rj@quartiq.de" },
     { name = "Christian Freier", email = "christian.freier@gmail.com" },
     { name = "Doron Behar", email = "doron.behar@gmail.com" },
 ]
@@ -20,15 +20,14 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.8"
 dependencies = [
     "appdirs>=1.4.4,<2.0",
-    "fire>=0.5.0",
     "importlib_metadata>=2.1.3,<5.0",
     "numpy>=1.21.5,<2.0",
     "rpyc>=6.0,<7.0",
     "scipy>=1.8.0,<2.0",
 ]
 
 [project.optional-dependencies]
```

