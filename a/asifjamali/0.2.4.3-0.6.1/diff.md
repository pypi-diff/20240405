# Comparing `tmp/asifjamali-0.2.4.3.tar.gz` & `tmp/asifjamali-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asifjamali-0.2.4.3.tar", last modified: Thu Mar 21 15:12:24 2024, max compression
+gzip compressed data, was "asifjamali-0.6.1.tar", last modified: Fri Apr  5 16:09:22 2024, max compression
```

## Comparing `asifjamali-0.2.4.3.tar` & `asifjamali-0.6.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 15:12:24.537394 asifjamali-0.2.4.3/
--rw-r--r--   0 root         (0) root         (0)     1056 2024-03-14 23:59:10.000000 asifjamali-0.2.4.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1477 2024-03-21 15:12:24.537394 asifjamali-0.2.4.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1105 2024-03-14 23:59:10.000000 asifjamali-0.2.4.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 15:12:24.533394 asifjamali-0.2.4.3/asifjamali/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-15 00:00:14.000000 asifjamali-0.2.4.3/asifjamali/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11819 2024-03-21 15:11:51.000000 asifjamali-0.2.4.3/asifjamali/musibat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 15:12:24.537394 asifjamali-0.2.4.3/asifjamali.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1477 2024-03-21 15:12:24.000000 asifjamali-0.2.4.3/asifjamali.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      240 2024-03-21 15:12:24.000000 asifjamali-0.2.4.3/asifjamali.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-21 15:12:24.000000 asifjamali-0.2.4.3/asifjamali.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-03-21 15:12:24.000000 asifjamali-0.2.4.3/asifjamali.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-03-21 15:12:24.000000 asifjamali-0.2.4.3/asifjamali.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-21 15:12:24.537394 asifjamali-0.2.4.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      642 2024-03-21 15:11:02.000000 asifjamali-0.2.4.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:09:22.080527 asifjamali-0.6.1/
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-04-05 12:59:12.000000 asifjamali-0.6.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1475 2024-04-05 16:09:22.080527 asifjamali-0.6.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1105 2024-04-05 12:59:12.000000 asifjamali-0.6.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:09:22.080527 asifjamali-0.6.1/asifjamali/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-05 12:59:12.000000 asifjamali-0.6.1/asifjamali/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19974 2024-04-05 12:59:12.000000 asifjamali-0.6.1/asifjamali/musibat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:09:22.080527 asifjamali-0.6.1/asifjamali.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1475 2024-04-05 16:09:22.000000 asifjamali-0.6.1/asifjamali.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      240 2024-04-05 16:09:22.000000 asifjamali-0.6.1/asifjamali.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 16:09:22.000000 asifjamali-0.6.1/asifjamali.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-05 16:09:22.000000 asifjamali-0.6.1/asifjamali.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-05 16:09:22.000000 asifjamali-0.6.1/asifjamali.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 16:09:22.080527 asifjamali-0.6.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      640 2024-04-05 12:59:12.000000 asifjamali-0.6.1/setup.py
```

### Comparing `asifjamali-0.2.4.3/LICENSE` & `asifjamali-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asifjamali-0.2.4.3/PKG-INFO` & `asifjamali-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asifjamali
-Version: 0.2.4.3
+Version: 0.6.1
 Summary: Team Musibat Bots
 Home-page: https://bitbucket.org/shahzain83/musibat
 Author: Shahzain Khan
 Author-email: technomusibat@hotmail.com
 License: MIT
 Project-URL: Bug Tracker, https://bitbucket.org/shahzain83/musibat/issues
 Description-Content-Type: text/markdown
```

### Comparing `asifjamali-0.2.4.3/README.md` & `asifjamali-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `asifjamali-0.2.4.3/asifjamali.egg-info/PKG-INFO` & `asifjamali-0.6.1/asifjamali.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asifjamali
-Version: 0.2.4.3
+Version: 0.6.1
 Summary: Team Musibat Bots
 Home-page: https://bitbucket.org/shahzain83/musibat
 Author: Shahzain Khan
 Author-email: technomusibat@hotmail.com
 License: MIT
 Project-URL: Bug Tracker, https://bitbucket.org/shahzain83/musibat/issues
 Description-Content-Type: text/markdown
```

### Comparing `asifjamali-0.2.4.3/setup.py` & `asifjamali-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='asifjamali',
-    version='0.2.4.3',
+    version='0.6.1',
     author='Shahzain Khan',
     author_email='technomusibat@hotmail.com',
     description='Team Musibat Bots',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://bitbucket.org/shahzain83/musibat',
     project_urls = {
```

