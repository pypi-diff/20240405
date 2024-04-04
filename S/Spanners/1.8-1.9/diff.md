# Comparing `tmp/Spanners-1.8.tar.gz` & `tmp/Spanners-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Spanners-1.8.tar", last modified: Mon Apr  6 23:33:08 2020, max compression
+gzip compressed data, was "dist/Spanners-1.9.tar", last modified: Sun Apr 12 10:46:51 2020, max compression
```

## Comparing `Spanners-1.8.tar` & `Spanners-1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 dave       (502) staff       (20)        0 2020-04-06 23:33:07.996016 Spanners-1.8/
--rw-r--r--   0 dave       (502) staff       (20)      646 2020-04-06 23:33:07.996288 Spanners-1.8/PKG-INFO
--rw-r--r--   0 dave       (502) staff       (20)      205 2020-03-11 08:16:38.000000 Spanners-1.8/README.md
-drwxr-xr-x   0 dave       (502) staff       (20)        0 2020-04-06 23:33:07.911998 Spanners-1.8/Spanners/
--rwxr-xr-x   0 dave       (502) staff       (20)     1959 2020-03-26 04:04:50.000000 Spanners-1.8/Spanners/Downloader.py
--rwxr-xr-x   0 dave       (502) staff       (20)      292 2020-03-26 03:35:54.000000 Spanners-1.8/Spanners/Errors.py
--rwxr-xr-x   0 dave       (502) staff       (20)     1926 2020-03-26 03:35:54.000000 Spanners-1.8/Spanners/Executor.py
--rwxr-xr-x   0 dave       (502) staff       (20)     1353 2020-03-26 03:35:54.000000 Spanners-1.8/Spanners/GoogleMaps.py
--rwxr-xr-x   0 dave       (502) staff       (20)     1164 2020-03-26 04:18:11.000000 Spanners-1.8/Spanners/IdentityCache.py
--rwxr-xr-x   0 dave       (502) staff       (20)     5366 2020-03-26 03:35:54.000000 Spanners-1.8/Spanners/Squirrel.py
--rwxr-xr-x   0 dave       (502) staff       (20)     4166 2020-04-06 23:32:49.000000 Spanners-1.8/Spanners/Treeify.py
--rwxr-xr-x   0 dave       (502) staff       (20)       24 2020-03-26 03:35:54.000000 Spanners-1.8/Spanners/__init__.py
-drwxr-xr-x   0 dave       (502) staff       (20)        0 2020-04-06 23:33:07.915359 Spanners-1.8/Spanners.egg-info/
--rw-r--r--   0 dave       (502) staff       (20)      646 2020-04-06 23:33:05.000000 Spanners-1.8/Spanners.egg-info/PKG-INFO
--rw-r--r--   0 dave       (502) staff       (20)      392 2020-04-06 23:33:05.000000 Spanners-1.8/Spanners.egg-info/SOURCES.txt
--rw-r--r--   0 dave       (502) staff       (20)        1 2020-04-06 23:33:05.000000 Spanners-1.8/Spanners.egg-info/dependency_links.txt
--rw-r--r--   0 dave       (502) staff       (20)       66 2020-04-06 23:33:05.000000 Spanners-1.8/Spanners.egg-info/requires.txt
--rw-r--r--   0 dave       (502) staff       (20)        9 2020-04-06 23:33:05.000000 Spanners-1.8/Spanners.egg-info/top_level.txt
-drwxr-xr-x   0 dave       (502) staff       (20)        0 2020-04-06 23:33:07.995522 Spanners-1.8/bin/
--rwxr-xr-x   0 dave       (502) staff       (20)     1009 2020-03-26 03:35:54.000000 Spanners-1.8/bin/squirrel.py
--rwxr-xr-x   0 dave       (502) staff       (20)     3514 2020-03-26 03:35:54.000000 Spanners-1.8/bin/treeify.py
--rw-r--r--   0 dave       (502) staff       (20)       79 2020-04-06 23:33:07.996991 Spanners-1.8/setup.cfg
--rwxr-xr-x   0 dave       (502) staff       (20)      860 2020-04-06 23:32:49.000000 Spanners-1.8/setup.py
+drwxr-xr-x   0 dave       (502) staff       (20)        0 2020-04-12 10:46:51.727811 Spanners-1.9/
+-rw-r--r--   0 dave       (502) staff       (20)      646 2020-04-12 10:46:51.727989 Spanners-1.9/PKG-INFO
+-rw-r--r--   0 dave       (502) staff       (20)      205 2020-03-11 08:16:38.000000 Spanners-1.9/README.md
+drwxr-xr-x   0 dave       (502) staff       (20)        0 2020-04-12 10:46:51.645312 Spanners-1.9/Spanners/
+-rwxr-xr-x   0 dave       (502) staff       (20)     1959 2020-03-26 04:04:50.000000 Spanners-1.9/Spanners/Downloader.py
+-rwxr-xr-x   0 dave       (502) staff       (20)      292 2020-03-26 03:35:54.000000 Spanners-1.9/Spanners/Errors.py
+-rwxr-xr-x   0 dave       (502) staff       (20)     1926 2020-03-26 03:35:54.000000 Spanners-1.9/Spanners/Executor.py
+-rwxr-xr-x   0 dave       (502) staff       (20)     1353 2020-03-26 03:35:54.000000 Spanners-1.9/Spanners/GoogleMaps.py
+-rwxr-xr-x   0 dave       (502) staff       (20)     1164 2020-03-26 04:18:11.000000 Spanners-1.9/Spanners/IdentityCache.py
+-rwxr-xr-x   0 dave       (502) staff       (20)     5366 2020-03-26 03:35:54.000000 Spanners-1.9/Spanners/Squirrel.py
+-rwxr-xr-x   0 dave       (502) staff       (20)     4179 2020-04-12 10:46:18.000000 Spanners-1.9/Spanners/Treeify.py
+-rwxr-xr-x   0 dave       (502) staff       (20)       24 2020-03-26 03:35:54.000000 Spanners-1.9/Spanners/__init__.py
+drwxr-xr-x   0 dave       (502) staff       (20)        0 2020-04-12 10:46:51.648026 Spanners-1.9/Spanners.egg-info/
+-rw-r--r--   0 dave       (502) staff       (20)      646 2020-04-12 10:46:49.000000 Spanners-1.9/Spanners.egg-info/PKG-INFO
+-rw-r--r--   0 dave       (502) staff       (20)      392 2020-04-12 10:46:49.000000 Spanners-1.9/Spanners.egg-info/SOURCES.txt
+-rw-r--r--   0 dave       (502) staff       (20)        1 2020-04-12 10:46:49.000000 Spanners-1.9/Spanners.egg-info/dependency_links.txt
+-rw-r--r--   0 dave       (502) staff       (20)       66 2020-04-12 10:46:49.000000 Spanners-1.9/Spanners.egg-info/requires.txt
+-rw-r--r--   0 dave       (502) staff       (20)        9 2020-04-12 10:46:49.000000 Spanners-1.9/Spanners.egg-info/top_level.txt
+drwxr-xr-x   0 dave       (502) staff       (20)        0 2020-04-12 10:46:51.727333 Spanners-1.9/bin/
+-rwxr-xr-x   0 dave       (502) staff       (20)     1009 2020-03-26 03:35:54.000000 Spanners-1.9/bin/squirrel.py
+-rwxr-xr-x   0 dave       (502) staff       (20)     3514 2020-03-26 03:35:54.000000 Spanners-1.9/bin/treeify.py
+-rw-r--r--   0 dave       (502) staff       (20)       79 2020-04-12 10:46:51.728742 Spanners-1.9/setup.cfg
+-rwxr-xr-x   0 dave       (502) staff       (20)      860 2020-04-12 10:46:34.000000 Spanners-1.9/setup.py
```

### Comparing `Spanners-1.8/PKG-INFO` & `Spanners-1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: Spanners
-Version: 1.8
+Version: 1.9
 Summary: UNKNOWN
 Home-page: https://github.com/eddo888/Spanners
 Author: David Edson
 Author-email: eddo888@tpg.com.au
 License: MIT
-Download-URL: https://github.com/eddo888/Spanners/archive/1.8.tar.gz
+Download-URL: https://github.com/eddo888/Spanners/archive/1.9.tar.gz
 Description: # toolbox of goodies
         
         ## squirrel.py
         
         simple commandline wrapper around credstash
         
         ## treeify.py
```

### Comparing `Spanners-1.8/Spanners/Downloader.py` & `Spanners-1.9/Spanners/Downloader.py`

 * *Files identical despite different names*

### Comparing `Spanners-1.8/Spanners/Executor.py` & `Spanners-1.9/Spanners/Executor.py`

 * *Files identical despite different names*

### Comparing `Spanners-1.8/Spanners/GoogleMaps.py` & `Spanners-1.9/Spanners/GoogleMaps.py`

 * *Files identical despite different names*

### Comparing `Spanners-1.8/Spanners/IdentityCache.py` & `Spanners-1.9/Spanners/IdentityCache.py`

 * *Files identical despite different names*

### Comparing `Spanners-1.8/Spanners/Squirrel.py` & `Spanners-1.9/Spanners/Squirrel.py`

 * *Files identical despite different names*

### Comparing `Spanners-1.8/Spanners/Treeify.py` & `Spanners-1.9/Spanners/Treeify.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 				new[key] = self.treeFix(node[n])
 			return new
 		if type(node) in [dict, OD]:
 			for key in list(node.keys()):
 				tipe = type(node[key])
 				value = self.treeFix(node[key])
 				del node[key]
-				if key[0] in ['@', '#']:
+				if len(key) and key[0] in ['@', '#']:
 					node[''.join([self.colours.Green, key, self.colours.Off])] = value
 				else:
 					if tipe in self.fundamentals:
 						parts = [self.colours.Green]
 					else:
 						parts = [self.colours.Teal]
 					parts += [key, self.colours.Off]
```

### Comparing `Spanners-1.8/Spanners.egg-info/PKG-INFO` & `Spanners-1.9/Spanners.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: Spanners
-Version: 1.8
+Version: 1.9
 Summary: UNKNOWN
 Home-page: https://github.com/eddo888/Spanners
 Author: David Edson
 Author-email: eddo888@tpg.com.au
 License: MIT
-Download-URL: https://github.com/eddo888/Spanners/archive/1.8.tar.gz
+Download-URL: https://github.com/eddo888/Spanners/archive/1.9.tar.gz
 Description: # toolbox of goodies
         
         ## squirrel.py
         
         simple commandline wrapper around credstash
         
         ## treeify.py
```

### Comparing `Spanners-1.8/bin/squirrel.py` & `Spanners-1.9/bin/squirrel.py`

 * *Files identical despite different names*

### Comparing `Spanners-1.8/bin/treeify.py` & `Spanners-1.9/bin/treeify.py`

 * *Files identical despite different names*

### Comparing `Spanners-1.8/setup.py` & `Spanners-1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 from setuptools import setup
 
 pwd = path.abspath(path.dirname(__file__))
 with codecs.open(path.join(pwd, 'README.md'), 'r', encoding='utf8') as input:
     long_description = input.read()
 
-version='1.8'
+version='1.9'
 	
 setup(
 	name='Spanners',
 	version=version,
 	license='MIT',
     long_description=long_description,
 	long_description_content_type="text/markdown",
```

