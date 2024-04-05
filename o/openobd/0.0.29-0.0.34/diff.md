# Comparing `tmp/openobd-0.0.29.tar.gz` & `tmp/openobd-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openobd-0.0.29.tar", last modified: Wed Mar  6 12:48:10 2024, max compression
+gzip compressed data, was "openobd-0.0.34.tar", last modified: Fri Apr  5 08:12:33 2024, max compression
```

## Comparing `openobd-0.0.29.tar` & `openobd-0.0.34.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 12:48:10.603656 openobd-0.0.29/
--rw-r--r--   0 root         (0) root         (0)     1066 2024-03-06 12:48:07.000000 openobd-0.0.29/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2344 2024-03-06 12:48:10.602656 openobd-0.0.29/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      195 2024-03-06 12:48:07.000000 openobd-0.0.29/README.md
--rw-r--r--   0 root         (0) root         (0)     1743 2024-03-06 12:48:07.000000 openobd-0.0.29/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-06 12:48:10.603656 openobd-0.0.29/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 12:48:10.599655 openobd-0.0.29/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 12:48:10.600655 openobd-0.0.29/src/openobd/
--rw-r--r--   0 root         (0) root         (0)     2173 2024-03-06 12:48:07.000000 openobd-0.0.29/src/openobd/__init__.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-06 12:48:07.000000 openobd-0.0.29/src/openobd/_metadata.py
--rwxr-xr-x   0 root         (0) root         (0)     3619 2024-03-06 12:48:07.000000 openobd-0.0.29/src/openobd/openobdclient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 12:48:10.602656 openobd-0.0.29/src/openobd.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2344 2024-03-06 12:48:10.000000 openobd-0.0.29/src/openobd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      284 2024-03-06 12:48:10.000000 openobd-0.0.29/src/openobd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-06 12:48:10.000000 openobd-0.0.29/src/openobd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-06 12:48:10.000000 openobd-0.0.29/src/openobd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-03-06 12:48:10.000000 openobd-0.0.29/src/openobd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 08:12:33.631628 openobd-0.0.34/
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-04-05 08:12:30.000000 openobd-0.0.34/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2415 2024-04-05 08:12:33.631628 openobd-0.0.34/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      265 2024-04-05 08:12:30.000000 openobd-0.0.34/README.md
+-rw-r--r--   0 root         (0) root         (0)     1744 2024-04-05 08:12:30.000000 openobd-0.0.34/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 08:12:33.631628 openobd-0.0.34/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 08:12:33.627628 openobd-0.0.34/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 08:12:33.629628 openobd-0.0.34/src/openobd/
+-rw-r--r--   0 root         (0) root         (0)     3410 2024-04-05 08:12:30.000000 openobd-0.0.34/src/openobd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-05 08:12:30.000000 openobd-0.0.34/src/openobd/_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     3067 2024-04-05 08:12:30.000000 openobd-0.0.34/src/openobd/openobdapi.py
+-rwxr-xr-x   0 root         (0) root         (0)     5194 2024-04-05 08:12:30.000000 openobd-0.0.34/src/openobd/openobdclient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 08:12:33.630628 openobd-0.0.34/src/openobd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2415 2024-04-05 08:12:33.000000 openobd-0.0.34/src/openobd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      310 2024-04-05 08:12:33.000000 openobd-0.0.34/src/openobd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 08:12:33.000000 openobd-0.0.34/src/openobd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-05 08:12:33.000000 openobd-0.0.34/src/openobd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-05 08:12:33.000000 openobd-0.0.34/src/openobd.egg-info/top_level.txt
```

### Comparing `openobd-0.0.29/LICENSE` & `openobd-0.0.34/LICENSE`

 * *Files identical despite different names*

### Comparing `openobd-0.0.29/PKG-INFO` & `openobd-0.0.34/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openobd
-Version: 0.0.29
+Version: 0.0.34
 Summary: Jifeline Networks OpenOBD Python Client Library
 Author-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 Maintainer-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 License: Copyright (c) 2024 Jifeline Networks B.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -28,22 +28,23 @@
 Keywords: OpenOBD,Protocol,gRPC,Jifeline,Remote,Diagnostics,OBD,On-board,Automotive,Car,Vehicle,CAN,K-line,DoIP
 Platform: any
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Communications
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openobd-protocol==0.0.29
+Requires-Dist: openobd-protocol==0.0.34
 
 OpenOBD Client by Jifeline Networks for Python 3
 
 Release notes:
 
- - 0.0.29 : First openobd package that uses openobd-protocol
+ - 0.0.30 : First openobd package that uses openobd-protocol
+ - 0.0.34 : openobd package supporting user interface functionality  
 
 
 ---------------------------------------------------------------
```

### Comparing `openobd-0.0.29/pyproject.toml` & `openobd-0.0.34/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openobd"
 description = "Jifeline Networks OpenOBD Python Client Library"
-requires-python = ">=3.8"
+requires-python = ">=3.11"
 dependencies = [
-    "openobd-protocol==0.0.29"
+    "openobd-protocol==0.0.34"
 ]
 
 license = {file = "LICENSE"}
 dynamic = ["version"]
 readme = "README.md"
 
 authors = [
```

### Comparing `openobd-0.0.29/src/openobd.egg-info/PKG-INFO` & `openobd-0.0.34/src/openobd.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openobd
-Version: 0.0.29
+Version: 0.0.34
 Summary: Jifeline Networks OpenOBD Python Client Library
 Author-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 Maintainer-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 License: Copyright (c) 2024 Jifeline Networks B.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -28,22 +28,23 @@
 Keywords: OpenOBD,Protocol,gRPC,Jifeline,Remote,Diagnostics,OBD,On-board,Automotive,Car,Vehicle,CAN,K-line,DoIP
 Platform: any
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Communications
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openobd-protocol==0.0.29
+Requires-Dist: openobd-protocol==0.0.34
 
 OpenOBD Client by Jifeline Networks for Python 3
 
 Release notes:
 
- - 0.0.29 : First openobd package that uses openobd-protocol
+ - 0.0.30 : First openobd package that uses openobd-protocol
+ - 0.0.34 : openobd package supporting user interface functionality  
 
 
 ---------------------------------------------------------------
```

