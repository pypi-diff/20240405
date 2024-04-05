# Comparing `tmp/sqlx-exec-2.3.3.tar.gz` & `tmp/sqlx-exec-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlx-exec-2.3.3.tar", last modified: Fri Mar 29 02:19:43 2024, max compression
+gzip compressed data, was "sqlx-exec-2.3.4.tar", last modified: Fri Apr  5 02:31:35 2024, max compression
```

## Comparing `sqlx-exec-2.3.3.tar` & `sqlx-exec-2.3.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-03-29 02:19:42.995468 sqlx-exec-2.3.3/
--rw-r--r--   0 summy      (501) staff       (20)    11357 2024-01-23 07:49:56.000000 sqlx-exec-2.3.3/LICENSE
--rw-r--r--   0 summy      (501) staff       (20)     7492 2024-03-29 02:19:42.994714 sqlx-exec-2.3.3/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)     6974 2024-03-29 02:19:13.000000 sqlx-exec-2.3.3/README.rst
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-03-29 02:19:42.995906 sqlx-exec-2.3.3/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1298 2024-03-29 02:12:39.000000 sqlx-exec-2.3.3/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-03-29 02:19:42.983882 sqlx-exec-2.3.3/sqlexec/
--rw-r--r--   0 summy      (501) staff       (20)     1768 2024-03-28 02:42:54.000000 sqlx-exec-2.3.3/sqlexec/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)      637 2024-03-27 13:46:01.000000 sqlx-exec-2.3.3/sqlexec/constant.py
--rw-r--r--   0 summy      (501) staff       (20)     6704 2024-03-27 13:04:34.000000 sqlx-exec-2.3.3/sqlexec/dialect.py
--rw-r--r--   0 summy      (501) staff       (20)    13843 2024-03-28 01:00:25.000000 sqlx-exec-2.3.3/sqlexec/exec.py
--rw-r--r--   0 summy      (501) staff       (20)     1956 2024-03-25 07:14:31.000000 sqlx-exec-2.3.3/sqlexec/loader.py
--rw-r--r--   0 summy      (501) staff       (20)      816 2024-03-27 08:41:08.000000 sqlx-exec-2.3.3/sqlexec/log_support.py
--rw-r--r--   0 summy      (501) staff       (20)     1933 2024-03-27 08:41:08.000000 sqlx-exec-2.3.3/sqlexec/page_exec.py
--rw-r--r--   0 summy      (501) staff       (20)    12121 2024-03-27 08:41:08.000000 sqlx-exec-2.3.3/sqlexec/sql_exec.py
--rw-r--r--   0 summy      (501) staff       (20)     3054 2024-03-28 00:30:18.000000 sqlx-exec-2.3.3/sqlexec/sql_support.py
--rw-r--r--   0 summy      (501) staff       (20)    17485 2024-03-27 08:41:08.000000 sqlx-exec-2.3.3/sqlexec/table_exec.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-03-29 02:19:42.991541 sqlx-exec-2.3.3/sqlx_exec.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)     7492 2024-03-29 02:19:42.000000 sqlx-exec-2.3.3/sqlx_exec.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      438 2024-03-29 02:19:42.000000 sqlx-exec-2.3.3/sqlx_exec.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-03-29 02:19:42.000000 sqlx-exec-2.3.3/sqlx_exec.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-03-27 09:08:34.000000 sqlx-exec-2.3.3/sqlx_exec.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)       21 2024-03-29 02:19:42.000000 sqlx-exec-2.3.3/sqlx_exec.egg-info/requires.txt
--rw-r--r--   0 summy      (501) staff       (20)        8 2024-03-29 02:19:42.000000 sqlx-exec-2.3.3/sqlx_exec.egg-info/top_level.txt
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-03-29 02:19:42.992540 sqlx-exec-2.3.3/test/
--rw-r--r--   0 summy      (501) staff       (20)      444 2024-03-25 01:37:05.000000 sqlx-exec-2.3.3/test/test.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-05 02:31:35.277598 sqlx-exec-2.3.4/
+-rw-r--r--   0 summy      (501) staff       (20)    11357 2024-01-23 07:49:56.000000 sqlx-exec-2.3.4/LICENSE
+-rw-r--r--   0 summy      (501) staff       (20)     7493 2024-04-05 02:31:35.276209 sqlx-exec-2.3.4/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)     6974 2024-03-29 02:19:13.000000 sqlx-exec-2.3.4/README.rst
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-04-05 02:31:35.277887 sqlx-exec-2.3.4/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1299 2024-04-05 02:31:24.000000 sqlx-exec-2.3.4/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-05 02:31:35.261004 sqlx-exec-2.3.4/sqlexec/
+-rw-r--r--   0 summy      (501) staff       (20)     1768 2024-03-28 02:42:54.000000 sqlx-exec-2.3.4/sqlexec/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)      637 2024-03-27 13:46:01.000000 sqlx-exec-2.3.4/sqlexec/constant.py
+-rw-r--r--   0 summy      (501) staff       (20)     6901 2024-04-05 02:12:59.000000 sqlx-exec-2.3.4/sqlexec/dialect.py
+-rw-r--r--   0 summy      (501) staff       (20)    13843 2024-03-28 01:00:25.000000 sqlx-exec-2.3.4/sqlexec/exec.py
+-rw-r--r--   0 summy      (501) staff       (20)     1956 2024-03-25 07:14:31.000000 sqlx-exec-2.3.4/sqlexec/loader.py
+-rw-r--r--   0 summy      (501) staff       (20)      816 2024-03-27 08:41:08.000000 sqlx-exec-2.3.4/sqlexec/log_support.py
+-rw-r--r--   0 summy      (501) staff       (20)     1933 2024-03-27 08:41:08.000000 sqlx-exec-2.3.4/sqlexec/page_exec.py
+-rw-r--r--   0 summy      (501) staff       (20)    12121 2024-03-27 08:41:08.000000 sqlx-exec-2.3.4/sqlexec/sql_exec.py
+-rw-r--r--   0 summy      (501) staff       (20)     3054 2024-03-28 00:30:18.000000 sqlx-exec-2.3.4/sqlexec/sql_support.py
+-rw-r--r--   0 summy      (501) staff       (20)    17485 2024-03-27 08:41:08.000000 sqlx-exec-2.3.4/sqlexec/table_exec.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-05 02:31:35.270625 sqlx-exec-2.3.4/sqlx_exec.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)     7493 2024-04-05 02:31:35.000000 sqlx-exec-2.3.4/sqlx_exec.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      438 2024-04-05 02:31:35.000000 sqlx-exec-2.3.4/sqlx_exec.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-05 02:31:35.000000 sqlx-exec-2.3.4/sqlx_exec.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-03-27 09:08:34.000000 sqlx-exec-2.3.4/sqlx_exec.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)       21 2024-04-05 02:31:35.000000 sqlx-exec-2.3.4/sqlx_exec.egg-info/requires.txt
+-rw-r--r--   0 summy      (501) staff       (20)        8 2024-04-05 02:31:35.000000 sqlx-exec-2.3.4/sqlx_exec.egg-info/top_level.txt
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-05 02:31:35.272552 sqlx-exec-2.3.4/test/
+-rw-r--r--   0 summy      (501) staff       (20)      444 2024-03-25 01:37:05.000000 sqlx-exec-2.3.4/test/test.py
```

### Comparing `sqlx-exec-2.3.3/LICENSE` & `sqlx-exec-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-2.3.3/PKG-INFO` & `sqlx-exec-2.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 2.3.3
+Version: 2.3.4
 Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage connections and transactions. Support MySQL, PostgreSQL, SQLite etc.
-Home-page: https://gitee.com/summry/sql-exec
+Home-page: https://gitee.com/summry/sqlx-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python,RDB
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `sqlx-exec-2.3.3/README.rst` & `sqlx-exec-2.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-exec-2.3.3/setup.py` & `sqlx-exec-2.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
     description="A thread safe sql executor for Python with connection pool. It helps you automatically manage connections and transactions. Support MySQL, PostgreSQL, SQLite etc.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='2.3.3',
+    version='2.3.4',
     install_requires=[
         'sqlx-executor>=1.1.1',
     ],
-    url='https://gitee.com/summry/sql-exec',
+    url='https://gitee.com/summry/sqlx-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Oracle', 'SQL Server', 'Database', 'Python', 'RDB'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
     },
```

### Comparing `sqlx-exec-2.3.3/sqlexec/__init__.py` & `sqlx-exec-2.3.4/sqlexec/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-2.3.3/sqlexec/constant.py` & `sqlx-exec-2.3.4/sqlexec/constant.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-2.3.3/sqlexec/dialect.py` & `sqlx-exec-2.3.4/sqlexec/dialect.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 def get_page_start(page_num: int, page_size: int):
     assert page_num >= 1 and page_size >= 1, "'page_name' and 'page_size' should be higher or equal to 1"
     return (page_num - 1) * page_size
 
 
 class BaseDialect:
 
+    def __init__(self, engine: Engine):
+        self.engine = engine
+
     @staticmethod
     def create_insert_sql(table: str, cols: Collection[str]):
         columns, placeholders = zip(*[('{}'.format(col), '?') for col in cols])
         return 'INSERT INTO {}({}) VALUES({})'.format(table, ', '.join(columns), ','.join(placeholders))
 
     @staticmethod
     def before_execute(sql: str):
@@ -158,23 +161,23 @@
 class Dialect:
 
     @classmethod
     def init(cls, engine: Engine):
         global _DIALECT
         if _DIALECT is None:
             if Engine.MYSQL == engine:
-                _DIALECT = MySQLDialect()
+                _DIALECT = MySQLDialect(engine)
             elif Engine.POSTGRESQL == engine:
-                _DIALECT = PostgresDialect()
+                _DIALECT = PostgresDialect(engine)
             elif Engine.ORACLE == engine:
-                _DIALECT = OracleDialect()
+                _DIALECT = OracleDialect(engine)
             elif Engine.SQLITE == engine:
-                _DIALECT = SQLiteDialect()
+                _DIALECT = SQLiteDialect(engine)
             else:
-                _DIALECT = BaseDialect()
+                _DIALECT = BaseDialect(engine)
 
     @staticmethod
     def create_insert_sql(table: str, cols: Collection[str]):
         global _DIALECT
         return _DIALECT.create_insert_sql(table, cols)
 
     @staticmethod
@@ -197,7 +200,12 @@
         global _DIALECT
         return _DIALECT.get_truncate_sql(table_name)
 
     @staticmethod
     def get_select_key(*args, **kwargs):
         global _DIALECT
         return _DIALECT.get_select_key(*args, **kwargs)
+
+    @staticmethod
+    def curr_engine():
+        global _DIALECT
+        return _DIALECT.engine
```

### Comparing `sqlx-exec-2.3.3/sqlexec/exec.py` & `sqlx-exec-2.3.4/sqlexec/exec.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-2.3.3/sqlexec/loader.py` & `sqlx-exec-2.3.4/sqlexec/loader.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-2.3.3/sqlexec/log_support.py` & `sqlx-exec-2.3.4/sqlexec/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-2.3.3/sqlexec/page_exec.py` & `sqlx-exec-2.3.4/sqlexec/page_exec.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-2.3.3/sqlexec/sql_exec.py` & `sqlx-exec-2.3.4/sqlexec/sql_exec.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-2.3.3/sqlexec/sql_support.py` & `sqlx-exec-2.3.4/sqlexec/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-2.3.3/sqlexec/table_exec.py` & `sqlx-exec-2.3.4/sqlexec/table_exec.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-2.3.3/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-2.3.4/sqlx_exec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 2.3.3
+Version: 2.3.4
 Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage connections and transactions. Support MySQL, PostgreSQL, SQLite etc.
-Home-page: https://gitee.com/summry/sql-exec
+Home-page: https://gitee.com/summry/sqlx-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python,RDB
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

