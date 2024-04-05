# Comparing `tmp/advcalc-0.0.6.tar.gz` & `tmp/advcalc-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advcalc-0.0.6.tar", last modified: Fri Apr  5 03:01:08 2024, max compression
+gzip compressed data, was "advcalc-0.0.7.tar", last modified: Fri Apr  5 03:06:58 2024, max compression
```

## Comparing `advcalc-0.0.6.tar` & `advcalc-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 03:01:08.605664 advcalc-0.0.6/
-drwxrwxrwx   0        0        0        0 2024-04-05 03:01:08.563454 advcalc-0.0.6/ADVCALC/
--rw-rw-rw-   0        0        0      878 2024-04-05 02:41:15.000000 advcalc-0.0.6/ADVCALC/__init__.py
--rw-rw-rw-   0        0        0     1091 2024-04-05 02:48:20.000000 advcalc-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      511 2024-04-05 03:01:08.602561 advcalc-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      336 2024-04-05 02:58:02.000000 advcalc-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 03:01:08.599051 advcalc-0.0.6/advcalc.egg-info/
--rw-rw-rw-   0        0        0      511 2024-04-05 03:01:08.000000 advcalc-0.0.6/advcalc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-04-05 03:01:08.000000 advcalc-0.0.6/advcalc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 03:01:08.000000 advcalc-0.0.6/advcalc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 03:01:08.000000 advcalc-0.0.6/advcalc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 03:01:08.605664 advcalc-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      533 2024-04-05 03:00:56.000000 advcalc-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 03:06:58.799033 advcalc-0.0.7/
+drwxrwxrwx   0        0        0        0 2024-04-05 03:06:58.762496 advcalc-0.0.7/ADVCALC/
+-rw-rw-rw-   0        0        0      878 2024-04-05 02:41:15.000000 advcalc-0.0.7/ADVCALC/__init__.py
+-rw-rw-rw-   0        0        0     1091 2024-04-05 02:48:20.000000 advcalc-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      552 2024-04-05 03:06:58.794981 advcalc-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2024-04-05 02:58:02.000000 advcalc-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 03:06:58.794981 advcalc-0.0.7/advcalc.egg-info/
+-rw-rw-rw-   0        0        0      552 2024-04-05 03:06:58.000000 advcalc-0.0.7/advcalc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-04-05 03:06:58.000000 advcalc-0.0.7/advcalc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 03:06:58.000000 advcalc-0.0.7/advcalc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 03:06:58.000000 advcalc-0.0.7/advcalc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 03:06:58.799033 advcalc-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      589 2024-04-05 03:06:56.000000 advcalc-0.0.7/setup.py
```

### Comparing `advcalc-0.0.6/ADVCALC/__init__.py` & `advcalc-0.0.7/ADVCALC/__init__.py`

 * *Files identical despite different names*

### Comparing `advcalc-0.0.6/LICENSE` & `advcalc-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `advcalc-0.0.6/setup.py` & `advcalc-0.0.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
         LONG_DESCRIPTION = fh.read()
 
-VERSION = '0.0.6' 
+VERSION = '0.0.7' 
 DESCRIPTION = 'Advanced Python Calculator'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="advcalc", 
         version=VERSION,
         author="Zack",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
+        long_description_content_type="text/markdown",
         packages=find_packages(),
         keywords=['python', 'calculator'],
         license="MIT"
 )
```

