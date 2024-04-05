# Comparing `tmp/integ-db-0.0.7.tar.gz` & `tmp/integ-db-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "integ-db-0.0.7.tar", last modified: Fri Apr  5 04:07:03 2024, max compression
+gzip compressed data, was "integ-db-0.0.8.tar", last modified: Fri Apr  5 04:08:51 2024, max compression
```

## Comparing `integ-db-0.0.7.tar` & `integ-db-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 04:07:03.951895 integ-db-0.0.7/
--rw-rw-rw-   0        0        0     1092 2024-04-04 23:49:32.000000 integ-db-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     2143 2024-04-05 04:07:03.949891 integ-db-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      983 2024-04-05 04:02:17.000000 integ-db-0.0.7/README.md
--rw-rw-rw-   0        0        0      108 2024-04-05 00:16:37.000000 integ-db-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 04:07:03.951895 integ-db-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1435 2024-04-05 04:03:04.000000 integ-db-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 04:07:03.886196 integ-db-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 04:07:03.947877 integ-db-0.0.7/src/integ_db.egg-info/
--rw-rw-rw-   0        0        0     2143 2024-04-05 04:07:03.000000 integ-db-0.0.7/src/integ_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2024-04-05 04:07:03.000000 integ-db-0.0.7/src/integ_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 04:07:03.000000 integ-db-0.0.7/src/integ_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-05 04:07:03.000000 integ-db-0.0.7/src/integ_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 04:07:03.000000 integ-db-0.0.7/src/integ_db.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 04:07:03.931898 integ-db-0.0.7/src/integdb/
--rw-rw-rw-   0        0        0       34 2024-04-05 03:16:38.000000 integ-db-0.0.7/src/integdb/__init__.py
--rw-rw-rw-   0        0        0      599 2024-04-05 02:30:35.000000 integ-db-0.0.7/src/integdb/controller.py
-drwxrwxrwx   0        0        0        0 2024-04-05 04:07:03.945884 integ-db-0.0.7/src/integdb/module/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:13:56.000000 integ-db-0.0.7/src/integdb/module/__init__.py
--rw-rw-rw-   0        0        0     2344 2024-04-04 01:28:29.000000 integ-db-0.0.7/src/integdb/module/interface.py
--rw-rw-rw-   0        0        0     1090 2024-04-05 03:22:42.000000 integ-db-0.0.7/src/integdb/module/mariadb.py
--rw-rw-rw-   0        0        0      618 2024-04-05 03:22:45.000000 integ-db-0.0.7/src/integdb/module/mssql.py
--rw-rw-rw-   0        0        0     1187 2024-04-05 03:22:49.000000 integ-db-0.0.7/src/integdb/module/mysql.py
--rw-rw-rw-   0        0        0     1825 2024-04-05 03:23:06.000000 integ-db-0.0.7/src/integdb/module/sqlalchemy.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:08:51.732106 integ-db-0.0.8/
+-rw-rw-rw-   0        0        0     1092 2024-04-04 23:49:32.000000 integ-db-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     2143 2024-04-05 04:08:51.730105 integ-db-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      983 2024-04-05 04:08:03.000000 integ-db-0.0.8/README.md
+-rw-rw-rw-   0        0        0      108 2024-04-05 00:16:37.000000 integ-db-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 04:08:51.733103 integ-db-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1435 2024-04-05 04:08:21.000000 integ-db-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:08:51.694421 integ-db-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 04:08:51.729060 integ-db-0.0.8/src/integ_db.egg-info/
+-rw-rw-rw-   0        0        0     2143 2024-04-05 04:08:51.000000 integ-db-0.0.8/src/integ_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2024-04-05 04:08:51.000000 integ-db-0.0.8/src/integ_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 04:08:51.000000 integ-db-0.0.8/src/integ_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-05 04:08:51.000000 integ-db-0.0.8/src/integ_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 04:08:51.000000 integ-db-0.0.8/src/integ_db.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 04:08:51.714541 integ-db-0.0.8/src/integdb/
+-rw-rw-rw-   0        0        0       34 2024-04-05 03:16:38.000000 integ-db-0.0.8/src/integdb/__init__.py
+-rw-rw-rw-   0        0        0      599 2024-04-05 02:30:35.000000 integ-db-0.0.8/src/integdb/controller.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:08:51.727492 integ-db-0.0.8/src/integdb/module/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:13:56.000000 integ-db-0.0.8/src/integdb/module/__init__.py
+-rw-rw-rw-   0        0        0     2344 2024-04-04 01:28:29.000000 integ-db-0.0.8/src/integdb/module/interface.py
+-rw-rw-rw-   0        0        0     1090 2024-04-05 03:22:42.000000 integ-db-0.0.8/src/integdb/module/mariadb.py
+-rw-rw-rw-   0        0        0      618 2024-04-05 03:22:45.000000 integ-db-0.0.8/src/integdb/module/mssql.py
+-rw-rw-rw-   0        0        0     1187 2024-04-05 03:22:49.000000 integ-db-0.0.8/src/integdb/module/mysql.py
+-rw-rw-rw-   0        0        0     1825 2024-04-05 03:23:06.000000 integ-db-0.0.8/src/integdb/module/sqlalchemy.py
```

### Comparing `integ-db-0.0.7/LICENSE` & `integ-db-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.7/PKG-INFO` & `integ-db-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integ-db
-Version: 0.0.7
+Version: 0.0.8
 Summary: This package Integrated Database library
 Home-page: https://github.com/Byeongin-Jeong/integdb
 Author: byeongin.jeong
 Author-email: jbi0214@gmail.com
 Project-URL: Bug Tracker, https://github.com/Byeongin-Jeong/integdb/issues
 Keywords: mysql,mssql,mariadb,python db,python database,integrate database,sqlalchemy
 Classifier: Programming Language :: Python :: 3
@@ -30,19 +30,19 @@
 
 # integdb
 ### This package Integrated Database library, based on PyMySQL, pymssql, mariadb, SQLAlchemy.
 
 #### Requirements
 - MySQL
 - MSSQL(SQL Server)
-- MaridDB
+- MariaDB
 
 #### Controller Object
 - MySQL
-- MaridDB
+- MariaDB
 - MSSQL
 - SQLAlchemy
 
 #### Object that provides a pool
 - MySQL
 - MariaDB
```

### Comparing `integ-db-0.0.7/README.md` & `integ-db-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # integdb
 ### This package Integrated Database library, based on PyMySQL, pymssql, mariadb, SQLAlchemy.
 
 #### Requirements
 - MySQL
 - MSSQL(SQL Server)
-- MaridDB
+- MariaDB
 
 #### Controller Object
 - MySQL
-- MaridDB
+- MariaDB
 - MSSQL
 - SQLAlchemy
 
 #### Object that provides a pool
 - MySQL
 - MariaDB
```

### Comparing `integ-db-0.0.7/setup.py` & `integ-db-0.0.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="integ-db",
-    version="0.0.7",
+    version="0.0.8",
     author="byeongin.jeong",
     author_email="jbi0214@gmail.com",
     description="This package Integrated Database library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Byeongin-Jeong/integdb",
     project_urls={
```

### Comparing `integ-db-0.0.7/src/integ_db.egg-info/PKG-INFO` & `integ-db-0.0.8/src/integ_db.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integ-db
-Version: 0.0.7
+Version: 0.0.8
 Summary: This package Integrated Database library
 Home-page: https://github.com/Byeongin-Jeong/integdb
 Author: byeongin.jeong
 Author-email: jbi0214@gmail.com
 Project-URL: Bug Tracker, https://github.com/Byeongin-Jeong/integdb/issues
 Keywords: mysql,mssql,mariadb,python db,python database,integrate database,sqlalchemy
 Classifier: Programming Language :: Python :: 3
@@ -30,19 +30,19 @@
 
 # integdb
 ### This package Integrated Database library, based on PyMySQL, pymssql, mariadb, SQLAlchemy.
 
 #### Requirements
 - MySQL
 - MSSQL(SQL Server)
-- MaridDB
+- MariaDB
 
 #### Controller Object
 - MySQL
-- MaridDB
+- MariaDB
 - MSSQL
 - SQLAlchemy
 
 #### Object that provides a pool
 - MySQL
 - MariaDB
```

### Comparing `integ-db-0.0.7/src/integdb/controller.py` & `integ-db-0.0.8/src/integdb/controller.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.7/src/integdb/module/interface.py` & `integ-db-0.0.8/src/integdb/module/interface.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.7/src/integdb/module/mariadb.py` & `integ-db-0.0.8/src/integdb/module/mariadb.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.7/src/integdb/module/mssql.py` & `integ-db-0.0.8/src/integdb/module/mssql.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.7/src/integdb/module/mysql.py` & `integ-db-0.0.8/src/integdb/module/mysql.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.7/src/integdb/module/sqlalchemy.py` & `integ-db-0.0.8/src/integdb/module/sqlalchemy.py`

 * *Files identical despite different names*

