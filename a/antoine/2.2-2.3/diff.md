# Comparing `tmp/antoine-2.2.tar.gz` & `tmp/antoine-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antoine-2.2.tar", last modified: Thu Apr  4 14:16:17 2024, max compression
+gzip compressed data, was "antoine-2.3.tar", last modified: Fri Apr  5 10:44:37 2024, max compression
```

## Comparing `antoine-2.2.tar` & `antoine-2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-04 14:16:17.368515 antoine-2.2/
--rw-r--r--   0 antoinebertin   (501) staff       (20)      206 2024-04-04 14:16:17.368329 antoine-2.2/PKG-INFO
--rw-r--r--   0 antoinebertin   (501) staff       (20)      260 2024-04-04 14:01:11.000000 antoine-2.2/README.md
-drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-04 14:16:17.367487 antoine-2.2/antoine/
--rw-r--r--   0 antoinebertin   (501) staff       (20)       42 2024-04-04 12:03:26.000000 antoine-2.2/antoine/__init__.py
--rw-r--r--   0 antoinebertin   (501) staff       (20)     1443 2024-04-04 13:08:46.000000 antoine-2.2/antoine/app.py
-drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-04 14:16:17.368128 antoine-2.2/antoine.egg-info/
--rw-r--r--   0 antoinebertin   (501) staff       (20)      206 2024-04-04 14:16:17.000000 antoine-2.2/antoine.egg-info/PKG-INFO
--rw-r--r--   0 antoinebertin   (501) staff       (20)      211 2024-04-04 14:16:17.000000 antoine-2.2/antoine.egg-info/SOURCES.txt
--rw-r--r--   0 antoinebertin   (501) staff       (20)        1 2024-04-04 14:16:17.000000 antoine-2.2/antoine.egg-info/dependency_links.txt
--rw-r--r--   0 antoinebertin   (501) staff       (20)       49 2024-04-04 14:16:17.000000 antoine-2.2/antoine.egg-info/entry_points.txt
--rw-r--r--   0 antoinebertin   (501) staff       (20)        8 2024-04-04 14:16:17.000000 antoine-2.2/antoine.egg-info/top_level.txt
--rw-r--r--   0 antoinebertin   (501) staff       (20)       38 2024-04-04 14:16:17.368553 antoine-2.2/setup.cfg
--rw-r--r--   0 antoinebertin   (501) staff       (20)      573 2024-04-04 14:13:04.000000 antoine-2.2/setup.py
+drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-05 10:44:37.344009 antoine-2.3/
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      206 2024-04-05 10:44:37.343799 antoine-2.3/PKG-INFO
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      261 2024-04-05 10:43:11.000000 antoine-2.3/README.md
+drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-05 10:44:37.342919 antoine-2.3/antoine/
+-rw-r--r--   0 antoinebertin   (501) staff       (20)       42 2024-04-04 12:03:26.000000 antoine-2.3/antoine/__init__.py
+-rw-r--r--   0 antoinebertin   (501) staff       (20)     2425 2024-04-05 10:41:40.000000 antoine-2.3/antoine/app.py
+drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-05 10:44:37.343578 antoine-2.3/antoine.egg-info/
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      206 2024-04-05 10:44:37.000000 antoine-2.3/antoine.egg-info/PKG-INFO
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      211 2024-04-05 10:44:37.000000 antoine-2.3/antoine.egg-info/SOURCES.txt
+-rw-r--r--   0 antoinebertin   (501) staff       (20)        1 2024-04-05 10:44:37.000000 antoine-2.3/antoine.egg-info/dependency_links.txt
+-rw-r--r--   0 antoinebertin   (501) staff       (20)       50 2024-04-05 10:44:37.000000 antoine-2.3/antoine.egg-info/entry_points.txt
+-rw-r--r--   0 antoinebertin   (501) staff       (20)        8 2024-04-05 10:44:37.000000 antoine-2.3/antoine.egg-info/top_level.txt
+-rw-r--r--   0 antoinebertin   (501) staff       (20)       38 2024-04-05 10:44:37.344050 antoine-2.3/setup.cfg
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      574 2024-04-05 09:43:39.000000 antoine-2.3/setup.py
```

### Comparing `antoine-2.2/setup.py` & `antoine-2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 setup(
     name='antoine',
-    version='2.2',
+    version='2.3',
     packages=['antoine'],  # 'antoine' is the name of the package
     author='Antoine Bertin',
     author_email='monolok35@gmail.com',
     description='Hiring Antoine is so much fun!',
     url='https://github.com/monolok/antoine/',
     license='MIT',
     entry_points={
         'console_scripts': [
-            'hireantoine=antoine.app:main',  # 'antoine' is the name of the package and 'app.py' contains a function 'main'
+            'hire_antoine=antoine.app:main',  # 'antoine' is the name of the package and 'app.py' contains a function 'main'
         ],
     },
     include_package_data=True,
     install_requires=[]
 )
```

