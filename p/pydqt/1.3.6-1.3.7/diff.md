# Comparing `tmp/pydqt-1.3.6.tar.gz` & `tmp/pydqt-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydqt-1.3.6.tar", max compression
+gzip compressed data, was "pydqt-1.3.7.tar", max compression
```

## Comparing `pydqt-1.3.6.tar` & `pydqt-1.3.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    17339 2024-04-04 14:56:15.673262 pydqt-1.3.6/README.md
--rw-r--r--   0        0        0     1202 2024-01-21 00:51:50.668840 pydqt-1.3.6/pydqt/__init__.py
--rw-r--r--   0        0        0    35249 2024-04-04 14:49:31.652917 pydqt-1.3.6/pydqt/pydqt.py
--rw-r--r--   0        0        0     1976 2023-10-21 17:25:29.558640 pydqt-1.3.6/pydqt/sql/templates/macros/macros.jinja
--rw-r--r--   0        0        0    15211 2023-10-23 13:44:10.606676 pydqt-1.3.6/pydqt/test.csv
--rw-r--r--   0        0        0     6669 2024-04-04 14:51:27.612073 pydqt-1.3.6/pydqt/tests/test_querying.py
--rw-r--r--   0        0        0        0 2024-01-18 10:56:59.448321 pydqt-1.3.6/pydqt/utils/__init__.py
--rw-r--r--   0        0        0      237 2024-01-18 10:37:58.921832 pydqt-1.3.6/pydqt/utils/custom_filters.py
--rw-r--r--   0        0        0      319 2024-01-05 09:56:24.111496 pydqt-1.3.6/pydqt/workspaces/main/templates/base.sql
--rw-r--r--   0        0        0      371 2024-01-05 09:56:27.441110 pydqt-1.3.6/pydqt/workspaces/main/templates/example.sql
--rw-r--r--   0        0        0      684 2024-04-04 14:57:26.436994 pydqt-1.3.6/pyproject.toml
--rw-r--r--   0        0        0    18235 1970-01-01 00:00:00.000000 pydqt-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0    17476 2024-04-05 11:55:14.501674 pydqt-1.3.7/README.md
+-rw-r--r--   0        0        0     1202 2024-01-21 00:51:50.668840 pydqt-1.3.7/pydqt/__init__.py
+-rw-r--r--   0        0        0    35253 2024-04-05 11:01:13.511539 pydqt-1.3.7/pydqt/pydqt.py
+-rw-r--r--   0        0        0     1976 2023-10-21 17:25:29.558640 pydqt-1.3.7/pydqt/sql/templates/macros/macros.jinja
+-rw-r--r--   0        0        0    15211 2023-10-23 13:44:10.606676 pydqt-1.3.7/pydqt/test.csv
+-rw-r--r--   0        0        0     6687 2024-04-05 11:52:33.920281 pydqt-1.3.7/pydqt/tests/test_querying.py
+-rw-r--r--   0        0        0        0 2024-01-18 10:56:59.448321 pydqt-1.3.7/pydqt/utils/__init__.py
+-rw-r--r--   0        0        0      237 2024-01-18 10:37:58.921832 pydqt-1.3.7/pydqt/utils/custom_filters.py
+-rw-r--r--   0        0        0      319 2024-01-05 09:56:24.111496 pydqt-1.3.7/pydqt/workspaces/main/templates/base.sql
+-rw-r--r--   0        0        0      371 2024-01-05 09:56:27.441110 pydqt-1.3.7/pydqt/workspaces/main/templates/example.sql
+-rw-r--r--   0        0        0      684 2024-04-05 11:56:23.240091 pydqt-1.3.7/pyproject.toml
+-rw-r--r--   0        0        0    18372 1970-01-01 00:00:00.000000 pydqt-1.3.7/PKG-INFO
```

### Comparing `pydqt-1.3.6/README.md` & `pydqt-1.3.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -278,17 +278,22 @@
 would do:
 
 <pre>
 query.write_sql("my_table", schema="SCHEMA_NAME", append=False, write_timestamp=False, EVENT_DS="DATE")
 </pre>
 
 You can also specify that a column is unique when writing data.  If inserting records this will check both what is already
-there as well as what is being added.  If not append=False, then a new table is created, in which case only the data being
+there as well as what is being added.  If append=False, then a new table is created, in which case only the data being
 added is de-duplicated.  The first record of the specified column sorted in ascending order is the one that is retained.
 
+<pre>
+query.write_sql("my_table", schema="SCHEMA_NAME", append=True, unique="AN_ID_COLUMN", write_timestamp=False, EVENT_DS="DATE")
+</pre>
+
+
 See write_sql help for more details
 
 ### Example 5: testing data
 DQT can test data for simple tests such as non null as well as testing combinations of columns
 
 Get some data:
```

### Comparing `pydqt-1.3.6/pydqt/__init__.py` & `pydqt-1.3.7/pydqt/__init__.py`

 * *Files identical despite different names*

### Comparing `pydqt-1.3.6/pydqt/pydqt.py` & `pydqt-1.3.7/pydqt/pydqt.py`

 * *Files 0% similar despite different names*

```diff
@@ -933,15 +933,15 @@
             template = environment.get_template(filename)
             os.remove(full_filename)
 
             rendered_str = template.render(kwargs)
             pattern = '\'[A-Za-z0-9_.-\/]+\.csv\''
             m=re.findall(pattern, rendered_str)
             if len(m)>0:
-                rendered_str=rendered_str.replace(m[0],f'read_csv_auto({m[0]}, header=true)')
+                rendered_str=rendered_str.replace(m[0],f'read_csv_auto({m[0]}, header=true)')    
             return (False,rendered_str)
         else:
             for key,val in kwargs.items():
                 s=s.replace('{{' + key + '}}',val)
             rendered_str=s                
             pattern = '\'[A-Za-z0-9_.-\/]+\.csv\''
             m=re.findall(pattern, rendered_str)
```

### Comparing `pydqt-1.3.6/pydqt/sql/templates/macros/macros.jinja` & `pydqt-1.3.7/pydqt/sql/templates/macros/macros.jinja`

 * *Files identical despite different names*

### Comparing `pydqt-1.3.6/pydqt/test.csv` & `pydqt-1.3.7/pydqt/test.csv`

 * *Files identical despite different names*

### Comparing `pydqt-1.3.6/pydqt/tests/test_querying.py` & `pydqt-1.3.7/pydqt/tests/test_querying.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,29 @@
     # if not test_data_exists():
     #     create_test_data()
     query = Query(query="select * from '{{table}}' limit 10;",table=full_path_test_data_file())
 
     query.load()
     assert len(query.df)>0  
 
+def test_write_sql_unique_on_append():
+    """
+    tests dqt's writing to sql if unique is specified.  This should prevents any duplicates of a particular column
+    """    
+    query = Query(query="select * from '{{table}}' limit 100;",table=full_path_test_data_file())
+    query.load()
+    df_no_dups = query.df.drop_duplicates(subset=['source'])
+    df_to_append = pd.DataFrame(data=np.array([[pd.to_datetime('2022-01-31'),94,584.37,'US','css'],[pd.to_datetime('2022-03-30'),103,523.10,'NZ','new_source']]),columns=['dates','orders','gmv','region','source'])
+    query.df = pd.concat([df_no_dups, df_to_append]).reset_index(drop=True)
+    query.write_sql("dqt_delme_test",schema="CORE_WIP", database='lyst', append=True, unique='source')
+    query_check = Query(query='select * from dqt_delme_test')
+    query_check.run(schema='core_wip', database='lyst')
+    tf = query_check.df.duplicated(subset=['SOURCE'])
+    assert tf.any()==False
+
 def test_write_sql_create_replace_date():
     """
     tests dqt's writing to sql
     """    
     query = Query(query="select * from '{{table}}' limit 10;",table=full_path_test_data_file())
     query.load()
     query.write_sql("dqt_delme_test",schema="CORE_WIP", append=False, timestamp=False)
@@ -64,28 +79,14 @@
     """
     tests dqt's writing to sql
     """    
     query = Query(query="select * from '{{table}}' limit 10;",table=full_path_test_data_file())
     query.load()
     query.write_sql("dqt_delme_test",schema="CORE_WIP", append=True)
 
-def test_write_sql_unique_on_append():
-    """
-    tests dqt's writing to sql if unique is specified.  This should prevents any duplicates of a particular column
-    """    
-    query = Query(query="select * from '{{table}}' limit 100;",table=full_path_test_data_file())
-    query.load()
-    df_no_dups = query.df.drop_duplicates(subset=['source'])
-    df_to_append = pd.DataFrame(data=np.array([[pd.to_datetime('2022-01-31'),94,584.37,'US','css'],[pd.to_datetime('2022-03-30'),103,523.10,'NZ','new_source']]),columns=['dates','orders','gmv','region','source'])
-    query.df = pd.concat([df_no_dups, df_to_append]).reset_index(drop=True)
-    query.write_sql("dqt_delme_test",schema="CORE_WIP", append=True, unique='source')
-    query_check = Query(query='select * from dqt_delme_test')
-    query_check.run(schema='core_wip', database='lyst')
-    tf = query_check.df.duplicated(subset=['SOURCE'])
-    assert tf.any()==False
 
 def test_write_sql_unique_on_create():
     """
     tests dqt's writing to sql if unique is specified.  This should prevents any duplicates of a particular column
     """    
     query = Query(query="select * from '{{table}}' limit 10;",table=full_path_test_data_file())
     query.load()
```

### Comparing `pydqt-1.3.6/pyproject.toml` & `pydqt-1.3.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydqt"
-version = "1.3.6"
+version = "1.3.7"
 description = "A package to help parameterise and macrofy sql queries"
 authors = ["Mark Ingham <mark.ingham@ly.st>"]
 readme = "README.md"
 repository = "https://github.com/markingham77/dqt"
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `pydqt-1.3.6/PKG-INFO` & `pydqt-1.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydqt
-Version: 1.3.6
+Version: 1.3.7
 Summary: A package to help parameterise and macrofy sql queries
 Home-page: https://github.com/markingham77/dqt
 License: MIT
 Author: Mark Ingham
 Author-email: mark.ingham@ly.st
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
@@ -302,17 +302,22 @@
 would do:
 
 <pre>
 query.write_sql("my_table", schema="SCHEMA_NAME", append=False, write_timestamp=False, EVENT_DS="DATE")
 </pre>
 
 You can also specify that a column is unique when writing data.  If inserting records this will check both what is already
-there as well as what is being added.  If not append=False, then a new table is created, in which case only the data being
+there as well as what is being added.  If append=False, then a new table is created, in which case only the data being
 added is de-duplicated.  The first record of the specified column sorted in ascending order is the one that is retained.
 
+<pre>
+query.write_sql("my_table", schema="SCHEMA_NAME", append=True, unique="AN_ID_COLUMN", write_timestamp=False, EVENT_DS="DATE")
+</pre>
+
+
 See write_sql help for more details
 
 ### Example 5: testing data
 DQT can test data for simple tests such as non null as well as testing combinations of columns
 
 Get some data:
```

