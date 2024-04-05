# Comparing `tmp/dockerflow-2024.3.0.tar.gz` & `tmp/dockerflow-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dockerflow-2024.3.0.tar", last modified: Mon Mar  4 10:46:32 2024, max compression
+gzip compressed data, was "dockerflow-2024.4.0.tar", last modified: Fri Apr  5 13:51:51 2024, max compression
```

## Comparing `dockerflow-2024.3.0.tar` & `dockerflow-2024.4.0.tar`

### file list

```diff
@@ -1,123 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:46:32.346461 dockerflow-2024.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:46:32.326461 dockerflow-2024.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:46:32.330461 dockerflow-2024.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-03-04 10:46:32.346461 dockerflow-2024.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:46:32.334461 dockerflow-2024.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:46:32.334461 dockerflow-2024.3.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/docs/api/django.rst
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/docs/api/fastapi.rst
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/docs/api/flask.rst
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/docs/api/logging.rst
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/docs/api/sanic.rst
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/docs/api/version.rst
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10976 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/docs/development.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14511 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/docs/django.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9674 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/docs/fastapi.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15000 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/docs/flask.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/docs/logging.rst
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14332 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/docs/sanic.rst
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-04 10:46:32.346461 dockerflow-2024.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:46:32.326461 dockerflow-2024.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:46:32.334461 dockerflow-2024.3.0/src/dockerflow/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/src/dockerflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:46:32.338461 dockerflow-2024.3.0/src/dockerflow/checks/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/src/dockerflow/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/src/dockerflow/checks/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/src/dockerflow/checks/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:46:32.338461 dockerflow-2024.3.0/src/dockerflow/django/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/src/dockerflow/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/src/dockerflow/django/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/src/dockerflow/django/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/src/dockerflow/django/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/src/dockerflow/django/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/src/dockerflow/django/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:46:32.338461 dockerflow-2024.3.0/src/dockerflow/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/src/dockerflow/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/src/dockerflow/fastapi/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/src/dockerflow/fastapi/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:46:32.338461 dockerflow-2024.3.0/src/dockerflow/flask/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/src/dockerflow/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13516 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/src/dockerflow/flask/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:46:32.338461 dockerflow-2024.3.0/src/dockerflow/flask/checks/
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/src/dockerflow/flask/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/src/dockerflow/flask/checks/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/src/dockerflow/flask/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/src/dockerflow/health.py
--rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/src/dockerflow/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:46:32.338461 dockerflow-2024.3.0/src/dockerflow/sanic/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/src/dockerflow/sanic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/src/dockerflow/sanic/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/src/dockerflow/sanic/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/src/dockerflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:46:32.346461 dockerflow-2024.3.0/src/dockerflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-03-04 10:46:32.000000 dockerflow-2024.3.0/src/dockerflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-03-04 10:46:32.000000 dockerflow-2024.3.0/src/dockerflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 10:46:32.000000 dockerflow-2024.3.0/src/dockerflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 10:46:32.000000 dockerflow-2024.3.0/src/dockerflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-04 10:46:32.000000 dockerflow-2024.3.0/src/dockerflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-04 10:46:32.000000 dockerflow-2024.3.0/src/dockerflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:46:32.342461 dockerflow-2024.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:46:32.342461 dockerflow-2024.3.0/tests/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/constraints/django-3.2.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/constraints/django-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/constraints/django-4.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/constraints/django-4.2.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/constraints/django-5.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/constraints/fastapi-0.100.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/constraints/flask-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/constraints/flask-2.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/constraints/flask-2.2.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/constraints/sanic-21.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/constraints/sanic-22.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:46:32.342461 dockerflow-2024.3.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/core/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/core/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/core/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:46:32.342461 dockerflow-2024.3.0/tests/django/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/django/django_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/django/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/django/test_django.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/django/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:46:32.342461 dockerflow-2024.3.0/tests/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/fastapi/test_fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:46:32.342461 dockerflow-2024.3.0/tests/flask/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:46:32.346461 dockerflow-2024.3.0/tests/flask/migrations/
--rwxr-xr-x   0 runner    (1001) docker     (127)       38 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/flask/migrations/README
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/flask/migrations/alembic.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)     2689 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/flask/migrations/env.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      494 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/flask/migrations/script.py.mako
--rw-r--r--   0 runner    (1001) docker     (127)    18113 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/flask/test_flask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:46:32.346461 dockerflow-2024.3.0/tests/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/requirements/default.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/requirements/django.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/requirements/fastapi.txt
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/requirements/flask.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/requirements/lint.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/requirements/sanic.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:46:32.346461 dockerflow-2024.3.0/tests/sanic/
--rw-r--r--   0 runner    (1001) docker     (127)     9854 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tests/sanic/test_sanic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-03-04 10:46:27.000000 dockerflow-2024.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:51:51.285091 dockerflow-2024.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:51:51.265091 dockerflow-2024.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:51:51.269091 dockerflow-2024.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-05 13:51:51.285091 dockerflow-2024.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:51:51.273091 dockerflow-2024.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:51:51.273091 dockerflow-2024.4.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/docs/api/django.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/docs/api/fastapi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/docs/api/flask.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/docs/api/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/docs/api/sanic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/docs/api/version.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10976 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/docs/development.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14949 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/docs/django.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/docs/fastapi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15439 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/docs/flask.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/docs/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14771 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/docs/sanic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-05 13:51:51.289091 dockerflow-2024.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:51:51.265091 dockerflow-2024.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:51:51.273091 dockerflow-2024.4.0/src/dockerflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/src/dockerflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:51:51.277091 dockerflow-2024.4.0/src/dockerflow/checks/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/src/dockerflow/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/src/dockerflow/checks/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/src/dockerflow/checks/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:51:51.277091 dockerflow-2024.4.0/src/dockerflow/django/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/src/dockerflow/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/src/dockerflow/django/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/src/dockerflow/django/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/src/dockerflow/django/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/src/dockerflow/django/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/src/dockerflow/django/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:51:51.277091 dockerflow-2024.4.0/src/dockerflow/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/src/dockerflow/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/src/dockerflow/fastapi/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/src/dockerflow/fastapi/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:51:51.277091 dockerflow-2024.4.0/src/dockerflow/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/src/dockerflow/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13516 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/src/dockerflow/flask/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:51:51.277091 dockerflow-2024.4.0/src/dockerflow/flask/checks/
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/src/dockerflow/flask/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/src/dockerflow/flask/checks/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/src/dockerflow/flask/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/src/dockerflow/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/src/dockerflow/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:51:51.277091 dockerflow-2024.4.0/src/dockerflow/sanic/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/src/dockerflow/sanic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/src/dockerflow/sanic/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/src/dockerflow/sanic/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/src/dockerflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:51:51.285091 dockerflow-2024.4.0/src/dockerflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-05 13:51:51.000000 dockerflow-2024.4.0/src/dockerflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-05 13:51:51.000000 dockerflow-2024.4.0/src/dockerflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:51:51.000000 dockerflow-2024.4.0/src/dockerflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:51:51.000000 dockerflow-2024.4.0/src/dockerflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-05 13:51:51.000000 dockerflow-2024.4.0/src/dockerflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 13:51:51.000000 dockerflow-2024.4.0/src/dockerflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:51:51.281091 dockerflow-2024.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:51:51.281091 dockerflow-2024.4.0/tests/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/constraints/django-3.2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/constraints/django-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/constraints/django-4.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/constraints/django-4.2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/constraints/django-5.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/constraints/fastapi-0.100.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/constraints/flask-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/constraints/flask-2.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/constraints/flask-2.2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/constraints/flask-2.3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/constraints/flask-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/constraints/sanic-21.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/constraints/sanic-22.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/constraints/sanic-23.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:51:51.281091 dockerflow-2024.4.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/core/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/core/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/core/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:51:51.281091 dockerflow-2024.4.0/tests/django/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/django/django_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/django/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/django/test_django.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/django/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:51:51.285091 dockerflow-2024.4.0/tests/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/fastapi/test_fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:51:51.285091 dockerflow-2024.4.0/tests/flask/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:51:51.285091 dockerflow-2024.4.0/tests/flask/migrations/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       38 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/flask/migrations/README
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/flask/migrations/alembic.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2689 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/flask/migrations/env.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      494 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/flask/migrations/script.py.mako
+-rw-r--r--   0 runner    (1001) docker     (127)    18297 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/flask/test_flask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:51:51.285091 dockerflow-2024.4.0/tests/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/requirements/default.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/requirements/django.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/requirements/fastapi.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/requirements/flask.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/requirements/lint.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/requirements/sanic.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:51:51.285091 dockerflow-2024.4.0/tests/sanic/
+-rw-r--r--   0 runner    (1001) docker     (127)     9854 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tests/sanic/test_sanic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-05 13:51:44.000000 dockerflow-2024.4.0/tox.ini
```

### Comparing `dockerflow-2024.3.0/.github/workflows/release.yml` & `dockerflow-2024.4.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/.github/workflows/test.yml` & `dockerflow-2024.4.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/LICENSE` & `dockerflow-2024.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/PKG-INFO` & `dockerflow-2024.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dockerflow
-Version: 2024.3.0
+Version: 2024.4.0
 Summary: Python tools and helpers for Mozilla's Dockerflow
 Home-page: https://github.com/mozilla-services/python-dockerflow
 Author: Mozilla Foundation
 Author-email: dev-webdev@lists.mozilla.org
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment :: Mozilla
```

### Comparing `dockerflow-2024.3.0/README.rst` & `dockerflow-2024.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/docs/Makefile` & `dockerflow-2024.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/docs/api/django.rst` & `dockerflow-2024.4.0/docs/api/django.rst`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/docs/changelog.rst` & `dockerflow-2024.4.0/docs/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 ---------
 
+
+2024.3.1 (unreleased)
+~~~~~~~~~~~~~~~~~~~~~
+
+- Add support for Flask 2.3 and 3.0 (#103)
+
+
 2024.3.0
 ~~~~~~~~~~~~~~~~~~~~~
 
 - Add request correlation ID support (#101).
   In order to add a ``rid`` field to all log messages, add the ``dockerflow.logging.RequestIdLogFilter`` filter to your logging handlers.
   See: :ref:`Django <django-logging>`, :ref:`FastAPI <fastapi-logging>`, :ref:`Flask <flask-logging>`, :ref:`Sanic <sanic-logging>` for details.
```

### Comparing `dockerflow-2024.3.0/docs/conf.py` & `dockerflow-2024.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/docs/development.rst` & `dockerflow-2024.4.0/docs/development.rst`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/docs/django.rst` & `dockerflow-2024.4.0/docs/django.rst`

 * *Files 6% similar despite different names*

```diff
@@ -410,17 +410,34 @@
 In order to include querystrings in the request summary log, set this flag in settings:
 
 .. code-block:: python
 
     DOCKERFLOW_SUMMARY_LOG_QUERYSTRING = True
 
 
-A unique request ID is read from the `X-Request-ID` request header, and a UUID4 value is generated if unset.
+MozLog App-Specific Fields
+~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Leveraging the `RequestIdFilter` in logging configuration as shown above will add a ``rid`` attribute to all log messages.
+The *MozLog* formatter will output ``Fields`` application-specific fields. It can be populated through the ``extra`` parameter:
+
+.. code-block:: python
+
+    logger.info(
+        "Subsystem %s running at %s:%s",
+        name, host, port,
+        extra={"phase": "started", "host": host, "port": port}
+    )
+
+
+Requests Correlation ID
+~~~~~~~~~~~~~~~~~~~~~~~
+
+A unique request ID is read from the ``X-Request-ID`` request header, and a UUID4 value is generated if unset.
+
+Leveraging the ``RequestIdFilter`` in logging configuration as shown above will add a ``rid`` field into the ``Fields`` entry of all log messages.
 
 The header name to obtain the request ID can be customized in settings:
 
 .. code-block:: python
 
     DOCKERFLOW_REQUEST_ID_HEADER_NAME = "X-Cloud-Trace-Context"
```

### Comparing `dockerflow-2024.3.0/docs/fastapi.rst` & `dockerflow-2024.4.0/docs/fastapi.rst`

 * *Files 5% similar despite different names*

```diff
@@ -322,17 +322,35 @@
 
 In order to include querystrings in the request summary log, set this flag in the application state:
 
 .. code-block:: python
 
     app.state.DOCKERFLOW_SUMMARY_LOG_QUERYSTRING = True
 
-A unique request ID is read from the `X-Request-ID` request header using the `RequestIdMiddleware` middleware (see :ref:`fastapi-setup`), and a UUID4 value is generated if unset.
 
-Leveraging the `RequestIdFilter` in logging configuration as shown above will add a ``rid`` attribute to all log messages.
+MozLog App-Specific Fields
+~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The *MozLog* formatter will output ``Fields`` application-specific fields. It can be populated through the ``extra`` parameter:
+
+.. code-block:: python
+
+    logger.info(
+        "Subsystem %s running at %s:%s",
+        name, host, port,
+        extra={"phase": "started", "host": host, "port": port}
+    )
+
+
+Requests Correlation ID
+~~~~~~~~~~~~~~~~~~~~~~~
+
+A unique request ID is read from the ``X-Request-ID`` request header, and a UUID4 value is generated if unset.
+
+Leveraging the ``RequestIdFilter`` in logging configuration as shown above will add a ``rid`` field into the ``Fields`` entry of all log messages.
 
 The header name to obtain the request ID can be customized in settings:
 
 .. code-block:: python
 
     app.state.DOCKERFLOW_REQUEST_ID_HEADER_NAME = "X-Cloud-Trace-Context"
```

### Comparing `dockerflow-2024.3.0/docs/flask.rst` & `dockerflow-2024.4.0/docs/flask.rst`

 * *Files 1% similar despite different names*

```diff
@@ -462,17 +462,35 @@
         }
     })
 
 In order to include querystrings in the request summary log, set this flag in :ref:`configuration <flask-config>`::
 
     DOCKERFLOW_SUMMARY_LOG_QUERYSTRING = True
 
-A unique request ID is read from the `X-Request-ID` request header, and a UUID4 value is generated if unset.
 
-Leveraging the `RequestIdFilter` in logging configuration as shown above will add a ``rid`` attribute to all log messages.
+MozLog App-Specific Fields
+~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The *MozLog* formatter will output ``Fields`` application-specific fields. It can be populated through the ``extra`` parameter:
+
+.. code-block:: python
+
+    logger.info(
+        "Subsystem %s running at %s:%s",
+        name, host, port,
+        extra={"phase": "started", "host": host, "port": port}
+    )
+
+
+Requests Correlation ID
+~~~~~~~~~~~~~~~~~~~~~~~
+
+A unique request ID is read from the ``X-Request-ID`` request header, and a UUID4 value is generated if unset.
+
+Leveraging the ``RequestIdFilter`` in logging configuration as shown above will add a ``rid`` field into the ``Fields`` entry of all log messages.
 
 The header name to obtain the request ID can be customized in settings:
 
 .. code-block:: python
 
     DOCKERFLOW_REQUEST_ID_HEADER_NAME = "X-Cloud-Trace-Context"
```

### Comparing `dockerflow-2024.3.0/docs/index.rst` & `dockerflow-2024.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/docs/logging.rst` & `dockerflow-2024.4.0/docs/logging.rst`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/docs/sanic.rst` & `dockerflow-2024.4.0/docs/sanic.rst`

 * *Files 3% similar despite different names*

```diff
@@ -461,17 +461,35 @@
 
     sanic = Sanic(__name__)
 
 In order to include querystrings in the request summary log, set this flag in :ref:`configuration <sanic-config>`::
 
     DOCKERFLOW_SUMMARY_LOG_QUERYSTRING = True
 
-A unique request ID is read from the `X-Request-ID` request header, and a UUID4 value is generated if unset.
 
-Leveraging the `RequestIdFilter` in logging configuration as shown above will add a ``rid`` attribute to all log messages.
+MozLog App-Specific Fields
+~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The *MozLog* formatter will output ``Fields`` application-specific fields. It can be populated through the ``extra`` parameter:
+
+.. code-block:: python
+
+    logger.info(
+        "Subsystem %s running at %s:%s",
+        name, host, port,
+        extra={"phase": "started", "host": host, "port": port}
+    )
+
+
+Requests Correlation ID
+~~~~~~~~~~~~~~~~~~~~~~~
+
+A unique request ID is read from the ``X-Request-ID`` request header, and a UUID4 value is generated if unset.
+
+Leveraging the ``RequestIdFilter`` in logging configuration as shown above will add a ``rid`` field into the ``Fields`` entry of all log messages.
 
 The header name to obtain the request ID can be customized in settings:
 
 .. code-block:: python
 
     DOCKERFLOW_REQUEST_ID_HEADER_NAME = "X-Cloud-Trace-Context"
```

### Comparing `dockerflow-2024.3.0/setup.py` & `dockerflow-2024.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/src/dockerflow/checks/__init__.py` & `dockerflow-2024.4.0/src/dockerflow/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/src/dockerflow/checks/messages.py` & `dockerflow-2024.4.0/src/dockerflow/checks/messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, you can obtain one at http://mozilla.org/MPL/2.0/.
 """
 This is a minor port of the Django checks system messages to be used
 for Dockerflow checks of the Flask and Sanic extensions.
 """
+
 # Levels
 DEBUG = 10
 INFO = 20
 WARNING = 30
 ERROR = 40
 CRITICAL = 50
 STATUSES = {
```

### Comparing `dockerflow-2024.3.0/src/dockerflow/checks/registry.py` & `dockerflow-2024.4.0/src/dockerflow/checks/registry.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/src/dockerflow/django/checks.py` & `dockerflow-2024.4.0/src/dockerflow/django/checks.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/src/dockerflow/django/middleware.py` & `dockerflow-2024.4.0/src/dockerflow/django/middleware.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/src/dockerflow/django/signals.py` & `dockerflow-2024.4.0/src/dockerflow/django/signals.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,11 +29,12 @@
     def heartbeat_passed_handler(sender, level, **kwargs):
         statsd.incr('heartbeat.pass')
 
     @receiver(heartbeat_failed)
     def heartbeat_failed_handler(sender, level, **kwargs):
         statsd.incr('heartbeat.fail')
 """
+
 from django.dispatch import Signal
 
 heartbeat_passed = Signal()
 heartbeat_failed = Signal()
```

### Comparing `dockerflow-2024.3.0/src/dockerflow/django/views.py` & `dockerflow-2024.4.0/src/dockerflow/django/views.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/src/dockerflow/fastapi/middleware.py` & `dockerflow-2024.4.0/src/dockerflow/fastapi/middleware.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     ) -> None:
         self.app = app
         if logger is None:
             logger = logging.getLogger("request.summary")
             logger.setLevel(logging.INFO)
             handler = logging.StreamHandler(sys.stdout)
             handler.setLevel(logging.INFO)
-            handler.setFormatter(JsonLogFormatter)
+            handler.setFormatter(JsonLogFormatter())
             logger.addHandler(handler)
         self.logger = logger
 
     async def __call__(
         self, scope: HTTPScope, receive: ASGIReceiveCallable, send: ASGISendCallable
     ) -> None:
         if scope["type"] != "http":
```

### Comparing `dockerflow-2024.3.0/src/dockerflow/fastapi/views.py` & `dockerflow-2024.4.0/src/dockerflow/fastapi/views.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/src/dockerflow/flask/app.py` & `dockerflow-2024.4.0/src/dockerflow/flask/app.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/src/dockerflow/flask/checks/__init__.py` & `dockerflow-2024.4.0/src/dockerflow/flask/checks/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, you can obtain one at http://mozilla.org/MPL/2.0/.
 """
 This module contains a few built-in checks for the Flask integration.
 """
+
 from sqlalchemy import text
 
 from ... import health
 from ...checks import (  # noqa
     CRITICAL,
     DEBUG,
     ERROR,
```

### Comparing `dockerflow-2024.3.0/src/dockerflow/flask/signals.py` & `dockerflow-2024.4.0/src/dockerflow/flask/signals.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,13 +29,14 @@
         statsd.incr('heartbeat.pass')
 
     @heartbeat_failed.connect_via(app)
     def heartbeat_failed_handler(sender, level, **extra):
         statsd.incr('heartbeat.fail')
 
 """
+
 from flask.signals import Namespace
 
 dockerflow_signals = Namespace()
 
 heartbeat_passed = dockerflow_signals.signal("heartbeat-passed")
 heartbeat_failed = dockerflow_signals.signal("heartbeat-failed")
```

### Comparing `dockerflow-2024.3.0/src/dockerflow/health.py` & `dockerflow-2024.4.0/src/dockerflow/health.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/src/dockerflow/logging.py` & `dockerflow-2024.4.0/src/dockerflow/logging.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/src/dockerflow/sanic/app.py` & `dockerflow-2024.4.0/src/dockerflow/sanic/app.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/src/dockerflow/sanic/checks.py` & `dockerflow-2024.4.0/src/dockerflow/sanic/checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, you can obtain one at http://mozilla.org/MPL/2.0/.
 """
 This module contains built-in checks for the Sanic integration.
 """
+
 from .. import health
 from ..checks import (  # noqa
     CRITICAL,
     DEBUG,
     ERROR,
     INFO,
     STATUSES,
```

### Comparing `dockerflow-2024.3.0/src/dockerflow/version.py` & `dockerflow-2024.4.0/src/dockerflow/version.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/src/dockerflow.egg-info/PKG-INFO` & `dockerflow-2024.4.0/src/dockerflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dockerflow
-Version: 2024.3.0
+Version: 2024.4.0
 Summary: Python tools and helpers for Mozilla's Dockerflow
 Home-page: https://github.com/mozilla-services/python-dockerflow
 Author: Mozilla Foundation
 Author-email: dev-webdev@lists.mozilla.org
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment :: Mozilla
```

### Comparing `dockerflow-2024.3.0/src/dockerflow.egg-info/SOURCES.txt` & `dockerflow-2024.4.0/src/dockerflow.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -69,16 +69,19 @@
 tests/constraints/django-4.1.txt
 tests/constraints/django-4.2.txt
 tests/constraints/django-5.0.txt
 tests/constraints/fastapi-0.100.txt
 tests/constraints/flask-2.0.txt
 tests/constraints/flask-2.1.txt
 tests/constraints/flask-2.2.txt
+tests/constraints/flask-2.3.txt
+tests/constraints/flask-3.0.txt
 tests/constraints/sanic-21.txt
 tests/constraints/sanic-22.txt
+tests/constraints/sanic-23.txt
 tests/core/test_checks.py
 tests/core/test_logging.py
 tests/core/test_version.py
 tests/django/__init__.py
 tests/django/django_checks.py
 tests/django/settings.py
 tests/django/test_django.py
```

### Comparing `dockerflow-2024.3.0/tests/conftest.py` & `dockerflow-2024.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/tests/core/test_checks.py` & `dockerflow-2024.4.0/tests/core/test_checks.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/tests/core/test_logging.py` & `dockerflow-2024.4.0/tests/core/test_logging.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/tests/core/test_version.py` & `dockerflow-2024.4.0/tests/core/test_version.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/tests/django/settings.py` & `dockerflow-2024.4.0/tests/django/settings.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/tests/django/test_django.py` & `dockerflow-2024.4.0/tests/django/test_django.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/tests/fastapi/test_fastapi.py` & `dockerflow-2024.4.0/tests/fastapi/test_fastapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,15 +43,29 @@
 
 def test_lbheartbeat_head(client):
     response = client.head("/__lbheartbeat__")
     assert response.status_code == 200
     assert response.content == b""
 
 
-def test_mozlog(app, client, caplog):
+def test_mozlog_record_formatted_as_json(app, client, capsys):
+    app.state.DOCKERFLOW_SUMMARY_LOG_QUERYSTRING = True
+
+    client.get(
+        "/__lbheartbeat__?x=شكر",
+        headers={
+            "User-Agent": "dockerflow/tests",
+            "Accept-Language": "en-US",
+        },
+    )
+    stdout = capsys.readouterr().out
+    assert json.loads(stdout)
+
+
+def test_mozlog_record_attrs(app, client, caplog):
     app.state.DOCKERFLOW_SUMMARY_LOG_QUERYSTRING = True
 
     client.get(
         "/__lbheartbeat__?x=شكر",
         headers={
             "User-Agent": "dockerflow/tests",
             "Accept-Language": "en-US",
```

### Comparing `dockerflow-2024.3.0/tests/flask/migrations/alembic.ini` & `dockerflow-2024.4.0/tests/flask/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/tests/flask/migrations/env.py` & `dockerflow-2024.4.0/tests/flask/migrations/env.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.3.0/tests/flask/test_flask.py` & `dockerflow-2024.4.0/tests/flask/test_flask.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,25 +9,31 @@
 import redis
 from fakeredis import FakeStrictRedis
 from flask import Flask, Response, g, has_request_context, request
 from flask_login import LoginManager, current_user, login_user
 from flask_login.mixins import UserMixin
 from flask_migrate import Migrate
 from flask_redis import FlaskRedis
-from flask_sqlalchemy import SQLAlchemy, get_debug_queries
+from flask_sqlalchemy import SQLAlchemy
 from sqlalchemy.exc import DBAPIError, SQLAlchemyError
 
 from dockerflow import checks, health
 from dockerflow.flask import Dockerflow
 from dockerflow.flask.checks import (
     check_database_connected,
     check_migrations_applied,
     check_redis_connected,
 )
 
+try:
+    from flask_sqlalchemy.record_queries import get_recorded_queries
+except ImportError:
+    # flask-sqlalchemy < 3
+    from flask_sqlalchemy import get_debug_queries as get_recorded_queries
+
 
 class MockUser(UserMixin):
     def __init__(self, id):
         self.id = id
 
 
 def load_user(user_id):
@@ -182,18 +188,18 @@
     logged = [(record.levelname, record.message) for record in caplog.records]
     assert ("ERROR", "tests.checks.E001: some error") in logged
     assert ("WARNING", "tests.checks.W001: some warning") in logged
 
 
 def test_lbheartbeat_makes_no_db_queries(dockerflow, app):
     with app.app_context():
-        assert len(get_debug_queries()) == 0
+        assert len(get_recorded_queries()) == 0
         response = app.test_client().get("/__lbheartbeat__")
         assert response.status_code == 200
-        assert len(get_debug_queries()) == 0
+        assert len(get_recorded_queries()) == 0
 
 
 def test_full_redis_check(mocker):
     app = Flask("redis-check")
     app.debug = True
     redis_store = FlaskRedis.from_custom_provider(FakeStrictRedis, app)
     Dockerflow(app, redis=redis_store)
```

### Comparing `dockerflow-2024.3.0/tests/sanic/test_sanic.py` & `dockerflow-2024.4.0/tests/sanic/test_sanic.py`

 * *Files identical despite different names*

