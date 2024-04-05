# Comparing `tmp/tulona-0.2.0.tar.gz` & `tmp/tulona-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tulona-0.2.0.tar", last modified: Wed Apr  3 02:58:52 2024, max compression
+gzip compressed data, was "tulona-0.2.1.tar", last modified: Fri Apr  5 04:16:51 2024, max compression
```

## Comparing `tulona-0.2.0.tar` & `tulona-0.2.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:58:52.486606 tulona-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-03 02:58:48.000000 tulona-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-03 02:58:52.482606 tulona-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-03 02:58:48.000000 tulona-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:58:52.478606 tulona-0.2.0/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:58:52.478606 tulona-0.2.0/core/tulona/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:58:52.478606 tulona-0.2.0/core/tulona/adapter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:58:52.482606 tulona-0.2.0/core/tulona/adapter/base/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/adapter/base/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/adapter/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/adapter/mssql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/adapter/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/adapter/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/adapter/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:58:52.482606 tulona-0.2.0/core/tulona/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/cli/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:58:52.482606 tulona-0.2.0/core/tulona/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/config/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:58:52.482606 tulona-0.2.0/core/tulona/task/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/task/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/task/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/task/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/task/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/task/test_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:58:52.482606 tulona-0.2.0/core/tulona/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/util/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/util/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/util/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/util/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/util/profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/util/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/util/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/util/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:58:52.482606 tulona-0.2.0/core/tulona.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-03 02:58:52.000000 tulona-0.2.0/core/tulona.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-03 02:58:52.000000 tulona-0.2.0/core/tulona.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:58:52.000000 tulona-0.2.0/core/tulona.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 02:58:52.000000 tulona-0.2.0/core/tulona.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-03 02:58:52.000000 tulona-0.2.0/core/tulona.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:58:52.000000 tulona-0.2.0/core/tulona.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-03 02:58:48.000000 tulona-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 02:58:52.486606 tulona-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:16:51.600195 tulona-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-05 04:16:47.000000 tulona-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-05 04:16:51.600195 tulona-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-05 04:16:47.000000 tulona-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:16:51.592195 tulona-0.2.1/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:16:51.592195 tulona-0.2.1/core/tulona/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:16:51.592195 tulona-0.2.1/core/tulona/adapter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:16:51.592195 tulona-0.2.1/core/tulona/adapter/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/adapter/base/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/adapter/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/adapter/mssql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/adapter/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/adapter/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/adapter/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:16:51.596195 tulona-0.2.1/core/tulona/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     7231 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/cli/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:16:51.596195 tulona-0.2.1/core/tulona/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:16:51.596195 tulona-0.2.1/core/tulona/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13412 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/task/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/task/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/task/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/task/test_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:16:51.596195 tulona-0.2.1/core/tulona/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/util/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/util/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/util/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/util/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/util/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/util/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/util/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-05 04:16:47.000000 tulona-0.2.1/core/tulona/util/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:16:51.596195 tulona-0.2.1/core/tulona.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-05 04:16:51.000000 tulona-0.2.1/core/tulona.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-05 04:16:51.000000 tulona-0.2.1/core/tulona.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 04:16:51.000000 tulona-0.2.1/core/tulona.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-05 04:16:51.000000 tulona-0.2.1/core/tulona.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-05 04:16:51.000000 tulona-0.2.1/core/tulona.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 04:16:51.000000 tulona-0.2.1/core/tulona.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-05 04:16:47.000000 tulona-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 04:16:51.600195 tulona-0.2.1/setup.cfg
```

### Comparing `tulona-0.2.0/LICENSE` & `tulona-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tulona-0.2.0/PKG-INFO` & `tulona-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.2.0
+Version: 0.2.1
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
@@ -104,24 +104,24 @@
   config-version: 1
 
   outdir: output # the folder comparison result is written into
 
   # This is just the list of data sources, doesn't mean tulona will run tasks for all of them.
   # Datasources need to be picked in the CLI command to run tasks against.
   datasources:
-    postgres_postgres_public_employee:
+    employee_postgres:
       connection_profile: pgdb
       database: postgres
       schema: public
       table: employee
       primary_key: employee_id
       exclude_columns:
         - name
       compare_column: Employee_ID
-    mysql_db_db_employee:
+    employee_mysql:
       connection_profile: mydb
       database: db
       schema: db
       table: employee
       primary_key: employee_id
       exclude_columns:
         - phone_number
```

### Comparing `tulona-0.2.0/README.rst` & `tulona-0.2.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -72,24 +72,24 @@
   config-version: 1
 
   outdir: output # the folder comparison result is written into
 
   # This is just the list of data sources, doesn't mean tulona will run tasks for all of them.
   # Datasources need to be picked in the CLI command to run tasks against.
   datasources:
-    postgres_postgres_public_employee:
+    employee_postgres:
       connection_profile: pgdb
       database: postgres
       schema: public
       table: employee
       primary_key: employee_id
       exclude_columns:
         - name
       compare_column: Employee_ID
-    mysql_db_db_employee:
+    employee_mysql:
       connection_profile: mydb
       database: db
       schema: db
       table: employee
       primary_key: employee_id
       exclude_columns:
         - phone_number
```

### Comparing `tulona-0.2.0/core/tulona/adapter/connection.py` & `tulona-0.2.1/core/tulona/adapter/connection.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.0/core/tulona/adapter/mssql.py` & `tulona-0.2.1/core/tulona/adapter/mssql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.0/core/tulona/adapter/mysql.py` & `tulona-0.2.1/core/tulona/adapter/mysql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.0/core/tulona/adapter/postgres.py` & `tulona-0.2.1/core/tulona/adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.0/core/tulona/adapter/snowflake.py` & `tulona-0.2.1/core/tulona/adapter/snowflake.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.0/core/tulona/cli/base.py` & `tulona-0.2.1/core/tulona/cli/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,17 +194,20 @@
 @click.pass_context
 @p.exec_engine
 @p.outdir
 @p.verbose
 @p.datasources
 def compare_column(ctx, **kwargs):
     """
-    Compares columns from two tables, generally primary keys.
-    Columns to compare can be specified with --datasources
-    argument in one of the following formats (column name is same for option 3 and 4):-
+    Column name must be specified for task: compare-column
+    either by specifying 'compare_column' property in
+    at least one of the datasource[project] configs
+    (check sample tulona-project.yml file for example)
+    or with '--datasources' command line argument
+    using one of the following formats (column name is same for option 3 and 4):-
     1. <datasource1>:<col1>,<datasource2>:<col2>
     2. <datasource1>:<col>,<datasource2>:<col>
     3. <datasource1>:<col>,<datasource2>
     4. <datasource1>,<datasource2>:<col>
     """
 
     if "datasources" not in kwargs:
```

### Comparing `tulona-0.2.0/core/tulona/cli/params.py` & `tulona-0.2.1/core/tulona/cli/params.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.0/core/tulona/config/profile.py` & `tulona-0.2.1/core/tulona/config/profile.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.0/core/tulona/config/project.py` & `tulona-0.2.1/core/tulona/config/project.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.0/core/tulona/exceptions.py` & `tulona-0.2.1/core/tulona/exceptions.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.0/core/tulona/task/base.py` & `tulona-0.2.1/core/tulona/task/base.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.0/core/tulona/task/compare.py` & `tulona-0.2.1/core/tulona/task/compare.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             )
 
         df = get_query_output_as_df(connection_manager=conman, query_text=query)
         return df
 
     def get_outfile_fqn(self, ds_list):
         outdir = create_dir_if_not_exist(self.project["outdir"])
-        out_timestamp = datetime.now().strftime("%Y_%m_%d_%H_%M_%S")
+        out_timestamp = datetime.now().strftime("%Y%m%d%H%M%S")
         outfile = f"{'_'.join(ds_list)}_data_comparison_{out_timestamp}.xlsx"
         outfile_fqn = Path(outdir, outfile)
         return outfile_fqn
 
     def execute(self):
         log.info("Starting task: Compare")
         start_time = time.time()
@@ -163,16 +163,18 @@
         else:
             raise TulonaMissingPrimaryKeyError(
                 "Primary key is required for data comparison"
             )
 
         # Exclude columns
         log.debug("Excluding columns")
-        df1 = apply_column_exclusion(df1, ds_dict1, table_name1)
-        df2 = apply_column_exclusion(df2, ds_dict2, table_name2)
+        if 'exclude_columns' in ds_dict1:
+            df1 = apply_column_exclusion(df1, ds_dict1, table_name1)
+        if 'exclude_columns' in ds_dict2:
+            df2 = apply_column_exclusion(df2, ds_dict2, table_name2)
 
         # Compare
         common_columns = list(
             set(df1.columns)
             .intersection(set(df2.columns))
             .union({ds_dict1["primary_key"].lower()})
             .union({ds_dict2["primary_key"].lower()})
@@ -233,15 +235,15 @@
             log.debug(f'Trying quoted column name: "{column}"')
             query = get_column_query(table, column, quoted=True)
             df = get_query_output_as_df(connection_manager=conman, query_text=query)
         return df
 
     def write_result(self, df, ds1, ds2):
         outdir = create_dir_if_not_exist(self.project["outdir"])
-        out_timestamp = datetime.now().strftime("%Y_%m_%d_%H_%M_%S")
+        out_timestamp = datetime.now().strftime("%Y%m%d%H%M%S")
         outfile = f"{ds1}_{ds2}_column_comparison_{out_timestamp}.xlsx"
         outfile_fqn = Path(outdir, outfile)
 
         log.debug(f"Writing output into: {outfile_fqn}")
         df.to_excel(outfile_fqn, sheet_name="Column Comparison", index=False)
 
     def execute(self):
@@ -272,21 +274,23 @@
             column2 = column1
         elif "compare_column" in self.project["datasources"][datasource2]:
             column2 = self.project["datasources"][datasource2]["compare_column"]
             column1 = column2
         else:
             raise TulonaMissingPropertyError(
                 "Column name must be specified for task: compare-column"
-                "either by specifying 'compare_column' property in datasource[project] config"
-                "or with --datasources command line argument"
-                "in one of the following formats (column name is same for option 3 and 4):-"
-                "1. <datasource1>:<col1>,<datasource2>:<col2>"
-                "2. <datasource1>:<col>,<datasource2>:<col>"
-                "3. <datasource1>:<col>,<datasource2>"
-                "4. <datasource1>,<datasource2>:<col>"
+                " either by specifying 'compare_column' property in"
+                " at least one of the datasource[project] configs"
+                " (check sample tulona-project.yml file for example)"
+                " or with '--datasources' command line argument"
+                " using one of the following formats (column name is same for option 3 and 4):-"
+                " 1. <datasource1>:<col1>,<datasource2>:<col2>"
+                " 2. <datasource1>:<col>,<datasource2>:<col>"
+                " 3. <datasource1>:<col>,<datasource2>"
+                " 4. <datasource1>,<datasource2>:<col>"
             )
 
         ds_dict1 = self.project["datasources"][datasource1]
         ds_dict2 = self.project["datasources"][datasource2]
 
         dbtype1 = self.profile["profiles"][
             extract_profile_name(self.project, datasource1)
```

### Comparing `tulona-0.2.0/core/tulona/task/profile.py` & `tulona-0.2.1/core/tulona/task/profile.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                 not isinstance(field.default, _MISSING_TYPE)
                 and getattr(self, field.name) is None
             ):
                 setattr(self, field.name, field.default)
 
     def get_outfile_fqn(self, ds_list):
         outdir = create_dir_if_not_exist(self.project["outdir"])
-        out_timestamp = datetime.now().strftime("%Y_%m_%d_%H_%M_%S")
+        out_timestamp = datetime.now().strftime("%Y%m%d%H%M%S")
         outfile = f"{'_'.join(ds_list)}_profiles_{out_timestamp}.xlsx"
         outfile_fqn = Path(outdir, outfile)
         return outfile_fqn
 
     def execute(self):
 
         log.info("Starting task: profiling")
@@ -142,35 +142,38 @@
 
             df_collection.append(df)
 
         outfile_fqn = self.get_outfile_fqn(ds_name_compressed_list)
 
         if self.compare:
             log.debug("Preparing metadata comparison")
-            common_columns = set(df_collection[0].columns.tolist())
+            common_columns = {c.lower() for c in df_collection[0].columns.tolist()}
             df_collection_final = []
             for ds_name, df in zip(ds_name_compressed_list, df_collection):
-                common_columns = common_columns.intersection(set(df.columns.tolist()))
+                colset = {c.lower() for c in df.columns.tolist()}
+                common_columns = common_columns.intersection(colset)
 
             for ds_name, df in zip(ds_name_compressed_list, df_collection):
                 df = df[list(common_columns)]
                 df = df.rename(
                     columns={
-                        c: f"{c}_{ds_name}" if c != "column_name" else c
+                        c: f"{c}_{ds_name}" if c.lower() != "column_name" else c.lower()
                         for c in df.columns
                     }
                 )
+                df["column_name"] = df["column_name"].str.lower()
                 df_collection_final.append(df)
 
             df_merge = df_collection_final.pop()
             for df in df_collection_final:
                 df_merge = pd.merge(
                     left=df_merge, right=df, on="column_name", how="inner"
                 )
             df_merge = df_merge[sorted(df_merge.columns.tolist())]
+            log.debug(f"Calculated comparison for {df_merge.shape[0]} columns")
 
             log.debug(f"Writing results into file: {outfile_fqn}")
             primary_key_col = df_merge.pop("column_name")
             df_merge.insert(loc=0, column="column_name", value=primary_key_col)
             df_merge.to_excel(outfile_fqn, sheet_name="Metadata Comparison", index=False)
 
             log.debug("Highlighting mismtach cells")
```

### Comparing `tulona-0.2.0/core/tulona/task/scan.py` & `tulona-0.2.1/core/tulona/task/scan.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.0/core/tulona/task/test_connection.py` & `tulona-0.2.1/core/tulona/task/test_connection.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.0/core/tulona/util/database.py` & `tulona-0.2.1/core/tulona/util/database.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.0/core/tulona/util/dataframe.py` & `tulona-0.2.1/core/tulona/util/dataframe.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.0/core/tulona/util/excel.py` & `tulona-0.2.1/core/tulona/util/excel.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,24 +18,24 @@
     ws = wb[sheet]
 
     yellow_fill = styles.PatternFill(
         start_color="FFFFFF00", end_color="FFFFFF00", fill_type="solid"
     )
 
     left_border = Border(
-        left=Side(border_style="thick"),
-        right=Side(border_style="thin"),
-        top=Side(border_style="thick"),
-        bottom=Side(border_style="thick"),
+        left=Side(border_style="thin"),
+        right=Side(border_style="dotted"),
+        top=Side(border_style="thin"),
+        bottom=Side(border_style="thin"),
     )
     right_border = Border(
-        left=Side(border_style="thin"),
-        right=Side(border_style="thick"),
-        top=Side(border_style="thick"),
-        bottom=Side(border_style="thick"),
+        left=Side(border_style="dotted"),
+        right=Side(border_style="thin"),
+        top=Side(border_style="thin"),
+        bottom=Side(border_style="thin"),
     )
 
     for row in ws.iter_rows(
         min_row=2, min_col=0, max_row=ws.max_row, max_col=ws.max_column
     ):
         for col_idx in range(0, ws.max_column, 2):
             if row[col_idx].value != row[col_idx + 1].value:
@@ -55,32 +55,32 @@
     ws = wb[sheet]
 
     yellow_fill = styles.PatternFill(
         start_color="FFFFFF00", end_color="FFFFFF00", fill_type="solid"
     )
 
     left_border = Border(
-        left=Side(border_style="thick"),
-        right=Side(border_style="thin"),
-        top=Side(border_style="thick"),
-        bottom=Side(border_style="thick"),
+        left=Side(border_style="thin"),
+        right=Side(border_style="dotted"),
+        top=Side(border_style="thin"),
+        bottom=Side(border_style="thin"),
     )
 
     middle_border = Border(
-        left=Side(border_style="thin"),
-        right=Side(border_style="thin"),
-        top=Side(border_style="thick"),
-        bottom=Side(border_style="thick"),
+        left=Side(border_style="dotted"),
+        right=Side(border_style="dotted"),
+        top=Side(border_style="thin"),
+        bottom=Side(border_style="thin"),
     )
 
     right_border = Border(
-        left=Side(border_style="thin"),
-        right=Side(border_style="thick"),
-        top=Side(border_style="thick"),
-        bottom=Side(border_style="thick"),
+        left=Side(border_style="dotted"),
+        right=Side(border_style="thin"),
+        top=Side(border_style="thin"),
+        bottom=Side(border_style="thin"),
     )
 
     if skip_columns:
         skip_columns = skip_columns if isinstance(skip_columns, list) else [skip_columns]
         skip_idxs = [get_column_index(ws, c) - 1 for c in skip_columns]
         compareable_col_idxs = list(set(range(ws.max_column)) - set(skip_idxs))
     else:
```

### Comparing `tulona-0.2.0/core/tulona/util/filesystem.py` & `tulona-0.2.1/core/tulona/util/filesystem.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.0/core/tulona/util/profiles.py` & `tulona-0.2.1/core/tulona/util/profiles.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.0/core/tulona/util/sql.py` & `tulona-0.2.1/core/tulona/util/sql.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,31 +52,30 @@
     return query_expr
 
 
 def get_metadata_query(database, schema, table):
     if database:
         query = f"""
         select * from information_schema.columns
-        where table_catalog = '{database}'
-        and table_schema = '{schema}'
-        and table_name = '{table}'
+        where upper(table_catalog) = '{database.upper()}'
+        and upper(table_schema) = '{schema.upper()}'
+        and upper(table_name) = '{table.upper()}'
         """
     else:
         query = f"""
         select * from information_schema.columns
-        where table_schema = '{schema}'
-        and table_name = '{table}'
+        where upper(table_schema) = '{schema.upper()}'
+        and upper(table_name) = '{table.upper()}'
         """
     return query
 
 
 def get_metric_query(
     database, schema, table, columns_dtype: Dict, metrics: list, quoted=False
 ):
-    # TODO: add support for date/timestamp
     numeric_types = [
         "smallint",
         "integer",
         "bigint",
         "decimal",
         "numeric",
         "real",
@@ -109,54 +108,54 @@
         "datetime2",
         "timestamp_tz",
         "timestamp_ltz",
         "timestamp_ntz",
         "timestamp with time zone",  # TODO probably incorrect representation
         "timestamp without time zone",
     ]
+
     numeric_funcs = [
         "min",
         "max",
         "average",
         "avg",
     ]
     timestamp_funcs = [
         "min",
         "max",
     ]
+    generic_funcs = [
+        "count",
+        "distinct_count",
+    ]
 
     function_map = {
         "min": "min({}) as {}_min",
         "max": "max({}) as {}_max",
         "avg": "avg({}) as {}_avg",
         "average": "avg({}) as {}_average",
         "count": "count({}) as {}_count",
         "distinct_count": "count(distinct({})) as {}_distinct_count",
     }
 
     call_funcs = []
     for col, dtype in columns_dtype.items():
-        if quoted:
-            qp = []
-            for m in metrics:
-                if (m in numeric_funcs and dtype not in numeric_types) or (
-                    m in timestamp_funcs and dtype not in timestamp_types
-                ):
-                    qp.append(f"'NA' as {col}_{m.lower()}")
-                else:
-                    qp.append(function_map[m.lower()].format(f'"{col}"', col))
-        else:
-            qp = []
-            for m in metrics:
-                if (m in numeric_funcs and dtype not in numeric_types) or (
-                    m in timestamp_funcs and dtype not in timestamp_types
-                ):
-                    qp.append(f"'NA' as {col}_{m.lower()}")
-                else:
-                    qp.append(function_map[m.lower()].format(col, col))
+        dtype = dtype.lower()
+        qp = []
+        for m in metrics:
+            if (
+                (m in numeric_funcs and dtype in numeric_types)
+                or (m in timestamp_funcs and dtype in timestamp_types)
+                or (m in generic_funcs)
+            ):
+                qp.append(
+                    function_map[m.lower()].format(f'"{col}"' if quoted else col, col)
+                )
+            else:
+                qp.append(f"'NA' as {col}_{m.lower()}")
         call_funcs.extend(qp)
 
     table_fqn = f"{database if database else ''}{'.' if database else ''}{schema}.{table}"
 
     query = f"""
     select
         {", ".join(call_funcs)}
```

### Comparing `tulona-0.2.0/core/tulona.egg-info/PKG-INFO` & `tulona-0.2.1/core/tulona.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.2.0
+Version: 0.2.1
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
@@ -104,24 +104,24 @@
   config-version: 1
 
   outdir: output # the folder comparison result is written into
 
   # This is just the list of data sources, doesn't mean tulona will run tasks for all of them.
   # Datasources need to be picked in the CLI command to run tasks against.
   datasources:
-    postgres_postgres_public_employee:
+    employee_postgres:
       connection_profile: pgdb
       database: postgres
       schema: public
       table: employee
       primary_key: employee_id
       exclude_columns:
         - name
       compare_column: Employee_ID
-    mysql_db_db_employee:
+    employee_mysql:
       connection_profile: mydb
       database: db
       schema: db
       table: employee
       primary_key: employee_id
       exclude_columns:
         - phone_number
```

### Comparing `tulona-0.2.0/core/tulona.egg-info/SOURCES.txt` & `tulona-0.2.1/core/tulona.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tulona-0.2.0/pyproject.toml` & `tulona-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tulona"
-version = "0.2.0"
+version = "0.2.1"
 description = "A tool to compare data from different sources."
 dependencies = [
   "click~=8.1",
   "ruamel.yaml~=0.18",
   "psycopg2-binary~=2.9",
   "pymysql~=1.1",
   "cryptography~=42.0",
```

