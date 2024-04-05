# Comparing `tmp/botocore.exceptions-1.2.4.tar.gz` & `tmp/botocore.exceptions-1.23.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore.exceptions-1.2.4.tar", last modified: Fri Apr  5 16:33:32 2024, max compression
+gzip compressed data, was "botocore.exceptions-1.23.19.tar", last modified: Fri Apr  5 16:33:50 2024, max compression
```

## Comparing `botocore.exceptions-1.2.4.tar` & `botocore.exceptions-1.23.19.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-04-05 16:33:32.909009 botocore.exceptions-1.2.4/
--rw-r--r--   0 kotko      (501) staff       (20)     1081 2021-02-11 13:14:03.000000 botocore.exceptions-1.2.4/LICENSE.txt
--rw-r--r--   0 kotko      (501) staff       (20)      194 2021-02-11 13:14:03.000000 botocore.exceptions-1.2.4/MANIFEST.in
--rw-r--r--   0 kotko      (501) staff       (20)      448 2024-04-05 16:33:32.908920 botocore.exceptions-1.2.4/PKG-INFO
--rw-r--r--   0 kotko      (501) staff       (20)       15 2023-05-10 17:51:27.000000 botocore.exceptions-1.2.4/README.md
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-04-05 16:33:32.908696 botocore.exceptions-1.2.4/botocore.exceptions.egg-info/
--rw-r--r--   0 kotko      (501) staff       (20)      448 2024-04-05 16:33:32.000000 botocore.exceptions-1.2.4/botocore.exceptions.egg-info/PKG-INFO
--rw-r--r--   0 kotko      (501) staff       (20)      335 2024-04-05 16:33:32.000000 botocore.exceptions-1.2.4/botocore.exceptions.egg-info/SOURCES.txt
--rw-r--r--   0 kotko      (501) staff       (20)        1 2024-04-05 16:33:32.000000 botocore.exceptions-1.2.4/botocore.exceptions.egg-info/dependency_links.txt
--rw-r--r--   0 kotko      (501) staff       (20)        9 2024-04-05 16:33:32.000000 botocore.exceptions-1.2.4/botocore.exceptions.egg-info/requires.txt
--rw-r--r--   0 kotko      (501) staff       (20)        6 2024-04-05 16:33:32.000000 botocore.exceptions-1.2.4/botocore.exceptions.egg-info/top_level.txt
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-04-05 16:33:32.907806 botocore.exceptions-1.2.4/data/
--rw-r--r--   0 kotko      (501) staff       (20)        9 2021-02-11 13:14:03.000000 botocore.exceptions-1.2.4/data/data_file
--rw-r--r--   0 kotko      (501) staff       (20)      253 2021-02-11 16:09:08.000000 botocore.exceptions-1.2.4/pyproject.toml
--rw-r--r--   0 kotko      (501) staff       (20)       78 2024-04-05 16:33:32.909230 botocore.exceptions-1.2.4/setup.cfg
--rw-r--r--   0 kotko      (501) staff       (20)      726 2024-04-05 16:33:18.000000 botocore.exceptions-1.2.4/setup.py
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-04-05 16:33:32.908383 botocore.exceptions-1.2.4/tests/
--rw-r--r--   0 kotko      (501) staff       (20)      208 2021-02-11 13:14:03.000000 botocore.exceptions-1.2.4/tests/__init__.py
--rw-r--r--   0 kotko      (501) staff       (20)      417 2021-02-11 13:14:03.000000 botocore.exceptions-1.2.4/tests/test_simple.py
+drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-04-05 16:33:50.953850 botocore.exceptions-1.23.19/
+-rw-r--r--   0 kotko      (501) staff       (20)     1081 2021-02-11 13:14:03.000000 botocore.exceptions-1.23.19/LICENSE.txt
+-rw-r--r--   0 kotko      (501) staff       (20)      194 2021-02-11 13:14:03.000000 botocore.exceptions-1.23.19/MANIFEST.in
+-rw-r--r--   0 kotko      (501) staff       (20)      450 2024-04-05 16:33:50.953781 botocore.exceptions-1.23.19/PKG-INFO
+-rw-r--r--   0 kotko      (501) staff       (20)       15 2023-05-10 17:51:27.000000 botocore.exceptions-1.23.19/README.md
+drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-04-05 16:33:50.953521 botocore.exceptions-1.23.19/botocore.exceptions.egg-info/
+-rw-r--r--   0 kotko      (501) staff       (20)      450 2024-04-05 16:33:50.000000 botocore.exceptions-1.23.19/botocore.exceptions.egg-info/PKG-INFO
+-rw-r--r--   0 kotko      (501) staff       (20)      335 2024-04-05 16:33:50.000000 botocore.exceptions-1.23.19/botocore.exceptions.egg-info/SOURCES.txt
+-rw-r--r--   0 kotko      (501) staff       (20)        1 2024-04-05 16:33:50.000000 botocore.exceptions-1.23.19/botocore.exceptions.egg-info/dependency_links.txt
+-rw-r--r--   0 kotko      (501) staff       (20)        9 2024-04-05 16:33:50.000000 botocore.exceptions-1.23.19/botocore.exceptions.egg-info/requires.txt
+-rw-r--r--   0 kotko      (501) staff       (20)        6 2024-04-05 16:33:50.000000 botocore.exceptions-1.23.19/botocore.exceptions.egg-info/top_level.txt
+drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-04-05 16:33:50.952686 botocore.exceptions-1.23.19/data/
+-rw-r--r--   0 kotko      (501) staff       (20)        9 2021-02-11 13:14:03.000000 botocore.exceptions-1.23.19/data/data_file
+-rw-r--r--   0 kotko      (501) staff       (20)      253 2021-02-11 16:09:08.000000 botocore.exceptions-1.23.19/pyproject.toml
+-rw-r--r--   0 kotko      (501) staff       (20)       78 2024-04-05 16:33:50.954085 botocore.exceptions-1.23.19/setup.cfg
+-rw-r--r--   0 kotko      (501) staff       (20)      728 2024-04-05 16:33:48.000000 botocore.exceptions-1.23.19/setup.py
+drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-04-05 16:33:50.953170 botocore.exceptions-1.23.19/tests/
+-rw-r--r--   0 kotko      (501) staff       (20)      208 2021-02-11 13:14:03.000000 botocore.exceptions-1.23.19/tests/__init__.py
+-rw-r--r--   0 kotko      (501) staff       (20)      417 2021-02-11 13:14:03.000000 botocore.exceptions-1.23.19/tests/test_simple.py
```

### Comparing `botocore.exceptions-1.2.4/LICENSE.txt` & `botocore.exceptions-1.23.19/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore.exceptions-1.2.4/setup.py` & `botocore.exceptions-1.23.19/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 
 company = "aws-samples--amazon-s3-default-encryption-audit"
 name = "botocore.exceptions"
-version = "1.2.4"
+version = "1.23.19"
 
 from setuptools import setup
 
 setup(
     name=name,
     version=version,
     author="Kotko Vladyslav",
```

