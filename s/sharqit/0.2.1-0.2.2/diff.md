# Comparing `tmp/sharqit-0.2.1.tar.gz` & `tmp/sharqit-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharqit-0.2.1.tar", last modified: Thu Mar 28 14:37:23 2024, max compression
+gzip compressed data, was "sharqit-0.2.2.tar", last modified: Fri Apr  5 13:15:59 2024, max compression
```

## Comparing `sharqit-0.2.1.tar` & `sharqit-0.2.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 nakagawa  (1000) nakagawa  (1000)        0 2024-03-28 14:37:23.186356 sharqit-0.2.1/
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     1572 2024-03-27 12:57:53.000000 sharqit-0.2.1/CMakeLists.txt
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     1067 2024-02-17 09:27:38.000000 sharqit-0.2.1/LICENSE
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)       79 2024-03-14 14:57:12.000000 sharqit-0.2.1/MANIFEST.in
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      411 2024-03-28 14:37:23.176356 sharqit-0.2.1/PKG-INFO
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     4843 2024-03-26 14:24:02.000000 sharqit-0.2.1/README.md
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)       38 2024-03-28 14:37:23.186356 sharqit-0.2.1/setup.cfg
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     1865 2024-03-26 14:24:02.000000 sharqit-0.2.1/setup.py
-drwxr-xr-x   0 nakagawa  (1000) nakagawa  (1000)        0 2024-03-28 14:37:23.176356 sharqit-0.2.1/sharqit/
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)       92 2024-03-26 14:24:02.000000 sharqit-0.2.1/sharqit/__init__.py
-drwxr-xr-x   0 nakagawa  (1000) nakagawa  (1000)        0 2024-03-28 14:37:23.176356 sharqit-0.2.1/sharqit/cpp/
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     1506 2024-03-14 14:57:12.000000 sharqit-0.2.1/sharqit/cpp/CMakeLists.txt
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)   112731 2024-03-14 14:57:12.000000 sharqit-0.2.1/sharqit/cpp/Doxyfile
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     2114 2024-03-17 23:24:30.000000 sharqit-0.2.1/sharqit/cpp/Makefile
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    26307 2024-03-10 15:49:56.000000 sharqit-0.2.1/sharqit/cpp/TAGS
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     2430 2024-03-14 14:57:12.000000 sharqit-0.2.1/sharqit/cpp/binary_matrix.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     5970 2024-03-14 14:57:12.000000 sharqit-0.2.1/sharqit/cpp/binary_matrix.h
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    14930 2024-03-14 14:57:12.000000 sharqit-0.2.1/sharqit/cpp/dag.h
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    20976 2024-03-14 14:57:12.000000 sharqit-0.2.1/sharqit/cpp/dagcirc.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      406 2024-03-14 14:57:12.000000 sharqit-0.2.1/sharqit/cpp/dagedge.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      317 2024-03-14 14:57:12.000000 sharqit-0.2.1/sharqit/cpp/dagnode.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    11949 2024-03-14 14:57:12.000000 sharqit-0.2.1/sharqit/cpp/extract_qcirc.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      357 2024-03-14 14:57:12.000000 sharqit-0.2.1/sharqit/cpp/fraction.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     8343 2024-03-14 14:57:12.000000 sharqit-0.2.1/sharqit/cpp/fraction.h
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     4047 2024-03-14 14:57:12.000000 sharqit-0.2.1/sharqit/cpp/linear_map.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     4528 2024-03-14 14:57:12.000000 sharqit-0.2.1/sharqit/cpp/linear_map.h
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     8745 2024-03-14 14:57:12.000000 sharqit-0.2.1/sharqit/cpp/merge_rotation.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     5617 2024-03-27 12:57:45.000000 sharqit-0.2.1/sharqit/cpp/nb_sharqit.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     5438 2024-03-14 14:57:12.000000 sharqit-0.2.1/sharqit/cpp/optimizer.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     4189 2024-03-14 14:57:12.000000 sharqit-0.2.1/sharqit/cpp/optimizer.h
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     2487 2024-03-14 14:57:12.000000 sharqit-0.2.1/sharqit/cpp/phase.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     4239 2024-03-14 14:57:12.000000 sharqit-0.2.1/sharqit/cpp/phase.h
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     2342 2024-03-14 14:57:12.000000 sharqit-0.2.1/sharqit/cpp/propagate_pauli_x.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    21119 2024-03-26 14:24:02.000000 sharqit-0.2.1/sharqit/cpp/qcirc.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    24657 2024-03-26 14:24:02.000000 sharqit-0.2.1/sharqit/cpp/qcirc.h
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    12727 2024-03-23 12:44:15.000000 sharqit-0.2.1/sharqit/cpp/qgate.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    10012 2024-03-26 14:24:02.000000 sharqit-0.2.1/sharqit/cpp/qgate.h
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     7660 2024-03-14 23:07:51.000000 sharqit-0.2.1/sharqit/cpp/sharqit.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      385 2024-03-26 14:24:02.000000 sharqit-0.2.1/sharqit/cpp/sharqit.h
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    28969 2024-03-14 14:57:12.000000 sharqit-0.2.1/sharqit/cpp/simplify.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     2168 2024-03-14 14:57:12.000000 sharqit-0.2.1/sharqit/cpp/util.h
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    28058 2024-03-14 14:57:12.000000 sharqit-0.2.1/sharqit/cpp/zx.h
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    17166 2024-03-14 14:57:12.000000 sharqit-0.2.1/sharqit/cpp/zxdiagram.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      539 2024-03-14 14:57:12.000000 sharqit-0.2.1/sharqit/cpp/zxnode.cpp
-drwxr-xr-x   0 nakagawa  (1000) nakagawa  (1000)        0 2024-03-28 14:37:23.176356 sharqit-0.2.1/sharqit.egg-info/
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      411 2024-03-28 14:37:23.000000 sharqit-0.2.1/sharqit.egg-info/PKG-INFO
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     1015 2024-03-28 14:37:23.000000 sharqit-0.2.1/sharqit.egg-info/SOURCES.txt
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)        1 2024-03-28 14:37:23.000000 sharqit-0.2.1/sharqit.egg-info/dependency_links.txt
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)       16 2024-03-28 14:37:23.000000 sharqit-0.2.1/sharqit.egg-info/requires.txt
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)       25 2024-03-28 14:37:23.000000 sharqit-0.2.1/sharqit.egg-info/top_level.txt
+drwxr-xr-x   0 nakagawa  (1000) nakagawa  (1000)        0 2024-04-05 13:15:59.769859 sharqit-0.2.2/
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     1572 2024-03-27 12:57:53.000000 sharqit-0.2.2/CMakeLists.txt
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     1067 2024-02-17 09:27:38.000000 sharqit-0.2.2/LICENSE
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)       79 2024-03-14 14:57:12.000000 sharqit-0.2.2/MANIFEST.in
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      437 2024-04-05 13:15:59.769859 sharqit-0.2.2/PKG-INFO
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     4981 2024-04-05 12:58:50.000000 sharqit-0.2.2/README.md
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)       38 2024-04-05 13:15:59.769859 sharqit-0.2.2/setup.cfg
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     1910 2024-04-05 12:58:50.000000 sharqit-0.2.2/setup.py
+drwxr-xr-x   0 nakagawa  (1000) nakagawa  (1000)        0 2024-04-05 13:15:59.769859 sharqit-0.2.2/sharqit/
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)       92 2024-03-26 14:24:02.000000 sharqit-0.2.2/sharqit/__init__.py
+drwxr-xr-x   0 nakagawa  (1000) nakagawa  (1000)        0 2024-04-05 13:15:59.769859 sharqit-0.2.2/sharqit/cpp/
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     1506 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/CMakeLists.txt
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)   112731 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/Doxyfile
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     2114 2024-03-17 23:24:30.000000 sharqit-0.2.2/sharqit/cpp/Makefile
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    26788 2024-03-31 23:29:48.000000 sharqit-0.2.2/sharqit/cpp/TAGS
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     2430 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/binary_matrix.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     5970 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/binary_matrix.h
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    14930 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/dag.h
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    20976 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/dagcirc.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      406 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/dagedge.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      317 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/dagnode.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    11949 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/extract_qcirc.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      357 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/fraction.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     8343 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/fraction.h
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     4047 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/linear_map.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     4528 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/linear_map.h
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     8745 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/merge_rotation.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    10169 2024-04-05 12:58:50.000000 sharqit-0.2.2/sharqit/cpp/nb_sharqit.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     5118 2024-04-05 12:58:50.000000 sharqit-0.2.2/sharqit/cpp/optimizer.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     3792 2024-04-05 12:58:50.000000 sharqit-0.2.2/sharqit/cpp/optimizer.h
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     2487 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/phase.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     4239 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/phase.h
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     2342 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/propagate_pauli_x.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    28756 2024-04-05 12:58:50.000000 sharqit-0.2.2/sharqit/cpp/qcirc.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    27013 2024-04-05 12:58:50.000000 sharqit-0.2.2/sharqit/cpp/qcirc.h
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    14516 2024-04-05 12:58:50.000000 sharqit-0.2.2/sharqit/cpp/qgate.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    10490 2024-04-05 12:58:50.000000 sharqit-0.2.2/sharqit/cpp/qgate.h
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     7660 2024-03-14 23:07:51.000000 sharqit-0.2.2/sharqit/cpp/sharqit.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      385 2024-04-05 12:58:50.000000 sharqit-0.2.2/sharqit/cpp/sharqit.h
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    28969 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/simplify.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     2168 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/util.h
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    28058 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/zx.h
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    17166 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/zxdiagram.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      539 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/zxnode.cpp
+drwxr-xr-x   0 nakagawa  (1000) nakagawa  (1000)        0 2024-04-05 13:15:59.769859 sharqit-0.2.2/sharqit.egg-info/
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      437 2024-04-05 13:15:59.000000 sharqit-0.2.2/sharqit.egg-info/PKG-INFO
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     1015 2024-04-05 13:15:59.000000 sharqit-0.2.2/sharqit.egg-info/SOURCES.txt
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)        1 2024-04-05 13:15:59.000000 sharqit-0.2.2/sharqit.egg-info/dependency_links.txt
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)       16 2024-04-05 13:15:59.000000 sharqit-0.2.2/sharqit.egg-info/requires.txt
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)       25 2024-04-05 13:15:59.000000 sharqit-0.2.2/sharqit.egg-info/top_level.txt
```

### Comparing `sharqit-0.2.1/CMakeLists.txt` & `sharqit-0.2.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.1/LICENSE` & `sharqit-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.1/README.md` & `sharqit-0.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 ## Feature
 
 - Support two types of gate-count reduction methods:
 	- 1) using ZX-calculus
 	- 2) using Phase Polynomial
 - Implemented in C++ language
-- Provide SDK for both C++ and Python and command line tool.
+- Provide command line tool, C++ library and Python package.
 
 ## Install
 
 Install the following softwares first.
 
     $ sudo apt install nlohmann-json3-dev 
 	$ sudo apt install graphviz
@@ -36,15 +36,21 @@
 Add following lines to your ~/.bashrc. (If you are using another shell, replace as appropriate.)
 
     export LD_LIBRARY_PATH="${HOME}/lib:$LD_LIBRARY_PATH"
     export PATH="${HOME}/bin:$PATH"
 
 ### Python package
 
-Install python package as follows,
+    $ pip install sharqit
+
+Or build from source codes (PyPI).
+
+    $ pip install --no-binary :all: sharqit
+
+Or dowonload and build from source codes (Github),
 
     $ git clone https://github.com/samn33/sharqit.git
     $ cd sharqit
     $ python setup.py install --user
 
 
 ## Uninstall
@@ -202,14 +208,15 @@
 "Automated optimization of large quantum circuits with continuous parameters",
 [arXiv:1710.07345](https://arxiv.org/abs/1710.07345)
 
 
 ## Requirements
 
 - Linux (Ubuntu 22.04 LTS)
+- Python 3.10
 
 
 ## Licence
 
 MIT
```

### Comparing `sharqit-0.2.1/setup.py` & `sharqit-0.2.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 import os
 import pathlib
 from setuptools import setup, find_packages, Extension
 from setuptools.command.build_ext import build_ext as build_ext_orig
 
-_VERSION = '0.2.1'
+_VERSION = '0.2.2'
 
 class CMakeExtension(Extension):
 
     def __init__(self, name):
         super().__init__(name, sources=[])
 
 class build_ext(build_ext_orig):
@@ -37,14 +37,15 @@
         if not self.dry_run:
             self.spawn(['cmake', '--build', '.'] + build_args)
         os.chdir(str(cwd))
 
 setup(
     name='sharqit',
     version=_VERSION,
+    url='https://github.com/samn33/sharqit',
     author='Sam.N',
     author_email='saminriver33@gmail.com',
     description='Quantum Circuit Optimizer',
     long_description='',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
```

### Comparing `sharqit-0.2.1/sharqit/cpp/CMakeLists.txt` & `sharqit-0.2.2/sharqit/cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.1/sharqit/cpp/Doxyfile` & `sharqit-0.2.2/sharqit/cpp/Doxyfile`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.1/sharqit/cpp/Makefile` & `sharqit-0.2.2/sharqit/cpp/Makefile`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.1/sharqit/cpp/TAGS` & `sharqit-0.2.2/sharqit/cpp/TAGS`

 * *Files 3% similar despite different names*

```diff
@@ -1,1645 +1,1675 @@
-00000000: 0c0a 6c69 6e65 6172 5f6d 6170 2e63 7070  ..linear_map.cpp
-00000010: 2c34 3431 0a62 6f6f 6c20 5368 6172 7169  ,441.bool Sharqi
-00000020: 743a 3a4c 696e 6561 724d 6170 3a3a 6973  t::LinearMap::is
-00000030: 5f7a 6572 6f28 7f69 735f 7a65 726f 0138  _zero(.is_zero.8
-00000040: 2c31 3034 0a62 6f6f 6c20 5368 6172 7169  ,104.bool Sharqi
-00000050: 743a 3a4c 696e 6561 724d 6170 3a3a 6973  t::LinearMap::is
-00000060: 5f69 6465 6e74 6974 7928 7f69 735f 6964  _identity(.is_id
-00000070: 656e 7469 7479 0132 312c 3434 340a 626f  entity.21,444.bo
-00000080: 6f6c 2053 6861 7271 6974 3a3a 4c69 6e65  ol Sharqit::Line
-00000090: 6172 4d61 703a 3a69 735f 6469 6167 6f6e  arMap::is_diagon
-000000a0: 616c 287f 6973 5f64 6961 676f 6e61 6c01  al(.is_diagonal.
-000000b0: 3333 2c37 3432 0a62 6f6f 6c20 5368 6172  33,742.bool Shar
-000000c0: 7169 743a 3a4c 696e 6561 724d 6170 3a3a  qit::LinearMap::
-000000d0: 6973 5f69 6465 6e74 6974 795f 6d75 6c74  is_identity_mult
-000000e0: 6970 6c65 5f63 6f6e 7374 616e 7428 7f69  iple_constant(.i
-000000f0: 735f 6964 656e 7469 7479 5f6d 756c 7469  s_identity_multi
-00000100: 706c 655f 636f 6e73 7461 6e74 0134 352c  ple_constant.45,
-00000110: 3130 3336 0a62 6f6f 6c20 5368 6172 7169  1036.bool Sharqi
-00000120: 743a 3a4c 696e 6561 724d 6170 3a3a 6973  t::LinearMap::is
-00000130: 5f75 6e69 7461 7279 287f 6973 5f75 6e69  _unitary(.is_uni
-00000140: 7461 7279 0135 392c 3134 3239 0a62 6f6f  tary.59,1429.boo
-00000150: 6c20 5368 6172 7169 743a 3a4c 696e 6561  l Sharqit::Linea
-00000160: 724d 6170 3a3a 6973 5f65 7175 616c 287f  rMap::is_equal(.
-00000170: 6973 5f65 7175 616c 0137 302c 3136 3930  is_equal.70,1690
-00000180: 0a53 6861 7271 6974 3a3a 4c69 6e65 6172  .Sharqit::Linear
-00000190: 4d61 7026 2053 6861 7271 6974 3a3a 4c69  Map& Sharqit::Li
-000001a0: 6e65 6172 4d61 703a 3a6f 7065 7261 7465  nearMap::operate
-000001b0: 5f71 6761 7465 287f 6f70 6572 6174 655f  _qgate(.operate_
-000001c0: 7167 6174 6501 3831 2c31 3934 330a 0c0a  qgate.81,1943...
-000001d0: 7368 6172 7169 742e 6370 702c 3137 360a  sharqit.cpp,176.
-000001e0: 766f 6964 2070 7269 6e74 5f68 656c 7028  void print_help(
-000001f0: 7f31 312c 3133 300a 766f 6964 206f 7074  .11,130.void opt
-00000200: 696d 697a 6528 7f35 372c 3236 3233 0a76  imize(.57,2623.v
-00000210: 6f69 6420 7665 7269 6679 5f65 7175 616c  oid verify_equal
-00000220: 6974 7928 7f37 372c 3331 3431 0a76 6f69  ity(.77,3141.voi
-00000230: 6420 7261 6e64 6f6d 5f71 6369 7263 287f  d random_qcirc(.
-00000240: 3938 2c33 3730 360a 766f 6964 2070 7269  98,3706.void pri
-00000250: 6e74 5f73 7461 7473 287f 3132 362c 3434  nt_stats(.126,44
-00000260: 3933 0a76 6f69 6420 7368 6f77 5f71 6369  93.void show_qci
-00000270: 7263 287f 3134 322c 3438 3132 0a69 6e74  rc(.142,4812.int
-00000280: 206d 6169 6e28 7f31 3539 2c35 3134 390a   main(.159,5149.
-00000290: 0c0a 6f70 7469 6d69 7a65 722e 6370 702c  ..optimizer.cpp,
-000002a0: 3431 380a 7374 643a 3a73 7472 696e 6720  418.std::string 
-000002b0: 5368 6172 7169 743a 3a4f 7074 696d 697a  Sharqit::Optimiz
-000002c0: 6572 3a3a 746f 5f73 7472 696e 6728 7f74  er::to_string(.t
-000002d0: 6f5f 7374 7269 6e67 0138 2c31 3032 0a73  o_string.8,102.s
-000002e0: 7464 3a3a 7374 7269 6e67 2053 6861 7271  td::string Sharq
-000002f0: 6974 3a3a 4f70 7469 6d69 7a65 723a 3a6e  it::Optimizer::n
-00000300: 616d 6528 7f6e 616d 6501 3531 2c32 3439  ame(.name.51,249
-00000310: 300a 5368 6172 7169 743a 3a51 4369 7263  0.Sharqit::QCirc
-00000320: 2053 6861 7271 6974 3a3a 4f70 7469 6d69   Sharqit::Optimi
-00000330: 7a65 723a 3a72 6564 7563 655f 6761 7465  zer::reduce_gate
-00000340: 735f 7573 696e 675f 7a78 287f 7265 6475  s_using_zx(.redu
-00000350: 6365 5f67 6174 6573 5f75 7369 6e67 5f7a  ce_gates_using_z
-00000360: 7801 3632 2c32 3832 350a 5368 6172 7169  x.62,2825.Sharqi
-00000370: 743a 3a51 4369 7263 2053 6861 7271 6974  t::QCirc Sharqit
-00000380: 3a3a 4f70 7469 6d69 7a65 723a 3a72 6564  ::Optimizer::red
-00000390: 7563 655f 6761 7465 735f 7573 696e 675f  uce_gates_using_
-000003a0: 7070 287f 7265 6475 6365 5f67 6174 6573  pp(.reduce_gates
-000003b0: 5f75 7369 6e67 5f70 7001 3930 2c33 3438  _using_pp.90,348
-000003c0: 300a 5368 6172 7169 743a 3a51 4369 7263  0.Sharqit::QCirc
-000003d0: 2053 6861 7271 6974 3a3a 4f70 7469 6d69   Sharqit::Optimi
-000003e0: 7a65 723a 3a72 6564 7563 655f 6761 7465  zer::reduce_gate
-000003f0: 7328 7f72 6564 7563 655f 6761 7465 7301  s(.reduce_gates.
-00000400: 3131 322c 3430 3235 0a53 6861 7271 6974  112,4025.Sharqit
-00000410: 3a3a 5143 6972 6320 5368 6172 7169 743a  ::QCirc Sharqit:
-00000420: 3a4f 7074 696d 697a 6572 3a3a 6578 6563  :Optimizer::exec
-00000430: 7574 6528 7f65 7865 6375 7465 0131 3836  ute(.execute.186
-00000440: 2c35 3934 390a 0c0a 7072 6f70 6167 6174  ,5949...propagat
-00000450: 655f 7061 756c 695f 782e 6370 702c 3634  e_pauli_x.cpp,64
-00000460: 0a76 6f69 6420 5368 6172 7169 743a 3a51  .void Sharqit::Q
-00000470: 4369 7263 3a3a 7072 6f70 6167 6174 655f  Circ::propagate_
-00000480: 7061 756c 695f 7828 7f70 726f 7061 6761  pauli_x(.propaga
-00000490: 7465 5f70 6175 6c69 5f78 0139 2c31 3938  te_pauli_x.9,198
-000004a0: 0a0c 0a75 7469 6c2e 682c 3436 0a23 6465  ...util.h,46.#de
-000004b0: 6669 6e65 2055 5449 4c5f 487f 372c 3834  fine UTIL_H.7,84
-000004c0: 0a6e 616d 6573 7061 6365 2053 6861 7271  .namespace Sharq
-000004d0: 6974 207f 3133 2c31 3536 0a0c 0a73 616e  it .13,156...san
-000004e0: 6462 6f78 2f67 6175 7373 5f72 6564 7563  dbox/gauss_reduc
-000004f0: 652f 6f6c 642f 6269 6e61 7279 5f6d 6174  e/old/binary_mat
-00000500: 7269 785f 626b 3230 3233 3132 3039 2e63  rix_bk20231209.c
-00000510: 7070 2c33 3732 0a73 7464 3a3a 7374 7269  pp,372.std::stri
-00000520: 6e67 2053 6861 7271 3a3a 4269 6e61 7279  ng Sharq::Binary
-00000530: 4d61 7472 6978 3a3a 746f 5f73 7472 696e  Matrix::to_strin
-00000540: 6728 7f74 6f5f 7374 7269 6e67 0133 2c32  g(.to_string.3,2
-00000550: 380a 766f 6964 2053 6861 7271 3a3a 4269  8.void Sharq::Bi
-00000560: 6e61 7279 4d61 7472 6978 3a3a 786f 725f  naryMatrix::xor_
-00000570: 726f 7773 287f 786f 725f 726f 7773 0132  rows(.xor_rows.2
-00000580: 332c 3430 330a 766f 6964 2053 6861 7271  3,403.void Sharq
-00000590: 3a3a 4269 6e61 7279 4d61 7472 6978 3a3a  ::BinaryMatrix::
-000005a0: 7377 6170 5f72 6f77 7328 7f73 7761 705f  swap_rows(.swap_
-000005b0: 726f 7773 0133 332c 3730 350a 766f 6964  rows.33,705.void
-000005c0: 2053 6861 7271 3a3a 4269 6e61 7279 4d61   Sharq::BinaryMa
-000005d0: 7472 6978 3a3a 7377 6170 5f63 6f6c 7328  trix::swap_cols(
-000005e0: 7f73 7761 705f 636f 6c73 0134 342c 3130  .swap_cols.44,10
-000005f0: 3234 0a62 6f6f 6c20 5368 6172 713a 3a42  24.bool Sharq::B
-00000600: 696e 6172 794d 6174 7269 783a 3a66 6561  inaryMatrix::fea
-00000610: 7369 626c 6528 7f66 6561 7369 626c 6501  sible(.feasible.
-00000620: 3534 2c31 3239 360a 7374 643a 3a76 6563  54,1296.std::vec
-00000630: 746f 723c 7374 643a 3a70 6169 723c 7569  tor<std::pair<ui
-00000640: 6e74 3332 5f74 2c20 7569 6e74 3332 5f74  nt32_t, uint32_t
-00000650: 3e3e 2053 6861 7271 3a3a 4269 6e61 7279  >> Sharq::Binary
-00000660: 4d61 7472 6978 3a3a 6761 7573 735f 7265  Matrix::gauss_re
-00000670: 6475 6365 287f 6761 7573 735f 7265 6475  duce(.gauss_redu
-00000680: 6365 0137 312c 3135 3632 0a0c 0a73 616e  ce.71,1562...san
-00000690: 6462 6f78 2f67 6175 7373 5f72 6564 7563  dbox/gauss_reduc
-000006a0: 652f 6f6c 642f 6269 6e61 7279 5f6d 6174  e/old/binary_mat
-000006b0: 7269 785f 626b 3230 3233 3132 3039 2e68  rix_bk20231209.h
-000006c0: 2c36 3339 0a23 6465 6669 6e65 2047 525f  ,639.#define GR_
-000006d0: 487f 322c 3133 0a20 2063 6c61 7373 2042  H.2,13.  class B
-000006e0: 696e 6172 794d 6174 7269 787f 3234 2c33  inaryMatrix.24,3
-000006f0: 3536 0a20 2020 2075 696e 7433 325f 7420  56.    uint32_t 
-00000700: 726f 775f 6e75 6d5f 3b7f 3237 2c33 3932  row_num_;.27,392
-00000710: 0a20 2020 2075 696e 7433 325f 7420 636f  .    uint32_t co
-00000720: 6c5f 6e75 6d5f 3b7f 3238 2c34 3135 0a20  l_num_;.28,415. 
-00000730: 2020 2073 7464 3a3a 7665 6374 6f72 3c73     std::vector<s
-00000740: 7464 3a3a 7665 6374 6f72 3c75 696e 7438  td::vector<uint8
-00000750: 5f74 3e3e 2065 6c65 6d65 6e74 735f 3b7f  _t>> elements_;.
-00000760: 3239 2c34 3338 0a20 2020 2073 7464 3a3a  29,438.    std::
-00000770: 7665 6374 6f72 3c75 696e 7433 325f 743e  vector<uint32_t>
-00000780: 2072 6f77 5f69 6e64 6578 6573 5f3b 7f33   row_indexes_;.3
-00000790: 302c 3438 370a 2020 2020 4269 6e61 7279  0,487.    Binary
-000007a0: 4d61 7472 6978 287f 3332 2c35 3337 0a20  Matrix(.32,537. 
-000007b0: 2020 2042 696e 6172 794d 6174 7269 7828     BinaryMatrix(
-000007c0: 7f33 372c 3831 390a 2020 2020 4269 6e61  .37,819.    Bina
-000007d0: 7279 4d61 7472 6978 287f 3434 2c31 3037  ryMatrix(.44,107
-000007e0: 310a 2020 2020 7569 6e74 3332 5f74 2072  1.    uint32_t r
-000007f0: 6f77 5f6e 756d 287f 3437 2c31 3234 310a  ow_num(.47,1241.
-00000800: 2020 2020 7569 6e74 3332 5f74 2063 6f6c      uint32_t col
-00000810: 5f6e 756d 287f 3438 2c31 3239 310a 2020  _num(.48,1291.  
-00000820: 2020 7374 643a 3a76 6563 746f 723c 7374    std::vector<st
-00000830: 643a 3a76 6563 746f 723c 7569 6e74 385f  d::vector<uint8_
-00000840: 743e 3e20 656c 656d 656e 7473 287f 3439  t>> elements(.49
-00000850: 2c31 3334 310a 2020 2020 7374 643a 3a76  ,1341.    std::v
-00000860: 6563 746f 723c 7569 6e74 3332 5f74 3e20  ector<uint32_t> 
-00000870: 726f 775f 696e 6465 7865 7328 7f35 302c  row_indexes(.50,
-00000880: 3134 3139 0a20 2020 2076 6f69 6420 726f  1419.    void ro
-00000890: 775f 6e75 6d28 7f35 322c 3135 3038 0a20  w_num(.52,1508. 
-000008a0: 2020 2076 6f69 6420 636f 6c5f 6e75 6d28     void col_num(
-000008b0: 7f35 332c 3135 3733 0a20 2020 2076 6f69  .53,1573.    voi
-000008c0: 6420 656c 656d 656e 7473 287f 3534 2c31  d elements(.54,1
-000008d0: 3633 380a 2020 2020 766f 6964 2072 6f77  638.    void row
-000008e0: 5f69 6e64 6578 6573 287f 3535 2c31 3733  _indexes(.55,173
-000008f0: 330a 2020 2020 7374 643a 3a76 6563 746f  3.    std::vecto
-00000900: 723c 7f73 7464 3a3a 7665 6374 6f72 0136  r<.std::vector.6
-00000910: 322c 3230 3834 0a20 2020 2066 7269 656e  2,2084.    frien
-00000920: 6420 7374 643a 3a6f 7374 7265 616d 2620  d std::ostream& 
-00000930: 6f70 6572 6174 6f72 3c3c 287f 3633 2c32  operator<<(.63,2
-00000940: 3134 370a 0c0a 7361 6e64 626f 782f 6761  147...sandbox/ga
-00000950: 7573 735f 7265 6475 6365 2f6f 6c64 2f62  uss_reduce/old/b
-00000960: 696e 6172 795f 6d61 7472 6978 2e68 2c36  inary_matrix.h,6
-00000970: 3037 0a23 6465 6669 6e65 2047 525f 487f  07.#define GR_H.
-00000980: 322c 3133 0a20 2063 6c61 7373 2042 696e  2,13.  class Bin
-00000990: 6172 794d 6174 7269 787f 3234 2c33 3536  aryMatrix.24,356
-000009a0: 0a20 2020 2075 696e 7433 325f 7420 726f  .    uint32_t ro
-000009b0: 775f 6e75 6d5f 3b7f 3237 2c33 3932 0a20  w_num_;.27,392. 
-000009c0: 2020 2075 696e 7433 325f 7420 636f 6c5f     uint32_t col_
-000009d0: 6e75 6d5f 3b7f 3238 2c34 3135 0a20 2020  num_;.28,415.   
-000009e0: 2073 7464 3a3a 7665 6374 6f72 3c73 7464   std::vector<std
-000009f0: 3a3a 7665 6374 6f72 3c62 6f6f 6c3e 3e20  ::vector<bool>> 
-00000a00: 656c 656d 656e 7473 5f3b 7f32 392c 3433  elements_;.29,43
-00000a10: 380a 2020 2020 7374 643a 3a76 6563 746f  8.    std::vecto
-00000a20: 723c 7569 6e74 3332 5f74 3e20 726f 775f  r<uint32_t> row_
-00000a30: 696e 6465 7865 735f 3b7f 3330 2c34 3834  indexes_;.30,484
-00000a40: 0a20 2020 2042 696e 6172 794d 6174 7269  .    BinaryMatri
-00000a50: 7828 7f33 322c 3533 340a 2020 2020 4269  x(.32,534.    Bi
-00000a60: 6e61 7279 4d61 7472 6978 287f 3337 2c37  naryMatrix(.37,7
-00000a70: 3932 0a20 2020 2075 696e 7433 325f 7420  92.    uint32_t 
-00000a80: 726f 775f 6e75 6d28 7f34 352c 3130 3538  row_num(.45,1058
-00000a90: 0a20 2020 2075 696e 7433 325f 7420 636f  .    uint32_t co
-00000aa0: 6c5f 6e75 6d28 7f34 362c 3131 3038 0a20  l_num(.46,1108. 
-00000ab0: 2020 2073 7464 3a3a 7665 6374 6f72 3c73     std::vector<s
-00000ac0: 7464 3a3a 7665 6374 6f72 3c62 6f6f 6c3e  td::vector<bool>
-00000ad0: 3e20 656c 656d 656e 7473 287f 3437 2c31  > elements(.47,1
-00000ae0: 3135 380a 2020 2020 7374 643a 3a76 6563  158.    std::vec
-00000af0: 746f 723c 7569 6e74 3332 5f74 3e20 726f  tor<uint32_t> ro
-00000b00: 775f 696e 6465 7865 7328 7f34 382c 3132  w_indexes(.48,12
-00000b10: 3333 0a20 2020 2076 6f69 6420 726f 775f  33.    void row_
-00000b20: 6e75 6d28 7f35 302c 3133 3232 0a20 2020  num(.50,1322.   
-00000b30: 2076 6f69 6420 636f 6c5f 6e75 6d28 7f35   void col_num(.5
-00000b40: 312c 3133 3837 0a20 2020 2076 6f69 6420  1,1387.    void 
-00000b50: 656c 656d 656e 7473 287f 3532 2c31 3435  elements(.52,145
-00000b60: 320a 2020 2020 766f 6964 2072 6f77 5f69  2.    void row_i
-00000b70: 6e64 6578 6573 287f 3533 2c31 3534 340a  ndexes(.53,1544.
-00000b80: 2020 2020 7374 643a 3a76 6563 746f 723c      std::vector<
-00000b90: 7f73 7464 3a3a 7665 6374 6f72 0135 382c  .std::vector.58,
-00000ba0: 3138 3132 0a20 2020 2066 7269 656e 6420  1812.    friend 
-00000bb0: 7374 643a 3a6f 7374 7265 616d 2620 6f70  std::ostream& op
-00000bc0: 6572 6174 6f72 3c3c 287f 3539 2c31 3837  erator<<(.59,187
-00000bd0: 350a 0c0a 7361 6e64 626f 782f 6761 7573  5...sandbox/gaus
-00000be0: 735f 7265 6475 6365 2f6f 6c64 2f6d 6169  s_reduce/old/mai
-00000bf0: 6e2e 6370 702c 3135 0a69 6e74 206d 6169  n.cpp,15.int mai
-00000c00: 6e28 7f33 2c32 380a 0c0a 7361 6e64 626f  n(.3,28...sandbo
-00000c10: 782f 6761 7573 735f 7265 6475 6365 2f6f  x/gauss_reduce/o
-00000c20: 6c64 2f62 696e 6172 795f 6d61 7472 6978  ld/binary_matrix
-00000c30: 2e63 7070 2c32 3634 0a73 7464 3a3a 7374  .cpp,264.std::st
-00000c40: 7269 6e67 2053 6861 7271 3a3a 4269 6e61  ring Sharq::Bina
-00000c50: 7279 4d61 7472 6978 3a3a 746f 5f73 7472  ryMatrix::to_str
-00000c60: 696e 6728 7f74 6f5f 7374 7269 6e67 0133  ing(.to_string.3
-00000c70: 2c32 380a 766f 6964 2053 6861 7271 3a3a  ,28.void Sharq::
-00000c80: 4269 6e61 7279 4d61 7472 6978 3a3a 786f  BinaryMatrix::xo
-00000c90: 725f 726f 7773 287f 786f 725f 726f 7773  r_rows(.xor_rows
-00000ca0: 0132 332c 3338 370a 766f 6964 2053 6861  .23,387.void Sha
-00000cb0: 7271 3a3a 4269 6e61 7279 4d61 7472 6978  rq::BinaryMatrix
-00000cc0: 3a3a 7377 6170 5f72 6f77 7328 7f73 7761  ::swap_rows(.swa
-00000cd0: 705f 726f 7773 0133 332c 3638 360a 7374  p_rows.33,686.st
-00000ce0: 643a 3a76 6563 746f 723c 7374 643a 3a70  d::vector<std::p
-00000cf0: 6169 723c 7569 6e74 3332 5f74 2c20 7569  air<uint32_t, ui
-00000d00: 6e74 3332 5f74 3e3e 2053 6861 7271 3a3a  nt32_t>> Sharq::
-00000d10: 4269 6e61 7279 4d61 7472 6978 3a3a 6761  BinaryMatrix::ga
-00000d20: 7573 735f 7265 6475 6365 287f 6761 7573  uss_reduce(.gaus
-00000d30: 735f 7265 6475 6365 0134 342c 3130 3035  s_reduce.44,1005
-00000d40: 0a0c 0a73 616e 6462 6f78 2f67 6175 7373  ...sandbox/gauss
-00000d50: 5f72 6564 7563 652f 6f6c 642f 6269 6e61  _reduce/old/bina
-00000d60: 7279 5f6d 6174 7269 785f 626b 3230 3233  ry_matrix_bk2023
-00000d70: 3130 3231 2e63 7070 2c33 3732 0a73 7464  1021.cpp,372.std
-00000d80: 3a3a 7374 7269 6e67 2053 6861 7271 3a3a  ::string Sharq::
-00000d90: 4269 6e61 7279 4d61 7472 6978 3a3a 746f  BinaryMatrix::to
-00000da0: 5f73 7472 696e 6728 7f74 6f5f 7374 7269  _string(.to_stri
-00000db0: 6e67 0133 2c32 380a 766f 6964 2053 6861  ng.3,28.void Sha
-00000dc0: 7271 3a3a 4269 6e61 7279 4d61 7472 6978  rq::BinaryMatrix
-00000dd0: 3a3a 786f 725f 726f 7773 287f 786f 725f  ::xor_rows(.xor_
-00000de0: 726f 7773 0132 332c 3338 370a 766f 6964  rows.23,387.void
-00000df0: 2053 6861 7271 3a3a 4269 6e61 7279 4d61   Sharq::BinaryMa
-00000e00: 7472 6978 3a3a 7377 6170 5f72 6f77 7328  trix::swap_rows(
-00000e10: 7f73 7761 705f 726f 7773 0133 332c 3638  .swap_rows.33,68
-00000e20: 360a 766f 6964 2053 6861 7271 3a3a 4269  6.void Sharq::Bi
-00000e30: 6e61 7279 4d61 7472 6978 3a3a 7377 6170  naryMatrix::swap
-00000e40: 5f63 6f6c 7328 7f73 7761 705f 636f 6c73  _cols(.swap_cols
-00000e50: 0134 342c 3130 3035 0a62 6f6f 6c20 5368  .44,1005.bool Sh
-00000e60: 6172 713a 3a42 696e 6172 794d 6174 7269  arq::BinaryMatri
-00000e70: 783a 3a66 6561 7369 626c 6528 7f66 6561  x::feasible(.fea
-00000e80: 7369 626c 6501 3534 2c31 3237 370a 7374  sible.54,1277.st
-00000e90: 643a 3a76 6563 746f 723c 7374 643a 3a70  d::vector<std::p
-00000ea0: 6169 723c 7569 6e74 3332 5f74 2c20 7569  air<uint32_t, ui
-00000eb0: 6e74 3332 5f74 3e3e 2053 6861 7271 3a3a  nt32_t>> Sharq::
-00000ec0: 4269 6e61 7279 4d61 7472 6978 3a3a 6761  BinaryMatrix::ga
-00000ed0: 7573 735f 7265 6475 6365 287f 6761 7573  uss_reduce(.gaus
-00000ee0: 735f 7265 6475 6365 0137 312c 3135 3433  s_reduce.71,1543
-00000ef0: 0a0c 0a73 616e 6462 6f78 2f67 6175 7373  ...sandbox/gauss
-00000f00: 5f72 6564 7563 652f 6269 6e61 7279 5f6d  _reduce/binary_m
-00000f10: 6174 7269 782e 682c 3735 310a 2364 6566  atrix.h,751.#def
-00000f20: 696e 6520 4752 5f48 7f32 2c31 330a 2020  ine GR_H.2,13.  
-00000f30: 636c 6173 7320 4269 6e61 7279 4d61 7472  class BinaryMatr
-00000f40: 6978 7f32 342c 3335 360a 2020 2020 7569  ix.24,356.    ui
-00000f50: 6e74 3332 5f74 2072 6f77 5f6e 756d 5f3b  nt32_t row_num_;
-00000f60: 7f32 372c 3339 320a 2020 2020 7569 6e74  .27,392.    uint
-00000f70: 3332 5f74 2063 6f6c 5f6e 756d 5f3b 7f32  32_t col_num_;.2
-00000f80: 382c 3431 350a 2020 2020 7374 643a 3a76  8,415.    std::v
-00000f90: 6563 746f 723c 7374 643a 3a76 6563 746f  ector<std::vecto
-00000fa0: 723c 7569 6e74 385f 743e 3e20 656c 656d  r<uint8_t>> elem
-00000fb0: 656e 7473 5f3b 7f32 392c 3433 380a 2020  ents_;.29,438.  
-00000fc0: 2020 7374 643a 3a76 6563 746f 723c 7569    std::vector<ui
-00000fd0: 6e74 3332 5f74 3e20 726f 775f 696e 6465  nt32_t> row_inde
-00000fe0: 7865 735f 3b7f 3330 2c34 3837 0a20 2020  xes_;.30,487.   
-00000ff0: 2042 696e 6172 794d 6174 7269 7828 7f33   BinaryMatrix(.3
-00001000: 322c 3533 370a 2020 2020 4269 6e61 7279  2,537.    Binary
-00001010: 4d61 7472 6978 287f 3337 2c38 3139 0a20  Matrix(.37,819. 
-00001020: 2020 2042 696e 6172 794d 6174 7269 7828     BinaryMatrix(
-00001030: 7f34 342c 3130 3731 0a20 2020 2075 696e  .44,1071.    uin
-00001040: 7433 325f 7420 726f 775f 6e75 6d28 7f34  t32_t row_num(.4
-00001050: 372c 3132 3431 0a20 2020 2075 696e 7433  7,1241.    uint3
-00001060: 325f 7420 636f 6c5f 6e75 6d28 7f34 382c  2_t col_num(.48,
-00001070: 3132 3931 0a20 2020 2073 7464 3a3a 7665  1291.    std::ve
-00001080: 6374 6f72 3c73 7464 3a3a 7665 6374 6f72  ctor<std::vector
-00001090: 3c75 696e 7438 5f74 3e3e 2065 6c65 6d65  <uint8_t>> eleme
-000010a0: 6e74 7328 7f34 392c 3133 3431 0a20 2020  nts(.49,1341.   
-000010b0: 2073 7464 3a3a 7665 6374 6f72 3c75 696e   std::vector<uin
-000010c0: 7433 325f 743e 2072 6f77 5f69 6e64 6578  t32_t> row_index
-000010d0: 6573 287f 3530 2c31 3431 390a 2020 2020  es(.50,1419.    
-000010e0: 766f 6964 2072 6f77 5f6e 756d 287f 3532  void row_num(.52
-000010f0: 2c31 3530 380a 2020 2020 766f 6964 2063  ,1508.    void c
-00001100: 6f6c 5f6e 756d 287f 3533 2c31 3537 330a  ol_num(.53,1573.
-00001110: 2020 2020 766f 6964 2065 6c65 6d65 6e74      void element
-00001120: 7328 7f35 342c 3136 3338 0a20 2020 2076  s(.54,1638.    v
-00001130: 6f69 6420 726f 775f 696e 6465 7865 7328  oid row_indexes(
-00001140: 7f35 352c 3137 3333 0a20 2020 2076 6f69  .55,1733.    voi
-00001150: 6420 786f 725f 726f 7773 287f 3538 2c31  d xor_rows(.58,1
-00001160: 3839 300a 2020 2020 766f 6964 2073 7761  890.    void swa
-00001170: 705f 726f 7773 287f 3637 2c32 3139 320a  p_rows(.67,2192.
-00001180: 2020 2020 766f 6964 2073 7761 705f 636f      void swap_co
-00001190: 6c73 287f 3737 2c32 3531 350a 2020 2020  ls(.77,2515.    
-000011a0: 626f 6f6c 2066 6561 7369 626c 6528 7f38  bool feasible(.8
-000011b0: 362c 3237 3837 0a20 2020 2073 7464 3a3a  6,2787.    std::
-000011c0: 7665 6374 6f72 3c7f 7374 643a 3a76 6563  vector<.std::vec
-000011d0: 746f 7201 3130 322c 3330 3433 0a20 2020  tor.102,3043.   
-000011e0: 2066 7269 656e 6420 7374 643a 3a6f 7374   friend std::ost
-000011f0: 7265 616d 2620 6f70 6572 6174 6f72 3c3c  ream& operator<<
-00001200: 287f 3130 332c 3331 3036 0a0c 0a73 616e  (.103,3106...san
-00001210: 6462 6f78 2f67 6175 7373 5f72 6564 7563  dbox/gauss_reduc
-00001220: 652f 6d61 696e 2e63 7070 2c31 370a 696e  e/main.cpp,17.in
-00001230: 7420 6d61 696e 287f 3430 2c35 3832 0a0c  t main(.40,582..
-00001240: 0a73 616e 6462 6f78 2f67 6175 7373 5f72  .sandbox/gauss_r
-00001250: 6564 7563 652f 6269 6e61 7279 5f6d 6174  educe/binary_mat
-00001260: 7269 782e 6370 702c 3135 370a 7374 643a  rix.cpp,157.std:
-00001270: 3a73 7472 696e 6720 5368 6172 713a 3a42  :string Sharq::B
-00001280: 696e 6172 794d 6174 7269 783a 3a74 6f5f  inaryMatrix::to_
-00001290: 7374 7269 6e67 287f 746f 5f73 7472 696e  string(.to_strin
-000012a0: 6701 332c 3238 0a73 7464 3a3a 7665 6374  g.3,28.std::vect
-000012b0: 6f72 3c73 7464 3a3a 7061 6972 3c75 696e  or<std::pair<uin
-000012c0: 7433 325f 742c 2075 696e 7433 325f 743e  t32_t, uint32_t>
-000012d0: 3e20 5368 6172 713a 3a42 696e 6172 794d  > Sharq::BinaryM
-000012e0: 6174 7269 783a 3a67 6175 7373 5f72 6564  atrix::gauss_red
-000012f0: 7563 6528 7f67 6175 7373 5f72 6564 7563  uce(.gauss_reduc
-00001300: 6501 3233 2c34 3033 0a0c 0a64 6167 6369  e.23,403...dagci
-00001310: 7263 2e63 7070 2c31 3632 350a 5368 6172  rc.cpp,1625.Shar
-00001320: 7169 743a 3a44 4147 4369 7263 3a3a 4441  qit::DAGCirc::DA
-00001330: 4743 6972 6328 7f44 4147 4369 7263 0138  GCirc(.DAGCirc.8
-00001340: 2c39 320a 5368 6172 7169 743a 3a44 4147  ,92.Sharqit::DAG
-00001350: 4369 7263 3a3a 4441 4743 6972 6328 7f44  Circ::DAGCirc(.D
-00001360: 4147 4369 7263 0132 392c 3639 390a 7374  AGCirc.29,699.st
-00001370: 643a 3a73 7472 696e 6720 5368 6172 7169  d::string Sharqi
-00001380: 743a 3a44 4147 4369 7263 3a3a 746f 5f73  t::DAGCirc::to_s
-00001390: 7472 696e 6728 7f74 6f5f 7374 7269 6e67  tring(.to_string
-000013a0: 0135 332c 3133 3933 0a75 696e 7433 325f  .53,1393.uint32_
-000013b0: 7420 5368 6172 7169 743a 3a44 4147 4369  t Sharqit::DAGCi
-000013c0: 7263 3a3a 6170 7065 6e64 5f6e 6f64 6528  rc::append_node(
-000013d0: 7f61 7070 656e 645f 6e6f 6465 0137 322c  .append_node.72,
-000013e0: 3138 3632 0a75 696e 7433 325f 7420 5368  1862.uint32_t Sh
-000013f0: 6172 7169 743a 3a44 4147 4369 7263 3a3a  arqit::DAGCirc::
-00001400: 7072 6576 5f6e 6f64 6528 7f70 7265 765f  prev_node(.prev_
-00001410: 6e6f 6465 0138 302c 3230 3535 0a75 696e  node.80,2055.uin
-00001420: 7433 325f 7420 5368 6172 7169 743a 3a44  t32_t Sharqit::D
-00001430: 4147 4369 7263 3a3a 6e65 7874 5f6e 6f64  AGCirc::next_nod
-00001440: 6528 7f6e 6578 745f 6e6f 6465 0139 392c  e(.next_node.99,
-00001450: 3235 3233 0a76 6f69 6420 5368 6172 7169  2523.void Sharqi
-00001460: 743a 3a44 4147 4369 7263 3a3a 636f 6e6e  t::DAGCirc::conn
-00001470: 6563 745f 6e6f 6465 7328 7f63 6f6e 6e65  ect_nodes(.conne
-00001480: 6374 5f6e 6f64 6573 0131 3138 2c32 3938  ct_nodes.118,298
-00001490: 380a 766f 6964 2053 6861 7271 6974 3a3a  8.void Sharqit::
-000014a0: 4441 4743 6972 633a 3a72 656d 6f76 655f  DAGCirc::remove_
-000014b0: 6e6f 6465 287f 7265 6d6f 7665 5f6e 6f64  node(.remove_nod
-000014c0: 6501 3132 392c 3334 3733 0a76 6f69 6420  e.129,3473.void 
-000014d0: 5368 6172 7169 743a 3a44 4147 4369 7263  Sharqit::DAGCirc
-000014e0: 3a3a 7265 6d6f 7665 5f65 6467 6528 7f72  ::remove_edge(.r
-000014f0: 656d 6f76 655f 6564 6765 0131 3631 2c34  emove_edge.161,4
-00001500: 3132 330a 766f 6964 2053 6861 7271 6974  123.void Sharqit
-00001510: 3a3a 4441 4743 6972 633a 3a72 656d 6f76  ::DAGCirc::remov
-00001520: 655f 6564 6765 287f 7265 6d6f 7665 5f65  e_edge(.remove_e
-00001530: 6467 6501 3137 392c 3435 3238 0a76 6f69  dge.179,4528.voi
-00001540: 6420 5368 6172 7169 743a 3a44 4147 4369  d Sharqit::DAGCi
-00001550: 7263 3a3a 7265 6d6f 7665 5f65 6467 6573  rc::remove_edges
-00001560: 5f6f 665f 6e6f 6465 287f 7265 6d6f 7665  _of_node(.remove
-00001570: 5f65 6467 6573 5f6f 665f 6e6f 6465 0131  _edges_of_node.1
-00001580: 3937 2c34 3938 330a 766f 6964 2053 6861  97,4983.void Sha
-00001590: 7271 6974 3a3a 4441 4743 6972 633a 3a72  rqit::DAGCirc::r
-000015a0: 656d 6f76 655f 6973 6f6c 6174 6564 5f6e  emove_isolated_n
-000015b0: 6f64 6573 287f 7265 6d6f 7665 5f69 736f  odes(.remove_iso
-000015c0: 6c61 7465 645f 6e6f 6465 7301 3231 312c  lated_nodes.211,
-000015d0: 3533 3132 0a53 6861 7271 6974 3a3a 4441  5312.Sharqit::DA
-000015e0: 4743 6972 6326 2053 6861 7271 6974 3a3a  GCirc& Sharqit::
-000015f0: 4441 4743 6972 633a 3a61 6464 5f71 6761  DAGCirc::add_qga
-00001600: 7465 287f 6164 645f 7167 6174 6501 3232  te(.add_qgate.22
-00001610: 372c 3536 3331 0a53 6861 7271 6974 3a3a  7,5631.Sharqit::
-00001620: 5143 6972 6320 5368 6172 7169 743a 3a44  QCirc Sharqit::D
-00001630: 4147 4369 7263 3a3a 746f 5f71 6369 7263  AGCirc::to_qcirc
-00001640: 287f 746f 5f71 6369 7263 0132 3634 2c36  (.to_qcirc.264,6
-00001650: 3731 370a 766f 6964 2053 6861 7271 6974  717.void Sharqit
-00001660: 3a3a 4441 4743 6972 633a 3a69 645f 7265  ::DAGCirc::id_re
-00001670: 6d6f 7661 6c28 7f69 645f 7265 6d6f 7661  moval(.id_remova
-00001680: 6c01 3330 362c 3737 3639 0a76 6f69 6420  l.306,7769.void 
-00001690: 5368 6172 7169 743a 3a44 4147 4369 7263  Sharqit::DAGCirc
-000016a0: 3a3a 6378 5f74 6f5f 637a 5f67 6174 6528  ::cx_to_cz_gate(
-000016b0: 7f63 785f 746f 5f63 7a5f 6761 7465 0133  .cx_to_cz_gate.3
-000016c0: 3239 2c38 3438 340a 766f 6964 2053 6861  29,8484.void Sha
-000016d0: 7271 6974 3a3a 4441 4743 6972 633a 3a63  rqit::DAGCirc::c
-000016e0: 7a5f 746f 5f63 785f 6761 7465 287f 637a  z_to_cx_gate(.cz
-000016f0: 5f74 6f5f 6378 5f67 6174 6501 3335 392c  _to_cx_gate.359,
-00001700: 3933 3037 0a76 6f69 6420 5368 6172 7169  9307.void Sharqi
-00001710: 743a 3a44 4147 4369 7263 3a3a 6861 6461  t::DAGCirc::hada
-00001720: 6d61 7264 5f67 6174 655f 7265 6475 6374  mard_gate_reduct
-00001730: 696f 6e5f 3128 7f68 6164 616d 6172 645f  ion_1(.hadamard_
-00001740: 6761 7465 5f72 6564 7563 7469 6f6e 5f31  gate_reduction_1
-00001750: 0133 3934 2c31 3035 3436 0a76 6f69 6420  .394,10546.void 
-00001760: 5368 6172 7169 743a 3a44 4147 4369 7263  Sharqit::DAGCirc
-00001770: 3a3a 6861 6461 6d61 7264 5f67 6174 655f  ::hadamard_gate_
-00001780: 7265 6475 6374 696f 6e5f 3228 7f68 6164  reduction_2(.had
-00001790: 616d 6172 645f 6761 7465 5f72 6564 7563  amard_gate_reduc
-000017a0: 7469 6f6e 5f32 0134 3334 2c31 3138 3036  tion_2.434,11806
-000017b0: 0a76 6f69 6420 5368 6172 7169 743a 3a44  .void Sharqit::D
-000017c0: 4147 4369 7263 3a3a 6861 6461 6d61 7264  AGCirc::hadamard
-000017d0: 5f67 6174 655f 7265 6475 6374 696f 6e5f  _gate_reduction_
-000017e0: 3328 7f68 6164 616d 6172 645f 6761 7465  3(.hadamard_gate
-000017f0: 5f72 6564 7563 7469 6f6e 5f33 0134 3735  _reduction_3.475
-00001800: 2c31 3330 3837 0a75 696e 7433 325f 7420  ,13087.uint32_t 
-00001810: 5368 6172 7169 743a 3a44 4147 4369 7263  Sharqit::DAGCirc
-00001820: 3a3a 6861 6461 6d61 7264 5f67 6174 655f  ::hadamard_gate_
-00001830: 7265 6475 6374 696f 6e28 7f68 6164 616d  reduction(.hadam
-00001840: 6172 645f 6761 7465 5f72 6564 7563 7469  ard_gate_reducti
-00001850: 6f6e 0135 3333 2c31 3530 3632 0a75 696e  on.533,15062.uin
-00001860: 7433 325f 7420 5368 6172 7169 743a 3a44  t32_t Sharqit::D
-00001870: 4147 4369 7263 3a3a 7369 6e67 6c65 5f71  AGCirc::single_q
-00001880: 7562 6974 5f67 6174 655f 6361 6e63 656c  ubit_gate_cancel
-00001890: 6c61 7469 6f6e 287f 7369 6e67 6c65 5f71  lation(.single_q
-000018a0: 7562 6974 5f67 6174 655f 6361 6e63 656c  ubit_gate_cancel
-000018b0: 6c61 7469 6f6e 0135 3434 2c31 3532 3735  lation.544,15275
-000018c0: 0a75 696e 7433 325f 7420 5368 6172 7169  .uint32_t Sharqi
-000018d0: 743a 3a44 4147 4369 7263 3a3a 7477 6f5f  t::DAGCirc::two_
-000018e0: 7175 6269 745f 6761 7465 5f63 616e 6365  qubit_gate_cance
-000018f0: 6c6c 6174 696f 6e28 7f74 776f 5f71 7562  llation(.two_qub
-00001900: 6974 5f67 6174 655f 6361 6e63 656c 6c61  it_gate_cancella
-00001910: 7469 6f6e 0136 3432 2c31 3739 3934 0a76  tion.642,17994.v
-00001920: 6f69 6420 5368 6172 7169 743a 3a44 4147  oid Sharqit::DAG
-00001930: 4369 7263 3a3a 7275 6c65 5f62 6173 6564  Circ::rule_based
-00001940: 5f67 6174 655f 7265 6475 6374 696f 6e28  _gate_reduction(
-00001950: 7f72 756c 655f 6261 7365 645f 6761 7465  .rule_based_gate
-00001960: 5f72 6564 7563 7469 6f6e 0137 3332 2c32  _reduction.732,2
-00001970: 3037 3235 0a0c 0a70 6861 7365 2e68 2c39  0725...phase.h,9
-00001980: 3134 0a23 6465 6669 6e65 2050 4841 5345  14.#define PHASE
-00001990: 5f48 7f37 2c38 300a 2020 636c 6173 7320  _H.7,80.  class 
-000019a0: 5068 6173 657f 3233 2c32 3936 0a20 2020  Phase.23,296.   
-000019b0: 2046 7261 6374 696f 6e20 6672 6163 5f3b   Fraction frac_;
-000019c0: 7f32 362c 3332 350a 2020 2020 5068 6173  .26,325.    Phas
-000019d0: 6528 7f33 332c 3632 380a 2020 2020 5068  e(.33,628.    Ph
-000019e0: 6173 6528 7f33 382c 3834 370a 2020 2020  ase(.38,847.    
-000019f0: 5068 6173 6528 7f34 332c 3130 3431 0a20  Phase(.43,1041. 
-00001a00: 2020 2050 6861 7365 287f 3438 2c31 3136     Phase(.48,116
-00001a10: 370a 2020 2020 4672 6163 7469 6f6e 2066  7.    Fraction f
-00001a20: 7261 6328 7f35 302c 3132 3439 0a20 2020  rac(.50,1249.   
-00001a30: 2076 6f69 6420 6672 6163 287f 3532 2c31   void frac(.52,1
-00001a40: 3332 310a 2020 2020 646f 7562 6c65 2076  321.    double v
-00001a50: 616c 7565 287f 3632 2c31 3630 380a 2020  alue(.62,1608.  
-00001a60: 2020 626f 6f6c 2069 735f 7a65 726f 287f    bool is_zero(.
-00001a70: 3637 2c31 3830 350a 2020 2020 626f 6f6c  67,1805.    bool
-00001a80: 2069 735f 706f 7369 7469 7665 287f 3732   is_positive(.72
-00001a90: 2c31 3938 330a 2020 2020 626f 6f6c 2069  ,1983.    bool i
-00001aa0: 735f 6e65 6761 7469 7665 287f 3737 2c32  s_negative(.77,2
-00001ab0: 3136 350a 2020 2020 766f 6964 2072 6564  165.    void red
-00001ac0: 7563 6528 7f38 312c 3233 3032 0a20 2020  uce(.81,2302.   
-00001ad0: 2076 6f69 6420 6d6f 645f 3270 6928 7f38   void mod_2pi(.8
-00001ae0: 352c 3233 3931 0a20 2020 2050 6861 7365  5,2391.    Phase
-00001af0: 206f 7065 7261 746f 722b 287f 3939 2c32   operator+(.99,2
-00001b00: 3839 320a 2020 2020 5068 6173 6520 6f70  892.    Phase op
-00001b10: 6572 6174 6f72 2d28 7f31 3030 2c32 3933  erator-(.100,293
-00001b20: 380a 2020 2020 5068 6173 6526 206f 7065  8.    Phase& ope
-00001b30: 7261 746f 722b 3d28 7f6f 7065 7261 746f  rator+=(.operato
-00001b40: 722b 3d01 3130 312c 3239 3932 0a20 2020  r+=.101,2992.   
-00001b50: 2050 6861 7365 2620 6f70 6572 6174 6f72   Phase& operator
-00001b60: 2d3d 287f 6f70 6572 6174 6f72 2d3d 0131  -=(.operator-=.1
-00001b70: 3032 2c33 3037 310a 2020 2020 5068 6173  02,3071.    Phas
-00001b80: 6526 206f 7065 7261 746f 722a 3d28 7f6f  e& operator*=(.o
-00001b90: 7065 7261 746f 722a 3d01 3130 332c 3331  perator*=.103,31
-00001ba0: 3530 0a20 2020 2050 6861 7365 2620 6f70  50.    Phase& op
-00001bb0: 6572 6174 6f72 2f3d 287f 6f70 6572 6174  erator/=(.operat
-00001bc0: 6f72 2f3d 0131 3034 2c33 3232 330a 2020  or/=.104,3223.  
-00001bd0: 2020 6672 6965 6e64 2062 6f6f 6c20 6f70    friend bool op
-00001be0: 6572 6174 6f72 3d3d 287f 6f70 6572 6174  erator==(.operat
-00001bf0: 6f72 3d3d 0131 3035 2c33 3239 360a 2020  or==.105,3296.  
-00001c00: 2020 6672 6965 6e64 2062 6f6f 6c20 6f70    friend bool op
-00001c10: 6572 6174 6f72 213d 287f 6f70 6572 6174  erator!=(.operat
-00001c20: 6f72 213d 0131 3130 2c33 3530 360a 2020  or!=.110,3506.  
-00001c30: 2020 6672 6965 6e64 2050 6861 7365 206f    friend Phase o
-00001c40: 7065 7261 746f 722b 287f 3131 312c 3335  perator+(.111,35
-00001c50: 3935 0a20 2020 2066 7269 656e 6420 5068  95.    friend Ph
-00001c60: 6173 6520 6f70 6572 6174 6f72 2d28 7f31  ase operator-(.1
-00001c70: 3132 2c33 3730 310a 2020 2020 6672 6965  12,3701.    frie
-00001c80: 6e64 2050 6861 7365 206f 7065 7261 746f  nd Phase operato
-00001c90: 722a 287f 3131 332c 3338 3037 0a20 2020  r*(.113,3807.   
-00001ca0: 2066 7269 656e 6420 5068 6173 6520 6f70   friend Phase op
-00001cb0: 6572 6174 6f72 2a28 7f31 3134 2c33 3930  erator*(.114,390
-00001cc0: 370a 2020 2020 6672 6965 6e64 2050 6861  7.    friend Pha
-00001cd0: 7365 206f 7065 7261 746f 722f 287f 3131  se operator/(.11
-00001ce0: 352c 3430 3037 0a20 2020 2066 7269 656e  5,4007.    frien
-00001cf0: 6420 7374 643a 3a6f 7374 7265 616d 2620  d std::ostream& 
-00001d00: 6f70 6572 6174 6f72 3c3c 287f 3131 362c  operator<<(.116,
-00001d10: 3431 3037 0a0c 0a6e 625f 7368 6172 7169  4107...nb_sharqi
-00001d20: 742e 6370 702c 3138 0a4e 425f 4d4f 4455  t.cpp,18.NB_MODU
-00001d30: 4c45 287f 3133 2c32 3331 0a0c 0a62 696e  LE(.13,231...bin
-00001d40: 6172 795f 6d61 7472 6978 2e68 2c38 3337  ary_matrix.h,837
-00001d50: 0a23 6465 6669 6e65 2042 494e 4152 595f  .#define BINARY_
-00001d60: 4d41 5452 4958 5f48 7f37 2c31 3033 0a20  MATRIX_H.7,103. 
-00001d70: 2063 6c61 7373 2042 696e 6172 794d 6174   class BinaryMat
-00001d80: 7269 787f 3230 2c32 3837 0a20 2020 2075  rix.20,287.    u
-00001d90: 696e 7433 325f 7420 726f 775f 6e75 6d5f  int32_t row_num_
-00001da0: 3b7f 3233 2c33 3233 0a20 2020 2075 696e  ;.23,323.    uin
-00001db0: 7433 325f 7420 636f 6c5f 6e75 6d5f 3b7f  t32_t col_num_;.
-00001dc0: 3234 2c33 3736 0a20 2020 2073 7464 3a3a  24,376.    std::
-00001dd0: 7665 6374 6f72 3c73 7464 3a3a 7665 6374  vector<std::vect
-00001de0: 6f72 3c75 696e 7438 5f74 3e3e 2065 6c65  or<uint8_t>> ele
-00001df0: 6d65 6e74 735f 3b7f 3235 2c34 3332 0a20  ments_;.25,432. 
-00001e00: 2020 2073 7464 3a3a 7665 6374 6f72 3c75     std::vector<u
-00001e10: 696e 7433 325f 743e 2072 6f77 5f69 6e64  int32_t> row_ind
-00001e20: 6578 6573 5f3b 7f32 362c 3533 330a 2020  exes_;.26,533.  
-00001e30: 2020 4269 6e61 7279 4d61 7472 6978 287f    BinaryMatrix(.
-00001e40: 3334 2c38 3631 0a20 2020 2042 696e 6172  34,861.    Binar
-00001e50: 794d 6174 7269 7828 7f34 332c 3132 3536  yMatrix(.43,1256
-00001e60: 0a20 2020 2042 696e 6172 794d 6174 7269  .    BinaryMatri
-00001e70: 7828 7f35 342c 3136 3135 0a20 2020 2075  x(.54,1615.    u
-00001e80: 696e 7433 325f 7420 726f 775f 6e75 6d28  int32_t row_num(
-00001e90: 7f35 372c 3137 3939 0a20 2020 2075 696e  .57,1799.    uin
-00001ea0: 7433 325f 7420 636f 6c5f 6e75 6d28 7f35  t32_t col_num(.5
-00001eb0: 392c 3138 3830 0a20 2020 2073 7464 3a3a  9,1880.    std::
-00001ec0: 7665 6374 6f72 3c73 7464 3a3a 7665 6374  vector<std::vect
-00001ed0: 6f72 3c75 696e 7438 5f74 3e3e 2065 6c65  or<uint8_t>> ele
-00001ee0: 6d65 6e74 7328 7f36 312c 3139 3632 0a20  ments(.61,1962. 
-00001ef0: 2020 2073 7464 3a3a 7665 6374 6f72 3c75     std::vector<u
-00001f00: 696e 7433 325f 743e 2072 6f77 5f69 6e64  int32_t> row_ind
-00001f10: 6578 6573 287f 3633 2c32 3037 350a 2020  exes(.63,2075.  
-00001f20: 2020 766f 6964 2072 6f77 5f6e 756d 287f    void row_num(.
-00001f30: 3635 2c32 3137 380a 2020 2020 766f 6964  65,2178.    void
-00001f40: 2063 6f6c 5f6e 756d 287f 3637 2c32 3237   col_num(.67,227
-00001f50: 340a 2020 2020 766f 6964 2065 6c65 6d65  4.    void eleme
-00001f60: 6e74 7328 7f36 392c 3233 3731 0a20 2020  nts(.69,2371.   
-00001f70: 2076 6f69 6420 726f 775f 696e 6465 7865   void row_indexe
-00001f80: 7328 7f37 312c 3235 3031 0a20 2020 2076  s(.71,2501.    v
-00001f90: 6f69 6420 7365 745f 6964 656e 7469 7479  oid set_identity
-00001fa0: 287f 3832 2c32 3935 340a 2020 2020 766f  (.82,2954.    vo
-00001fb0: 6964 2072 6576 6572 7365 5f65 6c65 6d65  id reverse_eleme
-00001fc0: 6e74 287f 3936 2c33 3335 360a 2020 2020  nt(.96,3356.    
-00001fd0: 7569 6e74 3332 5f74 2078 6f72 5f72 6f77  uint32_t xor_row
-00001fe0: 7328 7f31 3038 2c33 3833 390a 2020 2020  s(.108,3839.    
-00001ff0: 766f 6964 2073 7761 705f 726f 7773 287f  void swap_rows(.
-00002000: 3132 352c 3433 3431 0a20 2020 2076 6f69  125,4341.    voi
-00002010: 6420 7377 6170 5f63 6f6c 7328 7f31 3430  d swap_cols(.140
-00002020: 2c34 3739 300a 2020 2020 626f 6f6c 2066  ,4790.    bool f
-00002030: 6561 7369 626c 6528 7f31 3533 2c35 3138  easible(.153,518
-00002040: 330a 2020 2020 7374 643a 3a76 6563 746f  3.    std::vecto
-00002050: 723c 7f73 7464 3a3a 7665 6374 6f72 0131  r<.std::vector.1
-00002060: 3734 2c35 3733 390a 2020 2020 6672 6965  74,5739.    frie
-00002070: 6e64 2073 7464 3a3a 6f73 7472 6561 6d26  nd std::ostream&
-00002080: 206f 7065 7261 746f 723c 3c28 7f31 3735   operator<<(.175
-00002090: 2c35 3833 320a 0c0a 7369 6d70 6c69 6679  ,5832...simplify
-000020a0: 2e63 7070 2c31 3135 360a 766f 6964 2053  .cpp,1156.void S
-000020b0: 6861 7271 6974 3a3a 5a58 4469 6167 7261  harqit::ZXDiagra
-000020c0: 6d3a 3a66 7573 655f 7370 6964 6572 7328  m::fuse_spiders(
-000020d0: 7f66 7573 655f 7370 6964 6572 7301 382c  .fuse_spiders.8,
-000020e0: 3134 320a 766f 6964 2053 6861 7271 6974  142.void Sharqit
-000020f0: 3a3a 5a58 4469 6167 7261 6d3a 3a63 6f6e  ::ZXDiagram::con
-00002100: 765f 785f 746f 5f7a 287f 636f 6e76 5f78  v_x_to_z(.conv_x
-00002110: 5f74 6f5f 7a01 3638 2c31 3639 360a 766f  _to_z.68,1696.vo
-00002120: 6964 2053 6861 7271 6974 3a3a 5a58 4469  id Sharqit::ZXDi
-00002130: 6167 7261 6d3a 3a72 656d 6f76 655f 7061  agram::remove_pa
-00002140: 7261 6c6c 656c 5f73 656c 666c 6f6f 7073  rallel_selfloops
-00002150: 5f68 6164 616d 6172 645f 6564 6765 7328  _hadamard_edges(
-00002160: 7f72 656d 6f76 655f 7061 7261 6c6c 656c  .remove_parallel
-00002170: 5f73 656c 666c 6f6f 7073 5f68 6164 616d  _selfloops_hadam
-00002180: 6172 645f 6564 6765 7301 3837 2c32 3234  ard_edges.87,224
-00002190: 360a 766f 6964 2053 6861 7271 6974 3a3a  6.void Sharqit::
-000021a0: 5a58 4469 6167 7261 6d3a 3a75 7064 6174  ZXDiagram::updat
-000021b0: 655f 6e6f 6465 5f70 6c61 6365 7328 7f75  e_node_places(.u
-000021c0: 7064 6174 655f 6e6f 6465 5f70 6c61 6365  pdate_node_place
-000021d0: 7301 3131 382c 3333 3434 0a76 6f69 6420  s.118,3344.void 
-000021e0: 5368 6172 7169 743a 3a5a 5844 6961 6772  Sharqit::ZXDiagr
-000021f0: 616d 3a3a 7570 6461 7465 5f70 6861 7365  am::update_phase
-00002200: 5f67 6164 6765 7428 7f75 7064 6174 655f  _gadget(.update_
-00002210: 7068 6173 655f 6761 6467 6574 0131 3432  phase_gadget.142
-00002220: 2c34 3130 360a 766f 6964 2053 6861 7271  ,4106.void Sharq
-00002230: 6974 3a3a 5a58 4469 6167 7261 6d3a 3a67  it::ZXDiagram::g
-00002240: 7261 7068 5f6c 696b 6528 7f67 7261 7068  raph_like(.graph
-00002250: 5f6c 696b 6501 3136 352c 3437 3830 0a76  _like.165,4780.v
-00002260: 6f69 6420 5368 6172 7169 743a 3a5a 5844  oid Sharqit::ZXD
-00002270: 6961 6772 616d 3a3a 6c63 6f6d 705f 6f6e  iagram::lcomp_on
-00002280: 655f 7469 6d65 287f 6c63 6f6d 705f 6f6e  e_time(.lcomp_on
-00002290: 655f 7469 6d65 0132 3238 2c36 3530 300a  e_time.228,6500.
-000022a0: 7569 6e74 3332 5f74 2053 6861 7271 6974  uint32_t Sharqit
-000022b0: 3a3a 5a58 4469 6167 7261 6d3a 3a6c 636f  ::ZXDiagram::lco
-000022c0: 6d70 287f 6c63 6f6d 7001 3234 332c 3639  mp(.lcomp.243,69
-000022d0: 3830 0a76 6f69 6420 5368 6172 7169 743a  80.void Sharqit:
-000022e0: 3a5a 5844 6961 6772 616d 3a3a 7069 766f  :ZXDiagram::pivo
-000022f0: 7431 5f6f 6e65 5f74 696d 6528 7f70 6976  t1_one_time(.piv
-00002300: 6f74 315f 6f6e 655f 7469 6d65 0132 3935  ot1_one_time.295
-00002310: 2c38 3334 360a 7569 6e74 3332 5f74 2053  ,8346.uint32_t S
-00002320: 6861 7271 6974 3a3a 5a58 4469 6167 7261  harqit::ZXDiagra
-00002330: 6d3a 3a70 6976 6f74 3128 7f70 6976 6f74  m::pivot1(.pivot
-00002340: 3101 3335 312c 3130 3237 300a 766f 6964  1.351,10270.void
-00002350: 2053 6861 7271 6974 3a3a 5a58 4469 6167   Sharqit::ZXDiag
-00002360: 7261 6d3a 3a70 6976 6f74 325f 6f6e 655f  ram::pivot2_one_
-00002370: 7469 6d65 287f 7069 766f 7432 5f6f 6e65  time(.pivot2_one
-00002380: 5f74 696d 6501 3433 312c 3132 3238 300a  _time.431,12280.
-00002390: 7569 6e74 3332 5f74 2053 6861 7271 6974  uint32_t Sharqit
-000023a0: 3a3a 5a58 4469 6167 7261 6d3a 3a70 6976  ::ZXDiagram::piv
-000023b0: 6f74 3228 7f70 6976 6f74 3201 3531 312c  ot2(.pivot2.511,
-000023c0: 3134 3937 360a 766f 6964 2053 6861 7271  14976.void Sharq
-000023d0: 6974 3a3a 5a58 4469 6167 7261 6d3a 3a70  it::ZXDiagram::p
-000023e0: 6976 6f74 335f 6f6e 655f 7469 6d65 287f  ivot3_one_time(.
-000023f0: 7069 766f 7433 5f6f 6e65 5f74 696d 6501  pivot3_one_time.
-00002400: 3539 322c 3137 3033 380a 7569 6e74 3332  592,17038.uint32
-00002410: 5f74 2053 6861 7271 6974 3a3a 5a58 4469  _t Sharqit::ZXDi
-00002420: 6167 7261 6d3a 3a70 6976 6f74 3328 7f70  agram::pivot3(.p
-00002430: 6976 6f74 3301 3639 322c 3230 3336 330a  ivot3.692,20363.
-00002440: 766f 6964 2053 6861 7271 6974 3a3a 5a58  void Sharqit::ZX
-00002450: 4469 6167 7261 6d3a 3a69 645f 7265 6d6f  Diagram::id_remo
-00002460: 7661 6c28 7f69 645f 7265 6d6f 7661 6c01  val(.id_removal.
-00002470: 3738 332c 3232 3639 300a 766f 6964 2053  783,22690.void S
-00002480: 6861 7271 6974 3a3a 5a58 4469 6167 7261  harqit::ZXDiagra
-00002490: 6d3a 3a67 6675 7369 6f6e 5f6f 6e65 5f74  m::gfusion_one_t
-000024a0: 696d 6528 7f67 6675 7369 6f6e 5f6f 6e65  ime(.gfusion_one
-000024b0: 5f74 696d 6501 3833 382c 3234 3332 390a  _time.838,24329.
-000024c0: 7569 6e74 3332 5f74 2053 6861 7271 6974  uint32_t Sharqit
-000024d0: 3a3a 5a58 4469 6167 7261 6d3a 3a67 6675  ::ZXDiagram::gfu
-000024e0: 7369 6f6e 287f 6766 7573 696f 6e01 3834  sion(.gfusion.84
-000024f0: 362c 3234 3634 380a 766f 6964 2053 6861  6,24648.void Sha
-00002500: 7271 6974 3a3a 5a58 4469 6167 7261 6d3a  rqit::ZXDiagram:
-00002510: 3a73 696d 706c 6966 7928 7f73 696d 706c  :simplify(.simpl
-00002520: 6966 7901 3937 392c 3238 3434 370a 0c0a  ify.979,28447...
-00002530: 7167 6174 652e 6370 702c 3637 350a 5368  qgate.cpp,675.Sh
-00002540: 6172 7169 743a 3a51 4761 7465 3a3a 5147  arqit::QGate::QG
-00002550: 6174 6528 7f51 4761 7465 0138 2c39 300a  ate(.QGate.8,90.
-00002560: 5368 6172 7169 743a 3a51 4761 7465 3a3a  Sharqit::QGate::
-00002570: 5147 6174 6528 7f51 4761 7465 0135 352c  QGate(.QGate.55,
-00002580: 3133 3337 0a73 7464 3a3a 7665 6374 6f72  1337.std::vector
-00002590: 3c73 7464 3a3a 7665 6374 6f72 3c73 7464  <std::vector<std
-000025a0: 3a3a 636f 6d70 6c65 783c 646f 7562 6c65  ::complex<double
-000025b0: 3e3e 3e20 5368 6172 7169 743a 3a51 4761  >>> Sharqit::QGa
-000025c0: 7465 3a3a 6b69 6e64 5f74 6f5f 6f70 287f  te::kind_to_op(.
-000025d0: 6b69 6e64 5f74 6f5f 6f70 0137 332c 3138  kind_to_op.73,18
-000025e0: 3637 0a73 7464 3a3a 7374 7269 6e67 2053  67.std::string S
-000025f0: 6861 7271 6974 3a3a 5147 6174 653a 3a6e  harqit::QGate::n
-00002600: 616d 6528 7f6e 616d 6501 3133 392c 3335  ame(.name.139,35
-00002610: 3130 0a73 7464 3a3a 7374 7269 6e67 2053  10.std::string S
-00002620: 6861 7271 6974 3a3a 5147 6174 653a 3a74  harqit::QGate::t
-00002630: 6f5f 7374 7269 6e67 287f 746f 5f73 7472  o_string(.to_str
-00002640: 696e 6701 3134 382c 3338 3132 0a73 7464  ing.148,3812.std
-00002650: 3a3a 7475 706c 653c 5368 6172 7169 743a  ::tuple<Sharqit:
-00002660: 3a51 4761 7465 4b69 6e64 2c20 5368 6172  :QGateKind, Shar
-00002670: 7169 743a 3a50 6861 7365 3e20 5368 6172  qit::Phase> Shar
-00002680: 7169 743a 3a51 4761 7465 3a3a 6b69 6e64  qit::QGate::kind
-00002690: 5f70 6861 7365 287f 6b69 6e64 5f70 6861  _phase(.kind_pha
-000026a0: 7365 0131 3637 2c34 3131 330a 5368 6172  se.167,4113.Shar
-000026b0: 7169 743a 3a51 4761 7465 2053 6861 7271  qit::QGate Sharq
-000026c0: 6974 3a3a 5147 6174 653a 3a69 6e76 6572  it::QGate::inver
-000026d0: 7365 287f 696e 7665 7273 6501 3233 362c  se(.inverse.236,
-000026e0: 3537 3831 0a62 6f6f 6c20 5368 6172 7169  5781.bool Sharqi
-000026f0: 743a 3a51 4761 7465 3a3a 6973 5f69 6465  t::QGate::is_ide
-00002700: 6e74 6963 616c 287f 6973 5f69 6465 6e74  ntical(.is_ident
-00002710: 6963 616c 0133 3037 2c37 3938 300a 626f  ical.307,7980.bo
-00002720: 6f6c 2053 6861 7271 6974 3a3a 5147 6174  ol Sharqit::QGat
-00002730: 653a 3a6f 7665 726c 6170 287f 6f76 6572  e::overlap(.over
-00002740: 6c61 7001 3332 302c 3834 3036 0a62 6f6f  lap.320,8406.boo
-00002750: 6c20 5368 6172 7169 743a 3a51 4761 7465  l Sharqit::QGate
-00002760: 3a3a 6d65 7267 6561 626c 6528 7f6d 6572  ::mergeable(.mer
-00002770: 6765 6162 6c65 0133 3334 2c38 3635 370a  geable.334,8657.
-00002780: 626f 6f6c 2053 6861 7271 6974 3a3a 5147  bool Sharqit::QG
-00002790: 6174 653a 3a63 6f6d 6d75 7461 626c 6528  ate::commutable(
-000027a0: 7f63 6f6d 6d75 7461 626c 6501 3335 312c  .commutable.351,
-000027b0: 3933 3934 0a76 6f69 6420 5368 6172 7169  9394.void Sharqi
-000027c0: 743a 3a51 4761 7465 3a3a 6d65 7267 6528  t::QGate::merge(
-000027d0: 7f6d 6572 6765 0133 3935 2c31 3132 3939  .merge.395,11299
-000027e0: 0a0c 0a64 6167 6564 6765 2e63 7070 2c34  ...dagedge.cpp,4
-000027f0: 360a 7374 643a 3a73 7472 696e 6720 5368  6.std::string Sh
-00002800: 6172 7169 743a 3a44 4147 4564 6765 3a3a  arqit::DAGEdge::
-00002810: 6e61 6d65 287f 6e61 6d65 0138 2c39 320a  name(.name.8,92.
-00002820: 0c0a 7167 6174 652e 682c 3133 3835 0a23  ..qgate.h,1385.#
-00002830: 6465 6669 6e65 2051 4741 5445 5f48 7f37  define QGATE_H.7
-00002840: 2c38 300a 2020 656e 756d 2051 4761 7465  ,80.  enum QGate
-00002850: 4b69 6e64 207f 3139 2c32 3431 0a09 0920  Kind .19,241... 
-00002860: 2058 2c7f 3230 2c32 3630 0a09 0920 205a   X,.20,260...  Z
-00002870: 2c7f 3231 2c32 3835 0a09 0920 2053 2c7f  ,.21,285...  S,.
-00002880: 3232 2c33 3130 0a09 0920 2053 6467 2c7f  22,310...  Sdg,.
-00002890: 3233 2c33 3239 0a09 0920 2054 2c7f 3234  23,329...  T,.24
-000028a0: 2c33 3834 0a09 0920 2054 6467 2c7f 3235  ,384...  Tdg,.25
-000028b0: 2c34 3033 0a09 0920 2048 2c7f 3236 2c34  ,403...  H,.26,4
-000028c0: 3538 0a09 0920 2052 5a2c 7f32 372c 3438  58...  RZ,.27,48
-000028d0: 380a 0909 2020 4358 2c7f 3238 2c35 3039  8...  CX,.28,509
-000028e0: 0a09 0920 2043 5a2c 7f32 392c 3533 320a  ...  CZ,.29,532.
-000028f0: 0909 2020 4964 2c7f 3330 2c35 3533 0a09  ..  Id,.30,553..
-00002900: 0920 2049 6432 207f 3331 2c35 3933 0a20  .  Id2 .31,593. 
-00002910: 2063 6c61 7373 2051 4761 7465 7f33 382c   class QGate.38,
-00002920: 3639 300a 2020 2020 5147 6174 654b 696e  690.    QGateKin
-00002930: 6420 6b69 6e64 5f3b 7f34 312c 3731 390a  d kind_;.41,719.
-00002940: 2020 2020 7374 643a 3a76 6563 746f 723c      std::vector<
-00002950: 7569 6e74 3332 5f74 3e20 7169 645f 3b7f  uint32_t> qid_;.
-00002960: 3432 2c37 3636 0a20 2020 2050 6861 7365  42,766.    Phase
-00002970: 2070 6861 7365 5f3b 7f34 332c 3832 370a   phase_;.43,827.
-00002980: 2020 2020 7374 643a 3a76 6563 746f 723c      std::vector<
-00002990: 7374 643a 3a76 6563 746f 723c 7374 643a  std::vector<std:
-000029a0: 3a63 6f6d 706c 6578 3c64 6f75 626c 653e  :complex<double>
-000029b0: 3e3e 206f 705f 3b7f 3434 2c38 3733 0a20  >> op_;.44,873. 
-000029c0: 2020 2051 4761 7465 287f 3730 2c32 3031     QGate(.70,201
-000029d0: 310a 2020 2020 5147 6174 654b 696e 6420  1.    QGateKind 
-000029e0: 6b69 6e64 287f 3732 2c32 3134 390a 2020  kind(.72,2149.  
-000029f0: 2020 7374 643a 3a76 6563 746f 723c 7569    std::vector<ui
-00002a00: 6e74 3332 5f74 3e20 7169 6428 7f37 342c  nt32_t> qid(.74,
-00002a10: 3232 3231 0a20 2020 2050 6861 7365 2070  2221.    Phase p
-00002a20: 6861 7365 287f 3736 2c32 3330 350a 2020  hase(.76,2305.  
-00002a30: 2020 7374 643a 3a76 6563 746f 723c 7374    std::vector<st
-00002a40: 643a 3a76 6563 746f 723c 7374 643a 3a63  d::vector<std::c
-00002a50: 6f6d 706c 6578 3c64 6f75 626c 653e 3e3e  omplex<double>>>
-00002a60: 206f 7028 7f37 382c 3233 3734 0a20 2020   op(.78,2374.   
-00002a70: 2076 6f69 6420 6b69 6e64 287f 3830 2c32   void kind(.80,2
-00002a80: 3438 300a 2020 2020 766f 6964 2071 6964  480.    void qid
-00002a90: 287f 3832 2c32 3536 310a 2020 2020 766f  (.82,2561.    vo
-00002aa0: 6964 2070 6861 7365 287f 3834 2c32 3635  id phase(.84,265
-00002ab0: 330a 2020 2020 766f 6964 206f 7028 7f38  3.    void op(.8
-00002ac0: 362c 3237 3334 0a20 2020 2075 696e 7433  6,2734.    uint3
-00002ad0: 325f 7420 7175 6269 745f 6e75 6d28 7f31  2_t qubit_num(.1
-00002ae0: 3033 2c33 3336 330a 2020 2020 626f 6f6c  03,3363.    bool
-00002af0: 2069 735f 4964 5f67 6174 6528 7f31 3038   is_Id_gate(.108
-00002b00: 2c33 3535 370a 2020 2020 626f 6f6c 2069  ,3557.    bool i
-00002b10: 735f 4964 325f 6761 7465 287f 3131 332c  s_Id2_gate(.113,
-00002b20: 3337 3535 0a20 2020 2062 6f6f 6c20 6973  3755.    bool is
-00002b30: 5f58 5f67 6174 6528 7f31 3138 2c33 3933  _X_gate(.118,393
-00002b40: 320a 2020 2020 626f 6f6c 2069 735f 5a5f  2.    bool is_Z_
-00002b50: 6761 7465 287f 3132 332c 3431 3332 0a20  gate(.123,4132. 
-00002b60: 2020 2062 6f6f 6c20 6973 5f48 5f67 6174     bool is_H_gat
-00002b70: 6528 7f31 3333 2c34 3432 300a 2020 2020  e(.133,4420.    
-00002b80: 626f 6f6c 2069 735f 535f 6761 7465 287f  bool is_S_gate(.
-00002b90: 3133 382c 3436 3237 0a20 2020 2062 6f6f  138,4627.    boo
-00002ba0: 6c20 6973 5f53 315f 6761 7465 287f 3135  l is_S1_gate(.15
-00002bb0: 312c 3530 3234 0a20 2020 2062 6f6f 6c20  1,5024.    bool 
-00002bc0: 6973 5f53 335f 6761 7465 287f 3136 322c  is_S3_gate(.162,
-00002bd0: 3533 3537 0a20 2020 2062 6f6f 6c20 6973  5357.    bool is
-00002be0: 5f54 5f67 6174 6528 7f31 3733 2c35 3730  _T_gate(.173,570
-00002bf0: 350a 2020 2020 626f 6f6c 2069 735f 5431  5.    bool is_T1
-00002c00: 5f67 6174 6528 7f31 3836 2c36 3130 320a  _gate(.186,6102.
-00002c10: 2020 2020 626f 6f6c 2069 735f 5437 5f67      bool is_T7_g
-00002c20: 6174 6528 7f31 3939 2c36 3435 320a 2020  ate(.199,6452.  
-00002c30: 2020 626f 6f6c 2069 735f 4358 5f67 6174    bool is_CX_gat
-00002c40: 6528 7f32 3132 2c36 3738 300a 2020 2020  e(.212,6780.    
-00002c50: 626f 6f6c 2069 735f 435a 5f67 6174 6528  bool is_CZ_gate(
-00002c60: 7f32 3137 2c36 3934 350a 2020 2020 626f  .217,6945.    bo
-00002c70: 6f6c 2069 735f 525a 5f67 6174 6528 7f32  ol is_RZ_gate(.2
-00002c80: 3232 2c37 3131 300a 2020 2020 626f 6f6c  22,7110.    bool
-00002c90: 2069 735f 7061 756c 695f 6761 7465 287f   is_pauli_gate(.
-00002ca0: 3232 392c 3734 3536 0a20 2020 2062 6f6f  229,7456.    boo
-00002cb0: 6c20 6973 5f70 726f 7065 725f 636c 6966  l is_proper_clif
-00002cc0: 666f 7264 5f67 6174 6528 7f32 3334 2c37  ford_gate(.234,7
-00002cd0: 3637 300a 2020 2020 626f 6f6c 2069 735f  670.    bool is_
-00002ce0: 636c 6966 666f 7264 5f67 6174 6528 7f32  clifford_gate(.2
-00002cf0: 3339 2c37 3834 370a 2020 2020 626f 6f6c  39,7847.    bool
-00002d00: 2069 735f 6e6f 6e5f 636c 6966 666f 7264   is_non_clifford
-00002d10: 5f67 6174 6528 7f32 3434 2c38 3037 360a  _gate(.244,8076.
-00002d20: 2020 2020 626f 6f6c 2069 735f 696e 636c      bool is_incl
-00002d30: 7564 6564 287f 3235 302c 3833 3031 0a20  uded(.250,8301. 
-00002d40: 2020 2073 7461 7469 6320 7374 643a 3a74     static std::t
-00002d50: 7570 6c65 3c7f 7374 643a 3a74 7570 6c65  uple<.std::tuple
-00002d60: 0132 3934 2c39 3732 380a 2020 2020 6672  .294,9728.    fr
-00002d70: 6965 6e64 2073 7464 3a3a 6f73 7472 6561  iend std::ostrea
-00002d80: 6d26 206f 7065 7261 746f 723c 3c28 7f32  m& operator<<(.2
-00002d90: 3935 2c39 3830 340a 0c0a 6461 676e 6f64  95,9804...dagnod
-00002da0: 652e 6370 702c 3436 0a73 7464 3a3a 7374  e.cpp,46.std::st
-00002db0: 7269 6e67 2053 6861 7271 6974 3a3a 4441  ring Sharqit::DA
-00002dc0: 474e 6f64 653a 3a6e 616d 6528 7f6e 616d  GNode::name(.nam
-00002dd0: 6501 382c 3932 0a0c 0a64 6167 2e68 2c31  e.8,92...dag.h,1
-00002de0: 3839 330a 2364 6566 696e 6520 4441 475f  893.#define DAG_
-00002df0: 487f 372c 3133 370a 2020 656e 756d 2044  H.7,137.  enum D
-00002e00: 4147 4e6f 6465 4b69 6e64 207f 3232 2c33  AGNodeKind .22,3
-00002e10: 3239 0a09 0920 2020 204f 704e 6f64 652c  29...    OpNode,
-00002e20: 7f32 332c 3335 300a 0909 2020 2020 496e  .23,350...    In
-00002e30: 4e6f 6465 2c7f 3234 2c34 3031 0a09 0920  Node,.24,401... 
-00002e40: 2020 204f 7574 4e6f 6465 207f 3235 2c34     OutNode .25,4
-00002e50: 3331 0a20 2065 6e75 6d20 4441 4745 6467  31.  enum DAGEdg
-00002e60: 654b 696e 6420 7f32 382c 3439 330a 0909  eKind .28,493...
-00002e70: 2020 2020 466f 7277 6172 642c 7f32 392c      Forward,.29,
-00002e80: 3531 340a 0909 2020 2020 4261 636b 7761  514...    Backwa
-00002e90: 7264 207f 3330 2c35 3532 0a20 2063 6c61  rd .30,552.  cla
-00002ea0: 7373 2044 4147 4e6f 6465 7f33 392c 3731  ss DAGNode.39,71
-00002eb0: 330a 2020 2020 4441 474e 6f64 654b 696e  3.    DAGNodeKin
-00002ec0: 6420 6b69 6e64 5f3b 7f34 322c 3734 340a  d kind_;.42,744.
-00002ed0: 2020 2020 5147 6174 6520 7167 6174 655f      QGate qgate_
-00002ee0: 3b7f 3433 2c37 3839 0a20 2020 2044 4147  ;.43,789.    DAG
-00002ef0: 4e6f 6465 287f 3530 2c31 3030 310a 2020  Node(.50,1001.  
-00002f00: 2020 4441 474e 6f64 6528 7f35 362c 3132    DAGNode(.56,12
-00002f10: 3236 0a20 2020 2044 4147 4e6f 6465 4b69  26.    DAGNodeKi
-00002f20: 6e64 206b 696e 6428 7f35 382c 3133 3331  nd kind(.58,1331
-00002f30: 0a20 2020 2051 4761 7465 2071 6761 7465  .    QGate qgate
-00002f40: 287f 3630 2c31 3430 370a 2020 2020 766f  (.60,1407.    vo
-00002f50: 6964 206b 696e 6428 7f36 322c 3134 3738  id kind(.62,1478
-00002f60: 0a20 2020 2076 6f69 6420 7167 6174 6528  .    void qgate(
-00002f70: 7f36 342c 3135 3633 0a20 2020 2075 696e  .64,1563.    uin
-00002f80: 7433 325f 7420 7175 6269 745f 6e75 6d28  t32_t qubit_num(
-00002f90: 7f37 342c 3138 3934 0a20 2020 2073 7464  .74,1894.    std
-00002fa0: 3a3a 7665 6374 6f72 3c75 696e 7433 325f  ::vector<uint32_
-00002fb0: 743e 2071 6964 287f 3739 2c32 3130 380a  t> qid(.79,2108.
-00002fc0: 2020 2020 626f 6f6c 2069 735f 696e 6e6f      bool is_inno
-00002fd0: 6465 287f 3834 2c32 3330 320a 2020 2020  de(.84,2302.    
-00002fe0: 626f 6f6c 2069 735f 6f75 746e 6f64 6528  bool is_outnode(
-00002ff0: 7f38 392c 3235 3138 0a20 2020 2062 6f6f  .89,2518.    boo
-00003000: 6c20 6973 5f6f 706e 6f64 6528 7f39 342c  l is_opnode(.94,
-00003010: 3237 3732 0a20 2020 2062 6f6f 6c20 6973  2772.    bool is
-00003020: 5f69 6465 6e74 6974 7928 7f39 392c 3330  _identity(.99,30
-00003030: 3038 0a20 2020 2062 6f6f 6c20 6973 5f68  08.    bool is_h
-00003040: 6164 616d 6172 6428 7f31 3035 2c33 3238  adamard(.105,328
-00003050: 320a 2020 2020 626f 6f6c 2069 735f 726f  2.    bool is_ro
-00003060: 7461 7469 6f6e 287f 3131 302c 3334 3833  tation(.110,3483
-00003070: 0a20 2020 2062 6f6f 6c20 6973 5f63 6e6f  .    bool is_cno
-00003080: 7428 7f31 3135 2c33 3637 370a 2020 2020  t(.115,3677.    
-00003090: 626f 6f6c 2069 735f 696e 636c 7564 6564  bool is_included
-000030a0: 287f 3132 312c 3339 3532 0a20 2020 2062  (.121,3952.    b
-000030b0: 6f6f 6c20 6d65 7267 6561 626c 6528 7f31  ool mergeable(.1
-000030c0: 3331 2c34 3239 380a 2020 2020 626f 6f6c  31,4298.    bool
-000030d0: 2063 6f6d 6d75 7461 626c 6528 7f31 3337   commutable(.137
-000030e0: 2c34 3630 360a 2020 2020 766f 6964 206d  ,4606.    void m
-000030f0: 6572 6765 287f 3134 332c 3438 3730 0a20  erge(.143,4870. 
-00003100: 2063 6c61 7373 2044 4147 4564 6765 7f31   class DAGEdge.1
-00003110: 3531 2c35 3034 340a 2020 2020 4441 4745  51,5044.    DAGE
-00003120: 6467 654b 696e 6420 6b69 6e64 5f3b 7f31  dgeKind kind_;.1
-00003130: 3534 2c35 3037 350a 2020 2020 7569 6e74  54,5075.    uint
-00003140: 3332 5f74 2071 5f3b 7f31 3535 2c35 3134  32_t q_;.155,514
-00003150: 380a 2020 2020 7569 6e74 3332 5f74 2074  8.    uint32_t t
-00003160: 6f5f 3b7f 3135 362c 3531 3939 0a20 2020  o_;.156,5199.   
-00003170: 2044 4147 4564 6765 287f 3136 342c 3534   DAGEdge(.164,54
-00003180: 3630 0a20 2020 2044 4147 4564 6765 287f  60.    DAGEdge(.
-00003190: 3137 302c 3537 3132 0a20 2020 2044 4147  170,5712.    DAG
-000031a0: 4564 6765 4b69 6e64 206b 696e 6428 7f31  EdgeKind kind(.1
-000031b0: 3732 2c35 3832 340a 2020 2020 7569 6e74  72,5824.    uint
-000031c0: 3332 5f74 2071 287f 3137 342c 3538 3936  32_t q(.174,5896
-000031d0: 0a20 2020 2075 696e 7433 325f 7420 746f  .    uint32_t to
-000031e0: 287f 3137 362c 3539 3630 0a20 2020 2076  (.176,5960.    v
-000031f0: 6f69 6420 6b69 6e64 287f 3137 382c 3630  oid kind(.178,60
-00003200: 3238 0a20 2020 2076 6f69 6420 7128 7f31  28.    void q(.1
-00003210: 3830 2c36 3130 330a 2020 2020 766f 6964  80,6103.    void
-00003220: 2074 6f28 7f31 3832 2c36 3136 340a 2020   to(.182,6164.  
-00003230: 2020 626f 6f6c 2069 735f 666f 7277 6172    bool is_forwar
-00003240: 6428 7f31 3932 2c36 3435 350a 2020 2020  d(.192,6455.    
-00003250: 626f 6f6c 2069 735f 6261 636b 7761 7264  bool is_backward
-00003260: 287f 3139 372c 3636 3733 0a20 2063 6c61  (.197,6673.  cla
-00003270: 7373 2044 4147 4369 7263 7f32 3036 2c36  ss DAGCirc.206,6
-00003280: 3839 300a 2020 2020 7569 6e74 3332 5f74  890.    uint32_t
-00003290: 2071 7562 6974 5f6e 756d 5f3b 7f32 3039   qubit_num_;.209
-000032a0: 2c36 3932 310a 2020 2020 7374 643a 3a76  ,6921.    std::v
-000032b0: 6563 746f 723c 4441 474e 6f64 653e 206e  ector<DAGNode> n
-000032c0: 6f64 6573 5f3b 7f32 3130 2c36 3936 380a  odes_;.210,6968.
-000032d0: 2020 2020 7374 643a 3a76 6563 746f 723c      std::vector<
-000032e0: 7569 6e74 3332 5f74 3e20 696e 7075 7473  uint32_t> inputs
-000032f0: 5f3b 7f32 3131 2c37 3033 360a 2020 2020  _;.211,7036.    
-00003300: 7374 643a 3a76 6563 746f 723c 7569 6e74  std::vector<uint
-00003310: 3332 5f74 3e20 6f75 7470 7574 735f 3b7f  32_t> outputs_;.
-00003320: 3231 322c 3731 3039 0a20 2020 2073 7464  212,7109.    std
-00003330: 3a3a 7665 6374 6f72 3c73 7464 3a3a 7665  ::vector<std::ve
-00003340: 6374 6f72 3c44 4147 4564 6765 3e3e 2061  ctor<DAGEdge>> a
-00003350: 646a 5f6d 6174 5f3b 7f32 3133 2c37 3138  dj_mat_;.213,718
-00003360: 340a 2020 2020 4441 4743 6972 6328 7f32  4.    DAGCirc(.2
-00003370: 3637 2c39 3539 310a 2020 2020 7569 6e74  67,9591.    uint
-00003380: 3332 5f74 2071 7562 6974 5f6e 756d 287f  32_t qubit_num(.
-00003390: 3237 312c 3937 3833 0a20 2020 2073 7464  271,9783.    std
-000033a0: 3a3a 7665 6374 6f72 3c44 4147 4e6f 6465  ::vector<DAGNode
-000033b0: 3e20 6e6f 6465 7328 7f32 3733 2c39 3836  > nodes(.273,986
-000033c0: 360a 2020 2020 7374 643a 3a76 6563 746f  6.    std::vecto
-000033d0: 723c 7569 6e74 3332 5f74 3e20 696e 7075  r<uint32_t> inpu
-000033e0: 7473 287f 3237 352c 3939 3534 0a20 2020  ts(.275,9954.   
-000033f0: 2073 7464 3a3a 7665 6374 6f72 3c75 696e   std::vector<uin
-00003400: 7433 325f 743e 206f 7574 7075 7473 287f  t32_t> outputs(.
-00003410: 3237 372c 3130 3034 360a 2020 2020 7374  277,10046.    st
-00003420: 643a 3a76 6563 746f 723c 7374 643a 3a76  d::vector<std::v
-00003430: 6563 746f 723c 4441 4745 6467 653e 3e20  ector<DAGEdge>> 
-00003440: 6164 6a5f 6d61 7428 7f32 3739 2c31 3031  adj_mat(.279,101
-00003450: 3430 0a20 2020 2076 6f69 6420 7175 6269  40.    void qubi
-00003460: 745f 6e75 6d28 7f32 3831 2c31 3032 3438  t_num(.281,10248
-00003470: 0a20 2020 2076 6f69 6420 6e6f 6465 7328  .    void nodes(
-00003480: 7f32 3833 2c31 3033 3530 0a20 2020 2076  .283,10350.    v
-00003490: 6f69 6420 696e 7075 7473 287f 3238 352c  oid inputs(.285,
-000034a0: 3130 3435 300a 2020 2020 766f 6964 206f  10450.    void o
-000034b0: 7574 7075 7473 287f 3238 372c 3130 3535  utputs(.287,1055
-000034c0: 360a 2020 2020 766f 6964 2061 646a 5f6d  6.    void adj_m
-000034d0: 6174 287f 3238 392c 3130 3636 360a 2020  at(.289,10666.  
-000034e0: 2020 766f 6964 2073 686f 7728 7f32 3938    void show(.298
-000034f0: 2c31 3039 3635 0a20 2020 2075 696e 7433  ,10965.    uint3
-00003500: 325f 7420 6761 7465 5f63 6f75 6e74 287f  2_t gate_count(.
-00003510: 3330 322c 3131 3036 340a 2020 2020 6672  302,11064.    fr
-00003520: 6965 6e64 2073 7464 3a3a 6f73 7472 6561  iend std::ostrea
-00003530: 6d26 206f 7065 7261 746f 723c 3c28 7f33  m& operator<<(.3
-00003540: 3934 2c31 3438 3438 0a0c 0a73 6861 7271  94,14848...sharq
-00003550: 6974 2e68 2c34 390a 2364 6566 696e 6520  it.h,49.#define 
-00003560: 5348 4152 5149 545f 487f 372c 3838 0a6e  SHARQIT_H.7,88.n
-00003570: 616d 6573 7061 6365 2053 6861 7271 6974  amespace Sharqit
-00003580: 207f 3139 2c32 3934 0a0c 0a6d 6572 6765   .19,294...merge
-00003590: 5f72 6f74 6174 696f 6e2e 6370 702c 3230  _rotation.cpp,20
-000035a0: 390a 626f 6f6c 2053 6861 7271 6974 3a3a  9.bool Sharqit::
-000035b0: 5143 6972 633a 3a69 735f 7465 726d 696e  QCirc::is_termin
-000035c0: 6174 696f 6e5f 626f 7264 6572 287f 6973  ation_border(.is
-000035d0: 5f74 6572 6d69 6e61 7469 6f6e 5f62 6f72  _termination_bor
-000035e0: 6465 7201 382c 3134 380a 766f 6964 2053  der.8,148.void S
-000035f0: 6861 7271 6974 3a3a 5143 6972 633a 3a6d  harqit::QCirc::m
-00003600: 6572 6765 5f72 6f74 6174 696f 6e5f 6f6e  erge_rotation_on
-00003610: 655f 7469 6d65 287f 6d65 7267 655f 726f  e_time(.merge_ro
-00003620: 7461 7469 6f6e 5f6f 6e65 5f74 696d 6501  tation_one_time.
-00003630: 3138 2c34 3132 0a76 6f69 6420 5368 6172  18,412.void Shar
-00003640: 7169 743a 3a51 4369 7263 3a3a 6d65 7267  qit::QCirc::merg
-00003650: 655f 726f 7461 7469 6f6e 287f 6d65 7267  e_rotation(.merg
-00003660: 655f 726f 7461 7469 6f6e 0138 322c 3236  e_rotation.82,26
-00003670: 3031 0a0c 0a6f 7074 696d 697a 6572 2e68  01...optimizer.h
-00003680: 2c31 3232 330a 2364 6566 696e 6520 4f50  ,1223.#define OP
-00003690: 5449 4d49 5a45 525f 487f 372c 3932 0a20  TIMIZER_H.7,92. 
-000036a0: 2065 6e75 6d20 4f70 7469 6d69 7a65 724b   enum OptimizerK
-000036b0: 696e 6420 7f31 392c 3235 310a 0909 2020  ind .19,251...  
-000036c0: 2020 2020 5a58 4361 6c63 756c 7573 2c7f      ZXCalculus,.
-000036d0: 3230 2c32 3734 0a09 0920 2020 2020 2050  20,274...      P
-000036e0: 6861 7365 506f 6c79 6e6f 6d69 616c 207f  hasePolynomial .
-000036f0: 3231 2c33 3137 0a20 2063 6c61 7373 204f  21,317.  class O
-00003700: 7074 696d 697a 6572 7f32 382c 3434 350a  ptimizer.28,445.
-00003710: 2020 2020 4f70 7469 6d69 7a65 724b 696e      OptimizerKin
-00003720: 6420 6b69 6e64 5f3b 7f33 312c 3437 380a  d kind_;.31,478.
-00003730: 2020 2020 646f 7562 6c65 2070 726f 635f      double proc_
-00003740: 7469 6d65 5f3b 7f33 322c 3533 360a 2020  time_;.32,536.  
-00003750: 2020 7374 643a 3a6d 6170 3c7f 7374 643a    std::map<.std:
-00003760: 3a6d 6170 0133 332c 3538 300a 2020 2020  :map.33,580.    
-00003770: 7374 643a 3a6d 6170 3c73 7464 3a3a 7374  std::map<std::st
-00003780: 7269 6e67 2c20 7569 6e74 3332 5f74 3e20  ring, uint32_t> 
-00003790: 7374 6174 735f 696e 5f3b 7f33 332c 3538  stats_in_;.33,58
-000037a0: 300a 2020 2020 7374 643a 3a6d 6170 3c7f  0.    std::map<.
-000037b0: 7374 643a 3a6d 6170 0133 342c 3637 330a  std::map.34,673.
-000037c0: 2020 2020 7374 643a 3a6d 6170 3c73 7464      std::map<std
-000037d0: 3a3a 7374 7269 6e67 2c20 7569 6e74 3332  ::string, uint32
-000037e0: 5f74 3e20 7374 6174 735f 6f75 745f 3b7f  _t> stats_out_;.
-000037f0: 3334 2c36 3733 0a20 2020 2073 7464 3a3a  34,673.    std::
-00003800: 6d61 703c 7f73 7464 3a3a 6d61 7001 3335  map<.std::map.35
-00003810: 2c37 3636 0a20 2020 2073 7464 3a3a 6d61  ,766.    std::ma
-00003820: 703c 7374 643a 3a73 7472 696e 672c 2075  p<std::string, u
-00003830: 696e 7433 325f 743e 207a 785f 7374 6174  int32_t> zx_stat
-00003840: 735f 696e 5f3b 7f33 352c 3736 360a 2020  s_in_;.35,766.  
-00003850: 2020 7374 643a 3a6d 6170 3c7f 7374 643a    std::map<.std:
-00003860: 3a6d 6170 0133 362c 3836 370a 2020 2020  :map.36,867.    
-00003870: 7374 643a 3a6d 6170 3c73 7464 3a3a 7374  std::map<std::st
-00003880: 7269 6e67 2c20 7569 6e74 3332 5f74 3e20  ring, uint32_t> 
-00003890: 7a78 5f73 7461 7473 5f6f 7574 5f3b 7f33  zx_stats_out_;.3
-000038a0: 362c 3836 370a 2020 2020 4f70 7469 6d69  6,867.    Optimi
-000038b0: 7a65 724b 696e 6420 6b69 6e64 287f 3339  zerKind kind(.39
-000038c0: 2c31 3030 360a 2020 2020 646f 7562 6c65  ,1006.    double
-000038d0: 2070 726f 635f 7469 6d65 287f 3431 2c31   proc_time(.41,1
-000038e0: 3038 380a 2020 2020 646f 7562 6c65 2067  088.    double g
-000038f0: 6574 5f70 726f 635f 7469 6d65 287f 3433  et_proc_time(.43
-00003900: 2c31 3137 330a 2020 2020 7374 643a 3a6d  ,1173.    std::m
-00003910: 6170 3c7f 7374 643a 3a6d 6170 0134 352c  ap<.std::map.45,
-00003920: 3132 3631 0a20 2020 2073 7464 3a3a 6d61  1261.    std::ma
-00003930: 703c 7374 643a 3a73 7472 696e 672c 2075  p<std::string, u
-00003940: 696e 7433 325f 743e 2073 7461 7473 5f69  int32_t> stats_i
-00003950: 6e28 7f34 352c 3132 3631 0a20 2020 2073  n(.45,1261.    s
-00003960: 7464 3a3a 6d61 703c 7f73 7464 3a3a 6d61  td::map<.std::ma
-00003970: 7001 3437 2c31 3337 330a 2020 2020 7374  p.47,1373.    st
-00003980: 643a 3a6d 6170 3c73 7464 3a3a 7374 7269  d::map<std::stri
-00003990: 6e67 2c20 7569 6e74 3332 5f74 3e20 7374  ng, uint32_t> st
-000039a0: 6174 735f 6f75 7428 7f34 372c 3133 3733  ats_out(.47,1373
-000039b0: 0a20 2020 2073 7464 3a3a 6d61 703c 7f73  .    std::map<.s
-000039c0: 7464 3a3a 6d61 7001 3439 2c31 3438 390a  td::map.49,1489.
-000039d0: 2020 2020 7374 643a 3a6d 6170 3c73 7464      std::map<std
-000039e0: 3a3a 7374 7269 6e67 2c20 7569 6e74 3332  ::string, uint32
-000039f0: 5f74 3e20 7a78 5f73 7461 7473 5f69 6e28  _t> zx_stats_in(
-00003a00: 7f34 392c 3134 3839 0a20 2020 2073 7464  .49,1489.    std
-00003a10: 3a3a 6d61 703c 7f73 7464 3a3a 6d61 7001  ::map<.std::map.
-00003a20: 3531 2c31 3631 300a 2020 2020 7374 643a  51,1610.    std:
-00003a30: 3a6d 6170 3c73 7464 3a3a 7374 7269 6e67  :map<std::string
-00003a40: 2c20 7569 6e74 3332 5f74 3e20 7a78 5f73  , uint32_t> zx_s
-00003a50: 7461 7473 5f6f 7574 287f 3531 2c31 3631  tats_out(.51,161
-00003a60: 300a 2020 2020 766f 6964 206b 696e 6428  0.    void kind(
-00003a70: 7f35 332c 3137 3235 0a20 2020 2076 6f69  .53,1725.    voi
-00003a80: 6420 7072 6f63 5f74 696d 6528 7f35 352c  d proc_time(.55,
-00003a90: 3138 3136 0a20 2020 2076 6f69 6420 7374  1816.    void st
-00003aa0: 6174 735f 696e 287f 3537 2c31 3931 390a  ats_in(.57,1919.
-00003ab0: 2020 2020 766f 6964 2073 7461 7473 5f6f      void stats_o
-00003ac0: 7574 287f 3539 2c32 3034 350a 2020 2020  ut(.59,2045.    
-00003ad0: 766f 6964 207a 785f 7374 6174 735f 696e  void zx_stats_in
-00003ae0: 287f 3631 2c32 3137 360a 2020 2020 766f  (.61,2176.    vo
-00003af0: 6964 207a 785f 7374 6174 735f 6f75 7428  id zx_stats_out(
-00003b00: 7f36 332c 3233 3137 0a20 2020 2076 6f69  .63,2317.    voi
-00003b10: 6420 7368 6f77 287f 3737 2c32 3737 340a  d show(.77,2774.
-00003b20: 2020 2020 6672 6965 6e64 2073 7464 3a3a      friend std::
-00003b30: 6f73 7472 6561 6d26 206f 7065 7261 746f  ostream& operato
-00003b40: 723c 3c28 7f38 382c 3333 3039 0a0c 0a7a  r<<(.88,3309...z
-00003b50: 786e 6f64 652e 6370 702c 3435 0a73 7464  xnode.cpp,45.std
-00003b60: 3a3a 7374 7269 6e67 2053 6861 7271 6974  ::string Sharqit
-00003b70: 3a3a 5a58 4e6f 6465 3a3a 6e61 6d65 287f  ::ZXNode::name(.
-00003b80: 6e61 6d65 0138 2c38 390a 0c0a 7163 6972  name.8,89...qcir
-00003b90: 632e 6370 702c 3137 3237 0a76 6f69 6420  c.cpp,1727.void 
-00003ba0: 5368 6172 7169 743a 3a51 4369 7263 3a3a  Sharqit::QCirc::
-00003bb0: 7361 7665 287f 7361 7665 0138 2c39 390a  save(.save.8,99.
-00003bc0: 766f 6964 2053 6861 7271 6974 3a3a 5143  void Sharqit::QC
-00003bd0: 6972 633a 3a6c 6f61 6428 7f6c 6f61 6401  irc::load(.load.
-00003be0: 3230 2c33 3136 0a73 7464 3a3a 6d61 703c  20,316.std::map<
-00003bf0: 7374 643a 3a73 7472 696e 672c 2075 696e  std::string, uin
-00003c00: 7433 325f 743e 2053 6861 7271 6974 3a3a  t32_t> Sharqit::
-00003c10: 5143 6972 633a 3a73 7461 7473 287f 7374  QCirc::stats(.st
-00003c20: 6174 7301 3430 2c37 3431 0a76 6f69 6420  ats.40,741.void 
-00003c30: 5368 6172 7169 743a 3a51 4369 7263 3a3a  Sharqit::QCirc::
-00003c40: 7072 696e 745f 7374 6174 7328 7f70 7269  print_stats(.pri
-00003c50: 6e74 5f73 7461 7473 0135 382c 3132 3337  nt_stats.58,1237
-00003c60: 0a75 696e 7433 325f 7420 5368 6172 7169  .uint32_t Sharqi
-00003c70: 743a 3a51 4369 7263 3a3a 6964 5f63 6f75  t::QCirc::id_cou
-00003c80: 6e74 287f 6964 5f63 6f75 6e74 0137 342c  nt(.id_count.74,
-00003c90: 3230 3331 0a75 696e 7433 325f 7420 5368  2031.uint32_t Sh
-00003ca0: 6172 7169 743a 3a51 4369 7263 3a3a 785f  arqit::QCirc::x_
-00003cb0: 636f 756e 7428 7f78 5f63 6f75 6e74 0138  count(.x_count.8
-00003cc0: 312c 3231 3731 0a75 696e 7433 325f 7420  1,2171.uint32_t 
-00003cd0: 5368 6172 7169 743a 3a51 4369 7263 3a3a  Sharqit::QCirc::
-00003ce0: 7a5f 636f 756e 7428 7f7a 5f63 6f75 6e74  z_count(.z_count
-00003cf0: 0138 382c 3233 3039 0a75 696e 7433 325f  .88,2309.uint32_
-00003d00: 7420 5368 6172 7169 743a 3a51 4369 7263  t Sharqit::QCirc
-00003d10: 3a3a 685f 636f 756e 7428 7f68 5f63 6f75  ::h_count(.h_cou
-00003d20: 6e74 0139 352c 3234 3437 0a75 696e 7433  nt.95,2447.uint3
-00003d30: 325f 7420 5368 6172 7169 743a 3a51 4369  2_t Sharqit::QCi
-00003d40: 7263 3a3a 735f 636f 756e 7428 7f73 5f63  rc::s_count(.s_c
-00003d50: 6f75 6e74 0131 3032 2c32 3538 350a 7569  ount.102,2585.ui
-00003d60: 6e74 3332 5f74 2053 6861 7271 6974 3a3a  nt32_t Sharqit::
-00003d70: 5143 6972 633a 3a74 5f63 6f75 6e74 287f  QCirc::t_count(.
-00003d80: 745f 636f 756e 7401 3130 392c 3237 3233  t_count.109,2723
-00003d90: 0a75 696e 7433 325f 7420 5368 6172 7169  .uint32_t Sharqi
-00003da0: 743a 3a51 4369 7263 3a3a 727a 5f63 6f75  t::QCirc::rz_cou
-00003db0: 6e74 287f 727a 5f63 6f75 6e74 0131 3136  nt(.rz_count.116
-00003dc0: 2c32 3836 310a 7569 6e74 3332 5f74 2053  ,2861.uint32_t S
-00003dd0: 6861 7271 6974 3a3a 5143 6972 633a 3a63  harqit::QCirc::c
-00003de0: 785f 636f 756e 7428 7f63 785f 636f 756e  x_count(.cx_coun
-00003df0: 7401 3132 332c 3330 3031 0a75 696e 7433  t.123,3001.uint3
-00003e00: 325f 7420 5368 6172 7169 743a 3a51 4369  2_t Sharqit::QCi
-00003e10: 7263 3a3a 637a 5f63 6f75 6e74 287f 637a  rc::cz_count(.cz
-00003e20: 5f63 6f75 6e74 0131 3330 2c33 3134 310a  _count.130,3141.
-00003e30: 7569 6e74 3332 5f74 2053 6861 7271 6974  uint32_t Sharqit
-00003e40: 3a3a 5143 6972 633a 3a64 6570 7468 287f  ::QCirc::depth(.
-00003e50: 6465 7074 6801 3133 372c 3332 3831 0a73  depth.137,3281.s
-00003e60: 7464 3a3a 7374 7269 6e67 2053 6861 7271  td::string Sharq
-00003e70: 6974 3a3a 5143 6972 633a 3a74 6f5f 7374  it::QCirc::to_st
-00003e80: 7269 6e67 287f 746f 5f73 7472 696e 6701  ring(.to_string.
-00003e90: 3136 312c 3337 3933 0a53 6861 7271 6974  161,3793.Sharqit
-00003ea0: 3a3a 5143 6972 6326 2053 6861 7271 6974  ::QCirc& Sharqit
-00003eb0: 3a3a 5143 6972 633a 3a61 6464 5f71 6761  ::QCirc::add_qga
-00003ec0: 7465 287f 6164 645f 7167 6174 6501 3234  te(.add_qgate.24
-00003ed0: 342c 3632 3230 0a53 6861 7271 6974 3a3a  4,6220.Sharqit::
-00003ee0: 5143 6972 6326 2053 6861 7271 6974 3a3a  QCirc& Sharqit::
-00003ef0: 5143 6972 633a 3a61 6464 5f71 6761 7465  QCirc::add_qgate
-00003f00: 287f 6164 645f 7167 6174 6501 3235 342c  (.add_qgate.254,
-00003f10: 3634 3333 0a53 6861 7271 6974 3a3a 5143  6433.Sharqit::QC
-00003f20: 6972 6326 2053 6861 7271 6974 3a3a 5143  irc& Sharqit::QC
-00003f30: 6972 633a 3a61 6464 5f71 6369 7263 287f  irc::add_qcirc(.
-00003f40: 6164 645f 7163 6972 6301 3236 362c 3637  add_qcirc.266,67
-00003f50: 3432 0a53 6861 7271 6974 3a3a 5143 6972  42.Sharqit::QCir
-00003f60: 6326 2053 6861 7271 6974 3a3a 5143 6972  c& Sharqit::QCir
-00003f70: 633a 3a61 6464 5f72 616e 646f 6d28 7f61  c::add_random(.a
-00003f80: 6464 5f72 616e 646f 6d01 3238 322c 3731  dd_random.282,71
-00003f90: 3338 0a53 6861 7271 6974 3a3a 5143 6972  38.Sharqit::QCir
-00003fa0: 6320 5368 6172 7169 743a 3a51 4369 7263  c Sharqit::QCirc
-00003fb0: 3a3a 7265 7665 7273 6528 7f72 6576 6572  ::reverse(.rever
-00003fc0: 7365 0133 3534 2c39 3537 380a 5368 6172  se.354,9578.Shar
-00003fd0: 7169 743a 3a51 4369 7263 2053 6861 7271  qit::QCirc Sharq
-00003fe0: 6974 3a3a 5143 6972 633a 3a69 6e76 6572  it::QCirc::inver
-00003ff0: 7365 287f 696e 7665 7273 6501 3336 342c  se(.inverse.364,
-00004000: 3937 3938 0a62 6f6f 6c20 5368 6172 7169  9798.bool Sharqi
-00004010: 743a 3a51 4369 7263 3a3a 6973 5f69 6465  t::QCirc::is_ide
-00004020: 6e74 6963 616c 287f 6973 5f69 6465 6e74  ntical(.is_ident
-00004030: 6963 616c 0133 3734 2c31 3030 3238 0a62  ical.374,10028.b
-00004040: 6f6f 6c20 5368 6172 7169 743a 3a51 4369  ool Sharqit::QCi
-00004050: 7263 3a3a 6973 5f65 7175 616c 287f 6973  rc::is_equal(.is
-00004060: 5f65 7175 616c 0133 3833 2c31 3032 3731  _equal.383,10271
-00004070: 0a76 6f69 6420 5368 6172 7169 743a 3a51  .void Sharqit::Q
-00004080: 4369 7263 3a3a 746f 5f64 6f74 5f66 696c  Circ::to_dot_fil
-00004090: 6528 7f74 6f5f 646f 745f 6669 6c65 0133  e(.to_dot_file.3
-000040a0: 3933 2c31 3035 3936 0a76 6f69 6420 5368  93,10596.void Sh
-000040b0: 6172 7169 743a 3a51 4369 7263 3a3a 746f  arqit::QCirc::to
-000040c0: 5f73 7667 5f66 696c 6528 7f74 6f5f 7376  _svg_file(.to_sv
-000040d0: 675f 6669 6c65 0136 3030 2c31 3736 3230  g_file.600,17620
-000040e0: 0a53 6861 7271 6974 3a3a 5a58 4469 6167  .Sharqit::ZXDiag
-000040f0: 7261 6d20 5368 6172 7169 743a 3a51 4369  ram Sharqit::QCi
-00004100: 7263 3a3a 746f 5f7a 7864 6961 6772 616d  rc::to_zxdiagram
-00004110: 287f 746f 5f7a 7864 6961 6772 616d 0136  (.to_zxdiagram.6
-00004120: 3132 2c31 3830 3836 0a53 6861 7271 6974  12,18086.Sharqit
-00004130: 3a3a 4c69 6e65 6172 4d61 7020 5368 6172  ::LinearMap Shar
-00004140: 7169 743a 3a51 4369 7263 3a3a 746f 5f6c  qit::QCirc::to_l
-00004150: 696e 6561 726d 6170 287f 746f 5f6c 696e  inearmap(.to_lin
-00004160: 6561 726d 6170 0136 3330 2c31 3835 3636  earmap.630,18566
-00004170: 0a53 6861 7271 6974 3a3a 4441 4743 6972  .Sharqit::DAGCir
-00004180: 6320 5368 6172 7169 743a 3a51 4369 7263  c Sharqit::QCirc
-00004190: 3a3a 746f 5f64 6167 6369 7263 287f 746f  ::to_dagcirc(.to
-000041a0: 5f64 6167 6369 7263 0136 3339 2c31 3837  _dagcirc.639,187
-000041b0: 3633 0a76 6f69 6420 5368 6172 7169 743a  63.void Sharqit:
-000041c0: 3a51 4369 7263 3a3a 637a 5f74 6f5f 6378  :QCirc::cz_to_cx
-000041d0: 287f 637a 5f74 6f5f 6378 0137 3033 2c32  (.cz_to_cx.703,2
-000041e0: 3033 3339 0a76 6f69 6420 5368 6172 7169  0339.void Sharqi
-000041f0: 743a 3a51 4369 7263 3a3a 7265 6d6f 7665  t::QCirc::remove
-00004200: 5f69 6428 7f72 656d 6f76 655f 6964 0137  _id(.remove_id.7
-00004210: 3232 2c32 3039 3432 0a76 6f69 6420 2053  22,20942.void  S
-00004220: 6861 7271 6974 3a3a 5143 6972 633a 3a72  harqit::QCirc::r
-00004230: 6570 6c61 6365 5f77 6974 685f 727a 287f  eplace_with_rz(.
-00004240: 7265 706c 6163 655f 7769 7468 5f72 7a01  replace_with_rz.
-00004250: 3733 362c 3231 3438 390a 0c0a 6c69 6e65  736,21489...line
-00004260: 6172 5f6d 6170 2e68 2c36 3837 0a23 6465  ar_map.h,687.#de
-00004270: 6669 6e65 204c 494e 4541 525f 4d41 505f  fine LINEAR_MAP_
-00004280: 487f 372c 3934 0a6e 616d 6573 7061 6365  H.7,94.namespace
-00004290: 2053 6861 7271 6974 207f 3136 2c32 3134   Sharqit .16,214
-000042a0: 0a20 2063 6c61 7373 204c 696e 6561 724d  .  class LinearM
-000042b0: 6170 207f 3234 2c33 3730 0a20 2020 204c  ap .24,370.    L
-000042c0: 696e 6561 724d 6170 287f 3333 2c36 3635  inearMap(.33,665
-000042d0: 0a20 2020 204c 696e 6561 724d 6170 287f  .    LinearMap(.
-000042e0: 3339 2c39 3138 0a20 2020 204c 696e 6561  39,918.    Linea
-000042f0: 724d 6170 287f 3533 2c31 3333 370a 2020  rMap(.53,1337.  
-00004300: 2020 7569 6e74 3332 5f74 2072 6f77 5f6e    uint32_t row_n
-00004310: 756d 287f 3538 2c31 3532 360a 2020 2020  um(.58,1526.    
-00004320: 7569 6e74 3332 5f74 2063 6f6c 5f6e 756d  uint32_t col_num
-00004330: 287f 3633 2c31 3639 300a 2020 2020 4c69  (.63,1690.    Li
-00004340: 6e65 6172 4d61 7026 206f 7065 7261 746f  nearMap& operato
-00004350: 723d 287f 6f70 6572 6174 6f72 3d01 3130  r=(.operator=.10
-00004360: 312c 3331 3139 0a20 2020 204c 696e 6561  1,3119.    Linea
-00004370: 724d 6170 206f 7065 7261 746f 722b 287f  rMap operator+(.
-00004380: 3130 362c 3332 3730 0a20 2020 204c 696e  106,3270.    Lin
-00004390: 6561 724d 6170 206f 7065 7261 746f 722d  earMap operator-
-000043a0: 287f 3130 372c 3333 3230 0a20 2020 2066  (.107,3320.    f
-000043b0: 7269 656e 6420 4c69 6e65 6172 4d61 7020  riend LinearMap 
-000043c0: 6f70 6572 6174 6f72 2b28 7f31 3038 2c33  operator+(.108,3
-000043d0: 3337 390a 2020 2020 6672 6965 6e64 204c  379.    friend L
-000043e0: 696e 6561 724d 6170 206f 7065 7261 746f  inearMap operato
-000043f0: 722d 287f 3130 392c 3335 3033 0a20 2020  r-(.109,3503.   
-00004400: 2066 7269 656e 6420 4c69 6e65 6172 4d61   friend LinearMa
-00004410: 7020 6f70 6572 6174 6f72 2a28 7f31 3130  p operator*(.110
-00004420: 2c33 3632 370a 2020 2020 6672 6965 6e64  ,3627.    friend
-00004430: 204c 696e 6561 724d 6170 206f 7065 7261   LinearMap opera
-00004440: 746f 722a 287f 3131 312c 3337 3531 0a20  tor*(.111,3751. 
-00004450: 2020 2066 7269 656e 6420 4c69 6e65 6172     friend Linear
-00004460: 4d61 7020 6f70 6572 6174 6f72 2a28 7f31  Map operator*(.1
-00004470: 3132 2c33 3837 310a 2020 2020 6672 6965  12,3871.    frie
-00004480: 6e64 204c 696e 6561 724d 6170 206f 7065  nd LinearMap ope
-00004490: 7261 746f 722a 287f 3131 332c 3430 3035  rator*(.113,4005
-000044a0: 0a20 2020 2066 7269 656e 6420 4c69 6e65  .    friend Line
-000044b0: 6172 4d61 7020 6f70 6572 6174 6f72 2a28  arMap operator*(
-000044c0: 7f31 3134 2c34 3132 350a 2020 2020 6672  .114,4125.    fr
-000044d0: 6965 6e64 204c 696e 6561 724d 6170 206f  iend LinearMap o
-000044e0: 7065 7261 746f 722f 287f 3131 352c 3432  perator/(.115,42
-000044f0: 3539 0a20 2020 2066 7269 656e 6420 4c69  59.    friend Li
-00004500: 6e65 6172 4d61 7020 6f70 6572 6174 6f72  nearMap operator
-00004510: 2f28 7f31 3136 2c34 3337 390a 0c0a 7163  /(.116,4379...qc
-00004520: 6972 632e 682c 3135 3834 0a23 6465 6669  irc.h,1584.#defi
-00004530: 6e65 2051 4349 5243 5f48 7f37 2c38 300a  ne QCIRC_H.7,80.
-00004540: 2020 636c 6173 7320 5143 6972 637f 3334    class QCirc.34
-00004550: 2c34 3932 0a20 2020 2075 696e 7433 325f  ,492.    uint32_
-00004560: 7420 7175 6269 745f 6e75 6d5f 3b7f 3337  t qubit_num_;.37
-00004570: 2c35 3231 0a20 2020 2073 7464 3a3a 7665  ,521.    std::ve
-00004580: 6374 6f72 3c51 4761 7465 3e20 7167 6174  ctor<QGate> qgat
-00004590: 6573 5f3b 7f33 382c 3536 380a 2020 2020  es_;.38,568.    
-000045a0: 5143 6972 6328 7f36 302c 3135 3835 0a20  QCirc(.60,1585. 
-000045b0: 2020 2051 4369 7263 287f 3635 2c31 3735     QCirc(.65,175
-000045c0: 340a 2020 2020 5143 6972 6328 7f37 302c  4.    QCirc(.70,
-000045d0: 3139 3432 0a20 2020 2075 696e 7433 325f  1942.    uint32_
-000045e0: 7420 7175 6269 745f 6e75 6d28 7f37 322c  t qubit_num(.72,
-000045f0: 3230 3636 0a20 2020 2075 696e 7433 325f  2066.    uint32_
-00004600: 7420 6765 745f 7175 6269 745f 6e75 6d28  t get_qubit_num(
-00004610: 7f37 342c 3231 3533 0a20 2020 2073 7464  .74,2153.    std
-00004620: 3a3a 7665 6374 6f72 3c51 4761 7465 3e20  ::vector<QGate> 
-00004630: 7167 6174 6573 287f 3736 2c32 3234 310a  qgates(.76,2241.
-00004640: 2020 2020 766f 6964 2071 7562 6974 5f6e      void qubit_n
-00004650: 756d 287f 3738 2c32 3333 320a 2020 2020  um(.78,2332.    
-00004660: 766f 6964 2071 6761 7465 7328 7f38 302c  void qgates(.80,
-00004670: 3234 3335 0a20 2020 2075 696e 7433 325f  2435.    uint32_
-00004680: 7420 7167 6174 655f 6e75 6d28 7f38 352c  t qgate_num(.85,
-00004690: 3236 3130 0a20 2020 2076 6f69 6420 636c  2610.    void cl
-000046a0: 6561 7228 7f39 392c 3330 3633 0a20 2020  ear(.99,3063.   
-000046b0: 2073 7464 3a3a 6d61 703c 7f73 7464 3a3a   std::map<.std::
-000046c0: 6d61 7001 3130 342c 3332 3235 0a20 2020  map.104,3225.   
-000046d0: 2075 696e 7433 325f 7420 6761 7465 5f63   uint32_t gate_c
-000046e0: 6f75 6e74 287f 3130 392c 3334 3239 0a20  ount(.109,3429. 
-000046f0: 2020 2075 696e 7433 325f 7420 7477 6f71     uint32_t twoq
-00004700: 5f63 6f75 6e74 287f 3135 392c 3530 3031  _count(.159,5001
-00004710: 0a20 2020 2076 6f69 6420 7368 6f77 287f  .    void show(.
-00004720: 3137 342c 3535 3336 0a20 2020 2076 6f69  174,5536.    voi
-00004730: 6420 7072 696e 745f 7163 6972 6328 7f31  d print_qcirc(.1
-00004740: 3738 2c35 3639 320a 2020 2020 5143 6972  78,5692.    QCir
-00004750: 6326 2069 6428 7f32 3933 2c31 3032 3434  c& id(.293,10244
-00004760: 0a20 2020 2051 4369 7263 2620 7828 7f32  .    QCirc& x(.2
-00004770: 3939 2c31 3035 3032 0a20 2020 2051 4369  99,10502.    QCi
-00004780: 7263 2620 7a28 7f33 3035 2c31 3037 3538  rc& z(.305,10758
-00004790: 0a20 2020 2051 4369 7263 2620 7328 7f33  .    QCirc& s(.3
-000047a0: 3131 2c31 3130 3038 0a20 2020 2051 4369  11,11008.    QCi
-000047b0: 7263 2620 7364 6728 7f33 3137 2c31 3132  rc& sdg(.317,112
-000047c0: 3836 0a20 2020 2051 4369 7263 2620 7428  86.    QCirc& t(
-000047d0: 7f33 3233 2c31 3135 3430 0a20 2020 2051  .323,11540.    Q
-000047e0: 4369 7263 2620 7464 6728 7f33 3239 2c31  Circ& tdg(.329,1
-000047f0: 3138 3138 0a20 2020 2051 4369 7263 2620  1818.    QCirc& 
-00004800: 6828 7f33 3335 2c31 3230 3833 0a20 2020  h(.335,12083.   
-00004810: 2051 4369 7263 2620 727a 287f 3334 322c   QCirc& rz(.342,
-00004820: 3132 3338 310a 2020 2020 5143 6972 6326  12381.    QCirc&
-00004830: 2069 6432 287f 3334 392c 3132 3734 300a   id2(.349,12740.
-00004840: 2020 2020 5143 6972 6326 2063 7828 7f33      QCirc& cx(.3
-00004850: 3536 2c31 3330 3836 0a20 2020 2051 4369  56,13086.    QCi
-00004860: 7263 2620 637a 287f 3336 332c 3133 3432  rc& cz(.363,1342
-00004870: 330a 2020 2020 5143 6972 6326 2072 7828  3.    QCirc& rx(
-00004880: 7f33 3730 2c31 3337 3434 0a20 2020 2051  .370,13744.    Q
-00004890: 4369 7263 2620 7928 7f33 3736 2c31 3430  Circ& y(.376,140
-000048a0: 3233 0a20 2020 2051 4369 7263 2620 7378  23.    QCirc& sx
-000048b0: 287f 3338 322c 3134 3239 310a 2020 2020  (.382,14291.    
-000048c0: 5143 6972 6326 2073 7864 6728 7f33 3838  QCirc& sxdg(.388
-000048d0: 2c31 3435 3933 0a20 2020 2051 4369 7263  ,14593.    QCirc
-000048e0: 2620 7279 287f 3339 352c 3134 3838 380a  & ry(.395,14888.
-000048f0: 2020 2020 5143 6972 6326 2070 287f 3430      QCirc& p(.40
-00004900: 332c 3135 3235 340a 2020 2020 5143 6972  3,15254.    QCir
-00004910: 6326 2063 7928 7f34 3130 2c31 3535 3937  c& cy(.410,15597
-00004920: 0a20 2020 2051 4369 7263 2620 6373 7828  .    QCirc& csx(
-00004930: 7f34 3137 2c31 3539 3634 0a20 2020 2051  .417,15964.    Q
-00004940: 4369 7263 2620 6373 7864 6728 7f34 3234  Circ& csxdg(.424
-00004950: 2c31 3633 3534 0a20 2020 2051 4369 7263  ,16354.    QCirc
-00004960: 2620 6368 287f 3433 312c 3136 3733 330a  & ch(.431,16733.
-00004970: 2020 2020 5143 6972 6326 2063 7328 7f34      QCirc& cs(.4
-00004980: 3339 2c31 3731 3533 0a20 2020 2051 4369  39,17153.    QCi
-00004990: 7263 2620 6373 6467 287f 3434 372c 3137  rc& csdg(.447,17
-000049a0: 3534 370a 2020 2020 5143 6972 6326 2063  547.    QCirc& c
-000049b0: 7428 7f34 3535 2c31 3739 3232 0a20 2020  t(.455,17922.   
-000049c0: 2051 4369 7263 2620 6374 6467 287f 3436   QCirc& ctdg(.46
-000049d0: 332c 3138 3332 380a 2020 2020 5143 6972  3,18328.    QCir
-000049e0: 6326 2063 7278 287f 3437 322c 3138 3735  c& crx(.472,1875
-000049f0: 370a 2020 2020 5143 6972 6326 2063 7279  7.    QCirc& cry
-00004a00: 287f 3438 312c 3139 3139 340a 2020 2020  (.481,19194.    
-00004a10: 5143 6972 6326 2063 727a 287f 3439 302c  QCirc& crz(.490,
-00004a20: 3139 3635 360a 2020 2020 5143 6972 6326  19656.    QCirc&
-00004a30: 2063 7028 7f34 3939 2c32 3031 3137 0a20   cp(.499,20117. 
-00004a40: 2020 2051 4369 7263 2620 7278 7828 7f35     QCirc& rxx(.5
-00004a50: 3038 2c32 3035 3531 0a20 2020 2051 4369  08,20551.    QCi
-00004a60: 7263 2620 7279 7928 7f35 3232 2c32 3130  rc& ryy(.522,210
-00004a70: 3339 0a20 2020 2051 4369 7263 2620 727a  39.    QCirc& rz
-00004a80: 7a28 7f35 3336 2c32 3135 3737 0a20 2020  z(.536,21577.   
-00004a90: 2051 4369 7263 2620 7377 287f 3534 342c   QCirc& sw(.544,
-00004aa0: 3231 3933 350a 2020 2020 5143 6972 6326  21935.    QCirc&
-00004ab0: 2063 7377 287f 3535 332c 3232 3334 360a   csw(.553,22346.
-00004ac0: 2020 2020 5143 6972 6326 2063 6378 287f      QCirc& ccx(.
-00004ad0: 3536 322c 3232 3830 390a 2020 2020 5143  562,22809.    QC
-00004ae0: 6972 6326 206f 7065 7261 746f 722b 3d28  irc& operator+=(
-00004af0: 7f6f 7065 7261 746f 722b 3d01 3536 342c  .operator+=.564,
-00004b00: 3232 3938 330a 2020 2020 6672 6965 6e64  22983.    friend
-00004b10: 2051 4369 7263 206f 7065 7261 746f 722b   QCirc operator+
-00004b20: 287f 3536 352c 3233 3035 300a 2020 2020  (.565,23050.    
-00004b30: 6672 6965 6e64 2073 7464 3a3a 6f73 7472  friend std::ostr
-00004b40: 6561 6d26 206f 7065 7261 746f 723c 3c28  eam& operator<<(
-00004b50: 7f35 3636 2c32 3331 3539 0a0c 0a7a 7864  .566,23159...zxd
-00004b60: 6961 6772 616d 2e63 7070 2c31 3230 360a  iagram.cpp,1206.
-00004b70: 5368 6172 7169 743a 3a5a 5844 6961 6772  Sharqit::ZXDiagr
-00004b80: 616d 3a3a 5a58 4469 6167 7261 6d28 7f5a  am::ZXDiagram(.Z
-00004b90: 5844 6961 6772 616d 0138 2c39 350a 7374  XDiagram.8,95.st
-00004ba0: 643a 3a73 7472 696e 6720 5368 6172 7169  d::string Sharqi
-00004bb0: 743a 3a5a 5844 6961 6772 616d 3a3a 746f  t::ZXDiagram::to
-00004bc0: 5f73 7472 696e 6728 7f74 6f5f 7374 7269  _string(.to_stri
-00004bd0: 6e67 0133 342c 3839 350a 7374 643a 3a6d  ng.34,895.std::m
-00004be0: 6170 3c73 7464 3a3a 7374 7269 6e67 2c20  ap<std::string, 
-00004bf0: 7569 6e74 3332 5f74 3e20 5368 6172 7169  uint32_t> Sharqi
-00004c00: 743a 3a5a 5844 6961 6772 616d 3a3a 7374  t::ZXDiagram::st
-00004c10: 6174 7328 7f73 7461 7473 0135 342c 3134  ats(.stats.54,14
-00004c20: 3034 0a76 6f69 6420 5368 6172 7169 743a  04.void Sharqit:
-00004c30: 3a5a 5844 6961 6772 616d 3a3a 746f 5f64  :ZXDiagram::to_d
-00004c40: 6f74 5f66 696c 6528 7f74 6f5f 646f 745f  ot_file(.to_dot_
-00004c50: 6669 6c65 0138 302c 3233 3738 0a76 6f69  file.80,2378.voi
-00004c60: 6420 5368 6172 7169 743a 3a5a 5844 6961  d Sharqit::ZXDia
-00004c70: 6772 616d 3a3a 746f 5f73 7667 5f66 696c  gram::to_svg_fil
-00004c80: 6528 7f74 6f5f 7376 675f 6669 6c65 0132  e(.to_svg_file.2
-00004c90: 3234 2c36 3930 390a 766f 6964 2053 6861  24,6909.void Sha
-00004ca0: 7271 6974 3a3a 5a58 4469 6167 7261 6d3a  rqit::ZXDiagram:
-00004cb0: 3a61 6464 5f71 6761 7465 287f 6164 645f  :add_qgate(.add_
-00004cc0: 7167 6174 6501 3233 372c 3733 3834 0a62  qgate.237,7384.b
-00004cd0: 6f6f 6c20 5368 6172 7169 743a 3a5a 5844  ool Sharqit::ZXD
-00004ce0: 6961 6772 616d 3a3a 6368 6563 6b5f 636f  iagram::check_co
-00004cf0: 6e6e 6563 7428 7f63 6865 636b 5f63 6f6e  nnect(.check_con
-00004d00: 6e65 6374 0133 3738 2c31 3230 3235 0a76  nect.378,12025.v
-00004d10: 6f69 6420 5368 6172 7169 743a 3a5a 5844  oid Sharqit::ZXD
-00004d20: 6961 6772 616d 3a3a 786f 725f 6861 6461  iagram::xor_hada
-00004d30: 6d61 7264 5f65 6467 6528 7f78 6f72 5f68  mard_edge(.xor_h
-00004d40: 6164 616d 6172 645f 6564 6765 0134 3031  adamard_edge.401
-00004d50: 2c31 3234 3333 0a76 6f69 6420 5368 6172  ,12433.void Shar
-00004d60: 7169 743a 3a5a 5844 6961 6772 616d 3a3a  qit::ZXDiagram::
-00004d70: 786f 725f 6861 6461 6d61 7264 5f65 6467  xor_hadamard_edg
-00004d80: 6573 287f 786f 725f 6861 6461 6d61 7264  es(.xor_hadamard
-00004d90: 5f65 6467 6573 0134 3334 2c31 3334 3337  _edges.434,13437
-00004da0: 0a53 6861 7271 6974 3a3a 5a58 4e6f 6465  .Sharqit::ZXNode
-00004db0: 4b69 6e64 2053 6861 7271 6974 3a3a 5a58  Kind Sharqit::ZX
-00004dc0: 4469 6167 7261 6d3a 3a72 656d 6f76 655f  Diagram::remove_
-00004dd0: 6e6f 6465 287f 7265 6d6f 7665 5f6e 6f64  node(.remove_nod
-00004de0: 6501 3434 362c 3133 3830 370a 5368 6172  e.446,13807.Shar
-00004df0: 7169 743a 3a5a 5845 6467 654b 696e 6420  qit::ZXEdgeKind 
-00004e00: 5368 6172 7169 743a 3a5a 5844 6961 6772  Sharqit::ZXDiagr
-00004e10: 616d 3a3a 7265 6d6f 7665 5f65 6467 6528  am::remove_edge(
-00004e20: 7f72 656d 6f76 655f 6564 6765 0134 3830  .remove_edge.480
-00004e30: 2c31 3435 3036 0a75 696e 7433 325f 7420  ,14506.uint32_t 
-00004e40: 5368 6172 7169 743a 3a5a 5844 6961 6772  Sharqit::ZXDiagr
-00004e50: 616d 3a3a 6170 7065 6e64 5f6e 6f64 6528  am::append_node(
-00004e60: 7f61 7070 656e 645f 6e6f 6465 0135 3034  .append_node.504
-00004e70: 2c31 3530 3437 0a75 696e 7433 325f 7420  ,15047.uint32_t 
-00004e80: 5368 6172 7169 743a 3a5a 5844 6961 6772  Sharqit::ZXDiagr
-00004e90: 616d 3a3a 6170 7065 6e64 5f6e 6f64 6528  am::append_node(
-00004ea0: 7f61 7070 656e 645f 6e6f 6465 0135 3132  .append_node.512
-00004eb0: 2c31 3532 3431 0a76 6f69 6420 5368 6172  ,15241.void Shar
-00004ec0: 7169 743a 3a5a 5844 6961 6772 616d 3a3a  qit::ZXDiagram::
-00004ed0: 636f 6e6e 6563 745f 6e6f 6465 7328 7f63  connect_nodes(.c
-00004ee0: 6f6e 6e65 6374 5f6e 6f64 6573 0135 3235  onnect_nodes.525
-00004ef0: 2c31 3535 3833 0a76 6f69 6420 5368 6172  ,15583.void Shar
-00004f00: 7169 743a 3a5a 5844 6961 6772 616d 3a3a  qit::ZXDiagram::
-00004f10: 7377 6170 5f6e 6f64 6573 287f 7377 6170  swap_nodes(.swap
-00004f20: 5f6e 6f64 6573 0135 3333 2c31 3538 3339  _nodes.533,15839
-00004f30: 0a76 6f69 6420 5368 6172 7169 743a 3a5a  .void Sharqit::Z
-00004f40: 5844 6961 6772 616d 3a3a 7265 6d6f 7665  XDiagram::remove
-00004f50: 5f69 736f 6c61 7465 645f 7370 6964 6572  _isolated_spider
-00004f60: 7328 7f72 656d 6f76 655f 6973 6f6c 6174  s(.remove_isolat
-00004f70: 6564 5f73 7069 6465 7273 0135 3438 2c31  ed_spiders.548,1
-00004f80: 3632 3235 0a76 6f69 6420 5368 6172 7169  6225.void Sharqi
-00004f90: 743a 3a5a 5844 6961 6772 616d 3a3a 726f  t::ZXDiagram::ro
-00004fa0: 775f 6f70 6572 6174 696f 6e28 7f72 6f77  w_operation(.row
-00004fb0: 5f6f 7065 7261 7469 6f6e 0135 3634 2c31  _operation.564,1
-00004fc0: 3635 3438 0a73 7464 3a3a 7665 6374 6f72  6548.std::vector
-00004fd0: 3c75 696e 7433 325f 743e 2053 6861 7271  <uint32_t> Sharq
-00004fe0: 6974 3a3a 5a58 4469 6167 7261 6d3a 3a61  it::ZXDiagram::a
-00004ff0: 646a 6163 656e 745f 6e6f 6465 5f69 6e64  djacent_node_ind
-00005000: 6578 6573 287f 6164 6a61 6365 6e74 5f6e  exes(.adjacent_n
-00005010: 6f64 655f 696e 6465 7865 7301 3537 332c  ode_indexes.573,
-00005020: 3136 3736 360a 0c0a 6672 6163 7469 6f6e  16766...fraction
-00005030: 2e68 2c31 3731 320a 2364 6566 696e 6520  .h,1712.#define 
-00005040: 4652 4143 5449 4f4e 5f48 7f37 2c38 390a  FRACTION_H.7,89.
-00005050: 2020 636c 6173 7320 4672 6163 7469 6f6e    class Fraction
-00005060: 7f31 382c 3234 320a 2020 2020 696e 7433  .18,242.    int3
-00005070: 325f 7420 6e75 6d65 7261 746f 725f 3b7f  2_t numerator_;.
-00005080: 3231 2c32 3734 0a20 2020 2069 6e74 3332  21,274.    int32
-00005090: 5f74 2064 656e 6f6d 696e 6174 6f72 5f3b  _t denominator_;
-000050a0: 7f32 322c 3332 390a 2020 2020 4672 6163  .22,329.    Frac
-000050b0: 7469 6f6e 287f 3237 2c34 3536 0a20 2020  tion(.27,456.   
-000050c0: 2046 7261 6374 696f 6e28 7f33 332c 3637   Fraction(.33,67
-000050d0: 390a 2020 2020 4672 6163 7469 6f6e 287f  9.    Fraction(.
-000050e0: 3339 2c39 3139 0a20 2020 2069 6e74 3332  39,919.    int32
-000050f0: 5f74 206e 756d 6572 6174 6f72 287f 3431  _t numerator(.41
-00005100: 2c31 3035 330a 2020 2020 696e 7433 325f  ,1053.    int32_
-00005110: 7420 6465 6e6f 6d69 6e61 746f 7228 7f34  t denominator(.4
-00005120: 332c 3131 3431 0a20 2020 2076 6f69 6420  3,1141.    void 
-00005130: 6e75 6d65 7261 746f 7228 7f34 352c 3132  numerator(.45,12
-00005140: 3331 0a20 2020 2076 6f69 6420 6465 6e6f  31.    void deno
-00005150: 6d69 6e61 746f 7228 7f34 372c 3133 3438  minator(.47,1348
-00005160: 0a20 2020 2046 7261 6374 696f 6e20 6164  .    Fraction ad
-00005170: 6428 7f35 382c 3137 3039 0a20 2020 2046  d(.58,1709.    F
-00005180: 7261 6374 696f 6e20 6164 6428 7f36 392c  raction add(.69,
-00005190: 3231 3330 0a20 2020 2046 7261 6374 696f  2130.    Fractio
-000051a0: 6e20 7375 6228 7f37 352c 3233 3439 0a20  n sub(.75,2349. 
-000051b0: 2020 2046 7261 6374 696f 6e20 7375 6228     Fraction sub(
-000051c0: 7f38 362c 3237 3732 0a20 2020 2046 7261  .86,2772.    Fra
-000051d0: 6374 696f 6e20 6d75 6c28 7f39 322c 3239  ction mul(.92,29
-000051e0: 3931 0a20 2020 2046 7261 6374 696f 6e20  91.    Fraction 
-000051f0: 6d75 6c28 7f31 3033 2c33 3337 370a 2020  mul(.103,3377.  
-00005200: 2020 4672 6163 7469 6f6e 2064 6976 287f    Fraction div(.
-00005210: 3130 392c 3335 3931 0a20 2020 2046 7261  109,3591.    Fra
-00005220: 6374 696f 6e20 6469 7628 7f31 3230 2c33  ction div(.120,3
-00005230: 3937 360a 2020 2020 626f 6f6c 2069 735f  976.    bool is_
-00005240: 7a65 726f 287f 3132 352c 3431 3732 0a20  zero(.125,4172. 
-00005250: 2020 2062 6f6f 6c20 6973 5f70 6f73 6974     bool is_posit
-00005260: 6976 6528 7f31 3330 2c34 3335 320a 2020  ive(.130,4352.  
-00005270: 2020 626f 6f6c 2069 735f 6e65 6761 7469    bool is_negati
-00005280: 7665 287f 3133 352c 3435 3530 0a20 2020  ve(.135,4550.   
-00005290: 2076 6f69 6420 7265 6475 6365 287f 3133   void reduce(.13
-000052a0: 392c 3436 3731 0a20 2020 2073 7461 7469  9,4671.    stati
-000052b0: 6320 696e 7433 325f 7420 6763 6428 7f31  c int32_t gcd(.1
-000052c0: 3630 2c35 3237 390a 2020 2020 4672 6163  60,5279.    Frac
-000052d0: 7469 6f6e 206f 7065 7261 746f 722b 287f  tion operator+(.
-000052e0: 3137 322c 3535 3335 0a20 2020 2046 7261  172,5535.    Fra
-000052f0: 6374 696f 6e20 6f70 6572 6174 6f72 2d28  ction operator-(
-00005300: 7f31 3733 2c35 3538 340a 2020 2020 4672  .173,5584.    Fr
-00005310: 6163 7469 6f6e 2620 6f70 6572 6174 6f72  action& operator
-00005320: 2b3d 287f 6f70 6572 6174 6f72 2b3d 0131  +=(.operator+=.1
-00005330: 3734 2c35 3633 350a 2020 2020 4672 6163  74,5635.    Frac
-00005340: 7469 6f6e 2620 6f70 6572 6174 6f72 2b3d  tion& operator+=
-00005350: 287f 6f70 6572 6174 6f72 2b3d 0131 3831  (.operator+=.181
-00005360: 2c35 3832 330a 2020 2020 4672 6163 7469  ,5823.    Fracti
-00005370: 6f6e 2620 6f70 6572 6174 6f72 2d3d 287f  on& operator-=(.
-00005380: 6f70 6572 6174 6f72 2d3d 0131 3832 2c35  operator-=.182,5
-00005390: 3930 350a 2020 2020 4672 6163 7469 6f6e  905.    Fraction
-000053a0: 2620 6f70 6572 6174 6f72 2d3d 287f 6f70  & operator-=(.op
-000053b0: 6572 6174 6f72 2d3d 0131 3839 2c36 3039  erator-=.189,609
-000053c0: 330a 2020 2020 4672 6163 7469 6f6e 2620  3.    Fraction& 
-000053d0: 6f70 6572 6174 6f72 2a3d 287f 6f70 6572  operator*=(.oper
-000053e0: 6174 6f72 2a3d 0131 3930 2c36 3137 350a  ator*=.190,6175.
-000053f0: 2020 2020 4672 6163 7469 6f6e 2620 6f70      Fraction& op
-00005400: 6572 6174 6f72 2a3d 287f 6f70 6572 6174  erator*=(.operat
-00005410: 6f72 2a3d 0131 3937 2c36 3336 330a 2020  or*=.197,6363.  
-00005420: 2020 4672 6163 7469 6f6e 2620 6f70 6572    Fraction& oper
-00005430: 6174 6f72 2f3d 287f 6f70 6572 6174 6f72  ator/=(.operator
-00005440: 2f3d 0131 3938 2c36 3434 350a 2020 2020  /=.198,6445.    
-00005450: 4672 6163 7469 6f6e 2620 6f70 6572 6174  Fraction& operat
-00005460: 6f72 2f3d 287f 6f70 6572 6174 6f72 2f3d  or/=(.operator/=
-00005470: 0132 3035 2c36 3633 330a 2020 2020 6672  .205,6633.    fr
-00005480: 6965 6e64 2062 6f6f 6c20 6f70 6572 6174  iend bool operat
-00005490: 6f72 3d3d 287f 6f70 6572 6174 6f72 3d3d  or==(.operator==
-000054a0: 0132 3036 2c36 3731 350a 2020 2020 6672  .206,6715.    fr
-000054b0: 6965 6e64 2062 6f6f 6c20 6f70 6572 6174  iend bool operat
-000054c0: 6f72 213d 287f 6f70 6572 6174 6f72 213d  or!=(.operator!=
-000054d0: 0132 3130 2c36 3838 370a 2020 2020 6672  .210,6887.    fr
-000054e0: 6965 6e64 2046 7261 6374 696f 6e20 6f70  iend Fraction op
-000054f0: 6572 6174 6f72 2b28 7f32 3131 2c36 3938  erator+(.211,698
-00005500: 320a 2020 2020 6672 6965 6e64 2046 7261  2.    friend Fra
-00005510: 6374 696f 6e20 6f70 6572 6174 6f72 2b28  ction operator+(
-00005520: 7f32 3132 2c37 3037 390a 2020 2020 6672  .212,7079.    fr
-00005530: 6965 6e64 2046 7261 6374 696f 6e20 6f70  iend Fraction op
-00005540: 6572 6174 6f72 2b28 7f32 3133 2c37 3138  erator+(.213,718
-00005550: 340a 2020 2020 6672 6965 6e64 2046 7261  4.    friend Fra
-00005560: 6374 696f 6e20 6f70 6572 6174 6f72 2d28  ction operator-(
-00005570: 7f32 3134 2c37 3238 390a 2020 2020 6672  .214,7289.    fr
-00005580: 6965 6e64 2046 7261 6374 696f 6e20 6f70  iend Fraction op
-00005590: 6572 6174 6f72 2d28 7f32 3135 2c37 3338  erator-(.215,738
-000055a0: 360a 2020 2020 6672 6965 6e64 2046 7261  6.    friend Fra
-000055b0: 6374 696f 6e20 6f70 6572 6174 6f72 2d28  ction operator-(
-000055c0: 7f32 3136 2c37 3439 310a 2020 2020 6672  .216,7491.    fr
-000055d0: 6965 6e64 2046 7261 6374 696f 6e20 6f70  iend Fraction op
-000055e0: 6572 6174 6f72 2a28 7f32 3137 2c37 3539  erator*(.217,759
-000055f0: 360a 2020 2020 6672 6965 6e64 2046 7261  6.    friend Fra
-00005600: 6374 696f 6e20 6f70 6572 6174 6f72 2a28  ction operator*(
-00005610: 7f32 3138 2c37 3639 330a 2020 2020 6672  .218,7693.    fr
-00005620: 6965 6e64 2046 7261 6374 696f 6e20 6f70  iend Fraction op
-00005630: 6572 6174 6f72 2a28 7f32 3139 2c37 3739  erator*(.219,779
-00005640: 380a 2020 2020 6672 6965 6e64 2046 7261  8.    friend Fra
-00005650: 6374 696f 6e20 6f70 6572 6174 6f72 2f28  ction operator/(
-00005660: 7f32 3230 2c37 3930 330a 2020 2020 6672  .220,7903.    fr
-00005670: 6965 6e64 2046 7261 6374 696f 6e20 6f70  iend Fraction op
-00005680: 6572 6174 6f72 2f28 7f32 3231 2c38 3030  erator/(.221,800
-00005690: 300a 2020 2020 6672 6965 6e64 2046 7261  0.    friend Fra
-000056a0: 6374 696f 6e20 6f70 6572 6174 6f72 2f28  ction operator/(
-000056b0: 7f32 3232 2c38 3130 350a 2020 2020 6672  .222,8105.    fr
-000056c0: 6965 6e64 2073 7464 3a3a 6f73 7472 6561  iend std::ostrea
-000056d0: 6d26 206f 7065 7261 746f 723c 3c28 7f32  m& operator<<(.2
-000056e0: 3233 2c38 3231 300a 0c0a 6269 6e61 7279  23,8210...binary
-000056f0: 5f6d 6174 7269 782e 6370 702c 3136 320a  _matrix.cpp,162.
-00005700: 7374 643a 3a73 7472 696e 6720 5368 6172  std::string Shar
-00005710: 7169 743a 3a42 696e 6172 794d 6174 7269  qit::BinaryMatri
-00005720: 783a 3a74 6f5f 7374 7269 6e67 287f 746f  x::to_string(.to
-00005730: 5f73 7472 696e 6701 382c 3131 330a 7374  _string.8,113.st
-00005740: 643a 3a76 6563 746f 723c 7374 643a 3a70  d::vector<std::p
-00005750: 6169 723c 7569 6e74 3332 5f74 2c20 7569  air<uint32_t, ui
-00005760: 6e74 3332 5f74 3e3e 2053 6861 7271 6974  nt32_t>> Sharqit
-00005770: 3a3a 4269 6e61 7279 4d61 7472 6978 3a3a  ::BinaryMatrix::
-00005780: 6761 7573 735f 7265 6475 6365 287f 6761  gauss_reduce(.ga
-00005790: 7573 735f 7265 6475 6365 0132 382c 3439  uss_reduce.28,49
-000057a0: 300a 0c0a 6672 6163 7469 6f6e 2e63 7070  0...fraction.cpp
-000057b0: 2c35 370a 7374 643a 3a73 7472 696e 6720  ,57.std::string 
-000057c0: 5368 6172 7169 743a 3a46 7261 6374 696f  Sharqit::Fractio
-000057d0: 6e3a 3a74 6f5f 7374 7269 6e67 287f 746f  n::to_string(.to
-000057e0: 5f73 7472 696e 6701 382c 3939 0a0c 0a70  _string.8,99...p
-000057f0: 6861 7365 2e63 7070 2c39 300a 5368 6172  hase.cpp,90.Shar
-00005800: 7169 743a 3a50 6861 7365 3a3a 5068 6173  qit::Phase::Phas
-00005810: 6528 7f50 6861 7365 0138 2c39 300a 7374  e(.Phase.8,90.st
-00005820: 643a 3a73 7472 696e 6720 5368 6172 7169  d::string Sharqi
-00005830: 743a 3a50 6861 7365 3a3a 746f 5f73 7472  t::Phase::to_str
-00005840: 696e 6728 7f74 6f5f 7374 7269 6e67 0133  ing(.to_string.3
-00005850: 312c 3734 340a 0c0a 7a78 2e68 2c33 3139  1,744...zx.h,319
-00005860: 320a 2364 6566 696e 6520 5a58 5f48 7f31  2.#define ZX_H.1
-00005870: 312c 3839 330a 2020 656e 756d 205a 584e  1,893.  enum ZXN
-00005880: 6f64 654b 696e 6420 7f32 352c 3130 3832  odeKind .25,1082
-00005890: 0a09 0920 2020 5853 7069 6465 722c 7f32  ...   XSpider,.2
-000058a0: 362c 3131 3032 0a09 0920 2020 5a53 7069  6,1102...   ZSpi
-000058b0: 6465 722c 7f32 372c 3131 3330 0a09 0920  der,.27,1130... 
-000058c0: 2020 496e 7075 742c 7f32 382c 3131 3538    Input,.28,1158
-000058d0: 0a09 0920 2020 4f75 7470 7574 207f 3239  ...   Output .29
-000058e0: 2c31 3138 360a 2020 656e 756d 205a 5845  ,1186.  enum ZXE
-000058f0: 6467 654b 696e 6420 7f33 322c 3132 3534  dgeKind .32,1254
-00005900: 0a09 0920 2020 4e6f 6e65 2c7f 3333 2c31  ...   None,.33,1
-00005910: 3237 340a 0909 2020 2050 6c61 696e 2c7f  274...   Plain,.
-00005920: 3334 2c31 3331 320a 0909 2020 2048 6164  34,1312...   Had
-00005930: 616d 6172 6420 7f33 352c 3133 3738 0a20  amard .35,1378. 
-00005940: 2065 6e75 6d20 5a58 4469 6167 7261 6d4b   enum ZXDiagramK
-00005950: 696e 6420 7f33 382c 3134 3631 0a09 0920  ind .38,1461... 
-00005960: 2020 2020 2047 656e 6572 616c 2c7f 3339       General,.39
-00005970: 2c31 3438 340a 0909 2020 2020 2020 4772  ,1484...      Gr
-00005980: 6170 684c 696b 6520 7f34 302c 3135 3235  aphLike .40,1525
-00005990: 0a20 2065 6e75 6d20 5a58 4e6f 6465 506c  .  enum ZXNodePl
-000059a0: 6163 6520 7f34 332c 3136 3030 0a09 0920  ace .43,1600... 
-000059b0: 2020 2054 6572 6d69 6e61 6c2c 7f34 342c     Terminal,.44,
-000059c0: 3136 3231 0a09 0920 2020 2042 6f75 6e64  1621...    Bound
-000059d0: 6172 792c 7f34 352c 3136 3636 0a09 0920  ary,.45,1666... 
-000059e0: 2020 2049 6e74 6572 6e61 6c20 7f34 362c     Internal .46,
-000059f0: 3137 3436 0a20 2063 6c61 7373 205a 584e  1746.  class ZXN
-00005a00: 6f64 657f 3539 2c32 3233 320a 2020 2020  ode.59,2232.    
-00005a10: 5a58 4e6f 6465 4b69 6e64 206b 696e 645f  ZXNodeKind kind_
-00005a20: 3b7f 3632 2c32 3236 320a 2020 2020 5068  ;.62,2262.    Ph
-00005a30: 6173 6520 7068 6173 655f 3b7f 3633 2c32  ase phase_;.63,2
-00005a40: 3332 300a 2020 2020 7569 6e74 3332 5f74  320.    uint32_t
-00005a50: 2071 5f3b 7f36 342c 3233 3735 0a20 2020   q_;.64,2375.   
-00005a60: 2062 6f6f 6c20 7067 5f70 6861 7365 5f3b   bool pg_phase_;
-00005a70: 7f36 352c 3234 3430 0a20 2020 2062 6f6f  .65,2440.    boo
-00005a80: 6c20 7067 5f72 6f6f 745f 3b7f 3636 2c32  l pg_root_;.66,2
-00005a90: 3532 350a 2020 2020 626f 6f6c 2070 675f  525.    bool pg_
-00005aa0: 6c65 6166 5f3b 7f36 372c 3236 3038 0a20  leaf_;.67,2608. 
-00005ab0: 2020 205a 584e 6f64 6528 7f37 382c 3331     ZXNode(.78,31
-00005ac0: 3237 0a20 2020 205a 584e 6f64 6528 7f38  27.    ZXNode(.8
-00005ad0: 352c 3335 3232 0a20 2020 205a 584e 6f64  5,3522.    ZXNod
-00005ae0: 654b 696e 6420 6b69 6e64 287f 3838 2c33  eKind kind(.88,3
-00005af0: 3732 300a 2020 2020 5068 6173 6520 7068  720.    Phase ph
-00005b00: 6173 6528 7f39 302c 3337 3935 0a20 2020  ase(.90,3795.   
-00005b10: 2075 696e 7433 325f 7420 7128 7f39 322c   uint32_t q(.92,
-00005b20: 3338 3633 0a20 2020 2062 6f6f 6c20 7067  3863.    bool pg
-00005b30: 5f70 6861 7365 287f 3934 2c33 3933 330a  _phase(.94,3933.
-00005b40: 2020 2020 626f 6f6c 2070 675f 726f 6f74      bool pg_root
-00005b50: 287f 3936 2c34 3031 320a 2020 2020 626f  (.96,4012.    bo
-00005b60: 6f6c 2070 675f 6c65 6166 287f 3938 2c34  ol pg_leaf(.98,4
-00005b70: 3038 390a 2020 2020 766f 6964 206b 696e  089.    void kin
-00005b80: 6428 7f31 3030 2c34 3136 330a 2020 2020  d(.100,4163.    
-00005b90: 766f 6964 2070 6861 7365 287f 3130 322c  void phase(.102,
-00005ba0: 3432 3437 0a20 2020 2076 6f69 6420 7128  4247.    void q(
-00005bb0: 7f31 3034 2c34 3332 360a 2020 2020 766f  .104,4326.    vo
-00005bc0: 6964 2070 675f 7068 6173 6528 7f31 3036  id pg_phase(.106
-00005bd0: 2c34 3339 390a 2020 2020 766f 6964 2070  ,4399.    void p
-00005be0: 675f 726f 6f74 287f 3130 382c 3434 3935  g_root(.108,4495
-00005bf0: 0a20 2020 2076 6f69 6420 7067 5f6c 6561  .    void pg_lea
-00005c00: 6628 7f31 3130 2c34 3538 370a 2020 2020  f(.110,4587.    
-00005c10: 7374 643a 3a73 7472 696e 6720 6b69 6e64  std::string kind
-00005c20: 5f73 7472 287f 3131 352c 3437 3537 0a20  _str(.115,4757. 
-00005c30: 2063 6c61 7373 205a 5845 6467 657f 3133   class ZXEdge.13
-00005c40: 322c 3531 3430 0a20 2020 205a 5845 6467  2,5140.    ZXEdg
-00005c50: 654b 696e 6420 6b69 6e64 5f3b 7f31 3335  eKind kind_;.135
-00005c60: 2c35 3137 300a 2020 2020 7569 6e74 3332  ,5170.    uint32
-00005c70: 5f74 2074 6f5f 3b7f 3133 362c 3532 3238  _t to_;.136,5228
-00005c80: 0a20 2020 205a 5845 6467 6528 7f31 3433  .    ZXEdge(.143
-00005c90: 2c35 3438 390a 2020 2020 5a58 4564 6765  ,5489.    ZXEdge
-00005ca0: 287f 3134 382c 3536 3838 0a20 2020 205a  (.148,5688.    Z
-00005cb0: 5845 6467 654b 696e 6420 6b69 6e64 287f  XEdgeKind kind(.
-00005cc0: 3135 302c 3537 3835 0a20 2020 2075 696e  150,5785.    uin
-00005cd0: 7433 325f 7420 746f 287f 3135 322c 3538  t32_t to(.152,58
-00005ce0: 3537 0a20 2020 2076 6f69 6420 6b69 6e64  57.    void kind
-00005cf0: 287f 3135 342c 3539 3235 0a20 2020 2076  (.154,5925.    v
-00005d00: 6f69 6420 746f 287f 3135 362c 3630 3036  oid to(.156,6006
-00005d10: 0a20 2020 2073 7464 3a3a 7374 7269 6e67  .    std::string
-00005d20: 206b 696e 645f 7374 7228 7f31 3631 2c36   kind_str(.161,6
-00005d30: 3136 300a 2020 2020 7374 643a 3a73 7472  160.    std::str
-00005d40: 696e 6720 6e61 6d65 287f 3136 392c 3633  ing name(.169,63
-00005d50: 3837 0a20 2020 2076 6f69 6420 7265 7665  87.    void reve
-00005d60: 7273 655f 6b69 6e64 287f 3138 312c 3637  rse_kind(.181,67
-00005d70: 3236 0a20 2063 6c61 7373 205a 5844 6961  26.  class ZXDia
-00005d80: 6772 616d 7f31 3938 2c37 3731 340a 2020  gram.198,7714.  
-00005d90: 2020 5a58 4469 6167 7261 6d4b 696e 6420    ZXDiagramKind 
-00005da0: 6b69 6e64 5f3b 7f32 3031 2c37 3734 370a  kind_;.201,7747.
-00005db0: 2020 2020 7569 6e74 3332 5f74 2071 7562      uint32_t qub
-00005dc0: 6974 5f6e 756d 5f3b 7f32 3032 2c37 3830  it_num_;.202,780
-00005dd0: 300a 2020 2020 7374 643a 3a76 6563 746f  0.    std::vecto
-00005de0: 723c 5a58 4e6f 6465 3e20 6e6f 6465 735f  r<ZXNode> nodes_
-00005df0: 3b7f 3230 332c 3738 3437 0a20 2020 2073  ;.203,7847.    s
-00005e00: 7464 3a3a 7665 6374 6f72 3c75 696e 7433  td::vector<uint3
-00005e10: 325f 743e 2069 6e70 7574 735f 3b7f 3230  2_t> inputs_;.20
-00005e20: 342c 3739 3133 0a20 2020 2073 7464 3a3a  4,7913.    std::
-00005e30: 7665 6374 6f72 3c75 696e 7433 325f 743e  vector<uint32_t>
-00005e40: 206f 7574 7075 7473 5f3b 7f32 3035 2c37   outputs_;.205,7
-00005e50: 3938 360a 2020 2020 7374 643a 3a76 6563  986.    std::vec
-00005e60: 746f 723c 7374 643a 3a76 6563 746f 723c  tor<std::vector<
-00005e70: 5a58 4564 6765 3e3e 2061 646a 5f6d 6174  ZXEdge>> adj_mat
-00005e80: 5f3b 7f32 3036 2c38 3036 310a 2020 2020  _;.206,8061.    
-00005e90: 7374 643a 3a76 6563 746f 723c 5a58 4e6f  std::vector<ZXNo
-00005ea0: 6465 506c 6163 653e 206e 6f64 655f 706c  dePlace> node_pl
-00005eb0: 6163 6573 5f3b 7f32 3037 2c38 3134 370a  aces_;.207,8147.
-00005ec0: 2020 2020 7569 6e74 3332 5f74 206d 6178      uint32_t max
-00005ed0: 5f61 646a 5f6e 756d 287f 3231 312c 3833  _adj_num(.211,83
-00005ee0: 3237 0a20 2020 2062 6f6f 6c20 6368 6563  27.    bool chec
-00005ef0: 6b5f 785f 7370 6964 6572 287f 3232 342c  k_x_spider(.224,
-00005f00: 3837 3430 0a20 2020 2062 6f6f 6c20 6368  8740.    bool ch
-00005f10: 6563 6b5f 7a5f 7370 6964 6572 287f 3233  eck_z_spider(.23
-00005f20: 302c 3930 3837 0a20 2020 2062 6f6f 6c20  0,9087.    bool 
-00005f30: 6368 6563 6b5f 7a65 726f 5f70 6861 7365  check_zero_phase
-00005f40: 5f73 7069 6465 7228 7f32 3336 2c39 3435  _spider(.236,945
-00005f50: 320a 2020 2020 626f 6f6c 2063 6865 636b  2.    bool check
-00005f60: 5f70 6175 6c69 5f73 7069 6465 7228 7f32  _pauli_spider(.2
-00005f70: 3437 2c39 3935 370a 2020 2020 626f 6f6c  47,9957.    bool
-00005f80: 2063 6865 636b 5f70 726f 7065 725f 636c   check_proper_cl
-00005f90: 6966 666f 7264 5f73 7069 6465 7228 7f32  ifford_spider(.2
-00005fa0: 3538 2c31 3035 3139 0a20 2020 2062 6f6f  58,10519.    boo
-00005fb0: 6c20 6368 6563 6b5f 636c 6966 666f 7264  l check_clifford
-00005fc0: 5f73 7069 6465 7228 7f32 3639 2c31 3130  _spider(.269,110
-00005fd0: 3831 0a20 2020 2062 6f6f 6c20 6368 6563  81.    bool chec
-00005fe0: 6b5f 6e6f 6e5f 636c 6966 666f 7264 5f73  k_non_clifford_s
-00005ff0: 7069 6465 7228 7f32 3738 2c31 3134 3930  pider(.278,11490
-00006000: 0a20 2020 2062 6f6f 6c20 6368 6563 6b5f  .    bool check_
-00006010: 696e 7465 726e 616c 5f6e 6f64 6528 7f32  internal_node(.2
-00006020: 3834 2c31 3138 3335 0a20 2020 2062 6f6f  84,11835.    boo
-00006030: 6c20 6368 6563 6b5f 626f 756e 6461 7279  l check_boundary
-00006040: 5f6e 6f64 6528 7f32 3930 2c31 3231 3839  _node(.290,12189
-00006050: 0a20 2020 2062 6f6f 6c20 6368 6563 6b5f  .    bool check_
-00006060: 7067 5f70 6861 7365 5f6e 6f64 6528 7f32  pg_phase_node(.2
-00006070: 3936 2c31 3235 3733 0a20 2020 2062 6f6f  96,12573.    boo
-00006080: 6c20 6368 6563 6b5f 7067 5f72 6f6f 745f  l check_pg_root_
-00006090: 6e6f 6465 287f 3330 322c 3132 3933 350a  node(.302,12935.
-000060a0: 2020 2020 626f 6f6c 2063 6865 636b 5f70      bool check_p
-000060b0: 675f 6c65 6166 5f6e 6f64 6528 7f33 3038  g_leaf_node(.308
-000060c0: 2c31 3332 3935 0a20 2020 2062 6f6f 6c20  ,13295.    bool 
-000060d0: 6368 6563 6b5f 7068 6173 655f 6761 6467  check_phase_gadg
-000060e0: 6574 5f6e 6f64 6528 7f33 3134 2c31 3336  et_node(.314,136
-000060f0: 3737 0a20 2020 2062 6f6f 6c20 6368 6563  77.    bool chec
-00006100: 6b5f 696e 7075 745f 6e6f 6465 287f 3332  k_input_node(.32
-00006110: 312c 3134 3034 370a 2020 2020 626f 6f6c  1,14047.    bool
-00006120: 2063 6865 636b 5f6f 7574 7075 745f 6e6f   check_output_no
-00006130: 6465 287f 3332 372c 3134 3430 320a 2020  de(.327,14402.  
-00006140: 2020 626f 6f6c 2063 6865 636b 5f63 6f6e    bool check_con
-00006150: 6e65 6374 5f69 6e70 7574 5f6e 6f64 6528  nect_input_node(
-00006160: 7f33 3333 2c31 3437 3639 0a20 2020 2062  .333,14769.    b
-00006170: 6f6f 6c20 6368 6563 6b5f 636f 6e6e 6563  ool check_connec
-00006180: 745f 6f75 7470 7574 5f6e 6f64 6528 7f33  t_output_node(.3
-00006190: 3435 2c31 3532 3232 0a20 2020 2062 6f6f  45,15222.    boo
-000061a0: 6c20 6368 6563 6b5f 636f 6e6e 6563 745f  l check_connect_
-000061b0: 7068 6173 655f 6761 6467 6574 287f 3335  phase_gadget(.35
-000061c0: 372c 3135 3731 310a 2020 2020 766f 6964  7,15711.    void
-000061d0: 2072 656d 6f76 655f 6564 6765 735f 6f66   remove_edges_of
-000061e0: 5f6e 6f64 6528 7f33 3932 2c31 3730 3537  _node(.392,17057
-000061f0: 0a20 2020 2075 696e 7433 325f 7420 6465  .    uint32_t de
-00006200: 6772 6565 5f6f 665f 6e6f 6465 287f 3430  gree_of_node(.40
-00006210: 392c 3137 3536 310a 2020 2020 5a58 4e6f  9,17561.    ZXNo
-00006220: 6465 4b69 6e64 206b 696e 645f 6f66 5f6e  deKind kind_of_n
-00006230: 6f64 6528 7f34 3135 2c31 3738 3035 0a20  ode(.415,17805. 
-00006240: 2020 2073 7464 3a3a 7665 6374 6f72 3c7f     std::vector<.
-00006250: 7374 643a 3a76 6563 746f 7201 3532 322c  std::vector.522,
-00006260: 3232 3430 390a 2020 2020 5a58 4469 6167  22409.    ZXDiag
-00006270: 7261 6d28 7f35 3333 2c32 3237 3739 0a20  ram(.533,22779. 
-00006280: 2020 205a 5844 6961 6772 616d 4b69 6e64     ZXDiagramKind
-00006290: 206b 696e 6428 7f35 3338 2c32 3330 3233   kind(.538,23023
-000062a0: 0a20 2020 2075 696e 7433 325f 7420 7175  .    uint32_t qu
-000062b0: 6269 745f 6e75 6d28 7f35 3430 2c32 3331  bit_num(.540,231
-000062c0: 3035 0a20 2020 2073 7464 3a3a 7665 6374  05.    std::vect
-000062d0: 6f72 3c5a 584e 6f64 653e 206e 6f64 6573  or<ZXNode> nodes
-000062e0: 287f 3534 322c 3233 3138 380a 2020 2020  (.542,23188.    
-000062f0: 7374 643a 3a76 6563 746f 723c 7569 6e74  std::vector<uint
-00006300: 3332 5f74 3e20 696e 7075 7473 287f 3534  32_t> inputs(.54
-00006310: 342c 3233 3237 350a 2020 2020 7374 643a  4,23275.    std:
-00006320: 3a76 6563 746f 723c 7569 6e74 3332 5f74  :vector<uint32_t
-00006330: 3e20 6f75 7470 7574 7328 7f35 3436 2c32  > outputs(.546,2
-00006340: 3333 3637 0a20 2020 2073 7464 3a3a 7665  3367.    std::ve
-00006350: 6374 6f72 3c73 7464 3a3a 7665 6374 6f72  ctor<std::vector
-00006360: 3c5a 5845 6467 653e 3e20 6164 6a5f 6d61  <ZXEdge>> adj_ma
-00006370: 7428 7f35 3438 2c32 3334 3631 0a20 2020  t(.548,23461.   
-00006380: 2076 6f69 6420 6b69 6e64 287f 3535 302c   void kind(.550,
-00006390: 3233 3536 330a 2020 2020 766f 6964 2071  23563.    void q
-000063a0: 7562 6974 5f6e 756d 287f 3535 322c 3233  ubit_num(.552,23
-000063b0: 3635 340a 2020 2020 766f 6964 206e 6f64  654.    void nod
-000063c0: 6573 287f 3535 342c 3233 3735 360a 2020  es(.554,23756.  
-000063d0: 2020 766f 6964 2069 6e70 7574 7328 7f35    void inputs(.5
-000063e0: 3536 2c32 3338 3535 0a20 2020 2076 6f69  56,23855.    voi
-000063f0: 6420 6f75 7470 7574 7328 7f35 3538 2c32  d outputs(.558,2
-00006400: 3339 3631 0a20 2020 2076 6f69 6420 6164  3961.    void ad
-00006410: 6a5f 6d61 7428 7f35 3630 2c32 3430 3731  j_mat(.560,24071
-00006420: 0a20 2020 2076 6f69 6420 7368 6f77 287f  .    void show(.
-00006430: 3537 302c 3234 3337 340a 2020 2020 7374  570,24374.    st
-00006440: 643a 3a6d 6170 3c7f 7374 643a 3a6d 6170  d::map<.std::map
-00006450: 0135 3735 2c32 3435 3336 0a20 2020 2075  .575,24536.    u
-00006460: 696e 7433 325f 7420 7370 6964 6572 5f63  int32_t spider_c
-00006470: 6f75 6e74 287f 3538 392c 3234 3933 360a  ount(.589,24936.
-00006480: 2020 2020 7569 6e74 3332 5f74 206e 6f6e      uint32_t non
-00006490: 5f63 6c69 6666 6f72 645f 636f 756e 7428  _clifford_count(
-000064a0: 7f35 3933 2c32 3530 3838 0a20 2020 2066  .593,25088.    f
-000064b0: 7269 656e 6420 7374 643a 3a6f 7374 7265  riend std::ostre
-000064c0: 616d 2620 6f70 6572 6174 6f72 3c3c 287f  am& operator<<(.
-000064d0: 3638 332c 3237 3932 380a 0c0a 6578 7472  683,27928...extr
-000064e0: 6163 745f 7163 6972 632e 6370 702c 3436  act_qcirc.cpp,46
-000064f0: 350a 766f 6964 2053 6861 7271 6974 3a3a  5.void Sharqit::
-00006500: 5a58 4469 6167 7261 6d3a 3a70 6572 6d75  ZXDiagram::permu
-00006510: 7461 7469 6f6e 5f61 735f 7377 6170 287f  tation_as_swap(.
-00006520: 7065 726d 7574 6174 696f 6e5f 6173 5f73  permutation_as_s
-00006530: 7761 7001 382c 3135 310a 7374 643a 3a76  wap.8,151.std::v
-00006540: 6563 746f 723c 7374 643a 3a70 6169 723c  ector<std::pair<
-00006550: 7569 6e74 3332 5f74 2c20 7569 6e74 3332  uint32_t, uint32
-00006560: 5f74 3e3e 2053 6861 7271 6974 3a3a 5a58  _t>> Sharqit::ZX
-00006570: 4469 6167 7261 6d3a 3a65 7874 7261 6374  Diagram::extract
-00006580: 5f32 715f 636f 6e6e 6563 7473 287f 6578  _2q_connects(.ex
-00006590: 7472 6163 745f 3271 5f63 6f6e 6e65 6374  tract_2q_connect
-000065a0: 7301 3238 2c36 3237 0a62 6f6f 6c20 5368  s.28,627.bool Sh
-000065b0: 6172 7169 743a 3a5a 5844 6961 6772 616d  arqit::ZXDiagram
-000065c0: 3a3a 7570 6461 7465 5f66 726f 6e74 6965  ::update_frontie
-000065d0: 7228 7f75 7064 6174 655f 6672 6f6e 7469  r(.update_fronti
-000065e0: 6572 0138 362c 3232 3831 0a62 6f6f 6c20  er.86,2281.bool 
-000065f0: 5368 6172 7169 743a 3a5a 5844 6961 6772  Sharqit::ZXDiagr
-00006600: 616d 3a3a 7570 6461 7465 5f66 726f 6e74  am::update_front
-00006610: 6965 725f 7067 287f 7570 6461 7465 5f66  ier_pg(.update_f
-00006620: 726f 6e74 6965 725f 7067 0132 3235 2c36  rontier_pg.225,6
-00006630: 3430 380a 766f 6964 2053 6861 7271 6974  408.void Sharqit
-00006640: 3a3a 5a58 4469 6167 7261 6d3a 3a70 726f  ::ZXDiagram::pro
-00006650: 6365 7373 5f66 726f 6e74 6965 7228 7f70  cess_frontier(.p
-00006660: 726f 6365 7373 5f66 726f 6e74 6965 7201  rocess_frontier.
-00006670: 3330 352c 3930 3038 0a53 6861 7271 6974  305,9008.Sharqit
-00006680: 3a3a 5143 6972 6320 5368 6172 7169 743a  ::QCirc Sharqit:
-00006690: 3a5a 5844 6961 6772 616d 3a3a 6578 7472  :ZXDiagram::extr
-000066a0: 6163 745f 7163 6972 6328 7f65 7874 7261  act_qcirc(.extra
-000066b0: 6374 5f71 6369 7263 0133 3533 2c31 3035  ct_qcirc.353,105
-000066c0: 3935 0a                                  95.
+00000000: 0c0a 7072 6f70 6167 6174 655f 7061 756c  ..propagate_paul
+00000010: 695f 782e 6370 702c 3634 0a76 6f69 6420  i_x.cpp,64.void 
+00000020: 5368 6172 7169 743a 3a51 4369 7263 3a3a  Sharqit::QCirc::
+00000030: 7072 6f70 6167 6174 655f 7061 756c 695f  propagate_pauli_
+00000040: 7828 7f70 726f 7061 6761 7465 5f70 6175  x(.propagate_pau
+00000050: 6c69 5f78 0139 2c31 3938 0a0c 0a6e 625f  li_x.9,198...nb_
+00000060: 7368 6172 7169 742e 6370 702c 3138 0a4e  sharqit.cpp,18.N
+00000070: 425f 4d4f 4455 4c45 287f 3230 2c34 3139  B_MODULE(.20,419
+00000080: 0a0c 0a6c 696e 6561 725f 6d61 702e 682c  ...linear_map.h,
+00000090: 3638 370a 2364 6566 696e 6520 4c49 4e45  687.#define LINE
+000000a0: 4152 5f4d 4150 5f48 7f37 2c39 340a 6e61  AR_MAP_H.7,94.na
+000000b0: 6d65 7370 6163 6520 5368 6172 7169 7420  mespace Sharqit 
+000000c0: 7f31 362c 3231 340a 2020 636c 6173 7320  .16,214.  class 
+000000d0: 4c69 6e65 6172 4d61 7020 7f32 342c 3337  LinearMap .24,37
+000000e0: 300a 2020 2020 4c69 6e65 6172 4d61 7028  0.    LinearMap(
+000000f0: 7f33 332c 3636 350a 2020 2020 4c69 6e65  .33,665.    Line
+00000100: 6172 4d61 7028 7f33 392c 3931 380a 2020  arMap(.39,918.  
+00000110: 2020 4c69 6e65 6172 4d61 7028 7f35 332c    LinearMap(.53,
+00000120: 3133 3337 0a20 2020 2075 696e 7433 325f  1337.    uint32_
+00000130: 7420 726f 775f 6e75 6d28 7f35 382c 3135  t row_num(.58,15
+00000140: 3236 0a20 2020 2075 696e 7433 325f 7420  26.    uint32_t 
+00000150: 636f 6c5f 6e75 6d28 7f36 332c 3136 3930  col_num(.63,1690
+00000160: 0a20 2020 204c 696e 6561 724d 6170 2620  .    LinearMap& 
+00000170: 6f70 6572 6174 6f72 3d28 7f6f 7065 7261  operator=(.opera
+00000180: 746f 723d 0131 3031 2c33 3131 390a 2020  tor=.101,3119.  
+00000190: 2020 4c69 6e65 6172 4d61 7020 6f70 6572    LinearMap oper
+000001a0: 6174 6f72 2b28 7f31 3036 2c33 3237 300a  ator+(.106,3270.
+000001b0: 2020 2020 4c69 6e65 6172 4d61 7020 6f70      LinearMap op
+000001c0: 6572 6174 6f72 2d28 7f31 3037 2c33 3332  erator-(.107,332
+000001d0: 300a 2020 2020 6672 6965 6e64 204c 696e  0.    friend Lin
+000001e0: 6561 724d 6170 206f 7065 7261 746f 722b  earMap operator+
+000001f0: 287f 3130 382c 3333 3739 0a20 2020 2066  (.108,3379.    f
+00000200: 7269 656e 6420 4c69 6e65 6172 4d61 7020  riend LinearMap 
+00000210: 6f70 6572 6174 6f72 2d28 7f31 3039 2c33  operator-(.109,3
+00000220: 3530 330a 2020 2020 6672 6965 6e64 204c  503.    friend L
+00000230: 696e 6561 724d 6170 206f 7065 7261 746f  inearMap operato
+00000240: 722a 287f 3131 302c 3336 3237 0a20 2020  r*(.110,3627.   
+00000250: 2066 7269 656e 6420 4c69 6e65 6172 4d61   friend LinearMa
+00000260: 7020 6f70 6572 6174 6f72 2a28 7f31 3131  p operator*(.111
+00000270: 2c33 3735 310a 2020 2020 6672 6965 6e64  ,3751.    friend
+00000280: 204c 696e 6561 724d 6170 206f 7065 7261   LinearMap opera
+00000290: 746f 722a 287f 3131 322c 3338 3731 0a20  tor*(.112,3871. 
+000002a0: 2020 2066 7269 656e 6420 4c69 6e65 6172     friend Linear
+000002b0: 4d61 7020 6f70 6572 6174 6f72 2a28 7f31  Map operator*(.1
+000002c0: 3133 2c34 3030 350a 2020 2020 6672 6965  13,4005.    frie
+000002d0: 6e64 204c 696e 6561 724d 6170 206f 7065  nd LinearMap ope
+000002e0: 7261 746f 722a 287f 3131 342c 3431 3235  rator*(.114,4125
+000002f0: 0a20 2020 2066 7269 656e 6420 4c69 6e65  .    friend Line
+00000300: 6172 4d61 7020 6f70 6572 6174 6f72 2f28  arMap operator/(
+00000310: 7f31 3135 2c34 3235 390a 2020 2020 6672  .115,4259.    fr
+00000320: 6965 6e64 204c 696e 6561 724d 6170 206f  iend LinearMap o
+00000330: 7065 7261 746f 722f 287f 3131 362c 3433  perator/(.116,43
+00000340: 3739 0a0c 0a73 616e 6462 6f78 2f67 6175  79...sandbox/gau
+00000350: 7373 5f72 6564 7563 652f 6d61 696e 2e63  ss_reduce/main.c
+00000360: 7070 2c31 370a 696e 7420 6d61 696e 287f  pp,17.int main(.
+00000370: 3430 2c35 3832 0a0c 0a73 616e 6462 6f78  40,582...sandbox
+00000380: 2f67 6175 7373 5f72 6564 7563 652f 6269  /gauss_reduce/bi
+00000390: 6e61 7279 5f6d 6174 7269 782e 682c 3735  nary_matrix.h,75
+000003a0: 310a 2364 6566 696e 6520 4752 5f48 7f32  1.#define GR_H.2
+000003b0: 2c31 330a 2020 636c 6173 7320 4269 6e61  ,13.  class Bina
+000003c0: 7279 4d61 7472 6978 7f32 342c 3335 360a  ryMatrix.24,356.
+000003d0: 2020 2020 7569 6e74 3332 5f74 2072 6f77      uint32_t row
+000003e0: 5f6e 756d 5f3b 7f32 372c 3339 320a 2020  _num_;.27,392.  
+000003f0: 2020 7569 6e74 3332 5f74 2063 6f6c 5f6e    uint32_t col_n
+00000400: 756d 5f3b 7f32 382c 3431 350a 2020 2020  um_;.28,415.    
+00000410: 7374 643a 3a76 6563 746f 723c 7374 643a  std::vector<std:
+00000420: 3a76 6563 746f 723c 7569 6e74 385f 743e  :vector<uint8_t>
+00000430: 3e20 656c 656d 656e 7473 5f3b 7f32 392c  > elements_;.29,
+00000440: 3433 380a 2020 2020 7374 643a 3a76 6563  438.    std::vec
+00000450: 746f 723c 7569 6e74 3332 5f74 3e20 726f  tor<uint32_t> ro
+00000460: 775f 696e 6465 7865 735f 3b7f 3330 2c34  w_indexes_;.30,4
+00000470: 3837 0a20 2020 2042 696e 6172 794d 6174  87.    BinaryMat
+00000480: 7269 7828 7f33 322c 3533 370a 2020 2020  rix(.32,537.    
+00000490: 4269 6e61 7279 4d61 7472 6978 287f 3337  BinaryMatrix(.37
+000004a0: 2c38 3139 0a20 2020 2042 696e 6172 794d  ,819.    BinaryM
+000004b0: 6174 7269 7828 7f34 342c 3130 3731 0a20  atrix(.44,1071. 
+000004c0: 2020 2075 696e 7433 325f 7420 726f 775f     uint32_t row_
+000004d0: 6e75 6d28 7f34 372c 3132 3431 0a20 2020  num(.47,1241.   
+000004e0: 2075 696e 7433 325f 7420 636f 6c5f 6e75   uint32_t col_nu
+000004f0: 6d28 7f34 382c 3132 3931 0a20 2020 2073  m(.48,1291.    s
+00000500: 7464 3a3a 7665 6374 6f72 3c73 7464 3a3a  td::vector<std::
+00000510: 7665 6374 6f72 3c75 696e 7438 5f74 3e3e  vector<uint8_t>>
+00000520: 2065 6c65 6d65 6e74 7328 7f34 392c 3133   elements(.49,13
+00000530: 3431 0a20 2020 2073 7464 3a3a 7665 6374  41.    std::vect
+00000540: 6f72 3c75 696e 7433 325f 743e 2072 6f77  or<uint32_t> row
+00000550: 5f69 6e64 6578 6573 287f 3530 2c31 3431  _indexes(.50,141
+00000560: 390a 2020 2020 766f 6964 2072 6f77 5f6e  9.    void row_n
+00000570: 756d 287f 3532 2c31 3530 380a 2020 2020  um(.52,1508.    
+00000580: 766f 6964 2063 6f6c 5f6e 756d 287f 3533  void col_num(.53
+00000590: 2c31 3537 330a 2020 2020 766f 6964 2065  ,1573.    void e
+000005a0: 6c65 6d65 6e74 7328 7f35 342c 3136 3338  lements(.54,1638
+000005b0: 0a20 2020 2076 6f69 6420 726f 775f 696e  .    void row_in
+000005c0: 6465 7865 7328 7f35 352c 3137 3333 0a20  dexes(.55,1733. 
+000005d0: 2020 2076 6f69 6420 786f 725f 726f 7773     void xor_rows
+000005e0: 287f 3538 2c31 3839 300a 2020 2020 766f  (.58,1890.    vo
+000005f0: 6964 2073 7761 705f 726f 7773 287f 3637  id swap_rows(.67
+00000600: 2c32 3139 320a 2020 2020 766f 6964 2073  ,2192.    void s
+00000610: 7761 705f 636f 6c73 287f 3737 2c32 3531  wap_cols(.77,251
+00000620: 350a 2020 2020 626f 6f6c 2066 6561 7369  5.    bool feasi
+00000630: 626c 6528 7f38 362c 3237 3837 0a20 2020  ble(.86,2787.   
+00000640: 2073 7464 3a3a 7665 6374 6f72 3c7f 7374   std::vector<.st
+00000650: 643a 3a76 6563 746f 7201 3130 322c 3330  d::vector.102,30
+00000660: 3433 0a20 2020 2066 7269 656e 6420 7374  43.    friend st
+00000670: 643a 3a6f 7374 7265 616d 2620 6f70 6572  d::ostream& oper
+00000680: 6174 6f72 3c3c 287f 3130 332c 3331 3036  ator<<(.103,3106
+00000690: 0a0c 0a73 616e 6462 6f78 2f67 6175 7373  ...sandbox/gauss
+000006a0: 5f72 6564 7563 652f 6269 6e61 7279 5f6d  _reduce/binary_m
+000006b0: 6174 7269 782e 6370 702c 3135 370a 7374  atrix.cpp,157.st
+000006c0: 643a 3a73 7472 696e 6720 5368 6172 713a  d::string Sharq:
+000006d0: 3a42 696e 6172 794d 6174 7269 783a 3a74  :BinaryMatrix::t
+000006e0: 6f5f 7374 7269 6e67 287f 746f 5f73 7472  o_string(.to_str
+000006f0: 696e 6701 332c 3238 0a73 7464 3a3a 7665  ing.3,28.std::ve
+00000700: 6374 6f72 3c73 7464 3a3a 7061 6972 3c75  ctor<std::pair<u
+00000710: 696e 7433 325f 742c 2075 696e 7433 325f  int32_t, uint32_
+00000720: 743e 3e20 5368 6172 713a 3a42 696e 6172  t>> Sharq::Binar
+00000730: 794d 6174 7269 783a 3a67 6175 7373 5f72  yMatrix::gauss_r
+00000740: 6564 7563 6528 7f67 6175 7373 5f72 6564  educe(.gauss_red
+00000750: 7563 6501 3233 2c34 3033 0a0c 0a73 616e  uce.23,403...san
+00000760: 6462 6f78 2f67 6175 7373 5f72 6564 7563  dbox/gauss_reduc
+00000770: 652f 6f6c 642f 6d61 696e 2e63 7070 2c31  e/old/main.cpp,1
+00000780: 350a 696e 7420 6d61 696e 287f 332c 3238  5.int main(.3,28
+00000790: 0a0c 0a73 616e 6462 6f78 2f67 6175 7373  ...sandbox/gauss
+000007a0: 5f72 6564 7563 652f 6f6c 642f 6269 6e61  _reduce/old/bina
+000007b0: 7279 5f6d 6174 7269 782e 682c 3630 370a  ry_matrix.h,607.
+000007c0: 2364 6566 696e 6520 4752 5f48 7f32 2c31  #define GR_H.2,1
+000007d0: 330a 2020 636c 6173 7320 4269 6e61 7279  3.  class Binary
+000007e0: 4d61 7472 6978 7f32 342c 3335 360a 2020  Matrix.24,356.  
+000007f0: 2020 7569 6e74 3332 5f74 2072 6f77 5f6e    uint32_t row_n
+00000800: 756d 5f3b 7f32 372c 3339 320a 2020 2020  um_;.27,392.    
+00000810: 7569 6e74 3332 5f74 2063 6f6c 5f6e 756d  uint32_t col_num
+00000820: 5f3b 7f32 382c 3431 350a 2020 2020 7374  _;.28,415.    st
+00000830: 643a 3a76 6563 746f 723c 7374 643a 3a76  d::vector<std::v
+00000840: 6563 746f 723c 626f 6f6c 3e3e 2065 6c65  ector<bool>> ele
+00000850: 6d65 6e74 735f 3b7f 3239 2c34 3338 0a20  ments_;.29,438. 
+00000860: 2020 2073 7464 3a3a 7665 6374 6f72 3c75     std::vector<u
+00000870: 696e 7433 325f 743e 2072 6f77 5f69 6e64  int32_t> row_ind
+00000880: 6578 6573 5f3b 7f33 302c 3438 340a 2020  exes_;.30,484.  
+00000890: 2020 4269 6e61 7279 4d61 7472 6978 287f    BinaryMatrix(.
+000008a0: 3332 2c35 3334 0a20 2020 2042 696e 6172  32,534.    Binar
+000008b0: 794d 6174 7269 7828 7f33 372c 3739 320a  yMatrix(.37,792.
+000008c0: 2020 2020 7569 6e74 3332 5f74 2072 6f77      uint32_t row
+000008d0: 5f6e 756d 287f 3435 2c31 3035 380a 2020  _num(.45,1058.  
+000008e0: 2020 7569 6e74 3332 5f74 2063 6f6c 5f6e    uint32_t col_n
+000008f0: 756d 287f 3436 2c31 3130 380a 2020 2020  um(.46,1108.    
+00000900: 7374 643a 3a76 6563 746f 723c 7374 643a  std::vector<std:
+00000910: 3a76 6563 746f 723c 626f 6f6c 3e3e 2065  :vector<bool>> e
+00000920: 6c65 6d65 6e74 7328 7f34 372c 3131 3538  lements(.47,1158
+00000930: 0a20 2020 2073 7464 3a3a 7665 6374 6f72  .    std::vector
+00000940: 3c75 696e 7433 325f 743e 2072 6f77 5f69  <uint32_t> row_i
+00000950: 6e64 6578 6573 287f 3438 2c31 3233 330a  ndexes(.48,1233.
+00000960: 2020 2020 766f 6964 2072 6f77 5f6e 756d      void row_num
+00000970: 287f 3530 2c31 3332 320a 2020 2020 766f  (.50,1322.    vo
+00000980: 6964 2063 6f6c 5f6e 756d 287f 3531 2c31  id col_num(.51,1
+00000990: 3338 370a 2020 2020 766f 6964 2065 6c65  387.    void ele
+000009a0: 6d65 6e74 7328 7f35 322c 3134 3532 0a20  ments(.52,1452. 
+000009b0: 2020 2076 6f69 6420 726f 775f 696e 6465     void row_inde
+000009c0: 7865 7328 7f35 332c 3135 3434 0a20 2020  xes(.53,1544.   
+000009d0: 2073 7464 3a3a 7665 6374 6f72 3c7f 7374   std::vector<.st
+000009e0: 643a 3a76 6563 746f 7201 3538 2c31 3831  d::vector.58,181
+000009f0: 320a 2020 2020 6672 6965 6e64 2073 7464  2.    friend std
+00000a00: 3a3a 6f73 7472 6561 6d26 206f 7065 7261  ::ostream& opera
+00000a10: 746f 723c 3c28 7f35 392c 3138 3735 0a0c  tor<<(.59,1875..
+00000a20: 0a73 616e 6462 6f78 2f67 6175 7373 5f72  .sandbox/gauss_r
+00000a30: 6564 7563 652f 6f6c 642f 6269 6e61 7279  educe/old/binary
+00000a40: 5f6d 6174 7269 785f 626b 3230 3233 3132  _matrix_bk202312
+00000a50: 3039 2e63 7070 2c33 3732 0a73 7464 3a3a  09.cpp,372.std::
+00000a60: 7374 7269 6e67 2053 6861 7271 3a3a 4269  string Sharq::Bi
+00000a70: 6e61 7279 4d61 7472 6978 3a3a 746f 5f73  naryMatrix::to_s
+00000a80: 7472 696e 6728 7f74 6f5f 7374 7269 6e67  tring(.to_string
+00000a90: 0133 2c32 380a 766f 6964 2053 6861 7271  .3,28.void Sharq
+00000aa0: 3a3a 4269 6e61 7279 4d61 7472 6978 3a3a  ::BinaryMatrix::
+00000ab0: 786f 725f 726f 7773 287f 786f 725f 726f  xor_rows(.xor_ro
+00000ac0: 7773 0132 332c 3430 330a 766f 6964 2053  ws.23,403.void S
+00000ad0: 6861 7271 3a3a 4269 6e61 7279 4d61 7472  harq::BinaryMatr
+00000ae0: 6978 3a3a 7377 6170 5f72 6f77 7328 7f73  ix::swap_rows(.s
+00000af0: 7761 705f 726f 7773 0133 332c 3730 350a  wap_rows.33,705.
+00000b00: 766f 6964 2053 6861 7271 3a3a 4269 6e61  void Sharq::Bina
+00000b10: 7279 4d61 7472 6978 3a3a 7377 6170 5f63  ryMatrix::swap_c
+00000b20: 6f6c 7328 7f73 7761 705f 636f 6c73 0134  ols(.swap_cols.4
+00000b30: 342c 3130 3234 0a62 6f6f 6c20 5368 6172  4,1024.bool Shar
+00000b40: 713a 3a42 696e 6172 794d 6174 7269 783a  q::BinaryMatrix:
+00000b50: 3a66 6561 7369 626c 6528 7f66 6561 7369  :feasible(.feasi
+00000b60: 626c 6501 3534 2c31 3239 360a 7374 643a  ble.54,1296.std:
+00000b70: 3a76 6563 746f 723c 7374 643a 3a70 6169  :vector<std::pai
+00000b80: 723c 7569 6e74 3332 5f74 2c20 7569 6e74  r<uint32_t, uint
+00000b90: 3332 5f74 3e3e 2053 6861 7271 3a3a 4269  32_t>> Sharq::Bi
+00000ba0: 6e61 7279 4d61 7472 6978 3a3a 6761 7573  naryMatrix::gaus
+00000bb0: 735f 7265 6475 6365 287f 6761 7573 735f  s_reduce(.gauss_
+00000bc0: 7265 6475 6365 0137 312c 3135 3632 0a0c  reduce.71,1562..
+00000bd0: 0a73 616e 6462 6f78 2f67 6175 7373 5f72  .sandbox/gauss_r
+00000be0: 6564 7563 652f 6f6c 642f 6269 6e61 7279  educe/old/binary
+00000bf0: 5f6d 6174 7269 785f 626b 3230 3233 3132  _matrix_bk202312
+00000c00: 3039 2e68 2c36 3339 0a23 6465 6669 6e65  09.h,639.#define
+00000c10: 2047 525f 487f 322c 3133 0a20 2063 6c61   GR_H.2,13.  cla
+00000c20: 7373 2042 696e 6172 794d 6174 7269 787f  ss BinaryMatrix.
+00000c30: 3234 2c33 3536 0a20 2020 2075 696e 7433  24,356.    uint3
+00000c40: 325f 7420 726f 775f 6e75 6d5f 3b7f 3237  2_t row_num_;.27
+00000c50: 2c33 3932 0a20 2020 2075 696e 7433 325f  ,392.    uint32_
+00000c60: 7420 636f 6c5f 6e75 6d5f 3b7f 3238 2c34  t col_num_;.28,4
+00000c70: 3135 0a20 2020 2073 7464 3a3a 7665 6374  15.    std::vect
+00000c80: 6f72 3c73 7464 3a3a 7665 6374 6f72 3c75  or<std::vector<u
+00000c90: 696e 7438 5f74 3e3e 2065 6c65 6d65 6e74  int8_t>> element
+00000ca0: 735f 3b7f 3239 2c34 3338 0a20 2020 2073  s_;.29,438.    s
+00000cb0: 7464 3a3a 7665 6374 6f72 3c75 696e 7433  td::vector<uint3
+00000cc0: 325f 743e 2072 6f77 5f69 6e64 6578 6573  2_t> row_indexes
+00000cd0: 5f3b 7f33 302c 3438 370a 2020 2020 4269  _;.30,487.    Bi
+00000ce0: 6e61 7279 4d61 7472 6978 287f 3332 2c35  naryMatrix(.32,5
+00000cf0: 3337 0a20 2020 2042 696e 6172 794d 6174  37.    BinaryMat
+00000d00: 7269 7828 7f33 372c 3831 390a 2020 2020  rix(.37,819.    
+00000d10: 4269 6e61 7279 4d61 7472 6978 287f 3434  BinaryMatrix(.44
+00000d20: 2c31 3037 310a 2020 2020 7569 6e74 3332  ,1071.    uint32
+00000d30: 5f74 2072 6f77 5f6e 756d 287f 3437 2c31  _t row_num(.47,1
+00000d40: 3234 310a 2020 2020 7569 6e74 3332 5f74  241.    uint32_t
+00000d50: 2063 6f6c 5f6e 756d 287f 3438 2c31 3239   col_num(.48,129
+00000d60: 310a 2020 2020 7374 643a 3a76 6563 746f  1.    std::vecto
+00000d70: 723c 7374 643a 3a76 6563 746f 723c 7569  r<std::vector<ui
+00000d80: 6e74 385f 743e 3e20 656c 656d 656e 7473  nt8_t>> elements
+00000d90: 287f 3439 2c31 3334 310a 2020 2020 7374  (.49,1341.    st
+00000da0: 643a 3a76 6563 746f 723c 7569 6e74 3332  d::vector<uint32
+00000db0: 5f74 3e20 726f 775f 696e 6465 7865 7328  _t> row_indexes(
+00000dc0: 7f35 302c 3134 3139 0a20 2020 2076 6f69  .50,1419.    voi
+00000dd0: 6420 726f 775f 6e75 6d28 7f35 322c 3135  d row_num(.52,15
+00000de0: 3038 0a20 2020 2076 6f69 6420 636f 6c5f  08.    void col_
+00000df0: 6e75 6d28 7f35 332c 3135 3733 0a20 2020  num(.53,1573.   
+00000e00: 2076 6f69 6420 656c 656d 656e 7473 287f   void elements(.
+00000e10: 3534 2c31 3633 380a 2020 2020 766f 6964  54,1638.    void
+00000e20: 2072 6f77 5f69 6e64 6578 6573 287f 3535   row_indexes(.55
+00000e30: 2c31 3733 330a 2020 2020 7374 643a 3a76  ,1733.    std::v
+00000e40: 6563 746f 723c 7f73 7464 3a3a 7665 6374  ector<.std::vect
+00000e50: 6f72 0136 322c 3230 3834 0a20 2020 2066  or.62,2084.    f
+00000e60: 7269 656e 6420 7374 643a 3a6f 7374 7265  riend std::ostre
+00000e70: 616d 2620 6f70 6572 6174 6f72 3c3c 287f  am& operator<<(.
+00000e80: 3633 2c32 3134 370a 0c0a 7361 6e64 626f  63,2147...sandbo
+00000e90: 782f 6761 7573 735f 7265 6475 6365 2f6f  x/gauss_reduce/o
+00000ea0: 6c64 2f62 696e 6172 795f 6d61 7472 6978  ld/binary_matrix
+00000eb0: 2e63 7070 2c32 3634 0a73 7464 3a3a 7374  .cpp,264.std::st
+00000ec0: 7269 6e67 2053 6861 7271 3a3a 4269 6e61  ring Sharq::Bina
+00000ed0: 7279 4d61 7472 6978 3a3a 746f 5f73 7472  ryMatrix::to_str
+00000ee0: 696e 6728 7f74 6f5f 7374 7269 6e67 0133  ing(.to_string.3
+00000ef0: 2c32 380a 766f 6964 2053 6861 7271 3a3a  ,28.void Sharq::
+00000f00: 4269 6e61 7279 4d61 7472 6978 3a3a 786f  BinaryMatrix::xo
+00000f10: 725f 726f 7773 287f 786f 725f 726f 7773  r_rows(.xor_rows
+00000f20: 0132 332c 3338 370a 766f 6964 2053 6861  .23,387.void Sha
+00000f30: 7271 3a3a 4269 6e61 7279 4d61 7472 6978  rq::BinaryMatrix
+00000f40: 3a3a 7377 6170 5f72 6f77 7328 7f73 7761  ::swap_rows(.swa
+00000f50: 705f 726f 7773 0133 332c 3638 360a 7374  p_rows.33,686.st
+00000f60: 643a 3a76 6563 746f 723c 7374 643a 3a70  d::vector<std::p
+00000f70: 6169 723c 7569 6e74 3332 5f74 2c20 7569  air<uint32_t, ui
+00000f80: 6e74 3332 5f74 3e3e 2053 6861 7271 3a3a  nt32_t>> Sharq::
+00000f90: 4269 6e61 7279 4d61 7472 6978 3a3a 6761  BinaryMatrix::ga
+00000fa0: 7573 735f 7265 6475 6365 287f 6761 7573  uss_reduce(.gaus
+00000fb0: 735f 7265 6475 6365 0134 342c 3130 3035  s_reduce.44,1005
+00000fc0: 0a0c 0a73 616e 6462 6f78 2f67 6175 7373  ...sandbox/gauss
+00000fd0: 5f72 6564 7563 652f 6f6c 642f 6269 6e61  _reduce/old/bina
+00000fe0: 7279 5f6d 6174 7269 785f 626b 3230 3233  ry_matrix_bk2023
+00000ff0: 3130 3231 2e63 7070 2c33 3732 0a73 7464  1021.cpp,372.std
+00001000: 3a3a 7374 7269 6e67 2053 6861 7271 3a3a  ::string Sharq::
+00001010: 4269 6e61 7279 4d61 7472 6978 3a3a 746f  BinaryMatrix::to
+00001020: 5f73 7472 696e 6728 7f74 6f5f 7374 7269  _string(.to_stri
+00001030: 6e67 0133 2c32 380a 766f 6964 2053 6861  ng.3,28.void Sha
+00001040: 7271 3a3a 4269 6e61 7279 4d61 7472 6978  rq::BinaryMatrix
+00001050: 3a3a 786f 725f 726f 7773 287f 786f 725f  ::xor_rows(.xor_
+00001060: 726f 7773 0132 332c 3338 370a 766f 6964  rows.23,387.void
+00001070: 2053 6861 7271 3a3a 4269 6e61 7279 4d61   Sharq::BinaryMa
+00001080: 7472 6978 3a3a 7377 6170 5f72 6f77 7328  trix::swap_rows(
+00001090: 7f73 7761 705f 726f 7773 0133 332c 3638  .swap_rows.33,68
+000010a0: 360a 766f 6964 2053 6861 7271 3a3a 4269  6.void Sharq::Bi
+000010b0: 6e61 7279 4d61 7472 6978 3a3a 7377 6170  naryMatrix::swap
+000010c0: 5f63 6f6c 7328 7f73 7761 705f 636f 6c73  _cols(.swap_cols
+000010d0: 0134 342c 3130 3035 0a62 6f6f 6c20 5368  .44,1005.bool Sh
+000010e0: 6172 713a 3a42 696e 6172 794d 6174 7269  arq::BinaryMatri
+000010f0: 783a 3a66 6561 7369 626c 6528 7f66 6561  x::feasible(.fea
+00001100: 7369 626c 6501 3534 2c31 3237 370a 7374  sible.54,1277.st
+00001110: 643a 3a76 6563 746f 723c 7374 643a 3a70  d::vector<std::p
+00001120: 6169 723c 7569 6e74 3332 5f74 2c20 7569  air<uint32_t, ui
+00001130: 6e74 3332 5f74 3e3e 2053 6861 7271 3a3a  nt32_t>> Sharq::
+00001140: 4269 6e61 7279 4d61 7472 6978 3a3a 6761  BinaryMatrix::ga
+00001150: 7573 735f 7265 6475 6365 287f 6761 7573  uss_reduce(.gaus
+00001160: 735f 7265 6475 6365 0137 312c 3135 3433  s_reduce.71,1543
+00001170: 0a0c 0a71 6369 7263 2e63 7070 2c31 3932  ...qcirc.cpp,192
+00001180: 310a 766f 6964 2053 6861 7271 6974 3a3a  1.void Sharqit::
+00001190: 5143 6972 633a 3a73 6176 6528 7f73 6176  QCirc::save(.sav
+000011a0: 6501 382c 3939 0a76 6f69 6420 5368 6172  e.8,99.void Shar
+000011b0: 7169 743a 3a51 4369 7263 3a3a 6c6f 6164  qit::QCirc::load
+000011c0: 287f 6c6f 6164 0132 302c 3331 360a 7374  (.load.20,316.st
+000011d0: 643a 3a6d 6170 3c73 7464 3a3a 7374 7269  d::map<std::stri
+000011e0: 6e67 2c20 7569 6e74 3332 5f74 3e20 5368  ng, uint32_t> Sh
+000011f0: 6172 7169 743a 3a51 4369 7263 3a3a 7374  arqit::QCirc::st
+00001200: 6174 7328 7f73 7461 7473 0136 372c 3135  ats(.stats.67,15
+00001210: 3832 0a76 6f69 6420 5368 6172 7169 743a  82.void Sharqit:
+00001220: 3a51 4369 7263 3a3a 7072 696e 745f 7374  :QCirc::print_st
+00001230: 6174 7328 7f70 7269 6e74 5f73 7461 7473  ats(.print_stats
+00001240: 0138 352c 3230 3738 0a75 696e 7433 325f  .85,2078.uint32_
+00001250: 7420 5368 6172 7169 743a 3a51 4369 7263  t Sharqit::QCirc
+00001260: 3a3a 6964 5f63 6f75 6e74 287f 6964 5f63  ::id_count(.id_c
+00001270: 6f75 6e74 0131 3031 2c32 3837 320a 7569  ount.101,2872.ui
+00001280: 6e74 3332 5f74 2053 6861 7271 6974 3a3a  nt32_t Sharqit::
+00001290: 5143 6972 633a 3a78 5f63 6f75 6e74 287f  QCirc::x_count(.
+000012a0: 785f 636f 756e 7401 3130 382c 3330 3132  x_count.108,3012
+000012b0: 0a75 696e 7433 325f 7420 5368 6172 7169  .uint32_t Sharqi
+000012c0: 743a 3a51 4369 7263 3a3a 7a5f 636f 756e  t::QCirc::z_coun
+000012d0: 7428 7f7a 5f63 6f75 6e74 0131 3135 2c33  t(.z_count.115,3
+000012e0: 3135 300a 7569 6e74 3332 5f74 2053 6861  150.uint32_t Sha
+000012f0: 7271 6974 3a3a 5143 6972 633a 3a68 5f63  rqit::QCirc::h_c
+00001300: 6f75 6e74 287f 685f 636f 756e 7401 3132  ount(.h_count.12
+00001310: 322c 3332 3838 0a75 696e 7433 325f 7420  2,3288.uint32_t 
+00001320: 5368 6172 7169 743a 3a51 4369 7263 3a3a  Sharqit::QCirc::
+00001330: 735f 636f 756e 7428 7f73 5f63 6f75 6e74  s_count(.s_count
+00001340: 0131 3239 2c33 3432 360a 7569 6e74 3332  .129,3426.uint32
+00001350: 5f74 2053 6861 7271 6974 3a3a 5143 6972  _t Sharqit::QCir
+00001360: 633a 3a74 5f63 6f75 6e74 287f 745f 636f  c::t_count(.t_co
+00001370: 756e 7401 3133 362c 3335 3634 0a75 696e  unt.136,3564.uin
+00001380: 7433 325f 7420 5368 6172 7169 743a 3a51  t32_t Sharqit::Q
+00001390: 4369 7263 3a3a 727a 5f63 6f75 6e74 287f  Circ::rz_count(.
+000013a0: 727a 5f63 6f75 6e74 0131 3433 2c33 3730  rz_count.143,370
+000013b0: 320a 7569 6e74 3332 5f74 2053 6861 7271  2.uint32_t Sharq
+000013c0: 6974 3a3a 5143 6972 633a 3a63 785f 636f  it::QCirc::cx_co
+000013d0: 756e 7428 7f63 785f 636f 756e 7401 3135  unt(.cx_count.15
+000013e0: 302c 3338 3432 0a75 696e 7433 325f 7420  0,3842.uint32_t 
+000013f0: 5368 6172 7169 743a 3a51 4369 7263 3a3a  Sharqit::QCirc::
+00001400: 637a 5f63 6f75 6e74 287f 637a 5f63 6f75  cz_count(.cz_cou
+00001410: 6e74 0131 3537 2c33 3938 320a 7569 6e74  nt.157,3982.uint
+00001420: 3332 5f74 2053 6861 7271 6974 3a3a 5143  32_t Sharqit::QC
+00001430: 6972 633a 3a64 6570 7468 287f 6465 7074  irc::depth(.dept
+00001440: 6801 3136 342c 3431 3232 0a73 7464 3a3a  h.164,4122.std::
+00001450: 7374 7269 6e67 2053 6861 7271 6974 3a3a  string Sharqit::
+00001460: 5143 6972 633a 3a74 6f5f 7374 7269 6e67  QCirc::to_string
+00001470: 287f 746f 5f73 7472 696e 6701 3138 382c  (.to_string.188,
+00001480: 3436 3334 0a53 6861 7271 6974 3a3a 5143  4634.Sharqit::QC
+00001490: 6972 6326 2053 6861 7271 6974 3a3a 5143  irc& Sharqit::QC
+000014a0: 6972 633a 3a61 6464 5f71 6761 7465 287f  irc::add_qgate(.
+000014b0: 6164 645f 7167 6174 6501 3337 342c 3130  add_qgate.374,10
+000014c0: 3531 360a 5368 6172 7169 743a 3a51 4369  516.Sharqit::QCi
+000014d0: 7263 2620 5368 6172 7169 743a 3a51 4369  rc& Sharqit::QCi
+000014e0: 7263 3a3a 6164 645f 7167 6174 6528 7f61  rc::add_qgate(.a
+000014f0: 6464 5f71 6761 7465 0133 3834 2c31 3037  dd_qgate.384,107
+00001500: 3239 0a53 6861 7271 6974 3a3a 5143 6972  29.Sharqit::QCir
+00001510: 6326 2053 6861 7271 6974 3a3a 5143 6972  c& Sharqit::QCir
+00001520: 633a 3a61 6464 5f71 6369 7263 287f 6164  c::add_qcirc(.ad
+00001530: 645f 7163 6972 6301 3339 362c 3131 3033  d_qcirc.396,1103
+00001540: 380a 5368 6172 7169 743a 3a51 4369 7263  8.Sharqit::QCirc
+00001550: 2620 5368 6172 7169 743a 3a51 4369 7263  & Sharqit::QCirc
+00001560: 3a3a 6164 645f 7261 6e64 6f6d 287f 6164  ::add_random(.ad
+00001570: 645f 7261 6e64 6f6d 0134 3034 2c31 3131  d_random.404,111
+00001580: 3834 0a53 6861 7271 6974 3a3a 5143 6972  84.Sharqit::QCir
+00001590: 6326 2053 6861 7271 6974 3a3a 5143 6972  c& Sharqit::QCir
+000015a0: 633a 3a61 6464 5f72 616e 646f 6d5f 7374  c::add_random_st
+000015b0: 7228 7f61 6464 5f72 616e 646f 6d5f 7374  r(.add_random_st
+000015c0: 7201 3437 362c 3133 3631 390a 5368 6172  r.476,13619.Shar
+000015d0: 7169 743a 3a51 4369 7263 2053 6861 7271  qit::QCirc Sharq
+000015e0: 6974 3a3a 5143 6972 633a 3a72 6576 6572  it::QCirc::rever
+000015f0: 7365 287f 7265 7665 7273 6501 3439 302c  se(.reverse.490,
+00001600: 3134 3136 310a 5368 6172 7169 743a 3a51  14161.Sharqit::Q
+00001610: 4369 7263 2053 6861 7271 6974 3a3a 5143  Circ Sharqit::QC
+00001620: 6972 633a 3a69 6e76 6572 7365 287f 696e  irc::inverse(.in
+00001630: 7665 7273 6501 3530 302c 3134 3338 310a  verse.500,14381.
+00001640: 626f 6f6c 2053 6861 7271 6974 3a3a 5143  bool Sharqit::QC
+00001650: 6972 633a 3a69 735f 6964 656e 7469 6361  irc::is_identica
+00001660: 6c28 7f69 735f 6964 656e 7469 6361 6c01  l(.is_identical.
+00001670: 3531 302c 3134 3631 310a 626f 6f6c 2053  510,14611.bool S
+00001680: 6861 7271 6974 3a3a 5143 6972 633a 3a69  harqit::QCirc::i
+00001690: 735f 6571 7561 6c28 7f69 735f 6571 7561  s_equal(.is_equa
+000016a0: 6c01 3531 392c 3134 3835 340a 766f 6964  l.519,14854.void
+000016b0: 2053 6861 7271 6974 3a3a 5143 6972 633a   Sharqit::QCirc:
+000016c0: 3a74 6f5f 646f 745f 6669 6c65 287f 746f  :to_dot_file(.to
+000016d0: 5f64 6f74 5f66 696c 6501 3536 322c 3136  _dot_file.562,16
+000016e0: 3231 350a 766f 6964 2053 6861 7271 6974  215.void Sharqit
+000016f0: 3a3a 5143 6972 633a 3a74 6f5f 7376 675f  ::QCirc::to_svg_
+00001700: 6669 6c65 287f 746f 5f73 7667 5f66 696c  file(.to_svg_fil
+00001710: 6501 3736 392c 3233 3233 390a 5368 6172  e.769,23239.Shar
+00001720: 7169 743a 3a5a 5844 6961 6772 616d 2053  qit::ZXDiagram S
+00001730: 6861 7271 6974 3a3a 5143 6972 633a 3a74  harqit::QCirc::t
+00001740: 6f5f 7a78 6469 6167 7261 6d28 7f74 6f5f  o_zxdiagram(.to_
+00001750: 7a78 6469 6167 7261 6d01 3738 312c 3233  zxdiagram.781,23
+00001760: 3730 350a 5368 6172 7169 743a 3a4c 696e  705.Sharqit::Lin
+00001770: 6561 724d 6170 2053 6861 7271 6974 3a3a  earMap Sharqit::
+00001780: 5143 6972 633a 3a74 6f5f 6c69 6e65 6172  QCirc::to_linear
+00001790: 6d61 7028 7f74 6f5f 6c69 6e65 6172 6d61  map(.to_linearma
+000017a0: 7001 3739 392c 3234 3138 350a 5368 6172  p.799,24185.Shar
+000017b0: 7169 743a 3a44 4147 4369 7263 2053 6861  qit::DAGCirc Sha
+000017c0: 7271 6974 3a3a 5143 6972 633a 3a74 6f5f  rqit::QCirc::to_
+000017d0: 6461 6763 6972 6328 7f74 6f5f 6461 6763  dagcirc(.to_dagc
+000017e0: 6972 6301 3830 382c 3234 3338 320a 766f  irc.808,24382.vo
+000017f0: 6964 2053 6861 7271 6974 3a3a 5143 6972  id Sharqit::QCir
+00001800: 633a 3a63 7a5f 746f 5f63 7828 7f63 7a5f  c::cz_to_cx(.cz_
+00001810: 746f 5f63 7801 3831 352c 3234 3534 340a  to_cx.815,24544.
+00001820: 766f 6964 2053 6861 7271 6974 3a3a 5143  void Sharqit::QC
+00001830: 6972 633a 3a64 6563 6f6d 705f 746f 6628  irc::decomp_tof(
+00001840: 7f64 6563 6f6d 705f 746f 6601 3833 332c  .decomp_tof.833,
+00001850: 3235 3131 390a 626f 6f6c 2053 6861 7271  25119.bool Sharq
+00001860: 6974 3a3a 5143 6972 633a 3a69 6e63 6c75  it::QCirc::inclu
+00001870: 6465 5f74 6f66 287f 696e 636c 7564 655f  de_tof(.include_
+00001880: 746f 6601 3837 332c 3236 3031 380a 766f  tof.873,26018.vo
+00001890: 6964 2053 6861 7271 6974 3a3a 5143 6972  id Sharqit::QCir
+000018a0: 633a 3a72 656d 6f76 655f 6964 287f 7265  c::remove_id(.re
+000018b0: 6d6f 7665 5f69 6401 3838 322c 3236 3230  move_id.882,2620
+000018c0: 340a 766f 6964 2020 5368 6172 7169 743a  4.void  Sharqit:
+000018d0: 3a51 4369 7263 3a3a 7265 706c 6163 655f  :QCirc::replace_
+000018e0: 7769 7468 5f72 7a28 7f72 6570 6c61 6365  with_rz(.replace
+000018f0: 5f77 6974 685f 727a 0138 3936 2c32 3637  _with_rz.896,267
+00001900: 3531 0a0c 0a70 6861 7365 2e63 7070 2c39  51...phase.cpp,9
+00001910: 300a 5368 6172 7169 743a 3a50 6861 7365  0.Sharqit::Phase
+00001920: 3a3a 5068 6173 6528 7f50 6861 7365 0138  ::Phase(.Phase.8
+00001930: 2c39 300a 7374 643a 3a73 7472 696e 6720  ,90.std::string 
+00001940: 5368 6172 7169 743a 3a50 6861 7365 3a3a  Sharqit::Phase::
+00001950: 746f 5f73 7472 696e 6728 7f74 6f5f 7374  to_string(.to_st
+00001960: 7269 6e67 0133 312c 3734 340a 0c0a 6d65  ring.31,744...me
+00001970: 7267 655f 726f 7461 7469 6f6e 2e63 7070  rge_rotation.cpp
+00001980: 2c32 3039 0a62 6f6f 6c20 5368 6172 7169  ,209.bool Sharqi
+00001990: 743a 3a51 4369 7263 3a3a 6973 5f74 6572  t::QCirc::is_ter
+000019a0: 6d69 6e61 7469 6f6e 5f62 6f72 6465 7228  mination_border(
+000019b0: 7f69 735f 7465 726d 696e 6174 696f 6e5f  .is_termination_
+000019c0: 626f 7264 6572 0138 2c31 3438 0a76 6f69  border.8,148.voi
+000019d0: 6420 5368 6172 7169 743a 3a51 4369 7263  d Sharqit::QCirc
+000019e0: 3a3a 6d65 7267 655f 726f 7461 7469 6f6e  ::merge_rotation
+000019f0: 5f6f 6e65 5f74 696d 6528 7f6d 6572 6765  _one_time(.merge
+00001a00: 5f72 6f74 6174 696f 6e5f 6f6e 655f 7469  _rotation_one_ti
+00001a10: 6d65 0131 382c 3431 320a 766f 6964 2053  me.18,412.void S
+00001a20: 6861 7271 6974 3a3a 5143 6972 633a 3a6d  harqit::QCirc::m
+00001a30: 6572 6765 5f72 6f74 6174 696f 6e28 7f6d  erge_rotation(.m
+00001a40: 6572 6765 5f72 6f74 6174 696f 6e01 3832  erge_rotation.82
+00001a50: 2c32 3630 310a 0c0a 6269 6e61 7279 5f6d  ,2601...binary_m
+00001a60: 6174 7269 782e 682c 3833 370a 2364 6566  atrix.h,837.#def
+00001a70: 696e 6520 4249 4e41 5259 5f4d 4154 5249  ine BINARY_MATRI
+00001a80: 585f 487f 372c 3130 330a 2020 636c 6173  X_H.7,103.  clas
+00001a90: 7320 4269 6e61 7279 4d61 7472 6978 7f32  s BinaryMatrix.2
+00001aa0: 302c 3238 370a 2020 2020 7569 6e74 3332  0,287.    uint32
+00001ab0: 5f74 2072 6f77 5f6e 756d 5f3b 7f32 332c  _t row_num_;.23,
+00001ac0: 3332 330a 2020 2020 7569 6e74 3332 5f74  323.    uint32_t
+00001ad0: 2063 6f6c 5f6e 756d 5f3b 7f32 342c 3337   col_num_;.24,37
+00001ae0: 360a 2020 2020 7374 643a 3a76 6563 746f  6.    std::vecto
+00001af0: 723c 7374 643a 3a76 6563 746f 723c 7569  r<std::vector<ui
+00001b00: 6e74 385f 743e 3e20 656c 656d 656e 7473  nt8_t>> elements
+00001b10: 5f3b 7f32 352c 3433 320a 2020 2020 7374  _;.25,432.    st
+00001b20: 643a 3a76 6563 746f 723c 7569 6e74 3332  d::vector<uint32
+00001b30: 5f74 3e20 726f 775f 696e 6465 7865 735f  _t> row_indexes_
+00001b40: 3b7f 3236 2c35 3333 0a20 2020 2042 696e  ;.26,533.    Bin
+00001b50: 6172 794d 6174 7269 7828 7f33 342c 3836  aryMatrix(.34,86
+00001b60: 310a 2020 2020 4269 6e61 7279 4d61 7472  1.    BinaryMatr
+00001b70: 6978 287f 3433 2c31 3235 360a 2020 2020  ix(.43,1256.    
+00001b80: 4269 6e61 7279 4d61 7472 6978 287f 3534  BinaryMatrix(.54
+00001b90: 2c31 3631 350a 2020 2020 7569 6e74 3332  ,1615.    uint32
+00001ba0: 5f74 2072 6f77 5f6e 756d 287f 3537 2c31  _t row_num(.57,1
+00001bb0: 3739 390a 2020 2020 7569 6e74 3332 5f74  799.    uint32_t
+00001bc0: 2063 6f6c 5f6e 756d 287f 3539 2c31 3838   col_num(.59,188
+00001bd0: 300a 2020 2020 7374 643a 3a76 6563 746f  0.    std::vecto
+00001be0: 723c 7374 643a 3a76 6563 746f 723c 7569  r<std::vector<ui
+00001bf0: 6e74 385f 743e 3e20 656c 656d 656e 7473  nt8_t>> elements
+00001c00: 287f 3631 2c31 3936 320a 2020 2020 7374  (.61,1962.    st
+00001c10: 643a 3a76 6563 746f 723c 7569 6e74 3332  d::vector<uint32
+00001c20: 5f74 3e20 726f 775f 696e 6465 7865 7328  _t> row_indexes(
+00001c30: 7f36 332c 3230 3735 0a20 2020 2076 6f69  .63,2075.    voi
+00001c40: 6420 726f 775f 6e75 6d28 7f36 352c 3231  d row_num(.65,21
+00001c50: 3738 0a20 2020 2076 6f69 6420 636f 6c5f  78.    void col_
+00001c60: 6e75 6d28 7f36 372c 3232 3734 0a20 2020  num(.67,2274.   
+00001c70: 2076 6f69 6420 656c 656d 656e 7473 287f   void elements(.
+00001c80: 3639 2c32 3337 310a 2020 2020 766f 6964  69,2371.    void
+00001c90: 2072 6f77 5f69 6e64 6578 6573 287f 3731   row_indexes(.71
+00001ca0: 2c32 3530 310a 2020 2020 766f 6964 2073  ,2501.    void s
+00001cb0: 6574 5f69 6465 6e74 6974 7928 7f38 322c  et_identity(.82,
+00001cc0: 3239 3534 0a20 2020 2076 6f69 6420 7265  2954.    void re
+00001cd0: 7665 7273 655f 656c 656d 656e 7428 7f39  verse_element(.9
+00001ce0: 362c 3333 3536 0a20 2020 2075 696e 7433  6,3356.    uint3
+00001cf0: 325f 7420 786f 725f 726f 7773 287f 3130  2_t xor_rows(.10
+00001d00: 382c 3338 3339 0a20 2020 2076 6f69 6420  8,3839.    void 
+00001d10: 7377 6170 5f72 6f77 7328 7f31 3235 2c34  swap_rows(.125,4
+00001d20: 3334 310a 2020 2020 766f 6964 2073 7761  341.    void swa
+00001d30: 705f 636f 6c73 287f 3134 302c 3437 3930  p_cols(.140,4790
+00001d40: 0a20 2020 2062 6f6f 6c20 6665 6173 6962  .    bool feasib
+00001d50: 6c65 287f 3135 332c 3531 3833 0a20 2020  le(.153,5183.   
+00001d60: 2073 7464 3a3a 7665 6374 6f72 3c7f 7374   std::vector<.st
+00001d70: 643a 3a76 6563 746f 7201 3137 342c 3537  d::vector.174,57
+00001d80: 3430 0a20 2020 2066 7269 656e 6420 7374  40.    friend st
+00001d90: 643a 3a6f 7374 7265 616d 2620 6f70 6572  d::ostream& oper
+00001da0: 6174 6f72 3c3c 287f 3137 352c 3538 3333  ator<<(.175,5833
+00001db0: 0a0c 0a75 7469 6c2e 682c 3436 0a23 6465  ...util.h,46.#de
+00001dc0: 6669 6e65 2055 5449 4c5f 487f 372c 3834  fine UTIL_H.7,84
+00001dd0: 0a6e 616d 6573 7061 6365 2053 6861 7271  .namespace Sharq
+00001de0: 6974 207f 3133 2c31 3536 0a0c 0a71 6761  it .13,156...qga
+00001df0: 7465 2e63 7070 2c36 3738 0a53 6861 7271  te.cpp,678.Sharq
+00001e00: 6974 3a3a 5147 6174 653a 3a51 4761 7465  it::QGate::QGate
+00001e10: 287f 5147 6174 6501 382c 3930 0a53 6861  (.QGate.8,90.Sha
+00001e20: 7271 6974 3a3a 5147 6174 653a 3a51 4761  rqit::QGate::QGa
+00001e30: 7465 287f 5147 6174 6501 3634 2c31 3631  te(.QGate.64,161
+00001e40: 350a 7374 643a 3a76 6563 746f 723c 7374  5.std::vector<st
+00001e50: 643a 3a76 6563 746f 723c 7374 643a 3a63  d::vector<std::c
+00001e60: 6f6d 706c 6578 3c64 6f75 626c 653e 3e3e  omplex<double>>>
+00001e70: 2053 6861 7271 6974 3a3a 5147 6174 653a   Sharqit::QGate:
+00001e80: 3a6b 696e 645f 746f 5f6f 7028 7f6b 696e  :kind_to_op(.kin
+00001e90: 645f 746f 5f6f 7001 3832 2c32 3134 350a  d_to_op.82,2145.
+00001ea0: 7374 643a 3a73 7472 696e 6720 5368 6172  std::string Shar
+00001eb0: 7169 743a 3a51 4761 7465 3a3a 6e61 6d65  qit::QGate::name
+00001ec0: 287f 6e61 6d65 0131 3638 2c34 3631 380a  (.name.168,4618.
+00001ed0: 7374 643a 3a73 7472 696e 6720 5368 6172  std::string Shar
+00001ee0: 7169 743a 3a51 4761 7465 3a3a 746f 5f73  qit::QGate::to_s
+00001ef0: 7472 696e 6728 7f74 6f5f 7374 7269 6e67  tring(.to_string
+00001f00: 0131 3737 2c34 3933 340a 7374 643a 3a74  .177,4934.std::t
+00001f10: 7570 6c65 3c53 6861 7271 6974 3a3a 5147  uple<Sharqit::QG
+00001f20: 6174 654b 696e 642c 2053 6861 7271 6974  ateKind, Sharqit
+00001f30: 3a3a 5068 6173 653e 2053 6861 7271 6974  ::Phase> Sharqit
+00001f40: 3a3a 5147 6174 653a 3a6b 696e 645f 7068  ::QGate::kind_ph
+00001f50: 6173 6528 7f6b 696e 645f 7068 6173 6501  ase(.kind_phase.
+00001f60: 3139 362c 3532 3335 0a53 6861 7271 6974  196,5235.Sharqit
+00001f70: 3a3a 5147 6174 6520 5368 6172 7169 743a  ::QGate Sharqit:
+00001f80: 3a51 4761 7465 3a3a 696e 7665 7273 6528  :QGate::inverse(
+00001f90: 7f69 6e76 6572 7365 0132 3733 2c37 3039  .inverse.273,709
+00001fa0: 390a 626f 6f6c 2053 6861 7271 6974 3a3a  9.bool Sharqit::
+00001fb0: 5147 6174 653a 3a69 735f 6964 656e 7469  QGate::is_identi
+00001fc0: 6361 6c28 7f69 735f 6964 656e 7469 6361  cal(.is_identica
+00001fd0: 6c01 3335 342c 3936 3334 0a62 6f6f 6c20  l.354,9634.bool 
+00001fe0: 5368 6172 7169 743a 3a51 4761 7465 3a3a  Sharqit::QGate::
+00001ff0: 6f76 6572 6c61 7028 7f6f 7665 726c 6170  overlap(.overlap
+00002000: 0133 3639 2c31 3031 3933 0a62 6f6f 6c20  .369,10193.bool 
+00002010: 5368 6172 7169 743a 3a51 4761 7465 3a3a  Sharqit::QGate::
+00002020: 6d65 7267 6561 626c 6528 7f6d 6572 6765  mergeable(.merge
+00002030: 6162 6c65 0133 3833 2c31 3034 3434 0a62  able.383,10444.b
+00002040: 6f6f 6c20 5368 6172 7169 743a 3a51 4761  ool Sharqit::QGa
+00002050: 7465 3a3a 636f 6d6d 7574 6162 6c65 287f  te::commutable(.
+00002060: 636f 6d6d 7574 6162 6c65 0134 3030 2c31  commutable.400,1
+00002070: 3131 3831 0a76 6f69 6420 5368 6172 7169  1181.void Sharqi
+00002080: 743a 3a51 4761 7465 3a3a 6d65 7267 6528  t::QGate::merge(
+00002090: 7f6d 6572 6765 0134 3434 2c31 3330 3836  .merge.444,13086
+000020a0: 0a0c 0a65 7874 7261 6374 5f71 6369 7263  ...extract_qcirc
+000020b0: 2e63 7070 2c34 3635 0a76 6f69 6420 5368  .cpp,465.void Sh
+000020c0: 6172 7169 743a 3a5a 5844 6961 6772 616d  arqit::ZXDiagram
+000020d0: 3a3a 7065 726d 7574 6174 696f 6e5f 6173  ::permutation_as
+000020e0: 5f73 7761 7028 7f70 6572 6d75 7461 7469  _swap(.permutati
+000020f0: 6f6e 5f61 735f 7377 6170 0138 2c31 3531  on_as_swap.8,151
+00002100: 0a73 7464 3a3a 7665 6374 6f72 3c73 7464  .std::vector<std
+00002110: 3a3a 7061 6972 3c75 696e 7433 325f 742c  ::pair<uint32_t,
+00002120: 2075 696e 7433 325f 743e 3e20 5368 6172   uint32_t>> Shar
+00002130: 7169 743a 3a5a 5844 6961 6772 616d 3a3a  qit::ZXDiagram::
+00002140: 6578 7472 6163 745f 3271 5f63 6f6e 6e65  extract_2q_conne
+00002150: 6374 7328 7f65 7874 7261 6374 5f32 715f  cts(.extract_2q_
+00002160: 636f 6e6e 6563 7473 0132 382c 3632 370a  connects.28,627.
+00002170: 626f 6f6c 2053 6861 7271 6974 3a3a 5a58  bool Sharqit::ZX
+00002180: 4469 6167 7261 6d3a 3a75 7064 6174 655f  Diagram::update_
+00002190: 6672 6f6e 7469 6572 287f 7570 6461 7465  frontier(.update
+000021a0: 5f66 726f 6e74 6965 7201 3836 2c32 3238  _frontier.86,228
+000021b0: 310a 626f 6f6c 2053 6861 7271 6974 3a3a  1.bool Sharqit::
+000021c0: 5a58 4469 6167 7261 6d3a 3a75 7064 6174  ZXDiagram::updat
+000021d0: 655f 6672 6f6e 7469 6572 5f70 6728 7f75  e_frontier_pg(.u
+000021e0: 7064 6174 655f 6672 6f6e 7469 6572 5f70  pdate_frontier_p
+000021f0: 6701 3232 352c 3634 3038 0a76 6f69 6420  g.225,6408.void 
+00002200: 5368 6172 7169 743a 3a5a 5844 6961 6772  Sharqit::ZXDiagr
+00002210: 616d 3a3a 7072 6f63 6573 735f 6672 6f6e  am::process_fron
+00002220: 7469 6572 287f 7072 6f63 6573 735f 6672  tier(.process_fr
+00002230: 6f6e 7469 6572 0133 3035 2c39 3030 380a  ontier.305,9008.
+00002240: 5368 6172 7169 743a 3a51 4369 7263 2053  Sharqit::QCirc S
+00002250: 6861 7271 6974 3a3a 5a58 4469 6167 7261  harqit::ZXDiagra
+00002260: 6d3a 3a65 7874 7261 6374 5f71 6369 7263  m::extract_qcirc
+00002270: 287f 6578 7472 6163 745f 7163 6972 6301  (.extract_qcirc.
+00002280: 3335 332c 3130 3539 350a 0c0a 6461 672e  353,10595...dag.
+00002290: 682c 3138 3933 0a23 6465 6669 6e65 2044  h,1893.#define D
+000022a0: 4147 5f48 7f37 2c31 3337 0a20 2065 6e75  AG_H.7,137.  enu
+000022b0: 6d20 4441 474e 6f64 654b 696e 6420 7f32  m DAGNodeKind .2
+000022c0: 322c 3332 390a 0909 2020 2020 4f70 4e6f  2,329...    OpNo
+000022d0: 6465 2c7f 3233 2c33 3530 0a09 0920 2020  de,.23,350...   
+000022e0: 2049 6e4e 6f64 652c 7f32 342c 3430 310a   InNode,.24,401.
+000022f0: 0909 2020 2020 4f75 744e 6f64 6520 7f32  ..    OutNode .2
+00002300: 352c 3433 310a 2020 656e 756d 2044 4147  5,431.  enum DAG
+00002310: 4564 6765 4b69 6e64 207f 3238 2c34 3933  EdgeKind .28,493
+00002320: 0a09 0920 2020 2046 6f72 7761 7264 2c7f  ...    Forward,.
+00002330: 3239 2c35 3134 0a09 0920 2020 2042 6163  29,514...    Bac
+00002340: 6b77 6172 6420 7f33 302c 3535 320a 2020  kward .30,552.  
+00002350: 636c 6173 7320 4441 474e 6f64 657f 3339  class DAGNode.39
+00002360: 2c37 3133 0a20 2020 2044 4147 4e6f 6465  ,713.    DAGNode
+00002370: 4b69 6e64 206b 696e 645f 3b7f 3432 2c37  Kind kind_;.42,7
+00002380: 3434 0a20 2020 2051 4761 7465 2071 6761  44.    QGate qga
+00002390: 7465 5f3b 7f34 332c 3738 390a 2020 2020  te_;.43,789.    
+000023a0: 4441 474e 6f64 6528 7f35 302c 3130 3031  DAGNode(.50,1001
+000023b0: 0a20 2020 2044 4147 4e6f 6465 287f 3536  .    DAGNode(.56
+000023c0: 2c31 3232 360a 2020 2020 4441 474e 6f64  ,1226.    DAGNod
+000023d0: 654b 696e 6420 6b69 6e64 287f 3538 2c31  eKind kind(.58,1
+000023e0: 3333 310a 2020 2020 5147 6174 6520 7167  331.    QGate qg
+000023f0: 6174 6528 7f36 302c 3134 3037 0a20 2020  ate(.60,1407.   
+00002400: 2076 6f69 6420 6b69 6e64 287f 3632 2c31   void kind(.62,1
+00002410: 3437 380a 2020 2020 766f 6964 2071 6761  478.    void qga
+00002420: 7465 287f 3634 2c31 3536 330a 2020 2020  te(.64,1563.    
+00002430: 7569 6e74 3332 5f74 2071 7562 6974 5f6e  uint32_t qubit_n
+00002440: 756d 287f 3734 2c31 3839 340a 2020 2020  um(.74,1894.    
+00002450: 7374 643a 3a76 6563 746f 723c 7569 6e74  std::vector<uint
+00002460: 3332 5f74 3e20 7169 6428 7f37 392c 3231  32_t> qid(.79,21
+00002470: 3038 0a20 2020 2062 6f6f 6c20 6973 5f69  08.    bool is_i
+00002480: 6e6e 6f64 6528 7f38 342c 3233 3032 0a20  nnode(.84,2302. 
+00002490: 2020 2062 6f6f 6c20 6973 5f6f 7574 6e6f     bool is_outno
+000024a0: 6465 287f 3839 2c32 3531 380a 2020 2020  de(.89,2518.    
+000024b0: 626f 6f6c 2069 735f 6f70 6e6f 6465 287f  bool is_opnode(.
+000024c0: 3934 2c32 3737 320a 2020 2020 626f 6f6c  94,2772.    bool
+000024d0: 2069 735f 6964 656e 7469 7479 287f 3939   is_identity(.99
+000024e0: 2c33 3030 380a 2020 2020 626f 6f6c 2069  ,3008.    bool i
+000024f0: 735f 6861 6461 6d61 7264 287f 3130 352c  s_hadamard(.105,
+00002500: 3332 3832 0a20 2020 2062 6f6f 6c20 6973  3282.    bool is
+00002510: 5f72 6f74 6174 696f 6e28 7f31 3130 2c33  _rotation(.110,3
+00002520: 3438 330a 2020 2020 626f 6f6c 2069 735f  483.    bool is_
+00002530: 636e 6f74 287f 3131 352c 3336 3737 0a20  cnot(.115,3677. 
+00002540: 2020 2062 6f6f 6c20 6973 5f69 6e63 6c75     bool is_inclu
+00002550: 6465 6428 7f31 3231 2c33 3935 320a 2020  ded(.121,3952.  
+00002560: 2020 626f 6f6c 206d 6572 6765 6162 6c65    bool mergeable
+00002570: 287f 3133 312c 3432 3938 0a20 2020 2062  (.131,4298.    b
+00002580: 6f6f 6c20 636f 6d6d 7574 6162 6c65 287f  ool commutable(.
+00002590: 3133 372c 3436 3036 0a20 2020 2076 6f69  137,4606.    voi
+000025a0: 6420 6d65 7267 6528 7f31 3432 2c34 3832  d merge(.142,482
+000025b0: 340a 2020 636c 6173 7320 4441 4745 6467  4.  class DAGEdg
+000025c0: 657f 3135 302c 3439 3938 0a20 2020 2044  e.150,4998.    D
+000025d0: 4147 4564 6765 4b69 6e64 206b 696e 645f  AGEdgeKind kind_
+000025e0: 3b7f 3135 332c 3530 3239 0a20 2020 2075  ;.153,5029.    u
+000025f0: 696e 7433 325f 7420 715f 3b7f 3135 342c  int32_t q_;.154,
+00002600: 3531 3032 0a20 2020 2075 696e 7433 325f  5102.    uint32_
+00002610: 7420 746f 5f3b 7f31 3535 2c35 3135 330a  t to_;.155,5153.
+00002620: 2020 2020 4441 4745 6467 6528 7f31 3633      DAGEdge(.163
+00002630: 2c35 3431 340a 2020 2020 4441 4745 6467  ,5414.    DAGEdg
+00002640: 6528 7f31 3639 2c35 3636 360a 2020 2020  e(.169,5666.    
+00002650: 4441 4745 6467 654b 696e 6420 6b69 6e64  DAGEdgeKind kind
+00002660: 287f 3137 312c 3537 3738 0a20 2020 2075  (.171,5778.    u
+00002670: 696e 7433 325f 7420 7128 7f31 3733 2c35  int32_t q(.173,5
+00002680: 3835 300a 2020 2020 7569 6e74 3332 5f74  850.    uint32_t
+00002690: 2074 6f28 7f31 3735 2c35 3931 340a 2020   to(.175,5914.  
+000026a0: 2020 766f 6964 206b 696e 6428 7f31 3737    void kind(.177
+000026b0: 2c35 3938 320a 2020 2020 766f 6964 2071  ,5982.    void q
+000026c0: 287f 3137 392c 3630 3537 0a20 2020 2076  (.179,6057.    v
+000026d0: 6f69 6420 746f 287f 3138 312c 3631 3138  oid to(.181,6118
+000026e0: 0a20 2020 2062 6f6f 6c20 6973 5f66 6f72  .    bool is_for
+000026f0: 7761 7264 287f 3139 312c 3634 3039 0a20  ward(.191,6409. 
+00002700: 2020 2062 6f6f 6c20 6973 5f62 6163 6b77     bool is_backw
+00002710: 6172 6428 7f31 3936 2c36 3632 370a 2020  ard(.196,6627.  
+00002720: 636c 6173 7320 4441 4743 6972 637f 3230  class DAGCirc.20
+00002730: 352c 3638 3434 0a20 2020 2075 696e 7433  5,6844.    uint3
+00002740: 325f 7420 7175 6269 745f 6e75 6d5f 3b7f  2_t qubit_num_;.
+00002750: 3230 382c 3638 3735 0a20 2020 2073 7464  208,6875.    std
+00002760: 3a3a 7665 6374 6f72 3c44 4147 4e6f 6465  ::vector<DAGNode
+00002770: 3e20 6e6f 6465 735f 3b7f 3230 392c 3639  > nodes_;.209,69
+00002780: 3232 0a20 2020 2073 7464 3a3a 7665 6374  22.    std::vect
+00002790: 6f72 3c75 696e 7433 325f 743e 2069 6e70  or<uint32_t> inp
+000027a0: 7574 735f 3b7f 3231 302c 3639 3930 0a20  uts_;.210,6990. 
+000027b0: 2020 2073 7464 3a3a 7665 6374 6f72 3c75     std::vector<u
+000027c0: 696e 7433 325f 743e 206f 7574 7075 7473  int32_t> outputs
+000027d0: 5f3b 7f32 3131 2c37 3036 330a 2020 2020  _;.211,7063.    
+000027e0: 7374 643a 3a76 6563 746f 723c 7374 643a  std::vector<std:
+000027f0: 3a76 6563 746f 723c 4441 4745 6467 653e  :vector<DAGEdge>
+00002800: 3e20 6164 6a5f 6d61 745f 3b7f 3231 322c  > adj_mat_;.212,
+00002810: 3731 3338 0a20 2020 2044 4147 4369 7263  7138.    DAGCirc
+00002820: 287f 3236 362c 3935 3435 0a20 2020 2075  (.266,9545.    u
+00002830: 696e 7433 325f 7420 7175 6269 745f 6e75  int32_t qubit_nu
+00002840: 6d28 7f32 3730 2c39 3733 370a 2020 2020  m(.270,9737.    
+00002850: 7374 643a 3a76 6563 746f 723c 4441 474e  std::vector<DAGN
+00002860: 6f64 653e 206e 6f64 6573 287f 3237 322c  ode> nodes(.272,
+00002870: 3938 3230 0a20 2020 2073 7464 3a3a 7665  9820.    std::ve
+00002880: 6374 6f72 3c75 696e 7433 325f 743e 2069  ctor<uint32_t> i
+00002890: 6e70 7574 7328 7f32 3734 2c39 3930 380a  nputs(.274,9908.
+000028a0: 2020 2020 7374 643a 3a76 6563 746f 723c      std::vector<
+000028b0: 7569 6e74 3332 5f74 3e20 6f75 7470 7574  uint32_t> output
+000028c0: 7328 7f32 3736 2c31 3030 3030 0a20 2020  s(.276,10000.   
+000028d0: 2073 7464 3a3a 7665 6374 6f72 3c73 7464   std::vector<std
+000028e0: 3a3a 7665 6374 6f72 3c44 4147 4564 6765  ::vector<DAGEdge
+000028f0: 3e3e 2061 646a 5f6d 6174 287f 3237 382c  >> adj_mat(.278,
+00002900: 3130 3039 340a 2020 2020 766f 6964 2071  10094.    void q
+00002910: 7562 6974 5f6e 756d 287f 3238 302c 3130  ubit_num(.280,10
+00002920: 3230 320a 2020 2020 766f 6964 206e 6f64  202.    void nod
+00002930: 6573 287f 3238 322c 3130 3330 340a 2020  es(.282,10304.  
+00002940: 2020 766f 6964 2069 6e70 7574 7328 7f32    void inputs(.2
+00002950: 3834 2c31 3034 3034 0a20 2020 2076 6f69  84,10404.    voi
+00002960: 6420 6f75 7470 7574 7328 7f32 3836 2c31  d outputs(.286,1
+00002970: 3035 3130 0a20 2020 2076 6f69 6420 6164  0510.    void ad
+00002980: 6a5f 6d61 7428 7f32 3838 2c31 3036 3230  j_mat(.288,10620
+00002990: 0a20 2020 2076 6f69 6420 7368 6f77 287f  .    void show(.
+000029a0: 3239 372c 3130 3931 390a 2020 2020 7569  297,10919.    ui
+000029b0: 6e74 3332 5f74 2067 6174 655f 636f 756e  nt32_t gate_coun
+000029c0: 7428 7f33 3031 2c31 3130 3138 0a20 2020  t(.301,11018.   
+000029d0: 2066 7269 656e 6420 7374 643a 3a6f 7374   friend std::ost
+000029e0: 7265 616d 2620 6f70 6572 6174 6f72 3c3c  ream& operator<<
+000029f0: 287f 3339 332c 3134 3830 320a 0c0a 7163  (.393,14802...qc
+00002a00: 6972 632e 682c 3138 3033 0a23 6465 6669  irc.h,1803.#defi
+00002a10: 6e65 2051 4349 5243 5f48 7f37 2c38 300a  ne QCIRC_H.7,80.
+00002a20: 2020 636c 6173 7320 5143 6972 637f 3334    class QCirc.34
+00002a30: 2c34 3932 0a20 2020 2075 696e 7433 325f  ,492.    uint32_
+00002a40: 7420 7175 6269 745f 6e75 6d5f 3b7f 3337  t qubit_num_;.37
+00002a50: 2c35 3231 0a20 2020 2073 7464 3a3a 7665  ,521.    std::ve
+00002a60: 6374 6f72 3c51 4761 7465 3e20 7167 6174  ctor<QGate> qgat
+00002a70: 6573 5f3b 7f33 382c 3536 380a 2020 2020  es_;.38,568.    
+00002a80: 5143 6972 6328 7f35 392c 3135 3530 0a20  QCirc(.59,1550. 
+00002a90: 2020 2051 4369 7263 287f 3634 2c31 3731     QCirc(.64,171
+00002aa0: 390a 2020 2020 5143 6972 6328 7f36 392c  9.    QCirc(.69,
+00002ab0: 3139 3037 0a20 2020 2075 696e 7433 325f  1907.    uint32_
+00002ac0: 7420 7175 6269 745f 6e75 6d28 7f37 312c  t qubit_num(.71,
+00002ad0: 3230 3331 0a20 2020 2075 696e 7433 325f  2031.    uint32_
+00002ae0: 7420 6765 745f 7175 6269 745f 6e75 6d28  t get_qubit_num(
+00002af0: 7f37 332c 3231 3138 0a20 2020 2073 7464  .73,2118.    std
+00002b00: 3a3a 7665 6374 6f72 3c51 4761 7465 3e20  ::vector<QGate> 
+00002b10: 7167 6174 6573 287f 3735 2c32 3230 360a  qgates(.75,2206.
+00002b20: 2020 2020 766f 6964 2071 7562 6974 5f6e      void qubit_n
+00002b30: 756d 287f 3737 2c32 3239 370a 2020 2020  um(.77,2297.    
+00002b40: 766f 6964 2071 6761 7465 7328 7f37 392c  void qgates(.79,
+00002b50: 3234 3030 0a20 2020 2075 696e 7433 325f  2400.    uint32_
+00002b60: 7420 7167 6174 655f 6e75 6d28 7f38 342c  t qgate_num(.84,
+00002b70: 3235 3735 0a20 2020 2076 6f69 6420 636c  2575.    void cl
+00002b80: 6561 7228 7f39 382c 3330 3238 0a20 2020  ear(.98,3028.   
+00002b90: 2073 7464 3a3a 6d61 703c 7f73 7464 3a3a   std::map<.std::
+00002ba0: 6d61 7001 3130 332c 3331 3930 0a20 2020  map.103,3190.   
+00002bb0: 2075 696e 7433 325f 7420 6761 7465 5f63   uint32_t gate_c
+00002bc0: 6f75 6e74 287f 3130 382c 3333 3934 0a20  ount(.108,3394. 
+00002bd0: 2020 2075 696e 7433 325f 7420 7477 6f71     uint32_t twoq
+00002be0: 5f63 6f75 6e74 287f 3135 382c 3439 3636  _count(.158,4966
+00002bf0: 0a20 2020 2076 6f69 6420 7368 6f77 287f  .    void show(.
+00002c00: 3137 332c 3535 3031 0a20 2020 2076 6f69  173,5501.    voi
+00002c10: 6420 7072 696e 745f 7163 6972 6328 7f31  d print_qcirc(.1
+00002c20: 3737 2c35 3635 370a 2020 2020 5143 6972  77,5657.    QCir
+00002c30: 6326 2061 6464 5f71 6761 7465 287f 3230  c& add_qgate(.20
+00002c40: 312c 3637 3633 0a20 2020 2053 6861 7271  1,6763.    Sharq
+00002c50: 6974 3a3a 5147 6174 6520 6765 745f 7167  it::QGate get_qg
+00002c60: 6174 6528 7f32 3333 2c38 3533 310a 2020  ate(.233,8531.  
+00002c70: 2020 7374 643a 3a76 6563 746f 723c 5368    std::vector<Sh
+00002c80: 6172 7169 743a 3a51 4761 7465 3e20 6765  arqit::QGate> ge
+00002c90: 745f 7167 6174 6573 287f 3233 382c 3837  t_qgates(.238,87
+00002ca0: 3038 0a20 2020 2051 4369 7263 2620 6964  08.    QCirc& id
+00002cb0: 287f 3333 302c 3131 3938 300a 2020 2020  (.330,11980.    
+00002cc0: 5143 6972 6326 2078 287f 3333 362c 3132  QCirc& x(.336,12
+00002cd0: 3233 380a 2020 2020 5143 6972 6326 207a  238.    QCirc& z
+00002ce0: 287f 3334 322c 3132 3439 340a 2020 2020  (.342,12494.    
+00002cf0: 5143 6972 6326 2073 287f 3334 382c 3132  QCirc& s(.348,12
+00002d00: 3734 340a 2020 2020 5143 6972 6326 2073  744.    QCirc& s
+00002d10: 6467 287f 3335 342c 3133 3032 320a 2020  dg(.354,13022.  
+00002d20: 2020 5143 6972 6326 2074 287f 3336 302c    QCirc& t(.360,
+00002d30: 3133 3237 360a 2020 2020 5143 6972 6326  13276.    QCirc&
+00002d40: 2074 6467 287f 3336 362c 3133 3535 340a   tdg(.366,13554.
+00002d50: 2020 2020 5143 6972 6326 2068 287f 3337      QCirc& h(.37
+00002d60: 322c 3133 3832 300a 2020 2020 5143 6972  2,13820.    QCir
+00002d70: 6326 2072 7a28 7f33 3739 2c31 3431 3138  c& rz(.379,14118
+00002d80: 0a20 2020 2051 4369 7263 2620 6964 3228  .    QCirc& id2(
+00002d90: 7f33 3836 2c31 3434 3737 0a20 2020 2051  .386,14477.    Q
+00002da0: 4369 7263 2620 6378 287f 3339 332c 3134  Circ& cx(.393,14
+00002db0: 3832 330a 2020 2020 5143 6972 6326 2063  823.    QCirc& c
+00002dc0: 7a28 7f34 3030 2c31 3531 3630 0a20 2020  z(.400,15160.   
+00002dd0: 2051 4369 7263 2620 7278 287f 3430 372c   QCirc& rx(.407,
+00002de0: 3135 3438 310a 2020 2020 5143 6972 6326  15481.    QCirc&
+00002df0: 2063 6378 287f 3431 352c 3135 3837 370a   ccx(.415,15877.
+00002e00: 2020 2020 5143 6972 6326 2063 637a 287f      QCirc& ccz(.
+00002e10: 3432 332c 3136 3330 340a 2020 2020 5143  423,16304.    QC
+00002e20: 6972 6326 2079 287f 3432 392c 3136 3631  irc& y(.429,1661
+00002e30: 340a 2020 2020 5143 6972 6326 2073 7828  4.    QCirc& sx(
+00002e40: 7f34 3335 2c31 3638 3832 0a20 2020 2051  .435,16882.    Q
+00002e50: 4369 7263 2620 7378 6467 287f 3434 312c  Circ& sxdg(.441,
+00002e60: 3137 3138 340a 2020 2020 5143 6972 6326  17184.    QCirc&
+00002e70: 2072 7928 7f34 3438 2c31 3734 3739 0a20   ry(.448,17479. 
+00002e80: 2020 2051 4369 7263 2620 7028 7f34 3536     QCirc& p(.456
+00002e90: 2c31 3738 3435 0a20 2020 2051 4369 7263  ,17845.    QCirc
+00002ea0: 2620 6379 287f 3436 332c 3138 3138 380a  & cy(.463,18188.
+00002eb0: 2020 2020 5143 6972 6326 2063 7378 287f      QCirc& csx(.
+00002ec0: 3437 302c 3138 3535 350a 2020 2020 5143  470,18555.    QC
+00002ed0: 6972 6326 2063 7378 6467 287f 3437 372c  irc& csxdg(.477,
+00002ee0: 3138 3934 350a 2020 2020 5143 6972 6326  18945.    QCirc&
+00002ef0: 2063 6828 7f34 3834 2c31 3933 3234 0a20   ch(.484,19324. 
+00002f00: 2020 2051 4369 7263 2620 6373 287f 3439     QCirc& cs(.49
+00002f10: 322c 3139 3734 340a 2020 2020 5143 6972  2,19744.    QCir
+00002f20: 6326 2063 7364 6728 7f35 3030 2c32 3031  c& csdg(.500,201
+00002f30: 3338 0a20 2020 2051 4369 7263 2620 6374  38.    QCirc& ct
+00002f40: 287f 3530 382c 3230 3531 330a 2020 2020  (.508,20513.    
+00002f50: 5143 6972 6326 2063 7464 6728 7f35 3136  QCirc& ctdg(.516
+00002f60: 2c32 3039 3139 0a20 2020 2051 4369 7263  ,20919.    QCirc
+00002f70: 2620 6372 7828 7f35 3235 2c32 3133 3438  & crx(.525,21348
+00002f80: 0a20 2020 2051 4369 7263 2620 6372 7928  .    QCirc& cry(
+00002f90: 7f35 3334 2c32 3137 3835 0a20 2020 2051  .534,21785.    Q
+00002fa0: 4369 7263 2620 6372 7a28 7f35 3433 2c32  Circ& crz(.543,2
+00002fb0: 3232 3437 0a20 2020 2051 4369 7263 2620  2247.    QCirc& 
+00002fc0: 6370 287f 3535 322c 3232 3730 380a 2020  cp(.552,22708.  
+00002fd0: 2020 5143 6972 6326 2072 7878 287f 3536    QCirc& rxx(.56
+00002fe0: 312c 3233 3134 320a 2020 2020 5143 6972  1,23142.    QCir
+00002ff0: 6326 2072 7979 287f 3537 352c 3233 3633  c& ryy(.575,2363
+00003000: 300a 2020 2020 5143 6972 6326 2072 7a7a  0.    QCirc& rzz
+00003010: 287f 3538 392c 3234 3136 380a 2020 2020  (.589,24168.    
+00003020: 5143 6972 6326 2073 7728 7f35 3937 2c32  QCirc& sw(.597,2
+00003030: 3435 3236 0a20 2020 2051 4369 7263 2620  4526.    QCirc& 
+00003040: 6373 7728 7f36 3036 2c32 3439 3337 0a20  csw(.606,24937. 
+00003050: 2020 2051 4369 7263 2620 6363 785f 6465     QCirc& ccx_de
+00003060: 636f 6d70 5f41 287f 3631 352c 3235 3430  comp_A(.615,2540
+00003070: 300a 2020 2020 5143 6972 6326 2063 637a  0.    QCirc& ccz
+00003080: 5f64 6563 6f6d 705f 4128 7f36 3237 2c32  _decomp_A(.627,2
+00003090: 3539 3637 0a20 2020 2051 4369 7263 2620  5967.    QCirc& 
+000030a0: 6f70 6572 6174 6f72 2b3d 287f 6f70 6572  operator+=(.oper
+000030b0: 6174 6f72 2b3d 0136 3332 2c32 3632 3136  ator+=.632,26216
+000030c0: 0a20 2020 2066 7269 656e 6420 5143 6972  .    friend QCir
+000030d0: 6320 6f70 6572 6174 6f72 2b28 7f36 3333  c operator+(.633
+000030e0: 2c32 3632 3833 0a20 2020 2066 7269 656e  ,26283.    frien
+000030f0: 6420 7374 643a 3a6f 7374 7265 616d 2620  d std::ostream& 
+00003100: 6f70 6572 6174 6f72 3c3c 287f 3633 342c  operator<<(.634,
+00003110: 3236 3339 320a 0c0a 6461 6763 6972 632e  26392...dagcirc.
+00003120: 6370 702c 3136 3235 0a53 6861 7271 6974  cpp,1625.Sharqit
+00003130: 3a3a 4441 4743 6972 633a 3a44 4147 4369  ::DAGCirc::DAGCi
+00003140: 7263 287f 4441 4743 6972 6301 382c 3932  rc(.DAGCirc.8,92
+00003150: 0a53 6861 7271 6974 3a3a 4441 4743 6972  .Sharqit::DAGCir
+00003160: 633a 3a44 4147 4369 7263 287f 4441 4743  c::DAGCirc(.DAGC
+00003170: 6972 6301 3239 2c36 3939 0a73 7464 3a3a  irc.29,699.std::
+00003180: 7374 7269 6e67 2053 6861 7271 6974 3a3a  string Sharqit::
+00003190: 4441 4743 6972 633a 3a74 6f5f 7374 7269  DAGCirc::to_stri
+000031a0: 6e67 287f 746f 5f73 7472 696e 6701 3533  ng(.to_string.53
+000031b0: 2c31 3339 330a 7569 6e74 3332 5f74 2053  ,1393.uint32_t S
+000031c0: 6861 7271 6974 3a3a 4441 4743 6972 633a  harqit::DAGCirc:
+000031d0: 3a61 7070 656e 645f 6e6f 6465 287f 6170  :append_node(.ap
+000031e0: 7065 6e64 5f6e 6f64 6501 3732 2c31 3836  pend_node.72,186
+000031f0: 320a 7569 6e74 3332 5f74 2053 6861 7271  2.uint32_t Sharq
+00003200: 6974 3a3a 4441 4743 6972 633a 3a70 7265  it::DAGCirc::pre
+00003210: 765f 6e6f 6465 287f 7072 6576 5f6e 6f64  v_node(.prev_nod
+00003220: 6501 3830 2c32 3035 350a 7569 6e74 3332  e.80,2055.uint32
+00003230: 5f74 2053 6861 7271 6974 3a3a 4441 4743  _t Sharqit::DAGC
+00003240: 6972 633a 3a6e 6578 745f 6e6f 6465 287f  irc::next_node(.
+00003250: 6e65 7874 5f6e 6f64 6501 3939 2c32 3532  next_node.99,252
+00003260: 330a 766f 6964 2053 6861 7271 6974 3a3a  3.void Sharqit::
+00003270: 4441 4743 6972 633a 3a63 6f6e 6e65 6374  DAGCirc::connect
+00003280: 5f6e 6f64 6573 287f 636f 6e6e 6563 745f  _nodes(.connect_
+00003290: 6e6f 6465 7301 3131 382c 3239 3838 0a76  nodes.118,2988.v
+000032a0: 6f69 6420 5368 6172 7169 743a 3a44 4147  oid Sharqit::DAG
+000032b0: 4369 7263 3a3a 7265 6d6f 7665 5f6e 6f64  Circ::remove_nod
+000032c0: 6528 7f72 656d 6f76 655f 6e6f 6465 0131  e(.remove_node.1
+000032d0: 3239 2c33 3437 330a 766f 6964 2053 6861  29,3473.void Sha
+000032e0: 7271 6974 3a3a 4441 4743 6972 633a 3a72  rqit::DAGCirc::r
+000032f0: 656d 6f76 655f 6564 6765 287f 7265 6d6f  emove_edge(.remo
+00003300: 7665 5f65 6467 6501 3136 312c 3431 3233  ve_edge.161,4123
+00003310: 0a76 6f69 6420 5368 6172 7169 743a 3a44  .void Sharqit::D
+00003320: 4147 4369 7263 3a3a 7265 6d6f 7665 5f65  AGCirc::remove_e
+00003330: 6467 6528 7f72 656d 6f76 655f 6564 6765  dge(.remove_edge
+00003340: 0131 3739 2c34 3532 380a 766f 6964 2053  .179,4528.void S
+00003350: 6861 7271 6974 3a3a 4441 4743 6972 633a  harqit::DAGCirc:
+00003360: 3a72 656d 6f76 655f 6564 6765 735f 6f66  :remove_edges_of
+00003370: 5f6e 6f64 6528 7f72 656d 6f76 655f 6564  _node(.remove_ed
+00003380: 6765 735f 6f66 5f6e 6f64 6501 3139 372c  ges_of_node.197,
+00003390: 3439 3833 0a76 6f69 6420 5368 6172 7169  4983.void Sharqi
+000033a0: 743a 3a44 4147 4369 7263 3a3a 7265 6d6f  t::DAGCirc::remo
+000033b0: 7665 5f69 736f 6c61 7465 645f 6e6f 6465  ve_isolated_node
+000033c0: 7328 7f72 656d 6f76 655f 6973 6f6c 6174  s(.remove_isolat
+000033d0: 6564 5f6e 6f64 6573 0132 3131 2c35 3331  ed_nodes.211,531
+000033e0: 320a 5368 6172 7169 743a 3a44 4147 4369  2.Sharqit::DAGCi
+000033f0: 7263 2620 5368 6172 7169 743a 3a44 4147  rc& Sharqit::DAG
+00003400: 4369 7263 3a3a 6164 645f 7167 6174 6528  Circ::add_qgate(
+00003410: 7f61 6464 5f71 6761 7465 0132 3237 2c35  .add_qgate.227,5
+00003420: 3633 310a 5368 6172 7169 743a 3a51 4369  631.Sharqit::QCi
+00003430: 7263 2053 6861 7271 6974 3a3a 4441 4743  rc Sharqit::DAGC
+00003440: 6972 633a 3a74 6f5f 7163 6972 6328 7f74  irc::to_qcirc(.t
+00003450: 6f5f 7163 6972 6301 3236 342c 3637 3137  o_qcirc.264,6717
+00003460: 0a76 6f69 6420 5368 6172 7169 743a 3a44  .void Sharqit::D
+00003470: 4147 4369 7263 3a3a 6964 5f72 656d 6f76  AGCirc::id_remov
+00003480: 616c 287f 6964 5f72 656d 6f76 616c 0133  al(.id_removal.3
+00003490: 3036 2c37 3736 390a 766f 6964 2053 6861  06,7769.void Sha
+000034a0: 7271 6974 3a3a 4441 4743 6972 633a 3a63  rqit::DAGCirc::c
+000034b0: 785f 746f 5f63 7a5f 6761 7465 287f 6378  x_to_cz_gate(.cx
+000034c0: 5f74 6f5f 637a 5f67 6174 6501 3332 392c  _to_cz_gate.329,
+000034d0: 3834 3834 0a76 6f69 6420 5368 6172 7169  8484.void Sharqi
+000034e0: 743a 3a44 4147 4369 7263 3a3a 637a 5f74  t::DAGCirc::cz_t
+000034f0: 6f5f 6378 5f67 6174 6528 7f63 7a5f 746f  o_cx_gate(.cz_to
+00003500: 5f63 785f 6761 7465 0133 3539 2c39 3330  _cx_gate.359,930
+00003510: 370a 766f 6964 2053 6861 7271 6974 3a3a  7.void Sharqit::
+00003520: 4441 4743 6972 633a 3a68 6164 616d 6172  DAGCirc::hadamar
+00003530: 645f 6761 7465 5f72 6564 7563 7469 6f6e  d_gate_reduction
+00003540: 5f31 287f 6861 6461 6d61 7264 5f67 6174  _1(.hadamard_gat
+00003550: 655f 7265 6475 6374 696f 6e5f 3101 3339  e_reduction_1.39
+00003560: 342c 3130 3534 360a 766f 6964 2053 6861  4,10546.void Sha
+00003570: 7271 6974 3a3a 4441 4743 6972 633a 3a68  rqit::DAGCirc::h
+00003580: 6164 616d 6172 645f 6761 7465 5f72 6564  adamard_gate_red
+00003590: 7563 7469 6f6e 5f32 287f 6861 6461 6d61  uction_2(.hadama
+000035a0: 7264 5f67 6174 655f 7265 6475 6374 696f  rd_gate_reductio
+000035b0: 6e5f 3201 3433 342c 3131 3830 360a 766f  n_2.434,11806.vo
+000035c0: 6964 2053 6861 7271 6974 3a3a 4441 4743  id Sharqit::DAGC
+000035d0: 6972 633a 3a68 6164 616d 6172 645f 6761  irc::hadamard_ga
+000035e0: 7465 5f72 6564 7563 7469 6f6e 5f33 287f  te_reduction_3(.
+000035f0: 6861 6461 6d61 7264 5f67 6174 655f 7265  hadamard_gate_re
+00003600: 6475 6374 696f 6e5f 3301 3437 352c 3133  duction_3.475,13
+00003610: 3038 370a 7569 6e74 3332 5f74 2053 6861  087.uint32_t Sha
+00003620: 7271 6974 3a3a 4441 4743 6972 633a 3a68  rqit::DAGCirc::h
+00003630: 6164 616d 6172 645f 6761 7465 5f72 6564  adamard_gate_red
+00003640: 7563 7469 6f6e 287f 6861 6461 6d61 7264  uction(.hadamard
+00003650: 5f67 6174 655f 7265 6475 6374 696f 6e01  _gate_reduction.
+00003660: 3533 332c 3135 3036 320a 7569 6e74 3332  533,15062.uint32
+00003670: 5f74 2053 6861 7271 6974 3a3a 4441 4743  _t Sharqit::DAGC
+00003680: 6972 633a 3a73 696e 676c 655f 7175 6269  irc::single_qubi
+00003690: 745f 6761 7465 5f63 616e 6365 6c6c 6174  t_gate_cancellat
+000036a0: 696f 6e28 7f73 696e 676c 655f 7175 6269  ion(.single_qubi
+000036b0: 745f 6761 7465 5f63 616e 6365 6c6c 6174  t_gate_cancellat
+000036c0: 696f 6e01 3534 342c 3135 3237 350a 7569  ion.544,15275.ui
+000036d0: 6e74 3332 5f74 2053 6861 7271 6974 3a3a  nt32_t Sharqit::
+000036e0: 4441 4743 6972 633a 3a74 776f 5f71 7562  DAGCirc::two_qub
+000036f0: 6974 5f67 6174 655f 6361 6e63 656c 6c61  it_gate_cancella
+00003700: 7469 6f6e 287f 7477 6f5f 7175 6269 745f  tion(.two_qubit_
+00003710: 6761 7465 5f63 616e 6365 6c6c 6174 696f  gate_cancellatio
+00003720: 6e01 3634 322c 3137 3939 340a 766f 6964  n.642,17994.void
+00003730: 2053 6861 7271 6974 3a3a 4441 4743 6972   Sharqit::DAGCir
+00003740: 633a 3a72 756c 655f 6261 7365 645f 6761  c::rule_based_ga
+00003750: 7465 5f72 6564 7563 7469 6f6e 287f 7275  te_reduction(.ru
+00003760: 6c65 5f62 6173 6564 5f67 6174 655f 7265  le_based_gate_re
+00003770: 6475 6374 696f 6e01 3733 322c 3230 3732  duction.732,2072
+00003780: 350a 0c0a 6c69 6e65 6172 5f6d 6170 2e63  5...linear_map.c
+00003790: 7070 2c34 3431 0a62 6f6f 6c20 5368 6172  pp,441.bool Shar
+000037a0: 7169 743a 3a4c 696e 6561 724d 6170 3a3a  qit::LinearMap::
+000037b0: 6973 5f7a 6572 6f28 7f69 735f 7a65 726f  is_zero(.is_zero
+000037c0: 0138 2c31 3034 0a62 6f6f 6c20 5368 6172  .8,104.bool Shar
+000037d0: 7169 743a 3a4c 696e 6561 724d 6170 3a3a  qit::LinearMap::
+000037e0: 6973 5f69 6465 6e74 6974 7928 7f69 735f  is_identity(.is_
+000037f0: 6964 656e 7469 7479 0132 312c 3434 340a  identity.21,444.
+00003800: 626f 6f6c 2053 6861 7271 6974 3a3a 4c69  bool Sharqit::Li
+00003810: 6e65 6172 4d61 703a 3a69 735f 6469 6167  nearMap::is_diag
+00003820: 6f6e 616c 287f 6973 5f64 6961 676f 6e61  onal(.is_diagona
+00003830: 6c01 3333 2c37 3432 0a62 6f6f 6c20 5368  l.33,742.bool Sh
+00003840: 6172 7169 743a 3a4c 696e 6561 724d 6170  arqit::LinearMap
+00003850: 3a3a 6973 5f69 6465 6e74 6974 795f 6d75  ::is_identity_mu
+00003860: 6c74 6970 6c65 5f63 6f6e 7374 616e 7428  ltiple_constant(
+00003870: 7f69 735f 6964 656e 7469 7479 5f6d 756c  .is_identity_mul
+00003880: 7469 706c 655f 636f 6e73 7461 6e74 0134  tiple_constant.4
+00003890: 352c 3130 3336 0a62 6f6f 6c20 5368 6172  5,1036.bool Shar
+000038a0: 7169 743a 3a4c 696e 6561 724d 6170 3a3a  qit::LinearMap::
+000038b0: 6973 5f75 6e69 7461 7279 287f 6973 5f75  is_unitary(.is_u
+000038c0: 6e69 7461 7279 0135 392c 3134 3239 0a62  nitary.59,1429.b
+000038d0: 6f6f 6c20 5368 6172 7169 743a 3a4c 696e  ool Sharqit::Lin
+000038e0: 6561 724d 6170 3a3a 6973 5f65 7175 616c  earMap::is_equal
+000038f0: 287f 6973 5f65 7175 616c 0137 302c 3136  (.is_equal.70,16
+00003900: 3930 0a53 6861 7271 6974 3a3a 4c69 6e65  90.Sharqit::Line
+00003910: 6172 4d61 7026 2053 6861 7271 6974 3a3a  arMap& Sharqit::
+00003920: 4c69 6e65 6172 4d61 703a 3a6f 7065 7261  LinearMap::opera
+00003930: 7465 5f71 6761 7465 287f 6f70 6572 6174  te_qgate(.operat
+00003940: 655f 7167 6174 6501 3831 2c31 3934 330a  e_qgate.81,1943.
+00003950: 0c0a 7368 6172 7169 742e 682c 3439 0a23  ..sharqit.h,49.#
+00003960: 6465 6669 6e65 2053 4841 5251 4954 5f48  define SHARQIT_H
+00003970: 7f37 2c38 380a 6e61 6d65 7370 6163 6520  .7,88.namespace 
+00003980: 5368 6172 7169 7420 7f31 392c 3239 340a  Sharqit .19,294.
+00003990: 0c0a 7368 6172 7169 742e 6370 702c 3137  ..sharqit.cpp,17
+000039a0: 360a 766f 6964 2070 7269 6e74 5f68 656c  6.void print_hel
+000039b0: 7028 7f31 312c 3133 300a 766f 6964 206f  p(.11,130.void o
+000039c0: 7074 696d 697a 6528 7f35 372c 3236 3332  ptimize(.57,2632
+000039d0: 0a76 6f69 6420 7665 7269 6679 5f65 7175  .void verify_equ
+000039e0: 616c 6974 7928 7f37 372c 3331 3439 0a76  ality(.77,3149.v
+000039f0: 6f69 6420 7261 6e64 6f6d 5f71 6369 7263  oid random_qcirc
+00003a00: 287f 3938 2c33 3731 340a 766f 6964 2070  (.98,3714.void p
+00003a10: 7269 6e74 5f73 7461 7473 287f 3132 362c  rint_stats(.126,
+00003a20: 3435 3031 0a76 6f69 6420 7368 6f77 5f71  4501.void show_q
+00003a30: 6369 7263 287f 3134 322c 3438 3230 0a69  circ(.142,4820.i
+00003a40: 6e74 206d 6169 6e28 7f31 3539 2c35 3135  nt main(.159,515
+00003a50: 370a 0c0a 7369 6d70 6c69 6679 2e63 7070  7...simplify.cpp
+00003a60: 2c31 3135 360a 766f 6964 2053 6861 7271  ,1156.void Sharq
+00003a70: 6974 3a3a 5a58 4469 6167 7261 6d3a 3a66  it::ZXDiagram::f
+00003a80: 7573 655f 7370 6964 6572 7328 7f66 7573  use_spiders(.fus
+00003a90: 655f 7370 6964 6572 7301 382c 3134 320a  e_spiders.8,142.
+00003aa0: 766f 6964 2053 6861 7271 6974 3a3a 5a58  void Sharqit::ZX
+00003ab0: 4469 6167 7261 6d3a 3a63 6f6e 765f 785f  Diagram::conv_x_
+00003ac0: 746f 5f7a 287f 636f 6e76 5f78 5f74 6f5f  to_z(.conv_x_to_
+00003ad0: 7a01 3638 2c31 3639 360a 766f 6964 2053  z.68,1696.void S
+00003ae0: 6861 7271 6974 3a3a 5a58 4469 6167 7261  harqit::ZXDiagra
+00003af0: 6d3a 3a72 656d 6f76 655f 7061 7261 6c6c  m::remove_parall
+00003b00: 656c 5f73 656c 666c 6f6f 7073 5f68 6164  el_selfloops_had
+00003b10: 616d 6172 645f 6564 6765 7328 7f72 656d  amard_edges(.rem
+00003b20: 6f76 655f 7061 7261 6c6c 656c 5f73 656c  ove_parallel_sel
+00003b30: 666c 6f6f 7073 5f68 6164 616d 6172 645f  floops_hadamard_
+00003b40: 6564 6765 7301 3837 2c32 3234 360a 766f  edges.87,2246.vo
+00003b50: 6964 2053 6861 7271 6974 3a3a 5a58 4469  id Sharqit::ZXDi
+00003b60: 6167 7261 6d3a 3a75 7064 6174 655f 6e6f  agram::update_no
+00003b70: 6465 5f70 6c61 6365 7328 7f75 7064 6174  de_places(.updat
+00003b80: 655f 6e6f 6465 5f70 6c61 6365 7301 3131  e_node_places.11
+00003b90: 382c 3333 3434 0a76 6f69 6420 5368 6172  8,3344.void Shar
+00003ba0: 7169 743a 3a5a 5844 6961 6772 616d 3a3a  qit::ZXDiagram::
+00003bb0: 7570 6461 7465 5f70 6861 7365 5f67 6164  update_phase_gad
+00003bc0: 6765 7428 7f75 7064 6174 655f 7068 6173  get(.update_phas
+00003bd0: 655f 6761 6467 6574 0131 3432 2c34 3130  e_gadget.142,410
+00003be0: 360a 766f 6964 2053 6861 7271 6974 3a3a  6.void Sharqit::
+00003bf0: 5a58 4469 6167 7261 6d3a 3a67 7261 7068  ZXDiagram::graph
+00003c00: 5f6c 696b 6528 7f67 7261 7068 5f6c 696b  _like(.graph_lik
+00003c10: 6501 3136 352c 3437 3830 0a76 6f69 6420  e.165,4780.void 
+00003c20: 5368 6172 7169 743a 3a5a 5844 6961 6772  Sharqit::ZXDiagr
+00003c30: 616d 3a3a 6c63 6f6d 705f 6f6e 655f 7469  am::lcomp_one_ti
+00003c40: 6d65 287f 6c63 6f6d 705f 6f6e 655f 7469  me(.lcomp_one_ti
+00003c50: 6d65 0132 3238 2c36 3530 300a 7569 6e74  me.228,6500.uint
+00003c60: 3332 5f74 2053 6861 7271 6974 3a3a 5a58  32_t Sharqit::ZX
+00003c70: 4469 6167 7261 6d3a 3a6c 636f 6d70 287f  Diagram::lcomp(.
+00003c80: 6c63 6f6d 7001 3234 332c 3639 3830 0a76  lcomp.243,6980.v
+00003c90: 6f69 6420 5368 6172 7169 743a 3a5a 5844  oid Sharqit::ZXD
+00003ca0: 6961 6772 616d 3a3a 7069 766f 7431 5f6f  iagram::pivot1_o
+00003cb0: 6e65 5f74 696d 6528 7f70 6976 6f74 315f  ne_time(.pivot1_
+00003cc0: 6f6e 655f 7469 6d65 0132 3935 2c38 3334  one_time.295,834
+00003cd0: 360a 7569 6e74 3332 5f74 2053 6861 7271  6.uint32_t Sharq
+00003ce0: 6974 3a3a 5a58 4469 6167 7261 6d3a 3a70  it::ZXDiagram::p
+00003cf0: 6976 6f74 3128 7f70 6976 6f74 3101 3335  ivot1(.pivot1.35
+00003d00: 312c 3130 3237 300a 766f 6964 2053 6861  1,10270.void Sha
+00003d10: 7271 6974 3a3a 5a58 4469 6167 7261 6d3a  rqit::ZXDiagram:
+00003d20: 3a70 6976 6f74 325f 6f6e 655f 7469 6d65  :pivot2_one_time
+00003d30: 287f 7069 766f 7432 5f6f 6e65 5f74 696d  (.pivot2_one_tim
+00003d40: 6501 3433 312c 3132 3238 300a 7569 6e74  e.431,12280.uint
+00003d50: 3332 5f74 2053 6861 7271 6974 3a3a 5a58  32_t Sharqit::ZX
+00003d60: 4469 6167 7261 6d3a 3a70 6976 6f74 3228  Diagram::pivot2(
+00003d70: 7f70 6976 6f74 3201 3531 312c 3134 3937  .pivot2.511,1497
+00003d80: 360a 766f 6964 2053 6861 7271 6974 3a3a  6.void Sharqit::
+00003d90: 5a58 4469 6167 7261 6d3a 3a70 6976 6f74  ZXDiagram::pivot
+00003da0: 335f 6f6e 655f 7469 6d65 287f 7069 766f  3_one_time(.pivo
+00003db0: 7433 5f6f 6e65 5f74 696d 6501 3539 322c  t3_one_time.592,
+00003dc0: 3137 3033 380a 7569 6e74 3332 5f74 2053  17038.uint32_t S
+00003dd0: 6861 7271 6974 3a3a 5a58 4469 6167 7261  harqit::ZXDiagra
+00003de0: 6d3a 3a70 6976 6f74 3328 7f70 6976 6f74  m::pivot3(.pivot
+00003df0: 3301 3639 322c 3230 3336 330a 766f 6964  3.692,20363.void
+00003e00: 2053 6861 7271 6974 3a3a 5a58 4469 6167   Sharqit::ZXDiag
+00003e10: 7261 6d3a 3a69 645f 7265 6d6f 7661 6c28  ram::id_removal(
+00003e20: 7f69 645f 7265 6d6f 7661 6c01 3738 332c  .id_removal.783,
+00003e30: 3232 3639 300a 766f 6964 2053 6861 7271  22690.void Sharq
+00003e40: 6974 3a3a 5a58 4469 6167 7261 6d3a 3a67  it::ZXDiagram::g
+00003e50: 6675 7369 6f6e 5f6f 6e65 5f74 696d 6528  fusion_one_time(
+00003e60: 7f67 6675 7369 6f6e 5f6f 6e65 5f74 696d  .gfusion_one_tim
+00003e70: 6501 3833 382c 3234 3332 390a 7569 6e74  e.838,24329.uint
+00003e80: 3332 5f74 2053 6861 7271 6974 3a3a 5a58  32_t Sharqit::ZX
+00003e90: 4469 6167 7261 6d3a 3a67 6675 7369 6f6e  Diagram::gfusion
+00003ea0: 287f 6766 7573 696f 6e01 3834 362c 3234  (.gfusion.846,24
+00003eb0: 3634 380a 766f 6964 2053 6861 7271 6974  648.void Sharqit
+00003ec0: 3a3a 5a58 4469 6167 7261 6d3a 3a73 696d  ::ZXDiagram::sim
+00003ed0: 706c 6966 7928 7f73 696d 706c 6966 7901  plify(.simplify.
+00003ee0: 3937 392c 3238 3434 370a 0c0a 7068 6173  979,28447...phas
+00003ef0: 652e 682c 3931 340a 2364 6566 696e 6520  e.h,914.#define 
+00003f00: 5048 4153 455f 487f 372c 3830 0a20 2063  PHASE_H.7,80.  c
+00003f10: 6c61 7373 2050 6861 7365 7f32 332c 3239  lass Phase.23,29
+00003f20: 360a 2020 2020 4672 6163 7469 6f6e 2066  6.    Fraction f
+00003f30: 7261 635f 3b7f 3236 2c33 3235 0a20 2020  rac_;.26,325.   
+00003f40: 2050 6861 7365 287f 3333 2c36 3238 0a20   Phase(.33,628. 
+00003f50: 2020 2050 6861 7365 287f 3338 2c38 3437     Phase(.38,847
+00003f60: 0a20 2020 2050 6861 7365 287f 3433 2c31  .    Phase(.43,1
+00003f70: 3034 310a 2020 2020 5068 6173 6528 7f34  041.    Phase(.4
+00003f80: 382c 3131 3637 0a20 2020 2046 7261 6374  8,1167.    Fract
+00003f90: 696f 6e20 6672 6163 287f 3530 2c31 3234  ion frac(.50,124
+00003fa0: 390a 2020 2020 766f 6964 2066 7261 6328  9.    void frac(
+00003fb0: 7f35 322c 3133 3231 0a20 2020 2064 6f75  .52,1321.    dou
+00003fc0: 626c 6520 7661 6c75 6528 7f36 322c 3136  ble value(.62,16
+00003fd0: 3038 0a20 2020 2062 6f6f 6c20 6973 5f7a  08.    bool is_z
+00003fe0: 6572 6f28 7f36 372c 3138 3035 0a20 2020  ero(.67,1805.   
+00003ff0: 2062 6f6f 6c20 6973 5f70 6f73 6974 6976   bool is_positiv
+00004000: 6528 7f37 322c 3139 3833 0a20 2020 2062  e(.72,1983.    b
+00004010: 6f6f 6c20 6973 5f6e 6567 6174 6976 6528  ool is_negative(
+00004020: 7f37 372c 3231 3635 0a20 2020 2076 6f69  .77,2165.    voi
+00004030: 6420 7265 6475 6365 287f 3831 2c32 3330  d reduce(.81,230
+00004040: 320a 2020 2020 766f 6964 206d 6f64 5f32  2.    void mod_2
+00004050: 7069 287f 3835 2c32 3339 310a 2020 2020  pi(.85,2391.    
+00004060: 5068 6173 6520 6f70 6572 6174 6f72 2b28  Phase operator+(
+00004070: 7f39 392c 3238 3932 0a20 2020 2050 6861  .99,2892.    Pha
+00004080: 7365 206f 7065 7261 746f 722d 287f 3130  se operator-(.10
+00004090: 302c 3239 3338 0a20 2020 2050 6861 7365  0,2938.    Phase
+000040a0: 2620 6f70 6572 6174 6f72 2b3d 287f 6f70  & operator+=(.op
+000040b0: 6572 6174 6f72 2b3d 0131 3031 2c32 3939  erator+=.101,299
+000040c0: 320a 2020 2020 5068 6173 6526 206f 7065  2.    Phase& ope
+000040d0: 7261 746f 722d 3d28 7f6f 7065 7261 746f  rator-=(.operato
+000040e0: 722d 3d01 3130 322c 3330 3731 0a20 2020  r-=.102,3071.   
+000040f0: 2050 6861 7365 2620 6f70 6572 6174 6f72   Phase& operator
+00004100: 2a3d 287f 6f70 6572 6174 6f72 2a3d 0131  *=(.operator*=.1
+00004110: 3033 2c33 3135 300a 2020 2020 5068 6173  03,3150.    Phas
+00004120: 6526 206f 7065 7261 746f 722f 3d28 7f6f  e& operator/=(.o
+00004130: 7065 7261 746f 722f 3d01 3130 342c 3332  perator/=.104,32
+00004140: 3233 0a20 2020 2066 7269 656e 6420 626f  23.    friend bo
+00004150: 6f6c 206f 7065 7261 746f 723d 3d28 7f6f  ol operator==(.o
+00004160: 7065 7261 746f 723d 3d01 3130 352c 3332  perator==.105,32
+00004170: 3936 0a20 2020 2066 7269 656e 6420 626f  96.    friend bo
+00004180: 6f6c 206f 7065 7261 746f 7221 3d28 7f6f  ol operator!=(.o
+00004190: 7065 7261 746f 7221 3d01 3131 302c 3335  perator!=.110,35
+000041a0: 3036 0a20 2020 2066 7269 656e 6420 5068  06.    friend Ph
+000041b0: 6173 6520 6f70 6572 6174 6f72 2b28 7f31  ase operator+(.1
+000041c0: 3131 2c33 3539 350a 2020 2020 6672 6965  11,3595.    frie
+000041d0: 6e64 2050 6861 7365 206f 7065 7261 746f  nd Phase operato
+000041e0: 722d 287f 3131 322c 3337 3031 0a20 2020  r-(.112,3701.   
+000041f0: 2066 7269 656e 6420 5068 6173 6520 6f70   friend Phase op
+00004200: 6572 6174 6f72 2a28 7f31 3133 2c33 3830  erator*(.113,380
+00004210: 370a 2020 2020 6672 6965 6e64 2050 6861  7.    friend Pha
+00004220: 7365 206f 7065 7261 746f 722a 287f 3131  se operator*(.11
+00004230: 342c 3339 3037 0a20 2020 2066 7269 656e  4,3907.    frien
+00004240: 6420 5068 6173 6520 6f70 6572 6174 6f72  d Phase operator
+00004250: 2f28 7f31 3135 2c34 3030 370a 2020 2020  /(.115,4007.    
+00004260: 6672 6965 6e64 2073 7464 3a3a 6f73 7472  friend std::ostr
+00004270: 6561 6d26 206f 7065 7261 746f 723c 3c28  eam& operator<<(
+00004280: 7f31 3136 2c34 3130 370a 0c0a 6672 6163  .116,4107...frac
+00004290: 7469 6f6e 2e68 2c31 3731 320a 2364 6566  tion.h,1712.#def
+000042a0: 696e 6520 4652 4143 5449 4f4e 5f48 7f37  ine FRACTION_H.7
+000042b0: 2c38 390a 2020 636c 6173 7320 4672 6163  ,89.  class Frac
+000042c0: 7469 6f6e 7f31 382c 3234 320a 2020 2020  tion.18,242.    
+000042d0: 696e 7433 325f 7420 6e75 6d65 7261 746f  int32_t numerato
+000042e0: 725f 3b7f 3231 2c32 3734 0a20 2020 2069  r_;.21,274.    i
+000042f0: 6e74 3332 5f74 2064 656e 6f6d 696e 6174  nt32_t denominat
+00004300: 6f72 5f3b 7f32 322c 3332 390a 2020 2020  or_;.22,329.    
+00004310: 4672 6163 7469 6f6e 287f 3237 2c34 3536  Fraction(.27,456
+00004320: 0a20 2020 2046 7261 6374 696f 6e28 7f33  .    Fraction(.3
+00004330: 332c 3637 390a 2020 2020 4672 6163 7469  3,679.    Fracti
+00004340: 6f6e 287f 3339 2c39 3139 0a20 2020 2069  on(.39,919.    i
+00004350: 6e74 3332 5f74 206e 756d 6572 6174 6f72  nt32_t numerator
+00004360: 287f 3431 2c31 3035 330a 2020 2020 696e  (.41,1053.    in
+00004370: 7433 325f 7420 6465 6e6f 6d69 6e61 746f  t32_t denominato
+00004380: 7228 7f34 332c 3131 3431 0a20 2020 2076  r(.43,1141.    v
+00004390: 6f69 6420 6e75 6d65 7261 746f 7228 7f34  oid numerator(.4
+000043a0: 352c 3132 3331 0a20 2020 2076 6f69 6420  5,1231.    void 
+000043b0: 6465 6e6f 6d69 6e61 746f 7228 7f34 372c  denominator(.47,
+000043c0: 3133 3438 0a20 2020 2046 7261 6374 696f  1348.    Fractio
+000043d0: 6e20 6164 6428 7f35 382c 3137 3039 0a20  n add(.58,1709. 
+000043e0: 2020 2046 7261 6374 696f 6e20 6164 6428     Fraction add(
+000043f0: 7f36 392c 3231 3330 0a20 2020 2046 7261  .69,2130.    Fra
+00004400: 6374 696f 6e20 7375 6228 7f37 352c 3233  ction sub(.75,23
+00004410: 3439 0a20 2020 2046 7261 6374 696f 6e20  49.    Fraction 
+00004420: 7375 6228 7f38 362c 3237 3732 0a20 2020  sub(.86,2772.   
+00004430: 2046 7261 6374 696f 6e20 6d75 6c28 7f39   Fraction mul(.9
+00004440: 322c 3239 3931 0a20 2020 2046 7261 6374  2,2991.    Fract
+00004450: 696f 6e20 6d75 6c28 7f31 3033 2c33 3337  ion mul(.103,337
+00004460: 370a 2020 2020 4672 6163 7469 6f6e 2064  7.    Fraction d
+00004470: 6976 287f 3130 392c 3335 3931 0a20 2020  iv(.109,3591.   
+00004480: 2046 7261 6374 696f 6e20 6469 7628 7f31   Fraction div(.1
+00004490: 3230 2c33 3937 360a 2020 2020 626f 6f6c  20,3976.    bool
+000044a0: 2069 735f 7a65 726f 287f 3132 352c 3431   is_zero(.125,41
+000044b0: 3732 0a20 2020 2062 6f6f 6c20 6973 5f70  72.    bool is_p
+000044c0: 6f73 6974 6976 6528 7f31 3330 2c34 3335  ositive(.130,435
+000044d0: 320a 2020 2020 626f 6f6c 2069 735f 6e65  2.    bool is_ne
+000044e0: 6761 7469 7665 287f 3133 352c 3435 3530  gative(.135,4550
+000044f0: 0a20 2020 2076 6f69 6420 7265 6475 6365  .    void reduce
+00004500: 287f 3133 392c 3436 3731 0a20 2020 2073  (.139,4671.    s
+00004510: 7461 7469 6320 696e 7433 325f 7420 6763  tatic int32_t gc
+00004520: 6428 7f31 3630 2c35 3237 390a 2020 2020  d(.160,5279.    
+00004530: 4672 6163 7469 6f6e 206f 7065 7261 746f  Fraction operato
+00004540: 722b 287f 3137 322c 3535 3335 0a20 2020  r+(.172,5535.   
+00004550: 2046 7261 6374 696f 6e20 6f70 6572 6174   Fraction operat
+00004560: 6f72 2d28 7f31 3733 2c35 3538 340a 2020  or-(.173,5584.  
+00004570: 2020 4672 6163 7469 6f6e 2620 6f70 6572    Fraction& oper
+00004580: 6174 6f72 2b3d 287f 6f70 6572 6174 6f72  ator+=(.operator
+00004590: 2b3d 0131 3734 2c35 3633 350a 2020 2020  +=.174,5635.    
+000045a0: 4672 6163 7469 6f6e 2620 6f70 6572 6174  Fraction& operat
+000045b0: 6f72 2b3d 287f 6f70 6572 6174 6f72 2b3d  or+=(.operator+=
+000045c0: 0131 3831 2c35 3832 330a 2020 2020 4672  .181,5823.    Fr
+000045d0: 6163 7469 6f6e 2620 6f70 6572 6174 6f72  action& operator
+000045e0: 2d3d 287f 6f70 6572 6174 6f72 2d3d 0131  -=(.operator-=.1
+000045f0: 3832 2c35 3930 350a 2020 2020 4672 6163  82,5905.    Frac
+00004600: 7469 6f6e 2620 6f70 6572 6174 6f72 2d3d  tion& operator-=
+00004610: 287f 6f70 6572 6174 6f72 2d3d 0131 3839  (.operator-=.189
+00004620: 2c36 3039 330a 2020 2020 4672 6163 7469  ,6093.    Fracti
+00004630: 6f6e 2620 6f70 6572 6174 6f72 2a3d 287f  on& operator*=(.
+00004640: 6f70 6572 6174 6f72 2a3d 0131 3930 2c36  operator*=.190,6
+00004650: 3137 350a 2020 2020 4672 6163 7469 6f6e  175.    Fraction
+00004660: 2620 6f70 6572 6174 6f72 2a3d 287f 6f70  & operator*=(.op
+00004670: 6572 6174 6f72 2a3d 0131 3937 2c36 3336  erator*=.197,636
+00004680: 330a 2020 2020 4672 6163 7469 6f6e 2620  3.    Fraction& 
+00004690: 6f70 6572 6174 6f72 2f3d 287f 6f70 6572  operator/=(.oper
+000046a0: 6174 6f72 2f3d 0131 3938 2c36 3434 350a  ator/=.198,6445.
+000046b0: 2020 2020 4672 6163 7469 6f6e 2620 6f70      Fraction& op
+000046c0: 6572 6174 6f72 2f3d 287f 6f70 6572 6174  erator/=(.operat
+000046d0: 6f72 2f3d 0132 3035 2c36 3633 330a 2020  or/=.205,6633.  
+000046e0: 2020 6672 6965 6e64 2062 6f6f 6c20 6f70    friend bool op
+000046f0: 6572 6174 6f72 3d3d 287f 6f70 6572 6174  erator==(.operat
+00004700: 6f72 3d3d 0132 3036 2c36 3731 350a 2020  or==.206,6715.  
+00004710: 2020 6672 6965 6e64 2062 6f6f 6c20 6f70    friend bool op
+00004720: 6572 6174 6f72 213d 287f 6f70 6572 6174  erator!=(.operat
+00004730: 6f72 213d 0132 3130 2c36 3838 370a 2020  or!=.210,6887.  
+00004740: 2020 6672 6965 6e64 2046 7261 6374 696f    friend Fractio
+00004750: 6e20 6f70 6572 6174 6f72 2b28 7f32 3131  n operator+(.211
+00004760: 2c36 3938 320a 2020 2020 6672 6965 6e64  ,6982.    friend
+00004770: 2046 7261 6374 696f 6e20 6f70 6572 6174   Fraction operat
+00004780: 6f72 2b28 7f32 3132 2c37 3037 390a 2020  or+(.212,7079.  
+00004790: 2020 6672 6965 6e64 2046 7261 6374 696f    friend Fractio
+000047a0: 6e20 6f70 6572 6174 6f72 2b28 7f32 3133  n operator+(.213
+000047b0: 2c37 3138 340a 2020 2020 6672 6965 6e64  ,7184.    friend
+000047c0: 2046 7261 6374 696f 6e20 6f70 6572 6174   Fraction operat
+000047d0: 6f72 2d28 7f32 3134 2c37 3238 390a 2020  or-(.214,7289.  
+000047e0: 2020 6672 6965 6e64 2046 7261 6374 696f    friend Fractio
+000047f0: 6e20 6f70 6572 6174 6f72 2d28 7f32 3135  n operator-(.215
+00004800: 2c37 3338 360a 2020 2020 6672 6965 6e64  ,7386.    friend
+00004810: 2046 7261 6374 696f 6e20 6f70 6572 6174   Fraction operat
+00004820: 6f72 2d28 7f32 3136 2c37 3439 310a 2020  or-(.216,7491.  
+00004830: 2020 6672 6965 6e64 2046 7261 6374 696f    friend Fractio
+00004840: 6e20 6f70 6572 6174 6f72 2a28 7f32 3137  n operator*(.217
+00004850: 2c37 3539 360a 2020 2020 6672 6965 6e64  ,7596.    friend
+00004860: 2046 7261 6374 696f 6e20 6f70 6572 6174   Fraction operat
+00004870: 6f72 2a28 7f32 3138 2c37 3639 330a 2020  or*(.218,7693.  
+00004880: 2020 6672 6965 6e64 2046 7261 6374 696f    friend Fractio
+00004890: 6e20 6f70 6572 6174 6f72 2a28 7f32 3139  n operator*(.219
+000048a0: 2c37 3739 380a 2020 2020 6672 6965 6e64  ,7798.    friend
+000048b0: 2046 7261 6374 696f 6e20 6f70 6572 6174   Fraction operat
+000048c0: 6f72 2f28 7f32 3230 2c37 3930 330a 2020  or/(.220,7903.  
+000048d0: 2020 6672 6965 6e64 2046 7261 6374 696f    friend Fractio
+000048e0: 6e20 6f70 6572 6174 6f72 2f28 7f32 3231  n operator/(.221
+000048f0: 2c38 3030 300a 2020 2020 6672 6965 6e64  ,8000.    friend
+00004900: 2046 7261 6374 696f 6e20 6f70 6572 6174   Fraction operat
+00004910: 6f72 2f28 7f32 3232 2c38 3130 350a 2020  or/(.222,8105.  
+00004920: 2020 6672 6965 6e64 2073 7464 3a3a 6f73    friend std::os
+00004930: 7472 6561 6d26 206f 7065 7261 746f 723c  tream& operator<
+00004940: 3c28 7f32 3233 2c38 3231 300a 0c0a 7a78  <(.223,8210...zx
+00004950: 6e6f 6465 2e63 7070 2c34 350a 7374 643a  node.cpp,45.std:
+00004960: 3a73 7472 696e 6720 5368 6172 7169 743a  :string Sharqit:
+00004970: 3a5a 584e 6f64 653a 3a6e 616d 6528 7f6e  :ZXNode::name(.n
+00004980: 616d 6501 382c 3839 0a0c 0a7a 7864 6961  ame.8,89...zxdia
+00004990: 6772 616d 2e63 7070 2c31 3230 360a 5368  gram.cpp,1206.Sh
+000049a0: 6172 7169 743a 3a5a 5844 6961 6772 616d  arqit::ZXDiagram
+000049b0: 3a3a 5a58 4469 6167 7261 6d28 7f5a 5844  ::ZXDiagram(.ZXD
+000049c0: 6961 6772 616d 0138 2c39 350a 7374 643a  iagram.8,95.std:
+000049d0: 3a73 7472 696e 6720 5368 6172 7169 743a  :string Sharqit:
+000049e0: 3a5a 5844 6961 6772 616d 3a3a 746f 5f73  :ZXDiagram::to_s
+000049f0: 7472 696e 6728 7f74 6f5f 7374 7269 6e67  tring(.to_string
+00004a00: 0133 342c 3839 350a 7374 643a 3a6d 6170  .34,895.std::map
+00004a10: 3c73 7464 3a3a 7374 7269 6e67 2c20 7569  <std::string, ui
+00004a20: 6e74 3332 5f74 3e20 5368 6172 7169 743a  nt32_t> Sharqit:
+00004a30: 3a5a 5844 6961 6772 616d 3a3a 7374 6174  :ZXDiagram::stat
+00004a40: 7328 7f73 7461 7473 0135 342c 3134 3034  s(.stats.54,1404
+00004a50: 0a76 6f69 6420 5368 6172 7169 743a 3a5a  .void Sharqit::Z
+00004a60: 5844 6961 6772 616d 3a3a 746f 5f64 6f74  XDiagram::to_dot
+00004a70: 5f66 696c 6528 7f74 6f5f 646f 745f 6669  _file(.to_dot_fi
+00004a80: 6c65 0138 302c 3233 3738 0a76 6f69 6420  le.80,2378.void 
+00004a90: 5368 6172 7169 743a 3a5a 5844 6961 6772  Sharqit::ZXDiagr
+00004aa0: 616d 3a3a 746f 5f73 7667 5f66 696c 6528  am::to_svg_file(
+00004ab0: 7f74 6f5f 7376 675f 6669 6c65 0132 3234  .to_svg_file.224
+00004ac0: 2c36 3930 390a 766f 6964 2053 6861 7271  ,6909.void Sharq
+00004ad0: 6974 3a3a 5a58 4469 6167 7261 6d3a 3a61  it::ZXDiagram::a
+00004ae0: 6464 5f71 6761 7465 287f 6164 645f 7167  dd_qgate(.add_qg
+00004af0: 6174 6501 3233 372c 3733 3834 0a62 6f6f  ate.237,7384.boo
+00004b00: 6c20 5368 6172 7169 743a 3a5a 5844 6961  l Sharqit::ZXDia
+00004b10: 6772 616d 3a3a 6368 6563 6b5f 636f 6e6e  gram::check_conn
+00004b20: 6563 7428 7f63 6865 636b 5f63 6f6e 6e65  ect(.check_conne
+00004b30: 6374 0133 3738 2c31 3230 3235 0a76 6f69  ct.378,12025.voi
+00004b40: 6420 5368 6172 7169 743a 3a5a 5844 6961  d Sharqit::ZXDia
+00004b50: 6772 616d 3a3a 786f 725f 6861 6461 6d61  gram::xor_hadama
+00004b60: 7264 5f65 6467 6528 7f78 6f72 5f68 6164  rd_edge(.xor_had
+00004b70: 616d 6172 645f 6564 6765 0134 3031 2c31  amard_edge.401,1
+00004b80: 3234 3333 0a76 6f69 6420 5368 6172 7169  2433.void Sharqi
+00004b90: 743a 3a5a 5844 6961 6772 616d 3a3a 786f  t::ZXDiagram::xo
+00004ba0: 725f 6861 6461 6d61 7264 5f65 6467 6573  r_hadamard_edges
+00004bb0: 287f 786f 725f 6861 6461 6d61 7264 5f65  (.xor_hadamard_e
+00004bc0: 6467 6573 0134 3334 2c31 3334 3337 0a53  dges.434,13437.S
+00004bd0: 6861 7271 6974 3a3a 5a58 4e6f 6465 4b69  harqit::ZXNodeKi
+00004be0: 6e64 2053 6861 7271 6974 3a3a 5a58 4469  nd Sharqit::ZXDi
+00004bf0: 6167 7261 6d3a 3a72 656d 6f76 655f 6e6f  agram::remove_no
+00004c00: 6465 287f 7265 6d6f 7665 5f6e 6f64 6501  de(.remove_node.
+00004c10: 3434 362c 3133 3830 370a 5368 6172 7169  446,13807.Sharqi
+00004c20: 743a 3a5a 5845 6467 654b 696e 6420 5368  t::ZXEdgeKind Sh
+00004c30: 6172 7169 743a 3a5a 5844 6961 6772 616d  arqit::ZXDiagram
+00004c40: 3a3a 7265 6d6f 7665 5f65 6467 6528 7f72  ::remove_edge(.r
+00004c50: 656d 6f76 655f 6564 6765 0134 3830 2c31  emove_edge.480,1
+00004c60: 3435 3036 0a75 696e 7433 325f 7420 5368  4506.uint32_t Sh
+00004c70: 6172 7169 743a 3a5a 5844 6961 6772 616d  arqit::ZXDiagram
+00004c80: 3a3a 6170 7065 6e64 5f6e 6f64 6528 7f61  ::append_node(.a
+00004c90: 7070 656e 645f 6e6f 6465 0135 3034 2c31  ppend_node.504,1
+00004ca0: 3530 3437 0a75 696e 7433 325f 7420 5368  5047.uint32_t Sh
+00004cb0: 6172 7169 743a 3a5a 5844 6961 6772 616d  arqit::ZXDiagram
+00004cc0: 3a3a 6170 7065 6e64 5f6e 6f64 6528 7f61  ::append_node(.a
+00004cd0: 7070 656e 645f 6e6f 6465 0135 3132 2c31  ppend_node.512,1
+00004ce0: 3532 3431 0a76 6f69 6420 5368 6172 7169  5241.void Sharqi
+00004cf0: 743a 3a5a 5844 6961 6772 616d 3a3a 636f  t::ZXDiagram::co
+00004d00: 6e6e 6563 745f 6e6f 6465 7328 7f63 6f6e  nnect_nodes(.con
+00004d10: 6e65 6374 5f6e 6f64 6573 0135 3235 2c31  nect_nodes.525,1
+00004d20: 3535 3833 0a76 6f69 6420 5368 6172 7169  5583.void Sharqi
+00004d30: 743a 3a5a 5844 6961 6772 616d 3a3a 7377  t::ZXDiagram::sw
+00004d40: 6170 5f6e 6f64 6573 287f 7377 6170 5f6e  ap_nodes(.swap_n
+00004d50: 6f64 6573 0135 3333 2c31 3538 3339 0a76  odes.533,15839.v
+00004d60: 6f69 6420 5368 6172 7169 743a 3a5a 5844  oid Sharqit::ZXD
+00004d70: 6961 6772 616d 3a3a 7265 6d6f 7665 5f69  iagram::remove_i
+00004d80: 736f 6c61 7465 645f 7370 6964 6572 7328  solated_spiders(
+00004d90: 7f72 656d 6f76 655f 6973 6f6c 6174 6564  .remove_isolated
+00004da0: 5f73 7069 6465 7273 0135 3438 2c31 3632  _spiders.548,162
+00004db0: 3235 0a76 6f69 6420 5368 6172 7169 743a  25.void Sharqit:
+00004dc0: 3a5a 5844 6961 6772 616d 3a3a 726f 775f  :ZXDiagram::row_
+00004dd0: 6f70 6572 6174 696f 6e28 7f72 6f77 5f6f  operation(.row_o
+00004de0: 7065 7261 7469 6f6e 0135 3634 2c31 3635  peration.564,165
+00004df0: 3438 0a73 7464 3a3a 7665 6374 6f72 3c75  48.std::vector<u
+00004e00: 696e 7433 325f 743e 2053 6861 7271 6974  int32_t> Sharqit
+00004e10: 3a3a 5a58 4469 6167 7261 6d3a 3a61 646a  ::ZXDiagram::adj
+00004e20: 6163 656e 745f 6e6f 6465 5f69 6e64 6578  acent_node_index
+00004e30: 6573 287f 6164 6a61 6365 6e74 5f6e 6f64  es(.adjacent_nod
+00004e40: 655f 696e 6465 7865 7301 3537 332c 3136  e_indexes.573,16
+00004e50: 3736 360a 0c0a 6269 6e61 7279 5f6d 6174  766...binary_mat
+00004e60: 7269 782e 6370 702c 3136 320a 7374 643a  rix.cpp,162.std:
+00004e70: 3a73 7472 696e 6720 5368 6172 7169 743a  :string Sharqit:
+00004e80: 3a42 696e 6172 794d 6174 7269 783a 3a74  :BinaryMatrix::t
+00004e90: 6f5f 7374 7269 6e67 287f 746f 5f73 7472  o_string(.to_str
+00004ea0: 696e 6701 382c 3131 330a 7374 643a 3a76  ing.8,113.std::v
+00004eb0: 6563 746f 723c 7374 643a 3a70 6169 723c  ector<std::pair<
+00004ec0: 7569 6e74 3332 5f74 2c20 7569 6e74 3332  uint32_t, uint32
+00004ed0: 5f74 3e3e 2053 6861 7271 6974 3a3a 4269  _t>> Sharqit::Bi
+00004ee0: 6e61 7279 4d61 7472 6978 3a3a 6761 7573  naryMatrix::gaus
+00004ef0: 735f 7265 6475 6365 287f 6761 7573 735f  s_reduce(.gauss_
+00004f00: 7265 6475 6365 0132 382c 3439 300a 0c0a  reduce.28,490...
+00004f10: 7a78 2e68 2c33 3139 320a 2364 6566 696e  zx.h,3192.#defin
+00004f20: 6520 5a58 5f48 7f31 312c 3839 330a 2020  e ZX_H.11,893.  
+00004f30: 656e 756d 205a 584e 6f64 654b 696e 6420  enum ZXNodeKind 
+00004f40: 7f32 352c 3130 3832 0a09 0920 2020 5853  .25,1082...   XS
+00004f50: 7069 6465 722c 7f32 362c 3131 3032 0a09  pider,.26,1102..
+00004f60: 0920 2020 5a53 7069 6465 722c 7f32 372c  .   ZSpider,.27,
+00004f70: 3131 3330 0a09 0920 2020 496e 7075 742c  1130...   Input,
+00004f80: 7f32 382c 3131 3538 0a09 0920 2020 4f75  .28,1158...   Ou
+00004f90: 7470 7574 207f 3239 2c31 3138 360a 2020  tput .29,1186.  
+00004fa0: 656e 756d 205a 5845 6467 654b 696e 6420  enum ZXEdgeKind 
+00004fb0: 7f33 322c 3132 3534 0a09 0920 2020 4e6f  .32,1254...   No
+00004fc0: 6e65 2c7f 3333 2c31 3237 340a 0909 2020  ne,.33,1274...  
+00004fd0: 2050 6c61 696e 2c7f 3334 2c31 3331 320a   Plain,.34,1312.
+00004fe0: 0909 2020 2048 6164 616d 6172 6420 7f33  ..   Hadamard .3
+00004ff0: 352c 3133 3738 0a20 2065 6e75 6d20 5a58  5,1378.  enum ZX
+00005000: 4469 6167 7261 6d4b 696e 6420 7f33 382c  DiagramKind .38,
+00005010: 3134 3631 0a09 0920 2020 2020 2047 656e  1461...      Gen
+00005020: 6572 616c 2c7f 3339 2c31 3438 340a 0909  eral,.39,1484...
+00005030: 2020 2020 2020 4772 6170 684c 696b 6520        GraphLike 
+00005040: 7f34 302c 3135 3235 0a20 2065 6e75 6d20  .40,1525.  enum 
+00005050: 5a58 4e6f 6465 506c 6163 6520 7f34 332c  ZXNodePlace .43,
+00005060: 3136 3030 0a09 0920 2020 2054 6572 6d69  1600...    Termi
+00005070: 6e61 6c2c 7f34 342c 3136 3231 0a09 0920  nal,.44,1621... 
+00005080: 2020 2042 6f75 6e64 6172 792c 7f34 352c     Boundary,.45,
+00005090: 3136 3636 0a09 0920 2020 2049 6e74 6572  1666...    Inter
+000050a0: 6e61 6c20 7f34 362c 3137 3436 0a20 2063  nal .46,1746.  c
+000050b0: 6c61 7373 205a 584e 6f64 657f 3539 2c32  lass ZXNode.59,2
+000050c0: 3233 320a 2020 2020 5a58 4e6f 6465 4b69  232.    ZXNodeKi
+000050d0: 6e64 206b 696e 645f 3b7f 3632 2c32 3236  nd kind_;.62,226
+000050e0: 320a 2020 2020 5068 6173 6520 7068 6173  2.    Phase phas
+000050f0: 655f 3b7f 3633 2c32 3332 300a 2020 2020  e_;.63,2320.    
+00005100: 7569 6e74 3332 5f74 2071 5f3b 7f36 342c  uint32_t q_;.64,
+00005110: 3233 3735 0a20 2020 2062 6f6f 6c20 7067  2375.    bool pg
+00005120: 5f70 6861 7365 5f3b 7f36 352c 3234 3430  _phase_;.65,2440
+00005130: 0a20 2020 2062 6f6f 6c20 7067 5f72 6f6f  .    bool pg_roo
+00005140: 745f 3b7f 3636 2c32 3532 350a 2020 2020  t_;.66,2525.    
+00005150: 626f 6f6c 2070 675f 6c65 6166 5f3b 7f36  bool pg_leaf_;.6
+00005160: 372c 3236 3038 0a20 2020 205a 584e 6f64  7,2608.    ZXNod
+00005170: 6528 7f37 382c 3331 3237 0a20 2020 205a  e(.78,3127.    Z
+00005180: 584e 6f64 6528 7f38 352c 3335 3232 0a20  XNode(.85,3522. 
+00005190: 2020 205a 584e 6f64 654b 696e 6420 6b69     ZXNodeKind ki
+000051a0: 6e64 287f 3838 2c33 3732 300a 2020 2020  nd(.88,3720.    
+000051b0: 5068 6173 6520 7068 6173 6528 7f39 302c  Phase phase(.90,
+000051c0: 3337 3935 0a20 2020 2075 696e 7433 325f  3795.    uint32_
+000051d0: 7420 7128 7f39 322c 3338 3633 0a20 2020  t q(.92,3863.   
+000051e0: 2062 6f6f 6c20 7067 5f70 6861 7365 287f   bool pg_phase(.
+000051f0: 3934 2c33 3933 330a 2020 2020 626f 6f6c  94,3933.    bool
+00005200: 2070 675f 726f 6f74 287f 3936 2c34 3031   pg_root(.96,401
+00005210: 320a 2020 2020 626f 6f6c 2070 675f 6c65  2.    bool pg_le
+00005220: 6166 287f 3938 2c34 3038 390a 2020 2020  af(.98,4089.    
+00005230: 766f 6964 206b 696e 6428 7f31 3030 2c34  void kind(.100,4
+00005240: 3136 330a 2020 2020 766f 6964 2070 6861  163.    void pha
+00005250: 7365 287f 3130 322c 3432 3437 0a20 2020  se(.102,4247.   
+00005260: 2076 6f69 6420 7128 7f31 3034 2c34 3332   void q(.104,432
+00005270: 360a 2020 2020 766f 6964 2070 675f 7068  6.    void pg_ph
+00005280: 6173 6528 7f31 3036 2c34 3339 390a 2020  ase(.106,4399.  
+00005290: 2020 766f 6964 2070 675f 726f 6f74 287f    void pg_root(.
+000052a0: 3130 382c 3434 3935 0a20 2020 2076 6f69  108,4495.    voi
+000052b0: 6420 7067 5f6c 6561 6628 7f31 3130 2c34  d pg_leaf(.110,4
+000052c0: 3538 370a 2020 2020 7374 643a 3a73 7472  587.    std::str
+000052d0: 696e 6720 6b69 6e64 5f73 7472 287f 3131  ing kind_str(.11
+000052e0: 352c 3437 3537 0a20 2063 6c61 7373 205a  5,4757.  class Z
+000052f0: 5845 6467 657f 3133 322c 3531 3430 0a20  XEdge.132,5140. 
+00005300: 2020 205a 5845 6467 654b 696e 6420 6b69     ZXEdgeKind ki
+00005310: 6e64 5f3b 7f31 3335 2c35 3137 300a 2020  nd_;.135,5170.  
+00005320: 2020 7569 6e74 3332 5f74 2074 6f5f 3b7f    uint32_t to_;.
+00005330: 3133 362c 3532 3238 0a20 2020 205a 5845  136,5228.    ZXE
+00005340: 6467 6528 7f31 3433 2c35 3438 390a 2020  dge(.143,5489.  
+00005350: 2020 5a58 4564 6765 287f 3134 382c 3536    ZXEdge(.148,56
+00005360: 3838 0a20 2020 205a 5845 6467 654b 696e  88.    ZXEdgeKin
+00005370: 6420 6b69 6e64 287f 3135 302c 3537 3835  d kind(.150,5785
+00005380: 0a20 2020 2075 696e 7433 325f 7420 746f  .    uint32_t to
+00005390: 287f 3135 322c 3538 3537 0a20 2020 2076  (.152,5857.    v
+000053a0: 6f69 6420 6b69 6e64 287f 3135 342c 3539  oid kind(.154,59
+000053b0: 3235 0a20 2020 2076 6f69 6420 746f 287f  25.    void to(.
+000053c0: 3135 362c 3630 3036 0a20 2020 2073 7464  156,6006.    std
+000053d0: 3a3a 7374 7269 6e67 206b 696e 645f 7374  ::string kind_st
+000053e0: 7228 7f31 3631 2c36 3136 300a 2020 2020  r(.161,6160.    
+000053f0: 7374 643a 3a73 7472 696e 6720 6e61 6d65  std::string name
+00005400: 287f 3136 392c 3633 3837 0a20 2020 2076  (.169,6387.    v
+00005410: 6f69 6420 7265 7665 7273 655f 6b69 6e64  oid reverse_kind
+00005420: 287f 3138 312c 3637 3236 0a20 2063 6c61  (.181,6726.  cla
+00005430: 7373 205a 5844 6961 6772 616d 7f31 3938  ss ZXDiagram.198
+00005440: 2c37 3731 340a 2020 2020 5a58 4469 6167  ,7714.    ZXDiag
+00005450: 7261 6d4b 696e 6420 6b69 6e64 5f3b 7f32  ramKind kind_;.2
+00005460: 3031 2c37 3734 370a 2020 2020 7569 6e74  01,7747.    uint
+00005470: 3332 5f74 2071 7562 6974 5f6e 756d 5f3b  32_t qubit_num_;
+00005480: 7f32 3032 2c37 3830 300a 2020 2020 7374  .202,7800.    st
+00005490: 643a 3a76 6563 746f 723c 5a58 4e6f 6465  d::vector<ZXNode
+000054a0: 3e20 6e6f 6465 735f 3b7f 3230 332c 3738  > nodes_;.203,78
+000054b0: 3437 0a20 2020 2073 7464 3a3a 7665 6374  47.    std::vect
+000054c0: 6f72 3c75 696e 7433 325f 743e 2069 6e70  or<uint32_t> inp
+000054d0: 7574 735f 3b7f 3230 342c 3739 3133 0a20  uts_;.204,7913. 
+000054e0: 2020 2073 7464 3a3a 7665 6374 6f72 3c75     std::vector<u
+000054f0: 696e 7433 325f 743e 206f 7574 7075 7473  int32_t> outputs
+00005500: 5f3b 7f32 3035 2c37 3938 360a 2020 2020  _;.205,7986.    
+00005510: 7374 643a 3a76 6563 746f 723c 7374 643a  std::vector<std:
+00005520: 3a76 6563 746f 723c 5a58 4564 6765 3e3e  :vector<ZXEdge>>
+00005530: 2061 646a 5f6d 6174 5f3b 7f32 3036 2c38   adj_mat_;.206,8
+00005540: 3036 310a 2020 2020 7374 643a 3a76 6563  061.    std::vec
+00005550: 746f 723c 5a58 4e6f 6465 506c 6163 653e  tor<ZXNodePlace>
+00005560: 206e 6f64 655f 706c 6163 6573 5f3b 7f32   node_places_;.2
+00005570: 3037 2c38 3134 370a 2020 2020 7569 6e74  07,8147.    uint
+00005580: 3332 5f74 206d 6178 5f61 646a 5f6e 756d  32_t max_adj_num
+00005590: 287f 3231 312c 3833 3237 0a20 2020 2062  (.211,8327.    b
+000055a0: 6f6f 6c20 6368 6563 6b5f 785f 7370 6964  ool check_x_spid
+000055b0: 6572 287f 3232 342c 3837 3430 0a20 2020  er(.224,8740.   
+000055c0: 2062 6f6f 6c20 6368 6563 6b5f 7a5f 7370   bool check_z_sp
+000055d0: 6964 6572 287f 3233 302c 3930 3837 0a20  ider(.230,9087. 
+000055e0: 2020 2062 6f6f 6c20 6368 6563 6b5f 7a65     bool check_ze
+000055f0: 726f 5f70 6861 7365 5f73 7069 6465 7228  ro_phase_spider(
+00005600: 7f32 3336 2c39 3435 320a 2020 2020 626f  .236,9452.    bo
+00005610: 6f6c 2063 6865 636b 5f70 6175 6c69 5f73  ol check_pauli_s
+00005620: 7069 6465 7228 7f32 3437 2c39 3935 370a  pider(.247,9957.
+00005630: 2020 2020 626f 6f6c 2063 6865 636b 5f70      bool check_p
+00005640: 726f 7065 725f 636c 6966 666f 7264 5f73  roper_clifford_s
+00005650: 7069 6465 7228 7f32 3538 2c31 3035 3139  pider(.258,10519
+00005660: 0a20 2020 2062 6f6f 6c20 6368 6563 6b5f  .    bool check_
+00005670: 636c 6966 666f 7264 5f73 7069 6465 7228  clifford_spider(
+00005680: 7f32 3639 2c31 3130 3831 0a20 2020 2062  .269,11081.    b
+00005690: 6f6f 6c20 6368 6563 6b5f 6e6f 6e5f 636c  ool check_non_cl
+000056a0: 6966 666f 7264 5f73 7069 6465 7228 7f32  ifford_spider(.2
+000056b0: 3738 2c31 3134 3930 0a20 2020 2062 6f6f  78,11490.    boo
+000056c0: 6c20 6368 6563 6b5f 696e 7465 726e 616c  l check_internal
+000056d0: 5f6e 6f64 6528 7f32 3834 2c31 3138 3335  _node(.284,11835
+000056e0: 0a20 2020 2062 6f6f 6c20 6368 6563 6b5f  .    bool check_
+000056f0: 626f 756e 6461 7279 5f6e 6f64 6528 7f32  boundary_node(.2
+00005700: 3930 2c31 3231 3839 0a20 2020 2062 6f6f  90,12189.    boo
+00005710: 6c20 6368 6563 6b5f 7067 5f70 6861 7365  l check_pg_phase
+00005720: 5f6e 6f64 6528 7f32 3936 2c31 3235 3733  _node(.296,12573
+00005730: 0a20 2020 2062 6f6f 6c20 6368 6563 6b5f  .    bool check_
+00005740: 7067 5f72 6f6f 745f 6e6f 6465 287f 3330  pg_root_node(.30
+00005750: 322c 3132 3933 350a 2020 2020 626f 6f6c  2,12935.    bool
+00005760: 2063 6865 636b 5f70 675f 6c65 6166 5f6e   check_pg_leaf_n
+00005770: 6f64 6528 7f33 3038 2c31 3332 3935 0a20  ode(.308,13295. 
+00005780: 2020 2062 6f6f 6c20 6368 6563 6b5f 7068     bool check_ph
+00005790: 6173 655f 6761 6467 6574 5f6e 6f64 6528  ase_gadget_node(
+000057a0: 7f33 3134 2c31 3336 3737 0a20 2020 2062  .314,13677.    b
+000057b0: 6f6f 6c20 6368 6563 6b5f 696e 7075 745f  ool check_input_
+000057c0: 6e6f 6465 287f 3332 312c 3134 3034 370a  node(.321,14047.
+000057d0: 2020 2020 626f 6f6c 2063 6865 636b 5f6f      bool check_o
+000057e0: 7574 7075 745f 6e6f 6465 287f 3332 372c  utput_node(.327,
+000057f0: 3134 3430 320a 2020 2020 626f 6f6c 2063  14402.    bool c
+00005800: 6865 636b 5f63 6f6e 6e65 6374 5f69 6e70  heck_connect_inp
+00005810: 7574 5f6e 6f64 6528 7f33 3333 2c31 3437  ut_node(.333,147
+00005820: 3639 0a20 2020 2062 6f6f 6c20 6368 6563  69.    bool chec
+00005830: 6b5f 636f 6e6e 6563 745f 6f75 7470 7574  k_connect_output
+00005840: 5f6e 6f64 6528 7f33 3435 2c31 3532 3232  _node(.345,15222
+00005850: 0a20 2020 2062 6f6f 6c20 6368 6563 6b5f  .    bool check_
+00005860: 636f 6e6e 6563 745f 7068 6173 655f 6761  connect_phase_ga
+00005870: 6467 6574 287f 3335 372c 3135 3731 310a  dget(.357,15711.
+00005880: 2020 2020 766f 6964 2072 656d 6f76 655f      void remove_
+00005890: 6564 6765 735f 6f66 5f6e 6f64 6528 7f33  edges_of_node(.3
+000058a0: 3932 2c31 3730 3537 0a20 2020 2075 696e  92,17057.    uin
+000058b0: 7433 325f 7420 6465 6772 6565 5f6f 665f  t32_t degree_of_
+000058c0: 6e6f 6465 287f 3430 392c 3137 3536 310a  node(.409,17561.
+000058d0: 2020 2020 5a58 4e6f 6465 4b69 6e64 206b      ZXNodeKind k
+000058e0: 696e 645f 6f66 5f6e 6f64 6528 7f34 3135  ind_of_node(.415
+000058f0: 2c31 3738 3035 0a20 2020 2073 7464 3a3a  ,17805.    std::
+00005900: 7665 6374 6f72 3c7f 7374 643a 3a76 6563  vector<.std::vec
+00005910: 746f 7201 3532 322c 3232 3430 390a 2020  tor.522,22409.  
+00005920: 2020 5a58 4469 6167 7261 6d28 7f35 3333    ZXDiagram(.533
+00005930: 2c32 3237 3739 0a20 2020 205a 5844 6961  ,22779.    ZXDia
+00005940: 6772 616d 4b69 6e64 206b 696e 6428 7f35  gramKind kind(.5
+00005950: 3338 2c32 3330 3233 0a20 2020 2075 696e  38,23023.    uin
+00005960: 7433 325f 7420 7175 6269 745f 6e75 6d28  t32_t qubit_num(
+00005970: 7f35 3430 2c32 3331 3035 0a20 2020 2073  .540,23105.    s
+00005980: 7464 3a3a 7665 6374 6f72 3c5a 584e 6f64  td::vector<ZXNod
+00005990: 653e 206e 6f64 6573 287f 3534 322c 3233  e> nodes(.542,23
+000059a0: 3138 380a 2020 2020 7374 643a 3a76 6563  188.    std::vec
+000059b0: 746f 723c 7569 6e74 3332 5f74 3e20 696e  tor<uint32_t> in
+000059c0: 7075 7473 287f 3534 342c 3233 3237 350a  puts(.544,23275.
+000059d0: 2020 2020 7374 643a 3a76 6563 746f 723c      std::vector<
+000059e0: 7569 6e74 3332 5f74 3e20 6f75 7470 7574  uint32_t> output
+000059f0: 7328 7f35 3436 2c32 3333 3637 0a20 2020  s(.546,23367.   
+00005a00: 2073 7464 3a3a 7665 6374 6f72 3c73 7464   std::vector<std
+00005a10: 3a3a 7665 6374 6f72 3c5a 5845 6467 653e  ::vector<ZXEdge>
+00005a20: 3e20 6164 6a5f 6d61 7428 7f35 3438 2c32  > adj_mat(.548,2
+00005a30: 3334 3631 0a20 2020 2076 6f69 6420 6b69  3461.    void ki
+00005a40: 6e64 287f 3535 302c 3233 3536 330a 2020  nd(.550,23563.  
+00005a50: 2020 766f 6964 2071 7562 6974 5f6e 756d    void qubit_num
+00005a60: 287f 3535 322c 3233 3635 340a 2020 2020  (.552,23654.    
+00005a70: 766f 6964 206e 6f64 6573 287f 3535 342c  void nodes(.554,
+00005a80: 3233 3735 360a 2020 2020 766f 6964 2069  23756.    void i
+00005a90: 6e70 7574 7328 7f35 3536 2c32 3338 3535  nputs(.556,23855
+00005aa0: 0a20 2020 2076 6f69 6420 6f75 7470 7574  .    void output
+00005ab0: 7328 7f35 3538 2c32 3339 3631 0a20 2020  s(.558,23961.   
+00005ac0: 2076 6f69 6420 6164 6a5f 6d61 7428 7f35   void adj_mat(.5
+00005ad0: 3630 2c32 3430 3731 0a20 2020 2076 6f69  60,24071.    voi
+00005ae0: 6420 7368 6f77 287f 3537 302c 3234 3337  d show(.570,2437
+00005af0: 340a 2020 2020 7374 643a 3a6d 6170 3c7f  4.    std::map<.
+00005b00: 7374 643a 3a6d 6170 0135 3735 2c32 3435  std::map.575,245
+00005b10: 3336 0a20 2020 2075 696e 7433 325f 7420  36.    uint32_t 
+00005b20: 7370 6964 6572 5f63 6f75 6e74 287f 3538  spider_count(.58
+00005b30: 392c 3234 3933 360a 2020 2020 7569 6e74  9,24936.    uint
+00005b40: 3332 5f74 206e 6f6e 5f63 6c69 6666 6f72  32_t non_cliffor
+00005b50: 645f 636f 756e 7428 7f35 3933 2c32 3530  d_count(.593,250
+00005b60: 3838 0a20 2020 2066 7269 656e 6420 7374  88.    friend st
+00005b70: 643a 3a6f 7374 7265 616d 2620 6f70 6572  d::ostream& oper
+00005b80: 6174 6f72 3c3c 287f 3638 332c 3237 3932  ator<<(.683,2792
+00005b90: 380a 0c0a 6f70 7469 6d69 7a65 722e 682c  8...optimizer.h,
+00005ba0: 3132 3234 0a23 6465 6669 6e65 204f 5054  1224.#define OPT
+00005bb0: 494d 495a 4552 5f48 7f37 2c39 320a 2020  IMIZER_H.7,92.  
+00005bc0: 656e 756d 204f 7074 696d 697a 6572 4b69  enum OptimizerKi
+00005bd0: 6e64 207f 3139 2c32 3531 0a09 0920 2020  nd .19,251...   
+00005be0: 2020 205a 5843 616c 6375 6c75 732c 7f32     ZXCalculus,.2
+00005bf0: 302c 3237 340a 0909 2020 2020 2020 5068  0,274...      Ph
+00005c00: 6173 6550 6f6c 796e 6f6d 6961 6c20 7f32  asePolynomial .2
+00005c10: 312c 3331 370a 2020 636c 6173 7320 4f70  1,317.  class Op
+00005c20: 7469 6d69 7a65 727f 3238 2c34 3435 0a20  timizer.28,445. 
+00005c30: 2020 204f 7074 696d 697a 6572 4b69 6e64     OptimizerKind
+00005c40: 206b 696e 645f 3b7f 3331 2c34 3738 0a20   kind_;.31,478. 
+00005c50: 2020 2064 6f75 626c 6520 7072 6f63 5f74     double proc_t
+00005c60: 696d 655f 3b7f 3332 2c35 3336 0a20 2020  ime_;.32,536.   
+00005c70: 2073 7464 3a3a 6d61 703c 7f73 7464 3a3a   std::map<.std::
+00005c80: 6d61 7001 3333 2c35 3830 0a20 2020 2073  map.33,580.    s
+00005c90: 7464 3a3a 6d61 703c 7374 643a 3a73 7472  td::map<std::str
+00005ca0: 696e 672c 2075 696e 7433 325f 743e 2073  ing, uint32_t> s
+00005cb0: 7461 7473 5f69 6e5f 3b7f 3333 2c35 3830  tats_in_;.33,580
+00005cc0: 0a20 2020 2073 7464 3a3a 6d61 703c 7f73  .    std::map<.s
+00005cd0: 7464 3a3a 6d61 7001 3334 2c36 3733 0a20  td::map.34,673. 
+00005ce0: 2020 2073 7464 3a3a 6d61 703c 7374 643a     std::map<std:
+00005cf0: 3a73 7472 696e 672c 2075 696e 7433 325f  :string, uint32_
+00005d00: 743e 2073 7461 7473 5f6f 7574 5f3b 7f33  t> stats_out_;.3
+00005d10: 342c 3637 330a 2020 2020 7374 643a 3a6d  4,673.    std::m
+00005d20: 6170 3c7f 7374 643a 3a6d 6170 0133 352c  ap<.std::map.35,
+00005d30: 3736 360a 2020 2020 7374 643a 3a6d 6170  766.    std::map
+00005d40: 3c73 7464 3a3a 7374 7269 6e67 2c20 7569  <std::string, ui
+00005d50: 6e74 3332 5f74 3e20 7a78 5f73 7461 7473  nt32_t> zx_stats
+00005d60: 5f69 6e5f 3b7f 3335 2c37 3636 0a20 2020  _in_;.35,766.   
+00005d70: 2073 7464 3a3a 6d61 703c 7f73 7464 3a3a   std::map<.std::
+00005d80: 6d61 7001 3336 2c38 3637 0a20 2020 2073  map.36,867.    s
+00005d90: 7464 3a3a 6d61 703c 7374 643a 3a73 7472  td::map<std::str
+00005da0: 696e 672c 2075 696e 7433 325f 743e 207a  ing, uint32_t> z
+00005db0: 785f 7374 6174 735f 6f75 745f 3b7f 3336  x_stats_out_;.36
+00005dc0: 2c38 3637 0a20 2020 204f 7074 696d 697a  ,867.    Optimiz
+00005dd0: 6572 4b69 6e64 206b 696e 6428 7f33 392c  erKind kind(.39,
+00005de0: 3130 3036 0a20 2020 2064 6f75 626c 6520  1006.    double 
+00005df0: 7072 6f63 5f74 696d 6528 7f34 312c 3130  proc_time(.41,10
+00005e00: 3838 0a20 2020 2064 6f75 626c 6520 6765  88.    double ge
+00005e10: 745f 7072 6f63 5f74 696d 6528 7f34 332c  t_proc_time(.43,
+00005e20: 3131 3733 0a20 2020 2073 7464 3a3a 6d61  1173.    std::ma
+00005e30: 703c 7f73 7464 3a3a 6d61 7001 3435 2c31  p<.std::map.45,1
+00005e40: 3236 310a 2020 2020 7374 643a 3a6d 6170  261.    std::map
+00005e50: 3c73 7464 3a3a 7374 7269 6e67 2c20 7569  <std::string, ui
+00005e60: 6e74 3332 5f74 3e20 7374 6174 735f 696e  nt32_t> stats_in
+00005e70: 287f 3435 2c31 3236 310a 2020 2020 7374  (.45,1261.    st
+00005e80: 643a 3a6d 6170 3c7f 7374 643a 3a6d 6170  d::map<.std::map
+00005e90: 0134 372c 3133 3733 0a20 2020 2073 7464  .47,1373.    std
+00005ea0: 3a3a 6d61 703c 7374 643a 3a73 7472 696e  ::map<std::strin
+00005eb0: 672c 2075 696e 7433 325f 743e 2073 7461  g, uint32_t> sta
+00005ec0: 7473 5f6f 7574 287f 3437 2c31 3337 330a  ts_out(.47,1373.
+00005ed0: 2020 2020 7374 643a 3a6d 6170 3c7f 7374      std::map<.st
+00005ee0: 643a 3a6d 6170 0134 392c 3134 3839 0a20  d::map.49,1489. 
+00005ef0: 2020 2073 7464 3a3a 6d61 703c 7374 643a     std::map<std:
+00005f00: 3a73 7472 696e 672c 2075 696e 7433 325f  :string, uint32_
+00005f10: 743e 207a 785f 7374 6174 735f 696e 287f  t> zx_stats_in(.
+00005f20: 3439 2c31 3438 390a 2020 2020 7374 643a  49,1489.    std:
+00005f30: 3a6d 6170 3c7f 7374 643a 3a6d 6170 0135  :map<.std::map.5
+00005f40: 312c 3136 3130 0a20 2020 2073 7464 3a3a  1,1610.    std::
+00005f50: 6d61 703c 7374 643a 3a73 7472 696e 672c  map<std::string,
+00005f60: 2075 696e 7433 325f 743e 207a 785f 7374   uint32_t> zx_st
+00005f70: 6174 735f 6f75 7428 7f35 312c 3136 3130  ats_out(.51,1610
+00005f80: 0a20 2020 2076 6f69 6420 6b69 6e64 287f  .    void kind(.
+00005f90: 3533 2c31 3732 350a 2020 2020 766f 6964  53,1725.    void
+00005fa0: 2070 726f 635f 7469 6d65 287f 3535 2c31   proc_time(.55,1
+00005fb0: 3831 360a 2020 2020 766f 6964 2073 7461  816.    void sta
+00005fc0: 7473 5f69 6e28 7f35 372c 3139 3139 0a20  ts_in(.57,1919. 
+00005fd0: 2020 2076 6f69 6420 7374 6174 735f 6f75     void stats_ou
+00005fe0: 7428 7f35 392c 3230 3435 0a20 2020 2076  t(.59,2045.    v
+00005ff0: 6f69 6420 7a78 5f73 7461 7473 5f69 6e28  oid zx_stats_in(
+00006000: 7f36 312c 3231 3736 0a20 2020 2076 6f69  .61,2176.    voi
+00006010: 6420 7a78 5f73 7461 7473 5f6f 7574 287f  d zx_stats_out(.
+00006020: 3633 2c32 3331 370a 2020 2020 766f 6964  63,2317.    void
+00006030: 2073 686f 7728 7f37 372c 3237 3734 0a20   show(.77,2774. 
+00006040: 2020 2066 7269 656e 6420 7374 643a 3a6f     friend std::o
+00006050: 7374 7265 616d 2620 6f70 6572 6174 6f72  stream& operator
+00006060: 3c3c 287f 3130 352c 3430 3639 0a0c 0a64  <<(.105,4069...d
+00006070: 6167 6564 6765 2e63 7070 2c34 360a 7374  agedge.cpp,46.st
+00006080: 643a 3a73 7472 696e 6720 5368 6172 7169  d::string Sharqi
+00006090: 743a 3a44 4147 4564 6765 3a3a 6e61 6d65  t::DAGEdge::name
+000060a0: 287f 6e61 6d65 0138 2c39 320a 0c0a 6461  (.name.8,92...da
+000060b0: 676e 6f64 652e 6370 702c 3436 0a73 7464  gnode.cpp,46.std
+000060c0: 3a3a 7374 7269 6e67 2053 6861 7271 6974  ::string Sharqit
+000060d0: 3a3a 4441 474e 6f64 653a 3a6e 616d 6528  ::DAGNode::name(
+000060e0: 7f6e 616d 6501 382c 3932 0a0c 0a6f 7074  .name.8,92...opt
+000060f0: 696d 697a 6572 2e63 7070 2c33 3537 0a73  imizer.cpp,357.s
+00006100: 7464 3a3a 7374 7269 6e67 2053 6861 7271  td::string Sharq
+00006110: 6974 3a3a 4f70 7469 6d69 7a65 723a 3a74  it::Optimizer::t
+00006120: 6f5f 7374 7269 6e67 287f 746f 5f73 7472  o_string(.to_str
+00006130: 696e 6701 382c 3130 320a 7374 643a 3a73  ing.8,102.std::s
+00006140: 7472 696e 6720 5368 6172 7169 743a 3a4f  tring Sharqit::O
+00006150: 7074 696d 697a 6572 3a3a 6e61 6d65 287f  ptimizer::name(.
+00006160: 6e61 6d65 0135 312c 3234 3930 0a53 6861  name.51,2490.Sha
+00006170: 7271 6974 3a3a 5143 6972 6320 5368 6172  rqit::QCirc Shar
+00006180: 7169 743a 3a4f 7074 696d 697a 6572 3a3a  qit::Optimizer::
+00006190: 7265 6475 6365 5f67 6174 6573 5f75 7369  reduce_gates_usi
+000061a0: 6e67 5f7a 7828 7f72 6564 7563 655f 6761  ng_zx(.reduce_ga
+000061b0: 7465 735f 7573 696e 675f 7a78 0136 322c  tes_using_zx.62,
+000061c0: 3238 3235 0a53 6861 7271 6974 3a3a 5143  2825.Sharqit::QC
+000061d0: 6972 6320 5368 6172 7169 743a 3a4f 7074  irc Sharqit::Opt
+000061e0: 696d 697a 6572 3a3a 7265 6475 6365 5f67  imizer::reduce_g
+000061f0: 6174 6573 5f75 7369 6e67 5f70 7028 7f72  ates_using_pp(.r
+00006200: 6564 7563 655f 6761 7465 735f 7573 696e  educe_gates_usin
+00006210: 675f 7070 0139 302c 3334 3830 0a53 6861  g_pp.90,3480.Sha
+00006220: 7271 6974 3a3a 5143 6972 6320 5368 6172  rqit::QCirc Shar
+00006230: 7169 743a 3a4f 7074 696d 697a 6572 3a3a  qit::Optimizer::
+00006240: 7265 6475 6365 5f67 6174 6573 287f 7265  reduce_gates(.re
+00006250: 6475 6365 5f67 6174 6573 0131 3132 2c34  duce_gates.112,4
+00006260: 3032 350a 0c0a 7167 6174 652e 682c 3135  025...qgate.h,15
+00006270: 3130 0a23 6465 6669 6e65 2051 4741 5445  10.#define QGATE
+00006280: 5f48 7f37 2c38 300a 2020 656e 756d 2051  _H.7,80.  enum Q
+00006290: 4761 7465 4b69 6e64 207f 3139 2c32 3431  GateKind .19,241
+000062a0: 0a09 0920 2058 2c7f 3230 2c32 3630 0a09  ...  X,.20,260..
+000062b0: 0920 205a 2c7f 3231 2c32 3835 0a09 0920  .  Z,.21,285... 
+000062c0: 2053 2c7f 3232 2c33 3130 0a09 0920 2053   S,.22,310...  S
+000062d0: 6467 2c7f 3233 2c33 3239 0a09 0920 2054  dg,.23,329...  T
+000062e0: 2c7f 3234 2c33 3834 0a09 0920 2054 6467  ,.24,384...  Tdg
+000062f0: 2c7f 3235 2c34 3033 0a09 0920 2048 2c7f  ,.25,403...  H,.
+00006300: 3236 2c34 3538 0a09 0920 2052 5a2c 7f32  26,458...  RZ,.2
+00006310: 372c 3438 380a 0909 2020 4358 2c7f 3238  7,488...  CX,.28
+00006320: 2c35 3039 0a09 0920 2043 5a2c 7f32 392c  ,509...  CZ,.29,
+00006330: 3533 320a 0909 2020 4343 582c 7f33 302c  532...  CCX,.30,
+00006340: 3535 330a 0909 2020 4343 5a2c 7f33 312c  553...  CCZ,.31,
+00006350: 3537 360a 0909 2020 4964 2c7f 3332 2c35  576...  Id,.32,5
+00006360: 3939 0a09 0920 2049 6432 2c7f 3333 2c36  99...  Id2,.33,6
+00006370: 3339 0a20 2063 6c61 7373 2051 4761 7465  39.  class QGate
+00006380: 7f34 302c 3733 370a 2020 2020 5147 6174  .40,737.    QGat
+00006390: 654b 696e 6420 6b69 6e64 5f3b 7f34 332c  eKind kind_;.43,
+000063a0: 3736 360a 2020 2020 7374 643a 3a76 6563  766.    std::vec
+000063b0: 746f 723c 7569 6e74 3332 5f74 3e20 7169  tor<uint32_t> qi
+000063c0: 645f 3b7f 3434 2c38 3133 0a20 2020 2050  d_;.44,813.    P
+000063d0: 6861 7365 2070 6861 7365 5f3b 7f34 352c  hase phase_;.45,
+000063e0: 3837 340a 2020 2020 7374 643a 3a76 6563  874.    std::vec
+000063f0: 746f 723c 7374 643a 3a76 6563 746f 723c  tor<std::vector<
+00006400: 7374 643a 3a63 6f6d 706c 6578 3c64 6f75  std::complex<dou
+00006410: 626c 653e 3e3e 206f 705f 3b7f 3436 2c39  ble>>> op_;.46,9
+00006420: 3230 0a20 2020 2051 4761 7465 287f 3732  20.    QGate(.72
+00006430: 2c32 3035 380a 2020 2020 5147 6174 654b  ,2058.    QGateK
+00006440: 696e 6420 6b69 6e64 287f 3734 2c32 3139  ind kind(.74,219
+00006450: 360a 2020 2020 7374 643a 3a76 6563 746f  6.    std::vecto
+00006460: 723c 7569 6e74 3332 5f74 3e20 7169 6428  r<uint32_t> qid(
+00006470: 7f37 362c 3232 3638 0a20 2020 2050 6861  .76,2268.    Pha
+00006480: 7365 2070 6861 7365 287f 3738 2c32 3335  se phase(.78,235
+00006490: 320a 2020 2020 5068 6173 6520 6765 745f  2.    Phase get_
+000064a0: 7068 6173 6528 7f38 302c 3234 3234 0a20  phase(.80,2424. 
+000064b0: 2020 2073 7464 3a3a 7665 6374 6f72 3c73     std::vector<s
+000064c0: 7464 3a3a 7665 6374 6f72 3c73 7464 3a3a  td::vector<std::
+000064d0: 636f 6d70 6c65 783c 646f 7562 6c65 3e3e  complex<double>>
+000064e0: 3e20 6f70 287f 3832 2c32 3439 370a 2020  > op(.82,2497.  
+000064f0: 2020 766f 6964 206b 696e 6428 7f38 342c    void kind(.84,
+00006500: 3236 3033 0a20 2020 2076 6f69 6420 7169  2603.    void qi
+00006510: 6428 7f38 362c 3236 3834 0a20 2020 2076  d(.86,2684.    v
+00006520: 6f69 6420 7068 6173 6528 7f38 382c 3237  oid phase(.88,27
+00006530: 3736 0a20 2020 2076 6f69 6420 6f70 287f  76.    void op(.
+00006540: 3930 2c32 3835 370a 2020 2020 7569 6e74  90,2857.    uint
+00006550: 3332 5f74 2071 7562 6974 5f6e 756d 287f  32_t qubit_num(.
+00006560: 3130 372c 3334 3836 0a20 2020 2062 6f6f  107,3486.    boo
+00006570: 6c20 6973 5f49 645f 6761 7465 287f 3131  l is_Id_gate(.11
+00006580: 322c 3336 3830 0a20 2020 2062 6f6f 6c20  2,3680.    bool 
+00006590: 6973 5f49 6432 5f67 6174 6528 7f31 3137  is_Id2_gate(.117
+000065a0: 2c33 3837 380a 2020 2020 626f 6f6c 2069  ,3878.    bool i
+000065b0: 735f 585f 6761 7465 287f 3132 322c 3430  s_X_gate(.122,40
+000065c0: 3535 0a20 2020 2062 6f6f 6c20 6973 5f5a  55.    bool is_Z
+000065d0: 5f67 6174 6528 7f31 3237 2c34 3235 350a  _gate(.127,4255.
+000065e0: 2020 2020 626f 6f6c 2069 735f 485f 6761      bool is_H_ga
+000065f0: 7465 287f 3133 372c 3435 3433 0a20 2020  te(.137,4543.   
+00006600: 2062 6f6f 6c20 6973 5f53 5f67 6174 6528   bool is_S_gate(
+00006610: 7f31 3432 2c34 3735 300a 2020 2020 626f  .142,4750.    bo
+00006620: 6f6c 2069 735f 5331 5f67 6174 6528 7f31  ol is_S1_gate(.1
+00006630: 3535 2c35 3134 370a 2020 2020 626f 6f6c  55,5147.    bool
+00006640: 2069 735f 5333 5f67 6174 6528 7f31 3636   is_S3_gate(.166
+00006650: 2c35 3438 300a 2020 2020 626f 6f6c 2069  ,5480.    bool i
+00006660: 735f 545f 6761 7465 287f 3137 372c 3538  s_T_gate(.177,58
+00006670: 3238 0a20 2020 2062 6f6f 6c20 6973 5f54  28.    bool is_T
+00006680: 315f 6761 7465 287f 3139 302c 3632 3235  1_gate(.190,6225
+00006690: 0a20 2020 2062 6f6f 6c20 6973 5f54 375f  .    bool is_T7_
+000066a0: 6761 7465 287f 3230 332c 3635 3735 0a20  gate(.203,6575. 
+000066b0: 2020 2062 6f6f 6c20 6973 5f43 585f 6761     bool is_CX_ga
+000066c0: 7465 287f 3231 362c 3639 3033 0a20 2020  te(.216,6903.   
+000066d0: 2062 6f6f 6c20 6973 5f43 5a5f 6761 7465   bool is_CZ_gate
+000066e0: 287f 3232 312c 3730 3638 0a20 2020 2062  (.221,7068.    b
+000066f0: 6f6f 6c20 6973 5f43 4358 5f67 6174 6528  ool is_CCX_gate(
+00006700: 7f32 3236 2c37 3233 350a 2020 2020 626f  .226,7235.    bo
+00006710: 6f6c 2069 735f 4343 5a5f 6761 7465 287f  ol is_CCZ_gate(.
+00006720: 3233 312c 3734 3034 0a20 2020 2062 6f6f  231,7404.    boo
+00006730: 6c20 6973 5f52 5a5f 6761 7465 287f 3233  l is_RZ_gate(.23
+00006740: 362c 3735 3731 0a20 2020 2062 6f6f 6c20  6,7571.    bool 
+00006750: 6973 5f70 6175 6c69 5f67 6174 6528 7f32  is_pauli_gate(.2
+00006760: 3433 2c37 3931 370a 2020 2020 626f 6f6c  43,7917.    bool
+00006770: 2069 735f 7072 6f70 6572 5f63 6c69 6666   is_proper_cliff
+00006780: 6f72 645f 6761 7465 287f 3234 382c 3831  ord_gate(.248,81
+00006790: 3331 0a20 2020 2062 6f6f 6c20 6973 5f63  31.    bool is_c
+000067a0: 6c69 6666 6f72 645f 6761 7465 287f 3235  lifford_gate(.25
+000067b0: 332c 3833 3038 0a20 2020 2062 6f6f 6c20  3,8308.    bool 
+000067c0: 6973 5f6e 6f6e 5f63 6c69 6666 6f72 645f  is_non_clifford_
+000067d0: 6761 7465 287f 3235 382c 3835 3337 0a20  gate(.258,8537. 
+000067e0: 2020 2062 6f6f 6c20 6973 5f69 6e63 6c75     bool is_inclu
+000067f0: 6465 6428 7f32 3634 2c38 3736 320a 2020  ded(.264,8762.  
+00006800: 2020 7374 6174 6963 2073 7464 3a3a 7475    static std::tu
+00006810: 706c 653c 7f73 7464 3a3a 7475 706c 6501  ple<.std::tuple.
+00006820: 3330 382c 3130 3238 320a 2020 2020 6672  308,10282.    fr
+00006830: 6965 6e64 2073 7464 3a3a 6f73 7472 6561  iend std::ostrea
+00006840: 6d26 206f 7065 7261 746f 723c 3c28 7f33  m& operator<<(.3
+00006850: 3039 2c31 3033 3538 0a0c 0a66 7261 6374  09,10358...fract
+00006860: 696f 6e2e 6370 702c 3537 0a73 7464 3a3a  ion.cpp,57.std::
+00006870: 7374 7269 6e67 2053 6861 7271 6974 3a3a  string Sharqit::
+00006880: 4672 6163 7469 6f6e 3a3a 746f 5f73 7472  Fraction::to_str
+00006890: 696e 6728 7f74 6f5f 7374 7269 6e67 0138  ing(.to_string.8
+000068a0: 2c39 390a                                ,99.
```

### Comparing `sharqit-0.2.1/sharqit/cpp/binary_matrix.cpp` & `sharqit-0.2.2/sharqit/cpp/binary_matrix.cpp`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.1/sharqit/cpp/binary_matrix.h` & `sharqit-0.2.2/sharqit/cpp/binary_matrix.h`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.1/sharqit/cpp/dag.h` & `sharqit-0.2.2/sharqit/cpp/dag.h`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.1/sharqit/cpp/dagcirc.cpp` & `sharqit-0.2.2/sharqit/cpp/dagcirc.cpp`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.1/sharqit/cpp/extract_qcirc.cpp` & `sharqit-0.2.2/sharqit/cpp/extract_qcirc.cpp`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.1/sharqit/cpp/fraction.h` & `sharqit-0.2.2/sharqit/cpp/fraction.h`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.1/sharqit/cpp/linear_map.cpp` & `sharqit-0.2.2/sharqit/cpp/linear_map.cpp`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.1/sharqit/cpp/linear_map.h` & `sharqit-0.2.2/sharqit/cpp/linear_map.h`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.1/sharqit/cpp/merge_rotation.cpp` & `sharqit-0.2.2/sharqit/cpp/merge_rotation.cpp`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.1/sharqit/cpp/optimizer.cpp` & `sharqit-0.2.2/sharqit/cpp/optimizer.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -96,27 +96,30 @@
   dc.rule_based_gate_reduction();
   qc_out = dc.to_qcirc();
 
   /* T-count,2Q-count reduction using phase polynomials */
   qc_out.replace_with_rz();
   qc_out.merge_rotation();
   qc_out.propagate_pauli_x();
-    
+
   /* rule-based gate reduction */
   dc = qc_out.to_dagcirc();
   dc.rule_based_gate_reduction();
   qc_out = dc.to_qcirc();
 
   return qc_out;
 }
 
-Sharqit::QCirc Sharqit::Optimizer::reduce_gates(const Sharqit::QCirc& qc_in, const std::string& method)
+Sharqit::QCirc Sharqit::Optimizer::reduce_gates(const Sharqit::QCirc& qc, const std::string& method)
 {
   auto start = std::chrono::system_clock::now();
 
+  /* decompose CCX or CCZ */
+  Sharqit::QCirc qc_in = qc;
+  
   /* kind of optimizer */
   if (method == "zx") {
     kind_ = Sharqit::OptimizerKind::ZXCalculus;
   }
   else if (method == "pp") {
     kind_ = Sharqit::OptimizerKind::PhasePolynomial;
   }
@@ -145,20 +148,7 @@
   auto end = std::chrono::system_clock::now();
   auto dur = end - start;
   auto msec = std::chrono::duration_cast<std::chrono::milliseconds>(dur).count();
   proc_time_ = msec / 1000.;
 
   return qc_out;
 }
-
-Sharqit::QCirc Sharqit::Optimizer::execute(const Sharqit::QCirc& qc_in, const OptimizerKind kind)
-{
-  if (kind == Sharqit::OptimizerKind::ZXCalculus) {
-    return reduce_gates(qc_in, "zx");
-  }
-  else if (kind == Sharqit::OptimizerKind::PhasePolynomial) {
-    return reduce_gates(qc_in, "pp");
-  }
-  else {
-    throw std::runtime_error("Invalid kind of optimizer.");
-  }
-}
```

### Comparing `sharqit-0.2.1/sharqit/cpp/optimizer.h` & `sharqit-0.2.2/sharqit/cpp/optimizer.h`

 * *Files 7% similar despite different names*

```diff
@@ -89,21 +89,13 @@
     QCirc reduce_gates_using_pp(const QCirc& qc_in);
     /**
      * @brief execute the quantum circuit optimization (reduction of gate-count)
      * @param [in] qc_in input quantum circuit
      * @param [in] method optimization method ("zx" or "pp")
      * @return output quantum circuit
      */
-    QCirc reduce_gates(const QCirc& qc_in, const std::string& method);
-    /**
-     * @brief execute the quantum circuit optimization
-     * @param [in] qc_in input quantum circuit
-     * @param [in] kind optimization method
-     * @return output quantum circuit
-     * @note This method will be removed in near future. You should use reduce_gates method instead.
-     */
-    QCirc execute(const QCirc& qc_in, const OptimizerKind kind = OptimizerKind::ZXCalculus);
+    QCirc reduce_gates(const QCirc& qc, const std::string& method);
     friend std::ostream& operator<<(std::ostream& ost, const Optimizer& opt) { ost << opt.to_string(); return ost; }
    };
 }
 
 #endif
```

### Comparing `sharqit-0.2.1/sharqit/cpp/phase.cpp` & `sharqit-0.2.2/sharqit/cpp/phase.cpp`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.1/sharqit/cpp/phase.h` & `sharqit-0.2.2/sharqit/cpp/phase.h`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.1/sharqit/cpp/propagate_pauli_x.cpp` & `sharqit-0.2.2/sharqit/cpp/propagate_pauli_x.cpp`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.1/sharqit/cpp/qcirc.h` & `sharqit-0.2.2/sharqit/cpp/qcirc.h`

 * *Files 3% similar despite different names*

```diff
@@ -153,14 +153,29 @@
     uint32_t cz_count() const;
     /**
      * @brief get a number of two-qubit gates in the quantum circuit
      * @return number of two-qubit gates
      */
     uint32_t twoq_count() const { return (cx_count() + cz_count()); }
     /**
+     * @brief get a number of CCX gates in the quantum circuit
+     * @return number of CCX gates
+     */
+    uint32_t ccx_count() const;
+    /**
+     * @brief get a number of CCZ gates in the quantum circuit
+     * @return number of CCZ gates
+     */
+    uint32_t ccz_count() const;
+    /**
+     * @brief get a number of toffoli gates (CCX and CCZ gates) in the quantum circuit
+     * @return number of two-qubit gates
+     */
+    uint32_t tof_count() const { return (ccx_count() + ccz_count()); }
+    /**
      * @brief get a depth of the quantum circuit
      * @return depth of the quantum circuit
      */
     uint32_t depth() const;
     /**
      * @brief get a circuit diagram as ascii text of the quantum circuit
      * @return circuit diagram as ascii text
@@ -309,14 +324,24 @@
      */
     void propagate_pauli_x();
     /**
      * @brief all CZ gates are converted to CX gates
      */
     void cz_to_cx();
     /**
+     * @brief decompose all Toffoli gates (CCX and CCZ gates) to basic gats
+     * @return QCirc object after decomposing
+     */
+    void decomp_tof();
+    /**
+     * @brief whether any Toffoli gates (CCX or CCZ gates) are included or not
+     * @return QCirc object after decomposing
+     */
+    bool include_tof() const;
+    /**
      * @brief add an identity gate to the quantum circuit
      * @return reference of the QCirc after adding the quantum gate
      */
     QCirc& id(const uint32_t q) { return add_qgate(QGateKind::Id, {q}); }
     /**
      * @brief add a pauli-X gate to the quantum circuit
      * @param [in] q qubit id to be applied
@@ -350,15 +375,15 @@
     /**
      * @brief add a T+ (hermitian conjugate of T) gate to the quantum circuit
      * @param [in] q qubit id to be applied
      * @return reference of the QCirc after adding the quantum gate
      */
     QCirc& tdg(const uint32_t q) { return add_qgate(QGateKind::Tdg, {q}); }
     /**
-     * @brief add a H (hadamard) gate to the quantum circuit
+     * @brief add an H (hadamard) gate to the quantum circuit
      * @param [in] q qubit id to be applied
      * @return reference of the QCirc after adding the quantum gate
      */
     QCirc& h(const uint32_t q) { return add_qgate(QGateKind::H, {q}); }
     /**
      * @brief add a RZ gate to the quantum circuit
      * @param [in] q qubit id to be applied
@@ -391,14 +416,30 @@
      * @brief add a RX gate to the quantum circuit
      * @param [in] q qubit id to be applied
      * @param [in] phase phase of the rotation
      * @return reference of the QCirc after adding the quantum gate
      */
     QCirc& rx(const uint32_t q, const Phase& phase) { h(q); rz(q,phase); h(q); return *this; }
     /**
+     * @brief add a CCX gate to the quantum circuit
+     * @param [in] c0 qubit id (control) to be applied
+     * @param [in] c1 qubit id (control) to be applied
+     * @param [in] tar qubit id (target) to be applied
+     * @return reference of the QCirc after adding the quantum gate
+     */
+    QCirc& ccx(const uint32_t c0, const uint32_t c1, const uint32_t tar) { return add_qgate(QGateKind::CCX, {c0, c1, tar}); }
+    /**
+     * @brief add a CCZ gate to the quantum circuit
+     * @param [in] c0 qubit id (control) to be applied
+     * @param [in] c1 qubit id (control) to be applied
+     * @param [in] tar qubit id (target) to be applied
+     * @return reference of the QCirc after adding the quantum gate
+     */
+    QCirc& ccz(const uint32_t c0, const uint32_t c1, const uint32_t tar) { return add_qgate(QGateKind::CCZ, {c0, c1, tar}); }
+    /**
      * @brief add a pauli-Y gate to the quantum circuit
      * @param [in] q qubit id to be applied
      * @return reference of the QCirc after adding the quantum gate
      */
     QCirc& y(const uint32_t q) { x(q); z(q); return *this; }
     /**
      * @brief add a sqrt-X (squre root of pauli-X) gate to the quantum circuit
@@ -581,16 +622,35 @@
     /**
      * @brief add a controlled cnot (toffoli) gate to the quantum circuit
      * @param [in] c0 qubit id (control) to be applied
      * @param [in] c1 qubit id (control) to be applied
      * @param [in] tar qubit id to be applied
      * @return reference of the QCirc after adding the quantum gate
      */
-    QCirc& ccx(const uint32_t c0, const uint32_t c1, const uint32_t tar) // Toffoli gate
-    { csx(c1,tar); cx(c0,c1); csxdg(c1,tar); cx(c0,c1); csx(c0,tar); return *this; }
+    QCirc& ccx_decomp(const uint32_t c0, const uint32_t c1, const uint32_t tar)
+    {
+      h(tar);
+      cx(c1,tar); tdg(tar); cx(c0,tar); t(tar); cx(c1,tar); tdg(tar);
+      cx(c0,tar); cx(c0,c1); tdg(c1); cx(c0,c1); t(c0); t(c1); t(tar);
+      h(tar);
+      return *this;
+    }
+    /**
+     * @brief add a controlled CZ gate to the quantum circuit
+     * @param [in] c0 qubit id (control) to be applied
+     * @param [in] c1 qubit id (control) to be applied
+     * @param [in] tar qubit id to be applied
+     * @return reference of the QCirc after adding the quantum gate
+     */
+    QCirc& ccz_decomp(const uint32_t c0, const uint32_t c1, const uint32_t tar)
+    {
+      cx(c1,tar); tdg(tar); cx(c0,tar); t(tar); cx(c1,tar); tdg(tar);
+      cx(c0,tar); cx(c0,c1); tdg(c1); cx(c0,c1); t(c0); t(c1); t(tar);
+      return *this;
+    }
     QCirc& operator+=(const QCirc& rhs) { return add_qcirc(rhs); }
     friend QCirc operator+(const QCirc& lhs, const QCirc& rhs) { QCirc qc = lhs; return qc.add_qcirc(rhs); }
     friend std::ostream& operator<<(std::ostream& ost, const QCirc& qc) { ost << qc.to_string(); return ost; }
   };
 }
 
 #endif
```

### Comparing `sharqit-0.2.1/sharqit/cpp/qgate.cpp` & `sharqit-0.2.2/sharqit/cpp/qgate.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  * @file qgate.cpp
  * @brief member functions of QGate class
  */
 
 #include "qgate.h"
 
 Sharqit::QGate::QGate(const Sharqit::QGateKind kind, const std::vector<uint32_t>& qid,
-		    const Sharqit::Phase& phase)
+		      const Sharqit::Phase& phase)
 {
   Sharqit::Phase p = phase;
   p.mod_2pi();
   
   switch (kind) {
   case Sharqit::QGateKind::Id:
   case Sharqit::QGateKind::X:
@@ -38,14 +38,23 @@
     if (qid.size() != 2) {
       throw std::runtime_error("related qubit number must be 2.");
     }
     if (p.is_zero() == false) {
       throw std::runtime_error("phase parameter must be zero.");
     }
     break;
+  case Sharqit::QGateKind::CCX:
+  case Sharqit::QGateKind::CCZ:
+    if (qid.size() != 3) {
+      throw std::runtime_error("related qubit number must be 3.");
+    }
+    if (p.is_zero() == false) {
+      throw std::runtime_error("phase parameter must be zero.");
+    }
+    break;
   default:
     throw std::runtime_error("unknown QGateKind.");
   }
 
   kind_ = kind;
   qid_ = qid;
   phase_ = p;
@@ -126,23 +135,43 @@
     break;
   case Sharqit::QGateKind::CZ:
     op = {{1.0, 0.0, 0.0, 0.0},
 	  {0.0, 1.0, 0.0, 0.0},
 	  {0.0, 0.0, 1.0, 0.0},
 	  {0.0, 0.0, 0.0, -1.0}};
     break;
+  case Sharqit::QGateKind::CCX:
+    op = {{1.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0},
+	  {0.0, 1.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0},
+	  {0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 0.0, 0.0},
+	  {0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 0.0},
+	  {0.0, 0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0},
+	  {0.0, 0.0, 0.0, 0.0, 0.0, 1.0, 0.0, 0.0},
+	  {0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 1.0},
+	  {0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 1.0, 0.0}};
+    break;
+  case Sharqit::QGateKind::CCZ:
+    op = {{1.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0,  0.0},
+	  {0.0, 1.0, 0.0, 0.0, 0.0, 0.0, 0.0,  0.0},
+	  {0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 0.0,  0.0},
+	  {0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0,  0.0},
+	  {0.0, 0.0, 0.0, 0.0, 1.0, 0.0, 0.0,  0.0},
+	  {0.0, 0.0, 0.0, 0.0, 0.0, 1.0, 0.0,  0.0},
+	  {0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 1.0,  0.0},
+	  {0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, -1.0}};
+    break;
   default:
     throw std::runtime_error("unknown QGateKind.");
   }
   return op;
 }
 
 std::string Sharqit::QGate::name(bool pi_str) const
 {
-  std::vector<std::string> s = { "X", "Z", "S", "S+", "T", "T+", "H", "RZ", "CX", "CZ", "I", "I2" };
+  std::vector<std::string> s = { "X", "Z", "S", "S+", "T", "T+", "H", "RZ", "CX", "CZ", "CCX", "CCZ", "I", "I2" };
   Phase p = phase_;
   std::string p_str = "";
   if (kind_ == QGateKind::RZ) p_str = "(" + p.to_string(pi_str) + ")";
   return s[kind_] + p_str;
 }
 
 std::string Sharqit::QGate::to_string(bool pi_str) const
@@ -217,14 +246,22 @@
     kind = Sharqit::QGateKind::CX;
     phase = Sharqit::Phase(0);
   }
   else if (str == "CZ") {
     kind = Sharqit::QGateKind::CZ;
     phase = Sharqit::Phase(0);
   }
+  else if (str == "CCX") {
+    kind = Sharqit::QGateKind::CCX;
+    phase = Sharqit::Phase(0);
+  }
+  else if (str == "CCZ") {
+    kind = Sharqit::QGateKind::CCZ;
+    phase = Sharqit::Phase(0);
+  }
   else if (str.find("RZ") == 0) {
     phase = Sharqit::Phase(str.substr(3, str.size() - 4));
     phase.mod_2pi();
     if (str.find("RZ") == 0) kind = Sharqit::QGateKind::RZ;
   }
   else {
     throw std::runtime_error(str+" is not supported.");
@@ -294,28 +331,40 @@
     qgate_inv.op(kind_to_op(Sharqit::QGateKind::CX));
     break;
   case Sharqit::QGateKind::CZ:
     qgate_inv.kind(Sharqit::QGateKind::CZ);
     qgate_inv.qid(qid_);
     qgate_inv.op(kind_to_op(Sharqit::QGateKind::CZ));
     break;
+  case Sharqit::QGateKind::CCX:
+    qgate_inv.kind(Sharqit::QGateKind::CCX);
+    qgate_inv.qid(qid_);
+    qgate_inv.op(kind_to_op(Sharqit::QGateKind::CCX));
+    break;
+  case Sharqit::QGateKind::CCZ:
+    qgate_inv.kind(Sharqit::QGateKind::CCZ);
+    qgate_inv.qid(qid_);
+    qgate_inv.op(kind_to_op(Sharqit::QGateKind::CCZ));
+    break;
   default:
     throw std::runtime_error("unknown QGateKind.");
   }
   return qgate_inv;
 }
 
 bool Sharqit::QGate::is_identical(QGate& other) const
 {
   if (kind_ != other.kind()) return false;
   if (qid_.size() != other.qid().size()) return false;
   if (qid_.size() == 1 && qid_[0] != other.qid()[0]) return false;
   if (qid_.size() == 2 &&
       (qid_[0] != other.qid()[0] || qid_[1] != other.qid()[1])) return false;
-  if (qid_.size() > 2) return false;
+  if (qid_.size() == 3 &&
+      (qid_[0] != other.qid()[0] || qid_[1] != other.qid()[1] || qid_[2] != other.qid()[2])) return false;
+  if (qid_.size() > 3) return false;
   if (phase_ != other.phase()) return false;
 
   return true;
 }
 
 bool Sharqit::QGate::overlap(const Sharqit::QGate& other) const
 {
```

### Comparing `sharqit-0.2.1/sharqit/cpp/qgate.h` & `sharqit-0.2.2/sharqit/cpp/qgate.h`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,18 @@
 		  Sdg, //!< S+ gate (hermitian conjugagte of S gate)
 		  T, //!< T gate
 		  Tdg, //!< T+ gate (hermitian conjugagte of T gate)
 		  H, //!< H (hadamard) gate
 		  RZ, //!< RZ gate
 		  CX, //!< CNOT gate
 		  CZ, //!< CZ gate
+		  CCX, //!< CCX gate
+		  CCZ, //!< CCZ gate
 		  Id, //!< single-qubit identity gate
-		  Id2 //!< two-qubit identity gate
+		  Id2, //!< two-qubit identity gate
   };
 
   /**
    * @class QGate
    * @brief quantum gate
   */
   class QGate
@@ -214,14 +216,24 @@
     bool is_CX_gate() const { return (kind_ == QGateKind::CX); }
     /**
      * @brief CZ gate or not
      * @return true if it's a CZ gate, false otherwise
      */
     bool is_CZ_gate() const { return (kind_ == QGateKind::CZ); }
     /**
+     * @brief CCX gate or not
+     * @return true if it's a CCX gate, false otherwise
+     */
+    bool is_CCX_gate() const { return (kind_ == QGateKind::CCX); }
+    /**
+     * @brief CCZ gate or not
+     * @return true if it's a CCZ gate, false otherwise
+     */
+    bool is_CCZ_gate() const { return (kind_ == QGateKind::CCZ); }
+    /**
      * @brief RZ gate or not
      * @return true if it's a RZ gate, false otherwise
      */
     bool is_RZ_gate() const { return (kind_ == QGateKind::Z || kind_ == QGateKind::S || kind_ == QGateKind::Sdg ||
 				      kind_ == QGateKind::T || kind_ == QGateKind::Tdg || kind_ == QGateKind::RZ ||
 				      kind_ == QGateKind::Id); }
     /**
@@ -268,27 +280,27 @@
     /**
      * @brief overlap or not
      * @param [in] other quantum gate
      * @return true if the quantum gate is overlap to the other, false otherwise
      */
     bool overlap(const Sharqit::QGate& other) const;
     /**
-     * @brief mergeable or not
+     * @brief mergeable or not (for single or two qubit gate)
      * @param [in] other quantum gate
      * @return true if the quantum gate is mergeable to the other, false otherwise
      */
     bool mergeable(const QGate& other) const;
     /**
-     * @brief commutable or not
+     * @brief commutable or not (for single or two qubit gate)
      * @param [in] other quantum gate
      * @return true if the quantum gate is commutable to the other, false otherwise
      */
     bool commutable(const QGate& other) const;
     /**
-     * @brief merge to the other quantum gate
+     * @brief merge to the other quantum gate (for single or two qubit gate)
      * @param [in] other quantum gate
      */
     void merge(const QGate& other);
     /**
      * @brief get a kind and phase from the quantum gate string
      * @param [in] str quantum gate string
      * @return tuple of the kind and the phase
```

### Comparing `sharqit-0.2.1/sharqit/cpp/sharqit.cpp` & `sharqit-0.2.2/sharqit/cpp/sharqit.cpp`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.1/sharqit/cpp/simplify.cpp` & `sharqit-0.2.2/sharqit/cpp/simplify.cpp`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.1/sharqit/cpp/util.h` & `sharqit-0.2.2/sharqit/cpp/util.h`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.1/sharqit/cpp/zx.h` & `sharqit-0.2.2/sharqit/cpp/zx.h`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.1/sharqit/cpp/zxdiagram.cpp` & `sharqit-0.2.2/sharqit/cpp/zxdiagram.cpp`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.1/sharqit/cpp/zxnode.cpp` & `sharqit-0.2.2/sharqit/cpp/zxnode.cpp`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.1/sharqit.egg-info/SOURCES.txt` & `sharqit-0.2.2/sharqit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

