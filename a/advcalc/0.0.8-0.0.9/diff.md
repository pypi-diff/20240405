# Comparing `tmp/advcalc-0.0.8.tar.gz` & `tmp/advcalc-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advcalc-0.0.8.tar", last modified: Fri Apr  5 03:27:29 2024, max compression
+gzip compressed data, was "advcalc-0.0.9.tar", last modified: Fri Apr  5 03:28:54 2024, max compression
```

## Comparing `advcalc-0.0.8.tar` & `advcalc-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 03:27:29.627090 advcalc-0.0.8/
-drwxrwxrwx   0        0        0        0 2024-04-05 03:27:29.599523 advcalc-0.0.8/ADVCALC/
--rw-rw-rw-   0        0        0      878 2024-04-05 02:41:15.000000 advcalc-0.0.8/ADVCALC/__init__.py
--rw-rw-rw-   0        0        0     1091 2024-04-05 02:48:20.000000 advcalc-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      562 2024-04-05 03:27:29.627090 advcalc-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      346 2024-04-05 03:26:54.000000 advcalc-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 03:27:29.624363 advcalc-0.0.8/advcalc.egg-info/
--rw-rw-rw-   0        0        0      562 2024-04-05 03:27:29.000000 advcalc-0.0.8/advcalc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-04-05 03:27:29.000000 advcalc-0.0.8/advcalc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 03:27:29.000000 advcalc-0.0.8/advcalc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 03:27:29.000000 advcalc-0.0.8/advcalc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 03:27:29.630430 advcalc-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      589 2024-04-05 03:27:09.000000 advcalc-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 03:28:54.034927 advcalc-0.0.9/
+drwxrwxrwx   0        0        0        0 2024-04-05 03:28:54.002637 advcalc-0.0.9/ADVCALC/
+-rw-rw-rw-   0        0        0      878 2024-04-05 02:41:15.000000 advcalc-0.0.9/ADVCALC/__init__.py
+-rw-rw-rw-   0        0        0     1091 2024-04-05 02:48:20.000000 advcalc-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      588 2024-04-05 03:28:54.030856 advcalc-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2024-04-05 03:28:33.000000 advcalc-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 03:28:54.030856 advcalc-0.0.9/advcalc.egg-info/
+-rw-rw-rw-   0        0        0      588 2024-04-05 03:28:53.000000 advcalc-0.0.9/advcalc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-04-05 03:28:53.000000 advcalc-0.0.9/advcalc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 03:28:53.000000 advcalc-0.0.9/advcalc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 03:28:53.000000 advcalc-0.0.9/advcalc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 03:28:54.034927 advcalc-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      589 2024-04-05 03:28:43.000000 advcalc-0.0.9/setup.py
```

### Comparing `advcalc-0.0.8/ADVCALC/__init__.py` & `advcalc-0.0.9/ADVCALC/__init__.py`

 * *Files identical despite different names*

### Comparing `advcalc-0.0.8/LICENSE` & `advcalc-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `advcalc-0.0.8/PKG-INFO` & `advcalc-0.0.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,29 @@
 Metadata-Version: 2.1
 Name: advcalc
-Version: 0.0.8
+Version: 0.0.9
 Summary: Advanced Python Calculator
 Author: Zack
 License: MIT
 Keywords: python,calculator
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ADVCALC
 ## How to use it
 ##### First use, `pip instal advcalc`.
 ##### Then, import it in your python file by using `import ADVCALC` or you can use `from ADVCALC import pow` or what so ever.
 
-##### The functions include `advcalc``add``sub``div``mul``sqrt``square``round_without_decimal_place``round_with_decimal_place``cube``cbrt``and``pow`
+##### The functions include:
+`advcalc`
+`add`
+`sub`
+`div`
+`mul`
+`sqrt`
+`square`
+`round_without_decimal_place`
+`round_with_decimal_place`
+`cube`
+`cbrt`
+`and`
+`pow`
```

### Comparing `advcalc-0.0.8/advcalc.egg-info/PKG-INFO` & `advcalc-0.0.9/advcalc.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,29 @@
 Metadata-Version: 2.1
 Name: advcalc
-Version: 0.0.8
+Version: 0.0.9
 Summary: Advanced Python Calculator
 Author: Zack
 License: MIT
 Keywords: python,calculator
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ADVCALC
 ## How to use it
 ##### First use, `pip instal advcalc`.
 ##### Then, import it in your python file by using `import ADVCALC` or you can use `from ADVCALC import pow` or what so ever.
 
-##### The functions include `advcalc``add``sub``div``mul``sqrt``square``round_without_decimal_place``round_with_decimal_place``cube``cbrt``and``pow`
+##### The functions include:
+`advcalc`
+`add`
+`sub`
+`div`
+`mul`
+`sqrt`
+`square`
+`round_without_decimal_place`
+`round_with_decimal_place`
+`cube`
+`cbrt`
+`and`
+`pow`
```

### Comparing `advcalc-0.0.8/setup.py` & `advcalc-0.0.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
         LONG_DESCRIPTION = fh.read()
 
-VERSION = '0.0.8' 
+VERSION = '0.0.9' 
 DESCRIPTION = 'Advanced Python Calculator'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="advcalc", 
         version=VERSION,
```

