# Comparing `tmp/integ-db-0.0.6.tar.gz` & `tmp/integ-db-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "integ-db-0.0.6.tar", last modified: Fri Apr  5 03:24:33 2024, max compression
+gzip compressed data, was "integ-db-0.0.7.tar", last modified: Fri Apr  5 04:07:03 2024, max compression
```

## Comparing `integ-db-0.0.6.tar` & `integ-db-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 03:24:33.188956 integ-db-0.0.6/
--rw-rw-rw-   0        0        0     1092 2024-04-04 23:49:32.000000 integ-db-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      887 2024-04-05 03:24:33.185920 integ-db-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      131 2024-04-05 00:55:13.000000 integ-db-0.0.6/README.md
--rw-rw-rw-   0        0        0      108 2024-04-05 00:16:37.000000 integ-db-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 03:24:33.188956 integ-db-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1041 2024-04-05 03:24:22.000000 integ-db-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 03:24:33.147156 integ-db-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 03:24:33.184960 integ-db-0.0.6/src/integ_db.egg-info/
--rw-rw-rw-   0        0        0      887 2024-04-05 03:24:33.000000 integ-db-0.0.6/src/integ_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2024-04-05 03:24:33.000000 integ-db-0.0.6/src/integ_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 03:24:33.000000 integ-db-0.0.6/src/integ_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-05 03:24:33.000000 integ-db-0.0.6/src/integ_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 03:24:33.000000 integ-db-0.0.6/src/integ_db.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 03:24:33.169974 integ-db-0.0.6/src/integdb/
--rw-rw-rw-   0        0        0       34 2024-04-05 03:16:38.000000 integ-db-0.0.6/src/integdb/__init__.py
--rw-rw-rw-   0        0        0      599 2024-04-05 02:30:35.000000 integ-db-0.0.6/src/integdb/controller.py
-drwxrwxrwx   0        0        0        0 2024-04-05 03:24:33.181966 integ-db-0.0.6/src/integdb/module/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:13:56.000000 integ-db-0.0.6/src/integdb/module/__init__.py
--rw-rw-rw-   0        0        0     2344 2024-04-04 01:28:29.000000 integ-db-0.0.6/src/integdb/module/interface.py
--rw-rw-rw-   0        0        0     1090 2024-04-05 03:22:42.000000 integ-db-0.0.6/src/integdb/module/mariadb.py
--rw-rw-rw-   0        0        0      618 2024-04-05 03:22:45.000000 integ-db-0.0.6/src/integdb/module/mssql.py
--rw-rw-rw-   0        0        0     1187 2024-04-05 03:22:49.000000 integ-db-0.0.6/src/integdb/module/mysql.py
--rw-rw-rw-   0        0        0     1825 2024-04-05 03:23:06.000000 integ-db-0.0.6/src/integdb/module/sqlalchemy.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:07:03.951895 integ-db-0.0.7/
+-rw-rw-rw-   0        0        0     1092 2024-04-04 23:49:32.000000 integ-db-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     2143 2024-04-05 04:07:03.949891 integ-db-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      983 2024-04-05 04:02:17.000000 integ-db-0.0.7/README.md
+-rw-rw-rw-   0        0        0      108 2024-04-05 00:16:37.000000 integ-db-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 04:07:03.951895 integ-db-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1435 2024-04-05 04:03:04.000000 integ-db-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:07:03.886196 integ-db-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 04:07:03.947877 integ-db-0.0.7/src/integ_db.egg-info/
+-rw-rw-rw-   0        0        0     2143 2024-04-05 04:07:03.000000 integ-db-0.0.7/src/integ_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2024-04-05 04:07:03.000000 integ-db-0.0.7/src/integ_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 04:07:03.000000 integ-db-0.0.7/src/integ_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-05 04:07:03.000000 integ-db-0.0.7/src/integ_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 04:07:03.000000 integ-db-0.0.7/src/integ_db.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 04:07:03.931898 integ-db-0.0.7/src/integdb/
+-rw-rw-rw-   0        0        0       34 2024-04-05 03:16:38.000000 integ-db-0.0.7/src/integdb/__init__.py
+-rw-rw-rw-   0        0        0      599 2024-04-05 02:30:35.000000 integ-db-0.0.7/src/integdb/controller.py
+drwxrwxrwx   0        0        0        0 2024-04-05 04:07:03.945884 integ-db-0.0.7/src/integdb/module/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:13:56.000000 integ-db-0.0.7/src/integdb/module/__init__.py
+-rw-rw-rw-   0        0        0     2344 2024-04-04 01:28:29.000000 integ-db-0.0.7/src/integdb/module/interface.py
+-rw-rw-rw-   0        0        0     1090 2024-04-05 03:22:42.000000 integ-db-0.0.7/src/integdb/module/mariadb.py
+-rw-rw-rw-   0        0        0      618 2024-04-05 03:22:45.000000 integ-db-0.0.7/src/integdb/module/mssql.py
+-rw-rw-rw-   0        0        0     1187 2024-04-05 03:22:49.000000 integ-db-0.0.7/src/integdb/module/mysql.py
+-rw-rw-rw-   0        0        0     1825 2024-04-05 03:23:06.000000 integ-db-0.0.7/src/integdb/module/sqlalchemy.py
```

### Comparing `integ-db-0.0.6/LICENSE` & `integ-db-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.6/src/integdb/controller.py` & `integ-db-0.0.7/src/integdb/controller.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.6/src/integdb/module/interface.py` & `integ-db-0.0.7/src/integdb/module/interface.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.6/src/integdb/module/mariadb.py` & `integ-db-0.0.7/src/integdb/module/mariadb.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.6/src/integdb/module/mssql.py` & `integ-db-0.0.7/src/integdb/module/mssql.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.6/src/integdb/module/mysql.py` & `integ-db-0.0.7/src/integdb/module/mysql.py`

 * *Files identical despite different names*

### Comparing `integ-db-0.0.6/src/integdb/module/sqlalchemy.py` & `integ-db-0.0.7/src/integdb/module/sqlalchemy.py`

 * *Files identical despite different names*

