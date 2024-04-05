# Comparing `tmp/pyrp3-2.0.0.tar.gz` & `tmp/pyrp3-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrp3-2.0.0.tar", last modified: Tue Jan  2 13:17:21 2024, max compression
+gzip compressed data, was "pyrp3-2.0.1.tar", last modified: Fri Apr  5 12:51:31 2024, max compression
```

## Comparing `pyrp3-2.0.0.tar` & `pyrp3-2.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:17:21.170998 pyrp3-2.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:17:21.166998 pyrp3-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:17:21.170998 pyrp3-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-01-02 13:17:09.000000 pyrp3-2.0.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-01-02 13:17:09.000000 pyrp3-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-01-02 13:17:09.000000 pyrp3-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-01-02 13:17:09.000000 pyrp3-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-01-02 13:17:21.170998 pyrp3-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-01-02 13:17:09.000000 pyrp3-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:17:21.170998 pyrp3-2.0.0/monitor/
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-01-02 13:17:09.000000 pyrp3-2.0.0/monitor/monitor.c
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-01-02 13:17:09.000000 pyrp3-2.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:17:21.170998 pyrp3-2.0.0/pyrp3/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-01-02 13:17:09.000000 pyrp3-2.0.0/pyrp3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-02 13:17:09.000000 pyrp3-2.0.0/pyrp3/board.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-01-02 13:17:09.000000 pyrp3-2.0.0/pyrp3/client_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-01-02 13:17:09.000000 pyrp3-2.0.0/pyrp3/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    18272 2024-01-02 13:17:09.000000 pyrp3-2.0.0/pyrp3/instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-01-02 13:17:09.000000 pyrp3-2.0.0/pyrp3/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-01-02 13:17:09.000000 pyrp3-2.0.0/pyrp3/pc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-01-02 13:17:09.000000 pyrp3-2.0.0/pyrp3/raw_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-01-02 13:17:09.000000 pyrp3-2.0.0/pyrp3/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:17:21.170998 pyrp3-2.0.0/pyrp3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-01-02 13:17:21.000000 pyrp3-2.0.0/pyrp3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-01-02 13:17:21.000000 pyrp3-2.0.0/pyrp3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-02 13:17:21.000000 pyrp3-2.0.0/pyrp3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-01-02 13:17:21.000000 pyrp3-2.0.0/pyrp3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-02 13:17:21.000000 pyrp3-2.0.0/pyrp3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-02 13:17:21.170998 pyrp3-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-02 13:17:09.000000 pyrp3-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:17:21.170998 pyrp3-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-02 13:17:09.000000 pyrp3-2.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-01-02 13:17:09.000000 pyrp3-2.0.0/tests/test_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:51:31.792732 pyrp3-2.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:51:31.788732 pyrp3-2.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:51:31.788732 pyrp3-2.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-05 12:51:23.000000 pyrp3-2.0.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-05 12:51:23.000000 pyrp3-2.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-05 12:51:23.000000 pyrp3-2.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-05 12:51:23.000000 pyrp3-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-04-05 12:51:31.792732 pyrp3-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-05 12:51:23.000000 pyrp3-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:51:31.788732 pyrp3-2.0.1/monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-04-05 12:51:23.000000 pyrp3-2.0.1/monitor/monitor.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-05 12:51:23.000000 pyrp3-2.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:51:31.788732 pyrp3-2.0.1/pyrp3/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-05 12:51:23.000000 pyrp3-2.0.1/pyrp3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-05 12:51:23.000000 pyrp3-2.0.1/pyrp3/board.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-05 12:51:23.000000 pyrp3-2.0.1/pyrp3/client_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-05 12:51:23.000000 pyrp3-2.0.1/pyrp3/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18250 2024-04-05 12:51:23.000000 pyrp3-2.0.1/pyrp3/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-05 12:51:23.000000 pyrp3-2.0.1/pyrp3/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-05 12:51:23.000000 pyrp3-2.0.1/pyrp3/pc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-05 12:51:23.000000 pyrp3-2.0.1/pyrp3/raw_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-05 12:51:23.000000 pyrp3-2.0.1/pyrp3/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:51:31.788732 pyrp3-2.0.1/pyrp3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-04-05 12:51:31.000000 pyrp3-2.0.1/pyrp3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-05 12:51:31.000000 pyrp3-2.0.1/pyrp3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 12:51:31.000000 pyrp3-2.0.1/pyrp3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-05 12:51:31.000000 pyrp3-2.0.1/pyrp3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 12:51:31.000000 pyrp3-2.0.1/pyrp3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 12:51:31.792732 pyrp3-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-05 12:51:23.000000 pyrp3-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:51:31.788732 pyrp3-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:51:23.000000 pyrp3-2.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-05 12:51:23.000000 pyrp3-2.0.1/tests/test_enum.py
```

### Comparing `pyrp3-2.0.0/.github/workflows/publish.yml` & `pyrp3-2.0.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pyrp3-2.0.0/.gitignore` & `pyrp3-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyrp3-2.0.0/LICENSE` & `pyrp3-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrp3-2.0.0/PKG-INFO` & `pyrp3-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrp3
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python utilities for RedPitaya
 Author-email: Pierre Cladé <pierre.clade@upmc.fr>, Benjamin Wiegand <benjamin.wiegand@physik.hu-berlin.de>, Bastian Leykauf <leykauf@physik.hu-berlin.de>, Doron Behar <doron.behar@gmail.com>
 Maintainer-email: Bastian Leykauf <leykauf@physik.hu-berlin.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2016, Pierre Cladé  All rights reserved.
         Copyright (c) 2018-2019, Benjamin Wiegand  All rights reserved.
@@ -29,18 +29,18 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: cached_property>=1.5.2
+Requires-Dist: cached_property<2.0,>=1.5.2
 Requires-Dist: myhdl>=0.11
-Requires-Dist: numpy>=1.21.5
-Requires-Dist: rpyc<6.0,>=5.0
+Requires-Dist: numpy<2.0,>=1.21.5
+Requires-Dist: rpyc<7.0,>=6.0.0
 Provides-Extra: dev
 Requires-Dist: black>=22.8.0; extra == "dev"
 Requires-Dist: pre-commit>=2.20.0; extra == "dev"
 Requires-Dist: flake8>=5.0.4; extra == "dev"
 Requires-Dist: isort>=5.10.1; extra == "dev"
 Requires-Dist: flake8-pyproject>=1.2.3; extra == "dev"
 Requires-Dist: setuptools_scm>=6.2; extra == "dev"
```

### Comparing `pyrp3-2.0.0/README.md` & `pyrp3-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyrp3-2.0.0/monitor/monitor.c` & `pyrp3-2.0.1/monitor/monitor.c`

 * *Files identical despite different names*

### Comparing `pyrp3-2.0.0/pyproject.toml` & `pyrp3-2.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 maintainers = [
     { name = "Bastian Leykauf", email = "leykauf@physik.hu-berlin.de" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
-    "cached_property>=1.5.2",
+    "cached_property>=1.5.2,<2.0",
     "myhdl>=0.11",
-    "numpy>=1.21.5",
-    "rpyc>=5.0,<6.0",
+    "numpy>=1.21.5,<2.0",
+    "rpyc>=6.0.0,<7.0",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License",
     "Operating System :: POSIX :: Linux",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Education",
```

### Comparing `pyrp3-2.0.0/pyrp3/client_memory.py` & `pyrp3-2.0.1/pyrp3/client_memory.py`

 * *Files identical despite different names*

### Comparing `pyrp3-2.0.0/pyrp3/enum.py` & `pyrp3-2.0.1/pyrp3/enum.py`

 * *Files identical despite different names*

### Comparing `pyrp3-2.0.0/pyrp3/instrument.py` & `pyrp3-2.0.1/pyrp3/instrument.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,17 +19,15 @@
 
 
 class SignedInteger:
     def __init__(self, size):
         self.size = size
 
     def to_python(self, val):
-        return int(
-            intbv(val & (2**self.size - 1), min=0, max=2**self.size).signed()
-        )
+        return int(intbv(val & (2**self.size - 1), min=0, max=2**self.size).signed())
 
     def to_binary(self, val):
         return intbv(val, min=-(2 ** (self.size - 1)), max=2 ** (self.size - 1))[
             self.size :
         ]._val
```

### Comparing `pyrp3-2.0.0/pyrp3/memory.py` & `pyrp3-2.0.1/pyrp3/memory.py`

 * *Files identical despite different names*

### Comparing `pyrp3-2.0.0/pyrp3/raw_memory.py` & `pyrp3-2.0.1/pyrp3/raw_memory.py`

 * *Files identical despite different names*

### Comparing `pyrp3-2.0.0/pyrp3/service.py` & `pyrp3-2.0.1/pyrp3/service.py`

 * *Files identical despite different names*

### Comparing `pyrp3-2.0.0/pyrp3.egg-info/PKG-INFO` & `pyrp3-2.0.1/pyrp3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrp3
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python utilities for RedPitaya
 Author-email: Pierre Cladé <pierre.clade@upmc.fr>, Benjamin Wiegand <benjamin.wiegand@physik.hu-berlin.de>, Bastian Leykauf <leykauf@physik.hu-berlin.de>, Doron Behar <doron.behar@gmail.com>
 Maintainer-email: Bastian Leykauf <leykauf@physik.hu-berlin.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2016, Pierre Cladé  All rights reserved.
         Copyright (c) 2018-2019, Benjamin Wiegand  All rights reserved.
@@ -29,18 +29,18 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: cached_property>=1.5.2
+Requires-Dist: cached_property<2.0,>=1.5.2
 Requires-Dist: myhdl>=0.11
-Requires-Dist: numpy>=1.21.5
-Requires-Dist: rpyc<6.0,>=5.0
+Requires-Dist: numpy<2.0,>=1.21.5
+Requires-Dist: rpyc<7.0,>=6.0.0
 Provides-Extra: dev
 Requires-Dist: black>=22.8.0; extra == "dev"
 Requires-Dist: pre-commit>=2.20.0; extra == "dev"
 Requires-Dist: flake8>=5.0.4; extra == "dev"
 Requires-Dist: isort>=5.10.1; extra == "dev"
 Requires-Dist: flake8-pyproject>=1.2.3; extra == "dev"
 Requires-Dist: setuptools_scm>=6.2; extra == "dev"
```

### Comparing `pyrp3-2.0.0/tests/test_enum.py` & `pyrp3-2.0.1/tests/test_enum.py`

 * *Files identical despite different names*

