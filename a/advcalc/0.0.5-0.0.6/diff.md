# Comparing `tmp/advcalc-0.0.5.tar.gz` & `tmp/advcalc-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advcalc-0.0.5.tar", last modified: Fri Apr  5 02:41:55 2024, max compression
+gzip compressed data, was "advcalc-0.0.6.tar", last modified: Fri Apr  5 03:01:08 2024, max compression
```

## Comparing `advcalc-0.0.5.tar` & `advcalc-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 02:41:55.278854 advcalc-0.0.5/
-drwxrwxrwx   0        0        0        0 2024-04-05 02:41:55.235880 advcalc-0.0.5/ADVCALC/
--rw-rw-rw-   0        0        0      878 2024-04-05 02:41:15.000000 advcalc-0.0.5/ADVCALC/__init__.py
--rw-rw-rw-   0        0        0      167 2024-04-05 02:41:55.273480 advcalc-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-05 02:41:55.272880 advcalc-0.0.5/advcalc.egg-info/
--rw-rw-rw-   0        0        0      167 2024-04-05 02:41:55.000000 advcalc-0.0.5/advcalc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-04-05 02:41:55.000000 advcalc-0.0.5/advcalc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 02:41:55.000000 advcalc-0.0.5/advcalc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 02:41:55.000000 advcalc-0.0.5/advcalc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 02:41:55.278854 advcalc-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      486 2024-04-05 02:41:47.000000 advcalc-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 03:01:08.605664 advcalc-0.0.6/
+drwxrwxrwx   0        0        0        0 2024-04-05 03:01:08.563454 advcalc-0.0.6/ADVCALC/
+-rw-rw-rw-   0        0        0      878 2024-04-05 02:41:15.000000 advcalc-0.0.6/ADVCALC/__init__.py
+-rw-rw-rw-   0        0        0     1091 2024-04-05 02:48:20.000000 advcalc-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      511 2024-04-05 03:01:08.602561 advcalc-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2024-04-05 02:58:02.000000 advcalc-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 03:01:08.599051 advcalc-0.0.6/advcalc.egg-info/
+-rw-rw-rw-   0        0        0      511 2024-04-05 03:01:08.000000 advcalc-0.0.6/advcalc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-04-05 03:01:08.000000 advcalc-0.0.6/advcalc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 03:01:08.000000 advcalc-0.0.6/advcalc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 03:01:08.000000 advcalc-0.0.6/advcalc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 03:01:08.605664 advcalc-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      533 2024-04-05 03:00:56.000000 advcalc-0.0.6/setup.py
```

### Comparing `advcalc-0.0.5/ADVCALC/__init__.py` & `advcalc-0.0.6/ADVCALC/__init__.py`

 * *Files identical despite different names*

