# Comparing `tmp/edx-when-2.4.0.tar.gz` & `tmp/edx-when-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-when-2.4.0.tar", last modified: Fri Jun 23 13:52:41 2023, max compression
+gzip compressed data, was "edx-when-2.5.0.tar", last modified: Fri Apr  5 19:27:05 2024, max compression
```

## Comparing `edx-when-2.4.0.tar` & `edx-when-2.5.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:52:41.690486 edx-when-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)       74 2023-06-23 13:52:36.000000 edx-when-2.4.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (122)     3406 2023-06-23 13:52:36.000000 edx-when-2.4.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35119 2023-06-23 13:52:36.000000 edx-when-2.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      250 2023-06-23 13:52:36.000000 edx-when-2.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7153 2023-06-23 13:52:41.690486 edx-when-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2968 2023-06-23 13:52:36.000000 edx-when-2.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:52:41.686486 edx-when-2.4.0/edx_when/
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1771 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)    19535 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      466 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     4821 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/field_data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:52:41.686486 edx-when-2.4.0/edx_when/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     3072 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     1554 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/migrations/0002_auto_20190318_1736.py
--rw-r--r--   0 runner    (1001) docker     (122)     1077 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/migrations/0003_auto_20190402_1501.py
--rw-r--r--   0 runner    (1001) docker     (122)      409 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/migrations/0004_datepolicy_rel_date.py
--rw-r--r--   0 runner    (1001) docker     (122)      794 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/migrations/0005_auto_20190911_1056.py
--rw-r--r--   0 runner    (1001) docker     (122)      397 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/migrations/0006_drop_active_index.py
--rw-r--r--   0 runner    (1001) docker     (122)      368 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/migrations/0007_meta_tweaks.py
--rw-r--r--   0 runner    (1001) docker     (122)      584 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/migrations/0008_courseversion_block_type.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6099 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:52:41.682486 edx-when-2.4.0/edx_when/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:52:41.686486 edx-when-2.4.0/edx_when/templates/edx_schedule/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/templates/edx_schedule/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)      638 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      482 2023-06-23 13:52:36.000000 edx-when-2.4.0/edx_when/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:52:41.686486 edx-when-2.4.0/edx_when.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7153 2023-06-23 13:52:41.000000 edx-when-2.4.0/edx_when.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-06-23 13:52:41.000000 edx-when-2.4.0/edx_when.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-23 13:52:41.000000 edx-when-2.4.0/edx_when.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      211 2023-06-23 13:52:41.000000 edx-when-2.4.0/edx_when.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-23 13:52:41.000000 edx-when-2.4.0/edx_when.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       91 2023-06-23 13:52:41.000000 edx-when-2.4.0/edx_when.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-23 13:52:41.000000 edx-when-2.4.0/edx_when.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:52:41.686486 edx-when-2.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      265 2023-06-23 13:52:36.000000 edx-when-2.4.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-06-23 13:52:36.000000 edx-when-2.4.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-06-23 13:52:41.690486 edx-when-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5688 2023-06-23 13:52:36.000000 edx-when-2.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:52:41.690486 edx-when-2.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    28200 2023-06-23 13:52:36.000000 edx-when-2.4.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2700 2023-06-23 13:52:36.000000 edx-when-2.4.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     5385 2023-06-23 13:52:36.000000 edx-when-2.4.0/tests/test_xblock_services.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:27:05.098078 edx-when-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-05 19:27:01.000000 edx-when-2.5.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-05 19:27:01.000000 edx-when-2.5.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35119 2024-04-05 19:27:01.000000 edx-when-2.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-05 19:27:01.000000 edx-when-2.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-04-05 19:27:05.098078 edx-when-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-05 19:27:01.000000 edx-when-2.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:27:05.094078 edx-when-2.5.0/edx_when/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-05 19:27:01.000000 edx-when-2.5.0/edx_when/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-05 19:27:01.000000 edx-when-2.5.0/edx_when/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19535 2024-04-05 19:27:01.000000 edx-when-2.5.0/edx_when/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-05 19:27:01.000000 edx-when-2.5.0/edx_when/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-04-05 19:27:01.000000 edx-when-2.5.0/edx_when/field_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:27:05.098078 edx-when-2.5.0/edx_when/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-05 19:27:01.000000 edx-when-2.5.0/edx_when/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-05 19:27:01.000000 edx-when-2.5.0/edx_when/migrations/0002_auto_20190318_1736.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-05 19:27:01.000000 edx-when-2.5.0/edx_when/migrations/0003_auto_20190402_1501.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-05 19:27:01.000000 edx-when-2.5.0/edx_when/migrations/0004_datepolicy_rel_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-05 19:27:01.000000 edx-when-2.5.0/edx_when/migrations/0005_auto_20190911_1056.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-05 19:27:01.000000 edx-when-2.5.0/edx_when/migrations/0006_drop_active_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-05 19:27:01.000000 edx-when-2.5.0/edx_when/migrations/0007_meta_tweaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-05 19:27:01.000000 edx-when-2.5.0/edx_when/migrations/0008_courseversion_block_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:27:01.000000 edx-when-2.5.0/edx_when/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-05 19:27:01.000000 edx-when-2.5.0/edx_when/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:27:05.094078 edx-when-2.5.0/edx_when/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:27:05.098078 edx-when-2.5.0/edx_when/templates/edx_schedule/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-05 19:27:01.000000 edx-when-2.5.0/edx_when/templates/edx_schedule/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-05 19:27:01.000000 edx-when-2.5.0/edx_when/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-05 19:27:01.000000 edx-when-2.5.0/edx_when/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-05 19:27:01.000000 edx-when-2.5.0/edx_when/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:27:05.098078 edx-when-2.5.0/edx_when.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-04-05 19:27:05.000000 edx-when-2.5.0/edx_when.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-05 19:27:05.000000 edx-when-2.5.0/edx_when.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:27:05.000000 edx-when-2.5.0/edx_when.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-05 19:27:05.000000 edx-when-2.5.0/edx_when.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:27:05.000000 edx-when-2.5.0/edx_when.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-05 19:27:05.000000 edx-when-2.5.0/edx_when.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 19:27:05.000000 edx-when-2.5.0/edx_when.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:27:05.098078 edx-when-2.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-05 19:27:01.000000 edx-when-2.5.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-05 19:27:01.000000 edx-when-2.5.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-05 19:27:05.098078 edx-when-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-04-05 19:27:01.000000 edx-when-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:27:05.098078 edx-when-2.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    28200 2024-04-05 19:27:01.000000 edx-when-2.5.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-05 19:27:01.000000 edx-when-2.5.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-04-05 19:27:01.000000 edx-when-2.5.0/tests/test_xblock_services.py
```

### Comparing `edx-when-2.4.0/CHANGELOG.rst` & `edx-when-2.5.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,17 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[2.5.0] - 2024-04-02
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+* Add support for Python 3.11. Dropped django32 support.
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
 [2.4.0] - 2023-06-21
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Support added for Django 4.2
```

### Comparing `edx-when-2.4.0/LICENSE.txt` & `edx-when-2.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-when-2.4.0/PKG-INFO` & `edx-when-2.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: edx-when
-Version: 2.4.0
+Version: 2.5.0
 Summary: Your project description goes here
 Home-page: https://github.com/openedx/edx-when
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: AUTHORS
+Requires-Dist: Django>=1.11
+Requires-Dist: django-model-utils
+Requires-Dist: edx-django-utils
+Requires-Dist: edx-drf-extensions
+Requires-Dist: edx-opaque-keys
+Requires-Dist: xblock
 
 edx-when
 =============================
 
 |pypi-badge| |CI| |codecov-badge| |doc-badge| |pyversions-badge|
 |license-badge|
 
@@ -60,15 +65,15 @@
 
 Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
 can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/edx-when/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 Reporting Security Issues
 -------------------------
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 Getting Help
 ------------
 
 Have a question about this repository, or about Open edX in general?  Please
 refer to this `list of resources`_ if you need any assistance.
 
@@ -112,14 +117,17 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[2.5.0] - 2024-04-02
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+* Add support for Python 3.11. Dropped django32 support.
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
 [2.4.0] - 2023-06-21
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Support added for Django 4.2
```

### Comparing `edx-when-2.4.0/README.rst` & `edx-when-2.5.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
 can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/edx-when/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 Reporting Security Issues
 -------------------------
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 Getting Help
 ------------
 
 Have a question about this repository, or about Open edX in general?  Please
 refer to this `list of resources`_ if you need any assistance.
```

### Comparing `edx-when-2.4.0/edx_when/admin.py` & `edx-when-2.5.0/edx_when/admin.py`

 * *Files identical despite different names*

### Comparing `edx-when-2.4.0/edx_when/api.py` & `edx-when-2.5.0/edx_when/api.py`

 * *Files identical despite different names*

### Comparing `edx-when-2.4.0/edx_when/field_data.py` & `edx-when-2.5.0/edx_when/field_data.py`

 * *Files identical despite different names*

### Comparing `edx-when-2.4.0/edx_when/migrations/0001_initial.py` & `edx-when-2.5.0/edx_when/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-when-2.4.0/edx_when/migrations/0002_auto_20190318_1736.py` & `edx-when-2.5.0/edx_when/migrations/0002_auto_20190318_1736.py`

 * *Files identical despite different names*

### Comparing `edx-when-2.4.0/edx_when/migrations/0003_auto_20190402_1501.py` & `edx-when-2.5.0/edx_when/migrations/0003_auto_20190402_1501.py`

 * *Files identical despite different names*

### Comparing `edx-when-2.4.0/edx_when/migrations/0005_auto_20190911_1056.py` & `edx-when-2.5.0/edx_when/migrations/0005_auto_20190911_1056.py`

 * *Files identical despite different names*

### Comparing `edx-when-2.4.0/edx_when/migrations/0008_courseversion_block_type.py` & `edx-when-2.5.0/edx_when/migrations/0008_courseversion_block_type.py`

 * *Files identical despite different names*

### Comparing `edx-when-2.4.0/edx_when/models.py` & `edx-when-2.5.0/edx_when/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         Validate data before saving.
         """
         if self.abs_date and self.rel_date:
             raise ValidationError(_("Absolute and relative dates cannot both be used"))
 
         schedule = get_schedule_for_user(self.user.id, self.content_date.course_id)  # pylint: disable=no-member
         policy_date = self.content_date.policy.actual_date(schedule=schedule)
-        if self.rel_date is not None and self.rel_date.total_seconds() < 0:
+        if self.rel_date is not None and self.rel_date.total_seconds() < 0:  # pylint: disable=no-member
             raise ValidationError(_("Override date must be later than policy date"))
         if self.abs_date is not None and isinstance(policy_date, datetime) and self.abs_date < policy_date:
             raise ValidationError(_("Override date must be later than policy date"))
 
     def __str__(self):
         """
         Get a string representation of this model instance.
```

### Comparing `edx-when-2.4.0/edx_when/templates/edx_schedule/base.html` & `edx-when-2.5.0/edx_when/templates/edx_schedule/base.html`

 * *Files identical despite different names*

### Comparing `edx-when-2.4.0/edx_when/utils.py` & `edx-when-2.5.0/edx_when/utils.py`

 * *Files identical despite different names*

### Comparing `edx-when-2.4.0/edx_when.egg-info/PKG-INFO` & `edx-when-2.5.0/edx_when.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: edx-when
-Version: 2.4.0
+Version: 2.5.0
 Summary: Your project description goes here
 Home-page: https://github.com/openedx/edx-when
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: AUTHORS
+Requires-Dist: Django>=1.11
+Requires-Dist: django-model-utils
+Requires-Dist: edx-django-utils
+Requires-Dist: edx-drf-extensions
+Requires-Dist: edx-opaque-keys
+Requires-Dist: xblock
 
 edx-when
 =============================
 
 |pypi-badge| |CI| |codecov-badge| |doc-badge| |pyversions-badge|
 |license-badge|
 
@@ -60,15 +65,15 @@
 
 Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
 can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/edx-when/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 Reporting Security Issues
 -------------------------
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 Getting Help
 ------------
 
 Have a question about this repository, or about Open edX in general?  Please
 refer to this `list of resources`_ if you need any assistance.
 
@@ -112,14 +117,17 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[2.5.0] - 2024-04-02
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+* Add support for Python 3.11. Dropped django32 support.
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
 [2.4.0] - 2023-06-21
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Support added for Django 4.2
```

### Comparing `edx-when-2.4.0/edx_when.egg-info/SOURCES.txt` & `edx-when-2.5.0/edx_when.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-when-2.4.0/requirements/constraints.txt` & `edx-when-2.5.0/requirements/constraints.txt`

 * *Files 23% similar despite different names*

```diff
@@ -12,7 +12,10 @@
 -c common_constraints.txt
 
 # diff-cover latest requires (pluggy>=0.13.1,<0.14.0)
 # which conflicts with pytest(pluggy>=0.12,<2.0.0) and tox(pluggy>0.12) both of these fetch pluggy==1.0.0
 # but diff-cover latest has a pin (pluggy<1.0.0a1)
 # Using the same version of diff-cover which is being used currently in edx-platform to avoid this conflict.
 diff-cover==4.0.0
+
+# Temporary pin.
+backports-zoneinfo==0.2.1;python_version < "3.9"
```

### Comparing `edx-when-2.4.0/setup.py` & `edx-when-2.5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -119,22 +119,21 @@
     install_requires=load_requirements('requirements/base.in'),
     license="AGPL 3.0",
     zip_safe=False,
     keywords='Django edx',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Framework :: Django',
-        'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
         'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
     ],
     entry_points={
         'lms.djangoapp': [
             "edx_when = edx_when.apps:EdxWhenConfig",
         ],
         'cms.djangoapp': [
             "edx_when = edx_when.apps:EdxWhenConfig",
```

### Comparing `edx-when-2.4.0/tests/test_api.py` & `edx-when-2.5.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `edx-when-2.4.0/tests/test_models.py` & `edx-when-2.5.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-when-2.4.0/tests/test_xblock_services.py` & `edx-when-2.5.0/tests/test_xblock_services.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,16 +64,16 @@
         dfd = field_data.DateLookupFieldData(defaults, course_id=self.course_id, use_cached=False, user=self.user)
         block = MockBlock(self.items[0][0])
 
         date = dfd.get(block, 'due')
         assert date == self.items[0][1]['due']
 
         # non-date
-        dfd.get(block, b'foo')
-        assert defaults.get.called_once_with(block.location, 'foo')
+        dfd.get(block, 'foo')
+        defaults.get.assert_called_once_with(block, 'foo')
 
         # non-existent value
         defaults.has.return_value = False
         badblock = MockBlock('foo')
         assert dfd.has(badblock, 'foo') is False
 
         # block with parent with date
@@ -96,17 +96,17 @@
         assert dfd.default(child, 'due') == self.items[0][1]['due']
         assert dfd.default(child, 'foo') is defaults.default(child, 'foo')
 
     def test_field_data_set_delete(self):
         defaults = mock.MagicMock()
         dfd = field_data.DateLookupFieldData(defaults, course_id=self.course_id, use_cached=False, user=self.user)
         dfd.set('foo', 'bar', 'x')
-        assert defaults.called_once_with('foo', 'bar', 'x')
+        defaults.set.assert_called_once_with('foo', 'bar', 'x')
         dfd.delete('baz', 'boing')
-        assert defaults.called_once_with('baz', 'boing')
+        defaults.delete.assert_called_once_with('baz', 'boing')
 
     def test_wrapped_fielddata(self):
         defaults = mock.MagicMock()
         dfd1 = field_data.DateLookupFieldData(defaults, course_id=self.course_id, use_cached=False, user=self.user)
         dfd2 = field_data.DateLookupFieldData(dfd1, course_id=self.course_id, user=self.user)
         assert dfd1._defaults == dfd2._defaults  # pylint: disable=protected-access
 
@@ -118,15 +118,15 @@
 
     def test_name(self):
         assert field_data.DateOverrideTransformer.name() == 'load_date_data'
 
     def test_collect(self):
         block_structure = mock.MagicMock()
         field_data.DateOverrideTransformer.collect(block_structure)
-        assert block_structure.request_xblock_fields.called_once_with('due', 'start')
+        block_structure.request_xblock_fields.assert_called_once_with('due', 'start', 'end')
 
     @mock.patch('edx_when.api._are_relative_dates_enabled', return_value=True)
     def test_transform(self, _mock):
         override = datetime.datetime(2020, 1, 1)
         api.set_date_for_block(self.items[0][0].course_key, self.items[0][0], 'due', override, user=self.user)
         usage_info = mock.MagicMock()
         usage_info.course_key = self.course_id
```

