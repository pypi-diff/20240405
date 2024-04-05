# Comparing `tmp/sprocketship-0.0.8.tar.gz` & `tmp/sprocketship-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprocketship-0.0.8.tar", last modified: Fri Apr  5 17:38:30 2024, max compression
+gzip compressed data, was "sprocketship-0.0.9.tar", last modified: Fri Apr  5 17:44:43 2024, max compression
```

## Comparing `sprocketship-0.0.8.tar` & `sprocketship-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:38:30.583635 sprocketship-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 17:38:26.000000 sprocketship-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-04-05 17:38:30.583635 sprocketship-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-05 17:38:26.000000 sprocketship-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-05 17:38:26.000000 sprocketship-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 17:38:30.583635 sprocketship-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:38:30.583635 sprocketship-0.0.8/sprocketship/
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-04-05 17:38:26.000000 sprocketship-0.0.8/sprocketship/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:38:30.583635 sprocketship-0.0.8/sprocketship.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-04-05 17:38:30.000000 sprocketship-0.0.8/sprocketship.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-05 17:38:30.000000 sprocketship-0.0.8/sprocketship.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:38:30.000000 sprocketship-0.0.8/sprocketship.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 17:38:30.000000 sprocketship-0.0.8/sprocketship.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 17:38:30.000000 sprocketship-0.0.8/sprocketship.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 17:38:30.000000 sprocketship-0.0.8/sprocketship.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:44:43.652487 sprocketship-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 17:44:36.000000 sprocketship-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-04-05 17:44:43.652487 sprocketship-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-04-05 17:44:36.000000 sprocketship-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-05 17:44:36.000000 sprocketship-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 17:44:43.652487 sprocketship-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:44:43.648487 sprocketship-0.0.9/sprocketship/
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-04-05 17:44:36.000000 sprocketship-0.0.9/sprocketship/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:44:43.652487 sprocketship-0.0.9/sprocketship.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-04-05 17:44:43.000000 sprocketship-0.0.9/sprocketship.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-05 17:44:43.000000 sprocketship-0.0.9/sprocketship.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:44:43.000000 sprocketship-0.0.9/sprocketship.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 17:44:43.000000 sprocketship-0.0.9/sprocketship.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 17:44:43.000000 sprocketship-0.0.9/sprocketship.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 17:44:43.000000 sprocketship-0.0.9/sprocketship.egg-info/top_level.txt
```

### Comparing `sprocketship-0.0.8/LICENSE` & `sprocketship-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sprocketship-0.0.8/PKG-INFO` & `sprocketship-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.0.8
+Version: 0.0.9
 Summary: Better stored procedure management
 Author-email: Nicklaus Roacb <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -148,15 +148,19 @@
     - name: create_database_writer
       replace_if_exists: true
       database: {{ env.get('SNOWFLAKE_DATABASE') }}
       schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
       ...
 ```
 
-From here, simply run `sprocketship liftoff` from the project directory (or provide the directory, e.g. `sprocketship liftoff my/directory/path`) and sprocketship will launch your stored procedures into the given directory. 
+From here, simply run 
+
+`$ sprocketship liftoff` 
+
+from the project directory (or provide the directory, e.g. `sprocketship liftoff my/directory/path`) and sprocketship will launch your stored procedures into the given directory. 
 
 <!-- LICENSE -->
 ## License
 
 Distributed under the MIT License. See `LICENSE` for more information.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.0.8 Summary: Better stored
+Metadata-Version: 2.1 Name: sprocketship Version: 0.0.9 Summary: Better stored
 procedure management Author-email: Nicklaus Roacb
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel.yaml
@@ -38,15 +38,15 @@
 paths to their corresponding files in the `procedures/` directory. ```
 procedures: development: - name: create_temp_database replace_if_exists: true
 database: {{ env.get('SNOWFLAKE_DATABASE') }} schema: {{ env.get
 ('SNOWFLAKE_SCHEMA') }} ... admin: - name: create_database_reader
 replace_if_exists: true database: {{ env.get('SNOWFLAKE_DATABASE') }} schema: {
 { env.get('SNOWFLAKE_SCHEMA') }} ... - name: create_database_writer
 replace_if_exists: true database: {{ env.get('SNOWFLAKE_DATABASE') }} schema: {
-{ env.get('SNOWFLAKE_SCHEMA') }} ... ``` From here, simply run `sprocketship
+{ env.get('SNOWFLAKE_SCHEMA') }} ... ``` From here, simply run `$ sprocketship
 liftoff` from the project directory (or provide the directory, e.g.
 `sprocketship liftoff my/directory/path`) and sprocketship will launch your
 stored procedures into the given directory. ## License Distributed under the
 MIT License. See `LICENSE` for more information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/
 nicklausroach/sprocketship.svg?style=for-the-badge [contributors-url]: https://
```

### Comparing `sprocketship-0.0.8/README.md` & `sprocketship-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,19 @@
     - name: create_database_writer
       replace_if_exists: true
       database: {{ env.get('SNOWFLAKE_DATABASE') }}
       schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
       ...
 ```
 
-From here, simply run `sprocketship liftoff` from the project directory (or provide the directory, e.g. `sprocketship liftoff my/directory/path`) and sprocketship will launch your stored procedures into the given directory. 
+From here, simply run 
+
+`$ sprocketship liftoff` 
+
+from the project directory (or provide the directory, e.g. `sprocketship liftoff my/directory/path`) and sprocketship will launch your stored procedures into the given directory. 
 
 <!-- LICENSE -->
 ## License
 
 Distributed under the MIT License. See `LICENSE` for more information.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -29,15 +29,15 @@
 paths to their corresponding files in the `procedures/` directory. ```
 procedures: development: - name: create_temp_database replace_if_exists: true
 database: {{ env.get('SNOWFLAKE_DATABASE') }} schema: {{ env.get
 ('SNOWFLAKE_SCHEMA') }} ... admin: - name: create_database_reader
 replace_if_exists: true database: {{ env.get('SNOWFLAKE_DATABASE') }} schema: {
 { env.get('SNOWFLAKE_SCHEMA') }} ... - name: create_database_writer
 replace_if_exists: true database: {{ env.get('SNOWFLAKE_DATABASE') }} schema: {
-{ env.get('SNOWFLAKE_SCHEMA') }} ... ``` From here, simply run `sprocketship
+{ env.get('SNOWFLAKE_SCHEMA') }} ... ``` From here, simply run `$ sprocketship
 liftoff` from the project directory (or provide the directory, e.g.
 `sprocketship liftoff my/directory/path`) and sprocketship will launch your
 stored procedures into the given directory. ## License Distributed under the
 MIT License. See `LICENSE` for more information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/
 nicklausroach/sprocketship.svg?style=for-the-badge [contributors-url]: https://
```

### Comparing `sprocketship-0.0.8/pyproject.toml` & `sprocketship-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sprocketship"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Nicklaus Roacb", email="nicklausroach@gmail.com" },
 ]
 readme = "README.md"
 description = "Better stored procedure management"
 dependencies = [
     "click",
```

### Comparing `sprocketship-0.0.8/sprocketship/cli.py` & `sprocketship-0.0.9/sprocketship/cli.py`

 * *Files identical despite different names*

### Comparing `sprocketship-0.0.8/sprocketship.egg-info/PKG-INFO` & `sprocketship-0.0.9/sprocketship.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.0.8
+Version: 0.0.9
 Summary: Better stored procedure management
 Author-email: Nicklaus Roacb <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -148,15 +148,19 @@
     - name: create_database_writer
       replace_if_exists: true
       database: {{ env.get('SNOWFLAKE_DATABASE') }}
       schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
       ...
 ```
 
-From here, simply run `sprocketship liftoff` from the project directory (or provide the directory, e.g. `sprocketship liftoff my/directory/path`) and sprocketship will launch your stored procedures into the given directory. 
+From here, simply run 
+
+`$ sprocketship liftoff` 
+
+from the project directory (or provide the directory, e.g. `sprocketship liftoff my/directory/path`) and sprocketship will launch your stored procedures into the given directory. 
 
 <!-- LICENSE -->
 ## License
 
 Distributed under the MIT License. See `LICENSE` for more information.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.0.8 Summary: Better stored
+Metadata-Version: 2.1 Name: sprocketship Version: 0.0.9 Summary: Better stored
 procedure management Author-email: Nicklaus Roacb
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel.yaml
@@ -38,15 +38,15 @@
 paths to their corresponding files in the `procedures/` directory. ```
 procedures: development: - name: create_temp_database replace_if_exists: true
 database: {{ env.get('SNOWFLAKE_DATABASE') }} schema: {{ env.get
 ('SNOWFLAKE_SCHEMA') }} ... admin: - name: create_database_reader
 replace_if_exists: true database: {{ env.get('SNOWFLAKE_DATABASE') }} schema: {
 { env.get('SNOWFLAKE_SCHEMA') }} ... - name: create_database_writer
 replace_if_exists: true database: {{ env.get('SNOWFLAKE_DATABASE') }} schema: {
-{ env.get('SNOWFLAKE_SCHEMA') }} ... ``` From here, simply run `sprocketship
+{ env.get('SNOWFLAKE_SCHEMA') }} ... ``` From here, simply run `$ sprocketship
 liftoff` from the project directory (or provide the directory, e.g.
 `sprocketship liftoff my/directory/path`) and sprocketship will launch your
 stored procedures into the given directory. ## License Distributed under the
 MIT License. See `LICENSE` for more information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/
 nicklausroach/sprocketship.svg?style=for-the-badge [contributors-url]: https://
```

