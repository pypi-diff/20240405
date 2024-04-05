# Comparing `tmp/advcalc-0.0.9.tar.gz` & `tmp/advcalc-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advcalc-0.0.9.tar", last modified: Fri Apr  5 03:28:54 2024, max compression
+gzip compressed data, was "advcalc-0.1.0.tar", last modified: Fri Apr  5 03:31:00 2024, max compression
```

## Comparing `advcalc-0.0.9.tar` & `advcalc-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 03:28:54.034927 advcalc-0.0.9/
-drwxrwxrwx   0        0        0        0 2024-04-05 03:28:54.002637 advcalc-0.0.9/ADVCALC/
--rw-rw-rw-   0        0        0      878 2024-04-05 02:41:15.000000 advcalc-0.0.9/ADVCALC/__init__.py
--rw-rw-rw-   0        0        0     1091 2024-04-05 02:48:20.000000 advcalc-0.0.9/LICENSE
--rw-rw-rw-   0        0        0      588 2024-04-05 03:28:54.030856 advcalc-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      372 2024-04-05 03:28:33.000000 advcalc-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 03:28:54.030856 advcalc-0.0.9/advcalc.egg-info/
--rw-rw-rw-   0        0        0      588 2024-04-05 03:28:53.000000 advcalc-0.0.9/advcalc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-04-05 03:28:53.000000 advcalc-0.0.9/advcalc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 03:28:53.000000 advcalc-0.0.9/advcalc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 03:28:53.000000 advcalc-0.0.9/advcalc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 03:28:54.034927 advcalc-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      589 2024-04-05 03:28:43.000000 advcalc-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 03:31:00.388470 advcalc-0.1.0/
+drwxrwxrwx   0        0        0        0 2024-04-05 03:31:00.355874 advcalc-0.1.0/ADVCALC/
+-rw-rw-rw-   0        0        0      878 2024-04-05 02:41:15.000000 advcalc-0.1.0/ADVCALC/__init__.py
+-rw-rw-rw-   0        0        0     1091 2024-04-05 02:48:20.000000 advcalc-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      633 2024-04-05 03:31:00.384492 advcalc-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      417 2024-04-05 03:30:30.000000 advcalc-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 03:31:00.380396 advcalc-0.1.0/advcalc.egg-info/
+-rw-rw-rw-   0        0        0      633 2024-04-05 03:31:00.000000 advcalc-0.1.0/advcalc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-04-05 03:31:00.000000 advcalc-0.1.0/advcalc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 03:31:00.000000 advcalc-0.1.0/advcalc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 03:31:00.000000 advcalc-0.1.0/advcalc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 03:31:00.388470 advcalc-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      589 2024-04-05 03:30:56.000000 advcalc-0.1.0/setup.py
```

### Comparing `advcalc-0.0.9/ADVCALC/__init__.py` & `advcalc-0.1.0/ADVCALC/__init__.py`

 * *Files identical despite different names*

### Comparing `advcalc-0.0.9/LICENSE` & `advcalc-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `advcalc-0.0.9/setup.py` & `advcalc-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
         LONG_DESCRIPTION = fh.read()
 
-VERSION = '0.0.9' 
+VERSION = '0.1.0' 
 DESCRIPTION = 'Advanced Python Calculator'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="advcalc", 
         version=VERSION,
```

