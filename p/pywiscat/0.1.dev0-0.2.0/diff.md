# Comparing `tmp/pywiscat-0.1.dev0.tar.gz` & `tmp/pywiscat-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pywiscat-0.1.dev0.tar", last modified: Sat Jun  5 13:35:17 2021, max compression
+gzip compressed data, was "pywiscat-0.2.0.tar", last modified: Fri Apr  5 11:39:04 2024, max compression
```

## Comparing `pywiscat-0.1.dev0.tar` & `pywiscat-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 tkralidi   (501) staff       (20)        0 2021-06-05 13:35:17.000000 pywiscat-0.1.dev0/
--rw-r--r--   0 tkralidi   (501) staff       (20)     1091 2021-06-04 15:27:11.000000 pywiscat-0.1.dev0/LICENSE.md
--rw-r--r--   0 tkralidi   (501) staff       (20)       46 2021-06-04 15:26:23.000000 pywiscat-0.1.dev0/MANIFEST.in
--rw-r--r--   0 tkralidi   (501) staff       (20)     4295 2021-06-05 13:35:17.000000 pywiscat-0.1.dev0/PKG-INFO
--rw-r--r--   0 tkralidi   (501) staff       (20)     2514 2021-06-05 13:28:15.000000 pywiscat-0.1.dev0/README.md
-drwxr-xr-x   0 tkralidi   (501) staff       (20)        0 2021-06-05 13:35:17.000000 pywiscat-0.1.dev0/pywiscat/
--rw-r--r--   0 tkralidi   (501) staff       (20)     1463 2021-06-05 13:27:21.000000 pywiscat-0.1.dev0/pywiscat/__init__.py
--rw-r--r--   0 tkralidi   (501) staff       (20)     2060 2021-06-05 00:03:47.000000 pywiscat-0.1.dev0/pywiscat/cli_helpers.py
-drwxr-xr-x   0 tkralidi   (501) staff       (20)        0 2021-06-05 13:35:17.000000 pywiscat-0.1.dev0/pywiscat/wis1/
--rw-r--r--   0 tkralidi   (501) staff       (20)     1519 2021-06-05 13:24:33.000000 pywiscat-0.1.dev0/pywiscat/wis1/__init__.py
--rw-r--r--   0 tkralidi   (501) staff       (20)     2396 2021-06-05 13:27:46.000000 pywiscat-0.1.dev0/pywiscat/wis1/catalogue.py
--rw-r--r--   0 tkralidi   (501) staff       (20)     4370 2021-06-05 00:57:26.000000 pywiscat-0.1.dev0/pywiscat/wis1/report.py
-drwxr-xr-x   0 tkralidi   (501) staff       (20)        0 2021-06-05 13:35:17.000000 pywiscat-0.1.dev0/pywiscat.egg-info/
--rw-r--r--   0 tkralidi   (501) staff       (20)     4295 2021-06-05 13:35:17.000000 pywiscat-0.1.dev0/pywiscat.egg-info/PKG-INFO
--rw-r--r--   0 tkralidi   (501) staff       (20)      374 2021-06-05 13:35:17.000000 pywiscat-0.1.dev0/pywiscat.egg-info/SOURCES.txt
--rw-r--r--   0 tkralidi   (501) staff       (20)        1 2021-06-05 13:35:17.000000 pywiscat-0.1.dev0/pywiscat.egg-info/dependency_links.txt
--rw-r--r--   0 tkralidi   (501) staff       (20)       43 2021-06-05 13:35:17.000000 pywiscat-0.1.dev0/pywiscat.egg-info/entry_points.txt
--rw-r--r--   0 tkralidi   (501) staff       (20)       15 2021-06-05 13:35:17.000000 pywiscat-0.1.dev0/pywiscat.egg-info/requires.txt
--rw-r--r--   0 tkralidi   (501) staff       (20)        9 2021-06-05 13:35:17.000000 pywiscat-0.1.dev0/pywiscat.egg-info/top_level.txt
--rw-r--r--   0 tkralidi   (501) staff       (20)       15 2021-06-04 15:25:21.000000 pywiscat-0.1.dev0/requirements.txt
--rw-r--r--   0 tkralidi   (501) staff       (20)       38 2021-06-05 13:35:17.000000 pywiscat-0.1.dev0/setup.cfg
--rw-r--r--   0 tkralidi   (501) staff       (20)     3751 2021-06-04 15:31:03.000000 pywiscat-0.1.dev0/setup.py
+drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2024-04-05 11:39:04.210657 pywiscat-0.2.0/
+-rw-r--r--   0 tomkralidis   (501) staff       (20)     1091 2021-06-04 15:27:11.000000 pywiscat-0.2.0/LICENSE.md
+-rw-r--r--   0 tomkralidis   (501) staff       (20)       46 2021-06-04 15:26:23.000000 pywiscat-0.2.0/MANIFEST.in
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     3884 2024-04-05 11:39:04.210223 pywiscat-0.2.0/PKG-INFO
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     3013 2024-04-05 11:37:40.000000 pywiscat-0.2.0/README.md
+drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2024-04-05 11:39:04.203255 pywiscat-0.2.0/pywiscat/
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     1530 2024-04-05 11:38:12.000000 pywiscat-0.2.0/pywiscat/__init__.py
+-rw-r--r--   0 tomkralidis   (501) staff       (20)     2060 2023-03-13 21:14:30.000000 pywiscat-0.2.0/pywiscat/cli_helpers.py
+drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2024-04-05 11:39:04.209204 pywiscat-0.2.0/pywiscat/wis2/
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     1525 2023-10-06 11:32:01.000000 pywiscat-0.2.0/pywiscat/wis2/__init__.py
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     9417 2024-04-05 11:37:40.000000 pywiscat-0.2.0/pywiscat/wis2/catalogue.py
+drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2024-04-05 11:39:04.207257 pywiscat-0.2.0/pywiscat.egg-info/
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     3884 2024-04-05 11:39:04.000000 pywiscat-0.2.0/pywiscat.egg-info/PKG-INFO
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)      350 2024-04-05 11:39:04.000000 pywiscat-0.2.0/pywiscat.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)        1 2024-04-05 11:39:04.000000 pywiscat-0.2.0/pywiscat.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)       42 2024-04-05 11:39:04.000000 pywiscat-0.2.0/pywiscat.egg-info/entry_points.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)       54 2024-04-05 11:39:04.000000 pywiscat-0.2.0/pywiscat.egg-info/requires.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)        9 2024-04-05 11:39:04.000000 pywiscat-0.2.0/pywiscat.egg-info/top_level.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)       54 2023-10-06 11:32:01.000000 pywiscat-0.2.0/requirements.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)       38 2024-04-05 11:39:04.210821 pywiscat-0.2.0/setup.cfg
+-rw-r--r--   0 tomkralidis   (501) staff       (20)     3751 2023-09-19 03:07:40.000000 pywiscat-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pywiscat-0.1.dev0/LICENSE.md` & `pywiscat-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pywiscat-0.1.dev0/pywiscat/__init__.py` & `pywiscat-0.2.0/pywiscat/wis2/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # =================================================================
 #
 # Authors: Tom Kralidis <tomkralidis@gmail.com>
 #
-# Copyright (c) 2021 Tom Kralidis
+# Copyright (c) 2023 Tom Kralidis
 #
 # Permission is hereby granted, free of charge, to any person
 # obtaining a copy of this software and associated documentation
 # files (the "Software"), to deal in the Software without
 # restriction, including without limitation the rights to use,
 # copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the
@@ -25,19 +25,18 @@
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 # OTHER DEALINGS IN THE SOFTWARE.
 #
 # =================================================================
 
 import click
 
-from pywiscat.wis1 import wis1
-
-__version__ = '0.1.dev0'
+from pywiscat.wis2.catalogue import get_gdc_record, search_gdc
 
 
 @click.group()
-@click.version_option(version=__version__)
-def cli():
+def wis2():
+    """WIS2 Global Discovery Catalogue (GDC) utilities"""
     pass
 
 
-cli.add_command(wis1)
+wis2.add_command(search_gdc)
+wis2.add_command(get_gdc_record)
```

### Comparing `pywiscat-0.1.dev0/pywiscat/cli_helpers.py` & `pywiscat-0.2.0/pywiscat/cli_helpers.py`

 * *Files identical despite different names*

### Comparing `pywiscat-0.1.dev0/pywiscat/wis1/__init__.py` & `pywiscat-0.2.0/pywiscat/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # =================================================================
 #
 # Authors: Tom Kralidis <tomkralidis@gmail.com>
 #
-# Copyright (c) 2021 Tom Kralidis
+# Copyright (c) 2024 Tom Kralidis
 #
 # Permission is hereby granted, free of charge, to any person
 # obtaining a copy of this software and associated documentation
 # files (the "Software"), to deal in the Software without
 # restriction, including without limitation the rights to use,
 # copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the
@@ -25,19 +25,20 @@
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 # OTHER DEALINGS IN THE SOFTWARE.
 #
 # =================================================================
 
 import click
 
-from pywiscat.wis1.catalogue import catalogue
-from pywiscat.wis1.report import report
+from pywiscat.wis2.catalogue import get_gdc_record, search_gdc
+
+__version__ = '0.2.0'
 
 
 @click.group()
-def wis1():
-    """WIS 1.0 Catalogue utilities"""
+@click.version_option(version=__version__)
+def cli():
     pass
 
 
-wis1.add_command(catalogue)
-wis1.add_command(report)
+cli.add_command(search_gdc)
+cli.add_command(get_gdc_record)
```

### Comparing `pywiscat-0.1.dev0/setup.py` & `pywiscat-0.2.0/setup.py`

 * *Files identical despite different names*

