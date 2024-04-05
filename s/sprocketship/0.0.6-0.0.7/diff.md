# Comparing `tmp/sprocketship-0.0.6.tar.gz` & `tmp/sprocketship-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprocketship-0.0.6.tar", last modified: Fri Apr  5 16:46:43 2024, max compression
+gzip compressed data, was "sprocketship-0.0.7.tar", last modified: Fri Apr  5 17:33:53 2024, max compression
```

## Comparing `sprocketship-0.0.6.tar` & `sprocketship-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:46:43.510169 sprocketship-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 16:46:36.000000 sprocketship-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-04-05 16:46:43.510169 sprocketship-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-04-05 16:46:36.000000 sprocketship-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-05 16:46:36.000000 sprocketship-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:46:43.510169 sprocketship-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:46:43.510169 sprocketship-0.0.6/sprocketship/
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-04-05 16:46:36.000000 sprocketship-0.0.6/sprocketship/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:46:43.510169 sprocketship-0.0.6/sprocketship.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-04-05 16:46:43.000000 sprocketship-0.0.6/sprocketship.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-05 16:46:43.000000 sprocketship-0.0.6/sprocketship.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:46:43.000000 sprocketship-0.0.6/sprocketship.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 16:46:43.000000 sprocketship-0.0.6/sprocketship.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 16:46:43.000000 sprocketship-0.0.6/sprocketship.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 16:46:43.000000 sprocketship-0.0.6/sprocketship.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:33:53.758884 sprocketship-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 17:33:45.000000 sprocketship-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5964 2024-04-05 17:33:53.758884 sprocketship-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-05 17:33:45.000000 sprocketship-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-05 17:33:45.000000 sprocketship-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 17:33:53.758884 sprocketship-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:33:53.758884 sprocketship-0.0.7/sprocketship/
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-04-05 17:33:45.000000 sprocketship-0.0.7/sprocketship/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:33:53.758884 sprocketship-0.0.7/sprocketship.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5964 2024-04-05 17:33:53.000000 sprocketship-0.0.7/sprocketship.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-05 17:33:53.000000 sprocketship-0.0.7/sprocketship.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:33:53.000000 sprocketship-0.0.7/sprocketship.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 17:33:53.000000 sprocketship-0.0.7/sprocketship.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 17:33:53.000000 sprocketship-0.0.7/sprocketship.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 17:33:53.000000 sprocketship-0.0.7/sprocketship.egg-info/top_level.txt
```

### Comparing `sprocketship-0.0.6/LICENSE` & `sprocketship-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sprocketship-0.0.6/PKG-INFO` & `sprocketship-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.0.6
+Version: 0.0.7
 Author-email: Nicklaus Roacb <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -42,25 +42,21 @@
 [![LinkedIn][linkedin-shield]][linkedin-url]
 
 
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
-  <a href="https://github.com/nicklausroach/sprocketship" style="font-size: 30px">
+  <a href="https://github.com/nicklausroach/sprocketship" style="font-size: 30px; text-decoration: none;">
     ⚙️ 🚀
   </a>
 <h3 align="center">Sprocketship</h3>
 
   <p align="center">
     Better stored procedure management
-    <br />
-    <a href="https://github.com/nicklausroach/sprocketship"><strong>Explore the docs »</strong></a>
-    <br />
-    <br />
   </p>
 </div>
 
 
 
 <!-- TABLE OF CONTENTS -->
 <details>
@@ -75,19 +71,15 @@
     <li>
       <a href="#getting-started">Getting Started</a>
       <ul>
         <li><a href="#installation">Installation</a></li>
       </ul>
     </li>
     <li><a href="#usage">Usage</a></li>
-    <li><a href="#roadmap">Roadmap</a></li>
-    <li><a href="#contributing">Contributing</a></li>
     <li><a href="#license">License</a></li>
-    <li><a href="#contact">Contact</a></li>
-    <li><a href="#acknowledgments">Acknowledgments</a></li>
   </ol>
 </details>
 
 
 
 <!-- ABOUT THE PROJECT -->
 ## About The Project
@@ -104,14 +96,16 @@
 </a>
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- GETTING STARTED -->
+## Getting Started
+
 ### Installation
 
 `pip install sprocketship`
 
 
 
 <!-- USAGE EXAMPLES -->
```

#### html2text {}

```diff
@@ -1,61 +1,56 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.0.6 Author-email: Nicklaus
+Metadata-Version: 2.1 Name: sprocketship Version: 0.0.7 Author-email: Nicklaus
 Roacb
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel.yaml
 Requires-Dist: jinja2 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
 [Issues][issues-shield]][issues-url] [![LinkedIn][linkedin-shield]][linkedin-
 url]
                                   _â___ï_¸__ _ð___
                             ******** SSpprroocckkeettsshhiipp ********
                       Better stored procedure management
-                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
-
 Table of Contents
    1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _B_u_i_l_t_ _W_i_t_h
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
           o _I_n_s_t_a_l_l_a_t_i_o_n
    3. _U_s_a_g_e
-   4. _R_o_a_d_m_a_p
-   5. _C_o_n_t_r_i_b_u_t_i_n_g
-   6. _L_i_c_e_n_s_e
-   7. _C_o_n_t_a_c_t
-   8. _A_c_k_n_o_w_l_e_d_g_m_e_n_t_s
+   4. _L_i_c_e_n_s_e
 ## About The Project `sprocketship` makes it easy to develop, manage, and
 deploy stored procedures in Snowflake. Using the language of your choosing, you
 can write the contents of your stored procedure separately from its
 configurations (e.g., `EXECUTE AS`, `RETURN TYPE`, etc.). ### Built With_[_h_t_t_p_s_:
 _/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_p_i_p_e_l_i_n_e_-_t_o_o_l_s_/_A_B_S_Q_L_/
 _5_9_8_f_c_a_b_4_a_5_c_c_b_1_c_a_6_7_4_c_4_0_e_7_4_0_b_4_e_d_d_9_f_9_9_2_5_1_a_6_/_i_m_a_g_e_s_/_l_o_g_o___4_0_0_._s_v_g_]
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-### Installation `pip install sprocketship` ## Usage Currently, sprocketship
-expects a `.sprocketship.yml` file and a `procedures/` directory at the same
-level in a directory structure. ``` âââ dbt_models â âââ
-customers.sql â âââ products.sql âââ procedures â âââ
-admin â â âââ create_database_writer_role.js â â âââ
-create_database_reader_role.js â âââ development â â âââ
-create_temp_database.js âââ .sprocketship.yml ``` The yaml path to each
-procedure in the `sprocketship.yml` should follow that of the paths to their
-corresponding files in the `procedures/` directory. ``` procedures:
-development: - name: create_temp_database replace_if_exists: true database: {
-{ env.get('SNOWFLAKE_DATABASE') }} schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
-... admin: - name: create_database_reader replace_if_exists: true database: {
-{ env.get('SNOWFLAKE_DATABASE') }} schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
-... - name: create_database_writer replace_if_exists: true database: {{ env.get
-('SNOWFLAKE_DATABASE') }} schema: {{ env.get('SNOWFLAKE_SCHEMA') }} ... ```
-From here, simply run `sprocketship liftoff` from the project directory (or
-provide the directory, e.g. `sprocketship liftoff my/directory/path`) and
-sprocketship will launch your stored procedures into the given directory. ##
-License Distributed under the MIT License. See `LICENSE` for more information.
+## Getting Started ### Installation `pip install sprocketship` ## Usage
+Currently, sprocketship expects a `.sprocketship.yml` file and a `procedures/
+` directory at the same level in a directory structure. ``` âââ
+dbt_models â âââ customers.sql â âââ products.sql âââ
+procedures â âââ admin â â âââ create_database_writer_role.js
+â â âââ create_database_reader_role.js â âââ development â
+â âââ create_temp_database.js âââ .sprocketship.yml ``` The yaml
+path to each procedure in the `sprocketship.yml` should follow that of the
+paths to their corresponding files in the `procedures/` directory. ```
+procedures: development: - name: create_temp_database replace_if_exists: true
+database: {{ env.get('SNOWFLAKE_DATABASE') }} schema: {{ env.get
+('SNOWFLAKE_SCHEMA') }} ... admin: - name: create_database_reader
+replace_if_exists: true database: {{ env.get('SNOWFLAKE_DATABASE') }} schema: {
+{ env.get('SNOWFLAKE_SCHEMA') }} ... - name: create_database_writer
+replace_if_exists: true database: {{ env.get('SNOWFLAKE_DATABASE') }} schema: {
+{ env.get('SNOWFLAKE_SCHEMA') }} ... ``` From here, simply run `sprocketship
+liftoff` from the project directory (or provide the directory, e.g.
+`sprocketship liftoff my/directory/path`) and sprocketship will launch your
+stored procedures into the given directory. ## License Distributed under the
+MIT License. See `LICENSE` for more information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/
 nicklausroach/sprocketship.svg?style=for-the-badge [contributors-url]: https://
 github.com/nicklausroach/sprocketship/graphs/contributors [forks-shield]:
 https://img.shields.io/github/forks/nicklausroach/sprocketship.svg?style=for-
 the-badge [forks-url]: https://github.com/nicklausroach/sprocketship/network/
 members [stars-shield]: https://img.shields.io/github/stars/nicklausroach/
```

### Comparing `sprocketship-0.0.6/README.md` & `sprocketship-0.0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -25,25 +25,21 @@
 [![LinkedIn][linkedin-shield]][linkedin-url]
 
 
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
-  <a href="https://github.com/nicklausroach/sprocketship" style="font-size: 30px">
+  <a href="https://github.com/nicklausroach/sprocketship" style="font-size: 30px; text-decoration: none;">
     ⚙️ 🚀
   </a>
 <h3 align="center">Sprocketship</h3>
 
   <p align="center">
     Better stored procedure management
-    <br />
-    <a href="https://github.com/nicklausroach/sprocketship"><strong>Explore the docs »</strong></a>
-    <br />
-    <br />
   </p>
 </div>
 
 
 
 <!-- TABLE OF CONTENTS -->
 <details>
@@ -58,19 +54,15 @@
     <li>
       <a href="#getting-started">Getting Started</a>
       <ul>
         <li><a href="#installation">Installation</a></li>
       </ul>
     </li>
     <li><a href="#usage">Usage</a></li>
-    <li><a href="#roadmap">Roadmap</a></li>
-    <li><a href="#contributing">Contributing</a></li>
     <li><a href="#license">License</a></li>
-    <li><a href="#contact">Contact</a></li>
-    <li><a href="#acknowledgments">Acknowledgments</a></li>
   </ol>
 </details>
 
 
 
 <!-- ABOUT THE PROJECT -->
 ## About The Project
@@ -87,14 +79,16 @@
 </a>
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- GETTING STARTED -->
+## Getting Started
+
 ### Installation
 
 `pip install sprocketship`
 
 
 
 <!-- USAGE EXAMPLES -->
```

#### html2text {}

```diff
@@ -1,52 +1,47 @@
 [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
 shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
 shield]][issues-url] [![LinkedIn][linkedin-shield]][linkedin-url]
                                   _â___ï_¸__ _ð___
                             ******** SSpprroocckkeettsshhiipp ********
                       Better stored procedure management
-                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
-
 Table of Contents
    1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _B_u_i_l_t_ _W_i_t_h
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
           o _I_n_s_t_a_l_l_a_t_i_o_n
    3. _U_s_a_g_e
-   4. _R_o_a_d_m_a_p
-   5. _C_o_n_t_r_i_b_u_t_i_n_g
-   6. _L_i_c_e_n_s_e
-   7. _C_o_n_t_a_c_t
-   8. _A_c_k_n_o_w_l_e_d_g_m_e_n_t_s
+   4. _L_i_c_e_n_s_e
 ## About The Project `sprocketship` makes it easy to develop, manage, and
 deploy stored procedures in Snowflake. Using the language of your choosing, you
 can write the contents of your stored procedure separately from its
 configurations (e.g., `EXECUTE AS`, `RETURN TYPE`, etc.). ### Built With_[_h_t_t_p_s_:
 _/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_p_i_p_e_l_i_n_e_-_t_o_o_l_s_/_A_B_S_Q_L_/
 _5_9_8_f_c_a_b_4_a_5_c_c_b_1_c_a_6_7_4_c_4_0_e_7_4_0_b_4_e_d_d_9_f_9_9_2_5_1_a_6_/_i_m_a_g_e_s_/_l_o_g_o___4_0_0_._s_v_g_]
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-### Installation `pip install sprocketship` ## Usage Currently, sprocketship
-expects a `.sprocketship.yml` file and a `procedures/` directory at the same
-level in a directory structure. ``` âââ dbt_models â âââ
-customers.sql â âââ products.sql âââ procedures â âââ
-admin â â âââ create_database_writer_role.js â â âââ
-create_database_reader_role.js â âââ development â â âââ
-create_temp_database.js âââ .sprocketship.yml ``` The yaml path to each
-procedure in the `sprocketship.yml` should follow that of the paths to their
-corresponding files in the `procedures/` directory. ``` procedures:
-development: - name: create_temp_database replace_if_exists: true database: {
-{ env.get('SNOWFLAKE_DATABASE') }} schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
-... admin: - name: create_database_reader replace_if_exists: true database: {
-{ env.get('SNOWFLAKE_DATABASE') }} schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
-... - name: create_database_writer replace_if_exists: true database: {{ env.get
-('SNOWFLAKE_DATABASE') }} schema: {{ env.get('SNOWFLAKE_SCHEMA') }} ... ```
-From here, simply run `sprocketship liftoff` from the project directory (or
-provide the directory, e.g. `sprocketship liftoff my/directory/path`) and
-sprocketship will launch your stored procedures into the given directory. ##
-License Distributed under the MIT License. See `LICENSE` for more information.
+## Getting Started ### Installation `pip install sprocketship` ## Usage
+Currently, sprocketship expects a `.sprocketship.yml` file and a `procedures/
+` directory at the same level in a directory structure. ``` âââ
+dbt_models â âââ customers.sql â âââ products.sql âââ
+procedures â âââ admin â â âââ create_database_writer_role.js
+â â âââ create_database_reader_role.js â âââ development â
+â âââ create_temp_database.js âââ .sprocketship.yml ``` The yaml
+path to each procedure in the `sprocketship.yml` should follow that of the
+paths to their corresponding files in the `procedures/` directory. ```
+procedures: development: - name: create_temp_database replace_if_exists: true
+database: {{ env.get('SNOWFLAKE_DATABASE') }} schema: {{ env.get
+('SNOWFLAKE_SCHEMA') }} ... admin: - name: create_database_reader
+replace_if_exists: true database: {{ env.get('SNOWFLAKE_DATABASE') }} schema: {
+{ env.get('SNOWFLAKE_SCHEMA') }} ... - name: create_database_writer
+replace_if_exists: true database: {{ env.get('SNOWFLAKE_DATABASE') }} schema: {
+{ env.get('SNOWFLAKE_SCHEMA') }} ... ``` From here, simply run `sprocketship
+liftoff` from the project directory (or provide the directory, e.g.
+`sprocketship liftoff my/directory/path`) and sprocketship will launch your
+stored procedures into the given directory. ## License Distributed under the
+MIT License. See `LICENSE` for more information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/
 nicklausroach/sprocketship.svg?style=for-the-badge [contributors-url]: https://
 github.com/nicklausroach/sprocketship/graphs/contributors [forks-shield]:
 https://img.shields.io/github/forks/nicklausroach/sprocketship.svg?style=for-
 the-badge [forks-url]: https://github.com/nicklausroach/sprocketship/network/
 members [stars-shield]: https://img.shields.io/github/stars/nicklausroach/
```

### Comparing `sprocketship-0.0.6/pyproject.toml` & `sprocketship-0.0.7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sprocketship"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Nicklaus Roacb", email="nicklausroach@gmail.com" },
 ]
 readme = "README.md"
 dependencies = [
     "click",
     "snowflake",
```

### Comparing `sprocketship-0.0.6/sprocketship/cli.py` & `sprocketship-0.0.7/sprocketship/cli.py`

 * *Files identical despite different names*

### Comparing `sprocketship-0.0.6/sprocketship.egg-info/PKG-INFO` & `sprocketship-0.0.7/sprocketship.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.0.6
+Version: 0.0.7
 Author-email: Nicklaus Roacb <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -42,25 +42,21 @@
 [![LinkedIn][linkedin-shield]][linkedin-url]
 
 
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
-  <a href="https://github.com/nicklausroach/sprocketship" style="font-size: 30px">
+  <a href="https://github.com/nicklausroach/sprocketship" style="font-size: 30px; text-decoration: none;">
     ⚙️ 🚀
   </a>
 <h3 align="center">Sprocketship</h3>
 
   <p align="center">
     Better stored procedure management
-    <br />
-    <a href="https://github.com/nicklausroach/sprocketship"><strong>Explore the docs »</strong></a>
-    <br />
-    <br />
   </p>
 </div>
 
 
 
 <!-- TABLE OF CONTENTS -->
 <details>
@@ -75,19 +71,15 @@
     <li>
       <a href="#getting-started">Getting Started</a>
       <ul>
         <li><a href="#installation">Installation</a></li>
       </ul>
     </li>
     <li><a href="#usage">Usage</a></li>
-    <li><a href="#roadmap">Roadmap</a></li>
-    <li><a href="#contributing">Contributing</a></li>
     <li><a href="#license">License</a></li>
-    <li><a href="#contact">Contact</a></li>
-    <li><a href="#acknowledgments">Acknowledgments</a></li>
   </ol>
 </details>
 
 
 
 <!-- ABOUT THE PROJECT -->
 ## About The Project
@@ -104,14 +96,16 @@
 </a>
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- GETTING STARTED -->
+## Getting Started
+
 ### Installation
 
 `pip install sprocketship`
 
 
 
 <!-- USAGE EXAMPLES -->
```

#### html2text {}

```diff
@@ -1,61 +1,56 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.0.6 Author-email: Nicklaus
+Metadata-Version: 2.1 Name: sprocketship Version: 0.0.7 Author-email: Nicklaus
 Roacb
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel.yaml
 Requires-Dist: jinja2 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
 [Issues][issues-shield]][issues-url] [![LinkedIn][linkedin-shield]][linkedin-
 url]
                                   _â___ï_¸__ _ð___
                             ******** SSpprroocckkeettsshhiipp ********
                       Better stored procedure management
-                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
-
 Table of Contents
    1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _B_u_i_l_t_ _W_i_t_h
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
           o _I_n_s_t_a_l_l_a_t_i_o_n
    3. _U_s_a_g_e
-   4. _R_o_a_d_m_a_p
-   5. _C_o_n_t_r_i_b_u_t_i_n_g
-   6. _L_i_c_e_n_s_e
-   7. _C_o_n_t_a_c_t
-   8. _A_c_k_n_o_w_l_e_d_g_m_e_n_t_s
+   4. _L_i_c_e_n_s_e
 ## About The Project `sprocketship` makes it easy to develop, manage, and
 deploy stored procedures in Snowflake. Using the language of your choosing, you
 can write the contents of your stored procedure separately from its
 configurations (e.g., `EXECUTE AS`, `RETURN TYPE`, etc.). ### Built With_[_h_t_t_p_s_:
 _/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_p_i_p_e_l_i_n_e_-_t_o_o_l_s_/_A_B_S_Q_L_/
 _5_9_8_f_c_a_b_4_a_5_c_c_b_1_c_a_6_7_4_c_4_0_e_7_4_0_b_4_e_d_d_9_f_9_9_2_5_1_a_6_/_i_m_a_g_e_s_/_l_o_g_o___4_0_0_._s_v_g_]
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-### Installation `pip install sprocketship` ## Usage Currently, sprocketship
-expects a `.sprocketship.yml` file and a `procedures/` directory at the same
-level in a directory structure. ``` âââ dbt_models â âââ
-customers.sql â âââ products.sql âââ procedures â âââ
-admin â â âââ create_database_writer_role.js â â âââ
-create_database_reader_role.js â âââ development â â âââ
-create_temp_database.js âââ .sprocketship.yml ``` The yaml path to each
-procedure in the `sprocketship.yml` should follow that of the paths to their
-corresponding files in the `procedures/` directory. ``` procedures:
-development: - name: create_temp_database replace_if_exists: true database: {
-{ env.get('SNOWFLAKE_DATABASE') }} schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
-... admin: - name: create_database_reader replace_if_exists: true database: {
-{ env.get('SNOWFLAKE_DATABASE') }} schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
-... - name: create_database_writer replace_if_exists: true database: {{ env.get
-('SNOWFLAKE_DATABASE') }} schema: {{ env.get('SNOWFLAKE_SCHEMA') }} ... ```
-From here, simply run `sprocketship liftoff` from the project directory (or
-provide the directory, e.g. `sprocketship liftoff my/directory/path`) and
-sprocketship will launch your stored procedures into the given directory. ##
-License Distributed under the MIT License. See `LICENSE` for more information.
+## Getting Started ### Installation `pip install sprocketship` ## Usage
+Currently, sprocketship expects a `.sprocketship.yml` file and a `procedures/
+` directory at the same level in a directory structure. ``` âââ
+dbt_models â âââ customers.sql â âââ products.sql âââ
+procedures â âââ admin â â âââ create_database_writer_role.js
+â â âââ create_database_reader_role.js â âââ development â
+â âââ create_temp_database.js âââ .sprocketship.yml ``` The yaml
+path to each procedure in the `sprocketship.yml` should follow that of the
+paths to their corresponding files in the `procedures/` directory. ```
+procedures: development: - name: create_temp_database replace_if_exists: true
+database: {{ env.get('SNOWFLAKE_DATABASE') }} schema: {{ env.get
+('SNOWFLAKE_SCHEMA') }} ... admin: - name: create_database_reader
+replace_if_exists: true database: {{ env.get('SNOWFLAKE_DATABASE') }} schema: {
+{ env.get('SNOWFLAKE_SCHEMA') }} ... - name: create_database_writer
+replace_if_exists: true database: {{ env.get('SNOWFLAKE_DATABASE') }} schema: {
+{ env.get('SNOWFLAKE_SCHEMA') }} ... ``` From here, simply run `sprocketship
+liftoff` from the project directory (or provide the directory, e.g.
+`sprocketship liftoff my/directory/path`) and sprocketship will launch your
+stored procedures into the given directory. ## License Distributed under the
+MIT License. See `LICENSE` for more information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/
 nicklausroach/sprocketship.svg?style=for-the-badge [contributors-url]: https://
 github.com/nicklausroach/sprocketship/graphs/contributors [forks-shield]:
 https://img.shields.io/github/forks/nicklausroach/sprocketship.svg?style=for-
 the-badge [forks-url]: https://github.com/nicklausroach/sprocketship/network/
 members [stars-shield]: https://img.shields.io/github/stars/nicklausroach/
```

