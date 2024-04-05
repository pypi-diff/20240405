# Comparing `tmp/pytorch-cuda-0.0.1.tar.gz` & `tmp/pytorch-cuda-12.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-cuda-0.0.1.tar", last modified: Fri Apr  5 16:48:49 2024, max compression
+gzip compressed data, was "pytorch-cuda-12.1.tar", last modified: Fri Apr  5 16:49:23 2024, max compression
```

## Comparing `pytorch-cuda-0.0.1.tar` & `pytorch-cuda-12.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-04-05 16:48:49.492622 pytorch-cuda-0.0.1/
--rw-r--r--   0 kotko      (501) staff       (20)     1081 2021-02-11 13:14:03.000000 pytorch-cuda-0.0.1/LICENSE.txt
--rw-r--r--   0 kotko      (501) staff       (20)      194 2021-02-11 13:14:03.000000 pytorch-cuda-0.0.1/MANIFEST.in
--rw-r--r--   0 kotko      (501) staff       (20)      441 2024-04-05 16:48:49.492432 pytorch-cuda-0.0.1/PKG-INFO
--rw-r--r--   0 kotko      (501) staff       (20)       15 2023-05-10 17:51:27.000000 pytorch-cuda-0.0.1/README.md
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-04-05 16:48:49.490073 pytorch-cuda-0.0.1/data/
--rw-r--r--   0 kotko      (501) staff       (20)        9 2021-02-11 13:14:03.000000 pytorch-cuda-0.0.1/data/data_file
--rw-r--r--   0 kotko      (501) staff       (20)      253 2021-02-11 16:09:08.000000 pytorch-cuda-0.0.1/pyproject.toml
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-04-05 16:48:49.492059 pytorch-cuda-0.0.1/pytorch_cuda.egg-info/
--rw-r--r--   0 kotko      (501) staff       (20)      441 2024-04-05 16:48:49.000000 pytorch-cuda-0.0.1/pytorch_cuda.egg-info/PKG-INFO
--rw-r--r--   0 kotko      (501) staff       (20)      300 2024-04-05 16:48:49.000000 pytorch-cuda-0.0.1/pytorch_cuda.egg-info/SOURCES.txt
--rw-r--r--   0 kotko      (501) staff       (20)        1 2024-04-05 16:48:49.000000 pytorch-cuda-0.0.1/pytorch_cuda.egg-info/dependency_links.txt
--rw-r--r--   0 kotko      (501) staff       (20)        9 2024-04-05 16:48:49.000000 pytorch-cuda-0.0.1/pytorch_cuda.egg-info/requires.txt
--rw-r--r--   0 kotko      (501) staff       (20)        6 2024-04-05 16:48:49.000000 pytorch-cuda-0.0.1/pytorch_cuda.egg-info/top_level.txt
--rw-r--r--   0 kotko      (501) staff       (20)       78 2024-04-05 16:48:49.492959 pytorch-cuda-0.0.1/setup.cfg
--rw-r--r--   0 kotko      (501) staff       (20)      695 2024-04-05 16:48:42.000000 pytorch-cuda-0.0.1/setup.py
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-04-05 16:48:49.491625 pytorch-cuda-0.0.1/tests/
--rw-r--r--   0 kotko      (501) staff       (20)      208 2021-02-11 13:14:03.000000 pytorch-cuda-0.0.1/tests/__init__.py
--rw-r--r--   0 kotko      (501) staff       (20)      417 2021-02-11 13:14:03.000000 pytorch-cuda-0.0.1/tests/test_simple.py
+drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-04-05 16:49:23.125857 pytorch-cuda-12.1/
+-rw-r--r--   0 kotko      (501) staff       (20)     1081 2021-02-11 13:14:03.000000 pytorch-cuda-12.1/LICENSE.txt
+-rw-r--r--   0 kotko      (501) staff       (20)      194 2021-02-11 13:14:03.000000 pytorch-cuda-12.1/MANIFEST.in
+-rw-r--r--   0 kotko      (501) staff       (20)      440 2024-04-05 16:49:23.125759 pytorch-cuda-12.1/PKG-INFO
+-rw-r--r--   0 kotko      (501) staff       (20)       15 2023-05-10 17:51:27.000000 pytorch-cuda-12.1/README.md
+drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-04-05 16:49:23.123959 pytorch-cuda-12.1/data/
+-rw-r--r--   0 kotko      (501) staff       (20)        9 2021-02-11 13:14:03.000000 pytorch-cuda-12.1/data/data_file
+-rw-r--r--   0 kotko      (501) staff       (20)      253 2021-02-11 16:09:08.000000 pytorch-cuda-12.1/pyproject.toml
+drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-04-05 16:49:23.125517 pytorch-cuda-12.1/pytorch_cuda.egg-info/
+-rw-r--r--   0 kotko      (501) staff       (20)      440 2024-04-05 16:49:23.000000 pytorch-cuda-12.1/pytorch_cuda.egg-info/PKG-INFO
+-rw-r--r--   0 kotko      (501) staff       (20)      300 2024-04-05 16:49:23.000000 pytorch-cuda-12.1/pytorch_cuda.egg-info/SOURCES.txt
+-rw-r--r--   0 kotko      (501) staff       (20)        1 2024-04-05 16:49:23.000000 pytorch-cuda-12.1/pytorch_cuda.egg-info/dependency_links.txt
+-rw-r--r--   0 kotko      (501) staff       (20)        9 2024-04-05 16:49:23.000000 pytorch-cuda-12.1/pytorch_cuda.egg-info/requires.txt
+-rw-r--r--   0 kotko      (501) staff       (20)        6 2024-04-05 16:49:23.000000 pytorch-cuda-12.1/pytorch_cuda.egg-info/top_level.txt
+-rw-r--r--   0 kotko      (501) staff       (20)       78 2024-04-05 16:49:23.126086 pytorch-cuda-12.1/setup.cfg
+-rw-r--r--   0 kotko      (501) staff       (20)      694 2024-04-05 16:49:20.000000 pytorch-cuda-12.1/setup.py
+drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-04-05 16:49:23.125181 pytorch-cuda-12.1/tests/
+-rw-r--r--   0 kotko      (501) staff       (20)      208 2021-02-11 13:14:03.000000 pytorch-cuda-12.1/tests/__init__.py
+-rw-r--r--   0 kotko      (501) staff       (20)      417 2021-02-11 13:14:03.000000 pytorch-cuda-12.1/tests/test_simple.py
```

### Comparing `pytorch-cuda-0.0.1/LICENSE.txt` & `pytorch-cuda-12.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytorch-cuda-0.0.1/setup.py` & `pytorch-cuda-12.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 
 company = "facebookresearch--MMCSG"
 name = "pytorch-cuda"
-version = "0.0.1"
+version = "12.1"
 
 from setuptools import setup
 
 setup(
     name=name,
     version=version,
     author="Kotko Vladyslav",
```

