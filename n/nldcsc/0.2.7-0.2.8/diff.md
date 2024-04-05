# Comparing `tmp/nldcsc-0.2.7.tar.gz` & `tmp/nldcsc-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nldcsc-0.2.7.tar", last modified: Wed Feb  7 12:22:50 2024, max compression
+gzip compressed data, was "nldcsc-0.2.8.tar", last modified: Wed Feb  7 14:23:47 2024, max compression
```

## Comparing `nldcsc-0.2.7.tar` & `nldcsc-0.2.8.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:50.479915 nldcsc-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-07 12:22:21.000000 nldcsc-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-07 12:22:21.000000 nldcsc-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-02-07 12:22:50.479915 nldcsc-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-02-07 12:22:21.000000 nldcsc-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:50.459915 nldcsc-0.2.7/nldcsc/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:50.463915 nldcsc-0.2.7/nldcsc/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/auth/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/auth/ldap_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:50.463915 nldcsc-0.2.7/nldcsc/datatables/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/datatables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/datatables/server_side_dt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/datatables/server_side_dt_es.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/datatables/server_side_dt_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:50.463915 nldcsc-0.2.7/nldcsc/flask_managers/
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/flask_managers/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/flask_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/flask_managers/flask_app_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:50.463915 nldcsc-0.2.7/nldcsc/flask_midddleware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/flask_midddleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/flask_midddleware/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/flask_midddleware/debug_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/flask_midddleware/middleware_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:50.463915 nldcsc-0.2.7/nldcsc/flask_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/flask_plugins/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/flask_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/flask_plugins/flask_eswrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/flask_plugins/flask_kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/flask_plugins/flask_redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:50.463915 nldcsc-0.2.7/nldcsc/generic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/generic/times.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/generic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:50.463915 nldcsc-0.2.7/nldcsc/http_apis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/http_apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:50.467915 nldcsc-0.2.7/nldcsc/http_apis/base_class/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/http_apis/base_class/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7689 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/http_apis/base_class/api_base_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:50.467915 nldcsc-0.2.7/nldcsc/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/loggers/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/loggers/app_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:50.467915 nldcsc-0.2.7/nldcsc/loggers/formatters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/loggers/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/loggers/formatters/task_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/loggers/gunicorn_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:50.467915 nldcsc-0.2.7/nldcsc/loggers/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/loggers/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/loggers/handlers/gelf_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/loggers/handlers/syslog_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:50.467915 nldcsc-0.2.7/nldcsc/sql_migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/sql_migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-02-07 12:22:21.000000 nldcsc-0.2.7/nldcsc/sql_migrations/flask_sql_migrate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:50.471915 nldcsc-0.2.7/nldcsc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-02-07 12:22:50.000000 nldcsc-0.2.7/nldcsc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-02-07 12:22:50.000000 nldcsc-0.2.7/nldcsc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 12:22:50.000000 nldcsc-0.2.7/nldcsc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-02-07 12:22:50.000000 nldcsc-0.2.7/nldcsc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-07 12:22:50.000000 nldcsc-0.2.7/nldcsc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-07 12:22:21.000000 nldcsc-0.2.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:50.467915 nldcsc-0.2.7/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-07 12:22:21.000000 nldcsc-0.2.7/requirements/default.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:50.467915 nldcsc-0.2.7/requirements/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-07 12:22:21.000000 nldcsc-0.2.7/requirements/modules/auth.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-07 12:22:21.000000 nldcsc-0.2.7/requirements/modules/datatables.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-07 12:22:21.000000 nldcsc-0.2.7/requirements/modules/flask_managers.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 12:22:21.000000 nldcsc-0.2.7/requirements/modules/flask_middleware.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-07 12:22:21.000000 nldcsc-0.2.7/requirements/modules/flask_plugins.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-07 12:22:21.000000 nldcsc-0.2.7/requirements/modules/http_apis.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-07 12:22:21.000000 nldcsc-0.2.7/requirements/modules/loggers.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-07 12:22:21.000000 nldcsc-0.2.7/requirements/modules/sql_migrations.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-07 12:22:21.000000 nldcsc-0.2.7/requirements/test-ci-default.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-07 12:22:21.000000 nldcsc-0.2.7/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 12:22:50.479915 nldcsc-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-02-07 12:22:21.000000 nldcsc-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:50.471915 nldcsc-0.2.7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:50.471915 nldcsc-0.2.7/tests/applications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:21.000000 nldcsc-0.2.7/tests/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-02-07 12:22:21.000000 nldcsc-0.2.7/tests/applications/migrate_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:50.471915 nldcsc-0.2.7/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 12:22:21.000000 nldcsc-0.2.7/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-02-07 12:22:21.000000 nldcsc-0.2.7/tests/helpers/capture_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-02-07 12:22:21.000000 nldcsc-0.2.7/tests/test_flask_app_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-02-07 12:22:21.000000 nldcsc-0.2.7/tests/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6910 2024-02-07 12:22:21.000000 nldcsc-0.2.7/tests/test_http_apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-02-07 12:22:21.000000 nldcsc-0.2.7/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-02-07 12:22:21.000000 nldcsc-0.2.7/tests/test_sqlalchemy_migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:47.922954 nldcsc-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-07 14:23:16.000000 nldcsc-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-07 14:23:16.000000 nldcsc-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-02-07 14:23:47.922954 nldcsc-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-02-07 14:23:16.000000 nldcsc-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:47.902954 nldcsc-0.2.8/nldcsc/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:47.902954 nldcsc-0.2.8/nldcsc/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/auth/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/auth/ldap_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:47.902954 nldcsc-0.2.8/nldcsc/datatables/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/datatables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/datatables/server_side_dt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/datatables/server_side_dt_es.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/datatables/server_side_dt_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:47.906954 nldcsc-0.2.8/nldcsc/flask_managers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/flask_managers/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/flask_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/flask_managers/flask_app_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:47.906954 nldcsc-0.2.8/nldcsc/flask_midddleware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/flask_midddleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/flask_midddleware/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/flask_midddleware/debug_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/flask_midddleware/middleware_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:47.906954 nldcsc-0.2.8/nldcsc/flask_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/flask_plugins/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/flask_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/flask_plugins/flask_eswrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/flask_plugins/flask_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/flask_plugins/flask_redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:47.906954 nldcsc-0.2.8/nldcsc/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/generic/times.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/generic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:47.906954 nldcsc-0.2.8/nldcsc/http_apis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/http_apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:47.906954 nldcsc-0.2.8/nldcsc/http_apis/base_class/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/http_apis/base_class/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7857 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/http_apis/base_class/api_base_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:47.906954 nldcsc-0.2.8/nldcsc/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/loggers/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/loggers/app_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:47.906954 nldcsc-0.2.8/nldcsc/loggers/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/loggers/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/loggers/formatters/task_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/loggers/gunicorn_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:47.910954 nldcsc-0.2.8/nldcsc/loggers/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/loggers/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/loggers/handlers/gelf_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/loggers/handlers/syslog_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:47.910954 nldcsc-0.2.8/nldcsc/sql_migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/sql_migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-02-07 14:23:16.000000 nldcsc-0.2.8/nldcsc/sql_migrations/flask_sql_migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:47.914954 nldcsc-0.2.8/nldcsc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-02-07 14:23:47.000000 nldcsc-0.2.8/nldcsc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-02-07 14:23:47.000000 nldcsc-0.2.8/nldcsc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 14:23:47.000000 nldcsc-0.2.8/nldcsc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-02-07 14:23:47.000000 nldcsc-0.2.8/nldcsc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-07 14:23:47.000000 nldcsc-0.2.8/nldcsc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-07 14:23:16.000000 nldcsc-0.2.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:47.910954 nldcsc-0.2.8/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-07 14:23:16.000000 nldcsc-0.2.8/requirements/default.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:47.910954 nldcsc-0.2.8/requirements/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-07 14:23:16.000000 nldcsc-0.2.8/requirements/modules/auth.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-07 14:23:16.000000 nldcsc-0.2.8/requirements/modules/datatables.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-07 14:23:16.000000 nldcsc-0.2.8/requirements/modules/flask_managers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 14:23:16.000000 nldcsc-0.2.8/requirements/modules/flask_middleware.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-07 14:23:16.000000 nldcsc-0.2.8/requirements/modules/flask_plugins.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-07 14:23:16.000000 nldcsc-0.2.8/requirements/modules/http_apis.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-07 14:23:16.000000 nldcsc-0.2.8/requirements/modules/loggers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-07 14:23:16.000000 nldcsc-0.2.8/requirements/modules/sql_migrations.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-07 14:23:16.000000 nldcsc-0.2.8/requirements/test-ci-default.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-07 14:23:16.000000 nldcsc-0.2.8/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 14:23:47.922954 nldcsc-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-02-07 14:23:16.000000 nldcsc-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:47.910954 nldcsc-0.2.8/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:47.910954 nldcsc-0.2.8/tests/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:16.000000 nldcsc-0.2.8/tests/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-02-07 14:23:16.000000 nldcsc-0.2.8/tests/applications/migrate_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:47.914954 nldcsc-0.2.8/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 14:23:16.000000 nldcsc-0.2.8/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-02-07 14:23:16.000000 nldcsc-0.2.8/tests/helpers/capture_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-02-07 14:23:16.000000 nldcsc-0.2.8/tests/test_flask_app_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-02-07 14:23:16.000000 nldcsc-0.2.8/tests/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-02-07 14:23:16.000000 nldcsc-0.2.8/tests/test_http_apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-02-07 14:23:16.000000 nldcsc-0.2.8/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-02-07 14:23:16.000000 nldcsc-0.2.8/tests/test_sqlalchemy_migrate.py
```

### Comparing `nldcsc-0.2.7/LICENSE` & `nldcsc-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/PKG-INFO` & `nldcsc-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nldcsc
-Version: 0.2.7
+Version: 0.2.8
 Summary: Package with general devops code
 Home-page: https://github.com/NLDCSC/nldcsc
 Author: NLDCSC
 Author-email: NLDCSC@invalid.com
 License: GNU General Public License v3.0
 Project-URL: Code, https://github.com/NLDCSC/nldcsc
 Platform: any
@@ -15,32 +15,29 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools>=68.1.0
-Provides-Extra: flask-plugins
-Requires-Dist: eswrap>=0.5.0; extra == "flask-plugins"
-Requires-Dist: redis>=4.6.0; extra == "flask-plugins"
-Requires-Dist: kafka-python>=2.0.2; extra == "flask-plugins"
-Requires-Dist: elasticsearch>=8.7.0; extra == "flask-plugins"
-Requires-Dist: flask>=2.3.3; extra == "flask-plugins"
-Requires-Dist: SQLAlchemy>=2.0.21; extra == "flask-plugins"
-Requires-Dist: Flask_SQLAlchemy>=3.1.1; extra == "flask-plugins"
-Requires-Dist: Werkzeug>=2.3.7; extra == "flask-plugins"
-Provides-Extra: datatables
-Requires-Dist: eswrap>=0.5.0; extra == "datatables"
-Requires-Dist: redis>=4.6.0; extra == "datatables"
-Requires-Dist: kafka-python>=2.0.2; extra == "datatables"
-Requires-Dist: elasticsearch>=8.7.0; extra == "datatables"
-Requires-Dist: flask>=2.3.3; extra == "datatables"
-Requires-Dist: SQLAlchemy>=2.0.21; extra == "datatables"
-Requires-Dist: Flask_SQLAlchemy>=3.1.1; extra == "datatables"
-Requires-Dist: Werkzeug>=2.3.7; extra == "datatables"
+Provides-Extra: auth
+Requires-Dist: python-ldap>=3.4.3; extra == "auth"
+Provides-Extra: loggers
+Requires-Dist: gunicorn>=21.2.0; extra == "loggers"
+Requires-Dist: ansicolors>=1.1.8; extra == "loggers"
+Requires-Dist: pygelf>=0.4.2; extra == "loggers"
+Provides-Extra: sql-migrations
+Requires-Dist: Flask-Migrate>=4.0.5; extra == "sql-migrations"
+Requires-Dist: Flask_SQLAlchemy>=3.1.1; extra == "sql-migrations"
+Requires-Dist: flask>=2.3.3; extra == "sql-migrations"
+Requires-Dist: pymysql>=1.1.0; extra == "sql-migrations"
+Requires-Dist: mysqlclient>=2.1.1; extra == "sql-migrations"
+Requires-Dist: gunicorn>=21.2.0; extra == "sql-migrations"
+Requires-Dist: ansicolors>=1.1.8; extra == "sql-migrations"
+Requires-Dist: pygelf>=0.4.2; extra == "sql-migrations"
 Provides-Extra: flask-managers
 Requires-Dist: gunicorn>=21.2.0; extra == "flask-managers"
 Requires-Dist: flask>=2.3.3; extra == "flask-managers"
 Requires-Dist: pyopenssl>=23.2.0; extra == "flask-managers"
 Requires-Dist: Werkzeug>=2.3.7; extra == "flask-managers"
 Requires-Dist: gunicorn>=21.2.0; extra == "flask-managers"
 Requires-Dist: ansicolors>=1.1.8; extra == "flask-managers"
@@ -49,14 +46,16 @@
 Requires-Dist: Flask_SQLAlchemy>=3.1.1; extra == "flask-managers"
 Requires-Dist: flask>=2.3.3; extra == "flask-managers"
 Requires-Dist: pymysql>=1.1.0; extra == "flask-managers"
 Requires-Dist: mysqlclient>=2.1.1; extra == "flask-managers"
 Requires-Dist: gunicorn>=21.2.0; extra == "flask-managers"
 Requires-Dist: ansicolors>=1.1.8; extra == "flask-managers"
 Requires-Dist: pygelf>=0.4.2; extra == "flask-managers"
+Provides-Extra: http-apis
+Requires-Dist: requests>=2.31.0; extra == "http-apis"
 Provides-Extra: flask-middleware
 Requires-Dist: rfc3339>=6.2; extra == "flask-middleware"
 Requires-Dist: gunicorn>=21.2.0; extra == "flask-middleware"
 Requires-Dist: flask>=2.3.3; extra == "flask-middleware"
 Requires-Dist: pyopenssl>=23.2.0; extra == "flask-middleware"
 Requires-Dist: Werkzeug>=2.3.7; extra == "flask-middleware"
 Requires-Dist: gunicorn>=21.2.0; extra == "flask-middleware"
@@ -66,48 +65,49 @@
 Requires-Dist: Flask_SQLAlchemy>=3.1.1; extra == "flask-middleware"
 Requires-Dist: flask>=2.3.3; extra == "flask-middleware"
 Requires-Dist: pymysql>=1.1.0; extra == "flask-middleware"
 Requires-Dist: mysqlclient>=2.1.1; extra == "flask-middleware"
 Requires-Dist: gunicorn>=21.2.0; extra == "flask-middleware"
 Requires-Dist: ansicolors>=1.1.8; extra == "flask-middleware"
 Requires-Dist: pygelf>=0.4.2; extra == "flask-middleware"
-Provides-Extra: http-apis
-Requires-Dist: requests>=2.31.0; extra == "http-apis"
-Provides-Extra: loggers
-Requires-Dist: gunicorn>=21.2.0; extra == "loggers"
-Requires-Dist: ansicolors>=1.1.8; extra == "loggers"
-Requires-Dist: pygelf>=0.4.2; extra == "loggers"
-Provides-Extra: auth
-Requires-Dist: python-ldap>=3.4.3; extra == "auth"
-Provides-Extra: sql-migrations
-Requires-Dist: Flask-Migrate>=4.0.5; extra == "sql-migrations"
-Requires-Dist: Flask_SQLAlchemy>=3.1.1; extra == "sql-migrations"
-Requires-Dist: flask>=2.3.3; extra == "sql-migrations"
-Requires-Dist: pymysql>=1.1.0; extra == "sql-migrations"
-Requires-Dist: mysqlclient>=2.1.1; extra == "sql-migrations"
-Requires-Dist: gunicorn>=21.2.0; extra == "sql-migrations"
-Requires-Dist: ansicolors>=1.1.8; extra == "sql-migrations"
-Requires-Dist: pygelf>=0.4.2; extra == "sql-migrations"
+Provides-Extra: flask-plugins
+Requires-Dist: eswrap>=0.5.0; extra == "flask-plugins"
+Requires-Dist: redis>=4.6.0; extra == "flask-plugins"
+Requires-Dist: kafka-python>=2.0.2; extra == "flask-plugins"
+Requires-Dist: elasticsearch>=8.7.0; extra == "flask-plugins"
+Requires-Dist: flask>=2.3.3; extra == "flask-plugins"
+Requires-Dist: SQLAlchemy>=2.0.21; extra == "flask-plugins"
+Requires-Dist: Flask_SQLAlchemy>=3.1.1; extra == "flask-plugins"
+Requires-Dist: Werkzeug>=2.3.7; extra == "flask-plugins"
+Provides-Extra: datatables
+Requires-Dist: eswrap>=0.5.0; extra == "datatables"
+Requires-Dist: redis>=4.6.0; extra == "datatables"
+Requires-Dist: kafka-python>=2.0.2; extra == "datatables"
+Requires-Dist: elasticsearch>=8.7.0; extra == "datatables"
+Requires-Dist: flask>=2.3.3; extra == "datatables"
+Requires-Dist: SQLAlchemy>=2.0.21; extra == "datatables"
+Requires-Dist: Flask_SQLAlchemy>=3.1.1; extra == "datatables"
+Requires-Dist: Werkzeug>=2.3.7; extra == "datatables"
 Provides-Extra: all
+Requires-Dist: gunicorn>=21.2.0; extra == "all"
+Requires-Dist: pygelf>=0.4.2; extra == "all"
+Requires-Dist: rfc3339>=6.2; extra == "all"
 Requires-Dist: elasticsearch>=8.7.0; extra == "all"
-Requires-Dist: Flask-Migrate>=4.0.5; extra == "all"
+Requires-Dist: SQLAlchemy>=2.0.21; extra == "all"
+Requires-Dist: mysqlclient>=2.1.1; extra == "all"
+Requires-Dist: ansicolors>=1.1.8; extra == "all"
+Requires-Dist: pyopenssl>=23.2.0; extra == "all"
+Requires-Dist: pymysql>=1.1.0; extra == "all"
 Requires-Dist: Werkzeug>=2.3.7; extra == "all"
+Requires-Dist: requests>=2.31.0; extra == "all"
 Requires-Dist: flask>=2.3.3; extra == "all"
 Requires-Dist: eswrap>=0.5.0; extra == "all"
-Requires-Dist: pygelf>=0.4.2; extra == "all"
-Requires-Dist: pyopenssl>=23.2.0; extra == "all"
 Requires-Dist: redis>=4.6.0; extra == "all"
-Requires-Dist: mysqlclient>=2.1.1; extra == "all"
-Requires-Dist: rfc3339>=6.2; extra == "all"
-Requires-Dist: requests>=2.31.0; extra == "all"
-Requires-Dist: gunicorn>=21.2.0; extra == "all"
-Requires-Dist: ansicolors>=1.1.8; extra == "all"
-Requires-Dist: pymysql>=1.1.0; extra == "all"
 Requires-Dist: python-ldap>=3.4.3; extra == "all"
-Requires-Dist: SQLAlchemy>=2.0.21; extra == "all"
+Requires-Dist: Flask-Migrate>=4.0.5; extra == "all"
 Requires-Dist: kafka-python>=2.0.2; extra == "all"
 Requires-Dist: Flask_SQLAlchemy>=3.1.1; extra == "all"
 
 # NLDCSC package
 
 [![GitHub Release](https://img.shields.io/github/release/NLDCSC/nldcsc.svg?style=flat)]()
 [![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
```

### Comparing `nldcsc-0.2.7/README.md` & `nldcsc-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/nldcsc/auth/ldap_client.py` & `nldcsc-0.2.8/nldcsc/auth/ldap_client.py`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/nldcsc/datatables/server_side_dt.py` & `nldcsc-0.2.8/nldcsc/datatables/server_side_dt.py`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/nldcsc/datatables/server_side_dt_es.py` & `nldcsc-0.2.8/nldcsc/datatables/server_side_dt_es.py`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/nldcsc/datatables/server_side_dt_sql.py` & `nldcsc-0.2.8/nldcsc/datatables/server_side_dt_sql.py`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/nldcsc/flask_managers/README.md` & `nldcsc-0.2.8/nldcsc/flask_managers/README.md`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/nldcsc/flask_managers/flask_app_manager.py` & `nldcsc-0.2.8/nldcsc/flask_managers/flask_app_manager.py`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/nldcsc/flask_midddleware/base.py` & `nldcsc-0.2.8/nldcsc/flask_midddleware/base.py`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/nldcsc/flask_midddleware/debug_logging.py` & `nldcsc-0.2.8/nldcsc/flask_midddleware/debug_logging.py`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/nldcsc/flask_midddleware/middleware_manager.py` & `nldcsc-0.2.8/nldcsc/flask_midddleware/middleware_manager.py`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/nldcsc/flask_plugins/README.md` & `nldcsc-0.2.8/nldcsc/flask_plugins/README.md`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/nldcsc/flask_plugins/flask_eswrap.py` & `nldcsc-0.2.8/nldcsc/flask_plugins/flask_eswrap.py`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/nldcsc/flask_plugins/flask_kafka.py` & `nldcsc-0.2.8/nldcsc/flask_plugins/flask_kafka.py`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/nldcsc/flask_plugins/flask_redis.py` & `nldcsc-0.2.8/nldcsc/flask_plugins/flask_redis.py`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/nldcsc/generic/times.py` & `nldcsc-0.2.8/nldcsc/generic/times.py`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/nldcsc/generic/utils.py` & `nldcsc-0.2.8/nldcsc/generic/utils.py`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/nldcsc/http_apis/base_class/api_base_class.py` & `nldcsc-0.2.8/nldcsc/http_apis/base_class/api_base_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,16 +119,19 @@
                 r = session.get(self._build_url(resource), **request_api_resource)
 
             try:
                 if isinstance(r, Response):
                     if return_response_object:
                         return r
                     if r.status_code >= 400:
-                        the_response = json.loads(r.text)
-                        raise requests.exceptions.ConnectionError(the_response)
+                        if isinstance(r.text, str):
+                            raise requests.exceptions.ConnectionError(r.text)
+                        else:
+                            the_response = json.loads(r.text)
+                            raise requests.exceptions.ConnectionError(the_response)
                     else:
                         the_response = json.loads(r.text)
                 else:
                     the_response = r
             except JSONDecodeError:
                 if "content-type" in r.headers:
                     if r.headers["content-type"] == "text/plain":
```

### Comparing `nldcsc-0.2.7/nldcsc/loggers/README.md` & `nldcsc-0.2.8/nldcsc/loggers/README.md`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/nldcsc/loggers/app_logger.py` & `nldcsc-0.2.8/nldcsc/loggers/app_logger.py`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/nldcsc/loggers/formatters/task_formatter.py` & `nldcsc-0.2.8/nldcsc/loggers/formatters/task_formatter.py`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/nldcsc/loggers/gunicorn_logger.py` & `nldcsc-0.2.8/nldcsc/loggers/gunicorn_logger.py`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/nldcsc/loggers/handlers/gelf_handler.py` & `nldcsc-0.2.8/nldcsc/loggers/handlers/gelf_handler.py`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/nldcsc/loggers/handlers/syslog_handler.py` & `nldcsc-0.2.8/nldcsc/loggers/handlers/syslog_handler.py`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/nldcsc/sql_migrations/flask_sql_migrate.py` & `nldcsc-0.2.8/nldcsc/sql_migrations/flask_sql_migrate.py`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/nldcsc.egg-info/PKG-INFO` & `nldcsc-0.2.8/nldcsc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nldcsc
-Version: 0.2.7
+Version: 0.2.8
 Summary: Package with general devops code
 Home-page: https://github.com/NLDCSC/nldcsc
 Author: NLDCSC
 Author-email: NLDCSC@invalid.com
 License: GNU General Public License v3.0
 Project-URL: Code, https://github.com/NLDCSC/nldcsc
 Platform: any
@@ -15,32 +15,29 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools>=68.1.0
-Provides-Extra: flask-plugins
-Requires-Dist: eswrap>=0.5.0; extra == "flask-plugins"
-Requires-Dist: redis>=4.6.0; extra == "flask-plugins"
-Requires-Dist: kafka-python>=2.0.2; extra == "flask-plugins"
-Requires-Dist: elasticsearch>=8.7.0; extra == "flask-plugins"
-Requires-Dist: flask>=2.3.3; extra == "flask-plugins"
-Requires-Dist: SQLAlchemy>=2.0.21; extra == "flask-plugins"
-Requires-Dist: Flask_SQLAlchemy>=3.1.1; extra == "flask-plugins"
-Requires-Dist: Werkzeug>=2.3.7; extra == "flask-plugins"
-Provides-Extra: datatables
-Requires-Dist: eswrap>=0.5.0; extra == "datatables"
-Requires-Dist: redis>=4.6.0; extra == "datatables"
-Requires-Dist: kafka-python>=2.0.2; extra == "datatables"
-Requires-Dist: elasticsearch>=8.7.0; extra == "datatables"
-Requires-Dist: flask>=2.3.3; extra == "datatables"
-Requires-Dist: SQLAlchemy>=2.0.21; extra == "datatables"
-Requires-Dist: Flask_SQLAlchemy>=3.1.1; extra == "datatables"
-Requires-Dist: Werkzeug>=2.3.7; extra == "datatables"
+Provides-Extra: auth
+Requires-Dist: python-ldap>=3.4.3; extra == "auth"
+Provides-Extra: loggers
+Requires-Dist: gunicorn>=21.2.0; extra == "loggers"
+Requires-Dist: ansicolors>=1.1.8; extra == "loggers"
+Requires-Dist: pygelf>=0.4.2; extra == "loggers"
+Provides-Extra: sql-migrations
+Requires-Dist: Flask-Migrate>=4.0.5; extra == "sql-migrations"
+Requires-Dist: Flask_SQLAlchemy>=3.1.1; extra == "sql-migrations"
+Requires-Dist: flask>=2.3.3; extra == "sql-migrations"
+Requires-Dist: pymysql>=1.1.0; extra == "sql-migrations"
+Requires-Dist: mysqlclient>=2.1.1; extra == "sql-migrations"
+Requires-Dist: gunicorn>=21.2.0; extra == "sql-migrations"
+Requires-Dist: ansicolors>=1.1.8; extra == "sql-migrations"
+Requires-Dist: pygelf>=0.4.2; extra == "sql-migrations"
 Provides-Extra: flask-managers
 Requires-Dist: gunicorn>=21.2.0; extra == "flask-managers"
 Requires-Dist: flask>=2.3.3; extra == "flask-managers"
 Requires-Dist: pyopenssl>=23.2.0; extra == "flask-managers"
 Requires-Dist: Werkzeug>=2.3.7; extra == "flask-managers"
 Requires-Dist: gunicorn>=21.2.0; extra == "flask-managers"
 Requires-Dist: ansicolors>=1.1.8; extra == "flask-managers"
@@ -49,14 +46,16 @@
 Requires-Dist: Flask_SQLAlchemy>=3.1.1; extra == "flask-managers"
 Requires-Dist: flask>=2.3.3; extra == "flask-managers"
 Requires-Dist: pymysql>=1.1.0; extra == "flask-managers"
 Requires-Dist: mysqlclient>=2.1.1; extra == "flask-managers"
 Requires-Dist: gunicorn>=21.2.0; extra == "flask-managers"
 Requires-Dist: ansicolors>=1.1.8; extra == "flask-managers"
 Requires-Dist: pygelf>=0.4.2; extra == "flask-managers"
+Provides-Extra: http-apis
+Requires-Dist: requests>=2.31.0; extra == "http-apis"
 Provides-Extra: flask-middleware
 Requires-Dist: rfc3339>=6.2; extra == "flask-middleware"
 Requires-Dist: gunicorn>=21.2.0; extra == "flask-middleware"
 Requires-Dist: flask>=2.3.3; extra == "flask-middleware"
 Requires-Dist: pyopenssl>=23.2.0; extra == "flask-middleware"
 Requires-Dist: Werkzeug>=2.3.7; extra == "flask-middleware"
 Requires-Dist: gunicorn>=21.2.0; extra == "flask-middleware"
@@ -66,48 +65,49 @@
 Requires-Dist: Flask_SQLAlchemy>=3.1.1; extra == "flask-middleware"
 Requires-Dist: flask>=2.3.3; extra == "flask-middleware"
 Requires-Dist: pymysql>=1.1.0; extra == "flask-middleware"
 Requires-Dist: mysqlclient>=2.1.1; extra == "flask-middleware"
 Requires-Dist: gunicorn>=21.2.0; extra == "flask-middleware"
 Requires-Dist: ansicolors>=1.1.8; extra == "flask-middleware"
 Requires-Dist: pygelf>=0.4.2; extra == "flask-middleware"
-Provides-Extra: http-apis
-Requires-Dist: requests>=2.31.0; extra == "http-apis"
-Provides-Extra: loggers
-Requires-Dist: gunicorn>=21.2.0; extra == "loggers"
-Requires-Dist: ansicolors>=1.1.8; extra == "loggers"
-Requires-Dist: pygelf>=0.4.2; extra == "loggers"
-Provides-Extra: auth
-Requires-Dist: python-ldap>=3.4.3; extra == "auth"
-Provides-Extra: sql-migrations
-Requires-Dist: Flask-Migrate>=4.0.5; extra == "sql-migrations"
-Requires-Dist: Flask_SQLAlchemy>=3.1.1; extra == "sql-migrations"
-Requires-Dist: flask>=2.3.3; extra == "sql-migrations"
-Requires-Dist: pymysql>=1.1.0; extra == "sql-migrations"
-Requires-Dist: mysqlclient>=2.1.1; extra == "sql-migrations"
-Requires-Dist: gunicorn>=21.2.0; extra == "sql-migrations"
-Requires-Dist: ansicolors>=1.1.8; extra == "sql-migrations"
-Requires-Dist: pygelf>=0.4.2; extra == "sql-migrations"
+Provides-Extra: flask-plugins
+Requires-Dist: eswrap>=0.5.0; extra == "flask-plugins"
+Requires-Dist: redis>=4.6.0; extra == "flask-plugins"
+Requires-Dist: kafka-python>=2.0.2; extra == "flask-plugins"
+Requires-Dist: elasticsearch>=8.7.0; extra == "flask-plugins"
+Requires-Dist: flask>=2.3.3; extra == "flask-plugins"
+Requires-Dist: SQLAlchemy>=2.0.21; extra == "flask-plugins"
+Requires-Dist: Flask_SQLAlchemy>=3.1.1; extra == "flask-plugins"
+Requires-Dist: Werkzeug>=2.3.7; extra == "flask-plugins"
+Provides-Extra: datatables
+Requires-Dist: eswrap>=0.5.0; extra == "datatables"
+Requires-Dist: redis>=4.6.0; extra == "datatables"
+Requires-Dist: kafka-python>=2.0.2; extra == "datatables"
+Requires-Dist: elasticsearch>=8.7.0; extra == "datatables"
+Requires-Dist: flask>=2.3.3; extra == "datatables"
+Requires-Dist: SQLAlchemy>=2.0.21; extra == "datatables"
+Requires-Dist: Flask_SQLAlchemy>=3.1.1; extra == "datatables"
+Requires-Dist: Werkzeug>=2.3.7; extra == "datatables"
 Provides-Extra: all
+Requires-Dist: gunicorn>=21.2.0; extra == "all"
+Requires-Dist: pygelf>=0.4.2; extra == "all"
+Requires-Dist: rfc3339>=6.2; extra == "all"
 Requires-Dist: elasticsearch>=8.7.0; extra == "all"
-Requires-Dist: Flask-Migrate>=4.0.5; extra == "all"
+Requires-Dist: SQLAlchemy>=2.0.21; extra == "all"
+Requires-Dist: mysqlclient>=2.1.1; extra == "all"
+Requires-Dist: ansicolors>=1.1.8; extra == "all"
+Requires-Dist: pyopenssl>=23.2.0; extra == "all"
+Requires-Dist: pymysql>=1.1.0; extra == "all"
 Requires-Dist: Werkzeug>=2.3.7; extra == "all"
+Requires-Dist: requests>=2.31.0; extra == "all"
 Requires-Dist: flask>=2.3.3; extra == "all"
 Requires-Dist: eswrap>=0.5.0; extra == "all"
-Requires-Dist: pygelf>=0.4.2; extra == "all"
-Requires-Dist: pyopenssl>=23.2.0; extra == "all"
 Requires-Dist: redis>=4.6.0; extra == "all"
-Requires-Dist: mysqlclient>=2.1.1; extra == "all"
-Requires-Dist: rfc3339>=6.2; extra == "all"
-Requires-Dist: requests>=2.31.0; extra == "all"
-Requires-Dist: gunicorn>=21.2.0; extra == "all"
-Requires-Dist: ansicolors>=1.1.8; extra == "all"
-Requires-Dist: pymysql>=1.1.0; extra == "all"
 Requires-Dist: python-ldap>=3.4.3; extra == "all"
-Requires-Dist: SQLAlchemy>=2.0.21; extra == "all"
+Requires-Dist: Flask-Migrate>=4.0.5; extra == "all"
 Requires-Dist: kafka-python>=2.0.2; extra == "all"
 Requires-Dist: Flask_SQLAlchemy>=3.1.1; extra == "all"
 
 # NLDCSC package
 
 [![GitHub Release](https://img.shields.io/github/release/NLDCSC/nldcsc.svg?style=flat)]()
 [![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
```

### Comparing `nldcsc-0.2.7/nldcsc.egg-info/SOURCES.txt` & `nldcsc-0.2.8/nldcsc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/nldcsc.egg-info/requires.txt` & `nldcsc-0.2.8/nldcsc.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 setuptools>=68.1.0
 
 [all]
+gunicorn>=21.2.0
+pygelf>=0.4.2
+rfc3339>=6.2
 elasticsearch>=8.7.0
-Flask-Migrate>=4.0.5
+SQLAlchemy>=2.0.21
+mysqlclient>=2.1.1
+ansicolors>=1.1.8
+pyopenssl>=23.2.0
+pymysql>=1.1.0
 Werkzeug>=2.3.7
+requests>=2.31.0
 flask>=2.3.3
 eswrap>=0.5.0
-pygelf>=0.4.2
-pyopenssl>=23.2.0
 redis>=4.6.0
-mysqlclient>=2.1.1
-rfc3339>=6.2
-requests>=2.31.0
-gunicorn>=21.2.0
-ansicolors>=1.1.8
-pymysql>=1.1.0
 python-ldap>=3.4.3
-SQLAlchemy>=2.0.21
+Flask-Migrate>=4.0.5
 kafka-python>=2.0.2
 Flask_SQLAlchemy>=3.1.1
 
 [auth]
 python-ldap>=3.4.3
 
 [datatables]
```

### Comparing `nldcsc-0.2.7/setup.py` & `nldcsc-0.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/tests/applications/migrate_app.py` & `nldcsc-0.2.8/tests/applications/migrate_app.py`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/tests/helpers/capture_logging.py` & `nldcsc-0.2.8/tests/helpers/capture_logging.py`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/tests/test_generic.py` & `nldcsc-0.2.8/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/tests/test_http_apis.py` & `nldcsc-0.2.8/tests/test_http_apis.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,18 +149,17 @@
 
     def test_session_calls(self, http_api):
         with requests_mock.Mocker() as m:
             m.get(
                 "http://localhost:8000/dummy", text='{"data": "data"}', status_code=404
             )
 
-            with pytest.raises(requests.ConnectionError):
-                d = http_api.get_dummy_endpoint()
+            d = http_api.get_dummy_endpoint()
 
-                assert d == {"data": "data"}
+            assert isinstance(d, requests.Response)
 
         with requests_mock.Mocker() as m:
             m.get(
                 "http://localhost:8000/dummy?id=1&id2=10",
                 json={"id": "1", "id2": 10, "result": "success"},
                 status_code=200,
             )
@@ -215,16 +214,15 @@
         with requests_mock.Mocker() as m:
             m.get(
                 "http://localhost:8000/dummy",
                 text="just string data",
                 status_code=200,
             )
 
-            with pytest.raises(Exception):
-                http_api.get_dummy_endpoint()
+            http_api.get_dummy_endpoint()
         with pytest.raises(requests.ConnectionError):
             http_api.delete_dict_dummy()
 
         with requests_mock.Mocker() as m:
             m.post(
                 "http://localhost:8000/dummy",
                 text="just string data",
```

### Comparing `nldcsc-0.2.7/tests/test_logger.py` & `nldcsc-0.2.8/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `nldcsc-0.2.7/tests/test_sqlalchemy_migrate.py` & `nldcsc-0.2.8/tests/test_sqlalchemy_migrate.py`

 * *Files identical despite different names*

