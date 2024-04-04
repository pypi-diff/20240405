# Comparing `tmp/squirrels-0.2.1.tar.gz` & `tmp/squirrels-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squirrels-0.2.1.tar", max compression
+gzip compressed data, was "squirrels-0.2.2.tar", max compression
```

## Comparing `squirrels-0.2.1.tar` & `squirrels-0.2.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1067 2024-02-24 16:07:43.661375 squirrels-0.2.1/LICENSE
--rw-r--r--   0        0        0     3670 2024-02-24 16:07:43.661375 squirrels-0.2.1/README.md
--rw-r--r--   0        0        0     1220 2024-02-24 16:07:43.661375 squirrels-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      664 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/__init__.py
--rw-r--r--   0        0        0    15499 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/_api_server.py
--rw-r--r--   0        0        0     3742 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/_authenticator.py
--rw-r--r--   0        0        0     5668 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/_command_line.py
--rw-r--r--   0        0        0     2563 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/_connection_set.py
--rw-r--r--   0        0        0     3865 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/_constants.py
--rw-r--r--   0        0        0     2761 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/_environcfg.py
--rw-r--r--   0        0        0     7750 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/_initializer.py
--rw-r--r--   0        0        0     8599 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/_manifest.py
--rw-r--r--   0        0        0    21728 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/_models.py
--rw-r--r--   0        0        0     1020 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/_package_loader.py
--rw-r--r--   0        0        0    17120 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/_parameter_configs.py
--rw-r--r--   0        0        0     8917 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/_parameter_sets.py
--rw-r--r--   0        0        0     2624 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/_py_module.py
--rw-r--r--   0        0        0      802 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/_timer.py
--rw-r--r--   0        0        0     5438 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/_utils.py
--rw-r--r--   0        0        0      109 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/_version.py
--rw-r--r--   0        0        0      783 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/arguments/init_time_args.py
--rw-r--r--   0        0        0     3195 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/arguments/run_time_args.py
--rw-r--r--   0        0        0    25864 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/data_sources.py
--rw-r--r--   0        0        0    16487 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/dateutils.py
--rw-r--r--   0        0        0    61022 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/package_data/assets/favicon.ico
--rw-r--r--   0        0        0    11572 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/package_data/assets/index.css
--rw-r--r--   0        0        0   260298 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/package_data/assets/index.js
--rw-r--r--   0        0        0      134 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/package_data/base_project/.gitignore
--rw-r--r--   0        0        0      255 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/package_data/base_project/connections.yml
--rw-r--r--   0        0        0    36864 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/package_data/base_project/database/expenses.db
--rw-r--r--   0        0        0   188416 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/package_data/base_project/database/weather.db
--rw-r--r--   0        0        0       90 2024-02-24 16:07:43.665375 squirrels-0.2.1/squirrels/package_data/base_project/docker/.dockerignore
--rw-r--r--   0        0        0      467 2024-02-24 16:07:43.669375 squirrels-0.2.1/squirrels/package_data/base_project/docker/Dockerfile
--rw-r--r--   0        0        0      125 2024-02-24 16:07:43.669375 squirrels-0.2.1/squirrels/package_data/base_project/docker/compose.yml
--rw-r--r--   0        0        0      859 2024-02-24 16:07:43.669375 squirrels-0.2.1/squirrels/package_data/base_project/environcfg.yml
--rw-r--r--   0        0        0     1655 2024-02-24 16:07:43.669375 squirrels-0.2.1/squirrels/package_data/base_project/models/dbviews/database_view1.py
--rw-r--r--   0        0        0      488 2024-02-24 16:07:43.669375 squirrels-0.2.1/squirrels/package_data/base_project/models/dbviews/database_view1.sql
--rw-r--r--   0        0        0      686 2024-02-24 16:07:43.669375 squirrels-0.2.1/squirrels/package_data/base_project/models/federates/dataset_example.py
--rw-r--r--   0        0        0       78 2024-02-24 16:07:43.669375 squirrels-0.2.1/squirrels/package_data/base_project/models/federates/dataset_example.sql
--rw-r--r--   0        0        0     4463 2024-02-24 16:07:43.669375 squirrels-0.2.1/squirrels/package_data/base_project/parameters.yml
--rw-r--r--   0        0        0     1567 2024-02-24 16:07:43.669375 squirrels-0.2.1/squirrels/package_data/base_project/pyconfigs/auth.py
--rw-r--r--   0        0        0      809 2024-02-24 16:07:43.669375 squirrels-0.2.1/squirrels/package_data/base_project/pyconfigs/connections.py
--rw-r--r--   0        0        0     2599 2024-02-24 16:07:43.669375 squirrels-0.2.1/squirrels/package_data/base_project/pyconfigs/context.py
--rw-r--r--   0        0        0     3077 2024-02-24 16:07:43.669375 squirrels-0.2.1/squirrels/package_data/base_project/pyconfigs/parameters.py
--rw-r--r--   0        0        0       35 2024-02-24 16:07:43.669375 squirrels-0.2.1/squirrels/package_data/base_project/seeds/mocks/category.csv
--rw-r--r--   0        0        0       38 2024-02-24 16:07:43.669375 squirrels-0.2.1/squirrels/package_data/base_project/seeds/mocks/max_filter.csv
--rw-r--r--   0        0        0      105 2024-02-24 16:07:43.669375 squirrels-0.2.1/squirrels/package_data/base_project/seeds/mocks/subcategory.csv
--rw-r--r--   0        0        0     1727 2024-02-24 16:07:43.669375 squirrels-0.2.1/squirrels/package_data/base_project/squirrels.yml.j2
--rw-r--r--   0        0        0       13 2024-02-24 16:07:43.669375 squirrels-0.2.1/squirrels/package_data/base_project/tmp/.gitignore
--rw-r--r--   0        0        0      572 2024-02-24 16:07:43.669375 squirrels-0.2.1/squirrels/package_data/templates/index.html
--rw-r--r--   0        0        0    15638 2024-02-24 16:07:43.669375 squirrels-0.2.1/squirrels/parameter_options.py
--rw-r--r--   0        0        0    32401 2024-02-24 16:07:43.669375 squirrels-0.2.1/squirrels/parameters.py
--rw-r--r--   0        0        0     1698 2024-02-24 16:07:43.669375 squirrels-0.2.1/squirrels/user_base.py
--rw-r--r--   0        0        0     5208 1970-01-01 00:00:00.000000 squirrels-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-04 22:43:23.048620 squirrels-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3642 2024-04-04 22:43:23.048620 squirrels-0.2.2/README.md
+-rw-r--r--   0        0        0     1220 2024-04-04 22:43:23.048620 squirrels-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      664 2024-04-04 22:43:23.048620 squirrels-0.2.2/squirrels/__init__.py
+-rw-r--r--   0        0        0    15499 2024-04-04 22:43:23.048620 squirrels-0.2.2/squirrels/_api_server.py
+-rw-r--r--   0        0        0     3742 2024-04-04 22:43:23.048620 squirrels-0.2.2/squirrels/_authenticator.py
+-rw-r--r--   0        0        0     5668 2024-04-04 22:43:23.048620 squirrels-0.2.2/squirrels/_command_line.py
+-rw-r--r--   0        0        0     2563 2024-04-04 22:43:23.048620 squirrels-0.2.2/squirrels/_connection_set.py
+-rw-r--r--   0        0        0     3865 2024-04-04 22:43:23.048620 squirrels-0.2.2/squirrels/_constants.py
+-rw-r--r--   0        0        0     2761 2024-04-04 22:43:23.048620 squirrels-0.2.2/squirrels/_environcfg.py
+-rw-r--r--   0        0        0     7750 2024-04-04 22:43:23.048620 squirrels-0.2.2/squirrels/_initializer.py
+-rw-r--r--   0        0        0     8599 2024-04-04 22:43:23.048620 squirrels-0.2.2/squirrels/_manifest.py
+-rw-r--r--   0        0        0    21828 2024-04-04 22:43:23.048620 squirrels-0.2.2/squirrels/_models.py
+-rw-r--r--   0        0        0     1020 2024-04-04 22:43:23.048620 squirrels-0.2.2/squirrels/_package_loader.py
+-rw-r--r--   0        0        0    17120 2024-04-04 22:43:23.048620 squirrels-0.2.2/squirrels/_parameter_configs.py
+-rw-r--r--   0        0        0     8917 2024-04-04 22:43:23.048620 squirrels-0.2.2/squirrels/_parameter_sets.py
+-rw-r--r--   0        0        0     2624 2024-04-04 22:43:23.048620 squirrels-0.2.2/squirrels/_py_module.py
+-rw-r--r--   0        0        0      802 2024-04-04 22:43:23.048620 squirrels-0.2.2/squirrels/_timer.py
+-rw-r--r--   0        0        0     5438 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/_utils.py
+-rw-r--r--   0        0        0      109 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/_version.py
+-rw-r--r--   0        0        0      783 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/arguments/init_time_args.py
+-rw-r--r--   0        0        0     3195 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/arguments/run_time_args.py
+-rw-r--r--   0        0        0    25864 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/data_sources.py
+-rw-r--r--   0        0        0    16487 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/dateutils.py
+-rw-r--r--   0        0        0    61022 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/package_data/assets/favicon.ico
+-rw-r--r--   0        0        0    11572 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/package_data/assets/index.css
+-rw-r--r--   0        0        0   260298 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/package_data/assets/index.js
+-rw-r--r--   0        0        0      134 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/package_data/base_project/.gitignore
+-rw-r--r--   0        0        0      255 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/package_data/base_project/connections.yml
+-rw-r--r--   0        0        0    36864 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/package_data/base_project/database/expenses.db
+-rw-r--r--   0        0        0   188416 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/package_data/base_project/database/weather.db
+-rw-r--r--   0        0        0       90 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/package_data/base_project/docker/.dockerignore
+-rw-r--r--   0        0        0      467 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/package_data/base_project/docker/Dockerfile
+-rw-r--r--   0        0        0      125 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/package_data/base_project/docker/compose.yml
+-rw-r--r--   0        0        0      859 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/package_data/base_project/environcfg.yml
+-rw-r--r--   0        0        0     1655 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/package_data/base_project/models/dbviews/database_view1.py
+-rw-r--r--   0        0        0      488 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/package_data/base_project/models/dbviews/database_view1.sql
+-rw-r--r--   0        0        0      686 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/package_data/base_project/models/federates/dataset_example.py
+-rw-r--r--   0        0        0       78 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/package_data/base_project/models/federates/dataset_example.sql
+-rw-r--r--   0        0        0     4463 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/package_data/base_project/parameters.yml
+-rw-r--r--   0        0        0     1567 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/package_data/base_project/pyconfigs/auth.py
+-rw-r--r--   0        0        0      809 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/package_data/base_project/pyconfigs/connections.py
+-rw-r--r--   0        0        0     2599 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/package_data/base_project/pyconfigs/context.py
+-rw-r--r--   0        0        0     3077 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/package_data/base_project/pyconfigs/parameters.py
+-rw-r--r--   0        0        0       35 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/package_data/base_project/seeds/mocks/category.csv
+-rw-r--r--   0        0        0       38 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/package_data/base_project/seeds/mocks/max_filter.csv
+-rw-r--r--   0        0        0      105 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/package_data/base_project/seeds/mocks/subcategory.csv
+-rw-r--r--   0        0        0     1727 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/package_data/base_project/squirrels.yml.j2
+-rw-r--r--   0        0        0       13 2024-04-04 22:43:23.052620 squirrels-0.2.2/squirrels/package_data/base_project/tmp/.gitignore
+-rw-r--r--   0        0        0      572 2024-04-04 22:43:23.056620 squirrels-0.2.2/squirrels/package_data/templates/index.html
+-rw-r--r--   0        0        0    15638 2024-04-04 22:43:23.056620 squirrels-0.2.2/squirrels/parameter_options.py
+-rw-r--r--   0        0        0    32401 2024-04-04 22:43:23.056620 squirrels-0.2.2/squirrels/parameters.py
+-rw-r--r--   0        0        0     1698 2024-04-04 22:43:23.056620 squirrels-0.2.2/squirrels/user_base.py
+-rw-r--r--   0        0        0     5180 1970-01-01 00:00:00.000000 squirrels-0.2.2/PKG-INFO
```

### Comparing `squirrels-0.2.1/LICENSE` & `squirrels-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/README.md` & `squirrels-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Squirrels
 
 Squirrels is an API framework that lets you create REST APIs for dynamic data analytics!
 
-**Documentation**: <a href="https://squirrels-nest.github.io/squirrels-docs" target="_blank">https://squirrels-nest.github.io/squirrels-docs</a>
+**Documentation**: <a href="https://squirrels-nest.github.io/" target="_blank">https://squirrels-nest.github.io/</a>
 
 **Source Code**: <a href="https://github.com/squirrels-nest/squirrels" target="_blank">https://github.com/squirrels-nest/squirrels</a>
 
 ## Table of Contents
 
 - [Main Features](#main-features)
 - [License](#license)
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # Squirrels Squirrels is an API framework that lets you create REST APIs for
 dynamic data analytics! **Documentation**: _h_t_t_p_s_:_/_/_s_q_u_i_r_r_e_l_s_-_n_e_s_t_._g_i_t_h_u_b_._i_o_/
-_s_q_u_i_r_r_e_l_s_-_d_o_c_s **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_s_q_u_i_r_r_e_l_s_-_n_e_s_t_/_s_q_u_i_r_r_e_l_s ##
-Table of Contents - [Main Features](#main-features) - [License](#license) -
+**Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_s_q_u_i_r_r_e_l_s_-_n_e_s_t_/_s_q_u_i_r_r_e_l_s ## Table of
+Contents - [Main Features](#main-features) - [License](#license) -
 [Contributing to squirrels](#contributing-to-squirrels) - [Setup](#setup) -
 [Testing](#testing) - [Project Structure](#project-structure) ## Main Features
 Here are a few of the things that squirrels can do: - Connect to any database
 by specifying its sqlalchemy url without code (in `squirrels.yml`) or by using
 its native connector library in python (in `connections.py`). - Configure API
 routes without code (in `squirrels.yml`) for all datasets. - Configure
 parameter widgets (types include single-select, multi-select, date, number,
```

### Comparing `squirrels-0.2.1/pyproject.toml` & `squirrels-0.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "squirrels"
-version = "0.2.1"
+version = "0.2.2"
 description = "Squirrels - API Framework for Data Analytics"
 license = "MIT"
 authors = ["Tim Huang <tim.yuting@hotmail.com>"]
 readme = "README.md"
 homepage = "https://squirrels-nest.github.io"
 repository = "https://github.com/squirrels-nest/squirrels"
 documentation = "https://squirrels-nest.github.io"
```

### Comparing `squirrels-0.2.1/squirrels/__init__.py` & `squirrels-0.2.2/squirrels/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.2.1'
+__version__ = '0.2.2'
 
 from .arguments.init_time_args import ConnectionsArgs, ParametersArgs
 from .arguments.run_time_args import AuthArgs, ContextArgs, ModelDepsArgs, ModelArgs
 from .parameter_options import SelectParameterOption, DateParameterOption, DateRangeParameterOption, NumberParameterOption, NumberRangeParameterOption
 from .parameters import SingleSelectParameter, MultiSelectParameter, DateParameter, DateRangeParameter, NumberParameter, NumberRangeParameter
 from .data_sources import SingleSelectDataSource, MultiSelectDataSource, DateDataSource, DateRangeDataSource, NumberDataSource, NumberRangeDataSource
 from .user_base import User, WrongPassword
```

### Comparing `squirrels-0.2.1/squirrels/_api_server.py` & `squirrels-0.2.2/squirrels/_api_server.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/_authenticator.py` & `squirrels-0.2.2/squirrels/_authenticator.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/_command_line.py` & `squirrels-0.2.2/squirrels/_command_line.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/_connection_set.py` & `squirrels-0.2.2/squirrels/_connection_set.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/_constants.py` & `squirrels-0.2.2/squirrels/_constants.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/_environcfg.py` & `squirrels-0.2.2/squirrels/_environcfg.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/_initializer.py` & `squirrels-0.2.2/squirrels/_initializer.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/_manifest.py` & `squirrels-0.2.2/squirrels/_manifest.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/_models.py` & `squirrels-0.2.2/squirrels/_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,29 +211,29 @@
         coroutines = []
         for dep_model in dep_models:
             self._add_upstream(dep_model)
             coro = dep_model.compile(ctx, ctx_args, models_dict, recurse)
             coroutines.append(coro)
         await asyncio.gather(*coroutines)
     
-    def validate_no_cycles(self, depencency_path: set[str]) -> set[str]:
+    def get_terminal_nodes(self, depencency_path: set[str]) -> set[str]:
         if self.confirmed_no_cycles:
-            return
+            return set()
         
         if self.name in depencency_path:
             raise u.ConfigurationError(f'Cycle found in model dependency graph')
 
         terminal_nodes = set()
         if len(self.upstreams) == 0:
             terminal_nodes.add(self.name)
         else:
             new_path = set(depencency_path)
             new_path.add(self.name)
             for dep_model in self.upstreams.values():
-                terminal_nodes_under_dep = dep_model.validate_no_cycles(new_path)
+                terminal_nodes_under_dep = dep_model.get_terminal_nodes(new_path)
                 terminal_nodes = terminal_nodes.union(terminal_nodes_under_dep)
         
         self.confirmed_no_cycles = True
         return terminal_nodes
         
     def _load_pandas_to_table(self, df: pd.DataFrame, conn: sqlite3.Connection) -> None:
         if u.use_duckdb():
@@ -339,17 +339,19 @@
             raise u.FileExecutionError(f'Failed to run {c.CONTEXT_FILE} for dataset "{self.dataset}"', e)
         timer.add_activity_time(f"running context.py for dataset", start)
         return context, args
     
     async def _compile_models(self, context: dict[str, Any], ctx_args: ContextArgs, recurse: bool) -> None:
         await self.target_model.compile(context, ctx_args, self.models_dict, recurse)
     
-    def _validate_no_cycles(self) -> set[str]:
+    def _get_terminal_nodes(self) -> set[str]:
         start = time.time()
-        terminal_nodes = self.target_model.validate_no_cycles(set())
+        terminal_nodes = self.target_model.get_terminal_nodes(set())
+        for model in self.models_dict.values():
+            model.confirmed_no_cycles = False
         timer.add_activity_time(f"validating no cycles in models dependencies", start)
         return terminal_nodes
 
     async def _run_models(self, terminal_nodes: set[str]) -> None:
         if u.use_duckdb():
             import duckdb
             conn = duckdb.connect()
@@ -373,15 +375,15 @@
 
         self.apply_selections(user, selections, request_version=request_version)
 
         context, ctx_args = self._compile_context(context_func, user)
 
         await self._compile_models(context, ctx_args, recurse)
         
-        terminal_nodes = self._validate_no_cycles()
+        terminal_nodes = self._get_terminal_nodes()
 
         if runquery:
             await self._run_models(terminal_nodes)
     
     def get_all_model_names(self) -> set[str]:
         all_model_names = set()
         self.target_model.fill_dependent_model_names(all_model_names)
```

### Comparing `squirrels-0.2.1/squirrels/_package_loader.py` & `squirrels-0.2.2/squirrels/_package_loader.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/_parameter_configs.py` & `squirrels-0.2.2/squirrels/_parameter_configs.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/_parameter_sets.py` & `squirrels-0.2.2/squirrels/_parameter_sets.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/_py_module.py` & `squirrels-0.2.2/squirrels/_py_module.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/_timer.py` & `squirrels-0.2.2/squirrels/_timer.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/_utils.py` & `squirrels-0.2.2/squirrels/_utils.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/arguments/init_time_args.py` & `squirrels-0.2.2/squirrels/arguments/init_time_args.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/arguments/run_time_args.py` & `squirrels-0.2.2/squirrels/arguments/run_time_args.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/data_sources.py` & `squirrels-0.2.2/squirrels/data_sources.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/dateutils.py` & `squirrels-0.2.2/squirrels/dateutils.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/package_data/assets/favicon.ico` & `squirrels-0.2.2/squirrels/package_data/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/package_data/assets/index.css` & `squirrels-0.2.2/squirrels/package_data/assets/index.css`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/package_data/assets/index.js` & `squirrels-0.2.2/squirrels/package_data/assets/index.js`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/package_data/base_project/database/expenses.db` & `squirrels-0.2.2/squirrels/package_data/base_project/database/expenses.db`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/package_data/base_project/database/weather.db` & `squirrels-0.2.2/squirrels/package_data/base_project/database/weather.db`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/package_data/base_project/environcfg.yml` & `squirrels-0.2.2/squirrels/package_data/base_project/environcfg.yml`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/package_data/base_project/models/dbviews/database_view1.py` & `squirrels-0.2.2/squirrels/package_data/base_project/models/dbviews/database_view1.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/package_data/base_project/models/federates/dataset_example.py` & `squirrels-0.2.2/squirrels/package_data/base_project/models/federates/dataset_example.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/package_data/base_project/parameters.yml` & `squirrels-0.2.2/squirrels/package_data/base_project/parameters.yml`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/package_data/base_project/pyconfigs/auth.py` & `squirrels-0.2.2/squirrels/package_data/base_project/pyconfigs/auth.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/package_data/base_project/pyconfigs/connections.py` & `squirrels-0.2.2/squirrels/package_data/base_project/pyconfigs/connections.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/package_data/base_project/pyconfigs/context.py` & `squirrels-0.2.2/squirrels/package_data/base_project/pyconfigs/context.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/package_data/base_project/pyconfigs/parameters.py` & `squirrels-0.2.2/squirrels/package_data/base_project/pyconfigs/parameters.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/package_data/base_project/squirrels.yml.j2` & `squirrels-0.2.2/squirrels/package_data/base_project/squirrels.yml.j2`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/package_data/templates/index.html` & `squirrels-0.2.2/squirrels/package_data/templates/index.html`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/parameter_options.py` & `squirrels-0.2.2/squirrels/parameter_options.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/parameters.py` & `squirrels-0.2.2/squirrels/parameters.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/squirrels/user_base.py` & `squirrels-0.2.2/squirrels/user_base.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.2.1/PKG-INFO` & `squirrels-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squirrels
-Version: 0.2.1
+Version: 0.2.2
 Summary: Squirrels - API Framework for Data Analytics
 Home-page: https://squirrels-nest.github.io
 License: MIT
 Author: Tim Huang
 Author-email: tim.yuting@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
@@ -35,15 +35,15 @@
 Project-URL: Repository, https://github.com/squirrels-nest/squirrels
 Description-Content-Type: text/markdown
 
 # Squirrels
 
 Squirrels is an API framework that lets you create REST APIs for dynamic data analytics!
 
-**Documentation**: <a href="https://squirrels-nest.github.io/squirrels-docs" target="_blank">https://squirrels-nest.github.io/squirrels-docs</a>
+**Documentation**: <a href="https://squirrels-nest.github.io/" target="_blank">https://squirrels-nest.github.io/</a>
 
 **Source Code**: <a href="https://github.com/squirrels-nest/squirrels" target="_blank">https://github.com/squirrels-nest/squirrels</a>
 
 ## Table of Contents
 
 - [Main Features](#main-features)
 - [License](#license)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: squirrels Version: 0.2.1 Summary: Squirrels - API
+Metadata-Version: 2.1 Name: squirrels Version: 0.2.2 Summary: Squirrels - API
 Framework for Data Analytics Home-page: https://squirrels-nest.github.io
 License: MIT Author: Tim Huang Author-email: tim.yuting@hotmail.com Requires-
 Python: >=3.9,<4.0 Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
@@ -16,31 +16,31 @@
 pandas (>=2.1.4,<3.0.0) Requires-Dist: python-jose (>=3.3.0,<4.0.0) Requires-
 Dist: python-multipart (>=0.0.9,<0.0.10) Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: sqlalchemy (>=2.0.25,<3.0.0) Requires-Dist: uvicorn
 (>=0.27.1,<0.28.0) Project-URL: Documentation, https://squirrels-nest.github.io
 Project-URL: Repository, https://github.com/squirrels-nest/squirrels
 Description-Content-Type: text/markdown # Squirrels Squirrels is an API
 framework that lets you create REST APIs for dynamic data analytics!
-**Documentation**: _h_t_t_p_s_:_/_/_s_q_u_i_r_r_e_l_s_-_n_e_s_t_._g_i_t_h_u_b_._i_o_/_s_q_u_i_r_r_e_l_s_-_d_o_c_s **Source
-Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_s_q_u_i_r_r_e_l_s_-_n_e_s_t_/_s_q_u_i_r_r_e_l_s ## Table of Contents -
-[Main Features](#main-features) - [License](#license) - [Contributing to
-squirrels](#contributing-to-squirrels) - [Setup](#setup) - [Testing](#testing)
-- [Project Structure](#project-structure) ## Main Features Here are a few of
-the things that squirrels can do: - Connect to any database by specifying its
-sqlalchemy url without code (in `squirrels.yml`) or by using its native
-connector library in python (in `connections.py`). - Configure API routes
-without code (in `squirrels.yml`) for all datasets. - Configure parameter
-widgets (types include single-select, multi-select, date, number, etc.) for
-your datasets (in `parameters.py`). - Use Jinja SQL templates (just like dbt!)
-or python functions (that return a pandas dataframe) to define dynamic query
-logic based on parameter selections. - Query multiple databases and join the
-results together in a final view in one API endpoint/dataset! - Test your API
-endpoints with an interactive UI or by a command line that generates rendered
-sql queries and results (for a given set of parameter selections). - Define
-authentication logic (in `auth.py`) and authorize privacy scope per dataset (in
+**Documentation**: _h_t_t_p_s_:_/_/_s_q_u_i_r_r_e_l_s_-_n_e_s_t_._g_i_t_h_u_b_._i_o_/ **Source Code**: _h_t_t_p_s_:_/_/
+_g_i_t_h_u_b_._c_o_m_/_s_q_u_i_r_r_e_l_s_-_n_e_s_t_/_s_q_u_i_r_r_e_l_s ## Table of Contents - [Main Features]
+(#main-features) - [License](#license) - [Contributing to squirrels]
+(#contributing-to-squirrels) - [Setup](#setup) - [Testing](#testing) - [Project
+Structure](#project-structure) ## Main Features Here are a few of the things
+that squirrels can do: - Connect to any database by specifying its sqlalchemy
+url without code (in `squirrels.yml`) or by using its native connector library
+in python (in `connections.py`). - Configure API routes without code (in
+`squirrels.yml`) for all datasets. - Configure parameter widgets (types include
+single-select, multi-select, date, number, etc.) for your datasets (in
+`parameters.py`). - Use Jinja SQL templates (just like dbt!) or python
+functions (that return a pandas dataframe) to define dynamic query logic based
+on parameter selections. - Query multiple databases and join the results
+together in a final view in one API endpoint/dataset! - Test your API endpoints
+with an interactive UI or by a command line that generates rendered sql queries
+and results (for a given set of parameter selections). - Define authentication
+logic (in `auth.py`) and authorize privacy scope per dataset (in
 `squirrels.yml`). The user's attributes can even be used in your query logic!
 ## License Squirrels is released under the MIT license. See the file LICENSE
 for more details. ## Contributing to squirrels The sections below describe how
 to set up your local environment for squirrels development and run unit tests.
 A high level overview of the project structure is also provided. ### Setup This
 project requires python version 3.9 or above to be installed. It also uses the
 python build tool `poetry` which can be installed as follows. **Linux, MacOS,
```

