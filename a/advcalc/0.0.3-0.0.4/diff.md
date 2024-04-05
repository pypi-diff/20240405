# Comparing `tmp/advcalc-0.0.3.tar.gz` & `tmp/advcalc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advcalc-0.0.3.tar", last modified: Fri Apr  5 02:28:49 2024, max compression
+gzip compressed data, was "advcalc-0.0.4.tar", last modified: Fri Apr  5 02:29:00 2024, max compression
```

## Comparing `advcalc-0.0.3.tar` & `advcalc-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 02:28:49.436097 advcalc-0.0.3/
-drwxrwxrwx   0        0        0        0 2024-04-05 02:28:49.410882 advcalc-0.0.3/ADVCALC/
--rw-rw-rw-   0        0        0      317 2024-04-03 02:17:17.000000 advcalc-0.0.3/ADVCALC/__init__.py
--rw-rw-rw-   0        0        0      878 2024-04-05 02:02:00.000000 advcalc-0.0.3/ADVCALC/calc.py
--rw-rw-rw-   0        0        0      167 2024-04-05 02:28:49.433347 advcalc-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-05 02:28:49.428719 advcalc-0.0.3/advcalc.egg-info/
--rw-rw-rw-   0        0        0      167 2024-04-05 02:28:49.000000 advcalc-0.0.3/advcalc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2024-04-05 02:28:49.000000 advcalc-0.0.3/advcalc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 02:28:49.000000 advcalc-0.0.3/advcalc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 02:28:49.000000 advcalc-0.0.3/advcalc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 02:28:49.436097 advcalc-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      486 2024-04-05 02:20:40.000000 advcalc-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 02:29:00.475412 advcalc-0.0.4/
+drwxrwxrwx   0        0        0        0 2024-04-05 02:29:00.423425 advcalc-0.0.4/ADVCALC/
+-rw-rw-rw-   0        0        0      317 2024-04-03 02:17:17.000000 advcalc-0.0.4/ADVCALC/__init__.py
+-rw-rw-rw-   0        0        0      878 2024-04-05 02:02:00.000000 advcalc-0.0.4/ADVCALC/calc.py
+-rw-rw-rw-   0        0        0      167 2024-04-05 02:29:00.472480 advcalc-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-05 02:29:00.469304 advcalc-0.0.4/advcalc.egg-info/
+-rw-rw-rw-   0        0        0      167 2024-04-05 02:29:00.000000 advcalc-0.0.4/advcalc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2024-04-05 02:29:00.000000 advcalc-0.0.4/advcalc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 02:29:00.000000 advcalc-0.0.4/advcalc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 02:29:00.000000 advcalc-0.0.4/advcalc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 02:29:00.475412 advcalc-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      486 2024-04-05 02:28:57.000000 advcalc-0.0.4/setup.py
```

### Comparing `advcalc-0.0.3/ADVCALC/calc.py` & `advcalc-0.0.4/ADVCALC/calc.py`

 * *Files identical despite different names*

