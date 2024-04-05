# Comparing `tmp/integ-db-0.0.4.tar.gz` & `tmp/integ-db-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "integ-db-0.0.4.tar", last modified: Fri Apr  5 02:14:46 2024, max compression
+gzip compressed data, was "integ-db-0.0.5.tar", last modified: Fri Apr  5 03:18:37 2024, max compression
```

## Comparing `integ-db-0.0.4.tar` & `integ-db-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 02:14:46.558534 integ-db-0.0.4/
--rw-rw-rw-   0        0        0     1092 2024-04-04 23:49:32.000000 integ-db-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      887 2024-04-05 02:14:46.555543 integ-db-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      131 2024-04-05 00:55:13.000000 integ-db-0.0.4/README.md
--rw-rw-rw-   0        0        0      108 2024-04-05 00:16:37.000000 integ-db-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 02:14:46.559539 integ-db-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1041 2024-04-05 02:14:05.000000 integ-db-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 02:14:46.515491 integ-db-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 02:14:46.554535 integ-db-0.0.4/src/integ_db.egg-info/
--rw-rw-rw-   0        0        0      887 2024-04-05 02:14:46.000000 integ-db-0.0.4/src/integ_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2024-04-05 02:14:46.000000 integ-db-0.0.4/src/integ_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 02:14:46.000000 integ-db-0.0.4/src/integ_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-05 02:14:46.000000 integ-db-0.0.4/src/integ_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-05 02:14:46.000000 integ-db-0.0.4/src/integ_db.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 02:14:46.541543 integ-db-0.0.4/src/integrate/
--rw-rw-rw-   0        0        0        0 2024-04-05 01:40:47.000000 integ-db-0.0.4/src/integrate/__init__.py
--rw-rw-rw-   0        0        0      595 2024-04-05 02:13:53.000000 integ-db-0.0.4/src/integrate/integdb.py
-drwxrwxrwx   0        0        0        0 2024-04-05 02:14:46.552550 integ-db-0.0.4/src/integrate/module/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:13:56.000000 integ-db-0.0.4/src/integrate/module/__init__.py
--rw-rw-rw-   0        0        0     2344 2024-04-04 01:28:29.000000 integ-db-0.0.4/src/integrate/module/interface.py
--rw-rw-rw-   0        0        0     1096 2024-04-04 01:45:14.000000 integ-db-0.0.4/src/integrate/module/mariadb.py
--rw-rw-rw-   0        0        0      624 2024-04-04 01:45:26.000000 integ-db-0.0.4/src/integrate/module/mssql.py
--rw-rw-rw-   0        0        0     1193 2024-04-04 01:45:40.000000 integ-db-0.0.4/src/integrate/module/mysql.py
--rw-rw-rw-   0        0        0     1831 2024-04-04 01:45:59.000000 integ-db-0.0.4/src/integrate/module/sqlalchemy.py
+drwxrwxrwx   0        0        0        0 2024-04-05 03:18:37.188560 integ-db-0.0.5/
+-rw-rw-rw-   0        0        0     1092 2024-04-04 23:49:32.000000 integ-db-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      887 2024-04-05 03:18:37.186559 integ-db-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      131 2024-04-05 00:55:13.000000 integ-db-0.0.5/README.md
+-rw-rw-rw-   0        0        0      108 2024-04-05 00:16:37.000000 integ-db-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 03:18:37.188560 integ-db-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1041 2024-04-05 03:18:20.000000 integ-db-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 03:18:37.140014 integ-db-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 03:18:37.184681 integ-db-0.0.5/src/integ_db.egg-info/
+-rw-rw-rw-   0        0        0      887 2024-04-05 03:18:37.000000 integ-db-0.0.5/src/integ_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2024-04-05 03:18:37.000000 integ-db-0.0.5/src/integ_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 03:18:37.000000 integ-db-0.0.5/src/integ_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-05 03:18:37.000000 integ-db-0.0.5/src/integ_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 03:18:37.000000 integ-db-0.0.5/src/integ_db.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 03:18:37.169061 integ-db-0.0.5/src/integdb/
+-rw-rw-rw-   0        0        0       34 2024-04-05 03:16:38.000000 integ-db-0.0.5/src/integdb/__init__.py
+-rw-rw-rw-   0        0        0      599 2024-04-05 02:30:35.000000 integ-db-0.0.5/src/integdb/controller.py
+drwxrwxrwx   0        0        0        0 2024-04-05 03:18:37.182541 integ-db-0.0.5/src/integdb/module/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:13:56.000000 integ-db-0.0.5/src/integdb/module/__init__.py
+-rw-rw-rw-   0        0        0     2344 2024-04-04 01:28:29.000000 integ-db-0.0.5/src/integdb/module/interface.py
+-rw-rw-rw-   0        0        0     1096 2024-04-04 01:45:14.000000 integ-db-0.0.5/src/integdb/module/mariadb.py
+-rw-rw-rw-   0        0        0      624 2024-04-04 01:45:26.000000 integ-db-0.0.5/src/integdb/module/mssql.py
+-rw-rw-rw-   0        0        0     1193 2024-04-04 01:45:40.000000 integ-db-0.0.5/src/integdb/module/mysql.py
+-rw-rw-rw-   0        0        0     1831 2024-04-04 01:45:59.000000 integ-db-0.0.5/src/integdb/module/sqlalchemy.py
```

### Comparing `integ-db-0.0.4/LICENSE` & `integ-db-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.4/PKG-INFO` & `integ-db-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integ-db
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python Integrated Database
 Home-page: https://github.com/Byeongin-Jeong/integdb
 Author: byeongin.jeong
 Author-email: jbi0214@gmail.com
 Project-URL: Bug Tracker, https://github.com/Byeongin-Jeong/integdb/issues
 Keywords: mysql,mssql,mariadb,python db,python database,integrate database,sqlalchemy
 Classifier: Programming Language :: Python :: 3
```

### Comparing `integ-db-0.0.4/setup.py` & `integ-db-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="integ-db",
-    version="0.0.4",
+    version="0.0.5",
     author="byeongin.jeong",
     author_email="jbi0214@gmail.com",
     description="Python Integrated Database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Byeongin-Jeong/integdb",
     project_urls={
```

### Comparing `integ-db-0.0.4/src/integ_db.egg-info/PKG-INFO` & `integ-db-0.0.5/src/integ_db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integ-db
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python Integrated Database
 Home-page: https://github.com/Byeongin-Jeong/integdb
 Author: byeongin.jeong
 Author-email: jbi0214@gmail.com
 Project-URL: Bug Tracker, https://github.com/Byeongin-Jeong/integdb/issues
 Keywords: mysql,mssql,mariadb,python db,python database,integrate database,sqlalchemy
 Classifier: Programming Language :: Python :: 3
```

### Comparing `integ-db-0.0.4/src/integrate/module/interface.py` & `integ-db-0.0.5/src/integdb/module/interface.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.4/src/integrate/module/mariadb.py` & `integ-db-0.0.5/src/integdb/module/mariadb.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.4/src/integrate/module/mssql.py` & `integ-db-0.0.5/src/integdb/module/mssql.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.4/src/integrate/module/mysql.py` & `integ-db-0.0.5/src/integdb/module/mysql.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.4/src/integrate/module/sqlalchemy.py` & `integ-db-0.0.5/src/integdb/module/sqlalchemy.py`

 * *Files identical despite different names*

