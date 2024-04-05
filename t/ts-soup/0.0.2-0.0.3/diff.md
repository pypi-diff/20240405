# Comparing `tmp/ts-soup-0.0.2.tar.gz` & `tmp/ts-soup-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\PythonProjects\load_predict\syncdbs_new\dist\.tmp-qsev1_yt\ts-soup-0.0.2.tar", last modified: Fri Apr  5 12:34:15 2024, max compression
+gzip compressed data, was "D:\PythonProjects\load_predict\syncdbs_new\dist\.tmp-a23bktse\ts-soup-0.0.3.tar", last modified: Fri Apr  5 12:51:14 2024, max compression
```

## Comparing `ts-soup-0.0.2.tar` & `ts-soup-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 12:34:15.668506 ts-soup-0.0.2/
--rw-rw-rw-   0        0        0     1028 2024-04-05 12:34:15.667504 ts-soup-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      686 2024-04-05 12:25:36.000000 ts-soup-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-05 12:34:15.668506 ts-soup-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      605 2024-04-05 12:34:09.000000 ts-soup-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:34:15.659505 ts-soup-0.0.2/ts_soup/
--rw-rw-rw-   0        0        0      307 2024-04-05 10:42:41.000000 ts-soup-0.0.2/ts_soup/__init__.py
--rw-rw-rw-   0        0        0     1243 2024-04-05 11:35:42.000000 ts-soup-0.0.2/ts_soup/app.py
--rw-rw-rw-   0        0        0    18079 2024-04-05 12:15:49.000000 ts-soup-0.0.2/ts_soup/common.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:34:15.665503 ts-soup-0.0.2/ts_soup/workers/
--rw-rw-rw-   0        0        0       78 2024-04-05 04:01:53.000000 ts-soup-0.0.2/ts_soup/workers/__init__.py
--rw-rw-rw-   0        0        0     3689 2024-04-05 09:36:43.000000 ts-soup-0.0.2/ts_soup/workers/sources.py
--rw-rw-rw-   0        0        0     5793 2024-04-05 11:44:31.000000 ts-soup-0.0.2/ts_soup/workers/targets.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:34:15.666506 ts-soup-0.0.2/ts_soup.egg-info/
--rw-rw-rw-   0        0        0     1028 2024-04-05 12:34:15.000000 ts-soup-0.0.2/ts_soup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-04-05 12:34:15.000000 ts-soup-0.0.2/ts_soup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 12:34:15.000000 ts-soup-0.0.2/ts_soup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 12:34:15.000000 ts-soup-0.0.2/ts_soup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 12:51:14.217814 ts-soup-0.0.3/
+-rw-rw-rw-   0        0        0     1028 2024-04-05 12:51:14.216814 ts-soup-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2024-04-05 12:25:36.000000 ts-soup-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-05 12:51:14.217814 ts-soup-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      605 2024-04-05 12:51:11.000000 ts-soup-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:51:14.207862 ts-soup-0.0.3/ts_soup/
+-rw-rw-rw-   0        0        0      307 2024-04-05 10:42:41.000000 ts-soup-0.0.3/ts_soup/__init__.py
+-rw-rw-rw-   0        0        0     1393 2024-04-05 12:51:00.000000 ts-soup-0.0.3/ts_soup/app.py
+-rw-rw-rw-   0        0        0    18079 2024-04-05 12:15:49.000000 ts-soup-0.0.3/ts_soup/common.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:51:14.214802 ts-soup-0.0.3/ts_soup/workers/
+-rw-rw-rw-   0        0        0       78 2024-04-05 04:01:53.000000 ts-soup-0.0.3/ts_soup/workers/__init__.py
+-rw-rw-rw-   0        0        0     3689 2024-04-05 09:36:43.000000 ts-soup-0.0.3/ts_soup/workers/sources.py
+-rw-rw-rw-   0        0        0     5793 2024-04-05 11:44:31.000000 ts-soup-0.0.3/ts_soup/workers/targets.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:51:14.215815 ts-soup-0.0.3/ts_soup.egg-info/
+-rw-rw-rw-   0        0        0     1028 2024-04-05 12:51:14.000000 ts-soup-0.0.3/ts_soup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-04-05 12:51:14.000000 ts-soup-0.0.3/ts_soup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 12:51:14.000000 ts-soup-0.0.3/ts_soup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 12:51:14.000000 ts-soup-0.0.3/ts_soup.egg-info/top_level.txt
```

### Comparing `ts-soup-0.0.2/PKG-INFO` & `ts-soup-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-soup
-Version: 0.0.2
+Version: 0.0.3
 Summary: date series data synchronization
 Author: feihan ye
 Author-email: 445280206@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ts-soup-0.0.2/README.md` & `ts-soup-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ts-soup-0.0.2/setup.py` & `ts-soup-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r",encoding='utf8') as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="ts-soup",
-  version="0.0.2",
+  version="0.0.3",
   author="feihan ye",
   author_email="445280206@qq.com",
   description="date series data synchronization",
   long_description=long_description,
   long_description_content_type="text/markdown",
   # url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `ts-soup-0.0.2/ts_soup/common.py` & `ts-soup-0.0.3/ts_soup/common.py`

 * *Files identical despite different names*

### Comparing `ts-soup-0.0.2/ts_soup/workers/sources.py` & `ts-soup-0.0.3/ts_soup/workers/sources.py`

 * *Files identical despite different names*

### Comparing `ts-soup-0.0.2/ts_soup/workers/targets.py` & `ts-soup-0.0.3/ts_soup/workers/targets.py`

 * *Files identical despite different names*

### Comparing `ts-soup-0.0.2/ts_soup.egg-info/PKG-INFO` & `ts-soup-0.0.3/ts_soup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-soup
-Version: 0.0.2
+Version: 0.0.3
 Summary: date series data synchronization
 Author: feihan ye
 Author-email: 445280206@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

