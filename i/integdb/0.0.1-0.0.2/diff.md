# Comparing `tmp/integdb-0.0.1.tar.gz` & `tmp/integdb-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "integdb-0.0.1.tar", last modified: Fri Apr  5 00:35:12 2024, max compression
+gzip compressed data, was "integdb-0.0.2.tar", last modified: Fri Apr  5 01:28:05 2024, max compression
```

## Comparing `integdb-0.0.1.tar` & `integdb-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 00:35:12.233125 integdb-0.0.1/
--rw-rw-rw-   0        0        0     1092 2024-04-04 23:49:32.000000 integdb-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      804 2024-04-05 00:35:12.231109 integdb-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       49 2024-04-04 23:49:32.000000 integdb-0.0.1/README.md
--rw-rw-rw-   0        0        0      108 2024-04-05 00:16:37.000000 integdb-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 00:35:12.233125 integdb-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1040 2024-04-05 00:24:56.000000 integdb-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 00:35:12.190278 integdb-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 00:35:12.229869 integdb-0.0.1/src/integdb.egg-info/
--rw-rw-rw-   0        0        0      804 2024-04-05 00:35:12.000000 integdb-0.0.1/src/integdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2024-04-05 00:35:12.000000 integdb-0.0.1/src/integdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 00:35:12.000000 integdb-0.0.1/src/integdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-05 00:35:12.000000 integdb-0.0.1/src/integdb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-05 00:35:12.000000 integdb-0.0.1/src/integdb.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 00:35:12.226849 integdb-0.0.1/src/module/
--rw-rw-rw-   0        0        0      140 2024-04-04 01:44:48.000000 integdb-0.0.1/src/module/__init__.py
--rw-rw-rw-   0        0        0     2344 2024-04-04 01:28:29.000000 integdb-0.0.1/src/module/interface.py
--rw-rw-rw-   0        0        0     1096 2024-04-04 01:45:14.000000 integdb-0.0.1/src/module/mariadb.py
--rw-rw-rw-   0        0        0      624 2024-04-04 01:45:26.000000 integdb-0.0.1/src/module/mssql.py
--rw-rw-rw-   0        0        0     1193 2024-04-04 01:45:40.000000 integdb-0.0.1/src/module/mysql.py
--rw-rw-rw-   0        0        0     1831 2024-04-04 01:45:59.000000 integdb-0.0.1/src/module/sqlalchemy.py
+drwxrwxrwx   0        0        0        0 2024-04-05 01:28:05.850360 integdb-0.0.2/
+-rw-rw-rw-   0        0        0     1092 2024-04-04 23:49:32.000000 integdb-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      886 2024-04-05 01:28:05.846310 integdb-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      131 2024-04-05 00:55:13.000000 integdb-0.0.2/README.md
+-rw-rw-rw-   0        0        0      108 2024-04-05 00:16:37.000000 integdb-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 01:28:05.850360 integdb-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1080 2024-04-05 01:27:55.000000 integdb-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 01:28:05.793360 integdb-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 01:28:05.794351 integdb-0.0.2/src/integrated_database/
+drwxrwxrwx   0        0        0        0 2024-04-05 01:28:05.845322 integdb-0.0.2/src/integrated_database/integdb.egg-info/
+-rw-rw-rw-   0        0        0      886 2024-04-05 01:28:05.000000 integdb-0.0.2/src/integrated_database/integdb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      843 2024-04-05 01:28:05.000000 integdb-0.0.2/src/integrated_database/integdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 01:28:05.000000 integdb-0.0.2/src/integrated_database/integdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-05 01:28:05.000000 integdb-0.0.2/src/integrated_database/integdb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-05 01:28:05.000000 integdb-0.0.2/src/integrated_database/integdb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 01:28:05.843402 integdb-0.0.2/src/integrated_database/module/
+-rw-rw-rw-   0        0        0      140 2024-04-04 01:44:48.000000 integdb-0.0.2/src/integrated_database/module/__init__.py
+-rw-rw-rw-   0        0        0     2344 2024-04-04 01:28:29.000000 integdb-0.0.2/src/integrated_database/module/interface.py
+-rw-rw-rw-   0        0        0     1096 2024-04-04 01:45:14.000000 integdb-0.0.2/src/integrated_database/module/mariadb.py
+-rw-rw-rw-   0        0        0      624 2024-04-04 01:45:26.000000 integdb-0.0.2/src/integrated_database/module/mssql.py
+-rw-rw-rw-   0        0        0     1193 2024-04-04 01:45:40.000000 integdb-0.0.2/src/integrated_database/module/mysql.py
+-rw-rw-rw-   0        0        0     1831 2024-04-04 01:45:59.000000 integdb-0.0.2/src/integrated_database/module/sqlalchemy.py
```

### Comparing `integdb-0.0.1/LICENSE` & `integdb-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `integdb-0.0.1/PKG-INFO` & `integdb-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integdb
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python Integrated Database
 Home-page: https://github.com/Byeongin-Jeong/integdb
 Author: byeongin.jeong
 Author-email: jbi0214@gmail.com
 Project-URL: Bug Tracker, https://github.com/Byeongin-Jeong/integdb/issues
 Keywords: mysql,mssql,mariadb,python db,python database,integrate database,sqlalchemy
 Classifier: Programming Language :: Python :: 3
@@ -17,8 +17,15 @@
 Requires-Dist: mariadb
 Requires-Dist: pymssql
 Requires-Dist: pymysql-pool
 Requires-Dist: SQLAlchemy
 Requires-Dist: pandas
 
 # integdb
-python Module by Integrated Database
+#### Python Module by Integrated Database
+
+#### 1. Install Package
+```
+pip install integdb
+```
+
+#### 2. How to
```

### Comparing `integdb-0.0.1/setup.py` & `integdb-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="integdb",
-    version="0.0.1",
+    version="0.0.2",
     author="byeongin.jeong",
     author_email="jbi0214@gmail.com",
     description="Python Integrated Database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Byeongin-Jeong/integdb",
     project_urls={
         "Bug Tracker": "https://github.com/Byeongin-Jeong/integdb/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    package_dir={"": "src"},
-    packages=find_packages(where="src"),
+    package_dir={"": "src/integrated_database"},
+    packages=find_packages(where="src/integrated_database"),
     python_requires=">=3.6",
     keywords=['mysql', 'mssql', 'mariadb', 'python db', 'python database', 'integrate database', 'sqlalchemy'],
     install_requires=['pymysql', 'mariadb', 'pymssql', 'pymysql-pool', 'SQLAlchemy', 'pandas'],
 )
```

### Comparing `integdb-0.0.1/src/integdb.egg-info/PKG-INFO` & `integdb-0.0.2/src/integrated_database/integdb.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integdb
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python Integrated Database
 Home-page: https://github.com/Byeongin-Jeong/integdb
 Author: byeongin.jeong
 Author-email: jbi0214@gmail.com
 Project-URL: Bug Tracker, https://github.com/Byeongin-Jeong/integdb/issues
 Keywords: mysql,mssql,mariadb,python db,python database,integrate database,sqlalchemy
 Classifier: Programming Language :: Python :: 3
@@ -17,8 +17,15 @@
 Requires-Dist: mariadb
 Requires-Dist: pymssql
 Requires-Dist: pymysql-pool
 Requires-Dist: SQLAlchemy
 Requires-Dist: pandas
 
 # integdb
-python Module by Integrated Database
+#### Python Module by Integrated Database
+
+#### 1. Install Package
+```
+pip install integdb
+```
+
+#### 2. How to
```

### Comparing `integdb-0.0.1/src/module/interface.py` & `integdb-0.0.2/src/integrated_database/module/interface.py`

 * *Files identical despite different names*

### Comparing `integdb-0.0.1/src/module/mariadb.py` & `integdb-0.0.2/src/integrated_database/module/mariadb.py`

 * *Files identical despite different names*

### Comparing `integdb-0.0.1/src/module/mssql.py` & `integdb-0.0.2/src/integrated_database/module/mssql.py`

 * *Files identical despite different names*

### Comparing `integdb-0.0.1/src/module/mysql.py` & `integdb-0.0.2/src/integrated_database/module/mysql.py`

 * *Files identical despite different names*

### Comparing `integdb-0.0.1/src/module/sqlalchemy.py` & `integdb-0.0.2/src/integrated_database/module/sqlalchemy.py`

 * *Files identical despite different names*

