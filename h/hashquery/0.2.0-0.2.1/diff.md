# Comparing `tmp/hashquery-0.2.0.tar.gz` & `tmp/hashquery-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashquery-0.2.0.tar", last modified: Mon Apr  1 19:47:15 2024, max compression
+gzip compressed data, was "hashquery-0.2.1.tar", last modified: Fri Apr  5 21:39:06 2024, max compression
```

## Comparing `hashquery-0.2.0.tar` & `hashquery-0.2.1.tar`

### file list

```diff
@@ -1,131 +1,132 @@
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.637184 hashquery-0.2.0/
--rw-r--r--   0 charlie    (501) staff       (20)        7 2024-03-08 01:32:07.000000 hashquery-0.2.0/.gitignore
--rw-r--r--   0 charlie    (501) staff       (20)    11357 2024-03-08 01:32:07.000000 hashquery-0.2.0/LICENSE
--rw-r--r--   0 charlie    (501) staff       (20)      387 2024-03-08 01:32:07.000000 hashquery-0.2.0/Makefile
--rw-r--r--   0 charlie    (501) staff       (20)      266 2024-04-01 19:47:15.636942 hashquery-0.2.0/PKG-INFO
--rw-r--r--   0 charlie    (501) staff       (20)     1970 2024-03-08 01:32:07.000000 hashquery-0.2.0/README.md
--rw-r--r--   0 charlie    (501) staff       (20)     4209 2024-03-20 15:23:35.000000 hashquery-0.2.0/README_external.md
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.625507 hashquery-0.2.0/docs/
--rw-r--r--   0 charlie    (501) staff       (20)        8 2024-03-08 01:32:07.000000 hashquery-0.2.0/docs/.gitignore
--rw-r--r--   0 charlie    (501) staff       (20)      138 2024-03-08 01:32:07.000000 hashquery-0.2.0/docs/Makefile
--rw-r--r--   0 charlie    (501) staff       (20)      488 2024-03-08 01:32:07.000000 hashquery-0.2.0/docs/README.md
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.625738 hashquery-0.2.0/docs/_fragments/
--rw-r--r--   0 charlie    (501) staff       (20)      646 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/_fragments/alpha_notice.md
--rw-r--r--   0 charlie    (501) staff       (20)      381 2024-03-20 15:23:35.000000 hashquery-0.2.0/docs/_fragments/quickstart_smoke_test.md
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.625851 hashquery-0.2.0/docs/_static/
--rw-r--r--   0 charlie    (501) staff       (20)        0 2024-03-08 01:32:07.000000 hashquery-0.2.0/docs/_static/.gitkeep
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.625951 hashquery-0.2.0/docs/_static/css/
--rw-r--r--   0 charlie    (501) staff       (20)     3849 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/_static/css/overrides.css
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.626420 hashquery-0.2.0/docs/_static/js/
--rw-r--r--   0 charlie    (501) staff       (20)     2678 2024-03-20 15:23:35.000000 hashquery-0.2.0/docs/_static/js/analytics.js
--rw-r--r--   0 charlie    (501) staff       (20)   161921 2024-03-08 01:32:07.000000 hashquery-0.2.0/docs/_static/js/jquery.js
--rw-r--r--   0 charlie    (501) staff       (20)      396 2024-03-18 18:49:18.000000 hashquery-0.2.0/docs/_static/js/markup.js
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.627019 hashquery-0.2.0/docs/api_reference/
--rw-r--r--   0 charlie    (501) staff       (20)      340 2024-03-14 15:01:43.000000 hashquery-0.2.0/docs/api_reference/0_model.md
--rw-r--r--   0 charlie    (501) staff       (20)      223 2024-03-14 15:01:43.000000 hashquery-0.2.0/docs/api_reference/1_column_expression.md
--rw-r--r--   0 charlie    (501) staff       (20)      373 2024-03-14 15:01:43.000000 hashquery-0.2.0/docs/api_reference/2_func.md
--rw-r--r--   0 charlie    (501) staff       (20)      219 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/api_reference/3_project.md
--rw-r--r--   0 charlie    (501) staff       (20)      721 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/api_reference/4_keypath.md
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.627389 hashquery-0.2.0/docs/concept_explanations/
--rw-r--r--   0 charlie    (501) staff       (20)     1044 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/concept_explanations/0_models.md
--rw-r--r--   0 charlie    (501) staff       (20)      143 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/concept_explanations/1_column_expressions.md
--rw-r--r--   0 charlie    (501) staff       (20)     6971 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/concept_explanations/z_advanced_keypaths.md
--rw-r--r--   0 charlie    (501) staff       (20)     2328 2024-03-20 15:23:35.000000 hashquery-0.2.0/docs/conf.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.627626 hashquery-0.2.0/docs/hashboard_intg/
--rw-r--r--   0 charlie    (501) staff       (20)     2057 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/hashboard_intg/0_import.md
--rw-r--r--   0 charlie    (501) staff       (20)      234 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/hashboard_intg/dataops.md
--rw-r--r--   0 charlie    (501) staff       (20)     1302 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/index.md
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.628276 hashquery-0.2.0/docs/pattern_guides/
--rw-r--r--   0 charlie    (501) staff       (20)     1135 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/pattern_guides/binning.md
--rw-r--r--   0 charlie    (501) staff       (20)     7039 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/pattern_guides/events.md
--rw-r--r--   0 charlie    (501) staff       (20)     1202 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/pattern_guides/joins.md
--rw-r--r--   0 charlie    (501) staff       (20)     1257 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/pattern_guides/segments.md
--rw-r--r--   0 charlie    (501) staff       (20)     1356 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/pattern_guides/timeframes.md
--rw-r--r--   0 charlie    (501) staff       (20)      748 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/pattern_guides/visualizations.md
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.628492 hashquery-0.2.0/docs/project_info/
--rw-r--r--   0 charlie    (501) staff       (20)       21 2024-03-18 17:09:06.000000 hashquery-0.2.0/docs/project_info/feedback.md
--rw-r--r--   0 charlie    (501) staff       (20)      609 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/project_info/roadmap.md
--rw-r--r--   0 charlie    (501) staff       (20)       67 2024-03-08 01:32:07.000000 hashquery-0.2.0/docs/requirements.txt
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.629151 hashquery-0.2.0/docs/setup_tutorial/
--rw-r--r--   0 charlie    (501) staff       (20)     2905 2024-03-20 15:23:35.000000 hashquery-0.2.0/docs/setup_tutorial/1_quickstart.md
--rw-r--r--   0 charlie    (501) staff       (20)     4519 2024-03-20 15:23:35.000000 hashquery-0.2.0/docs/setup_tutorial/2_first_analysis.md
--rw-r--r--   0 charlie    (501) staff       (20)     1813 2024-03-21 17:47:59.000000 hashquery-0.2.0/docs/setup_tutorial/3_authentication.md
--rw-r--r--   0 charlie    (501) staff       (20)      284 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/setup_tutorial/first_analysis_0.py
--rw-r--r--   0 charlie    (501) staff       (20)      377 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/setup_tutorial/first_analysis_1.py
--rw-r--r--   0 charlie    (501) staff       (20)      508 2024-03-19 21:35:44.000000 hashquery-0.2.0/docs/setup_tutorial/first_analysis_2.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.636642 hashquery-0.2.0/hashquery.egg-info/
--rw-r--r--   0 charlie    (501) staff       (20)      266 2024-04-01 19:47:15.000000 hashquery-0.2.0/hashquery.egg-info/PKG-INFO
--rw-r--r--   0 charlie    (501) staff       (20)     3065 2024-04-01 19:47:15.000000 hashquery-0.2.0/hashquery.egg-info/SOURCES.txt
--rw-r--r--   0 charlie    (501) staff       (20)        1 2024-04-01 19:47:15.000000 hashquery-0.2.0/hashquery.egg-info/dependency_links.txt
--rw-r--r--   0 charlie    (501) staff       (20)       42 2024-04-01 19:47:15.000000 hashquery-0.2.0/hashquery.egg-info/requires.txt
--rw-r--r--   0 charlie    (501) staff       (20)       10 2024-04-01 19:47:15.000000 hashquery-0.2.0/hashquery.egg-info/top_level.txt
--rw-r--r--   0 charlie    (501) staff       (20)      400 2024-04-01 19:46:34.000000 hashquery-0.2.0/pyproject.toml
--rw-r--r--   0 charlie    (501) staff       (20)       38 2024-04-01 19:47:15.637226 hashquery-0.2.0/setup.cfg
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.629760 hashquery-0.2.0/src/
--rw-r--r--   0 charlie    (501) staff       (20)      300 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/__init__.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.629975 hashquery-0.2.0/src/demo/
--rw-r--r--   0 charlie    (501) staff       (20)       62 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/demo/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)      861 2024-03-19 21:35:44.000000 hashquery-0.2.0/src/demo/project.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.630442 hashquery-0.2.0/src/func/
--rw-r--r--   0 charlie    (501) staff       (20)      489 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/func/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)     1232 2024-03-14 15:01:43.000000 hashquery-0.2.0/src/func/_cases.py
--rw-r--r--   0 charlie    (501) staff       (20)      702 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/func/_logical.py
--rw-r--r--   0 charlie    (501) staff       (20)     2121 2024-03-14 15:01:43.000000 hashquery-0.2.0/src/func/_sql_functions.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.631121 hashquery-0.2.0/src/hashboard_api/
--rw-r--r--   0 charlie    (501) staff       (20)        0 2024-03-08 01:32:07.000000 hashquery-0.2.0/src/hashboard_api/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)     1905 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/hashboard_api/api.py
--rw-r--r--   0 charlie    (501) staff       (20)     4659 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/hashboard_api/credentials.py
--rw-r--r--   0 charlie    (501) staff       (20)     1214 2024-03-19 21:35:44.000000 hashquery-0.2.0/src/hashboard_api/default_project.py
--rw-r--r--   0 charlie    (501) staff       (20)     2074 2024-03-19 21:35:44.000000 hashquery-0.2.0/src/hashboard_api/project_importer.py
--rw-r--r--   0 charlie    (501) staff       (20)     6334 2024-03-19 21:35:44.000000 hashquery-0.2.0/src/hashboard_api/project_manifest.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.631979 hashquery-0.2.0/src/model/
--rw-r--r--   0 charlie    (501) staff       (20)        0 2024-03-08 01:32:07.000000 hashquery-0.2.0/src/model/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)      945 2024-03-27 19:20:01.000000 hashquery-0.2.0/src/model/accessors.py
--rw-r--r--   0 charlie    (501) staff       (20)     1283 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/model/activity_schema.py
--rw-r--r--   0 charlie    (501) staff       (20)     2355 2024-04-01 19:00:43.000000 hashquery-0.2.0/src/model/column.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.633210 hashquery-0.2.0/src/model/column_expression/
--rw-r--r--   0 charlie    (501) staff       (20)      446 2024-03-27 21:43:29.000000 hashquery-0.2.0/src/model/column_expression/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)     1562 2024-04-01 19:00:43.000000 hashquery-0.2.0/src/model/column_expression/binary_op.py
--rw-r--r--   0 charlie    (501) staff       (20)     1698 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/model/column_expression/cases.py
--rw-r--r--   0 charlie    (501) staff       (20)    19869 2024-04-01 19:00:43.000000 hashquery-0.2.0/src/model/column_expression/column_expression.py
--rw-r--r--   0 charlie    (501) staff       (20)     1467 2024-03-14 15:01:43.000000 hashquery-0.2.0/src/model/column_expression/column_name.py
--rw-r--r--   0 charlie    (501) staff       (20)     1240 2024-03-08 01:32:07.000000 hashquery-0.2.0/src/model/column_expression/granularity.py
--rw-r--r--   0 charlie    (501) staff       (20)     1287 2024-03-14 15:01:43.000000 hashquery-0.2.0/src/model/column_expression/py_value.py
--rw-r--r--   0 charlie    (501) staff       (20)     2698 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/model/column_expression/sql_function.py
--rw-r--r--   0 charlie    (501) staff       (20)     4294 2024-04-01 19:00:43.000000 hashquery-0.2.0/src/model/column_expression/sql_text.py
--rw-r--r--   0 charlie    (501) staff       (20)     1139 2024-03-27 21:43:29.000000 hashquery-0.2.0/src/model/column_expression/subquery_expression.py
--rw-r--r--   0 charlie    (501) staff       (20)      181 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/model/data_connection.py
--rw-r--r--   0 charlie    (501) staff       (20)    30027 2024-04-01 19:00:43.000000 hashquery-0.2.0/src/model/model.py
--rw-r--r--   0 charlie    (501) staff       (20)     2184 2024-03-27 19:19:55.000000 hashquery-0.2.0/src/model/namespace.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.634611 hashquery-0.2.0/src/model/source/
--rw-r--r--   0 charlie    (501) staff       (20)      374 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/model/source/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)     1406 2024-03-08 02:35:55.000000 hashquery-0.2.0/src/model/source/aggregate.py
--rw-r--r--   0 charlie    (501) staff       (20)      957 2024-03-08 02:35:55.000000 hashquery-0.2.0/src/model/source/filter.py
--rw-r--r--   0 charlie    (501) staff       (20)     1523 2024-03-14 15:01:43.000000 hashquery-0.2.0/src/model/source/join_one.py
--rw-r--r--   0 charlie    (501) staff       (20)      953 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/model/source/limit.py
--rw-r--r--   0 charlie    (501) staff       (20)     1111 2024-03-14 15:01:43.000000 hashquery-0.2.0/src/model/source/match_steps.py
--rw-r--r--   0 charlie    (501) staff       (20)      988 2024-03-08 02:35:55.000000 hashquery-0.2.0/src/model/source/pick.py
--rw-r--r--   0 charlie    (501) staff       (20)     1181 2024-03-19 21:35:44.000000 hashquery-0.2.0/src/model/source/sort.py
--rw-r--r--   0 charlie    (501) staff       (20)     1371 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/model/source/source.py
--rw-r--r--   0 charlie    (501) staff       (20)      709 2024-03-08 01:32:07.000000 hashquery-0.2.0/src/model/source/sql_text.py
--rw-r--r--   0 charlie    (501) staff       (20)     1032 2024-03-14 15:01:43.000000 hashquery-0.2.0/src/model/source/table_name.py
--rw-r--r--   0 charlie    (501) staff       (20)      903 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/model/source/union.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.634937 hashquery-0.2.0/src/run/
--rw-r--r--   0 charlie    (501) staff       (20)        0 2024-03-08 01:32:07.000000 hashquery-0.2.0/src/run/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)     1894 2024-03-19 21:35:44.000000 hashquery-0.2.0/src/run/post_run_endpoint.py
--rw-r--r--   0 charlie    (501) staff       (20)     4034 2024-03-19 21:35:44.000000 hashquery-0.2.0/src/run/run_results.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.635866 hashquery-0.2.0/src/utils/
--rw-r--r--   0 charlie    (501) staff       (20)        0 2024-03-08 01:32:07.000000 hashquery-0.2.0/src/utils/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)      720 2024-03-27 20:58:55.000000 hashquery-0.2.0/src/utils/builder.py
--rw-r--r--   0 charlie    (501) staff       (20)      872 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/utils/env.py
--rw-r--r--   0 charlie    (501) staff       (20)     2062 2024-03-14 15:01:43.000000 hashquery-0.2.0/src/utils/identifiable.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-01 19:47:15.636484 hashquery-0.2.0/src/utils/keypath/
--rw-r--r--   0 charlie    (501) staff       (20)      644 2024-03-21 15:14:14.000000 hashquery-0.2.0/src/utils/keypath/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)     8520 2024-03-21 15:14:14.000000 hashquery-0.2.0/src/utils/keypath/keypath.py
--rw-r--r--   0 charlie    (501) staff       (20)      443 2024-03-14 15:01:43.000000 hashquery-0.2.0/src/utils/keypath/keypath_ctx.py
--rw-r--r--   0 charlie    (501) staff       (20)     6705 2024-04-01 19:28:53.000000 hashquery-0.2.0/src/utils/keypath/resolve.py
--rw-r--r--   0 charlie    (501) staff       (20)      746 2024-03-08 01:32:07.000000 hashquery-0.2.0/src/utils/keypath/unwrap.py
--rw-r--r--   0 charlie    (501) staff       (20)      744 2024-03-18 21:55:46.000000 hashquery-0.2.0/src/utils/resource.py
--rw-r--r--   0 charlie    (501) staff       (20)     4809 2024-04-01 19:00:43.000000 hashquery-0.2.0/src/utils/serializable.py
--rw-r--r--   0 charlie    (501) staff       (20)      662 2024-03-27 16:32:34.000000 hashquery-0.2.0/src/utils/timeinterval.py
--rw-r--r--   0 charlie    (501) staff       (20)      106 2024-03-27 21:43:29.000000 hashquery-0.2.0/src/utils/types.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-05 21:39:06.318353 hashquery-0.2.1/
+-rw-r--r--   0 charlie    (501) staff       (20)        7 2024-03-08 01:32:07.000000 hashquery-0.2.1/.gitignore
+-rw-r--r--   0 charlie    (501) staff       (20)    11357 2024-03-08 01:32:07.000000 hashquery-0.2.1/LICENSE
+-rw-r--r--   0 charlie    (501) staff       (20)      387 2024-03-08 01:32:07.000000 hashquery-0.2.1/Makefile
+-rw-r--r--   0 charlie    (501) staff       (20)      266 2024-04-05 21:39:06.318102 hashquery-0.2.1/PKG-INFO
+-rw-r--r--   0 charlie    (501) staff       (20)     1970 2024-03-08 01:32:07.000000 hashquery-0.2.1/README.md
+-rw-r--r--   0 charlie    (501) staff       (20)     4209 2024-03-20 15:23:35.000000 hashquery-0.2.1/README_external.md
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-05 21:39:06.304301 hashquery-0.2.1/docs/
+-rw-r--r--   0 charlie    (501) staff       (20)        8 2024-03-08 01:32:07.000000 hashquery-0.2.1/docs/.gitignore
+-rw-r--r--   0 charlie    (501) staff       (20)      138 2024-03-08 01:32:07.000000 hashquery-0.2.1/docs/Makefile
+-rw-r--r--   0 charlie    (501) staff       (20)      488 2024-03-08 01:32:07.000000 hashquery-0.2.1/docs/README.md
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-05 21:39:06.304540 hashquery-0.2.1/docs/_fragments/
+-rw-r--r--   0 charlie    (501) staff       (20)      646 2024-03-19 21:35:44.000000 hashquery-0.2.1/docs/_fragments/alpha_notice.md
+-rw-r--r--   0 charlie    (501) staff       (20)      381 2024-03-20 15:23:35.000000 hashquery-0.2.1/docs/_fragments/quickstart_smoke_test.md
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-05 21:39:06.304670 hashquery-0.2.1/docs/_static/
+-rw-r--r--   0 charlie    (501) staff       (20)        0 2024-03-08 01:32:07.000000 hashquery-0.2.1/docs/_static/.gitkeep
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-05 21:39:06.304783 hashquery-0.2.1/docs/_static/css/
+-rw-r--r--   0 charlie    (501) staff       (20)     3849 2024-03-19 21:35:44.000000 hashquery-0.2.1/docs/_static/css/overrides.css
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-05 21:39:06.305338 hashquery-0.2.1/docs/_static/js/
+-rw-r--r--   0 charlie    (501) staff       (20)     2678 2024-03-20 15:23:35.000000 hashquery-0.2.1/docs/_static/js/analytics.js
+-rw-r--r--   0 charlie    (501) staff       (20)   161921 2024-03-08 01:32:07.000000 hashquery-0.2.1/docs/_static/js/jquery.js
+-rw-r--r--   0 charlie    (501) staff       (20)      396 2024-03-18 18:49:18.000000 hashquery-0.2.1/docs/_static/js/markup.js
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-05 21:39:06.306507 hashquery-0.2.1/docs/api_reference/
+-rw-r--r--   0 charlie    (501) staff       (20)      340 2024-03-14 15:01:43.000000 hashquery-0.2.1/docs/api_reference/0_model.md
+-rw-r--r--   0 charlie    (501) staff       (20)      223 2024-03-14 15:01:43.000000 hashquery-0.2.1/docs/api_reference/1_column_expression.md
+-rw-r--r--   0 charlie    (501) staff       (20)      373 2024-03-14 15:01:43.000000 hashquery-0.2.1/docs/api_reference/2_func.md
+-rw-r--r--   0 charlie    (501) staff       (20)      219 2024-03-19 21:35:44.000000 hashquery-0.2.1/docs/api_reference/3_project.md
+-rw-r--r--   0 charlie    (501) staff       (20)      721 2024-03-19 21:35:44.000000 hashquery-0.2.1/docs/api_reference/4_keypath.md
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-05 21:39:06.306889 hashquery-0.2.1/docs/concept_explanations/
+-rw-r--r--   0 charlie    (501) staff       (20)     1044 2024-03-19 21:35:44.000000 hashquery-0.2.1/docs/concept_explanations/0_models.md
+-rw-r--r--   0 charlie    (501) staff       (20)      143 2024-03-19 21:35:44.000000 hashquery-0.2.1/docs/concept_explanations/1_column_expressions.md
+-rw-r--r--   0 charlie    (501) staff       (20)     6971 2024-03-19 21:35:44.000000 hashquery-0.2.1/docs/concept_explanations/z_advanced_keypaths.md
+-rw-r--r--   0 charlie    (501) staff       (20)     2328 2024-03-20 15:23:35.000000 hashquery-0.2.1/docs/conf.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-05 21:39:06.307163 hashquery-0.2.1/docs/hashboard_intg/
+-rw-r--r--   0 charlie    (501) staff       (20)     2057 2024-03-19 21:35:44.000000 hashquery-0.2.1/docs/hashboard_intg/0_import.md
+-rw-r--r--   0 charlie    (501) staff       (20)      234 2024-03-19 21:35:44.000000 hashquery-0.2.1/docs/hashboard_intg/dataops.md
+-rw-r--r--   0 charlie    (501) staff       (20)     1302 2024-03-19 21:35:44.000000 hashquery-0.2.1/docs/index.md
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-05 21:39:06.307927 hashquery-0.2.1/docs/pattern_guides/
+-rw-r--r--   0 charlie    (501) staff       (20)     1135 2024-03-19 21:35:44.000000 hashquery-0.2.1/docs/pattern_guides/binning.md
+-rw-r--r--   0 charlie    (501) staff       (20)     7039 2024-03-19 21:35:44.000000 hashquery-0.2.1/docs/pattern_guides/events.md
+-rw-r--r--   0 charlie    (501) staff       (20)     1202 2024-03-19 21:35:44.000000 hashquery-0.2.1/docs/pattern_guides/joins.md
+-rw-r--r--   0 charlie    (501) staff       (20)     1257 2024-03-19 21:35:44.000000 hashquery-0.2.1/docs/pattern_guides/segments.md
+-rw-r--r--   0 charlie    (501) staff       (20)     1356 2024-03-19 21:35:44.000000 hashquery-0.2.1/docs/pattern_guides/timeframes.md
+-rw-r--r--   0 charlie    (501) staff       (20)      748 2024-03-19 21:35:44.000000 hashquery-0.2.1/docs/pattern_guides/visualizations.md
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-05 21:39:06.308161 hashquery-0.2.1/docs/project_info/
+-rw-r--r--   0 charlie    (501) staff       (20)       21 2024-03-18 17:09:06.000000 hashquery-0.2.1/docs/project_info/feedback.md
+-rw-r--r--   0 charlie    (501) staff       (20)      609 2024-03-19 21:35:44.000000 hashquery-0.2.1/docs/project_info/roadmap.md
+-rw-r--r--   0 charlie    (501) staff       (20)       67 2024-03-08 01:32:07.000000 hashquery-0.2.1/docs/requirements.txt
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-05 21:39:06.308910 hashquery-0.2.1/docs/setup_tutorial/
+-rw-r--r--   0 charlie    (501) staff       (20)     2905 2024-03-20 15:23:35.000000 hashquery-0.2.1/docs/setup_tutorial/1_quickstart.md
+-rw-r--r--   0 charlie    (501) staff       (20)     4519 2024-03-20 15:23:35.000000 hashquery-0.2.1/docs/setup_tutorial/2_first_analysis.md
+-rw-r--r--   0 charlie    (501) staff       (20)     1813 2024-03-21 17:47:59.000000 hashquery-0.2.1/docs/setup_tutorial/3_authentication.md
+-rw-r--r--   0 charlie    (501) staff       (20)      284 2024-03-19 21:35:44.000000 hashquery-0.2.1/docs/setup_tutorial/first_analysis_0.py
+-rw-r--r--   0 charlie    (501) staff       (20)      377 2024-03-19 21:35:44.000000 hashquery-0.2.1/docs/setup_tutorial/first_analysis_1.py
+-rw-r--r--   0 charlie    (501) staff       (20)      508 2024-03-19 21:35:44.000000 hashquery-0.2.1/docs/setup_tutorial/first_analysis_2.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-05 21:39:06.317770 hashquery-0.2.1/hashquery.egg-info/
+-rw-r--r--   0 charlie    (501) staff       (20)      266 2024-04-05 21:39:06.000000 hashquery-0.2.1/hashquery.egg-info/PKG-INFO
+-rw-r--r--   0 charlie    (501) staff       (20)     3086 2024-04-05 21:39:06.000000 hashquery-0.2.1/hashquery.egg-info/SOURCES.txt
+-rw-r--r--   0 charlie    (501) staff       (20)        1 2024-04-05 21:39:06.000000 hashquery-0.2.1/hashquery.egg-info/dependency_links.txt
+-rw-r--r--   0 charlie    (501) staff       (20)       42 2024-04-05 21:39:06.000000 hashquery-0.2.1/hashquery.egg-info/requires.txt
+-rw-r--r--   0 charlie    (501) staff       (20)       10 2024-04-05 21:39:06.000000 hashquery-0.2.1/hashquery.egg-info/top_level.txt
+-rw-r--r--   0 charlie    (501) staff       (20)      400 2024-04-03 20:18:41.000000 hashquery-0.2.1/pyproject.toml
+-rw-r--r--   0 charlie    (501) staff       (20)       38 2024-04-05 21:39:06.318406 hashquery-0.2.1/setup.cfg
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-05 21:39:06.310046 hashquery-0.2.1/src/
+-rw-r--r--   0 charlie    (501) staff       (20)      435 2024-04-03 20:18:41.000000 hashquery-0.2.1/src/__init__.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-05 21:39:06.310272 hashquery-0.2.1/src/demo/
+-rw-r--r--   0 charlie    (501) staff       (20)       62 2024-03-18 21:55:46.000000 hashquery-0.2.1/src/demo/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)      861 2024-03-19 21:35:44.000000 hashquery-0.2.1/src/demo/project.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-05 21:39:06.310726 hashquery-0.2.1/src/func/
+-rw-r--r--   0 charlie    (501) staff       (20)      489 2024-03-18 21:55:46.000000 hashquery-0.2.1/src/func/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1232 2024-03-14 15:01:43.000000 hashquery-0.2.1/src/func/_cases.py
+-rw-r--r--   0 charlie    (501) staff       (20)      702 2024-03-18 21:55:46.000000 hashquery-0.2.1/src/func/_logical.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2121 2024-03-14 15:01:43.000000 hashquery-0.2.1/src/func/_sql_functions.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-05 21:39:06.311433 hashquery-0.2.1/src/hashboard_api/
+-rw-r--r--   0 charlie    (501) staff       (20)        0 2024-03-08 01:32:07.000000 hashquery-0.2.1/src/hashboard_api/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1905 2024-03-18 21:55:46.000000 hashquery-0.2.1/src/hashboard_api/api.py
+-rw-r--r--   0 charlie    (501) staff       (20)     4999 2024-04-03 20:18:41.000000 hashquery-0.2.1/src/hashboard_api/credentials.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1214 2024-03-19 21:35:44.000000 hashquery-0.2.1/src/hashboard_api/default_project.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2074 2024-03-19 21:35:44.000000 hashquery-0.2.1/src/hashboard_api/project_importer.py
+-rw-r--r--   0 charlie    (501) staff       (20)     6334 2024-03-19 21:35:44.000000 hashquery-0.2.1/src/hashboard_api/project_manifest.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-05 21:39:06.312383 hashquery-0.2.1/src/model/
+-rw-r--r--   0 charlie    (501) staff       (20)        0 2024-03-08 01:32:07.000000 hashquery-0.2.1/src/model/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)      945 2024-03-27 19:20:01.000000 hashquery-0.2.1/src/model/accessors.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1283 2024-03-18 21:55:46.000000 hashquery-0.2.1/src/model/activity_schema.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2355 2024-04-01 19:00:43.000000 hashquery-0.2.1/src/model/column.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-05 21:39:06.313593 hashquery-0.2.1/src/model/column_expression/
+-rw-r--r--   0 charlie    (501) staff       (20)      446 2024-03-27 21:43:29.000000 hashquery-0.2.1/src/model/column_expression/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1562 2024-04-01 19:00:43.000000 hashquery-0.2.1/src/model/column_expression/binary_op.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1698 2024-03-18 21:55:46.000000 hashquery-0.2.1/src/model/column_expression/cases.py
+-rw-r--r--   0 charlie    (501) staff       (20)    19869 2024-04-01 19:00:43.000000 hashquery-0.2.1/src/model/column_expression/column_expression.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1467 2024-03-14 15:01:43.000000 hashquery-0.2.1/src/model/column_expression/column_name.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1240 2024-03-08 01:32:07.000000 hashquery-0.2.1/src/model/column_expression/granularity.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1287 2024-03-14 15:01:43.000000 hashquery-0.2.1/src/model/column_expression/py_value.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2698 2024-03-18 21:55:46.000000 hashquery-0.2.1/src/model/column_expression/sql_function.py
+-rw-r--r--   0 charlie    (501) staff       (20)     5542 2024-04-03 20:18:41.000000 hashquery-0.2.1/src/model/column_expression/sql_text.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1139 2024-03-27 21:43:29.000000 hashquery-0.2.1/src/model/column_expression/subquery_expression.py
+-rw-r--r--   0 charlie    (501) staff       (20)      181 2024-03-18 21:55:46.000000 hashquery-0.2.1/src/model/data_connection.py
+-rw-r--r--   0 charlie    (501) staff       (20)    30027 2024-04-01 21:50:05.000000 hashquery-0.2.1/src/model/model.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2184 2024-03-27 19:19:55.000000 hashquery-0.2.1/src/model/namespace.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-05 21:39:06.315263 hashquery-0.2.1/src/model/source/
+-rw-r--r--   0 charlie    (501) staff       (20)      374 2024-03-18 21:55:46.000000 hashquery-0.2.1/src/model/source/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1406 2024-03-08 02:35:55.000000 hashquery-0.2.1/src/model/source/aggregate.py
+-rw-r--r--   0 charlie    (501) staff       (20)      957 2024-03-08 02:35:55.000000 hashquery-0.2.1/src/model/source/filter.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1523 2024-03-14 15:01:43.000000 hashquery-0.2.1/src/model/source/join_one.py
+-rw-r--r--   0 charlie    (501) staff       (20)      953 2024-03-18 21:55:46.000000 hashquery-0.2.1/src/model/source/limit.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1111 2024-03-14 15:01:43.000000 hashquery-0.2.1/src/model/source/match_steps.py
+-rw-r--r--   0 charlie    (501) staff       (20)      988 2024-03-08 02:35:55.000000 hashquery-0.2.1/src/model/source/pick.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1181 2024-03-19 21:35:44.000000 hashquery-0.2.1/src/model/source/sort.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1371 2024-03-18 21:55:46.000000 hashquery-0.2.1/src/model/source/source.py
+-rw-r--r--   0 charlie    (501) staff       (20)      709 2024-03-08 01:32:07.000000 hashquery-0.2.1/src/model/source/sql_text.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1032 2024-03-14 15:01:43.000000 hashquery-0.2.1/src/model/source/table_name.py
+-rw-r--r--   0 charlie    (501) staff       (20)      903 2024-03-18 21:55:46.000000 hashquery-0.2.1/src/model/source/union.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-05 21:39:06.315579 hashquery-0.2.1/src/run/
+-rw-r--r--   0 charlie    (501) staff       (20)        0 2024-03-08 01:32:07.000000 hashquery-0.2.1/src/run/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1894 2024-03-19 21:35:44.000000 hashquery-0.2.1/src/run/post_run_endpoint.py
+-rw-r--r--   0 charlie    (501) staff       (20)     4034 2024-03-19 21:35:44.000000 hashquery-0.2.1/src/run/run_results.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-05 21:39:06.316630 hashquery-0.2.1/src/utils/
+-rw-r--r--   0 charlie    (501) staff       (20)        0 2024-03-08 01:32:07.000000 hashquery-0.2.1/src/utils/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)      720 2024-03-27 20:58:55.000000 hashquery-0.2.1/src/utils/builder.py
+-rw-r--r--   0 charlie    (501) staff       (20)      872 2024-03-18 21:55:46.000000 hashquery-0.2.1/src/utils/env.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2062 2024-03-14 15:01:43.000000 hashquery-0.2.1/src/utils/identifiable.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-04-05 21:39:06.317576 hashquery-0.2.1/src/utils/keypath/
+-rw-r--r--   0 charlie    (501) staff       (20)      644 2024-03-21 15:14:14.000000 hashquery-0.2.1/src/utils/keypath/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)     8520 2024-03-21 15:14:14.000000 hashquery-0.2.1/src/utils/keypath/keypath.py
+-rw-r--r--   0 charlie    (501) staff       (20)      443 2024-03-14 15:01:43.000000 hashquery-0.2.1/src/utils/keypath/keypath_ctx.py
+-rw-r--r--   0 charlie    (501) staff       (20)     6705 2024-04-03 17:10:43.000000 hashquery-0.2.1/src/utils/keypath/resolve.py
+-rw-r--r--   0 charlie    (501) staff       (20)      746 2024-03-08 01:32:07.000000 hashquery-0.2.1/src/utils/keypath/unwrap.py
+-rw-r--r--   0 charlie    (501) staff       (20)      744 2024-03-18 21:55:46.000000 hashquery-0.2.1/src/utils/resource.py
+-rw-r--r--   0 charlie    (501) staff       (20)     4809 2024-04-01 19:00:43.000000 hashquery-0.2.1/src/utils/serializable.py
+-rw-r--r--   0 charlie    (501) staff       (20)      662 2024-03-27 16:32:34.000000 hashquery-0.2.1/src/utils/timeinterval.py
+-rw-r--r--   0 charlie    (501) staff       (20)      106 2024-03-27 21:43:29.000000 hashquery-0.2.1/src/utils/types.py
+-rw-r--r--   0 charlie    (501) staff       (20)      211 2024-04-03 20:18:41.000000 hashquery-0.2.1/src/utils/version.py
```

### Comparing `hashquery-0.2.0/LICENSE` & `hashquery-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/README.md` & `hashquery-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/README_external.md` & `hashquery-0.2.1/README_external.md`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/docs/_fragments/alpha_notice.md` & `hashquery-0.2.1/docs/_fragments/alpha_notice.md`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/docs/_static/css/overrides.css` & `hashquery-0.2.1/docs/_static/css/overrides.css`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/docs/_static/js/analytics.js` & `hashquery-0.2.1/docs/_static/js/analytics.js`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/docs/_static/js/jquery.js` & `hashquery-0.2.1/docs/_static/js/jquery.js`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/docs/api_reference/4_keypath.md` & `hashquery-0.2.1/docs/api_reference/4_keypath.md`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/docs/concept_explanations/0_models.md` & `hashquery-0.2.1/docs/concept_explanations/0_models.md`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/docs/concept_explanations/z_advanced_keypaths.md` & `hashquery-0.2.1/docs/concept_explanations/z_advanced_keypaths.md`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/docs/conf.py` & `hashquery-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/docs/hashboard_intg/0_import.md` & `hashquery-0.2.1/docs/hashboard_intg/0_import.md`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/docs/index.md` & `hashquery-0.2.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/docs/pattern_guides/binning.md` & `hashquery-0.2.1/docs/pattern_guides/binning.md`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/docs/pattern_guides/events.md` & `hashquery-0.2.1/docs/pattern_guides/events.md`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/docs/pattern_guides/joins.md` & `hashquery-0.2.1/docs/pattern_guides/joins.md`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/docs/pattern_guides/segments.md` & `hashquery-0.2.1/docs/pattern_guides/segments.md`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/docs/pattern_guides/timeframes.md` & `hashquery-0.2.1/docs/pattern_guides/timeframes.md`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/docs/pattern_guides/visualizations.md` & `hashquery-0.2.1/docs/pattern_guides/visualizations.md`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/docs/project_info/roadmap.md` & `hashquery-0.2.1/docs/project_info/roadmap.md`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/docs/setup_tutorial/1_quickstart.md` & `hashquery-0.2.1/docs/setup_tutorial/1_quickstart.md`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/docs/setup_tutorial/2_first_analysis.md` & `hashquery-0.2.1/docs/setup_tutorial/2_first_analysis.md`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/docs/setup_tutorial/3_authentication.md` & `hashquery-0.2.1/docs/setup_tutorial/3_authentication.md`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/hashquery.egg-info/SOURCES.txt` & `hashquery-0.2.1/hashquery.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -95,12 +95,13 @@
 src/utils/builder.py
 src/utils/env.py
 src/utils/identifiable.py
 src/utils/resource.py
 src/utils/serializable.py
 src/utils/timeinterval.py
 src/utils/types.py
+src/utils/version.py
 src/utils/keypath/__init__.py
 src/utils/keypath/keypath.py
 src/utils/keypath/keypath_ctx.py
 src/utils/keypath/resolve.py
 src/utils/keypath/unwrap.py
```

### Comparing `hashquery-0.2.0/src/demo/project.py` & `hashquery-0.2.1/src/demo/project.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/func/_cases.py` & `hashquery-0.2.1/src/func/_cases.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/func/_logical.py` & `hashquery-0.2.1/src/func/_logical.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/func/_sql_functions.py` & `hashquery-0.2.1/src/func/_sql_functions.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/hashboard_api/api.py` & `hashquery-0.2.1/src/hashboard_api/api.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/hashboard_api/credentials.py` & `hashquery-0.2.1/src/hashboard_api/credentials.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 import base64
 import json
 import os
+from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
-from typing import Optional, Protocol
+from typing import Optional
 
 from ..utils.env import env_with_fallback
+from ..utils.version import HASHQUERY_VERSION
 
 
-class HashboardClientCredentials(Protocol):
+class HashboardClientCredentials(ABC):
     """
     Generic class for a method for an external client to authorize into
     Hashboard within a project. Use `get_client_credentials` to form
     an instance from the client's current `env`.
     """
 
     project_id: str
 
+    @abstractmethod
     def get_headers(self) -> dict:
-        ...
+        return {
+            "X-GLEAN-UNSAFE-PROJECT-ID": self.project_id,
+            "X-GLEAN-HASHQUERY-VERSION": HASHQUERY_VERSION,
+        }
 
 
 @dataclass
 class HashboardUserJWTClientCredentials(HashboardClientCredentials):
     user_jwt: str
     project_id: str
 
     def get_headers(self) -> dict:
-        return {"X-GLEAN-BASE-JWT": self.user_jwt}
+        return {
+            **super().get_headers(),
+            "X-GLEAN-BASE-JWT": self.user_jwt,
+        }
 
 
 @dataclass
 class HashboardAccessKeyClientCredentials(HashboardClientCredentials):
     project_id: str
     access_key_id: str
     access_key_token: str
@@ -46,15 +55,18 @@
             "access_key_id": self.access_key_id,
             "access_key_token": self.access_key_token,
         }
         payload_bytes = json.dumps(payload).encode()
         self.encoded_key = base64.b64encode(payload_bytes).decode()
 
     def get_headers(self) -> dict:
-        return {"Authorization": self.encoded_key}
+        return {
+            **super().get_headers(),
+            "Authorization": self.encoded_key,
+        }
 
     @classmethod
     def from_encoded_key(cls, key: str) -> "HashboardAccessKeyClientCredentials":
         try:
             decoded = base64.b64decode(key).decode()
             loaded: dict = json.loads(decoded)
             return HashboardAccessKeyClientCredentials(
```

### Comparing `hashquery-0.2.0/src/hashboard_api/default_project.py` & `hashquery-0.2.1/src/hashboard_api/default_project.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/hashboard_api/project_importer.py` & `hashquery-0.2.1/src/hashboard_api/project_importer.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/hashboard_api/project_manifest.py` & `hashquery-0.2.1/src/hashboard_api/project_manifest.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/model/accessors.py` & `hashquery-0.2.1/src/model/accessors.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/model/activity_schema.py` & `hashquery-0.2.1/src/model/activity_schema.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/model/column.py` & `hashquery-0.2.1/src/model/column.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/model/column_expression/binary_op.py` & `hashquery-0.2.1/src/model/column_expression/binary_op.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/model/column_expression/cases.py` & `hashquery-0.2.1/src/model/column_expression/cases.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/model/column_expression/column_expression.py` & `hashquery-0.2.1/src/model/column_expression/column_expression.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/model/column_expression/column_name.py` & `hashquery-0.2.1/src/model/column_expression/column_name.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/model/column_expression/granularity.py` & `hashquery-0.2.1/src/model/column_expression/granularity.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/model/column_expression/py_value.py` & `hashquery-0.2.1/src/model/column_expression/py_value.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/model/column_expression/sql_function.py` & `hashquery-0.2.1/src/model/column_expression/sql_function.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/model/column_expression/sql_text.py` & `hashquery-0.2.1/src/model/column_expression/sql_text.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,66 @@
 from copy import deepcopy
 from typing import *
 import re
 
 from .column_expression import ColumnExpression
+from ..namespace import ModelNamespace
 from ...utils.builder import builder_method
 from ...utils.keypath.keypath import _, KeyPath, BoundKeyPath, KeyPathComponentCall
 
 if TYPE_CHECKING:
     from ..model import Model
-    from ..namespace import ModelNamespace
 
-# Detects matches against the pattern `{{ some_name }}` which can be used
-# to substitute the definition of `some_name` into that string. The first
-# capture group denotes the identifier of the referenced expression.
+
+"""
+Hashquery may lift transformations and expressions into a chain of arbitrarily
+named CTEs or use a SQL fragment in a new context where it needs to be
+disambiguated differently. For example, when selecting a column through a JOINed
+relation, SQL expressions on those columns must be disambiguated with the name of
+the relation, not the source table.
+
+Hashquery must transform some SQL snippets to ensure that your SQL statement
+references these contextual elements correctly. To do so, we provide this special
+identifier. If you disambiguate a column reference with this identifier, it will
+be automatically adjusted to point at the "main" table (be that from a loaded
+table, a chain of CTEs, or a joined relation).
+"""
+SELF_TABLE_ALIAS = "self"
+
+"""
+Detects matches against the pattern `{{ some_name }}` which can be used
+to substitute the definition of `some_name` into that string. The first
+capture group denotes the identifier of the referenced expression.
+"""
 SQL_REFERENCE_SUBSTITUTION_REGEX = re.compile(r"{{\s*([\w\d_\.]+)\s*}}")
 
 
 class SqlTextColumnExpression(ColumnExpression):
-    def __init__(
-        self,
-        sql: str,
-        nested_expressions: Optional[Dict[str, ColumnExpression]] = None,
-    ) -> None:
+    def __init__(self, sql: str) -> None:
         super().__init__()
         self.sql = sql
-        self.nested_expressions = nested_expressions or {}
+        self.namespace_identifier: Optional[str] = None
+        self.nested_expressions: Dict[str, ColumnExpression] = {}
 
     def default_identifier(self) -> str:
-        if self.sql.isidentifier():
-            return self.sql
-        return None
+        tokens = self.sql.split(".")
+        if len(tokens) == 1 and tokens[0].isidentifier():
+            return tokens[1]  # column expression is directly nameable
+        elif len(tokens) == 2 and tokens[1].isidentifier():
+            return tokens[1]  # passthrough a name through a namespace
+        else:
+            return None
 
     @builder_method
     def disambiguated(self, namespace) -> "SqlTextColumnExpression":
+        self.namespace_identifier = (
+            namespace._identifier
+            if isinstance(namespace, ModelNamespace)
+            else namespace
+        )
         self.nested_expressions = {
             id: expr.disambiguated(namespace)
             for id, expr in self.nested_expressions.items()
         }
 
     def __repr__(self) -> str:
         return f'sql("{self.sql}")'
@@ -96,25 +120,25 @@
 
     __TYPE_KEY__ = "sqlText"
 
     def to_wire_format(self) -> dict:
         return {
             **super().to_wire_format(),
             "sql": self.sql,
+            "namespaceIdentifier": self.namespace_identifier,
             "nestedExpressions": {
                 id: expr.to_wire_format()
                 for id, expr in self.nested_expressions.items()
             },
         }
 
     @classmethod
     def from_wire_format(cls, wire: dict) -> "SqlTextColumnExpression":
         assert wire["subType"] == cls.__TYPE_KEY__
-        result = SqlTextColumnExpression(
-            wire["sql"],
-            {
-                id: ColumnExpression.from_wire_format(expr_wire)
-                for id, expr_wire in wire.get("nestedExpressions", {}).items()
-            },
-        )
+        result = SqlTextColumnExpression(wire["sql"])
+        result.namespace_identifier = wire.get("namespaceIdentifier")
+        result.nested_expressions = {
+            id: ColumnExpression.from_wire_format(expr_wire)
+            for id, expr_wire in wire.get("nestedExpressions", {}).items()
+        }
         result._from_wire_format_shared(wire)
         return result
```

### Comparing `hashquery-0.2.0/src/model/column_expression/subquery_expression.py` & `hashquery-0.2.1/src/model/column_expression/subquery_expression.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/model/model.py` & `hashquery-0.2.1/src/model/model.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/model/namespace.py` & `hashquery-0.2.1/src/model/namespace.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/model/source/aggregate.py` & `hashquery-0.2.1/src/model/source/aggregate.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/model/source/filter.py` & `hashquery-0.2.1/src/model/source/filter.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/model/source/join_one.py` & `hashquery-0.2.1/src/model/source/join_one.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/model/source/limit.py` & `hashquery-0.2.1/src/model/source/limit.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/model/source/match_steps.py` & `hashquery-0.2.1/src/model/source/match_steps.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/model/source/pick.py` & `hashquery-0.2.1/src/model/source/pick.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/model/source/sort.py` & `hashquery-0.2.1/src/model/source/sort.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/model/source/source.py` & `hashquery-0.2.1/src/model/source/source.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/model/source/sql_text.py` & `hashquery-0.2.1/src/model/source/sql_text.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/model/source/table_name.py` & `hashquery-0.2.1/src/model/source/table_name.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/model/source/union.py` & `hashquery-0.2.1/src/model/source/union.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/run/post_run_endpoint.py` & `hashquery-0.2.1/src/run/post_run_endpoint.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/run/run_results.py` & `hashquery-0.2.1/src/run/run_results.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/utils/builder.py` & `hashquery-0.2.1/src/utils/builder.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/utils/env.py` & `hashquery-0.2.1/src/utils/env.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/utils/identifiable.py` & `hashquery-0.2.1/src/utils/identifiable.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/utils/keypath/__init__.py` & `hashquery-0.2.1/src/utils/keypath/__init__.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/utils/keypath/keypath.py` & `hashquery-0.2.1/src/utils/keypath/keypath.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/utils/keypath/resolve.py` & `hashquery-0.2.1/src/utils/keypath/resolve.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/utils/keypath/unwrap.py` & `hashquery-0.2.1/src/utils/keypath/unwrap.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/utils/resource.py` & `hashquery-0.2.1/src/utils/resource.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/utils/serializable.py` & `hashquery-0.2.1/src/utils/serializable.py`

 * *Files identical despite different names*

### Comparing `hashquery-0.2.0/src/utils/timeinterval.py` & `hashquery-0.2.1/src/utils/timeinterval.py`

 * *Files identical despite different names*

