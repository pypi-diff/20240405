# Comparing `tmp/SQLDataModel-0.3.3.tar.gz` & `tmp/SQLDataModel-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLDataModel-0.3.3.tar", last modified: Wed Apr  3 22:34:10 2024, max compression
+gzip compressed data, was "SQLDataModel-0.3.4.tar", last modified: Fri Apr  5 20:08:36 2024, max compression
```

## Comparing `SQLDataModel-0.3.3.tar` & `SQLDataModel-0.3.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 22:34:10.948078 SQLDataModel-0.3.3/
--rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 SQLDataModel-0.3.3/LICENSE
--rw-rw-rw-   0        0        0    27185 2024-04-03 22:34:10.943078 SQLDataModel-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0    25313 2024-04-01 18:33:13.000000 SQLDataModel-0.3.3/README.md
--rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 SQLDataModel-0.3.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 22:34:10.949077 SQLDataModel-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     2312 2024-04-03 22:33:17.000000 SQLDataModel-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 22:34:09.587853 SQLDataModel-0.3.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 22:34:10.719510 SQLDataModel-0.3.3/src/SQLDataModel/
--rw-rw-rw-   0        0        0     6899 2024-03-19 22:34:49.000000 SQLDataModel-0.3.3/src/SQLDataModel/ANSIColor.py
--rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 SQLDataModel-0.3.3/src/SQLDataModel/HTMLParser.py
--rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 SQLDataModel-0.3.3/src/SQLDataModel/JSONEncoder.py
--rw-rw-rw-   0        0        0   543039 2024-04-03 22:30:42.000000 SQLDataModel-0.3.3/src/SQLDataModel/SQLDataModel.py
--rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 SQLDataModel-0.3.3/src/SQLDataModel/StandardDeviation.py
--rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 SQLDataModel-0.3.3/src/SQLDataModel/__init__.py
--rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 SQLDataModel-0.3.3/src/SQLDataModel/converters.py
--rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 SQLDataModel-0.3.3/src/SQLDataModel/demo.py
--rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 SQLDataModel-0.3.3/src/SQLDataModel/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-03 22:34:10.873275 SQLDataModel-0.3.3/src/SQLDataModel/extensions/
--rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 SQLDataModel-0.3.3/src/SQLDataModel/extensions/__init__.py
--rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 SQLDataModel-0.3.3/src/SQLDataModel/extensions/str_utils.c
-drwxrwxrwx   0        0        0        0 2024-04-03 22:34:10.939078 SQLDataModel-0.3.3/src/SQLDataModel.egg-info/
--rw-rw-rw-   0        0        0    27185 2024-04-03 22:34:09.000000 SQLDataModel-0.3.3/src/SQLDataModel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2024-04-03 22:34:09.000000 SQLDataModel-0.3.3/src/SQLDataModel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 22:34:09.000000 SQLDataModel-0.3.3/src/SQLDataModel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-03 22:34:09.000000 SQLDataModel-0.3.3/src/SQLDataModel.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-03 22:34:10.884274 SQLDataModel-0.3.3/tests/
--rw-rw-rw-   0        0        0    41468 2024-04-01 21:30:07.000000 SQLDataModel-0.3.3/tests/test_Future.py
--rw-rw-rw-   0        0        0    41471 2024-04-01 21:30:05.000000 SQLDataModel-0.3.3/tests/test_SQLDataModel.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:08:36.399945 SQLDataModel-0.3.4/
+-rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 SQLDataModel-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0    27185 2024-04-05 20:08:36.391336 SQLDataModel-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0    25313 2024-04-01 18:33:13.000000 SQLDataModel-0.3.4/README.md
+-rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 SQLDataModel-0.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 20:08:36.400946 SQLDataModel-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     2312 2024-04-05 20:07:12.000000 SQLDataModel-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:08:34.140985 SQLDataModel-0.3.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 20:08:35.503520 SQLDataModel-0.3.4/src/SQLDataModel/
+-rw-rw-rw-   0        0        0     6899 2024-03-19 22:34:49.000000 SQLDataModel-0.3.4/src/SQLDataModel/ANSIColor.py
+-rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 SQLDataModel-0.3.4/src/SQLDataModel/HTMLParser.py
+-rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 SQLDataModel-0.3.4/src/SQLDataModel/JSONEncoder.py
+-rw-rw-rw-   0        0        0   555539 2024-04-05 20:06:19.000000 SQLDataModel-0.3.4/src/SQLDataModel/SQLDataModel.py
+-rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 SQLDataModel-0.3.4/src/SQLDataModel/StandardDeviation.py
+-rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 SQLDataModel-0.3.4/src/SQLDataModel/__init__.py
+-rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 SQLDataModel-0.3.4/src/SQLDataModel/converters.py
+-rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 SQLDataModel-0.3.4/src/SQLDataModel/demo.py
+-rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 SQLDataModel-0.3.4/src/SQLDataModel/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:08:36.304262 SQLDataModel-0.3.4/src/SQLDataModel/extensions/
+-rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 SQLDataModel-0.3.4/src/SQLDataModel/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 SQLDataModel-0.3.4/src/SQLDataModel/extensions/str_utils.c
+drwxrwxrwx   0        0        0        0 2024-04-05 20:08:36.384334 SQLDataModel-0.3.4/src/SQLDataModel.egg-info/
+-rw-rw-rw-   0        0        0    27185 2024-04-05 20:08:33.000000 SQLDataModel-0.3.4/src/SQLDataModel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2024-04-05 20:08:34.000000 SQLDataModel-0.3.4/src/SQLDataModel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 20:08:33.000000 SQLDataModel-0.3.4/src/SQLDataModel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-05 20:08:33.000000 SQLDataModel-0.3.4/src/SQLDataModel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 20:08:36.320693 SQLDataModel-0.3.4/tests/
+-rw-rw-rw-   0        0        0    48008 2024-04-05 19:51:59.000000 SQLDataModel-0.3.4/tests/test_Future.py
+-rw-rw-rw-   0        0        0    48011 2024-04-05 19:52:16.000000 SQLDataModel-0.3.4/tests/test_SQLDataModel.py
```

### Comparing `SQLDataModel-0.3.3/LICENSE` & `SQLDataModel-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.3/PKG-INFO` & `SQLDataModel-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.3.3
+Version: 0.3.4
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package
```

### Comparing `SQLDataModel-0.3.3/README.md` & `SQLDataModel-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.3/setup.py` & `SQLDataModel-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='SQLDataModel',  
-     version='0.3.3',
+     version='0.3.4',
      scripts=['src/SQLDataModel/SQLDataModel.py'] ,
      author='Ante Tonkovic-Capin',
      author_email='antetc@icloud.com',
      description='SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.',
      keywords='SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package',
      license_file='LICENSE',
      long_description=long_description,
```

### Comparing `SQLDataModel-0.3.3/src/SQLDataModel/ANSIColor.py` & `SQLDataModel-0.3.4/src/SQLDataModel/ANSIColor.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.3/src/SQLDataModel/HTMLParser.py` & `SQLDataModel-0.3.4/src/SQLDataModel/HTMLParser.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.3/src/SQLDataModel/JSONEncoder.py` & `SQLDataModel-0.3.4/src/SQLDataModel/JSONEncoder.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.3/src/SQLDataModel/SQLDataModel.py` & `SQLDataModel-0.3.4/src/SQLDataModel/SQLDataModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -847,20 +847,28 @@
             ID as ID
             ID as ID_2
             Name as Name
             Name as Name_2
             Name as Name_3
             Unique as Unique
         ```
+
+        Change Log:
+            - Version 0.3.4 (2024-04-05):
+                - Modified to re-alias partially aliased input to prevent runaway incrementation on suffixes.
         """        
         dupes = {}
         for col in headers:
             if col in dupes:
                 dupes[col] += 1
-                yield f"{col}_{dupes[col]}"
+                new_col = f"{col}_{dupes[col]}"
+                while new_col in headers:
+                    dupes[col] += 1
+                    new_col = f"{col}_{dupes[col]}"
+                yield new_col
             else:
                 dupes[col] = 1
                 yield col
     
     @staticmethod
     def flatten_json(json_source:list|dict, flatten_rows:bool=True, level_sep:str='_', key_prefix:str=None) -> dict:
         """
@@ -7949,14 +7957,123 @@
         ```
 
         Note:
             - See related :meth:`SQLDataModel.tail()` for the opposite, grabbing the bottom ``n_rows`` from the current model.
         
         """
         return self.execute_fetch(self._generate_unordered_sql_stmt(n_rows, ordering="asc"))
+                    
+    def hstack(self, *other:SQLDataModel, inplace:bool=False) -> SQLDataModel:
+        """
+        Horizontally stacks one or more ``SQLDataModel`` objects to the current model.
+
+        Parameters:
+            ``other`` (SQLDataModel or sequence of): The SQLDataModel objects to horizontally stack.
+            ``inplace`` (bool, optional): If True, performs the horizontal stacking in-place, modifying the current model. Defaults to False, returning a new ``SQLDataModel``.
+
+        Returns:
+            ``SQLDataModel``: The horizontally stacked SQLDataModel instance when inplace is False.
+
+        Raises:
+            ``ValueError``: If no additional SQLDataModels are provided for horizontal stacking.
+            ``TypeError``: If any argument in 'other' is not of type SQLDataModel, list, or tuple.
+            ``SQLProgrammingError``: If an error occurs when updating the model values in place.            
+
+        Example::
+
+            from SQLDataModel import SQLDataModel
+
+            # Create models A and B
+            sdm_a = SQLDataModel([('A', 'B'), ('1', '2')], headers=['A1', 'A2'])
+            sdm_b = SQLDataModel([('C', 'D'), ('3', '4')], headers=['B1', 'B2'])
+
+            # Horizontally stack B onto A
+            sdm_ab = sdm_a.hstack(sdm_b)
+
+            # View stacked model
+            print(sdm_ab)
+
+        This will output the result of stacking B onto A, using the each model's headers and dtypes:    
+
+        ```shell
+            ┌─────┬─────┬─────┬─────┐
+            │ A1  │ A2  │ B1  │ B2  │
+            ├─────┼─────┼─────┼─────┤
+            │ A   │ B   │ C   │ D   │
+            │ 1   │ 2   │ 3   │ 4   │
+            └─────┴─────┴─────┴─────┘
+            [2 rows x 4 columns]
+        ```
+
+        Multiple models can be stacked simultaneously, here we stack a total of 3 models:
+
+        ```python
+            # Create a third model C
+            sdm_c = SQLDataModel([('E', 'F'), ('5', '6')], headers=['C1', 'C2'])
+
+            # Horizontally stack three models
+            sdm_abc = sdm_a.hstack([sdm_b, sdm_c])
+
+            # View stacked result
+            print(sdm_abc)
+        ```
+
+        This will output the result of stacking C and B onto A:
+
+        ```shell
+            ┌─────┬─────┬─────┬─────┬─────┬─────┐
+            │ A1  │ A2  │ B1  │ B2  │ C1  │ C2  │
+            ├─────┼─────┼─────┼─────┼─────┼─────┤
+            │ A   │ B   │ C   │ D   │ E   │ F   │
+            │ 1   │ 2   │ 3   │ 4   │ 5   │ 6   │
+            └─────┴─────┴─────┴─────┴─────┴─────┘
+            [2 rows x 6 columns]
+        ```
+
+        Note:
+            - Model dimensions will be truncated or padded to coerce compatible dimensions when stacking, use :meth:`SQLDataModel.merge()` for strict SQL joins instead of hstack.
+            - Headers and data types are inherited from all the models being stacked, this requires aliasing duplicate column names if present, see :meth:`SQLDataModel.alias_duplicates()` for aliasing rules.
+            - Use ``setitem`` syntax such as ``sdm['New Column'] = values`` to create new columns directly into the currently model instead of stacking or see :meth:`SQLDataModel.add_column_with_values()` for convenience method accomplishing the same.
+            - See :meth:`SQLDataModel.vstack()` for vertical stacking.
+        """
+        other = list(other[0]) if len(other) == 1 and isinstance(other[0], (list,tuple)) else list(other)
+        if len(other) < 1:
+            raise ValueError(
+                SQLDataModel.ErrorFormat(f"ValueError: insufficient model count '{len(other)}', at least 1 additional 'SQLDataModel' is required to horizontally stack against")
+            )
+        if not all(isinstance(sdm, SQLDataModel) for sdm in other):
+            raise TypeError(
+                SQLDataModel.ErrorFormat(f"TypeError: invalid type encountered in '{[type(other[n]).__name__ for n in other]}', arguments for `other` must all be of type 'SQLDataModel' to horizontally stack")
+            )
+        other_headers, other_dtypes = zip(*[(col[0], col[1]) for sdm in other for col in sdm.get_column_dtypes().items()])
+        other_headers, other_dtypes = list(SQLDataModel.alias_duplicates([*self.headers,*other_headers])), [*self.get_column_dtypes().values(), *other_dtypes]
+        other_data = [(sdm[:self.row_count].data() if sdm.row_count > 1 else [sdm[:self.row_count].data()]) + [tuple(None for _ in range(sdm.column_count)) for _ in range(self.row_count - sdm.row_count)] for sdm in other]
+        other_data = [tuple(item for sublist in row for item in sublist) for row in list(zip(*other_data))]
+        if inplace:
+            other_headers = other_headers[self.column_count:] # since in place remove current model's headers
+            other_dtypes = other_dtypes[self.column_count:] # since in place remove current model's dtypes
+            update_sql_script = ";".join([f"""alter table "{self.sql_model}" add column "{col_name}" {self.static_py_to_sql_map_dict.get(col_type, 'TEXT')}""" for col_name, col_type in zip(other_headers, other_dtypes)])
+            col_val_param = ','.join([f""" "{col}" = {SQLDataModel.sqlite_cast_type_format(param='?', dtype=dtype)} """ for col,dtype in zip(other_headers, other_dtypes)])
+            update_stmt = f"""update "{self.sql_model}" set {col_val_param} where {self.sql_idx} = ?"""
+            update_params = [(*other_data[i], row) for i,row in enumerate(self.indicies)]
+            try:
+                self.execute_transaction(update_sql_script)
+                self.sql_db_conn.executemany(update_stmt, update_params)
+                self.sql_db_conn.commit()
+            except sqlite3.ProgrammingError as e:
+                self.sql_db_conn.rollback()
+                raise SQLProgrammingError(
+                    SQLDataModel.ErrorFormat(f"SQLProgrammingError: invalid update values, SQL execution failed with '{e}'")
+                ) from None
+            self._update_model_metadata()
+            return
+        else:
+            other_data = [(t1 + t2) for t1, t2 in zip(self.data(index=False, include_headers=False), other_data)]
+            dtype_dict = dict(zip(other_headers, other_dtypes))
+            return type(self)(data=other_data, headers=other_headers, dtypes=dtype_dict, **self._get_display_args())
 
     def iter_rows(self, min_row:int=None, max_row:int=None, index:bool=True, include_headers:bool=False) -> Generator:
         """
         Returns a generator object of the rows in the model from ``min_row`` to `max_row`.
 
         Parameters:
             ``min_row`` (int, optional): The minimum row index to start iterating from (inclusive). Defaults to None.
@@ -8645,14 +8762,119 @@
         ```    
         Note:
             - See related :meth:`SQLDataModel.head()` for the opposite, grabbing the top ``n_rows`` from the current model.
 
         """
         return self.execute_fetch(self._generate_unordered_sql_stmt(n_rows, ordering="desc"))
   
+    def vstack(self, *other:SQLDataModel, inplace:bool=False) -> SQLDataModel:
+        """
+        Vertically stacks one or more ``SQLDataModel`` objects to the current model.
+
+        Parameters:
+            ``other`` (SQLDataModel or sequence of): The SQLDataModel objects to vertically stack.
+            ``inplace`` (bool, optional): If True, performs the vertical stacking in-place, modifying the current model. Defaults to False, returning a new ``SQLDataModel``.
+
+        Returns:
+            ``SQLDataModel``: The vertically stacked SQLDataModel instance when inplace is False.
+
+        Raises:
+            ``ValueError``: If no additional SQLDataModels are provided for vertical stacking.
+            ``TypeError``: If any argument in 'other' is not of type SQLDataModel, list, or tuple.
+            ``SQLProgrammingError``: If an error occurs when updating the model values in place.
+
+        Example::
+
+            from SQLDataModel import SQLDataModel
+
+            # Create models A and B
+            sdm_a = SQLDataModel([('A', 1), ('B', 2)], headers=['A1', 'A2'])
+            sdm_b = SQLDataModel([('C', 3), ('D', 4)], headers=['B1', 'B2'])
+
+            # Vertically stack B onto A
+            sdm_ab = sdm_a.vstack(sdm_b)
+
+            # View stacked model
+            print(sdm_ab)
+
+        This will output the result of stacking B onto A, using the base model columns and dtypes:
+
+        ```shell
+            ┌─────┬─────┐
+            │ A1  │  A2 │
+            ├─────┼─────┤
+            │ A   │   1 │
+            │ B   │   2 │
+            │ C   │   3 │
+            │ D   │   4 │
+            └─────┴─────┘
+            [4 rows x 2 columns]
+        ```
+
+        Multiple models can be stacked simultaneously, here we vertically stack 3 models:
+
+        ```python
+            # Create a third model C
+            sdm_c = SQLDataModel([('E', 5), ('F', 6)], headers=['C1', 'C2'])
+
+            # Vertically stack all three models
+            sdm_abc = sdm_a.vstack([sdm_b, sdm_c])
+
+            # View stacked result
+            print(sdm_abc)
+        ```
+
+        This will output the result of stacking C and B onto A:
+
+        ```shell
+            ┌─────┬─────┐
+            │ A1  │  A2 │
+            ├─────┼─────┤
+            │ A   │   1 │
+            │ B   │   2 │
+            │ C   │   3 │
+            │ D   │   4 │
+            │ E   │   5 │
+            │ F   │   6 │
+            └─────┴─────┘
+            [6 rows x 2 columns]
+        ```
+
+        Note:
+            - Headers and data types are inherited from the model calling the :meth:`SQLDataModel.vstack()` method, casting stacked values corresponding to the base model types.
+            - Model dimensions will be truncated or padded to coerce compatible dimensions when stacking, use :meth:`SQLDataModel.concat()` for strict concatenation instead of vstack.
+            - See :meth:`SQLDataModel.insert_row()` for inserting new values or types other than ``SQLDataModel`` directly into the current model.
+            - See :meth:`SQLDataModel.hstack()` for horizontal stacking.
+        """
+        other = list(other[0]) if len(other) == 1 and isinstance(other[0], (list,tuple)) else list(other)
+        if len(other) < 1:
+            raise ValueError(
+                SQLDataModel.ErrorFormat(f"ValueError: insufficient model count '{len(other)}', at least 1 additional 'SQLDataModel' is required to vertically stack against")
+            )
+        if not all(isinstance(sdm, SQLDataModel) for sdm in other):
+            raise TypeError(
+                SQLDataModel.ErrorFormat(f"TypeError: invalid type encountered in '{[type(other[n]).__name__ for n in other]}', arguments for `other` must all be of type 'SQLDataModel' to vertically stack")
+            )
+        other_data = [[cell for cell in sublist] + [None] * (self.column_count - len(sublist)) for sublist in [item for sublist in [sdm[:,:self.column_count].data(index=False,include_headers=False) for sdm in other] for item in sublist]]
+        if inplace:
+            sql_insert_stmt = f"""insert into "{self.sql_model}" ({','.join([f'"{col}"' for col in self.headers])}) values ({",".join([SQLDataModel.sqlite_cast_type_format(dtype=self.header_master[col][1], as_binding=True) for col in self.headers])})"""
+            try:
+                self.sql_db_conn.executemany(sql_insert_stmt, other_data)
+                self.sql_db_conn.commit()
+            except sqlite3.ProgrammingError as e:
+                self.sql_db_conn.rollback()
+                raise SQLProgrammingError(
+                    SQLDataModel.ErrorFormat(f"SQLProgrammingError: invalid update values, SQL execution failed with '{e}'")
+                ) from None            
+            self._update_model_metadata(update_row_meta=True)
+            return
+        else:
+            other_data = (*self.data(index=False, include_headers=False),*other_data)
+            return type(self)(data=other_data, headers=self.headers, dtypes=self.get_column_dtypes(), **self._get_display_args())
+
     def where(self, predicate:str) -> SQLDataModel:
         """
         Filters the rows of the current ``SQLDataModel`` object based on the specified SQL predicate and returns a
         new ``SQLDataModel`` containing only the rows that satisfy the condition. Only the predicates are needed as the statement prepends the select clause as "select [current model columns] where [`predicate`]", see below for detailed examples.
 
         Parameters:
             ``predicate`` (str): The SQL predicate used for filtering rows that follows the 'where' keyword in a normal SQL statement.
@@ -10246,8 +10468,8 @@
         if dtype not in ('bool','bytes','date','datetime','float','int','None','str'):
             raise ValueError(
                 SQLDataModel.ErrorFormat(f"ValueError: invalid value '{type(dtype).__name__}', argument for `dtype` must be one of 'bool','bytes','date','datetime','float','int','None' or 'str'")
             )        
         str_col_cast = ",".join([SQLDataModel.sqlite_cast_type_format(param=col, dtype=dtype, as_binding=False, as_alias=True) for col in self.headers])        
         sql_stmt = " ".join(("select",str_col_cast,f'from "{self.sql_model}"'))
         dtype_dict = {col:dtype for col in self.headers}
-        return self.execute_fetch(sql_stmt, dtypes=dtype_dict)
+        return self.execute_fetch(sql_stmt, dtypes=dtype_dict)
```

### Comparing `SQLDataModel-0.3.3/src/SQLDataModel/StandardDeviation.py` & `SQLDataModel-0.3.4/src/SQLDataModel/StandardDeviation.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.3/src/SQLDataModel/converters.py` & `SQLDataModel-0.3.4/src/SQLDataModel/converters.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.3/src/SQLDataModel/demo.py` & `SQLDataModel-0.3.4/src/SQLDataModel/demo.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.3/src/SQLDataModel/exceptions.py` & `SQLDataModel-0.3.4/src/SQLDataModel/exceptions.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.3/src/SQLDataModel/extensions/str_utils.c` & `SQLDataModel-0.3.4/src/SQLDataModel/extensions/str_utils.c`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.3/src/SQLDataModel.egg-info/PKG-INFO` & `SQLDataModel-0.3.4/src/SQLDataModel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.3.3
+Version: 0.3.4
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package
```

### Comparing `SQLDataModel-0.3.3/src/SQLDataModel.egg-info/SOURCES.txt` & `SQLDataModel-0.3.4/src/SQLDataModel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.3/tests/test_Future.py` & `SQLDataModel-0.3.4/tests/test_Future.py`

 * *Files 17% similar despite different names*

```diff
@@ -669,8 +669,100 @@
     expected_max = ('xnq6', 811, 995.075213, '1', datetime.date(2022, 12, 24), b'sNLjVGWGaub5', None, datetime.datetime(2018, 2, 15, 17, 6, 3))    
     sdm = SQLDataModel(data, headers)
     output_count = sdm.count().data()
     output_min = sdm.min().data()
     output_max = sdm.max().data()
     assert output_count == expected_count
     assert output_min == expected_min
-    assert output_max == expected_max
+    assert output_max == expected_max
+
+@pytest.mark.core
+def test_hstack():
+    data_0, headers_0 = [('U_qF', -36, 62.04), ('4Z7w', 36, 80.43), ('ErUL', 80, -37.97)], ['string', 'int', 'float']
+    data_1, headers_1 = [('IXdh', 84, 89.05), ('CxnD', -42, 80.29), ('AVaB', 51, -93.88)], ['string_2', 'int_2', 'float_2']
+    data_2, headers_2 = [('fwkX', -5, 0.41), ('pncP', 39, 80.24), ('NX1F', 13, 74.21)], ['string_3', 'int_3', 'float_3']
+    data_3, headers_3 = [('Ki4C', 63, 26.97), ('L4CH', -62, 73.61), ('9CZD', -41, 4.64)], ['string_4', 'int_4', 'float_4']
+    sdm_0 = SQLDataModel(data=data_0, headers=headers_0, display_float_precision=2)
+    sdm_1 = SQLDataModel(data=data_1, headers=headers_1, display_float_precision=2)
+    sdm_2 = SQLDataModel(data=data_2, headers=headers_2, display_float_precision=2)
+    sdm_3 = SQLDataModel(data=data_3, headers=headers_3, display_float_precision=2)
+    ### single stack test returned as new model ###
+    single_stack_test = sdm_0.hstack(sdm_1, inplace=False)
+    output_data, output_headers = single_stack_test.data(), single_stack_test.get_headers()
+    expected_data, expected_headers = [(t1 + t2) for t1, t2 in zip(data_0, data_1)], [*headers_0, *headers_1]
+    assert output_headers == expected_headers
+    assert output_data == expected_data
+    ### multiple stack test returned as new model ###
+    multi_stack_test = sdm_0.hstack([sdm_1, sdm_2, sdm_3], inplace=False)
+    output_data, output_headers = multi_stack_test.data(), multi_stack_test.get_headers()
+    expected_data, expected_headers = [(t1 + t2 + t3 + t4) for t1, t2, t3, t4 in zip(data_0, data_1, data_2, data_3)], [*headers_0, *headers_1, *headers_2, *headers_3]
+    assert output_headers == expected_headers
+    assert output_data == expected_data    
+    ### single stack inplace ###
+    single_stack_test = SQLDataModel(sdm_0.data(), dtypes=sdm_0.get_column_dtypes()) # copy into new sdm to avoid tarnishing remaining tests
+    single_stack_test.hstack(sdm_1, inplace=True)
+    output_data, output_headers = single_stack_test.data(), single_stack_test.get_headers()
+    expected_data, expected_headers = [(t1 + t2) for t1, t2 in zip(data_0, data_1)], [*headers_0, *headers_1]
+    assert output_headers == expected_headers
+    assert output_data == expected_data
+    ### multi stack inplace ###
+    mult_stack_test = SQLDataModel(sdm_0.data(), dtypes=sdm_0.get_column_dtypes()) # copy into new sdm to avoid tarnishing remaining tests
+    mult_stack_test.hstack([sdm_1, sdm_2, sdm_3], inplace=True)
+    output_data, output_headers = multi_stack_test.data(), multi_stack_test.get_headers()
+    expected_data, expected_headers = [(t1 + t2 + t3 + t4) for t1, t2, t3, t4 in zip(data_0, data_1, data_2, data_3)], [*headers_0, *headers_1, *headers_2, *headers_3]
+    assert output_headers == expected_headers
+    assert output_data == expected_data   
+    ### test dimension coercion ###
+    sdm_0[sdm_0.row_count] = ['new', 99, 3.1415]
+    single_stack_test = sdm_0.hstack(sdm_1, inplace=False)
+    output_data, output_headers = single_stack_test.data(), single_stack_test.get_headers()
+    data_0 += [('new', 99, 3.1415)] # simulate required padding for dim coercion
+    data_1 += [(None, None, None)]
+    expected_data, expected_headers = [(t1 + t2) for t1, t2 in zip(data_0, data_1)], [*headers_0, *headers_1]
+    assert output_headers == expected_headers
+    assert output_data == expected_data
+    
+@pytest.mark.core
+def test_vstack():
+    data_0, headers_0 = [('U_qF', -36, 62.04), ('4Z7w', 36, 80.43), ('ErUL', 80, -37.97)], ['string', 'int', 'float']
+    data_1, headers_1 = [('IXdh', 84, 89.05), ('CxnD', -42, 80.29), ('AVaB', 51, -93.88)], ['string_2', 'int_2', 'float_2']
+    data_2, headers_2 = [('fwkX', -5, 0.41), ('pncP', 39, 80.24), ('NX1F', 13, 74.21)], ['string_3', 'int_3', 'float_3']
+    data_3, headers_3 = [('Ki4C', 63, 26.97), ('L4CH', -62, 73.61), ('9CZD', -41, 4.64)], ['string_4', 'int_4', 'float_4']
+    sdm_0 = SQLDataModel(data=data_0, headers=headers_0, display_float_precision=2)
+    sdm_1 = SQLDataModel(data=data_1, headers=headers_1, display_float_precision=2)
+    sdm_2 = SQLDataModel(data=data_2, headers=headers_2, display_float_precision=2)
+    sdm_3 = SQLDataModel(data=data_3, headers=headers_3, display_float_precision=2)
+    ### single stack test returned as new model ###
+    single_stack_test = sdm_0.vstack(sdm_1, inplace=False)
+    output_data, output_headers = single_stack_test.data(), single_stack_test.get_headers()
+    expected_data, expected_headers = data_0 + data_1, headers_0
+    assert output_headers == expected_headers
+    assert output_data == expected_data
+    ### multiple stack test returned as new model ###
+    multi_stack_test = sdm_0.vstack([sdm_1, sdm_2, sdm_3], inplace=False)
+    output_data, output_headers = multi_stack_test.data(), multi_stack_test.get_headers()
+    expected_data, expected_headers = data_0 + data_1 + data_2 + data_3, headers_0
+    assert output_headers == expected_headers
+    assert output_data == expected_data  
+    ### single stack inplace ###
+    single_stack_test = SQLDataModel(sdm_0.data(), dtypes=sdm_0.get_column_dtypes()) # copy into new sdm to avoid tarnishing remaining tests
+    single_stack_test.vstack(sdm_1, inplace=True)
+    output_data, output_headers = single_stack_test.data(), single_stack_test.get_headers()
+    expected_data, expected_headers = data_0 + data_1, headers_0
+    assert output_headers == expected_headers
+    assert output_data == expected_data
+    ### multi stack inplace ###
+    mult_stack_test = SQLDataModel(sdm_0.data(), dtypes=sdm_0.get_column_dtypes()) # copy into new sdm to avoid tarnishing remaining tests
+    mult_stack_test.vstack([sdm_1, sdm_2, sdm_3], inplace=True)
+    output_data, output_headers = multi_stack_test.data(), multi_stack_test.get_headers()
+    expected_data, expected_headers = data_0 + data_1 + data_2 + data_3, headers_0
+    assert output_headers == expected_headers
+    assert output_data == expected_data   
+    ### test dimension coercion ###
+    sdm_0['bytes'] = b'pad test'
+    single_stack_test = sdm_0.vstack(sdm_1, inplace=False)
+    output_data, output_headers = single_stack_test.data(), single_stack_test.get_headers()
+    data_0 = [tuple([*row, b'pad test']) for row in data_0]
+    data_1 = [tuple([*row, None]) for row in data_1]
+    expected_data, expected_headers = data_0 + data_1, [*headers_0, 'bytes']
+    assert output_headers == expected_headers
+    assert output_data == expected_data
```

### Comparing `SQLDataModel-0.3.3/tests/test_SQLDataModel.py` & `SQLDataModel-0.3.4/tests/test_SQLDataModel.py`

 * *Files 18% similar despite different names*

```diff
@@ -669,8 +669,100 @@
     expected_max = ('xnq6', 811, 995.075213, '1', datetime.date(2022, 12, 24), b'sNLjVGWGaub5', None, datetime.datetime(2018, 2, 15, 17, 6, 3))    
     sdm = SQLDataModel(data, headers)
     output_count = sdm.count().data()
     output_min = sdm.min().data()
     output_max = sdm.max().data()
     assert output_count == expected_count
     assert output_min == expected_min
-    assert output_max == expected_max
+    assert output_max == expected_max
+
+@pytest.mark.core
+def test_hstack():
+    data_0, headers_0 = [('U_qF', -36, 62.04), ('4Z7w', 36, 80.43), ('ErUL', 80, -37.97)], ['string', 'int', 'float']
+    data_1, headers_1 = [('IXdh', 84, 89.05), ('CxnD', -42, 80.29), ('AVaB', 51, -93.88)], ['string_2', 'int_2', 'float_2']
+    data_2, headers_2 = [('fwkX', -5, 0.41), ('pncP', 39, 80.24), ('NX1F', 13, 74.21)], ['string_3', 'int_3', 'float_3']
+    data_3, headers_3 = [('Ki4C', 63, 26.97), ('L4CH', -62, 73.61), ('9CZD', -41, 4.64)], ['string_4', 'int_4', 'float_4']
+    sdm_0 = SQLDataModel(data=data_0, headers=headers_0, display_float_precision=2)
+    sdm_1 = SQLDataModel(data=data_1, headers=headers_1, display_float_precision=2)
+    sdm_2 = SQLDataModel(data=data_2, headers=headers_2, display_float_precision=2)
+    sdm_3 = SQLDataModel(data=data_3, headers=headers_3, display_float_precision=2)
+    ### single stack test returned as new model ###
+    single_stack_test = sdm_0.hstack(sdm_1, inplace=False)
+    output_data, output_headers = single_stack_test.data(), single_stack_test.get_headers()
+    expected_data, expected_headers = [(t1 + t2) for t1, t2 in zip(data_0, data_1)], [*headers_0, *headers_1]
+    assert output_headers == expected_headers
+    assert output_data == expected_data
+    ### multiple stack test returned as new model ###
+    multi_stack_test = sdm_0.hstack([sdm_1, sdm_2, sdm_3], inplace=False)
+    output_data, output_headers = multi_stack_test.data(), multi_stack_test.get_headers()
+    expected_data, expected_headers = [(t1 + t2 + t3 + t4) for t1, t2, t3, t4 in zip(data_0, data_1, data_2, data_3)], [*headers_0, *headers_1, *headers_2, *headers_3]
+    assert output_headers == expected_headers
+    assert output_data == expected_data    
+    ### single stack inplace ###
+    single_stack_test = SQLDataModel(sdm_0.data(), dtypes=sdm_0.get_column_dtypes()) # copy into new sdm to avoid tarnishing remaining tests
+    single_stack_test.hstack(sdm_1, inplace=True)
+    output_data, output_headers = single_stack_test.data(), single_stack_test.get_headers()
+    expected_data, expected_headers = [(t1 + t2) for t1, t2 in zip(data_0, data_1)], [*headers_0, *headers_1]
+    assert output_headers == expected_headers
+    assert output_data == expected_data
+    ### multi stack inplace ###
+    mult_stack_test = SQLDataModel(sdm_0.data(), dtypes=sdm_0.get_column_dtypes()) # copy into new sdm to avoid tarnishing remaining tests
+    mult_stack_test.hstack([sdm_1, sdm_2, sdm_3], inplace=True)
+    output_data, output_headers = multi_stack_test.data(), multi_stack_test.get_headers()
+    expected_data, expected_headers = [(t1 + t2 + t3 + t4) for t1, t2, t3, t4 in zip(data_0, data_1, data_2, data_3)], [*headers_0, *headers_1, *headers_2, *headers_3]
+    assert output_headers == expected_headers
+    assert output_data == expected_data   
+    ### test dimension coercion ###
+    sdm_0[sdm_0.row_count] = ['new', 99, 3.1415]
+    single_stack_test = sdm_0.hstack(sdm_1, inplace=False)
+    output_data, output_headers = single_stack_test.data(), single_stack_test.get_headers()
+    data_0 += [('new', 99, 3.1415)] # simulate required padding for dim coercion
+    data_1 += [(None, None, None)]
+    expected_data, expected_headers = [(t1 + t2) for t1, t2 in zip(data_0, data_1)], [*headers_0, *headers_1]
+    assert output_headers == expected_headers
+    assert output_data == expected_data
+    
+@pytest.mark.core
+def test_vstack():
+    data_0, headers_0 = [('U_qF', -36, 62.04), ('4Z7w', 36, 80.43), ('ErUL', 80, -37.97)], ['string', 'int', 'float']
+    data_1, headers_1 = [('IXdh', 84, 89.05), ('CxnD', -42, 80.29), ('AVaB', 51, -93.88)], ['string_2', 'int_2', 'float_2']
+    data_2, headers_2 = [('fwkX', -5, 0.41), ('pncP', 39, 80.24), ('NX1F', 13, 74.21)], ['string_3', 'int_3', 'float_3']
+    data_3, headers_3 = [('Ki4C', 63, 26.97), ('L4CH', -62, 73.61), ('9CZD', -41, 4.64)], ['string_4', 'int_4', 'float_4']
+    sdm_0 = SQLDataModel(data=data_0, headers=headers_0, display_float_precision=2)
+    sdm_1 = SQLDataModel(data=data_1, headers=headers_1, display_float_precision=2)
+    sdm_2 = SQLDataModel(data=data_2, headers=headers_2, display_float_precision=2)
+    sdm_3 = SQLDataModel(data=data_3, headers=headers_3, display_float_precision=2)
+    ### single stack test returned as new model ###
+    single_stack_test = sdm_0.vstack(sdm_1, inplace=False)
+    output_data, output_headers = single_stack_test.data(), single_stack_test.get_headers()
+    expected_data, expected_headers = data_0 + data_1, headers_0
+    assert output_headers == expected_headers
+    assert output_data == expected_data
+    ### multiple stack test returned as new model ###
+    multi_stack_test = sdm_0.vstack([sdm_1, sdm_2, sdm_3], inplace=False)
+    output_data, output_headers = multi_stack_test.data(), multi_stack_test.get_headers()
+    expected_data, expected_headers = data_0 + data_1 + data_2 + data_3, headers_0
+    assert output_headers == expected_headers
+    assert output_data == expected_data  
+    ### single stack inplace ###
+    single_stack_test = SQLDataModel(sdm_0.data(), dtypes=sdm_0.get_column_dtypes()) # copy into new sdm to avoid tarnishing remaining tests
+    single_stack_test.vstack(sdm_1, inplace=True)
+    output_data, output_headers = single_stack_test.data(), single_stack_test.get_headers()
+    expected_data, expected_headers = data_0 + data_1, headers_0
+    assert output_headers == expected_headers
+    assert output_data == expected_data
+    ### multi stack inplace ###
+    mult_stack_test = SQLDataModel(sdm_0.data(), dtypes=sdm_0.get_column_dtypes()) # copy into new sdm to avoid tarnishing remaining tests
+    mult_stack_test.vstack([sdm_1, sdm_2, sdm_3], inplace=True)
+    output_data, output_headers = multi_stack_test.data(), multi_stack_test.get_headers()
+    expected_data, expected_headers = data_0 + data_1 + data_2 + data_3, headers_0
+    assert output_headers == expected_headers
+    assert output_data == expected_data   
+    ### test dimension coercion ###
+    sdm_0['bytes'] = b'pad test'
+    single_stack_test = sdm_0.vstack(sdm_1, inplace=False)
+    output_data, output_headers = single_stack_test.data(), single_stack_test.get_headers()
+    data_0 = [tuple([*row, b'pad test']) for row in data_0]
+    data_1 = [tuple([*row, None]) for row in data_1]
+    expected_data, expected_headers = data_0 + data_1, [*headers_0, 'bytes']
+    assert output_headers == expected_headers
+    assert output_data == expected_data
```

