# Comparing `tmp/integ-db-0.0.2.tar.gz` & `tmp/integ-db-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "integ-db-0.0.2.tar", last modified: Fri Apr  5 02:04:04 2024, max compression
+gzip compressed data, was "integ-db-0.0.3.tar", last modified: Fri Apr  5 02:11:08 2024, max compression
```

## Comparing `integ-db-0.0.2.tar` & `integ-db-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 02:04:04.755648 integ-db-0.0.2/
--rw-rw-rw-   0        0        0     1092 2024-04-04 23:49:32.000000 integ-db-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      887 2024-04-05 02:04:04.753265 integ-db-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      131 2024-04-05 00:55:13.000000 integ-db-0.0.2/README.md
--rw-rw-rw-   0        0        0      108 2024-04-05 00:16:37.000000 integ-db-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 02:04:04.755648 integ-db-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1086 2024-04-05 02:03:53.000000 integ-db-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 02:04:04.701834 integ-db-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 02:04:04.722215 integ-db-0.0.2/src/integrate/
-drwxrwxrwx   0        0        0        0 2024-04-05 02:04:04.752269 integ-db-0.0.2/src/integrate/integ_db.egg-info/
--rw-rw-rw-   0        0        0      887 2024-04-05 02:04:04.000000 integ-db-0.0.2/src/integrate/integ_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      718 2024-04-05 02:04:04.000000 integ-db-0.0.2/src/integrate/integ_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 02:04:04.000000 integ-db-0.0.2/src/integrate/integ_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-05 02:04:04.000000 integ-db-0.0.2/src/integrate/integ_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 02:04:04.000000 integ-db-0.0.2/src/integrate/integ_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      564 2024-04-05 00:14:01.000000 integ-db-0.0.2/src/integrate/integdb.py
-drwxrwxrwx   0        0        0        0 2024-04-05 02:04:04.749270 integ-db-0.0.2/src/integrate/module/
--rw-rw-rw-   0        0        0      140 2024-04-04 01:44:48.000000 integ-db-0.0.2/src/integrate/module/__init__.py
--rw-rw-rw-   0        0        0     2344 2024-04-04 01:28:29.000000 integ-db-0.0.2/src/integrate/module/interface.py
--rw-rw-rw-   0        0        0     1096 2024-04-04 01:45:14.000000 integ-db-0.0.2/src/integrate/module/mariadb.py
--rw-rw-rw-   0        0        0      624 2024-04-04 01:45:26.000000 integ-db-0.0.2/src/integrate/module/mssql.py
--rw-rw-rw-   0        0        0     1193 2024-04-04 01:45:40.000000 integ-db-0.0.2/src/integrate/module/mysql.py
--rw-rw-rw-   0        0        0     1831 2024-04-04 01:45:59.000000 integ-db-0.0.2/src/integrate/module/sqlalchemy.py
+drwxrwxrwx   0        0        0        0 2024-04-05 02:11:08.083497 integ-db-0.0.3/
+-rw-rw-rw-   0        0        0     1092 2024-04-04 23:49:32.000000 integ-db-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      887 2024-04-05 02:11:08.081471 integ-db-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      131 2024-04-05 00:55:13.000000 integ-db-0.0.3/README.md
+-rw-rw-rw-   0        0        0      108 2024-04-05 00:16:37.000000 integ-db-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 02:11:08.083497 integ-db-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1041 2024-04-05 02:10:49.000000 integ-db-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 02:11:08.037623 integ-db-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 02:11:08.079510 integ-db-0.0.3/src/integ_db.egg-info/
+-rw-rw-rw-   0        0        0      887 2024-04-05 02:11:08.000000 integ-db-0.0.3/src/integ_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2024-04-05 02:11:08.000000 integ-db-0.0.3/src/integ_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 02:11:08.000000 integ-db-0.0.3/src/integ_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-05 02:11:08.000000 integ-db-0.0.3/src/integ_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-05 02:11:08.000000 integ-db-0.0.3/src/integ_db.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 02:11:08.060758 integ-db-0.0.3/src/integrate/
+-rw-rw-rw-   0        0        0        0 2024-04-05 01:40:47.000000 integ-db-0.0.3/src/integrate/__init__.py
+-rw-rw-rw-   0        0        0      564 2024-04-05 00:14:01.000000 integ-db-0.0.3/src/integrate/integdb.py
+drwxrwxrwx   0        0        0        0 2024-04-05 02:11:08.077475 integ-db-0.0.3/src/integrate/module/
+-rw-rw-rw-   0        0        0      140 2024-04-04 01:44:48.000000 integ-db-0.0.3/src/integrate/module/__init__.py
+-rw-rw-rw-   0        0        0     2344 2024-04-04 01:28:29.000000 integ-db-0.0.3/src/integrate/module/interface.py
+-rw-rw-rw-   0        0        0     1096 2024-04-04 01:45:14.000000 integ-db-0.0.3/src/integrate/module/mariadb.py
+-rw-rw-rw-   0        0        0      624 2024-04-04 01:45:26.000000 integ-db-0.0.3/src/integrate/module/mssql.py
+-rw-rw-rw-   0        0        0     1193 2024-04-04 01:45:40.000000 integ-db-0.0.3/src/integrate/module/mysql.py
+-rw-rw-rw-   0        0        0     1831 2024-04-04 01:45:59.000000 integ-db-0.0.3/src/integrate/module/sqlalchemy.py
```

### Comparing `integ-db-0.0.2/LICENSE` & `integ-db-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.2/PKG-INFO` & `integ-db-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integ-db
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python Integrated Database
 Home-page: https://github.com/Byeongin-Jeong/integdb
 Author: byeongin.jeong
 Author-email: jbi0214@gmail.com
 Project-URL: Bug Tracker, https://github.com/Byeongin-Jeong/integdb/issues
 Keywords: mysql,mssql,mariadb,python db,python database,integrate database,sqlalchemy
 Classifier: Programming Language :: Python :: 3
```

### Comparing `integ-db-0.0.2/setup.py` & `integ-db-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="integ-db",
-    version="0.0.2",
+    version="0.0.3",
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
-    package_dir={"": "src/integrate"},
-    py_modules=['integdb'],
-    packages=find_packages(where="integrate"),
+    package_dir={"": "src"},
+    packages=find_packages(where="src"),
     python_requires=">=3.6",
     keywords=['mysql', 'mssql', 'mariadb', 'python db', 'python database', 'integrate database', 'sqlalchemy'],
     install_requires=['pymysql', 'mariadb', 'pymssql', 'pymysql-pool', 'SQLAlchemy', 'pandas'],
 )
```

### Comparing `integ-db-0.0.2/src/integrate/integ_db.egg-info/PKG-INFO` & `integ-db-0.0.3/src/integ_db.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integ-db
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python Integrated Database
 Home-page: https://github.com/Byeongin-Jeong/integdb
 Author: byeongin.jeong
 Author-email: jbi0214@gmail.com
 Project-URL: Bug Tracker, https://github.com/Byeongin-Jeong/integdb/issues
 Keywords: mysql,mssql,mariadb,python db,python database,integrate database,sqlalchemy
 Classifier: Programming Language :: Python :: 3
```

### Comparing `integ-db-0.0.2/src/integrate/integdb.py` & `integ-db-0.0.3/src/integrate/integdb.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.2/src/integrate/module/interface.py` & `integ-db-0.0.3/src/integrate/module/interface.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.2/src/integrate/module/mariadb.py` & `integ-db-0.0.3/src/integrate/module/mariadb.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.2/src/integrate/module/mssql.py` & `integ-db-0.0.3/src/integrate/module/mssql.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.2/src/integrate/module/mysql.py` & `integ-db-0.0.3/src/integrate/module/mysql.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.2/src/integrate/module/sqlalchemy.py` & `integ-db-0.0.3/src/integrate/module/sqlalchemy.py`

 * *Files identical despite different names*

