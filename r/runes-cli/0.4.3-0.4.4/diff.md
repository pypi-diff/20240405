# Comparing `tmp/runes-cli-0.4.3.tar.gz` & `tmp/runes-cli-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runes-cli-0.4.3.tar", last modified: Wed Apr  3 23:45:31 2024, max compression
+gzip compressed data, was "runes-cli-0.4.4.tar", last modified: Fri Apr  5 20:52:38 2024, max compression
```

## Comparing `runes-cli-0.4.3.tar` & `runes-cli-0.4.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-03 23:45:31.867638 runes-cli-0.4.3/
--rw-r--r--   0 stevehiehn   (501) staff       (20)    35149 2024-03-13 17:06:20.000000 runes-cli-0.4.3/LICENSE
--rw-r--r--   0 stevehiehn   (501) staff       (20)     1341 2024-04-03 23:45:31.867490 runes-cli-0.4.3/PKG-INFO
--rw-r--r--   0 stevehiehn   (501) staff       (20)      960 2024-04-02 15:54:01.000000 runes-cli-0.4.3/README.md
--rw-r--r--   0 stevehiehn   (501) staff       (20)       38 2024-04-03 23:45:31.867679 runes-cli-0.4.3/setup.cfg
--rw-r--r--   0 stevehiehn   (501) staff       (20)      914 2024-04-03 23:41:58.000000 runes-cli-0.4.3/setup.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-03 23:45:31.862758 runes-cli-0.4.3/src/
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-03 23:45:31.866343 runes-cli-0.4.3/src/runes_cli/
--rw-r--r--   0 stevehiehn   (501) staff       (20)        0 2024-03-13 17:06:20.000000 runes-cli-0.4.3/src/runes_cli/__init__.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     6763 2024-04-03 15:55:07.000000 runes-cli-0.4.3/src/runes_cli/api.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     3157 2024-03-13 17:06:20.000000 runes-cli-0.4.3/src/runes_cli/builder.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)    32817 2024-04-03 23:34:15.000000 runes-cli-0.4.3/src/runes_cli/cli.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)      153 2024-04-02 22:18:02.000000 runes-cli-0.4.3/src/runes_cli/config.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     8827 2024-04-03 22:37:41.000000 runes-cli-0.4.3/src/runes_cli/containers.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     1554 2024-03-31 06:30:26.000000 runes-cli-0.4.3/src/runes_cli/file_uploader.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     2062 2024-04-03 16:26:46.000000 runes-cli-0.4.3/src/runes_cli/models.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     6187 2024-03-27 18:35:57.000000 runes-cli-0.4.3/src/runes_cli/persistence.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-03 23:45:31.867285 runes-cli-0.4.3/src/runes_cli.egg-info/
--rw-r--r--   0 stevehiehn   (501) staff       (20)     1341 2024-04-03 23:45:31.000000 runes-cli-0.4.3/src/runes_cli.egg-info/PKG-INFO
--rw-r--r--   0 stevehiehn   (501) staff       (20)      479 2024-04-03 23:45:31.000000 runes-cli-0.4.3/src/runes_cli.egg-info/SOURCES.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)        1 2024-04-03 23:45:31.000000 runes-cli-0.4.3/src/runes_cli.egg-info/dependency_links.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       45 2024-04-03 23:45:31.000000 runes-cli-0.4.3/src/runes_cli.egg-info/entry_points.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       50 2024-04-03 23:45:31.000000 runes-cli-0.4.3/src/runes_cli.egg-info/requires.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       10 2024-04-03 23:45:31.000000 runes-cli-0.4.3/src/runes_cli.egg-info/top_level.txt
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-05 20:52:38.683506 runes-cli-0.4.4/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    35149 2024-03-13 17:06:20.000000 runes-cli-0.4.4/LICENSE
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     1532 2024-04-05 20:52:38.683271 runes-cli-0.4.4/PKG-INFO
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      960 2024-04-02 15:54:01.000000 runes-cli-0.4.4/README.md
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       38 2024-04-05 20:52:38.683546 runes-cli-0.4.4/setup.cfg
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      957 2024-04-05 20:51:33.000000 runes-cli-0.4.4/setup.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-05 20:52:38.678771 runes-cli-0.4.4/src/
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-05 20:52:38.681870 runes-cli-0.4.4/src/runes_cli/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)        0 2024-03-13 17:06:20.000000 runes-cli-0.4.4/src/runes_cli/__init__.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     6763 2024-04-03 15:55:07.000000 runes-cli-0.4.4/src/runes_cli/api.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     3336 2024-04-05 01:29:42.000000 runes-cli-0.4.4/src/runes_cli/builder.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    32817 2024-04-03 23:34:15.000000 runes-cli-0.4.4/src/runes_cli/cli.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      153 2024-04-02 22:18:02.000000 runes-cli-0.4.4/src/runes_cli/config.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     8827 2024-04-03 22:37:41.000000 runes-cli-0.4.4/src/runes_cli/containers.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     1554 2024-03-31 06:30:26.000000 runes-cli-0.4.4/src/runes_cli/file_uploader.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     2062 2024-04-03 16:26:46.000000 runes-cli-0.4.4/src/runes_cli/models.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     6187 2024-03-27 18:35:57.000000 runes-cli-0.4.4/src/runes_cli/persistence.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-05 20:52:38.683040 runes-cli-0.4.4/src/runes_cli.egg-info/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     1532 2024-04-05 20:52:38.000000 runes-cli-0.4.4/src/runes_cli.egg-info/PKG-INFO
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      479 2024-04-05 20:52:38.000000 runes-cli-0.4.4/src/runes_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)        1 2024-04-05 20:52:38.000000 runes-cli-0.4.4/src/runes_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       45 2024-04-05 20:52:38.000000 runes-cli-0.4.4/src/runes_cli.egg-info/entry_points.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       71 2024-04-05 20:52:38.000000 runes-cli-0.4.4/src/runes_cli.egg-info/requires.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       10 2024-04-05 20:52:38.000000 runes-cli-0.4.4/src/runes_cli.egg-info/top_level.txt
```

### Comparing `runes-cli-0.4.3/LICENSE` & `runes-cli-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `runes-cli-0.4.3/PKG-INFO` & `runes-cli-0.4.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 Metadata-Version: 2.1
 Name: runes-cli
-Version: 0.4.3
+Version: 0.4.4
 Summary: A python CLI used to manage the Signals & Sorcery platform
 Author: Steve Hiehn
 Author-email: stevehiehn@gmail.com
 License: GPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp
+Requires-Dist: click
+Requires-Dist: cryptography
+Requires-Dist: docker
+Requires-Dist: questionary
+Requires-Dist: urllib3
+Requires-Dist: requests
+Requires-Dist: appdirs
 
 # Signals And Sorcery CLI
 A python CLI used to setup &amp; manage [Crucible Plugins](https://dawnet.tools/) remote scripts on MAC, LINUX and Servers
 
 ### Requirements:
 
 - ensure Python >= 3.x is installed
```

### Comparing `runes-cli-0.4.3/README.md` & `runes-cli-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `runes-cli-0.4.3/setup.py` & `runes-cli-0.4.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name="runes-cli",
-    version="0.4.3",
+    version="0.4.4",
     author="Steve Hiehn",
     author_email="stevehiehn@gmail.com",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     include_package_data=True,
     install_requires=[
+        "aiohttp",
         "click",
+        "cryptography",
         "docker",
         "questionary",
         "urllib3",
         "requests",
         "appdirs",
         # other dependencies
     ],
```

### Comparing `runes-cli-0.4.3/src/runes_cli/api.py` & `runes-cli-0.4.4/src/runes_cli/api.py`

 * *Files identical despite different names*

### Comparing `runes-cli-0.4.3/src/runes_cli/cli.py` & `runes-cli-0.4.4/src/runes_cli/cli.py`

 * *Files identical despite different names*

### Comparing `runes-cli-0.4.3/src/runes_cli/containers.py` & `runes-cli-0.4.4/src/runes_cli/containers.py`

 * *Files identical despite different names*

### Comparing `runes-cli-0.4.3/src/runes_cli/file_uploader.py` & `runes-cli-0.4.4/src/runes_cli/file_uploader.py`

 * *Files identical despite different names*

### Comparing `runes-cli-0.4.3/src/runes_cli/models.py` & `runes-cli-0.4.4/src/runes_cli/models.py`

 * *Files identical despite different names*

### Comparing `runes-cli-0.4.3/src/runes_cli/persistence.py` & `runes-cli-0.4.4/src/runes_cli/persistence.py`

 * *Files identical despite different names*

### Comparing `runes-cli-0.4.3/src/runes_cli.egg-info/PKG-INFO` & `runes-cli-0.4.4/src/runes_cli.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 Metadata-Version: 2.1
 Name: runes-cli
-Version: 0.4.3
+Version: 0.4.4
 Summary: A python CLI used to manage the Signals & Sorcery platform
 Author: Steve Hiehn
 Author-email: stevehiehn@gmail.com
 License: GPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp
+Requires-Dist: click
+Requires-Dist: cryptography
+Requires-Dist: docker
+Requires-Dist: questionary
+Requires-Dist: urllib3
+Requires-Dist: requests
+Requires-Dist: appdirs
 
 # Signals And Sorcery CLI
 A python CLI used to setup &amp; manage [Crucible Plugins](https://dawnet.tools/) remote scripts on MAC, LINUX and Servers
 
 ### Requirements:
 
 - ensure Python >= 3.x is installed
```

