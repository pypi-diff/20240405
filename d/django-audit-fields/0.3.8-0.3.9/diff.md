# Comparing `tmp/django-audit-fields-0.3.8.tar.gz` & `tmp/django-audit-fields-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-audit-fields-0.3.8.tar", last modified: Wed Aug 10 01:20:41 2022, max compression
+gzip compressed data, was "django-audit-fields-0.3.9.tar", last modified: Thu Aug 11 22:47:39 2022, max compression
```

## Comparing `django-audit-fields-0.3.8.tar` & `django-audit-fields-0.3.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 01:20:41.083668 django-audit-fields-0.3.8/
--rw-r--r--   0 erikvw     (501) staff       (20)       83 2020-03-04 23:22:52.000000 django-audit-fields-0.3.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-06-01 12:42:06.000000 django-audit-fields-0.3.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 01:20:41.077032 django-audit-fields-0.3.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 01:20:41.080262 django-audit-fields-0.3.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1934 2022-08-10 01:20:33.000000 django-audit-fields-0.3.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1259 2022-06-01 12:42:06.000000 django-audit-fields-0.3.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-08-10 01:20:33.000000 django-audit-fields-0.3.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 01:20:33.000000 django-audit-fields-0.3.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)       38 2020-03-04 23:22:52.000000 django-audit-fields-0.3.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)      253 2022-06-01 12:42:06.000000 django-audit-fields-0.3.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2020-03-04 23:22:42.000000 django-audit-fields-0.3.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 12:42:06.000000 django-audit-fields-0.3.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     3532 2022-08-10 01:20:41.083789 django-audit-fields-0.3.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     2504 2022-06-01 12:42:06.000000 django-audit-fields-0.3.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-10 01:20:33.000000 django-audit-fields-0.3.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-10 01:20:33.000000 django-audit-fields-0.3.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 01:20:41.081201 django-audit-fields-0.3.8/django_audit_fields/
--rw-r--r--   0 erikvw     (501) staff       (20)      225 2022-06-01 12:42:06.000000 django-audit-fields-0.3.8/django_audit_fields/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1274 2022-08-10 01:20:33.000000 django-audit-fields-0.3.8/django_audit_fields/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      122 2022-06-01 12:24:57.000000 django-audit-fields-0.3.8/django_audit_fields/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      318 2022-08-10 01:20:33.000000 django-audit-fields-0.3.8/django_audit_fields/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 01:20:41.082652 django-audit-fields-0.3.8/django_audit_fields/fields/
--rw-r--r--   0 erikvw     (501) staff       (20)      167 2020-03-04 23:22:52.000000 django-audit-fields-0.3.8/django_audit_fields/fields/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      556 2022-06-01 12:42:06.000000 django-audit-fields-0.3.8/django_audit_fields/fields/hostname_modification_field.py
--rw-r--r--   0 erikvw     (501) staff       (20)      840 2022-06-01 12:42:06.000000 django-audit-fields-0.3.8/django_audit_fields/fields/userfield.py
--rw-r--r--   0 erikvw     (501) staff       (20)      550 2022-06-01 12:42:06.000000 django-audit-fields-0.3.8/django_audit_fields/fields/uuid_auto_field.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 01:20:41.083107 django-audit-fields-0.3.8/django_audit_fields/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      119 2020-03-04 23:22:52.000000 django-audit-fields-0.3.8/django_audit_fields/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3052 2022-08-10 01:20:33.000000 django-audit-fields-0.3.8/django_audit_fields/models/audit_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      496 2020-03-04 23:22:52.000000 django-audit-fields-0.3.8/django_audit_fields/models/audit_uuid_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      319 2022-06-01 12:42:06.000000 django-audit-fields-0.3.8/django_audit_fields/stubs.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 01:20:41.083547 django-audit-fields-0.3.8/django_audit_fields/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:22:52.000000 django-audit-fields-0.3.8/django_audit_fields/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      441 2022-06-01 12:42:06.000000 django-audit-fields-0.3.8/django_audit_fields/tests/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3431 2022-06-01 12:42:06.000000 django-audit-fields-0.3.8/django_audit_fields/tests/test_fields.py
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-06-01 12:25:12.000000 django-audit-fields-0.3.8/django_audit_fields/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 01:20:41.082066 django-audit-fields-0.3.8/django_audit_fields.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     3532 2022-08-10 01:20:41.000000 django-audit-fields-0.3.8/django_audit_fields.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1075 2022-08-10 01:20:41.000000 django-audit-fields-0.3.8/django_audit_fields.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-10 01:20:41.000000 django-audit-fields-0.3.8/django_audit_fields.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-06-01 12:47:38.000000 django-audit-fields-0.3.8/django_audit_fields.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-08-10 01:20:41.000000 django-audit-fields-0.3.8/django_audit_fields.egg-info/requires.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       20 2022-08-10 01:20:41.000000 django-audit-fields-0.3.8/django_audit_fields.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1740 2022-08-10 01:20:33.000000 django-audit-fields-0.3.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1124 2022-06-01 12:42:06.000000 django-audit-fields-0.3.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1330 2022-08-10 01:20:41.084115 django-audit-fields-0.3.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 22:47:39.984095 django-audit-fields-0.3.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)       83 2020-03-04 23:22:52.000000 django-audit-fields-0.3.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-06-01 12:42:06.000000 django-audit-fields-0.3.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 22:47:39.977004 django-audit-fields-0.3.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 22:47:39.980728 django-audit-fields-0.3.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1934 2022-08-10 01:20:33.000000 django-audit-fields-0.3.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1259 2022-06-01 12:42:06.000000 django-audit-fields-0.3.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-08-10 01:20:33.000000 django-audit-fields-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 01:20:33.000000 django-audit-fields-0.3.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)       38 2020-03-04 23:22:52.000000 django-audit-fields-0.3.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)      433 2022-08-11 22:47:30.000000 django-audit-fields-0.3.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2020-03-04 23:22:42.000000 django-audit-fields-0.3.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 12:42:06.000000 django-audit-fields-0.3.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     3532 2022-08-11 22:47:39.984197 django-audit-fields-0.3.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     2504 2022-06-01 12:42:06.000000 django-audit-fields-0.3.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-11 22:47:30.000000 django-audit-fields-0.3.9/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-10 01:20:33.000000 django-audit-fields-0.3.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 22:47:39.981720 django-audit-fields-0.3.9/django_audit_fields/
+-rw-r--r--   0 erikvw     (501) staff       (20)      225 2022-06-01 12:42:06.000000 django-audit-fields-0.3.9/django_audit_fields/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1810 2022-08-11 22:47:30.000000 django-audit-fields-0.3.9/django_audit_fields/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      122 2022-06-01 12:24:57.000000 django-audit-fields-0.3.9/django_audit_fields/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      318 2022-08-10 01:20:33.000000 django-audit-fields-0.3.9/django_audit_fields/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 22:47:39.983152 django-audit-fields-0.3.9/django_audit_fields/fields/
+-rw-r--r--   0 erikvw     (501) staff       (20)      167 2020-03-04 23:22:52.000000 django-audit-fields-0.3.9/django_audit_fields/fields/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      556 2022-06-01 12:42:06.000000 django-audit-fields-0.3.9/django_audit_fields/fields/hostname_modification_field.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      840 2022-06-01 12:42:06.000000 django-audit-fields-0.3.9/django_audit_fields/fields/userfield.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      550 2022-06-01 12:42:06.000000 django-audit-fields-0.3.9/django_audit_fields/fields/uuid_auto_field.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 22:47:39.983649 django-audit-fields-0.3.9/django_audit_fields/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      119 2020-03-04 23:22:52.000000 django-audit-fields-0.3.9/django_audit_fields/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3052 2022-08-10 01:20:33.000000 django-audit-fields-0.3.9/django_audit_fields/models/audit_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      496 2020-03-04 23:22:52.000000 django-audit-fields-0.3.9/django_audit_fields/models/audit_uuid_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      319 2022-06-01 12:42:06.000000 django-audit-fields-0.3.9/django_audit_fields/stubs.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 22:47:39.983976 django-audit-fields-0.3.9/django_audit_fields/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:22:52.000000 django-audit-fields-0.3.9/django_audit_fields/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      441 2022-06-01 12:42:06.000000 django-audit-fields-0.3.9/django_audit_fields/tests/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3431 2022-06-01 12:42:06.000000 django-audit-fields-0.3.9/django_audit_fields/tests/test_fields.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-06-01 12:25:12.000000 django-audit-fields-0.3.9/django_audit_fields/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 22:47:39.982547 django-audit-fields-0.3.9/django_audit_fields.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     3532 2022-08-11 22:47:39.000000 django-audit-fields-0.3.9/django_audit_fields.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1075 2022-08-11 22:47:39.000000 django-audit-fields-0.3.9/django_audit_fields.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-11 22:47:39.000000 django-audit-fields-0.3.9/django_audit_fields.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-06-01 12:47:38.000000 django-audit-fields-0.3.9/django_audit_fields.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-08-11 22:47:39.000000 django-audit-fields-0.3.9/django_audit_fields.egg-info/requires.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       20 2022-08-11 22:47:39.000000 django-audit-fields-0.3.9/django_audit_fields.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1740 2022-08-10 01:20:33.000000 django-audit-fields-0.3.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1124 2022-06-01 12:42:06.000000 django-audit-fields-0.3.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1330 2022-08-11 22:47:39.984539 django-audit-fields-0.3.9/setup.cfg
```

### Comparing `django-audit-fields-0.3.8/.github/workflows/build.yml` & `django-audit-fields-0.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `django-audit-fields-0.3.8/.gitignore` & `django-audit-fields-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `django-audit-fields-0.3.8/.pre-commit-config.yaml` & `django-audit-fields-0.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-audit-fields-0.3.8/LICENSE` & `django-audit-fields-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-audit-fields-0.3.8/PKG-INFO` & `django-audit-fields-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-audit-fields
-Version: 0.3.8
+Version: 0.3.9
 Summary: Add model fields to track creation and modification dates, users and more on save.
 Home-page: http://github.com/erikvw/django-audit-fields
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc audit field clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `django-audit-fields-0.3.8/README.rst` & `django-audit-fields-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `django-audit-fields-0.3.8/django_audit_fields/fields/hostname_modification_field.py` & `django-audit-fields-0.3.9/django_audit_fields/fields/hostname_modification_field.py`

 * *Files identical despite different names*

### Comparing `django-audit-fields-0.3.8/django_audit_fields/fields/userfield.py` & `django-audit-fields-0.3.9/django_audit_fields/fields/userfield.py`

 * *Files identical despite different names*

### Comparing `django-audit-fields-0.3.8/django_audit_fields/fields/uuid_auto_field.py` & `django-audit-fields-0.3.9/django_audit_fields/fields/uuid_auto_field.py`

 * *Files identical despite different names*

### Comparing `django-audit-fields-0.3.8/django_audit_fields/models/audit_model_mixin.py` & `django-audit-fields-0.3.9/django_audit_fields/models/audit_model_mixin.py`

 * *Files identical despite different names*

### Comparing `django-audit-fields-0.3.8/django_audit_fields/tests/test_fields.py` & `django-audit-fields-0.3.9/django_audit_fields/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `django-audit-fields-0.3.8/django_audit_fields.egg-info/PKG-INFO` & `django-audit-fields-0.3.9/django_audit_fields.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-audit-fields
-Version: 0.3.8
+Version: 0.3.9
 Summary: Add model fields to track creation and modification dates, users and more on save.
 Home-page: http://github.com/erikvw/django-audit-fields
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc audit field clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `django-audit-fields-0.3.8/django_audit_fields.egg-info/SOURCES.txt` & `django-audit-fields-0.3.9/django_audit_fields.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-audit-fields-0.3.8/pyproject.toml` & `django-audit-fields-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-audit-fields-0.3.8/runtests.py` & `django-audit-fields-0.3.9/runtests.py`

 * *Files identical despite different names*

### Comparing `django-audit-fields-0.3.8/setup.cfg` & `django-audit-fields-0.3.9/setup.cfg`

 * *Files identical despite different names*

