# Comparing `tmp/django-loose-fk-1.0.3.tar.gz` & `tmp/django-loose-fk-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-loose-fk-1.0.3.tar", last modified: Fri Jul 14 14:33:31 2023, max compression
+gzip compressed data, was "django-loose-fk-1.0.4.tar", last modified: Fri Apr  5 10:34:58 2024, max compression
```

## Comparing `django-loose-fk-1.0.3.tar` & `django-loose-fk-1.0.4.tar`

### file list

```diff
@@ -1,60 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:33:31.294602 django-loose-fk-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-07-14 14:33:31.294602 django-loose-fk-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:33:31.286602 django-loose-fk-1.0.3/django_loose_fk/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/drf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:33:31.290602 django-loose-fk-1.0.3/django_loose_fk/inspectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/inspectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/inspectors/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/inspectors/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/lookups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/query_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/virtual_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:33:31.290602 django-loose-fk-1.0.3/django_loose_fk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-07-14 14:33:31.000000 django-loose-fk-1.0.3/django_loose_fk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-14 14:33:31.000000 django-loose-fk-1.0.3/django_loose_fk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:33:31.000000 django-loose-fk-1.0.3/django_loose_fk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:33:31.000000 django-loose-fk-1.0.3/django_loose_fk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-14 14:33:31.000000 django-loose-fk-1.0.3/django_loose_fk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-14 14:33:31.000000 django-loose-fk-1.0.3/django_loose_fk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-14 14:33:31.294602 django-loose-fk-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:33:31.290602 django-loose-fk-1.0.3/testapp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/testapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/testapp/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/testapp/loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:33:31.290602 django-loose-fk-1.0.3/testapp/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/testapp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/testapp/migrations/0002_auto_20220310_1612.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/testapp/migrations/0003_auto_20230705_0917.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/testapp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/testapp/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/testapp/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/testapp/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:33:31.294602 django-loose-fk-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/test_api_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/test_chain_loose_fk.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/test_integrity.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/test_model_field_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/test_model_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/test_querying.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/test_querylist.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/test_serializer_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/test_system_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:34:58.120771 django-loose-fk-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-04-05 10:34:58.120771 django-loose-fk-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:34:58.112771 django-loose-fk-1.0.4/django_loose_fk/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/drf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:34:58.116771 django-loose-fk-1.0.4/django_loose_fk/inspectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/inspectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/inspectors/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/inspectors/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/lookups.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/query_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/django_loose_fk/virtual_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:34:58.120771 django-loose-fk-1.0.4/django_loose_fk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-04-05 10:34:58.000000 django-loose-fk-1.0.4/django_loose_fk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-05 10:34:58.000000 django-loose-fk-1.0.4/django_loose_fk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 10:34:58.000000 django-loose-fk-1.0.4/django_loose_fk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 10:34:58.000000 django-loose-fk-1.0.4/django_loose_fk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-05 10:34:58.000000 django-loose-fk-1.0.4/django_loose_fk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 10:34:58.000000 django-loose-fk-1.0.4/django_loose_fk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-05 10:34:58.120771 django-loose-fk-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:34:58.116771 django-loose-fk-1.0.4/testapp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/testapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/testapp/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/testapp/loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:34:58.116771 django-loose-fk-1.0.4/testapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/testapp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/testapp/migrations/0002_auto_20220310_1612.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/testapp/migrations/0003_auto_20230705_0917.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/testapp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/testapp/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/testapp/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/testapp/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:34:58.120771 django-loose-fk-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_api_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_chain_loose_fk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_integrity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_is_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_model_field_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_model_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_querying.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_querylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_serializer_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-05 10:34:52.000000 django-loose-fk-1.0.4/tests/test_system_checks.py
```

### Comparing `django-loose-fk-1.0.3/LICENSE` & `django-loose-fk-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.3/PKG-INFO` & `django-loose-fk-1.0.4/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,12 @@
-Metadata-Version: 2.1
-Name: django-loose-fk
-Version: 1.0.3
-Summary: Django Loose FK handles local or remote "ForeignKey" references.
-Home-page: https://github.com/maykinmedia/django-loose-fk
-Author: Maykin Media
-Author-email: support@maykinmedia.nl
-License: MIT
-Keywords: ForeignKey,URL reference,decentralization,integrity
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Provides-Extra: openapi
-Provides-Extra: tests
-Provides-Extra: pep8
-Provides-Extra: coverage
-Provides-Extra: docs
-Provides-Extra: release
-License-File: LICENSE
-
 ===============
 Django Loose FK
 ===============
 
-:Version: 1.0.3
+:Version: 1.0.4
 :Source: https://github.com/maykinmedia/django-loose-fk
 :Keywords: ``ForeignKey``, ``URL reference``, ``decentralization``, ``integrity``
 
 |build-status| |code-quality| |black| |coverage|
 
 |python-versions| |django-versions| |pypi-version|
 
@@ -150,14 +121,28 @@
 
         relation = FkOrURLField(
             fk_field="local",
             url_field="remote",
             loader=RequestsLoader()
         )
 
+Local and remote urls
+---------------------
+
+If several services are hosted within the same domain, it could be tricky to separate
+local and remote urls. In this case an additional setting ``LOOSE_FK_LOCAL_BASE_URLS`` can be used
+to define an explicit list of allowed prefixes for local urls.
+
+.. code-block:: python
+
+    LOOSE_FK_LOCAL_BASE_URLS = [
+        "https://api.example.nl/ozgv-t/zaken/",
+        "https://api.example.nl/ozgv-t/catalogi/",
+    ]
+
 
 .. |build-status| image:: https://github.com/maykinmedia/django-loose-fk/workflows/Run%20CI/badge.svg
     :alt: Build status
     :target: https://github.com/maykinmedia/django-loose-fk/actions?query=workflow%3A%22Run+CI%22
 
 .. |code-quality| image:: https://github.com/maykinmedia/django-loose-fk/workflows/Code%20quality%20checks/badge.svg
      :alt: Code quality checks
```

### Comparing `django-loose-fk-1.0.3/django_loose_fk/apps.py` & `django-loose-fk-1.0.4/django_loose_fk/apps.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.3/django_loose_fk/checks.py` & `django-loose-fk-1.0.4/django_loose_fk/checks.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.3/django_loose_fk/constraints.py` & `django-loose-fk-1.0.4/django_loose_fk/constraints.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from django.db import models
 from django.db.models.constraints import BaseConstraint
+from django.db.utils import DEFAULT_DB_ALIAS
 
 
 class FkOrURLFieldConstraint(BaseConstraint):
     """
     Wrap around models.CheckConstraint based on the field name passed in.
     """
 
@@ -31,15 +32,15 @@
                 "model_name": self.model_name,
                 "fk_field": self.fk_field,
                 "url_field": self.url_field,
             }
         )
         return (path, args, kwargs)
 
-    def _get_check_constraint(self, model, schema_editor):
+    def _get_check_constraint(self, model, schema_editor=None):
         """
         Return the underlying check constraint generated.
         """
         if not hasattr(self, "_check_constraint"):
             # URL field is empty if empty string or None
             empty_url_field = models.Q(**{self.url_field: ""})
             empty_fk_field = models.Q(**{f"{self.fk_field}__isnull": True})
@@ -62,14 +63,18 @@
         check_constraint = self._get_check_constraint(model, schema_editor)
         return check_constraint.create_sql(model, schema_editor)
 
     def remove_sql(self, model, schema_editor):
         check_constraint = self._get_check_constraint(model, schema_editor)
         return check_constraint.remove_sql(model, schema_editor)
 
+    def validate(self, model, instance, exclude=None, using=DEFAULT_DB_ALIAS):
+        check_constraint = self._get_check_constraint(model)
+        return check_constraint.validate(model, instance, exclude, using)
+
     def __repr__(self):
         return "<%s: field=%r>" % (self.__class__.__name__, self.name)
 
     def __eq__(self, other):
         if isinstance(other, FkOrURLFieldConstraint):
             return self.name == other.name
         return super().__eq__(other)
```

### Comparing `django-loose-fk-1.0.3/django_loose_fk/drf.py` & `django-loose-fk-1.0.4/django_loose_fk/drf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Django Rest Framework integration.
 
 Provides a custom field.
 """
+
 import logging
 from dataclasses import dataclass
 from typing import Tuple, Union
 from urllib.parse import ParseResult, urlparse
 
 from django.core.exceptions import ValidationError as DjangoValidationError
 from django.core.validators import URLValidator as _URLValidator
@@ -16,15 +17,15 @@
 from django.utils.translation import gettext_lazy as _
 
 from rest_framework import fields, serializers
 from rest_framework.utils.model_meta import get_field_info
 
 from .fields import FkOrURLField, InstanceOrUrl
 from .loaders import FetchError, FetchJsonError
-from .utils import get_resource_for_path
+from .utils import get_resource_for_path, is_local
 
 logger = logging.getLogger(__name__)
 
 
 # django tests use testserver host, but that doesn't pass core URLValidation
 # regex...
 class URLValidator(_URLValidator):
@@ -41,16 +42,16 @@
     """
 
     model: ModelBase
     field: FkOrURLField
 
     def resolve(self, host: str, url: str) -> models.Model:
         parsed = urlparse(url)
-        is_local = parsed.netloc == host
-        return self.resolve_local(parsed) if is_local else self.resolve_remote(url)
+        local = is_local(host, url)
+        return self.resolve_local(parsed) if local else self.resolve_remote(url)
 
     def resolve_local(self, parsed: ParseResult) -> models.Model:
         return get_resource_for_path(parsed.path)
 
     def resolve_remote(self, url: str) -> models.Model:
         # load the remote object
         instance = self.model(**{self.field.name: url})
```

### Comparing `django-loose-fk-1.0.3/django_loose_fk/fields.py` & `django-loose-fk-1.0.4/django_loose_fk/fields.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.3/django_loose_fk/filters.py` & `django-loose-fk-1.0.4/django_loose_fk/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 Filter support for django-filter.
 """
+
 import logging
-from functools import reduce
 from urllib.parse import urlparse
 
 from django import forms
 from django.db.models import Q
 
 import django_filters
 from django_filters.filterset import FilterSet, remote_queryset as _remote_queryset
 
 from .fields import FkOrURLField
-from .utils import get_resource_for_path, get_subclasses
+from .utils import get_resource_for_path, get_subclasses, is_local
 
 logger = logging.getLogger(__name__)
 
 
 def remote_queryset(field: FkOrURLField):
     fk_field = field._fk_field
     return _remote_queryset(fk_field)
@@ -70,15 +70,15 @@
 
     def get_filters(self, model_field, parsed_values, host) -> dict:
         local_filter_key = f"{model_field.fk_field}__{self.lookup_expr}"
         external_filter_key = f"{model_field.url_field}__{self.lookup_expr}"
 
         filters = {}
         for value in parsed_values:
-            local = value.netloc == host
+            local = is_local(host, value.geturl())
             if local:
                 local_object = get_resource_for_path(value.path)
                 if self.instance_path:
                     for bit in self.instance_path.split("."):
                         local_object = getattr(local_object, bit)
                 filter_key = local_filter_key
                 filter_value = local_object
```

### Comparing `django-loose-fk-1.0.3/django_loose_fk/inspectors/fields.py` & `django-loose-fk-1.0.4/django_loose_fk/inspectors/fields.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.3/django_loose_fk/inspectors/query.py` & `django-loose-fk-1.0.4/django_loose_fk/inspectors/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Define a query parameters inspector that can handle the custom fields.
 
 Requires drf-yasg, which can be installed as the [openapi] optional group
 dependency.
 """
+
 from django_filters.rest_framework.backends import DjangoFilterBackend
 from drf_yasg import openapi
 
 from .. import filters
 
 try:
     from vng_api_common.inspectors.query import FilterInspector as BaseFilterInspector
```

### Comparing `django-loose-fk-1.0.3/django_loose_fk/loaders.py` & `django-loose-fk-1.0.4/django_loose_fk/loaders.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,22 +42,27 @@
 
         Validation if a URL is local is done by looking at the host and
         comparing it against the ALLOWED_HOSTS setting, as Django serves
         those domains.
         """
         allowed_hosts = settings.ALLOWED_HOSTS
         parsed = urlparse(url)
+        local_base_urls = getattr(settings, "LOOSE_FK_LOCAL_BASE_URLS", [])
 
         if any(pattern == "*" for pattern in allowed_hosts):
             warnings.warn(
                 "You have wildcards in your ALLOWED_HOSTS setting - "
                 "this will cause all remote URLs to be considered local URLs and "
                 "break django-loose-fk's behaviour. You should use an explicit list.",
                 RuntimeWarning,
             )
+            return validate_host(parsed.netloc, allowed_hosts)
+
+        if local_base_urls:
+            return any(url.startswith(base_url) for base_url in local_base_urls)
 
         return validate_host(parsed.netloc, allowed_hosts)
 
     def load_local_object(self, url: str, model: ModelBase) -> models.Model:
         parsed = urlparse(url)
         return get_resource_for_path(parsed.path)
```

### Comparing `django-loose-fk-1.0.3/django_loose_fk/lookups.py` & `django-loose-fk-1.0.4/django_loose_fk/lookups.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,14 +112,22 @@
 
         return url_rhs_sql, url_rhs_params, fk_rhs_sql, fk_rhs_params
 
     def get_prep_lookup(self):
         if self.rhs_is_direct_value():
             # If we get here, we are dealing with single-column relations.
             self.rhs = [get_normalized_value(val)[0] for val in self.rhs]
+
+        else:
+            # we're dealing with something that can be expressed as SQL -> it's local only!
+            target = self.lhs.target
+            db_table = target.model._meta.db_table
+            fk_lhs = target._fk_field.get_col(db_table)
+            target_field = fk_lhs.target.target_field.name
+            self.rhs.set_values([target_field])
         return super().get_prep_lookup()
 
     def as_sql(self, compiler, connection):
         # TODO: support connection.ops.max_in_list_size()
         url_lhs_sql, url_params, fk_lhs_sql, fk_params = self.process_lhs(
             compiler, connection
         )
```

### Comparing `django-loose-fk-1.0.3/django_loose_fk/query_list.py` & `django-loose-fk-1.0.4/django_loose_fk/query_list.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.3/django_loose_fk/utils.py` & `django-loose-fk-1.0.4/django_loose_fk/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,33 @@
+from urllib.parse import urlparse
+
 from django.conf import settings
 from django.db import models
 from django.http import HttpRequest
 from django.urls import Resolver404, get_resolver, get_script_prefix
 
 from rest_framework import viewsets
 from rest_framework.request import Request
 
 
+def is_local(host: str, url: str) -> bool:
+    """
+    Define if the url is local or external based on LOOSE_FK_LOCAL_BASE_URLS
+    setting or a host
+    """
+    parsed = urlparse(url)
+    local_base_urls = getattr(settings, "LOOSE_FK_LOCAL_BASE_URLS", [])
+    # if local base urls are defined - use them
+    if local_base_urls:
+        return any(url.startswith(base_url) for base_url in local_base_urls)
+
+        # otherwise use hostname
+    return parsed.netloc == host
+
+
 def get_viewset_for_path(path: str) -> viewsets.ViewSet:
     """
     Look up which viewset matches a path.
     """
     # NOTE: this doesn't support setting a different urlconf on the request
     resolver = get_resolver()
     try:
```

### Comparing `django-loose-fk-1.0.3/django_loose_fk/virtual_models.py` & `django-loose-fk-1.0.4/django_loose_fk/virtual_models.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.3/django_loose_fk.egg-info/PKG-INFO` & `django-loose-fk-1.0.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-loose-fk
-Version: 1.0.3
+Version: 1.0.4
 Summary: Django Loose FK handles local or remote "ForeignKey" references.
 Home-page: https://github.com/maykinmedia/django-loose-fk
 Author: Maykin Media
 Author-email: support@maykinmedia.nl
 License: MIT
 Keywords: ForeignKey,URL reference,decentralization,integrity
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,27 +15,45 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+Requires-Dist: django>=3.2
+Requires-Dist: djangorestframework>=3.11.0
+Requires-Dist: django-filter
+Requires-Dist: coreapi
 Provides-Extra: openapi
+Requires-Dist: drf-yasg; extra == "openapi"
 Provides-Extra: tests
+Requires-Dist: psycopg2; extra == "tests"
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-django; extra == "tests"
+Requires-Dist: tox; extra == "tests"
+Requires-Dist: black; extra == "tests"
+Requires-Dist: isort; extra == "tests"
+Requires-Dist: requests; extra == "tests"
+Requires-Dist: requests-mock; extra == "tests"
 Provides-Extra: pep8
+Requires-Dist: flake8; extra == "pep8"
 Provides-Extra: coverage
+Requires-Dist: pytest-cov; extra == "coverage"
 Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Provides-Extra: release
-License-File: LICENSE
+Requires-Dist: bump2version; extra == "release"
 
 ===============
 Django Loose FK
 ===============
 
-:Version: 1.0.3
+:Version: 1.0.4
 :Source: https://github.com/maykinmedia/django-loose-fk
 :Keywords: ``ForeignKey``, ``URL reference``, ``decentralization``, ``integrity``
 
 |build-status| |code-quality| |black| |coverage|
 
 |python-versions| |django-versions| |pypi-version|
 
@@ -150,14 +168,28 @@
 
         relation = FkOrURLField(
             fk_field="local",
             url_field="remote",
             loader=RequestsLoader()
         )
 
+Local and remote urls
+---------------------
+
+If several services are hosted within the same domain, it could be tricky to separate
+local and remote urls. In this case an additional setting ``LOOSE_FK_LOCAL_BASE_URLS`` can be used
+to define an explicit list of allowed prefixes for local urls.
+
+.. code-block:: python
+
+    LOOSE_FK_LOCAL_BASE_URLS = [
+        "https://api.example.nl/ozgv-t/zaken/",
+        "https://api.example.nl/ozgv-t/catalogi/",
+    ]
+
 
 .. |build-status| image:: https://github.com/maykinmedia/django-loose-fk/workflows/Run%20CI/badge.svg
     :alt: Build status
     :target: https://github.com/maykinmedia/django-loose-fk/actions?query=workflow%3A%22Run+CI%22
 
 .. |code-quality| image:: https://github.com/maykinmedia/django-loose-fk/workflows/Code%20quality%20checks/badge.svg
      :alt: Code quality checks
```

### Comparing `django-loose-fk-1.0.3/django_loose_fk.egg-info/SOURCES.txt` & `django-loose-fk-1.0.4/django_loose_fk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 django_loose_fk/checks.py
 django_loose_fk/constraints.py
 django_loose_fk/drf.py
 django_loose_fk/fields.py
 django_loose_fk/filters.py
 django_loose_fk/loaders.py
 django_loose_fk/lookups.py
+django_loose_fk/py.typed
 django_loose_fk/query_list.py
 django_loose_fk/utils.py
 django_loose_fk/virtual_models.py
 django_loose_fk.egg-info/PKG-INFO
 django_loose_fk.egg-info/SOURCES.txt
 django_loose_fk.egg-info/dependency_links.txt
 django_loose_fk.egg-info/not-zip-safe
@@ -39,14 +40,15 @@
 tests/conftest.py
 tests/test_api.py
 tests/test_api_docs.py
 tests/test_chain_loose_fk.py
 tests/test_compare.py
 tests/test_filter.py
 tests/test_integrity.py
+tests/test_is_local.py
 tests/test_loaders.py
 tests/test_model_field_interface.py
 tests/test_model_layer.py
 tests/test_querying.py
 tests/test_querylist.py
 tests/test_serializer_field.py
 tests/test_system_checks.py
```

### Comparing `django-loose-fk-1.0.3/setup.cfg` & `django-loose-fk-1.0.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-loose-fk
-version = 1.0.3
+version = 1.0.4
 description = Django Loose FK handles local or remote "ForeignKey" references.
 long_description = file: README.rst
 url = https://github.com/maykinmedia/django-loose-fk
 license = MIT
 author = Maykin Media
 author_email = support@maykinmedia.nl
 keywords = ForeignKey, URL reference, decentralization, integrity
```

### Comparing `django-loose-fk-1.0.3/testapp/api.py` & `django-loose-fk-1.0.4/testapp/api.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.3/testapp/migrations/0001_initial.py` & `django-loose-fk-1.0.4/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.3/testapp/migrations/0002_auto_20220310_1612.py` & `django-loose-fk-1.0.4/testapp/migrations/0002_auto_20220310_1612.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.3/testapp/migrations/0003_auto_20230705_0917.py` & `django-loose-fk-1.0.4/testapp/migrations/0003_auto_20230705_0917.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.3/testapp/models.py` & `django-loose-fk-1.0.4/testapp/models.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.3/testapp/settings.py` & `django-loose-fk-1.0.4/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.3/tests/test_api.py` & `django-loose-fk-1.0.4/tests/test_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Test the API interface to handle local/remote references.
 """
+
 from unittest.mock import patch
 
 from django.test import override_settings
 
 import pytest
 import requests_mock
 from rest_framework.reverse import reverse
@@ -187,7 +188,49 @@
         url,
         {"zaaktype": f"http://testserver.com{zaaktype_path}"},
         HTTP_HOST="testserver.com",
     )
 
     assert len(response.data) == 1
     assert response.data[0]["url"] == f"http://testserver.com{zaak_url}"
+
+
+@patch("django_loose_fk.utils.get_script_prefix", return_value="/subpath/")
+@override_settings(
+    ALLOWED_HOSTS=["testserver.com"],
+    LOOSE_FK_LOCAL_BASE_URLS=["http://testserver.com/subpath/zaaktypes/"],
+)
+def test_write_local_url_with_local_base_urls(mock, api_client):
+    url = reverse("zaak-list")
+    zaaktype = ZaakType.objects.create(name="test")
+    zaaktype_url = reverse("zaaktype-detail", kwargs={"pk": zaaktype.pk})
+
+    data = {"name": "test", "zaaktype": f"http://testserver.com/subpath{zaaktype_url}"}
+
+    response = api_client.post(url, data, HTTP_HOST="testserver.com")
+
+    assert response.status_code == 201
+    zaak = Zaak.objects.get()
+    assert zaak.zaaktype == zaaktype
+
+
+@patch("django_loose_fk.utils.get_script_prefix", return_value="/subpath/")
+@override_settings(
+    ALLOWED_HOSTS=["testserver.com"],
+    LOOSE_FK_LOCAL_BASE_URLS=["http://testserver.com/subpath/zaaktypes/"],
+)
+def test_write_remote_url_with_local_base_urls(mock, api_client):
+    """
+    test that service with the same host and prefix can still be external
+    """
+    url = reverse("zaak-list")
+    zaaktype_url = "http://testserver.com/subpath/service/zaaktypes/10/"
+    data = {"name": "test", "zaaktype": zaaktype_url}
+
+    with requests_mock.Mocker() as m:
+        m.get(zaaktype_url, json={"url": zaaktype_url, "name": "test"})
+
+        response = api_client.post(url, data, HTTP_HOST="testserver.com")
+
+        assert response.status_code == 201
+        zaak = Zaak.objects.get()
+        assert zaak.zaaktype == zaaktype_url
```

### Comparing `django-loose-fk-1.0.3/tests/test_api_docs.py` & `django-loose-fk-1.0.4/tests/test_api_docs.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.3/tests/test_chain_loose_fk.py` & `django-loose-fk-1.0.4/tests/test_chain_loose_fk.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Test the API interface to handle chained local/remote references.
 """
+
 import pytest
 import requests_mock
 from rest_framework.reverse import reverse
 
 from testapp.models import ZaakObject, ZaakType
 
 pytestmark = pytest.mark.django_db()
```

### Comparing `django-loose-fk-1.0.3/tests/test_compare.py` & `django-loose-fk-1.0.4/tests/test_compare.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Test the API interface to handle comparing of loose-fk urls
 """
+
 import pytest
 import requests_mock
 
 from testapp.models import Zaak, ZaakType
 
 pytestmark = pytest.mark.django_db()
```

### Comparing `django-loose-fk-1.0.3/tests/test_filter.py` & `django-loose-fk-1.0.4/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.3/tests/test_integrity.py` & `django-loose-fk-1.0.4/tests/test_integrity.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.3/tests/test_loaders.py` & `django-loose-fk-1.0.4/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.3/tests/test_model_field_interface.py` & `django-loose-fk-1.0.4/tests/test_model_field_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Test that it's possibly to handle remote/local objects transparently.
 """
+
 import uuid
 
 import pytest
 import requests_mock
 
 from django_loose_fk.loaders import BaseLoader
 from testapp.models import B, C, TypeA, TypeB, Zaak, ZaakType
```

### Comparing `django-loose-fk-1.0.3/tests/test_querying.py` & `django-loose-fk-1.0.4/tests/test_querying.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Test the ORM queries against the virtual field.
 """
+
 import pytest
 import requests_mock
 
 from testapp.models import Zaak, ZaakType
 
 pytestmark = pytest.mark.django_db
```

### Comparing `django-loose-fk-1.0.3/tests/test_querylist.py` & `django-loose-fk-1.0.4/tests/test_querylist.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.3/tests/test_serializer_field.py` & `django-loose-fk-1.0.4/tests/test_serializer_field.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.3/tests/test_system_checks.py` & `django-loose-fk-1.0.4/tests/test_system_checks.py`

 * *Files identical despite different names*

