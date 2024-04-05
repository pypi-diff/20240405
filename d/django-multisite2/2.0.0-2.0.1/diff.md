# Comparing `tmp/django-multisite2-2.0.0.tar.gz` & `tmp/django-multisite2-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-multisite2-2.0.0.tar", last modified: Sun Mar 31 01:58:36 2024, max compression
+gzip compressed data, was "django-multisite2-2.0.1.tar", last modified: Fri Apr  5 18:56:15 2024, max compression
```

## Comparing `django-multisite2-2.0.0.tar` & `django-multisite2-2.0.1.tar`

### file list

```diff
@@ -1,79 +1,129 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 01:58:36.794163 django-multisite2-2.0.0/
--rw-r--r--   0 erikvw     (501) staff       (20)       98 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/.coveragerc
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 01:58:36.781638 django-multisite2-2.0.0/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 01:58:36.784834 django-multisite2-2.0.0/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     2091 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)      258 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1078 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)     3218 2024-03-31 01:58:23.000000 django-multisite2-2.0.0/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)     1497 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       55 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     7622 2024-03-31 01:58:36.794091 django-multisite2-2.0.0/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     6653 2024-03-31 01:58:23.000000 django-multisite2-2.0.0/README.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 01:58:36.793765 django-multisite2-2.0.0/django_multisite2.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     7622 2024-03-31 01:58:36.000000 django-multisite2-2.0.0/django_multisite2.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     2066 2024-03-31 01:58:36.000000 django-multisite2-2.0.0/django_multisite2.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2024-03-31 01:58:36.000000 django-multisite2-2.0.0/django_multisite2.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2024-03-31 01:58:36.000000 django-multisite2-2.0.0/django_multisite2.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       11 2024-03-31 01:58:36.000000 django-multisite2-2.0.0/django_multisite2.egg-info/requires.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       24 2024-03-31 01:58:36.000000 django-multisite2-2.0.0/django_multisite2.egg-info/top_level.txt
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 01:58:36.787380 django-multisite2-2.0.0/multisite/
--rw-r--r--   0 erikvw     (501) staff       (20)       45 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 01:58:36.787958 django-multisite2-2.0.0/multisite/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)      145 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1706 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/admin/alias_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2376 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/admin/multisite_changelist.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6414 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/admin/multisite_model_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      975 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1317 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/exceptions.py
--rw-r--r--   0 erikvw     (501) staff       (20)      681 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/forms.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5171 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/hacks.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 01:58:36.788106 django-multisite2-2.0.0/multisite/management/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/management/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 01:58:36.788299 django-multisite2-2.0.0/multisite/management/commands/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/management/commands/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      974 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/management/commands/update_public_suffix_list.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 01:58:36.788734 django-multisite2-2.0.0/multisite/middleware/
--rw-r--r--   0 erikvw     (501) staff       (20)      183 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/middleware/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2358 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/middleware/cookie_domain_middleware.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7515 2024-03-31 01:58:23.000000 django-multisite2-2.0.0/multisite/middleware/dynamic_site_middleware.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 01:58:36.789425 django-multisite2-2.0.0/multisite/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)     2273 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)      911 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/migrations/0002_alter_alias_id_alter_alias_is_canonical.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1252 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/migrations/0003_alter_alias_options_alter_alias_unique_together_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      649 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/migrations/0004_alter_alias_managers.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 01:58:36.790073 django-multisite2-2.0.0/multisite/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      165 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3692 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/models/alias.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6929 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/models/managers.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1540 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/models/signals.py
--rw-r--r--   0 erikvw     (501) staff       (20)      380 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/models/validators.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 01:58:36.791145 django-multisite2-2.0.0/multisite/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      400 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/tests/get_test_allowed_hosts.py
--rw-r--r--   0 erikvw     (501) staff       (20)      329 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/tests/get_test_http_response.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1212 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/tests/hosts.py
--rw-r--r--   0 erikvw     (501) staff       (20)      575 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/tests/test_settings.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 01:58:36.793011 django-multisite2-2.0.0/multisite/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      381 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/tests/tests/request_factory.py
--rw-r--r--   0 erikvw     (501) staff       (20)    10544 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/tests/tests/test_alias.py
--rw-r--r--   0 erikvw     (501) staff       (20)      638 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/tests/tests/test_contrib_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9193 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/tests/tests/test_cookie_domain_middleware.py
--rw-r--r--   0 erikvw     (501) staff       (20)    10931 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/tests/tests/test_dynamic_site_middleware.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5139 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/tests/tests/test_site_cache.py
--rw-r--r--   0 erikvw     (501) staff       (20)      923 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/tests/tests/test_site_domain.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2889 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/tests/tests/test_site_id.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1798 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/tests/tests/test_template_loader.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4140 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite/threadlocals.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5544 2024-03-31 01:58:23.000000 django-multisite2-2.0.0/multisite/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 01:58:36.793560 django-multisite2-2.0.0/multisite_app/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite_app/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      149 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite_app/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      129 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite_app/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      217 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/multisite_app/views.py
--rw-r--r--   0 erikvw     (501) staff       (20)      605 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)      640 2024-03-31 01:57:24.000000 django-multisite2-2.0.0/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1328 2024-03-31 01:58:36.794505 django-multisite2-2.0.0/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-05 18:56:15.161813 django-multisite2-2.0.1/
+-rw-r--r--   0 erikvw     (501) staff       (20)       98 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/.coveragerc
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-05 18:56:15.136637 django-multisite2-2.0.1/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-05 18:56:15.141130 django-multisite2-2.0.1/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2137 2024-04-05 18:53:41.000000 django-multisite2-2.0.1/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)      258 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1078 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)     3360 2024-04-05 18:56:07.000000 django-multisite2-2.0.1/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)     1497 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       55 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     7661 2024-04-05 18:56:15.161739 django-multisite2-2.0.1/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     6692 2024-04-05 18:53:41.000000 django-multisite2-2.0.1/README.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-05 18:56:15.161367 django-multisite2-2.0.1/django_multisite2.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     7661 2024-04-05 18:56:15.000000 django-multisite2-2.0.1/django_multisite2.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     4635 2024-04-05 18:56:15.000000 django-multisite2-2.0.1/django_multisite2.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2024-04-05 18:56:15.000000 django-multisite2-2.0.1/django_multisite2.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2024-03-31 01:58:36.000000 django-multisite2-2.0.1/django_multisite2.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       11 2024-04-05 18:56:15.000000 django-multisite2-2.0.1/django_multisite2.egg-info/requires.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       24 2024-04-05 18:56:15.000000 django-multisite2-2.0.1/django_multisite2.egg-info/top_level.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-05 18:56:15.143866 django-multisite2-2.0.1/multisite/
+-rw-r--r--   0 erikvw     (501) staff       (20)       45 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-05 18:56:15.145712 django-multisite2-2.0.1/multisite/__pycache__/
+-rw-r--r--   0 erikvw     (501) staff       (20)      238 2024-04-03 19:45:08.000000 django-multisite2-2.0.1/multisite/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)     1630 2024-04-03 19:45:08.000000 django-multisite2-2.0.1/multisite/__pycache__/apps.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)     2818 2024-04-03 20:27:43.000000 django-multisite2-2.0.1/multisite/__pycache__/exceptions.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)     1343 2024-04-03 19:45:10.000000 django-multisite2-2.0.1/multisite/__pycache__/forms.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)     8497 2024-04-03 19:45:08.000000 django-multisite2-2.0.1/multisite/__pycache__/hacks.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)     6432 2024-04-03 20:27:43.000000 django-multisite2-2.0.1/multisite/__pycache__/threadlocals.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)     7725 2024-04-03 19:45:08.000000 django-multisite2-2.0.1/multisite/__pycache__/utils.cpython-312.pyc
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-05 18:56:15.146433 django-multisite2-2.0.1/multisite/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      145 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/admin/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-05 18:56:15.147429 django-multisite2-2.0.1/multisite/admin/__pycache__/
+-rw-r--r--   0 erikvw     (501) staff       (20)      354 2024-04-03 19:45:10.000000 django-multisite2-2.0.1/multisite/admin/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)     2863 2024-04-03 19:45:10.000000 django-multisite2-2.0.1/multisite/admin/__pycache__/alias_admin.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)     3416 2024-04-03 19:45:10.000000 django-multisite2-2.0.1/multisite/admin/__pycache__/multisite_changelist.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)     8509 2024-04-03 19:45:10.000000 django-multisite2-2.0.1/multisite/admin/__pycache__/multisite_model_admin.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)     1706 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/admin/alias_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2376 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/admin/multisite_changelist.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6414 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/admin/multisite_model_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      975 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1373 2024-04-05 18:53:41.000000 django-multisite2-2.0.1/multisite/exceptions.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      681 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/forms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5171 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/hacks.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-05 18:56:15.147733 django-multisite2-2.0.1/multisite/management/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/management/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-05 18:56:15.147833 django-multisite2-2.0.1/multisite/management/__pycache__/
+-rw-r--r--   0 erikvw     (501) staff       (20)      179 2024-04-03 19:46:02.000000 django-multisite2-2.0.1/multisite/management/__pycache__/__init__.cpython-312.pyc
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-05 18:56:15.148175 django-multisite2-2.0.1/multisite/management/commands/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/management/commands/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-05 18:56:15.148584 django-multisite2-2.0.1/multisite/management/commands/__pycache__/
+-rw-r--r--   0 erikvw     (501) staff       (20)      188 2024-04-03 20:27:44.000000 django-multisite2-2.0.1/multisite/management/commands/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)     2092 2024-04-03 20:27:44.000000 django-multisite2-2.0.1/multisite/management/commands/__pycache__/update_public_suffix_list.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)      974 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/management/commands/update_public_suffix_list.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-05 18:56:15.149115 django-multisite2-2.0.1/multisite/middleware/
+-rw-r--r--   0 erikvw     (501) staff       (20)      183 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/middleware/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-05 18:56:15.149899 django-multisite2-2.0.1/multisite/middleware/__pycache__/
+-rw-r--r--   0 erikvw     (501) staff       (20)      361 2024-04-03 19:46:02.000000 django-multisite2-2.0.1/multisite/middleware/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)     3569 2024-04-03 19:46:02.000000 django-multisite2-2.0.1/multisite/middleware/__pycache__/cookie_domain_middleware.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)    10250 2024-04-03 20:27:43.000000 django-multisite2-2.0.1/multisite/middleware/__pycache__/dynamic_site_middleware.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)     2358 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/middleware/cookie_domain_middleware.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7823 2024-04-05 18:53:41.000000 django-multisite2-2.0.1/multisite/middleware/dynamic_site_middleware.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-05 18:56:15.150793 django-multisite2-2.0.1/multisite/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2273 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      911 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/migrations/0002_alter_alias_id_alter_alias_is_canonical.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1252 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/migrations/0003_alter_alias_options_alter_alias_unique_together_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      649 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/migrations/0004_alter_alias_managers.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-05 18:56:15.151844 django-multisite2-2.0.1/multisite/migrations/__pycache__/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2045 2024-04-03 19:45:22.000000 django-multisite2-2.0.1/multisite/migrations/__pycache__/0001_initial.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)     1251 2024-04-03 19:45:22.000000 django-multisite2-2.0.1/multisite/migrations/__pycache__/0002_alter_alias_id_alter_alias_is_canonical.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)     1622 2024-04-03 19:45:22.000000 django-multisite2-2.0.1/multisite/migrations/__pycache__/0003_alter_alias_options_alter_alias_unique_together_and_more.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)     1154 2024-04-03 19:45:22.000000 django-multisite2-2.0.1/multisite/migrations/__pycache__/0004_alter_alias_managers.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)      179 2024-04-03 19:45:22.000000 django-multisite2-2.0.1/multisite/migrations/__pycache__/__init__.cpython-312.pyc
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-05 18:56:15.152892 django-multisite2-2.0.1/multisite/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      165 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/models/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-05 18:56:15.154208 django-multisite2-2.0.1/multisite/models/__pycache__/
+-rw-r--r--   0 erikvw     (501) staff       (20)      396 2024-04-03 19:45:08.000000 django-multisite2-2.0.1/multisite/models/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)     5465 2024-04-03 19:45:08.000000 django-multisite2-2.0.1/multisite/models/__pycache__/alias.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)     9760 2024-04-03 19:45:08.000000 django-multisite2-2.0.1/multisite/models/__pycache__/managers.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)     1938 2024-04-03 19:45:08.000000 django-multisite2-2.0.1/multisite/models/__pycache__/signals.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)      721 2024-04-03 19:45:08.000000 django-multisite2-2.0.1/multisite/models/__pycache__/validators.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)     3692 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/models/alias.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6929 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/models/managers.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1540 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/models/signals.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      380 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/models/validators.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-05 18:56:15.155185 django-multisite2-2.0.1/multisite/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-05 18:56:15.156141 django-multisite2-2.0.1/multisite/tests/__pycache__/
+-rw-r--r--   0 erikvw     (501) staff       (20)      174 2024-04-03 20:27:43.000000 django-multisite2-2.0.1/multisite/tests/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)      564 2024-04-03 20:27:43.000000 django-multisite2-2.0.1/multisite/tests/__pycache__/get_test_allowed_hosts.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)      800 2024-04-03 20:27:43.000000 django-multisite2-2.0.1/multisite/tests/__pycache__/get_test_http_response.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)      712 2024-04-03 20:27:43.000000 django-multisite2-2.0.1/multisite/tests/__pycache__/test_settings.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)      400 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/tests/get_test_allowed_hosts.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      329 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/tests/get_test_http_response.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1212 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/tests/hosts.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      575 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/tests/test_settings.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-05 18:56:15.158252 django-multisite2-2.0.1/multisite/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/tests/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-05 18:56:15.160544 django-multisite2-2.0.1/multisite/tests/tests/__pycache__/
+-rw-r--r--   0 erikvw     (501) staff       (20)      180 2024-04-03 20:27:43.000000 django-multisite2-2.0.1/multisite/tests/tests/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)     1006 2024-04-03 20:27:43.000000 django-multisite2-2.0.1/multisite/tests/tests/__pycache__/request_factory.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)    15510 2024-04-03 20:27:43.000000 django-multisite2-2.0.1/multisite/tests/tests/__pycache__/test_alias.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)     1720 2024-04-03 20:27:43.000000 django-multisite2-2.0.1/multisite/tests/tests/__pycache__/test_contrib_site.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)    12540 2024-04-03 20:27:43.000000 django-multisite2-2.0.1/multisite/tests/tests/__pycache__/test_cookie_domain_middleware.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)    18990 2024-04-03 20:27:43.000000 django-multisite2-2.0.1/multisite/tests/tests/__pycache__/test_dynamic_site_middleware.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)    10181 2024-04-03 20:27:43.000000 django-multisite2-2.0.1/multisite/tests/tests/__pycache__/test_site_cache.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)     2201 2024-04-03 20:27:43.000000 django-multisite2-2.0.1/multisite/tests/tests/__pycache__/test_site_domain.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)     7205 2024-04-03 20:28:31.000000 django-multisite2-2.0.1/multisite/tests/tests/__pycache__/test_site_id.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)     3636 2024-04-03 20:27:43.000000 django-multisite2-2.0.1/multisite/tests/tests/__pycache__/test_template_loader.cpython-312.pyc
+-rw-r--r--   0 erikvw     (501) staff       (20)      381 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/tests/tests/request_factory.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    10544 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/tests/tests/test_alias.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      638 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/tests/tests/test_contrib_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9193 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/tests/tests/test_cookie_domain_middleware.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    10931 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/tests/tests/test_dynamic_site_middleware.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5139 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/tests/tests/test_site_cache.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      923 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/tests/tests/test_site_domain.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2945 2024-04-05 18:53:41.000000 django-multisite2-2.0.1/multisite/tests/tests/test_site_id.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1798 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite/tests/tests/test_template_loader.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4309 2024-04-05 18:53:41.000000 django-multisite2-2.0.1/multisite/threadlocals.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5544 2024-03-31 01:58:23.000000 django-multisite2-2.0.1/multisite/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-05 18:56:15.161130 django-multisite2-2.0.1/multisite_app/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite_app/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      149 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite_app/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      129 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite_app/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      217 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/multisite_app/views.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      605 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)      640 2024-03-31 01:57:24.000000 django-multisite2-2.0.1/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1328 2024-04-05 18:56:15.162197 django-multisite2-2.0.1/setup.cfg
```

### Comparing `django-multisite2-2.0.0/.github/workflows/build.yml` & `django-multisite2-2.0.1/.github/workflows/build.yml`

 * *Files 5% similar despite different names*

```diff
@@ -64,11 +64,12 @@
 
       - name: Tox tests
         run: |
           tox -v
         env:
           DJANGO: ${{ matrix.django-version }}
 
-      - name: Upload coverage to Codecov
-        uses: codecov/codecov-action@v3
+      - name: Upload coverage reports to Codecov
+        uses: codecov/codecov-action@v4.0.1
         with:
-          name: Python ${{ matrix.python-version }}
+          token: ${{ secrets.CODECOV_TOKEN }}
+          slug: erikvw/django-multisite2
```

### Comparing `django-multisite2-2.0.0/.pre-commit-config.yaml` & `django-multisite2-2.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/CHANGES` & `django-multisite2-2.0.1/CHANGES`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =============
 Release Notes
 =============
 
+2.0.1
+-----
+- change from ValueError to multisite specific exceptions
+  when getting default SITE_ID in development mode.
+- add typing hints
+
 2.0.0
 -----
  - major refactor, drop support for lower than py 3.11 and DJ4.2
  - drop pytest, use unitests / runtests.py 
  - replace rel.to with related_model (Django 4.2)
  - remove deprecated `process_requests`
  - add more specific exception handling
```

### Comparing `django-multisite2-2.0.0/LICENSE` & `django-multisite2-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/PKG-INFO` & `django-multisite2-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-multisite2
-Version: 2.0.0
+Version: 2.0.1
 Summary: Serve multiple sites from a single Django application
 Home-page: http://github.com/erikvw/django-multisite
 Author: Leonid S Shestera
 Author-email: leonid@shestera.ru
 Maintainer: Ecometrica
 Maintainer-email: dev@ecometrica.com
 Classifier: Development Status :: 4 - Beta
@@ -21,15 +21,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: tldextract
 
- |actions| |codecov| |downloads| |maintainability| |black|
+|pypi| |actions| |codecov| |downloads| |maintainability| |black|
 
 
 
 README
 ======
 
 Python 3.11+ Django 4.2+
@@ -42,15 +42,15 @@
 Installation
 ============
 
 Install with pip:
 
 .. code-block::
 
-    pip install django-multisite2 (no release yet)
+    pip install django-multisite2
 
 
 Replace your ``SITE_ID`` in ``settings.py`` to:
 
 .. code-block::
 
     from multisite import SiteID
@@ -125,14 +125,17 @@
     # Keyword arguments for the MULTISITE_FALLBACK view.
     # Default: {}
     MULTISITE_FALLBACK_KWARGS = {'url': 'http://example.com/',
                                  'permanent': False}
 
 Templates
 ---------
+
+This feature has been removed in version 2.0.0.
+
 If required, create template subdirectories for domain level templates (in a
 location specified in settings.TEMPLATES['DIRS'].
 
 Multisite's template loader will look for templates in folders with the names of
 domains, such as::
 
     templates/example.com
```

### Comparing `django-multisite2-2.0.0/README.rst` & `django-multisite2-2.0.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
- |actions| |codecov| |downloads| |maintainability| |black|
+|pypi| |actions| |codecov| |downloads| |maintainability| |black|
 
 
 
 README
 ======
 
 Python 3.11+ Django 4.2+
@@ -15,15 +15,15 @@
 Installation
 ============
 
 Install with pip:
 
 .. code-block::
 
-    pip install django-multisite2 (no release yet)
+    pip install django-multisite2
 
 
 Replace your ``SITE_ID`` in ``settings.py`` to:
 
 .. code-block::
 
     from multisite import SiteID
@@ -98,14 +98,17 @@
     # Keyword arguments for the MULTISITE_FALLBACK view.
     # Default: {}
     MULTISITE_FALLBACK_KWARGS = {'url': 'http://example.com/',
                                  'permanent': False}
 
 Templates
 ---------
+
+This feature has been removed in version 2.0.0.
+
 If required, create template subdirectories for domain level templates (in a
 location specified in settings.TEMPLATES['DIRS'].
 
 Multisite's template loader will look for templates in folders with the names of
 domains, such as::
 
     templates/example.com
```

### Comparing `django-multisite2-2.0.0/django_multisite2.egg-info/PKG-INFO` & `django-multisite2-2.0.1/django_multisite2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-multisite2
-Version: 2.0.0
+Version: 2.0.1
 Summary: Serve multiple sites from a single Django application
 Home-page: http://github.com/erikvw/django-multisite
 Author: Leonid S Shestera
 Author-email: leonid@shestera.ru
 Maintainer: Ecometrica
 Maintainer-email: dev@ecometrica.com
 Classifier: Development Status :: 4 - Beta
@@ -21,15 +21,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: tldextract
 
- |actions| |codecov| |downloads| |maintainability| |black|
+|pypi| |actions| |codecov| |downloads| |maintainability| |black|
 
 
 
 README
 ======
 
 Python 3.11+ Django 4.2+
@@ -42,15 +42,15 @@
 Installation
 ============
 
 Install with pip:
 
 .. code-block::
 
-    pip install django-multisite2 (no release yet)
+    pip install django-multisite2
 
 
 Replace your ``SITE_ID`` in ``settings.py`` to:
 
 .. code-block::
 
     from multisite import SiteID
@@ -125,14 +125,17 @@
     # Keyword arguments for the MULTISITE_FALLBACK view.
     # Default: {}
     MULTISITE_FALLBACK_KWARGS = {'url': 'http://example.com/',
                                  'permanent': False}
 
 Templates
 ---------
+
+This feature has been removed in version 2.0.0.
+
 If required, create template subdirectories for domain level templates (in a
 location specified in settings.TEMPLATES['DIRS'].
 
 Multisite's template loader will look for templates in folders with the names of
 domains, such as::
 
     templates/example.com
```

### Comparing `django-multisite2-2.0.0/multisite/admin/alias_admin.py` & `django-multisite2-2.0.1/multisite/admin/alias_admin.py`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/multisite/admin/multisite_changelist.py` & `django-multisite2-2.0.1/multisite/admin/multisite_changelist.py`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/multisite/admin/multisite_model_admin.py` & `django-multisite2-2.0.1/multisite/admin/multisite_model_admin.py`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/multisite/apps.py` & `django-multisite2-2.0.1/multisite/apps.py`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/multisite/exceptions.py` & `django-multisite2-2.0.1/multisite/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,18 @@
     pass
 
 
 class MultisiteSiteDoesNotExist(Exception):
     pass
 
 
+class MultisiteAliasDoesNotExist(Exception):
+    pass
+
+
 class MultisiteCacheError(Exception):
     pass
 
 
 class MultisiteFallbackError(Exception):
     pass
```

### Comparing `django-multisite2-2.0.0/multisite/forms.py` & `django-multisite2-2.0.1/multisite/forms.py`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/multisite/hacks.py` & `django-multisite2-2.0.1/multisite/hacks.py`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/multisite/management/commands/update_public_suffix_list.py` & `django-multisite2-2.0.1/multisite/management/commands/update_public_suffix_list.py`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/multisite/middleware/cookie_domain_middleware.py` & `django-multisite2-2.0.1/multisite/middleware/cookie_domain_middleware.py`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/multisite/middleware/dynamic_site_middleware.py` & `django-multisite2-2.0.1/multisite/middleware/dynamic_site_middleware.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 from hashlib import md5 as md5_constructor
 from urllib.parse import urlsplit, urlunsplit
 
 from django.conf import settings
 from django.contrib.sites.models import SITE_CACHE, Site
 from django.core import mail
 from django.core.cache import caches
-from django.core.exceptions import DisallowedHost
+from django.core.exceptions import DisallowedHost, ObjectDoesNotExist
 from django.db.models.signals import post_delete, post_init, pre_save
 from django.http import HttpResponse, HttpResponsePermanentRedirect
 
 from ..exceptions import (
+    MultisiteAliasDoesNotExist,
     MultisiteError,
     MultisiteInvalidHostError,
     debug_check_status_code,
     debug_raise_cache_missed_exception,
     debug_raise_disallowed_host_exception,
 )
 from ..models import Alias
@@ -166,19 +167,24 @@
         # When using runserver, assume that host will only have one path
         # component. This covers 'localhost' and your machine name.
         is_local_debug = settings.DEBUG and len(netloc.split(".")) == 1
         if is_testserver or is_local_debug:
             try:
                 # Prefer the default SITE_ID
                 site_id = settings.SITE_ID.get_default()
-            except ValueError:
+            except MultisiteError:
                 # Fallback to the first Site object
                 alias = Alias.canonical.order_by("site")[0]
             else:
-                alias = Alias.canonical.get(site=site_id)
+                try:
+                    alias = Alias.canonical.get(site=site_id)
+                except ObjectDoesNotExist as e:
+                    raise MultisiteAliasDoesNotExist(
+                        f"Invalid default SITE_ID. See {settings}. Got `{e}` for SITE_ID=`{site_id}`."
+                    )
         return alias
 
     @classmethod
     def site_domain_cache_hook(cls, sender, instance, *args, **kwargs):
         """Caches `Site.domain` in the object for
         site_domain_changed_hook.
         """
```

### Comparing `django-multisite2-2.0.0/multisite/migrations/0001_initial.py` & `django-multisite2-2.0.1/multisite/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/multisite/migrations/0002_alter_alias_id_alter_alias_is_canonical.py` & `django-multisite2-2.0.1/multisite/migrations/0002_alter_alias_id_alter_alias_is_canonical.py`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/multisite/migrations/0003_alter_alias_options_alter_alias_unique_together_and_more.py` & `django-multisite2-2.0.1/multisite/migrations/0003_alter_alias_options_alter_alias_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/multisite/migrations/0004_alter_alias_managers.py` & `django-multisite2-2.0.1/multisite/migrations/0004_alter_alias_managers.py`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/multisite/models/alias.py` & `django-multisite2-2.0.1/multisite/models/alias.py`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/multisite/models/managers.py` & `django-multisite2-2.0.1/multisite/models/managers.py`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/multisite/models/signals.py` & `django-multisite2-2.0.1/multisite/models/signals.py`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/multisite/tests/hosts.py` & `django-multisite2-2.0.1/multisite/tests/hosts.py`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/multisite/tests/test_settings.py` & `django-multisite2-2.0.1/multisite/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/multisite/tests/tests/test_alias.py` & `django-multisite2-2.0.1/multisite/tests/tests/test_alias.py`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/multisite/tests/tests/test_contrib_site.py` & `django-multisite2-2.0.1/multisite/tests/tests/test_contrib_site.py`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/multisite/tests/tests/test_cookie_domain_middleware.py` & `django-multisite2-2.0.1/multisite/tests/tests/test_cookie_domain_middleware.py`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/multisite/tests/tests/test_dynamic_site_middleware.py` & `django-multisite2-2.0.1/multisite/tests/tests/test_dynamic_site_middleware.py`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/multisite/tests/tests/test_site_cache.py` & `django-multisite2-2.0.1/multisite/tests/tests/test_site_cache.py`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/multisite/tests/tests/test_site_domain.py` & `django-multisite2-2.0.1/multisite/tests/tests/test_site_domain.py`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/multisite/tests/tests/test_site_id.py` & `django-multisite2-2.0.1/multisite/tests/tests/test_site_id.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from django.contrib.sites.models import Site
 from django.test import TestCase
 
 from multisite import SiteID
+from multisite.exceptions import MultisiteError
 
 
 class TestSiteID(TestCase):
     def setUp(self):
         Site.objects.all().delete()
         self.site = Site.objects.create(domain="example.com")
         self.site_id = SiteID()
 
     def test_invalid_default(self):
-        self.assertRaises(ValueError, SiteID, default="a")
-        self.assertRaises(ValueError, SiteID, default=self.site_id)
+        self.assertRaises(MultisiteError, SiteID, default="a")
+        self.assertRaises(MultisiteError, SiteID, default=self.site_id)
 
     def test_compare_default_site_id(self):
         self.site_id = SiteID(default=self.site.id)
         self.assertEqual(self.site_id, self.site.id)
         self.assertFalse(self.site_id != self.site.id)
         self.assertFalse(self.site_id < self.site.id)
         self.assertTrue(self.site_id <= self.site.id)
```

### Comparing `django-multisite2-2.0.0/multisite/tests/tests/test_template_loader.py` & `django-multisite2-2.0.1/multisite/tests/tests/test_template_loader.py`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/multisite/threadlocals.py` & `django-multisite2-2.0.1/multisite/threadlocals.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 from contextlib import contextmanager
 from threading import local
 
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 
+from multisite.exceptions import MultisiteError
+
 
 class SiteID(local):
     """
     Dynamic settings.SITE_ID replacement, which acts like an integer.
 
     django.contrib.sites can allow multiple Django sites to share the
     same database. However, they cannot share the same code by
     default.
 
     SiteID can be used to replace the static settings.SITE_ID integer
     when combined with the appropriate middleware.
     """
 
-    def __init__(self, default=None, *args, **kwargs):
+    def __init__(self, default: int | None = None, *args, **kwargs):
         """
         ``default``, if specified, determines the default SITE_ID,
         if that is unset.
         """
         if default is not None and not isinstance(default, int):
-            raise ValueError("%r is not a valid default." % default)
+            raise MultisiteError(
+                f"Invalid default value for SITE_ID. See settings.SITE_ID. Got `{default}`."
+            )
         self.default = default
         self.reset()
 
     def __repr__(self):
         return repr(self.__int__())
 
     def __str__(self):
@@ -96,15 +100,15 @@
 
     def reset(self):
         self.site_id = None
 
     def get_default(self):
         """Returns the default SITE_ID."""
         if self.default is None:
-            raise ValueError("SITE_ID has not been set.")
+            raise MultisiteError("SITE_ID default has not been set. See settings.SITE_ID.")
         return self.default
 
 
 class SiteDomain(SiteID):
     def __init__(self, default, *args, **kwargs):
         """
         ``default`` is the default domain name, resolved to SITE_ID, if
```

### Comparing `django-multisite2-2.0.0/multisite/utils.py` & `django-multisite2-2.0.1/multisite/utils.py`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/pyproject.toml` & `django-multisite2-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/runtests.py` & `django-multisite2-2.0.1/runtests.py`

 * *Files identical despite different names*

### Comparing `django-multisite2-2.0.0/setup.cfg` & `django-multisite2-2.0.1/setup.cfg`

 * *Files identical despite different names*

