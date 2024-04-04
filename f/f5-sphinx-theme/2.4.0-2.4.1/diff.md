# Comparing `tmp/f5_sphinx_theme-2.4.0.tar.gz` & `tmp/f5_sphinx_theme-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/f5_sphinx_theme-2.4.0.tar", last modified: Wed Oct  4 23:12:10 2023, max compression
+gzip compressed data, was "/home/runner/work/f5-sphinx-theme/f5-sphinx-theme/dist/.tmp-wv7r1ara/f5_sphinx_theme-2.4.1.tar", last modified: Thu Apr  4 21:58:12 2024, max compression
```

## Comparing `f5_sphinx_theme-2.4.0.tar` & `f5_sphinx_theme-2.4.1.tar`

### file list

```diff
@@ -1,55 +1,54 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-10-04 23:12:10.000000 f5_sphinx_theme-2.4.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11341 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      150 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     5343 2023-10-04 23:12:10.000000 f5_sphinx_theme-2.4.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     4526 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-10-04 23:12:10.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1123 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      479 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/breadcrumb.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      152 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/extralinks.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      603 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/globaltoc.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1637 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/head.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     6142 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/layout.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      695 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/localtoc.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      546 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/searchbox.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-10-04 23:12:10.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-10-04 23:12:10.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/css/
--rwxrwxr-x   0 travis    (2000) travis    (2000)   453169 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/css/CoveoFullSearch.css
--rwxrwxr-x   0 travis    (2000) travis    (2000)    25897 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/css/bootstrap-theme.css
--rwxrwxr-x   0 travis    (2000) travis    (2000)    24167 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/css/bootstrap-theme.min.css
--rwxrwxr-x   0 travis    (2000) travis    (2000)   108100 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/css/bootstrap.css
--rwxrwxr-x   0 travis    (2000) travis    (2000)    89501 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/css/bootstrap.min.css
--rw-rw-r--   0 travis    (2000) travis    (2000)      739 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/css/custom.css
--rw-rw-r--   0 travis    (2000) travis    (2000)    19559 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/css/f5-theme.css
--rw-rw-r--   0 travis    (2000) travis    (2000)   121080 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/css/f5.css
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-10-04 23:12:10.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/fonts/
--rw-rw-r--   0 travis    (2000) travis    (2000)    25336 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/fonts/ProximaBold.woff
--rw-rw-r--   0 travis    (2000) travis    (2000)    19040 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/fonts/ProximaBold.woff2
--rw-rw-r--   0 travis    (2000) travis    (2000)    25452 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/fonts/ProximaMedium.woff
--rw-rw-r--   0 travis    (2000) travis    (2000)    19068 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/fonts/ProximaMedium.woff2
--rw-rw-r--   0 travis    (2000) travis    (2000)    25620 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/fonts/ProximaThin.woff
--rw-rw-r--   0 travis    (2000) travis    (2000)    18964 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/fonts/ProximaThin.woff2
--rw-rw-r--   0 travis    (2000) travis    (2000)    20127 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.eot
--rw-rw-r--   0 travis    (2000) travis    (2000)   108738 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.svg
--rw-rw-r--   0 travis    (2000) travis    (2000)    45404 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.ttf
--rw-rw-r--   0 travis    (2000) travis    (2000)    23424 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff
--rw-rw-r--   0 travis    (2000) travis    (2000)    18028 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-10-04 23:12:10.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/js/
--rwxrwxr-x   0 travis    (2000) travis    (2000)   548426 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/js/CoveoJsSearch.Lazy.min.js
--rwxrwxr-x   0 travis    (2000) travis    (2000)    56583 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/js/bootstrap.js
--rwxrwxr-x   0 travis    (2000) travis    (2000)    58072 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/js/bootstrap.min.js
--rwxrwxr-x   0 travis    (2000) travis    (2000)    12128 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/js/clouddocs.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     3474 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/js/feedback.js
--rw-r--r--   0 travis    (2000) travis    (2000)   156972 2023-10-04 23:11:12.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/js/index.js
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2417 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/js/jquery.appear.js
--rwxrwxr-x   0 travis    (2000) travis    (2000)    13945 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/js/printThis.js
--rw-rw-r--   0 travis    (2000) travis    (2000)      397 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme/theme.conf
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-10-04 23:12:10.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5343 2023-10-04 23:12:10.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1817 2023-10-04 23:12:10.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-10-04 23:12:10.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       55 2023-10-04 23:12:10.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-10-04 23:10:17.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2023-10-04 23:12:10.000000 f5_sphinx_theme-2.4.0/f5_sphinx_theme.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2023-10-04 23:12:10.000000 f5_sphinx_theme-2.4.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2016 2023-10-04 23:10:02.000000 f5_sphinx_theme-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/breadcrumb.html
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/extralinks.html
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/head.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/searchbox.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   453169 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/CoveoFullSearch.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25897 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/bootstrap-theme.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24167 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/bootstrap-theme.min.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)   108100 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/bootstrap.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)    89501 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    19559 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/f5-theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)   121080 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/f5.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    25336 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/ProximaBold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19040 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/ProximaBold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    25452 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/ProximaMedium.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19068 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/ProximaMedium.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    25620 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/ProximaThin.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/ProximaThin.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    20127 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   108738 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    45404 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   548426 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/CoveoJsSearch.Lazy.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    56583 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/bootstrap.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    58072 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/bootstrap.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12128 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/clouddocs.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/feedback.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2417 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/jquery.appear.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13945 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/printThis.js
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 21:57:52.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/f5_sphinx_theme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-04 21:58:12.000000 f5_sphinx_theme-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-04 21:57:50.000000 f5_sphinx_theme-2.4.1/setup.py
```

### Comparing `f5_sphinx_theme-2.4.0/LICENSE` & `f5_sphinx_theme-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/PKG-INFO` & `f5_sphinx_theme-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f5_sphinx_theme
-Version: 2.4.0
+Version: 2.4.1
 Summary: Sphinx theme for F5 Networks
 Home-page: https://github.com/F5DevCentral/f5-sphinx-theme
 Author: F5 Networks
 Author-email: f5-sphinx-theme@f5.com
 License: Apache2
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
```

### Comparing `f5_sphinx_theme-2.4.0/README.rst` & `f5_sphinx_theme-2.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/__init__.py` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 from os import path
 
 
-__version__ = "2.4.0"
+__version__ = "2.4.1"
 
 
 def get_html_theme_path():
     """Return the html theme path for this template library.
 
     :returns: List of directories to find template files in
     """
```

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/globaltoc.html` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/globaltoc.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-00000000: 7b23 0a20 436f 7079 7269 6768 7420 3230  {#. Copyright 20
-00000010: 3137 2046 3520 4e65 7477 6f72 6b73 0a0a  17 F5 Networks..
-00000020: 204c 6963 656e 7365 6420 756e 6465 7220   Licensed under 
-00000030: 7468 6520 4170 6163 6865 204c 6963 656e  the Apache Licen
-00000040: 7365 2c20 5665 7273 696f 6e20 322e 3020  se, Version 2.0 
-00000050: 2874 6865 2022 4c69 6365 6e73 6522 293b  (the "License");
-00000060: 0a20 796f 7520 6d61 7920 6e6f 7420 7573  . you may not us
-00000070: 6520 7468 6973 2066 696c 6520 6578 6365  e this file exce
-00000080: 7074 2069 6e20 636f 6d70 6c69 616e 6365  pt in compliance
-00000090: 2077 6974 6820 7468 6520 4c69 6365 6e73   with the Licens
-000000a0: 652e 0a20 596f 7520 6d61 7920 6f62 7461  e.. You may obta
-000000b0: 696e 2061 2063 6f70 7920 6f66 2074 6865  in a copy of the
-000000c0: 204c 6963 656e 7365 2061 740a 0a20 2020   License at..   
-000000d0: 2020 6874 7470 3a2f 2f77 7777 2e61 7061    http://www.apa
-000000e0: 6368 652e 6f72 672f 6c69 6365 6e73 6573  che.org/licenses
-000000f0: 2f4c 4943 454e 5345 2d32 2e30 0a0a 2055  /LICENSE-2.0.. U
-00000100: 6e6c 6573 7320 7265 7175 6972 6564 2062  nless required b
-00000110: 7920 6170 706c 6963 6162 6c65 206c 6177  y applicable law
-00000120: 206f 7220 6167 7265 6564 2074 6f20 696e   or agreed to in
-00000130: 2077 7269 7469 6e67 2c20 736f 6674 7761   writing, softwa
-00000140: 7265 0a20 6469 7374 7269 6275 7465 6420  re. distributed 
-00000150: 756e 6465 7220 7468 6520 4c69 6365 6e73  under the Licens
-00000160: 6520 6973 2064 6973 7472 6962 7574 6564  e is distributed
-00000170: 206f 6e20 616e 2022 4153 2049 5322 2042   on an "AS IS" B
-00000180: 4153 4953 2c0a 2057 4954 484f 5554 2057  ASIS,. WITHOUT W
-00000190: 4152 5241 4e54 4945 5320 4f52 2043 4f4e  ARRANTIES OR CON
-000001a0: 4449 5449 4f4e 5320 4f46 2041 4e59 204b  DITIONS OF ANY K
-000001b0: 494e 442c 2065 6974 6865 7220 6578 7072  IND, either expr
-000001c0: 6573 7320 6f72 2069 6d70 6c69 6564 2e0a  ess or implied..
-000001d0: 2053 6565 2074 6865 204c 6963 656e 7365   See the License
-000001e0: 2066 6f72 2074 6865 2073 7065 6369 6669   for the specifi
-000001f0: 6320 6c61 6e67 7561 6765 2067 6f76 6572  c language gover
-00000200: 6e69 6e67 2070 6572 6d69 7373 696f 6e73  ning permissions
-00000210: 2061 6e64 0a20 6c69 6d69 7461 7469 6f6e   and. limitation
-00000220: 7320 756e 6465 7220 7468 6520 4c69 6365  s under the Lice
-00000230: 6e73 652e 0a23 7d0a 0a7b 7b20 746f 6374  nse..#}..{{ toct
-00000240: 7265 6528 696e 636c 7564 6568 6964 6465  ree(includehidde
-00000250: 6e3d 5472 7565 2920 7d7d 0a              n=True) }}.
+00000000: 3c21 444f 4354 5950 4520 6874 6d6c 3e0a  <!DOCTYPE html>.
+00000010: 7b23 0a43 6f70 7972 6967 6874 2032 3031  {#.Copyright 201
+00000020: 3720 4635 204e 6574 776f 726b 730a 0a4c  7 F5 Networks..L
+00000030: 6963 656e 7365 6420 756e 6465 7220 7468  icensed under th
+00000040: 6520 4170 6163 6865 204c 6963 656e 7365  e Apache License
+00000050: 2c20 5665 7273 696f 6e20 322e 3020 2874  , Version 2.0 (t
+00000060: 6865 2022 4c69 6365 6e73 6522 293b 0a79  he "License");.y
+00000070: 6f75 206d 6179 206e 6f74 2075 7365 2074  ou may not use t
+00000080: 6869 7320 6669 6c65 2065 7863 6570 7420  his file except 
+00000090: 696e 2063 6f6d 706c 6961 6e63 6520 7769  in compliance wi
+000000a0: 7468 2074 6865 204c 6963 656e 7365 2e0a  th the License..
+000000b0: 596f 7520 6d61 7920 6f62 7461 696e 2061  You may obtain a
+000000c0: 2063 6f70 7920 6f66 2074 6865 204c 6963   copy of the Lic
+000000d0: 656e 7365 2061 740a 0a68 7474 703a 2f2f  ense at..http://
+000000e0: 7777 772e 6170 6163 6865 2e6f 7267 2f6c  www.apache.org/l
+000000f0: 6963 656e 7365 732f 4c49 4345 4e53 452d  icenses/LICENSE-
+00000100: 322e 300a 0a55 6e6c 6573 7320 7265 7175  2.0..Unless requ
+00000110: 6972 6564 2062 7920 6170 706c 6963 6162  ired by applicab
+00000120: 6c65 206c 6177 206f 7220 6167 7265 6564  le law or agreed
+00000130: 2074 6f20 696e 2077 7269 7469 6e67 2c20   to in writing, 
+00000140: 736f 6674 7761 7265 0a64 6973 7472 6962  software.distrib
+00000150: 7574 6564 2075 6e64 6572 2074 6865 204c  uted under the L
+00000160: 6963 656e 7365 2069 7320 6469 7374 7269  icense is distri
+00000170: 6275 7465 6420 6f6e 2061 6e20 2241 5320  buted on an "AS 
+00000180: 4953 2220 4241 5349 532c 0a57 4954 484f  IS" BASIS,.WITHO
+00000190: 5554 2057 4152 5241 4e54 4945 5320 4f52  UT WARRANTIES OR
+000001a0: 2043 4f4e 4449 5449 4f4e 5320 4f46 2041   CONDITIONS OF A
+000001b0: 4e59 204b 494e 442c 2065 6974 6865 7220  NY KIND, either 
+000001c0: 6578 7072 6573 7320 6f72 2069 6d70 6c69  express or impli
+000001d0: 6564 2e0a 5365 6520 7468 6520 4c69 6365  ed..See the Lice
+000001e0: 6e73 6520 666f 7220 7468 6520 7370 6563  nse for the spec
+000001f0: 6966 6963 206c 616e 6775 6167 6520 676f  ific language go
+00000200: 7665 726e 696e 6720 7065 726d 6973 7369  verning permissi
+00000210: 6f6e 7320 616e 640a 6c69 6d69 7461 7469  ons and.limitati
+00000220: 6f6e 7320 756e 6465 7220 7468 6520 4c69  ons under the Li
+00000230: 6365 6e73 652e 0a23 7d0a 7b7b 2074 6f63  cense..#}.{{ toc
+00000240: 7472 6565 2869 6e63 6c75 6465 6869 6464  tree(includehidd
+00000250: 656e 3d54 7275 6529 207d 7d0a            en=True) }}.
```

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/head.html` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/head.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,103 +1,108 @@
-00000000: 3c68 6561 643e 0a20 207b 252d 2062 6c6f  <head>.  {%- blo
-00000010: 636b 2061 6e61 6c79 7469 6373 2025 7d0a  ck analytics %}.
-00000020: 2020 7b23 2047 6f6f 676c 6541 6e61 6c79    {# GoogleAnaly
-00000030: 7469 6373 2023 7d0a 2020 3c21 2d2d 2047  tics #}.  <!-- G
-00000040: 6f6f 676c 6520 5461 6720 4d61 6e61 6765  oogle Tag Manage
-00000050: 7220 2d2d 3e0a 2020 3c73 6372 6970 743e  r -->.  <script>
-00000060: 2866 756e 6374 696f 6e28 772c 642c 732c  (function(w,d,s,
-00000070: 6c2c 6929 7b77 5b6c 5d3d 775b 6c5d 7c7c  l,i){w[l]=w[l]||
-00000080: 5b5d 3b77 5b6c 5d2e 7075 7368 287b 2767  [];w[l].push({'g
-00000090: 746d 2e73 7461 7274 273a 6e65 7720 4461  tm.start':new Da
-000000a0: 7465 2829 2e67 6574 5469 6d65 2829 2c65  te().getTime(),e
-000000b0: 7665 6e74 3a27 6774 6d2e 6a73 277d 293b  vent:'gtm.js'});
-000000c0: 7661 7220 663d 642e 6765 7445 6c65 6d65  var f=d.getEleme
-000000d0: 6e74 7342 7954 6167 4e61 6d65 2873 295b  ntsByTagName(s)[
-000000e0: 305d 2c6a 3d64 2e63 7265 6174 6545 6c65  0],j=d.createEle
-000000f0: 6d65 6e74 2873 292c 646c 3d6c 213d 2764  ment(s),dl=l!='d
-00000100: 6174 614c 6179 6572 273f 2726 6c3d 272b  ataLayer'?'&l='+
-00000110: 6c3a 2727 3b6a 2e61 7379 6e63 3d74 7275  l:'';j.async=tru
-00000120: 653b 6a2e 7372 633d 2768 7474 7073 3a2f  e;j.src='https:/
-00000130: 2f77 7777 2e67 6f6f 676c 6574 6167 6d61  /www.googletagma
-00000140: 6e61 6765 722e 636f 6d2f 6774 6d2e 6a73  nager.com/gtm.js
-00000150: 3f69 643d 272b 692b 646c 3b66 2e70 6172  ?id='+i+dl;f.par
-00000160: 656e 744e 6f64 652e 696e 7365 7274 4265  entNode.insertBe
-00000170: 666f 7265 286a 2c66 293b 7d29 2877 696e  fore(j,f);})(win
-00000180: 646f 772c 646f 6375 6d65 6e74 2c27 7363  dow,document,'sc
-00000190: 7269 7074 272c 2764 6174 614c 6179 6572  ript','dataLayer
-000001a0: 272c 2747 544d 2d50 505a 5051 3627 293b  ','GTM-PPZPQ6');
-000001b0: 3c2f 7363 7269 7074 3e0a 2020 3c21 2d2d  </script>.  <!--
-000001c0: 2045 6e64 2047 6f6f 676c 6520 5461 6720   End Google Tag 
-000001d0: 4d61 6e61 6765 7220 2d2d 3e0a 2020 7b25  Manager -->.  {%
-000001e0: 2d20 656e 6462 6c6f 636b 2025 7d0a 0a20  - endblock %}.. 
-000001f0: 207b 252d 2062 6c6f 636b 2068 746d 6c74   {%- block htmlt
-00000200: 6974 6c65 2025 7d0a 2020 2020 3c74 6974  itle %}.    <tit
-00000210: 6c65 3e7b 7b20 7469 746c 657c 7374 7269  le>{{ title|stri
-00000220: 7074 6167 737c 6520 7d7d 7b7b 2074 6974  ptags|e }}{{ tit
-00000230: 6c65 7375 6666 6978 207d 7d3c 2f74 6974  lesuffix }}</tit
-00000240: 6c65 3e0a 2020 7b25 2d20 656e 6462 6c6f  le>.  {%- endblo
-00000250: 636b 2025 7d0a 0a20 207b 252d 2062 6c6f  ck %}..  {%- blo
-00000260: 636b 206d 6574 6164 6174 6120 257d 0a20  ck metadata %}. 
-00000270: 207b 2320 4d45 5441 4441 5441 2023 7d0a   {# METADATA #}.
-00000280: 0a20 203c 6d65 7461 2063 6861 7273 6574  .  <meta charset
-00000290: 3d22 7574 662d 3822 3e0a 2020 3c21 2d2d  ="utf-8">.  <!--
-000002a0: 2054 7769 7474 6572 2042 6f6f 7473 7472   Twitter Bootstr
-000002b0: 6170 2076 6965 7770 6f72 7420 7365 7474  ap viewport sett
-000002c0: 696e 6720 2d2d 3e0a 2020 3c6d 6574 6120  ing -->.  <meta 
-000002d0: 6e61 6d65 3d22 7669 6577 706f 7274 2220  name="viewport" 
-000002e0: 636f 6e74 656e 743d 2277 6964 7468 3d64  content="width=d
-000002f0: 6576 6963 652d 7769 6474 682c 2069 6e69  evice-width, ini
-00000300: 7469 616c 2d73 6361 6c65 3d31 2c20 7368  tial-scale=1, sh
-00000310: 7269 6e6b 2d74 6f2d 6669 743d 6e6f 223e  rink-to-fit=no">
-00000320: 0a20 203c 212d 2d20 4635 206d 6574 6164  .  <!-- F5 metad
-00000330: 6174 6120 2d2d 3e0a 2020 3c6d 6574 6120  ata -->.  <meta 
-00000340: 6e61 6d65 3d22 7469 746c 6522 2063 6f6e  name="title" con
-00000350: 7465 6e74 3d22 7b7b 2074 6974 6c65 7c73  tent="{{ title|s
-00000360: 7472 6970 7461 6773 7c65 207d 7d22 2f3e  triptags|e }}"/>
-00000370: 0a20 203c 6d65 7461 206e 616d 653d 2270  .  <meta name="p
-00000380: 726f 6475 6374 2220 636f 6e74 656e 743d  roduct" content=
-00000390: 227b 7b20 7072 6f6a 6563 747c 7374 7269  "{{ project|stri
-000003a0: 7074 6167 737c 6520 7d7d 222f 3e0a 2020  ptags|e }}"/>.  
-000003b0: 3c6d 6574 6120 6e61 6d65 3d22 7665 7273  <meta name="vers
-000003c0: 696f 6e22 2063 6f6e 7465 6e74 3d22 7b7b  ion" content="{{
-000003d0: 2072 656c 6561 7365 7c73 7472 6970 7461   release|stripta
-000003e0: 6773 7c65 207d 7d22 2f3e 0a20 203c 6d65  gs|e }}"/>.  <me
-000003f0: 7461 206e 616d 653d 2275 7064 6174 6564  ta name="updated
-00000400: 5f64 6174 6522 2020 636f 6e74 656e 743d  _date"  content=
-00000410: 227b 7b20 6c61 7374 5f75 7064 6174 6564  "{{ last_updated
-00000420: 7c65 207d 7d22 2f3e 0a20 203c 6d65 7461  |e }}"/>.  <meta
-00000430: 206e 616d 653d 2261 7263 6869 7665 6422   name="archived"
-00000440: 2063 6f6e 7465 6e74 3d22 4172 6368 6976   content="Archiv
-00000450: 6564 2064 6f63 756d 656e 7473 2065 7863  ed documents exc
-00000460: 6c75 6465 6422 2f3e 0a20 203c 6d65 7461  luded"/>.  <meta
-00000470: 206e 616d 653d 2264 6f63 5f74 7970 6522   name="doc_type"
-00000480: 2063 6f6e 7465 6e74 3d22 4d61 6e75 616c   content="Manual
-00000490: 222f 3e0a 2020 3c6d 6574 6120 6e61 6d65  "/>.  <meta name
-000004a0: 3d22 6c69 6665 6379 636c 6522 2063 6f6e  ="lifecycle" con
-000004b0: 7465 6e74 3d22 7265 6c65 6173 6522 2f3e  tent="release"/>
-000004c0: 0a20 203c 6d65 7461 206e 616d 653d 227b  .  <meta name="{
-000004d0: 7b20 7072 6f6a 6563 747c 7374 7269 7074  { project|stript
-000004e0: 6167 737c 6520 7d7d 2220 636f 6e74 656e  ags|e }}" conten
-000004f0: 743d 227b 7b20 7265 6c65 6173 657c 7374  t="{{ release|st
-00000500: 7269 7074 6167 737c 6520 7d7d 222f 3e0a  riptags|e }}"/>.
-00000510: 0a7b 2520 6966 2028 7468 656d 655f 7665  .{% if (theme_ve
-00000520: 7273 696f 6e5f 7365 6c65 6374 6f72 2021  rsion_selector !
-00000530: 3d20 2746 616c 7365 2729 2025 7d0a 2020  = 'False') %}.  
-00000540: 3c21 2d2d 2056 6572 7369 6f6e 2073 656c  <!-- Version sel
-00000550: 6563 746f 7220 6d65 7461 2074 6167 732d  ector meta tags-
-00000560: 2d3e 0a20 203c 6d65 7461 206e 616d 653d  ->.  <meta name=
-00000570: 2276 6572 7369 6f6e 5f6d 6574 615f 7061  "version_meta_pa
-00000580: 7468 2220 636f 6e74 656e 743d 227b 7b20  th" content="{{ 
-00000590: 7665 7273 696f 6e5f 6d65 7461 5f70 6174  version_meta_pat
-000005a0: 6820 7d7d 223e 0a20 203c 6d65 7461 206e  h }}">.  <meta n
-000005b0: 616d 653d 2270 726f 6a65 6374 5f73 6166  ame="project_saf
-000005c0: 6522 2063 6f6e 7465 6e74 3d22 7b7b 2070  e" content="{{ p
-000005d0: 726f 6a65 6374 5f73 6166 6520 7d7d 223e  roject_safe }}">
-000005e0: 0a7b 252d 2065 6e64 6966 2025 7d0a 2020  .{%- endif %}.  
-000005f0: 7b7b 206d 6574 6174 6167 7320 7d7d 0a0a  {{ metatags }}..
-00000600: 2020 7b25 2d20 656e 6462 6c6f 636b 2025    {%- endblock %
-00000610: 7d0a 0a20 207b 2320 4641 5649 434f 4e20  }..  {# FAVICON 
-00000620: 237d 0a20 203c 6c69 6e6b 2068 7265 663d  #}.  <link href=
-00000630: 2268 7474 7073 3a2f 2f63 646e 2e66 352e  "https://cdn.f5.
-00000640: 636f 6d2f 6661 7669 636f 6e2e 6963 6f22  com/favicon.ico"
-00000650: 2072 656c 3d22 6963 6f6e 223e 0a0a 3c2f   rel="icon">..</
-00000660: 6865 6164 3e                             head>
+00000000: 3c21 444f 4354 5950 4520 6874 6d6c 3e0a  <!DOCTYPE html>.
+00000010: 0a3c 6865 6164 3e0a 2020 7b25 2d20 626c  .<head>.  {%- bl
+00000020: 6f63 6b20 616e 616c 7974 6963 7320 257d  ock analytics %}
+00000030: 0a20 207b 2320 476f 6f67 6c65 416e 616c  .  {# GoogleAnal
+00000040: 7974 6963 7320 237d 0a20 203c 212d 2d20  ytics #}.  <!-- 
+00000050: 476f 6f67 6c65 2054 6167 204d 616e 6167  Google Tag Manag
+00000060: 6572 202d 2d3e 0a20 203c 7363 7269 7074  er -->.  <script
+00000070: 3e28 6675 6e63 7469 6f6e 2028 772c 2064  >(function (w, d
+00000080: 2c20 732c 206c 2c20 6929 207b 2077 5b6c  , s, l, i) { w[l
+00000090: 5d20 3d20 775b 6c5d 207c 7c20 5b5d 3b20  ] = w[l] || []; 
+000000a0: 775b 6c5d 2e70 7573 6828 7b20 2767 746d  w[l].push({ 'gtm
+000000b0: 2e73 7461 7274 273a 206e 6577 2044 6174  .start': new Dat
+000000c0: 6528 292e 6765 7454 696d 6528 292c 2065  e().getTime(), e
+000000d0: 7665 6e74 3a20 2767 746d 2e6a 7327 207d  vent: 'gtm.js' }
+000000e0: 293b 2076 6172 2066 203d 2064 2e67 6574  ); var f = d.get
+000000f0: 456c 656d 656e 7473 4279 5461 674e 616d  ElementsByTagNam
+00000100: 6528 7329 5b30 5d2c 206a 203d 2064 2e63  e(s)[0], j = d.c
+00000110: 7265 6174 6545 6c65 6d65 6e74 2873 292c  reateElement(s),
+00000120: 2064 6c20 3d20 6c20 213d 2027 6461 7461   dl = l != 'data
+00000130: 4c61 7965 7227 203f 2027 266c 3d27 202b  Layer' ? '&l=' +
+00000140: 206c 203a 2027 273b 206a 2e61 7379 6e63   l : ''; j.async
+00000150: 203d 2074 7275 653b 206a 2e73 7263 203d   = true; j.src =
+00000160: 2027 6874 7470 733a 2f2f 7777 772e 676f   'https://www.go
+00000170: 6f67 6c65 7461 676d 616e 6167 6572 2e63  ogletagmanager.c
+00000180: 6f6d 2f67 746d 2e6a 733f 6964 3d27 202b  om/gtm.js?id=' +
+00000190: 2069 202b 2064 6c3b 2066 2e70 6172 656e   i + dl; f.paren
+000001a0: 744e 6f64 652e 696e 7365 7274 4265 666f  tNode.insertBefo
+000001b0: 7265 286a 2c20 6629 3b20 7d29 2877 696e  re(j, f); })(win
+000001c0: 646f 772c 2064 6f63 756d 656e 742c 2027  dow, document, '
+000001d0: 7363 7269 7074 272c 2027 6461 7461 4c61  script', 'dataLa
+000001e0: 7965 7227 2c20 2747 544d 2d50 505a 5051  yer', 'GTM-PPZPQ
+000001f0: 3627 293b 3c2f 7363 7269 7074 3e0a 2020  6');</script>.  
+00000200: 3c21 2d2d 2045 6e64 2047 6f6f 676c 6520  <!-- End Google 
+00000210: 5461 6720 4d61 6e61 6765 7220 2d2d 3e0a  Tag Manager -->.
+00000220: 2020 7b25 2d20 656e 6462 6c6f 636b 2025    {%- endblock %
+00000230: 7d0a 0a20 207b 252d 2062 6c6f 636b 2068  }..  {%- block h
+00000240: 746d 6c74 6974 6c65 2025 7d0a 2020 3c74  tmltitle %}.  <t
+00000250: 6974 6c65 3e7b 7b20 7469 746c 657c 7374  itle>{{ title|st
+00000260: 7269 7074 6167 737c 6520 7d7d 7b7b 2074  riptags|e }}{{ t
+00000270: 6974 6c65 7375 6666 6978 207d 7d3c 2f74  itlesuffix }}</t
+00000280: 6974 6c65 3e0a 2020 7b25 2d20 656e 6462  itle>.  {%- endb
+00000290: 6c6f 636b 2025 7d0a 0a20 207b 252d 2062  lock %}..  {%- b
+000002a0: 6c6f 636b 206d 6574 6164 6174 6120 257d  lock metadata %}
+000002b0: 0a20 207b 2320 4d45 5441 4441 5441 2023  .  {# METADATA #
+000002c0: 7d0a 0a20 203c 6d65 7461 2063 6861 7273  }..  <meta chars
+000002d0: 6574 3d22 7574 662d 3822 3e0a 2020 3c21  et="utf-8">.  <!
+000002e0: 2d2d 2054 7769 7474 6572 2042 6f6f 7473  -- Twitter Boots
+000002f0: 7472 6170 2076 6965 7770 6f72 7420 7365  trap viewport se
+00000300: 7474 696e 6720 2d2d 3e0a 2020 3c6d 6574  tting -->.  <met
+00000310: 6120 6e61 6d65 3d22 7669 6577 706f 7274  a name="viewport
+00000320: 2220 636f 6e74 656e 743d 2277 6964 7468  " content="width
+00000330: 3d64 6576 6963 652d 7769 6474 682c 2069  =device-width, i
+00000340: 6e69 7469 616c 2d73 6361 6c65 3d31 2c20  nitial-scale=1, 
+00000350: 7368 7269 6e6b 2d74 6f2d 6669 743d 6e6f  shrink-to-fit=no
+00000360: 223e 0a20 203c 212d 2d20 4635 206d 6574  ">.  <!-- F5 met
+00000370: 6164 6174 6120 2d2d 3e0a 2020 3c6d 6574  adata -->.  <met
+00000380: 6120 6e61 6d65 3d22 7469 746c 6522 2063  a name="title" c
+00000390: 6f6e 7465 6e74 3d22 7b7b 2074 6974 6c65  ontent="{{ title
+000003a0: 7c73 7472 6970 7461 6773 7c65 207d 7d22  |striptags|e }}"
+000003b0: 202f 3e0a 2020 3c6d 6574 6120 6e61 6d65   />.  <meta name
+000003c0: 3d22 7072 6f64 7563 7422 2063 6f6e 7465  ="product" conte
+000003d0: 6e74 3d22 7b7b 2070 726f 6a65 6374 7c73  nt="{{ project|s
+000003e0: 7472 6970 7461 6773 7c65 207d 7d22 202f  triptags|e }}" /
+000003f0: 3e0a 2020 3c6d 6574 6120 6e61 6d65 3d22  >.  <meta name="
+00000400: 7665 7273 696f 6e22 2063 6f6e 7465 6e74  version" content
+00000410: 3d22 7b7b 2072 656c 6561 7365 7c73 7472  ="{{ release|str
+00000420: 6970 7461 6773 7c65 207d 7d22 202f 3e0a  iptags|e }}" />.
+00000430: 2020 3c6d 6574 6120 6e61 6d65 3d22 7570    <meta name="up
+00000440: 6461 7465 645f 6461 7465 2220 636f 6e74  dated_date" cont
+00000450: 656e 743d 227b 7b20 6c61 7374 5f75 7064  ent="{{ last_upd
+00000460: 6174 6564 7c65 207d 7d22 202f 3e0a 2020  ated|e }}" />.  
+00000470: 3c6d 6574 6120 6e61 6d65 3d22 6172 6368  <meta name="arch
+00000480: 6976 6564 2220 636f 6e74 656e 743d 2241  ived" content="A
+00000490: 7263 6869 7665 6420 646f 6375 6d65 6e74  rchived document
+000004a0: 7320 6578 636c 7564 6564 2220 2f3e 0a20  s excluded" />. 
+000004b0: 203c 6d65 7461 206e 616d 653d 2264 6f63   <meta name="doc
+000004c0: 5f74 7970 6522 2063 6f6e 7465 6e74 3d22  _type" content="
+000004d0: 4d61 6e75 616c 2220 2f3e 0a20 203c 6d65  Manual" />.  <me
+000004e0: 7461 206e 616d 653d 226c 6966 6563 7963  ta name="lifecyc
+000004f0: 6c65 2220 636f 6e74 656e 743d 2272 656c  le" content="rel
+00000500: 6561 7365 2220 2f3e 0a20 203c 6d65 7461  ease" />.  <meta
+00000510: 206e 616d 653d 227b 7b20 7072 6f6a 6563   name="{{ projec
+00000520: 747c 7374 7269 7074 6167 737c 6520 7d7d  t|striptags|e }}
+00000530: 2220 636f 6e74 656e 743d 227b 7b20 7265  " content="{{ re
+00000540: 6c65 6173 657c 7374 7269 7074 6167 737c  lease|striptags|
+00000550: 6520 7d7d 2220 2f3e 0a0a 2020 7b25 2069  e }}" />..  {% i
+00000560: 6620 2874 6865 6d65 5f76 6572 7369 6f6e  f (theme_version
+00000570: 5f73 656c 6563 746f 7220 213d 2027 4661  _selector != 'Fa
+00000580: 6c73 6527 2920 257d 0a20 203c 212d 2d20  lse') %}.  <!-- 
+00000590: 5665 7273 696f 6e20 7365 6c65 6374 6f72  Version selector
+000005a0: 206d 6574 6120 7461 6773 2d2d 3e0a 2020   meta tags-->.  
+000005b0: 3c6d 6574 6120 6e61 6d65 3d22 7665 7273  <meta name="vers
+000005c0: 696f 6e5f 6d65 7461 5f70 6174 6822 2063  ion_meta_path" c
+000005d0: 6f6e 7465 6e74 3d22 7b7b 2076 6572 7369  ontent="{{ versi
+000005e0: 6f6e 5f6d 6574 615f 7061 7468 207d 7d22  on_meta_path }}"
+000005f0: 3e0a 2020 3c6d 6574 6120 6e61 6d65 3d22  >.  <meta name="
+00000600: 7072 6f6a 6563 745f 7361 6665 2220 636f  project_safe" co
+00000610: 6e74 656e 743d 227b 7b20 7072 6f6a 6563  ntent="{{ projec
+00000620: 745f 7361 6665 207d 7d22 3e0a 2020 7b25  t_safe }}">.  {%
+00000630: 2d20 656e 6469 6620 257d 0a20 207b 7b20  - endif %}.  {{ 
+00000640: 6d65 7461 7461 6773 207d 7d0a 0a20 207b  metatags }}..  {
+00000650: 252d 2065 6e64 626c 6f63 6b20 257d 0a0a  %- endblock %}..
+00000660: 2020 7b23 2046 4156 4943 4f4e 2023 7d0a    {# FAVICON #}.
+00000670: 2020 3c6c 696e 6b20 6872 6566 3d22 6874    <link href="ht
+00000680: 7470 733a 2f2f 6364 6e2e 6635 2e63 6f6d  tps://cdn.f5.com
+00000690: 2f66 6176 6963 6f6e 2e69 636f 2220 7265  /favicon.ico" re
+000006a0: 6c3d 2269 636f 6e22 3e0a 0a3c 2f68 6561  l="icon">..</hea
+000006b0: 643e 0a                                  d>.
```

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/layout.html` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/layout.html`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/localtoc.html` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/localtoc.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-00000000: 7b23 0a20 436f 7079 7269 6768 7420 3230  {#. Copyright 20
-00000010: 3137 2046 3520 4e65 7477 6f72 6b73 0a0a  17 F5 Networks..
-00000020: 204c 6963 656e 7365 6420 756e 6465 7220   Licensed under 
-00000030: 7468 6520 4170 6163 6865 204c 6963 656e  the Apache Licen
-00000040: 7365 2c20 5665 7273 696f 6e20 322e 3020  se, Version 2.0 
-00000050: 2874 6865 2022 4c69 6365 6e73 6522 293b  (the "License");
-00000060: 0a20 796f 7520 6d61 7920 6e6f 7420 7573  . you may not us
-00000070: 6520 7468 6973 2066 696c 6520 6578 6365  e this file exce
-00000080: 7074 2069 6e20 636f 6d70 6c69 616e 6365  pt in compliance
-00000090: 2077 6974 6820 7468 6520 4c69 6365 6e73   with the Licens
-000000a0: 652e 0a20 596f 7520 6d61 7920 6f62 7461  e.. You may obta
-000000b0: 696e 2061 2063 6f70 7920 6f66 2074 6865  in a copy of the
-000000c0: 204c 6963 656e 7365 2061 740a 0a20 2020   License at..   
-000000d0: 2020 6874 7470 3a2f 2f77 7777 2e61 7061    http://www.apa
-000000e0: 6368 652e 6f72 672f 6c69 6365 6e73 6573  che.org/licenses
-000000f0: 2f4c 4943 454e 5345 2d32 2e30 0a0a 2055  /LICENSE-2.0.. U
-00000100: 6e6c 6573 7320 7265 7175 6972 6564 2062  nless required b
-00000110: 7920 6170 706c 6963 6162 6c65 206c 6177  y applicable law
-00000120: 206f 7220 6167 7265 6564 2074 6f20 696e   or agreed to in
-00000130: 2077 7269 7469 6e67 2c20 736f 6674 7761   writing, softwa
-00000140: 7265 0a20 6469 7374 7269 6275 7465 6420  re. distributed 
-00000150: 756e 6465 7220 7468 6520 4c69 6365 6e73  under the Licens
-00000160: 6520 6973 2064 6973 7472 6962 7574 6564  e is distributed
-00000170: 206f 6e20 616e 2022 4153 2049 5322 2042   on an "AS IS" B
-00000180: 4153 4953 2c0a 2057 4954 484f 5554 2057  ASIS,. WITHOUT W
-00000190: 4152 5241 4e54 4945 5320 4f52 2043 4f4e  ARRANTIES OR CON
-000001a0: 4449 5449 4f4e 5320 4f46 2041 4e59 204b  DITIONS OF ANY K
-000001b0: 494e 442c 2065 6974 6865 7220 6578 7072  IND, either expr
-000001c0: 6573 7320 6f72 2069 6d70 6c69 6564 2e0a  ess or implied..
-000001d0: 2053 6565 2074 6865 204c 6963 656e 7365   See the License
-000001e0: 2066 6f72 2074 6865 2073 7065 6369 6669   for the specifi
-000001f0: 6320 6c61 6e67 7561 6765 2067 6f76 6572  c language gover
-00000200: 6e69 6e67 2070 6572 6d69 7373 696f 6e73  ning permissions
-00000210: 2061 6e64 0a20 6c69 6d69 7461 7469 6f6e   and. limitation
-00000220: 7320 756e 6465 7220 7468 6520 4c69 6365  s under the Lice
-00000230: 6e73 652e 0a23 7d0a 0a7b 252d 2069 6620  nse..#}..{%- if 
-00000240: 6469 7370 6c61 795f 746f 6320 257d 0a20  display_toc %}. 
-00000250: 203c 7020 636c 6173 733d 2263 6170 7469   <p class="capti
-00000260: 6f6e 223e 0a20 2020 3c73 7061 6e20 636c  on">.   <span cl
-00000270: 6173 733d 2263 6170 7469 6f6e 2d74 6578  ass="caption-tex
-00000280: 7422 3e43 7572 7265 6e74 2050 6167 653c  t">Current Page<
-00000290: 2f73 7061 6e3e 0a20 203c 2f70 3e0a 2020  /span>.  </p>.  
-000002a0: 7b7b 2074 6f63 207d 7d0a 7b25 2d20 656e  {{ toc }}.{%- en
-000002b0: 6469 6620 257d 0a                        dif %}.
+00000000: 3c21 444f 4354 5950 4520 6874 6d6c 3e0a  <!DOCTYPE html>.
+00000010: 7b23 0a43 6f70 7972 6967 6874 2032 3031  {#.Copyright 201
+00000020: 3720 4635 204e 6574 776f 726b 730a 0a4c  7 F5 Networks..L
+00000030: 6963 656e 7365 6420 756e 6465 7220 7468  icensed under th
+00000040: 6520 4170 6163 6865 204c 6963 656e 7365  e Apache License
+00000050: 2c20 5665 7273 696f 6e20 322e 3020 2874  , Version 2.0 (t
+00000060: 6865 2022 4c69 6365 6e73 6522 293b 0a79  he "License");.y
+00000070: 6f75 206d 6179 206e 6f74 2075 7365 2074  ou may not use t
+00000080: 6869 7320 6669 6c65 2065 7863 6570 7420  his file except 
+00000090: 696e 2063 6f6d 706c 6961 6e63 6520 7769  in compliance wi
+000000a0: 7468 2074 6865 204c 6963 656e 7365 2e0a  th the License..
+000000b0: 596f 7520 6d61 7920 6f62 7461 696e 2061  You may obtain a
+000000c0: 2063 6f70 7920 6f66 2074 6865 204c 6963   copy of the Lic
+000000d0: 656e 7365 2061 740a 0a68 7474 703a 2f2f  ense at..http://
+000000e0: 7777 772e 6170 6163 6865 2e6f 7267 2f6c  www.apache.org/l
+000000f0: 6963 656e 7365 732f 4c49 4345 4e53 452d  icenses/LICENSE-
+00000100: 322e 300a 0a55 6e6c 6573 7320 7265 7175  2.0..Unless requ
+00000110: 6972 6564 2062 7920 6170 706c 6963 6162  ired by applicab
+00000120: 6c65 206c 6177 206f 7220 6167 7265 6564  le law or agreed
+00000130: 2074 6f20 696e 2077 7269 7469 6e67 2c20   to in writing, 
+00000140: 736f 6674 7761 7265 0a64 6973 7472 6962  software.distrib
+00000150: 7574 6564 2075 6e64 6572 2074 6865 204c  uted under the L
+00000160: 6963 656e 7365 2069 7320 6469 7374 7269  icense is distri
+00000170: 6275 7465 6420 6f6e 2061 6e20 2241 5320  buted on an "AS 
+00000180: 4953 2220 4241 5349 532c 0a57 4954 484f  IS" BASIS,.WITHO
+00000190: 5554 2057 4152 5241 4e54 4945 5320 4f52  UT WARRANTIES OR
+000001a0: 2043 4f4e 4449 5449 4f4e 5320 4f46 2041   CONDITIONS OF A
+000001b0: 4e59 204b 494e 442c 2065 6974 6865 7220  NY KIND, either 
+000001c0: 6578 7072 6573 7320 6f72 2069 6d70 6c69  express or impli
+000001d0: 6564 2e0a 5365 6520 7468 6520 4c69 6365  ed..See the Lice
+000001e0: 6e73 6520 666f 7220 7468 6520 7370 6563  nse for the spec
+000001f0: 6966 6963 206c 616e 6775 6167 6520 676f  ific language go
+00000200: 7665 726e 696e 6720 7065 726d 6973 7369  verning permissi
+00000210: 6f6e 7320 616e 640a 6c69 6d69 7461 7469  ons and.limitati
+00000220: 6f6e 7320 756e 6465 7220 7468 6520 4c69  ons under the Li
+00000230: 6365 6e73 652e 0a23 7d0a 7b25 2d20 6966  cense..#}.{%- if
+00000240: 2064 6973 706c 6179 5f74 6f63 2025 7d0a   display_toc %}.
+00000250: 3c70 2063 6c61 7373 3d22 6361 7074 696f  <p class="captio
+00000260: 6e22 3e0a 2020 3c73 7061 6e20 636c 6173  n">.  <span clas
+00000270: 733d 2263 6170 7469 6f6e 2d74 6578 7422  s="caption-text"
+00000280: 3e43 7572 7265 6e74 2050 6167 653c 2f73  >Current Page</s
+00000290: 7061 6e3e 0a3c 2f70 3e0a 7b7b 2074 6f63  pan>.</p>.{{ toc
+000002a0: 207d 7d0a 7b25 2d20 656e 6469 6620 257d   }}.{%- endif %}
+000002b0: 0a                                       .
```

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/searchbox.html` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/searchbox.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+<!DOCTYPE html>
 {%- if pagename != "search" and builder != "singlehtml" %}
 <div id="searchbox" role="search">
   <form class="search" action="{{ pathto('search') }}" method="get">
     <input type="text" class="search" name="q" placeholder=" Search..." />
     <button type="submit" class="btn btn-info navbar-btn"><i class="fa fa-search"></i></button>
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
 </div>
 <script type="text/javascript">$('#searchbox').show(0);</script>
-{%- endif %}
+{%- endif %}
```

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/css/CoveoFullSearch.css` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/CoveoFullSearch.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/css/bootstrap-theme.css` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/css/bootstrap-theme.min.css` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/css/bootstrap.css` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/css/bootstrap.min.css` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/css/custom.css` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/custom.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/css/f5-theme.css` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/f5-theme.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/css/f5.css` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/css/f5.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/fonts/ProximaBold.woff` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/ProximaBold.woff`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/fonts/ProximaBold.woff2` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/ProximaBold.woff2`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/fonts/ProximaMedium.woff` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/ProximaMedium.woff`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/fonts/ProximaMedium.woff2` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/ProximaMedium.woff2`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/fonts/ProximaThin.woff` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/ProximaThin.woff`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/fonts/ProximaThin.woff2` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/ProximaThin.woff2`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.eot` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.svg` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.ttf` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff2` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/js/CoveoJsSearch.Lazy.min.js` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/CoveoJsSearch.Lazy.min.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/js/bootstrap.js` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/js/bootstrap.min.js` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/js/clouddocs.js` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/clouddocs.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/js/feedback.js` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/feedback.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/js/jquery.appear.js` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/jquery.appear.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme/static/js/printThis.js` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme/static/js/printThis.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme.egg-info/PKG-INFO` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f5-sphinx-theme
-Version: 2.4.0
+Version: 2.4.1
 Summary: Sphinx theme for F5 Networks
 Home-page: https://github.com/F5DevCentral/f5-sphinx-theme
 Author: F5 Networks
 Author-email: f5-sphinx-theme@f5.com
 License: Apache2
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
```

### Comparing `f5_sphinx_theme-2.4.0/f5_sphinx_theme.egg-info/SOURCES.txt` & `f5_sphinx_theme-2.4.1/f5_sphinx_theme.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -38,10 +38,9 @@
 f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff
 f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff2
 f5_sphinx_theme/static/js/CoveoJsSearch.Lazy.min.js
 f5_sphinx_theme/static/js/bootstrap.js
 f5_sphinx_theme/static/js/bootstrap.min.js
 f5_sphinx_theme/static/js/clouddocs.js
 f5_sphinx_theme/static/js/feedback.js
-f5_sphinx_theme/static/js/index.js
 f5_sphinx_theme/static/js/jquery.appear.js
 f5_sphinx_theme/static/js/printThis.js
```

### Comparing `f5_sphinx_theme-2.4.0/setup.py` & `f5_sphinx_theme-2.4.1/setup.py`

 * *Files identical despite different names*

