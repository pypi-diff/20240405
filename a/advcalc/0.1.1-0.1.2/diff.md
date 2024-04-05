# Comparing `tmp/advcalc-0.1.1.tar.gz` & `tmp/advcalc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advcalc-0.1.1.tar", last modified: Fri Apr  5 03:32:35 2024, max compression
+gzip compressed data, was "advcalc-0.1.2.tar", last modified: Fri Apr  5 03:40:05 2024, max compression
```

## Comparing `advcalc-0.1.1.tar` & `advcalc-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 03:32:35.710537 advcalc-0.1.1/
-drwxrwxrwx   0        0        0        0 2024-04-05 03:32:35.680723 advcalc-0.1.1/ADVCALC/
--rw-rw-rw-   0        0        0      878 2024-04-05 02:41:15.000000 advcalc-0.1.1/ADVCALC/__init__.py
--rw-rw-rw-   0        0        0     1091 2024-04-05 02:48:20.000000 advcalc-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      702 2024-04-05 03:32:35.708009 advcalc-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      486 2024-04-05 03:32:25.000000 advcalc-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 03:32:35.705541 advcalc-0.1.1/advcalc.egg-info/
--rw-rw-rw-   0        0        0      702 2024-04-05 03:32:35.000000 advcalc-0.1.1/advcalc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-04-05 03:32:35.000000 advcalc-0.1.1/advcalc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 03:32:35.000000 advcalc-0.1.1/advcalc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 03:32:35.000000 advcalc-0.1.1/advcalc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 03:32:35.710537 advcalc-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      589 2024-04-05 03:32:32.000000 advcalc-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 03:40:05.284151 advcalc-0.1.2/
+drwxrwxrwx   0        0        0        0 2024-04-05 03:40:05.222454 advcalc-0.1.2/ADVCALC/
+-rw-rw-rw-   0        0        0      894 2024-04-05 03:38:57.000000 advcalc-0.1.2/ADVCALC/__init__.py
+-rw-rw-rw-   0        0        0     1091 2024-04-05 02:48:20.000000 advcalc-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      702 2024-04-05 03:40:05.279919 advcalc-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      486 2024-04-05 03:32:25.000000 advcalc-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 03:40:05.279919 advcalc-0.1.2/advcalc.egg-info/
+-rw-rw-rw-   0        0        0      702 2024-04-05 03:40:05.000000 advcalc-0.1.2/advcalc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-04-05 03:40:05.000000 advcalc-0.1.2/advcalc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 03:40:05.000000 advcalc-0.1.2/advcalc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 03:40:05.000000 advcalc-0.1.2/advcalc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 03:40:05.284151 advcalc-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      589 2024-04-05 03:39:01.000000 advcalc-0.1.2/setup.py
```

### Comparing `advcalc-0.1.1/ADVCALC/__init__.py` & `advcalc-0.1.2/ADVCALC/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,8 +38,9 @@
     print(sum)
     
 def cbrt(num):
     sum = float(num) ** (1. / 3)
     print(sum)
 
 def pow(num1, num2):
-    sum = float(num1) ** float(num2)
+    sum = float(num1) ** float(num2)
+    print(sum)
```

### Comparing `advcalc-0.1.1/LICENSE` & `advcalc-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `advcalc-0.1.1/PKG-INFO` & `advcalc-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: advcalc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Advanced Python Calculator
 Author: Zack
 License: MIT
 Keywords: python,calculator
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `advcalc-0.1.1/advcalc.egg-info/PKG-INFO` & `advcalc-0.1.2/advcalc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: advcalc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Advanced Python Calculator
 Author: Zack
 License: MIT
 Keywords: python,calculator
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `advcalc-0.1.1/setup.py` & `advcalc-0.1.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
         LONG_DESCRIPTION = fh.read()
 
-VERSION = '0.1.1' 
+VERSION = '0.1.2' 
 DESCRIPTION = 'Advanced Python Calculator'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="advcalc", 
         version=VERSION,
```

