# Comparing `tmp/integ-db-0.0.5.tar.gz` & `tmp/integ-db-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "integ-db-0.0.5.tar", last modified: Fri Apr  5 03:18:37 2024, max compression
+gzip compressed data, was "integ-db-0.0.6.tar", last modified: Fri Apr  5 03:24:33 2024, max compression
```

## Comparing `integ-db-0.0.5.tar` & `integ-db-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 03:18:37.188560 integ-db-0.0.5/
--rw-rw-rw-   0        0        0     1092 2024-04-04 23:49:32.000000 integ-db-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      887 2024-04-05 03:18:37.186559 integ-db-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      131 2024-04-05 00:55:13.000000 integ-db-0.0.5/README.md
--rw-rw-rw-   0        0        0      108 2024-04-05 00:16:37.000000 integ-db-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 03:18:37.188560 integ-db-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1041 2024-04-05 03:18:20.000000 integ-db-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 03:18:37.140014 integ-db-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 03:18:37.184681 integ-db-0.0.5/src/integ_db.egg-info/
--rw-rw-rw-   0        0        0      887 2024-04-05 03:18:37.000000 integ-db-0.0.5/src/integ_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2024-04-05 03:18:37.000000 integ-db-0.0.5/src/integ_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 03:18:37.000000 integ-db-0.0.5/src/integ_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-05 03:18:37.000000 integ-db-0.0.5/src/integ_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 03:18:37.000000 integ-db-0.0.5/src/integ_db.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 03:18:37.169061 integ-db-0.0.5/src/integdb/
--rw-rw-rw-   0        0        0       34 2024-04-05 03:16:38.000000 integ-db-0.0.5/src/integdb/__init__.py
--rw-rw-rw-   0        0        0      599 2024-04-05 02:30:35.000000 integ-db-0.0.5/src/integdb/controller.py
-drwxrwxrwx   0        0        0        0 2024-04-05 03:18:37.182541 integ-db-0.0.5/src/integdb/module/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:13:56.000000 integ-db-0.0.5/src/integdb/module/__init__.py
--rw-rw-rw-   0        0        0     2344 2024-04-04 01:28:29.000000 integ-db-0.0.5/src/integdb/module/interface.py
--rw-rw-rw-   0        0        0     1096 2024-04-04 01:45:14.000000 integ-db-0.0.5/src/integdb/module/mariadb.py
--rw-rw-rw-   0        0        0      624 2024-04-04 01:45:26.000000 integ-db-0.0.5/src/integdb/module/mssql.py
--rw-rw-rw-   0        0        0     1193 2024-04-04 01:45:40.000000 integ-db-0.0.5/src/integdb/module/mysql.py
--rw-rw-rw-   0        0        0     1831 2024-04-04 01:45:59.000000 integ-db-0.0.5/src/integdb/module/sqlalchemy.py
+drwxrwxrwx   0        0        0        0 2024-04-05 03:24:33.188956 integ-db-0.0.6/
+-rw-rw-rw-   0        0        0     1092 2024-04-04 23:49:32.000000 integ-db-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      887 2024-04-05 03:24:33.185920 integ-db-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      131 2024-04-05 00:55:13.000000 integ-db-0.0.6/README.md
+-rw-rw-rw-   0        0        0      108 2024-04-05 00:16:37.000000 integ-db-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 03:24:33.188956 integ-db-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1041 2024-04-05 03:24:22.000000 integ-db-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 03:24:33.147156 integ-db-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 03:24:33.184960 integ-db-0.0.6/src/integ_db.egg-info/
+-rw-rw-rw-   0        0        0      887 2024-04-05 03:24:33.000000 integ-db-0.0.6/src/integ_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2024-04-05 03:24:33.000000 integ-db-0.0.6/src/integ_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 03:24:33.000000 integ-db-0.0.6/src/integ_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-05 03:24:33.000000 integ-db-0.0.6/src/integ_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 03:24:33.000000 integ-db-0.0.6/src/integ_db.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 03:24:33.169974 integ-db-0.0.6/src/integdb/
+-rw-rw-rw-   0        0        0       34 2024-04-05 03:16:38.000000 integ-db-0.0.6/src/integdb/__init__.py
+-rw-rw-rw-   0        0        0      599 2024-04-05 02:30:35.000000 integ-db-0.0.6/src/integdb/controller.py
+drwxrwxrwx   0        0        0        0 2024-04-05 03:24:33.181966 integ-db-0.0.6/src/integdb/module/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:13:56.000000 integ-db-0.0.6/src/integdb/module/__init__.py
+-rw-rw-rw-   0        0        0     2344 2024-04-04 01:28:29.000000 integ-db-0.0.6/src/integdb/module/interface.py
+-rw-rw-rw-   0        0        0     1090 2024-04-05 03:22:42.000000 integ-db-0.0.6/src/integdb/module/mariadb.py
+-rw-rw-rw-   0        0        0      618 2024-04-05 03:22:45.000000 integ-db-0.0.6/src/integdb/module/mssql.py
+-rw-rw-rw-   0        0        0     1187 2024-04-05 03:22:49.000000 integ-db-0.0.6/src/integdb/module/mysql.py
+-rw-rw-rw-   0        0        0     1825 2024-04-05 03:23:06.000000 integ-db-0.0.6/src/integdb/module/sqlalchemy.py
```

### Comparing `integ-db-0.0.5/LICENSE` & `integ-db-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.5/PKG-INFO` & `integ-db-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integ-db
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python Integrated Database
 Home-page: https://github.com/Byeongin-Jeong/integdb
 Author: byeongin.jeong
 Author-email: jbi0214@gmail.com
 Project-URL: Bug Tracker, https://github.com/Byeongin-Jeong/integdb/issues
 Keywords: mysql,mssql,mariadb,python db,python database,integrate database,sqlalchemy
 Classifier: Programming Language :: Python :: 3
```

### Comparing `integ-db-0.0.5/setup.py` & `integ-db-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="integ-db",
-    version="0.0.5",
+    version="0.0.6",
     author="byeongin.jeong",
     author_email="jbi0214@gmail.com",
     description="Python Integrated Database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Byeongin-Jeong/integdb",
     project_urls={
```

### Comparing `integ-db-0.0.5/src/integ_db.egg-info/PKG-INFO` & `integ-db-0.0.6/src/integ_db.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integ-db
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python Integrated Database
 Home-page: https://github.com/Byeongin-Jeong/integdb
 Author: byeongin.jeong
 Author-email: jbi0214@gmail.com
 Project-URL: Bug Tracker, https://github.com/Byeongin-Jeong/integdb/issues
 Keywords: mysql,mssql,mariadb,python db,python database,integrate database,sqlalchemy
 Classifier: Programming Language :: Python :: 3
```

### Comparing `integ-db-0.0.5/src/integdb/controller.py` & `integ-db-0.0.6/src/integdb/controller.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.5/src/integdb/module/interface.py` & `integ-db-0.0.6/src/integdb/module/interface.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.5/src/integdb/module/mariadb.py` & `integ-db-0.0.6/src/integdb/module/mariadb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import mariadb
-from module.interface import DefaultInterface
+from .interface import DefaultInterface
 
 class MariaDB(DefaultInterface):
     def connect(self, pool_name="app-pool", pool_size=20):
         try:
             if self._ispool is False:
                 self._conn = mariadb.connect(
                     host=self._host,
```

### Comparing `integ-db-0.0.5/src/integdb/module/mssql.py` & `integ-db-0.0.6/src/integdb/module/mssql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pymssql
-from module.interface import DefaultInterface
+from .interface import DefaultInterface
 
 class MSSQL(DefaultInterface):
     def connect(self):
         try:
             self._conn = pymssql.connect(
                 host=self._host,
                 user=self._user,
```

### Comparing `integ-db-0.0.5/src/integdb/module/mysql.py` & `integ-db-0.0.6/src/integdb/module/mysql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pymysql
 from pymysqlpool import ConnectionPool
-from module.interface import DefaultInterface
+from .interface import DefaultInterface
 
 pymysql.install_as_MySQLdb()
 
 class MySQL(DefaultInterface):
     def connect(self, pool_size=10):
         try:
             print (pool_size)
```

### Comparing `integ-db-0.0.5/src/integdb/module/sqlalchemy.py` & `integ-db-0.0.6/src/integdb/module/sqlalchemy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 from sqlalchemy import create_engine
-from module.interface import SessionConfig
 from sqlalchemy.exc import IntegrityError
+from .interface import SessionConfig
 
 class SQLAlchemy(SessionConfig):
     def __init__(self, host, user, password, port, schema, connection_pool):
         super().__init__(host, user, password, port, schema, connection_pool)
 
     def connect(self, db_url="mysql+pymysql"):
         try:
```

