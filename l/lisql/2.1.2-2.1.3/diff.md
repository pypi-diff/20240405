# Comparing `tmp/lisql-2.1.2.tar.gz` & `tmp/lisql-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lisql-2.1.2.tar", last modified: Mon Sep 18 18:37:21 2023, max compression
+gzip compressed data, was "lisql-2.1.3.tar", last modified: Fri Apr  5 12:30:24 2024, max compression
```

## Comparing `lisql-2.1.2.tar` & `lisql-2.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 li         (501) staff       (20)        0 2023-09-18 18:37:21.213875 lisql-2.1.2/
--rw-r--r--   0 li         (501) staff       (20)     1068 2023-09-18 16:51:59.000000 lisql-2.1.2/LICENSE
--rw-r--r--   0 li         (501) staff       (20)    18999 2023-09-18 18:37:21.213957 lisql-2.1.2/PKG-INFO
--rw-r--r--   0 li         (501) staff       (20)    18180 2023-09-18 17:41:56.000000 lisql-2.1.2/README.md
--rw-r--r--   0 li         (501) staff       (20)      103 2023-09-18 17:41:59.000000 lisql-2.1.2/pyproject.toml
--rw-r--r--   0 li         (501) staff       (20)      644 2023-09-18 18:37:21.214264 lisql-2.1.2/setup.cfg
--rw-r--r--   0 li         (501) staff       (20)      725 2023-09-18 17:41:13.000000 lisql-2.1.2/setup.py
-drwxr-xr-x   0 li         (501) staff       (20)        0 2023-09-18 18:37:21.213265 lisql-2.1.2/src/
-drwxr-xr-x   0 li         (501) staff       (20)        0 2023-09-18 18:37:21.213776 lisql-2.1.2/src/lisql.egg-info/
--rw-r--r--   0 li         (501) staff       (20)    18999 2023-09-18 18:37:20.000000 lisql-2.1.2/src/lisql.egg-info/PKG-INFO
--rw-r--r--   0 li         (501) staff       (20)      196 2023-09-18 18:37:21.000000 lisql-2.1.2/src/lisql.egg-info/SOURCES.txt
--rw-r--r--   0 li         (501) staff       (20)        1 2023-09-18 18:37:20.000000 lisql-2.1.2/src/lisql.egg-info/dependency_links.txt
--rw-r--r--   0 li         (501) staff       (20)        6 2023-09-18 18:37:21.000000 lisql-2.1.2/src/lisql.egg-info/top_level.txt
--rw-r--r--   0 li         (501) staff       (20)    22742 2023-09-18 18:37:01.000000 lisql-2.1.2/src/lisql.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2024-04-05 12:30:24.346324 lisql-2.1.3/
+-rw-r--r--   0 li         (501) staff       (20)     1068 2024-04-05 11:57:55.000000 lisql-2.1.3/LICENSE
+-rw-r--r--   0 li         (501) staff       (20)    18962 2024-04-05 12:30:24.346138 lisql-2.1.3/PKG-INFO
+-rw-r--r--   0 li         (501) staff       (20)    18180 2024-04-05 11:57:55.000000 lisql-2.1.3/README.md
+-rw-r--r--   0 li         (501) staff       (20)      103 2024-04-05 11:57:55.000000 lisql-2.1.3/pyproject.toml
+-rw-r--r--   0 li         (501) staff       (20)      644 2024-04-05 12:30:24.346704 lisql-2.1.3/setup.cfg
+-rw-r--r--   0 li         (501) staff       (20)      725 2024-04-05 12:09:19.000000 lisql-2.1.3/setup.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2024-04-05 12:30:24.344795 lisql-2.1.3/src/
+drwxr-xr-x   0 li         (501) staff       (20)        0 2024-04-05 12:30:24.345820 lisql-2.1.3/src/lisql.egg-info/
+-rw-r--r--   0 li         (501) staff       (20)    18962 2024-04-05 12:30:24.000000 lisql-2.1.3/src/lisql.egg-info/PKG-INFO
+-rw-r--r--   0 li         (501) staff       (20)      196 2024-04-05 12:30:24.000000 lisql-2.1.3/src/lisql.egg-info/SOURCES.txt
+-rw-r--r--   0 li         (501) staff       (20)        1 2024-04-05 12:30:24.000000 lisql-2.1.3/src/lisql.egg-info/dependency_links.txt
+-rw-r--r--   0 li         (501) staff       (20)        6 2024-04-05 12:30:24.000000 lisql-2.1.3/src/lisql.egg-info/top_level.txt
+-rw-r--r--   0 li         (501) staff       (20)    22742 2024-04-05 11:57:55.000000 lisql-2.1.3/src/lisql.py
```

### Comparing `lisql-2.1.2/LICENSE` & `lisql-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lisql-2.1.2/PKG-INFO` & `lisql-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: lisql
-Version: 2.1.2
+Version: 2.1.3
 Summary: Provides simple funtions to interact with MySQL databases and tables.
 Home-page: https://github.com/li812/lisql
 Author: Ali Ahammad
 Author-email: aliahammad0812@outlook.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/li812/lisql/issues
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -570,9 +568,7 @@
 
 ## Contact
 stions, bug reports, or feedback, please feel free to contact the developers via:
 ### Email: aliahammad0812@outlook.com 
 
 ### Instagram: https://www.instagram.com/the_raptor_rider_/ 
 
-
-
```

### Comparing `lisql-2.1.2/README.md` & `lisql-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `lisql-2.1.2/setup.cfg` & `lisql-2.1.3/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lisql
-version = 2.1.2
+version = 2.1.3
 author = Ali Ahammad
 author_email = aliahammad0812@outlook.com
 description = Provides a simple interface to interact with MySQL databases.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/li812/lisql
 project_urls =
```

### Comparing `lisql-2.1.2/setup.py` & `lisql-2.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='lisql',
-    version='2.1.2',
+    version='2.1.3',
     py_modules=['lisql'],
     description='Provides simple funtions to interact with MySQL databases and tables.',
     author='Ali Ahammad',
     author_email='aliahammad0812@outlook.com',
     url='https://github.com/li812/lisql',
     classifiers=[
         'License :: OSI Approved :: MIT License',
```

### Comparing `lisql-2.1.2/src/lisql.egg-info/PKG-INFO` & `lisql-2.1.3/src/lisql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: lisql
-Version: 2.1.2
+Version: 2.1.3
 Summary: Provides simple funtions to interact with MySQL databases and tables.
 Home-page: https://github.com/li812/lisql
 Author: Ali Ahammad
 Author-email: aliahammad0812@outlook.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/li812/lisql/issues
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -570,9 +568,7 @@
 
 ## Contact
 stions, bug reports, or feedback, please feel free to contact the developers via:
 ### Email: aliahammad0812@outlook.com 
 
 ### Instagram: https://www.instagram.com/the_raptor_rider_/ 
 
-
-
```

### Comparing `lisql-2.1.2/src/lisql.py` & `lisql-2.1.3/src/lisql.py`

 * *Files identical despite different names*

