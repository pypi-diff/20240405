# Comparing `tmp/qnngds-1.0.1.tar.gz` & `tmp/qnngds-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qnngds-1.0.1.tar", last modified: Thu Apr  4 21:36:38 2024, max compression
+gzip compressed data, was "qnngds-1.0.2.tar", last modified: Fri Apr  5 18:39:27 2024, max compression
```

## Comparing `qnngds-1.0.1.tar` & `qnngds-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2024-04-04 21:36:36.131832 qnngds-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1199 2024-04-04 21:36:36.131832 qnngds-1.0.1/README.md
--rw-r--r--   0        0        0     1108 2024-04-04 21:36:38.987835 qnngds-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      111 2024-04-04 21:36:36.135832 qnngds-1.0.1/src/qnngds/__init__.py
--rw-r--r--   0        0        0    10600 2024-04-04 21:36:36.135832 qnngds-1.0.1/src/qnngds/circuits.py
--rw-r--r--   0        0        0    51283 2024-04-04 21:36:36.139832 qnngds-1.0.1/src/qnngds/design.py
--rw-r--r--   0        0        0     8019 2024-04-04 21:36:36.139832 qnngds-1.0.1/src/qnngds/devices.py
--rw-r--r--   0        0        0     8244 2024-04-04 21:36:36.139832 qnngds-1.0.1/src/qnngds/geometries.py
--rw-r--r--   0        0        0    21375 2024-04-04 21:36:36.139832 qnngds-1.0.1/src/qnngds/utilities.py
--rw-r--r--   0        0        0     3344 1970-01-01 00:00:00.000000 qnngds-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-05 18:39:25.130454 qnngds-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     1129 2024-04-05 18:39:25.130454 qnngds-1.0.2/README.md
+-rw-r--r--   0        0        0     1161 2024-04-05 18:39:27.890477 qnngds-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      111 2024-04-05 18:39:25.138454 qnngds-1.0.2/src/qnngds/__init__.py
+-rw-r--r--   0        0        0    10600 2024-04-05 18:39:25.138454 qnngds-1.0.2/src/qnngds/circuits.py
+-rw-r--r--   0        0        0    51283 2024-04-05 18:39:25.138454 qnngds-1.0.2/src/qnngds/design.py
+-rw-r--r--   0        0        0     8019 2024-04-05 18:39:25.138454 qnngds-1.0.2/src/qnngds/devices.py
+-rw-r--r--   0        0        0     8244 2024-04-05 18:39:25.138454 qnngds-1.0.2/src/qnngds/geometries.py
+-rw-r--r--   0        0        0    21375 2024-04-05 18:39:25.138454 qnngds-1.0.2/src/qnngds/utilities.py
+-rw-r--r--   0        0        0     3301 1970-01-01 00:00:00.000000 qnngds-1.0.2/PKG-INFO
```

### Comparing `qnngds-1.0.1/LICENSE.txt` & `qnngds-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qnngds-1.0.1/README.md` & `qnngds-1.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -19,12 +19,11 @@
 - [scipy](https://pypi.org/project/scipy/)
 
 ## License
 This project is licensed under the MIT License - see the LICENSE.txt file for details
 
 ## [Documentation](https://qnngds.readthedocs.io/en/latest/)
 - [API](https://qnngds.readthedocs.io/en/latest/api.html)
-- [Libraries](https://qnngds.readthedocs.io/en/latest/libraries.html)
 - [Tutorials](https://qnngds.readthedocs.io/en/latest/tutorials.html)
 
 ## How to contribute
 - [Developer's documentation](https://qnngds-dev.readthedocs.io/en/latest)
```

### Comparing `qnngds-1.0.1/pyproject.toml` & `qnngds-1.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "qnngds"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
     { name = "A. Jacquillat", email = "audrey01@mit.edu" },
     { name = "A. Jacquillat", email = "audrey.jacquillat@gmail.com" },
+    { name = "R. Foster", email = "reedf@mit.edu" },
 ]
 maintainers = [
     { name = "A. Jacquillat", email = "audrey01@mit.edu" },
 ]
 description = "The QNN library for creating gds files"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `qnngds-1.0.1/src/qnngds/circuits.py` & `qnngds-1.0.2/src/qnngds/circuits.py`

 * *Files identical despite different names*

### Comparing `qnngds-1.0.1/src/qnngds/design.py` & `qnngds-1.0.2/src/qnngds/design.py`

 * *Files identical despite different names*

### Comparing `qnngds-1.0.1/src/qnngds/devices.py` & `qnngds-1.0.2/src/qnngds/devices.py`

 * *Files identical despite different names*

### Comparing `qnngds-1.0.1/src/qnngds/geometries.py` & `qnngds-1.0.2/src/qnngds/geometries.py`

 * *Files identical despite different names*

### Comparing `qnngds-1.0.1/src/qnngds/utilities.py` & `qnngds-1.0.2/src/qnngds/utilities.py`

 * *Files identical despite different names*

### Comparing `qnngds-1.0.1/PKG-INFO` & `qnngds-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: qnngds
-Version: 1.0.1
+Version: 1.0.2
 Summary: The QNN library for creating gds files
 Keywords: phidl nanowire_electronics nanofabrication gds
-Author-Email: A. Jacquillat <audrey01@mit.edu>, A. Jacquillat <audrey.jacquillat@gmail.com>
+Author-Email: A. Jacquillat <audrey01@mit.edu>, A. Jacquillat <audrey.jacquillat@gmail.com>, R. Foster <reedf@mit.edu>
 Maintainer-Email: A. Jacquillat <audrey01@mit.edu>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
         use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
@@ -59,12 +59,11 @@
 - [scipy](https://pypi.org/project/scipy/)
 
 ## License
 This project is licensed under the MIT License - see the LICENSE.txt file for details
 
 ## [Documentation](https://qnngds.readthedocs.io/en/latest/)
 - [API](https://qnngds.readthedocs.io/en/latest/api.html)
-- [Libraries](https://qnngds.readthedocs.io/en/latest/libraries.html)
 - [Tutorials](https://qnngds.readthedocs.io/en/latest/tutorials.html)
 
 ## How to contribute
 - [Developer's documentation](https://qnngds-dev.readthedocs.io/en/latest)
```

