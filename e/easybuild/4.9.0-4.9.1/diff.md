# Comparing `tmp/easybuild-4.9.0.tar.gz` & `tmp/easybuild-4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easybuild-4.9.0.tar", last modified: Sat Dec 30 20:55:30 2023, max compression
+gzip compressed data, was "easybuild-4.9.1.tar", last modified: Fri Apr  5 08:32:30 2024, max compression
```

## Comparing `easybuild-4.9.0.tar` & `easybuild-4.9.1.tar`

### file list

```diff
@@ -1,6 +1,13 @@
-drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2023-12-30 20:55:30.389677 easybuild-4.9.0/
--rw-r--r--   0 kehoste    (501) staff       (20)    18092 2022-10-21 08:06:35.751435 easybuild-4.9.0/LICENSE
--rw-r--r--   0 kehoste    (501) staff       (20)     6905 2023-12-30 20:55:30.389730 easybuild-4.9.0/PKG-INFO
--rw-r--r--   0 kehoste    (501) staff       (20)     4538 2023-10-29 20:07:52.592501 easybuild-4.9.0/README.rst
--rw-r--r--   0 kehoste    (501) staff       (20)       31 2022-10-21 08:06:35.795029 easybuild-4.9.0/setup.cfg
--rw-r--r--   0 kehoste    (501) staff       (20)     3502 2023-12-30 20:55:04.585824 easybuild-4.9.0/setup.py
+drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2024-04-05 08:32:30.647655 easybuild-4.9.1/
+-rw-r--r--   0 kehoste    (501) staff       (20)    18092 2022-10-21 08:06:35.000000 easybuild-4.9.1/LICENSE
+-rw-r--r--   0 kehoste    (501) staff       (20)       52 2022-10-21 08:06:35.000000 easybuild-4.9.1/MANIFEST.in
+-rw-r--r--   0 kehoste    (501) staff       (20)     6131 2024-04-05 08:32:30.647581 easybuild-4.9.1/PKG-INFO
+-rw-r--r--   0 kehoste    (501) staff       (20)     4538 2023-10-29 20:07:52.000000 easybuild-4.9.1/README.rst
+drwxr-xr-x   0 kehoste    (501) staff       (20)        0 2024-04-05 08:32:30.647203 easybuild-4.9.1/easybuild.egg-info/
+-rw-r--r--   0 kehoste    (501) staff       (20)     6131 2024-04-05 08:32:30.000000 easybuild-4.9.1/easybuild.egg-info/PKG-INFO
+-rw-r--r--   0 kehoste    (501) staff       (20)      213 2024-04-05 08:32:30.000000 easybuild-4.9.1/easybuild.egg-info/SOURCES.txt
+-rw-r--r--   0 kehoste    (501) staff       (20)        1 2024-04-05 08:32:30.000000 easybuild-4.9.1/easybuild.egg-info/dependency_links.txt
+-rw-r--r--   0 kehoste    (501) staff       (20)       84 2024-04-05 08:32:30.000000 easybuild-4.9.1/easybuild.egg-info/requires.txt
+-rw-r--r--   0 kehoste    (501) staff       (20)        5 2024-04-05 08:32:30.000000 easybuild-4.9.1/easybuild.egg-info/top_level.txt
+-rw-r--r--   0 kehoste    (501) staff       (20)       70 2024-04-05 08:32:30.647985 easybuild-4.9.1/setup.cfg
+-rw-r--r--   0 kehoste    (501) staff       (20)     3502 2024-04-05 08:32:15.000000 easybuild-4.9.1/setup.py
```

### Comparing `easybuild-4.9.0/LICENSE` & `easybuild-4.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easybuild-4.9.0/README.rst` & `easybuild-4.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `easybuild-4.9.0/setup.py` & `easybuild-4.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 import os
 from distutils import log
 from distutils.core import setup
 
 # note: release candidates should be versioned as a pre-release, e.g. "1.1rc1"
 # 1.1-rc1 would indicate a post-release, i.e., and update of 1.1, so beware
-VERSION = '4.9.0'
+VERSION = '4.9.1'
 
 
 # Utility function to read README file
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
```

