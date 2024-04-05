# Comparing `tmp/sprocketship-0.0.3.tar.gz` & `tmp/sprocketship-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprocketship-0.0.3.tar", last modified: Fri Apr  5 16:04:22 2024, max compression
+gzip compressed data, was "sprocketship-0.0.4.tar", last modified: Fri Apr  5 16:18:46 2024, max compression
```

## Comparing `sprocketship-0.0.3.tar` & `sprocketship-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:04:22.122514 sprocketship-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 16:04:17.000000 sprocketship-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-05 16:04:22.118514 sprocketship-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-05 16:04:17.000000 sprocketship-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-05 16:04:17.000000 sprocketship-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:04:22.122514 sprocketship-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:04:22.118514 sprocketship-0.0.3/sprocketship/
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-05 16:04:17.000000 sprocketship-0.0.3/sprocketship/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:04:22.118514 sprocketship-0.0.3/sprocketship.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-05 16:04:22.000000 sprocketship-0.0.3/sprocketship.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-05 16:04:22.000000 sprocketship-0.0.3/sprocketship.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:04:22.000000 sprocketship-0.0.3/sprocketship.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 16:04:22.000000 sprocketship-0.0.3/sprocketship.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 16:04:22.000000 sprocketship-0.0.3/sprocketship.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 16:04:22.000000 sprocketship-0.0.3/sprocketship.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:46.389598 sprocketship-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 16:18:42.000000 sprocketship-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-04-05 16:18:46.389598 sprocketship-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-04-05 16:18:42.000000 sprocketship-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-05 16:18:42.000000 sprocketship-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:18:46.389598 sprocketship-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:46.385598 sprocketship-0.0.4/sprocketship/
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-05 16:18:42.000000 sprocketship-0.0.4/sprocketship/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:46.389598 sprocketship-0.0.4/sprocketship.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-04-05 16:18:46.000000 sprocketship-0.0.4/sprocketship.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-05 16:18:46.000000 sprocketship-0.0.4/sprocketship.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:18:46.000000 sprocketship-0.0.4/sprocketship.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 16:18:46.000000 sprocketship-0.0.4/sprocketship.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 16:18:46.000000 sprocketship-0.0.4/sprocketship.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 16:18:46.000000 sprocketship-0.0.4/sprocketship.egg-info/top_level.txt
```

### Comparing `sprocketship-0.0.3/LICENSE` & `sprocketship-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sprocketship-0.0.3/PKG-INFO` & `sprocketship-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.0.3
+Version: 0.0.4
 Author-email: Nicklaus Roacb <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -88,15 +88,15 @@
 </details>
 
 
 
 <!-- ABOUT THE PROJECT -->
 ## About The Project
 
-`sprocketship` makes it easy to develop, manage, and deploy stored procedures in snowflake. Using the language of your choosing, you can write the contents of your stored procedure separately from its configurations (e.g., `EXECUTE AS`, `RETURN TYPE`, etc.). 
+`sprocketship` makes it easy to develop, manage, and deploy stored procedures in Snowflake. Using the language of your choosing, you can write the contents of your stored procedure separately from its configurations (e.g., `EXECUTE AS`, `RETURN TYPE`, etc.). 
 
 
 
 
 ### Built With
 
 <a href=https://github.com/pipeline-tools/ABSQL>
@@ -113,20 +113,53 @@
 `pip install sprocketship`
 
 
 
 <!-- USAGE EXAMPLES -->
 ## Usage
 
-Use this space to show useful examples of how a project can be used. Additional screenshots, code examples and demos work well in this space. You may also link to more resources.
-
-_For more examples, please refer to the [Documentation](https://example.com)_
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
+Currently, sprocketship expects a `.sprocketship.yml` file and a `procedures/` directory at the same level in a directory structure.
 
+```
+├── dbt_models
+│   ├── customers.sql
+│   ├── products.sql
+├── procedures
+│   ├── admin
+│   │   ├── create_database_writer_role.js
+│   │   ├── create_database_reader_role.js
+│   ├── development
+│   │   ├── create_temp_database.js
+└── .sprocketship.yml
+```
+
+The yaml path to each procedure in the `sprocketship.yml` should follow that of the paths to their corresponding files in the `procedures/` directory. 
+
+```
+procedures:
+  development:
+    - name: create_temp_database
+      replace_if_exists: true
+      database: {{ env.get('SNOWFLAKE_DATABASE') }}
+      schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
+      ...
+
+  admin:
+    - name: create_database_reader
+      replace_if_exists: true
+      database: {{ env.get('SNOWFLAKE_DATABASE') }}
+      schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
+      ...
+
+    - name: create_database_writer
+      replace_if_exists: true
+      database: {{ env.get('SNOWFLAKE_DATABASE') }}
+      schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
+      ...
+```
 
 <!-- LICENSE -->
 ## License
 
 Distributed under the MIT License. See `LICENSE` for more information.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.0.3 Author-email: Nicklaus
+Metadata-Version: 2.1 Name: sprocketship Version: 0.0.4 Author-email: Nicklaus
 Roacb
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel.yaml
@@ -23,28 +23,36 @@
    3. _U_s_a_g_e
    4. _R_o_a_d_m_a_p
    5. _C_o_n_t_r_i_b_u_t_i_n_g
    6. _L_i_c_e_n_s_e
    7. _C_o_n_t_a_c_t
    8. _A_c_k_n_o_w_l_e_d_g_m_e_n_t_s
 ## About The Project `sprocketship` makes it easy to develop, manage, and
-deploy stored procedures in snowflake. Using the language of your choosing, you
+deploy stored procedures in Snowflake. Using the language of your choosing, you
 can write the contents of your stored procedure separately from its
 configurations (e.g., `EXECUTE AS`, `RETURN TYPE`, etc.). ### Built With_[_h_t_t_p_s_:
 _/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_p_i_p_e_l_i_n_e_-_t_o_o_l_s_/_A_B_S_Q_L_/
 _5_9_8_f_c_a_b_4_a_5_c_c_b_1_c_a_6_7_4_c_4_0_e_7_4_0_b_4_e_d_d_9_f_9_9_2_5_1_a_6_/_i_m_a_g_e_s_/_l_o_g_o___4_0_0_._s_v_g_]
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-### Installation `pip install sprocketship` ## Usage Use this space to show
-useful examples of how a project can be used. Additional screenshots, code
-examples and demos work well in this space. You may also link to more
-resources. _For more examples, please refer to the [Documentation](https://
-example.com)_
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## License Distributed under the MIT License. See `LICENSE` for more
-information.
+### Installation `pip install sprocketship` ## Usage Currently, sprocketship
+expects a `.sprocketship.yml` file and a `procedures/` directory at the same
+level in a directory structure. ``` âââ dbt_models â âââ
+customers.sql â âââ products.sql âââ procedures â âââ
+admin â â âââ create_database_writer_role.js â â âââ
+create_database_reader_role.js â âââ development â â âââ
+create_temp_database.js âââ .sprocketship.yml ``` The yaml path to each
+procedure in the `sprocketship.yml` should follow that of the paths to their
+corresponding files in the `procedures/` directory. ``` procedures:
+development: - name: create_temp_database replace_if_exists: true database: {
+{ env.get('SNOWFLAKE_DATABASE') }} schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
+... admin: - name: create_database_reader replace_if_exists: true database: {
+{ env.get('SNOWFLAKE_DATABASE') }} schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
+... - name: create_database_writer replace_if_exists: true database: {{ env.get
+('SNOWFLAKE_DATABASE') }} schema: {{ env.get('SNOWFLAKE_SCHEMA') }} ... ``` ##
+License Distributed under the MIT License. See `LICENSE` for more information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/
 nicklausroach/sprocketship.svg?style=for-the-badge [contributors-url]: https://
 github.com/nicklausroach/sprocketship/graphs/contributors [forks-shield]:
 https://img.shields.io/github/forks/nicklausroach/sprocketship.svg?style=for-
 the-badge [forks-url]: https://github.com/nicklausroach/sprocketship/network/
 members [stars-shield]: https://img.shields.io/github/stars/nicklausroach/
```

### Comparing `sprocketship-0.0.3/README.md` & `sprocketship-0.0.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 </details>
 
 
 
 <!-- ABOUT THE PROJECT -->
 ## About The Project
 
-`sprocketship` makes it easy to develop, manage, and deploy stored procedures in snowflake. Using the language of your choosing, you can write the contents of your stored procedure separately from its configurations (e.g., `EXECUTE AS`, `RETURN TYPE`, etc.). 
+`sprocketship` makes it easy to develop, manage, and deploy stored procedures in Snowflake. Using the language of your choosing, you can write the contents of your stored procedure separately from its configurations (e.g., `EXECUTE AS`, `RETURN TYPE`, etc.). 
 
 
 
 
 ### Built With
 
 <a href=https://github.com/pipeline-tools/ABSQL>
@@ -96,20 +96,53 @@
 `pip install sprocketship`
 
 
 
 <!-- USAGE EXAMPLES -->
 ## Usage
 
-Use this space to show useful examples of how a project can be used. Additional screenshots, code examples and demos work well in this space. You may also link to more resources.
-
-_For more examples, please refer to the [Documentation](https://example.com)_
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
+Currently, sprocketship expects a `.sprocketship.yml` file and a `procedures/` directory at the same level in a directory structure.
 
+```
+├── dbt_models
+│   ├── customers.sql
+│   ├── products.sql
+├── procedures
+│   ├── admin
+│   │   ├── create_database_writer_role.js
+│   │   ├── create_database_reader_role.js
+│   ├── development
+│   │   ├── create_temp_database.js
+└── .sprocketship.yml
+```
+
+The yaml path to each procedure in the `sprocketship.yml` should follow that of the paths to their corresponding files in the `procedures/` directory. 
+
+```
+procedures:
+  development:
+    - name: create_temp_database
+      replace_if_exists: true
+      database: {{ env.get('SNOWFLAKE_DATABASE') }}
+      schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
+      ...
+
+  admin:
+    - name: create_database_reader
+      replace_if_exists: true
+      database: {{ env.get('SNOWFLAKE_DATABASE') }}
+      schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
+      ...
+
+    - name: create_database_writer
+      replace_if_exists: true
+      database: {{ env.get('SNOWFLAKE_DATABASE') }}
+      schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
+      ...
+```
 
 <!-- LICENSE -->
 ## License
 
 Distributed under the MIT License. See `LICENSE` for more information.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -14,28 +14,36 @@
    3. _U_s_a_g_e
    4. _R_o_a_d_m_a_p
    5. _C_o_n_t_r_i_b_u_t_i_n_g
    6. _L_i_c_e_n_s_e
    7. _C_o_n_t_a_c_t
    8. _A_c_k_n_o_w_l_e_d_g_m_e_n_t_s
 ## About The Project `sprocketship` makes it easy to develop, manage, and
-deploy stored procedures in snowflake. Using the language of your choosing, you
+deploy stored procedures in Snowflake. Using the language of your choosing, you
 can write the contents of your stored procedure separately from its
 configurations (e.g., `EXECUTE AS`, `RETURN TYPE`, etc.). ### Built With_[_h_t_t_p_s_:
 _/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_p_i_p_e_l_i_n_e_-_t_o_o_l_s_/_A_B_S_Q_L_/
 _5_9_8_f_c_a_b_4_a_5_c_c_b_1_c_a_6_7_4_c_4_0_e_7_4_0_b_4_e_d_d_9_f_9_9_2_5_1_a_6_/_i_m_a_g_e_s_/_l_o_g_o___4_0_0_._s_v_g_]
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-### Installation `pip install sprocketship` ## Usage Use this space to show
-useful examples of how a project can be used. Additional screenshots, code
-examples and demos work well in this space. You may also link to more
-resources. _For more examples, please refer to the [Documentation](https://
-example.com)_
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## License Distributed under the MIT License. See `LICENSE` for more
-information.
+### Installation `pip install sprocketship` ## Usage Currently, sprocketship
+expects a `.sprocketship.yml` file and a `procedures/` directory at the same
+level in a directory structure. ``` âââ dbt_models â âââ
+customers.sql â âââ products.sql âââ procedures â âââ
+admin â â âââ create_database_writer_role.js â â âââ
+create_database_reader_role.js â âââ development â â âââ
+create_temp_database.js âââ .sprocketship.yml ``` The yaml path to each
+procedure in the `sprocketship.yml` should follow that of the paths to their
+corresponding files in the `procedures/` directory. ``` procedures:
+development: - name: create_temp_database replace_if_exists: true database: {
+{ env.get('SNOWFLAKE_DATABASE') }} schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
+... admin: - name: create_database_reader replace_if_exists: true database: {
+{ env.get('SNOWFLAKE_DATABASE') }} schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
+... - name: create_database_writer replace_if_exists: true database: {{ env.get
+('SNOWFLAKE_DATABASE') }} schema: {{ env.get('SNOWFLAKE_SCHEMA') }} ... ``` ##
+License Distributed under the MIT License. See `LICENSE` for more information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/
 nicklausroach/sprocketship.svg?style=for-the-badge [contributors-url]: https://
 github.com/nicklausroach/sprocketship/graphs/contributors [forks-shield]:
 https://img.shields.io/github/forks/nicklausroach/sprocketship.svg?style=for-
 the-badge [forks-url]: https://github.com/nicklausroach/sprocketship/network/
 members [stars-shield]: https://img.shields.io/github/stars/nicklausroach/
```

### Comparing `sprocketship-0.0.3/pyproject.toml` & `sprocketship-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sprocketship"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Nicklaus Roacb", email="nicklausroach@gmail.com" },
 ]
 readme = "README.md"
 dependencies = [
     "click",
     "snowflake",
```

### Comparing `sprocketship-0.0.3/sprocketship/cli.py` & `sprocketship-0.0.4/sprocketship/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 @click.option("--dir", default=".")
 def main(subcommand, dir):
     if subcommand == "liftoff":
         click.echo(click.style(f"🚀 Sprocketship lifting off!", fg='white', bold=True))
         # Open config in current directory
 
         yaml = YAML(typ='safe')
-        with open(os.path.join(dir, '.sprocketship.yaml'), 'r') as file:
+        with open(os.path.join(dir, '.sprocketship.yml'), 'r') as file:
             data = yaml.load(Environment().from_string(file.read()).render(env=os.environ))
 
         con = connector.connect(**data["snowflake"])
 
         # Get the configurations for each procedure and attach relative path to file directory
         configs_with_paths = extract_configs(data["procedures"])
         procs = list(itertools.chain(*configs_with_paths.values()))
```

### Comparing `sprocketship-0.0.3/sprocketship.egg-info/PKG-INFO` & `sprocketship-0.0.4/sprocketship.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.0.3
+Version: 0.0.4
 Author-email: Nicklaus Roacb <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -88,15 +88,15 @@
 </details>
 
 
 
 <!-- ABOUT THE PROJECT -->
 ## About The Project
 
-`sprocketship` makes it easy to develop, manage, and deploy stored procedures in snowflake. Using the language of your choosing, you can write the contents of your stored procedure separately from its configurations (e.g., `EXECUTE AS`, `RETURN TYPE`, etc.). 
+`sprocketship` makes it easy to develop, manage, and deploy stored procedures in Snowflake. Using the language of your choosing, you can write the contents of your stored procedure separately from its configurations (e.g., `EXECUTE AS`, `RETURN TYPE`, etc.). 
 
 
 
 
 ### Built With
 
 <a href=https://github.com/pipeline-tools/ABSQL>
@@ -113,20 +113,53 @@
 `pip install sprocketship`
 
 
 
 <!-- USAGE EXAMPLES -->
 ## Usage
 
-Use this space to show useful examples of how a project can be used. Additional screenshots, code examples and demos work well in this space. You may also link to more resources.
-
-_For more examples, please refer to the [Documentation](https://example.com)_
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
+Currently, sprocketship expects a `.sprocketship.yml` file and a `procedures/` directory at the same level in a directory structure.
 
+```
+├── dbt_models
+│   ├── customers.sql
+│   ├── products.sql
+├── procedures
+│   ├── admin
+│   │   ├── create_database_writer_role.js
+│   │   ├── create_database_reader_role.js
+│   ├── development
+│   │   ├── create_temp_database.js
+└── .sprocketship.yml
+```
+
+The yaml path to each procedure in the `sprocketship.yml` should follow that of the paths to their corresponding files in the `procedures/` directory. 
+
+```
+procedures:
+  development:
+    - name: create_temp_database
+      replace_if_exists: true
+      database: {{ env.get('SNOWFLAKE_DATABASE') }}
+      schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
+      ...
+
+  admin:
+    - name: create_database_reader
+      replace_if_exists: true
+      database: {{ env.get('SNOWFLAKE_DATABASE') }}
+      schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
+      ...
+
+    - name: create_database_writer
+      replace_if_exists: true
+      database: {{ env.get('SNOWFLAKE_DATABASE') }}
+      schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
+      ...
+```
 
 <!-- LICENSE -->
 ## License
 
 Distributed under the MIT License. See `LICENSE` for more information.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.0.3 Author-email: Nicklaus
+Metadata-Version: 2.1 Name: sprocketship Version: 0.0.4 Author-email: Nicklaus
 Roacb
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel.yaml
@@ -23,28 +23,36 @@
    3. _U_s_a_g_e
    4. _R_o_a_d_m_a_p
    5. _C_o_n_t_r_i_b_u_t_i_n_g
    6. _L_i_c_e_n_s_e
    7. _C_o_n_t_a_c_t
    8. _A_c_k_n_o_w_l_e_d_g_m_e_n_t_s
 ## About The Project `sprocketship` makes it easy to develop, manage, and
-deploy stored procedures in snowflake. Using the language of your choosing, you
+deploy stored procedures in Snowflake. Using the language of your choosing, you
 can write the contents of your stored procedure separately from its
 configurations (e.g., `EXECUTE AS`, `RETURN TYPE`, etc.). ### Built With_[_h_t_t_p_s_:
 _/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_p_i_p_e_l_i_n_e_-_t_o_o_l_s_/_A_B_S_Q_L_/
 _5_9_8_f_c_a_b_4_a_5_c_c_b_1_c_a_6_7_4_c_4_0_e_7_4_0_b_4_e_d_d_9_f_9_9_2_5_1_a_6_/_i_m_a_g_e_s_/_l_o_g_o___4_0_0_._s_v_g_]
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-### Installation `pip install sprocketship` ## Usage Use this space to show
-useful examples of how a project can be used. Additional screenshots, code
-examples and demos work well in this space. You may also link to more
-resources. _For more examples, please refer to the [Documentation](https://
-example.com)_
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## License Distributed under the MIT License. See `LICENSE` for more
-information.
+### Installation `pip install sprocketship` ## Usage Currently, sprocketship
+expects a `.sprocketship.yml` file and a `procedures/` directory at the same
+level in a directory structure. ``` âââ dbt_models â âââ
+customers.sql â âââ products.sql âââ procedures â âââ
+admin â â âââ create_database_writer_role.js â â âââ
+create_database_reader_role.js â âââ development â â âââ
+create_temp_database.js âââ .sprocketship.yml ``` The yaml path to each
+procedure in the `sprocketship.yml` should follow that of the paths to their
+corresponding files in the `procedures/` directory. ``` procedures:
+development: - name: create_temp_database replace_if_exists: true database: {
+{ env.get('SNOWFLAKE_DATABASE') }} schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
+... admin: - name: create_database_reader replace_if_exists: true database: {
+{ env.get('SNOWFLAKE_DATABASE') }} schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
+... - name: create_database_writer replace_if_exists: true database: {{ env.get
+('SNOWFLAKE_DATABASE') }} schema: {{ env.get('SNOWFLAKE_SCHEMA') }} ... ``` ##
+License Distributed under the MIT License. See `LICENSE` for more information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/
 nicklausroach/sprocketship.svg?style=for-the-badge [contributors-url]: https://
 github.com/nicklausroach/sprocketship/graphs/contributors [forks-shield]:
 https://img.shields.io/github/forks/nicklausroach/sprocketship.svg?style=for-
 the-badge [forks-url]: https://github.com/nicklausroach/sprocketship/network/
 members [stars-shield]: https://img.shields.io/github/stars/nicklausroach/
```

