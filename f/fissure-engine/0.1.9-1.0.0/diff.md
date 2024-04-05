# Comparing `tmp/fissure_engine-0.1.9.tar.gz` & `tmp/fissure_engine-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fissure_engine-0.1.9.tar", last modified: Sat Nov 19 02:45:34 2022, max compression
+gzip compressed data, was "fissure_engine-1.0.0.tar", last modified: Fri Apr  5 16:18:15 2024, max compression
```

## Comparing `fissure_engine-0.1.9.tar` & `fissure_engine-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,9 @@
-drwxrwxrwx   0        0        0        0 2022-11-19 02:45:34.632774 fissure_engine-0.1.9/
--rw-rw-rw-   0        0        0      446 2022-11-19 02:45:34.631775 fissure_engine-0.1.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-11-19 02:45:34.627495 fissure_engine-0.1.9/fissure_engine/
--rw-rw-rw-   0        0        0    77055 2022-11-19 02:45:11.000000 fissure_engine-0.1.9/fissure_engine/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-19 02:45:34.630774 fissure_engine-0.1.9/fissure_engine.egg-info/
--rw-rw-rw-   0        0        0      446 2022-11-19 02:45:34.000000 fissure_engine-0.1.9/fissure_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2022-11-19 02:45:34.000000 fissure_engine-0.1.9/fissure_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-19 02:45:34.000000 fissure_engine-0.1.9/fissure_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2022-11-19 02:45:34.000000 fissure_engine-0.1.9/fissure_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-19 02:45:34.632774 fissure_engine-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      706 2022-11-19 02:45:27.000000 fissure_engine-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:18:15.793820 fissure_engine-1.0.0/
+-rw-rw-rw-   0        0        0      387 2024-04-05 16:18:15.792820 fissure_engine-1.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-05 16:18:15.791812 fissure_engine-1.0.0/fissure_engine.egg-info/
+-rw-rw-rw-   0        0        0      387 2024-04-05 16:18:15.000000 fissure_engine-1.0.0/fissure_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      160 2024-04-05 16:18:15.000000 fissure_engine-1.0.0/fissure_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 16:18:15.000000 fissure_engine-1.0.0/fissure_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 16:18:15.000000 fissure_engine-1.0.0/fissure_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 16:18:15.793820 fissure_engine-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      706 2024-04-05 16:16:31.000000 fissure_engine-1.0.0/setup.py
```

### Comparing `fissure_engine-0.1.9/setup.py` & `fissure_engine-1.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.9'
+VERSION = '1.0.0'
 DESCRIPTION = 'Engine for getting fissure information in Warframe.'
 LONG_DESCRIPTION = 'Engine for getting the current fissures for Warframe in a dictionary object.'
 
 setup(
         name="fissure_engine", 
         version=VERSION,
         author="Jacob McBride",
```

