# Comparing `tmp/sqlx-orm-0.0.2.tar.gz` & `tmp/sqlx-orm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlx-orm-0.0.2.tar", last modified: Thu Apr  4 10:08:35 2024, max compression
+gzip compressed data, was "sqlx-orm-0.0.3.tar", last modified: Fri Apr  5 02:42:34 2024, max compression
```

## Comparing `sqlx-orm-0.0.2.tar` & `sqlx-orm-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-04 10:08:35.456204 sqlx-orm-0.0.2/
--rw-r--r--   0 summy      (501) staff       (20)     2145 2024-04-04 10:08:35.455385 sqlx-orm-0.0.2/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)     1733 2024-04-04 10:08:32.000000 sqlx-orm-0.0.2/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-04 10:08:35.448193 sqlx-orm-0.0.2/orm/
--rw-r--r--   0 summy      (501) staff       (20)      288 2024-04-04 08:43:34.000000 sqlx-orm-0.0.2/orm/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)      867 2024-04-04 01:04:08.000000 sqlx-orm-0.0.2/orm/constant.py
--rw-r--r--   0 summy      (501) staff       (20)     3657 2024-04-04 01:03:37.000000 sqlx-orm-0.0.2/orm/log_support.py
--rw-r--r--   0 summy      (501) staff       (20)    29103 2024-04-04 01:10:00.000000 sqlx-orm-0.0.2/orm/orm.py
--rw-r--r--   0 summy      (501) staff       (20)    12126 2024-04-04 01:02:32.000000 sqlx-orm-0.0.2/orm/orm_support.py
--rw-r--r--   0 summy      (501) staff       (20)     2603 2024-04-04 01:12:05.000000 sqlx-orm-0.0.2/orm/snowflake.py
--rw-r--r--   0 summy      (501) staff       (20)      991 2024-04-04 01:12:05.000000 sqlx-orm-0.0.2/orm/sql_support.py
--rw-r--r--   0 summy      (501) staff       (20)      128 2024-04-04 01:12:05.000000 sqlx-orm-0.0.2/orm/support.py
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-04-04 10:08:35.456496 sqlx-orm-0.0.2/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1206 2024-04-04 10:08:32.000000 sqlx-orm-0.0.2/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-04 10:08:35.454157 sqlx-orm-0.0.2/sqlx_orm.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)     2145 2024-04-04 10:08:35.000000 sqlx-orm-0.0.2/sqlx_orm.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      341 2024-04-04 10:08:35.000000 sqlx-orm-0.0.2/sqlx_orm.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-04 10:08:35.000000 sqlx-orm-0.0.2/sqlx_orm.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-04 10:07:39.000000 sqlx-orm-0.0.2/sqlx_orm.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)       17 2024-04-04 10:08:35.000000 sqlx-orm-0.0.2/sqlx_orm.egg-info/requires.txt
--rw-r--r--   0 summy      (501) staff       (20)        4 2024-04-04 10:08:35.000000 sqlx-orm-0.0.2/sqlx_orm.egg-info/top_level.txt
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-05 02:42:34.337436 sqlx-orm-0.0.3/
+-rw-r--r--   0 summy      (501) staff       (20)     2145 2024-04-05 02:42:34.336516 sqlx-orm-0.0.3/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)     1733 2024-04-04 10:08:32.000000 sqlx-orm-0.0.3/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-05 02:42:34.323202 sqlx-orm-0.0.3/orm/
+-rw-r--r--   0 summy      (501) staff       (20)      288 2024-04-04 08:43:34.000000 sqlx-orm-0.0.3/orm/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     1036 2024-04-05 02:16:39.000000 sqlx-orm-0.0.3/orm/constant.py
+-rw-r--r--   0 summy      (501) staff       (20)     2344 2024-04-05 02:37:00.000000 sqlx-orm-0.0.3/orm/log_support.py
+-rw-r--r--   0 summy      (501) staff       (20)    29422 2024-04-05 02:30:25.000000 sqlx-orm-0.0.3/orm/orm.py
+-rw-r--r--   0 summy      (501) staff       (20)    12045 2024-04-05 02:41:28.000000 sqlx-orm-0.0.3/orm/orm_support.py
+-rw-r--r--   0 summy      (501) staff       (20)     2603 2024-04-04 01:12:05.000000 sqlx-orm-0.0.3/orm/snowflake.py
+-rw-r--r--   0 summy      (501) staff       (20)      128 2024-04-04 01:12:05.000000 sqlx-orm-0.0.3/orm/support.py
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-04-05 02:42:34.338098 sqlx-orm-0.0.3/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1209 2024-04-05 02:37:00.000000 sqlx-orm-0.0.3/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-05 02:42:34.334054 sqlx-orm-0.0.3/sqlx_orm.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)     2145 2024-04-05 02:42:34.000000 sqlx-orm-0.0.3/sqlx_orm.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      322 2024-04-05 02:42:34.000000 sqlx-orm-0.0.3/sqlx_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-05 02:42:34.000000 sqlx-orm-0.0.3/sqlx_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-04 10:07:39.000000 sqlx-orm-0.0.3/sqlx_orm.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)       17 2024-04-05 02:42:34.000000 sqlx-orm-0.0.3/sqlx_orm.egg-info/requires.txt
+-rw-r--r--   0 summy      (501) staff       (20)        4 2024-04-05 02:42:34.000000 sqlx-orm-0.0.3/sqlx_orm.egg-info/top_level.txt
```

### Comparing `sqlx-orm-0.0.2/PKG-INFO` & `sqlx-orm-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-orm
-Version: 0.0.2
+Version: 0.0.3
 Summary: A single table ORM framework for python. Support MySQL, PostgreSQL, SQLite etc.
 Home-page: https://gitee.com/summry/sqlx-orm
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python,RDB
 Platform: UNKNOWN
```

### Comparing `sqlx-orm-0.0.2/README.rst` & `sqlx-orm-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-orm-0.0.2/orm/constant.py` & `sqlx-orm-0.0.3/orm/constant.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,10 +16,13 @@
 POSTGRES_COLUMN_SQL = '''SELECT array_to_string(array_agg(column_name),',') as column_name FROM information_schema.columns 
                           WHERE table_schema='public' and table_name = ? LIMIT ?'''
 
 DYNAMIC_REGEX = '{%|{{|}}|%}'
 
 DEFAULT_KEY_FIELD = 'id'
 
-KEY, SELECT_KEY, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, KEY_STRATEGY = '__key__', '__select_key__', '__table__', '__update_by__', '__update_time__',\
-    '__del_flag__', '__key_strategy__'
+KEY, SELECT_KEY, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, KEY_STRATEGY = '__key__', '__select_key__', '__table__', \
+                                                                         '__update_by__', '__update_time__',\
+                                                                         '__del_flag__', '__key_strategy__'
+
+KEY_SEQ = '__key_seq__'
```

### Comparing `sqlx-orm-0.0.2/orm/log_support.py` & `sqlx-orm-0.0.3/orm/log_support.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,10 @@
 from sqlexec.log_support import logger
 
 
-def save_log(table, **kwargs):
-    logger.debug("Exec func 'pgsqlx.db.save' \n\t Table: '%s', kwargs: %s" % (table, kwargs))
-
-
-def do_page_log(function: str, sql: str, page_num, page_size, *args):
-    logger.debug(
-        "Exec func 'sqlbatis.db.%s', page_num: %d, page_size: %d \n\t sql: %s \n\t args: %s" % (function, page_num, page_size, sql.strip(), args))
-
-
-def page_log(function: str, sql: str, page_num, page_size, *args, **kwargs):
-    logger.debug("Exec func 'sqlbatis.db.%s', page_num: %d, page_size: %d \n\tsql: %s \n\targs: %s \n\tkwargs: %s" % (
-                 function, page_num, page_size, sql.strip(), args, kwargs))
-
-
-def page_sql_id_log(function: str, sql_id: str, page_num, page_size, *args, **kwargs):
-    logger.debug("Exec func 'sqlbatis.dbx.%s', page_num: %d, page_size: %d, sql_id: %s, args: %s, kwargs: %s" % (function, page_num, page_size, sql_id, args, kwargs))
-
-
-def sql_id_log(function: str, sql_id: str, *args, **kwargs):
-    logger.debug("Exec func '%s', sql_id: %s, args: %s, kwargs: %s" % (function, sql_id.strip(), args, kwargs))
-
-
-def sql_id_select_key_log(function: str, select_key: str, sql_id: str, *args, **kwargs):
-    logger.debug("Exec func 'sqlbatis.dbx.%s', select_key: %s, sql_id: %s, args: %s, kwargs: %s" % (function, select_key, sql_id.strip(), args, kwargs))
-
-
 def orm_insert_log(function, class_name, **kwargs):
     logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', kwargs: %s" % (function, class_name, kwargs))
 
 
 def orm_delete_by_id_log(function, class_name, _id, update_by):
     logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', id: %d, update_by: %s" % (function, class_name, _id, update_by))
```

### Comparing `sqlx-orm-0.0.2/orm/orm.py` & `sqlx-orm-0.0.3/orm/orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import sys
 from datetime import datetime
 from enum import Enum, IntEnum
 from typing import Sequence, Union
 from .snowflake import get_snowflake_id
 from .support import DBError, NotFoundError
 from . import db, log_support, transaction, orm_support, Dialect
-from .constant import LIMIT_1, NO_LIMIT, DEFAULT_KEY_FIELD, KEY, SELECT_KEY, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, KEY_STRATEGY
+from .constant import LIMIT_1, NO_LIMIT, DEFAULT_KEY_FIELD, KEY, SELECT_KEY, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, \
+    KEY_STRATEGY, KEY_SEQ
 
 
 class DelFlag(IntEnum):
     UN_DELETE = 0
     DELETED = 1
 
 
@@ -205,16 +206,18 @@
             kwargs[key] = get_snowflake_id()
             db.insert(table, **kwargs)
             return kwargs[key]
         else:
             select_key = cls._get_select_key()
             if not select_key:
                 try:
-                    select_key = Dialect.get_select_key(table=table, key=key)
+                    select_key = Dialect.get_select_key(keq_seq=cls._get_key_seq(), table=table, key=key)
                 except NotImplementedError:
+                    if Dialect.curr_engine() == db.Engine.POSTGRESQL:
+                        raise DBError(f"Expect 'key_seq' or 'select_key'. you can set it in model class with '__key_seq__' or '__select_key__'.")
                     raise DBError(f"Expect 'select_key'. you can set it in model class with '__select_key__'.")
             return db.save_select_key(select_key, table, **kwargs)
 
     @classmethod
     def create(cls, **kwargs):
         """
         person = Person.create(name='张三', age=20)
@@ -351,15 +354,15 @@
         if key_strategy == KeyStrategy.SNOWFLAKE:
             for arg in args:
                 if key not in arg:
                     arg[key] = get_snowflake_id()
 
         return db.batch_insert(table, *args)
 
-    # ------------------------------------------------Class query method--------------------------------------------------------
+    # ------------------------------------------------Class query method------------------------------------------------
     @classmethod
     def count(cls, **kwargs):
         """
         count = Person.count(name='张三', age=55)
         """
         log_support.orm_count_log('count', cls.__name__, **kwargs)
         table = cls.get_table()
@@ -586,15 +589,15 @@
                 return {k: v for k, v in self.__dict__.items() if v is not None and k in fields}
             return {k: v for k, v in self.__dict__.items() if k in fields}
 
         if ignored_none:
             return {k: v for k, v in self.__dict__.items() if v is not None}
         return {k: v for k, v in self.__dict__.items()}
 
-    # ------------------------------------------------Private class method------------------------------------------------------------------
+    # ------------------------------------------------Private class method----------------------------------------------
     @classmethod
     def _logical_delete_by_id_op(cls, _id: Union[int, str], update_by: Union[int, str] = None, del_status=DelFlag.DELETED):
         key, table = cls._get_key_and_table()
         del_flag_field = cls._get_del_flag_field()
         update_by_field = cls._get_update_by_field()
 
         where = '%s = ?' % key
@@ -648,17 +651,19 @@
         if hasattr(cls, KEY):
             return cls.__key__
         log_support.logger.warning("%s not set attribute '%s'" % (cls.__name__, KEY))
         return DEFAULT_KEY_FIELD
 
     @classmethod
     def _get_select_key(cls):
-        if hasattr(cls, SELECT_KEY):
-            return cls.__select_key__
-        return None
+        return cls.__select_key__ if hasattr(cls, SELECT_KEY) else None
+
+    @classmethod
+    def _get_key_seq(cls):
+        return cls.__key_seq__ if hasattr(cls, KEY_SEQ) else None
 
     @classmethod
     def get_table(cls):
         if hasattr(cls, TABLE):
             return cls.__table__
         log_support.logger.warning("%s not set attribute '%s'" % (cls.__name__, TABLE))
         return orm_support.get_table_name(cls.__name__)
```

### Comparing `sqlx-orm-0.0.2/orm/orm_support.py` & `sqlx-orm-0.0.3/orm/orm_support.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-from .constant import NO_LIMIT
-from .sql_support import simple_sql, get_table_select_sql
+from sqlexec.sql_support import get_table_select_sql
 from typing import Sequence, Union, List, Tuple
 from sqlexec.table_exec import get_condition_arg, get_where_arg_limit
-from . import db
-from sqlexec import Dialect
 
 
 class FieldExec:
     def __init__(self, cls, *fields):
         self.cls = cls
         self.fields = fields
```

### Comparing `sqlx-orm-0.0.2/orm/snowflake.py` & `sqlx-orm-0.0.3/orm/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlx-orm-0.0.2/setup.py` & `sqlx-orm-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import os
 from setuptools import setup
 
+
 # INSTALL_PACKAGES = open(path.join(DIR, 'requirements.txt')).read().splitlines()
 def read(rel_path: str) -> str:
     here = os.path.abspath(os.path.dirname(__file__))
     # intentionally *not* adding an encoding option to open, See:
     #   https://github.com/pypa/virtualenv/issues/201#issuecomment-3145690
     with open(os.path.join(here, rel_path), 'r', encoding='UTF-8') as fp:
         return fp.read()
 
+
 long_description = read("README.rst")
 
+
 setup(
     name='sqlx-orm',
     packages=['orm'],
     description="A single table ORM framework for python. Support MySQL, PostgreSQL, SQLite etc.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.0.2',
+    version='0.0.3',
     install_requires=[
-        'sqlx-exec>=2.3.3',
+        'sqlx-exec>=2.3.4',
     ],
     url='https://gitee.com/summry/sqlx-orm',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Oracle', 'SQL Server', 'Database', 'Python', 'RDB'],
     package_data={
         # include json and txt files
```

### Comparing `sqlx-orm-0.0.2/sqlx_orm.egg-info/PKG-INFO` & `sqlx-orm-0.0.3/sqlx_orm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-orm
-Version: 0.0.2
+Version: 0.0.3
 Summary: A single table ORM framework for python. Support MySQL, PostgreSQL, SQLite etc.
 Home-page: https://gitee.com/summry/sqlx-orm
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python,RDB
 Platform: UNKNOWN
```

