# Comparing `tmp/pypomes_db-0.3.6.tar.gz` & `tmp/pypomes_db-0.3.7.tar.gz`

## Comparing `pypomes_db-0.3.6.tar` & `pypomes_db-0.3.7.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 pypomes_db-0.3.6/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 pypomes_db-0.3.6/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0     9604 2020-02-02 00:00:00.000000 pypomes_db-0.3.6/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 pypomes_db-0.3.6/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    14205 2020-02-02 00:00:00.000000 pypomes_db-0.3.6/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.3.6/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.3.6/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.3.6/README.md
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 pypomes_db-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 pypomes_db-0.3.7/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 pypomes_db-0.3.7/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    10439 2020-02-02 00:00:00.000000 pypomes_db-0.3.7/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0     5209 2020-02-02 00:00:00.000000 pypomes_db-0.3.7/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0     9226 2020-02-02 00:00:00.000000 pypomes_db-0.3.7/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0     8682 2020-02-02 00:00:00.000000 pypomes_db-0.3.7/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.3.7/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.3.7/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.3.7/README.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.3.7/PKG-INFO
```

### Comparing `pypomes_db-0.3.6/src/pypomes_db/__init__.py` & `pypomes_db-0.3.7/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.3.6/src/pypomes_db/db_pomes.py` & `pypomes_db-0.3.7/src/pypomes_db/db_pomes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from logging import Logger
 from typing import Any
 
 from .db_common import DB_ENGINE
 
 match DB_ENGINE:
+    case "oracle":
+        from . import oracle_pomes
     case "postgres":
         from . import postgres_pomes
     case "sqlserver":
         from . import sqlserver_pomes
 
 
 def db_connect(errors: list[str] | None, logger: Logger = None) -> Any:
@@ -24,36 +26,39 @@
             result = postgres_pomes.db_connect(errors, logger)
         case "sqlserver":
             result = sqlserver_pomes.db_connect(errors, logger)
 
     return result
 
 
-def db_exists(errors: list[str] | None, table: str,
+def db_exists(errors: list[str], table: str,
               where_attrs: list[str], where_vals: tuple, logger: Logger = None) -> bool:
     """
     Determine whether the table *table* in the database contains at least one tuple.
 
-    For this determination, the where *where_attrs* are made equal to the
-    *where_values* in the query, respectively.
+    For this determination, *where_attrs* are made equal to *where_values* in the query, respectively.
     If more than one, the attributes are concatenated by the *AND* logical connector.
 
     :param errors: incidental error messages
     :param table: the table to be searched
     :param where_attrs: the search attributes
     :param where_vals: the values for the search attributes
     :param logger: optional logger
     :return: True if at least one tuple was found
     """
-    result: bool | None = None
-    match DB_ENGINE:
-        case "postgres":
-            result = postgres_pomes.db_exists(errors, table, where_attrs, where_vals, logger)
-        case "sqlserver":
-            result = sqlserver_pomes.db_exists(errors, table, where_attrs, where_vals, logger)
+    # noinspection PyDataSource
+    sel_stmt: str = "SELECT * FROM " + table
+    if len(where_attrs) > 0:
+        sel_stmt += " WHERE " + "".join(f"{attr} = %s AND " for attr in where_attrs)[0:-5]
+    rec: tuple = db_select_one(errors=errors,
+                               sel_stmt=sel_stmt,
+                               where_vals=where_vals,
+                               require_nonempty=False,
+                               logger=logger)
+    result: bool = None if len(errors) > 0 else rec is not None
 
     return result
 
 
 def db_select_one(errors: list[str] | None, sel_stmt: str, where_vals: tuple,
                   require_nonempty: bool = False, logger: Logger = None) -> tuple:
     """
@@ -66,22 +71,23 @@
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: values to be associated with the search criteria
     :param require_nonempty: defines whether an empty search should be considered an error
     :param logger: optional logger
     :return: tuple containing the search result, or None if there was an error, or if the search was empty
     """
-    result: tuple | None = None
-    match DB_ENGINE:
-        case "postgres":
-            result = postgres_pomes.db_select_one(errors, sel_stmt, where_vals, require_nonempty, logger)
-        case "sqlserver":
-            result = sqlserver_pomes.db_select_one(errors, sel_stmt, where_vals, require_nonempty, logger)
+    require_min: int = 1 if require_nonempty else None
+    reply: list[tuple] = db_select_all(errors=errors,
+                                       sel_stmt=sel_stmt,
+                                       where_vals=where_vals,
+                                       require_min=require_min,
+                                       require_max=1,
+                                       logger=logger)
 
-    return result
+    return reply[0] if reply else None
 
 
 def db_select_all(errors: list[str] | None, sel_stmt: str,  where_vals: tuple,
                   require_min: int = None, require_max: int = None, logger: Logger = None) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
@@ -96,14 +102,16 @@
     :param require_min: optionally defines the minimum number of tuples to be returned
     :param require_max: optionally defines the maximum number of tuples to be returned
     :param logger: optional logger
     :return: list of tuples containing the search result, or [] if the search is empty
     """
     result: list[tuple] | None = None
     match DB_ENGINE:
+        case "oracle":
+            result = oracle_pomes.db_select_all(errors, sel_stmt, where_vals, require_min, require_max,  logger)
         case "postgres":
             result = postgres_pomes.db_select_all(errors, sel_stmt, where_vals, require_min, require_max,  logger)
         case "sqlserver":
             result = sqlserver_pomes.db_select_all(errors, sel_stmt, where_vals, require_min, require_max, logger)
 
     return result
 
@@ -117,18 +125,20 @@
     :param insert_stmt: the INSERT command
     :param insert_vals: the values to be inserted
     :param logger: optional logger
     :return: the number of inserted tuples (0 ou 1), or None if an error occurred
     """
     result: int | None = None
     match DB_ENGINE:
+        case "oracle":
+            result = oracle_pomes.db_modify(errors, insert_stmt, insert_vals, logger)
         case "postgres":
-            result = postgres_pomes.db_insert(errors, insert_stmt, insert_vals, logger)
+            result = postgres_pomes.db_modify(errors, insert_stmt, insert_vals, logger)
         case "sqlserver":
-            result = sqlserver_pomes.db_insert(errors, insert_stmt, insert_vals, logger)
+            result = sqlserver_pomes.db_modify(errors, insert_stmt, insert_vals, logger)
 
     return result
 
 
 def db_update(errors: list[str] | None, update_stmt: str,
               update_vals: tuple, where_vals: tuple, logger: Logger = None) -> int:
     """
@@ -141,19 +151,22 @@
     :param update_stmt: the UPDATE command
     :param update_vals: the values for the update operation
     :param where_vals: the values to be associated with the search criteria
     :param logger: optional logger
     :return: the number of updated tuples, or None if an error occurred
     """
     result: int | None = None
+    values: tuple = update_vals + where_vals
     match DB_ENGINE:
+        case "oracle":
+            result = oracle_pomes.db_modify(errors, update_stmt, values, logger)
         case "postgres":
-            result = postgres_pomes.db_update(errors, update_stmt, update_vals, where_vals,  logger)
+            result = postgres_pomes.db_modify(errors, update_stmt, values, logger)
         case "sqlserver":
-            result = sqlserver_pomes.db_update(errors, update_stmt, update_vals, where_vals, logger)
+            result = sqlserver_pomes.db_modify(errors, update_stmt, values, logger)
 
     return result
 
 
 def db_delete(errors: list[str] | None, delete_stmt: str,
               where_vals: tuple, logger: Logger = None) -> int:
     """
@@ -165,18 +178,20 @@
     :param delete_stmt: the DELETE command
     :param where_vals: the values to be associated with the search criteria
     :param logger: optional logger
     :return: the number of deleted tuples, or None if an error occurred
     """
     result: int | None = None
     match DB_ENGINE:
+        case "oracle":
+            result = oracle_pomes.db_modify(errors, delete_stmt, where_vals, logger)
         case "postgres":
-            result = postgres_pomes.db_delete(errors, delete_stmt, where_vals,  logger)
+            result = postgres_pomes.db_modify(errors, delete_stmt, where_vals, logger)
         case "sqlserver":
-            result = sqlserver_pomes.db_delete(errors, delete_stmt, where_vals, logger)
+            result = sqlserver_pomes.db_modify(errors, delete_stmt, where_vals, logger)
 
     return result
 
 
 def db_bulk_insert(errors: list[str] | None, insert_stmt: str,
                    insert_vals: list[tuple], logger: Logger = None) -> int:
     """
```

### Comparing `pypomes_db-0.3.6/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.3.7/src/pypomes_db/postgres_pomes.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from psycopg2 import connect
 from psycopg2.extras import execute_values
 # noinspection PyProtectedMember
 from psycopg2._psycopg import connection
 
 from .db_common import (
     DB_NAME, DB_HOST, DB_PORT, DB_PWD, DB_USER,
-    _db_log, _db_except_msg, _db_build_query_msg
+    _assert_query_quota, _db_log, _db_except_msg
 )
 
 
-def db_connect(errors: list[str], logger: Logger = None) -> connection:
+def db_connect(errors: list[str] | None, logger: Logger = None) -> connection:
     """
     Obtain and return a connection to the database, or *None* if the connection cannot be obtained.
 
     :param errors: incidental error messages
     :param logger: optional logger
     :return: the connection to the database
     """
@@ -34,63 +34,15 @@
 
     # log the results
     _db_log(errors, err_msg, logger, f"Connected to '{DB_NAME}'")
 
     return result
 
 
-def db_exists(errors: list[str], table: str,
-              where_attrs: list[str], where_vals: tuple, logger: Logger = None) -> bool:
-    """
-    Determine whether the table *table* in the database contains at least one tuple.
-
-    For this determination, the where *where_attrs* are made equal to the
-    *where_values* in the query, respectively.
-    If more than one, the attributes are concatenated by the *AND* logical connector.
-
-    :param errors: incidental error messages
-    :param table: the table to be searched
-    :param where_attrs: the search attributes
-    :param where_vals: the values for the search attributes
-    :param logger: optional logger
-    :return: True if at least one tuple was found
-    """
-    # noinspection PyDataSource
-    sel_stmt: str = "SELECT * FROM " + table
-    if len(where_attrs) > 0:
-        sel_stmt += " WHERE " + "".join(f"{attr} = %s AND " for attr in where_attrs)[0:-5]
-    rec: tuple = db_select_one(errors, sel_stmt, where_vals, False, logger)
-    result: bool = None if len(errors) > 0 else rec is not None
-
-    return result
-
-
-def db_select_one(errors: list[str], sel_stmt: str,
-                  where_vals: tuple, require_nonempty: bool = False, logger: Logger = None) -> tuple:
-    """
-    Search the database and return the first tuple that satisfies the *sel_stmt* search command.
-
-    The command can optionally contain search criteria, with respective values given
-    in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
-    in a specific tuple. In case of error, or if the search is empty, *None* is returned.
-
-    :param errors: incidental error messages
-    :param sel_stmt: SELECT command for the search
-    :param where_vals: values to be associated with the search criteria
-    :param require_nonempty: defines whether an empty search should be considered an error
-    :param logger: optional logger
-    :return: tuple containing the search result, or None if there was an error, or if the search was empty
-    """
-    require_min: int = 1 if require_nonempty else None
-    reply: list[tuple] = db_select_all(errors, sel_stmt, where_vals, require_min, 1, logger)
-
-    return reply[0] if reply else None
-
-
-def db_select_all(errors: list[str], sel_stmt: str, where_vals: tuple,
+def db_select_all(errors: list[str] | None, sel_stmt: str, where_vals: tuple,
                   require_min: int = None, require_max: int = None, logger: Logger = None) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
@@ -107,149 +59,102 @@
     # initialize the return variable
     result: list[tuple] = []
     if isinstance(require_max, int) and require_max >= 0:
         sel_stmt += f" LIMIT {require_max}"
 
     err_msg: str | None = None
     try:
-        # obtem o cursor e executa a operação
+        # obtain a connection
         with connect(host=DB_HOST,
                      port=DB_PORT,
                      database=DB_NAME,
                      user=DB_USER,
-                     password=DB_PWD) as conn, \
-             conn.cursor() as cursor:
-            cursor.execute(query=f"{sel_stmt};",
-                           vars=where_vals)
-
-            # has a minimum number of tuples been defined but not returned ?
-            if isinstance(require_min, int) and require_min > 0 and cursor.rowcount < require_min:
-                # yes, report the error
-                err_msg = (
-                    f"{cursor.rowcount} tuples returned, at least {require_min} expected, "
-                    f"for '{_db_build_query_msg(sel_stmt, where_vals)}'"
-                )
-            else:
-                # no, obtain the returned tuples
-                result = list(cursor)
+                     password=DB_PWD) as conn:
+            # make sure the connection is not in autocommit mode
+            conn.autocommit = False
+
+            # obtain a cursor and execute the operation
+            with conn.cursor() as cursor:
+                cursor.execute(query=f"{sel_stmt};",
+                               vars=where_vals)
+                # obtain the number of tuples returned
+                count: int = cursor.rowcount
+
+                # has the query quota been satisfied ?
+                if _assert_query_quota(errors, sel_stmt, where_vals, count, require_min, require_max):
+                    # yes, retrieve the returned tuples
+                    result = list(cursor)
 
             # commit the transaction
             conn.commit()
     except Exception as e:
         err_msg = _db_except_msg(e)
 
     # log the results
     _db_log(errors, err_msg, logger, sel_stmt, where_vals)
 
     return result
 
 
-def db_insert(errors: list[str], insert_stmt: str, insert_vals: tuple, logger: Logger = None) -> int:
-    """
-    Insert a tuple, with values defined in *insert_vals*, into the database.
-
-    :param errors: incidental error messages
-    :param insert_stmt: the INSERT command
-    :param insert_vals: the values to be inserted
-    :param logger: optional logger
-    :return: the number of inserted tuples (0 ou 1), or None if an error occurred
-    """
-    return __db_modify(errors, insert_stmt, insert_vals, logger)
-
-
-def db_update(errors: list[str], update_stmt: str,
-              update_vals: tuple, where_vals: tuple, logger: Logger = None) -> int:
-    """
-    Update one or more tuples in the database, as defined by the command *update_stmt*.
-
-    The values for this update are in *update_vals*.
-    The values for selecting the tuples to be updated are in *where_vals*.
-
-    :param errors: incidental error messages
-    :param update_stmt: the UPDATE command
-    :param update_vals: the values for the update operation
-    :param where_vals: the values to be associated with the search criteria
-    :param logger: optional logger
-    :return: the number of updated tuples, or None if an error occurred
-    """
-    values: tuple = update_vals + where_vals
-    return __db_modify(errors, update_stmt, values, logger)
-
-
-def db_delete(errors: list[str], delete_stmt: str, where_vals: tuple, logger: Logger = None) -> int:
-    """
-    Delete one or more tuples in the database, as defined by the *delete_stmt* command.
-
-    The values for selecting the tuples to be deleted are in *where_vals*.
-
-    :param errors: incidental error messages
-    :param delete_stmt: the DELETE command
-    :param where_vals: the values to be associated with the search criteria
-    :param logger: optional logger
-    :return: the number of deleted tuples, or None if an error occurred
-    """
-    return __db_modify(errors, delete_stmt, where_vals, logger)
-
-
 def db_bulk_insert(errors: list[str] | None, insert_stmt: str,
                    insert_vals: list[tuple], logger: Logger = None) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
     The 'VALUES' clause in *insert_stmt' must be simply 'VALUES %s'.
     Note that, after the execution of 'execute_values', the 'cursor.rowcount' property
     will not contain a total result, and thus the value 1 (one) is returned on success.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
     :param logger: optional logger
-    :return: 1 (one), or None if an error occurred
+    :return: the number of inserted tuples, or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
     # execute the bulk insert
     err_msg: str | None = None
     try:
+        # obtain a connection
         with connect(host=DB_HOST,
                      port=DB_PORT,
                      database=DB_NAME,
                      user=DB_USER,
                      password=DB_PWD) as conn:
             # make sure the connection is not in autocommit mode
             conn.autocommit = False
-            # obtain the cursor and execute the operation
+            # obtain a cursor and perform the operation
             with conn.cursor() as cursor:
                 execute_values(cur=cursor,
                                sql=insert_stmt,
                                argslist=insert_vals)
-                result = 1
+                result = len(insert_vals)
             # commit the transaction
             conn.commit()
     except Exception as e:
         err_msg = _db_except_msg(e)
 
     # log the results
     _db_log(errors, err_msg, logger, insert_stmt)
 
     return result
 
 
 def db_exec_stored_procedure(errors: list[str] | None, proc_name: str, proc_vals: tuple,
-                             require_nonempty: bool = False, require_count: int = None,
-                             logger: Logger = None) -> list[tuple]:
+                             require_min: int = None, require_max: int = None, logger: Logger = None) -> list[tuple]:
     """
     Execute the stored procedure *proc_name*, with the arguments given in *proc_vals*.
 
     :param errors:  incidental error messages
     :param proc_name: the name of the sotred procedure
     :param proc_vals: the arguments to be passed
-    :param require_nonempty:
-    :param require_count:
+    :param require_min: optionally defines the minimum number of tuples to be returned
+    :param require_max: optionally defines the maximum number of tuples to be returned
     :param logger: optional logger
     :return: the tuples returned
     """
     # initialize the return variable
     result: list[tuple] = [()]
 
     # build the command
@@ -257,57 +162,46 @@
     for i in range(0, len(proc_vals)):
         proc_stmt += "%s, "
     proc_stmt = f"{proc_stmt[:-2]})"
 
     # execute the stored procedure
     err_msg: str | None = None
     try:
+        # obtain a connection
         with connect(host=DB_HOST,
                      port=DB_PORT,
                      database=DB_NAME,
                      user=DB_USER,
                      password=DB_PWD) as conn:
             # make sure the connection is not in autocommit mode
             conn.autocommit = False
-            # obtain the cursor and execute the operation
+            # obtain a cursor and perform the operation
             with conn.cursor() as cursor:
                 cursor.execute(query=proc_stmt,
                                argslist=proc_vals)
+                # obtain the number of tuples returned
+                count: int = cursor.rowcount
 
-                # has 'require_nonempty' been defined, and the search is empty ?
-                if require_nonempty and cursor.rowcount == 0:
-                    # yes, report the error
-                    err_msg = (
-                        f"No tuple returned in '{DB_NAME}' at '{DB_HOST}', "
-                        f"for stored procedure '{proc_name}', with values '{proc_vals}'"
-                    )
-
-                # has 'require_count' been defined, and a different number of tuples was returned ?
-                elif isinstance(require_count, int) and require_count != cursor.rowcount:
-                    # yes, report the error
-                    err_msg = (
-                        f"{cursor.rowcount} tuples returned, "
-                        f"but {require_count} expected, in '{DB_NAME}' at '{DB_HOST}', "
-                        f"for stored procedure '{proc_name}', with values '{proc_vals}'"
-                    )
-                else:
-                    # obtain the returned tuples
+                # has the query quota been satisfied ?
+                # noinspection PyTypeChecker
+                if _assert_query_quota(errors, proc_name, None, count, require_min, require_max):
+                    # yes, retrieve the returned tuples
                     result = list(cursor)
             # commit the transaction
             conn.commit()
     except Exception as e:
         err_msg = _db_except_msg(e)
 
     # log the results
     _db_log(errors, err_msg, logger, proc_stmt, proc_vals)
 
     return result
 
 
-def __db_modify(errors: list[str], modify_stmt: str, bind_vals: tuple | list[tuple], logger: Logger) -> int:
+def db_modify(errors: list[str] | None, modify_stmt: str, bind_vals: tuple | list[tuple], logger: Logger) -> int:
     """
     Modify the database, inserting, updating or deleting tuples, according to the *modify_stmt* command definitions.
 
     The values for this modification, followed by the values for selecting tuples are in *bind_vals*.
 
     :param errors: incidental error messages
     :param modify_stmt: INSERT, UPDATE, or DELETE command
@@ -316,14 +210,15 @@
     :return: the number of inserted, modified, or deleted tuples, ou None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
     err_msg: str | None = None
     try:
+        # obtain a connection
         with connect(host=DB_HOST,
                      port=DB_PORT,
                      database=DB_NAME,
                      user=DB_USER,
                      password=DB_PWD) as conn:
             # make sure the connection is not in autocommit mode
             conn.autocommit = False
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypomes_db-0.3.6/LICENSE` & `pypomes_db-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.3.6/pyproject.toml` & `pypomes_db-0.3.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.3.6"
+version = "0.3.7"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "pip>=24.0",
+#   "oracledb>=2.1.1",
 #   "psycopg2-binary>=2.9.9",
 #   "pyodbc>=5.1.0",
     "pypomes_core>=0.7.3",
     "setuptools>=68.0.0",
     "wheel>=0.42.0"
 ]
```

### Comparing `pypomes_db-0.3.6/PKG-INFO` & `pypomes_db-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.3.6
+Version: 0.3.7
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

