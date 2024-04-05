# Comparing `tmp/integ-db-0.0.1.tar.gz` & `tmp/integ-db-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "integ-db-0.0.1.tar", last modified: Fri Apr  5 01:53:02 2024, max compression
+gzip compressed data, was "integ-db-0.0.2.tar", last modified: Fri Apr  5 02:04:04 2024, max compression
```

## Comparing `integ-db-0.0.1.tar` & `integ-db-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 01:53:02.342275 integ-db-0.0.1/
--rw-rw-rw-   0        0        0     1092 2024-04-04 23:49:32.000000 integ-db-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      887 2024-04-05 01:53:02.340242 integ-db-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      131 2024-04-05 00:55:13.000000 integ-db-0.0.1/README.md
--rw-rw-rw-   0        0        0      108 2024-04-05 00:16:37.000000 integ-db-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 01:53:02.342275 integ-db-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1061 2024-04-05 01:52:39.000000 integ-db-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 01:53:02.285320 integ-db-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 01:53:02.287321 integ-db-0.0.1/src/integrate/
-drwxrwxrwx   0        0        0        0 2024-04-05 01:53:02.338228 integ-db-0.0.1/src/integrate/integ_db.egg-info/
--rw-rw-rw-   0        0        0      887 2024-04-05 01:53:02.000000 integ-db-0.0.1/src/integrate/integ_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      693 2024-04-05 01:53:02.000000 integ-db-0.0.1/src/integrate/integ_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 01:53:02.000000 integ-db-0.0.1/src/integrate/integ_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-05 01:53:02.000000 integ-db-0.0.1/src/integrate/integ_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-05 01:53:02.000000 integ-db-0.0.1/src/integrate/integ_db.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 01:53:02.335134 integ-db-0.0.1/src/integrate/module/
--rw-rw-rw-   0        0        0      140 2024-04-04 01:44:48.000000 integ-db-0.0.1/src/integrate/module/__init__.py
--rw-rw-rw-   0        0        0     2344 2024-04-04 01:28:29.000000 integ-db-0.0.1/src/integrate/module/interface.py
--rw-rw-rw-   0        0        0     1096 2024-04-04 01:45:14.000000 integ-db-0.0.1/src/integrate/module/mariadb.py
--rw-rw-rw-   0        0        0      624 2024-04-04 01:45:26.000000 integ-db-0.0.1/src/integrate/module/mssql.py
--rw-rw-rw-   0        0        0     1193 2024-04-04 01:45:40.000000 integ-db-0.0.1/src/integrate/module/mysql.py
--rw-rw-rw-   0        0        0     1831 2024-04-04 01:45:59.000000 integ-db-0.0.1/src/integrate/module/sqlalchemy.py
+drwxrwxrwx   0        0        0        0 2024-04-05 02:04:04.755648 integ-db-0.0.2/
+-rw-rw-rw-   0        0        0     1092 2024-04-04 23:49:32.000000 integ-db-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      887 2024-04-05 02:04:04.753265 integ-db-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      131 2024-04-05 00:55:13.000000 integ-db-0.0.2/README.md
+-rw-rw-rw-   0        0        0      108 2024-04-05 00:16:37.000000 integ-db-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 02:04:04.755648 integ-db-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1086 2024-04-05 02:03:53.000000 integ-db-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 02:04:04.701834 integ-db-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 02:04:04.722215 integ-db-0.0.2/src/integrate/
+drwxrwxrwx   0        0        0        0 2024-04-05 02:04:04.752269 integ-db-0.0.2/src/integrate/integ_db.egg-info/
+-rw-rw-rw-   0        0        0      887 2024-04-05 02:04:04.000000 integ-db-0.0.2/src/integrate/integ_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      718 2024-04-05 02:04:04.000000 integ-db-0.0.2/src/integrate/integ_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 02:04:04.000000 integ-db-0.0.2/src/integrate/integ_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-05 02:04:04.000000 integ-db-0.0.2/src/integrate/integ_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 02:04:04.000000 integ-db-0.0.2/src/integrate/integ_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      564 2024-04-05 00:14:01.000000 integ-db-0.0.2/src/integrate/integdb.py
+drwxrwxrwx   0        0        0        0 2024-04-05 02:04:04.749270 integ-db-0.0.2/src/integrate/module/
+-rw-rw-rw-   0        0        0      140 2024-04-04 01:44:48.000000 integ-db-0.0.2/src/integrate/module/__init__.py
+-rw-rw-rw-   0        0        0     2344 2024-04-04 01:28:29.000000 integ-db-0.0.2/src/integrate/module/interface.py
+-rw-rw-rw-   0        0        0     1096 2024-04-04 01:45:14.000000 integ-db-0.0.2/src/integrate/module/mariadb.py
+-rw-rw-rw-   0        0        0      624 2024-04-04 01:45:26.000000 integ-db-0.0.2/src/integrate/module/mssql.py
+-rw-rw-rw-   0        0        0     1193 2024-04-04 01:45:40.000000 integ-db-0.0.2/src/integrate/module/mysql.py
+-rw-rw-rw-   0        0        0     1831 2024-04-04 01:45:59.000000 integ-db-0.0.2/src/integrate/module/sqlalchemy.py
```

### Comparing `integ-db-0.0.1/LICENSE` & `integ-db-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.1/PKG-INFO` & `integ-db-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integ-db
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python Integrated Database
 Home-page: https://github.com/Byeongin-Jeong/integdb
 Author: byeongin.jeong
 Author-email: jbi0214@gmail.com
 Project-URL: Bug Tracker, https://github.com/Byeongin-Jeong/integdb/issues
 Keywords: mysql,mssql,mariadb,python db,python database,integrate database,sqlalchemy
 Classifier: Programming Language :: Python :: 3
```

### Comparing `integ-db-0.0.1/setup.py` & `integ-db-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="integ-db",
-    version="0.0.1",
+    version="0.0.2",
     author="byeongin.jeong",
     author_email="jbi0214@gmail.com",
     description="Python Integrated Database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Byeongin-Jeong/integdb",
     project_urls={
@@ -17,12 +17,13 @@
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src/integrate"},
-    packages=find_packages(where="src/integrate"),
+    py_modules=['integdb'],
+    packages=find_packages(where="integrate"),
     python_requires=">=3.6",
     keywords=['mysql', 'mssql', 'mariadb', 'python db', 'python database', 'integrate database', 'sqlalchemy'],
     install_requires=['pymysql', 'mariadb', 'pymssql', 'pymysql-pool', 'SQLAlchemy', 'pandas'],
 )
```

### Comparing `integ-db-0.0.1/src/integrate/integ_db.egg-info/PKG-INFO` & `integ-db-0.0.2/src/integrate/integ_db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integ-db
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python Integrated Database
 Home-page: https://github.com/Byeongin-Jeong/integdb
 Author: byeongin.jeong
 Author-email: jbi0214@gmail.com
 Project-URL: Bug Tracker, https://github.com/Byeongin-Jeong/integdb/issues
 Keywords: mysql,mssql,mariadb,python db,python database,integrate database,sqlalchemy
 Classifier: Programming Language :: Python :: 3
```

### Comparing `integ-db-0.0.1/src/integrate/integ_db.egg-info/SOURCES.txt` & `integ-db-0.0.2/src/integrate/integ_db.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 setup.py
 src/integrate/integ_db.egg-info/PKG-INFO
 src/integrate/integ_db.egg-info/SOURCES.txt
 src/integrate/integ_db.egg-info/dependency_links.txt
 src/integrate/integ_db.egg-info/requires.txt
 src/integrate/integ_db.egg-info/top_level.txt
+src/integrate/integdb.py
 src/integrate/integ_db.egg-info/PKG-INFO
 src/integrate/integ_db.egg-info/SOURCES.txt
 src/integrate/integ_db.egg-info/dependency_links.txt
 src/integrate/integ_db.egg-info/requires.txt
 src/integrate/integ_db.egg-info/top_level.txt
 src/integrate/module/__init__.py
 src/integrate/module/interface.py
```

### Comparing `integ-db-0.0.1/src/integrate/module/interface.py` & `integ-db-0.0.2/src/integrate/module/interface.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.1/src/integrate/module/mariadb.py` & `integ-db-0.0.2/src/integrate/module/mariadb.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.1/src/integrate/module/mssql.py` & `integ-db-0.0.2/src/integrate/module/mssql.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.1/src/integrate/module/mysql.py` & `integ-db-0.0.2/src/integrate/module/mysql.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.1/src/integrate/module/sqlalchemy.py` & `integ-db-0.0.2/src/integrate/module/sqlalchemy.py`

 * *Files identical despite different names*

