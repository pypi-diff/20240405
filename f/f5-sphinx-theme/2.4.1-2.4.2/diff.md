# Comparing `tmp/f5_sphinx_theme-2.4.1.tar.gz` & `tmp/f5_sphinx_theme-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/f5-sphinx-theme/f5-sphinx-theme/dist/.tmp-wv7r1ara/f5_sphinx_theme-2.4.1.tar", last modified: Thu Apr  4 21:58:12 2024, max compression
+gzip compressed data, was "/home/runner/work/f5-sphinx-theme/f5-sphinx-theme/dist/.tmp-g1wlvesz/f5_sphinx_theme-2.4.2.tar", last modified: Thu Apr  4 22:15:17 2024, max compression
```

## Comparing `f5_sphinx_theme-2.4.1.tar` & `f5_sphinx_theme-2.4.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/breadcrumb.html
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/extralinks.html
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/head.html
--rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/localtoc.html
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/searchbox.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/
--rwxr-xr-x   0 runner    (1001) docker     (127)   453169 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/CoveoFullSearch.css
--rwxr-xr-x   0 runner    (1001) docker     (127)    25897 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/bootstrap-theme.css
--rwxr-xr-x   0 runner    (1001) docker     (127)    24167 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/bootstrap-theme.min.css
--rwxr-xr-x   0 runner    (1001) docker     (127)   108100 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/bootstrap.css
--rwxr-xr-x   0 runner    (1001) docker     (127)    89501 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)    19559 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/f5-theme.css
--rw-r--r--   0 runner    (1001) docker     (127)   121080 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/f5.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    25336 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/ProximaBold.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19040 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/ProximaBold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    25452 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/ProximaMedium.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19068 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/ProximaMedium.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    25620 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/ProximaThin.woff
--rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/ProximaThin.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    20127 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (127)   108738 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (127)    45404 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/
--rwxr-xr-x   0 runner    (1001) docker     (127)   548426 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/CoveoJsSearch.Lazy.min.js
--rwxr-xr-x   0 runner    (1001) docker     (127)    56583 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/bootstrap.js
--rwxr-xr-x   0 runner    (1001) docker     (127)    58072 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/bootstrap.min.js
--rwxr-xr-x   0 runner    (1001) docker     (127)    12128 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/clouddocs.js
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/feedback.js
--rwxr-xr-x   0 runner    (1001) docker     (127)     2417 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/jquery.appear.js
--rwxr-xr-x   0 runner    (1001) docker     (127)    13945 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/printThis.js
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/theme.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 21:57:52.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:15:17.000000 f5_sphinx_theme-2.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-04-04 22:15:17.000000 f5_sphinx_theme-2.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:15:17.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/breadcrumb.html
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/extralinks.html
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/head.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/searchbox.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:15:17.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:15:17.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/css/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   453169 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/css/CoveoFullSearch.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25897 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/css/bootstrap-theme.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24167 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/css/bootstrap-theme.min.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)   108100 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/css/bootstrap.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)    89501 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    19559 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/css/f5-theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)   121080 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/css/f5.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:15:17.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    25336 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/fonts/ProximaBold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19040 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/fonts/ProximaBold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    25452 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/fonts/ProximaMedium.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19068 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/fonts/ProximaMedium.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    25620 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/fonts/ProximaThin.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/fonts/ProximaThin.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    20127 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   108738 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    45404 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:15:17.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/js/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   548426 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/js/CoveoJsSearch.Lazy.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    56583 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/js/bootstrap.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    58072 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/js/bootstrap.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12128 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/js/clouddocs.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/js/feedback.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2417 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/js/jquery.appear.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13945 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/js/printThis.js
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:15:17.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-04-04 22:15:17.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-04 22:15:17.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 22:15:17.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-04 22:15:17.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 22:15:00.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 22:15:17.000000 f5_sphinx_theme-2.4.2/f5_sphinx_theme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-04 22:15:17.000000 f5_sphinx_theme-2.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-04 22:14:58.000000 f5_sphinx_theme-2.4.2/setup.py
```

### Comparing `f5_sphinx_theme-2.4.1/LICENSE` & `f5_sphinx_theme-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/PKG-INFO` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: f5_sphinx_theme
-Version: 2.4.1
+Name: f5-sphinx-theme
+Version: 2.4.2
 Summary: Sphinx theme for F5 Networks
 Home-page: https://github.com/F5DevCentral/f5-sphinx-theme
 Author: F5 Networks
 Author-email: f5-sphinx-theme@f5.com
 License: Apache2
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
@@ -19,16 +19,15 @@
 Classifier: Topic :: Software Development :: Documentation
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 License-File: LICENSE
 
 F5 Sphinx Theme
 ===============
 
-.. image:: https://travis-ci.org/f5devcentral/f5-sphinx-theme.svg?branch=master
-   :target: https://travis-ci.org/f5devcentral/f5-sphinx-theme
+.. image:: https://github.com/f5devcentral/f5-sphinx-theme/actions/workflows/test.yml/badge.svg
 
 The f5-sphinx-theme provides F5 Networks styling and layouts for projects built with `Sphinx <http://www.sphinx-doc.org/en/stable/index.html>`_. This theme should not be used without modification for any project that doesn't publish documentation to `clouddocs.f5.com <http://clouddocs.f5.com>`_.
 
 
 Setup and Configuration
 -----------------------
 1. ``pip install f5-sphinx-theme``
@@ -112,15 +111,15 @@
 -----
 
 See the `project wiki <https://github.com/f5devcentral/f5-sphinx-theme/wiki>`_ for more information.
 
 Testing
 -------
 
-This project uses Travis-CI for CI/CD.
+This project uses GitHub Actions for CI/CD.
 
 Copyright
 ---------
 
 Copyright 2017-18 F5 Networks Inc.
 
 License
```

### Comparing `f5_sphinx_theme-2.4.1/README.rst` & `f5_sphinx_theme-2.4.2/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 F5 Sphinx Theme
 ===============
 
-.. image:: https://travis-ci.org/f5devcentral/f5-sphinx-theme.svg?branch=master
-   :target: https://travis-ci.org/f5devcentral/f5-sphinx-theme
+.. image:: https://github.com/f5devcentral/f5-sphinx-theme/actions/workflows/test.yml/badge.svg
 
 The f5-sphinx-theme provides F5 Networks styling and layouts for projects built with `Sphinx <http://www.sphinx-doc.org/en/stable/index.html>`_. This theme should not be used without modification for any project that doesn't publish documentation to `clouddocs.f5.com <http://clouddocs.f5.com>`_.
 
 
 Setup and Configuration
 -----------------------
 1. ``pip install f5-sphinx-theme``
@@ -90,15 +89,15 @@
 -----
 
 See the `project wiki <https://github.com/f5devcentral/f5-sphinx-theme/wiki>`_ for more information.
 
 Testing
 -------
 
-This project uses Travis-CI for CI/CD.
+This project uses GitHub Actions for CI/CD.
 
 Copyright
 ---------
 
 Copyright 2017-18 F5 Networks Inc.
 
 License
```

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/__init__.py` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 from os import path
 
 
-__version__ = "2.4.1"
+__version__ = "2.4.2"
 
 
 def get_html_theme_path():
     """Return the html theme path for this template library.
 
     :returns: List of directories to find template files in
     """
```

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/globaltoc.html` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/globaltoc.html`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/head.html` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/head.html`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/layout.html` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/layout.html`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/localtoc.html` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/localtoc.html`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/searchbox.html` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/searchbox.html`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/CoveoFullSearch.css` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/css/CoveoFullSearch.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/bootstrap-theme.css` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/bootstrap-theme.min.css` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/bootstrap.css` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/bootstrap.min.css` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/custom.css` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/css/custom.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/f5-theme.css` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/css/f5-theme.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/f5.css` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/css/f5.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/ProximaBold.woff` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/fonts/ProximaBold.woff`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/ProximaBold.woff2` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/fonts/ProximaBold.woff2`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/ProximaMedium.woff` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/fonts/ProximaMedium.woff`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/ProximaMedium.woff2` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/fonts/ProximaMedium.woff2`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/ProximaThin.woff` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/fonts/ProximaThin.woff`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/ProximaThin.woff2` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/fonts/ProximaThin.woff2`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.eot` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.svg` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.ttf` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff2` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/CoveoJsSearch.Lazy.min.js` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/js/CoveoJsSearch.Lazy.min.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/bootstrap.js` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/bootstrap.min.js` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/clouddocs.js` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/js/clouddocs.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/feedback.js` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/js/feedback.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/jquery.appear.js` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/js/jquery.appear.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/printThis.js` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme/static/js/printThis.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme.egg-info/PKG-INFO` & `f5_sphinx_theme-2.4.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: f5-sphinx-theme
-Version: 2.4.1
+Name: f5_sphinx_theme
+Version: 2.4.2
 Summary: Sphinx theme for F5 Networks
 Home-page: https://github.com/F5DevCentral/f5-sphinx-theme
 Author: F5 Networks
 Author-email: f5-sphinx-theme@f5.com
 License: Apache2
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
@@ -19,16 +19,15 @@
 Classifier: Topic :: Software Development :: Documentation
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 License-File: LICENSE
 
 F5 Sphinx Theme
 ===============
 
-.. image:: https://travis-ci.org/f5devcentral/f5-sphinx-theme.svg?branch=master
-   :target: https://travis-ci.org/f5devcentral/f5-sphinx-theme
+.. image:: https://github.com/f5devcentral/f5-sphinx-theme/actions/workflows/test.yml/badge.svg
 
 The f5-sphinx-theme provides F5 Networks styling and layouts for projects built with `Sphinx <http://www.sphinx-doc.org/en/stable/index.html>`_. This theme should not be used without modification for any project that doesn't publish documentation to `clouddocs.f5.com <http://clouddocs.f5.com>`_.
 
 
 Setup and Configuration
 -----------------------
 1. ``pip install f5-sphinx-theme``
@@ -112,15 +111,15 @@
 -----
 
 See the `project wiki <https://github.com/f5devcentral/f5-sphinx-theme/wiki>`_ for more information.
 
 Testing
 -------
 
-This project uses Travis-CI for CI/CD.
+This project uses GitHub Actions for CI/CD.
 
 Copyright
 ---------
 
 Copyright 2017-18 F5 Networks Inc.
 
 License
```

### Comparing `f5_sphinx_theme-2.4.1/f5_sphinx_theme.egg-info/SOURCES.txt` & `f5_sphinx_theme-2.4.2/f5_sphinx_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.1/setup.py` & `f5_sphinx_theme-2.4.2/setup.py`

 * *Files identical despite different names*

