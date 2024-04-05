# Comparing `tmp/ASnake-0.13.34.tar.gz` & `tmp/ASnake-0.13.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ASnake-0.13.34.tar", last modified: Wed Apr  3 20:39:46 2024, max compression
+gzip compressed data, was "ASnake-0.13.35.tar", last modified: Fri Apr  5 08:11:42 2024, max compression
```

## Comparing `ASnake-0.13.34.tar` & `ASnake-0.13.35.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-03 20:39:46.316698 ASnake-0.13.34/
-drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-03 20:39:46.316698 ASnake-0.13.34/ASnake.egg-info/
--rw-r--r--   0 ahri      (1002) ahri      (1002)     1091 2024-04-03 20:39:46.000000 ASnake-0.13.34/ASnake.egg-info/PKG-INFO
--rw-r--r--   0 ahri      (1002) ahri      (1002)      222 2024-04-03 20:39:46.000000 ASnake-0.13.34/ASnake.egg-info/SOURCES.txt
--rw-r--r--   0 ahri      (1002) ahri      (1002)        1 2024-04-03 20:39:46.000000 ASnake-0.13.34/ASnake.egg-info/dependency_links.txt
--rw-r--r--   0 ahri      (1002) ahri      (1002)       39 2024-04-03 20:39:46.000000 ASnake-0.13.34/ASnake.egg-info/entry_points.txt
--rw-r--r--   0 ahri      (1002) ahri      (1002)       25 2024-04-03 20:39:46.000000 ASnake-0.13.34/ASnake.egg-info/requires.txt
--rw-r--r--   0 ahri      (1002) ahri      (1002)        1 2024-04-03 20:39:46.000000 ASnake-0.13.34/ASnake.egg-info/top_level.txt
--rw-r--r--   0 ahri      (1002) ahri      (1002)    11357 2021-09-03 10:06:02.000000 ASnake-0.13.34/LICENSE.txt
--rw-r--r--   0 ahri      (1002) ahri      (1002)     1091 2024-04-03 20:39:46.316698 ASnake-0.13.34/PKG-INFO
--rw-r--r--   0 ahri      (1002) ahri      (1002)      772 2022-05-13 17:12:20.000000 ASnake-0.13.34/README.md
--rw-r--r--   0 ahri      (1002) ahri      (1002)      454 2024-04-03 20:39:46.316698 ASnake-0.13.34/setup.cfg
--rw-r--r--   0 ahri      (1002) ahri      (1002)      686 2024-04-03 20:33:36.000000 ASnake-0.13.34/setup.py
+drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-05 08:11:42.079517 ASnake-0.13.35/
+drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-05 08:11:42.079517 ASnake-0.13.35/ASnake.egg-info/
+-rw-r--r--   0 ahri      (1002) ahri      (1002)     1133 2024-04-05 08:11:42.000000 ASnake-0.13.35/ASnake.egg-info/PKG-INFO
+-rw-r--r--   0 ahri      (1002) ahri      (1002)      263 2024-04-05 08:11:42.000000 ASnake-0.13.35/ASnake.egg-info/SOURCES.txt
+-rw-r--r--   0 ahri      (1002) ahri      (1002)        1 2024-04-05 08:11:42.000000 ASnake-0.13.35/ASnake.egg-info/dependency_links.txt
+-rw-r--r--   0 ahri      (1002) ahri      (1002)       39 2024-04-05 08:11:42.000000 ASnake-0.13.35/ASnake.egg-info/entry_points.txt
+-rw-r--r--   0 ahri      (1002) ahri      (1002)       25 2024-04-05 08:11:42.000000 ASnake-0.13.35/ASnake.egg-info/requires.txt
+-rw-r--r--   0 ahri      (1002) ahri      (1002)       19 2024-04-05 08:11:42.000000 ASnake-0.13.35/ASnake.egg-info/top_level.txt
+-rwxr-xr-x   0 ahri      (1002) ahri      (1002)   536080 2024-04-03 17:22:37.000000 ASnake-0.13.35/ASnake.py
+-rw-r--r--   0 ahri      (1002) ahri      (1002)    11357 2021-09-03 10:06:02.000000 ASnake-0.13.35/LICENSE.txt
+-rw-r--r--   0 ahri      (1002) ahri      (1002)     1133 2024-04-05 08:11:42.079517 ASnake-0.13.35/PKG-INFO
+-rw-r--r--   0 ahri      (1002) ahri      (1002)      814 2024-04-03 21:05:15.000000 ASnake-0.13.35/README.md
+-rw-r--r--   0 ahri      (1002) ahri      (1002)       25 2024-04-05 08:11:22.000000 ASnake-0.13.35/__version__.py
+-rwxr-xr-x   0 ahri      (1002) ahri      (1002)     8889 2024-03-31 14:25:37.000000 ASnake-0.13.35/megaTest.asnake
+-rw-r--r--   0 ahri      (1002) ahri      (1002)      454 2024-04-05 08:11:42.079517 ASnake-0.13.35/setup.cfg
+-rw-r--r--   0 ahri      (1002) ahri      (1002)      750 2024-04-05 08:11:22.000000 ASnake-0.13.35/setup.py
```

### Comparing `ASnake-0.13.34/ASnake.egg-info/PKG-INFO` & `ASnake-0.13.35/ASnake.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASnake
-Version: 0.13.34
+Version: 0.13.35
 Summary: Optimizing Python transpiler for the ASnake programming language.
 Home-page: https://asnake.org
 Author: Ahri Fox
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: sly>=0.4
@@ -12,18 +12,20 @@
 
 # ASnake
 Optimizing Python transpiler for the ASnake programming language.
 
 A proper readme is yet to come. If you are super interested, we have a lot more info (including some draft documentation) on this Discord:
 https://discord.gg/ySDFchT
 
-To install, clone this repository or download a release. Open a terminal in the directory and run:
+To install run:
 ```console
-pip install -e .
+python -m pip install ASnake
 ```
+You may have to use `py` or `python3` or similar depending on what you have installed for a Python interpreter.
+
 After that, ASnake and all it's compiler flags can be callable via:
 ```console
 python -m ASnake
 ```
 Here are some examples:
 ```console
 python -m ASnake -e "'Hello world!'"
```

### Comparing `ASnake-0.13.34/LICENSE.txt` & `ASnake-0.13.35/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ASnake-0.13.34/PKG-INFO` & `ASnake-0.13.35/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASnake
-Version: 0.13.34
+Version: 0.13.35
 Summary: Optimizing Python transpiler for the ASnake programming language.
 Home-page: https://asnake.org
 Author: Ahri Fox
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: sly>=0.4
@@ -12,18 +12,20 @@
 
 # ASnake
 Optimizing Python transpiler for the ASnake programming language.
 
 A proper readme is yet to come. If you are super interested, we have a lot more info (including some draft documentation) on this Discord:
 https://discord.gg/ySDFchT
 
-To install, clone this repository or download a release. Open a terminal in the directory and run:
+To install run:
 ```console
-pip install -e .
+python -m pip install ASnake
 ```
+You may have to use `py` or `python3` or similar depending on what you have installed for a Python interpreter.
+
 After that, ASnake and all it's compiler flags can be callable via:
 ```console
 python -m ASnake
 ```
 Here are some examples:
 ```console
 python -m ASnake -e "'Hello world!'"
```

