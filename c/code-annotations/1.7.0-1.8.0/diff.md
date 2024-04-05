# Comparing `tmp/code-annotations-1.7.0.tar.gz` & `tmp/code-annotations-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code-annotations-1.7.0.tar", last modified: Thu Mar 14 11:56:33 2024, max compression
+gzip compressed data, was "code-annotations-1.8.0.tar", last modified: Fri Apr  5 16:37:53 2024, max compression
```

## Comparing `code-annotations-1.7.0.tar` & `code-annotations-1.8.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:56:33.102578 code-annotations-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-03-14 11:56:29.000000 code-annotations-1.7.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-14 11:56:29.000000 code-annotations-1.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-14 11:56:29.000000 code-annotations-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-14 11:56:29.000000 code-annotations-1.7.0/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8531 2024-03-14 11:56:33.102578 code-annotations-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-03-14 11:56:29.000000 code-annotations-1.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:56:33.094578 code-annotations-1.7.0/code_annotations/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-14 11:56:29.000000 code-annotations-1.7.0/code_annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-03-14 11:56:29.000000 code-annotations-1.7.0/code_annotations/annotation_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    23608 2024-03-14 11:56:29.000000 code-annotations-1.7.0/code_annotations/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-03-14 11:56:29.000000 code-annotations-1.7.0/code_annotations/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:56:33.094578 code-annotations-1.7.0/code_annotations/contrib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:56:33.098578 code-annotations-1.7.0/code_annotations/contrib/config/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-14 11:56:29.000000 code-annotations-1.7.0/code_annotations/contrib/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-03-14 11:56:29.000000 code-annotations-1.7.0/code_annotations/contrib/config/feature_toggle_annotations.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-14 11:56:29.000000 code-annotations-1.7.0/code_annotations/contrib/config/openedx_events_annotations.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-14 11:56:29.000000 code-annotations-1.7.0/code_annotations/contrib/config/setting_annotations.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:56:33.094578 code-annotations-1.7.0/code_annotations/contrib/sphinx/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:56:33.098578 code-annotations-1.7.0/code_annotations/contrib/sphinx/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-14 11:56:29.000000 code-annotations-1.7.0/code_annotations/contrib/sphinx/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-03-14 11:56:29.000000 code-annotations-1.7.0/code_annotations/contrib/sphinx/extensions/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-03-14 11:56:29.000000 code-annotations-1.7.0/code_annotations/contrib/sphinx/extensions/featuretoggles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-03-14 11:56:29.000000 code-annotations-1.7.0/code_annotations/contrib/sphinx/extensions/openedx_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-03-14 11:56:29.000000 code-annotations-1.7.0/code_annotations/contrib/sphinx/extensions/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-14 11:56:29.000000 code-annotations-1.7.0/code_annotations/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:56:33.098578 code-annotations-1.7.0/code_annotations/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-14 11:56:29.000000 code-annotations-1.7.0/code_annotations/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-03-14 11:56:29.000000 code-annotations-1.7.0/code_annotations/extensions/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-14 11:56:29.000000 code-annotations-1.7.0/code_annotations/extensions/javascript.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-14 11:56:29.000000 code-annotations-1.7.0/code_annotations/extensions/python.py
--rw-r--r--   0 runner    (1001) docker     (127)    16689 2024-03-14 11:56:29.000000 code-annotations-1.7.0/code_annotations/find_django.py
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-03-14 11:56:29.000000 code-annotations-1.7.0/code_annotations/find_static.py
--rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-03-14 11:56:29.000000 code-annotations-1.7.0/code_annotations/generate_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-03-14 11:56:29.000000 code-annotations-1.7.0/code_annotations/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:56:33.102578 code-annotations-1.7.0/code_annotations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8531 2024-03-14 11:56:33.000000 code-annotations-1.7.0/code_annotations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-03-14 11:56:33.000000 code-annotations-1.7.0/code_annotations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 11:56:33.000000 code-annotations-1.7.0/code_annotations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 11:56:33.000000 code-annotations-1.7.0/code_annotations.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 11:56:33.000000 code-annotations-1.7.0/code_annotations.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-14 11:56:33.000000 code-annotations-1.7.0/code_annotations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-14 11:56:33.000000 code-annotations-1.7.0/code_annotations.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:56:33.098578 code-annotations-1.7.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-14 11:56:29.000000 code-annotations-1.7.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-14 11:56:33.102578 code-annotations-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-03-14 11:56:29.000000 code-annotations-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:56:33.102578 code-annotations-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-03-14 11:56:29.000000 code-annotations-1.7.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-03-14 11:56:29.000000 code-annotations-1.7.0/tests/test_django_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-03-14 11:56:29.000000 code-annotations-1.7.0/tests/test_django_generate_safelist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-03-14 11:56:29.000000 code-annotations-1.7.0/tests/test_django_list_local_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    15941 2024-03-14 11:56:29.000000 code-annotations-1.7.0/tests/test_find_django.py
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-03-14 11:56:29.000000 code-annotations-1.7.0/tests/test_find_static.py
--rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-03-14 11:56:29.000000 code-annotations-1.7.0/tests/test_generate_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-03-14 11:56:29.000000 code-annotations-1.7.0/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-14 11:56:29.000000 code-annotations-1.7.0/tests/test_sphinx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:53.117139 code-annotations-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-05 16:37:49.000000 code-annotations-1.8.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-05 16:37:49.000000 code-annotations-1.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-05 16:37:49.000000 code-annotations-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-05 16:37:49.000000 code-annotations-1.8.0/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-04-05 16:37:53.117139 code-annotations-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-05 16:37:49.000000 code-annotations-1.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:53.113139 code-annotations-1.8.0/code_annotations/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-05 16:37:49.000000 code-annotations-1.8.0/code_annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-05 16:37:49.000000 code-annotations-1.8.0/code_annotations/annotation_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23608 2024-04-05 16:37:49.000000 code-annotations-1.8.0/code_annotations/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-04-05 16:37:49.000000 code-annotations-1.8.0/code_annotations/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:53.109139 code-annotations-1.8.0/code_annotations/contrib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:53.113139 code-annotations-1.8.0/code_annotations/contrib/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-05 16:37:49.000000 code-annotations-1.8.0/code_annotations/contrib/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-05 16:37:49.000000 code-annotations-1.8.0/code_annotations/contrib/config/feature_toggle_annotations.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-05 16:37:49.000000 code-annotations-1.8.0/code_annotations/contrib/config/openedx_events_annotations.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-05 16:37:49.000000 code-annotations-1.8.0/code_annotations/contrib/config/setting_annotations.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:53.109139 code-annotations-1.8.0/code_annotations/contrib/sphinx/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:53.113139 code-annotations-1.8.0/code_annotations/contrib/sphinx/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-05 16:37:49.000000 code-annotations-1.8.0/code_annotations/contrib/sphinx/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-05 16:37:49.000000 code-annotations-1.8.0/code_annotations/contrib/sphinx/extensions/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-04-05 16:37:49.000000 code-annotations-1.8.0/code_annotations/contrib/sphinx/extensions/featuretoggles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-04-05 16:37:49.000000 code-annotations-1.8.0/code_annotations/contrib/sphinx/extensions/openedx_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-05 16:37:49.000000 code-annotations-1.8.0/code_annotations/contrib/sphinx/extensions/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-05 16:37:49.000000 code-annotations-1.8.0/code_annotations/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:53.113139 code-annotations-1.8.0/code_annotations/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-05 16:37:49.000000 code-annotations-1.8.0/code_annotations/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-04-05 16:37:49.000000 code-annotations-1.8.0/code_annotations/extensions/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-05 16:37:49.000000 code-annotations-1.8.0/code_annotations/extensions/javascript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-05 16:37:49.000000 code-annotations-1.8.0/code_annotations/extensions/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16689 2024-04-05 16:37:49.000000 code-annotations-1.8.0/code_annotations/find_django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-05 16:37:49.000000 code-annotations-1.8.0/code_annotations/find_static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-04-05 16:37:49.000000 code-annotations-1.8.0/code_annotations/generate_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-04-05 16:37:49.000000 code-annotations-1.8.0/code_annotations/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:53.117139 code-annotations-1.8.0/code_annotations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-04-05 16:37:53.000000 code-annotations-1.8.0/code_annotations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-05 16:37:53.000000 code-annotations-1.8.0/code_annotations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:37:53.000000 code-annotations-1.8.0/code_annotations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-05 16:37:53.000000 code-annotations-1.8.0/code_annotations.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:37:53.000000 code-annotations-1.8.0/code_annotations.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-05 16:37:53.000000 code-annotations-1.8.0/code_annotations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 16:37:53.000000 code-annotations-1.8.0/code_annotations.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:53.113139 code-annotations-1.8.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-05 16:37:49.000000 code-annotations-1.8.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-05 16:37:53.117139 code-annotations-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-04-05 16:37:49.000000 code-annotations-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:53.117139 code-annotations-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-04-05 16:37:49.000000 code-annotations-1.8.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-04-05 16:37:49.000000 code-annotations-1.8.0/tests/test_django_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-05 16:37:49.000000 code-annotations-1.8.0/tests/test_django_generate_safelist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-05 16:37:49.000000 code-annotations-1.8.0/tests/test_django_list_local_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15941 2024-04-05 16:37:49.000000 code-annotations-1.8.0/tests/test_find_django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-05 16:37:49.000000 code-annotations-1.8.0/tests/test_find_static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-04-05 16:37:49.000000 code-annotations-1.8.0/tests/test_generate_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-05 16:37:49.000000 code-annotations-1.8.0/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-05 16:37:49.000000 code-annotations-1.8.0/tests/test_sphinx.py
```

### Comparing `code-annotations-1.7.0/CHANGELOG.rst` & `code-annotations-1.8.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,20 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+[1.8.0] - 2024-03-31
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+* Added python3.11 and 3.12 support. Dropped django32 support.
+
+
 [1.6.0] - 2024-01-31
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 * Added new annotation ``toggle_removal_ticket``
 
 [1.5.0] - 2023-07-21
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `code-annotations-1.7.0/LICENSE.txt` & `code-annotations-1.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `code-annotations-1.7.0/NOTICE.txt` & `code-annotations-1.8.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `code-annotations-1.7.0/PKG-INFO` & `code-annotations-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: code-annotations
-Version: 1.7.0
+Version: 1.8.0
 Summary: Extensible tools for parsing annotations in codebases
 Home-page: https://github.com/openedx/code-annotations
 Author: edX
 Author-email: oscm@edx.org
 License: Apache Software License 2.0
 Keywords: edx pii code annotations
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: NOTICE.txt
-Requires-Dist: python-slugify
-Requires-Dist: click
 Requires-Dist: pyyaml
 Requires-Dist: stevedore
+Requires-Dist: python-slugify
+Requires-Dist: click
 Requires-Dist: Jinja2
 Provides-Extra: django
 Requires-Dist: Django<2.3,>=2.2; extra == "django"
 
 code-annotations
 =============================
 
@@ -124,14 +125,20 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+[1.8.0] - 2024-03-31
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+* Added python3.11 and 3.12 support. Dropped django32 support.
+
+
 [1.6.0] - 2024-01-31
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 * Added new annotation ``toggle_removal_ticket``
 
 [1.5.0] - 2023-07-21
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `code-annotations-1.7.0/README.rst` & `code-annotations-1.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `code-annotations-1.7.0/code_annotations/annotation_errors.py` & `code-annotations-1.8.0/code_annotations/annotation_errors.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.7.0/code_annotations/base.py` & `code-annotations-1.8.0/code_annotations/base.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.7.0/code_annotations/cli.py` & `code-annotations-1.8.0/code_annotations/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
                 annotation_count += len(annotated_models[filename])
 
             elapsed = datetime.datetime.now() - start_time
             click.echo("Search found {} annotations in {} seconds.".format(
                 annotation_count, elapsed.total_seconds()
             ))
 
-    except Exception as exc:  # pylint: disable=broad-except
+    except Exception as exc:
         click.echo(traceback.print_exc())
         fail(str(exc))
 
 
 @entry_point.command('static_find_annotations')
 @click.option(
     '--config_file',
@@ -165,15 +165,15 @@
         annotation_count = 0
 
         for filename in all_results:
             annotation_count += len(all_results[filename])
 
         click.echo(f"Search found {annotation_count} annotations in {elapsed}.")
 
-    except Exception as exc:  # pylint: disable=broad-except
+    except Exception as exc:
         click.echo(traceback.print_exc())
         fail(str(exc))
 
 
 @entry_point.command("generate_docs")
 @click.option(
     '--config_file',
@@ -208,10 +208,10 @@
         config.echo("Rendering the following reports: \n{}".format("\n".join([r.name for r in report_files])))
 
         renderer = ReportRenderer(config, report_files)
         renderer.render()
 
         elapsed = datetime.datetime.now() - start_time
         click.echo(f"Report rendered in {elapsed.total_seconds()} seconds.")
-    except Exception as exc:  # pylint: disable=broad-except
+    except Exception as exc:
         click.echo(traceback.print_exc())
         fail(str(exc))
```

### Comparing `code-annotations-1.7.0/code_annotations/contrib/config/__init__.py` & `code-annotations-1.8.0/code_annotations/contrib/config/__init__.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.7.0/code_annotations/contrib/config/feature_toggle_annotations.yaml` & `code-annotations-1.8.0/code_annotations/contrib/config/feature_toggle_annotations.yaml`

 * *Files identical despite different names*

### Comparing `code-annotations-1.7.0/code_annotations/contrib/config/openedx_events_annotations.yaml` & `code-annotations-1.8.0/code_annotations/contrib/config/openedx_events_annotations.yaml`

 * *Files identical despite different names*

### Comparing `code-annotations-1.7.0/code_annotations/contrib/sphinx/extensions/base.py` & `code-annotations-1.8.0/code_annotations/contrib/sphinx/extensions/base.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.7.0/code_annotations/contrib/sphinx/extensions/featuretoggles.py` & `code-annotations-1.8.0/code_annotations/contrib/sphinx/extensions/featuretoggles.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
                 "target_removal_date",
                 "implementation",
                 "use_cases",
             ]
             for opt in optional_attrs:
                 if toggle.get(f".. toggle_{opt}:") not in (None, "None", "n/a", "N/A"):
                     toggle_section += nodes.paragraph(
-                        text=f'{opt.title().replace("_"," ")}: {toggle[f".. toggle_{opt}:"]}',
+                        text=f'{opt.title().replace("_", " ")}: {toggle[f".. toggle_{opt}:"]}',
                         ids=[f"{opt}-{toggle_name}"],
                     )
             yield toggle_section
 
 
 def setup(app):
     """
```

### Comparing `code-annotations-1.7.0/code_annotations/contrib/sphinx/extensions/openedx_events.py` & `code-annotations-1.8.0/code_annotations/contrib/sphinx/extensions/openedx_events.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.7.0/code_annotations/contrib/sphinx/extensions/settings.py` & `code-annotations-1.8.0/code_annotations/contrib/sphinx/extensions/settings.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.7.0/code_annotations/extensions/base.py` & `code-annotations-1.8.0/code_annotations/extensions/base.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.7.0/code_annotations/find_django.py` & `code-annotations-1.8.0/code_annotations/find_django.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.7.0/code_annotations/find_static.py` & `code-annotations-1.8.0/code_annotations/find_static.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.7.0/code_annotations/generate_docs.py` & `code-annotations-1.8.0/code_annotations/generate_docs.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.7.0/code_annotations/helpers.py` & `code-annotations-1.8.0/code_annotations/helpers.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.7.0/code_annotations.egg-info/PKG-INFO` & `code-annotations-1.8.0/code_annotations.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: code-annotations
-Version: 1.7.0
+Version: 1.8.0
 Summary: Extensible tools for parsing annotations in codebases
 Home-page: https://github.com/openedx/code-annotations
 Author: edX
 Author-email: oscm@edx.org
 License: Apache Software License 2.0
 Keywords: edx pii code annotations
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: NOTICE.txt
-Requires-Dist: python-slugify
-Requires-Dist: click
 Requires-Dist: pyyaml
 Requires-Dist: stevedore
+Requires-Dist: python-slugify
+Requires-Dist: click
 Requires-Dist: Jinja2
 Provides-Extra: django
 Requires-Dist: Django<2.3,>=2.2; extra == "django"
 
 code-annotations
 =============================
 
@@ -124,14 +125,20 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+[1.8.0] - 2024-03-31
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+* Added python3.11 and 3.12 support. Dropped django32 support.
+
+
 [1.6.0] - 2024-01-31
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 * Added new annotation ``toggle_removal_ticket``
 
 [1.5.0] - 2023-07-21
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `code-annotations-1.7.0/code_annotations.egg-info/SOURCES.txt` & `code-annotations-1.8.0/code_annotations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `code-annotations-1.7.0/setup.py` & `code-annotations-1.8.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,17 +93,18 @@
     extras_require={"django": ["Django>=2.2,<2.3"]},
     license="Apache Software License 2.0",
     zip_safe=False,
     keywords='edx pii code annotations',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Framework :: Django',
-        'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
 )
```

### Comparing `code-annotations-1.7.0/tests/test_base.py` & `code-annotations-1.8.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.7.0/tests/test_django_coverage.py` & `code-annotations-1.8.0/tests/test_django_coverage.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.7.0/tests/test_django_generate_safelist.py` & `code-annotations-1.8.0/tests/test_django_generate_safelist.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.7.0/tests/test_django_list_local_models.py` & `code-annotations-1.8.0/tests/test_django_list_local_models.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.7.0/tests/test_find_django.py` & `code-annotations-1.8.0/tests/test_find_django.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.7.0/tests/test_find_static.py` & `code-annotations-1.8.0/tests/test_find_static.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.7.0/tests/test_generate_docs.py` & `code-annotations-1.8.0/tests/test_generate_docs.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.7.0/tests/test_search.py` & `code-annotations-1.8.0/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.7.0/tests/test_sphinx.py` & `code-annotations-1.8.0/tests/test_sphinx.py`

 * *Files identical despite different names*

